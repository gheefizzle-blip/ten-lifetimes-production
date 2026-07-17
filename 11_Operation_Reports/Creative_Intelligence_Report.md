# TEN LIFETIMES — Creative Intelligence Report

> **Auto-generated analytics over the Creative Provenance Dossiers** (not a governance doc; does not trip the Director's Rule). Regenerate on cadence — target **weekly** — by re-reading every `*.md` Dossier across all GitHub stage folders: `12_Review_Queue/`, `12_Dailies/`, `13_Production_History/`, `14_Selected/`, `15_Final/`.

- Generated: 2026-07-17 (instance #5 — weekly regen; corpus unchanged from #4; 7 open items carried forward)
- Corpus: **22 Dossiers** (17 stills + 5 motion), 1 sequence (Sequence One), 2 chapters (Cosmos, Egypt), 1 performance segment (PS001). Sample is growing — read trends as directional, not statistical.
- Coverage: 4 Selected/LOCKED stills · 3 Dailies stills (GVR pending) · 5 motion dossiers (3 clips cleared/locked for assembly) · 10 Production_History stills (8 archived, 2 superseded).

---

## Pipeline Snapshot

| Stage | Stills | Motion | Notes |
|---|---|---|---|
| **Review Queue** (`12_Review_Queue`) | 0 | 5 | C1 (92/100, cleared for assembly) · C2 (100/100, locked) · C3 (89/100, accepted) · PS001-VEO (EP-rejected, clips archived within dossier) · PS001-GROK (qualification closed — no video output path) |
| **Dailies** (`12_Dailies`) | 3 | 0 | Gary_hero_v1 · Jen_hero_v2 · Recognition_v3 — marked Selected in dossiers; GVR-001/002/003 pending |
| **Production History** (`13_Production_History`) | 10 | 0* | 8 archived (continuity failures), 2 superseded (authorized single-image pickups) |
| **Selected / LOCKED** (`14_Selected`) | 4 | 0 | HERO-01 v2 · HERO-02 v3 · HERO-03 v5 · HERO-04 v2 |
| **Final** (`15_Final`) | 0 | 0 | None yet |

*PS001-VEO's two archived clips are recorded within that single dossier, not as separate Production_History files.

Full PS001 segment (12.6 s = C1+C2+C3) is pending editorial assembly → EP LOCK. C2 and C3 are locked; C1 is cleared for assembly with a 4.2 s front-window editorial trim. No new dossiers since instance #4 (2026-07-10).

---

## Top Prompt Improvements

### Stills

| Change | From → To | Effect |
|---|---|---|
| Added explicit gaze geometry: "he looks DIRECTLY AT the woman", "connected by a direct eye-line", negatives for "both looking at camera / looking away from each other / man smiling" | TL-Seq1_Egypt_Recognition_v1 → v2 | Fixed side-by-side default staging; recognition beat lands as intended |
| Added `glasses, eyeglasses, spectacles, eyewear` negatives + conditioned on bare-face master ref (Gary_Master_02_Bareface) | TL-Seq1_Egypt_Recognition_v2 → v3 | Removed anachronistic eyeglasses; historical immersion restored (CD-001) |
| Added quiet-Nile-path positive description + temple/spectacle negatives (`grand temple, Karnak, towering columns, hypostyle hall, pyramids, crowds, spectacle, monuments`) | TL-Seq1_Egypt_Jen_hero_v1 → v2 | Removed temple-spectacle drift; returned environment to Director's quiet-path Intent |
| Added `border, black border, picture frame, rounded corners, vignette frame, matte, inset image, letterbox bars` negatives + "full-bleed edge to edge" positive | TL-0001_Cosmos_BeforeTime_v1 → v2 | Fixed rounded-corner border/matte artifact; clean full-bleed cinematic frame |
| Pulled camera extreme-wide; figure SMALL and OFF-CENTER; dropped all frontal face refs; negatives added `centered subject, large figure, prominent person, profile portrait, standing still, posing` | TL-0010_Egypt_TheLongRoad_v1 → v2 → v3 (two iterations) | "Observational accompaniment" framing achieved on third attempt — merely "wide + from behind" is not enough if the subject is still centered |
| Switched to Sheet-Based Conditioning (CCA × locked costume sheets); dropped selfie refs entirely; one-direction identity rule enforced | TL-0070_Egypt_FirstRecognition_v1/v2 → v3 → v4/v5 | Selfie-era face drift eliminated; both identities now match CCAs exactly |
| Single-image pickup: exposed silver pendant outside collar, catching light — all else frozen | TL-0070_Egypt_FirstRecognition_v4 → v5 | CRE-004 pendant motif now visible without reopening identity, staging, or composition |
| Single-image edit: rebalanced expressions so Gary's gentle smile leads, Jen's is the smaller echo | TL-0080_Egypt_FirstSmile_v1 → v2 | Asymmetry restored (Gary first/stronger); HERO-04 locked at GVR 95% |

### Motion (PS001 family)

| Change | From → To | Effect |
|---|---|---|
| Veo model: Fast tier → Standard tier (`veo-3.1-fast` → `veo-3.1-generate-preview`) | PS001-VEO v1 → v2 | Identity drift (age/hair jump on Gary) resolved; Standard tier is the production motion baseline |
| First-frame-only conditioning (drop last frame); explicit trailing-witness camera; frontal/facing added to negatives | PS001-VEO v2 → v3 | Camera deviation resolved (trailing-from-behind achieved); face not visible — camera/face tension documented for editorial |
| Rebuilt as three 4.2 s clips (Observe/Trigger/Recognition); new keyframes conditioned on locked CCA turnarounds + HERO-02 as shared environment anchor | PS001-VEO EP rejection → PS001R2 three-clip rebuild | Identity carried end-to-end; one storytelling job per clip; pendant/shoreline/costume consistent across all three |
| First-frame-only + free trailing camera for C1 (dropped far end-keyframe); ghost/dissolve/duplicate added to negatives | PS001R2-C1 initial ghost (55/100) → stabilization re-roll (92/100) | Cross-dissolve ghost eliminated; 4.2 s editorial trim handles faint residual |
| Extended negatives: `snail/pendant/amulet/medallion/spiral/silver pendant on the woman`, `duplicate pendant`; positive clause "ONLY THE MAN wears the silver snail pendant" | PS001R2-C3 pendant-migration → pendant-migration fix | Snail migration onto Jen eliminated end-to-end |
| Static OTS anchor (first-frame-only, static camera, OTS keyframe built from turnarounds) replacing camera arc with two far-apart keyframes | PS001R2-C3 arc re-renders (42/100) → stabilization re-roll (89/100) | Cross-dissolve ghosting eliminated; identity rock-solid (GVR Identity 25/25); EP accepted |

---

## Most Common Continuity Errors

*Grouped by category, archived in `13_Production_History/`. Counts reflect all archived dossiers (still and motion).*

| Category | Count | Severity | Preventable? | Root Cause summary | CD-### |
|---|---|---|---|---|---|
| **Composition / Staging** | 3 | Major / Moderate | PARTIALLY | (a) Gaze geometry unstated → side-by-side staging (Recognition_v1); (b) subject scale under-specified → two iterations to achieve "world larger than man" (Long Road v1/v2); (c) two far-apart Veo keyframes on a camera arc → cross-dissolve ghost (C3 arc version, 42/100) | n/a — corrective rules in Prompt Package |
| **Character_Consistency** | 3 | Major | YES | (a) Selfie-era face drift (HERO-03 v1 — selfies instead of CCAs); (b) CCA-only, pre-costume/asymmetry intermediate superseded by full CCA×Costume regen (HERO-03 v3); (c) Veo Fast tier → identity drift across clip (PS001-VEO v1, age/hair jump) | Sheet-Based Conditioning; Standard Veo tier |
| **Historical_Continuity** | 1 | Moderate | YES | Modern eyeglasses carried from reference photos into ancient-Egypt frame; negative prompt did not suppress eyewear | **CD-001** |
| **Environment** | 1 | Major | YES | Under-constrained environment + "temple scholar" role phrasing → model defaulted to Karnak-scale monumental setting | n/a — environment positive+negative rule |
| **Rendering_Artifact** | 1 | Minor | YES | "First frame of a film" phrasing without border suppression → rounded-corner border/matte inset instead of full-bleed | n/a — standing border/matte negatives |
| **Camera_Motion** | 1 | Critical | YES | Frontal first+last frame conditioning → Veo rendered frontal two-shot instead of directed trailing witness; GVR rated camera 5/15 CRITICAL FAIL | First-frame-only for moving cameras; RENDER-BRIDGE-DOCTRINE-001 |
| **Prop Continuity** | 1 | Major | YES | Pendant negative applied only to Gary's prompt; Veo migrated the silver snail onto Jen's collar mid-clip | Extend prop negatives to ALL characters who should NOT carry that prop |

> Two stills in `13_Production_History/Superseded/` (HERO-03 v4, HERO-04 v1) were superseded by authorized single-image pickups/edits — intentional incremental refinements, not continuity failures; not counted in the table above.

---

## Highest-Rated Intent Matches

*Selected and Locked assets only, ranked by Gemini emotional-vs-Intent score.*

| Asset | Shot | Intent | GVR Score | Notes |
|---|---|---|---|---|
| **PS001R2-C2 `TRIGGER`** | PS001 Clip 2 | Ordinary world breaks by one tiny detail | **100/100** | Emotional 30/30 · Identity 25/25 · Camera 15/15 · Motion 15/15 · Fidelity 10/10 · Technical 5/5. "The execution of the pendant glint, the most difficult element, was flawless." |
| **TL-0080_Egypt_FirstSmile_v2 (HERO-04)** | TL-0080 | First emotional release — HOPE, very quiet | **95%** | GVR-007: Identity 99% / Staging 96% / Emotional Potential 98%. "Resists over-polish." Locked as Performance Anchor (PRO-017). |
| **PS001R2-C1 `OBSERVE`** | PS001 Clip 1 | Isolation & scale — history following him | **92/100** | Emotional 30/30 · Identity 24/25 · Camera 15/15 · Motion 8/15 (faint residual cleared by 4.2 s editorial trim). Cleared for PS001 assembly. |
| **PS001R2-C3 `RECOGNITION`** | PS001 Clip 3 | Mutual but asymmetrical recognition | **89/100** | Emotional 25/30 · Identity 25/25. EP accepted (gate >85 AND identity rock-solid). "Slimmer Jen" deferred as separate turnaround workstream. |
| **TL-0010_Egypt_TheLongRoad_v3 (HERO-02)** | TL-0010 | Witness persistence; audience walks beside him | Verbal (GVR-005) | "Emotional truth aligns with CRE-003; scale shift = accompanying, not observing." No numeric score logged. |
| **TL-0001_Cosmos_BeforeTime_v2 (HERO-01)** | TL-0001 | Enter silence; lower the heartbeat | No GVR on record | EP advanced the lock without a logged Gemini GVR (flagged in dossier). Q2 approved by EP/Director. |
| **TL-0070_Egypt_FirstRecognition_v5 (HERO-03)** | TL-0070 | Recognition before memory | No GVR on record | Director approved + EP locked; Gemini was redirected from creative GVR to the Resolution Bridge engineering task. |

> HERO-01 GVR gap and HERO-03 creative-GVR gap are open items. Dailies stills (GVR-001/002/003 pending) will populate this table when scored.

---

## Prompt Patterns That Failed

| Root Cause | Failure Mode | Asset(s) | Fix Now Standard |
|---|---|---|---|
| Emotion named, gaze geometry unstated | Model defaulted to side-by-side two-shot; recognition beat lost | TL-Seq1_Egypt_Recognition_v1 | State who-looks-at-whom + eye-line direction explicitly for ALL relational/two-shot frames |
| Character described, environment under-constrained, no spectacle negatives | Model invented monumental Karnak-style temple, contradicting Director's quiet-path intent | TL-Seq1_Egypt_Jen_hero_v1 | Describe environment positively AND negatively for all historical chapters |
| Period subject, modern accessories not negatively suppressed | Model preserved modern eyeglasses from reference photos into ancient-Egypt frame | TL-Seq1_Egypt_Recognition_v2 | Eyewear negatives + bare-face ref for all pre-WWII Gary frames (CD-001) |
| "First frame of a film" phrasing without border suppression | Rendered as a bordered/matted inset rather than full-bleed frame | TL-0001_Cosmos_BeforeTime_v1 | Border/matte negatives on ALL still generations (standing rule) |
| Frontal face refs used for a distant back-view shot | Model biased toward near-portrait; subject too large/centered despite "wide + from behind" instruction | TL-0010_Egypt_TheLongRoad_v1/v2 | Drop all face refs for distant back-view shots; specify SMALL + OFF-CENTER; iterate scale aggressively for "accompaniment" beats |
| Selfie photos used as identity refs instead of CCA sheets | Face drift across generations; modern accessories invaded historical frames | TL-0070 v1/v2, PS001-VEO v1/v2 | Sheet-Based Conditioning (CCA sheets only); never selfies or prior scene images (one-direction identity rule) |
| Veo Fast tier for identity-critical motion | Identity drift (age/hair jump) across the clip | PS001-VEO v1 | Veo Standard (`veo-3.1-generate-preview`) is the production motion baseline; never Fast for identity-sensitive clips |
| First+last keyframe conditioning with two far-apart frames (large camera move or angle change) | Veo cross-dissolves the gap → translucent ghost/duplicate figures mid-clip | PS001R2-C1 initial (55/100), PS001R2-C3 arc version (42/100) | First-frame-only conditioning whenever camera moves substantially; let Veo generate motion freely, guided by prompt |
| Pendant negative applied only to the character who should *have* it — not to characters who should *not* | Veo migrated the silver snail from Gary onto Jen's collar mid-clip (appear/vanish read) | PS001R2-C3 pendant-migration version | Extend prop/motif negatives explicitly to ALL characters who should NOT carry that prop |
| Camera arc with two far-apart keyframes (rear OTS → side two-shot) for a performance clip | Severe ghosting, costume-change read, prop teleport; GVR 42/100 | PS001R2-C3 arc re-renders | Static anchor when performance happens within the frame; arc requires first-frame-only + free motion |

---

## Studio Standards Established

| Standard | Status | Source | Applies to |
|---|---|---|---|
| **CD-001** — Gary bare-eyed in all pre-WWII chapters (glasses WWII+ only) | **Active** | TL-Seq1_Egypt_Recognition_v2 lesson; ratified by EP | Rome, Viking, Medieval, Renaissance, Frontier, Victorian, all pre-WWII chapters |
| **Border/matte negatives** on all stills (`border, black border, picture frame, rounded corners, vignette frame, matte, inset image, letterbox bars`) | **Active** | TL-0001_Cosmos_BeforeTime_v1 lesson | Every still generation |
| **Gaze geometry required** for relational two-shots (state who looks at whom; eye-line direction; complementary negatives) | **Active** | TL-Seq1_Egypt_Recognition_v1 lesson | Every two-shot in the film |
| **Environment positive + negative** for historical chapters (describe the world AND suppress spectacle explicitly) | **Active** | TL-Seq1_Egypt_Jen_hero_v1 lesson | Every historical chapter |
| **Sheet-Based Conditioning** — CCA sheets only; one-direction identity flow (`CCA → Scene → Scene`, never `Scene → Identity` or selfies) | **Active** | Director order 2026-06-27; first applied TL-0070 v3 | ALL scene generation |
| **Veo Standard tier** (`veo-3.1-generate-preview`) as production motion baseline | **Active** | PS001-VEO v1/v2 controlled comparison | All Veo motion renders |
| **First-frame-only conditioning** for clips with significant camera movement | **Active** | PS001R2-C1 stabilization re-roll; PS001R2-C3 static OTS | Any Veo clip where start/end keyframes are far apart in angle or distance |
| **Extend prop negatives to all non-carrying characters** (forbid the prop on everyone who should not have it) | **Active** | PS001R2-C3 pendant-migration fix | Any clip with a character-specific motif or prop |
| **Performance Anchor standard (PRO-017)** — hero stills are judged on whether animation can naturally arrive at the destination, not on being the climax | Studio Standard = **Accepted** | TL-0080_Egypt_FirstSmile_v2 (GVR-007 95%; EP locked 2026-06-27) | All future hero stills |
| **Witness Camera — Opening Movement Candidate Lesson** | Informational only (not canon) | PS001-VEO v3 / Director directive 2026-06-29 | Reclassified from "Accepted" after EP rejected the underlying take; informs PS001R2-C1 trailing camera but is NOT a standing studio standard |

**Assets with Studio Standard = Accepted:** TL-0080_Egypt_FirstSmile_v2 (Performance Anchor, PRO-017). TL-Seq1_Egypt_Recognition_v3 is the leading candidate for "recognition beat reference frame" — awaiting GVR-003 to formalize.

---

## Knowledge Reused

- **0 formal reuses recorded** — `Knowledge Reused In` is empty across all 22 Dossiers. Egypt and Cosmos are the first chapters produced; no forward application yet.
- **Within-Seq01 applications** (evidence of knowledge propagating internally — will populate `Knowledge Reused In` as future chapters are generated):

| Knowledge / Decision | Established in | Applied within Seq01 |
|---|---|---|
| CD-001 (Gary bare-eyed pre-WWII) | TL-Seq1_Egypt_Recognition_v2 | All subsequent Egypt Gary stills (v3 onward, TL-0070 family, TL-0080 family, all PS001R2 clips) |
| Border/matte negatives | TL-0001_Cosmos_BeforeTime_v1 lesson | Every still generated from HERO-02 onward |
| Gaze geometry explicit for two-shots | TL-Seq1_Egypt_Recognition_v1 lesson | Recognition_v2/v3, TL-0070 family |
| Ref-less generation for distant back-view shots | TL-0010 v1/v2 lessons | TL-0010_v3 (no face refs; figure small/incidental) |
| Sheet-Based Conditioning | CCA standard 2026-06-27 | TL-0070 v3/v4/v5, TL-0080 v1/v2, all PS001R2 keyframes |
| Veo Standard tier preference | PS001-VEO v1→v2 | All PS001R2 clips (C1/C2/C3) |
| First-frame-only conditioning for moving cameras | PS001R2-C1 stabilization re-roll | PS001R2-C3 static OTS (re-applied when arc failed) |

> **Queued to reuse forward** as future chapters are produced: CD-001 → Rome, Viking, Medieval, Renaissance, Frontier, Victorian. Gaze-geometry rule → every two-shot. Environment positive+negative → every historical chapter. Sheet-Based Conditioning → every chapter.

---

## Emerging Risks

*Predictive, grounded only in observed dossier data — no invented creative opinions.*

1. **Modern-accessory preservation in historical chapters.** Has manifested in stills (eyeglasses → CD-001) and recurred in motion (Jen CCA-002 drift in PS001-VEO Standard frontal clip — "reading younger/fuller" documented in the GVR re-audit). Source CCA photos contain modern styling. Eyewear negatives + bare-face refs must travel to every pre-WWII chapter without exception. Rome is the next high-risk chapter.

2. **Veo cross-dissolve ghosting on large camera moves (over-conditioning).** Re-manifested twice in PS001R2 despite the lesson being established after the first occurrence (C1 initial 55/100 → C3 arc 42/100). Root cause — two far-apart keyframes forcing a gap Veo cannot smoothly interpolate — recurs whenever a clip has a large camera move AND two conditioning frames. Every future motion clip with a significant angle or distance change is at risk until first-frame-only is the team's default reflex.

3. **Environment spectacle drift in upcoming historical chapters.** Manifested once (Jen hero v1 → Karnak). Egypt required explicit positive+negative environment constraints on every shot. Rome (Forum, marble), Viking (longships, fjords), Medieval (castles) are analogous high-risk settings where the model will default to the most visually spectacular period interpretation if the world is under-constrained.

4. **Border/matte artifacts on cinematic-frame prompts.** Triggered by "the very first frame of a film" phrasing on HERO-01. Risk recurs on any prompt evoking "cinematic frame," "first frame," or "film still." Standing border negatives are the fix; watch for this in Cosmos chapter and future sequence-opening frames.

5. **HERO-03 (TL-0070 v5) out-of-current-canon as a Veo conditioning anchor.** v5 (the locked HERO-03) was rendered pre-turnaround-conditioning and carries the fuller Jen build, temple/village background, and non-snail pendant. PS001R2-C3 had to retire v5 as its end frame and derive a v6 candidate (`Keyframes/TL-0070_v6_candidate.png`) — but v6 has **not yet received formal EP/Director approval to the locked registry**. Until v6 is approved and v5 archived, any future motion clip conditioning on HERO-03 as a last frame will interpolate to old canon (fuller Jen, temple, non-snail). High-priority open item.

6. **Jen canonical build (slim vs fuller) unresolved.** PS001R2-C3 Stabilization Re-Roll GVR (89/100) noted Jen does not read as canonical slim build; the EP spun off a **"re-slim the Jen turnaround" workstream**. Until the Jen turnaround is re-derived and CCAs updated, every scene conditioned on current Jen sheets may carry an inconsistent body build. Affects identity continuity across all Egypt clips and forward to future chapters.

7. **Pendant design not yet canonicalized.** The silver pendant shape has varied frame-to-frame (PS001-R2 continuity-anchor finding: "No canonical pendant reference exists — not on the costume sheet, none in `18_Motifs`"). The pendant is the film's key recurring motif; without a canonical reference plate, every new render may invent a different shape. Pendant migration onto Jen (C3 family) was a downstream consequence of this gap. Unresolved as of corpus date.

8. **"Observational accompaniment" framing will recur in future chapters.** HERO-02 required 3 iterations (v1→v2→v3) to achieve the small/incidental figure in a world-dominant landscape. The lesson is documented, but Rome, Viking, Medieval, and other chapters will each have analogous isolation or walking beats. Merely specifying "wide + from behind" is insufficient — the iteration lesson (SMALL + OFF-CENTER; drop face refs; specify environment as dominant) must be applied from the first render of each chapter.

---

## Watch Items

*Subtlety guardrails derived from Director Notes in Dossiers. Direct quotes attributed; none invented.*

- **"Do not romanticize loneliness. Do not exaggerate sadness. Stillness is stronger than melancholy. The audience should feel that something is missing... without yet knowing what it is."** (Director, HERO-02 / CRE-003.) Applies to every isolation beat in the film. Protect emotional absence over emotional display.

- **"This is not love at first sight. It is recognition before memory. Protect the hesitation. Do not rush the moment. The audience must discover it... one heartbeat before the characters do."** (Director, HERO-03 / CRE-004.) Guard against staging that resolves the recognition too clearly, too fast, or too symmetrically. Asymmetry — Gary first, Jen the echo — is structural, not optional.

- **"Do not play romance. Play relief. Do not play destiny. Play possibility. Hope should enter quietly enough that the audience discovers it inside themselves before they recognize it on screen."** (Director, HERO-04 / CRE-006.) The First Smile is the first crack in the armor, not the climax. Watch this distinction as the still transitions to the motion version.

- **Pendant dominance.** Director glint guardrail (PS001R2-C2, verbatim): *"The pendant reflection is a brief natural glint, not a glow, beam, or supernatural effect. Do not intensify the light beyond the keyframe. Treat it as sunlight catching polished silver for a fraction of a second."* Supervisor observed C2's glint rendered "fairly pronounced" before Gemini GVR rated it subtle — the margin is narrow. Watch pendant intensity on every new render; the motif must stay subordinate to the characters.

- **"If the audience notices the camera, the shot failed."** (Cinematic philosophy, PSD-001/PSD-001-R2.) Every motion clip should feel photographed, not generated. Camera attention — push-ins, orbit, overly smooth motion — is the primary motion quality risk.

- **"If one honest take captures the performance, keep it — do not improve it into dishonesty."** (Director ruling, 2026-06-29.) Re-rolling for a "better" take risks introducing artifice. Document the first honest take; iterate only when a specific, measurable criterion is unmet.

- **Dawn glow vs sunrise.** The opening's *"first possibility of light"* must not tip into a full sunrise or golden spectacle (CRE-001/CRE-002: "NOT a sunrise, only the first possibility of light"). Watch warm-glow intensity through Cosmos and Egypt, particularly as motion clips revisit the same dawn environment.

- **Same apparent age across ten lifetimes.** Gary and Jen must read as the same two souls across every chapter. Identity drift is the film's existential continuity risk; verify appearance continuity as Rome, Viking, and subsequent chapters accumulate.

---

> Method note: this report is derived purely from Dossier fields (Intent, prompt/negative, evolutionary tree, review verdicts, archive lessons, living fields, Director Notes). No creative opinions have been introduced. As the corpus grows — Rome, Viking, Medieval, and beyond — the tables sharpen and show where the pipeline systematically struggles, so prompt/ref/conditioning fixes can target the real failure modes.
