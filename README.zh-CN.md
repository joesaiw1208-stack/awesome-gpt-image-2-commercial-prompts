# Awesome GPT-Image-2 E-Commerce Prompts

[English](./README.md) | 简体中文

[![License: MIT](https://img.shields.io/badge/License-MIT-black.svg)](./LICENSE)
[![Contributions Welcome](https://img.shields.io/badge/contributions-welcome-brightgreen.svg)](./CONTRIBUTING.md)
[![Prompt Count](https://img.shields.io/badge/prompts-12-blue.svg)](./prompts)
[![Category Focus](https://img.shields.io/badge/focus-e--commerce-orange.svg)](./prompts)

一个面向 **GPT-Image-2** 的专业开源提示词库，专注于 **电商增长**、**产品叙事** 与 **高转化视觉生产**。

目前 GitHub 上很多 GPT-Image-2 项目更像“灵感展示馆”，而不是“可直接用于商业生产的提示词系统”。这个项目的目标，就是把 GPT-Image-2 在电商场景中的价值做成一套真正能复用、能协作、能持续扩展的开源资产。

## 为什么做这个项目

现有公开仓库里，已经有不少通用型 GPT-Image-2 提示词合集，但在以下场景里仍然缺少一个结构清晰、定位鲜明、足够专业的开源仓库：

- 产品主视觉
- 电商 packshot
- 服饰上身图
- 美妆护肤广告图
- 食品饮料上新图
- 节日营销横幅
- 对比创意图
- PDP 与 A+ 内容视觉

这个仓库的差异化方向非常明确：**不是收集泛艺术提示词，而是沉淀电商可落地的商业提示词模板**。

## 差异化亮点

- 电商专用：围绕目录图、活动图、广告图、PDP、社媒投放等真实场景设计
- 结构化提示词：每个 prompt 都包含用途、构图、光线、约束条件和变体建议
- 可复用系统：适合品牌团队、设计师、增长团队快速改写和批量产出
- 配套示例图：核心 prompt 附带生成效果图，降低理解成本
- 真正开源：支持社区贡献、迭代和扩展更多垂直品类

## 调研结论

截至 **2026 年 4 月 23 日**，GitHub 上较有代表性的 GPT-Image-2 相关仓库主要还是偏“通用灵感库”路线：

- [ZeroLu/awesome-gpt-image](https://github.com/ZeroLu/awesome-gpt-image) 以社区案例为主，覆盖摄影、游戏、UI、文字、编辑等多个方向。
- [EvoLinkAI/awesome-gpt-image-2-prompts](https://github.com/EvoLinkAI/awesome-gpt-image-2-prompts) 以通用 prompt 展示为主，覆盖人物、海报、UI mockup 等内容。

机会点很明显：**还没有一个公开仓库，把 GPT-Image-2 的电商商业化提示词做成“专业、系统、可 star、可扩展”的标杆项目。**

## 仓库结构

```text
assets/
  examples/               本仓库提示词生成的示例图片
data/
  prompts.json            结构化提示词元数据，方便检索和工具化
prompts/
  beauty/
  fashion/
  food-beverage/
  home-living/
  jewelry/
  seasonal-campaigns/
```

## Prompt 设计标准

本仓库中的每条 prompt 都尽量遵循统一结构：

1. Use case
2. Asset type
3. Primary request
4. Scene and backdrop
5. Subject and styling
6. Composition and framing
7. Lighting and mood
8. Text constraints
9. Commercial constraints
10. Adaptation tips

这样做的好处是：更容易复用、更适合协作，也更方便后续扩展成搜索库、生成器或网站。

## 精选 Prompt

### 1. Luxury Skincare Hero

文件: [prompts/beauty/luxury-skincare-hero.md](./prompts/beauty/luxury-skincare-hero.md)

适合高端精华、护肤新品发布页、投放素材和首页视觉。

![Luxury Skincare Hero](./assets/examples/luxury-skincare-hero.png)

### 2. Clean Supplement Packshot

文件: [prompts/food-beverage/clean-supplement-packshot.md](./prompts/food-beverage/clean-supplement-packshot.md)

适合保健品、营养品、DTC 健康品牌的电商主图与 marketplace 视觉。

![Clean Supplement Packshot](./assets/examples/clean-supplement-packshot.png)

### 3. Luxury Jewelry Campaign Visual

文件: [prompts/jewelry/luxury-jewelry-campaign.md](./prompts/jewelry/luxury-jewelry-campaign.md)

适合珠宝新品发布、首页 hero、社媒广告与高端品牌视觉。

![Luxury Jewelry Campaign](./assets/examples/luxury-jewelry-campaign.png)

### 4. Summer Beverage Launch Banner

文件: [prompts/seasonal-campaigns/summer-beverage-launch-banner.md](./prompts/seasonal-campaigns/summer-beverage-launch-banner.md)

适合夏季饮品上新、活动页横幅和季节性增长 campaign。

![Summer Beverage Launch Banner](./assets/examples/summer-beverage-launch-banner.png)

## 分类目录

- [Beauty](./prompts/beauty)
- [Fashion](./prompts/fashion)
- [Food & Beverage](./prompts/food-beverage)
- [Home & Living](./prompts/home-living)
- [Jewelry](./prompts/jewelry)
- [Seasonal Campaigns](./prompts/seasonal-campaigns)

## 完整 Prompt 库

- Beauty: [Luxury Skincare Hero](./prompts/beauty/luxury-skincare-hero.md), [Clinical Beauty Dropper Detail](./prompts/beauty/clinical-beauty-dropper-detail.md)
- Fashion: [Editorial Fashion Flatlay](./prompts/fashion/editorial-fashion-flatlay.md), [Streetwear On-Model Launch](./prompts/fashion/streetwear-on-model-launch.md)
- Food & Beverage: [Clean Supplement Packshot](./prompts/food-beverage/clean-supplement-packshot.md), [Organic Coffee Lifestyle Pour](./prompts/food-beverage/organic-coffee-lifestyle-pour.md)
- Home & Living: [Scandinavian Chair Lifestyle](./prompts/home-living/scandinavian-chair-lifestyle.md), [Minimal Bedding Hero](./prompts/home-living/minimal-bedding-hero.md)
- Jewelry: [Luxury Jewelry Campaign](./prompts/jewelry/luxury-jewelry-campaign.md), [Bridal Ring Macro Detail](./prompts/jewelry/bridal-ring-macro-detail.md)
- Seasonal Campaigns: [Summer Beverage Launch Banner](./prompts/seasonal-campaigns/summer-beverage-launch-banner.md), [Holiday Gift Box Hero](./prompts/seasonal-campaigns/holiday-gift-box-hero.md)

## 适合谁使用

- AI 原生品牌创业者
- 电商增长团队
- 需要快速出图的设计师
- 平台与 marketplace 团队
- 提示词工程师
- 创意代理商与内容团队

## 使用方式

1. 选择一个品类和 prompt 模板。
2. 替换产品、品牌、颜色和 campaign 细节。
3. 尽量保留商业约束条件，除非你明确想要更自由的输出。
4. 生成多组变体，对比清晰度、转化意图和品牌适配度。
5. 把效果好的 prompt 重新贡献回仓库。

## 贡献原则

我们更欢迎这些内容：

- 真的适合商业使用
- 有足够明确的视觉指向
- 适合复用，不依赖私有素材
- 约束条件清晰
- 既有惊艳感，也不臃肿

提交 PR 前请先阅读 [CONTRIBUTING.md](./CONTRIBUTING.md)。

## 关于 Star 增长

如果你希望这个项目更容易获得 star，关键不是“多放一些 prompt”，而是持续维持下面这几个特点：

- 方向足够垂直
- 结构足够专业
- 示例图足够惊艳
- README 足够清楚
- 社区贡献门槛足够低

这个版本已经具备一个不错的公开首发基础。

## 开源协议

MIT，详见 [LICENSE](./LICENSE)。

## 声明

本仓库由社区维护，与 OpenAI 无官方隶属关系。不同模型版本、界面和工作流下，prompt 的效果可能会有所差异。
