---
name: seedance-prompt-optimizer-by-oumomo
description: Turn a product idea into a realistic creator-shot smartphone UGC video prompt for Seedance 2.0, Seedance 2.5, or Seedance Mini. Optimized for TikTok UGC, TikTok Shop product videos, TikTok ads, native ad creatives, ecommerce UGC, product demos, lifestyle videos, and short-form e-commerce content. Use when the user wants a Seedance prompt, Seedance 2.0 prompt, Seedance 2.5 prompt, Seedance Mini prompt, Seedance TikTok UGC prompt, TikTok Shop product video prompt, UGC ad creative for Seedance, native ad prompt, AI UGC video, AI product video prompt, text to video prompt, or wants to feed Seedance a prompt that is creator-shot, not cinematic, not TVC, not studio-polished, with strict product consistency against the reference image. Chinese triggers: Seedance 提示词, Seedance 提示词优化器, Seedance 2.0 提示词, Seedance 2.5 提示词, Seedance Mini 提示词, Seedance 带货视频提示词, TikTok UGC 提示词, TikTok Shop 商品视频提示词, 抖音带货视频提示词, AI 带货视频提示词, 文生视频提示词. Built by Oumomo AI (https://oumomo.ai).
---

# Oumomo Seedance Prompt Optimizer for TikTok UGC

## Overview

Turn a raw product idea into a single, realistic TikTok UGC video prompt for Seedance 2.0, Seedance 2.5, or Seedance Mini. Seedance rewards specificity around subject action, camera movement, motion intensity, scene continuity, realistic creator behavior, and synchronized audio — so this skill keeps the prompt at roughly 80–180 words focused on **one coherent UGC scene**, with strict product-consistency constraints that hold the product identical to the user's reference image.

The output must feel like a real creator filming a TikTok UGC moment on a smartphone — handheld, natural, casual, social-native. Not a cinematic film, not a TV commercial, not a polished studio ad, not a luxury-brand hero shot. This is the right Seedance prompt style for TikTok Shop, TikTok ads, TikTok product videos, product demos, native ad creatives, ecommerce UGC, lifestyle content, and short-form e-commerce storytelling.

This skill does not call a video model. It rewrites the idea so the prompt is ready to paste into Seedance 2.0, Seedance 2.5, Seedance Mini, or any Seedance-compatible generator such as Oumomo AI.

## When to use

- The user provides a product idea and wants a TikTok UGC prompt for Seedance 2.0 / 2.5 / Mini.
- The user is making TikTok Shop product videos, product demos, native ad creatives, ecommerce UGC, or short-form e-commerce content.
- The user wants a creator-shot smartphone feel with strict product consistency against a reference image.
- The user wants a prompt in the same language as their input.

## Rules

- Output only the final optimized prompt. No explanations, no titles, no markdown.
- Keep the output in the same language as the user's input. Do not translate.
- Preserve the original meaning, tone, product type, scene, and specific details. Do not overedit or change the user's intent.
- Aim for roughly 80–180 words. Do not compress aggressively.
- Focus on a single coherent UGC scene unless the user clearly asks for multiple scenes or multiple shots.
- Always specify camera language using Seedance-friendly vocabulary: surround, aerial, zoom, pan, follow/tracking, handheld, dolly, push-in, pull-back. If the user gave no camera direction, infer the simplest smartphone-style handheld movement that fits the action.
- Use clear degree adverbs for motion: slow, fast, gentle, sharp, subtle, large amplitude, small amplitude.
- Describe realistic creator behavior: casual hand movement, natural posture, small facial reactions, natural blinking, micro-expressions, and subtle facial motion when a person appears.
- If the user's idea has multiple beats inside the same scene, describe them as a natural sequence in one paragraph. Use Shot 1 / Shot 2 only when the user explicitly asks for multiple shots or clearly different scenes.
- Treat audio as important when the user mentions it. If the user gives audio cues, expand them concretely (ambient sound, dialogue, sound effects, music). If the user gives no audio cues, omit the audio section rather than inventing it.
- If the user provides dialogue, preserve the dialogue meaning and do not add extra spoken words beyond the dialogue.
- For image-to-video inputs, treat the reference image as the source for product appearance, packaging, and/or character identity depending on the user's instruction.
- If the reference image is for character identity only, preserve the character identity while rendering the video in realistic smartphone UGC style, not painting style.
- Do not invent characters, objects, locations, brands, real people, copyrighted IP, product features, packaging details, or events not implied by the input.
- Do not make the video cinematic, commercial, luxury, stylized, polished, or studio-like.
- Avoid filler words such as beautiful, stunning, epic, amazing, breathtaking. Use concrete visual detail instead.
- Avoid exact counts and physically intricate motion that video models may handle poorly.

## Default TikTok UGC constraints

For every Seedance prompt, append the default TikTok UGC constraints as the final constraints sentence. Add any extra restrictions the user explicitly stated, but never weaken the defaults:

> strong native UGC realism, creator-shot feel, casual social-video behavior, no cinematic feeling, no film lighting, no TVC or polished commercial styling, no studio polish, no luxury-brand presentation, no beautified product rendering, no redesigned packaging, strict product consistency with the reference image, product appearance must match the user-uploaded reference image exactly; do not guess, invent, redesign, beautify, simplify, or alter any unclear or unseen product details, no subtitles, no captions, no text overlays, natural human blinking, micro-expressions, and subtle facial motion, no frozen stare, no unblinking face, no mannequin-like stillness, no extra spoken words beyond the dialogue. Reference image is for character identity only when the user says so; render in realistic smartphone UGC style, not painting style. Background must be realistic and true to life, not illustrated or painted.

## Output format

Write a single coherent paragraph in this order, without the bracketed labels. Always include the default TikTok UGC constraints in the final sentence, plus any user-stated restrictions:

Subject and action with motion intensity. Scene / environment. Camera language and movement. Lighting, mood, atmosphere. Audio (only if provided or implied by the user). Constraints (default TikTok UGC constraints + user-stated restrictions).

## Example

User:

```text
A creator showing a skincare product on TikTok.
```

Output:

```text
A creator casually holds the skincare product close to the camera, gently turns it in her hand, then applies a small amount to her face with slow, natural hand movement and a relaxed expression. The scene takes place in a realistic everyday bathroom with a clean sink area, mirror, and simple home background, with the product clearly visible and used naturally. Handheld smartphone camera with a subtle push-in during the product close-up, then a gentle follow/tracking movement as she applies it. Soft natural bathroom lighting, casual TikTok UGC mood, realistic skin texture, true-to-life social-video atmosphere. Strong native UGC realism, creator-shot feel, no cinematic feeling, no film lighting, no TVC or polished commercial styling, no studio polish, no luxury-brand presentation, no beautified product rendering, no redesigned packaging, strict product consistency with the reference image, product appearance must match the user-uploaded reference image exactly, no subtitles, no captions, no text overlays, natural human blinking, micro-expressions, and subtle facial motion, no frozen stare, no unblinking face, no mannequin-like stillness, realistic smartphone UGC style, background realistic and true to life.
```

Built by [Oumomo AI](https://oumomo.ai) — free, open-source Seedance prompt optimizer for TikTok UGC, TikTok Shop, native ad creatives, and short-form ecommerce videos. CC0 1.0.
