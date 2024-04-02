# Comparing `tmp/neon-skill-alerts-2.0.1a4.tar.gz` & `tmp/neon-skill-alerts-2.0.1a5.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "neon-skill-alerts-2.0.1a4.tar", last modified: Thu Feb 22 20:31:00 2024, max compression
+gzip compressed data, was "neon-skill-alerts-2.0.1a5.tar", last modified: Tue Apr  2 17:56:38 2024, max compression
```

## Comparing `neon-skill-alerts-2.0.1a4.tar` & `neon-skill-alerts-2.0.1a5.tar`

### file list

```diff
@@ -1,138 +1,138 @@
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-02-22 20:30:59.994544 neon-skill-alerts-2.0.1a4/
--rw-r--r--   0 runner    (1001) docker     (127)     1635 2024-02-22 20:30:57.000000 neon-skill-alerts-2.0.1a4/LICENSE.md
--rw-r--r--   0 runner    (1001) docker     (127)     3149 2024-02-22 20:30:59.994544 neon-skill-alerts-2.0.1a4/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (127)     2870 2024-02-22 20:30:57.000000 neon-skill-alerts-2.0.1a4/README.md
--rw-r--r--   0 runner    (1001) docker     (127)    65247 2024-02-22 20:30:57.000000 neon-skill-alerts-2.0.1a4/__init__.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-02-22 20:30:59.974544 neon-skill-alerts-2.0.1a4/locale/
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-02-22 20:30:59.974544 neon-skill-alerts-2.0.1a4/locale/en-us/
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-02-22 20:30:59.982544 neon-skill-alerts-2.0.1a4/locale/en-us/dialog/
--rw-r--r--   0 runner    (1001) docker     (127)       68 2024-02-22 20:30:57.000000 neon-skill-alerts-2.0.1a4/locale/en-us/dialog/confirm_alert_playback.dialog
--rw-r--r--   0 runner    (1001) docker     (127)       52 2024-02-22 20:30:57.000000 neon-skill-alerts-2.0.1a4/locale/en-us/dialog/confirm_alert_recurring.dialog
--rw-r--r--   0 runner    (1001) docker     (127)       59 2024-02-22 20:30:57.000000 neon-skill-alerts-2.0.1a4/locale/en-us/dialog/confirm_alert_recurring_playback.dialog
--rw-r--r--   0 runner    (1001) docker     (127)       61 2024-02-22 20:30:57.000000 neon-skill-alerts-2.0.1a4/locale/en-us/dialog/confirm_alert_recurring_script.dialog
--rw-r--r--   0 runner    (1001) docker     (127)       67 2024-02-22 20:30:57.000000 neon-skill-alerts-2.0.1a4/locale/en-us/dialog/confirm_alert_script.dialog
--rw-r--r--   0 runner    (1001) docker     (127)       51 2024-02-22 20:30:57.000000 neon-skill-alerts-2.0.1a4/locale/en-us/dialog/confirm_alert_set.dialog
--rw-r--r--   0 runner    (1001) docker     (127)       29 2024-02-22 20:30:57.000000 neon-skill-alerts-2.0.1a4/locale/en-us/dialog/confirm_cancel_alert.dialog
--rw-r--r--   0 runner    (1001) docker     (127)       30 2024-02-22 20:30:57.000000 neon-skill-alerts-2.0.1a4/locale/en-us/dialog/confirm_cancel_all.dialog
--rw-r--r--   0 runner    (1001) docker     (127)       19 2024-02-22 20:30:57.000000 neon-skill-alerts-2.0.1a4/locale/en-us/dialog/confirm_dismiss_alert.dialog
--rw-r--r--   0 runner    (1001) docker     (127)       35 2024-02-22 20:30:57.000000 neon-skill-alerts-2.0.1a4/locale/en-us/dialog/confirm_snooze_alert.dialog
--rw-r--r--   0 runner    (1001) docker     (127)       37 2024-02-22 20:30:57.000000 neon-skill-alerts-2.0.1a4/locale/en-us/dialog/confirm_timer_started.dialog
--rw-r--r--   0 runner    (1001) docker     (127)       97 2024-02-22 20:30:57.000000 neon-skill-alerts-2.0.1a4/locale/en-us/dialog/error_audio_reminder_too_far.dialog
--rw-r--r--   0 runner    (1001) docker     (127)       41 2024-02-22 20:30:57.000000 neon-skill-alerts-2.0.1a4/locale/en-us/dialog/error_no_duration.dialog
--rw-r--r--   0 runner    (1001) docker     (127)       31 2024-02-22 20:30:57.000000 neon-skill-alerts-2.0.1a4/locale/en-us/dialog/error_no_scheduled_kind_to_cancel.dialog
--rw-r--r--   0 runner    (1001) docker     (127)       64 2024-02-22 20:30:57.000000 neon-skill-alerts-2.0.1a4/locale/en-us/dialog/error_no_time.dialog
--rw-r--r--   0 runner    (1001) docker     (127)       44 2024-02-22 20:30:57.000000 neon-skill-alerts-2.0.1a4/locale/en-us/dialog/error_nothing_to_cancel.dialog
--rw-r--r--   0 runner    (1001) docker     (127)       20 2024-02-22 20:30:57.000000 neon-skill-alerts-2.0.1a4/locale/en-us/dialog/expired_alert.dialog
--rw-r--r--   0 runner    (1001) docker     (127)       27 2024-02-22 20:30:57.000000 neon-skill-alerts-2.0.1a4/locale/en-us/dialog/expired_audio_alert_intro.dialog
--rw-r--r--   0 runner    (1001) docker     (127)       32 2024-02-22 20:30:57.000000 neon-skill-alerts-2.0.1a4/locale/en-us/dialog/expired_reminder.dialog
--rw-r--r--   0 runner    (1001) docker     (127)       23 2024-02-22 20:30:57.000000 neon-skill-alerts-2.0.1a4/locale/en-us/dialog/list_alert.dialog
--rw-r--r--   0 runner    (1001) docker     (127)       33 2024-02-22 20:30:57.000000 neon-skill-alerts-2.0.1a4/locale/en-us/dialog/list_alert_intro.dialog
--rw-r--r--   0 runner    (1001) docker     (127)       23 2024-02-22 20:30:57.000000 neon-skill-alerts-2.0.1a4/locale/en-us/dialog/list_alert_missed_intro.dialog
--rw-r--r--   0 runner    (1001) docker     (127)       30 2024-02-22 20:30:57.000000 neon-skill-alerts-2.0.1a4/locale/en-us/dialog/list_alert_none_missed.dialog
--rw-r--r--   0 runner    (1001) docker     (127)       31 2024-02-22 20:30:57.000000 neon-skill-alerts-2.0.1a4/locale/en-us/dialog/list_alert_none_upcoming.dialog
--rw-r--r--   0 runner    (1001) docker     (127)       40 2024-02-22 20:30:57.000000 neon-skill-alerts-2.0.1a4/locale/en-us/dialog/list_alert_repeating.dialog
--rw-r--r--   0 runner    (1001) docker     (127)       55 2024-02-22 20:30:57.000000 neon-skill-alerts-2.0.1a4/locale/en-us/dialog/next_alert_named.dialog
--rw-r--r--   0 runner    (1001) docker     (127)       45 2024-02-22 20:30:57.000000 neon-skill-alerts-2.0.1a4/locale/en-us/dialog/next_alert_unnamed.dialog
--rw-r--r--   0 runner    (1001) docker     (127)       22 2024-02-22 20:30:57.000000 neon-skill-alerts-2.0.1a4/locale/en-us/dialog/quiet_hours_end.dialog
--rw-r--r--   0 runner    (1001) docker     (127)       85 2024-02-22 20:30:57.000000 neon-skill-alerts-2.0.1a4/locale/en-us/dialog/quiet_hours_start.dialog
--rw-r--r--   0 runner    (1001) docker     (127)       41 2024-02-22 20:30:57.000000 neon-skill-alerts-2.0.1a4/locale/en-us/dialog/timer_status.dialog
--rw-r--r--   0 runner    (1001) docker     (127)       27 2024-02-22 20:30:57.000000 neon-skill-alerts-2.0.1a4/locale/en-us/dialog/timer_status_none_active.dialog
--rw-r--r--   0 runner    (1001) docker     (127)        5 2024-02-22 20:30:57.000000 neon-skill-alerts-2.0.1a4/locale/en-us/dialog/word_alarm.dialog
--rw-r--r--   0 runner    (1001) docker     (127)        5 2024-02-22 20:30:57.000000 neon-skill-alerts-2.0.1a4/locale/en-us/dialog/word_alert.dialog
--rw-r--r--   0 runner    (1001) docker     (127)        3 2024-02-22 20:30:57.000000 neon-skill-alerts-2.0.1a4/locale/en-us/dialog/word_day.dialog
--rw-r--r--   0 runner    (1001) docker     (127)        8 2024-02-22 20:30:57.000000 neon-skill-alerts-2.0.1a4/locale/en-us/dialog/word_reminder.dialog
--rw-r--r--   0 runner    (1001) docker     (127)        5 2024-02-22 20:30:57.000000 neon-skill-alerts-2.0.1a4/locale/en-us/dialog/word_timer.dialog
--rw-r--r--   0 runner    (1001) docker     (127)       21 2024-02-22 20:30:57.000000 neon-skill-alerts-2.0.1a4/locale/en-us/dialog/word_weekday.dialog
--rw-r--r--   0 runner    (1001) docker     (127)        6 2024-02-22 20:30:57.000000 neon-skill-alerts-2.0.1a4/locale/en-us/dialog/word_weekday_friday.dialog
--rw-r--r--   0 runner    (1001) docker     (127)        6 2024-02-22 20:30:57.000000 neon-skill-alerts-2.0.1a4/locale/en-us/dialog/word_weekday_monday.dialog
--rw-r--r--   0 runner    (1001) docker     (127)        8 2024-02-22 20:30:57.000000 neon-skill-alerts-2.0.1a4/locale/en-us/dialog/word_weekday_saturday.dialog
--rw-r--r--   0 runner    (1001) docker     (127)        6 2024-02-22 20:30:57.000000 neon-skill-alerts-2.0.1a4/locale/en-us/dialog/word_weekday_sunday.dialog
--rw-r--r--   0 runner    (1001) docker     (127)        8 2024-02-22 20:30:57.000000 neon-skill-alerts-2.0.1a4/locale/en-us/dialog/word_weekday_thursday.dialog
--rw-r--r--   0 runner    (1001) docker     (127)        7 2024-02-22 20:30:57.000000 neon-skill-alerts-2.0.1a4/locale/en-us/dialog/word_weekday_tuesday.dialog
--rw-r--r--   0 runner    (1001) docker     (127)        9 2024-02-22 20:30:57.000000 neon-skill-alerts-2.0.1a4/locale/en-us/dialog/word_weekday_wednesday.dialog
--rw-r--r--   0 runner    (1001) docker     (127)       19 2024-02-22 20:30:57.000000 neon-skill-alerts-2.0.1a4/locale/en-us/dialog/word_weekend.dialog
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-02-22 20:30:59.982544 neon-skill-alerts-2.0.1a4/locale/en-us/intent/
--rw-r--r--   0 runner    (1001) docker     (127)      163 2024-02-22 20:30:57.000000 neon-skill-alerts-2.0.1a4/locale/en-us/intent/list_alerts.intent
--rw-r--r--   0 runner    (1001) docker     (127)      133 2024-02-22 20:30:57.000000 neon-skill-alerts-2.0.1a4/locale/en-us/intent/quiet_hours_end.intent
--rw-r--r--   0 runner    (1001) docker     (127)      199 2024-02-22 20:30:57.000000 neon-skill-alerts-2.0.1a4/locale/en-us/intent/quiet_hours_start.intent
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-02-22 20:30:59.986544 neon-skill-alerts-2.0.1a4/locale/en-us/vocab/
--rw-r--r--   0 runner    (1001) docker     (127)       23 2024-02-22 20:30:57.000000 neon-skill-alerts-2.0.1a4/locale/en-us/vocab/alarm.voc
--rw-r--r--   0 runner    (1001) docker     (127)       12 2024-02-22 20:30:57.000000 neon-skill-alerts-2.0.1a4/locale/en-us/vocab/alert.voc
--rw-r--r--   0 runner    (1001) docker     (127)       20 2024-02-22 20:30:57.000000 neon-skill-alerts-2.0.1a4/locale/en-us/vocab/all.voc
--rw-r--r--   0 runner    (1001) docker     (127)       32 2024-02-22 20:30:57.000000 neon-skill-alerts-2.0.1a4/locale/en-us/vocab/articles.voc
--rw-r--r--   0 runner    (1001) docker     (127)       39 2024-02-22 20:30:57.000000 neon-skill-alerts-2.0.1a4/locale/en-us/vocab/cancel.voc
--rw-r--r--   0 runner    (1001) docker     (127)       68 2024-02-22 20:30:57.000000 neon-skill-alerts-2.0.1a4/locale/en-us/vocab/dismiss.voc
--rw-r--r--   0 runner    (1001) docker     (127)       37 2024-02-22 20:30:57.000000 neon-skill-alerts-2.0.1a4/locale/en-us/vocab/event.voc
--rw-r--r--   0 runner    (1001) docker     (127)       88 2024-02-22 20:30:57.000000 neon-skill-alerts-2.0.1a4/locale/en-us/vocab/everyday.voc
--rw-r--r--   0 runner    (1001) docker     (127)        4 2024-02-22 20:30:57.000000 neon-skill-alerts-2.0.1a4/locale/en-us/vocab/next.voc
--rw-r--r--   0 runner    (1001) docker     (127)       73 2024-02-22 20:30:57.000000 neon-skill-alerts-2.0.1a4/locale/en-us/vocab/playable.voc
--rw-r--r--   0 runner    (1001) docker     (127)       24 2024-02-22 20:30:57.000000 neon-skill-alerts-2.0.1a4/locale/en-us/vocab/priority.voc
--rw-r--r--   0 runner    (1001) docker     (127)       32 2024-02-22 20:30:57.000000 neon-skill-alerts-2.0.1a4/locale/en-us/vocab/query.voc
--rw-r--r--   0 runner    (1001) docker     (127)       20 2024-02-22 20:30:57.000000 neon-skill-alerts-2.0.1a4/locale/en-us/vocab/remind_me.voc
--rw-r--r--   0 runner    (1001) docker     (127)       18 2024-02-22 20:30:57.000000 neon-skill-alerts-2.0.1a4/locale/en-us/vocab/reminder.voc
--rw-r--r--   0 runner    (1001) docker     (127)       15 2024-02-22 20:30:57.000000 neon-skill-alerts-2.0.1a4/locale/en-us/vocab/repeat.voc
--rw-r--r--   0 runner    (1001) docker     (127)       22 2024-02-22 20:30:57.000000 neon-skill-alerts-2.0.1a4/locale/en-us/vocab/script.voc
--rw-r--r--   0 runner    (1001) docker     (127)       32 2024-02-22 20:30:57.000000 neon-skill-alerts-2.0.1a4/locale/en-us/vocab/set.voc
--rw-r--r--   0 runner    (1001) docker     (127)       16 2024-02-22 20:30:57.000000 neon-skill-alerts-2.0.1a4/locale/en-us/vocab/snooze.voc
--rw-r--r--   0 runner    (1001) docker     (127)       17 2024-02-22 20:30:57.000000 neon-skill-alerts-2.0.1a4/locale/en-us/vocab/timer.voc
--rw-r--r--   0 runner    (1001) docker     (127)       43 2024-02-22 20:30:57.000000 neon-skill-alerts-2.0.1a4/locale/en-us/vocab/timer_time_remaining.voc
--rw-r--r--   0 runner    (1001) docker     (127)       23 2024-02-22 20:30:57.000000 neon-skill-alerts-2.0.1a4/locale/en-us/vocab/until.voc
--rw-r--r--   0 runner    (1001) docker     (127)       35 2024-02-22 20:30:57.000000 neon-skill-alerts-2.0.1a4/locale/en-us/vocab/weekdays.voc
--rw-r--r--   0 runner    (1001) docker     (127)       35 2024-02-22 20:30:57.000000 neon-skill-alerts-2.0.1a4/locale/en-us/vocab/weekends.voc
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-02-22 20:30:59.986544 neon-skill-alerts-2.0.1a4/neon_skill_alerts.egg-info/
--rw-r--r--   0 runner    (1001) docker     (127)     3149 2024-02-22 20:30:59.000000 neon-skill-alerts-2.0.1a4/neon_skill_alerts.egg-info/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (127)     4283 2024-02-22 20:30:59.000000 neon-skill-alerts-2.0.1a4/neon_skill_alerts.egg-info/SOURCES.txt
--rw-r--r--   0 runner    (1001) docker     (127)        1 2024-02-22 20:30:59.000000 neon-skill-alerts-2.0.1a4/neon_skill_alerts.egg-info/dependency_links.txt
--rw-r--r--   0 runner    (1001) docker     (127)       72 2024-02-22 20:30:59.000000 neon-skill-alerts-2.0.1a4/neon_skill_alerts.egg-info/entry_points.txt
--rw-r--r--   0 runner    (1001) docker     (127)      146 2024-02-22 20:30:59.000000 neon-skill-alerts-2.0.1a4/neon_skill_alerts.egg-info/requires.txt
--rw-r--r--   0 runner    (1001) docker     (127)       13 2024-02-22 20:30:59.000000 neon-skill-alerts-2.0.1a4/neon_skill_alerts.egg-info/top_level.txt
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-02-22 20:30:59.974544 neon-skill-alerts-2.0.1a4/res/
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-02-22 20:30:59.990544 neon-skill-alerts-2.0.1a4/res/snd/
--rw-r--r--   0 runner    (1001) docker     (127)   496586 2024-02-22 20:30:57.000000 neon-skill-alerts-2.0.1a4/res/snd/default-alarm.wav
--rw-r--r--   0 runner    (1001) docker     (127)   143564 2024-02-22 20:30:57.000000 neon-skill-alerts-2.0.1a4/res/snd/default-timer.wav
--rw-r--r--   0 runner    (1001) docker     (127)       38 2024-02-22 20:30:59.994544 neon-skill-alerts-2.0.1a4/setup.cfg
--rw-r--r--   0 runner    (1001) docker     (127)     4533 2024-02-22 20:30:57.000000 neon-skill-alerts-2.0.1a4/setup.py
--rw-r--r--   0 runner    (1001) docker     (127)     3170 2024-02-22 20:30:57.000000 neon-skill-alerts-2.0.1a4/skill.json
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-02-22 20:30:59.990544 neon-skill-alerts-2.0.1a4/test/
--rw-r--r--   0 runner    (1001) docker     (127)   113860 2024-02-22 20:30:57.000000 neon-skill-alerts-2.0.1a4/test/test_skill.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-02-22 20:30:59.990544 neon-skill-alerts-2.0.1a4/ui/
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-02-22 20:30:59.990544 neon-skill-alerts-2.0.1a4/ui/+mediacenter/
--rw-r--r--   0 runner    (1001) docker     (127)     3546 2024-02-22 20:30:57.000000 neon-skill-alerts-2.0.1a4/ui/+mediacenter/RoundProgress.qml
--rw-r--r--   0 runner    (1001) docker     (127)     2234 2024-02-22 20:30:57.000000 neon-skill-alerts-2.0.1a4/ui/+mediacenter/Timer.qml
--rw-r--r--   0 runner    (1001) docker     (127)     3896 2024-02-22 20:30:57.000000 neon-skill-alerts-2.0.1a4/ui/+mediacenter/TimerCard.qml
--rw-r--r--   0 runner    (1001) docker     (127)     1153 2024-02-22 20:30:57.000000 neon-skill-alerts-2.0.1a4/ui/AlarmBoxControl.qml
--rw-r--r--   0 runner    (1001) docker     (127)     3437 2024-02-22 20:30:57.000000 neon-skill-alerts-2.0.1a4/ui/AlarmBoxView.qml
--rw-r--r--   0 runner    (1001) docker     (127)     4930 2024-02-22 20:30:57.000000 neon-skill-alerts-2.0.1a4/ui/AlarmButtonView.qml
--rw-r--r--   0 runner    (1001) docker     (127)     4468 2024-02-22 20:30:57.000000 neon-skill-alerts-2.0.1a4/ui/AlarmCard.qml
--rw-r--r--   0 runner    (1001) docker     (127)     3073 2024-02-22 20:30:57.000000 neon-skill-alerts-2.0.1a4/ui/AlarmsOverviewCard.qml
--rw-r--r--   0 runner    (1001) docker     (127)     2427 2024-02-22 20:30:57.000000 neon-skill-alerts-2.0.1a4/ui/AlarmsOverviewDelegate.qml
--rw-r--r--   0 runner    (1001) docker     (127)     3546 2024-02-22 20:30:57.000000 neon-skill-alerts-2.0.1a4/ui/RoundProgress.qml
--rw-r--r--   0 runner    (1001) docker     (127)     2557 2024-02-22 20:30:57.000000 neon-skill-alerts-2.0.1a4/ui/Timer.qml
--rw-r--r--   0 runner    (1001) docker     (127)     3469 2024-02-22 20:30:57.000000 neon-skill-alerts-2.0.1a4/ui/TimerCard.qml
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-02-22 20:30:59.990544 neon-skill-alerts-2.0.1a4/ui/icons/
--rw-r--r--   0 runner    (1001) docker     (127)      550 2024-02-22 20:30:57.000000 neon-skill-alerts-2.0.1a4/ui/icons/close.svg
--rw-r--r--   0 runner    (1001) docker     (127)      275 2024-02-22 20:30:57.000000 neon-skill-alerts-2.0.1a4/ui/icons/continue.svg
--rw-r--r--   0 runner    (1001) docker     (127)      352 2024-02-22 20:30:57.000000 neon-skill-alerts-2.0.1a4/ui/icons/pause.svg
--rw-r--r--   0 runner    (1001) docker     (127)      272 2024-02-22 20:30:57.000000 neon-skill-alerts-2.0.1a4/ui/qmldir
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-02-22 20:30:59.990544 neon-skill-alerts-2.0.1a4/ui/sounds/
--rw-r--r--   0 runner    (1001) docker     (127)    15240 2024-02-22 20:30:57.000000 neon-skill-alerts-2.0.1a4/ui/sounds/clicked.wav
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-02-22 20:30:59.994544 neon-skill-alerts-2.0.1a4/ui/translations/
--rw-r--r--   0 runner    (1001) docker     (127)       90 2024-02-22 20:30:57.000000 neon-skill-alerts-2.0.1a4/ui/translations/TimerCard_de.ts
--rw-r--r--   0 runner    (1001) docker     (127)       90 2024-02-22 20:30:57.000000 neon-skill-alerts-2.0.1a4/ui/translations/TimerCard_es.ts
--rw-r--r--   0 runner    (1001) docker     (127)       90 2024-02-22 20:30:57.000000 neon-skill-alerts-2.0.1a4/ui/translations/TimerCard_fr.ts
--rw-r--r--   0 runner    (1001) docker     (127)       90 2024-02-22 20:30:57.000000 neon-skill-alerts-2.0.1a4/ui/translations/TimerCard_it.ts
--rw-r--r--   0 runner    (1001) docker     (127)       90 2024-02-22 20:30:57.000000 neon-skill-alerts-2.0.1a4/ui/translations/TimerCard_nl.ts
--rw-r--r--   0 runner    (1001) docker     (127)       90 2024-02-22 20:30:57.000000 neon-skill-alerts-2.0.1a4/ui/translations/TimerCard_pt.ts
--rw-r--r--   0 runner    (1001) docker     (127)       33 2024-02-22 20:30:57.000000 neon-skill-alerts-2.0.1a4/ui/translations/skill-ovos-timer.openvoiceos_de.qm
--rw-r--r--   0 runner    (1001) docker     (127)       33 2024-02-22 20:30:57.000000 neon-skill-alerts-2.0.1a4/ui/translations/skill-ovos-timer.openvoiceos_es.qm
--rw-r--r--   0 runner    (1001) docker     (127)       33 2024-02-22 20:30:57.000000 neon-skill-alerts-2.0.1a4/ui/translations/skill-ovos-timer.openvoiceos_fr.qm
--rw-r--r--   0 runner    (1001) docker     (127)       33 2024-02-22 20:30:57.000000 neon-skill-alerts-2.0.1a4/ui/translations/skill-ovos-timer.openvoiceos_it.qm
--rw-r--r--   0 runner    (1001) docker     (127)       33 2024-02-22 20:30:57.000000 neon-skill-alerts-2.0.1a4/ui/translations/skill-ovos-timer.openvoiceos_nl.qm
--rw-r--r--   0 runner    (1001) docker     (127)       33 2024-02-22 20:30:57.000000 neon-skill-alerts-2.0.1a4/ui/translations/skill-ovos-timer.openvoiceos_pt.qm
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-02-22 20:30:59.994544 neon-skill-alerts-2.0.1a4/util/
--rw-r--r--   0 runner    (1001) docker     (127)     2573 2024-02-22 20:30:57.000000 neon-skill-alerts-2.0.1a4/util/__init__.py
--rw-r--r--   0 runner    (1001) docker     (127)    10166 2024-02-22 20:30:57.000000 neon-skill-alerts-2.0.1a4/util/alert.py
--rw-r--r--   0 runner    (1001) docker     (127)    16625 2024-02-22 20:30:57.000000 neon-skill-alerts-2.0.1a4/util/alert_manager.py
--rw-r--r--   0 runner    (1001) docker     (127)    22330 2024-02-22 20:30:57.000000 neon-skill-alerts-2.0.1a4/util/parse_utils.py
--rw-r--r--   0 runner    (1001) docker     (127)     4503 2024-02-22 20:30:57.000000 neon-skill-alerts-2.0.1a4/util/ui_models.py
--rw-r--r--   0 runner    (1001) docker     (127)     1856 2024-02-22 20:30:57.000000 neon-skill-alerts-2.0.1a4/version.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-02 17:56:38.384293 neon-skill-alerts-2.0.1a5/
+-rw-r--r--   0 runner    (1001) docker     (127)     1635 2024-04-02 17:56:34.000000 neon-skill-alerts-2.0.1a5/LICENSE.md
+-rw-r--r--   0 runner    (1001) docker     (127)     3149 2024-04-02 17:56:38.384293 neon-skill-alerts-2.0.1a5/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (127)     2870 2024-04-02 17:56:34.000000 neon-skill-alerts-2.0.1a5/README.md
+-rw-r--r--   0 runner    (1001) docker     (127)    65247 2024-04-02 17:56:34.000000 neon-skill-alerts-2.0.1a5/__init__.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-02 17:56:38.364293 neon-skill-alerts-2.0.1a5/locale/
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-02 17:56:38.364293 neon-skill-alerts-2.0.1a5/locale/en-us/
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-02 17:56:38.372293 neon-skill-alerts-2.0.1a5/locale/en-us/dialog/
+-rw-r--r--   0 runner    (1001) docker     (127)       68 2024-04-02 17:56:34.000000 neon-skill-alerts-2.0.1a5/locale/en-us/dialog/confirm_alert_playback.dialog
+-rw-r--r--   0 runner    (1001) docker     (127)       52 2024-04-02 17:56:34.000000 neon-skill-alerts-2.0.1a5/locale/en-us/dialog/confirm_alert_recurring.dialog
+-rw-r--r--   0 runner    (1001) docker     (127)       59 2024-04-02 17:56:34.000000 neon-skill-alerts-2.0.1a5/locale/en-us/dialog/confirm_alert_recurring_playback.dialog
+-rw-r--r--   0 runner    (1001) docker     (127)       61 2024-04-02 17:56:34.000000 neon-skill-alerts-2.0.1a5/locale/en-us/dialog/confirm_alert_recurring_script.dialog
+-rw-r--r--   0 runner    (1001) docker     (127)       67 2024-04-02 17:56:34.000000 neon-skill-alerts-2.0.1a5/locale/en-us/dialog/confirm_alert_script.dialog
+-rw-r--r--   0 runner    (1001) docker     (127)       51 2024-04-02 17:56:34.000000 neon-skill-alerts-2.0.1a5/locale/en-us/dialog/confirm_alert_set.dialog
+-rw-r--r--   0 runner    (1001) docker     (127)       29 2024-04-02 17:56:34.000000 neon-skill-alerts-2.0.1a5/locale/en-us/dialog/confirm_cancel_alert.dialog
+-rw-r--r--   0 runner    (1001) docker     (127)       30 2024-04-02 17:56:34.000000 neon-skill-alerts-2.0.1a5/locale/en-us/dialog/confirm_cancel_all.dialog
+-rw-r--r--   0 runner    (1001) docker     (127)       19 2024-04-02 17:56:34.000000 neon-skill-alerts-2.0.1a5/locale/en-us/dialog/confirm_dismiss_alert.dialog
+-rw-r--r--   0 runner    (1001) docker     (127)       35 2024-04-02 17:56:34.000000 neon-skill-alerts-2.0.1a5/locale/en-us/dialog/confirm_snooze_alert.dialog
+-rw-r--r--   0 runner    (1001) docker     (127)       37 2024-04-02 17:56:34.000000 neon-skill-alerts-2.0.1a5/locale/en-us/dialog/confirm_timer_started.dialog
+-rw-r--r--   0 runner    (1001) docker     (127)       97 2024-04-02 17:56:34.000000 neon-skill-alerts-2.0.1a5/locale/en-us/dialog/error_audio_reminder_too_far.dialog
+-rw-r--r--   0 runner    (1001) docker     (127)       41 2024-04-02 17:56:34.000000 neon-skill-alerts-2.0.1a5/locale/en-us/dialog/error_no_duration.dialog
+-rw-r--r--   0 runner    (1001) docker     (127)       31 2024-04-02 17:56:34.000000 neon-skill-alerts-2.0.1a5/locale/en-us/dialog/error_no_scheduled_kind_to_cancel.dialog
+-rw-r--r--   0 runner    (1001) docker     (127)       64 2024-04-02 17:56:34.000000 neon-skill-alerts-2.0.1a5/locale/en-us/dialog/error_no_time.dialog
+-rw-r--r--   0 runner    (1001) docker     (127)       44 2024-04-02 17:56:34.000000 neon-skill-alerts-2.0.1a5/locale/en-us/dialog/error_nothing_to_cancel.dialog
+-rw-r--r--   0 runner    (1001) docker     (127)       20 2024-04-02 17:56:34.000000 neon-skill-alerts-2.0.1a5/locale/en-us/dialog/expired_alert.dialog
+-rw-r--r--   0 runner    (1001) docker     (127)       27 2024-04-02 17:56:34.000000 neon-skill-alerts-2.0.1a5/locale/en-us/dialog/expired_audio_alert_intro.dialog
+-rw-r--r--   0 runner    (1001) docker     (127)       32 2024-04-02 17:56:34.000000 neon-skill-alerts-2.0.1a5/locale/en-us/dialog/expired_reminder.dialog
+-rw-r--r--   0 runner    (1001) docker     (127)       23 2024-04-02 17:56:34.000000 neon-skill-alerts-2.0.1a5/locale/en-us/dialog/list_alert.dialog
+-rw-r--r--   0 runner    (1001) docker     (127)       33 2024-04-02 17:56:34.000000 neon-skill-alerts-2.0.1a5/locale/en-us/dialog/list_alert_intro.dialog
+-rw-r--r--   0 runner    (1001) docker     (127)       23 2024-04-02 17:56:34.000000 neon-skill-alerts-2.0.1a5/locale/en-us/dialog/list_alert_missed_intro.dialog
+-rw-r--r--   0 runner    (1001) docker     (127)       30 2024-04-02 17:56:34.000000 neon-skill-alerts-2.0.1a5/locale/en-us/dialog/list_alert_none_missed.dialog
+-rw-r--r--   0 runner    (1001) docker     (127)       31 2024-04-02 17:56:34.000000 neon-skill-alerts-2.0.1a5/locale/en-us/dialog/list_alert_none_upcoming.dialog
+-rw-r--r--   0 runner    (1001) docker     (127)       40 2024-04-02 17:56:34.000000 neon-skill-alerts-2.0.1a5/locale/en-us/dialog/list_alert_repeating.dialog
+-rw-r--r--   0 runner    (1001) docker     (127)       55 2024-04-02 17:56:34.000000 neon-skill-alerts-2.0.1a5/locale/en-us/dialog/next_alert_named.dialog
+-rw-r--r--   0 runner    (1001) docker     (127)       45 2024-04-02 17:56:34.000000 neon-skill-alerts-2.0.1a5/locale/en-us/dialog/next_alert_unnamed.dialog
+-rw-r--r--   0 runner    (1001) docker     (127)       22 2024-04-02 17:56:34.000000 neon-skill-alerts-2.0.1a5/locale/en-us/dialog/quiet_hours_end.dialog
+-rw-r--r--   0 runner    (1001) docker     (127)       85 2024-04-02 17:56:34.000000 neon-skill-alerts-2.0.1a5/locale/en-us/dialog/quiet_hours_start.dialog
+-rw-r--r--   0 runner    (1001) docker     (127)       41 2024-04-02 17:56:34.000000 neon-skill-alerts-2.0.1a5/locale/en-us/dialog/timer_status.dialog
+-rw-r--r--   0 runner    (1001) docker     (127)       27 2024-04-02 17:56:34.000000 neon-skill-alerts-2.0.1a5/locale/en-us/dialog/timer_status_none_active.dialog
+-rw-r--r--   0 runner    (1001) docker     (127)        5 2024-04-02 17:56:34.000000 neon-skill-alerts-2.0.1a5/locale/en-us/dialog/word_alarm.dialog
+-rw-r--r--   0 runner    (1001) docker     (127)        5 2024-04-02 17:56:34.000000 neon-skill-alerts-2.0.1a5/locale/en-us/dialog/word_alert.dialog
+-rw-r--r--   0 runner    (1001) docker     (127)        3 2024-04-02 17:56:34.000000 neon-skill-alerts-2.0.1a5/locale/en-us/dialog/word_day.dialog
+-rw-r--r--   0 runner    (1001) docker     (127)        8 2024-04-02 17:56:34.000000 neon-skill-alerts-2.0.1a5/locale/en-us/dialog/word_reminder.dialog
+-rw-r--r--   0 runner    (1001) docker     (127)        5 2024-04-02 17:56:34.000000 neon-skill-alerts-2.0.1a5/locale/en-us/dialog/word_timer.dialog
+-rw-r--r--   0 runner    (1001) docker     (127)       21 2024-04-02 17:56:34.000000 neon-skill-alerts-2.0.1a5/locale/en-us/dialog/word_weekday.dialog
+-rw-r--r--   0 runner    (1001) docker     (127)        6 2024-04-02 17:56:34.000000 neon-skill-alerts-2.0.1a5/locale/en-us/dialog/word_weekday_friday.dialog
+-rw-r--r--   0 runner    (1001) docker     (127)        6 2024-04-02 17:56:34.000000 neon-skill-alerts-2.0.1a5/locale/en-us/dialog/word_weekday_monday.dialog
+-rw-r--r--   0 runner    (1001) docker     (127)        8 2024-04-02 17:56:34.000000 neon-skill-alerts-2.0.1a5/locale/en-us/dialog/word_weekday_saturday.dialog
+-rw-r--r--   0 runner    (1001) docker     (127)        6 2024-04-02 17:56:34.000000 neon-skill-alerts-2.0.1a5/locale/en-us/dialog/word_weekday_sunday.dialog
+-rw-r--r--   0 runner    (1001) docker     (127)        8 2024-04-02 17:56:34.000000 neon-skill-alerts-2.0.1a5/locale/en-us/dialog/word_weekday_thursday.dialog
+-rw-r--r--   0 runner    (1001) docker     (127)        7 2024-04-02 17:56:34.000000 neon-skill-alerts-2.0.1a5/locale/en-us/dialog/word_weekday_tuesday.dialog
+-rw-r--r--   0 runner    (1001) docker     (127)        9 2024-04-02 17:56:34.000000 neon-skill-alerts-2.0.1a5/locale/en-us/dialog/word_weekday_wednesday.dialog
+-rw-r--r--   0 runner    (1001) docker     (127)       19 2024-04-02 17:56:34.000000 neon-skill-alerts-2.0.1a5/locale/en-us/dialog/word_weekend.dialog
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-02 17:56:38.372293 neon-skill-alerts-2.0.1a5/locale/en-us/intent/
+-rw-r--r--   0 runner    (1001) docker     (127)      163 2024-04-02 17:56:34.000000 neon-skill-alerts-2.0.1a5/locale/en-us/intent/list_alerts.intent
+-rw-r--r--   0 runner    (1001) docker     (127)      133 2024-04-02 17:56:34.000000 neon-skill-alerts-2.0.1a5/locale/en-us/intent/quiet_hours_end.intent
+-rw-r--r--   0 runner    (1001) docker     (127)      199 2024-04-02 17:56:34.000000 neon-skill-alerts-2.0.1a5/locale/en-us/intent/quiet_hours_start.intent
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-02 17:56:38.376293 neon-skill-alerts-2.0.1a5/locale/en-us/vocab/
+-rw-r--r--   0 runner    (1001) docker     (127)       23 2024-04-02 17:56:34.000000 neon-skill-alerts-2.0.1a5/locale/en-us/vocab/alarm.voc
+-rw-r--r--   0 runner    (1001) docker     (127)       12 2024-04-02 17:56:34.000000 neon-skill-alerts-2.0.1a5/locale/en-us/vocab/alert.voc
+-rw-r--r--   0 runner    (1001) docker     (127)       20 2024-04-02 17:56:34.000000 neon-skill-alerts-2.0.1a5/locale/en-us/vocab/all.voc
+-rw-r--r--   0 runner    (1001) docker     (127)       32 2024-04-02 17:56:34.000000 neon-skill-alerts-2.0.1a5/locale/en-us/vocab/articles.voc
+-rw-r--r--   0 runner    (1001) docker     (127)       39 2024-04-02 17:56:34.000000 neon-skill-alerts-2.0.1a5/locale/en-us/vocab/cancel.voc
+-rw-r--r--   0 runner    (1001) docker     (127)       68 2024-04-02 17:56:34.000000 neon-skill-alerts-2.0.1a5/locale/en-us/vocab/dismiss.voc
+-rw-r--r--   0 runner    (1001) docker     (127)       37 2024-04-02 17:56:34.000000 neon-skill-alerts-2.0.1a5/locale/en-us/vocab/event.voc
+-rw-r--r--   0 runner    (1001) docker     (127)       88 2024-04-02 17:56:34.000000 neon-skill-alerts-2.0.1a5/locale/en-us/vocab/everyday.voc
+-rw-r--r--   0 runner    (1001) docker     (127)        4 2024-04-02 17:56:34.000000 neon-skill-alerts-2.0.1a5/locale/en-us/vocab/next.voc
+-rw-r--r--   0 runner    (1001) docker     (127)       73 2024-04-02 17:56:34.000000 neon-skill-alerts-2.0.1a5/locale/en-us/vocab/playable.voc
+-rw-r--r--   0 runner    (1001) docker     (127)       24 2024-04-02 17:56:34.000000 neon-skill-alerts-2.0.1a5/locale/en-us/vocab/priority.voc
+-rw-r--r--   0 runner    (1001) docker     (127)       32 2024-04-02 17:56:34.000000 neon-skill-alerts-2.0.1a5/locale/en-us/vocab/query.voc
+-rw-r--r--   0 runner    (1001) docker     (127)       20 2024-04-02 17:56:34.000000 neon-skill-alerts-2.0.1a5/locale/en-us/vocab/remind_me.voc
+-rw-r--r--   0 runner    (1001) docker     (127)       18 2024-04-02 17:56:34.000000 neon-skill-alerts-2.0.1a5/locale/en-us/vocab/reminder.voc
+-rw-r--r--   0 runner    (1001) docker     (127)       15 2024-04-02 17:56:34.000000 neon-skill-alerts-2.0.1a5/locale/en-us/vocab/repeat.voc
+-rw-r--r--   0 runner    (1001) docker     (127)       22 2024-04-02 17:56:34.000000 neon-skill-alerts-2.0.1a5/locale/en-us/vocab/script.voc
+-rw-r--r--   0 runner    (1001) docker     (127)       32 2024-04-02 17:56:34.000000 neon-skill-alerts-2.0.1a5/locale/en-us/vocab/set.voc
+-rw-r--r--   0 runner    (1001) docker     (127)       16 2024-04-02 17:56:34.000000 neon-skill-alerts-2.0.1a5/locale/en-us/vocab/snooze.voc
+-rw-r--r--   0 runner    (1001) docker     (127)       17 2024-04-02 17:56:34.000000 neon-skill-alerts-2.0.1a5/locale/en-us/vocab/timer.voc
+-rw-r--r--   0 runner    (1001) docker     (127)       43 2024-04-02 17:56:34.000000 neon-skill-alerts-2.0.1a5/locale/en-us/vocab/timer_time_remaining.voc
+-rw-r--r--   0 runner    (1001) docker     (127)       23 2024-04-02 17:56:34.000000 neon-skill-alerts-2.0.1a5/locale/en-us/vocab/until.voc
+-rw-r--r--   0 runner    (1001) docker     (127)       35 2024-04-02 17:56:34.000000 neon-skill-alerts-2.0.1a5/locale/en-us/vocab/weekdays.voc
+-rw-r--r--   0 runner    (1001) docker     (127)       35 2024-04-02 17:56:34.000000 neon-skill-alerts-2.0.1a5/locale/en-us/vocab/weekends.voc
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-02 17:56:38.376293 neon-skill-alerts-2.0.1a5/neon_skill_alerts.egg-info/
+-rw-r--r--   0 runner    (1001) docker     (127)     3149 2024-04-02 17:56:38.000000 neon-skill-alerts-2.0.1a5/neon_skill_alerts.egg-info/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (127)     4283 2024-04-02 17:56:38.000000 neon-skill-alerts-2.0.1a5/neon_skill_alerts.egg-info/SOURCES.txt
+-rw-r--r--   0 runner    (1001) docker     (127)        1 2024-04-02 17:56:38.000000 neon-skill-alerts-2.0.1a5/neon_skill_alerts.egg-info/dependency_links.txt
+-rw-r--r--   0 runner    (1001) docker     (127)       72 2024-04-02 17:56:38.000000 neon-skill-alerts-2.0.1a5/neon_skill_alerts.egg-info/entry_points.txt
+-rw-r--r--   0 runner    (1001) docker     (127)      136 2024-04-02 17:56:38.000000 neon-skill-alerts-2.0.1a5/neon_skill_alerts.egg-info/requires.txt
+-rw-r--r--   0 runner    (1001) docker     (127)       13 2024-04-02 17:56:38.000000 neon-skill-alerts-2.0.1a5/neon_skill_alerts.egg-info/top_level.txt
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-02 17:56:38.364293 neon-skill-alerts-2.0.1a5/res/
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-02 17:56:38.376293 neon-skill-alerts-2.0.1a5/res/snd/
+-rw-r--r--   0 runner    (1001) docker     (127)   496586 2024-04-02 17:56:34.000000 neon-skill-alerts-2.0.1a5/res/snd/default-alarm.wav
+-rw-r--r--   0 runner    (1001) docker     (127)   143564 2024-04-02 17:56:34.000000 neon-skill-alerts-2.0.1a5/res/snd/default-timer.wav
+-rw-r--r--   0 runner    (1001) docker     (127)       38 2024-04-02 17:56:38.384293 neon-skill-alerts-2.0.1a5/setup.cfg
+-rw-r--r--   0 runner    (1001) docker     (127)     4533 2024-04-02 17:56:34.000000 neon-skill-alerts-2.0.1a5/setup.py
+-rw-r--r--   0 runner    (1001) docker     (127)     3170 2024-04-02 17:56:34.000000 neon-skill-alerts-2.0.1a5/skill.json
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-02 17:56:38.376293 neon-skill-alerts-2.0.1a5/test/
+-rw-r--r--   0 runner    (1001) docker     (127)   113860 2024-04-02 17:56:34.000000 neon-skill-alerts-2.0.1a5/test/test_skill.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-02 17:56:38.380293 neon-skill-alerts-2.0.1a5/ui/
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-02 17:56:38.380293 neon-skill-alerts-2.0.1a5/ui/+mediacenter/
+-rw-r--r--   0 runner    (1001) docker     (127)     3546 2024-04-02 17:56:34.000000 neon-skill-alerts-2.0.1a5/ui/+mediacenter/RoundProgress.qml
+-rw-r--r--   0 runner    (1001) docker     (127)     2234 2024-04-02 17:56:34.000000 neon-skill-alerts-2.0.1a5/ui/+mediacenter/Timer.qml
+-rw-r--r--   0 runner    (1001) docker     (127)     3896 2024-04-02 17:56:34.000000 neon-skill-alerts-2.0.1a5/ui/+mediacenter/TimerCard.qml
+-rw-r--r--   0 runner    (1001) docker     (127)     1153 2024-04-02 17:56:34.000000 neon-skill-alerts-2.0.1a5/ui/AlarmBoxControl.qml
+-rw-r--r--   0 runner    (1001) docker     (127)     3437 2024-04-02 17:56:34.000000 neon-skill-alerts-2.0.1a5/ui/AlarmBoxView.qml
+-rw-r--r--   0 runner    (1001) docker     (127)     4930 2024-04-02 17:56:34.000000 neon-skill-alerts-2.0.1a5/ui/AlarmButtonView.qml
+-rw-r--r--   0 runner    (1001) docker     (127)     4468 2024-04-02 17:56:34.000000 neon-skill-alerts-2.0.1a5/ui/AlarmCard.qml
+-rw-r--r--   0 runner    (1001) docker     (127)     3073 2024-04-02 17:56:34.000000 neon-skill-alerts-2.0.1a5/ui/AlarmsOverviewCard.qml
+-rw-r--r--   0 runner    (1001) docker     (127)     2427 2024-04-02 17:56:34.000000 neon-skill-alerts-2.0.1a5/ui/AlarmsOverviewDelegate.qml
+-rw-r--r--   0 runner    (1001) docker     (127)     3546 2024-04-02 17:56:34.000000 neon-skill-alerts-2.0.1a5/ui/RoundProgress.qml
+-rw-r--r--   0 runner    (1001) docker     (127)     2557 2024-04-02 17:56:34.000000 neon-skill-alerts-2.0.1a5/ui/Timer.qml
+-rw-r--r--   0 runner    (1001) docker     (127)     3469 2024-04-02 17:56:34.000000 neon-skill-alerts-2.0.1a5/ui/TimerCard.qml
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-02 17:56:38.380293 neon-skill-alerts-2.0.1a5/ui/icons/
+-rw-r--r--   0 runner    (1001) docker     (127)      550 2024-04-02 17:56:34.000000 neon-skill-alerts-2.0.1a5/ui/icons/close.svg
+-rw-r--r--   0 runner    (1001) docker     (127)      275 2024-04-02 17:56:34.000000 neon-skill-alerts-2.0.1a5/ui/icons/continue.svg
+-rw-r--r--   0 runner    (1001) docker     (127)      352 2024-04-02 17:56:34.000000 neon-skill-alerts-2.0.1a5/ui/icons/pause.svg
+-rw-r--r--   0 runner    (1001) docker     (127)      272 2024-04-02 17:56:34.000000 neon-skill-alerts-2.0.1a5/ui/qmldir
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-02 17:56:38.380293 neon-skill-alerts-2.0.1a5/ui/sounds/
+-rw-r--r--   0 runner    (1001) docker     (127)    15240 2024-04-02 17:56:34.000000 neon-skill-alerts-2.0.1a5/ui/sounds/clicked.wav
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-02 17:56:38.384293 neon-skill-alerts-2.0.1a5/ui/translations/
+-rw-r--r--   0 runner    (1001) docker     (127)       90 2024-04-02 17:56:34.000000 neon-skill-alerts-2.0.1a5/ui/translations/TimerCard_de.ts
+-rw-r--r--   0 runner    (1001) docker     (127)       90 2024-04-02 17:56:34.000000 neon-skill-alerts-2.0.1a5/ui/translations/TimerCard_es.ts
+-rw-r--r--   0 runner    (1001) docker     (127)       90 2024-04-02 17:56:34.000000 neon-skill-alerts-2.0.1a5/ui/translations/TimerCard_fr.ts
+-rw-r--r--   0 runner    (1001) docker     (127)       90 2024-04-02 17:56:34.000000 neon-skill-alerts-2.0.1a5/ui/translations/TimerCard_it.ts
+-rw-r--r--   0 runner    (1001) docker     (127)       90 2024-04-02 17:56:34.000000 neon-skill-alerts-2.0.1a5/ui/translations/TimerCard_nl.ts
+-rw-r--r--   0 runner    (1001) docker     (127)       90 2024-04-02 17:56:34.000000 neon-skill-alerts-2.0.1a5/ui/translations/TimerCard_pt.ts
+-rw-r--r--   0 runner    (1001) docker     (127)       33 2024-04-02 17:56:34.000000 neon-skill-alerts-2.0.1a5/ui/translations/skill-ovos-timer.openvoiceos_de.qm
+-rw-r--r--   0 runner    (1001) docker     (127)       33 2024-04-02 17:56:34.000000 neon-skill-alerts-2.0.1a5/ui/translations/skill-ovos-timer.openvoiceos_es.qm
+-rw-r--r--   0 runner    (1001) docker     (127)       33 2024-04-02 17:56:34.000000 neon-skill-alerts-2.0.1a5/ui/translations/skill-ovos-timer.openvoiceos_fr.qm
+-rw-r--r--   0 runner    (1001) docker     (127)       33 2024-04-02 17:56:34.000000 neon-skill-alerts-2.0.1a5/ui/translations/skill-ovos-timer.openvoiceos_it.qm
+-rw-r--r--   0 runner    (1001) docker     (127)       33 2024-04-02 17:56:34.000000 neon-skill-alerts-2.0.1a5/ui/translations/skill-ovos-timer.openvoiceos_nl.qm
+-rw-r--r--   0 runner    (1001) docker     (127)       33 2024-04-02 17:56:34.000000 neon-skill-alerts-2.0.1a5/ui/translations/skill-ovos-timer.openvoiceos_pt.qm
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-02 17:56:38.384293 neon-skill-alerts-2.0.1a5/util/
+-rw-r--r--   0 runner    (1001) docker     (127)     2573 2024-04-02 17:56:34.000000 neon-skill-alerts-2.0.1a5/util/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (127)    10166 2024-04-02 17:56:34.000000 neon-skill-alerts-2.0.1a5/util/alert.py
+-rw-r--r--   0 runner    (1001) docker     (127)    16625 2024-04-02 17:56:34.000000 neon-skill-alerts-2.0.1a5/util/alert_manager.py
+-rw-r--r--   0 runner    (1001) docker     (127)    22330 2024-04-02 17:56:34.000000 neon-skill-alerts-2.0.1a5/util/parse_utils.py
+-rw-r--r--   0 runner    (1001) docker     (127)     4503 2024-04-02 17:56:34.000000 neon-skill-alerts-2.0.1a5/util/ui_models.py
+-rw-r--r--   0 runner    (1001) docker     (127)     1856 2024-04-02 17:56:34.000000 neon-skill-alerts-2.0.1a5/version.py
```

### Comparing `neon-skill-alerts-2.0.1a4/LICENSE.md` & `neon-skill-alerts-2.0.1a5/LICENSE.md`

 * *Files identical despite different names*

### Comparing `neon-skill-alerts-2.0.1a4/PKG-INFO` & `neon-skill-alerts-2.0.1a5/PKG-INFO`

 * *Files 1% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: neon-skill-alerts
-Version: 2.0.1a4
+Version: 2.0.1a5
 Home-page: https://github.com/NeonGeckoCom/skill-alerts
 Author: Neongecko
 Author-email: developers@neon.ai
 License: BSD-3-Clause
 Description-Content-Type: text/markdown
 Provides-Extra: test
 License-File: LICENSE.md
```

