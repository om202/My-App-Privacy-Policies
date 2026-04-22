# True Full Screen for Safari — Support

Thanks for installing! Everything you need to use, troubleshoot, and get help with the extension is below.

## Getting started

1. Install **True Full Screen for Safari** from the Mac App Store.
2. Open Safari.
3. Go to **Safari → Settings → Extensions** (or press `⌘,` then click *Extensions*).
4. Check the box next to **True Full Screen** to enable it.
5. Open any Netflix or YouTube video (e.g. `netflix.com/watch/…` or `youtube.com/watch?v=…`).
6. Click the **True Full Screen** icon in Safari's toolbar.
7. Drag the zoom slider or tap a preset. That's it.

Your zoom level is saved automatically and per-site (your Netflix zoom and YouTube zoom are independent).

## Usage tips

- **Slider:** fine-grained zoom between 100% and 200%.
- **Presets:** 10 buttons from Off (100%) to 200%, tap any for instant zoom.
- **Off:** the red "Off" button resets to 100% and disables the effect.
- **Per-site memory:** your preferred level is remembered separately for Netflix and YouTube.
- **Theater / fullscreen:** zoom persists across default view, theater mode, and native fullscreen.
- **Advanced → Strategy:** if the default zoom isn't matching your site's layout, switch to the *Smart ancestor* fallback strategy — useful for YouTube Shorts, embeds, or layout experiments.

## Troubleshooting

### "Start a video" message, controls greyed out
You're not on a supported video page. The extension only activates on:
- Netflix: URLs matching `/watch/…`
- YouTube: URLs matching `/watch`, `/shorts/`, `/embed/`

Open a video and the controls re-enable automatically.

### Zoom has no visible effect
1. Make sure the video is actually playing (controls won't act on a loading / paused frame with no dimensions).
2. Open the popup → expand **Advanced → Diagnostics**. Check:
   - **Video:** should be "yes"
   - **Dimensions:** should show real numbers like `1920 × 1080`
   - **scale-target:** should show a DOM element, not "NONE"
3. If *scale-target* is NONE, try switching strategy to **Smart ancestor (fallback)** in Advanced.
4. If it still does nothing, YouTube or Netflix may have shipped a layout change — please email me and I'll ship a fix.

### Page looks weird after I left a video
If you scroll / navigate and parts of the page seem clipped, refresh the tab. The extension auto-cleans when you navigate away, but single-page reloads sometimes lag a frame.

### Extension disappeared from Safari's toolbar
Right-click the toolbar → **Customize Toolbar…** → drag the True Full Screen icon back.

### Extension isn't active even after enabling
Quit Safari completely (`⌘Q`) and reopen. Safari occasionally needs a restart to register new web extensions.

## FAQ

**Does this work on Prime Video / Disney+ / Hulu / HBO?**
Not yet. The extension currently supports Netflix and YouTube. More sites may be added in future updates based on demand — email me your vote.

**Does it work on iPhone or iPad Safari?**
Not currently. The release is macOS-only. An iOS build may come later.

**Why can't I zoom below 100%?**
The extension is designed for filling the screen, not shrinking it. If you want to zoom out, use Safari's built-in zoom (`⌘–`).

**Does it support ultrawide monitors (21:9, 32:9)?**
Yes — that's exactly what it's for. Use 150%–200% on a 21:9 to remove letterbox bars from a 16:9 video.

**Does it slow down my videos or affect quality?**
No. The extension uses a pure CSS transform on the video element. There's no re-encoding, no JavaScript running per-frame, and no impact on playback performance.

**Does the extension collect any data?**
No. See the [Privacy Policy](PRIVACY.md) for details. No tracking, no analytics, no network requests.

## Request a feature or report a bug

I read every email personally. Please include:

- **macOS version** (Apple menu → About This Mac)
- **Safari version**
- **Which site** (Netflix / YouTube / both)
- **What you expected vs. what happened**
- A **screenshot** if possible

## Contact

**Omprakash Sah Kanu** — exonary.build@gmail.com

Reply usually within 24–48 hours.

---

© 2026 Omprakash Sah Kanu
