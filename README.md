# Cannoli watch page

The page branded shortlinks from **Cannoli Screen Recorder** land on. One static file, no backend:
the Vimeo player with captions on from the first frame, the AI summary and clickable chapters next to it.

- `index.html` — the page. Source of truth is `web/watch.html` in the (private) app repo; copy it here on change.
- Served by GitHub Pages at `https://dzisner.github.io/cannoli-live-videos/`.
- The app appends `?v=<vimeo id>&h=<unlisted hash>`; optional `cc=<lang>` prefers a caption language.

Everything shown is read live from Vimeo (oEmbed for title + description, player API for chapters and
text tracks), so editing a transcript or regenerating a summary in the app updates the page with no deploy.
