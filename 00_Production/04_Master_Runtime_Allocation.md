# TEN LIFETIMES — EDL-001 · Master Runtime Allocation

> **The timeline controls the visuals. Visual ambition does not control the timeline.** (Director's governing rule, EDL-001.)
> This document allocates all **329.60 s** of the film across the ten lifetimes + framing blocks **before any motion is generated.** We build video to this schedule, not the reverse.

- **Work order:** EDL-001 (Director Sam → EP Gary → Production Supervisor Claude). Issued 2026-06-28.
- **Status:** v0.1 — **DRAFT for Director review.** No media generated; no new hero shots created (per EDL-001 §6–7).
- **Built on MEASURED data** (TL-WO-001 forced alignment, EP-LOCKED 2026-06-25): section boundaries from drums/percussion stems × lyric anchors; line timings from `20_REFERENCE\alignment\lines.csv`; total **329.60 s** (vocal stem), fps **24**.
- **What is locked vs proposed:** Section boundaries and lyric-line times are **MEASURED (locked)**. Era→section assignments follow the **EP-approved chapter overlay** (Director's Timeline §3). The **sub-splits inside shared sections** (Rome|Viking, Frontier|Victorian, WWII|Modern) are **my proposals on lyric lines — Director's to redline.**

---

## 1. The math first (EP's question answered)

| Quantity | Value |
|---|---|
| Total runtime | **329.60 s** (5:29.6) |
| Instrumental intro (no vocals) | 0.00 – 19.02 s (19.02 s) |
| Vocal span | 19.02 – 315.57 s |
| Outro tail (after last vocal) | 315.57 – 329.60 s (14.03 s) |
| **Ten lifetimes (eras) total** | **251.16 s** |
| **Average per era** | **25.1 s** |
| Non-era framing (Cosmos prologue 19.02 + The Bridge 45.39 + ending fade 14.03) | 78.44 s |

**Egypt — extended or compressed?** The music decides, and it decides in your favor: Egypt = **Verse 1 = 29.82 s**, the **single longest era** (~19 % over the 25.1 s average) — "slightly longer because it introduces the emotional grammar," exactly as you framed it. It does **not** approach a full minute, so **no later era has to be compressed to pay for it.** The naturally short eras (Renaissance 14.0 s, WWII 19.7 s) are short because they sit on a pre-chorus and a chorus-half — impressionistic by the song's own structure, not by sacrifice. **Recommendation: accept Egypt at 29.8 s; do not extend it into the pre-chorus (that time belongs to Rome).**

---

## 2. Master Runtime Allocation — all 13 blocks (the spine)

Times are MEASURED section/line boundaries. `mm:ss` and seconds both given. "Video-gen target" = how the block should be produced (clip count × length); Sora ≈ 20 s max per clip, so held notes can be one long clip, walks become 2–4 clips.

| # | Block (Era) | Start | End | Dur | Section / Music | Lyric cue (first line) | Emotional beat | Anchor IDs | Transition IN | Video-gen target |
|---|---|---|---|---|---|---|---|---|---|---|
| 0 | **Cosmos — "Before Time"** *(prologue)* | 0:00.00 / 0.00 | 0:19.02 / 19.02 | **19.02** | S0 Intro — solo piano, reversed textures, **no drums** | *(instrumental)* | Wonder, mystery | **HERO-01 · TL-0001** 🔒 | Fade up from black | 1–2 clips, ~10–19 s (slow drift) |
| 1 | **Egypt** | 0:19.02 / 19.02 | 0:48.84 / 48.84 | **29.82** | S1 Verse 1 — intimate, no drums | "I've walked through empty centuries" | Discovery → spark of hope | **HERO-02 · TL-0010** 🔒 · **HERO-03 · TL-0070** 🔒 · **HERO-04 · TL-0080** 🔒 | Dust/sunrise dissolve from Cosmos | 4 clips (see §4) |
| 2 | **Rome** | 0:48.84 / 48.84 | 1:17.78 / 77.78 | **28.94** | S2 Pre-Chorus 1 + Chorus 1 (first half) — strings rise → "ten lifetimes" | "Maybe souls remember" | Recognition, certainty | *(none yet)* | Light-flare match-cut on "first break of light" | 3–4 clips, ~7–8 s |
| 3 | **Viking** | 1:17.78 / 77.78 | 1:51.84 / 111.84 | **34.06** | S3 Chorus 1 (second half) — **soft drums build ~1:38, FULL KICK ~1:45**, held "I was always yours" to 1:51.84 | "If time is just a river" | Epic lift; vow | *(none yet)* | Sweep / whip-pan on "every age" | 3–4 clips; the 15 s held note = 1 sustained clip |
| 4 | **Medieval** | 1:51.84 / 111.84 | 2:19.60 / 139.60 | **27.76** | S4 Verse 2 — heartbeat kick, **percussion enters ~2:00** | "You laugh and call me vampire blood" | Comfort, the half-myth wink | *(none yet)* | Hard cut on the heartbeat kick | 3–4 clips, ~7–8 s |
| 5 | **Renaissance** | 2:19.60 / 139.60 | 2:33.60 / 153.60 | **14.00** | S5 Pre-Chorus 2 — choir pads | "Maybe stars are witnesses" | Inspiration, faith | *(none yet)* | Light-bloom dissolve | 2 clips, ~7 s (impressionistic) |
| 6 | **Frontier** | 2:33.60 / 153.60 | 2:55.76 / 175.76 | **22.16** | S6 Chorus 2 (first half) — full percussion, deep toms | "I would wait ten lifetimes" (2nd) | Bigger lift, motion | *(none yet)* | Lift cut on chorus downbeat | 3 clips, ~7 s |
| 7 | **Victorian** | 2:55.76 / 175.76 | 3:19.66 / 199.66 | **23.90** | S6 Chorus 2 (second half) — held "You finally brought me life" to 3:19.66 | "And after all these endless years" | Grand swell, held | *(none yet)* | Match-cut on "forever starts tonight" | 2–3 clips; 20 s held note = 1 sustained clip |
| 8 | **THE BRIDGE — "leave history"** *(interstitial)* | 3:19.66 / 199.66 | 4:05.05 / 245.05 | **45.39** | S7 Bridge — **DRUMS DROP at 3:20**, piano+strings+choir, **DRUMS CRASH BACK at 3:48.3** | "If the world should fade tomorrow" | Loss → searching → transcendence | *(VFX/transition shots — not a lifetime)* | **The drop** = cut to void on 3:20 | 4–5 clips; **3:48.3 crash = the cleanest cut in the song** |
| 9 | **WWII** | 4:05.05 / 245.05 | 4:24.71 / 264.71 | **19.66** | S8 Final Chorus (first part) — massive swell, full choir | "I would wait ten lifetimes" (final) | Full climax begins | *(none yet)* | Crash cut out of the Bridge | 2–3 clips, ~7 s |
| 10 | **Modern** | 4:24.71 / 264.71 | 4:47.25 / 287.25 | **22.54** | S8 Final Chorus (second part) — crashes; **ALL-COUPLES FINALE montage** begins; held "To find you again" to 4:47.25 | "I'll still be reaching through eternity" | Climax, every lifetime at once | *(montage of locked anchors)* | Cross-dissolve into the montage | Montage — rapid cuts of prior anchors + new |
| 11 | **Future** | 4:47.25 / 287.25 | 5:15.57 / 315.57 | **28.32** | S9 Outro — **drums fade ~5:01**; final "mine" ends 5:15.57 | "Maybe love is timeless" | Fulfillment, peace | *(none yet)* | Gentle dissolve, drums receding | 3 clips, ~8 s; ends on the morph |
| 12 | **Ending fade — morph to REAL PHOTO** | 5:15.57 / 315.57 | 5:29.60 / 329.60 | **14.03** | S9 tail — final chord ~5:14, silence to 5:29.6 | *(instrumental tail)* | Real → peace → black | *(real photograph reveal)* | Morph from Future-Jen → **real photo of Gary & Jen** | 1 clip, ~14 s (morph + slow fade to black) |

**Sum check:** 19.02 + 29.82 + 28.94 + 34.06 + 27.76 + 14.00 + 22.16 + 23.90 + 45.39 + 19.66 + 22.54 + 28.32 + 14.03 = **329.60 s** ✅ (full runtime allocated, zero gaps).

---

## 3. Crescendo & cut map (where edits must land)

The cleanest, musically-true cut points — transitions should land on these, not on arbitrary seconds:

| Time | Musical event | Use as |
|---|---|---|
| 0:19.02 | First vocal "I've walked" | Cosmos → Egypt |
| 0:48.84 | Strings rise (pre-chorus 1) | Egypt → Rome |
| ~1:45 | **Full kick drum enters** | Peak of Viking lift (under "I was always yours") |
| 1:51.84 | Verse 2 + heartbeat kick | Viking → Medieval |
| ~2:00 | Percussion layer enters | Mid-Medieval energy step |
| 2:33.60 | Chorus 2 downbeat | Renaissance → Frontier |
| **3:19.66 / 3:20** | **DRUMS DROP** | Victorian → Bridge (cut to void) |
| **3:48.3** | **DRUMS CRASH BACK** | **Mid-Bridge — the single cleanest cut in the song**; the soul leaves history |
| 4:05.05 | Final chorus, massive swell | Bridge → WWII (climax) |
| ~5:01 | Drums fade | Modern → Future settling |
| 5:15.57 | Last vocal "mine" | Future → real-photo morph |

---

## 4. Worked example — Egypt internal breakdown (the locked era)

Egypt is the only era with locked anchors, so it sets the template for how every era is later subdivided into anchor + motion + transition. Lyric-line times are measured (`lines.csv`).

| Segment | Time | Dur | Lyric | Anchor | Motion / job | Video-gen target |
|---|---|---|---|---|---|---|
| Enter | 19.02 | — | *(dust up)* | — | Dissolve from Cosmos | (part of clip 1) |
| **The Long Road** | 19.02 – 38.80 | 19.78 | "I've walked through empty centuries" → "To another lonely night" (lines 0–5) | **HERO-02 TL-0010** 🔒 | The lonely walk: push-in → slow orbit → widen. **Likely needs 2–3 motion clips** + possibly 1–2 supporting anchors *(flagged future — not generated under EDL-001)* | 2–3 clips, ~7 s each |
| **The First Recognition** | 39.58 – 42.22 | 2.64 | "Till your smile cut through the dark" (line 6) | **HERO-03 TL-0070** 🔒 | He notices her — Recognition Rule #1. One clip. | 1 clip, ~3–4 s |
| **The First Smile** | 42.82 – 48.84 | 6.02 | "Like the first break of light" (line 7) + instrumental tail | **HERO-04 TL-0080** 🔒 | Hope blooms (Performance Trajectory: stillness → soften → smile); golden flare carries into Rome | 1 clip, ~6 s |

> Egypt confirms a structural truth: **a single anchor can own ~20 s of screen time only if its motion is broken into 2–3 directed clips** (and may want supporting sub-anchors). HERO-02 "The Long Road" is the first place this applies. This is a future hero/motion-planning note, **not** an EDL-001 action.

---

## 5. Video-generation strategy (targets, not media)

- **Clip length:** plan motion in **4–8 s** directed segments; **held notes** (Viking 15 s, Victorian 20 s, Bridge) may be single sustained clips (Sora ≈ 20 s ceiling). Never generate one 30 s era as a single clip — direct it as a sequence.
- **Rough clip budget (whole film):** ~**38–46 motion clips** + transitions across the 13 blocks (Egypt 4 · Rome 3–4 · Viking 3–4 · Medieval 3–4 · Renaissance 2 · Frontier 3 · Victorian 2–3 · Bridge 4–5 · WWII 2–3 · Modern montage · Future 3 · ending 1 · Cosmos 1–2).
- **Each motion clip is born from a Performance Anchor (PRO-017)** with a directed trajectory; transitions are timed to land on §3 crescendos.

---

## 6. Open decisions for Director / EP (redline these)

1. **Shared-section sub-splits** — confirm or move my proposed boundaries: **Rome|Viking at 1:17.78** (mid-Chorus 1), **Frontier|Victorian at 2:55.76** (mid-Chorus 2), **WWII|Modern at 4:24.71** (mid-Final Chorus). These are lyric-line cuts, not measured music events.
2. **The Bridge (45.4 s) is an interstitial "leave history," not an 11th lifetime** — confirm it stays framing (with Cosmos 19 s + ending 14 s) rather than being charged to an era's budget.
3. **All-couples finale placement** — I've seated it in **Modern (S8 second half) → carried through Future**; confirm whether the montage starts earlier (4:05 climax) or holds to 4:24.
4. **Egypt at 29.8 s** — accept as the longest era (recommended), or compress toward 25 s and hand the difference elsewhere.
5. **HERO-02 span** — "The Long Road" owns ~20 s on one locked anchor; approve planning 2–3 motion clips (and possibly future supporting anchors) for it.

---

## 7. Production gate

**No motion generation begins until this allocation is Director-approved** (EDL-001 §6–7 honored: nothing generated here). On approval, every future hero/motion shot is timed to this map; HERO-05 (the first Performance-Trajectory motion) is built **to its allocated slot**, not to ambition.

> *Inputs:* `02_Directors_Timeline.md` §3 (measured section map) · `20_REFERENCE\alignment\lines.csv` (66 line timings) · `20_REFERENCE\Section_Map_Measured.md` · locked anchors HERO-01..04. *Author:* Production Supervisor (Claude), translating EDL-001. *Awaiting:* Director redline → EP lock.
