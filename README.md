# Landing Page Intelligence

### Turn landing pages into conversion opportunities through evidence-based AI audits.

**Landing Page Intelligence** is an open-source collection of AI-powered Claude Agent Skills designed to evaluate landing pages systematically across 12 critical dimensions of user experience, conversion optimisation, messaging, credibility and performance.

Instead of relying on generic AI feedback, these skills follow a structured audit methodology that distinguishes observable evidence, business claims, interpretations, hypotheses and actionable recommendations.

Whether you are a digital marketer, CRO specialist, business owner, agency, or developer, Landing Page Intelligence helps you identify what is working, what is not, and what should be improved.

---

## Why Landing Page Intelligence?

A landing page can look attractive and still fail to convert.

Poor messaging, unclear offers, weak calls to action, missing trust signals and unnecessary friction can prevent visitors from taking action.

Landing Page Intelligence approaches this problem through a structured 12-module audit framework.

**The objective is simple: move beyond surface-level feedback and produce practical, prioritised recommendations.**

## What Can You Audit?

The framework evaluates landing pages across these 12 dimensions:

| # | Audit Module | What It Evaluates |
|---|---|---|
| 01 | UX Audit | Navigation, information architecture, hierarchy, readability and visitor journey |
| 02 | CRO Audit | Conversion goals, friction, forms, objections and decision barriers |
| 03 | Content & Copywriting | Headlines, messaging, benefits, persuasion and content structure |
| 04 | CTA Audit | CTA wording, placement, hierarchy, visibility and destinations |
| 05 | Trust & Credibility | Testimonials, credentials, proof, transparency and risk reversal |
| 06 | Mobile Experience | Responsive layout, mobile usability, readability and touch interactions |
| 07 | Performance | Page speed evidence, Core Web Vitals and technical performance risks |
| 08 | Competitor Benchmarking | Comparative positioning, offers, messaging and conversion experiences |
| 09 | Offer & Value Proposition | Offer clarity, audience fit, perceived value and differentiation |
| 10 | Message Match | Alignment between advertising, traffic sources and landing-page messaging |
| 11 | Accessibility | Inclusive usability and accessibility considerations using WCAG 2.2 as a reference |
| 12 | Strategic Recommendations | Prioritisation, experimentation and a practical 30-day optimisation roadmap |

## Two Ways to Use the Framework

### 1. Individual Audit Skills

The repository contains 12 standalone skills. Each can be used independently to investigate a specific landing-page dimension.

Use an individual skill when you need a focused assessment, such as a CRO audit, CTA review or accessibility assessment.

### 2. Complete Audit

The additional `complete-audit` skill combines all 12 modules into one comprehensive landing-page audit workflow.

It is independently usable and contains the complete audit methodology. You do not need to install the other 12 skills to run it.

**Recommended starting point: `complete-audit`.**

## Key Capabilities

- Structured 12-module landing-page assessment.
- Evidence-based findings rather than generic suggestions.
- Diagnostic scoring on a 0–100 scale.
- Identification of conversion barriers and usability issues.
- Targeted headline, messaging and CTA recommendations.
- Competitor comparisons when competitor URLs are supplied.
- Clear distinction between observed facts, reported claims, hypotheses and recommendations.
- Prioritised optimisation opportunities.
- Proposed A/B testing ideas.
- A practical 30-day optimisation roadmap.

## Installation — Claude

The `complete-audit` skill can be installed in Claude using its custom Skills interface.

1. Download or access the repository.
2. Navigate to `skills/complete-audit`.
3. Package the skill folder as a ZIP file, retaining `SKILL.md` inside it.
4. Open Claude.
5. Navigate to **Customize → Skills**.
6. Select **Add → Upload skill**.
7. Upload the ZIP file and enable the skill.

Once enabled, start a new conversation and request a complete landing-page audit.

## How to Use

Start by providing the following information:

1. Landing-page URL.
2. Business or brand name and product/service.
3. Target audience and market.
4. Primary conversion goal.
5. Offer details, including pricing, guarantees and key terms where available.

