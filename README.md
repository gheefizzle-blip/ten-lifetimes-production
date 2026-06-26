# Ten Lifetimes — A Cinematic Short Film

## The Production Journal

This repository is the **Production Journal** for *Ten Lifetimes* — a cinematic short film
(a narrative interpretation of the song, not a music video). Every meaningful decision,
completed work order, operation report, review, and approval is recorded here. Read it from
the first commit to the last and you can understand exactly how the film was made.

- **Song:** *Ten Lifetimes* — Tommy Ransome & The Gary Spear Experience
- **Runtime:** 5:29 (329.6s) · **Gate:** PT-0.5 (timeline locked)

## The production team (no overlap)

| Role | System | Owns |
|---|---|---|
| Executive Producer | Gary | Final creative & business approval |
| Director (Creative) | ChatGPT "Sam" | Story, symbolism, emotion, cinematic language |
| Production Supervisor | Claude Code | Work orders, assets, documentation, execution |
| Visual Effects / Review | Gemini | Image/video quality, realism, continuity, Veo optimization |
| Editorial | Premiere + Gary | Timeline assembly and pacing |
| Governance | Continuum | Lineage, reports, approvals, history |

Voice: **ChatGPT writes - Gemini critiques - Claude executes - Gary approves.**

## What lives here vs. what doesn't

The public source of truth for production **documents** — deliberately **no media**.

| In this repo (public) | NOT here (private NAS vault) |
|---|---|
| Bible, timeline, shot DB, master production timeline | Reference photos (Gary / Jen / couple), master refs |
| Work orders, storyboards, prompts (text) | Audio master (`.mp3`), stems (`.wav`) |
| Operation reports, reviews, registers, logs | Premiere projects (`.prproj`), renders |
| Dashboard, revision history | Generated stills / motion / final video |

Media and personal assets stay on the NAS and are excluded by [`.gitignore`](.gitignore).

## Structure (highlights)

```text
00_Production/
  00_PROJECT_STATE.md          Single source of truth for where production stands
  00_PRODUCTION_DASHBOARD.md   At-a-glance status
  01_Production_Bible.md       The constitution (vision, roles, governance, rules)
  02_Directors_Timeline.md     Section map + edit model
  MASTER_PRODUCTION_TIMELINE.md  The foundational relational table (word -> shot -> render)
  03_Shot_Database.md          Every shot (TL-####)
  Emotional_Storyboard.md      What the audience should feel (+ Memory)
  Transition_Bible.md          Named reusable transitions (TS-###)
  Camera_Bible.md / Character_Bible.md / ...
  40_SEQUENCES/Seq01_Opening/  Sequence One creative-development scaffolds
  11_REVIEWS/Gemini/           Gemini video/continuity reviews (GVR)
11_Operation_Reports/          Public completion report per operation (PRO-006 standard)
60_Templates/                  Operation report template
```

## How work flows

`Director (ChatGPT) -> Production (Claude Code) -> Generation -> Gemini Review -> EP Approval -> Canon`

Every operation produces a completion report in `11_Operation_Reports/` so all collaborators
share one machine-readable production memory.

## License

All rights reserved. See [`LICENSE`](LICENSE). Contents — including the song lyrics and the
Production Bible — are copyrighted creative works and may not be reused without permission.
