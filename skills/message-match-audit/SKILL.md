---
name: message-match-audit
description: Assess whether an existing landing page matches the promise and expectations of its traffic sources, ads, campaign creative, email or search intent. Use when asked for message-match or traffic-alignment review.
---

# Landing Page Message Match & Traffic Alignment Audit

## Purpose

Run a standalone, evidence-based audit of the **Message Match & Traffic Alignment** module for an existing landing page. The purpose is to diagnose the current experience and recommend practical improvements, not to build a replacement page.

## How to run this skill independently

This skill audits **only its named module**. Do not assume any other module has been run. Begin with the user's request and supplied materials. If essential context is missing, ask only for information that materially affects this module; do not block on analytics or details that are unavailable. If the page URL is inaccessible, request screenshots, a recording, exported page text, or HTML. Work within the evidence available and label the scope limitation.

Useful context, when available: business/brand and industry; target audience and geography; page URL or assets; product/service and business model; primary conversion goal; offer/price; campaign or traffic source; brand constraints; relevant competitors; and analytics/testing data. Mark missing data **Not provided** or **Unavailable** rather than guessing. Distinguish business-provided claims from your own page observations.

## Evidence and integrity rules

- Separate **Observed** (directly visible/tested), **Reported** (provided by the business), **Inference/Hypothesis** (plausible but unverified), and **Recommendation**.
- Tie important findings to a page section, element, source URL, supplied asset or test result. Quote exact copy only if it is available; otherwise label a paraphrase.
- Explain **what** is present, **why** it matters to the relevant user/task, and **what** to change. Avoid treating every weakness as a proven conversion loss.
- Do not invent business facts, results, analytics, guarantees, user research, certifications, or test outcomes. Avoid causal and uplift claims unless supported by valid experiments.
- If only static screenshots or text are available, do not claim to have tested links, forms, responsive behavior, performance, keyboard access, or assistive technology.
- Consider audience, offer, conversion goal, traffic context and accessibility needs where supplied. State assumptions and material limitations.

## Priorities, confidence and scoring

Use priority **P0 Critical** (serious broken/usability/trust issue requiring immediate attention), **P1 High** (important, potentially consequential), **P2 Medium** (valuable after higher priorities), **P3 Low** (minor refinement/longer-term). Use confidence **High** (directly observable/measured), **Medium** (reasonable evidence with gaps), or **Low** (limited evidence or substantial assumptions).

Score applicable criteria from 0–5: 0 missing/broken/critically deficient; 1 very poor; 2 below expectations; 3 acceptable; 4 very good; 5 excellent. Mark unassessable items N/A and exclude them from the denominator. Calculate the module score as `(points earned ÷ maximum applicable points) × 100`, rounded to a whole number; state the numerator/denominator or list scored criteria. If nothing can reasonably be scored, report **Not Evaluated**, not 0. Do not treat this diagnostic score as an industry benchmark or a forecast of conversion performance.

## Output format

Write a self-contained, client-ready Markdown audit with a title, audit scope/evidence basis, concise summary, strengths, prioritized findings/recommendations (prefer a table where useful), module score, overall evidence confidence, and limitations/next evidence needed. Keep advice specific and actionable. Do not produce a full multi-module report or score unless the user explicitly asks for one.


## Module-specific review checklist

Compare provided source materials with the landing page: ad-to-headline alignment, campaign promise, audience, offer consistency, pricing/conditions, visuals/brand cues, CTA alignment, search intent and continuity through the visitor journey. Inspect only campaign/source inputs actually supplied or accessible.

## Required deliverable

State which traffic sources were assessed and which were not. Show aligned elements, mismatches and likely expectation gaps, with source/landing-page evidence, recommendation, priority, confidence and module score. If ads/campaign/search context is unavailable, explicitly mark the complete audit as not possible and provide only a limited page-side review.

## Module-specific guidance

Do not infer campaign promises from a landing page alone, nor claim a mismatch without a source message. Verify that referenced terms, offer details and destinations match. Clearly separate exact source copy from summary/paraphrase.

## Strategic diagnostic questions

- What exact expectation did the source message create for this audience, and where is that source evidence?
- Does the landing page continue the same promise, audience, offer, conditions and next step—or introduce a material shift?
- Is a mismatch specific to a campaign/segment, or is the evidence too limited to generalize across traffic sources?
- If source assets are missing, what campaign inputs are needed to complete the comparison rather than guess?

## Final quality check

Before delivering, confirm that the review stayed within this module, every material conclusion is evidence-labelled, all recommendations are actionable and appropriately prioritized, unknowns remain unknown, N/A items were excluded from scoring, and the score calculation is correct. If the user asks for a full 12-module audit, explain that this skill covers one module and can be run alongside the other skills in this repository.
