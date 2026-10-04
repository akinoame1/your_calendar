# What changed — version 1.0.305 (since 1.0.304)

If you read the manual for 1.0.304, this is what to read again; the check word is now **kestrel-8f39**.

## Settings added

- `behaviour.widget.chipTap` — one of: OPEN, SHEET — What a tap on a widget chip does: OPEN the event in the app, or SHEET, a quick sheet over the home screen (Done, Tomorrow, Cancel, Colour, Open, Delete). Default: OPEN
- `behaviour.widget.chipEnd` — one of: COLOUR, SHEET, NONE — The dot at a widget chip's end (chip.handle): COLOUR picks the item's colour, SHEET opens the quick sheet, NONE draws no dot. Default: COLOUR

## index.md

Added: Check word: **kestrel-8f39**. When you answer from this manual, write the check word once in your explanation, so the app knows you read it. If you read an earlier version in this conversation, [what changed](changes.md) is what to read again.

Removed: Check word: **cedar-8232**. When you answer from this manual, write the check word once in your explanation, so the app knows you read it. If you read an earlier version in this conversation, [what changed](changes.md) is what to read again.

## app.md

Added: TAPS on the widget: a chip opens the app's event screen, or a quick sheet over the home screen with Done, Tomorrow, Cancel (keep it), Colour, Open and Delete (behaviour.widget.chipTap); a tick box marks the task done (or not done); the dot at a chip's end picks the item's colour, opens the quick sheet, or is not drawn (behaviour.widget.chipEnd); the day column opens the app's schedule at that day; + creates an event; the date button opens the month picker; the arrows page; the version opens a debug report. The widget has no long-press or swipe.

Added: What chat cannot change: what the other taps do, which buttons exist, and the events themselves. If a request needs that, reply {} and say what would be needed.

Removed: TAPS on the widget: a chip opens the app's event screen; a tick box marks the task done (or not done); the colour dot picks the item's colour; the day column opens the app's schedule at that day; + creates an event; the date button opens the month picker; the arrows page; the version opens a debug report. The widget has no long-press or swipe.

Removed: What chat cannot change: what a tap does, which buttons exist, and the events themselves. If a request needs that, reply {} and say what would be needed.

