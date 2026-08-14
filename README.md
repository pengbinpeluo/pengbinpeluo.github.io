# pengbinpeluo.github.io — Jekyll rebuild

A Jekyll rebuild of Bin Peng's personal academic site, migrated from the old
Hugo/blogdown + Wowchemy "Academic" theme repo at `website_binpeng`.

Builds and serves cleanly with `bundle exec jekyll serve` (verified locally).

## What's here

- `_config.yml` — site config: author info (name, role, department/university
  links, office affiliations, email, office address), the WACI Lab URL, and
  social links.
- `_data/publications.yml` — all 100 journal publications as structured
  data, cross-checked against the WACI Lab site and Bin Peng's CV. `authors`
  may contain inline HTML: `<strong>` bolds Bin Peng's own name, and
  `<span class="lab-member">` marks co-authors who are/were lab members
  supervised by Dr. Peng (matches the CV's bold-italic-underline convention).
  Rendered by `_includes/pub-entry.html`. Numbering on the publications page
  runs continuously from 100 (newest) to 1 (oldest) across the whole list.
- `_data/experience.yml` — professional experience timeline.
- `_data/education.yml` — education timeline.
- `_data/honors.yml` — honors & awards.
- `_includes/pub-entry.html` — renders one publication entry.
- `_layouts/default.html` — the single shared page layout/nav/footer. Also
  contains a small script that opens any off-site link in a new tab.
- `index.md` — bio/home page (photo, contact info, research interests).
- `experience.md` — professional experience, education, and honors & awards.
- `publications.md` — full publication list.
- `engagement.md` — extension/outreach and scientific community engagement.
- `teaching.md` — teaching & mentoring.
- `hiring.md` — links out to the WACI Lab hiring page.
- `assets/css/main.css` — all styling, plain CSS, no build step.
- `assets/img/bin-peng.jpg` — profile photo.

## Not version-controlled (by design)

`CLAUDE.md` (an internal project handoff note, not meant for the public
repo) is excluded from both the Jekyll build (`_config.yml`'s `exclude:`)
and from git (`.gitignore`) — see that file if you're picking this project
up and need the history/context it records.

## Building locally

```bash
bundle install
bundle exec jekyll serve
```

Then open http://localhost:4000.

## Deploying

Simplest path: push this repo (or this content, if reusing the existing
`pengbinpeluo.github.io` repo) to GitHub and let GitHub Pages' native Jekyll
build handle it — no local build-and-commit step required, unlike the old
Hugo/blogdown workflow.
