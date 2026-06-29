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
- **Returned clip:** ✅ `PS001-VEO.mp4` (rendered 2026-06-29 via the programmatic Veo bridge — Gemini API, no manual upload; pulled HERO-02/HERO-03 from `14_Selected/`).
- **Render settings actually used:** model **`veo-3.1-fast-generate-preview`** (Gemini API) · **first frame = HERO-02, last frame = HERO-03** · negative prompt = forbidden list · aspect 16:9 · **1280×720 (720p), 24 fps, 8.0 s (192 frames)** · 1 video · no reference images this pass · enhance_prompt off · seed unset · Veo-generated AAC audio present (to be muted/replaced — music is master). *(Note: 8 s is Veo's native clip length; the full 12.6 s assembles in editorial 2C.)*
- **Blind label at scoring:** *(assigned at GVR)*
- **Gemini GVR (blind, 2B scorecard):** **pending** — routed for blind review.
- **Supervisor objective observations (measurable only — judgment is Gemini's/Director's):**
  - Start frame faithful to HERO-02 (distant figure, Nile dawn, boatman, birds, indifferent world).
  - **Identity drift on Gary across the clip:** mid-frame (long-haired, lean — strong CCA-001 match) vs end-frame (older, balding, grayer) — not consistent end-to-end. ⚠️
  - **Jen (end frame):** Scholar costume correct (lapis collar, braided wig, headband) but silhouette/body reads fuller/different than CCA-002 — possible drift. ⚠️
  - **Camera deviated from PSD-001:** directed as a *trailing witness behind* Gary; Veo rendered a *frontal approach* → *static two-shot* instead. ⚠️
  - Held: costumes, **silver pendant visible**, period accuracy, no eyewear (CD-001), indifferent world (workers washing linen), recognition two-shot composition.
- **Disposition:** Review Queue — pending Gemini blind GVR + EP. *(First clip of the 2B benchmark; needs a Grok clip for the A/B, or score solo as a first data point — EP's call.)*

## Lifecycle / Review
- Created: 2026-06-28 (request) · **Rendered: 2026-06-29 ✅** · Reviewed (Gemini GVR-###): pending · EP: pending · Disposition: Review Queue
- Three-question review (Q1 Technical / Q2 Creative-vs-PSD-001 / Q3 Institutional): pending Gemini

> **Pipeline proof:** this is the first asset produced by the programmatic Veo bridge (repo → Veo first+last frame → download → commit). No manual upload; conditioned on the exact locked anchors. The bridge works end-to-end.

### Render v2 — `PS001-VEO_std.mp4` (standard tier — PREFERRED) — 2026-06-29
- **Change vs v1:** model only, **`veo-3.1-fast` → `veo-3.1-generate-preview` (standard)**. Same first+last frame, same prompt/negative, 16:9, 720p, 24 fps, 8.0 s. Controlled single-variable test.
- **Result:** ✅ **Identity drift RESOLVED.** Gary is now consistent across the whole clip (mid-frame matches end-frame — no more long-haired-younger-Gary jump); reaches the recognition two-shot; **clean, no watermark** (the manual Gemini-app clip carries a baked-in ✦ watermark — disqualifying for final; the API output does not).
- **Finding (canon):** the v1 drift was caused by the **Fast tier**, not the programmatic/API path. **Standard Veo 3.1 is the preferred motion setting.** v1 (Fast) kept as provenance — it demonstrates *why* we use standard.
- **Remaining objective flag:** camera still reads frontal→two-shot rather than the directed *trailing witness* (PSD-001). Next lever = first-frame-only conditioning or stronger camera prompt. Identity + recognition + clean output now solid.
- **Comparison clip (manual, app):** `MOTION_WORK_ORDER_DOSSIER.mp4` (EP-generated, 10 s) — held camera/identity well **but watermarked + manual**; retained as a comparison data point, not a canon deliverable.

> *Provenance rule:* this file is the canonical record of the Veo attempt — request preserved verbatim, result appended; never deleted. Mirrors the still workflow exactly.
