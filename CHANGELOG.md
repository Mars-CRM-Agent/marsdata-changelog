# Marsdata AI — product changelog

Every change we ship to **Marsdata AI** (also known as Mars Agent), the AI that maintains your relationships. This repository mirrors the changelog published at [https://marsdata.ai/changelog](https://marsdata.ai/changelog).

> Canonical source of record: [https://marsdata.ai/changelog](https://marsdata.ai/changelog)

## [Atlas turns your relationships into distinct, living circles.](releases/2026-08-13-atlas-turns-your-relationships-into-distinct-living-circles.md)

`0.1.1.2873` · 2026-08-13

- **New** — Atlas now organizes your relationship map into distinct circles. Each circle has its own color, focusing one reveals the people inside it, and someone who belongs in more than one part of your life can appear in more than one circle. People Mars cannot place yet stay visible as ungrouped planets instead of being filed under a dismissive catch-all label.
- **Improved** — A nickname, a new name and an uncertain match no longer collapse into the same person by default. Mars now asks you to confirm an unclear identity before it merges records, reveals personal details or writes new information, while an unmistakably new person can still be added without getting stuck in a confirmation loop.
- **Fixed** — Tell Mars about two people in the same message and each person's update now keeps its own result. Successful details stay saved even when another detail needs clarification, merge-and-split corrections restore the right records, and Mars reports partial outcomes instead of claiming that everything worked.
- **Improved** — Web answers are no longer forced through one blanket brevity rule. Mars can now give a fuller answer when the question needs context, while straightforward questions can still stay concise.

## [The words you mean to send now arrive ready to copy.](releases/2026-08-11-the-words-you-mean-to-send-now-arrive.md)

`0.1.1.2820` · 2026-08-11

- **New** — When Mars writes something you are meant to send — an opening line, a reply, a message to smooth something over — it now arrives in its own card with its own copy button, and what you get is exactly the text you will send: no heading, no explanation, no quote marks. Ordinary answers and whole-answer copy are unchanged. On the web for now.
- **New** — Ask Mars whether to do something and it now answers on two books instead of one: the practical costs and outcomes, and the private rule that makes the choice mean something about who you are. It builds that second reading only from what you actually told it, states it as a hypothesis rather than a verdict, and names the one observation that would overturn it — and when it does not know how someone else will react, it asks you instead of inventing them.
- **Improved** — Turning on deep research a second time now opens a fresh conversation instead of asking whether to restart the one you are already in. First activation, turning the mode off, and the upgrade prompt on the free plan all behave as before.
- **Fixed** — Answers stream word by word again. A security layer meant only for run-history requests was also matching the token stream, so it held every word back and replayed the whole answer in one burst at the end — measured as fifteen seconds of nothing followed by thirty events in three milliseconds. The model had been streaming correctly the whole time.
- **Fixed** — Lock your phone mid-answer and the text keeps moving when you come back. The rule that protects a live answer from being overwritten was keyed to the connection rather than to the run, so the moment the connection dropped in the background an older saved snapshot took over the display and the visible text froze — or advanced in lumps.
- **Fixed** — A turn that ends with nothing to show now says so. When the model finishes having thought but never actually speaks, you get a visible note telling you to retry — kept in the conversation rather than flashed once — instead of an empty bubble. And a reply that could not be recovered is no longer reported as successfully finished.
- **Fixed** — Images, videos and documents reach the model again. For a stretch at the start of August every upload was quietly dropped on the way in: the file was stored and appeared in your own bubble, and the model then asked you for a screenshot you had already sent.
- **Fixed** — Charts and mind maps that used to come out as a wall of raw code now draw. When the underlying description arrives with a missing bracket, full-width punctuation or invisible characters — or as one unbroken line — it is repaired and rendered instead of shown as source or as a conversion failure. Anything genuinely unreadable still falls back to code rather than being guessed at.
- **Improved** — Mars only says it saved something after it really did. Every write into a person's record now comes back with a receipt, and a claim without one is corrected before it reaches you — so "noted" stops being something the model can say out of politeness.
- **Improved** — Tell Mars six things about one person in a single breath and all six get recorded. They used to be split into six competing writes, of which one landed and the rest were dropped against a per-turn limit — while the reply confirmed all six anyway. One write now carries every field, each stamped with the exact sentence of yours that authorises it.
- **Fixed** — Deleting a person now also clears the names they went by. A whole-node delete used to leave the alias list still naming them, and the underlying folder was reported as gone without being checked; both are verified before the delete reports success, and anything that survives is shown to you as a partial delete rather than a clean one.
- **Fixed** — Journal entries read back at the time they happened. A note written at ten in the evening Beijing time was being rendered as two in the morning, and for a while the day's entries were not reaching the record at all. Deleting a preference now removes it, instead of only clearing the text and leaving the row behind.
- **Fixed** — Mention an old transfer again and Mars asks before booking it twice. Restating a payment from further back than its de-duplication window used to slip past the check that catches repeats, and an entry still waiting on your confirmation could be counted into the totals as settled.
- **Fixed** — Binding and unbinding a phone number works. A first-time bind never sent the code at all, unbinding signed you out while leaving the number bound, and the Unbind button answered every tap with a session-expired error. The two actions now also sit side by side as filled capsules, in the same visual language as the WeChat panel one row below.
- **Improved** — The welcome screen opens without waiting on the work behind it. Its relationship read used to be composed on the spot — eight scanners and one billed authoring call — before the page could answer, and a second visitor arriving inside that window waited on the first. It now serves what is already prepared and prepares the next batch after the page has loaded.
- **Fixed** — Signed-in visitors on iPhone stop landing on a half-drawn page. Safari implements none of the API the cache gate relied on, so a signed-in iOS visitor was served the anonymous copy of the page — after a release, the previous build's copy, whose asset addresses no longer exist — and what loaded was the header alone, with no composer and no sidebar. The gate no longer depends on that API, and a page that fails to come up now reloads itself.

## [Every person you know becomes a structured record.](releases/2026-08-01-every-person-you-know-becomes-a-structured-record.md)

`0.1.1.2598` · 2026-08-01

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

## [Mention a person right inside the chat.](releases/2026-07-24-mention-a-person-right-inside-the-chat.md)

`0.1.1.2383` · 2026-07-24

- **New** — You can now @-mention a person directly in chat — type @ and the picker opens on your Relationships by default, so you can pull someone you've already told Mars about straight into your message. Their key details ride along automatically.
- **New** — Upload a screenshot of a chat and Mars reads the conversation style, then offers to save a personalized reply coach for that exact person — one tap turns it into a reusable skill you can call anytime with /.
- **Improved** — After you save a reply coach, Mars now confirms it back to you — what got saved, that it'll recognize this person next time, and how to invoke it — so you're never left guessing whether the save actually worked.
- **New** — @-mention someone and Mars shows a rich relationship card right inside your message — their recent facts, latest interactions, and a short profile excerpt — instead of a plain name tag.

## [All three models step up to 1.7.](releases/2026-07-22-all-three-models-step-up-to-1-7.md)

`0.1.1.2353` · 2026-07-22

- **New** — All three models upgraded: 1.6 becomes 1.7. mini moves to a newer-generation fast model, while think and pro both step up to the brand-new flagship engine released this week — think tuned for speed, pro tuned for maximum reasoning depth. Smarter on complex analysis and long tasks, and each answer now costs less than before.
- **Improved** — Memory got smarter too — the engine that quietly captures people and facts from your conversations was upgraded to a newer model, so what Mars remembers is more accurate and better organized.

## [Atlas · Relation Nebula is live.](releases/2026-07-20-atlas-relation-nebula-is-live.md)

`0.1.1.2324` · 2026-07-20

- **New** — New: Atlas · Relation Nebula — a 3D star map of your relationships. Every person you've told Mars about becomes a star; tap one to fly in and watch their key facts orbit it like moons, tap again to open the full dossier. Includes search, quick-jump chips, and a fullscreen mode, tuned for both desktop and phone.
- **New** — Your Deep Research reports live in the star map too — each research topic is a planet whose moons are the titles of that session's documents; tap the planet to browse and read every document, including the full report and each dimension chapter.
- **New** — Sign in with your +86 phone number — receive a code by SMS with a live validity countdown. A new Account & Security section in Settings lets you bind, change, or unbind your phone, change your password, and read the privacy policy without leaving the app.
- **New** — PowerPoint (.pptx / .ppt), Word (.doc), and Excel (.xls) uploads are now fully supported — Mars actually reads their contents instead of skipping them.
- **New** — Copying a reply now keeps its formatting — headings, tables, and lists paste cleanly into documents, and charts and diagrams come along as images.
- **Improved** — Opening a conversation from history is faster and more dependable — cold opens no longer stall, the loading skeleton always resolves instead of hanging, and a case where the page could go blank when jumping from the welcome screen is fixed.
- **Improved** — The site loads faster and replies start sooner during busy hours — first-time visitors get the welcome page near-instantly, and response start times under heavy load improved by an order of magnitude.
- **Fixed** — Text you typed in the input box now survives a page reload — drafts are kept per conversation, so an accidental refresh no longer eats your message.
- **Fixed** — Chart and math rendering fixes: quadrant charts now draw as clean interactive charts, timeline diagrams tolerate more formatting quirks from the model, and multi-line block math renders correctly instead of showing raw symbols.

## [Everyone you mention now gets their own dossier.](releases/2026-07-06-everyone-you-mention-now-gets-their-own-dossier.md)

`0.1.1.2173` · 2026-07-06

- **New** — Mars now automatically builds a structured record for each person you talk about — identity, background, how you know each other, key interactions, and an overall value read are extracted from your conversations into a dedicated database record and summarized on the person's page. Details you've already told Mars no longer get silently overwritten when new information arrives, and when two records turn out to be the same person, merging them now keeps everything from both sides.
- **New** — When you chat about someone Mars already knows, the conversation is now automatically filed into that person's folder — so everything about one person stays in one place without manual sorting.
- **Improved** — The person detail page got a cleaner desktop layout — interaction log, profile, and key facts now sit side by side in three equal columns instead of one long scroll, duplicated profile text is gone, and the memory panel now shows titles and writes new memories in your chosen language.
- **Improved** — Opening a conversation is more dependable — cases where a chat could stay stuck on the loading skeleton forever (right after our servers restarted, or when you switched conversations at just the wrong moment) are fixed; the loading view now always resolves within a few seconds.
- **Improved** — Switching between Wi-Fi and cellular mid-conversation now recovers much faster — requests stranded on the old network are cut off and retried right away instead of hanging.
- **Improved** — Our servers now detect and automatically recover from a rare internal stall that could previously make replies hang for everyone until we stepped in manually.
- **Fixed** — Excel (.xlsx) files you upload are now actually read and analyzed — previously the file was silently dropped on the way in, and Mars could end up analyzing unrelated data instead.
- **Fixed** — A batch of rendering fixes: amounts like "$6,000$" and fractions like "$1/3$" now render as proper math instead of literal dollar signs, flowcharts with Chinese quotation marks in their labels no longer fail to draw, and a chart block that arrives without its closing marker now still renders instead of showing raw code.
- **Improved** — The welcome screen feels smoother on iPhone — the glow animation now renders at full quality on every device (a visible color-banding artifact is gone), the input box expands without a sudden jump in Safari, and tapping the input no longer shoves the page around when the keyboard appears.

## [Projects — keep one topic in one clean space.](releases/2026-06-23-projects-keep-one-topic-in-one-clean-space.md)

`0.1.1.2098` · 2026-06-23

- **New** — Projects are here — a place to group related conversations together so a whole topic, person, or piece of work lives in one tidy space instead of being scattered across your chat list. Open a project and you'll see everything that belongs to it side by side.
- **New** — Each project now gathers the images and media from the conversations inside it automatically — so the photos and files you've shared on a topic show up together, no manual sorting needed.
- **New** — You can now name a project, pick a color for it, and rename or delete it anytime from a simple settings panel — making your projects easy to tell apart at a glance.
- **Improved** — The project view got a cleaner layout — a header that stays put while you scroll, and a sidebar that tucks itself away to give your content more room.

## [Mars now feels the time that passed between you.](releases/2026-06-18-mars-now-feels-the-time-that-passed-between.md)

`0.1.1.2018` · 2026-06-18

- **New** — Mars now keeps track of time across a conversation. When you come back after a few days away, it notices the gap instead of picking up the old plan as if no time had passed — so it won't keep pushing a next step that may already be behind you. It quietly checks how much time has passed since you last talked and re-confirms what may have changed before continuing.
- **Improved** — Mars is more honest about what it can't be sure of. Instead of confidently carrying forward stale assumptions, after a long gap it now asks where things stand now — cutting down the kind of mix-ups where it acts on information that's days out of date.

## [A smoother home screen, answers shaped to the question.](releases/2026-06-14-a-smoother-home-screen-answers-shaped-to-the.md)

`0.1.1.1967` · 2026-06-14

- **Improved** — The home screen now runs smoother and uses less battery — the glowing animation on the welcome page automatically goes lighter on older or slower phones, so it stays fluid instead of stuttering, and it quietly rests when you scroll it out of view. It also looks a little cleaner.
- **Improved** — Mars now answers in the way that suits your question — if you ask how to do something, it gives you the answer up front; if you ask for advice on a decision, it walks you through the thinking first; and if you just need to talk something out, it listens and responds with understanding before anything else.

## [The memory panel became a relationship graph.](releases/2026-06-13-the-memory-panel-became-a-relationship-graph.md)

`0.1.1.1959` · 2026-06-13

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

## [Long browser tasks now hold together end to end.](releases/2026-06-01-long-browser-tasks-now-hold-together-end-to.md)

`0.1.1.1828` · 2026-06-01

- **Improved** — Long, multi-step tasks — especially ones where Mars drives a browser for you (logging into a site, clicking through pages, pulling data) — now stay reliable from start to finish. Previously a single conversation could get quietly handed off between our servers partway through, which sometimes dropped the browser's logged-in session and left a browser task stalled or failed. Now each conversation stays anchored in one place and the browser session is shared, so the browser keeps your login and picks up exactly where it left off, even across a long back-and-forth.

## [Deep Research, rewritten — deeper and safer.](releases/2026-05-26-deep-research-rewritten-deeper-and-safer.md)

`0.1.1.1803` · 2026-05-26

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

[简体中文](./CHANGELOG.zh-CN.md) · [繁體中文](./CHANGELOG.zh-HK.md)
