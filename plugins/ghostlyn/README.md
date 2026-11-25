# Ghostlyn

Ghostlyn is a shared agent for your team. It holds the team's knowledge, such as
wiki pages, notes and documents, and runs the team's skills, connected accounts,
tasks and schedules.

This plugin connects Claude to Ghostlyn and adds a skill that tells Claude when
to ask it. Without the skill, Claude has the connector but mostly uses it when
you mention Ghostlyn by name.

## Use it

1. Add the plugin, then connect Ghostlyn under Connectors on its page. In Claude
   Code, run `/plugin install ghostlyn --marketplace ghostlynhq/claude-plugin`.
2. Sign in with your Ghostlyn account and approve the permissions it asks for.
3. Ask Claude about your company, its customers or its decisions, with no
   mention of Ghostlyn. Claude searches your team's knowledge and cites the
   files it read.

Claude hands work to the Ghostlyn agent when it needs one of your team's skills
or connected accounts. It offers to save a fact the conversation settled and
saves only after you agree.

## What it sends

Claude sends Ghostlyn the search terms and the requests it passes on, and the
text of anything you agree to save. Ghostlyn returns the matching files and the
agent's reply. Nothing is sent about a conversation that never touches your
team. Each call runs as you, with the permissions your Ghostlyn account has.

Learn more at https://www.ghostlyn.com and read the privacy policy at
https://www.ghostlyn.com/privacy.
