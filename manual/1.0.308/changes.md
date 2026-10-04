# What changed — version 1.0.308 (since 1.0.307)

If you read the manual for 1.0.307, this is what to read again; the check word is now **amber-6d0c**.

## Settings added

- `behaviour.rules` — list of {"titleContains": list of words (any, ignoring case), "calendar": calendar name, "colour": "#RRGGBB", "hide": true}; at least one of titleContains/calendar and one of colour/hide — Rules for how items are drawn, first match wins: an item whose title contains any of the words and/or is in the named calendar gets the colour, or is not drawn (hide). The widget and the app only; the event itself is not changed. Empty by default. Default: none

## index.md

Added: Check word: **amber-6d0c**. When you answer from this manual, write the check word once in your explanation, so the app knows you read it. If you read an earlier version in this conversation, [what changed](changes.md) is what to read again.

Removed: Check word: **quartz-636e**. When you answer from this manual, write the check word once in your explanation, so the app knows you read it. If you read an earlier version in this conversation, [what changed](changes.md) is what to read again.

## app.md

Added: THE APP: a schedule list like the widget's, with a month grid above it that can be shown or hidden (app.monthGridOpen), and its own sizes (app.size.*). An event screen to read, edit, move or delete an item: a task's bar has Mark done, a one-tap move (behaviour.reschedule.oneTap) and Other day, a list of preset days (behaviour.reschedule.presets) above a date picker; an event's bar has the quick actions chosen in behaviour.event.quickActions, none by default; a screen to create one (new events take newEvent.*). Settings, and this chat. Undone tasks from past days are drawn on today ("from Tue, Sep 29"); behaviour.tasks.autoMove TODAY also moves them there in the calendar each morning from behaviour.tasks.autoMoveAt, and the schedule then shows "Moved N tasks to today this morning" with Put back. behaviour.rules recolours or hides items by words in their title or by calendar, on the widget and in the app, without changing the events. A line at the bottom of the schedule shows the app version and opens a debug report when tapped; app.versionLine chooses which screens show it (none hides it), app.versionLine.parts what it says, app.versionLine.position and app.versionLine.align where it sits. The month picker (picker.size) is shared by the widget and the app. The look.* keys colour the widget only; the app keeps its own colours for now.

Removed: THE APP: a schedule list like the widget's, with a month grid above it that can be shown or hidden (app.monthGridOpen), and its own sizes (app.size.*). An event screen to read, edit, move or delete an item: a task's bar has Mark done, a one-tap move (behaviour.reschedule.oneTap) and Other day, a list of preset days (behaviour.reschedule.presets) above a date picker; an event's bar has the quick actions chosen in behaviour.event.quickActions, none by default; a screen to create one (new events take newEvent.*). Settings, and this chat. Undone tasks from past days are drawn on today ("from Tue, Sep 29"); behaviour.tasks.autoMove TODAY also moves them there in the calendar each morning from behaviour.tasks.autoMoveAt, and the schedule then shows "Moved N tasks to today this morning" with Put back. A line at the bottom of the schedule shows the app version and opens a debug report when tapped; app.versionLine chooses which screens show it (none hides it), app.versionLine.parts what it says, app.versionLine.position and app.versionLine.align where it sits. The month picker (picker.size) is shared by the widget and the app. The look.* keys colour the widget only; the app keeps its own colours for now.

