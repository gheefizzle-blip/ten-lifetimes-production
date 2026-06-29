# TEN LIFETIMES — PVP-001 · Performance Validation Program

> **A laboratory, not a contest.** We do not ask "which AI is best." We ask **"which department (stage) does each engine perform best?"** Every engine receives the *identical* locked input; only the renderer changes. Scoring is **objective** and **blind** (Gemini), against fixed scorecards.

- **Work order:** PVP-001 (Director Sam → EP Gary → Production Supervisor Claude). Issued 2026-06-28. **Phase 2** of production.
- **Does NOT touch EDL-001 / story / timing.** This qualifies *tools*, not content. The master clock, anchors, CCAs, and costumes are all locked and unchanged. No creative changes — ever — within PVP.
- **Constraint (EP):** we benchmark only platforms we actually license — **OpenAI · Google · Anthropic · Suno · xAI/Grok** (Grok pending access confirm). No academic shotgun across engines we won't use in production. This keeps the methodology reproducible by any reasonably-funded studio.
- **Course-corrections (2026-06-28):** (1) **Anthropic image gen dropped** — not in the production environment; *capability ≠ qualification*; Anthropic remains orchestration. (2) **Grok added as a Motion Candidate** in 2B, no special treatment, must not delay Performance Segment 001. (3) **OpenAI Sora REMOVED — product retired** (Sora consumer app shut down 2026; API sunset). *Roster update only — no methodology change; the studio is built on `Anchor → Trajectory → Segment`, which is renderer-independent.*

> **🎬 MOTION DEPARTMENT — current roster.** **Qualified Candidates:** Google **Veo** · xAI **Grok**. **Historical note:** OpenAI **Sora** removed following product retirement (2026). **Future candidates:** any Anthropic motion capability, or any future OpenAI motion platform, *if and when it appears in the production environment* — qualified through the standard **Cultural + Technical** process. The disappearance of a renderer does not stop the studio: it is built on methodology, not a vendor.

---

## 1. The model — Stage vs Stage (not Vendor vs Vendor)

We test each pipeline **stage** independently, isolating still-generation from motion-generation so one never confounds the other:

| Phase | Stage | Question | Candidates | Deliverable |
|---|---|---|---|---|
| **2A** | **Anchor Qualification** (still) | *Which engine creates the strongest Performance Anchor?* | Google **Nano Banana** — **incumbent, qualified** (it produced the four locked anchors). No challenger currently in-environment. | **Preferred Anchor Generator = Nano Banana** (current) |
| **2B** | **Renderer Qualification** (image→video, motion) | *Which engine best animates the SAME approved anchor?* | Google **Veo** · xAI **Grok** — Motion Candidates, none pre-promoted *(OpenAI Sora removed — retired 2026)* | **Preferred Motion Engine(s) by role** |
| **2C** | **Editorial Qualification** (assembly) | *Can Claude + Gemini preserve performance through the edit?* | Claude (assemble) + Gemini (review) + Premiere | **Performance Segment 001** |

> **Predicted outcome (Director):** no single winner — each engine wins a different stage/role (one "can it perform?", one "can it preserve?", one best at cinematography). The film becomes a **directed orchestration of specialists**, and the renderer becomes incidental. That result is itself a Continuum Creative innovation.

> **Methodology is the constant, not the tool.** The chain `Story → Performance → Character → Costume → Performance Anchor → Performance Trajectory → Performance Segment → Finished Sequence` does not change for any engine. A new capability earns its place by demonstrating value on a *defined task* — never by replacing locked work because it is new. **No locked asset (CCAs, costumes, HERO-01→04, the timeline) is regenerated for PVP.**

### Two qualification stages (every candidate department — Director, 2026-06-28)
A department earns its place in **two distinct passes; never conflate them.**
- **Qualification 1 — Cultural.** Does the department understand authority, canon, the Studio Memory, locked assets, and its own lane? (Demonstrated at onboarding by accepting constraints and *declining to act without direction*.)
- **Qualification 2 — Technical.** Can the department actually produce world-class output for its craft? (Demonstrated on the assigned task, scored blind by Gemini.)

