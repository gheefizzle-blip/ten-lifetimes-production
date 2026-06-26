# SEQUENCE ONE — Prompt Package (TL-WO-004 #11)

> **Scaffold — Supervisor builds once the Storyboard/Direction docs are authored.** ⚠️ **GATED on B-1 (generation-tooling host).** Prompts are translated from the Director's creative direction, not invented.

## Hero stills - first pass (VFX-001, 2026-06-26, Nano Banana Gemini-3-Pro-Image)
Params: model_tier `pro`, 16:9, resolution 2k, thinking_level high, grounding on. Output (local, not committed): `C:\Users\Gary\nanobanana-images\`.

| Prompt ID | Shot/beat | Master refs (conditioning) | Render ID (select) | Status |
|---|---|---|---|---|
| PR-S1-001 | Gary - Egypt lonely walk (hero, pre-recognition) | Gary_01/02/03 | `TL-Seq1_Egypt_Gary_hero_v1.png` | **SELECT** - awaiting GVR-001 |
| PR-S1-002 v2 | Jen - Egypt, walking toward (hero) | Jen_01/02/03 | `TL-Seq1_Egypt_Jen_hero_v2.png` | **SELECT** - awaiting GVR-002 (v1 superseded) |
| PR-S1-003 v3 | Recognition two-shot (the sequence's defining frame) | Gary_02+Gary_01 + Jen_01 | `TL-Seq1_Egypt_Recognition_v3.png` | **SELECT** - awaiting GVR-003 (v1/v2 superseded) |

> Full prompt text for the first pass is in the VFX-001 report; retake prompts (v2/v3) are in the **VFX-002** report. These are a **look-establishing pass** for Director review + Gemini GVR + EP approval -> then LOCK the visual language (Production Loop step 5) before supporting stills.
> **VFX-002 retake resolutions (2026-06-26):** (a) **Recognition v3** - gaze choreography fixed: explicit "he looks directly at her, not smiling / she hesitates then gives a gentle questioning smile"; the v2 model had added modern eyeglasses (anachronism), removed in v3 via negative prompt + bare-face master ref; pendant now catches the light. (b) **Jen hero v2** - returned to Sam's quiet Nile dawn path; temple/columns/spectacle removed via negative prompt; tighter face match at 4k. (c) Gary hero v1 held unchanged as the lock candidate.
> **Standing prompt lesson (period eyewear rule, EP 2026-06-26):** Nano Banana injects modern eyewear onto an older male subject unprompted. **Gary is bare-eyed (NO glasses) in every chapter before WWII** (Egypt/Rome/Viking/Medieval/Renaissance/Frontier/Victorian) - carry `glasses, eyeglasses, spectacles, eyewear` in his negative prompt and prefer the bare-face master ref for all of these. Glasses are allowed only WWII onward (WWII/Modern/Future). See Character Bible "Gary eyewear - PERIOD RULE."

## Build rules
- Every human shot cites the locked master refs; **strip modern styling** (Gary cap/glasses, Jen dyed hair/nose ring).
- Encode the Three Recognition Rules where applicable (notices first / smiles second / pendant catches light first).
- Period-correct; correct chapter grade; pendant present; Reality Test.
- Prompt IDs register back into `MASTER_PRODUCTION_TIMELINE.md` + `Asset_Register.md`.

## Tooling (B-1 — verified 2026-06-25, GSA-1000)
- **Stills: Nano Banana MCP `mcp__nanobanana__generate_image` is LIVE.** Use **multi-image conditioning** with the 3 master refs (input_image_path_1/2/3), `aspect_ratio: 16:9`, `model_tier: pro` + `resolution: 4k` for hero stills, `enable_grounding: true` for period accuracy.
- **OUTPUT GOES TO THE NAS VAULT — never C:.** Set `output_path` to the chapter's NAS `Stills\` folder, e.g. `D:\My_Music\Ten_Lifetimes\04_Egypt\Stills\<name>.png` (Egypt). Approved stills → chapter `Final\`. Register all in the Asset Register. (Media never committed to GitHub.)
- **Motion: Veo/Sora — no direct bridge.** Native web + manual download → Gemini GVR. (Future: n8n route.)
- **Master refs:** interim set locked; fresh portrait set recommended before *final* renders.

> Generation still gated on: Director authoring the Storyboard/Direction, then EP approval of the prompt package (workflow Bible §0d).
