<div align="center">

# d2query-pocketwiki

static pocket wiki for d2query: a github pages site with client-side search and local favorites.

![github pages](https://img.shields.io/badge/github%20pages-ready-0b0b0b?style=for-the-badge)
![static](https://img.shields.io/badge/static-only-ff78c8?style=for-the-badge)
![license](https://img.shields.io/badge/license-mit-0b0b0b?style=for-the-badge)

</div>

---

## what is this?

d2query-pocketwiki is a static website that behaves like a tiny searchable codex.
it runs entirely in the browser:
- search box
- local json dataset
- favorites saved in localStorage

no backend. no database. it is meant for github pages.

---

## live site

after enabling github pages, your url will be:

`https://bellacactus.github.io/<repo-name>/`

example:
`https://bellacactus.github.io/d2query-pocketwiki/`

---

## repo layout

```txt
/
├─ index.html
├─ data/
│  └─ *.json
├─ LICENSE
└─ README.md
```

---

## run locally

quick test (may work by opening `index.html` directly):
- open `index.html` in a browser

recommended (avoids file access edge cases):

```bash
python -m http.server 8000
```

then open:
`http://localhost:8000/`

---

## deploy to github pages

1. repo settings
2. pages
3. build and deployment:
   - source: deploy from a branch
   - branch: main
   - folder: /(root)
4. save

---

## data and favorites

- dataset is loaded from `data/` in the repo
- favorites are stored locally in the browser using `localStorage`
- favorites do not sync between devices (by design)

---

## license

MIT. see `LICENSE`.
