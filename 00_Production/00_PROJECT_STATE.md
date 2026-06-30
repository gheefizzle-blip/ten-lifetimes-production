# TEN LIFETIMES — A Cinematic Short Film — PROJECT STATE (canonical)

> **The single source of truth for where the production stands.** Read this first.
> Per Director's architecture (2026-06-24): the project is organized around **authority**. These canonical files
> (`00_PROJECT_STATE`, `01_Production_Bible`, `02_Directors_Timeline`, `03_Shot_Database`) hold the state;
> everything else is **evidence supporting** it.

- **🎬 MILESTONE: EDL-001 CANON LOCKED — PLANNING PHASE CLOSED; PRODUCTION BEGINS** (2026-06-28). The master runtime allocation is immutable; the music is the master clock. Four Performance Anchors locked (HERO-01→04). Identity (CCAs) + costumes solved; PRO-017 Performance Anchor methodology validated. **Pre-production is over — the studio is now a production organization.**
- **Phase:** **PRODUCTION — Phase 2: Performance Validation.** Sole deliverable = **Performance Segment 001** (Opening Movement, HERO-01→04). Planning is frozen (runtime/era/chorus/emotional allocation locked — Director's Standing Order). Every hour now moves pixels, not paragraphs.
- **Production version:** **PT-1.0** (planning complete; EDL-001 locked 2026-06-28).
- **Last updated:** 2026-06-29 by Agent B (Production Supervisor) — first motion rendered: programmatic Veo bridge live; PS001-VEO standard-tier clip in Review Queue pending Gemini blind GVR; Grok clip not yet delivered.
- **Public docs repo (system of record for docs/prompts):** `gheefizzle-blip/ten-lifetimes-production` (GitHub, PUBLIC, docs only — **no media**). NAS = private asset vault. Claude Code pushes doc updates.

---

## Lock status

| Element | Locked? | Gate doc |
|---|---|---|
| Audio (master delivered) | ✅ Yes | `TEN LIFETIMES.mp3` |
| **Timeline v1.0** (fps=24) | ✅ **LOCKED** (EP, 2026-06-25) — TL-WO-001 | 02_Directors_Timeline |
| **Master Runtime Allocation (EDL-001)** | ✅ **CANON LOCKED — IMMUTABLE** (EP, 2026-06-28) | 04_Master_Runtime_Allocation |
| **Cast / identity (CCA-001 Gary, CCA-002 Jen)** | ✅ **LOCKED** (Egypt set; Sheet-Based Conditioning) | CCA_Registry, 00_Identity_Master |
| **Costumes (Egypt: Architect / Scholar)** | ✅ **LOCKED** | 00_Costume_Master |
| **Performance Anchors HERO-01→04** | ✅ **LOCKED** (Cosmos + Egypt ×3) | 14_Selected/Seq01 |
| Story / emotional structure | ✅ Locked (CRE-001..006 + EDL-001) | 01_Production_Bible, 40_SEQUENCES |
| Motion (Performance Segments) | 🟡 In production — **first Veo clip rendered** (PS001-VEO, pending Gemini GVR) | EDL-001 §7 · `12_Review_Queue/Seq01_PerfSeg001/` |
| Picture / Color (full cut) | ⬜ Downstream | 21_STYLE_GUIDES |

---

## Authority-based document map (`00_Production\`)

**Canonical state (root):**
- `00_PROJECT_STATE.md` — this file
- `00_PRODUCTION_DASHBOARD.md` — at-a-glance status (sequences + pipeline + blockers)
- `01_Production_Bible.md` — the constitution (creative decisions only) · **§0a Canon Rule = systems of truth**
- `MASTER_PRODUCTION_TIMELINE.md` — **THE foundational relational artifact** (TL-WO-002): every word → time/section/chapter/shot/prompt/render/clip/status. Effectively immutable; everything downstream references it.
- `02_Directors_Timeline.md` — narrative/structural timeline (section map, edit model, decisions) feeding the master table
- `Emotional_Storyboard.md` — **the layer between Timeline and Shot DB:** "what should the audience *feel*?" + **Memory** ("what they remember 30 min later")
- `Transition_Bible.md` — named reusable chapter-to-chapter transitions `TS-###` (history transforms, love continuous)
- `40_SEQUENCES\Seq01_Opening\` — **Sequence One (the benchmark)** — TL-WO-004 deliverable scaffolds (Cosmos→Egypt→Rome, 0:00–1:03.82)
- **Bible §0b** (roles: Director/Supervisor/EP) · **§0c** (Three Recognition Rules) · Camera Bible **Presence**
- `03_Shot_Database.md` — every shot TL-####
- `07_Revision_Log.md` — major decisions
- `Risk_Register.md` — production risk register

**Evidence / supporting (subfolders):**
| Folder | Holds |
|---|---|
| `10_WORK_ORDERS\` | TL-WO-### work orders + `00_Work_Order_Log.md` index |
| `11_REVIEWS\` | Director (Sam) reviews |
| `12_APPROVALS\` | EP (Gary) approvals → what becomes canon |
| `13_RENDER_LOGS\` | `Render_Register.md` + per-render notes |
| `20_REFERENCE\` | `Asset_Register.md`, `Continuity_Report.md`, `Lyrics_Annotated.md` |
| `21_STYLE_GUIDES\` | color script / grade per chapter |
| `22_CAMERA_BIBLE\` | lens/movement language |
| `23_CHARACTER_BIBLE\` | master refs, permanent traits, per-chapter casting |
| `30_EXPORTS\` | deliverable exports (reels, full cut) |

**Asset folders (project root):** `01_Reference_Gary` (5) · `02_Reference_Jen` (8) · `03_Couple_Photos` (7) · `04_Egypt`…`13_Future` · `14_Bridge` · `15_Finale` · `16_Master_References` · `18_Motifs`. Each chapter: `References/Stills/Motion/Final`.

---

## Roles (team — Bible §0b/§0d)
- **EP / final authority:** Gary Spear — approvals → `12_APPROVALS\`
- **Director:** ChatGPT "Sam" — creative authorship; reviews → `11_REVIEWS\`
- **Production Supervisor:** Claude Code (Agent B) — execution, docs, assets, tracking
- **VFX / Cinematic Review:** Gemini — reviews generated output only (GVR + continuity); **no creative authorship**; reviews → `11_REVIEWS\Gemini\`
- Systems: Editorial = Premiere · Vault = NAS · Brain = GitHub · Governance = Continuum
- **Voice:** ChatGPT writes · Gemini critiques · Claude executes · Gary approves.

## Acceptance criteria carried on EVERY work order
1. **Reality Test** — could a frame be mistaken for a real film?
2. Faces match master references.
3. Same age across all chapters.
4. Silver pendant present (period-appropriate).
5. No anachronisms in historical chapters.
6. Correct chapter color grade.

---

## Current focus — PHASE 2: PERFORMANCE VALIDATION
**Deliverable: Performance Segment 001 — the Opening Movement** (0:00–0:48.84, Cosmos through Egypt):
`HERO-01 → Motion → HERO-02 → Motion → HERO-03 → Motion → HERO-04`
**Objective:** prove the Performance Anchor methodology produces emotionally believable *motion*. This is the **proof-of-concept for the entire Continuum Creative methodology** — no new eras, no Rome, no new Hero Anchors until it proves out.
- **What we are now testing (editorial disciplines, not image gen):** continuity · pacing · interpolation · emotional timing · camera language · transition philosophy.
- **DONE:** Sam's **Performance Segment Direction PSD-001** (HERO-02→HERO-03, ~12.6 s) delivered 2026-06-28, preserved verbatim, and translated into per-engine motion work orders (`12_Review_Queue/Seq01_PerfSeg001/` — Veo + Grok; Sora retired).
- **STATUS (2026-06-29): ⛔ EP REJECTED BOTH VEO TAKES → Performance Segment 001 returns to RE-ENGINEERING.** The Continuum Render Bridge produced two standard-tier takes and the Gemini GVR re-audit ranked the Trailing-Witness take over the Frontal take — but on EP review (final authority, overriding VFX/Director) **both fail:** emotion does not land in either, and `PS001-VEO_cam.mp4` does not carry the proper faces (back-to-camera). Both archived to `13_Production_History/Seq01_Egypt/` (std→`Camera_Motion/`, cam→`Character_Consistency/`). *The bridge + standard-tier + camera-lever findings remain valid engineering learnings; the takes themselves are rejected.*
- **WITNESS CAMERA — reclassified (Director directive 2026-06-29) from "Standard" to "Witness Camera — Opening Movement Candidate Lesson"** (removed from accepted status; it was drawn from an EP-rejected take). It informs the C1 trailing camera but is not canon.
- **THE GATE NOW (2026-06-29): Sam delivered `PSD-001-R2` → PS001 REBUILT as THREE 4.2 s clips** (OBSERVE / TRIGGER / RECOGNITION), assembled editorially to 12.6 s — *no single continuous render* (the R1 lesson: the Performance Segment is the story unit, the motion clip is the execution unit). Translated to `PS001-R2_ThreeClip_WorkOrder.md`. **NEXT ACTION: generate the new "Performance Keyframes"** (conditioning-still class — NOT Hero Anchors; Nano Banana, **conditioned on the locked CCA face sheets** to fix the R1 face failure), **for Director/EP review BEFORE any Veo render.** Then render 3 clips → Gemini GVR → editorial assembly → EP LOCK. *(Grok not a gate; motion MCP still deferred.)*
- **Foundation already locked:** EDL-001 master clock · CCAs (Gary/Jen) · Egypt costumes · HERO-01→04 anchors · PRO-017 (Anchor → Trajectory → Segment → Finished Sequence).
- **Parallel, independent:** Gemini's **Performance Preservation Pass** (~1K → 4K fidelity on locked frames) — improves fidelity, does not touch story or timeline.

## Renderer roster (canon — `RENDER-BRIDGE-DOCTRINE-001`, 2026-06-29)
- **Primary Motion Renderer = Google Veo 3.1** (PRODUCTION QUALIFIED) — rendered by the Production Supervisor via the **Continuum Render Bridge** (programmatic Gemini API; standard `veo-3.1-generate-preview`).
- **Sora — retired.** **Grok — Creative Motion Consultant** (motion reasoning / prompt / image / critique; **not a renderer** — no production video API).
- **Phase 2 is now Production Pipeline Validation**, not multi-renderer qualification. Review stays multi-agent (Director / Supervisor / VFX / EP) even with one renderer.

## Active blockers
- **B-1 (MOTION) — LARGELY RESOLVED (2026-06-29).** The **Continuum Render Bridge** renders Veo 3.1 image→video end-to-end (repo anchor → render → download → commit; no manual upload). Remaining: Veo's native clip length is ~8 s, so Performance Segments assemble from multiple directed clips in editorial (2C).
- **Identity / costume / runtime / anchors — RESOLVED & LOCKED.** (CCAs, Egypt costumes, EDL-001, HERO-01→04.) Former B-2 (master refs) fully superseded by the locked CCA cast.

## Recent history
- 2026-06-29 — **🎬 PSD-001-R2 (Director) — PS001 rebuilt as a THREE-CLIP edited sequence.** Sam's revised direction: split the 12.6 s into 3 × 4.2 s clips (OBSERVE elevated trailing → TRIGGER front/off-axis pendant + first sight → RECOGNITION Jen answers), each carrying one job; assemble editorially, no single continuous render. New **Performance Keyframe** class introduced (technical CCA-conditioned conditioning stills, not Hero Anchors). Terminology corrected (Nile riverbank not beach; desert hills not mountains). **Witness Camera reclassified** Standard → "Opening Movement Candidate Lesson." Lesson canonized: *the Performance Segment is the story unit; the motion clip is the execution unit.* Translated to `PS001-R2_ThreeClip_WorkOrder.md`; next = generate keyframes for review.
- 2026-06-29 — **⛔ EP REJECTED BOTH PS001 VEO TAKES → re-engineering.** After the GVR re-audit ranked the Trailing-Witness take the winner, the **EP (final authority) rejected both**: emotion doesn't land, and the witness take doesn't carry the proper faces. Both archived to `13_Production_History`. **Witness Camera Standard downgraded to PROPOSED** (establishing take rejected). Next = re-engineer (CCA reference-image conditioning + face-revealing camera + Director on emotion) **or** stand up a motion MCP — EP's call. *(The pipeline/bridge worked end-to-end; the creative result did not meet the bar — the right gate functioned.)*
- 2026-06-29 — **PS001 GVR re-audit (superseded by EP rejection above):** Gemini ranked Trailing-Witness (`PS001-VEO_cam.mp4`, 77) over Frontal (`PS001-VEO_std.mp4`, 53) after the Supervisor caught a first-pass mapping cross-talk via FFmpeg frame extraction. Director had ruled to adopt Witness Camera + "keep the one honest take." *(Retained as provenance; EP review is the governing decision.)*
- 2026-06-29 — **📜 `RENDER-BRIDGE-DOCTRINE-001` ACCEPTED (Studio Doctrine, first-class canon).** Framed by Director Sam, formalized by Production Supervisor, EP-authorized. Distinguishes Studio Methodology from Rendering Technology; promotes the renderer-agnostic **Continuum Render Bridge** to permanent studio architecture. Roster resolved: **Veo 3.1 = Primary Motion Renderer (production-qualified)**; **Sora retired**; **Grok = Creative Motion Consultant (not a renderer)**. Phase 2 reframed → Production Pipeline Validation. PVP-001 superseded-in-part; PS001-GROK closed unrendered.
- 2026-06-29 — **🎬 FIRST MOTION RENDERED — programmatic Veo bridge live.** B-1 motion blocker partially broken: a **Gemini-API Veo bridge** renders image→video end-to-end from the locked anchors (first frame HERO-02, last frame HERO-03) with no manual upload. **PS001-VEO** rendered twice: v1 (`veo-3.1-fast`) drifted identity; **v2 `PS001-VEO_std.mp4` (`veo-3.1-generate-preview`, standard) is PREFERRED** — identity drift resolved, clean/no watermark, reaches the recognition two-shot. **Canon finding: standard Veo 3.1 is the motion setting; Fast caused the drift.** Open objective flag: camera reads frontal→two-shot, not the PSD-001 *trailing witness*. **Grok did NOT deliver a clip** (text confirmation only; self-assessment inadmissible) → 2B A/B benchmark stalled on the Grok side. Veo clip routed for Gemini blind GVR (pending).
- 2026-06-28 — **PSD-001 (Performance Segment Direction) delivered by Sam** (HERO-02→HERO-03, ~12.6 s; 3 shots Observe→Transition→Reveal; camera = witness; "photographed not generated"; Gary changes first). Preserved verbatim; translated into renderer packages + per-engine motion work orders (`12_Review_Queue/Seq01_PerfSeg001/`). Principal photography of motion begun.
- 2026-06-28 — **🎬 EDL-001 CANON LOCKED — PLANNING CLOSED, PRODUCTION BEGINS.** Master runtime allocation (329.60 s across 10 lifetimes + framing) ruled and EP-locked: chorus splits B/A/B, Egypt 29.82 s, Bridge interstitial, finale = editorial-after-rough-cut. Music = immutable master clock. **Phase 2 — Performance Validation** opens; deliverable = Performance Segment 001 (HERO-01→04). Studio shifts from planning org → production org.
- 2026-06-27 — **HERO-04 "The First Smile" LOCKED** (4th anchor) under **PRO-017 — the Performance Anchor Standard** (stills are anchors for motion, not finished moments; Anchor → Trajectory → Segment → Finished Sequence). Director + Gemini GVR-007 (95%) + EP. "Resolution Bridge" renamed **Performance Preservation Pass**.
- 2026-06-27 — **HERO-02 & HERO-03 LOCKED; identity & costume solved.** Identity drift fixed via **Canonical Character Assets** (CCA-001 Gary / CCA-002 Jen) + **Sheet-Based Conditioning**; **Canonical Costume Assets** (Egypt Architect/Scholar) locked. **Creative Provenance** Dossier system + Director Review Packet + public **GitHub Asset Canon** (full production history public) established.
- 2026-06-26 — **PRINCIPAL PHOTOGRAPHY BEGAN.** **CRE-001** (Sam's Sequence One Narrative) authored → canon. **VFX-001** generated the first 3 Egypt hero stills (Gary / Jen / Recognition) via Nano Banana Pro; **VFX-002** retook two of them — Jen hero v2 (removed temple "spectacle," returned to the quiet Nile dawn path Sam directed) and the Recognition two-shot v3 (fixed the look-first/smile-second gaze; removed anachronistic eyeglasses). Selects = **Gary v1 · Jen v2 · Recognition v3**, on NAS `04_Egypt\Stills\`, exposed to the public repo `12_Dailies\Seq01_Egypt\` for Gemini. GVR-001/002/003 queued PENDING; awaiting Director + Gemini + EP review before the Egypt look LOCKs.
- 2026-06-25 — **PRO-005: Gemini onboarded as VFX/Cinematic Review Authority** (Bible §0b team + §0d Charter, ratified by Gemini — review-only). Added **Production Departments** (CRE/VFX/EDL/PRO/CON/REL) + crosswalk; built **`00_PRODUCTION_DASHBOARD.md`** and **`11_REVIEWS\Gemini\`** GVR log. Charter-gate satisfied → Sequence One generation may proceed once B-1 resolved.
- 2026-06-25 — **Director review of TL-WO-003A → ACCEPTED; reframed to SEQUENCE ONE.** Egypt → **Sequence One** (Cosmos→Egypt→Rome, 0:00–1:03.82) = the film's benchmark. **TL-WO-004 issued**; 12 deliverable scaffolds built in `40_SEQUENCES\Seq01_Opening\` (Storyboard spine + Narrative/Environment/Costume/Shot List/Prompt/Review). Canon additions: Bible **§0b roles**, **§0c Three Recognition Rules** (notices first / smiles second / pendant catches light first); Camera Bible **Presence**; Emotional Storyboard **Memory** field. TL-WO-003A superseded.
- 2026-06-25 — **Director review of TL-WO-002 → ACCEPTED.** Rebranded **"A Cinematic Short Film."** Canon Rule gained 4th system (**Continuum = governance history**). New hierarchy layers created: **Emotional Storyboard** + **Transition Bible**; Camera Bible gained **Narrative-Camera language**. **TL-WO-003A issued** (Director's Creative Development — Chapter One/Egypt); Egypt Emotional Storyboard + TS-001 drafted. Generation gated on B-2.
- 2026-06-25 — **TL-WO-002 COMPLETE + public sync.** `MASTER_PRODUCTION_TIMELINE.md` generated (320 words × 14 cols); Canon Rule added to Bible §0a. **TL-WO-003 (b+c) DONE:** doc path-cleanup + public GitHub sync (commit `ab83ee1`, 6 docs + master timeline, zero media). **TL-WO-003 (a) folder restructure DEFERRED** pending Director mapping (EP: use-don't-expand).
- 2026-06-25 — **TL-WO-001 COMPLETED on GSA-1000, EP-LOCKED → PT-0.5.** Section boundaries measured from drums/percussion stems; Premiere markers (24fps), full 320-word Master Timeline, and 66 preliminary line-shots generated to `20_REFERENCE\`. Timeline → **v1.0-draft**; §3 estimates replaced with measured values; Shot DB → v0.2. EP decisions outstanding: fps + chorus chapter-mapping.
- 2026-06-25 — **TL-WO-001 forced alignment EXECUTED on GSA-1000.** ffmpeg + stable-ts installed; `medium.en` align of known lyrics → vocal stem. 320 word timings + 66 line timings written to `20_REFERENCE\alignment\`. Duration confirmed 329.60s.
- 2026-06-24 — Project initialized; folder scaffold built + cleaned; production system v0.1 authored; **restructured to authority-based layout per Director review**; TL-WO-001 issued.
