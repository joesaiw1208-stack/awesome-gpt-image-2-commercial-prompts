# GPT-Image-2 Prompting Best Practices

This repository standard is aligned with OpenAI's current image-generation guidance as of April 23, 2026.

## Official Sources

- [OpenAI Image generation guide](https://developers.openai.com/api/docs/guides/image-generation)
- [OpenAI GPT Image Generation Models Prompting Guide](https://developers.openai.com/cookbook/examples/multimodal/image-gen-models-prompting-guide)

## What We Standardized

The prompt template used in this repo is an inference from the official docs and cookbook examples, not a literal OpenAI-required schema.

We standardize on:

1. Goal or intended use
2. Asset type
3. Scene
4. Subject
5. Composition
6. Lighting
7. Materials and styling
8. Constraints

## Why This Matches The Docs

- OpenAI recommends writing prompts in a consistent order and including intended use so the model knows the polish level and mode. Source: prompting guide.
- OpenAI notes that minimal, paragraph, JSON-like, and instruction-style prompts can all work, but production systems should prefer a skimmable format with clear intent and constraints. Source: prompting guide.
- OpenAI recommends putting exact in-image text in quotes and specifying placement and typography constraints. Source: prompting guide.
- OpenAI recommends small iterative edits and restating invariants during edits to reduce drift. Source: prompting guide.
- OpenAI documents that `gpt-image-2` always processes image inputs at high fidelity, so we do not rely on `input_fidelity` controls in this repo's guidance. Source: image-generation guide.
- OpenAI documents that `gpt-image-2` does not support transparent backgrounds. Source: image-generation guide.
- OpenAI documents that square images are usually fastest, and highlights `1024x1024`, `1536x1024`, and `1024x1536` as strong defaults. Source: image-generation guide.
- OpenAI notes that text rendering and precise layout control are improved but still imperfect, so text-heavy assets need stricter prompts and careful iteration. Source: image-generation guide.

## Repo Rules

- Use blank or unlabeled packaging unless text is essential.
- Keep prompts production-oriented, not poetic.
- For e-commerce, always specify the commercial context: PDP hero, marketplace packshot, paid social, collection launch, and so on.
- Use explicit negative constraints to suppress clutter, duplicate products, stray hands, unreadable labels, and watermark-like artifacts.
- If the asset needs real copy, quote it exactly and add placement constraints.
