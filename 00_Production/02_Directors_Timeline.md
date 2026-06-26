# TEN LIFETIMES — Master Production Timeline

> **The backbone of the production.** One row per word. Every creative and technical decision references this table.
> When we're deep in a single shot, this is how we pull back to the whole film.

- **Version:** **v1.0 — LOCKED** (EP Gary, 2026-06-25; PT-0.5). Measured by TL-WO-001. fps = **24** confirmed. Chapter overlay approved as-is; Director details line-level chorus chapter-splits.
- **Last updated:** 2026-06-25 by Agent B
- **Runtime:** **329.60 s** (vocal stem) / 329.67 s (master mp3) — measured

---

## ✅ Timing status — MEASURED (TL-WO-001)

Timecodes below are **measured**, not estimated. TL-WO-001 completed:

1. ✅ **Exact duration** — 329.60 s (vocal stem) / 329.67 s (master mp3, ffprobe).
2. ✅ **Section boundaries** — measured from forced-alignment lyric anchors cross-checked against the **Drums** + **Percussion** stems (RMS energy envelope). Evidence: `20_REFERENCE\Section_Map_Measured.md`.
3. ✅ **Word-level timings** — forced alignment (stable-ts `medium.en` on vocal stem): 320 words, 66 lines. Full per-word table: `20_REFERENCE\master_timeline_words.md`.
4. ✅ **Premiere markers** — `20_REFERENCE\premiere_markers.csv` (16 markers @ 24 fps; section + key drum events). **fps = EP confirm.**

**✅ EP-LOCKED 2026-06-25 → PT-0.5.** (a) fps = **24** confirmed; (b) chapter overlay **approved as-is** — Director (Sam) to detail line-level chorus chapter-splits (Rome/Viking, Frontier/Victorian, WWII/Modern/Finale) as a follow-on, no re-lock required.

---

## 1. Master Production Timeline (format)

The canonical table. One row per word; columns per Director's spec:

| Time | Word | Beat | Emotion | Camera | Scene | Shot ID | VFX | Transition |
|---|---|---|---|---|---|---|---|---|

**Verse 1 stub (template — values to be measured/assigned):**

| Time | Word | Beat | Emotion | Camera | Scene | Shot ID | VFX | Transition |
|---|---|---|---|---|---|---|---|---|
| ~0:25.??? | *(whisper in)* | — | Lonely | Fade up | Egypt | TL-0010 | Sunrise/dust | from Cosmos |
| ~0:25.??? | I've | 1 | Lonely | Push in | Egypt | TL-0010 | Dust | None |
| ~0:26.??? | walked | 2 | Searching | Continue | Egypt | TL-0010 | Dust | None |
| ~0:27.??? | through | 3 | Wonder | Slow orbit | Egypt | TL-0010 | Sunlight | None |
| ~0:27.??? | empty | 4 | Lonely | Slow orbit | Egypt | TL-0010 | — | None |
| ~0:28.??? | centuries | 5 | Vastness | Widen | Egypt | TL-0020 | — | None |
| … | Chasing ghosts through fading dreams | — | Searching | — | Egypt | TL-0020 | ghost dissolves | None |
| … | Faces came and disappeared / But none of them stayed here | — | Yearning | — | Egypt | TL-0020 | faces fade | None |
| … | Till your smile cut through the dark | — | **Spark** | Push to Jen | Egypt | TL-0030 | light break | None |
| … | Like the first break of light | — | Hope | Two-shot | Egypt | TL-0030 | golden flare | → setup gesture |

