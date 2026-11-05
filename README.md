# Gaurav Ratra — Portfolio

A single-page portfolio site. Everything (design, images, animation) lives inside one file, `index.html`, so there is nothing to build or install.

## What is in this folder

| File | What it does |
|---|---|
| `index.html` | The whole website |
| `.nojekyll` | Tells GitHub Pages to serve the file as it is |
| `404.html` | Sends any wrong address back to the home page |
| `README.md` | These instructions (you can delete it from the repo if you like) |

## Put it online with GitHub Pages (about 5 minutes)

1. **Create a repository.** On github.com click **New repository**.
   - For the address `https://YOUR-USERNAME.github.io`, name it exactly `YOUR-USERNAME.github.io`.
   - Any other name works too; the site is then at `https://YOUR-USERNAME.github.io/REPO-NAME/`.
   - Choose **Public**.
2. **Upload the files.** In the new repo click **Add file → Upload files**, drag in everything from this folder (`index.html`, `.nojekyll`, `404.html`), then **Commit changes**.
   - `.nojekyll` can look hidden on a Mac. Press `Cmd + Shift + .` in Finder to show hidden files, or skip it; the site still works without it.
3. **Switch on Pages.** Go to **Settings → Pages**. Under **Build and deployment** set **Source** to **Deploy from a branch**, pick the **main** branch and the **/ (root)** folder, then **Save**.
4. **Wait a minute or two**, refresh that Settings page, and your link appears at the top.

### Prefer the command line?

```bash
git init
git add .
git commit -m "Portfolio site"
git branch -M main
git remote add origin https://github.com/YOUR-USERNAME/REPO-NAME.git
git push -u origin main
```

Then do step 3 above.

## Use your own domain (optional)

1. In **Settings → Pages → Custom domain**, type your domain (for example `gauravratra.com`) and save. GitHub adds a `CNAME` file for you.
2. At your domain registrar, add these DNS records:
   - Four **A** records for `@` pointing to `185.199.108.153`, `185.199.109.153`, `185.199.110.153` and `185.199.111.153`.
   - One **CNAME** record for `www` pointing to `YOUR-USERNAME.github.io`.
3. Back in Settings → Pages, tick **Enforce HTTPS** once it becomes available (it can take up to a day).

## Turn on the "Download CV" button

Add your CV to the repo, next to `index.html`, named exactly:

```
Gaurav_Ratra_CV.pdf
```

That is all. The site checks for that file and, when it finds it, both "Download CV" buttons start downloading it. Until then they scroll to the resume section.

## Update the site later

Replace `index.html` in the repo (**Add file → Upload files**, same filename) and commit. The live site refreshes within a minute or two.

## Good to know

- **Experiments page:** My Mixtapes, Kshann and Scrooge open inside the page on GitHub Pages. If one stays blank, that site does not allow being shown inside another page. The "Open it in a new tab" link under the viewer always works.
- **Figma and 3D mockup prototypes** in the case studies play inside the page too, as long as their share links are public.
- **Sharing on social media:** Links show a title and description. To also show a preview image, add `<meta property="og:image" content="https://YOUR-DOMAIN/preview.jpg">` to the `<head>` of `index.html` and upload `preview.jpg` (about 1200 × 630 px).
- **File size:** `index.html` is about 9 MB. That is fine for GitHub (the limit is 100 MB per file).
