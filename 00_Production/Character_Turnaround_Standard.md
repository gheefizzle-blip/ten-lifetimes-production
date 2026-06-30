# CONTINUUM STUDIO — Character Turnaround Standard
### Canonical Character Assets are built as 360° model sheets, not single views

> **Standard established by the EP (Gary), 2026-06-30; formalized by the Production Supervisor; for Director (Sam) creative sign-off.** Evolves the existing **Canonical Character Asset (CCA)** + **Canonical Costume Asset** standards: a character + costume is specified the way a **video-game / animation character turnaround** is — *"a slowly spinning holographic image that captures every detail,"* so **every render of that character stays consistent.** This is the root-cause fix for the drift seen in Performance Segment 001 (face, costume back, pendant, accessories all drifted because references were partial).

## MANDATORY STUDIO RULE (EP, 2026-06-30)
**Every character — in this project and every future Continuum Studio production — is built as a full profile + character sheet + costume turnaround at the moment the character is introduced, BEFORE any scene/motion work.** No character is photographed into a scene until its turnaround exists and is locked. This is a permanent studio onboarding step (belongs with the Layer-1 Constitution): it is the single highest-leverage consistency investment — it prevents countless failed-render retries and delivers better character consistency across the board. Cost is a handful of reference stills up front; the payoff compounds over every shot of that character forever.

## Principle
Partial references → the model invents the unspecified detail differently each render (verified: costume back, pendant, shoreline all drifted on PS001-R2). **A complete multi-angle reference removes the invention.** Every scene/motion render conditions on the turnaround; nothing is re-discovered per shot.

## What a Canonical Character Turnaround contains (per character, per era)
**A. Rotation set (the "spin") — full-figure, in locked costume, neutral pose, even light, plain background:**
1. Front · 2. 3/4 Left · 3. Profile Left · 4. **Back** · 5. 3/4 Right · 6. Profile Right
*(6 steps minimum; add 45° intermediates if a shot needs them.)*

**B. Detail callouts (close, unambiguous, locked):**
- Face — neutral + "recognition" expression (already have CCA v2 face sheets)
- **Pendant — THE SILVER SNAIL (canon, EP 2026-06-30).** Gary's pendant is a **silver snail**, worn in **every lifetime/era** — a fixed motif and a story key. *Meaning (provenance):* Jen calls Gary her "Snail" (after SpongeBob's pet snail, named Gary); the film shows only the snail pendant — no external IP on screen. The **form (silver snail) is constant across eras**; craftsmanship adapts per era (e.g. Egypt = hand-cast silver amulet; Modern = fine silver necklace). Lock one canonical design; it is the recognition motif ("pendant catches light first"). **⚠️ Retrofit needed:** locked Egypt heroes (HERO-03 v5, HERO-04) currently show a generic pendant → require a surgical pendant→snail edit for cross-timeline consistency. **Must propagate to Bible §0c Recognition Rules + Character Bible.**
- Costume **neckline** (front + back), sleeve, hem
- Sash / belt + tools (Architect: drafting tube, measuring cord, stylus) / accessories
- Hair (or wig, for Jen) — front + back
- Footwear · hands

**C. Spec card:** one-line written lock of each attribute (color, material, count) beside the images, so text + image agree.

## How it's used (conditioning rule)
- The turnaround **is** the Canonical Character Asset. Store under `00_Identity_Master/<Char>_<Era>/Turnaround/` (+ NAS mirror). Register in `CCA_Registry.md`.
- **Every scene/keyframe/motion render conditions on the turnaround angle(s) closest to the shot** (e.g. a rear shot conditions on the Back + pendant-cord detail; a two-shot on Front/3-4 + pendant). One-direction rule unchanged: **Turnaround → Scene, never Scene → Turnaround.**
- Tooling note (from PS001-R2): `nb2` conditioned-generation is sticky — it holds detail well **when the detail is in the reference**, but will not invent/correct an absent detail from words alone. The turnaround supplies the detail so the model never has to invent it.

## Build method (Nano Banana)
Build each rotation angle conditioned on the locked anchors (matching CCA face-angle sheet + costume front + costume back-ref + pendant detail), so the character stays identical while rotating. Lock the set as a whole (Director + EP) before it becomes the conditioning source. Detail callouts derived from locked hero frames where possible (pendant from HERO-03; nothing invented).

## Lifecycle
`Build rotation + detail set → Director/EP lock → becomes the Canonical Character Asset → ALL renders condition on it`. Supersedes single-view CCA/costume conditioning. Existing locked CCA v2 face sheets + `Gary_Costume_Egypt_BACK_ref` fold in as the face + back components.

> **Status (2026-06-30):** standard authored per EP directive. First builds queued: **Gary (Egypt)** turnaround (pilot, validates the method) → **Jen (Egypt)** → then re-derive the PS001-R2 keyframes from the turnarounds. Pendant design to be locked (proposed: from HERO-03 v5) as part of Gary's detail callouts.
