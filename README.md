# THUNDER Research Group website

This is a static website for the THUNDER Research Group. It has English and Korean pages and uses plain HTML, CSS, and JavaScript. There is no build step or package installation.

## Where to find things

| Path | What it contains |
| --- | --- |
| `index.html`, `research.html`, `people.html`, `publications.html`, `join.html` | English pages |
| `ko/` | Korean versions of those pages |
| `assets/css/style.css` | Shared layout, colors, and responsive styles |
| `assets/js/main.js` | Shared navigation, theme toggle, filters, and home page canvas |
| `assets/img/people/`, `assets/img/group/` | Images used by the site |
| `people/`, `tools/make-avatars.py` | Source portraits and the optional avatar cropping script |

## Editing the site

- Edit page content directly in the relevant HTML file. Update the corresponding page in `ko/` when the content should appear in both languages.
- The header and footer are repeated in each HTML file, so update them on every page when changing navigation or contact details.
- Change colors and other shared styles near the top of `assets/css/style.css`. Shared interactions are in `assets/js/main.js`.
- To add a publication, copy an existing `<article class="pub">` in `publications.html` and update its `data-tags` value so the filters work. Do the same in `ko/publications.html` if needed.
- To add or change a portrait, see the instructions at the top of `tools/make-avatars.py`. That optional script requires Python's Pillow package. Group gallery images are described in `assets/img/group/README.md`.

After editing, check the affected pages in both languages and at a narrow browser width. The site can be published from the repository root with GitHub Pages (`main` branch, `/(root)` folder).
