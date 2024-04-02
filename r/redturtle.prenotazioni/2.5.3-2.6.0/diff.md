# Comparing `tmp/redturtle.prenotazioni-2.5.3.tar.gz` & `tmp/redturtle.prenotazioni-2.6.0.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "redturtle.prenotazioni-2.5.3.tar", last modified: Tue Mar 19 08:48:10 2024, max compression
+gzip compressed data, was "redturtle.prenotazioni-2.6.0.tar", last modified: Tue Apr  2 07:43:54 2024, max compression
```

## Comparing `redturtle.prenotazioni-2.5.3.tar` & `redturtle.prenotazioni-2.6.0.tar`

### file list

```diff
@@ -1,377 +1,380 @@
-drwxr-xr-x   0 lucabel    (501) staff       (20)        0 2024-03-19 08:48:10.839102 redturtle.prenotazioni-2.5.3/
--rw-r--r--   0 lucabel    (501) staff       (20)      748 2024-03-19 08:48:10.000000 redturtle.prenotazioni-2.5.3/APP_IO.txt
--rw-r--r--   0 lucabel    (501) staff       (20)    16591 2024-03-19 08:48:10.000000 redturtle.prenotazioni-2.5.3/CHANGES.rst
--rw-r--r--   0 lucabel    (501) staff       (20)      152 2024-03-19 08:48:10.000000 redturtle.prenotazioni-2.5.3/CONTRIBUTORS.rst
--rw-r--r--   0 lucabel    (501) staff       (20)      586 2024-03-19 08:48:10.000000 redturtle.prenotazioni-2.5.3/DEVELOP.rst
--rw-r--r--   0 lucabel    (501) staff       (20)    18092 2024-03-19 08:48:10.000000 redturtle.prenotazioni-2.5.3/LICENSE.GPL
--rw-r--r--   0 lucabel    (501) staff       (20)      667 2024-03-19 08:48:10.000000 redturtle.prenotazioni-2.5.3/LICENSE.rst
--rw-r--r--   0 lucabel    (501) staff       (20)      110 2024-03-19 08:48:10.000000 redturtle.prenotazioni-2.5.3/MANIFEST.in
--rw-r--r--   0 lucabel    (501) staff       (20)    45109 2024-03-19 08:48:10.839260 redturtle.prenotazioni-2.5.3/PKG-INFO
--rw-r--r--   0 lucabel    (501) staff       (20)    27109 2024-03-19 08:48:10.000000 redturtle.prenotazioni-2.5.3/README.rst
--rw-r--r--   0 lucabel    (501) staff       (20)      164 2024-03-19 08:48:10.000000 redturtle.prenotazioni-2.5.3/TODO.txt
--rw-r--r--   0 lucabel    (501) staff       (20)      105 2024-03-19 08:48:10.000000 redturtle.prenotazioni-2.5.3/constraints-5.2.x.txt
--rw-r--r--   0 lucabel    (501) staff       (20)      105 2024-03-19 08:48:10.000000 redturtle.prenotazioni-2.5.3/constraints.txt
-drwxr-xr-x   0 lucabel    (501) staff       (20)        0 2024-03-19 08:48:10.749092 redturtle.prenotazioni-2.5.3/docs/
--rw-r--r--   0 lucabel    (501) staff       (20)     7984 2024-03-19 08:48:10.000000 redturtle.prenotazioni-2.5.3/docs/conf.py
--rw-r--r--   0 lucabel    (501) staff       (20)       89 2024-03-19 08:48:10.000000 redturtle.prenotazioni-2.5.3/docs/index.rst
--rw-r--r--   0 lucabel    (501) staff       (20)      476 2024-03-19 08:48:10.000000 redturtle.prenotazioni-2.5.3/requirements-6.0.x.txt
--rw-r--r--   0 lucabel    (501) staff       (20)       48 2024-03-19 08:48:10.000000 redturtle.prenotazioni-2.5.3/requirements.txt
--rw-r--r--   0 lucabel    (501) staff       (20)      344 2024-03-19 08:48:10.839724 redturtle.prenotazioni-2.5.3/setup.cfg
--rw-r--r--   0 lucabel    (501) staff       (20)     3420 2024-03-19 08:48:10.000000 redturtle.prenotazioni-2.5.3/setup.py
-drwxr-xr-x   0 lucabel    (501) staff       (20)        0 2024-03-19 08:48:10.735452 redturtle.prenotazioni-2.5.3/src/
-drwxr-xr-x   0 lucabel    (501) staff       (20)        0 2024-03-19 08:48:10.749313 redturtle.prenotazioni-2.5.3/src/redturtle/
--rw-r--r--   0 lucabel    (501) staff       (20)       80 2024-03-19 08:48:10.000000 redturtle.prenotazioni-2.5.3/src/redturtle/__init__.py
-drwxr-xr-x   0 lucabel    (501) staff       (20)        0 2024-03-19 08:48:10.754321 redturtle.prenotazioni-2.5.3/src/redturtle/prenotazioni/
--rw-r--r--   0 lucabel    (501) staff       (20)     4638 2024-03-19 08:48:10.000000 redturtle.prenotazioni-2.5.3/src/redturtle/prenotazioni/__init__.py
-drwxr-xr-x   0 lucabel    (501) staff       (20)        0 2024-03-19 08:48:10.755020 redturtle.prenotazioni-2.5.3/src/redturtle/prenotazioni/actions/
--rw-r--r--   0 lucabel    (501) staff       (20)        0 2024-03-19 08:48:10.000000 redturtle.prenotazioni-2.5.3/src/redturtle/prenotazioni/actions/__init__.py
--rw-r--r--   0 lucabel    (501) staff       (20)      226 2024-03-19 08:48:10.000000 redturtle.prenotazioni-2.5.3/src/redturtle/prenotazioni/actions/configure.zcml
--rw-r--r--   0 lucabel    (501) staff       (20)     3333 2024-03-19 08:48:10.000000 redturtle.prenotazioni-2.5.3/src/redturtle/prenotazioni/actions/mail.py
-drwxr-xr-x   0 lucabel    (501) staff       (20)        0 2024-03-19 08:48:10.757310 redturtle.prenotazioni-2.5.3/src/redturtle/prenotazioni/adapters/
--rw-r--r--   0 lucabel    (501) staff       (20)       24 2024-03-19 08:48:10.000000 redturtle.prenotazioni-2.5.3/src/redturtle/prenotazioni/adapters/__init__.py
--rw-r--r--   0 lucabel    (501) staff       (20)    15273 2024-03-19 08:48:10.000000 redturtle.prenotazioni-2.5.3/src/redturtle/prenotazioni/adapters/booker.py
--rw-r--r--   0 lucabel    (501) staff       (20)      729 2024-03-19 08:48:10.000000 redturtle.prenotazioni-2.5.3/src/redturtle/prenotazioni/adapters/booking_code.py
--rw-r--r--   0 lucabel    (501) staff       (20)     5974 2024-03-19 08:48:10.000000 redturtle.prenotazioni-2.5.3/src/redturtle/prenotazioni/adapters/configure.zcml
--rw-r--r--   0 lucabel    (501) staff       (20)     4786 2024-03-19 08:48:10.000000 redturtle.prenotazioni-2.5.3/src/redturtle/prenotazioni/adapters/conflict.py
--rw-r--r--   0 lucabel    (501) staff       (20)     5037 2024-03-19 08:48:10.000000 redturtle.prenotazioni-2.5.3/src/redturtle/prenotazioni/adapters/ical.py
--rw-r--r--   0 lucabel    (501) staff       (20)      273 2024-03-19 08:48:10.000000 redturtle.prenotazioni-2.5.3/src/redturtle/prenotazioni/adapters/prenotazione_menu.py
--rw-r--r--   0 lucabel    (501) staff       (20)     9662 2024-03-19 08:48:10.000000 redturtle.prenotazioni-2.5.3/src/redturtle/prenotazioni/adapters/slot.py
--rw-r--r--   0 lucabel    (501) staff       (20)     8771 2024-03-19 08:48:10.000000 redturtle.prenotazioni-2.5.3/src/redturtle/prenotazioni/adapters/stringinterp.py
-drwxr-xr-x   0 lucabel    (501) staff       (20)        0 2024-03-19 08:48:10.757541 redturtle.prenotazioni-2.5.3/src/redturtle/prenotazioni/behaviors/
-drwxr-xr-x   0 lucabel    (501) staff       (20)        0 2024-03-19 08:48:10.758209 redturtle.prenotazioni-2.5.3/src/redturtle/prenotazioni/behaviors/booking_folder/
--rw-r--r--   0 lucabel    (501) staff       (20)        0 2024-03-19 08:48:10.000000 redturtle.prenotazioni-2.5.3/src/redturtle/prenotazioni/behaviors/booking_folder/__init__.py
--rw-r--r--   0 lucabel    (501) staff       (20)      563 2024-03-19 08:48:10.000000 redturtle.prenotazioni-2.5.3/src/redturtle/prenotazioni/behaviors/booking_folder/configure.zcml
--rw-r--r--   0 lucabel    (501) staff       (20)     1766 2024-03-19 08:48:10.000000 redturtle.prenotazioni-2.5.3/src/redturtle/prenotazioni/behaviors/booking_folder/contacts.py
-drwxr-xr-x   0 lucabel    (501) staff       (20)        0 2024-03-19 08:48:10.758821 redturtle.prenotazioni-2.5.3/src/redturtle/prenotazioni/behaviors/booking_folder/notifications/
--rw-r--r--   0 lucabel    (501) staff       (20)     1454 2024-03-19 08:48:10.000000 redturtle.prenotazioni-2.5.3/src/redturtle/prenotazioni/behaviors/booking_folder/notifications/__init__.py
-drwxr-xr-x   0 lucabel    (501) staff       (20)        0 2024-03-19 08:48:10.760268 redturtle.prenotazioni-2.5.3/src/redturtle/prenotazioni/behaviors/booking_folder/notifications/appio/
--rw-r--r--   0 lucabel    (501) staff       (20)    10220 2024-03-19 08:48:10.000000 redturtle.prenotazioni-2.5.3/src/redturtle/prenotazioni/behaviors/booking_folder/notifications/appio/__init__.py
--rw-r--r--   0 lucabel    (501) staff       (20)     4071 2024-03-19 08:48:10.000000 redturtle.prenotazioni-2.5.3/src/redturtle/prenotazioni/behaviors/booking_folder/notifications/appio/adapters.py
--rw-r--r--   0 lucabel    (501) staff       (20)     2364 2024-03-19 08:48:10.000000 redturtle.prenotazioni-2.5.3/src/redturtle/prenotazioni/behaviors/booking_folder/notifications/appio/configure.zcml
--rw-r--r--   0 lucabel    (501) staff       (20)     2592 2024-03-19 08:48:10.000000 redturtle.prenotazioni-2.5.3/src/redturtle/prenotazioni/behaviors/booking_folder/notifications/appio/events.py
--rw-r--r--   0 lucabel    (501) staff       (20)     3178 2024-03-19 08:48:10.000000 redturtle.prenotazioni-2.5.3/src/redturtle/prenotazioni/behaviors/booking_folder/notifications/appio/notfication_appio_message.py
--rw-r--r--   0 lucabel    (501) staff       (20)     1151 2024-03-19 08:48:10.000000 redturtle.prenotazioni-2.5.3/src/redturtle/prenotazioni/behaviors/booking_folder/notifications/appio/voc_service_keys.py
--rw-r--r--   0 lucabel    (501) staff       (20)      423 2024-03-19 08:48:10.000000 redturtle.prenotazioni-2.5.3/src/redturtle/prenotazioni/behaviors/booking_folder/notifications/configure.zcml
-drwxr-xr-x   0 lucabel    (501) staff       (20)        0 2024-03-19 08:48:10.761481 redturtle.prenotazioni-2.5.3/src/redturtle/prenotazioni/behaviors/booking_folder/notifications/email/
--rw-r--r--   0 lucabel    (501) staff       (20)     9647 2024-03-19 08:48:10.000000 redturtle.prenotazioni-2.5.3/src/redturtle/prenotazioni/behaviors/booking_folder/notifications/email/__init__.py
--rw-r--r--   0 lucabel    (501) staff       (20)     1607 2024-03-19 08:48:10.000000 redturtle.prenotazioni-2.5.3/src/redturtle/prenotazioni/behaviors/booking_folder/notifications/email/adapters.py
--rw-r--r--   0 lucabel    (501) staff       (20)     2284 2024-03-19 08:48:10.000000 redturtle.prenotazioni-2.5.3/src/redturtle/prenotazioni/behaviors/booking_folder/notifications/email/configure.zcml
--rw-r--r--   0 lucabel    (501) staff       (20)     3600 2024-03-19 08:48:10.000000 redturtle.prenotazioni-2.5.3/src/redturtle/prenotazioni/behaviors/booking_folder/notifications/email/events.py
--rw-r--r--   0 lucabel    (501) staff       (20)    11940 2024-03-19 08:48:10.000000 redturtle.prenotazioni-2.5.3/src/redturtle/prenotazioni/behaviors/booking_folder/notifications/email/notification_email_message.py
-drwxr-xr-x   0 lucabel    (501) staff       (20)        0 2024-03-19 08:48:10.762771 redturtle.prenotazioni-2.5.3/src/redturtle/prenotazioni/behaviors/booking_folder/notifications/sms/
--rw-r--r--   0 lucabel    (501) staff       (20)     5724 2024-03-19 08:48:10.000000 redturtle.prenotazioni-2.5.3/src/redturtle/prenotazioni/behaviors/booking_folder/notifications/sms/__init__.py
--rw-r--r--   0 lucabel    (501) staff       (20)     1115 2024-03-19 08:48:10.000000 redturtle.prenotazioni-2.5.3/src/redturtle/prenotazioni/behaviors/booking_folder/notifications/sms/adapters.py
--rw-r--r--   0 lucabel    (501) staff       (20)     1689 2024-03-19 08:48:10.000000 redturtle.prenotazioni-2.5.3/src/redturtle/prenotazioni/behaviors/booking_folder/notifications/sms/configure.zcml
--rw-r--r--   0 lucabel    (501) staff       (20)     2931 2024-03-19 08:48:10.000000 redturtle.prenotazioni-2.5.3/src/redturtle/prenotazioni/behaviors/booking_folder/notifications/sms/events.py
--rw-r--r--   0 lucabel    (501) staff       (20)     2216 2024-03-19 08:48:10.000000 redturtle.prenotazioni-2.5.3/src/redturtle/prenotazioni/behaviors/booking_folder/notifications/sms/message.py
--rw-r--r--   0 lucabel    (501) staff       (20)      284 2024-03-19 08:48:10.000000 redturtle.prenotazioni-2.5.3/src/redturtle/prenotazioni/behaviors/configure.zcml
-drwxr-xr-x   0 lucabel    (501) staff       (20)        0 2024-03-19 08:48:10.767513 redturtle.prenotazioni-2.5.3/src/redturtle/prenotazioni/browser/
--rw-r--r--   0 lucabel    (501) staff       (20)        0 2024-03-19 08:48:10.000000 redturtle.prenotazioni-2.5.3/src/redturtle/prenotazioni/browser/__init__.py
--rw-r--r--   0 lucabel    (501) staff       (20)     1817 2024-03-19 08:48:10.000000 redturtle.prenotazioni-2.5.3/src/redturtle/prenotazioni/browser/base.py
--rw-r--r--   0 lucabel    (501) staff       (20)     7331 2024-03-19 08:48:10.000000 redturtle.prenotazioni-2.5.3/src/redturtle/prenotazioni/browser/configure.zcml
--rw-r--r--   0 lucabel    (501) staff       (20)      655 2024-03-19 08:48:10.000000 redturtle.prenotazioni-2.5.3/src/redturtle/prenotazioni/browser/custom_radio_input.pt
--rw-r--r--   0 lucabel    (501) staff       (20)     5709 2024-03-19 08:48:10.000000 redturtle.prenotazioni-2.5.3/src/redturtle/prenotazioni/browser/delete_reservation.py
--rw-r--r--   0 lucabel    (501) staff       (20)      673 2024-03-19 08:48:10.000000 redturtle.prenotazioni-2.5.3/src/redturtle/prenotazioni/browser/folderfactories.py
--rw-r--r--   0 lucabel    (501) staff       (20)      155 2024-03-19 08:48:10.000000 redturtle.prenotazioni-2.5.3/src/redturtle/prenotazioni/browser/interfaces.py
-drwxr-xr-x   0 lucabel    (501) staff       (20)        0 2024-03-19 08:48:10.767827 redturtle.prenotazioni-2.5.3/src/redturtle/prenotazioni/browser/overrides/
--rw-r--r--   0 lucabel    (501) staff       (20)        0 2024-03-19 08:48:10.000000 redturtle.prenotazioni-2.5.3/src/redturtle/prenotazioni/browser/overrides/.gitkeep
--rw-r--r--   0 lucabel    (501) staff       (20)     3169 2024-03-19 08:48:10.000000 redturtle.prenotazioni-2.5.3/src/redturtle/prenotazioni/browser/prenotazione.py
--rw-r--r--   0 lucabel    (501) staff       (20)    10057 2024-03-19 08:48:10.000000 redturtle.prenotazioni-2.5.3/src/redturtle/prenotazioni/browser/prenotazione_add.py
--rw-r--r--   0 lucabel    (501) staff       (20)     5252 2024-03-19 08:48:10.000000 redturtle.prenotazioni-2.5.3/src/redturtle/prenotazioni/browser/prenotazione_move.py
--rw-r--r--   0 lucabel    (501) staff       (20)     2721 2024-03-19 08:48:10.000000 redturtle.prenotazioni-2.5.3/src/redturtle/prenotazioni/browser/prenotazione_print.py
--rw-r--r--   0 lucabel    (501) staff       (20)    37170 2024-03-19 08:48:10.000000 redturtle.prenotazioni-2.5.3/src/redturtle/prenotazioni/browser/prenotazioni_context_state.py
--rw-r--r--   0 lucabel    (501) staff       (20)     1735 2024-03-19 08:48:10.000000 redturtle.prenotazioni-2.5.3/src/redturtle/prenotazioni/browser/prenotazioni_portal_state.py
--rw-r--r--   0 lucabel    (501) staff       (20)    13800 2024-03-19 08:48:10.000000 redturtle.prenotazioni-2.5.3/src/redturtle/prenotazioni/browser/prenotazioni_search.py
-drwxr-xr-x   0 lucabel    (501) staff       (20)        0 2024-03-19 08:48:10.769816 redturtle.prenotazioni-2.5.3/src/redturtle/prenotazioni/browser/static/
--rw-r--r--   0 lucabel    (501) staff       (20)        0 2024-03-19 08:48:10.000000 redturtle.prenotazioni-2.5.3/src/redturtle/prenotazioni/browser/static/.gitkeep
--rw-r--r--   0 lucabel    (501) staff       (20)      364 2024-03-19 08:48:10.000000 redturtle.prenotazioni-2.5.3/src/redturtle/prenotazioni/browser/static/calendar-add.png
--rw-r--r--   0 lucabel    (501) staff       (20)      503 2024-03-19 08:48:10.000000 redturtle.prenotazioni-2.5.3/src/redturtle/prenotazioni/browser/static/calendar-icon.png
--rw-r--r--   0 lucabel    (501) staff       (20)      266 2024-03-19 08:48:10.000000 redturtle.prenotazioni-2.5.3/src/redturtle/prenotazioni/browser/static/cross-icon.png
--rw-r--r--   0 lucabel    (501) staff       (20)     9794 2024-03-19 08:48:10.000000 redturtle.prenotazioni-2.5.3/src/redturtle/prenotazioni/browser/static/redturtle-reservation.css
--rw-r--r--   0 lucabel    (501) staff       (20)     1600 2024-03-19 08:48:10.000000 redturtle.prenotazioni-2.5.3/src/redturtle/prenotazioni/browser/static/redturtle-reservation.js
--rw-r--r--   0 lucabel    (501) staff       (20)      922 2024-03-19 08:48:10.000000 redturtle.prenotazioni-2.5.3/src/redturtle/prenotazioni/browser/static/times-solid.png
-drwxr-xr-x   0 lucabel    (501) staff       (20)        0 2024-03-19 08:48:10.737597 redturtle.prenotazioni-2.5.3/src/redturtle/prenotazioni/browser/static/widget/
-drwxr-xr-x   0 lucabel    (501) staff       (20)        0 2024-03-19 08:48:10.737470 redturtle.prenotazioni-2.5.3/src/redturtle/prenotazioni/browser/static/widget/dist/
-drwxr-xr-x   0 lucabel    (501) staff       (20)        0 2024-03-19 08:48:10.771121 redturtle.prenotazioni-2.5.3/src/redturtle/prenotazioni/browser/static/widget/dist/prod/
--rw-r--r--   0 lucabel    (501) staff       (20)     3239 2024-03-19 08:48:10.000000 redturtle.prenotazioni-2.5.3/src/redturtle/prenotazioni/browser/static/widget/dist/prod/main.css
--rw-r--r--   0 lucabel    (501) staff       (20)     3808 2024-03-19 08:48:10.000000 redturtle.prenotazioni-2.5.3/src/redturtle/prenotazioni/browser/static/widget/dist/prod/main.css.map
--rw-r--r--   0 lucabel    (501) staff       (20)   349785 2024-03-19 08:48:10.000000 redturtle.prenotazioni-2.5.3/src/redturtle/prenotazioni/browser/static/widget/dist/prod/main.js
--rw-r--r--   0 lucabel    (501) staff       (20)      148 2024-03-19 08:48:10.000000 redturtle.prenotazioni-2.5.3/src/redturtle/prenotazioni/browser/static/widget/dist/prod/main.js.map
-drwxr-xr-x   0 lucabel    (501) staff       (20)        0 2024-03-19 08:48:10.771359 redturtle.prenotazioni-2.5.3/src/redturtle/prenotazioni/browser/static/widget/js/
-drwxr-xr-x   0 lucabel    (501) staff       (20)        0 2024-03-19 08:48:10.771646 redturtle.prenotazioni-2.5.3/src/redturtle/prenotazioni/browser/static/widget/js/WidgetContainer/
--rw-r--r--   0 lucabel    (501) staff       (20)     5095 2024-03-19 08:48:10.000000 redturtle.prenotazioni-2.5.3/src/redturtle/prenotazioni/browser/static/widget/js/WidgetContainer/index.js
-drwxr-xr-x   0 lucabel    (501) staff       (20)        0 2024-03-19 08:48:10.772334 redturtle.prenotazioni-2.5.3/src/redturtle/prenotazioni/browser/static/widget/js/WidgetDataContainer/
--rw-r--r--   0 lucabel    (501) staff       (20)     4705 2024-03-19 08:48:10.000000 redturtle.prenotazioni-2.5.3/src/redturtle/prenotazioni/browser/static/widget/js/WidgetDataContainer/index.js
--rw-r--r--   0 lucabel    (501) staff       (20)     1059 2024-03-19 08:48:10.000000 redturtle.prenotazioni-2.5.3/src/redturtle/prenotazioni/browser/static/widget/js/WidgetDataContainer/index.less
-drwxr-xr-x   0 lucabel    (501) staff       (20)        0 2024-03-19 08:48:10.775444 redturtle.prenotazioni-2.5.3/src/redturtle/prenotazioni/browser/static/widget/js/fields/
--rw-r--r--   0 lucabel    (501) staff       (20)     3010 2024-03-19 08:48:10.000000 redturtle.prenotazioni-2.5.3/src/redturtle/prenotazioni/browser/static/widget/js/fields/DaysTableField.js
--rw-r--r--   0 lucabel    (501) staff       (20)      204 2024-03-19 08:48:10.000000 redturtle.prenotazioni-2.5.3/src/redturtle/prenotazioni/browser/static/widget/js/fields/DaysTableField.less
--rw-r--r--   0 lucabel    (501) staff       (20)     2874 2024-03-19 08:48:10.000000 redturtle.prenotazioni-2.5.3/src/redturtle/prenotazioni/browser/static/widget/js/fields/GatesField.js
--rw-r--r--   0 lucabel    (501) staff       (20)      401 2024-03-19 08:48:10.000000 redturtle.prenotazioni-2.5.3/src/redturtle/prenotazioni/browser/static/widget/js/fields/GatesField.less
--rw-r--r--   0 lucabel    (501) staff       (20)     1888 2024-03-19 08:48:10.000000 redturtle.prenotazioni-2.5.3/src/redturtle/prenotazioni/browser/static/widget/js/fields/IntervalSelectorField.js
--rw-r--r--   0 lucabel    (501) staff       (20)      314 2024-03-19 08:48:10.000000 redturtle.prenotazioni-2.5.3/src/redturtle/prenotazioni/browser/static/widget/js/fields/IntervalSelectorField.less
--rw-r--r--   0 lucabel    (501) staff       (20)     4187 2024-03-19 08:48:10.000000 redturtle.prenotazioni-2.5.3/src/redturtle/prenotazioni/browser/static/widget/js/fields/PauseTableField.js
--rw-r--r--   0 lucabel    (501) staff       (20)      337 2024-03-19 08:48:10.000000 redturtle.prenotazioni-2.5.3/src/redturtle/prenotazioni/browser/static/widget/js/fields/PauseTableField.less
--rw-r--r--   0 lucabel    (501) staff       (20)     1745 2024-03-19 08:48:10.000000 redturtle.prenotazioni-2.5.3/src/redturtle/prenotazioni/browser/static/widget/js/fields/SelectField.js
--rw-r--r--   0 lucabel    (501) staff       (20)      961 2024-03-19 08:48:10.000000 redturtle.prenotazioni-2.5.3/src/redturtle/prenotazioni/browser/static/widget/js/fields/TextLineField.js
--rw-r--r--   0 lucabel    (501) staff       (20)     1261 2024-03-19 08:48:10.000000 redturtle.prenotazioni-2.5.3/src/redturtle/prenotazioni/browser/static/widget/js/index.js
-drwxr-xr-x   0 lucabel    (501) staff       (20)        0 2024-03-19 08:48:10.775979 redturtle.prenotazioni-2.5.3/src/redturtle/prenotazioni/browser/static/widget/js/utils/
--rw-r--r--   0 lucabel    (501) staff       (20)      941 2024-03-19 08:48:10.000000 redturtle.prenotazioni-2.5.3/src/redturtle/prenotazioni/browser/static/widget/js/utils/i18n.js
--rw-r--r--   0 lucabel    (501) staff       (20)      298 2024-03-19 08:48:10.000000 redturtle.prenotazioni-2.5.3/src/redturtle/prenotazioni/browser/static/widget/js/utils/widgetContext.js
-drwxr-xr-x   0 lucabel    (501) staff       (20)        0 2024-03-19 08:48:10.777161 redturtle.prenotazioni-2.5.3/src/redturtle/prenotazioni/browser/stats/
--rw-r--r--   0 lucabel    (501) staff       (20)       24 2024-03-19 08:48:10.000000 redturtle.prenotazioni-2.5.3/src/redturtle/prenotazioni/browser/stats/__init__.py
--rw-r--r--   0 lucabel    (501) staff       (20)      698 2024-03-19 08:48:10.000000 redturtle.prenotazioni-2.5.3/src/redturtle/prenotazioni/browser/stats/booking_stats.pt
--rw-r--r--   0 lucabel    (501) staff       (20)     3863 2024-03-19 08:48:10.000000 redturtle.prenotazioni-2.5.3/src/redturtle/prenotazioni/browser/stats/booking_stats.py
--rw-r--r--   0 lucabel    (501) staff       (20)      575 2024-03-19 08:48:10.000000 redturtle.prenotazioni-2.5.3/src/redturtle/prenotazioni/browser/stats/configure.zcml
-drwxr-xr-x   0 lucabel    (501) staff       (20)        0 2024-03-19 08:48:10.781293 redturtle.prenotazioni-2.5.3/src/redturtle/prenotazioni/browser/templates/
--rw-r--r--   0 lucabel    (501) staff       (20)     2836 2024-03-19 08:48:10.000000 redturtle.prenotazioni-2.5.3/src/redturtle/prenotazioni/browser/templates/booking_type_radio_widget.pt
--rw-r--r--   0 lucabel    (501) staff       (20)     1518 2024-03-19 08:48:10.000000 redturtle.prenotazioni-2.5.3/src/redturtle/prenotazioni/browser/templates/custom_dgf_input.pt
--rw-r--r--   0 lucabel    (501) staff       (20)     4828 2024-03-19 08:48:10.000000 redturtle.prenotazioni-2.5.3/src/redturtle/prenotazioni/browser/templates/delete_reservation.pt
--rw-r--r--   0 lucabel    (501) staff       (20)     2417 2024-03-19 08:48:10.000000 redturtle.prenotazioni-2.5.3/src/redturtle/prenotazioni/browser/templates/manager_notification_mail.pt
--rw-r--r--   0 lucabel    (501) staff       (20)       48 2024-03-19 08:48:10.000000 redturtle.prenotazioni-2.5.3/src/redturtle/prenotazioni/browser/templates/nofollow.pt
--rw-r--r--   0 lucabel    (501) staff       (20)     7714 2024-03-19 08:48:10.000000 redturtle.prenotazioni-2.5.3/src/redturtle/prenotazioni/browser/templates/prenotazione.pt
--rw-r--r--   0 lucabel    (501) staff       (20)     9592 2024-03-19 08:48:10.000000 redturtle.prenotazioni-2.5.3/src/redturtle/prenotazioni/browser/templates/prenotazione_add.pt
--rw-r--r--   0 lucabel    (501) staff       (20)    16384 2024-03-19 08:48:10.000000 redturtle.prenotazioni-2.5.3/src/redturtle/prenotazioni/browser/templates/prenotazione_macros.pt
--rw-r--r--   0 lucabel    (501) staff       (20)     2227 2024-03-19 08:48:10.000000 redturtle.prenotazioni-2.5.3/src/redturtle/prenotazioni/browser/templates/prenotazione_move.pt
--rw-r--r--   0 lucabel    (501) staff       (20)     5299 2024-03-19 08:48:10.000000 redturtle.prenotazioni-2.5.3/src/redturtle/prenotazioni/browser/templates/prenotazione_print.pt
--rw-r--r--   0 lucabel    (501) staff       (20)     5241 2024-03-19 08:48:10.000000 redturtle.prenotazioni-2.5.3/src/redturtle/prenotazioni/browser/templates/prenotazioni_search.pt
--rw-r--r--   0 lucabel    (501) staff       (20)     1858 2024-03-19 08:48:10.000000 redturtle.prenotazioni-2.5.3/src/redturtle/prenotazioni/browser/templates/week.pt
--rw-r--r--   0 lucabel    (501) staff       (20)      362 2024-03-19 08:48:10.000000 redturtle.prenotazioni-2.5.3/src/redturtle/prenotazioni/browser/templates/week_table_overrides_widget_input.pt
-drwxr-xr-x   0 lucabel    (501) staff       (20)        0 2024-03-19 08:48:10.782086 redturtle.prenotazioni-2.5.3/src/redturtle/prenotazioni/browser/utilities/
--rw-r--r--   0 lucabel    (501) staff       (20)        0 2024-03-19 08:48:10.000000 redturtle.prenotazioni-2.5.3/src/redturtle/prenotazioni/browser/utilities/__init__.py
--rw-r--r--   0 lucabel    (501) staff       (20)      494 2024-03-19 08:48:10.000000 redturtle.prenotazioni-2.5.3/src/redturtle/prenotazioni/browser/utilities/configure.zcml
--rw-r--r--   0 lucabel    (501) staff       (20)     1676 2024-03-19 08:48:10.000000 redturtle.prenotazioni-2.5.3/src/redturtle/prenotazioni/browser/utilities/notify_upcoming_bookings.py
--rw-r--r--   0 lucabel    (501) staff       (20)     8087 2024-03-19 08:48:10.000000 redturtle.prenotazioni-2.5.3/src/redturtle/prenotazioni/browser/vacations.py
--rw-r--r--   0 lucabel    (501) staff       (20)     1524 2024-03-19 08:48:10.000000 redturtle.prenotazioni-2.5.3/src/redturtle/prenotazioni/browser/viewlets.py
--rw-r--r--   0 lucabel    (501) staff       (20)    10867 2024-03-19 08:48:10.000000 redturtle.prenotazioni-2.5.3/src/redturtle/prenotazioni/browser/week.py
--rw-r--r--   0 lucabel    (501) staff       (20)     1193 2024-03-19 08:48:10.000000 redturtle.prenotazioni-2.5.3/src/redturtle/prenotazioni/browser/widget.py
--rw-r--r--   0 lucabel    (501) staff       (20)     6310 2024-03-19 08:48:10.000000 redturtle.prenotazioni-2.5.3/src/redturtle/prenotazioni/browser/z3c_custom_widget.py
--rw-r--r--   0 lucabel    (501) staff       (20)      485 2024-03-19 08:48:10.000000 redturtle.prenotazioni-2.5.3/src/redturtle/prenotazioni/config.py
--rw-r--r--   0 lucabel    (501) staff       (20)     2049 2024-03-19 08:48:10.000000 redturtle.prenotazioni-2.5.3/src/redturtle/prenotazioni/configure.zcml
-drwxr-xr-x   0 lucabel    (501) staff       (20)        0 2024-03-19 08:48:10.785189 redturtle.prenotazioni-2.5.3/src/redturtle/prenotazioni/content/
--rw-r--r--   0 lucabel    (501) staff       (20)       24 2024-03-19 08:48:10.000000 redturtle.prenotazioni-2.5.3/src/redturtle/prenotazioni/content/__init__.py
--rw-r--r--   0 lucabel    (501) staff       (20)      111 2024-03-19 08:48:10.000000 redturtle.prenotazioni-2.5.3/src/redturtle/prenotazioni/content/booking_type.py
--rw-r--r--   0 lucabel    (501) staff       (20)     1537 2024-03-19 08:48:10.000000 redturtle.prenotazioni-2.5.3/src/redturtle/prenotazioni/content/pause.py
--rw-r--r--   0 lucabel    (501) staff       (20)     7504 2024-03-19 08:48:10.000000 redturtle.prenotazioni-2.5.3/src/redturtle/prenotazioni/content/prenotazione.py
--rw-r--r--   0 lucabel    (501) staff       (20)     1251 2024-03-19 08:48:10.000000 redturtle.prenotazioni-2.5.3/src/redturtle/prenotazioni/content/prenotazione_type.py
--rw-r--r--   0 lucabel    (501) staff       (20)      367 2024-03-19 08:48:10.000000 redturtle.prenotazioni-2.5.3/src/redturtle/prenotazioni/content/prenotazioni_day.py
--rw-r--r--   0 lucabel    (501) staff       (20)    18932 2024-03-19 08:48:10.000000 redturtle.prenotazioni-2.5.3/src/redturtle/prenotazioni/content/prenotazioni_folder.py
--rw-r--r--   0 lucabel    (501) staff       (20)      371 2024-03-19 08:48:10.000000 redturtle.prenotazioni-2.5.3/src/redturtle/prenotazioni/content/prenotazioni_week.py
--rw-r--r--   0 lucabel    (501) staff       (20)      371 2024-03-19 08:48:10.000000 redturtle.prenotazioni-2.5.3/src/redturtle/prenotazioni/content/prenotazioni_year.py
--rw-r--r--   0 lucabel    (501) staff       (20)     8518 2024-03-19 08:48:10.000000 redturtle.prenotazioni-2.5.3/src/redturtle/prenotazioni/content/validators.py
-drwxr-xr-x   0 lucabel    (501) staff       (20)        0 2024-03-19 08:48:10.786450 redturtle.prenotazioni-2.5.3/src/redturtle/prenotazioni/demo/
--rw-r--r--   0 lucabel    (501) staff       (20)       77 2024-03-19 08:48:10.000000 redturtle.prenotazioni-2.5.3/src/redturtle/prenotazioni/demo/__init__.py
--rw-r--r--   0 lucabel    (501) staff       (20)     1088 2024-03-19 08:48:10.000000 redturtle.prenotazioni-2.5.3/src/redturtle/prenotazioni/demo/configure.zcml
--rw-r--r--   0 lucabel    (501) staff       (20)      227 2024-03-19 08:48:10.000000 redturtle.prenotazioni-2.5.3/src/redturtle/prenotazioni/demo/interfaces.py
-drwxr-xr-x   0 lucabel    (501) staff       (20)        0 2024-03-19 08:48:10.739084 redturtle.prenotazioni-2.5.3/src/redturtle/prenotazioni/demo/profiles/
-drwxr-xr-x   0 lucabel    (501) staff       (20)        0 2024-03-19 08:48:10.786990 redturtle.prenotazioni-2.5.3/src/redturtle/prenotazioni/demo/profiles/default/
--rw-r--r--   0 lucabel    (501) staff       (20)      208 2024-03-19 08:48:10.000000 redturtle.prenotazioni-2.5.3/src/redturtle/prenotazioni/demo/profiles/default/browserlayer.xml
--rw-r--r--   0 lucabel    (501) staff       (20)       88 2024-03-19 08:48:10.000000 redturtle.prenotazioni-2.5.3/src/redturtle/prenotazioni/demo/profiles/default/metadata.xml
-drwxr-xr-x   0 lucabel    (501) staff       (20)        0 2024-03-19 08:48:10.787232 redturtle.prenotazioni-2.5.3/src/redturtle/prenotazioni/demo/profiles/uninstall/
--rw-r--r--   0 lucabel    (501) staff       (20)      133 2024-03-19 08:48:10.000000 redturtle.prenotazioni-2.5.3/src/redturtle/prenotazioni/demo/profiles/uninstall/browserlayer.xml
--rw-r--r--   0 lucabel    (501) staff       (20)      630 2024-03-19 08:48:10.000000 redturtle.prenotazioni-2.5.3/src/redturtle/prenotazioni/demo/setuphandlers.py
--rw-r--r--   0 lucabel    (501) staff       (20)     1347 2024-03-19 08:48:10.000000 redturtle.prenotazioni-2.5.3/src/redturtle/prenotazioni/demo/smsdemo.py
-drwxr-xr-x   0 lucabel    (501) staff       (20)        0 2024-03-19 08:48:10.788544 redturtle.prenotazioni-2.5.3/src/redturtle/prenotazioni/events/
--rw-r--r--   0 lucabel    (501) staff       (20)      270 2024-03-19 08:48:10.000000 redturtle.prenotazioni-2.5.3/src/redturtle/prenotazioni/events/__init__.py
--rw-r--r--   0 lucabel    (501) staff       (20)     1615 2024-03-19 08:48:10.000000 redturtle.prenotazioni-2.5.3/src/redturtle/prenotazioni/events/configure.zcml
--rw-r--r--   0 lucabel    (501) staff       (20)     2128 2024-03-19 08:48:10.000000 redturtle.prenotazioni-2.5.3/src/redturtle/prenotazioni/events/events_logger.py
--rw-r--r--   0 lucabel    (501) staff       (20)     1907 2024-03-19 08:48:10.000000 redturtle.prenotazioni-2.5.3/src/redturtle/prenotazioni/events/prenotazione.py
--rw-r--r--   0 lucabel    (501) staff       (20)     1189 2024-03-19 08:48:10.000000 redturtle.prenotazioni-2.5.3/src/redturtle/prenotazioni/events/prenotazioni_folder.py
-drwxr-xr-x   0 lucabel    (501) staff       (20)        0 2024-03-19 08:48:10.789056 redturtle.prenotazioni-2.5.3/src/redturtle/prenotazioni/exceptions/
--rw-r--r--   0 lucabel    (501) staff       (20)      129 2024-03-19 08:48:10.000000 redturtle.prenotazioni-2.5.3/src/redturtle/prenotazioni/exceptions/__init__.py
--rw-r--r--   0 lucabel    (501) staff       (20)      712 2024-03-19 08:48:10.000000 redturtle.prenotazioni-2.5.3/src/redturtle/prenotazioni/exceptions/booker.py
-drwxr-xr-x   0 lucabel    (501) staff       (20)        0 2024-03-19 08:48:10.789800 redturtle.prenotazioni-2.5.3/src/redturtle/prenotazioni/indexers/
--rw-r--r--   0 lucabel    (501) staff       (20)       24 2024-03-19 08:48:10.000000 redturtle.prenotazioni-2.5.3/src/redturtle/prenotazioni/indexers/__init__.py
--rw-r--r--   0 lucabel    (501) staff       (20)      476 2024-03-19 08:48:10.000000 redturtle.prenotazioni-2.5.3/src/redturtle/prenotazioni/indexers/configure.zcml
--rw-r--r--   0 lucabel    (501) staff       (20)     1410 2024-03-19 08:48:10.000000 redturtle.prenotazioni-2.5.3/src/redturtle/prenotazioni/indexers/prenotazione.py
--rw-r--r--   0 lucabel    (501) staff       (20)     1445 2024-03-19 08:48:10.000000 redturtle.prenotazioni-2.5.3/src/redturtle/prenotazioni/interfaces.py
-drwxr-xr-x   0 lucabel    (501) staff       (20)        0 2024-03-19 08:48:10.793086 redturtle.prenotazioni-2.5.3/src/redturtle/prenotazioni/io_tools/
--rw-r--r--   0 lucabel    (501) staff       (20)     5302 2024-03-19 08:48:10.000000 redturtle.prenotazioni-2.5.3/src/redturtle/prenotazioni/io_tools/README.md
--rw-r--r--   0 lucabel    (501) staff       (20)      207 2024-03-19 08:48:10.000000 redturtle.prenotazioni-2.5.3/src/redturtle/prenotazioni/io_tools/__init__.py
--rw-r--r--   0 lucabel    (501) staff       (20)     9443 2024-03-19 08:48:10.000000 redturtle.prenotazioni-2.5.3/src/redturtle/prenotazioni/io_tools/api.py
--rw-r--r--   0 lucabel    (501) staff       (20)     1035 2024-03-19 08:48:10.000000 redturtle.prenotazioni-2.5.3/src/redturtle/prenotazioni/io_tools/cli.py
--rw-r--r--   0 lucabel    (501) staff       (20)    16384 2024-03-19 08:48:10.000000 redturtle.prenotazioni-2.5.3/src/redturtle/prenotazioni/io_tools/io.db
--rw-r--r--   0 lucabel    (501) staff       (20)       45 2024-03-19 08:48:10.000000 redturtle.prenotazioni-2.5.3/src/redturtle/prenotazioni/io_tools/io_tools.py
--rw-r--r--   0 lucabel    (501) staff       (20)     1945 2024-03-19 08:48:10.000000 redturtle.prenotazioni-2.5.3/src/redturtle/prenotazioni/io_tools/monkey.py
--rw-r--r--   0 lucabel    (501) staff       (20)     2833 2024-03-19 08:48:10.000000 redturtle.prenotazioni-2.5.3/src/redturtle/prenotazioni/io_tools/rdbms.py
--rw-r--r--   0 lucabel    (501) staff       (20)    27521 2024-03-19 08:48:10.000000 redturtle.prenotazioni-2.5.3/src/redturtle/prenotazioni/io_tools/spec.yaml
--rw-r--r--   0 lucabel    (501) staff       (20)      961 2024-03-19 08:48:10.000000 redturtle.prenotazioni-2.5.3/src/redturtle/prenotazioni/io_tools/storage.py
-drwxr-xr-x   0 lucabel    (501) staff       (20)        0 2024-03-19 08:48:10.794252 redturtle.prenotazioni-2.5.3/src/redturtle/prenotazioni/locales/
-drwxr-xr-x   0 lucabel    (501) staff       (20)        0 2024-03-19 08:48:10.740075 redturtle.prenotazioni-2.5.3/src/redturtle/prenotazioni/locales/en/
-drwxr-xr-x   0 lucabel    (501) staff       (20)        0 2024-03-19 08:48:10.794485 redturtle.prenotazioni-2.5.3/src/redturtle/prenotazioni/locales/en/LC_MESSAGES/
--rw-r--r--   0 lucabel    (501) staff       (20)    56619 2024-03-19 08:48:10.000000 redturtle.prenotazioni-2.5.3/src/redturtle/prenotazioni/locales/en/LC_MESSAGES/redturtle.prenotazioni.po
-drwxr-xr-x   0 lucabel    (501) staff       (20)        0 2024-03-19 08:48:10.740527 redturtle.prenotazioni-2.5.3/src/redturtle/prenotazioni/locales/it/
-drwxr-xr-x   0 lucabel    (501) staff       (20)        0 2024-03-19 08:48:10.795035 redturtle.prenotazioni-2.5.3/src/redturtle/prenotazioni/locales/it/LC_MESSAGES/
--rw-r--r--   0 lucabel    (501) staff       (20)      623 2024-03-19 08:48:10.000000 redturtle.prenotazioni-2.5.3/src/redturtle/prenotazioni/locales/it/LC_MESSAGES/plone.po
--rw-r--r--   0 lucabel    (501) staff       (20)    73109 2024-03-19 08:48:10.000000 redturtle.prenotazioni-2.5.3/src/redturtle/prenotazioni/locales/it/LC_MESSAGES/redturtle.prenotazioni.po
--rw-r--r--   0 lucabel    (501) staff       (20)      830 2024-03-19 08:48:10.000000 redturtle.prenotazioni-2.5.3/src/redturtle/prenotazioni/locales/manual.pot
--rw-r--r--   0 lucabel    (501) staff       (20)    56728 2024-03-19 08:48:10.000000 redturtle.prenotazioni-2.5.3/src/redturtle/prenotazioni/locales/redturtle.prenotazioni.pot
--rw-r--r--   0 lucabel    (501) staff       (20)     1618 2024-03-19 08:48:10.000000 redturtle.prenotazioni-2.5.3/src/redturtle/prenotazioni/locales/update.py
--rwxr-xr-x   0 lucabel    (501) staff       (20)      521 2024-03-19 08:48:10.000000 redturtle.prenotazioni-2.5.3/src/redturtle/prenotazioni/locales/update.sh
-drwxr-xr-x   0 lucabel    (501) staff       (20)        0 2024-03-19 08:48:10.795556 redturtle.prenotazioni-2.5.3/src/redturtle/prenotazioni/monkeypatcher/
--rw-r--r--   0 lucabel    (501) staff       (20)        0 2024-03-19 08:48:10.000000 redturtle.prenotazioni-2.5.3/src/redturtle/prenotazioni/monkeypatcher/__init__.py
--rw-r--r--   0 lucabel    (501) staff       (20)      499 2024-03-19 08:48:10.000000 redturtle.prenotazioni-2.5.3/src/redturtle/prenotazioni/monkeypatcher/configure.zcml
--rw-r--r--   0 lucabel    (501) staff       (20)     1565 2024-03-19 08:48:10.000000 redturtle.prenotazioni-2.5.3/src/redturtle/prenotazioni/permissions.zcml
--rw-r--r--   0 lucabel    (501) staff       (20)      507 2024-03-19 08:48:10.000000 redturtle.prenotazioni-2.5.3/src/redturtle/prenotazioni/prenotazione_event.py
-drwxr-xr-x   0 lucabel    (501) staff       (20)        0 2024-03-19 08:48:10.742855 redturtle.prenotazioni-2.5.3/src/redturtle/prenotazioni/profiles/
-drwxr-xr-x   0 lucabel    (501) staff       (20)        0 2024-03-19 08:48:10.797731 redturtle.prenotazioni-2.5.3/src/redturtle/prenotazioni/profiles/default/
--rw-r--r--   0 lucabel    (501) staff       (20)     2656 2024-03-19 08:48:10.000000 redturtle.prenotazioni-2.5.3/src/redturtle/prenotazioni/profiles/default/actions.xml
--rw-r--r--   0 lucabel    (501) staff       (20)      185 2024-03-19 08:48:10.000000 redturtle.prenotazioni-2.5.3/src/redturtle/prenotazioni/profiles/default/browserlayer.xml
--rw-r--r--   0 lucabel    (501) staff       (20)      349 2024-03-19 08:48:10.000000 redturtle.prenotazioni-2.5.3/src/redturtle/prenotazioni/profiles/default/catalog.xml
--rw-r--r--   0 lucabel    (501) staff       (20)       71 2024-03-19 08:48:10.000000 redturtle.prenotazioni-2.5.3/src/redturtle/prenotazioni/profiles/default/contentrules.xml
--rw-r--r--   0 lucabel    (501) staff       (20)      325 2024-03-19 08:48:10.000000 redturtle.prenotazioni-2.5.3/src/redturtle/prenotazioni/profiles/default/metadata.xml
-drwxr-xr-x   0 lucabel    (501) staff       (20)        0 2024-03-19 08:48:10.798496 redturtle.prenotazioni-2.5.3/src/redturtle/prenotazioni/profiles/default/registry/
--rw-r--r--   0 lucabel    (501) staff       (20)     5140 2024-03-19 08:48:10.000000 redturtle.prenotazioni-2.5.3/src/redturtle/prenotazioni/profiles/default/registry/caching.xml
--rw-r--r--   0 lucabel    (501) staff       (20)     2015 2024-03-19 08:48:10.000000 redturtle.prenotazioni-2.5.3/src/redturtle/prenotazioni/profiles/default/registry/resources.xml
--rw-r--r--   0 lucabel    (501) staff       (20)     1001 2024-03-19 08:48:10.000000 redturtle.prenotazioni-2.5.3/src/redturtle/prenotazioni/profiles/default/registry/settings.xml
--rw-r--r--   0 lucabel    (501) staff       (20)     3277 2024-03-19 08:48:10.000000 redturtle.prenotazioni-2.5.3/src/redturtle/prenotazioni/profiles/default/rolemap.xml
--rw-r--r--   0 lucabel    (501) staff       (20)      277 2024-03-19 08:48:10.000000 redturtle.prenotazioni-2.5.3/src/redturtle/prenotazioni/profiles/default/sharing.xml
-drwxr-xr-x   0 lucabel    (501) staff       (20)        0 2024-03-19 08:48:10.800148 redturtle.prenotazioni-2.5.3/src/redturtle/prenotazioni/profiles/default/types/
--rw-r--r--   0 lucabel    (501) staff       (20)     3607 2024-03-19 08:48:10.000000 redturtle.prenotazioni-2.5.3/src/redturtle/prenotazioni/profiles/default/types/Prenotazione.xml
--rw-r--r--   0 lucabel    (501) staff       (20)     2983 2024-03-19 08:48:10.000000 redturtle.prenotazioni-2.5.3/src/redturtle/prenotazioni/profiles/default/types/PrenotazioneType.xml
--rw-r--r--   0 lucabel    (501) staff       (20)     3861 2024-03-19 08:48:10.000000 redturtle.prenotazioni-2.5.3/src/redturtle/prenotazioni/profiles/default/types/PrenotazioniDay.xml
--rw-r--r--   0 lucabel    (501) staff       (20)     3257 2024-03-19 08:48:10.000000 redturtle.prenotazioni-2.5.3/src/redturtle/prenotazioni/profiles/default/types/PrenotazioniFolder.xml
--rw-r--r--   0 lucabel    (501) staff       (20)     3845 2024-03-19 08:48:10.000000 redturtle.prenotazioni-2.5.3/src/redturtle/prenotazioni/profiles/default/types/PrenotazioniWeek.xml
--rw-r--r--   0 lucabel    (501) staff       (20)     3846 2024-03-19 08:48:10.000000 redturtle.prenotazioni-2.5.3/src/redturtle/prenotazioni/profiles/default/types/PrenotazioniYear.xml
--rw-r--r--   0 lucabel    (501) staff       (20)      713 2024-03-19 08:48:10.000000 redturtle.prenotazioni-2.5.3/src/redturtle/prenotazioni/profiles/default/types.xml
-drwxr-xr-x   0 lucabel    (501) staff       (20)        0 2024-03-19 08:48:10.741861 redturtle.prenotazioni-2.5.3/src/redturtle/prenotazioni/profiles/default/workflows/
-drwxr-xr-x   0 lucabel    (501) staff       (20)        0 2024-03-19 08:48:10.800688 redturtle.prenotazioni-2.5.3/src/redturtle/prenotazioni/profiles/default/workflows/prenotazioni_workflow/
--rw-r--r--   0 lucabel    (501) staff       (20)    12711 2024-03-19 08:48:10.000000 redturtle.prenotazioni-2.5.3/src/redturtle/prenotazioni/profiles/default/workflows/prenotazioni_workflow/definition.xml
-drwxr-xr-x   0 lucabel    (501) staff       (20)        0 2024-03-19 08:48:10.801088 redturtle.prenotazioni-2.5.3/src/redturtle/prenotazioni/profiles/default/workflows/prenotazionifolder_workflow/
--rw-r--r--   0 lucabel    (501) staff       (20)     8877 2024-03-19 08:48:10.000000 redturtle.prenotazioni-2.5.3/src/redturtle/prenotazioni/profiles/default/workflows/prenotazionifolder_workflow/definition.xml
--rw-r--r--   0 lucabel    (501) staff       (20)      613 2024-03-19 08:48:10.000000 redturtle.prenotazioni-2.5.3/src/redturtle/prenotazioni/profiles/default/workflows.xml
-drwxr-xr-x   0 lucabel    (501) staff       (20)        0 2024-03-19 08:48:10.801316 redturtle.prenotazioni-2.5.3/src/redturtle/prenotazioni/profiles/to_1402/
--rw-r--r--   0 lucabel    (501) staff       (20)     1508 2024-03-19 08:48:10.000000 redturtle.prenotazioni-2.5.3/src/redturtle/prenotazioni/profiles/to_1402/contentrules.xml
-drwxr-xr-x   0 lucabel    (501) staff       (20)        0 2024-03-19 08:48:10.801542 redturtle.prenotazioni-2.5.3/src/redturtle/prenotazioni/profiles/to_1500/
--rw-r--r--   0 lucabel    (501) staff       (20)      226 2024-03-19 08:48:10.000000 redturtle.prenotazioni-2.5.3/src/redturtle/prenotazioni/profiles/to_1500/types.xml
-drwxr-xr-x   0 lucabel    (501) staff       (20)        0 2024-03-19 08:48:10.802102 redturtle.prenotazioni-2.5.3/src/redturtle/prenotazioni/profiles/to_2005/
--rw-r--r--   0 lucabel    (501) staff       (20)       88 2024-03-19 08:48:10.000000 redturtle.prenotazioni-2.5.3/src/redturtle/prenotazioni/profiles/to_2005/metadata.xml
--rw-r--r--   0 lucabel    (501) staff       (20)      638 2024-03-19 08:48:10.000000 redturtle.prenotazioni-2.5.3/src/redturtle/prenotazioni/profiles/to_2005/rolemap.xml
-drwxr-xr-x   0 lucabel    (501) staff       (20)        0 2024-03-19 08:48:10.802720 redturtle.prenotazioni-2.5.3/src/redturtle/prenotazioni/profiles/to_2006/
--rw-r--r--   0 lucabel    (501) staff       (20)       88 2024-03-19 08:48:10.000000 redturtle.prenotazioni-2.5.3/src/redturtle/prenotazioni/profiles/to_2006/metadata.xml
-drwxr-xr-x   0 lucabel    (501) staff       (20)        0 2024-03-19 08:48:10.742692 redturtle.prenotazioni-2.5.3/src/redturtle/prenotazioni/profiles/to_2006/workflows/
-drwxr-xr-x   0 lucabel    (501) staff       (20)        0 2024-03-19 08:48:10.803160 redturtle.prenotazioni-2.5.3/src/redturtle/prenotazioni/profiles/to_2006/workflows/prenotazioni_workflow/
--rw-r--r--   0 lucabel    (501) staff       (20)    12711 2024-03-19 08:48:10.000000 redturtle.prenotazioni-2.5.3/src/redturtle/prenotazioni/profiles/to_2006/workflows/prenotazioni_workflow/definition.xml
--rw-r--r--   0 lucabel    (501) staff       (20)      279 2024-03-19 08:48:10.000000 redturtle.prenotazioni-2.5.3/src/redturtle/prenotazioni/profiles/to_2006/workflows.xml
-drwxr-xr-x   0 lucabel    (501) staff       (20)        0 2024-03-19 08:48:10.803465 redturtle.prenotazioni-2.5.3/src/redturtle/prenotazioni/profiles/uninstall/
--rw-r--r--   0 lucabel    (501) staff       (20)      125 2024-03-19 08:48:10.000000 redturtle.prenotazioni-2.5.3/src/redturtle/prenotazioni/profiles/uninstall/browserlayer.xml
-drwxr-xr-x   0 lucabel    (501) staff       (20)        0 2024-03-19 08:48:10.804042 redturtle.prenotazioni-2.5.3/src/redturtle/prenotazioni/profiles/uninstall/registry/
--rw-r--r--   0 lucabel    (501) staff       (20)      431 2024-03-19 08:48:10.000000 redturtle.prenotazioni-2.5.3/src/redturtle/prenotazioni/profiles/uninstall/registry/resources.xml
--rw-r--r--   0 lucabel    (501) staff       (20)      152 2024-03-19 08:48:10.000000 redturtle.prenotazioni-2.5.3/src/redturtle/prenotazioni/profiles/uninstall/registry/settings.xml
-drwxr-xr-x   0 lucabel    (501) staff       (20)        0 2024-03-19 08:48:10.804713 redturtle.prenotazioni-2.5.3/src/redturtle/prenotazioni/restapi/
--rw-r--r--   0 lucabel    (501) staff       (20)        0 2024-03-19 08:48:10.000000 redturtle.prenotazioni-2.5.3/src/redturtle/prenotazioni/restapi/__init__.py
--rw-r--r--   0 lucabel    (501) staff       (20)      199 2024-03-19 08:48:10.000000 redturtle.prenotazioni-2.5.3/src/redturtle/prenotazioni/restapi/configure.zcml
-drwxr-xr-x   0 lucabel    (501) staff       (20)        0 2024-03-19 08:48:10.805400 redturtle.prenotazioni-2.5.3/src/redturtle/prenotazioni/restapi/serializers/
--rw-r--r--   0 lucabel    (501) staff       (20)        0 2024-03-19 08:48:10.000000 redturtle.prenotazioni-2.5.3/src/redturtle/prenotazioni/restapi/serializers/__init__.py
-drwxr-xr-x   0 lucabel    (501) staff       (20)        0 2024-03-19 08:48:10.807526 redturtle.prenotazioni-2.5.3/src/redturtle/prenotazioni/restapi/serializers/adapters/
--rw-r--r--   0 lucabel    (501) staff       (20)        0 2024-03-19 08:48:10.000000 redturtle.prenotazioni-2.5.3/src/redturtle/prenotazioni/restapi/serializers/adapters/__init__.py
--rw-r--r--   0 lucabel    (501) staff       (20)      468 2024-03-19 08:48:10.000000 redturtle.prenotazioni-2.5.3/src/redturtle/prenotazioni/restapi/serializers/adapters/configure.zcml
--rw-r--r--   0 lucabel    (501) staff       (20)     7441 2024-03-19 08:48:10.000000 redturtle.prenotazioni-2.5.3/src/redturtle/prenotazioni/restapi/serializers/adapters/prenotazione.py
--rw-r--r--   0 lucabel    (501) staff       (20)      973 2024-03-19 08:48:10.000000 redturtle.prenotazioni-2.5.3/src/redturtle/prenotazioni/restapi/serializers/adapters/prenotazione_type.py
--rw-r--r--   0 lucabel    (501) staff       (20)      925 2024-03-19 08:48:10.000000 redturtle.prenotazioni-2.5.3/src/redturtle/prenotazioni/restapi/serializers/adapters/prenotazioni_folder.py
--rw-r--r--   0 lucabel    (501) staff       (20)     1721 2024-03-19 08:48:10.000000 redturtle.prenotazioni-2.5.3/src/redturtle/prenotazioni/restapi/serializers/adapters/slot.py
--rw-r--r--   0 lucabel    (501) staff       (20)      162 2024-03-19 08:48:10.000000 redturtle.prenotazioni-2.5.3/src/redturtle/prenotazioni/restapi/serializers/configure.zcml
-drwxr-xr-x   0 lucabel    (501) staff       (20)        0 2024-03-19 08:48:10.811950 redturtle.prenotazioni-2.5.3/src/redturtle/prenotazioni/restapi/services/
-drwxr-xr-x   0 lucabel    (501) staff       (20)        0 2024-03-19 08:48:10.817899 redturtle.prenotazioni-2.5.3/src/redturtle/prenotazioni/restapi/services/available_slots/
--rw-r--r--   0 lucabel    (501) staff       (20)        0 2024-03-19 08:48:10.000000 redturtle.prenotazioni-2.5.3/src/redturtle/prenotazioni/restapi/services/available_slots/__init__.py
--rw-r--r--   0 lucabel    (501) staff       (20)      352 2024-03-19 08:48:10.000000 redturtle.prenotazioni-2.5.3/src/redturtle/prenotazioni/restapi/services/available_slots/configure.zcml
--rw-r--r--   0 lucabel    (501) staff       (20)     2822 2024-03-19 08:48:10.000000 redturtle.prenotazioni-2.5.3/src/redturtle/prenotazioni/restapi/services/available_slots/get.py
-drwxr-xr-x   0 lucabel    (501) staff       (20)        0 2024-03-19 08:48:10.820235 redturtle.prenotazioni-2.5.3/src/redturtle/prenotazioni/restapi/services/booking/
--rw-r--r--   0 lucabel    (501) staff       (20)        0 2024-03-19 08:48:10.000000 redturtle.prenotazioni-2.5.3/src/redturtle/prenotazioni/restapi/services/booking/__init__.py
--rw-r--r--   0 lucabel    (501) staff       (20)     6595 2024-03-19 08:48:10.000000 redturtle.prenotazioni-2.5.3/src/redturtle/prenotazioni/restapi/services/booking/add.py
--rw-r--r--   0 lucabel    (501) staff       (20)     1641 2024-03-19 08:48:10.000000 redturtle.prenotazioni-2.5.3/src/redturtle/prenotazioni/restapi/services/booking/configure.zcml
--rw-r--r--   0 lucabel    (501) staff       (20)     1209 2024-03-19 08:48:10.000000 redturtle.prenotazioni-2.5.3/src/redturtle/prenotazioni/restapi/services/booking/delete.py
--rw-r--r--   0 lucabel    (501) staff       (20)     1166 2024-03-19 08:48:10.000000 redturtle.prenotazioni-2.5.3/src/redturtle/prenotazioni/restapi/services/booking/get.py
--rw-r--r--   0 lucabel    (501) staff       (20)     1328 2024-03-19 08:48:10.000000 redturtle.prenotazioni-2.5.3/src/redturtle/prenotazioni/restapi/services/booking/move.py
--rw-r--r--   0 lucabel    (501) staff       (20)     1152 2024-03-19 08:48:10.000000 redturtle.prenotazioni-2.5.3/src/redturtle/prenotazioni/restapi/services/booking/notify_about_confirm.py
--rw-r--r--   0 lucabel    (501) staff       (20)      966 2024-03-19 08:48:10.000000 redturtle.prenotazioni-2.5.3/src/redturtle/prenotazioni/restapi/services/booking/vacation.py
-drwxr-xr-x   0 lucabel    (501) staff       (20)        0 2024-03-19 08:48:10.821050 redturtle.prenotazioni-2.5.3/src/redturtle/prenotazioni/restapi/services/booking_schema/
--rw-r--r--   0 lucabel    (501) staff       (20)        0 2024-03-19 08:48:10.000000 redturtle.prenotazioni-2.5.3/src/redturtle/prenotazioni/restapi/services/booking_schema/__init__.py
--rw-r--r--   0 lucabel    (501) staff       (20)      404 2024-03-19 08:48:10.000000 redturtle.prenotazioni-2.5.3/src/redturtle/prenotazioni/restapi/services/booking_schema/configure.zcml
--rw-r--r--   0 lucabel    (501) staff       (20)     4916 2024-03-19 08:48:10.000000 redturtle.prenotazioni-2.5.3/src/redturtle/prenotazioni/restapi/services/booking_schema/get.py
-drwxr-xr-x   0 lucabel    (501) staff       (20)        0 2024-03-19 08:48:10.821846 redturtle.prenotazioni-2.5.3/src/redturtle/prenotazioni/restapi/services/bookings/
--rw-r--r--   0 lucabel    (501) staff       (20)        0 2024-03-19 08:48:10.000000 redturtle.prenotazioni-2.5.3/src/redturtle/prenotazioni/restapi/services/bookings/__init__.py
--rw-r--r--   0 lucabel    (501) staff       (20)      548 2024-03-19 08:48:10.000000 redturtle.prenotazioni-2.5.3/src/redturtle/prenotazioni/restapi/services/bookings/configure.zcml
--rw-r--r--   0 lucabel    (501) staff       (20)     3898 2024-03-19 08:48:10.000000 redturtle.prenotazioni-2.5.3/src/redturtle/prenotazioni/restapi/services/bookings/search.py
--rw-r--r--   0 lucabel    (501) staff       (20)      336 2024-03-19 08:48:10.000000 redturtle.prenotazioni-2.5.3/src/redturtle/prenotazioni/restapi/services/configure.zcml
-drwxr-xr-x   0 lucabel    (501) staff       (20)        0 2024-03-19 08:48:10.822687 redturtle.prenotazioni-2.5.3/src/redturtle/prenotazioni/restapi/services/day/
--rw-r--r--   0 lucabel    (501) staff       (20)        0 2024-03-19 08:48:10.000000 redturtle.prenotazioni-2.5.3/src/redturtle/prenotazioni/restapi/services/day/__init__.py
--rw-r--r--   0 lucabel    (501) staff       (20)      365 2024-03-19 08:48:10.000000 redturtle.prenotazioni-2.5.3/src/redturtle/prenotazioni/restapi/services/day/configure.zcml
--rw-r--r--   0 lucabel    (501) staff       (20)     6198 2024-03-19 08:48:10.000000 redturtle.prenotazioni-2.5.3/src/redturtle/prenotazioni/restapi/services/day/day.py
-drwxr-xr-x   0 lucabel    (501) staff       (20)        0 2024-03-19 08:48:10.823555 redturtle.prenotazioni-2.5.3/src/redturtle/prenotazioni/restapi/services/types/
--rw-r--r--   0 lucabel    (501) staff       (20)        0 2024-03-19 08:48:10.000000 redturtle.prenotazioni-2.5.3/src/redturtle/prenotazioni/restapi/services/types/__init__.py
--rw-r--r--   0 lucabel    (501) staff       (20)      216 2024-03-19 08:48:10.000000 redturtle.prenotazioni-2.5.3/src/redturtle/prenotazioni/restapi/services/types/configure.zcml
--rw-r--r--   0 lucabel    (501) staff       (20)      915 2024-03-19 08:48:10.000000 redturtle.prenotazioni-2.5.3/src/redturtle/prenotazioni/restapi/services/types/get.py
-drwxr-xr-x   0 lucabel    (501) staff       (20)        0 2024-03-19 08:48:10.824061 redturtle.prenotazioni-2.5.3/src/redturtle/prenotazioni/scripts/
--rw-r--r--   0 lucabel    (501) staff       (20)        0 2024-03-19 08:48:10.000000 redturtle.prenotazioni-2.5.3/src/redturtle/prenotazioni/scripts/__init__.py
--rw-r--r--   0 lucabel    (501) staff       (20)      892 2024-03-19 08:48:10.000000 redturtle.prenotazioni-2.5.3/src/redturtle/prenotazioni/scripts/notify_upcoming_bookings.py
--rw-r--r--   0 lucabel    (501) staff       (20)     1062 2024-03-19 08:48:10.000000 redturtle.prenotazioni-2.5.3/src/redturtle/prenotazioni/setuphandlers.py
--rw-r--r--   0 lucabel    (501) staff       (20)     3443 2024-03-19 08:48:10.000000 redturtle.prenotazioni-2.5.3/src/redturtle/prenotazioni/testing.py
-drwxr-xr-x   0 lucabel    (501) staff       (20)        0 2024-03-19 08:48:10.834302 redturtle.prenotazioni-2.5.3/src/redturtle/prenotazioni/tests/
--rw-r--r--   0 lucabel    (501) staff       (20)      105 2024-03-19 08:48:10.000000 redturtle.prenotazioni-2.5.3/src/redturtle/prenotazioni/tests/__init__.py
--rw-r--r--   0 lucabel    (501) staff       (20)     1223 2024-03-19 08:48:10.000000 redturtle.prenotazioni-2.5.3/src/redturtle/prenotazioni/tests/helpers.py
--rw-r--r--   0 lucabel    (501) staff       (20)     3222 2024-03-19 08:48:10.000000 redturtle.prenotazioni-2.5.3/src/redturtle/prenotazioni/tests/test_add_block.py
--rw-r--r--   0 lucabel    (501) staff       (20)    24795 2024-03-19 08:48:10.000000 redturtle.prenotazioni-2.5.3/src/redturtle/prenotazioni/tests/test_add_booking.py
--rw-r--r--   0 lucabel    (501) staff       (20)     1980 2024-03-19 08:48:10.000000 redturtle.prenotazioni-2.5.3/src/redturtle/prenotazioni/tests/test_add_booking_type.py
--rw-r--r--   0 lucabel    (501) staff       (20)    14461 2024-03-19 08:48:10.000000 redturtle.prenotazioni-2.5.3/src/redturtle/prenotazioni/tests/test_available_slots.py
--rw-r--r--   0 lucabel    (501) staff       (20)     2011 2024-03-19 08:48:10.000000 redturtle.prenotazioni-2.5.3/src/redturtle/prenotazioni/tests/test_base_slot.py
--rw-r--r--   0 lucabel    (501) staff       (20)     4387 2024-03-19 08:48:10.000000 redturtle.prenotazioni-2.5.3/src/redturtle/prenotazioni/tests/test_booker_choose_available_slot.py
--rw-r--r--   0 lucabel    (501) staff       (20)     6402 2024-03-19 08:48:10.000000 redturtle.prenotazioni-2.5.3/src/redturtle/prenotazioni/tests/test_booking_info.py
--rw-r--r--   0 lucabel    (501) staff       (20)     6901 2024-03-19 08:48:10.000000 redturtle.prenotazioni-2.5.3/src/redturtle/prenotazioni/tests/test_booking_notify.py
--rw-r--r--   0 lucabel    (501) staff       (20)     8748 2024-03-19 08:48:10.000000 redturtle.prenotazioni-2.5.3/src/redturtle/prenotazioni/tests/test_booking_schema.py
--rw-r--r--   0 lucabel    (501) staff       (20)     8696 2024-03-19 08:48:10.000000 redturtle.prenotazioni-2.5.3/src/redturtle/prenotazioni/tests/test_bookings_num_limit.py
--rw-r--r--   0 lucabel    (501) staff       (20)     5952 2024-03-19 08:48:10.000000 redturtle.prenotazioni-2.5.3/src/redturtle/prenotazioni/tests/test_browser_utilities_notify_upcoming_bookings.py
--rw-r--r--   0 lucabel    (501) staff       (20)     3088 2024-03-19 08:48:10.000000 redturtle.prenotazioni-2.5.3/src/redturtle/prenotazioni/tests/test_content_validators_validate_pause_table.py
--rw-r--r--   0 lucabel    (501) staff       (20)     5810 2024-03-19 08:48:10.000000 redturtle.prenotazioni-2.5.3/src/redturtle/prenotazioni/tests/test_day.py
--rw-r--r--   0 lucabel    (501) staff       (20)    10871 2024-03-19 08:48:10.000000 redturtle.prenotazioni-2.5.3/src/redturtle/prenotazioni/tests/test_delete_booking.py
--rw-r--r--   0 lucabel    (501) staff       (20)    10361 2024-03-19 08:48:10.000000 redturtle.prenotazioni-2.5.3/src/redturtle/prenotazioni/tests/test_delete_booking_api.py
--rw-r--r--   0 lucabel    (501) staff       (20)     4000 2024-03-19 08:48:10.000000 redturtle.prenotazioni-2.5.3/src/redturtle/prenotazioni/tests/test_gates_overrides.py
--rw-r--r--   0 lucabel    (501) staff       (20)     8184 2024-03-19 08:48:10.000000 redturtle.prenotazioni-2.5.3/src/redturtle/prenotazioni/tests/test_move_booking_api.py
--rw-r--r--   0 lucabel    (501) staff       (20)     5216 2024-03-19 08:48:10.000000 redturtle.prenotazioni-2.5.3/src/redturtle/prenotazioni/tests/test_notification_supervisor_utility.py
--rw-r--r--   0 lucabel    (501) staff       (20)    14545 2024-03-19 08:48:10.000000 redturtle.prenotazioni-2.5.3/src/redturtle/prenotazioni/tests/test_pauses_overrides.py
--rw-r--r--   0 lucabel    (501) staff       (20)     5029 2024-03-19 08:48:10.000000 redturtle.prenotazioni-2.5.3/src/redturtle/prenotazioni/tests/test_prenotazione_email_sent_to_managers.py
--rw-r--r--   0 lucabel    (501) staff       (20)    15081 2024-03-19 08:48:10.000000 redturtle.prenotazioni-2.5.3/src/redturtle/prenotazioni/tests/test_prenotazione_events.py
--rw-r--r--   0 lucabel    (501) staff       (20)     4861 2024-03-19 08:48:10.000000 redturtle.prenotazioni-2.5.3/src/redturtle/prenotazioni/tests/test_prenotazione_searchable_item_serializer.py
--rw-r--r--   0 lucabel    (501) staff       (20)     7049 2024-03-19 08:48:10.000000 redturtle.prenotazioni-2.5.3/src/redturtle/prenotazioni/tests/test_prenotazioni_context_state.py
--rw-r--r--   0 lucabel    (501) staff       (20)      740 2024-03-19 08:48:10.000000 redturtle.prenotazioni-2.5.3/src/redturtle/prenotazioni/tests/test_prenotazioni_folder_holidays_constraint.py
--rw-r--r--   0 lucabel    (501) staff       (20)    19833 2024-03-19 08:48:10.000000 redturtle.prenotazioni-2.5.3/src/redturtle/prenotazioni/tests/test_prenotazioni_search.py
--rw-r--r--   0 lucabel    (501) staff       (20)     2485 2024-03-19 08:48:10.000000 redturtle.prenotazioni-2.5.3/src/redturtle/prenotazioni/tests/test_restapi_types_override.py
--rw-r--r--   0 lucabel    (501) staff       (20)     9722 2024-03-19 08:48:10.000000 redturtle.prenotazioni-2.5.3/src/redturtle/prenotazioni/tests/test_send_ical.py
--rw-r--r--   0 lucabel    (501) staff       (20)     4180 2024-03-19 08:48:10.000000 redturtle.prenotazioni-2.5.3/src/redturtle/prenotazioni/tests/test_setup.py
--rw-r--r--   0 lucabel    (501) staff       (20)     3046 2024-03-19 08:48:10.000000 redturtle.prenotazioni-2.5.3/src/redturtle/prenotazioni/tests/test_stringinterp.py
--rw-r--r--   0 lucabel    (501) staff       (20)      905 2024-03-19 08:48:10.000000 redturtle.prenotazioni-2.5.3/src/redturtle/prenotazioni/tests/test_utils.py
--rw-r--r--   0 lucabel    (501) staff       (20)     6486 2024-03-19 08:48:10.000000 redturtle.prenotazioni-2.5.3/src/redturtle/prenotazioni/tests/test_vacation_api.py
--rw-r--r--   0 lucabel    (501) staff       (20)     2349 2024-03-19 08:48:10.000000 redturtle.prenotazioni-2.5.3/src/redturtle/prenotazioni/tests/test_vocabularies.py
--rw-r--r--   0 lucabel    (501) staff       (20)    22242 2024-03-19 08:48:10.000000 redturtle.prenotazioni-2.5.3/src/redturtle/prenotazioni/tests/test_week_table_overrides.py
--rw-r--r--   0 lucabel    (501) staff       (20)    16547 2024-03-19 08:48:10.000000 redturtle.prenotazioni-2.5.3/src/redturtle/prenotazioni/upgrades.py
--rw-r--r--   0 lucabel    (501) staff       (20)    10360 2024-03-19 08:48:10.000000 redturtle.prenotazioni-2.5.3/src/redturtle/prenotazioni/upgrades.zcml
-drwxr-xr-x   0 lucabel    (501) staff       (20)        0 2024-03-19 08:48:10.835627 redturtle.prenotazioni-2.5.3/src/redturtle/prenotazioni/utilities/
--rw-r--r--   0 lucabel    (501) staff       (20)       94 2024-03-19 08:48:10.000000 redturtle.prenotazioni-2.5.3/src/redturtle/prenotazioni/utilities/__init__.py
--rw-r--r--   0 lucabel    (501) staff       (20)     2900 2024-03-19 08:48:10.000000 redturtle.prenotazioni-2.5.3/src/redturtle/prenotazioni/utilities/dateutils.py
--rw-r--r--   0 lucabel    (501) staff       (20)      489 2024-03-19 08:48:10.000000 redturtle.prenotazioni-2.5.3/src/redturtle/prenotazioni/utilities/email.py
--rw-r--r--   0 lucabel    (501) staff       (20)      504 2024-03-19 08:48:10.000000 redturtle.prenotazioni-2.5.3/src/redturtle/prenotazioni/utilities/log_errors.py
--rw-r--r--   0 lucabel    (501) staff       (20)     1118 2024-03-19 08:48:10.000000 redturtle.prenotazioni-2.5.3/src/redturtle/prenotazioni/utilities/urls.py
-drwxr-xr-x   0 lucabel    (501) staff       (20)        0 2024-03-19 08:48:10.836124 redturtle.prenotazioni-2.5.3/src/redturtle/prenotazioni/utils/
--rw-r--r--   0 lucabel    (501) staff       (20)       67 2024-03-19 08:48:10.000000 redturtle.prenotazioni-2.5.3/src/redturtle/prenotazioni/utils/__init__.py
--rw-r--r--   0 lucabel    (501) staff       (20)      597 2024-03-19 08:48:10.000000 redturtle.prenotazioni-2.5.3/src/redturtle/prenotazioni/utils/get_prenotazioni_folder.py
-drwxr-xr-x   0 lucabel    (501) staff       (20)        0 2024-03-19 08:48:10.838853 redturtle.prenotazioni-2.5.3/src/redturtle/prenotazioni/vocabularies/
--rw-r--r--   0 lucabel    (501) staff       (20)       24 2024-03-19 08:48:10.000000 redturtle.prenotazioni-2.5.3/src/redturtle/prenotazioni/vocabularies/__init__.py
--rw-r--r--   0 lucabel    (501) staff       (20)     1444 2024-03-19 08:48:10.000000 redturtle.prenotazioni-2.5.3/src/redturtle/prenotazioni/vocabularies/configure.zcml
--rw-r--r--   0 lucabel    (501) staff       (20)      607 2024-03-19 08:48:10.000000 redturtle.prenotazioni-2.5.3/src/redturtle/prenotazioni/vocabularies/gates.py
--rw-r--r--   0 lucabel    (501) staff       (20)     1011 2024-03-19 08:48:10.000000 redturtle.prenotazioni-2.5.3/src/redturtle/prenotazioni/vocabularies/requirable_booking_fields.py
--rw-r--r--   0 lucabel    (501) staff       (20)      598 2024-03-19 08:48:10.000000 redturtle.prenotazioni-2.5.3/src/redturtle/prenotazioni/vocabularies/review_states.py
--rw-r--r--   0 lucabel    (501) staff       (20)     1814 2024-03-19 08:48:10.000000 redturtle.prenotazioni-2.5.3/src/redturtle/prenotazioni/vocabularies/tipologies.py
--rw-r--r--   0 lucabel    (501) staff       (20)      776 2024-03-19 08:48:10.000000 redturtle.prenotazioni-2.5.3/src/redturtle/prenotazioni/vocabularies/voc_booking_type_gates.py
--rw-r--r--   0 lucabel    (501) staff       (20)     1128 2024-03-19 08:48:10.000000 redturtle.prenotazioni-2.5.3/src/redturtle/prenotazioni/vocabularies/voc_durata_incontro.py
--rw-r--r--   0 lucabel    (501) staff       (20)     2549 2024-03-19 08:48:10.000000 redturtle.prenotazioni-2.5.3/src/redturtle/prenotazioni/vocabularies/voc_months.py
--rw-r--r--   0 lucabel    (501) staff       (20)     1367 2024-03-19 08:48:10.000000 redturtle.prenotazioni-2.5.3/src/redturtle/prenotazioni/vocabularies/voc_ore_inizio.py
--rw-r--r--   0 lucabel    (501) staff       (20)      440 2024-03-19 08:48:10.000000 redturtle.prenotazioni-2.5.3/src/redturtle/prenotazioni/vocabularies/voc_pause_scheduler.py
-drwxr-xr-x   0 lucabel    (501) staff       (20)        0 2024-03-19 08:48:10.751876 redturtle.prenotazioni-2.5.3/src/redturtle.prenotazioni.egg-info/
--rw-r--r--   0 lucabel    (501) staff       (20)    45109 2024-03-19 08:48:10.000000 redturtle.prenotazioni-2.5.3/src/redturtle.prenotazioni.egg-info/PKG-INFO
--rw-r--r--   0 lucabel    (501) staff       (20)    17477 2024-03-19 08:48:10.000000 redturtle.prenotazioni-2.5.3/src/redturtle.prenotazioni.egg-info/SOURCES.txt
--rw-r--r--   0 lucabel    (501) staff       (20)        1 2024-03-19 08:48:10.000000 redturtle.prenotazioni-2.5.3/src/redturtle.prenotazioni.egg-info/dependency_links.txt
--rw-r--r--   0 lucabel    (501) staff       (20)      267 2024-03-19 08:48:10.000000 redturtle.prenotazioni-2.5.3/src/redturtle.prenotazioni.egg-info/entry_points.txt
--rw-r--r--   0 lucabel    (501) staff       (20)       10 2024-03-19 08:48:10.000000 redturtle.prenotazioni-2.5.3/src/redturtle.prenotazioni.egg-info/namespace_packages.txt
--rw-r--r--   0 lucabel    (501) staff       (20)        1 2024-03-19 08:48:10.000000 redturtle.prenotazioni-2.5.3/src/redturtle.prenotazioni.egg-info/not-zip-safe
--rw-r--r--   0 lucabel    (501) staff       (20)      425 2024-03-19 08:48:10.000000 redturtle.prenotazioni-2.5.3/src/redturtle.prenotazioni.egg-info/requires.txt
--rw-r--r--   0 lucabel    (501) staff       (20)       10 2024-03-19 08:48:10.000000 redturtle.prenotazioni-2.5.3/src/redturtle.prenotazioni.egg-info/top_level.txt
+drwxr-xr-x   0 cekk       (501) staff       (20)        0 2024-04-02 07:43:54.802766 redturtle.prenotazioni-2.6.0/
+-rw-r--r--   0 cekk       (501) staff       (20)      748 2024-04-02 07:43:54.000000 redturtle.prenotazioni-2.6.0/APP_IO.txt
+-rw-r--r--   0 cekk       (501) staff       (20)    16940 2024-04-02 07:43:54.000000 redturtle.prenotazioni-2.6.0/CHANGES.rst
+-rw-r--r--   0 cekk       (501) staff       (20)      152 2024-04-02 07:43:54.000000 redturtle.prenotazioni-2.6.0/CONTRIBUTORS.rst
+-rw-r--r--   0 cekk       (501) staff       (20)      586 2024-04-02 07:43:54.000000 redturtle.prenotazioni-2.6.0/DEVELOP.rst
+-rw-r--r--   0 cekk       (501) staff       (20)    18092 2024-04-02 07:43:54.000000 redturtle.prenotazioni-2.6.0/LICENSE.GPL
+-rw-r--r--   0 cekk       (501) staff       (20)      667 2024-04-02 07:43:54.000000 redturtle.prenotazioni-2.6.0/LICENSE.rst
+-rw-r--r--   0 cekk       (501) staff       (20)      110 2024-04-02 07:43:54.000000 redturtle.prenotazioni-2.6.0/MANIFEST.in
+-rw-r--r--   0 cekk       (501) staff       (20)    45601 2024-04-02 07:43:54.802847 redturtle.prenotazioni-2.6.0/PKG-INFO
+-rw-r--r--   0 cekk       (501) staff       (20)    27252 2024-04-02 07:43:54.000000 redturtle.prenotazioni-2.6.0/README.rst
+-rw-r--r--   0 cekk       (501) staff       (20)      164 2024-04-02 07:43:54.000000 redturtle.prenotazioni-2.6.0/TODO.txt
+-rw-r--r--   0 cekk       (501) staff       (20)      105 2024-04-02 07:43:54.000000 redturtle.prenotazioni-2.6.0/constraints-5.2.x.txt
+-rw-r--r--   0 cekk       (501) staff       (20)      105 2024-04-02 07:43:54.000000 redturtle.prenotazioni-2.6.0/constraints.txt
+drwxr-xr-x   0 cekk       (501) staff       (20)        0 2024-04-02 07:43:54.768036 redturtle.prenotazioni-2.6.0/docs/
+-rw-r--r--   0 cekk       (501) staff       (20)     7984 2024-04-02 07:43:54.000000 redturtle.prenotazioni-2.6.0/docs/conf.py
+-rw-r--r--   0 cekk       (501) staff       (20)       89 2024-04-02 07:43:54.000000 redturtle.prenotazioni-2.6.0/docs/index.rst
+-rw-r--r--   0 cekk       (501) staff       (20)      476 2024-04-02 07:43:54.000000 redturtle.prenotazioni-2.6.0/requirements-6.0.x.txt
+-rw-r--r--   0 cekk       (501) staff       (20)       48 2024-04-02 07:43:54.000000 redturtle.prenotazioni-2.6.0/requirements.txt
+-rw-r--r--   0 cekk       (501) staff       (20)      344 2024-04-02 07:43:54.803074 redturtle.prenotazioni-2.6.0/setup.cfg
+-rw-r--r--   0 cekk       (501) staff       (20)     3420 2024-04-02 07:43:54.000000 redturtle.prenotazioni-2.6.0/setup.py
+drwxr-xr-x   0 cekk       (501) staff       (20)        0 2024-04-02 07:43:54.762115 redturtle.prenotazioni-2.6.0/src/
+drwxr-xr-x   0 cekk       (501) staff       (20)        0 2024-04-02 07:43:54.768138 redturtle.prenotazioni-2.6.0/src/redturtle/
+-rw-r--r--   0 cekk       (501) staff       (20)       80 2024-04-02 07:43:54.000000 redturtle.prenotazioni-2.6.0/src/redturtle/__init__.py
+drwxr-xr-x   0 cekk       (501) staff       (20)        0 2024-04-02 07:43:54.770060 redturtle.prenotazioni-2.6.0/src/redturtle/prenotazioni/
+-rw-r--r--   0 cekk       (501) staff       (20)     4638 2024-04-02 07:43:54.000000 redturtle.prenotazioni-2.6.0/src/redturtle/prenotazioni/__init__.py
+drwxr-xr-x   0 cekk       (501) staff       (20)        0 2024-04-02 07:43:54.770352 redturtle.prenotazioni-2.6.0/src/redturtle/prenotazioni/actions/
+-rw-r--r--   0 cekk       (501) staff       (20)        0 2024-04-02 07:43:54.000000 redturtle.prenotazioni-2.6.0/src/redturtle/prenotazioni/actions/__init__.py
+-rw-r--r--   0 cekk       (501) staff       (20)      226 2024-04-02 07:43:54.000000 redturtle.prenotazioni-2.6.0/src/redturtle/prenotazioni/actions/configure.zcml
+-rw-r--r--   0 cekk       (501) staff       (20)     3333 2024-04-02 07:43:54.000000 redturtle.prenotazioni-2.6.0/src/redturtle/prenotazioni/actions/mail.py
+drwxr-xr-x   0 cekk       (501) staff       (20)        0 2024-04-02 07:43:54.771290 redturtle.prenotazioni-2.6.0/src/redturtle/prenotazioni/adapters/
+-rw-r--r--   0 cekk       (501) staff       (20)       24 2024-04-02 07:43:54.000000 redturtle.prenotazioni-2.6.0/src/redturtle/prenotazioni/adapters/__init__.py
+-rw-r--r--   0 cekk       (501) staff       (20)    15273 2024-04-02 07:43:54.000000 redturtle.prenotazioni-2.6.0/src/redturtle/prenotazioni/adapters/booker.py
+-rw-r--r--   0 cekk       (501) staff       (20)      729 2024-04-02 07:43:54.000000 redturtle.prenotazioni-2.6.0/src/redturtle/prenotazioni/adapters/booking_code.py
+-rw-r--r--   0 cekk       (501) staff       (20)     5974 2024-04-02 07:43:54.000000 redturtle.prenotazioni-2.6.0/src/redturtle/prenotazioni/adapters/configure.zcml
+-rw-r--r--   0 cekk       (501) staff       (20)     4786 2024-04-02 07:43:54.000000 redturtle.prenotazioni-2.6.0/src/redturtle/prenotazioni/adapters/conflict.py
+-rw-r--r--   0 cekk       (501) staff       (20)     5037 2024-04-02 07:43:54.000000 redturtle.prenotazioni-2.6.0/src/redturtle/prenotazioni/adapters/ical.py
+-rw-r--r--   0 cekk       (501) staff       (20)      273 2024-04-02 07:43:54.000000 redturtle.prenotazioni-2.6.0/src/redturtle/prenotazioni/adapters/prenotazione_menu.py
+-rw-r--r--   0 cekk       (501) staff       (20)     9662 2024-04-02 07:43:54.000000 redturtle.prenotazioni-2.6.0/src/redturtle/prenotazioni/adapters/slot.py
+-rw-r--r--   0 cekk       (501) staff       (20)     8771 2024-04-02 07:43:54.000000 redturtle.prenotazioni-2.6.0/src/redturtle/prenotazioni/adapters/stringinterp.py
+drwxr-xr-x   0 cekk       (501) staff       (20)        0 2024-04-02 07:43:54.771399 redturtle.prenotazioni-2.6.0/src/redturtle/prenotazioni/behaviors/
+drwxr-xr-x   0 cekk       (501) staff       (20)        0 2024-04-02 07:43:54.771774 redturtle.prenotazioni-2.6.0/src/redturtle/prenotazioni/behaviors/booking_folder/
+-rw-r--r--   0 cekk       (501) staff       (20)        0 2024-04-02 07:43:54.000000 redturtle.prenotazioni-2.6.0/src/redturtle/prenotazioni/behaviors/booking_folder/__init__.py
+-rw-r--r--   0 cekk       (501) staff       (20)      563 2024-04-02 07:43:54.000000 redturtle.prenotazioni-2.6.0/src/redturtle/prenotazioni/behaviors/booking_folder/configure.zcml
+-rw-r--r--   0 cekk       (501) staff       (20)     1766 2024-04-02 07:43:54.000000 redturtle.prenotazioni-2.6.0/src/redturtle/prenotazioni/behaviors/booking_folder/contacts.py
+drwxr-xr-x   0 cekk       (501) staff       (20)        0 2024-04-02 07:43:54.772039 redturtle.prenotazioni-2.6.0/src/redturtle/prenotazioni/behaviors/booking_folder/notifications/
+-rw-r--r--   0 cekk       (501) staff       (20)     1454 2024-04-02 07:43:54.000000 redturtle.prenotazioni-2.6.0/src/redturtle/prenotazioni/behaviors/booking_folder/notifications/__init__.py
+drwxr-xr-x   0 cekk       (501) staff       (20)        0 2024-04-02 07:43:54.772873 redturtle.prenotazioni-2.6.0/src/redturtle/prenotazioni/behaviors/booking_folder/notifications/appio/
+-rw-r--r--   0 cekk       (501) staff       (20)    10220 2024-04-02 07:43:54.000000 redturtle.prenotazioni-2.6.0/src/redturtle/prenotazioni/behaviors/booking_folder/notifications/appio/__init__.py
+-rw-r--r--   0 cekk       (501) staff       (20)     4071 2024-04-02 07:43:54.000000 redturtle.prenotazioni-2.6.0/src/redturtle/prenotazioni/behaviors/booking_folder/notifications/appio/adapters.py
+-rw-r--r--   0 cekk       (501) staff       (20)     2364 2024-04-02 07:43:54.000000 redturtle.prenotazioni-2.6.0/src/redturtle/prenotazioni/behaviors/booking_folder/notifications/appio/configure.zcml
+-rw-r--r--   0 cekk       (501) staff       (20)     2592 2024-04-02 07:43:54.000000 redturtle.prenotazioni-2.6.0/src/redturtle/prenotazioni/behaviors/booking_folder/notifications/appio/events.py
+-rw-r--r--   0 cekk       (501) staff       (20)     3178 2024-04-02 07:43:54.000000 redturtle.prenotazioni-2.6.0/src/redturtle/prenotazioni/behaviors/booking_folder/notifications/appio/notfication_appio_message.py
+-rw-r--r--   0 cekk       (501) staff       (20)     1151 2024-04-02 07:43:54.000000 redturtle.prenotazioni-2.6.0/src/redturtle/prenotazioni/behaviors/booking_folder/notifications/appio/voc_service_keys.py
+-rw-r--r--   0 cekk       (501) staff       (20)      423 2024-04-02 07:43:54.000000 redturtle.prenotazioni-2.6.0/src/redturtle/prenotazioni/behaviors/booking_folder/notifications/configure.zcml
+drwxr-xr-x   0 cekk       (501) staff       (20)        0 2024-04-02 07:43:54.773572 redturtle.prenotazioni-2.6.0/src/redturtle/prenotazioni/behaviors/booking_folder/notifications/email/
+-rw-r--r--   0 cekk       (501) staff       (20)     9647 2024-04-02 07:43:54.000000 redturtle.prenotazioni-2.6.0/src/redturtle/prenotazioni/behaviors/booking_folder/notifications/email/__init__.py
+-rw-r--r--   0 cekk       (501) staff       (20)     1607 2024-04-02 07:43:54.000000 redturtle.prenotazioni-2.6.0/src/redturtle/prenotazioni/behaviors/booking_folder/notifications/email/adapters.py
+-rw-r--r--   0 cekk       (501) staff       (20)     2284 2024-04-02 07:43:54.000000 redturtle.prenotazioni-2.6.0/src/redturtle/prenotazioni/behaviors/booking_folder/notifications/email/configure.zcml
+-rw-r--r--   0 cekk       (501) staff       (20)     3600 2024-04-02 07:43:54.000000 redturtle.prenotazioni-2.6.0/src/redturtle/prenotazioni/behaviors/booking_folder/notifications/email/events.py
+-rw-r--r--   0 cekk       (501) staff       (20)    11940 2024-04-02 07:43:54.000000 redturtle.prenotazioni-2.6.0/src/redturtle/prenotazioni/behaviors/booking_folder/notifications/email/notification_email_message.py
+drwxr-xr-x   0 cekk       (501) staff       (20)        0 2024-04-02 07:43:54.774272 redturtle.prenotazioni-2.6.0/src/redturtle/prenotazioni/behaviors/booking_folder/notifications/sms/
+-rw-r--r--   0 cekk       (501) staff       (20)     5724 2024-04-02 07:43:54.000000 redturtle.prenotazioni-2.6.0/src/redturtle/prenotazioni/behaviors/booking_folder/notifications/sms/__init__.py
+-rw-r--r--   0 cekk       (501) staff       (20)     1115 2024-04-02 07:43:54.000000 redturtle.prenotazioni-2.6.0/src/redturtle/prenotazioni/behaviors/booking_folder/notifications/sms/adapters.py
+-rw-r--r--   0 cekk       (501) staff       (20)     1689 2024-04-02 07:43:54.000000 redturtle.prenotazioni-2.6.0/src/redturtle/prenotazioni/behaviors/booking_folder/notifications/sms/configure.zcml
+-rw-r--r--   0 cekk       (501) staff       (20)     2931 2024-04-02 07:43:54.000000 redturtle.prenotazioni-2.6.0/src/redturtle/prenotazioni/behaviors/booking_folder/notifications/sms/events.py
+-rw-r--r--   0 cekk       (501) staff       (20)     2216 2024-04-02 07:43:54.000000 redturtle.prenotazioni-2.6.0/src/redturtle/prenotazioni/behaviors/booking_folder/notifications/sms/message.py
+-rw-r--r--   0 cekk       (501) staff       (20)      284 2024-04-02 07:43:54.000000 redturtle.prenotazioni-2.6.0/src/redturtle/prenotazioni/behaviors/configure.zcml
+drwxr-xr-x   0 cekk       (501) staff       (20)        0 2024-04-02 07:43:54.777027 redturtle.prenotazioni-2.6.0/src/redturtle/prenotazioni/browser/
+-rw-r--r--   0 cekk       (501) staff       (20)        0 2024-04-02 07:43:54.000000 redturtle.prenotazioni-2.6.0/src/redturtle/prenotazioni/browser/__init__.py
+-rw-r--r--   0 cekk       (501) staff       (20)     1817 2024-04-02 07:43:54.000000 redturtle.prenotazioni-2.6.0/src/redturtle/prenotazioni/browser/base.py
+-rw-r--r--   0 cekk       (501) staff       (20)     7331 2024-04-02 07:43:54.000000 redturtle.prenotazioni-2.6.0/src/redturtle/prenotazioni/browser/configure.zcml
+-rw-r--r--   0 cekk       (501) staff       (20)      655 2024-04-02 07:43:54.000000 redturtle.prenotazioni-2.6.0/src/redturtle/prenotazioni/browser/custom_radio_input.pt
+-rw-r--r--   0 cekk       (501) staff       (20)     5709 2024-04-02 07:43:54.000000 redturtle.prenotazioni-2.6.0/src/redturtle/prenotazioni/browser/delete_reservation.py
+-rw-r--r--   0 cekk       (501) staff       (20)      673 2024-04-02 07:43:54.000000 redturtle.prenotazioni-2.6.0/src/redturtle/prenotazioni/browser/folderfactories.py
+-rw-r--r--   0 cekk       (501) staff       (20)      155 2024-04-02 07:43:54.000000 redturtle.prenotazioni-2.6.0/src/redturtle/prenotazioni/browser/interfaces.py
+drwxr-xr-x   0 cekk       (501) staff       (20)        0 2024-04-02 07:43:54.777198 redturtle.prenotazioni-2.6.0/src/redturtle/prenotazioni/browser/overrides/
+-rw-r--r--   0 cekk       (501) staff       (20)        0 2024-04-02 07:43:54.000000 redturtle.prenotazioni-2.6.0/src/redturtle/prenotazioni/browser/overrides/.gitkeep
+-rw-r--r--   0 cekk       (501) staff       (20)     3169 2024-04-02 07:43:54.000000 redturtle.prenotazioni-2.6.0/src/redturtle/prenotazioni/browser/prenotazione.py
+-rw-r--r--   0 cekk       (501) staff       (20)    10057 2024-04-02 07:43:54.000000 redturtle.prenotazioni-2.6.0/src/redturtle/prenotazioni/browser/prenotazione_add.py
+-rw-r--r--   0 cekk       (501) staff       (20)     5252 2024-04-02 07:43:54.000000 redturtle.prenotazioni-2.6.0/src/redturtle/prenotazioni/browser/prenotazione_move.py
+-rw-r--r--   0 cekk       (501) staff       (20)     2721 2024-04-02 07:43:54.000000 redturtle.prenotazioni-2.6.0/src/redturtle/prenotazioni/browser/prenotazione_print.py
+-rw-r--r--   0 cekk       (501) staff       (20)    37552 2024-04-02 07:43:54.000000 redturtle.prenotazioni-2.6.0/src/redturtle/prenotazioni/browser/prenotazioni_context_state.py
+-rw-r--r--   0 cekk       (501) staff       (20)     1735 2024-04-02 07:43:54.000000 redturtle.prenotazioni-2.6.0/src/redturtle/prenotazioni/browser/prenotazioni_portal_state.py
+-rw-r--r--   0 cekk       (501) staff       (20)    13800 2024-04-02 07:43:54.000000 redturtle.prenotazioni-2.6.0/src/redturtle/prenotazioni/browser/prenotazioni_search.py
+drwxr-xr-x   0 cekk       (501) staff       (20)        0 2024-04-02 07:43:54.778153 redturtle.prenotazioni-2.6.0/src/redturtle/prenotazioni/browser/static/
+-rw-r--r--   0 cekk       (501) staff       (20)        0 2024-04-02 07:43:54.000000 redturtle.prenotazioni-2.6.0/src/redturtle/prenotazioni/browser/static/.gitkeep
+-rw-r--r--   0 cekk       (501) staff       (20)      364 2024-04-02 07:43:54.000000 redturtle.prenotazioni-2.6.0/src/redturtle/prenotazioni/browser/static/calendar-add.png
+-rw-r--r--   0 cekk       (501) staff       (20)      503 2024-04-02 07:43:54.000000 redturtle.prenotazioni-2.6.0/src/redturtle/prenotazioni/browser/static/calendar-icon.png
+-rw-r--r--   0 cekk       (501) staff       (20)      266 2024-04-02 07:43:54.000000 redturtle.prenotazioni-2.6.0/src/redturtle/prenotazioni/browser/static/cross-icon.png
+-rw-r--r--   0 cekk       (501) staff       (20)     9794 2024-04-02 07:43:54.000000 redturtle.prenotazioni-2.6.0/src/redturtle/prenotazioni/browser/static/redturtle-reservation.css
+-rw-r--r--   0 cekk       (501) staff       (20)     1600 2024-04-02 07:43:54.000000 redturtle.prenotazioni-2.6.0/src/redturtle/prenotazioni/browser/static/redturtle-reservation.js
+-rw-r--r--   0 cekk       (501) staff       (20)      922 2024-04-02 07:43:54.000000 redturtle.prenotazioni-2.6.0/src/redturtle/prenotazioni/browser/static/times-solid.png
+drwxr-xr-x   0 cekk       (501) staff       (20)        0 2024-04-02 07:43:54.763108 redturtle.prenotazioni-2.6.0/src/redturtle/prenotazioni/browser/static/widget/
+drwxr-xr-x   0 cekk       (501) staff       (20)        0 2024-04-02 07:43:54.763045 redturtle.prenotazioni-2.6.0/src/redturtle/prenotazioni/browser/static/widget/dist/
+drwxr-xr-x   0 cekk       (501) staff       (20)        0 2024-04-02 07:43:54.778898 redturtle.prenotazioni-2.6.0/src/redturtle/prenotazioni/browser/static/widget/dist/prod/
+-rw-r--r--   0 cekk       (501) staff       (20)     3239 2024-04-02 07:43:54.000000 redturtle.prenotazioni-2.6.0/src/redturtle/prenotazioni/browser/static/widget/dist/prod/main.css
+-rw-r--r--   0 cekk       (501) staff       (20)     3808 2024-04-02 07:43:54.000000 redturtle.prenotazioni-2.6.0/src/redturtle/prenotazioni/browser/static/widget/dist/prod/main.css.map
+-rw-r--r--   0 cekk       (501) staff       (20)   349785 2024-04-02 07:43:54.000000 redturtle.prenotazioni-2.6.0/src/redturtle/prenotazioni/browser/static/widget/dist/prod/main.js
+-rw-r--r--   0 cekk       (501) staff       (20)      148 2024-04-02 07:43:54.000000 redturtle.prenotazioni-2.6.0/src/redturtle/prenotazioni/browser/static/widget/dist/prod/main.js.map
+drwxr-xr-x   0 cekk       (501) staff       (20)        0 2024-04-02 07:43:54.779040 redturtle.prenotazioni-2.6.0/src/redturtle/prenotazioni/browser/static/widget/js/
+drwxr-xr-x   0 cekk       (501) staff       (20)        0 2024-04-02 07:43:54.779186 redturtle.prenotazioni-2.6.0/src/redturtle/prenotazioni/browser/static/widget/js/WidgetContainer/
+-rw-r--r--   0 cekk       (501) staff       (20)     5095 2024-04-02 07:43:54.000000 redturtle.prenotazioni-2.6.0/src/redturtle/prenotazioni/browser/static/widget/js/WidgetContainer/index.js
+drwxr-xr-x   0 cekk       (501) staff       (20)        0 2024-04-02 07:43:54.779477 redturtle.prenotazioni-2.6.0/src/redturtle/prenotazioni/browser/static/widget/js/WidgetDataContainer/
+-rw-r--r--   0 cekk       (501) staff       (20)     4705 2024-04-02 07:43:54.000000 redturtle.prenotazioni-2.6.0/src/redturtle/prenotazioni/browser/static/widget/js/WidgetDataContainer/index.js
+-rw-r--r--   0 cekk       (501) staff       (20)     1059 2024-04-02 07:43:54.000000 redturtle.prenotazioni-2.6.0/src/redturtle/prenotazioni/browser/static/widget/js/WidgetDataContainer/index.less
+drwxr-xr-x   0 cekk       (501) staff       (20)        0 2024-04-02 07:43:54.780693 redturtle.prenotazioni-2.6.0/src/redturtle/prenotazioni/browser/static/widget/js/fields/
+-rw-r--r--   0 cekk       (501) staff       (20)     3010 2024-04-02 07:43:54.000000 redturtle.prenotazioni-2.6.0/src/redturtle/prenotazioni/browser/static/widget/js/fields/DaysTableField.js
+-rw-r--r--   0 cekk       (501) staff       (20)      204 2024-04-02 07:43:54.000000 redturtle.prenotazioni-2.6.0/src/redturtle/prenotazioni/browser/static/widget/js/fields/DaysTableField.less
+-rw-r--r--   0 cekk       (501) staff       (20)     2874 2024-04-02 07:43:54.000000 redturtle.prenotazioni-2.6.0/src/redturtle/prenotazioni/browser/static/widget/js/fields/GatesField.js
+-rw-r--r--   0 cekk       (501) staff       (20)      401 2024-04-02 07:43:54.000000 redturtle.prenotazioni-2.6.0/src/redturtle/prenotazioni/browser/static/widget/js/fields/GatesField.less
+-rw-r--r--   0 cekk       (501) staff       (20)     1888 2024-04-02 07:43:54.000000 redturtle.prenotazioni-2.6.0/src/redturtle/prenotazioni/browser/static/widget/js/fields/IntervalSelectorField.js
+-rw-r--r--   0 cekk       (501) staff       (20)      314 2024-04-02 07:43:54.000000 redturtle.prenotazioni-2.6.0/src/redturtle/prenotazioni/browser/static/widget/js/fields/IntervalSelectorField.less
+-rw-r--r--   0 cekk       (501) staff       (20)     4187 2024-04-02 07:43:54.000000 redturtle.prenotazioni-2.6.0/src/redturtle/prenotazioni/browser/static/widget/js/fields/PauseTableField.js
+-rw-r--r--   0 cekk       (501) staff       (20)      337 2024-04-02 07:43:54.000000 redturtle.prenotazioni-2.6.0/src/redturtle/prenotazioni/browser/static/widget/js/fields/PauseTableField.less
+-rw-r--r--   0 cekk       (501) staff       (20)     1745 2024-04-02 07:43:54.000000 redturtle.prenotazioni-2.6.0/src/redturtle/prenotazioni/browser/static/widget/js/fields/SelectField.js
+-rw-r--r--   0 cekk       (501) staff       (20)      961 2024-04-02 07:43:54.000000 redturtle.prenotazioni-2.6.0/src/redturtle/prenotazioni/browser/static/widget/js/fields/TextLineField.js
+-rw-r--r--   0 cekk       (501) staff       (20)     1261 2024-04-02 07:43:54.000000 redturtle.prenotazioni-2.6.0/src/redturtle/prenotazioni/browser/static/widget/js/index.js
+drwxr-xr-x   0 cekk       (501) staff       (20)        0 2024-04-02 07:43:54.780933 redturtle.prenotazioni-2.6.0/src/redturtle/prenotazioni/browser/static/widget/js/utils/
+-rw-r--r--   0 cekk       (501) staff       (20)      941 2024-04-02 07:43:54.000000 redturtle.prenotazioni-2.6.0/src/redturtle/prenotazioni/browser/static/widget/js/utils/i18n.js
+-rw-r--r--   0 cekk       (501) staff       (20)      298 2024-04-02 07:43:54.000000 redturtle.prenotazioni-2.6.0/src/redturtle/prenotazioni/browser/static/widget/js/utils/widgetContext.js
+drwxr-xr-x   0 cekk       (501) staff       (20)        0 2024-04-02 07:43:54.781377 redturtle.prenotazioni-2.6.0/src/redturtle/prenotazioni/browser/stats/
+-rw-r--r--   0 cekk       (501) staff       (20)       24 2024-04-02 07:43:54.000000 redturtle.prenotazioni-2.6.0/src/redturtle/prenotazioni/browser/stats/__init__.py
+-rw-r--r--   0 cekk       (501) staff       (20)      698 2024-04-02 07:43:54.000000 redturtle.prenotazioni-2.6.0/src/redturtle/prenotazioni/browser/stats/booking_stats.pt
+-rw-r--r--   0 cekk       (501) staff       (20)     3863 2024-04-02 07:43:54.000000 redturtle.prenotazioni-2.6.0/src/redturtle/prenotazioni/browser/stats/booking_stats.py
+-rw-r--r--   0 cekk       (501) staff       (20)      575 2024-04-02 07:43:54.000000 redturtle.prenotazioni-2.6.0/src/redturtle/prenotazioni/browser/stats/configure.zcml
+drwxr-xr-x   0 cekk       (501) staff       (20)        0 2024-04-02 07:43:54.782937 redturtle.prenotazioni-2.6.0/src/redturtle/prenotazioni/browser/templates/
+-rw-r--r--   0 cekk       (501) staff       (20)     2836 2024-04-02 07:43:54.000000 redturtle.prenotazioni-2.6.0/src/redturtle/prenotazioni/browser/templates/booking_type_radio_widget.pt
+-rw-r--r--   0 cekk       (501) staff       (20)     1518 2024-04-02 07:43:54.000000 redturtle.prenotazioni-2.6.0/src/redturtle/prenotazioni/browser/templates/custom_dgf_input.pt
+-rw-r--r--   0 cekk       (501) staff       (20)     4828 2024-04-02 07:43:54.000000 redturtle.prenotazioni-2.6.0/src/redturtle/prenotazioni/browser/templates/delete_reservation.pt
+-rw-r--r--   0 cekk       (501) staff       (20)     2417 2024-04-02 07:43:54.000000 redturtle.prenotazioni-2.6.0/src/redturtle/prenotazioni/browser/templates/manager_notification_mail.pt
+-rw-r--r--   0 cekk       (501) staff       (20)       48 2024-04-02 07:43:54.000000 redturtle.prenotazioni-2.6.0/src/redturtle/prenotazioni/browser/templates/nofollow.pt
+-rw-r--r--   0 cekk       (501) staff       (20)     7714 2024-04-02 07:43:54.000000 redturtle.prenotazioni-2.6.0/src/redturtle/prenotazioni/browser/templates/prenotazione.pt
+-rw-r--r--   0 cekk       (501) staff       (20)     9592 2024-04-02 07:43:54.000000 redturtle.prenotazioni-2.6.0/src/redturtle/prenotazioni/browser/templates/prenotazione_add.pt
+-rw-r--r--   0 cekk       (501) staff       (20)    16384 2024-04-02 07:43:54.000000 redturtle.prenotazioni-2.6.0/src/redturtle/prenotazioni/browser/templates/prenotazione_macros.pt
+-rw-r--r--   0 cekk       (501) staff       (20)     2227 2024-04-02 07:43:54.000000 redturtle.prenotazioni-2.6.0/src/redturtle/prenotazioni/browser/templates/prenotazione_move.pt
+-rw-r--r--   0 cekk       (501) staff       (20)     5299 2024-04-02 07:43:54.000000 redturtle.prenotazioni-2.6.0/src/redturtle/prenotazioni/browser/templates/prenotazione_print.pt
+-rw-r--r--   0 cekk       (501) staff       (20)     5241 2024-04-02 07:43:54.000000 redturtle.prenotazioni-2.6.0/src/redturtle/prenotazioni/browser/templates/prenotazioni_search.pt
+-rw-r--r--   0 cekk       (501) staff       (20)     1858 2024-04-02 07:43:54.000000 redturtle.prenotazioni-2.6.0/src/redturtle/prenotazioni/browser/templates/week.pt
+-rw-r--r--   0 cekk       (501) staff       (20)      362 2024-04-02 07:43:54.000000 redturtle.prenotazioni-2.6.0/src/redturtle/prenotazioni/browser/templates/week_table_overrides_widget_input.pt
+drwxr-xr-x   0 cekk       (501) staff       (20)        0 2024-04-02 07:43:54.783234 redturtle.prenotazioni-2.6.0/src/redturtle/prenotazioni/browser/utilities/
+-rw-r--r--   0 cekk       (501) staff       (20)        0 2024-04-02 07:43:54.000000 redturtle.prenotazioni-2.6.0/src/redturtle/prenotazioni/browser/utilities/__init__.py
+-rw-r--r--   0 cekk       (501) staff       (20)      494 2024-04-02 07:43:54.000000 redturtle.prenotazioni-2.6.0/src/redturtle/prenotazioni/browser/utilities/configure.zcml
+-rw-r--r--   0 cekk       (501) staff       (20)     1676 2024-04-02 07:43:54.000000 redturtle.prenotazioni-2.6.0/src/redturtle/prenotazioni/browser/utilities/notify_upcoming_bookings.py
+-rw-r--r--   0 cekk       (501) staff       (20)     8087 2024-04-02 07:43:54.000000 redturtle.prenotazioni-2.6.0/src/redturtle/prenotazioni/browser/vacations.py
+-rw-r--r--   0 cekk       (501) staff       (20)     1524 2024-04-02 07:43:54.000000 redturtle.prenotazioni-2.6.0/src/redturtle/prenotazioni/browser/viewlets.py
+-rw-r--r--   0 cekk       (501) staff       (20)    10867 2024-04-02 07:43:54.000000 redturtle.prenotazioni-2.6.0/src/redturtle/prenotazioni/browser/week.py
+-rw-r--r--   0 cekk       (501) staff       (20)     1193 2024-04-02 07:43:54.000000 redturtle.prenotazioni-2.6.0/src/redturtle/prenotazioni/browser/widget.py
+-rw-r--r--   0 cekk       (501) staff       (20)     6310 2024-04-02 07:43:54.000000 redturtle.prenotazioni-2.6.0/src/redturtle/prenotazioni/browser/z3c_custom_widget.py
+-rw-r--r--   0 cekk       (501) staff       (20)      485 2024-04-02 07:43:54.000000 redturtle.prenotazioni-2.6.0/src/redturtle/prenotazioni/config.py
+-rw-r--r--   0 cekk       (501) staff       (20)     2049 2024-04-02 07:43:54.000000 redturtle.prenotazioni-2.6.0/src/redturtle/prenotazioni/configure.zcml
+drwxr-xr-x   0 cekk       (501) staff       (20)        0 2024-04-02 07:43:54.784309 redturtle.prenotazioni-2.6.0/src/redturtle/prenotazioni/content/
+-rw-r--r--   0 cekk       (501) staff       (20)       24 2024-04-02 07:43:54.000000 redturtle.prenotazioni-2.6.0/src/redturtle/prenotazioni/content/__init__.py
+-rw-r--r--   0 cekk       (501) staff       (20)      111 2024-04-02 07:43:54.000000 redturtle.prenotazioni-2.6.0/src/redturtle/prenotazioni/content/booking_type.py
+-rw-r--r--   0 cekk       (501) staff       (20)     1537 2024-04-02 07:43:54.000000 redturtle.prenotazioni-2.6.0/src/redturtle/prenotazioni/content/pause.py
+-rw-r--r--   0 cekk       (501) staff       (20)     7504 2024-04-02 07:43:54.000000 redturtle.prenotazioni-2.6.0/src/redturtle/prenotazioni/content/prenotazione.py
+-rw-r--r--   0 cekk       (501) staff       (20)     1251 2024-04-02 07:43:54.000000 redturtle.prenotazioni-2.6.0/src/redturtle/prenotazioni/content/prenotazione_type.py
+-rw-r--r--   0 cekk       (501) staff       (20)      367 2024-04-02 07:43:54.000000 redturtle.prenotazioni-2.6.0/src/redturtle/prenotazioni/content/prenotazioni_day.py
+-rw-r--r--   0 cekk       (501) staff       (20)    18932 2024-04-02 07:43:54.000000 redturtle.prenotazioni-2.6.0/src/redturtle/prenotazioni/content/prenotazioni_folder.py
+-rw-r--r--   0 cekk       (501) staff       (20)      371 2024-04-02 07:43:54.000000 redturtle.prenotazioni-2.6.0/src/redturtle/prenotazioni/content/prenotazioni_week.py
+-rw-r--r--   0 cekk       (501) staff       (20)      371 2024-04-02 07:43:54.000000 redturtle.prenotazioni-2.6.0/src/redturtle/prenotazioni/content/prenotazioni_year.py
+-rw-r--r--   0 cekk       (501) staff       (20)     8518 2024-04-02 07:43:54.000000 redturtle.prenotazioni-2.6.0/src/redturtle/prenotazioni/content/validators.py
+drwxr-xr-x   0 cekk       (501) staff       (20)        0 2024-04-02 07:43:54.784846 redturtle.prenotazioni-2.6.0/src/redturtle/prenotazioni/demo/
+-rw-r--r--   0 cekk       (501) staff       (20)       77 2024-04-02 07:43:54.000000 redturtle.prenotazioni-2.6.0/src/redturtle/prenotazioni/demo/__init__.py
+-rw-r--r--   0 cekk       (501) staff       (20)     1088 2024-04-02 07:43:54.000000 redturtle.prenotazioni-2.6.0/src/redturtle/prenotazioni/demo/configure.zcml
+-rw-r--r--   0 cekk       (501) staff       (20)      227 2024-04-02 07:43:54.000000 redturtle.prenotazioni-2.6.0/src/redturtle/prenotazioni/demo/interfaces.py
+drwxr-xr-x   0 cekk       (501) staff       (20)        0 2024-04-02 07:43:54.763868 redturtle.prenotazioni-2.6.0/src/redturtle/prenotazioni/demo/profiles/
+drwxr-xr-x   0 cekk       (501) staff       (20)        0 2024-04-02 07:43:54.785065 redturtle.prenotazioni-2.6.0/src/redturtle/prenotazioni/demo/profiles/default/
+-rw-r--r--   0 cekk       (501) staff       (20)      208 2024-04-02 07:43:54.000000 redturtle.prenotazioni-2.6.0/src/redturtle/prenotazioni/demo/profiles/default/browserlayer.xml
+-rw-r--r--   0 cekk       (501) staff       (20)       88 2024-04-02 07:43:54.000000 redturtle.prenotazioni-2.6.0/src/redturtle/prenotazioni/demo/profiles/default/metadata.xml
+drwxr-xr-x   0 cekk       (501) staff       (20)        0 2024-04-02 07:43:54.785178 redturtle.prenotazioni-2.6.0/src/redturtle/prenotazioni/demo/profiles/uninstall/
+-rw-r--r--   0 cekk       (501) staff       (20)      133 2024-04-02 07:43:54.000000 redturtle.prenotazioni-2.6.0/src/redturtle/prenotazioni/demo/profiles/uninstall/browserlayer.xml
+-rw-r--r--   0 cekk       (501) staff       (20)      630 2024-04-02 07:43:54.000000 redturtle.prenotazioni-2.6.0/src/redturtle/prenotazioni/demo/setuphandlers.py
+-rw-r--r--   0 cekk       (501) staff       (20)     1347 2024-04-02 07:43:54.000000 redturtle.prenotazioni-2.6.0/src/redturtle/prenotazioni/demo/smsdemo.py
+drwxr-xr-x   0 cekk       (501) staff       (20)        0 2024-04-02 07:43:54.785755 redturtle.prenotazioni-2.6.0/src/redturtle/prenotazioni/events/
+-rw-r--r--   0 cekk       (501) staff       (20)      270 2024-04-02 07:43:54.000000 redturtle.prenotazioni-2.6.0/src/redturtle/prenotazioni/events/__init__.py
+-rw-r--r--   0 cekk       (501) staff       (20)     1615 2024-04-02 07:43:54.000000 redturtle.prenotazioni-2.6.0/src/redturtle/prenotazioni/events/configure.zcml
+-rw-r--r--   0 cekk       (501) staff       (20)     2128 2024-04-02 07:43:54.000000 redturtle.prenotazioni-2.6.0/src/redturtle/prenotazioni/events/events_logger.py
+-rw-r--r--   0 cekk       (501) staff       (20)     1907 2024-04-02 07:43:54.000000 redturtle.prenotazioni-2.6.0/src/redturtle/prenotazioni/events/prenotazione.py
+-rw-r--r--   0 cekk       (501) staff       (20)     1189 2024-04-02 07:43:54.000000 redturtle.prenotazioni-2.6.0/src/redturtle/prenotazioni/events/prenotazioni_folder.py
+drwxr-xr-x   0 cekk       (501) staff       (20)        0 2024-04-02 07:43:54.785997 redturtle.prenotazioni-2.6.0/src/redturtle/prenotazioni/exceptions/
+-rw-r--r--   0 cekk       (501) staff       (20)      129 2024-04-02 07:43:54.000000 redturtle.prenotazioni-2.6.0/src/redturtle/prenotazioni/exceptions/__init__.py
+-rw-r--r--   0 cekk       (501) staff       (20)      712 2024-04-02 07:43:54.000000 redturtle.prenotazioni-2.6.0/src/redturtle/prenotazioni/exceptions/booker.py
+drwxr-xr-x   0 cekk       (501) staff       (20)        0 2024-04-02 07:43:54.786363 redturtle.prenotazioni-2.6.0/src/redturtle/prenotazioni/indexers/
+-rw-r--r--   0 cekk       (501) staff       (20)       24 2024-04-02 07:43:54.000000 redturtle.prenotazioni-2.6.0/src/redturtle/prenotazioni/indexers/__init__.py
+-rw-r--r--   0 cekk       (501) staff       (20)      476 2024-04-02 07:43:54.000000 redturtle.prenotazioni-2.6.0/src/redturtle/prenotazioni/indexers/configure.zcml
+-rw-r--r--   0 cekk       (501) staff       (20)     1410 2024-04-02 07:43:54.000000 redturtle.prenotazioni-2.6.0/src/redturtle/prenotazioni/indexers/prenotazione.py
+-rw-r--r--   0 cekk       (501) staff       (20)     1445 2024-04-02 07:43:54.000000 redturtle.prenotazioni-2.6.0/src/redturtle/prenotazioni/interfaces.py
+drwxr-xr-x   0 cekk       (501) staff       (20)        0 2024-04-02 07:43:54.787689 redturtle.prenotazioni-2.6.0/src/redturtle/prenotazioni/io_tools/
+-rw-r--r--   0 cekk       (501) staff       (20)     5302 2024-04-02 07:43:54.000000 redturtle.prenotazioni-2.6.0/src/redturtle/prenotazioni/io_tools/README.md
+-rw-r--r--   0 cekk       (501) staff       (20)      207 2024-04-02 07:43:54.000000 redturtle.prenotazioni-2.6.0/src/redturtle/prenotazioni/io_tools/__init__.py
+-rw-r--r--   0 cekk       (501) staff       (20)     9443 2024-04-02 07:43:54.000000 redturtle.prenotazioni-2.6.0/src/redturtle/prenotazioni/io_tools/api.py
+-rw-r--r--   0 cekk       (501) staff       (20)     1035 2024-04-02 07:43:54.000000 redturtle.prenotazioni-2.6.0/src/redturtle/prenotazioni/io_tools/cli.py
+-rw-r--r--   0 cekk       (501) staff       (20)    16384 2024-04-02 07:43:54.000000 redturtle.prenotazioni-2.6.0/src/redturtle/prenotazioni/io_tools/io.db
+-rw-r--r--   0 cekk       (501) staff       (20)       45 2024-04-02 07:43:54.000000 redturtle.prenotazioni-2.6.0/src/redturtle/prenotazioni/io_tools/io_tools.py
+-rw-r--r--   0 cekk       (501) staff       (20)     1945 2024-04-02 07:43:54.000000 redturtle.prenotazioni-2.6.0/src/redturtle/prenotazioni/io_tools/monkey.py
+-rw-r--r--   0 cekk       (501) staff       (20)     2833 2024-04-02 07:43:54.000000 redturtle.prenotazioni-2.6.0/src/redturtle/prenotazioni/io_tools/rdbms.py
+-rw-r--r--   0 cekk       (501) staff       (20)    27521 2024-04-02 07:43:54.000000 redturtle.prenotazioni-2.6.0/src/redturtle/prenotazioni/io_tools/spec.yaml
+-rw-r--r--   0 cekk       (501) staff       (20)      961 2024-04-02 07:43:54.000000 redturtle.prenotazioni-2.6.0/src/redturtle/prenotazioni/io_tools/storage.py
+drwxr-xr-x   0 cekk       (501) staff       (20)        0 2024-04-02 07:43:54.788224 redturtle.prenotazioni-2.6.0/src/redturtle/prenotazioni/locales/
+drwxr-xr-x   0 cekk       (501) staff       (20)        0 2024-04-02 07:43:54.764291 redturtle.prenotazioni-2.6.0/src/redturtle/prenotazioni/locales/en/
+drwxr-xr-x   0 cekk       (501) staff       (20)        0 2024-04-02 07:43:54.788482 redturtle.prenotazioni-2.6.0/src/redturtle/prenotazioni/locales/en/LC_MESSAGES/
+-rw-r--r--   0 cekk       (501) staff       (20)      509 2024-04-02 07:43:54.000000 redturtle.prenotazioni-2.6.0/src/redturtle/prenotazioni/locales/en/LC_MESSAGES/redturtle.prenotazioni.mo
+-rw-r--r--   0 cekk       (501) staff       (20)    56619 2024-04-02 07:43:54.000000 redturtle.prenotazioni-2.6.0/src/redturtle/prenotazioni/locales/en/LC_MESSAGES/redturtle.prenotazioni.po
+drwxr-xr-x   0 cekk       (501) staff       (20)        0 2024-04-02 07:43:54.764397 redturtle.prenotazioni-2.6.0/src/redturtle/prenotazioni/locales/it/
+drwxr-xr-x   0 cekk       (501) staff       (20)        0 2024-04-02 07:43:54.789029 redturtle.prenotazioni-2.6.0/src/redturtle/prenotazioni/locales/it/LC_MESSAGES/
+-rw-r--r--   0 cekk       (501) staff       (20)      588 2024-04-02 07:43:54.000000 redturtle.prenotazioni-2.6.0/src/redturtle/prenotazioni/locales/it/LC_MESSAGES/plone.mo
+-rw-r--r--   0 cekk       (501) staff       (20)      623 2024-04-02 07:43:54.000000 redturtle.prenotazioni-2.6.0/src/redturtle/prenotazioni/locales/it/LC_MESSAGES/plone.po
+-rw-r--r--   0 cekk       (501) staff       (20)    30940 2024-04-02 07:43:54.000000 redturtle.prenotazioni-2.6.0/src/redturtle/prenotazioni/locales/it/LC_MESSAGES/redturtle.prenotazioni.mo
+-rw-r--r--   0 cekk       (501) staff       (20)    73109 2024-04-02 07:43:54.000000 redturtle.prenotazioni-2.6.0/src/redturtle/prenotazioni/locales/it/LC_MESSAGES/redturtle.prenotazioni.po
+-rw-r--r--   0 cekk       (501) staff       (20)      830 2024-04-02 07:43:54.000000 redturtle.prenotazioni-2.6.0/src/redturtle/prenotazioni/locales/manual.pot
+-rw-r--r--   0 cekk       (501) staff       (20)    56728 2024-04-02 07:43:54.000000 redturtle.prenotazioni-2.6.0/src/redturtle/prenotazioni/locales/redturtle.prenotazioni.pot
+-rw-r--r--   0 cekk       (501) staff       (20)     1618 2024-04-02 07:43:54.000000 redturtle.prenotazioni-2.6.0/src/redturtle/prenotazioni/locales/update.py
+-rwxr-xr-x   0 cekk       (501) staff       (20)      521 2024-04-02 07:43:54.000000 redturtle.prenotazioni-2.6.0/src/redturtle/prenotazioni/locales/update.sh
+drwxr-xr-x   0 cekk       (501) staff       (20)        0 2024-04-02 07:43:54.789303 redturtle.prenotazioni-2.6.0/src/redturtle/prenotazioni/monkeypatcher/
+-rw-r--r--   0 cekk       (501) staff       (20)        0 2024-04-02 07:43:54.000000 redturtle.prenotazioni-2.6.0/src/redturtle/prenotazioni/monkeypatcher/__init__.py
+-rw-r--r--   0 cekk       (501) staff       (20)      499 2024-04-02 07:43:54.000000 redturtle.prenotazioni-2.6.0/src/redturtle/prenotazioni/monkeypatcher/configure.zcml
+-rw-r--r--   0 cekk       (501) staff       (20)     1565 2024-04-02 07:43:54.000000 redturtle.prenotazioni-2.6.0/src/redturtle/prenotazioni/permissions.zcml
+-rw-r--r--   0 cekk       (501) staff       (20)      507 2024-04-02 07:43:54.000000 redturtle.prenotazioni-2.6.0/src/redturtle/prenotazioni/prenotazione_event.py
+drwxr-xr-x   0 cekk       (501) staff       (20)        0 2024-04-02 07:43:54.765298 redturtle.prenotazioni-2.6.0/src/redturtle/prenotazioni/profiles/
+drwxr-xr-x   0 cekk       (501) staff       (20)        0 2024-04-02 07:43:54.790391 redturtle.prenotazioni-2.6.0/src/redturtle/prenotazioni/profiles/default/
+-rw-r--r--   0 cekk       (501) staff       (20)     2656 2024-04-02 07:43:54.000000 redturtle.prenotazioni-2.6.0/src/redturtle/prenotazioni/profiles/default/actions.xml
+-rw-r--r--   0 cekk       (501) staff       (20)      185 2024-04-02 07:43:54.000000 redturtle.prenotazioni-2.6.0/src/redturtle/prenotazioni/profiles/default/browserlayer.xml
+-rw-r--r--   0 cekk       (501) staff       (20)      349 2024-04-02 07:43:54.000000 redturtle.prenotazioni-2.6.0/src/redturtle/prenotazioni/profiles/default/catalog.xml
+-rw-r--r--   0 cekk       (501) staff       (20)       71 2024-04-02 07:43:54.000000 redturtle.prenotazioni-2.6.0/src/redturtle/prenotazioni/profiles/default/contentrules.xml
+-rw-r--r--   0 cekk       (501) staff       (20)      325 2024-04-02 07:43:54.000000 redturtle.prenotazioni-2.6.0/src/redturtle/prenotazioni/profiles/default/metadata.xml
+drwxr-xr-x   0 cekk       (501) staff       (20)        0 2024-04-02 07:43:54.790758 redturtle.prenotazioni-2.6.0/src/redturtle/prenotazioni/profiles/default/registry/
+-rw-r--r--   0 cekk       (501) staff       (20)     5140 2024-04-02 07:43:54.000000 redturtle.prenotazioni-2.6.0/src/redturtle/prenotazioni/profiles/default/registry/caching.xml
+-rw-r--r--   0 cekk       (501) staff       (20)     2015 2024-04-02 07:43:54.000000 redturtle.prenotazioni-2.6.0/src/redturtle/prenotazioni/profiles/default/registry/resources.xml
+-rw-r--r--   0 cekk       (501) staff       (20)     1001 2024-04-02 07:43:54.000000 redturtle.prenotazioni-2.6.0/src/redturtle/prenotazioni/profiles/default/registry/settings.xml
+-rw-r--r--   0 cekk       (501) staff       (20)     3277 2024-04-02 07:43:54.000000 redturtle.prenotazioni-2.6.0/src/redturtle/prenotazioni/profiles/default/rolemap.xml
+-rw-r--r--   0 cekk       (501) staff       (20)      277 2024-04-02 07:43:54.000000 redturtle.prenotazioni-2.6.0/src/redturtle/prenotazioni/profiles/default/sharing.xml
+drwxr-xr-x   0 cekk       (501) staff       (20)        0 2024-04-02 07:43:54.791396 redturtle.prenotazioni-2.6.0/src/redturtle/prenotazioni/profiles/default/types/
+-rw-r--r--   0 cekk       (501) staff       (20)     3607 2024-04-02 07:43:54.000000 redturtle.prenotazioni-2.6.0/src/redturtle/prenotazioni/profiles/default/types/Prenotazione.xml
+-rw-r--r--   0 cekk       (501) staff       (20)     2983 2024-04-02 07:43:54.000000 redturtle.prenotazioni-2.6.0/src/redturtle/prenotazioni/profiles/default/types/PrenotazioneType.xml
+-rw-r--r--   0 cekk       (501) staff       (20)     3861 2024-04-02 07:43:54.000000 redturtle.prenotazioni-2.6.0/src/redturtle/prenotazioni/profiles/default/types/PrenotazioniDay.xml
+-rw-r--r--   0 cekk       (501) staff       (20)     3257 2024-04-02 07:43:54.000000 redturtle.prenotazioni-2.6.0/src/redturtle/prenotazioni/profiles/default/types/PrenotazioniFolder.xml
+-rw-r--r--   0 cekk       (501) staff       (20)     3845 2024-04-02 07:43:54.000000 redturtle.prenotazioni-2.6.0/src/redturtle/prenotazioni/profiles/default/types/PrenotazioniWeek.xml
+-rw-r--r--   0 cekk       (501) staff       (20)     3846 2024-04-02 07:43:54.000000 redturtle.prenotazioni-2.6.0/src/redturtle/prenotazioni/profiles/default/types/PrenotazioniYear.xml
+-rw-r--r--   0 cekk       (501) staff       (20)      713 2024-04-02 07:43:54.000000 redturtle.prenotazioni-2.6.0/src/redturtle/prenotazioni/profiles/default/types.xml
+drwxr-xr-x   0 cekk       (501) staff       (20)        0 2024-04-02 07:43:54.764866 redturtle.prenotazioni-2.6.0/src/redturtle/prenotazioni/profiles/default/workflows/
+drwxr-xr-x   0 cekk       (501) staff       (20)        0 2024-04-02 07:43:54.791502 redturtle.prenotazioni-2.6.0/src/redturtle/prenotazioni/profiles/default/workflows/prenotazioni_workflow/
+-rw-r--r--   0 cekk       (501) staff       (20)    12711 2024-04-02 07:43:54.000000 redturtle.prenotazioni-2.6.0/src/redturtle/prenotazioni/profiles/default/workflows/prenotazioni_workflow/definition.xml
+drwxr-xr-x   0 cekk       (501) staff       (20)        0 2024-04-02 07:43:54.791613 redturtle.prenotazioni-2.6.0/src/redturtle/prenotazioni/profiles/default/workflows/prenotazionifolder_workflow/
+-rw-r--r--   0 cekk       (501) staff       (20)     8877 2024-04-02 07:43:54.000000 redturtle.prenotazioni-2.6.0/src/redturtle/prenotazioni/profiles/default/workflows/prenotazionifolder_workflow/definition.xml
+-rw-r--r--   0 cekk       (501) staff       (20)      613 2024-04-02 07:43:54.000000 redturtle.prenotazioni-2.6.0/src/redturtle/prenotazioni/profiles/default/workflows.xml
+drwxr-xr-x   0 cekk       (501) staff       (20)        0 2024-04-02 07:43:54.791718 redturtle.prenotazioni-2.6.0/src/redturtle/prenotazioni/profiles/to_1402/
+-rw-r--r--   0 cekk       (501) staff       (20)     1508 2024-04-02 07:43:54.000000 redturtle.prenotazioni-2.6.0/src/redturtle/prenotazioni/profiles/to_1402/contentrules.xml
+drwxr-xr-x   0 cekk       (501) staff       (20)        0 2024-04-02 07:43:54.791826 redturtle.prenotazioni-2.6.0/src/redturtle/prenotazioni/profiles/to_1500/
+-rw-r--r--   0 cekk       (501) staff       (20)      226 2024-04-02 07:43:54.000000 redturtle.prenotazioni-2.6.0/src/redturtle/prenotazioni/profiles/to_1500/types.xml
+drwxr-xr-x   0 cekk       (501) staff       (20)        0 2024-04-02 07:43:54.792038 redturtle.prenotazioni-2.6.0/src/redturtle/prenotazioni/profiles/to_2005/
+-rw-r--r--   0 cekk       (501) staff       (20)       88 2024-04-02 07:43:54.000000 redturtle.prenotazioni-2.6.0/src/redturtle/prenotazioni/profiles/to_2005/metadata.xml
+-rw-r--r--   0 cekk       (501) staff       (20)      638 2024-04-02 07:43:54.000000 redturtle.prenotazioni-2.6.0/src/redturtle/prenotazioni/profiles/to_2005/rolemap.xml
+drwxr-xr-x   0 cekk       (501) staff       (20)        0 2024-04-02 07:43:54.792243 redturtle.prenotazioni-2.6.0/src/redturtle/prenotazioni/profiles/to_2006/
+-rw-r--r--   0 cekk       (501) staff       (20)       88 2024-04-02 07:43:54.000000 redturtle.prenotazioni-2.6.0/src/redturtle/prenotazioni/profiles/to_2006/metadata.xml
+drwxr-xr-x   0 cekk       (501) staff       (20)        0 2024-04-02 07:43:54.765236 redturtle.prenotazioni-2.6.0/src/redturtle/prenotazioni/profiles/to_2006/workflows/
+drwxr-xr-x   0 cekk       (501) staff       (20)        0 2024-04-02 07:43:54.792353 redturtle.prenotazioni-2.6.0/src/redturtle/prenotazioni/profiles/to_2006/workflows/prenotazioni_workflow/
+-rw-r--r--   0 cekk       (501) staff       (20)    12711 2024-04-02 07:43:54.000000 redturtle.prenotazioni-2.6.0/src/redturtle/prenotazioni/profiles/to_2006/workflows/prenotazioni_workflow/definition.xml
+-rw-r--r--   0 cekk       (501) staff       (20)      279 2024-04-02 07:43:54.000000 redturtle.prenotazioni-2.6.0/src/redturtle/prenotazioni/profiles/to_2006/workflows.xml
+drwxr-xr-x   0 cekk       (501) staff       (20)        0 2024-04-02 07:43:54.792468 redturtle.prenotazioni-2.6.0/src/redturtle/prenotazioni/profiles/uninstall/
+-rw-r--r--   0 cekk       (501) staff       (20)      125 2024-04-02 07:43:54.000000 redturtle.prenotazioni-2.6.0/src/redturtle/prenotazioni/profiles/uninstall/browserlayer.xml
+drwxr-xr-x   0 cekk       (501) staff       (20)        0 2024-04-02 07:43:54.792687 redturtle.prenotazioni-2.6.0/src/redturtle/prenotazioni/profiles/uninstall/registry/
+-rw-r--r--   0 cekk       (501) staff       (20)      431 2024-04-02 07:43:54.000000 redturtle.prenotazioni-2.6.0/src/redturtle/prenotazioni/profiles/uninstall/registry/resources.xml
+-rw-r--r--   0 cekk       (501) staff       (20)      152 2024-04-02 07:43:54.000000 redturtle.prenotazioni-2.6.0/src/redturtle/prenotazioni/profiles/uninstall/registry/settings.xml
+drwxr-xr-x   0 cekk       (501) staff       (20)        0 2024-04-02 07:43:54.792882 redturtle.prenotazioni-2.6.0/src/redturtle/prenotazioni/restapi/
+-rw-r--r--   0 cekk       (501) staff       (20)        0 2024-04-02 07:43:54.000000 redturtle.prenotazioni-2.6.0/src/redturtle/prenotazioni/restapi/__init__.py
+-rw-r--r--   0 cekk       (501) staff       (20)      199 2024-04-02 07:43:54.000000 redturtle.prenotazioni-2.6.0/src/redturtle/prenotazioni/restapi/configure.zcml
+drwxr-xr-x   0 cekk       (501) staff       (20)        0 2024-04-02 07:43:54.793065 redturtle.prenotazioni-2.6.0/src/redturtle/prenotazioni/restapi/serializers/
+-rw-r--r--   0 cekk       (501) staff       (20)        0 2024-04-02 07:43:54.000000 redturtle.prenotazioni-2.6.0/src/redturtle/prenotazioni/restapi/serializers/__init__.py
+drwxr-xr-x   0 cekk       (501) staff       (20)        0 2024-04-02 07:43:54.793686 redturtle.prenotazioni-2.6.0/src/redturtle/prenotazioni/restapi/serializers/adapters/
+-rw-r--r--   0 cekk       (501) staff       (20)        0 2024-04-02 07:43:54.000000 redturtle.prenotazioni-2.6.0/src/redturtle/prenotazioni/restapi/serializers/adapters/__init__.py
+-rw-r--r--   0 cekk       (501) staff       (20)      468 2024-04-02 07:43:54.000000 redturtle.prenotazioni-2.6.0/src/redturtle/prenotazioni/restapi/serializers/adapters/configure.zcml
+-rw-r--r--   0 cekk       (501) staff       (20)     7441 2024-04-02 07:43:54.000000 redturtle.prenotazioni-2.6.0/src/redturtle/prenotazioni/restapi/serializers/adapters/prenotazione.py
+-rw-r--r--   0 cekk       (501) staff       (20)      973 2024-04-02 07:43:54.000000 redturtle.prenotazioni-2.6.0/src/redturtle/prenotazioni/restapi/serializers/adapters/prenotazione_type.py
+-rw-r--r--   0 cekk       (501) staff       (20)      925 2024-04-02 07:43:54.000000 redturtle.prenotazioni-2.6.0/src/redturtle/prenotazioni/restapi/serializers/adapters/prenotazioni_folder.py
+-rw-r--r--   0 cekk       (501) staff       (20)     1721 2024-04-02 07:43:54.000000 redturtle.prenotazioni-2.6.0/src/redturtle/prenotazioni/restapi/serializers/adapters/slot.py
+-rw-r--r--   0 cekk       (501) staff       (20)      162 2024-04-02 07:43:54.000000 redturtle.prenotazioni-2.6.0/src/redturtle/prenotazioni/restapi/serializers/configure.zcml
+drwxr-xr-x   0 cekk       (501) staff       (20)        0 2024-04-02 07:43:54.793795 redturtle.prenotazioni-2.6.0/src/redturtle/prenotazioni/restapi/services/
+drwxr-xr-x   0 cekk       (501) staff       (20)        0 2024-04-02 07:43:54.794100 redturtle.prenotazioni-2.6.0/src/redturtle/prenotazioni/restapi/services/available_slots/
+-rw-r--r--   0 cekk       (501) staff       (20)        0 2024-04-02 07:43:54.000000 redturtle.prenotazioni-2.6.0/src/redturtle/prenotazioni/restapi/services/available_slots/__init__.py
+-rw-r--r--   0 cekk       (501) staff       (20)      352 2024-04-02 07:43:54.000000 redturtle.prenotazioni-2.6.0/src/redturtle/prenotazioni/restapi/services/available_slots/configure.zcml
+-rw-r--r--   0 cekk       (501) staff       (20)     3537 2024-04-02 07:43:54.000000 redturtle.prenotazioni-2.6.0/src/redturtle/prenotazioni/restapi/services/available_slots/get.py
+drwxr-xr-x   0 cekk       (501) staff       (20)        0 2024-04-02 07:43:54.794913 redturtle.prenotazioni-2.6.0/src/redturtle/prenotazioni/restapi/services/booking/
+-rw-r--r--   0 cekk       (501) staff       (20)        0 2024-04-02 07:43:54.000000 redturtle.prenotazioni-2.6.0/src/redturtle/prenotazioni/restapi/services/booking/__init__.py
+-rw-r--r--   0 cekk       (501) staff       (20)     6595 2024-04-02 07:43:54.000000 redturtle.prenotazioni-2.6.0/src/redturtle/prenotazioni/restapi/services/booking/add.py
+-rw-r--r--   0 cekk       (501) staff       (20)     1641 2024-04-02 07:43:54.000000 redturtle.prenotazioni-2.6.0/src/redturtle/prenotazioni/restapi/services/booking/configure.zcml
+-rw-r--r--   0 cekk       (501) staff       (20)     1209 2024-04-02 07:43:54.000000 redturtle.prenotazioni-2.6.0/src/redturtle/prenotazioni/restapi/services/booking/delete.py
+-rw-r--r--   0 cekk       (501) staff       (20)     1166 2024-04-02 07:43:54.000000 redturtle.prenotazioni-2.6.0/src/redturtle/prenotazioni/restapi/services/booking/get.py
+-rw-r--r--   0 cekk       (501) staff       (20)     1328 2024-04-02 07:43:54.000000 redturtle.prenotazioni-2.6.0/src/redturtle/prenotazioni/restapi/services/booking/move.py
+-rw-r--r--   0 cekk       (501) staff       (20)     1152 2024-04-02 07:43:54.000000 redturtle.prenotazioni-2.6.0/src/redturtle/prenotazioni/restapi/services/booking/notify_about_confirm.py
+-rw-r--r--   0 cekk       (501) staff       (20)      966 2024-04-02 07:43:54.000000 redturtle.prenotazioni-2.6.0/src/redturtle/prenotazioni/restapi/services/booking/vacation.py
+drwxr-xr-x   0 cekk       (501) staff       (20)        0 2024-04-02 07:43:54.795205 redturtle.prenotazioni-2.6.0/src/redturtle/prenotazioni/restapi/services/booking_schema/
+-rw-r--r--   0 cekk       (501) staff       (20)        0 2024-04-02 07:43:54.000000 redturtle.prenotazioni-2.6.0/src/redturtle/prenotazioni/restapi/services/booking_schema/__init__.py
+-rw-r--r--   0 cekk       (501) staff       (20)      404 2024-04-02 07:43:54.000000 redturtle.prenotazioni-2.6.0/src/redturtle/prenotazioni/restapi/services/booking_schema/configure.zcml
+-rw-r--r--   0 cekk       (501) staff       (20)     4916 2024-04-02 07:43:54.000000 redturtle.prenotazioni-2.6.0/src/redturtle/prenotazioni/restapi/services/booking_schema/get.py
+drwxr-xr-x   0 cekk       (501) staff       (20)        0 2024-04-02 07:43:54.795501 redturtle.prenotazioni-2.6.0/src/redturtle/prenotazioni/restapi/services/bookings/
+-rw-r--r--   0 cekk       (501) staff       (20)        0 2024-04-02 07:43:54.000000 redturtle.prenotazioni-2.6.0/src/redturtle/prenotazioni/restapi/services/bookings/__init__.py
+-rw-r--r--   0 cekk       (501) staff       (20)      548 2024-04-02 07:43:54.000000 redturtle.prenotazioni-2.6.0/src/redturtle/prenotazioni/restapi/services/bookings/configure.zcml
+-rw-r--r--   0 cekk       (501) staff       (20)     3898 2024-04-02 07:43:54.000000 redturtle.prenotazioni-2.6.0/src/redturtle/prenotazioni/restapi/services/bookings/search.py
+-rw-r--r--   0 cekk       (501) staff       (20)      336 2024-04-02 07:43:54.000000 redturtle.prenotazioni-2.6.0/src/redturtle/prenotazioni/restapi/services/configure.zcml
+drwxr-xr-x   0 cekk       (501) staff       (20)        0 2024-04-02 07:43:54.795799 redturtle.prenotazioni-2.6.0/src/redturtle/prenotazioni/restapi/services/day/
+-rw-r--r--   0 cekk       (501) staff       (20)        0 2024-04-02 07:43:54.000000 redturtle.prenotazioni-2.6.0/src/redturtle/prenotazioni/restapi/services/day/__init__.py
+-rw-r--r--   0 cekk       (501) staff       (20)      365 2024-04-02 07:43:54.000000 redturtle.prenotazioni-2.6.0/src/redturtle/prenotazioni/restapi/services/day/configure.zcml
+-rw-r--r--   0 cekk       (501) staff       (20)     6731 2024-04-02 07:43:54.000000 redturtle.prenotazioni-2.6.0/src/redturtle/prenotazioni/restapi/services/day/day.py
+drwxr-xr-x   0 cekk       (501) staff       (20)        0 2024-04-02 07:43:54.796096 redturtle.prenotazioni-2.6.0/src/redturtle/prenotazioni/restapi/services/types/
+-rw-r--r--   0 cekk       (501) staff       (20)        0 2024-04-02 07:43:54.000000 redturtle.prenotazioni-2.6.0/src/redturtle/prenotazioni/restapi/services/types/__init__.py
+-rw-r--r--   0 cekk       (501) staff       (20)      216 2024-04-02 07:43:54.000000 redturtle.prenotazioni-2.6.0/src/redturtle/prenotazioni/restapi/services/types/configure.zcml
+-rw-r--r--   0 cekk       (501) staff       (20)      915 2024-04-02 07:43:54.000000 redturtle.prenotazioni-2.6.0/src/redturtle/prenotazioni/restapi/services/types/get.py
+drwxr-xr-x   0 cekk       (501) staff       (20)        0 2024-04-02 07:43:54.796283 redturtle.prenotazioni-2.6.0/src/redturtle/prenotazioni/scripts/
+-rw-r--r--   0 cekk       (501) staff       (20)        0 2024-04-02 07:43:54.000000 redturtle.prenotazioni-2.6.0/src/redturtle/prenotazioni/scripts/__init__.py
+-rw-r--r--   0 cekk       (501) staff       (20)      892 2024-04-02 07:43:54.000000 redturtle.prenotazioni-2.6.0/src/redturtle/prenotazioni/scripts/notify_upcoming_bookings.py
+-rw-r--r--   0 cekk       (501) staff       (20)     1062 2024-04-02 07:43:54.000000 redturtle.prenotazioni-2.6.0/src/redturtle/prenotazioni/setuphandlers.py
+-rw-r--r--   0 cekk       (501) staff       (20)     3443 2024-04-02 07:43:54.000000 redturtle.prenotazioni-2.6.0/src/redturtle/prenotazioni/testing.py
+drwxr-xr-x   0 cekk       (501) staff       (20)        0 2024-04-02 07:43:54.800245 redturtle.prenotazioni-2.6.0/src/redturtle/prenotazioni/tests/
+-rw-r--r--   0 cekk       (501) staff       (20)      105 2024-04-02 07:43:54.000000 redturtle.prenotazioni-2.6.0/src/redturtle/prenotazioni/tests/__init__.py
+-rw-r--r--   0 cekk       (501) staff       (20)     1223 2024-04-02 07:43:54.000000 redturtle.prenotazioni-2.6.0/src/redturtle/prenotazioni/tests/helpers.py
+-rw-r--r--   0 cekk       (501) staff       (20)     3222 2024-04-02 07:43:54.000000 redturtle.prenotazioni-2.6.0/src/redturtle/prenotazioni/tests/test_add_block.py
+-rw-r--r--   0 cekk       (501) staff       (20)    24795 2024-04-02 07:43:54.000000 redturtle.prenotazioni-2.6.0/src/redturtle/prenotazioni/tests/test_add_booking.py
+-rw-r--r--   0 cekk       (501) staff       (20)     1980 2024-04-02 07:43:54.000000 redturtle.prenotazioni-2.6.0/src/redturtle/prenotazioni/tests/test_add_booking_type.py
+-rw-r--r--   0 cekk       (501) staff       (20)    17344 2024-04-02 07:43:54.000000 redturtle.prenotazioni-2.6.0/src/redturtle/prenotazioni/tests/test_available_slots.py
+-rw-r--r--   0 cekk       (501) staff       (20)     2011 2024-04-02 07:43:54.000000 redturtle.prenotazioni-2.6.0/src/redturtle/prenotazioni/tests/test_base_slot.py
+-rw-r--r--   0 cekk       (501) staff       (20)     4387 2024-04-02 07:43:54.000000 redturtle.prenotazioni-2.6.0/src/redturtle/prenotazioni/tests/test_booker_choose_available_slot.py
+-rw-r--r--   0 cekk       (501) staff       (20)     6402 2024-04-02 07:43:54.000000 redturtle.prenotazioni-2.6.0/src/redturtle/prenotazioni/tests/test_booking_info.py
+-rw-r--r--   0 cekk       (501) staff       (20)     6901 2024-04-02 07:43:54.000000 redturtle.prenotazioni-2.6.0/src/redturtle/prenotazioni/tests/test_booking_notify.py
+-rw-r--r--   0 cekk       (501) staff       (20)     8748 2024-04-02 07:43:54.000000 redturtle.prenotazioni-2.6.0/src/redturtle/prenotazioni/tests/test_booking_schema.py
+-rw-r--r--   0 cekk       (501) staff       (20)     8696 2024-04-02 07:43:54.000000 redturtle.prenotazioni-2.6.0/src/redturtle/prenotazioni/tests/test_bookings_num_limit.py
+-rw-r--r--   0 cekk       (501) staff       (20)     5952 2024-04-02 07:43:54.000000 redturtle.prenotazioni-2.6.0/src/redturtle/prenotazioni/tests/test_browser_utilities_notify_upcoming_bookings.py
+-rw-r--r--   0 cekk       (501) staff       (20)     3088 2024-04-02 07:43:54.000000 redturtle.prenotazioni-2.6.0/src/redturtle/prenotazioni/tests/test_content_validators_validate_pause_table.py
+-rw-r--r--   0 cekk       (501) staff       (20)     6317 2024-04-02 07:43:54.000000 redturtle.prenotazioni-2.6.0/src/redturtle/prenotazioni/tests/test_day.py
+-rw-r--r--   0 cekk       (501) staff       (20)    10871 2024-04-02 07:43:54.000000 redturtle.prenotazioni-2.6.0/src/redturtle/prenotazioni/tests/test_delete_booking.py
+-rw-r--r--   0 cekk       (501) staff       (20)    10361 2024-04-02 07:43:54.000000 redturtle.prenotazioni-2.6.0/src/redturtle/prenotazioni/tests/test_delete_booking_api.py
+-rw-r--r--   0 cekk       (501) staff       (20)     4000 2024-04-02 07:43:54.000000 redturtle.prenotazioni-2.6.0/src/redturtle/prenotazioni/tests/test_gates_overrides.py
+-rw-r--r--   0 cekk       (501) staff       (20)     8150 2024-04-02 07:43:54.000000 redturtle.prenotazioni-2.6.0/src/redturtle/prenotazioni/tests/test_move_booking_api.py
+-rw-r--r--   0 cekk       (501) staff       (20)     5216 2024-04-02 07:43:54.000000 redturtle.prenotazioni-2.6.0/src/redturtle/prenotazioni/tests/test_notification_supervisor_utility.py
+-rw-r--r--   0 cekk       (501) staff       (20)    14545 2024-04-02 07:43:54.000000 redturtle.prenotazioni-2.6.0/src/redturtle/prenotazioni/tests/test_pauses_overrides.py
+-rw-r--r--   0 cekk       (501) staff       (20)     5029 2024-04-02 07:43:54.000000 redturtle.prenotazioni-2.6.0/src/redturtle/prenotazioni/tests/test_prenotazione_email_sent_to_managers.py
+-rw-r--r--   0 cekk       (501) staff       (20)    15081 2024-04-02 07:43:54.000000 redturtle.prenotazioni-2.6.0/src/redturtle/prenotazioni/tests/test_prenotazione_events.py
+-rw-r--r--   0 cekk       (501) staff       (20)     4861 2024-04-02 07:43:54.000000 redturtle.prenotazioni-2.6.0/src/redturtle/prenotazioni/tests/test_prenotazione_searchable_item_serializer.py
+-rw-r--r--   0 cekk       (501) staff       (20)     7049 2024-04-02 07:43:54.000000 redturtle.prenotazioni-2.6.0/src/redturtle/prenotazioni/tests/test_prenotazioni_context_state.py
+-rw-r--r--   0 cekk       (501) staff       (20)      740 2024-04-02 07:43:54.000000 redturtle.prenotazioni-2.6.0/src/redturtle/prenotazioni/tests/test_prenotazioni_folder_holidays_constraint.py
+-rw-r--r--   0 cekk       (501) staff       (20)    19833 2024-04-02 07:43:54.000000 redturtle.prenotazioni-2.6.0/src/redturtle/prenotazioni/tests/test_prenotazioni_search.py
+-rw-r--r--   0 cekk       (501) staff       (20)     2485 2024-04-02 07:43:54.000000 redturtle.prenotazioni-2.6.0/src/redturtle/prenotazioni/tests/test_restapi_types_override.py
+-rw-r--r--   0 cekk       (501) staff       (20)     9722 2024-04-02 07:43:54.000000 redturtle.prenotazioni-2.6.0/src/redturtle/prenotazioni/tests/test_send_ical.py
+-rw-r--r--   0 cekk       (501) staff       (20)     4180 2024-04-02 07:43:54.000000 redturtle.prenotazioni-2.6.0/src/redturtle/prenotazioni/tests/test_setup.py
+-rw-r--r--   0 cekk       (501) staff       (20)     3046 2024-04-02 07:43:54.000000 redturtle.prenotazioni-2.6.0/src/redturtle/prenotazioni/tests/test_stringinterp.py
+-rw-r--r--   0 cekk       (501) staff       (20)      905 2024-04-02 07:43:54.000000 redturtle.prenotazioni-2.6.0/src/redturtle/prenotazioni/tests/test_utils.py
+-rw-r--r--   0 cekk       (501) staff       (20)     6486 2024-04-02 07:43:54.000000 redturtle.prenotazioni-2.6.0/src/redturtle/prenotazioni/tests/test_vacation_api.py
+-rw-r--r--   0 cekk       (501) staff       (20)     2349 2024-04-02 07:43:54.000000 redturtle.prenotazioni-2.6.0/src/redturtle/prenotazioni/tests/test_vocabularies.py
+-rw-r--r--   0 cekk       (501) staff       (20)    23517 2024-04-02 07:43:54.000000 redturtle.prenotazioni-2.6.0/src/redturtle/prenotazioni/tests/test_week_table_overrides.py
+-rw-r--r--   0 cekk       (501) staff       (20)    16547 2024-04-02 07:43:54.000000 redturtle.prenotazioni-2.6.0/src/redturtle/prenotazioni/upgrades.py
+-rw-r--r--   0 cekk       (501) staff       (20)    10360 2024-04-02 07:43:54.000000 redturtle.prenotazioni-2.6.0/src/redturtle/prenotazioni/upgrades.zcml
+drwxr-xr-x   0 cekk       (501) staff       (20)        0 2024-04-02 07:43:54.800908 redturtle.prenotazioni-2.6.0/src/redturtle/prenotazioni/utilities/
+-rw-r--r--   0 cekk       (501) staff       (20)       94 2024-04-02 07:43:54.000000 redturtle.prenotazioni-2.6.0/src/redturtle/prenotazioni/utilities/__init__.py
+-rw-r--r--   0 cekk       (501) staff       (20)     2900 2024-04-02 07:43:54.000000 redturtle.prenotazioni-2.6.0/src/redturtle/prenotazioni/utilities/dateutils.py
+-rw-r--r--   0 cekk       (501) staff       (20)      489 2024-04-02 07:43:54.000000 redturtle.prenotazioni-2.6.0/src/redturtle/prenotazioni/utilities/email.py
+-rw-r--r--   0 cekk       (501) staff       (20)      504 2024-04-02 07:43:54.000000 redturtle.prenotazioni-2.6.0/src/redturtle/prenotazioni/utilities/log_errors.py
+-rw-r--r--   0 cekk       (501) staff       (20)     1118 2024-04-02 07:43:54.000000 redturtle.prenotazioni-2.6.0/src/redturtle/prenotazioni/utilities/urls.py
+drwxr-xr-x   0 cekk       (501) staff       (20)        0 2024-04-02 07:43:54.801172 redturtle.prenotazioni-2.6.0/src/redturtle/prenotazioni/utils/
+-rw-r--r--   0 cekk       (501) staff       (20)       67 2024-04-02 07:43:54.000000 redturtle.prenotazioni-2.6.0/src/redturtle/prenotazioni/utils/__init__.py
+-rw-r--r--   0 cekk       (501) staff       (20)      597 2024-04-02 07:43:54.000000 redturtle.prenotazioni-2.6.0/src/redturtle/prenotazioni/utils/get_prenotazioni_folder.py
+drwxr-xr-x   0 cekk       (501) staff       (20)        0 2024-04-02 07:43:54.802624 redturtle.prenotazioni-2.6.0/src/redturtle/prenotazioni/vocabularies/
+-rw-r--r--   0 cekk       (501) staff       (20)       24 2024-04-02 07:43:54.000000 redturtle.prenotazioni-2.6.0/src/redturtle/prenotazioni/vocabularies/__init__.py
+-rw-r--r--   0 cekk       (501) staff       (20)     1444 2024-04-02 07:43:54.000000 redturtle.prenotazioni-2.6.0/src/redturtle/prenotazioni/vocabularies/configure.zcml
+-rw-r--r--   0 cekk       (501) staff       (20)      607 2024-04-02 07:43:54.000000 redturtle.prenotazioni-2.6.0/src/redturtle/prenotazioni/vocabularies/gates.py
+-rw-r--r--   0 cekk       (501) staff       (20)     1011 2024-04-02 07:43:54.000000 redturtle.prenotazioni-2.6.0/src/redturtle/prenotazioni/vocabularies/requirable_booking_fields.py
+-rw-r--r--   0 cekk       (501) staff       (20)      598 2024-04-02 07:43:54.000000 redturtle.prenotazioni-2.6.0/src/redturtle/prenotazioni/vocabularies/review_states.py
+-rw-r--r--   0 cekk       (501) staff       (20)     1814 2024-04-02 07:43:54.000000 redturtle.prenotazioni-2.6.0/src/redturtle/prenotazioni/vocabularies/tipologies.py
+-rw-r--r--   0 cekk       (501) staff       (20)      776 2024-04-02 07:43:54.000000 redturtle.prenotazioni-2.6.0/src/redturtle/prenotazioni/vocabularies/voc_booking_type_gates.py
+-rw-r--r--   0 cekk       (501) staff       (20)     1128 2024-04-02 07:43:54.000000 redturtle.prenotazioni-2.6.0/src/redturtle/prenotazioni/vocabularies/voc_durata_incontro.py
+-rw-r--r--   0 cekk       (501) staff       (20)     2549 2024-04-02 07:43:54.000000 redturtle.prenotazioni-2.6.0/src/redturtle/prenotazioni/vocabularies/voc_months.py
+-rw-r--r--   0 cekk       (501) staff       (20)     1367 2024-04-02 07:43:54.000000 redturtle.prenotazioni-2.6.0/src/redturtle/prenotazioni/vocabularies/voc_ore_inizio.py
+-rw-r--r--   0 cekk       (501) staff       (20)      440 2024-04-02 07:43:54.000000 redturtle.prenotazioni-2.6.0/src/redturtle/prenotazioni/vocabularies/voc_pause_scheduler.py
+drwxr-xr-x   0 cekk       (501) staff       (20)        0 2024-04-02 07:43:54.768998 redturtle.prenotazioni-2.6.0/src/redturtle.prenotazioni.egg-info/
+-rw-r--r--   0 cekk       (501) staff       (20)    45601 2024-04-02 07:43:54.000000 redturtle.prenotazioni-2.6.0/src/redturtle.prenotazioni.egg-info/PKG-INFO
+-rw-r--r--   0 cekk       (501) staff       (20)    17688 2024-04-02 07:43:54.000000 redturtle.prenotazioni-2.6.0/src/redturtle.prenotazioni.egg-info/SOURCES.txt
+-rw-r--r--   0 cekk       (501) staff       (20)        1 2024-04-02 07:43:54.000000 redturtle.prenotazioni-2.6.0/src/redturtle.prenotazioni.egg-info/dependency_links.txt
+-rw-r--r--   0 cekk       (501) staff       (20)      267 2024-04-02 07:43:54.000000 redturtle.prenotazioni-2.6.0/src/redturtle.prenotazioni.egg-info/entry_points.txt
+-rw-r--r--   0 cekk       (501) staff       (20)       10 2024-04-02 07:43:54.000000 redturtle.prenotazioni-2.6.0/src/redturtle.prenotazioni.egg-info/namespace_packages.txt
+-rw-r--r--   0 cekk       (501) staff       (20)        1 2024-04-02 07:43:54.000000 redturtle.prenotazioni-2.6.0/src/redturtle.prenotazioni.egg-info/not-zip-safe
+-rw-r--r--   0 cekk       (501) staff       (20)      425 2024-04-02 07:43:54.000000 redturtle.prenotazioni-2.6.0/src/redturtle.prenotazioni.egg-info/requires.txt
+-rw-r--r--   0 cekk       (501) staff       (20)       10 2024-04-02 07:43:54.000000 redturtle.prenotazioni-2.6.0/src/redturtle.prenotazioni.egg-info/top_level.txt
```

### Comparing `redturtle.prenotazioni-2.5.3/APP_IO.txt` & `redturtle.prenotazioni-2.6.0/APP_IO.txt`

 * *Files identical despite different names*

### Comparing `redturtle.prenotazioni-2.5.3/CHANGES.rst` & `redturtle.prenotazioni-2.6.0/CHANGES.rst`

 * *Files 1% similar despite different names*

```diff
@@ -1,11 +1,27 @@
 Changelog
 =========
 
 
