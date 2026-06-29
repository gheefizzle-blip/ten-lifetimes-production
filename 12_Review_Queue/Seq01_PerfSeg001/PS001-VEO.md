# MOTION WORK ORDER + DOSSIER — PS001-VEO
### Performance Segment 001 · Engine: Google Veo · (Blind label assigned at scoring)

> **Self-contained motion work order** — Veo can read THIS file alone and render. Carries **both the request and the result** (same provenance discipline as a still's Dossier: *no Dossier = the asset does not exist*). Born 2026-06-28 with the request; the result section is filled when the clip returns.

## Identity
- **Asset ID:** PS001-VEO · **Type:** Motion Clip (Performance Segment) · **Engine:** Google Veo (image→video)
- **Work order:** PVP-001 · Phase 2B Renderer Qualification · **Segment:** Performance Segment 001
- **Span:** HERO-02 "The Long Road" → HERO-03 "The First Recognition" · ~12.6 s · 16:9 · 24 fps
- **Source direction (verbatim, do not reinterpret):** `PSD-001_Performance_Segment_Direction_OpeningMovement.md`
- **Shot spec:** `Performance_Segment_001_Shot_List.md` · **Parents:** HERO-02 (TL-0010), HERO-03 (TL-0070)

## Conditioning frames (image→video)
- **First frame = HERO-02:** `raw.githubusercontent.com/gheefizzle-blip/ten-lifetimes-production/main/14_Selected/Seq01/TL-0010_Egypt_TheLongRoad_v3.png`
- **Last frame = HERO-03:** `raw.githubusercontent.com/gheefizzle-blip/ten-lifetimes-production/main/14_Selected/Seq01/TL-0070_Egypt_FirstRecognition_v5.png`
- First+last keyframes where supported; else condition on HERO-02 and direct motion to *arrive* at the HERO-03 pose.

## Cinematic philosophy (identical for all engines)
The camera is a **witness**, never a participant — never rushes, predicts, or announces. *If the audience notices the camera, the shot failed.* Motion must feel **photographed, not generated** (human-operator imperfection welcome). Silence is the dominant language. **Gary changes first, Jen follows — mandatory.** Success = the viewer thinks *"I don't know why… but something important just happened."*

## THE REQUEST — Veo structured prompt (one entry per shot, render in sequence)

**Shot 1 — Observe (6.3s)**
- **Subject:** A New Kingdom Egyptian man in fine pleated linen (Royal Architect), silver pendant at the collar.
- **Action:** Walks naturally along a Nile-side path at dawn; shoulders slightly lowered, eyes forward; expression peaceful but emotionally empty, accustomed to solitude.
- **Scene:** Early morning, ancient Egypt; morning workers, flowing river, birds — all continuing independently, indifferent to him.
- **Camera:** Slow trailing dolly, several paces behind, eye-level, gentle forward travel matched to his pace. No orbit, no push, no drama.
- **Lighting/Mood:** Soft natural dawn light; observational; routine.
- **Negative:** smiling, eye contact, push-in, zoom, slow-motion, VFX, glowing pendant, glasses, identity drift, costume drift, anachronisms, orbit/whip/crane, text/watermark/border.

**Shot 2 — Transition (3.5s)**
- **Subject:** Same man, identical identity and costume.
- **Action:** Rhythm changes by almost nothing — one slightly shorter step, one slower breath; he does not know why. Silver pendant catches one brief, natural light reflection (not magical).
- **Scene:** Unchanged; workers, water, birds continue; history unaware.
- **Camera:** Continue the same trailing move; almost imperceptibly reduce forward speed; camera lags slightly behind; time subtly stretches.
- **Lighting/Mood:** Same dawn light; intuition that something is different, with no explanation.
- **Negative:** (same as Shot 1.)

**Shot 3 — Reveal (2.64s)**
- **Subject:** Same man; a New Kingdom Egyptian woman in pleated linen and lapis collar (Royal Scholar), matching her conditioning frame.
- **Action:** Woman enters frame naturally. Man stops a touch early; his eyes move first, body follows; shoulders soften; breath pauses. Woman notices him — only familiarity, expression almost neutral. Man changes first, woman follows.
- **Scene:** Same Nile morning.
- **Camera:** Observational; no push-in, no whip, no dramatic reveal; let her enter naturally.
- **Lighting/Mood:** Quiet; the felt sense that something impossible just happened.
- **Negative:** (same as Shot 1) + no recognition smile, no exaggerated reaction.

## Locked constraints (every shot)
Gary = CCA-001, Jen = CCA-002 (no drift) · costumes Architect/Scholar (no drift) · silver pendant present, subtle/natural · period-accurate, no anachronisms · no eyewear (CD-001) · timing immutable.

---

## THE RESULT  (filled when the clip returns — keeps request+result together)
- **Returned clip:** `PS001-VEO.mp4` *(pending)*
- **Render settings actually used (model/version, frames, fps, resolution, seed):** *(pending)*
- **Blind label at scoring:** *(assigned A/B at GVR)*
- **Gemini GVR (blind, 2B scorecard):** Emotional /30 · Identity /25 · Camera /15 · Motion Continuity /15 · Prompt Fidelity /10 · Technical /5 → **Total /100** *(pending)*
- **Objective observations:** *(pending — identity hold, camera fidelity to PSD-001, artifacts, timing)*
- **Disposition:** *(pending — Selected motion / Production_History)*

## Lifecycle / Review
- Created: 2026-06-28 (request) · Rendered: pending · Reviewed (Gemini GVR-###): pending · EP: pending · Disposition: pending
- Three-question review (Q1 Technical / Q2 Creative-vs-PSD-001 / Q3 Institutional): pending

> *Provenance rule:* this file is the canonical record of the Veo attempt — request preserved verbatim, result appended; never deleted. Mirrors the still workflow exactly.
