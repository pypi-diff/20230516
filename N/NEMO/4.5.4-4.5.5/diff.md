# Comparing `tmp/NEMO-4.5.4.tar.gz` & `tmp/NEMO-4.5.5.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "NEMO-4.5.4.tar", last modified: Fri Apr 21 23:04:43 2023, max compression
+gzip compressed data, was "NEMO-4.5.5.tar", last modified: Tue May 16 14:04:38 2023, max compression
```

## Comparing `NEMO-4.5.4.tar` & `NEMO-4.5.5.tar`

### file list

```diff
@@ -1,481 +1,482 @@
-drwxr-xr-x   0 root         (0) root         (0)        0 2023-04-21 23:04:43.449914 NEMO-4.5.4/
--rw-rw-rw-   0 root         (0) root         (0)     1644 2023-04-11 20:18:49.000000 NEMO-4.5.4/LICENSE.md
--rw-rw-rw-   0 root         (0) root         (0)      131 2023-04-11 20:18:49.000000 NEMO-4.5.4/MANIFEST.in
-drwxr-xr-x   0 root         (0) root         (0)        0 2023-04-21 23:04:43.387914 NEMO-4.5.4/NEMO/
--rw-rw-rw-   0 root         (0) root         (0)     1254 2023-04-11 20:18:49.000000 NEMO-4.5.4/NEMO/__init__.py
--rw-rw-rw-   0 root         (0) root         (0)     4594 2023-04-11 20:18:49.000000 NEMO-4.5.4/NEMO/actions.py
--rw-rw-rw-   0 root         (0) root         (0)    48729 2023-04-13 18:53:48.000000 NEMO-4.5.4/NEMO/admin.py
-drwxr-xr-x   0 root         (0) root         (0)        0 2023-04-21 23:04:43.388914 NEMO-4.5.4/NEMO/apps/
--rw-rw-rw-   0 root         (0) root         (0)        0 2023-04-21 23:04:29.000000 NEMO-4.5.4/NEMO/apps/__init__.py
-drwxr-xr-x   0 root         (0) root         (0)        0 2023-04-21 23:04:43.388914 NEMO-4.5.4/NEMO/apps/area_access/
--rw-rw-rw-   0 root         (0) root         (0)        0 2023-04-21 23:04:29.000000 NEMO-4.5.4/NEMO/apps/area_access/__init__.py
-drwxr-xr-x   0 root         (0) root         (0)        0 2023-04-21 23:04:43.375914 NEMO-4.5.4/NEMO/apps/area_access/static/
-drwxr-xr-x   0 root         (0) root         (0)        0 2023-04-21 23:04:43.388914 NEMO-4.5.4/NEMO/apps/area_access/static/area_access/
--rw-rw-rw-   0 root         (0) root         (0)      304 2023-04-11 20:18:49.000000 NEMO-4.5.4/NEMO/apps/area_access/static/area_access/area_access.css
-drwxr-xr-x   0 root         (0) root         (0)        0 2023-04-21 23:04:43.376914 NEMO-4.5.4/NEMO/apps/area_access/templates/
-drwxr-xr-x   0 root         (0) root         (0)        0 2023-04-21 23:04:43.391914 NEMO-4.5.4/NEMO/apps/area_access/templates/area_access/
--rw-rw-rw-   0 root         (0) root         (0)     1531 2023-04-11 20:18:49.000000 NEMO-4.5.4/NEMO/apps/area_access/templates/area_access/already_logged_in.html
--rw-rw-rw-   0 root         (0) root         (0)      349 2023-04-11 20:18:49.000000 NEMO-4.5.4/NEMO/apps/area_access/templates/area_access/badge_not_found.html
--rw-rw-rw-   0 root         (0) root         (0)     9067 2023-04-11 20:18:49.000000 NEMO-4.5.4/NEMO/apps/area_access/templates/area_access/base.html
--rw-rw-rw-   0 root         (0) root         (0)      664 2023-04-11 20:18:49.000000 NEMO-4.5.4/NEMO/apps/area_access/templates/area_access/choose_project.html
--rw-rw-rw-   0 root         (0) root         (0)       54 2023-04-11 20:18:49.000000 NEMO-4.5.4/NEMO/apps/area_access/templates/area_access/door_is_open.html
--rw-rw-rw-   0 root         (0) root         (0)      236 2023-04-11 20:18:49.000000 NEMO-4.5.4/NEMO/apps/area_access/templates/area_access/farewell_screen.html
--rw-rw-rw-   0 root         (0) root         (0)      143 2023-04-11 20:18:49.000000 NEMO-4.5.4/NEMO/apps/area_access/templates/area_access/inactive.html
--rw-rw-rw-   0 root         (0) root         (0)      363 2023-04-11 20:18:49.000000 NEMO-4.5.4/NEMO/apps/area_access/templates/area_access/login_success.html
--rw-rw-rw-   0 root         (0) root         (0)      244 2023-04-11 20:18:49.000000 NEMO-4.5.4/NEMO/apps/area_access/templates/area_access/logout_success.html
--rw-rw-rw-   0 root         (0) root         (0)      666 2023-04-11 20:18:49.000000 NEMO-4.5.4/NEMO/apps/area_access/templates/area_access/logout_warning.html
--rw-rw-rw-   0 root         (0) root         (0)      239 2023-04-11 20:18:49.000000 NEMO-4.5.4/NEMO/apps/area_access/templates/area_access/no_active_projects.html
--rw-rw-rw-   0 root         (0) root         (0)      338 2023-04-11 20:18:49.000000 NEMO-4.5.4/NEMO/apps/area_access/templates/area_access/not_logged_in.html
--rw-rw-rw-   0 root         (0) root         (0)      210 2023-04-11 20:18:49.000000 NEMO-4.5.4/NEMO/apps/area_access/templates/area_access/physical_access_denied.html
--rw-rw-rw-   0 root         (0) root         (0)      566 2023-04-11 20:18:49.000000 NEMO-4.5.4/NEMO/apps/area_access/templates/area_access/resource_unavailable.html
--rw-rw-rw-   0 root         (0) root         (0)      224 2023-04-11 20:18:49.000000 NEMO-4.5.4/NEMO/apps/area_access/templates/area_access/welcome_screen.html
--rw-rw-rw-   0 root         (0) root         (0)      629 2023-04-11 20:18:49.000000 NEMO-4.5.4/NEMO/apps/area_access/urls.py
--rw-rw-rw-   0 root         (0) root         (0)    12271 2023-04-11 20:18:49.000000 NEMO-4.5.4/NEMO/apps/area_access/views.py
-drwxr-xr-x   0 root         (0) root         (0)        0 2023-04-21 23:04:43.391914 NEMO-4.5.4/NEMO/apps/kiosk/
--rw-rw-rw-   0 root         (0) root         (0)        0 2023-04-21 23:04:29.000000 NEMO-4.5.4/NEMO/apps/kiosk/__init__.py
-drwxr-xr-x   0 root         (0) root         (0)        0 2023-04-21 23:04:43.376914 NEMO-4.5.4/NEMO/apps/kiosk/static/
-drwxr-xr-x   0 root         (0) root         (0)        0 2023-04-21 23:04:43.391914 NEMO-4.5.4/NEMO/apps/kiosk/static/kiosk/
--rw-rw-rw-   0 root         (0) root         (0)      116 2023-04-11 20:18:49.000000 NEMO-4.5.4/NEMO/apps/kiosk/static/kiosk/kiosk.css
-drwxr-xr-x   0 root         (0) root         (0)        0 2023-04-21 23:04:43.376914 NEMO-4.5.4/NEMO/apps/kiosk/templates/
-drwxr-xr-x   0 root         (0) root         (0)        0 2023-04-21 23:04:43.393914 NEMO-4.5.4/NEMO/apps/kiosk/templates/kiosk/
--rw-rw-rw-   0 root         (0) root         (0)      170 2023-04-11 20:18:49.000000 NEMO-4.5.4/NEMO/apps/kiosk/templates/kiosk/acknowledgement.html
--rw-rw-rw-   0 root         (0) root         (0)     2125 2023-04-11 20:18:49.000000 NEMO-4.5.4/NEMO/apps/kiosk/templates/kiosk/category_choices.html
--rw-rw-rw-   0 root         (0) root         (0)     2012 2023-04-11 20:18:49.000000 NEMO-4.5.4/NEMO/apps/kiosk/templates/kiosk/choices.html
--rw-rw-rw-   0 root         (0) root         (0)     1072 2023-04-11 20:18:49.000000 NEMO-4.5.4/NEMO/apps/kiosk/templates/kiosk/error.html
--rw-rw-rw-   0 root         (0) root         (0)     2923 2023-04-11 20:18:49.000000 NEMO-4.5.4/NEMO/apps/kiosk/templates/kiosk/individual_reservation.html
--rw-rw-rw-   0 root         (0) root         (0)    12184 2023-04-11 20:18:49.000000 NEMO-4.5.4/NEMO/apps/kiosk/templates/kiosk/kiosk.html
--rw-rw-rw-   0 root         (0) root         (0)      240 2023-04-11 20:18:49.000000 NEMO-4.5.4/NEMO/apps/kiosk/templates/kiosk/location_directory.html
--rw-rw-rw-   0 root         (0) root         (0)      901 2023-04-11 20:18:49.000000 NEMO-4.5.4/NEMO/apps/kiosk/templates/kiosk/success.html
--rw-rw-rw-   0 root         (0) root         (0)    16575 2023-04-11 20:18:49.000000 NEMO-4.5.4/NEMO/apps/kiosk/templates/kiosk/tool_information.html
--rw-rw-rw-   0 root         (0) root         (0)     1108 2023-04-11 20:18:49.000000 NEMO-4.5.4/NEMO/apps/kiosk/templates/kiosk/tool_project_selection_snippet.html
--rw-rw-rw-   0 root         (0) root         (0)     4472 2023-04-11 20:18:49.000000 NEMO-4.5.4/NEMO/apps/kiosk/templates/kiosk/tool_reservation.html
--rw-rw-rw-   0 root         (0) root         (0)     1198 2023-04-11 20:18:49.000000 NEMO-4.5.4/NEMO/apps/kiosk/urls.py
--rw-rw-rw-   0 root         (0) root         (0)    13550 2023-04-11 20:18:49.000000 NEMO-4.5.4/NEMO/apps/kiosk/views.py
-drwxr-xr-x   0 root         (0) root         (0)        0 2023-04-21 23:04:43.394914 NEMO-4.5.4/NEMO/apps/sensors/
--rw-rw-rw-   0 root         (0) root         (0)        0 2023-04-21 23:04:29.000000 NEMO-4.5.4/NEMO/apps/sensors/__init__.py
--rw-rw-rw-   0 root         (0) root         (0)     6966 2023-04-11 20:18:49.000000 NEMO-4.5.4/NEMO/apps/sensors/admin.py
--rw-rw-rw-   0 root         (0) root         (0)      539 2023-04-11 20:18:49.000000 NEMO-4.5.4/NEMO/apps/sensors/customizations.py
--rw-rw-rw-   0 root         (0) root         (0)     5237 2023-04-11 20:18:49.000000 NEMO-4.5.4/NEMO/apps/sensors/evaluators.py
-drwxr-xr-x   0 root         (0) root         (0)        0 2023-04-21 23:04:43.394914 NEMO-4.5.4/NEMO/apps/sensors/management/
--rw-rw-rw-   0 root         (0) root         (0)        0 2023-04-21 23:04:29.000000 NEMO-4.5.4/NEMO/apps/sensors/management/__init__.py
-drwxr-xr-x   0 root         (0) root         (0)        0 2023-04-21 23:04:43.395914 NEMO-4.5.4/NEMO/apps/sensors/management/commands/
--rw-rw-rw-   0 root         (0) root         (0)        0 2023-04-21 23:04:29.000000 NEMO-4.5.4/NEMO/apps/sensors/management/commands/__init__.py
--rw-rw-rw-   0 root         (0) root         (0)      278 2023-04-11 20:18:49.000000 NEMO-4.5.4/NEMO/apps/sensors/management/commands/manage_sensor_data.py
-drwxr-xr-x   0 root         (0) root         (0)        0 2023-04-21 23:04:43.395914 NEMO-4.5.4/NEMO/apps/sensors/migrations/
--rw-rw-rw-   0 root         (0) root         (0)     7794 2023-04-11 20:18:49.000000 NEMO-4.5.4/NEMO/apps/sensors/migrations/0001_initial.py
--rw-rw-rw-   0 root         (0) root         (0)        0 2023-04-21 23:04:29.000000 NEMO-4.5.4/NEMO/apps/sensors/migrations/__init__.py
--rw-rw-rw-   0 root         (0) root         (0)    12955 2023-04-11 20:18:49.000000 NEMO-4.5.4/NEMO/apps/sensors/models.py
--rw-rw-rw-   0 root         (0) root         (0)     4564 2023-04-11 20:18:49.000000 NEMO-4.5.4/NEMO/apps/sensors/sensors.py
-drwxr-xr-x   0 root         (0) root         (0)        0 2023-04-21 23:04:43.376914 NEMO-4.5.4/NEMO/apps/sensors/static/
-drwxr-xr-x   0 root         (0) root         (0)        0 2023-04-21 23:04:43.397914 NEMO-4.5.4/NEMO/apps/sensors/static/sensors/
--rw-rw-rw-   0 root         (0) root         (0)   408236 2023-04-11 20:18:49.000000 NEMO-4.5.4/NEMO/apps/sensors/static/sensors/chart.js
--rw-rw-rw-   0 root         (0) root         (0)   195090 2023-04-11 20:18:49.000000 NEMO-4.5.4/NEMO/apps/sensors/static/sensors/chart.min.js
--rw-rw-rw-   0 root         (0) root         (0)     1376 2023-04-11 20:18:49.000000 NEMO-4.5.4/NEMO/apps/sensors/static/sensors/chartjs-adapter-moment.js
--rw-rw-rw-   0 root         (0) root         (0)     7659 2023-04-11 20:18:49.000000 NEMO-4.5.4/NEMO/apps/sensors/static/sensors/daterangepicker.css
--rw-rw-rw-   0 root         (0) root         (0)    66305 2023-04-11 20:18:49.000000 NEMO-4.5.4/NEMO/apps/sensors/static/sensors/daterangepicker.js
--rw-rw-rw-   0 root         (0) root         (0)      608 2023-04-11 20:18:49.000000 NEMO-4.5.4/NEMO/apps/sensors/static/sensors/sensors.css
-drwxr-xr-x   0 root         (0) root         (0)        0 2023-04-21 23:04:43.376914 NEMO-4.5.4/NEMO/apps/sensors/templates/
-drwxr-xr-x   0 root         (0) root         (0)        0 2023-04-21 23:04:43.397914 NEMO-4.5.4/NEMO/apps/sensors/templates/customizations/
--rw-rw-rw-   0 root         (0) root         (0)     3701 2023-04-11 20:18:49.000000 NEMO-4.5.4/NEMO/apps/sensors/templates/customizations/customizations_sensors.html
-drwxr-xr-x   0 root         (0) root         (0)        0 2023-04-21 23:04:43.397914 NEMO-4.5.4/NEMO/apps/sensors/templates/sensors/
--rw-rw-rw-   0 root         (0) root         (0)      347 2023-04-11 20:18:49.000000 NEMO-4.5.4/NEMO/apps/sensors/templates/sensors/sensor_alerts.html
--rw-rw-rw-   0 root         (0) root         (0)    15165 2023-04-11 20:18:49.000000 NEMO-4.5.4/NEMO/apps/sensors/templates/sensors/sensor_data.html
--rw-rw-rw-   0 root         (0) root         (0)     2615 2023-04-11 20:18:49.000000 NEMO-4.5.4/NEMO/apps/sensors/templates/sensors/sensors.html
--rw-rw-rw-   0 root         (0) root         (0)      790 2023-04-11 20:18:49.000000 NEMO-4.5.4/NEMO/apps/sensors/urls.py
--rw-rw-rw-   0 root         (0) root         (0)     5069 2023-04-11 20:18:49.000000 NEMO-4.5.4/NEMO/apps/sensors/views.py
--rw-rw-rw-   0 root         (0) root         (0)     3966 2023-04-11 20:18:49.000000 NEMO-4.5.4/NEMO/context_processors.py
--rw-rw-rw-   0 root         (0) root         (0)     5778 2023-04-11 20:18:49.000000 NEMO-4.5.4/NEMO/decorators.py
--rw-rw-rw-   0 root         (0) root         (0)     4513 2023-04-11 20:18:49.000000 NEMO-4.5.4/NEMO/exceptions.py
--rw-rw-rw-   0 root         (0) root         (0)     3833 2023-04-11 20:18:49.000000 NEMO-4.5.4/NEMO/fields.py
--rw-rw-rw-   0 root         (0) root         (0)    12935 2023-04-11 20:18:49.000000 NEMO-4.5.4/NEMO/forms.py
--rw-rw-rw-   0 root         (0) root         (0)    17784 2023-04-13 18:53:48.000000 NEMO-4.5.4/NEMO/interlocks.py
-drwxr-xr-x   0 root         (0) root         (0)        0 2023-04-21 23:04:43.397914 NEMO-4.5.4/NEMO/management/
--rw-rw-rw-   0 root         (0) root         (0)        0 2023-04-21 23:04:29.000000 NEMO-4.5.4/NEMO/management/__init__.py
-drwxr-xr-x   0 root         (0) root         (0)        0 2023-04-21 23:04:43.400914 NEMO-4.5.4/NEMO/management/commands/
--rw-rw-rw-   0 root         (0) root         (0)        0 2023-04-21 23:04:29.000000 NEMO-4.5.4/NEMO/management/commands/__init__.py
--rw-rw-rw-   0 root         (0) root         (0)      385 2023-04-11 20:18:49.000000 NEMO-4.5.4/NEMO/management/commands/cancel_unused_reservations.py
--rw-rw-rw-   0 root         (0) root         (0)      382 2023-04-11 20:18:49.000000 NEMO-4.5.4/NEMO/management/commands/create_closure_alerts.py
--rw-rw-rw-   0 root         (0) root         (0)      376 2023-04-11 20:18:49.000000 NEMO-4.5.4/NEMO/management/commands/manage_recurring_charges.py
--rw-rw-rw-   0 root         (0) root         (0)      431 2023-04-11 20:18:49.000000 NEMO-4.5.4/NEMO/management/commands/manage_tool_qualifications.py
--rw-rw-rw-   0 root         (0) root         (0)      417 2023-04-11 20:18:49.000000 NEMO-4.5.4/NEMO/management/commands/send_email_out_of_time_reservation_notification.py
--rw-rw-rw-   0 root         (0) root         (0)      415 2023-04-11 20:18:49.000000 NEMO-4.5.4/NEMO/management/commands/send_email_reservation_ending_reminders.py
--rw-rw-rw-   0 root         (0) root         (0)      408 2023-04-11 20:18:49.000000 NEMO-4.5.4/NEMO/management/commands/send_email_reservation_reminders.py
--rw-rw-rw-   0 root         (0) root         (0)      554 2023-04-11 20:18:49.000000 NEMO-4.5.4/NEMO/management/commands/send_email_usage_reminders.py
--rw-rw-rw-   0 root         (0) root         (0)      456 2023-04-11 20:18:49.000000 NEMO-4.5.4/NEMO/management/commands/send_email_user_access_expiration_reminders.py
--rw-rw-rw-   0 root         (0) root         (0)      406 2023-04-11 20:18:49.000000 NEMO-4.5.4/NEMO/management/commands/send_email_weekend_access_notification.py
--rw-rw-rw-   0 root         (0) root         (0)     5578 2023-04-11 20:18:49.000000 NEMO-4.5.4/NEMO/middleware.py
-drwxr-xr-x   0 root         (0) root         (0)        0 2023-04-21 23:04:43.404914 NEMO-4.5.4/NEMO/migrations/
--rw-rw-rw-   0 root         (0) root         (0)    50307 2023-04-11 20:18:49.000000 NEMO-4.5.4/NEMO/migrations/0001_version_1_0_0.py
--rw-rw-rw-   0 root         (0) root         (0)    32962 2023-04-11 20:18:49.000000 NEMO-4.5.4/NEMO/migrations/0002_version_1_0_0_squashed.py
--rw-rw-rw-   0 root         (0) root         (0)     7988 2023-04-11 20:18:49.000000 NEMO-4.5.4/NEMO/migrations/0012_version_2_0_0_squashed.py
--rw-rw-rw-   0 root         (0) root         (0)     9904 2023-04-11 20:18:49.000000 NEMO-4.5.4/NEMO/migrations/0020_version_3_0_0.py
--rw-rw-rw-   0 root         (0) root         (0)     1712 2023-04-11 20:18:49.000000 NEMO-4.5.4/NEMO/migrations/0021_version_3_1_0.py
--rw-rw-rw-   0 root         (0) root         (0)     1095 2023-04-11 20:18:49.000000 NEMO-4.5.4/NEMO/migrations/0022_version_3_3_0.py
--rw-rw-rw-   0 root         (0) root         (0)      913 2023-04-11 20:18:49.000000 NEMO-4.5.4/NEMO/migrations/0023_badgereader.py
--rw-rw-rw-   0 root         (0) root         (0)      705 2023-04-11 20:18:49.000000 NEMO-4.5.4/NEMO/migrations/0024_contactinformation_user.py
--rw-rw-rw-   0 root         (0) root         (0)     2674 2023-04-11 20:18:49.000000 NEMO-4.5.4/NEMO/migrations/0025_version_3_6_0.py
--rw-rw-rw-   0 root         (0) root         (0)     5405 2023-04-11 20:18:49.000000 NEMO-4.5.4/NEMO/migrations/0026_version_3_7_0.py
--rw-rw-rw-   0 root         (0) root         (0)      420 2023-04-11 20:18:49.000000 NEMO-4.5.4/NEMO/migrations/0027_version_3_8_0.py
--rw-rw-rw-   0 root         (0) root         (0)     2233 2023-04-11 20:18:49.000000 NEMO-4.5.4/NEMO/migrations/0028_version_3_9_0.py
--rw-rw-rw-   0 root         (0) root         (0)     1127 2023-04-11 20:18:49.000000 NEMO-4.5.4/NEMO/migrations/0030_version_3_9_2.py
--rw-rw-rw-   0 root         (0) root         (0)     2785 2023-04-11 20:18:49.000000 NEMO-4.5.4/NEMO/migrations/0031_version_3_10_0.py
--rw-rw-rw-   0 root         (0) root         (0)     3166 2023-04-11 20:18:49.000000 NEMO-4.5.4/NEMO/migrations/0032_version_3_11_0.py
--rw-rw-rw-   0 root         (0) root         (0)      380 2023-04-11 20:18:49.000000 NEMO-4.5.4/NEMO/migrations/0033_version_3_12_0.py
--rw-rw-rw-   0 root         (0) root         (0)      372 2023-04-11 20:18:49.000000 NEMO-4.5.4/NEMO/migrations/0034_version_3_13_0.py
--rw-rw-rw-   0 root         (0) root         (0)     6747 2023-04-11 20:18:49.000000 NEMO-4.5.4/NEMO/migrations/0035_version_3_14_0.py
--rw-rw-rw-   0 root         (0) root         (0)     7792 2023-04-11 20:18:49.000000 NEMO-4.5.4/NEMO/migrations/0036_version_3_15_0.py
--rw-rw-rw-   0 root         (0) root         (0)     3717 2023-04-11 20:18:49.000000 NEMO-4.5.4/NEMO/migrations/0037_version_3_16_0.py
--rw-rw-rw-   0 root         (0) root         (0)      935 2023-04-11 20:18:49.000000 NEMO-4.5.4/NEMO/migrations/0038_version_4_0_0.py
--rw-rw-rw-   0 root         (0) root         (0)     3601 2023-04-11 20:18:49.000000 NEMO-4.5.4/NEMO/migrations/0039_version_4_1_0.py
--rw-rw-rw-   0 root         (0) root         (0)     2444 2023-04-11 20:18:49.000000 NEMO-4.5.4/NEMO/migrations/0040_version_4_2_0.py
--rw-rw-rw-   0 root         (0) root         (0)      487 2023-04-11 20:18:49.000000 NEMO-4.5.4/NEMO/migrations/0041_version_4_2_1.py
--rw-rw-rw-   0 root         (0) root         (0)    16454 2023-04-11 20:18:49.000000 NEMO-4.5.4/NEMO/migrations/0042_version_4_3_0.py
--rw-rw-rw-   0 root         (0) root         (0)      524 2023-04-11 20:18:49.000000 NEMO-4.5.4/NEMO/migrations/0043_version_4_3_2.py
--rw-rw-rw-   0 root         (0) root         (0)     5420 2023-04-11 20:18:49.000000 NEMO-4.5.4/NEMO/migrations/0044_version_4_4_0.py
--rw-rw-rw-   0 root         (0) root         (0)    13447 2023-04-11 22:02:40.000000 NEMO-4.5.4/NEMO/migrations/0045_version_4_5_0.py
--rw-rw-rw-   0 root         (0) root         (0)        0 2023-04-21 23:04:29.000000 NEMO-4.5.4/NEMO/migrations/__init__.py
--rw-rw-rw-   0 root         (0) root         (0)     2304 2023-04-11 20:18:49.000000 NEMO-4.5.4/NEMO/migrations_utils.py
--rw-rw-rw-   0 root         (0) root         (0)     5874 2023-04-11 20:18:49.000000 NEMO-4.5.4/NEMO/mixins.py
--rw-rw-rw-   0 root         (0) root         (0)     3855 2023-04-11 20:18:49.000000 NEMO-4.5.4/NEMO/model_tree.py
--rw-rw-rw-   0 root         (0) root         (0)   151437 2023-04-11 20:18:49.000000 NEMO-4.5.4/NEMO/models.py
--rw-rw-rw-   0 root         (0) root         (0)     1076 2023-04-11 20:18:49.000000 NEMO-4.5.4/NEMO/parsers.py
--rw-rw-rw-   0 root         (0) root         (0)      870 2023-04-11 20:18:49.000000 NEMO-4.5.4/NEMO/permissions.py
--rw-rw-rw-   0 root         (0) root         (0)    49395 2023-04-11 20:18:49.000000 NEMO-4.5.4/NEMO/policy.py
--rw-rw-rw-   0 root         (0) root         (0)     9943 2023-04-11 20:18:49.000000 NEMO-4.5.4/NEMO/provisioning.py
--rw-rw-rw-   0 root         (0) root         (0)     5646 2023-04-11 20:18:49.000000 NEMO-4.5.4/NEMO/rates.py
--rw-rw-rw-   0 root         (0) root         (0)     1037 2023-04-11 20:18:49.000000 NEMO-4.5.4/NEMO/rest_filter_backend.py
--rw-rw-rw-   0 root         (0) root         (0)     9310 2023-04-11 20:18:49.000000 NEMO-4.5.4/NEMO/serializers.py
-drwxr-xr-x   0 root         (0) root         (0)        0 2023-04-21 23:04:43.409914 NEMO-4.5.4/NEMO/static/
-drwxr-xr-x   0 root         (0) root         (0)        0 2023-04-21 23:04:43.409914 NEMO-4.5.4/NEMO/static/admin/
-drwxr-xr-x   0 root         (0) root         (0)        0 2023-04-21 23:04:43.409914 NEMO-4.5.4/NEMO/static/admin/physical_access_level/
--rw-rw-rw-   0 root         (0) root         (0)      607 2023-04-11 20:18:49.000000 NEMO-4.5.4/NEMO/static/admin/physical_access_level/access_level.js
-drwxr-xr-x   0 root         (0) root         (0)        0 2023-04-21 23:04:43.409914 NEMO-4.5.4/NEMO/static/admin/questions_preview/
--rw-rw-rw-   0 root         (0) root         (0)     4122 2023-04-11 20:18:49.000000 NEMO-4.5.4/NEMO/static/admin/questions_preview/questions_preview.css
--rw-rw-rw-   0 root         (0) root         (0)     1372 2023-04-11 20:18:49.000000 NEMO-4.5.4/NEMO/static/admin/questions_preview/questions_preview.js
-drwxr-xr-x   0 root         (0) root         (0)        0 2023-04-21 23:04:43.410914 NEMO-4.5.4/NEMO/static/admin/reservation_questions/
--rw-rw-rw-   0 root         (0) root         (0)      247 2023-04-11 20:18:49.000000 NEMO-4.5.4/NEMO/static/admin/reservation_questions/reservation_questions.js
--rw-rw-rw-   0 root         (0) root         (0)     1225 2023-04-11 20:18:49.000000 NEMO-4.5.4/NEMO/static/admin/time_options_override.js
-drwxr-xr-x   0 root         (0) root         (0)        0 2023-04-21 23:04:43.410914 NEMO-4.5.4/NEMO/static/admin/tool/
--rw-rw-rw-   0 root         (0) root         (0)     1437 2023-04-11 20:18:49.000000 NEMO-4.5.4/NEMO/static/admin/tool/tool.js
--rw-rw-rw-   0 root         (0) root         (0)     1278 2023-04-11 20:18:49.000000 NEMO-4.5.4/NEMO/static/badge_reader.js
-drwxr-xr-x   0 root         (0) root         (0)        0 2023-04-21 23:04:43.377914 NEMO-4.5.4/NEMO/static/bootstrap/
-drwxr-xr-x   0 root         (0) root         (0)        0 2023-04-21 23:04:43.411914 NEMO-4.5.4/NEMO/static/bootstrap/css/
--rw-rw-rw-   0 root         (0) root         (0)    22608 2023-04-11 20:18:49.000000 NEMO-4.5.4/NEMO/static/bootstrap/css/bootstrap-theme.css
--rw-rw-rw-   0 root         (0) root         (0)    43339 2023-04-11 20:18:49.000000 NEMO-4.5.4/NEMO/static/bootstrap/css/bootstrap-theme.css.map
--rw-rw-rw-   0 root         (0) root         (0)    19963 2023-04-11 20:18:49.000000 NEMO-4.5.4/NEMO/static/bootstrap/css/bootstrap-theme.min.css
--rw-rw-rw-   0 root         (0) root         (0)   141622 2023-04-11 20:18:49.000000 NEMO-4.5.4/NEMO/static/bootstrap/css/bootstrap.css
--rw-rw-rw-   0 root         (0) root         (0)   380986 2023-04-11 20:18:49.000000 NEMO-4.5.4/NEMO/static/bootstrap/css/bootstrap.css.map
--rw-rw-rw-   0 root         (0) root         (0)   117305 2023-04-11 20:18:49.000000 NEMO-4.5.4/NEMO/static/bootstrap/css/bootstrap.min.css
-drwxr-xr-x   0 root         (0) root         (0)        0 2023-04-21 23:04:43.413914 NEMO-4.5.4/NEMO/static/bootstrap/fonts/
--rw-rw-rw-   0 root         (0) root         (0)    20127 2023-04-11 20:18:49.000000 NEMO-4.5.4/NEMO/static/bootstrap/fonts/glyphicons-halflings-regular.eot
--rw-rw-rw-   0 root         (0) root         (0)   108738 2023-04-11 20:18:49.000000 NEMO-4.5.4/NEMO/static/bootstrap/fonts/glyphicons-halflings-regular.svg
--rw-rw-rw-   0 root         (0) root         (0)    45404 2023-04-11 20:18:49.000000 NEMO-4.5.4/NEMO/static/bootstrap/fonts/glyphicons-halflings-regular.ttf
--rw-rw-rw-   0 root         (0) root         (0)    23424 2023-04-11 20:18:49.000000 NEMO-4.5.4/NEMO/static/bootstrap/fonts/glyphicons-halflings-regular.woff
--rw-rw-rw-   0 root         (0) root         (0)    18028 2023-04-11 20:18:49.000000 NEMO-4.5.4/NEMO/static/bootstrap/fonts/glyphicons-halflings-regular.woff2
-drwxr-xr-x   0 root         (0) root         (0)        0 2023-04-21 23:04:43.413914 NEMO-4.5.4/NEMO/static/bootstrap/js/
--rw-rw-rw-   0 root         (0) root         (0)    67546 2023-04-11 20:18:49.000000 NEMO-4.5.4/NEMO/static/bootstrap/js/bootstrap.js
--rw-rw-rw-   0 root         (0) root         (0)    35951 2023-04-11 20:18:49.000000 NEMO-4.5.4/NEMO/static/bootstrap/js/bootstrap.min.js
-drwxr-xr-x   0 root         (0) root         (0)        0 2023-04-21 23:04:43.414914 NEMO-4.5.4/NEMO/static/datetimepicker/
--rw-rw-rw-   0 root         (0) root         (0)     9020 2023-04-11 20:18:49.000000 NEMO-4.5.4/NEMO/static/datetimepicker/bootstrap-datetimepicker.css
--rw-rw-rw-   0 root         (0) root         (0)   105978 2023-04-11 20:18:49.000000 NEMO-4.5.4/NEMO/static/datetimepicker/bootstrap-datetimepicker.js
--rw-rw-rw-   0 root         (0) root         (0)     1150 2023-04-11 20:18:49.000000 NEMO-4.5.4/NEMO/static/favicon.ico
-drwxr-xr-x   0 root         (0) root         (0)        0 2023-04-21 23:04:43.415914 NEMO-4.5.4/NEMO/static/fullcalendar/
--rw-rw-rw-   0 root         (0) root         (0)    28531 2023-04-11 20:18:49.000000 NEMO-4.5.4/NEMO/static/fullcalendar/fullcalendar.css
--rw-rw-rw-   0 root         (0) root         (0)   357749 2023-04-11 20:18:49.000000 NEMO-4.5.4/NEMO/static/fullcalendar/fullcalendar.js
--rw-rw-rw-   0 root         (0) root         (0)    13687 2023-04-11 20:18:49.000000 NEMO-4.5.4/NEMO/static/fullcalendar/fullcalendar.min.css
--rw-rw-rw-   0 root         (0) root         (0)   168700 2023-04-11 20:18:49.000000 NEMO-4.5.4/NEMO/static/fullcalendar/fullcalendar.min.js
-drwxr-xr-x   0 root         (0) root         (0)        0 2023-04-21 23:04:43.416914 NEMO-4.5.4/NEMO/static/icons/
--rw-rw-rw-   0 root         (0) root         (0)    24065 2023-04-11 20:18:49.000000 NEMO-4.5.4/NEMO/static/icons/agreement.png
--rw-rw-rw-   0 root         (0) root         (0)    16685 2023-04-11 20:18:49.000000 NEMO-4.5.4/NEMO/static/icons/caution.png
--rw-rw-rw-   0 root         (0) root         (0)     4664 2023-04-11 20:18:49.000000 NEMO-4.5.4/NEMO/static/icons/preferences.png
--rw-rw-rw-   0 root         (0) root         (0)   247387 2023-04-11 20:18:49.000000 NEMO-4.5.4/NEMO/static/jquery.js
--rw-rw-rw-   0 root         (0) root         (0)    84320 2023-04-11 20:18:49.000000 NEMO-4.5.4/NEMO/static/jquery.min.js
--rw-rw-rw-   0 root         (0) root         (0)  1183392 2023-04-11 20:18:49.000000 NEMO-4.5.4/NEMO/static/jumbotron_watermark.bmp
--rw-rw-rw-   0 root         (0) root         (0)     1017 2023-04-11 20:18:49.000000 NEMO-4.5.4/NEMO/static/mobile.js
--rw-rw-rw-   0 root         (0) root         (0)   174603 2023-04-11 20:18:49.000000 NEMO-4.5.4/NEMO/static/moment.js
--rw-rw-rw-   0 root         (0) root         (0)    58102 2023-04-11 20:18:49.000000 NEMO-4.5.4/NEMO/static/moment.min.js
--rw-rw-rw-   0 root         (0) root         (0)    86041 2023-04-11 20:18:49.000000 NEMO-4.5.4/NEMO/static/moment.min.js.map
--rw-rw-rw-   0 root         (0) root         (0)    15594 2023-04-11 20:18:49.000000 NEMO-4.5.4/NEMO/static/nemo.css
--rw-rw-rw-   0 root         (0) root         (0)    20155 2023-04-11 20:18:49.000000 NEMO-4.5.4/NEMO/static/nemo.js
-drwxr-xr-x   0 root         (0) root         (0)        0 2023-04-21 23:04:43.416914 NEMO-4.5.4/NEMO/static/numpad/
--rw-rw-rw-   0 root         (0) root         (0)    12285 2023-04-11 20:18:49.000000 NEMO-4.5.4/NEMO/static/numpad/custom_numpad.jquery.js
--rw-rw-rw-   0 root         (0) root         (0)      255 2023-04-11 20:18:49.000000 NEMO-4.5.4/NEMO/static/numpad/numpad.jquery.css
-drwxr-xr-x   0 root         (0) root         (0)        0 2023-04-21 23:04:43.417914 NEMO-4.5.4/NEMO/static/pickadate/
--rw-rw-rw-   0 root         (0) root         (0)     3795 2023-04-11 20:18:49.000000 NEMO-4.5.4/NEMO/static/pickadate/default.css
--rw-rw-rw-   0 root         (0) root         (0)     6040 2023-04-11 20:18:49.000000 NEMO-4.5.4/NEMO/static/pickadate/default.date.css
--rw-rw-rw-   0 root         (0) root         (0)     2785 2023-04-11 20:18:49.000000 NEMO-4.5.4/NEMO/static/pickadate/default.time.css
--rw-rw-rw-   0 root         (0) root         (0)    48215 2023-04-11 20:18:49.000000 NEMO-4.5.4/NEMO/static/pickadate/picker.date.js
--rw-rw-rw-   0 root         (0) root         (0)    36941 2023-04-11 20:18:49.000000 NEMO-4.5.4/NEMO/static/pickadate/picker.js
--rw-rw-rw-   0 root         (0) root         (0)    31899 2023-04-11 20:18:49.000000 NEMO-4.5.4/NEMO/static/pickadate/picker.time.js
--rw-rw-rw-   0 root         (0) root         (0)       25 2023-04-11 20:18:49.000000 NEMO-4.5.4/NEMO/static/robots.txt
--rw-rw-rw-   0 root         (0) root         (0)    48446 2023-04-11 20:18:49.000000 NEMO-4.5.4/NEMO/static/typeahead.jquery.js
--rw-rw-rw-   0 root         (0) root         (0)    20748 2023-04-11 20:18:49.000000 NEMO-4.5.4/NEMO/static/typeahead.jquery.min.js
-drwxr-xr-x   0 root         (0) root         (0)        0 2023-04-21 23:04:43.418914 NEMO-4.5.4/NEMO/static/virtualkeyboard/
--rw-rw-rw-   0 root         (0) root         (0)   113008 2023-04-11 20:18:49.000000 NEMO-4.5.4/NEMO/static/virtualkeyboard/jquery.keyboard.js
--rw-rw-rw-   0 root         (0) root         (0)    47325 2023-04-11 20:18:49.000000 NEMO-4.5.4/NEMO/static/virtualkeyboard/jquery.keyboard.min.js
--rw-rw-rw-   0 root         (0) root         (0)     7848 2023-04-11 20:18:49.000000 NEMO-4.5.4/NEMO/static/virtualkeyboard/keyboard-basic.css
--rw-rw-rw-   0 root         (0) root         (0)     5889 2023-04-11 20:18:49.000000 NEMO-4.5.4/NEMO/static/virtualkeyboard/keyboard-basic.min.css
-drwxr-xr-x   0 root         (0) root         (0)        0 2023-04-21 23:04:43.421914 NEMO-4.5.4/NEMO/templates/
-drwxr-xr-x   0 root         (0) root         (0)        0 2023-04-21 23:04:43.421914 NEMO-4.5.4/NEMO/templates/abuse/
--rw-rw-rw-   0 root         (0) root         (0)     4059 2023-04-11 20:18:49.000000 NEMO-4.5.4/NEMO/templates/abuse/abuse.html
--rw-rw-rw-   0 root         (0) root         (0)      580 2023-04-11 20:18:49.000000 NEMO-4.5.4/NEMO/templates/abuse/user_drill_down.html
-drwxr-xr-x   0 root         (0) root         (0)        0 2023-04-21 23:04:43.422914 NEMO-4.5.4/NEMO/templates/accounts_and_projects/
--rw-rw-rw-   0 root         (0) root         (0)     7380 2023-04-11 20:18:49.000000 NEMO-4.5.4/NEMO/templates/accounts_and_projects/account_and_projects.html
--rw-rw-rw-   0 root         (0) root         (0)     6415 2023-04-11 20:18:49.000000 NEMO-4.5.4/NEMO/templates/accounts_and_projects/accounts_and_projects.html
--rw-rw-rw-   0 root         (0) root         (0)     2843 2023-04-11 20:18:49.000000 NEMO-4.5.4/NEMO/templates/accounts_and_projects/create_account.html
--rw-rw-rw-   0 root         (0) root         (0)     5002 2023-04-11 20:18:49.000000 NEMO-4.5.4/NEMO/templates/accounts_and_projects/create_project.html
--rw-rw-rw-   0 root         (0) root         (0)      888 2023-04-11 20:18:49.000000 NEMO-4.5.4/NEMO/templates/accounts_and_projects/documents_for_project.html
--rw-rw-rw-   0 root         (0) root         (0)     3530 2023-04-11 20:18:49.000000 NEMO-4.5.4/NEMO/templates/accounts_and_projects/projects.html
--rw-rw-rw-   0 root         (0) root         (0)      924 2023-04-11 20:18:49.000000 NEMO-4.5.4/NEMO/templates/accounts_and_projects/users_for_project.html
--rw-rw-rw-   0 root         (0) root         (0)      433 2023-04-11 20:18:49.000000 NEMO-4.5.4/NEMO/templates/acknowledgement.html
--rw-rw-rw-   0 root         (0) root         (0)     4694 2023-04-11 20:18:49.000000 NEMO-4.5.4/NEMO/templates/alerts.html
-drwxr-xr-x   0 root         (0) root         (0)        0 2023-04-21 23:04:43.423914 NEMO-4.5.4/NEMO/templates/area_access/
--rw-rw-rw-   0 root         (0) root         (0)     2951 2023-04-11 20:18:49.000000 NEMO-4.5.4/NEMO/templates/area_access/area_access.html
--rw-rw-rw-   0 root         (0) root         (0)     1687 2023-04-11 20:18:49.000000 NEMO-4.5.4/NEMO/templates/area_access/calendar_self_login.html
--rw-rw-rw-   0 root         (0) root         (0)     1111 2023-04-11 20:18:49.000000 NEMO-4.5.4/NEMO/templates/area_access/change_project.html
--rw-rw-rw-   0 root         (0) root         (0)     1141 2023-04-11 20:18:49.000000 NEMO-4.5.4/NEMO/templates/area_access/login_areas.html
--rw-rw-rw-   0 root         (0) root         (0)     1245 2023-04-11 20:18:49.000000 NEMO-4.5.4/NEMO/templates/area_access/new_area_access_record.html
--rw-rw-rw-   0 root         (0) root         (0)     1938 2023-04-11 20:18:49.000000 NEMO-4.5.4/NEMO/templates/area_access/new_area_access_record_details.html
--rw-rw-rw-   0 root         (0) root         (0)     1454 2023-04-11 20:18:49.000000 NEMO-4.5.4/NEMO/templates/area_access/self_login.html
--rw-rw-rw-   0 root         (0) root         (0)      837 2023-04-11 20:18:49.000000 NEMO-4.5.4/NEMO/templates/authorization_failed.html
-drwxr-xr-x   0 root         (0) root         (0)        0 2023-04-21 23:04:43.423914 NEMO-4.5.4/NEMO/templates/base/
--rw-rw-rw-   0 root         (0) root         (0)      308 2023-04-11 20:18:49.000000 NEMO-4.5.4/NEMO/templates/base/footer.html
--rw-rw-rw-   0 root         (0) root         (0)      292 2023-04-11 20:18:49.000000 NEMO-4.5.4/NEMO/templates/base/impersonate_header.html
--rw-rw-rw-   0 root         (0) root         (0)       37 2023-04-11 20:18:49.000000 NEMO-4.5.4/NEMO/templates/base/navbar.html
--rw-rw-rw-   0 root         (0) root         (0)     7633 2023-04-11 20:18:49.000000 NEMO-4.5.4/NEMO/templates/base/navbar_base.html
--rw-rw-rw-   0 root         (0) root         (0)      247 2023-04-11 20:18:49.000000 NEMO-4.5.4/NEMO/templates/base/popup.html
--rw-rw-rw-   0 root         (0) root         (0)     5811 2023-04-11 20:18:49.000000 NEMO-4.5.4/NEMO/templates/base.html
-drwxr-xr-x   0 root         (0) root         (0)        0 2023-04-21 23:04:43.425914 NEMO-4.5.4/NEMO/templates/calendar/
--rw-rw-rw-   0 root         (0) root         (0)    24260 2023-04-11 20:18:49.000000 NEMO-4.5.4/NEMO/templates/calendar/calendar.html
--rw-rw-rw-   0 root         (0) root         (0)     1381 2023-04-11 20:18:49.000000 NEMO-4.5.4/NEMO/templates/calendar/configuration.html
--rw-rw-rw-   0 root         (0) root         (0)     2834 2023-04-11 20:18:49.000000 NEMO-4.5.4/NEMO/templates/calendar/configuration_helper.html
--rw-rw-rw-   0 root         (0) root         (0)     1254 2023-04-11 20:18:49.000000 NEMO-4.5.4/NEMO/templates/calendar/policy_dialog.html
--rw-rw-rw-   0 root         (0) root         (0)     1300 2023-04-11 20:18:49.000000 NEMO-4.5.4/NEMO/templates/calendar/project_choice.html
--rw-rw-rw-   0 root         (0) root         (0)     1335 2023-04-11 20:18:49.000000 NEMO-4.5.4/NEMO/templates/calendar/proxy_reservation.html
--rw-rw-rw-   0 root         (0) root         (0)     1862 2023-04-11 20:18:49.000000 NEMO-4.5.4/NEMO/templates/calendar/reservation_event_feed.html
--rw-rw-rw-   0 root         (0) root         (0)     1619 2023-04-11 20:18:49.000000 NEMO-4.5.4/NEMO/templates/calendar/reservation_questions.html
--rw-rw-rw-   0 root         (0) root         (0)     1285 2023-04-11 20:18:49.000000 NEMO-4.5.4/NEMO/templates/calendar/reservation_warning.html
--rw-rw-rw-   0 root         (0) root         (0)     4094 2023-04-11 20:18:49.000000 NEMO-4.5.4/NEMO/templates/calendar/scheduled_outage_information.html
--rw-rw-rw-   0 root         (0) root         (0)     2011 2023-04-11 20:18:49.000000 NEMO-4.5.4/NEMO/templates/calendar/specific_user_feed.html
--rw-rw-rw-   0 root         (0) root         (0)     2543 2023-04-11 20:18:49.000000 NEMO-4.5.4/NEMO/templates/calendar/usage_event_feed.html
--rw-rw-rw-   0 root         (0) root         (0)     6530 2023-04-11 20:18:49.000000 NEMO-4.5.4/NEMO/templates/configuration_agenda.html
-drwxr-xr-x   0 root         (0) root         (0)        0 2023-04-21 23:04:43.426914 NEMO-4.5.4/NEMO/templates/consumables/
--rw-rw-rw-   0 root         (0) root         (0)     8048 2023-04-11 20:18:49.000000 NEMO-4.5.4/NEMO/templates/consumables/consumables.html
--rw-rw-rw-   0 root         (0) root         (0)     1518 2023-04-11 20:18:49.000000 NEMO-4.5.4/NEMO/templates/consumables/consumables_order.html
--rw-rw-rw-   0 root         (0) root         (0)    11695 2023-04-11 20:18:49.000000 NEMO-4.5.4/NEMO/templates/consumables/recurring_charge.html
--rw-rw-rw-   0 root         (0) root         (0)     5491 2023-04-11 20:18:49.000000 NEMO-4.5.4/NEMO/templates/consumables/recurring_charges.html
-drwxr-xr-x   0 root         (0) root         (0)        0 2023-04-21 23:04:43.426914 NEMO-4.5.4/NEMO/templates/contact/
--rw-rw-rw-   0 root         (0) root         (0)      692 2023-04-11 20:18:49.000000 NEMO-4.5.4/NEMO/templates/contact/contact_staff.html
-drwxr-xr-x   0 root         (0) root         (0)        0 2023-04-21 23:04:43.428914 NEMO-4.5.4/NEMO/templates/customizations/
--rw-rw-rw-   0 root         (0) root         (0)     1848 2023-04-11 20:18:49.000000 NEMO-4.5.4/NEMO/templates/customizations/customizations.html
--rw-rw-rw-   0 root         (0) root         (0)     2318 2023-04-11 20:18:49.000000 NEMO-4.5.4/NEMO/templates/customizations/customizations_application.html
--rw-rw-rw-   0 root         (0) root         (0)     7799 2023-04-11 20:18:49.000000 NEMO-4.5.4/NEMO/templates/customizations/customizations_calendar.html
--rw-rw-rw-   0 root         (0) root         (0)     7324 2023-04-11 20:18:49.000000 NEMO-4.5.4/NEMO/templates/customizations/customizations_dashboard.html
--rw-rw-rw-   0 root         (0) root         (0)     4202 2023-04-11 20:18:49.000000 NEMO-4.5.4/NEMO/templates/customizations/customizations_emails.html
--rw-rw-rw-   0 root         (0) root         (0)     2545 2023-04-11 20:18:49.000000 NEMO-4.5.4/NEMO/templates/customizations/customizations_interlock.html
--rw-rw-rw-   0 root         (0) root         (0)     5553 2023-04-11 20:18:49.000000 NEMO-4.5.4/NEMO/templates/customizations/customizations_projects_and_accounts.html
--rw-rw-rw-   0 root         (0) root         (0)     2224 2023-04-11 20:18:49.000000 NEMO-4.5.4/NEMO/templates/customizations/customizations_rates.html
--rw-rw-rw-   0 root         (0) root         (0)     3519 2023-04-11 20:18:49.000000 NEMO-4.5.4/NEMO/templates/customizations/customizations_recurring_charges.html
--rw-rw-rw-   0 root         (0) root         (0)     2183 2023-04-11 20:18:49.000000 NEMO-4.5.4/NEMO/templates/customizations/customizations_remote_work.html
--rw-rw-rw-   0 root         (0) root         (0)    16061 2023-04-11 20:18:49.000000 NEMO-4.5.4/NEMO/templates/customizations/customizations_requests.html
--rw-rw-rw-   0 root         (0) root         (0)     3678 2023-04-11 20:18:49.000000 NEMO-4.5.4/NEMO/templates/customizations/customizations_safety.html
--rw-rw-rw-   0 root         (0) root         (0)    27806 2023-04-11 20:18:49.000000 NEMO-4.5.4/NEMO/templates/customizations/customizations_templates.html
--rw-rw-rw-   0 root         (0) root         (0)     8661 2023-04-11 20:18:49.000000 NEMO-4.5.4/NEMO/templates/customizations/customizations_tool.html
--rw-rw-rw-   0 root         (0) root         (0)     1731 2023-04-11 20:18:49.000000 NEMO-4.5.4/NEMO/templates/customizations/customizations_upload.html
--rw-rw-rw-   0 root         (0) root         (0)     5214 2023-04-11 20:18:49.000000 NEMO-4.5.4/NEMO/templates/customizations/customizations_user.html
--rw-rw-rw-   0 root         (0) root         (0)      441 2023-04-11 20:18:49.000000 NEMO-4.5.4/NEMO/templates/display_success_and_redirect.html
-drwxr-xr-x   0 root         (0) root         (0)        0 2023-04-21 23:04:43.429914 NEMO-4.5.4/NEMO/templates/email/
--rw-rw-rw-   0 root         (0) root         (0)     7800 2023-04-11 20:18:49.000000 NEMO-4.5.4/NEMO/templates/email/compose_email.html
--rw-rw-rw-   0 root         (0) root         (0)     3153 2023-04-11 20:18:49.000000 NEMO-4.5.4/NEMO/templates/email/email_broadcast.html
--rw-rw-rw-   0 root         (0) root         (0)     1045 2023-04-11 20:18:49.000000 NEMO-4.5.4/NEMO/templates/email/email_form.html
-drwxr-xr-x   0 root         (0) root         (0)        0 2023-04-21 23:04:43.429914 NEMO-4.5.4/NEMO/templates/event_details/
--rw-rw-rw-   0 root         (0) root         (0)      751 2023-04-11 20:18:49.000000 NEMO-4.5.4/NEMO/templates/event_details/area_access_details.html
--rw-rw-rw-   0 root         (0) root         (0)     1347 2023-04-11 20:18:49.000000 NEMO-4.5.4/NEMO/templates/event_details/outage_details.html
--rw-rw-rw-   0 root         (0) root         (0)     9603 2023-04-11 20:18:49.000000 NEMO-4.5.4/NEMO/templates/event_details/reservation_details.html
--rw-rw-rw-   0 root         (0) root         (0)      589 2023-04-11 20:18:49.000000 NEMO-4.5.4/NEMO/templates/event_details/usage_details.html
--rw-rw-rw-   0 root         (0) root         (0)      426 2023-04-11 20:18:49.000000 NEMO-4.5.4/NEMO/templates/facility_rules.html
--rw-rw-rw-   0 root         (0) root         (0)     1247 2023-04-11 20:18:49.000000 NEMO-4.5.4/NEMO/templates/feedback.html
--rw-rw-rw-   0 root         (0) root         (0)      937 2023-04-11 20:18:49.000000 NEMO-4.5.4/NEMO/templates/history.html
--rw-rw-rw-   0 root         (0) root         (0)     1217 2023-04-11 20:18:49.000000 NEMO-4.5.4/NEMO/templates/impersonate.html
-drwxr-xr-x   0 root         (0) root         (0)        0 2023-04-21 23:04:43.430914 NEMO-4.5.4/NEMO/templates/jumbotron/
--rw-rw-rw-   0 root         (0) root         (0)     2059 2023-04-11 20:18:49.000000 NEMO-4.5.4/NEMO/templates/jumbotron/jumbotron.html
--rw-rw-rw-   0 root         (0) root         (0)     3635 2023-04-11 20:18:49.000000 NEMO-4.5.4/NEMO/templates/jumbotron/jumbotron_content.html
--rw-rw-rw-   0 root         (0) root         (0)     8671 2023-04-11 20:18:49.000000 NEMO-4.5.4/NEMO/templates/landing.html
--rw-rw-rw-   0 root         (0) root         (0)     3496 2023-04-11 20:18:49.000000 NEMO-4.5.4/NEMO/templates/login.html
-drwxr-xr-x   0 root         (0) root         (0)        0 2023-04-21 23:04:43.430914 NEMO-4.5.4/NEMO/templates/maintenance/
--rw-rw-rw-   0 root         (0) root         (0)     1558 2023-04-11 20:18:49.000000 NEMO-4.5.4/NEMO/templates/maintenance/closed_task_details.html
--rw-rw-rw-   0 root         (0) root         (0)     5566 2023-04-11 20:18:49.000000 NEMO-4.5.4/NEMO/templates/maintenance/maintenance.html
--rw-rw-rw-   0 root         (0) root         (0)     7450 2023-04-11 20:18:49.000000 NEMO-4.5.4/NEMO/templates/maintenance/pending_task_details.html
-drwxr-xr-x   0 root         (0) root         (0)        0 2023-04-21 23:04:43.431914 NEMO-4.5.4/NEMO/templates/mobile/
--rw-rw-rw-   0 root         (0) root         (0)      762 2023-04-11 20:18:49.000000 NEMO-4.5.4/NEMO/templates/mobile/cancellation_result.html
--rw-rw-rw-   0 root         (0) root         (0)     1916 2023-04-11 20:18:49.000000 NEMO-4.5.4/NEMO/templates/mobile/choose_item.html
--rw-rw-rw-   0 root         (0) root         (0)      453 2023-04-11 20:18:49.000000 NEMO-4.5.4/NEMO/templates/mobile/error.html
--rw-rw-rw-   0 root         (0) root         (0)     1025 2023-04-11 20:18:49.000000 NEMO-4.5.4/NEMO/templates/mobile/individual_outage.html
--rw-rw-rw-   0 root         (0) root         (0)     2625 2023-04-11 20:18:49.000000 NEMO-4.5.4/NEMO/templates/mobile/individual_reservation.html
--rw-rw-rw-   0 root         (0) root         (0)     5899 2023-04-11 20:18:49.000000 NEMO-4.5.4/NEMO/templates/mobile/new_reservation.html
--rw-rw-rw-   0 root         (0) root         (0)      313 2023-04-11 20:18:49.000000 NEMO-4.5.4/NEMO/templates/mobile/no_active_projects.html
--rw-rw-rw-   0 root         (0) root         (0)      777 2023-04-11 20:18:49.000000 NEMO-4.5.4/NEMO/templates/mobile/reservation_success.html
--rw-rw-rw-   0 root         (0) root         (0)     1442 2023-04-11 20:18:49.000000 NEMO-4.5.4/NEMO/templates/mobile/view_calendar.html
-drwxr-xr-x   0 root         (0) root         (0)        0 2023-04-21 23:04:43.432914 NEMO-4.5.4/NEMO/templates/news/
--rw-rw-rw-   0 root         (0) root         (0)      981 2023-04-11 20:18:49.000000 NEMO-4.5.4/NEMO/templates/news/archived_news.html
--rw-rw-rw-   0 root         (0) root         (0)     1027 2023-04-11 20:18:49.000000 NEMO-4.5.4/NEMO/templates/news/new_news_form.html
--rw-rw-rw-   0 root         (0) root         (0)     1198 2023-04-11 20:18:49.000000 NEMO-4.5.4/NEMO/templates/news/news_update_form.html
--rw-rw-rw-   0 root         (0) root         (0)     2038 2023-04-11 20:18:49.000000 NEMO-4.5.4/NEMO/templates/news/recent_news.html
--rw-rw-rw-   0 root         (0) root         (0)      209 2023-04-11 20:18:49.000000 NEMO-4.5.4/NEMO/templates/no_project.html
-drwxr-xr-x   0 root         (0) root         (0)        0 2023-04-21 23:04:43.432914 NEMO-4.5.4/NEMO/templates/occupancy/
--rw-rw-rw-   0 root         (0) root         (0)      408 2023-04-11 20:18:49.000000 NEMO-4.5.4/NEMO/templates/occupancy/occupancy.html
--rw-rw-rw-   0 root         (0) root         (0)     1841 2023-04-11 20:18:49.000000 NEMO-4.5.4/NEMO/templates/occupancy/occupancy_content.html
--rw-rw-rw-   0 root         (0) root         (0)     1147 2023-04-11 20:18:49.000000 NEMO-4.5.4/NEMO/templates/occupancy/occupancy_count.html
-drwxr-xr-x   0 root         (0) root         (0)        0 2023-04-21 23:04:43.433914 NEMO-4.5.4/NEMO/templates/pagination/
--rw-rw-rw-   0 root         (0) root         (0)      865 2023-04-11 20:18:49.000000 NEMO-4.5.4/NEMO/templates/pagination/pagination_base.html
--rw-rw-rw-   0 root         (0) root         (0)      521 2023-04-11 20:18:49.000000 NEMO-4.5.4/NEMO/templates/pagination/pagination_column.html
--rw-rw-rw-   0 root         (0) root         (0)      673 2023-04-11 20:18:49.000000 NEMO-4.5.4/NEMO/templates/pagination/pagination_pages.html
--rw-rw-rw-   0 root         (0) root         (0)      642 2023-04-11 20:18:49.000000 NEMO-4.5.4/NEMO/templates/pagination/pagination_selector.html
--rw-rw-rw-   0 root         (0) root         (0)     2841 2023-04-11 20:18:49.000000 NEMO-4.5.4/NEMO/templates/qualifications.html
--rw-rw-rw-   0 root         (0) root         (0)     5462 2023-04-11 20:18:49.000000 NEMO-4.5.4/NEMO/templates/refresh_sidebar_icons.html
-drwxr-xr-x   0 root         (0) root         (0)        0 2023-04-21 23:04:43.433914 NEMO-4.5.4/NEMO/templates/remote_work/
--rw-rw-rw-   0 root         (0) root         (0)    10561 2023-04-11 20:18:49.000000 NEMO-4.5.4/NEMO/templates/remote_work/remote_work.html
--rw-rw-rw-   0 root         (0) root         (0)     1081 2023-04-11 20:18:49.000000 NEMO-4.5.4/NEMO/templates/remote_work/remote_work_base.html
-drwxr-xr-x   0 root         (0) root         (0)        0 2023-04-21 23:04:43.433914 NEMO-4.5.4/NEMO/templates/requests/
-drwxr-xr-x   0 root         (0) root         (0)        0 2023-04-21 23:04:43.434914 NEMO-4.5.4/NEMO/templates/requests/access_requests/
--rw-rw-rw-   0 root         (0) root         (0)     7754 2023-04-11 20:18:49.000000 NEMO-4.5.4/NEMO/templates/requests/access_requests/access_request.html
--rw-rw-rw-   0 root         (0) root         (0)     3450 2023-04-11 20:18:49.000000 NEMO-4.5.4/NEMO/templates/requests/access_requests/access_requests.html
--rw-rw-rw-   0 root         (0) root         (0)     3480 2023-04-11 20:18:49.000000 NEMO-4.5.4/NEMO/templates/requests/access_requests/access_requests_table.html
-drwxr-xr-x   0 root         (0) root         (0)        0 2023-04-21 23:04:43.434914 NEMO-4.5.4/NEMO/templates/requests/adjustment_requests/
--rw-rw-rw-   0 root         (0) root         (0)     8607 2023-04-11 20:18:49.000000 NEMO-4.5.4/NEMO/templates/requests/adjustment_requests/adjustment_request.html
--rw-rw-rw-   0 root         (0) root         (0)     3733 2023-04-11 20:18:49.000000 NEMO-4.5.4/NEMO/templates/requests/adjustment_requests/adjustment_requests.html
--rw-rw-rw-   0 root         (0) root         (0)     6659 2023-04-11 20:18:49.000000 NEMO-4.5.4/NEMO/templates/requests/adjustment_requests/adjustment_requests_table.html
-drwxr-xr-x   0 root         (0) root         (0)        0 2023-04-21 23:04:43.434914 NEMO-4.5.4/NEMO/templates/requests/buddy_requests/
--rw-rw-rw-   0 root         (0) root         (0)     3910 2023-04-11 20:18:49.000000 NEMO-4.5.4/NEMO/templates/requests/buddy_requests/buddy_request.html
--rw-rw-rw-   0 root         (0) root         (0)     5602 2023-04-11 20:18:49.000000 NEMO-4.5.4/NEMO/templates/requests/buddy_requests/buddy_requests.html
--rw-rw-rw-   0 root         (0) root         (0)     4246 2023-04-11 20:18:49.000000 NEMO-4.5.4/NEMO/templates/requests/user_requests.html
-drwxr-xr-x   0 root         (0) root         (0)        0 2023-04-21 23:04:43.435914 NEMO-4.5.4/NEMO/templates/resources/
--rw-rw-rw-   0 root         (0) root         (0)     2950 2023-04-11 20:18:49.000000 NEMO-4.5.4/NEMO/templates/resources/modify_resource.html
--rw-rw-rw-   0 root         (0) root         (0)     3846 2023-04-11 20:18:49.000000 NEMO-4.5.4/NEMO/templates/resources/resource_details.html
--rw-rw-rw-   0 root         (0) root         (0)     1423 2023-04-11 20:18:49.000000 NEMO-4.5.4/NEMO/templates/resources/resources.html
--rw-rw-rw-   0 root         (0) root         (0)     3807 2023-04-11 20:18:49.000000 NEMO-4.5.4/NEMO/templates/resources/scheduled_outage.html
-drwxr-xr-x   0 root         (0) root         (0)        0 2023-04-21 23:04:43.435914 NEMO-4.5.4/NEMO/templates/rest_framework/
--rw-rw-rw-   0 root         (0) root         (0)     2736 2023-04-11 20:18:49.000000 NEMO-4.5.4/NEMO/templates/rest_framework/api.html
--rw-rw-rw-   0 root         (0) root         (0)      446 2023-04-11 20:18:49.000000 NEMO-4.5.4/NEMO/templates/rest_framework/custom_error.html
-drwxr-xr-x   0 root         (0) root         (0)        0 2023-04-21 23:04:43.436914 NEMO-4.5.4/NEMO/templates/safety/
--rw-rw-rw-   0 root         (0) root         (0)     3112 2023-04-11 20:18:49.000000 NEMO-4.5.4/NEMO/templates/safety/safety.html
--rw-rw-rw-   0 root         (0) root         (0)     1831 2023-04-11 20:18:49.000000 NEMO-4.5.4/NEMO/templates/safety/safety_base.html
--rw-rw-rw-   0 root         (0) root         (0)     7754 2023-04-11 20:18:49.000000 NEMO-4.5.4/NEMO/templates/safety/safety_data_sheets.html
--rw-rw-rw-   0 root         (0) root         (0)     1990 2023-04-11 20:18:49.000000 NEMO-4.5.4/NEMO/templates/safety/safety_issues.html
--rw-rw-rw-   0 root         (0) root         (0)     1723 2023-04-11 20:18:49.000000 NEMO-4.5.4/NEMO/templates/safety/safety_issues_create.html
--rw-rw-rw-   0 root         (0) root         (0)     1722 2023-04-11 20:18:49.000000 NEMO-4.5.4/NEMO/templates/safety/safety_issues_resolved.html
--rw-rw-rw-   0 root         (0) root         (0)     1762 2023-04-11 20:18:49.000000 NEMO-4.5.4/NEMO/templates/safety/safety_issues_update.html
--rw-rw-rw-   0 root         (0) root         (0)     1713 2023-04-11 20:18:49.000000 NEMO-4.5.4/NEMO/templates/safety/safety_items.html
-drwxr-xr-x   0 root         (0) root         (0)        0 2023-04-21 23:04:43.437914 NEMO-4.5.4/NEMO/templates/snippets/
--rw-rw-rw-   0 root         (0) root         (0)      516 2023-04-11 20:18:49.000000 NEMO-4.5.4/NEMO/templates/snippets/button.html
--rw-rw-rw-   0 root         (0) root         (0)      904 2023-04-11 20:18:49.000000 NEMO-4.5.4/NEMO/templates/snippets/contact_person.html
--rw-rw-rw-   0 root         (0) root         (0)     1128 2023-04-11 20:18:49.000000 NEMO-4.5.4/NEMO/templates/snippets/embedded_document.html
--rw-rw-rw-   0 root         (0) root         (0)     1673 2023-04-11 20:18:49.000000 NEMO-4.5.4/NEMO/templates/snippets/tool_info.html
-drwxr-xr-x   0 root         (0) root         (0)        0 2023-04-21 23:04:43.438914 NEMO-4.5.4/NEMO/templates/staff_charges/
--rw-rw-rw-   0 root         (0) root         (0)      860 2023-04-11 20:18:49.000000 NEMO-4.5.4/NEMO/templates/staff_charges/change_status.html
--rw-rw-rw-   0 root         (0) root         (0)     1242 2023-04-11 20:18:49.000000 NEMO-4.5.4/NEMO/templates/staff_charges/choose_project.html
--rw-rw-rw-   0 root         (0) root         (0)      498 2023-04-11 20:18:49.000000 NEMO-4.5.4/NEMO/templates/staff_charges/end_area_charge.html
--rw-rw-rw-   0 root         (0) root         (0)     1198 2023-04-11 20:18:49.000000 NEMO-4.5.4/NEMO/templates/staff_charges/new_staff_charge.html
--rw-rw-rw-   0 root         (0) root         (0)      953 2023-04-11 20:18:49.000000 NEMO-4.5.4/NEMO/templates/staff_charges/reminder.html
--rw-rw-rw-   0 root         (0) root         (0)     1854 2023-04-11 20:18:49.000000 NEMO-4.5.4/NEMO/templates/staff_charges/staff_charges_base.html
-drwxr-xr-x   0 root         (0) root         (0)        0 2023-04-21 23:04:43.439914 NEMO-4.5.4/NEMO/templates/status_dashboard/
--rw-rw-rw-   0 root         (0) root         (0)     1554 2023-04-11 20:18:49.000000 NEMO-4.5.4/NEMO/templates/status_dashboard/occupancy.html
--rw-rw-rw-   0 root         (0) root         (0)     8659 2023-04-11 20:18:49.000000 NEMO-4.5.4/NEMO/templates/status_dashboard/staff.html
--rw-rw-rw-   0 root         (0) root         (0)     7728 2023-04-11 20:18:49.000000 NEMO-4.5.4/NEMO/templates/status_dashboard/staff_absence.html
--rw-rw-rw-   0 root         (0) root         (0)     5799 2023-04-11 20:18:49.000000 NEMO-4.5.4/NEMO/templates/status_dashboard/status_dashboard.html
--rw-rw-rw-   0 root         (0) root         (0)     3534 2023-04-11 20:18:49.000000 NEMO-4.5.4/NEMO/templates/status_dashboard/tools.html
-drwxr-xr-x   0 root         (0) root         (0)        0 2023-04-21 23:04:43.439914 NEMO-4.5.4/NEMO/templates/tasks/
--rw-rw-rw-   0 root         (0) root         (0)     2542 2023-04-11 20:18:49.000000 NEMO-4.5.4/NEMO/templates/tasks/resolve.html
--rw-rw-rw-   0 root         (0) root         (0)     5037 2023-04-11 20:18:49.000000 NEMO-4.5.4/NEMO/templates/tasks/update.html
-drwxr-xr-x   0 root         (0) root         (0)        0 2023-04-21 23:04:43.440914 NEMO-4.5.4/NEMO/templates/tool_control/
--rw-rw-rw-   0 root         (0) root         (0)      873 2023-04-11 20:18:49.000000 NEMO-4.5.4/NEMO/templates/tool_control/get_projects.html
--rw-rw-rw-   0 root         (0) root         (0)      679 2023-04-11 20:18:49.000000 NEMO-4.5.4/NEMO/templates/tool_control/interlock_error.html
--rw-rw-rw-   0 root         (0) root         (0)     3502 2023-04-11 20:18:49.000000 NEMO-4.5.4/NEMO/templates/tool_control/past_tasks_and_comments.html
--rw-rw-rw-   0 root         (0) root         (0)     2472 2023-04-11 20:18:49.000000 NEMO-4.5.4/NEMO/templates/tool_control/qualified_users.html
--rw-rw-rw-   0 root         (0) root         (0)    15540 2023-04-11 20:18:49.000000 NEMO-4.5.4/NEMO/templates/tool_control/tool_control.html
--rw-rw-rw-   0 root         (0) root         (0)    36294 2023-04-11 20:18:49.000000 NEMO-4.5.4/NEMO/templates/tool_control/tool_status.html
--rw-rw-rw-   0 root         (0) root         (0)     6142 2023-04-11 20:18:49.000000 NEMO-4.5.4/NEMO/templates/tool_control/usage_data.html
--rw-rw-rw-   0 root         (0) root         (0)      409 2023-04-11 20:18:49.000000 NEMO-4.5.4/NEMO/templates/tool_control/use_tool_for_other.html
-drwxr-xr-x   0 root         (0) root         (0)        0 2023-04-21 23:04:43.441914 NEMO-4.5.4/NEMO/templates/training/
--rw-rw-rw-   0 root         (0) root         (0)      512 2023-04-11 20:18:49.000000 NEMO-4.5.4/NEMO/templates/training/get_projects.html
--rw-rw-rw-   0 root         (0) root         (0)     4964 2023-04-11 20:18:49.000000 NEMO-4.5.4/NEMO/templates/training/training.html
--rw-rw-rw-   0 root         (0) root         (0)     1596 2023-04-11 20:18:49.000000 NEMO-4.5.4/NEMO/templates/training/training_entry.html
-drwxr-xr-x   0 root         (0) root         (0)        0 2023-04-21 23:04:43.441914 NEMO-4.5.4/NEMO/templates/usage/
--rw-rw-rw-   0 root         (0) root         (0)      495 2023-04-11 20:18:49.000000 NEMO-4.5.4/NEMO/templates/usage/adjustment_request_button.html
--rw-rw-rw-   0 root         (0) root         (0)     3573 2023-04-11 20:18:49.000000 NEMO-4.5.4/NEMO/templates/usage/billing.html
--rw-rw-rw-   0 root         (0) root         (0)     9302 2023-04-11 20:18:49.000000 NEMO-4.5.4/NEMO/templates/usage/usage.html
--rw-rw-rw-   0 root         (0) root         (0)     6781 2023-04-11 20:18:49.000000 NEMO-4.5.4/NEMO/templates/usage/usage_base.html
-drwxr-xr-x   0 root         (0) root         (0)        0 2023-04-21 23:04:43.442914 NEMO-4.5.4/NEMO/templates/users/
--rw-rw-rw-   0 root         (0) root         (0)    20751 2023-04-11 20:18:49.000000 NEMO-4.5.4/NEMO/templates/users/create_or_modify_user.html
--rw-rw-rw-   0 root         (0) root         (0)     8054 2023-04-11 20:18:49.000000 NEMO-4.5.4/NEMO/templates/users/preferences.html
--rw-rw-rw-   0 root         (0) root         (0)     3758 2023-04-11 20:18:49.000000 NEMO-4.5.4/NEMO/templates/users/safe_deactivation.html
--rw-rw-rw-   0 root         (0) root         (0)     4160 2023-04-11 20:18:49.000000 NEMO-4.5.4/NEMO/templates/users/users.html
-drwxr-xr-x   0 root         (0) root         (0)        0 2023-04-21 23:04:43.442914 NEMO-4.5.4/NEMO/templatetags/
--rw-rw-rw-   0 root         (0) root         (0)        0 2023-04-21 23:04:29.000000 NEMO-4.5.4/NEMO/templatetags/__init__.py
--rw-rw-rw-   0 root         (0) root         (0)     7223 2023-04-21 23:04:29.000000 NEMO-4.5.4/NEMO/templatetags/custom_tags_and_filters.py
--rw-rw-rw-   0 root         (0) root         (0)    25064 2023-04-11 20:18:49.000000 NEMO-4.5.4/NEMO/urls.py
--rw-rw-rw-   0 root         (0) root         (0)    23455 2023-04-11 20:18:49.000000 NEMO-4.5.4/NEMO/utilities.py
-drwxr-xr-x   0 root         (0) root         (0)        0 2023-04-21 23:04:43.448914 NEMO-4.5.4/NEMO/views/
--rw-rw-rw-   0 root         (0) root         (0)        0 2023-04-21 23:04:29.000000 NEMO-4.5.4/NEMO/views/__init__.py
--rw-rw-rw-   0 root         (0) root         (0)     4308 2023-04-11 20:18:49.000000 NEMO-4.5.4/NEMO/views/abuse.py
--rw-rw-rw-   0 root         (0) root         (0)    14736 2023-04-11 20:18:49.000000 NEMO-4.5.4/NEMO/views/access_requests.py
--rw-rw-rw-   0 root         (0) root         (0)     8275 2023-04-11 20:18:49.000000 NEMO-4.5.4/NEMO/views/accounts_and_projects.py
--rw-rw-rw-   0 root         (0) root         (0)    17076 2023-04-11 20:18:49.000000 NEMO-4.5.4/NEMO/views/adjustment_requests.py
--rw-rw-rw-   0 root         (0) root         (0)     1812 2023-04-11 20:18:49.000000 NEMO-4.5.4/NEMO/views/alerts.py
--rw-rw-rw-   0 root         (0) root         (0)    13935 2023-04-11 20:18:49.000000 NEMO-4.5.4/NEMO/views/api.py
--rw-rw-rw-   0 root         (0) root         (0)    12115 2023-04-11 20:18:49.000000 NEMO-4.5.4/NEMO/views/api_billing.py
--rw-rw-rw-   0 root         (0) root         (0)     2013 2023-04-11 20:18:49.000000 NEMO-4.5.4/NEMO/views/api_file_import.py
--rw-rw-rw-   0 root         (0) root         (0)    18830 2023-04-11 20:18:49.000000 NEMO-4.5.4/NEMO/views/area_access.py
--rw-rw-rw-   0 root         (0) root         (0)    11992 2023-04-11 20:18:49.000000 NEMO-4.5.4/NEMO/views/authentication.py
--rw-rw-rw-   0 root         (0) root         (0)     6625 2023-04-11 20:18:49.000000 NEMO-4.5.4/NEMO/views/buddy_requests.py
--rw-rw-rw-   0 root         (0) root         (0)    68771 2023-04-11 20:18:49.000000 NEMO-4.5.4/NEMO/views/calendar.py
--rw-rw-rw-   0 root         (0) root         (0)     1867 2023-04-11 20:18:49.000000 NEMO-4.5.4/NEMO/views/configuration_agenda.py
--rw-rw-rw-   0 root         (0) root         (0)      174 2023-04-11 20:18:49.000000 NEMO-4.5.4/NEMO/views/constants.py
--rw-rw-rw-   0 root         (0) root         (0)    10021 2023-04-11 20:18:49.000000 NEMO-4.5.4/NEMO/views/consumables.py
--rw-rw-rw-   0 root         (0) root         (0)      467 2023-04-11 20:18:49.000000 NEMO-4.5.4/NEMO/views/contact_staff.py
--rw-rw-rw-   0 root         (0) root         (0)    17713 2023-04-11 20:18:49.000000 NEMO-4.5.4/NEMO/views/customization.py
--rw-rw-rw-   0 root         (0) root         (0)     1335 2023-04-11 20:18:49.000000 NEMO-4.5.4/NEMO/views/documents.py
--rw-rw-rw-   0 root         (0) root         (0)     9978 2023-04-11 20:18:49.000000 NEMO-4.5.4/NEMO/views/email.py
--rw-rw-rw-   0 root         (0) root         (0)     1973 2023-04-11 20:18:49.000000 NEMO-4.5.4/NEMO/views/event_details.py
--rw-rw-rw-   0 root         (0) root         (0)     1482 2023-04-11 20:18:49.000000 NEMO-4.5.4/NEMO/views/feedback.py
--rw-rw-rw-   0 root         (0) root         (0)     1672 2023-04-11 20:18:49.000000 NEMO-4.5.4/NEMO/views/get_projects.py
--rw-rw-rw-   0 root         (0) root         (0)     4168 2023-04-11 20:18:49.000000 NEMO-4.5.4/NEMO/views/history.py
--rw-rw-rw-   0 root         (0) root         (0)     1027 2023-04-11 20:18:49.000000 NEMO-4.5.4/NEMO/views/jumbotron.py
--rw-rw-rw-   0 root         (0) root         (0)     3293 2023-04-11 20:18:49.000000 NEMO-4.5.4/NEMO/views/landing.py
--rw-rw-rw-   0 root         (0) root         (0)     2289 2023-04-11 20:18:49.000000 NEMO-4.5.4/NEMO/views/maintenance.py
--rw-rw-rw-   0 root         (0) root         (0)     8059 2023-04-11 20:18:49.000000 NEMO-4.5.4/NEMO/views/mobile.py
--rw-rw-rw-   0 root         (0) root         (0)     3356 2023-04-11 20:18:49.000000 NEMO-4.5.4/NEMO/views/news.py
--rw-rw-rw-   0 root         (0) root         (0)     5188 2023-04-11 20:18:49.000000 NEMO-4.5.4/NEMO/views/notifications.py
--rw-rw-rw-   0 root         (0) root         (0)     1326 2023-04-11 20:18:49.000000 NEMO-4.5.4/NEMO/views/pagination.py
--rw-rw-rw-   0 root         (0) root         (0)     4822 2023-04-11 20:18:49.000000 NEMO-4.5.4/NEMO/views/qualifications.py
--rw-rw-rw-   0 root         (0) root         (0)     9965 2023-04-11 20:18:49.000000 NEMO-4.5.4/NEMO/views/remote_work.py
--rw-rw-rw-   0 root         (0) root         (0)     3700 2023-04-11 20:18:49.000000 NEMO-4.5.4/NEMO/views/resources.py
--rw-rw-rw-   0 root         (0) root         (0)     8877 2023-04-11 20:18:49.000000 NEMO-4.5.4/NEMO/views/safety.py
--rw-rw-rw-   0 root         (0) root         (0)      932 2023-04-11 20:18:49.000000 NEMO-4.5.4/NEMO/views/sidebar.py
--rw-rw-rw-   0 root         (0) root         (0)    19900 2023-04-11 20:18:49.000000 NEMO-4.5.4/NEMO/views/status_dashboard.py
--rw-rw-rw-   0 root         (0) root         (0)    12963 2023-04-11 20:18:49.000000 NEMO-4.5.4/NEMO/views/tasks.py
--rw-rw-rw-   0 root         (0) root         (0)    23605 2023-04-11 20:18:49.000000 NEMO-4.5.4/NEMO/views/tool_control.py
--rw-rw-rw-   0 root         (0) root         (0)     5953 2023-04-11 20:18:49.000000 NEMO-4.5.4/NEMO/views/training.py
--rw-rw-rw-   0 root         (0) root         (0)     1909 2023-04-11 20:18:49.000000 NEMO-4.5.4/NEMO/views/tutorials.py
--rw-rw-rw-   0 root         (0) root         (0)    18008 2023-04-11 20:18:49.000000 NEMO-4.5.4/NEMO/views/usage.py
--rw-rw-rw-   0 root         (0) root         (0)     1049 2023-04-18 21:38:03.000000 NEMO-4.5.4/NEMO/views/user_requests.py
--rw-rw-rw-   0 root         (0) root         (0)    20715 2023-04-11 20:18:49.000000 NEMO-4.5.4/NEMO/views/users.py
-drwxr-xr-x   0 root         (0) root         (0)        0 2023-04-21 23:04:43.449914 NEMO-4.5.4/NEMO/widgets/
--rw-rw-rw-   0 root         (0) root         (0)        0 2023-04-21 23:04:29.000000 NEMO-4.5.4/NEMO/widgets/__init__.py
--rw-rw-rw-   0 root         (0) root         (0)     2968 2023-04-11 20:18:49.000000 NEMO-4.5.4/NEMO/widgets/configuration_editor.py
--rw-rw-rw-   0 root         (0) root         (0)    26295 2023-04-11 20:18:49.000000 NEMO-4.5.4/NEMO/widgets/dynamic_form.py
--rw-rw-rw-   0 root         (0) root         (0)     8029 2023-04-11 20:18:49.000000 NEMO-4.5.4/NEMO/widgets/item_tree.py
--rw-rw-rw-   0 root         (0) root         (0)       88 2023-04-11 20:18:49.000000 NEMO-4.5.4/NEMO/wsgi.py
-drwxr-xr-x   0 root         (0) root         (0)        0 2023-04-21 23:04:43.387914 NEMO-4.5.4/NEMO.egg-info/
--rw-r--r--   0 root         (0) root         (0)      904 2023-04-21 23:04:43.000000 NEMO-4.5.4/NEMO.egg-info/PKG-INFO
--rw-r--r--   0 root         (0) root         (0)    16399 2023-04-21 23:04:43.000000 NEMO-4.5.4/NEMO.egg-info/SOURCES.txt
--rw-r--r--   0 root         (0) root         (0)        1 2023-04-21 23:04:43.000000 NEMO-4.5.4/NEMO.egg-info/dependency_links.txt
--rw-r--r--   0 root         (0) root         (0)       55 2023-04-21 23:04:43.000000 NEMO-4.5.4/NEMO.egg-info/entry_points.txt
--rw-r--r--   0 root         (0) root         (0)      263 2023-04-21 23:04:43.000000 NEMO-4.5.4/NEMO.egg-info/requires.txt
--rw-r--r--   0 root         (0) root         (0)       29 2023-04-21 23:04:43.000000 NEMO-4.5.4/NEMO.egg-info/top_level.txt
--rw-r--r--   0 root         (0) root         (0)      904 2023-04-21 23:04:43.449914 NEMO-4.5.4/PKG-INFO
--rw-rw-rw-   0 root         (0) root         (0)     4066 2023-04-18 21:38:03.000000 NEMO-4.5.4/README.md
-drwxr-xr-x   0 root         (0) root         (0)        0 2023-04-21 23:04:43.449914 NEMO-4.5.4/resources/
--rw-rw-rw-   0 root         (0) root         (0)     3957 2023-04-11 20:18:49.000000 NEMO-4.5.4/resources/splash_pad_settings.py
--rw-r--r--   0 root         (0) root         (0)      109 2023-04-21 23:04:43.450914 NEMO-4.5.4/setup.cfg
--rw-rw-rw-   0 root         (0) root         (0)     1460 2023-04-21 23:04:29.000000 NEMO-4.5.4/setup.py
+drwxr-xr-x   0 root         (0) root         (0)        0 2023-05-16 14:04:38.621849 NEMO-4.5.5/
+-rw-rw-rw-   0 root         (0) root         (0)     1865 2023-05-16 14:04:26.000000 NEMO-4.5.5/LICENSE.md
+-rw-rw-rw-   0 root         (0) root         (0)      131 2023-05-16 14:04:26.000000 NEMO-4.5.5/MANIFEST.in
+drwxr-xr-x   0 root         (0) root         (0)        0 2023-05-16 14:04:38.557849 NEMO-4.5.5/NEMO/
+-rw-rw-rw-   0 root         (0) root         (0)     1254 2023-05-16 14:04:26.000000 NEMO-4.5.5/NEMO/__init__.py
+-rw-rw-rw-   0 root         (0) root         (0)     4594 2023-05-16 14:04:26.000000 NEMO-4.5.5/NEMO/actions.py
+-rw-rw-rw-   0 root         (0) root         (0)    48729 2023-05-16 14:04:26.000000 NEMO-4.5.5/NEMO/admin.py
+drwxr-xr-x   0 root         (0) root         (0)        0 2023-05-16 14:04:38.558849 NEMO-4.5.5/NEMO/apps/
+-rw-rw-rw-   0 root         (0) root         (0)        0 2023-05-16 14:04:26.000000 NEMO-4.5.5/NEMO/apps/__init__.py
+drwxr-xr-x   0 root         (0) root         (0)        0 2023-05-16 14:04:38.559849 NEMO-4.5.5/NEMO/apps/area_access/
+-rw-rw-rw-   0 root         (0) root         (0)        0 2023-05-16 14:04:26.000000 NEMO-4.5.5/NEMO/apps/area_access/__init__.py
+drwxr-xr-x   0 root         (0) root         (0)        0 2023-05-16 14:04:38.545849 NEMO-4.5.5/NEMO/apps/area_access/static/
+drwxr-xr-x   0 root         (0) root         (0)        0 2023-05-16 14:04:38.559849 NEMO-4.5.5/NEMO/apps/area_access/static/area_access/
+-rw-rw-rw-   0 root         (0) root         (0)      304 2023-05-16 14:04:26.000000 NEMO-4.5.5/NEMO/apps/area_access/static/area_access/area_access.css
+drwxr-xr-x   0 root         (0) root         (0)        0 2023-05-16 14:04:38.545849 NEMO-4.5.5/NEMO/apps/area_access/templates/
+drwxr-xr-x   0 root         (0) root         (0)        0 2023-05-16 14:04:38.561849 NEMO-4.5.5/NEMO/apps/area_access/templates/area_access/
+-rw-rw-rw-   0 root         (0) root         (0)     1531 2023-05-16 14:04:26.000000 NEMO-4.5.5/NEMO/apps/area_access/templates/area_access/already_logged_in.html
+-rw-rw-rw-   0 root         (0) root         (0)      349 2023-05-16 14:04:26.000000 NEMO-4.5.5/NEMO/apps/area_access/templates/area_access/badge_not_found.html
+-rw-rw-rw-   0 root         (0) root         (0)     9006 2023-05-16 14:04:26.000000 NEMO-4.5.5/NEMO/apps/area_access/templates/area_access/base.html
+-rw-rw-rw-   0 root         (0) root         (0)      664 2023-05-16 14:04:26.000000 NEMO-4.5.5/NEMO/apps/area_access/templates/area_access/choose_project.html
+-rw-rw-rw-   0 root         (0) root         (0)       54 2023-05-16 14:04:26.000000 NEMO-4.5.5/NEMO/apps/area_access/templates/area_access/door_is_open.html
+-rw-rw-rw-   0 root         (0) root         (0)      236 2023-05-16 14:04:26.000000 NEMO-4.5.5/NEMO/apps/area_access/templates/area_access/farewell_screen.html
+-rw-rw-rw-   0 root         (0) root         (0)      143 2023-05-16 14:04:26.000000 NEMO-4.5.5/NEMO/apps/area_access/templates/area_access/inactive.html
+-rw-rw-rw-   0 root         (0) root         (0)      363 2023-05-16 14:04:26.000000 NEMO-4.5.5/NEMO/apps/area_access/templates/area_access/login_success.html
+-rw-rw-rw-   0 root         (0) root         (0)      244 2023-05-16 14:04:26.000000 NEMO-4.5.5/NEMO/apps/area_access/templates/area_access/logout_success.html
+-rw-rw-rw-   0 root         (0) root         (0)      666 2023-05-16 14:04:26.000000 NEMO-4.5.5/NEMO/apps/area_access/templates/area_access/logout_warning.html
+-rw-rw-rw-   0 root         (0) root         (0)      239 2023-05-16 14:04:26.000000 NEMO-4.5.5/NEMO/apps/area_access/templates/area_access/no_active_projects.html
+-rw-rw-rw-   0 root         (0) root         (0)      338 2023-05-16 14:04:26.000000 NEMO-4.5.5/NEMO/apps/area_access/templates/area_access/not_logged_in.html
+-rw-rw-rw-   0 root         (0) root         (0)      210 2023-05-16 14:04:26.000000 NEMO-4.5.5/NEMO/apps/area_access/templates/area_access/physical_access_denied.html
+-rw-rw-rw-   0 root         (0) root         (0)      566 2023-05-16 14:04:26.000000 NEMO-4.5.5/NEMO/apps/area_access/templates/area_access/resource_unavailable.html
+-rw-rw-rw-   0 root         (0) root         (0)      224 2023-05-16 14:04:26.000000 NEMO-4.5.5/NEMO/apps/area_access/templates/area_access/welcome_screen.html
+-rw-rw-rw-   0 root         (0) root         (0)      629 2023-05-16 14:04:26.000000 NEMO-4.5.5/NEMO/apps/area_access/urls.py
+-rw-rw-rw-   0 root         (0) root         (0)    12271 2023-05-16 14:04:26.000000 NEMO-4.5.5/NEMO/apps/area_access/views.py
+drwxr-xr-x   0 root         (0) root         (0)        0 2023-05-16 14:04:38.561849 NEMO-4.5.5/NEMO/apps/kiosk/
+-rw-rw-rw-   0 root         (0) root         (0)        0 2023-05-16 14:04:26.000000 NEMO-4.5.5/NEMO/apps/kiosk/__init__.py
+drwxr-xr-x   0 root         (0) root         (0)        0 2023-05-16 14:04:38.545849 NEMO-4.5.5/NEMO/apps/kiosk/static/
+drwxr-xr-x   0 root         (0) root         (0)        0 2023-05-16 14:04:38.562849 NEMO-4.5.5/NEMO/apps/kiosk/static/kiosk/
+-rw-rw-rw-   0 root         (0) root         (0)      116 2023-05-16 14:04:26.000000 NEMO-4.5.5/NEMO/apps/kiosk/static/kiosk/kiosk.css
+drwxr-xr-x   0 root         (0) root         (0)        0 2023-05-16 14:04:38.546849 NEMO-4.5.5/NEMO/apps/kiosk/templates/
+drwxr-xr-x   0 root         (0) root         (0)        0 2023-05-16 14:04:38.564849 NEMO-4.5.5/NEMO/apps/kiosk/templates/kiosk/
+-rw-rw-rw-   0 root         (0) root         (0)      170 2023-05-16 14:04:26.000000 NEMO-4.5.5/NEMO/apps/kiosk/templates/kiosk/acknowledgement.html
+-rw-rw-rw-   0 root         (0) root         (0)     2125 2023-05-16 14:04:26.000000 NEMO-4.5.5/NEMO/apps/kiosk/templates/kiosk/category_choices.html
+-rw-rw-rw-   0 root         (0) root         (0)     2012 2023-05-16 14:04:26.000000 NEMO-4.5.5/NEMO/apps/kiosk/templates/kiosk/choices.html
+-rw-rw-rw-   0 root         (0) root         (0)     1072 2023-05-16 14:04:26.000000 NEMO-4.5.5/NEMO/apps/kiosk/templates/kiosk/error.html
+-rw-rw-rw-   0 root         (0) root         (0)     2923 2023-05-16 14:04:26.000000 NEMO-4.5.5/NEMO/apps/kiosk/templates/kiosk/individual_reservation.html
+-rw-rw-rw-   0 root         (0) root         (0)    12510 2023-05-16 14:04:26.000000 NEMO-4.5.5/NEMO/apps/kiosk/templates/kiosk/kiosk.html
+-rw-rw-rw-   0 root         (0) root         (0)      901 2023-05-16 14:04:26.000000 NEMO-4.5.5/NEMO/apps/kiosk/templates/kiosk/success.html
+-rw-rw-rw-   0 root         (0) root         (0)    16575 2023-05-16 14:04:26.000000 NEMO-4.5.5/NEMO/apps/kiosk/templates/kiosk/tool_information.html
+-rw-rw-rw-   0 root         (0) root         (0)     1108 2023-05-16 14:04:26.000000 NEMO-4.5.5/NEMO/apps/kiosk/templates/kiosk/tool_project_selection_snippet.html
+-rw-rw-rw-   0 root         (0) root         (0)     4472 2023-05-16 14:04:26.000000 NEMO-4.5.5/NEMO/apps/kiosk/templates/kiosk/tool_reservation.html
+-rw-rw-rw-   0 root         (0) root         (0)     1271 2023-05-16 14:04:26.000000 NEMO-4.5.5/NEMO/apps/kiosk/urls.py
+-rw-rw-rw-   0 root         (0) root         (0)    13059 2023-05-16 14:04:26.000000 NEMO-4.5.5/NEMO/apps/kiosk/views.py
+drwxr-xr-x   0 root         (0) root         (0)        0 2023-05-16 14:04:38.565849 NEMO-4.5.5/NEMO/apps/sensors/
+-rw-rw-rw-   0 root         (0) root         (0)        0 2023-05-16 14:04:26.000000 NEMO-4.5.5/NEMO/apps/sensors/__init__.py
+-rw-rw-rw-   0 root         (0) root         (0)     7165 2023-05-16 14:04:26.000000 NEMO-4.5.5/NEMO/apps/sensors/admin.py
+-rw-rw-rw-   0 root         (0) root         (0)      539 2023-05-16 14:04:26.000000 NEMO-4.5.5/NEMO/apps/sensors/customizations.py
+-rw-rw-rw-   0 root         (0) root         (0)     5237 2023-05-16 14:04:26.000000 NEMO-4.5.5/NEMO/apps/sensors/evaluators.py
+drwxr-xr-x   0 root         (0) root         (0)        0 2023-05-16 14:04:38.565849 NEMO-4.5.5/NEMO/apps/sensors/management/
+-rw-rw-rw-   0 root         (0) root         (0)        0 2023-05-16 14:04:26.000000 NEMO-4.5.5/NEMO/apps/sensors/management/__init__.py
+drwxr-xr-x   0 root         (0) root         (0)        0 2023-05-16 14:04:38.565849 NEMO-4.5.5/NEMO/apps/sensors/management/commands/
+-rw-rw-rw-   0 root         (0) root         (0)        0 2023-05-16 14:04:26.000000 NEMO-4.5.5/NEMO/apps/sensors/management/commands/__init__.py
+-rw-rw-rw-   0 root         (0) root         (0)      278 2023-05-16 14:04:26.000000 NEMO-4.5.5/NEMO/apps/sensors/management/commands/manage_sensor_data.py
+drwxr-xr-x   0 root         (0) root         (0)        0 2023-05-16 14:04:38.566849 NEMO-4.5.5/NEMO/apps/sensors/migrations/
+-rw-rw-rw-   0 root         (0) root         (0)     7794 2023-05-16 14:04:26.000000 NEMO-4.5.5/NEMO/apps/sensors/migrations/0001_initial.py
+-rw-rw-rw-   0 root         (0) root         (0)        0 2023-05-16 14:04:26.000000 NEMO-4.5.5/NEMO/apps/sensors/migrations/__init__.py
+-rw-rw-rw-   0 root         (0) root         (0)    12955 2023-05-16 14:04:26.000000 NEMO-4.5.5/NEMO/apps/sensors/models.py
+-rw-rw-rw-   0 root         (0) root         (0)     4564 2023-05-16 14:04:26.000000 NEMO-4.5.5/NEMO/apps/sensors/sensors.py
+drwxr-xr-x   0 root         (0) root         (0)        0 2023-05-16 14:04:38.546849 NEMO-4.5.5/NEMO/apps/sensors/static/
+drwxr-xr-x   0 root         (0) root         (0)        0 2023-05-16 14:04:38.567849 NEMO-4.5.5/NEMO/apps/sensors/static/sensors/
+-rw-rw-rw-   0 root         (0) root         (0)   408236 2023-05-16 14:04:26.000000 NEMO-4.5.5/NEMO/apps/sensors/static/sensors/chart.js
+-rw-rw-rw-   0 root         (0) root         (0)   195090 2023-05-16 14:04:26.000000 NEMO-4.5.5/NEMO/apps/sensors/static/sensors/chart.min.js
+-rw-rw-rw-   0 root         (0) root         (0)     1376 2023-05-16 14:04:26.000000 NEMO-4.5.5/NEMO/apps/sensors/static/sensors/chartjs-adapter-moment.js
+-rw-rw-rw-   0 root         (0) root         (0)     7659 2023-05-16 14:04:26.000000 NEMO-4.5.5/NEMO/apps/sensors/static/sensors/daterangepicker.css
+-rw-rw-rw-   0 root         (0) root         (0)    66305 2023-05-16 14:04:26.000000 NEMO-4.5.5/NEMO/apps/sensors/static/sensors/daterangepicker.js
+-rw-rw-rw-   0 root         (0) root         (0)      608 2023-05-16 14:04:26.000000 NEMO-4.5.5/NEMO/apps/sensors/static/sensors/sensors.css
+drwxr-xr-x   0 root         (0) root         (0)        0 2023-05-16 14:04:38.546849 NEMO-4.5.5/NEMO/apps/sensors/templates/
+drwxr-xr-x   0 root         (0) root         (0)        0 2023-05-16 14:04:38.567849 NEMO-4.5.5/NEMO/apps/sensors/templates/customizations/
+-rw-rw-rw-   0 root         (0) root         (0)     3701 2023-05-16 14:04:26.000000 NEMO-4.5.5/NEMO/apps/sensors/templates/customizations/customizations_sensors.html
+drwxr-xr-x   0 root         (0) root         (0)        0 2023-05-16 14:04:38.568849 NEMO-4.5.5/NEMO/apps/sensors/templates/sensors/
+-rw-rw-rw-   0 root         (0) root         (0)      347 2023-05-16 14:04:26.000000 NEMO-4.5.5/NEMO/apps/sensors/templates/sensors/sensor_alerts.html
+-rw-rw-rw-   0 root         (0) root         (0)    15165 2023-05-16 14:04:26.000000 NEMO-4.5.5/NEMO/apps/sensors/templates/sensors/sensor_data.html
+-rw-rw-rw-   0 root         (0) root         (0)     2615 2023-05-16 14:04:26.000000 NEMO-4.5.5/NEMO/apps/sensors/templates/sensors/sensors.html
+-rw-rw-rw-   0 root         (0) root         (0)      790 2023-05-16 14:04:26.000000 NEMO-4.5.5/NEMO/apps/sensors/urls.py
+-rw-rw-rw-   0 root         (0) root         (0)     5069 2023-05-16 14:04:26.000000 NEMO-4.5.5/NEMO/apps/sensors/views.py
+-rw-rw-rw-   0 root         (0) root         (0)     3966 2023-05-16 14:04:26.000000 NEMO-4.5.5/NEMO/context_processors.py
+-rw-rw-rw-   0 root         (0) root         (0)     5778 2023-05-16 14:04:26.000000 NEMO-4.5.5/NEMO/decorators.py
+-rw-rw-rw-   0 root         (0) root         (0)     4513 2023-05-16 14:04:26.000000 NEMO-4.5.5/NEMO/exceptions.py
+-rw-rw-rw-   0 root         (0) root         (0)     3833 2023-05-16 14:04:26.000000 NEMO-4.5.5/NEMO/fields.py
+-rw-rw-rw-   0 root         (0) root         (0)    12935 2023-05-16 14:04:26.000000 NEMO-4.5.5/NEMO/forms.py
+-rw-rw-rw-   0 root         (0) root         (0)    17784 2023-05-16 14:04:26.000000 NEMO-4.5.5/NEMO/interlocks.py
+drwxr-xr-x   0 root         (0) root         (0)        0 2023-05-16 14:04:38.568849 NEMO-4.5.5/NEMO/management/
+-rw-rw-rw-   0 root         (0) root         (0)        0 2023-05-16 14:04:26.000000 NEMO-4.5.5/NEMO/management/__init__.py
+drwxr-xr-x   0 root         (0) root         (0)        0 2023-05-16 14:04:38.570849 NEMO-4.5.5/NEMO/management/commands/
+-rw-rw-rw-   0 root         (0) root         (0)        0 2023-05-16 14:04:26.000000 NEMO-4.5.5/NEMO/management/commands/__init__.py
+-rw-rw-rw-   0 root         (0) root         (0)      385 2023-05-16 14:04:26.000000 NEMO-4.5.5/NEMO/management/commands/cancel_unused_reservations.py
+-rw-rw-rw-   0 root         (0) root         (0)      382 2023-05-16 14:04:26.000000 NEMO-4.5.5/NEMO/management/commands/create_closure_alerts.py
+-rw-rw-rw-   0 root         (0) root         (0)      376 2023-05-16 14:04:26.000000 NEMO-4.5.5/NEMO/management/commands/manage_recurring_charges.py
+-rw-rw-rw-   0 root         (0) root         (0)      431 2023-05-16 14:04:26.000000 NEMO-4.5.5/NEMO/management/commands/manage_tool_qualifications.py
+-rw-rw-rw-   0 root         (0) root         (0)      417 2023-05-16 14:04:26.000000 NEMO-4.5.5/NEMO/management/commands/send_email_out_of_time_reservation_notification.py
+-rw-rw-rw-   0 root         (0) root         (0)      415 2023-05-16 14:04:26.000000 NEMO-4.5.5/NEMO/management/commands/send_email_reservation_ending_reminders.py
+-rw-rw-rw-   0 root         (0) root         (0)      408 2023-05-16 14:04:26.000000 NEMO-4.5.5/NEMO/management/commands/send_email_reservation_reminders.py
+-rw-rw-rw-   0 root         (0) root         (0)      554 2023-05-16 14:04:26.000000 NEMO-4.5.5/NEMO/management/commands/send_email_usage_reminders.py
+-rw-rw-rw-   0 root         (0) root         (0)      456 2023-05-16 14:04:26.000000 NEMO-4.5.5/NEMO/management/commands/send_email_user_access_expiration_reminders.py
+-rw-rw-rw-   0 root         (0) root         (0)      406 2023-05-16 14:04:26.000000 NEMO-4.5.5/NEMO/management/commands/send_email_weekend_access_notification.py
+-rw-rw-rw-   0 root         (0) root         (0)     5578 2023-05-16 14:04:26.000000 NEMO-4.5.5/NEMO/middleware.py
+drwxr-xr-x   0 root         (0) root         (0)        0 2023-05-16 14:04:38.575849 NEMO-4.5.5/NEMO/migrations/
+-rw-rw-rw-   0 root         (0) root         (0)    50307 2023-05-16 14:04:26.000000 NEMO-4.5.5/NEMO/migrations/0001_version_1_0_0.py
+-rw-rw-rw-   0 root         (0) root         (0)    32962 2023-05-16 14:04:26.000000 NEMO-4.5.5/NEMO/migrations/0002_version_1_0_0_squashed.py
+-rw-rw-rw-   0 root         (0) root         (0)     7988 2023-05-16 14:04:26.000000 NEMO-4.5.5/NEMO/migrations/0012_version_2_0_0_squashed.py
+-rw-rw-rw-   0 root         (0) root         (0)     9904 2023-05-16 14:04:26.000000 NEMO-4.5.5/NEMO/migrations/0020_version_3_0_0.py
+-rw-rw-rw-   0 root         (0) root         (0)     1712 2023-05-16 14:04:26.000000 NEMO-4.5.5/NEMO/migrations/0021_version_3_1_0.py
+-rw-rw-rw-   0 root         (0) root         (0)     1095 2023-05-16 14:04:26.000000 NEMO-4.5.5/NEMO/migrations/0022_version_3_3_0.py
+-rw-rw-rw-   0 root         (0) root         (0)      913 2023-05-16 14:04:26.000000 NEMO-4.5.5/NEMO/migrations/0023_badgereader.py
+-rw-rw-rw-   0 root         (0) root         (0)      705 2023-05-16 14:04:26.000000 NEMO-4.5.5/NEMO/migrations/0024_contactinformation_user.py
+-rw-rw-rw-   0 root         (0) root         (0)     2674 2023-05-16 14:04:26.000000 NEMO-4.5.5/NEMO/migrations/0025_version_3_6_0.py
+-rw-rw-rw-   0 root         (0) root         (0)     5405 2023-05-16 14:04:26.000000 NEMO-4.5.5/NEMO/migrations/0026_version_3_7_0.py
+-rw-rw-rw-   0 root         (0) root         (0)      420 2023-05-16 14:04:26.000000 NEMO-4.5.5/NEMO/migrations/0027_version_3_8_0.py
+-rw-rw-rw-   0 root         (0) root         (0)     2233 2023-05-16 14:04:26.000000 NEMO-4.5.5/NEMO/migrations/0028_version_3_9_0.py
+-rw-rw-rw-   0 root         (0) root         (0)     1127 2023-05-16 14:04:26.000000 NEMO-4.5.5/NEMO/migrations/0030_version_3_9_2.py
+-rw-rw-rw-   0 root         (0) root         (0)     2785 2023-05-16 14:04:26.000000 NEMO-4.5.5/NEMO/migrations/0031_version_3_10_0.py
+-rw-rw-rw-   0 root         (0) root         (0)     3166 2023-05-16 14:04:26.000000 NEMO-4.5.5/NEMO/migrations/0032_version_3_11_0.py
+-rw-rw-rw-   0 root         (0) root         (0)      380 2023-05-16 14:04:26.000000 NEMO-4.5.5/NEMO/migrations/0033_version_3_12_0.py
+-rw-rw-rw-   0 root         (0) root         (0)      372 2023-05-16 14:04:26.000000 NEMO-4.5.5/NEMO/migrations/0034_version_3_13_0.py
+-rw-rw-rw-   0 root         (0) root         (0)     6747 2023-05-16 14:04:26.000000 NEMO-4.5.5/NEMO/migrations/0035_version_3_14_0.py
+-rw-rw-rw-   0 root         (0) root         (0)     7792 2023-05-16 14:04:26.000000 NEMO-4.5.5/NEMO/migrations/0036_version_3_15_0.py
+-rw-rw-rw-   0 root         (0) root         (0)     3717 2023-05-16 14:04:26.000000 NEMO-4.5.5/NEMO/migrations/0037_version_3_16_0.py
+-rw-rw-rw-   0 root         (0) root         (0)      935 2023-05-16 14:04:26.000000 NEMO-4.5.5/NEMO/migrations/0038_version_4_0_0.py
+-rw-rw-rw-   0 root         (0) root         (0)     3601 2023-05-16 14:04:26.000000 NEMO-4.5.5/NEMO/migrations/0039_version_4_1_0.py
+-rw-rw-rw-   0 root         (0) root         (0)     2444 2023-05-16 14:04:26.000000 NEMO-4.5.5/NEMO/migrations/0040_version_4_2_0.py
+-rw-rw-rw-   0 root         (0) root         (0)      487 2023-05-16 14:04:26.000000 NEMO-4.5.5/NEMO/migrations/0041_version_4_2_1.py
+-rw-rw-rw-   0 root         (0) root         (0)    16454 2023-05-16 14:04:26.000000 NEMO-4.5.5/NEMO/migrations/0042_version_4_3_0.py
+-rw-rw-rw-   0 root         (0) root         (0)      524 2023-05-16 14:04:26.000000 NEMO-4.5.5/NEMO/migrations/0043_version_4_3_2.py
+-rw-rw-rw-   0 root         (0) root         (0)     5420 2023-05-16 14:04:26.000000 NEMO-4.5.5/NEMO/migrations/0044_version_4_4_0.py
+-rw-rw-rw-   0 root         (0) root         (0)    13447 2023-05-16 14:04:26.000000 NEMO-4.5.5/NEMO/migrations/0045_version_4_5_0.py
+-rw-rw-rw-   0 root         (0) root         (0)     2037 2023-05-16 14:04:26.000000 NEMO-4.5.5/NEMO/migrations/0045_version_4_5_5.py
+-rw-rw-rw-   0 root         (0) root         (0)        0 2023-05-16 14:04:26.000000 NEMO-4.5.5/NEMO/migrations/__init__.py
+-rw-rw-rw-   0 root         (0) root         (0)     2269 2023-05-16 14:04:26.000000 NEMO-4.5.5/NEMO/migrations_utils.py
+-rw-rw-rw-   0 root         (0) root         (0)     5874 2023-05-16 14:04:26.000000 NEMO-4.5.5/NEMO/mixins.py
+-rw-rw-rw-   0 root         (0) root         (0)     3855 2023-05-16 14:04:26.000000 NEMO-4.5.5/NEMO/model_tree.py
+-rw-rw-rw-   0 root         (0) root         (0)   152793 2023-05-16 14:04:26.000000 NEMO-4.5.5/NEMO/models.py
+-rw-rw-rw-   0 root         (0) root         (0)     1429 2023-05-16 14:04:26.000000 NEMO-4.5.5/NEMO/parsers.py
+-rw-rw-rw-   0 root         (0) root         (0)      870 2023-05-16 14:04:26.000000 NEMO-4.5.5/NEMO/permissions.py
+-rw-rw-rw-   0 root         (0) root         (0)    49395 2023-05-16 14:04:26.000000 NEMO-4.5.5/NEMO/policy.py
+-rw-rw-rw-   0 root         (0) root         (0)     9943 2023-05-16 14:04:26.000000 NEMO-4.5.5/NEMO/provisioning.py
+-rw-rw-rw-   0 root         (0) root         (0)     5646 2023-05-16 14:04:26.000000 NEMO-4.5.5/NEMO/rates.py
+-rw-rw-rw-   0 root         (0) root         (0)     1037 2023-05-16 14:04:26.000000 NEMO-4.5.5/NEMO/rest_filter_backend.py
+-rw-rw-rw-   0 root         (0) root         (0)     9391 2023-05-16 14:04:26.000000 NEMO-4.5.5/NEMO/serializers.py
+drwxr-xr-x   0 root         (0) root         (0)        0 2023-05-16 14:04:38.579849 NEMO-4.5.5/NEMO/static/
+drwxr-xr-x   0 root         (0) root         (0)        0 2023-05-16 14:04:38.579849 NEMO-4.5.5/NEMO/static/admin/
+drwxr-xr-x   0 root         (0) root         (0)        0 2023-05-16 14:04:38.579849 NEMO-4.5.5/NEMO/static/admin/physical_access_level/
+-rw-rw-rw-   0 root         (0) root         (0)      607 2023-05-16 14:04:26.000000 NEMO-4.5.5/NEMO/static/admin/physical_access_level/access_level.js
+drwxr-xr-x   0 root         (0) root         (0)        0 2023-05-16 14:04:38.580849 NEMO-4.5.5/NEMO/static/admin/questions_preview/
+-rw-rw-rw-   0 root         (0) root         (0)     4122 2023-05-16 14:04:26.000000 NEMO-4.5.5/NEMO/static/admin/questions_preview/questions_preview.css
+-rw-rw-rw-   0 root         (0) root         (0)     1372 2023-05-16 14:04:26.000000 NEMO-4.5.5/NEMO/static/admin/questions_preview/questions_preview.js
+drwxr-xr-x   0 root         (0) root         (0)        0 2023-05-16 14:04:38.580849 NEMO-4.5.5/NEMO/static/admin/reservation_questions/
+-rw-rw-rw-   0 root         (0) root         (0)      247 2023-05-16 14:04:26.000000 NEMO-4.5.5/NEMO/static/admin/reservation_questions/reservation_questions.js
+-rw-rw-rw-   0 root         (0) root         (0)     1225 2023-05-16 14:04:26.000000 NEMO-4.5.5/NEMO/static/admin/time_options_override.js
+drwxr-xr-x   0 root         (0) root         (0)        0 2023-05-16 14:04:38.580849 NEMO-4.5.5/NEMO/static/admin/tool/
+-rw-rw-rw-   0 root         (0) root         (0)     1437 2023-05-16 14:04:26.000000 NEMO-4.5.5/NEMO/static/admin/tool/tool.js
+-rw-rw-rw-   0 root         (0) root         (0)     1278 2023-05-16 14:04:26.000000 NEMO-4.5.5/NEMO/static/badge_reader.js
+drwxr-xr-x   0 root         (0) root         (0)        0 2023-05-16 14:04:38.548849 NEMO-4.5.5/NEMO/static/bootstrap/
+drwxr-xr-x   0 root         (0) root         (0)        0 2023-05-16 14:04:38.582849 NEMO-4.5.5/NEMO/static/bootstrap/css/
+-rw-rw-rw-   0 root         (0) root         (0)    22608 2023-05-16 14:04:26.000000 NEMO-4.5.5/NEMO/static/bootstrap/css/bootstrap-theme.css
+-rw-rw-rw-   0 root         (0) root         (0)    43339 2023-05-16 14:04:26.000000 NEMO-4.5.5/NEMO/static/bootstrap/css/bootstrap-theme.css.map
+-rw-rw-rw-   0 root         (0) root         (0)    19963 2023-05-16 14:04:26.000000 NEMO-4.5.5/NEMO/static/bootstrap/css/bootstrap-theme.min.css
+-rw-rw-rw-   0 root         (0) root         (0)   141622 2023-05-16 14:04:26.000000 NEMO-4.5.5/NEMO/static/bootstrap/css/bootstrap.css
+-rw-rw-rw-   0 root         (0) root         (0)   380986 2023-05-16 14:04:26.000000 NEMO-4.5.5/NEMO/static/bootstrap/css/bootstrap.css.map
+-rw-rw-rw-   0 root         (0) root         (0)   117305 2023-05-16 14:04:26.000000 NEMO-4.5.5/NEMO/static/bootstrap/css/bootstrap.min.css
+drwxr-xr-x   0 root         (0) root         (0)        0 2023-05-16 14:04:38.583849 NEMO-4.5.5/NEMO/static/bootstrap/fonts/
+-rw-rw-rw-   0 root         (0) root         (0)    20127 2023-05-16 14:04:26.000000 NEMO-4.5.5/NEMO/static/bootstrap/fonts/glyphicons-halflings-regular.eot
+-rw-rw-rw-   0 root         (0) root         (0)   108738 2023-05-16 14:04:26.000000 NEMO-4.5.5/NEMO/static/bootstrap/fonts/glyphicons-halflings-regular.svg
+-rw-rw-rw-   0 root         (0) root         (0)    45404 2023-05-16 14:04:26.000000 NEMO-4.5.5/NEMO/static/bootstrap/fonts/glyphicons-halflings-regular.ttf
+-rw-rw-rw-   0 root         (0) root         (0)    23424 2023-05-16 14:04:26.000000 NEMO-4.5.5/NEMO/static/bootstrap/fonts/glyphicons-halflings-regular.woff
+-rw-rw-rw-   0 root         (0) root         (0)    18028 2023-05-16 14:04:26.000000 NEMO-4.5.5/NEMO/static/bootstrap/fonts/glyphicons-halflings-regular.woff2
+drwxr-xr-x   0 root         (0) root         (0)        0 2023-05-16 14:04:38.583849 NEMO-4.5.5/NEMO/static/bootstrap/js/
+-rw-rw-rw-   0 root         (0) root         (0)    67546 2023-05-16 14:04:26.000000 NEMO-4.5.5/NEMO/static/bootstrap/js/bootstrap.js
+-rw-rw-rw-   0 root         (0) root         (0)    35951 2023-05-16 14:04:26.000000 NEMO-4.5.5/NEMO/static/bootstrap/js/bootstrap.min.js
+drwxr-xr-x   0 root         (0) root         (0)        0 2023-05-16 14:04:38.583849 NEMO-4.5.5/NEMO/static/datetimepicker/
+-rw-rw-rw-   0 root         (0) root         (0)     9020 2023-05-16 14:04:26.000000 NEMO-4.5.5/NEMO/static/datetimepicker/bootstrap-datetimepicker.css
+-rw-rw-rw-   0 root         (0) root         (0)   105978 2023-05-16 14:04:26.000000 NEMO-4.5.5/NEMO/static/datetimepicker/bootstrap-datetimepicker.js
+-rw-rw-rw-   0 root         (0) root         (0)     1150 2023-05-16 14:04:26.000000 NEMO-4.5.5/NEMO/static/favicon.ico
+drwxr-xr-x   0 root         (0) root         (0)        0 2023-05-16 14:04:38.585849 NEMO-4.5.5/NEMO/static/fullcalendar/
+-rw-rw-rw-   0 root         (0) root         (0)    28531 2023-05-16 14:04:26.000000 NEMO-4.5.5/NEMO/static/fullcalendar/fullcalendar.css
+-rw-rw-rw-   0 root         (0) root         (0)   357749 2023-05-16 14:04:26.000000 NEMO-4.5.5/NEMO/static/fullcalendar/fullcalendar.js
+-rw-rw-rw-   0 root         (0) root         (0)    13687 2023-05-16 14:04:26.000000 NEMO-4.5.5/NEMO/static/fullcalendar/fullcalendar.min.css
+-rw-rw-rw-   0 root         (0) root         (0)   168700 2023-05-16 14:04:26.000000 NEMO-4.5.5/NEMO/static/fullcalendar/fullcalendar.min.js
+drwxr-xr-x   0 root         (0) root         (0)        0 2023-05-16 14:04:38.585849 NEMO-4.5.5/NEMO/static/icons/
+-rw-rw-rw-   0 root         (0) root         (0)    24065 2023-05-16 14:04:26.000000 NEMO-4.5.5/NEMO/static/icons/agreement.png
+-rw-rw-rw-   0 root         (0) root         (0)    16685 2023-05-16 14:04:26.000000 NEMO-4.5.5/NEMO/static/icons/caution.png
+-rw-rw-rw-   0 root         (0) root         (0)     4664 2023-05-16 14:04:26.000000 NEMO-4.5.5/NEMO/static/icons/preferences.png
+-rw-rw-rw-   0 root         (0) root         (0)   247387 2023-05-16 14:04:26.000000 NEMO-4.5.5/NEMO/static/jquery.js
+-rw-rw-rw-   0 root         (0) root         (0)    84320 2023-05-16 14:04:26.000000 NEMO-4.5.5/NEMO/static/jquery.min.js
+-rw-rw-rw-   0 root         (0) root         (0)  1183392 2023-05-16 14:04:26.000000 NEMO-4.5.5/NEMO/static/jumbotron_watermark.bmp
+-rw-rw-rw-   0 root         (0) root         (0)     1017 2023-05-16 14:04:26.000000 NEMO-4.5.5/NEMO/static/mobile.js
+-rw-rw-rw-   0 root         (0) root         (0)   174603 2023-05-16 14:04:26.000000 NEMO-4.5.5/NEMO/static/moment.js
+-rw-rw-rw-   0 root         (0) root         (0)    58102 2023-05-16 14:04:26.000000 NEMO-4.5.5/NEMO/static/moment.min.js
+-rw-rw-rw-   0 root         (0) root         (0)    86041 2023-05-16 14:04:26.000000 NEMO-4.5.5/NEMO/static/moment.min.js.map
+-rw-rw-rw-   0 root         (0) root         (0)    15594 2023-05-16 14:04:26.000000 NEMO-4.5.5/NEMO/static/nemo.css
+-rw-rw-rw-   0 root         (0) root         (0)    20182 2023-05-16 14:04:26.000000 NEMO-4.5.5/NEMO/static/nemo.js
+drwxr-xr-x   0 root         (0) root         (0)        0 2023-05-16 14:04:38.586849 NEMO-4.5.5/NEMO/static/numpad/
+-rw-rw-rw-   0 root         (0) root         (0)    12285 2023-05-16 14:04:26.000000 NEMO-4.5.5/NEMO/static/numpad/custom_numpad.jquery.js
+-rw-rw-rw-   0 root         (0) root         (0)      255 2023-05-16 14:04:26.000000 NEMO-4.5.5/NEMO/static/numpad/numpad.jquery.css
+drwxr-xr-x   0 root         (0) root         (0)        0 2023-05-16 14:04:38.587849 NEMO-4.5.5/NEMO/static/pickadate/
+-rw-rw-rw-   0 root         (0) root         (0)     3795 2023-05-16 14:04:26.000000 NEMO-4.5.5/NEMO/static/pickadate/default.css
+-rw-rw-rw-   0 root         (0) root         (0)     6040 2023-05-16 14:04:26.000000 NEMO-4.5.5/NEMO/static/pickadate/default.date.css
+-rw-rw-rw-   0 root         (0) root         (0)     2785 2023-05-16 14:04:26.000000 NEMO-4.5.5/NEMO/static/pickadate/default.time.css
+-rw-rw-rw-   0 root         (0) root         (0)    48215 2023-05-16 14:04:26.000000 NEMO-4.5.5/NEMO/static/pickadate/picker.date.js
+-rw-rw-rw-   0 root         (0) root         (0)    36941 2023-05-16 14:04:26.000000 NEMO-4.5.5/NEMO/static/pickadate/picker.js
+-rw-rw-rw-   0 root         (0) root         (0)    31899 2023-05-16 14:04:26.000000 NEMO-4.5.5/NEMO/static/pickadate/picker.time.js
+-rw-rw-rw-   0 root         (0) root         (0)       25 2023-05-16 14:04:26.000000 NEMO-4.5.5/NEMO/static/robots.txt
+-rw-rw-rw-   0 root         (0) root         (0)    48446 2023-05-16 14:04:26.000000 NEMO-4.5.5/NEMO/static/typeahead.jquery.js
+-rw-rw-rw-   0 root         (0) root         (0)    20748 2023-05-16 14:04:26.000000 NEMO-4.5.5/NEMO/static/typeahead.jquery.min.js
+drwxr-xr-x   0 root         (0) root         (0)        0 2023-05-16 14:04:38.588849 NEMO-4.5.5/NEMO/static/virtualkeyboard/
+-rw-rw-rw-   0 root         (0) root         (0)   113008 2023-05-16 14:04:26.000000 NEMO-4.5.5/NEMO/static/virtualkeyboard/jquery.keyboard.js
+-rw-rw-rw-   0 root         (0) root         (0)    47325 2023-05-16 14:04:26.000000 NEMO-4.5.5/NEMO/static/virtualkeyboard/jquery.keyboard.min.js
+-rw-rw-rw-   0 root         (0) root         (0)     7848 2023-05-16 14:04:26.000000 NEMO-4.5.5/NEMO/static/virtualkeyboard/keyboard-basic.css
+-rw-rw-rw-   0 root         (0) root         (0)     5889 2023-05-16 14:04:26.000000 NEMO-4.5.5/NEMO/static/virtualkeyboard/keyboard-basic.min.css
+drwxr-xr-x   0 root         (0) root         (0)        0 2023-05-16 14:04:38.590849 NEMO-4.5.5/NEMO/templates/
+drwxr-xr-x   0 root         (0) root         (0)        0 2023-05-16 14:04:38.590849 NEMO-4.5.5/NEMO/templates/abuse/
+-rw-rw-rw-   0 root         (0) root         (0)     4059 2023-05-16 14:04:26.000000 NEMO-4.5.5/NEMO/templates/abuse/abuse.html
+-rw-rw-rw-   0 root         (0) root         (0)      580 2023-05-16 14:04:26.000000 NEMO-4.5.5/NEMO/templates/abuse/user_drill_down.html
+drwxr-xr-x   0 root         (0) root         (0)        0 2023-05-16 14:04:38.591849 NEMO-4.5.5/NEMO/templates/accounts_and_projects/
+-rw-rw-rw-   0 root         (0) root         (0)     7380 2023-05-16 14:04:26.000000 NEMO-4.5.5/NEMO/templates/accounts_and_projects/account_and_projects.html
+-rw-rw-rw-   0 root         (0) root         (0)     6415 2023-05-16 14:04:26.000000 NEMO-4.5.5/NEMO/templates/accounts_and_projects/accounts_and_projects.html
+-rw-rw-rw-   0 root         (0) root         (0)     2843 2023-05-16 14:04:26.000000 NEMO-4.5.5/NEMO/templates/accounts_and_projects/create_account.html
+-rw-rw-rw-   0 root         (0) root         (0)     5002 2023-05-16 14:04:26.000000 NEMO-4.5.5/NEMO/templates/accounts_and_projects/create_project.html
+-rw-rw-rw-   0 root         (0) root         (0)      888 2023-05-16 14:04:26.000000 NEMO-4.5.5/NEMO/templates/accounts_and_projects/documents_for_project.html
+-rw-rw-rw-   0 root         (0) root         (0)     3530 2023-05-16 14:04:26.000000 NEMO-4.5.5/NEMO/templates/accounts_and_projects/projects.html
+-rw-rw-rw-   0 root         (0) root         (0)      924 2023-05-16 14:04:26.000000 NEMO-4.5.5/NEMO/templates/accounts_and_projects/users_for_project.html
+-rw-rw-rw-   0 root         (0) root         (0)      433 2023-05-16 14:04:26.000000 NEMO-4.5.5/NEMO/templates/acknowledgement.html
+-rw-rw-rw-   0 root         (0) root         (0)     4694 2023-05-16 14:04:26.000000 NEMO-4.5.5/NEMO/templates/alerts.html
+drwxr-xr-x   0 root         (0) root         (0)        0 2023-05-16 14:04:38.593849 NEMO-4.5.5/NEMO/templates/area_access/
+-rw-rw-rw-   0 root         (0) root         (0)     2951 2023-05-16 14:04:26.000000 NEMO-4.5.5/NEMO/templates/area_access/area_access.html
+-rw-rw-rw-   0 root         (0) root         (0)     1687 2023-05-16 14:04:26.000000 NEMO-4.5.5/NEMO/templates/area_access/calendar_self_login.html
+-rw-rw-rw-   0 root         (0) root         (0)     1111 2023-05-16 14:04:26.000000 NEMO-4.5.5/NEMO/templates/area_access/change_project.html
+-rw-rw-rw-   0 root         (0) root         (0)     1141 2023-05-16 14:04:26.000000 NEMO-4.5.5/NEMO/templates/area_access/login_areas.html
+-rw-rw-rw-   0 root         (0) root         (0)     1245 2023-05-16 14:04:26.000000 NEMO-4.5.5/NEMO/templates/area_access/new_area_access_record.html
+-rw-rw-rw-   0 root         (0) root         (0)     1938 2023-05-16 14:04:26.000000 NEMO-4.5.5/NEMO/templates/area_access/new_area_access_record_details.html
+-rw-rw-rw-   0 root         (0) root         (0)     1454 2023-05-16 14:04:26.000000 NEMO-4.5.5/NEMO/templates/area_access/self_login.html
+-rw-rw-rw-   0 root         (0) root         (0)      837 2023-05-16 14:04:26.000000 NEMO-4.5.5/NEMO/templates/authorization_failed.html
+drwxr-xr-x   0 root         (0) root         (0)        0 2023-05-16 14:04:38.594849 NEMO-4.5.5/NEMO/templates/base/
+-rw-rw-rw-   0 root         (0) root         (0)      308 2023-05-16 14:04:26.000000 NEMO-4.5.5/NEMO/templates/base/footer.html
+-rw-rw-rw-   0 root         (0) root         (0)      292 2023-05-16 14:04:26.000000 NEMO-4.5.5/NEMO/templates/base/impersonate_header.html
+-rw-rw-rw-   0 root         (0) root         (0)       37 2023-05-16 14:04:26.000000 NEMO-4.5.5/NEMO/templates/base/navbar.html
+-rw-rw-rw-   0 root         (0) root         (0)     7673 2023-05-16 14:04:26.000000 NEMO-4.5.5/NEMO/templates/base/navbar_base.html
+-rw-rw-rw-   0 root         (0) root         (0)      247 2023-05-16 14:04:26.000000 NEMO-4.5.5/NEMO/templates/base/popup.html
+-rw-rw-rw-   0 root         (0) root         (0)     5811 2023-05-16 14:04:26.000000 NEMO-4.5.5/NEMO/templates/base.html
+drwxr-xr-x   0 root         (0) root         (0)        0 2023-05-16 14:04:38.596849 NEMO-4.5.5/NEMO/templates/calendar/
+-rw-rw-rw-   0 root         (0) root         (0)    24260 2023-05-16 14:04:26.000000 NEMO-4.5.5/NEMO/templates/calendar/calendar.html
+-rw-rw-rw-   0 root         (0) root         (0)     1381 2023-05-16 14:04:26.000000 NEMO-4.5.5/NEMO/templates/calendar/configuration.html
+-rw-rw-rw-   0 root         (0) root         (0)     2834 2023-05-16 14:04:26.000000 NEMO-4.5.5/NEMO/templates/calendar/configuration_helper.html
+-rw-rw-rw-   0 root         (0) root         (0)     1254 2023-05-16 14:04:26.000000 NEMO-4.5.5/NEMO/templates/calendar/policy_dialog.html
+-rw-rw-rw-   0 root         (0) root         (0)     1300 2023-05-16 14:04:26.000000 NEMO-4.5.5/NEMO/templates/calendar/project_choice.html
+-rw-rw-rw-   0 root         (0) root         (0)     1335 2023-05-16 14:04:26.000000 NEMO-4.5.5/NEMO/templates/calendar/proxy_reservation.html
+-rw-rw-rw-   0 root         (0) root         (0)     1862 2023-05-16 14:04:26.000000 NEMO-4.5.5/NEMO/templates/calendar/reservation_event_feed.html
+-rw-rw-rw-   0 root         (0) root         (0)     1619 2023-05-16 14:04:26.000000 NEMO-4.5.5/NEMO/templates/calendar/reservation_questions.html
+-rw-rw-rw-   0 root         (0) root         (0)     1285 2023-05-16 14:04:26.000000 NEMO-4.5.5/NEMO/templates/calendar/reservation_warning.html
+-rw-rw-rw-   0 root         (0) root         (0)     4094 2023-05-16 14:04:26.000000 NEMO-4.5.5/NEMO/templates/calendar/scheduled_outage_information.html
+-rw-rw-rw-   0 root         (0) root         (0)     2011 2023-05-16 14:04:26.000000 NEMO-4.5.5/NEMO/templates/calendar/specific_user_feed.html
+-rw-rw-rw-   0 root         (0) root         (0)     2543 2023-05-16 14:04:26.000000 NEMO-4.5.5/NEMO/templates/calendar/usage_event_feed.html
+-rw-rw-rw-   0 root         (0) root         (0)     6530 2023-05-16 14:04:26.000000 NEMO-4.5.5/NEMO/templates/configuration_agenda.html
+drwxr-xr-x   0 root         (0) root         (0)        0 2023-05-16 14:04:38.596849 NEMO-4.5.5/NEMO/templates/consumables/
+-rw-rw-rw-   0 root         (0) root         (0)     8048 2023-05-16 14:04:26.000000 NEMO-4.5.5/NEMO/templates/consumables/consumables.html
+-rw-rw-rw-   0 root         (0) root         (0)     1518 2023-05-16 14:04:26.000000 NEMO-4.5.5/NEMO/templates/consumables/consumables_order.html
+-rw-rw-rw-   0 root         (0) root         (0)    11695 2023-05-16 14:04:26.000000 NEMO-4.5.5/NEMO/templates/consumables/recurring_charge.html
+-rw-rw-rw-   0 root         (0) root         (0)     5491 2023-05-16 14:04:26.000000 NEMO-4.5.5/NEMO/templates/consumables/recurring_charges.html
+drwxr-xr-x   0 root         (0) root         (0)        0 2023-05-16 14:04:38.597849 NEMO-4.5.5/NEMO/templates/contact/
+-rw-rw-rw-   0 root         (0) root         (0)      692 2023-05-16 14:04:26.000000 NEMO-4.5.5/NEMO/templates/contact/contact_staff.html
+drwxr-xr-x   0 root         (0) root         (0)        0 2023-05-16 14:04:38.599849 NEMO-4.5.5/NEMO/templates/customizations/
+-rw-rw-rw-   0 root         (0) root         (0)     1848 2023-05-16 14:04:26.000000 NEMO-4.5.5/NEMO/templates/customizations/customizations.html
+-rw-rw-rw-   0 root         (0) root         (0)     2318 2023-05-16 14:04:26.000000 NEMO-4.5.5/NEMO/templates/customizations/customizations_application.html
+-rw-rw-rw-   0 root         (0) root         (0)     7799 2023-05-16 14:04:26.000000 NEMO-4.5.5/NEMO/templates/customizations/customizations_calendar.html
+-rw-rw-rw-   0 root         (0) root         (0)     7324 2023-05-16 14:04:26.000000 NEMO-4.5.5/NEMO/templates/customizations/customizations_dashboard.html
+-rw-rw-rw-   0 root         (0) root         (0)     4202 2023-05-16 14:04:26.000000 NEMO-4.5.5/NEMO/templates/customizations/customizations_emails.html
+-rw-rw-rw-   0 root         (0) root         (0)     2545 2023-05-16 14:04:26.000000 NEMO-4.5.5/NEMO/templates/customizations/customizations_interlock.html
+-rw-rw-rw-   0 root         (0) root         (0)     5553 2023-05-16 14:04:26.000000 NEMO-4.5.5/NEMO/templates/customizations/customizations_projects_and_accounts.html
+-rw-rw-rw-   0 root         (0) root         (0)     2224 2023-05-16 14:04:26.000000 NEMO-4.5.5/NEMO/templates/customizations/customizations_rates.html
+-rw-rw-rw-   0 root         (0) root         (0)     3519 2023-05-16 14:04:26.000000 NEMO-4.5.5/NEMO/templates/customizations/customizations_recurring_charges.html
+-rw-rw-rw-   0 root         (0) root         (0)     2183 2023-05-16 14:04:26.000000 NEMO-4.5.5/NEMO/templates/customizations/customizations_remote_work.html
+-rw-rw-rw-   0 root         (0) root         (0)    16712 2023-05-16 14:04:26.000000 NEMO-4.5.5/NEMO/templates/customizations/customizations_requests.html
+-rw-rw-rw-   0 root         (0) root         (0)     3678 2023-05-16 14:04:26.000000 NEMO-4.5.5/NEMO/templates/customizations/customizations_safety.html
+-rw-rw-rw-   0 root         (0) root         (0)    27806 2023-05-16 14:04:26.000000 NEMO-4.5.5/NEMO/templates/customizations/customizations_templates.html
+-rw-rw-rw-   0 root         (0) root         (0)     8661 2023-05-16 14:04:26.000000 NEMO-4.5.5/NEMO/templates/customizations/customizations_tool.html
+-rw-rw-rw-   0 root         (0) root         (0)     1731 2023-05-16 14:04:26.000000 NEMO-4.5.5/NEMO/templates/customizations/customizations_upload.html
+-rw-rw-rw-   0 root         (0) root         (0)     5214 2023-05-16 14:04:26.000000 NEMO-4.5.5/NEMO/templates/customizations/customizations_user.html
+-rw-rw-rw-   0 root         (0) root         (0)      441 2023-05-16 14:04:26.000000 NEMO-4.5.5/NEMO/templates/display_success_and_redirect.html
+drwxr-xr-x   0 root         (0) root         (0)        0 2023-05-16 14:04:38.600849 NEMO-4.5.5/NEMO/templates/email/
+-rw-rw-rw-   0 root         (0) root         (0)     7800 2023-05-16 14:04:26.000000 NEMO-4.5.5/NEMO/templates/email/compose_email.html
+-rw-rw-rw-   0 root         (0) root         (0)     3153 2023-05-16 14:04:26.000000 NEMO-4.5.5/NEMO/templates/email/email_broadcast.html
+-rw-rw-rw-   0 root         (0) root         (0)     1045 2023-05-16 14:04:26.000000 NEMO-4.5.5/NEMO/templates/email/email_form.html
+drwxr-xr-x   0 root         (0) root         (0)        0 2023-05-16 14:04:38.600849 NEMO-4.5.5/NEMO/templates/event_details/
+-rw-rw-rw-   0 root         (0) root         (0)      751 2023-05-16 14:04:26.000000 NEMO-4.5.5/NEMO/templates/event_details/area_access_details.html
+-rw-rw-rw-   0 root         (0) root         (0)     1347 2023-05-16 14:04:26.000000 NEMO-4.5.5/NEMO/templates/event_details/outage_details.html
+-rw-rw-rw-   0 root         (0) root         (0)     9603 2023-05-16 14:04:26.000000 NEMO-4.5.5/NEMO/templates/event_details/reservation_details.html
+-rw-rw-rw-   0 root         (0) root         (0)      589 2023-05-16 14:04:26.000000 NEMO-4.5.5/NEMO/templates/event_details/usage_details.html
+-rw-rw-rw-   0 root         (0) root         (0)      426 2023-05-16 14:04:26.000000 NEMO-4.5.5/NEMO/templates/facility_rules.html
+-rw-rw-rw-   0 root         (0) root         (0)     1247 2023-05-16 14:04:26.000000 NEMO-4.5.5/NEMO/templates/feedback.html
+-rw-rw-rw-   0 root         (0) root         (0)      937 2023-05-16 14:04:26.000000 NEMO-4.5.5/NEMO/templates/history.html
+-rw-rw-rw-   0 root         (0) root         (0)     1217 2023-05-16 14:04:26.000000 NEMO-4.5.5/NEMO/templates/impersonate.html
+drwxr-xr-x   0 root         (0) root         (0)        0 2023-05-16 14:04:38.600849 NEMO-4.5.5/NEMO/templates/jumbotron/
+-rw-rw-rw-   0 root         (0) root         (0)     2059 2023-05-16 14:04:26.000000 NEMO-4.5.5/NEMO/templates/jumbotron/jumbotron.html
+-rw-rw-rw-   0 root         (0) root         (0)     3635 2023-05-16 14:04:26.000000 NEMO-4.5.5/NEMO/templates/jumbotron/jumbotron_content.html
+-rw-rw-rw-   0 root         (0) root         (0)     8671 2023-05-16 14:04:26.000000 NEMO-4.5.5/NEMO/templates/landing.html
+-rw-rw-rw-   0 root         (0) root         (0)     3496 2023-05-16 14:04:26.000000 NEMO-4.5.5/NEMO/templates/login.html
+drwxr-xr-x   0 root         (0) root         (0)        0 2023-05-16 14:04:38.601849 NEMO-4.5.5/NEMO/templates/maintenance/
+-rw-rw-rw-   0 root         (0) root         (0)     1558 2023-05-16 14:04:26.000000 NEMO-4.5.5/NEMO/templates/maintenance/closed_task_details.html
+-rw-rw-rw-   0 root         (0) root         (0)     5566 2023-05-16 14:04:26.000000 NEMO-4.5.5/NEMO/templates/maintenance/maintenance.html
+-rw-rw-rw-   0 root         (0) root         (0)     7450 2023-05-16 14:04:26.000000 NEMO-4.5.5/NEMO/templates/maintenance/pending_task_details.html
+drwxr-xr-x   0 root         (0) root         (0)        0 2023-05-16 14:04:38.602849 NEMO-4.5.5/NEMO/templates/mobile/
+-rw-rw-rw-   0 root         (0) root         (0)      762 2023-05-16 14:04:26.000000 NEMO-4.5.5/NEMO/templates/mobile/cancellation_result.html
+-rw-rw-rw-   0 root         (0) root         (0)     1916 2023-05-16 14:04:26.000000 NEMO-4.5.5/NEMO/templates/mobile/choose_item.html
+-rw-rw-rw-   0 root         (0) root         (0)      453 2023-05-16 14:04:26.000000 NEMO-4.5.5/NEMO/templates/mobile/error.html
+-rw-rw-rw-   0 root         (0) root         (0)     1025 2023-05-16 14:04:26.000000 NEMO-4.5.5/NEMO/templates/mobile/individual_outage.html
+-rw-rw-rw-   0 root         (0) root         (0)     2625 2023-05-16 14:04:26.000000 NEMO-4.5.5/NEMO/templates/mobile/individual_reservation.html
+-rw-rw-rw-   0 root         (0) root         (0)     5899 2023-05-16 14:04:26.000000 NEMO-4.5.5/NEMO/templates/mobile/new_reservation.html
+-rw-rw-rw-   0 root         (0) root         (0)      313 2023-05-16 14:04:26.000000 NEMO-4.5.5/NEMO/templates/mobile/no_active_projects.html
+-rw-rw-rw-   0 root         (0) root         (0)      777 2023-05-16 14:04:26.000000 NEMO-4.5.5/NEMO/templates/mobile/reservation_success.html
+-rw-rw-rw-   0 root         (0) root         (0)     1442 2023-05-16 14:04:26.000000 NEMO-4.5.5/NEMO/templates/mobile/view_calendar.html
+drwxr-xr-x   0 root         (0) root         (0)        0 2023-05-16 14:04:38.603849 NEMO-4.5.5/NEMO/templates/news/
+-rw-rw-rw-   0 root         (0) root         (0)      981 2023-05-16 14:04:26.000000 NEMO-4.5.5/NEMO/templates/news/archived_news.html
+-rw-rw-rw-   0 root         (0) root         (0)     1027 2023-05-16 14:04:26.000000 NEMO-4.5.5/NEMO/templates/news/new_news_form.html
+-rw-rw-rw-   0 root         (0) root         (0)     1198 2023-05-16 14:04:26.000000 NEMO-4.5.5/NEMO/templates/news/news_update_form.html
+-rw-rw-rw-   0 root         (0) root         (0)     2038 2023-05-16 14:04:26.000000 NEMO-4.5.5/NEMO/templates/news/recent_news.html
+-rw-rw-rw-   0 root         (0) root         (0)      209 2023-05-16 14:04:26.000000 NEMO-4.5.5/NEMO/templates/no_project.html
+drwxr-xr-x   0 root         (0) root         (0)        0 2023-05-16 14:04:38.604849 NEMO-4.5.5/NEMO/templates/occupancy/
+-rw-rw-rw-   0 root         (0) root         (0)      408 2023-05-16 14:04:26.000000 NEMO-4.5.5/NEMO/templates/occupancy/occupancy.html
+-rw-rw-rw-   0 root         (0) root         (0)     1841 2023-05-16 14:04:26.000000 NEMO-4.5.5/NEMO/templates/occupancy/occupancy_content.html
+-rw-rw-rw-   0 root         (0) root         (0)     1147 2023-05-16 14:04:26.000000 NEMO-4.5.5/NEMO/templates/occupancy/occupancy_count.html
+drwxr-xr-x   0 root         (0) root         (0)        0 2023-05-16 14:04:38.604849 NEMO-4.5.5/NEMO/templates/pagination/
+-rw-rw-rw-   0 root         (0) root         (0)      865 2023-05-16 14:04:26.000000 NEMO-4.5.5/NEMO/templates/pagination/pagination_base.html
+-rw-rw-rw-   0 root         (0) root         (0)      521 2023-05-16 14:04:26.000000 NEMO-4.5.5/NEMO/templates/pagination/pagination_column.html
+-rw-rw-rw-   0 root         (0) root         (0)      673 2023-05-16 14:04:26.000000 NEMO-4.5.5/NEMO/templates/pagination/pagination_pages.html
+-rw-rw-rw-   0 root         (0) root         (0)      642 2023-05-16 14:04:26.000000 NEMO-4.5.5/NEMO/templates/pagination/pagination_selector.html
+-rw-rw-rw-   0 root         (0) root         (0)     2841 2023-05-16 14:04:26.000000 NEMO-4.5.5/NEMO/templates/qualifications.html
+-rw-rw-rw-   0 root         (0) root         (0)     5462 2023-05-16 14:04:26.000000 NEMO-4.5.5/NEMO/templates/refresh_sidebar_icons.html
+drwxr-xr-x   0 root         (0) root         (0)        0 2023-05-16 14:04:38.604849 NEMO-4.5.5/NEMO/templates/remote_work/
+-rw-rw-rw-   0 root         (0) root         (0)    10648 2023-05-16 14:04:26.000000 NEMO-4.5.5/NEMO/templates/remote_work/remote_work.html
+-rw-rw-rw-   0 root         (0) root         (0)     1081 2023-05-16 14:04:26.000000 NEMO-4.5.5/NEMO/templates/remote_work/remote_work_base.html
+drwxr-xr-x   0 root         (0) root         (0)        0 2023-05-16 14:04:38.605849 NEMO-4.5.5/NEMO/templates/requests/
+drwxr-xr-x   0 root         (0) root         (0)        0 2023-05-16 14:04:38.605849 NEMO-4.5.5/NEMO/templates/requests/access_requests/
+-rw-rw-rw-   0 root         (0) root         (0)     7754 2023-05-16 14:04:26.000000 NEMO-4.5.5/NEMO/templates/requests/access_requests/access_request.html
+-rw-rw-rw-   0 root         (0) root         (0)     3450 2023-05-16 14:04:26.000000 NEMO-4.5.5/NEMO/templates/requests/access_requests/access_requests.html
+-rw-rw-rw-   0 root         (0) root         (0)     3480 2023-05-16 14:04:26.000000 NEMO-4.5.5/NEMO/templates/requests/access_requests/access_requests_table.html
+drwxr-xr-x   0 root         (0) root         (0)        0 2023-05-16 14:04:38.606849 NEMO-4.5.5/NEMO/templates/requests/adjustment_requests/
+-rw-rw-rw-   0 root         (0) root         (0)     8607 2023-05-16 14:04:26.000000 NEMO-4.5.5/NEMO/templates/requests/adjustment_requests/adjustment_request.html
+-rw-rw-rw-   0 root         (0) root         (0)     3733 2023-05-16 14:04:26.000000 NEMO-4.5.5/NEMO/templates/requests/adjustment_requests/adjustment_requests.html
+-rw-rw-rw-   0 root         (0) root         (0)     7180 2023-05-16 14:04:26.000000 NEMO-4.5.5/NEMO/templates/requests/adjustment_requests/adjustment_requests_table.html
+drwxr-xr-x   0 root         (0) root         (0)        0 2023-05-16 14:04:38.606849 NEMO-4.5.5/NEMO/templates/requests/buddy_requests/
+-rw-rw-rw-   0 root         (0) root         (0)     3910 2023-05-16 14:04:26.000000 NEMO-4.5.5/NEMO/templates/requests/buddy_requests/buddy_request.html
+-rw-rw-rw-   0 root         (0) root         (0)     5602 2023-05-16 14:04:26.000000 NEMO-4.5.5/NEMO/templates/requests/buddy_requests/buddy_requests.html
+-rw-rw-rw-   0 root         (0) root         (0)     4246 2023-05-16 14:04:26.000000 NEMO-4.5.5/NEMO/templates/requests/user_requests.html
+drwxr-xr-x   0 root         (0) root         (0)        0 2023-05-16 14:04:38.606849 NEMO-4.5.5/NEMO/templates/resources/
+-rw-rw-rw-   0 root         (0) root         (0)     2950 2023-05-16 14:04:26.000000 NEMO-4.5.5/NEMO/templates/resources/modify_resource.html
+-rw-rw-rw-   0 root         (0) root         (0)     3846 2023-05-16 14:04:26.000000 NEMO-4.5.5/NEMO/templates/resources/resource_details.html
+-rw-rw-rw-   0 root         (0) root         (0)     1423 2023-05-16 14:04:26.000000 NEMO-4.5.5/NEMO/templates/resources/resources.html
+-rw-rw-rw-   0 root         (0) root         (0)     3807 2023-05-16 14:04:26.000000 NEMO-4.5.5/NEMO/templates/resources/scheduled_outage.html
+drwxr-xr-x   0 root         (0) root         (0)        0 2023-05-16 14:04:38.607849 NEMO-4.5.5/NEMO/templates/rest_framework/
+-rw-rw-rw-   0 root         (0) root         (0)     2736 2023-05-16 14:04:26.000000 NEMO-4.5.5/NEMO/templates/rest_framework/api.html
+-rw-rw-rw-   0 root         (0) root         (0)      446 2023-05-16 14:04:26.000000 NEMO-4.5.5/NEMO/templates/rest_framework/custom_error.html
+drwxr-xr-x   0 root         (0) root         (0)        0 2023-05-16 14:04:38.608849 NEMO-4.5.5/NEMO/templates/safety/
+-rw-rw-rw-   0 root         (0) root         (0)     3112 2023-05-16 14:04:26.000000 NEMO-4.5.5/NEMO/templates/safety/safety.html
+-rw-rw-rw-   0 root         (0) root         (0)     1831 2023-05-16 14:04:26.000000 NEMO-4.5.5/NEMO/templates/safety/safety_base.html
+-rw-rw-rw-   0 root         (0) root         (0)     7754 2023-05-16 14:04:26.000000 NEMO-4.5.5/NEMO/templates/safety/safety_data_sheets.html
+-rw-rw-rw-   0 root         (0) root         (0)     1990 2023-05-16 14:04:26.000000 NEMO-4.5.5/NEMO/templates/safety/safety_issues.html
+-rw-rw-rw-   0 root         (0) root         (0)     1723 2023-05-16 14:04:26.000000 NEMO-4.5.5/NEMO/templates/safety/safety_issues_create.html
+-rw-rw-rw-   0 root         (0) root         (0)     1722 2023-05-16 14:04:26.000000 NEMO-4.5.5/NEMO/templates/safety/safety_issues_resolved.html
+-rw-rw-rw-   0 root         (0) root         (0)     1762 2023-05-16 14:04:26.000000 NEMO-4.5.5/NEMO/templates/safety/safety_issues_update.html
+-rw-rw-rw-   0 root         (0) root         (0)     1713 2023-05-16 14:04:26.000000 NEMO-4.5.5/NEMO/templates/safety/safety_items.html
+drwxr-xr-x   0 root         (0) root         (0)        0 2023-05-16 14:04:38.608849 NEMO-4.5.5/NEMO/templates/snippets/
+-rw-rw-rw-   0 root         (0) root         (0)      516 2023-05-16 14:04:26.000000 NEMO-4.5.5/NEMO/templates/snippets/button.html
+-rw-rw-rw-   0 root         (0) root         (0)      904 2023-05-16 14:04:26.000000 NEMO-4.5.5/NEMO/templates/snippets/contact_person.html
+-rw-rw-rw-   0 root         (0) root         (0)     1128 2023-05-16 14:04:26.000000 NEMO-4.5.5/NEMO/templates/snippets/embedded_document.html
+-rw-rw-rw-   0 root         (0) root         (0)     1673 2023-05-16 14:04:26.000000 NEMO-4.5.5/NEMO/templates/snippets/tool_info.html
+drwxr-xr-x   0 root         (0) root         (0)        0 2023-05-16 14:04:38.609849 NEMO-4.5.5/NEMO/templates/staff_charges/
+-rw-rw-rw-   0 root         (0) root         (0)      860 2023-05-16 14:04:26.000000 NEMO-4.5.5/NEMO/templates/staff_charges/change_status.html
+-rw-rw-rw-   0 root         (0) root         (0)     1242 2023-05-16 14:04:26.000000 NEMO-4.5.5/NEMO/templates/staff_charges/choose_project.html
+-rw-rw-rw-   0 root         (0) root         (0)      498 2023-05-16 14:04:26.000000 NEMO-4.5.5/NEMO/templates/staff_charges/end_area_charge.html
+-rw-rw-rw-   0 root         (0) root         (0)     1198 2023-05-16 14:04:26.000000 NEMO-4.5.5/NEMO/templates/staff_charges/new_staff_charge.html
+-rw-rw-rw-   0 root         (0) root         (0)      953 2023-05-16 14:04:26.000000 NEMO-4.5.5/NEMO/templates/staff_charges/reminder.html
+-rw-rw-rw-   0 root         (0) root         (0)     1854 2023-05-16 14:04:26.000000 NEMO-4.5.5/NEMO/templates/staff_charges/staff_charges_base.html
+drwxr-xr-x   0 root         (0) root         (0)        0 2023-05-16 14:04:38.610849 NEMO-4.5.5/NEMO/templates/status_dashboard/
+-rw-rw-rw-   0 root         (0) root         (0)     1554 2023-05-16 14:04:26.000000 NEMO-4.5.5/NEMO/templates/status_dashboard/occupancy.html
+-rw-rw-rw-   0 root         (0) root         (0)     8659 2023-05-16 14:04:26.000000 NEMO-4.5.5/NEMO/templates/status_dashboard/staff.html
+-rw-rw-rw-   0 root         (0) root         (0)     7728 2023-05-16 14:04:26.000000 NEMO-4.5.5/NEMO/templates/status_dashboard/staff_absence.html
+-rw-rw-rw-   0 root         (0) root         (0)     5799 2023-05-16 14:04:26.000000 NEMO-4.5.5/NEMO/templates/status_dashboard/status_dashboard.html
+-rw-rw-rw-   0 root         (0) root         (0)     3557 2023-05-16 14:04:26.000000 NEMO-4.5.5/NEMO/templates/status_dashboard/tools.html
+drwxr-xr-x   0 root         (0) root         (0)        0 2023-05-16 14:04:38.610849 NEMO-4.5.5/NEMO/templates/tasks/
+-rw-rw-rw-   0 root         (0) root         (0)     2542 2023-05-16 14:04:26.000000 NEMO-4.5.5/NEMO/templates/tasks/resolve.html
+-rw-rw-rw-   0 root         (0) root         (0)     5037 2023-05-16 14:04:26.000000 NEMO-4.5.5/NEMO/templates/tasks/update.html
+drwxr-xr-x   0 root         (0) root         (0)        0 2023-05-16 14:04:38.611849 NEMO-4.5.5/NEMO/templates/tool_control/
+-rw-rw-rw-   0 root         (0) root         (0)      873 2023-05-16 14:04:26.000000 NEMO-4.5.5/NEMO/templates/tool_control/get_projects.html
+-rw-rw-rw-   0 root         (0) root         (0)      679 2023-05-16 14:04:26.000000 NEMO-4.5.5/NEMO/templates/tool_control/interlock_error.html
+-rw-rw-rw-   0 root         (0) root         (0)     3502 2023-05-16 14:04:26.000000 NEMO-4.5.5/NEMO/templates/tool_control/past_tasks_and_comments.html
+-rw-rw-rw-   0 root         (0) root         (0)     2472 2023-05-16 14:04:26.000000 NEMO-4.5.5/NEMO/templates/tool_control/qualified_users.html
+-rw-rw-rw-   0 root         (0) root         (0)    15560 2023-05-16 14:04:26.000000 NEMO-4.5.5/NEMO/templates/tool_control/tool_control.html
+-rw-rw-rw-   0 root         (0) root         (0)    36294 2023-05-16 14:04:26.000000 NEMO-4.5.5/NEMO/templates/tool_control/tool_status.html
+-rw-rw-rw-   0 root         (0) root         (0)     6142 2023-05-16 14:04:26.000000 NEMO-4.5.5/NEMO/templates/tool_control/usage_data.html
+-rw-rw-rw-   0 root         (0) root         (0)      409 2023-05-16 14:04:26.000000 NEMO-4.5.5/NEMO/templates/tool_control/use_tool_for_other.html
+drwxr-xr-x   0 root         (0) root         (0)        0 2023-05-16 14:04:38.612849 NEMO-4.5.5/NEMO/templates/training/
+-rw-rw-rw-   0 root         (0) root         (0)      512 2023-05-16 14:04:26.000000 NEMO-4.5.5/NEMO/templates/training/get_projects.html
+-rw-rw-rw-   0 root         (0) root         (0)     4964 2023-05-16 14:04:26.000000 NEMO-4.5.5/NEMO/templates/training/training.html
+-rw-rw-rw-   0 root         (0) root         (0)     1596 2023-05-16 14:04:26.000000 NEMO-4.5.5/NEMO/templates/training/training_entry.html
+drwxr-xr-x   0 root         (0) root         (0)        0 2023-05-16 14:04:38.612849 NEMO-4.5.5/NEMO/templates/usage/
+-rw-rw-rw-   0 root         (0) root         (0)     1000 2023-05-16 14:04:26.000000 NEMO-4.5.5/NEMO/templates/usage/adjustment_request_button.html
+-rw-rw-rw-   0 root         (0) root         (0)     3573 2023-05-16 14:04:26.000000 NEMO-4.5.5/NEMO/templates/usage/billing.html
+-rw-rw-rw-   0 root         (0) root         (0)     9302 2023-05-16 14:04:26.000000 NEMO-4.5.5/NEMO/templates/usage/usage.html
+-rw-rw-rw-   0 root         (0) root         (0)     6781 2023-05-16 14:04:26.000000 NEMO-4.5.5/NEMO/templates/usage/usage_base.html
+drwxr-xr-x   0 root         (0) root         (0)        0 2023-05-16 14:04:38.613849 NEMO-4.5.5/NEMO/templates/users/
+-rw-rw-rw-   0 root         (0) root         (0)    20751 2023-05-16 14:04:26.000000 NEMO-4.5.5/NEMO/templates/users/create_or_modify_user.html
+-rw-rw-rw-   0 root         (0) root         (0)     8054 2023-05-16 14:04:26.000000 NEMO-4.5.5/NEMO/templates/users/preferences.html
+-rw-rw-rw-   0 root         (0) root         (0)     3758 2023-05-16 14:04:26.000000 NEMO-4.5.5/NEMO/templates/users/safe_deactivation.html
+-rw-rw-rw-   0 root         (0) root         (0)     4160 2023-05-16 14:04:26.000000 NEMO-4.5.5/NEMO/templates/users/users.html
+drwxr-xr-x   0 root         (0) root         (0)        0 2023-05-16 14:04:38.613849 NEMO-4.5.5/NEMO/templatetags/
+-rw-rw-rw-   0 root         (0) root         (0)        0 2023-05-16 14:04:26.000000 NEMO-4.5.5/NEMO/templatetags/__init__.py
+-rw-rw-rw-   0 root         (0) root         (0)     7825 2023-05-16 14:04:26.000000 NEMO-4.5.5/NEMO/templatetags/custom_tags_and_filters.py
+-rw-rw-rw-   0 root         (0) root         (0)    25690 2023-05-16 14:04:26.000000 NEMO-4.5.5/NEMO/urls.py
+-rw-rw-rw-   0 root         (0) root         (0)    23501 2023-05-16 14:04:26.000000 NEMO-4.5.5/NEMO/utilities.py
+drwxr-xr-x   0 root         (0) root         (0)        0 2023-05-16 14:04:38.620849 NEMO-4.5.5/NEMO/views/
+-rw-rw-rw-   0 root         (0) root         (0)        0 2023-05-16 14:04:26.000000 NEMO-4.5.5/NEMO/views/__init__.py
+-rw-rw-rw-   0 root         (0) root         (0)     4308 2023-05-16 14:04:26.000000 NEMO-4.5.5/NEMO/views/abuse.py
+-rw-rw-rw-   0 root         (0) root         (0)    14736 2023-05-16 14:04:26.000000 NEMO-4.5.5/NEMO/views/access_requests.py
+-rw-rw-rw-   0 root         (0) root         (0)     8275 2023-05-16 14:04:26.000000 NEMO-4.5.5/NEMO/views/accounts_and_projects.py
+-rw-rw-rw-   0 root         (0) root         (0)    17416 2023-05-16 14:04:26.000000 NEMO-4.5.5/NEMO/views/adjustment_requests.py
+-rw-rw-rw-   0 root         (0) root         (0)     1812 2023-05-16 14:04:26.000000 NEMO-4.5.5/NEMO/views/alerts.py
+-rw-rw-rw-   0 root         (0) root         (0)    13935 2023-05-16 14:04:26.000000 NEMO-4.5.5/NEMO/views/api.py
+-rw-rw-rw-   0 root         (0) root         (0)    12115 2023-05-16 14:04:26.000000 NEMO-4.5.5/NEMO/views/api_billing.py
+-rw-rw-rw-   0 root         (0) root         (0)     2013 2023-05-16 14:04:26.000000 NEMO-4.5.5/NEMO/views/api_file_import.py
+-rw-rw-rw-   0 root         (0) root         (0)    18830 2023-05-16 14:04:26.000000 NEMO-4.5.5/NEMO/views/area_access.py
+-rw-rw-rw-   0 root         (0) root         (0)    11992 2023-05-16 14:04:26.000000 NEMO-4.5.5/NEMO/views/authentication.py
+-rw-rw-rw-   0 root         (0) root         (0)     6625 2023-05-16 14:04:26.000000 NEMO-4.5.5/NEMO/views/buddy_requests.py
+-rw-rw-rw-   0 root         (0) root         (0)    68771 2023-05-16 14:04:26.000000 NEMO-4.5.5/NEMO/views/calendar.py
+-rw-rw-rw-   0 root         (0) root         (0)     2149 2023-05-16 14:04:26.000000 NEMO-4.5.5/NEMO/views/charge_validation.py
+-rw-rw-rw-   0 root         (0) root         (0)     1867 2023-05-16 14:04:26.000000 NEMO-4.5.5/NEMO/views/configuration_agenda.py
+-rw-rw-rw-   0 root         (0) root         (0)      174 2023-05-16 14:04:26.000000 NEMO-4.5.5/NEMO/views/constants.py
+-rw-rw-rw-   0 root         (0) root         (0)    10021 2023-05-16 14:04:26.000000 NEMO-4.5.5/NEMO/views/consumables.py
+-rw-rw-rw-   0 root         (0) root         (0)      467 2023-05-16 14:04:26.000000 NEMO-4.5.5/NEMO/views/contact_staff.py
+-rw-rw-rw-   0 root         (0) root         (0)    17761 2023-05-16 14:04:26.000000 NEMO-4.5.5/NEMO/views/customization.py
+-rw-rw-rw-   0 root         (0) root         (0)     1335 2023-05-16 14:04:26.000000 NEMO-4.5.5/NEMO/views/documents.py
+-rw-rw-rw-   0 root         (0) root         (0)     9978 2023-05-16 14:04:26.000000 NEMO-4.5.5/NEMO/views/email.py
+-rw-rw-rw-   0 root         (0) root         (0)     1973 2023-05-16 14:04:26.000000 NEMO-4.5.5/NEMO/views/event_details.py
+-rw-rw-rw-   0 root         (0) root         (0)     1482 2023-05-16 14:04:26.000000 NEMO-4.5.5/NEMO/views/feedback.py
+-rw-rw-rw-   0 root         (0) root         (0)     1672 2023-05-16 14:04:26.000000 NEMO-4.5.5/NEMO/views/get_projects.py
+-rw-rw-rw-   0 root         (0) root         (0)     4168 2023-05-16 14:04:26.000000 NEMO-4.5.5/NEMO/views/history.py
+-rw-rw-rw-   0 root         (0) root         (0)     1027 2023-05-16 14:04:26.000000 NEMO-4.5.5/NEMO/views/jumbotron.py
+-rw-rw-rw-   0 root         (0) root         (0)     3293 2023-05-16 14:04:26.000000 NEMO-4.5.5/NEMO/views/landing.py
+-rw-rw-rw-   0 root         (0) root         (0)     2289 2023-05-16 14:04:26.000000 NEMO-4.5.5/NEMO/views/maintenance.py
+-rw-rw-rw-   0 root         (0) root         (0)     8059 2023-05-16 14:04:26.000000 NEMO-4.5.5/NEMO/views/mobile.py
+-rw-rw-rw-   0 root         (0) root         (0)     3356 2023-05-16 14:04:26.000000 NEMO-4.5.5/NEMO/views/news.py
+-rw-rw-rw-   0 root         (0) root         (0)     5188 2023-05-16 14:04:26.000000 NEMO-4.5.5/NEMO/views/notifications.py
+-rw-rw-rw-   0 root         (0) root         (0)     1326 2023-05-16 14:04:26.000000 NEMO-4.5.5/NEMO/views/pagination.py
+-rw-rw-rw-   0 root         (0) root         (0)     4822 2023-05-16 14:04:26.000000 NEMO-4.5.5/NEMO/views/qualifications.py
+-rw-rw-rw-   0 root         (0) root         (0)     9504 2023-05-16 14:04:26.000000 NEMO-4.5.5/NEMO/views/remote_work.py
+-rw-rw-rw-   0 root         (0) root         (0)     3700 2023-05-16 14:04:26.000000 NEMO-4.5.5/NEMO/views/resources.py
+-rw-rw-rw-   0 root         (0) root         (0)     8877 2023-05-16 14:04:26.000000 NEMO-4.5.5/NEMO/views/safety.py
+-rw-rw-rw-   0 root         (0) root         (0)      932 2023-05-16 14:04:26.000000 NEMO-4.5.5/NEMO/views/sidebar.py
+-rw-rw-rw-   0 root         (0) root         (0)    19900 2023-05-16 14:04:26.000000 NEMO-4.5.5/NEMO/views/status_dashboard.py
+-rw-rw-rw-   0 root         (0) root         (0)    12963 2023-05-16 14:04:26.000000 NEMO-4.5.5/NEMO/views/tasks.py
+-rw-rw-rw-   0 root         (0) root         (0)    23605 2023-05-16 14:04:26.000000 NEMO-4.5.5/NEMO/views/tool_control.py
+-rw-rw-rw-   0 root         (0) root         (0)     5953 2023-05-16 14:04:26.000000 NEMO-4.5.5/NEMO/views/training.py
+-rw-rw-rw-   0 root         (0) root         (0)     1909 2023-05-16 14:04:26.000000 NEMO-4.5.5/NEMO/views/tutorials.py
+-rw-rw-rw-   0 root         (0) root         (0)    18636 2023-05-16 14:04:26.000000 NEMO-4.5.5/NEMO/views/usage.py
+-rw-rw-rw-   0 root         (0) root         (0)     1049 2023-05-16 14:04:26.000000 NEMO-4.5.5/NEMO/views/user_requests.py
+-rw-rw-rw-   0 root         (0) root         (0)    20715 2023-05-16 14:04:26.000000 NEMO-4.5.5/NEMO/views/users.py
+drwxr-xr-x   0 root         (0) root         (0)        0 2023-05-16 14:04:38.621849 NEMO-4.5.5/NEMO/widgets/
+-rw-rw-rw-   0 root         (0) root         (0)        0 2023-05-16 14:04:26.000000 NEMO-4.5.5/NEMO/widgets/__init__.py
+-rw-rw-rw-   0 root         (0) root         (0)     2968 2023-05-16 14:04:26.000000 NEMO-4.5.5/NEMO/widgets/configuration_editor.py
+-rw-rw-rw-   0 root         (0) root         (0)    26360 2023-05-16 14:04:26.000000 NEMO-4.5.5/NEMO/widgets/dynamic_form.py
+-rw-rw-rw-   0 root         (0) root         (0)     8029 2023-05-16 14:04:26.000000 NEMO-4.5.5/NEMO/widgets/item_tree.py
+-rw-rw-rw-   0 root         (0) root         (0)       88 2023-05-16 14:04:26.000000 NEMO-4.5.5/NEMO/wsgi.py
+drwxr-xr-x   0 root         (0) root         (0)        0 2023-05-16 14:04:38.558849 NEMO-4.5.5/NEMO.egg-info/
+-rw-r--r--   0 root         (0) root         (0)      904 2023-05-16 14:04:38.000000 NEMO-4.5.5/NEMO.egg-info/PKG-INFO
+-rw-r--r--   0 root         (0) root         (0)    16413 2023-05-16 14:04:38.000000 NEMO-4.5.5/NEMO.egg-info/SOURCES.txt
+-rw-r--r--   0 root         (0) root         (0)        1 2023-05-16 14:04:38.000000 NEMO-4.5.5/NEMO.egg-info/dependency_links.txt
+-rw-r--r--   0 root         (0) root         (0)       55 2023-05-16 14:04:38.000000 NEMO-4.5.5/NEMO.egg-info/entry_points.txt
+-rw-r--r--   0 root         (0) root         (0)      263 2023-05-16 14:04:38.000000 NEMO-4.5.5/NEMO.egg-info/requires.txt
+-rw-r--r--   0 root         (0) root         (0)       29 2023-05-16 14:04:38.000000 NEMO-4.5.5/NEMO.egg-info/top_level.txt
+-rw-r--r--   0 root         (0) root         (0)      904 2023-05-16 14:04:38.621849 NEMO-4.5.5/PKG-INFO
+-rw-rw-rw-   0 root         (0) root         (0)     4066 2023-05-16 14:04:26.000000 NEMO-4.5.5/README.md
+drwxr-xr-x   0 root         (0) root         (0)        0 2023-05-16 14:04:38.621849 NEMO-4.5.5/resources/
+-rw-rw-rw-   0 root         (0) root         (0)     3957 2023-05-16 14:04:26.000000 NEMO-4.5.5/resources/splash_pad_settings.py
+-rw-r--r--   0 root         (0) root         (0)      109 2023-05-16 14:04:38.622849 NEMO-4.5.5/setup.cfg
+-rw-rw-rw-   0 root         (0) root         (0)     1460 2023-05-16 14:04:26.000000 NEMO-4.5.5/setup.py
```

### Comparing `NEMO-4.5.4/NEMO/__init__.py` & `NEMO-4.5.5/NEMO/__init__.py`

 * *Files identical despite different names*

### Comparing `NEMO-4.5.4/NEMO/actions.py` & `NEMO-4.5.5/NEMO/actions.py`

 * *Files identical despite different names*

### Comparing `NEMO-4.5.4/NEMO/admin.py` & `NEMO-4.5.5/NEMO/admin.py`

 * *Files identical despite different names*

### Comparing `NEMO-4.5.4/NEMO/apps/area_access/templates/area_access/already_logged_in.html` & `NEMO-4.5.5/NEMO/apps/area_access/templates/area_access/already_logged_in.html`

 * *Files identical despite different names*

### Comparing `NEMO-4.5.4/NEMO/apps/area_access/templates/area_access/base.html` & `NEMO-4.5.5/NEMO/apps/area_access/templates/area_access/base.html`

 * *Files 4% similar despite different names*

```diff
@@ -141,47 +141,34 @@
 		}
 		function try_post_catch_interlock_error(url, data)
         {
             ajax_post(url, data, function(response, status, xml_http_request) {interlock_success_callback(response, status, xml_http_request)}, function(response, status, xml_http_request) { return interlock_failure_callback(response, status, xml_http_request, url, data) });
         }
 		function just_open_the_door(badge_number)
 		{
-			let data = {
-				'door_id': {{ door.id }},
-				'badge_number': badge_number,
-				'csrfmiddlewaretoken': '{{ csrf_token }}'
-			};
+			let data = 'door_id={{ door.id }}&csrfmiddlewaretoken={{ csrf_token }}&badge_number=' + badge_number;
 			default_content_element.hide();
 			error_element.hide();
 			error_interlock_element.hide();
 			status_element.html("<h1>Opening the door...</h1>").show();
             try_post_catch_interlock_error('{% url 'open_door' door.id %}', data);
 		}
 		function enter_area(badge_number, project_id)
 		{
-			let data = {
-				'door_id': {{ door.id }},
-				'badge_number': badge_number,
-				'csrfmiddlewaretoken': '{{ csrf_token }}'
-			};
-			if(project_id)
-				data.project_id = project_id;
+            let data = 'door_id={{ door.id }}&csrfmiddlewaretoken={{ csrf_token }}&badge_number=' + badge_number;
+			if(project_id) data += '&project_id=' + project_id;
 			default_content_element.hide();
 			error_element.hide();
 			error_interlock_element.hide();
 			status_element.html("<h1>Logging you in to the {{ area }}...</h1>").show();
 			try_post_catch_interlock_error('{% url 'login_to_area' door.id %}', data);
 		}
 		function exit_area(badge_number)
 		{
-			let data = {
-				'door_id': {{ door.id }},
-				'badge_number': badge_number,
-				'csrfmiddlewaretoken': '{{ csrf_token }}'
-			};
+            let data = 'door_id={{ door.id }}&csrfmiddlewaretoken={{ csrf_token }}&badge_number=' + badge_number;
 			default_content_element.hide();
 			error_element.hide();
 			error_interlock_element.hide();
 			status_element.html("<h1>Logging you out of the {{ area }}...</h1>").show();
 			try_post_catch_interlock_error('{% url 'logout_of_area' door.id %}', data);
 		}
 		function csrf_token()
