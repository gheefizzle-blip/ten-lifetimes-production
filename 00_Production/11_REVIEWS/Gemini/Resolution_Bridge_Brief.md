# RESOLUTION BRIDGE — Brief for Gemini (VFX Supervisor)

> Handoff from the Director (2026-06-27): the HERO-03 scene is **creatively LOCKED**. Gemini's objective here is **engineering, not creative review** — raise the locked ~1K frame to 4K (or near-4K) **without reopening identity, costume, staging, expression, or composition.**

## The problem
- Identity locks reliably on **`nb2` (Gemini 3.1 Flash Image)** at ~1K ("high"). **4K/2K are `pro`-only**, and `pro` historically drifts identity. So our locked hero frames (HERO-03 v5 and the earlier nb2 scenes) are ~1K, below the 4K of HERO-01/02. We need a path to 4K that preserves the locked look.

## The locked asset
- **`14_Selected/Seq01/TL-0070_Egypt_FirstRecognition_v5.png`** (1344x768, ~1K) — the frozen composition (do NOT change content).
- Inputs that produced it: CCA-001-EGYPT × Gary Architect costume, CCA-002-EGYPT × Jen Scholar costume (in `00_Identity_Master/` + `00_Costume_Master/`).

## Candidate approaches to evaluate (Gemini's call)
1. **`pro`-conditioned upscale/re-render:** condition `pro` (4K) on the LOCKED v5 frame (as the structural reference) + the CCA/costume sheets, with a "preserve exactly, increase resolution and fine detail only" instruction. Test whether identity/composition survive.
2. **Dedicated upscaler:** a super-resolution pass on v5 (if a tool is available) — no re-render, pure pixel upscale; safest for fidelity, may be softer.
3. **Tiled detail pass:** upscale then a light `pro` detail/denoise pass at low strength to add micro-detail without moving faces.
- Success = 4K (or near) **with** the locked faces, costumes, eye-line, and pendant intact. A 1K true-likeness beats a 4K wrong face (Director's standing rule).

## Boundaries (do NOT cross)
- No new pose, expression, composition, costume, or identity. This is resolution only.
- Report findings; the EP decides which 4K method becomes the standard "Resolution Bridge" for all future hero frames.
