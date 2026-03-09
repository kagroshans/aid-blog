# Alternative Investing Doctor — Blog

Minimal Jekyll blog for [blog.alternativeinvestingdoctor.com](https://blog.alternativeinvestingdoctor.com). Deployed via GitHub Pages.

---

## Local Development

**Prerequisites:** Ruby + Bundler installed.

```bash
bundle install
bundle exec jekyll serve
```

Visit `http://localhost:4000`. The site rebuilds automatically on file changes.

---

## Adding a New Post

Create a file in `_posts/` following the naming convention `YYYY-MM-DD-post-slug.md`:

```markdown
---
layout: post
title: "Your Post Title"
date: 2026-03-08
excerpt: "One or two sentence summary shown on the index and in meta tags."
---

Your content here in standard markdown.
```

The post will be live at `https://blog.alternativeinvestingdoctor.com/post-slug`.

---

## Deployment

This blog deploys automatically via GitHub Pages on every push to `main`.

**Initial setup (one time):**
1. Push this repo to GitHub
2. Go to repo **Settings → Pages**
3. Set Source to **Deploy from branch → main → / (root)**
4. GitHub Pages will build and deploy automatically

---

## Custom Domain

The `CNAME` file contains `blog.alternativeinvestingdoctor.com`. Configure these DNS records at your registrar:

| Type  | Host | Value                         |
|-------|------|-------------------------------|
| A     | @    | 185.199.108.153               |
| A     | @    | 185.199.109.153               |
| A     | @    | 185.199.110.153               |
| A     | @    | 185.199.111.153               |
| CNAME | www  | your-github-username.github.io |

DNS propagation typically takes a few minutes to a few hours. GitHub Pages will provision an SSL certificate automatically once the domain is verified.
