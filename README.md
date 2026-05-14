# RW.HackSpace — Content

Open content base for the [RW.HackSpace](https://fab20.ee) hackspace and coworking in Tallinn, Estonia.

This repository holds equipment pages, articles, FAQs, event descriptions, member projects, and static pages. Content is served by the main web application via the GitHub API and published on [fab20.ee](https://fab20.ee).

## Repository layout

| Folder | What's there |
|---|---|
| `equipment/` | Equipment pages. Each tool is its own SEO landing page (e.g. "laser cutting Tallinn"). |
| `articles/` | Blog articles. |
| `faqs/` | Frequently asked questions, grouped by category. |
| `events/` | Public event descriptions (board games nights, workshops, etc.). |
| `projects/` | Wall of Fame — projects made by hackspace members. |
| `pages/` | Static pages (About, Privacy, Terms, Rules). |
| `redirects.yml` | 301 redirects for renamed slugs. |

## Localization

The site serves three languages: Estonian (`et`), English (`en`), Russian (`ru`).

Each content item ships **three files**: `index.en.md`, `index.et.md`, `index.ru.md`. If a file in a given language is missing, the site falls back to English for most content (Estonian for government-mandated pages).

Shared metadata (slugs, prices, flags) lives in `meta.yml` next to the localized files — one per content item, common across all languages.

## Frontmatter — specification

### `meta.yml` (shared across languages)

```yaml
# Localized slugs — these become the public URL on the site
slug:
  en: laser-engraver-co2
  et: co2-lasergraveerimine
  ru: lazernyy-graver-co2

# Status — controls whether the page is shown on the site
status: active        # active | maintenance | retired
category: cutting     # used for grouping in the catalog
order: 10             # sort order within the category

# Images (paths relative to meta.yml)
cover: images/cover.jpg
gallery:
  - images/gallery-01.jpg
  - images/gallery-02.jpg

# Rental (only if the equipment can be taken out of the space)
rental:
  enabled: false
  dailyRate: 0.00
  deposit: 0.00

# Whether an induction (safety briefing) is required before use
induction:
  required: false

# External resources — tutorials, manuals, source code
externalLinks:
  - { type: youtube, label: "Tutorial",     url: "https://youtu.be/..." }
  - { type: manual,  label: "User manual",  url: "https://example.com/manual.pdf" }
  - { type: github,  label: "Templates",    url: "https://github.com/..." }

# Subscription slugs (from the application database) that grant access to this equipment
relatedSubscriptions: [hackspace-monthly, hackspace-day]
```

### `index.{lang}.md` (localized)

```markdown
---
title: "CO2 Laser Engraver"
seoDescription: "Access to the CO2 laser engraver at the Tallinn hackspace. Cut plywood, acrylic, leather. EUR 19/day."
---

# Page title

Description for both the visitor and search engines. Markdown supports headings,
lists, tables, links, images, and code blocks.

## Technical specifications

| Parameter | Value |
|---|---|
| Power | 80W CO2 |
| Work area | 600×400 mm |
| Supported materials | plywood, acrylic, leather |

## Safety

...

## How to use

...
```

## Adding new equipment

1. Copy the `equipment/_example-laser-engraver/` folder to `equipment/<your-slug>/`.
2. Replace the photos in `images/`.
3. Update `meta.yml` — localized slugs, prices, links.
4. Replace the content in `index.{en,et,ru}.md`.
5. Open a Pull Request — after review, the changes go live on the site.

## Adding an article or a project

Same flow: drop a folder under `articles/<slug>/` or `projects/<slug>/`, fill in `meta.yml` and the per-language files.

## Slugs and redirects

The slug becomes part of the URL: `/{lang}/equipment/{slug}`. If you rename a slug, **always** add a record to `redirects.yml` so the old URL returns a 301 redirect and SEO is preserved:

```yaml
# redirects.yml
redirects:
  - from: /en/equipment/old-name
    to:   /en/equipment/new-name
```

## License

Content in this repository is released under Creative Commons Attribution-ShareAlike 4.0 (CC BY-SA 4.0) unless stated otherwise inside a specific article or project. Member projects: copyright stays with the author.

## Contributing

Anyone can propose improvements via Pull Request. Changes are reviewed and merged by the RW.HackSpace team.

If you are a member of the hackspace and want to add your own project, send a PR to `projects/` — we are happy to feature your work.
