# OPERATION REPORT - VFX-002 Sequence One Hero Stills Retakes (Egypt)

## Header

- Work Order ID: VFX-002 (continues VFX-001; executes CRE-001)
- Title: Sequence One hero stills - Egypt - retake pass (Jen hero + Recognition two-shot)
- Department: Visual Effects (VFX)
- Executor: Claude Code (Production Supervisor)
- Started: 2026-06-26
- Completed: 2026-06-26 (generation + tracking done; review pending)

## Inputs

- CRE-001 Director's Narrative (Sam) - Sequence One emotional intent (recognition; quiet path, no spectacle; he looks first / she hesitates then smiles; pendant catches the light).
- VFX-001 first pass + its Supervisor iteration notes (Jen drifted to temple spectacle; recognition gaze read side-by-side).
- Master references (16_Master_References): 3 Gary + 3 Jen (interim, locked).
- Acceptance criteria (no anachronisms; period-correct; pendant present; Reality Test).
- Tooling: Nano Banana MCP, model Gemini-3-Pro-Image, live on GSA-1000.

## Actions Performed

1. Re-ran the **Jen hero** (PR-S1-002 v2): returned her to Sam's quiet Nile dawn path; removed grand-temple/columns/crowds via negative prompt; conditioned on the 3 Jen master refs; pro model, 4k.
2. Re-ran the **Recognition two-shot** (PR-S1-003 v2): rewrote the prompt to state gaze direction explicitly ("he looks DIRECTLY at her, not smiling; she pauses, then a gentle questioning smile") and the pendant light-catch.
3. Caught an acceptance-criteria fail in v2 (model added modern **eyeglasses** onto Gary - period anachronism) and re-ran as **v3**: added `glasses/eyeglasses/spectacles/eyewear` to the negative prompt and conditioned on the bare-face master ref. v3 is clean.
4. Selected the batch: **Gary hero v1** (held, unchanged) - **Jen hero v2** - **Recognition v3**. Marked v1 Jen and v1/v2 Recognition SUPERSEDED.
5. Registered selects + supersessions in the Asset Register; updated the Prompt Package; re-pointed GVR-001/002/003 at the selects; reconciled 00_PROJECT_STATE + dashboard to current reality.
6. Mirrored the two new selects into the public repo working tree `12_Dailies/Seq01_Egypt/` and removed the superseded v1 frames there. **Did NOT commit/push** - see Open Blockers.

## Prompts (retakes, as run)

- PR-S1-002 v2 (Jen, Jen_01/02/03): quiet sandy Nile path at dawn; late-30s warm genuine face (match refs), natural dark hair, undyed linen, small silver pendant; faint beginning of recognition; low mud-brick dwellings far in misty distance; NO temple/columns/crowds/spectacle; 85mm shallow DOF, 35mm grain, warm-gold grade. Negative: grand temple, Karnak, columns, pyramids, crowds, spectacle, monuments, modern styling, dyed hair, nose ring.
- PR-S1-003 v2 -> v3 (two-shot, v3 = Gary_02 bareface + Gary_01 + Jen_01): 50mm two-shot, eye-line connecting them; man (left) stopped, looking directly at her, NOT smiling, calm/intent; small silver pendant catching a low sun-beam; woman (right) pauses, smallest hesitation softening into a gentle questioning small smile; recognition not romance; quiet Nile dawn, no spectacle; warm-gold grade. Negative (v3 added): glasses, eyeglasses, spectacles, eyewear; plus both-looking-at-camera, romance, temple, modern styling.

## Files Created

- `11_OPERATION_REPORTS\2026-06-26_VFX-002_Sequence_One_Hero_Stills_Retakes_REPORT.md` (this file)

## Files Modified (NAS canon)

- `00_PROJECT_STATE.md` - milestone -> Principal Photography Begun; current focus -> CRE-001 authored + VFX-001/002 selects awaiting GVR; recent-history entry.
- `00_PRODUCTION_DASHBOARD.md` - sequence/pipeline bars, Generated Stills 0 -> 3 selects, dept table.
- `20_REFERENCE\Asset_Register.md` - 3 selects + 3 supersessions; media-exposure mechanics note.
- `40_SEQUENCES\Seq01_Opening\Sequence_One_Prompt_Package.md` - v2/v3 select IDs + retake resolutions + glasses lesson.
- `11_REVIEWS\Gemini\00_Gemini_Review_Log.md` - GVR-002/003 re-pointed at v2/v3 selects.

