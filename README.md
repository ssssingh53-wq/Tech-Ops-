# EM – Issue Tracker & SLA Report v2.2

A browser-based, view-only viewer for the SLA report deck (10 slides, rendered from
`EM - Issue Tracker & SLA Report v2.2.pptx`). Open `index.html` to view; navigate with
the arrow keys, thumbnails, or the on-screen arrows. Press **F** for fullscreen.

The viewer has **no download button**, and right-click, image-drag, and text selection
are disabled, so there is no obvious way to save the slides.

## Files
- `index.html` — the slide viewer
- `slides/slide-01.png … slide-10.png` — the rendered slides
- `.nojekyll` — tells GitHub Pages to serve the files as-is

## Publishing on GitHub Pages (gives you a URL to share)
1. Push this folder to a GitHub repo (see below).
2. Repo → **Settings → Pages**.
3. Under **Build and deployment**, set **Source = Deploy from a branch**,
   **Branch = main**, **Folder = / (root)**, then **Save**.
4. After a minute your URL is: `https://<your-username>.github.io/<repo-name>/`

## Pushing this folder to GitHub
```bash
cd em-sla-report-v2.2
git init
git add .
git commit -m "Add EM Issue Tracker & SLA Report v2.2 viewer"
git branch -M main
git remote add origin https://github.com/<your-username>/<repo-name>.git
git push -u origin main
```

## Important — about access control
GitHub cannot give a *link-only, no-account, no-download* page on a standard account:

- **GitHub Pages is public.** Anyone with the URL can open it. "Only people I give the
  URL to" works only as *obscurity* (the URL is hard to guess), not as enforced access.
  Member-only Pages require **GitHub Enterprise Cloud**.
- **A private repo** restricts viewing to GitHub users you invite as collaborators — but
  that is not a plain URL, and repo files are downloadable by those collaborators.
- **No web page can fully prevent copying** (screenshots always work). This viewer removes
  the easy ways (download button, right-click, drag), which stops casual saving.

If enforced "only specific people, no download" is the real goal, **Google Drive**
("anyone with the link – Viewer" + *disable download/print/copy*) matches it far better
than GitHub.
