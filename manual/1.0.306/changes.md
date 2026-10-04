# What changed — version 1.0.306 (since 1.0.305)

If you read the manual for 1.0.305, this is what to read again; the check word is now **nectar-b7ea**.

## Settings added

- `behaviour.reschedule.oneTap` — one of: ONE_DAY, WEEKEND, NEXT_WEEK, NEXT_MONTH, NONE — The task screen's one-tap move: ONE_DAY (tomorrow, or a day after the task), WEEKEND, NEXT_WEEK, NEXT_MONTH, or NONE (no button; Other day stays). Default: ONE_DAY
- `behaviour.reschedule.presets` — ordered list of: PULL_IN, TOMORROW, NEXT_DAY, THIS_WEEKEND, NEXT_WEEKEND, NEXT_WEEK, NEXT_MONTH — The days Other day offers a task, in this order; one that would not move it later is left out (PULL_IN only for a task still ahead). A date picker is always below them. Default: PULL_IN, TOMORROW, NEXT_DAY, THIS_WEEKEND, NEXT_WEEKEND
- `behaviour.event.quickActions` — ordered list of: LATER_15_MIN, LATER_1_HOUR, NEXT_DAY, NEXT_WEEK, CANCEL — Buttons on an event's screen (not a task's), in this order: LATER_15_MIN, LATER_1_HOUR (timed events only), NEXT_DAY and NEXT_WEEK (same time), CANCEL (cancel or uncancel, keeping it). None by default. Default: none

## index.md

Added: Check word: **nectar-b7ea**. When you answer from this manual, write the check word once in your explanation, so the app knows you read it. If you read an earlier version in this conversation, [what changed](changes.md) is what to read again.

Removed: Check word: **kestrel-8f39**. When you answer from this manual, write the check word once in your explanation, so the app knows you read it. If you read an earlier version in this conversation, [what changed](changes.md) is what to read again.

## app.md

Added: THE APP: a schedule list like the widget's, with a month grid above it that can be shown or hidden (app.monthGridOpen), and its own sizes (app.size.*). An event screen to read, edit, move or delete an item: a task's bar has Mark done, a one-tap move (behaviour.reschedule.oneTap) and Other day, a list of preset days (behaviour.reschedule.presets) above a date picker; an event's bar has the quick actions chosen in behaviour.event.quickActions, none by default; a screen to create one (new events take newEvent.*). Settings, and this chat. A line at the bottom of the schedule shows the app version and opens a debug report when tapped; app.versionLine chooses which screens show it (none hides it), app.versionLine.parts what it says, app.versionLine.position and app.versionLine.align where it sits. The month picker (picker.size) is shared by the widget and the app. The look.* keys colour the widget only; the app keeps its own colours for now.

Removed: THE APP: a schedule list like the widget's, with a month grid above it that can be shown or hidden (app.monthGridOpen), and its own sizes (app.size.*). An event screen to read, edit, move or delete an item; a screen to create one (new events take newEvent.*). Settings, and this chat. A line at the bottom of the schedule shows the app version and opens a debug report when tapped; app.versionLine chooses which screens show it (none hides it), app.versionLine.parts what it says, app.versionLine.position and app.versionLine.align where it sits. The month picker (picker.size) is shared by the widget and the app. The look.* keys colour the widget only; the app keeps its own colours for now.

