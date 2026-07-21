# jgorisek.github.io

Personal website built for GitHub Pages with Jekyll.

## What is included

- Home page with bio and contact icons
- CV/resume page
- Photography gallery
- Projects and publications
- Blog index and post layout
- Responsive navigation and styling

## Edit the main profile content

Update `_data/profile.yml` for:

- Name, role, location, tagline, and bio
- LinkedIn, GitHub, email, and resume links
- CV experience, education, and skills

Blank social URLs are ignored on the home page. Add your LinkedIn or email URL when you want those icons to appear.

## Add a blog post

Create a Markdown file in `_posts/` using this naming pattern:

```text
YYYY-MM-DD-post-title.md
```

Start it with front matter:

```yaml
---
title: "Post title"
description: "Short summary for the blog index."
---
```

## Add a project

Create a Markdown file in `_projects/`:

```yaml
---
title: "Project title"
description: "Short project summary."
year: "2026"
status: "In progress"
tags:
  - Robotics
  - Simulation
---
```

## Add a publication

Create a Markdown file in `_publications/`:

```yaml
---
title: "Publication title"
authors: "Author list"
description: "Short summary."
year: "2026"
venue: "Conference or Journal"
paper_url: "https://example.com/paper.pdf"
---
```

## Add photography

Edit `_data/photography.yml`. Each image can point to a local file in `assets/img/` or to a hosted URL such as Cloudflare Images or Cloudflare R2:

```yaml
- title: "Photo title"
  image: "https://imagedelivery.net/account/image-id/public"
  alt: "Accessible description of the photo."
  location: "Location or series"
  year: "2026"
  tags:
    - Street
    - Travel
```

## GitHub Pages

For a `username.github.io` repository, GitHub Pages can serve from the `main` branch. In GitHub, go to Settings -> Pages and select the branch/source if it is not already enabled.

## Local preview

If you have Ruby and Bundler available:

```bash
bundle install
bundle exec jekyll serve
```

Then open `http://localhost:4000`.
