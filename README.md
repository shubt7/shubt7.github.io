# My Blog

A GitHub Pages blog built with Jekyll.

## Write a post
Create a file in `_posts/` named `YYYY-MM-DD-title.md`, starting with front matter:

```
---
layout: post
title: "Your title"
date: YYYY-MM-DD
---
```

## Preview locally
```
bundle install
bundle exec jekyll serve
```
Then open http://localhost:4000.

## Publish
Push to the `main` branch, then in the repo go to Settings → Pages and set the source to "Deploy from a branch", branch `main`, folder `/ (root)`.
