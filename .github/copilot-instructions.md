# Copilot / AI Agent Guidance for this repository

Purpose: help AI coding agents be immediately productive editing this GitHub Pages (Jekyll) site.

- **Big picture**: This is a Jekyll-based personal website (GitHub Pages). Content pages live under `_pages/` and many page fragments are in `_pages/includes/`. Layouts and reusable snippets are in `_layouts/` and `_includes/`. Assets are under `assets/` and styles are written in `_sass/` (compiled into `assets/css/main.scss`). Data-driven navigation uses `_data/navigation.yml`.

- **Key files/dirs**:
  - [_config.yml](_config.yml) — site config, plugins, and lists directories excluded from build.
  - [run_server.sh](run_server.sh) — convenience script used locally (`bundle exec jekyll liveserve`). Use it if present.
  - [Gemfile](Gemfile) — manages Jekyll/GitHub Pages gems. Run `bundle install` to match the environment.
  - [_pages/includes/](_pages/includes/) — canonical place for small markdown fragments (see `github_myprofile_updater/update.py` which reads these files to regenerate README.md).
  - [assets/css/main.scss](assets/css/main.scss) and `_sass/` — edit SASS here; site uses compressed output in `_config.yml`.
  - [github_myprofile_updater/update.py](github_myprofile_updater/update.py) — script that composes `README.md` from `_pages/includes/` fragments.
  - [google_scholar_crawler/](google_scholar_crawler/) — python crawler with its own `requirements.txt`; this folder is excluded from Jekyll builds per `_config.yml`.
  - [.github/workflows/update_github_myprofile.yaml](.github/workflows/update_github_myprofile.yaml) — CI action that runs `update.py` on page build and pushes changes using `secrets.GHRS_GITHUB_API_TOKEN`.

- **Local dev / build commands** (reproducible from repo files):
  - Install Ruby gems: `bundle install`
  - Start the site: `bundle exec jekyll serve` (or run `./run_server.sh` which calls `bundle exec jekyll liveserve`). If you use `bundle`, always run Jekyll with `bundle exec` to match Gemfile.
  - Build static site: `bundle exec jekyll build`
  - Python helpers: `python3 -m pip install -r google_scholar_crawler/requirements.txt` then run scripts in that folder with `python3`.

- **Repository conventions & patterns** (do not assume generic patterns):
  - Page content is frequently split into small fragments under `_pages/includes/` and then included or composed (see `update.py`). When adding or editing author/home fragments, update these include files rather than single large markdown pages.
  - The `assets/js/_main.js` and plugin/vendor JS files are excluded from Jekyll build in `_config.yml` — treat `assets/js/` as a source folder, not a compiled output.
  - SASS is modular: prefer editing `_sass/*.scss` files (vendor code kept in `assets/_sass/vendor/` style) and import into `assets/css/main.scss`.
  - The repo keeps some automation outside Jekyll: `github_myprofile_updater` directly rewrites `README.md` and the workflow force-pushes it. Be cautious editing those generated files manually.

- **Integration & secrets**:
  - CI uses `secrets.GHRS_GITHUB_API_TOKEN` to push README updates in the workflow. Never hardcode tokens; use `secrets` when adding new workflows.
  - `google_scholar_crawler` depends on `scholarly` and `jsonpickle`; network access and appropriate rate limits are expected when running.

- **When making PRs / edits**:
  - Small content changes: edit `_pages/includes/*` or `_pages/*`. Preview locally with `bundle exec jekyll serve`.
  - Styling changes: update `_sass/` modules and re-build locally to verify CSS output.
  - Automation changes: inspect `.github/workflows/update_github_myprofile.yaml` and `github_myprofile_updater/update.py` before altering behavior; note the workflow runs on `page_build` and force-pushes README updates.

- **Examples from the codebase**:
  - `github_myprofile_updater/update.py` composes `README.md` using fragments from `_pages/includes/` — follow its minimal templating approach when adding new public fragments.
  - `_config.yml` excludes folders like `google_scholar_crawler` and `github_myprofile_updater` from the site build; treat these as tooling directories rather than content.

- **Limitations / unknowns** (check with repo owner if needed):
  - `run_server.sh` calls `jekyll liveserve` (non-standard subcommand). If local environment errors, prefer `bundle exec jekyll serve`.
  - There are no automated tests in the repo; validate changes locally before PRs.

If anything here is unclear or you want more detail (for example, specific SASS compilation steps, JS bundling expectations, or how to extend the GitHub Action safely), tell me which area to expand. I'll iterate on this file.
