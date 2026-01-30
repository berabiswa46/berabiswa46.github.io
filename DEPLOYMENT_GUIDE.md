# MIRAI VISION LAB Website - Complete Deployment Guide

## 📋 Table of Contents

1. [Prerequisites](#prerequisites)
2. [Initial Setup](#initial-setup)
3. [Content Customization](#content-customization)
4. [GitHub Pages Deployment](#github-pages-deployment)
5. [Domain Configuration](#domain-configuration)
6. [Post-Deployment](#post-deployment)
7. [Maintenance](#maintenance)
8. [Troubleshooting](#troubleshooting)

---

## Prerequisites

### Required Software

1. **Git** - Version control
   ```bash
   # Check if installed
   git --version
   
   # Install on Ubuntu/Debian
   sudo apt-get install git
   
   # Install on macOS
   brew install git
   ```

2. **Ruby** (2.7 or higher)
   ```bash
   # Check version
   ruby --version
   
   # Install on Ubuntu/Debian
   sudo apt-get install ruby-full
   
   # Install on macOS
   brew install ruby
   ```

3. **Bundler**
   ```bash
   gem install bundler
   ```

### Required Accounts

- GitHub account
- (Optional) Custom domain registrar account
- (Optional) Formspree account for contact form
- (Optional) Google Analytics account

---

## Initial Setup

### Step 1: Repository Setup

1. **Create GitHub Repository**
   - Go to https://github.com/new
   - Repository name options:
     - `username.github.io` (for user/org site)
     - `miraivision-lab` (for project site)
   - Make it public
   - Don't initialize with README

2. **Clone and Setup**
   ```bash
   # Navigate to your local copy
   cd /media/voyager/ssd1tb/miraivision_lab_site/al-folio
   
   # Initialize git (if not already)
   git init
   
   # Add remote
   git remote add origin https://github.com/username/your-repo-name.git
   
   # Or if already has remote
   git remote set-url origin https://github.com/username/your-repo-name.git
   ```

### Step 2: Install Dependencies

```bash
# Install Ruby gems
bundle install

# If you encounter permission errors
bundle install --path vendor/bundle
```

### Step 3: Local Testing

```bash
# Start development server
bundle exec jekyll serve

# Server will run at http://localhost:4000
# Press Ctrl+C to stop
```

---

## Content Customization

### 1. Basic Site Configuration

Edit `_config.yml`:

```yaml
# Site Information
title: MIRAI VISION LAB
description: Your updated description
url: https://username.github.io  # Your GitHub Pages URL
baseurl: # For user site, leave blank. For project site: /repo-name

# Contact
email: info@miraivision.lab

# Social Media
# Update in _data/socials.yml
```

### 2. Update Team Members

**File:** `_pages/team.md`

Replace placeholder content with actual team information:

```html
<!-- For each team member -->
<div class="team-card">
  <img src="{{ '/assets/img/team/john_doe.jpg' | relative_url }}" alt="John Doe">
  <div class="team-card-content">
    <h3 class="team-card-name">Dr. John Doe</h3>
    <p class="team-card-role">PhD Student (Year 2)</p>
    <p class="team-card-research">
      <strong>Research Area:</strong> Deep Learning for Medical Imaging
    </p>
    <div class="team-card-contact">
      <a href="mailto:john.doe@university.edu">Email</a>
      <a href="https://scholar.google.com/..." target="_blank">Scholar</a>
    </div>
  </div>
</div>
```

### 3. Add Team Photos

1. Prepare photos (recommended: 300x300px, square)
2. Save to `assets/img/team/`
3. Update image paths in `_pages/team.md`

### 4. Update Research Projects

Create/edit files in `_projects/`:

```markdown
---
layout: page
title: Your Project Title
description: Brief one-line description
img: assets/img/projects/your_project.jpg
importance: 1
category: ongoing  # or completed
related_publications: true
---

## Project Overview
Your detailed project description here...

### Key Objectives
- Objective 1
- Objective 2

### Team Members
- Dr. Jane Smith
- PhD Student Name
```

### 5. Add Publications

Edit `_bibliography/papers.bib`:

```bibtex
@article{smith2026medical,
  title={Advanced Medical Image Analysis},
  author={Smith, Jane and Doe, John},
  journal={CVPR},
  year={2026},
  selected={true},  # Mark as featured
  pdf={paper.pdf},  # Optional: Add PDF to assets/pdf/
  code={https://github.com/...},  # Optional: GitHub link
  abstract={Your abstract here...}
}
```

### 6. Update News/Announcements

Create files in `_news/`:

```markdown
---
layout: post
date: 2026-01-15 09:00:00
inline: true  # Short announcement
related_posts: false
---

🎉 Your announcement text here!
```

For longer announcements, set `inline: false` and add title:

```markdown
---
layout: post
title: Major Research Breakthrough
date: 2026-01-15 09:00:00
inline: false
---

Full announcement content with formatting...
```

### 7. Gallery Images

1. Add photos to `assets/img/gallery/`
2. Update `_pages/gallery.md` with new images:

```html
<div class="gallery-item" data-category="events">
  <span class="category-badge">Events</span>
  <img src="{{ '/assets/img/gallery/your_image.jpg' | relative_url }}" 
       alt="Event Description" loading="lazy">
  <div class="gallery-overlay">
    <h3 class="gallery-title">Event Name</h3>
    <p class="gallery-date">January 15, 2026</p>
  </div>
</div>
```

### 8. Contact Information

Edit `_pages/contact.md`:

- Update address, phone, email
- Configure Google Maps embed
- Set up Formspree (see below)

**Formspree Setup:**
1. Create account at https://formspree.io
2. Create new form
3. Copy form endpoint
4. Update form action:
   ```html
   <form action="https://formspree.io/f/YOUR_FORM_ID" method="POST">
   ```

---

## GitHub Pages Deployment

### Method 1: Automatic Deployment (Recommended)

1. **Commit all changes**
   ```bash
   git add .
   git commit -m "Initial MIRAI VISION LAB site setup"
   ```

2. **Push to GitHub**
   ```bash
   git branch -M main
   git push -u origin main
   ```

3. **Enable GitHub Pages**
   - Go to repository Settings
   - Navigate to "Pages" section
   - Source: Deploy from a branch
   - Branch: Select `main` and `/root`
   - Click Save

4. **Wait for deployment** (2-5 minutes)
   - Check Actions tab for build status
   - Site will be live at: `https://username.github.io` or `https://username.github.io/repo-name`

### Method 2: Manual Build

```bash
# Build the site locally
JEKYLL_ENV=production bundle exec jekyll build

# The _site folder contains the built site
# You can deploy this folder to any static hosting service
```

---

## Domain Configuration

### Using Custom Domain

1. **Purchase domain** (e.g., miraivision.lab)

2. **Add CNAME file** to repository root:
   ```
   www.miraivision.lab
   ```

3. **Configure DNS** with your provider:
   ```
   Type: CNAME
   Host: www
   Value: username.github.io
   
   Type: A (add all four)
   Host: @
   Values:
   185.199.108.153
   185.199.109.153
   185.199.110.153
   185.199.111.153
   ```

4. **Update GitHub Pages settings**
   - Settings → Pages
   - Custom domain: www.miraivision.lab
   - Enforce HTTPS: ✓

5. **Wait for DNS propagation** (up to 24 hours)

---

## Post-Deployment

### 1. Verify Deployment

Check these items:
- [ ] Home page loads correctly
- [ ] All navigation links work
- [ ] Images display properly
- [ ] Contact form works (test submission)
- [ ] Responsive design on mobile
- [ ] Publications render correctly
- [ ] Gallery lightbox functions
- [ ] Social media links open correctly

### 2. Set Up Analytics

**Google Analytics:**

1. Create GA4 property
2. Get measurement ID (G-XXXXXXXXXX)
3. Add to `_config.yml`:
   ```yaml
   google_analytics: G-XXXXXXXXXX
   ```
4. Commit and push

### 3. SEO Optimization

**sitemap.xml**: Generated automatically

**robots.txt**: Already configured

**Submit to search engines:**
- Google Search Console: https://search.google.com/search-console
- Bing Webmaster Tools: https://www.bing.com/webmasters

### 4. Social Media Setup

Create profiles and update links:
- Twitter/X
- LinkedIn
- GitHub Organization
- YouTube Channel
- ResearchGate
- Google Scholar

Update `_data/socials.yml` with actual handles.

---

## Maintenance

### Regular Updates

**Weekly:**
- Add news announcements
- Update project progress

**Monthly:**
- Add new publications
- Update team member info
- Add gallery photos

**Quarterly:**
- Review and update research descriptions
- Check for broken links
- Update achievement timeline

### Making Changes

```bash
# Pull latest changes
git pull origin main

# Make your edits
# ...

# Test locally
bundle exec jekyll serve

# Commit and push
git add .
git commit -m "Update: description of changes"
git push origin main

# Site auto-deploys in 2-5 minutes
```

### Dependency Updates

```bash
# Update gems
bundle update

# Update to latest al-folio features
git remote add upstream https://github.com/alshedivat/al-folio.git
git fetch upstream
git merge upstream/main
```

---

## Troubleshooting

### Build Fails

**Check build log:**
- Go to Actions tab
- Click on failed workflow
- Review error messages

**Common issues:**

1. **Jekyll version mismatch**
   ```bash
   bundle update jekyll
   ```

2. **Missing dependencies**
   ```bash
   bundle install
   ```

3. **Syntax errors**
   - Check YAML front matter
   - Validate markdown syntax
   - Look for unclosed HTML tags

### Images Not Loading

1. **Check file paths**
   - Use relative URLs: `{{ '/assets/img/photo.jpg' | relative_url }}`
   - Not absolute: `/assets/img/photo.jpg`

2. **Verify file exists**
   ```bash
   ls -la assets/img/team/
   ```

3. **Check file size** (keep under 1MB for web)

### Site Not Updating

1. **Clear browser cache** (Ctrl+Shift+R)

2. **Check deployment status**
   - GitHub Actions should show green checkmark

3. **Verify changes pushed**
   ```bash
   git status
   git log
   ```

### Contact Form Not Working

1. **Verify Formspree setup**
   - Check form endpoint URL
   - Confirm form is active in Formspree dashboard

2. **Test locally**
   - Forms won't submit locally
   - Must test on live site

### Performance Issues

1. **Optimize images**
   ```bash
   # Use ImageMagick to resize
   mogrify -resize 1920x1080 -quality 85 assets/img/gallery/*.jpg
   ```

2. **Enable lazy loading**
   - Already implemented in gallery

3. **Check PageSpeed Insights**
   - Visit: https://pagespeed.web.dev/

---

## Quick Reference Commands

```bash
# Local development
bundle exec jekyll serve

# Clean build
bundle exec jekyll clean
bundle exec jekyll build

# Update dependencies
bundle update

# Git workflow
git status
git add .
git commit -m "Your message"
git push origin main

# Check site status
git log --oneline
git remote -v
```

---

## Support Resources

- **Jekyll Documentation**: https://jekyllrb.com/docs/
- **GitHub Pages**: https://docs.github.com/pages
- **al-folio Theme**: https://github.com/alshedivat/al-folio
- **Markdown Guide**: https://www.markdownguide.org/
- **Liquid Template**: https://shopify.github.io/liquid/

---

## Checklist for Go-Live

- [ ] All content reviewed and updated
- [ ] Team member photos added
- [ ] Research projects documented
- [ ] Publications added to bibliography
- [ ] Contact information verified
- [ ] Social media links updated
- [ ] Google Maps configured
- [ ] Contact form tested
- [ ] Analytics configured
- [ ] Custom domain configured (if applicable)
- [ ] Mobile responsive checked
- [ ] All links tested
- [ ] SEO meta tags verified
- [ ] Submitted to search engines
- [ ] README documentation complete

---

**Last Updated: January 29, 2026**

For additional assistance, contact: info@miraivision.lab
