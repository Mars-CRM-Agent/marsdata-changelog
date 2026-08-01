# Deep Research, rewritten — deeper and safer.

> Canonical source of record: [https://marsdata.ai/changelog](https://marsdata.ai/changelog)
> Release `0.1.1.1803` · 2026-05-26

- **New** — Deep Research mode rebuilt for depth and recovery — Mars now does a quick pre-search before asking you to confirm the research questions (so the suggested questions are grounded in what's actually out there), runs a cross-review pass after gathering sources, and continuously saves a recovery copy of the long report to cloud storage. If the final synthesis is ever interrupted (network blip, app close), the draft can be restored instead of starting from zero. The mode also waits for you to actually confirm the questions before it spends time on the deep dive, and won't ship a final report that came up suspiciously thin
- **Fixed** — Conversations that recently reopened as a blank loading shell now load correctly again — and a quieter problem where a single bad conversation could 500 the entire sidebar list has been closed at the same time. Previously affected conversations should now open, and the sidebar list should be reliable
- **Improved** — Read-aloud now reads cleaner prose — the play button no longer speaks JSON braces, code fences, or special HTML formatting blocks aloud, so playback sounds like someone reading you the answer rather than dictating syntax. Push-notification previews use the same cleanup, so the preview text on your lock screen reads as natural prose instead of raw markdown
- **Fixed** — Mermaid charts now render correctly on older iPhones (iOS 16) — a regex compatibility issue that left the chart blank on those devices is fixed
- **Fixed** — Math formulas that contained a currency escape next to a number (e.g. "$\$72亿$") no longer leave a red LaTeX error in place of the formula — the surrounding math now renders cleanly
- **Fixed** — Push notifications now reliably reach every device you've enabled them on — the prior design had a race where multiple devices could quietly deactivate each other's subscriptions, so the "task complete" push silently stopped arriving for many of you. Fleet now converges; each device is tracked independently
- **Improved** — WeChat Channel login flow smoother — when Mars opens a Channel page that needs you to log in, the right-side panel now auto-takes over so you can finish the login and Mars resumes the task. The panel also won't show up empty anymore when there's nothing to display, and the credentials you provided in one login flow are now correctly carried forward to subsequent sessions in the same conversation
- **Fixed** — An empty grey section box that occasionally appeared between sections of a long AI reply no longer shows up
- **Fixed** — The conversation title at the top of the sidebar no longer briefly flips between an early guess and the final version on the first turn — Mars now derives the title from your first message in a single authoritative step so it lands correctly the first time

---

[Back to all releases](../README.md) · [Try Marsdata AI](https://marsdata.ai) · [简体中文](./2026-05-26-deep-research-rewritten-deeper-and-safer.zh-CN.md) · [繁體中文](./2026-05-26-deep-research-rewritten-deeper-and-safer.zh-HK.md)