| Candidate | Cultural | Technical |
|---|---|---|
| **Grok (Motion)** | ✅ **PASS** (onboarded 2026-06-28 — read the Studio Memory, accepted all locked constraints, declined to render without Director direction) | ⏳ Pending — Performance Segment 001 |
| Veo (Motion) | n/a (EP-operated web tool) | ⏳ Pending — Performance Segment 001 |
| ~~Sora (Motion)~~ | — | **Removed — product retired (2026)** |

> **Lesson recorded (Studio Memory):** *A candidate that declines to generate until it has locked direction is behaving like a professional department, not a chatbot.* Most AI systems begin creating immediately; a professional department waits for the Director. That distinction is a qualification signal in itself.

---

## 2. Scorecards (objective; Gemini scores blind)

**2A — Anchor scorecard** (a still is judged by its value *as a conditioning source for motion*):
| Category | Weight |
|---|---|
| Identity preservation (vs CCAs) | 30% |
| Costume / continuity fidelity | 20% |
| Emotional readability (anchor potential) | 20% |
| Editability (surgical pickups) | 15% |
| Conditioning quality (clean for image→video) | 15% |

**2B — Motion scorecard** (Director-specified):
| Category | Weight |
|---|---|
| Emotional Performance | 30% |
| Identity Preservation | 25% |
| Camera Language | 15% |
| Motion Continuity | 15% |
| Prompt Fidelity | 10% |
| Technical Quality | 5% |

> **Resolution is ≤5% everywhere.** A month ago that would have been unthinkable; it now correctly reflects our priorities (the Performance Preservation Pass handles fidelity separately). Truth and performance outrank pixels.

---

## 3. Execution-access reality (HONEST — what can actually run, and by whom)

This is the gating fact. Only one generator is bridged into the Production Supervisor's environment; the rest are **manual web** (EP-run) or **need access**.

