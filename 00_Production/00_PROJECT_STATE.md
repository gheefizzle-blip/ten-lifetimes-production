# TEN LIFETIMES — A Cinematic Short Film — PROJECT STATE (canonical)

> **The single source of truth for where the production stands.** Read this first.
> Per Director's architecture (2026-06-24): the project is organized around **authority**. These canonical files
> (`00_PROJECT_STATE`, `01_Production_Bible`, `02_Directors_Timeline`, `03_Shot_Database`) hold the state;
> everything else is **evidence supporting** it.

- **🎬 MILESTONE: EDL-001 CANON LOCKED — PLANNING PHASE CLOSED; PRODUCTION BEGINS** (2026-06-28). The master runtime allocation is immutable; the music is the master clock. Four Performance Anchors locked (HERO-01→04). Identity (CCAs) + costumes solved; PRO-017 Performance Anchor methodology validated. **Pre-production is over — the studio is now a production organization.**
- **Phase:** **PRODUCTION — Phase 2: Performance Validation.** Sole deliverable = **Performance Segment 001** (Opening Movement, HERO-01→04). Planning is frozen (runtime/era/chorus/emotional allocation locked — Director's Standing Order). Every hour now moves pixels, not paragraphs.
- **Production version:** **PT-1.0** (planning complete; EDL-001 locked 2026-06-28).
- **Last updated:** 2026-06-28 by Agent B (Production Supervisor) — EDL-001 lock + phase transition; awaiting Sam's Performance Segment Direction.
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
| Motion (Performance Segments) | ⬜ In production (Phase 2) | EDL-001 §7 |
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
- **Awaiting:** Sam's **Performance Segment Direction** (a shot-by-shot directing package for the first 48 s — NOT a still, NOT CRE-007). The Supervisor then translates it into motion prompts / camera direction / editorial pacing / transition timing and runs the motion engine.
- **Foundation already locked:** EDL-001 master clock · CCAs (Gary/Jen) · Egypt costumes · HERO-01→04 anchors · PRO-017 (Anchor → Trajectory → Segment → Finished Sequence).
- **Parallel, independent:** Gemini's **Performance Preservation Pass** (~1K → 4K fidelity on locked frames) — improves fidelity, does not touch story or timeline.

## Active blockers
- **B-1 (MOTION) — THE live blocker for Phase 2.** Stills tooling is solved (Nano Banana MCP: multi-image conditioning, 16:9/4K, grounding). **Motion (Veo / Sora / Runway) has no direct MCP bridge yet** — native web + manual download, then Gemini GVR on the clip. Resolving the motion-generation path is the first practical task of Performance Segment 001. *(Sora ≈ 20 s clip ceiling; plan Performance Segments as 4–8 s directed clips.)*
- **Identity / costume / runtime / anchors — RESOLVED & LOCKED.** (CCAs, Egypt costumes, EDL-001, HERO-01→04.) Former B-2 (master refs) fully superseded by the locked CCA cast.

## Recent history
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
