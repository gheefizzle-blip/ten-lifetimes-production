# TEN LIFETIMES — Production Bible

> ## ⭐ THE GUIDING PRINCIPLE (Director, 2026-06-27)
> **"Every technical decision must preserve or strengthen the emotional integrity of the performance. If it does not, the performance wins."**
> This is the first principle of the studio. Resolution, tooling, and process all serve the performance — never the reverse. (Applies to all Continuum Creative productions, not just Ten Lifetimes.)

> **The Constitution of the project.** Answers the question: *"What kind of film are we making?"*
> Once approved, this document changes rarely. Everything else (timeline, shots, work orders) traces back here.

- **Document version:** v1.0
- **Last updated:** 2026-06-28 by Agent B (Claude Code, Production Supervisor)
- **Production version:** **PT-1.0 — PLANNING COMPLETE; PRODUCTION PHASE.** (Pre-production closed 2026-06-28 with the EDL-001 lock.)

> ## 🎬 PHASE TRANSITION (2026-06-28) — Pre-Production CLOSED → Production (Phase 2: Performance Validation)
> **EDL-001 (Master Runtime Allocation) is CANON LOCKED.** The music is the immutable master clock. The studio is now a **production organization**, not a planning one.
> **Director's Standing Order:** from this point, no changes are authorized to **runtime · era durations · chorus splits (B/A/B) · emotional allocation** — those decisions are complete. Every creative discussion is now *"how do we make these allocated seconds emotionally unforgettable?"*
> **What is locked:** screenplay/lyrics · emotional timeline (329.60 s) · cast (CCAs) · costumes · Performance Anchors HERO-01→04 · the Performance Anchor/Trajectory/Segment methodology · the master clock.
> **Next:** Performance Segment 001 (Opening Movement, HERO-01→04). From here, *every hour moves pixels on the screen, not paragraphs in the Bible.*

---

## 0. Production Facts

