# Reminder Basics

**One reminder that comes back every day until you say it's done.**

This is a free Grok Bot skill / AI agent skill template. It is a `SKILL.md` instruction file you can paste into a Grok Bot or any similar assistant that supports standing instructions and a daily routine.

## Important

These instructions tell the bot how to remind and when to keep going. They are not a hard technical block. A bot can still miss a day, fire late, or misread a message. They lower the chance of a dropped to-do but don't guarantee a reminder will arrive on time, or at all, so test it before you rely on it for anything time-sensitive. Keep cards, wallets and payment logins out of any bot you don't fully trust, and use your platform's own approval and spending controls as the real safeguard. You're responsible for your own bot's actions and for the underlying to-do. This is provided as is, with no warranty.

## Who it's for

Anyone with one nagging task that keeps slipping: a renewal, a form, a call you keep putting off. Normal reminders fire once and get swiped away. This one keeps coming back.

## What's included

- A rule for what counts as "done" (and what doesn't, like "I'm working on it" or "thanks")
- A two-line daily reminder message
- A copy-paste bot description and a daily routine prompt

## What's not included (free version limits)

- One item only, not a list
- One daily time only, no other schedules
- No chat commands for editing, notes, pausing, or showing a list

Those are in the full [Nag-Until-Cleared Reminders](https://skillsforbots.gumroad.com/l/hdqoqb) pack.

## 5-minute setup

1. Open `SKILL.md` and fill in `[OWNER NAME]`, `[BOT NAME]`, `[ITEM]`, and `[LOCAL TIME]`.
2. Paste the bot description into your bot as standing instructions.
3. Create a daily routine at `[LOCAL TIME]` for that bot, using the daily routine prompt.
4. Reply "ok" to the first reminder. The next day's reminder should still come.
5. Reply "done." The reminders should stop.

## Example

Sam Ortiz sets a reminder for "book the dentist cleaning" at 9:00 every morning. On day one Sam replies "thanks, will do," and the bot keeps going. On day two Sam says "I called but they were closed," and the bot keeps going. On day three Sam books it and replies "done." The bot confirms in one line and stops.

## Limits and disclaimers

- This is a reminder template, not a task runner or an accountability service.
- Reminders depend on your platform's routine staying on. Turning the routine off stops reminders.
- The bot won't do the task, pay for anything, or send anything unless you ask.
- This doesn't offer medical, financial, or other professional advice about the underlying to-do.

The free skill in this folder is released under the [MIT License](../../LICENSE). The full Nag-Until-Cleared Reminders pack is sold separately on Gumroad under its own terms: https://skillsforbots.gumroad.com/l/hdqoqb
