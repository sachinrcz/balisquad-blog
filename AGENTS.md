# AGENTS.md

Marketing blog built with Hugo. Config lives in `hugo.toml` / `config/_default/`.

## Cursor Cloud specific instructions

- **Hugo extended** is installed at `/usr/local/bin/hugo` (the `stack` theme requires
  Hugo extended >= 0.154; 0.155 is installed).
- The theme is a **git submodule** (`themes/stack`). The startup update script runs
  `git submodule update --init --recursive`; if the theme dir is empty, run that yourself
  before building (submodule init needs network access to GitHub).
- Build: `hugo --gc --minify` (outputs to `public/`). Local preview: `hugo server` (port 1313).
