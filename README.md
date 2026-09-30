# Shoreline Lots

Offering website for two designed homesites at 19339 & 19335 11th Ave NW, Shoreline, WA 98177 (shorelinelots.com).

Everything the page needs (styles, script, renderings and drawing sheets) is built into `index.html`, so the site works wherever that one file lands. No build step.

## Files

```
index.html   the whole site
CNAME        tells GitHub Pages the domain is shorelinelots.com
.nojekyll    tells GitHub Pages to serve files as-is
img/og.jpg   preview image for links shared on social media / iMessage
README.md    this file
```

## Publish on GitHub Pages (drag-and-drop)

1. Create a new repository on github.com (public is fine).
2. On the repository page, click **Add file → Upload files**, drag in `index.html`, `CNAME`, `.nojekyll` and the `img` folder (drag the folder itself so `img/og.jpg` keeps its path; if it flattens, that only affects the social preview image, not the site). Click **Commit changes**.
3. Open **Settings → Pages**. Under **Build and deployment**, set Source to **Deploy from a branch**, choose `main` and `/ (root)`, and save.
4. After a minute or two the site is live at `https://<your-username>.github.io/<repo-name>/`. Clicking `index.html` inside the repository shows its source code, not the site; use the Pages address to see it.

## Custom domain: shorelinelots.com

1. At your domain registrar, add these DNS records:
   - `A` records for `@` (the root) pointing to `185.199.108.153`, `185.199.109.153`, `185.199.110.153`, `185.199.111.153`
   - `CNAME` record for `www` pointing to `<your-username>.github.io`
2. In **Settings → Pages → Custom domain**, enter `shorelinelots.com` and save. GitHub checks the DNS (this can take up to a day to propagate).
3. Once the check passes, tick **Enforce HTTPS**.

`www.shorelinelots.com` will redirect to the root domain automatically.

## Editing

Everything is in `index.html`. Contact details are in the `#contact` section, the permit-status cards and timeline in `#status`. The document list in `#documents` is an inventory only; no plan sets or reports are hosted, and buyers are directed to Adam Cobb.
