# ASSET PROVENANCE — TL-Seq1_Egypt_Recognition_v2  (ARCHIVED — the canonical glasses lesson)

> Companion to `TL-Seq1_Egypt_Recognition_v2.png`. Standard: `00_Production\20_REFERENCE\Asset_Provenance_Standard.md`. This asset is KEPT, not deleted: it is the reference example that produced continuity decision CD-001.

## Identity
- Asset ID: TL-Seq1_Egypt_Recognition_v2
- Created: 2026-06-26
- Sequence: Sequence One
- Chapter / Scene: Egypt (Recognition two-shot)
- Shot: TL-0070 (recognition beat)
- Creator: Claude Code (Supervisor)
- Generator: Nano Banana
- Model / Version: Gemini 3 Pro Image (gemini-3-pro-image-preview)

## References used (conditioning)
- Master refs: Gary_Master_01_Front, Jen_Master_01_Front

## Prompt (verbatim)
```
Ancient Egypt, sunrise, on a quiet sandy path beside the Nile. A cinematic 50mm two-shot of a man and a woman who have just stopped walking and noticed each other, both faces clearly visible and connected by a direct eye-line. LEFT: a man in his early 50s with a salt-and-pepper beard and kind, weathered, searching eyes (match the male reference exactly), in undyed linen robes. He has stopped walking and stands still, turning his head and looking DIRECTLY AT the woman, calm and quietly recognizing — he is NOT smiling, his lips are closed, his expression is still and intent. A small silver pendant rests on his chest and a narrow beam of low golden morning sunlight catches it, making it glint for an instant. RIGHT: a woman in her late 30s with a warm genuine face and bright expressive eyes (match the female reference exactly), natural dark hair pulled back, in fine undyed linen. She has paused and looks back at him — the smallest hesitation in her expression softening into a gentle, almost questioning small smile. This is recognition, not romance; a quiet, ancient familiarity. No words. Their gazes meet. Soft warm golden dawn light fully clearing the horizon, warming both faces equally. Quiet riverbank, low mud-brick dwellings far in the misty distance, no crowds, no spectacle. Shot on 50mm, gentle shallow depth of field, subtle 35mm film grain, warm-gold cinematic grade. Photorealistic, indistinguishable from a real frame of a feature film.
```

## Negative Prompt (verbatim)
```
both looking at camera, looking away from each other, man smiling, big grin, romance, kiss, embrace, crowds, temple, columns, pyramids, monuments, modern clothing, dyed hair, nose ring, cartoon, illustration, CGI look, plastic skin, fused faces, identical twins
```
> Note: the negative prompt did NOT include eyewear terms. That omission is the root cause below.

## Generation parameters
- Aspect ratio: 16:9
- Resolution: 4k (5504x3072)
- Grounding: on   - Thinking level: high
- Output file: TL-Seq1_Egypt_Recognition_v2.png

## Lifecycle
- Created: 2026-06-26
- Reviewed: 2026-06-26 (Supervisor caught the artifact)
- Disposition set: 2026-06-26 (Archived -> Production_History)

## Disposition
- Status: Archived (Production_History)
- Current location: 04_Egypt\Stills\Production_History\Historical_Continuity\
- Derived From: TL-Seq1_Egypt_Recognition_v1 (gaze choreography corrected)
- Superseded By: TL-Seq1_Egypt_Recognition_v3

## Review history
- Director (Sam): n/a (caught pre-GVR)
- Gemini: n/a
- EP (Gary): flagged glasses on review; ratified the period rule

## THE LESSON
- Primary Category: Historical Continuity
- Secondary Categories: Character Consistency
- Severity: Moderate  (does not ruin the frame, but blocks acceptance)
- Preventable?: YES
- Reason for Archive: Modern eyeglasses appeared on Gary — an anachronism in ancient Egypt.
- Root Cause: The model preserved a modern accessory from the reference photographs (Gary wears glasses in the source snapshots) rather than adapting identity to the historical period; the negative prompt did not suppress eyewear.
- Continuity Decision: CD-001 (Gary eyewear period cutoff — no glasses before WWII).
- Corrective Action: (1) added `glasses, eyeglasses, spectacles, eyewear` to Gary's negative prompt; (2) conditioned the retake on the bare-face master ref (Gary_Master_02_Bareface); (3) encoded the period rule in the Character Bible + Prompt Package.
- Creative Impact: Removing the glasses restored historical immersion without reducing character recognizability.
- Pipeline Impact: Standing prompt rule + Character Bible PERIOD RULE + CD-001; all future pre-WWII Gary generations are now protected.
- Lessons Learned: Identity references should preserve facial STRUCTURE, not modern accessories. Always suppress era-inappropriate eyewear/jewelry/styling for historical chapters.
- Would We Generate This Again?: Yes — keeping this failed frame is precisely how the studio learns. It is the worked example behind CD-001.
