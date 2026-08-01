# Every person you know becomes a structured record.

> Canonical source of record: [https://marsdata.ai/changelog](https://marsdata.ai/changelog)
> Release `0.1.1.2598` · 2026-08-01

- **New** — Everything you tell Mars about a person is now kept as a structured record — every detail is its own field, sitting next to that person's interaction log, money ledger and change history. Edit one detail and only that detail changes; remove one and the person, their history and everything else you saved stay exactly where they were.
- **Improved** — One person, one record. Mars no longer splits the same contact across several entries, no longer turns a role word like "my date" into a person of its own, and books one transfer as exactly one row.
- **Improved** — Details Mars captures on its own now carry a confidence level. When it is confident enough to treat two entries as the same person or the same payment, it tells you it did instead of merging quietly; when it isn't sure — especially about money — it holds the entry and asks you first, and anything still waiting on your answer is left out of the totals.
- **Improved** — Your personal memory — your goals, your preferences, your own profile — is now read in full on every turn instead of being partially searched, so Mars stops missing something you already told it.
- **Fixed** — Delete something and it is really gone. A person or a detail you removed no longer comes back from an older copy, and Mars no longer recites a value you deleted as if it were still current.
- **New** — The relationship cards on the welcome screen now answer instead of asking. Tap one and Mars opens with the analysis it has already done — who has gone quiet, which promises are still open, who among the people you just met is worth following up — rather than handing you an empty composer.
- **New** — @-mention someone in chat and Mars now reads their structured record — the fields, the recent interactions, the ledger — so a detail you just corrected or deleted is reflected in the very next answer.
- **New** — Send a screenshot of a chat or a transfer and the facts inside it settle into that person's record on their own — including exchanges that involve no money at all, which previously had nowhere to land.
- **New** — Signing in no longer asks for a password — there is nothing to register and nothing to remember. If you already set a password, the entry to it is still on the sign-in card.
- **New** — Hong Kong Traditional Chinese is now a language you can actually read the whole product in — the app, the landing pages and the relationship views included.
- **Fixed** — Ask a follow-up about a finished research report and Mars answers from the report itself, instead of starting the whole research over. Reloading the page during a long task also lets you watch it continue live again, rather than staring at a silent screen until it ends.
- **Fixed** — A skill you imported is findable again — some imports were saved successfully but could never be recalled afterwards, so they silently did nothing.

---

[Back to all releases](../README.md) · [Try Marsdata AI](https://marsdata.ai) · [简体中文](./2026-08-01-every-person-you-know-becomes-a-structured-record.zh-CN.md) · [繁體中文](./2026-08-01-every-person-you-know-becomes-a-structured-record.zh-HK.md)
