# Creating Photo Albums

## Quick Start

1. **Create an image folder** at `assets/images/your-album-name/`
2. **Drop your photos** into that folder
3. **Create a page** in this `photos/` folder:

```markdown
---
layout: album
title: Your Album Title
folder: your-album-name
---
```

Done! All images in the folder appear automatically in a responsive grid with lightbox.

---

## Full Options

```markdown
---
layout: album
title: Summer Vacation
date: 2025-08-15
description: |
  Two weeks exploring the Pacific coast.
  Found some amazing hidden beaches.
folder: summer-vacation
permalink: /photos/summer-vacation/
---
```

| Field | Required | Description |
|-------|----------|-------------|
| `layout` | Yes | Always `album` |
| `title` | Yes | Album title shown on page |
| `folder` | Yes* | Folder name inside `assets/images/` |
| `date` | No | Shows as "August 2025" format |
| `description` | No | Intro text (supports markdown) |
| `permalink` | No | Custom URL (defaults to filename) |

*Or use `photos:` for manual control (see below)

---

## Manual Photo List

If you need custom order or captions, use `photos:` instead of `folder:`:

```markdown
---
layout: album
title: Favorites
photos:
  - src: /assets/images/photo1.jpg
    alt: Sunset over the ocean
    caption: Big Sur, California
  - src: /assets/images/photo2.jpg
  - src: /assets/images/photo3.jpg
    caption: Morning light
---
```

---

## Supported Formats

`.jpg` `.jpeg` `.png` `.gif` `.webp`

---

## Tips

- Images are sorted alphabetically by filename
- Use numbered prefixes for custom order: `01-first.jpg`, `02-second.jpg`
- Large images work fine—they're displayed responsively

