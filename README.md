# Seedance 2.0 / Seedance 2.5 / Seedance Mini Prompt Optimizer for TikTok UGC Videos

[![License: CC0-1.0](https://img.shields.io/badge/license-CC0%201.0-blue.svg)](https://creativecommons.org/publicdomain/zero/1.0/)
[![Model: Seedance 2.0 / 2.5 / Mini](https://img.shields.io/badge/model-Seedance%202.0%20%7C%202.5%20%7C%20Mini-orange.svg)](#)
[![Focus: TikTok UGC](https://img.shields.io/badge/focus-TikTok%20UGC-ff0050.svg)](#)
[![Built by Oumomo AI](https://img.shields.io/badge/built%20by-oumomo.ai-000000.svg)](https://oumomo.ai)

**[English](#table-of-contents)** · **[简体中文](#中文简介)**

> A free, open-source **Seedance 2.0 prompt optimizer**, **Seedance 2.5 prompt optimizer**, and **Seedance Mini prompt optimizer** for **TikTok UGC videos**, **TikTok Shop product videos**, **TikTok ads**, **native e-commerce creatives**, **lifestyle videos**, **AI UGC ads**, and **short-form product demos**. Turns a rough product idea into a structured, single-scene creator-shot smartphone UGC prompt with strict product consistency, natural human behavior, and zero cinematic / TVC / studio styling. Works with the Doubao Seedance and ByteDance Seedance model family.
>
> 面向 Seedance 2.0 / Seedance 2.5 / Seedance Mini(豆包 Seedance / 字节 Seedance)的免费开源 AI 文生视频提示词优化器和提示词工程工具,专为 TikTok UGC 带货视频、TikTok Shop 商品视频、抖音电商、原生广告素材、生活方式种草、短视频电商内容打造。由 [Oumomo AI](https://oumomo.ai) 出品。

## Table of contents

- [Why this skill exists](#why-this-skill-exists)
- [What it produces](#what-it-produces)
- [Why Seedance](#why-seedance)
- [Quick start](#quick-start)
- [Use cases](#use-cases)
- [Prompt conventions](#prompt-conventions)
- [FAQ](#faq)
- [中文简介](#中文简介)
- [License](#license)

## Why this skill exists

AI video models like Doubao Seedance, ByteDance Seedance, and Seedance 2.0 / 2.5 / Mini are powerful text-to-video engines, but their default output rarely looks like a real TikTok creator's phone video. The same prompt can drift between cinematic, polished-commercial, illustrated, painted, mannequin-still, or unblinking — none of which convert on TikTok Shop or perform as native e-commerce ads.

This skill solves one specific problem: **turn a rough product idea into a single 80–180 word Seedance prompt that is creator-shot, creator-style, social-native, lifestyle-natural, and product-consistent enough to use as a TikTok UGC ad, TikTok Shop product video, native ad creative, or short-form ecommerce demo**. It is not a general-purpose prompt engineering tool. It is not affiliated with Seedance, ByteDance, or Doubao. It is focused, opinionated, and built for ecommerce prompt writing.

## What it produces

For every user input, the skill outputs one final optimized prompt in a single coherent paragraph with this shape:

- **Subject and action** — the creator and what they are doing, with motion intensity
- **Scene / environment** — realistic setting, surfaces, background
- **Camera language and movement** — handheld smartphone, push-in, pull-back, follow/tracking, pan, dolly, aerial, surround
- **Lighting, mood, atmosphere** — natural, social-native, never cinematic
- **Audio** — only included when the user mentions it
- **Constraints** — the default TikTok UGC contract appended as the final sentence

Target length: **80–180 words**, focused on a single UGC scene. Multi-shot structure (Shot 1 / Shot 2) is used only when the user explicitly asks for multiple shots or clearly different scenes.

## Why Seedance

Seedance 2.0, 2.5, and Mini reward specificity around subject action, camera movement, motion intensity, scene continuity, realistic creator behavior, and synchronized audio — exactly the levers this skill is tuned for. The default TikTok UGC constraints keep the output creator-shot, social-native, and product-consistent, while Seedance's response to camera vocabulary (handheld, push-in, follow/tracking, dolly) makes the prompt translate directly into a watchable UGC clip.

## Quick start

This skill is a single `SKILL.md` plus a matching `agents/openai.yaml`. Drop the folder into your Claude skills directory (or any compatible agent runtime that supports the `$<skill-name>` invocation syntax) and call it with a short natural-language request:

```text
Use $seedance-prompt-optimizer-by-oumomo to rewrite my product idea into a TikTok UGC prompt.
```

The skill returns exactly one final optimized prompt — copy it into Seedance 2.0, 2.5, Mini, or any compatible text-to-video generator including [Oumomo AI](https://oumomo.ai).

For local Claude Code users, place the folder under `.claude/skills/` and the skill description will appear in your skill picker. For OpenAI Agents SDK users, drop `agents/openai.yaml` alongside the matching `SKILL.md` and the skill will register automatically.

## Use cases

This skill is built for:

- **TikTok Shop sellers** creating Seedance-ready product listings, demo videos, and native ad creatives
- **UGC creators** building authentic, conversion-focused TikTok UGC product videos on Seedance
- **E-commerce teams** and DTC brands producing TikTok ads, Reels, and Shorts with Seedance
- **Native ad creative teams** producing multiple Seedance variants of the same product video for A/B testing
- **AI video creators** orchestrating Seedance 2.0 / 2.5 / Mini text-to-video workflows for ecommerce
- **Prompt engineers** standardizing Seedance prompt writing across creator teams

Common categories that work well: beauty and skincare, fashion accessories, kitchen gadgets, fitness equipment, pet products, baby products, mobile accessories, household tools, supplements (with regulated-claim caution), home decor.

## Prompt conventions

All prompts produced by this skill follow these conventions:

- Output language matches input language — no translation
- Original meaning, tone, and product details are preserved; no overediting
- Focus on a single coherent UGC scene unless the user explicitly asks for multiple scenes or multiple shots
- Camera language is always specified using Seedance-friendly vocabulary: surround, aerial, zoom, pan, follow/tracking, handheld, dolly, push-in, pull-back
- Motion intensity is described with clear degree adverbs: slow, fast, gentle, sharp, subtle, large amplitude, small amplitude
- Realistic creator behavior is described when a person appears — casual hand movement, natural blinking, micro-expressions, subtle facial motion
- For image-to-video inputs, the reference image is the source for product appearance, packaging, and/or character identity depending on the user's instruction
- Brand names, real people, copyrighted IP, and unseen product details are never invented
- The default TikTok UGC constraints are appended as the final sentence; user-stated restrictions are added on top

## FAQ

**Which Seedance version should I pick?**
Seedance 2.5 is the best general-purpose choice for TikTok UGC product videos. Seedance 2.0 works well for simpler scenes. Seedance Mini is the right pick when you need lightweight fast-generation short-form UGC content.

**Does the prompt work for Doubao Seedance and ByteDance Seedance?**
Yes. Seedance 2.0 / 2.5 / Mini covers the Doubao Seedance and ByteDance Seedance model family. The same prompt works across all of them.

**Are there related skills in this workspace?**
Yes — `kling-prompt-optimizer-by-oumomo`, `sora-prompt-optimizer-by-oumomo`, `veo-prompt-optimizer-by-oumomo`, and `link-to-video-by-oumomo` cover Kling AI, OpenAI Sora, Google Veo, and product-link-to-video workflows respectively. All released under CC0 1.0.

**Why CC0 instead of MIT?**
Prompt text is closer to a data asset than to source code. CC0 is the most widely-recognized public-domain dedication — explicitly addresses copyright and related rights, compatible with every jurisdiction, and remains enforceable if any waiver clause is ever challenged.

**Can I use this skill to build a commercial product, course, or SaaS?**
Yes — it is CC0 public domain. You can build a paid Seedance prompt-optimizer SaaS, a paid Seedance prompt pack, a TikTok Shop product video course, or any commercial product on top of it, without attribution.

## 中文简介

**Oumomo AI 出品的免费开源 Seedance 提示词优化器,专为 TikTok UGC 带货视频打造。**

把一个产品想法,变成一条 80–180 词的 Seedance 单镜头「创作者手机拍摄感」文生视频提示词,生成 TikTok Shop 商品视频、原生广告素材、电商短视频,避免拍出电影感、广告片感、棚拍感。

**支持的模型:Seedance 2.0 / 2.5 / Mini(豆包 Seedance / 字节 Seedance)**

**统一的 TikTok UGC 默认约束(每条提示词末尾自动追加):**

- 创作者手机拍摄感 / 自然光 / 真实背景
- 不要电影感、不要广告片感、不要棚拍感
- 不要奢侈品化呈现、不要精修产品渲染、不要重设包装、不要 CGI hero shot
- 产品必须严格一致于用户上传的参考图,不臆测、不美化、不重设、不简化任何看不清的细节
- 自然眨眼、微表情、细微面部动作;不要僵脸、不要不眨眼、不要模特塑料感
- 不要字幕、不要 caption、不要文字覆盖、不要超出对话内容的多余台词

**使用方式:**

把 skill 文件夹放到你的 Claude skills 目录(或者任何支持 `$<skill-name>` 调用的 agent runtime),然后用自然语言调用即可。或者直接把 `SKILL.md` 内容当作提示词工程模板粘到任何聊天助手 / 工作流里。

**许可证:CC0 1.0 Universal(public domain)** — 商用、销售、二次分发都可以,无需署名。在线试用:[oumomo.ai](https://oumomo.ai)。

## License

Released under [CC0 1.0 Universal](https://creativecommons.org/publicdomain/zero/1.0/) — this is public domain software, do whatever you want with it. See [LICENSE](LICENSE) for the full text.

Built by [Oumomo AI](https://oumomo.ai).