# TEN LIFETIMES — A Cinematic Short Film — PROJECT STATE (canonical)

> **The single source of truth for where the production stands.** Read this first.
> Per Director's architecture (2026-06-24): the project is organized around **authority**. These canonical files
> (`00_PROJECT_STATE`, `01_Production_Bible`, `02_Directors_Timeline`, `03_Shot_Database`) hold the state;
> everything else is **evidence supporting** it.

- **🎬 MILESTONE: PRINCIPAL PHOTOGRAPHY BEGUN** (2026-06-26). **The film has started.** CRE-001 (Sam's Sequence One Narrative) authored; first Egypt hero stills generated, registered, and exposed for review. Studio fully operational (governance/roles frozen · production + Gemini-GVR + documentation pipelines operational · generation tooling live for stills).
- **Phase:** **CREATIVE PRODUCTION** (infrastructure frozen 2026-06-25 — see Bible §0g, The Director's Rule). Creative work is the default; infra changes need a demonstrated production problem or measurable film-quality gain.
- **Production version:** **PT-0.5** (timeline locked, 2026-06-25) → next gate PT-1.0 (story/characters/picture)
- **Last updated:** 2026-06-26 by Agent B (Production Supervisor) — CRE-001 + VFX-001/002 hero stills (Seq One Egypt), awaiting GVR/EP review
- **Public docs repo (system of record for docs/prompts):** `gheefizzle-blip/ten-lifetimes-production` (GitHub, PUBLIC, docs only — **no media**). NAS = private asset vault. Claude Code pushes doc updates.

---

## Lock status (gates → PT-1.0)

| Element | Locked? | Gate doc |
|---|---|---|
| Audio (master delivered) | ✅ Yes | `TEN LIFETIMES.mp3` |
| Story / synopsis | ⬜ Draft (Bible v0.1) | 01_Production_Bible |
| **Timeline v1.0** | ✅ **LOCKED** (EP, 2026-06-25; fps=24) — TL-WO-001 | 02_Directors_Timeline |
| Characters (master refs) | ⬜ Not selected | 23_CHARACTER_BIBLE |
| Picture | ⬜ No | — |
| Color | ⬜ No | 21_STYLE_GUIDES |

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

## Current focus
**TL-WO-001 — Master Timeline Synchronization.** Vocal stem = `...\TEN LIFETIMES Stems (1)\0 Lead Vocals.wav`.
**✅ FORCED ALIGNMENT EXECUTED on GSA-1000 (2026-06-25)** — a Claude Code session on GSA-1000 installed ffmpeg + stable-ts and ran `align_ten_lifetimes.py --model medium.en`. Artifacts in `20_REFERENCE\alignment\`: `word_timestamps.csv` (**320 words**, measured start/end), `lines.csv` (66 lyric lines), `word_timestamps.json`, `ten_lifetimes.srt`, `duration.txt` (**329.60s** confirmed). First sung word 0:19.02; last word ("mine") ends 5:15.57.
**✅ TL-WO-001 EXECUTION COMPLETE (2026-06-25) — awaiting EP lock.** All remaining steps done on GSA-1000:
- **Section boundaries MEASURED** — drums + percussion stems (RMS envelope) cross-checked vs alignment lyric anchors. Drums silent until ~1:45, DROP for bridge 3:20→3:48.3, crash back 3:48.3 (cleanest boundary), fade ~5:01. → `20_REFERENCE\Section_Map_Measured.md` and §3 of the Timeline (estimates replaced).
- **Premiere markers** — `20_REFERENCE\premiere_markers.csv` (16 markers @ 24fps: 10 sections + 6 key drum events).
- **Master Production Timeline** — full 320-word measured table → `20_REFERENCE\master_timeline_words.md` (Time/Word/Section/Chapter/Shot ID locked; creative columns = Director).
- **Preliminary Shot IDs** — 66 line-shots TL-0010–TL-0660 + 3 intro → `20_REFERENCE\shot_database_prelim.md`; Shot DB allocation table updated to measured ranges.

**✅ TIMELINE v1.0 LOCKED by EP (Gary) 2026-06-25 → PT-0.5.** fps = **24** confirmed; chapter overlay approved as-is. TL-WO-001 CLOSED.

**Active focus — TL-WO-004: PERFECT SEQUENCE ONE** (0:00.000–1:03.820 · Cosmos→Egypt→Rome) — the benchmark for the whole film. *"Don't generate Egypt — perfect Sequence One."*
1. **✅ CRE-001 AUTHORED (Sam, 2026-06-26)** — Sequence One Director's Narrative is canon in `40_SEQUENCES\Seq01_Opening\Sequence_One_Narrative.md` (recognition over history; "Love existed before memory"). Supervisor preserved verbatim; translates → prompts/cameras/lighting (does not edit).
2. **✅ VFX-001 + VFX-002 — Egypt hero stills generated.** Three select frames on NAS `04_Egypt\Stills\`: **Gary hero v1**, **Jen hero v2** (retake — quiet Nile path, spectacle removed), **Recognition two-shot v3** (retake — gaze choreography fixed, anachronistic glasses removed). **→ Now at Production Loop step 2–4: awaiting Director review + Gemini GVR-001/002/003 + EP approval → then LOCK the Egypt visual language** before supporting stills.
3. **✅ Master refs LOCKED (interim)** in `16_Master_References\` (B-2 resolved). *Recommended:* fresh purpose-shot portrait set before final renders.
4. **B-1 (stills) RESOLVED** — Nano Banana MCP live (pro/4K, multi-ref conditioning, grounding); output → chapter NAS `Stills\`. **Motion (Veo/Sora) still unbridged.**
5. (Parallel, low-priority) Director: line-level chorus chapter-splits + fill Master Timeline creative columns.

## Active blockers
- **B-1 — PARTIALLY RESOLVED (2026-06-25, GSA-1000).** **Stills: Nano Banana MCP bridge is LIVE** in the CC session (`mcp__nanobanana__generate_image`) — verified responsive; supports **multi-image conditioning (≤3 inputs = our 3 master refs), 16:9/21:9, 4K, Google-Search grounding**. Output → `C:\Users\Gary\nanobanana-images`. Premiere Pro MCP also live (markers/assembly). **Still open: Veo/Sora (motion)** — no direct bridge; native web + manual download (or future n8n route), then Gemini GVR. *Stills generation is now tooling-unblocked; remaining gate = Director authoring + workflow approval.*
- **B-2 — RESOLVED (interim, 2026-06-25).** Master set locked in `16_Master_References\` (3 Gary + 3 Jen, from existing snapshots). Generation unblocked. *Residual:* interim set is casual snapshots — a purpose-shot portrait set recommended before final-quality renders (strip Gary cap/glasses, Jen dyed hair/nose ring per Character Bible).

## Recent history
- 2026-06-26 — **PRINCIPAL PHOTOGRAPHY BEGAN.** **CRE-001** (Sam's Sequence One Narrative) authored → canon. **VFX-001** generated the first 3 Egypt hero stills (Gary / Jen / Recognition) via Nano Banana Pro; **VFX-002** retook two of them — Jen hero v2 (removed temple "spectacle," returned to the quiet Nile dawn path Sam directed) and the Recognition two-shot v3 (fixed the look-first/smile-second gaze; removed anachronistic eyeglasses). Selects = **Gary v1 · Jen v2 · Recognition v3**, on NAS `04_Egypt\Stills\`, exposed to the public repo `12_Dailies\Seq01_Egypt\` for Gemini. GVR-001/002/003 queued PENDING; awaiting Director + Gemini + EP review before the Egypt look LOCKs.
- 2026-06-25 — **PRO-005: Gemini onboarded as VFX/Cinematic Review Authority** (Bible §0b team + §0d Charter, ratified by Gemini — review-only). Added **Production Departments** (CRE/VFX/EDL/PRO/CON/REL) + crosswalk; built **`00_PRODUCTION_DASHBOARD.md`** and **`11_REVIEWS\Gemini\`** GVR log. Charter-gate satisfied → Sequence One generation may proceed once B-1 resolved.
- 2026-06-25 — **Director review of TL-WO-003A → ACCEPTED; reframed to SEQUENCE ONE.** Egypt → **Sequence One** (Cosmos→Egypt→Rome, 0:00–1:03.82) = the film's benchmark. **TL-WO-004 issued**; 12 deliverable scaffolds built in `40_SEQUENCES\Seq01_Opening\` (Storyboard spine + Narrative/Environment/Costume/Shot List/Prompt/Review). Canon additions: Bible **§0b roles**, **§0c Three Recognition Rules** (notices first / smiles second / pendant catches light first); Camera Bible **Presence**; Emotional Storyboard **Memory** field. TL-WO-003A superseded.
- 2026-06-25 — **Director review of TL-WO-002 → ACCEPTED.** Rebranded **"A Cinematic Short Film."** Canon Rule gained 4th system (**Continuum = governance history**). New hierarchy layers created: **Emotional Storyboard** + **Transition Bible**; Camera Bible gained **Narrative-Camera language**. **TL-WO-003A issued** (Director's Creative Development — Chapter One/Egypt); Egypt Emotional Storyboard + TS-001 drafted. Generation gated on B-2.
- 2026-06-25 — **TL-WO-002 COMPLETE + public sync.** `MASTER_PRODUCTION_TIMELINE.md` generated (320 words × 14 cols); Canon Rule added to Bible §0a. **TL-WO-003 (b+c) DONE:** doc path-cleanup + public GitHub sync (commit `ab83ee1`, 6 docs + master timeline, zero media). **TL-WO-003 (a) folder restructure DEFERRED** pending Director mapping (EP: use-don't-expand).
- 2026-06-25 — **TL-WO-001 COMPLETED on GSA-1000, EP-LOCKED → PT-0.5.** Section boundaries measured from drums/percussion stems; Premiere markers (24fps), full 320-word Master Timeline, and 66 preliminary line-shots generated to `20_REFERENCE\`. Timeline → **v1.0-draft**; §3 estimates replaced with measured values; Shot DB → v0.2. EP decisions outstanding: fps + chorus chapter-mapping.
- 2026-06-25 — **TL-WO-001 forced alignment EXECUTED on GSA-1000.** ffmpeg + stable-ts installed; `medium.en` align of known lyrics → vocal stem. 320 word timings + 66 line timings written to `20_REFERENCE\alignment\`. Duration confirmed 329.60s.
- 2026-06-24 — Project initialized; folder scaffold built + cleaned; production system v0.1 authored; **restructured to authority-based layout per Director review**; TL-WO-001 issued.
