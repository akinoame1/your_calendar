# What changed — version 1.0.307 (since 1.0.306)

If you read the manual for 1.0.306, this is what to read again; the check word is now **quartz-636e**.

## Settings added

- `behaviour.tasks.autoMove` — one of: OFF, TODAY — Undone tasks from past days, as carried onto today: OFF only draws them there (default); TODAY moves them to today in the calendar itself, once each morning, keeping their time of day. Writes to the calendar; the app lists what it moved, with Put back. Default: OFF
- `behaviour.tasks.autoMoveAt` — integer 0..23 — The hour from which the morning move runs (the first refresh after it, within about 15 minutes). Default: 6

## index.md

Added: Check word: **quartz-636e**. When you answer from this manual, write the check word once in your explanation, so the app knows you read it. If you read an earlier version in this conversation, [what changed](changes.md) is what to read again.

Removed: Check word: **nectar-b7ea**. When you answer from this manual, write the check word once in your explanation, so the app knows you read it. If you read an earlier version in this conversation, [what changed](changes.md) is what to read again.

## app.md

Added: THE APP: a schedule list like the widget's, with a month grid above it that can be shown or hidden (app.monthGridOpen), and its own sizes (app.size.*). An event screen to read, edit, move or delete an item: a task's bar has Mark done, a one-tap move (behaviour.reschedule.oneTap) and Other day, a list of preset days (behaviour.reschedule.presets) above a date picker; an event's bar has the quick actions chosen in behaviour.event.quickActions, none by default; a screen to create one (new events take newEvent.*). Settings, and this chat. Undone tasks from past days are drawn on today ("from Tue, Sep 29"); behaviour.tasks.autoMove TODAY also moves them there in the calendar each morning from behaviour.tasks.autoMoveAt, and the schedule then shows "Moved N tasks to today this morning" with Put back. A line at the bottom of the schedule shows the app version and opens a debug report when tapped; app.versionLine chooses which screens show it (none hides it), app.versionLine.parts what it says, app.versionLine.position and app.versionLine.align where it sits. The month picker (picker.size) is shared by the widget and the app. The look.* keys colour the widget only; the app keeps its own colours for now.

Removed: THE APP: a schedule list like the widget's, with a month grid above it that can be shown or hidden (app.monthGridOpen), and its own sizes (app.size.*). An event screen to read, edit, move or delete an item: a task's bar has Mark done, a one-tap move (behaviour.reschedule.oneTap) and Other day, a list of preset days (behaviour.reschedule.presets) above a date picker; an event's bar has the quick actions chosen in behaviour.event.quickActions, none by default; a screen to create one (new events take newEvent.*). Settings, and this chat. A line at the bottom of the schedule shows the app version and opens a debug report when tapped; app.versionLine chooses which screens show it (none hides it), app.versionLine.parts what it says, app.versionLine.position and app.versionLine.align where it sits. The month picker (picker.size) is shared by the widget and the app. The look.* keys colour the widget only; the app keeps its own colours for now.

