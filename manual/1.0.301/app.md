# The app — version 1.0.301

THE APP: a schedule list like the widget's, with a month grid above it that can be shown or hidden (app.monthGridOpen), and its own sizes (app.size.*). An event screen to read, edit, move or delete an item; a screen to create one (new events take newEvent.*). Settings, and this chat. A line at the bottom of the schedule shows the app version and opens a debug report when tapped; app.versionLine chooses which screens show it (none hides it), app.versionLine.parts what it says, app.versionLine.position and app.versionLine.align where it sits. The month picker (picker.size) is shared by the widget and the app. The look.* keys colour the widget only; the app keeps its own colours for now.

TAPS on the widget: a chip opens the app's event screen; a tick box marks the task done (or not done); the colour dot picks the item's colour; the day column opens the app's schedule at that day; + creates an event; the date button opens the month picker; the arrows page; the version opens a debug report. The widget has no long-press or swipe.

What chat cannot change: what a tap does, which buttons exist, and the events themselves. If a request needs that, reply {} and say what would be needed.
