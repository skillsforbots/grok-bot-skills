---
name: reminder-basics
description: >-
  Use this when the owner wants one simple reminder that repeats once a day
  and stays on until they clearly say it is done. Free, limited version: one
  item, one daily time, no lists or custom schedules.
---

# Reminder basics

Use this skill when the owner asks for a single reminder that should keep coming back until they finish it. The bot reminds once a day at a set time and does not stop just because a date passed, the owner said "ok," or the owner talked about the task. It stops only when the owner clearly says the item is done.

This is a free, limited skill. It handles **one reminder item** on **one fixed daily time**. It does not keep a list of several to-dos, offer other schedules, or include chat commands for editing, notes, or pausing. Those are in the full version (see the end of this file).

## Important

These instructions tell the bot how to remind and when to keep going. They are not a hard technical block. A bot can still miss a day, fire late, or misread a message. They lower the chance of a dropped to-do but don't guarantee a reminder will arrive on time, or at all, so test it before you rely on it for anything time-sensitive. Keep cards, wallets and payment logins out of any bot you don't fully trust, and use your platform's own approval and spending controls as the real safeguard. You're responsible for your own bot's actions and for the underlying to-do. This is provided as is, with no warranty.

## Customization placeholders

Fill these in before the first run. Do not invent a value.

- `[OWNER NAME]` — the person the reminder is for
- `[BOT NAME]` — the bot that sends the reminder
- `[ITEM]` — the one thing to be reminded about, in a few words (for example, "renew the car registration")
- `[LOCAL TIME]` — the time of day the reminder fires, in the owner's timezone

## The one rule: when the reminder stops

The reminder stops **only** when the owner clearly says the item is done or asks to stop it.

**Stops the reminder** (stop, then confirm in one line):

- "Done"
- "`[ITEM]` is done"
- "Clear it" or "Clear `[ITEM]`"
- "Stop reminding me about `[ITEM]`"

**Does not stop the reminder** (keep going, and do not argue):

- "I'm working on it" or "I started"
- "I'll do it tomorrow" or "later"
- "Thanks," "ok," "got it," or a thumbs-up
- Talking about the item or asking a question about it
- The bot thinking the task *looks* finished
- Silence after a reminder

If a reply is unclear, ask once: "Is `[ITEM]` done, or should I keep reminding you?" Then wait. Keep reminding unless the answer is a clear yes.

## When the reminder fires

1. If the item has been cleared, send nothing and stop.
2. Otherwise send one short message:

```
Reminder: [ITEM]

This comes back every day at [LOCAL TIME] until you tell me it's done. Reply "done" to stop it.
```

3. Stop. Do not do the task, add tips, or pile on pressure.

## What the bot does not do

- Do the task itself unless the owner explicitly asks in that message
- Stop the reminder by guessing, or because a date passed
- Add a second item. If the owner asks for another reminder, say this free version holds one item at a time; they can clear the current one first, or set up the full version for a list.
- Change the time on its own

## Copy-paste setup

### Bot description

Paste this into `[BOT NAME]` as standing instructions, after replacing every `[BRACKET]`:

```
You remind [OWNER NAME] about one thing: [ITEM].

Remind once a day at [LOCAL TIME]. Keep reminding until [OWNER NAME] clearly says it is done (for example "done," "clear it," or "stop reminding me about it").

These do not count as done: "I'm working on it," "later," "thanks," "ok," talking about it, or anything you only guess. If a reply is unclear, ask once whether it is done, then wait.

Do not do the task yourself unless asked. Keep each reminder to two lines.
```

### Daily routine prompt

Create a routine that runs every day at `[LOCAL TIME]`, assigned to `[BOT NAME]`, with this prompt:

```
If [ITEM] has not been cleared by [OWNER NAME], send:
"Reminder: [ITEM]. This comes back every day at [LOCAL TIME] until you tell me it's done. Reply "done" to stop it."
If it has been cleared, send nothing.
Do not do the task. Then stop.
```

When the owner says the item is done, confirm in one line and pause or delete the routine if your platform allows it, or simply send nothing on later runs.

## After setup

Read the item and time back to the owner and confirm the reminder will keep coming until they say "done." Then wait for the first run.

## Want more than one item?

This free skill covers one reminder. The full **Nag-Until-Cleared Reminders** pack keeps a whole list of to-dos on one reminder, lets you pick a schedule (every few days, weekly, every other week, or monthly), adds chat commands to add, edit, clear, pause, or show items, and includes a starter list prompt. It's here: https://skillsforbots.gumroad.com/l/hdqoqb
