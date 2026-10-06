# What changed — version 1.0.319 (since 1.0.318)

If you read the manual for 1.0.318, this is what to read again; the check word is now **nectar-4d60**.

## Settings changed

- `widget.lingerMinutes` — integer 0..720 — Minutes a finished event stays on today's list on the widget: to stop showing events N minutes after they finish, set N; 0 takes them off as they end. The app's schedule keeps past events. Default: 60

## examples.md

Added: Shallow: `{"widget.comingUpMinutes": 5}`

Added: Good: `{"widget.lingerMinutes": 5}`

Added: Why: widget.lingerMinutes is how long a finished event stays on today's list; widget.comingUpMinutes is the notice before an event starts. And never invent a key such as pastEvents.today.hideAfterMinutes: the app refuses every key that is not in the settings.

## index.md

Added: Check word: **nectar-4d60**. When you answer from this manual, write the check word once in your explanation, so the app knows you read it. If you read an earlier version in this conversation, [what changed](changes.md) is what to read again.

Removed: Check word: **quartz-e336**. When you answer from this manual, write the check word once in your explanation, so the app knows you read it. If you read an earlier version in this conversation, [what changed](changes.md) is what to read again.