## Media Generated

- 2 new stills on NAS `D:\My_Music\Ten_Lifetimes\04_Egypt\Stills\` (5504x3072, 4k): `TL-Seq1_Egypt_Jen_hero_v2.png`, `TL-Seq1_Egypt_Recognition_v3.png`. (Plus interim `Recognition_v2.png`, superseded by v3.) Mirrored selects into public `12_Dailies\Seq01_Egypt\` working tree; NOT yet committed.

## Open Blockers

- **PUBLIC REPO MID-OPERATION (raised by VFX-002, for EP).** The public repo working tree is dirty with a **prior-session staged-but-uncommitted batch** (the `.gitignore` media exception, the three v1 daily PNGs, and public-copy edits to Bible / Asset Register / Revision Log / Gemini log / Prompt Package / VFX-001 report). HEAD = `c9a1ecb`; despite VFX-001 reporting commit `163c577`, the daily IMAGES never actually committed (the .gitignore exception was staged after). Net: GitHub does not yet actually expose the stills to Gemini. Reconciliation + a clean commit/push is an EP-gated, outward-facing action - HELD pending EP direction. Public-repo doc copies also still need syncing to the NAS edits above.
- **B-1 (motion):** Veo/Sora still no direct bridge (stills tooling fully working).

## Next Recommended Action

- EP decides the public-repo path (see Open Blockers): reconcile the prior staged batch + this batch into one clean "VFX-002: Egypt hero selects + dailies exposure" commit, then push - so Gemini can pull the selects for GVR-001/002/003.
- Director (Sam) review + Gemini GVR + EP approval of the three selects -> if approved, LOCK the Egypt visual language (Production Loop step 5) before any supporting stills.

## Lessons Learned

- Explicit gaze direction is mandatory for two-shots: stating "he looks at her / she looks back at him" fixed the side-by-side default in one pass.
- Nano Banana can add modern eyewear to an older male subject unprompted; carry `glasses/eyeglasses/spectacles/eyewear` in Gary's negative prompt and prefer the bare-face master ref. Added as a standing prompt rule in the Prompt Package.
- Negative-prompting environment ("no temple/columns/spectacle") plus a positive quiet-path description reliably pulled Jen back to Sam's intent.
- Catching the anachronism at still-review cost one extra image; catching it after motion/edit would have cost a chapter.

## Creative Impact

- The opening's defining frame (the recognition) now reads as Sam wrote it: he sees her first and goes still; she hesitates, then the smallest knowing smile. The pendant catches the light. This is the emotional hinge of Sequence One and it now lands in a single still.
- Jen's hero no longer competes with a monument; she is a person on a quiet morning road - which is the whole point ("an ancient civilization breathing").
- Still a concept-lock pass: faces + look are not yet Director/Gemini/EP-approved. Treat as selects, not locked.

## Pipeline Impact

- Confirms the retake loop inside the Production Loop: generate -> Supervisor flags vs Director intent + acceptance criteria -> targeted re-run -> register/supersede. Cheap, fast, and it keeps a clean audit trail (every superseded frame is logged, not deleted).

## Recommendations

- Hold all supporting-still generation until the three selects are GVR'd and the Egypt look is locked.
- Before final-quality renders, shoot the recommended fresh purpose-shot master portrait set (interim casual snapshots are good enough for concept-lock, as VFX-001/002 prove).

## Would We Do This Again?

- Yes. A tight 3-frame hero set with a fast retake loop validated faces, environment, and the key emotional beat for the price of a few images - exactly the de-risking a benchmark sequence needs before scaling.

## Supervisor Attestation

- Files: created 1, modified 5 (NAS canon), deleted 0. Media generated: 2 selects + 1 interim (local NAS; mirrored to public working tree but NOT committed/pushed).
- GitHub: nothing committed or pushed this operation; the public repo remains on HEAD `c9a1ecb` with a pre-existing staged batch left untouched by me (only 2 untracked PNGs added to the working tree). Public commit/push is EP-gated and HELD.
- Local Agent C operational-memory writes this operation: 0.
- Attestation: faithful, literal account. The Supervisor translated the Director's authored intent into prompts and did NOT author story/emotion. Creative and visual approval remain with the Director, Gemini, and the EP.
