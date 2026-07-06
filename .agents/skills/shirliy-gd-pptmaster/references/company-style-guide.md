# GeekDance Official Business Style

## 风格名称

**GeekDance Official Business Style**  
中文：**极客跳动官方商务科技风**

当用户选择「采用公司风格」时，必须默认使用本风格。

## 默认背景

默认背景文件：

```text
assets/geekdance-default-background.jpg
```

使用规则：

1. 页面比例固定为 **16:9 横版**。
2. 背景图铺满整页。
3. 不得裁切或遮挡右上角 GeekDance Logo。
4. 保留顶部浅色 GeekDance 大水印作为品牌识别。
5. 页面内容应避开右上角 Logo 区域。
6. 页面主体内容优先放在左侧、中部或下方留白区域。
7. 内容较多时，使用白色半透明圆角卡片承载。

## 整体视觉

- 高级、干净、专业、商务、科技感强。
- 白色、浅灰白、淡粉白作为主视觉底色。
- 红色作为品牌点缀色，不大面积滥用。
- 顶部保留超大浅色 GeekDance 品牌水印。
- 右上角保留 GeekDance Logo 的清晰识别。
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
- 背景使用 GeekDance 通用背景。
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

当生成公司风格页面 Prompt 时，必须附加：

```text
16:9 horizontal business proposal PPT page, use GeekDance default background, white and pale gray clean corporate technology style, large subtle GeekDance watermark feel, clear top-right GeekDance logo area, red accent color, rounded white cards, soft shadow, light red outlines, clean typography hierarchy, premium consulting deck layout, suitable for client-facing business proposal, no blue dashboard style, no generic template look, no copied content from references.
```
