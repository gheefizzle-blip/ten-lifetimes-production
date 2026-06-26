# OPERATION REPORT - PRO-014 GitHub Asset Canon and Review Queue Correction

## Header
- Work Order ID: PRO-014 (Director-issued)
- Title: GitHub Asset Canon and Review Queue Correction
- Department: Production (PRO) / Governance (GOV)
- Executor: Claude Code (Production Supervisor)
- Started / Completed: 2026-06-26

## Objective
Correct the asset-visibility workflow so all generated production assets are committed to GitHub with their Dossiers (Review Queue, Dailies, Production History, Selected, Final), and reviewers evaluate the published FRAME, not a description.

## Why this clears the Director's Rule
- Removes a demonstrated blocker: the Director (and Gemini) could not review HERO-01 because it lived NAS-only; they were handed the Supervisor's written description instead. No creative authority approves a description.

## Canon rules established
1. **GitHub is the canonical production-history repository** for all generated assets + Dossiers.
2. **NAS is the local working mirror** (Premiere / Adobe / generation). It also remains the private home of NON-generated source assets (Gary/Jen source photos, music masters, stems, .prproj) -- those are NOT published.
3. **No generated asset may remain NAS-only once it has a Dossier.**
4. Every generated asset is published to GitHub with its Dossier **before** Director / Gemini / EP review.
5. Review Queue assets are visible dailies, NOT approved canon.
6. Rejected/superseded -> Production_History (never deleted).
7. Selected (locked) -> 14_Selected. 8. Final approved -> 15_Final.
9. Every movement updates the Dossier lifecycle + the Asset Register.

## Public folder model
- `12_Review_Queue/Seq<NN>_Hero<NN>/` -- under review (image + Dossier); not canon.
- `12_Dailies/Seq<NN>_<Chapter>/` -- review/working selects (earlier Egypt selects).
- `13_Production_History/Seq<NN>_<Chapter>/<Category>/` -- archived/rejected, classified.
- `14_Selected/Seq<NN>/` -- LOCKED selects. `15_Final/Seq<NN>/` -- final approved.
Lifecycle: `Created -> Review Queue -> Director -> Gemini -> EP -> LOCK -> Selected -> Final` (or -> Production_History).

## Supervisor conduct rule (Director, 2026-06-26)
The Supervisor announces readiness ("HERO-01 ready for Director review") and reports only OBJECTIVE, MEASURABLE observations (e.g. "eyeglasses detected", "a landform is present vs the brief", "rendered with a border"). It does NOT issue SUBJECTIVE cinematic judgments before Director + Gemini have seen the frame; reviewers evaluate independently.

## Actions Performed
1. Canon: Bible 0a Canon Rule revised (GitHub = full production history; NAS = working mirror); Creative Provenance Standard rewritten with the GitHub Asset Canon + 5-folder public model + lifecycle; Asset Dossier template gained the Review Queue state.
2. Created the public folder model: `12_Review_Queue/`, `14_Selected/`, `15_Final/` (with READMEs); `.gitignore` exceptions for `12_Review_Queue/**`, `14_Selected/**`, `15_Final/**` (joining the existing `12_Dailies` + `13_Production_History`).
3. Published HERO-01 to GitHub: `TL-0001_Cosmos_BeforeTime_v2` image + Dossier -> `12_Review_Queue/Seq01_Hero01/`; archived parent `v1` image + Dossier -> `13_Production_History/Seq01_Cosmos/Rendering_Artifact/`. (No NEW media generated -- existing renders published.)
4. HERO-01 Dossier set to Status = Review Queue; subjective notes replaced with objective-only observations (a distant landform is present vs the "no land features" brief).
5. Updated the Creative Intelligence Report scope + the weekly cloud routine to read Review Queue / Dailies / Production History / Selected / Final.
6. Asset Register + Revision Log updated.

## Self-correction (logged)
- On HERO-01 the Supervisor previously offered subjective judgments ("shoreline distracting", "dawn-glow tipping toward sunrise") on a frame the authorities had not seen -- the exact failure this gate removes. Retracted; reserved to Director + Gemini from the published frame.

## EP exposure note (flagged for the record)
- This reverses the project's founding media firewall ("never commit media; NAS private vault"). It makes ALL generated AI likenesses (incl. rejected renders) permanently public on the All-Rights-Reserved repo. Executed per EP direction (Gary relaying the Director's PRO-014); flagged so the exposure is a conscious EP choice. Non-generated source assets (real source photos, music) remain NAS-private.

## Open / Pending
- **HERO-01 is now in the Review Queue on GitHub, READY for Director review.** Gate: Director -> Gemini GVR-004 -> EP -> LOCK. No HERO-02 until HERO-01 LOCKs.

## Would We Do This Again?
- Yes. The blocker was real (reviewers couldn't see the asset); the correction is structural and small.

## Supervisor Attestation
- Files: created this report + 2 folder READMEs + Review Queue/Production_History publish copies; modified ~7 NAS canon docs; deleted 0. **No new media generated** (HERO-01 v1/v2 already existed; published, not regenerated).
- No creative content or subjective cinematic judgment authored.
- Public commit/push performed; HERO-01 now public for review by Director direction; founding-firewall reversal flagged for EP.