You can also provide optional information to improve the audit:

- Advertising or campaign materials.
- Competitor landing-page URLs.
- Customer pain points and objections.
- Testimonials, credentials and other trust assets.
- Analytics and conversion data.
- PageSpeed or Core Web Vitals reports.
- Brand and platform constraints.

The skill may request missing essential information before beginning the audit.

If the page cannot be accessed, provide screenshots, a screen recording or exported page content. Findings must be limited to the evidence available.

## Sample Audit

Explore a real-world landing page audit generated using the Landing Page Intelligence framework.

### Jones Gym – Complete Landing Page Audit

A comprehensive 12-module assessment of the Jones Gym website, covering:

- User Experience and Conversion Rate Optimisation.
- Content, Copywriting and Calls to Action.
- Trust, Credibility and Value Proposition.
- Mobile Experience and Accessibility.
- Strategic Recommendations and Optimisation Roadmap.

**[View the Complete Jones Gym Audit (PDF)](examples/Jones%20Gym%20Complete%20Landing%20Page%20Audit%20%2812%20Modules%29.pdf)**

This example demonstrates how the framework identifies conversion barriers, evaluates available evidence and translates findings into actionable recommendations.

## Evidence-Based Scoring

The framework uses a diagnostic scoring methodology.

- Applicable audit criteria are evaluated on a 0–5 scale.
- Module scores are expressed on a 0–100 scale.
- Not-applicable and unevaluable criteria are excluded from the relevant denominator.
- Unevaluated modules are disclosed rather than assigned invented scores.
- The provisional overall score is calculated from applicable modules.

Scores are diagnostic assessments, not industry benchmarks, guarantees or predictions of conversion performance.

The framework does not fabricate analytics, performance measurements, customer testimonials, certifications, competitor results or research findings.

## Repository Structure

```text
landing-page-intelligence/
│
├── README.md
├── LICENSE
├── CONTRIBUTING.md
│
└── skills/
    ├── ux-audit/
    ├── cro-audit/
    ├── content-copywriting-audit/
    ├── cta-audit/
    ├── trust-credibility-audit/
    ├── mobile-experience-audit/
    ├── performance-audit/
    ├── competitor-benchmarking-audit/
    ├── offer-value-proposition-audit/
    ├── message-match-audit/
    ├── accessibility-audit/
    ├── optimization-roadmap/
    └── complete-audit/
```

Each skill folder contains its own `SKILL.md` instructions.

## Who Is This For?

- Digital marketing professionals.
- Conversion Rate Optimisation specialists.
- SEO and content strategists.
- Freelance marketers and consultants.
- Digital marketing agencies.
- SaaS founders and startup teams.
- Small and medium-sized businesses.
- Web designers and developers.
- AI enthusiasts exploring practical agent workflows.

## Contributing

Landing Page Intelligence is an open-source project, and contributions are welcome.

You can contribute by:

- Improving audit instructions.
- Identifying gaps in the evaluation framework.
- Suggesting additional audit criteria.
- Improving scoring consistency.
- Reporting issues or inaccurate recommendations.
- Sharing practical use cases and feedback.

Please read [CONTRIBUTING.md](CONTRIBUTING.md) before submitting a contribution.

## Project Roadmap

The project aims to evolve through practical usage, community feedback and continuous improvements.

Potential future developments include:

- More robust evidence-verification workflows.
- Improved scoring consistency.
- Additional industry-specific audit considerations.
- Better integration with analytics and performance data.
- Expanded reporting and benchmarking capabilities.

Feature development will be guided by real-world use cases and community contributions.

## Open Source

This project is intended to be an open, collaborative resource for people working with landing pages, marketing and conversion optimisation.

Explore the skills, try the framework, report issues and contribute improvements.

**If you find this project useful, consider giving it a ⭐ on GitHub and sharing it with others.**

---

*Landing Page Intelligence — Evidence. Insight. Optimisation.*