@@ -215,15 +202,15 @@
                 if (response_data["bypass_allowed"] === true)
                 {
                     bypass_button.off("click")
                     $('#bypass_text').html(response_data['action'] + " anyway");
                     bypass_button.show();
                     bypass_button.one('click', function ()
                     {
-                        data["bypass"] = 'True';
+                        data += "&bypass=True";
                         try_post_catch_interlock_error(url, data);
                     });
                 }
                 {# hook up try again button #}
                 let inter_try_again_button = $("#inter_try_again");
                 inter_try_again_button.off("click");
                 inter_try_again_button.one('click', function ()
```

### Comparing `NEMO-4.5.4/NEMO/apps/area_access/templates/area_access/choose_project.html` & `NEMO-4.5.5/NEMO/apps/area_access/templates/area_access/choose_project.html`

 * *Files identical despite different names*

### Comparing `NEMO-4.5.4/NEMO/apps/area_access/templates/area_access/logout_warning.html` & `NEMO-4.5.5/NEMO/apps/area_access/templates/area_access/logout_warning.html`

 * *Files identical despite different names*

### Comparing `NEMO-4.5.4/NEMO/apps/area_access/templates/area_access/resource_unavailable.html` & `NEMO-4.5.5/NEMO/apps/area_access/templates/area_access/resource_unavailable.html`

 * *Files identical despite different names*

### Comparing `NEMO-4.5.4/NEMO/apps/area_access/urls.py` & `NEMO-4.5.5/NEMO/apps/area_access/urls.py`

 * *Files identical despite different names*

### Comparing `NEMO-4.5.4/NEMO/apps/area_access/views.py` & `NEMO-4.5.5/NEMO/apps/area_access/views.py`

 * *Files identical despite different names*

### Comparing `NEMO-4.5.4/NEMO/apps/kiosk/templates/kiosk/category_choices.html` & `NEMO-4.5.5/NEMO/apps/kiosk/templates/kiosk/category_choices.html`

 * *Files identical despite different names*

### Comparing `NEMO-4.5.4/NEMO/apps/kiosk/templates/kiosk/choices.html` & `NEMO-4.5.5/NEMO/apps/kiosk/templates/kiosk/choices.html`

 * *Files identical despite different names*

### Comparing `NEMO-4.5.4/NEMO/apps/kiosk/templates/kiosk/error.html` & `NEMO-4.5.5/NEMO/apps/kiosk/templates/kiosk/error.html`

 * *Files identical despite different names*

### Comparing `NEMO-4.5.4/NEMO/apps/kiosk/templates/kiosk/individual_reservation.html` & `NEMO-4.5.5/NEMO/apps/kiosk/templates/kiosk/individual_reservation.html`

 * *Files identical despite different names*

### Comparing `NEMO-4.5.4/NEMO/apps/kiosk/templates/kiosk/kiosk.html` & `NEMO-4.5.5/NEMO/apps/kiosk/templates/kiosk/kiosk.html`

 * *Files 8% similar despite different names*

```diff
@@ -126,14 +126,18 @@
 			{
 				default_content_element.hide();
 				status_element.hide();
 				error_interlock_element.hide();
 				error_element.show();
 				revert(15);
 			}
+            else
+            {
+                status_element.html(response).show();
+            }
 			$("#badge_number").html("");
 			show_alerts();
 		}
 		function revert(delay)
 		{
 			clear_timeout();
 			let countdown = delay;
@@ -179,77 +183,83 @@
 			let data = {
 				'location': '{{ location }}',
 				'badge_number': badge_number
 			};
 			default_content_element.hide();
 			error_interlock_element.hide();
 			error_element.hide();
-			status_element.html("<h1>Loading choices...</h1>").show().load('{% url 'kiosk_choices' %}?' + $.param(data), undefined, load_complete);
+			status_element.html("<h1>Loading choices...</h1>").show();
+            ajax_get('{% url 'kiosk_choices' %}?' + $.param(data), undefined, load_complete);
 		}
 		function tool_information(url)
 		{
 			default_content_element.hide();
 			error_element.hide();
 			error_interlock_element.hide();
-			status_element.html("<h1>Loading tool information...</h1>").show().load(url, undefined, load_complete);
+			status_element.html("<h1>Loading tool information...</h1>").show();
+            ajax_get(url, undefined, load_complete);
 		}
 		function view_category(url)
 		{
 			default_content_element.hide();
 			error_element.hide();
 			error_interlock_element.hide();
-			status_element.html("<h1>Loading category...</h1>").show().load(url, undefined, load_complete);
+			status_element.html("<h1>Loading category...</h1>").show();
+            ajax_get(url, undefined, load_complete);
 		}
 		function tool_reservation(url)
 		{
 			default_content_element.hide();
 			error_element.hide();
 			error_interlock_element.hide();
-			let data = serialize('#tool_control');
-			status_element.html("<h1>Loading tool reservation...</h1>").show().load(url, data, load_complete);
+			let data = $('#tool_control').serialize();
+			status_element.html("<h1>Loading tool reservation...</h1>").show();
+            ajax_post(url, data, load_complete);
 		}
 		function cancel_reservation(url, reservation_id)
 		{
 			default_content_element.hide();
 			error_element.hide();
 			error_interlock_element.hide();
-            let data = serialize('#cancel_reservation_' + reservation_id);
-			status_element.html("<h1>Cancelling reservation...</h1>").show().load(url, data, load_complete);
+            let data = $('#cancel_reservation_' + reservation_id).serialize();
+			status_element.html("<h1>Cancelling reservation...</h1>").show();
+            ajax_post(url, data, load_complete);
 		}
 		function reserve_tool()
 		{
 			default_content_element.hide();
 			error_element.hide();
 			error_interlock_element.hide();
-			let data = serialize('#tool_reservation');
-			status_element.html("<h1>Reserving tool...</h1>").show().load('{% url 'reserve_tool_from_kiosk' %}', data, load_complete);
+			let data = $('#tool_reservation').serialize();
+			status_element.html("<h1>Reserving tool...</h1>").show();
+            ajax_post('{% url 'reserve_tool_from_kiosk' %}', data, load_complete);
 		}
 		function try_post_catch_interlock_error(url, data)
         {
             ajax_post(url, data, function(response, status, xml_http_request) {interlock_success_callback(response, status, xml_http_request)}, function(response, status, xml_http_request) { return interlock_failure_callback(response, status, xml_http_request, url, data) })
         }
 		function enable_tool(tool_id)
 		{
 			default_content_element.hide();
 			error_element.hide();
 			error_interlock_element.hide();
-			let data = serialize('#tool_control');
+			let data = $('#tool_control').serialize();
 			if (tool_id)
 			{
-				data['tool_id'] = tool_id;
+				data += '&tool_id=' + tool_id;
 			}
 			status_element.html("<h1>Enabling tool...</h1>").show();
 			try_post_catch_interlock_error('{% url 'enable_tool_from_kiosk' %}', data);
 		}
 		function disable_tool()
 		{
 			default_content_element.hide();
 			error_element.hide();
 			error_interlock_element.hide();
-			let data = serialize('#tool_control');
+			let data = $('#tool_control').serialize();
 			status_element.html("<h1>Disabling tool...</h1>").show();
 			try_post_catch_interlock_error('{% url 'disable_tool_from_kiosk' %}', data);
 		}
 		function interlock_success_callback(response, status, xml_http_request)
         {
             error_interlock_element.hide();
             status_element.html(response).show();
@@ -269,15 +279,15 @@
                 if (response_data["bypass_allowed"] === true)
                 {
                     bypass_button.off("click")
                     $('#bypass_text').html(response_data['action'] + " anyway");
                     bypass_button.show();
                     bypass_button.one('click', function ()
                     {
-                        data["bypass"] = 'True';
+                        data += "&bypass=True";
                         try_post_catch_interlock_error(url, data);
                     });
                 }
                 {# hook up try again button #}
                 let inter_try_again_button = $("#inter_try_again");
                 inter_try_again_button.off("click");
                 inter_try_again_button.one('click', function ()
@@ -290,15 +300,16 @@
                     }, 200);
                 });
                 {# hook up back button #}
                 let inter_back_button = $("#inter_back");
                 inter_back_button.off("click");
                 inter_back_button.one('click', function ()
                 {
-                    tool_information("{% url 'kiosk_tool_information' '11111111111' '999999999999' 'back_to_start' %}".replace('11111111111', data.tool_id).replace('999999999999', data.customer_id).replace('back_to_start', data.back));
+                    let urlParams = new URLSearchParams(data);
+                    tool_information("{% url 'kiosk_tool_information' '11111111111' '999999999999' 'back_to_start' %}".replace('11111111111', urlParams.get("tool_id")).replace('999999999999', urlParams.get("customer_id")).replace('back_to_start', urlParams.get("back")));
                 });
             }
             else
             {
                 load_complete(response, status, xml_http_request);
             }
         }
