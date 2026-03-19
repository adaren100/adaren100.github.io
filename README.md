# Hugo Cheat Sheet

## Start

```bash
cd /Users/ada/Documents/MQ/repo/my-site
hugo server -D
```

Open: `http://localhost:1313/`

Stop: `Ctrl+C`

## New Post

```bash
cd /Users/ada/Documents/MQ/repo/my-site
hugo new content posts/my-new-post.md
```

Edit: `content/posts/my-new-post.md`

## Post Template

```md
+++
date = '2026-03-19T13:30:00+11:00'
draft = true
title = 'My New Post'
+++

Write here.
```

Rule: write the article body below the second `+++`.

## Publish

Change:

```toml
draft = false
```
