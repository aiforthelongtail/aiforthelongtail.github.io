# aiforthelongtail.github.io

Website for **AI for the Long-Tail (ALT): What Generalizes, What Works, and When
to Use It**, a workshop proposed to ICLR 2027. Content follows the proposal
`main_1007v1.tex`.

Plain HTML and CSS, with no build step. GitHub Pages serves the `main` branch as is.

```
index.html              all page content
assets/css/style.css    styles (colors are CSS variables at the top; dark mode included)
assets/img/people/      480x480 headshots, named <first>-<last>.jpg
assets/img/og.png       social preview image (1200x630)
assets/img/favicon.svg
```

## Edit

- **Text, dates, people:** edit `index.html` directly. Each person is one `<li>`
  in the speakers or organizers list.
- **New photo:** a square JPEG of about 480x480 in `assets/img/people/`.
- **Hero plot labels:** the examples along the tail are the `<text>` elements
  inside `<svg class="tail">` in `index.html`.
- **After acceptance:** update the hero line ("A proposed workshop at ICLR 2027 …"),
  the call-for-papers status line, the footer, and the `<title>`.

## Preview locally

```sh
python3 -m http.server 8000
# open http://localhost:8000
```

## Deploy

The repository must be named `aiforthelongtail.github.io` under the
`aiforthelongtail` GitHub account. Push to `main`, and the site appears at
https://aiforthelongtail.github.io/ within a minute or two. If it doesn't, check
Settings → Pages: source "Deploy from a branch", branch `main`, folder `/`.