+2.6.0 (2024-04-02)
+------------------
+
+- Return empty data from the @day endpoint if requested date is out of PrenotazioniFolder range
+  [folix-01]
+
+- Fix double gate bug.
+  [folix-01]
+
+- first_available flag for the @available-slots endpoint.
+  [folix-01]
+
+- Fix double gate when it is repeated in more than one week table overrides.
+  [folix-01]
+
+
 2.5.3 (2024-03-19)
 ------------------
 
 - Fix SMS links. Removed the dot immediately after the url
   [folix-01]
 
 
@@ -19,15 +35,15 @@
   [folix-01]
 
 2.5.1 (2024-03-06)
 ------------------
 
 - Add the years range configuration to week table overrides.
   [folix-01]
- 
+
 - Bypass the today delete limit for the 'out-of-office' types
   [folix-01]
 
 - Change the booking notification flag label.
   [folix-01]
```

### Comparing `redturtle.prenotazioni-2.5.3/DEVELOP.rst` & `redturtle.prenotazioni-2.6.0/DEVELOP.rst`

 * *Files identical despite different names*

### Comparing `redturtle.prenotazioni-2.5.3/LICENSE.GPL` & `redturtle.prenotazioni-2.6.0/LICENSE.GPL`

 * *Files identical despite different names*

### Comparing `redturtle.prenotazioni-2.5.3/LICENSE.rst` & `redturtle.prenotazioni-2.6.0/LICENSE.rst`

 * *Files identical despite different names*

### Comparing `redturtle.prenotazioni-2.5.3/PKG-INFO` & `redturtle.prenotazioni-2.6.0/PKG-INFO`

 * *Files 2% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: redturtle.prenotazioni
-Version: 2.5.3
+Version: 2.6.0
 Summary: An add-on for Plone
 Home-page: https://github.com/redturtle/redturtle.prenotazioni
 Author: RedTurtle Technology
 Author-email: sviluppoplone@redturtle.it
 License: GPL version 2
 Project-URL: PyPI, https://pypi.org/project/redturtle.prenotazioni
 Project-URL: Source, https://github.com/redturtle/redturtle.prenotazioni
@@ -475,15 +475,15 @@
 
 By default (without parameters) the endpoint returns available slots for the current month, starting from today.
 
 Parameters:
 
 - **start** a start date. If not given, the start will be today.
 - **end** an end date. If not given, the end will be the last day of current month.
-
+- **first_available** a boolean flag, if valiorized, the first available slot returned without the current month search limit but the one year.
 
 Example::
 
    curl -i http://localhost:8080/Plone/folder/@available-slots -H 'Accept: application/json'
 
 Response::
 
@@ -934,14 +934,30 @@
 .. _List of contributors: https://github.com/RedTurtle/redturtle.prenotazioni/graphs/contributors
 
 
 Changelog
 =========
 
 
+2.6.0 (2024-04-02)
+------------------
+
+- Return empty data from the @day endpoint if requested date is out of PrenotazioniFolder range
+  [folix-01]
+
+- Fix double gate bug.
+  [folix-01]
+
+- first_available flag for the @available-slots endpoint.
+  [folix-01]
+
+- Fix double gate when it is repeated in more than one week table overrides.
+  [folix-01]
+
+
 2.5.3 (2024-03-19)
 ------------------
 
 - Fix SMS links. Removed the dot immediately after the url
   [folix-01]
 
 
@@ -955,15 +971,15 @@
   [folix-01]
 
 2.5.1 (2024-03-06)
 ------------------
 
 - Add the years range configuration to week table overrides.
   [folix-01]
- 
+
 - Bypass the today delete limit for the 'out-of-office' types
   [folix-01]
 
 - Change the booking notification flag label.
   [folix-01]
```

