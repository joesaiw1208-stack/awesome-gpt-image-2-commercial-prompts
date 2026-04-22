# Contributing

Thanks for helping improve this repository.

## What We Accept

- new commercial prompt templates for GPT-Image-2
- stronger versions of existing prompts
- category expansions with real commercial value
- example outputs generated from prompts in this repo
- metadata improvements in `data/prompts.json`
- documentation improvements

## What We Do Not Accept

- generic art prompts with no commercial use case
- prompts copied without meaningful adaptation or attribution context
- prompts with unclear output goals
- prompts that depend on private brand assets without permission
- prompts that imitate a living brand too literally instead of abstracting the visual language

## Prompt Submission Standard

Each prompt file should include:

- title
- best-for scenarios
- English prompt
- Chinese prompt
- why it works

## Prompt Format

We align the repo with [docs/gpt-image-2-best-practices.md](./docs/gpt-image-2-best-practices.md).

Preferred field order:

- goal
- asset
- scene
- subject
- composition
- lighting
- materials and styling
- constraints

## Naming

Use lowercase kebab-case filenames, for example:

`luxury-skincare-hero.md`

## Images

If you contribute example outputs:

- place them in `assets/examples/`
- use descriptive filenames
- ensure the image can be shared publicly
- ensure the image actually matches the prompt title and category

## Pull Requests

Keep PRs focused. One category, one prompt family, or one documentation improvement per PR is ideal.
