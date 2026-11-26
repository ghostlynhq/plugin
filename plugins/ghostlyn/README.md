# Ghostlyn

Ghostlyn is a shared agent for your team. It holds the team's knowledge, such as
wiki pages, notes and documents, and runs the team's skills and connected
accounts.

This plugin connects Claude to Ghostlyn and adds a skill that tells Claude when
to ask it and where the team keeps things. Without the skill, Claude has the
connector but mostly uses it when you mention Ghostlyn by name.

## Use it

1. Add the plugin, then connect Ghostlyn under Connectors on its page. In Claude
   Code, run `/plugin install ghostlyn --marketplace ghostlynhq/claude-plugin`.
2. Sign in with your Ghostlyn account and approve the permissions it asks for.
3. Ask Claude about your company, its customers or its decisions, with no
   mention of Ghostlyn. Claude searches your team's knowledge and cites the
   files it read.

Claude reads where your team keeps things before it files or saves. When you ask
it to record something, or say others should know it, Claude saves it in the
project that fits and tells you where it went and who can see it. When you only
state a fact, it offers first. A private note or preference you ask it to keep
goes in your Home project, which stays private unless you share it. Claude hands
work to the Ghostlyn agent when it needs one of your team's skills or connected
accounts.

## What it sends

Claude sends Ghostlyn the search terms and the requests it passes on, and the
text of anything it saves. Ghostlyn returns the matching files, the agent's
reply and a description of where your team keeps things: your organization's
name, your name and each project you can open, with its name, description, who
can see it and whether you can change it. It lists a project's skills and tables
too. It adds the AGENTS.md of your Home and company projects, with the files
they import, which hold what your members wrote about how they work. Nothing is
sent about a conversation that never touches your team. Each call runs as you,
with the permissions your Ghostlyn account has.

Learn more at https://www.ghostlyn.com and read the privacy policy at
https://www.ghostlyn.com/privacy.
