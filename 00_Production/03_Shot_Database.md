# TEN LIFETIMES — Shot Database

> Every shot in the film as a uniquely-ID'd, searchable record. Eventually ~80–120 entries.
> Each shot traces up to the Timeline (when) and the Bible (why).

- **Version:** v0.2 (preliminary shots assigned from measured Timeline — TL-WO-001)
- **Last updated:** 2026-06-25 by Agent B
- **Preliminary per-line shot list:** `20_REFERENCE\shot_database_prelim.md` (66 lyric-line shots TL-0010–TL-0660 + 3 intro). One shot per lyric line; Director subdivides during generation.

---

## Shot-ID schema

`TL-####` — zero-padded, assigned in **timeline order** (TL-0001 = first frame). Leave gaps (increment by 10 within a chapter: TL-0010, TL-0020…) so inserts don't force renumbering.

**Status values:** `PLANNED` → `PROMPTED` (prompt written) → `STILL_GEN` (image generated) → `STILL_APPROVED` → `MOTION_GEN` (clip generated) → `APPROVED` (canon, in edit) → `RETIRED`.

**Every shot record carries these fields:**

| Field | Meaning |
|---|---|
| ID | TL-#### |
| Chapter | Cosmos / Egypt / … / Bridge / Finale |
| Timecode | start–end (from Director's Timeline) |
| Duration | seconds (≤ tool max, Sora ≈ 20s) |
| Type | hero portrait / medium interaction / environmental wide / close-up / ending frame / transition / VFX |
| Lens | 35 wide · 50 intimate · 85 close (per Bible §9) |
| Movement | dolly/push/orbit/static/crane… |
| Lighting | key look |
| Color | dominant palette (Bible §7) |
| Emotion | one word |
| Gesture | the chapter's signature gesture if present (Bible §6) |
| Motif | silver pendant / clock gears / stars / … |
| Narrative Purpose | **why the shot exists** (the safeguard sentence — what emotional job it must do) |
| Tool | Sora / Nano Banana / Veo-Flow |
| Prompt | the generation prompt (or link to it) |
| Status | see above |

---

## Seed shots (examples — to expand)

### TL-0001 — Opening Star Field
- **Chapter:** Cosmos / Before Time · **Timecode:** ~0:00–0:12 · **Duration:** 12s
- **Type:** environmental wide · **Lens:** 50 · **Movement:** slow dolly in
- **Lighting:** celestial blue · **Color:** deep blue/black + silver starlight · **Emotion:** wonder
- **Gesture:** — · **Motif:** stars, drifting dust
- **Narrative Purpose:** Establish that love exists *outside* of history, waiting — before a single human appears. Sets the contract for the whole film.
- **Tool:** Veo/Flow (atmospheric) · **Status:** PLANNED · **Prompt:** _TBD_

### TL-0002 — Clockwork Awakens
- **Chapter:** Cosmos · **Timecode:** ~0:07–0:18 · **Duration:** 11s
- **Type:** VFX/insert · **Lens:** 85 · **Movement:** orbit
- **Lighting:** rim-lit brass · **Color:** deep blue + warm gold glints · **Emotion:** mystery
- **Motif:** clock gears, constellations forming two silhouettes
- **Narrative Purpose:** "Time itself awakens." Plant the clock-gear motif that will *stop* in the Bridge.
- **Tool:** Veo/Flow · **Status:** PLANNED · **Prompt:** _TBD_

### TL-0003 — Sunrise over Egypt (transition into Ch.1)
- **Chapter:** Cosmos → Egypt · **Timecode:** ~0:18–0:27 · **Duration:** 9s
- **Type:** transition · **Lens:** 35 · **Movement:** push through light
- **Lighting:** first rays / golden hour · **Color:** blue → gold morph · **Emotion:** awakening
- **Narrative Purpose:** Hand off from cosmos to the first lifetime on the whisper vocal; "their story begins."
- **Tool:** Sora (hero transition) · **Status:** PLANNED · **Prompt:** _TBD_

### TL-0010 — Egypt Hero Portrait
- **Chapter:** Egypt · **Timecode:** ~0:27–0:40 · **Duration:** ~12s (still→subtle motion)
- **Type:** hero portrait · **Lens:** 85 · **Movement:** slow push
- **Lighting:** warm gold, low sun · **Color:** gold · **Emotion:** destiny
- **Gesture:** (sets up) hands by the Nile · **Motif:** Egyptian amulet (silver pendant)
- **Narrative Purpose:** First reveal that these are believable people of their age — Gary the royal architect, Jen the noblewoman — yet unmistakably *them*. The audience's first "wait… is that the same couple?" seed.
- **Tool:** Nano Banana (consistency) → Sora (motion) · **Status:** PLANNED · **Prompt:** _TBD_

### TL-0020 — Egypt, Hands by the Nile (signature gesture)
- **Chapter:** Egypt · **Timecode:** ~0:45–0:58 · **Duration:** ~13s
- **Type:** medium interaction · **Lens:** 50 · **Movement:** slow orbit
- **Lighting:** golden hour, Nile reflections · **Color:** gold · **Emotion:** first spark
- **Gesture:** **holding hands beside the Nile** · **Motif:** silver pendant catches light
- **Narrative Purpose:** Land Egypt's signature gesture on "till your smile cut through the dark." This gesture's *motion* (fingers touching) seeds the sand→marble transition into Rome.
- **Tool:** Sora · **Status:** PLANNED · **Prompt:** _TBD_

---

## Chapter shot allocation — MEASURED (TL-WO-001, supersedes v0.1 guess)

Derived from the measured timeline: one preliminary shot per lyric line, numbered sequentially by 10 in timeline order. (The old v0.1 70-wide blocks assumed ~7 shots/chapter but the verse/chorus sections carry 8–10 lyric lines each, so ranges are now measured, not pre-allocated.)

| Chapter (overlay) | Shot ID range | Lines | Section |
|---|---|---|---|
| Cosmos / Intro | TL-0001 – TL-0003 | 3 intro | S0 |
| Egypt | TL-0010 – TL-0080 | 8 | S1 |
| Rome | TL-0090 – TL-0120 | 4 | S2 |
| Rome → Viking | TL-0130 – TL-0220 | 10 | S3 |
| Medieval | TL-0230 – TL-0300 | 8 | S4 |
| Renaissance | TL-0310 – TL-0340 | 4 | S5 |
| Frontier → Victorian | TL-0350 – TL-0420 | 8 | S6 |
| Bridge | TL-0430 – TL-0500 | 8 | S7 |
| WWII → Modern → Finale | TL-0510 – TL-0590 | 9 | S8 |
| Future → morph → Real | TL-0600 – TL-0660 | 7 | S9 |

> **Insert room:** subdivide any line-shot during generation as `TL-####a/b` or `+1..+9` (e.g. TL-0150 → TL-0151, TL-0152).
>
> ⚠️ **Reserved decision (Timeline §2):** the chorus/finale sections collapse multiple chapters into one section (S3 = Rome→Viking, S6 = Frontier→Victorian, S8 = WWII→Modern→Finale, S9 = Future→Real). Several historical chapters (Viking, Frontier, WWII, Modern) have **no dedicated solo section** — they live inside the choruses/montage. **Director + EP must ratify how the 10 historical chapters map onto the measured sections before generation.**

*(Generation order per Bible §13: Modern → Future → Victorian → Frontier → Renaissance → Medieval → Viking → Rome → Egypt, then Bridge & Finale.)*
