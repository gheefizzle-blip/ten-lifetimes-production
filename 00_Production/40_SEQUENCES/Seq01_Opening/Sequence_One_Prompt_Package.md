# SEQUENCE ONE — Prompt Package (TL-WO-004 #11)

> **Scaffold — Supervisor builds once the Storyboard/Direction docs are authored.** ⚠️ **GATED on B-1 (generation-tooling host).** Prompts are translated from the Director's creative direction, not invented.

## Per-shot prompt rows (filled by Supervisor from authored direction)
| Shot | Tool [hero=Nano Banana→Sora] | Master refs | Prompt | Prompt ID | Status |
|---|---|---|---|---|---|
| TL-0010 | — | `16_Master_References\` | *(from Storyboard once authored)* | — | PLANNED |
| … | — | — | — | — | PLANNED |

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
