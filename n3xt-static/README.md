# n3xt — static export

A self-contained static version of the n3xt site. The ENTIRE site (all pages + all data) is inside the single index.html file. No backend, no build step, no other files needed.

## Deploy on GitHub Pages (3 steps)
1. Create a new GitHub repository.
2. Unzip this archive and upload index.html (and .nojekyll) to the repo ROOT — the very top level, NOT inside any folder.
3. In the repo: Settings -> Pages -> Source: Deploy from a branch -> branch: main -> folder: / (root) -> Save. Wait ~1 minute, open the URL. Done.

## Troubleshooting
- White/blank page: index.html is NOT at the repo root (it must be at the top level), or Pages source is not set to / (root).
- "loading n3xt…" stuck on screen: a JavaScript error occurred — the error text will be shown on screen.
- Games do not open: game files stream from truffled.lol and need an internet connection.

## Notes
- Everything (games, movies, tools, apps, updates, covers) is baked into index.html. There are no separate data files to upload.
- Games and tools load inside iframes from truffled.lol; movies load from Google Drive previews. An internet connection is required for those.
- .nojekyll tells GitHub Pages to serve files as-is.