### Comparing `redturtle.prenotazioni-2.5.3/README.rst` & `redturtle.prenotazioni-2.6.0/README.rst`

 * *Files 0% similar despite different names*

```diff
@@ -443,15 +443,15 @@
 
 By default (without parameters) the endpoint returns available slots for the current month, starting from today.
 
 Parameters:
 
 - **start** a start date. If not given, the start will be today.
 - **end** an end date. If not given, the end will be the last day of current month.
-
+- **first_available** a boolean flag, if valiorized, the first available slot returned without the current month search limit but the one year.
 
 Example::
 
    curl -i http://localhost:8080/Plone/folder/@available-slots -H 'Accept: application/json'
 
 Response::
```

### Comparing `redturtle.prenotazioni-2.5.3/docs/conf.py` & `redturtle.prenotazioni-2.6.0/docs/conf.py`

 * *Files identical despite different names*

### Comparing `redturtle.prenotazioni-2.5.3/setup.py` & `redturtle.prenotazioni-2.6.0/setup.py`

 * *Files 0% similar despite different names*

```diff
@@ -11,15 +11,15 @@
         open("CHANGES.rst").read(),
     ]
 )
 
 
 setup(
     name="redturtle.prenotazioni",
-    version="2.5.3",
+    version="2.6.0",
     description="An add-on for Plone",
     long_description=long_description,
     # Get more from https://pypi.python.org/pypi?%3Aaction=list_classifiers
     classifiers=[
         "Development Status :: 5 - Production/Stable",
         "Environment :: Web Environment",
         "Framework :: Plone",
```

