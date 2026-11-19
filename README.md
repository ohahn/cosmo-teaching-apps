# Interactive cosmology

Interactive figures from the lecture course Cosmology (280416 VU) at the University of Vienna.
Each app is one self-contained HTML file that runs entirely in the browser, offline too.

**Licence:** the code is free software under the GNU General Public License, version 3 or later
(`LICENSE`); the explanatory text is under CC BY-SA 4.0 (`LICENSE-TEXT.md`). Third-party
components and data: `THIRD-PARTY.md`.

**Use them:** open `index.html` (or the published site) and pick an app.

## Layout

| Path | Content |
|---|---|
| `index.html` | Landing page: one card per app, list of archived versions |
| `latest/` | Current version of every app |
| `2026/`, … | Frozen versions. They are never rebuilt, so links into them stay valid |
| `thumbs/<app>.jpg` | Optional screenshots shown on the cards (16:9, about 1280×720) |

## Updating (from the lecture repository)

The apps are built from the sources in `slides/apps/` of the lecture repository:

```bash
python3 slides/make_site.py                 # rebuild latest/ and the landing page
python3 slides/make_site.py --freeze 2026   # also keep the current state as 2026/
```

Then commit and push this folder; GitHub Pages republishes within a minute.

## Publishing on GitHub Pages (once)

1. Create an empty public repository on GitHub, e.g. `cosmo-apps`.
2. In this folder: `git add -A && git commit -m "Interactive cosmology apps"`,
   `git remote add origin git@github.com:<user>/cosmo-apps.git`, `git push -u origin main`.
3. On GitHub: *Settings → Pages → Build and deployment*: source *Deploy from a branch*,
   branch `main`, folder `/ (root)`.
4. The site appears at `https://<user>.github.io/cosmo-apps/`.

Optional: connect the repository to [Zenodo](https://zenodo.org) (GitHub integration) so every
GitHub release gets a citable DOI.
