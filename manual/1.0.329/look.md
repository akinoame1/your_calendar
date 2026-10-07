# Looks — version 1.0.329

LOOK: every look.* key is a colour of one part of the widget. A value is "default" (as drawn today), "#RRGGBB" or "#AARRGGBB", {"light": "#RRGGBB", "dark": "#RRGGBB"} for the two modes, or "@name" to take another part's colour and follow it as it changes. Names that can be followed: app.accent, app.background, app.line, app.muted, app.onAccent, app.text, battery.fill, battery.fill.critical, battery.fill.fullCharge, battery.fill.regular, battery.fill.warning, battery.percent, battery.temperature.cool, battery.temperature.hot, battery.temperature.warm, batteryBar.cells, batteryBar.fill, batteryBar.fill.critical, batteryBar.fill.fullCharge, batteryBar.fill.regular, batteryBar.fill.warning, batteryBar.track, batteryDate.cuts, batteryDate.fill, batteryDate.fill.critical, batteryDate.fill.fullCharge, batteryDate.fill.regular, batteryDate.fill.warning, batteryDate.outline, batteryDate.terminal, batteryDate.track, chip.alarm, date.fill, date.text, day.number, day.observance, day.weekday, day.weekend, empty.fill, empty.text, header.text, midday.text, month.text, more.text, nav.mark, palette.accent, palette.line, palette.muted, palette.onAccent, palette.text, plus, rule.day, rule.midday, today.fill, today.text, widget.background, widget.text. battery.fill, batteryBar.fill and batteryDate.fill are the colour for the battery's present charge. A part marked (under X) in the list of look keys keeps its own colour until X is set, then takes X's; setting the part itself always wins. A value may also be a list of cases, [{"when": "state" or ["state", …], "value": colour}, …, {"value": colour}]: the first case whose states all hold is used, and a last case without "when" is the rest. States are read when the widget draws, at least every 15 minutes, so a time-of-day look turns within 15 minutes. States:
  now.morning: 06:00–11:59 when drawn
  now.afternoon: 12:00–17:59 when drawn
  now.evening: 18:00–21:59 when drawn
  now.night: 22:00–05:59 when drawn
  now.beforeNoon: before 12:00 when drawn
  now.afterNoon: from 12:00 when drawn
  season.winter: December to February (of the day drawn, in the list; of today, in the header)
  season.spring: March to May
  season.summer: June to August
  season.autumn: September to November
  battery.fullCharge: the charge is at or above widget.batteryFullChargeAt
  battery.regular: the charge is above widget.batteryWarningAt and below widget.batteryFullChargeAt
  battery.warning: the charge is at or below widget.batteryWarningAt
  battery.critical: the charge is at or below widget.batteryCriticalAt
  battery.charging: plugged in
  battery.warm: the battery is at or above widget.batteryWarmAt and below widget.batteryHotAt
  battery.hot: the battery is at or above widget.batteryHotAt
  widget.paged: the widget shows a window other than today's
  day.past: the day drawn is before today
  day.today: the day drawn is today
  day.future: the day drawn is after today
  day.weekend: the day drawn is a weekend day
  day.holiday: the day drawn is a holiday
  day.observance: the day drawn is an observance
  day.trip: the day drawn is in a trip
  day.empty: the day drawn has nothing on it
  chip.task: the item drawn is a task
  chip.done: the item drawn is a done task
  chip.cancelled: the item is cancelled: its title starts with one of behaviour.cancelled.words
  chip.alarm: the item drawn has an alarm
  chip.allDay: the item drawn is all-day
  chip.beforeNoon: the item drawn starts before 12:00
  chip.afterNoon: the item drawn starts at 12:00 or later
