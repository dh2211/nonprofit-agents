---
name: npo-impact-report
description: "Writes an impact report for funders, donors, or the board using only the organization's own numbers, outcomes, and consented stories, with sources and honest notes on what didn't go to plan. Use when an organization asks for an impact report, an annual report section, a grant progress report, or a results summary."
license: MIT
---

# Impact report

Tell what happened, with the organization's real numbers, for the audience who will read it.

## Ask first

1. The audience: a specific funder (paste their reporting template), individual donors, or the board.
2. The period covered.
3. The numbers, with dates and sources, ideally from the `npo-program-facts` skill. For a grant report, the goals promised in the proposal.
4. Consented stories and quotes, with the person's preference on how they are named.
5. What didn't go to plan, and what the organization changed.

## Steps

1. For a grant report, follow the funder's template and order. Compare each promised goal with the actual result, side by side.
2. Lead with the two or three results the audience cares most about, in plain words.
3. Write every number exactly as given, with its period. Don't round up, combine numbers from different periods, or turn outputs into outcomes.
4. Use stories only as provided and consented. Describe people with dignity, by what they did, not by what they lack.
5. Include what didn't work and what changed. Funders and boards trust a report that has some.
6. Close with what's next and, for donors, a thank-you.

## Output

The report in Markdown, a sources table (figure, period, source), and "Check before you send": every number, quote, and consent to confirm.

## Guardrails

- Real numbers only: use only the figures, outcomes, quotes, and stories the organization gives you, with their dates and sources. Write `[number from your records]` where one is missing. Never invent statistics, outcomes, quotes, partners, funders, or the people you serve.
- Funder rules first: follow the guidelines, eligibility rules, format, word limits, and AI-use policy the user gives you. If you don't have the guidelines, ask for them. Never misstate eligibility, budgets, or partnerships.
- Privacy: work without donor, volunteer, or client names, contact details, giving history, health details, or background-check information. If the user pastes them, replace them with placeholders such as `[donor name]` and say that you did. Honor anonymity and contact preferences.
- Consent and dignity: use only real stories the organization says were shared with consent. Describe people with respect. Don't exaggerate need or outcomes, and label any composite story as a composite.
- The organization decides: you draft. Nothing is submitted or sent automatically. Receipt and tax wording, budgets, and safeguarding steps must be checked by someone qualified at the organization. This is not legal, tax, accounting, or fundraising-compliance advice.
