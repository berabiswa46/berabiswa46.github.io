# Content Templates for MIRAI VISION LAB Website

Quick copy-paste templates for adding new content to your website.

---

## 📰 News Announcement Templates

### Short Inline Announcement

```markdown
---
layout: post
date: 2026-MM-DD HH:MM:00
inline: true
related_posts: false
---

🎉 Your short announcement text here! Can include emojis and links.
```

### Detailed Announcement with Title

```markdown
---
layout: post
title: Your Announcement Title
date: 2026-MM-DD HH:MM:00
inline: false
related_posts: false
---

First paragraph of your announcement...

***

## Additional Details

More content here...

**Key Points:**
- Point 1
- Point 2
- Point 3

For more information, contact [email@lab.edu](mailto:email@lab.edu)
```

---

## 👥 Team Member Templates

### Professor/Faculty Card

```html
<div class="professor-card">
  <img src="{{ '/assets/img/team/name.jpg' | relative_url }}" alt="Dr. Name" class="professor-image">
  <h3 class="professor-name">Dr. [Full Name]</h3>
  <p class="professor-title">Professor & Lab Director</p>
  
  <div class="professor-bio">
    <p>Brief bio paragraph highlighting expertise, background, and achievements...</p>
  </div>
  
  <div class="professor-interests">
    <h4>Research Interests:</h4>
    <ul>
      <li>Research Area 1</li>
      <li>Research Area 2</li>
      <li>Research Area 3</li>
      <li>Research Area 4</li>
    </ul>
  </div>
  
  <div class="professor-contact">
    <a href="mailto:professor@university.edu">Email</a>
    <a href="https://scholar.google.com/citations?user=XXX" target="_blank">Google Scholar</a>
    <a href="https://personal-website.com" target="_blank">Website</a>
  </div>
</div>
```

### Student Card (PhD/M.Tech/M.Sc/Project)

```html
<div class="team-card">
  <img src="{{ '/assets/img/team/student_name.jpg' | relative_url }}" alt="Student Name" class="team-card-image">
  <div class="team-card-content">
    <h3 class="team-card-name">[Full Name]</h3>
    <p class="team-card-role">PhD Student (Year 2)</p>
    <p class="team-card-research">
      <strong>Research Area:</strong> Specific research focus description
    </p>
    <div class="team-card-contact">
      <a href="mailto:student@university.edu">Email</a>
      <a href="https://scholar.google.com/..." target="_blank">Scholar</a>
      <a href="https://linkedin.com/in/..." target="_blank">LinkedIn</a>
    </div>
  </div>
</div>
```

---

## 🔬 Project Templates

### New Project File (create in `_projects/`)

Filename: `N_project_name.md` (where N is importance number)

```markdown
---
layout: page
title: Project Title
description: One-line description for project card
img: assets/img/projects/project_name.jpg
importance: 1
category: ongoing  # or: completed
related_publications: true
---

## Project Overview

Brief introduction to the project (2-3 paragraphs)...

### Key Objectives

- Objective 1
- Objective 2
- Objective 3

<div class="row">
    <div class="col-sm mt-3 mt-md-0">
        {% include figure.liquid loading="eager" path="assets/img/projects/image1.jpg" title="description" class="img-fluid rounded z-depth-1" %}
    </div>
    <div class="col-sm mt-3 mt-md-0">
        {% include figure.liquid loading="eager" path="assets/img/projects/image2.jpg" title="description" class="img-fluid rounded z-depth-1" %}
    </div>
</div>
<div class="caption">
    Caption explaining the images above
</div>

### Technical Approach

Description of methods and techniques...

1. **Method 1**: Explanation
2. **Method 2**: Explanation
3. **Method 3**: Explanation

### Current Results

- **Metric 1**: Value and explanation
- **Metric 2**: Value and explanation
- **Metric 3**: Value and explanation

### Team & Collaborators

**Lab Members:**
- Principal Investigator Name
- PhD Student Name
- M.Tech Student Name

**External Collaborators:**
- Institution/Company Name
- Partner Name

### Funding

- Funding Source 1: $XXX,XXX
- Funding Source 2: $XXX,XXX
- **Total**: $XXX,XXX

### Publications

{% cite bibtex_key_1 bibtex_key_2 %}

### Future Directions

- Next step 1
- Next step 2
- Next step 3

---

**Project Timeline**: Month YYYY - Month YYYY

**Status**: <span style="background: #28a745; color: white; padding: 4px 12px; border-radius: 4px;">Active</span>

**Contact**: [email@lab.edu](mailto:email@lab.edu)
```

