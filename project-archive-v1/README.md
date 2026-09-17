# project-archive
Independent Mechanical Watch Projects

A static archive for one-of-one mechanical watch projects. Built with HTML and shared CSS only. No JavaScript, build step, framework or package manager is required.

## Structure

- `index.html` — general archive homepage.
- `project-001/index.html` — long-form PROJECT No. 001 record.
- `style.css` — shared typography, layout, responsive and reduced-motion styles.
- `assets/general/` — local fonts, font licenses and site icon.
- `assets/project-001/` — reserved for original media; empty except for `.gitkeep`.

All navigation and asset paths are relative, including `../style.css` on the project page. The site supports GitHub Pages project-site hosting at `/project-archive/` and hosting at a domain root. GitHub Pages should publish from **main**, **/(root)**. No additional deployment tooling is required.

## Local preview

From the repository directory, run `python3 -m http.server 8000` and open:

- Homepage: `http://localhost:8000/`
- Project: `http://localhost:8000/project-001/`

To reproduce GitHub Pages project-site paths, run the server from the parent directory instead and open `http://localhost:8000/project-archive/`.

## Adding real media

The empty media fields are intentional. No photographs, stock images or concept renders are included. Each field has a visible pending label. Comments above the project figures suggest filenames and explain how to write accurate alt text.

1. Place the original image in `assets/project-001/` with a descriptive filename.
2. Replace the relevant `.media-slot` with an `<img>` using a relative source, real `width` and `height`, and alt text describing what the photograph actually shows. Use `loading="lazy"` below the fold, not on the hero.
3. Keep the surrounding `<figure>` and update its caption to the actual subject, date or revision. Remove “pending” only when the asset exists.
4. Clearly label concept artwork **CONCEPT RENDER** or **DESIGN STUDY** in its visible caption. Never present it as a build photograph.

A future project-page image source is `../assets/project-001/finished-watch-hero.webp`; on the homepage it is `assets/project-001/finished-watch-hero.webp`. Do not use domain-root paths beginning with `/`.

## Content and verification still required

- Original hero and finished-watch photographs; dial/vector records, iterations, actual print tests and final artwork.
- Actual assembly photographs and dated notes; any box/certificate records that exist.
- Designer/assembler name, recipient details and exact assembly date.
- Confirmation of titanium grade, supplier case rating and strap material.
- Final assembled-watch pressure-test results. The intended “200 M” dial inscription is not a verified water-resistance specification.

Movement values reproduce the supplied project brief, distinguishing rated power reserve from measured performance. Component selection is not evidence of final installation or testing. The site does not imply official Bitfinex affiliation, sponsorship or endorsement.

Nothing goes into the archive unless it is true.

## Typography

Cormorant Garamond and Inter are served locally, with system-font fallbacks. Both use the SIL Open Font License; the corresponding licenses are included in `assets/general/`. Viewing the site requires no third-party requests.
