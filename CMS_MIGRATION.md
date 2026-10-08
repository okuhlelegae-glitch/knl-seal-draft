# CMS Migration

## Recommendation: Sanity

Reasons:
- Structured content, great for pages/products/partners/stories/faqs
- Portable JSON schema, easy to swap
- Clean GROQ queries

## Proposed Schema
- page (title, slug, blocks)
- product (name, slug, priceZAR, variants, description)
- partner (name, logo, tier)
- story (name, quote, image)
- keyholder (name, cohort, bio)
- faq (question, answer, category)

## Notes
- Keep all copy in /content as typed files now for zero coupling.
- When migrating, replace content loaders with Sanity client without rewriting UI components.

