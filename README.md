# tertueanhvu.github.io

Personal portfolio built with [MkDocs Material](https://squidfunk.github.io/mkdocs-material/).

- `docs/index.md`: Portfolio tab (intro, contact, skills, education, projects)
- `docs/certifications.md`: Certifications tab
- `docs/projects/`: detail pages for projects that are still in progress

Preview locally:

```bash
pip install -r requirements.txt
mkdocs serve
```

Every push to `main` builds the site and publishes it to the `gh-pages` branch (`.github/workflows/deploy.yml`).
