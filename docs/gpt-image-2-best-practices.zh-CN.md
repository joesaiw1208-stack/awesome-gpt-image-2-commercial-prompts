# GPT-Image-2 提示词最佳实践

本仓库的提示词写法，已按 **2026 年 4 月 23 日** 可获取到的 OpenAI 官方图像文档进行校准。

## 官方来源

- [OpenAI Image generation guide](https://developers.openai.com/api/docs/guides/image-generation)
- [OpenAI GPT Image Generation Models Prompting Guide](https://developers.openai.com/cookbook/examples/multimodal/image-gen-models-prompting-guide)

## 本仓库采用的标准

本仓库使用的提示词模板，是基于官方文档与 cookbook 示例归纳出的工程化写法，并不是 OpenAI 强制要求的唯一格式。

我们统一采用以下顺序：

1. 目标或用途
2. 资产类型
3. 场景
4. 主体
5. 构图
6. 光线
7. 材质与风格
8. 约束条件

## 为什么这样写更符合官方建议

- OpenAI 建议使用一致的提示词顺序，并写明 intended use，这样模型更容易理解输出的完成度与应用场景。来源：prompting guide。
- OpenAI 说明最重要的不是花哨语法，而是清晰的意图与约束；对生产系统来说，可快速浏览的结构化格式更合适。来源：prompting guide。
- OpenAI 建议当图片中需要真实文案时，把文字精确写出来，并补充字体、位置、对比度等约束。来源：prompting guide。
- OpenAI 建议在编辑工作流里做小步修改，并反复重申哪些内容不能变，以减少漂移。来源：prompting guide。
- OpenAI 文档说明 `gpt-image-2` 对输入图默认就是高保真处理，因此本仓库不再围绕 `input_fidelity` 做模板设计。来源：image-generation guide。
- OpenAI 文档说明 `gpt-image-2` 暂不支持透明背景，因此本仓库不会把透明背景当成默认能力。来源：image-generation guide。
- OpenAI 文档列出了 `1024x1024`、`1536x1024`、`1024x1536` 等常用尺寸，并指出正方形通常生成更快。来源：image-generation guide。
- OpenAI 同时提醒：虽然文字渲染和版式控制明显提升，但对精确排版仍不应过度乐观，因此文字密集场景仍需更严格的提示和反复迭代。来源：image-generation guide。

## 本仓库的额外规则

- 除非必须展示文字，否则优先使用无品牌、无可读文字包装。
- 提示词强调商业生产，不追求空泛文学化表达。
- 电商场景必须写清楚用途，例如 PDP hero、marketplace 主图、投放素材、上新海报等。
- 用明确的负向约束抑制杂物、重复产品、漂浮手部、乱码标签和水印式伪影。
- 如果一定要在图中出现真实文案，必须使用精确引号文本并补充排版约束。