### Comparing `redturtle.prenotazioni-2.5.3/src/redturtle/prenotazioni/__init__.py` & `redturtle.prenotazioni-2.6.0/src/redturtle/prenotazioni/__init__.py`

 * *Files identical despite different names*

### Comparing `redturtle.prenotazioni-2.5.3/src/redturtle/prenotazioni/actions/mail.py` & `redturtle.prenotazioni-2.6.0/src/redturtle/prenotazioni/actions/mail.py`

 * *Files identical despite different names*

### Comparing `redturtle.prenotazioni-2.5.3/src/redturtle/prenotazioni/adapters/booker.py` & `redturtle.prenotazioni-2.6.0/src/redturtle/prenotazioni/adapters/booker.py`

 * *Files identical despite different names*

### Comparing `redturtle.prenotazioni-2.5.3/src/redturtle/prenotazioni/adapters/booking_code.py` & `redturtle.prenotazioni-2.6.0/src/redturtle/prenotazioni/adapters/booking_code.py`

 * *Files identical despite different names*

### Comparing `redturtle.prenotazioni-2.5.3/src/redturtle/prenotazioni/adapters/configure.zcml` & `redturtle.prenotazioni-2.6.0/src/redturtle/prenotazioni/adapters/configure.zcml`

 * *Files identical despite different names*

