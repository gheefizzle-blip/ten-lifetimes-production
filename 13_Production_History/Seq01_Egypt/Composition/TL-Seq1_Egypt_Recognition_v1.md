# ASSET PROVENANCE — TL-Seq1_Egypt_Recognition_v1  (ARCHIVED — staging/eye-line)

> Companion to `TL-Seq1_Egypt_Recognition_v1.png`. Standard: `00_Production\20_REFERENCE\Asset_Provenance_Standard.md`. Kept, not deleted.

## Identity
- Asset ID: TL-Seq1_Egypt_Recognition_v1
- Created: 2026-06-26
- Sequence: Sequence One
- Chapter / Scene: Egypt (Recognition two-shot)
- Shot: TL-0070 (recognition beat)
- Creator: Claude Code (Supervisor)
- Generator: Nano Banana
- Model / Version: Gemini 3 Pro Image (gemini-3-pro-image-preview)

## References used (conditioning)
- Master refs: Gary_Master_01_Front, Jen_Master_01_Front

## Prompt (recorded form — see note)
```
Two-shot at sunrise: man (left) stops walking and lifts his eyes, still and
recognizing, not smiling; woman (right) pauses with the smallest hesitation and a
gentle questioning smile... silver pendant on his chest catches the first beam of
sun... 50mm two-shot... warm-gold grade.
```
> NOTE: generated before this provenance standard; verbatim string not preserved. Recorded form from the VFX-001 report. "Lifts his eyes" did not pin the eye-line TO HER — see root cause.

## Negative Prompt
```
(not recorded by the prior session)
```

## Generation parameters
- Aspect ratio: 16:9
- Resolution: 2k (~2752x1536)
- Grounding: on   - Thinking level: high
- Output file: TL-Seq1_Egypt_Recognition_v1.png

## Lifecycle
- Created: 2026-06-26
- Reviewed: 2026-06-26
- Disposition set: 2026-06-26 (Archived -> Production_History)

## Disposition
- Status: Archived (Production_History)
- Current location: 04_Egypt\Stills\Production_History\Composition\
- Derived From: original
- Superseded By: TL-Seq1_Egypt_Recognition_v2 -> v3

## THE LESSON
- Primary Category: Composition
- Secondary Categories: Creative Direction
- Severity: Major  (misses the sequence's defining emotional beat)
- Preventable?: YES
- Reason for Archive: The eye-line choreography is wrong — Gary reads as looking up/away rather than AT Jen; they read side-by-side instead of two souls recognizing each other.
- Root Cause: The prompt named the emotions but not the GAZE GEOMETRY; the model defaulted to a side-by-side two-shot. "Lifts his eyes" was read as upward, not toward her.
- Continuity Decision: n/a.
- Corrective Action: v2/v3 stated gaze explicitly — "he looks DIRECTLY at her, not smiling; she looks back at him" + "connected by a direct eye-line" + negatives (both looking at camera, looking away from each other).
- Creative Impact: The recognition is the emotional hinge of Sequence One; the gaze IS the beat. Getting it wrong loses the whole point.
- Pipeline Impact: New standing rule for two-shots: always specify who looks at whom and the eye-line.
- Lessons Learned: For relational shots, describe geometry (gaze direction, who faces whom) explicitly; emotion words alone won't stage it.
- Would We Generate This Again?: Yes as a staging teaching example; no for the cut.
