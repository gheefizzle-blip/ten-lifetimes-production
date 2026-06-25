# TEN LIFETIMES — Production Risk Register

> Every film has one. Over weeks of generating hundreds of assets, this lets us anticipate and manage issues systematically instead of reactively.
> **Owner:** Production Supervisor (Agent B), reviewed by Director. **Updated:** 2026-06-24.

**Scoring:** Probability / Impact = Low · Medium · High · Critical.

| ID | Risk | Prob | Impact | Mitigation | Owner | Status |
|---|---|---|---|---|---|---|
| R-01 | **Character drift** — Gary/Jen stop looking like themselves across chapters | High | High | Locked master references + Nano Banana consistency pass before each chapter; continuity check (`20_REFERENCE\Continuity_Report.md`) every chapter | Supervisor | OPEN |
| R-02 | **Sora visual artifacts** (hands, faces, morphing) | Medium | Medium | Generate alternates; favor stills→subtle motion over full text-to-video for hero shots; reject+log in Render Register | Supervisor | OPEN |
| R-03 | **Historical inaccuracy / anachronisms** | Medium | Low | Period reference review per chapter; acceptance criterion "no anachronisms"; Director QC | Director | OPEN |
| R-04 | **Timeline drift** — edit diverges from the planned sync | Low | High | **Premiere project is source of truth** for the edit; Master Production Timeline locked at v1.0; changes go through Revision Log | Supervisor | OPEN |
| R-05 | **Asset loss / corruption** | Low | Critical | NAS primary (`D:` gary_spear share) + consider Google Drive / second backup of `30_EXPORTS` and master refs; never edit-in-place on originals | EP + Supervisor | OPEN |
| R-06 | **Generation tooling unavailable** — MCPs not reachable from the active CC host | High (now) | High | Confirm MCP host (gheehplaptop vs GSA-1000) + reload; document working config in PROJECT_STATE; until resolved, restrict to planning/alignment work (blocker B-1) | Supervisor | **ACTIVE** |
| R-07 | **Likeness/consent** — using real photos of Gary & Jen | Low | Medium | Both are the subjects and consenting principals; keep refs private to the NAS; no third-party faces | EP | OPEN |
| R-08 | **Scope/time creep** — perfecting one shot stalls the whole film | Medium | Medium | Work-order discipline + Shot Database statuses; "good enough to lock, refine later" passes; the Timeline keeps the big picture | Director | OPEN |
| R-09 | **Audio re-version** — a different master/mix would invalidate word timings | Low | High | Treat current `TEN LIFETIMES.mp3` as locked audio; if remixed, re-run TL-WO-001 alignment before re-editing | EP | OPEN |
| R-10 | **Tone mismatch in the Bridge** — cosmic sequence reads cheesy instead of transcendent | Medium | High | Reference tone (Interstellar/The Fountain/Cloud Atlas); disproportionate iteration budget; Director sign-off on Bridge before Finale | Director | OPEN |

*(Add rows as new risks surface; move to RETIRED when mitigated, don't delete — keep the history.)*
