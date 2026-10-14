---
name: npo-grant-proposal
description: "Drafts grant proposal sections from a nonprofit's real program facts and the funder's own guidelines: need, program description, goals and outcomes, evaluation, organizational capacity, and sustainability, within the funder's word limits. Use when an organization asks for a grant proposal, a letter of inquiry, or one section of an application."
license: MIT
---

# Grant proposal

Draft what this funder asks for, in the order and length they ask for it, from the organization's real facts.

## Ask first

1. The funder's guidelines, pasted in: priorities, eligibility, required sections, word or character limits, attachments, deadline, and any policy on AI-assisted applications. If they aren't available, stop and ask for them.
2. The program facts, ideally from the `npo-program-facts` skill.
3. The amount requested and what it pays for.
4. Whether this is a letter of inquiry, a full proposal, or one section.

## Steps

1. Check fit first. List each eligibility rule and priority, and whether the facts show the organization meets it. If something doesn't fit or is unclear, say so before drafting. Never stretch the facts to fit.
2. If the funder restricts or asks you to disclose AI use, tell the user before drafting and follow their decision.
3. Outline the proposal using the funder's section names and order, with each section's limit.
4. Draft each section from the facts. Keep each number exactly as given, with its date. Use `[number from your records]` for gaps.
5. Answer the funder's actual question in each section's first sentence.
6. Count words or characters per section and cut to fit the limits.
7. Check the requested amount matches the budget. Use the `npo-budget-narrative` skill for the budget justification.

## Output

1. Fit check against the guidelines.
2. The draft, section by section, each with its count and limit.
3. "Check before you submit": every figure to verify against records, every gap, every attachment the funder requires, and the AI-use policy.

## Guardrails

- Real numbers only: use only the figures, outcomes, quotes, and stories the organization gives you, with their dates and sources. Write `[number from your records]` where one is missing. Never invent statistics, outcomes, quotes, partners, funders, or the people you serve.
- Funder rules first: follow the guidelines, eligibility rules, format, word limits, and AI-use policy the user gives you. If you don't have the guidelines, ask for them. Never misstate eligibility, budgets, or partnerships.
- Privacy: work without donor, volunteer, or client names, contact details, giving history, health details, or background-check information. If the user pastes them, replace them with placeholders such as `[donor name]` and say that you did. Honor anonymity and contact preferences.
- Consent and dignity: use only real stories the organization says were shared with consent. Describe people with respect. Don't exaggerate need or outcomes, and label any composite story as a composite.
- The organization decides: you draft. Nothing is submitted or sent automatically. Receipt and tax wording, budgets, and safeguarding steps must be checked by someone qualified at the organization. This is not legal, tax, accounting, or fundraising-compliance advice.
