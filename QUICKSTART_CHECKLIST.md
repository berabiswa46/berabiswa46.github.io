# 🚀 MIRAI VISION LAB Website - Quick Start Checklist

## Before You Begin

- [ ] Read `README_MIRAIVISION.md` for complete documentation
- [ ] Read `DEPLOYMENT_GUIDE.md` for step-by-step instructions
- [ ] Read `IMPLEMENTATION_SUMMARY.md` to understand what's been built

---

## Phase 1: Content Preparation (1-2 hours)

### Gather Information

- [ ] Lab description and mission statement
- [ ] Research focus areas descriptions
- [ ] Professor names, bios, photos, contact info, websites
- [ ] Student names, roles, research areas, emails
- [ ] Project titles and descriptions
- [ ] Publication BibTeX entries
- [ ] Award and grant information
- [ ] Lab photos (events, equipment, team)
- [ ] Contact details (address, phone, email)

### Prepare Images

- [ ] Lab logo (recommended: 500x500px)
- [ ] Professor photos (300x300px, square)
- [ ] Team member photos (300x300px, square)
- [ ] Project images (1200x800px)
- [ ] Gallery photos (1920x1080px)
- [ ] Compress all images (use https://tinypng.com or similar)

---

## Phase 2: Configuration (30 minutes)

### Update `_config.yml`

- [ ] Line 5: Change URL to your GitHub Pages URL
- [ ] Line 6: Set `baseurl` (blank for user site, /repo-name for project site)
- [ ] Verify title, description, keywords
- [ ] Update contact email

### Update `_data/socials.yml`

- [ ] Add lab email address
- [ ] Add GitHub username/organization
- [ ] Add Twitter handle
- [ ] Add LinkedIn company page
- [ ] Add YouTube channel
- [ ] Add Google Scholar ID (when available)

---

## Phase 3: Content Updates (2-3 hours)

### Home Page (`_pages/about.md`)

- [ ] Update mission statement
- [ ] Update quick stats (publications, team members, projects count)
- [ ] Update profile info (address, contact)
- [ ] Add lab logo image to `assets/img/`

### About Page (`_pages/about_lab.md`)

- [ ] Customize vision and mission
- [ ] Update research focus descriptions
- [ ] Add lab history milestones with actual dates
- [ ] Update facilities and equipment details
- [ ] Update collaboration partners

### Team Page (`_pages/team.md`)

- [ ] Replace Professor 1 information (name, bio, research interests, contact, website)
- [ ] Replace Professor 2 information
- [ ] Add actual PhD student information (repeat for each student)
- [ ] Add actual M.Tech student information
- [ ] Add actual M.Sc student information
- [ ] Add actual Project student information
- [ ] Upload all team photos to `assets/img/team/`
- [ ] Update image paths in team cards

### Projects (`_projects/*.md`)

- [ ] Update `1_project.md` (Medical AI) with actual project details OR create your own
- [ ] Update `2_project.md` (Autonomous Vehicles) OR create your own
- [ ] Update `3_project.md` to `9_project.md` with actual projects OR delete unused ones
- [ ] Add project images to `assets/img/projects/`
- [ ] Update funding information
- [ ] Update team member lists

### Publications (`_bibliography/papers.bib`)

- [ ] Delete example entries (Einstein papers)
- [ ] Add your actual publications in BibTeX format
- [ ] Mark featured papers with `selected={true}`
- [ ] Add PDF files to `assets/pdf/` (optional)
- [ ] Add code links (optional)

### Achievements (`_pages/achievements.md`)

- [ ] Update "Impact at a Glance" stats (papers, funding, awards, patents)
- [ ] Replace award cards with actual awards
- [ ] Update grant timeline with actual grants
- [ ] Update media coverage with actual articles
- [ ] Update patent information
- [ ] Update competition wins

### Gallery (`_pages/gallery.md`)

- [ ] Add actual event photos to `assets/img/gallery/`
- [ ] Update gallery items with real images
- [ ] Update titles and dates
- [ ] Adjust categories as needed
- [ ] Delete unused placeholder items

### Contact (`_pages/contact.md`)

- [ ] Update lab address
- [ ] Update email addresses (general, director, collaborations)
- [ ] Update phone numbers
- [ ] Update office hours
- [ ] Set up Formspree account at https://formspree.io
- [ ] Get form endpoint and update form action
- [ ] Update Google Maps embed with actual location
- [ ] Update social media links
- [ ] Update directions section

### News (`_news/`)

- [ ] Update `announcement_1.md` to `announcement_6.md` with real news
- [ ] Create additional announcement files as needed
- [ ] Use correct dates
- [ ] Set `inline: true` for short announcements
- [ ] Set `inline: false` and add title for longer posts

---

## Phase 4: External Services Setup (30 minutes)

### Formspree (Contact Form)

- [ ] Create account: https://formspree.io
- [ ] Create new form
- [ ] Copy form endpoint ID
- [ ] Update in `_pages/contact.md`: `https://formspree.io/f/YOUR_FORM_ID`

### Google Maps

- [ ] Go to Google Maps: https://maps.google.com
- [ ] Search for your lab location
- [ ] Click Share → Embed a map
- [ ] Copy iframe code
- [ ] Replace iframe in `_pages/contact.md`

### Google Analytics (Optional)

- [ ] Create GA4 property: https://analytics.google.com
- [ ] Get measurement ID (G-XXXXXXXXXX)
- [ ] Add to `_config.yml`: `google_analytics: G-XXXXXXXXXX`

---

## Phase 5: Local Testing (30 minutes)

### Install and Run

```bash
# Navigate to project
cd /media/voyager/ssd1tb/miraivision_lab_site/al-folio

# Install dependencies (first time only)
bundle install

# Start server
bundle exec jekyll serve

# Open browser to http://localhost:4000
```

### Test Checklist

- [ ] Home page loads correctly
- [ ] All navigation menu links work
- [ ] About page displays properly
- [ ] Team page shows all members
- [ ] Projects page displays correctly
- [ ] Publications render (if any added)
- [ ] Achievements page loads
- [ ] Gallery displays and filters work
- [ ] Lightbox opens when clicking gallery images
- [ ] Contact page shows form
- [ ] Google Maps displays
- [ ] All images load
- [ ] Mobile responsive (resize browser)
- [ ] No broken links
- [ ] No console errors (F12 → Console)

---

## Phase 6: Git & GitHub Setup (15 minutes)

### Create Repository

- [ ] Go to https://github.com/new
- [ ] Create repository:
  - Option A: `username.github.io` (user/org site)
  - Option B: `miraivision-lab` (project site)
- [ ] Make it public
- [ ] Don't initialize with README

### Connect and Push

```bash
# Check git status
git status

# Initialize if needed
git init

# Add remote (replace with your URL)
git remote add origin https://github.com/username/your-repo.git

# Or update existing remote
git remote set-url origin https://github.com/username/your-repo.git

# Add all files
git add .

# Commit
git commit -m "Initial MIRAI VISION LAB website"

# Push
git branch -M main
git push -u origin main
```

---

## Phase 7: GitHub Pages Deployment (10 minutes)

### Enable GitHub Pages

- [ ] Go to repository on GitHub
- [ ] Click Settings
- [ ] Scroll to Pages section (left sidebar)
- [ ] Under "Source":
  - Branch: Select `main`
  - Folder: Select `/ (root)`
- [ ] Click Save
- [ ] Wait 2-5 minutes for deployment

### Verify Deployment

- [ ] Check Actions tab for green checkmark
- [ ] Visit your site:
  - User site: `https://username.github.io`
  - Project site: `https://username.github.io/repo-name`
- [ ] Test all pages on live site
- [ ] Test contact form submission
- [ ] Check mobile view

---

## Phase 8: Post-Deployment (30 minutes)

### SEO & Search Engines

- [ ] Submit to Google Search Console: https://search.google.com/search-console
- [ ] Submit to Bing Webmaster: https://www.bing.com/webmasters
- [ ] Verify sitemap: `https://yoursite.com/sitemap.xml`
- [ ] Check robots.txt: `https://yoursite.com/robots.txt`

### Social Media

- [ ] Create Twitter account
- [ ] Create LinkedIn company page
- [ ] Create GitHub organization (optional)
- [ ] Create YouTube channel
- [ ] Update all social links in `_data/socials.yml`
- [ ] Push changes

### Testing

- [ ] Test on real mobile device
- [ ] Test on tablet
- [ ] Test in different browsers (Chrome, Firefox, Safari, Edge)
- [ ] Have someone else review the site
- [ ] Fix any issues found

### Performance

- [ ] Check PageSpeed Insights: https://pagespeed.web.dev/
- [ ] Optimize any large images
- [ ] Verify lazy loading works

---

## Phase 9: Launch Announcement (Optional)

- [ ] Prepare launch announcement
- [ ] Share on lab social media
- [ ] Send email to department
- [ ] Update lab email signature with URL
- [ ] Add to relevant directories

---

## Maintenance Schedule

### Daily
- [ ] Check for form submissions

### Weekly
- [ ] Add new announcements
- [ ] Respond to inquiries

### Monthly
- [ ] Add new publications
- [ ] Update project progress
- [ ] Add gallery photos

### Quarterly
- [ ] Review all content for accuracy
- [ ] Update team members
- [ ] Check for broken links
- [ ] Update achievements

---

## Common Issues & Solutions

**Site not updating after push?**
```bash
# Clear cache and rebuild
git push origin main --force
# Wait 2-5 minutes
# Hard refresh browser (Ctrl+Shift+R)
```

**Images not loading?**
- Check file paths use `{{ '/assets/img/...' | relative_url }}`
- Verify images exist in correct folder
- Check image file names (case-sensitive)

**Contact form not working?**
- Verify Formspree endpoint is correct
- Check form is active in Formspree dashboard
- Test on live site (won't work locally)

**Build failing?**
- Check Actions tab for errors
- Verify YAML syntax in front matter
- Run `bundle exec jekyll build` locally

---

## Resources

- 📖 Full Documentation: `README_MIRAIVISION.md`
- 🚀 Deployment Guide: `DEPLOYMENT_GUIDE.md`
- 📊 Implementation Summary: `IMPLEMENTATION_SUMMARY.md`
- 🌐 Jekyll Docs: https://jekyllrb.com/docs/
- 💻 GitHub Pages: https://docs.github.com/pages

---

## Success Criteria

Your site is ready when:
- ✅ All pages load without errors
- ✅ All content is updated (no placeholders)
- ✅ All images display correctly
- ✅ Contact form works
- ✅ Mobile responsive
- ✅ Deployed to GitHub Pages
- ✅ Analytics configured (if desired)
- ✅ SEO submitted
- ✅ Social media linked

---

**Estimated Total Time: 5-7 hours**

- Content Preparation: 1-2 hours
- Configuration: 30 minutes
- Content Updates: 2-3 hours
- External Services: 30 minutes
- Local Testing: 30 minutes
- Git & GitHub: 15 minutes
- Deployment: 10 minutes
- Post-Deployment: 30 minutes

---

**Questions?** Review the documentation files or check Jekyll/GitHub Pages documentation.

**Ready to launch?** Follow this checklist step by step, and you'll have a professional research lab website live in less than a day!

---

**Last Updated: January 29, 2026**
