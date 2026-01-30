# MIRAI VISION LAB Website

![MIRAI VISION LAB](assets/img/lab_logo.jpg)

**A modern, responsive research lab website for MIRAI VISION LAB - Advanced Computer Vision and AI Research**

[![Jekyll](https://img.shields.io/badge/Jekyll-4.3-red.svg)](https://jekyllrb.com/)
[![License](https://img.shields.io/badge/License-MIT-blue.svg)](LICENSE)
[![GitHub Pages](https://img.shields.io/badge/Hosted%20on-GitHub%20Pages-green.svg)](https://pages.github.com/)

---

## 🔬 About

MIRAI VISION LAB is a cutting-edge research laboratory specializing in Computer Vision, Artificial Intelligence, and Machine Learning. This website showcases our research, team, publications, and achievements.

## ✨ Features

- **Responsive Design**: Optimized for desktop, tablet, and mobile devices
- **Modern UI/UX**: Clean, professional design with smooth animations
- **Dynamic Content**: 
  - Home page with lab statistics and latest news
  - Comprehensive about page
  - Team member profiles with grid layout
  - Research projects showcase
  - Publications page with BibTeX support
  - Achievements timeline
  - Photo gallery with lightbox
  - Contact form with Google Maps integration
- **SEO Optimized**: Meta tags and structured data
- **Fast Loading**: Lazy loading images and optimized assets
- **Dark Mode Support**: Built-in theme switching
- **Social Media Integration**: Links to lab's social profiles

## 📁 Project Structure

```
al-folio/
├── _config.yml                 # Main configuration file
├── _pages/                     # Site pages
│   ├── about.md               # Home/landing page
│   ├── about_lab.md          # Detailed about page
│   ├── team.md               # Team members page
│   ├── projects.md           # Research projects
│   ├── publications.md       # Publications list
│   ├── achievements.md       # Awards & achievements
│   ├── gallery.md            # Photo gallery
│   └── contact.md            # Contact page
├── _projects/                 # Individual project pages
├── _news/                     # News announcements
├── _bibliography/            # BibTeX files for publications
├── _data/                    # Data files (socials, cv, etc.)
├── _layouts/                 # Page templates
├── _includes/                # Reusable components
├── assets/                   # Static assets
│   ├── img/                 # Images
│   ├── css/                 # Stylesheets
│   ├── js/                  # JavaScript files
│   └── pdf/                 # PDF documents
└── _sass/                    # Sass stylesheets
```

## 🚀 Quick Start

### Prerequisites

- Ruby (version 2.7 or higher)
- RubyGems
- GCC and Make
- Jekyll and Bundler gems

### Local Development

1. **Clone the repository**
   ```bash
   git clone https://github.com/yourusername/miraivision-lab.git
   cd miraivision-lab
   ```

2. **Install dependencies**
   ```bash
   bundle install
   ```

3. **Run the development server**
   ```bash
   bundle exec jekyll serve
   ```

4. **View the site**
   Open your browser and navigate to `http://localhost:4000`

### Using Docker (Alternative)

```bash
docker-compose up
```

The site will be available at `http://localhost:8080`

## 📝 Customization Guide

### 1. Basic Configuration

Edit `_config.yml` to customize:

```yaml
title: MIRAI VISION LAB
description: Your lab description
url: https://yourusername.github.io
baseurl: # Leave blank for user/org pages, or /repo-name for project pages
email: info@miraivision.lab
```

### 2. Update Team Members

Edit `_pages/team.md` to add/modify team members:

```html
<div class="team-card">
  <img src="{{ '/assets/img/team/member.jpg' | relative_url }}" alt="Member Name">
  <div class="team-card-content">
    <h3 class="team-card-name">Member Name</h3>
    <p class="team-card-role">PhD Student</p>
    <p class="team-card-research">Research interests...</p>
  </div>
</div>
```

### 3. Add Research Projects

Create new files in `_projects/` directory:

```markdown
---
layout: page
title: Project Name
description: Brief description
img: assets/img/projects/project.jpg
importance: 1
category: ongoing
---

Project content here...
```

### 4. Add News/Announcements

Create files in `_news/` directory:

```markdown
---
layout: post
date: 2026-01-15 09:00:00
inline: true
---

Your announcement here!
```

### 5. Update Publications

Edit `_bibliography/papers.bib` with BibTeX entries:

```bibtex
@article{your_paper_2026,
  title={Your Paper Title},
  author={Author, Name and Another, Author},
  journal={Conference/Journal Name},
  year={2026}
}
```

### 6. Customize Images

Replace images in `assets/img/` with your own:
- `assets/img/lab_logo.jpg` - Lab logo
- `assets/img/team/*.jpg` - Team member photos
- `assets/img/projects/*.jpg` - Project images
- `assets/img/gallery/*.jpg` - Gallery photos

## 🌐 Deployment to GitHub Pages

### Option 1: User/Organization Page

1. **Create a repository named**: `username.github.io`
2. **Update `_config.yml`**:
   ```yaml
   url: https://username.github.io
   baseurl: # Leave blank
   ```
3. **Push to GitHub**:
   ```bash
   git add .
   git commit -m "Initial commit"
   git push origin main
   ```
4. **Enable GitHub Pages**: Go to Settings → Pages → Select main branch → Save

### Option 2: Project Page

1. **Create a repository** with any name (e.g., `miraivision-lab`)
2. **Update `_config.yml`**:
   ```yaml
   url: https://username.github.io
   baseurl: /miraivision-lab
   ```
3. **Push to GitHub** and enable Pages as above

### Automatic Deployment

GitHub Actions will automatically build and deploy your site when you push to the main branch. The workflow is configured in `.github/workflows/deploy.yml`.

## 📧 Contact Form Setup

The contact form uses [Formspree](https://formspree.io/). To set it up:

1. Create a free Formspree account
2. Get your form endpoint
3. Update the form action in `_pages/contact.md`:
   ```html
   <form action="https://formspree.io/f/YOUR_FORM_ID" method="POST">
   ```

## 🗺️ Google Maps Integration

Update the Google Maps embed in `_pages/contact.md`:

1. Go to [Google Maps](https://maps.google.com)
2. Search for your location
3. Click "Share" → "Embed a map"
4. Copy the iframe code
5. Replace the iframe src in `_pages/contact.md`

## 🎨 Styling Customization

### Colors

Edit `_sass/_variables.scss` to change colors:

```scss
$primary-color: #667eea;
$secondary-color: #764ba2;
$text-color: #2c3e50;
```

### Fonts

Update fonts in `_config.yml` under `third_party_libraries` → `google_fonts`

## 📱 Social Media Links

Update `_data/socials.yml`:

```yaml
email: info@miraivision.lab
github_username: miraivisionlab
twitter_username: miraivisionlab
linkedin_username: company/miraivisionlab
```

## 🔧 Advanced Configuration

### Analytics

Add Google Analytics in `_config.yml`:

```yaml
google_analytics: G-XXXXXXXXXX
```

### SEO

Update meta tags in `_config.yml`:

```yaml
keywords: computer vision, AI, machine learning, research
description: Your lab description
```

### Custom Domain

1. Add a `CNAME` file to the root with your domain
2. Configure DNS settings with your domain provider
3. Enable HTTPS in GitHub Pages settings

## 📚 Content Guidelines

### Adding Images

- **Recommended sizes**:
  - Team photos: 300x300px (square)
  - Project images: 1200x800px
  - Gallery photos: 1920x1080px
- **Format**: JPG for photos, PNG for graphics
- **Optimization**: Compress images before uploading

### Writing Style

- Use clear, accessible language
- Include alt text for all images
- Keep paragraphs short and scannable
- Use headings to structure content

## 🐛 Troubleshooting

### Build Errors

```bash
# Clear cache and rebuild
bundle exec jekyll clean
bundle exec jekyll build
```

### Dependency Issues

```bash
# Update dependencies
bundle update
```

### Local Server Issues

```bash
# Kill existing process
killall -9 jekyll
# Restart server
bundle exec jekyll serve
```

## 📄 License

This project is licensed under the MIT License - see the [LICENSE](LICENSE) file for details.

## 🙏 Acknowledgments

Built on the [al-folio](https://github.com/alshedivat/al-folio) theme framework.

## 📞 Support

For questions or issues:
- Email: info@miraivision.lab
- GitHub Issues: [Create an issue](https://github.com/yourusername/miraivision-lab/issues)

## 🔄 Updates

Keep your site updated:

```bash
git pull origin main
bundle update
```

---

**Made with ❤️ by MIRAI VISION LAB**

*Last Updated: January 2026*
