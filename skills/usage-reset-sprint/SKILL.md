---
name: usage-reset-sprint
description: >-
  Use this when the owner wants to use remaining usage on a project
  right before a usage or token limit resets: check the reset time and
  remaining usage, pick the highest-value finishable chunk, save a
  progress handoff, wrap up cleanly, and resume after reset. Never buy
  extra credits or spend money to get more usage.
---

# Usage reset sprint

Use this skill when the owner wants to get the most useful work done on a project before a usage or token window resets. The bot checks remaining usage and the reset time, picks the highest-value chunk that can actually finish in that window, does that work, saves a progress handoff so nothing is lost, and stops cleanly. It does not spend leftover usage just to use it up, and it does not buy more.

## Important

These instructions tell the bot how to plan and wrap up work near a usage reset. They are not a hard technical block. A bot can still misread remaining usage, start a job that does not finish, or get cut off mid-reply. They lower the chance of losing mid-task work when a window ends, but don't guarantee the bot will see usage correctly, finish in time, or that a cutoff will leave files saved, so test them before you rely on them for anything time-sensitive. Keep cards, wallets and payment logins out of any bot you don't fully trust, and use your platform's own approval and spending controls as the real safeguard. You're responsible for your own bot's actions. This is provided as is, with no warranty.

## Purpose

Turn leftover usage into finished, saved progress on one project, then leave a clear handoff so the next session can resume after the reset. The owner stays in control: the bot does not spend money, buy credits, upgrade a plan, or send messages to get more usage, and it asks before doing anything outside the agreed plan.

## Customization placeholders

Fill these in before the first run. If a field does not apply, write `None`. Do not invent a value.

- `[OWNER NAME]` — the person who owns the bot
- `[BOT NAME]` — the bot these instructions are pasted into
- `[PROJECT]` — the project to sprint on, or `Ask` if the bot should ask each time
- `[RESET TIME]` — when the usage window resets, in the owner's timezone, or `Unknown` if the bot should look it up or ask
- `[APPROVAL CHANNEL]` — where the bot asks about anything outside the plan, and where the owner's instructions count. This can list more than one place (for example, this chat, the phone app, or a linked chat app).

## When to run a sprint

Start a sprint when the owner asks to use remaining usage, finish something before the reset, or wrap up a project because the window is ending. If the owner has already filled in `[RESET TIME]` and the reset is soon, the bot may offer a sprint, then wait for a yes. Do not start a sprint on your own, and do not invent urgency.

## How the sprint works

1. **Check remaining usage and the reset time.** Use the platform's usage page, settings, or status view if you can see it. If `[RESET TIME]` is already filled in, use that time and still check remaining usage. If you cannot see a number or a time, ask [OWNER NAME] in [APPROVAL CHANNEL]. Do not guess. Do not open a checkout, upgrade, or buy-credits page to find the answer.
2. **Name the project.** Use `[PROJECT]` if it is filled in with a real project. If it is `Ask` or `None`, ask which project to focus on. Stay on that project for the sprint unless the owner changes it.
3. **List leftover work** in a short list: what is already done, what is left, and which leftovers can finish in the remaining window, with a buffer so the wrap-up still fits.
4. **Pick the highest-value finishable chunk.** Prefer work that can be completed and saved before reset, leaves a usable artifact (a finished draft, a saved file, a written decision, or a handoff), and unblocks the next session. Do not start a large rewrite, a wide research sweep, or a multi-file job that will not finish. If nothing can finish, spend the remaining usage saving current work and writing a thorough handoff, then stop. If remaining usage is too small even for that, write the shortest honest handoff you can and stop.
5. **Show the plan and wait for a short yes**, unless the owner already said to use the rest of the window on this project and the plan stays inside that request. If the plan would send a message, spend money, buy credits, upgrade a plan, switch projects, or do anything else outside the plan, stop and ask first in `[APPROVAL CHANNEL]`.
6. **Do that chunk only.** Save as you go: write files, keep drafts in the chat, and do not leave the only copy inside an unsaved reply. Watch the remaining window. When usage is running low or the reset is close, stop starting new work.
7. **Wrap up cleanly.** Finish the current sentence or file if you can, write the progress handoff below, tell [OWNER NAME] what was finished and what will wait, and stop. Leave a little usage for this wrap-up; do not spend the last of the window mid-thought.
8. **After the reset:** Do not automatically start a new big job. Show the handoff, confirm what is left, and wait for the owner to say to resume, unless they already asked to continue after reset as part of this sprint. Then pick up from the handoff instead of starting over.

