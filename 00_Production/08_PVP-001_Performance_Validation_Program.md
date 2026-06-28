# TEN LIFETIMES — PVP-001 · Performance Validation Program

> **A laboratory, not a contest.** We do not ask "which AI is best." We ask **"which department (stage) does each engine perform best?"** Every engine receives the *identical* locked input; only the renderer changes. Scoring is **objective** and **blind** (Gemini), against fixed scorecards.

- **Work order:** PVP-001 (Director Sam → EP Gary → Production Supervisor Claude). Issued 2026-06-28. **Phase 2** of production.
- **Does NOT touch EDL-001 / story / timing.** This qualifies *tools*, not content. The master clock, anchors, CCAs, and costumes are all locked and unchanged. No creative changes — ever — within PVP.
- **Constraint (EP):** we benchmark only platforms we actually license — **OpenAI · Google · Anthropic · Suno · xAI/Grok** (Grok pending access confirm). No academic shotgun across engines we won't use in production. This keeps the methodology reproducible by any reasonably-funded studio.
- **Two course-corrections (2026-06-28):** (1) **Anthropic image gen dropped** — not in the production environment; *capability ≠ qualification*; Anthropic remains orchestration. (2) **Grok added as a Motion Candidate** in 2B (Sora · Veo · Grok), no special treatment, must not delay Performance Segment 001.

---

## 1. The model — Stage vs Stage (not Vendor vs Vendor)

We test each pipeline **stage** independently, isolating still-generation from motion-generation so one never confounds the other:

| Phase | Stage | Question | Candidates | Deliverable |
|---|---|---|---|---|
| **2A** | **Anchor Qualification** (still) | *Which engine creates the strongest Performance Anchor?* | Google **Nano Banana** — **incumbent, qualified** (it produced the four locked anchors). No challenger currently in-environment. | **Preferred Anchor Generator = Nano Banana** (current) |
| **2B** | **Renderer Qualification** (image→video, motion) | *Which engine best animates the SAME approved anchor?* | OpenAI **Sora** · Google **Veo** · xAI **Grok** *(if practically available)* — Motion Candidates, none pre-promoted | **Preferred Motion Engine(s) by role** |
| **2C** | **Editorial Qualification** (assembly) | *Can Claude + Gemini preserve performance through the edit?* | Claude (assemble) + Gemini (review) + Premiere | **Performance Segment 001** |

> **Predicted outcome (Director):** no single winner — each engine wins a different stage/role (one "can it perform?", one "can it preserve?", one best at cinematography). The film becomes a **directed orchestration of specialists**, and the renderer becomes incidental. That result is itself a Continuum Creative innovation.

> **Methodology is the constant, not the tool.** The chain `Story → Performance → Character → Costume → Performance Anchor → Performance Trajectory → Performance Segment → Finished Sequence` does not change for any engine. A new capability earns its place by demonstrating value on a *defined task* — never by replacing locked work because it is new. **No locked asset (CCAs, costumes, HERO-01→04, the timeline) is regenerated for PVP.**

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
| **OpenAI Sora** | 2B motion | ❌ No bridge | **Manual web (EP runs).** Claude prepares the identical package; Gemini reviews the clip. |
| **Google Veo** | 2B motion | ❌ No bridge | **Manual web (EP runs).** Same package; Gemini reviews. |
| **xAI Grok** | 2B motion | ❌ No bridge | **Manual web (EP runs)** — *if EP confirms practical access.* Same package; Gemini reviews. |
| **Anthropic image gen** | — | ❌ **Not in environment — NOT pursued** | Director ruling: capability ≠ qualification, and it isn't present in the production environment. **Anthropic stays Production Supervisor / orchestration.** Re-evaluate only if/when a real tool appears, and only on a *future* scene. |
| **OpenAI image gen** | — | ❌ Not present | Not pursued now (Nano Banana is the qualified still engine). |
| **Claude + Gemini + Premiere** | 2C editorial | ✅ Yes (Premiere MCP live) | Claude assembles; Gemini reviews. |

