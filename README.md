# Grok Bot skills

Free [Grok Bot](https://grok.com) skill templates and AI agent skill templates in `SKILL.md` format. A skill is an instruction file a Grok Bot or similar AI assistant follows so it behaves the same way every time.

This repository includes one free starter skill you can install in about five minutes. Premium packs for a multi-bot / bot fleet coordinator, nag-until-cleared reminders and routines, and a credit coach are sold separately.

## What a skill is

A bot skill is a `SKILL.md` file: standing instructions, rules, and copy-paste prompts. You fill in the `[BRACKET]` placeholders, then add the file to your Grok Bot or any assistant that accepts a skill or instruction file. The bot follows the skill on later runs, instead of relying on a one-off chat.

## 5-minute install

1. Open [`skills/bot-safety-rules-starter/SKILL.md`](skills/bot-safety-rules-starter/SKILL.md).
2. Replace every `[BRACKET]` placeholder (owner name, bot name, approval channel, and the two rule toggles). Leave a rule `ON` unless you want that bot to send or spend on its own.
3. Paste the "bot description" block from the file into your Grok Bot (or similar assistant) as its standing instructions, or attach the `SKILL.md` if your tool loads skills from a folder.
4. Send a test request that would require a send or a spend. The bot should draft the message or state the cost, then wait for your explicit approval.
5. If you pass work to another bot, copy the blank handoff note, fill every field, and use `None` where a field does not apply.

More detail is in the [starter skill README](skills/bot-safety-rules-starter/README.md).

Read the Important section at the top of the [starter skill](skills/bot-safety-rules-starter/SKILL.md) before you rely on these rules.


## Free skill in this repo

**[Bot Safety Rules Starter](skills/bot-safety-rules-starter/)** — Standing safety rules for any bot: no sending email or messages without owner approval, no spending money, and a one-time "send this" or "pay this" is approval for that item only, not a standing waiver. Includes a blank structured handoff note so work can move between bots without dropping context.

The free skill in this repository is released under the [MIT License](LICENSE).

## Premium packs

These packs are sold separately on Gumroad under their own terms. They are not covered by this repository's MIT License.

- **[Bot Fleet Coordinator](https://skillsforbots.gumroad.com/l/ergple)** — $19. One primary bot routes every task to the right specialist, writes a structured handoff, and follows no-send / no-spend rules, with a weekly read-only review of the fleet.
- **[Nag-Until-Cleared Reminders](https://skillsforbots.gumroad.com/l/hdqoqb)** — $17. Reminders and routines that keep coming back until you clearly say an item is done — not when a date passes, and not when you mention it in passing.
- **[Credit Repair Coach](https://skillsforbots.gumroad.com/l/ifujn)** — $24. A daily or on-demand brief with today's top 3 credit moves, impact figures labeled as estimates, and letter drafts you review and send yourself. Educational only. Not financial advice, not legal advice, and not credit repair company services. No results are promised.
- **[Bot Owner Starter Bundle](https://skillsforbots.gumroad.com/l/vxecie)** — $39. All three packs together.

## License

The free Bot Safety Rules Starter skill in this repository is MIT-licensed. The premium packs above are sold separately under their own terms and are not included in this repo.
