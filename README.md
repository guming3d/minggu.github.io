# Personal Blog — minggu.github.io

This repository hosts my GitHub Pages site powered by Jekyll (Minima theme). It focuses on AI engineering, LLMs, and my personal journey.

## Local preview

GitHub Pages builds with `github-pages` gem, but you can preview with system Jekyll too.

1. Install Ruby (>= 3.0) and Bundler.
2. Option A (simpler):
   - `gem install jekyll bundler`
   - `bundle init` then add `gem "jekyll"` to Gemfile
   - `bundle install`
   - `bundle exec jekyll serve`
3. Option B (closer to GH Pages):
   - Create a Gemfile with `gem "github-pages", group: :jekyll_plugins`
   - `bundle install`
   - `bundle exec jekyll serve`

Then open `http://localhost:4000`.

## Content structure

- Home: `index.md` shows recent posts
- About: `about.md`
- Archive: `archive.md`
- Posts: `_posts/YYYY-MM-DD-title.md`

## Writing posts

Create a file under `_posts` named `YYYY-MM-DD-your-title.md` with front matter:

```
---
layout: post
title: "Post Title"
description: Optional summary
tags: [ai, llms]
---

Your content here.
```

## Deploy

Push to `main` (or the default branch). In repo settings, enable GitHub Pages and select the `main` branch root. GitHub will build and serve at `https://minggu.github.io`.

