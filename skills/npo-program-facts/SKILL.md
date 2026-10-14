---
name: npo-program-facts
description: "Organizes a nonprofit's real program information into a reusable fact sheet and simple logic model: need, activities, outputs, outcomes, with the date and source of every number. Use when an organization starts a grant season, asks for a logic model or theory of change, or wants one place for the facts other skills draw on."
license: MIT
---

# Program facts

Build one fact sheet from the organization's own records, so every later draft uses the same, sourced numbers.

## Ask first

1. The program: name, purpose, who it serves (described in general terms), where, and since when.
2. The organization's numbers, each with its date range and source: people served, sessions held, outcomes measured, budget, staff and volunteers.
3. Any evaluation, survey, or report the numbers come from.
4. Stories the organization has consent to use, already stripped of identifying details.

## Steps

1. Write the need statement using only facts the organization gives. Where it cites outside data, keep its source and ask the user to confirm it; don't add statistics from memory.
2. Build a logic model table: inputs, activities, outputs (counts of what was done), short-term outcomes, longer-term outcomes. Put each number in with its date and source.
3. Separate outputs from outcomes. "120 workshops held" is an output; "68% of participants report ..." is an outcome, and only goes in if the organization measured it.
4. List gaps: claims a funder will likely ask for that have no number yet, written as `[number from your records]`.
5. List the consented stories with a one-line summary each.

## Output

Program summary, need statement, logic model table, numbers table (figure, date range, source), gaps, consented stories. Tell the user to keep this sheet current; the `npo-grant-proposal` skill and the `npo-impact-report` skill can start from it.

## Guardrails

- Real numbers only: use only the figures, outcomes, quotes, and stories the organization gives you, with their dates and sources. Write `[number from your records]` where one is missing. Never invent statistics, outcomes, quotes, partners, funders, or the people you serve.
- Funder rules first: follow the guidelines, eligibility rules, format, word limits, and AI-use policy the user gives you. If you don't have the guidelines, ask for them. Never misstate eligibility, budgets, or partnerships.
- Privacy: work without donor, volunteer, or client names, contact details, giving history, health details, or background-check information. If the user pastes them, replace them with placeholders such as `[donor name]` and say that you did. Honor anonymity and contact preferences.
- Consent and dignity: use only real stories the organization says were shared with consent. Describe people with respect. Don't exaggerate need or outcomes, and label any composite story as a composite.
- The organization decides: you draft. Nothing is submitted or sent automatically. Receipt and tax wording, budgets, and safeguarding steps must be checked by someone qualified at the organization. This is not legal, tax, accounting, or fundraising-compliance advice.
