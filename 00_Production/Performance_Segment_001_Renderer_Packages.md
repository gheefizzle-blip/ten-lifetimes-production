# PERFORMANCE SEGMENT 001 — Renderer Packages (Sora · Veo · Grok)
### Translation of PSD-001 · HERO-02 "The Long Road" → HERO-03 "The First Recognition"

> **Faithful translation of `PSD-001` (Director Sam).** Per the Director's order: the emotional direction, camera language, timing, and performance are **identical** across all three packages; only prompt **syntax/format** differs per engine. Nothing optimized, nothing reinterpreted. The blind benchmark (Gemini, PVP-001 2B) depends on this — so **§0 Common Direction is the single source of truth; Packages A/B/C are the same content in each engine's idiom.**

---

## 0. COMMON DIRECTION (authoritative — identical for all engines)

**Conditioning frames (image-to-video):**
- **Opening frame = HERO-02 "The Long Road":** `raw.githubusercontent.com/gheefizzle-blip/ten-lifetimes-production/main/14_Selected/Seq01/TL-0010_Egypt_TheLongRoad_v3.png`
- **Closing frame = HERO-03 "The First Recognition":** `raw.githubusercontent.com/gheefizzle-blip/ten-lifetimes-production/main/14_Selected/Seq01/TL-0070_Egypt_FirstRecognition_v5.png`
- Use **start + end keyframes** where the engine supports it (begin on HERO-02, arrive on HERO-03). Where only a start frame is supported, condition on HERO-02 and direct the motion to *arrive* at the recognition pose.

**Global spec:** 16:9 · ~12.6 s total (Shot 1 = 6.30 s · Shot 2 = 3.50 s · Shot 3 = 2.64 s) · 24 fps · photographic realism · ancient Egypt, New Kingdom, early morning by the Nile · natural light · no on-screen audio needed (music is the master).

**Cinematic philosophy:** the camera is a **witness**, never a participant — it never rushes, predicts, or announces. *If the audience notices the camera, the shot has failed.* Motion must feel **photographed, not generated** — the tiny imperfections of a human operator walking beside another human. Silence is the dominant language.

**Locked identity/continuity:** Gary = CCA-001, Jen = CCA-002 (no drift) · costumes: Gary Royal Architect, Jen Royal Scholar (no drift) · silver pendant present, subtle and natural · period-accurate, no anachronisms.

**The three shots:**
| # | Time | Purpose | Camera | Performance / World |
|---|---|---|---|---|
| 1 | 29.62–35.92 (6.30s) | **Observe** | Slow trailing dolly, several paces behind Gary, eye-level; gentle forward travel matching his walking speed; no orbit/push/drama. | Gary walks naturally, shoulders slightly lowered, eyes forward; peaceful but emotionally empty (not sad — accustomed to solitude). Workers, Nile, birds continue; nothing acknowledges him; the world is indifferent. |
| 2 | 36.08–39.58 (3.50s) | **Transition** | Continue the same trailing move; almost imperceptibly reduce forward speed; camera begins to lag slightly behind him; time subtly stretches. | Gary's rhythm changes by almost nothing — one slightly shorter step, one slower breath; he doesn't know why. The pendant catches one brief, natural reflection (not magical). Environment unchanged; history unaware. |
| 3 | 39.58–42.22 (2.64s) | **Reveal** | Remain observational — no push-in, no whip, no dramatic reveal; let Jen enter frame naturally; Gary stops a touch before the audience expects. | Gary's eyes move first, body follows; shoulders soften; breathing pauses; no language for the feeling. Jen notices Gary — only familiarity, recognition not yet conscious; her expression almost neutral. **Gary changes first, Jen follows — mandatory.** |

**FORBIDDEN (applies to every shot — hard negatives):** no smiling · no dramatic eye contact · no cinematic push/zoom · no slow-motion · no magical visual effects · no glowing pendant · no exaggerated reactions · no audience manipulation · no eyewear/glasses · no identity or costume drift · no modern objects/anachronisms · no orbit/whip/crane moves · no text, captions, watermark, logo, border, or letterbox.

**Success criterion:** the viewer should finish thinking *"I don't know why… but something important just happened."* Feeling, not spectacle.

---

## Package A — SORA (cinematic prose)

> Condition on the opening frame (HERO-02); target the closing frame (HERO-03). Render as three continuous shots. Style: observational documentary realism, ancient Egypt at dawn, natural light, handheld-subtle. Negatives at the end.