### Comparing `redturtle.prenotazioni-2.5.3/src/redturtle/prenotazioni/adapters/conflict.py` & `redturtle.prenotazioni-2.6.0/src/redturtle/prenotazioni/adapters/conflict.py`

 * *Files identical despite different names*

### Comparing `redturtle.prenotazioni-2.5.3/src/redturtle/prenotazioni/adapters/ical.py` & `redturtle.prenotazioni-2.6.0/src/redturtle/prenotazioni/adapters/ical.py`

 * *Files identical despite different names*

### Comparing `redturtle.prenotazioni-2.5.3/src/redturtle/prenotazioni/adapters/slot.py` & `redturtle.prenotazioni-2.6.0/src/redturtle/prenotazioni/adapters/slot.py`

 * *Files identical despite different names*

### Comparing `redturtle.prenotazioni-2.5.3/src/redturtle/prenotazioni/adapters/stringinterp.py` & `redturtle.prenotazioni-2.6.0/src/redturtle/prenotazioni/adapters/stringinterp.py`

 * *Files identical despite different names*

### Comparing `redturtle.prenotazioni-2.5.3/src/redturtle/prenotazioni/behaviors/booking_folder/configure.zcml` & `redturtle.prenotazioni-2.6.0/src/redturtle/prenotazioni/behaviors/booking_folder/configure.zcml`

 * *Files identical despite different names*

