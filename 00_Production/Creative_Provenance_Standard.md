# TEN LIFETIMES — Creative Provenance Standard (the Dossier system)

> **Authored by the Director (Sam) + VFX Supervisor (Gemini), adopted by EP (Gary) 2026-06-26. Implemented by the Supervisor (Claude Code).**
> **Provenance** = origin · ownership · evolution · authenticity · lineage. We are **not versioning files — we are versioning creative thought.** (Renamed from "Asset Provenance" 2026-06-26 to name what it actually is.)

## Three products
This work now yields **three** artifacts, not one:
1. **Ten Lifetimes** — the film.
2. **Continuum Creative** — the reusable production methodology.
3. **The Creative Provenance Library** — a structured body of reusable creative knowledge. **The Dossiers ARE product #3.**

## The smallest unit of learning
Not the prompt — the **whole chain**:
```
Intent -> Prompt -> Image -> Review -> Decision -> Lesson
```
A Dossier records the entire chain. **The Dossier describes the EXPERIMENT; the image is merely the evidence.**

## Asset-as-Object — the Dossier IS the asset's identity
Each asset is a linked pair: the image (`Asset ID`) + its **Dossier** (`.md`). The Dossier is the asset's identity, not "metadata about" it. **Rule (Gemini): if an asset has no Dossier, it does not exist in the production ecosystem.** Never refer to a filename in a vacuum.

## The Dossier is BORN WITH the asset (atomic & automated)
The image and its Dossier are created **together, in the same action, at generation time.** The Supervisor writes the Dossier the moment the image is generated — never reconstructed from memory later (that loss is exactly what this standard prevents). Template: `60_TEMPLATES\Asset_Dossier_Template.md`.

## Intent / Narrative Purpose — the review North-Star
Every Dossier states the asset's **Intent**: what it must achieve narratively/emotionally. Set at birth (translated from the Director's CRE narrative), never silently changed.

## Director Notes — reminders to future reviewers
Each Dossier carries short **Director Notes**: terse guardrails for whoever reviews the asset later (e.g. *"the expression matters more than the environment"* · *"do not lose the feeling of familiarity"*). They are NOT the Intent and NOT generator instructions — they are the Director's reminders to reviewers. **Director-authored; the Supervisor leaves them empty** (same role boundary as Creative Discovery).

## The three-question review (every review answers all three)
1. **Technical** — did the render match the prompt?
2. **Creative** — did the prompt successfully implement the Director's **Intent**?
3. **Institutional** — should future productions reuse this approach?

These are three different evaluations. Gemini owns 1-2 (graded against Intent — a technical-pass / intent-fail is flagged for revision); Q3 feeds **Studio Standard**. Verdicts are written INTO the Dossier so reasoning stays locked to the image.

