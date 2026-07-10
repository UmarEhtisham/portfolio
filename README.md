# Portfolio — Muhammad Umar Ehtisham Mian

Personal portfolio site built with Astro. Live at [umarehtisham.vercel.app](https://umarehtisham.vercel.app).

## Stack

- Astro 7 (static, no UI framework)
- Vanilla CSS (`src/styles/global.css`)
- `astro:transitions` (`ClientRouter`) for page transitions

## Structure

```
src/
├── layouts/
│   └── Layout.astro          # shared shell: nav, meta, transitions
├── pages/
│   ├── index.astro           # hero, arc, currently, skills, about, career, projects, certifications, contact
│   ├── thanks.astro          # post-contact-form confirmation
│   └── projects/
│       ├── hsy.astro
│       ├── netdressed.astro
│       └── digital-marketing-ai-worker.astro
public/
├── avatar.png / avatar.jpg
├── resume.pdf
└── favicon.ico / favicon.svg
```

## Commands

| Command           | Action                                   |
| ------------------ | ----------------------------------------- |
| `npm install`       | Install dependencies                      |
| `npm run dev`       | Start local dev server (`localhost:4321`) |
| `npm run build`     | Build production site to `./dist/`        |
| `npm run preview`   | Preview the production build locally      |

Requires Node >= 22.12.0.

## Notes

- No CMS/content collections — page content is hand-authored directly in `.astro` files.
- Update resume by replacing `public/resume.pdf`.
- Nav anchors (`arc`, `currently`, `skills`, `about`, `career`, `projects`, `certifications`, `contact`) must match section `id`s in `index.astro` — keep in sync if sections are renamed.
