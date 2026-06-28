# TEN LIFETIMES — EDL-001 · Master Runtime Allocation

> **The timeline controls the visuals. Visual ambition does not control the timeline.** (Director's governing rule, EDL-001.)
> This document allocates all **329.60 s** of the film across the ten lifetimes + framing blocks **before any motion is generated.** We build video to this schedule, not the reverse.

- **Work order:** EDL-001 (Director Sam → EP Gary → Production Supervisor Claude). Issued 2026-06-28.
- **Status:** ✅ **v1.0 — CANON LOCKED (EP Gary, 2026-06-28). IMMUTABLE.** The music is now the **master clock**. Frozen permanently: the 329.60 s runtime · the emotional allocation across all ten lifetimes · narrative pacing · the chorus boundaries (**B / A / B**) · Egypt's 29.82 s · the Bridge as interstitial · the Performance Segment methodology. **Director's Standing Order:** no runtime / era-duration / chorus-split / emotional-allocation changes are authorized — ever. We no longer ask *"how long should this scene be?"* — only *"how do we make these allocated seconds emotionally unforgettable?"* **The Planning Phase is closed; Production begins.**
- **Built on MEASURED data** (TL-WO-001 forced alignment, EP-LOCKED 2026-06-25): section boundaries from drums/percussion stems × lyric anchors; line timings from `20_REFERENCE\alignment\lines.csv`; total **329.60 s** (vocal stem), fps **24**.
- **All boundaries are now measured lyric-line times** — no proposals remain.

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

> The chorus sub-splits move boundaries *within* the shared regions, so the ten-era total (251.16 s) and average (25.1 s) are unchanged — only the balance between paired eras shifted per the Director's rulings.

**Egypt — extended or compressed?** The music decides, and it decides in your favor: Egypt = **Verse 1 = 29.82 s**, the **single longest era** (~19 % over the 25.1 s average) — "slightly longer because it introduces the emotional grammar." It does **not** approach a full minute, so **no later era has to be compressed to pay for it.** ✅ Director-LOCKED.

---

## 2. Master Runtime Allocation — all 13 blocks (the spine, all splits baked in)

Times are MEASURED section/line boundaries. `mm:ss` and seconds both given. **Narrative Function** = the emotional job of the block. "Video-gen target" = clip count × length; Sora ≈ 20 s max per clip.

| # | Block (Era) | Start | End | Dur | **Narrative Function** | Section / Music | Lyric cue (first line) | Anchor IDs | Transition IN | Video-gen target |
|---|---|---|---|---|---|---|---|---|---|---|
| 0 | **Cosmos — "Before Time"** *(prologue)* | 0:00.00 / 0.00 | 0:19.02 / 19.02 | **19.02** | **Establish the Eternal** — the soul before time | S0 Intro — solo piano, reversed textures, **no drums** | *(instrumental)* | **HERO-01 · TL-0001** 🔒 | Fade up from black | 1–2 clips, ~10–19 s (slow drift) |
| 1 | **Egypt** | 0:19.02 / 19.02 | 0:48.84 / 48.84 | **29.82** | **Introduce the Search → First Recognition → First Hope** (set the emotional grammar) | S1 Verse 1 — intimate, no drums | "I've walked through empty centuries" | **HERO-02 · TL-0010** 🔒 · **HERO-03 · TL-0070** 🔒 · **HERO-04 · TL-0080** 🔒 | Dust/sunrise dissolve from Cosmos | 1 Performance Segment, 4 clips (see §4) |
| 2 | **Rome** | 0:48.84 / 48.84 | 1:11.12 / 74.50 | **25.66** | **Recognition Deepens → time becomes the subject** (ends on "every age") | S2 Pre-Chorus 1 + Chorus 1 (to "every age") | "Maybe souls remember" | *(none yet)* | Light-flare match-cut from Egypt | 3 clips, ~7–8 s |
| 3 | **Viking** | 1:11.12 / 74.50 | 1:51.84 / 111.84 | **37.34** | **The Search Continues → The Vow** — refocus on Jen, then "I was always yours" | S3 Chorus 1 (from "Just to find your eyes") — **soft drums build ~1:38, FULL KICK ~1:45**, held vow to 1:51.84 | "Just to find your eyes" | *(none yet)* | **Shift to Jen on "Just to find your eyes"** (search, not history) | 3–4 clips; 15 s held vow = 1 sustained clip |
| 4 | **Medieval** | 1:51.84 / 111.84 | 2:19.60 / 139.60 | **27.76** | **Comfort & the Wink** — the half-myth, ease | S4 Verse 2 — heartbeat kick, **percussion enters ~2:00** | "You laugh and call me vampire blood" | *(none yet)* | Hard cut on the heartbeat kick | 3–4 clips, ~7–8 s |
| 5 | **Renaissance** | 2:19.60 / 139.60 | 2:33.60 / 153.60 | **14.00** | **Faith** — stars as witnesses (brief, luminous) | S5 Pre-Chorus 2 — choir pads | "Maybe stars are witnesses" | *(none yet)* | Light-bloom dissolve | 2 clips, ~7 s (impressionistic) |
| 6 | **Frontier** | 2:33.60 / 153.60 | 2:55.76 / 175.76 | **22.16** | **Choosing Each Other → commitment becomes the subject** (ends on "forever starts tonight") | S6 Chorus 2 (to "forever starts tonight") — full percussion, deep toms | "I would wait ten lifetimes" (2nd) | *(none yet)* | Lift cut on chorus downbeat | 3 clips, ~7 s |
| 7 | **Victorian** | 2:55.76 / 175.76 | 3:19.66 / 199.66 | **23.90** | **Living With the Choice (Consequence)** — the grand held swell | S6 Chorus 2 (from "endless years") — held "You finally brought me life" to 3:19.66 | "And after all these endless years" | *(none yet)* | Match-cut on "forever starts tonight" | 2–3 clips; 20 s held note = 1 sustained clip |
| 8 | **THE BRIDGE — "leave history"** *(interstitial — LOCKED, not a lifetime)* | 3:19.66 / 199.66 | 4:05.05 / 245.05 | **45.39** | **Leave History — Loss → Searching → Transcendence** (timeless space; history falls away) | S7 Bridge — **DRUMS DROP at 3:20**, piano+strings+choir, **DRUMS CRASH BACK at 3:48.3** | "If the world should fade tomorrow" | *(VFX/transition shots — not a lifetime)* | **The drop** = cut to void on 3:20 | 4–5 clips; **3:48.3 crash = the cleanest cut in the song** |
| 9 | **WWII** | 4:05.05 / 245.05 | 4:14.63 / 258.19 | **13.14** | **The Darkest Century — war, winter, rise & rust** (history endured) | S8 Final Chorus (to "rise and rust") — massive swell, full choir | "I would wait ten lifetimes" (final) | *(none yet)* | Crash cut out of the Bridge | 2 clips, ~6–7 s (compressed/intense) |
| 10 | **Modern** | 4:14.63 / 258.19 | 4:47.25 / 287.25 | **29.06** | **History Becomes Personal Again → Every Lifetime at Once** (all-couples finale) | S8 Final Chorus (from "final curtain falls") — crashes; **ALL-COUPLES FINALE** begins; held "To find you again" to 4:47.25 | "And when the final curtain falls" | *(montage of locked anchors)* | **On "final curtain falls" — line leaves history, becomes Gary & Jen** | Montage — rapid cuts of prior anchors + new |
| 11 | **Future** | 4:47.25 / 287.25 | 5:15.57 / 315.57 | **28.32** | **Fulfillment / Peace** — love is timeless | S9 Outro — **drums fade ~5:01**; final "mine" ends 5:15.57 | "Maybe love is timeless" | *(none yet)* | Gentle dissolve, drums receding | 3 clips, ~8 s; ends on the morph |
| 12 | **Ending fade — morph to REAL PHOTO** | 5:15.57 / 315.57 | 5:29.60 / 329.60 | **14.03** | **Return to the Real** — the lifetimes resolve into now | S9 tail — final chord ~5:14, silence to 5:29.6 | *(instrumental tail)* | *(real photograph reveal)* | Morph from Future-Jen → **real photo of Gary & Jen** | 1 clip, ~14 s (morph + slow fade to black) |

**Sum check:** 19.02 + 29.82 + 25.66 + 37.34 + 27.76 + 14.00 + 22.16 + 23.90 + 45.39 + 13.14 + 29.06 + 28.32 + 14.03 = **329.60 s** ✅ (full runtime allocated, zero gaps).

---

## 3. Crescendo & cut map (where edits must land)

| Time | Musical event | Use as |
|---|---|---|
| 0:19.02 | First vocal "I've walked" | Cosmos → Egypt |
| 0:48.84 | Strings rise (pre-chorus 1) | Egypt → Rome |
| 1:11.12 | "Just to find your eyes" | **Rome → Viking** (ruled B — time becomes the subject) |
| ~1:45 | **Full kick drum enters** | Peak of Viking lift (under "I was always yours") |
| 1:51.84 | Verse 2 + heartbeat kick | Viking → Medieval |
| ~2:00 | Percussion layer enters | Mid-Medieval energy step |
| 2:33.60 | Chorus 2 downbeat | Renaissance → Frontier |
| 2:55.76 | "Then forever starts tonight" | **Frontier → Victorian** (ruled A — commitment becomes the subject) |
| **3:19.66 / 3:20** | **DRUMS DROP** | Victorian → Bridge (cut to void) |
| **3:48.3** | **DRUMS CRASH BACK** | **Mid-Bridge — the single cleanest cut in the song**; the soul leaves history |
| 4:05.05 | Final chorus, massive swell | Bridge → WWII (climax) |
| 4:14.63 | "And when the final curtain falls" | **WWII → Modern** (ruled B — history becomes personal) |
| ~5:01 | Drums fade | Modern → Future settling |
| 5:15.57 | Last vocal "mine" | Future → real-photo morph |

---

## 4. Worked example — Egypt internal breakdown (the locked era + the first Performance Segment)

Egypt is the only era with locked anchors; it templates how every era subdivides into anchor + Performance Segment + transition. A **Performance Segment** = the directed motion chain between two anchors (PRO-017).

| Segment | Time | Dur | **Narrative Function** | Lyric | Anchor | Motion / job | Video-gen target |
|---|---|---|---|---|---|---|---|
| Enter | 19.02 | — | *(dust up)* | *(instrumental)* | — | Dissolve from Cosmos | (part of clip 1) |
| **The Long Road** | 19.02 – 38.80 | 19.78 | **Loneliness / The Search** | "I've walked through empty centuries" → "To another lonely night" (lines 0–5) | **HERO-02 TL-0010** 🔒 | A **Performance Segment**: push-in → slow orbit → widen. **2–3 directed clips** (one still cannot carry 20 s) + possibly 1–2 supporting anchors *(flagged future)* | 2–3 clips, ~7 s each |
| **The First Recognition** | 39.58 – 42.22 | 2.64 | **Recognition** — he notices her (Rule #1) | "Till your smile cut through the dark" (line 6) | **HERO-03 TL-0070** 🔒 | One clip. | 1 clip, ~3–4 s |
| **The First Smile** | 42.82 – 48.84 | 6.02 | **Hope** — the first crack in the armor | "Like the first break of light" (line 7) + instrumental tail | **HERO-04 TL-0080** 🔒 | Trajectory: stillness → soften → smile; golden flare carries into Rome | 1 clip, ~6 s |

> HERO-02 "The Long Road" is the natural site of our **first Performance Segment test** (Director's post-EDL priority, extended to the full HERO-01→04 opening). A planning note, **not** an EDL-001 generation action.

---

## 5. Video-generation strategy (targets, not media)

- **Unit of production = the Performance Segment** (the motion chain between two anchors), not the individual clip.
- **Clip length:** plan motion in **4–8 s** directed segments; **held notes** (Viking 15 s, Victorian 20 s, Bridge) may be single sustained clips (Sora ≈ 20 s ceiling). Never generate one 30 s era as a single clip.
- **Impressionistic acceleration:** Egypt (establishing grammar) is densest; later eras become **fewer, faster clips** as the song accelerates. WWII at 13 s is intentionally compressed/intense; density follows the music.
- **Rough clip budget (whole film):** ~**38–46 motion clips** across the 13 blocks.

---

## 6. The five redlines — Director's rulings (CLOSED)

| # | Item | Director's ruling |
|---|---|---|
| 1 | **Shared-chorus sub-splits** | ✅ **RULED — see §8.** Rome\|Viking = **B** (after "every age"); Frontier\|Victorian = **A** (after "forever starts tonight"); WWII\|Modern = **B** (after "rise and rust"). |
| 2 | **Bridge — interstitial or 11th era?** | ✅ **LOCKED as interstitial** — the moment history falls away; timeless space, not a civilization. |
| 3 | **All-couples finale start** | ✅ **Editorial lock after rough cut.** Modern (S8b) is its provisional home. |
| 4 | **Egypt at 29.8 s** | ✅ **LOCKED** — the longest era; not revisited. |
| 5 | **HERO-02 as a multi-clip Performance Segment** | ✅ **LOCKED** — validates the Performance Segment concept. |

> **All five resolved.** EDL-001 is ready for the EP's permanent lock. After the lock, runtime allocation is **frozen forever** — never reopened.

---

## 8. Chorus Sub-Split Decision — RESOLVED (Director, 2026-06-28)

The Director ruled each split on a **change of meaning, not merely a change of time** — so each new era begins with a new emotional question, giving every lifetime its own identity.

| Shared chorus | Selection | Split at | Director's reason |
|---|---|---|---|
| **Rome → Viking** | **Option B** | 1:11.12, after *"Lose myself in **every age**"* | That lyric is literally the transition between incarnations — the first place the audience consciously feels *time itself is no longer the boundary.* Viking then opens on *"Just to find your eyes,"* shifting focus from history back to Jen — the search continues. |
| **Frontier → Victorian** | **Option A** | 2:55.76, after *"Then forever starts tonight"* | Frontier ends on **commitment** (choosing each other); Victorian begins on **consequence** (living with that choice). A satisfying emotional cadence. |
| **WWII → Modern** | **Option B** | 4:14.63, after *"rise and rust"* | The strongest symbolic division in the song. WWII owns *"through every war / winter / rise and rust"* — humanity's darkest century. Modern opens on *"And when the final curtain falls"* — the line leaves history and becomes Gary & Jen. Personal again. |

> **The unifying principle (Director):** *Rome ends when time becomes the subject. Frontier ends when commitment becomes the subject. WWII ends when history becomes the subject.* Each succeeding era opens on a new emotional question.

---

## 7. Production gate

**No motion generation begins until this allocation is EP-locked** (EDL-001 §6–7 honored: nothing generated here). On EP lock, the music officially becomes the **master clock** — every future scene length is already answered; the only question left is *"how do we make these seconds unforgettable?"* From that point, runtime allocation is **frozen permanently — never reopened.**

**Director's post-EDL priority:** not another hero — the **first Performance Segment, built across the locked opening (HERO-01 → HERO-02 → HERO-03 → HERO-04 = Cosmos through Egypt, 0:00–0:48.84)**. The first time the studio produces motion as a *directed performance constrained by a locked emotional timeline* — the **proof-of-concept for the entire Continuum Creative methodology**, where we learn the camera / pacing / interpolation / continuity / emotional-timing lessons *before* Rome begins.

> *Inputs:* `02_Directors_Timeline.md` §3 (measured section map) · `20_REFERENCE\alignment\lines.csv` (66 line timings) · `20_REFERENCE\Section_Map_Measured.md` · locked anchors HERO-01..04. *Author:* Production Supervisor (Claude), translating EDL-001. *Status:* all narrative questions resolved → **awaiting EP permanent lock.**
