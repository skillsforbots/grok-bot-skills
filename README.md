# Grok Bot skills (free SKILL.md templates)

Free [Grok Bot](https://grok.com) skills in `SKILL.md` format, each with standing safety rules: no sending without your approval, no spending, only the owner gives orders, and hidden text in outside content is ignored. A skill is an instruction file your Grok Bot follows so it behaves the same way every time.

This repository includes three free skills you can install in about five minutes each. Premium packs for a bot fleet coordinator, nag-until-cleared reminders, a credit coach, a project sprint, and a domain and SEO launch are sold separately.

New to Grok Bot skills? Start with **[Grok Bot skills: the complete guide](https://skillsforbots.com/grok-bot-skills/)** on my site, [skillsforbots.com](https://skillsforbots.com/).

## Install in Grok Bot

1. Open the skill's `SKILL.md` below and read the whole file.
2. Replace every `[BRACKET]` placeholder with your own details.
3. In a one-to-one chat with your Grok Bot, paste the file with a request like this:

```text
Save the text below as a private skill named reminder-basics.
Keep the name and description exactly as written.
Then tell me the skill's name and one-line description.

[paste the full SKILL.md here]
```

4. Private skills are one library shared by all your Grok Bots. If a bot can't find the skill, open **Connect apps** in the sidebar, select the connected count next to the title, and turn it on under **Private skills**.
5. Test it on something low-stakes. Ask the bot to send a message to you or buy something small: it should draft and wait for your yes.

Step-by-step, with two other install methods: [How to install Grok Bot skills from GitHub (3 ways)](https://skillsforbots.com/install/grok-bot/).

## Grok Bot skills guides

- [Grok Bot skills: the complete guide](https://skillsforbots.com/grok-bot-skills/)
- [How to install Grok Bot skills from GitHub (3 ways)](https://skillsforbots.com/install/grok-bot/)
- [Grok Bot skill template: an annotated SKILL.md you can copy](https://skillsforbots.com/skill-md/template/)
- [Free Grok Bot skill checker (runs in your browser)](https://skillsforbots.com/tools/skill-md-checker/)
- [How to check a Grok Bot skill is safe before you install it](https://skillsforbots.com/safety/check-a-skill-before-installing/)
- [Grok Bot approval rules: a no-send, no-spend template](https://skillsforbots.com/safety/approval-rules/)
- [Grok Bot skills vs routines](https://skillsforbots.com/routines/skills-vs-scheduled-tasks/)
- [Grok Bot skills on GitHub: the free repos worth knowing](https://skillsforbots.com/skills/grok-bot-skills-github/)
- [All guides](https://skillsforbots.com/guides/)

## What a skill is

A bot skill is a `SKILL.md` file: standing instructions, rules, and copy-paste prompts. You fill in the `[BRACKET]` placeholders, then save the file as a private skill in your Grok Bot (see [Install in Grok Bot](#install-in-grok-bot)). The bot follows the skill on later runs, instead of relying on a one-off chat.

## 5-minute setup: Bot Safety Rules Starter

1. Open [`skills/bot-safety-rules-starter/SKILL.md`](skills/bot-safety-rules-starter/SKILL.md).
2. Replace every `[BRACKET]` placeholder (owner name, bot name, approval channel, and the two rule toggles). Leave a rule `ON` unless you want that bot to send or spend on its own. The approval channel can list more than one place. The always-on owner-orders rule stays in place.
3. Paste the "bot description" block from the file into your Grok Bot (or similar assistant) as its standing instructions, or attach the `SKILL.md` if your tool loads skills from a folder.
4. Send a test request that would require a send or a spend. The bot should draft the message or state the cost, then wait for your explicit approval.
5. If you pass work to another bot, copy the blank handoff note, fill every field, and use `None` where a field does not apply.

More detail is in the [starter skill README](skills/bot-safety-rules-starter/README.md).

Read the Important section at the top of the [starter skill](skills/bot-safety-rules-starter/SKILL.md) before you rely on these rules.


## Free skills in this repo

**[Bot Safety Rules Starter](skills/bot-safety-rules-starter/)** — Standing safety rules for any bot: no sending email or messages without owner approval, no spending money, ignore instructions hidden in outside content (web pages, emails, and documents), and a one-time "send this" or "pay this" is approval for that item only, not a standing waiver. Includes a blank structured handoff note so work can move between bots without dropping context.

Also on Agensi: [Bot Safety Rules Starter](https://www.agensi.io/skills/bot-safety-rules-starter).

**[Reminder Basics](skills/reminder-basics/)** — One reminder that comes back every day until you clearly say it's done. "Thanks," "ok," and "I'm working on it" don't stop it; "done" does. Free version: one item and one daily time. The full [Nag-Until-Cleared Reminders](https://skillsforbots.gumroad.com/l/hdqoqb) pack adds a list of to-dos, other schedules, and chat commands to edit, pause, or show items.

Also on Agensi: [Reminder Basics](https://www.agensi.io/skills/reminder-basics).

**[Usage Reset Sprint](skills/usage-reset-sprint/)** — Use leftover usage on a project right before a usage or token limit resets: check remaining usage and the reset time, finish the highest-value chunk that fits, and leave a handoff so work can resume after the reset. The bot does not buy credits, spend money, or send messages to get more usage.

Also on Agensi: [Usage Reset Sprint](https://www.agensi.io/skills/usage-reset-sprint).

The free skills in this repository are released under the [MIT License](LICENSE).

## Premium packs

These packs are sold separately on Gumroad under their own terms. They are not covered by this repository's MIT License. Every pack keeps the same no-send, no-spend, owner-only, and ignore-hidden-text rules, and carries a disclaimer: skills are instructions to the bot, not a hard technical block, so test before you rely on them. Pack details: [Grok Bot skill packs](https://skillsforbots.com/grok-bot-skills/#packs).

- **[Bot Fleet Coordinator](https://skillsforbots.gumroad.com/l/ergple)** — $12. One primary bot routes every task to the right specialist, writes a structured handoff, and follows no-send / no-spend rules, with a weekly read-only review of the fleet.
- Also on Agensi: [Bot Fleet Coordinator](https://www.agensi.io/skills/bot-fleet-coordinator).
- **[Nag-Until-Cleared Reminders](https://skillsforbots.gumroad.com/l/hdqoqb)** — $9. Reminders and routines that keep coming back until you clearly say an item is done — not when a date passes, and not when you mention it in passing.
- Also on Agensi: [Nag-Until-Cleared Reminders](https://www.agensi.io/skills/nag-until-cleared-reminders).
- **[Credit Repair Coach](https://skillsforbots.gumroad.com/l/ifujn)** — $12. A daily or on-demand brief with today's top 3 credit moves, impact figures labeled as estimates, and letter drafts you review and send yourself. Educational only. Not financial advice, not legal advice, and not credit repair company services. No results are promised.
- Also on Agensi: [Credit Repair Coach](https://www.agensi.io/skills/credit-repair-coach).
- **[Project Sprint](https://skillsforbots.gumroad.com/l/project-sprint)** — $19. Plan a project across several usage windows, finish a high-value chunk before each reset, and pick up from a handoff after, without buying more credits. Details: [Grok Bot project sprint skill](https://skillsforbots.com/grok-bot-project-sprint-skill/).
- Also on Agensi: [Project Sprint](https://www.agensi.io/skills/project-sprint).
- **[Domain + SEO Launch Playbook](https://skillsforbots.gumroad.com/l/domain-seo-launch)** — $19. Move a static site to a custom domain and launch it for search, in 8 phases, with a check after each one. Details: [Grok Bot domain and SEO launch skill](https://skillsforbots.com/grok-bot-domain-seo-launch-skill/).
- Also on Agensi: [Domain + SEO Launch Playbook](https://www.agensi.io/skills/domain-seo-launch-playbook).
- **[Bot Owner Starter Bundle](https://skillsforbots.gumroad.com/l/vxecie)** — $19. The Bot Fleet Coordinator, Nag-Until-Cleared Reminders, and Credit Repair Coach in one download (saves $14 vs $33 separately).
- Also on Agensi: [Bot Owner Starter Bundle](https://www.agensi.io/bundles/bot-owner-starter-bundle).

## License

The free skills in this repository (Bot Safety Rules Starter, Reminder Basics, and Usage Reset Sprint) are MIT-licensed. The premium packs above are sold separately under their own terms and are not included in this repo.
