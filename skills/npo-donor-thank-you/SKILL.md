---
name: npo-donor-thank-you
description: "Drafts warm, specific thank-you letters, emails, and notes to donors, using placeholders for donor details the organization adds in its own systems, and honoring anonymity and contact preferences. Use when an organization asks for a donor thank-you, an acknowledgment letter, a batch of thank-you notes, or a thank-you call script."
license: MIT
---

# Donor thank-you

Write a thank-you the donor will feel was meant for them, without putting their personal details into the AI tool.

## Ask first

1. The kind of gift (first gift, monthly, major, in-kind, event sponsor, memorial or tribute) and what it supports. Use placeholders for the donor and amount: `[donor name]`, `[gift amount]`.
2. One real thing the gift made possible, from the organization's records.
3. The format: letter, email, handwritten card, or call script. Who signs it.
4. Whether a receipt or tax statement must go with it, and the organization's approved wording if so.

## Steps

1. Open with thanks in the first sentence. No "Dear Friend" if the organization uses names.
2. Say what the gift does, with one concrete, real example. Use `[number from your records]` if the user gave none.
3. Keep it about the donor and the people served, not the organization's needs. Don't ask for another gift in a thank-you unless the user asks for it.
4. For tribute or memorial gifts, acknowledge the person honored with care.
5. If receipt or tax wording is needed, insert only the organization's approved text, or `[receipt wording: approved by your finance lead]`.
6. For a batch, write one base letter and two or three variant paragraphs for different gift types.

## Output

The thank-you, a subject line for email, and a checklist: names, amounts, gift details, and donor preferences (anonymity, how they like to be contacted) to confirm before sending.

## Guardrails

- Real numbers only: use only the figures, outcomes, quotes, and stories the organization gives you, with their dates and sources. Write `[number from your records]` where one is missing. Never invent statistics, outcomes, quotes, partners, funders, or the people you serve.
- Funder rules first: follow the guidelines, eligibility rules, format, word limits, and AI-use policy the user gives you. If you don't have the guidelines, ask for them. Never misstate eligibility, budgets, or partnerships.
- Privacy: work without donor, volunteer, or client names, contact details, giving history, health details, or background-check information. If the user pastes them, replace them with placeholders such as `[donor name]` and say that you did. Honor anonymity and contact preferences.
- Consent and dignity: use only real stories the organization says were shared with consent. Describe people with respect. Don't exaggerate need or outcomes, and label any composite story as a composite.
- The organization decides: you draft. Nothing is submitted or sent automatically. Receipt and tax wording, budgets, and safeguarding steps must be checked by someone qualified at the organization. This is not legal, tax, accounting, or fundraising-compliance advice.
