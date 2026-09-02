# FAB20 — Content

Open content base for [FAB20](https://fab20.ee), the coworking and hackspace in Tallinn, Estonia.

This repository holds equipment pages, articles, FAQs, event descriptions, member projects, and static pages. Content is served by the main web application via the GitHub API and published on [fab20.ee](https://fab20.ee). A push to `main` goes live within seconds — there is no separate deploy step.

## Repository layout

| Folder | What's there |
|---|---|
| `equipment/` | Equipment pages. Each tool is its own landing page (e.g. "laser cutting Tallinn"). |
| `articles/` | Blog articles. |
| `faqs/` | Frequently asked questions, one folder per category. |
| `events/` | Public event descriptions (board games nights, workshops, etc.). |
| `projects/` | Wall of Fame — projects made by hackspace members. |
| `pages/` | Static pages (About, Privacy, Terms, Rules, Cookies). |
| `redirects.yml` | 301 redirects for renamed slugs. |

Every content item is a **folder** holding one `meta.yml` and one `index.{lang}.md` per language:

```
equipment/co2-laser-1060-100w/
├── meta.yml            # shared across languages: slugs, status, prices, links
├── index.en.md         # English text
├── index.et.md         # Estonian text
├── index.ru.md         # Russian text
└── images/
    ├── cover.jpg
    └── gallery-01.jpg
```

The folder name is a technical identifier for humans and git history — it is never shown to
visitors. Articles and events may use a date prefix (`articles/2026-04-laser-tips/`) so the
file tree sorts chronologically.

**Folders starting with `_` are ignored by the site.** Use them for templates and drafts —
where a section has a `_template/` folder, it is a ready-to-copy skeleton.

## How content becomes a URL

Public URLs are built from the localized slugs in `meta.yml`, and the path segment is
localized too:

| Content | en | et | ru |
|---|---|---|---|
| Zones | `/en/hackspace` | `/et/hackspace` | `/ru/hackspace` |
| Equipment | `/en/equipment/{slug}` | `/et/seadmed/{slug}` | `/ru/oborudovanie/{slug}` |
| Articles | `/en/articles/{slug}` | `/et/artiklid/{slug}` | `/ru/stati/{slug}` |
| Events | `/en/events/{slug}` | `/et/sundmused/{slug}` | `/ru/meropriyatiya/{slug}` |
| Projects | `/en/projects/{slug}` | `/et/projektid/{slug}` | `/ru/proekty/{slug}` |
| Pages | `/en/{slug}` | `/et/{slug}` | `/ru/{slug}` |
| FAQ | `/en/faq` | `/et/kkk` | `/ru/faq` |

Slugs use lowercase latin letters, digits, and hyphens — no diacritics, so that URLs survive
copy-pasting (`co2-laserloikur`, not `co2-laserlõikur`).

> **The English slug is special.** The application database references content by its English
> slug (equipment rentals, event registrations). Renaming an English slug requires a data
> migration, so treat it as permanent. Estonian and Russian slugs can be changed freely — just
> add a redirect.

## Localization

The site serves three languages: Estonian (`et`), English (`en`), Russian (`ru`).

Each content item ships **three files**: `index.en.md`, `index.et.md`, `index.ru.md`.

If a language file is missing, the site shows the fallback language with a small notice
("this text is only available in English so far") rather than hiding the page. The default
fallback is English; legal pages override it to Estonian via `fallbackLang` in `meta.yml`,
because the jurisdiction is Estonian.

## `meta.yml` — shared metadata

### Common to every content type

```yaml
# Localized slugs — these become the public URL
slug:
  en: co2-laser-cutter-100w
  et: co2-laserloikur-100w
  ru: lazernyy-stanok-co2-100w

status: active        # see the status table below
order: 10             # sort order in listings, lower comes first

cover: images/cover.jpg
gallery:
  - images/gallery-01.jpg
  - images/gallery-02.jpg
```

### Statuses

| Status | In listings | Own page | In sitemap |
|---|---|---|---|
| `active` / `published` | yes | yes | yes |
| `maintenance` | yes, marked as under maintenance | yes | yes |
| `retired` | no | yes, marked as retired | no |
| `cancelled` (events only) | no | yes, marked as cancelled | no |
| `draft` | no | no (visible only on a developer machine) | no |

`retired` keeps the page alive on purpose: inbound links and search results built up over
years should not turn into 404s.

### Equipment

```yaml
category: cutting     # groups the catalog: cutting | printing | electronics | measurement | optics | office
zone: hackspace       # coworking | hackspace — which room the tool lives in

rental:               # only if the tool can be taken out of the space
  enabled: false
  dailyRate: 0.00
  deposit: 0.00

induction:
  required: true      # a safety briefing is required before first use

serial: "1060-100W-2024-01"        # serial number, used in rental agreements
code: P12             # sticker code (1–8 letters/digits, unique); the sticker's QR opens fab20.ee/p/P12
                      # A page with `layout: rental` (pages/rental) lists every tool with rental.enabled: true

externalLinks:
  - { type: manual,  label: "Factory manual", url: "https://github.com/fab20ee/docs/raw/main/100W%201060%20CO2%20laser.pdf" }
  - { type: youtube, label: "Tutorial",       url: "https://youtu.be/..." }
  - { type: github,  label: "Templates",      url: "https://github.com/..." }

# Subscription slugs (from the application database) that grant access to this tool
relatedSubscriptions: [hackspace-monthly, hackspace-day]
```

`zone` matters because a coworking-only membership does not open the hackspace room — the
catalog has to state which plan a tool needs.

**Factory manuals are not stored in this repository.** They live in
[fab20ee/docs](https://github.com/fab20ee/docs) and are linked as `externalLinks` of type
`manual` — those PDFs are tens of megabytes and the site keeps all content in memory.

### Articles

```yaml
status: published                 # draft | published
publishedAt: 2026-04-18
updatedAt: 2026-05-02             # optional
author: { name: "Sasha Sovenko", url: "https://..." }
tags: [laser, materials]
relatedEquipment: [co2-laser-cutter-100w]   # English slugs
```

### Events

```yaml
status: active                    # draft | active | cancelled
startsAt: 2026-09-12T19:00:00     # local time, Europe/Tallinn
endsAt:   2026-09-12T22:00:00
zone: coworking
capacity: 16                      # omit for unlimited
price: 0.00                       # shown on the page; paid on site
currency: EUR
registration:
  enabled: true
  membersOnly: false
  deadline: 2026-09-12T12:00:00
tags: [board-games, social]
```

Past events stay published as an archive; they move to a "past events" section and
registration closes automatically.

### Projects (Wall of Fame)

```yaml
status: published
completedAt: 2026-04-20
author: { name: "Mart T.", url: null }             # display name, not a site account
equipmentUsed: [co2-laser-cutter-100w, cnc-router] # English slugs
links:
  - { type: github, label: "Source", url: "https://github.com/..." }
featured: true
tags: [woodwork, arduino]
```

`equipmentUsed` works both ways: the project page credits the machines, and each machine's
page automatically gains a "made here" section.

### Static pages

```yaml
status: published
updatedAt: 2026-03-01     # "last updated", required on legal pages
fallbackLang: et          # defaults to en
version: "1.2"            # optional, for versioned terms

zone: hackspace           # optional — see below
```

#### The home page

The site's front page is content too. `pages/home/` carries `layout: home`, has no slug (it
answers on `/{lang}`), and its text lives as **structured blocks** in the frontmatter of each
`index.{lang}.md`:

```yaml
# pages/home/meta.yml
layout: home
status: published
featuredEquipment: [co2-laser-cutter-100w, 3d-printer-anycubic-kobra-3-combo]
```

```yaml
# pages/home/index.en.md — frontmatter
hero:
  eyebrow: "Pärnu mnt. 30, Tallinn · 24/7"
  title: "A quiet place to work. A workshop to build in."
  text: "Coworking and hackspace under one roof, but in separate rooms."
  portals:
    - { zone: coworking, label: "For work",     title: "Coworking", note: "Quiet, wifi, coffee" }
    - { zone: hackspace, label: "For projects", title: "Hackspace", note: "3D printers, laser" }
zones:
  heading: "Two rooms, a wall between them"
  text: "..."
  cards:
    - zone: hackspace
      badge: "Hackspace"
      title: "A workshop for what you can't make at home"
      text: "..."
      bullets: ["Room for noisy work", "Consumables included within reason"]
howItWorks:
  heading: "How to get access"
  text: "..."
  steps:
    - { title: "Sign in with Smart-ID", text: "..." }
equipment:
  heading: "What's in the hackspace"
  text: "..."
  linkLabel: "All equipment"
pricing:
  heading: "Plans"
  text: "..."
```

Why named fields instead of free markdown: the composition of the page is fixed by the design, and
markdown would not survive it. Blocks you leave out are simply not rendered.

Links, not copies: `zone` points at a zone landing page and `featuredEquipment` at equipment
cards, so titles and URLs come from that content and stay localized.

**Prices are not here.** Plans live in the application database, and repeating their numbers in git
would eventually disagree with what the payment provider charges. The content only supplies the
heading and the lead-in of the pricing section.

#### Zone landing pages

The site has no single equipment catalog. Instead there are two landing pages — one per room —
and each is both a description of that room and the list of what stands in it. A page becomes a
zone landing by carrying a `zone` field:

```yaml
# pages/hackspace/meta.yml
slug: { en: hackspace, et: hackspace, ru: hackspace }
status: published
zone: hackspace           # coworking | hackspace
```

Write the description in `index.{lang}.md` as usual — what the room is, what is included in the
price, which plan opens it. The equipment list is added automatically from every tool whose own
`meta.yml` says `zone: hackspace`, so the two can never drift apart.

Each zone may have **at most one** landing page. Equipment in a zone with no landing page is not
listed anywhere, and the site reports that as a warning.

### FAQ categories

```yaml
status: published
order: 10
```

FAQ categories have no slugs of their own — every category is rendered as a section of the
single `/{lang}/faq` page.

## `index.{lang}.md` — localized text

```markdown
---
title: "CO2 Laser Cutter 100 W"
seoDescription: "Access to a 100 W CO2 laser cutter in central Tallinn. Cut plywood, acrylic, leather. Open 24/7."
specs:
  - { label: "Power",      value: "100 W CO2" }
  - { label: "Work area",  value: "1000 × 600 mm" }
  - { label: "Materials",  value: "plywood, acrylic, leather, paper" }
---

An opening paragraph for a first-time visitor: what this machine does and why someone
would want access to it.

## Safety

...

## How to use

...
```

Notes:

- **Do not repeat the title as an `# H1`** in the body — the site renders `title` as the page
  heading. Start with text, and use `## H2` for sections.
- `seoDescription` is what shows up in search results. Aim for 140–160 characters, mention the
  city, and write it for a human.
- `seoTitle` (optional) replaces `title` in the browser tab and in search results only; the page
  heading stays `title`. Use it where the heading is short but people search for more words:
  "Hackspace in Tallinn: laser, 3D printing, electronics 24/7". Up to ~55 characters — the site
  name is appended.
- `specs` is optional but recommended for equipment: it renders as a consistent table across
  all tools and feeds structured data to search engines. Labels are translated, so they live
  here rather than in `meta.yml`.
- Markdown supports headings, lists, tables, links, images, and code blocks.

### FAQ format

Inside a FAQ category, **each `## H2` is a question** and everything until the next `## H2`
is the answer:

```markdown
---
title: "Billing"
---

## How do I pay for my membership?

By card through Stripe, right after you sign the membership agreement.

## Can I pause my subscription?

...
```

## Images

- Put images next to the content: `images/cover.jpg`, `events/.../cover.jpg`.
- Upload one reasonably sized original (**up to about 2000 px wide**, JPEG or PNG). The site
  generates the smaller variants and WebP versions itself — `thumb` (320 px), `card` (640 px),
  `hero` (1600 px).
- Do not commit multi-megabyte camera originals; resize first.
- Photos of machines: shoot the whole machine for `cover`, put details and sample work in
  `gallery`.

## Slugs and redirects

If you rename a slug, **always** add an entry to `redirects.yml` so the old URL keeps its
search ranking:

```yaml
redirects:
  - from: /en/equipment/old-name
    to:   /en/equipment/new-name
```

## Adding new content

1. Copy the `_template/` folder of the matching section to `<section>/<your-folder>/`.
2. Fill in `meta.yml` — localized slugs first.
3. Write `index.en.md`, `index.et.md`, `index.ru.md`.
4. Add images to `images/`.
5. Open a Pull Request. Once merged, the change is live on the site within seconds.

## License

Content in this repository is released under Creative Commons Attribution-ShareAlike 4.0
(CC BY-SA 4.0) unless stated otherwise inside a specific article or project. Member projects:
copyright stays with the author.

## Contributing

Anyone can propose improvements via Pull Request. Changes are reviewed and merged by the
FAB20 team.

If you are a member of the hackspace and want to add your own project, send a PR to
`projects/` — we are happy to feature your work.
