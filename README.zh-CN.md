# Awesome GPT-Image-2 E-Commerce Prompts

[English](./README.md) | 简体中文

[![License: MIT](https://img.shields.io/badge/License-MIT-black.svg)](./LICENSE)
[![Prompts](https://img.shields.io/badge/prompts-16-blue.svg)](./prompts)
[![Featured Gallery](https://img.shields.io/badge/featured-6-gold.svg)](./README.zh-CN.md#精选案例画廊)
[![Languages](https://img.shields.io/badge/prompt_languages-EN%20%7C%20ZH-green.svg)](./README.md)

这是一个面向 **GPT-Image-2** 的双语 Prompt Gallery，专门服务于 **电商视觉**、**零售产品叙事** 和 **更接近转化目标的商业出图**。

## 这个版本修了什么

这次重构的重点不是“再堆更多提示词”，而是把仓库修成更专业的开源产品：

- 按 OpenAI 官方图像文档重新校准 prompt 写法
- 所有新增与重写的核心案例都提供英文版和中文版
- README 直接展示图片和 prompt，不再强依赖跳转
- 新案例优先补电商真正高频的实用场景

## 已按 OpenAI 官方建议校准

本仓库的 prompt 结构，参考了当前 OpenAI 图像文档与 cookbook 示例：

- 统一顺序：`goal -> asset -> scene -> subject -> composition -> lighting -> materials -> constraints`
- 强制写清 intended use，让模型知道这是 marketplace 图、PDP 图还是 campaign 图
- 优先使用具体材质、镜头意图与负向约束，而不是空泛形容词
- 除非必须，不在图里要求真实文字
- 编辑类工作流中，把“改什么”和“哪些不能变”分开写

来源：

- [OpenAI Image generation guide](https://developers.openai.com/api/docs/guides/image-generation)
- [OpenAI GPT Image Generation Models Prompting Guide](https://developers.openai.com/cookbook/examples/multimodal/image-gen-models-prompting-guide)
- 仓库整理版说明：[docs/gpt-image-2-best-practices.zh-CN.md](./docs/gpt-image-2-best-practices.zh-CN.md)

说明：本仓库使用的模板是基于官方建议提炼出的工程化写法，不是 OpenAI 唯一允许的固定格式。

## 精选案例画廊

### 1. Marketplace Bundle Packshot

适用场景：Amazon 组合装主图、Shopify 套装 PDP、平台促销组合图  
完整文件：[prompts/food-beverage/marketplace-bundle-packshot.md](./prompts/food-beverage/marketplace-bundle-packshot.md)

![Marketplace Bundle Packshot](./assets/examples/marketplace-bundle-packshot.png)

**Prompt (EN)**

```text
Goal: Create a clean marketplace bundle image that is immediately understandable at a glance.
Asset: Bundle packshot for e-commerce and marketplaces.
Scene: Pure white seamless background with subtle grounding shadows.
Subject: One hero product plus two clearly related accessories or refill units arranged in a tidy bundle layout.
Composition: Front-facing arrangement, all items fully visible, spacing clean, hierarchy obvious, no overlap that hides key shapes.
Lighting: Bright commercial studio light with crisp edges and soft natural shadow.
Materials and styling: Modern packaging, neutral retail-safe color palette, practical catalog look.
Constraints: No people, no props, no decoration, no logo, no readable text, no floating items, no clutter, no watermark.
```

**提示词（中文）**

```text
目标：生成一张一眼就能看懂的电商组合装产品图。
资产类型：用于电商平台和 marketplace 的 bundle packshot。
场景：纯白无缝背景，带轻微落影。
主体：一个主产品加两个明确相关的配件或补充装，整齐组合陈列。
构图：正面摆放，所有物品完整可见，间距干净，主次清楚，不要遮挡关键轮廓。
光线：明亮商业棚拍光，边缘清晰，阴影柔和自然。
材质与风格：现代包装，中性安全的零售色彩，偏目录图的实用风格。
约束：不要人物，不要道具，不要装饰，不要 logo，不要可读文字，不要悬浮摆放，不要杂乱，不要水印。
```

### 2. Luxury Skincare Hero

适用场景：首页主视觉、PDP 顶部横幅、高端护肤投放图  
完整文件：[prompts/beauty/luxury-skincare-hero.md](./prompts/beauty/luxury-skincare-hero.md)

![Luxury Skincare Hero](./assets/examples/luxury-skincare-hero.png)

**Prompt (EN)**

```text
Goal: Create a premium skincare hero image that feels expensive, clean, and conversion-ready.
Asset: E-commerce hero banner for a facial serum launch.
Scene: Warm ivory studio set with a round travertine pedestal, shallow water ripples, and soft botanical shadows.
Subject: One frosted glass serum bottle with a brushed champagne cap and a blank label area.
Composition: Centered product, slightly low camera angle, full bottle clearly visible, generous negative space for headline overlay.
Lighting: Soft diffused studio light with luminous highlights and calm luxury mood.
Materials and styling: Frosted glass, brushed metal, polished stone, subtle water shimmer, restrained neutral palette.
Constraints: No logo, no readable text, no hands, no extra props, no duplicate products, no clutter, no deformation, no watermark.
```

**提示词（中文）**

```text
目标：生成一张高端护肤品主视觉，画面要昂贵、干净，并且适合电商转化。
资产类型：面部精华新品的电商 hero 横幅。
场景：温暖象牙色摄影棚场景，圆形洞石底座，浅浅水波反射，带有柔和植物投影。
主体：一只磨砂玻璃精华瓶，搭配香槟金拉丝瓶盖，标签区域保持空白。
构图：产品居中，略微低机位，整瓶完整可见，预留足够文案留白。
光线：柔和漫射棚拍光，带通透高光，整体情绪安静、洁净、奢华。
材质与风格：磨砂玻璃、拉丝金属、抛光石材、轻微水面反光，色调克制。
约束：不要 logo，不要可读文字，不要手，不要多余道具，不要重复产品，不要杂乱，不要变形，不要水印。
```

### 3. Streetwear On-Model Launch

适用场景：新品 drop 主图、4:5 投放素材、首页 campaign 卡片  
完整文件：[prompts/fashion/streetwear-on-model-launch.md](./prompts/fashion/streetwear-on-model-launch.md)

![Streetwear On-Model Launch](./assets/examples/streetwear-on-model-launch.png)

**Prompt (EN)**

```text
Goal: Create a premium on-model streetwear launch image that feels aspirational but still product-readable.
Asset: Campaign static for a new collection drop.
Scene: Clean urban architecture with concrete, brushed steel, and minimal background distraction.
Subject: One confident model wearing a complete streetwear outfit, clearly showing the jacket, pants, and footwear.
Composition: Mid-to-full-length framing, strong silhouette, relaxed campaign pose, negative space for copy.
Lighting: Natural daylight with polished editorial contrast, cool and sharp but believable.
Materials and styling: Cotton fleece, nylon, denim, technical fabric, muted charcoal and concrete tones with one accent color.
Constraints: No logo, no text, no crowd, no street clutter, no distorted hands, no distorted body proportions, no watermark.
```

**提示词（中文）**

```text
目标：生成一张高级街头服饰上身图，既有品牌调性，也能清楚展示产品。
资产类型：新品 drop 的 campaign 静态图。
场景：干净的城市建筑背景，包含混凝土和拉丝金属元素，但不喧宾夺主。
主体：一位自信模特，穿完整街头造型，外套、裤装和鞋款都要清楚可见。
构图：中长到全身构图，轮廓清晰，姿态自然，有文案留白。
光线：自然日光配合克制的编辑感对比，整体清爽、真实、有质感。
材质与风格：棉卫衣、尼龙、丹宁、机能面料，色彩以炭灰和水泥灰为主，辅以一个强调色。
约束：不要 logo，不要文字，不要人群，不要街景杂乱，不要手部畸形，不要身体比例错误，不要水印。
```

### 4. Footwear Floating Hero

适用场景：鞋履 PDP 主图、投放 launch 图、系列落地页横幅  
完整文件：[prompts/fashion/footwear-floating-hero.md](./prompts/fashion/footwear-floating-hero.md)

![Footwear Floating Hero](./assets/examples/footwear-floating-hero.png)

**Prompt (EN)**

```text
Goal: Create a premium footwear hero image that makes the product feel light, technical, and launch-ready.
Asset: Sneaker campaign visual for e-commerce.
Scene: Clean seamless gray studio gradient with subtle depth and restrained motion energy.
Subject: One modern sneaker floating in midair, showing upper material, side profile, and outsole shape clearly.
Composition: Three-quarter hero angle, product large in frame, strong negative space, crisp silhouette, no crop.
Lighting: Controlled studio lighting with sharp edge highlights and realistic grounding shadow.
Materials and styling: Mesh, suede, rubber outsole, subtle performance texture, premium sport-fashion finish.
Constraints: No logo, no readable text, no extra shoes, no feet, no laces flying wildly, no clutter, no watermark.
```

**提示词（中文）**

```text
目标：生成一张高级鞋履主视觉，让产品看起来轻盈、专业、适合新品发布。
资产类型：用于电商的运动鞋 campaign 视觉。
场景：干净的灰色无缝棚拍渐变背景，带轻微空间层次和克制的动态感。
主体：一只现代运动鞋悬浮在半空，鞋面材质、侧面轮廓和鞋底形态都要清楚。
构图：三分之四英雄角度，产品在画面中占比大，留白强，轮廓锐利，整只鞋不要被裁切。
光线：受控棚拍光，边缘高光明确，同时有真实落影。
材质与风格：网布、麂皮、橡胶大底、细腻性能纹理，兼具运动感和高端感。
约束：不要 logo，不要可读文字，不要第二只鞋，不要脚，不要夸张飞散鞋带，不要杂乱，不要水印。
```

### 5. Luxury Jewelry Campaign

适用场景：珠宝发布 campaign、首页 hero、社媒高端广告  
完整文件：[prompts/jewelry/luxury-jewelry-campaign.md](./prompts/jewelry/luxury-jewelry-campaign.md)

![Luxury Jewelry Campaign](./assets/examples/luxury-jewelry-campaign.png)

**Prompt (EN)**

```text
Goal: Create a luxury jewelry campaign image with clear craftsmanship and believable premium sparkle.
Asset: Homepage hero or social campaign for fine jewelry.
Scene: Deep charcoal-to-black luxury backdrop with a glossy black pedestal and restrained reflective surfaces.
Subject: One diamond necklace arranged elegantly as the hero piece.
Composition: Close-to-medium crop, full focal section of the necklace clearly visible, upscale magazine-ad balance, controlled negative space.
Lighting: Dramatic but controlled spotlighting with crisp gemstone highlights and soft shadow falloff.
Materials and styling: Polished precious metal, refined stone facets, black lacquer surface, intimate editorial mood.
Constraints: No model, no hands, no text, no logo, no exaggerated sparkle effects, no clutter, no cheap costume-jewelry look, no watermark.
```

**提示词（中文）**

```text
目标：生成一张高级珠宝 campaign 图，既要体现工艺，又要让珠宝闪耀真实可信。
资产类型：用于首页 hero 或社媒投放的高级珠宝主视觉。
场景：深炭黑到黑色的奢华背景，搭配高光黑色底座和克制的反射面。
主体：一条钻石项链作为唯一主角，摆放优雅。
构图：近景到中近景构图，项链核心部分必须清晰可见，整体像高级杂志广告。
光线：戏剧化但可控的聚光，钻石高光锐利，阴影柔和下沉。
材质与风格：抛光贵金属、精细切割宝石、黑色漆面反射、亲密而高端的编辑感。
约束：不要模特，不要手，不要文字，不要 logo，不要夸张星芒特效，不要杂乱，不要廉价饰品感，不要水印。
```

### 6. Kitchen Appliance Countertop Demo

适用场景：小家电 PDP 辅助图、上新 campaign、家居投放图  
完整文件：[prompts/home-living/kitchen-appliance-countertop-demo.md](./prompts/home-living/kitchen-appliance-countertop-demo.md)

![Kitchen Appliance Countertop Demo](./assets/examples/kitchen-appliance-countertop-demo.png)

**Prompt (EN)**

```text
Goal: Create a premium lifestyle image for a countertop kitchen appliance that looks useful, modern, and giftable.
Asset: PDP secondary visual for a compact espresso machine.
Scene: Clean contemporary kitchen counter with stone backsplash, subtle morning light, and restrained supporting props.
Subject: One compact espresso machine as the hero product with a single cup nearby.
Composition: Three-quarter countertop view, appliance clearly dominant, enough surrounding context to feel lived-in but uncluttered.
Lighting: Soft natural morning light with crisp metallic highlights and believable shadow.
Materials and styling: Brushed metal, matte black details, ceramic cup, stone counter, minimal premium styling.
Constraints: No people, no text, no logo, no clutter, no extra appliances, no unrealistic steam, no watermark.
```

**提示词（中文）**

```text
目标：生成一张高端厨房小家电生活方式图，让产品显得实用、现代、适合送礼。
资产类型：紧凑型咖啡机的 PDP 辅助场景图。
场景：干净的现代厨房台面，石材挡板，柔和晨光，少量辅助道具。
主体：一台紧凑型咖啡机作为主产品，旁边只有一只咖啡杯。
构图：三分之四角度的台面视角，家电必须是绝对主角，环境提供生活感但不能杂乱。
光线：柔和自然晨光，金属高光清晰，阴影真实。
材质与风格：拉丝金属、哑光黑色细节、陶瓷杯、石材台面，整体极简高级。
约束：不要人物，不要文字，不要 logo，不要杂乱，不要额外家电，不要不真实的蒸汽，不要水印。
```

## 更多双语案例

- Beauty: [Clinical Beauty Dropper Detail](./prompts/beauty/clinical-beauty-dropper-detail.md)
- Fashion: [Editorial Fashion Flatlay](./prompts/fashion/editorial-fashion-flatlay.md), [Luxury Handbag Shelf Hero](./prompts/fashion/luxury-handbag-shelf-hero.md)
- Food & Beverage: [Clean Supplement Packshot](./prompts/food-beverage/clean-supplement-packshot.md), [Organic Coffee Lifestyle Pour](./prompts/food-beverage/organic-coffee-lifestyle-pour.md)
- Home & Living: [Minimal Bedding Hero](./prompts/home-living/minimal-bedding-hero.md), [Scandinavian Chair Lifestyle](./prompts/home-living/scandinavian-chair-lifestyle.md)
- Jewelry: [Bridal Ring Macro Detail](./prompts/jewelry/bridal-ring-macro-detail.md)
- Seasonal: [Summer Beverage Launch Banner](./prompts/seasonal-campaigns/summer-beverage-launch-banner.md), [Holiday Gift Box Hero](./prompts/seasonal-campaigns/holiday-gift-box-hero.md)

## 仓库结构

```text
assets/examples/          示例图片
docs/                    提示词最佳实践说明
data/prompts.json        Prompt 元数据
prompts/                 双语 prompt 文件
```

## 贡献标准

我们更欢迎这些 prompt：

- 对真实电商工作流有用
- 复现性强，不是纯灵感句子
- 同时提供英文和中文版本
- 约束条件明确
- 视觉强但不沦为泛化 AI 图

提交前请先阅读 [CONTRIBUTING.md](./CONTRIBUTING.md)。
