# Grok Bot skills

Free [Grok Bot](https://grok.com) skill templates and AI agent skill templates in `SKILL.md` format. A skill is an instruction file a Grok Bot or similar AI assistant follows so it behaves the same way every time.

This repository includes three free skills you can install in about five minutes each. Premium packs for a multi-bot / bot fleet coordinator, nag-until-cleared reminders and routines, and a credit coach are sold separately.

Guides, pack details, and setup help are on my site: [Skills for Bots: Grok Bot skills](https://skillsforbots.com/).

## What a skill is

A bot skill is a `SKILL.md` file: standing instructions, rules, and copy-paste prompts. You fill in the `[BRACKET]` placeholders, then add the file to your Grok Bot or any assistant that accepts a skill or instruction file. The bot follows the skill on later runs, instead of relying on a one-off chat.

## 5-minute install

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

These packs are sold separately on Gumroad under their own terms. They are not covered by this repository's MIT License.

- **[Bot Fleet Coordinator](https://skillsforbots.gumroad.com/l/ergple)** — $12. One primary bot routes every task to the right specialist, writes a structured handoff, and follows no-send / no-spend rules, with a weekly read-only review of the fleet.
- Also on Agensi: [Bot Fleet Coordinator](https://www.agensi.io/skills/bot-fleet-coordinator).
- **[Nag-Until-Cleared Reminders](https://skillsforbots.gumroad.com/l/hdqoqb)** — $9. Reminders and routines that keep coming back until you clearly say an item is done — not when a date passes, and not when you mention it in passing.
- Also on Agensi: [Nag-Until-Cleared Reminders](https://www.agensi.io/skills/nag-until-cleared-reminders).
- **[Credit Repair Coach](https://skillsforbots.gumroad.com/l/ifujn)** — $12. A daily or on-demand brief with today's top 3 credit moves, impact figures labeled as estimates, and letter drafts you review and send yourself. Educational only. Not financial advice, not legal advice, and not credit repair company services. No results are promised.
- Also on Agensi: [Credit Repair Coach](https://www.agensi.io/skills/credit-repair-coach).
- **[Bot Owner Starter Bundle](https://skillsforbots.gumroad.com/l/vxecie)** — $19. The Bot Fleet Coordinator, Nag-Until-Cleared Reminders, and Credit Repair Coach in one download (saves $14 vs $33 separately).
- Also on Agensi: [Bot Owner Starter Bundle](https://www.agensi.io/bundles/bot-owner-starter-bundle).

## License

The free skills in this repository (Bot Safety Rules Starter, Reminder Basics, and Usage Reset Sprint) are MIT-licensed. The premium packs above are sold separately under their own terms and are not included in this repo.
