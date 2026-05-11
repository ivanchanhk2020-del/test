## Cursor Cloud specific instructions

This is a **static HTML/CSS/JS website** with no build system, no package manager, no tests, and no linting tools. There are no dependencies to install.

### Running the site

Serve the workspace directory with any static HTTP server. The simplest option:

```
python3 -m http.server 8000 --directory /workspace
```

Then open `http://localhost:8000/home.html` in a browser. The site has four pages reachable from the nav bar: Home (`home.html`), Our Team (`team.html`), Research (`research.html`), and Services (`services.html`).

### Notes

- Some images and the embedded YouTube video load from external URLs (`obsgyn.med.hku.hk`, `images.unsplash.com`, `youtube.com`). Pages still render without internet, but those assets will be broken.
- `testing.html` is a design-testing variant of the home page layout.
- `*_profile_raw.html` files are scraped reference pages, not part of the live site.
- `tmp_staff_scrape.py` is a one-off Python utility; it is not part of the site.
- There are no automated tests, linting, or build steps configured in this repository.
