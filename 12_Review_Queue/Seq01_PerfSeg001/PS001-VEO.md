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

### Render v3 — `PS001-VEO_cam.mp4` (camera fix — trailing witness) — 2026-06-29
- **Change vs v2 (single lever, the open camera flag):** **first-frame-only conditioning** (condition on HERO-02 only; **no HERO-03 last frame**) + camera prompt that explicitly enforces the PSD-001 *trailing witness several paces BEHIND Gary*, with frontal/facing/front-view added to negatives. Same standard model (`veo-3.1-generate-preview`), 16:9, 720p, 24 fps, 8.0 s, 1 video. Conditioning frame pulled from `14_Selected/Seq01/`.
- **Result — CAMERA DEVIATION RESOLVED.** Across the full clip the camera is a **trailing witness directly behind Gary** (start frame distant per HERO-02 → steady behind-the-back follow). No frontal approach, no static frontal two-shot, no orbit/push/zoom. This is the directed *witness behind* framing from PSD-001. Clean output, no watermark (API path).
- **Supervisor objective observations (measurable only — creative verdict is Gemini's/Director's):**
  - **Camera:** trailing-from-behind for the entire 8 s; Gary's back to camera throughout; Jen enters naturally far ahead on the path (~frame 4.5 s onward) and the two converge. ✅ matches direction.
  - **Identity (Gary):** never seen frontally (camera is behind), so a frontal CCA-001 match **cannot be confirmed from this take**; hair (dark, short, slight temple recession) is **consistent across the clip** — no v1-style age/hair jump.
  - **Identity (Jen):** distant; Scholar costume reads correct (pleated linen + turquoise/lapis collar); face too far to verify.
  - **Costume / pendant:** Gary's Architect linen consistent; pendant cord visible at the nape (front pendant not visible — back-of-subject framing). Period-accurate; no eyewear (CD-001); no anachronisms; no smiling visible; no glowing pendant.
  - **World indifferent:** boatman poling the Nile, birds, misty dawn cliffs — held throughout.
  - **⚠️ New objective tradeoff (inherent to the behind-camera fix):** because we never see Gary's face, the PSD-001 **"Gary changes first / eyes move first / shoulders soften"** facial recognition beat is **not legible** in this take — recognition now reads as two figures converging on the path rather than a readable change on Gary's face. Camera vs facial-performance tension for the Director to weigh; **`PS001-VEO_std.mp4` (v2) shows the face but not the camera; this take (v3) shows the camera but not the face.**
