# publora-post-ideas

An Agent Skill that offers you three different angles for a social post, then
writes the one you pick.

## Why I made this

Someone told me they stay with their scheduling tool mostly because of its post
templates. When they run out of ideas, the templates give them a way back in.
That stuck with me. It is not the part of the job I would have guessed people
get stuck on.

Asking an agent to "write me a post" has the same problem from the other side.
You get one draft, produced on the first guess. You read it, you are not
convinced, and there is nothing specific to push back on, so you rewrite it
yourself and the agent saved you nothing.

This changes the first move. The skill looks at what you have already published,
offers three angles from three different categories, and asks which one. Then it
asks for the one thing only you have: the mistake, the number, the name. Then it
writes from that.

## What is in it

- `SKILL.md`: how the agent chooses angles, what it has to ask before drafting,
  and what it is never allowed to invent.
- `references/angles.md`: 40 angles across 8 categories: Story, Behind the
  scenes, Tip, Case study, List, How-to, Opinion, Question. Each one names the
  specific fact that has to come from you.

## Install

Copy the folder into your skills directory:

```bash
git clone https://github.com/publora-team/publora-post-ideas.git \
  ~/.claude/skills/publora-post-ideas
```

Or install it as a plugin:

```
/plugin marketplace add publora-team/publora-claude-plugin
/plugin install publora-post-ideas@publora
```

The `SKILL.md` format is the open Agent Skills standard, so it also works in
Codex CLI, Cursor, Gemini CLI and Copilot.

## With Publora connected

It works on its own. The angle library is a text file and the draft comes back
as text you can paste anywhere.

Connected to [Publora](https://publora.com), it also reads what you have
actually published, so the angles are chosen against your real feed instead of
in the abstract, the rotation is real rather than guessed, and the finished post
goes into a queue instead of your clipboard. Publora's Starter plan is free
forever and includes the API and MCP access this uses.

## The one rule

An angle is only a way in. Every one of them asks for something only you can
supply, and the skill is told, more than once, never to make that part up. A
post with an invented failure in it reads plausible, is false, and goes out
under your own name.

## License

MIT
