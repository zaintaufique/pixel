# pixel.pk — TV Backlight Finder

A single-page site that matches TV brands/models to their backlight LED strip and
lets customers order the part on WhatsApp.

## Files

    index.html        The whole website (structure, styles, and data in one file)
    photos/           Backlight photos, named by serial (see photos/README.md)
    LICENSE           All rights reserved

## Add a new TV + backlight

1. Open `index.html` and find the `DATA` list near the bottom.
2. Copy an existing line and fill in the values:

       { brand:"Samsung", model:"UA40J5200", size:40, serial:"SVS400A79",
         lights:8, vpl:3, total:24, strips:1, type:"LED Strip", img:null },

   - Use `null` for any spec you don't have yet (it shows as "—").
   - Leave `img:null` — photos are linked automatically from the serial.
3. Commit. The new card appears, and its photo slot shows the filename to add.

## Add the photo

Save the picture in `photos/` using the name shown on the card
(serial in lowercase, non-letters/numbers become `-`, `.jpg`). Commit. Done.
See `photos/README.md` for examples.

## Publish (GitHub Pages)

Settings → Pages → Deploy from a branch → `main` / root → Save.
Your site goes live at `https://<username>.github.io/<repo>/`, and you can point
the `pixel.pk` domain at it under the same Pages settings.