### Comparing `neon-skill-alerts-2.0.1a4/README.md` & `neon-skill-alerts-2.0.1a5/README.md`

 * *Files identical despite different names*

### Comparing `neon-skill-alerts-2.0.1a4/__init__.py` & `neon-skill-alerts-2.0.1a5/__init__.py`

 * *Files 0% similar despite different names*

```diff
@@ -1046,15 +1046,15 @@
             volume = resp.data.get('percent')
         else:
             volume = None
         while self.alert_manager.get_alert_status(alert_id) == \
                 AlertState.ACTIVE and time.time() < timeout:
             if message.context.get("klat_data"):
                 log_deprecation("`klat.response` emit will be removed. Listen "
-                                "for `neon.alert_expired", "3.0.0")
+                                "for `neon.alert_expired", "4.0.0")
                 self.send_with_audio(self.dialog_renderer.render(
                     "expired_alert", {'name': alert.alert_name}),
                     to_play, message, private=True)
             else:
                 # TODO: refactor to `self.play_audio`
                 LOG.debug(f"Playing file: {to_play}")
                 play_audio(to_play).wait(60)
```

### Comparing `neon-skill-alerts-2.0.1a4/neon_skill_alerts.egg-info/PKG-INFO` & `neon-skill-alerts-2.0.1a5/neon_skill_alerts.egg-info/PKG-INFO`

 * *Files 1% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: neon-skill-alerts
-Version: 2.0.1a4
+Version: 2.0.1a5
 Home-page: https://github.com/NeonGeckoCom/skill-alerts
 Author: Neongecko
 Author-email: developers@neon.ai
 License: BSD-3-Clause
 Description-Content-Type: text/markdown
 Provides-Extra: test
 License-File: LICENSE.md
```