### Comparing `redturtle.prenotazioni-2.5.3/src/redturtle/prenotazioni/behaviors/booking_folder/contacts.py` & `redturtle.prenotazioni-2.6.0/src/redturtle/prenotazioni/behaviors/booking_folder/contacts.py`

 * *Files identical despite different names*

### Comparing `redturtle.prenotazioni-2.5.3/src/redturtle/prenotazioni/behaviors/booking_folder/notifications/__init__.py` & `redturtle.prenotazioni-2.6.0/src/redturtle/prenotazioni/behaviors/booking_folder/notifications/__init__.py`

 * *Files identical despite different names*

### Comparing `redturtle.prenotazioni-2.5.3/src/redturtle/prenotazioni/behaviors/booking_folder/notifications/appio/__init__.py` & `redturtle.prenotazioni-2.6.0/src/redturtle/prenotazioni/behaviors/booking_folder/notifications/appio/__init__.py`

 * *Files identical despite different names*

### Comparing `redturtle.prenotazioni-2.5.3/src/redturtle/prenotazioni/behaviors/booking_folder/notifications/appio/adapters.py` & `redturtle.prenotazioni-2.6.0/src/redturtle/prenotazioni/behaviors/booking_folder/notifications/appio/adapters.py`

 * *Files identical despite different names*

### Comparing `redturtle.prenotazioni-2.5.3/src/redturtle/prenotazioni/behaviors/booking_folder/notifications/appio/configure.zcml` & `redturtle.prenotazioni-2.6.0/src/redturtle/prenotazioni/behaviors/booking_folder/notifications/appio/configure.zcml`

 * *Files identical despite different names*

### Comparing `redturtle.prenotazioni-2.5.3/src/redturtle/prenotazioni/behaviors/booking_folder/notifications/appio/events.py` & `redturtle.prenotazioni-2.6.0/src/redturtle/prenotazioni/behaviors/booking_folder/notifications/appio/events.py`

 * *Files identical despite different names*

### Comparing `redturtle.prenotazioni-2.5.3/src/redturtle/prenotazioni/behaviors/booking_folder/notifications/appio/notfication_appio_message.py` & `redturtle.prenotazioni-2.6.0/src/redturtle/prenotazioni/behaviors/booking_folder/notifications/appio/notfication_appio_message.py`

 * *Files identical despite different names*

### Comparing `redturtle.prenotazioni-2.5.3/src/redturtle/prenotazioni/behaviors/booking_folder/notifications/appio/voc_service_keys.py` & `redturtle.prenotazioni-2.6.0/src/redturtle/prenotazioni/behaviors/booking_folder/notifications/appio/voc_service_keys.py`

 * *Files identical despite different names*

### Comparing `redturtle.prenotazioni-2.5.3/src/redturtle/prenotazioni/behaviors/booking_folder/notifications/email/__init__.py` & `redturtle.prenotazioni-2.6.0/src/redturtle/prenotazioni/behaviors/booking_folder/notifications/email/__init__.py`

 * *Files identical despite different names*

### Comparing `redturtle.prenotazioni-2.5.3/src/redturtle/prenotazioni/behaviors/booking_folder/notifications/email/adapters.py` & `redturtle.prenotazioni-2.6.0/src/redturtle/prenotazioni/behaviors/booking_folder/notifications/email/adapters.py`

 * *Files identical despite different names*

### Comparing `redturtle.prenotazioni-2.5.3/src/redturtle/prenotazioni/behaviors/booking_folder/notifications/email/configure.zcml` & `redturtle.prenotazioni-2.6.0/src/redturtle/prenotazioni/behaviors/booking_folder/notifications/email/configure.zcml`

 * *Files identical despite different names*

### Comparing `redturtle.prenotazioni-2.5.3/src/redturtle/prenotazioni/behaviors/booking_folder/notifications/email/events.py` & `redturtle.prenotazioni-2.6.0/src/redturtle/prenotazioni/behaviors/booking_folder/notifications/email/events.py`

 * *Files identical despite different names*

### Comparing `redturtle.prenotazioni-2.5.3/src/redturtle/prenotazioni/behaviors/booking_folder/notifications/email/notification_email_message.py` & `redturtle.prenotazioni-2.6.0/src/redturtle/prenotazioni/behaviors/booking_folder/notifications/email/notification_email_message.py`

 * *Files identical despite different names*

### Comparing `redturtle.prenotazioni-2.5.3/src/redturtle/prenotazioni/behaviors/booking_folder/notifications/sms/__init__.py` & `redturtle.prenotazioni-2.6.0/src/redturtle/prenotazioni/behaviors/booking_folder/notifications/sms/__init__.py`

 * *Files identical despite different names*

### Comparing `redturtle.prenotazioni-2.5.3/src/redturtle/prenotazioni/behaviors/booking_folder/notifications/sms/adapters.py` & `redturtle.prenotazioni-2.6.0/src/redturtle/prenotazioni/behaviors/booking_folder/notifications/sms/adapters.py`

 * *Files identical despite different names*

### Comparing `redturtle.prenotazioni-2.5.3/src/redturtle/prenotazioni/behaviors/booking_folder/notifications/sms/configure.zcml` & `redturtle.prenotazioni-2.6.0/src/redturtle/prenotazioni/behaviors/booking_folder/notifications/sms/configure.zcml`

 * *Files identical despite different names*

### Comparing `redturtle.prenotazioni-2.5.3/src/redturtle/prenotazioni/behaviors/booking_folder/notifications/sms/events.py` & `redturtle.prenotazioni-2.6.0/src/redturtle/prenotazioni/behaviors/booking_folder/notifications/sms/events.py`

 * *Files identical despite different names*

### Comparing `redturtle.prenotazioni-2.5.3/src/redturtle/prenotazioni/behaviors/booking_folder/notifications/sms/message.py` & `redturtle.prenotazioni-2.6.0/src/redturtle/prenotazioni/behaviors/booking_folder/notifications/sms/message.py`

 * *Files identical despite different names*

### Comparing `redturtle.prenotazioni-2.5.3/src/redturtle/prenotazioni/browser/base.py` & `redturtle.prenotazioni-2.6.0/src/redturtle/prenotazioni/browser/base.py`

 * *Files identical despite different names*

### Comparing `redturtle.prenotazioni-2.5.3/src/redturtle/prenotazioni/browser/configure.zcml` & `redturtle.prenotazioni-2.6.0/src/redturtle/prenotazioni/browser/configure.zcml`

 * *Files identical despite different names*

### Comparing `redturtle.prenotazioni-2.5.3/src/redturtle/prenotazioni/browser/custom_radio_input.pt` & `redturtle.prenotazioni-2.6.0/src/redturtle/prenotazioni/browser/custom_radio_input.pt`

 * *Files identical despite different names*

### Comparing `redturtle.prenotazioni-2.5.3/src/redturtle/prenotazioni/browser/delete_reservation.py` & `redturtle.prenotazioni-2.6.0/src/redturtle/prenotazioni/browser/delete_reservation.py`

 * *Files identical despite different names*

### Comparing `redturtle.prenotazioni-2.5.3/src/redturtle/prenotazioni/browser/folderfactories.py` & `redturtle.prenotazioni-2.6.0/src/redturtle/prenotazioni/browser/folderfactories.py`

 * *Files identical despite different names*

### Comparing `redturtle.prenotazioni-2.5.3/src/redturtle/prenotazioni/browser/prenotazione.py` & `redturtle.prenotazioni-2.6.0/src/redturtle/prenotazioni/browser/prenotazione.py`

 * *Files identical despite different names*

### Comparing `redturtle.prenotazioni-2.5.3/src/redturtle/prenotazioni/browser/prenotazione_add.py` & `redturtle.prenotazioni-2.6.0/src/redturtle/prenotazioni/browser/prenotazione_add.py`

 * *Files identical despite different names*

### Comparing `redturtle.prenotazioni-2.5.3/src/redturtle/prenotazioni/browser/prenotazione_move.py` & `redturtle.prenotazioni-2.6.0/src/redturtle/prenotazioni/browser/prenotazione_move.py`

 * *Files identical despite different names*

### Comparing `redturtle.prenotazioni-2.5.3/src/redturtle/prenotazioni/browser/prenotazione_print.py` & `redturtle.prenotazioni-2.6.0/src/redturtle/prenotazioni/browser/prenotazione_print.py`

 * *Files identical despite different names*

### Comparing `redturtle.prenotazioni-2.5.3/src/redturtle/prenotazioni/browser/prenotazioni_context_state.py` & `redturtle.prenotazioni-2.6.0/src/redturtle/prenotazioni/browser/prenotazioni_context_state.py`

 * *Files 1% similar despite different names*

```diff
@@ -1,10 +1,11 @@
 # -*- coding: utf-8 -*-
 import itertools
 import json
+from copy import deepcopy
 from datetime import date
 from datetime import datetime
 from datetime import timedelta
 
 import six
 from DateTime import DateTime
 from plone import api
@@ -238,14 +239,24 @@
 
                 if from_date <= booking_date <= to_date:
                     unlimited_overrides.append(override)
 
         # More specific overrides first
         overrides = unlimited_overrides + overrides
 
+        # remove double gates, we are interested only about the last one
+        gates = []
+
+        for i, j in reversed(list(enumerate(overrides))):
+            for gate in deepcopy(j.get("gates", [])):
+                if gate in gates:
+                    overrides[i]["gates"].remove(gate)
+                else:
+                    gates.append(gate)
+
         return overrides
 
     def get_week_table(self, day):
         """
         return week table divided by gates because overrides can have
         different gate timetables
         """
```

### Comparing `redturtle.prenotazioni-2.5.3/src/redturtle/prenotazioni/browser/prenotazioni_portal_state.py` & `redturtle.prenotazioni-2.6.0/src/redturtle/prenotazioni/browser/prenotazioni_portal_state.py`

 * *Files identical despite different names*

### Comparing `redturtle.prenotazioni-2.5.3/src/redturtle/prenotazioni/browser/prenotazioni_search.py` & `redturtle.prenotazioni-2.6.0/src/redturtle/prenotazioni/browser/prenotazioni_search.py`

 * *Files identical despite different names*

### Comparing `redturtle.prenotazioni-2.5.3/src/redturtle/prenotazioni/browser/static/redturtle-reservation.css` & `redturtle.prenotazioni-2.6.0/src/redturtle/prenotazioni/browser/static/redturtle-reservation.css`

 * *Files identical despite different names*

### Comparing `redturtle.prenotazioni-2.5.3/src/redturtle/prenotazioni/browser/static/redturtle-reservation.js` & `redturtle.prenotazioni-2.6.0/src/redturtle/prenotazioni/browser/static/redturtle-reservation.js`

 * *Files identical despite different names*

### Comparing `redturtle.prenotazioni-2.5.3/src/redturtle/prenotazioni/browser/static/times-solid.png` & `redturtle.prenotazioni-2.6.0/src/redturtle/prenotazioni/browser/static/times-solid.png`

 * *Files identical despite different names*

### Comparing `redturtle.prenotazioni-2.5.3/src/redturtle/prenotazioni/browser/static/widget/dist/prod/main.css` & `redturtle.prenotazioni-2.6.0/src/redturtle/prenotazioni/browser/static/widget/dist/prod/main.css`

 * *Files identical despite different names*

### Comparing `redturtle.prenotazioni-2.5.3/src/redturtle/prenotazioni/browser/static/widget/dist/prod/main.css.map` & `redturtle.prenotazioni-2.6.0/src/redturtle/prenotazioni/browser/static/widget/dist/prod/main.css.map`

 * *Files identical despite different names*

### Comparing `redturtle.prenotazioni-2.5.3/src/redturtle/prenotazioni/browser/static/widget/dist/prod/main.js` & `redturtle.prenotazioni-2.6.0/src/redturtle/prenotazioni/browser/static/widget/dist/prod/main.js`

 * *Files identical despite different names*

### Comparing `redturtle.prenotazioni-2.5.3/src/redturtle/prenotazioni/browser/static/widget/js/WidgetContainer/index.js` & `redturtle.prenotazioni-2.6.0/src/redturtle/prenotazioni/browser/static/widget/js/WidgetContainer/index.js`

 * *Files identical despite different names*

### Comparing `redturtle.prenotazioni-2.5.3/src/redturtle/prenotazioni/browser/static/widget/js/WidgetDataContainer/index.js` & `redturtle.prenotazioni-2.6.0/src/redturtle/prenotazioni/browser/static/widget/js/WidgetDataContainer/index.js`

 * *Files identical despite different names*

### Comparing `redturtle.prenotazioni-2.5.3/src/redturtle/prenotazioni/browser/static/widget/js/WidgetDataContainer/index.less` & `redturtle.prenotazioni-2.6.0/src/redturtle/prenotazioni/browser/static/widget/js/WidgetDataContainer/index.less`

 * *Files identical despite different names*