| Field | Value |
|---|---|
| **Title** | Ten Lifetimes — A Cinematic Short Film |
| **Artist** | Tommy Ransome & The Gary Spear Experience |
| **Format** | Cinematic short film (a narrative interpretation of the song — not a music video; visuals carry the story, the music is the score) |
| **Runtime** | **5:29 (329.0 sec)** — exact lock pending audio measurement |
| **Aspect ratio** | 16:9 (2.39:1 letterbox optional for "film" feel) |
| **Master audio** | `D:\My_Music\Tommy Ransome & The Gary Spear Experience\TEN LIFETIMES\TEN LIFETIMES.mp3` |
| **Stems** | same folder — `TEN LIFETIMES Stems (1)\` (isolated tracks for precise timing) |
| **Edit project** | `Ten Lifetimes.prproj` (Adobe Premiere Pro) — same folder |
| **Project root** | `D:\My_Music\Ten_Lifetimes\` (NAS `gary_spear` share, reachable all devices) |

---

## 0a. Canon Rule — Systems of Truth (governance)

> Adopted 2026-06-25 (Director Sam → EP Gary). Now that documentation is public, each system owns **exactly one** type of truth — no overlap.

| System | Owns | Location |
|---|---|---|
| **GitHub** | Canonical **production history** — documentation **AND all generated assets + their Dossiers** (Review Queue, Dailies, Production History, Selected, Final). **Revised 2026-06-26 (Director Sam → EP Gary): GitHub is the full record, not docs-only.** | `gheefizzle-blip/ten-lifetimes-production` (PUBLIC) |
| **NAS** | **Local working mirror** for generation + Premiere/Adobe performance, AND the private home for **non-published production files** (music masters, stems, `.prproj`, raw HEIC originals). No *generated* asset stays NAS-only once it has a Dossier. (Reference PHOTOS of Gary/Jen are now also published — EP 2026-06-27.) | `D:\My_Music\Ten_Lifetimes\` (working mirror) |
| **Premiere** | Canonical **editorial assembly** (the cut itself) | `Ten Lifetimes.prproj` |
| **Continuum** | Canonical **governance history** (work-order lifecycle, approvals, attestations, decision provenance) | Aegis Continuum system of record |

A fact lives in exactly one of these. Documentation never holds assets; assets never hold canon docs; the cut is owned by Premiere, described by the Master Production Timeline; governance provenance is owned by Continuum. This prevents drift and ambiguity as the project scales.

> **Media on GitHub (current canon — see §0a + Creative Provenance Standard; updated 2026-06-26 PRO-014):** GitHub is the full production history — **all generated assets + their Dossiers** are public across the FIVE stage folders **`12_Review_Queue/` · `12_Dailies/` · `13_Production_History/` · `14_Selected/` · `15_Final/`** (the `.gitignore` un-ignores media only there). **Reference photos of Gary/Jen are PUBLIC** (EP decision 2026-06-27 — they are public figures, no privacy concern; reference set published at `00_Identity_Master/Source_Photos/`, so the cast can be re-referenced anytime). **Music masters, stems, and the `.prproj` remain NAS-private** (production/distribution files, not a privacy matter; HEIC originals stay on the NAS, JPG conversions are published). ⚠️ The repo is PUBLIC and All-Rights-Reserved; committed media is world-visible and permanent in git history.

The **`MASTER_PRODUCTION_TIMELINE.md`** is the relational index that binds all three: every lyric word → time → shot → prompt → render → editorial clip.

---

## 0b. Production Team & Authority (governance — formalized 2026-06-25)

A multi-agent film studio. One responsibility each — **nobody overlaps** (this is why it scales).

| Role | System | Responsibility |
|---|---|---|
| **Executive Producer** | Gary | Final creative & business approval — what becomes canon |
| **Director** | ChatGPT "Sam" | Story, emotion, symbolism, pacing, cinematic language (**creative authorship**) |
| **Production Supervisor** | Claude Code (Agent B) | Execution: work orders, documentation, prompts, asset tracking, GitHub, Continuum integration |
| **Visual Effects Supervisor** | Gemini | Cinematic critique, video analysis, continuity review, Veo generation strategy (**review only — see §0d**) |
| *Editorial* | Adobe Premiere | Final assembly & timing |
| *Working mirror* | NAS | Local mirror for generation + editing; **GitHub is canonical for generated assets — §0a** |

**The four responsibilities (operating principle, Director 2026-06-26 — nobody crosses these lines):**
- **Director owns MEANING.** Authors creative-intent documents ONLY — Director's Narrative, Director's Notes, Emotional/Memory Storyboard, Camera Presence, Performance Direction, Review Decisions. The Director does NOT write prompts, mockups, concept art, folder structures, or commits.
- **Production Supervisor (Claude) owns EXECUTION.** Translates the Director's intent into prompts, Dossiers, assets, GitHub, provenance, review plumbing. Never guesses emotional intent; never authors meaning or cinematic opinion.
- **VFX Supervisor (Gemini) owns VISUAL TRUTH.** Independently judges whether the rendered frame communicates the Director's intent. Never authors meaning.
- **Executive Producer (Gary) owns CANON.** Decides what becomes part of Ten Lifetimes.
> A Director directive answers: *what should the audience feel / attend to / remember / not notice?* Everything downstream is the Supervisor's translation. The Director hands over intent; the Supervisor never has to guess it.
| *Production Brain* | GitHub | Canonical documentation |
| *Governance* | Continuum | Decision history, approvals, lineage |

**Creative voice stays singular:** **ChatGPT writes · Gemini critiques · Claude executes · Gary approves.** The Supervisor makes no creative decisions; the VFX Supervisor authors no story/symbol/character/emotion; the Director manages no files; approval is the EP's alone.

**Production workflow:**
`Director (ChatGPT) → Production (Claude Code) → Generation → Gemini Review → EP Approval → Canon`

## 0b-PA. The Performance Anchor Standard (PRO-017 — Director + VFX, 2026-06-27)

> The single most important methodology shift since Canonical Character Assets. We have stopped making *finished cinematic moments* as stills and started making **Performance Anchors**.

**The principle.** A hero still is not the climax of the performance — it is the **Performance Anchor** (the key pose) for the video model that follows. It establishes *emotional truth* (Frame 1); the *emotional event* (the climax) belongs to motion. We separate the **Emotional Foundation** (the still) from the **Emotional Event** (the animation).

**New success criterion.** A still is no longer judged by *"Is this the climax?"* — it is judged by *"Can the performance naturally arrive at the climax from here?"* A still is "perfect" when it holds the **maximum potential** for the subsequent animation (Sora / Veo / Runway) to reach the intended emotional destination. **Do not over-polish a still** — the emotion should bloom in motion, not be fully spent in the anchor.

**Two-section directing.** From PRO-017 forward, every **Director's Narrative** (CRE) and every Dossier carries two emotional waypoints:
- **Performance Anchor** — what emotional state exists at **Frame 1** (where the still begins).
- **Performance Trajectory** — what emotional state exists at the **final frame** (where the animation ends).
Everything between the two is cinematography/interpolation. This removes AI video's biggest weakness — the model no longer invents where motion starts or ends; we direct both. *Start here. Finish here.*

**HERO-04 is the first asset evaluated under this standard:** Anchor = *hope has just appeared* (Gary leads, Jen echoes); Trajectory = *hope quietly becomes the first genuine smile, over time*. The regeneration chase is **cancelled** — the smile belongs to motion, not the still.

**The third object — the Performance Segment (added 2026-06-28, EDL-001).** Between two anchors lives a **Performance Segment**: the *complete motion sequence* that carries the performance from one anchor to the next. It is not a single clip — it is a directed chain:
`Anchor → Motion Clip A → Motion Clip B → Motion Clip C → next Anchor`
EDL-001 proved why this object is necessary: a single still cannot carry ~20 s of screen time (HERO-02 "The Long Road" owns ~19.8 s), so that time is built as a Performance Segment of 2–3 directed clips, not one impossible animation. **The unit of motion production is the Performance Segment, not the clip.**

**Impressionistic acceleration (EDL-001 corollary).** Not every era needs the same clip count. Egypt (the establishing grammar) wants 2–3 clips per beat; later eras can become **increasingly impressionistic** — fewer, faster clips — exactly as the song accelerates emotionally. Density follows the music.

**The complete motion production model (Director-validated 2026-06-28):**
`Performance Anchor → Performance Trajectory → Performance Segment → Finished Sequence`
The Director has ruled this model complete — it needs no further refinement before animation testing begins.

> Concept ownership: Director (Sam) + VFX (Gemini) co-authored; Performance Segment added by Director (Sam) at EDL-001. Applies to all Continuum Creative productions. *"We've stopped asking AI to invent emotion. We're asking it to perform emotion we've already directed."*

## 0c. The Three Recognition Rules (permanent — every lifetime)

Established in Sequence One (Egypt) and **silently repeated across all ten lifetimes**. The audience should never consciously notice them — by the finale they should feel these have *always* been true.

1. **Gary always notices Jen first** — not because she's prettier, because his soul recognizes her.
2. **Jen always smiles second** — a tiny hesitation first, almost *"I know you…"* without knowing why.
3. **The pendant always catches the light first** — the *light* finds it, not the camera; subconscious, never spotlit.

> These are micro-choreography laws of every reunion. They join the existing character laws (recognizable gesture / same age / pendant present) in the Character Bible.

## 0d. Gemini Production Charter (adopted & **ratified by Gemini** 2026-06-25)

**Role:** Visual Effects Supervisor & Cinematic Review Authority.

**Primary responsibilities** — review only:
- Conduct **Daily Video Reviews (GVR)** of all generated clips.
- Evaluate visual realism, camera movement, and lighting consistency.
- Detect and flag AI artifacts and historical anachronisms.
- Recommend **Veo/Sora** prompt optimizations and motion refinements.
- Review assembled edits for pacing, flow, and visual continuity.

**Authority & boundaries:** Gemini provides visual & cinematic review **only**, and is **strictly prohibited from altering or authoring** story, symbolism, character arcs, or emotional direction. This preserves a single creative voice (the Director). Gemini's Veo/Sora recommendations are translated into VFX work orders by the Supervisor (Claude); the Director's creative intent governs. *(In Gemini's words: "Sam owns the soul of the film; I protect its cinematic reality.")*

**Workflow:** `Director (ChatGPT) → Production (Claude Code) → Generation → Gemini Review → EP Approval → Canon`.

**Review artifacts:**
- `GVR-###` — **Gemini Video Review** (per generated clip): facial consistency · lighting continuity · historical authenticity · camera motion · AI artifacts · emotional impact · suggested retakes.
- **Gemini Continuity Review** — on the *assembled edit*: emotional-arc flow, pacing, transition smoothness, sustained engagement.
- Reviews land in `11_REVIEWS\Gemini\`; verdicts route to EP for approval. No-self-validation holds (the generator does not review its own output).

> **Gate:** per Director, no Sequence One generation begins until this charter is canonized (now in effect).

## 0e. Operation Report Standard (PRO-006, adopted 2026-06-25)

So all agents share one operational audit trail readable from the public repo: **every work order / production operation produces a public Markdown completion report.**

**Every operation produces:** (1) a work-order file, (2) a completion/operation report, (3) canon updates, (4) public GitHub sync — **unless held by the EP** (then the report states why).

- Reports live in **`11_Operation_Reports/`** (public mirror; NAS `11_OPERATION_REPORTS\`), named `YYYY-MM-DD_<WO-ID>_<Short_Title>_REPORT.md`. Template: **`60_TEMPLATES\Operation_Report_Template.md`**.
- **Rules:** ASCII-only (no em-dashes / smart quotes); **no private media** (photos/audio/generated assets) committed; NAS paths may be referenced but personal media never exposed; every report identifies files **created / modified / deleted** and **whether GitHub was synced** (if deferred, why); every report states **open blockers** and **next recommended action**; closes with the **reflection block** in order — **Lessons Learned** (institutional knowledge, mineable by Continuum), **Creative Impact** (why it mattered creatively + Risk + Downstream), **Pipeline Impact** (effect on tooling/workflow), **Recommendations** (for future WOs), and **Would We Do This Again?** (would we build a film this way again — turns the project into training data) — then a **Supervisor Attestation**.
- **Goal:** ChatGPT and Gemini can understand a completed operation by reading its report alone.

## 0f. The Production Loop & Creative North-Star (Director, 2026-06-25)

**North-star (sharpens the Reality Test):** *We are not trying to impress people with AI — we are trying to make them forget AI exists.* If a viewer says **"that's beautiful AI,"** we failed. If they say **"that felt like a movie,"** we succeeded. Every prompt, render, and review is judged against this.

**Corollary — underwhelm visually, overwhelm emotionally (Director, 2026-06-26):** the opening minute should *underwhelm visually and overwhelm emotionally.* It sounds contradictory; it isn't. If the audience's first-minute thought is *"wow, beautiful visuals,"* we probably missed. If it is *"why do I already care about these two people?"*, we succeeded. Restraint is the goal, not spectacle.

**Asset provenance (born-with-asset rule, Director 2026-06-26):** EVERY generated asset is created together with a companion `.md` provenance file capturing the **exact prompt + negative prompt + params + refs + lineage** — at generation time, never reconstructed later. Assets are **never deleted**; superseded/rejected ones are classified into `Production_History\<Category>\` with a `Preventable?`/severity/lesson record. The repo is a Production Journal, not a lean source tree — we version creative thought, not files. Full spec: `20_REFERENCE\Creative_Provenance_Standard.md`.

**Casting & Sheet-Based Conditioning (STUDIO STANDARD, Director 2026-06-27):** we **cast actors once and lock them**, then photograph them into scenes — we never re-invent a face per scene. The locked identity sheets are **Canonical Character Assets (CCA)**: **CCA-001 = Gary · CCA-002 = Jen** (era variants `CCA-00N-<ERA>`), living in `00_Identity_Master/`. **Casting Complete = identity FROZEN** (scenes photograph the actor, never modify it). **ALL scene generation conditions on the approved CCA sheets** — never on the original selfies or a prior scene; identity flows one way (`CCA → Scene`), never `Scene → Identity`. Build sheets via `nb2` edit-restyle of real photos. Full spec: Creative Provenance Standard.

**The Production Loop — run per sequence, in order (no generating everything at once):**
1. Build **hero stills** (each born with its provenance `.md`).
2. **Director** review.
3. **Gemini GVR** review.
4. **EP** approval.
5. **Lock the visual language** (the look becomes the standard for the sequence).
6. Generate **supporting stills**.
7. Generate **motion**.
8. **Gemini motion** review.
9. **Final approval**.
→ repeat for every sequence.

**Per-hero approval gates (Director, CRE-002, 2026-06-26):** within step 1, each hero still is its OWN micro-production with its own LOCK — `Generate → Dossier → Publish to Review Queue → Director → Gemini → EP → LOCK → move (Selected | Production_History)`, then (and only then) the next hero. Think in **approval gates, not in "a batch of six."** No batch generation. **Reviewers evaluate the published FRAME in the Review Queue (`12_Review_Queue/Seq<NN>_Hero<NN>/` — image + Dossier + Director Review Packet, PRO-015), never a description** — see Creative Provenance Standard "The Review Queue." Each approved frame informs the next, which is how the sequence acquires one consistent cinematic language and avoids downstream drift. A hero is not "done" until **LOCKED.**

**Sequence Retrospective (craftsmanship, not governance) — at the close of *each sequence*, not each WO:** What surprised us? · What worked? · What failed? · What would we never do again? · What becomes studio standard? Captured in the sequence's final operation report (and any standard it mints feeds the Camera/Character/Lighting bibles).

> Hierarchy parallel (Hollywood ↔ ours): Writer/Director → Production Supervisor → Generation → Gemini Dailies → Premiere → Executive Producer.
> **First-minute contract:** by the Chorus 1 downbeat (1:03.820), the audience should already believe they're watching a real cinematic love story — that emotional contract carries the whole film.

## 0g. Phase: CREATIVE PRODUCTION (declared 2026-06-25) + The Director's Rule

The infrastructure phase is **complete and frozen.** The project has moved from *pre-production* to **Creative Production** — creative work is now the default; infrastructure changes require justification.

> **The Director's Rule:** *During Creative Production, no new governance, infrastructure, documentation, workflow, or organizational artifact may be introduced unless it removes a demonstrated production blocker or measurably improves the quality of the finished film.*
>
> This binds everyone, including the Director. It protects momentum and creativity. Every change — and every operation report — is judged by one standard: **Did it make the film better?**

This keeps the film the priority and prevents documentation from expanding just because a good idea appears. PRO-009 is the final infrastructure operation that enacts this freeze.

**Reference-implementation note:** beyond this one film, the repository has become a **Production Journal** documenting *how AI-directed films are made* — the reference implementation for **Continuum Creative**. Its biggest success is organizational: four collaborators, no competition, each with a bounded authority. Preserve that.

---

## 1. Vision Statement

*Ten Lifetimes* is not a history lesson and not a slideshow. It is **one continuous love story told through time** — the same two souls (Gary & Jen) finding each other again and again across ten lifetimes, from Ancient Egypt to a peaceful far future, before the fantasy dissolves into a single **real photograph** of the two of them.

The film must clear one bar on every frame:

> **The Reality Test — "Could someone mistake this frame for a real movie?"**
> If a frame looks like "AI content," it fails. Every still and every clip is held to feature-film standard.

The emotional core is already in the song. The visuals exist to **protect and amplify** that core — never to show off the technology.

---

## 2. Logline

> *Across ten lifetimes and ten thousand years, two souls keep finding their way back to each other — until the story stops being a fantasy and becomes the real love of Gary and Jen.*

---

## 3. Themes

- Eternal love / love that outlives death and time
- Destiny and recognition ("we've met before")
- Searching, waiting, and faith across separation
- The reveal that the grandest imagined love story points to a **real** person

---

## 4. Character Bible

Two souls, **ten faces of history, one constant connection.** Faces stay recognizably Gary & Jen in every chapter (see §6 Visual Rules).

### Gary
- Source refs: `01_Reference_Gary\` (Gary 1–5.jpg). Primary identity anchor: **gary 2.jpg** (clear, straight-on, natural smile). Canonical master → `16_Master_References\Gary_Master.jpg` (TBD select).
- **Permanent traits (never change across eras):** tall male presence; strong defined jawline; well-defined beard; kind, warm eyes; confident, grounded bearing; salt-and-pepper coloring.
- **Keep OUT of historical refs:** red cap, modern clothing, sunglasses (great for facial structure, wrong for period).

### Jen
- Source refs: `02_Reference_Jen\` (Jen 1–10.jpg). Canonical master → `16_Master_References\Jen_Master.jpg` (TBD select).
- **Permanent traits:** warm, genuine smile; bright, expressive eyes; approachable elegance; long dark hair (or actual color). Emphasize *expression and warmth* over recreating any one reference hairstyle.

### The Couple (chemistry anchor)
- Source refs: `03_Couple_Photos\` (7 photos). Candid interactions teach the models how they *naturally look together* — that chemistry is what we preserve across every lifetime.
- One real couple photo is **reserved for the final frame** (see §11). Canonical → `16_Master_References\Couple_Master.jpg` (TBD select — strongest *emotional* image, not necessarily most technically perfect).

### Casting principle — they *become* people of each era
Not "Gary in Egyptian clothes." In each chapter they are believable citizens of that civilization, revealing a different side of who they could have been — while the emotional connection stays unmistakably familiar (see §8 chapter roles).

---

## 5. The Ten Chapters (overview)

We say **"Chapter," not "era"** — this is a cinematic love story in ten chapters, not a collection of historical scenes.

| # | Chapter | Period | Dominant Color | Atmosphere |
|---|---|---|---|---|
| 1 | Egypt | ~3000 BC | Gold | Warm, eternal, sunlit |
| 2 | Rome | ~100 AD | White marble | Noble, elegant |
| 3 | Viking | ~900 AD | Blue-gray | Cold, rugged, windswept |
| 4 | Medieval | ~1200 AD | Amber | Firelight and stone |
| 5 | Renaissance | ~1500 AD | Rich burgundy | Romantic, artistic |
| 6 | Frontier | 1800s | Orange | Dust, sunsets, freedom (Arizona-style) |
| 7 | Victorian | 1890s | Emerald | Sophisticated, nostalgic |
| 8 | WWII | 1940s | Muted olive | Hope amid uncertainty |
| 9 | Modern | 2020s | Natural | Authentic, grounded |
| 10 | Future | ~2500 AD | Silver & blue | Peaceful, timeless |

Plus two non-historical sequences: **The Bridge** (cosmic, between time) and **The Finale** (all-couples convergence → real photo).

---

## 6. Visual Rules (the three laws)

**Rule 1 — Every chapter contains ONE recognizable gesture.** The audience subconsciously registers it as the *same relationship*:

| Chapter | Signature gesture |
|---|---|
| Egypt | Holding hands beside the Nile |
| Rome | Fingertips touching across a marble table |
| Viking | Embracing before a voyage |
| Medieval | Meeting in a castle courtyard |
| Renaissance | He paints her portrait |
| Frontier | Dancing under lantern light |
| Victorian | Touching hands through a train window |
| WWII | A goodbye kiss before departure |
| Modern | Walking hand in hand |
| Future | Reaching for each other among the stars |

**Rule 2 — Same age throughout.** Both stay approximately their **current age** in every chapter. This is *not* reincarnation-as-rebirth (no aging up/down). It is **two souls finding each other again and again**, always recognizably themselves. (Exception by direction: Viking may read slightly *weathered/hardened* via lighting & wardrobe, not age.)

**Rule 3 — One recurring symbol in every chapter: a simple SILVER PENDANT.** Most viewers won't consciously notice it; it creates continuity:
Egyptian amulet → Roman necklace → Viking talisman → Medieval charm → Renaissance pendant → Frontier locket → Victorian locket → WWII keepsake → Modern necklace → Future holographic pendant. *Same silhouette, period-appropriate material.* (See `18_Motifs\`.)

**Rule 4 (standard) — The Reality Test** applies to every asset (see §1).

---

## 7. Color Script

Each chapter is instantly identifiable by its grade alone (see table in §5). Transitions should also *morph the color* from one chapter's palette to the next (gold→marble-white, etc.). The **Bridge** abandons all chapter palettes for deep cosmic blue/black + starlight silver. The **real-photo ending** uses *natural, ungraded* color — the deliberate visual "exhale" after the fantasy.

---

## 8. Chapter Roles & Settings (who they *are*)

| Chapter | Gary is… | Jen is… | Setting beats |
|---|---|---|---|
| Egypt | Royal architect / engineer | Noblewoman / temple scholar | Nile at sunset, monuments, gold light |
| Rome | Senator's son / military commander | Educated noblewoman | Marble temples, busy marketplace |
| Viking | Weathered, strong seafarer | Resilient, hardened by the North | Longship, northern shoreline, aurora |
| Medieval | Knight | Lady | Castle courtyard, torchlight, candlelit village |
| Renaissance | Thoughtful artist | His muse & inspiration | Workshop, paintings, candlelight |
| Frontier | Frontiersman / cowboy | Frontier woman | Horseback, dusty roads, Arizona sunset |
| Victorian | Formal gentleman | Elegant lady | Train station, handwritten letters, near-misses |
| WWII | Departing soldier | Woman waiting on the platform | Train platform, emotional separation |
| Modern | **Real present-day Gary** | **Real present-day Jen** | Coffee shop, walking hand-in-hand |
| Future | Timeless, at peace | Timeless, at peace | Glass/stone/water/trees/stars — tech invisible |

**Future direction note:** NOT a sci-fi city with flying cars. The future is **peace** — humanity matured, technology dissolved into the background, architecture timeless. Emphasis stays on *them*, not gadgets.

---

## 9. Camera Language & the Emotional Wave

Camera scale follows the song's emotional intensity. **Never** move dramatically during intimate lyrics; grow the visual scale as the orchestra grows.

```
Intensity
10 |                                   FINAL CHORUS
 9 |                                  /\
 8 |                                 /  \
 7 |                    Chorus 2    /    \
 6 |          Chorus 1 /\          /      \
 5 |                  /  \        /        \   (Bridge dip → surge)
 4 | Verse2          /    \______/          \
 3 | Verse1  ______ /                        \___ Outro
 2 | Intro  /
 1 |_______/________________________________________
        0:00                                      5:29
