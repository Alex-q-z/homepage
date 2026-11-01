# Qizheng (Alex) Zhang — homepage

Source for my personal website. Built with [Jekyll](https://jekyllrb.com/) and the [al-folio](https://github.com/alshedivat/al-folio) starter, and deployed to GitHub Pages by GitHub Actions.

- Preview: https://alex-q-z.github.io/homepage/
- Current site: https://alex-q-z.github.io/ (old repo, unchanged until go-live)

## Where things live

| To change | Edit |
| --- | --- |
| Bio, profile photo, home page sections | `_pages/about.md`, `assets/img/prof_pic.jpg` |
| News | one file per item in `_news/` (`YYYY-MM-DD-name.md`) |
| Publications | `_bibliography/papers.bib` (the `topic` field sets the section; `selected = {true}` puts it on the home page) |
| Blog posts | `_posts/` (copy `2026-11-01-post-template.md`) |
| Talks | `_pages/talks.md` |
| CV | replace `QizhengZhang-CV.pdf` |
| Name, links, site settings | `_config.yml`, `_data/socials.yml` |
| Colors and small style tweaks | `_sass/_custom.scss` |

Old URLs keep working: `/research.html` redirects to `/publications/`, and `/QizhengZhang-CV.pdf`, `/why-fail.pdf` and `/papers/*.bib` stay at the same paths.

## How it deploys

Every push to `main` runs `.github/workflows/deploy.yml`, which builds the site and publishes it to the `gh-pages` branch. In the repo's **Settings → Pages**, the source must be **Deploy from a branch → `gh-pages` / root**.

## Preview locally (optional)

With Docker: `docker compose up`, then open http://localhost:8080/homepage/.

With Ruby 3.3: `bundle install && bundle exec jekyll serve`, then open http://localhost:4000/homepage/.

## Going live

1. Rename the old repo `alex-q-z.github.io` to something like `homepage-legacy` and turn off its Pages.
2. Rename this repo to `alex-q-z.github.io`.
3. In `_config.yml`, set `baseurl:` to empty and push.
4. Optional custom domain: add it under Settings → Pages, point the DNS records at GitHub, then set `url:` in `_config.yml` to the new domain.

## Credits

Theme: [al-folio](https://github.com/alshedivat/al-folio) (MIT License).