### Comparing `redturtle.prenotazioni-2.5.3/src/redturtle/prenotazioni/browser/static/widget/js/fields/DaysTableField.js` & `redturtle.prenotazioni-2.6.0/src/redturtle/prenotazioni/browser/static/widget/js/fields/DaysTableField.js`

 * *Files identical despite different names*

### Comparing `redturtle.prenotazioni-2.5.3/src/redturtle/prenotazioni/browser/static/widget/js/fields/GatesField.js` & `redturtle.prenotazioni-2.6.0/src/redturtle/prenotazioni/browser/static/widget/js/fields/GatesField.js`

 * *Files identical despite different names*

### Comparing `redturtle.prenotazioni-2.5.3/src/redturtle/prenotazioni/browser/static/widget/js/fields/IntervalSelectorField.js` & `redturtle.prenotazioni-2.6.0/src/redturtle/prenotazioni/browser/static/widget/js/fields/IntervalSelectorField.js`

 * *Files identical despite different names*

### Comparing `redturtle.prenotazioni-2.5.3/src/redturtle/prenotazioni/browser/static/widget/js/fields/PauseTableField.js` & `redturtle.prenotazioni-2.6.0/src/redturtle/prenotazioni/browser/static/widget/js/fields/PauseTableField.js`

 * *Files identical despite different names*

### Comparing `redturtle.prenotazioni-2.5.3/src/redturtle/prenotazioni/browser/static/widget/js/fields/SelectField.js` & `redturtle.prenotazioni-2.6.0/src/redturtle/prenotazioni/browser/static/widget/js/fields/SelectField.js`

 * *Files identical despite different names*

### Comparing `redturtle.prenotazioni-2.5.3/src/redturtle/prenotazioni/browser/static/widget/js/fields/TextLineField.js` & `redturtle.prenotazioni-2.6.0/src/redturtle/prenotazioni/browser/static/widget/js/fields/TextLineField.js`

 * *Files identical despite different names*

### Comparing `redturtle.prenotazioni-2.5.3/src/redturtle/prenotazioni/browser/static/widget/js/index.js` & `redturtle.prenotazioni-2.6.0/src/redturtle/prenotazioni/browser/static/widget/js/index.js`

 * *Files identical despite different names*

### Comparing `redturtle.prenotazioni-2.5.3/src/redturtle/prenotazioni/browser/static/widget/js/utils/i18n.js` & `redturtle.prenotazioni-2.6.0/src/redturtle/prenotazioni/browser/static/widget/js/utils/i18n.js`

 * *Files identical despite different names*

### Comparing `redturtle.prenotazioni-2.5.3/src/redturtle/prenotazioni/browser/stats/booking_stats.pt` & `redturtle.prenotazioni-2.6.0/src/redturtle/prenotazioni/browser/stats/booking_stats.pt`

 * *Files identical despite different names*

### Comparing `redturtle.prenotazioni-2.5.3/src/redturtle/prenotazioni/browser/stats/booking_stats.py` & `redturtle.prenotazioni-2.6.0/src/redturtle/prenotazioni/browser/stats/booking_stats.py`

 * *Files identical despite different names*

### Comparing `redturtle.prenotazioni-2.5.3/src/redturtle/prenotazioni/browser/stats/configure.zcml` & `redturtle.prenotazioni-2.6.0/src/redturtle/prenotazioni/browser/stats/configure.zcml`

 * *Files identical despite different names*

### Comparing `redturtle.prenotazioni-2.5.3/src/redturtle/prenotazioni/browser/templates/booking_type_radio_widget.pt` & `redturtle.prenotazioni-2.6.0/src/redturtle/prenotazioni/browser/templates/booking_type_radio_widget.pt`

 * *Files identical despite different names*

### Comparing `redturtle.prenotazioni-2.5.3/src/redturtle/prenotazioni/browser/templates/custom_dgf_input.pt` & `redturtle.prenotazioni-2.6.0/src/redturtle/prenotazioni/browser/templates/custom_dgf_input.pt`

 * *Files identical despite different names*

### Comparing `redturtle.prenotazioni-2.5.3/src/redturtle/prenotazioni/browser/templates/delete_reservation.pt` & `redturtle.prenotazioni-2.6.0/src/redturtle/prenotazioni/browser/templates/delete_reservation.pt`

 * *Files identical despite different names*

### Comparing `redturtle.prenotazioni-2.5.3/src/redturtle/prenotazioni/browser/templates/manager_notification_mail.pt` & `redturtle.prenotazioni-2.6.0/src/redturtle/prenotazioni/browser/templates/manager_notification_mail.pt`

 * *Files identical despite different names*

### Comparing `redturtle.prenotazioni-2.5.3/src/redturtle/prenotazioni/browser/templates/prenotazione.pt` & `redturtle.prenotazioni-2.6.0/src/redturtle/prenotazioni/browser/templates/prenotazione.pt`

 * *Files identical despite different names*

### Comparing `redturtle.prenotazioni-2.5.3/src/redturtle/prenotazioni/browser/templates/prenotazione_add.pt` & `redturtle.prenotazioni-2.6.0/src/redturtle/prenotazioni/browser/templates/prenotazione_add.pt`

 * *Files identical despite different names*

### Comparing `redturtle.prenotazioni-2.5.3/src/redturtle/prenotazioni/browser/templates/prenotazione_macros.pt` & `redturtle.prenotazioni-2.6.0/src/redturtle/prenotazioni/browser/templates/prenotazione_macros.pt`

 * *Files identical despite different names*

### Comparing `redturtle.prenotazioni-2.5.3/src/redturtle/prenotazioni/browser/templates/prenotazione_move.pt` & `redturtle.prenotazioni-2.6.0/src/redturtle/prenotazioni/browser/templates/prenotazione_move.pt`

 * *Files identical despite different names*

### Comparing `redturtle.prenotazioni-2.5.3/src/redturtle/prenotazioni/browser/templates/prenotazione_print.pt` & `redturtle.prenotazioni-2.6.0/src/redturtle/prenotazioni/browser/templates/prenotazione_print.pt`

 * *Files identical despite different names*

### Comparing `redturtle.prenotazioni-2.5.3/src/redturtle/prenotazioni/browser/templates/prenotazioni_search.pt` & `redturtle.prenotazioni-2.6.0/src/redturtle/prenotazioni/browser/templates/prenotazioni_search.pt`

 * *Files identical despite different names*

### Comparing `redturtle.prenotazioni-2.5.3/src/redturtle/prenotazioni/browser/templates/week.pt` & `redturtle.prenotazioni-2.6.0/src/redturtle/prenotazioni/browser/templates/week.pt`

 * *Files identical despite different names*

### Comparing `redturtle.prenotazioni-2.5.3/src/redturtle/prenotazioni/browser/utilities/notify_upcoming_bookings.py` & `redturtle.prenotazioni-2.6.0/src/redturtle/prenotazioni/browser/utilities/notify_upcoming_bookings.py`

 * *Files identical despite different names*

### Comparing `redturtle.prenotazioni-2.5.3/src/redturtle/prenotazioni/browser/vacations.py` & `redturtle.prenotazioni-2.6.0/src/redturtle/prenotazioni/browser/vacations.py`

 * *Files identical despite different names*

### Comparing `redturtle.prenotazioni-2.5.3/src/redturtle/prenotazioni/browser/viewlets.py` & `redturtle.prenotazioni-2.6.0/src/redturtle/prenotazioni/browser/viewlets.py`

 * *Files identical despite different names*

### Comparing `redturtle.prenotazioni-2.5.3/src/redturtle/prenotazioni/browser/week.py` & `redturtle.prenotazioni-2.6.0/src/redturtle/prenotazioni/browser/week.py`

 * *Files identical despite different names*

### Comparing `redturtle.prenotazioni-2.5.3/src/redturtle/prenotazioni/browser/widget.py` & `redturtle.prenotazioni-2.6.0/src/redturtle/prenotazioni/browser/widget.py`

 * *Files identical despite different names*

### Comparing `redturtle.prenotazioni-2.5.3/src/redturtle/prenotazioni/browser/z3c_custom_widget.py` & `redturtle.prenotazioni-2.6.0/src/redturtle/prenotazioni/browser/z3c_custom_widget.py`

 * *Files identical despite different names*

### Comparing `redturtle.prenotazioni-2.5.3/src/redturtle/prenotazioni/configure.zcml` & `redturtle.prenotazioni-2.6.0/src/redturtle/prenotazioni/configure.zcml`

 * *Files identical despite different names*

### Comparing `redturtle.prenotazioni-2.5.3/src/redturtle/prenotazioni/content/pause.py` & `redturtle.prenotazioni-2.6.0/src/redturtle/prenotazioni/content/pause.py`

 * *Files identical despite different names*

### Comparing `redturtle.prenotazioni-2.5.3/src/redturtle/prenotazioni/content/prenotazione.py` & `redturtle.prenotazioni-2.6.0/src/redturtle/prenotazioni/content/prenotazione.py`

 * *Files identical despite different names*

### Comparing `redturtle.prenotazioni-2.5.3/src/redturtle/prenotazioni/content/prenotazione_type.py` & `redturtle.prenotazioni-2.6.0/src/redturtle/prenotazioni/content/prenotazione_type.py`

 * *Files identical despite different names*

### Comparing `redturtle.prenotazioni-2.5.3/src/redturtle/prenotazioni/content/prenotazioni_folder.py` & `redturtle.prenotazioni-2.6.0/src/redturtle/prenotazioni/content/prenotazioni_folder.py`

 * *Files identical despite different names*

### Comparing `redturtle.prenotazioni-2.5.3/src/redturtle/prenotazioni/content/validators.py` & `redturtle.prenotazioni-2.6.0/src/redturtle/prenotazioni/content/validators.py`

 * *Files identical despite different names*

### Comparing `redturtle.prenotazioni-2.5.3/src/redturtle/prenotazioni/demo/configure.zcml` & `redturtle.prenotazioni-2.6.0/src/redturtle/prenotazioni/demo/configure.zcml`

 * *Files identical despite different names*

### Comparing `redturtle.prenotazioni-2.5.3/src/redturtle/prenotazioni/demo/setuphandlers.py` & `redturtle.prenotazioni-2.6.0/src/redturtle/prenotazioni/demo/setuphandlers.py`

 * *Files identical despite different names*

### Comparing `redturtle.prenotazioni-2.5.3/src/redturtle/prenotazioni/demo/smsdemo.py` & `redturtle.prenotazioni-2.6.0/src/redturtle/prenotazioni/demo/smsdemo.py`

 * *Files identical despite different names*

### Comparing `redturtle.prenotazioni-2.5.3/src/redturtle/prenotazioni/events/configure.zcml` & `redturtle.prenotazioni-2.6.0/src/redturtle/prenotazioni/events/configure.zcml`

 * *Files identical despite different names*

### Comparing `redturtle.prenotazioni-2.5.3/src/redturtle/prenotazioni/events/events_logger.py` & `redturtle.prenotazioni-2.6.0/src/redturtle/prenotazioni/events/events_logger.py`

 * *Files identical despite different names*

### Comparing `redturtle.prenotazioni-2.5.3/src/redturtle/prenotazioni/events/prenotazione.py` & `redturtle.prenotazioni-2.6.0/src/redturtle/prenotazioni/events/prenotazione.py`

 * *Files identical despite different names*

### Comparing `redturtle.prenotazioni-2.5.3/src/redturtle/prenotazioni/events/prenotazioni_folder.py` & `redturtle.prenotazioni-2.6.0/src/redturtle/prenotazioni/events/prenotazioni_folder.py`

 * *Files identical despite different names*

### Comparing `redturtle.prenotazioni-2.5.3/src/redturtle/prenotazioni/exceptions/booker.py` & `redturtle.prenotazioni-2.6.0/src/redturtle/prenotazioni/exceptions/booker.py`

 * *Files identical despite different names*

### Comparing `redturtle.prenotazioni-2.5.3/src/redturtle/prenotazioni/indexers/prenotazione.py` & `redturtle.prenotazioni-2.6.0/src/redturtle/prenotazioni/indexers/prenotazione.py`

 * *Files identical despite different names*

### Comparing `redturtle.prenotazioni-2.5.3/src/redturtle/prenotazioni/interfaces.py` & `redturtle.prenotazioni-2.6.0/src/redturtle/prenotazioni/interfaces.py`

 * *Files identical despite different names*

### Comparing `redturtle.prenotazioni-2.5.3/src/redturtle/prenotazioni/io_tools/README.md` & `redturtle.prenotazioni-2.6.0/src/redturtle/prenotazioni/io_tools/README.md`

 * *Files identical despite different names*

### Comparing `redturtle.prenotazioni-2.5.3/src/redturtle/prenotazioni/io_tools/api.py` & `redturtle.prenotazioni-2.6.0/src/redturtle/prenotazioni/io_tools/api.py`

 * *Files identical despite different names*

### Comparing `redturtle.prenotazioni-2.5.3/src/redturtle/prenotazioni/io_tools/cli.py` & `redturtle.prenotazioni-2.6.0/src/redturtle/prenotazioni/io_tools/cli.py`

 * *Files identical despite different names*

### Comparing `redturtle.prenotazioni-2.5.3/src/redturtle/prenotazioni/io_tools/io.db` & `redturtle.prenotazioni-2.6.0/src/redturtle/prenotazioni/io_tools/io.db`

 * *Files identical despite different names*

### Comparing `redturtle.prenotazioni-2.5.3/src/redturtle/prenotazioni/io_tools/monkey.py` & `redturtle.prenotazioni-2.6.0/src/redturtle/prenotazioni/io_tools/monkey.py`

 * *Files identical despite different names*

### Comparing `redturtle.prenotazioni-2.5.3/src/redturtle/prenotazioni/io_tools/rdbms.py` & `redturtle.prenotazioni-2.6.0/src/redturtle/prenotazioni/io_tools/rdbms.py`

 * *Files identical despite different names*

### Comparing `redturtle.prenotazioni-2.5.3/src/redturtle/prenotazioni/io_tools/spec.yaml` & `redturtle.prenotazioni-2.6.0/src/redturtle/prenotazioni/io_tools/spec.yaml`

 * *Files identical despite different names*

### Comparing `redturtle.prenotazioni-2.5.3/src/redturtle/prenotazioni/io_tools/storage.py` & `redturtle.prenotazioni-2.6.0/src/redturtle/prenotazioni/io_tools/storage.py`

 * *Files identical despite different names*

### Comparing `redturtle.prenotazioni-2.5.3/src/redturtle/prenotazioni/locales/en/LC_MESSAGES/redturtle.prenotazioni.po` & `redturtle.prenotazioni-2.6.0/src/redturtle/prenotazioni/locales/en/LC_MESSAGES/redturtle.prenotazioni.po`

 * *Files identical despite different names*

### Comparing `redturtle.prenotazioni-2.5.3/src/redturtle/prenotazioni/locales/it/LC_MESSAGES/plone.po` & `redturtle.prenotazioni-2.6.0/src/redturtle/prenotazioni/locales/it/LC_MESSAGES/plone.po`

 * *Files identical despite different names*

### Comparing `redturtle.prenotazioni-2.5.3/src/redturtle/prenotazioni/locales/it/LC_MESSAGES/redturtle.prenotazioni.po` & `redturtle.prenotazioni-2.6.0/src/redturtle/prenotazioni/locales/it/LC_MESSAGES/redturtle.prenotazioni.po`

 * *Files identical despite different names*

### Comparing `redturtle.prenotazioni-2.5.3/src/redturtle/prenotazioni/locales/manual.pot` & `redturtle.prenotazioni-2.6.0/src/redturtle/prenotazioni/locales/manual.pot`

 * *Files identical despite different names*

### Comparing `redturtle.prenotazioni-2.5.3/src/redturtle/prenotazioni/locales/redturtle.prenotazioni.pot` & `redturtle.prenotazioni-2.6.0/src/redturtle/prenotazioni/locales/redturtle.prenotazioni.pot`

 * *Files identical despite different names*

### Comparing `redturtle.prenotazioni-2.5.3/src/redturtle/prenotazioni/locales/update.py` & `redturtle.prenotazioni-2.6.0/src/redturtle/prenotazioni/locales/update.py`

 * *Files identical despite different names*

### Comparing `redturtle.prenotazioni-2.5.3/src/redturtle/prenotazioni/locales/update.sh` & `redturtle.prenotazioni-2.6.0/src/redturtle/prenotazioni/locales/update.sh`

 * *Files identical despite different names*

### Comparing `redturtle.prenotazioni-2.5.3/src/redturtle/prenotazioni/permissions.zcml` & `redturtle.prenotazioni-2.6.0/src/redturtle/prenotazioni/permissions.zcml`

 * *Files identical despite different names*

### Comparing `redturtle.prenotazioni-2.5.3/src/redturtle/prenotazioni/profiles/default/actions.xml` & `redturtle.prenotazioni-2.6.0/src/redturtle/prenotazioni/profiles/default/actions.xml`

 * *Files identical despite different names*

### Comparing `redturtle.prenotazioni-2.5.3/src/redturtle/prenotazioni/profiles/default/registry/caching.xml` & `redturtle.prenotazioni-2.6.0/src/redturtle/prenotazioni/profiles/default/registry/caching.xml`

 * *Files identical despite different names*

### Comparing `redturtle.prenotazioni-2.5.3/src/redturtle/prenotazioni/profiles/default/registry/resources.xml` & `redturtle.prenotazioni-2.6.0/src/redturtle/prenotazioni/profiles/default/registry/resources.xml`

 * *Files identical despite different names*

### Comparing `redturtle.prenotazioni-2.5.3/src/redturtle/prenotazioni/profiles/default/registry/settings.xml` & `redturtle.prenotazioni-2.6.0/src/redturtle/prenotazioni/profiles/default/registry/settings.xml`

 * *Files identical despite different names*

### Comparing `redturtle.prenotazioni-2.5.3/src/redturtle/prenotazioni/profiles/default/rolemap.xml` & `redturtle.prenotazioni-2.6.0/src/redturtle/prenotazioni/profiles/default/rolemap.xml`

 * *Files identical despite different names*

### Comparing `redturtle.prenotazioni-2.5.3/src/redturtle/prenotazioni/profiles/default/types/Prenotazione.xml` & `redturtle.prenotazioni-2.6.0/src/redturtle/prenotazioni/profiles/default/types/Prenotazione.xml`

 * *Files identical despite different names*

### Comparing `redturtle.prenotazioni-2.5.3/src/redturtle/prenotazioni/profiles/default/types/PrenotazioneType.xml` & `redturtle.prenotazioni-2.6.0/src/redturtle/prenotazioni/profiles/default/types/PrenotazioneType.xml`

 * *Files identical despite different names*

### Comparing `redturtle.prenotazioni-2.5.3/src/redturtle/prenotazioni/profiles/default/types/PrenotazioniDay.xml` & `redturtle.prenotazioni-2.6.0/src/redturtle/prenotazioni/profiles/default/types/PrenotazioniDay.xml`

 * *Files identical despite different names*

### Comparing `redturtle.prenotazioni-2.5.3/src/redturtle/prenotazioni/profiles/default/types/PrenotazioniFolder.xml` & `redturtle.prenotazioni-2.6.0/src/redturtle/prenotazioni/profiles/default/types/PrenotazioniFolder.xml`

 * *Files identical despite different names*

### Comparing `redturtle.prenotazioni-2.5.3/src/redturtle/prenotazioni/profiles/default/types/PrenotazioniWeek.xml` & `redturtle.prenotazioni-2.6.0/src/redturtle/prenotazioni/profiles/default/types/PrenotazioniWeek.xml`

 * *Files identical despite different names*

### Comparing `redturtle.prenotazioni-2.5.3/src/redturtle/prenotazioni/profiles/default/types/PrenotazioniYear.xml` & `redturtle.prenotazioni-2.6.0/src/redturtle/prenotazioni/profiles/default/types/PrenotazioniYear.xml`

 * *Files identical despite different names*

### Comparing `redturtle.prenotazioni-2.5.3/src/redturtle/prenotazioni/profiles/default/types.xml` & `redturtle.prenotazioni-2.6.0/src/redturtle/prenotazioni/profiles/default/types.xml`

 * *Files identical despite different names*

### Comparing `redturtle.prenotazioni-2.5.3/src/redturtle/prenotazioni/profiles/default/workflows/prenotazioni_workflow/definition.xml` & `redturtle.prenotazioni-2.6.0/src/redturtle/prenotazioni/profiles/default/workflows/prenotazioni_workflow/definition.xml`

 * *Files identical despite different names*

### Comparing `redturtle.prenotazioni-2.5.3/src/redturtle/prenotazioni/profiles/default/workflows/prenotazionifolder_workflow/definition.xml` & `redturtle.prenotazioni-2.6.0/src/redturtle/prenotazioni/profiles/default/workflows/prenotazionifolder_workflow/definition.xml`

 * *Files identical despite different names*

### Comparing `redturtle.prenotazioni-2.5.3/src/redturtle/prenotazioni/profiles/default/workflows.xml` & `redturtle.prenotazioni-2.6.0/src/redturtle/prenotazioni/profiles/default/workflows.xml`

 * *Files identical despite different names*

### Comparing `redturtle.prenotazioni-2.5.3/src/redturtle/prenotazioni/profiles/to_1402/contentrules.xml` & `redturtle.prenotazioni-2.6.0/src/redturtle/prenotazioni/profiles/to_1402/contentrules.xml`

 * *Files identical despite different names*

### Comparing `redturtle.prenotazioni-2.5.3/src/redturtle/prenotazioni/profiles/to_2005/rolemap.xml` & `redturtle.prenotazioni-2.6.0/src/redturtle/prenotazioni/profiles/to_2005/rolemap.xml`

 * *Files identical despite different names*

### Comparing `redturtle.prenotazioni-2.5.3/src/redturtle/prenotazioni/profiles/to_2006/workflows/prenotazioni_workflow/definition.xml` & `redturtle.prenotazioni-2.6.0/src/redturtle/prenotazioni/profiles/to_2006/workflows/prenotazioni_workflow/definition.xml`

 * *Files identical despite different names*

### Comparing `redturtle.prenotazioni-2.5.3/src/redturtle/prenotazioni/restapi/serializers/adapters/prenotazione.py` & `redturtle.prenotazioni-2.6.0/src/redturtle/prenotazioni/restapi/serializers/adapters/prenotazione.py`

 * *Files identical despite different names*

### Comparing `redturtle.prenotazioni-2.5.3/src/redturtle/prenotazioni/restapi/serializers/adapters/prenotazione_type.py` & `redturtle.prenotazioni-2.6.0/src/redturtle/prenotazioni/restapi/serializers/adapters/prenotazione_type.py`

 * *Files identical despite different names*

### Comparing `redturtle.prenotazioni-2.5.3/src/redturtle/prenotazioni/restapi/serializers/adapters/prenotazioni_folder.py` & `redturtle.prenotazioni-2.6.0/src/redturtle/prenotazioni/restapi/serializers/adapters/prenotazioni_folder.py`

 * *Files identical despite different names*

### Comparing `redturtle.prenotazioni-2.5.3/src/redturtle/prenotazioni/restapi/serializers/adapters/slot.py` & `redturtle.prenotazioni-2.6.0/src/redturtle/prenotazioni/restapi/serializers/adapters/slot.py`

 * *Files identical despite different names*

### Comparing `redturtle.prenotazioni-2.5.3/src/redturtle/prenotazioni/restapi/services/available_slots/get.py` & `redturtle.prenotazioni-2.6.0/src/redturtle/prenotazioni/restapi/services/available_slots/get.py`

 * *Files 16% similar despite different names*

```diff
@@ -15,35 +15,48 @@
     def reply(self):
         """
         Finds all the available slots in a month.
 
         If you pass a start and end date, the search will be made between these dates.
 
         If not, the search will start from current date until the end of current month.
+
+        If you pass the `first_available` flag the site will search in all the available time range of the Bookging Folder or in the next year
+        and obtain the first one if exits, note that this option is only allowed for Booking Managers
         """
+
         # XXX: nocache also for anonymous
         self.request.response.setHeader("Cache-Control", "no-cache")
 
         prenotazioni_context_state = api.content.get_view(
             "prenotazioni_context_state",
             self.context,
             self.request,
         )
 
         start = self.request.form.get("start", "")
         end = self.request.form.get("end", "")
         past_slots = self.request.form.get("past_slots", False)
+        first_available = self.request.form.get("first_available")
 
         if start:
             start = datetime.date.fromisoformat(start)
         else:
             start = datetime.date.today()
 
         if end:
             end = datetime.date.fromisoformat(end)
+        elif first_available and api.user.has_permission(
+            "redturtle.prenotazioni: Manage Prenotazioni", obj=self.context
+        ):
+            end = (
+                self.context.aData
+                and self.context.aData
+                or datetime.date(start.year + 1, start.month, start.day)
+            )
         else:
             end = start.replace(day=calendar.monthrange(start.year, start.month)[1])
 
         if start > end:
             msg = self.context.translate(
                 _(
                     "available_slots_wrong_dates",
@@ -73,13 +86,18 @@
                 info = prenotazioni_context_state.get_anonymous_booking_url(
                     booking_date, slot, slot_min_size=slot_min_size
                 )
                 if not info.get("url", ""):
                     continue
                 if not past_slots and not info.get("future"):
                     continue
+
                 response["items"].append(json_compatible(info.get("booking_date", "")))
+
+                if first_available:
+                    return response
+
         return response
 
 
 # from mrs.doubtfire.meta import metricmethod
 # AvailableSlots.reply = metricmethod(AvailableSlots.reply)
```

### Comparing `redturtle.prenotazioni-2.5.3/src/redturtle/prenotazioni/restapi/services/booking/add.py` & `redturtle.prenotazioni-2.6.0/src/redturtle/prenotazioni/restapi/services/booking/add.py`

 * *Files identical despite different names*

### Comparing `redturtle.prenotazioni-2.5.3/src/redturtle/prenotazioni/restapi/services/booking/configure.zcml` & `redturtle.prenotazioni-2.6.0/src/redturtle/prenotazioni/restapi/services/booking/configure.zcml`

 * *Files identical despite different names*

### Comparing `redturtle.prenotazioni-2.5.3/src/redturtle/prenotazioni/restapi/services/booking/delete.py` & `redturtle.prenotazioni-2.6.0/src/redturtle/prenotazioni/restapi/services/booking/delete.py`

 * *Files identical despite different names*

### Comparing `redturtle.prenotazioni-2.5.3/src/redturtle/prenotazioni/restapi/services/booking/get.py` & `redturtle.prenotazioni-2.6.0/src/redturtle/prenotazioni/restapi/services/booking/get.py`

 * *Files identical despite different names*

### Comparing `redturtle.prenotazioni-2.5.3/src/redturtle/prenotazioni/restapi/services/booking/move.py` & `redturtle.prenotazioni-2.6.0/src/redturtle/prenotazioni/restapi/services/booking/move.py`

 * *Files identical despite different names*

### Comparing `redturtle.prenotazioni-2.5.3/src/redturtle/prenotazioni/restapi/services/booking/notify_about_confirm.py` & `redturtle.prenotazioni-2.6.0/src/redturtle/prenotazioni/restapi/services/booking/notify_about_confirm.py`

 * *Files identical despite different names*

### Comparing `redturtle.prenotazioni-2.5.3/src/redturtle/prenotazioni/restapi/services/booking/vacation.py` & `redturtle.prenotazioni-2.6.0/src/redturtle/prenotazioni/restapi/services/booking/vacation.py`

 * *Files identical despite different names*

### Comparing `redturtle.prenotazioni-2.5.3/src/redturtle/prenotazioni/restapi/services/booking_schema/get.py` & `redturtle.prenotazioni-2.6.0/src/redturtle/prenotazioni/restapi/services/booking_schema/get.py`

 * *Files identical despite different names*

### Comparing `redturtle.prenotazioni-2.5.3/src/redturtle/prenotazioni/restapi/services/bookings/configure.zcml` & `redturtle.prenotazioni-2.6.0/src/redturtle/prenotazioni/restapi/services/bookings/configure.zcml`

 * *Files identical despite different names*

### Comparing `redturtle.prenotazioni-2.5.3/src/redturtle/prenotazioni/restapi/services/bookings/search.py` & `redturtle.prenotazioni-2.6.0/src/redturtle/prenotazioni/restapi/services/bookings/search.py`

 * *Files identical despite different names*

### Comparing `redturtle.prenotazioni-2.5.3/src/redturtle/prenotazioni/restapi/services/day/day.py` & `redturtle.prenotazioni-2.6.0/src/redturtle/prenotazioni/restapi/services/day/day.py`

 * *Files 4% similar despite different names*

