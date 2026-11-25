---
name: ghostlyn
description:
  Use when the user asks about the company, its people, customers, projects,
  decisions or internal processes, when the work needs one of the team's skills,
  tools or connected accounts, or when the conversation settles a fact the team
  should keep. Reaches the team's shared knowledge and agent in Ghostlyn.
---

# Ghostlyn

Ghostlyn holds this team's shared knowledge and runs the team's agent, with its
skills, connected accounts, tasks and schedules. Claude does not see any of it
unless it asks.

## Look things up

For a question about the company, its people, customers, projects, decisions or
internal processes, call `lookup` first and then `read` the files it points to.
Answer from what you read and cite the `volume:path` of each file you used. When
`lookup` finds nothing, say so rather than guessing.

## Hand work to the agent

When the work needs one of the team's skills, tools or connected accounts, or a
task or schedule, call `invoke`. The `invoke` description names the skills the
team has. Pass the whole request in `message`, since Ghostlyn does not see this
conversation. Keep the `chatId` from the reply to continue the same
conversation, and cite the files the reply lists.

## Offer to save

When the conversation settles a fact that Ghostlyn lacks or gets wrong, offer to
save it and wait for the user to agree. Then send it through `invoke`, so it
lands where the team files it. Make no save without the user's yes.

## Leave general questions alone

Never call Ghostlyn for general knowledge, such as a definition, a public fact
or help with code that has nothing to do with the team. Answer those directly.
