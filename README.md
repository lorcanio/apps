# apps.lorcan.dev

Public site for lorcan.dev apps: privacy policies and support pages. Jekyll, GitHub Pages, no theme, no JavaScript, no external requests. Public repository: nothing private goes in it.

- `_layouts/`, `_includes/`, `assets/css/site.css`: the whole design.
- `_data/apps.yml`: the apps list on the home page (empty list shows "first app coming soon").
- `/privacy`, `/support`: site-level pages (the footer links).
- `_template-app/`: copy for a new app, see its README. Not published.
- `logo.svg`, `logo-dark.svg`: the lorcan.dev wordmark, letters outlined from Newsreader Medium (SIL Open Font License 1.1, free for commercial use) with an ultramarine `#2430c8` stop. `_includes/logo.html` is the inline copy the site uses (colours from CSS).
- `CNAME`: custom domain. Do not edit.

Preview: `bundle install && bundle exec jekyll serve`, then open http://127.0.0.1:4000.
