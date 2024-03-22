# jn2024

This is the repository for the informational website about Cascade Orienteering Club's Columbia Gorge Classic event in March 2024, which is also the 2024 OUSA Junior National Championships

## How it's Served

The site overall uses Jekyll. Github Actions runners build and deploy automatically when changes are merged into `main` or `liveprod`.

This one repository is hooked into two different Azure Static Web Apps, and there is a separate Github Actions runner for each.

### Live Site

The live site is served at https://jn2024.cascadeoc.org
When code is merged to `liveprod` branch in this repository, a github actions runner builds and deploys to azure app `kind-tree-{redacted}`.

### Test / Preview Site

The preview site is served at https://jn2024-test.cascadeoc.org
When code is merged to `main` branch in this repository, a github actions runner builds and deploys to azure app `ambitious-grass-{redacted}`.

### Development reminders

Just run `jeykll serve` to launch the site during development.

Might need to run `bundle exec jekyll serve` when running in windows rather than WSL/linux.