```

- **Intimate lyrics (verses, bridge whisper):** close mic energy → close lenses (50–85mm), slow dolly/push, minimal movement.
- **Lifts (pre-chorus → chorus):** strings rise → camera widens, swells, rises.
- **Final chorus:** full scale — wide, sweeping, cymbal-crash impacts, the all-couples convergence.
- Default lens grammar: **50mm** intimate, **35mm** environmental wide, **85mm** emotional close-up.

---

## 10. Transition Philosophy — *History Transforms*

Avoid hard cuts between chapters wherever possible. Make **history evolve around the same two people** in continuous motion:

> Egypt: fingers touch → sand blows across frame → sand becomes **marble dust** → Rome.
> Rome: he kisses her hand → sleeve becomes a **Viking fur** → Viking.
> Then: **snow → ash → flower petals → prairie dust → train steam …** one continuous move through two thousand years.

Even achieving this in a *few* hero transitions gives the film a signature identity. Where a morph isn't feasible, use a matched-motion or match-on-gesture cut (same gesture, new century).

---

## 11. The Bridge & The Ending (the two scenes people will remember)

**The Bridge — "If the world should fade tomorrow…"** This is the emotional centerpiece and the most-clipped moment. The film **leaves history entirely**: cities crumble to starlight, castles to dust, the battlefield and future city dissolve, clocks stop, photographs float away. Only stars remain. Then **"I would still find you…"** — one lone figure walks an endless star field, searching; Jen appears in the distance. No era, no costumes, just two souls. Reference tone: *Interstellar, The Fountain, Cloud Atlas, What Dreams May Come* — dreamlike, Nolan-scale, not historical drama.

**The Finale — convergence.** As the orchestra peaks, all ten couples appear, every historical pair turning toward the present-day center; the nine historical couples dissolve into light and **merge into present-day Gary & Jen.** Visual thesis, no words: *"Every path led here."*

**The Real Ending — "I finally found mine."** The future Gary & Jen look at each other; slow push in; their faces **morph into the real Gary & Jen** from an actual photograph — the AI literally disappears, reality takes over. Hold on the real photo. Slow zoom. Final piano chord rings out. Fade to black. Simple title card:

```
Ten Lifetimes
Gary & Jen
```

No credits. No effects. No logos. Just the emotional landing.

---

## 12. Recurring Motifs (`18_Motifs\`)

Reusable elements that thread every chapter together: **silver pendant** (primary), wedding ring, pocket watch, stars, clock gears, dust particles, constellations, roses, ancient map textures. Generate these once as clean reusable plates; reintroduce across chapters and especially in the Bridge.

---

## 13. Generation Order (consistency strategy)

Do **NOT** start with Egypt. Establish facial consistency in modern dress first, then move progressively further from contemporary:

**Modern → Future → Victorian → Frontier → Renaissance → Medieval → Viking → Rome → Egypt.**
(Bridge & Finale generated last, as their own dreamlike pass.)

Per the 7-shots-per-chapter target (§14), that's ~70 cinematic stills before motion.

---

## 14. Rendering & Asset Standards

**Per chapter, target 7 hero stills:** 1 hero portrait · 2 medium interaction shots · 2 environmental wides · 1 dramatic close-up · 1 cinematic ending frame. → 10 chapters ≈ **70 stills**, then animated into 5–10s clips (subtle motion: hair/cloth in wind, lantern flicker, snow, camera push, eye contact, hand movement).

**Standards for every asset:**
- 16:9, maximum photographic realism, feature-film lighting.
- Faces **must** match the master references (§4).
- The **silver pendant** present (period-appropriate).
- **No anachronisms** in historical chapters (no modern artifacts, text, logos, watches, eyeglasses unless period-correct).
- Highest available resolution; upscale as needed for 4K timeline.
- Clip length capped by tool (Sora Max: up to ~20s/clip) — design shots to that limit.

---

## 15. Production Roles & Toolchain

| Role | Who | Responsibility |
|---|---|---|
| **Executive Producer / Final Authority** | **Gary Spear** | Approves everything; nothing becomes canon without his sign-off |
| **Director** | **ChatGPT ("Sam")** | Protects the vision: bible, continuity, pacing, shot composition, work-order authoring, final QC |
| **Production Supervisor** | **Claude Code (Agent B)** | Executes work orders, maintains folders/naming, batch generation, local automation, MCP interfacing, updates the registers/logs |
| **Asset generation** | tool-specific | **Sora** = hero shots, performances, emotional close-ups, premium transitions · **Nano Banana** = reference iteration & character-consistency studies, alt compositions · **Veo / Google Flow** = long establishing shots, landscapes, atmospheric motion |
| **Post** | Adobe Premiere / After Effects / Audition | Final assembly, VFX, audio |

**Governance rule (from Atlas model):** Director authors work orders (**TL-WO-NNN**); Supervisor executes "as written" and **STOPs + REPORTs** if a work order's premise is invalidated by actual state — never silently re-interpret. Approvals flow EP → canon.

---

## 16. Film Versioning (lock gates)

| Version | Story | Timeline | Characters | Picture | Color | Audio |
|---|---|---|---|---|---|---|
| **PT-0.1** (now) | No | No | No | No | No | Locked (master delivered) |
| PT-0.5 | Yes | Yes | No | No | No | Yes |
| PT-0.9 | Yes | Yes | Yes | No | No | Yes |
| **PT-1.0** (release) | Yes | Yes | Yes | **Yes** | **Yes** | Yes |

---

## 17. Social / Distribution Strategy

Three products from one production:
1. **Full 5:29 film** — YouTube (the complete story).
2. **Short-form reels (30–60s)** — Egypt→Rome transition · WWII goodbye · Bridge reunion · final-chorus montage → TikTok / Reels / Shorts.
3. **Behind-the-scenes** — original photos, generation evolution, timeline build (the *process* draws as much engagement as the film).

Goal: emotional impact → shares/replays → organic reach. The comments we're aiming for: *"I cried," "this reminds me of my wife," "I hope someone loves me like this someday."*

---

## 18. Companion Documents (authority-based layout)

**Canonical state (`00_Production\` root):**
- `00_PROJECT_STATE.md` — single source of truth for status (read first).
- `02_Directors_Timeline.md` — the **Master Production Timeline** (one row/word; the GPS).
- `03_Shot_Database.md` — every shot (TL-####) with prompt, tool, status, narrative purpose.
- `07_Revision_Log.md` · `Risk_Register.md`.

**Evidence (subfolders):** `10_WORK_ORDERS\` (+ `00_Work_Order_Log.md`) · `11_REVIEWS\` · `12_APPROVALS\` · `13_RENDER_LOGS\` (`Render_Register.md`) · `20_REFERENCE\` (`Asset_Register.md`, `Continuity_Report.md`, `Lyrics_Annotated.md`) · `21_STYLE_GUIDES\` · `22_CAMERA_BIBLE\` · `23_CHARACTER_BIBLE\` · `30_EXPORTS\`.
- `..\START_HERE.md` — quick pointer into the system.
