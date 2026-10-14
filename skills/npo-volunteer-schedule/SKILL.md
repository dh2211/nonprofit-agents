---
name: npo-volunteer-schedule
description: "Builds a volunteer schedule and the messages that go with it: shift grid, coverage gaps, reminders, and change notices, using roles and placeholders instead of volunteer contact details. Use when an organization asks for a volunteer rota, shift schedule, coverage plan, or volunteer reminder messages."
license: MIT
---

# Volunteer schedule

Plan shifts so every slot is covered and every volunteer knows when they're needed.

## Ask first

1. The shifts: dates, times, locations, and how many volunteers each needs, by role.
2. Availability, as initials or volunteer IDs, never phone numbers or addresses.
3. Rules: maximum hours, required pairings (for example, two adults with children), required supervisors.
4. The messages needed: confirmation, reminder, change notice, thank-you.

## Steps

1. Build a shift grid: date, time, location, role, slots needed, assigned (initials or IDs).
2. Apply the rules. Flag any shift that breaks one, such as a lone volunteer where the policy requires two.
3. List coverage gaps clearly.
4. Draft each message with placeholders: `[volunteer first name]`, `[shift date]`, `[location]`. Keep reminders short.
5. Add a thank-you for after the shift.

## Output

The shift grid, flags and gaps, and the messages. Remind the user to send messages from their own volunteer system so contact details stay there.

## Guardrails

- Real numbers only: use only the figures, outcomes, quotes, and stories the organization gives you, with their dates and sources. Write `[number from your records]` where one is missing. Never invent statistics, outcomes, quotes, partners, funders, or the people you serve.
- Funder rules first: follow the guidelines, eligibility rules, format, word limits, and AI-use policy the user gives you. If you don't have the guidelines, ask for them. Never misstate eligibility, budgets, or partnerships.
- Privacy: work without donor, volunteer, or client names, contact details, giving history, health details, or background-check information. If the user pastes them, replace them with placeholders such as `[donor name]` and say that you did. Honor anonymity and contact preferences.
- Consent and dignity: use only real stories the organization says were shared with consent. Describe people with respect. Don't exaggerate need or outcomes, and label any composite story as a composite.
- The organization decides: you draft. Nothing is submitted or sent automatically. Receipt and tax wording, budgets, and safeguarding steps must be checked by someone qualified at the organization. This is not legal, tax, accounting, or fundraising-compliance advice.
