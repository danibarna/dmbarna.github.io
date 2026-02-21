# Setup Guide for Academic Personal Website

This guide will help you customize this template for your own academic website.

## Quick Setup (5 minutes)

### 1. Create Your Repository

1. Click the "Use this template" button at the top of this repository
2. Name your repository (e.g., `your-username.github.io` for a user site, or any name for a project site)
3. Make it public (required for free GitHub Pages)
4. Click "Create repository from template"

### 2. Enable GitHub Pages

1. Go to your repository settings
2. Navigate to "Pages" in the left sidebar
3. Under "Source", select the `main` branch
4. Click "Save"
5. Your site will be published at `https://your-username.github.io/repository-name/`

### 3. Edit Configuration

Edit `_config.yml` and update:

```yaml
title: Your Name
email: your.email@institution.edu
description: >-
  Personal academic website of Your Name, Assistant Professor at Your Institution.
  Research interests include Topic 1, Topic 2, and Topic 3.

author:
  name: "Your Full Name"
  avatar: "/assets/images/bio-photo.jpg"
  bio: "Assistant Professor of Computer Science at University Name"
  location: "City, Country"
```

### 4. Add Your Photo

Replace `assets/images/bio-photo.jpg` with your professional photo (recommended: 200x200px or larger, square aspect ratio).

## Detailed Customization

### Update Your Profile

Edit the author links in `_config.yml`:

```yaml
author:
  links:
    - label: "Email"
      icon: "fas fa-fw fa-envelope-square"
      url: "mailto:your.email@institution.edu"
    - label: "Google Scholar"
      icon: "fas fa-fw fa-graduation-cap"
      url: "https://scholar.google.com/citations?user=YOUR_ID"
    - label: "GitHub"
      icon: "fab fa-fw fa-github"
      url: "https://github.com/your-username"
```

### Customize Pages

#### About Page (`_pages/about.md`)

Replace the placeholder content with:
- Your biography
- Research interests
- Recent news/updates
- Contact information

#### Research Page (`_pages/research.md`)

Add:
- Overview of your research
- Current projects
- Past projects
- Research group members
- Collaborators
- Information for prospective students

#### Publications Page (`_pages/publications.md`)

Option 1: Use the data file (recommended)
- Edit `_data/publications.yml`
- Add your publications in YAML format
- They'll be automatically displayed

Option 2: Manual entry
- Edit `_pages/publications.md` directly
- Add publications in markdown format

Example publication entry in `_data/publications.yml`:

```yaml
- title: "Your Paper Title"
  authors: "Author1, Author2, Your Name"
  venue: "Conference Name (CONF '24)"
  year: 2024
  pdf: "https://example.com/paper.pdf"
  doi: "10.xxxx/xxxxx"
  code: "https://github.com/username/repo"
```

#### Teaching Page (`_pages/teaching.md`)

Add:
- Current courses
- Past courses
- Teaching philosophy
- Student advising
- Teaching awards

#### CV Page (`_pages/cv.md`)

Update with:
- Education
- Academic appointments
- Publications (or link to publications page)
- Grants & awards
- Teaching experience
- Service activities
- Invited talks

Also add a PDF version:
- Create your CV as a PDF
- Place it in `assets/files/cv.pdf`

### Navigation

The navigation menu is defined in `_data/navigation.yml`:

```yaml
main:
  - title: "About"
    url: /about/
  - title: "Research"
    url: /research/
  - title: "Publications"
    url: /publications/
  - title: "Teaching"
    url: /teaching/
  - title: "CV"
    url: /cv/
  - title: "Blog"
    url: /posts/
```

Add, remove, or reorder items as needed.

### Blog Posts

To add a blog post:

1. Create a new file in `_posts/` with format: `YYYY-MM-DD-title.md`
2. Add front matter:

```yaml
---
title: "Your Post Title"
date: 2024-01-15
categories:
  - Blog
tags:
  - research
  - news
---

Your post content here...
```

### Colors and Theme

Change the site skin in `_config.yml`:

```yaml
minimal_mistakes_skin: default
```

Available skins: `default`, `air`, `aqua`, `contrast`, `dark`, `dirt`, `neon`, `mint`, `plum`, `sunrise`

## Advanced Customization

### Custom Domain

To use a custom domain (e.g., `www.yourname.com`):

1. Add a file named `CNAME` with your domain:
   ```
   www.yourname.com
   ```
2. Configure DNS settings with your domain provider
3. See [GitHub Pages custom domain docs](https://docs.github.com/en/pages/configuring-a-custom-domain-for-your-github-pages-site)

### Adding More Pages

To add a new page:

1. Create `_pages/newpage.md`
2. Add front matter:
   ```yaml
   ---
   permalink: /newpage/
   title: "Page Title"
   ---
   ```
3. Add link to `_data/navigation.yml`

### Local Development

To preview your site locally:

1. Install Ruby and Bundler
2. Run:
   ```bash
   bundle install
   bundle exec jekyll serve
   ```
3. Visit `http://localhost:4000`

## Troubleshooting

### Site not showing up
- Make sure GitHub Pages is enabled in settings
- Check that your repository is public
- Wait a few minutes for GitHub to build the site

### Images not displaying
- Check that image paths start with `/assets/`
- Make sure files are committed and pushed
- Verify image files exist in the repository

### Changes not appearing
- GitHub Pages can take 1-2 minutes to rebuild
- Hard refresh your browser (Ctrl+F5 or Cmd+Shift+R)
- Check the Actions tab for build status

### Build failures
- Validate YAML syntax in `_config.yml`
- Check that all front matter is properly formatted
- Review the Actions tab for error messages

## Resources

- [Jekyll Documentation](https://jekyllrb.com/docs/)
- [Minimal Mistakes Theme Docs](https://mmistakes.github.io/minimal-mistakes/)
- [GitHub Pages Documentation](https://docs.github.com/en/pages)
- [Markdown Guide](https://www.markdownguide.org/)
- [YAML Syntax](https://yaml.org/spec/1.2/spec.html)

## Getting Help

- [Jekyll Forum](https://talk.jekyllrb.com/)
- [Stack Overflow - Jekyll tag](https://stackoverflow.com/questions/tagged/jekyll)
- [GitHub Pages Community](https://github.com/orgs/community/discussions/categories/pages)
