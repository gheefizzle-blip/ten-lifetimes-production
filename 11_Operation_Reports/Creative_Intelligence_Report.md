# TEN LIFETIMES — Creative Intelligence Report

> **Auto-generated analytics over the Creative Provenance Dossiers** (not a governance doc; does not trip the Director's Rule). Regenerate on cadence — target **weekly** — by re-reading every `*.md` Dossier under each chapter's `Stills\` tree.

- Generated: 2026-06-26 (instance #2 + forward-looking sections added per Director, PRO-013)
- Corpus: **6 Dossiers**, 1 sequence (Sequence One), 1 chapter generated (Egypt). Sample is small — read trends as directional, not statistical.
- Coverage: 3 Selected (awaiting GVR) · 3 Production_History (archived, classified).

## Top Prompt Improvements
| Change | From → To | Effect |
|---|---|---|
| Added explicit gaze geometry: "he looks DIRECTLY AT the woman", "connected by a direct eye-line", negatives (both looking at camera, looking away from each other, man smiling) | TL-Seq1_Egypt_Recognition_v1 → v2 | Fixed side-by-side default staging; recognition beat lands as intended |
| Added `glasses, eyeglasses, spectacles, eyewear` to negative prompt + conditioned on bare-face master ref (Gary_Master_02_Bareface) | TL-Seq1_Egypt_Recognition_v2 → v3 | Removed anachronistic eyeglasses artifact; historical immersion restored (CD-001) |
| Added quiet-Nile-path positive description + negatives: `grand temple, Karnak, towering columns, hypostyle hall, pyramids, crowds, spectacle, monuments` | TL-Seq1_Egypt_Jen_hero_v1 → v2 | Removed temple spectacle; returned environment to Director's quiet-path Intent (CRE-001) |

## Most Common Continuity Errors
| Error type | Category | Count | Severity | Preventable? | Decision |
|---|---|---|---|---|---|
| Modern eyewear carried from reference photos into ancient-Egypt frame | Historical_Continuity | 1 | Moderate | YES | **CD-001** (Gary bare-eyed in all pre-WWII chapters; glasses WWII+ only) |
| Eye-line geometry wrong — side-by-side staging instead of mutual gaze | Composition | 1 | Major | YES | n/a (corrective rule encoded in Prompt Package) |
| Environment drift to grand temple — contradicts Director's no-spectacle intent | Environment | 1 | Major | YES | n/a (corrective rule encoded in Prompt Package) |

> N=3 archived assets total. Only 1 is a strict Historical_Continuity failure (CD-001); the other two are Creative-Direction class (Composition/gaze, Environment/spectacle).

## Highest-Rated Intent Matches
- **Pending — no GVR scores recorded yet.** GVR-001 (Gary_hero_v1), GVR-002 (Jen_hero_v2), and GVR-003 (Recognition_v3) are all queued but not yet scored by Gemini. Once landed, this section will rank Selected assets by emotional-impact-vs-Intent score. (Informal Supervisor note from VFX-001: Gary_hero_v1 read strongest on first pass — not a scored verdict.)

## Prompt Patterns That Failed
| Root Cause | Failure Mode | Asset(s) | Fix Now Standard |
|---|---|---|---|
| Emotion named, gaze geometry unstated | Model defaulted to side-by-side two-shot; recognition beat lost | TL-Seq1_Egypt_Recognition_v1 | State who-looks-at-whom + eye-line explicitly for all relational/two-shot frames |
| Character described, environment under-constrained, no spectacle negatives | Model invented grand monumental temple setting, contradicting Director's quiet-path intent | TL-Seq1_Egypt_Jen_hero_v1 | Describe environment positively AND negatively for all historical chapters |
| Period subject, modern accessories not negatively suppressed | Model preserved modern eyeglasses from reference photographs into ancient-Egypt frame | TL-Seq1_Egypt_Recognition_v2 | Negative-prompt era-inappropriate accessories; prefer bare-face reference for pre-WWII Gary |

## Studio Standards Established
- **CD-001** — Gary bare-eyed in all pre-WWII chapters (glasses WWII+ only). Source: TL-Seq1_Egypt_Recognition_v2 lesson, ratified by EP (Gary). Applies forward to Rome, Viking, Medieval, Renaissance, Frontier, Victorian.
- **Standing prompt rules** now encoded in Prompt Package / Character Bible:
  - Eyewear negatives (`glasses, eyeglasses, spectacles, eyewear`) for all pre-WWII Gary generations.
  - Gaze geometry (who looks at whom, eye-line direction) required for all relational/two-shot frames.
  - Environment described positively + negatively (spectacle suppression) for all historical chapters.
- **Assets with Studio Standard = Accepted:** none yet — all 3 Selected assets are Pending GVR. TL-Seq1_Egypt_Recognition_v3 is the leading candidate (encodes CD-001 compliance + the Three Recognition Rules; if Accepted, becomes the reference frame for every chapter's recognition beat).

## Knowledge Reused
- **0 reuses recorded** — Egypt is the first sequence generated; `Knowledge Reused In` is empty across all 6 Dossiers.
- **Queued to reuse** (will populate each Dossier's `Knowledge Reused In` as future chapters are produced):
  - CD-001 (Gary eyewear cutoff) → Rome, Viking, Medieval, Renaissance, Frontier, Victorian.
  - Gaze-geometry rule → every two-shot in the film.
  - Environment positive+negative rule → every historical chapter.

## Emerging Risks (forward-looking)
- **Modern-accessory preservation.** The model has carried modern styling into a period frame once (eyeglasses → CD-001). The master refs contain modern styling (Gary cap/glasses; Jen dyed hair/nose ring), so this risk recurs in EVERY pre-WWII chapter. **Watch closely during Rome and all historical chapters** — carry the accessory negatives every time.
- **Rendering frame artifacts.** A rounded border/matte appeared once (TL-0001 v1) on a "first frame of a film" prompt. Risk on any prompt invoking "frame"/"cinematic frame." Keep border/matte negatives standing.
- **Environment overrun toward spectacle.** Under-constrained historical environments drift to monumental settings (Jen v1 temple). Rome (forum, marble) is the next high-risk setting. Constrain environment positively AND negatively.

## Watch Items (protect subtlety)
- **Pendant dominance** (Director guidance) — the pendant must stay subtle: "light finds it, never the camera." Watch it does not become visually dominant as chapters accumulate.
- **Dawn glow vs sunrise** — the opening's "first possibility of light" must not tip into a full sunrise / "beautiful visuals" (north-star: underwhelm visually). Watch warm-glow intensity through Cosmos and Egypt.
- **Same apparent age** — verify continuity as the same two souls recur across ten periods.

---
> Method note: this report is derived purely from Dossier fields (Intent, prompt/negative, evolutionary tree, review, archive lesson, living fields). As the corpus grows, the tables sharpen — eventually showing where the pipeline struggles (e.g. eyewear N, character-drift N) so prompt/ref fixes can target the real failure modes.
