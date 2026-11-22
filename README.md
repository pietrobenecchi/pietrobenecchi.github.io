# pietrobenecchi.github.io

Personal portfolio site of Pietro Benecchi, served by GitHub Pages at
<https://pietrobenecchi.github.io/>.

It is a plain static site with no build step and no JavaScript (the only external resource is Google Fonts: Montserrat + Roboto):

- `index.html`: the whole single-page site
- `assets/style.css`: styles (light academic layout, blue accent)
- `assets/favicon.svg`: "PB" favicon
- `.nojekyll`: tells GitHub Pages to serve the files as they are, without Jekyll

## View locally

```sh
python3 -m http.server 8000
# then open http://localhost:8000
```

## TODO

- [ ] **Add the CV**: put the PDF at `assets/cv.pdf`. The "CV" button in the hero already links there and returns 404 until the file exists.
- [ ] **Add the email** in the Contact section of `index.html` (see the `TODO` comment there).
- [ ] **Publications**: add the title and link of the SEAMS paper (Distinguished Paper Award) and of the poster at the 3rd FPGA Developers' Forum, CERN (see the `TODO` comments in `index.html`).
- [ ] **Add a photo**: save it as `assets/avatar.jpg` and replace the "PB" initials circle in the About section (see the `TODO` comment in `index.html`).
- [ ] Optional: add an `og:image` (PNG, 1200×630) for nicer link previews.
