# Comparing `tmp/redturtle.prenotazioni-2.6.5.tar.gz` & `tmp/redturtle.prenotazioni-2.7.0.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "redturtle.prenotazioni-2.6.5.tar", last modified: Wed Apr 24 08:56:49 2024, max compression
+gzip compressed data, was "redturtle.prenotazioni-2.7.0.tar", last modified: Wed May 29 09:53:33 2024, max compression
```

## Comparing `redturtle.prenotazioni-2.6.5.tar` & `redturtle.prenotazioni-2.7.0.tar`

### file list

```diff
@@ -1,378 +1,381 @@
-drwxr-xr-x   0 roman      (502) staff       (20)        0 2024-04-24 08:56:49.776600 redturtle.prenotazioni-2.6.5/
--rw-r--r--   0 roman      (502) staff       (20)      748 2024-04-24 08:56:49.000000 redturtle.prenotazioni-2.6.5/APP_IO.txt
--rw-r--r--   0 roman      (502) staff       (20)    17651 2024-04-24 08:56:49.000000 redturtle.prenotazioni-2.6.5/CHANGES.rst
--rw-r--r--   0 roman      (502) staff       (20)      152 2024-04-24 08:56:49.000000 redturtle.prenotazioni-2.6.5/CONTRIBUTORS.rst
--rw-r--r--   0 roman      (502) staff       (20)      586 2024-04-24 08:56:49.000000 redturtle.prenotazioni-2.6.5/DEVELOP.rst
--rw-r--r--   0 roman      (502) staff       (20)    18092 2024-04-24 08:56:49.000000 redturtle.prenotazioni-2.6.5/LICENSE.GPL
--rw-r--r--   0 roman      (502) staff       (20)      667 2024-04-24 08:56:49.000000 redturtle.prenotazioni-2.6.5/LICENSE.rst
--rw-r--r--   0 roman      (502) staff       (20)      110 2024-04-24 08:56:49.000000 redturtle.prenotazioni-2.6.5/MANIFEST.in
--rw-r--r--   0 roman      (502) staff       (20)    61067 2024-04-24 08:56:49.777049 redturtle.prenotazioni-2.6.5/PKG-INFO
--rw-r--r--   0 roman      (502) staff       (20)    27508 2024-04-24 08:56:49.000000 redturtle.prenotazioni-2.6.5/README.rst
--rw-r--r--   0 roman      (502) staff       (20)      164 2024-04-24 08:56:49.000000 redturtle.prenotazioni-2.6.5/TODO.txt
--rw-r--r--   0 roman      (502) staff       (20)      105 2024-04-24 08:56:49.000000 redturtle.prenotazioni-2.6.5/constraints-5.2.x.txt
--rw-r--r--   0 roman      (502) staff       (20)      105 2024-04-24 08:56:49.000000 redturtle.prenotazioni-2.6.5/constraints.txt
-drwxr-xr-x   0 roman      (502) staff       (20)        0 2024-04-24 08:56:49.706302 redturtle.prenotazioni-2.6.5/docs/
--rw-r--r--   0 roman      (502) staff       (20)     7984 2024-04-24 08:56:49.000000 redturtle.prenotazioni-2.6.5/docs/conf.py
--rw-r--r--   0 roman      (502) staff       (20)       89 2024-04-24 08:56:49.000000 redturtle.prenotazioni-2.6.5/docs/index.rst
--rw-r--r--   0 roman      (502) staff       (20)      476 2024-04-24 08:56:49.000000 redturtle.prenotazioni-2.6.5/requirements-6.0.x.txt
--rw-r--r--   0 roman      (502) staff       (20)       48 2024-04-24 08:56:49.000000 redturtle.prenotazioni-2.6.5/requirements.txt
--rw-r--r--   0 roman      (502) staff       (20)      344 2024-04-24 08:56:49.777632 redturtle.prenotazioni-2.6.5/setup.cfg
--rw-r--r--   0 roman      (502) staff       (20)     3420 2024-04-24 08:56:49.000000 redturtle.prenotazioni-2.6.5/setup.py
-drwxr-xr-x   0 roman      (502) staff       (20)        0 2024-04-24 08:56:49.693874 redturtle.prenotazioni-2.6.5/src/
-drwxr-xr-x   0 roman      (502) staff       (20)        0 2024-04-24 08:56:49.706527 redturtle.prenotazioni-2.6.5/src/redturtle/
--rw-r--r--   0 roman      (502) staff       (20)       80 2024-04-24 08:56:49.000000 redturtle.prenotazioni-2.6.5/src/redturtle/__init__.py
-drwxr-xr-x   0 roman      (502) staff       (20)        0 2024-04-24 08:56:49.711233 redturtle.prenotazioni-2.6.5/src/redturtle/prenotazioni/
--rw-r--r--   0 roman      (502) staff       (20)     4638 2024-04-24 08:56:49.000000 redturtle.prenotazioni-2.6.5/src/redturtle/prenotazioni/__init__.py
-drwxr-xr-x   0 roman      (502) staff       (20)        0 2024-04-24 08:56:49.711888 redturtle.prenotazioni-2.6.5/src/redturtle/prenotazioni/actions/
--rw-r--r--   0 roman      (502) staff       (20)        0 2024-04-24 08:56:49.000000 redturtle.prenotazioni-2.6.5/src/redturtle/prenotazioni/actions/__init__.py
--rw-r--r--   0 roman      (502) staff       (20)      226 2024-04-24 08:56:49.000000 redturtle.prenotazioni-2.6.5/src/redturtle/prenotazioni/actions/configure.zcml
--rw-r--r--   0 roman      (502) staff       (20)     3333 2024-04-24 08:56:49.000000 redturtle.prenotazioni-2.6.5/src/redturtle/prenotazioni/actions/mail.py
-drwxr-xr-x   0 roman      (502) staff       (20)        0 2024-04-24 08:56:49.714050 redturtle.prenotazioni-2.6.5/src/redturtle/prenotazioni/adapters/
--rw-r--r--   0 roman      (502) staff       (20)       24 2024-04-24 08:56:49.000000 redturtle.prenotazioni-2.6.5/src/redturtle/prenotazioni/adapters/__init__.py
--rw-r--r--   0 roman      (502) staff       (20)    15296 2024-04-24 08:56:49.000000 redturtle.prenotazioni-2.6.5/src/redturtle/prenotazioni/adapters/booker.py
--rw-r--r--   0 roman      (502) staff       (20)      729 2024-04-24 08:56:49.000000 redturtle.prenotazioni-2.6.5/src/redturtle/prenotazioni/adapters/booking_code.py
--rw-r--r--   0 roman      (502) staff       (20)     5974 2024-04-24 08:56:49.000000 redturtle.prenotazioni-2.6.5/src/redturtle/prenotazioni/adapters/configure.zcml
--rw-r--r--   0 roman      (502) staff       (20)     4988 2024-04-24 08:56:49.000000 redturtle.prenotazioni-2.6.5/src/redturtle/prenotazioni/adapters/conflict.py
--rw-r--r--   0 roman      (502) staff       (20)     5037 2024-04-24 08:56:49.000000 redturtle.prenotazioni-2.6.5/src/redturtle/prenotazioni/adapters/ical.py
--rw-r--r--   0 roman      (502) staff       (20)      273 2024-04-24 08:56:49.000000 redturtle.prenotazioni-2.6.5/src/redturtle/prenotazioni/adapters/prenotazione_menu.py
--rw-r--r--   0 roman      (502) staff       (20)     9662 2024-04-24 08:56:49.000000 redturtle.prenotazioni-2.6.5/src/redturtle/prenotazioni/adapters/slot.py
--rw-r--r--   0 roman      (502) staff       (20)     8771 2024-04-24 08:56:49.000000 redturtle.prenotazioni-2.6.5/src/redturtle/prenotazioni/adapters/stringinterp.py
-drwxr-xr-x   0 roman      (502) staff       (20)        0 2024-04-24 08:56:49.714279 redturtle.prenotazioni-2.6.5/src/redturtle/prenotazioni/behaviors/
-drwxr-xr-x   0 roman      (502) staff       (20)        0 2024-04-24 08:56:49.714994 redturtle.prenotazioni-2.6.5/src/redturtle/prenotazioni/behaviors/booking_folder/
--rw-r--r--   0 roman      (502) staff       (20)        0 2024-04-24 08:56:49.000000 redturtle.prenotazioni-2.6.5/src/redturtle/prenotazioni/behaviors/booking_folder/__init__.py
--rw-r--r--   0 roman      (502) staff       (20)      563 2024-04-24 08:56:49.000000 redturtle.prenotazioni-2.6.5/src/redturtle/prenotazioni/behaviors/booking_folder/configure.zcml
--rw-r--r--   0 roman      (502) staff       (20)     1766 2024-04-24 08:56:49.000000 redturtle.prenotazioni-2.6.5/src/redturtle/prenotazioni/behaviors/booking_folder/contacts.py
-drwxr-xr-x   0 roman      (502) staff       (20)        0 2024-04-24 08:56:49.715446 redturtle.prenotazioni-2.6.5/src/redturtle/prenotazioni/behaviors/booking_folder/notifications/
--rw-r--r--   0 roman      (502) staff       (20)     1454 2024-04-24 08:56:49.000000 redturtle.prenotazioni-2.6.5/src/redturtle/prenotazioni/behaviors/booking_folder/notifications/__init__.py
-drwxr-xr-x   0 roman      (502) staff       (20)        0 2024-04-24 08:56:49.716891 redturtle.prenotazioni-2.6.5/src/redturtle/prenotazioni/behaviors/booking_folder/notifications/appio/
--rw-r--r--   0 roman      (502) staff       (20)    10220 2024-04-24 08:56:49.000000 redturtle.prenotazioni-2.6.5/src/redturtle/prenotazioni/behaviors/booking_folder/notifications/appio/__init__.py
--rw-r--r--   0 roman      (502) staff       (20)     4071 2024-04-24 08:56:49.000000 redturtle.prenotazioni-2.6.5/src/redturtle/prenotazioni/behaviors/booking_folder/notifications/appio/adapters.py
--rw-r--r--   0 roman      (502) staff       (20)     2364 2024-04-24 08:56:49.000000 redturtle.prenotazioni-2.6.5/src/redturtle/prenotazioni/behaviors/booking_folder/notifications/appio/configure.zcml
--rw-r--r--   0 roman      (502) staff       (20)     2592 2024-04-24 08:56:49.000000 redturtle.prenotazioni-2.6.5/src/redturtle/prenotazioni/behaviors/booking_folder/notifications/appio/events.py
--rw-r--r--   0 roman      (502) staff       (20)     3178 2024-04-24 08:56:49.000000 redturtle.prenotazioni-2.6.5/src/redturtle/prenotazioni/behaviors/booking_folder/notifications/appio/notfication_appio_message.py
--rw-r--r--   0 roman      (502) staff       (20)     1151 2024-04-24 08:56:49.000000 redturtle.prenotazioni-2.6.5/src/redturtle/prenotazioni/behaviors/booking_folder/notifications/appio/voc_service_keys.py
--rw-r--r--   0 roman      (502) staff       (20)      423 2024-04-24 08:56:49.000000 redturtle.prenotazioni-2.6.5/src/redturtle/prenotazioni/behaviors/booking_folder/notifications/configure.zcml
-drwxr-xr-x   0 roman      (502) staff       (20)        0 2024-04-24 08:56:49.718368 redturtle.prenotazioni-2.6.5/src/redturtle/prenotazioni/behaviors/booking_folder/notifications/email/
--rw-r--r--   0 roman      (502) staff       (20)     9647 2024-04-24 08:56:49.000000 redturtle.prenotazioni-2.6.5/src/redturtle/prenotazioni/behaviors/booking_folder/notifications/email/__init__.py
--rw-r--r--   0 roman      (502) staff       (20)     1607 2024-04-24 08:56:49.000000 redturtle.prenotazioni-2.6.5/src/redturtle/prenotazioni/behaviors/booking_folder/notifications/email/adapters.py
--rw-r--r--   0 roman      (502) staff       (20)     2284 2024-04-24 08:56:49.000000 redturtle.prenotazioni-2.6.5/src/redturtle/prenotazioni/behaviors/booking_folder/notifications/email/configure.zcml
--rw-r--r--   0 roman      (502) staff       (20)     3600 2024-04-24 08:56:49.000000 redturtle.prenotazioni-2.6.5/src/redturtle/prenotazioni/behaviors/booking_folder/notifications/email/events.py
--rw-r--r--   0 roman      (502) staff       (20)    11940 2024-04-24 08:56:49.000000 redturtle.prenotazioni-2.6.5/src/redturtle/prenotazioni/behaviors/booking_folder/notifications/email/notification_email_message.py
-drwxr-xr-x   0 roman      (502) staff       (20)        0 2024-04-24 08:56:49.719574 redturtle.prenotazioni-2.6.5/src/redturtle/prenotazioni/behaviors/booking_folder/notifications/sms/
--rw-r--r--   0 roman      (502) staff       (20)     5724 2024-04-24 08:56:49.000000 redturtle.prenotazioni-2.6.5/src/redturtle/prenotazioni/behaviors/booking_folder/notifications/sms/__init__.py
--rw-r--r--   0 roman      (502) staff       (20)     1115 2024-04-24 08:56:49.000000 redturtle.prenotazioni-2.6.5/src/redturtle/prenotazioni/behaviors/booking_folder/notifications/sms/adapters.py
--rw-r--r--   0 roman      (502) staff       (20)     1689 2024-04-24 08:56:49.000000 redturtle.prenotazioni-2.6.5/src/redturtle/prenotazioni/behaviors/booking_folder/notifications/sms/configure.zcml
--rw-r--r--   0 roman      (502) staff       (20)     2931 2024-04-24 08:56:49.000000 redturtle.prenotazioni-2.6.5/src/redturtle/prenotazioni/behaviors/booking_folder/notifications/sms/events.py
--rw-r--r--   0 roman      (502) staff       (20)     2216 2024-04-24 08:56:49.000000 redturtle.prenotazioni-2.6.5/src/redturtle/prenotazioni/behaviors/booking_folder/notifications/sms/message.py
--rw-r--r--   0 roman      (502) staff       (20)      284 2024-04-24 08:56:49.000000 redturtle.prenotazioni-2.6.5/src/redturtle/prenotazioni/behaviors/configure.zcml
-drwxr-xr-x   0 roman      (502) staff       (20)        0 2024-04-24 08:56:49.724007 redturtle.prenotazioni-2.6.5/src/redturtle/prenotazioni/browser/
--rw-r--r--   0 roman      (502) staff       (20)        0 2024-04-24 08:56:49.000000 redturtle.prenotazioni-2.6.5/src/redturtle/prenotazioni/browser/__init__.py
--rw-r--r--   0 roman      (502) staff       (20)     1817 2024-04-24 08:56:49.000000 redturtle.prenotazioni-2.6.5/src/redturtle/prenotazioni/browser/base.py
--rw-r--r--   0 roman      (502) staff       (20)     7331 2024-04-24 08:56:49.000000 redturtle.prenotazioni-2.6.5/src/redturtle/prenotazioni/browser/configure.zcml
--rw-r--r--   0 roman      (502) staff       (20)      655 2024-04-24 08:56:49.000000 redturtle.prenotazioni-2.6.5/src/redturtle/prenotazioni/browser/custom_radio_input.pt
--rw-r--r--   0 roman      (502) staff       (20)     5709 2024-04-24 08:56:49.000000 redturtle.prenotazioni-2.6.5/src/redturtle/prenotazioni/browser/delete_reservation.py
--rw-r--r--   0 roman      (502) staff       (20)      673 2024-04-24 08:56:49.000000 redturtle.prenotazioni-2.6.5/src/redturtle/prenotazioni/browser/folderfactories.py
--rw-r--r--   0 roman      (502) staff       (20)      155 2024-04-24 08:56:49.000000 redturtle.prenotazioni-2.6.5/src/redturtle/prenotazioni/browser/interfaces.py
-drwxr-xr-x   0 roman      (502) staff       (20)        0 2024-04-24 08:56:49.724231 redturtle.prenotazioni-2.6.5/src/redturtle/prenotazioni/browser/overrides/
--rw-r--r--   0 roman      (502) staff       (20)        0 2024-04-24 08:56:49.000000 redturtle.prenotazioni-2.6.5/src/redturtle/prenotazioni/browser/overrides/.gitkeep
--rw-r--r--   0 roman      (502) staff       (20)     3169 2024-04-24 08:56:49.000000 redturtle.prenotazioni-2.6.5/src/redturtle/prenotazioni/browser/prenotazione.py
--rw-r--r--   0 roman      (502) staff       (20)    10057 2024-04-24 08:56:49.000000 redturtle.prenotazioni-2.6.5/src/redturtle/prenotazioni/browser/prenotazione_add.py
--rw-r--r--   0 roman      (502) staff       (20)     5252 2024-04-24 08:56:49.000000 redturtle.prenotazioni-2.6.5/src/redturtle/prenotazioni/browser/prenotazione_move.py
--rw-r--r--   0 roman      (502) staff       (20)     2721 2024-04-24 08:56:49.000000 redturtle.prenotazioni-2.6.5/src/redturtle/prenotazioni/browser/prenotazione_print.py
--rw-r--r--   0 roman      (502) staff       (20)    38319 2024-04-24 08:56:49.000000 redturtle.prenotazioni-2.6.5/src/redturtle/prenotazioni/browser/prenotazioni_context_state.py
--rw-r--r--   0 roman      (502) staff       (20)     1735 2024-04-24 08:56:49.000000 redturtle.prenotazioni-2.6.5/src/redturtle/prenotazioni/browser/prenotazioni_portal_state.py
--rw-r--r--   0 roman      (502) staff       (20)    13800 2024-04-24 08:56:49.000000 redturtle.prenotazioni-2.6.5/src/redturtle/prenotazioni/browser/prenotazioni_search.py
-drwxr-xr-x   0 roman      (502) staff       (20)        0 2024-04-24 08:56:49.725750 redturtle.prenotazioni-2.6.5/src/redturtle/prenotazioni/browser/static/
--rw-r--r--   0 roman      (502) staff       (20)        0 2024-04-24 08:56:49.000000 redturtle.prenotazioni-2.6.5/src/redturtle/prenotazioni/browser/static/.gitkeep
--rw-r--r--   0 roman      (502) staff       (20)      364 2024-04-24 08:56:49.000000 redturtle.prenotazioni-2.6.5/src/redturtle/prenotazioni/browser/static/calendar-add.png
--rw-r--r--   0 roman      (502) staff       (20)      503 2024-04-24 08:56:49.000000 redturtle.prenotazioni-2.6.5/src/redturtle/prenotazioni/browser/static/calendar-icon.png
--rw-r--r--   0 roman      (502) staff       (20)      266 2024-04-24 08:56:49.000000 redturtle.prenotazioni-2.6.5/src/redturtle/prenotazioni/browser/static/cross-icon.png
--rw-r--r--   0 roman      (502) staff       (20)     9794 2024-04-24 08:56:49.000000 redturtle.prenotazioni-2.6.5/src/redturtle/prenotazioni/browser/static/redturtle-reservation.css
--rw-r--r--   0 roman      (502) staff       (20)     1600 2024-04-24 08:56:49.000000 redturtle.prenotazioni-2.6.5/src/redturtle/prenotazioni/browser/static/redturtle-reservation.js
--rw-r--r--   0 roman      (502) staff       (20)      922 2024-04-24 08:56:49.000000 redturtle.prenotazioni-2.6.5/src/redturtle/prenotazioni/browser/static/times-solid.png
-drwxr-xr-x   0 roman      (502) staff       (20)        0 2024-04-24 08:56:49.696170 redturtle.prenotazioni-2.6.5/src/redturtle/prenotazioni/browser/static/widget/
-drwxr-xr-x   0 roman      (502) staff       (20)        0 2024-04-24 08:56:49.696046 redturtle.prenotazioni-2.6.5/src/redturtle/prenotazioni/browser/static/widget/dist/
-drwxr-xr-x   0 roman      (502) staff       (20)        0 2024-04-24 08:56:49.727057 redturtle.prenotazioni-2.6.5/src/redturtle/prenotazioni/browser/static/widget/dist/prod/
--rw-r--r--   0 roman      (502) staff       (20)     3239 2024-04-24 08:56:49.000000 redturtle.prenotazioni-2.6.5/src/redturtle/prenotazioni/browser/static/widget/dist/prod/main.css
--rw-r--r--   0 roman      (502) staff       (20)     3808 2024-04-24 08:56:49.000000 redturtle.prenotazioni-2.6.5/src/redturtle/prenotazioni/browser/static/widget/dist/prod/main.css.map
--rw-r--r--   0 roman      (502) staff       (20)   349785 2024-04-24 08:56:49.000000 redturtle.prenotazioni-2.6.5/src/redturtle/prenotazioni/browser/static/widget/dist/prod/main.js
--rw-r--r--   0 roman      (502) staff       (20)      148 2024-04-24 08:56:49.000000 redturtle.prenotazioni-2.6.5/src/redturtle/prenotazioni/browser/static/widget/dist/prod/main.js.map
-drwxr-xr-x   0 roman      (502) staff       (20)        0 2024-04-24 08:56:49.727286 redturtle.prenotazioni-2.6.5/src/redturtle/prenotazioni/browser/static/widget/js/
-drwxr-xr-x   0 roman      (502) staff       (20)        0 2024-04-24 08:56:49.727519 redturtle.prenotazioni-2.6.5/src/redturtle/prenotazioni/browser/static/widget/js/WidgetContainer/
--rw-r--r--   0 roman      (502) staff       (20)     5095 2024-04-24 08:56:49.000000 redturtle.prenotazioni-2.6.5/src/redturtle/prenotazioni/browser/static/widget/js/WidgetContainer/index.js
-drwxr-xr-x   0 roman      (502) staff       (20)        0 2024-04-24 08:56:49.728063 redturtle.prenotazioni-2.6.5/src/redturtle/prenotazioni/browser/static/widget/js/WidgetDataContainer/
--rw-r--r--   0 roman      (502) staff       (20)     4705 2024-04-24 08:56:49.000000 redturtle.prenotazioni-2.6.5/src/redturtle/prenotazioni/browser/static/widget/js/WidgetDataContainer/index.js
--rw-r--r--   0 roman      (502) staff       (20)     1059 2024-04-24 08:56:49.000000 redturtle.prenotazioni-2.6.5/src/redturtle/prenotazioni/browser/static/widget/js/WidgetDataContainer/index.less
-drwxr-xr-x   0 roman      (502) staff       (20)        0 2024-04-24 08:56:49.730380 redturtle.prenotazioni-2.6.5/src/redturtle/prenotazioni/browser/static/widget/js/fields/
--rw-r--r--   0 roman      (502) staff       (20)     3010 2024-04-24 08:56:49.000000 redturtle.prenotazioni-2.6.5/src/redturtle/prenotazioni/browser/static/widget/js/fields/DaysTableField.js
--rw-r--r--   0 roman      (502) staff       (20)      204 2024-04-24 08:56:49.000000 redturtle.prenotazioni-2.6.5/src/redturtle/prenotazioni/browser/static/widget/js/fields/DaysTableField.less
--rw-r--r--   0 roman      (502) staff       (20)     2874 2024-04-24 08:56:49.000000 redturtle.prenotazioni-2.6.5/src/redturtle/prenotazioni/browser/static/widget/js/fields/GatesField.js
--rw-r--r--   0 roman      (502) staff       (20)      401 2024-04-24 08:56:49.000000 redturtle.prenotazioni-2.6.5/src/redturtle/prenotazioni/browser/static/widget/js/fields/GatesField.less
--rw-r--r--   0 roman      (502) staff       (20)     1888 2024-04-24 08:56:49.000000 redturtle.prenotazioni-2.6.5/src/redturtle/prenotazioni/browser/static/widget/js/fields/IntervalSelectorField.js
--rw-r--r--   0 roman      (502) staff       (20)      314 2024-04-24 08:56:49.000000 redturtle.prenotazioni-2.6.5/src/redturtle/prenotazioni/browser/static/widget/js/fields/IntervalSelectorField.less
--rw-r--r--   0 roman      (502) staff       (20)     4187 2024-04-24 08:56:49.000000 redturtle.prenotazioni-2.6.5/src/redturtle/prenotazioni/browser/static/widget/js/fields/PauseTableField.js
--rw-r--r--   0 roman      (502) staff       (20)      337 2024-04-24 08:56:49.000000 redturtle.prenotazioni-2.6.5/src/redturtle/prenotazioni/browser/static/widget/js/fields/PauseTableField.less
--rw-r--r--   0 roman      (502) staff       (20)     1745 2024-04-24 08:56:49.000000 redturtle.prenotazioni-2.6.5/src/redturtle/prenotazioni/browser/static/widget/js/fields/SelectField.js
--rw-r--r--   0 roman      (502) staff       (20)      961 2024-04-24 08:56:49.000000 redturtle.prenotazioni-2.6.5/src/redturtle/prenotazioni/browser/static/widget/js/fields/TextLineField.js
--rw-r--r--   0 roman      (502) staff       (20)     1261 2024-04-24 08:56:49.000000 redturtle.prenotazioni-2.6.5/src/redturtle/prenotazioni/browser/static/widget/js/index.js
-drwxr-xr-x   0 roman      (502) staff       (20)        0 2024-04-24 08:56:49.730835 redturtle.prenotazioni-2.6.5/src/redturtle/prenotazioni/browser/static/widget/js/utils/
--rw-r--r--   0 roman      (502) staff       (20)      941 2024-04-24 08:56:49.000000 redturtle.prenotazioni-2.6.5/src/redturtle/prenotazioni/browser/static/widget/js/utils/i18n.js
--rw-r--r--   0 roman      (502) staff       (20)      298 2024-04-24 08:56:49.000000 redturtle.prenotazioni-2.6.5/src/redturtle/prenotazioni/browser/static/widget/js/utils/widgetContext.js
-drwxr-xr-x   0 roman      (502) staff       (20)        0 2024-04-24 08:56:49.731748 redturtle.prenotazioni-2.6.5/src/redturtle/prenotazioni/browser/stats/
--rw-r--r--   0 roman      (502) staff       (20)       24 2024-04-24 08:56:49.000000 redturtle.prenotazioni-2.6.5/src/redturtle/prenotazioni/browser/stats/__init__.py
--rw-r--r--   0 roman      (502) staff       (20)      698 2024-04-24 08:56:49.000000 redturtle.prenotazioni-2.6.5/src/redturtle/prenotazioni/browser/stats/booking_stats.pt
--rw-r--r--   0 roman      (502) staff       (20)     3863 2024-04-24 08:56:49.000000 redturtle.prenotazioni-2.6.5/src/redturtle/prenotazioni/browser/stats/booking_stats.py
--rw-r--r--   0 roman      (502) staff       (20)      575 2024-04-24 08:56:49.000000 redturtle.prenotazioni-2.6.5/src/redturtle/prenotazioni/browser/stats/configure.zcml
-drwxr-xr-x   0 roman      (502) staff       (20)        0 2024-04-24 08:56:49.734872 redturtle.prenotazioni-2.6.5/src/redturtle/prenotazioni/browser/templates/
--rw-r--r--   0 roman      (502) staff       (20)     2836 2024-04-24 08:56:49.000000 redturtle.prenotazioni-2.6.5/src/redturtle/prenotazioni/browser/templates/booking_type_radio_widget.pt
--rw-r--r--   0 roman      (502) staff       (20)     1518 2024-04-24 08:56:49.000000 redturtle.prenotazioni-2.6.5/src/redturtle/prenotazioni/browser/templates/custom_dgf_input.pt
--rw-r--r--   0 roman      (502) staff       (20)     4828 2024-04-24 08:56:49.000000 redturtle.prenotazioni-2.6.5/src/redturtle/prenotazioni/browser/templates/delete_reservation.pt
--rw-r--r--   0 roman      (502) staff       (20)     2417 2024-04-24 08:56:49.000000 redturtle.prenotazioni-2.6.5/src/redturtle/prenotazioni/browser/templates/manager_notification_mail.pt
--rw-r--r--   0 roman      (502) staff       (20)       48 2024-04-24 08:56:49.000000 redturtle.prenotazioni-2.6.5/src/redturtle/prenotazioni/browser/templates/nofollow.pt
--rw-r--r--   0 roman      (502) staff       (20)     7714 2024-04-24 08:56:49.000000 redturtle.prenotazioni-2.6.5/src/redturtle/prenotazioni/browser/templates/prenotazione.pt
--rw-r--r--   0 roman      (502) staff       (20)     9592 2024-04-24 08:56:49.000000 redturtle.prenotazioni-2.6.5/src/redturtle/prenotazioni/browser/templates/prenotazione_add.pt
--rw-r--r--   0 roman      (502) staff       (20)    16384 2024-04-24 08:56:49.000000 redturtle.prenotazioni-2.6.5/src/redturtle/prenotazioni/browser/templates/prenotazione_macros.pt
--rw-r--r--   0 roman      (502) staff       (20)     2227 2024-04-24 08:56:49.000000 redturtle.prenotazioni-2.6.5/src/redturtle/prenotazioni/browser/templates/prenotazione_move.pt
--rw-r--r--   0 roman      (502) staff       (20)     5299 2024-04-24 08:56:49.000000 redturtle.prenotazioni-2.6.5/src/redturtle/prenotazioni/browser/templates/prenotazione_print.pt
--rw-r--r--   0 roman      (502) staff       (20)     5241 2024-04-24 08:56:49.000000 redturtle.prenotazioni-2.6.5/src/redturtle/prenotazioni/browser/templates/prenotazioni_search.pt
--rw-r--r--   0 roman      (502) staff       (20)     1858 2024-04-24 08:56:49.000000 redturtle.prenotazioni-2.6.5/src/redturtle/prenotazioni/browser/templates/week.pt
--rw-r--r--   0 roman      (502) staff       (20)      362 2024-04-24 08:56:49.000000 redturtle.prenotazioni-2.6.5/src/redturtle/prenotazioni/browser/templates/week_table_overrides_widget_input.pt
-drwxr-xr-x   0 roman      (502) staff       (20)        0 2024-04-24 08:56:49.735499 redturtle.prenotazioni-2.6.5/src/redturtle/prenotazioni/browser/utilities/
--rw-r--r--   0 roman      (502) staff       (20)        0 2024-04-24 08:56:49.000000 redturtle.prenotazioni-2.6.5/src/redturtle/prenotazioni/browser/utilities/__init__.py
--rw-r--r--   0 roman      (502) staff       (20)      494 2024-04-24 08:56:49.000000 redturtle.prenotazioni-2.6.5/src/redturtle/prenotazioni/browser/utilities/configure.zcml
--rw-r--r--   0 roman      (502) staff       (20)     1873 2024-04-24 08:56:49.000000 redturtle.prenotazioni-2.6.5/src/redturtle/prenotazioni/browser/utilities/notify_upcoming_bookings.py
--rw-r--r--   0 roman      (502) staff       (20)     8087 2024-04-24 08:56:49.000000 redturtle.prenotazioni-2.6.5/src/redturtle/prenotazioni/browser/vacations.py
--rw-r--r--   0 roman      (502) staff       (20)     1524 2024-04-24 08:56:49.000000 redturtle.prenotazioni-2.6.5/src/redturtle/prenotazioni/browser/viewlets.py
--rw-r--r--   0 roman      (502) staff       (20)    10867 2024-04-24 08:56:49.000000 redturtle.prenotazioni-2.6.5/src/redturtle/prenotazioni/browser/week.py
--rw-r--r--   0 roman      (502) staff       (20)     1193 2024-04-24 08:56:49.000000 redturtle.prenotazioni-2.6.5/src/redturtle/prenotazioni/browser/widget.py
--rw-r--r--   0 roman      (502) staff       (20)     6310 2024-04-24 08:56:49.000000 redturtle.prenotazioni-2.6.5/src/redturtle/prenotazioni/browser/z3c_custom_widget.py
--rw-r--r--   0 roman      (502) staff       (20)      485 2024-04-24 08:56:49.000000 redturtle.prenotazioni-2.6.5/src/redturtle/prenotazioni/config.py
--rw-r--r--   0 roman      (502) staff       (20)     2049 2024-04-24 08:56:49.000000 redturtle.prenotazioni-2.6.5/src/redturtle/prenotazioni/configure.zcml
-drwxr-xr-x   0 roman      (502) staff       (20)        0 2024-04-24 08:56:49.737859 redturtle.prenotazioni-2.6.5/src/redturtle/prenotazioni/content/
--rw-r--r--   0 roman      (502) staff       (20)       24 2024-04-24 08:56:49.000000 redturtle.prenotazioni-2.6.5/src/redturtle/prenotazioni/content/__init__.py
--rw-r--r--   0 roman      (502) staff       (20)      111 2024-04-24 08:56:49.000000 redturtle.prenotazioni-2.6.5/src/redturtle/prenotazioni/content/booking_type.py
--rw-r--r--   0 roman      (502) staff       (20)     1537 2024-04-24 08:56:49.000000 redturtle.prenotazioni-2.6.5/src/redturtle/prenotazioni/content/pause.py
--rw-r--r--   0 roman      (502) staff       (20)     7504 2024-04-24 08:56:49.000000 redturtle.prenotazioni-2.6.5/src/redturtle/prenotazioni/content/prenotazione.py
--rw-r--r--   0 roman      (502) staff       (20)     1251 2024-04-24 08:56:49.000000 redturtle.prenotazioni-2.6.5/src/redturtle/prenotazioni/content/prenotazione_type.py
--rw-r--r--   0 roman      (502) staff       (20)      367 2024-04-24 08:56:49.000000 redturtle.prenotazioni-2.6.5/src/redturtle/prenotazioni/content/prenotazioni_day.py
--rw-r--r--   0 roman      (502) staff       (20)    19501 2024-04-24 08:56:49.000000 redturtle.prenotazioni-2.6.5/src/redturtle/prenotazioni/content/prenotazioni_folder.py
--rw-r--r--   0 roman      (502) staff       (20)      371 2024-04-24 08:56:49.000000 redturtle.prenotazioni-2.6.5/src/redturtle/prenotazioni/content/prenotazioni_week.py
--rw-r--r--   0 roman      (502) staff       (20)      371 2024-04-24 08:56:49.000000 redturtle.prenotazioni-2.6.5/src/redturtle/prenotazioni/content/prenotazioni_year.py
--rw-r--r--   0 roman      (502) staff       (20)     8518 2024-04-24 08:56:49.000000 redturtle.prenotazioni-2.6.5/src/redturtle/prenotazioni/content/validators.py
-drwxr-xr-x   0 roman      (502) staff       (20)        0 2024-04-24 08:56:49.739064 redturtle.prenotazioni-2.6.5/src/redturtle/prenotazioni/demo/
--rw-r--r--   0 roman      (502) staff       (20)       77 2024-04-24 08:56:49.000000 redturtle.prenotazioni-2.6.5/src/redturtle/prenotazioni/demo/__init__.py
--rw-r--r--   0 roman      (502) staff       (20)     1088 2024-04-24 08:56:49.000000 redturtle.prenotazioni-2.6.5/src/redturtle/prenotazioni/demo/configure.zcml
--rw-r--r--   0 roman      (502) staff       (20)      227 2024-04-24 08:56:49.000000 redturtle.prenotazioni-2.6.5/src/redturtle/prenotazioni/demo/interfaces.py
-drwxr-xr-x   0 roman      (502) staff       (20)        0 2024-04-24 08:56:49.697631 redturtle.prenotazioni-2.6.5/src/redturtle/prenotazioni/demo/profiles/
-drwxr-xr-x   0 roman      (502) staff       (20)        0 2024-04-24 08:56:49.739581 redturtle.prenotazioni-2.6.5/src/redturtle/prenotazioni/demo/profiles/default/
--rw-r--r--   0 roman      (502) staff       (20)      208 2024-04-24 08:56:49.000000 redturtle.prenotazioni-2.6.5/src/redturtle/prenotazioni/demo/profiles/default/browserlayer.xml
--rw-r--r--   0 roman      (502) staff       (20)       88 2024-04-24 08:56:49.000000 redturtle.prenotazioni-2.6.5/src/redturtle/prenotazioni/demo/profiles/default/metadata.xml
-drwxr-xr-x   0 roman      (502) staff       (20)        0 2024-04-24 08:56:49.739883 redturtle.prenotazioni-2.6.5/src/redturtle/prenotazioni/demo/profiles/uninstall/
--rw-r--r--   0 roman      (502) staff       (20)      133 2024-04-24 08:56:49.000000 redturtle.prenotazioni-2.6.5/src/redturtle/prenotazioni/demo/profiles/uninstall/browserlayer.xml
--rw-r--r--   0 roman      (502) staff       (20)      630 2024-04-24 08:56:49.000000 redturtle.prenotazioni-2.6.5/src/redturtle/prenotazioni/demo/setuphandlers.py
--rw-r--r--   0 roman      (502) staff       (20)     1347 2024-04-24 08:56:49.000000 redturtle.prenotazioni-2.6.5/src/redturtle/prenotazioni/demo/smsdemo.py
-drwxr-xr-x   0 roman      (502) staff       (20)        0 2024-04-24 08:56:49.741504 redturtle.prenotazioni-2.6.5/src/redturtle/prenotazioni/events/
--rw-r--r--   0 roman      (502) staff       (20)      270 2024-04-24 08:56:49.000000 redturtle.prenotazioni-2.6.5/src/redturtle/prenotazioni/events/__init__.py
--rw-r--r--   0 roman      (502) staff       (20)     1615 2024-04-24 08:56:49.000000 redturtle.prenotazioni-2.6.5/src/redturtle/prenotazioni/events/configure.zcml
--rw-r--r--   0 roman      (502) staff       (20)     2128 2024-04-24 08:56:49.000000 redturtle.prenotazioni-2.6.5/src/redturtle/prenotazioni/events/events_logger.py
--rw-r--r--   0 roman      (502) staff       (20)     1907 2024-04-24 08:56:49.000000 redturtle.prenotazioni-2.6.5/src/redturtle/prenotazioni/events/prenotazione.py
--rw-r--r--   0 roman      (502) staff       (20)     1189 2024-04-24 08:56:49.000000 redturtle.prenotazioni-2.6.5/src/redturtle/prenotazioni/events/prenotazioni_folder.py
-drwxr-xr-x   0 roman      (502) staff       (20)        0 2024-04-24 08:56:49.741970 redturtle.prenotazioni-2.6.5/src/redturtle/prenotazioni/exceptions/
--rw-r--r--   0 roman      (502) staff       (20)      129 2024-04-24 08:56:49.000000 redturtle.prenotazioni-2.6.5/src/redturtle/prenotazioni/exceptions/__init__.py
--rw-r--r--   0 roman      (502) staff       (20)      712 2024-04-24 08:56:49.000000 redturtle.prenotazioni-2.6.5/src/redturtle/prenotazioni/exceptions/booker.py
-drwxr-xr-x   0 roman      (502) staff       (20)        0 2024-04-24 08:56:49.742803 redturtle.prenotazioni-2.6.5/src/redturtle/prenotazioni/indexers/
--rw-r--r--   0 roman      (502) staff       (20)       24 2024-04-24 08:56:49.000000 redturtle.prenotazioni-2.6.5/src/redturtle/prenotazioni/indexers/__init__.py
--rw-r--r--   0 roman      (502) staff       (20)      476 2024-04-24 08:56:49.000000 redturtle.prenotazioni-2.6.5/src/redturtle/prenotazioni/indexers/configure.zcml
--rw-r--r--   0 roman      (502) staff       (20)     1410 2024-04-24 08:56:49.000000 redturtle.prenotazioni-2.6.5/src/redturtle/prenotazioni/indexers/prenotazione.py
--rw-r--r--   0 roman      (502) staff       (20)     1445 2024-04-24 08:56:49.000000 redturtle.prenotazioni-2.6.5/src/redturtle/prenotazioni/interfaces.py
-drwxr-xr-x   0 roman      (502) staff       (20)        0 2024-04-24 08:56:49.745361 redturtle.prenotazioni-2.6.5/src/redturtle/prenotazioni/io_tools/
--rw-r--r--   0 roman      (502) staff       (20)     5302 2024-04-24 08:56:49.000000 redturtle.prenotazioni-2.6.5/src/redturtle/prenotazioni/io_tools/README.md
--rw-r--r--   0 roman      (502) staff       (20)      207 2024-04-24 08:56:49.000000 redturtle.prenotazioni-2.6.5/src/redturtle/prenotazioni/io_tools/__init__.py
--rw-r--r--   0 roman      (502) staff       (20)     9443 2024-04-24 08:56:49.000000 redturtle.prenotazioni-2.6.5/src/redturtle/prenotazioni/io_tools/api.py
--rw-r--r--   0 roman      (502) staff       (20)     1035 2024-04-24 08:56:49.000000 redturtle.prenotazioni-2.6.5/src/redturtle/prenotazioni/io_tools/cli.py
--rw-r--r--   0 roman      (502) staff       (20)    16384 2024-04-24 08:56:49.000000 redturtle.prenotazioni-2.6.5/src/redturtle/prenotazioni/io_tools/io.db
--rw-r--r--   0 roman      (502) staff       (20)       45 2024-04-24 08:56:49.000000 redturtle.prenotazioni-2.6.5/src/redturtle/prenotazioni/io_tools/io_tools.py
--rw-r--r--   0 roman      (502) staff       (20)     1945 2024-04-24 08:56:49.000000 redturtle.prenotazioni-2.6.5/src/redturtle/prenotazioni/io_tools/monkey.py
--rw-r--r--   0 roman      (502) staff       (20)     2833 2024-04-24 08:56:49.000000 redturtle.prenotazioni-2.6.5/src/redturtle/prenotazioni/io_tools/rdbms.py
--rw-r--r--   0 roman      (502) staff       (20)    27521 2024-04-24 08:56:49.000000 redturtle.prenotazioni-2.6.5/src/redturtle/prenotazioni/io_tools/spec.yaml
--rw-r--r--   0 roman      (502) staff       (20)      961 2024-04-24 08:56:49.000000 redturtle.prenotazioni-2.6.5/src/redturtle/prenotazioni/io_tools/storage.py
-drwxr-xr-x   0 roman      (502) staff       (20)        0 2024-04-24 08:56:49.746348 redturtle.prenotazioni-2.6.5/src/redturtle/prenotazioni/locales/
-drwxr-xr-x   0 roman      (502) staff       (20)        0 2024-04-24 08:56:49.698444 redturtle.prenotazioni-2.6.5/src/redturtle/prenotazioni/locales/en/
-drwxr-xr-x   0 roman      (502) staff       (20)        0 2024-04-24 08:56:49.746573 redturtle.prenotazioni-2.6.5/src/redturtle/prenotazioni/locales/en/LC_MESSAGES/
--rw-r--r--   0 roman      (502) staff       (20)    56804 2024-04-24 08:56:49.000000 redturtle.prenotazioni-2.6.5/src/redturtle/prenotazioni/locales/en/LC_MESSAGES/redturtle.prenotazioni.po
-drwxr-xr-x   0 roman      (502) staff       (20)        0 2024-04-24 08:56:49.698648 redturtle.prenotazioni-2.6.5/src/redturtle/prenotazioni/locales/it/
-drwxr-xr-x   0 roman      (502) staff       (20)        0 2024-04-24 08:56:49.747233 redturtle.prenotazioni-2.6.5/src/redturtle/prenotazioni/locales/it/LC_MESSAGES/
--rw-r--r--   0 roman      (502) staff       (20)      623 2024-04-24 08:56:49.000000 redturtle.prenotazioni-2.6.5/src/redturtle/prenotazioni/locales/it/LC_MESSAGES/plone.po
--rw-r--r--   0 roman      (502) staff       (20)    73449 2024-04-24 08:56:49.000000 redturtle.prenotazioni-2.6.5/src/redturtle/prenotazioni/locales/it/LC_MESSAGES/redturtle.prenotazioni.po
--rw-r--r--   0 roman      (502) staff       (20)      830 2024-04-24 08:56:49.000000 redturtle.prenotazioni-2.6.5/src/redturtle/prenotazioni/locales/manual.pot
--rw-r--r--   0 roman      (502) staff       (20)    56913 2024-04-24 08:56:49.000000 redturtle.prenotazioni-2.6.5/src/redturtle/prenotazioni/locales/redturtle.prenotazioni.pot
--rw-r--r--   0 roman      (502) staff       (20)     1618 2024-04-24 08:56:49.000000 redturtle.prenotazioni-2.6.5/src/redturtle/prenotazioni/locales/update.py
--rwxr-xr-x   0 roman      (502) staff       (20)      521 2024-04-24 08:56:49.000000 redturtle.prenotazioni-2.6.5/src/redturtle/prenotazioni/locales/update.sh
-drwxr-xr-x   0 roman      (502) staff       (20)        0 2024-04-24 08:56:49.747725 redturtle.prenotazioni-2.6.5/src/redturtle/prenotazioni/monkeypatcher/
--rw-r--r--   0 roman      (502) staff       (20)        0 2024-04-24 08:56:49.000000 redturtle.prenotazioni-2.6.5/src/redturtle/prenotazioni/monkeypatcher/__init__.py
--rw-r--r--   0 roman      (502) staff       (20)      499 2024-04-24 08:56:49.000000 redturtle.prenotazioni-2.6.5/src/redturtle/prenotazioni/monkeypatcher/configure.zcml
--rw-r--r--   0 roman      (502) staff       (20)     1565 2024-04-24 08:56:49.000000 redturtle.prenotazioni-2.6.5/src/redturtle/prenotazioni/permissions.zcml
--rw-r--r--   0 roman      (502) staff       (20)      507 2024-04-24 08:56:49.000000 redturtle.prenotazioni-2.6.5/src/redturtle/prenotazioni/prenotazione_event.py
-drwxr-xr-x   0 roman      (502) staff       (20)        0 2024-04-24 08:56:49.700384 redturtle.prenotazioni-2.6.5/src/redturtle/prenotazioni/profiles/
-drwxr-xr-x   0 roman      (502) staff       (20)        0 2024-04-24 08:56:49.749920 redturtle.prenotazioni-2.6.5/src/redturtle/prenotazioni/profiles/default/
--rw-r--r--   0 roman      (502) staff       (20)     2656 2024-04-24 08:56:49.000000 redturtle.prenotazioni-2.6.5/src/redturtle/prenotazioni/profiles/default/actions.xml
--rw-r--r--   0 roman      (502) staff       (20)      185 2024-04-24 08:56:49.000000 redturtle.prenotazioni-2.6.5/src/redturtle/prenotazioni/profiles/default/browserlayer.xml
--rw-r--r--   0 roman      (502) staff       (20)      349 2024-04-24 08:56:49.000000 redturtle.prenotazioni-2.6.5/src/redturtle/prenotazioni/profiles/default/catalog.xml
--rw-r--r--   0 roman      (502) staff       (20)       71 2024-04-24 08:56:49.000000 redturtle.prenotazioni-2.6.5/src/redturtle/prenotazioni/profiles/default/contentrules.xml
--rw-r--r--   0 roman      (502) staff       (20)      325 2024-04-24 08:56:49.000000 redturtle.prenotazioni-2.6.5/src/redturtle/prenotazioni/profiles/default/metadata.xml
-drwxr-xr-x   0 roman      (502) staff       (20)        0 2024-04-24 08:56:49.750642 redturtle.prenotazioni-2.6.5/src/redturtle/prenotazioni/profiles/default/registry/
--rw-r--r--   0 roman      (502) staff       (20)     5140 2024-04-24 08:56:49.000000 redturtle.prenotazioni-2.6.5/src/redturtle/prenotazioni/profiles/default/registry/caching.xml
--rw-r--r--   0 roman      (502) staff       (20)     2015 2024-04-24 08:56:49.000000 redturtle.prenotazioni-2.6.5/src/redturtle/prenotazioni/profiles/default/registry/resources.xml
--rw-r--r--   0 roman      (502) staff       (20)     1001 2024-04-24 08:56:49.000000 redturtle.prenotazioni-2.6.5/src/redturtle/prenotazioni/profiles/default/registry/settings.xml
--rw-r--r--   0 roman      (502) staff       (20)     3277 2024-04-24 08:56:49.000000 redturtle.prenotazioni-2.6.5/src/redturtle/prenotazioni/profiles/default/rolemap.xml
--rw-r--r--   0 roman      (502) staff       (20)      277 2024-04-24 08:56:49.000000 redturtle.prenotazioni-2.6.5/src/redturtle/prenotazioni/profiles/default/sharing.xml
-drwxr-xr-x   0 roman      (502) staff       (20)        0 2024-04-24 08:56:49.752083 redturtle.prenotazioni-2.6.5/src/redturtle/prenotazioni/profiles/default/types/
--rw-r--r--   0 roman      (502) staff       (20)     3607 2024-04-24 08:56:49.000000 redturtle.prenotazioni-2.6.5/src/redturtle/prenotazioni/profiles/default/types/Prenotazione.xml
--rw-r--r--   0 roman      (502) staff       (20)     2983 2024-04-24 08:56:49.000000 redturtle.prenotazioni-2.6.5/src/redturtle/prenotazioni/profiles/default/types/PrenotazioneType.xml
--rw-r--r--   0 roman      (502) staff       (20)     3861 2024-04-24 08:56:49.000000 redturtle.prenotazioni-2.6.5/src/redturtle/prenotazioni/profiles/default/types/PrenotazioniDay.xml
--rw-r--r--   0 roman      (502) staff       (20)     3257 2024-04-24 08:56:49.000000 redturtle.prenotazioni-2.6.5/src/redturtle/prenotazioni/profiles/default/types/PrenotazioniFolder.xml
--rw-r--r--   0 roman      (502) staff       (20)     3845 2024-04-24 08:56:49.000000 redturtle.prenotazioni-2.6.5/src/redturtle/prenotazioni/profiles/default/types/PrenotazioniWeek.xml
--rw-r--r--   0 roman      (502) staff       (20)     3846 2024-04-24 08:56:49.000000 redturtle.prenotazioni-2.6.5/src/redturtle/prenotazioni/profiles/default/types/PrenotazioniYear.xml
--rw-r--r--   0 roman      (502) staff       (20)      713 2024-04-24 08:56:49.000000 redturtle.prenotazioni-2.6.5/src/redturtle/prenotazioni/profiles/default/types.xml
-drwxr-xr-x   0 roman      (502) staff       (20)        0 2024-04-24 08:56:49.699561 redturtle.prenotazioni-2.6.5/src/redturtle/prenotazioni/profiles/default/workflows/
-drwxr-xr-x   0 roman      (502) staff       (20)        0 2024-04-24 08:56:49.752307 redturtle.prenotazioni-2.6.5/src/redturtle/prenotazioni/profiles/default/workflows/prenotazioni_workflow/
--rw-r--r--   0 roman      (502) staff       (20)    12711 2024-04-24 08:56:49.000000 redturtle.prenotazioni-2.6.5/src/redturtle/prenotazioni/profiles/default/workflows/prenotazioni_workflow/definition.xml
-drwxr-xr-x   0 roman      (502) staff       (20)        0 2024-04-24 08:56:49.752612 redturtle.prenotazioni-2.6.5/src/redturtle/prenotazioni/profiles/default/workflows/prenotazionifolder_workflow/
--rw-r--r--   0 roman      (502) staff       (20)     8877 2024-04-24 08:56:49.000000 redturtle.prenotazioni-2.6.5/src/redturtle/prenotazioni/profiles/default/workflows/prenotazionifolder_workflow/definition.xml
--rw-r--r--   0 roman      (502) staff       (20)      613 2024-04-24 08:56:49.000000 redturtle.prenotazioni-2.6.5/src/redturtle/prenotazioni/profiles/default/workflows.xml
-drwxr-xr-x   0 roman      (502) staff       (20)        0 2024-04-24 08:56:49.752842 redturtle.prenotazioni-2.6.5/src/redturtle/prenotazioni/profiles/to_1402/
--rw-r--r--   0 roman      (502) staff       (20)     1508 2024-04-24 08:56:49.000000 redturtle.prenotazioni-2.6.5/src/redturtle/prenotazioni/profiles/to_1402/contentrules.xml
-drwxr-xr-x   0 roman      (502) staff       (20)        0 2024-04-24 08:56:49.753067 redturtle.prenotazioni-2.6.5/src/redturtle/prenotazioni/profiles/to_1500/
--rw-r--r--   0 roman      (502) staff       (20)      226 2024-04-24 08:56:49.000000 redturtle.prenotazioni-2.6.5/src/redturtle/prenotazioni/profiles/to_1500/types.xml
-drwxr-xr-x   0 roman      (502) staff       (20)        0 2024-04-24 08:56:49.753590 redturtle.prenotazioni-2.6.5/src/redturtle/prenotazioni/profiles/to_2005/
--rw-r--r--   0 roman      (502) staff       (20)       88 2024-04-24 08:56:49.000000 redturtle.prenotazioni-2.6.5/src/redturtle/prenotazioni/profiles/to_2005/metadata.xml
--rw-r--r--   0 roman      (502) staff       (20)      638 2024-04-24 08:56:49.000000 redturtle.prenotazioni-2.6.5/src/redturtle/prenotazioni/profiles/to_2005/rolemap.xml
-drwxr-xr-x   0 roman      (502) staff       (20)        0 2024-04-24 08:56:49.754089 redturtle.prenotazioni-2.6.5/src/redturtle/prenotazioni/profiles/to_2006/
--rw-r--r--   0 roman      (502) staff       (20)       88 2024-04-24 08:56:49.000000 redturtle.prenotazioni-2.6.5/src/redturtle/prenotazioni/profiles/to_2006/metadata.xml
-drwxr-xr-x   0 roman      (502) staff       (20)        0 2024-04-24 08:56:49.700265 redturtle.prenotazioni-2.6.5/src/redturtle/prenotazioni/profiles/to_2006/workflows/
-drwxr-xr-x   0 roman      (502) staff       (20)        0 2024-04-24 08:56:49.754325 redturtle.prenotazioni-2.6.5/src/redturtle/prenotazioni/profiles/to_2006/workflows/prenotazioni_workflow/
--rw-r--r--   0 roman      (502) staff       (20)    12711 2024-04-24 08:56:49.000000 redturtle.prenotazioni-2.6.5/src/redturtle/prenotazioni/profiles/to_2006/workflows/prenotazioni_workflow/definition.xml
--rw-r--r--   0 roman      (502) staff       (20)      279 2024-04-24 08:56:49.000000 redturtle.prenotazioni-2.6.5/src/redturtle/prenotazioni/profiles/to_2006/workflows.xml
-drwxr-xr-x   0 roman      (502) staff       (20)        0 2024-04-24 08:56:49.754569 redturtle.prenotazioni-2.6.5/src/redturtle/prenotazioni/profiles/uninstall/
--rw-r--r--   0 roman      (502) staff       (20)      125 2024-04-24 08:56:49.000000 redturtle.prenotazioni-2.6.5/src/redturtle/prenotazioni/profiles/uninstall/browserlayer.xml
-drwxr-xr-x   0 roman      (502) staff       (20)        0 2024-04-24 08:56:49.755083 redturtle.prenotazioni-2.6.5/src/redturtle/prenotazioni/profiles/uninstall/registry/
--rw-r--r--   0 roman      (502) staff       (20)      431 2024-04-24 08:56:49.000000 redturtle.prenotazioni-2.6.5/src/redturtle/prenotazioni/profiles/uninstall/registry/resources.xml
--rw-r--r--   0 roman      (502) staff       (20)      152 2024-04-24 08:56:49.000000 redturtle.prenotazioni-2.6.5/src/redturtle/prenotazioni/profiles/uninstall/registry/settings.xml
-drwxr-xr-x   0 roman      (502) staff       (20)        0 2024-04-24 08:56:49.755478 redturtle.prenotazioni-2.6.5/src/redturtle/prenotazioni/restapi/
--rw-r--r--   0 roman      (502) staff       (20)        0 2024-04-24 08:56:49.000000 redturtle.prenotazioni-2.6.5/src/redturtle/prenotazioni/restapi/__init__.py
--rw-r--r--   0 roman      (502) staff       (20)      199 2024-04-24 08:56:49.000000 redturtle.prenotazioni-2.6.5/src/redturtle/prenotazioni/restapi/configure.zcml
-drwxr-xr-x   0 roman      (502) staff       (20)        0 2024-04-24 08:56:49.756112 redturtle.prenotazioni-2.6.5/src/redturtle/prenotazioni/restapi/serializers/
--rw-r--r--   0 roman      (502) staff       (20)        0 2024-04-24 08:56:49.000000 redturtle.prenotazioni-2.6.5/src/redturtle/prenotazioni/restapi/serializers/__init__.py
-drwxr-xr-x   0 roman      (502) staff       (20)        0 2024-04-24 08:56:49.757556 redturtle.prenotazioni-2.6.5/src/redturtle/prenotazioni/restapi/serializers/adapters/
--rw-r--r--   0 roman      (502) staff       (20)        0 2024-04-24 08:56:49.000000 redturtle.prenotazioni-2.6.5/src/redturtle/prenotazioni/restapi/serializers/adapters/__init__.py
--rw-r--r--   0 roman      (502) staff       (20)      468 2024-04-24 08:56:49.000000 redturtle.prenotazioni-2.6.5/src/redturtle/prenotazioni/restapi/serializers/adapters/configure.zcml
--rw-r--r--   0 roman      (502) staff       (20)     7441 2024-04-24 08:56:49.000000 redturtle.prenotazioni-2.6.5/src/redturtle/prenotazioni/restapi/serializers/adapters/prenotazione.py
--rw-r--r--   0 roman      (502) staff       (20)      973 2024-04-24 08:56:49.000000 redturtle.prenotazioni-2.6.5/src/redturtle/prenotazioni/restapi/serializers/adapters/prenotazione_type.py
--rw-r--r--   0 roman      (502) staff       (20)      925 2024-04-24 08:56:49.000000 redturtle.prenotazioni-2.6.5/src/redturtle/prenotazioni/restapi/serializers/adapters/prenotazioni_folder.py
--rw-r--r--   0 roman      (502) staff       (20)     1721 2024-04-24 08:56:49.000000 redturtle.prenotazioni-2.6.5/src/redturtle/prenotazioni/restapi/serializers/adapters/slot.py
--rw-r--r--   0 roman      (502) staff       (20)      162 2024-04-24 08:56:49.000000 redturtle.prenotazioni-2.6.5/src/redturtle/prenotazioni/restapi/serializers/configure.zcml
-drwxr-xr-x   0 roman      (502) staff       (20)        0 2024-04-24 08:56:49.757781 redturtle.prenotazioni-2.6.5/src/redturtle/prenotazioni/restapi/services/
-drwxr-xr-x   0 roman      (502) staff       (20)        0 2024-04-24 08:56:49.758457 redturtle.prenotazioni-2.6.5/src/redturtle/prenotazioni/restapi/services/available_slots/
--rw-r--r--   0 roman      (502) staff       (20)        0 2024-04-24 08:56:49.000000 redturtle.prenotazioni-2.6.5/src/redturtle/prenotazioni/restapi/services/available_slots/__init__.py
--rw-r--r--   0 roman      (502) staff       (20)      352 2024-04-24 08:56:49.000000 redturtle.prenotazioni-2.6.5/src/redturtle/prenotazioni/restapi/services/available_slots/configure.zcml
--rw-r--r--   0 roman      (502) staff       (20)     3736 2024-04-24 08:56:49.000000 redturtle.prenotazioni-2.6.5/src/redturtle/prenotazioni/restapi/services/available_slots/get.py
-drwxr-xr-x   0 roman      (502) staff       (20)        0 2024-04-24 08:56:49.760277 redturtle.prenotazioni-2.6.5/src/redturtle/prenotazioni/restapi/services/booking/
--rw-r--r--   0 roman      (502) staff       (20)        0 2024-04-24 08:56:49.000000 redturtle.prenotazioni-2.6.5/src/redturtle/prenotazioni/restapi/services/booking/__init__.py
--rw-r--r--   0 roman      (502) staff       (20)     6595 2024-04-24 08:56:49.000000 redturtle.prenotazioni-2.6.5/src/redturtle/prenotazioni/restapi/services/booking/add.py
--rw-r--r--   0 roman      (502) staff       (20)     1641 2024-04-24 08:56:49.000000 redturtle.prenotazioni-2.6.5/src/redturtle/prenotazioni/restapi/services/booking/configure.zcml
--rw-r--r--   0 roman      (502) staff       (20)     1209 2024-04-24 08:56:49.000000 redturtle.prenotazioni-2.6.5/src/redturtle/prenotazioni/restapi/services/booking/delete.py
--rw-r--r--   0 roman      (502) staff       (20)     1166 2024-04-24 08:56:49.000000 redturtle.prenotazioni-2.6.5/src/redturtle/prenotazioni/restapi/services/booking/get.py
--rw-r--r--   0 roman      (502) staff       (20)     1328 2024-04-24 08:56:49.000000 redturtle.prenotazioni-2.6.5/src/redturtle/prenotazioni/restapi/services/booking/move.py
--rw-r--r--   0 roman      (502) staff       (20)     1152 2024-04-24 08:56:49.000000 redturtle.prenotazioni-2.6.5/src/redturtle/prenotazioni/restapi/services/booking/notify_about_confirm.py
--rw-r--r--   0 roman      (502) staff       (20)      966 2024-04-24 08:56:49.000000 redturtle.prenotazioni-2.6.5/src/redturtle/prenotazioni/restapi/services/booking/vacation.py
-drwxr-xr-x   0 roman      (502) staff       (20)        0 2024-04-24 08:56:49.760899 redturtle.prenotazioni-2.6.5/src/redturtle/prenotazioni/restapi/services/booking_schema/
--rw-r--r--   0 roman      (502) staff       (20)        0 2024-04-24 08:56:49.000000 redturtle.prenotazioni-2.6.5/src/redturtle/prenotazioni/restapi/services/booking_schema/__init__.py
--rw-r--r--   0 roman      (502) staff       (20)      404 2024-04-24 08:56:49.000000 redturtle.prenotazioni-2.6.5/src/redturtle/prenotazioni/restapi/services/booking_schema/configure.zcml
--rw-r--r--   0 roman      (502) staff       (20)     5243 2024-04-24 08:56:49.000000 redturtle.prenotazioni-2.6.5/src/redturtle/prenotazioni/restapi/services/booking_schema/get.py
-drwxr-xr-x   0 roman      (502) staff       (20)        0 2024-04-24 08:56:49.761570 redturtle.prenotazioni-2.6.5/src/redturtle/prenotazioni/restapi/services/bookings/
--rw-r--r--   0 roman      (502) staff       (20)        0 2024-04-24 08:56:49.000000 redturtle.prenotazioni-2.6.5/src/redturtle/prenotazioni/restapi/services/bookings/__init__.py
--rw-r--r--   0 roman      (502) staff       (20)      548 2024-04-24 08:56:49.000000 redturtle.prenotazioni-2.6.5/src/redturtle/prenotazioni/restapi/services/bookings/configure.zcml
--rw-r--r--   0 roman      (502) staff       (20)     3898 2024-04-24 08:56:49.000000 redturtle.prenotazioni-2.6.5/src/redturtle/prenotazioni/restapi/services/bookings/search.py
--rw-r--r--   0 roman      (502) staff       (20)      336 2024-04-24 08:56:49.000000 redturtle.prenotazioni-2.6.5/src/redturtle/prenotazioni/restapi/services/configure.zcml
-drwxr-xr-x   0 roman      (502) staff       (20)        0 2024-04-24 08:56:49.762186 redturtle.prenotazioni-2.6.5/src/redturtle/prenotazioni/restapi/services/day/
--rw-r--r--   0 roman      (502) staff       (20)        0 2024-04-24 08:56:49.000000 redturtle.prenotazioni-2.6.5/src/redturtle/prenotazioni/restapi/services/day/__init__.py
--rw-r--r--   0 roman      (502) staff       (20)      365 2024-04-24 08:56:49.000000 redturtle.prenotazioni-2.6.5/src/redturtle/prenotazioni/restapi/services/day/configure.zcml
--rw-r--r--   0 roman      (502) staff       (20)     6732 2024-04-24 08:56:49.000000 redturtle.prenotazioni-2.6.5/src/redturtle/prenotazioni/restapi/services/day/day.py
-drwxr-xr-x   0 roman      (502) staff       (20)        0 2024-04-24 08:56:49.762840 redturtle.prenotazioni-2.6.5/src/redturtle/prenotazioni/restapi/services/types/
--rw-r--r--   0 roman      (502) staff       (20)        0 2024-04-24 08:56:49.000000 redturtle.prenotazioni-2.6.5/src/redturtle/prenotazioni/restapi/services/types/__init__.py
--rw-r--r--   0 roman      (502) staff       (20)      216 2024-04-24 08:56:49.000000 redturtle.prenotazioni-2.6.5/src/redturtle/prenotazioni/restapi/services/types/configure.zcml
--rw-r--r--   0 roman      (502) staff       (20)      915 2024-04-24 08:56:49.000000 redturtle.prenotazioni-2.6.5/src/redturtle/prenotazioni/restapi/services/types/get.py
-drwxr-xr-x   0 roman      (502) staff       (20)        0 2024-04-24 08:56:49.763239 redturtle.prenotazioni-2.6.5/src/redturtle/prenotazioni/scripts/
--rw-r--r--   0 roman      (502) staff       (20)        0 2024-04-24 08:56:49.000000 redturtle.prenotazioni-2.6.5/src/redturtle/prenotazioni/scripts/__init__.py
--rw-r--r--   0 roman      (502) staff       (20)      525 2024-04-24 08:56:49.000000 redturtle.prenotazioni-2.6.5/src/redturtle/prenotazioni/scripts/notify_upcoming_bookings.py
--rw-r--r--   0 roman      (502) staff       (20)     1062 2024-04-24 08:56:49.000000 redturtle.prenotazioni-2.6.5/src/redturtle/prenotazioni/setuphandlers.py
--rw-r--r--   0 roman      (502) staff       (20)     3443 2024-04-24 08:56:49.000000 redturtle.prenotazioni-2.6.5/src/redturtle/prenotazioni/testing.py
-drwxr-xr-x   0 roman      (502) staff       (20)        0 2024-04-24 08:56:49.772025 redturtle.prenotazioni-2.6.5/src/redturtle/prenotazioni/tests/
--rw-r--r--   0 roman      (502) staff       (20)      105 2024-04-24 08:56:49.000000 redturtle.prenotazioni-2.6.5/src/redturtle/prenotazioni/tests/__init__.py
--rw-r--r--   0 roman      (502) staff       (20)     1223 2024-04-24 08:56:49.000000 redturtle.prenotazioni-2.6.5/src/redturtle/prenotazioni/tests/helpers.py
--rw-r--r--   0 roman      (502) staff       (20)     3222 2024-04-24 08:56:49.000000 redturtle.prenotazioni-2.6.5/src/redturtle/prenotazioni/tests/test_add_block.py
--rw-r--r--   0 roman      (502) staff       (20)    25000 2024-04-24 08:56:49.000000 redturtle.prenotazioni-2.6.5/src/redturtle/prenotazioni/tests/test_add_booking.py
--rw-r--r--   0 roman      (502) staff       (20)     1980 2024-04-24 08:56:49.000000 redturtle.prenotazioni-2.6.5/src/redturtle/prenotazioni/tests/test_add_booking_type.py
--rw-r--r--   0 roman      (502) staff       (20)    17450 2024-04-24 08:56:49.000000 redturtle.prenotazioni-2.6.5/src/redturtle/prenotazioni/tests/test_available_slots.py
--rw-r--r--   0 roman      (502) staff       (20)     2011 2024-04-24 08:56:49.000000 redturtle.prenotazioni-2.6.5/src/redturtle/prenotazioni/tests/test_base_slot.py
--rw-r--r--   0 roman      (502) staff       (20)     4387 2024-04-24 08:56:49.000000 redturtle.prenotazioni-2.6.5/src/redturtle/prenotazioni/tests/test_booker_choose_available_slot.py
--rw-r--r--   0 roman      (502) staff       (20)     6402 2024-04-24 08:56:49.000000 redturtle.prenotazioni-2.6.5/src/redturtle/prenotazioni/tests/test_booking_info.py
--rw-r--r--   0 roman      (502) staff       (20)     6901 2024-04-24 08:56:49.000000 redturtle.prenotazioni-2.6.5/src/redturtle/prenotazioni/tests/test_booking_notify.py
--rw-r--r--   0 roman      (502) staff       (20)     8748 2024-04-24 08:56:49.000000 redturtle.prenotazioni-2.6.5/src/redturtle/prenotazioni/tests/test_booking_schema.py
--rw-r--r--   0 roman      (502) staff       (20)     8696 2024-04-24 08:56:49.000000 redturtle.prenotazioni-2.6.5/src/redturtle/prenotazioni/tests/test_bookings_num_limit.py
--rw-r--r--   0 roman      (502) staff       (20)     5952 2024-04-24 08:56:49.000000 redturtle.prenotazioni-2.6.5/src/redturtle/prenotazioni/tests/test_browser_utilities_notify_upcoming_bookings.py
--rw-r--r--   0 roman      (502) staff       (20)     3088 2024-04-24 08:56:49.000000 redturtle.prenotazioni-2.6.5/src/redturtle/prenotazioni/tests/test_content_validators_validate_pause_table.py
--rw-r--r--   0 roman      (502) staff       (20)     6317 2024-04-24 08:56:49.000000 redturtle.prenotazioni-2.6.5/src/redturtle/prenotazioni/tests/test_day.py
--rw-r--r--   0 roman      (502) staff       (20)    10871 2024-04-24 08:56:49.000000 redturtle.prenotazioni-2.6.5/src/redturtle/prenotazioni/tests/test_delete_booking.py
--rw-r--r--   0 roman      (502) staff       (20)    10361 2024-04-24 08:56:49.000000 redturtle.prenotazioni-2.6.5/src/redturtle/prenotazioni/tests/test_delete_booking_api.py
--rw-r--r--   0 roman      (502) staff       (20)     4000 2024-04-24 08:56:49.000000 redturtle.prenotazioni-2.6.5/src/redturtle/prenotazioni/tests/test_gates_overrides.py
--rw-r--r--   0 roman      (502) staff       (20)     8160 2024-04-24 08:56:49.000000 redturtle.prenotazioni-2.6.5/src/redturtle/prenotazioni/tests/test_move_booking_api.py
--rw-r--r--   0 roman      (502) staff       (20)     5216 2024-04-24 08:56:49.000000 redturtle.prenotazioni-2.6.5/src/redturtle/prenotazioni/tests/test_notification_supervisor_utility.py
--rw-r--r--   0 roman      (502) staff       (20)    14545 2024-04-24 08:56:49.000000 redturtle.prenotazioni-2.6.5/src/redturtle/prenotazioni/tests/test_pauses_overrides.py
--rw-r--r--   0 roman      (502) staff       (20)     5029 2024-04-24 08:56:49.000000 redturtle.prenotazioni-2.6.5/src/redturtle/prenotazioni/tests/test_prenotazione_email_sent_to_managers.py
--rw-r--r--   0 roman      (502) staff       (20)    15081 2024-04-24 08:56:49.000000 redturtle.prenotazioni-2.6.5/src/redturtle/prenotazioni/tests/test_prenotazione_events.py
--rw-r--r--   0 roman      (502) staff       (20)     4861 2024-04-24 08:56:49.000000 redturtle.prenotazioni-2.6.5/src/redturtle/prenotazioni/tests/test_prenotazione_searchable_item_serializer.py
--rw-r--r--   0 roman      (502) staff       (20)     7049 2024-04-24 08:56:49.000000 redturtle.prenotazioni-2.6.5/src/redturtle/prenotazioni/tests/test_prenotazioni_context_state.py
--rw-r--r--   0 roman      (502) staff       (20)      740 2024-04-24 08:56:49.000000 redturtle.prenotazioni-2.6.5/src/redturtle/prenotazioni/tests/test_prenotazioni_folder_holidays_constraint.py
--rw-r--r--   0 roman      (502) staff       (20)    19833 2024-04-24 08:56:49.000000 redturtle.prenotazioni-2.6.5/src/redturtle/prenotazioni/tests/test_prenotazioni_search.py
--rw-r--r--   0 roman      (502) staff       (20)     2485 2024-04-24 08:56:49.000000 redturtle.prenotazioni-2.6.5/src/redturtle/prenotazioni/tests/test_restapi_types_override.py
--rw-r--r--   0 roman      (502) staff       (20)     9722 2024-04-24 08:56:49.000000 redturtle.prenotazioni-2.6.5/src/redturtle/prenotazioni/tests/test_send_ical.py
--rw-r--r--   0 roman      (502) staff       (20)     4180 2024-04-24 08:56:49.000000 redturtle.prenotazioni-2.6.5/src/redturtle/prenotazioni/tests/test_setup.py
--rw-r--r--   0 roman      (502) staff       (20)     3046 2024-04-24 08:56:49.000000 redturtle.prenotazioni-2.6.5/src/redturtle/prenotazioni/tests/test_stringinterp.py
--rw-r--r--   0 roman      (502) staff       (20)      905 2024-04-24 08:56:49.000000 redturtle.prenotazioni-2.6.5/src/redturtle/prenotazioni/tests/test_utils.py
--rw-r--r--   0 roman      (502) staff       (20)     6486 2024-04-24 08:56:49.000000 redturtle.prenotazioni-2.6.5/src/redturtle/prenotazioni/tests/test_vacation_api.py
--rw-r--r--   0 roman      (502) staff       (20)     1198 2024-04-24 08:56:49.000000 redturtle.prenotazioni-2.6.5/src/redturtle/prenotazioni/tests/test_validate_max_bookings_allowed.py
--rw-r--r--   0 roman      (502) staff       (20)     2349 2024-04-24 08:56:49.000000 redturtle.prenotazioni-2.6.5/src/redturtle/prenotazioni/tests/test_vocabularies.py
--rw-r--r--   0 roman      (502) staff       (20)    23517 2024-04-24 08:56:49.000000 redturtle.prenotazioni-2.6.5/src/redturtle/prenotazioni/tests/test_week_table_overrides.py
--rw-r--r--   0 roman      (502) staff       (20)    16547 2024-04-24 08:56:49.000000 redturtle.prenotazioni-2.6.5/src/redturtle/prenotazioni/upgrades.py
--rw-r--r--   0 roman      (502) staff       (20)    10360 2024-04-24 08:56:49.000000 redturtle.prenotazioni-2.6.5/src/redturtle/prenotazioni/upgrades.zcml
-drwxr-xr-x   0 roman      (502) staff       (20)        0 2024-04-24 08:56:49.773286 redturtle.prenotazioni-2.6.5/src/redturtle/prenotazioni/utilities/
--rw-r--r--   0 roman      (502) staff       (20)       94 2024-04-24 08:56:49.000000 redturtle.prenotazioni-2.6.5/src/redturtle/prenotazioni/utilities/__init__.py
--rw-r--r--   0 roman      (502) staff       (20)     2900 2024-04-24 08:56:49.000000 redturtle.prenotazioni-2.6.5/src/redturtle/prenotazioni/utilities/dateutils.py
--rw-r--r--   0 roman      (502) staff       (20)      489 2024-04-24 08:56:49.000000 redturtle.prenotazioni-2.6.5/src/redturtle/prenotazioni/utilities/email.py
--rw-r--r--   0 roman      (502) staff       (20)      504 2024-04-24 08:56:49.000000 redturtle.prenotazioni-2.6.5/src/redturtle/prenotazioni/utilities/log_errors.py
--rw-r--r--   0 roman      (502) staff       (20)     1118 2024-04-24 08:56:49.000000 redturtle.prenotazioni-2.6.5/src/redturtle/prenotazioni/utilities/urls.py
-drwxr-xr-x   0 roman      (502) staff       (20)        0 2024-04-24 08:56:49.773729 redturtle.prenotazioni-2.6.5/src/redturtle/prenotazioni/utils/
--rw-r--r--   0 roman      (502) staff       (20)       67 2024-04-24 08:56:49.000000 redturtle.prenotazioni-2.6.5/src/redturtle/prenotazioni/utils/__init__.py
--rw-r--r--   0 roman      (502) staff       (20)      597 2024-04-24 08:56:49.000000 redturtle.prenotazioni-2.6.5/src/redturtle/prenotazioni/utils/get_prenotazioni_folder.py
-drwxr-xr-x   0 roman      (502) staff       (20)        0 2024-04-24 08:56:49.776253 redturtle.prenotazioni-2.6.5/src/redturtle/prenotazioni/vocabularies/
--rw-r--r--   0 roman      (502) staff       (20)       24 2024-04-24 08:56:49.000000 redturtle.prenotazioni-2.6.5/src/redturtle/prenotazioni/vocabularies/__init__.py
--rw-r--r--   0 roman      (502) staff       (20)     1444 2024-04-24 08:56:49.000000 redturtle.prenotazioni-2.6.5/src/redturtle/prenotazioni/vocabularies/configure.zcml
--rw-r--r--   0 roman      (502) staff       (20)      607 2024-04-24 08:56:49.000000 redturtle.prenotazioni-2.6.5/src/redturtle/prenotazioni/vocabularies/gates.py
--rw-r--r--   0 roman      (502) staff       (20)     1011 2024-04-24 08:56:49.000000 redturtle.prenotazioni-2.6.5/src/redturtle/prenotazioni/vocabularies/requirable_booking_fields.py
--rw-r--r--   0 roman      (502) staff       (20)      598 2024-04-24 08:56:49.000000 redturtle.prenotazioni-2.6.5/src/redturtle/prenotazioni/vocabularies/review_states.py
--rw-r--r--   0 roman      (502) staff       (20)     1814 2024-04-24 08:56:49.000000 redturtle.prenotazioni-2.6.5/src/redturtle/prenotazioni/vocabularies/tipologies.py
--rw-r--r--   0 roman      (502) staff       (20)      776 2024-04-24 08:56:49.000000 redturtle.prenotazioni-2.6.5/src/redturtle/prenotazioni/vocabularies/voc_booking_type_gates.py
--rw-r--r--   0 roman      (502) staff       (20)     1128 2024-04-24 08:56:49.000000 redturtle.prenotazioni-2.6.5/src/redturtle/prenotazioni/vocabularies/voc_durata_incontro.py
--rw-r--r--   0 roman      (502) staff       (20)     2549 2024-04-24 08:56:49.000000 redturtle.prenotazioni-2.6.5/src/redturtle/prenotazioni/vocabularies/voc_months.py
--rw-r--r--   0 roman      (502) staff       (20)     1367 2024-04-24 08:56:49.000000 redturtle.prenotazioni-2.6.5/src/redturtle/prenotazioni/vocabularies/voc_ore_inizio.py
--rw-r--r--   0 roman      (502) staff       (20)      440 2024-04-24 08:56:49.000000 redturtle.prenotazioni-2.6.5/src/redturtle/prenotazioni/vocabularies/voc_pause_scheduler.py
-drwxr-xr-x   0 roman      (502) staff       (20)        0 2024-04-24 08:56:49.708685 redturtle.prenotazioni-2.6.5/src/redturtle.prenotazioni.egg-info/
--rw-r--r--   0 roman      (502) staff       (20)    61067 2024-04-24 08:56:49.000000 redturtle.prenotazioni-2.6.5/src/redturtle.prenotazioni.egg-info/PKG-INFO
--rw-r--r--   0 roman      (502) staff       (20)    17548 2024-04-24 08:56:49.000000 redturtle.prenotazioni-2.6.5/src/redturtle.prenotazioni.egg-info/SOURCES.txt
--rw-r--r--   0 roman      (502) staff       (20)        1 2024-04-24 08:56:49.000000 redturtle.prenotazioni-2.6.5/src/redturtle.prenotazioni.egg-info/dependency_links.txt
--rw-r--r--   0 roman      (502) staff       (20)      295 2024-04-24 08:56:49.000000 redturtle.prenotazioni-2.6.5/src/redturtle.prenotazioni.egg-info/entry_points.txt
--rw-r--r--   0 roman      (502) staff       (20)       10 2024-04-24 08:56:49.000000 redturtle.prenotazioni-2.6.5/src/redturtle.prenotazioni.egg-info/namespace_packages.txt
--rw-r--r--   0 roman      (502) staff       (20)        1 2024-04-24 08:56:49.000000 redturtle.prenotazioni-2.6.5/src/redturtle.prenotazioni.egg-info/not-zip-safe
--rw-r--r--   0 roman      (502) staff       (20)      425 2024-04-24 08:56:49.000000 redturtle.prenotazioni-2.6.5/src/redturtle.prenotazioni.egg-info/requires.txt
--rw-r--r--   0 roman      (502) staff       (20)       10 2024-04-24 08:56:49.000000 redturtle.prenotazioni-2.6.5/src/redturtle.prenotazioni.egg-info/top_level.txt
+drwxr-xr-x   0 lucabel    (501) staff       (20)        0 2024-05-29 09:53:33.621829 redturtle.prenotazioni-2.7.0/
+-rw-r--r--   0 lucabel    (501) staff       (20)      748 2024-05-29 09:53:32.000000 redturtle.prenotazioni-2.7.0/APP_IO.txt
+-rw-r--r--   0 lucabel    (501) staff       (20)    18210 2024-05-29 09:53:32.000000 redturtle.prenotazioni-2.7.0/CHANGES.rst
+-rw-r--r--   0 lucabel    (501) staff       (20)      152 2024-05-29 09:53:32.000000 redturtle.prenotazioni-2.7.0/CONTRIBUTORS.rst
+-rw-r--r--   0 lucabel    (501) staff       (20)      586 2024-05-29 09:53:32.000000 redturtle.prenotazioni-2.7.0/DEVELOP.rst
+-rw-r--r--   0 lucabel    (501) staff       (20)    18092 2024-05-29 09:53:32.000000 redturtle.prenotazioni-2.7.0/LICENSE.GPL
+-rw-r--r--   0 lucabel    (501) staff       (20)      667 2024-05-29 09:53:32.000000 redturtle.prenotazioni-2.7.0/LICENSE.rst
+-rw-r--r--   0 lucabel    (501) staff       (20)      110 2024-05-29 09:53:32.000000 redturtle.prenotazioni-2.7.0/MANIFEST.in
+-rw-r--r--   0 lucabel    (501) staff       (20)    47127 2024-05-29 09:53:33.621964 redturtle.prenotazioni-2.7.0/PKG-INFO
+-rw-r--r--   0 lucabel    (501) staff       (20)    27508 2024-05-29 09:53:32.000000 redturtle.prenotazioni-2.7.0/README.rst
+-rw-r--r--   0 lucabel    (501) staff       (20)      164 2024-05-29 09:53:32.000000 redturtle.prenotazioni-2.7.0/TODO.txt
+-rw-r--r--   0 lucabel    (501) staff       (20)      105 2024-05-29 09:53:32.000000 redturtle.prenotazioni-2.7.0/constraints-5.2.x.txt
+-rw-r--r--   0 lucabel    (501) staff       (20)      105 2024-05-29 09:53:32.000000 redturtle.prenotazioni-2.7.0/constraints.txt
+drwxr-xr-x   0 lucabel    (501) staff       (20)        0 2024-05-29 09:53:33.542757 redturtle.prenotazioni-2.7.0/docs/
+-rw-r--r--   0 lucabel    (501) staff       (20)     7984 2024-05-29 09:53:32.000000 redturtle.prenotazioni-2.7.0/docs/conf.py
+-rw-r--r--   0 lucabel    (501) staff       (20)       89 2024-05-29 09:53:32.000000 redturtle.prenotazioni-2.7.0/docs/index.rst
+-rw-r--r--   0 lucabel    (501) staff       (20)      476 2024-05-29 09:53:32.000000 redturtle.prenotazioni-2.7.0/requirements-6.0.x.txt
+-rw-r--r--   0 lucabel    (501) staff       (20)       48 2024-05-29 09:53:32.000000 redturtle.prenotazioni-2.7.0/requirements.txt
+-rw-r--r--   0 lucabel    (501) staff       (20)      344 2024-05-29 09:53:33.622430 redturtle.prenotazioni-2.7.0/setup.cfg
+-rw-r--r--   0 lucabel    (501) staff       (20)     3420 2024-05-29 09:53:32.000000 redturtle.prenotazioni-2.7.0/setup.py
+drwxr-xr-x   0 lucabel    (501) staff       (20)        0 2024-05-29 09:53:33.524665 redturtle.prenotazioni-2.7.0/src/
+drwxr-xr-x   0 lucabel    (501) staff       (20)        0 2024-05-29 09:53:33.543047 redturtle.prenotazioni-2.7.0/src/redturtle/
+-rw-r--r--   0 lucabel    (501) staff       (20)       80 2024-05-29 09:53:32.000000 redturtle.prenotazioni-2.7.0/src/redturtle/__init__.py
+drwxr-xr-x   0 lucabel    (501) staff       (20)        0 2024-05-29 09:53:33.548627 redturtle.prenotazioni-2.7.0/src/redturtle/prenotazioni/
+-rw-r--r--   0 lucabel    (501) staff       (20)     4638 2024-05-29 09:53:32.000000 redturtle.prenotazioni-2.7.0/src/redturtle/prenotazioni/__init__.py
+drwxr-xr-x   0 lucabel    (501) staff       (20)        0 2024-05-29 09:53:33.549482 redturtle.prenotazioni-2.7.0/src/redturtle/prenotazioni/actions/
+-rw-r--r--   0 lucabel    (501) staff       (20)        0 2024-05-29 09:53:32.000000 redturtle.prenotazioni-2.7.0/src/redturtle/prenotazioni/actions/__init__.py
+-rw-r--r--   0 lucabel    (501) staff       (20)      226 2024-05-29 09:53:32.000000 redturtle.prenotazioni-2.7.0/src/redturtle/prenotazioni/actions/configure.zcml
+-rw-r--r--   0 lucabel    (501) staff       (20)     3333 2024-05-29 09:53:32.000000 redturtle.prenotazioni-2.7.0/src/redturtle/prenotazioni/actions/mail.py
+drwxr-xr-x   0 lucabel    (501) staff       (20)        0 2024-05-29 09:53:33.552142 redturtle.prenotazioni-2.7.0/src/redturtle/prenotazioni/adapters/
+-rw-r--r--   0 lucabel    (501) staff       (20)       24 2024-05-29 09:53:32.000000 redturtle.prenotazioni-2.7.0/src/redturtle/prenotazioni/adapters/__init__.py
+-rw-r--r--   0 lucabel    (501) staff       (20)    15296 2024-05-29 09:53:32.000000 redturtle.prenotazioni-2.7.0/src/redturtle/prenotazioni/adapters/booker.py
+-rw-r--r--   0 lucabel    (501) staff       (20)      729 2024-05-29 09:53:32.000000 redturtle.prenotazioni-2.7.0/src/redturtle/prenotazioni/adapters/booking_code.py
+-rw-r--r--   0 lucabel    (501) staff       (20)     5974 2024-05-29 09:53:32.000000 redturtle.prenotazioni-2.7.0/src/redturtle/prenotazioni/adapters/configure.zcml
+-rw-r--r--   0 lucabel    (501) staff       (20)     4988 2024-05-29 09:53:32.000000 redturtle.prenotazioni-2.7.0/src/redturtle/prenotazioni/adapters/conflict.py
+-rw-r--r--   0 lucabel    (501) staff       (20)     5035 2024-05-29 09:53:32.000000 redturtle.prenotazioni-2.7.0/src/redturtle/prenotazioni/adapters/ical.py
+-rw-r--r--   0 lucabel    (501) staff       (20)      273 2024-05-29 09:53:32.000000 redturtle.prenotazioni-2.7.0/src/redturtle/prenotazioni/adapters/prenotazione_menu.py
+-rw-r--r--   0 lucabel    (501) staff       (20)     9662 2024-05-29 09:53:32.000000 redturtle.prenotazioni-2.7.0/src/redturtle/prenotazioni/adapters/slot.py
+-rw-r--r--   0 lucabel    (501) staff       (20)     8771 2024-05-29 09:53:32.000000 redturtle.prenotazioni-2.7.0/src/redturtle/prenotazioni/adapters/stringinterp.py
+drwxr-xr-x   0 lucabel    (501) staff       (20)        0 2024-05-29 09:53:33.552442 redturtle.prenotazioni-2.7.0/src/redturtle/prenotazioni/behaviors/
+drwxr-xr-x   0 lucabel    (501) staff       (20)        0 2024-05-29 09:53:33.553285 redturtle.prenotazioni-2.7.0/src/redturtle/prenotazioni/behaviors/booking_folder/
+-rw-r--r--   0 lucabel    (501) staff       (20)        0 2024-05-29 09:53:32.000000 redturtle.prenotazioni-2.7.0/src/redturtle/prenotazioni/behaviors/booking_folder/__init__.py
+-rw-r--r--   0 lucabel    (501) staff       (20)      563 2024-05-29 09:53:32.000000 redturtle.prenotazioni-2.7.0/src/redturtle/prenotazioni/behaviors/booking_folder/configure.zcml
+-rw-r--r--   0 lucabel    (501) staff       (20)     1766 2024-05-29 09:53:32.000000 redturtle.prenotazioni-2.7.0/src/redturtle/prenotazioni/behaviors/booking_folder/contacts.py
+drwxr-xr-x   0 lucabel    (501) staff       (20)        0 2024-05-29 09:53:33.553882 redturtle.prenotazioni-2.7.0/src/redturtle/prenotazioni/behaviors/booking_folder/notifications/
+-rw-r--r--   0 lucabel    (501) staff       (20)     2362 2024-05-29 09:53:32.000000 redturtle.prenotazioni-2.7.0/src/redturtle/prenotazioni/behaviors/booking_folder/notifications/__init__.py
+drwxr-xr-x   0 lucabel    (501) staff       (20)        0 2024-05-29 09:53:33.555673 redturtle.prenotazioni-2.7.0/src/redturtle/prenotazioni/behaviors/booking_folder/notifications/appio/
+-rw-r--r--   0 lucabel    (501) staff       (20)    11754 2024-05-29 09:53:32.000000 redturtle.prenotazioni-2.7.0/src/redturtle/prenotazioni/behaviors/booking_folder/notifications/appio/__init__.py
+-rw-r--r--   0 lucabel    (501) staff       (20)     4255 2024-05-29 09:53:32.000000 redturtle.prenotazioni-2.7.0/src/redturtle/prenotazioni/behaviors/booking_folder/notifications/appio/adapters.py
+-rw-r--r--   0 lucabel    (501) staff       (20)     2364 2024-05-29 09:53:32.000000 redturtle.prenotazioni-2.7.0/src/redturtle/prenotazioni/behaviors/booking_folder/notifications/appio/configure.zcml
+-rw-r--r--   0 lucabel    (501) staff       (20)     3445 2024-05-29 09:53:32.000000 redturtle.prenotazioni-2.7.0/src/redturtle/prenotazioni/behaviors/booking_folder/notifications/appio/events.py
+-rw-r--r--   0 lucabel    (501) staff       (20)     4807 2024-05-29 09:53:32.000000 redturtle.prenotazioni-2.7.0/src/redturtle/prenotazioni/behaviors/booking_folder/notifications/appio/notfication_appio_message.py
+-rw-r--r--   0 lucabel    (501) staff       (20)     1151 2024-05-29 09:53:32.000000 redturtle.prenotazioni-2.7.0/src/redturtle/prenotazioni/behaviors/booking_folder/notifications/appio/voc_service_keys.py
+-rw-r--r--   0 lucabel    (501) staff       (20)      423 2024-05-29 09:53:32.000000 redturtle.prenotazioni-2.7.0/src/redturtle/prenotazioni/behaviors/booking_folder/notifications/configure.zcml
+drwxr-xr-x   0 lucabel    (501) staff       (20)        0 2024-05-29 09:53:33.557173 redturtle.prenotazioni-2.7.0/src/redturtle/prenotazioni/behaviors/booking_folder/notifications/email/
+-rw-r--r--   0 lucabel    (501) staff       (20)    11125 2024-05-29 09:53:32.000000 redturtle.prenotazioni-2.7.0/src/redturtle/prenotazioni/behaviors/booking_folder/notifications/email/__init__.py
+-rw-r--r--   0 lucabel    (501) staff       (20)     1791 2024-05-29 09:53:32.000000 redturtle.prenotazioni-2.7.0/src/redturtle/prenotazioni/behaviors/booking_folder/notifications/email/adapters.py
+-rw-r--r--   0 lucabel    (501) staff       (20)     2284 2024-05-29 09:53:32.000000 redturtle.prenotazioni-2.7.0/src/redturtle/prenotazioni/behaviors/booking_folder/notifications/email/configure.zcml
+-rw-r--r--   0 lucabel    (501) staff       (20)     4353 2024-05-29 09:53:32.000000 redturtle.prenotazioni-2.7.0/src/redturtle/prenotazioni/behaviors/booking_folder/notifications/email/events.py
+-rw-r--r--   0 lucabel    (501) staff       (20)    13947 2024-05-29 09:53:32.000000 redturtle.prenotazioni-2.7.0/src/redturtle/prenotazioni/behaviors/booking_folder/notifications/email/notification_email_message.py
+drwxr-xr-x   0 lucabel    (501) staff       (20)        0 2024-05-29 09:53:33.558662 redturtle.prenotazioni-2.7.0/src/redturtle/prenotazioni/behaviors/booking_folder/notifications/sms/
+-rw-r--r--   0 lucabel    (501) staff       (20)     6521 2024-05-29 09:53:32.000000 redturtle.prenotazioni-2.7.0/src/redturtle/prenotazioni/behaviors/booking_folder/notifications/sms/__init__.py
+-rw-r--r--   0 lucabel    (501) staff       (20)     1495 2024-05-29 09:53:32.000000 redturtle.prenotazioni-2.7.0/src/redturtle/prenotazioni/behaviors/booking_folder/notifications/sms/adapters.py
+-rw-r--r--   0 lucabel    (501) staff       (20)     1689 2024-05-29 09:53:32.000000 redturtle.prenotazioni-2.7.0/src/redturtle/prenotazioni/behaviors/booking_folder/notifications/sms/configure.zcml
+-rw-r--r--   0 lucabel    (501) staff       (20)     3775 2024-05-29 09:53:32.000000 redturtle.prenotazioni-2.7.0/src/redturtle/prenotazioni/behaviors/booking_folder/notifications/sms/events.py
+-rw-r--r--   0 lucabel    (501) staff       (20)     3877 2024-05-29 09:53:32.000000 redturtle.prenotazioni-2.7.0/src/redturtle/prenotazioni/behaviors/booking_folder/notifications/sms/message.py
+-rw-r--r--   0 lucabel    (501) staff       (20)      284 2024-05-29 09:53:32.000000 redturtle.prenotazioni-2.7.0/src/redturtle/prenotazioni/behaviors/configure.zcml
+drwxr-xr-x   0 lucabel    (501) staff       (20)        0 2024-05-29 09:53:33.563909 redturtle.prenotazioni-2.7.0/src/redturtle/prenotazioni/browser/
+-rw-r--r--   0 lucabel    (501) staff       (20)        0 2024-05-29 09:53:32.000000 redturtle.prenotazioni-2.7.0/src/redturtle/prenotazioni/browser/__init__.py
+-rw-r--r--   0 lucabel    (501) staff       (20)     1817 2024-05-29 09:53:32.000000 redturtle.prenotazioni-2.7.0/src/redturtle/prenotazioni/browser/base.py
+-rw-r--r--   0 lucabel    (501) staff       (20)     7331 2024-05-29 09:53:32.000000 redturtle.prenotazioni-2.7.0/src/redturtle/prenotazioni/browser/configure.zcml
+-rw-r--r--   0 lucabel    (501) staff       (20)      655 2024-05-29 09:53:32.000000 redturtle.prenotazioni-2.7.0/src/redturtle/prenotazioni/browser/custom_radio_input.pt
+-rw-r--r--   0 lucabel    (501) staff       (20)     5709 2024-05-29 09:53:32.000000 redturtle.prenotazioni-2.7.0/src/redturtle/prenotazioni/browser/delete_reservation.py
+-rw-r--r--   0 lucabel    (501) staff       (20)      673 2024-05-29 09:53:32.000000 redturtle.prenotazioni-2.7.0/src/redturtle/prenotazioni/browser/folderfactories.py
+-rw-r--r--   0 lucabel    (501) staff       (20)      155 2024-05-29 09:53:32.000000 redturtle.prenotazioni-2.7.0/src/redturtle/prenotazioni/browser/interfaces.py
+drwxr-xr-x   0 lucabel    (501) staff       (20)        0 2024-05-29 09:53:33.564180 redturtle.prenotazioni-2.7.0/src/redturtle/prenotazioni/browser/overrides/
+-rw-r--r--   0 lucabel    (501) staff       (20)        0 2024-05-29 09:53:32.000000 redturtle.prenotazioni-2.7.0/src/redturtle/prenotazioni/browser/overrides/.gitkeep
+-rw-r--r--   0 lucabel    (501) staff       (20)     3169 2024-05-29 09:53:32.000000 redturtle.prenotazioni-2.7.0/src/redturtle/prenotazioni/browser/prenotazione.py
+-rw-r--r--   0 lucabel    (501) staff       (20)    10057 2024-05-29 09:53:32.000000 redturtle.prenotazioni-2.7.0/src/redturtle/prenotazioni/browser/prenotazione_add.py
+-rw-r--r--   0 lucabel    (501) staff       (20)     5252 2024-05-29 09:53:32.000000 redturtle.prenotazioni-2.7.0/src/redturtle/prenotazioni/browser/prenotazione_move.py
+-rw-r--r--   0 lucabel    (501) staff       (20)     2721 2024-05-29 09:53:32.000000 redturtle.prenotazioni-2.7.0/src/redturtle/prenotazioni/browser/prenotazione_print.py
+-rw-r--r--   0 lucabel    (501) staff       (20)    38319 2024-05-29 09:53:32.000000 redturtle.prenotazioni-2.7.0/src/redturtle/prenotazioni/browser/prenotazioni_context_state.py
+-rw-r--r--   0 lucabel    (501) staff       (20)     1735 2024-05-29 09:53:32.000000 redturtle.prenotazioni-2.7.0/src/redturtle/prenotazioni/browser/prenotazioni_portal_state.py
+-rw-r--r--   0 lucabel    (501) staff       (20)    13788 2024-05-29 09:53:32.000000 redturtle.prenotazioni-2.7.0/src/redturtle/prenotazioni/browser/prenotazioni_search.py
+drwxr-xr-x   0 lucabel    (501) staff       (20)        0 2024-05-29 09:53:33.565890 redturtle.prenotazioni-2.7.0/src/redturtle/prenotazioni/browser/static/
+-rw-r--r--   0 lucabel    (501) staff       (20)        0 2024-05-29 09:53:32.000000 redturtle.prenotazioni-2.7.0/src/redturtle/prenotazioni/browser/static/.gitkeep
+-rw-r--r--   0 lucabel    (501) staff       (20)      364 2024-05-29 09:53:32.000000 redturtle.prenotazioni-2.7.0/src/redturtle/prenotazioni/browser/static/calendar-add.png
+-rw-r--r--   0 lucabel    (501) staff       (20)      503 2024-05-29 09:53:32.000000 redturtle.prenotazioni-2.7.0/src/redturtle/prenotazioni/browser/static/calendar-icon.png
+-rw-r--r--   0 lucabel    (501) staff       (20)      266 2024-05-29 09:53:32.000000 redturtle.prenotazioni-2.7.0/src/redturtle/prenotazioni/browser/static/cross-icon.png
+-rw-r--r--   0 lucabel    (501) staff       (20)     9794 2024-05-29 09:53:32.000000 redturtle.prenotazioni-2.7.0/src/redturtle/prenotazioni/browser/static/redturtle-reservation.css
+-rw-r--r--   0 lucabel    (501) staff       (20)     1600 2024-05-29 09:53:32.000000 redturtle.prenotazioni-2.7.0/src/redturtle/prenotazioni/browser/static/redturtle-reservation.js
+-rw-r--r--   0 lucabel    (501) staff       (20)      922 2024-05-29 09:53:32.000000 redturtle.prenotazioni-2.7.0/src/redturtle/prenotazioni/browser/static/times-solid.png
+drwxr-xr-x   0 lucabel    (501) staff       (20)        0 2024-05-29 09:53:33.527995 redturtle.prenotazioni-2.7.0/src/redturtle/prenotazioni/browser/static/widget/
+drwxr-xr-x   0 lucabel    (501) staff       (20)        0 2024-05-29 09:53:33.527785 redturtle.prenotazioni-2.7.0/src/redturtle/prenotazioni/browser/static/widget/dist/
+drwxr-xr-x   0 lucabel    (501) staff       (20)        0 2024-05-29 09:53:33.567298 redturtle.prenotazioni-2.7.0/src/redturtle/prenotazioni/browser/static/widget/dist/prod/
+-rw-r--r--   0 lucabel    (501) staff       (20)     3239 2024-05-29 09:53:32.000000 redturtle.prenotazioni-2.7.0/src/redturtle/prenotazioni/browser/static/widget/dist/prod/main.css
+-rw-r--r--   0 lucabel    (501) staff       (20)     3808 2024-05-29 09:53:32.000000 redturtle.prenotazioni-2.7.0/src/redturtle/prenotazioni/browser/static/widget/dist/prod/main.css.map
+-rw-r--r--   0 lucabel    (501) staff       (20)   349785 2024-05-29 09:53:32.000000 redturtle.prenotazioni-2.7.0/src/redturtle/prenotazioni/browser/static/widget/dist/prod/main.js
+-rw-r--r--   0 lucabel    (501) staff       (20)      148 2024-05-29 09:53:32.000000 redturtle.prenotazioni-2.7.0/src/redturtle/prenotazioni/browser/static/widget/dist/prod/main.js.map
+drwxr-xr-x   0 lucabel    (501) staff       (20)        0 2024-05-29 09:53:33.567558 redturtle.prenotazioni-2.7.0/src/redturtle/prenotazioni/browser/static/widget/js/
+drwxr-xr-x   0 lucabel    (501) staff       (20)        0 2024-05-29 09:53:33.567814 redturtle.prenotazioni-2.7.0/src/redturtle/prenotazioni/browser/static/widget/js/WidgetContainer/
+-rw-r--r--   0 lucabel    (501) staff       (20)     5095 2024-05-29 09:53:32.000000 redturtle.prenotazioni-2.7.0/src/redturtle/prenotazioni/browser/static/widget/js/WidgetContainer/index.js
+drwxr-xr-x   0 lucabel    (501) staff       (20)        0 2024-05-29 09:53:33.568335 redturtle.prenotazioni-2.7.0/src/redturtle/prenotazioni/browser/static/widget/js/WidgetDataContainer/
+-rw-r--r--   0 lucabel    (501) staff       (20)     4705 2024-05-29 09:53:32.000000 redturtle.prenotazioni-2.7.0/src/redturtle/prenotazioni/browser/static/widget/js/WidgetDataContainer/index.js
+-rw-r--r--   0 lucabel    (501) staff       (20)     1059 2024-05-29 09:53:32.000000 redturtle.prenotazioni-2.7.0/src/redturtle/prenotazioni/browser/static/widget/js/WidgetDataContainer/index.less
+drwxr-xr-x   0 lucabel    (501) staff       (20)        0 2024-05-29 09:53:33.570926 redturtle.prenotazioni-2.7.0/src/redturtle/prenotazioni/browser/static/widget/js/fields/
+-rw-r--r--   0 lucabel    (501) staff       (20)     3010 2024-05-29 09:53:32.000000 redturtle.prenotazioni-2.7.0/src/redturtle/prenotazioni/browser/static/widget/js/fields/DaysTableField.js
+-rw-r--r--   0 lucabel    (501) staff       (20)      204 2024-05-29 09:53:32.000000 redturtle.prenotazioni-2.7.0/src/redturtle/prenotazioni/browser/static/widget/js/fields/DaysTableField.less
+-rw-r--r--   0 lucabel    (501) staff       (20)     2874 2024-05-29 09:53:32.000000 redturtle.prenotazioni-2.7.0/src/redturtle/prenotazioni/browser/static/widget/js/fields/GatesField.js
+-rw-r--r--   0 lucabel    (501) staff       (20)      401 2024-05-29 09:53:32.000000 redturtle.prenotazioni-2.7.0/src/redturtle/prenotazioni/browser/static/widget/js/fields/GatesField.less
+-rw-r--r--   0 lucabel    (501) staff       (20)     1888 2024-05-29 09:53:32.000000 redturtle.prenotazioni-2.7.0/src/redturtle/prenotazioni/browser/static/widget/js/fields/IntervalSelectorField.js
+-rw-r--r--   0 lucabel    (501) staff       (20)      314 2024-05-29 09:53:32.000000 redturtle.prenotazioni-2.7.0/src/redturtle/prenotazioni/browser/static/widget/js/fields/IntervalSelectorField.less
+-rw-r--r--   0 lucabel    (501) staff       (20)     4187 2024-05-29 09:53:32.000000 redturtle.prenotazioni-2.7.0/src/redturtle/prenotazioni/browser/static/widget/js/fields/PauseTableField.js
+-rw-r--r--   0 lucabel    (501) staff       (20)      337 2024-05-29 09:53:32.000000 redturtle.prenotazioni-2.7.0/src/redturtle/prenotazioni/browser/static/widget/js/fields/PauseTableField.less
+-rw-r--r--   0 lucabel    (501) staff       (20)     1745 2024-05-29 09:53:32.000000 redturtle.prenotazioni-2.7.0/src/redturtle/prenotazioni/browser/static/widget/js/fields/SelectField.js
+-rw-r--r--   0 lucabel    (501) staff       (20)      961 2024-05-29 09:53:32.000000 redturtle.prenotazioni-2.7.0/src/redturtle/prenotazioni/browser/static/widget/js/fields/TextLineField.js
+-rw-r--r--   0 lucabel    (501) staff       (20)     1261 2024-05-29 09:53:32.000000 redturtle.prenotazioni-2.7.0/src/redturtle/prenotazioni/browser/static/widget/js/index.js
+drwxr-xr-x   0 lucabel    (501) staff       (20)        0 2024-05-29 09:53:33.571445 redturtle.prenotazioni-2.7.0/src/redturtle/prenotazioni/browser/static/widget/js/utils/
+-rw-r--r--   0 lucabel    (501) staff       (20)      941 2024-05-29 09:53:32.000000 redturtle.prenotazioni-2.7.0/src/redturtle/prenotazioni/browser/static/widget/js/utils/i18n.js
+-rw-r--r--   0 lucabel    (501) staff       (20)      298 2024-05-29 09:53:32.000000 redturtle.prenotazioni-2.7.0/src/redturtle/prenotazioni/browser/static/widget/js/utils/widgetContext.js
+drwxr-xr-x   0 lucabel    (501) staff       (20)        0 2024-05-29 09:53:33.572462 redturtle.prenotazioni-2.7.0/src/redturtle/prenotazioni/browser/stats/
+-rw-r--r--   0 lucabel    (501) staff       (20)       24 2024-05-29 09:53:32.000000 redturtle.prenotazioni-2.7.0/src/redturtle/prenotazioni/browser/stats/__init__.py
+-rw-r--r--   0 lucabel    (501) staff       (20)      698 2024-05-29 09:53:32.000000 redturtle.prenotazioni-2.7.0/src/redturtle/prenotazioni/browser/stats/booking_stats.pt
+-rw-r--r--   0 lucabel    (501) staff       (20)     3863 2024-05-29 09:53:32.000000 redturtle.prenotazioni-2.7.0/src/redturtle/prenotazioni/browser/stats/booking_stats.py
+-rw-r--r--   0 lucabel    (501) staff       (20)      575 2024-05-29 09:53:32.000000 redturtle.prenotazioni-2.7.0/src/redturtle/prenotazioni/browser/stats/configure.zcml
+drwxr-xr-x   0 lucabel    (501) staff       (20)        0 2024-05-29 09:53:33.575857 redturtle.prenotazioni-2.7.0/src/redturtle/prenotazioni/browser/templates/
+-rw-r--r--   0 lucabel    (501) staff       (20)     2836 2024-05-29 09:53:32.000000 redturtle.prenotazioni-2.7.0/src/redturtle/prenotazioni/browser/templates/booking_type_radio_widget.pt
+-rw-r--r--   0 lucabel    (501) staff       (20)     1518 2024-05-29 09:53:32.000000 redturtle.prenotazioni-2.7.0/src/redturtle/prenotazioni/browser/templates/custom_dgf_input.pt
+-rw-r--r--   0 lucabel    (501) staff       (20)     4828 2024-05-29 09:53:32.000000 redturtle.prenotazioni-2.7.0/src/redturtle/prenotazioni/browser/templates/delete_reservation.pt
+-rw-r--r--   0 lucabel    (501) staff       (20)     2417 2024-05-29 09:53:32.000000 redturtle.prenotazioni-2.7.0/src/redturtle/prenotazioni/browser/templates/manager_notification_mail.pt
+-rw-r--r--   0 lucabel    (501) staff       (20)       48 2024-05-29 09:53:32.000000 redturtle.prenotazioni-2.7.0/src/redturtle/prenotazioni/browser/templates/nofollow.pt
+-rw-r--r--   0 lucabel    (501) staff       (20)     7714 2024-05-29 09:53:32.000000 redturtle.prenotazioni-2.7.0/src/redturtle/prenotazioni/browser/templates/prenotazione.pt
+-rw-r--r--   0 lucabel    (501) staff       (20)     9592 2024-05-29 09:53:32.000000 redturtle.prenotazioni-2.7.0/src/redturtle/prenotazioni/browser/templates/prenotazione_add.pt
+-rw-r--r--   0 lucabel    (501) staff       (20)    16384 2024-05-29 09:53:32.000000 redturtle.prenotazioni-2.7.0/src/redturtle/prenotazioni/browser/templates/prenotazione_macros.pt
+-rw-r--r--   0 lucabel    (501) staff       (20)     2227 2024-05-29 09:53:32.000000 redturtle.prenotazioni-2.7.0/src/redturtle/prenotazioni/browser/templates/prenotazione_move.pt
+-rw-r--r--   0 lucabel    (501) staff       (20)     5299 2024-05-29 09:53:32.000000 redturtle.prenotazioni-2.7.0/src/redturtle/prenotazioni/browser/templates/prenotazione_print.pt
+-rw-r--r--   0 lucabel    (501) staff       (20)     5241 2024-05-29 09:53:32.000000 redturtle.prenotazioni-2.7.0/src/redturtle/prenotazioni/browser/templates/prenotazioni_search.pt
+-rw-r--r--   0 lucabel    (501) staff       (20)     1858 2024-05-29 09:53:32.000000 redturtle.prenotazioni-2.7.0/src/redturtle/prenotazioni/browser/templates/week.pt
+-rw-r--r--   0 lucabel    (501) staff       (20)      362 2024-05-29 09:53:32.000000 redturtle.prenotazioni-2.7.0/src/redturtle/prenotazioni/browser/templates/week_table_overrides_widget_input.pt
+drwxr-xr-x   0 lucabel    (501) staff       (20)        0 2024-05-29 09:53:33.576563 redturtle.prenotazioni-2.7.0/src/redturtle/prenotazioni/browser/utilities/
+-rw-r--r--   0 lucabel    (501) staff       (20)        0 2024-05-29 09:53:32.000000 redturtle.prenotazioni-2.7.0/src/redturtle/prenotazioni/browser/utilities/__init__.py
+-rw-r--r--   0 lucabel    (501) staff       (20)      494 2024-05-29 09:53:32.000000 redturtle.prenotazioni-2.7.0/src/redturtle/prenotazioni/browser/utilities/configure.zcml
+-rw-r--r--   0 lucabel    (501) staff       (20)     1873 2024-05-29 09:53:32.000000 redturtle.prenotazioni-2.7.0/src/redturtle/prenotazioni/browser/utilities/notify_upcoming_bookings.py
+-rw-r--r--   0 lucabel    (501) staff       (20)     8087 2024-05-29 09:53:32.000000 redturtle.prenotazioni-2.7.0/src/redturtle/prenotazioni/browser/vacations.py
+-rw-r--r--   0 lucabel    (501) staff       (20)     1524 2024-05-29 09:53:32.000000 redturtle.prenotazioni-2.7.0/src/redturtle/prenotazioni/browser/viewlets.py
+-rw-r--r--   0 lucabel    (501) staff       (20)    10861 2024-05-29 09:53:32.000000 redturtle.prenotazioni-2.7.0/src/redturtle/prenotazioni/browser/week.py
+-rw-r--r--   0 lucabel    (501) staff       (20)     1193 2024-05-29 09:53:32.000000 redturtle.prenotazioni-2.7.0/src/redturtle/prenotazioni/browser/widget.py
+-rw-r--r--   0 lucabel    (501) staff       (20)     6304 2024-05-29 09:53:32.000000 redturtle.prenotazioni-2.7.0/src/redturtle/prenotazioni/browser/z3c_custom_widget.py
+-rw-r--r--   0 lucabel    (501) staff       (20)      485 2024-05-29 09:53:32.000000 redturtle.prenotazioni-2.7.0/src/redturtle/prenotazioni/config.py
+-rw-r--r--   0 lucabel    (501) staff       (20)     2049 2024-05-29 09:53:32.000000 redturtle.prenotazioni-2.7.0/src/redturtle/prenotazioni/configure.zcml
+drwxr-xr-x   0 lucabel    (501) staff       (20)        0 2024-05-29 09:53:33.579140 redturtle.prenotazioni-2.7.0/src/redturtle/prenotazioni/content/
+-rw-r--r--   0 lucabel    (501) staff       (20)       24 2024-05-29 09:53:32.000000 redturtle.prenotazioni-2.7.0/src/redturtle/prenotazioni/content/__init__.py
+-rw-r--r--   0 lucabel    (501) staff       (20)      111 2024-05-29 09:53:32.000000 redturtle.prenotazioni-2.7.0/src/redturtle/prenotazioni/content/booking_type.py
+-rw-r--r--   0 lucabel    (501) staff       (20)     1537 2024-05-29 09:53:32.000000 redturtle.prenotazioni-2.7.0/src/redturtle/prenotazioni/content/pause.py
+-rw-r--r--   0 lucabel    (501) staff       (20)     7504 2024-05-29 09:53:32.000000 redturtle.prenotazioni-2.7.0/src/redturtle/prenotazioni/content/prenotazione.py
+-rw-r--r--   0 lucabel    (501) staff       (20)     1251 2024-05-29 09:53:32.000000 redturtle.prenotazioni-2.7.0/src/redturtle/prenotazioni/content/prenotazione_type.py
+-rw-r--r--   0 lucabel    (501) staff       (20)      367 2024-05-29 09:53:32.000000 redturtle.prenotazioni-2.7.0/src/redturtle/prenotazioni/content/prenotazioni_day.py
+-rw-r--r--   0 lucabel    (501) staff       (20)    19857 2024-05-29 09:53:32.000000 redturtle.prenotazioni-2.7.0/src/redturtle/prenotazioni/content/prenotazioni_folder.py
+-rw-r--r--   0 lucabel    (501) staff       (20)      371 2024-05-29 09:53:32.000000 redturtle.prenotazioni-2.7.0/src/redturtle/prenotazioni/content/prenotazioni_week.py
+-rw-r--r--   0 lucabel    (501) staff       (20)      371 2024-05-29 09:53:32.000000 redturtle.prenotazioni-2.7.0/src/redturtle/prenotazioni/content/prenotazioni_year.py
+-rw-r--r--   0 lucabel    (501) staff       (20)     8518 2024-05-29 09:53:32.000000 redturtle.prenotazioni-2.7.0/src/redturtle/prenotazioni/content/validators.py
+drwxr-xr-x   0 lucabel    (501) staff       (20)        0 2024-05-29 09:53:33.580489 redturtle.prenotazioni-2.7.0/src/redturtle/prenotazioni/demo/
+-rw-r--r--   0 lucabel    (501) staff       (20)       77 2024-05-29 09:53:32.000000 redturtle.prenotazioni-2.7.0/src/redturtle/prenotazioni/demo/__init__.py
+-rw-r--r--   0 lucabel    (501) staff       (20)     1088 2024-05-29 09:53:32.000000 redturtle.prenotazioni-2.7.0/src/redturtle/prenotazioni/demo/configure.zcml
+-rw-r--r--   0 lucabel    (501) staff       (20)      227 2024-05-29 09:53:32.000000 redturtle.prenotazioni-2.7.0/src/redturtle/prenotazioni/demo/interfaces.py
+drwxr-xr-x   0 lucabel    (501) staff       (20)        0 2024-05-29 09:53:33.530438 redturtle.prenotazioni-2.7.0/src/redturtle/prenotazioni/demo/profiles/
+drwxr-xr-x   0 lucabel    (501) staff       (20)        0 2024-05-29 09:53:33.581107 redturtle.prenotazioni-2.7.0/src/redturtle/prenotazioni/demo/profiles/default/
+-rw-r--r--   0 lucabel    (501) staff       (20)      208 2024-05-29 09:53:32.000000 redturtle.prenotazioni-2.7.0/src/redturtle/prenotazioni/demo/profiles/default/browserlayer.xml
+-rw-r--r--   0 lucabel    (501) staff       (20)       88 2024-05-29 09:53:32.000000 redturtle.prenotazioni-2.7.0/src/redturtle/prenotazioni/demo/profiles/default/metadata.xml
+drwxr-xr-x   0 lucabel    (501) staff       (20)        0 2024-05-29 09:53:33.581370 redturtle.prenotazioni-2.7.0/src/redturtle/prenotazioni/demo/profiles/uninstall/
+-rw-r--r--   0 lucabel    (501) staff       (20)      133 2024-05-29 09:53:32.000000 redturtle.prenotazioni-2.7.0/src/redturtle/prenotazioni/demo/profiles/uninstall/browserlayer.xml
+-rw-r--r--   0 lucabel    (501) staff       (20)      630 2024-05-29 09:53:32.000000 redturtle.prenotazioni-2.7.0/src/redturtle/prenotazioni/demo/setuphandlers.py
+-rw-r--r--   0 lucabel    (501) staff       (20)     1347 2024-05-29 09:53:32.000000 redturtle.prenotazioni-2.7.0/src/redturtle/prenotazioni/demo/smsdemo.py
+drwxr-xr-x   0 lucabel    (501) staff       (20)        0 2024-05-29 09:53:33.582615 redturtle.prenotazioni-2.7.0/src/redturtle/prenotazioni/events/
+-rw-r--r--   0 lucabel    (501) staff       (20)      270 2024-05-29 09:53:32.000000 redturtle.prenotazioni-2.7.0/src/redturtle/prenotazioni/events/__init__.py
+-rw-r--r--   0 lucabel    (501) staff       (20)     1615 2024-05-29 09:53:32.000000 redturtle.prenotazioni-2.7.0/src/redturtle/prenotazioni/events/configure.zcml
+-rw-r--r--   0 lucabel    (501) staff       (20)     2101 2024-05-29 09:53:32.000000 redturtle.prenotazioni-2.7.0/src/redturtle/prenotazioni/events/events_logger.py
+-rw-r--r--   0 lucabel    (501) staff       (20)     1907 2024-05-29 09:53:32.000000 redturtle.prenotazioni-2.7.0/src/redturtle/prenotazioni/events/prenotazione.py
+-rw-r--r--   0 lucabel    (501) staff       (20)     1189 2024-05-29 09:53:32.000000 redturtle.prenotazioni-2.7.0/src/redturtle/prenotazioni/events/prenotazioni_folder.py
+drwxr-xr-x   0 lucabel    (501) staff       (20)        0 2024-05-29 09:53:33.583110 redturtle.prenotazioni-2.7.0/src/redturtle/prenotazioni/exceptions/
+-rw-r--r--   0 lucabel    (501) staff       (20)      129 2024-05-29 09:53:32.000000 redturtle.prenotazioni-2.7.0/src/redturtle/prenotazioni/exceptions/__init__.py
+-rw-r--r--   0 lucabel    (501) staff       (20)      712 2024-05-29 09:53:32.000000 redturtle.prenotazioni-2.7.0/src/redturtle/prenotazioni/exceptions/booker.py
+drwxr-xr-x   0 lucabel    (501) staff       (20)        0 2024-05-29 09:53:33.583856 redturtle.prenotazioni-2.7.0/src/redturtle/prenotazioni/indexers/
+-rw-r--r--   0 lucabel    (501) staff       (20)       24 2024-05-29 09:53:32.000000 redturtle.prenotazioni-2.7.0/src/redturtle/prenotazioni/indexers/__init__.py
+-rw-r--r--   0 lucabel    (501) staff       (20)      476 2024-05-29 09:53:32.000000 redturtle.prenotazioni-2.7.0/src/redturtle/prenotazioni/indexers/configure.zcml
+-rw-r--r--   0 lucabel    (501) staff       (20)     1410 2024-05-29 09:53:32.000000 redturtle.prenotazioni-2.7.0/src/redturtle/prenotazioni/indexers/prenotazione.py
+-rw-r--r--   0 lucabel    (501) staff       (20)     1445 2024-05-29 09:53:32.000000 redturtle.prenotazioni-2.7.0/src/redturtle/prenotazioni/interfaces.py
+drwxr-xr-x   0 lucabel    (501) staff       (20)        0 2024-05-29 09:53:33.586769 redturtle.prenotazioni-2.7.0/src/redturtle/prenotazioni/io_tools/
+-rw-r--r--   0 lucabel    (501) staff       (20)     5302 2024-05-29 09:53:32.000000 redturtle.prenotazioni-2.7.0/src/redturtle/prenotazioni/io_tools/README.md
+-rw-r--r--   0 lucabel    (501) staff       (20)      207 2024-05-29 09:53:32.000000 redturtle.prenotazioni-2.7.0/src/redturtle/prenotazioni/io_tools/__init__.py
+-rw-r--r--   0 lucabel    (501) staff       (20)     9443 2024-05-29 09:53:32.000000 redturtle.prenotazioni-2.7.0/src/redturtle/prenotazioni/io_tools/api.py
+-rw-r--r--   0 lucabel    (501) staff       (20)     1035 2024-05-29 09:53:32.000000 redturtle.prenotazioni-2.7.0/src/redturtle/prenotazioni/io_tools/cli.py
+-rw-r--r--   0 lucabel    (501) staff       (20)    16384 2024-05-29 09:53:32.000000 redturtle.prenotazioni-2.7.0/src/redturtle/prenotazioni/io_tools/io.db
+-rw-r--r--   0 lucabel    (501) staff       (20)       45 2024-05-29 09:53:32.000000 redturtle.prenotazioni-2.7.0/src/redturtle/prenotazioni/io_tools/io_tools.py
+-rw-r--r--   0 lucabel    (501) staff       (20)     1945 2024-05-29 09:53:32.000000 redturtle.prenotazioni-2.7.0/src/redturtle/prenotazioni/io_tools/monkey.py
+-rw-r--r--   0 lucabel    (501) staff       (20)     2833 2024-05-29 09:53:32.000000 redturtle.prenotazioni-2.7.0/src/redturtle/prenotazioni/io_tools/rdbms.py
+-rw-r--r--   0 lucabel    (501) staff       (20)    27521 2024-05-29 09:53:32.000000 redturtle.prenotazioni-2.7.0/src/redturtle/prenotazioni/io_tools/spec.yaml
+-rw-r--r--   0 lucabel    (501) staff       (20)      961 2024-05-29 09:53:32.000000 redturtle.prenotazioni-2.7.0/src/redturtle/prenotazioni/io_tools/storage.py
+drwxr-xr-x   0 lucabel    (501) staff       (20)        0 2024-05-29 09:53:33.588083 redturtle.prenotazioni-2.7.0/src/redturtle/prenotazioni/locales/
+drwxr-xr-x   0 lucabel    (501) staff       (20)        0 2024-05-29 09:53:33.531763 redturtle.prenotazioni-2.7.0/src/redturtle/prenotazioni/locales/en/
+drwxr-xr-x   0 lucabel    (501) staff       (20)        0 2024-05-29 09:53:33.588372 redturtle.prenotazioni-2.7.0/src/redturtle/prenotazioni/locales/en/LC_MESSAGES/
+-rw-r--r--   0 lucabel    (501) staff       (20)    62535 2024-05-29 09:53:32.000000 redturtle.prenotazioni-2.7.0/src/redturtle/prenotazioni/locales/en/LC_MESSAGES/redturtle.prenotazioni.po
+drwxr-xr-x   0 lucabel    (501) staff       (20)        0 2024-05-29 09:53:33.532106 redturtle.prenotazioni-2.7.0/src/redturtle/prenotazioni/locales/it/
+drwxr-xr-x   0 lucabel    (501) staff       (20)        0 2024-05-29 09:53:33.589041 redturtle.prenotazioni-2.7.0/src/redturtle/prenotazioni/locales/it/LC_MESSAGES/
+-rw-r--r--   0 lucabel    (501) staff       (20)      804 2024-05-29 09:53:32.000000 redturtle.prenotazioni-2.7.0/src/redturtle/prenotazioni/locales/it/LC_MESSAGES/plone.po
+-rw-r--r--   0 lucabel    (501) staff       (20)    80885 2024-05-29 09:53:32.000000 redturtle.prenotazioni-2.7.0/src/redturtle/prenotazioni/locales/it/LC_MESSAGES/redturtle.prenotazioni.po
+-rw-r--r--   0 lucabel    (501) staff       (20)     1012 2024-05-29 09:53:32.000000 redturtle.prenotazioni-2.7.0/src/redturtle/prenotazioni/locales/manual.pot
+-rw-r--r--   0 lucabel    (501) staff       (20)    62826 2024-05-29 09:53:32.000000 redturtle.prenotazioni-2.7.0/src/redturtle/prenotazioni/locales/redturtle.prenotazioni.pot
+-rw-r--r--   0 lucabel    (501) staff       (20)     1618 2024-05-29 09:53:32.000000 redturtle.prenotazioni-2.7.0/src/redturtle/prenotazioni/locales/update.py
+-rwxr-xr-x   0 lucabel    (501) staff       (20)      521 2024-05-29 09:53:32.000000 redturtle.prenotazioni-2.7.0/src/redturtle/prenotazioni/locales/update.sh
+drwxr-xr-x   0 lucabel    (501) staff       (20)        0 2024-05-29 09:53:33.589588 redturtle.prenotazioni-2.7.0/src/redturtle/prenotazioni/monkeypatcher/
+-rw-r--r--   0 lucabel    (501) staff       (20)        0 2024-05-29 09:53:32.000000 redturtle.prenotazioni-2.7.0/src/redturtle/prenotazioni/monkeypatcher/__init__.py
+-rw-r--r--   0 lucabel    (501) staff       (20)      499 2024-05-29 09:53:32.000000 redturtle.prenotazioni-2.7.0/src/redturtle/prenotazioni/monkeypatcher/configure.zcml
+-rw-r--r--   0 lucabel    (501) staff       (20)     1565 2024-05-29 09:53:32.000000 redturtle.prenotazioni-2.7.0/src/redturtle/prenotazioni/permissions.zcml
+-rw-r--r--   0 lucabel    (501) staff       (20)      507 2024-05-29 09:53:32.000000 redturtle.prenotazioni-2.7.0/src/redturtle/prenotazioni/prenotazione_event.py
+drwxr-xr-x   0 lucabel    (501) staff       (20)        0 2024-05-29 09:53:33.534731 redturtle.prenotazioni-2.7.0/src/redturtle/prenotazioni/profiles/
+drwxr-xr-x   0 lucabel    (501) staff       (20)        0 2024-05-29 09:53:33.592378 redturtle.prenotazioni-2.7.0/src/redturtle/prenotazioni/profiles/default/
+-rw-r--r--   0 lucabel    (501) staff       (20)     2656 2024-05-29 09:53:32.000000 redturtle.prenotazioni-2.7.0/src/redturtle/prenotazioni/profiles/default/actions.xml
+-rw-r--r--   0 lucabel    (501) staff       (20)      185 2024-05-29 09:53:32.000000 redturtle.prenotazioni-2.7.0/src/redturtle/prenotazioni/profiles/default/browserlayer.xml
+-rw-r--r--   0 lucabel    (501) staff       (20)      349 2024-05-29 09:53:32.000000 redturtle.prenotazioni-2.7.0/src/redturtle/prenotazioni/profiles/default/catalog.xml
+-rw-r--r--   0 lucabel    (501) staff       (20)       71 2024-05-29 09:53:32.000000 redturtle.prenotazioni-2.7.0/src/redturtle/prenotazioni/profiles/default/contentrules.xml
+-rw-r--r--   0 lucabel    (501) staff       (20)      196 2024-05-29 09:53:32.000000 redturtle.prenotazioni-2.7.0/src/redturtle/prenotazioni/profiles/default/diff_tool.xml
+-rw-r--r--   0 lucabel    (501) staff       (20)      325 2024-05-29 09:53:32.000000 redturtle.prenotazioni-2.7.0/src/redturtle/prenotazioni/profiles/default/metadata.xml
+drwxr-xr-x   0 lucabel    (501) staff       (20)        0 2024-05-29 09:53:33.593145 redturtle.prenotazioni-2.7.0/src/redturtle/prenotazioni/profiles/default/registry/
+-rw-r--r--   0 lucabel    (501) staff       (20)     5140 2024-05-29 09:53:32.000000 redturtle.prenotazioni-2.7.0/src/redturtle/prenotazioni/profiles/default/registry/caching.xml
+-rw-r--r--   0 lucabel    (501) staff       (20)     2015 2024-05-29 09:53:32.000000 redturtle.prenotazioni-2.7.0/src/redturtle/prenotazioni/profiles/default/registry/resources.xml
+-rw-r--r--   0 lucabel    (501) staff       (20)     1001 2024-05-29 09:53:32.000000 redturtle.prenotazioni-2.7.0/src/redturtle/prenotazioni/profiles/default/registry/settings.xml
+-rw-r--r--   0 lucabel    (501) staff       (20)      251 2024-05-29 09:53:32.000000 redturtle.prenotazioni-2.7.0/src/redturtle/prenotazioni/profiles/default/repositorytool.xml
+-rw-r--r--   0 lucabel    (501) staff       (20)     3421 2024-05-29 09:53:32.000000 redturtle.prenotazioni-2.7.0/src/redturtle/prenotazioni/profiles/default/rolemap.xml
+-rw-r--r--   0 lucabel    (501) staff       (20)      277 2024-05-29 09:53:32.000000 redturtle.prenotazioni-2.7.0/src/redturtle/prenotazioni/profiles/default/sharing.xml
+drwxr-xr-x   0 lucabel    (501) staff       (20)        0 2024-05-29 09:53:33.594665 redturtle.prenotazioni-2.7.0/src/redturtle/prenotazioni/profiles/default/types/
+-rw-r--r--   0 lucabel    (501) staff       (20)     3565 2024-05-29 09:53:32.000000 redturtle.prenotazioni-2.7.0/src/redturtle/prenotazioni/profiles/default/types/Prenotazione.xml
+-rw-r--r--   0 lucabel    (501) staff       (20)     2983 2024-05-29 09:53:32.000000 redturtle.prenotazioni-2.7.0/src/redturtle/prenotazioni/profiles/default/types/PrenotazioneType.xml
+-rw-r--r--   0 lucabel    (501) staff       (20)     3861 2024-05-29 09:53:32.000000 redturtle.prenotazioni-2.7.0/src/redturtle/prenotazioni/profiles/default/types/PrenotazioniDay.xml
+-rw-r--r--   0 lucabel    (501) staff       (20)     3257 2024-05-29 09:53:32.000000 redturtle.prenotazioni-2.7.0/src/redturtle/prenotazioni/profiles/default/types/PrenotazioniFolder.xml
+-rw-r--r--   0 lucabel    (501) staff       (20)     3845 2024-05-29 09:53:32.000000 redturtle.prenotazioni-2.7.0/src/redturtle/prenotazioni/profiles/default/types/PrenotazioniWeek.xml
+-rw-r--r--   0 lucabel    (501) staff       (20)     3846 2024-05-29 09:53:32.000000 redturtle.prenotazioni-2.7.0/src/redturtle/prenotazioni/profiles/default/types/PrenotazioniYear.xml
+-rw-r--r--   0 lucabel    (501) staff       (20)      713 2024-05-29 09:53:32.000000 redturtle.prenotazioni-2.7.0/src/redturtle/prenotazioni/profiles/default/types.xml
+drwxr-xr-x   0 lucabel    (501) staff       (20)        0 2024-05-29 09:53:33.533509 redturtle.prenotazioni-2.7.0/src/redturtle/prenotazioni/profiles/default/workflows/
+drwxr-xr-x   0 lucabel    (501) staff       (20)        0 2024-05-29 09:53:33.594926 redturtle.prenotazioni-2.7.0/src/redturtle/prenotazioni/profiles/default/workflows/prenotazioni_workflow/
+-rw-r--r--   0 lucabel    (501) staff       (20)    12711 2024-05-29 09:53:32.000000 redturtle.prenotazioni-2.7.0/src/redturtle/prenotazioni/profiles/default/workflows/prenotazioni_workflow/definition.xml
+drwxr-xr-x   0 lucabel    (501) staff       (20)        0 2024-05-29 09:53:33.595273 redturtle.prenotazioni-2.7.0/src/redturtle/prenotazioni/profiles/default/workflows/prenotazionifolder_workflow/
+-rw-r--r--   0 lucabel    (501) staff       (20)     8877 2024-05-29 09:53:32.000000 redturtle.prenotazioni-2.7.0/src/redturtle/prenotazioni/profiles/default/workflows/prenotazionifolder_workflow/definition.xml
+-rw-r--r--   0 lucabel    (501) staff       (20)      613 2024-05-29 09:53:32.000000 redturtle.prenotazioni-2.7.0/src/redturtle/prenotazioni/profiles/default/workflows.xml
+drwxr-xr-x   0 lucabel    (501) staff       (20)        0 2024-05-29 09:53:33.595547 redturtle.prenotazioni-2.7.0/src/redturtle/prenotazioni/profiles/to_1402/
+-rw-r--r--   0 lucabel    (501) staff       (20)     1508 2024-05-29 09:53:32.000000 redturtle.prenotazioni-2.7.0/src/redturtle/prenotazioni/profiles/to_1402/contentrules.xml
+drwxr-xr-x   0 lucabel    (501) staff       (20)        0 2024-05-29 09:53:33.595812 redturtle.prenotazioni-2.7.0/src/redturtle/prenotazioni/profiles/to_1500/
+-rw-r--r--   0 lucabel    (501) staff       (20)      226 2024-05-29 09:53:32.000000 redturtle.prenotazioni-2.7.0/src/redturtle/prenotazioni/profiles/to_1500/types.xml
+drwxr-xr-x   0 lucabel    (501) staff       (20)        0 2024-05-29 09:53:33.596330 redturtle.prenotazioni-2.7.0/src/redturtle/prenotazioni/profiles/to_2005/
+-rw-r--r--   0 lucabel    (501) staff       (20)       88 2024-05-29 09:53:32.000000 redturtle.prenotazioni-2.7.0/src/redturtle/prenotazioni/profiles/to_2005/metadata.xml
+-rw-r--r--   0 lucabel    (501) staff       (20)      638 2024-05-29 09:53:32.000000 redturtle.prenotazioni-2.7.0/src/redturtle/prenotazioni/profiles/to_2005/rolemap.xml
+drwxr-xr-x   0 lucabel    (501) staff       (20)        0 2024-05-29 09:53:33.596950 redturtle.prenotazioni-2.7.0/src/redturtle/prenotazioni/profiles/to_2006/
+-rw-r--r--   0 lucabel    (501) staff       (20)       88 2024-05-29 09:53:32.000000 redturtle.prenotazioni-2.7.0/src/redturtle/prenotazioni/profiles/to_2006/metadata.xml
+drwxr-xr-x   0 lucabel    (501) staff       (20)        0 2024-05-29 09:53:33.534549 redturtle.prenotazioni-2.7.0/src/redturtle/prenotazioni/profiles/to_2006/workflows/
+drwxr-xr-x   0 lucabel    (501) staff       (20)        0 2024-05-29 09:53:33.597204 redturtle.prenotazioni-2.7.0/src/redturtle/prenotazioni/profiles/to_2006/workflows/prenotazioni_workflow/
+-rw-r--r--   0 lucabel    (501) staff       (20)    12711 2024-05-29 09:53:32.000000 redturtle.prenotazioni-2.7.0/src/redturtle/prenotazioni/profiles/to_2006/workflows/prenotazioni_workflow/definition.xml
+-rw-r--r--   0 lucabel    (501) staff       (20)      279 2024-05-29 09:53:32.000000 redturtle.prenotazioni-2.7.0/src/redturtle/prenotazioni/profiles/to_2006/workflows.xml
+drwxr-xr-x   0 lucabel    (501) staff       (20)        0 2024-05-29 09:53:33.597466 redturtle.prenotazioni-2.7.0/src/redturtle/prenotazioni/profiles/uninstall/
+-rw-r--r--   0 lucabel    (501) staff       (20)      125 2024-05-29 09:53:32.000000 redturtle.prenotazioni-2.7.0/src/redturtle/prenotazioni/profiles/uninstall/browserlayer.xml
+drwxr-xr-x   0 lucabel    (501) staff       (20)        0 2024-05-29 09:53:33.598172 redturtle.prenotazioni-2.7.0/src/redturtle/prenotazioni/profiles/uninstall/registry/
+-rw-r--r--   0 lucabel    (501) staff       (20)      431 2024-05-29 09:53:32.000000 redturtle.prenotazioni-2.7.0/src/redturtle/prenotazioni/profiles/uninstall/registry/resources.xml
+-rw-r--r--   0 lucabel    (501) staff       (20)      152 2024-05-29 09:53:32.000000 redturtle.prenotazioni-2.7.0/src/redturtle/prenotazioni/profiles/uninstall/registry/settings.xml
+drwxr-xr-x   0 lucabel    (501) staff       (20)        0 2024-05-29 09:53:33.598627 redturtle.prenotazioni-2.7.0/src/redturtle/prenotazioni/restapi/
+-rw-r--r--   0 lucabel    (501) staff       (20)        0 2024-05-29 09:53:32.000000 redturtle.prenotazioni-2.7.0/src/redturtle/prenotazioni/restapi/__init__.py
+-rw-r--r--   0 lucabel    (501) staff       (20)      199 2024-05-29 09:53:32.000000 redturtle.prenotazioni-2.7.0/src/redturtle/prenotazioni/restapi/configure.zcml
+drwxr-xr-x   0 lucabel    (501) staff       (20)        0 2024-05-29 09:53:33.599120 redturtle.prenotazioni-2.7.0/src/redturtle/prenotazioni/restapi/serializers/
+-rw-r--r--   0 lucabel    (501) staff       (20)        0 2024-05-29 09:53:32.000000 redturtle.prenotazioni-2.7.0/src/redturtle/prenotazioni/restapi/serializers/__init__.py
+drwxr-xr-x   0 lucabel    (501) staff       (20)        0 2024-05-29 09:53:33.600828 redturtle.prenotazioni-2.7.0/src/redturtle/prenotazioni/restapi/serializers/adapters/
+-rw-r--r--   0 lucabel    (501) staff       (20)        0 2024-05-29 09:53:32.000000 redturtle.prenotazioni-2.7.0/src/redturtle/prenotazioni/restapi/serializers/adapters/__init__.py
+-rw-r--r--   0 lucabel    (501) staff       (20)      468 2024-05-29 09:53:32.000000 redturtle.prenotazioni-2.7.0/src/redturtle/prenotazioni/restapi/serializers/adapters/configure.zcml
+-rw-r--r--   0 lucabel    (501) staff       (20)     7769 2024-05-29 09:53:32.000000 redturtle.prenotazioni-2.7.0/src/redturtle/prenotazioni/restapi/serializers/adapters/prenotazione.py
+-rw-r--r--   0 lucabel    (501) staff       (20)      973 2024-05-29 09:53:32.000000 redturtle.prenotazioni-2.7.0/src/redturtle/prenotazioni/restapi/serializers/adapters/prenotazione_type.py
+-rw-r--r--   0 lucabel    (501) staff       (20)      925 2024-05-29 09:53:32.000000 redturtle.prenotazioni-2.7.0/src/redturtle/prenotazioni/restapi/serializers/adapters/prenotazioni_folder.py
+-rw-r--r--   0 lucabel    (501) staff       (20)     1721 2024-05-29 09:53:32.000000 redturtle.prenotazioni-2.7.0/src/redturtle/prenotazioni/restapi/serializers/adapters/slot.py
+-rw-r--r--   0 lucabel    (501) staff       (20)      162 2024-05-29 09:53:32.000000 redturtle.prenotazioni-2.7.0/src/redturtle/prenotazioni/restapi/serializers/configure.zcml
+drwxr-xr-x   0 lucabel    (501) staff       (20)        0 2024-05-29 09:53:33.601081 redturtle.prenotazioni-2.7.0/src/redturtle/prenotazioni/restapi/services/
+drwxr-xr-x   0 lucabel    (501) staff       (20)        0 2024-05-29 09:53:33.601797 redturtle.prenotazioni-2.7.0/src/redturtle/prenotazioni/restapi/services/available_slots/
+-rw-r--r--   0 lucabel    (501) staff       (20)        0 2024-05-29 09:53:32.000000 redturtle.prenotazioni-2.7.0/src/redturtle/prenotazioni/restapi/services/available_slots/__init__.py
+-rw-r--r--   0 lucabel    (501) staff       (20)      352 2024-05-29 09:53:32.000000 redturtle.prenotazioni-2.7.0/src/redturtle/prenotazioni/restapi/services/available_slots/configure.zcml
+-rw-r--r--   0 lucabel    (501) staff       (20)     3734 2024-05-29 09:53:32.000000 redturtle.prenotazioni-2.7.0/src/redturtle/prenotazioni/restapi/services/available_slots/get.py
+drwxr-xr-x   0 lucabel    (501) staff       (20)        0 2024-05-29 09:53:33.603742 redturtle.prenotazioni-2.7.0/src/redturtle/prenotazioni/restapi/services/booking/
+-rw-r--r--   0 lucabel    (501) staff       (20)        0 2024-05-29 09:53:32.000000 redturtle.prenotazioni-2.7.0/src/redturtle/prenotazioni/restapi/services/booking/__init__.py
+-rw-r--r--   0 lucabel    (501) staff       (20)     6553 2024-05-29 09:53:32.000000 redturtle.prenotazioni-2.7.0/src/redturtle/prenotazioni/restapi/services/booking/add.py
+-rw-r--r--   0 lucabel    (501) staff       (20)     1641 2024-05-29 09:53:32.000000 redturtle.prenotazioni-2.7.0/src/redturtle/prenotazioni/restapi/services/booking/configure.zcml
+-rw-r--r--   0 lucabel    (501) staff       (20)     1209 2024-05-29 09:53:32.000000 redturtle.prenotazioni-2.7.0/src/redturtle/prenotazioni/restapi/services/booking/delete.py
+-rw-r--r--   0 lucabel    (501) staff       (20)     1166 2024-05-29 09:53:32.000000 redturtle.prenotazioni-2.7.0/src/redturtle/prenotazioni/restapi/services/booking/get.py
+-rw-r--r--   0 lucabel    (501) staff       (20)     1328 2024-05-29 09:53:32.000000 redturtle.prenotazioni-2.7.0/src/redturtle/prenotazioni/restapi/services/booking/move.py
+-rw-r--r--   0 lucabel    (501) staff       (20)     1152 2024-05-29 09:53:32.000000 redturtle.prenotazioni-2.7.0/src/redturtle/prenotazioni/restapi/services/booking/notify_about_confirm.py
+-rw-r--r--   0 lucabel    (501) staff       (20)      966 2024-05-29 09:53:32.000000 redturtle.prenotazioni-2.7.0/src/redturtle/prenotazioni/restapi/services/booking/vacation.py
+drwxr-xr-x   0 lucabel    (501) staff       (20)        0 2024-05-29 09:53:33.604515 redturtle.prenotazioni-2.7.0/src/redturtle/prenotazioni/restapi/services/booking_schema/
+-rw-r--r--   0 lucabel    (501) staff       (20)        0 2024-05-29 09:53:32.000000 redturtle.prenotazioni-2.7.0/src/redturtle/prenotazioni/restapi/services/booking_schema/__init__.py
+-rw-r--r--   0 lucabel    (501) staff       (20)      404 2024-05-29 09:53:32.000000 redturtle.prenotazioni-2.7.0/src/redturtle/prenotazioni/restapi/services/booking_schema/configure.zcml
+-rw-r--r--   0 lucabel    (501) staff       (20)     5395 2024-05-29 09:53:32.000000 redturtle.prenotazioni-2.7.0/src/redturtle/prenotazioni/restapi/services/booking_schema/get.py
+drwxr-xr-x   0 lucabel    (501) staff       (20)        0 2024-05-29 09:53:33.605376 redturtle.prenotazioni-2.7.0/src/redturtle/prenotazioni/restapi/services/bookings/
+-rw-r--r--   0 lucabel    (501) staff       (20)        0 2024-05-29 09:53:32.000000 redturtle.prenotazioni-2.7.0/src/redturtle/prenotazioni/restapi/services/bookings/__init__.py
+-rw-r--r--   0 lucabel    (501) staff       (20)      548 2024-05-29 09:53:32.000000 redturtle.prenotazioni-2.7.0/src/redturtle/prenotazioni/restapi/services/bookings/configure.zcml
+-rw-r--r--   0 lucabel    (501) staff       (20)     4137 2024-05-29 09:53:32.000000 redturtle.prenotazioni-2.7.0/src/redturtle/prenotazioni/restapi/services/bookings/search.py
+-rw-r--r--   0 lucabel    (501) staff       (20)      336 2024-05-29 09:53:32.000000 redturtle.prenotazioni-2.7.0/src/redturtle/prenotazioni/restapi/services/configure.zcml
+drwxr-xr-x   0 lucabel    (501) staff       (20)        0 2024-05-29 09:53:33.606123 redturtle.prenotazioni-2.7.0/src/redturtle/prenotazioni/restapi/services/day/
+-rw-r--r--   0 lucabel    (501) staff       (20)        0 2024-05-29 09:53:32.000000 redturtle.prenotazioni-2.7.0/src/redturtle/prenotazioni/restapi/services/day/__init__.py
+-rw-r--r--   0 lucabel    (501) staff       (20)      365 2024-05-29 09:53:32.000000 redturtle.prenotazioni-2.7.0/src/redturtle/prenotazioni/restapi/services/day/configure.zcml
+-rw-r--r--   0 lucabel    (501) staff       (20)     6732 2024-05-29 09:53:32.000000 redturtle.prenotazioni-2.7.0/src/redturtle/prenotazioni/restapi/services/day/day.py
+drwxr-xr-x   0 lucabel    (501) staff       (20)        0 2024-05-29 09:53:33.606821 redturtle.prenotazioni-2.7.0/src/redturtle/prenotazioni/restapi/services/types/
+-rw-r--r--   0 lucabel    (501) staff       (20)        0 2024-05-29 09:53:32.000000 redturtle.prenotazioni-2.7.0/src/redturtle/prenotazioni/restapi/services/types/__init__.py
+-rw-r--r--   0 lucabel    (501) staff       (20)      216 2024-05-29 09:53:32.000000 redturtle.prenotazioni-2.7.0/src/redturtle/prenotazioni/restapi/services/types/configure.zcml
+-rw-r--r--   0 lucabel    (501) staff       (20)      915 2024-05-29 09:53:32.000000 redturtle.prenotazioni-2.7.0/src/redturtle/prenotazioni/restapi/services/types/get.py
+drwxr-xr-x   0 lucabel    (501) staff       (20)        0 2024-05-29 09:53:33.607264 redturtle.prenotazioni-2.7.0/src/redturtle/prenotazioni/scripts/
+-rw-r--r--   0 lucabel    (501) staff       (20)        0 2024-05-29 09:53:32.000000 redturtle.prenotazioni-2.7.0/src/redturtle/prenotazioni/scripts/__init__.py
+-rw-r--r--   0 lucabel    (501) staff       (20)      525 2024-05-29 09:53:32.000000 redturtle.prenotazioni-2.7.0/src/redturtle/prenotazioni/scripts/notify_upcoming_bookings.py
+-rw-r--r--   0 lucabel    (501) staff       (20)     1062 2024-05-29 09:53:32.000000 redturtle.prenotazioni-2.7.0/src/redturtle/prenotazioni/setuphandlers.py
+-rw-r--r--   0 lucabel    (501) staff       (20)     3443 2024-05-29 09:53:32.000000 redturtle.prenotazioni-2.7.0/src/redturtle/prenotazioni/testing.py
+drwxr-xr-x   0 lucabel    (501) staff       (20)        0 2024-05-29 09:53:33.616875 redturtle.prenotazioni-2.7.0/src/redturtle/prenotazioni/tests/
+-rw-r--r--   0 lucabel    (501) staff       (20)      105 2024-05-29 09:53:32.000000 redturtle.prenotazioni-2.7.0/src/redturtle/prenotazioni/tests/__init__.py
+-rw-r--r--   0 lucabel    (501) staff       (20)     1223 2024-05-29 09:53:32.000000 redturtle.prenotazioni-2.7.0/src/redturtle/prenotazioni/tests/helpers.py
+-rw-r--r--   0 lucabel    (501) staff       (20)     3222 2024-05-29 09:53:32.000000 redturtle.prenotazioni-2.7.0/src/redturtle/prenotazioni/tests/test_add_block.py
+-rw-r--r--   0 lucabel    (501) staff       (20)    25000 2024-05-29 09:53:32.000000 redturtle.prenotazioni-2.7.0/src/redturtle/prenotazioni/tests/test_add_booking.py
+-rw-r--r--   0 lucabel    (501) staff       (20)     1980 2024-05-29 09:53:32.000000 redturtle.prenotazioni-2.7.0/src/redturtle/prenotazioni/tests/test_add_booking_type.py
+-rw-r--r--   0 lucabel    (501) staff       (20)    17450 2024-05-29 09:53:32.000000 redturtle.prenotazioni-2.7.0/src/redturtle/prenotazioni/tests/test_available_slots.py
+-rw-r--r--   0 lucabel    (501) staff       (20)     2011 2024-05-29 09:53:32.000000 redturtle.prenotazioni-2.7.0/src/redturtle/prenotazioni/tests/test_base_slot.py
+-rw-r--r--   0 lucabel    (501) staff       (20)     4387 2024-05-29 09:53:32.000000 redturtle.prenotazioni-2.7.0/src/redturtle/prenotazioni/tests/test_booker_choose_available_slot.py
+-rw-r--r--   0 lucabel    (501) staff       (20)     6402 2024-05-29 09:53:32.000000 redturtle.prenotazioni-2.7.0/src/redturtle/prenotazioni/tests/test_booking_info.py
+-rw-r--r--   0 lucabel    (501) staff       (20)     6901 2024-05-29 09:53:32.000000 redturtle.prenotazioni-2.7.0/src/redturtle/prenotazioni/tests/test_booking_notify.py
+-rw-r--r--   0 lucabel    (501) staff       (20)     8748 2024-05-29 09:53:32.000000 redturtle.prenotazioni-2.7.0/src/redturtle/prenotazioni/tests/test_booking_schema.py
+-rw-r--r--   0 lucabel    (501) staff       (20)     8696 2024-05-29 09:53:32.000000 redturtle.prenotazioni-2.7.0/src/redturtle/prenotazioni/tests/test_bookings_num_limit.py
+-rw-r--r--   0 lucabel    (501) staff       (20)     6036 2024-05-29 09:53:32.000000 redturtle.prenotazioni-2.7.0/src/redturtle/prenotazioni/tests/test_browser_utilities_notify_upcoming_bookings.py
+-rw-r--r--   0 lucabel    (501) staff       (20)     3088 2024-05-29 09:53:32.000000 redturtle.prenotazioni-2.7.0/src/redturtle/prenotazioni/tests/test_content_validators_validate_pause_table.py
+-rw-r--r--   0 lucabel    (501) staff       (20)     6317 2024-05-29 09:53:32.000000 redturtle.prenotazioni-2.7.0/src/redturtle/prenotazioni/tests/test_day.py
+-rw-r--r--   0 lucabel    (501) staff       (20)    10871 2024-05-29 09:53:32.000000 redturtle.prenotazioni-2.7.0/src/redturtle/prenotazioni/tests/test_delete_booking.py
+-rw-r--r--   0 lucabel    (501) staff       (20)    10361 2024-05-29 09:53:32.000000 redturtle.prenotazioni-2.7.0/src/redturtle/prenotazioni/tests/test_delete_booking_api.py
+-rw-r--r--   0 lucabel    (501) staff       (20)     4000 2024-05-29 09:53:32.000000 redturtle.prenotazioni-2.7.0/src/redturtle/prenotazioni/tests/test_gates_overrides.py
+-rw-r--r--   0 lucabel    (501) staff       (20)     8161 2024-05-29 09:53:32.000000 redturtle.prenotazioni-2.7.0/src/redturtle/prenotazioni/tests/test_move_booking_api.py
+-rw-r--r--   0 lucabel    (501) staff       (20)     5216 2024-05-29 09:53:32.000000 redturtle.prenotazioni-2.7.0/src/redturtle/prenotazioni/tests/test_notification_supervisor_utility.py
+-rw-r--r--   0 lucabel    (501) staff       (20)     3591 2024-05-29 09:53:32.000000 redturtle.prenotazioni-2.7.0/src/redturtle/prenotazioni/tests/test_notify_the_message_failure.py
+-rw-r--r--   0 lucabel    (501) staff       (20)    14545 2024-05-29 09:53:32.000000 redturtle.prenotazioni-2.7.0/src/redturtle/prenotazioni/tests/test_pauses_overrides.py
+-rw-r--r--   0 lucabel    (501) staff       (20)     5029 2024-05-29 09:53:32.000000 redturtle.prenotazioni-2.7.0/src/redturtle/prenotazioni/tests/test_prenotazione_email_sent_to_managers.py
+-rw-r--r--   0 lucabel    (501) staff       (20)    15081 2024-05-29 09:53:32.000000 redturtle.prenotazioni-2.7.0/src/redturtle/prenotazioni/tests/test_prenotazione_events.py
+-rw-r--r--   0 lucabel    (501) staff       (20)     4861 2024-05-29 09:53:32.000000 redturtle.prenotazioni-2.7.0/src/redturtle/prenotazioni/tests/test_prenotazione_searchable_item_serializer.py
+-rw-r--r--   0 lucabel    (501) staff       (20)     7049 2024-05-29 09:53:32.000000 redturtle.prenotazioni-2.7.0/src/redturtle/prenotazioni/tests/test_prenotazioni_context_state.py
+-rw-r--r--   0 lucabel    (501) staff       (20)      740 2024-05-29 09:53:32.000000 redturtle.prenotazioni-2.7.0/src/redturtle/prenotazioni/tests/test_prenotazioni_folder_holidays_constraint.py
+-rw-r--r--   0 lucabel    (501) staff       (20)    19833 2024-05-29 09:53:32.000000 redturtle.prenotazioni-2.7.0/src/redturtle/prenotazioni/tests/test_prenotazioni_search.py
+-rw-r--r--   0 lucabel    (501) staff       (20)     2485 2024-05-29 09:53:32.000000 redturtle.prenotazioni-2.7.0/src/redturtle/prenotazioni/tests/test_restapi_types_override.py
+-rw-r--r--   0 lucabel    (501) staff       (20)     9722 2024-05-29 09:53:32.000000 redturtle.prenotazioni-2.7.0/src/redturtle/prenotazioni/tests/test_send_ical.py
+-rw-r--r--   0 lucabel    (501) staff       (20)     4180 2024-05-29 09:53:32.000000 redturtle.prenotazioni-2.7.0/src/redturtle/prenotazioni/tests/test_setup.py
+-rw-r--r--   0 lucabel    (501) staff       (20)     3046 2024-05-29 09:53:32.000000 redturtle.prenotazioni-2.7.0/src/redturtle/prenotazioni/tests/test_stringinterp.py
+-rw-r--r--   0 lucabel    (501) staff       (20)      905 2024-05-29 09:53:32.000000 redturtle.prenotazioni-2.7.0/src/redturtle/prenotazioni/tests/test_utils.py
+-rw-r--r--   0 lucabel    (501) staff       (20)     6486 2024-05-29 09:53:32.000000 redturtle.prenotazioni-2.7.0/src/redturtle/prenotazioni/tests/test_vacation_api.py
+-rw-r--r--   0 lucabel    (501) staff       (20)     1198 2024-05-29 09:53:32.000000 redturtle.prenotazioni-2.7.0/src/redturtle/prenotazioni/tests/test_validate_max_bookings_allowed.py
+-rw-r--r--   0 lucabel    (501) staff       (20)     2349 2024-05-29 09:53:32.000000 redturtle.prenotazioni-2.7.0/src/redturtle/prenotazioni/tests/test_vocabularies.py
+-rw-r--r--   0 lucabel    (501) staff       (20)    23517 2024-05-29 09:53:32.000000 redturtle.prenotazioni-2.7.0/src/redturtle/prenotazioni/tests/test_week_table_overrides.py
+-rw-r--r--   0 lucabel    (501) staff       (20)    16971 2024-05-29 09:53:32.000000 redturtle.prenotazioni-2.7.0/src/redturtle/prenotazioni/upgrades.py
+-rw-r--r--   0 lucabel    (501) staff       (20)    10649 2024-05-29 09:53:32.000000 redturtle.prenotazioni-2.7.0/src/redturtle/prenotazioni/upgrades.zcml
+drwxr-xr-x   0 lucabel    (501) staff       (20)        0 2024-05-29 09:53:33.618296 redturtle.prenotazioni-2.7.0/src/redturtle/prenotazioni/utilities/
+-rw-r--r--   0 lucabel    (501) staff       (20)       94 2024-05-29 09:53:32.000000 redturtle.prenotazioni-2.7.0/src/redturtle/prenotazioni/utilities/__init__.py
+-rw-r--r--   0 lucabel    (501) staff       (20)     2900 2024-05-29 09:53:32.000000 redturtle.prenotazioni-2.7.0/src/redturtle/prenotazioni/utilities/dateutils.py
+-rw-r--r--   0 lucabel    (501) staff       (20)      489 2024-05-29 09:53:32.000000 redturtle.prenotazioni-2.7.0/src/redturtle/prenotazioni/utilities/email.py
+-rw-r--r--   0 lucabel    (501) staff       (20)      549 2024-05-29 09:53:32.000000 redturtle.prenotazioni-2.7.0/src/redturtle/prenotazioni/utilities/log_errors.py
+-rw-r--r--   0 lucabel    (501) staff       (20)     1118 2024-05-29 09:53:32.000000 redturtle.prenotazioni-2.7.0/src/redturtle/prenotazioni/utilities/urls.py
+drwxr-xr-x   0 lucabel    (501) staff       (20)        0 2024-05-29 09:53:33.618836 redturtle.prenotazioni-2.7.0/src/redturtle/prenotazioni/utils/
+-rw-r--r--   0 lucabel    (501) staff       (20)       67 2024-05-29 09:53:32.000000 redturtle.prenotazioni-2.7.0/src/redturtle/prenotazioni/utils/__init__.py
+-rw-r--r--   0 lucabel    (501) staff       (20)      597 2024-05-29 09:53:32.000000 redturtle.prenotazioni-2.7.0/src/redturtle/prenotazioni/utils/get_prenotazioni_folder.py
+drwxr-xr-x   0 lucabel    (501) staff       (20)        0 2024-05-29 09:53:33.621628 redturtle.prenotazioni-2.7.0/src/redturtle/prenotazioni/vocabularies/
+-rw-r--r--   0 lucabel    (501) staff       (20)       24 2024-05-29 09:53:32.000000 redturtle.prenotazioni-2.7.0/src/redturtle/prenotazioni/vocabularies/__init__.py
+-rw-r--r--   0 lucabel    (501) staff       (20)     1444 2024-05-29 09:53:32.000000 redturtle.prenotazioni-2.7.0/src/redturtle/prenotazioni/vocabularies/configure.zcml
+-rw-r--r--   0 lucabel    (501) staff       (20)      607 2024-05-29 09:53:32.000000 redturtle.prenotazioni-2.7.0/src/redturtle/prenotazioni/vocabularies/gates.py
+-rw-r--r--   0 lucabel    (501) staff       (20)     1011 2024-05-29 09:53:32.000000 redturtle.prenotazioni-2.7.0/src/redturtle/prenotazioni/vocabularies/requirable_booking_fields.py
+-rw-r--r--   0 lucabel    (501) staff       (20)      598 2024-05-29 09:53:32.000000 redturtle.prenotazioni-2.7.0/src/redturtle/prenotazioni/vocabularies/review_states.py
+-rw-r--r--   0 lucabel    (501) staff       (20)     1814 2024-05-29 09:53:32.000000 redturtle.prenotazioni-2.7.0/src/redturtle/prenotazioni/vocabularies/tipologies.py
+-rw-r--r--   0 lucabel    (501) staff       (20)      776 2024-05-29 09:53:32.000000 redturtle.prenotazioni-2.7.0/src/redturtle/prenotazioni/vocabularies/voc_booking_type_gates.py
+-rw-r--r--   0 lucabel    (501) staff       (20)     1128 2024-05-29 09:53:32.000000 redturtle.prenotazioni-2.7.0/src/redturtle/prenotazioni/vocabularies/voc_durata_incontro.py
+-rw-r--r--   0 lucabel    (501) staff       (20)     2549 2024-05-29 09:53:32.000000 redturtle.prenotazioni-2.7.0/src/redturtle/prenotazioni/vocabularies/voc_months.py
+-rw-r--r--   0 lucabel    (501) staff       (20)     1367 2024-05-29 09:53:32.000000 redturtle.prenotazioni-2.7.0/src/redturtle/prenotazioni/vocabularies/voc_ore_inizio.py
+-rw-r--r--   0 lucabel    (501) staff       (20)      440 2024-05-29 09:53:32.000000 redturtle.prenotazioni-2.7.0/src/redturtle/prenotazioni/vocabularies/voc_pause_scheduler.py
+drwxr-xr-x   0 lucabel    (501) staff       (20)        0 2024-05-29 09:53:33.545560 redturtle.prenotazioni-2.7.0/src/redturtle.prenotazioni.egg-info/
+-rw-r--r--   0 lucabel    (501) staff       (20)    47127 2024-05-29 09:53:33.000000 redturtle.prenotazioni-2.7.0/src/redturtle.prenotazioni.egg-info/PKG-INFO
+-rw-r--r--   0 lucabel    (501) staff       (20)    17737 2024-05-29 09:53:33.000000 redturtle.prenotazioni-2.7.0/src/redturtle.prenotazioni.egg-info/SOURCES.txt
+-rw-r--r--   0 lucabel    (501) staff       (20)        1 2024-05-29 09:53:33.000000 redturtle.prenotazioni-2.7.0/src/redturtle.prenotazioni.egg-info/dependency_links.txt
+-rw-r--r--   0 lucabel    (501) staff       (20)      267 2024-05-29 09:53:33.000000 redturtle.prenotazioni-2.7.0/src/redturtle.prenotazioni.egg-info/entry_points.txt
+-rw-r--r--   0 lucabel    (501) staff       (20)       10 2024-05-29 09:53:33.000000 redturtle.prenotazioni-2.7.0/src/redturtle.prenotazioni.egg-info/namespace_packages.txt
+-rw-r--r--   0 lucabel    (501) staff       (20)        1 2024-05-29 09:53:33.000000 redturtle.prenotazioni-2.7.0/src/redturtle.prenotazioni.egg-info/not-zip-safe
+-rw-r--r--   0 lucabel    (501) staff       (20)      425 2024-05-29 09:53:33.000000 redturtle.prenotazioni-2.7.0/src/redturtle.prenotazioni.egg-info/requires.txt
+-rw-r--r--   0 lucabel    (501) staff       (20)       10 2024-05-29 09:53:33.000000 redturtle.prenotazioni-2.7.0/src/redturtle.prenotazioni.egg-info/top_level.txt
```

### Comparing `redturtle.prenotazioni-2.6.5/APP_IO.txt` & `redturtle.prenotazioni-2.7.0/APP_IO.txt`

 * *Files identical despite different names*

### Comparing `redturtle.prenotazioni-2.6.5/CHANGES.rst` & `redturtle.prenotazioni-2.7.0/CHANGES.rst`

 * *Files 2% similar despite different names*

```diff
@@ -1,11 +1,31 @@
 Changelog
 =========
 
 
+2.7.0 (2024-05-29)
+------------------
+
+- Workarounds for external integration: search with tinit- prefixed user,
+  schema with some fields with only spaces
+  [mamico]
+
+- Write to history the booking notifications log
+  [folix-01]
+
+- Write to history if could not send booking notification
+  [folix-01]
+
+- Booking canceled message + wf states translations
+  BREAKING CHANGE: frontend uses booking_state_label insteat of booking_state, this change of translations
+  requires a new release of the frontend (@redturtle/volto-io-prenoto >= 1.20.0)
+  [folix-01]
+
+
+
 2.6.5 (2024-04-24)
 ------------------
 
 - Package chore.
   [folix-01]
```

### Comparing `redturtle.prenotazioni-2.6.5/DEVELOP.rst` & `redturtle.prenotazioni-2.7.0/DEVELOP.rst`

 * *Files identical despite different names*

### Comparing `redturtle.prenotazioni-2.6.5/LICENSE.GPL` & `redturtle.prenotazioni-2.7.0/LICENSE.GPL`

 * *Files identical despite different names*

### Comparing `redturtle.prenotazioni-2.6.5/LICENSE.rst` & `redturtle.prenotazioni-2.7.0/LICENSE.rst`

 * *Files identical despite different names*

### Comparing `redturtle.prenotazioni-2.6.5/README.rst` & `redturtle.prenotazioni-2.7.0/README.rst`

 * *Files identical despite different names*

### Comparing `redturtle.prenotazioni-2.6.5/docs/conf.py` & `redturtle.prenotazioni-2.7.0/docs/conf.py`

 * *Files identical despite different names*

### Comparing `redturtle.prenotazioni-2.6.5/setup.py` & `redturtle.prenotazioni-2.7.0/setup.py`

 * *Files 0% similar despite different names*

```diff
@@ -11,15 +11,15 @@
         open("CHANGES.rst").read(),
     ]
 )
 
 
 setup(
     name="redturtle.prenotazioni",
-    version="2.6.5",
+    version="2.7.0",
     description="An add-on for Plone",
     long_description=long_description,
     # Get more from https://pypi.python.org/pypi?%3Aaction=list_classifiers
     classifiers=[
         "Development Status :: 5 - Production/Stable",
         "Environment :: Web Environment",
         "Framework :: Plone",
```

### Comparing `redturtle.prenotazioni-2.6.5/src/redturtle/prenotazioni/__init__.py` & `redturtle.prenotazioni-2.7.0/src/redturtle/prenotazioni/__init__.py`

 * *Files identical despite different names*

### Comparing `redturtle.prenotazioni-2.6.5/src/redturtle/prenotazioni/actions/mail.py` & `redturtle.prenotazioni-2.7.0/src/redturtle/prenotazioni/actions/mail.py`

 * *Files identical despite different names*

### Comparing `redturtle.prenotazioni-2.6.5/src/redturtle/prenotazioni/adapters/booker.py` & `redturtle.prenotazioni-2.7.0/src/redturtle/prenotazioni/adapters/booker.py`

 * *Files identical despite different names*

### Comparing `redturtle.prenotazioni-2.6.5/src/redturtle/prenotazioni/adapters/booking_code.py` & `redturtle.prenotazioni-2.7.0/src/redturtle/prenotazioni/adapters/booking_code.py`

 * *Files identical despite different names*

### Comparing `redturtle.prenotazioni-2.6.5/src/redturtle/prenotazioni/adapters/configure.zcml` & `redturtle.prenotazioni-2.7.0/src/redturtle/prenotazioni/adapters/configure.zcml`

 * *Files identical despite different names*

### Comparing `redturtle.prenotazioni-2.6.5/src/redturtle/prenotazioni/adapters/conflict.py` & `redturtle.prenotazioni-2.7.0/src/redturtle/prenotazioni/adapters/conflict.py`

 * *Files identical despite different names*

### Comparing `redturtle.prenotazioni-2.6.5/src/redturtle/prenotazioni/adapters/ical.py` & `redturtle.prenotazioni-2.7.0/src/redturtle/prenotazioni/adapters/ical.py`

 * *Files 3% similar despite different names*

```diff
@@ -61,15 +61,15 @@
 
     @property
     def dtend(self):
         return {"value": self.context.booking_expiration_date}
 
     @property
     def summary(self):
-        # XXX: `self.context.translate` raise Unauthorized exception
+        # XXX: `api.portal.translate` raise Unauthorized exception
         # Module Products.PythonScripts.PythonScript, line 338, in _exec
         # Module script, line 19, in translate
         # <FSPythonScript at /Plone/cartella-prenotazioni/2023/37/1//translate>
         # Line 19
         # Module Products.CMFPlone.TranslationServiceTool, line 47, in translate
         # Module Shared.DC.Scripts.Bindings, line 199, in __getattr__
         # Module Shared.DC.Scripts.Bindings, line 205, in __you_lose
```

### Comparing `redturtle.prenotazioni-2.6.5/src/redturtle/prenotazioni/adapters/slot.py` & `redturtle.prenotazioni-2.7.0/src/redturtle/prenotazioni/adapters/slot.py`

 * *Files identical despite different names*

### Comparing `redturtle.prenotazioni-2.6.5/src/redturtle/prenotazioni/adapters/stringinterp.py` & `redturtle.prenotazioni-2.7.0/src/redturtle/prenotazioni/adapters/stringinterp.py`

 * *Files identical despite different names*

### Comparing `redturtle.prenotazioni-2.6.5/src/redturtle/prenotazioni/behaviors/booking_folder/configure.zcml` & `redturtle.prenotazioni-2.7.0/src/redturtle/prenotazioni/behaviors/booking_folder/configure.zcml`

 * *Files identical despite different names*

### Comparing `redturtle.prenotazioni-2.6.5/src/redturtle/prenotazioni/behaviors/booking_folder/contacts.py` & `redturtle.prenotazioni-2.7.0/src/redturtle/prenotazioni/behaviors/booking_folder/contacts.py`

 * *Files identical despite different names*

### Comparing `redturtle.prenotazioni-2.6.5/src/redturtle/prenotazioni/behaviors/booking_folder/notifications/appio/__init__.py` & `redturtle.prenotazioni-2.7.0/src/redturtle/prenotazioni/behaviors/booking_folder/notifications/email/__init__.py`

 * *Files 10% similar despite different names*

```diff
@@ -9,300 +9,331 @@
 from zope.interface import provider
 from zope.schema.interfaces import IContextAwareDefaultFactory
 
 from redturtle.prenotazioni import _
 
 
 @provider(IContextAwareDefaultFactory)
-def notify_on_submit_appio_subject_default_factory(context):
+def notify_on_submit_subject_default_factory(context):
     return api.portal.translate(
         _(
-            "notify_on_submit_appio_subject_default_value",
+            "notify_on_submit_subject_default_value",
             "[${prenotazioni_folder_title}] Booking created",
         )
     )
 
 
 @provider(IContextAwareDefaultFactory)
-def notify_on_submit_appio_message_default_factory(context):
+def notify_on_submit_message_default_factory(context):
     return api.portal.translate(
         _(
-            "notify_on_submit_appio_message_default_value",
-            "Booking ${booking_type} for ${booking_date} at ${booking_time} has been created.<br/><br/>You can see details and print a reminder following this [${booking_print_url}](link).",
+            "notify_on_submit_message_default_value",
+            "Booking ${booking_type} for ${booking_date} at ${booking_time} has been created.<br/><br/>You can see details and print a reminder following this <a href=${booking_print_url}>link</a>.",
         )
     )
 
 
 @provider(IContextAwareDefaultFactory)
-def notify_on_confirm_appio_subject_default_factory(context):
+def notify_on_confirm_subject_default_factory(context):
     return api.portal.translate(
         _(
-            "notify_on_confirm_appio_subject_default_value",
+            "notify_on_confirm_subject_default_value",
             "[${prenotazioni_folder_title}] Booking of ${booking_date} at ${booking_time} was accepted",
         )
     )
 
 
 @provider(IContextAwareDefaultFactory)
-def notify_on_confirm_appio_message_default_factory(context):
+def notify_on_confirm_message_default_factory(context):
     return api.portal.translate(
         _(
-            "notify_on_confirm_appio_message_default_value",
+            "notify_on_confirm_message_default_value",
             "The booking ${booking_type} for ${title} has been confirmed."
-            "<br/><br/>You can see details and print a reminder following this [link](${booking_print_url}).",
+            "<br/><br/>You can see details and print a reminder following this <a href=${booking_print_url}>link</a>.",
         )
     )
 
 
 @provider(IContextAwareDefaultFactory)
-def notify_on_move_appio_subject_default_factory(context):
+def notify_on_move_subject_default_factory(context):
     return api.portal.translate(
         _(
-            "notify_on_move_appio_subject_default_value",
+            "notify_on_move_subject_default_value",
             "[${prenotazioni_folder_title}] Booking date modified for ${title}",
         )
     )
 
 
 @provider(IContextAwareDefaultFactory)
-def notify_on_move_appio_message_default_factory(context):
+def notify_on_move_message_default_factory(context):
     return api.portal.translate(
         _(
-            "notify_on_move_appio_message_default_value",
+            "notify_on_move_message_default_value",
             "The booking scheduling for ${booking_type} was modified."
             "<br/><br/>The new one is on ${booking_date} at ${booking_time}."
-            "<br/><br/>You can see details and print a reminder following this [link](${booking_print_url}).",
+            "<br/><br/>You can see details and print a reminder following this <a href=${booking_print_url}>link</a>.",
         )
     )
 
 
 @provider(IContextAwareDefaultFactory)
-def notify_on_refuse_appio_subject_default_factory(context):
+def notify_on_refuse_subject_default_factory(context):
     return api.portal.translate(
         _(
-            "notify_on_refuse_appio_subject_default_value",
+            "notify_on_refuse_subject_default_value",
             "[${prenotazioni_folder_title}] Booking refused for ${title}",
         )
     )
 
 
 @provider(IContextAwareDefaultFactory)
-def notify_on_refuse_appio_message_default_factory(context):
+def notify_on_refuse_message_default_factory(context):
     return api.portal.translate(
         _(
-            "notify_on_refuse_appio_message_default_value",
+            "notify_on_refuse_message_default_value",
             "The booking ${booking_type} of ${booking_date} at ${booking_time} was refused.",
         )
     )
 
 
 @provider(IContextAwareDefaultFactory)
-def notify_as_reminder_appio_subject_default_factory(context):
+def notify_on_cancel_subject_default_factory(context):
     return api.portal.translate(
         _(
-            "notify_as_reminder_appio_subject_default_value",
+            "notify_on_cancel_subject_default_value",
+            "[${prenotazioni_folder_title}] Booking canceled for ${title}",
+        )
+    )
+
+
+@provider(IContextAwareDefaultFactory)
+def notify_on_cancel_message_default_factory(context):
+    return api.portal.translate(
+        _(
+            "notify_on_cancel_message_default_value",
+            "The booking ${booking_type} of ${booking_date} at ${booking_time} was canceled.",
+        )
+    )
+
+
+@provider(IContextAwareDefaultFactory)
+def notify_as_reminder_subject_default_factory(context):
+    return api.portal.translate(
+        _(
+            "notify_as_reminder_subject_default_value",
             "[${prenotazioni_folder_title}] Booking reminder on ${booking_date}",
         )
     )
 
 
 @provider(IContextAwareDefaultFactory)
-def notify_as_reminder_appio_message_default_factory(context):
+def notify_as_reminder_message_default_factory(context):
     return api.portal.translate(
         _(
-            "notify_as_reminder_appio_message_default_value",
+            "notify_as_reminder_message_default_value",
             "This is an automatic reminder about your booking on ${date} for ${booking_type}."
-            "<br/><br/>You can see details and print a reminder following this [link](${booking_print_url}).",
+            "<br/><br/>You can see details and print a reminder following this <a href=${booking_print_url}>link</a>.",
         )
     )
 
 
 @provider(IFormFieldProvider)
-class INotificationAppIO(model.Schema):
-    notifications_appio_enabled = schema.Bool(
-        title=_("notifications_appio_enabled_label", default="AppIO notifications"),
+class INotificationEmail(model.Schema):
+    notifications_email_enabled = schema.Bool(
+        title=_("notifications_email_enabled_label", default="Email notifications"),
         description=_(
-            "notifications_appio_enabled_help",
-            default="Enable AppIO notifications.",
+            "notifications_email_enabled_help",
+            default="Enable Email notifications.",
         ),
-        default=False,
+        default=True,
         required=False,
     )
-    notify_on_submit_appio_subject = schema.TextLine(
+    email_from = schema.TextLine(
+        title=_("Email from"),
+        description=_(
+            'Insert an email address used as "from" in email notifications. '
+            "Leave empty to use the default from set in the site configuration."
+        ),
+        required=False,
+        default="",
+    )
+    notify_on_submit_subject = schema.TextLine(
         title=_(
             "notify_on_submit_subject",
             default="[Created] subject",
         ),
         description=_(
             "notify_on_submit_subject_help",
             default="The message subject when a booking has been created.",
         ),
-        defaultFactory=notify_on_submit_appio_subject_default_factory,
+        defaultFactory=notify_on_submit_subject_default_factory,
         required=False,
     )
-    notify_on_submit_appio_message = schema.Text(
+    notify_on_submit_message = schema.Text(
         title=_(
             "notify_on_submit_message",
             default="[Created] message",
         ),
         description=_(
             "notify_on_submit_message_help",
             default="The message text when a booking has been created.",
         ),
-        defaultFactory=notify_on_submit_appio_message_default_factory,
+        defaultFactory=notify_on_submit_message_default_factory,
         required=False,
     )
-    notify_on_confirm_appio_subject = schema.Text(
+    notify_on_confirm_subject = schema.TextLine(
         title=_(
             "notify_on_confirm_subject",
             default="[Confirm] subject",
         ),
         description=_(
             "notify_on_confirm_subject_help",
             default="The message subject when a booking has been confirmed.",
         ),
-        defaultFactory=notify_on_confirm_appio_subject_default_factory,
+        defaultFactory=notify_on_confirm_subject_default_factory,
         required=False,
     )
-    notify_on_confirm_appio_message = schema.Text(
+    notify_on_confirm_message = schema.Text(
         title=_(
             "notify_on_confirm_message",
             default="[Confirmed] message",
         ),
         description=_(
             "notify_on_confirm_message_help",
             default="The message text when a booking has been confirmed.",
         ),
-        defaultFactory=notify_on_confirm_appio_message_default_factory,
+        defaultFactory=notify_on_confirm_message_default_factory,
         required=False,
     )
-    notify_on_move_appio_subject = schema.Text(
+    notify_on_move_subject = schema.TextLine(
         title=_(
             "notify_on_move_subject",
             default="[Move] subject",
         ),
         description=_(
             "notify_on_move_subject_help",
             default="The message subject when a booking has been moved.",
         ),
-        defaultFactory=notify_on_move_appio_subject_default_factory,
+        defaultFactory=notify_on_move_subject_default_factory,
         required=False,
     )
-    notify_on_move_appio_message = schema.Text(
+    notify_on_move_message = schema.Text(
         title=_(
             "notify_on_move_message",
             default="[Move] message",
         ),
         description=_(
             "notify_on_move_message_help",
             default="The message text when a booking has been moved.",
         ),
-        defaultFactory=notify_on_move_appio_message_default_factory,
+        defaultFactory=notify_on_move_message_default_factory,
         required=False,
     )
-    notify_on_refuse_appio_subject = schema.Text(
+    notify_on_refuse_subject = schema.TextLine(
         title=_(
             "notify_on_refuse_subject",
             default="[Refuse] subject",
         ),
         description=_(
             "notify_on_refuse_subject_help",
             default="The message subject when a booking has been refused.",
         ),
-        defaultFactory=notify_on_refuse_appio_subject_default_factory,
+        defaultFactory=notify_on_refuse_subject_default_factory,
         required=False,
     )
-    notify_on_refuse_appio_message = schema.Text(
+    notify_on_refuse_message = schema.Text(
         title=_(
             "notify_on_refuse_message",
             default="[Refuse] message",
         ),
         description=_(
             "notify_on_refuse_message_help",
             default="The message text when a booking has been refused.",
         ),
-        defaultFactory=notify_on_refuse_appio_message_default_factory,
+        defaultFactory=notify_on_refuse_message_default_factory,
+        required=False,
+    )
+    notify_on_cancel_subject = schema.TextLine(
+        title=_(
+            "notify_on_cancel_subject",
+            default="[Cancel] subject",
+        ),
+        description=_(
+            "notify_on_cancel_subject_help",
+            default="The message subject when a booking has been canceled.",
+        ),
+        defaultFactory=notify_on_cancel_subject_default_factory,
+        required=False,
+    )
+    notify_on_cancel_message = schema.Text(
+        title=_(
+            "notify_on_cancel_message",
+            default="[Cancel] message",
+        ),
+        description=_(
+            "notify_on_cancel_message_help",
+            default="The message text when a booking has been canceled.",
+        ),
+        defaultFactory=notify_on_cancel_message_default_factory,
         required=False,
     )
-    notify_as_reminder_appio_subject = schema.Text(
+    notify_as_reminder_subject = schema.TextLine(
         title=_(
             "notify_as_reminder_subject",
             default="[Reminder] subject",
         ),
         description=_(
-            "notify_as_reminder_appio_subject_help",
+            "notify_as_reminder_subject_help",
             default="The message subject when a reminder will be sent.",
         ),
-        defaultFactory=notify_as_reminder_appio_subject_default_factory,
+        defaultFactory=notify_as_reminder_subject_default_factory,
         required=False,
     )
-    notify_as_reminder_appio_message = schema.Text(
+    notify_as_reminder_message = schema.Text(
         title=_(
             "notify_as_reminder_message",
             default="[Reminder] message",
         ),
         description=_(
             "notify_as_reminder_message_help",
             default="The message text when a reminder will be sent.",
         ),
-        defaultFactory=notify_as_reminder_appio_message_default_factory,
+        defaultFactory=notify_as_reminder_message_default_factory,
         required=False,
     )
 
     model.fieldset(
-        "appio_notifications",
+        "email_notifications",
         label=_(
-            "bookings_appio_templates_label",
-            default="AppIO Notifications",
+            "bookings_email_templates_label",
+            default="Email Notifications",
         ),
         description=_(
-            "bookings_appio_templates_help",
+            "bookings_email_templates_help",
             default="Set message text for all available notification events.",
         ),
         fields=[
-            "notifications_appio_enabled",
-            "notify_on_submit_appio_subject",
-            "notify_on_submit_appio_message",
-            "notify_on_confirm_appio_subject",
-            "notify_on_confirm_appio_message",
-            "notify_on_move_appio_subject",
-            "notify_on_move_appio_message",
-            "notify_on_refuse_appio_subject",
-            "notify_on_refuse_appio_message",
-            "notify_as_reminder_appio_subject",
-            "notify_as_reminder_appio_message",
+            "notifications_email_enabled",
+            "email_from",
+            "notify_on_submit_subject",
+            "notify_on_submit_message",
+            "notify_on_confirm_subject",
+            "notify_on_confirm_message",
+            "notify_on_move_subject",
+            "notify_on_move_message",
+            "notify_on_refuse_subject",
+            "notify_on_refuse_message",
+            "notify_on_cancel_subject",
+            "notify_on_cancel_message",
+            "notify_as_reminder_subject",
+            "notify_as_reminder_message",
         ],
     )
 
 
-@implementer(INotificationAppIO)
-@adapter(IDexterityContent)
-class NotificationAppIO(object):
-    """ """
-
-    def __init__(self, context):
-        self.context = context
-
-
-@provider(IFormFieldProvider)
-class INotificationAppioBookingType(model.Schema):
-    service_code = schema.Choice(
-        title=_(
-            "service_code_label",
-            default="AppIO service code.",
-        ),
-        description=_(
-            "service_code_help",
-            default="AppIO service code related to the current booking type",
-        ),
-        required=False,
-        vocabulary="redturtle.prenotazioni.appio_services",
-    )
-
-
-@implementer(INotificationAppioBookingType)
+@implementer(INotificationEmail)
 @adapter(IDexterityContent)
-class NotificationAppIOBookingType(object):
+class NotificationEmail(object):
     """ """
 
     def __init__(self, context):
         self.context = context
```

### Comparing `redturtle.prenotazioni-2.6.5/src/redturtle/prenotazioni/behaviors/booking_folder/notifications/appio/adapters.py` & `redturtle.prenotazioni-2.7.0/src/redturtle/prenotazioni/behaviors/booking_folder/notifications/appio/adapters.py`

 * *Files 3% similar despite different names*

```diff
@@ -43,14 +43,16 @@
 class BookingTransitionAPPIoSender:
     def __init__(self, message_adapter, booking, request) -> None:
         self.message_adapter = message_adapter
         self.booking = booking
         self.request = request
 
     def send(self) -> bool:
+        from .. import write_message_to_object_history
+
         supervisor = getUtility(IBookingNotificatorSupervisorUtility)
 
         if supervisor.is_appio_message_allowed(self.booking):
             message = self.message_adapter.message
             subject = self.message_adapter.subject
             booking_type = self.booking.get_booking_type()
             service_code = getattr(booking_type, "service_code", None)
@@ -105,8 +107,13 @@
 
             logger.info(
                 "Sent the notification <%s>(`%s`) via AppIO gateway, id returned: %s",
                 self.booking.UID(),
                 subject,
                 msgid,
             )
+
+            write_message_to_object_history(
+                self.booking, self.message_adapter.message_history
+            )
+
             return True
```

### Comparing `redturtle.prenotazioni-2.6.5/src/redturtle/prenotazioni/behaviors/booking_folder/notifications/appio/configure.zcml` & `redturtle.prenotazioni-2.7.0/src/redturtle/prenotazioni/behaviors/booking_folder/notifications/appio/configure.zcml`

 * *Files identical despite different names*

### Comparing `redturtle.prenotazioni-2.6.5/src/redturtle/prenotazioni/behaviors/booking_folder/notifications/appio/events.py` & `redturtle.prenotazioni-2.7.0/src/redturtle/prenotazioni/behaviors/booking_folder/notifications/appio/events.py`

 * *Files 6% similar despite different names*

```diff
@@ -1,24 +1,30 @@
 # -*- coding: utf-8 -*-
+from functools import partial
 
 from zope.component import getMultiAdapter
 from zope.globalrequest import getRequest
 
 from redturtle.prenotazioni.interfaces import IBookingAPPIoMessage
 from redturtle.prenotazioni.interfaces import IBookingNotificationSender
 from redturtle.prenotazioni.utilities import handle_exception_by_log
 
+from .. import notify_the_message_failure
 from . import INotificationAppIO
 
 
 def booking_folder_provides_current_behavior(booking):
     return INotificationAppIO.providedBy(booking.getPrenotazioniFolder())
 
 
+notify_the_message_failure = partial(notify_the_message_failure, gateway_type="AppIO")
+
+
 @handle_exception_by_log
+@notify_the_message_failure
 def send_notification_on_transition(context, event) -> None:
     if not booking_folder_provides_current_behavior(context):
         return
 
     booking_folder = context.getPrenotazioniFolder()
     flags = booking_folder.get_notification_flags()
 
@@ -37,14 +43,15 @@
                 IBookingNotificationSender,
                 name="booking_transition_appio_sender",
             )
             sender_adapter.send()
 
 
 @handle_exception_by_log
+@notify_the_message_failure
 def notify_on_move(context, event):
     if not booking_folder_provides_current_behavior(context):
         return
 
     booking_folder = context.getPrenotazioniFolder()
     if not getattr(booking_folder, "notify_on_move", False):
         return
@@ -59,14 +66,15 @@
             IBookingNotificationSender,
             name="booking_transition_appio_sender",
         )
         sender_adapter.send()
 
 
 @handle_exception_by_log
+@notify_the_message_failure
 def send_booking_reminder(context, event):
     if not booking_folder_provides_current_behavior(context):
         return
 
     message_adapter = getMultiAdapter(
         (context, event),
         IBookingAPPIoMessage,
@@ -74,9 +82,30 @@
     )
 
     if message_adapter and message_adapter.message:
         sender_adapter = getMultiAdapter(
             (message_adapter, context, getRequest()),
             IBookingNotificationSender,
             name="booking_transition_appio_sender",
+        )
+        sender_adapter.send()
+
+
+@handle_exception_by_log
+@notify_the_message_failure
+def send_booking_removed(context, event):
+    if not booking_folder_provides_current_behavior(context):
+        return
+
+    message_adapter = getMultiAdapter(
+        (context, event),
+        IBookingAPPIoMessage,
+        name="removed_notification_appio_message",
+    )
+
+    if message_adapter and message_adapter.message:
+        sender_adapter = getMultiAdapter(
+            (message_adapter, context, getRequest()),
+            IBookingNotificationSender,
+            name="booking_transition_appio_sender",
         )
         sender_adapter.send()
```

### Comparing `redturtle.prenotazioni-2.6.5/src/redturtle/prenotazioni/behaviors/booking_folder/notifications/appio/notfication_appio_message.py` & `redturtle.prenotazioni-2.7.0/src/redturtle/prenotazioni/behaviors/booking_folder/notifications/sms/message.py`

 * *Files 16% similar despite different names*

```diff
@@ -1,98 +1,121 @@
 # -*- coding: utf-8 -*-
-"""AppIO notification templates"""
-
+"""SMS Notification Templates"""
+from plone import api
 from plone.stringinterp.interfaces import IContextWrapper
 from plone.stringinterp.interfaces import IStringInterpolator
 from Products.DCWorkflow.interfaces import IAfterTransitionEvent
 from zope.component import adapter
 from zope.interface import implementer
 
+from redturtle.prenotazioni import _
 from redturtle.prenotazioni.content.prenotazione import IPrenotazione
-from redturtle.prenotazioni.interfaces import IBookingAPPIoMessage
 from redturtle.prenotazioni.interfaces import IBookingReminderEvent
+from redturtle.prenotazioni.interfaces import IBookingSMSMessage
 from redturtle.prenotazioni.prenotazione_event import IMovedPrenotazione
 
 
-class PrenotazioneAPPIoMessage:
+class PrenotazioneSMSMessage:
     prenotazione = None
     event = None
 
     def __init__(self, prenotazione, event):
         self.prenotazione = prenotazione
         self.event = event
 
     @property
     def message(self) -> str:
-        NotImplementedError
+        raise NotImplementedError("The method was not implemented")
+
+    @property
+    def message_history(self) -> str:
+        raise NotImplementedError("The method was not implemented")
 
 
-@implementer(IBookingAPPIoMessage)
+@implementer(IBookingSMSMessage)
 @adapter(IPrenotazione, IMovedPrenotazione)
-class PrenotazioneMovedAPPIoMessage(PrenotazioneAPPIoMessage):
+class PrenotazioneMovedSMSMessage(PrenotazioneSMSMessage):
     @property
     def message(self) -> str:
         return IStringInterpolator(IContextWrapper(self.prenotazione)())(
             getattr(
                 self.prenotazione.getPrenotazioniFolder(),
-                "notify_on_move_appio_message",
+                "notify_on_move_sms_message",
                 None,
-            )
+            ),
         )
 
     @property
-    def subject(self) -> str:
-        return IStringInterpolator(IContextWrapper(self.prenotazione)())(
-            getattr(
-                self.prenotazione.getPrenotazioniFolder(),
-                "notify_on_move_appio_subject",
-                "",
-            )
+    def message_history(self) -> str:
+        _(
+            "history_sms_reschedule_sent",
+            default="SMS message about the booking reschedule was sent",
         )
 
 
-@implementer(IBookingAPPIoMessage)
+@implementer(IBookingSMSMessage)
 @adapter(IPrenotazione, IAfterTransitionEvent)
-class PrenotazioneAfterTransitionAPPIoMessage(PrenotazioneAPPIoMessage):
+class PrenotazioneAfterTransitionSMSMessage(PrenotazioneSMSMessage):
     @property
     def message(self) -> str:
         return IStringInterpolator(IContextWrapper(self.prenotazione)())(
             getattr(
                 self.prenotazione.getPrenotazioniFolder(),
-                f"notify_on_{self.event.transition and self.event.transition.__name__}_appio_message",
+                f"notify_on_{self.event.transition and self.event.transition.__name__}_sms_message",
                 None,
-            )
+            ),
         )
 
     @property
-    def subject(self) -> str:
-        return IStringInterpolator(IContextWrapper(self.prenotazione)())(
-            getattr(
-                self.prenotazione.getPrenotazioniFolder(),
-                f"notify_on_{self.event.transition and self.event.transition.__name__}_appio_subject",
-                None,
-            )
+    def message_history(self) -> str:
+        transition = (
+            self.event.transition
+            and api.portal.translate(self.event.transition.title)
+            or ""
+        )
+        return api.portal.translate(
+            _(
+                "history_sms_transition_sent",
+                "SMS message about the ${transition} transition was sent",
+                mapping={"transition": transition},
+            ),
         )
 
 
-@implementer(IBookingAPPIoMessage)
+@implementer(IBookingSMSMessage)
 @adapter(IPrenotazione, IBookingReminderEvent)
-class PrenotazioneReminderAppIOMessage(PrenotazioneAPPIoMessage):
+class PrenotazioneReminderSMSMessage(PrenotazioneSMSMessage):
     @property
     def message(self) -> str:
         return IStringInterpolator(IContextWrapper(self.prenotazione)())(
             getattr(
                 self.prenotazione.getPrenotazioniFolder(),
-                "notify_as_reminder_appio_message",
+                "notify_as_reminder_sms_message",
                 "",
             )
         )
 
     @property
-    def subject(self) -> str:
+    def message_history(self) -> str:
+        return api.portal.translate(
+            _("history_sms_reminder_sent", default="SMS reminder was sent")
+        )
+
+
+@implementer(IBookingSMSMessage)
+@adapter(IPrenotazione, IBookingReminderEvent)
+class PrenotazioneRemovedSMSMessage(PrenotazioneSMSMessage):
+    @property
+    def message(self) -> str:
         return IStringInterpolator(IContextWrapper(self.prenotazione)())(
             getattr(
                 self.prenotazione.getPrenotazioniFolder(),
-                "notify_as_reminder_appio_subject",
+                "notify_as_removed_sms_message",
                 "",
             )
         )
+
+    @property
+    def message_history(self) -> str:
+        return api.portal.translate(
+            _("history_sms_removed_sent", default="SMS removed notification was sent")
+        )
```

### Comparing `redturtle.prenotazioni-2.6.5/src/redturtle/prenotazioni/behaviors/booking_folder/notifications/appio/voc_service_keys.py` & `redturtle.prenotazioni-2.7.0/src/redturtle/prenotazioni/behaviors/booking_folder/notifications/appio/voc_service_keys.py`

 * *Files identical despite different names*

### Comparing `redturtle.prenotazioni-2.6.5/src/redturtle/prenotazioni/behaviors/booking_folder/notifications/email/adapters.py` & `redturtle.prenotazioni-2.7.0/src/redturtle/prenotazioni/behaviors/booking_folder/notifications/email/adapters.py`

 * *Files 10% similar despite different names*

```diff
@@ -7,14 +7,16 @@
 from redturtle.prenotazioni.content.prenotazione import IPrenotazione
 from redturtle.prenotazioni.interfaces import IBookingEmailMessage
 from redturtle.prenotazioni.interfaces import IBookingNotificationSender
 from redturtle.prenotazioni.interfaces import IBookingNotificatorSupervisorUtility
 from redturtle.prenotazioni.interfaces import IRedturtlePrenotazioniLayer
 from redturtle.prenotazioni.utilities import send_email
 
+from .. import write_message_to_object_history
+
 
 @implementer(IBookingNotificationSender)
 @adapter(IBookingEmailMessage, IPrenotazione, IRedturtlePrenotazioniLayer)
 class BookingTransitionEmailSender:
     def __init__(self, message_adapter, booking, request) -> None:
         self.message_adapter = message_adapter
         self.booking = booking
@@ -22,19 +24,24 @@
 
     def send(self, force=False):
         """
         force: bool
             If True, the message will be sent even if the email is not allowed
             (ie. for operator notifications)
         """
+
         message = self.message_adapter.message
 
         if force or getUtility(
             IBookingNotificatorSupervisorUtility
         ).is_email_message_allowed(self.booking):
             logger.debug(
                 f"Sending the notification <{self.booking.UID()}>(`{message}`) via Email gateway"
             )
             logger.info(
                 f"Sending the notification <{self.booking.UID()}> via Email gateway"
             )
+
             send_email(message)
+            write_message_to_object_history(
+                self.booking, message=self.message_adapter.message_history
+            )
```

### Comparing `redturtle.prenotazioni-2.6.5/src/redturtle/prenotazioni/behaviors/booking_folder/notifications/email/configure.zcml` & `redturtle.prenotazioni-2.7.0/src/redturtle/prenotazioni/behaviors/booking_folder/notifications/email/configure.zcml`

 * *Files identical despite different names*

### Comparing `redturtle.prenotazioni-2.6.5/src/redturtle/prenotazioni/behaviors/booking_folder/notifications/email/events.py` & `redturtle.prenotazioni-2.7.0/src/redturtle/prenotazioni/behaviors/booking_folder/notifications/sms/events.py`

 * *Files 11% similar despite different names*

```diff
@@ -1,123 +1,115 @@
 # -*- coding: utf-8 -*-
+from functools import partial
 
 from zope.component import getMultiAdapter
 from zope.globalrequest import getRequest
 
-from redturtle.prenotazioni.interfaces import IBookingEmailMessage
 from redturtle.prenotazioni.interfaces import IBookingNotificationSender
+from redturtle.prenotazioni.interfaces import IBookingSMSMessage
 from redturtle.prenotazioni.utilities import handle_exception_by_log
 
-from . import INotificationEmail
+from .. import notify_the_message_failure
+from . import INotificationSMS
 
 
 def booking_folder_provides_current_behavior(booking):
-    return INotificationEmail.providedBy(booking.getPrenotazioniFolder())
+    return INotificationSMS.providedBy(booking.getPrenotazioniFolder())
+
+
+notify_the_message_failure = partial(notify_the_message_failure, gateway_type="SMS")
 
 
 @handle_exception_by_log
-def send_email_notification_on_transition(context, event) -> None:
+@notify_the_message_failure
+def send_notification_on_transition(context, event) -> None:
     if not booking_folder_provides_current_behavior(context):
         return
 
     booking_folder = context.getPrenotazioniFolder()
     flags = booking_folder.get_notification_flags()
 
     if flags["confirm"] and getattr(booking_folder, "auto_confirm", False):
         flags["submit"] = False
 
-    if flags.get(
-        event.transition and event.transition.__name__ or "",
-        False,
-    ):
-        if not getattr(context, "email", ""):
-            # booking does not have an email set
+    if event.transition and flags.get(event.transition.__name__):
+        if not getattr(context, "phone", ""):
+            # booking does not have an phone set
             return
+
         message_adapter = getMultiAdapter(
             (context, event),
-            IBookingEmailMessage,
+            IBookingSMSMessage,
         )
 
         if message_adapter and message_adapter.message:
             sender_adapter = getMultiAdapter(
                 (message_adapter, context, getRequest()),
                 IBookingNotificationSender,
-                name="booking_transition_email_sender",
+                name="booking_transition_sms_sender",
             )
             sender_adapter.send()
 
 
-# TODO: use the notify_on_after_transition_event method techique instead
 @handle_exception_by_log
+@notify_the_message_failure
 def notify_on_move(context, event):
     if not booking_folder_provides_current_behavior(context):
         return
 
     booking_folder = context.getPrenotazioniFolder()
     if not getattr(booking_folder, "notify_on_move", False):
         return
-    if not getattr(context, "email", ""):
-        # booking does not have an email set
-        return
-    message_adapter = getMultiAdapter((context, event), IBookingEmailMessage)
-    sender_adapter = getMultiAdapter(
-        (message_adapter, context, getRequest()),
-        IBookingNotificationSender,
-        name="booking_transition_email_sender",
-    )
-
-    sender_adapter.send()
+    # XXX: il controllo immagino sia altrove e deve controllare
+    #      non solo se l'email è presente ma anche se le notifiche email
+    #      sono attive
+    # if not getattr(context, "email", ""):
+    #     # booking does not have an email set
+    #     return
+    message_adapter = getMultiAdapter((context, event), IBookingSMSMessage)
+    if message_adapter and message_adapter.message:
+        sender_adapter = getMultiAdapter(
+            (message_adapter, context, getRequest()),
+            IBookingNotificationSender,
+            name="booking_transition_sms_sender",
+        )
+        sender_adapter.send()
 
 
 @handle_exception_by_log
+@notify_the_message_failure
 def send_booking_reminder(context, event):
     if not booking_folder_provides_current_behavior(context):
         return
 
     message_adapter = getMultiAdapter(
         (context, event),
-        IBookingEmailMessage,
-        name="reminder_notification_email_message",
-    )
-    sender_adapter = getMultiAdapter(
-        (message_adapter, context, getRequest()),
-        IBookingNotificationSender,
-        name="booking_transition_email_sender",
+        IBookingSMSMessage,
+        name="reminder_notification_sms_message",
     )
+    if message_adapter and message_adapter.message:
+        sender_adapter = getMultiAdapter(
+            (message_adapter, context, getRequest()),
+            IBookingNotificationSender,
+            name="booking_transition_sms_sender",
+        )
+        sender_adapter.send()
 
-    sender_adapter.send()
-
-
-def send_booking_canceled_to_managers(booking, event):
-    """
-    Send email notification for managers
-    """
-    if (
-        event.transition is None
-        or not getattr(event.transition, "id", None) == "cancel"
-    ):
-        return
-
-    if not booking_folder_provides_current_behavior(booking):
-        return
-
-    if booking.isVacation():
-        return
 
-    if not getattr(booking.getPrenotazioniFolder(), "email_responsabile", []):
+@handle_exception_by_log
+@notify_the_message_failure
+def send_booking_removed(context, event):
+    if not booking_folder_provides_current_behavior(context):
         return
 
-    request = getRequest()
-
     message_adapter = getMultiAdapter(
-        (booking, request),
-        IBookingEmailMessage,
-        name="notify_manager_booking_canceled",
-    )
-
-    sender_adapter = getMultiAdapter(
-        (message_adapter, booking, request),
-        IBookingNotificationSender,
-        name="booking_transition_email_sender",
+        (context, event),
+        IBookingSMSMessage,
+        name="removed_notification_sms_message",
     )
-
-    sender_adapter.send(force=True)
+    if message_adapter and message_adapter.message:
+        sender_adapter = getMultiAdapter(
+            (message_adapter, context, getRequest()),
+            IBookingNotificationSender,
+            name="booking_transition_sms_sender",
+        )
+        sender_adapter.send()
```

#### encoding

```diff
@@ -1 +1 @@
-us-ascii
+utf-8
```

### Comparing `redturtle.prenotazioni-2.6.5/src/redturtle/prenotazioni/behaviors/booking_folder/notifications/email/notification_email_message.py` & `redturtle.prenotazioni-2.7.0/src/redturtle/prenotazioni/behaviors/booking_folder/notifications/email/notification_email_message.py`

 * *Files 12% similar despite different names*

```diff
@@ -12,15 +12,14 @@
 from plone.stringinterp.interfaces import IContextWrapper
 from plone.stringinterp.interfaces import IStringInterpolator
 from plone.stringinterp.interfaces import IStringSubstitution
 from Products.DCWorkflow.interfaces import IAfterTransitionEvent
 from zope.annotation.interfaces import IAnnotations
 from zope.component import adapter
 from zope.component import getAdapter
-from zope.i18n import translate
 from zope.interface import Interface
 from zope.interface import implementer
 
 from redturtle.prenotazioni import _
 from redturtle.prenotazioni import logger
 from redturtle.prenotazioni.content.prenotazione import IPrenotazione
 from redturtle.prenotazioni.interfaces import IBookingEmailMessage
@@ -36,14 +35,18 @@
     error_msg = "Could not send notification email due to: {message}"
 
     def __init__(self, prenotazione, event):
         self.prenotazione = prenotazione
         self.event = event
 
     @property
+    def message_history(self) -> str:
+        raise NotImplementedError("The method was not implemented")
+
+    @property
     def message_subject(self) -> str:
         raise NotImplementedError("The method was not implemented")
 
     @property
     def message_text(self) -> MIMEText:
         raise NotImplementedError("The method was not implemented")
 
@@ -117,14 +120,23 @@
 
 @implementer(IBookingEmailMessage)
 @adapter(IPrenotazione, IMovedPrenotazione)
 class PrenotazioneMovedICalEmailMessage(
     PrenotazioneEventMessageICalMixIn, PrenotazioneEmailMessage
 ):
     @property
+    def message_history(self) -> str:
+        return api.portal.translate(
+            _(
+                "history_email_reschedule_sent",
+                default="Email message about the booking reschedule was sent",
+            )
+        )
+
+    @property
     def message_subject(self) -> str:
         return IStringInterpolator(IContextWrapper(self.prenotazione)())(
             getattr(self.prenotazioni_folder, "notify_on_move_subject", "")
         )
 
     @property
     def message_text(self) -> MIMEText:
@@ -139,14 +151,29 @@
             return MIMEText(text, "html")
 
 
 @implementer(IBookingEmailMessage)
 @adapter(IPrenotazione, IAfterTransitionEvent)
 class PrenotazioneAfterTransitionEmailMessage(PrenotazioneEmailMessage):
     @property
+    def message_history(self) -> str:
+        transition = (
+            self.event.transition
+            and api.portal.translate(self.event.transition.title)
+            or ""
+        )
+        return api.portal.translate(
+            _(
+                "history_email_transition_sent",
+                "Email message about the ${transition} transition was sent",
+                mapping={"transition": transition},
+            ),
+        )
+
+    @property
     def message_subject(self) -> str:
         return IStringInterpolator(IContextWrapper(self.prenotazione)())(
             getattr(
                 self.prenotazioni_folder,
                 f"notify_on_{self.event.transition and self.event.transition.__name__}_subject",
                 "",
             )
@@ -177,14 +204,20 @@
     pass
 
 
 @implementer(IBookingEmailMessage)
 @adapter(IPrenotazione, IBookingReminderEvent)
 class PrenotazioneReminderEmailMessage(PrenotazioneEmailMessage):
     @property
+    def message_history(self) -> str:
+        return api.portal.translate(
+            _("history_reminder_sent", default="Email reminder was sent")
+        )
+
+    @property
     def message_subject(self) -> str:
         return IStringInterpolator(IContextWrapper(self.prenotazione)())(
             getattr(self.prenotazioni_folder, "notify_as_reminder_subject", "")
         )
 
     @property
     def message_text(self) -> MIMEText:
@@ -216,14 +249,23 @@
         self.request = request
         # set request annotation to mark it as manager notification.
         # this will be used in ical adapter to change the title of the ical item
         annotations = IAnnotations(prenotazione.REQUEST)
         annotations["ical_manager_notification"] = True
 
     @property
+    def message_history(self) -> str:
+        return api.portal.translate(
+            _(
+                "history_email_manager_notification_sent",
+                default="Email notification was sent to booking manager",
+            ),
+        )
+
+    @property
     def message(self) -> MIMEMultipart:
         """
         customized to send Bcc instead To
         """
         mfrom = self.message_from
         bcc = ", ".join(getattr(self.prenotazione, "email_responsabile", []))
 
@@ -318,17 +360,16 @@
         """
         return subject
         """
         booking_type = getattr(self.prenotazione, "booking_type", "")
         booking_code = self.prenotazione.getBookingCode()
         date = self.prenotazione.booking_date.strftime("%d-%m-%Y %H:%M")
 
-        booking_canceled = translate(
-            _("booking_canceled_mail_subject_part", default="Booking canceled: "),
-            context=self.request,
+        booking_canceled = api.portal.translate(
+            _("booking_canceled_mail_subject_part", default="Booking canceled: ")
         )
         return f"{booking_canceled} [{booking_type}] {date} {booking_code}"
 
     @property
     def message(self) -> MIMEMultipart:
         """
         customized to send Bcc instead To
@@ -346,7 +387,29 @@
 
         msg.attach(self.message_text)
         msg["Subject"] = self.message_subject
         msg["From"] = mfrom
         msg["Bcc"] = bcc
 
         return msg
+
+
+@implementer(IBookingEmailMessage)
+@adapter(IPrenotazione, IBookingReminderEvent)
+class PrenotazioneRemovedEmailMessage(PrenotazioneEmailMessage):
+    @property
+    def message_subject(self) -> str:
+        return IStringInterpolator(IContextWrapper(self.prenotazione)())(
+            getattr(self.prenotazioni_folder, "notify_as_removed_subject", "")
+        )
+
+    @property
+    def message_text(self) -> MIMEText:
+        text = IStringInterpolator(IContextWrapper(self.prenotazione)())(
+            getattr(self.prenotazioni_folder, "notify_as_removed_message", None),
+        )
+        if CTE:
+            cs = Charset("utf-8")
+            cs.body_encoding = CTE  # e.g. 'base64'
+            return MIMEText(text, "html", cs)
+        else:
+            return MIMEText(text, "html")
```

### Comparing `redturtle.prenotazioni-2.6.5/src/redturtle/prenotazioni/behaviors/booking_folder/notifications/sms/__init__.py` & `redturtle.prenotazioni-2.7.0/src/redturtle/prenotazioni/behaviors/booking_folder/notifications/sms/__init__.py`

 * *Files 5% similar despite different names*

```diff
@@ -49,14 +49,24 @@
             "notify_on_refuse_sms_message_default_value",
             "[${prenotazioni_folder_title}]: The booking ${booking_type} of ${booking_date} at ${booking_time} was refused.",
         )
     )
 
 
 @provider(IContextAwareDefaultFactory)
+def notify_on_cancel_sms_message_default_factory(context):
+    return api.portal.translate(
+        _(
+            "notify_on_cancel_sms_message_default_value",
+            "[${prenotazioni_folder_title}]: The booking ${booking_type} of ${booking_date} at ${booking_time} was canceled.",
+        )
+    )
+
+
+@provider(IContextAwareDefaultFactory)
 def notify_as_reminder_sms_message_default_factory(context):
     return api.portal.translate(
         _(
             "notify_as_reminder_sms_message_default_value",
             "[${prenotazioni_folder_title}]: This is an automatic reminder about your booking on ${date} for ${booking_type} ."
             "\nSee details or delete it: ${booking_print_url} .",
         )
@@ -118,14 +128,26 @@
         description=_(
             "notify_on_refuse_message_help",
             default="The message text when a booking has been refused.",
         ),
         defaultFactory=notify_on_refuse_sms_message_default_factory,
         required=False,
     )
+    notify_on_cancel_sms_message = schema.Text(
+        title=_(
+            "notify_on_cancel_message",
+            default="[Cancel] message",
+        ),
+        description=_(
+            "notify_on_cancel_message_help",
+            default="The message text when a booking has been canceled.",
+        ),
+        defaultFactory=notify_on_cancel_sms_message_default_factory,
+        required=False,
+    )
     notify_as_reminder_sms_message = schema.Text(
         title=_(
             "notify_as_reminder_message",
             default="[Reminder] message",
         ),
         description=_(
             "notify_as_reminder_message_help",
@@ -147,14 +169,15 @@
         ),
         fields=[
             "notifications_sms_enabled",
             "notify_on_submit_sms_message",
             "notify_on_confirm_sms_message",
             "notify_on_move_sms_message",
             "notify_on_refuse_sms_message",
+            "notify_on_cancel_sms_message",
             "notify_as_reminder_sms_message",
         ],
     )
 
 
 @implementer(INotificationSMS)
 @adapter(IDexterityContent)
```

### Comparing `redturtle.prenotazioni-2.6.5/src/redturtle/prenotazioni/behaviors/booking_folder/notifications/sms/adapters.py` & `redturtle.prenotazioni-2.7.0/src/redturtle/prenotazioni/restapi/serializers/adapters/prenotazione_type.py`

 * *Files 26% similar despite different names*

```diff
@@ -1,31 +1,26 @@
 # -*- coding: utf-8 -*-
-
+from plone import api
 from zope.component import adapter
-from zope.component import getUtility
-from zope.interface import Interface
 from zope.interface import implementer
 
-from redturtle.prenotazioni.content.prenotazione import IPrenotazione
-from redturtle.prenotazioni.interfaces import IBookingNotificationSender
-from redturtle.prenotazioni.interfaces import IBookingNotificatorSupervisorUtility
-from redturtle.prenotazioni.interfaces import IBookingSMSMessage
+from redturtle.prenotazioni.content.prenotazione_type import IPrenotazioneType
+from redturtle.prenotazioni.interfaces import IRedturtlePrenotazioniLayer
+from redturtle.prenotazioni.interfaces import ISerializeToRetroCompatibleJson
 
 
-@implementer(IBookingNotificationSender)
-@adapter(IBookingSMSMessage, IPrenotazione, Interface)
-class BookingNotificationSender:
-    def __init__(self, message_adapter, booking, request) -> None:
-        self.message_adapter = message_adapter
-        self.booking = booking
-        self.request = request
+@implementer(ISerializeToRetroCompatibleJson)
+@adapter(IPrenotazioneType, IRedturtlePrenotazioniLayer)
+class PrenotazioneTypeRetroCompatibleSerializer:
+    """PrenotazioneType c.t. serializer retrocompatible with earlier frontend implementation"""
 
-    def send(self):
-        if self.is_notification_allowed():
-            raise NotImplementedError("The method was not implemented")
+    def __init__(self, context, request):
+        self.context = context
+        self.request = request
 
-    def is_notification_allowed(self):
-        if getUtility(
-            IBookingNotificatorSupervisorUtility,
-        ).is_sms_message_allowed(self.booking):
-            return True
-        return False
+    def __call__(self, *args, **kwargs):
+        hidden = api.content.get_state(self.context) not in ("published",)
+        return {
+            "name": self.context.title,
+            "duration": str(self.context.duration),
+            "hidden": hidden,
+        }
```

### Comparing `redturtle.prenotazioni-2.6.5/src/redturtle/prenotazioni/behaviors/booking_folder/notifications/sms/configure.zcml` & `redturtle.prenotazioni-2.7.0/src/redturtle/prenotazioni/behaviors/booking_folder/notifications/sms/configure.zcml`

 * *Files identical despite different names*

### Comparing `redturtle.prenotazioni-2.6.5/src/redturtle/prenotazioni/behaviors/booking_folder/notifications/sms/message.py` & `redturtle.prenotazioni-2.7.0/src/redturtle/prenotazioni/tests/test_restapi_types_override.py`

 * *Files 24% similar despite different names*

```diff
@@ -1,68 +1,75 @@
 # -*- coding: utf-8 -*-
-"""SMS Notification Templates"""
+import unittest
+from datetime import date
 
-from plone.stringinterp.interfaces import IContextWrapper
-from plone.stringinterp.interfaces import IStringInterpolator
-from Products.DCWorkflow.interfaces import IAfterTransitionEvent
-from zope.component import adapter
-from zope.interface import implementer
-
-from redturtle.prenotazioni.content.prenotazione import IPrenotazione
-from redturtle.prenotazioni.interfaces import IBookingReminderEvent
-from redturtle.prenotazioni.interfaces import IBookingSMSMessage
-from redturtle.prenotazioni.prenotazione_event import IMovedPrenotazione
-
-
-class PrenotazioneSMSMessage:
-    prenotazione = None
-    event = None
-
-    def __init__(self, prenotazione, event):
-        self.prenotazione = prenotazione
-        self.event = event
-
-    @property
-    def message(self) -> str:
-        NotImplementedError
-
-
-@implementer(IBookingSMSMessage)
-@adapter(IPrenotazione, IMovedPrenotazione)
-class PrenotazioneMovedSMSMessage(PrenotazioneSMSMessage):
-    @property
-    def message(self) -> str:
-        return IStringInterpolator(IContextWrapper(self.prenotazione)())(
-            getattr(
-                self.prenotazione.getPrenotazioniFolder(),
-                "notify_on_move_sms_message",
-                None,
-            ),
+import transaction
+from plone import api
+from plone.app.testing import SITE_OWNER_NAME
+from plone.app.testing import SITE_OWNER_PASSWORD
+from plone.app.testing import TEST_USER_ID
+from plone.app.testing import setRoles
+from plone.restapi.testing import RelativeSession
+
+from redturtle.prenotazioni.testing import REDTURTLE_PRENOTAZIONI_API_FUNCTIONAL_TESTING
+
+
+class TestTypesOverrides(unittest.TestCase):
+    layer = REDTURTLE_PRENOTAZIONI_API_FUNCTIONAL_TESTING
+
+    def setUp(self):
+        self.app = self.layer["app"]
+        self.portal = self.layer["portal"]
+        self.request = self.layer["request"]
+        self.portal_url = self.portal.absolute_url()
+        setRoles(self.portal, TEST_USER_ID, ["Manager"])
+
+        self.api_session = RelativeSession(self.portal_url)
+        self.api_session.headers.update({"Accept": "application/json"})
+        self.api_session.auth = (SITE_OWNER_NAME, SITE_OWNER_PASSWORD)
+
+        self.portal_url = self.portal.absolute_url()
+        self.folder_prenotazioni = api.content.create(
+            container=self.portal,
+            type="PrenotazioniFolder",
+            title="Folder",
+            description="",
+            daData=date.today(),
+            gates=["Gate A", "Gate B"],
+            same_day_booking_disallowed="no",
         )
 
+        booking_type_A = api.content.create(
+            type="PrenotazioneType",
+            title="Type A",
+            duration=30,
+            container=self.folder_prenotazioni,
+            gates=["all"],
+        )
 
-@implementer(IBookingSMSMessage)
-@adapter(IPrenotazione, IAfterTransitionEvent)
-class PrenotazioneAfterTransitionSMSMessage(PrenotazioneSMSMessage):
-    @property
-    def message(self) -> str:
-        return IStringInterpolator(IContextWrapper(self.prenotazione)())(
-            getattr(
-                self.prenotazione.getPrenotazioniFolder(),
-                f"notify_on_{self.event.transition and self.event.transition.__name__}_sms_message",
-                None,
-            ),
+        api.content.transition(
+            booking_type_A,
+            transition="publish",
         )
+        api.content.transition(obj=self.folder_prenotazioni, transition="publish")
+
+        transaction.commit()
 
+    def tearDown(self):
+        self.api_session.close()
 
-@implementer(IBookingSMSMessage)
-@adapter(IPrenotazione, IBookingReminderEvent)
-class PrenotazioneReminderSMSMessage(PrenotazioneSMSMessage):
-    @property
-    def message(self) -> str:
-        return IStringInterpolator(IContextWrapper(self.prenotazione)())(
-            getattr(
-                self.prenotazione.getPrenotazioniFolder(),
-                "notify_as_reminder_sms_message",
-                "",
-            )
+    def test_types_expanded_hide_prenotazioniyear(self):
+        response = self.api_session.get(
+            self.folder_prenotazioni.absolute_url(), params={"expand": "types"}
         )
+
+        self.assertEqual(response.status_code, 200)
+        res = response.json()
+        prenotazioni_year = None
+        for x in res["@components"]["types"]:
+            if x["id"] == "PrenotazioniYear":
+                prenotazioni_year = x
+                break
+
+        self.assertIsNotNone(prenotazioni_year)
+        self.assertFalse(prenotazioni_year["immediately_addable"])
+        self.assertFalse(prenotazioni_year["addable"])
```

### Comparing `redturtle.prenotazioni-2.6.5/src/redturtle/prenotazioni/browser/base.py` & `redturtle.prenotazioni-2.7.0/src/redturtle/prenotazioni/browser/base.py`

 * *Files identical despite different names*

### Comparing `redturtle.prenotazioni-2.6.5/src/redturtle/prenotazioni/browser/configure.zcml` & `redturtle.prenotazioni-2.7.0/src/redturtle/prenotazioni/browser/configure.zcml`

 * *Files identical despite different names*

### Comparing `redturtle.prenotazioni-2.6.5/src/redturtle/prenotazioni/browser/custom_radio_input.pt` & `redturtle.prenotazioni-2.7.0/src/redturtle/prenotazioni/browser/custom_radio_input.pt`

 * *Files identical despite different names*

### Comparing `redturtle.prenotazioni-2.6.5/src/redturtle/prenotazioni/browser/delete_reservation.py` & `redturtle.prenotazioni-2.7.0/src/redturtle/prenotazioni/browser/delete_reservation.py`

 * *Files identical despite different names*

### Comparing `redturtle.prenotazioni-2.6.5/src/redturtle/prenotazioni/browser/folderfactories.py` & `redturtle.prenotazioni-2.7.0/src/redturtle/prenotazioni/browser/folderfactories.py`

 * *Files identical despite different names*

### Comparing `redturtle.prenotazioni-2.6.5/src/redturtle/prenotazioni/browser/prenotazione.py` & `redturtle.prenotazioni-2.7.0/src/redturtle/prenotazioni/browser/prenotazione.py`

 * *Files identical despite different names*

### Comparing `redturtle.prenotazioni-2.6.5/src/redturtle/prenotazioni/browser/prenotazione_add.py` & `redturtle.prenotazioni-2.7.0/src/redturtle/prenotazioni/browser/prenotazione_add.py`

 * *Files identical despite different names*

### Comparing `redturtle.prenotazioni-2.6.5/src/redturtle/prenotazioni/browser/prenotazione_move.py` & `redturtle.prenotazioni-2.7.0/src/redturtle/prenotazioni/browser/prenotazione_move.py`

 * *Files identical despite different names*

### Comparing `redturtle.prenotazioni-2.6.5/src/redturtle/prenotazioni/browser/prenotazione_print.py` & `redturtle.prenotazioni-2.7.0/src/redturtle/prenotazioni/browser/prenotazione_print.py`

 * *Files identical despite different names*

### Comparing `redturtle.prenotazioni-2.6.5/src/redturtle/prenotazioni/browser/prenotazioni_context_state.py` & `redturtle.prenotazioni-2.7.0/src/redturtle/prenotazioni/browser/prenotazioni_context_state.py`

 * *Files identical despite different names*

### Comparing `redturtle.prenotazioni-2.6.5/src/redturtle/prenotazioni/browser/prenotazioni_portal_state.py` & `redturtle.prenotazioni-2.7.0/src/redturtle/prenotazioni/browser/prenotazioni_portal_state.py`

 * *Files identical despite different names*

### Comparing `redturtle.prenotazioni-2.6.5/src/redturtle/prenotazioni/browser/prenotazioni_search.py` & `redturtle.prenotazioni-2.7.0/src/redturtle/prenotazioni/browser/prenotazioni_search.py`

 * *Files 2% similar despite different names*

```diff
@@ -175,54 +175,54 @@
 
     def set_search_string(self, data):
         result = []
         MARKUP = "<strong>{}:</strong> {}"
         if "text" in data and data.get("text", None):
             result.append(
                 MARKUP.format(
-                    self.context.translate(_("label_text", "Text to search")),
+                    api.portal.translate(_("label_text", "Text to search")),
                     data["text"],
                 )
             )
         if "review_state" in data and data.get("review_state", None):
             result.append(
                 MARKUP.format(
-                    self.context.translate(
+                    api.portal.translate(
                         __("State"),
                     ),
-                    self.context.translate(__(data["review_state"])),
+                    api.portal.translate(__(data["review_state"])),
                 )
             )
 
         if "gate" in data and data.get("gate", None):
             result.append(
                 MARKUP.format(
-                    self.context.translate(
+                    api.portal.translate(
                         _("label_gate", "Gate"),
                     ),
                     data["gate"],
                 )
             )
 
         if "start" in data and data.get("start", None):
             if isinstance(data.get("start"), str):
                 data["start"] = datetime.strptime(data.get("start"), "%Y-%m-%d")
             result.append(
                 MARKUP.format(
-                    self.context.translate(_("label_start", "Start date ")),
+                    api.portal.translate(_("label_start", "Start date ")),
                     data["start"].strftime("%d/%m/%Y"),
                 )
             )
 
         if "end" in data and data.get("end", None):
             if isinstance(data.get("end"), str):
                 data["end"] = datetime.strptime(data.get("end"), "%Y-%m-%d")
             result.append(
                 MARKUP.format(
-                    self.context.translate(_("label_end", "End date")),
+                    api.portal.translate(_("label_end", "End date")),
                     data["end"].strftime("%d/%m/%Y"),
                 )
             )
         search_string = ""
         if result:
             search_string = "; ".join(result)
             search_string = "<p>{}</p>".format(search_string)
```

### Comparing `redturtle.prenotazioni-2.6.5/src/redturtle/prenotazioni/browser/static/redturtle-reservation.css` & `redturtle.prenotazioni-2.7.0/src/redturtle/prenotazioni/browser/static/redturtle-reservation.css`

 * *Files identical despite different names*

### Comparing `redturtle.prenotazioni-2.6.5/src/redturtle/prenotazioni/browser/static/redturtle-reservation.js` & `redturtle.prenotazioni-2.7.0/src/redturtle/prenotazioni/browser/static/redturtle-reservation.js`

 * *Files identical despite different names*

### Comparing `redturtle.prenotazioni-2.6.5/src/redturtle/prenotazioni/browser/static/times-solid.png` & `redturtle.prenotazioni-2.7.0/src/redturtle/prenotazioni/browser/static/times-solid.png`

 * *Files identical despite different names*

### Comparing `redturtle.prenotazioni-2.6.5/src/redturtle/prenotazioni/browser/static/widget/dist/prod/main.css` & `redturtle.prenotazioni-2.7.0/src/redturtle/prenotazioni/browser/static/widget/dist/prod/main.css`

 * *Files identical despite different names*

### Comparing `redturtle.prenotazioni-2.6.5/src/redturtle/prenotazioni/browser/static/widget/dist/prod/main.css.map` & `redturtle.prenotazioni-2.7.0/src/redturtle/prenotazioni/browser/static/widget/dist/prod/main.css.map`

 * *Files identical despite different names*

### Comparing `redturtle.prenotazioni-2.6.5/src/redturtle/prenotazioni/browser/static/widget/dist/prod/main.js` & `redturtle.prenotazioni-2.7.0/src/redturtle/prenotazioni/browser/static/widget/dist/prod/main.js`

 * *Files identical despite different names*

### Comparing `redturtle.prenotazioni-2.6.5/src/redturtle/prenotazioni/browser/static/widget/js/WidgetContainer/index.js` & `redturtle.prenotazioni-2.7.0/src/redturtle/prenotazioni/browser/static/widget/js/WidgetContainer/index.js`

 * *Files identical despite different names*

### Comparing `redturtle.prenotazioni-2.6.5/src/redturtle/prenotazioni/browser/static/widget/js/WidgetDataContainer/index.js` & `redturtle.prenotazioni-2.7.0/src/redturtle/prenotazioni/browser/static/widget/js/WidgetDataContainer/index.js`

 * *Files identical despite different names*

### Comparing `redturtle.prenotazioni-2.6.5/src/redturtle/prenotazioni/browser/static/widget/js/WidgetDataContainer/index.less` & `redturtle.prenotazioni-2.7.0/src/redturtle/prenotazioni/browser/static/widget/js/WidgetDataContainer/index.less`

 * *Files identical despite different names*

### Comparing `redturtle.prenotazioni-2.6.5/src/redturtle/prenotazioni/browser/static/widget/js/fields/DaysTableField.js` & `redturtle.prenotazioni-2.7.0/src/redturtle/prenotazioni/browser/static/widget/js/fields/DaysTableField.js`

 * *Files identical despite different names*

### Comparing `redturtle.prenotazioni-2.6.5/src/redturtle/prenotazioni/browser/static/widget/js/fields/GatesField.js` & `redturtle.prenotazioni-2.7.0/src/redturtle/prenotazioni/browser/static/widget/js/fields/GatesField.js`

 * *Files identical despite different names*

### Comparing `redturtle.prenotazioni-2.6.5/src/redturtle/prenotazioni/browser/static/widget/js/fields/IntervalSelectorField.js` & `redturtle.prenotazioni-2.7.0/src/redturtle/prenotazioni/browser/static/widget/js/fields/IntervalSelectorField.js`

 * *Files identical despite different names*

### Comparing `redturtle.prenotazioni-2.6.5/src/redturtle/prenotazioni/browser/static/widget/js/fields/PauseTableField.js` & `redturtle.prenotazioni-2.7.0/src/redturtle/prenotazioni/browser/static/widget/js/fields/PauseTableField.js`

 * *Files identical despite different names*

### Comparing `redturtle.prenotazioni-2.6.5/src/redturtle/prenotazioni/browser/static/widget/js/fields/SelectField.js` & `redturtle.prenotazioni-2.7.0/src/redturtle/prenotazioni/browser/static/widget/js/fields/SelectField.js`

 * *Files identical despite different names*

### Comparing `redturtle.prenotazioni-2.6.5/src/redturtle/prenotazioni/browser/static/widget/js/fields/TextLineField.js` & `redturtle.prenotazioni-2.7.0/src/redturtle/prenotazioni/browser/static/widget/js/fields/TextLineField.js`

 * *Files identical despite different names*

### Comparing `redturtle.prenotazioni-2.6.5/src/redturtle/prenotazioni/browser/static/widget/js/index.js` & `redturtle.prenotazioni-2.7.0/src/redturtle/prenotazioni/browser/static/widget/js/index.js`

 * *Files identical despite different names*

### Comparing `redturtle.prenotazioni-2.6.5/src/redturtle/prenotazioni/browser/static/widget/js/utils/i18n.js` & `redturtle.prenotazioni-2.7.0/src/redturtle/prenotazioni/browser/static/widget/js/utils/i18n.js`

 * *Files identical despite different names*

### Comparing `redturtle.prenotazioni-2.6.5/src/redturtle/prenotazioni/browser/stats/booking_stats.pt` & `redturtle.prenotazioni-2.7.0/src/redturtle/prenotazioni/browser/stats/booking_stats.pt`

 * *Files identical despite different names*

### Comparing `redturtle.prenotazioni-2.6.5/src/redturtle/prenotazioni/browser/stats/booking_stats.py` & `redturtle.prenotazioni-2.7.0/src/redturtle/prenotazioni/browser/stats/booking_stats.py`

 * *Files identical despite different names*

### Comparing `redturtle.prenotazioni-2.6.5/src/redturtle/prenotazioni/browser/stats/configure.zcml` & `redturtle.prenotazioni-2.7.0/src/redturtle/prenotazioni/browser/stats/configure.zcml`

 * *Files identical despite different names*

### Comparing `redturtle.prenotazioni-2.6.5/src/redturtle/prenotazioni/browser/templates/booking_type_radio_widget.pt` & `redturtle.prenotazioni-2.7.0/src/redturtle/prenotazioni/browser/templates/booking_type_radio_widget.pt`

 * *Files identical despite different names*

### Comparing `redturtle.prenotazioni-2.6.5/src/redturtle/prenotazioni/browser/templates/custom_dgf_input.pt` & `redturtle.prenotazioni-2.7.0/src/redturtle/prenotazioni/browser/templates/custom_dgf_input.pt`

 * *Files identical despite different names*

### Comparing `redturtle.prenotazioni-2.6.5/src/redturtle/prenotazioni/browser/templates/delete_reservation.pt` & `redturtle.prenotazioni-2.7.0/src/redturtle/prenotazioni/browser/templates/delete_reservation.pt`

 * *Files identical despite different names*

### Comparing `redturtle.prenotazioni-2.6.5/src/redturtle/prenotazioni/browser/templates/manager_notification_mail.pt` & `redturtle.prenotazioni-2.7.0/src/redturtle/prenotazioni/browser/templates/manager_notification_mail.pt`

 * *Files identical despite different names*

### Comparing `redturtle.prenotazioni-2.6.5/src/redturtle/prenotazioni/browser/templates/prenotazione.pt` & `redturtle.prenotazioni-2.7.0/src/redturtle/prenotazioni/browser/templates/prenotazione.pt`

 * *Files identical despite different names*

### Comparing `redturtle.prenotazioni-2.6.5/src/redturtle/prenotazioni/browser/templates/prenotazione_add.pt` & `redturtle.prenotazioni-2.7.0/src/redturtle/prenotazioni/browser/templates/prenotazione_add.pt`

 * *Files identical despite different names*

### Comparing `redturtle.prenotazioni-2.6.5/src/redturtle/prenotazioni/browser/templates/prenotazione_macros.pt` & `redturtle.prenotazioni-2.7.0/src/redturtle/prenotazioni/browser/templates/prenotazione_macros.pt`

 * *Files identical despite different names*

### Comparing `redturtle.prenotazioni-2.6.5/src/redturtle/prenotazioni/browser/templates/prenotazione_move.pt` & `redturtle.prenotazioni-2.7.0/src/redturtle/prenotazioni/browser/templates/prenotazione_move.pt`

 * *Files identical despite different names*

### Comparing `redturtle.prenotazioni-2.6.5/src/redturtle/prenotazioni/browser/templates/prenotazione_print.pt` & `redturtle.prenotazioni-2.7.0/src/redturtle/prenotazioni/browser/templates/prenotazione_print.pt`

 * *Files identical despite different names*

### Comparing `redturtle.prenotazioni-2.6.5/src/redturtle/prenotazioni/browser/templates/prenotazioni_search.pt` & `redturtle.prenotazioni-2.7.0/src/redturtle/prenotazioni/browser/templates/prenotazioni_search.pt`

 * *Files identical despite different names*

### Comparing `redturtle.prenotazioni-2.6.5/src/redturtle/prenotazioni/browser/templates/week.pt` & `redturtle.prenotazioni-2.7.0/src/redturtle/prenotazioni/browser/templates/week.pt`

 * *Files identical despite different names*

### Comparing `redturtle.prenotazioni-2.6.5/src/redturtle/prenotazioni/browser/utilities/notify_upcoming_bookings.py` & `redturtle.prenotazioni-2.7.0/src/redturtle/prenotazioni/browser/utilities/notify_upcoming_bookings.py`

 * *Files identical despite different names*

### Comparing `redturtle.prenotazioni-2.6.5/src/redturtle/prenotazioni/browser/vacations.py` & `redturtle.prenotazioni-2.7.0/src/redturtle/prenotazioni/browser/vacations.py`

 * *Files identical despite different names*

### Comparing `redturtle.prenotazioni-2.6.5/src/redturtle/prenotazioni/browser/viewlets.py` & `redturtle.prenotazioni-2.7.0/src/redturtle/prenotazioni/browser/viewlets.py`

 * *Files identical despite different names*

### Comparing `redturtle.prenotazioni-2.6.5/src/redturtle/prenotazioni/browser/week.py` & `redturtle.prenotazioni-2.7.0/src/redturtle/prenotazioni/browser/week.py`

 * *Files 2% similar despite different names*

```diff
@@ -224,15 +224,15 @@
         booking_url = self.prenotazioni.get_anonymous_booking_url(day, slot)
         message = _(
             "foreseen_booking_time",
             default="Foreseen booking time: ${booking_time}",
             mapping={
                 "booking_time": booking_url["title"],
                 "day": "{} {}".format(
-                    self.context.translate(
+                    api.portal.translate(
                         self.get_day_msgid(day), domain="plonelocales"
                     ),
                     day.strftime("%d"),
                 ),
             },
         )
         return message
@@ -255,15 +255,15 @@
 
         message = _(
             "prenotation_slot_message",
             default="${day}, ore ${booking_time}",
             mapping={
                 "booking_time": link["title"],
                 "day": "{} {}".format(
-                    self.context.translate(
+                    api.portal.translate(
                         self.get_day_msgid(day), domain="plonelocales"
                     ),
                     day.strftime("%d"),
                 ),
             },
         )
         return message
@@ -275,15 +275,15 @@
 
         message = _(
             "booked_prenotation_message",
             default="${day}, ore ${booking_time}, prenotato da ${booked_by}, prenotazione: ${booking_type} durata: ${duration} minuti",
             mapping={
                 "booking_time": booking.Date().strftime("%H:%M"),
                 "day": "{} {}".format(
-                    self.context.translate(
+                    api.portal.translate(
                         self.get_day_msgid(day), domain="plonelocales"
                     ),
                     day.strftime("%d"),
                 ),
                 "booked_by": booking.Title(),
                 "duration": booking.getDuration().seconds // 60,
                 "booking_type": booking.getBooking_type() or "",
```

### Comparing `redturtle.prenotazioni-2.6.5/src/redturtle/prenotazioni/browser/widget.py` & `redturtle.prenotazioni-2.7.0/src/redturtle/prenotazioni/browser/widget.py`

 * *Files identical despite different names*

### Comparing `redturtle.prenotazioni-2.6.5/src/redturtle/prenotazioni/browser/z3c_custom_widget.py` & `redturtle.prenotazioni-2.7.0/src/redturtle/prenotazioni/browser/z3c_custom_widget.py`

 * *Files 3% similar despite different names*

```diff
@@ -143,17 +143,17 @@
                     "index": count,
                 }
             )
         return results
 
     def get_radio_message(self, label):
         message = "{} {}, {}".format(
-            self.context.translate(_("Field", "Campo")),
-            self.context.translate(label),
-            self.context.translate(
+            api.portal.translate(_("Field", "Campo")),
+            api.portal.translate(label),
+            api.portal.translate(
                 _(
                     "select-option",
                     "seleziona l'opzione desiderata dal gruppo di radio button seguente",
                 )
             ),
         )
         return message
```

### Comparing `redturtle.prenotazioni-2.6.5/src/redturtle/prenotazioni/configure.zcml` & `redturtle.prenotazioni-2.7.0/src/redturtle/prenotazioni/configure.zcml`

 * *Files identical despite different names*

### Comparing `redturtle.prenotazioni-2.6.5/src/redturtle/prenotazioni/content/pause.py` & `redturtle.prenotazioni-2.7.0/src/redturtle/prenotazioni/content/pause.py`

 * *Files identical despite different names*

### Comparing `redturtle.prenotazioni-2.6.5/src/redturtle/prenotazioni/content/prenotazione.py` & `redturtle.prenotazioni-2.7.0/src/redturtle/prenotazioni/content/prenotazione.py`

 * *Files identical despite different names*

### Comparing `redturtle.prenotazioni-2.6.5/src/redturtle/prenotazioni/content/prenotazione_type.py` & `redturtle.prenotazioni-2.7.0/src/redturtle/prenotazioni/content/prenotazione_type.py`

 * *Files identical despite different names*

### Comparing `redturtle.prenotazioni-2.6.5/src/redturtle/prenotazioni/content/prenotazioni_folder.py` & `redturtle.prenotazioni-2.7.0/src/redturtle/prenotazioni/content/prenotazioni_folder.py`

 * *Files 1% similar despite different names*

```diff
@@ -464,14 +464,23 @@
         description=_(
             "notify_on_refuse_help",
             default="Notify via mail the user when his booking has been rejected.",
         ),
         default=False,
         required=False,
     )
+    notify_on_cancel = schema.Bool(
+        title=_("notify_on_cancel", default="Notify when canceled."),
+        description=_(
+            "notify_on_cancel_help",
+            default="Notify via mail the user when his booking has been canceled.",
+        ),
+        default=False,
+        required=False,
+    )
     max_bookings_allowed = schema.Int(
         title=_(
             "max_bookings_allowed_label",
             default="Maximum bookings number allowed",
         ),
         description=_(
             "max_bookings_allowed_description",
@@ -536,14 +545,15 @@
         fields=[
             "email_responsabile",
             "reminder_notification_gap",
             "notify_on_submit",
             "notify_on_confirm",
             "notify_on_move",
             "notify_on_refuse",
+            "notify_on_cancel",
         ],
     )
 
     @invariant
     def puse_table_invariant(data):
         validate_pause_table(data=data)
 
@@ -578,15 +588,15 @@
         return self.listFolderContents(
             contentFilter={"portal_type": "PrenotazioneType"}
         )
 
     def get_notification_flags(self):
         return {
             action: getattr(self, f"notify_on_{action}", False)
-            for action in ("confirm", "submit", "refuse")
+            for action in ("confirm", "submit", "refuse", "cancel")
         }
 
     # BBB: compatibility with old code (booking_types was a List of IBookingTypeRow)
     @property
     def booking_types(self):
         return [
             {
```

### Comparing `redturtle.prenotazioni-2.6.5/src/redturtle/prenotazioni/content/validators.py` & `redturtle.prenotazioni-2.7.0/src/redturtle/prenotazioni/content/validators.py`

 * *Files identical despite different names*

### Comparing `redturtle.prenotazioni-2.6.5/src/redturtle/prenotazioni/demo/configure.zcml` & `redturtle.prenotazioni-2.7.0/src/redturtle/prenotazioni/demo/configure.zcml`

 * *Files identical despite different names*

### Comparing `redturtle.prenotazioni-2.6.5/src/redturtle/prenotazioni/demo/setuphandlers.py` & `redturtle.prenotazioni-2.7.0/src/redturtle/prenotazioni/demo/setuphandlers.py`

 * *Files identical despite different names*

### Comparing `redturtle.prenotazioni-2.6.5/src/redturtle/prenotazioni/demo/smsdemo.py` & `redturtle.prenotazioni-2.7.0/src/redturtle/prenotazioni/demo/smsdemo.py`

 * *Files identical despite different names*

### Comparing `redturtle.prenotazioni-2.6.5/src/redturtle/prenotazioni/events/configure.zcml` & `redturtle.prenotazioni-2.7.0/src/redturtle/prenotazioni/events/configure.zcml`

 * *Files identical despite different names*

### Comparing `redturtle.prenotazioni-2.6.5/src/redturtle/prenotazioni/events/events_logger.py` & `redturtle.prenotazioni-2.7.0/src/redturtle/prenotazioni/events/events_logger.py`

 * *Files 8% similar despite different names*

```diff
@@ -61,23 +61,24 @@
         "gate",
         "phone",
         "staff_notes",
         "booking_type",
         "title",
     ]
     pr = api.portal.get_tool(name="portal_repository")
+
     try:
         old = pr.retrieve(obj, old_version).object
     except Exception:
         # ArchivistRetrieveError see https://github.com/RedTurtle/redturtle.prenotazioni/pull/178
         logger.exception("error on_modify %s", obj.absolute_url())
         return
 
     changes = []
     for fname in fnames:
-        c_value = obj.getField(fname, obj).get(obj)
-        o_value = old.getField(fname, old).get(old)
+        c_value = getattr(obj, fname)
+        o_value = getattr(old, fname)
         if c_value != o_value:
             changes.append({"new_" + fname: c_value, "old_" + fname: o_value})
 
     data = ["changed", dumps(changes)]
     log_data_for_booking(obj, data)
```

### Comparing `redturtle.prenotazioni-2.6.5/src/redturtle/prenotazioni/events/prenotazione.py` & `redturtle.prenotazioni-2.7.0/src/redturtle/prenotazioni/events/prenotazione.py`

 * *Files identical despite different names*

### Comparing `redturtle.prenotazioni-2.6.5/src/redturtle/prenotazioni/events/prenotazioni_folder.py` & `redturtle.prenotazioni-2.7.0/src/redturtle/prenotazioni/events/prenotazioni_folder.py`

 * *Files identical despite different names*

### Comparing `redturtle.prenotazioni-2.6.5/src/redturtle/prenotazioni/exceptions/booker.py` & `redturtle.prenotazioni-2.7.0/src/redturtle/prenotazioni/exceptions/booker.py`

 * *Files identical despite different names*

### Comparing `redturtle.prenotazioni-2.6.5/src/redturtle/prenotazioni/indexers/prenotazione.py` & `redturtle.prenotazioni-2.7.0/src/redturtle/prenotazioni/indexers/prenotazione.py`

 * *Files identical despite different names*

### Comparing `redturtle.prenotazioni-2.6.5/src/redturtle/prenotazioni/interfaces.py` & `redturtle.prenotazioni-2.7.0/src/redturtle/prenotazioni/interfaces.py`

 * *Files identical despite different names*

### Comparing `redturtle.prenotazioni-2.6.5/src/redturtle/prenotazioni/io_tools/README.md` & `redturtle.prenotazioni-2.7.0/src/redturtle/prenotazioni/io_tools/README.md`

 * *Files identical despite different names*

### Comparing `redturtle.prenotazioni-2.6.5/src/redturtle/prenotazioni/io_tools/api.py` & `redturtle.prenotazioni-2.7.0/src/redturtle/prenotazioni/io_tools/api.py`

 * *Files identical despite different names*

### Comparing `redturtle.prenotazioni-2.6.5/src/redturtle/prenotazioni/io_tools/cli.py` & `redturtle.prenotazioni-2.7.0/src/redturtle/prenotazioni/io_tools/cli.py`

 * *Files identical despite different names*

### Comparing `redturtle.prenotazioni-2.6.5/src/redturtle/prenotazioni/io_tools/io.db` & `redturtle.prenotazioni-2.7.0/src/redturtle/prenotazioni/io_tools/io.db`

 * *Files identical despite different names*

### Comparing `redturtle.prenotazioni-2.6.5/src/redturtle/prenotazioni/io_tools/monkey.py` & `redturtle.prenotazioni-2.7.0/src/redturtle/prenotazioni/io_tools/monkey.py`

 * *Files identical despite different names*

### Comparing `redturtle.prenotazioni-2.6.5/src/redturtle/prenotazioni/io_tools/rdbms.py` & `redturtle.prenotazioni-2.7.0/src/redturtle/prenotazioni/io_tools/rdbms.py`

 * *Files identical despite different names*

### Comparing `redturtle.prenotazioni-2.6.5/src/redturtle/prenotazioni/io_tools/spec.yaml` & `redturtle.prenotazioni-2.7.0/src/redturtle/prenotazioni/io_tools/spec.yaml`

 * *Files identical despite different names*

### Comparing `redturtle.prenotazioni-2.6.5/src/redturtle/prenotazioni/io_tools/storage.py` & `redturtle.prenotazioni-2.7.0/src/redturtle/prenotazioni/io_tools/storage.py`

 * *Files identical despite different names*

### Comparing `redturtle.prenotazioni-2.6.5/src/redturtle/prenotazioni/locales/en/LC_MESSAGES/redturtle.prenotazioni.po` & `redturtle.prenotazioni-2.7.0/src/redturtle/prenotazioni/locales/en/LC_MESSAGES/redturtle.prenotazioni.po`

 * *Files 5% similar despite different names*

```diff
@@ -1,11 +1,11 @@
 msgid ""
 msgstr ""
 "Project-Id-Version: PACKAGE VERSION\n"
-"POT-Creation-Date: 2024-03-29 10:56+0000\n"
+"POT-Creation-Date: 2024-05-21 14:53+0000\n"
 "PO-Revision-Date: YEAR-MO-DA HO:MI +ZONE\n"
 "Last-Translator: FULL NAME <EMAIL@ADDRESS>\n"
 "Language-Team: LANGUAGE <LL@li.org>\n"
 "MIME-Version: 1.0\n"
 "Content-Type: text/plain; charset=utf-8\n"
 "Content-Transfer-Encoding: 8bit\n"
 "Plural-Forms: nplurals=1; plural=0\n"
@@ -76,24 +76,32 @@
 msgid "Booking for"
 msgstr ""
 
 #: redturtle/prenotazioni/behaviors/booking_folder/notifications/appio/configure.zcml:27
 msgid "Booking type notification appio"
 msgstr ""
 
+#: redturtle/prenotazioni/profiles/default/workflows/prenotazioni_workflow/definition.xml
+msgid "Canceled"
+msgstr ""
+
 #. Default: "Change date/time"
 #: redturtle/prenotazioni/profiles/default/actions.xml
 msgid "Change date/time"
 msgstr ""
 
 #. Default: "Complete address"
 #: redturtle/prenotazioni/behaviors/booking_folder/contacts.py:43
 msgid "Complete address"
 msgstr ""
 
+#: redturtle/prenotazioni/profiles/default/workflows/prenotazioni_workflow/definition.xml
+msgid "Confirmed"
+msgstr ""
+
 #: redturtle/prenotazioni/behaviors/booking_folder/contacts.py:36
 msgid "Contact PEC"
 msgstr ""
 
 #: redturtle/prenotazioni/behaviors/booking_folder/contacts.py:30
 msgid "Contact fax"
 msgstr ""
@@ -110,23 +118,27 @@
 msgid "Contatti cartella prenotazioni"
 msgstr ""
 
 #: redturtle/prenotazioni/browser/templates/prenotazioni_search.pt:46
 msgid "Content listing"
 msgstr ""
 
+#: redturtle/prenotazioni/behaviors/booking_folder/notifications/__init__.py:34
+msgid "Could not send {gateway_type} message due to internal errors"
+msgstr ""
+
 #: redturtle/prenotazioni/content/prenotazioni_folder.py:207
 msgid "Data fine validità"
 msgstr ""
 
 #: redturtle/prenotazioni/content/prenotazioni_folder.py:204
 msgid "Data inizio validità"
 msgstr ""
 
-#: redturtle/prenotazioni/content/prenotazioni_folder.py:498
+#: redturtle/prenotazioni/content/prenotazioni_folder.py:507
 msgid "Date validità"
 msgstr ""
 
 #: redturtle/prenotazioni/content/prenotazioni_folder.py:367
 msgid "Days booking is not allowed before"
 msgstr ""
 
@@ -140,15 +152,15 @@
 
 #: redturtle/prenotazioni/profiles/default/types/Prenotazione.xml
 #: redturtle/prenotazioni/profiles/default/types/PrenotazioneType.xml
 #: redturtle/prenotazioni/profiles/default/types/PrenotazioniDay.xml
 msgid "Edit"
 msgstr ""
 
-#: redturtle/prenotazioni/behaviors/booking_folder/notifications/email/__init__.py:131
+#: redturtle/prenotazioni/behaviors/booking_folder/notifications/email/__init__.py:151
 msgid "Email from"
 msgstr ""
 
 #: redturtle/prenotazioni/content/prenotazione.py:175
 msgid "Expiration date booking"
 msgstr ""
 
@@ -186,15 +198,15 @@
 msgid "Inserire il testo di presentazione dell'agenda corrente"
 msgstr ""
 
 #: redturtle/prenotazioni/content/prenotazioni_folder.py:405
 msgid "Insert a list of email addresses that will be notified when new bookings get created."
 msgstr ""
 
-#: redturtle/prenotazioni/behaviors/booking_folder/notifications/email/__init__.py:132
+#: redturtle/prenotazioni/behaviors/booking_folder/notifications/email/__init__.py:152
 msgid "Insert an email address used as \"from\" in email notifications. Leave empty to use the default from set in the site configuration."
 msgstr ""
 
 #: redturtle/prenotazioni/behaviors/booking_folder/contacts.py:20
 msgid "Insert here indications on how to reach the office"
 msgstr ""
 
@@ -289,14 +301,18 @@
 msgid "Pause should be included in morning slot or afternoon slot"
 msgstr ""
 
 #: redturtle/prenotazioni/content/prenotazioni_folder.py:316
 msgid "Pause table"
 msgstr ""
 
+#: redturtle/prenotazioni/profiles/default/workflows/prenotazioni_workflow/definition.xml
+msgid "Pending"
+msgstr ""
+
 #: redturtle/prenotazioni/browser/prenotazione_add.py:220
 msgid "Please provide a booking date"
 msgstr ""
 
 #: redturtle/prenotazioni/profiles/default/types/Prenotazione.xml
 msgid "Prenotazione"
 msgstr ""
@@ -313,15 +329,23 @@
 msgid "PrenotazioniYear"
 msgstr ""
 
 #: redturtle/prenotazioni/browser/templates/prenotazione_print.pt:129
 msgid "Print"
 msgstr ""
 
-#: redturtle/prenotazioni/restapi/services/booking/add.py:122
+#: redturtle/prenotazioni/profiles/default/workflows/prenotazioni_workflow/definition.xml
+msgid "Private"
+msgstr ""
+
+#: redturtle/prenotazioni/profiles/default/workflows/prenotazioni_workflow/definition.xml
+msgid "Refused"
+msgstr ""
+
+#: redturtle/prenotazioni/restapi/services/booking/add.py:120
 msgid "Required input '${field}' is missing."
 msgstr ""
 
 #: redturtle/prenotazioni/browser/prenotazione_add.py:216
 msgid "Required input is missing."
 msgstr ""
 
@@ -338,15 +362,15 @@
 msgstr ""
 
 #: redturtle/prenotazioni/content/prenotazioni_folder.py:107
 msgid "Select a day"
 msgstr ""
 
 #: redturtle/prenotazioni/adapters/booker.py:299
-#: redturtle/prenotazioni/restapi/services/booking/add.py:64
+#: redturtle/prenotazioni/restapi/services/booking/add.py:63
 msgid "Sorry, this slot is not available anymore."
 msgstr ""
 
 #: redturtle/prenotazioni/adapters/booker.py:342
 msgid "Sorry, this slot is not available or does not fit your booking."
 msgstr ""
 
@@ -466,15 +490,15 @@
 msgid "Uninstalls the redturtle.prenotazioni add-on."
 msgstr ""
 
 #: redturtle/prenotazioni/demo/configure.zcml:25
 msgid "Uninstalls the redturtle.prenotazioni.demo add-on (demo site purpose only)."
 msgstr ""
 
-#: redturtle/prenotazioni/restapi/services/booking/add.py:158
+#: redturtle/prenotazioni/restapi/services/booking/add.py:156
 msgid "Unknown booking type '${booking_type}'."
 msgstr ""
 
 #: redturtle/prenotazioni/content/prenotazioni_folder.py:151
 msgid "Usage of `max_bookings_allowed` field requires the `fiscalcode` to be between the required fields."
 msgstr ""
 
@@ -492,15 +516,15 @@
 msgid "Week table"
 msgstr ""
 
 #: redturtle/prenotazioni/content/prenotazioni_folder.py:218
 msgid "Yes"
 msgstr ""
 
-#: redturtle/prenotazioni/restapi/services/booking/add.py:115
+#: redturtle/prenotazioni/restapi/services/booking/add.py:113
 msgid "You are not allowed to force the gate."
 msgstr ""
 
 #: redturtle/prenotazioni/content/validators.py:70
 msgid "You must set both start and end"
 msgstr ""
 
@@ -588,15 +612,15 @@
 
 #. Default: "All bookings created by Managers will be automatically accepted."
 #: redturtle/prenotazioni/content/prenotazioni_folder.py:395
 msgid "auto_confirm_manager_help"
 msgstr ""
 
 #. Default: "End date should be greater than start."
-#: redturtle/prenotazioni/restapi/services/available_slots/get.py:61
+#: redturtle/prenotazioni/restapi/services/available_slots/get.py:63
 msgid "available_slots_wrong_dates"
 msgstr ""
 
 #. Default: "Please select a booking slot."
 #: redturtle/prenotazioni/browser/templates/week.pt:40
 msgid "book_it"
 msgstr ""
@@ -608,15 +632,15 @@
 
 #. Default: "${day}, ore ${booking_time}, prenotato da ${booked_by}, prenotazione: ${booking_type} durata: ${duration} minuti"
 #: redturtle/prenotazioni/browser/week.py:276
 msgid "booked_prenotation_message"
 msgstr ""
 
 #. Default: "Booking canceled: "
-#: redturtle/prenotazioni/behaviors/booking_folder/notifications/email/notification_email_message.py:326
+#: redturtle/prenotazioni/behaviors/booking_folder/notifications/email/notification_email_message.py:368
 msgid "booking_canceled_mail_subject_part"
 msgstr ""
 
 #. Default: "Booking confirmed"
 #: redturtle/prenotazioni/browser/templates/prenotazione_macros.pt:456
 msgid "booking_confirmed"
 msgstr ""
@@ -628,15 +652,15 @@
 
 #. Default: "Your booking has been deleted."
 #: redturtle/prenotazioni/browser/delete_reservation.py:115
 msgid "booking_deleted_success"
 msgstr ""
 
 #. Default: "Booking fields"
-#: redturtle/prenotazioni/content/prenotazioni_folder.py:527
+#: redturtle/prenotazioni/content/prenotazioni_folder.py:536
 msgid "booking_fields_label"
 msgstr ""
 
 #: redturtle/prenotazioni/browser/prenotazione_move.py:135
 msgid "booking_moved"
 msgstr ""
 
@@ -682,50 +706,50 @@
 
 #. Default: "The following tipologies will not fit the time you selected:"
 #: redturtle/prenotazioni/browser/templates/booking_type_radio_widget.pt:65
 msgid "booking_type_widget_warn_unavailable"
 msgstr ""
 
 #. Default: "Set message text for all available notification events."
-#: redturtle/prenotazioni/behaviors/booking_folder/notifications/appio/__init__.py:257
+#: redturtle/prenotazioni/behaviors/booking_folder/notifications/appio/__init__.py:301
 msgid "bookings_appio_templates_help"
 msgstr ""
 
 #. Default: "AppIO Notifications"
-#: redturtle/prenotazioni/behaviors/booking_folder/notifications/appio/__init__.py:253
+#: redturtle/prenotazioni/behaviors/booking_folder/notifications/appio/__init__.py:297
 msgid "bookings_appio_templates_label"
 msgstr ""
 
 #. Default: "Set message text for all available notification events."
-#: redturtle/prenotazioni/behaviors/booking_folder/notifications/email/__init__.py:266
+#: redturtle/prenotazioni/behaviors/booking_folder/notifications/email/__init__.py:310
 msgid "bookings_email_templates_help"
 msgstr ""
 
 #. Default: "Email Notifications"
-#: redturtle/prenotazioni/behaviors/booking_folder/notifications/email/__init__.py:262
+#: redturtle/prenotazioni/behaviors/booking_folder/notifications/email/__init__.py:306
 msgid "bookings_email_templates_label"
 msgstr ""
 
 #. Default: "Booking limit({limit}) for the {booking_type} type is exceed for the current user"
 #: redturtle/prenotazioni/exceptions/booker.py:15
 msgid "bookings_limit_exceeded_exception"
 msgstr ""
 
 #. Default: "Bookings not in agenda"
 #: redturtle/prenotazioni/browser/templates/prenotazione_macros.pt:111
 msgid "bookings_not_in_agenda"
 msgstr ""
 
 #. Default: "Set message text for all available notification events. Remember that SMS has a 160 characters limit. Depending on your gateway service, it can split messages, if you exceed that limit."
-#: redturtle/prenotazioni/behaviors/booking_folder/notifications/sms/__init__.py:144
+#: redturtle/prenotazioni/behaviors/booking_folder/notifications/sms/__init__.py:166
 msgid "bookings_sms_templates_help"
 msgstr ""
 
 #. Default: "SMS Notifications"
-#: redturtle/prenotazioni/behaviors/booking_folder/notifications/sms/__init__.py:140
+#: redturtle/prenotazioni/behaviors/booking_folder/notifications/sms/__init__.py:162
 msgid "bookings_sms_templates_label"
 msgstr ""
 
 #. Default: "Busy"
 #: redturtle/prenotazioni/browser/prenotazioni_context_state.py:45
 msgid "busy"
 msgstr ""
@@ -873,14 +897,69 @@
 msgstr ""
 
 #. Default: "User will not be able to add a booking unless those fields are filled. Remember that, whatever you selected in this list, users have to supply at least one of \"Email\" or \"Telephone\""
 #: redturtle/prenotazioni/content/prenotazioni_folder.py:172
 msgid "help_visible_booking_fields"
 msgstr ""
 
+#. Default: "AppIO reminder was sent"
+#: redturtle/prenotazioni/behaviors/booking_folder/notifications/appio/notfication_appio_message.py:107
+msgid "history_appio_reminder_sent"
+msgstr ""
+
+#. Default: "AppIO message about the booking reschedule was sent"
+#: redturtle/prenotazioni/behaviors/booking_folder/notifications/appio/notfication_appio_message.py:35
+msgid "history_appio_reschedule_sent"
+msgstr ""
+
+#. Default: "AppIO message about the ${transition} transition was sent."
+#: redturtle/prenotazioni/behaviors/booking_folder/notifications/appio/notfication_appio_message.py:73
+msgid "history_appio_transition_sent"
+msgstr ""
+
+#. Default: "Email notification was sent to booking manager"
+#: redturtle/prenotazioni/behaviors/booking_folder/notifications/email/notification_email_message.py:258
+msgid "history_email_manager_notification_sent"
+msgstr ""
+
+#. Default: "Email message about the booking reschedule was sent"
+#: redturtle/prenotazioni/behaviors/booking_folder/notifications/email/notification_email_message.py:129
+msgid "history_email_reschedule_sent"
+msgstr ""
+
+#. Default: "Email message about the ${transition} transition was sent"
+#: redturtle/prenotazioni/behaviors/booking_folder/notifications/email/notification_email_message.py:165
+msgid "history_email_transition_sent"
+msgstr ""
+
+#. Default: "Email reminder was sent"
+#: redturtle/prenotazioni/behaviors/booking_folder/notifications/email/notification_email_message.py:213
+msgid "history_reminder_sent"
+msgstr ""
+
+#. Default: "SMS reminder was sent"
+#: redturtle/prenotazioni/behaviors/booking_folder/notifications/sms/message.py:100
+msgid "history_sms_reminder_sent"
+msgstr ""
+
+#. Default: "SMS removed notification was sent"
+#: redturtle/prenotazioni/behaviors/booking_folder/notifications/sms/message.py:120
+msgid "history_sms_removed_sent"
+msgstr ""
+
+#. Default: "SMS message about the booking reschedule was sent"
+#: redturtle/prenotazioni/behaviors/booking_folder/notifications/sms/message.py:49
+msgid "history_sms_reschedule_sent"
+msgstr ""
+
+#. Default: "SMS message about the ${transition} transition was sent"
+#: redturtle/prenotazioni/behaviors/booking_folder/notifications/sms/message.py:76
+msgid "history_sms_transition_sent"
+msgstr ""
+
 #. Default: "Set holidays (one for line) in DD/MM/YYYY. you can write * for the year, if this event is yearly."
 #: redturtle/prenotazioni/content/prenotazioni_folder.py:330
 msgid "holidays_help"
 msgstr ""
 
 #. Default: "Holidays"
 #: redturtle/prenotazioni/content/prenotazioni_folder.py:329
@@ -1100,20 +1179,20 @@
 
 #. Default: "The minimum value of a single slot is 5 minutes. You cannot book a reservation when the needed time exceeds the available time."
 #: redturtle/prenotazioni/browser/templates/prenotazione_macros.pt:469
 msgid "legend_note"
 msgstr ""
 
 #. Default: "The number of simultaneous bookings allowed for the same user."
-#: redturtle/prenotazioni/content/prenotazioni_folder.py:476
+#: redturtle/prenotazioni/content/prenotazioni_folder.py:485
 msgid "max_bookings_allowed_description"
 msgstr ""
 
 #. Default: "Maximum bookings number allowed"
-#: redturtle/prenotazioni/content/prenotazioni_folder.py:472
+#: redturtle/prenotazioni/content/prenotazioni_folder.py:481
 msgid "max_bookings_allowed_label"
 msgstr ""
 
 #. Default: "Unable to find a booking with the givend id: ${uid}."
 #: redturtle/prenotazioni/browser/delete_reservation.py:45
 msgid "missing_booking"
 msgstr ""
@@ -1160,103 +1239,164 @@
 
 #. Default: "Booking is not allowed before the amount of days specified. \nKeep 0 to give no limits."
 #: redturtle/prenotazioni/content/prenotazioni_folder.py:368
 msgid "notBeforeDays"
 msgstr ""
 
 #. Default: "Enable AppIO notifications."
-#: redturtle/prenotazioni/behaviors/booking_folder/notifications/appio/__init__.py:123
+#: redturtle/prenotazioni/behaviors/booking_folder/notifications/appio/__init__.py:143
 msgid "notifications_appio_enabled_help"
 msgstr ""
 
 #. Default: "AppIO notifications"
-#: redturtle/prenotazioni/behaviors/booking_folder/notifications/appio/__init__.py:122
+#: redturtle/prenotazioni/behaviors/booking_folder/notifications/appio/__init__.py:142
 msgid "notifications_appio_enabled_label"
 msgstr ""
 
 #. Default: "Enable Email notifications."
-#: redturtle/prenotazioni/behaviors/booking_folder/notifications/email/__init__.py:123
+#: redturtle/prenotazioni/behaviors/booking_folder/notifications/email/__init__.py:143
 msgid "notifications_email_enabled_help"
 msgstr ""
 
 #. Default: "Email notifications"
-#: redturtle/prenotazioni/behaviors/booking_folder/notifications/email/__init__.py:122
+#: redturtle/prenotazioni/behaviors/booking_folder/notifications/email/__init__.py:142
 msgid "notifications_email_enabled_label"
 msgstr ""
 
 #. Default: "Notifications"
-#: redturtle/prenotazioni/content/prenotazioni_folder.py:535
+#: redturtle/prenotazioni/content/prenotazioni_folder.py:544
 msgid "notifications_label"
 msgstr ""
 
 #. Default: "Enable SMS notifications."
-#: redturtle/prenotazioni/behaviors/booking_folder/notifications/sms/__init__.py:70
+#: redturtle/prenotazioni/behaviors/booking_folder/notifications/sms/__init__.py:80
 msgid "notifications_sms_enabled_help"
 msgstr ""
 
 #. Default: "SMS notifications"
-#: redturtle/prenotazioni/behaviors/booking_folder/notifications/sms/__init__.py:69
+#: redturtle/prenotazioni/behaviors/booking_folder/notifications/sms/__init__.py:79
 msgid "notifications_sms_enabled_label"
 msgstr ""
 
 #. Default: "This is an automatic reminder about your booking on ${date} for ${booking_type}.<br/><br/>You can see details and print a reminder following this [link](${booking_print_url})."
-#: redturtle/prenotazioni/behaviors/booking_folder/notifications/appio/__init__.py:111
+#: redturtle/prenotazioni/behaviors/booking_folder/notifications/appio/__init__.py:131
 msgid "notify_as_reminder_appio_message_default_value"
 msgstr ""
 
 #. Default: "[${prenotazioni_folder_title}] Booking reminder on ${booking_date}"
-#: redturtle/prenotazioni/behaviors/booking_folder/notifications/appio/__init__.py:101
+#: redturtle/prenotazioni/behaviors/booking_folder/notifications/appio/__init__.py:121
 msgid "notify_as_reminder_appio_subject_default_value"
 msgstr ""
 
 #. Default: "The message subject when a reminder will be sent."
-#: redturtle/prenotazioni/behaviors/booking_folder/notifications/appio/__init__.py:231
+#: redturtle/prenotazioni/behaviors/booking_folder/notifications/appio/__init__.py:275
 msgid "notify_as_reminder_appio_subject_help"
 msgstr ""
 
 #. Default: "[Reminder] message"
-#: redturtle/prenotazioni/behaviors/booking_folder/notifications/appio/__init__.py:239
-#: redturtle/prenotazioni/behaviors/booking_folder/notifications/email/__init__.py:248
-#: redturtle/prenotazioni/behaviors/booking_folder/notifications/sms/__init__.py:126
+#: redturtle/prenotazioni/behaviors/booking_folder/notifications/appio/__init__.py:283
+#: redturtle/prenotazioni/behaviors/booking_folder/notifications/email/__init__.py:292
+#: redturtle/prenotazioni/behaviors/booking_folder/notifications/sms/__init__.py:148
 msgid "notify_as_reminder_message"
 msgstr ""
 
 #. Default: "This is an automatic reminder about your booking on ${date} for ${booking_type}.<br/><br/>You can see details and print a reminder following this <a href=${booking_print_url}>link</a>."
-#: redturtle/prenotazioni/behaviors/booking_folder/notifications/email/__init__.py:111
+#: redturtle/prenotazioni/behaviors/booking_folder/notifications/email/__init__.py:131
 msgid "notify_as_reminder_message_default_value"
 msgstr ""
 
 #. Default: "The message text when a reminder will be sent."
-#: redturtle/prenotazioni/behaviors/booking_folder/notifications/appio/__init__.py:243
-#: redturtle/prenotazioni/behaviors/booking_folder/notifications/email/__init__.py:252
-#: redturtle/prenotazioni/behaviors/booking_folder/notifications/sms/__init__.py:130
+#: redturtle/prenotazioni/behaviors/booking_folder/notifications/appio/__init__.py:287
+#: redturtle/prenotazioni/behaviors/booking_folder/notifications/email/__init__.py:296
+#: redturtle/prenotazioni/behaviors/booking_folder/notifications/sms/__init__.py:152
 msgid "notify_as_reminder_message_help"
 msgstr ""
 
 #. Default: "[${prenotazioni_folder_title}]: This is an automatic reminder about your booking on ${date} for ${booking_type} .\nSee details or delete it: ${booking_print_url} ."
-#: redturtle/prenotazioni/behaviors/booking_folder/notifications/sms/__init__.py:58
+#: redturtle/prenotazioni/behaviors/booking_folder/notifications/sms/__init__.py:68
 msgid "notify_as_reminder_sms_message_default_value"
 msgstr ""
 
 #. Default: "[Reminder] subject"
-#: redturtle/prenotazioni/behaviors/booking_folder/notifications/appio/__init__.py:227
-#: redturtle/prenotazioni/behaviors/booking_folder/notifications/email/__init__.py:236
+#: redturtle/prenotazioni/behaviors/booking_folder/notifications/appio/__init__.py:271
+#: redturtle/prenotazioni/behaviors/booking_folder/notifications/email/__init__.py:280
 msgid "notify_as_reminder_subject"
 msgstr ""
 
 #. Default: "[${prenotazioni_folder_title}] Booking reminder on ${booking_date}"
-#: redturtle/prenotazioni/behaviors/booking_folder/notifications/email/__init__.py:101
+#: redturtle/prenotazioni/behaviors/booking_folder/notifications/email/__init__.py:121
 msgid "notify_as_reminder_subject_default_value"
 msgstr ""
 
 #. Default: "The message subject when a reminder will be sent."
-#: redturtle/prenotazioni/behaviors/booking_folder/notifications/email/__init__.py:240
+#: redturtle/prenotazioni/behaviors/booking_folder/notifications/email/__init__.py:284
 msgid "notify_as_reminder_subject_help"
 msgstr ""
 
+#. Default: "Notify when canceled."
+#: redturtle/prenotazioni/content/prenotazioni_folder.py:472
+msgid "notify_on_cancel"
+msgstr ""
+
+#. Default: "The booking ${booking_type} of ${booking_date} at ${booking_time} was canceled."
+#: redturtle/prenotazioni/behaviors/booking_folder/notifications/appio/__init__.py:111
+msgid "notify_on_cancel_appio_message_default_value"
+msgstr ""
+
+#. Default: "[${prenotazioni_folder_title}] Booking canceled for ${title}"
+#: redturtle/prenotazioni/behaviors/booking_folder/notifications/appio/__init__.py:101
+msgid "notify_on_cancel_appio_subject_default_value"
+msgstr ""
+
+#. Default: "Notify via mail the user when his booking has been canceled."
+#: redturtle/prenotazioni/content/prenotazioni_folder.py:473
+msgid "notify_on_cancel_help"
+msgstr ""
+
+#. Default: "[Cancel] message"
+#: redturtle/prenotazioni/behaviors/booking_folder/notifications/appio/__init__.py:259
+#: redturtle/prenotazioni/behaviors/booking_folder/notifications/email/__init__.py:268
+#: redturtle/prenotazioni/behaviors/booking_folder/notifications/sms/__init__.py:136
+msgid "notify_on_cancel_message"
+msgstr ""
+
+#. Default: "The booking ${booking_type} of ${booking_date} at ${booking_time} was canceled."
+#: redturtle/prenotazioni/behaviors/booking_folder/notifications/email/__init__.py:111
+msgid "notify_on_cancel_message_default_value"
+msgstr ""
+
+#. Default: "The message text when a booking has been canceled."
+#: redturtle/prenotazioni/behaviors/booking_folder/notifications/appio/__init__.py:263
+#: redturtle/prenotazioni/behaviors/booking_folder/notifications/email/__init__.py:272
+#: redturtle/prenotazioni/behaviors/booking_folder/notifications/sms/__init__.py:140
+msgid "notify_on_cancel_message_help"
+msgstr ""
+
+#. Default: "[${prenotazioni_folder_title}]: The booking ${booking_type} of ${booking_date} at ${booking_time} was canceled."
+#: redturtle/prenotazioni/behaviors/booking_folder/notifications/sms/__init__.py:58
+msgid "notify_on_cancel_sms_message_default_value"
+msgstr ""
+
+#. Default: "[Cancel] subject"
+#: redturtle/prenotazioni/behaviors/booking_folder/notifications/appio/__init__.py:247
+#: redturtle/prenotazioni/behaviors/booking_folder/notifications/email/__init__.py:256
+msgid "notify_on_cancel_subject"
+msgstr ""
+
+#. Default: "[${prenotazioni_folder_title}] Booking canceled for ${title}"
+#: redturtle/prenotazioni/behaviors/booking_folder/notifications/email/__init__.py:101
+msgid "notify_on_cancel_subject_default_value"
+msgstr ""
+
+#. Default: "The message subject when a booking has been canceled."
+#: redturtle/prenotazioni/behaviors/booking_folder/notifications/appio/__init__.py:251
+#: redturtle/prenotazioni/behaviors/booking_folder/notifications/email/__init__.py:260
+msgid "notify_on_cancel_subject_help"
+msgstr ""
+
 #. Default: "Notify when confirmed."
 #: redturtle/prenotazioni/content/prenotazioni_folder.py:445
 msgid "notify_on_confirm"
 msgstr ""
 
 #. Default: "The booking ${booking_type} for ${title} has been confirmed.<br/><br/>You can see details and print a reminder following this [link](${booking_print_url})."
 #: redturtle/prenotazioni/behaviors/booking_folder/notifications/appio/__init__.py:48
@@ -1270,51 +1410,51 @@
 
 #. Default: "Notify via mail the user when his booking has been confirmed."
 #: redturtle/prenotazioni/content/prenotazioni_folder.py:446
 msgid "notify_on_confirm_help"
 msgstr ""
 
 #. Default: "[Confirmed] message"
-#: redturtle/prenotazioni/behaviors/booking_folder/notifications/appio/__init__.py:167
-#: redturtle/prenotazioni/behaviors/booking_folder/notifications/email/__init__.py:176
-#: redturtle/prenotazioni/behaviors/booking_folder/notifications/sms/__init__.py:90
+#: redturtle/prenotazioni/behaviors/booking_folder/notifications/appio/__init__.py:187
+#: redturtle/prenotazioni/behaviors/booking_folder/notifications/email/__init__.py:196
+#: redturtle/prenotazioni/behaviors/booking_folder/notifications/sms/__init__.py:100
 msgid "notify_on_confirm_message"
 msgstr ""
 
 #. Default: "The booking ${booking_type} for ${title} has been confirmed.<br/><br/>You can see details and print a reminder following this <a href=${booking_print_url}>link</a>."
 #: redturtle/prenotazioni/behaviors/booking_folder/notifications/email/__init__.py:48
 msgid "notify_on_confirm_message_default_value"
 msgstr ""
 
 #. Default: "The message text when a booking has been confirmed."
-#: redturtle/prenotazioni/behaviors/booking_folder/notifications/appio/__init__.py:171
-#: redturtle/prenotazioni/behaviors/booking_folder/notifications/email/__init__.py:180
-#: redturtle/prenotazioni/behaviors/booking_folder/notifications/sms/__init__.py:94
+#: redturtle/prenotazioni/behaviors/booking_folder/notifications/appio/__init__.py:191
+#: redturtle/prenotazioni/behaviors/booking_folder/notifications/email/__init__.py:200
+#: redturtle/prenotazioni/behaviors/booking_folder/notifications/sms/__init__.py:104
 msgid "notify_on_confirm_message_help"
 msgstr ""
 
 #. Default: "[${prenotazioni_folder_title}]: Booking of ${booking_date} at ${booking_time} has been accepted.\nSee details or delete it: ${booking_print_url} ."
 #: redturtle/prenotazioni/behaviors/booking_folder/notifications/sms/__init__.py:28
 msgid "notify_on_confirm_sms_message_default_value"
 msgstr ""
 
 #. Default: "[Confirm] subject"
-#: redturtle/prenotazioni/behaviors/booking_folder/notifications/appio/__init__.py:155
-#: redturtle/prenotazioni/behaviors/booking_folder/notifications/email/__init__.py:164
+#: redturtle/prenotazioni/behaviors/booking_folder/notifications/appio/__init__.py:175
+#: redturtle/prenotazioni/behaviors/booking_folder/notifications/email/__init__.py:184
 msgid "notify_on_confirm_subject"
 msgstr ""
 
 #. Default: "[${prenotazioni_folder_title}] Booking of ${booking_date} at ${booking_time} was accepted"
 #: redturtle/prenotazioni/behaviors/booking_folder/notifications/email/__init__.py:38
 msgid "notify_on_confirm_subject_default_value"
 msgstr ""
 
 #. Default: "The message subject when a booking has been confirmed."
-#: redturtle/prenotazioni/behaviors/booking_folder/notifications/appio/__init__.py:159
-#: redturtle/prenotazioni/behaviors/booking_folder/notifications/email/__init__.py:168
+#: redturtle/prenotazioni/behaviors/booking_folder/notifications/appio/__init__.py:179
+#: redturtle/prenotazioni/behaviors/booking_folder/notifications/email/__init__.py:188
 msgid "notify_on_confirm_subject_help"
 msgstr ""
 
 #. Default: "Notify when moved."
 #: redturtle/prenotazioni/content/prenotazioni_folder.py:454
 msgid "notify_on_move"
 msgstr ""
@@ -1331,51 +1471,51 @@
 
 #. Default: "Notify via mail the user when his booking has been moved."
 #: redturtle/prenotazioni/content/prenotazioni_folder.py:455
 msgid "notify_on_move_help"
 msgstr ""
 
 #. Default: "[Move] message"
-#: redturtle/prenotazioni/behaviors/booking_folder/notifications/appio/__init__.py:191
-#: redturtle/prenotazioni/behaviors/booking_folder/notifications/email/__init__.py:200
-#: redturtle/prenotazioni/behaviors/booking_folder/notifications/sms/__init__.py:102
+#: redturtle/prenotazioni/behaviors/booking_folder/notifications/appio/__init__.py:211
+#: redturtle/prenotazioni/behaviors/booking_folder/notifications/email/__init__.py:220
+#: redturtle/prenotazioni/behaviors/booking_folder/notifications/sms/__init__.py:112
 msgid "notify_on_move_message"
 msgstr ""
 
 #. Default: "The booking scheduling for ${booking_type} was modified.<br/><br/>The new one is on ${booking_date} at ${booking_time}.<br/><br/>You can see details and print a reminder following this <a href=${booking_print_url}>link</a>."
 #: redturtle/prenotazioni/behaviors/booking_folder/notifications/email/__init__.py:69
 msgid "notify_on_move_message_default_value"
 msgstr ""
 
 #. Default: "The message text when a booking has been moved."
-#: redturtle/prenotazioni/behaviors/booking_folder/notifications/appio/__init__.py:195
-#: redturtle/prenotazioni/behaviors/booking_folder/notifications/email/__init__.py:204
-#: redturtle/prenotazioni/behaviors/booking_folder/notifications/sms/__init__.py:106
+#: redturtle/prenotazioni/behaviors/booking_folder/notifications/appio/__init__.py:215
+#: redturtle/prenotazioni/behaviors/booking_folder/notifications/email/__init__.py:224
+#: redturtle/prenotazioni/behaviors/booking_folder/notifications/sms/__init__.py:116
 msgid "notify_on_move_message_help"
 msgstr ""
 
 #. Default: "[${prenotazioni_folder_title}]: The booking scheduling for ${booking_type} was modified.\nThe new one is on ${booking_date} at ${booking_time} .\nSee details or delete it: ${booking_print_url} ."
 #: redturtle/prenotazioni/behaviors/booking_folder/notifications/sms/__init__.py:38
 msgid "notify_on_move_sms_message_default_value"
 msgstr ""
 
 #. Default: "[Move] subject"
-#: redturtle/prenotazioni/behaviors/booking_folder/notifications/appio/__init__.py:179
-#: redturtle/prenotazioni/behaviors/booking_folder/notifications/email/__init__.py:188
+#: redturtle/prenotazioni/behaviors/booking_folder/notifications/appio/__init__.py:199
+#: redturtle/prenotazioni/behaviors/booking_folder/notifications/email/__init__.py:208
 msgid "notify_on_move_subject"
 msgstr ""
 
 #. Default: "[${prenotazioni_folder_title}] Booking date modified for ${title}"
 #: redturtle/prenotazioni/behaviors/booking_folder/notifications/email/__init__.py:59
 msgid "notify_on_move_subject_default_value"
 msgstr ""
 
 #. Default: "The message subject when a booking has been moved."
-#: redturtle/prenotazioni/behaviors/booking_folder/notifications/appio/__init__.py:183
-#: redturtle/prenotazioni/behaviors/booking_folder/notifications/email/__init__.py:192
+#: redturtle/prenotazioni/behaviors/booking_folder/notifications/appio/__init__.py:203
+#: redturtle/prenotazioni/behaviors/booking_folder/notifications/email/__init__.py:212
 msgid "notify_on_move_subject_help"
 msgstr ""
 
 #. Default: "Notify when rejected."
 #: redturtle/prenotazioni/content/prenotazioni_folder.py:463
 msgid "notify_on_refuse"
 msgstr ""
@@ -1392,51 +1532,51 @@
 
 #. Default: "Notify via mail the user when his booking has been rejected."
 #: redturtle/prenotazioni/content/prenotazioni_folder.py:464
 msgid "notify_on_refuse_help"
 msgstr ""
 
 #. Default: "[Refuse] message"
-#: redturtle/prenotazioni/behaviors/booking_folder/notifications/appio/__init__.py:215
-#: redturtle/prenotazioni/behaviors/booking_folder/notifications/email/__init__.py:224
-#: redturtle/prenotazioni/behaviors/booking_folder/notifications/sms/__init__.py:114
+#: redturtle/prenotazioni/behaviors/booking_folder/notifications/appio/__init__.py:235
+#: redturtle/prenotazioni/behaviors/booking_folder/notifications/email/__init__.py:244
+#: redturtle/prenotazioni/behaviors/booking_folder/notifications/sms/__init__.py:124
 msgid "notify_on_refuse_message"
 msgstr ""
 
 #. Default: "The booking ${booking_type} of ${booking_date} at ${booking_time} was refused."
 #: redturtle/prenotazioni/behaviors/booking_folder/notifications/email/__init__.py:91
 msgid "notify_on_refuse_message_default_value"
 msgstr ""
 
 #. Default: "The message text when a booking has been refused."
-#: redturtle/prenotazioni/behaviors/booking_folder/notifications/appio/__init__.py:219
-#: redturtle/prenotazioni/behaviors/booking_folder/notifications/email/__init__.py:228
-#: redturtle/prenotazioni/behaviors/booking_folder/notifications/sms/__init__.py:118
+#: redturtle/prenotazioni/behaviors/booking_folder/notifications/appio/__init__.py:239
+#: redturtle/prenotazioni/behaviors/booking_folder/notifications/email/__init__.py:248
+#: redturtle/prenotazioni/behaviors/booking_folder/notifications/sms/__init__.py:128
 msgid "notify_on_refuse_message_help"
 msgstr ""
 
 #. Default: "[${prenotazioni_folder_title}]: The booking ${booking_type} of ${booking_date} at ${booking_time} was refused."
 #: redturtle/prenotazioni/behaviors/booking_folder/notifications/sms/__init__.py:48
 msgid "notify_on_refuse_sms_message_default_value"
 msgstr ""
 
 #. Default: "[Refuse] subject"
-#: redturtle/prenotazioni/behaviors/booking_folder/notifications/appio/__init__.py:203
-#: redturtle/prenotazioni/behaviors/booking_folder/notifications/email/__init__.py:212
+#: redturtle/prenotazioni/behaviors/booking_folder/notifications/appio/__init__.py:223
+#: redturtle/prenotazioni/behaviors/booking_folder/notifications/email/__init__.py:232
 msgid "notify_on_refuse_subject"
 msgstr ""
 
 #. Default: "[${prenotazioni_folder_title}] Booking refused for ${title}"
 #: redturtle/prenotazioni/behaviors/booking_folder/notifications/email/__init__.py:81
 msgid "notify_on_refuse_subject_default_value"
 msgstr ""
 
 #. Default: "The message subject when a booking has been refused."
-#: redturtle/prenotazioni/behaviors/booking_folder/notifications/appio/__init__.py:207
-#: redturtle/prenotazioni/behaviors/booking_folder/notifications/email/__init__.py:216
+#: redturtle/prenotazioni/behaviors/booking_folder/notifications/appio/__init__.py:227
+#: redturtle/prenotazioni/behaviors/booking_folder/notifications/email/__init__.py:236
 msgid "notify_on_refuse_subject_help"
 msgstr ""
 
 #. Default: "Notify when created."
 #: redturtle/prenotazioni/content/prenotazioni_folder.py:436
 msgid "notify_on_submit"
 msgstr ""
@@ -1453,51 +1593,51 @@
 
 #. Default: "Notify via mail the user when his booking has been created. If auto-confirm flag is selected and confirm notify is selected, this one will be ignored."
 #: redturtle/prenotazioni/content/prenotazioni_folder.py:437
 msgid "notify_on_submit_help"
 msgstr ""
 
 #. Default: "[Created] message"
-#: redturtle/prenotazioni/behaviors/booking_folder/notifications/appio/__init__.py:143
-#: redturtle/prenotazioni/behaviors/booking_folder/notifications/email/__init__.py:152
-#: redturtle/prenotazioni/behaviors/booking_folder/notifications/sms/__init__.py:78
+#: redturtle/prenotazioni/behaviors/booking_folder/notifications/appio/__init__.py:163
+#: redturtle/prenotazioni/behaviors/booking_folder/notifications/email/__init__.py:172
+#: redturtle/prenotazioni/behaviors/booking_folder/notifications/sms/__init__.py:88
 msgid "notify_on_submit_message"
 msgstr ""
 
 #. Default: "Booking ${booking_type} for ${booking_date} at ${booking_time} has been created.<br/><br/>You can see details and print a reminder following this <a href=${booking_print_url}>link</a>."
 #: redturtle/prenotazioni/behaviors/booking_folder/notifications/email/__init__.py:28
 msgid "notify_on_submit_message_default_value"
 msgstr ""
 
 #. Default: "The message text when a booking has been created."
-#: redturtle/prenotazioni/behaviors/booking_folder/notifications/appio/__init__.py:147
-#: redturtle/prenotazioni/behaviors/booking_folder/notifications/email/__init__.py:156
-#: redturtle/prenotazioni/behaviors/booking_folder/notifications/sms/__init__.py:82
+#: redturtle/prenotazioni/behaviors/booking_folder/notifications/appio/__init__.py:167
+#: redturtle/prenotazioni/behaviors/booking_folder/notifications/email/__init__.py:176
+#: redturtle/prenotazioni/behaviors/booking_folder/notifications/sms/__init__.py:92
 msgid "notify_on_submit_message_help"
 msgstr ""
 
 #. Default: "[${prenotazioni_folder_title}]: Booking ${booking_type} for ${booking_date} at ${booking_time} has been created.\nSee details or delete it: ${booking_print_url} ."
 #: redturtle/prenotazioni/behaviors/booking_folder/notifications/sms/__init__.py:18
 msgid "notify_on_submit_sms_message_default_value"
 msgstr ""
 
 #. Default: "[Created] subject"
-#: redturtle/prenotazioni/behaviors/booking_folder/notifications/appio/__init__.py:131
-#: redturtle/prenotazioni/behaviors/booking_folder/notifications/email/__init__.py:140
+#: redturtle/prenotazioni/behaviors/booking_folder/notifications/appio/__init__.py:151
+#: redturtle/prenotazioni/behaviors/booking_folder/notifications/email/__init__.py:160
 msgid "notify_on_submit_subject"
 msgstr ""
 
 #. Default: "[${prenotazioni_folder_title}] Booking created"
 #: redturtle/prenotazioni/behaviors/booking_folder/notifications/email/__init__.py:18
 msgid "notify_on_submit_subject_default_value"
 msgstr ""
 
 #. Default: "The message subject when a booking has been created."
-#: redturtle/prenotazioni/behaviors/booking_folder/notifications/appio/__init__.py:135
-#: redturtle/prenotazioni/behaviors/booking_folder/notifications/email/__init__.py:144
+#: redturtle/prenotazioni/behaviors/booking_folder/notifications/appio/__init__.py:155
+#: redturtle/prenotazioni/behaviors/booking_folder/notifications/email/__init__.py:164
 msgid "notify_on_submit_subject_help"
 msgstr ""
 
 #. Default: "Pause end"
 #: redturtle/prenotazioni/content/prenotazioni_folder.py:124
 msgid "pause_end_label"
 msgstr ""
@@ -1563,20 +1703,20 @@
 
 #. Default: "Reject booking"
 #: redturtle/prenotazioni/browser/templates/prenotazione.pt:176
 msgid "reject_booking"
 msgstr ""
 
 #. Default: "Set how many days before of a booking date the user will be notified about it."
-#: redturtle/prenotazioni/content/prenotazioni_folder.py:488
+#: redturtle/prenotazioni/content/prenotazioni_folder.py:497
 msgid "reminder_notification_gap_description"
 msgstr ""
 
 #. Default: "Booking reminder days"
-#: redturtle/prenotazioni/content/prenotazioni_folder.py:484
+#: redturtle/prenotazioni/content/prenotazioni_folder.py:493
 msgid "reminder_notification_gap_label"
 msgstr ""
 
 #. Default: "Code"
 #: redturtle/prenotazioni/browser/templates/prenotazioni_search.pt:58
 msgid "reservation_code"
 msgstr ""
@@ -1618,20 +1758,20 @@
 
 #. Default: "seleziona l'opzione desiderata dal gruppo di radio button seguente"
 #: redturtle/prenotazioni/browser/z3c_custom_widget.py:153
 msgid "select-option"
 msgstr ""
 
 #. Default: "AppIO service code related to the current booking type"
-#: redturtle/prenotazioni/behaviors/booking_folder/notifications/appio/__init__.py:293
+#: redturtle/prenotazioni/behaviors/booking_folder/notifications/appio/__init__.py:339
 msgid "service_code_help"
 msgstr ""
 
 #. Default: "AppIO service code."
-#: redturtle/prenotazioni/behaviors/booking_folder/notifications/appio/__init__.py:289
+#: redturtle/prenotazioni/behaviors/booking_folder/notifications/appio/__init__.py:335
 msgid "service_code_label"
 msgstr ""
 
 #. Default: "This gate has some booking schedule in this time period."
 #: redturtle/prenotazioni/browser/vacations.py:216
 msgid "slot_conflict_error"
 msgstr ""
@@ -1651,15 +1791,15 @@
 
 #. Default: "Selected day is too big for that month for \"to\" field."
 #: redturtle/prenotazioni/content/validators.py:191
 msgid "to_month_too_days_error"
 msgstr ""
 
 #. Default: "You can't add a booking with type '${booking_type}'."
-#: redturtle/prenotazioni/restapi/services/booking/add.py:134
+#: redturtle/prenotazioni/restapi/services/booking/add.py:132
 msgid "unauthorized_add_vacation"
 msgstr ""
 
 #. Default: "Unbookable time"
 #: redturtle/prenotazioni/browser/templates/prenotazione_macros.pt:452
 msgid "unbookable_time"
 msgstr ""
```

### Comparing `redturtle.prenotazioni-2.6.5/src/redturtle/prenotazioni/locales/it/LC_MESSAGES/plone.po` & `redturtle.prenotazioni-2.7.0/src/redturtle/prenotazioni/locales/it/LC_MESSAGES/plone.po`

 * *Files 26% similar despite different names*

```diff
@@ -14,7 +14,22 @@
 "Preferred-Encodings: utf-8 latin1\n"
 "Domain: plone\n"
 "Language: en_US\n"
 "X-Generator: Lokalize 1.5\n"
 
 msgid "Can Manage Bookings"
 msgstr "Può gestire le prenotazioni"
+
+msgid "pending"
+msgstr "In attesa"
+
+msgid "private"
+msgstr "Privato"
+
+msgid "confirmed"
+msgstr "Confermato"
+
+msgid "refused"
+msgstr "Rifiutato"
+
+msgid "canceled"
+msgstr "Annullato"
```

### Comparing `redturtle.prenotazioni-2.6.5/src/redturtle/prenotazioni/locales/it/LC_MESSAGES/redturtle.prenotazioni.po` & `redturtle.prenotazioni-2.7.0/src/redturtle/prenotazioni/locales/it/LC_MESSAGES/redturtle.prenotazioni.po`

 * *Files 3% similar despite different names*

```diff
@@ -1,11 +1,11 @@
 msgid ""
 msgstr ""
 "Project-Id-Version: \n"
-"POT-Creation-Date: 2024-03-29 10:56+0000\n"
+"POT-Creation-Date: 2024-05-21 14:53+0000\n"
 "PO-Revision-Date: 2014-05-27 17:36+0200\n"
 "Last-Translator: Alessandro Pisa <alessandro.pisa@redturtle.it>\n"
 "Language-Team: American English <kde-i18n-doc@kde.org>\n"
 "MIME-Version: 1.0\n"
 "Content-Type: text/plain; charset=UTF-8\n"
 "Content-Transfer-Encoding: 8bit\n"
 "Plural-Forms: nplurals=1; plural=0\n"
@@ -27,15 +27,15 @@
 msgstr "Una cartella che conterrà le prenotazioni"
 
 #: redturtle/prenotazioni/profiles/default/types/PrenotazioniDay.xml
 msgid "A folder that will contain booking for this day"
 msgstr "Una cartella che conterrà le prenotazioni per questo day"
 
 msgid "Add"
-msgstr ""
+msgstr "Aggiungi"
 
 #: redturtle/prenotazioni/content/prenotazioni_folder.py:433
 #: redturtle/prenotazioni/content/validators.py:222
 msgid "Afternoon start should not be greater than end."
 msgstr "L'orario di inizio del pomeriggio non può essere successivo alla chiusura."
 
 #: redturtle/prenotazioni/browser/templates/prenotazione.pt:29
@@ -78,24 +78,32 @@
 msgid "Booking for"
 msgstr "Prenotazione di"
 
 #: redturtle/prenotazioni/behaviors/booking_folder/notifications/appio/configure.zcml:27
 msgid "Booking type notification appio"
 msgstr "Notifiche AppIO per tipologia prenotazione"
 
+#: redturtle/prenotazioni/profiles/default/workflows/prenotazioni_workflow/definition.xml
+msgid "Canceled"
+msgstr "Cancellato"
+
 #. Default: "Change date/time"
 #: redturtle/prenotazioni/profiles/default/actions.xml
 msgid "Change date/time"
 msgstr "Cambia la data di prenotazione."
 
 #. Default: "Complete address"
 #: redturtle/prenotazioni/behaviors/booking_folder/contacts.py:43
 msgid "Complete address"
 msgstr "Indirizzo completo"
 
+#: redturtle/prenotazioni/profiles/default/workflows/prenotazioni_workflow/definition.xml
+msgid "Confirmed"
+msgstr "Confermato"
+
 #: redturtle/prenotazioni/behaviors/booking_folder/contacts.py:36
 msgid "Contact PEC"
 msgstr "Indirizzo PEC per il contatto"
 
 #: redturtle/prenotazioni/behaviors/booking_folder/contacts.py:30
 msgid "Contact fax"
 msgstr "Numero di FAX per il contatto"
@@ -112,45 +120,49 @@
 msgid "Contatti cartella prenotazioni"
 msgstr "Contatti cartella prenotazioni"
 
 #: redturtle/prenotazioni/browser/templates/prenotazioni_search.pt:46
 msgid "Content listing"
 msgstr "Elenco dei contenuti"
 
+#: redturtle/prenotazioni/behaviors/booking_folder/notifications/__init__.py:34
+msgid "Could not send {gateway_type} message due to internal errors"
+msgstr "Non è stato possibile inviare la notifica via {gateway_type}"
+
 #: redturtle/prenotazioni/content/prenotazioni_folder.py:207
 msgid "Data fine validità"
 msgstr "Data fine validità"
 
 #: redturtle/prenotazioni/content/prenotazioni_folder.py:204
 msgid "Data inizio validità"
 msgstr "Data inizio validità"
 
-#: redturtle/prenotazioni/content/prenotazioni_folder.py:498
+#: redturtle/prenotazioni/content/prenotazioni_folder.py:507
 msgid "Date validità"
 msgstr "Date Validità"
 
 #: redturtle/prenotazioni/content/prenotazioni_folder.py:367
 msgid "Days booking is not allowed before"
 msgstr "Giorni da cui si può effettuare una prenotazione"
 
 msgid "Delete"
-msgstr ""
+msgstr "Cancella"
 
 #. Default: "Descrizione Agenda"
 #: redturtle/prenotazioni/content/prenotazioni_folder.py:163
 msgid "Descrizione Agenda"
 msgstr "Descrizione Agenda"
 
 #: redturtle/prenotazioni/profiles/default/types/Prenotazione.xml
 #: redturtle/prenotazioni/profiles/default/types/PrenotazioneType.xml
 #: redturtle/prenotazioni/profiles/default/types/PrenotazioniDay.xml
 msgid "Edit"
 msgstr "Modifica"
 
-#: redturtle/prenotazioni/behaviors/booking_folder/notifications/email/__init__.py:131
+#: redturtle/prenotazioni/behaviors/booking_folder/notifications/email/__init__.py:151
 msgid "Email from"
 msgstr "Mittente"
 
 #: redturtle/prenotazioni/content/prenotazione.py:175
 msgid "Expiration date booking"
 msgstr "Data scandenza prenotazione"
 
@@ -165,15 +177,15 @@
 
 #: redturtle/prenotazioni/browser/templates/prenotazione.pt:107
 #: redturtle/prenotazioni/content/prenotazione.py:170
 msgid "Gate"
 msgstr "Postazione"
 
 msgid "Group"
-msgstr ""
+msgstr "Gruppo"
 
 #. Default: "How to get here"
 #: redturtle/prenotazioni/behaviors/booking_folder/contacts.py:19
 msgid "How to get here"
 msgstr "Indicazioni su come raggiungere l'ufficio"
 
 #: redturtle/prenotazioni/content/validators.py:93
@@ -188,15 +200,15 @@
 msgid "Inserire il testo di presentazione dell'agenda corrente"
 msgstr "Inserire il testo di presentazione dell'agenda corrente"
 
 #: redturtle/prenotazioni/content/prenotazioni_folder.py:405
 msgid "Insert a list of email addresses that will be notified when new bookings get created."
 msgstr "Inserisci una lista di indirizzi email che verranno notificati alla creazione di una nuova prenotazione."
 
-#: redturtle/prenotazioni/behaviors/booking_folder/notifications/email/__init__.py:132
+#: redturtle/prenotazioni/behaviors/booking_folder/notifications/email/__init__.py:152
 msgid "Insert an email address used as \"from\" in email notifications. Leave empty to use the default from set in the site configuration."
 msgstr "Inserisci un indirizzo email da usare come mittente per queste notifiche. Se vuoto, verrà utilizzato l'indirizzo mitente impostato nel sito."
 
 #: redturtle/prenotazioni/behaviors/booking_folder/contacts.py:20
 msgid "Insert here indications on how to reach the office"
 msgstr "Scrivere le indicazioni complete per raggiungere l'ufficio"
 
@@ -226,15 +238,15 @@
 
 #: redturtle/prenotazioni/configure.zcml:31
 msgid "Installs the redturtle.prenotazioni add-on."
 msgstr "Install redturtle.prenotazioni"
 
 #: redturtle/prenotazioni/demo/configure.zcml:16
 msgid "Installs the redturtle.prenotazioni.demo add-on (demo site purpose only)."
-msgstr ""
+msgstr "Installa il profilo redturtle.prenotazioni.demo."
 
 #: redturtle/prenotazioni/content/prenotazioni_folder.py:355
 msgid "Max days in the future"
 msgstr "Massimi giorni nel futuro"
 
 #: redturtle/prenotazioni/content/prenotazioni_folder.py:108
 msgid "Monday"
@@ -246,18 +258,18 @@
 msgstr "L'orario di inizio della mattina non può essere successivo alla fine."
 
 #: redturtle/prenotazioni/browser/templates/prenotazione.pt:152
 msgid "Move booking"
 msgstr "Sposta la prenotazione"
 
 msgid "Move down"
-msgstr ""
+msgstr "Sposta in giù"
 
 msgid "Move up"
-msgstr ""
+msgstr "Sposta in su"
 
 #: redturtle/prenotazioni/restapi/services/booking/vacation.py:27
 msgid "Nessuno slot creato, verificare la corretteza dei dati inseriti"
 msgstr "Nessuno slot creato, verificare la corretteza dei dati inseriti"
 
 #: redturtle/prenotazioni/content/prenotazioni_folder.py:219
 msgid "No"
@@ -291,14 +303,18 @@
 msgid "Pause should be included in morning slot or afternoon slot"
 msgstr "Le pause devono essere comprese tra l'orario di inizio o di termine dell'intervallo di orari di lavoro"
 
 #: redturtle/prenotazioni/content/prenotazioni_folder.py:316
 msgid "Pause table"
 msgstr "Schedulazione delle pause"
 
+#: redturtle/prenotazioni/profiles/default/workflows/prenotazioni_workflow/definition.xml
+msgid "Pending"
+msgstr "In attes"
+
 #: redturtle/prenotazioni/browser/prenotazione_add.py:220
 msgid "Please provide a booking date"
 msgstr "Per favore seleziona una data."
 
 #: redturtle/prenotazioni/profiles/default/types/Prenotazione.xml
 msgid "Prenotazione"
 msgstr "Prenotazione"
@@ -315,15 +331,23 @@
 msgid "PrenotazioniYear"
 msgstr "PrenotazioniYear"
 
 #: redturtle/prenotazioni/browser/templates/prenotazione_print.pt:129
 msgid "Print"
 msgstr "Stampa"
 
-#: redturtle/prenotazioni/restapi/services/booking/add.py:122
+#: redturtle/prenotazioni/profiles/default/workflows/prenotazioni_workflow/definition.xml
+msgid "Private"
+msgstr "Privato"
+
+#: redturtle/prenotazioni/profiles/default/workflows/prenotazioni_workflow/definition.xml
+msgid "Refused"
+msgstr "Rifiutato"
+
+#: redturtle/prenotazioni/restapi/services/booking/add.py:120
 msgid "Required input '${field}' is missing."
 msgstr "Campo obbligatorio '${field}' mancante."
 
 #: redturtle/prenotazioni/browser/prenotazione_add.py:216
 msgid "Required input is missing."
 msgstr "Manca l'input obbligatorio."
 
@@ -340,15 +364,15 @@
 msgstr "Parametri di ricerca"
 
 #: redturtle/prenotazioni/content/prenotazioni_folder.py:107
 msgid "Select a day"
 msgstr "Seleziona un giorno"
 
 #: redturtle/prenotazioni/adapters/booker.py:299
-#: redturtle/prenotazioni/restapi/services/booking/add.py:64
+#: redturtle/prenotazioni/restapi/services/booking/add.py:63
 msgid "Sorry, this slot is not available anymore."
 msgstr "Ci dispiace, ma questo intervallo di tempo non è più disponibile"
 
 #: redturtle/prenotazioni/adapters/booker.py:342
 msgid "Sorry, this slot is not available or does not fit your booking."
 msgstr "Ci dispiace questo intervallo di tempo non è disponibile o non è adatto alla tua prenotazione."
 
@@ -466,17 +490,17 @@
 
 #: redturtle/prenotazioni/configure.zcml:40
 msgid "Uninstalls the redturtle.prenotazioni add-on."
 msgstr "Disinstall redturtle.prenotazioni"
 
 #: redturtle/prenotazioni/demo/configure.zcml:25
 msgid "Uninstalls the redturtle.prenotazioni.demo add-on (demo site purpose only)."
-msgstr ""
+msgstr "Disinstalla redturtle.prenotazioni.demo."
 
-#: redturtle/prenotazioni/restapi/services/booking/add.py:158
+#: redturtle/prenotazioni/restapi/services/booking/add.py:156
 msgid "Unknown booking type '${booking_type}'."
 msgstr "Tipologia di prenotazione sconosciuta '${booking_type}'."
 
 #: redturtle/prenotazioni/content/prenotazioni_folder.py:151
 msgid "Usage of `max_bookings_allowed` field requires the `fiscalcode` to be between the required fields."
 msgstr "L'uso del campo 'Numero massimo di prenotazioni' richiede il `Codice fiscale` tra i campi richiesti della prenotazione."
 
@@ -494,15 +518,15 @@
 msgid "Week table"
 msgstr "Schedulazione Settimanale"
 
 #: redturtle/prenotazioni/content/prenotazioni_folder.py:218
 msgid "Yes"
 msgstr "Si"
 
-#: redturtle/prenotazioni/restapi/services/booking/add.py:115
+#: redturtle/prenotazioni/restapi/services/booking/add.py:113
 msgid "You are not allowed to force the gate."
 msgstr "Non hai i permessi necessari a forzare lo sportello."
 
 #: redturtle/prenotazioni/content/validators.py:70
 msgid "You must set both start and end"
 msgstr "Devi impostare sia un orario di inizio che di termine della pausa"
 
@@ -590,15 +614,15 @@
 
 #. Default: "All bookings created by Managers will be automatically accepted."
 #: redturtle/prenotazioni/content/prenotazioni_folder.py:395
 msgid "auto_confirm_manager_help"
 msgstr "Tutte le prenotazioni create dai Gestori verranno accettate automaticamente."
 
 #. Default: "End date should be greater than start."
-#: redturtle/prenotazioni/restapi/services/available_slots/get.py:61
+#: redturtle/prenotazioni/restapi/services/available_slots/get.py:63
 msgid "available_slots_wrong_dates"
 msgstr "La data di fine prenotazione deve essere maggiore della data di inizio."
 
 #. Default: "Please select a booking slot."
 #: redturtle/prenotazioni/browser/templates/week.pt:40
 msgid "book_it"
 msgstr "Per favore seleziona uno slot per la prenotazione"
@@ -610,15 +634,15 @@
 
 #. Default: "${day}, ore ${booking_time}, prenotato da ${booked_by}, prenotazione: ${booking_type} durata: ${duration} minuti"
 #: redturtle/prenotazioni/browser/week.py:276
 msgid "booked_prenotation_message"
 msgstr "${day}, ore ${booking_time}, prenotato da ${booked_by}, prenotazione: ${booking_type} durata: ${duration} minuti"
 
 #. Default: "Booking canceled: "
-#: redturtle/prenotazioni/behaviors/booking_folder/notifications/email/notification_email_message.py:326
+#: redturtle/prenotazioni/behaviors/booking_folder/notifications/email/notification_email_message.py:368
 msgid "booking_canceled_mail_subject_part"
 msgstr "Prenotazione cancellata: "
 
 #. Default: "Booking confirmed"
 #: redturtle/prenotazioni/browser/templates/prenotazione_macros.pt:456
 msgid "booking_confirmed"
 msgstr "Prenotazione confermata"
@@ -631,15 +655,15 @@
 
 #. Default: "Your booking has been deleted."
 #: redturtle/prenotazioni/browser/delete_reservation.py:115
 msgid "booking_deleted_success"
 msgstr "La tua prenotazione è stata cancellata."
 
 #. Default: "Booking fields"
-#: redturtle/prenotazioni/content/prenotazioni_folder.py:527
+#: redturtle/prenotazioni/content/prenotazioni_folder.py:536
 msgid "booking_fields_label"
 msgstr "Campi Prenotazioni"
 
 #: redturtle/prenotazioni/browser/prenotazione_move.py:135
 msgid "booking_moved"
 msgstr "Prenotazione spostata correttamente"
 
@@ -685,50 +709,50 @@
 
 #. Default: "The following tipologies will not fit the time you selected:"
 #: redturtle/prenotazioni/browser/templates/booking_type_radio_widget.pt:65
 msgid "booking_type_widget_warn_unavailable"
 msgstr "Le seguenti tipologie non sono selezionabili nell'orario selezionato:"
 
 #. Default: "Set message text for all available notification events."
-#: redturtle/prenotazioni/behaviors/booking_folder/notifications/appio/__init__.py:257
+#: redturtle/prenotazioni/behaviors/booking_folder/notifications/appio/__init__.py:301
 msgid "bookings_appio_templates_help"
 msgstr "Imposta i testi dei messaggi per i vari tipi di notifiche disponibili."
 
 #. Default: "AppIO Notifications"
-#: redturtle/prenotazioni/behaviors/booking_folder/notifications/appio/__init__.py:253
+#: redturtle/prenotazioni/behaviors/booking_folder/notifications/appio/__init__.py:297
 msgid "bookings_appio_templates_label"
 msgstr "Notifiche AppIO"
 
 #. Default: "Set message text for all available notification events."
-#: redturtle/prenotazioni/behaviors/booking_folder/notifications/email/__init__.py:266
+#: redturtle/prenotazioni/behaviors/booking_folder/notifications/email/__init__.py:310
 msgid "bookings_email_templates_help"
 msgstr "Imposta i testi dei messaggi per i vari tipi di notifiche disponibili."
 
 #. Default: "Email Notifications"
-#: redturtle/prenotazioni/behaviors/booking_folder/notifications/email/__init__.py:262
+#: redturtle/prenotazioni/behaviors/booking_folder/notifications/email/__init__.py:306
 msgid "bookings_email_templates_label"
 msgstr "Notifiche E-mail"
 
 #. Default: "Booking limit({limit}) for the {booking_type} type is exceed for the current user"
 #: redturtle/prenotazioni/exceptions/booker.py:15
 msgid "bookings_limit_exceeded_exception"
 msgstr "Attenzione: hai superato il massimo di {limit} prenotazioni per la tipologia {booking_type}. Potrai richiedere nuove prenotazioni ad appuntamento avvenuto"
 
 #. Default: "Bookings not in agenda"
 #: redturtle/prenotazioni/browser/templates/prenotazione_macros.pt:111
 msgid "bookings_not_in_agenda"
 msgstr "Prenotazioni non in agenda"
 
 #. Default: "Set message text for all available notification events. Remember that SMS has a 160 characters limit. Depending on your gateway service, it can split messages, if you exceed that limit."
-#: redturtle/prenotazioni/behaviors/booking_folder/notifications/sms/__init__.py:144
+#: redturtle/prenotazioni/behaviors/booking_folder/notifications/sms/__init__.py:166
 msgid "bookings_sms_templates_help"
 msgstr "Imposta i testi dei messaggi per i vari tipi di notifiche disponibili. Gli sms hanno un limite di 160 caratteri. A seconda del gateway per l'invio utilizzato, i messaggi più lunghi potrebbero venire spezzati in più parti."
 
 #. Default: "SMS Notifications"
-#: redturtle/prenotazioni/behaviors/booking_folder/notifications/sms/__init__.py:140
+#: redturtle/prenotazioni/behaviors/booking_folder/notifications/sms/__init__.py:162
 msgid "bookings_sms_templates_label"
 msgstr "Notifiche SMS"
 
 #. Default: "Busy"
 #: redturtle/prenotazioni/browser/prenotazioni_context_state.py:45
 msgid "busy"
 msgstr "Occupato"
@@ -876,14 +900,69 @@
 msgstr "Lista dei tipi di prenotazione disponibili per l'agenda corrente"
 
 #. Default: "User will not be able to add a booking unless those fields are filled. Remember that, whatever you selected in this list, users have to supply at least one of \"Email\" or \"Telephone\""
 #: redturtle/prenotazioni/content/prenotazioni_folder.py:172
 msgid "help_visible_booking_fields"
 msgstr "Gli utenti vedranno solo i campi selezionati all'atto della creazione della prenotazione."
 
+#. Default: "AppIO reminder was sent"
+#: redturtle/prenotazioni/behaviors/booking_folder/notifications/appio/notfication_appio_message.py:107
+msgid "history_appio_reminder_sent"
+msgstr "Inviata notifica AppIO per il promemoria"
+
+#. Default: "AppIO message about the booking reschedule was sent"
+#: redturtle/prenotazioni/behaviors/booking_folder/notifications/appio/notfication_appio_message.py:35
+msgid "history_appio_reschedule_sent"
+msgstr "Inviata notifica AppIO per lo spostamento della prenotazione"
+
+#. Default: "AppIO message about the ${transition} transition was sent."
+#: redturtle/prenotazioni/behaviors/booking_folder/notifications/appio/notfication_appio_message.py:73
+msgid "history_appio_transition_sent"
+msgstr "Inviata notifica AppIO per il cambio di stato della prenotazione: ${transition}"
+
+#. Default: "Email notification was sent to booking manager"
+#: redturtle/prenotazioni/behaviors/booking_folder/notifications/email/notification_email_message.py:258
+msgid "history_email_manager_notification_sent"
+msgstr "Inviata notifica email al Gestore delle prenotazioni"
+
+#. Default: "Email message about the booking reschedule was sent"
+#: redturtle/prenotazioni/behaviors/booking_folder/notifications/email/notification_email_message.py:129
+msgid "history_email_reschedule_sent"
+msgstr "Inviata notifica email per lo spostamento della prenotazione"
+
+#. Default: "Email message about the ${transition} transition was sent"
+#: redturtle/prenotazioni/behaviors/booking_folder/notifications/email/notification_email_message.py:165
+msgid "history_email_transition_sent"
+msgstr "Inviata notifica email per il cambio di stato della prenotazione: ${transition}"
+
+#. Default: "Email reminder was sent"
+#: redturtle/prenotazioni/behaviors/booking_folder/notifications/email/notification_email_message.py:213
+msgid "history_reminder_sent"
+msgstr "Inviata notifica email per il promemoria"
+
+#. Default: "SMS reminder was sent"
+#: redturtle/prenotazioni/behaviors/booking_folder/notifications/sms/message.py:100
+msgid "history_sms_reminder_sent"
+msgstr "Inviata notifica SMS per il promemoria"
+
+#. Default: "SMS removed notification was sent"
+#: redturtle/prenotazioni/behaviors/booking_folder/notifications/sms/message.py:120
+msgid "history_sms_removed_sent"
+msgstr ""
+
+#. Default: "SMS message about the booking reschedule was sent"
+#: redturtle/prenotazioni/behaviors/booking_folder/notifications/sms/message.py:49
+msgid "history_sms_reschedule_sent"
+msgstr "Inviata notifica SMS per lo spostamento della prenotazione"
+
+#. Default: "SMS message about the ${transition} transition was sent"
+#: redturtle/prenotazioni/behaviors/booking_folder/notifications/sms/message.py:76
+msgid "history_sms_transition_sent"
+msgstr "Inviata notifica SMS per il cambio di stato della prenotazione: ${transition}"
+
 #. Default: "Set holidays (one for line) in DD/MM/YYYY. you can write * for the year, if this event is yearly."
 #: redturtle/prenotazioni/content/prenotazioni_folder.py:330
 msgid "holidays_help"
 msgstr "Imposta eventuali festività (una per riga) nel formato GG/MM/AAAA. Se la data si ripete ogni anno, puoi scrivere * al posto dell'anno."
 
 #. Default: "Holidays"
 #: redturtle/prenotazioni/content/prenotazioni_folder.py:329
@@ -1105,20 +1184,20 @@
 
 #. Default: "The minimum value of a single slot is 5 minutes. You cannot book a reservation when the needed time exceeds the available time."
 #: redturtle/prenotazioni/browser/templates/prenotazione_macros.pt:469
 msgid "legend_note"
 msgstr "L'unità di tempo minima è 5 minuti. La tua prenotazione non può eccedere il tempo disponibile."
 
 #. Default: "The number of simultaneous bookings allowed for the same user."
-#: redturtle/prenotazioni/content/prenotazioni_folder.py:476
+#: redturtle/prenotazioni/content/prenotazioni_folder.py:485
 msgid "max_bookings_allowed_description"
 msgstr "Numero massimo delle prenotazioni contemporanee per una stessa tipologia, per lo stesso utente. Impostare '0' o lasciare vuoto per non porre limitazioni. Per attivare questo controllo è necessario richiedere obbligatoriamente all'utente il campo 'codice fiscale'"
 
 #. Default: "Maximum bookings number allowed"
-#: redturtle/prenotazioni/content/prenotazioni_folder.py:472
+#: redturtle/prenotazioni/content/prenotazioni_folder.py:481
 msgid "max_bookings_allowed_label"
 msgstr "Numero massimo delle prenotazioni"
 
 #. Default: "Unable to find a booking with the givend id: ${uid}."
 #: redturtle/prenotazioni/browser/delete_reservation.py:45
 msgid "missing_booking"
 msgstr "Impossibile trovare la prenotazione con id: ${uid}."
@@ -1165,106 +1244,166 @@
 
 #. Default: "Booking is not allowed before the amount of days specified. \nKeep 0 to give no limits."
 #: redturtle/prenotazioni/content/prenotazioni_folder.py:368
 msgid "notBeforeDays"
 msgstr "La prenotazione non e' permessa prima del numero di giorni specificata. Impostare il valore 0 per non imporre limitazioni."
 
 #. Default: "Enable AppIO notifications."
-#: redturtle/prenotazioni/behaviors/booking_folder/notifications/appio/__init__.py:123
+#: redturtle/prenotazioni/behaviors/booking_folder/notifications/appio/__init__.py:143
 msgid "notifications_appio_enabled_help"
 msgstr "Abilita le notifiche via App IO. I campi del messaggio accettano il formato Markdown"
 
 #. Default: "AppIO notifications"
-#: redturtle/prenotazioni/behaviors/booking_folder/notifications/appio/__init__.py:122
+#: redturtle/prenotazioni/behaviors/booking_folder/notifications/appio/__init__.py:142
 msgid "notifications_appio_enabled_label"
 msgstr "Notifiche AppIO"
 
 #. Default: "Enable Email notifications."
-#: redturtle/prenotazioni/behaviors/booking_folder/notifications/email/__init__.py:123
+#: redturtle/prenotazioni/behaviors/booking_folder/notifications/email/__init__.py:143
 msgid "notifications_email_enabled_help"
 msgstr "Abilita le notifiche via email"
 
 #. Default: "Email notifications"
-#: redturtle/prenotazioni/behaviors/booking_folder/notifications/email/__init__.py:122
+#: redturtle/prenotazioni/behaviors/booking_folder/notifications/email/__init__.py:142
 msgid "notifications_email_enabled_label"
 msgstr "Notifiche Email"
 
 #. Default: "Notifications"
-#: redturtle/prenotazioni/content/prenotazioni_folder.py:535
+#: redturtle/prenotazioni/content/prenotazioni_folder.py:544
 msgid "notifications_label"
 msgstr "Gestione delle Notifiche"
 
 #. Default: "Enable SMS notifications."
-#: redturtle/prenotazioni/behaviors/booking_folder/notifications/sms/__init__.py:70
+#: redturtle/prenotazioni/behaviors/booking_folder/notifications/sms/__init__.py:80
 msgid "notifications_sms_enabled_help"
 msgstr "Abilita le notifiche via SMS. Per poter ricevere un SMS, il campo 'Numero di telefono' della Prenotazione deve essere compilato."
 
 #. Default: "SMS notifications"
-#: redturtle/prenotazioni/behaviors/booking_folder/notifications/sms/__init__.py:69
+#: redturtle/prenotazioni/behaviors/booking_folder/notifications/sms/__init__.py:79
 msgid "notifications_sms_enabled_label"
 msgstr "Notifiche SMS"
 
 #. Default: "This is an automatic reminder about your booking on ${date} for ${booking_type}.<br/><br/>You can see details and print a reminder following this [link](${booking_print_url})."
-#: redturtle/prenotazioni/behaviors/booking_folder/notifications/appio/__init__.py:111
+#: redturtle/prenotazioni/behaviors/booking_folder/notifications/appio/__init__.py:131
 msgid "notify_as_reminder_appio_message_default_value"
 msgstr "Promemoria automatico per la prenotazione per ${booking_type} il ${booking_date} alle ${booking_time}. <br/><br/>Dal tuo [promemoria](${booking_print_url}) puoi controllare i dati, stampare ed eventualmente cancellare la prenotazione."
 
 #. Default: "[${prenotazioni_folder_title}] Booking reminder on ${booking_date}"
-#: redturtle/prenotazioni/behaviors/booking_folder/notifications/appio/__init__.py:101
+#: redturtle/prenotazioni/behaviors/booking_folder/notifications/appio/__init__.py:121
 msgid "notify_as_reminder_appio_subject_default_value"
 msgstr "[${prenotazioni_folder_title}] Promemoria prenotazione del ${booking_date}"
 
 #. Default: "The message subject when a reminder will be sent."
-#: redturtle/prenotazioni/behaviors/booking_folder/notifications/appio/__init__.py:231
+#: redturtle/prenotazioni/behaviors/booking_folder/notifications/appio/__init__.py:275
 msgid "notify_as_reminder_appio_subject_help"
 msgstr "L'oggetto del messaggio inviato come promemoria."
 
 #. Default: "[Reminder] message"
-#: redturtle/prenotazioni/behaviors/booking_folder/notifications/appio/__init__.py:239
-#: redturtle/prenotazioni/behaviors/booking_folder/notifications/email/__init__.py:248
-#: redturtle/prenotazioni/behaviors/booking_folder/notifications/sms/__init__.py:126
+#: redturtle/prenotazioni/behaviors/booking_folder/notifications/appio/__init__.py:283
+#: redturtle/prenotazioni/behaviors/booking_folder/notifications/email/__init__.py:292
+#: redturtle/prenotazioni/behaviors/booking_folder/notifications/sms/__init__.py:148
 msgid "notify_as_reminder_message"
 msgstr "[Promemoria] messaggio"
 
 #. Default: "This is an automatic reminder about your booking on ${date} for ${booking_type}.<br/><br/>You can see details and print a reminder following this <a href=${booking_print_url}>link</a>."
-#: redturtle/prenotazioni/behaviors/booking_folder/notifications/email/__init__.py:111
+#: redturtle/prenotazioni/behaviors/booking_folder/notifications/email/__init__.py:131
 msgid "notify_as_reminder_message_default_value"
 msgstr "Promemoria automatico per la prenotazione per ${booking_type} il ${booking_date} alle ${booking_time}. <br/><br/>Dal tuo <a href=${booking_print_url}>promemoria</a> puoi controllare i dati, stampare ed eventualmente cancellare la prenotazione."
 
 #. Default: "The message text when a reminder will be sent."
-#: redturtle/prenotazioni/behaviors/booking_folder/notifications/appio/__init__.py:243
-#: redturtle/prenotazioni/behaviors/booking_folder/notifications/email/__init__.py:252
-#: redturtle/prenotazioni/behaviors/booking_folder/notifications/sms/__init__.py:130
+#: redturtle/prenotazioni/behaviors/booking_folder/notifications/appio/__init__.py:287
+#: redturtle/prenotazioni/behaviors/booking_folder/notifications/email/__init__.py:296
+#: redturtle/prenotazioni/behaviors/booking_folder/notifications/sms/__init__.py:152
 msgid "notify_as_reminder_message_help"
 msgstr "Il testo del messaggio inviato come promemoria."
 
 #. Default: "[${prenotazioni_folder_title}]: This is an automatic reminder about your booking on ${date} for ${booking_type} .\nSee details or delete it: ${booking_print_url} ."
-#: redturtle/prenotazioni/behaviors/booking_folder/notifications/sms/__init__.py:58
-#, fuzzy
+#: redturtle/prenotazioni/behaviors/booking_folder/notifications/sms/__init__.py:68
 msgid "notify_as_reminder_sms_message_default_value"
 msgstr ""
 "[${prenotazioni_folder_title}]: Promemoria prenotazione per ${booking_type} il ${booking_date} alle ${booking_time}.\n"
 "Per dettagli: ${booking_print_url} ."
 
 #. Default: "[Reminder] subject"
-#: redturtle/prenotazioni/behaviors/booking_folder/notifications/appio/__init__.py:227
-#: redturtle/prenotazioni/behaviors/booking_folder/notifications/email/__init__.py:236
+#: redturtle/prenotazioni/behaviors/booking_folder/notifications/appio/__init__.py:271
+#: redturtle/prenotazioni/behaviors/booking_folder/notifications/email/__init__.py:280
 msgid "notify_as_reminder_subject"
 msgstr "[Promemoria] oggetto"
 
 #. Default: "[${prenotazioni_folder_title}] Booking reminder on ${booking_date}"
-#: redturtle/prenotazioni/behaviors/booking_folder/notifications/email/__init__.py:101
+#: redturtle/prenotazioni/behaviors/booking_folder/notifications/email/__init__.py:121
 msgid "notify_as_reminder_subject_default_value"
 msgstr "[${prenotazioni_folder_title}] Promemoria prenotazione del ${booking_date}"
 
 #. Default: "The message subject when a reminder will be sent."
-#: redturtle/prenotazioni/behaviors/booking_folder/notifications/email/__init__.py:240
+#: redturtle/prenotazioni/behaviors/booking_folder/notifications/email/__init__.py:284
 msgid "notify_as_reminder_subject_help"
 msgstr "L'oggetto del messaggio inviato come promemoria."
 
+#. Default: "Notify when canceled."
+#: redturtle/prenotazioni/content/prenotazioni_folder.py:472
+msgid "notify_on_cancel"
+msgstr "Notifica alla cancellazione"
+
+#. Default: "The booking ${booking_type} of ${booking_date} at ${booking_time} was canceled."
+#: redturtle/prenotazioni/behaviors/booking_folder/notifications/appio/__init__.py:111
+msgid "notify_on_cancel_appio_message_default_value"
+msgstr "La prenotazione ${booking_type} del ${booking_date} delle ore ${booking_time} è stata cancellata."
+
+#. Default: "[${prenotazioni_folder_title}] Booking canceled for ${title}"
+#: redturtle/prenotazioni/behaviors/booking_folder/notifications/appio/__init__.py:101
+msgid "notify_on_cancel_appio_subject_default_value"
+msgstr "[${prenotazioni_folder_title}] Prenotazione cancellata per ${title}"
+
+#. Default: "Notify via mail the user when his booking has been canceled."
+#: redturtle/prenotazioni/content/prenotazioni_folder.py:473
+msgid "notify_on_cancel_help"
+msgstr "Notifica l'utente via mail se la prenotazione viene cancellata"
+
+#. Default: "[Cancel] message"
+#: redturtle/prenotazioni/behaviors/booking_folder/notifications/appio/__init__.py:259
+#: redturtle/prenotazioni/behaviors/booking_folder/notifications/email/__init__.py:268
+#: redturtle/prenotazioni/behaviors/booking_folder/notifications/sms/__init__.py:136
+msgid "notify_on_cancel_message"
+msgstr "Testo notifica prenotazione cancellata"
+
+#. Default: "The booking ${booking_type} of ${booking_date} at ${booking_time} was canceled."
+#: redturtle/prenotazioni/behaviors/booking_folder/notifications/email/__init__.py:111
+msgid "notify_on_cancel_message_default_value"
+msgstr "La prenotazione ${booking_type} del ${booking_date} delle ore ${booking_time} è stata cancellata."
+
+#. Default: "The message text when a booking has been canceled."
+#: redturtle/prenotazioni/behaviors/booking_folder/notifications/appio/__init__.py:263
+#: redturtle/prenotazioni/behaviors/booking_folder/notifications/email/__init__.py:272
+#: redturtle/prenotazioni/behaviors/booking_folder/notifications/sms/__init__.py:140
+msgid "notify_on_cancel_message_help"
+msgstr "Il testo del messaggio quando una prenotazione è stata cancellata."
+
+#. Default: "[${prenotazioni_folder_title}]: The booking ${booking_type} of ${booking_date} at ${booking_time} was canceled."
+#: redturtle/prenotazioni/behaviors/booking_folder/notifications/sms/__init__.py:58
+msgid "notify_on_cancel_sms_message_default_value"
+msgstr "[${prenotazioni_folder_title}]: La prenotazione ${booking_type} del ${booking_date} alle ${booking_time} è stata cancellata."
+
+#. Default: "[Cancel] subject"
+#: redturtle/prenotazioni/behaviors/booking_folder/notifications/appio/__init__.py:247
+#: redturtle/prenotazioni/behaviors/booking_folder/notifications/email/__init__.py:256
+msgid "notify_on_cancel_subject"
+msgstr "[Cancella] oggetto"
+
+#. Default: "[${prenotazioni_folder_title}] Booking canceled for ${title}"
+#: redturtle/prenotazioni/behaviors/booking_folder/notifications/email/__init__.py:101
+msgid "notify_on_cancel_subject_default_value"
+msgstr "[${prenotazioni_folder_title}] Prenotazione cancellata per ${title}"
+
+#. Default: "The message subject when a booking has been canceled."
+#: redturtle/prenotazioni/behaviors/booking_folder/notifications/appio/__init__.py:251
+#: redturtle/prenotazioni/behaviors/booking_folder/notifications/email/__init__.py:260
+msgid "notify_on_cancel_subject_help"
+msgstr "L'oggetto del messaggio quando una prenotazione è stata cancellata."
+
 #. Default: "Notify when confirmed."
 #: redturtle/prenotazioni/content/prenotazioni_folder.py:445
 msgid "notify_on_confirm"
 msgstr "Notifica alla conferma"
 
 #. Default: "The booking ${booking_type} for ${title} has been confirmed.<br/><br/>You can see details and print a reminder following this [link](${booking_print_url})."
 #: redturtle/prenotazioni/behaviors/booking_folder/notifications/appio/__init__.py:48
@@ -1280,54 +1419,53 @@
 
 #. Default: "Notify via mail the user when his booking has been confirmed."
 #: redturtle/prenotazioni/content/prenotazioni_folder.py:446
 msgid "notify_on_confirm_help"
 msgstr "Notifica l'utente quando la prenotazione viene confermata."
 
 #. Default: "[Confirmed] message"
-#: redturtle/prenotazioni/behaviors/booking_folder/notifications/appio/__init__.py:167
-#: redturtle/prenotazioni/behaviors/booking_folder/notifications/email/__init__.py:176
-#: redturtle/prenotazioni/behaviors/booking_folder/notifications/sms/__init__.py:90
+#: redturtle/prenotazioni/behaviors/booking_folder/notifications/appio/__init__.py:187
+#: redturtle/prenotazioni/behaviors/booking_folder/notifications/email/__init__.py:196
+#: redturtle/prenotazioni/behaviors/booking_folder/notifications/sms/__init__.py:100
 msgid "notify_on_confirm_message"
 msgstr "[Conferma] messaggio"
 
 #. Default: "The booking ${booking_type} for ${title} has been confirmed.<br/><br/>You can see details and print a reminder following this <a href=${booking_print_url}>link</a>."
 #: redturtle/prenotazioni/behaviors/booking_folder/notifications/email/__init__.py:48
 msgid "notify_on_confirm_message_default_value"
 msgstr "La prenotazione ${booking_type} per ${title} è stata confermata.<br/><br/>Dal tuo <a href=${booking_print_url}>promemoria</a> puoi controllare i dati, stampare ed eventualmente cancellare la prenotazione."
 
 #. Default: "The message text when a booking has been confirmed."
-#: redturtle/prenotazioni/behaviors/booking_folder/notifications/appio/__init__.py:171
-#: redturtle/prenotazioni/behaviors/booking_folder/notifications/email/__init__.py:180
-#: redturtle/prenotazioni/behaviors/booking_folder/notifications/sms/__init__.py:94
+#: redturtle/prenotazioni/behaviors/booking_folder/notifications/appio/__init__.py:191
+#: redturtle/prenotazioni/behaviors/booking_folder/notifications/email/__init__.py:200
+#: redturtle/prenotazioni/behaviors/booking_folder/notifications/sms/__init__.py:104
 msgid "notify_on_confirm_message_help"
 msgstr "Il testo del messaggio quando una prenotazione è stata confermata."
 
 #. Default: "[${prenotazioni_folder_title}]: Booking of ${booking_date} at ${booking_time} has been accepted.\nSee details or delete it: ${booking_print_url} ."
 #: redturtle/prenotazioni/behaviors/booking_folder/notifications/sms/__init__.py:28
-#, fuzzy
 msgid "notify_on_confirm_sms_message_default_value"
 msgstr ""
 "[${prenotazioni_folder_title}]: La prenotazione ${booking_type} per ${title} è stata confermata.\n"
 "Per dettagli: ${booking_print_url} ."
 
 #. Default: "[Confirm] subject"
-#: redturtle/prenotazioni/behaviors/booking_folder/notifications/appio/__init__.py:155
-#: redturtle/prenotazioni/behaviors/booking_folder/notifications/email/__init__.py:164
+#: redturtle/prenotazioni/behaviors/booking_folder/notifications/appio/__init__.py:175
+#: redturtle/prenotazioni/behaviors/booking_folder/notifications/email/__init__.py:184
 msgid "notify_on_confirm_subject"
 msgstr "[Conferma] oggetto"
 
 #. Default: "[${prenotazioni_folder_title}] Booking of ${booking_date} at ${booking_time} was accepted"
 #: redturtle/prenotazioni/behaviors/booking_folder/notifications/email/__init__.py:38
 msgid "notify_on_confirm_subject_default_value"
 msgstr "[${prenotazioni_folder_title}] Prenotazione del ${booking_date} alle ${booking_time} accettata"
 
 #. Default: "The message subject when a booking has been confirmed."
-#: redturtle/prenotazioni/behaviors/booking_folder/notifications/appio/__init__.py:159
-#: redturtle/prenotazioni/behaviors/booking_folder/notifications/email/__init__.py:168
+#: redturtle/prenotazioni/behaviors/booking_folder/notifications/appio/__init__.py:179
+#: redturtle/prenotazioni/behaviors/booking_folder/notifications/email/__init__.py:188
 msgid "notify_on_confirm_subject_help"
 msgstr "L'oggetto del messaggio quando una prenotazione è stata confermata."
 
 #. Default: "Notify when moved."
 #: redturtle/prenotazioni/content/prenotazioni_folder.py:454
 msgid "notify_on_move"
 msgstr "Notifica allo spostamento"
@@ -1347,54 +1485,53 @@
 
 #. Default: "Notify via mail the user when his booking has been moved."
 #: redturtle/prenotazioni/content/prenotazioni_folder.py:455
 msgid "notify_on_move_help"
 msgstr "Notifica l'utente quando la prenotazione viene spostata di giorno/orario."
 
 #. Default: "[Move] message"
-#: redturtle/prenotazioni/behaviors/booking_folder/notifications/appio/__init__.py:191
-#: redturtle/prenotazioni/behaviors/booking_folder/notifications/email/__init__.py:200
-#: redturtle/prenotazioni/behaviors/booking_folder/notifications/sms/__init__.py:102
+#: redturtle/prenotazioni/behaviors/booking_folder/notifications/appio/__init__.py:211
+#: redturtle/prenotazioni/behaviors/booking_folder/notifications/email/__init__.py:220
+#: redturtle/prenotazioni/behaviors/booking_folder/notifications/sms/__init__.py:112
 msgid "notify_on_move_message"
 msgstr "[Spostamento] messaggio"
 
 #. Default: "The booking scheduling for ${booking_type} was modified.<br/><br/>The new one is on ${booking_date} at ${booking_time}.<br/><br/>You can see details and print a reminder following this <a href=${booking_print_url}>link</a>."
 #: redturtle/prenotazioni/behaviors/booking_folder/notifications/email/__init__.py:69
 msgid "notify_on_move_message_default_value"
 msgstr "L'orario della sua prenotazione ${booking_type} è stato modificato.<br/><br/>La nuova data è ${booking_date} alle ore ${booking_time}.<br/><br/>Dal tuo <a href=${booking_print_url}>promemoria</a> puoi controllare i dati, stampare ed eventualmente cancellare la prenotazione."
 
 #. Default: "The message text when a booking has been moved."
-#: redturtle/prenotazioni/behaviors/booking_folder/notifications/appio/__init__.py:195
-#: redturtle/prenotazioni/behaviors/booking_folder/notifications/email/__init__.py:204
-#: redturtle/prenotazioni/behaviors/booking_folder/notifications/sms/__init__.py:106
+#: redturtle/prenotazioni/behaviors/booking_folder/notifications/appio/__init__.py:215
+#: redturtle/prenotazioni/behaviors/booking_folder/notifications/email/__init__.py:224
+#: redturtle/prenotazioni/behaviors/booking_folder/notifications/sms/__init__.py:116
 msgid "notify_on_move_message_help"
 msgstr "Il testo del messaggio quando una prenotazione è stata spostata."
 
 #. Default: "[${prenotazioni_folder_title}]: The booking scheduling for ${booking_type} was modified.\nThe new one is on ${booking_date} at ${booking_time} .\nSee details or delete it: ${booking_print_url} ."
 #: redturtle/prenotazioni/behaviors/booking_folder/notifications/sms/__init__.py:38
-#, fuzzy
 msgid "notify_on_move_sms_message_default_value"
 msgstr ""
 "[${prenotazioni_folder_title}]: orario della prenotazione ${booking_type} modificato: ${booking_date} alle ${booking_time}.\n"
 "Per dettagli: ${booking_print_url} ."
 
 #. Default: "[Move] subject"
-#: redturtle/prenotazioni/behaviors/booking_folder/notifications/appio/__init__.py:179
-#: redturtle/prenotazioni/behaviors/booking_folder/notifications/email/__init__.py:188
+#: redturtle/prenotazioni/behaviors/booking_folder/notifications/appio/__init__.py:199
+#: redturtle/prenotazioni/behaviors/booking_folder/notifications/email/__init__.py:208
 msgid "notify_on_move_subject"
 msgstr "[Spostamento] oggetto"
 
 #. Default: "[${prenotazioni_folder_title}] Booking date modified for ${title}"
 #: redturtle/prenotazioni/behaviors/booking_folder/notifications/email/__init__.py:59
 msgid "notify_on_move_subject_default_value"
 msgstr "[${prenotazioni_folder_title}] Data di prenotazione modificata per ${title} - ${booking_date}"
 
 #. Default: "The message subject when a booking has been moved."
-#: redturtle/prenotazioni/behaviors/booking_folder/notifications/appio/__init__.py:183
-#: redturtle/prenotazioni/behaviors/booking_folder/notifications/email/__init__.py:192
+#: redturtle/prenotazioni/behaviors/booking_folder/notifications/appio/__init__.py:203
+#: redturtle/prenotazioni/behaviors/booking_folder/notifications/email/__init__.py:212
 msgid "notify_on_move_subject_help"
 msgstr "L'oggetto del messaggio quando una prenotazione è stata spostata."
 
 #. Default: "Notify when rejected."
 #: redturtle/prenotazioni/content/prenotazioni_folder.py:463
 msgid "notify_on_refuse"
 msgstr "Notifica al rifiuto"
@@ -1411,53 +1548,53 @@
 
 #. Default: "Notify via mail the user when his booking has been rejected."
 #: redturtle/prenotazioni/content/prenotazioni_folder.py:464
 msgid "notify_on_refuse_help"
 msgstr "Notifica l'utente via mail se la prenotazione viene rifiutata"
 
 #. Default: "[Refuse] message"
-#: redturtle/prenotazioni/behaviors/booking_folder/notifications/appio/__init__.py:215
-#: redturtle/prenotazioni/behaviors/booking_folder/notifications/email/__init__.py:224
-#: redturtle/prenotazioni/behaviors/booking_folder/notifications/sms/__init__.py:114
+#: redturtle/prenotazioni/behaviors/booking_folder/notifications/appio/__init__.py:235
+#: redturtle/prenotazioni/behaviors/booking_folder/notifications/email/__init__.py:244
+#: redturtle/prenotazioni/behaviors/booking_folder/notifications/sms/__init__.py:124
 msgid "notify_on_refuse_message"
 msgstr "Testo notifica prenotazione rifiutata"
 
 #. Default: "The booking ${booking_type} of ${booking_date} at ${booking_time} was refused."
 #: redturtle/prenotazioni/behaviors/booking_folder/notifications/email/__init__.py:91
 msgid "notify_on_refuse_message_default_value"
 msgstr "La prenotazione ${booking_type} del ${booking_date} delle ore ${booking_time} è stata rifiutata. Motivo del rifiuto: ${booking_refuse_message}"
 
 #. Default: "The message text when a booking has been refused."
-#: redturtle/prenotazioni/behaviors/booking_folder/notifications/appio/__init__.py:219
-#: redturtle/prenotazioni/behaviors/booking_folder/notifications/email/__init__.py:228
-#: redturtle/prenotazioni/behaviors/booking_folder/notifications/sms/__init__.py:118
+#: redturtle/prenotazioni/behaviors/booking_folder/notifications/appio/__init__.py:239
+#: redturtle/prenotazioni/behaviors/booking_folder/notifications/email/__init__.py:248
+#: redturtle/prenotazioni/behaviors/booking_folder/notifications/sms/__init__.py:128
 msgid "notify_on_refuse_message_help"
 msgstr "Il testo del messaggio quando una prenotazione è stata rifiutata."
 
 #. Default: "[${prenotazioni_folder_title}]: The booking ${booking_type} of ${booking_date} at ${booking_time} was refused."
 #: redturtle/prenotazioni/behaviors/booking_folder/notifications/sms/__init__.py:48
 msgid "notify_on_refuse_sms_message_default_value"
 msgstr ""
 "[${prenotazioni_folder_title}]: La prenotazione ${booking_type} del ${booking_date} alle ${booking_time} è stata rifiutata.\n"
 "Motivo: ${booking_refuse_message}"
 
 #. Default: "[Refuse] subject"
-#: redturtle/prenotazioni/behaviors/booking_folder/notifications/appio/__init__.py:203
-#: redturtle/prenotazioni/behaviors/booking_folder/notifications/email/__init__.py:212
+#: redturtle/prenotazioni/behaviors/booking_folder/notifications/appio/__init__.py:223
+#: redturtle/prenotazioni/behaviors/booking_folder/notifications/email/__init__.py:232
 msgid "notify_on_refuse_subject"
 msgstr "[Rifiuto] oggetto"
 
 #. Default: "[${prenotazioni_folder_title}] Booking refused for ${title}"
 #: redturtle/prenotazioni/behaviors/booking_folder/notifications/email/__init__.py:81
 msgid "notify_on_refuse_subject_default_value"
 msgstr "[${prenotazioni_folder_title}] Prenotazione rifiutata per ${title}"
 
 #. Default: "The message subject when a booking has been refused."
-#: redturtle/prenotazioni/behaviors/booking_folder/notifications/appio/__init__.py:207
-#: redturtle/prenotazioni/behaviors/booking_folder/notifications/email/__init__.py:216
+#: redturtle/prenotazioni/behaviors/booking_folder/notifications/appio/__init__.py:227
+#: redturtle/prenotazioni/behaviors/booking_folder/notifications/email/__init__.py:236
 msgid "notify_on_refuse_subject_help"
 msgstr "L'oggetto del messaggio quando una prenotazione è stata rifiutata."
 
 #. Default: "Notify when created."
 #: redturtle/prenotazioni/content/prenotazioni_folder.py:436
 msgid "notify_on_submit"
 msgstr "Notifica alla creazione"
@@ -1476,52 +1613,51 @@
 
 #. Default: "Notify via mail the user when his booking has been created. If auto-confirm flag is selected and confirm notify is selected, this one will be ignored."
 #: redturtle/prenotazioni/content/prenotazioni_folder.py:437
 msgid "notify_on_submit_help"
 msgstr "Notifica l'utente quando la prenotazione viene creata. Se il flag di conferma automatica e di notifica alla conferma sono selezionati, questa opzione verrà ignorata."
 
 #. Default: "[Created] message"
-#: redturtle/prenotazioni/behaviors/booking_folder/notifications/appio/__init__.py:143
-#: redturtle/prenotazioni/behaviors/booking_folder/notifications/email/__init__.py:152
-#: redturtle/prenotazioni/behaviors/booking_folder/notifications/sms/__init__.py:78
+#: redturtle/prenotazioni/behaviors/booking_folder/notifications/appio/__init__.py:163
+#: redturtle/prenotazioni/behaviors/booking_folder/notifications/email/__init__.py:172
+#: redturtle/prenotazioni/behaviors/booking_folder/notifications/sms/__init__.py:88
 msgid "notify_on_submit_message"
 msgstr "[Creazione] messaggio"
 
 #. Default: "Booking ${booking_type} for ${booking_date} at ${booking_time} has been created.<br/><br/>You can see details and print a reminder following this <a href=${booking_print_url}>link</a>."
 #: redturtle/prenotazioni/behaviors/booking_folder/notifications/email/__init__.py:28
 msgid "notify_on_submit_message_default_value"
 msgstr "La prenotazione ${booking_type} per il ${booking_date} alle ${booking_time} è stata creata.<br/><br/>Dal tuo <a href=${booking_print_url}>promemoria</a> puoi controllare i dati, stampare ed eventualmente cancellare la prenotazione."
 
 #. Default: "The message text when a booking has been created."
-#: redturtle/prenotazioni/behaviors/booking_folder/notifications/appio/__init__.py:147
-#: redturtle/prenotazioni/behaviors/booking_folder/notifications/email/__init__.py:156
-#: redturtle/prenotazioni/behaviors/booking_folder/notifications/sms/__init__.py:82
+#: redturtle/prenotazioni/behaviors/booking_folder/notifications/appio/__init__.py:167
+#: redturtle/prenotazioni/behaviors/booking_folder/notifications/email/__init__.py:176
+#: redturtle/prenotazioni/behaviors/booking_folder/notifications/sms/__init__.py:92
 msgid "notify_on_submit_message_help"
 msgstr "Il testo del messaggio quando una prenotazione è stata creata."
 
 #. Default: "[${prenotazioni_folder_title}]: Booking ${booking_type} for ${booking_date} at ${booking_time} has been created.\nSee details or delete it: ${booking_print_url} ."
 #: redturtle/prenotazioni/behaviors/booking_folder/notifications/sms/__init__.py:18
-#, fuzzy
 msgid "notify_on_submit_sms_message_default_value"
 msgstr "[${prenotazioni_folder_title}]: La prenotazione ${booking_type} per il ${booking_date} alle ${booking_time} è stata creata. Per dettagli: ${booking_print_url} ."
 
 #. Default: "[Created] subject"
-#: redturtle/prenotazioni/behaviors/booking_folder/notifications/appio/__init__.py:131
-#: redturtle/prenotazioni/behaviors/booking_folder/notifications/email/__init__.py:140
+#: redturtle/prenotazioni/behaviors/booking_folder/notifications/appio/__init__.py:151
+#: redturtle/prenotazioni/behaviors/booking_folder/notifications/email/__init__.py:160
 msgid "notify_on_submit_subject"
 msgstr "[Creazione] oggetto"
 
 #. Default: "[${prenotazioni_folder_title}] Booking created"
 #: redturtle/prenotazioni/behaviors/booking_folder/notifications/email/__init__.py:18
 msgid "notify_on_submit_subject_default_value"
 msgstr "[${prenotazioni_folder_title}] Prenotazione creata"
 
 #. Default: "The message subject when a booking has been created."
-#: redturtle/prenotazioni/behaviors/booking_folder/notifications/appio/__init__.py:135
-#: redturtle/prenotazioni/behaviors/booking_folder/notifications/email/__init__.py:144
+#: redturtle/prenotazioni/behaviors/booking_folder/notifications/appio/__init__.py:155
+#: redturtle/prenotazioni/behaviors/booking_folder/notifications/email/__init__.py:164
 msgid "notify_on_submit_subject_help"
 msgstr "L'oggetto del messaggio quando una prenotazione è stata creata."
 
 #. Default: "Pause end"
 #: redturtle/prenotazioni/content/prenotazioni_folder.py:124
 msgid "pause_end_label"
 msgstr "Termine pausa"
@@ -1587,20 +1723,20 @@
 
 #. Default: "Reject booking"
 #: redturtle/prenotazioni/browser/templates/prenotazione.pt:176
 msgid "reject_booking"
 msgstr "Rifiuta la prenotazione"
 
 #. Default: "Set how many days before of a booking date the user will be notified about it."
-#: redturtle/prenotazioni/content/prenotazioni_folder.py:488
+#: redturtle/prenotazioni/content/prenotazioni_folder.py:497
 msgid "reminder_notification_gap_description"
 msgstr "Indicare quanti giorni prima della data di prenotazione, inviare un promemoria agli utenti."
 
 #. Default: "Booking reminder days"
-#: redturtle/prenotazioni/content/prenotazioni_folder.py:484
+#: redturtle/prenotazioni/content/prenotazioni_folder.py:493
 msgid "reminder_notification_gap_label"
 msgstr "Promemoria prenotazione"
 
 #. Default: "Code"
 #: redturtle/prenotazioni/browser/templates/prenotazioni_search.pt:58
 msgid "reservation_code"
 msgstr "Codice prenotazione"
@@ -1642,20 +1778,20 @@
 
 #. Default: "seleziona l'opzione desiderata dal gruppo di radio button seguente"
 #: redturtle/prenotazioni/browser/z3c_custom_widget.py:153
 msgid "select-option"
 msgstr "seleziona l'opzione desiderata dal gruppo di campi seguente"
 
 #. Default: "AppIO service code related to the current booking type"
-#: redturtle/prenotazioni/behaviors/booking_folder/notifications/appio/__init__.py:293
+#: redturtle/prenotazioni/behaviors/booking_folder/notifications/appio/__init__.py:339
 msgid "service_code_help"
 msgstr "Matricola del servizio legato alla tipologia (serve per l'invio coretto delle notifiche)"
 
 #. Default: "AppIO service code."
-#: redturtle/prenotazioni/behaviors/booking_folder/notifications/appio/__init__.py:289
+#: redturtle/prenotazioni/behaviors/booking_folder/notifications/appio/__init__.py:335
 msgid "service_code_label"
 msgstr "Matricola servizio App IO"
 
 #. Default: "This gate has some booking schedule in this time period."
 #: redturtle/prenotazioni/browser/vacations.py:216
 msgid "slot_conflict_error"
 msgstr "Questa postazione ha già appuntamenti schedulati in questo periodo."
@@ -1675,15 +1811,15 @@
 
 #. Default: "Selected day is too big for that month for \"to\" field."
 #: redturtle/prenotazioni/content/validators.py:191
 msgid "to_month_too_days_error"
 msgstr "Il giorno selezionato non è compatibile col mese selezionato nel campo \"Al\"."
 
 #. Default: "You can't add a booking with type '${booking_type}'."
-#: redturtle/prenotazioni/restapi/services/booking/add.py:134
+#: redturtle/prenotazioni/restapi/services/booking/add.py:132
 msgid "unauthorized_add_vacation"
 msgstr "Impossibile creare una nuova prenotazione per la tipologia '${booking_type}'."
 
 #. Default: "Unbookable time"
 #: redturtle/prenotazioni/browser/templates/prenotazione_macros.pt:452
 msgid "unbookable_time"
 msgstr "Tempo non prenotabile "
@@ -1714,7 +1850,22 @@
 msgid "week_table_overrides_label"
 msgstr "Personalizzazioni Schedulazione Settimanale"
 
 #. Default: "You tried to delete booking with a wrong action."
 #: redturtle/prenotazioni/browser/delete_reservation.py:98
 msgid "wrong_authenticator"
 msgstr "Stai cercando di cancellare una prenotazione con un'azione sbagliata."
+
+msgid "pending"
+msgstr "In attesa"
+
+msgid "private"
+msgstr "Privato"
+
+msgid "confirmed"
+msgstr "Confermato"
+
+msgid "refused"
+msgstr "Rifiutato"
+
+msgid "canceled"
+msgstr "Annullato"
```

### Comparing `redturtle.prenotazioni-2.6.5/src/redturtle/prenotazioni/locales/manual.pot` & `redturtle.prenotazioni-2.7.0/src/redturtle/prenotazioni/locales/manual.pot`

 * *Files 14% similar despite different names*

```diff
@@ -36,7 +36,22 @@
 msgstr ""
 
 msgid "Delete"
 msgstr ""
 
 msgid "Add"
 msgstr ""
+
+msgid "pending"
+msgstr "In attesa"
+
+msgid "private"
+msgstr "Privato"
+
+msgid "confirmed"
+msgstr "Confermato"
+
+msgid "refused"
+msgstr "Rifiutato"
+
+msgid "canceled"
+msgstr "Annullato"
```

### Comparing `redturtle.prenotazioni-2.6.5/src/redturtle/prenotazioni/locales/redturtle.prenotazioni.pot` & `redturtle.prenotazioni-2.7.0/src/redturtle/prenotazioni/locales/redturtle.prenotazioni.pot`

 * *Files 5% similar despite different names*

```diff
@@ -1,14 +1,14 @@
 # --- PLEASE EDIT THE LINES BELOW CORRECTLY ---
 # SOME DESCRIPTIVE TITLE.
 # FIRST AUTHOR <EMAIL@ADDRESS>, YEAR.
 msgid ""
 msgstr ""
 "Project-Id-Version: PACKAGE VERSION\n"
-"POT-Creation-Date: 2024-03-29 10:56+0000\n"
+"POT-Creation-Date: 2024-05-21 14:53+0000\n"
 "PO-Revision-Date: YEAR-MO-DA HO:MI +ZONE\n"
 "Last-Translator: FULL NAME <EMAIL@ADDRESS>\n"
 "Language-Team: LANGUAGE <LL@li.org>\n"
 "MIME-Version: 1.0\n"
 "Content-Type: text/plain; charset=utf-8\n"
 "Content-Transfer-Encoding: 8bit\n"
 "Plural-Forms: nplurals=1; plural=0\n"
@@ -79,24 +79,32 @@
 msgid "Booking for"
 msgstr ""
 
 #: redturtle/prenotazioni/behaviors/booking_folder/notifications/appio/configure.zcml:27
 msgid "Booking type notification appio"
 msgstr ""
 
+#: redturtle/prenotazioni/profiles/default/workflows/prenotazioni_workflow/definition.xml
+msgid "Canceled"
+msgstr ""
+
 #. Default: "Change date/time"
 #: redturtle/prenotazioni/profiles/default/actions.xml
 msgid "Change date/time"
 msgstr ""
 
 #. Default: "Complete address"
 #: redturtle/prenotazioni/behaviors/booking_folder/contacts.py:43
 msgid "Complete address"
 msgstr ""
 
+#: redturtle/prenotazioni/profiles/default/workflows/prenotazioni_workflow/definition.xml
+msgid "Confirmed"
+msgstr ""
+
 #: redturtle/prenotazioni/behaviors/booking_folder/contacts.py:36
 msgid "Contact PEC"
 msgstr ""
 
 #: redturtle/prenotazioni/behaviors/booking_folder/contacts.py:30
 msgid "Contact fax"
 msgstr ""
@@ -113,23 +121,27 @@
 msgid "Contatti cartella prenotazioni"
 msgstr ""
 
 #: redturtle/prenotazioni/browser/templates/prenotazioni_search.pt:46
 msgid "Content listing"
 msgstr ""
 
+#: redturtle/prenotazioni/behaviors/booking_folder/notifications/__init__.py:34
+msgid "Could not send {gateway_type} message due to internal errors"
+msgstr ""
+
 #: redturtle/prenotazioni/content/prenotazioni_folder.py:207
 msgid "Data fine validità"
 msgstr ""
 
 #: redturtle/prenotazioni/content/prenotazioni_folder.py:204
 msgid "Data inizio validità"
 msgstr ""
 
-#: redturtle/prenotazioni/content/prenotazioni_folder.py:498
+#: redturtle/prenotazioni/content/prenotazioni_folder.py:507
 msgid "Date validità"
 msgstr ""
 
 #: redturtle/prenotazioni/content/prenotazioni_folder.py:367
 msgid "Days booking is not allowed before"
 msgstr ""
 
@@ -143,15 +155,15 @@
 
 #: redturtle/prenotazioni/profiles/default/types/Prenotazione.xml
 #: redturtle/prenotazioni/profiles/default/types/PrenotazioneType.xml
 #: redturtle/prenotazioni/profiles/default/types/PrenotazioniDay.xml
 msgid "Edit"
 msgstr ""
 
-#: redturtle/prenotazioni/behaviors/booking_folder/notifications/email/__init__.py:131
+#: redturtle/prenotazioni/behaviors/booking_folder/notifications/email/__init__.py:151
 msgid "Email from"
 msgstr ""
 
 #: redturtle/prenotazioni/content/prenotazione.py:175
 msgid "Expiration date booking"
 msgstr ""
 
@@ -189,15 +201,15 @@
 msgid "Inserire il testo di presentazione dell'agenda corrente"
 msgstr ""
 
 #: redturtle/prenotazioni/content/prenotazioni_folder.py:405
 msgid "Insert a list of email addresses that will be notified when new bookings get created."
 msgstr ""
 
-#: redturtle/prenotazioni/behaviors/booking_folder/notifications/email/__init__.py:132
+#: redturtle/prenotazioni/behaviors/booking_folder/notifications/email/__init__.py:152
 msgid "Insert an email address used as \"from\" in email notifications. Leave empty to use the default from set in the site configuration."
 msgstr ""
 
 #: redturtle/prenotazioni/behaviors/booking_folder/contacts.py:20
 msgid "Insert here indications on how to reach the office"
 msgstr ""
 
@@ -292,14 +304,18 @@
 msgid "Pause should be included in morning slot or afternoon slot"
 msgstr ""
 
 #: redturtle/prenotazioni/content/prenotazioni_folder.py:316
 msgid "Pause table"
 msgstr ""
 
+#: redturtle/prenotazioni/profiles/default/workflows/prenotazioni_workflow/definition.xml
+msgid "Pending"
+msgstr ""
+
 #: redturtle/prenotazioni/browser/prenotazione_add.py:220
 msgid "Please provide a booking date"
 msgstr ""
 
 #: redturtle/prenotazioni/profiles/default/types/Prenotazione.xml
 msgid "Prenotazione"
 msgstr ""
@@ -316,15 +332,23 @@
 msgid "PrenotazioniYear"
 msgstr ""
 
 #: redturtle/prenotazioni/browser/templates/prenotazione_print.pt:129
 msgid "Print"
 msgstr ""
 
-#: redturtle/prenotazioni/restapi/services/booking/add.py:122
+#: redturtle/prenotazioni/profiles/default/workflows/prenotazioni_workflow/definition.xml
+msgid "Private"
+msgstr ""
+
+#: redturtle/prenotazioni/profiles/default/workflows/prenotazioni_workflow/definition.xml
+msgid "Refused"
+msgstr ""
+
+#: redturtle/prenotazioni/restapi/services/booking/add.py:120
 msgid "Required input '${field}' is missing."
 msgstr ""
 
 #: redturtle/prenotazioni/browser/prenotazione_add.py:216
 msgid "Required input is missing."
 msgstr ""
 
@@ -341,15 +365,15 @@
 msgstr ""
 
 #: redturtle/prenotazioni/content/prenotazioni_folder.py:107
 msgid "Select a day"
 msgstr ""
 
 #: redturtle/prenotazioni/adapters/booker.py:299
-#: redturtle/prenotazioni/restapi/services/booking/add.py:64
+#: redturtle/prenotazioni/restapi/services/booking/add.py:63
 msgid "Sorry, this slot is not available anymore."
 msgstr ""
 
 #: redturtle/prenotazioni/adapters/booker.py:342
 msgid "Sorry, this slot is not available or does not fit your booking."
 msgstr ""
 
@@ -469,15 +493,15 @@
 msgid "Uninstalls the redturtle.prenotazioni add-on."
 msgstr ""
 
 #: redturtle/prenotazioni/demo/configure.zcml:25
 msgid "Uninstalls the redturtle.prenotazioni.demo add-on (demo site purpose only)."
 msgstr ""
 
-#: redturtle/prenotazioni/restapi/services/booking/add.py:158
+#: redturtle/prenotazioni/restapi/services/booking/add.py:156
 msgid "Unknown booking type '${booking_type}'."
 msgstr ""
 
 #: redturtle/prenotazioni/content/prenotazioni_folder.py:151
 msgid "Usage of `max_bookings_allowed` field requires the `fiscalcode` to be between the required fields."
 msgstr ""
 
@@ -495,15 +519,15 @@
 msgid "Week table"
 msgstr ""
 
 #: redturtle/prenotazioni/content/prenotazioni_folder.py:218
 msgid "Yes"
 msgstr ""
 
-#: redturtle/prenotazioni/restapi/services/booking/add.py:115
+#: redturtle/prenotazioni/restapi/services/booking/add.py:113
 msgid "You are not allowed to force the gate."
 msgstr ""
 
 #: redturtle/prenotazioni/content/validators.py:70
 msgid "You must set both start and end"
 msgstr ""
 
@@ -591,15 +615,15 @@
 
 #. Default: "All bookings created by Managers will be automatically accepted."
 #: redturtle/prenotazioni/content/prenotazioni_folder.py:395
 msgid "auto_confirm_manager_help"
 msgstr ""
 
 #. Default: "End date should be greater than start."
-#: redturtle/prenotazioni/restapi/services/available_slots/get.py:61
+#: redturtle/prenotazioni/restapi/services/available_slots/get.py:63
 msgid "available_slots_wrong_dates"
 msgstr ""
 
 #. Default: "Please select a booking slot."
 #: redturtle/prenotazioni/browser/templates/week.pt:40
 msgid "book_it"
 msgstr ""
@@ -611,15 +635,15 @@
 
 #. Default: "${day}, ore ${booking_time}, prenotato da ${booked_by}, prenotazione: ${booking_type} durata: ${duration} minuti"
 #: redturtle/prenotazioni/browser/week.py:276
 msgid "booked_prenotation_message"
 msgstr ""
 
 #. Default: "Booking canceled: "
-#: redturtle/prenotazioni/behaviors/booking_folder/notifications/email/notification_email_message.py:326
+#: redturtle/prenotazioni/behaviors/booking_folder/notifications/email/notification_email_message.py:368
 msgid "booking_canceled_mail_subject_part"
 msgstr ""
 
 #. Default: "Booking confirmed"
 #: redturtle/prenotazioni/browser/templates/prenotazione_macros.pt:456
 msgid "booking_confirmed"
 msgstr ""
@@ -631,15 +655,15 @@
 
 #. Default: "Your booking has been deleted."
 #: redturtle/prenotazioni/browser/delete_reservation.py:115
 msgid "booking_deleted_success"
 msgstr ""
 
 #. Default: "Booking fields"
-#: redturtle/prenotazioni/content/prenotazioni_folder.py:527
+#: redturtle/prenotazioni/content/prenotazioni_folder.py:536
 msgid "booking_fields_label"
 msgstr ""
 
 #: redturtle/prenotazioni/browser/prenotazione_move.py:135
 msgid "booking_moved"
 msgstr ""
 
@@ -685,50 +709,50 @@
 
 #. Default: "The following tipologies will not fit the time you selected:"
 #: redturtle/prenotazioni/browser/templates/booking_type_radio_widget.pt:65
 msgid "booking_type_widget_warn_unavailable"
 msgstr ""
 
 #. Default: "Set message text for all available notification events."
-#: redturtle/prenotazioni/behaviors/booking_folder/notifications/appio/__init__.py:257
+#: redturtle/prenotazioni/behaviors/booking_folder/notifications/appio/__init__.py:301
 msgid "bookings_appio_templates_help"
 msgstr ""
 
 #. Default: "AppIO Notifications"
-#: redturtle/prenotazioni/behaviors/booking_folder/notifications/appio/__init__.py:253
+#: redturtle/prenotazioni/behaviors/booking_folder/notifications/appio/__init__.py:297
 msgid "bookings_appio_templates_label"
 msgstr ""
 
 #. Default: "Set message text for all available notification events."
-#: redturtle/prenotazioni/behaviors/booking_folder/notifications/email/__init__.py:266
+#: redturtle/prenotazioni/behaviors/booking_folder/notifications/email/__init__.py:310
 msgid "bookings_email_templates_help"
 msgstr ""
 
 #. Default: "Email Notifications"
-#: redturtle/prenotazioni/behaviors/booking_folder/notifications/email/__init__.py:262
+#: redturtle/prenotazioni/behaviors/booking_folder/notifications/email/__init__.py:306
 msgid "bookings_email_templates_label"
 msgstr ""
 
 #. Default: "Booking limit({limit}) for the {booking_type} type is exceed for the current user"
 #: redturtle/prenotazioni/exceptions/booker.py:15
 msgid "bookings_limit_exceeded_exception"
 msgstr ""
 
 #. Default: "Bookings not in agenda"
 #: redturtle/prenotazioni/browser/templates/prenotazione_macros.pt:111
 msgid "bookings_not_in_agenda"
 msgstr ""
 
 #. Default: "Set message text for all available notification events. Remember that SMS has a 160 characters limit. Depending on your gateway service, it can split messages, if you exceed that limit."
-#: redturtle/prenotazioni/behaviors/booking_folder/notifications/sms/__init__.py:144
+#: redturtle/prenotazioni/behaviors/booking_folder/notifications/sms/__init__.py:166
 msgid "bookings_sms_templates_help"
 msgstr ""
 
 #. Default: "SMS Notifications"
-#: redturtle/prenotazioni/behaviors/booking_folder/notifications/sms/__init__.py:140
+#: redturtle/prenotazioni/behaviors/booking_folder/notifications/sms/__init__.py:162
 msgid "bookings_sms_templates_label"
 msgstr ""
 
 #. Default: "Busy"
 #: redturtle/prenotazioni/browser/prenotazioni_context_state.py:45
 msgid "busy"
 msgstr ""
@@ -876,14 +900,69 @@
 msgstr ""
 
 #. Default: "User will not be able to add a booking unless those fields are filled. Remember that, whatever you selected in this list, users have to supply at least one of \"Email\" or \"Telephone\""
 #: redturtle/prenotazioni/content/prenotazioni_folder.py:172
 msgid "help_visible_booking_fields"
 msgstr ""
 
+#. Default: "AppIO reminder was sent"
+#: redturtle/prenotazioni/behaviors/booking_folder/notifications/appio/notfication_appio_message.py:107
+msgid "history_appio_reminder_sent"
+msgstr ""
+
+#. Default: "AppIO message about the booking reschedule was sent"
+#: redturtle/prenotazioni/behaviors/booking_folder/notifications/appio/notfication_appio_message.py:35
+msgid "history_appio_reschedule_sent"
+msgstr ""
+
+#. Default: "AppIO message about the ${transition} transition was sent."
+#: redturtle/prenotazioni/behaviors/booking_folder/notifications/appio/notfication_appio_message.py:73
+msgid "history_appio_transition_sent"
+msgstr ""
+
+#. Default: "Email notification was sent to booking manager"
+#: redturtle/prenotazioni/behaviors/booking_folder/notifications/email/notification_email_message.py:258
+msgid "history_email_manager_notification_sent"
+msgstr ""
+
+#. Default: "Email message about the booking reschedule was sent"
+#: redturtle/prenotazioni/behaviors/booking_folder/notifications/email/notification_email_message.py:129
+msgid "history_email_reschedule_sent"
+msgstr ""
+
+#. Default: "Email message about the ${transition} transition was sent"
+#: redturtle/prenotazioni/behaviors/booking_folder/notifications/email/notification_email_message.py:165
+msgid "history_email_transition_sent"
+msgstr ""
+
+#. Default: "Email reminder was sent"
+#: redturtle/prenotazioni/behaviors/booking_folder/notifications/email/notification_email_message.py:213
+msgid "history_reminder_sent"
+msgstr ""
+
+#. Default: "SMS reminder was sent"
+#: redturtle/prenotazioni/behaviors/booking_folder/notifications/sms/message.py:100
+msgid "history_sms_reminder_sent"
+msgstr ""
+
+#. Default: "SMS removed notification was sent"
+#: redturtle/prenotazioni/behaviors/booking_folder/notifications/sms/message.py:120
+msgid "history_sms_removed_sent"
+msgstr ""
+
+#. Default: "SMS message about the booking reschedule was sent"
+#: redturtle/prenotazioni/behaviors/booking_folder/notifications/sms/message.py:49
+msgid "history_sms_reschedule_sent"
+msgstr ""
+
+#. Default: "SMS message about the ${transition} transition was sent"
+#: redturtle/prenotazioni/behaviors/booking_folder/notifications/sms/message.py:76
+msgid "history_sms_transition_sent"
+msgstr ""
+
 #. Default: "Set holidays (one for line) in DD/MM/YYYY. you can write * for the year, if this event is yearly."
 #: redturtle/prenotazioni/content/prenotazioni_folder.py:330
 msgid "holidays_help"
 msgstr ""
 
 #. Default: "Holidays"
 #: redturtle/prenotazioni/content/prenotazioni_folder.py:329
@@ -1103,20 +1182,20 @@
 
 #. Default: "The minimum value of a single slot is 5 minutes. You cannot book a reservation when the needed time exceeds the available time."
 #: redturtle/prenotazioni/browser/templates/prenotazione_macros.pt:469
 msgid "legend_note"
 msgstr ""
 
 #. Default: "The number of simultaneous bookings allowed for the same user."
-#: redturtle/prenotazioni/content/prenotazioni_folder.py:476
+#: redturtle/prenotazioni/content/prenotazioni_folder.py:485
 msgid "max_bookings_allowed_description"
 msgstr ""
 
 #. Default: "Maximum bookings number allowed"
-#: redturtle/prenotazioni/content/prenotazioni_folder.py:472
+#: redturtle/prenotazioni/content/prenotazioni_folder.py:481
 msgid "max_bookings_allowed_label"
 msgstr ""
 
 #. Default: "Unable to find a booking with the givend id: ${uid}."
 #: redturtle/prenotazioni/browser/delete_reservation.py:45
 msgid "missing_booking"
 msgstr ""
@@ -1163,103 +1242,164 @@
 
 #. Default: "Booking is not allowed before the amount of days specified. \nKeep 0 to give no limits."
 #: redturtle/prenotazioni/content/prenotazioni_folder.py:368
 msgid "notBeforeDays"
 msgstr ""
 
 #. Default: "Enable AppIO notifications."
-#: redturtle/prenotazioni/behaviors/booking_folder/notifications/appio/__init__.py:123
+#: redturtle/prenotazioni/behaviors/booking_folder/notifications/appio/__init__.py:143
 msgid "notifications_appio_enabled_help"
 msgstr ""
 
 #. Default: "AppIO notifications"
-#: redturtle/prenotazioni/behaviors/booking_folder/notifications/appio/__init__.py:122
+#: redturtle/prenotazioni/behaviors/booking_folder/notifications/appio/__init__.py:142
 msgid "notifications_appio_enabled_label"
 msgstr ""
 
 #. Default: "Enable Email notifications."
-#: redturtle/prenotazioni/behaviors/booking_folder/notifications/email/__init__.py:123
+#: redturtle/prenotazioni/behaviors/booking_folder/notifications/email/__init__.py:143
 msgid "notifications_email_enabled_help"
 msgstr ""
 
 #. Default: "Email notifications"
-#: redturtle/prenotazioni/behaviors/booking_folder/notifications/email/__init__.py:122
+#: redturtle/prenotazioni/behaviors/booking_folder/notifications/email/__init__.py:142
 msgid "notifications_email_enabled_label"
 msgstr ""
 
 #. Default: "Notifications"
-#: redturtle/prenotazioni/content/prenotazioni_folder.py:535
+#: redturtle/prenotazioni/content/prenotazioni_folder.py:544
 msgid "notifications_label"
 msgstr ""
 
 #. Default: "Enable SMS notifications."
-#: redturtle/prenotazioni/behaviors/booking_folder/notifications/sms/__init__.py:70
+#: redturtle/prenotazioni/behaviors/booking_folder/notifications/sms/__init__.py:80
 msgid "notifications_sms_enabled_help"
 msgstr ""
 
 #. Default: "SMS notifications"
-#: redturtle/prenotazioni/behaviors/booking_folder/notifications/sms/__init__.py:69
+#: redturtle/prenotazioni/behaviors/booking_folder/notifications/sms/__init__.py:79
 msgid "notifications_sms_enabled_label"
 msgstr ""
 
 #. Default: "This is an automatic reminder about your booking on ${date} for ${booking_type}.<br/><br/>You can see details and print a reminder following this [link](${booking_print_url})."
-#: redturtle/prenotazioni/behaviors/booking_folder/notifications/appio/__init__.py:111
+#: redturtle/prenotazioni/behaviors/booking_folder/notifications/appio/__init__.py:131
 msgid "notify_as_reminder_appio_message_default_value"
 msgstr ""
 
 #. Default: "[${prenotazioni_folder_title}] Booking reminder on ${booking_date}"
-#: redturtle/prenotazioni/behaviors/booking_folder/notifications/appio/__init__.py:101
+#: redturtle/prenotazioni/behaviors/booking_folder/notifications/appio/__init__.py:121
 msgid "notify_as_reminder_appio_subject_default_value"
 msgstr ""
 
 #. Default: "The message subject when a reminder will be sent."
-#: redturtle/prenotazioni/behaviors/booking_folder/notifications/appio/__init__.py:231
+#: redturtle/prenotazioni/behaviors/booking_folder/notifications/appio/__init__.py:275
 msgid "notify_as_reminder_appio_subject_help"
 msgstr ""
 
 #. Default: "[Reminder] message"
-#: redturtle/prenotazioni/behaviors/booking_folder/notifications/appio/__init__.py:239
-#: redturtle/prenotazioni/behaviors/booking_folder/notifications/email/__init__.py:248
-#: redturtle/prenotazioni/behaviors/booking_folder/notifications/sms/__init__.py:126
+#: redturtle/prenotazioni/behaviors/booking_folder/notifications/appio/__init__.py:283
+#: redturtle/prenotazioni/behaviors/booking_folder/notifications/email/__init__.py:292
+#: redturtle/prenotazioni/behaviors/booking_folder/notifications/sms/__init__.py:148
 msgid "notify_as_reminder_message"
 msgstr ""
 
 #. Default: "This is an automatic reminder about your booking on ${date} for ${booking_type}.<br/><br/>You can see details and print a reminder following this <a href=${booking_print_url}>link</a>."
-#: redturtle/prenotazioni/behaviors/booking_folder/notifications/email/__init__.py:111
+#: redturtle/prenotazioni/behaviors/booking_folder/notifications/email/__init__.py:131
 msgid "notify_as_reminder_message_default_value"
 msgstr ""
 
 #. Default: "The message text when a reminder will be sent."
-#: redturtle/prenotazioni/behaviors/booking_folder/notifications/appio/__init__.py:243
-#: redturtle/prenotazioni/behaviors/booking_folder/notifications/email/__init__.py:252
-#: redturtle/prenotazioni/behaviors/booking_folder/notifications/sms/__init__.py:130
+#: redturtle/prenotazioni/behaviors/booking_folder/notifications/appio/__init__.py:287
+#: redturtle/prenotazioni/behaviors/booking_folder/notifications/email/__init__.py:296
+#: redturtle/prenotazioni/behaviors/booking_folder/notifications/sms/__init__.py:152
 msgid "notify_as_reminder_message_help"
 msgstr ""
 
 #. Default: "[${prenotazioni_folder_title}]: This is an automatic reminder about your booking on ${date} for ${booking_type} .\nSee details or delete it: ${booking_print_url} ."
-#: redturtle/prenotazioni/behaviors/booking_folder/notifications/sms/__init__.py:58
+#: redturtle/prenotazioni/behaviors/booking_folder/notifications/sms/__init__.py:68
 msgid "notify_as_reminder_sms_message_default_value"
 msgstr ""
 
 #. Default: "[Reminder] subject"
-#: redturtle/prenotazioni/behaviors/booking_folder/notifications/appio/__init__.py:227
-#: redturtle/prenotazioni/behaviors/booking_folder/notifications/email/__init__.py:236
+#: redturtle/prenotazioni/behaviors/booking_folder/notifications/appio/__init__.py:271
+#: redturtle/prenotazioni/behaviors/booking_folder/notifications/email/__init__.py:280
 msgid "notify_as_reminder_subject"
 msgstr ""
 
 #. Default: "[${prenotazioni_folder_title}] Booking reminder on ${booking_date}"
-#: redturtle/prenotazioni/behaviors/booking_folder/notifications/email/__init__.py:101
+#: redturtle/prenotazioni/behaviors/booking_folder/notifications/email/__init__.py:121
 msgid "notify_as_reminder_subject_default_value"
 msgstr ""
 
 #. Default: "The message subject when a reminder will be sent."
-#: redturtle/prenotazioni/behaviors/booking_folder/notifications/email/__init__.py:240
+#: redturtle/prenotazioni/behaviors/booking_folder/notifications/email/__init__.py:284
 msgid "notify_as_reminder_subject_help"
 msgstr ""
 
+#. Default: "Notify when canceled."
+#: redturtle/prenotazioni/content/prenotazioni_folder.py:472
+msgid "notify_on_cancel"
+msgstr ""
+
+#. Default: "The booking ${booking_type} of ${booking_date} at ${booking_time} was canceled."
+#: redturtle/prenotazioni/behaviors/booking_folder/notifications/appio/__init__.py:111
+msgid "notify_on_cancel_appio_message_default_value"
+msgstr ""
+
+#. Default: "[${prenotazioni_folder_title}] Booking canceled for ${title}"
+#: redturtle/prenotazioni/behaviors/booking_folder/notifications/appio/__init__.py:101
+msgid "notify_on_cancel_appio_subject_default_value"
+msgstr ""
+
+#. Default: "Notify via mail the user when his booking has been canceled."
+#: redturtle/prenotazioni/content/prenotazioni_folder.py:473
+msgid "notify_on_cancel_help"
+msgstr ""
+
+#. Default: "[Cancel] message"
+#: redturtle/prenotazioni/behaviors/booking_folder/notifications/appio/__init__.py:259
+#: redturtle/prenotazioni/behaviors/booking_folder/notifications/email/__init__.py:268
+#: redturtle/prenotazioni/behaviors/booking_folder/notifications/sms/__init__.py:136
+msgid "notify_on_cancel_message"
+msgstr ""
+
+#. Default: "The booking ${booking_type} of ${booking_date} at ${booking_time} was canceled."
+#: redturtle/prenotazioni/behaviors/booking_folder/notifications/email/__init__.py:111
+msgid "notify_on_cancel_message_default_value"
+msgstr ""
+
+#. Default: "The message text when a booking has been canceled."
+#: redturtle/prenotazioni/behaviors/booking_folder/notifications/appio/__init__.py:263
+#: redturtle/prenotazioni/behaviors/booking_folder/notifications/email/__init__.py:272
+#: redturtle/prenotazioni/behaviors/booking_folder/notifications/sms/__init__.py:140
+msgid "notify_on_cancel_message_help"
+msgstr ""
+
+#. Default: "[${prenotazioni_folder_title}]: The booking ${booking_type} of ${booking_date} at ${booking_time} was canceled."
+#: redturtle/prenotazioni/behaviors/booking_folder/notifications/sms/__init__.py:58
+msgid "notify_on_cancel_sms_message_default_value"
+msgstr ""
+
+#. Default: "[Cancel] subject"
+#: redturtle/prenotazioni/behaviors/booking_folder/notifications/appio/__init__.py:247
+#: redturtle/prenotazioni/behaviors/booking_folder/notifications/email/__init__.py:256
+msgid "notify_on_cancel_subject"
+msgstr ""
+
+#. Default: "[${prenotazioni_folder_title}] Booking canceled for ${title}"
+#: redturtle/prenotazioni/behaviors/booking_folder/notifications/email/__init__.py:101
+msgid "notify_on_cancel_subject_default_value"
+msgstr ""
+
+#. Default: "The message subject when a booking has been canceled."
+#: redturtle/prenotazioni/behaviors/booking_folder/notifications/appio/__init__.py:251
+#: redturtle/prenotazioni/behaviors/booking_folder/notifications/email/__init__.py:260
+msgid "notify_on_cancel_subject_help"
+msgstr ""
+
 #. Default: "Notify when confirmed."
 #: redturtle/prenotazioni/content/prenotazioni_folder.py:445
 msgid "notify_on_confirm"
 msgstr ""
 
 #. Default: "The booking ${booking_type} for ${title} has been confirmed.<br/><br/>You can see details and print a reminder following this [link](${booking_print_url})."
 #: redturtle/prenotazioni/behaviors/booking_folder/notifications/appio/__init__.py:48
@@ -1273,51 +1413,51 @@
 
 #. Default: "Notify via mail the user when his booking has been confirmed."
 #: redturtle/prenotazioni/content/prenotazioni_folder.py:446
 msgid "notify_on_confirm_help"
 msgstr ""
 
 #. Default: "[Confirmed] message"
-#: redturtle/prenotazioni/behaviors/booking_folder/notifications/appio/__init__.py:167
-#: redturtle/prenotazioni/behaviors/booking_folder/notifications/email/__init__.py:176
-#: redturtle/prenotazioni/behaviors/booking_folder/notifications/sms/__init__.py:90
+#: redturtle/prenotazioni/behaviors/booking_folder/notifications/appio/__init__.py:187
+#: redturtle/prenotazioni/behaviors/booking_folder/notifications/email/__init__.py:196
+#: redturtle/prenotazioni/behaviors/booking_folder/notifications/sms/__init__.py:100
 msgid "notify_on_confirm_message"
 msgstr ""
 
 #. Default: "The booking ${booking_type} for ${title} has been confirmed.<br/><br/>You can see details and print a reminder following this <a href=${booking_print_url}>link</a>."
 #: redturtle/prenotazioni/behaviors/booking_folder/notifications/email/__init__.py:48
 msgid "notify_on_confirm_message_default_value"
 msgstr ""
 
 #. Default: "The message text when a booking has been confirmed."
-#: redturtle/prenotazioni/behaviors/booking_folder/notifications/appio/__init__.py:171
-#: redturtle/prenotazioni/behaviors/booking_folder/notifications/email/__init__.py:180
-#: redturtle/prenotazioni/behaviors/booking_folder/notifications/sms/__init__.py:94
+#: redturtle/prenotazioni/behaviors/booking_folder/notifications/appio/__init__.py:191
+#: redturtle/prenotazioni/behaviors/booking_folder/notifications/email/__init__.py:200
+#: redturtle/prenotazioni/behaviors/booking_folder/notifications/sms/__init__.py:104
 msgid "notify_on_confirm_message_help"
 msgstr ""
 
 #. Default: "[${prenotazioni_folder_title}]: Booking of ${booking_date} at ${booking_time} has been accepted.\nSee details or delete it: ${booking_print_url} ."
 #: redturtle/prenotazioni/behaviors/booking_folder/notifications/sms/__init__.py:28
 msgid "notify_on_confirm_sms_message_default_value"
 msgstr ""
 
 #. Default: "[Confirm] subject"
-#: redturtle/prenotazioni/behaviors/booking_folder/notifications/appio/__init__.py:155
-#: redturtle/prenotazioni/behaviors/booking_folder/notifications/email/__init__.py:164
+#: redturtle/prenotazioni/behaviors/booking_folder/notifications/appio/__init__.py:175
+#: redturtle/prenotazioni/behaviors/booking_folder/notifications/email/__init__.py:184
 msgid "notify_on_confirm_subject"
 msgstr ""
 
 #. Default: "[${prenotazioni_folder_title}] Booking of ${booking_date} at ${booking_time} was accepted"
 #: redturtle/prenotazioni/behaviors/booking_folder/notifications/email/__init__.py:38
 msgid "notify_on_confirm_subject_default_value"
 msgstr ""
 
 #. Default: "The message subject when a booking has been confirmed."
-#: redturtle/prenotazioni/behaviors/booking_folder/notifications/appio/__init__.py:159
-#: redturtle/prenotazioni/behaviors/booking_folder/notifications/email/__init__.py:168
+#: redturtle/prenotazioni/behaviors/booking_folder/notifications/appio/__init__.py:179
+#: redturtle/prenotazioni/behaviors/booking_folder/notifications/email/__init__.py:188
 msgid "notify_on_confirm_subject_help"
 msgstr ""
 
 #. Default: "Notify when moved."
 #: redturtle/prenotazioni/content/prenotazioni_folder.py:454
 msgid "notify_on_move"
 msgstr ""
@@ -1334,51 +1474,51 @@
 
 #. Default: "Notify via mail the user when his booking has been moved."
 #: redturtle/prenotazioni/content/prenotazioni_folder.py:455
 msgid "notify_on_move_help"
 msgstr ""
 
 #. Default: "[Move] message"
-#: redturtle/prenotazioni/behaviors/booking_folder/notifications/appio/__init__.py:191
-#: redturtle/prenotazioni/behaviors/booking_folder/notifications/email/__init__.py:200
-#: redturtle/prenotazioni/behaviors/booking_folder/notifications/sms/__init__.py:102
+#: redturtle/prenotazioni/behaviors/booking_folder/notifications/appio/__init__.py:211
+#: redturtle/prenotazioni/behaviors/booking_folder/notifications/email/__init__.py:220
+#: redturtle/prenotazioni/behaviors/booking_folder/notifications/sms/__init__.py:112
 msgid "notify_on_move_message"
 msgstr ""
 
 #. Default: "The booking scheduling for ${booking_type} was modified.<br/><br/>The new one is on ${booking_date} at ${booking_time}.<br/><br/>You can see details and print a reminder following this <a href=${booking_print_url}>link</a>."
 #: redturtle/prenotazioni/behaviors/booking_folder/notifications/email/__init__.py:69
 msgid "notify_on_move_message_default_value"
 msgstr ""
 
 #. Default: "The message text when a booking has been moved."
-#: redturtle/prenotazioni/behaviors/booking_folder/notifications/appio/__init__.py:195
-#: redturtle/prenotazioni/behaviors/booking_folder/notifications/email/__init__.py:204
-#: redturtle/prenotazioni/behaviors/booking_folder/notifications/sms/__init__.py:106
+#: redturtle/prenotazioni/behaviors/booking_folder/notifications/appio/__init__.py:215
+#: redturtle/prenotazioni/behaviors/booking_folder/notifications/email/__init__.py:224
+#: redturtle/prenotazioni/behaviors/booking_folder/notifications/sms/__init__.py:116
 msgid "notify_on_move_message_help"
 msgstr ""
 
 #. Default: "[${prenotazioni_folder_title}]: The booking scheduling for ${booking_type} was modified.\nThe new one is on ${booking_date} at ${booking_time} .\nSee details or delete it: ${booking_print_url} ."
 #: redturtle/prenotazioni/behaviors/booking_folder/notifications/sms/__init__.py:38
 msgid "notify_on_move_sms_message_default_value"
 msgstr ""
 
 #. Default: "[Move] subject"
-#: redturtle/prenotazioni/behaviors/booking_folder/notifications/appio/__init__.py:179
-#: redturtle/prenotazioni/behaviors/booking_folder/notifications/email/__init__.py:188
+#: redturtle/prenotazioni/behaviors/booking_folder/notifications/appio/__init__.py:199
+#: redturtle/prenotazioni/behaviors/booking_folder/notifications/email/__init__.py:208
 msgid "notify_on_move_subject"
 msgstr ""
 
 #. Default: "[${prenotazioni_folder_title}] Booking date modified for ${title}"
 #: redturtle/prenotazioni/behaviors/booking_folder/notifications/email/__init__.py:59
 msgid "notify_on_move_subject_default_value"
 msgstr ""
 
 #. Default: "The message subject when a booking has been moved."
-#: redturtle/prenotazioni/behaviors/booking_folder/notifications/appio/__init__.py:183
-#: redturtle/prenotazioni/behaviors/booking_folder/notifications/email/__init__.py:192
+#: redturtle/prenotazioni/behaviors/booking_folder/notifications/appio/__init__.py:203
+#: redturtle/prenotazioni/behaviors/booking_folder/notifications/email/__init__.py:212
 msgid "notify_on_move_subject_help"
 msgstr ""
 
 #. Default: "Notify when rejected."
 #: redturtle/prenotazioni/content/prenotazioni_folder.py:463
 msgid "notify_on_refuse"
 msgstr ""
@@ -1395,51 +1535,51 @@
 
 #. Default: "Notify via mail the user when his booking has been rejected."
 #: redturtle/prenotazioni/content/prenotazioni_folder.py:464
 msgid "notify_on_refuse_help"
 msgstr ""
 
 #. Default: "[Refuse] message"
-#: redturtle/prenotazioni/behaviors/booking_folder/notifications/appio/__init__.py:215
-#: redturtle/prenotazioni/behaviors/booking_folder/notifications/email/__init__.py:224
-#: redturtle/prenotazioni/behaviors/booking_folder/notifications/sms/__init__.py:114
+#: redturtle/prenotazioni/behaviors/booking_folder/notifications/appio/__init__.py:235
+#: redturtle/prenotazioni/behaviors/booking_folder/notifications/email/__init__.py:244
+#: redturtle/prenotazioni/behaviors/booking_folder/notifications/sms/__init__.py:124
 msgid "notify_on_refuse_message"
 msgstr ""
 
 #. Default: "The booking ${booking_type} of ${booking_date} at ${booking_time} was refused."
 #: redturtle/prenotazioni/behaviors/booking_folder/notifications/email/__init__.py:91
 msgid "notify_on_refuse_message_default_value"
 msgstr ""
 
 #. Default: "The message text when a booking has been refused."
-#: redturtle/prenotazioni/behaviors/booking_folder/notifications/appio/__init__.py:219
-#: redturtle/prenotazioni/behaviors/booking_folder/notifications/email/__init__.py:228
-#: redturtle/prenotazioni/behaviors/booking_folder/notifications/sms/__init__.py:118
+#: redturtle/prenotazioni/behaviors/booking_folder/notifications/appio/__init__.py:239
+#: redturtle/prenotazioni/behaviors/booking_folder/notifications/email/__init__.py:248
+#: redturtle/prenotazioni/behaviors/booking_folder/notifications/sms/__init__.py:128
 msgid "notify_on_refuse_message_help"
 msgstr ""
 
 #. Default: "[${prenotazioni_folder_title}]: The booking ${booking_type} of ${booking_date} at ${booking_time} was refused."
 #: redturtle/prenotazioni/behaviors/booking_folder/notifications/sms/__init__.py:48
 msgid "notify_on_refuse_sms_message_default_value"
 msgstr ""
 
 #. Default: "[Refuse] subject"
-#: redturtle/prenotazioni/behaviors/booking_folder/notifications/appio/__init__.py:203
-#: redturtle/prenotazioni/behaviors/booking_folder/notifications/email/__init__.py:212
+#: redturtle/prenotazioni/behaviors/booking_folder/notifications/appio/__init__.py:223
+#: redturtle/prenotazioni/behaviors/booking_folder/notifications/email/__init__.py:232
 msgid "notify_on_refuse_subject"
 msgstr ""
 
 #. Default: "[${prenotazioni_folder_title}] Booking refused for ${title}"
 #: redturtle/prenotazioni/behaviors/booking_folder/notifications/email/__init__.py:81
 msgid "notify_on_refuse_subject_default_value"
 msgstr ""
 
 #. Default: "The message subject when a booking has been refused."
-#: redturtle/prenotazioni/behaviors/booking_folder/notifications/appio/__init__.py:207
-#: redturtle/prenotazioni/behaviors/booking_folder/notifications/email/__init__.py:216
+#: redturtle/prenotazioni/behaviors/booking_folder/notifications/appio/__init__.py:227
+#: redturtle/prenotazioni/behaviors/booking_folder/notifications/email/__init__.py:236
 msgid "notify_on_refuse_subject_help"
 msgstr ""
 
 #. Default: "Notify when created."
 #: redturtle/prenotazioni/content/prenotazioni_folder.py:436
 msgid "notify_on_submit"
 msgstr ""
@@ -1456,51 +1596,51 @@
 
 #. Default: "Notify via mail the user when his booking has been created. If auto-confirm flag is selected and confirm notify is selected, this one will be ignored."
 #: redturtle/prenotazioni/content/prenotazioni_folder.py:437
 msgid "notify_on_submit_help"
 msgstr ""
 
 #. Default: "[Created] message"
-#: redturtle/prenotazioni/behaviors/booking_folder/notifications/appio/__init__.py:143
-#: redturtle/prenotazioni/behaviors/booking_folder/notifications/email/__init__.py:152
-#: redturtle/prenotazioni/behaviors/booking_folder/notifications/sms/__init__.py:78
+#: redturtle/prenotazioni/behaviors/booking_folder/notifications/appio/__init__.py:163
+#: redturtle/prenotazioni/behaviors/booking_folder/notifications/email/__init__.py:172
+#: redturtle/prenotazioni/behaviors/booking_folder/notifications/sms/__init__.py:88
 msgid "notify_on_submit_message"
 msgstr ""
 
 #. Default: "Booking ${booking_type} for ${booking_date} at ${booking_time} has been created.<br/><br/>You can see details and print a reminder following this <a href=${booking_print_url}>link</a>."
 #: redturtle/prenotazioni/behaviors/booking_folder/notifications/email/__init__.py:28
 msgid "notify_on_submit_message_default_value"
 msgstr ""
 
 #. Default: "The message text when a booking has been created."
-#: redturtle/prenotazioni/behaviors/booking_folder/notifications/appio/__init__.py:147
-#: redturtle/prenotazioni/behaviors/booking_folder/notifications/email/__init__.py:156
-#: redturtle/prenotazioni/behaviors/booking_folder/notifications/sms/__init__.py:82
+#: redturtle/prenotazioni/behaviors/booking_folder/notifications/appio/__init__.py:167
+#: redturtle/prenotazioni/behaviors/booking_folder/notifications/email/__init__.py:176
+#: redturtle/prenotazioni/behaviors/booking_folder/notifications/sms/__init__.py:92
 msgid "notify_on_submit_message_help"
 msgstr ""
 
 #. Default: "[${prenotazioni_folder_title}]: Booking ${booking_type} for ${booking_date} at ${booking_time} has been created.\nSee details or delete it: ${booking_print_url} ."
 #: redturtle/prenotazioni/behaviors/booking_folder/notifications/sms/__init__.py:18
 msgid "notify_on_submit_sms_message_default_value"
 msgstr ""
 
 #. Default: "[Created] subject"
-#: redturtle/prenotazioni/behaviors/booking_folder/notifications/appio/__init__.py:131
-#: redturtle/prenotazioni/behaviors/booking_folder/notifications/email/__init__.py:140
+#: redturtle/prenotazioni/behaviors/booking_folder/notifications/appio/__init__.py:151
+#: redturtle/prenotazioni/behaviors/booking_folder/notifications/email/__init__.py:160
 msgid "notify_on_submit_subject"
 msgstr ""
 
 #. Default: "[${prenotazioni_folder_title}] Booking created"
 #: redturtle/prenotazioni/behaviors/booking_folder/notifications/email/__init__.py:18
 msgid "notify_on_submit_subject_default_value"
 msgstr ""
 
 #. Default: "The message subject when a booking has been created."
-#: redturtle/prenotazioni/behaviors/booking_folder/notifications/appio/__init__.py:135
-#: redturtle/prenotazioni/behaviors/booking_folder/notifications/email/__init__.py:144
+#: redturtle/prenotazioni/behaviors/booking_folder/notifications/appio/__init__.py:155
+#: redturtle/prenotazioni/behaviors/booking_folder/notifications/email/__init__.py:164
 msgid "notify_on_submit_subject_help"
 msgstr ""
 
 #. Default: "Pause end"
 #: redturtle/prenotazioni/content/prenotazioni_folder.py:124
 msgid "pause_end_label"
 msgstr ""
@@ -1566,20 +1706,20 @@
 
 #. Default: "Reject booking"
 #: redturtle/prenotazioni/browser/templates/prenotazione.pt:176
 msgid "reject_booking"
 msgstr ""
 
 #. Default: "Set how many days before of a booking date the user will be notified about it."
-#: redturtle/prenotazioni/content/prenotazioni_folder.py:488
+#: redturtle/prenotazioni/content/prenotazioni_folder.py:497
 msgid "reminder_notification_gap_description"
 msgstr ""
 
 #. Default: "Booking reminder days"
-#: redturtle/prenotazioni/content/prenotazioni_folder.py:484
+#: redturtle/prenotazioni/content/prenotazioni_folder.py:493
 msgid "reminder_notification_gap_label"
 msgstr ""
 
 #. Default: "Code"
 #: redturtle/prenotazioni/browser/templates/prenotazioni_search.pt:58
 msgid "reservation_code"
 msgstr ""
@@ -1621,20 +1761,20 @@
 
 #. Default: "seleziona l'opzione desiderata dal gruppo di radio button seguente"
 #: redturtle/prenotazioni/browser/z3c_custom_widget.py:153
 msgid "select-option"
 msgstr ""
 
 #. Default: "AppIO service code related to the current booking type"
-#: redturtle/prenotazioni/behaviors/booking_folder/notifications/appio/__init__.py:293
+#: redturtle/prenotazioni/behaviors/booking_folder/notifications/appio/__init__.py:339
 msgid "service_code_help"
 msgstr ""
 
 #. Default: "AppIO service code."
-#: redturtle/prenotazioni/behaviors/booking_folder/notifications/appio/__init__.py:289
+#: redturtle/prenotazioni/behaviors/booking_folder/notifications/appio/__init__.py:335
 msgid "service_code_label"
 msgstr ""
 
 #. Default: "This gate has some booking schedule in this time period."
 #: redturtle/prenotazioni/browser/vacations.py:216
 msgid "slot_conflict_error"
 msgstr ""
@@ -1654,15 +1794,15 @@
 
 #. Default: "Selected day is too big for that month for \"to\" field."
 #: redturtle/prenotazioni/content/validators.py:191
 msgid "to_month_too_days_error"
 msgstr ""
 
 #. Default: "You can't add a booking with type '${booking_type}'."
-#: redturtle/prenotazioni/restapi/services/booking/add.py:134
+#: redturtle/prenotazioni/restapi/services/booking/add.py:132
 msgid "unauthorized_add_vacation"
 msgstr ""
 
 #. Default: "Unbookable time"
 #: redturtle/prenotazioni/browser/templates/prenotazione_macros.pt:452
 msgid "unbookable_time"
 msgstr ""
@@ -1693,7 +1833,22 @@
 msgid "week_table_overrides_label"
 msgstr ""
 
 #. Default: "You tried to delete booking with a wrong action."
 #: redturtle/prenotazioni/browser/delete_reservation.py:98
 msgid "wrong_authenticator"
 msgstr ""
+
+msgid "pending"
+msgstr "In attesa"
+
+msgid "private"
+msgstr "Privato"
+
+msgid "confirmed"
+msgstr "Confermato"
+
+msgid "refused"
+msgstr "Rifiutato"
+
+msgid "canceled"
+msgstr "Annullato"
```

### Comparing `redturtle.prenotazioni-2.6.5/src/redturtle/prenotazioni/locales/update.py` & `redturtle.prenotazioni-2.7.0/src/redturtle/prenotazioni/locales/update.py`

 * *Files identical despite different names*

### Comparing `redturtle.prenotazioni-2.6.5/src/redturtle/prenotazioni/locales/update.sh` & `redturtle.prenotazioni-2.7.0/src/redturtle/prenotazioni/locales/update.sh`

 * *Files identical despite different names*

### Comparing `redturtle.prenotazioni-2.6.5/src/redturtle/prenotazioni/permissions.zcml` & `redturtle.prenotazioni-2.7.0/src/redturtle/prenotazioni/permissions.zcml`

 * *Files identical despite different names*

### Comparing `redturtle.prenotazioni-2.6.5/src/redturtle/prenotazioni/profiles/default/actions.xml` & `redturtle.prenotazioni-2.7.0/src/redturtle/prenotazioni/profiles/default/actions.xml`

 * *Files identical despite different names*

### Comparing `redturtle.prenotazioni-2.6.5/src/redturtle/prenotazioni/profiles/default/registry/caching.xml` & `redturtle.prenotazioni-2.7.0/src/redturtle/prenotazioni/profiles/default/registry/caching.xml`

 * *Files identical despite different names*

### Comparing `redturtle.prenotazioni-2.6.5/src/redturtle/prenotazioni/profiles/default/registry/resources.xml` & `redturtle.prenotazioni-2.7.0/src/redturtle/prenotazioni/profiles/default/registry/resources.xml`

 * *Files identical despite different names*

### Comparing `redturtle.prenotazioni-2.6.5/src/redturtle/prenotazioni/profiles/default/registry/settings.xml` & `redturtle.prenotazioni-2.7.0/src/redturtle/prenotazioni/profiles/default/registry/settings.xml`

 * *Files identical despite different names*

### Comparing `redturtle.prenotazioni-2.6.5/src/redturtle/prenotazioni/profiles/default/rolemap.xml` & `redturtle.prenotazioni-2.7.0/src/redturtle/prenotazioni/profiles/default/rolemap.xml`

 * *Files 1% similar despite different names*

#### Comparing `redturtle.prenotazioni-2.6.5/src/redturtle/prenotazioni/profiles/default/rolemap.xml` & `redturtle.prenotazioni-2.7.0/src/redturtle/prenotazioni/profiles/default/rolemap.xml`

```diff
@@ -72,9 +72,12 @@
       <role name="Manager"/>
       <role name="Site Administrator"/>
       <role name="Owner"/>
       <role name="Editor"/>
       <role name="Reviewer"/>
       <role name="Contributor"/>
     </permission>
+    <permission acquire="True" name="CMFEditions: Save new version">
+      <role name="Bookings Manager"/>
+    </permission>
   </permissions>
 </rolemap>
```

### Comparing `redturtle.prenotazioni-2.6.5/src/redturtle/prenotazioni/profiles/default/types/Prenotazione.xml` & `redturtle.prenotazioni-2.7.0/src/redturtle/prenotazioni/profiles/default/types/Prenotazione.xml`

 * *Files 4% similar despite different names*

#### Comparing `redturtle.prenotazioni-2.6.5/src/redturtle/prenotazioni/profiles/default/types/Prenotazione.xml` & `redturtle.prenotazioni-2.7.0/src/redturtle/prenotazioni/profiles/default/types/Prenotazione.xml`

```diff
@@ -21,19 +21,19 @@
     <element value="plone.app.dexterity.behaviors.discussion.IAllowDiscussion"/>
     <element value="plone.app.dexterity.behaviors.exclfromnav.IExcludeFromNavigation"/>
     <element value="plone.app.dexterity.behaviors.id.IShortName"/>
     <element value="plone.app.dexterity.behaviors.metadata.IOwnership"/>
     <element value="plone.app.dexterity.behaviors.metadata.IPublication"/>
     <element value="plone.app.dexterity.behaviors.metadata.ICategorization"/>
     <element value="plone.app.dexterity.behaviors.metadata.IBasic"/>
-    <!--<element value="plone.app.referenceablebehavior.referenceable.IReferenceable" />-->
     <element value="plone.app.lockingbehavior.behaviors.ILocking"/>
+    <element value="plone.versioning"/>
+    <!--<element value="plone.app.referenceablebehavior.referenceable.IReferenceable" />-->
     <!--<element value="plone.app.contenttypes.behaviors.leadimage.ILeadImage"/>-->
     <!--<element value="plone.app.relationfield.behavior.IRelatedItems"/>-->
-    <!--<element value="plone.app.versioningbehavior.behaviors.IVersionable" />-->
     <!--<element value="plone.app.contenttypes.behaviors.tableofcontents.ITableOfContents"/>-->
     <!--<element value="plone.app.contenttypes.behaviors.richtext.IRichText"/>-->
   </property>
   <!-- View information -->
   <property name="add_view_expr">string:${folder_url}/++add++Prenotazione</property>
   <property name="default_view">prenotazione_view</property>
   <property name="default_view_fallback">False</property>
```

### Comparing `redturtle.prenotazioni-2.6.5/src/redturtle/prenotazioni/profiles/default/types/PrenotazioneType.xml` & `redturtle.prenotazioni-2.7.0/src/redturtle/prenotazioni/profiles/default/types/PrenotazioneType.xml`

 * *Files identical despite different names*

### Comparing `redturtle.prenotazioni-2.6.5/src/redturtle/prenotazioni/profiles/default/types/PrenotazioniDay.xml` & `redturtle.prenotazioni-2.7.0/src/redturtle/prenotazioni/profiles/default/types/PrenotazioniDay.xml`

 * *Files identical despite different names*

### Comparing `redturtle.prenotazioni-2.6.5/src/redturtle/prenotazioni/profiles/default/types/PrenotazioniFolder.xml` & `redturtle.prenotazioni-2.7.0/src/redturtle/prenotazioni/profiles/default/types/PrenotazioniFolder.xml`

 * *Files identical despite different names*

### Comparing `redturtle.prenotazioni-2.6.5/src/redturtle/prenotazioni/profiles/default/types/PrenotazioniWeek.xml` & `redturtle.prenotazioni-2.7.0/src/redturtle/prenotazioni/profiles/default/types/PrenotazioniWeek.xml`

 * *Files identical despite different names*

### Comparing `redturtle.prenotazioni-2.6.5/src/redturtle/prenotazioni/profiles/default/types/PrenotazioniYear.xml` & `redturtle.prenotazioni-2.7.0/src/redturtle/prenotazioni/profiles/default/types/PrenotazioniYear.xml`

 * *Files identical despite different names*

### Comparing `redturtle.prenotazioni-2.6.5/src/redturtle/prenotazioni/profiles/default/types.xml` & `redturtle.prenotazioni-2.7.0/src/redturtle/prenotazioni/profiles/default/types.xml`

 * *Files identical despite different names*

### Comparing `redturtle.prenotazioni-2.6.5/src/redturtle/prenotazioni/profiles/default/workflows/prenotazioni_workflow/definition.xml` & `redturtle.prenotazioni-2.7.0/src/redturtle/prenotazioni/profiles/default/workflows/prenotazioni_workflow/definition.xml`

 * *Files identical despite different names*

### Comparing `redturtle.prenotazioni-2.6.5/src/redturtle/prenotazioni/profiles/default/workflows/prenotazionifolder_workflow/definition.xml` & `redturtle.prenotazioni-2.7.0/src/redturtle/prenotazioni/profiles/default/workflows/prenotazionifolder_workflow/definition.xml`

 * *Files identical despite different names*

### Comparing `redturtle.prenotazioni-2.6.5/src/redturtle/prenotazioni/profiles/default/workflows.xml` & `redturtle.prenotazioni-2.7.0/src/redturtle/prenotazioni/profiles/default/workflows.xml`

 * *Files identical despite different names*

### Comparing `redturtle.prenotazioni-2.6.5/src/redturtle/prenotazioni/profiles/to_1402/contentrules.xml` & `redturtle.prenotazioni-2.7.0/src/redturtle/prenotazioni/profiles/to_1402/contentrules.xml`

 * *Files identical despite different names*

### Comparing `redturtle.prenotazioni-2.6.5/src/redturtle/prenotazioni/profiles/to_2005/rolemap.xml` & `redturtle.prenotazioni-2.7.0/src/redturtle/prenotazioni/profiles/to_2005/rolemap.xml`

 * *Files identical despite different names*

### Comparing `redturtle.prenotazioni-2.6.5/src/redturtle/prenotazioni/profiles/to_2006/workflows/prenotazioni_workflow/definition.xml` & `redturtle.prenotazioni-2.7.0/src/redturtle/prenotazioni/profiles/to_2006/workflows/prenotazioni_workflow/definition.xml`

 * *Files identical despite different names*

### Comparing `redturtle.prenotazioni-2.6.5/src/redturtle/prenotazioni/restapi/serializers/adapters/prenotazione.py` & `redturtle.prenotazioni-2.7.0/src/redturtle/prenotazioni/restapi/serializers/adapters/prenotazione.py`

 * *Files 4% similar despite different names*

```diff
@@ -1,28 +1,42 @@
 # -*- coding: utf-8 -*-
 import json
 
 from plone import api
 from plone.restapi.interfaces import IFieldSerializer
 from plone.restapi.interfaces import ISerializeToJson
 from plone.restapi.serializer.converters import json_compatible
+from Products.CMFCore.utils import getToolByName
 from zope.component import adapter
 from zope.component import getMultiAdapter
 from zope.i18n import translate
 from zope.interface import implementer
 from zope.interface.interfaces import ComponentLookupError
 from zope.publisher.interfaces import IRequest
 from zope.schema import getFields
 
 from redturtle.prenotazioni import logger
 from redturtle.prenotazioni.content.prenotazione import IPrenotazione
 from redturtle.prenotazioni.content.prenotazione_type import IPrenotazioneType
 from redturtle.prenotazioni.interfaces import ISerializeToPrenotazioneSearchableItem
 
 
+def get_booking_wf_state_title(context):
+    portal_workflow = getToolByName(context, "portal_workflow")
+    state = portal_workflow.getInfoFor(context, "review_state")
+
+    return translate(
+        msgid=state,
+        domain="plone",
+        target_language=getToolByName(
+            context, "portal_languages"
+        ).getPreferredLanguage(),
+    )
+
+
 @implementer(ISerializeToJson)
 @adapter(IPrenotazione, IRequest)
 class PrenotazioneSerializer:
     def __init__(self, prenotazione, request):
         self.prenotazione = prenotazione
         self.request = request
 
@@ -55,14 +69,15 @@
             and booking_date.date() != booking_expiration_date.date()
         ):
             logger.warning("Booking date and expiration date are different, fixing")
             booking_date = booking_date.date()
             booking_expiration_date = booking_expiration_date.replace(
                 booking_date.year, booking_date.month, booking_date.day
             )
+
         return {
             "@id": self.prenotazione.absolute_url(),
             "UID": self.prenotazione.UID(),
             "@type": self.prenotazione.portal_type,
             "title": self.prenotazione.title,
             "description": self.prenotazione.description,
             "gate": self.prenotazione.gate,
@@ -71,17 +86,15 @@
             "email": self.prenotazione.email,
             "fiscalcode": fiscalcode,
             "company": self.prenotazione.company,
             "staff_notes": self.prenotazione.staff_notes,
             "booking_date": json_compatible(booking_date),
             "booking_expiration_date": json_compatible(booking_expiration_date),
             "booking_status": status["review_state"],
-            "booking_status_label": translate(
-                status["review_state"], context=self.request
-            ),
+            "booking_status_label": get_booking_wf_state_title(self.prenotazione),
             "booking_type": self.prenotazione.booking_type,
             "booking_folder_uid": booking_folder.UID(),
             "vacation": self.prenotazione.isVacation(),
             "booking_code": self.prenotazione.getBookingCode(),
             "notify_on_confirm": booking_folder.notify_on_confirm,
             "cosa_serve": requirements,  # BBB
             "requirements": requirements,
@@ -111,17 +124,15 @@
             "booking_expiration_date": json_compatible(
                 self.prenotazione.booking_expiration_date
             ),
             "booking_type": self.prenotazione.booking_type,
             # "booking_room": None,
             "booking_gate": self.prenotazione.gate,
             "booking_status": status["review_state"],
-            "booking_status_label": translate(
-                status["review_state"], context=self.request
-            ),
+            "booking_status_label": get_booking_wf_state_title(self.prenotazione),
             "booking_status_date": json_compatible(status["time"]),
             "booking_status_notes": status["comments"],
             "email": self.prenotazione.email,
             "fiscalcode": self.prenotazione.fiscalcode,
             "phone": self.prenotazione.phone,
             "staff_notes": self.prenotazione.staff_notes,
             "company": self.prenotazione.company,
```

### Comparing `redturtle.prenotazioni-2.6.5/src/redturtle/prenotazioni/restapi/serializers/adapters/prenotazione_type.py` & `redturtle.prenotazioni-2.7.0/src/redturtle/prenotazioni/restapi/serializers/adapters/prenotazioni_folder.py`

 * *Files 27% similar despite different names*

```diff
@@ -1,26 +1,24 @@
 # -*- coding: utf-8 -*-
-from plone import api
+from plone.restapi.interfaces import ISerializeToJson
+from plone.restapi.serializer.dxcontent import SerializeFolderToJson
 from zope.component import adapter
+from zope.component import getMultiAdapter
 from zope.interface import implementer
 
-from redturtle.prenotazioni.content.prenotazione_type import IPrenotazioneType
+from redturtle.prenotazioni.content.prenotazioni_folder import IPrenotazioniFolder
 from redturtle.prenotazioni.interfaces import IRedturtlePrenotazioniLayer
 from redturtle.prenotazioni.interfaces import ISerializeToRetroCompatibleJson
 
 
-@implementer(ISerializeToRetroCompatibleJson)
-@adapter(IPrenotazioneType, IRedturtlePrenotazioniLayer)
-class PrenotazioneTypeRetroCompatibleSerializer:
-    """PrenotazioneType c.t. serializer retrocompatible with earlier frontend implementation"""
+@implementer(ISerializeToJson)
+@adapter(IPrenotazioniFolder, IRedturtlePrenotazioniLayer)
+class PrenotazioniFolderSerializer(SerializeFolderToJson):
+    def __call__(self, *args, **kwargs):
+        res = super().__call__()
 
-    def __init__(self, context, request):
-        self.context = context
-        self.request = request
+        res["booking_types"] = [
+            getMultiAdapter((i, self.request), ISerializeToRetroCompatibleJson)()
+            for i in self.context.get_booking_types()
+        ]
 
-    def __call__(self, *args, **kwargs):
-        hidden = api.content.get_state(self.context) not in ("published",)
-        return {
-            "name": self.context.title,
-            "duration": str(self.context.duration),
-            "hidden": hidden,
-        }
+        return res
```

### Comparing `redturtle.prenotazioni-2.6.5/src/redturtle/prenotazioni/restapi/serializers/adapters/slot.py` & `redturtle.prenotazioni-2.7.0/src/redturtle/prenotazioni/restapi/serializers/adapters/slot.py`

 * *Files identical despite different names*

### Comparing `redturtle.prenotazioni-2.6.5/src/redturtle/prenotazioni/restapi/services/available_slots/get.py` & `redturtle.prenotazioni-2.7.0/src/redturtle/prenotazioni/restapi/services/available_slots/get.py`

 * *Files 3% similar despite different names*

```diff
@@ -55,15 +55,15 @@
                 or datetime.date(start.year + 1, start.month, start.day)
             )
             bypass_user_restrictions = True
         else:
             end = start.replace(day=calendar.monthrange(start.year, start.month)[1])
 
         if start > end:
-            msg = self.context.translate(
+            msg = api.portal.translate(
                 _(
                     "available_slots_wrong_dates",
                     default="End date should be greater than start.",
                 )
             )
             raise BadRequest(msg)
```

### Comparing `redturtle.prenotazioni-2.6.5/src/redturtle/prenotazioni/restapi/services/booking/add.py` & `redturtle.prenotazioni-2.7.0/src/redturtle/prenotazioni/restapi/services/booking/add.py`

 * *Files 5% similar despite different names*

```diff
@@ -56,17 +56,15 @@
                     duration=duration,
                 )
             else:
                 obj = booker.book(data=book_data)
         except BookerException as e:
             raise BadRequest(e) from e
         if not obj:
-            msg = self.context.translate(
-                _("Sorry, this slot is not available anymore.")
-            )
+            msg = api.portal.translate(_("Sorry, this slot is not available anymore."))
             raise BadRequest(msg)
 
         # other_fields: {
         #   booking_address: prenotazioneObj.booking_folder?.address?.['@id'],
         #   booking_office: prenotazioneObj.booking_office?.['url'],
         #   booking_contact_info: (prenotazioneObj.booking_office?.contact_info || []).map((c) => c['@id']),
         # },
@@ -108,57 +106,57 @@
             logger.exception("Error while saving %s field %s for %s", value, field, obj)
 
     def validate(self):
         data = json_body(self.request)
         data_fields = {field["name"]: field["value"] for field in data["fields"]}
 
         if data.get("force", False) and not self.is_manager:
-            msg = self.context.translate(_("You are not allowed to force the gate."))
+            msg = api.portal.translate(_("You are not allowed to force the gate."))
             raise BadRequest(msg)
 
         # campi che non sono nei data_fields
         for field in ("booking_date", "booking_type"):
             if not data.get(field):
-                msg = self.context.translate(
+                msg = api.portal.translate(
                     _(
                         "Required input '${field}' is missing.",
                         mapping=dict(field=field),
                     )
                 )
                 raise BadRequest(msg)
 
         if data["booking_type"] in [VACATION_TYPE]:
             if not api.user.has_permission(
                 "redturtle.prenotazioni: Manage Prenotazioni", obj=self.context
             ):
-                msg = self.context.translate(
+                msg = api.portal.translate(
                     _(
                         "unauthorized_add_vacation",
                         "You can't add a booking with type '${booking_type}'.",
                         mapping=dict(booking_type=data["booking_type"]),
                     )
                 )
                 raise BadRequest(msg)
             # TODO: check permission for special booking_types ?
             return data, data_fields
 
         for field in self.required_fields:
             if not data_fields.get(field):
-                msg = self.context.translate(
+                msg = api.portal.translate(
                     _(
                         "Required input '${field}' is missing.",
                         mapping=dict(field=field),
                     )
                 )
                 raise BadRequest(msg)
 
         if data["booking_type"] not in [
             _t.title for _t in self.context.get_booking_types()
         ]:
-            msg = self.context.translate(
+            msg = api.portal.translate(
                 _(
                     "Unknown booking type '${booking_type}'.",
                     mapping=dict(booking_type=data["booking_type"]),
                 )
             )
             raise BadRequest(msg)
```

### Comparing `redturtle.prenotazioni-2.6.5/src/redturtle/prenotazioni/restapi/services/booking/configure.zcml` & `redturtle.prenotazioni-2.7.0/src/redturtle/prenotazioni/restapi/services/booking/configure.zcml`

 * *Files identical despite different names*

### Comparing `redturtle.prenotazioni-2.6.5/src/redturtle/prenotazioni/restapi/services/booking/delete.py` & `redturtle.prenotazioni-2.7.0/src/redturtle/prenotazioni/restapi/services/booking/delete.py`

 * *Files identical despite different names*

### Comparing `redturtle.prenotazioni-2.6.5/src/redturtle/prenotazioni/restapi/services/booking/get.py` & `redturtle.prenotazioni-2.7.0/src/redturtle/prenotazioni/restapi/services/booking/get.py`

 * *Files identical despite different names*

### Comparing `redturtle.prenotazioni-2.6.5/src/redturtle/prenotazioni/restapi/services/booking/move.py` & `redturtle.prenotazioni-2.7.0/src/redturtle/prenotazioni/restapi/services/booking/move.py`

 * *Files identical despite different names*

### Comparing `redturtle.prenotazioni-2.6.5/src/redturtle/prenotazioni/restapi/services/booking/notify_about_confirm.py` & `redturtle.prenotazioni-2.7.0/src/redturtle/prenotazioni/restapi/services/booking/notify_about_confirm.py`

 * *Files identical despite different names*

### Comparing `redturtle.prenotazioni-2.6.5/src/redturtle/prenotazioni/restapi/services/booking/vacation.py` & `redturtle.prenotazioni-2.7.0/src/redturtle/prenotazioni/restapi/services/booking/vacation.py`

 * *Files identical despite different names*

### Comparing `redturtle.prenotazioni-2.6.5/src/redturtle/prenotazioni/restapi/services/booking_schema/get.py` & `redturtle.prenotazioni-2.7.0/src/redturtle/prenotazioni/restapi/services/booking_schema/get.py`

 * *Files 4% similar despite different names*

```diff
@@ -91,26 +91,30 @@
             value = ""
             is_readonly = False
 
             if current_user:
                 if field == "email":
                     value = current_user.getProperty("email")
                     # readonly solo se ha un valore
+                    if value:
+                        value = value.strip()
                     is_readonly = bool(value)
                 if field == "phone":
                     value = current_user.getProperty("phone", "")
                     # readonly solo se ha un valore (?) non lo lascerei mai readonly permettendo al cittadino
                     # di modificare il proprio numero di telefono
                     # is_readonly = bool(value)
                 if field == "fiscalcode":
                     value = current_user.getUserName()
                     is_readonly = True
                 if field == "title":
                     value = current_user.getProperty("fullname")
                     # readonly solo se ha un valore
+                    if value:
+                        value = value.strip()
                     is_readonly = bool(value)
 
             fields_list.append(
                 {
                     "label": self.labels_mapping.get(field, {}).get("label", field),
                     "desc": self.labels_mapping.get(field, {}).get("description", ""),
                     "type": self.field_type_mapping.get(field, "text"),
```

### Comparing `redturtle.prenotazioni-2.6.5/src/redturtle/prenotazioni/restapi/services/bookings/configure.zcml` & `redturtle.prenotazioni-2.7.0/src/redturtle/prenotazioni/restapi/services/bookings/configure.zcml`

 * *Files identical despite different names*

### Comparing `redturtle.prenotazioni-2.6.5/src/redturtle/prenotazioni/restapi/services/bookings/search.py` & `redturtle.prenotazioni-2.7.0/src/redturtle/prenotazioni/restapi/services/bookings/search.py`

 * *Files 4% similar despite different names*

```diff
@@ -40,15 +40,19 @@
             "redturtle.prenotazioni: search prenotazioni", obj=self.context
         ):
             userid = self.request.get("userid", None)
         else:
             userid = api.user.get_current().getUserId()
 
         if userid:
-            query["fiscalcode"] = userid.upper()
+            if userid.lower().startswith("tinit-") and userid[6:]:
+                # search for both the original and the prefixed fiscalcode
+                query["fiscalcode"] = [userid.upper(), userid[6:].upper()]
+            else:
+                query["fiscalcode"] = userid.upper()
 
         start_date = self.request.get("from", None)
         end_date = self.request.get("to", None)
         gate = self.request.get("gate", None)
         booking_type = self.request.get("booking_type", None)
         SearchableText = self.request.get("SearchableText", None)
         review_state = self.request.get("review_state", None)
```

### Comparing `redturtle.prenotazioni-2.6.5/src/redturtle/prenotazioni/restapi/services/day/day.py` & `redturtle.prenotazioni-2.7.0/src/redturtle/prenotazioni/restapi/services/day/day.py`

 * *Files identical despite different names*

### Comparing `redturtle.prenotazioni-2.6.5/src/redturtle/prenotazioni/restapi/services/types/get.py` & `redturtle.prenotazioni-2.7.0/src/redturtle/prenotazioni/restapi/services/types/get.py`

 * *Files identical despite different names*

### Comparing `redturtle.prenotazioni-2.6.5/src/redturtle/prenotazioni/scripts/notify_upcoming_bookings.py` & `redturtle.prenotazioni-2.7.0/src/redturtle/prenotazioni/scripts/notify_upcoming_bookings.py`

 * *Files identical despite different names*

### Comparing `redturtle.prenotazioni-2.6.5/src/redturtle/prenotazioni/setuphandlers.py` & `redturtle.prenotazioni-2.7.0/src/redturtle/prenotazioni/setuphandlers.py`

 * *Files identical despite different names*

### Comparing `redturtle.prenotazioni-2.6.5/src/redturtle/prenotazioni/testing.py` & `redturtle.prenotazioni-2.7.0/src/redturtle/prenotazioni/testing.py`

 * *Files identical despite different names*

### Comparing `redturtle.prenotazioni-2.6.5/src/redturtle/prenotazioni/tests/helpers.py` & `redturtle.prenotazioni-2.7.0/src/redturtle/prenotazioni/tests/helpers.py`

 * *Files identical despite different names*

### Comparing `redturtle.prenotazioni-2.6.5/src/redturtle/prenotazioni/tests/test_add_block.py` & `redturtle.prenotazioni-2.7.0/src/redturtle/prenotazioni/tests/test_add_block.py`

 * *Files identical despite different names*

### Comparing `redturtle.prenotazioni-2.6.5/src/redturtle/prenotazioni/tests/test_add_booking.py` & `redturtle.prenotazioni-2.7.0/src/redturtle/prenotazioni/tests/test_add_booking.py`

 * *Files identical despite different names*

### Comparing `redturtle.prenotazioni-2.6.5/src/redturtle/prenotazioni/tests/test_add_booking_type.py` & `redturtle.prenotazioni-2.7.0/src/redturtle/prenotazioni/tests/test_add_booking_type.py`

 * *Files identical despite different names*

### Comparing `redturtle.prenotazioni-2.6.5/src/redturtle/prenotazioni/tests/test_available_slots.py` & `redturtle.prenotazioni-2.7.0/src/redturtle/prenotazioni/tests/test_available_slots.py`

 * *Files identical despite different names*

### Comparing `redturtle.prenotazioni-2.6.5/src/redturtle/prenotazioni/tests/test_base_slot.py` & `redturtle.prenotazioni-2.7.0/src/redturtle/prenotazioni/tests/test_base_slot.py`

 * *Files identical despite different names*

### Comparing `redturtle.prenotazioni-2.6.5/src/redturtle/prenotazioni/tests/test_booker_choose_available_slot.py` & `redturtle.prenotazioni-2.7.0/src/redturtle/prenotazioni/tests/test_booker_choose_available_slot.py`

 * *Files identical despite different names*

### Comparing `redturtle.prenotazioni-2.6.5/src/redturtle/prenotazioni/tests/test_booking_info.py` & `redturtle.prenotazioni-2.7.0/src/redturtle/prenotazioni/tests/test_booking_info.py`

 * *Files identical despite different names*

### Comparing `redturtle.prenotazioni-2.6.5/src/redturtle/prenotazioni/tests/test_booking_notify.py` & `redturtle.prenotazioni-2.7.0/src/redturtle/prenotazioni/tests/test_booking_notify.py`

 * *Files identical despite different names*

### Comparing `redturtle.prenotazioni-2.6.5/src/redturtle/prenotazioni/tests/test_booking_schema.py` & `redturtle.prenotazioni-2.7.0/src/redturtle/prenotazioni/tests/test_booking_schema.py`

 * *Files identical despite different names*

### Comparing `redturtle.prenotazioni-2.6.5/src/redturtle/prenotazioni/tests/test_bookings_num_limit.py` & `redturtle.prenotazioni-2.7.0/src/redturtle/prenotazioni/tests/test_bookings_num_limit.py`

 * *Files identical despite different names*

### Comparing `redturtle.prenotazioni-2.6.5/src/redturtle/prenotazioni/tests/test_browser_utilities_notify_upcoming_bookings.py` & `redturtle.prenotazioni-2.7.0/src/redturtle/prenotazioni/tests/test_browser_utilities_notify_upcoming_bookings.py`

 * *Files 2% similar despite different names*

```diff
@@ -60,14 +60,16 @@
             type="PrenotazioneType",
             title="Type B",
             duration=90,
             container=self.folder_prenotazioni,
             gates=["all"],
         )
 
+        api.content.transition(obj=self.folder_prenotazioni, transition="publish")
+
         self.today_8_0 = self.dt_local_to_utc(
             datetime.now().replace(hour=8, minute=0, second=0, microsecond=0)
         )
         self.tomorrow_8_0 = self.today_8_0 + timedelta(1)
         self.folder_prenotazioni.email_responsabile = ["admin@test.com"]
         api.portal.set_registry_record(
             "plone.portal_timezone",
```

### Comparing `redturtle.prenotazioni-2.6.5/src/redturtle/prenotazioni/tests/test_content_validators_validate_pause_table.py` & `redturtle.prenotazioni-2.7.0/src/redturtle/prenotazioni/tests/test_content_validators_validate_pause_table.py`

 * *Files identical despite different names*

### Comparing `redturtle.prenotazioni-2.6.5/src/redturtle/prenotazioni/tests/test_day.py` & `redturtle.prenotazioni-2.7.0/src/redturtle/prenotazioni/tests/test_day.py`

 * *Files identical despite different names*

### Comparing `redturtle.prenotazioni-2.6.5/src/redturtle/prenotazioni/tests/test_delete_booking.py` & `redturtle.prenotazioni-2.7.0/src/redturtle/prenotazioni/tests/test_delete_booking.py`

 * *Files identical despite different names*

### Comparing `redturtle.prenotazioni-2.6.5/src/redturtle/prenotazioni/tests/test_delete_booking_api.py` & `redturtle.prenotazioni-2.7.0/src/redturtle/prenotazioni/tests/test_delete_booking_api.py`

 * *Files identical despite different names*

### Comparing `redturtle.prenotazioni-2.6.5/src/redturtle/prenotazioni/tests/test_gates_overrides.py` & `redturtle.prenotazioni-2.7.0/src/redturtle/prenotazioni/tests/test_gates_overrides.py`

 * *Files identical despite different names*

### Comparing `redturtle.prenotazioni-2.6.5/src/redturtle/prenotazioni/tests/test_move_booking_api.py` & `redturtle.prenotazioni-2.7.0/src/redturtle/prenotazioni/tests/test_move_booking_api.py`

 * *Files 0% similar despite different names*

```diff
@@ -150,14 +150,15 @@
         response = self.api_session_bookings_manager.post(
             f"{self.folder_prenotazioni.absolute_url()}/@booking-move",
             json={
                 "booking_id": uid,
                 "booking_date": nextmonth.isoformat(),  # nextmonth
             },
         )
+
         self.assertEqual(response.status_code, 204)
 
         response = self.api_session_bookings_manager.get(
             f"{self.folder_prenotazioni.absolute_url()}/@booking/{uid}",
         )
         self.assertEqual(response.status_code, 200)
         self.assertEqual(
```

### Comparing `redturtle.prenotazioni-2.6.5/src/redturtle/prenotazioni/tests/test_notification_supervisor_utility.py` & `redturtle.prenotazioni-2.7.0/src/redturtle/prenotazioni/tests/test_notification_supervisor_utility.py`

 * *Files identical despite different names*

### Comparing `redturtle.prenotazioni-2.6.5/src/redturtle/prenotazioni/tests/test_pauses_overrides.py` & `redturtle.prenotazioni-2.7.0/src/redturtle/prenotazioni/tests/test_pauses_overrides.py`

 * *Files identical despite different names*

### Comparing `redturtle.prenotazioni-2.6.5/src/redturtle/prenotazioni/tests/test_prenotazione_email_sent_to_managers.py` & `redturtle.prenotazioni-2.7.0/src/redturtle/prenotazioni/tests/test_prenotazione_email_sent_to_managers.py`

 * *Files identical despite different names*

### Comparing `redturtle.prenotazioni-2.6.5/src/redturtle/prenotazioni/tests/test_prenotazione_events.py` & `redturtle.prenotazioni-2.7.0/src/redturtle/prenotazioni/tests/test_prenotazione_events.py`

 * *Files identical despite different names*

### Comparing `redturtle.prenotazioni-2.6.5/src/redturtle/prenotazioni/tests/test_prenotazione_searchable_item_serializer.py` & `redturtle.prenotazioni-2.7.0/src/redturtle/prenotazioni/tests/test_prenotazione_searchable_item_serializer.py`

 * *Files identical despite different names*

### Comparing `redturtle.prenotazioni-2.6.5/src/redturtle/prenotazioni/tests/test_prenotazioni_context_state.py` & `redturtle.prenotazioni-2.7.0/src/redturtle/prenotazioni/tests/test_prenotazioni_context_state.py`

 * *Files identical despite different names*

### Comparing `redturtle.prenotazioni-2.6.5/src/redturtle/prenotazioni/tests/test_prenotazioni_folder_holidays_constraint.py` & `redturtle.prenotazioni-2.7.0/src/redturtle/prenotazioni/tests/test_prenotazioni_folder_holidays_constraint.py`

 * *Files identical despite different names*

### Comparing `redturtle.prenotazioni-2.6.5/src/redturtle/prenotazioni/tests/test_prenotazioni_search.py` & `redturtle.prenotazioni-2.7.0/src/redturtle/prenotazioni/tests/test_prenotazioni_search.py`

 * *Files identical despite different names*

### Comparing `redturtle.prenotazioni-2.6.5/src/redturtle/prenotazioni/tests/test_restapi_types_override.py` & `redturtle.prenotazioni-2.7.0/src/redturtle/prenotazioni/tests/test_vocabularies.py`

 * *Files 23% similar despite different names*

```diff
@@ -1,75 +1,76 @@
 # -*- coding: utf-8 -*-
 import unittest
 from datetime import date
 
-import transaction
 from plone import api
-from plone.app.testing import SITE_OWNER_NAME
-from plone.app.testing import SITE_OWNER_PASSWORD
 from plone.app.testing import TEST_USER_ID
 from plone.app.testing import setRoles
-from plone.restapi.testing import RelativeSession
+from zope.component import getUtility
+from zope.schema.interfaces import IVocabularyFactory
 
 from redturtle.prenotazioni.testing import REDTURTLE_PRENOTAZIONI_API_FUNCTIONAL_TESTING
 
 
-class TestTypesOverrides(unittest.TestCase):
+class TestVocabularies(unittest.TestCase):
     layer = REDTURTLE_PRENOTAZIONI_API_FUNCTIONAL_TESTING
 
     def setUp(self):
         self.app = self.layer["app"]
         self.portal = self.layer["portal"]
-        self.request = self.layer["request"]
         self.portal_url = self.portal.absolute_url()
         setRoles(self.portal, TEST_USER_ID, ["Manager"])
 
-        self.api_session = RelativeSession(self.portal_url)
-        self.api_session.headers.update({"Accept": "application/json"})
-        self.api_session.auth = (SITE_OWNER_NAME, SITE_OWNER_PASSWORD)
-
-        self.portal_url = self.portal.absolute_url()
         self.folder_prenotazioni = api.content.create(
             container=self.portal,
             type="PrenotazioniFolder",
             title="Folder",
             description="",
             daData=date.today(),
             gates=["Gate A", "Gate B"],
             same_day_booking_disallowed="no",
         )
-
-        booking_type_A = api.content.create(
+        api.content.create(
             type="PrenotazioneType",
             title="Type A",
             duration=30,
             container=self.folder_prenotazioni,
             gates=["all"],
         )
-
-        api.content.transition(
-            booking_type_A,
-            transition="publish",
+        api.content.create(
+            type="PrenotazioneType",
+            title="Type B",
+            duration=10,
+            container=self.folder_prenotazioni,
+            gates=["all"],
         )
-        api.content.transition(obj=self.folder_prenotazioni, transition="publish")
 
-        transaction.commit()
+        self.folder_prenotazioni_2 = api.content.create(
+            container=self.portal,
+            type="PrenotazioniFolder",
+            title="Folder 2",
+            description="",
+            daData=date.today(),
+            gates=["Gate c", "Gate D"],
+            same_day_booking_disallowed="no",
+        )
+        api.content.create(
+            type="PrenotazioneType",
+            title="Type C",
+            duration=30,
+            container=self.folder_prenotazioni_2,
+            gates=["all"],
+        )
 
     def tearDown(self):
-        self.api_session.close()
+        pass
 
-    def test_types_expanded_hide_prenotazioniyear(self):
-        response = self.api_session.get(
-            self.folder_prenotazioni.absolute_url(), params={"expand": "types"}
-        )
-
-        self.assertEqual(response.status_code, 200)
-        res = response.json()
-        prenotazioni_year = None
-        for x in res["@components"]["types"]:
-            if x["id"] == "PrenotazioniYear":
-                prenotazioni_year = x
-                break
-
-        self.assertIsNotNone(prenotazioni_year)
-        self.assertFalse(prenotazioni_year["immediately_addable"])
-        self.assertFalse(prenotazioni_year["addable"])
+    def test_booking_types(self):
+        factory = getUtility(
+            IVocabularyFactory, name="redturtle.prenotazioni.booking_types"
+        )
+        self.assertEqual(
+            set(factory(self.portal).by_token.keys()), {"Type A", "Type B", "Type C"}
+        )
+        self.assertEqual(
+            set(factory(self.folder_prenotazioni).by_token.keys()), {"Type A", "Type B"}
+        )
```

### Comparing `redturtle.prenotazioni-2.6.5/src/redturtle/prenotazioni/tests/test_send_ical.py` & `redturtle.prenotazioni-2.7.0/src/redturtle/prenotazioni/tests/test_send_ical.py`

 * *Files identical despite different names*

### Comparing `redturtle.prenotazioni-2.6.5/src/redturtle/prenotazioni/tests/test_setup.py` & `redturtle.prenotazioni-2.7.0/src/redturtle/prenotazioni/tests/test_setup.py`

 * *Files identical despite different names*

### Comparing `redturtle.prenotazioni-2.6.5/src/redturtle/prenotazioni/tests/test_stringinterp.py` & `redturtle.prenotazioni-2.7.0/src/redturtle/prenotazioni/tests/test_stringinterp.py`

 * *Files identical despite different names*

### Comparing `redturtle.prenotazioni-2.6.5/src/redturtle/prenotazioni/tests/test_utils.py` & `redturtle.prenotazioni-2.7.0/src/redturtle/prenotazioni/tests/test_utils.py`

 * *Files identical despite different names*

### Comparing `redturtle.prenotazioni-2.6.5/src/redturtle/prenotazioni/tests/test_vacation_api.py` & `redturtle.prenotazioni-2.7.0/src/redturtle/prenotazioni/tests/test_vacation_api.py`

 * *Files identical despite different names*

### Comparing `redturtle.prenotazioni-2.6.5/src/redturtle/prenotazioni/tests/test_validate_max_bookings_allowed.py` & `redturtle.prenotazioni-2.7.0/src/redturtle/prenotazioni/tests/test_validate_max_bookings_allowed.py`

 * *Files identical despite different names*

### Comparing `redturtle.prenotazioni-2.6.5/src/redturtle/prenotazioni/tests/test_week_table_overrides.py` & `redturtle.prenotazioni-2.7.0/src/redturtle/prenotazioni/tests/test_week_table_overrides.py`

 * *Files identical despite different names*

### Comparing `redturtle.prenotazioni-2.6.5/src/redturtle/prenotazioni/upgrades.py` & `redturtle.prenotazioni-2.7.0/src/redturtle/prenotazioni/upgrades.py`

 * *Files 2% similar despite different names*

```diff
@@ -501,7 +501,18 @@
             value = getattr(booking_folder, field, "")
 
             value and setattr(
                 booking_folder,
                 field,
                 value.replace("${booking_print_url}.", "${booking_print_url} ."),
             )
+
+
+def to_2009(context):
+    update_profile(context, "plone-difftool")
+    update_profile(context, "repositorytool")
+
+    portal_types = api.portal.get_tool(name="portal_types")
+    modulo_behaviors = [x for x in portal_types["Prenotazione"].behaviors]
+    if "plone.versioning" not in modulo_behaviors:
+        modulo_behaviors.append("plone.versioning")
+    portal_types["Prenotazione"].behaviors = tuple(modulo_behaviors)
```

### Comparing `redturtle.prenotazioni-2.6.5/src/redturtle/prenotazioni/upgrades.zcml` & `redturtle.prenotazioni-2.7.0/src/redturtle/prenotazioni/upgrades.zcml`

 * *Files 1% similar despite different names*

```diff
@@ -351,9 +351,19 @@
       destination="2008"
       >
     <genericsetup:upgradeStep
         title="Fix sms links"
         handler=".upgrades.to_2008"
         />
   </genericsetup:upgradeSteps>
+  <genericsetup:upgradeSteps
+      profile="redturtle.prenotazioni:default"
+      source="2008"
+      destination="2009"
+      >
+    <genericsetup:upgradeStep
+        title="Add versioning to Prenotazione c.t."
+        handler=".upgrades.to_2009"
+        />
+  </genericsetup:upgradeSteps>
 
 </configure>
```

### Comparing `redturtle.prenotazioni-2.6.5/src/redturtle/prenotazioni/utilities/dateutils.py` & `redturtle.prenotazioni-2.7.0/src/redturtle/prenotazioni/utilities/dateutils.py`

 * *Files identical despite different names*

### Comparing `redturtle.prenotazioni-2.6.5/src/redturtle/prenotazioni/utilities/urls.py` & `redturtle.prenotazioni-2.7.0/src/redturtle/prenotazioni/utilities/urls.py`

 * *Files identical despite different names*

### Comparing `redturtle.prenotazioni-2.6.5/src/redturtle/prenotazioni/utils/get_prenotazioni_folder.py` & `redturtle.prenotazioni-2.7.0/src/redturtle/prenotazioni/utils/get_prenotazioni_folder.py`

 * *Files identical despite different names*

### Comparing `redturtle.prenotazioni-2.6.5/src/redturtle/prenotazioni/vocabularies/configure.zcml` & `redturtle.prenotazioni-2.7.0/src/redturtle/prenotazioni/vocabularies/configure.zcml`

 * *Files identical despite different names*

### Comparing `redturtle.prenotazioni-2.6.5/src/redturtle/prenotazioni/vocabularies/gates.py` & `redturtle.prenotazioni-2.7.0/src/redturtle/prenotazioni/vocabularies/gates.py`

 * *Files identical despite different names*

### Comparing `redturtle.prenotazioni-2.6.5/src/redturtle/prenotazioni/vocabularies/requirable_booking_fields.py` & `redturtle.prenotazioni-2.7.0/src/redturtle/prenotazioni/vocabularies/requirable_booking_fields.py`

 * *Files identical despite different names*

### Comparing `redturtle.prenotazioni-2.6.5/src/redturtle/prenotazioni/vocabularies/review_states.py` & `redturtle.prenotazioni-2.7.0/src/redturtle/prenotazioni/vocabularies/review_states.py`

 * *Files identical despite different names*

### Comparing `redturtle.prenotazioni-2.6.5/src/redturtle/prenotazioni/vocabularies/tipologies.py` & `redturtle.prenotazioni-2.7.0/src/redturtle/prenotazioni/vocabularies/tipologies.py`

 * *Files identical despite different names*

### Comparing `redturtle.prenotazioni-2.6.5/src/redturtle/prenotazioni/vocabularies/voc_booking_type_gates.py` & `redturtle.prenotazioni-2.7.0/src/redturtle/prenotazioni/vocabularies/voc_booking_type_gates.py`

 * *Files identical despite different names*

### Comparing `redturtle.prenotazioni-2.6.5/src/redturtle/prenotazioni/vocabularies/voc_durata_incontro.py` & `redturtle.prenotazioni-2.7.0/src/redturtle/prenotazioni/vocabularies/voc_durata_incontro.py`

 * *Files identical despite different names*

### Comparing `redturtle.prenotazioni-2.6.5/src/redturtle/prenotazioni/vocabularies/voc_months.py` & `redturtle.prenotazioni-2.7.0/src/redturtle/prenotazioni/vocabularies/voc_months.py`

 * *Files identical despite different names*

### Comparing `redturtle.prenotazioni-2.6.5/src/redturtle/prenotazioni/vocabularies/voc_ore_inizio.py` & `redturtle.prenotazioni-2.7.0/src/redturtle/prenotazioni/vocabularies/voc_ore_inizio.py`

 * *Files identical despite different names*

### Comparing `redturtle.prenotazioni-2.6.5/src/redturtle.prenotazioni.egg-info/SOURCES.txt` & `redturtle.prenotazioni-2.7.0/src/redturtle.prenotazioni.egg-info/SOURCES.txt`

 * *Files 0% similar despite different names*

```diff
@@ -182,15 +182,17 @@
 src/redturtle/prenotazioni/locales/it/LC_MESSAGES/redturtle.prenotazioni.po
 src/redturtle/prenotazioni/monkeypatcher/__init__.py
 src/redturtle/prenotazioni/monkeypatcher/configure.zcml
 src/redturtle/prenotazioni/profiles/default/actions.xml
 src/redturtle/prenotazioni/profiles/default/browserlayer.xml
 src/redturtle/prenotazioni/profiles/default/catalog.xml
 src/redturtle/prenotazioni/profiles/default/contentrules.xml
+src/redturtle/prenotazioni/profiles/default/diff_tool.xml
 src/redturtle/prenotazioni/profiles/default/metadata.xml
+src/redturtle/prenotazioni/profiles/default/repositorytool.xml
 src/redturtle/prenotazioni/profiles/default/rolemap.xml
 src/redturtle/prenotazioni/profiles/default/sharing.xml
 src/redturtle/prenotazioni/profiles/default/types.xml
 src/redturtle/prenotazioni/profiles/default/workflows.xml
 src/redturtle/prenotazioni/profiles/default/registry/caching.xml
 src/redturtle/prenotazioni/profiles/default/registry/resources.xml
 src/redturtle/prenotazioni/profiles/default/registry/settings.xml
@@ -264,14 +266,15 @@
 src/redturtle/prenotazioni/tests/test_content_validators_validate_pause_table.py
 src/redturtle/prenotazioni/tests/test_day.py
 src/redturtle/prenotazioni/tests/test_delete_booking.py
 src/redturtle/prenotazioni/tests/test_delete_booking_api.py
 src/redturtle/prenotazioni/tests/test_gates_overrides.py
 src/redturtle/prenotazioni/tests/test_move_booking_api.py
 src/redturtle/prenotazioni/tests/test_notification_supervisor_utility.py
+src/redturtle/prenotazioni/tests/test_notify_the_message_failure.py
 src/redturtle/prenotazioni/tests/test_pauses_overrides.py
 src/redturtle/prenotazioni/tests/test_prenotazione_email_sent_to_managers.py
 src/redturtle/prenotazioni/tests/test_prenotazione_events.py
 src/redturtle/prenotazioni/tests/test_prenotazione_searchable_item_serializer.py
 src/redturtle/prenotazioni/tests/test_prenotazioni_context_state.py
 src/redturtle/prenotazioni/tests/test_prenotazioni_folder_holidays_constraint.py
 src/redturtle/prenotazioni/tests/test_prenotazioni_search.py
```

