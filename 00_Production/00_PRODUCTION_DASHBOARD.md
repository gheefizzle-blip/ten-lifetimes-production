# TEN LIFETIMES — Production Dashboard

> One-glance status. Maintained by the Production Supervisor. Updated 2026-06-25. Format per Gemini (PRO-005); status reported to actual state. Canonical detail: `00_PROJECT_STATE.md`.

## Production gate: **PT-0.5** (timeline locked) → next PT-1.0

## Sequence Status
```
Sequence One (Opening: Cosmos → Egypt → Rome, 0:00–1:03.82)
██░░░░░░░░  ~15%  — planning SCAFFOLDED; awaiting Director authoring
Sequence Two
░░░░░░░░░░   0%   — not yet defined by Director
Sequence Three
░░░░░░░░░░   0%   — not yet defined by Director
```
> ⚠️ Correction vs draft dashboard: Sequence One planning is **scaffolded, not complete** — the creative cells of TL-WO-004 are still the Director's to author. "Complete" applies only to the measured backbone.

## Sequence One — Generation Progress
| Department | Progress | Status |
|---|---|---|
| **Story & Direction** (CRE / TL-WO-004) | ██░░░░░░░░ | Scaffolded — **awaiting Director authoring** |
| **Prompts** (VFX) | ░░░░░░░░░░ | Pending — gated by **B-1** + authoring |
| **Stills (Hero/Style)** (VFX) | ░░░░░░░░░░ | Pending |
| **Motion Generation** (VFX) | ░░░░░░░░░░ | Pending |
| **Gemini Dailies (GVR)** | ░░░░░░░░░░ | Pending — reviewer ready (Bible §0d) |
| **EP Final Approval** | ░░░░░░░░░░ | Pending |

## Film-wide pipeline
```
Story / Bible        ████████░░  ~85%
Production System    ██████████  100%
Music Synchronization██████████  100%
Editorial Timeline   ██████████  100%  (v1.0 LOCKED, fps 24)
Creative Direction   ██░░░░░░░░  ~20%  (Seq One scaffolded)
Prompts / Stills / Motion / Review  ░░░░░░░░░░  0%
```

## Blockers
- **B-1** — PARTIALLY RESOLVED. **Stills: Nano Banana MCP bridge LIVE on GSA-1000** (multi-image conditioning, 16:9 4K, grounding) — stills tooling-unblocked. **Motion (Veo/Sora): no direct bridge** → native web + download, then Gemini GVR. Remaining gate for stills = Director authoring + workflow approval.
- **B-2** — RESOLVED (interim master refs locked; fresh portrait set recommended before final renders).

## Team (Bible §0b / §0d)
EP (Gary) · Director (ChatGPT/Sam) · Supervisor (Claude Code) · **VFX/Review (Gemini)** · Editorial (Premiere) · Vault (NAS) · Brain (GitHub) · Governance (Continuum)
Voice: **ChatGPT writes · Gemini critiques · Claude executes · Gary approves.**
