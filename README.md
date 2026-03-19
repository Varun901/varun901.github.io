# varun901.github.io

Personal website for Varun Jain — researcher and graduate of McMaster University's Integrated Biomedical Engineering and Health Sciences (iBioMed) program.

Live at [varun901.github.io](https://varun901.github.io)

---

## Overview

A single-page personal site covering:

- **About** — background, skills, and interests
- **Publications** — dynamically fetched from [ORCID](https://orcid.org/0000-0002-1366-9331) at page load, supplemented with institutional repository works from MacSphere
- **Projects** — software projects built across hackathons, coursework, and personal work
- **Contact** — form powered by [Formspree](https://formspree.io)

## Stack

Built with plain HTML, CSS (Bootstrap 4), and vanilla JavaScript. No build step required.

| Dependency | Purpose |
|---|---|
| Bootstrap 4 | Layout and base styles |
| Font Awesome 4.7 | Icons |
| jQuery | DOM and scroll animations (template dependency) |
| Formspree | Contact form backend |
| ORCID Public API | Live publication data |

## Publications

Publications are fetched at runtime from the [ORCID public API](https://pub.orcid.org/v3.0/0000-0002-1366-9331/works) — no API key required. Two additional works hosted on McMaster's MacSphere institutional repository are included as a static supplement and merged at render time.

To add a new publication: add it to your ORCID profile and it will appear automatically. For works without a DOI (e.g. institutional repository items), add an entry to the `STATIC_WORKS` array in `index.html`.

## Development

No build tooling needed. Open `index.html` directly in a browser or serve with any static file server:

```bash
npx serve .
```

## Deployment

Deployed via GitHub Pages from the `master` branch.
