# TEN LIFETIMES — Asset Provenance Standard

> **Authored by the Director (Sam), adopted by EP (Gary) 2026-06-26. Implemented by the Supervisor (Claude Code).**
> The repository is not a source-code repo to be kept lean. It is a **Production Journal / creative-provenance system**. We do not delete generated assets — we classify, annotate, and learn from them. Every mistake that teaches the studio something becomes an asset, not waste.

## The core rule — metadata is BORN WITH the asset

**No generated asset exists without its companion `.md`.** The image and its metadata file are created **together**, at generation time, and never separate:

```
TL-Seq1_Egypt_Gary_hero_v1.png      <- the asset
TL-Seq1_Egypt_Gary_hero_v1.md       <- its birth certificate (provenance)
```

The `.md` captures, while the context is still live: the **exact prompt + negative prompt**, model/version, parameters, master references used, and lineage. This is non-negotiable — reconstructing a prompt from memory later is exactly the failure this standard prevents. Template: `60_TEMPLATES\Asset_Provenance_Template.md`.

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
