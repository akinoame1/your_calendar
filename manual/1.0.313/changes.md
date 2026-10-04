# What changed — version 1.0.313 (since 1.0.310)

If you read the manual for 1.0.310, this is what to read again; the check word is now **quartz-e336**.

## Settings added

- `widget.batteryLive` — boolean — Show plugging in, unplugging and each percent on the widget at once, instead of within 5-15 minutes. Android allows this only to a running app, so while on a silent notification stays in the shade (it has Stop). Off by default. Default: false

## widget.md

Added: - The battery, by widget.battery; it is redrawn every 15 minutes (5 while charging), or at once on every change with widget.batteryLive on, which keeps a silent notification. BAR is a thin bar across the very top, filled to the charge (batteryBar.fill, one colour per charge level: fullCharge, regular, warning, critical; batteryBar.track the empty part; batteryBar.cells the gaps cutting it in quarters; batteryBar.height its thickness). PILL draws the battery inside the date button instead, see below. OFF draws none. The charge levels: fullCharge from widget.batteryFullChargeAt (80 %), regular, warning at or below widget.batteryWarningAt (30 %), critical at or below widget.batteryCriticalAt (15 %) -- numbers as shipped, CURRENT has his.

Removed: - The battery, by widget.battery: BAR is a thin bar across the very top, filled to the charge (batteryBar.fill, one colour per charge level: fullCharge, regular, warning, critical; batteryBar.track the empty part; batteryBar.cells the gaps cutting it in quarters; batteryBar.height its thickness). PILL draws the battery inside the date button instead, see below. OFF draws none. The charge levels: fullCharge from widget.batteryFullChargeAt (80 %), regular, warning at or below widget.batteryWarningAt (30 %), critical at or below widget.batteryCriticalAt (15 %) -- numbers as shipped, CURRENT has his.

## index.md

Added: Check word: **quartz-e336**. When you answer from this manual, write the check word once in your explanation, so the app knows you read it. If you read an earlier version in this conversation, [what changed](changes.md) is what to read again.

Removed: Check word: **kestrel-6914**. When you answer from this manual, write the check word once in your explanation, so the app knows you read it. If you read an earlier version in this conversation, [what changed](changes.md) is what to read again.

