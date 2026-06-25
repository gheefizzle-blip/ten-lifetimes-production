# TL-WO-001 (Revised) — Master Timeline Synchronization

- **Authored by:** Director (Sam), 2026-06-24 · captured by Agent B
- **Owner / executor:** Claude Code (Agent B)
- **Status:** IN PROGRESS — **forced alignment EXECUTED on GSA-1000 (2026-06-25).** Steps 1–2 done: duration confirmed 329.60s; `medium.en` align of known lyrics → vocal stem produced `word_timestamps.csv` (320 words), `lines.csv` (66 lines), `.json`, `.srt`, `duration.txt` in `20_REFERENCE\alignment\`. **Remaining:** §3 section boundaries (drums stem) · §4 Premiere markers · §5 Master Production Timeline build · §6 Shot IDs · §7 EP lock v1.0.
- **Gate:** completes → Timeline **v1.0** → Production **PT-0.5**
- **Precondition:** **No image generation begins until this WO is COMPLETE.**

## Objective
Turn the song into a measured backbone: exact word timings, synchronized to the Premiere project, expressed as the Master Production Timeline, with preliminary Shot IDs — then lock Timeline v1.0.

## Inputs
- `D:\My_Music\Tommy Ransome & The Gary Spear Experience\TEN LIFETIMES\TEN LIFETIMES.mp3` (master, 5:29)
- `...\TEN LIFETIMES Stems (1)\` — isolated stems (vocal stem = alignment input; drums stem = section boundaries)
- `20_REFERENCE\Lyrics_Annotated.md` — known transcript (sections S0–S9)
- `...\Ten Lifetimes.prproj` — Premiere project (markers target)

## Steps
1. **Exact duration** — `ffprobe` the master; confirm 329.0s; record in PROJECT_STATE + Timeline.
2. **Forced alignment** — align known lyrics to the **vocal stem** (WhisperX / Montreal Forced Aligner / aeneas) → per-word start/end timestamps.
3. **Section boundaries** — from the **drums/percussion stem** (onset of each chorus/section), confirm/adjust S0–S9 boundaries.
4. **Premiere markers** — generate a marker list (CSV/XML) at each section + key lyric beat; import into the `.prproj` so edit and table agree.
5. **Build the Master Production Timeline** — populate `02_Directors_Timeline.md` §1 (one row per word: Time/Word/Beat/Emotion/Camera/Scene/Shot ID/VFX/Transition), replacing all `~` estimates.
6. **Assign preliminary Shot IDs** — map TL-#### blocks (`03_Shot_Database.md`) onto the measured timeline.
7. **Lock** — set Timeline v1.0; update PROJECT_STATE to PT-0.5; log in Revision Log; route to EP `12_APPROVALS\`.

## Acceptance criteria
- Every lyric word has a measured start time (±~50ms) sourced from the vocal stem, not estimated.
- Section boundaries justified by an audible musical event.
- Premiere markers match the table (single source of truth: Premiere for the edit, this WO for the sync map).
- Master Production Timeline fully populated S1–S9; Shot IDs assigned; v1.0 stamped.

## Blockers / tooling
- Needs a forced aligner + `ffmpeg/ffprobe` + Python. **Not yet confirmed on the active host.** First action: probe what's installed here (gheehplaptop); if absent or too heavy for the 8GB thin-client, run on **GSA-1000** (i9/128GB) and sync results back to the NAS. (Ties to blocker B-1 / Risk R-06, though alignment tooling is separate from the generation MCPs.)

## Deliverables
- Updated `02_Directors_Timeline.md` (v1.0)
- `13_RENDER_LOGS\` n/a · alignment artifacts (word-timestamps CSV/JSON) → `20_REFERENCE\alignment\`
- Premiere marker file → audio/edit folder
- PROJECT_STATE + Revision Log updated
