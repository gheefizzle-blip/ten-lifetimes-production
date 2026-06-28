# DIRECTOR'S SHOT LIST — Performance Segment 001
### Opening Movement benchmark · HERO-02 "The Long Road" → HERO-03 "The First Recognition"

> **The cinematography spec.** Two artifacts, two purposes: the **Performance Segment Direction** (Director, Sam) describes the *emotion*; this **Shot List** describes the *cinematography* — the literal, timed shot breakdown every renderer (Sora · Veo · Grok) receives **identically**. Separating emotion from cinematography keeps the renderer comparison clean.
>
> **Role boundary:** the Production Supervisor fills the **measurable spine** (timecodes, durations, governing anchor, lyric cue, already-canonized narrative beats, locked constraints). The **Camera** and **Performance** cells are the **Director's** — populated from Sam's Performance Segment Direction. This is a **SCAFFOLD** until that Direction lands; the creative cells are reserved, not invented.

---

## Span & sources (locked)
- **Benchmark span:** ~**29.62 s – 42.22 s** (≈12.6 s) — candidate window, **Director confirms exact in/out**. Covers the back of *The Long Road* into *The First Recognition*. (EDL-001 allocates Egypt 0:19.02–0:48.84; HERO-02 governs 19.02–38.80, HERO-03 governs 39.58–42.22.)
- **Start anchor (condition from):** `14_Selected/Seq01/TL-0010_Egypt_TheLongRoad_v3.png`
- **End anchor (arrive at):** `14_Selected/Seq01/TL-0070_Egypt_FirstRecognition_v5.png`
- **Lyric/timecode source:** `20_REFERENCE/alignment/lines.csv` (measured).

## Locked constraints (every shot, no exceptions)
- Identity = CCA-001 (Gary) / CCA-002 (Jen) — **no drift.** · Costumes = Egypt Architect / Scholar. · **Silver pendant present.** · **No eyewear** (CD-001, pre-WWII). · Timing is **immutable** (master clock). · Recognition Rules: **Gary notices first; Jen answers a heartbeat later; the pendant catches light first.**

---

## The shots

| Shot | In – Out | Dur | Governing Anchor | Lyric cue (measured) | Narrative beat (canon) | Camera *(Director)* | Performance *(Director)* |
|---|---|---|---|---|---|---|---|
| **1** | 29.62 – 35.92 | 6.30 s | HERO-02 (The Long Road) | "But none of them stayed here / Every road just led me back" | The long road — routine, solitude; centuries of walking. No awareness of Jen yet. | *[Performance Segment Direction]* | *[Performance Segment Direction]* |
| **2** | 36.08 – 39.58 | 3.50 s | HERO-02 → transition | "To another lonely night" → (instrumental beat into recognition) | The turn — the threshold from routine to the first flicker of awareness. | *[Performance Segment Direction]* | *[Performance Segment Direction]* |
| **3** | 39.58 – 42.22 | 2.64 s | HERO-03 (First Recognition) | "Till your smile cut through the dark" | **Recognition.** Gary notices Jen first (Rule #1); the pendant catches light; Jen's answer begins a heartbeat later. | *[Performance Segment Direction]* | *[Performance Segment Direction]* |

> Shot count, in/out points, and the split at 36.08 are a **proposed scaffold** for the Director to confirm or re-cut. The **Camera** and **Performance** columns are intentionally empty — they are authored by the Director's Performance Segment Direction and then transcribed here verbatim, so all three renderers receive identical cinematography.

---

## How this feeds the benchmark
Once the Director fills Camera + Performance: the Production Supervisor transcribes them here, then issues **three identical packages** — Package A (Sora), B (Veo), C (Grok) — same Shot List, engine-appropriate syntax only. Each renderer animates start-anchor → end-anchor along these timed shots. **Gemini scores blind** on the motion scorecard (Emotional Performance 30 · Identity 25 · Camera 15 · Motion Continuity 15 · Prompt Fidelity 10 · Technical 5).

> *Status:* format locked; measurable spine filled; **Camera + Performance reserved for the Director's Performance Segment Direction.** No renderer package issues until those cells are populated.
