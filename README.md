# pietrobenecchi.github.io

Personal portfolio site of Pietro Benecchi, served by GitHub Pages at
<https://pietrobenecchi.github.io/>.

It is a plain static site with no build step and no JavaScript (the only external resource is Google Fonts: Montserrat + Roboto):

- `index.html`: Home: biography, interests, education summary and contact
- `cv.html`: CV & Experience: experience, education, projects, publications, skills, CV download
- `blog.html`: Blog: list of posts
- `blog/_template.html`: template for a new blog post
- `assets/style.css`: styles (light academic layout, blue accent)
- `assets/favicon.svg`: "PB" favicon
- `.nojekyll`: tells GitHub Pages to serve the files as they are, without Jekyll

## View locally

```sh
python3 -m http.server 8000
# then open http://localhost:8000
```

## Writing a blog post

1. Copy `blog/_template.html` to `blog/<slug>.html`, then edit the title, date, description and body.
2. In `blog.html`, add an entry at the top of the `<ul class="posts">` list (an example is in the HTML comment just above it). The "No posts yet" message disappears automatically once the list has an entry.
3. Commit and push.

The navbar, `<head>` and icon sprite are repeated in each page (there is no build step), so a change to the navbar must be made in every HTML file.

## TODO

- [ ] **Add the CV**: put the PDF at `assets/cv.pdf`. The links on Home and CV already point there and returns 404 until the file exists.
- [ ] **Add the email** in the Contact section of `index.html` (see the `TODO` comment there).
- [ ] **Publications**: add the title and link of the SEAMS paper (Distinguished Paper Award) and of the poster at the 3rd FPGA Developers' Forum, CERN (see the `TODO` comments in `cv.html`).
- [ ] **Add a photo**: save it as `assets/avatar.jpg` and replace the "PB" initials circle in the About section (see the `TODO` comment in `index.html`).
- [ ] Optional: add an `og:image` (PNG, 1200×630) for nicer link previews.
