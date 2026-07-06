# Al Koran Korvettes — Website

The public website for the Al Koran Korvettes, a parade driving unit of the
Al Koran Shriners. Built as a single, dependency-free HTML file so it is easy
to host and easy to maintain.

## What's here

```
site/
├── index.html                 ← the whole website (edit this)
├── CNAME                       ← custom domain (alkorankorvettes.com)
├── .nojekyll                   ← tells GitHub Pages to serve files as-is
└── assets/
    ├── tevis-logo.png
    └── pictures/               ← all photos (drop new ones here)
        ├── korvettes-banner.jpg
        ├── memorial-day-krazy-kops-chagrin-falls-2026.png
        ├── memorial-day-in-the-parade-2026.png
        ├── memorial-day-unit-photo-1-2026.png
        └── memorial-day-unit-photo-2-2026.png
```

## Publishing on GitHub Pages

1. Copy the **contents of this `site/` folder** into the root of your
   `alkorankorvettes/alkorankorvettes` repository (so `index.html` sits at the
   repo root).
2. In the repo, go to **Settings → Pages** and set the source to
   **Deploy from a branch**, branch **main**, folder **/ (root)**.
3. The included `CNAME` file already points at **alkorankorvettes.com** — set
   that domain in **Settings → Pages → Custom domain** and add the DNS records
   your registrar shows (an `A`/`ALIAS` or `CNAME` to GitHub Pages).
4. Give it a couple of minutes; the site goes live at
   https://alkorankorvettes.com/.

> Prefer to keep the site in a subfolder? Move these files into a `/docs`
> folder instead and choose the **/docs** option in Settings → Pages.

## Editing the site — no coding needed

Open `index.html` in any text editor.

- **Text** (headlines, mission, contact info): find it in the page and type
  over it. Sections are clearly marked with `<!-- ==== SECTION ==== -->`.
- **Logo**: replace the placeholder "AK" circle in the header (and footer) —
  the header comment shows how. Drop your crest into `assets/pictures/`.
- **Events, News, and Gallery photos**: scroll to the bottom `<script>` and edit
  the three lists — `EVENTS`, `NEWS`, and `PHOTOS`. Each item is one line. Copy
  a line, paste it, change the details, save. New categories you type in an
  event automatically appear as schedule filter buttons.
- **Photos**: put the image file in `assets/pictures/`, then reference it as
  `assets/pictures/your-file.jpg` in the `NEWS` or `PHOTOS` list.

That's the whole workflow — edit, save, commit, and GitHub Pages updates the
live site.

---

*Website designed and powered by Tevis Engineering Solutions, LLC.*