```

### Comparing `NEMO-4.5.4/NEMO/apps/kiosk/templates/kiosk/success.html` & `NEMO-4.5.5/NEMO/apps/kiosk/templates/kiosk/success.html`

 * *Files identical despite different names*

### Comparing `NEMO-4.5.4/NEMO/apps/kiosk/templates/kiosk/tool_information.html` & `NEMO-4.5.5/NEMO/apps/kiosk/templates/kiosk/tool_information.html`

 * *Files identical despite different names*

### Comparing `NEMO-4.5.4/NEMO/apps/kiosk/templates/kiosk/tool_project_selection_snippet.html` & `NEMO-4.5.5/NEMO/apps/kiosk/templates/kiosk/tool_project_selection_snippet.html`

 * *Files identical despite different names*

### Comparing `NEMO-4.5.4/NEMO/apps/kiosk/templates/kiosk/tool_reservation.html` & `NEMO-4.5.5/NEMO/apps/kiosk/templates/kiosk/tool_reservation.html`

 * *Files identical despite different names*

### Comparing `NEMO-4.5.4/NEMO/apps/kiosk/views.py` & `NEMO-4.5.5/NEMO/apps/kiosk/views.py`

 * *Files 4% similar despite different names*

```diff
@@ -1,13 +1,12 @@
 from datetime import datetime, timedelta
 from http import HTTPStatus
 
 from django.contrib.auth.decorators import login_required, permission_required
 from django.shortcuts import render
