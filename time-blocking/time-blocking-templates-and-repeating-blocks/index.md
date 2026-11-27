# Time Blocking Templates and Repeating Blocks

> A table of reusable time block templates with lengths, and how daily, weekday and custom repeats work in the Time Blocking Android app.

- Web: https://apps.schimpf.es/time-blocking/time-blocking-templates-and-repeating-blocks/
- App: Time Blocking: Day Planner, https://apps.schimpf.es/time-blocking/index.md
## Why reuse blocks

Most days contain the same blocks: a planning slot, lunch, a daily review. Typing them again each day takes longer than the planning itself. Two features cover this: templates for blocks you add by hand, and repeating blocks for blocks that return on a schedule.

This page lists template ideas with lengths and shows how each repeat option works in Time Blocking.

## Template ideas with lengths

A template in the app holds a name, a duration and a color. It has no start time, so you choose the time when you add it.

| Template | Length | Weekly total if used once per weekday |
|---|---|---|
| Plan the day | 15m | 1h 15m |
| Deep work | 2h | 10h |
| Email | 30m | 2h 30m |
| Lunch | 1h | 5h |
| Calls | 45m | 3h 45m |
| Review and shutdown | 15m | 1h 15m |
| Workout | 1h | 5h |

The weekly total is the length times 5. For example, 45 minutes times 5 is 225 minutes, or 3h 45m.

Use one color per kind of work. The palette has 12 colors: indigo, blue, cyan, teal, green, lime, amber, orange, coral, red, pink and purple.

## Create and use a template

1. Open the Templates screen to create, edit or delete templates. Deleting asks you to confirm.
2. Or edit a block you already placed and save it as a template.
3. When you add a block and at least one template exists, a picker offers Block (blank) or one of your templates.
4. Pick a template, then set the start time.

The app stores the duration, so a 45 minute Calls template always creates a 45 minute block.

## Repeating blocks

A block can repeat. The Repeat field has four choices:

- **Never**: a single block.
- **Daily**: every day from the start date.
- **Weekdays**: Monday to Friday.
- **Custom**: the weekdays you tick, for example Monday, Wednesday and Friday.

You can add an end date. The block appears on every matching day from its start date up to and including the end date.

### Worked example

A "Plan the day" block of 15 minutes at 08:00, repeating on weekdays, starting on a Monday with an end date on the Friday of the following week, appears on 10 days (two Monday to Friday weeks). That is 10 times 15 minutes, or 2h 30m of planning in total.

A custom repeat on Monday, Wednesday and Friday for the same two weeks gives 6 occurrences.

## Editing one occurrence or all of them

When you edit, move, resize or delete a repeating block, the app asks: "This occurrence" or "All occurrences".

- **This occurrence** changes only that day. The block becomes a normal one-off block on that day, and the series continues around it.
- **All occurrences** changes the whole series.

Some rules to know:

- Moving an occurrence to another day affects that occurrence only. A whole series cannot change day.
- If you set a series to Never from one occurrence, the series ends the day before, and that day becomes a one-off block.
- Deleting one occurrence skips that day and leaves the rest of the series.

## Day actions that interact with repeats

- **Duplicate a day** copies it to another date as one-off blocks. A series that already runs on the target date is not doubled.
- **Clear a day** deletes the one-off blocks. Repeating blocks are skipped for that day only and return on the next matching day.

## Which one to pick

| You want | Use |
|---|---|
| The same block at the same time every weekday | Repeat: Weekdays |
| The same block on three fixed days | Repeat: Custom |
| A block with a fixed length but a different time each day | Template |
| One day copied to a new date | Duplicate day |

## Limits

- Templates carry no start time and no note.
- The app has no reminders or notifications, so a repeating block does not alert you.
- Upgrading from the first database version removes old whole-day templates.

For the steps to build a full day, see [how to time block your day](../how-to-time-block-your-day/).

Time Blocking runs offline and stores everything on your device.