### Comparing `neon-skill-alerts-2.0.1a4/neon_skill_alerts.egg-info/SOURCES.txt` & `neon-skill-alerts-2.0.1a5/neon_skill_alerts.egg-info/SOURCES.txt`

 * *Files identical despite different names*

### Comparing `neon-skill-alerts-2.0.1a4/res/snd/default-alarm.wav` & `neon-skill-alerts-2.0.1a5/res/snd/default-alarm.wav`

 * *Files identical despite different names*

### Comparing `neon-skill-alerts-2.0.1a4/res/snd/default-timer.wav` & `neon-skill-alerts-2.0.1a5/res/snd/default-timer.wav`

 * *Files identical despite different names*

### Comparing `neon-skill-alerts-2.0.1a4/setup.py` & `neon-skill-alerts-2.0.1a5/setup.py`

 * *Files identical despite different names*

### Comparing `neon-skill-alerts-2.0.1a4/skill.json` & `neon-skill-alerts-2.0.1a5/skill.json`

 * *Files identical despite different names*

### Comparing `neon-skill-alerts-2.0.1a4/test/test_skill.py` & `neon-skill-alerts-2.0.1a5/test/test_skill.py`

 * *Files identical despite different names*

### Comparing `neon-skill-alerts-2.0.1a4/ui/+mediacenter/RoundProgress.qml` & `neon-skill-alerts-2.0.1a5/ui/+mediacenter/RoundProgress.qml`

 * *Files identical despite different names*

