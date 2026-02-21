# Academic Personal Website Template

A clean, responsive GitHub Pages template for academic personal websites built with Jekyll and the [Minimal Mistakes theme](https://github.com/mmistakes/minimal-mistakes).

## Features

This template includes:

- **About page** - Professional bio and photo
- **Publications page** - List your academic papers and publications
- **Research page** - Describe your research interests and projects
- **CV page** - Display your academic CV
- **Teaching page** - List courses taught and teaching experience
- **Blog** - Optional blog for sharing updates and thoughts
- **Responsive design** - Works great on mobile, tablet, and desktop
- **Site-wide search** - Find content easily
- **Google Scholar integration** - Link to your academic profiles

## Quick Start

1. Click [**Use this template**](../../generate) to create your own repository
2. Enable GitHub Pages in your repository settings (Settings → Pages → Source: main branch)
3. Edit `_config.yml` with your information
4. Customize the content in `_pages/` to add your own information
5. Add your publications to `_data/publications.yml`
6. Replace the bio photo in `assets/images/bio-photo.jpg` with your own

Your site will be published at `https://your-username.github.io/repository-name/`

**📋 Follow the [setup checklist](CHECKLIST.md) to track your progress!**  
**📖 See [detailed setup guide](SETUP.md) for step-by-step instructions.**

## Customization Guide

### Update Your Profile (_config.yml)

Edit the following fields in `_config.yml`:

```yaml
title: Your Name
email: your.email@institution.edu
description: Brief description of your research
```

Update the author section:

```yaml
author:
  name: "Your Full Name"
  avatar: "/assets/images/bio-photo.jpg"
  bio: "Your academic title and affiliation"
  location: "City, Country"
  links:
    - label: "Email"
      icon: "fas fa-fw fa-envelope-square"
      url: "mailto:your.email@institution.edu"
    - label: "Google Scholar"
      icon: "fas fa-fw fa-graduation-cap"
      url: "https://scholar.google.com/citations?user=YOUR_ID"
    # Add more links as needed
```

### Add Your Publications

Edit `_data/publications.yml` to add your papers:

```yaml
- title: "Your Paper Title"
  authors: "Author1, Author2, Author3"
  venue: "Conference or Journal Name"
  year: 2024
  pdf: "link-to-pdf"
  doi: "10.xxxx/xxxxx"
```

### Customize Pages

- **About**: Edit `_pages/about.md`
- **Research**: Edit `_pages/research.md`
- **Publications**: Edit `_pages/publications.md`
- **Teaching**: Edit `_pages/teaching.md`
- **CV**: Edit `_pages/cv.md`

### Add Your Photo

Replace `assets/images/bio-photo.jpg` with your professional photo (recommended size: 200x200px or larger, square aspect ratio).

## Local Development

To test your site locally:

```bash
bundle install
bundle exec jekyll serve
```

Visit `http://localhost:4000` in your browser.

## Resources

- [Jekyll Documentation](https://jekyllrb.com/docs/)
- [Minimal Mistakes Documentation](https://mmistakes.github.io/minimal-mistakes/docs/quick-start-guide/)
- [GitHub Pages Documentation](https://docs.github.com/en/pages)
- [Markdown Guide](https://www.markdownguide.org/)

## Support

If you have questions:
- Check the [Jekyll Forum](https://talk.jekyllrb.com/)
- Ask on [StackOverflow](https://stackoverflow.com/questions/tagged/jekyll)
- Review [Minimal Mistakes documentation](https://mmistakes.github.io/minimal-mistakes/docs/configuration/)

## License

This template is based on the Minimal Mistakes Jekyll theme and is free to use for academic purposes.
