# Google Play listing — draft

Drafts for the Play Console, to be checked and edited before use. Issue: akinoame1/my_calendare#333.
Everything here describes the **release** build: no internet permission, no log upload. If a Play
build ever carries the opt-in log upload, the privacy policy, the Data safety answers and the
permission declarations below change with it.

## App details

- **App name** (≤30 chars): `MyCalendar — Schedule widget` _(placeholder: the final name and app ID
  are open decisions)_
- **Short description** (≤80 chars):
  `Your calendars and tasks as a clean schedule widget, with reminders and quick edits.`
- **Category:** Productivity
- **Contact email:** akinoame1@gmail.com
- **Privacy policy URL:** https://github.com/akinoame1/your_calendar/blob/main/privacy-policy.md

## Full description (≤4000 chars)

MyCalendar puts your day on the home screen. It shows the calendars your phone already syncs
(Google Calendar, shared family calendars and others) as a schedule widget: today first, then the
days ahead, each event in its own colour.

• A schedule widget you can scroll, and a date picker that jumps to any day.
• Tasks live in a calendar of your choice. Tick them done from the widget; undone tasks carry over
  to today.
• Create, edit, duplicate, move and recolour events. Change one occurrence of a repeating event or
  the whole series.
• Reminders at the time you choose, with Snooze and Done.
• Holidays and observances marked on the days they fall.
• Notes with simple formatting and checklists.
• A built-in chat helper: describe how you want the widget to look and copy the answer from your
  AI assistant back into the app.
• Battery and charging shown on the widget.

No account, no ads, no tracking. Your calendar data stays on your phone and syncs through your
phone's own calendar sync.

## Graphics checklist

- App icon 512×512 PNG.
- Feature graphic 1024×500.
- At least 2 phone screenshots (16:9 or 9:16, 320–3840 px): the widget on the home screen, the
  schedule app, the event screen, the editor, the date picker.

## Data safety form (release build)

- **Does your app collect or share any of the required user data types?** No.
  - Calendar data is processed only on the device and is not sent to the developer.
  - User-initiated sharing to another app through the system share sheet is not collection by the
    developer.
- **Is all user data encrypted in transit?** Not applicable: no data is transmitted.
- **Do you provide a way for users to request that their data be deleted?** Not applicable:
  nothing is held off the device. Uninstalling removes the app's local data.

## Content rating

IARC questionnaire, category "Utility, Productivity, Communication or Other". It has no violence,
sexuality, gambling or user-generated content shared between users, and no location sharing. The
expected rating is Everyone / PEGI 3.

## Permission declarations

**USE_EXACT_ALARM (exact alarms)**
> MyCalendar is a calendar app that shows event and task notifications at the times the user sets.
> Exact alarms deliver each reminder at its minute, which inexact alarms cannot guarantee.

Play policy names "a calendar app that shows event notifications" as an allowed use.

**USE_FULL_SCREEN_INTENT (full-screen notifications)**
> Event and task reminders the user set appear over the lock screen like an alarm, so a reminder
> is seen at its time. The app asks the user for this permission and works without it, falling
> back to a normal notification.

Play pre-grants this only to alarm and calling apps, so for MyCalendar it is a user-granted
permission.

**FOREGROUND_SERVICE_SPECIAL_USE**
> An optional, user-enabled "live battery" mode keeps the widget's battery and charging display
> current while the phone is charging. It is off by default, shows a persistent notification while
> running, and stops from that notification.

Play requires a video, and the policy asks a foreground service to run "only as long as
necessary". **Recommended:** leave this out of the Play build, and keep the 15-minute battery
refresh there.

## Before the first upload

1. Final app ID and name (permanent once uploaded).
2. Upload-key secrets added (MyTasks task, 2026-10-09). The release then carries
   `mycalendar-play.aab`.
3. Create the app in the Play Console. Under Testing → Internal testing, add testers by email and
   upload `mycalendar-play.aab` by hand. Play App Signing is on by default.
4. Fill in the declarations above, the privacy policy URL, and the Data safety and content rating
   forms.
