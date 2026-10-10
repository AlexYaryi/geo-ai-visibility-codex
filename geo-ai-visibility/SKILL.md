---
name: geo-ai-visibility
description: Audit and improve a website for Generative Engine Optimization (GEO), AI search visibility, citations in ChatGPT, Gemini, Perplexity and AI Overviews, alongside technical SEO and local SEO. Use when asked to optimize a website for AI answers, LLM discovery, structured data, topical authority, or GEO.
---

# GEO / AI Search Visibility — execution skill

## Mission
Make the website technically accessible, genuinely useful, credible, citable, and commercially effective for people arriving from search engines and AI answer systems. Do not promise rankings, mentions, or citations. Distinguish verified findings from hypotheses.

## Start with evidence
1. Inspect the repository, framework, routes, rendering strategy, sitemap, robots.txt, canonical tags, hreflang, structured data, content templates, analytics and deployment configuration.
2. If network access is available, test live pages and HTTP status codes, rendered HTML, robots directives and public search appearance. If not, explicitly mark live checks as pending.
3. Ask for target markets, languages, commercial priorities and analytics access only if missing and necessary. Otherwise infer provisional targets from repository content and label assumptions.
4. Capture baseline in `reports/geo-baseline.md` with date, checked URLs, evidence and limitations.

## Technical accessibility
- Validate robots.txt syntax and sitemap references; do not blindly allow all bots. Distinguish AI search crawlers from training crawlers; respect owner preferences and platform policies.
- Verify indexable pages return HTTP 200, have stable canonical URLs, no accidental noindex, and meaningful server-rendered or prerendered HTML where necessary.
- Check mobile usability, performance, internal linking, URL architecture, duplicate content, broken links, language targeting, hreflang reciprocity and localized metadata.
- Verify content visibility without authentication or essential JavaScript interactions. Check CDN/WAF restrictions and bot-specific responses when permitted.
- Treat `llms.txt` as optional and experimental; never present it as a guaranteed ranking factor.

## Answer-ready content
- Map intent clusters: informational, comparison, transactional, local, trust and after-sale questions.
- Prioritize pages that answer a specific user question directly in the first useful paragraph, followed by evidence, examples, limitations and next steps.
- Use descriptive headings, short accurate answer sections, clear tables when relevant, useful FAQs, original first-party details, updated dates, and transparent commercial terms.
- Never invent reviews, ratings, availability, prices, policies, customer experiences, statistics, awards or citations. Source all externally derived claims and note update dates.
- Avoid mass-producing near-duplicate city, language or keyword pages. Translate and localize meaningfully.
- Build relevant internal links from guides to product/service pages and clear conversion paths.

## Entity, reputation and structured data
- Keep organization name, website, address, contact methods and business identity consistent across owned pages and external listings.
- Audit existing schema.org JSON-LD and implement only types and properties justified by visible page content (e.g. Organization, LocalBusiness or AutoRental where appropriate, BreadcrumbList, Product/Offer only when facts exist). Validate JSON syntax and eligibility separately; schema does not guarantee rich results or AI citations.
- Recommend legitimate third-party references, reputable directories, editorial coverage and authentic reviews. Never fabricate endorsements or use spam link schemes.

## Measurement and evaluation
- Build a fixed multilingual prompt set reflecting real buyer questions and competitors; record model, date, locale, query, whether the brand appears, citation URLs, recommendation context and landing-page traffic.
- Separate: brand mention rate, cited-source rate, AI-referred sessions, qualified leads and bookings. Model answers vary and are not reproducible rankings.
- If model/browser access is unavailable, produce a reproducible testing plan rather than claiming live AI visibility.
- Add analytics events only when compatible with consent/privacy requirements; do not overwrite existing tracking.

## Execution discipline
1. Audit before editing. Create `reports/geo-audit.md` with severity P0/P1/P2, affected URLs/files, evidence, proposed fix and verification method.
2. Draft a prioritized implementation plan based on impact, effort and business value.
3. Implement safe, scoped changes in the actual project when requested. Preserve existing UI, translations, routing, booking flow and analytics. Do not change prices, deposits, insurance terms or delivery policies without verified source data or approval.
4. Run available tests, builds, schema checks and link checks. Record command outputs and failures. Do not claim tests were run if they were not.
5. Deliver `reports/geo-changelog.md`, `reports/geo-test-plan.md` and a short Russian-language summary: done, evidence, risks, pending inputs, next actions.

## For vehicle rental websites
Consult `references/car-rental.md` for industry-specific question clusters, content and commercial safeguards.

## Source and epistemic rules
- GEO is an evolving practice; search engine and AI product behavior may change. Verify current official crawler and structured-data documentation before prescribing platform-specific controls.
- Do not confuse AI training crawler access with AI search inclusion.
- Cite primary documentation for technical recommendations where possible.
- Treat the Yandex Practicum article as conceptual inspiration, not proof of specific ranking mechanisms: https://thecode.media/kak-popast-v-otvety-nejrosetej-geo/
