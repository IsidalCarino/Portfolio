# Isidal Kent A. Carino · Portfolio

A single-page portfolio, ready for GitHub Pages. No build step.

## What's in this folder

- `index.html`: the page.
- `img/`: the images. They load as you scroll.
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

Paste this where you want the portfolio to appear. Replace the URL with yours.
It grows to the full height of the page, so there's no inner scrollbar.

```html
<iframe id="ikc-portfolio" src="https://yourusername.github.io/portfolio/"
  title="Isidal Kent A. Carino portfolio" loading="lazy"
  style="display:block;width:100%;height:900px;border:0"></iframe>
<script>
  window.addEventListener('message', function (e) {
    var f = document.getElementById('ikc-portfolio');
    if (!f || !e.data || e.source !== f.contentWindow) return;
    if (e.data.type === 'ikc-portfolio:height') f.style.height = e.data.height + 'px';
    if (e.data.type === 'ikc-portfolio:scroll') {
      window.scrollTo({ top: f.getBoundingClientRect().top + window.scrollY + e.data.top, behavior: 'smooth' });
    }
  });
</script>
```

On Canva, use the **Embed** app and paste just the URL; the script part isn't needed there.
