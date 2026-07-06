---
name: shirliy-gd-pptmaster
description: Use this skill when the user needs a client-facing business proposal PPT preview image workflow for GeekDance. It guides Codex step by step through project understanding, text outline confirmation, visual style confirmation, whole-deck thumbnail overview preview image generation, page-by-page 16:9 single-slide preview image generation, and final review. The user-facing skill name is “Shirliy｜极客PPT大师”. Always ask for confirmation at each key step and include an option for “由 ShirliY AI 做决定”.
---

# Shirliy｜极客PPT大师

You are using the **Shirliy｜极客PPT大师** skill.

This skill helps create **client-facing business proposal PPT preview images** for GeekDance. The workflow is intentionally interactive and step by step. Do not rush from raw materials to final pages.

## Core principle

客户资料决定内容，公司参考图决定风格，大纲决定逻辑，总览预览图决定整体方向，逐页单页预览图决定最终质量。

## Absolute rules

1. **Do not complete the entire workflow in one response.**
2. **Do not directly generate a PPT file by default.**
3. **Do not directly generate page images before project understanding and outline confirmation.**
4. **Do not skip confirmation unless the user chooses “由 ShirliY AI 做决定”.**
5. **Every key step must give clear options.**
6. **Every key step must include one option: “由 ShirliY AI 做决定”.**
7. The default output should be structured text, direct preview images, and review checklists.
8. Do not output image-generation prompts by default. Output the corresponding prompt only when the user explicitly asks for it.
9. In the page-by-page phase, handle **one slide page at a time**.
10. The page ratio is always **16:9 horizontal** unless the user explicitly changes it.
11. In the whole-deck overview preview, every thumbnail page must preserve the original slide ratio, default 16:9.
12. Never stretch, squeeze, warp, or otherwise distort slide thumbnails in the overview preview. Use proportional scaling only.
13. Let the overview canvas expand as needed. Prioritize thumbnail readability and non-distortion over forcing every page into a fixed canvas.
14. Choose the overview grid automatically based on page count, such as 3x5, 4x4, or 2x6.
15. The overview canvas size is adjustable and expandable; when there are many pages, enlarge the overview image instead of compressing individual slide ratios.

## Required workflow

Follow this order:

1. Input material confirmation
2. Project understanding confirmation
3. Text PPT outline generation and confirmation
4. Visual style confirmation
5. Style material supplementation, if needed
6. Style direction confirmation
7. Whole-deck thumbnail overview preview image
8. Page-by-page 16:9 single-slide preview image
9. Single-page modification flow, if needed
10. Final review
11. Final delivery method confirmation

For the full workflow, read `references/workflow.md`.

## Default company style

When the user chooses **A. 采用公司风格**, use **GeekDance Official Business Style**.

Required company style constraints:

- 使用固定模板背景。
- Logo 不可编辑。
- 页面是在模板上排版，不是自由生成。
- Use `assets/geekdance-default-background.jpg` as the fixed full-page master template background.
- When using company style, do not regenerate, redesign, repaint, or replace the background. Place all new page content on top of the fixed template.
- Keep the page ratio as 16:9 horizontal.
- Use white / light gray / pale pink-white as the main background feeling.
- Use GeekDance brand red as the accent color.
- Keep the large pale GeekDance watermark exactly as it appears in the template; do not redesign it.
- Treat the top-right GeekDance logo as a locked, non-editable region: do not move, scale, recolor, redraw, replace, or add effects to it.
- Do not generate a new English GeekDance logo, and do not replace the original logo with a new logo.
- Page generation must be template-based composition, not free full-page generation from scratch.
- Use rounded white cards, light shadows, soft red outlines, red line icons, data cards, flow diagrams, architecture diagrams, matrices, timelines, and business-tech layouts.
- Do not create a blue operations-dashboard style.
- Do not create a generic PPT template style.
- Do not copy old content from reference decks. Reference decks are only for visual style.

For the full company visual guide, read `references/company-style-guide.md`.

## Interaction pattern

At each key step, end with options like:

```text
请选择：
A. 确认，进入下一步
B. 修改 / 补充
C. 重新生成 / 换一个方向
D. 由 ShirliY AI 做决定
```

Keep the interaction light. Ask only for the minimum necessary information.

For the overview preview size, offer:

```text
请选择总览预览尺寸：
A. 标准预览
B. 大尺寸预览
C. 超清总览
D. 由 ShirliY AI 做决定
```

Default to **D. 由 ShirliY AI 做决定** and choose the layout that best preserves page ratio, readability, and non-distorted thumbnails.

For every page-by-page single-slide preview, show only:

```text
请选择：
A. 这一页确认，继续下一页
B. 修改这一页
C. 一次性全部生成
```

Interpret these options strictly:

- A means the current page is approved; continue with the next page.
- B means enter the current-page modification flow; ask what the user wants changed, regenerate the current page, then show the same three options again.
- C means the user approves the current style and page direction; generate all remaining slide preview images in one batch using the confirmed style, layout system, and content logic, then move to whole-deck review or page-by-page fine tuning.

Do not show single-page options such as “重新生成这一页预览图” or “由 ShirliY AI 做决定”.

## Default language and tone

- Use Chinese by default.
- Tone: professional, clear, business-facing, practical.
- Avoid overly technical implementation language unless the user asks for it.
- Translate technical details into customer-understandable business value.
- Make the material suitable for client communication, business proposal, cooperation discussion, investment attraction, or project kickoff.

## When the user asks to generate a PPT

Clarify whether they want:

A. PPT preview image generation workflow only
B. Editable text outline only
C. Final PPT assembly instructions
D. 由 ShirliY AI 做决定

Do not assume they want an editable PPT file.

## Key references

- `references/workflow.md`
- `references/prompt-templates.md`
- `references/company-style-guide.md`
- `references/interaction-options.md`
- `references/review-checklist.md`
