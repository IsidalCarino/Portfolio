# Isidal Kent A. Carino · Portfolio

A menu-style, full-screen portfolio, ready for GitHub Pages. No build step.

Use the arrow keys and Enter on the title screen, Esc to go back. Each section also has its own link, e.g. `#matech` or `#contact`.

## What's in this folder

- `index.html`: the page.
- `img/`: the images. Each section's images load when you open it.
- `.nojekyll`: tells GitHub to serve the files as they are.

## Put it online

1. On GitHub, create a new **public** repository.
   - Name it `yourusername.github.io` and the site lives at `https://yourusername.github.io/`.
   - Any other name, e.g. `portfolio`, gives `https://yourusername.github.io/portfolio/`.
2. Click **Add file → Upload files**. Drag in everything in this folder: `index.html`, the `img` folder, `README.md` and `.nojekyll`. Then click **Commit changes**.
   - `.nojekyll` is hidden on Mac and Windows. If you can't see it, skip it; the site still works.
3. Go to **Settings → Pages**. Under **Build and deployment**, set Source to **Deploy from a branch**, pick **main** and **/(root)**, and click **Save**.
4. Wait a minute or two, then open the link GitHub shows at the top of that page.

To update the site later, upload the new `index.html` (and any new images) the same way. GitHub republishes on its own.

## Embed it on another site

The portfolio fills the screen it's shown in, so give the frame a fixed height. Replace the URL with yours.

```html
<iframe src="https://yourusername.github.io/portfolio/"
  title="Isidal Kent A. Carino portfolio" loading="lazy"
  style="display:block;width:100%;height:100vh;min-height:640px;border:0"></iframe>
```

To open the frame on one section, add it to the URL, e.g. `https://yourusername.github.io/portfolio/#matech`.

On Canva, use the **Embed** app and paste just the URL.
