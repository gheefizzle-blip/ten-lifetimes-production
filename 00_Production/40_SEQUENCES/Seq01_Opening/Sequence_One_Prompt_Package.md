# SEQUENCE ONE — Prompt Package (TL-WO-004 #11)

> **Scaffold — Supervisor builds once the Storyboard/Direction docs are authored.** ⚠️ **GATED on B-1 (generation-tooling host).** Prompts are translated from the Director's creative direction, not invented.

## Hero stills - first pass (VFX-001, 2026-06-26, Nano Banana Gemini-3-Pro-Image)
Params: model_tier `pro`, 16:9, resolution 2k, thinking_level high, grounding on. Output (local, not committed): `C:\Users\Gary\nanobanana-images\`.

| Prompt ID | Shot/beat | Master refs (conditioning) | Render ID (file) | Status |
|---|---|---|---|---|
| PR-S1-001 | Gary - Egypt lonely walk (hero, pre-recognition) | Gary_01/02/03 | `TL-Seq1_Egypt_Gary_hero_v1.png` | STILL_GEN - awaiting GVR/review |
| PR-S1-002 | Jen - Egypt, walking toward (hero) | Jen_01/02/03 | `TL-Seq1_Egypt_Jen_hero_v1.png` | STILL_GEN - awaiting GVR/review |
| PR-S1-003 | Recognition two-shot (the sequence's defining frame) | Gary_01 + Jen_01 | `TL-Seq1_Egypt_Recognition_v1.png` | STILL_GEN - awaiting GVR/review |

> Full prompt text for each is recorded in the VFX-001 operation report. These are a **look-establishing pass** for Director review + Gemini GVR + EP approval -> then LOCK the visual language (Production Loop step 5) before supporting stills.
> **Supervisor notes for iteration:** (a) recognition two-shot did not fully capture the eye-contact choreography (he looks first / she hesitates then smiles) - they read side-by-side; needs staging retake. (b) Jen hero leans toward temple "spectacle" vs Sam's "quiet path, no spectacle." (c) pendant present but not yet the "catches the light first" beat.

## Build rules
- Every human shot cites the locked master refs; **strip modern styling** (Gary cap/glasses, Jen dyed hair/nose ring).
- Encode the Three Recognition Rules where applicable (notices first / smiles second / pendant catches light first).
- Period-correct; correct chapter grade; pendant present; Reality Test.
- Prompt IDs register back into `MASTER_PRODUCTION_TIMELINE.md` + `Asset_Register.md`.

## Tooling (B-1 — verified 2026-06-25, GSA-1000)
- **Stills: Nano Banana MCP `mcp__nanobanana__generate_image` is LIVE.** Use **multi-image conditioning** with the 3 master refs (input_image_path_1/2/3), `aspect_ratio: 16:9`, `model_tier: pro` + `resolution: 4k` for hero stills, `enable_grounding: true` for period accuracy. Output → `C:\Users\Gary\nanobanana-images` (move approved stills to NAS chapter `Stills\`, register in Asset Register).
- **Motion: Veo/Sora — no direct bridge.** Native web + manual download → Gemini GVR. (Future: n8n route.)
- **Master refs:** interim set locked; fresh portrait set recommended before *final* renders.

> Generation still gated on: Director authoring the Storyboard/Direction, then EP approval of the prompt package (workflow Bible §0d).