## GitHub Asset Canon + the Review Queue (Director, 2026-06-26)
A demonstrated blocker surfaced: the Director cannot direct an asset he cannot see, and **no creative authority approves a description.** The fix is also a canon correction:
- **GitHub is the canonical production-history repository for ALL generated assets and their Dossiers** (Review Queue, Dailies, Production History, Selected, Final). **The NAS is the local working mirror** for Premiere / Adobe / generation performance — NOT the only record.
- **No generated asset may remain NAS-only once it has a Dossier.** Every asset is published to GitHub with its Dossier **before** Director / Gemini / EP review, so all three evaluate the **same pixels, independently** (no reviewer inherits another's opinion).

**Public folder model (per sequence):**
- **`12_Review_Queue/Seq<NN>_Hero<NN>/`** — image + Dossier under review. Dailies / unapproved footage, explicitly **NOT canon.**
- **`12_Dailies/Seq<NN>_<Chapter>/`** — review/working selects (the earlier VFX-001/002 Egypt selects live here).
- **`13_Production_History/Seq<NN>_<Chapter>/<Category>/`** — superseded/rejected, kept + classified.
- **`14_Selected/Seq<NN>/`** — LOCKED selects (Director + Gemini + EP approved).
- **`15_Final/Seq<NN>/`** — final approved production assets (the deliverable cut).

**Lifecycle:** `Created → Review Queue → Director → Gemini → EP → LOCK → Selected → Final` (or → Production_History if rejected/superseded). Every move updates the Dossier lifecycle **and** the Asset Register. NAS mirror: `Stills/Working/` ↔ Review Queue · `Stills/Selected/` ↔ Selected · chapter `Final/` ↔ Final · `Stills/Production_History/` ↔ Production_History.

## Supervisor conduct — observe, don't opine (Director, 2026-06-26)
The Supervisor (Claude Code) announces readiness — *"HERO-01 ready for Director review"* — and may report **objective, measurable observations** (e.g. *"modern eyeglasses detected"*, *"a distant landform is present vs the 'no land features' brief"*, *"rendered with a border"*). The Supervisor does **NOT** offer **subjective cinematic judgments** (*"distracting"*, *"too much sunrise"*, *"beautiful"*) before the Director and Gemini have seen the frame. Each authority evaluates independently, then compares — agreement is signal, disagreement is signal. Same role boundary as Creative Discovery and Director Notes.

## Evolutionary tree — version control of creative decisions
Every Dossier records **Parent / Children / Siblings** (+ Supersedes / Superseded By) so the studio can A/B on the fly — *which single change caused the improvement?* (e.g. Recognition_v3 vs v2 = the eyewear negative prompt, CD-001).

## Living fields — beyond pass/fail
- **Creative Discovery** — capture happy accidents: neither failure nor success but **discovery** (e.g. "reflected Nile light read as hope more than the planned sunlight"), with a Recommendation. Authored by Director/Gemini, not the Supervisor.
- **Studio Standard** — `Pending | Accepted | Deprecated`. **Accepted** = future productions should BEGIN here.
- **Knowledge Reused In** — the sequences/projects where this asset's lesson was reused (Rome, Viking, Future...). Makes the Dossier **recursive** and lets us **measure knowledge reuse.**

## Every creative object gets a Dossier
Not just stills. **Still -> Motion Clip -> Transition -> Composite -> Final Scene -> Final Sequence** — each self-describing. A motion clip links its hero **still as Parent**, an unbroken chain from the first "break of light" still to the final sequence.

## The Creative Intelligence Report (analytics, NOT governance)
A **generated VIEW over all Dossiers** — `11_OPERATION_REPORTS\Creative_Intelligence_Report.md`, regenerated on cadence (target: weekly). It is analytics, not a new governance artifact, so it does **not** trip the Director's Rule. **Backward-looking** sections: Top Prompt Improvements · Most Common Continuity Errors · Highest-Rated Intent Matches · Prompt Patterns That Failed · Studio Standards Established · Knowledge Reused. **Forward-looking** sections (Director, 2026-06-26 — turn analytics into predictive guidance): **Emerging Risks** (e.g. *"the model keeps preserving modern accessories — watch closely during Rome"*) and **Watch Items** (e.g. *"pendant becoming too visually dominant — protect subtlety"*). Continuum thereby remembers **creative evolution** AND anticipates where it may stumble next.

## Never delete — classify (folder taxonomy)
Generated assets are **never deleted**; superseded/rejected ones are KEPT and classified. Per chapter, under `Stills\`:
```
Working\  ·  Selected\  ·  Production_History\<Category>\
```
Approved finals promote to chapter `Final\`. Categories: Historical_Continuity · Character_Consistency · Lighting · Composition · Camera_Motion · Prompt_Failure · Rendering_Artifact · Anatomy · Costume · Environment · Color_Grade · Experimental · Creative_Direction. Each archived asset's Dossier carries: Primary/Secondary Category · Severity (Critical/Major/Moderate/Minor/Cosmetic) · **Preventable?** (YES/NO/PARTIALLY) · Root Cause · Corrective Action · Continuity Decision (CD-###) · Lessons.

## Public exposure (EP, 2026-06-26)
Full ILM-style public archive: **all generated assets + Dossiers** publish to the public repo as institutional memory. Media is permitted under the FIVE stage folders — `12_Review_Queue/`, `12_Dailies/`, `13_Production_History/`, `14_Selected/`, `15_Final/`. Only **non-generated source assets** (real source photos, music, stems, `.prproj`) stay NAS-private. (See "GitHub Asset Canon + the Review Queue" above.)
