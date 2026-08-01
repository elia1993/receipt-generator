# מחולל קבלות PDF

A small static page (`index.html`) that lets you pick receipt images from a
library and download them combined into a single PDF.

## Receipts library

The library shown on the page comes from a hardcoded list of filenames
inside `index.html` (the `LIBRARY_FILES` array near the top of the
`<script>` block). This is intentional so the page works by simply opening
`index.html` directly (`file://...`) — no server, no `fetch()`, no build
step.

### Adding or removing a receipt image

1. Add or delete the image file(s) in `receipts/`.
2. Update the `LIBRARY_FILES` array in `index.html` to match.
3. Commit and push.
