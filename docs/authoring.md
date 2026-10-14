# Write a new skill

A skill is a folder with a `SKILL.md` file. This page explains how to add one that passes the validator and fits the kit.

## Decide whether it should be a skill

Add a skill when nonprofit staff and volunteers need a distinct document or procedure the current skills don't produce. If the request is a variation of an existing skill ("a grant proposal for a foundation with a two-page limit"), improve that skill instead. Fewer, better skills are easier for the agent to choose between.

## Create the folder

```bash
mkdir skills/npo-board-report
```

The folder name is the skill name. It must start with `npo-` and use only lowercase letters, digits, and single hyphens, at most 64 characters. The prefix keeps our skills from replacing your own skills with the same name when both sit in a shared folder. Agent file names in `agents/` start with `npo-` for the same reason.

## Write the frontmatter

`SKILL.md` must start on line 1 with YAML frontmatter:

```markdown
---
name: npo-board-report
description: "Drafts a short board report from the organization's real program and finance figures: highlights, risks, and decisions needed. Use when staff ask for a board report, a board update, or an executive director's report."
license: MIT
---
```

- `name` must match the folder name.
- Put `description` in double quotes. Descriptions often contain a colon, and an unquoted colon makes the YAML invalid, so agents load the skill without its description.
- `description` must be 50 to 1,024 characters. Say what the skill makes, then "Use when" with the words a nonprofit would type. The agent picks skills by this text alone.

Use only the fields from the [Agent Skills specification](https://agentskills.io/specification). Tool-specific fields work in one agent and are ignored or rejected in another.

## Write the body

Follow the shape of the existing skills:

1. A one-line purpose.
2. **Ask first.** The 3 to 5 inputs the skill needs. The agent asks only for missing ones.
3. **Steps**, as numbered commands.
4. **Output.** The exact sections and order of the result, ending with what the user must check.
5. **Guardrails.** Copy the section from any existing skill, word for word. The validator fails if it is missing or different.

Keep `SKILL.md` under 500 lines. If you need long reference material, put it in a `references/` folder inside the skill and link it with a relative path. Keep links one level deep.

To point at another skill, write its name in backticks followed by "skill": "use the `npo-grant-proposal` skill". Don't link to another skill's file. People can install one skill without the others, and a link would break. The validator checks that every name written this way exists.

## Write for nonprofit staff and volunteers and for the agent

- Plain English, short sentences, no jargon.
- Write instructions the agent can follow without guessing: "Write two reply options", not "write some options".
- Never ask the agent to supply numbers, outcomes, stories, funder rules, or legal and tax wording from memory. Ask the user for them, or write a placeholder.
- Don't claim research findings or legal rules without a source.
- No em dashes. The validator rejects them.

## Add an example

Produce a real output by following your skill for one invented organization, and add it to `examples/`. Every name, figure, and story in it must be invented, and the file must say so. If you can't produce a good example by following the instructions, the instructions need work.

## Check it

```bash
npm run validate
npm test
```

Both run in CI on every pull request.
