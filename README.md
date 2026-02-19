# Reflections

Personal blog built with [Astro](https://astro.build).

Live site: `https://felipe-vrgs.github.io`

## Local development

Prereqs: Node.js LTS + npm.

```bash
npm ci
npm run dev
```

Astro will print the local URL in the terminal (usually `http://localhost:4321`).

## Commands

```bash
npm run dev
npm run build
npm run preview
```

Build output is written to `dist/`.

## Writing posts

Posts live in `src/data/blog-posts/` and are loaded as an Astro content collection
(see `src/content.config.js`).

Each post is a Markdown file with frontmatter like:

```md
---
title: "My post title"
slug: my-post
publishDate: 19 Feb 2026
description: "One sentence summary."
---
```

Routes:

- `/blog` lists posts
- `/blog/<slug>` renders a post

## Images and other assets

Static files go in `public/` and are referenced from the site root.

- Site assets: `public/assets/` -> `/assets/...`
- Blog images: `public/assets/blog/` -> `/assets/blog/...`

## Deployment

This repo deploys to GitHub Pages on push to `main` via
`.github/workflows/deploy.yml`.

The workflow runs `npm ci`, builds the site, and uploads `dist/` as the Pages
artifact.
