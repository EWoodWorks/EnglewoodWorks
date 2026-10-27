# Englewood Works website

A single-page static site for englewoodworks.org. No build step, no dependencies beyond two Google Fonts (Jost and Lora).

## Files

- `index.html` — the whole site
- `style.css` — styles
- `img/` — logo, favicons, and the nine program photos (exported from the Facebook banner)
- `CNAME` — tells GitHub Pages the site lives at englewoodworks.org

## Publish with GitHub Pages

1. Create a public repository (for example `englewoodworks-site`) and upload every file in this folder to its root.
2. In the repository, open Settings, then Pages. Under Build and deployment, set Source to "Deploy from a branch", pick the `main` branch and the `/ (root)` folder, and save.
3. At your DNS provider, point the domain at GitHub Pages:
   - Four A records for `englewoodworks.org` pointing to 185.199.108.153, 185.199.109.153, 185.199.110.153 and 185.199.111.153
   - A CNAME record for `www` pointing to `<your-github-username>.github.io`
   - Remove the existing forward to englewoodfamily.org so the domain no longer redirects.
4. Back in Settings, then Pages, enter `englewoodworks.org` as the custom domain and, once the DNS check passes, turn on "Enforce HTTPS".

## Editing

Everything a funder reads is plain text inside `index.html`. Search for the section ids (`#club`, `#why`, `#path`, `#support`, `#leadership`, `#contact`) to find each block. To swap a photo, replace the file in `img/` and keep the same name, or change the `src` on the matching `<img>`.
