---
name: ux-audit
description: Audit landing-page usability, information architecture, hierarchy, readability, navigation, cognitive load and visitor flow. Use when asked to assess or improve the user experience of an existing landing page, using a URL, screenshots, recordings or supplied page content.
---

# Landing Page UX Audit

## Purpose

Run a standalone, evidence-based audit of the **UX** module for an existing landing page. The purpose is to diagnose the current experience and recommend practical improvements, not to build a replacement page.

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

Review page structure and navigation; information architecture and section order; visual hierarchy and scanability; content grouping, readability and typography; spacing and consistency; findability of essential information; interaction clarity; cognitive load; and the visitor path to the stated goal.

## Required deliverable

Report a concise scope and evidence basis; what works well; an issue table with location/observation, why it matters to visitors, recommendation, priority and confidence; prioritized quick wins; and a 0–100 module score with calculation and rationale. Do not assess conversion lifts or make claims outside UX scope.

## Module-specific guidance

Give special attention to the hero-to-action path, whether headings support scanning, whether users can find price, eligibility, process, proof and next steps, and whether navigation distracts from the task. Avoid subjective design taste unless it creates a usability consequence.

## Strategic diagnostic questions

- Can a first-time visitor quickly identify who the page is for, what is offered, why it matters, and what to do next?
- Does the order of information answer the visitor's likely questions in sequence, or force them to hunt/remember?
- Is the visual hierarchy helping people make a decision, or merely decorating the page?
- Where does the experience create uncertainty, unnecessary choices, or avoidable mental effort? Treat aesthetic preference as a finding only when it has a usability consequence.

## Final quality check

Before delivering, confirm that the review stayed within this module, every material conclusion is evidence-labelled, all recommendations are actionable and appropriately prioritized, unknowns remain unknown, N/A items were excluded from scoring, and the score calculation is correct. If the user asks for a full 12-module audit, explain that this skill covers one module and can be run alongside the other skills in this repository.
