---
name: npo-event-plan
description: "Plans a nonprofit event: fundraiser, community day, volunteer appreciation, or open house, with goals, budget from the organization's figures, task list, run-of-show timeline, and safety and accessibility checks. Use when an organization asks for an event plan, a run of show, an event checklist, or an event timeline."
license: MIT
---

# Event plan

Plan an event the team can run, with the budget and people it really has.

## Ask first

1. The event type, goal (funds to raise, people to reach, thanks to give), date, place, and expected attendance.
2. Budget and known costs from the organization. Venue requirements if known.
3. Team: staff and volunteer roles available (roles, not names).
4. Audience needs: accessibility, languages, children, food restrictions.

## Steps

1. Restate the goal as something countable.
2. Build a budget table from the organization's figures. Mark unknown costs `[quote needed]`. Total it and check the arithmetic.
3. Build a backward task list from the event date: what, who (role), due date.
4. Write a run-of-show for the day: time, what happens, who leads, what is needed.
5. Add checks the organization must confirm with the venue and local authorities: permits, insurance, food handling, alcohol or raffle rules, capacity, first aid `[confirm with your venue and local authorities]`.
6. Add an accessibility check: step-free access, seating, captioning or interpretation, quiet space.
7. Add follow-up: thank-yous with the `npo-donor-thank-you` skill and a results summary.

## Output

Goal, budget table, task list, run-of-show, safety and permit checks, accessibility check, follow-up.

## Guardrails

- Real numbers only: use only the figures, outcomes, quotes, and stories the organization gives you, with their dates and sources. Write `[number from your records]` where one is missing. Never invent statistics, outcomes, quotes, partners, funders, or the people you serve.
- Funder rules first: follow the guidelines, eligibility rules, format, word limits, and AI-use policy the user gives you. If you don't have the guidelines, ask for them. Never misstate eligibility, budgets, or partnerships.
- Privacy: work without donor, volunteer, or client names, contact details, giving history, health details, or background-check information. If the user pastes them, replace them with placeholders such as `[donor name]` and say that you did. Honor anonymity and contact preferences.
- Consent and dignity: use only real stories the organization says were shared with consent. Describe people with respect. Don't exaggerate need or outcomes, and label any composite story as a composite.
- The organization decides: you draft. Nothing is submitted or sent automatically. Receipt and tax wording, budgets, and safeguarding steps must be checked by someone qualified at the organization. This is not legal, tax, accounting, or fundraising-compliance advice.
