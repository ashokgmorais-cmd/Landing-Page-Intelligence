---
name: performance-audit
description: Assess available technical performance evidence for an existing landing page, including Core Web Vitals, loading behavior, assets, scripts and likely bottlenecks. Use when asked to audit landing-page speed or performance.
---

# Landing Page Performance Audit

## Purpose

Run a standalone, evidence-based audit of the **Performance** module for an existing landing page. The purpose is to diagnose the current experience and recommend practical improvements, not to build a replacement page.

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

Review only available evidence about load timing, Core Web Vitals, image/font delivery, JavaScript/CSS, render-blocking resources, layout shifts, third-party scripts, lazy loading and network/resource efficiency. Record URL, date/time, device/network, tool, test conditions, and whether results are lab or field data when known.

## Required deliverable

Report measurements with units and provenance; distinguish measured findings, visual observations and hypotheses; explain user impact cautiously; recommend specific next diagnostics/fixes; assign priority/confidence and score. If no technical measurements are available, mark performance findings unverified and explain how to obtain evidence.

## Module-specific guidance

Reference thresholds: LCP good ≤2.5 s, needs improvement >2.5–4 s, poor >4 s; INP good ≤200 ms, needs improvement >200–500 ms, poor >500 ms; CLS good ≤0.1, needs improvement >0.1–0.25, poor >0.25. Use exact boundary consistently. Do not invent metrics or claim a pass without valid measurements. A screenshot cannot establish speed.

## Strategic diagnostic questions

- Which performance conclusions are backed by field/lab measurements, and under what device, network, region and test conditions?
- Is the proposed fix connected to an observed bottleneck, or is it a generic optimization checklist?
- Could a third-party script, oversized asset, font, or layout shift affect a critical action; what evidence would isolate it?
- What should be measured after remediation, and how will lab results be distinguished from real-user outcomes?

## Final quality check

Before delivering, confirm that the review stayed within this module, every material conclusion is evidence-labelled, all recommendations are actionable and appropriately prioritized, unknowns remain unknown, N/A items were excluded from scoring, and the score calculation is correct. If the user asks for a full 12-module audit, explain that this skill covers one module and can be run alongside the other skills in this repository.
