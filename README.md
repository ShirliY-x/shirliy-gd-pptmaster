# Shirliy｜极客PPT大师

这是一个用于 Codex 的客户方案 PPT 图片生成工作流 Skill。它不会默认直接生成可编辑 PPT 文件，而是引导 Codex 按照“项目理解 → 文本版大纲 → 风格确认 → 整套缩略总览图 → 逐页 16:9 高清页面图片 Prompt → 人工复核”的方式，协助生成更适合客户沟通、商务汇报、方案洽谈的 PPT 页面图片。

## Skill 信息

- GitHub 项目名：`shirliy-gd-pptmaster`
- Skill 技术名：`shirliy-gd-pptmaster`
- Skill 展示名：`Shirliy｜极客PPT大师`
- 默认公司风格：`GeekDance Official Business Style`
- 默认背景图：`.agents/skills/shirliy-gd-pptmaster/assets/geekdance-default-background.jpg`
- 默认页面比例：16:9 横版
- 默认点缀色：GeekDance 品牌红

## 目录结构

```text
shirliy-gd-pptmaster/
├── README.md
├── .gitignore
├── examples/
│   └── example-session.md
└── .agents/
    └── skills/
        └── shirliy-gd-pptmaster/
            ├── SKILL.md
            ├── assets/
            │   └── geekdance-default-background.jpg
            └── references/
                ├── workflow.md
                ├── prompt-templates.md
                ├── company-style-guide.md
                ├── interaction-options.md
                └── review-checklist.md
```

## 推荐使用方式

在 Codex 中调用：

```text
使用 $shirliy-gd-pptmaster，基于我上传的客户资料，先做项目理解，再一步一步生成方案汇报 PPT 大纲和页面图片 Prompt。
```

或者：

```text
使用 Shirliy｜极客PPT大师，采用公司风格，帮我做客户方案汇报 PPT 的文本大纲和逐页图片生成 Prompt。
```

## 核心规则

1. 不要一次性走完整个流程，必须每一步向用户确认。
2. 默认不直接生成 PPT 文件。
3. 默认先生成文本版 PPT 大纲。
4. 默认先确认风格，再生成总览图。
5. 默认先确认总览图，再逐页生成高清单页图片 Prompt。
6. 逐页阶段每次只处理一页。
7. 每个关键选择都必须包含“由 ShirliY AI 做决定”。
8. 公司风格必须使用 GeekDance 通用背景图、16:9 横版、红色点缀、右上角 Logo、浅色大水印、圆角卡片和商务科技感表达。
