# eduardojsbarroso.github.io

Personal academic homepage for Eduardo Jose Barroso (cosmologist, LAPP, Annecy, France).
Plain HTML/CSS, no build step, hosted on GitHub Pages.

## Publish it

1. **(Recommended) Rename this repo** to `eduardojsbarroso.github.io` in
   GitHub → Settings → General → Repository name. This gives you the clean
   URL `https://eduardojsbarroso.github.io/` instead of
   `https://eduardojsbarroso.github.io/personal_website/`.
   (If you'd rather keep the current repo name, everything below still
   works — just update the URLs in `index.html`/`robots.txt`/`sitemap.xml`
   to include the `/personal_website/` path.)
2. GitHub → Settings → Pages → Source: deploy from branch `main` (or
   whichever branch holds this content), folder `/ (root)`.
3. Wait a minute, then visit the URL GitHub shows you.

## Personalize the content

Everything is in `index.html`. Search for the text `REPLACE` — every
occurrence marks something to fill in:

- Your INSPIRE-HEP, ORCID, and Google Scholar profile URLs
- Your LinkedIn (optional)
- Your email
- Your actual bio / research-interests text
- Your real publication list (title, authors, venue, link) — add one
  `<li>` per paper inside `#publications`
- LAPP address, if you want it more precise

Add your photo as `assets/photo.jpg` (square works best) — the page falls
back to a placeholder silhouette automatically if that file is missing.
Add your CV as `assets/CV.pdf` — the "CV" section links to it directly.

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
