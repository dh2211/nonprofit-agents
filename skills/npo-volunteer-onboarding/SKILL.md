---
name: npo-volunteer-onboarding
description: "Writes a volunteer onboarding guide and welcome message: what to expect on the first day, who to ask, key procedures, safeguarding and conduct rules from the organization's policy, and a first-week checklist. Use when an organization asks for a volunteer handbook section, a welcome email, or first-day instructions."
license: MIT
---

# Volunteer onboarding

Help a new volunteer feel welcome and know exactly what to do.

## Ask first

1. The role, ideally from the `npo-volunteer-role` skill.
2. First-day logistics: where to go, when, what to bring, who to ask for (role).
3. The organization's policies to include: code of conduct, safeguarding, confidentiality, health and safety, expenses. Paste them; don't summarize policies from memory.
4. The format: welcome email, one-page guide, or handbook section.

## Steps

1. Write a short welcome that names the difference the role makes.
2. Write first-day logistics as a numbered list.
3. Summarize each policy in plain words, then link or attach the full policy. Keep the organization's exact wording for safeguarding and confidentiality rules.
4. Add "Who to ask" by role, and what to do if something goes wrong or someone is at risk, from the organization's procedure.
5. Add a first-week checklist with `- [ ]` boxes.

## Output

The welcome message, the guide, and a list of policy text the organization must supply or confirm.

## Guardrails

- Real numbers only: use only the figures, outcomes, quotes, and stories the organization gives you, with their dates and sources. Write `[number from your records]` where one is missing. Never invent statistics, outcomes, quotes, partners, funders, or the people you serve.
- Funder rules first: follow the guidelines, eligibility rules, format, word limits, and AI-use policy the user gives you. If you don't have the guidelines, ask for them. Never misstate eligibility, budgets, or partnerships.
- Privacy: work without donor, volunteer, or client names, contact details, giving history, health details, or background-check information. If the user pastes them, replace them with placeholders such as `[donor name]` and say that you did. Honor anonymity and contact preferences.
- Consent and dignity: use only real stories the organization says were shared with consent. Describe people with respect. Don't exaggerate need or outcomes, and label any composite story as a composite.
- The organization decides: you draft. Nothing is submitted or sent automatically. Receipt and tax wording, budgets, and safeguarding steps must be checked by someone qualified at the organization. This is not legal, tax, accounting, or fundraising-compliance advice.
