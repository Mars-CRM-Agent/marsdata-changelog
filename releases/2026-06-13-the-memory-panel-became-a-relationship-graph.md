# The memory panel became a relationship graph.

> Canonical source of record: [https://marsdata.ai/changelog](https://marsdata.ai/changelog)
> Release `0.1.1.1959` · 2026-06-13

- **New** — The memory panel now shows a relationship graph — the people and topics Mars remembers about you arranged around a central hub, with each one sized by how much detail it holds, and you can click any person to open their full profile. Mars is also more careful about what it keeps: it won't file away traits that actually belong to someone else, and when you delete a person or a memory folder they now stay deleted instead of quietly regrowing from past chat logs.
- **New** — Select any text in a reply and a small toolbar now appears — you can quote it straight into your next message, or have it read aloud. The labels follow your chosen language.
- **Improved** — Opening your conversation history and switching between chats is noticeably faster — the list now paints progressively, and a chat you recently opened shows its content almost instantly. It's also more resilient: a brief hiccup right after you open the app no longer freezes the "scroll down to load more" behavior or makes conversations inside folders disappear — the list now recovers on its own as you keep scrolling.
- **Improved** — The app's first screen loads faster and more cleanly — visitors now see the real home page right away instead of a brief grey skeleton flash, and signed-in users no longer momentarily glimpse the logged-out intro page before their workspace appears.
- **Improved** — Uploading large or long videos now works reliably — the previous length limit is gone, videos no longer have to be re-compressed in your browser before sending, and an upload placeholder appears right away so you can see it's in progress. A case on iPhone where a video upload could get stuck and never finish is also fixed.
- **Improved** — Long, complex tasks end more gracefully — when Mars reaches an internal safety limit it now hands you a real, usable answer instead of a generic "stopped" message, and it no longer mistakes a completed action (such as saving your data) for a failed one.
- **Improved** — Strengthened how your account and data are protected — closed several issues where information could potentially be reached across separate accounts, hardened the app against malicious content hidden in pages Mars reads for you, and tightened the safeguards around your data sandbox.
- **Improved** — Pop-up confirmations, alerts, and the "usage limit reached" notice now appear in your chosen language instead of defaulting to one language.
- **Improved** — On iPhone and iPad, launching Mars from the Home Screen now opens straight into a dark splash that matches the app, instead of a brief white flash.
- **Fixed** — The stop button now reliably stops a reply that's still being generated, and starting to type a new message while Mars is producing its very first answer no longer accidentally creates a duplicate conversation.
- **Fixed** — Generating images is smoother — the placeholder no longer flickers while an image is being created, and when Mars produces several images they now show together in a gallery.
- **Fixed** — Math formulas written inside table cells now render properly instead of showing up as raw code.
- **Fixed** — Times shown for Douyin live-stream data are now correct — they were previously off by eight hours.
- **Fixed** — Signing in with Apple using a hidden (relay) email address no longer occasionally merges two separate accounts into one.
- **Fixed** — The storage panel is steadier and more informative — it no longer jitters on high-DPI Windows displays, and it now lists the built-in data tables alongside how many rows you have in each.

---

[Back to all releases](../README.md) · [Try Marsdata AI](https://marsdata.ai) · [简体中文](./2026-06-13-the-memory-panel-became-a-relationship-graph.zh-CN.md) · [繁體中文](./2026-06-13-the-memory-panel-became-a-relationship-graph.zh-HK.md)