### Comparing `neon-skill-alerts-2.0.1a4/ui/+mediacenter/Timer.qml` & `neon-skill-alerts-2.0.1a5/ui/+mediacenter/Timer.qml`

 * *Files identical despite different names*

### Comparing `neon-skill-alerts-2.0.1a4/ui/+mediacenter/TimerCard.qml` & `neon-skill-alerts-2.0.1a5/ui/+mediacenter/TimerCard.qml`

 * *Files identical despite different names*

### Comparing `neon-skill-alerts-2.0.1a4/ui/AlarmBoxControl.qml` & `neon-skill-alerts-2.0.1a5/ui/AlarmBoxControl.qml`

 * *Files identical despite different names*

### Comparing `neon-skill-alerts-2.0.1a4/ui/AlarmBoxView.qml` & `neon-skill-alerts-2.0.1a5/ui/AlarmBoxView.qml`

 * *Files identical despite different names*

### Comparing `neon-skill-alerts-2.0.1a4/ui/AlarmButtonView.qml` & `neon-skill-alerts-2.0.1a5/ui/AlarmButtonView.qml`

 * *Files identical despite different names*

### Comparing `neon-skill-alerts-2.0.1a4/ui/AlarmCard.qml` & `neon-skill-alerts-2.0.1a5/ui/AlarmCard.qml`

 * *Files identical despite different names*