**Shot 1 (0–6.3s) — Observe.** A man in fine pleated Egyptian linen walks a dirt path beside the Nile at early morning. The camera is a quiet witness several paces behind him at eye level, dollying gently forward at exactly his walking pace — no orbit, no push, no flourish. His shoulders are slightly lowered, eyes forward; his face is peaceful but emotionally empty — not sad, simply a man long accustomed to solitude. Around him, morning workers go about their tasks, the river flows, birds move on their own; nothing acknowledges him. The world is indifferent. The mood is pure routine.

**Shot 2 (6.3–9.8s) — Transition.** The camera continues the same trailing move but its forward speed eases almost imperceptibly, beginning to lag a half-step behind him, so time seems faintly to stretch. The man's rhythm changes by almost nothing — one slightly shorter step, one slower breath; he does not understand why. His silver pendant catches a single brief, natural glint of morning light — ordinary, not magical. The workers, the water, the birds continue unchanged. Something feels different, with no explanation — only intuition.

**Shot 3 (9.8–12.6s) — Reveal.** The camera stays observational — no push-in, no whip, no dramatic reveal. A woman in pleated linen and a lapis collar enters the frame naturally. The man stops a moment before we expect him to. His eyes move first, then his body follows; his shoulders soften and his breath pauses — he has no language for what he feels. She notices him — only familiarity, recognition not yet conscious — her expression almost neutral. He changes first; she only begins to follow. Hold on the quiet impossibility of it.

**Identity/continuity:** the man and woman must exactly match the two conditioning frames (same faces, ages, costumes, the silver pendant). Photographed, not generated; human imperfection welcome.
**Negative:** smiling, dramatic eye contact, push-in/zoom, slow-motion, VFX, glowing pendant, exaggerated reactions, glasses/eyewear, identity drift, costume drift, modern objects, orbit/whip/crane, text/caption/watermark/border/letterbox.

---

## Package B — VEO (structured fields)

> First frame = HERO-02; last frame = HERO-03 (if last-frame supported). One entry per shot; render in sequence. Veo-style structured prompt + negative_prompt.

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

---

## Package C — GROK (directive natural language)

> Condition on HERO-02 (start) and arrive at HERO-03 (end). Three shots, rendered in order. Explicit DO / NEVER per shot. Faithful to PSD-001 — execute, do not reinterpret.

**Shot 1 — Observe · 6.3s.**
DO: Photograph a man in fine pleated Egyptian linen walking a Nile path at dawn. Place the camera as a silent witness several paces behind him, eye-level, dollying forward at exactly his pace. Keep his expression peaceful but emotionally empty — not sad, just used to being alone. Let the world (workers, river, birds) continue indifferently around him.
NEVER: orbit, push in, zoom, add drama, or let anything acknowledge him. No smiling.

**Shot 2 — Transition · 3.5s.**
DO: Keep the same trailing move but ease the forward speed almost imperceptibly so the camera lags slightly and time feels stretched. Let his rhythm change by almost nothing — one shorter step, one slower breath; he doesn't know why. Allow the silver pendant a single brief, natural glint of light.
NEVER: make the pendant glow or magical; change the environment; explain the shift; exaggerate anything.

**Shot 3 — Reveal · 2.64s.**
DO: Stay observational and let a woman in pleated linen and lapis collar enter the frame naturally. Have the man stop a moment before expected; his eyes move first, then his body; shoulders soften; breath pauses. Let the woman simply notice him — familiarity only, expression almost neutral. The man changes first; the woman only begins to follow.
NEVER: push in, whip, or stage a dramatic reveal; no smile; no recognition "moment" played to camera; no exaggerated reaction.

**All shots — identity & feel:** match the two conditioning frames exactly (faces, ages, costumes, pendant). Motion must look photographed, not generated; small human imperfections are good. Forbidden globally: glasses, identity/costume drift, slow-motion, VFX, modern objects, text/watermark/border/letterbox, audience manipulation.

---

## Issue & review
- **Renderer:** EP runs each package on its engine's web interface (no MCP bridge). Same conditioning frames; same three shots; same timing.
- **Provenance:** each returned clip + objective notes is committed by the Supervisor with a Dossier (PVP-001 2B); resolution is ≤5% of the score.
- **Scoring:** **Gemini, blind** (engines labeled A/B/C) — Emotional Performance 30 · Identity 25 · Camera Language 15 · Motion Continuity 15 · Prompt Fidelity 10 · Technical 5.
- **Then:** EP reviews; the studio assigns motion role(s) by demonstrated strength.

> *Status:* packages translated from PSD-001, identical-except-syntax. **Ready for the EP to render on Sora, Veo, and Grok.**
