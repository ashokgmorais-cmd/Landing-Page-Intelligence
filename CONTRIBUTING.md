# Contributing

Thanks for helping improve Landing Page Intelligence. Contributions should make audits more accurate, useful, evidence-aware and actionable while preserving the ability to use each module independently.

## Before proposing a change

- Identify the relevant folder under `skills/`; make a focused change to the affected skill(s).
- For cross-module changes, check both the 12 individual skills and `skills/complete-audit/SKILL.md` so their methodology stays aligned.
- Keep each skill self-contained. Do not make an individual module skill require the complete-audit skill or another module directory.
- Do not add claims that are not supported by the supplied source prompt, valid measurement, or clearly identified expertise. Label assumptions and hypotheses.

## Standards for skill changes

Each skill should:

- Retain valid YAML frontmatter with a unique kebab-case `name` and a useful `description` that explains what it does and when to use it.
- Keep its scope explicit and provide a clear workflow and usable output format.
- Separate observed evidence, business-reported information, inference/hypothesis and recommendation.
- Avoid inventing business facts, performance or conversion outcomes, testimonials, credentials, guarantees or competitor results.
- State evidence limitations and never claim testing or standards conformance that did not occur.
- Use the shared 0–5 criterion scoring approach, exclude N/A criteria, and explain when a module cannot be evaluated.
- Prefer concise, specific instructions and actionable recommendations over generic CRO advice.

For the complete audit, preserve all 12 modules, the report sequence, scorecard and overall-score handling, three experiment proposals, 30-day roadmap and the rule that the roadmap score evaluates roadmap quality rather than the page.

## Validation checklist

Before submitting a change:

1. Confirm the skill folder still contains its `SKILL.md`.
2. Review the edited skill in full for contradictory or repeated instructions.
3. Verify frontmatter YAML and that the `name` matches the folder name.
4. Confirm all changes respect the evidence and non-fabrication rules above.
5. For the complete audit, confirm every module is present and unevaluable modules are disclosed and excluded from the provisional average.
6. If multiple tools or Claude versions are involved, note compatibility constraints in the pull request.

## Pull requests

Include a concise summary of the skills changed, the rationale, and any example request or edge case that motivated the update. Call out behavioral changes, scoring changes, and any changed assumptions. Keep unrelated edits in separate pull requests when practical.