### Comparing `neon-skill-alerts-2.0.1a4/ui/AlarmsOverviewCard.qml` & `neon-skill-alerts-2.0.1a5/ui/AlarmsOverviewCard.qml`

 * *Files identical despite different names*

### Comparing `neon-skill-alerts-2.0.1a4/ui/AlarmsOverviewDelegate.qml` & `neon-skill-alerts-2.0.1a5/ui/AlarmsOverviewDelegate.qml`

 * *Files identical despite different names*

### Comparing `neon-skill-alerts-2.0.1a4/ui/RoundProgress.qml` & `neon-skill-alerts-2.0.1a5/ui/RoundProgress.qml`

 * *Files identical despite different names*

### Comparing `neon-skill-alerts-2.0.1a4/ui/Timer.qml` & `neon-skill-alerts-2.0.1a5/ui/Timer.qml`

 * *Files identical despite different names*

### Comparing `neon-skill-alerts-2.0.1a4/ui/TimerCard.qml` & `neon-skill-alerts-2.0.1a5/ui/TimerCard.qml`

 * *Files identical despite different names*

### Comparing `neon-skill-alerts-2.0.1a4/ui/icons/close.svg` & `neon-skill-alerts-2.0.1a5/ui/icons/close.svg`

 * *Files identical despite different names*

