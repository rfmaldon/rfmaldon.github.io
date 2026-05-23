# rubenf.com

Personal portfolio site for Ruben Francisco — Creative Director & Production Designer.

Static site hosted on GitHub Pages, pointed at the custom domain `www.rubenf.com`.

## Structure

- `index.html` — homepage with the eight portfolio categories
- `about.html` — bio, work history, clients, contact
- 8 category pages: `concept-art.html`, `set-design.html`, `animation.html`, `advertising.html`, `murals.html`, `illustration.html`, `rock-work.html`, `graphic-design.html`
- `styles.css` — single stylesheet for the whole site
- `images/` — portfolio image assets
- `CNAME` — GitHub Pages custom-domain config (points to `www.rubenf.com`)

## Local preview

```
cd /path/to/this/folder
python3 -m http.server 8000
# then open http://localhost:8000
```

## Deploy

This repo is set up for GitHub Pages. After pushing to GitHub:

1. Go to repo **Settings → Pages**
2. Set **Source** to `Deploy from a branch`
3. Choose branch `main` and folder `/ (root)`
4. Under **Custom domain**, enter `www.rubenf.com`
5. Update DNS at your registrar:
   - `CNAME` record for `www` → `<your-username>.github.io`
   - For the apex `rubenf.com`, add `A` records pointing to GitHub's IPs:
     - `185.199.108.153`
     - `185.199.109.153`
     - `185.199.110.153`
     - `185.199.111.153`