---

## 📚 Publication (BibTeX) Templates

### Journal Article

```bibtex
@article{authorYEARkeyword,
  title={Full Paper Title},
  author={LastName1, FirstName1 and LastName2, FirstName2},
  journal={Journal Name},
  volume={XX},
  number={Y},
  pages={XXX--YYY},
  year={2026},
  publisher={Publisher Name},
  doi={10.XXXX/XXXXX},
  selected={true},
  pdf={paper.pdf},
  code={https://github.com/username/repo},
  abstract={Your abstract text here...}
}
```

### Conference Paper

```bibtex
@inproceedings{authorYEARkeyword,
  title={Full Paper Title},
  author={LastName1, FirstName1 and LastName2, FirstName2},
  booktitle={Proceedings of Conference Full Name (ABBR)},
  pages={XXX--YYY},
  year={2026},
  organization={IEEE/ACM/etc},
  selected={true},
  pdf={paper.pdf},
  slides={slides.pdf},
  poster={poster.pdf},
  code={https://github.com/username/repo},
  website={https://project-website.com},
  abstract={Your abstract text here...}
}
```

### Preprint/ArXiv

```bibtex
@article{authorYEARkeyword,
  title={Full Paper Title},
  author={LastName1, FirstName1 and LastName2, FirstName2},
  journal={arXiv preprint arXiv:XXXX.XXXXX},
  year={2026},
  arxiv={XXXX.XXXXX},
  selected={false},
  abstract={Your abstract text here...}
}
```

---

## 🏆 Achievement Templates

### Award Card

```html
<div class="achievement-card">
  <div class="achievement-icon">🏆</div>
  <h3 class="achievement-title">Award Name</h3>
  <p class="achievement-description">
    Description of the award, what it was for, and any relevant details...
  </p>
  <div class="achievement-meta">
    <strong>Date:</strong> Month Year<br>
    <strong>Recipient:</strong> Person Name<br>
    <strong>Organization:</strong> Awarding Body
  </div>
</div>
```

### Grant Timeline Item

```html
<div class="timeline-item">
  <span class="timeline-date">Mon YYYY</span>
  <div class="timeline-content">
    <h3>Grant Title</h3>
    <p><strong>Amount:</strong> $XXX,XXX</p>
    <p><strong>Duration:</strong> X years</p>
    <p><strong>Project:</strong> Project Title</p>
    <p>Brief description of what the grant funds...</p>
  </div>
</div>
```

### Patent Entry

```html
<div class="achievement-card">
  <div class="achievement-icon">📄</div>
  <h3 class="achievement-title">Patent: Title</h3>
  <p class="achievement-description">
    <strong>Application No:</strong> US 2026/0XXXXXX<br>
    <strong>Status:</strong> Pending / Granted<br>
    <strong>Inventors:</strong> Name1, Name2, Name3<br>
    Brief description of the invention...
  </p>
</div>
```

---

## 📸 Gallery Item Template

```html
<div class="gallery-item" data-category="events">
  <span class="category-badge">Events</span>
  <img src="{{ '/assets/img/gallery/filename.jpg' | relative_url }}" 
       alt="Description" 
       loading="lazy">
  <div class="gallery-overlay">
    <h3 class="gallery-title">Event/Photo Title</h3>
    <p class="gallery-date">Month DD, YYYY</p>
  </div>
</div>
```

**Available Categories:**
- `events` - Events & Seminars
- `lab` - Lab Activities
- `team` - Team Outings
- `conferences` - Conferences
- `equipment` - Equipment & Facilities

---

## 📝 Custom Page Template

Create new file in `_pages/` folder:

