# Everyone you mention now gets their own dossier.

> Canonical source of record: [https://marsdata.ai/changelog](https://marsdata.ai/changelog)
> Release `0.1.1.2173` · 2026-07-06

- **New** — Mars now automatically builds a structured record for each person you talk about — identity, background, how you know each other, key interactions, and an overall value read are extracted from your conversations into a dedicated database record and summarized on the person's page. Details you've already told Mars no longer get silently overwritten when new information arrives, and when two records turn out to be the same person, merging them now keeps everything from both sides.
- **New** — When you chat about someone Mars already knows, the conversation is now automatically filed into that person's folder — so everything about one person stays in one place without manual sorting.
- **Improved** — The person detail page got a cleaner desktop layout — interaction log, profile, and key facts now sit side by side in three equal columns instead of one long scroll, duplicated profile text is gone, and the memory panel now shows titles and writes new memories in your chosen language.
- **Improved** — Opening a conversation is more dependable — cases where a chat could stay stuck on the loading skeleton forever (right after our servers restarted, or when you switched conversations at just the wrong moment) are fixed; the loading view now always resolves within a few seconds.
- **Improved** — Switching between Wi-Fi and cellular mid-conversation now recovers much faster — requests stranded on the old network are cut off and retried right away instead of hanging.
- **Improved** — Our servers now detect and automatically recover from a rare internal stall that could previously make replies hang for everyone until we stepped in manually.
- **Fixed** — Excel (.xlsx) files you upload are now actually read and analyzed — previously the file was silently dropped on the way in, and Mars could end up analyzing unrelated data instead.
- **Fixed** — A batch of rendering fixes: amounts like "$6,000$" and fractions like "$1/3$" now render as proper math instead of literal dollar signs, flowcharts with Chinese quotation marks in their labels no longer fail to draw, and a chart block that arrives without its closing marker now still renders instead of showing raw code.
- **Improved** — The welcome screen feels smoother on iPhone — the glow animation now renders at full quality on every device (a visible color-banding artifact is gone), the input box expands without a sudden jump in Safari, and tapping the input no longer shoves the page around when the keyboard appears.

---

[Back to all releases](../README.md) · [Try Marsdata AI](https://marsdata.ai) · [简体中文](./2026-07-06-everyone-you-mention-now-gets-their-own-dossier.zh-CN.md) · [繁體中文](./2026-07-06-everyone-you-mention-now-gets-their-own-dossier.zh-HK.md)
