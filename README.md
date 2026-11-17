# Landing Page Intelligence

**An evidence-led landing page audit toolkit for Claude.**

Landing Page Intelligence is an open-source suite of **13 Claude Agent Skills**: 12 specialist audit skills and one orchestration skill that combines them into a complete landing page audit.

It helps marketers, founders, agencies and conversion specialists understand what a landing page communicates, where visitors may encounter friction, which improvements deserve attention first, and how recommendations can be validated.

> **Audit what visitors experience. Understand what may obstruct action. Prioritise what to improve.**

---

## What is included?

### 12 specialist audit skills

| # | Skill | What it examines |
|---:|---|---|
| 1 | **UX Audit** (`ux-audit`) | Usability, information architecture, visual hierarchy, interaction design, cognitive load and visitor journey |
| 2 | **CRO Audit** (`cro-audit`) | Conversion objectives, funnel, friction, research evidence, hypotheses, prioritisation and experimentation |
| 3 | **Content & Copywriting Audit** (`content-copywriting-audit`) | Landing page messaging, persuasion, clarity, proof and **15 embedded copywriting frameworks** |
| 4 | **CTA Audit** (`cta-audit`) | CTA inventory, action clarity, hierarchy, placement, microcopy, destinations and interaction |
| 5 | **Trust & Credibility Audit** (`trust-credibility-audit`) | Testimonials, reviews, case studies, credentials, guarantees, security and claim-proof alignment |
| 6 | **Mobile Experience Audit** (`mobile-experience-audit`) | Responsive layout, readability, touch targets, navigation, forms, overlays and mobile conversion journey |
| 7 | **Performance Audit** (`performance-audit`) | Loading speed, Core Web Vitals, images, scripts, CSS, render-blocking resources and third-party impact |
| 8 | **Competitor Benchmarking Audit** (`competitor-benchmarking-audit`) | Dated comparison of positioning, offer, proof, page structure, conversion journey and differentiation |
| 9 | **Offer & Value Proposition Audit** (`offer-value-proposition-audit`) | Offer clarity, audience-fit, perceived value, pricing, packaging, risk reversal and differentiation |
| 10 | **Message Match & Traffic Alignment Audit** (`message-match-audit`) | Alignment between the landing page and the promise made by ads, search results, emails or referrals |
| 11 | **Accessibility & Inclusive Design Audit** (`accessibility-audit`) | WCAG 2.2-referenced accessibility, contrast, semantics, keyboard access, forms, focus and inclusive usability |
| 12 | **Strategic Recommendations & Optimization Roadmap** (`optimization-roadmap`) | Coverage, evidence consolidation, root causes, prioritised opportunities, implementation briefs, experiments and a 30-day plan |

### 1 orchestration skill

**Complete Audit** (`complete-audit`) coordinates all 12 specialist modules, collects business context once, reviews the landing page, checks module outputs and consolidates the findings into one integrated report and optimisation roadmap.

Each specialist skill can be used independently. The Complete Audit skill requires the 12 specialist skills to be installed alongside it.

---

## Why use Landing Page Intelligence?

A useful audit should do more than list generic best practices. It should connect each important observation to evidence, visitor impact and a practical next step.

The suite is designed around six principles:

1. **Evidence before assumption.** Findings distinguish what was observed, supported by data, inferred or still requires verification.
2. **Business context matters.** Recommendations are evaluated against the offer, audience, traffic source and conversion objective.
3. **Specialist depth.** Each module has its own scope, procedure, finding format and required deliverables.
4. **Traceable recommendations.** Significant findings carry stable identifiers, page locations, evidence, priority and confidence.
5. **Preserve what works.** Effective page elements are recorded rather than changed merely for novelty.
6. **Audit before implementation.** The default mode is diagnosis and recommendations. Implementation happens only when explicitly requested and authorised.

## Two ways to use the skills

### 1. Run a standalone audit

Install and invoke the specialist skill that matches the work you need.

Examples:

```text
Run a UX audit on https://example.com/landing.
```

```text
Audit the calls to action on https://example.com/landing.
```

```text
Compare this landing page with the competitor URLs I provide.
```

```text
Audit this page's message match against the Google Ads copy below.
```

### 2. Run the complete audit

Install all 13 skills, then ask Claude to run the full audit:

```text
Run the complete Landing Page Intelligence audit for
https://example.com/landing.
```

The `complete-audit` skill coordinates the 12 specialist modules in sequence and runs the optimisation roadmap after the module findings have been collected.

