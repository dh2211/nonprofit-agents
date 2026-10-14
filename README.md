# nonprofit-agents

Agent Skills that help nonprofits with the writing and planning behind the mission: program fact sheets, grant proposals, budget narratives, impact reports, donor thank-yous, appeals, event plans, and volunteer roles, onboarding, and schedules.

Each skill is a folder with a `SKILL.md` file in the open [Agent Skills](https://agentskills.io/specification) format. You bring your own AI tool, ideally one your organization has approved. Claude Code, Codex, Cursor, Grok, OpenCode, and other agents document support for that format. You install the skills once, then ask in plain English: "Draft the need statement for this foundation's application. Their guidelines are below."

**Status: not yet tested live in any tool.** The skills pass the validator in this repository, and the worked examples were produced by following the skills by hand. Nobody has yet recorded a run in Claude Code, Codex, Cursor, Grok, or OpenCode. Please [report what you find](CONTRIBUTING.md).

## Real numbers only

Every figure, outcome, quote, and story must come from your own records. The skills use what you provide, write `[number from your records]` where something is missing, and never fill gaps with plausible-sounding statistics. Check every number before anything reaches a funder or donor.

## Quick start

1. Clone the repository:

   ```bash
   git clone https://github.com/NonprofitKit/nonprofit-agents.git
   ```

2. Copy the `skills/` folders into the skills folder your agent reads. For Claude Code on macOS or Linux:

   ```bash
   mkdir -p ~/.claude/skills
   cp -R nonprofit-agents/skills/* ~/.claude/skills/
   ```

   [docs/install.md](docs/install.md) lists the folder for each agent, with links to each tool's documentation. You don't need Node.js or any other software to use the skills.

3. Start your agent and ask for what you need:

   > Draft a thank-you letter for a first-time monthly donor to our after-school reading program. Signed by our executive director. Use placeholders for the donor's name and amount.

   The agent picks the matching skill, asks for anything missing, and drafts it.

## Skills

| Skill | What it makes |
| --- | --- |
| [npo-program-facts](skills/npo-program-facts/SKILL.md) | A sourced fact sheet and logic model that the other skills draw on |
| [npo-grant-proposal](skills/npo-grant-proposal/SKILL.md) | A fit check against the funder's guidelines, then proposal sections within their limits |
| [npo-budget-narrative](skills/npo-budget-narrative/SKILL.md) | A budget justification with the arithmetic checked against the funder's rules |
| [npo-impact-report](skills/npo-impact-report/SKILL.md) | An impact or grant progress report from your numbers and consented stories |
| [npo-donor-thank-you](skills/npo-donor-thank-you/SKILL.md) | Specific thank-you letters, emails, cards, or call scripts, with donor details as placeholders |
| [npo-appeal-letter](skills/npo-appeal-letter/SKILL.md) | A fundraising appeal with one clear ask and no invented urgency |
| [npo-event-plan](skills/npo-event-plan/SKILL.md) | An event plan with budget, task list, run-of-show, and safety and accessibility checks |
| [npo-volunteer-role](skills/npo-volunteer-role/SKILL.md) | A volunteer role description and recruitment post |
| [npo-volunteer-onboarding](skills/npo-volunteer-onboarding/SKILL.md) | A welcome message, onboarding guide, and first-week checklist |
| [npo-volunteer-schedule](skills/npo-volunteer-schedule/SKILL.md) | A shift grid with coverage gaps and reminder messages |

## Agents

An agent here is a short role file that names the skills it uses and the order to use them in. It adds no new instructions. Those live in the skills.

| Agent | Role |
| --- | --- |
| [npo-grants-agent](agents/npo-grants-agent.md) | From program facts to proposal, budget narrative, and progress report, pausing for your approval at each step |
| [npo-donor-relations-agent](agents/npo-donor-relations-agent.md) | Thank-yous, appeals, and impact updates for donors |
| [npo-volunteer-events-agent](agents/npo-volunteer-events-agent.md) | Event plans, volunteer roles, onboarding, schedules, and follow-up thank-yous |

You don't need the agents. Every skill works on its own.

## Examples

[examples/](examples/) has complete outputs produced by following the skills. Every organization, figure, and story in them is invented, and figures are marked as such.

- [Food bank: foundation grant](examples/food-bank-foundation-grant.md). A fact sheet, a fit check, proposal sections, and a budget narrative.
- [Youth reading program: year-end donors](examples/reading-program-donors.md). An impact update, a thank-you letter, and an appeal.
- [Park cleanup day: event and volunteers](examples/park-cleanup-volunteers.md). An event plan, a volunteer role, and a shift schedule with reminders.

## What the skills always do

Every skill ends with the same Guardrails section, and the validator fails if one is missing or different. The agent:

- uses only your figures, outcomes, quotes, and stories, with dates and sources, and marks gaps `[number from your records]`,
- follows the funder's guidelines, limits, and AI-use policy, and asks for them if it doesn't have them,
- works without donor, volunteer, or client personal details, and honors anonymity and contact preferences,
- uses only consented stories, told with dignity,
- drafts, and submits or sends nothing. Receipt and tax wording, budgets, and safeguarding steps go to someone qualified at your organization.

## Funder rules come first

Some funders restrict AI-assisted applications or ask you to disclose AI use. Check each funder's guidelines before you start. Nothing here is legal, tax, accounting, or fundraising-compliance advice.

## Privacy

Keep donor names, addresses, giving history, and volunteer and client details out of AI tools unless your organization has approved your tool and setup for that data. Write with placeholders and add details in your own CRM or mail tool. The skills tell the agent to remove details it sees, but by then the text has already reached the AI provider.

## Why Agent Skills

[docs/format.md](docs/format.md) explains the choice. In short, a skill is plain Markdown in a folder, several major coding agents already load the same folder layout, and anyone on your team can read and edit every instruction.

## Documentation

- [Install for your agent](docs/install.md)
- [Use the skills](docs/usage.md)
- [Write a new skill](docs/authoring.md)
- [Why this format](docs/format.md)
- [Contributing](CONTRIBUTING.md)

## License

[MIT](LICENSE).
