# ASSET DOSSIER — TL-0001_Cosmos_BeforeTime_v1  (ARCHIVED — rendering artifact)

> The Dossier for `TL-0001_Cosmos_BeforeTime_v1.png`. Standard: `00_Production\20_REFERENCE\Creative_Provenance_Standard.md`. Work order: **CRE-002 HERO 01**. Kept, not deleted.

## Intent / Narrative Purpose
- **HERO 01 "Before Time" (Director, CRE-002).** The audience enters silence; no history, no civilizations; only the possibility that two souls have always existed. Subtle, almost motionless; lower the heartbeat. No sci-fi/galaxies/fantasy. (This render achieved the MOOD but failed technically — see lesson.)

## Director Notes  (Director-authored — reminders to future reviewers)
- (none — asset archived)

## Identity
- Asset ID: TL-0001  (HERO 01, "Before Time", Cosmos / S0)
- Object type: Still
- Created: 2026-06-26
- Sequence / Chapter / Scene: Sequence One / Cosmos / opening
- Shot: TL-0001
- Creator: Claude Code (Supervisor)
- Generator: Nano Banana  ·  Model / Version: Gemini 3 Pro Image (gemini-3-pro-image-preview)

## References used (conditioning)
- Master refs: none  ·  Other-character refs: none

## Prompt (verbatim)
```
The very first frame of a contemplative feature film, before history begins. A vast, silent, primordial pre-dawn — an immense calm darkness. A deep indigo-to-black night sky holds a faint, delicate scattering of soft emerging stars, as if points of light are only just becoming visible — not a busy starfield, not a galaxy, no nebula. Below, mirror-still dark water (or low ground-mist) stretches to an unseen horizon, perfectly motionless, faintly reflecting the dim sky. At the very lowest edge of the sky the faintest warm-gold glow is only beginning to appear inside the darkness — not a sunrise, only the first possibility of light. No land features, no structures, no civilization, no people — only timeless stillness and space. The mood is hushed, patient, meditative; an image that lowers the viewer's heartbeat. Cinematic anamorphic widescreen, deep natural blacks, extremely subtle and restrained, photorealistic, fine 35mm film grain, naturalistic muted color. Looks like a real frame from a quiet, meditative feature film — emphatically NOT science fiction.
```

## Negative Prompt (verbatim)
```
science fiction, sci-fi, outer space, galaxy, nebula, milky way, exploding stars, supernova, planets, moon, spaceship, dramatic aurora, fantasy, magic, glowing particles, busy starfield, lens flare, sun rays beams, people, figures, silhouettes, buildings, architecture, boats, animals, text, watermark, oversaturated, HDR, neon, cartoon, illustration, CGI look, plastic
```
> Note: the negative prompt did NOT suppress border/frame/matte. That omission is the root cause below.

## Generation parameters
- Aspect ratio: 16:9  ·  Resolution: 4k (5504x3072)  ·  Grounding: OFF  ·  Thinking: high
- Output file: TL-0001_Cosmos_BeforeTime_v1.png

## Evolutionary tree (lineage)
- Parent: original  ·  Children: TL-0001_Cosmos_BeforeTime_v2  ·  Siblings: v2
- Superseded By: v2 (technical fix)

## Lifecycle
- Created: 2026-06-26  ·  Reviewed: 2026-06-26 (Supervisor caught the artifact)  ·  Disposition set: 2026-06-26 (Archived)

## Disposition
- Status: Archived (Production_History)
- Current location: 00_Cosmos\Stills\Production_History\Rendering_Artifact\

## Review (three questions)
- Q1 Technical (render matches prompt?): NO — rendered as a bordered/matted inset instead of a full-bleed frame.
- Q2 Creative (prompt implements Intent?): YES on mood (quiet, motionless, lowers heartbeat) — but unusable due to Q1.
- Q3 Institutional (reuse this approach?): NO for the asset; YES for the lesson.

## Living fields
- Creative Discovery: none recorded.
- Studio Standard: Deprecated (archived; the LESSON is the durable standard).
- Knowledge Reused In: none yet — "always negative-prompt border/frame/matte/rounded-corners for full-bleed film frames" applies to EVERY still generation.

## THE LESSON
- Primary Category: Rendering Artifact
- Secondary Categories: Composition
- Severity: Minor  (mood intact; purely a framing defect, cheaply fixed)
- Preventable?: YES
- Reason for Archive: The render came out with a rounded-corner black border / matte framing the scene instead of a full-bleed 16:9 cinematic frame.
- Root Cause: The phrase "the very first frame of a film" plus no border suppression nudged the model toward depicting a framed photograph/inset rather than the scene filling the canvas.
- Corrective Action: v2 added `border, black border, picture frame, rounded corners, vignette frame, matte, inset image, letterbox bars` to the negative prompt and "full-bleed edge to edge" to the positive prompt. Clean full-frame result.
- Creative Impact: None to the story; the mood was right. Purely a deliverability fix.
- Pipeline Impact: New standing prompt rule — carry border/frame/matte negatives on all stills.
- Lessons Learned: Phrasings like "first frame of a film" can invoke a literal frame border; suppress it explicitly.
- Would We Generate This Again?: No for the asset; yes as the worked example behind the border-suppression rule.
