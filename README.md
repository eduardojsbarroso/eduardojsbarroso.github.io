# eduardojsbarroso.github.io

Personal academic homepage for Eduardo Jose Barroso (cosmologist, LAPP, Annecy, France).
Plain HTML/CSS, no build step, hosted on GitHub Pages.

## Structure

A landing page (`index.html`) with your photo and six clickable cards, each
linking to its own page:

- `about.html` — background / who you are
- `research.html` — research interests
- `publications.html` — papers and preprints
- `cv.html` — CV download, plus PhD and Master's thesis downloads
- `profiles.html` — INSPIRE-HEP, ORCID, Google Scholar, GitHub, LinkedIn
- `contact.html` — email and address

Every page shares `assets/style.css` and a consistent top nav bar so you can
jump between sections from anywhere, not just the home page.

## Publish it

1. Repo is already at `eduardojsbarroso/eduardojsbarroso.github.io`, so the
   URL is `https://eduardojsbarroso.github.io/`.
2. GitHub → Settings → Pages → Source: deploy from branch `main`, folder
   `/ (root)`.
3. Wait a minute, then visit the URL GitHub shows you.

## Personalize the content

Bio, research, publications, CV, positions, and contact are filled in with
real content already. One thing still needs `REPLACE`d:

- **Google Scholar link** and **LinkedIn** (optional) — in `index.html`
  (JSON-LD `sameAs`), `publications.html`, and `profiles.html`.

Already in place: `assets/photo.jpg`, `assets/CV.pdf`,
`assets/thesis-phd.pdf`, `assets/thesis-msc.pdf`.

## Why this helps you show up when people Google your name

- The `<title>`, headings, and body text all repeat your full name
  ("Eduardo Jose Barroso"), which is what search engines match against.
- The embedded JSON-LD (`Person` schema) tells Google explicitly "this
  page is about a person named X, affiliated with LAPP, and here are
  their other profiles" via `sameAs`.
- Once published, submit the URL in [Google Search
  Console](https://search.google.com/search-console) and request
  indexing — this is the single biggest lever for showing up quickly.
- **Backlinks matter more than on-page tweaks.** Add this URL to your
  INSPIRE-HEP profile, ORCID profile, Google Scholar profile, and your
  LAPP staff page if one exists. A link from LAPP's institutional site in
  particular carries a lot of weight with Google.

## Local preview

No build tools needed — just open `index.html` in a browser, or run a
tiny local server:

```
python3 -m http.server 8000
```

then visit `http://localhost:8000/`.
