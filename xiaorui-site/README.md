# Xiaorui Su — Personal Website

A clean, single-page academic homepage built with plain HTML + CSS. No build step, no dependencies.

## Files

```
index.html          # the page (edit content here)
assets/style.css     # styling
assets/cv.pdf        # your CV — drop your PDF here with this exact name
assets/photo.jpg     # optional headshot — add with this exact name to show it
.nojekyll            # tells GitHub Pages to serve files as-is
```

## Publish on GitHub Pages (username site — recommended)

Your site will live at **https://blair1213.github.io**

1. Create a new repository on GitHub named **`Blair1213.github.io`** (must match your username exactly, followed by `.github.io`). Make it **Public**.
2. Upload every file in this folder to the repo (keep the `assets/` folder structure). Two easy ways:
   - **Web:** on the repo page click *Add file → Upload files*, drag everything in, then *Commit changes*.
   - **Git (command line):**
     ```bash
     git init
     git add .
     git commit -m "Add personal website"
     git branch -M main
     git remote add origin https://github.com/Blair1213/Blair1213.github.io.git
     git push -u origin main
     ```
3. In the repo, go to **Settings → Pages**. Under *Build and deployment → Source*, choose **Deploy from a branch**, set branch to **main** and folder to **/(root)**, then **Save**.
4. Wait 1–2 minutes, then open **https://blair1213.github.io**. Done.

## Add your CV and photo

- Put your CV PDF at `assets/cv.pdf` (the "CV (PDF)" link already points there).
- Put a headshot at `assets/photo.jpg` to replace the "XS" placeholder in the sidebar. Square images look best (e.g. 500×500).

## Custom domain (optional)

If you own a domain (e.g. `xiaoruisu.com`), add a file named `CNAME` containing just the domain, then set it under Settings → Pages → Custom domain.

## Editing later

Everything is in `index.html`. To add a paper, copy one `<li class="pub">…</li>` block and edit the title, authors, and venue. To add a news item, copy one `<li>` under the News list.
