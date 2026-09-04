# AppreviewGen

**App Store screenshots and app preview videos, made on the device you already own.**

Drop in the raw screenshots and screen recordings you already have. AppreviewGen lays
them out, frames them, styles them, and exports at the exact pixel sizes App Store
Connect accepts — including the app preview video, which almost nothing else gets right.

Native on iPhone, iPad and Mac. No account, no internet connection, no advertising, no
in-app purchases, no subscription. It works in aeroplane mode, because it has no network
code in it at all.

---

## What is inside

**A project library**
- Every project is a folder on disk. Searchable, sortable, and open where you left off.
- Drag screenshots onto the gallery to start a project from them.

**A screenshot editor**
- A live canvas laid out in design points, with draggable, selectable layers and undo.
- Copy, captures, tint, device dressing and attachments, per frame.

**Template groups**
- Classic groups — Studio Mono, Midnight, Aurora, Bold Type and others — that mix their
  ground from colour.
- Futurist groups — Holo Foil, Vector Horizon, Cathode, Topograph, Orbital and others —
  that *draw* their ground: scanlines, contours, a perspective grid running to a horizon,
  board routing, a dot lattice, a star field, signal traces, drafting rules.
- Switching group re-lays every frame. Your copy and your captures survive it.

**Device framing**
- Bezels, colourways, sensor housings, home indicator, status bar and screen glare, all
  drawn rather than shipped as bitmaps, so they stay sharp at any export size.

**A video editor**
- A zoomable timeline: trim, split at the playhead, reorder, replace, delete.
- Text cues placed on the stage, a poster frame you choose, and a duration meter measured
  against Apple's 15–30 second window.

**Export that Apple accepts**
- Screenshots at exact pixel dimensions per display class, in sRGB, **with the alpha
  channel stripped** — Apple prohibits it — into `deliver`-shaped folders.
- App previews written through `AVAssetReader` and `AVAssetWriter` rather than
  `AVAssetExportSession`, because only that route can pin the bitrate and the H.264
  profile level Apple's specification is explicit about.

**A pre-flight report**
- Every rule listed as pass, warn or block before you upload: frame count, duration,
  dimensions, transparency, codec, poster frame, placeholder copy left unedited, text
  legibility, and device frames in a preview, which Guideline 2.3.4 rejects.

---

## How it works

- **One model, three consumers.** The interactive canvas, the still export and the video
  export are the same view at three rasterisation scales. The editor and the export cannot
  drift, because they are not two pieces of code.
- **The canvas is a fixed size, not your screen.** Most tools derive the export canvas from
  whatever device they happen to be running on, so a correct screenshot is a coincidence.
  Here it is a design-point size per export target.
- **Everything stays on your device.** Your screenshots and recordings are copied into the
  project folder in the app's own sandbox and go nowhere else.

## Requirements

iOS 26 or later, or macOS 26 or later. iPhone, iPad and Mac. The Mac app is a native
build, not Catalyst.

## Support

Questions and bug reports: **9z7hzt2dzv@privaterelay.appleid.com**

See [Support](support.md) for what to include.

## Legal

- [Privacy Policy](privacy-policy.md) — the app collects nothing
- [Terms of Use](terms-of-service.md)
- [Licence](license.md)

---

© 2026 Egzon Pllana. This repository holds the published documents for AppreviewGen. The
app's source code is not part of it.