```diff
@@ -101,23 +101,44 @@
                             "morning": {
                                 "start": "2023-05-22T05:00:00+00:00",
                                 "stop": "2023-05-22T11:00:00+00:00"
                             }
                         }
                     }`
         """
+
         if self.day is None:
             self.day = date.today()
-        return {
+
+        response = {
             "@id": f"{self.context.absolute_url()}/@day/{self.day.isoformat()}",
-            "bookings": self.get_bookings(),
-            "pauses": self.get_pauses(),
-            "gates": self.get_gates(),
         }
 
+        # check if date is in the Booking Folder availability dates range
+        if self.context.daData < self.day and (
+            not self.context.aData or self.context.aData >= self.day
+        ):
+            response.update(
+                {
+                    "bookings": self.get_bookings(),
+                    "pauses": self.get_pauses(),
+                    "gates": self.get_gates(),
+                }
+            )
+        else:
+            response.update(
+                {
+                    "bookings": [],
+                    "pauses": [],
+                    "gates": [],
+                }
+            )
+
+        return response
+
     def get_bookings(self):
         bookings = self.prenotazioni_context_state.get_bookings_in_day_folder(self.day)
         bookings_result = {}
         for gate in {i.gate for i in bookings}:
             bookings_result[gate] = [
                 getMultiAdapter((booking, self.request), ISerializeToJson)()
                 for booking in bookings
```

### Comparing `redturtle.prenotazioni-2.5.3/src/redturtle/prenotazioni/restapi/services/types/get.py` & `redturtle.prenotazioni-2.6.0/src/redturtle/prenotazioni/restapi/services/types/get.py`

 * *Files identical despite different names*

### Comparing `redturtle.prenotazioni-2.5.3/src/redturtle/prenotazioni/scripts/notify_upcoming_bookings.py` & `redturtle.prenotazioni-2.6.0/src/redturtle/prenotazioni/scripts/notify_upcoming_bookings.py`

 * *Files identical despite different names*

### Comparing `redturtle.prenotazioni-2.5.3/src/redturtle/prenotazioni/setuphandlers.py` & `redturtle.prenotazioni-2.6.0/src/redturtle/prenotazioni/setuphandlers.py`

 * *Files identical despite different names*

### Comparing `redturtle.prenotazioni-2.5.3/src/redturtle/prenotazioni/testing.py` & `redturtle.prenotazioni-2.6.0/src/redturtle/prenotazioni/testing.py`

 * *Files identical despite different names*

### Comparing `redturtle.prenotazioni-2.5.3/src/redturtle/prenotazioni/tests/helpers.py` & `redturtle.prenotazioni-2.6.0/src/redturtle/prenotazioni/tests/helpers.py`

 * *Files identical despite different names*

### Comparing `redturtle.prenotazioni-2.5.3/src/redturtle/prenotazioni/tests/test_add_block.py` & `redturtle.prenotazioni-2.6.0/src/redturtle/prenotazioni/tests/test_add_block.py`

 * *Files identical despite different names*

### Comparing `redturtle.prenotazioni-2.5.3/src/redturtle/prenotazioni/tests/test_add_booking.py` & `redturtle.prenotazioni-2.6.0/src/redturtle/prenotazioni/tests/test_add_booking.py`

 * *Files identical despite different names*

### Comparing `redturtle.prenotazioni-2.5.3/src/redturtle/prenotazioni/tests/test_add_booking_type.py` & `redturtle.prenotazioni-2.6.0/src/redturtle/prenotazioni/tests/test_add_booking_type.py`

 * *Files identical despite different names*

### Comparing `redturtle.prenotazioni-2.5.3/src/redturtle/prenotazioni/tests/test_available_slots.py` & `redturtle.prenotazioni-2.6.0/src/redturtle/prenotazioni/tests/test_available_slots.py`

 * *Files 12% similar despite different names*

```diff
@@ -9,14 +9,15 @@
 import transaction
 from dateutil import relativedelta
 from freezegun import freeze_time
 from plone import api
 from plone.app.testing import SITE_OWNER_NAME
 from plone.app.testing import SITE_OWNER_PASSWORD
 from plone.app.testing import TEST_USER_ID
+from plone.app.testing import TEST_USER_PASSWORD
 from plone.app.testing import setRoles
 from plone.restapi.serializer.converters import json_compatible
 from plone.restapi.testing import RelativeSession
 
 from redturtle.prenotazioni.adapters.booker import IBooker
 from redturtle.prenotazioni.testing import REDTURTLE_PRENOTAZIONI_API_FUNCTIONAL_TESTING
 
@@ -35,14 +36,15 @@
         return json_compatible(self.dt_local_to_utc(value))
 
     def setUp(self):
         self.app = self.layer["app"]
         self.portal = self.layer["portal"]
         self.request = self.layer["request"]
         self.portal_url = self.portal.absolute_url()
+
         setRoles(self.portal, TEST_USER_ID, ["Manager"])
 
         self.api_session = RelativeSession(self.portal_url)
         self.api_session.headers.update({"Accept": "application/json"})
         self.api_session.auth = (SITE_OWNER_NAME, SITE_OWNER_PASSWORD)
 
         self.folder_prenotazioni = api.content.create(
@@ -267,14 +269,99 @@
                 expected.append(
                     self.dt_local_to_json(
                         datetime(current_year, next_month, monday, 9, 0)
                     )
                 )
         self.assertEqual(expected, response.json()["items"])
 
+    @freeze_time(DATE_STR)
+    def test_if_first_available_return_the_first_available(
+        self,
+    ):
+        api_manager_session = RelativeSession(self.portal_url)
+        api_manager_session.headers.update({"Accept": "application/json"})
+        api_manager_session.auth = (SITE_OWNER_NAME, SITE_OWNER_PASSWORD)
+
+        now = date.today()
+        current_year = now.year
+        current_month = now.month
+        next_month = current_month + 1
+
+        self.folder_prenotazioni.daData = now
+        transaction.commit()
+
+        # all mondays in next month
+        response = api_manager_session.get(
+            "{}/@available-slots?first_available=true&start={}".format(
+                self.folder_prenotazioni.absolute_url(),
+                json_compatible(date(current_year, next_month, 1)),
+            )
+        )
+
+        # get first available slot
+        expected = []
+        for week in calendar.monthcalendar(current_year, next_month):
+            monday = week[0]
+            if monday > 0:
+                expected.append(
+                    self.dt_local_to_json(
+                        datetime(current_year, next_month, monday, 7, 0)
+                    )
+                )
+
+                break
+
+        self.assertEqual(expected, response.json()["items"])
+
+    @freeze_time(DATE_STR)
+    def test_if_first_available_and_no_bookign_manager_permission(
+        self,
+    ):
+        """Nothing to happen is expexted"""
+
+        api_manager_session = RelativeSession(self.portal_url)
+        api_manager_session.headers.update({"Accept": "application/json"})
+        api_manager_session.auth = (TEST_USER_ID, TEST_USER_PASSWORD)
+
+        now = date.today()
+        current_year = now.year
+        current_month = now.month
+        next_month = current_month + 1
+
+        self.folder_prenotazioni.daData = now
+
+        api.content.transition(self.folder_prenotazioni, transition="publish")
+
+        self.folder_prenotazioni.reindexObject(idxs=["review_state"])
+
+        setRoles(self.portal, TEST_USER_ID, ["Anonymous"])
+
+        transaction.commit()
+
+        # all mondays in next month
+        response = api_manager_session.get(
+            "{}/@available-slots?first_available=true&start={}".format(
+                self.folder_prenotazioni.absolute_url(),
+                json_compatible(date(current_year, current_month, 1)),
+            )
+        )
+
+        # get next mondays in next
+        expected = []
+        for week in calendar.monthcalendar(current_year, next_month):
+            monday = week[0]
+            if monday > 0:
+                expected.append(
+                    self.dt_local_to_json(
+                        datetime(current_year, next_month, monday, 7, 0)
+                    )
+                )
+
+        [self.assertNotIn(i, response.json()["items"]) for i in expected]
+
     def test_if_start_and_end_return_all_available_slots_between_these_dates(
         self,
     ):
         now = date.today()
         next_month = now + relativedelta.relativedelta(months=1)
         # all mondays in the first 10 days of next month
         response = self.api_session.get(
```

### Comparing `redturtle.prenotazioni-2.5.3/src/redturtle/prenotazioni/tests/test_base_slot.py` & `redturtle.prenotazioni-2.6.0/src/redturtle/prenotazioni/tests/test_base_slot.py`

 * *Files identical despite different names*

### Comparing `redturtle.prenotazioni-2.5.3/src/redturtle/prenotazioni/tests/test_booker_choose_available_slot.py` & `redturtle.prenotazioni-2.6.0/src/redturtle/prenotazioni/tests/test_booker_choose_available_slot.py`

 * *Files identical despite different names*

### Comparing `redturtle.prenotazioni-2.5.3/src/redturtle/prenotazioni/tests/test_booking_info.py` & `redturtle.prenotazioni-2.6.0/src/redturtle/prenotazioni/tests/test_booking_info.py`

 * *Files identical despite different names*

### Comparing `redturtle.prenotazioni-2.5.3/src/redturtle/prenotazioni/tests/test_booking_notify.py` & `redturtle.prenotazioni-2.6.0/src/redturtle/prenotazioni/tests/test_booking_notify.py`

 * *Files identical despite different names*

### Comparing `redturtle.prenotazioni-2.5.3/src/redturtle/prenotazioni/tests/test_booking_schema.py` & `redturtle.prenotazioni-2.6.0/src/redturtle/prenotazioni/tests/test_booking_schema.py`

 * *Files identical despite different names*

### Comparing `redturtle.prenotazioni-2.5.3/src/redturtle/prenotazioni/tests/test_bookings_num_limit.py` & `redturtle.prenotazioni-2.6.0/src/redturtle/prenotazioni/tests/test_bookings_num_limit.py`

 * *Files identical despite different names*

### Comparing `redturtle.prenotazioni-2.5.3/src/redturtle/prenotazioni/tests/test_browser_utilities_notify_upcoming_bookings.py` & `redturtle.prenotazioni-2.6.0/src/redturtle/prenotazioni/tests/test_browser_utilities_notify_upcoming_bookings.py`

 * *Files identical despite different names*

### Comparing `redturtle.prenotazioni-2.5.3/src/redturtle/prenotazioni/tests/test_content_validators_validate_pause_table.py` & `redturtle.prenotazioni-2.6.0/src/redturtle/prenotazioni/tests/test_content_validators_validate_pause_table.py`

 * *Files identical despite different names*

### Comparing `redturtle.prenotazioni-2.5.3/src/redturtle/prenotazioni/tests/test_day.py` & `redturtle.prenotazioni-2.6.0/src/redturtle/prenotazioni/tests/test_day.py`

 * *Files 24% similar despite different names*

```diff
@@ -169,7 +169,24 @@
                 "morning": {
                     "start": tomorrow_start_utc.strftime("%Y-%m-%dT%H:%M:00+00:00"),
                     "end": tomorrow_end_utc.strftime("%Y-%m-%dT%H:%M:00+00:00"),
                 },
             },
             results["gates"][0]["daily_schedule"],
         )
+
+    def test_requested_day_is_out_of_range(self):
+        self.folder_prenotazioni.aData = self.today.date()
+
+        commit()
+
+        response = self.api_session.get(
+            f"{self.folder_prenotazioni.absolute_url()}/@day/{self.tomorrow.isoformat()}"
+        )
+
+        self.assertEqual(response.status_code, 200)
+
+        results = response.json()
+
+        self.assertEquals(results["gates"], [])
+        self.assertEquals(results["pauses"], [])
+        self.assertEquals(results["bookings"], [])
```

### Comparing `redturtle.prenotazioni-2.5.3/src/redturtle/prenotazioni/tests/test_delete_booking.py` & `redturtle.prenotazioni-2.6.0/src/redturtle/prenotazioni/tests/test_delete_booking.py`

 * *Files identical despite different names*

### Comparing `redturtle.prenotazioni-2.5.3/src/redturtle/prenotazioni/tests/test_delete_booking_api.py` & `redturtle.prenotazioni-2.6.0/src/redturtle/prenotazioni/tests/test_delete_booking_api.py`

 * *Files identical despite different names*

### Comparing `redturtle.prenotazioni-2.5.3/src/redturtle/prenotazioni/tests/test_gates_overrides.py` & `redturtle.prenotazioni-2.6.0/src/redturtle/prenotazioni/tests/test_gates_overrides.py`

 * *Files identical despite different names*

### Comparing `redturtle.prenotazioni-2.5.3/src/redturtle/prenotazioni/tests/test_move_booking_api.py` & `redturtle.prenotazioni-2.6.0/src/redturtle/prenotazioni/tests/test_move_booking_api.py`

 * *Files 2% similar despite different names*

```diff
@@ -1,9 +1,8 @@
 # -*- coding: utf-8 -*-
-import time
 import unittest
 from datetime import date
 from datetime import datetime
 from datetime import timedelta
 
 import pytz
 import transaction
@@ -221,15 +220,14 @@
         response = self.api_session_admin.get(
             f"{self.folder_prenotazioni.absolute_url()}/@booking/{uid}"
         ).json()
 
         self.assertEqual(old_modified, response["modification_date"])
 
         # now move the booking
-        time.sleep(1)
         tomorrow = self.today + timedelta(1)
         response = self.api_session_admin.post(
             f"{self.folder_prenotazioni.absolute_url()}/@booking-move",
             json={
                 "booking_id": uid,
                 "booking_date": tomorrow.isoformat(),  # tomorrow
             },
```

### Comparing `redturtle.prenotazioni-2.5.3/src/redturtle/prenotazioni/tests/test_notification_supervisor_utility.py` & `redturtle.prenotazioni-2.6.0/src/redturtle/prenotazioni/tests/test_notification_supervisor_utility.py`

 * *Files identical despite different names*

### Comparing `redturtle.prenotazioni-2.5.3/src/redturtle/prenotazioni/tests/test_pauses_overrides.py` & `redturtle.prenotazioni-2.6.0/src/redturtle/prenotazioni/tests/test_pauses_overrides.py`

 * *Files identical despite different names*

### Comparing `redturtle.prenotazioni-2.5.3/src/redturtle/prenotazioni/tests/test_prenotazione_email_sent_to_managers.py` & `redturtle.prenotazioni-2.6.0/src/redturtle/prenotazioni/tests/test_prenotazione_email_sent_to_managers.py`

 * *Files identical despite different names*

### Comparing `redturtle.prenotazioni-2.5.3/src/redturtle/prenotazioni/tests/test_prenotazione_events.py` & `redturtle.prenotazioni-2.6.0/src/redturtle/prenotazioni/tests/test_prenotazione_events.py`

 * *Files identical despite different names*

### Comparing `redturtle.prenotazioni-2.5.3/src/redturtle/prenotazioni/tests/test_prenotazione_searchable_item_serializer.py` & `redturtle.prenotazioni-2.6.0/src/redturtle/prenotazioni/tests/test_prenotazione_searchable_item_serializer.py`

 * *Files identical despite different names*

### Comparing `redturtle.prenotazioni-2.5.3/src/redturtle/prenotazioni/tests/test_prenotazioni_context_state.py` & `redturtle.prenotazioni-2.6.0/src/redturtle/prenotazioni/tests/test_prenotazioni_context_state.py`

 * *Files identical despite different names*

### Comparing `redturtle.prenotazioni-2.5.3/src/redturtle/prenotazioni/tests/test_prenotazioni_folder_holidays_constraint.py` & `redturtle.prenotazioni-2.6.0/src/redturtle/prenotazioni/tests/test_prenotazioni_folder_holidays_constraint.py`

 * *Files identical despite different names*

### Comparing `redturtle.prenotazioni-2.5.3/src/redturtle/prenotazioni/tests/test_prenotazioni_search.py` & `redturtle.prenotazioni-2.6.0/src/redturtle/prenotazioni/tests/test_prenotazioni_search.py`

 * *Files identical despite different names*

### Comparing `redturtle.prenotazioni-2.5.3/src/redturtle/prenotazioni/tests/test_restapi_types_override.py` & `redturtle.prenotazioni-2.6.0/src/redturtle/prenotazioni/tests/test_restapi_types_override.py`

 * *Files identical despite different names*

### Comparing `redturtle.prenotazioni-2.5.3/src/redturtle/prenotazioni/tests/test_send_ical.py` & `redturtle.prenotazioni-2.6.0/src/redturtle/prenotazioni/tests/test_send_ical.py`

 * *Files identical despite different names*

### Comparing `redturtle.prenotazioni-2.5.3/src/redturtle/prenotazioni/tests/test_setup.py` & `redturtle.prenotazioni-2.6.0/src/redturtle/prenotazioni/tests/test_setup.py`

 * *Files identical despite different names*

### Comparing `redturtle.prenotazioni-2.5.3/src/redturtle/prenotazioni/tests/test_stringinterp.py` & `redturtle.prenotazioni-2.6.0/src/redturtle/prenotazioni/tests/test_stringinterp.py`

 * *Files identical despite different names*

### Comparing `redturtle.prenotazioni-2.5.3/src/redturtle/prenotazioni/tests/test_utils.py` & `redturtle.prenotazioni-2.6.0/src/redturtle/prenotazioni/tests/test_utils.py`

 * *Files identical despite different names*

### Comparing `redturtle.prenotazioni-2.5.3/src/redturtle/prenotazioni/tests/test_vacation_api.py` & `redturtle.prenotazioni-2.6.0/src/redturtle/prenotazioni/tests/test_vacation_api.py`

 * *Files identical despite different names*

### Comparing `redturtle.prenotazioni-2.5.3/src/redturtle/prenotazioni/tests/test_vocabularies.py` & `redturtle.prenotazioni-2.6.0/src/redturtle/prenotazioni/tests/test_vocabularies.py`

 * *Files identical despite different names*

### Comparing `redturtle.prenotazioni-2.5.3/src/redturtle/prenotazioni/tests/test_week_table_overrides.py` & `redturtle.prenotazioni-2.6.0/src/redturtle/prenotazioni/tests/test_week_table_overrides.py`

 * *Files 7% similar despite different names*

```diff
@@ -28,15 +28,15 @@
 
         self.folder_prenotazioni = api.content.create(
             container=self.portal,
             type="PrenotazioniFolder",
             title="Prenota foo",
             description="",
             daData=date.today(),
-            gates=["Gate A"],
+            gates=["Gate A", "Gate B"],
             week_table=[
                 {
                     "day": "Lunedì",
                     "morning_start": "0700",
                     "morning_end": "1000",
                     "afternoon_start": None,
                     "afternoon_end": None,
@@ -76,26 +76,22 @@
             context=self.folder_prenotazioni,
             request=self.request,
         )
 
     def test_if_day_not_in_overrides_use_default_week_table(self):
         now = date.today()
         res = self.view.get_week_table(date(now.year, 6, 1))
-        self.assertEqual(res, {"Gate A": self.folder_prenotazioni.week_table})
+        self.assertEqual(res["Gate A"], self.folder_prenotazioni.week_table)
 
     def test_if_day_is_in_overrides_use_override_week_table(self):
         now = date.today()
         res = self.view.get_week_table(date(now.year, 1, 10))
         self.assertEqual(
-            res,
-            {
-                "Gate A": json.loads(self.folder_prenotazioni.week_table_overrides)[0][
-                    "week_table"
-                ]
-            },
+            res["Gate A"],
+            json.loads(self.folder_prenotazioni.week_table_overrides)[0]["week_table"],
         )
 
     @freeze_time("2023-05-14")
     def test_override_between_year(self):
         self.folder_prenotazioni.week_table_overrides = json.dumps(
             [
                 {
@@ -115,45 +111,33 @@
                 }
             ]
         )
         now = date.today()
 
         # if in range, return table overrides
         self.assertEqual(
-            self.view.get_week_table(date(now.year, 12, 25)),
-            {
-                "Gate A": json.loads(self.folder_prenotazioni.week_table_overrides)[0][
-                    "week_table"
-                ]
-            },
+            self.view.get_week_table(date(now.year, 12, 25))["Gate A"],
+            json.loads(self.folder_prenotazioni.week_table_overrides)[0]["week_table"],
         )
 
         # if in range and next year, return table overrides
         self.assertEqual(
-            self.view.get_week_table(date(now.year + 1, 1, 25)),
-            {
-                "Gate A": json.loads(self.folder_prenotazioni.week_table_overrides)[0][
-                    "week_table"
-                ]
-            },
+            self.view.get_week_table(date(now.year + 1, 1, 25))["Gate A"],
+            json.loads(self.folder_prenotazioni.week_table_overrides)[0]["week_table"],
         )
         # if in range and next year +1, return table overrides
         self.assertEqual(
-            self.view.get_week_table(date(now.year + 1, 12, 25)),
-            {
-                "Gate A": json.loads(self.folder_prenotazioni.week_table_overrides)[0][
-                    "week_table"
-                ]
-            },
+            self.view.get_week_table(date(now.year + 1, 12, 25))["Gate A"],
+            json.loads(self.folder_prenotazioni.week_table_overrides)[0]["week_table"],
         )
 
         # if out of range, return base table
         self.assertEqual(
-            self.view.get_week_table(date(now.year, 10, 10)),
-            {"Gate A": self.folder_prenotazioni.week_table},
+            self.view.get_week_table(date(now.year, 10, 10))["Gate A"],
+            self.folder_prenotazioni.week_table,
         )
 
     @freeze_time("2023-05-14")
     def test_overrides_in_years_range(self):
         self.folder_prenotazioni.week_table_overrides = json.dumps(
             [
                 {
@@ -175,20 +159,16 @@
                 }
             ]
         )
         now = date.today()
 
         # if in range, return table overrides
         self.assertEqual(
-            self.view.get_week_table(date(now.year, 12, 25)),
-            {
-                "Gate A": json.loads(self.folder_prenotazioni.week_table_overrides)[0][
-                    "week_table"
-                ]
-            },
+            self.view.get_week_table(date(now.year, 12, 25))["Gate A"],
+            json.loads(self.folder_prenotazioni.week_table_overrides)[0]["week_table"],
         )
 
     @freeze_time("2023-05-14")
     def test_out_of_years_range_specific_override_not_affects(self):
         self.folder_prenotazioni.week_table_overrides = json.dumps(
             [
                 {
@@ -209,16 +189,16 @@
                     ],
                 }
             ]
         )
 
         # if out of range, return base table
         self.assertEqual(
-            self.view.get_week_table(date(2026, 10, 10)),
-            {"Gate A": self.folder_prenotazioni.week_table},
+            self.view.get_week_table(date(2026, 10, 10))["Gate A"],
+            self.folder_prenotazioni.week_table,
         )
 
     @freeze_time("2023-05-14")
     def test_years_specific_overrides_wins_over_the_generic(self):
         self.folder_prenotazioni.week_table_overrides = json.dumps(
             [
                 {
@@ -255,20 +235,16 @@
                 },
             ],
         )
         now = date.today()
 
         # if in range, return table overrides
         self.assertEqual(
-            self.view.get_week_table(date(now.year, 12, 25)),
-            {
-                "Gate A": json.loads(self.folder_prenotazioni.week_table_overrides)[0][
-                    "week_table"
-                ]
-            },
+            self.view.get_week_table(date(now.year, 12, 25))["Gate A"],
+            json.loads(self.folder_prenotazioni.week_table_overrides)[0]["week_table"],
         )
 
     @freeze_time("2023-05-14")
     def test_between_the_years_specific_overrides_win_the_last_one(self):
         self.folder_prenotazioni.week_table_overrides = json.dumps(
             [
                 {
@@ -323,20 +299,65 @@
                 },
             ],
         )
         now = date.today()
 
         # if in range, return table overrides
         self.assertEqual(
-            self.view.get_week_table(date(now.year, 12, 25)),
-            {
-                "Gate A": json.loads(self.folder_prenotazioni.week_table_overrides)[1][
-                    "week_table"
-                ]
-            },
+            self.view.get_week_table(date(now.year, 12, 25))["Gate A"],
+            json.loads(self.folder_prenotazioni.week_table_overrides)[1]["week_table"],
+        )
+
+    @freeze_time("2023-05-14")
+    def test_only_the_last_gate_is_returtned(self):
+        self.folder_prenotazioni.week_table_overrides = json.dumps(
+            [
+                {
+                    "from_year": "2021",
+                    "from_day": "1",
+                    "from_month": "12",
+                    "to_year": "2024",
+                    "to_day": "1",
+                    "to_month": "3",
+                    "gates": ["Gate B"],
+                    "week_table": [
+                        {
+                            "day": "Lunedì",
+                            "morning_start": "1200",
+                            "morning_end": "1300",
+                            "afternoon_start": None,
+                            "afternoon_end": None,
+                        },
+                    ],
+                },
+                {
+                    "from_year": "2021",
+                    "from_day": "1",
+                    "from_month": "12",
+                    "to_year": "2024",
+                    "to_day": "1",
+                    "to_month": "3",
+                    "gates": ["Gate B"],
+                    "week_table": [
+                        {
+                            "day": "Lunedì",
+                            "morning_start": "1300",
+                            "morning_end": "1400",
+                            "afternoon_start": None,
+                            "afternoon_end": None,
+                        },
+                    ],
+                },
+            ],
+        )
+        now = date.today()
+
+        self.assertEqual(
+            self.view.get_week_table(date(now.year, 12, 25))["Gate B"],
+            json.loads(self.folder_prenotazioni.week_table_overrides)[1]["week_table"],
         )
 
 
 class TestWeekTableOverridesApiValidateDataOnPost(unittest.TestCase):
     layer = REDTURTLE_PRENOTAZIONI_API_FUNCTIONAL_TESTING
 
     def setUp(self):
```

### Comparing `redturtle.prenotazioni-2.5.3/src/redturtle/prenotazioni/upgrades.py` & `redturtle.prenotazioni-2.6.0/src/redturtle/prenotazioni/upgrades.py`

 * *Files identical despite different names*

### Comparing `redturtle.prenotazioni-2.5.3/src/redturtle/prenotazioni/upgrades.zcml` & `redturtle.prenotazioni-2.6.0/src/redturtle/prenotazioni/upgrades.zcml`

 * *Files identical despite different names*

### Comparing `redturtle.prenotazioni-2.5.3/src/redturtle/prenotazioni/utilities/dateutils.py` & `redturtle.prenotazioni-2.6.0/src/redturtle/prenotazioni/utilities/dateutils.py`

 * *Files identical despite different names*

### Comparing `redturtle.prenotazioni-2.5.3/src/redturtle/prenotazioni/utilities/urls.py` & `redturtle.prenotazioni-2.6.0/src/redturtle/prenotazioni/utilities/urls.py`

 * *Files identical despite different names*

### Comparing `redturtle.prenotazioni-2.5.3/src/redturtle/prenotazioni/utils/get_prenotazioni_folder.py` & `redturtle.prenotazioni-2.6.0/src/redturtle/prenotazioni/utils/get_prenotazioni_folder.py`

 * *Files identical despite different names*

### Comparing `redturtle.prenotazioni-2.5.3/src/redturtle/prenotazioni/vocabularies/configure.zcml` & `redturtle.prenotazioni-2.6.0/src/redturtle/prenotazioni/vocabularies/configure.zcml`

 * *Files identical despite different names*

### Comparing `redturtle.prenotazioni-2.5.3/src/redturtle/prenotazioni/vocabularies/gates.py` & `redturtle.prenotazioni-2.6.0/src/redturtle/prenotazioni/vocabularies/gates.py`

 * *Files identical despite different names*

### Comparing `redturtle.prenotazioni-2.5.3/src/redturtle/prenotazioni/vocabularies/requirable_booking_fields.py` & `redturtle.prenotazioni-2.6.0/src/redturtle/prenotazioni/vocabularies/requirable_booking_fields.py`

 * *Files identical despite different names*

### Comparing `redturtle.prenotazioni-2.5.3/src/redturtle/prenotazioni/vocabularies/review_states.py` & `redturtle.prenotazioni-2.6.0/src/redturtle/prenotazioni/vocabularies/review_states.py`

 * *Files identical despite different names*

### Comparing `redturtle.prenotazioni-2.5.3/src/redturtle/prenotazioni/vocabularies/tipologies.py` & `redturtle.prenotazioni-2.6.0/src/redturtle/prenotazioni/vocabularies/tipologies.py`

 * *Files identical despite different names*

### Comparing `redturtle.prenotazioni-2.5.3/src/redturtle/prenotazioni/vocabularies/voc_booking_type_gates.py` & `redturtle.prenotazioni-2.6.0/src/redturtle/prenotazioni/vocabularies/voc_booking_type_gates.py`

 * *Files identical despite different names*

### Comparing `redturtle.prenotazioni-2.5.3/src/redturtle/prenotazioni/vocabularies/voc_durata_incontro.py` & `redturtle.prenotazioni-2.6.0/src/redturtle/prenotazioni/vocabularies/voc_durata_incontro.py`

 * *Files identical despite different names*

### Comparing `redturtle.prenotazioni-2.5.3/src/redturtle/prenotazioni/vocabularies/voc_months.py` & `redturtle.prenotazioni-2.6.0/src/redturtle/prenotazioni/vocabularies/voc_months.py`

 * *Files identical despite different names*

### Comparing `redturtle.prenotazioni-2.5.3/src/redturtle/prenotazioni/vocabularies/voc_ore_inizio.py` & `redturtle.prenotazioni-2.6.0/src/redturtle/prenotazioni/vocabularies/voc_ore_inizio.py`

 * *Files identical despite different names*

### Comparing `redturtle.prenotazioni-2.5.3/src/redturtle.prenotazioni.egg-info/PKG-INFO` & `redturtle.prenotazioni-2.6.0/src/redturtle.prenotazioni.egg-info/PKG-INFO`

 * *Files 2% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: redturtle.prenotazioni
-Version: 2.5.3
+Version: 2.6.0
 Summary: An add-on for Plone
 Home-page: https://github.com/redturtle/redturtle.prenotazioni
 Author: RedTurtle Technology
 Author-email: sviluppoplone@redturtle.it
 License: GPL version 2
 Project-URL: PyPI, https://pypi.org/project/redturtle.prenotazioni
 Project-URL: Source, https://github.com/redturtle/redturtle.prenotazioni
@@ -475,15 +475,15 @@
 
 By default (without parameters) the endpoint returns available slots for the current month, starting from today.
 
 Parameters:
 
 - **start** a start date. If not given, the start will be today.
 - **end** an end date. If not given, the end will be the last day of current month.
-
+- **first_available** a boolean flag, if valiorized, the first available slot returned without the current month search limit but the one year.
 
 Example::
 
    curl -i http://localhost:8080/Plone/folder/@available-slots -H 'Accept: application/json'
 
 Response::
 
@@ -934,14 +934,30 @@
 .. _List of contributors: https://github.com/RedTurtle/redturtle.prenotazioni/graphs/contributors
 
 
 Changelog
 =========
 
 
+2.6.0 (2024-04-02)
+------------------
+
+- Return empty data from the @day endpoint if requested date is out of PrenotazioniFolder range
+  [folix-01]
+
+- Fix double gate bug.
+  [folix-01]
+
+- first_available flag for the @available-slots endpoint.
+  [folix-01]
+
+- Fix double gate when it is repeated in more than one week table overrides.
+  [folix-01]
+
+
 2.5.3 (2024-03-19)
 ------------------
 
 - Fix SMS links. Removed the dot immediately after the url
   [folix-01]
 
 
@@ -955,15 +971,15 @@
   [folix-01]
 
 2.5.1 (2024-03-06)
 ------------------
 
 - Add the years range configuration to week table overrides.
   [folix-01]
- 
+
 - Bypass the today delete limit for the 'out-of-office' types
   [folix-01]
 
 - Change the booking notification flag label.
   [folix-01]
```

### Comparing `redturtle.prenotazioni-2.5.3/src/redturtle.prenotazioni.egg-info/SOURCES.txt` & `redturtle.prenotazioni-2.6.0/src/redturtle.prenotazioni.egg-info/SOURCES.txt`

 * *Files 1% similar despite different names*

```diff
@@ -173,16 +173,19 @@
 src/redturtle/prenotazioni/io_tools/rdbms.py
 src/redturtle/prenotazioni/io_tools/spec.yaml
 src/redturtle/prenotazioni/io_tools/storage.py
 src/redturtle/prenotazioni/locales/manual.pot
 src/redturtle/prenotazioni/locales/redturtle.prenotazioni.pot
 src/redturtle/prenotazioni/locales/update.py
 src/redturtle/prenotazioni/locales/update.sh
+src/redturtle/prenotazioni/locales/en/LC_MESSAGES/redturtle.prenotazioni.mo
 src/redturtle/prenotazioni/locales/en/LC_MESSAGES/redturtle.prenotazioni.po
+src/redturtle/prenotazioni/locales/it/LC_MESSAGES/plone.mo
 src/redturtle/prenotazioni/locales/it/LC_MESSAGES/plone.po
+src/redturtle/prenotazioni/locales/it/LC_MESSAGES/redturtle.prenotazioni.mo
 src/redturtle/prenotazioni/locales/it/LC_MESSAGES/redturtle.prenotazioni.po
 src/redturtle/prenotazioni/monkeypatcher/__init__.py
 src/redturtle/prenotazioni/monkeypatcher/configure.zcml
 src/redturtle/prenotazioni/profiles/default/actions.xml
 src/redturtle/prenotazioni/profiles/default/browserlayer.xml
 src/redturtle/prenotazioni/profiles/default/catalog.xml
 src/redturtle/prenotazioni/profiles/default/contentrules.xml
```

