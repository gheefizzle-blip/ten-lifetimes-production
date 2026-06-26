# OPERATION REPORT - PRO-011 Asset Provenance System

## Header

- Work Order ID: PRO-011
- Title: Asset Provenance System (Production Journal / creative-provenance)
- Department: Production (PRO) / Governance (GOV)
- Executor: Claude Code (Production Supervisor)
- Started: 2026-06-26
- Completed: 2026-06-26

## Inputs

- Director (Sam) design conversation + EP (Gary) direction, 2026-06-26: the repo is a Production Journal, not a lean source tree; never delete generated assets - classify, annotate, learn. Metadata is born with the asset and carries the exact prompt.
- The demonstrated problem: the Recognition_v2 glasses incident nearly erased a reusable lesson when the superseded frame was dropped from the repo.
- Existing 6 Egypt renders (VFX-001/002) to bring under the standard retroactively.

## Actions Performed

1. Authored `20_REFERENCE\Asset_Provenance_Standard.md` (born-with-asset rule, lifecycle, four destinies, folder structure, 13 categories, 5-level severity, Preventable? field, never-delete principle).
2. Authored `60_TEMPLATES\Asset_Provenance_Template.md` (per-asset fill-in incl. verbatim prompt/negative/params/refs/lineage + the archive lesson block).
3. Formalized **CD-001** (Gary eyewear period cutoff) in a new Continuity Decisions ledger in `Continuity_Report.md`.
4. Restructured `04_Egypt\Stills\` into `Working\` / `Selected\` / `Production_History\<Category>\`; relocated the 6 assets to their dispositions (3 selects -> Selected; 3 superseded -> Production_History by category).
5. Wrote a companion `.md` provenance file for ALL 6 assets - exact prompts/negatives/params captured verbatim for the 3 I generated this session (Jen v2, Recognition v2, v3); v1 trio captured in the recorded form from the VFX-001 report with an explicit note that they pre-date the standard (the gap that motivates it).
6. Wired the standard into canon: Bible **§0f** (born-with-asset rule in the Production Loop) + Asset Register (provenance table, new locations, never-delete storage model).

## Classification of the first archived set

- `Recognition_v2` -> Historical_Continuity, Severity Moderate, Preventable YES, **CD-001** (glasses).
- `Jen_hero_v1` -> Environment (Major, Preventable YES) - temple "spectacle" vs CRE-001.
- `Recognition_v1` -> Composition (Major, Preventable YES) - gaze/eye-line staging.

## Files Created (NAS)

- `20_REFERENCE\Asset_Provenance_Standard.md`
- `60_TEMPLATES\Asset_Provenance_Template.md`
- 6 companion provenance `.md` files under `04_Egypt\Stills\...`
- this report

## Files Modified (NAS)

- `20_REFERENCE\Continuity_Report.md` (CD-### ledger + CD-001)
- `20_REFERENCE\Asset_Register.md` (provenance table, locations, storage model)
- `01_Production_Bible.md` (§0f born-with-asset rule)

## Media

- No new media generated. 6 existing PNGs relocated within the NAS vault (nothing deleted).

## Public exposure (EP decision 2026-06-26)

- EP chose **full ILM-style public archive**: provenance `.md` (selects + archived) AND the archived images publish to the public repo. New `.gitignore` exception for `13_Production_History/**`; selects' `.md` join their images in `12_Dailies/`. (Per-asset images of real likenesses now public on the All-Rights-Reserved repo by explicit EP choice - institutional value weighed over privacy.)

## Open Blockers

- B-1 (motion) unchanged. No new blockers.

## Next Recommended Action

- Apply the born-with-asset rule to every future generation automatically (generate PNG -> immediately write `.md` -> register both). Director + Gemini GVR + EP review of the 3 Egypt selects still pending -> their verdicts get written into the selects' provenance files, then look-lock.

## Lessons Learned

- Provenance must be captured at generation time: the v1 trio already lost their verbatim prompts (only the report's condensed form survives) - exactly the loss this standard prevents going forward.
- A failed render plus its "why" is more valuable than a clean render alone; CD-001 exists because we kept Recognition_v2.

## Creative Impact

- Converts discarded generations into a production-intelligence database: searchable by failure type, prompt, and corrective decision. Compounds in value every sequence.

## Pipeline Impact

- New standing workflow + folder taxonomy + classification scheme; the repo is now explicitly a Production Journal. Future Continuum productions inherit the method.

## Recommendations

- Track aggregate failure categories over time (e.g. eyewear N, character-drift N) to see where the pipeline struggles and target prompt/ref fixes.

## Would We Do This Again?

- Yes. This is arguably the most valuable systemic addition since the Master Production Timeline.

## Supervisor Attestation

- Files: created ~9 (2 framework + 6 provenance + this report), modified 3 (NAS canon), 6 media relocated (0 deleted).
- This operation translated the Director's authored design + EP direction into structure; it did not author creative content.
- Local Agent C operational-memory writes this operation: 0 (memory update, if any, disclosed separately after public sync).
- Public commit/push performed per the EP full-archive decision; recorded in the follow-up sync.
