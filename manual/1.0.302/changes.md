# What changed — version 1.0.302 (since 1.0.301)

If you read the manual for 1.0.301, this is what to read again; the check word is now **birch-3ec8**.

## Settings changed

- `app.versionLine.parts` — ordered list of: VERSION, BUILT, REPORT, at least 1 — What the version line says, in this order: VERSION (1.0.N), BUILT (the build time), REPORT (the word report). Default: VERSION, BUILT, REPORT
- `behaviour.cancelled.words` — list of texts, at least 1 — Words that mark an event or task as cancelled when its title starts with one (any case); Cancel writes the first. Cancelled items never notify, ring or carry over. Default: CANCELED, CANCELLED
- `newEvent.calendar` — one of, or null (this phone's calendar names) — Calendar a new event goes to; null for the phone's first writable one. Default: none
- `tasks.calendar` — one of, or null (this phone's calendar names) — The calendar whose events are tasks. Default: none
- `calendars.hidden` — list of (this phone's calendar names) — Calendars kept off the widget and the schedule. Default: none
- `look.palette.accent` — The accent: the date button, today's mark, the outline of the battery in the date, the paging arrows and words
- `look.palette.onAccent` — Words drawn on the accent: the date's words, today's number
- `look.palette.text` — Main words: day numbers, month names, messages on the page
- `look.palette.muted` — Quiet words: weekday names, the +, the header's time and version, the midday time, "Nothing here"
- `look.palette.line` — Lines and quiet fills: between days, the midday line, the battery bar's empty part, an empty day's box
- `look.battery.fill.fullCharge` — The battery's colour everywhere -- the bar, the battery in the date, and the percentage, when the battery is at full charge
- `look.battery.fill.regular` — The battery's colour everywhere -- the bar, the battery in the date, and the percentage, when the battery is regular
- `look.battery.fill.warning` — The battery's colour everywhere -- the bar, the battery in the date, and the percentage, when the battery is at warning
- `look.battery.fill.critical` — The battery's colour everywhere -- the bar, the battery in the date, and the percentage, when the battery is critical
- `look.widget.background` — The widget's page
- `look.widget.text` — Plain words on the page: the empty-list and loading messages (under palette.text)
- `look.header.text` — The time and version in the header (under palette.muted)
- `look.date.fill` — The date button's fill (when the battery is not drawn in it) (under palette.accent)
- `look.date.text` — The date button's words (under palette.onAccent)
- `look.batteryBar.track` — The battery bar's empty part (under palette.line)
- `look.batteryBar.cells` — The gaps between the battery bar's quarters (follows widget.background)
- `look.batteryBar.fill.fullCharge` — The battery bar's filled part, when the battery is at full charge (under battery.fill)
- `look.batteryBar.fill.regular` — The battery bar's filled part, when the battery is regular (under battery.fill)
- `look.batteryBar.fill.warning` — The battery bar's filled part, when the battery is at warning (under battery.fill)
- `look.batteryBar.fill.critical` — The battery bar's filled part, when the battery is critical (under battery.fill)
- `look.batteryDate.fill.fullCharge` — The battery's filled part, in the date, when the battery is at full charge (under battery.fill)
- `look.batteryDate.fill.regular` — The battery's filled part, in the date, when the battery is regular (under battery.fill)
- `look.batteryDate.fill.warning` — The battery's filled part, in the date, when the battery is at warning (under battery.fill)
- `look.batteryDate.fill.critical` — The battery's filled part, in the date, when the battery is critical (under battery.fill)
- `look.batteryDate.outline` — The outline of the battery drawn in the date (under palette.accent)
- `look.batteryDate.terminal` — The battery's band and + terminal, in the date (follows batteryDate.outline)
- `look.batteryDate.track` — The battery's empty part, in the date (follows widget.background)
- `look.batteryDate.cuts` — The cuts at the quarters of the battery in the date (follows widget.background)
- `look.battery.percent` — The battery percentage (follows batteryBar.fill)
- `look.battery.temperature.cool` — The battery temperature below widget.batteryWarmAt
- `look.battery.temperature.warm` — The battery temperature from widget.batteryWarmAt to below widget.batteryHotAt
- `look.battery.temperature.hot` — The battery temperature from widget.batteryHotAt
- `look.rule.day` — The line between days and before a month (under palette.line)
- `look.rule.midday` — The midday line (under palette.line)
- `look.midday.text` — The midday line's time (under palette.muted)
- `look.month.text` — A month's name in the list (under palette.text)
- `look.day.weekday` — A weekday's name (under palette.muted)
- `look.day.number` — A day's number (under palette.text)
- `look.day.weekend` — A weekend's or holiday's name and number
- `look.day.observance` — An observance's name and number
- `look.today.fill` — Today's round mark, and today's weekday name (under palette.accent)
- `look.today.text` — Today's number on its mark (under palette.onAccent)
- `look.plus` — The + under a day (under palette.muted)
- `look.more.text` — The 'earlier' and 'more days' words (under palette.accent)
- `look.empty.fill` — A day with nothing on it: its box (under palette.line)
- `look.empty.text` — A day with nothing on it: its words (under palette.muted)
- `look.chip.text` — Every event's and task's words (by default worked out from each chip's colour) (per item)
- `look.chip.time` — Every event's time (per item)
- `look.chip.check` — A task's tick box (per item)
- `look.chip.handle` — The colour dot at a chip's end (per item)
- `look.nav.mark` — The double arrows that page the list (under palette.accent)
- `look.chip.alarm` — The bell on a chip with an alarm
- `look.size.date` — The date button's words (and the button with them)
- `look.size.header.text` — The time and version in the header
- `look.size.battery.text` — The battery's percentage and temperature
- `look.size.batteryBar.height` — The battery bar's thickness
- `look.size.widget.text` — The words on an empty or unreadable list
- `look.size.day.column` — The day column's width
- `look.size.day.weekday` — A weekday's name
- `look.size.day.number` — A day's number
- `look.size.today` — Today's round mark and its number
- `look.size.day.specials` — Special days' dots under the day number
- `look.size.plus` — The + under a day
- `look.size.midday.text` — The midday line's time
- `look.size.month.text` — A month's name in the list
- `look.size.more.text` — The 'earlier' and 'more days' words
- `look.size.chip.text` — Every event's and task's words (the chip grows with them)
- `look.size.chip.time` — Every event's time

## schema.md

Added: Settings — one per line: key — what it takes — what it does. Default: a fresh install's value.

## look-keys.md

Added: Look colours — every look.* key below takes a colour value (see LOOK); on a fresh install each is "default", drawn as shipped.

Added: (under X): its own colour until X is set, then X's. (follows X): X's colour unless set itself. (per item): worked out for each item unless set. Setting the part itself always wins.

Added: Look sizes — every look.size.* key takes a whole percent of its usual size, 50..250; 100 on a fresh install.

## look.md

Added: LOOK: every look.* key is a colour of one part of the widget. A value is "default" (as drawn today), "#RRGGBB" or "#AARRGGBB", {"light": "#RRGGBB", "dark": "#RRGGBB"} for the two modes, or "@name" to take another part's colour and follow it as it changes. Names that can be followed: battery.fill, battery.fill.critical, battery.fill.fullCharge, battery.fill.regular, battery.fill.warning, battery.percent, battery.temperature.cool, battery.temperature.hot, battery.temperature.warm, batteryBar.cells, batteryBar.fill, batteryBar.fill.critical, batteryBar.fill.fullCharge, batteryBar.fill.regular, batteryBar.fill.warning, batteryBar.track, batteryDate.cuts, batteryDate.fill, batteryDate.fill.critical, batteryDate.fill.fullCharge, batteryDate.fill.regular, batteryDate.fill.warning, batteryDate.outline, batteryDate.terminal, batteryDate.track, chip.alarm, date.fill, date.text, day.number, day.observance, day.weekday, day.weekend, empty.fill, empty.text, header.text, midday.text, month.text, more.text, nav.mark, palette.accent, palette.line, palette.muted, palette.onAccent, palette.text, plus, rule.day, rule.midday, today.fill, today.text, widget.background, widget.text. battery.fill, batteryBar.fill and batteryDate.fill are the colour for the battery's present charge. A part marked (under X) in the list of look keys keeps its own colour until X is set, then takes X's; setting the part itself always wins. A value may also be a list of cases, [{"when": "state" or ["state", …], "value": colour}, …, {"value": colour}]: the first case whose states all hold is used, and a last case without "when" is the rest. States are read when the widget draws, at least every 15 minutes, so a time-of-day look turns within 15 minutes. States:

Removed: LOOK: every look.* key is a colour of one part of the widget. A value is "default" (as drawn today), "#RRGGBB" or "#AARRGGBB", {"light": "#RRGGBB", "dark": "#RRGGBB"} for the two modes, or "@name" to take another part's colour and follow it as it changes. Names that can be followed: battery.fill, battery.fill.critical, battery.fill.fullCharge, battery.fill.regular, battery.fill.warning, battery.percent, battery.temperature.cool, battery.temperature.hot, battery.temperature.warm, batteryBar.cells, batteryBar.fill, batteryBar.fill.critical, batteryBar.fill.fullCharge, batteryBar.fill.regular, batteryBar.fill.warning, batteryBar.track, batteryDate.cuts, batteryDate.fill, batteryDate.fill.critical, batteryDate.fill.fullCharge, batteryDate.fill.regular, batteryDate.fill.warning, batteryDate.outline, batteryDate.terminal, batteryDate.track, chip.alarm, date.fill, date.text, day.number, day.observance, day.weekday, day.weekend, empty.fill, empty.text, header.text, midday.text, month.text, more.text, nav.mark, palette.accent, palette.line, palette.muted, palette.onAccent, palette.text, plus, rule.day, rule.midday, today.fill, today.text, widget.background, widget.text. battery.fill, batteryBar.fill and batteryDate.fill are the colour for the battery's present charge. A part whose SCHEMA line says "follows look.X once that is set" keeps its own colour until X is set, then takes X's; setting the part itself always wins. A value may also be a list of cases, [{"when": "state" or ["state", …], "value": colour}, …, {"value": colour}]: the first case whose states all hold is used, and a last case without "when" is the rest. States are read when the widget draws, at least every 15 minutes, so a time-of-day look turns within 15 minutes. States:

## index.md

Added: Check word: **birch-3ec8**. When you answer from this manual, write the check word once in your explanation, so the app knows you read it. If you read an earlier version in this conversation, [what changed](changes.md) is what to read again.

Added: - [Worked examples](examples.md) — real requests, a shallow answer and a good one, and why

Removed: Check word: **quartz-3722**. When you answer from this manual, write the check word once in your explanation, so the app knows you read it. If you read an earlier version in this conversation, [what changed](changes.md) is what to read again.

## examples.md

Added: Each is a real kind of request, an answer the app would accept but that misses what was meant, and a good one. Shallow answers are not refused by the app — only you can avoid them.

Added: Shallow: `{"look.batteryDate.fill.fullCharge": "#00FF00"}`

Added: Good: `{"look.battery.fill.fullCharge": "#2E7D32"}`

Added: Why: "Above 79" is the full-charge level, and battery.fill colours the bar, the battery in the date and the percentage together; the shallow answer coloured one of the three. Pure #00FF00 under the date's white words reads at 1.4:1; #2E7D32 reads at 5:1.

Added: Shallow: `{"look.batteryDate.outline": "#E5A000"}`

Added: Good: `{"look.batteryDate.outline": "@batteryDate.fill"}`

Added: Why: The filling changes colour with the charge; "@" follows it, while a fixed colour matches only one level and is wrong at the others.

Added: Shallow: `{"app.versionLine": ["SCHEDULE", "EVENT", "EDIT", "SEARCH", "SETTINGS", "CHAT", "REPORT"]}`

Added: Good: `{"app.versionLine": "ALL"}`

Added: Why: A list means exactly the screens it names: this one missed HIDDEN, and every screen a later version adds. "ALL" covers them.

Added: Shallow: `{"look.widget.background": "#000000"}`

Added: Good: `{"look.widget.background": [{"when": "now.night", "value": "#000000"}, {"value": "default"}]}`

Added: Why: "At night" is a condition: a list of cases changes it only while now.night holds and leaves the day as it was.

Added: Shallow: `{"look.palette.accent": "#00FF00"}`

Added: Good — ask first: Which part should be green -- the date button and today's mark (the accent), the battery, or something else? And a bright green, or a darker one that keeps white words readable?

Added: Why: "It" could be any part, and the shade decides whether words stay readable: asking first costs one message, guessing costs an Apply and a Back.

Added: Shallow: `{"calendars.hidden": []}`

Added: Good: `{"behaviour.cancelled.show": "HIDDEN"}`

Added: Why: Cancelled items have their own setting; hiding calendars would hide everything else in them too.

