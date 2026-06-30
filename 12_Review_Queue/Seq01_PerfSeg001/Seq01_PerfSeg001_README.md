# Performance Segment 001 — Motion Work Orders (Review Queue)

> Individual, self-contained **motion work orders**, one per renderer — the motion equivalent of a still's born-with-it Dossier. Each carries **the request and (later) the result**, preserved on GitHub exactly like a still. Lifecycle mirrors stills: **Created → render → Gemini GVR (blind) → EP → LOCK** → winner to `14_Selected/Seq01/`, others kept in `13_Production_History/Seq01_Egypt/`.

## Segment
- **Performance Segment 001:** HERO-02 "The Long Road" → HERO-03 "The First Recognition" · ~12.6 s
- **Direction (source of truth):** `00_Production/PSD-001_Performance_Segment_Direction_OpeningMovement.md`
- **Cinematography spec:** `00_Production/Performance_Segment_001_Shot_List.md`
- **Audit view (all engines, identical-except-syntax):** `00_Production/Performance_Segment_001_Renderer_Packages.md`

> **Roster (per `RENDER-BRIDGE-DOCTRINE-001`, 2026-06-29):** **Google Veo 3.1 = Primary Motion Renderer (PRODUCTION QUALIFIED)**, rendered by the Production Supervisor via the **Continuum Render Bridge** (programmatic Gemini API). **Sora retired. Grok = Creative Motion Consultant (NOT a renderer** — no production video output path); `PS001-GROK.md` is closed unrendered, retained as provenance.

## Work orders
| Engine | Role | Work order |
|---|---|---|
| **Google Veo 3.1** | **Primary Motion Renderer** | `raw.githubusercontent.com/gheefizzle-blip/ten-lifetimes-production/main/12_Review_Queue/Seq01_PerfSeg001/PS001-VEO.md` |
| xAI Grok | Creative Motion Consultant (not rendered) | `raw.githubusercontent.com/gheefizzle-blip/ten-lifetimes-production/main/12_Review_Queue/Seq01_PerfSeg001/PS001-GROK.md` |
| ~~OpenAI Sora~~ | retired (product retirement 2026) | — no work order |

## Conditioning frames (both engines)
- First/Start = HERO-02: `.../14_Selected/Seq01/TL-0010_Egypt_TheLongRoad_v3.png`
- Last/End = HERO-03: `.../14_Selected/Seq01/TL-0070_Egypt_FirstRecognition_v5.png`

## Status (2026-06-29) — ⛔ EP REJECTED BOTH TAKES → RE-ENGINEERING
**EP (Gary, final authority) reviewed both clips and rejected both**, overriding the VFX/Director promote: emotion does not land in either, and `PS001-VEO_cam.mp4` does not carry the proper faces (back-to-camera framing). Both archived to `13_Production_History/Seq01_Egypt/` (`PS001-VEO_std.mp4` → `Camera_Motion/`; `PS001-VEO_cam.mp4` → `Character_Consistency/`). **Witness Camera Standard downgraded to PROPOSED / under reconciliation** (its establishing take was EP-rejected). **NEXT (EP's open call):** (a) re-engineer — Veo **reference-image conditioning on the CCA face sheets** (untested lever, targets identity) + a face-revealing camera + Director revisits emotion/shot structure; or (b) stand up a proper **motion MCP** (Render Bridge as a first-class tool). **Grok: closed unrendered.** v1 Fast `PS001-VEO.mp4` retained as provenance.
