---
name: image2-realistic-texture
description: Generate prompt-only high-end realistic OpenAI image-2 prompts from modular texture recipes. Use when the user asks to write, make, generate, or refine a ChatGPT/image-2 prompt for realistic portraits, fashion-cover portraits, studio beauty close-ups, skin texture, eyes, hair, hands, commercial group portraits, or "no AI-looking" photo realism. This skill outputs precise prompts only and must not generate images.
---

# Image2 Realistic Texture

## Purpose

Create image-2-ready prompts that turn a short image request into a high-end realistic photography prompt. Keep the output focused on believable biological texture, optical realism, controlled lighting, restrained post-processing, and natural-language avoidance constraints. This skill is prompt-only: it must prepare text for the user to copy into ChatGPT/image-2.

## Core Workflow

1. Identify the scene family from the user's request.
   - Read `references/scene-recipes.md` first.
   - If the scene is one of the supported recipes, use that recipe.
   - If the scene is close but not exact, choose the nearest recipe and lightly adapt it.
2. Select only the modules needed for the scene.
   - Read `references/module-library.md` for reusable texture, lighting, camera, imaging, and post-production modules.
   - Do not include every module by default. Use the fewest modules that make the scene convincing.
3. Add natural-language avoidance constraints.
   - Read `references/negative-constraints.md` and choose only relevant errors to avoid.
   - Phrase constraints for image-2 as "避免..." or "不要..." instead of negative-prompt syntax.
4. Preserve the user's subject, setting, mood, and composition.
   - Put the user's subject and framing first.
   - Add realism modules after the subject.
   - Do not overwrite the user's creative intent unless it conflicts with realism or safety.
5. Output in Chinese by default.
   - Use English only if the user asks for English.
   - Keep the prompt as one polished, directly usable prompt unless the user asks for variants.

## Output Rules

- Optimize for OpenAI image-2.
- Do not output Midjourney parameters such as `--ar`, `--style`, `--raw`, `--s`, `--chaos`, `--seed`, or `--no`.
- Do not output Stable Diffusion fields such as `negative_prompt`, `guidance_scale`, `steps`, `sampler`, `CFG`, or `strength`.
- Use natural language for constraints: "避免塑料皮肤、蜡面肌肤、过度磨皮..."
- Never call an image generation tool from this skill.
- Even if the user says "生成图片", "制作图片", "出图", "画一张", or similar, output only the complete prompt text that the user can send to ChatGPT/image-2.
- Do not describe that an image was generated. Do not attach, preview, or save images.

## Prompt Shape

Use this order:

```text
[主体与构图]，[生物微结构]，[眼部/毛发/嘴唇/牙齿/手部等相关局部]，[光线]，[镜头与成像]，[后期]。避免[相关错误]。
```

If the user's request is ambiguous, make one concise assumption before the prompt:

```text
我按“棚拍美容近景”处理。

[完整 image-2 提示词]
```

Ask a clarification question only when the missing choice materially changes the prompt, such as portrait versus product-only imagery.

## Supported Scene Families

- Studio beauty close-up.
- Outdoor golden-hour portrait.
- Three-quarter commercial portrait.
- Head-and-shoulders close-up.
- Hand detail close-up.
- Skincare-style skin texture close-up.
- Hyperreal eye macro.
- Multi-person commercial group portrait.

## Restraint Principles

- Prefer "自然、轻微、克制、受控、细腻" over exaggerated intensity.
- Keep skin believable: visible pores and microtexture, not flat perfection.
- Keep eyes alive: subtle tear-film reflection and iris texture, not glassy CG eyes.
- Keep hair physical: grouped strands plus a few flyaways, not helmet-like blocks.
- Keep lighting photographic: controlled softbox, beauty dish, rim light, or golden-hour geometry.
- Keep post-processing restrained: subtle commercial grading, light dodge and burn, and light frequency-separation-style retouching while preserving texture.
- Avoid piling on conflicting film stocks, extreme grain, heavy glow, or over-sharpening.

## Safety

If a request involves a real identifiable person, a brand/logo, protected packaging, or an "official ad" imitation, avoid implying permission. Keep the prompt generic unless the user confirms they have rights or consent.
