# ASSET DOSSIER — TL-Seq1_Egypt_Jen_hero_v1  (ARCHIVED — environment drift)

> The Dossier for `TL-Seq1_Egypt_Jen_hero_v1.png`. Standard: `00_Production\20_REFERENCE\Creative_Provenance_Standard.md`. Kept, not deleted.

## Intent / Narrative Purpose
- (Intended: Jen as a real woman on a quiet morning road, faint recognition.) The render FAILED this Intent — it drifted into temple spectacle, contradicting "no spectacle." Intent vs failure is why it is kept.

## Director Notes  (Director-authored — reminders to future reviewers)
- (none — asset archived)

## Identity
- Asset ID: TL-Seq1_Egypt_Jen_hero_v1
- Created: 2026-06-26
- Sequence: Sequence One
- Chapter / Scene: Egypt (Jen approaching, first light)
- Shot: TL-0070..0080 area (Jen hero)
- Creator: Claude Code (Supervisor)
- Generator: Nano Banana
- Model / Version: Gemini 3 Pro Image (gemini-3-pro-image-preview)

## References used (conditioning)
- Master refs: Jen_Master_01_Front, Jen_Master_02_Profile, Jen_Master_03_Proportions

## Prompt (recorded form — see note)
```
A woman in her late 30s, warm genuine face, bright expressive eyes (match references),
walks gently toward camera at first light... noblewoman/temple scholar in fine linen,
small silver pendant... calm and open, faint beginning of recognition... 85mm, shallow
DOF, film grain, warm-gold grade.
```
> NOTE: generated before this provenance standard; verbatim string not preserved. Recorded form from the VFX-001 report. The phrase "temple scholar" with no environment constraint is implicated in the root cause below.

## Negative Prompt
```
(not recorded by the prior session — and critically, no "no temple/spectacle" suppression)
```

## Generation parameters
- Aspect ratio: 16:9
- Resolution: 2k (~2752x1536)
- Grounding: on   - Thinking level: high
- Output file: TL-Seq1_Egypt_Jen_hero_v1.png

## Lifecycle
- Created: 2026-06-26
- Reviewed: 2026-06-26
- Disposition set: 2026-06-26 (Archived -> Production_History)

## Disposition
- Status: Archived (Production_History)
- Current location: 04_Egypt\Stills\Production_History\Environment\

## Evolutionary tree (lineage)
- Parent: original  ·  Children: TL-Seq1_Egypt_Jen_hero_v2  ·  Siblings: Jen_hero_v2
- Superseded By: TL-Seq1_Egypt_Jen_hero_v2 (the change: explicit quiet-Nile-path + temple/spectacle negatives)

## Review (three questions)
- Q1 Technical (render matches prompt?): YES — faithful to an under-constrained prompt (no environment limits).
- Q2 Creative (prompt implements Intent?): NO — drifted into temple spectacle vs the quiet-path Intent.
- Q3 Institutional (reuse this approach?): NO — see lesson.

## Living fields
- Creative Discovery: none recorded.
- Studio Standard: Deprecated (archived; the LESSON is the durable standard).
- Knowledge Reused In: none yet — "constrain the environment positively AND negatively in historical chapters" applies to every historical sequence.

## THE LESSON
- Primary Category: Environment
- Secondary Categories: Creative Direction
- Severity: Major  (the frame contradicts the Director's stated intent)
- Preventable?: YES
- Reason for Archive: Drifted into a grand Karnak-style temple with towering columns, palms and background figures — the "spectacle" CRE-001 explicitly forbids ("No pyramids dominating the frame... an ancient civilization breathing").
- Root Cause: The prompt described the character but left the environment under-constrained ("temple scholar"); the model defaulted to a monumental temple. No negative suppression of temple/columns/spectacle.
- Continuity Decision: n/a (creative-direction drift, not a continuity rule).
- Corrective Action: v2 added an explicit quiet-Nile-dawn-path description PLUS negatives (grand temple, Karnak, columns, crowds, spectacle, monuments). Standing lesson: state the environment positively AND negatively for historical chapters.
- Creative Impact: A monument competes with the human moment; the quiet path keeps Jen a person on a morning road — the point of the scene.
- Pipeline Impact: Reinforced "describe environment per shot, suppress spectacle" in the Prompt Package build rules.
- Lessons Learned: Character-only prompts let the model invent the world; constrain the world explicitly in historical chapters.
- Would We Generate This Again?: Yes as a teaching example of environment drift; no for the cut.
