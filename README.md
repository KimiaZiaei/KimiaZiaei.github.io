# KimiaZiaei.github.io

Personal academic website of Kimia Ziaei, built with plain [Jekyll](https://jekyllrb.com/) and no theme gem.
GitHub Pages builds it automatically on every push (Settings → Pages → Source: *Deploy from a branch*, pick the branch, `/ (root)`).

Because the repository is `KimiaZz/KimiaZiaei.github.io`, the site is served at
https://kimiazz.github.io/KimiaZiaei.github.io/ (`baseurl` in `_config.yml`).
If the repository is renamed to `KimiaZz.github.io`, set `baseurl: ""` and the site moves to https://kimiazz.github.io/.

## Updating content

Most content lives in YAML files, so an update is usually a one-line edit:

| What | File |
|---|---|
| Name, links, photo, CV path | `_config.yml` (`author:`) |
| Navigation menu | `_config.yml` (`navigation:`) |
| Bio and research interests | `index.md` |
| Papers (shows "TBA" while empty) | `_data/publications.yml` |
| Education | `_data/education.yml` |
| CV | replace `files/KimiaZiaei_CV.pdf` |

To change the photo, replace `assets/img/profile.jpg` (square, about 400×400).
To add LinkedIn or Google Scholar links, uncomment `linkedin:` or `google_scholar:` in `_config.yml`; the sidebar picks them up.

## Running locally

```sh
bundle install
bundle exec jekyll serve
```

Then open http://localhost:4000/KimiaZiaei.github.io/.

## Structure

```
_config.yml        site settings, profile, navigation
_data/             content (papers, education)
_includes/         head, masthead, sidebar, icons, list partials
_layouts/          default (masthead + sidebar), page
assets/css/        main.css (light and dark themes)
assets/fonts/      self-hosted Inter and Source Serif 4
files/             CV
```