To protect the depth of the specialist audits, the orchestrator:

- Reads each module skill completely before running it, using line ranges where needed.
- Checks each module against a per-module output checklist and quality gate.
- Runs the work in stages and saves module outputs and a run record so an interrupted audit can be resumed.
- Can run continuously or in checkpointed mode when you request pauses between stages.
- Discloses incomplete modules or evidence gaps rather than silently skipping them.

## How findings are handled

The skills use common conventions so findings can be compared and consolidated:

| Convention | Meaning |
|---|---|
| **Observed** | Directly visible or verified from the page or supplied material |
| **Data-Supported** | Supported by supplied analytics, testing or research |
| **Inferred** | A reasoned interpretation of the available evidence |
| **Requires Verification** | Cannot be confirmed without further access, measurement or research |
| **P0 – Critical** | Serious issue or blocker requiring immediate attention |
| **P1 – High** | Important issue or opportunity with material relevance |
| **P2 – Medium** | Meaningful improvement with moderate impact |
| **P3 – Low** | Lower-impact refinement |
| **Confidence: High / Medium / Low** | How strongly the available evidence supports the finding |

Each applicable criterion is scored from **0 to 5**, or marked **N/A** when it cannot be evaluated. A module score is calculated as:

`Module Score = (Points Earned / Maximum Applicable Points) × 100`

The overall score is the average of applicable module scores. Scores are diagnostic interpretations, not industry benchmarks or predictions of conversion performance.

Finding identifiers make recommendations traceable across modules. Examples include `UX-`, `CRO-`, `COPY-`, `CTA-`, `TRUST-`, `MOB-`, `PERF-`, `COMP-`, `OFFER-`, `MATCH-` and `A11Y-`. Roadmap items use `RM-`; experiments use `EXP-`.

## Installation

Each skill is stored in its own folder and contains a `SKILL.md`.

### Claude.ai

1. Download or clone this repository.
2. Zip each individual skill folder so that the ZIP contains the skill folder at its top level.
3. Upload each skill ZIP through Claude's Skills settings.
4. For a complete audit, install all 12 specialist skills as well as `complete-audit`.

The exact menu names may vary as Claude's interface evolves. Follow Anthropic's current Skills documentation if the interface differs.

To create one ZIP per skill from the `skills` directory:

```bash
for d in */; do
  zip -r "${d%/}.zip" "$d"
done
```

### Claude Code

Copy the skill folders into your personal or project skills directory:

```bash
# Personal skills
cp -R skills/* ~/.claude/skills/

# Or copy them into the current project's skills directory
cp -R skills/* .claude/skills/
```

### Claude API

Use the current Anthropic Skills API documentation for the supported upload and invocation workflow.

## Repository structure

```text
Landing-Page-Intelligence/
├── README.md
├── CONTRIBUTING.md
├── LICENSE
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

## Contributing

Contributions are welcome. Before proposing a substantial change, please read [CONTRIBUTING.md](CONTRIBUTING.md).

Useful contributions include:

- Reporting unclear, conflicting or misleading instructions.
- Improving evidence handling and recommendation specificity.
- Adding privacy-safe test cases and expected audit qualities.
- Improving documentation and installation guidance.
- Identifying outdated technical or standards references.

Please do not submit confidential client data, personal information, credentials or unsupported claims.

## Sources and attribution

- The Accessibility Audit references **WCAG 2.2** from the World Wide Web Consortium (W3C).
- Core Web Vitals thresholds are based on Google's published web.dev guidance; consult current guidance because thresholds and recommendations may evolve.
- The Value Equation lens in `offer-value-proposition-audit` is attributed to Alex Hormozi.
- Persuasion lenses in `offer-value-proposition-audit` and `message-match-audit` are adapted, in the project's own words, from ideas in Andy Maslen, *Persuasive Copywriting: Using Psychology to Influence, Engage and Sell* (Kogan Page, 2015). No text from the book is reproduced.
- Named copywriting frameworks and usability heuristics belong to their respective originators.

## Limitations

Landing Page Intelligence produces diagnostic assessments and practical recommendations. It does not guarantee conversion improvement, speed gains or search rankings. It does not provide legal advice, accessibility certification or security assurance.

The skills do not assume access to analytics, heatmaps, session recordings, user research or A/B testing platforms. When those materials are not supplied or accessible, findings must state the evidence limitations and distinguish observations from hypotheses.

## License

Released under the [MIT License](LICENSE).

