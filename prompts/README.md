# Prompt Library Structure

The `prompts/` directory is organized by **industry first**, because that is usually how commercial teams search for reusable visual systems.

## Current Categories

- `automotive/`
- `beauty/`
- `commercial-formats/`
- `consumer-tech/`
- `fashion/`
- `food-beverage/`
- `fragrance/`
- `home-living/`
- `hospitality/`
- `jewelry/`
- `seasonal-campaigns/`
- `spirits/`
- `watches/`

## Why Industry-First

Many prompt repos are organized only by abstract prompt patterns. That is good for experimentation, but weaker for commercial production.

This repo keeps:

- industry-specific language close to the prompt
- material references close to the business context
- campaign examples grouped in ways that brand and ecommerce teams naturally browse

## Supporting Navigation

To avoid making `prompts/` too deep, cross-cutting navigation lives in `docs/`:

- [Browse by Industry](../docs/by-industry.md)
- [Browse by Use Case](../docs/by-use-case.md)
- [Browse by Format](../docs/by-format.md)
