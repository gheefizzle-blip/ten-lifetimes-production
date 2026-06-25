# Ten Lifetimes — Production

Public **production brain** for *Ten Lifetimes*, a cinematic AI music video / short film.

- **Song:** *Ten Lifetimes* — Tommy Ransome & The Gary Spear Experience
- **Runtime:** 5:29 (329.6s) · **Version:** PT-0.1 (planning)
- **Executive Producer / final authority:** Gary Spear
- **Director (vision):** ChatGPT "Sam"
- **Production Supervisor (execution):** Claude Code (Agent B)

## What lives here vs. what doesn't

This repository is the **public source of truth for production documents and prompts** — the
planning brain that all collaborators can read. It deliberately contains **no media**.

| In this repo (public) | NOT in this repo (private asset vault on NAS) |
|---|---|
| Production docs, bible, timeline, shot DB | Reference photos (Gary / Jen / couple) |
| Work orders, prompts, storyboards (text) | Audio master (`.mp3`), stems (`.wav`) |
| Continuity reports, registers, logs | Premiere projects (`.prproj`), renders (`.mp4`/`.mov`) |
| Edit decision lists, revision logs | Generated stills / motion / final video assets |

Personal photos, audio masters, stems, Premiere files, and generated video assets stay on the
NAS asset vault and are excluded by [`.gitignore`](.gitignore). The repo is built from a
docs-only tree, so no media is ever staged.

## Structure

```text
00_Production/            Canonical state docs (the constitution + live state)
  00_PROJECT_STATE.md     Single source of truth for where the production stands
  01_Production_Bible.md  Creative decisions (the constitution)
  02_Directors_Timeline.md  Master Production Timeline (word -> beat/camera/scene/shot)
  03_Shot_Database.md     Every shot (TL-####)
  04_Work_Order_Log.md    Index of work orders
  05_Asset_Register.md    Asset inventory (pointers, not the assets)
  06_Render_Register.md   Render log
  07_Revision_Log.md      Major decisions
  08_Continuity_Report.md Continuity tracking
  09_Edit_Decision_List.md  EDL
  Lyrics_Annotated.md     Annotated lyric transcript (sections S0-S9)
10_Work_Orders/           TL-WO-### work order specs
20_Prompts/               Generation prompts (text)
30_Public_Storyboard/     Shareable storyboard (text / links)
40_Continuity_Reports/    Per-chapter continuity reports
```

## Roles & flow

Director (Sam) authors work orders → Production Supervisor (Claude Code / Agent B) executes and
maintains state → Executive Producer (Gary) approves → approved decisions become canon.

## License

All rights reserved. See [`LICENSE`](LICENSE). The contents — including the song lyrics and the
Production Bible — are copyrighted creative works and may not be reused without permission.
