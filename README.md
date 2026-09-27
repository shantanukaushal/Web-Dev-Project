# Shantanu Kaushal — Portfolio

A single-page personal portfolio, built with plain HTML and CSS. No
frameworks, no build step, no JavaScript beyond what the browser does
natively for `prefers-reduced-motion` and anchor scrolling.

## About

I'm a BSc Computer Science student at BITS Pilani, also doing the UGP
in AI & Business at Scaler School of Technology. This site is where
that shows up online — a short bio, what I actually work with, and a
way to get in touch.

## Stack

- **HTML5** — semantic markup, no div soup
- **CSS3** — Grid + Flexbox for layout, custom properties for the
  color/type tokens, one CSS animation on page load
- **Fonts** — [Fraunces](https://fonts.google.com/specimen/Fraunces),
  [IBM Plex Sans](https://fonts.google.com/specimen/IBM+Plex+Sans), and
  [IBM Plex Mono](https://fonts.google.com/specimen/IBM+Plex+Mono),
  loaded from Google Fonts

No CSS framework, no bundler, no npm install required.

## Running it locally

Clone the repo and open `index.html` directly in a browser, or serve
it with any static server if you'd rather not deal with `file://`
paths (e.g. VS Code's **Live Server** extension, or):

```bash
python3 -m http.server 8000
```

then visit `http://localhost:8000`.

## Project structure

```
.
├── index.html            # all page content and markup
├── style.css              # design tokens, layout, and component styles
├── portrait-shantanu.png  # profile photo used in the hero section
└── README.md
```

## Notes for future edits

- Color, type, and spacing tokens all live at the top of `style.css`
  under `:root` — change a value there rather than hunting for it
  inline further down the file.
- The offset gold block behind the portrait is a `::before` on
  `.portrait-photo`, kept deliberately separate from the caption
  below it so resizing one never bleeds into the other.
- Motion is intentionally limited to one entrance animation on the
  name in the hero; it's skipped entirely for anyone with
  `prefers-reduced-motion` set.

## Contact

- Email: [shantanu.26bcs10499@sst.scaler.com](mailto:shantanu.26bcs10499@sst.scaler.com)
- LinkedIn: [linkedin.com/in/shantanu-kaushal](https://www.linkedin.com/in/shantanu-kaushal/)
- GitHub: [github.com/shantanukaushal](https://github.com/shantanukaushal)
