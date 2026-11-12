# thergopinath.github.io

Personal website of Rohith Gopinath, served by GitHub Pages at <https://thergopinath.github.io>.

Plain HTML and CSS: no build step and no Jekyll (`.nojekyll` is set). Edit a file, commit, and the site updates within a minute or two.

## Layout

| Path | What it is |
|---|---|
| `index.html` | Landing page with two floating cards, Academic and Personal (keyboard: `A` / `P`) |
| `academic/index.html` | Research, other projects, code, talks, education, honours |
| `cv/index.html` | Web CV (prints cleanly to A4) |
| `cv/Rohith_Gopinath_CV.pdf` | CV PDF linked from the site; replace it with your own PDF under the same name |
| `personal/index.html` | Now, writing, kitchen (recipes), bookshelf, ClosedSpace |
| `personal/writing/_template.html` | Copy this to start a new essay |
| `personal/recipes/_template.html` | Copy this to start a new recipe |
| `assets/site.css` | Shared styles (green theme = academic, rust theme = personal) |
| `404.html` | Not-found page |

## Adding things

- **Essay:** copy `personal/writing/_template.html` to `personal/writing/<name>.html` and fill it in. Then copy the commented card template in the Writing section of `personal/index.html` and point it at the new file.
- **Recipe:** same steps, using `personal/recipes/_template.html` and the Kitchen section.
- **Book:** copy the commented `<li>` template in the Bookshelf section into the `<ul class="books">` list.
- **Code repo:** copy the commented card template in the Code section of `academic/index.html`.

Each section shows an "empty" box until its first item is added. Delete that box when you add one.

## Regenerating the CV PDF

```bash
google-chrome --headless --no-pdf-header-footer --print-to-pdf=cv/Rohith_Gopinath_CV.pdf cv/index.html
```
