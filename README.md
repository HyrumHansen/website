# Personal Portfolio Site

A small, dependency-free static website. Three pages, one stylesheet, no build
tools, no frameworks — just HTML and CSS. If you can edit a text file, you can
maintain this site.

## What's in here

```
index.html         → About page (home)
publications.html  → Publications, each with your commentary
personal.html      → Personal page
style.css          → All styling (colors, fonts, spacing)
README.md          → This file
```

The only external dependency is Google Fonts (Newsreader and IBM Plex Mono),
loaded automatically by the visitor's browser. Nothing to install.

## Editing the content

Open any `.html` file in a text editor. Everywhere you need to change something
there's a comment that starts with `<!-- EDIT: ... -->`. Search for the word
`EDIT` and work through them:

- Your name (it appears in the header, hero, and footer of each page)
- The intro and background paragraphs on `index.html`
- Universities and years in the Education section
- Your real email / Scholar / GitHub / LinkedIn links
- Publications: copy-paste one `<article class="pub">` block per paper and
  fill in venue, year, title, commentary, and links
- The Personal page: write freely; add a `photo.jpg` next to the HTML files
  or delete the `<figure>` block

To preview locally, just double-click `index.html` — it opens in your browser.
No server needed.

## Changing the look

All colors live at the top of `style.css` as variables (`--paper`, `--ink`,
`--gold`, etc.). Change a hex code there and it updates everywhere.

## Hosting on GitHub Pages (free, ~5 minutes)

1. **Create a GitHub account** at github.com if you don't have one.

2. **Create a new repository.** Click the “+” in the top right → *New
   repository*. Name it exactly:

   ```
   yourusername.github.io
   ```

   (replace `yourusername` with your actual GitHub username — this special
   name is what makes it a website). Keep it Public. Click *Create repository*.

3. **Upload the files.** On the new repository page, click *uploading an
   existing file*, drag in `index.html`, `publications.html`,
   `personal.html`, `style.css`, and this `README.md` (plus `photo.jpg` if
   you added one), then click *Commit changes*. No command line required.

4. **Wait a minute or two**, then visit:

   ```
   https://yourusername.github.io
   ```

   That's it. The site is live and hosting is free.

### Updating the site later

Edit a file on your computer, then on GitHub click *Add file → Upload files*
and upload it again — the new version replaces the old one. (Or edit directly
in the browser: open the file on GitHub, click the pencil icon, make your
change, and commit.) The live site updates within a minute or so.

### Optional: a custom domain

If you later buy a domain (e.g. `yourname.com`), GitHub Pages supports it:
repository *Settings → Pages → Custom domain*. Not required — the
`.github.io` address works fine on its own.

## Why this setup

- **GitHub Pages** is free, has no servers to manage, and doubles as the
  place your code lives — which covers your "store it on GitHub" preference
  and your "don't want to do much work" preference at the same time.
- **No build step** means nothing can break. There are no dependencies to
  update, ever.