-from django.urls import reverse
 from django.utils import timezone
 from django.utils.dateparse import parse_date, parse_time
 from django.views.decorators.http import require_GET, require_POST
 
 from NEMO.decorators import synchronized
 from NEMO.exceptions import RequiredUnansweredQuestionsException
 from NEMO.models import BadgeReader, Project, Reservation, ReservationItemType, Tool, UsageEvent, User
@@ -235,46 +234,45 @@
 @permission_required("NEMO.kiosk")
 @require_GET
 def choices(request):
 	try:
 		customer = User.objects.get(badge_number=request.GET["badge_number"])
 		usage_events = (
 			UsageEvent.objects.filter(operator=customer.id, end=None)
-				.order_by("tool__name")
-				.prefetch_related("tool", "project")
+			.order_by("tool__name")
+			.prefetch_related("tool", "project")
 		)
 		tools_in_use = [u.tool.tool_or_parent_id() for u in usage_events]
 		fifteen_minutes_from_now = timezone.now() + timedelta(minutes=15)
 		tool_reservations = (
 			Reservation.objects.filter(
 				tool__isnull=False,
 				end__gt=timezone.now(),
 				user=customer,
 				missed=False,
 				cancelled=False,
 				shortened=False,
 			)
-				.exclude(tool_id__in=tools_in_use, start__lte=fifteen_minutes_from_now)
-				.exclude(ancestor__shortened=True)
-				.order_by("start")
+			.exclude(tool_id__in=tools_in_use, start__lte=fifteen_minutes_from_now)
+			.exclude(ancestor__shortened=True)
+			.order_by("start")
 		)
 	except:
 		dictionary = {
 			"message": "Your badge wasn't recognized. If you got a new one recently then we'll need to update your account. Please contact staff to resolve the problem."
 		}
 		return render(request, "kiosk/acknowledgement.html", dictionary)
 
 	categories = [
 		t[0] for t in Tool.objects.filter(visible=True).order_by("_category").values_list("_category").distinct()
 	]
 	unqualified_categories = [
 		category
 		for category in categories
-		if not customer.is_staff
-		   and not Tool.objects.filter(
+		if not customer.is_staff and not Tool.objects.filter(
 			visible=True, _category=category, id__in=customer.qualifications.all().values_list("id")
 		).exists()
 	]
 	dictionary = {
 		"now": timezone.now(),
 		"customer": customer,
 		"usage_events": list(usage_events),
@@ -345,22 +343,12 @@
 	return render(request, "kiosk/tool_information.html", dictionary)
 
 
 @login_required
 @permission_required("NEMO.kiosk")
 @require_GET
 def kiosk(request, location=None):
-	if location and Tool.objects.filter(_location=location, visible=True).exists():
-		reader_id = request.GET.get("reader_id")
-		dictionary = {
-			"location": location,
-			"badge_reader": BadgeReader.objects.get(id=reader_id) if reader_id else BadgeReader.default(),
-		}
-		return render(request, "kiosk/kiosk.html", dictionary)
-	else:
-		locations = sorted(list(set([tool.location for tool in Tool.objects.filter(visible=True) if tool.location])))
-		dictionary = {
-			"locations": [
-				{"url": reverse("kiosk", kwargs={"location": location}), "name": location} for location in locations
-			]
-		}
-		return render(request, "kiosk/location_directory.html", dictionary)
+	reader_id = request.GET.get("reader_id")
+	dictionary = {
+		"badge_reader": BadgeReader.objects.get(id=reader_id) if reader_id else BadgeReader.default(),
+	}
+	return render(request, "kiosk/kiosk.html", dictionary)
```

### Comparing `NEMO-4.5.4/NEMO/apps/sensors/admin.py` & `NEMO-4.5.5/NEMO/apps/sensors/admin.py`

 * *Files 4% similar despite different names*

```diff
@@ -192,14 +192,21 @@
 		last_data_point = obj.last_data_point()
 		return last_data_point.created_date if last_data_point else ""
 
 	@display(ordering="read_frequency", description="Read frequency")
 	def get_read_frequency(self, obj: Sensor):
 		return obj.read_frequency if obj.read_frequency != 0 else display_for_value(False, "", boolean=True)
 
+	def get_deleted_objects(self, objs, request):
+		deleted_objects = [str(obj) for obj in objs]
+		model_count = {Sensor._meta.verbose_name_plural: len(deleted_objects)}
+		perms_needed = []
+		protected = []
+		return deleted_objects, model_count, perms_needed, protected
+
 
 @register(SensorCardCategory)
 class SensorCardCategoryAdmin(admin.ModelAdmin):
 	list_display = ("name", "key")
 
 
 @register(SensorData)
@@ -224,15 +231,12 @@
 
 @register(SensorAlertLog)
 class SensorAlertLogAdmin(admin.ModelAdmin):
 	list_display = ["id", "time", "sensor", "reset", "value"]
 	list_filter = [("sensor", admin.RelatedOnlyFieldListFilter), "value", "reset"]
 	date_hierarchy = "time"
 
-	def has_delete_permission(self, request, obj=None):
-		return False
-
 	def has_add_permission(self, request):
 		return False
 
 	def has_change_permission(self, request, obj=None):
 		return False
```

### Comparing `NEMO-4.5.4/NEMO/apps/sensors/customizations.py` & `NEMO-4.5.5/NEMO/apps/sensors/customizations.py`

 * *Files identical despite different names*

### Comparing `NEMO-4.5.4/NEMO/apps/sensors/evaluators.py` & `NEMO-4.5.5/NEMO/apps/sensors/evaluators.py`

 * *Files identical despite different names*

### Comparing `NEMO-4.5.4/NEMO/apps/sensors/migrations/0001_initial.py` & `NEMO-4.5.5/NEMO/apps/sensors/migrations/0001_initial.py`

 * *Files identical despite different names*

### Comparing `NEMO-4.5.4/NEMO/apps/sensors/models.py` & `NEMO-4.5.5/NEMO/apps/sensors/models.py`

 * *Files identical despite different names*

### Comparing `NEMO-4.5.4/NEMO/apps/sensors/sensors.py` & `NEMO-4.5.5/NEMO/apps/sensors/sensors.py`

 * *Files identical despite different names*

### Comparing `NEMO-4.5.4/NEMO/apps/sensors/static/sensors/chart.js` & `NEMO-4.5.5/NEMO/apps/sensors/static/sensors/chart.js`

 * *Files identical despite different names*

### Comparing `NEMO-4.5.4/NEMO/apps/sensors/static/sensors/chart.min.js` & `NEMO-4.5.5/NEMO/apps/sensors/static/sensors/chart.min.js`

 * *Files identical despite different names*

### Comparing `NEMO-4.5.4/NEMO/apps/sensors/static/sensors/chartjs-adapter-moment.js` & `NEMO-4.5.5/NEMO/apps/sensors/static/sensors/chartjs-adapter-moment.js`

 * *Files identical despite different names*

### Comparing `NEMO-4.5.4/NEMO/apps/sensors/static/sensors/daterangepicker.css` & `NEMO-4.5.5/NEMO/apps/sensors/static/sensors/daterangepicker.css`

 * *Files identical despite different names*

### Comparing `NEMO-4.5.4/NEMO/apps/sensors/static/sensors/daterangepicker.js` & `NEMO-4.5.5/NEMO/apps/sensors/static/sensors/daterangepicker.js`

 * *Files identical despite different names*

### Comparing `NEMO-4.5.4/NEMO/apps/sensors/static/sensors/sensors.css` & `NEMO-4.5.5/NEMO/apps/sensors/static/sensors/sensors.css`

 * *Files identical despite different names*

### Comparing `NEMO-4.5.4/NEMO/apps/sensors/templates/customizations/customizations_sensors.html` & `NEMO-4.5.5/NEMO/apps/sensors/templates/customizations/customizations_sensors.html`

 * *Files identical despite different names*

### Comparing `NEMO-4.5.4/NEMO/apps/sensors/templates/sensors/sensor_data.html` & `NEMO-4.5.5/NEMO/apps/sensors/templates/sensors/sensor_data.html`

 * *Files identical despite different names*

### Comparing `NEMO-4.5.4/NEMO/apps/sensors/templates/sensors/sensors.html` & `NEMO-4.5.5/NEMO/apps/sensors/templates/sensors/sensors.html`

 * *Files identical despite different names*

### Comparing `NEMO-4.5.4/NEMO/apps/sensors/urls.py` & `NEMO-4.5.5/NEMO/apps/sensors/urls.py`

 * *Files identical despite different names*

### Comparing `NEMO-4.5.4/NEMO/apps/sensors/views.py` & `NEMO-4.5.5/NEMO/apps/sensors/views.py`

 * *Files identical despite different names*

### Comparing `NEMO-4.5.4/NEMO/context_processors.py` & `NEMO-4.5.5/NEMO/context_processors.py`

 * *Files identical despite different names*

### Comparing `NEMO-4.5.4/NEMO/decorators.py` & `NEMO-4.5.5/NEMO/decorators.py`

 * *Files identical despite different names*

### Comparing `NEMO-4.5.4/NEMO/exceptions.py` & `NEMO-4.5.5/NEMO/exceptions.py`

 * *Files identical despite different names*

### Comparing `NEMO-4.5.4/NEMO/fields.py` & `NEMO-4.5.5/NEMO/fields.py`

 * *Files identical despite different names*

### Comparing `NEMO-4.5.4/NEMO/forms.py` & `NEMO-4.5.5/NEMO/forms.py`

 * *Files identical despite different names*

### Comparing `NEMO-4.5.4/NEMO/interlocks.py` & `NEMO-4.5.5/NEMO/interlocks.py`

 * *Files identical despite different names*

### Comparing `NEMO-4.5.4/NEMO/management/commands/send_email_usage_reminders.py` & `NEMO-4.5.5/NEMO/management/commands/send_email_usage_reminders.py`

 * *Files identical despite different names*

### Comparing `NEMO-4.5.4/NEMO/middleware.py` & `NEMO-4.5.5/NEMO/middleware.py`

 * *Files identical despite different names*

### Comparing `NEMO-4.5.4/NEMO/migrations/0001_version_1_0_0.py` & `NEMO-4.5.5/NEMO/migrations/0001_version_1_0_0.py`

 * *Files identical despite different names*

### Comparing `NEMO-4.5.4/NEMO/migrations/0002_version_1_0_0_squashed.py` & `NEMO-4.5.5/NEMO/migrations/0002_version_1_0_0_squashed.py`

 * *Files identical despite different names*

### Comparing `NEMO-4.5.4/NEMO/migrations/0012_version_2_0_0_squashed.py` & `NEMO-4.5.5/NEMO/migrations/0012_version_2_0_0_squashed.py`

 * *Files identical despite different names*

### Comparing `NEMO-4.5.4/NEMO/migrations/0020_version_3_0_0.py` & `NEMO-4.5.5/NEMO/migrations/0020_version_3_0_0.py`

 * *Files identical despite different names*

### Comparing `NEMO-4.5.4/NEMO/migrations/0021_version_3_1_0.py` & `NEMO-4.5.5/NEMO/migrations/0021_version_3_1_0.py`

 * *Files identical despite different names*

### Comparing `NEMO-4.5.4/NEMO/migrations/0022_version_3_3_0.py` & `NEMO-4.5.5/NEMO/migrations/0022_version_3_3_0.py`

 * *Files identical despite different names*

### Comparing `NEMO-4.5.4/NEMO/migrations/0023_badgereader.py` & `NEMO-4.5.5/NEMO/migrations/0023_badgereader.py`

 * *Files identical despite different names*

### Comparing `NEMO-4.5.4/NEMO/migrations/0024_contactinformation_user.py` & `NEMO-4.5.5/NEMO/migrations/0024_contactinformation_user.py`

 * *Files identical despite different names*

### Comparing `NEMO-4.5.4/NEMO/migrations/0025_version_3_6_0.py` & `NEMO-4.5.5/NEMO/migrations/0025_version_3_6_0.py`

 * *Files identical despite different names*

### Comparing `NEMO-4.5.4/NEMO/migrations/0026_version_3_7_0.py` & `NEMO-4.5.5/NEMO/migrations/0026_version_3_7_0.py`

 * *Files identical despite different names*

### Comparing `NEMO-4.5.4/NEMO/migrations/0028_version_3_9_0.py` & `NEMO-4.5.5/NEMO/migrations/0028_version_3_9_0.py`

 * *Files identical despite different names*

### Comparing `NEMO-4.5.4/NEMO/migrations/0030_version_3_9_2.py` & `NEMO-4.5.5/NEMO/migrations/0030_version_3_9_2.py`

 * *Files identical despite different names*

### Comparing `NEMO-4.5.4/NEMO/migrations/0031_version_3_10_0.py` & `NEMO-4.5.5/NEMO/migrations/0031_version_3_10_0.py`

 * *Files identical despite different names*

### Comparing `NEMO-4.5.4/NEMO/migrations/0032_version_3_11_0.py` & `NEMO-4.5.5/NEMO/migrations/0032_version_3_11_0.py`

 * *Files identical despite different names*

### Comparing `NEMO-4.5.4/NEMO/migrations/0035_version_3_14_0.py` & `NEMO-4.5.5/NEMO/migrations/0035_version_3_14_0.py`

 * *Files identical despite different names*

### Comparing `NEMO-4.5.4/NEMO/migrations/0036_version_3_15_0.py` & `NEMO-4.5.5/NEMO/migrations/0036_version_3_15_0.py`

 * *Files identical despite different names*

### Comparing `NEMO-4.5.4/NEMO/migrations/0037_version_3_16_0.py` & `NEMO-4.5.5/NEMO/migrations/0037_version_3_16_0.py`

 * *Files identical despite different names*

### Comparing `NEMO-4.5.4/NEMO/migrations/0038_version_4_0_0.py` & `NEMO-4.5.5/NEMO/migrations/0038_version_4_0_0.py`

 * *Files identical despite different names*

### Comparing `NEMO-4.5.4/NEMO/migrations/0039_version_4_1_0.py` & `NEMO-4.5.5/NEMO/migrations/0039_version_4_1_0.py`

 * *Files identical despite different names*

### Comparing `NEMO-4.5.4/NEMO/migrations/0040_version_4_2_0.py` & `NEMO-4.5.5/NEMO/migrations/0040_version_4_2_0.py`

 * *Files identical despite different names*

### Comparing `NEMO-4.5.4/NEMO/migrations/0042_version_4_3_0.py` & `NEMO-4.5.5/NEMO/migrations/0042_version_4_3_0.py`

 * *Files identical despite different names*

### Comparing `NEMO-4.5.4/NEMO/migrations/0043_version_4_3_2.py` & `NEMO-4.5.5/NEMO/migrations/0043_version_4_3_2.py`

 * *Files identical despite different names*

### Comparing `NEMO-4.5.4/NEMO/migrations/0044_version_4_4_0.py` & `NEMO-4.5.5/NEMO/migrations/0044_version_4_4_0.py`

 * *Files identical despite different names*

### Comparing `NEMO-4.5.4/NEMO/migrations/0045_version_4_5_0.py` & `NEMO-4.5.5/NEMO/migrations/0045_version_4_5_0.py`

 * *Files identical despite different names*

### Comparing `NEMO-4.5.4/NEMO/migrations_utils.py` & `NEMO-4.5.5/NEMO/migrations_utils.py`

 * *Files 4% similar despite different names*

```diff
@@ -19,15 +19,15 @@
         story = News()
         story.title = f"What's new in NEMO {version}?"
         content = f"Thank you for updating to NEMO {version}.\n"
         if extra_content:
             content += extra_content + "\n"
         content += (
             f"\nClick on the following links to consult the <a href='https://github.com/usnistgov/NEMO/releases/tag/{version}' target='_blank'>Release Notes</a> "
-            f"and the <a href='https://github.com/usnistgov/NEMO/raw/{version}/documentation/NEMO_Feature_Manual.pdf' target='_blank'>Feature manual</a>"
+            f"and the <a href='https://www.nist.gov/document/nemofeaturemanualpdf' target='_blank'>Feature manual</a>"
         )
         content = f"Originally published on {migration_format_datetime(now)} by NEMO:\n" + content.strip()
         story.original_content = content
         story.created = now
         story.all_content = content
         story.last_updated = now
         story.last_update_content = content
```

### Comparing `NEMO-4.5.4/NEMO/mixins.py` & `NEMO-4.5.5/NEMO/mixins.py`

 * *Files identical despite different names*

### Comparing `NEMO-4.5.4/NEMO/model_tree.py` & `NEMO-4.5.5/NEMO/model_tree.py`

 * *Files identical despite different names*

### Comparing `NEMO-4.5.4/NEMO/models.py` & `NEMO-4.5.5/NEMO/models.py`

 * *Files 1% similar despite different names*

```diff
@@ -1352,15 +1352,15 @@
 
 	new_file = instance.document
 	if not old_file == new_file:
 		if os.path.isfile(old_file.path):
 			os.remove(old_file.path)
 
 
-class ToolQualificationGroup(BaseModel):
+class ToolQualificationGroup(SerializationByNameModel):
 	name = models.CharField(max_length=200, unique=True, help_text="The name of this tool group")
 	tools = models.ManyToManyField(Tool, blank=False)
 
 	def __str__(self):
 		return self.name
 
 
@@ -1442,14 +1442,15 @@
 	tool = models.ForeignKey(Tool, on_delete=models.CASCADE)
 	project = models.ForeignKey('Project', on_delete=models.CASCADE)
 	duration = models.PositiveIntegerField(help_text="The duration of the training session in minutes.")
 	type = models.IntegerField(choices=Type.Choices)
 	date = models.DateTimeField(default=timezone.now)
 	qualified = models.BooleanField(default=False, help_text="Indicates that after this training session the user was qualified to use the tool.")
 	validated = models.BooleanField(default=False)
+	validated_by = models.ForeignKey(User, null=True, blank=True, related_name="training_validated_set", on_delete=models.CASCADE)
 
 	class Meta:
 		ordering = ['-date']
 
 	def __str__(self):
 		return str(self.id)
 
@@ -1458,14 +1459,15 @@
 	staff_member = models.ForeignKey(User, related_name='staff_charge_actor', on_delete=models.CASCADE)
 	customer = models.ForeignKey(User, related_name='staff_charge_customer', on_delete=models.CASCADE)
 	project = models.ForeignKey('Project', on_delete=models.CASCADE)
 	start = models.DateTimeField(default=timezone.now)
 	end = models.DateTimeField(null=True, blank=True)
 	note = models.TextField(null=True, blank=True)
 	validated = models.BooleanField(default=False)
+	validated_by = models.ForeignKey(User, null=True, blank=True, related_name="staff_charge_validated_set", on_delete=models.CASCADE)
 
 	class Meta:
 		ordering = ['-start']
 
 	def __str__(self):
 		return f"Staff charge #{self.id}"
 
@@ -1599,14 +1601,15 @@
 	area = TreeForeignKey(Area, on_delete=models.CASCADE)
 	customer = models.ForeignKey(User, on_delete=models.CASCADE)
 	project = models.ForeignKey('Project', on_delete=models.CASCADE)
 	start = models.DateTimeField(default=timezone.now)
 	end = models.DateTimeField(null=True, blank=True)
 	staff_charge = models.ForeignKey(StaffCharge, blank=True, null=True, on_delete=models.CASCADE)
 	validated = models.BooleanField(default=False)
+	validated_by = models.ForeignKey(User, null=True, blank=True, related_name="area_access_validated_set", on_delete=models.CASCADE)
 
 	class Meta:
 		indexes = [
 			models.Index(fields=['end']),
 		]
 
 	def __str__(self):
@@ -1750,14 +1753,15 @@
 	shortened = models.BooleanField(default=False, help_text="Indicates that the user finished using the tool and relinquished the remaining time on their reservation. The reservation will no longer be visible on the calendar and a descendant reservation will be created in place of the existing one.")
 	descendant = models.OneToOneField('Reservation', related_name='ancestor', null=True, blank=True, on_delete=models.SET_NULL, help_text="Any time a reservation is moved or resized, the old reservation is cancelled and a new reservation with updated information takes its place. This field links the old reservation to the new one, so the history of reservation moves & changes can be easily tracked.")
 	additional_information = models.TextField(null=True, blank=True)
 	self_configuration = models.BooleanField(default=False, help_text="When checked, indicates that the user will perform their own tool configuration (instead of requesting that the staff configure it for them).")
 	title = models.TextField(default='', blank=True, max_length=200, help_text="Shows a custom title for this reservation on the calendar. Leave this field blank to display the reservation's user name as the title (which is the default behaviour).")
 	question_data = models.TextField(null=True, blank=True)
 	validated = models.BooleanField(default=False)
+	validated_by = models.ForeignKey(User, null=True, blank=True, related_name="reservation_validated_set", on_delete=models.CASCADE)
 
 	@property
 	def reservation_item(self) -> Union[Tool, Area]:
 		if self.tool:
 			return self.tool
 		elif self.area:
 			return self.area
@@ -1842,14 +1846,15 @@
 	user = models.ForeignKey(User, related_name="usage_event_user", on_delete=models.CASCADE)
 	operator = models.ForeignKey(User, related_name="usage_event_operator", on_delete=models.CASCADE)
 	project = models.ForeignKey(Project, on_delete=models.CASCADE)
 	tool = models.ForeignKey(Tool, related_name='+', on_delete=models.CASCADE)  # The related_name='+' disallows reverse lookups. Helper functions of other models should be used instead.
 	start = models.DateTimeField(default=timezone.now)
 	end = models.DateTimeField(null=True, blank=True)
 	validated = models.BooleanField(default=False)
+	validated_by = models.ForeignKey(User, null=True, blank=True, related_name="usage_event_validated_set", on_delete=models.CASCADE)
 	remote_work = models.BooleanField(default=False)
 	run_data = models.TextField(null=True, blank=True)
 
 	def duration(self):
 		return calculate_duration(self.start, self.end, "In progress")
 
 	class Meta:
@@ -1919,14 +1924,15 @@
 	customer = models.ForeignKey(User, related_name="consumable_user", help_text="The user who will use the consumable item.", on_delete=models.CASCADE)
 	merchant = models.ForeignKey(User, related_name="consumable_merchant", help_text="The staff member that performed the withdraw.", on_delete=models.CASCADE)
 	consumable = models.ForeignKey(Consumable, on_delete=models.CASCADE)
 	quantity = models.PositiveIntegerField()
 	project = models.ForeignKey(Project, help_text="The withdraw will be billed to this project.", on_delete=models.CASCADE)
 	date = models.DateTimeField(default=timezone.now, help_text="The date and time when the user withdrew the consumable.")
 	validated = models.BooleanField(default=False)
+	validated_by = models.ForeignKey(User, null=True, blank=True, related_name="consumable_withdrawal_validated_set", on_delete=models.CASCADE)
 
 	class Meta:
 		ordering = ['-date']
 
 	def clean(self):
 		errors = {}
 		if self.customer_id:
@@ -2891,30 +2897,39 @@
 
 	def get_time_difference(self) -> str:
 		if self.item and self.new_start and self.new_end:
 			previous_duration = self.item.end.replace(microsecond=0, second=0) - self.item.start.replace(microsecond=0, second=0)
 			new_duration = self.new_end - self.new_start
 			return f"+{(new_duration - previous_duration)}" if new_duration >= previous_duration else f"- {(previous_duration - new_duration)}"
 
+	def editable_charge(self) -> bool:
+		""" Returns whether the original charge is editable, i.e. if it has a changed start or end """
+		return self.item and (self.get_new_end() or self.get_new_start())
+
 	def creator_and_reply_users(self) -> List[User]:
 		result = {self.creator}
 		for reply in self.replies:
 			result.add(reply.author)
 		for manager in User.objects.filter(is_active=True, is_facility_manager=True):
 			result.add(manager)
 		return list(result)
 
 	def clean(self):
 		if not self.description:
 			raise ValidationError({"description": _("This field is required.")})
 		if self.item:
+			already_adjusted = AdjustmentRequest.objects.filter(deleted=False, item_type_id=self.item_type_id, item_id=self.item_id)
+			if self.pk:
+				already_adjusted = already_adjusted.exclude(pk=self.pk)
+			if already_adjusted.exists():
+				raise ValidationError({NON_FIELD_ERRORS: _("There is already an adjustment request for this charge")})
 			if self.new_start and self.new_end and self.new_start > self.new_end:
-				raise ValidationError({"new_end": "The end must be later than the start"})
+				raise ValidationError({"new_end": _("The end must be later than the start")})
 			if self.new_start and format_datetime(self.new_start) == format_datetime(self.item.start) and self.new_end and format_datetime(self.new_end) == format_datetime(self.item.end):
-				raise ValidationError({NON_FIELD_ERRORS: "One of the dates must be different from the original charge"})
+				raise ValidationError({NON_FIELD_ERRORS: _("One of the dates must be different from the original charge")})
 
 	class Meta:
 		ordering = ['-creation_time']
 
 
 class RequestMessage(BaseModel):
 	content_type = models.ForeignKey(ContentType, on_delete=models.CASCADE)
```

### Comparing `NEMO-4.5.4/NEMO/parsers.py` & `NEMO-4.5.5/NEMO/parsers.py`

 * *Files 20% similar despite different names*

```diff
@@ -1,8 +1,10 @@
 import csv
+import json
+from typing import Iterable, List, Union
 
 from rest_framework.exceptions import ParseError
 from rest_framework.parsers import BaseParser
 
 
 class CSVParser(BaseParser):
 	"""
@@ -22,12 +24,23 @@
 			# Read the csv into a list of rows
 			rows = csv.reader(str_data.splitlines(), dialect=csv.excel, delimiter=delimiter)
 			# First row (headers) are field names
 			header_row = next(rows)
 			# Clean them up
 			headers = [c.strip() for c in header_row] if (header_row is not None) else None
 			# Create data dict structure
-			data = [dict(zip(headers, row)) for row in rows]
+			data = [dict(zip(headers, self.check_for_related_fields(row))) for row in rows]
 			# If only one record return it as json object, otherwise return our list of json object
 			return data[0] if len(data) == 1 else data
 		except Exception as exc:
 			raise ParseError("CSV parse error - %s" % str(exc))
+
+	def check_for_related_fields(self, row: Iterable) -> Iterable:
+		return [self.to_json(item) for item in row]
+
+	def to_json(self, item: str) -> Union[str, List]:
+		if item and item.startswith("["):
+			try:
+				return json.loads(item)
+			except:
+				pass
+		return item
```

### Comparing `NEMO-4.5.4/NEMO/permissions.py` & `NEMO-4.5.5/NEMO/permissions.py`

 * *Files identical despite different names*

### Comparing `NEMO-4.5.4/NEMO/policy.py` & `NEMO-4.5.5/NEMO/policy.py`

 * *Files identical despite different names*

### Comparing `NEMO-4.5.4/NEMO/provisioning.py` & `NEMO-4.5.5/NEMO/provisioning.py`

 * *Files identical despite different names*

### Comparing `NEMO-4.5.4/NEMO/rates.py` & `NEMO-4.5.5/NEMO/rates.py`

 * *Files identical despite different names*

### Comparing `NEMO-4.5.4/NEMO/rest_filter_backend.py` & `NEMO-4.5.5/NEMO/rest_filter_backend.py`

 * *Files identical despite different names*

### Comparing `NEMO-4.5.4/NEMO/serializers.py` & `NEMO-4.5.5/NEMO/serializers.py`

 * *Files 0% similar despite different names*

```diff
@@ -90,14 +90,17 @@
 		fields = "__all__"
 
 
 class AccountSerializer(FlexFieldsSerializerMixin, ModelSerializer):
 	class Meta:
 		model = Account
 		fields = "__all__"
+		expandable_fields = {
+			"type": "NEMO.serializers.AccountTypeSerializer",
+		}
 
 
 class QualificationSerializer(FlexFieldsSerializerMixin, ModelSerializer):
 	class Meta:
 		model = Qualification
 		fields = "__all__"
 		expandable_fields = {
```

### Comparing `NEMO-4.5.4/NEMO/static/admin/physical_access_level/access_level.js` & `NEMO-4.5.5/NEMO/static/admin/physical_access_level/access_level.js`

 * *Files identical despite different names*

### Comparing `NEMO-4.5.4/NEMO/static/admin/questions_preview/questions_preview.css` & `NEMO-4.5.5/NEMO/static/admin/questions_preview/questions_preview.css`

 * *Files identical despite different names*

### Comparing `NEMO-4.5.4/NEMO/static/admin/questions_preview/questions_preview.js` & `NEMO-4.5.5/NEMO/static/admin/questions_preview/questions_preview.js`

 * *Files identical despite different names*

### Comparing `NEMO-4.5.4/NEMO/static/admin/time_options_override.js` & `NEMO-4.5.5/NEMO/static/admin/time_options_override.js`

 * *Files identical despite different names*

### Comparing `NEMO-4.5.4/NEMO/static/admin/tool/tool.js` & `NEMO-4.5.5/NEMO/static/admin/tool/tool.js`

 * *Files identical despite different names*

### Comparing `NEMO-4.5.4/NEMO/static/badge_reader.js` & `NEMO-4.5.5/NEMO/static/badge_reader.js`

 * *Files identical despite different names*

### Comparing `NEMO-4.5.4/NEMO/static/bootstrap/css/bootstrap-theme.css` & `NEMO-4.5.5/NEMO/static/bootstrap/css/bootstrap-theme.css`

 * *Files identical despite different names*

### Comparing `NEMO-4.5.4/NEMO/static/bootstrap/css/bootstrap-theme.css.map` & `NEMO-4.5.5/NEMO/static/bootstrap/css/bootstrap-theme.css.map`

 * *Files identical despite different names*

### Comparing `NEMO-4.5.4/NEMO/static/bootstrap/css/bootstrap-theme.min.css` & `NEMO-4.5.5/NEMO/static/bootstrap/css/bootstrap-theme.min.css`

 * *Files identical despite different names*

### Comparing `NEMO-4.5.4/NEMO/static/bootstrap/css/bootstrap.css` & `NEMO-4.5.5/NEMO/static/bootstrap/css/bootstrap.css`

 * *Files identical despite different names*

### Comparing `NEMO-4.5.4/NEMO/static/bootstrap/css/bootstrap.css.map` & `NEMO-4.5.5/NEMO/static/bootstrap/css/bootstrap.css.map`

 * *Files identical despite different names*

### Comparing `NEMO-4.5.4/NEMO/static/bootstrap/css/bootstrap.min.css` & `NEMO-4.5.5/NEMO/static/bootstrap/css/bootstrap.min.css`

 * *Files identical despite different names*

### Comparing `NEMO-4.5.4/NEMO/static/bootstrap/fonts/glyphicons-halflings-regular.eot` & `NEMO-4.5.5/NEMO/static/bootstrap/fonts/glyphicons-halflings-regular.eot`

 * *Files identical despite different names*

### Comparing `NEMO-4.5.4/NEMO/static/bootstrap/fonts/glyphicons-halflings-regular.svg` & `NEMO-4.5.5/NEMO/static/bootstrap/fonts/glyphicons-halflings-regular.svg`

 * *Files identical despite different names*

### Comparing `NEMO-4.5.4/NEMO/static/bootstrap/fonts/glyphicons-halflings-regular.ttf` & `NEMO-4.5.5/NEMO/static/bootstrap/fonts/glyphicons-halflings-regular.ttf`

 * *Files identical despite different names*

### Comparing `NEMO-4.5.4/NEMO/static/bootstrap/fonts/glyphicons-halflings-regular.woff` & `NEMO-4.5.5/NEMO/static/bootstrap/fonts/glyphicons-halflings-regular.woff`

 * *Files identical despite different names*

### Comparing `NEMO-4.5.4/NEMO/static/bootstrap/fonts/glyphicons-halflings-regular.woff2` & `NEMO-4.5.5/NEMO/static/bootstrap/fonts/glyphicons-halflings-regular.woff2`

 * *Files identical despite different names*

### Comparing `NEMO-4.5.4/NEMO/static/bootstrap/js/bootstrap.js` & `NEMO-4.5.5/NEMO/static/bootstrap/js/bootstrap.js`

 * *Files identical despite different names*

### Comparing `NEMO-4.5.4/NEMO/static/bootstrap/js/bootstrap.min.js` & `NEMO-4.5.5/NEMO/static/bootstrap/js/bootstrap.min.js`

 * *Files identical despite different names*

### Comparing `NEMO-4.5.4/NEMO/static/datetimepicker/bootstrap-datetimepicker.css` & `NEMO-4.5.5/NEMO/static/datetimepicker/bootstrap-datetimepicker.css`

 * *Files identical despite different names*

### Comparing `NEMO-4.5.4/NEMO/static/datetimepicker/bootstrap-datetimepicker.js` & `NEMO-4.5.5/NEMO/static/datetimepicker/bootstrap-datetimepicker.js`

 * *Files identical despite different names*

### Comparing `NEMO-4.5.4/NEMO/static/favicon.ico` & `NEMO-4.5.5/NEMO/static/favicon.ico`

 * *Files identical despite different names*

### Comparing `NEMO-4.5.4/NEMO/static/fullcalendar/fullcalendar.css` & `NEMO-4.5.5/NEMO/static/fullcalendar/fullcalendar.css`

 * *Files identical despite different names*

### Comparing `NEMO-4.5.4/NEMO/static/fullcalendar/fullcalendar.js` & `NEMO-4.5.5/NEMO/static/fullcalendar/fullcalendar.js`

 * *Files identical despite different names*

### Comparing `NEMO-4.5.4/NEMO/static/fullcalendar/fullcalendar.min.css` & `NEMO-4.5.5/NEMO/static/fullcalendar/fullcalendar.min.css`

 * *Files identical despite different names*

### Comparing `NEMO-4.5.4/NEMO/static/fullcalendar/fullcalendar.min.js` & `NEMO-4.5.5/NEMO/static/fullcalendar/fullcalendar.min.js`

 * *Files identical despite different names*

### Comparing `NEMO-4.5.4/NEMO/static/icons/agreement.png` & `NEMO-4.5.5/NEMO/static/icons/agreement.png`

 * *Files identical despite different names*

### Comparing `NEMO-4.5.4/NEMO/static/icons/caution.png` & `NEMO-4.5.5/NEMO/static/icons/caution.png`

 * *Files identical despite different names*

### Comparing `NEMO-4.5.4/NEMO/static/icons/preferences.png` & `NEMO-4.5.5/NEMO/static/icons/preferences.png`

 * *Files identical despite different names*

### Comparing `NEMO-4.5.4/NEMO/static/jquery.js` & `NEMO-4.5.5/NEMO/static/jquery.js`

 * *Files identical despite different names*

### Comparing `NEMO-4.5.4/NEMO/static/jquery.min.js` & `NEMO-4.5.5/NEMO/static/jquery.min.js`

 * *Files identical despite different names*

### Comparing `NEMO-4.5.4/NEMO/static/jumbotron_watermark.bmp` & `NEMO-4.5.5/NEMO/static/jumbotron_watermark.bmp`

 * *Files identical despite different names*

### Comparing `NEMO-4.5.4/NEMO/static/mobile.js` & `NEMO-4.5.5/NEMO/static/mobile.js`

 * *Files identical despite different names*

### Comparing `NEMO-4.5.4/NEMO/static/moment.js` & `NEMO-4.5.5/NEMO/static/moment.js`

 * *Files identical despite different names*

### Comparing `NEMO-4.5.4/NEMO/static/moment.min.js` & `NEMO-4.5.5/NEMO/static/moment.min.js`

 * *Files identical despite different names*

### Comparing `NEMO-4.5.4/NEMO/static/moment.min.js.map` & `NEMO-4.5.5/NEMO/static/moment.min.js.map`

 * *Files identical despite different names*

### Comparing `NEMO-4.5.4/NEMO/static/nemo.css` & `NEMO-4.5.5/NEMO/static/nemo.css`

 * *Files identical despite different names*

### Comparing `NEMO-4.5.4/NEMO/static/nemo.js` & `NEMO-4.5.5/NEMO/static/nemo.js`

 * *Files 2% similar despite different names*

#### js-beautify {}

```diff
@@ -569,23 +569,22 @@
     if (textarea) {
         textarea.rows = 1;
         textarea.style.height = '';
         textarea.style.height = textarea.scrollHeight + 3 + 'px';
     }
 }
 
-function set_start_end_datetime_pickers(start_jq, end_jq, properties, end_before_start) {
+function set_start_end_datetime_pickers(start_jq, end_jq, properties, set_end_date) {
     start_jq.datetimepicker(properties);
     end_jq.datetimepicker(properties);
-    if (end_before_start == null || end_before_start) {
-        let end_date_picker = end_jq.data("DateTimePicker");
-        start_jq.on("dp.change", function(e) {
-            end_date_picker.minDate(e.date);
-        });
-    }
+    let end_date_picker = end_jq.data("DateTimePicker");
+    start_jq.on("dp.change", function(e) {
+        if (set_end_date == null || !set_end_date) end_date_picker.minDate(e.date);
+        else end_date_picker.date(e.date);
+    });
 }
 
 function sort_compare(element) {
     return element.innerText.toLowerCase();
 }
 
 function sort_elements(list_element, selector, sort_function) {
```

### Comparing `NEMO-4.5.4/NEMO/static/numpad/custom_numpad.jquery.js` & `NEMO-4.5.5/NEMO/static/numpad/custom_numpad.jquery.js`

 * *Files identical despite different names*

### Comparing `NEMO-4.5.4/NEMO/static/pickadate/default.css` & `NEMO-4.5.5/NEMO/static/pickadate/default.css`

 * *Files identical despite different names*

### Comparing `NEMO-4.5.4/NEMO/static/pickadate/default.date.css` & `NEMO-4.5.5/NEMO/static/pickadate/default.date.css`

 * *Files identical despite different names*

### Comparing `NEMO-4.5.4/NEMO/static/pickadate/default.time.css` & `NEMO-4.5.5/NEMO/static/pickadate/default.time.css`

 * *Files identical despite different names*

### Comparing `NEMO-4.5.4/NEMO/static/pickadate/picker.date.js` & `NEMO-4.5.5/NEMO/static/pickadate/picker.date.js`

 * *Files identical despite different names*

### Comparing `NEMO-4.5.4/NEMO/static/pickadate/picker.js` & `NEMO-4.5.5/NEMO/static/pickadate/picker.js`

 * *Files identical despite different names*

### Comparing `NEMO-4.5.4/NEMO/static/pickadate/picker.time.js` & `NEMO-4.5.5/NEMO/static/pickadate/picker.time.js`

 * *Files identical despite different names*

### Comparing `NEMO-4.5.4/NEMO/static/typeahead.jquery.js` & `NEMO-4.5.5/NEMO/static/typeahead.jquery.js`

 * *Files identical despite different names*

### Comparing `NEMO-4.5.4/NEMO/static/typeahead.jquery.min.js` & `NEMO-4.5.5/NEMO/static/typeahead.jquery.min.js`

 * *Files identical despite different names*

### Comparing `NEMO-4.5.4/NEMO/static/virtualkeyboard/jquery.keyboard.js` & `NEMO-4.5.5/NEMO/static/virtualkeyboard/jquery.keyboard.js`

 * *Files identical despite different names*

### Comparing `NEMO-4.5.4/NEMO/static/virtualkeyboard/jquery.keyboard.min.js` & `NEMO-4.5.5/NEMO/static/virtualkeyboard/jquery.keyboard.min.js`

 * *Files identical despite different names*

### Comparing `NEMO-4.5.4/NEMO/static/virtualkeyboard/keyboard-basic.css` & `NEMO-4.5.5/NEMO/static/virtualkeyboard/keyboard-basic.css`

 * *Files identical despite different names*

### Comparing `NEMO-4.5.4/NEMO/static/virtualkeyboard/keyboard-basic.min.css` & `NEMO-4.5.5/NEMO/static/virtualkeyboard/keyboard-basic.min.css`

 * *Files identical despite different names*

### Comparing `NEMO-4.5.4/NEMO/templates/abuse/abuse.html` & `NEMO-4.5.5/NEMO/templates/abuse/abuse.html`

 * *Files identical despite different names*

### Comparing `NEMO-4.5.4/NEMO/templates/abuse/user_drill_down.html` & `NEMO-4.5.5/NEMO/templates/abuse/user_drill_down.html`

 * *Files identical despite different names*

### Comparing `NEMO-4.5.4/NEMO/templates/accounts_and_projects/account_and_projects.html` & `NEMO-4.5.5/NEMO/templates/accounts_and_projects/account_and_projects.html`

 * *Files identical despite different names*

### Comparing `NEMO-4.5.4/NEMO/templates/accounts_and_projects/accounts_and_projects.html` & `NEMO-4.5.5/NEMO/templates/accounts_and_projects/accounts_and_projects.html`

 * *Files identical despite different names*

### Comparing `NEMO-4.5.4/NEMO/templates/accounts_and_projects/create_account.html` & `NEMO-4.5.5/NEMO/templates/accounts_and_projects/create_account.html`

 * *Files identical despite different names*

### Comparing `NEMO-4.5.4/NEMO/templates/accounts_and_projects/create_project.html` & `NEMO-4.5.5/NEMO/templates/accounts_and_projects/create_project.html`

 * *Files identical despite different names*

### Comparing `NEMO-4.5.4/NEMO/templates/accounts_and_projects/documents_for_project.html` & `NEMO-4.5.5/NEMO/templates/accounts_and_projects/documents_for_project.html`

 * *Files identical despite different names*

### Comparing `NEMO-4.5.4/NEMO/templates/accounts_and_projects/projects.html` & `NEMO-4.5.5/NEMO/templates/accounts_and_projects/projects.html`

 * *Files identical despite different names*

### Comparing `NEMO-4.5.4/NEMO/templates/accounts_and_projects/users_for_project.html` & `NEMO-4.5.5/NEMO/templates/accounts_and_projects/users_for_project.html`

 * *Files identical despite different names*

### Comparing `NEMO-4.5.4/NEMO/templates/alerts.html` & `NEMO-4.5.5/NEMO/templates/alerts.html`

 * *Files identical despite different names*

### Comparing `NEMO-4.5.4/NEMO/templates/area_access/area_access.html` & `NEMO-4.5.5/NEMO/templates/area_access/area_access.html`

 * *Files identical despite different names*

### Comparing `NEMO-4.5.4/NEMO/templates/area_access/calendar_self_login.html` & `NEMO-4.5.5/NEMO/templates/area_access/calendar_self_login.html`

 * *Files identical despite different names*

### Comparing `NEMO-4.5.4/NEMO/templates/area_access/change_project.html` & `NEMO-4.5.5/NEMO/templates/area_access/change_project.html`

 * *Files identical despite different names*

### Comparing `NEMO-4.5.4/NEMO/templates/area_access/login_areas.html` & `NEMO-4.5.5/NEMO/templates/area_access/login_areas.html`

 * *Files identical despite different names*

### Comparing `NEMO-4.5.4/NEMO/templates/area_access/new_area_access_record.html` & `NEMO-4.5.5/NEMO/templates/area_access/new_area_access_record.html`

 * *Files identical despite different names*

### Comparing `NEMO-4.5.4/NEMO/templates/area_access/new_area_access_record_details.html` & `NEMO-4.5.5/NEMO/templates/area_access/new_area_access_record_details.html`

 * *Files identical despite different names*

### Comparing `NEMO-4.5.4/NEMO/templates/area_access/self_login.html` & `NEMO-4.5.5/NEMO/templates/area_access/self_login.html`

 * *Files identical despite different names*

### Comparing `NEMO-4.5.4/NEMO/templates/authorization_failed.html` & `NEMO-4.5.5/NEMO/templates/authorization_failed.html`

 * *Files identical despite different names*

### Comparing `NEMO-4.5.4/NEMO/templates/base/navbar_base.html` & `NEMO-4.5.5/NEMO/templates/base/navbar_base.html`

 * *Files 1% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 {% load static %}
 {% load custom_tags_and_filters %}
-<nav class="navbar navbar-default navbar-static-top">
+<nav class="navbar navbar-default navbar-static-top" role="navigation">
 	<div class="container">
 		<div class="navbar-header">
 			<a class="navbar-brand" href="{% url 'landing' %}">{{ site_title }}</a>
 			<button type="button" class="navbar-toggle navbar-btn" data-toggle="collapse" data-target="#site-navigation" aria-label="menu button">
 				<span class="icon-bar"></span>
 				<span class="icon-bar"></span>
 				<span class="icon-bar"></span>
@@ -80,15 +80,15 @@
 					<li class="visible-xs visible-sm"><a href="{% url 'logout' %}">Logout</a></li>
 				{% endif %}
 			</ul>
 			<ul class="nav navbar-nav navbar-right hidden-sm hidden-xs">
 				{% if user.is_staff and user.charging_staff_time %}
 					<li>
 						<p class="navbar-text">
-							<a id="staff_charge_link" href="{% url 'staff_charges' %}" style="color:red; text-decoration: none" data-toggle="tooltip" data-placement="bottom" title="{% with user.get_staff_charge as staff_charge %}You are charging staff time to {{ staff_charge.customer }} for the project named {{ staff_charge.project }} since {{ staff_charge.start }}.{% endwith %}">
+							<a id="staff_charge_link" href="{% url 'staff_charges' %}" style="color:red; text-decoration: none" data-container="body" data-toggle="tooltip" data-placement="bottom" title="{% with user.get_staff_charge as staff_charge %}You are charging staff time to {{ staff_charge.customer }} for the project named {{ staff_charge.project }} since {{ staff_charge.start }}.{% endwith %}">
 								Charging staff time
 							</a>
 						</p>
 						<script>
 							$("#staff_charge_link").tooltip();
 						</script>
 					</li>
```

### Comparing `NEMO-4.5.4/NEMO/templates/base.html` & `NEMO-4.5.5/NEMO/templates/base.html`

 * *Files identical despite different names*

### Comparing `NEMO-4.5.4/NEMO/templates/calendar/calendar.html` & `NEMO-4.5.5/NEMO/templates/calendar/calendar.html`

 * *Files identical despite different names*

### Comparing `NEMO-4.5.4/NEMO/templates/calendar/configuration.html` & `NEMO-4.5.5/NEMO/templates/calendar/configuration.html`

 * *Files identical despite different names*

### Comparing `NEMO-4.5.4/NEMO/templates/calendar/configuration_helper.html` & `NEMO-4.5.5/NEMO/templates/calendar/configuration_helper.html`

 * *Files identical despite different names*

### Comparing `NEMO-4.5.4/NEMO/templates/calendar/policy_dialog.html` & `NEMO-4.5.5/NEMO/templates/calendar/policy_dialog.html`

 * *Files identical despite different names*

### Comparing `NEMO-4.5.4/NEMO/templates/calendar/project_choice.html` & `NEMO-4.5.5/NEMO/templates/calendar/project_choice.html`

 * *Files identical despite different names*

### Comparing `NEMO-4.5.4/NEMO/templates/calendar/proxy_reservation.html` & `NEMO-4.5.5/NEMO/templates/calendar/proxy_reservation.html`

 * *Files identical despite different names*

### Comparing `NEMO-4.5.4/NEMO/templates/calendar/reservation_event_feed.html` & `NEMO-4.5.5/NEMO/templates/calendar/reservation_event_feed.html`

 * *Files identical despite different names*

### Comparing `NEMO-4.5.4/NEMO/templates/calendar/reservation_questions.html` & `NEMO-4.5.5/NEMO/templates/calendar/reservation_questions.html`

 * *Files identical despite different names*

### Comparing `NEMO-4.5.4/NEMO/templates/calendar/reservation_warning.html` & `NEMO-4.5.5/NEMO/templates/calendar/reservation_warning.html`

 * *Files identical despite different names*

### Comparing `NEMO-4.5.4/NEMO/templates/calendar/scheduled_outage_information.html` & `NEMO-4.5.5/NEMO/templates/calendar/scheduled_outage_information.html`

 * *Files identical despite different names*

### Comparing `NEMO-4.5.4/NEMO/templates/calendar/specific_user_feed.html` & `NEMO-4.5.5/NEMO/templates/calendar/specific_user_feed.html`

 * *Files identical despite different names*

### Comparing `NEMO-4.5.4/NEMO/templates/calendar/usage_event_feed.html` & `NEMO-4.5.5/NEMO/templates/calendar/usage_event_feed.html`

 * *Files identical despite different names*

### Comparing `NEMO-4.5.4/NEMO/templates/configuration_agenda.html` & `NEMO-4.5.5/NEMO/templates/configuration_agenda.html`

 * *Files identical despite different names*

### Comparing `NEMO-4.5.4/NEMO/templates/consumables/consumables.html` & `NEMO-4.5.5/NEMO/templates/consumables/consumables.html`

 * *Files identical despite different names*

### Comparing `NEMO-4.5.4/NEMO/templates/consumables/consumables_order.html` & `NEMO-4.5.5/NEMO/templates/consumables/consumables_order.html`

 * *Files identical despite different names*

### Comparing `NEMO-4.5.4/NEMO/templates/consumables/recurring_charge.html` & `NEMO-4.5.5/NEMO/templates/consumables/recurring_charge.html`

 * *Files identical despite different names*

### Comparing `NEMO-4.5.4/NEMO/templates/consumables/recurring_charges.html` & `NEMO-4.5.5/NEMO/templates/consumables/recurring_charges.html`

 * *Files identical despite different names*

### Comparing `NEMO-4.5.4/NEMO/templates/contact/contact_staff.html` & `NEMO-4.5.5/NEMO/templates/contact/contact_staff.html`

 * *Files identical despite different names*

### Comparing `NEMO-4.5.4/NEMO/templates/customizations/customizations.html` & `NEMO-4.5.5/NEMO/templates/customizations/customizations.html`

 * *Files identical despite different names*

### Comparing `NEMO-4.5.4/NEMO/templates/customizations/customizations_application.html` & `NEMO-4.5.5/NEMO/templates/customizations/customizations_application.html`

 * *Files identical despite different names*

### Comparing `NEMO-4.5.4/NEMO/templates/customizations/customizations_calendar.html` & `NEMO-4.5.5/NEMO/templates/customizations/customizations_calendar.html`

 * *Files identical despite different names*

### Comparing `NEMO-4.5.4/NEMO/templates/customizations/customizations_dashboard.html` & `NEMO-4.5.5/NEMO/templates/customizations/customizations_dashboard.html`

 * *Files identical despite different names*

### Comparing `NEMO-4.5.4/NEMO/templates/customizations/customizations_emails.html` & `NEMO-4.5.5/NEMO/templates/customizations/customizations_emails.html`

 * *Files identical despite different names*

### Comparing `NEMO-4.5.4/NEMO/templates/customizations/customizations_interlock.html` & `NEMO-4.5.5/NEMO/templates/customizations/customizations_interlock.html`

 * *Files identical despite different names*

### Comparing `NEMO-4.5.4/NEMO/templates/customizations/customizations_projects_and_accounts.html` & `NEMO-4.5.5/NEMO/templates/customizations/customizations_projects_and_accounts.html`

 * *Files identical despite different names*

### Comparing `NEMO-4.5.4/NEMO/templates/customizations/customizations_rates.html` & `NEMO-4.5.5/NEMO/templates/customizations/customizations_rates.html`

 * *Files identical despite different names*

### Comparing `NEMO-4.5.4/NEMO/templates/customizations/customizations_recurring_charges.html` & `NEMO-4.5.5/NEMO/templates/customizations/customizations_recurring_charges.html`

 * *Files identical despite different names*

### Comparing `NEMO-4.5.4/NEMO/templates/customizations/customizations_remote_work.html` & `NEMO-4.5.5/NEMO/templates/customizations/customizations_remote_work.html`

 * *Files identical despite different names*

### Comparing `NEMO-4.5.4/NEMO/templates/customizations/customizations_requests.html` & `NEMO-4.5.5/NEMO/templates/customizations/customizations_requests.html`

 * *Files 2% similar despite different names*

```diff
@@ -112,14 +112,25 @@
                 {% elif errors.adjustment_requests_time_limit_frequency %}
                     {{ errors.adjustment_requests_time_limit_frequency.error }}
                 {% else %}
                     The timeframe for users to be able to request adjustment on charges.
                 {% endif %}
             </div>
         </div>
+        <div class="form-group">
+            <label class="control-label col-md-4">Approved charges</label>
+            <div class="col-md-8">
+                <div class="checkbox">
+                    <label><input type="checkbox" name="adjustment_requests_edit_charge_button" {% if adjustment_requests_edit_charge_button %}checked{% endif %} value="enabled">Check this box to show a link to edit the original charge after approval</label><br/>
+                </div>
+            </div>
+            <div class="col-md-offset-4 col-md-8 help-block light-grey">
+                This does not apply to general charges.
+            </div>
+        </div>
         <div class="customization-separation" style="margin-bottom: 15px"></div>
         <h3 class="customization-section-title">Access requests settings</h3>
         <div class="form-group">
             <label class="control-label col-md-4" for="access_requests_title">Access request tab title</label>
             <div class="col-md-7">
                 <input type="text" id="access_requests_title" name="access_requests_title" class="form-control" value="{{ access_requests_title }}"/>
             </div>
```

### Comparing `NEMO-4.5.4/NEMO/templates/customizations/customizations_safety.html` & `NEMO-4.5.5/NEMO/templates/customizations/customizations_safety.html`

 * *Files identical despite different names*

### Comparing `NEMO-4.5.4/NEMO/templates/customizations/customizations_templates.html` & `NEMO-4.5.5/NEMO/templates/customizations/customizations_templates.html`

 * *Files identical despite different names*

### Comparing `NEMO-4.5.4/NEMO/templates/customizations/customizations_tool.html` & `NEMO-4.5.5/NEMO/templates/customizations/customizations_tool.html`

 * *Files identical despite different names*

### Comparing `NEMO-4.5.4/NEMO/templates/customizations/customizations_upload.html` & `NEMO-4.5.5/NEMO/templates/customizations/customizations_upload.html`

 * *Files identical despite different names*

### Comparing `NEMO-4.5.4/NEMO/templates/customizations/customizations_user.html` & `NEMO-4.5.5/NEMO/templates/customizations/customizations_user.html`

 * *Files identical despite different names*

### Comparing `NEMO-4.5.4/NEMO/templates/email/compose_email.html` & `NEMO-4.5.5/NEMO/templates/email/compose_email.html`

 * *Files identical despite different names*

### Comparing `NEMO-4.5.4/NEMO/templates/email/email_broadcast.html` & `NEMO-4.5.5/NEMO/templates/email/email_broadcast.html`

 * *Files identical despite different names*

### Comparing `NEMO-4.5.4/NEMO/templates/email/email_form.html` & `NEMO-4.5.5/NEMO/templates/email/email_form.html`

 * *Files identical despite different names*

### Comparing `NEMO-4.5.4/NEMO/templates/event_details/area_access_details.html` & `NEMO-4.5.5/NEMO/templates/event_details/area_access_details.html`

 * *Files identical despite different names*

### Comparing `NEMO-4.5.4/NEMO/templates/event_details/outage_details.html` & `NEMO-4.5.5/NEMO/templates/event_details/outage_details.html`

 * *Files identical despite different names*

### Comparing `NEMO-4.5.4/NEMO/templates/event_details/reservation_details.html` & `NEMO-4.5.5/NEMO/templates/event_details/reservation_details.html`

 * *Files identical despite different names*

### Comparing `NEMO-4.5.4/NEMO/templates/event_details/usage_details.html` & `NEMO-4.5.5/NEMO/templates/event_details/usage_details.html`

 * *Files identical despite different names*

### Comparing `NEMO-4.5.4/NEMO/templates/feedback.html` & `NEMO-4.5.5/NEMO/templates/feedback.html`

 * *Files identical despite different names*

### Comparing `NEMO-4.5.4/NEMO/templates/history.html` & `NEMO-4.5.5/NEMO/templates/history.html`

 * *Files identical despite different names*

### Comparing `NEMO-4.5.4/NEMO/templates/impersonate.html` & `NEMO-4.5.5/NEMO/templates/impersonate.html`

 * *Files identical despite different names*

### Comparing `NEMO-4.5.4/NEMO/templates/jumbotron/jumbotron.html` & `NEMO-4.5.5/NEMO/templates/jumbotron/jumbotron.html`

 * *Files identical despite different names*

### Comparing `NEMO-4.5.4/NEMO/templates/jumbotron/jumbotron_content.html` & `NEMO-4.5.5/NEMO/templates/jumbotron/jumbotron_content.html`

 * *Files identical despite different names*

### Comparing `NEMO-4.5.4/NEMO/templates/landing.html` & `NEMO-4.5.5/NEMO/templates/landing.html`

 * *Files identical despite different names*

### Comparing `NEMO-4.5.4/NEMO/templates/login.html` & `NEMO-4.5.5/NEMO/templates/login.html`

 * *Files identical despite different names*

### Comparing `NEMO-4.5.4/NEMO/templates/maintenance/closed_task_details.html` & `NEMO-4.5.5/NEMO/templates/maintenance/closed_task_details.html`

 * *Files identical despite different names*

### Comparing `NEMO-4.5.4/NEMO/templates/maintenance/maintenance.html` & `NEMO-4.5.5/NEMO/templates/maintenance/maintenance.html`

 * *Files identical despite different names*

### Comparing `NEMO-4.5.4/NEMO/templates/maintenance/pending_task_details.html` & `NEMO-4.5.5/NEMO/templates/maintenance/pending_task_details.html`

 * *Files identical despite different names*

### Comparing `NEMO-4.5.4/NEMO/templates/mobile/cancellation_result.html` & `NEMO-4.5.5/NEMO/templates/mobile/cancellation_result.html`

 * *Files identical despite different names*

### Comparing `NEMO-4.5.4/NEMO/templates/mobile/choose_item.html` & `NEMO-4.5.5/NEMO/templates/mobile/choose_item.html`

 * *Files identical despite different names*

### Comparing `NEMO-4.5.4/NEMO/templates/mobile/individual_outage.html` & `NEMO-4.5.5/NEMO/templates/mobile/individual_outage.html`

 * *Files identical despite different names*

### Comparing `NEMO-4.5.4/NEMO/templates/mobile/individual_reservation.html` & `NEMO-4.5.5/NEMO/templates/mobile/individual_reservation.html`

 * *Files identical despite different names*

### Comparing `NEMO-4.5.4/NEMO/templates/mobile/new_reservation.html` & `NEMO-4.5.5/NEMO/templates/mobile/new_reservation.html`

 * *Files identical despite different names*

### Comparing `NEMO-4.5.4/NEMO/templates/mobile/reservation_success.html` & `NEMO-4.5.5/NEMO/templates/mobile/reservation_success.html`

 * *Files identical despite different names*

### Comparing `NEMO-4.5.4/NEMO/templates/mobile/view_calendar.html` & `NEMO-4.5.5/NEMO/templates/mobile/view_calendar.html`

 * *Files identical despite different names*

### Comparing `NEMO-4.5.4/NEMO/templates/news/archived_news.html` & `NEMO-4.5.5/NEMO/templates/news/archived_news.html`

 * *Files identical despite different names*

### Comparing `NEMO-4.5.4/NEMO/templates/news/new_news_form.html` & `NEMO-4.5.5/NEMO/templates/news/new_news_form.html`

 * *Files identical despite different names*

### Comparing `NEMO-4.5.4/NEMO/templates/news/news_update_form.html` & `NEMO-4.5.5/NEMO/templates/news/news_update_form.html`

 * *Files identical despite different names*

### Comparing `NEMO-4.5.4/NEMO/templates/news/recent_news.html` & `NEMO-4.5.5/NEMO/templates/news/recent_news.html`

 * *Files identical despite different names*

### Comparing `NEMO-4.5.4/NEMO/templates/occupancy/occupancy_content.html` & `NEMO-4.5.5/NEMO/templates/occupancy/occupancy_content.html`

 * *Files identical despite different names*

### Comparing `NEMO-4.5.4/NEMO/templates/occupancy/occupancy_count.html` & `NEMO-4.5.5/NEMO/templates/occupancy/occupancy_count.html`

 * *Files identical despite different names*

### Comparing `NEMO-4.5.4/NEMO/templates/pagination/pagination_base.html` & `NEMO-4.5.5/NEMO/templates/pagination/pagination_base.html`

 * *Files identical despite different names*

### Comparing `NEMO-4.5.4/NEMO/templates/pagination/pagination_column.html` & `NEMO-4.5.5/NEMO/templates/pagination/pagination_column.html`

 * *Files identical despite different names*

### Comparing `NEMO-4.5.4/NEMO/templates/pagination/pagination_pages.html` & `NEMO-4.5.5/NEMO/templates/pagination/pagination_pages.html`

 * *Files identical despite different names*

### Comparing `NEMO-4.5.4/NEMO/templates/pagination/pagination_selector.html` & `NEMO-4.5.5/NEMO/templates/pagination/pagination_selector.html`

 * *Files identical despite different names*

### Comparing `NEMO-4.5.4/NEMO/templates/qualifications.html` & `NEMO-4.5.5/NEMO/templates/qualifications.html`

 * *Files identical despite different names*

### Comparing `NEMO-4.5.4/NEMO/templates/refresh_sidebar_icons.html` & `NEMO-4.5.5/NEMO/templates/refresh_sidebar_icons.html`

 * *Files identical despite different names*

### Comparing `NEMO-4.5.4/NEMO/templates/remote_work/remote_work.html` & `NEMO-4.5.5/NEMO/templates/remote_work/remote_work.html`

 * *Files 2% similar despite different names*

```diff
@@ -8,20 +8,22 @@
 	<script type="text/javascript" src="{% static "datetimepicker/bootstrap-datetimepicker.js" %}"></script>
 	<link rel="stylesheet" type="text/css" href="{% static "datetimepicker/bootstrap-datetimepicker.css" %}"/>
 {% endblock %}
 {% block tab_content %}
 	<p>This page displays remote work done by {{ facility_name }} staff on behalf of users. You can filter by which staff member performed the work, and
 	when, by using the dropdown boxes below.</p>
 
-	<p>Each charge can be validated, which means that you have confirmed that the charge is legitimate and correct, and no adjustment needs to
-	be made to it. Press the green 'Validate' button on an individual row to validate a charge. Charges that have already been validated are
-	highlighted in <span class="success-highlight">green</span>.</p>
+    {% if remote_work_validation %}
+        <p>Each charge can be validated, which means that you have confirmed that the charge is legitimate and correct, and no adjustment needs to
+        be made to it. Press the green 'Validate' button on an individual row to validate a charge. Charges that have already been validated are
+        highlighted in <span class="success-highlight">green</span>.</p>
 
-	<p>Do not validate a charge if part or all of it is incorrect. Instead, visit the user office so an adjustment can be entered
-	into the billing system. Furthermore, please visit the user office if there is a charge that you forgot to enter.</p>
+        <p>Do not validate a charge if part or all of it is incorrect. Instead, visit the user office so an adjustment can be entered
+        into the billing system. Furthermore, please visit the user office if there is a charge that you forgot to enter.</p>
+    {% endif %}
 
 	<form id="remote_work_form" class="form-horizontal" role="form" style="margin-top: 20px">
 		<input type="hidden" name="csv" id="hidden_data_csv"/>
 		<div class="form-group">
 			<label class="control-label col-md-2" for="operator">View charges for</label>
 			<div class="col-md-4">
 				<select id="operator" name="operator" class="form-control">
```

#### html2text {}

```diff
@@ -3,22 +3,24 @@
 block remote_work_title %}Previous work{% endblock %} {% block
 remote_work_tab_class %}active{% endblock %} {% block extrahead %}
 ootstrap-datetimepicker.js" %}">
 ootstrap-datetimepicker.css" %}"/> {% endblock %} {% block tab_content %}
 This page displays remote work done by {{ facility_name }} staff on behalf of
 users. You can filter by which staff member performed the work, and when, by
 using the dropdown boxes below.
+{% if remote_work_validation %}
 Each charge can be validated, which means that you have confirmed that the
 charge is legitimate and correct, and no adjustment needs to be made to it.
 Press the green 'Validate' button on an individual row to validate a charge.
 Charges that have already been validated are highlighted in green.
 Do not validate a charge if part or all of it is incorrect. Instead, visit the
 user office so an adjustment can be entered into the billing system.
 Furthermore, please visit the user office if there is a charge that you forgot
 to enter.
+{% endif %}
 View charges for
 % if selected_staff == "all staff" %}selected{% endif %}>all staff
 {% for s in staff_list %}
 % if s.id == selected_staff %}selected{% endif %}>{{ s }}
 {% endfor %}
 and for
 % if selected_project == "all projects" %}selected{% endif %}>all projects
```

### Comparing `NEMO-4.5.4/NEMO/templates/remote_work/remote_work_base.html` & `NEMO-4.5.5/NEMO/templates/remote_work/remote_work_base.html`

 * *Files identical despite different names*

### Comparing `NEMO-4.5.4/NEMO/templates/requests/access_requests/access_request.html` & `NEMO-4.5.5/NEMO/templates/requests/access_requests/access_request.html`

 * *Files identical despite different names*

### Comparing `NEMO-4.5.4/NEMO/templates/requests/access_requests/access_requests.html` & `NEMO-4.5.5/NEMO/templates/requests/access_requests/access_requests.html`

 * *Files identical despite different names*

### Comparing `NEMO-4.5.4/NEMO/templates/requests/access_requests/access_requests_table.html` & `NEMO-4.5.5/NEMO/templates/requests/access_requests/access_requests_table.html`

 * *Files identical despite different names*

### Comparing `NEMO-4.5.4/NEMO/templates/requests/adjustment_requests/adjustment_request.html` & `NEMO-4.5.5/NEMO/templates/requests/adjustment_requests/adjustment_request.html`

 * *Files identical despite different names*

### Comparing `NEMO-4.5.4/NEMO/templates/requests/adjustment_requests/adjustment_requests.html` & `NEMO-4.5.5/NEMO/templates/requests/adjustment_requests/adjustment_requests.html`

 * *Files identical despite different names*

### Comparing `NEMO-4.5.4/NEMO/templates/requests/adjustment_requests/adjustment_requests_table.html` & `NEMO-4.5.5/NEMO/templates/requests/adjustment_requests/adjustment_requests_table.html`

 * *Files 6% similar despite different names*

```diff
@@ -31,14 +31,20 @@
                 <td class="text-center" style="vertical-align: middle">{{ a_request.item.get_display }}</td>
                 <td class="text-center" style="vertical-align: middle">{{ a_request.get_new_start|date:'SHORT_DATETIME_FORMAT' }}</td>
                 <td class="text-center" style="vertical-align: middle">{{ a_request.get_new_end|date:'SHORT_DATETIME_FORMAT' }}</td>
                 <td class="text-center" style="vertical-align: middle">{{ a_request.get_time_difference|default_if_none:"" }}</td>
                 <td class="text-right text-nowrap" style="vertical-align: middle">
                     {% if request_status == 'approved' or request_status == 'denied' %}
                         {{ a_request.reviewer.get_name }}
+                        {% if request_status == 'approved' and a_request.editable_charge and "django.contrib.admin"|app_installed and "requests"|customization:"adjustment_requests_edit_charge_button" == "enabled" %}
+                            {% admin_edit_url a_request.item as edit_url %}
+                            {% if edit_url %}
+                                <br>{% button type="edit" size="small" value="Edit charge" url=edit_url %}
+                            {% endif %}
+                        {% endif %}
                     {% else %}
                         {% if request_status == 'pending' and user.is_facility_manager %}
                             <a class="btn btn-sm btn-default" title="Approve/Deny" href="{% url 'edit_adjustment_request' a_request.id %}"><i class="glyphicon glyphicon-ok-circle success-highlight"></i>&nbsp;&nbsp;<i class="glyphicon glyphicon-ban-circle danger-highlight"></i> Review</a>
                         {% endif %}
                         {% if request_status == 'pending' and a_request.creator == user %}
                             {% url 'edit_adjustment_request' a_request.id as edit_request_url %}
                             {% url 'delete_adjustment_request' a_request.id as delete_request_url %}
```

#### html2text {}

```diff
@@ -1,50 +1,45 @@
 {% load custom_tags_and_filters %}
-                                                                                                                                                                                                   {% if request_status ==
-                                                                                                                                                                                                   'pending' and
-                                                                                                                                                                                                   user.is_facility_manager %}
-                                                                                                                                                                                                   Action {% elif
-Created                             User                       Charge                     New start                     New end                     Difference                                     request_status ==
-                                                                                                                                                                                                   'approved' %} Approved by
-                                                                                                                                                                                                   {% elif request_status ==
-                                                                                                                                                                                                   'denied' %} Denied by {%
+                                                                                                                                                                                                   {% if request_status == 'pending' and
+                                                                                                                                                                                                   user.is_facility_manager %} Action {%
+Created                             User                       Charge                     New start                     New end                     Difference                                     elif request_status == 'approved' %}
+                                                                                                                                                                                                   Approved by {% elif request_status ==
+                                                                                                                                                                                                   'denied' %} Denied by {% endif %}
+                                                                                                                                                                                                   {% if request_status == 'approved' or
+                                                                                                                                                                                                   request_status == 'denied' %} {
+                                                                                                                                                                                                   { a_request.reviewer.get_name }} {% if
+                                                                                                                                                                                                   request_status == 'approved' and
+                                                                                                                                                                                                   a_request.editable_charge and
+                                                                                                                                                                                                   "django.contrib.admin"|app_installed and
+                                                                                                                                                                                                   "requests"|customization:
+                                                                                                                                                                                                   "adjustment_requests_edit_charge_button"
+                                                                                                                                                                                                   == "enabled" %} {% admin_edit_url
+                                                                                                                                                                                                   a_request.item as edit_url %} {% if
+                                                                                                                                                                                                   edit_url %}
+                                                                                                                                                                                                   {% button type="edit" size="small"
+                                                                                                                                                                                                   value="Edit charge" url=edit_url %} {%
+{% if a_request.id in                                                                                                                                                                              endif %} {% endif %} {% else %} {% if
+request_notifications %}New {%      {                          {                          {                             {                           {                                              request_status == 'pending' and
+endif %}{                           {                          {                          {                             {                           {                                              user.is_facility_manager %}
+{ a_request.creation_time|date:     a_request.creator.get_name a_request.item.get_display a_request.get_new_start|date: a_request.get_new_end|date: a_request.get_time_difference|default_if_none:   _Review
+'SHORT_DATETIME_FORMAT' }}          }}                         }}                         'SHORT_DATETIME_FORMAT' }}    'SHORT_DATETIME_FORMAT' }}  "" }}                                           {% endif %} {% if request_status ==
+                                                                                                                                                                                                   'pending' and a_request.creator == user
+                                                                                                                                                                                                   %} {% url 'edit_adjustment_request'
+                                                                                                                                                                                                   a_request.id as edit_request_url %} {%
+                                                                                                                                                                                                   url 'delete_adjustment_request'
+                                                                                                                                                                                                   a_request.id as delete_request_url %} {%
+                                                                                                                                                                                                   button type="edit" size="small"
+                                                                                                                                                                                                   value="Edit" title="Edit request"
+                                                                                                                                                                                                   url=edit_request_url %} {% button
+                                                                                                                                                                                                   type="delete" size="small"
+                                                                                                                                                                                                   value="Delete" title="Delete request"
+                                                                                                                                                                                                   url=delete_request_url onclick="return
+                                                                                                                                                                                                   confirm('Are you sure you want to delete
+                                                                                                                                                                                                   this request?');" %} {% endif %} {%
                                                                                                                                                                                                    endif %}
-                                                                                                                                                                                                   {% if request_status ==
-                                                                                                                                                                                                   'approved' or
-                                                                                                                                                                                                   request_status == 'denied'
-                                                                                                                                                                                                   %} {
-                                                                                                                                                                                                   {
-                                                                                                                                                                                                   a_request.reviewer.get_name
-                                                                                                                                                                                                   }} {% else %} {% if
-                                                                                                                                                                                                   request_status == 'pending'
-                                                                                                                                                                                                   and
-                                                                                                                                                                                                   user.is_facility_manager %}
-                                                                                                                                                                                                     _Review
-                                                                                                                                                                                                    {% endif %} {% if
-                                                                                                                                                                                                   request_status == 'pending'
-                                                                                                                                                                                                   and a_request.creator ==
-{% if a_request.id in               {                          {                          {                             {                           {                                              user %} {% url
-request_notifications %}New {%      {                          {                          {                             {                           {                                              'edit_adjustment_request'
-endif %}{                           a_request.creator.get_name a_request.item.get_display a_request.get_new_start|date: a_request.get_new_end|date: a_request.get_time_difference|default_if_none: a_request.id as
-{ a_request.creation_time|date:     }}                         }}                         'SHORT_DATETIME_FORMAT' }}    'SHORT_DATETIME_FORMAT' }}  "" }}                                          edit_request_url %} {% url
-'SHORT_DATETIME_FORMAT' }}                                                                                                                                                                         'delete_adjustment_request'
-                                                                                                                                                                                                   a_request.id as
-                                                                                                                                                                                                   delete_request_url %} {%
-                                                                                                                                                                                                   button type="edit"
-                                                                                                                                                                                                   size="small" value="Edit"
-                                                                                                                                                                                                   title="Edit request"
-                                                                                                                                                                                                   url=edit_request_url %} {%
-                                                                                                                                                                                                   button type="delete"
-                                                                                                                                                                                                   size="small" value="Delete"
-                                                                                                                                                                                                   title="Delete request"
-                                                                                                                                                                                                   url=delete_request_url
-                                                                                                                                                                                                   onclick="return confirm
-                                                                                                                                                                                                   ('Are you sure you want to
-                                                                                                                                                                                                   delete this request?');" %}
-                                                                                                                                                                                                   {% endif %} {% endif %}
 {% if a_request.description %}
 {
 {
 a_request.description|linebreaksbr
 }}
 {{ a_request.creator.get_name }}, {
 { a_request.creation_time }}
```

### Comparing `NEMO-4.5.4/NEMO/templates/requests/buddy_requests/buddy_request.html` & `NEMO-4.5.5/NEMO/templates/requests/buddy_requests/buddy_request.html`

 * *Files identical despite different names*

### Comparing `NEMO-4.5.4/NEMO/templates/requests/buddy_requests/buddy_requests.html` & `NEMO-4.5.5/NEMO/templates/requests/buddy_requests/buddy_requests.html`

 * *Files identical despite different names*

### Comparing `NEMO-4.5.4/NEMO/templates/requests/user_requests.html` & `NEMO-4.5.5/NEMO/templates/requests/user_requests.html`

 * *Files identical despite different names*

### Comparing `NEMO-4.5.4/NEMO/templates/resources/modify_resource.html` & `NEMO-4.5.5/NEMO/templates/resources/modify_resource.html`

 * *Files identical despite different names*

### Comparing `NEMO-4.5.4/NEMO/templates/resources/resource_details.html` & `NEMO-4.5.5/NEMO/templates/resources/resource_details.html`

 * *Files identical despite different names*

### Comparing `NEMO-4.5.4/NEMO/templates/resources/resources.html` & `NEMO-4.5.5/NEMO/templates/resources/resources.html`

 * *Files identical despite different names*

### Comparing `NEMO-4.5.4/NEMO/templates/resources/scheduled_outage.html` & `NEMO-4.5.5/NEMO/templates/resources/scheduled_outage.html`

 * *Files identical despite different names*

### Comparing `NEMO-4.5.4/NEMO/templates/rest_framework/api.html` & `NEMO-4.5.5/NEMO/templates/rest_framework/api.html`

 * *Files identical despite different names*

### Comparing `NEMO-4.5.4/NEMO/templates/safety/safety.html` & `NEMO-4.5.5/NEMO/templates/safety/safety.html`

 * *Files identical despite different names*

### Comparing `NEMO-4.5.4/NEMO/templates/safety/safety_base.html` & `NEMO-4.5.5/NEMO/templates/safety/safety_base.html`

 * *Files identical despite different names*

### Comparing `NEMO-4.5.4/NEMO/templates/safety/safety_data_sheets.html` & `NEMO-4.5.5/NEMO/templates/safety/safety_data_sheets.html`

 * *Files identical despite different names*

### Comparing `NEMO-4.5.4/NEMO/templates/safety/safety_issues.html` & `NEMO-4.5.5/NEMO/templates/safety/safety_issues.html`

 * *Files identical despite different names*

### Comparing `NEMO-4.5.4/NEMO/templates/safety/safety_issues_create.html` & `NEMO-4.5.5/NEMO/templates/safety/safety_issues_create.html`

 * *Files identical despite different names*

### Comparing `NEMO-4.5.4/NEMO/templates/safety/safety_issues_resolved.html` & `NEMO-4.5.5/NEMO/templates/safety/safety_issues_resolved.html`

 * *Files identical despite different names*

### Comparing `NEMO-4.5.4/NEMO/templates/safety/safety_issues_update.html` & `NEMO-4.5.5/NEMO/templates/safety/safety_issues_update.html`

 * *Files identical despite different names*

### Comparing `NEMO-4.5.4/NEMO/templates/safety/safety_items.html` & `NEMO-4.5.5/NEMO/templates/safety/safety_items.html`

 * *Files identical despite different names*

### Comparing `NEMO-4.5.4/NEMO/templates/snippets/button.html` & `NEMO-4.5.5/NEMO/templates/snippets/button.html`

 * *Files identical despite different names*

### Comparing `NEMO-4.5.4/NEMO/templates/snippets/contact_person.html` & `NEMO-4.5.5/NEMO/templates/snippets/contact_person.html`

 * *Files identical despite different names*

### Comparing `NEMO-4.5.4/NEMO/templates/snippets/embedded_document.html` & `NEMO-4.5.5/NEMO/templates/snippets/embedded_document.html`

 * *Files identical despite different names*

### Comparing `NEMO-4.5.4/NEMO/templates/snippets/tool_info.html` & `NEMO-4.5.5/NEMO/templates/snippets/tool_info.html`

 * *Files identical despite different names*

### Comparing `NEMO-4.5.4/NEMO/templates/staff_charges/change_status.html` & `NEMO-4.5.5/NEMO/templates/staff_charges/change_status.html`

 * *Files identical despite different names*

### Comparing `NEMO-4.5.4/NEMO/templates/staff_charges/choose_project.html` & `NEMO-4.5.5/NEMO/templates/staff_charges/choose_project.html`

 * *Files identical despite different names*

### Comparing `NEMO-4.5.4/NEMO/templates/staff_charges/new_staff_charge.html` & `NEMO-4.5.5/NEMO/templates/staff_charges/new_staff_charge.html`

 * *Files identical despite different names*

### Comparing `NEMO-4.5.4/NEMO/templates/staff_charges/reminder.html` & `NEMO-4.5.5/NEMO/templates/staff_charges/reminder.html`

 * *Files identical despite different names*

### Comparing `NEMO-4.5.4/NEMO/templates/staff_charges/staff_charges_base.html` & `NEMO-4.5.5/NEMO/templates/staff_charges/staff_charges_base.html`

 * *Files identical despite different names*

### Comparing `NEMO-4.5.4/NEMO/templates/status_dashboard/occupancy.html` & `NEMO-4.5.5/NEMO/templates/status_dashboard/occupancy.html`

 * *Files identical despite different names*

### Comparing `NEMO-4.5.4/NEMO/templates/status_dashboard/staff.html` & `NEMO-4.5.5/NEMO/templates/status_dashboard/staff.html`

 * *Files identical despite different names*

### Comparing `NEMO-4.5.4/NEMO/templates/status_dashboard/staff_absence.html` & `NEMO-4.5.5/NEMO/templates/status_dashboard/staff_absence.html`

 * *Files identical despite different names*

### Comparing `NEMO-4.5.4/NEMO/templates/status_dashboard/status_dashboard.html` & `NEMO-4.5.5/NEMO/templates/status_dashboard/status_dashboard.html`

 * *Files identical despite different names*

### Comparing `NEMO-4.5.4/NEMO/templates/status_dashboard/tools.html` & `NEMO-4.5.5/NEMO/templates/status_dashboard/tools.html`

 * *Files 1% similar despite different names*

```diff
@@ -36,15 +36,15 @@
 				{% if tool.nonrequired_resource_is_unavailable %}
 					<span class="glyphicon glyphicon-leaf warning-highlight" title="This tool is operating in a diminished capacity because an optional resource is unavailable"></span>
 				{% endif %}
 			</td>
 			{% if tool.in_use %}
 				{# Output the operator & user of the tool. If the person viewing this page is a staff member, then also allow them to force the operator off the tool. #}
 				<td>
-					{% if user.is_staff %}
+					{% if user.is_staff or user.is_user_office %}
 						<span class="glyphicon glyphicon-remove-circle grey pointer" onclick="force_user_off_of_tool('{% url 'disable_tool' tool.id %}')" title="Force {{ tool.operator }} to stop using the {{ tool.name }}"></span>
 					{% endif %}
 					{{ tool.user }}
 				</td>
 				<td>{{ tool.in_use_since|date:"l @ "}} {{ tool.in_use_since|time }}</td>
 			{% else %}
 				<td></td>
```

#### html2text {}

```diff
@@ -1,16 +1,16 @@
-Tool                                     User          In use since...
+Tool                                     User                In use since...
 {{ tool.get_tool_info_html|safe }} {#
 Output the state of the tool,
 summarizing any associated problems. #}
 {% if tool.in_use %}  {% endif %} {% if
-tool.delayed_logoff_in_progress %}  {%   {% if         {
-endif %} {% if tool.scheduled_outage %}  user.is_staff {
-{% endif %} {% if                        %}  {% endif  tool.in_use_since|date:
-tool.scheduled_partial_outage %}  {%     %} {          "l @ "}} {
-endif %} {% if tool.problematic %}  {%   { tool.user   {
-endif %} {% if tool.operational == False }}            tool.in_use_since|time
-%}  {% endif %} {% if                                  }}
+tool.delayed_logoff_in_progress %}  {%                       {
+endif %} {% if tool.scheduled_outage %}  {% if user.is_staff {
+{% endif %} {% if                        or                  tool.in_use_since|date:
+tool.scheduled_partial_outage %}  {%     user.is_user_office "l @ "}} {
+endif %} {% if tool.problematic %}  {%   %}  {% endif %} {   {
+endif %} {% if tool.operational == False { tool.user }}      tool.in_use_since|time
+%}  {% endif %} {% if                                        }}
 tool.required_resource_is_unavailable %}
 {% endif %} {% if
 tool.nonrequired_resource_is_unavailable
 %}  {% endif %}
```

### Comparing `NEMO-4.5.4/NEMO/templates/tasks/resolve.html` & `NEMO-4.5.5/NEMO/templates/tasks/resolve.html`

 * *Files identical despite different names*

### Comparing `NEMO-4.5.4/NEMO/templates/tasks/update.html` & `NEMO-4.5.5/NEMO/templates/tasks/update.html`

 * *Files identical despite different names*

### Comparing `NEMO-4.5.4/NEMO/templates/tool_control/get_projects.html` & `NEMO-4.5.5/NEMO/templates/tool_control/get_projects.html`

 * *Files identical despite different names*

### Comparing `NEMO-4.5.4/NEMO/templates/tool_control/interlock_error.html` & `NEMO-4.5.5/NEMO/templates/tool_control/interlock_error.html`

 * *Files identical despite different names*

### Comparing `NEMO-4.5.4/NEMO/templates/tool_control/past_tasks_and_comments.html` & `NEMO-4.5.5/NEMO/templates/tool_control/past_tasks_and_comments.html`

 * *Files identical despite different names*

### Comparing `NEMO-4.5.4/NEMO/templates/tool_control/qualified_users.html` & `NEMO-4.5.5/NEMO/templates/tool_control/qualified_users.html`

 * *Files identical despite different names*

### Comparing `NEMO-4.5.4/NEMO/templates/tool_control/tool_control.html` & `NEMO-4.5.5/NEMO/templates/tool_control/tool_control.html`

 * *Files 2% similar despite different names*

```diff
@@ -113,15 +113,15 @@
             ajax_post(url, data, success_callback, function(response, status, xml_http_request) { return interlock_failure_callback(response, status, xml_http_request, url, data, success_callback) }, always_callback);
         }
 
 		function interlock_failure_callback(response, status, xml_http_request, url, data, success_callback, always_callback)
         {
             if(data === undefined)
             {
-                data = {};
+                data = "";
             }
             {# Specific case here where we have an error but it could be bypassed #}
             if (status === 'error' && response.status === 501)
             {
                 let modal_dialog = $('#dialog');
                 $("#dialog .modal-content").html($('#interlock_error_contents').html());
 		        modal_dialog.modal('show');
@@ -135,15 +135,15 @@
                     bypass_button.off("click")
                     $('#dialog .bypass_text').html(response_data['action'] + " anyway");
                     bypass_button.show();
                     bypass_button.one('click', function ()
                     {
                         modal_dialog.on('hidden.bs.modal', function ()
                         {
-                            data["bypass"] = 'True';
+                            data += "&bypass=True";
                             try_post_catch_interlock_error(url, data, success_callback, always_callback);
                             modal_dialog.off();
                         });
                         modal_dialog.modal('hide');
                     });
                 }
                 {# hook up try again button #}
@@ -178,23 +178,24 @@
 			let url = "{% url 'enable_tool' tool_id=111 user_id=22222222 project_id=33333333 staff_charge='false' %}".replace('111', tool_id).replace('22222222', user_id.toString()).replace('33333333', project_id.toString()).replace('false', staff_charge.toString())
 			let success_callbacks;
 			if(staff_charge === true)
 				success_callbacks = [reload_page]; {# If there's a new staff charge then we need to reload the whole page so it's displayed in the menu bar. #}
 			else
 				success_callbacks = [refresh_tool_status, ajax_success_callback];
 			let enable_start_button = function() { $("#start button").prop("disabled", false); };
-			try_post_catch_interlock_error(url, {"remote_work": $("#remote_work").val()}, success_callbacks, enable_start_button);
+            let data = "remote_work=" + $("#remote_work").val();
+			try_post_catch_interlock_error(url, data, success_callbacks, enable_start_button);
 		}
 
 		function disable_tool(url)
 		{
 			$("#stop").prop("disabled", true);
-			let contents = $("#tool_control").serialize();
+			let data = $("#tool_control").serialize();
 			let enable_stop_button = function() { $("#stop").prop("disabled", false); };
-			try_post_catch_interlock_error(url, contents, [refresh_tool_status, ajax_success_callback], enable_stop_button);
+			try_post_catch_interlock_error(url, data, [refresh_tool_status, ajax_success_callback], enable_stop_button);
 		}
 
 		{% if user.is_staff %}
 
 			{# Only staff can perform the functions in this if-block. #}
 
 			function use_tool_for_other(remote_work)
```

### Comparing `NEMO-4.5.4/NEMO/templates/tool_control/tool_status.html` & `NEMO-4.5.5/NEMO/templates/tool_control/tool_status.html`

 * *Files identical despite different names*

### Comparing `NEMO-4.5.4/NEMO/templates/tool_control/usage_data.html` & `NEMO-4.5.5/NEMO/templates/tool_control/usage_data.html`

 * *Files identical despite different names*

### Comparing `NEMO-4.5.4/NEMO/templates/training/get_projects.html` & `NEMO-4.5.5/NEMO/templates/training/get_projects.html`

 * *Files identical despite different names*

### Comparing `NEMO-4.5.4/NEMO/templates/training/training.html` & `NEMO-4.5.5/NEMO/templates/training/training.html`

 * *Files identical despite different names*

### Comparing `NEMO-4.5.4/NEMO/templates/training/training_entry.html` & `NEMO-4.5.5/NEMO/templates/training/training_entry.html`

 * *Files identical despite different names*

### Comparing `NEMO-4.5.4/NEMO/templates/usage/billing.html` & `NEMO-4.5.5/NEMO/templates/usage/billing.html`

 * *Files identical despite different names*

### Comparing `NEMO-4.5.4/NEMO/templates/usage/usage.html` & `NEMO-4.5.5/NEMO/templates/usage/usage.html`

 * *Files identical despite different names*

### Comparing `NEMO-4.5.4/NEMO/templates/usage/usage_base.html` & `NEMO-4.5.5/NEMO/templates/usage/usage_base.html`

 * *Files identical despite different names*

### Comparing `NEMO-4.5.4/NEMO/templates/users/create_or_modify_user.html` & `NEMO-4.5.5/NEMO/templates/users/create_or_modify_user.html`

 * *Files identical despite different names*

### Comparing `NEMO-4.5.4/NEMO/templates/users/preferences.html` & `NEMO-4.5.5/NEMO/templates/users/preferences.html`

 * *Files identical despite different names*

### Comparing `NEMO-4.5.4/NEMO/templates/users/safe_deactivation.html` & `NEMO-4.5.5/NEMO/templates/users/safe_deactivation.html`

 * *Files identical despite different names*

### Comparing `NEMO-4.5.4/NEMO/templates/users/users.html` & `NEMO-4.5.5/NEMO/templates/users/users.html`

 * *Files identical despite different names*

### Comparing `NEMO-4.5.4/NEMO/templatetags/custom_tags_and_filters.py` & `NEMO-4.5.5/NEMO/templatetags/custom_tags_and_filters.py`

 * *Files 4% similar despite different names*

```diff
@@ -11,14 +11,15 @@
 from django.utils import timezone
 from django.utils.formats import localize_input
 from django.utils.html import escape, escapejs, format_html
 from django.utils.safestring import mark_safe
 
 from NEMO.mixins import BillableItemMixin
 from NEMO.models import User
+from NEMO.utilities import get_full_url
 from NEMO.views.customization import CustomizationBase, ProjectsAccountsCustomization
 
 register = template.Library()
 
 
 @register.filter
 def class_name(value):
@@ -171,14 +172,27 @@
 
 @register.filter
 def content_type(obj):
 	if obj:
 		return ContentType.objects.get_for_model(obj)
 
 
+@register.simple_tag(takes_context=True)
+def admin_edit_url(context, obj):
+	user = context["request"].user
+	try:
+		obj_type = content_type(obj)
+		permission = user.has_perm(f"{obj_type.app_label}.change_{obj_type.model}")
+		if permission:
+			url = reverse(f"admin:{obj_type.app_label}_{obj_type.model}_change", args=[obj.id])
+			return url
+	except:
+		pass
+
+
 @register.filter
 def billable_display(item: BillableItemMixin, user: User):
 	return item.get_display(user) if item else ""
 
 
 @register.inclusion_tag("snippets/button.html")
 def button(value, type="default", size="", icon=None, onclick=None, dismiss="", submit=None, title=None, url="", **kwargs):
@@ -225,7 +239,13 @@
 		"btn_icon": btn_icon + second_icon if icon is None else btn_icon + icon,
 		"btn_onclick": onclick if onclick is not None else "submit_and_disable(this);" if submit else "",
 		"btn_type": None if url else "submit" if submit else "button",
 		"btn_url": resolve_url(url) if url else None,
 		"btn_dismiss": dismiss,
 		"kwargs": kwargs,  # pass the rest of the kwargs directly to the button to be used as attributes
 	}
+
+
+@register.simple_tag(takes_context=True)
+def absolute_url(context, view_name, *args, **kwargs):
+	url = reverse(view_name, args=args, kwargs=kwargs)
+	return get_full_url(url, request=context['request'])
```

### Comparing `NEMO-4.5.4/NEMO/urls.py` & `NEMO-4.5.5/NEMO/urls.py`

 * *Files 2% similar despite different names*

```diff
@@ -22,14 +22,15 @@
 	alerts,
 	api,
 	api_file_import,
 	area_access,
 	authentication,
 	buddy_requests,
 	calendar,
+	charge_validation,
 	configuration_agenda,
 	consumables,
 	contact_staff,
 	customization,
 	documents,
 	email,
 	event_details,
@@ -209,16 +210,21 @@
 	path("remote_work/", remote_work.remote_work, name="remote_work"),
 	path("staff_charges/", remote_work.staff_charges, name="staff_charges"),
 	path("begin_staff_charge/", remote_work.begin_staff_charge, name="begin_staff_charge"),
 	path("begin_staff_area_charge/", remote_work.begin_staff_area_charge, name="begin_staff_area_charge"),
 	path("end_staff_area_charge/", remote_work.end_staff_area_charge, name="end_staff_area_charge"),
 	path("end_staff_charge/", remote_work.end_staff_charge, name="end_staff_charge"),
 	path("edit_staff_charge_note/", remote_work.edit_staff_charge_note, name="edit_staff_charge_note"),
-	path("validate_staff_charge/<int:staff_charge_id>/", remote_work.validate_staff_charge, name="validate_staff_charge"),
-	path("validate_usage_event/<int:usage_event_id>/", remote_work.validate_usage_event, name="validate_usage_event"),
+
+	path("validate_staff_charge/<int:staff_charge_id>/", charge_validation.validate_staff_charge, name="validate_staff_charge"),
+	path("validate_usage_event/<int:usage_event_id>/", charge_validation.validate_usage_event, name="validate_usage_event"),
+	path("validate_area_access_record/<int:area_access_record_id>/", charge_validation.validate_area_access_record, name="validate_area_access_record"),
+	path("validate_missed_reservation/<int:reservation_id>/", charge_validation.validate_missed_reservation, name="validate_missed_reservation"),
+	path("validate_training_session/<int:training_session_id>/", charge_validation.validate_training_session, name="validate_training_session"),
+	path("validate_consumable_withdraw/<int:consumable_withdraw_id>/", charge_validation.validate_consumable_withdrawal, name="validate_consumable_withdrawal"),
 
 	# Status dashboard:
 	path("status_dashboard/", status_dashboard.status_dashboard, name="status_dashboard"),
 	re_path(r"^status_dashboard/(?P<tab>tools|occupancy|staff)/$", status_dashboard.status_dashboard, name="status_dashboard_tab"),
 
 	# Jumbotron:
 	path("jumbotron/", jumbotron.jumbotron, name="jumbotron"),
```

### Comparing `NEMO-4.5.4/NEMO/utilities.py` & `NEMO-4.5.5/NEMO/utilities.py`

 * *Files 0% similar despite different names*

```diff
@@ -618,15 +618,15 @@
 	"""
 	Function used mainly in emails and places where the request might or might not be available.
 	If the request is available, use django's built in way to build the absolute URL, otherwise
 	use the SERVER_DOMAIN variable from settings, which defaults to the first ALLOWED_HOSTS value.
 	"""
 	# For lazy locations
 	location = str(location)
-	if request:
+	if request and not isinstance(request, EmptyHttpRequest):
 		return request.build_absolute_uri(location)
 	else:
 		domain = getattr(settings, "SERVER_DOMAIN", "https://{}".format(settings.ALLOWED_HOSTS[0]))
 		return urljoin(domain, location)
 
 
 def capitalize(string: Optional[str]) -> str:
```

### Comparing `NEMO-4.5.4/NEMO/views/abuse.py` & `NEMO-4.5.5/NEMO/views/abuse.py`

 * *Files identical despite different names*

### Comparing `NEMO-4.5.4/NEMO/views/access_requests.py` & `NEMO-4.5.5/NEMO/views/access_requests.py`

 * *Files identical despite different names*

### Comparing `NEMO-4.5.4/NEMO/views/accounts_and_projects.py` & `NEMO-4.5.5/NEMO/views/accounts_and_projects.py`

 * *Files identical despite different names*

### Comparing `NEMO-4.5.4/NEMO/views/adjustment_requests.py` & `NEMO-4.5.5/NEMO/views/adjustment_requests.py`

 * *Files 2% similar despite different names*

```diff
@@ -320,17 +320,22 @@
             .order_by("-end")[:item_number]
         )
         items.extend(
             AreaAccessRecord.objects.filter(end__isnull=False, staff_charge__staff_member=user)
             .filter(**end_filter)
             .order_by("-end")[:item_number]
         )
-        items.extend(StaffCharge.objects.filter(staff_member=user).filter(**end_filter).order_by("-end")[:item_number])
+        items.extend(StaffCharge.objects.filter(end__isnull=False, staff_member=user).filter(**end_filter).order_by("-end")[:item_number])
     if current_item and current_item in items:
         items.remove(current_item)
+    # Remove already adjusted charges. filter by id first
+    for previously_adjusted in AdjustmentRequest.objects.filter(deleted=False, item_id__in=[item.id for item in items]):
+        # Then confirm it's the correct item
+        if previously_adjusted.item in items:
+            items.remove(previously_adjusted.item)
     items.sort(key=lambda x: (x.get_end(), x.get_start()), reverse=True)
     return items[:item_number]
 
 
 @accounting_or_user_office_or_manager_required
 @require_GET
 def csv_export(request):
```

### Comparing `NEMO-4.5.4/NEMO/views/alerts.py` & `NEMO-4.5.5/NEMO/views/alerts.py`

 * *Files identical despite different names*

### Comparing `NEMO-4.5.4/NEMO/views/api.py` & `NEMO-4.5.5/NEMO/views/api.py`

 * *Files identical despite different names*

### Comparing `NEMO-4.5.4/NEMO/views/api_billing.py` & `NEMO-4.5.5/NEMO/views/api_billing.py`

 * *Files identical despite different names*

### Comparing `NEMO-4.5.4/NEMO/views/api_file_import.py` & `NEMO-4.5.5/NEMO/views/api_file_import.py`

 * *Files identical despite different names*

### Comparing `NEMO-4.5.4/NEMO/views/area_access.py` & `NEMO-4.5.5/NEMO/views/area_access.py`

 * *Files identical despite different names*

### Comparing `NEMO-4.5.4/NEMO/views/authentication.py` & `NEMO-4.5.5/NEMO/views/authentication.py`

 * *Files identical despite different names*

### Comparing `NEMO-4.5.4/NEMO/views/buddy_requests.py` & `NEMO-4.5.5/NEMO/views/buddy_requests.py`

 * *Files identical despite different names*

### Comparing `NEMO-4.5.4/NEMO/views/calendar.py` & `NEMO-4.5.5/NEMO/views/calendar.py`

 * *Files identical despite different names*

### Comparing `NEMO-4.5.4/NEMO/views/configuration_agenda.py` & `NEMO-4.5.5/NEMO/views/configuration_agenda.py`

 * *Files identical despite different names*

### Comparing `NEMO-4.5.4/NEMO/views/consumables.py` & `NEMO-4.5.5/NEMO/views/consumables.py`

 * *Files identical despite different names*

### Comparing `NEMO-4.5.4/NEMO/views/customization.py` & `NEMO-4.5.5/NEMO/views/customization.py`

 * *Files 0% similar despite different names*

```diff
@@ -273,14 +273,15 @@
 		"adjustment_requests_staff_staff_charges_enabled": "enabled",
 		"adjustment_requests_title": "Adjustment requests",
 		"adjustment_requests_description": "",
 		"adjustment_requests_charges_display_number": "10",
 		"adjustment_requests_display_max": "",
 		"adjustment_requests_time_limit_interval": "2",
 		"adjustment_requests_time_limit_frequency": RecurrenceFrequency.WEEKLY.index,
+		"adjustment_requests_edit_charge_button": "",
 		"weekend_access_notification_emails": "",
 		"weekend_access_notification_cutoff_hour": "",
 		"weekend_access_notification_cutoff_day": "",
 	}
 
 	@classmethod
 	def get_date_limit(cls) -> datetime:
```

### Comparing `NEMO-4.5.4/NEMO/views/documents.py` & `NEMO-4.5.5/NEMO/views/documents.py`

 * *Files identical despite different names*

### Comparing `NEMO-4.5.4/NEMO/views/email.py` & `NEMO-4.5.5/NEMO/views/email.py`

 * *Files identical despite different names*

### Comparing `NEMO-4.5.4/NEMO/views/event_details.py` & `NEMO-4.5.5/NEMO/views/event_details.py`

 * *Files identical despite different names*

### Comparing `NEMO-4.5.4/NEMO/views/feedback.py` & `NEMO-4.5.5/NEMO/views/feedback.py`

 * *Files identical despite different names*

### Comparing `NEMO-4.5.4/NEMO/views/get_projects.py` & `NEMO-4.5.5/NEMO/views/get_projects.py`

 * *Files identical despite different names*

### Comparing `NEMO-4.5.4/NEMO/views/history.py` & `NEMO-4.5.5/NEMO/views/history.py`

 * *Files identical despite different names*

### Comparing `NEMO-4.5.4/NEMO/views/jumbotron.py` & `NEMO-4.5.5/NEMO/views/jumbotron.py`

 * *Files identical despite different names*

### Comparing `NEMO-4.5.4/NEMO/views/landing.py` & `NEMO-4.5.5/NEMO/views/landing.py`

 * *Files identical despite different names*

### Comparing `NEMO-4.5.4/NEMO/views/maintenance.py` & `NEMO-4.5.5/NEMO/views/maintenance.py`

 * *Files identical despite different names*

### Comparing `NEMO-4.5.4/NEMO/views/mobile.py` & `NEMO-4.5.5/NEMO/views/mobile.py`

 * *Files identical despite different names*

### Comparing `NEMO-4.5.4/NEMO/views/news.py` & `NEMO-4.5.5/NEMO/views/news.py`

 * *Files identical despite different names*

### Comparing `NEMO-4.5.4/NEMO/views/notifications.py` & `NEMO-4.5.5/NEMO/views/notifications.py`

 * *Files identical despite different names*

### Comparing `NEMO-4.5.4/NEMO/views/pagination.py` & `NEMO-4.5.5/NEMO/views/pagination.py`

 * *Files identical despite different names*

### Comparing `NEMO-4.5.4/NEMO/views/qualifications.py` & `NEMO-4.5.5/NEMO/views/qualifications.py`

 * *Files identical despite different names*

### Comparing `NEMO-4.5.4/NEMO/views/remote_work.py` & `NEMO-4.5.5/NEMO/views/remote_work.py`

 * *Files 2% similar despite different names*

```diff
@@ -136,32 +136,14 @@
 		"selected_project": project.id if project else "all projects",
 		"remote_work_validation": RemoteWorkCustomization.get_bool("remote_work_validation"),
 	}
 	return render(request, "remote_work/remote_work.html", dictionary)
 
 
 @staff_member_required
-@require_POST
-def validate_staff_charge(request, staff_charge_id):
-	staff_charge = get_object_or_404(StaffCharge, id=staff_charge_id)
-	staff_charge.validated = True
-	staff_charge.save()
-	return HttpResponse()
-
-
-@staff_member_required
-@require_POST
-def validate_usage_event(request, usage_event_id):
-	usage_event = get_object_or_404(UsageEvent, id=usage_event_id)
-	usage_event.validated = True
-	usage_event.save()
-	return HttpResponse()
-
-
-@staff_member_required
 @require_GET
 def staff_charges(request):
 	staff_member: User = request.user
 	staff_charge: StaffCharge = staff_member.get_staff_charge()
 	dictionary = dict()
 	if staff_charge:
 		try:
```

### Comparing `NEMO-4.5.4/NEMO/views/resources.py` & `NEMO-4.5.5/NEMO/views/resources.py`

 * *Files identical despite different names*

### Comparing `NEMO-4.5.4/NEMO/views/safety.py` & `NEMO-4.5.5/NEMO/views/safety.py`

 * *Files identical despite different names*

### Comparing `NEMO-4.5.4/NEMO/views/sidebar.py` & `NEMO-4.5.5/NEMO/views/sidebar.py`

 * *Files identical despite different names*

### Comparing `NEMO-4.5.4/NEMO/views/status_dashboard.py` & `NEMO-4.5.5/NEMO/views/status_dashboard.py`

 * *Files identical despite different names*

### Comparing `NEMO-4.5.4/NEMO/views/tasks.py` & `NEMO-4.5.5/NEMO/views/tasks.py`

 * *Files identical despite different names*

### Comparing `NEMO-4.5.4/NEMO/views/tool_control.py` & `NEMO-4.5.5/NEMO/views/tool_control.py`

 * *Files identical despite different names*

### Comparing `NEMO-4.5.4/NEMO/views/training.py` & `NEMO-4.5.5/NEMO/views/training.py`

 * *Files identical despite different names*

### Comparing `NEMO-4.5.4/NEMO/views/tutorials.py` & `NEMO-4.5.5/NEMO/views/tutorials.py`

 * *Files identical despite different names*

### Comparing `NEMO-4.5.4/NEMO/views/usage.py` & `NEMO-4.5.5/NEMO/views/usage.py`

 * *Files 3% similar despite different names*

```diff
@@ -1,21 +1,23 @@
+from collections import defaultdict
 from logging import getLogger
 from typing import List, Set
 
 from django.conf import settings
 from django.contrib.auth.decorators import login_required
 from django.db.models import Q
 from django.shortcuts import get_object_or_404, redirect, render
 from django.urls import reverse
 from django.views.decorators.http import require_GET
 from requests import get
 
 from NEMO.decorators import accounting_or_user_office_or_manager_required
 from NEMO.models import (
 	Account,
+	AdjustmentRequest,
 	AreaAccessRecord,
 	ConsumableWithdraw,
 	Project,
 	Reservation,
 	StaffCharge,
 	TrainingSession,
 	UsageEvent,
@@ -122,22 +124,26 @@
 	missed_reservations = Reservation.objects.filter(user_filter).filter(missed=True, end__gt=start_date, end__lte=end_date)
 	staff_charges = StaffCharge.objects.filter(customer_filter).filter(end__gt=start_date, end__lte=end_date)
 	training_sessions = TrainingSession.objects.filter(trainee_filter).filter(date__gt=start_date, date__lte=end_date)
 	usage_events = UsageEvent.objects.filter(user_filter).filter(end__gt=start_date, end__lte=end_date)
 	if csv_export:
 		return csv_export_response(usage_events, area_access, training_sessions, staff_charges, consumables, missed_reservations)
 	else:
+		existing_adjustments = defaultdict(list)
+		for values in AdjustmentRequest.objects.filter(deleted=False, creator=user).values("item_type", "item_id").distinct():
+			existing_adjustments[values["item_type"]].append(values["item_id"])
 		dictionary = {
 			'area_access': area_access,
 			'consumables': consumables,
 			'missed_reservations': missed_reservations,
 			'staff_charges': staff_charges,
 			'training_sessions': training_sessions,
 			'usage_events': usage_events,
 			'adjustment_time_limit': UserRequestsCustomization.get_date_limit(),
+			'existing_adjustments': existing_adjustments,
 			'can_export': True,
 		}
 		if user_managed_projects:
 			dictionary['pi_projects'] = user_managed_projects
 		dictionary['no_charges'] = not (dictionary['area_access'] or dictionary['consumables'] or dictionary['missed_reservations'] or dictionary['staff_charges'] or dictionary['training_sessions'] or dictionary['usage_events'])
 		return render(request, 'usage/usage.html', {**base_dictionary, **dictionary})
 
@@ -199,23 +205,27 @@
 				staff_charges = staff_charges.filter(customer=user)
 				training_sessions = training_sessions.filter(trainee=user)
 				usage_events = usage_events.filter(user=user)
 			if bool(request.GET.get("csv", False)):
 				return csv_export_response(usage_events, area_access, training_sessions, staff_charges, consumables, missed_reservations)
 	except:
 		pass
+	existing_adjustments = defaultdict(list)
+	for values in AdjustmentRequest.objects.filter(deleted=False, creator=request.user).values("item_type", "item_id").distinct():
+		existing_adjustments[values["item_type"]].append(values["item_id"])
 	dictionary = {
 		'search_items': set(Account.objects.all()) | set(Project.objects.all()) | set(get_project_applications()) | set(User.objects.filter(is_active=True)),
 		'area_access': area_access,
 		'consumables': consumables,
 		'missed_reservations': missed_reservations,
 		'staff_charges': staff_charges,
 		'training_sessions': training_sessions,
 		'usage_events': usage_events,
 		'adjustment_time_limit': UserRequestsCustomization.get_date_limit(),
+		'existing_adjustments': existing_adjustments,
 		'project_autocomplete': True,
 		'selection': selection,
 		'can_export': True,
 	}
 	dictionary['no_charges'] = not (dictionary['area_access'] or dictionary['consumables'] or dictionary['missed_reservations'] or dictionary['staff_charges'] or dictionary['training_sessions'] or dictionary['usage_events'])
 	return render(request, 'usage/usage.html', {**base_dictionary, **dictionary})
```

### Comparing `NEMO-4.5.4/NEMO/views/user_requests.py` & `NEMO-4.5.5/NEMO/views/user_requests.py`

 * *Files identical despite different names*

### Comparing `NEMO-4.5.4/NEMO/views/users.py` & `NEMO-4.5.5/NEMO/views/users.py`

 * *Files identical despite different names*

### Comparing `NEMO-4.5.4/NEMO/widgets/configuration_editor.py` & `NEMO-4.5.5/NEMO/widgets/configuration_editor.py`

 * *Files identical despite different names*

### Comparing `NEMO-4.5.4/NEMO/widgets/dynamic_form.py` & `NEMO-4.5.5/NEMO/widgets/dynamic_form.py`

 * *Files 1% similar despite different names*

```diff
@@ -405,15 +405,17 @@
 		self.untreated_questions = []
 		self.questions = []
 		if questions:
 			self.untreated_questions = loads(questions)
 			self.questions: List[PostUsageQuestion] = PostUsageQuestion.load_questions(self.untreated_questions)
 
 	def render(self, group_question_url: str, group_item_id: int, virtual_inputs: bool = False):
-		result = "<script>if (!$) { $ = django.jQuery; }</script>"
+		result = ""
+		if self.questions:
+			result += "<script>if (!$) { $ = django.jQuery; }</script>"
 		for question in self.questions:
 			result += question.render(virtual_inputs, group_question_url, group_item_id)
 		return mark_safe(result)
 
 	def validate(self, group_question_url: str, group_item_id: int):
 		# We need to validate the raw json for types
 		for question in self.untreated_questions:
@@ -573,25 +575,25 @@
 				)
 				pass
 
 
 def get_counter_increment_for_question(question, input_data, counter_question):
 	additional_value = 0
 	if isinstance(question, PostUsageNumberFieldQuestion) or isinstance(question, PostUsageFloatFieldQuestion):
-		if question.name == counter_question and "user_input" in input_data:
+		if question.name == counter_question and "user_input" in input_data and input_data["user_input"]:
 			if isinstance(input_data["user_input"], dict):
 				for user_input in input_data["user_input"].values():
 					if question.name in user_input and user_input[question.name]:
 						additional_value += float(user_input[question.name])
 			else:
 				additional_value = float(input_data["user_input"])
 	return additional_value
 
 
-question_types : Dict[str, Type[PostUsageQuestion]] = {
+question_types: Dict[str, Type[PostUsageQuestion]] = {
 	"number": PostUsageNumberFieldQuestion,
 	"float": PostUsageFloatFieldQuestion,
 	"textbox": PostUsageTextFieldQuestion,
 	"textarea": PostUsageTextAreaFieldQuestion,
 	"radio": PostUsageRadioQuestion,
 	"checkbox": PostUsageCheckboxQuestion,
 	"dropdown": PostUsageDropdownQuestion,
```

### Comparing `NEMO-4.5.4/NEMO/widgets/item_tree.py` & `NEMO-4.5.5/NEMO/widgets/item_tree.py`

 * *Files identical despite different names*

### Comparing `NEMO-4.5.4/NEMO.egg-info/PKG-INFO` & `NEMO-4.5.5/NEMO.egg-info/PKG-INFO`

 * *Files 1% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: NEMO
-Version: 4.5.4
+Version: 4.5.5
 Summary: NEMO is a laboratory logistics web application. Use it to schedule reservations, control tool access, track maintenance issues, and more.
 Home-page: https://github.com/usnistgov/NEMO
 Author: Center for Nanoscale Science and Technology
 Author-email: CNSTapplications@nist.gov
 License: Public domain
 Classifier: Development Status :: 5 - Production/Stable
 Classifier: Environment :: Web Environment
```

### Comparing `NEMO-4.5.4/NEMO.egg-info/SOURCES.txt` & `NEMO-4.5.5/NEMO.egg-info/SOURCES.txt`

 * *Files 0% similar despite different names*

```diff
@@ -59,15 +59,14 @@
 NEMO/apps/kiosk/static/kiosk/kiosk.css
 NEMO/apps/kiosk/templates/kiosk/acknowledgement.html
 NEMO/apps/kiosk/templates/kiosk/category_choices.html
 NEMO/apps/kiosk/templates/kiosk/choices.html
 NEMO/apps/kiosk/templates/kiosk/error.html
 NEMO/apps/kiosk/templates/kiosk/individual_reservation.html
 NEMO/apps/kiosk/templates/kiosk/kiosk.html
-NEMO/apps/kiosk/templates/kiosk/location_directory.html
 NEMO/apps/kiosk/templates/kiosk/success.html
 NEMO/apps/kiosk/templates/kiosk/tool_information.html
 NEMO/apps/kiosk/templates/kiosk/tool_project_selection_snippet.html
 NEMO/apps/kiosk/templates/kiosk/tool_reservation.html
 NEMO/apps/sensors/__init__.py
 NEMO/apps/sensors/admin.py
 NEMO/apps/sensors/customizations.py
@@ -127,14 +126,15 @@
 NEMO/migrations/0039_version_4_1_0.py
 NEMO/migrations/0040_version_4_2_0.py
 NEMO/migrations/0041_version_4_2_1.py
 NEMO/migrations/0042_version_4_3_0.py
 NEMO/migrations/0043_version_4_3_2.py
 NEMO/migrations/0044_version_4_4_0.py
 NEMO/migrations/0045_version_4_5_0.py
+NEMO/migrations/0045_version_4_5_5.py
 NEMO/migrations/__init__.py
 NEMO/static/badge_reader.js
 NEMO/static/favicon.ico
 NEMO/static/jquery.js
 NEMO/static/jquery.min.js
 NEMO/static/jumbotron_watermark.bmp
 NEMO/static/mobile.js
@@ -359,14 +359,15 @@
 NEMO/views/api.py
 NEMO/views/api_billing.py
 NEMO/views/api_file_import.py
 NEMO/views/area_access.py
 NEMO/views/authentication.py
 NEMO/views/buddy_requests.py
 NEMO/views/calendar.py
+NEMO/views/charge_validation.py
 NEMO/views/configuration_agenda.py
 NEMO/views/constants.py
 NEMO/views/consumables.py
 NEMO/views/contact_staff.py
 NEMO/views/customization.py
 NEMO/views/documents.py
 NEMO/views/email.py
```

### Comparing `NEMO-4.5.4/PKG-INFO` & `NEMO-4.5.5/PKG-INFO`

 * *Files 1% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: NEMO
-Version: 4.5.4
+Version: 4.5.5
 Summary: NEMO is a laboratory logistics web application. Use it to schedule reservations, control tool access, track maintenance issues, and more.
 Home-page: https://github.com/usnistgov/NEMO
 Author: Center for Nanoscale Science and Technology
 Author-email: CNSTapplications@nist.gov
 License: Public domain
 Classifier: Development Status :: 5 - Production/Stable
 Classifier: Environment :: Web Environment
```

### Comparing `NEMO-4.5.4/README.md` & `NEMO-4.5.5/README.md`

 * *Files identical despite different names*

### Comparing `NEMO-4.5.4/resources/splash_pad_settings.py` & `NEMO-4.5.5/resources/splash_pad_settings.py`

 * *Files identical despite different names*

### Comparing `NEMO-4.5.4/setup.py` & `NEMO-4.5.5/setup.py`

 * *Files 2% similar despite different names*

```diff
@@ -1,12 +1,12 @@
 from setuptools import find_namespace_packages, setup
 
 setup(
 	name='NEMO',
-	version='4.5.4',
+	version='4.5.5',
 	python_requires='>=3.8, <4',
 	packages=find_namespace_packages(exclude=['NEMO.tests', 'NEMO.tests.*']),
 	include_package_data=True,
 	url='https://github.com/usnistgov/NEMO',
 	license='Public domain',
 	author='Center for Nanoscale Science and Technology',
 	author_email='CNSTapplications@nist.gov',
@@ -21,15 +21,15 @@
 		'License :: Public Domain',
 		'Natural Language :: English',
 		'Operating System :: OS Independent',
 		'Programming Language :: Python :: 3.8',
 	],
 	install_requires=[
 		'cryptography==40.0.1',
-		'Django==3.2.18',
+		'Django==3.2.19',
 		'django-auditlog==2.2.2',
 		'django-filter==23.1',
 		'django-mptt==0.14.0',
 		'djangorestframework==3.14.0',
 		'drf-excel==2.3.0',
 		'drf-flex-fields==1.0.2',
 		'ldap3==2.9.1',
```

