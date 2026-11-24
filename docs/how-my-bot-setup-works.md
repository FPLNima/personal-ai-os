# How my bot setup works

This is a public, high-level description of a personal AI setup. It covers the shape of the system, not any private contents.

You can take this document and feed it to your own agent (for example Grok Bot, or any similar system) as a starting point for setting up your own team of agents.

## The idea

Use a small team of specialist agents, with one chief-of-staff agent that coordinates the rest. Shared context lives in Notion, following [Notion's official agent setup guide](https://developers.notion.com/prompts/setup). Other systems stay the source of truth for their own records. Agents can read those systems. They do not replace them.

## The team

These run in Grok Bot, but the same pattern can be set up in another agent system:

- Bob is my chief of staff, for daily coordination, drafts, and follow-through
- A solutions engineering coach
- A content strategist, for content planning
- A builder, for coding and shipping personal tools
- A travel planner and concierge bot
- A finance bot
- A fitness bot
- A language coach

Add or drop specialists to match the work you actually have.

## Shared context in Notion

Notion is the shared context layer that these agents can check, so each one does not have to be retrained from scratch.

The setup follows Notion's official guide:

- **Agent Operating Guide**: the first page an agent reads. It says where things live and how to work.
- **Memories**: lasting facts the agents should remember.
- **Skills**: reusable ways of working, saved as Notion Skills.
- **Documents**: where finished write-ups go.

The guide can improve over time as useful memories, skills, and finished work are saved back into Notion. Personal material stays out unless you explicitly include it.

## Sources of truth

- Attio is the source of truth for my personal CRM.
- Notion is the source of truth for shared agent context, not for CRM records.

Keep personal data out of public Git repositories. This repo stays at the level of setup and examples.

## Working rules

- Default permission is read-only.
- External messages are drafted first, then approved before anything is sent or published.
- Public changes are shown as a preview or diff before they go out.
- Agents should not invent data, and should leave out anything they have not checked.

## Status

This is a living personal setup, not a product. The write-up will drift, and it should be updated when the setup changes in a lasting way.
