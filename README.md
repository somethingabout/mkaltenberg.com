# mkaltenberg.com

Academic website for Mary Kaltenberg, built with [Hugo](https://gohugo.io/) and deployed via GitHub Pages.

## Structure

```
config.toml               Site config: title, menu, contact params
content/
  _index.md               Homepage (About)
  research/_index.md      Publications & working papers
  teaching/_index.md      Teaching philosophy & courses
  cv/_index.md            CV page (links to static/files/cv.pdf)
  code-data/_index.md     Code & data links
  contact/_index.md       Contact info
layouts/                  HTML templates (no external theme)
assets/css/main.css       Site stylesheet
static/
  img/headshot.jpg        <- ADD: your headshot (square crop works best)
  files/cv.pdf            <- ADD: your CV PDF
.github/workflows/        Auto-deploy on push to main
```

## Local preview

Install Hugo (any recent version), then:

```
hugo server
```

Open http://localhost:1313.

## Deployment (one-time setup)

1. Create a GitHub repository (e.g. `mkaltenberg.com`), push this folder to `main`.
2. In the repo: Settings → Pages → Source → **GitHub Actions**.
3. Push to `main`; the included workflow builds and deploys automatically.

### Custom domain

To serve at www.mkaltenberg.com:
1. Add a file named `CNAME` (no extension) at the repo root containing exactly: `www.mkaltenberg.com`
2. In Settings → Pages, enter the custom domain and enable "Enforce HTTPS".
3. At your DNS provider, add a CNAME record pointing `www` to `<username>.github.io`.

## To do after cloning

- [ ] Add `static/img/headshot.jpg`
- [ ] Add `static/files/cv.pdf` (the mary-cv.pdf produced earlier works)
- [ ] Add Google Scholar URL in `config.toml` (`scholar` param)
- [ ] Update GitHub username in `config.toml` and content pages if it has changed
