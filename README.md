# Lunceford Holdings

A one-page static site for Lunceford Holdings. No build step, no dependencies —
a single `index.html` you can drop on any host.

## Editing the portfolio

Everything you'll want to change lives in `index.html`:

- **Ventures** — the `<ul class="ventures">` block, marked with an `EDIT HERE`
  comment. One `<li class="venture">` per business. If a venture has no website
  of its own, delete the `<a>` wrapper and leave the plain name.
- **Contact address** — the `mailto:` link in the `<footer>`.
- **Intro line** — the `<p class="lede">` under the wordmark.

## Local preview

Open `index.html` in a browser, or:

```
python3 -m http.server 8000
```

then visit http://localhost:8000.

## Deploying

Any static host works. A few that need no configuration beyond pointing at this
repo:

- **GitHub Pages** — repo Settings → Pages → deploy from branch, root folder.
- **Netlify / Cloudflare Pages** — connect the repo, leave the build command
  blank, set the publish directory to `/`.

Point the domain at the host, and set the email address up separately through
your registrar or mail provider — the site doesn't need to know about it.

## Notes

- Light and dark themes follow the visitor's system setting.
- Responsive down to small phones; no JavaScript required beyond the copyright
  year.
