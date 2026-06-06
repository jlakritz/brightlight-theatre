# Brightlight Theatre Hugo site

This repository is a markdown-driven Hugo site for Brightlight Theatre.

## What is included

- responsive split hero homepage
- production landing pages
- productions archive/list page
- news pages
- clean navigation, footer and booking banners
- CSS with the Brightlight hot pink / yellow palette
- Google font loading for Alfa Slab One and Inter
- GitHub Pages workflow

## Local development

1. Install Hugo Extended.
2. Run:

```bash
hugo server
```

3. Open the local URL printed in the terminal.

## Update the site

- Add or edit show pages in `content/productions/`
- Add news posts in `content/news/`
- Edit the site navigation in `config.toml`
- Edit the colours and layout in `static/css/main.css`

## Front matter fields for shows

Recommended fields:

```yaml
---
title: "Entertaining Angels"
status: "current" # current, upcoming, archive
author: "by Richard Everett"
details: "18th and 25th April at St. Peter's Church Hall, Frimley"
price: "£10 adult (£8 concessions)"
venue: "St. Peter's Church Hall, Frimley, GU16 7AQ"
booking_url: "https://..."
show_logo: "https://..."
cover_image: "https://..."
dates:
  - "Saturday 18th April 2026, 7.30pm"
cast:
  - "Grace"
crew:
  - "Director: ..."
gallery:
  - "https://..."
---
```

## GitHub Pages

The workflow in `.github/workflows/hugo.yml` deploys on pushes to `main`.

If you are using a custom domain, update `baseURL` in `config.toml`.