## Progress handoff

Use this block at the end of every sprint, even if the chunk finished cleanly. Copy it and fill every field. Do not skip fields; use `None` if a field does not apply. Do not invent files, progress, usage figures, or a reset time.

```
USAGE RESET HANDOFF
From: [BOT NAME]
To: [OWNER NAME] (next session)
Project: [PROJECT]

Reset time: [time in the owner's timezone, or Unknown]
Remaining usage when this was written: [what was visible, or Unknown]
Done this sprint: [what was finished and where it is saved]
What's left: [next highest-value work, in order]
Open files / drafts: [paths or links, or None]
Do not restart: [anything that should not be redone, or None]
Needs owner approval: [yes/no — if yes, say exactly what]
Resume prompt: [one short sentence the owner can paste after reset]
```

## Copy-paste setup prompts

The owner pastes these into the bot when creating or editing it. Replace every `[BRACKET]` first.

### Bot description

```
You are [BOT NAME], a bot for [OWNER NAME].

When [OWNER NAME] wants to use remaining usage on [PROJECT] before a usage or token window resets:
- Check remaining usage and the reset time ([RESET TIME], or look it up / ask if Unknown). Do not guess. Do not open a checkout or upgrade page to find it.
- Pick the highest-value chunk of [PROJECT] that can actually finish and be saved before reset, with a buffer for wrap-up. Do not start a big job that will not finish. Do not spend leftover usage just to use it up.
- Show the plan in [APPROVAL CHANNEL] and wait for a short yes, unless they already asked to use the rest of the window on this project and the plan stays inside that request.
- Do that chunk only, save as you go, then write a usage-reset handoff (done this sprint, what's left, where files are, what not to restart, and a short resume prompt) and stop.
- After reset, show the handoff and wait to be told to resume, unless they already asked to continue after reset. Then pick up from the handoff; do not start over.

Never buy credits, upgrade a plan, spend money, or send email or messages to get more usage. If a step would send, spend, or go outside the agreed plan, stop, ask in [APPROVAL CHANNEL], and wait. A one-time yes is for that item only.
```

### Start-sprint prompt (paste when the window is almost over)

```
We're close to the usage reset. Check remaining usage and the reset time, then propose the highest-value chunk of [PROJECT] that can finish before reset. Don't buy more usage or start a job that won't finish. Wait for my yes, then do that chunk, save the work, leave a handoff, and stop.
```

### Handoff note (blank, for quick copy)

```
USAGE RESET HANDOFF
From: [BOT NAME]
To: [OWNER NAME] (next session)
Project: [PROJECT]

Reset time:
Remaining usage when this was written:
Done this sprint:
What's left:
Open files / drafts:
Do not restart:
Needs owner approval:
Resume prompt:
```

## After setup

Read back `[PROJECT]`, `[RESET TIME]`, and `[APPROVAL CHANNEL]`. Confirm that you will not buy credits, spend money, or send messages to get more usage. Then wait for the owner to start a sprint.

## Never

- Spend money, buy extra credits or tokens, start a paid trial, or upgrade a plan to get more usage
- Send an email, chat message, text, or post to request more usage, or as part of wrapping up, unless the owner has approved that specific send
- Invent remaining usage, a reset time, or progress that was not actually saved
- Start a job that clearly cannot finish before reset
- Spend leftover usage just to use it up
- Treat "use the rest of my usage" as permission to send, spend, change plans, or start a different project
- Skip handoff fields, or leave the only copy of the work inside an unsaved reply
