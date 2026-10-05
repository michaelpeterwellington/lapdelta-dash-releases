# LapDelta Dash firmware releases

Signed firmware for the LapDelta Dash. Dashes check `manifest.json` here for updates
over Wi-Fi and install the image it names; the images are signed, so a dash only
accepts builds from the maker. The source lives in a private repository; this one
holds only what a dash or a laptop needs:

- `manifest.json`: the current version, download URL, SHA-256 and release notes.
- `flasher.json` + `index.html`: a browser USB flasher (Chrome or Edge) for a dash that
  will not start. Open https://michaelpeterwellington.github.io/lapdelta-dash-releases/
- `firmware/`: merged images for the USB flasher.
- Releases: the signed application image per version.

Normal updates need no file handling: switch on Wi-Fi export on the dash, open its page,
and press Install under Firmware. Or copy a release `.bin` to the SD card as `UPDATE.BIN`.
