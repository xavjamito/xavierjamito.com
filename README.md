# Xavier Jamito Blog

Personal blog built with Astro and Tailwind CSS. Posts live as Markdown files in `src/content/blog`.

## Local Development

```sh
npm install
npm run dev
```

The site runs at `http://localhost:4321` by default.

## Build for Deployment

```sh
npm run build
npm run preview
```

Production output is generated in `dist/`. Deploy that directory to your web server or static hosting platform.

## Project Structure

```text
/
├── public/                  # Static assets (favicons, images)
├── src/
│   ├── content/
│   │   ├── config.ts        # Content collection schema
│   │   └── blog/            # Markdown blog posts
│   ├── layouts/             # Shared page layouts
│   ├── pages/               # Routes (home, blog, tags)
│   └── styles/              # Global styles
├── astro.config.mjs
└── package.json
```

## Writing Posts

Create a new Markdown file in `src/content/blog` with frontmatter:

```md
---
title: "Post title"
date: 2026-01-01
description: "Short summary"
tags: ["tag-1", "tag-2"]
draft: false
---
```

`draft` is optional and defaults to `false`.
