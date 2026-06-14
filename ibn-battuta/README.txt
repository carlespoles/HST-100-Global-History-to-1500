IBN BATTUTA STORYMAP (self-contained) — deploy to GitHub Pages
==============================================================
WHAT CHANGED: the StoryMapJS library is now bundled INSIDE this folder
(assets/storymapjs/). It no longer depends on Knight Lab's CDN, which was
failing to load (the "SM is not a constructor" error). Nothing external is
required except the OpenStreetMap map tiles, which load in the browser.

DEPLOY
1. Copy this whole "ibn-battuta" folder into your repo:
      carlespoles.github.io/ibn-battuta/index.html
      carlespoles.github.io/ibn-battuta/assets/...
      carlespoles.github.io/ibn-battuta/images/...
2. Commit and push.
3. Live URL to submit:
      https://carlespoles.github.io/ibn-battuta/

PREVIEW LOCALLY FIRST (recommended)
   cd into this folder, then:   python3 -m http.server
   open:  http://localhost:8000/
   (It must be served over http/https — opening index.html directly from
    the file system will not load the map.)

NOTES
- Basemap is OpenStreetMap (no API key). To change it, edit "map_type" in
  index.html.
- All 8 slides (title, six stops, conclusion) are embedded directly in
  index.html — no Google sign-in, no external data file.
