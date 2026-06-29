# DIRECTOR'S SHOT LIST — Performance Segment 001
### Opening Movement benchmark · HERO-02 "The Long Road" → HERO-03 "The First Recognition"

> **The cinematography spec.** Two artifacts, two purposes: the **Performance Segment Direction** (Director, Sam) describes the *emotion*; this **Shot List** describes the *cinematography* — the literal, timed shot breakdown every renderer (Sora · Veo · Grok) receives **identically**. Separating emotion from cinematography keeps the renderer comparison clean.
>
> **Role boundary (honored):** the Production Supervisor filled the **measurable spine** (timecodes, durations, governing anchor, lyric cue, narrative beats, Editorial Purpose, constraints). The **Camera** and **Performance** cells are the **Director's** — now **transcribed verbatim from PSD-001** (`PSD-001_Performance_Segment_Direction_OpeningMovement.md`). **COMPLETE** — this table is the locked cinematography spec feeding all three renderer packages.

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

| Shot | In – Out | Dur | Governing Anchor | Lyric cue (measured) | Narrative beat (canon) | Editorial Purpose | Camera *(PSD-001)* | Performance *(PSD-001)* |
|---|---|---|---|---|---|---|---|---|
| **1** | 29.62 – 35.92 | 6.30 s | HERO-02 (The Long Road) | "But none of them stayed here / Every road just led me back" | The long road — routine, solitude; centuries of walking. No awareness of Jen yet. | **Observe** | Slow trailing dolly, several paces behind Gary, eye-level. No dramatic movement, no orbit, no push — only gentle forward travel matching his walking speed. | Gary walks naturally, shoulders slightly lowered, eyes forward; peaceful but emotionally empty (not sad — accustomed to solitude). Workers/Nile/birds continue; nothing acknowledges him; the world is indifferent. |
| **2** | 36.08 – 39.58 | 3.50 s | HERO-02 → transition | "To another lonely night" → (instrumental beat into recognition) | The turn — the threshold from routine to the first flicker of awareness. | **Transition** | Continue the same trailing movement; almost imperceptibly reduce forward speed; camera begins lagging slightly behind Gary; audience subconsciously feels time stretching. | Walking rhythm changes by almost nothing — one slightly shorter step, one slower breath; he doesn't understand why. The pendant catches one brief reflection — natural, not magical — just enough to interrupt unconscious routine. Environment unchanged. |
| **3** | 39.58 – 42.22 | 2.64 s | HERO-03 (First Recognition) | "Till your smile cut through the dark" | **Recognition.** Gary notices Jen first (Rule #1); the pendant catches light; Jen's answer begins a heartbeat later. | **Reveal** | Remain observational — no push-in, no whip, no dramatic reveal. Allow Jen to enter frame naturally. Gary stops before the audience consciously expects him to. | Gary's eyes move first, body follows; shoulders soften; breathing pauses; he has no language for the feeling. Jen notices Gary — nothing more; only familiarity, recognition not yet conscious; her expression almost neutral. |

> ✅ **Camera + Performance transcribed verbatim from PSD-001 (Director, 2026-06-28).** Editorial Purpose confirmed (Observe / Transition / Reveal). This is now the locked cinematography spec; all three renderer packages derive from this table unchanged.

---

## How this feeds the benchmark
Once the Director fills Camera + Performance: the Production Supervisor transcribes them here, then issues **three identical packages** — Package A (Sora), B (Veo), C (Grok) — same Shot List, engine-appropriate syntax only. Each renderer animates start-anchor → end-anchor along these timed shots. **Gemini scores blind** on the motion scorecard (Emotional Performance 30 · Identity 25 · Camera 15 · Motion Continuity 15 · Prompt Fidelity 10 · Technical 5).

> *Status:* ✅ **COMPLETE** — spine + Camera + Performance all filled (PSD-001 transcribed). Feeds `Performance_Segment_001_Renderer_Packages.md` (**Veo · Grok**; Sora retired 2026).