```markdown
---
layout: page
title: page title
permalink: /url-slug/
description: SEO description for this page
nav: true  # Include in navigation?
nav_order: 7  # Order in navigation menu
---

<style>
/* Optional: Page-specific CSS */
.custom-class {
  /* your styles */
}
</style>

## Main Heading

Your content here...

### Subheading

More content...

<div class="custom-section">
  <p>You can include HTML as needed</p>
</div>

---

## Another Section

Additional content...
```

---

## 🎨 Styling Shortcuts

### Call-to-Action Button

```html
<a href="/contact/" class="btn btn-primary">Contact Us</a>
```

Options: `.btn-primary`, `.btn-secondary`, `.btn-outline`

### Colored Badge

```html
<span class="badge badge-success">Active</span>
```

Options: `.badge-primary`, `.badge-success`, `.badge-warning`, `.badge-info`

### Two-Column Layout

```html
<div class="row">
  <div class="col-md-6">
    Left column content
  </div>
  <div class="col-md-6">
    Right column content
  </div>
</div>
```

### Three-Column Layout

```html
<div class="row">
  <div class="col-md-4">Column 1</div>
  <div class="col-md-4">Column 2</div>
  <div class="col-md-4">Column 3</div>
</div>
```

### Image with Caption

```liquid
{% include figure.liquid 
   path="assets/img/filename.jpg" 
   title="Alt text" 
   class="img-fluid rounded z-depth-1" 
   loading="lazy" %}
```

### Highlighted Box

```html
<div style="background: #f8f9fa; padding: 2rem; border-radius: 12px; margin: 2rem 0;">
  <h3>Box Title</h3>
  <p>Content in highlighted box...</p>
</div>
```

### Gradient Background Box

```html
<div style="background: linear-gradient(135deg, #667eea 0%, #764ba2 100%); color: white; padding: 3rem; border-radius: 12px; text-align: center; margin: 4rem 0;">
  <h2 style="color: white;">Heading</h2>
  <p>Content...</p>
</div>
```

---

## 📊 Data File Templates

### Adding Social Link (`_data/socials.yml`)

```yaml
email: your.email@lab.edu
github_username: labusername
twitter_username: labhandle
linkedin_username: company/labname
youtube_username: @labchannel
scholar_userid: googlescholarid
orcid_id: 0000-0000-0000-0000
```

---

## 🔗 Useful Markdown Syntax

### Links

```markdown
[Link Text](https://url.com)
[Email Link](mailto:email@domain.com)
```

### Emphasis

```markdown
*italic* or _italic_
**bold** or __bold__
***bold italic***
```

### Lists

```markdown
- Bullet point 1
- Bullet point 2
  - Nested bullet

1. Numbered item 1
2. Numbered item 2
```

### Images

```markdown
![Alt text](path/to/image.jpg)
```

### Code

```markdown
`inline code`

\```python
# code block
def function():
    return True
\```
```

### Blockquote

```markdown
> This is a quoted text
```

### Horizontal Rule

```markdown
---
```

### Tables

```markdown
| Column 1 | Column 2 |
|----------|----------|
| Data 1   | Data 2   |
```

---

## 💡 Pro Tips

1. **Consistent naming**: Use lowercase with hyphens for files (e.g., `new-project.md`)
2. **Image optimization**: Compress images before uploading (use TinyPNG.com)
3. **Date format**: Use `YYYY-MM-DD HH:MM:SS` for dates
4. **Testing**: Always test locally with `bundle exec jekyll serve` before pushing
5. **Commit messages**: Use clear messages like "Add new research project" or "Update team photos"
6. **Backup**: Keep copies of original high-res images separate from web versions

---

## 📋 Quick Reference: File Locations

- Team member photos: `assets/img/team/`
- Project images: `assets/img/projects/`
- Gallery photos: `assets/img/gallery/`
- PDF files: `assets/pdf/`
- News posts: `_news/`
- Project pages: `_projects/`
- Bibliography: `_bibliography/papers.bib`
- Site pages: `_pages/`
- Social links: `_data/socials.yml`

---

**Need help?** Refer to:
- `README_MIRAIVISION.md` - Full documentation
- `DEPLOYMENT_GUIDE.md` - Deployment instructions
- `QUICKSTART_CHECKLIST.md` - Step-by-step checklist

---

**Last Updated: January 29, 2026**
