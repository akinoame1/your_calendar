# What changed — version 1.0.339 (since 1.0.338)

If you read the manual for 1.0.338, this is what to read again; the check word is now **harbor-8ce0**.

## examples.md

Added: Shallow: `{"look.chip.alarm": "#808080"}`

Added: Good: `{"look.chip.alarm": [{"when": "chip.alarmRang", "value": "#808080"}, {"value": "default"}]}`

Added: Why: The bell is look.chip.alarm, and "after it rang" is the state chip.alarmRang; the shallow answer greys every bell, including the ones still to ring. Never invent a part such as alarm.past.fill: the app refuses it.

## look.md

Added:   chip.alarmRang: the item's alarm is over: it rang, or the item has started (all-day: its day is over); a snoozed alarm is not over

## index.md

Added: Check word: **harbor-8ce0**. When you answer from this manual, write the check word once in your explanation, so the app knows you read it. If you read an earlier version in this conversation, [what changed](changes.md) is what to read again.

Removed: Check word: **umber-5e17**. When you answer from this manual, write the check word once in your explanation, so the app knows you read it. If you read an earlier version in this conversation, [what changed](changes.md) is what to read again.

