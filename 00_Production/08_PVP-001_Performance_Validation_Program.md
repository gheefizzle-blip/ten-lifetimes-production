# TEN LIFETIMES — PVP-001 · Performance Validation Program

> **A laboratory, not a contest.** We do not ask "which AI is best." We ask **"which department (stage) does each engine perform best?"** Every engine receives the *identical* locked input; only the renderer changes. Scoring is **objective** and **blind** (Gemini), against fixed scorecards.

- **Work order:** PVP-001 (Director Sam → EP Gary → Production Supervisor Claude). Issued 2026-06-28. **Phase 2** of production.
- **Does NOT touch EDL-001 / story / timing.** This qualifies *tools*, not content. The master clock, anchors, CCAs, and costumes are all locked and unchanged. No creative changes — ever — within PVP.
- **Constraint (EP):** we benchmark only the platforms we actually license — **OpenAI · Google · Anthropic · Suno**. No academic shotgun across engines we won't use in production. This also makes the methodology reproducible by any reasonably-funded studio.

---

## 1. The model — Stage vs Stage (not Vendor vs Vendor)

We test each pipeline **stage** independently, isolating still-generation from motion-generation so one never confounds the other:

| Phase | Stage | Question | Candidates | Deliverable |
|---|---|---|---|---|
| **2A** | **Anchor Qualification** (still) | *Which engine creates the strongest Performance Anchor?* | Google **Nano Banana** (incumbent) · **Anthropic image gen** · OpenAI image gen *(where applicable)* | **Preferred Anchor Generator** |
| **2B** | **Motion Qualification** (image→video) | *Which engine best animates the same approved anchor?* | OpenAI **Sora** vs Google **Veo** | **Preferred Motion Engine(s)** |
| **2C** | **Editorial Qualification** (assembly) | *Can Claude + Gemini preserve performance through the edit?* | Claude (assemble) + Gemini (review) + Premiere | **Performance Segment 001** |

> **Predicted outcome (Director):** no single winner — each engine wins a different stage/role (e.g. one "can it perform?", one "can it preserve?"). The film becomes a **directed orchestration of specialists**, and the renderer becomes incidental. That result is itself a Continuum Creative innovation.

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
| **Google Nano Banana** | 2A still | ✅ **YES** (`mcp__nanobanana__generate_image`) | Claude generates directly. *(The locked HERO anchors already ARE its output — it is the control.)* |
| **Anthropic image gen** | 2A still | ❌ **No tool present** | **Needs access** — see §5. Claude cannot invoke it until a tool/MCP exists or EP runs it on web. |
| **OpenAI image gen** | 2A still | ❌ No tool present | Manual web (EP), or skip. |
| **OpenAI Sora** | 2B motion | ❌ No bridge | **Manual web (EP runs).** Claude prepares the identical package; Gemini reviews the clip. |
| **Google Veo** | 2B motion | ❌ No bridge | **Manual web (EP runs).** Same package; Gemini reviews. |
| **Claude + Gemini + Premiere** | 2C editorial | ✅ Yes (Premiere MCP live) | Claude assembles; Gemini reviews. |

> **Division of labor (Director-confirmed):** *Claude does not generate video.* Claude produces **identical input packages** (prompt, timing, camera, trajectory, output spec); the EP runs Sora/Veo on web; **Gemini scores both, blind, on the same scorecard.** For 2A stills, Claude can run the Nano Banana arm directly; the Anthropic/OpenAI arms need access (§5).

---

## 4. Phase 2A — first pilot (defined; Anthropic arm BLOCKED on access)

**Pilot target:** recreate ONE existing **locked** anchor with a different still engine and compare to the Nano Banana original. **Recommended: HERO-03 "The First Recognition" (TL-0070 v5)** — it is the most diagnostic anchor (two characters, both CCAs, both costumes, the pendant, and recognition eye-line — everything an Anchor Generator must nail at once). *(Simpler alternative: HERO-02 "The Long Road" — single distant figure, lighter identity load.)*

**Identical input package (handoff-ready):**
- **Control (Nano Banana):** the locked frame `14_Selected/Seq01/TL-0070_Egypt_FirstRecognition_v5.png` — no regeneration; it is the reference.
- **Verbatim prompt + negative + params:** from its Dossier `14_Selected/Seq01/TL-0070_Egypt_FirstRecognition_v5.md` (use exactly — no creative changes).
- **Conditioning images (same for every engine):** CCA-001-EGYPT (Gary) + Gary Royal Architect costume sheet + CCA-002-EGYPT (Jen) + Jen Royal Scholar costume sheet, from `00_Identity_Master/` and `00_Costume_Master/Egypt/`.
- **Output spec:** 16:9, full-bleed, no eyewear (CD-001), pendant exposed.
- **Scoring:** Gemini, blind (label A/B only), 2A anchor scorecard.

**Status:** Control ready. **Anthropic arm BLOCKED** pending access (§5). When access exists, Claude (or EP, depending on the access path) runs the Anthropic recreation on the *same* package; Gemini scores A vs B.

**Why this matters before Rome:** the still is the conditioning source for *both* Sora and Veo. A stronger Anchor Generator improves every downstream motion clip and every one of the hundreds of stills across the remaining lifetimes. Measuring this now is high-leverage.

---

## 5. What the Supervisor needs from the EP (to unblock)

1. **Anthropic image generation — access details.** I have no such tool in this environment and cannot confirm the product from my side. Please point me to it: product/API name, a web URL, or an MCP/connector to add. Then I can either (a) bridge it and run the 2A arm directly, or (b) prepare a manual package for you to run, exactly as with Sora/Veo.
2. **Sora & Veo (2B):** confirmed **manual-web, EP-run**. I will prepare two packages — **Package A (Sora syntax)** and **Package B (Veo syntax)** — same direction, different phrasing, once we reach 2B.
3. **2A pilot target:** confirm **HERO-03** (recommended, most diagnostic) vs HERO-02 (lighter).

> Until #1 is resolved, 2A's Anthropic arm cannot run; the Nano Banana control and the input package are ready now. **No engine is run, and no credits spent, without EP go-ahead per arm.**

---

## 6. Gate & sequence

`2A Anchor Qualification → 2B Motion Qualification → 2C Editorial Qualification → Performance Segment 001`

PVP-001 runs *before* committing hundreds of stills/clips across the ten lifetimes, so every later asset is produced by the measured-best department for its stage. **No EDL-001 timing, story, or anchor changes occur in PVP** — this is pure tool qualification. Sam's **Performance Segment Direction** (the shot-by-shot directing package for 0:00–0:48.84) feeds 2B/2C when motion begins.

> *Author:* Production Supervisor (Claude), translating PVP-001. *Status:* program defined; 2A control + package ready; **awaiting EP on Anthropic access + pilot-target confirm.** Scoring authority: Gemini (blind). Approval: EP.
