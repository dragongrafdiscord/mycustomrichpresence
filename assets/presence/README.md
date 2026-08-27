# Presence artwork

The overhaul keeps each preset's existing direct image URL when one was already available.

The local `assets/previews/` folder is the self-contained preview catalog. Presence artwork can be mirrored into this folder later without changing the preset roster or metadata structure. Historical Discord attachment URLs are retained in `presets.json` when available, but many signed Discord CDN links from old exports expire.
