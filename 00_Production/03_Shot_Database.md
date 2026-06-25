# TEN LIFETIMES — Shot Database

> Every shot in the film as a uniquely-ID'd, searchable record. Eventually ~80–120 entries.
> Each shot traces up to the Timeline (when) and the Bible (why).

- **Version:** v0.1 (schema + seed shots; populated as the Timeline locks)
- **Last updated:** 2026-06-24 by Agent B

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

## Chapter shot allocation (target 7 stills/chapter → ~70 + cosmos/bridge/finale)

| Chapter | ID block | Planned | Generated | Approved |
|---|---|---|---|---|
| Cosmos / Intro | TL-0001–0009 | 3 | 0 | 0 |
| Egypt | TL-0010–0079 | 0/7 | 0 | 0 |
| Rome | TL-0080–0149 | 0/7 | 0 | 0 |
| Viking | TL-0150–0219 | 0/7 | 0 | 0 |
| Medieval | TL-0220–0289 | 0/7 | 0 | 0 |
| Renaissance | TL-0290–0359 | 0/7 | 0 | 0 |
| Frontier | TL-0360–0429 | 0/7 | 0 | 0 |
| Victorian | TL-0430–0499 | 0/7 | 0 | 0 |
| WWII | TL-0500–0569 | 0/7 | 0 | 0 |
| Modern | TL-0570–0639 | 0/7 | 0 | 0 |
| Future | TL-0640–0709 | 0/7 | 0 | 0 |
| Bridge | TL-0710–0799 | 0 | 0 | 0 |
| Finale / Real ending | TL-0800–0899 | 0 | 0 | 0 |

*(Generation order per Bible §13: Modern → Future → Victorian → Frontier → Renaissance → Medieval → Viking → Rome → Egypt, then Bridge & Finale.)*
