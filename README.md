# SkyHigh Wiki

The official documentation library for the SkyHigh aviation simulation network.

Built with [MkDocs](https://mkdocs.org) + [Material for MkDocs](https://squidfunk.github.io/mkdocs-material/).

## Live site

'[Live Site](https://wiki.skyhighnetwork.co.uk/)'

## Local development

```bash
pip install mkdocs-material
mkdocs serve
```

Then open `http://127.0.0.1:8000`.

## Contributing

1. Edit the relevant `.md` file inside `docs/`.
2. Commit and push to `main` — the GitHub Action will auto-deploy to GitHub Pages.

## Structure

```
docs/
  index.md           # Home page
  pilots/            # Pilot guides
  controllers/       # Controller guides
  network/           # Network rules
  training/          # Training & exams
  tools/             # Software documentation
  staff/             # Staff SOPs (internal)
  tech/              # Technical reference
```
