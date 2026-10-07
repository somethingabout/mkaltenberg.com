# mkaltenberg.com

Academic website for Mary Kaltenberg, built with [Hugo](https://gohugo.io/) and deployed via GitHub Pages.

Built with Claude Opus 5.5.

## Structure

```
config.toml               Site config: title, menu, contact params
content/
  _index.md               Homepage (About)
  research/_index.md      Publications & working papers
  teaching/_index.md      Teaching philosophy & courses
  teaching/econhack/_index.md EconHack information
  cv/_index.md            CV page (links to static/files/cv.pdf)
  code-data/_index.md     Code & data links
  contact/_index.md       Contact info
layouts/                  HTML templates (no external theme)
assets/css/main.css       Site stylesheet
.github/workflows/        Auto-deploy on push to main
```

## Local preview

Install Hugo (any recent version), then:

```
hugo server
```

Open http://localhost:1313.