> **Division of labor (Director-confirmed):** *Claude does not generate video.* Claude produces **identical input packages** (prompt, timing, camera, trajectory, output spec); the **EP runs Sora / Veo / Grok on web**; **Gemini scores all, blind, on the same scorecard.** For 2A stills, Nano Banana is the qualified incumbent and Claude runs it directly.

---

## 4. The first benchmark — 2B Renderer Qualification (the near-term work)

**Test a SHORT segment, not the full 48 s** (credit discipline — Director). Recommended benchmark span: **HERO-02 → HERO-03 (~10–15 s)** — enough to evaluate walking, slowing, recognition, eye movement, camera, and pacing without burning credits on the whole Opening Movement. The full HERO-01→04 segment is assembled in 2C only after a renderer is chosen.

**The identical package (every renderer gets exactly this — only the engine changes):**
- **Start anchor:** locked HERO-02 `14_Selected/Seq01/TL-0010_Egypt_TheLongRoad_v3.png`. **End anchor:** locked HERO-03 `14_Selected/Seq01/TL-0070_Egypt_FirstRecognition_v5.png` (image→video conditioning on the locked stills — no new stills).
- **Performance Trajectory, camera direction, runtime, emotional objective:** from **Sam's forthcoming Performance Segment Direction** (the shot-by-shot directing package). Identical across engines.
- **Per-engine syntax packages:** Claude prepares **Package A (Sora), Package B (Veo), Package C (Grok)** — *same direction, different phrasing.* That syntax translation is the Supervisor's job; the direction itself is invariant.
- **Output spec:** 16:9, no eyewear (CD-001), identity/costume/pendant continuity from the anchors.
- **Scoring:** Gemini, **blind** (engines labeled A/B/C), 2B motion scorecard. EP approves.

**Discipline:** if Grok introduces friction/access delay, run **Sora + Veo first**, add Grok in a second cycle — do not let it stall Performance Segment 001. No renderer-specific creative changes; no locked asset regenerated.

**Deferred (contingent):** a future **still-engine** challenger (Anthropic image gen, OpenAI, etc.) is qualified **only if it actually appears in the environment, and only on a future scene not yet in production** — never by re-rolling a locked anchor. Until then Nano Banana is the qualified Anchor Generator.

---

## 5. What the Supervisor needs from the EP

1. **Grok access** — confirm you have practical web access to xAI Grok's image/video generation. If yes, it joins the 2B benchmark as a Motion Candidate; if it adds friction, **Sora + Veo first, Grok in cycle 2** (do not stall Performance Segment 001).
2. **Sora / Veo / Grok = manual-web, EP-run** — confirmed division of labor. I prepare **Packages A (Sora) / B (Veo) / C (Grok)** — same direction, engine-specific syntax; you render on web; **Gemini scores blind**.
3. **Anthropic image gen — CLOSED, no action.** Not pursued: it isn't in the production environment, and *capability ≠ qualification.* Anthropic stays Production Supervisor / orchestration.
4. **True next input = Sam's Performance Segment Direction.** 2B packages encode *his* trajectory / camera / timing; the benchmark can't start until that directing package exists. PVP-001 is staged and waiting on it — not on me.

> No engine is run, and no credits spent, without EP go-ahead per arm.

---

## 6. Gate & sequence

`2A Anchor (Nano Banana, qualified) → 2B Renderer Qualification (Sora · Veo · Grok) → 2C Editorial Qualification → Performance Segment 001`

PVP-001 runs *before* committing hundreds of stills/clips across the ten lifetimes, so every later asset is produced by the measured-best department for its stage. **No EDL-001 timing, story, or anchor changes occur in PVP** — this is pure tool qualification. Sam's **Performance Segment Direction** (the shot-by-shot directing package for 0:00–0:48.84) feeds 2B/2C when motion begins.

> *Author:* Production Supervisor (Claude), translating PVP-001. *Status:* program defined; 2A control + package ready; **awaiting EP on Anthropic access + pilot-target confirm.** Scoring authority: Gemini (blind). Approval: EP.
