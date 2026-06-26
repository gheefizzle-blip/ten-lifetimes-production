# TEN LIFETIMES — PROJECT STATE (canonical)

> **The single source of truth for where the production stands.** Read this first.
> Per Director's architecture (2026-06-24): the project is organized around **authority**. These canonical files
> (`00_PROJECT_STATE`, `01_Production_Bible`, `02_Directors_Timeline`, `03_Shot_Database`) hold the state;
> everything else is **evidence supporting** it.

- **Production version:** **PT-0.5** (timeline locked, 2026-06-25) → next gate PT-1.0 (story/characters/picture)
- **Last updated:** 2026-06-25 by Agent B (Production Supervisor)
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
- `01_Production_Bible.md` — the constitution (creative decisions only) · **§0a Canon Rule = systems of truth**
- `MASTER_PRODUCTION_TIMELINE.md` — **THE foundational relational artifact** (TL-WO-002): every word → time/section/chapter/shot/prompt/render/clip/status. Effectively immutable; everything downstream references it.
- `02_Directors_Timeline.md` — narrative/structural timeline (section map, edit model, decisions) feeding the master table
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

## Roles
- **EP / final authority:** Gary Spear — approvals land in `12_APPROVALS\`
- **Director:** ChatGPT "Sam" — authors work orders, reviews land in `11_REVIEWS\`
- **Production Supervisor:** Claude Code (Agent B) — executes work orders, maintains state

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

**Next focus (toward PT-1.0):**
1. **Director (Sam):** detail line-level chorus chapter-splits (Rome/Viking in S3, Frontier/Victorian in S6, WWII/Modern/Finale in S8) + fill the Beat/Emotion/Camera/VFX/Transition columns of the Master Timeline.
2. **Master references** (blocker B-2) — select `16_Master_References\` so consistency work can begin.
3. Resolve generation-tooling host (blocker B-1) before any image generation.

## Active blockers
- **B-1 — Generation tooling not reachable from this CC session.** Only Playwright MCP is connected (gheehplaptop). Nano Banana / Sora / Veo bridges not visible. Confirm host (gheehplaptop vs GSA-1000) + reload. *Does not block TL-WO-001 docs/alignment.*
- **B-2 — Master references not selected.** All consistency work provisional until `16_Master_References\` chosen.

## Recent history
- 2026-06-25 — **TL-WO-002 COMPLETE + public sync.** `MASTER_PRODUCTION_TIMELINE.md` generated (320 words × 14 cols); Canon Rule added to Bible §0a. **TL-WO-003 (b+c) DONE:** doc path-cleanup + public GitHub sync (commit `ab83ee1`, 6 docs + master timeline, zero media). **TL-WO-003 (a) folder restructure DEFERRED** pending Director mapping (EP: use-don't-expand).
- 2026-06-25 — **TL-WO-001 COMPLETED on GSA-1000, EP-LOCKED → PT-0.5.** Section boundaries measured from drums/percussion stems; Premiere markers (24fps), full 320-word Master Timeline, and 66 preliminary line-shots generated to `20_REFERENCE\`. Timeline → **v1.0-draft**; §3 estimates replaced with measured values; Shot DB → v0.2. EP decisions outstanding: fps + chorus chapter-mapping.
- 2026-06-25 — **TL-WO-001 forced alignment EXECUTED on GSA-1000.** ffmpeg + stable-ts installed; `medium.en` align of known lyrics → vocal stem. 320 word timings + 66 line timings written to `20_REFERENCE\alignment\`. Duration confirmed 329.60s.
- 2026-06-24 — Project initialized; folder scaffold built + cleaned; production system v0.1 authored; **restructured to authority-based layout per Director review**; TL-WO-001 issued.
