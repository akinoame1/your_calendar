# Worked examples — version 1.0.305

Each is a real kind of request, an answer the app would accept but that misses what was meant, and a good one. Shallow answers are not refused by the app — only you can avoid them.

## "Battery above 79 should be green"

Shallow: `{"look.batteryDate.fill.fullCharge": "#00FF00"}`

Good: `{"look.battery.fill.fullCharge": "#2E7D32"}`

Why: "Above 79" is the full-charge level, and battery.fill colours the bar, the battery in the date and the percentage together; the shallow answer coloured one of the three. Pure #00FF00 under the date's white words reads at 1.4:1; #2E7D32 reads at 5:1.

## "Make battery same color as its filling"

Shallow: `{"look.batteryDate.outline": "#E5A000"}`

Good: `{"look.batteryDate.outline": "@batteryDate.fill"}`

Why: The filling changes colour with the charge; "@" follows it, while a fixed colour matches only one level and is wrong at the others.

## "Version and report line on every screen"

Shallow: `{"app.versionLine": ["SCHEDULE", "EVENT", "EDIT", "SEARCH", "SETTINGS", "CHAT", "REPORT"]}`

Good: `{"app.versionLine": "ALL"}`

Why: A list means exactly the screens it names: this one missed HIDDEN, and every screen a later version adds. "ALL" covers them.

## "Darker widget at night"

Shallow: `{"look.widget.background": "#000000"}`

Good: `{"look.widget.background": [{"when": "now.night", "value": "#000000"}, {"value": "default"}]}`

Why: "At night" is a condition: a list of cases changes it only while now.night holds and leaves the day as it was.

## "Make it green"

Shallow: `{"look.palette.accent": "#00FF00"}`

Good — ask first: Which part should be green -- the date button and today's mark (the accent), the battery, or something else? And a bright green, or a darker one that keeps white words readable?

Why: "It" could be any part, and the shade decides whether words stay readable: asking first costs one message, guessing costs an Apply and a Back.

## "I don't want to see cancelled events"

Shallow: `{"calendars.hidden": []}`

Good: `{"behaviour.cancelled.show": "HIDDEN"}`

Why: Cancelled items have their own setting; hiding calendars would hide everything else in them too.

