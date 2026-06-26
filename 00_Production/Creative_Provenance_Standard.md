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

## The three-question review (every review answers all three)
1. **Technical** — did the render match the prompt?
2. **Creative** — did the prompt successfully implement the Director's **Intent**?
3. **Institutional** — should future productions reuse this approach?

These are three different evaluations. Gemini owns 1-2 (graded against Intent — a technical-pass / intent-fail is flagged for revision); Q3 feeds **Studio Standard**. Verdicts are written INTO the Dossier so reasoning stays locked to the image.

## Evolutionary tree — version control of creative decisions
Every Dossier records **Parent / Children / Siblings** (+ Supersedes / Superseded By) so the studio can A/B on the fly — *which single change caused the improvement?* (e.g. Recognition_v3 vs v2 = the eyewear negative prompt, CD-001).

## Living fields — beyond pass/fail
- **Creative Discovery** — capture happy accidents: neither failure nor success but **discovery** (e.g. "reflected Nile light read as hope more than the planned sunlight"), with a Recommendation. Authored by Director/Gemini, not the Supervisor.
- **Studio Standard** — `Pending | Accepted | Deprecated`. **Accepted** = future productions should BEGIN here.
- **Knowledge Reused In** — the sequences/projects where this asset's lesson was reused (Rome, Viking, Future...). Makes the Dossier **recursive** and lets us **measure knowledge reuse.**

## Every creative object gets a Dossier
Not just stills. **Still -> Motion Clip -> Transition -> Composite -> Final Scene -> Final Sequence** — each self-describing. A motion clip links its hero **still as Parent**, an unbroken chain from the first "break of light" still to the final sequence.

## The Creative Intelligence Report (analytics, NOT governance)
A **generated VIEW over all Dossiers** — `11_OPERATION_REPORTS\Creative_Intelligence_Report.md`, regenerated on cadence (target: weekly). It is analytics, not a new governance artifact, so it does **not** trip the Director's Rule. Sections: **Top Prompt Improvements · Most Common Continuity Errors · Highest-Rated Intent Matches · Prompt Patterns That Failed · Studio Standards Established · Knowledge Reused.** Continuum thereby remembers **creative evolution**, not files.

## Never delete — classify (folder taxonomy)
Generated assets are **never deleted**; superseded/rejected ones are KEPT and classified. Per chapter, under `Stills\`:
```
Working\  ·  Selected\  ·  Production_History\<Category>\
```
Approved finals promote to chapter `Final\`. Categories: Historical_Continuity · Character_Consistency · Lighting · Composition · Camera_Motion · Prompt_Failure · Rendering_Artifact · Anatomy · Costume · Environment · Color_Grade · Experimental · Creative_Direction. Each archived asset's Dossier carries: Primary/Secondary Category · Severity (Critical/Major/Moderate/Minor/Cosmetic) · **Preventable?** (YES/NO/PARTIALLY) · Root Cause · Corrective Action · Continuity Decision (CD-###) · Lessons.

## Public exposure (EP, 2026-06-26)
Full ILM-style public archive: Dossiers + archived images publish to the public repo as institutional memory. Media is permitted ONLY under `12_Dailies/` (selects) and `13_Production_History/` (archive); all other media stays on the NAS vault.