*(**The full measured per-word table — all 320 words, Verse 1 through Outro, with Section / Chapter / Shot ID / Line — is generated and lives at `20_REFERENCE\master_timeline_words.md`.** The Beat / Emotion / Camera / VFX / Transition columns are the Director's to fill; the measured Time / Word / Section / Chapter / Shot ID are locked. Source lyrics: `20_REFERENCE\Lyrics_Annotated.md`.)*

**Beat** = musical beat index within the bar (filled from tempo/grid). **Scene** = chapter. **Shot ID** = `TL-####` from `03_Shot_Database.md`. Empty cells = "no change from row above."

---

## 2. Open structural decision (for Director + EP)

10 musical sections vs 10 chapters — they don't line up 1:1; the chapters are a **visual overlay** on a single first-person story. Built on **Strategy B (music-driven):** chapter changes land on musical events (drum entrances, key changes, the word that opens each chorus). Mapping below is the v0.1 proposal for Sam to redline.

---

## 3. Section Map (MEASURED — TL-WO-001)

Boundaries measured from forced-alignment lyric anchors cross-checked against the Drums + Percussion stems. Evidence: `20_REFERENCE\Section_Map_Measured.md`.

| # | Section | Start | End | Len | Music (measured) | Chapter overlay | Emotional arc |
|---|---|---|---|---|---|---|---|
| S0 | **Intro** | 0:00.00 | 0:19.02 | 19.0s | Solo piano, reversed textures, faint female "ahhh", **no drums** | **Cosmos / Before Time** | Wonder, mystery |
| S1 | **Verse 1** | 0:19.02 | 0:48.84 | 29.8s | Intimate close-mic, no drums | **Egypt** | Discovery, destiny |
| S2 | **Pre-Chorus 1** | 0:48.84 | 1:03.82 | 15.0s | Strings rise, light cello, female harmony, no drums | **Rome** | Recognition, certainty |
| S3 | **Chorus 1** | 1:03.82 | 1:51.84 | 48.0s | "I would wait ten lifetimes"; **soft drums build ~1:38, full kick ~1:45**; ends on held "I was always yours" | **Rome → Viking** | Lift; "I was always yours" |
| S4 | **Verse 2** | 1:51.84 | 2:19.60 | 27.8s | "You laugh and call me vampire blood"; heartbeat kick; **percussion enters ~2:00** | **Medieval** | Comfort, the half-myth wink |
| S5 | **Pre-Chorus 2** | 2:19.60 | 2:33.60 | 14.0s | "Maybe stars are witnesses"; choir pads | **Renaissance** | Inspiration, faith |
| S6 | **Chorus 2** | 2:33.60 | 3:19.66 | 46.1s | "I would wait ten lifetimes" (2nd); full percussion, deep toms; ends on held "You finally brought me life" | **Frontier → Victorian** | Bigger lift |
| S7 | **Bridge** | 3:19.66 | 4:05.05 | 45.4s | "If the world should fade tomorrow"; **DRUMS DROP at 3:20**; piano+strings+choir; **drums CRASH back at 3:48.3** under held "Beyond who we are" | **THE BRIDGE — leave history** | Loss → searching → transcendence |
| S8 | **Final Chorus** | 4:05.05 | 4:47.25 | 42.2s | "I would wait ten lifetimes" (final); massive swell, full choir, crashes; through "To find you again" | **WWII → Modern → ALL-COUPLES FINALE** | Full climax |
| S9 | **Outro** | 4:47.25 | 5:29.60 | 42.4s | "Maybe love is timeless"; **drums fade ~5:01**; final "mine" ends 5:15.57; final chord 5:14 | **Future → morph → REAL PHOTO** | Fulfillment, peace → real |

> **Key edit beat:** in the Bridge, the music re-ignites (drums crash back) at **3:48.3**, ~17 s *before* the vocal final chorus at 4:05.05 — two distinct beats. The drum re-entry is the cleanest boundary in the song and a prime VFX/transition anchor.
>
> Lyric hook to feature: **"You laugh and call me vampire blood / Half a man and half a myth / Like I've lived a thousand stories"** — the song's own wink at the ten-lifetimes conceit.

---

## 4. The Layered Edit Model
Every layer reads down the same timeline columns: Audio · Lyrics · Emotion · Camera · VFX · Color · Chapter · Shot IDs · Edit notes. To locate any work:
> *"Refining **TL-0042**: second half of Viking, just before the lift into Medieval — ~1:47.3–1:58.9."*

---

## 5. Change log
| Date | Version | Change | By |
|---|---|---|---|
| 2026-06-24 | v0.1 | Section map + Strategy-B mapping; estimates pending alignment | Agent B |
| 2026-06-24 | v0.1 | Reformatted to **Master Production Timeline** (9-col, one row/word) per Director review | Agent B |
| 2026-06-25 | **v1.0-draft** | TL-WO-001: section boundaries MEASURED (drums/perc stem + alignment); §3 estimates → measured; per-word table (320) + markers + prelim shot IDs generated to `20_REFERENCE\`. Awaiting EP lock → PT-0.5 | Agent B |
