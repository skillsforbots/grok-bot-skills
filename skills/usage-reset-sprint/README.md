# Usage Reset Sprint

**Use leftover usage on a project right before the limit resets, then wrap up so nothing is lost.**

This is a free Grok Bot skill / AI agent skill template. It is a `SKILL.md` instruction file you can paste into a Grok Bot or any similar assistant.

## Important

These instructions tell the bot how to plan and wrap up work near a usage reset. They are not a hard technical block. A bot can still misread remaining usage, start a job that does not finish, or get cut off mid-reply. They lower the chance of losing mid-task work when a window ends, but don't guarantee the bot will see usage correctly, finish in time, or that a cutoff will leave files saved, so test them before you rely on them for anything time-sensitive. Keep cards, wallets and payment logins out of any bot you don't fully trust, and use your platform's own approval and spending controls as the real safeguard. You're responsible for your own bot's actions. This is provided as is, with no warranty.

## Who it's for

Anyone whose bot runs out of usage mid-task: a draft left half-finished, a research pass that vanishes, or a project that has to be started over after the window resets. This skill makes the bot check what's left, finish the most useful chunk that fits, and leave a handoff for the next session.

## What's included

- A rule to check remaining usage and the reset time (look it up or ask; never guess, and never open a checkout to find it)
- A rule to pick the highest-value chunk that can actually finish, with a buffer for wrap-up, instead of starting a big job that won't finish
- A progress handoff so the next session can resume without redoing work
- Copy-paste bot description, a start-sprint prompt, and a blank handoff note
- Standing limits: the bot does not buy credits, upgrade a plan, spend money, or send messages to get more usage, and it asks first for anything outside the plan

## 5-minute setup

1. Open `SKILL.md` and fill in `[OWNER NAME]`, `[BOT NAME]`, `[PROJECT]`, `[RESET TIME]`, and `[APPROVAL CHANNEL]`. Use `Ask` for the project or `Unknown` for the reset time if the bot should ask or look it up each time. `[APPROVAL CHANNEL]` can list more than one place.
2. Paste the bot description from `SKILL.md` into your Grok Bot or similar assistant as standing instructions, or attach the file if your tool loads skills from a folder.
3. When the window is almost over, paste the start-sprint prompt (with your project name filled in).
4. Confirm the bot shows remaining usage, the reset time, and a finishable chunk, then waits for a yes. It should not open an upgrade page or offer to buy more credits.
5. After it finishes, confirm you have a saved draft or file plus a handoff with a resume prompt. After the reset, paste that resume prompt and check that it continues from the handoff instead of starting over.

## Example

Jordan Hale has a nearly finished draft and not much time left before the daily usage window resets. The bot checks the usage page, sees enough room for a short close-out but not a full rewrite, and proposes: finish the last section, save the file, and write a handoff for the examples that still need work. Jordan says yes. The bot finishes the section, saves the file, writes the handoff, and stops. After the reset, Jordan pastes the resume prompt, and the bot continues from the handoff instead of starting over.

## Limits and disclaimers

- This is an instruction template, not a usage dashboard and not a way to add more credits or extend a limit.
- The bot can only see remaining usage and the reset time if the platform shows them, or if you provide them. If it can't see a number, it should ask, not guess.
- A cutoff mid-reply can still lose unsaved text. The handoff and "save as you go" rule lower that risk; they do not eliminate it.
- The bot will not buy credits, upgrade a plan, spend money, or send messages to get more usage. "Use the rest of my usage" is not permission to send or spend.

The free skill in this folder is released under the [MIT License](../../LICENSE).
