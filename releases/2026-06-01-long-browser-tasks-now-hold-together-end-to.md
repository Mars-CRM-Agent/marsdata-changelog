# Long browser tasks now hold together end to end.

> Canonical source of record: [https://marsdata.ai/changelog](https://marsdata.ai/changelog)
> Release `0.1.1.1828` · 2026-06-01

- **Improved** — Long, multi-step tasks — especially ones where Mars drives a browser for you (logging into a site, clicking through pages, pulling data) — now stay reliable from start to finish. Previously a single conversation could get quietly handed off between our servers partway through, which sometimes dropped the browser's logged-in session and left a browser task stalled or failed. Now each conversation stays anchored in one place and the browser session is shared, so the browser keeps your login and picks up exactly where it left off, even across a long back-and-forth.

---

[Back to all releases](../README.md) · [Try Marsdata AI](https://marsdata.ai) · [简体中文](./2026-06-01-long-browser-tasks-now-hold-together-end-to.zh-CN.md) · [繁體中文](./2026-06-01-long-browser-tasks-now-hold-together-end-to.zh-HK.md)
