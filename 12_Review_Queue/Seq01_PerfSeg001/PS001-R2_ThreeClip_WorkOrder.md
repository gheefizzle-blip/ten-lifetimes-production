# PS001-R2 — Three-Clip Motion Work Order (Opening Movement)
### Supervisor translation of `PSD-001-R2` (Director Sam) · HERO-02 → HERO-03 · 12.6 s = 3 × 4.2 s

> **Execution unit ≠ story unit.** PS001 is rebuilt as **three separate 4.2 s Veo clips assembled editorially** — no single continuous render. Each clip carries ONE storytelling job. Direction is preserved verbatim from `PSD-001-R2`; this doc adds only the technical conditioning/keyframe plan and lifecycle. Engine = Google Veo 3.1 (standard `veo-3.1-generate-preview`) via the Continuum Render Bridge.

## Locked constraints (every clip)
Gary = CCA-001, Jen = CCA-002 (no drift) · costumes Architect/Scholar · silver pendant present, subtle/natural · period-accurate New Kingdom Egypt, Nile riverbank at dawn · no eyewear (CD-001) · no anachronisms · timing immutable (4.2 s each).

## Performance Keyframes (new conditioning-still class — NOT Hero Anchors, do NOT alter canon)
Technical in-between stills generated via **Nano Banana**, **conditioned on the locked CCA face sheets + costumes (+ HERO anchors)**, used solely to seed/bound Veo so it cannot invent identity. This is the direct fix for the R1 face failure. Stored at `04_Egypt/Motion/PerfSeg001/Keyframes/` (NAS) + committed for review. Naming: `PK-PS001-<clip><a/b>`.

| Clip | Span | Job | Camera (PSD-001-R2) | Conditioning plan (start → end keyframe) |
|---|---|---|---|---|
| **C1 OBSERVE** | 0.0–4.2 | Isolation & scale | Elevated ~50 ft high / ~50 m behind Gary, descending+closing to ~2 m behind. "History following him, not a drone shot." | **start = `PK-PS001-C1a`** (NEW — elevated high rear, Gary small on the Nile riverbank) → **end = `PK-PS001-C1b`** (NEW — ~2 m behind Gary, matching HERO-02 framing). Both rear views; CCA-001 build/costume, no face needed. |
| **C2 TRIGGER** | 4.2–8.4 | Ordinary world breaks | Cut to **front / off-axis Gary**, looking past camera to the dawn over distant desert hills; ray catches the pendant. | **start = `PK-PS001-C2a`** (NEW — front/off-axis Gary, routine, eyes not yet shifted; **CCA-001 face — identity-critical**) → **end = `PK-PS001-C2b`** (NEW — same Gary, eyes shifted forward, beginning of recognition, no smile). |
| **C3 RECOGNITION** | 8.4–12.6 | Mutual but asymmetrical | Jen enters frame naturally; over-Gary-shoulder / slightly offset. | **start = `PK-PS001-C3a`** (NEW — Jen entering, over-Gary-shoulder; **CCA-002 face — identity-critical**) → **end = HERO-03 `TL-0070_Egypt_FirstRecognition_v5`** (locked anchor; recognition in the eyes, not mouth-first). |

> **Anchors at the segment ends:** HERO-02 (`TL-0010_..._v3`) informs C1's close; HERO-03 (`TL-0070_..._v5`) is C3's end target. New PKs fill the in-betweens. **No Hero Anchor is regenerated; no story beat changes.**

## Render plan (per clip — after keyframes are approved)
Veo 3.1 standard, 16:9, 24 fps, first+last frame conditioning (or first-frame-only where a trailing camera must stay free, per the R1 camera lever); negative prompt = forbidden list (no smiling [C1/C2], no mouth-first smile [C3], no eyewear, no anachronisms, no glowing pendant, no text/watermark/border). Each clip = its own provenanced motion work order (`PS001R2-C1.md` / `-C2.md` / `-C3.md`) carrying request + result, scored by Gemini, EP-gated.

## Lifecycle / gate
`Performance Keyframes (Nano Banana) → Director/EP review of keyframes → Veo render per clip → Gemini GVR per clip → EP → editorial assembly to 12.6 s → EP LOCK`.
**Current step:** keyframes not yet generated. **Gate before any Veo render = keyframe approval** (identity is the prior failure; review the stills first).

## Status (2026-06-29)
Created from `PSD-001-R2`. Both R1 takes archived (`13_Production_History/Seq01_Egypt/`). **Next action: generate the Performance Keyframes (Nano Banana, CCA-conditioned), starting with Clip 1, for Director/EP review before any motion render.** Awaiting EP go to generate keyframes.
