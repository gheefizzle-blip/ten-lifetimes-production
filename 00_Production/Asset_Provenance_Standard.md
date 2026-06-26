# TEN LIFETIMES — Asset Provenance Standard (the Dossier system)

> **Authored by the Director (Sam) + VFX Supervisor (Gemini), adopted by EP (Gary) 2026-06-26. Implemented by the Supervisor (Claude Code).**
> The repository is not a source-code repo to be kept lean. It is a **Production Journal / creative-intelligence library**. We do not delete generated assets — we classify, annotate, and learn from them. Every mistake that teaches the studio something becomes an asset, not waste.

## Asset-as-Object — the Dossier IS the asset's identity

Each generated asset is a **linked pair**: the image (`Asset ID`) + its **Dossier** (the companion `.md`). The Dossier is not "metadata about" the file — it is the asset's identity and birth certificate. **Rule (Gemini, 2026-06-26): if an asset has no Dossier, it does not exist in the production ecosystem.** We never refer to a filename in a vacuum.

```
TL-Seq1_Egypt_Gary_hero_v1.png      <- the image
TL-Seq1_Egypt_Gary_hero_v1.md       <- the DOSSIER (identity + provenance + intent + lineage + reviews)
```

## The core rule — the Dossier is BORN WITH the asset (atomic & automated)

**No generated asset exists without its Dossier.** The image and its Dossier are created **together, in the same action, at generation time** — the birth is atomic. The Supervisor (Claude Code) writes the Dossier the moment the image is generated; it is never reconstructed from memory later (that loss is exactly what this standard prevents). The Dossier captures, while context is live: **Intent**, the **exact prompt + negative prompt**, model/version, parameters, master references, and **lineage**. Template: `60_TEMPLATES\Asset_Provenance_Template.md`.

## Intent / Narrative Purpose — the review North-Star

Every Dossier states the asset's **Intent**: what it must achieve narratively/emotionally (e.g. *the thousand-yard stare of a man who has walked this road before*). **Gemini grades every render against its Intent field, not just its technical quality.** A technically flawless render that misses its narrative purpose is flagged for revision. Intent is set at birth (translated from the Director's CRE narrative) and never silently changed.

## Evolutionary tree — version control of creative decisions

Every Dossier records its place in the asset family so the studio can A/B test on the fly — *which prompt change caused the improvement?*
- **Parent:** the asset this one was derived from (e.g. Recognition_v3's parent is v2).
- **Children:** assets derived from this one.
- **Siblings:** alternate renders of the same beat/shot.
- **Supersedes / Superseded By:** the disposition link.
Example the system was built to answer: *why is Recognition_v3 better than v2?* The Dossiers show the single change — the eyewear negative prompt (CD-001).

## Motion provenance chain (forward-looking)

When a still is promoted to motion (Sora/Veo), the **still hero is the Parent** of the motion clip's Dossier — an unbroken chain from the first "break of light" still to the final animated transition. Motion Dossiers carry the same Intent/lineage/review fields.

## The generation workflow (replaces "generate -> register")

```
Generate PNG
   -> IMMEDIATELY write the matching .md (full prompt/negative/params/refs)
   -> register both together (Asset Register)
   -> Review (Director / Gemini GVR / EP)
   -> update the .md (review history + disposition)
   -> Promote (Selected -> Final) OR move to Production_History (never delete)
```

## Lifecycle (every transition timestamped in the .md)

```
Created -> Reviewed -> Selected -> Approved -> Published -> (Final | Production_History)
```

Every generated asset has one of four destinies — **nothing is deleted, only classified**:

```
Generated -> Review -> Accepted -> Final            (the cut)
                    -> Accepted -> Production_History (good, not used)
          -> Review -> Rejected -> Production_History (failed, but a lesson)
```

## Folder structure (per chapter, e.g. `04_Egypt\Stills\`)

```
Stills\
  Working\                     fresh generations under review
  Selected\                    current selects awaiting / passed review
  Production_History\          superseded or rejected — KEPT, never deleted, classified by category
    Historical_Continuity\
    Character_Consistency\
    Lighting\
    Composition\
    Camera_Motion\
    Prompt_Failure\
    Rendering_Artifact\
    Anatomy\
    Costume\
    Environment\
    Color_Grade\
    Experimental\
    Creative_Direction\
```
Approved finals are promoted to the chapter-level `Final\` (existing convention). `Production_History` is Sam's deliberate rename of "Archive" — these files are **active reference material, not dead storage.**

## Classification fields (in every archived asset's .md)

- **Primary Category** (exactly one, from the list above) + optional **Secondary Categories**.
- **Severity:** `Critical` | `Major` | `Moderate` | `Minor` | `Cosmetic`.
  (six-fingered hand = Critical; modern eyeglasses = Moderate — doesn't ruin the frame but blocks acceptance.)
- **Preventable?** `YES` | `NO` | `PARTIALLY` — the highest-value field. A `YES` invites the question "why wasn't it prevented?" and drives a pipeline improvement.
- **Continuity Decision:** link to the `CD-###` it triggered (ledger in `Continuity_Report.md`).
- **Superseded By / Derived From:** the asset family tree (version control of creative decisions).

## Why this exists (institutional memory)

After N archived assets we can answer, by searching the provenance files:
*"How often does Nano Banana preserve modern eyewear?"* · *"Which negative prompts eliminated modern accessories?"* · *"What continuity failures are common in historical generation?"* · *"Why did Recognition_v7 work?"* — open its `.md`; the exact prompt and lineage are there. This turns discarded generations into **production intelligence** for Ten Lifetimes and every future Continuum Creative production.

> Governance note: adopted under the Creative-Production freeze (Bible §0g) because it removes a **demonstrated** problem — the Recognition_v2 glasses incident nearly erased a reusable lesson. Director-authored, EP-approved.