### Comparing `neon-skill-alerts-2.0.1a4/ui/sounds/clicked.wav` & `neon-skill-alerts-2.0.1a5/ui/sounds/clicked.wav`

 * *Files identical despite different names*

### Comparing `neon-skill-alerts-2.0.1a4/util/__init__.py` & `neon-skill-alerts-2.0.1a5/util/__init__.py`

 * *Files identical despite different names*

### Comparing `neon-skill-alerts-2.0.1a4/util/alert.py` & `neon-skill-alerts-2.0.1a5/util/alert.py`

 * *Files identical despite different names*

### Comparing `neon-skill-alerts-2.0.1a4/util/alert_manager.py` & `neon-skill-alerts-2.0.1a5/util/alert_manager.py`

 * *Files identical despite different names*

### Comparing `neon-skill-alerts-2.0.1a4/util/parse_utils.py` & `neon-skill-alerts-2.0.1a5/util/parse_utils.py`

 * *Files identical despite different names*

### Comparing `neon-skill-alerts-2.0.1a4/util/ui_models.py` & `neon-skill-alerts-2.0.1a5/util/ui_models.py`

 * *Files identical despite different names*

### Comparing `neon-skill-alerts-2.0.1a4/version.py` & `neon-skill-alerts-2.0.1a5/version.py`

 * *Files 1% similar despite different names*

```diff
@@ -22,8 +22,8 @@
 # EXEMPLARY, OR CONSEQUENTIAL DAMAGES (INCLUDING, BUT NOT LIMITED TO,
 # PROCUREMENT OF SUBSTITUTE GOODS OR SERVICES; LOSS OF USE, DATA,
 # OR PROFITS;  OR BUSINESS INTERRUPTION) HOWEVER CAUSED AND ON ANY THEORY OF
 # LIABILITY, WHETHER IN CONTRACT, STRICT LIABILITY, OR TORT (INCLUDING
 # NEGLIGENCE OR OTHERWISE) ARISING IN ANY WAY OUT OF THE USE OF THIS
 # SOFTWARE,  EVEN IF ADVISED OF THE POSSIBILITY OF SUCH DAMAGE.
 
-__version__ = "2.0.1a4"
+__version__ = "2.0.1a5"
```

