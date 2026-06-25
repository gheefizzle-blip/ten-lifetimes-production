# TEN LIFETIMES — Revision Log

> Chronological record of significant decisions and changes (not file-level edits).

| Date | Change | Decision by | Doc(s) affected |
|---|---|---|---|
| 2026-06-24 | Project initialized. Root = `D:\My Music\Ten Lifetimes`. Folder scaffold built; typo folders cleaned (`02_Reference__Jen`, `07_Medival`); Jen refs consolidated. Production system v0.1 authored. | EP (Gary) + Agent B | all |
| 2026-06-24 | Director's Timeline built on **Strategy B (music-driven)** v0.1; timecodes flagged estimates pending alignment. | Agent B (for Director) | 02_Directors_Timeline |
| 2026-06-24 | **Director review (PT-0.1).** Reorganized `00_Production` around **authority** (canonical state files at root + evidence subfolders 10–30). Added `00_PROJECT_STATE.md` and `Risk_Register.md`. Reformatted timeline to **Master Production Timeline** (one row/word, 9 cols). Extracted Camera/Character/Style bibles. Issued **TL-WO-001**. Deferred all image generation until timeline locks. | Director (Sam) → Agent B | all |
| 2026-06-24 | Minor deviation logged: canonical filenames kept mixed-case (not ALL-CAPS) to avoid fragile case-only renames on the NAS; folder structure adopted as directed. | Agent B | 11_REVIEWS |
| 2026-06-25 | **TL-WO-001 forced alignment executed on GSA-1000** (ffmpeg + stable-ts `medium.en`). 320 word + 66 line timings written to `20_REFERENCE\alignment\`; duration confirmed 329.60s. WO advanced AUTHORIZED → IN PROGRESS. | Agent B | 00_PROJECT_STATE, 02, TL-WO-001 |
| 2026-06-25 | **Public production repo created** (Director proposal, EP authorized): `gheefizzle-blip/ten-lifetimes-production` (PUBLIC, docs & prompts only). Built from a docs-only tree → guaranteed no media; verified `git ls-files` zero media. License = **All Rights Reserved**. NAS remains the private asset vault. GitHub = public system of record for docs. | Director (Sam) → EP (Gary) → Agent B | repo |