| Engine | Stage | Bridged to Claude? | How it actually runs |
|---|---|---|---|
| **Google Nano Banana** | 2A still | ✅ **YES** (`mcp__nanobanana__generate_image`) | Claude generates directly. The four locked anchors ARE its output — it is the qualified incumbent. |
| **Google Veo** | 2B motion | ❌ No bridge | **Manual web (EP runs).** Claude prepares the identical package; Gemini reviews the clip. |
| ~~OpenAI Sora~~ | 2B motion | — | **REMOVED — product retired (2026).** Re-add only if OpenAI re-enters video and it appears in the environment. |
| **xAI Grok** | 2B motion | ❌ No bridge | **Manual web (EP runs).** ✅ **Access confirmed; onboarded 2026-06-28** (Charter in Project Instructions + Ten Lifetimes Assignment Brief received; read the Studio Memory; standing by, no render until Sam's direction). Same package; Gemini reviews. |
| **Anthropic image gen** | — | ❌ **Not in environment — NOT pursued** | Director ruling: capability ≠ qualification, and it isn't present in the production environment. **Anthropic stays Production Supervisor / orchestration.** Re-evaluate only if/when a real tool appears, and only on a *future* scene. |
| **OpenAI image gen** | — | ❌ Not present | Not pursued now (Nano Banana is the qualified still engine). |
| **Claude + Gemini + Premiere** | 2C editorial | ✅ Yes (Premiere MCP live) | Claude assembles; Gemini reviews. |

> **Division of labor (Director-confirmed):** *Claude does not generate video.* Claude produces **identical input packages** (prompt, timing, camera, trajectory, output spec); the **EP runs Veo + Grok on web**; **Gemini scores both, blind, on the same scorecard.** For 2A stills, Nano Banana is the qualified incumbent and Claude runs it directly.

---

## 4. The first benchmark — 2B Renderer Qualification (the near-term work)

**Test a SHORT segment, not the full 48 s** (credit discipline — Director). Recommended benchmark span: **HERO-02 → HERO-03 (~10–15 s)** — enough to evaluate walking, slowing, recognition, eye movement, camera, and pacing without burning credits on the whole Opening Movement. The full HERO-01→04 segment is assembled in 2C only after a renderer is chosen.

**The identical package (every renderer gets exactly this — only the engine changes):**
- **Start anchor:** locked HERO-02 `14_Selected/Seq01/TL-0010_Egypt_TheLongRoad_v3.png`. **End anchor:** locked HERO-03 `14_Selected/Seq01/TL-0070_Egypt_FirstRecognition_v5.png` (image→video conditioning on the locked stills — no new stills).
- **Performance Trajectory, camera direction, runtime, emotional objective:** from **Sam's forthcoming Performance Segment Direction** (the shot-by-shot directing package). Identical across engines.
- **Per-engine syntax packages:** Claude prepares **Package B (Veo) and Package C (Grok)** — *same direction, different phrasing* (Package A — Sora — retired). That syntax translation is the Supervisor's job; the direction itself is invariant.
- **Output spec:** 16:9, no eyewear (CD-001), identity/costume/pendant continuity from the anchors.
- **Scoring:** Gemini, **blind** (engines labeled A/B), 2B motion scorecard. EP approves.

**Discipline:** no renderer-specific creative changes; no locked asset regenerated. Two candidates remain (Veo, Grok); both have practical access, so the benchmark runs as a single cycle.

**Deferred (contingent):** a future **still-engine** challenger (Anthropic image gen, OpenAI, etc.) is qualified **only if it actually appears in the environment, and only on a future scene not yet in production** — never by re-rolling a locked anchor. Until then Nano Banana is the qualified Anchor Generator.

---

## 5. What the Supervisor needs from the EP

1. **Veo + Grok = manual-web, EP-run** — confirmed division of labor. I prepare **Package B (Veo) and Package C (Grok)** — same direction, engine-specific syntax; you render on web; **Gemini scores blind**.
2. **Sora — retired; no action.** Removed from the roster (OpenAI product retirement). Re-qualify only if OpenAI re-enters video and it appears in the environment.
3. **Anthropic image gen — CLOSED, no action.** Not pursued: it isn't in the production environment, and *capability ≠ qualification.* Anthropic stays Production Supervisor / orchestration.
4. **PSD-001 delivered (2026-06-28).** Sam's Performance Segment Direction is in; packages are translated and ready. The benchmark now waits on the **EP rendering Veo + Grok**.

> No engine is run, and no credits spent, without EP go-ahead per arm.

---

## 6. Gate & sequence

`2A Anchor (Nano Banana, qualified) → 2B Renderer Qualification (Veo · Grok) → 2C Editorial Qualification → Performance Segment 001`

**The 2B render-package pipeline (motion):**
`Director's Performance Segment Direction (emotion) → Director's Shot List (cinematography, timed) → 2 identical packages (Veo/Grok, engine syntax only) → EP renders → Gemini blind score`

**Motion provenance workflow (same as stills — EP, 2026-06-28):** each renderer attempt is an individual, self-contained **motion work order** committed to GitHub (`12_Review_Queue/Seq<NN>_PerfSeg<NNN>/PS<NNN>-<ENGINE>.md`) so the renderer can read it directly AND the **request + result are preserved together** (request born with the file; render settings, blind score, observations, and disposition appended). Lifecycle mirrors stills: Created → render → Gemini GVR (blind) → EP → LOCK → winning clip to `14_Selected/`, others kept in `13_Production_History/`. *No motion clip exists without its work-order Dossier.*
The **Director's Shot List** (`Performance_Segment_001_Shot_List.md`) separates *cinematography* (camera, timed shots) from *emotion* (the Direction), so every renderer receives identical cinematic intent. Format + measurable spine are built; Camera/Performance cells await Sam's Direction.

PVP-001 runs *before* committing hundreds of stills/clips across the ten lifetimes, so every later asset is produced by the measured-best department for its stage. **No EDL-001 timing, story, or anchor changes occur in PVP** — this is pure tool qualification. Sam's **Performance Segment Direction** (the shot-by-shot directing package for 0:00–0:48.84) feeds 2B/2C when motion begins.

> *Author:* Production Supervisor (Claude), translating PVP-001. *Status:* program defined; 2A control + package ready; **awaiting EP on Anthropic access + pilot-target confirm.** Scoring authority: Gemini (blind). Approval: EP.