- **Disposition:** Review Queue — **two standard-tier candidates now exist** (v2 face-forward, v3 trailing-witness). Routed for Gemini blind GVR; EP to weigh the camera/face tradeoff. No further variants rendered pending review (Director's "don't re-roll endlessly" standard).
- **Lifecycle:** Rendered 2026-06-29 ✅ · Gemini GVR: pending · EP: pending.

## GEMINI GVR (blind, 2B motion scorecard) — first pass 2026-06-29 — ⚠️ SUPERSEDED by the RE-AUDIT below (mapping was cross-talked; corrected via FFmpeg frame extraction)
**Blind key set by Supervisor:** Clip A = `PS001-VEO_cam.mp4` (v3, trailing-witness camera, Gary's face not seen) · Clip B = `PS001-VEO_std.mp4` (v2, frontal two-shot, face + chest pendant visible).

**Gemini scores as received:**
- **Clip A — TOTAL 70/100** — Emotional 18/30 ("flatter… reaction to the camera rather than an internal epiphany"), Identity 20/25 (minor tunic-fabric drift), Camera 12/15 (one pan "announced"), Motion Continuity 9/15 (background boat jitter / "mechanical smoothing"), Prompt Fidelity 8/10, Technical 3/5 (shadow compression).
- **Clip B — TOTAL 93/100** — Emotional 27/30 ("organic and internal… recognition lands"), Identity 24/25 ("pendant perfectly tracked… no facial drift"), Camera 14/15 ("truly *witness* quality… human operator following the characters"), Motion Continuity 14/15, Prompt Fidelity 10/10 ("Gary changes first; Jen's reaction a perfect echo"), Technical 4/5.
- **Gemini verdict:** "Clip B is the superior candidate… acceptable as-is, no editorial combination required… promote Clip B to the locked registry; archive Clip A." No hard forbidden-list violations in either clip.

**⚠️ SUPERVISOR OBJECTIVE DISCREPANCY (why this is HELD, not locked):** Gemini's review does not match the footage on the dimension that mattered most for this re-render — **the camera.**
- Under the blind key, **Clip B = `PS001-VEO_std.mp4` is the FRONTAL two-shot** (verified by extracted frames at 0/2/4/6/7.5 s: camera comes in front of Gary, face visible, ends on a frontal two-shot). Gemini scored that clip's camera **14/15 "truly witness quality, operator following the characters"** — the opposite of what the frames show.
- Conversely **Clip A = `PS001-VEO_cam.mp4` is the genuine trailing-witness-behind** take (verified by frames), which Gemini scored **12/15** and called camera-reactive.
- Gemini's "Clip B" praise also **blends attributes of two different physical clips**: "operator *following* the characters" (a trailing/CAM trait) with "Gary changes first / Jen echoes / pendant perfectly tracked" (readable faces + a chest pendant = the FRONTAL/STD clip). No single file has both.
- Gemini also reported **Clip B identity 24/25 "no facial drift,"** but the std end-frames show a **Jen who reads younger/fuller than CCA-002** (objective identity flag the review did not catch).

**Likely causes (to resolve before any promotion):** (a) the A/B→file order Gemini actually reviewed differs from the Supervisor key, and/or (b) Gemini scored from the work-order *text*/URLs without reliably viewing each specific `.mp4`. Either way, the **scores cannot be attached to a specific take with confidence**, so no LOCK is recorded.
- **Disposition:** **HELD — Review Queue.** Required next: confirm the exact A/B→filename mapping Gemini reviewed and re-run the camera scoring against the actual footage (Supervisor can pre-label the two files and have the EP upload them in that fixed order). The *editorial* question (camera-vs-face → possibly a multi-shot answer) remains Sam's; it is not foreclosed by this review.
- **Lifecycle:** Rendered 2026-06-29 ✅ · Gemini GVR received 2026-06-29 (⚠️ held — discrepancy) · EP: pending · LOCK: NOT recorded.

## GEMINI GVR RE-AUDIT (corrected mapping, hard-filtered to on-screen pixels) — 2026-06-29 — RESOLVED ✅
**Mapping confirmed:** Gemini's re-audit identifies `PS001-VEO_cam.mp4` as the trailing-witness take and `PS001-VEO_std.mp4` as the frontal two-shot with late Jen drift — **matching the Supervisor's FFmpeg frame extraction exactly.** The first-pass cross-talk is corrected. Verbatim re-audit (per VFX directive):

> **AUDIT-CLIP-A (`PS001-VEO_cam.mp4` — Trailing Witness):** Emotional 22/30 ("powerful internal restraint… withholding the faces, the physical posture carries the weight"), Identity 19/25 (build + linen weave match HERO-02 from the reverse angle), Camera 13/15 ("truly a trailing witness… never anticipates or forces"), Motion Continuity 11/15 (stable spatial physics), Prompt Fidelity 8/10, Technical 4/5. **TOTAL 77/100.**
> **AUDIT-CLIP-B (`PS001-VEO_std.mp4` — Frontal Two-Shot):** Emotional 16/30 ("undermined by the incorrect framing"), Identity 14/25 ("Jen's face drifts… reading younger, breaking CCA-002"), Camera **5/15 CRITICAL FAIL** ("forces an unearned frontal studio structure"), Motion Continuity 11/15, Prompt Fidelity 3/10 (fails PSD-001 staging), Technical 4/5. **TOTAL 53/100.**
> **Three-question:** Q1 — A sound; B disqualified (Jen drift). Q2 — A honors isolation/restraint; B trades the cinematic language for a generic frontal shot. Q3 — reject any generation that drops the observational witness perspective; log AUDIT-CLIP-A's parameters to anchor future reverse-angle shots.
> **Verdict:** AUDIT-CLIP-A (Trailing Witness) is the definitive winner; approved as-is for the trailing segment. AUDIT-CLIP-B committed a structural violation (broke the observational camera mandate) — rejected.

**Standard established (Director ruling, 2026-06-29 — record the *standard*, not the score):** this take sets the **WITNESS CAMERA STANDARD** — the observational, trailing-from-behind, "operator following the characters" camera is the studio's proven cinematic baseline; future productions begin there. Companion philosophy: **"if one honest take captures the performance, keep it — do not improve it into dishonesty."**

**DISPOSITIONS:**
- **`PS001-VEO_cam.mp4` (AUDIT-CLIP-A) = WINNER.** VFX-approved; Director-ruled promote. **Routed to Sam (Director) for formal layout integration.** *(Open creative question for Sam: the witness take never shows Gary's face, so the "Gary changes first" facial beat is not literally visible — Sam confirms whether one take stands or the layout needs a second angle. EP LOCK to `14_Selected/` pending.)*
- **`PS001-VEO_std.mp4` (AUDIT-CLIP-B) = REJECTED** (camera mandate violation + Jen CCA-002 drift). Archived to `13_Production_History/Seq01_Egypt/Camera_Motion/` (kept as provenance, never deleted).
- **`PS001-VEO.mp4` (v1, Fast tier)** — prior provenance (demonstrates why standard tier is used).
- **Lifecycle:** Rendered 2026-06-29 ✅ · Gemini GVR re-audit 2026-06-29 ✅ RESOLVED · winner → Sam (layout) · EP LOCK: pending.

> *Provenance rule:* this file is the canonical record of the Veo attempt — request preserved verbatim, result appended; never deleted. Mirrors the still workflow exactly.
