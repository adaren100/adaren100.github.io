# Ada's Notes

This repo is a Hugo site using the PaperMod theme and is set up to deploy to GitHub Pages at:

`https://adaren100.github.io/`

## Run Locally

```bash
cd /Users/ada/Documents/MQ/repo/my-site
hugo server -D
```

Open `http://localhost:1313/`.

## Create a New Post

```bash
cd /Users/ada/Documents/MQ/repo/my-site
hugo new content posts/my-new-post.md
```

Then edit `content/posts/my-new-post.md`.

Example front matter:

```toml
+++
date = '2026-03-19T13:30:00+11:00'
draft = true
title = 'My New Post'
+++
```

Write the article body below the second `+++`.

## Publish Online

1. Set `draft = false` in the post you want to publish.
2. Check the site locally:

   ```bash
   hugo
   hugo server
   ```

3. Commit and push to `main`:

   ```bash
   git add .
   git commit -m "Publish site updates"
   git push origin main
   ```

4. GitHub Actions will run `.github/workflows/hugo.yaml` and deploy the site to GitHub Pages.
5. In GitHub, make sure the repo uses `Settings > Pages > Source: GitHub Actions`.

After the workflow finishes, the live site will be available at `https://adaren100.github.io/`.
