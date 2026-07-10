# Rich Push Format Playbook

An interactive gallery of CleverTap rich push notification formats, built for enterprise CS conversations across APAC. Browse by vertical, format or platform, preview each one live on a phone mockup, read the thinking behind it, and copy a ready-to-run config.

**Live:** https://shijunneo-bot.github.io/rich-push-gallery/

> Replace the URL above with your actual repo name after deploying.

---

## What's inside

- **182 prototypes** — 168 brand campaign examples (12 verticals × 14 formats) plus a 14-card Format Library.
- **14 real CleverTap push formats** — Standard, Advanced, Single Image, Content Slider, Auto Carousel, Manual Carousel, Timer, Text over Image, Five Icons, Rating, Product Catalog, Input Box, Vertical Image + CTA, and GIF. Each carries doc-verified requirements, platform support and the events it fires.
- **12 APAC verticals** — e-commerce, food & beverage, on-demand, travel, fintech, banking, insurance, education, OTT, telco, social and gaming. Every cell is filled, so there is no empty vertical × format combination.
- **Live interactions** — tap a card and it opens on a lock screen. Timers count down, carousels advance, stars pop, catalog rows highlight, and a transient pill names the exact CleverTap event captured.
- **Six award cases** — isolate them with the trophy filter. Each carries a Case notes panel: the brief, the mechanics, and why it won, fact-checked against the public record.
- **Config recipe in every campaign card** — open the Config tab for a field-by-field dashboard walkthrough and a copy-paste `/1/targets/create.json` API payload, with a toggle between the real example values and a blank template.

---

## How to use it in a client conversation

1. **Filter to the moment.** Pick the client's vertical, a format you're proposing, or a platform if their app is Android or iOS only.
2. **Tap a card.** It opens live. Replay runs the interaction again.
3. **Tap inside the mock.** Buttons, stars, carousels and catalog rows respond, and the pill names the event fired.
4. **Open Config.** The dashboard recipe shows exactly which field takes which value; the API tab gives the raw payload for the client's dev team.

---

## Deploying

This is a single self-contained `index.html`. Every photo is embedded as base64, so there is no asset folder, no zip, and no build step.

1. Put `index.html` at the **root** of a public repo.
2. Go to **Settings → Pages**.
3. Set **Source** to **Deploy from a branch**, branch `main`, folder `/ (root)`, and Save.
4. Wait about a minute. The live URL appears in the Pages settings.

To update, replace the same `index.html` and push again. The URL stays the same. Hard-refresh (Cmd+Shift+R) if a change doesn't show, since GitHub caches.

---

## Swapping in client imagery

The gallery ships with stock photography baked in. To show a client their own creative, replace the relevant base64 value in the `SCENE_IMG` map inside the file with a base64 data URI of the client image. Keep the same key so every reference updates at once.

---

## Notes

- Fonts (DM Sans, DM Serif Display, DM Mono) and the browser tab icon load from external CDNs at view time. On a live URL this is seamless. Opened offline, fonts fall back to system defaults and the tab icon is blank; everything else, including all embedded photos, still renders.
- Format facts, template keys and API payload shapes are verified against the CleverTap developer documentation. Award claims are checked against public sources; unverifiable claims are labelled honestly rather than asserted.

---

Built by SJ Neo · CleverTap APAC CS
