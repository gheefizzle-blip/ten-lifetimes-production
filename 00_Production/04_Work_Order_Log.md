# TEN LIFETIMES — Work Order Log

> Director (Sam) authors work orders. Supervisor (Agent B) executes "as written," STOPs+REPORTs if state invalidates the premise, returns assets. EP (Gary) approves → canon. Reviews route through Gemini (VFX) where visual (Bible §0d).

## Production Departments (taxonomy, adopted 2026-06-25)
Work orders belong to a **department**; new WOs use department-prefixed IDs (`DEPT-###`) for navigability at scale.

| Department | Owner | Responsibility | WO prefix |
|---|---|---|---|
| Creative | ChatGPT (Sam) | Story, symbolism, emotion, cinematic language | `CRE` |
| Production | Claude Code | Work orders, assets, documentation, execution | `PRO` |
| Visual | Gemini | Image/video quality, realism, **continuity**, Veo optimization | `VFX` |
| Editorial | Premiere + Gary | Timeline assembly and pacing | `EDL` |
| Executive Producer | Gary | Final approval, creative/business decisions | (approval gate — not a WO owner) |
| Governance | Continuum | Lineage, reports, approvals, history | `GOV` |

> Refined per Director 2026-06-25. **Continuity folded into VFX** (Gemini); **Release folded into PRO**; **GOV** added (Continuum's lineage/history). WO-execution prefixes: `CRE / PRO / VFX / EDL / GOV`. EP is the approval gate, not a WO owner. (Prior `CON`/`REL` retired; no WOs were issued under them.)

**Legacy crosswalk** (existing `TL-WO-###` IDs retained — not renamed, to preserve canon references):
| Legacy ID | Dept | Note |
|---|---|---|
| TL-WO-000 / 000b | PRO | Scaffold + restructure |
| TL-WO-001 | PRO/EDL | Timeline sync + markers |
| TL-WO-002 | PRO | Master timeline |
| TL-WO-003 | REL | Repo cleanup/sync (restructure deferred) |
| TL-WO-003A | CRE | (superseded by 004) |
| TL-WO-004 | CRE | Sequence One direction |

*New work orders use `DEPT-###` (e.g. `CRE-005`, `VFX-001`). Department + legacy IDs both indexed here.*

**Work-order template:**
```
TL-WO-###  | <title>
Owner:      <Claude Code / Director>
Status:     DRAFT | AUTHORIZED | IN PROGRESS | BLOCKED | COMPLETE | COMPLETE WITH NOTES
Inputs:     <master refs, prior assets, prompts>
Output:     <exact deliverables>
Acceptance: <criteria — faces match masters, period-correct, pendant present, 16:9, realism, etc.>
Notes:      <constraints / safety>
```

| WO | Title | Owner | Status | Result | Date |
|---|---|---|---|---|---|
| TL-WO-000 | Project scaffold + production system (this build) | Claude Code | COMPLETE | Folder tree, Bible, Timeline, Shot DB, logs, lyrics, START_HERE created | 2026-06-24 |
| TL-WO-000b | Authority-based restructure (per Director review) | Claude Code | COMPLETE | Subfolders 10–30; PROJECT_STATE; Risk Register; Master Production Timeline format; Camera/Character/Style bibles | 2026-06-24 |
| **TL-WO-001** | **Master Timeline Synchronization** | Claude Code | **COMPLETE** (EP-locked) | Alignment (320 words/66 lines/329.60s) + section boundaries MEASURED from drums/perc stems + Premiere markers (24fps) + 320-word Master Timeline + 66 prelim line-shots, all in `20_REFERENCE\`. **EP locked Timeline v1.0 → PT-0.5 on 2026-06-25** (fps=24; chapter overlay approved as-is). Shot DB → v0.2. | 2026-06-25 |

| **TL-WO-002** | **Master Production Timeline Generation** | Claude Code | **COMPLETE** | Generated `00_Production\MASTER_PRODUCTION_TIMELINE.md` — the single foundational relational artifact: 320 words × 14 cols (Time/Word/Beat/Section/Emotion/Chapter/Shot/Transition/Camera/Color/Prompt ID/Render ID/Premiere Marker/Status). Objective cols MEASURED+locked; creative cols → Director; production cols → pipeline. Canon Rule (systems of truth) added to Bible §0a. | 2026-06-25 |
| TL-WO-003 | Public-repo restructure + targeted doc path-cleanup + sync | Claude Code | **IN PROGRESS** (b+c done; a deferred) | ✅ (b) **Path-cleanup DONE** — 3 real stale paths fixed (Bible ×2, Revision Log ×1); title prose + un-renamed `Tommy Ransome…\TEN LIFETIMES\` preserved. ✅ (c) **Public sync DONE** — 6 canon docs + new MASTER_PRODUCTION_TIMELINE pushed to `main` (commit `ab83ee1`), zero media verified. ⏸ (a) **Folder restructure DEFERRED** (EP: use-don't-expand) — needs Director mapping vs the flattened public mirror before churning. | 2026-06-25 |

| **TL-WO-003A** | **Director's Creative Development — Chapter One (Egypt)** | Director (Sam) → Claude Code | **SUPERSEDED by TL-WO-004** (reframed Egypt → Sequence One; scaffolds rebuilt at sequence scope) | Finish Egypt to feature quality first. **Agent B scaffolded** (measured backbone, creative fields for Director) in `40_CHAPTERS\01_Egypt\`: (3) Scene Breakdown ✅ (4) Shot Breakdown ✅ (TL-0010–0080) (6) Costume Bible ✅ (7) Environment Bible ✅ (8) Lighting Plan ✅; plus (1) Emotional Storyboard ✅ *draft* and (5) TS-001 ✅ *draft*. **Pending Director authoring:** (2) Camera Storyboard + creative fill of 1,3–8. **Pending:** (9) Prompt Package, (10) Review. **B-2 master refs LOCKED (interim)** → generation unblocked (residual: B-1 tooling host; fresh portrait set recommended before final renders). New global layers: `Emotional_Storyboard.md`, `Transition_Bible.md`; Camera Bible Narrative-Camera language. | 2026-06-25 |

| **TL-WO-004** | **Director's Sequence One** (0:00.000–1:03.820 · Cosmos→Egypt→Rome) | Director (Sam) → Claude Code | **IN PROGRESS** (scaffolds ready; Director authoring) | Reframes Egypt → **Sequence One** (one continuous opening; the film's benchmark). **Agent B scaffolded** `40_SEQUENCES\Seq01_Opening\` — 12 deliverables: INDEX + Storyboard (the relational spine consolidating Emotional/Memory/Camera/Lighting/Transition/Symbol as columns) + Narrative + Environment + Costume + Shot List + Prompt Package (gated B-1) + Review Package. Measured backbone (TL-0001–0120, TS-001) LOCKED; creative cells **[Director to author]**. Absorbs TL-WO-003A. Canon: Bible §0b (roles) + §0c (Three Recognition Rules); Camera Bible **Presence**; Emotional Storyboard **Memory** field. | 2026-06-25 |

| **PRO-005** | **Gemini onboarding + Departments + Dashboard** (governance) | Director (Sam) / Gemini → Claude Code | **COMPLETE** | Added Gemini as **VFX Supervisor / Cinematic Review Authority** (Bible §0b team + §0d Charter, **ratified by Gemini 2026-06-25** — review-only, no creative authorship). Established **Production Departments** (CRE/VFX/EDL/PRO/CON/REL) + legacy crosswalk. Built **`00_PRODUCTION_DASHBOARD.md`** and **`11_REVIEWS\Gemini\00_Gemini_Review_Log.md`** (GVR + Continuity + Veo/Sora strategy). First department-prefixed WO. **Gate satisfied:** charter canonized → Sequence One generation may proceed once B-1 resolved. | 2026-06-25 |

| **PRO-006** | **Public Operation Report Standard** | EP (Gary) → Claude Code | **COMPLETE** | Durable cross-agent audit trail: every operation → work-order file + **public completion report** + canon updates + GitHub sync (unless EP-held). Created `60_TEMPLATES\Operation_Report_Template.md`, `11_OPERATION_REPORTS\` (NAS) / `11_Operation_Reports\` (public); Bible **§0e** rule; backfilled first reports (PRO-005, PRO-006). ASCII-only, zero media. | 2026-06-25 |

| **PRO-007** | **Op-Report Standard v1.1 + Production Loop + North-Star** | Director (Sam) → Claude Code | **COMPLETE** | Per Director feedback: reformatted `Operation_Report_Template.md` (ASCII-only — removed em-dashes — + short lines, no long-line flattening); added **Lessons Learned** section to the standard (Bible §0e) + template + backfilled PRO-005/PRO-006. Canonized the **Production Loop** (hero stills → Director → Gemini GVR → EP → lock look → supporting stills → motion → Gemini motion → final) and the **creative north-star** ("make them forget AI exists") as Bible **§0f**. Dashboard aligned to Director's framing (system done, film 0%). | 2026-06-26 |

| **PRO-008** | **Dept refinement + Creative Impact + Production Journal** | Director (Sam) → Claude Code | **COMPLETE** | Per Director: refined departments to **CRE/PRO/VFX/EDL/EP/GOV** (Continuity→VFX, Release→PRO, +GOV=Continuum; retired CON/REL). Added **Creative Impact** section to the report standard (Bible §0e + template) + backfilled PRO-005/006/007. Reframed the public repo as **"The Production Journal"** (README rewrite). | 2026-06-26 |

| **PRO-009** | **Creative Production transition (infrastructure FREEZE)** | Director (Sam) → Claude Code | **COMPLETE — FINAL INFRA WO** | Enacts the phase change pre-production → **Creative Production**. Expanded the report reflection block to **Lessons Learned / Creative Impact / Pipeline Impact / Recommendations / Would We Do This Again?** (Bible §0e + template + backfilled PRO-005/006/007/008). Added Bible **§0g** + **The Director's Rule** (no new infra unless it solves a demonstrated production problem). Phase relabeled in PROJECT_STATE + Dashboard. **Infrastructure is now frozen; next WO is CRE-001 (Director).** | 2026-06-26 |

| **PRO-010** | **Milestone: Studio Operational** | EP (Gary) + Director (Sam) + Gemini → Claude Code | **COMPLETE — milestone recorded** | Recorded the **Studio Operational** milestone (Ready for Principal Photography) in PROJECT_STATE / Dashboard / Revision Log. Finalized **The Director's Rule** to its binding wording (judged by: did it make the film better?). Added the **Sequence Retrospective** craftsmanship practice (sequence-level, Bible §0f). Closing administrative act of the freeze. | 2026-06-26 |

*(Infrastructure FROZEN per Bible §0g. The next work order is **CRE-001** (Director). Further PRO/infra WOs require a demonstrated blocker or measurable film-quality gain.)*
