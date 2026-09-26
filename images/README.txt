This folder feeds the Gallery section on the site automatically.

To add a photo: just drop the image file in here (jpg/jpeg/png/webp/gif)
and push to GitHub. The deploy workflow (.github/workflows/deploy-pages.yml)
scans this folder on every push, regenerates images/manifest.json with
whatever files it finds, and the site reads that file at load time.

No HTML/JS edits needed — ever. Delete a photo from this folder and it
disappears from the gallery on the next push too.

Captions: the site titles each photo by turning the filename into a
title, e.g. "cypher-2026-keynote.jpg" becomes "Cypher 2026 Keynote".
Name your files accordingly, using dashes or underscores between words.

Order: images appear in alphabetical filename order. Prefix filenames
with numbers (01-, 02-, ...) if you want to control the order shown.
