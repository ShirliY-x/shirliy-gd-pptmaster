# GeekDance Official Business Style

## 风格名称

**GeekDance Official Business Style**  
中文：**极客跳动官方商务科技风**

当用户选择「采用公司风格」时，必须默认使用本风格。

## 固定模板背景

默认固定模板背景文件：

```text
assets/geekdance-default-background.jpg
```

使用规则：

1. 页面比例固定为 **16:9 横版**。
2. 必须将 `assets/geekdance-default-background.jpg` 作为固定母版模板直接使用。
3. 不要重新生成背景，不要从零自由生成整页背景。
4. 所有页面都应在该背景模板之上叠加内容。
5. 背景图铺满整页，不得裁切、拉伸变形或遮挡模板现有元素。
6. 页面内容应避开右上角 Logo 区域。
7. 页面主体内容优先放在左侧、中部或下方留白区域。
8. 内容较多时，使用白色半透明圆角卡片承载。

## 锁定模板元素

右上角 GeekDance Logo 是锁定区域，必须保持模板原样：

1. 不允许移动。
2. 不允许缩放。
3. 不允许改色。
4. 不允许重绘。
5. 不允许替换。
6. 不允许加特效。
7. 不要生成新的英文 GeekDance logo。
8. 不要把原 Logo 替换成新 Logo。

顶部浅色 GeekDance 大字水印也是模板固定元素，必须保持原样，不要重新设计、重绘、移动、替换或加特效。

公司风格页面生成逻辑：页面是在固定模板上排版，不是自由生成整页。先使用模板作为页面底板，再把标题、正文、图表、卡片、图标和项目视觉元素叠加到模板留白区域。

## 整体视觉

- 高级、干净、专业、商务、科技感强。
- 白色、浅灰白、淡粉白作为主视觉底色。
- 红色作为品牌点缀色，不大面积滥用。
- 顶部保留超大浅色 GeekDance 品牌水印。
- 右上角保留 GeekDance Logo 的清晰识别。
- 右上角 Logo 和顶部水印来自固定模板，不可编辑、不可重绘、不可替换。
- 页面要有留白感，不要信息堆满。

## 配色

- 主色：白色 / 浅灰白 / 淡粉白
- 点缀色：GeekDance 品牌红
- 辅助色：浅红 / 淡粉 / 灰黑
- 正文色：深灰 / 黑色
- 强调方式：关键词、数字、标签、图标、短横线使用红色

## 版式语言

推荐使用：

- 大标题左上或居中偏上
- 标题下方短红线强调
- 圆角白色卡片
- 轻阴影
- 浅红描边
- 模块矩阵
- 流程图
- 时间轴
- 环形图
- 漏斗图
- 架构图
- 大数字数据卡
- 客户价值卡片
- 分割页大数字 + PART 标签

避免使用：

- 蓝色运维大屏风
- 过强赛博朋克风
- 密集表格风
- 普通办公模板风
- 花哨卡通风
- 过多渐变堆叠
- 文字堆满页面

## 分页类型设计建议

### 封面页

- 使用大标题 + 项目副标题 + 汇报单位 + 日期。
- 背景使用固定 GeekDance 通用模板背景。
- 可以加入项目相关视觉元素，但不要遮挡右上角 Logo。

### 目录 / 分割页

- 可使用红色渐变蒙版。
- 大数字编号，例如 01 / 02 / 03。
- 使用 PART ONE / PART TWO 标签。
- 文字简洁，适合业务章节切换。

### 项目背景页

- 左侧写痛点或背景说明。
- 右侧用数据卡、趋势图或场景图表达。
- 红色突出关键痛点和业务机会。

### 功能架构页

- 适合使用模块矩阵、中心圆扩散、分层架构、流程闭环。
- 每个模块不超过 2 行描述。
- 技术术语要转化成客户能理解的业务价值。

### 方案价值页

- 推荐使用 3～5 个价值卡片。
- 每个卡片包括：价值标题、简短描述、业务收益。
- 强调降本、增效、体验提升、管理可视化、数据沉淀、持续运营。

### 技术能力页

- 不堆技术栈清单。
- 用能力模型表达：数据能力、系统能力、AI 能力、交付能力、运维能力。
- 技术名词可以小字出现，主体表达要面向客户。

### 服务流程页

- 推荐使用横向时间轴或 4～6 步流程图。
- 突出调研、方案、设计、开发、测试、上线、运维。

### 报价 / 周期页

- 信息必须谨慎。
- 金额、日期、工期必须提醒用户人工复核。
- 不得擅自承诺未确认的内容。

## 文字风格

- 标题简洁、有力、商务化。
- 正文使用短句。
- 少用“我们会做很多功能”这种空话。
- 多用“帮助客户实现什么业务价值”。
- 技术细节转成客户语言。

示例：

```text
不好：使用 RAG、Agent、向量库、微服务架构实现系统升级。
更好：通过企业知识库与智能任务执行能力，让员工能够更快查询资料、处理流程、沉淀经验。
```

## 生图 Prompt 固定附加要求

当生成公司风格页面 Prompt 或预览图时，必须附加：

```text
16:9 horizontal business proposal PPT page, use assets/geekdance-default-background.jpg as the fixed master template background, compose content on top of the template rather than generating the full page from scratch, preserve the existing top-right GeekDance logo exactly, logo is locked and non-editable, do not move scale recolor redraw replace or add effects to the logo, do not generate a new English GeekDance logo, preserve the large pale GeekDance watermark exactly as in the template, white and pale gray clean corporate technology style, red accent color, rounded white cards, soft shadow, light red outlines, clean typography hierarchy, premium consulting deck layout, suitable for client-facing business proposal, no blue dashboard style, no generic template look, no copied content from references.
```
