# Landing Page Intelligence

A collection of Claude skills for evidence-based landing-page audits, adapted from the **Landing Page Intelligence — Universal 12-Module Landing Page Audit Master Prompt** supplied with this project.

Use any of the 12 module skills independently, or use the additional `complete-audit` skill to perform all 12 modules in one run and produce a consolidated report.

## Repository structure

```text
landing-page-intelligence/
├── README.md
├── LICENSE
├── CONTRIBUTING.md
└── skills/
    ├── ux-audit/SKILL.md
    ├── cro-audit/SKILL.md
    ├── content-copywriting-audit/SKILL.md
    ├── cta-audit/SKILL.md
    ├── trust-credibility-audit/SKILL.md
    ├── mobile-experience-audit/SKILL.md
    ├── performance-audit/SKILL.md
    ├── competitor-benchmarking-audit/SKILL.md
    ├── offer-value-proposition-audit/SKILL.md
    ├── message-match-audit/SKILL.md
    ├── accessibility-audit/SKILL.md
    ├── optimization-roadmap/SKILL.md
    └── complete-audit/SKILL.md
```

`complete-audit` is an additional, independent skill. It does not depend on installing the other 12 folders; it contains the full 12-module workflow itself.

## Skills

| Skill folder | Purpose |
|---|---|
| `ux-audit` | Navigation, structure, hierarchy, readability, cognitive load and visitor flow |
| `cro-audit` | Conversion goals, competing actions, friction, forms, objections and conversion hypotheses |
| `content-copywriting-audit` | Headline, message, benefits, persuasion, structure and targeted replacement copy |
| `cta-audit` | CTA wording, hierarchy, visibility, placement, destinations and accessibility |
| `trust-credibility-audit` | Proof, credibility, transparency, identity, privacy and risk-reversal signals |
| `mobile-experience-audit` | Responsive layout, mobile readability, touch usability, forms and the mobile journey |
| `performance-audit` | Measured speed evidence, Core Web Vitals and technical performance risks |
| `competitor-benchmarking-audit` | Evidence-based comparison with competitors supplied or approved by the user |
| `offer-value-proposition-audit` | Offer clarity, audience fit, perceived value, differentiation and risk reversal |
| `message-match-audit` | Alignment between campaign/traffic promises and landing-page experience |
| `accessibility-audit` | Inclusive usability review using WCAG 2.2 as a reference framework |
| `optimization-roadmap` | Prioritization, experiments and a practical 30-day improvement plan |
| `complete-audit` | One-run audit across all 12 modules with combined scorecard and roadmap |

## Use one skill

Install or copy the folder for the module you need, keeping its `SKILL.md` inside that folder. For Claude Code, copy skill folders into a personal or project skills directory:

```bash
# Personal skills
mkdir -p ~/.claude/skills
cp -R skills/ux-audit ~/.claude/skills/

# Or project-specific skills, from your project root
mkdir -p .claude/skills
cp -R /path/to/landing-page-intelligence/skills/ux-audit .claude/skills/
```

Use `complete-audit` when you want all twelve modules in one Claude interaction:

```bash
cp -R skills/complete-audit ~/.claude/skills/
```

Claude product import mechanisms may vary. Where the interface offers custom skills, import the relevant skill folder using the method supported by that Claude version. You may install the 12 focused skills, the complete audit, or both.

### Example full-audit request

> Run a complete 12-module landing-page audit for [URL]. The business is [brand/business], the product or service is [offer], the target audience is [audience/market], and the primary conversion goal is [goal]. Please use the attached campaign/ad and competitor URLs where relevant. Analytics or performance measurements are [available/not available].

The skill may ask for essential missing context before auditing. It does not require metrics the business does not have. If the URL cannot be inspected, provide screenshots, page text or a recording; conclusions must then be limited to that evidence.

## Evidence and scoring principles

The skills distinguish direct observations, business-reported information, hypotheses and recommendations. They do not invent conversion rates, performance metrics, testimonials, certifications, guarantees, competitor results or user research. They label untestable items and disclose the evidence method.

Applicable criteria use a 0–5 diagnostic scale and module scores are expressed from 0–100. Not-applicable or unevaluable items are excluded from the denominator; the full audit discloses any unevaluated modules and excludes them from the provisional overall average. Scores are diagnostic interpretations, not industry benchmarks or promises of business outcomes.

The full-audit skill includes a scorecard, detailed findings for all modules, targeted copy suggestions, competitor analysis when sources are supplied, consolidated priorities, three proposed experiments, a 30-day roadmap and a final consultant verdict. It does not promise conversion uplift. If testing feasibility is unclear or traffic is low, it recommends suitable qualitative validation.

## Contributing

See [CONTRIBUTING.md](CONTRIBUTING.md) for how to propose corrections or improvements. The license template is in [LICENSE](LICENSE); replace its copyright-holder placeholder before publishing under that license.
