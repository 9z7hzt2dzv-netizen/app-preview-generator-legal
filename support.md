# Support

**AppreviewGen**

## Contact

**[Open an issue](https://github.com/9z7hzt2dzv-netizen/app-preview-generator-legal/issues)**

There is no support mailbox. Everything goes through the tracker, so every report has a
number, a thread, and an answer the next reader finds instead of writing the same message
again. Search the open and closed issues first — the thing may already have one.

The **Report a bug** row on the About screen opens the form with your version and platform
already filled in.

Write in English. A reply usually comes within a few days.

Useful things to include, when you have them:

- what you were doing when it happened, and in which editor
- your device and OS version (Settings › General › About, or Apple menu › About This Mac)
- the app version, from the About screen — the button in the top right of the project gallery
- a screenshot, if it is something you can see

## Common questions

**Does the app need the internet?**
No. It has no network code in it. Everything is rendered and encoded on your device, and it
works exactly the same in aeroplane mode.

**Where are my projects stored?**
In the app's own folder, under Application Support, one folder per project holding a
`project.json` and the media you imported. They are not in iCloud and not on any server.
Deleting the app deletes them, so export anything you want to keep.

**Apple rejected my screenshots. What now?**
Check the pre-flight report before exporting — it lists dimensions, transparency and frame
count as pass, warn or block. If the report was clean and the upload was still refused, send
the rejection text. A rule that changed is worth knowing about and gets fixed.

**Why does my preview warn when it has a device frame on it?**
Guideline 2.3.4 rejects app previews that show a device frame. The app warns rather than
silently removing the frame, because removing it would change a composition you approved.
Turn the frame off for the video, or accept the risk knowingly.

**Why is the video export size different from the screenshot size?**
Because Apple's accepted app preview sizes are not the screenshot sizes — 886 × 1920 for
iPhone and 1200 × 1600 for iPad. The app targets the preview sizes for video and the display
class sizes for stills, which is the whole point of it.

**The exported PNG looks right but the upload says it has transparency.**
It should not: exports strip the alpha channel, because Apple prohibits it. If you see this,
send the file — that is a bug, not a setting.

**My export folder stopped working after I restarted the Mac.**
Pick it again. The app stores the permission the system gave it, and a folder that moved or
a volume that unmounted invalidates it.

**How do I get a refund?**
Refunds are handled by Apple, not by the developer: <https://reportaproblem.apple.com>

## Reporting a bug

Say what you did, what you expected, and what happened instead. If it involves an export,
the export target and the display class matter. Every report gets read.

## Legal

- [Privacy Policy](privacy-policy.md)
- [Terms of Use](terms-of-service.md)
- [Licence](license.md)

© 2026 Egzon Pllana
