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

## Performance Keyframes — GENERATED 2026-06-30 (pending Director/EP review)
All five generated via Nano Banana (`nb2`, 16:9, multi-image conditioning on the **locked CCA v2 face sheets + approved costumes + HERO anchors**). In `12_Review_Queue/Seq01_PerfSeg001/Keyframes/` (raw URL base: `raw.githubusercontent.com/gheefizzle-blip/ten-lifetimes-production/main/12_Review_Queue/Seq01_PerfSeg001/Keyframes/`). NAS master: `04_Egypt/Motion/PerfSeg001/Keyframes/`.

| Keyframe | Conditioning | Supervisor objective notes (reviewers decide) |
|---|---|---|
| `PK-PS001-C1a.png` | HERO-02 + Gary costume | Elevated wide; lone figure on the reed-lined path, river, birds, boatman, hazy desert hills. Isolation/scale reads. Rear/distant — no face. |
| `PK-PS001-C1b.png` | HERO-02 + Gary costume | ~2 m behind Gary; back of head, pendant cord at nape, woven tool-belt, river ahead. Rear — no face. |
| `PK-PS001-C2a.png` | **CCA-001 v2** + Gary costume + HERO-02 | Front/off-axis Gary, routine, looking off; pendant at chest. ⚠️ **beard reads fuller/darker & face rounder than CCA-001** (which has a lean face + grey goatee) — possible identity drift; flag for review. |
| `PK-PS001-C2b.png` | **CCA-001 v2** + Gary costume + HERO-02 | Front Gary, eyes shifted forward, no smile. **Closer CCA-001 match** (grey-flecked beard, leaner). |
| `PK-PS001-C3a.png` | **CCA-002 v2** + Jen costume v2 + HERO-03 | Over-Gary-shoulder; Jen entering, costume correct (braided wig, lapis/turquoise collar); eyes-first, no full smile. Face plausibly consistent w/ CCA-002 — verify at full res. |

> **GATE:** review these stills (identity especially — it was the R1 failure) **before** any Veo render. If C2a's identity reads off, I re-gen it (cheap) before motion. C3 end target remains the locked HERO-03 (`TL-0070_v5`).

## CONTINUITY-ANCHOR finding (2026-06-30) — EP flags (costume back · pendant · shoreline)
EP flagged three continuity drifts across the keyframes — **all one root cause: any detail not pinned by a canonical reference image drifts, because the model invents it differently each render.**
1. **Costume back:** C1a/C1b = pleated tunic back; original C3a = invented **deep-V back**. (Costume Master defines only the FRONT.)
2. **Pendant:** the silver pendant design changes frame to frame. **No canonical pendant reference exists** (not on the costume sheet, none in `18_Motifs`). EP: the costume sheet should specify the pendant.
3. **Shoreline:** the Nile bank should be a consistent **sandy reed shoreline** throughout — not muddy in one frame. **No canonical environment reference plate exists** (only `Sequence_One_Environment_Direction.md`, a text doc).

**Tooling lesson (important):** `nb2` conditioned-generation will NOT correct a drifting detail via negatives or by adding a reference image — it reproduces the same composition. `nb2` **EDIT mode** can repaint a detail (it fixed the C3a back), but it alters framing. **The durable fix is canonical REFERENCE IMAGES** the keyframes condition on — same principle that fixed identity (CCA sheets).

**THE FIX (proposed — stop re-rolling; lock the anchors, then derive once):** before re-deriving the 5 keyframes, build the missing canonical anchors so every frame inherits identical detail:
- ✅ `Gary_Costume_Egypt_BACK_ref.png` — created (plain pleated back, round neck, sash). Propose → Costume Master.
- 🆕 **Canonical Pendant reference** — lock the exact silver-pendant design (shape/material/cord/size); add to Costume Master / `18_Motifs`. The recognition motif ("pendant catches light first") demands a fixed design.
- 🆕 **Canonical Environment reference** (Opening Movement) — a locked "Nile riverbank at dawn, sandy reed shoreline" plate (first Canonical Environment Asset) so all three clips share one shoreline/lighting.
- Then re-derive C1a/C1b/C2a/C2b/C3a conditioning on the FULL set (CCA face + costume + back-ref + pendant + environment) → consistent identity, costume, back, pendant, and shoreline.

> Status: paused keyframe re-derivation pending these anchors + EP/Director alignment. `Gary_Costume_Egypt_BACK_ref.png` preserved; C3a back-fix candidate (`edit` mode) retained on NAS/local as provenance of the tooling finding.

## Status (2026-06-30) — KEYFRAMES RE-DERIVED FROM TURNAROUNDS ✅
All 5 keyframes regenerated conditioned on the locked **character turnarounds** (Gary w/ snail, slimmer Jen) + **HERO-02 as the shared environment anchor**. Result: consistent identity, costume, plain pleated back, **silver snail** (C2b shows the dawn ray catching the snail — the motif beat), **slimmer Jen** (C3a), and **one consistent sandy reed shoreline across all three clips** (the earlier drift — costume back, pendant, muddy shoreline — is resolved). Turnaround-as-conditioning-source validated end to end.
- C1a elevated isolation · C1b 2 m trailing · C2a front routine · C2b pendant-catches-light + eyes shift (no smile) · C3a Jen enters over-Gary-shoulder (eyes-first, no smile).
- **NEXT: Veo render the three 4.2 s clips** (C1: C1a→C1b · C2: C2a→C2b · C3: C3a→HERO-03) via the Continuum Render Bridge → Gemini GVR per clip → editorial assembly to 12.6 s → EP lock. **Awaiting EP go to render.**
