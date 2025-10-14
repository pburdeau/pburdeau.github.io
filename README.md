# Academic Website (GitHub Pages + Jekyll Minimal Mistakes)

## Quick start
1. Create a new public repo named `your-username.github.io` on GitHub.
2. Upload all files from this folder (or push via git).
3. In **Settings → Pages**, set **Build and deployment** to "GitHub Pages" using the `main` branch (root).
4. Wait ~1–2 minutes for the site to build, then visit `https://your-username.github.io`.

## Customize
- Edit `_config.yml`: set `url`, `repository`, your social links, and site title.
- Replace `/assets/img/avatar.jpg` with a square headshot.
- Add your CV PDF in `/assets/cv/` and link it in `cv.md`.
- Add new pages by creating `.md` files with the front matter at the top.

## Local preview (optional)
If you want to build locally:
```bash
gem install bundler
bundle add webrick
bundle install
bundle exec jekyll serve
```
Then open http://127.0.0.1:4000.

## Notes
- This uses the Minimal Mistakes theme via `remote_theme`, compatible with GitHub Pages.
- Avoid unsupported plugins on GitHub Pages (e.g., `jekyll-scholar`). Render citations offline and paste static HTML.