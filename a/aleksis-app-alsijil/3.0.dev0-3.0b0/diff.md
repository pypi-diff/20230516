# Comparing `tmp/AlekSIS-App-Alsijil-3.0.dev0.tar.gz` & `tmp/aleksis_app_alsijil-3.0b0.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "AlekSIS-App-Alsijil-3.0.dev0.tar", max compression
+gzip compressed data, was "aleksis_app_alsijil-3.0b0.tar", max compression
```

## Comparing `AlekSIS-App-Alsijil-3.0.dev0.tar` & `aleksis_app_alsijil-3.0b0.tar`

### file list

```diff
@@ -1,163 +1,157 @@
--rw-r--r--   0        0        0     8170 2022-08-18 20:28:10.129582 AlekSIS-App-Alsijil-3.0.dev0/CHANGELOG.rst
--rw-r--r--   0        0        0    14361 2022-08-18 20:28:10.129582 AlekSIS-App-Alsijil-3.0.dev0/LICENCE.rst
--rw-r--r--   0        0        0     2153 2022-08-18 20:28:10.129582 AlekSIS-App-Alsijil-3.0.dev0/README.rst
--rw-r--r--   0        0        0      153 2022-08-18 20:28:10.129582 AlekSIS-App-Alsijil-3.0.dev0/aleksis/apps/alsijil/__init__.py
--rw-r--r--   0        0        0      326 2022-08-18 20:31:34.530012 AlekSIS-App-Alsijil-3.0.dev0/aleksis/apps/alsijil/__pycache__/__init__.cpython-310.pyc
--rw-r--r--   0        0        0     1066 2022-08-18 20:31:34.986022 AlekSIS-App-Alsijil-3.0.dev0/aleksis/apps/alsijil/__pycache__/apps.cpython-310.pyc
--rw-r--r--   0        0        0     5895 2022-08-18 20:31:35.670036 AlekSIS-App-Alsijil-3.0.dev0/aleksis/apps/alsijil/__pycache__/data_checks.cpython-310.pyc
--rw-r--r--   0        0        0     7237 2022-08-18 20:31:35.670036 AlekSIS-App-Alsijil-3.0.dev0/aleksis/apps/alsijil/__pycache__/managers.cpython-310.pyc
--rw-r--r--   0        0        0    13486 2022-08-18 20:31:35.810040 AlekSIS-App-Alsijil-3.0.dev0/aleksis/apps/alsijil/__pycache__/model_extensions.cpython-310.pyc
--rw-r--r--   0        0        0    15829 2022-08-18 20:31:35.666036 AlekSIS-App-Alsijil-3.0.dev0/aleksis/apps/alsijil/__pycache__/models.cpython-310.pyc
--rw-r--r--   0        0        0     5142 2022-08-18 20:31:35.850040 AlekSIS-App-Alsijil-3.0.dev0/aleksis/apps/alsijil/__pycache__/preferences.cpython-310.pyc
--rw-r--r--   0        0        0     6949 2022-08-18 20:31:35.734038 AlekSIS-App-Alsijil-3.0.dev0/aleksis/apps/alsijil/__pycache__/rules.cpython-310.pyc
--rw-r--r--   0        0        0     3192 2022-08-18 20:28:10.129582 AlekSIS-App-Alsijil-3.0.dev0/aleksis/apps/alsijil/actions.py
--rw-r--r--   0        0        0      848 2022-08-18 20:28:10.129582 AlekSIS-App-Alsijil-3.0.dev0/aleksis/apps/alsijil/apps.py
--rw-r--r--   0        0        0      278 2022-08-18 20:28:10.129582 AlekSIS-App-Alsijil-3.0.dev0/aleksis/apps/alsijil/assets/UpdateStatuses.js
--rw-r--r--   0        0        0     1050 2022-08-18 20:28:10.129582 AlekSIS-App-Alsijil-3.0.dev0/aleksis/apps/alsijil/assets/components/coursebook/CourseBook.graphql
--rw-r--r--   0        0        0     2661 2022-08-18 20:28:10.133582 AlekSIS-App-Alsijil-3.0.dev0/aleksis/apps/alsijil/assets/components/coursebook/CourseBook.vue
--rw-r--r--   0        0        0      709 2022-08-18 20:28:10.133582 AlekSIS-App-Alsijil-3.0.dev0/aleksis/apps/alsijil/assets/components/coursebook/LessonDocumentation.graphql
--rw-r--r--   0        0        0     5842 2022-08-18 20:28:10.133582 AlekSIS-App-Alsijil-3.0.dev0/aleksis/apps/alsijil/assets/components/coursebook/LessonDocumentation.vue
--rw-r--r--   0        0        0    10850 2022-08-18 20:28:10.133582 AlekSIS-App-Alsijil-3.0.dev0/aleksis/apps/alsijil/assets/components/coursebook/LessonDocumentations.vue
--rw-r--r--   0        0        0    12719 2022-08-18 20:28:10.133582 AlekSIS-App-Alsijil-3.0.dev0/aleksis/apps/alsijil/assets/components/coursebook/PersonalNotes.vue
--rw-r--r--   0        0        0     2252 2022-08-18 20:28:10.133582 AlekSIS-App-Alsijil-3.0.dev0/aleksis/apps/alsijil/assets/components/coursebook/UpdateIndicator.vue
--rw-r--r--   0        0        0      172 2022-08-18 20:28:10.133582 AlekSIS-App-Alsijil-3.0.dev0/aleksis/apps/alsijil/assets/index.js
--rw-r--r--   0        0        0     6039 2022-08-18 20:28:10.133582 AlekSIS-App-Alsijil-3.0.dev0/aleksis/apps/alsijil/data_checks.py
--rw-r--r--   0        0        0     1628 2022-08-18 20:28:10.137582 AlekSIS-App-Alsijil-3.0.dev0/aleksis/apps/alsijil/filters.py
--rw-r--r--   0        0        0    14927 2022-08-18 20:28:10.137582 AlekSIS-App-Alsijil-3.0.dev0/aleksis/apps/alsijil/forms.py
--rw-r--r--   0        0        0      463 2022-08-18 20:31:35.886041 AlekSIS-App-Alsijil-3.0.dev0/aleksis/apps/alsijil/locale/ar/LC_MESSAGES/django.mo
--rw-r--r--   0        0        0    46822 2022-08-18 20:28:10.137582 AlekSIS-App-Alsijil-3.0.dev0/aleksis/apps/alsijil/locale/ar/LC_MESSAGES/django.po
--rw-r--r--   0        0        0    25907 2022-08-18 20:31:35.898041 AlekSIS-App-Alsijil-3.0.dev0/aleksis/apps/alsijil/locale/de_DE/LC_MESSAGES/django.mo
--rw-r--r--   0        0        0    59688 2022-08-18 20:28:10.137582 AlekSIS-App-Alsijil-3.0.dev0/aleksis/apps/alsijil/locale/de_DE/LC_MESSAGES/django.po
--rw-r--r--   0        0        0     2793 2022-08-18 20:31:35.870041 AlekSIS-App-Alsijil-3.0.dev0/aleksis/apps/alsijil/locale/fr/LC_MESSAGES/django.mo
--rw-r--r--   0        0        0    54052 2022-08-18 20:28:10.137582 AlekSIS-App-Alsijil-3.0.dev0/aleksis/apps/alsijil/locale/fr/LC_MESSAGES/django.po
--rw-r--r--   0        0        0      732 2022-08-18 20:31:35.890041 AlekSIS-App-Alsijil-3.0.dev0/aleksis/apps/alsijil/locale/la/LC_MESSAGES/django.mo
--rw-r--r--   0        0        0    47314 2022-08-18 20:28:10.137582 AlekSIS-App-Alsijil-3.0.dev0/aleksis/apps/alsijil/locale/la/LC_MESSAGES/django.po
--rw-r--r--   0        0        0      337 2022-08-18 20:31:35.882041 AlekSIS-App-Alsijil-3.0.dev0/aleksis/apps/alsijil/locale/nb_NO/LC_MESSAGES/django.mo
--rw-r--r--   0        0        0    46692 2022-08-18 20:28:10.141582 AlekSIS-App-Alsijil-3.0.dev0/aleksis/apps/alsijil/locale/nb_NO/LC_MESSAGES/django.po
--rw-r--r--   0        0        0    30658 2022-08-18 20:31:35.882041 AlekSIS-App-Alsijil-3.0.dev0/aleksis/apps/alsijil/locale/ru/LC_MESSAGES/django.mo
--rw-r--r--   0        0        0    63117 2022-08-18 20:28:10.141582 AlekSIS-App-Alsijil-3.0.dev0/aleksis/apps/alsijil/locale/ru/LC_MESSAGES/django.po
--rw-r--r--   0        0        0      337 2022-08-18 20:31:35.898041 AlekSIS-App-Alsijil-3.0.dev0/aleksis/apps/alsijil/locale/tr_TR/LC_MESSAGES/django.mo
--rw-r--r--   0        0        0    46692 2022-08-18 20:28:10.141582 AlekSIS-App-Alsijil-3.0.dev0/aleksis/apps/alsijil/locale/tr_TR/LC_MESSAGES/django.po
--rw-r--r--   0        0        0    30046 2022-08-18 20:31:35.874041 AlekSIS-App-Alsijil-3.0.dev0/aleksis/apps/alsijil/locale/uk/LC_MESSAGES/django.mo
--rw-r--r--   0        0        0    66284 2022-08-18 20:28:10.141582 AlekSIS-App-Alsijil-3.0.dev0/aleksis/apps/alsijil/locale/uk/LC_MESSAGES/django.po
--rw-r--r--   0        0        0     6289 2022-08-18 20:28:10.141582 AlekSIS-App-Alsijil-3.0.dev0/aleksis/apps/alsijil/managers.py
--rw-r--r--   0        0        0     6086 2022-08-18 20:28:10.141582 AlekSIS-App-Alsijil-3.0.dev0/aleksis/apps/alsijil/menus.py
--rw-r--r--   0        0        0     7046 2022-08-18 20:28:10.141582 AlekSIS-App-Alsijil-3.0.dev0/aleksis/apps/alsijil/migrations/0001_initial.py
--rw-r--r--   0        0        0     2240 2022-08-18 20:28:10.141582 AlekSIS-App-Alsijil-3.0.dev0/aleksis/apps/alsijil/migrations/0002_excuse_type.py
--rw-r--r--   0        0        0     2162 2022-08-18 20:28:10.145582 AlekSIS-App-Alsijil-3.0.dev0/aleksis/apps/alsijil/migrations/0003_extra_mark.py
--rw-r--r--   0        0        0      463 2022-08-18 20:28:10.145582 AlekSIS-App-Alsijil-3.0.dev0/aleksis/apps/alsijil/migrations/0004_group_notes.py
--rw-r--r--   0        0        0      941 2022-08-18 20:28:10.145582 AlekSIS-App-Alsijil-3.0.dev0/aleksis/apps/alsijil/migrations/0005_groups_of_person.py
--rw-r--r--   0        0        0      283 2022-08-18 20:28:10.145582 AlekSIS-App-Alsijil-3.0.dev0/aleksis/apps/alsijil/migrations/0006_delete_personal_notes_filter.py
--rw-r--r--   0        0        0     1684 2022-08-18 20:28:10.145582 AlekSIS-App-Alsijil-3.0.dev0/aleksis/apps/alsijil/migrations/0007_personal_note_lesson_documentation_year.py
--rw-r--r--   0        0        0      996 2022-08-18 20:28:10.145582 AlekSIS-App-Alsijil-3.0.dev0/aleksis/apps/alsijil/migrations/0008_global_permissions.py
--rw-r--r--   0        0        0     2761 2022-08-18 20:28:10.149582 AlekSIS-App-Alsijil-3.0.dev0/aleksis/apps/alsijil/migrations/0009_group_roles.py
--rw-r--r--   0        0        0     4948 2022-08-18 20:28:10.149582 AlekSIS-App-Alsijil-3.0.dev0/aleksis/apps/alsijil/migrations/0010_events_extra_lessons.py
--rw-r--r--   0        0        0      629 2022-08-18 20:28:10.149582 AlekSIS-App-Alsijil-3.0.dev0/aleksis/apps/alsijil/migrations/0011_tardiness_positive.py
--rw-r--r--   0        0        0      648 2022-08-18 20:28:10.149582 AlekSIS-App-Alsijil-3.0.dev0/aleksis/apps/alsijil/migrations/0012_unique_relation.py
--rw-r--r--   0        0        0     1904 2022-08-18 20:28:10.149582 AlekSIS-App-Alsijil-3.0.dev0/aleksis/apps/alsijil/migrations/0013_fix_uniqueness_per_site.py
--rw-r--r--   0        0        0     1026 2022-08-18 20:28:10.153582 AlekSIS-App-Alsijil-3.0.dev0/aleksis/apps/alsijil/migrations/0014_fix_unique_lesson_documentation.py
--rw-r--r--   0        0        0     1009 2022-08-18 20:28:10.153582 AlekSIS-App-Alsijil-3.0.dev0/aleksis/apps/alsijil/migrations/0015_fix_unique_personal_note.py
--rw-r--r--   0        0        0      579 2022-08-18 20:28:10.153582 AlekSIS-App-Alsijil-3.0.dev0/aleksis/apps/alsijil/migrations/0016_add_not_counted_excuse_types.py
--rw-r--r--   0        0        0        0 2022-08-18 20:28:10.153582 AlekSIS-App-Alsijil-3.0.dev0/aleksis/apps/alsijil/migrations/__init__.py
--rw-r--r--   0        0        0    17436 2022-08-18 20:28:10.153582 AlekSIS-App-Alsijil-3.0.dev0/aleksis/apps/alsijil/model_extensions.py
--rw-r--r--   0        0        0    18173 2022-08-18 20:28:10.153582 AlekSIS-App-Alsijil-3.0.dev0/aleksis/apps/alsijil/models.py
--rw-r--r--   0        0        0     5072 2022-08-18 20:28:10.153582 AlekSIS-App-Alsijil-3.0.dev0/aleksis/apps/alsijil/preferences.py
--rw-r--r--   0        0        0    13096 2022-08-18 20:28:10.157582 AlekSIS-App-Alsijil-3.0.dev0/aleksis/apps/alsijil/rules.py
--rw-r--r--   0        0        0     8238 2022-08-18 20:28:10.157582 AlekSIS-App-Alsijil-3.0.dev0/aleksis/apps/alsijil/schema.py
--rw-r--r--   0        0        0     1025 2022-08-18 20:28:10.157582 AlekSIS-App-Alsijil-3.0.dev0/aleksis/apps/alsijil/static/css/alsijil/alsijil.css
--rw-r--r--   0        0        0     1064 2022-08-18 20:28:10.157582 AlekSIS-App-Alsijil-3.0.dev0/aleksis/apps/alsijil/static/css/alsijil/full_register.css
--rw-r--r--   0        0        0     2893 2022-08-18 20:28:10.157582 AlekSIS-App-Alsijil-3.0.dev0/aleksis/apps/alsijil/static/css/alsijil/lesson.css
--rw-r--r--   0        0        0     1828 2022-08-18 20:28:10.161582 AlekSIS-App-Alsijil-3.0.dev0/aleksis/apps/alsijil/static/css/alsijil/person.css
--rw-r--r--   0        0        0     2139 2022-08-18 20:28:10.161582 AlekSIS-App-Alsijil-3.0.dev0/aleksis/apps/alsijil/static/css/alsijil/week_view.css
--rw-r--r--   0        0        0      643 2022-08-18 20:28:10.161582 AlekSIS-App-Alsijil-3.0.dev0/aleksis/apps/alsijil/static/js/alsijil/week_view.js
--rw-r--r--   0        0        0     7497 2022-08-18 20:28:10.161582 AlekSIS-App-Alsijil-3.0.dev0/aleksis/apps/alsijil/tables.py
--rw-r--r--   0        0        0      742 2022-08-18 20:28:10.161582 AlekSIS-App-Alsijil-3.0.dev0/aleksis/apps/alsijil/templates/alsijil/absences/register.html
--rw-r--r--   0        0        0     3102 2022-08-18 20:28:10.161582 AlekSIS-App-Alsijil-3.0.dev0/aleksis/apps/alsijil/templates/alsijil/absences/register_confirm.html
--rw-r--r--   0        0        0      574 2022-08-18 20:28:10.161582 AlekSIS-App-Alsijil-3.0.dev0/aleksis/apps/alsijil/templates/alsijil/class_register/all_objects.html
--rw-r--r--   0        0        0      524 2022-08-18 20:28:10.161582 AlekSIS-App-Alsijil-3.0.dev0/aleksis/apps/alsijil/templates/alsijil/class_register/coursebook.html
--rw-r--r--   0        0        0     3889 2022-08-18 20:28:10.161582 AlekSIS-App-Alsijil-3.0.dev0/aleksis/apps/alsijil/templates/alsijil/class_register/groups.html
--rw-r--r--   0        0        0     7223 2022-08-18 20:28:10.165583 AlekSIS-App-Alsijil-3.0.dev0/aleksis/apps/alsijil/templates/alsijil/class_register/lesson.html
--rw-r--r--   0        0        0     7414 2022-08-18 20:28:10.165583 AlekSIS-App-Alsijil-3.0.dev0/aleksis/apps/alsijil/templates/alsijil/class_register/person.html
--rw-r--r--   0        0        0     2312 2022-08-18 20:28:10.165583 AlekSIS-App-Alsijil-3.0.dev0/aleksis/apps/alsijil/templates/alsijil/class_register/persons.html
--rw-r--r--   0        0        0     1810 2022-08-18 20:28:10.165583 AlekSIS-App-Alsijil-3.0.dev0/aleksis/apps/alsijil/templates/alsijil/class_register/select_coursebook.html
--rw-r--r--   0        0        0     1859 2022-08-18 20:28:10.165583 AlekSIS-App-Alsijil-3.0.dev0/aleksis/apps/alsijil/templates/alsijil/class_register/students_list.html
--rw-r--r--   0        0        0    20937 2022-08-18 20:28:10.165583 AlekSIS-App-Alsijil-3.0.dev0/aleksis/apps/alsijil/templates/alsijil/class_register/week_view.html
--rw-r--r--   0        0        0      506 2022-08-18 20:28:10.165583 AlekSIS-App-Alsijil-3.0.dev0/aleksis/apps/alsijil/templates/alsijil/excuse_type/create.html
--rw-r--r--   0        0        0      451 2022-08-18 20:28:10.165583 AlekSIS-App-Alsijil-3.0.dev0/aleksis/apps/alsijil/templates/alsijil/excuse_type/edit.html
--rw-r--r--   0        0        0      707 2022-08-18 20:28:10.169582 AlekSIS-App-Alsijil-3.0.dev0/aleksis/apps/alsijil/templates/alsijil/excuse_type/list.html
--rw-r--r--   0        0        0      364 2022-08-18 20:28:10.169582 AlekSIS-App-Alsijil-3.0.dev0/aleksis/apps/alsijil/templates/alsijil/excuse_type/warning.html
--rw-r--r--   0        0        0      465 2022-08-18 20:28:10.169582 AlekSIS-App-Alsijil-3.0.dev0/aleksis/apps/alsijil/templates/alsijil/extra_mark/create.html
--rw-r--r--   0        0        0      449 2022-08-18 20:28:10.169582 AlekSIS-App-Alsijil-3.0.dev0/aleksis/apps/alsijil/templates/alsijil/extra_mark/edit.html
--rw-r--r--   0        0        0      527 2022-08-18 20:28:10.169582 AlekSIS-App-Alsijil-3.0.dev0/aleksis/apps/alsijil/templates/alsijil/extra_mark/list.html
--rw-r--r--   0        0        0     1009 2022-08-18 20:28:10.169582 AlekSIS-App-Alsijil-3.0.dev0/aleksis/apps/alsijil/templates/alsijil/group_role/assign.html
--rw-r--r--   0        0        0     3082 2022-08-18 20:28:10.169582 AlekSIS-App-Alsijil-3.0.dev0/aleksis/apps/alsijil/templates/alsijil/group_role/assigned_list.html
--rw-r--r--   0        0        0      286 2022-08-18 20:28:10.169582 AlekSIS-App-Alsijil-3.0.dev0/aleksis/apps/alsijil/templates/alsijil/group_role/chip.html
--rw-r--r--   0        0        0      451 2022-08-18 20:28:10.169582 AlekSIS-App-Alsijil-3.0.dev0/aleksis/apps/alsijil/templates/alsijil/group_role/create.html
--rw-r--r--   0        0        0      471 2022-08-18 20:28:10.169582 AlekSIS-App-Alsijil-3.0.dev0/aleksis/apps/alsijil/templates/alsijil/group_role/edit.html
--rw-r--r--   0        0        0      488 2022-08-18 20:28:10.173583 AlekSIS-App-Alsijil-3.0.dev0/aleksis/apps/alsijil/templates/alsijil/group_role/edit_assignment.html
--rw-r--r--   0        0        0      651 2022-08-18 20:28:10.173583 AlekSIS-App-Alsijil-3.0.dev0/aleksis/apps/alsijil/templates/alsijil/group_role/list.html
--rw-r--r--   0        0        0     1708 2022-08-18 20:28:10.173583 AlekSIS-App-Alsijil-3.0.dev0/aleksis/apps/alsijil/templates/alsijil/group_role/partials/assigned_roles.html
--rw-r--r--   0        0        0      365 2022-08-18 20:28:10.173583 AlekSIS-App-Alsijil-3.0.dev0/aleksis/apps/alsijil/templates/alsijil/group_role/partials/assignment.html
--rw-r--r--   0        0        0     1034 2022-08-18 20:28:10.173583 AlekSIS-App-Alsijil-3.0.dev0/aleksis/apps/alsijil/templates/alsijil/group_role/partials/assignment_options.html
--rw-r--r--   0        0        0      364 2022-08-18 20:28:10.173583 AlekSIS-App-Alsijil-3.0.dev0/aleksis/apps/alsijil/templates/alsijil/group_role/warning.html
--rw-r--r--   0        0        0      194 2022-08-18 20:28:10.173583 AlekSIS-App-Alsijil-3.0.dev0/aleksis/apps/alsijil/templates/alsijil/notifications/check.html
--rw-r--r--   0        0        0      501 2022-08-18 20:28:10.173583 AlekSIS-App-Alsijil-3.0.dev0/aleksis/apps/alsijil/templates/alsijil/partials/absences.html
--rw-r--r--   0        0        0     2661 2022-08-18 20:28:10.173583 AlekSIS-App-Alsijil-3.0.dev0/aleksis/apps/alsijil/templates/alsijil/partials/legend.html
--rw-r--r--   0        0        0     2630 2022-08-18 20:28:10.173583 AlekSIS-App-Alsijil-3.0.dev0/aleksis/apps/alsijil/templates/alsijil/partials/lesson/heading.html
--rw-r--r--   0        0        0     1404 2022-08-18 20:28:10.173583 AlekSIS-App-Alsijil-3.0.dev0/aleksis/apps/alsijil/templates/alsijil/partials/lesson/prev_next.html
--rw-r--r--   0        0        0     1852 2022-08-18 20:28:10.173583 AlekSIS-App-Alsijil-3.0.dev0/aleksis/apps/alsijil/templates/alsijil/partials/lesson/tabs/documentation.html
--rw-r--r--   0        0        0      560 2022-08-18 20:28:10.173583 AlekSIS-App-Alsijil-3.0.dev0/aleksis/apps/alsijil/templates/alsijil/partials/lesson/tabs/more.html
--rw-r--r--   0        0        0     5474 2022-08-18 20:28:10.173583 AlekSIS-App-Alsijil-3.0.dev0/aleksis/apps/alsijil/templates/alsijil/partials/lesson/tabs/notes.html
--rw-r--r--   0        0        0     1885 2022-08-18 20:28:10.173583 AlekSIS-App-Alsijil-3.0.dev0/aleksis/apps/alsijil/templates/alsijil/partials/lesson/tabs/previous_lesson.html
--rw-r--r--   0        0        0     3961 2022-08-18 20:28:10.177583 AlekSIS-App-Alsijil-3.0.dev0/aleksis/apps/alsijil/templates/alsijil/partials/lesson/tabs/seating_plan.html
--rw-r--r--   0        0        0     2020 2022-08-18 20:28:10.177583 AlekSIS-App-Alsijil-3.0.dev0/aleksis/apps/alsijil/templates/alsijil/partials/lesson_status.html
--rw-r--r--   0        0        0      411 2022-08-18 20:28:10.177583 AlekSIS-App-Alsijil-3.0.dev0/aleksis/apps/alsijil/templates/alsijil/partials/lesson_status_icon.html
--rw-r--r--   0        0        0     1340 2022-08-18 20:28:10.177583 AlekSIS-App-Alsijil-3.0.dev0/aleksis/apps/alsijil/templates/alsijil/partials/objects_table.html
--rw-r--r--   0        0        0     4954 2022-08-18 20:28:10.177583 AlekSIS-App-Alsijil-3.0.dev0/aleksis/apps/alsijil/templates/alsijil/partials/persons_with_stats.html
--rw-r--r--   0        0        0      277 2022-08-18 20:28:10.177583 AlekSIS-App-Alsijil-3.0.dev0/aleksis/apps/alsijil/templates/alsijil/partials/tardinesses.html
--rw-r--r--   0        0        0    17539 2022-08-18 20:28:10.177583 AlekSIS-App-Alsijil-3.0.dev0/aleksis/apps/alsijil/templates/alsijil/print/full_register.html
--rw-r--r--   0        0        0        0 2022-08-18 20:28:10.177583 AlekSIS-App-Alsijil-3.0.dev0/aleksis/apps/alsijil/templatetags/__init__.py
--rw-r--r--   0        0        0      353 2022-08-18 20:28:10.177583 AlekSIS-App-Alsijil-3.0.dev0/aleksis/apps/alsijil/templatetags/time_helpers.py
--rw-r--r--   0        0        0     3598 2022-08-18 20:28:10.177583 AlekSIS-App-Alsijil-3.0.dev0/aleksis/apps/alsijil/tests/test_actions.py
--rw-r--r--   0        0        0     4545 2022-08-18 20:28:10.177583 AlekSIS-App-Alsijil-3.0.dev0/aleksis/apps/alsijil/urls.py
--rw-r--r--   0        0        0     9671 2022-08-18 20:31:35.738038 AlekSIS-App-Alsijil-3.0.dev0/aleksis/apps/alsijil/util/__pycache__/predicates.cpython-310.pyc
--rw-r--r--   0        0        0    16315 2022-08-18 20:28:10.177583 AlekSIS-App-Alsijil-3.0.dev0/aleksis/apps/alsijil/util/alsijil_helpers.py
--rw-r--r--   0        0        0     9889 2022-08-18 20:28:10.181583 AlekSIS-App-Alsijil-3.0.dev0/aleksis/apps/alsijil/util/predicates.py
--rw-r--r--   0        0        0    58947 2022-08-18 20:28:10.181583 AlekSIS-App-Alsijil-3.0.dev0/aleksis/apps/alsijil/views.py
--rw-r--r--   0        0        0      581 2022-08-18 20:28:10.181583 AlekSIS-App-Alsijil-3.0.dev0/docs/Makefile
--rw-r--r--   0        0        0    81006 2022-08-18 20:28:10.193583 AlekSIS-App-Alsijil-3.0.dev0/docs/_static/assign_group_role.png
--rw-r--r--   0        0        0    78757 2022-08-18 20:28:10.197583 AlekSIS-App-Alsijil-3.0.dev0/docs/_static/create_excuse_type.png
--rw-r--r--   0        0        0    63748 2022-08-18 20:28:10.201583 AlekSIS-App-Alsijil-3.0.dev0/docs/_static/create_extra_mark.png
--rw-r--r--   0        0        0    62703 2022-08-18 20:28:10.201583 AlekSIS-App-Alsijil-3.0.dev0/docs/_static/edit_group_role.png
--rw-r--r--   0        0        0    84526 2022-08-18 20:28:10.201583 AlekSIS-App-Alsijil-3.0.dev0/docs/_static/excuse_types.png
--rw-r--r--   0        0        0    79794 2022-08-18 20:28:10.205583 AlekSIS-App-Alsijil-3.0.dev0/docs/_static/extra_marks.png
--rw-r--r--   0        0        0    69601 2022-08-18 20:28:10.205583 AlekSIS-App-Alsijil-3.0.dev0/docs/_static/group_roles.png
--rw-r--r--   0        0        0    86554 2022-08-18 20:28:10.209583 AlekSIS-App-Alsijil-3.0.dev0/docs/_static/lesson_documentation.png
--rw-r--r--   0        0        0    90453 2022-08-18 20:28:10.209583 AlekSIS-App-Alsijil-3.0.dev0/docs/_static/lesson_personal_notes.png
--rw-r--r--   0        0        0    77148 2022-08-18 20:28:10.209583 AlekSIS-App-Alsijil-3.0.dev0/docs/_static/lesson_version_history.png
--rw-r--r--   0        0        0   156092 2022-08-18 20:28:10.213584 AlekSIS-App-Alsijil-3.0.dev0/docs/_static/my_groups.png
--rw-r--r--   0        0        0   151265 2022-08-18 20:28:10.213584 AlekSIS-App-Alsijil-3.0.dev0/docs/_static/my_students.png
--rw-r--r--   0        0        0   109932 2022-08-18 20:28:10.229584 AlekSIS-App-Alsijil-3.0.dev0/docs/_static/overview_lessons.png
--rw-r--r--   0        0        0    93584 2022-08-18 20:28:10.229584 AlekSIS-App-Alsijil-3.0.dev0/docs/_static/overview_person.png
--rw-r--r--   0        0        0    72488 2022-08-18 20:28:10.233584 AlekSIS-App-Alsijil-3.0.dev0/docs/_static/register_absence.png
--rw-r--r--   0        0        0    92604 2022-08-18 20:28:10.233584 AlekSIS-App-Alsijil-3.0.dev0/docs/_static/register_absence_confirm.png
--rw-r--r--   0        0        0   139320 2022-08-18 20:28:10.237584 AlekSIS-App-Alsijil-3.0.dev0/docs/_static/students_list.png
--rw-r--r--   0        0        0   106128 2022-08-18 20:28:10.237584 AlekSIS-App-Alsijil-3.0.dev0/docs/_static/week_view.png
--rw-r--r--   0        0        0   107577 2022-08-18 20:28:10.241584 AlekSIS-App-Alsijil-3.0.dev0/docs/_static/week_view_personal_notes.png
--rw-r--r--   0        0        0      152 2022-08-18 20:28:10.241584 AlekSIS-App-Alsijil-3.0.dev0/docs/admin/00_index.rst
--rw-r--r--   0        0        0     1513 2022-08-18 20:28:10.241584 AlekSIS-App-Alsijil-3.0.dev0/docs/admin/30_configure.rst
--rw-r--r--   0        0        0     2345 2022-08-18 20:28:10.241584 AlekSIS-App-Alsijil-3.0.dev0/docs/admin/40_preferences.rst
--rw-r--r--   0        0        0     6407 2022-08-18 20:28:10.241584 AlekSIS-App-Alsijil-3.0.dev0/docs/conf.py
--rw-r--r--   0        0        0      528 2022-08-18 20:28:10.241584 AlekSIS-App-Alsijil-3.0.dev0/docs/index.rst
--rw-r--r--   0        0        0      787 2022-08-18 20:28:10.241584 AlekSIS-App-Alsijil-3.0.dev0/docs/make.bat
--rw-r--r--   0        0        0       76 2022-08-18 20:28:10.241584 AlekSIS-App-Alsijil-3.0.dev0/docs/user/00_index.rst
--rw-r--r--   0        0        0     2330 2022-08-18 20:28:10.241584 AlekSIS-App-Alsijil-3.0.dev0/docs/user/10_basic.rst
--rw-r--r--   0        0        0     1437 2022-08-18 20:28:10.241584 AlekSIS-App-Alsijil-3.0.dev0/docs/user/15_concepts.rst
--rw-r--r--   0        0        0     2939 2022-08-18 20:28:10.241584 AlekSIS-App-Alsijil-3.0.dev0/docs/user/20_overview.rst
--rw-r--r--   0        0        0     2833 2022-08-18 20:28:10.245584 AlekSIS-App-Alsijil-3.0.dev0/docs/user/21_lesson.rst
--rw-r--r--   0        0        0      308 2022-08-18 20:28:10.245584 AlekSIS-App-Alsijil-3.0.dev0/docs/user/25_group_roles.rst
--rw-r--r--   0        0        0      591 2022-08-18 20:28:10.245584 AlekSIS-App-Alsijil-3.0.dev0/docs/user/40_export.rst
--rw-r--r--   0        0        0     2104 2022-08-18 20:29:07.162818 AlekSIS-App-Alsijil-3.0.dev0/pyproject.toml
--rw-r--r--   0        0        0     2344 2022-08-18 20:28:10.249584 AlekSIS-App-Alsijil-3.0.dev0/tox.ini
--rw-r--r--   0        0        0     4768 2022-08-18 20:31:37.564669 AlekSIS-App-Alsijil-3.0.dev0/setup.py
--rw-r--r--   0        0        0     3429 2022-08-18 20:31:37.565028 AlekSIS-App-Alsijil-3.0.dev0/PKG-INFO
+-rw-r--r--   0        0        0     9564 2023-03-01 19:31:48.011203 aleksis_app_alsijil-3.0b0/CHANGELOG.rst
+-rw-r--r--   0        0        0    14361 2023-03-01 19:31:48.011203 aleksis_app_alsijil-3.0b0/LICENCE.rst
+-rw-r--r--   0        0        0     2096 2023-03-01 19:31:48.011203 aleksis_app_alsijil-3.0b0/README.rst
+-rw-r--r--   0        0        0      153 2023-03-01 19:31:48.011203 aleksis_app_alsijil-3.0b0/aleksis/apps/alsijil/__init__.py
+-rw-r--r--   0        0        0      447 2023-03-01 19:33:56.558946 aleksis_app_alsijil-3.0b0/aleksis/apps/alsijil/__pycache__/__init__.cpython-311.pyc
+-rw-r--r--   0        0        0     1236 2023-03-01 19:33:56.978945 aleksis_app_alsijil-3.0b0/aleksis/apps/alsijil/__pycache__/apps.cpython-311.pyc
+-rw-r--r--   0        0        0    10157 2023-03-01 19:33:57.830943 aleksis_app_alsijil-3.0b0/aleksis/apps/alsijil/__pycache__/data_checks.cpython-311.pyc
+-rw-r--r--   0        0        0    11056 2023-03-01 19:33:57.830943 aleksis_app_alsijil-3.0b0/aleksis/apps/alsijil/__pycache__/managers.cpython-311.pyc
+-rw-r--r--   0        0        0    24420 2023-03-01 19:33:58.018942 aleksis_app_alsijil-3.0b0/aleksis/apps/alsijil/__pycache__/model_extensions.cpython-311.pyc
+-rw-r--r--   0        0        0    25759 2023-03-01 19:33:57.826943 aleksis_app_alsijil-3.0b0/aleksis/apps/alsijil/__pycache__/models.cpython-311.pyc
+-rw-r--r--   0        0        0     8382 2023-03-01 19:33:58.198942 aleksis_app_alsijil-3.0b0/aleksis/apps/alsijil/__pycache__/preferences.cpython-311.pyc
+-rw-r--r--   0        0        0    11463 2023-03-01 19:33:57.970943 aleksis_app_alsijil-3.0b0/aleksis/apps/alsijil/__pycache__/rules.cpython-311.pyc
+-rw-r--r--   0        0        0     3197 2023-03-01 19:31:48.011203 aleksis_app_alsijil-3.0b0/aleksis/apps/alsijil/actions.py
+-rw-r--r--   0        0        0      789 2023-03-01 19:31:48.011203 aleksis_app_alsijil-3.0b0/aleksis/apps/alsijil/apps.py
+-rw-r--r--   0        0        0     6057 2023-03-01 19:31:48.011203 aleksis_app_alsijil-3.0b0/aleksis/apps/alsijil/data_checks.py
+-rw-r--r--   0        0        0     1653 2023-03-01 19:31:48.011203 aleksis_app_alsijil-3.0b0/aleksis/apps/alsijil/filters.py
+-rw-r--r--   0        0        0    15807 2023-03-01 19:31:48.011203 aleksis_app_alsijil-3.0b0/aleksis/apps/alsijil/forms.py
+-rw-r--r--   0        0        0    13943 2023-03-01 19:31:48.015203 aleksis_app_alsijil-3.0b0/aleksis/apps/alsijil/frontend/index.js
+-rw-r--r--   0        0        0      803 2023-03-01 19:31:48.015203 aleksis_app_alsijil-3.0b0/aleksis/apps/alsijil/frontend/messages/de.json
+-rw-r--r--   0        0        0      725 2023-03-01 19:31:48.015203 aleksis_app_alsijil-3.0b0/aleksis/apps/alsijil/frontend/messages/en.json
+-rw-r--r--   0        0        0      930 2023-03-01 19:31:48.015203 aleksis_app_alsijil-3.0b0/aleksis/apps/alsijil/frontend/messages/ru.json
+-rw-r--r--   0        0        0      910 2023-03-01 19:31:48.015203 aleksis_app_alsijil-3.0b0/aleksis/apps/alsijil/frontend/messages/uk.json
+-rw-r--r--   0        0        0      463 2023-03-01 19:33:58.366942 aleksis_app_alsijil-3.0b0/aleksis/apps/alsijil/locale/ar/LC_MESSAGES/django.mo
+-rw-r--r--   0        0        0    46822 2023-03-01 19:31:48.015203 aleksis_app_alsijil-3.0b0/aleksis/apps/alsijil/locale/ar/LC_MESSAGES/django.po
+-rw-r--r--   0        0        0    25907 2023-03-01 19:33:58.354942 aleksis_app_alsijil-3.0b0/aleksis/apps/alsijil/locale/de_DE/LC_MESSAGES/django.mo
+-rw-r--r--   0        0        0    59688 2023-03-01 19:31:48.019203 aleksis_app_alsijil-3.0b0/aleksis/apps/alsijil/locale/de_DE/LC_MESSAGES/django.po
+-rw-r--r--   0        0        0     2793 2023-03-01 19:33:58.354942 aleksis_app_alsijil-3.0b0/aleksis/apps/alsijil/locale/fr/LC_MESSAGES/django.mo
+-rw-r--r--   0        0        0    54052 2023-03-01 19:31:48.019203 aleksis_app_alsijil-3.0b0/aleksis/apps/alsijil/locale/fr/LC_MESSAGES/django.po
+-rw-r--r--   0        0        0      732 2023-03-01 19:33:58.342942 aleksis_app_alsijil-3.0b0/aleksis/apps/alsijil/locale/la/LC_MESSAGES/django.mo
+-rw-r--r--   0        0        0    47314 2023-03-01 19:31:48.019203 aleksis_app_alsijil-3.0b0/aleksis/apps/alsijil/locale/la/LC_MESSAGES/django.po
+-rw-r--r--   0        0        0      337 2023-03-01 19:33:58.362942 aleksis_app_alsijil-3.0b0/aleksis/apps/alsijil/locale/nb_NO/LC_MESSAGES/django.mo
+-rw-r--r--   0        0        0    46692 2023-03-01 19:31:48.019203 aleksis_app_alsijil-3.0b0/aleksis/apps/alsijil/locale/nb_NO/LC_MESSAGES/django.po
+-rw-r--r--   0        0        0    31812 2023-03-01 19:33:58.358942 aleksis_app_alsijil-3.0b0/aleksis/apps/alsijil/locale/ru/LC_MESSAGES/django.mo
+-rw-r--r--   0        0        0    63294 2023-03-01 19:31:48.019203 aleksis_app_alsijil-3.0b0/aleksis/apps/alsijil/locale/ru/LC_MESSAGES/django.po
+-rw-r--r--   0        0        0      337 2023-03-01 19:33:58.350942 aleksis_app_alsijil-3.0b0/aleksis/apps/alsijil/locale/tr_TR/LC_MESSAGES/django.mo
+-rw-r--r--   0        0        0    46692 2023-03-01 19:31:48.019203 aleksis_app_alsijil-3.0b0/aleksis/apps/alsijil/locale/tr_TR/LC_MESSAGES/django.po
+-rw-r--r--   0        0        0    31219 2023-03-01 19:33:58.350942 aleksis_app_alsijil-3.0b0/aleksis/apps/alsijil/locale/uk/LC_MESSAGES/django.mo
+-rw-r--r--   0        0        0    66679 2023-03-01 19:31:48.019203 aleksis_app_alsijil-3.0b0/aleksis/apps/alsijil/locale/uk/LC_MESSAGES/django.po
+-rw-r--r--   0        0        0     6294 2023-03-01 19:31:48.019203 aleksis_app_alsijil-3.0b0/aleksis/apps/alsijil/managers.py
+-rw-r--r--   0        0        0     7046 2023-03-01 19:31:48.019203 aleksis_app_alsijil-3.0b0/aleksis/apps/alsijil/migrations/0001_initial.py
+-rw-r--r--   0        0        0     2240 2023-03-01 19:31:48.019203 aleksis_app_alsijil-3.0b0/aleksis/apps/alsijil/migrations/0002_excuse_type.py
+-rw-r--r--   0        0        0     2162 2023-03-01 19:31:48.019203 aleksis_app_alsijil-3.0b0/aleksis/apps/alsijil/migrations/0003_extra_mark.py
+-rw-r--r--   0        0        0      463 2023-03-01 19:31:48.019203 aleksis_app_alsijil-3.0b0/aleksis/apps/alsijil/migrations/0004_group_notes.py
+-rw-r--r--   0        0        0      941 2023-03-01 19:31:48.019203 aleksis_app_alsijil-3.0b0/aleksis/apps/alsijil/migrations/0005_groups_of_person.py
+-rw-r--r--   0        0        0      283 2023-03-01 19:31:48.019203 aleksis_app_alsijil-3.0b0/aleksis/apps/alsijil/migrations/0006_delete_personal_notes_filter.py
+-rw-r--r--   0        0        0     1684 2023-03-01 19:31:48.019203 aleksis_app_alsijil-3.0b0/aleksis/apps/alsijil/migrations/0007_personal_note_lesson_documentation_year.py
+-rw-r--r--   0        0        0      996 2023-03-01 19:31:48.019203 aleksis_app_alsijil-3.0b0/aleksis/apps/alsijil/migrations/0008_global_permissions.py
+-rw-r--r--   0        0        0     2761 2023-03-01 19:31:48.019203 aleksis_app_alsijil-3.0b0/aleksis/apps/alsijil/migrations/0009_group_roles.py
+-rw-r--r--   0        0        0     4948 2023-03-01 19:31:48.019203 aleksis_app_alsijil-3.0b0/aleksis/apps/alsijil/migrations/0010_events_extra_lessons.py
+-rw-r--r--   0        0        0      629 2023-03-01 19:31:48.019203 aleksis_app_alsijil-3.0b0/aleksis/apps/alsijil/migrations/0011_tardiness_positive.py
+-rw-r--r--   0        0        0      648 2023-03-01 19:31:48.019203 aleksis_app_alsijil-3.0b0/aleksis/apps/alsijil/migrations/0012_unique_relation.py
+-rw-r--r--   0        0        0     1904 2023-03-01 19:31:48.019203 aleksis_app_alsijil-3.0b0/aleksis/apps/alsijil/migrations/0013_fix_uniqueness_per_site.py
+-rw-r--r--   0        0        0     1026 2023-03-01 19:31:48.019203 aleksis_app_alsijil-3.0b0/aleksis/apps/alsijil/migrations/0014_fix_unique_lesson_documentation.py
+-rw-r--r--   0        0        0     1009 2023-03-01 19:31:48.019203 aleksis_app_alsijil-3.0b0/aleksis/apps/alsijil/migrations/0015_fix_unique_personal_note.py
+-rw-r--r--   0        0        0      579 2023-03-01 19:31:48.019203 aleksis_app_alsijil-3.0b0/aleksis/apps/alsijil/migrations/0016_add_not_counted_excuse_types.py
+-rw-r--r--   0        0        0      389 2023-03-01 19:31:48.019203 aleksis_app_alsijil-3.0b0/aleksis/apps/alsijil/migrations/0017_rename_late_to_tardiness.py
+-rw-r--r--   0        0        0        0 2023-03-01 19:31:48.019203 aleksis_app_alsijil-3.0b0/aleksis/apps/alsijil/migrations/__init__.py
+-rw-r--r--   0        0        0    17661 2023-03-01 19:31:48.019203 aleksis_app_alsijil-3.0b0/aleksis/apps/alsijil/model_extensions.py
+-rw-r--r--   0        0        0    18359 2023-03-01 19:31:48.023203 aleksis_app_alsijil-3.0b0/aleksis/apps/alsijil/models.py
+-rw-r--r--   0        0        0     5283 2023-03-01 19:31:48.023203 aleksis_app_alsijil-3.0b0/aleksis/apps/alsijil/preferences.py
+-rw-r--r--   0        0        0    13123 2023-03-01 19:31:48.023203 aleksis_app_alsijil-3.0b0/aleksis/apps/alsijil/rules.py
+-rw-r--r--   0        0        0      977 2023-03-01 19:31:48.023203 aleksis_app_alsijil-3.0b0/aleksis/apps/alsijil/static/css/alsijil/alsijil.css
+-rw-r--r--   0        0        0     1020 2023-03-01 19:31:48.023203 aleksis_app_alsijil-3.0b0/aleksis/apps/alsijil/static/css/alsijil/full_register.css
+-rw-r--r--   0        0        0     2709 2023-03-01 19:31:48.023203 aleksis_app_alsijil-3.0b0/aleksis/apps/alsijil/static/css/alsijil/lesson.css
+-rw-r--r--   0        0        0     1700 2023-03-01 19:31:48.023203 aleksis_app_alsijil-3.0b0/aleksis/apps/alsijil/static/css/alsijil/person.css
+-rw-r--r--   0        0        0     2038 2023-03-01 19:31:48.023203 aleksis_app_alsijil-3.0b0/aleksis/apps/alsijil/static/css/alsijil/week_view.css
+-rw-r--r--   0        0        0      611 2023-03-01 19:31:48.023203 aleksis_app_alsijil-3.0b0/aleksis/apps/alsijil/static/js/alsijil/week_view.js
+-rw-r--r--   0        0        0     7512 2023-03-01 19:31:48.023203 aleksis_app_alsijil-3.0b0/aleksis/apps/alsijil/tables.py
+-rw-r--r--   0        0        0     7170 2023-03-01 19:31:48.023203 aleksis_app_alsijil-3.0b0/aleksis/apps/alsijil/tasks.py
+-rw-r--r--   0        0        0      870 2023-03-01 19:31:48.023203 aleksis_app_alsijil-3.0b0/aleksis/apps/alsijil/templates/alsijil/absences/register.html
+-rw-r--r--   0        0        0     3336 2023-03-01 19:31:48.023203 aleksis_app_alsijil-3.0b0/aleksis/apps/alsijil/templates/alsijil/absences/register_confirm.html
+-rw-r--r--   0        0        0      574 2023-03-01 19:31:48.023203 aleksis_app_alsijil-3.0b0/aleksis/apps/alsijil/templates/alsijil/class_register/all_objects.html
+-rw-r--r--   0        0        0     4183 2023-03-01 19:31:48.023203 aleksis_app_alsijil-3.0b0/aleksis/apps/alsijil/templates/alsijil/class_register/groups.html
+-rw-r--r--   0        0        0     4971 2023-03-01 19:31:48.023203 aleksis_app_alsijil-3.0b0/aleksis/apps/alsijil/templates/alsijil/class_register/lesson.html
+-rw-r--r--   0        0        0     7662 2023-03-01 19:31:48.027203 aleksis_app_alsijil-3.0b0/aleksis/apps/alsijil/templates/alsijil/class_register/person.html
+-rw-r--r--   0        0        0     2448 2023-03-01 19:31:48.027203 aleksis_app_alsijil-3.0b0/aleksis/apps/alsijil/templates/alsijil/class_register/persons.html
+-rw-r--r--   0        0        0     2021 2023-03-01 19:31:48.027203 aleksis_app_alsijil-3.0b0/aleksis/apps/alsijil/templates/alsijil/class_register/students_list.html
+-rw-r--r--   0        0        0    21343 2023-03-01 19:31:48.027203 aleksis_app_alsijil-3.0b0/aleksis/apps/alsijil/templates/alsijil/class_register/week_view.html
+-rw-r--r--   0        0        0      506 2023-03-01 19:31:48.027203 aleksis_app_alsijil-3.0b0/aleksis/apps/alsijil/templates/alsijil/excuse_type/create.html
+-rw-r--r--   0        0        0      451 2023-03-01 19:31:48.027203 aleksis_app_alsijil-3.0b0/aleksis/apps/alsijil/templates/alsijil/excuse_type/edit.html
+-rw-r--r--   0        0        0      732 2023-03-01 19:31:48.027203 aleksis_app_alsijil-3.0b0/aleksis/apps/alsijil/templates/alsijil/excuse_type/list.html
+-rw-r--r--   0        0        0      395 2023-03-01 19:31:48.027203 aleksis_app_alsijil-3.0b0/aleksis/apps/alsijil/templates/alsijil/excuse_type/warning.html
+-rw-r--r--   0        0        0      465 2023-03-01 19:31:48.027203 aleksis_app_alsijil-3.0b0/aleksis/apps/alsijil/templates/alsijil/extra_mark/create.html
+-rw-r--r--   0        0        0      449 2023-03-01 19:31:48.027203 aleksis_app_alsijil-3.0b0/aleksis/apps/alsijil/templates/alsijil/extra_mark/edit.html
+-rw-r--r--   0        0        0      553 2023-03-01 19:31:48.027203 aleksis_app_alsijil-3.0b0/aleksis/apps/alsijil/templates/alsijil/extra_mark/list.html
+-rw-r--r--   0        0        0     1045 2023-03-01 19:31:48.027203 aleksis_app_alsijil-3.0b0/aleksis/apps/alsijil/templates/alsijil/group_role/assign.html
+-rw-r--r--   0        0        0     3184 2023-03-01 19:31:48.027203 aleksis_app_alsijil-3.0b0/aleksis/apps/alsijil/templates/alsijil/group_role/assigned_list.html
+-rw-r--r--   0        0        0      322 2023-03-01 19:31:48.027203 aleksis_app_alsijil-3.0b0/aleksis/apps/alsijil/templates/alsijil/group_role/chip.html
+-rw-r--r--   0        0        0      451 2023-03-01 19:31:48.027203 aleksis_app_alsijil-3.0b0/aleksis/apps/alsijil/templates/alsijil/group_role/create.html
+-rw-r--r--   0        0        0      471 2023-03-01 19:31:48.027203 aleksis_app_alsijil-3.0b0/aleksis/apps/alsijil/templates/alsijil/group_role/edit.html
+-rw-r--r--   0        0        0      488 2023-03-01 19:31:48.027203 aleksis_app_alsijil-3.0b0/aleksis/apps/alsijil/templates/alsijil/group_role/edit_assignment.html
+-rw-r--r--   0        0        0      677 2023-03-01 19:31:48.027203 aleksis_app_alsijil-3.0b0/aleksis/apps/alsijil/templates/alsijil/group_role/list.html
+-rw-r--r--   0        0        0     1796 2023-03-01 19:31:48.027203 aleksis_app_alsijil-3.0b0/aleksis/apps/alsijil/templates/alsijil/group_role/partials/assigned_roles.html
+-rw-r--r--   0        0        0      365 2023-03-01 19:31:48.027203 aleksis_app_alsijil-3.0b0/aleksis/apps/alsijil/templates/alsijil/group_role/partials/assignment.html
+-rw-r--r--   0        0        0     1127 2023-03-01 19:31:48.027203 aleksis_app_alsijil-3.0b0/aleksis/apps/alsijil/templates/alsijil/group_role/partials/assignment_options.html
+-rw-r--r--   0        0        0      395 2023-03-01 19:31:48.027203 aleksis_app_alsijil-3.0b0/aleksis/apps/alsijil/templates/alsijil/group_role/warning.html
+-rw-r--r--   0        0        0      194 2023-03-01 19:31:48.027203 aleksis_app_alsijil-3.0b0/aleksis/apps/alsijil/templates/alsijil/notifications/check.html
+-rw-r--r--   0        0        0      501 2023-03-01 19:31:48.027203 aleksis_app_alsijil-3.0b0/aleksis/apps/alsijil/templates/alsijil/partials/absences.html
+-rw-r--r--   0        0        0     2661 2023-03-01 19:31:48.027203 aleksis_app_alsijil-3.0b0/aleksis/apps/alsijil/templates/alsijil/partials/legend.html
+-rw-r--r--   0        0        0     5218 2023-03-01 19:31:48.027203 aleksis_app_alsijil-3.0b0/aleksis/apps/alsijil/templates/alsijil/partials/lesson/heading.html
+-rw-r--r--   0        0        0     1503 2023-03-01 19:31:48.027203 aleksis_app_alsijil-3.0b0/aleksis/apps/alsijil/templates/alsijil/partials/lesson/prev_next.html
+-rw-r--r--   0        0        0     1799 2023-03-01 19:31:48.027203 aleksis_app_alsijil-3.0b0/aleksis/apps/alsijil/templates/alsijil/partials/lesson/tabs/documentation.html
+-rw-r--r--   0        0        0      506 2023-03-01 19:31:48.027203 aleksis_app_alsijil-3.0b0/aleksis/apps/alsijil/templates/alsijil/partials/lesson/tabs/more.html
+-rw-r--r--   0        0        0     5656 2023-03-01 19:31:48.027203 aleksis_app_alsijil-3.0b0/aleksis/apps/alsijil/templates/alsijil/partials/lesson/tabs/notes.html
+-rw-r--r--   0        0        0     1885 2023-03-01 19:31:48.027203 aleksis_app_alsijil-3.0b0/aleksis/apps/alsijil/templates/alsijil/partials/lesson/tabs/previous_lesson.html
+-rw-r--r--   0        0        0     4146 2023-03-01 19:31:48.027203 aleksis_app_alsijil-3.0b0/aleksis/apps/alsijil/templates/alsijil/partials/lesson/tabs/seating_plan.html
+-rw-r--r--   0        0        0     2084 2023-03-01 19:31:48.027203 aleksis_app_alsijil-3.0b0/aleksis/apps/alsijil/templates/alsijil/partials/lesson_status.html
+-rw-r--r--   0        0        0      441 2023-03-01 19:31:48.027203 aleksis_app_alsijil-3.0b0/aleksis/apps/alsijil/templates/alsijil/partials/lesson_status_icon.html
+-rw-r--r--   0        0        0     1398 2023-03-01 19:31:48.027203 aleksis_app_alsijil-3.0b0/aleksis/apps/alsijil/templates/alsijil/partials/objects_table.html
+-rw-r--r--   0        0        0     5041 2023-03-01 19:31:48.027203 aleksis_app_alsijil-3.0b0/aleksis/apps/alsijil/templates/alsijil/partials/persons_with_stats.html
+-rw-r--r--   0        0        0      282 2023-03-01 19:31:48.027203 aleksis_app_alsijil-3.0b0/aleksis/apps/alsijil/templates/alsijil/partials/tardinesses.html
+-rw-r--r--   0        0        0    17749 2023-03-01 19:31:48.027203 aleksis_app_alsijil-3.0b0/aleksis/apps/alsijil/templates/alsijil/print/full_register.html
+-rw-r--r--   0        0        0        0 2023-03-01 19:31:48.027203 aleksis_app_alsijil-3.0b0/aleksis/apps/alsijil/templatetags/__init__.py
+-rw-r--r--   0        0        0      353 2023-03-01 19:31:48.027203 aleksis_app_alsijil-3.0b0/aleksis/apps/alsijil/templatetags/time_helpers.py
+-rw-r--r--   0        0        0     3603 2023-03-01 19:31:48.027203 aleksis_app_alsijil-3.0b0/aleksis/apps/alsijil/tests/test_actions.py
+-rw-r--r--   0        0        0     4446 2023-03-01 19:31:48.027203 aleksis_app_alsijil-3.0b0/aleksis/apps/alsijil/urls.py
+-rw-r--r--   0        0        0    15259 2023-03-01 19:33:57.970943 aleksis_app_alsijil-3.0b0/aleksis/apps/alsijil/util/__pycache__/predicates.cpython-311.pyc
+-rw-r--r--   0        0        0    16315 2023-03-01 19:31:48.027203 aleksis_app_alsijil-3.0b0/aleksis/apps/alsijil/util/alsijil_helpers.py
+-rw-r--r--   0        0        0     9889 2023-03-01 19:31:48.031203 aleksis_app_alsijil-3.0b0/aleksis/apps/alsijil/util/predicates.py
+-rw-r--r--   0        0        0    53666 2023-03-01 19:31:48.031203 aleksis_app_alsijil-3.0b0/aleksis/apps/alsijil/views.py
+-rw-r--r--   0        0        0      581 2023-03-01 19:31:48.031203 aleksis_app_alsijil-3.0b0/docs/Makefile
+-rw-r--r--   0        0        0    81006 2023-03-01 19:31:48.031203 aleksis_app_alsijil-3.0b0/docs/_static/assign_group_role.png
+-rw-r--r--   0        0        0    78757 2023-03-01 19:31:48.031203 aleksis_app_alsijil-3.0b0/docs/_static/create_excuse_type.png
+-rw-r--r--   0        0        0    63748 2023-03-01 19:31:48.035203 aleksis_app_alsijil-3.0b0/docs/_static/create_extra_mark.png
+-rw-r--r--   0        0        0    62703 2023-03-01 19:31:48.035203 aleksis_app_alsijil-3.0b0/docs/_static/edit_group_role.png
+-rw-r--r--   0        0        0    84526 2023-03-01 19:31:48.035203 aleksis_app_alsijil-3.0b0/docs/_static/excuse_types.png
+-rw-r--r--   0        0        0    79794 2023-03-01 19:31:48.035203 aleksis_app_alsijil-3.0b0/docs/_static/extra_marks.png
+-rw-r--r--   0        0        0    69601 2023-03-01 19:31:48.035203 aleksis_app_alsijil-3.0b0/docs/_static/group_roles.png
+-rw-r--r--   0        0        0    86554 2023-03-01 19:31:48.039203 aleksis_app_alsijil-3.0b0/docs/_static/lesson_documentation.png
+-rw-r--r--   0        0        0    90453 2023-03-01 19:31:48.039203 aleksis_app_alsijil-3.0b0/docs/_static/lesson_personal_notes.png
+-rw-r--r--   0        0        0    77148 2023-03-01 19:31:48.039203 aleksis_app_alsijil-3.0b0/docs/_static/lesson_version_history.png
+-rw-r--r--   0        0        0   156092 2023-03-01 19:31:48.043203 aleksis_app_alsijil-3.0b0/docs/_static/my_groups.png
+-rw-r--r--   0        0        0   151265 2023-03-01 19:31:48.043203 aleksis_app_alsijil-3.0b0/docs/_static/my_students.png
+-rw-r--r--   0        0        0   109932 2023-03-01 19:31:48.043203 aleksis_app_alsijil-3.0b0/docs/_static/overview_lessons.png
+-rw-r--r--   0        0        0    93584 2023-03-01 19:31:48.047203 aleksis_app_alsijil-3.0b0/docs/_static/overview_person.png
+-rw-r--r--   0        0        0    72488 2023-03-01 19:31:48.047203 aleksis_app_alsijil-3.0b0/docs/_static/register_absence.png
+-rw-r--r--   0        0        0    92604 2023-03-01 19:31:48.047203 aleksis_app_alsijil-3.0b0/docs/_static/register_absence_confirm.png
+-rw-r--r--   0        0        0   139320 2023-03-01 19:31:48.051203 aleksis_app_alsijil-3.0b0/docs/_static/students_list.png
+-rw-r--r--   0        0        0   106128 2023-03-01 19:31:48.051203 aleksis_app_alsijil-3.0b0/docs/_static/week_view.png
+-rw-r--r--   0        0        0   107577 2023-03-01 19:31:48.051203 aleksis_app_alsijil-3.0b0/docs/_static/week_view_personal_notes.png
+-rw-r--r--   0        0        0      152 2023-03-01 19:31:48.051203 aleksis_app_alsijil-3.0b0/docs/admin/00_index.rst
+-rw-r--r--   0        0        0     1513 2023-03-01 19:31:48.051203 aleksis_app_alsijil-3.0b0/docs/admin/30_configure.rst
+-rw-r--r--   0        0        0     2345 2023-03-01 19:31:48.051203 aleksis_app_alsijil-3.0b0/docs/admin/40_preferences.rst
+-rw-r--r--   0        0        0     6404 2023-03-01 19:31:48.051203 aleksis_app_alsijil-3.0b0/docs/conf.py
+-rw-r--r--   0        0        0      528 2023-03-01 19:31:48.051203 aleksis_app_alsijil-3.0b0/docs/index.rst
+-rw-r--r--   0        0        0      787 2023-03-01 19:31:48.051203 aleksis_app_alsijil-3.0b0/docs/make.bat
+-rw-r--r--   0        0        0       76 2023-03-01 19:31:48.051203 aleksis_app_alsijil-3.0b0/docs/user/00_index.rst
+-rw-r--r--   0        0        0     2330 2023-03-01 19:31:48.051203 aleksis_app_alsijil-3.0b0/docs/user/10_basic.rst
+-rw-r--r--   0        0        0     1437 2023-03-01 19:31:48.051203 aleksis_app_alsijil-3.0b0/docs/user/15_concepts.rst
+-rw-r--r--   0        0        0     2939 2023-03-01 19:31:48.055203 aleksis_app_alsijil-3.0b0/docs/user/20_overview.rst
+-rw-r--r--   0        0        0     2833 2023-03-01 19:31:48.055203 aleksis_app_alsijil-3.0b0/docs/user/21_lesson.rst
+-rw-r--r--   0        0        0      308 2023-03-01 19:31:48.055203 aleksis_app_alsijil-3.0b0/docs/user/25_group_roles.rst
+-rw-r--r--   0        0        0      591 2023-03-01 19:31:48.055203 aleksis_app_alsijil-3.0b0/docs/user/40_export.rst
+-rw-r--r--   0        0        0     2049 2023-03-01 19:32:15.363149 aleksis_app_alsijil-3.0b0/pyproject.toml
+-rw-r--r--   0        0        0     2730 2023-03-01 19:31:48.055203 aleksis_app_alsijil-3.0b0/tox.ini
+-rw-r--r--   0        0        0     4671 1970-01-01 00:00:00.000000 aleksis_app_alsijil-3.0b0/setup.py
+-rw-r--r--   0        0        0     3407 1970-01-01 00:00:00.000000 aleksis_app_alsijil-3.0b0/PKG-INFO
```

### Comparing `AlekSIS-App-Alsijil-3.0.dev0/CHANGELOG.rst` & `aleksis_app_alsijil-3.0b0/CHANGELOG.rst`

 * *Files 10% similar despite different names*

```diff
@@ -2,16 +2,56 @@
 =========
 
 All notable changes to this project will be documented in this file.
 
 The format is based on `Keep a Changelog`_,
 and this project adheres to `Semantic Versioning`_.
 
-Unreleased
-----------
+`3.0b0`_ - 2022-02-28
+---------------------
+
+This version requires AlekSIS-Core 3.0. It is incompatible with any previous
+version.
+
+Removed
+~~~~~~~
+
+* Legacy menu integration for AlekSIS-Core pre-3.0
+
+Added
+~~~~~
+
+* Add SPA support for AlekSIS-Core 3.0
+
+Changed
+~~~~~~~
+
+* [Dev] Rename the "late" field in the PersonalNote model to "tardiness".
+* Use new icon set inside of models and templates
+* Run full register printout generation in background 
+
+Fixed
+~~~~~
+
+* Extra marks and excused absences were counted multiple times in some class register views.
+* Substitution teachers couldn't see any persons in the person list of a substituted lesson.
+* Events were shown for days not being inside the timetable schema in full register printout.
+
+`2.1.1`_ - 2022-09-01
+---------------------
+
+Fixed
+~~~~~
+
+* Register absence form wasn't accessible without direct access to class register.
+* Printing the full group register failed when a person had no personal notes.
+* Data checks reported all Lesson Documentations as being during Holidays if there was no Holiday object.
+* Students were displayed multiple times in class register views.
+* Absences were counted multiple times in some class register views.
+* Group owners couldn't create new seating plans.
 
 `2.1`_ - 2022-06-25
 -------------------
 
 Added
 ~~~~~
 
@@ -257,7 +297,9 @@
 .. _2.0rc4: https://edugit.org/AlekSIS/Official/AlekSIS-App-Alsijil/-/tags/2.0rc4
 .. _2.0rc5: https://edugit.org/AlekSIS/Official/AlekSIS-App-Alsijil/-/tags/2.0rc5
 .. _2.0rc6: https://edugit.org/AlekSIS/Official/AlekSIS-App-Alsijil/-/tags/2.0rc6
 .. _2.0rc7: https://edugit.org/AlekSIS/Official/AlekSIS-App-Alsijil/-/tags/2.0rc7
 .. _2.0: https://edugit.org/AlekSIS/Official/AlekSIS-App-Alsijil/-/tags/2.0
 .. _2.0.1: https://edugit.org/AlekSIS/Official/AlekSIS-App-Alsijil/-/tags/2.0.1
 .. _2.1: https://edugit.org/AlekSIS/Official/AlekSIS-App-Alsijil/-/tags/2.1
+.. _2.1.1: https://edugit.org/AlekSIS/Official/AlekSIS-App-Alsijil/-/tags/2.1.1
+.. _3.0b0: https://edugit.org/AlekSIS/Official/AlekSIS-App-Alsijil/-/tags/3.0b0
```

### Comparing `AlekSIS-App-Alsijil-3.0.dev0/LICENCE.rst` & `aleksis_app_alsijil-3.0b0/LICENCE.rst`

 * *Files identical despite different names*

### Comparing `AlekSIS-App-Alsijil-3.0.dev0/README.rst` & `aleksis_app_alsijil-3.0b0/README.rst`

 * *Files 3% similar despite different names*

```diff
@@ -34,15 +34,14 @@
   Copyright © 2019, 2021 Dominik George <dominik.george@teckids.org>
   Copyright © 2019, 2020 Tom Teichler <tom.teichler@teckids.org>
   Copyright © 2019 mirabilos <thorsten.glaser@teckids.org>
   Copyright © 2020, 2021, 2022 Jonathan Weth <dev@jonathanweth.de>
   Copyright © 2020, 2021 Julian Leucker <leuckeju@katharineum.de>
   Copyright © 2020, 2022 Hangzhi Yu <yuha@katharineum.de>
   Copyright © 2021 Lloyd Meins <meinsll@katharineum.de>
-  Copyright © 2022 magicfelix <felix@felix-zauberer.de>
 
 
   Licenced under the EUPL, version 1.2 or later, by Teckids e.V. (Bonn, Germany).
 
 Please see the LICENCE.rst file accompanying this distribution for the
 full licence text or on the `European Union Public Licence`_ website
 https://joinup.ec.europa.eu/collection/eupl/guidelines-users-and-developers
```

### Comparing `AlekSIS-App-Alsijil-3.0.dev0/aleksis/apps/alsijil/__pycache__/apps.cpython-310.pyc` & `aleksis_app_alsijil-3.0b0/aleksis/apps/alsijil/__pycache__/apps.cpython-311.pyc`

 * *Format-specific differences are supported for Python .pyc files but no file-specific differences were detected; falling back to a binary diff. file(1) reports: Byte-compiled Python module for CPython 3.10, timestamp-based, .py timestamp: Thu Aug 18 20:28:10 2022 UTC, .py size: 848 bytes*

 * *Could not decompile bytecode: bad marshal data (unknown type code)*

 * *Files 24% similar despite different names*

```diff
@@ -1,67 +1,78 @@
-00000000: 6f0d 0d0a 0000 0000 daa0 fe62 5003 0000  o..........bP...
-00000010: e300 0000 0000 0000 0000 0000 0000 0000  ................
-00000020: 0004 0000 0040 0000 0073 2000 0000 6400  .....@...s ...d.
-00000030: 6401 6c00 6d01 5a01 0100 4700 6402 6403  d.l.m.Z...G.d.d.
-00000040: 8400 6403 6501 8303 5a02 6404 5300 2905  ..d.e...Z.d.S.).
-00000050: e900 0000 0029 01da 0941 7070 436f 6e66  .....)...AppConf
-00000060: 6967 6300 0000 0000 0000 0000 0000 0000  igc.............
-00000070: 0000 000a 0000 0040 0000 0073 7e00 0000  .......@...s~...
-00000080: 6500 5a01 6400 5a02 6401 5a03 6402 5a04  e.Z.d.Z.d.Z.d.Z.
-00000090: 6403 6404 6901 5a05 6405 5a06 6406 6407  d.d.i.Z.d.Z.d.d.
-000000a0: 6702 6408 6409 6603 6406 640a 6702 640b  g.d.d.f.d.d.g.d.
-000000b0: 640c 6603 6406 6701 640d 640e 6603 6700  d.f.d.g.d.d.f.g.
-000000c0: 640f a201 6410 6411 6603 640a 6407 6702  d...d.d.f.d.d.g.
-000000d0: 6412 6413 6603 640a 6414 6702 6415 6416  d.d.f.d.d.g.d.d.
-000000e0: 6603 6407 6701 6417 6418 6603 6414 6701  f.d.g.d.d.f.d.g.
-000000f0: 6419 641a 6603 6608 5a07 641b 5300 291c  d.d.f.f.Z.d.S.).
-00000100: da0d 416c 7369 6a69 6c43 6f6e 6669 677a  ..AlsijilConfigz
-00000110: 1461 6c65 6b73 6973 2e61 7070 732e 616c  .aleksis.apps.al
-00000120: 7369 6a69 6c75 2400 0000 416c 656b 5349  sijilu$...AlekSI
-00000130: 5320 e280 9420 416c 7369 6a69 6c20 2843  S ... Alsijil (C
-00000140: 6c61 7373 2072 6567 6973 7465 7229 da0a  lass register)..
-00000150: 5265 706f 7369 746f 7279 7a38 6874 7470  Repositoryz8http
-00000160: 733a 2f2f 6564 7567 6974 2e6f 7267 2f41  s://edugit.org/A
-00000170: 6c65 6b53 4953 2f6f 6666 6963 6961 6c2f  lekSIS/official/
-00000180: 416c 656b 5349 532d 4170 702d 416c 7369  AlekSIS-App-Alsi
-00000190: 6a69 6c2f 7a09 4555 504c 2d31 2e32 2b69  jil/z.EUPL-1.2+i
-000001a0: e307 0000 e9e5 0700 007a 0e44 6f6d 696e  .........z.Domin
-000001b0: 696b 2047 656f 7267 657a 1a64 6f6d 696e  ik Georgez.domin
-000001c0: 696b 2e67 656f 7267 6540 7465 636b 6964  ik.george@teckid
-000001d0: 732e 6f72 67e9 e407 0000 7a0c 546f 6d20  s.org.....z.Tom 
-000001e0: 5465 6963 686c 6572 7a18 746f 6d2e 7465  Teichlerz.tom.te
-000001f0: 6963 686c 6572 4074 6563 6b69 6473 2e6f  ichler@teckids.o
-00000200: 7267 da09 6d69 7261 6269 6c6f 737a 1b74  rg..mirabilosz.t
-00000210: 686f 7273 7465 6e2e 676c 6173 6572 4074  horsten.glaser@t
-00000220: 6563 6b69 6473 2e6f 7267 2903 7206 0000  eckids.org).r...
-00000230: 0072 0500 0000 e9e6 0700 007a 0d4a 6f6e  .r.........z.Jon
-00000240: 6174 6861 6e20 5765 7468 7a13 6465 7640  athan Wethz.dev@
-00000250: 6a6f 6e61 7468 616e 7765 7468 2e64 657a  jonathanweth.dez
-00000260: 0e4a 756c 6961 6e20 4c65 7563 6b65 727a  .Julian Leuckerz
-00000270: 176c 6575 636b 656a 7540 6b61 7468 6172  .leuckeju@kathar
-00000280: 696e 6575 6d2e 6465 7208 0000 007a 0a48  ineum.der....z.H
-00000290: 616e 677a 6869 2059 757a 1379 7568 6140  angzhi Yuz.yuha@
-000002a0: 6b61 7468 6172 696e 6575 6d2e 6465 7a0b  katharineum.dez.
-000002b0: 4c6c 6f79 6420 4d65 696e 737a 166d 6569  Lloyd Meinsz.mei
-000002c0: 6e73 6c6c 406b 6174 6861 7269 6e65 756d  nsll@katharineum
-000002d0: 2e64 65da 0a6d 6167 6963 6665 6c69 787a  .de..magicfelixz
-000002e0: 1766 656c 6978 4066 656c 6978 2d7a 6175  .felix@felix-zau
-000002f0: 6265 7265 722e 6465 4e29 08da 085f 5f6e  berer.deN)...__n
-00000300: 616d 655f 5fda 0a5f 5f6d 6f64 756c 655f  ame__..__module_
-00000310: 5fda 0c5f 5f71 7561 6c6e 616d 655f 5fda  _..__qualname__.
-00000320: 046e 616d 65da 0c76 6572 626f 7365 5f6e  .name..verbose_n
-00000330: 616d 65da 0475 726c 73da 076c 6963 656e  ame..urls..licen
-00000340: 6365 da0e 636f 7079 7269 6768 745f 696e  ce..copyright_in
-00000350: 666f a900 7212 0000 0072 1200 0000 fa49  fo..r....r.....I
-00000360: 2f62 7569 6c64 732f 416c 656b 5349 532f  /builds/AlekSIS/
-00000370: 6f66 6669 6369 616c 2f41 6c65 6b53 4953  official/AlekSIS
-00000380: 2d41 7070 2d41 6c73 696a 696c 2f61 6c65  -App-Alsijil/ale
-00000390: 6b73 6973 2f61 7070 732f 616c 7369 6a69  ksis/apps/alsiji
-000003a0: 6c2f 6170 7073 2e70 7972 0300 0000 0400  l/apps.pyr......
-000003b0: 0000 731e 0000 0008 0004 0104 0104 0304  ..s.............
-000003c0: ff04 030c 020c 010a 010c 010c 010c 010a  ................
-000003d0: 010a 0108 f872 0300 0000 4e29 03da 1661  .....r....N)...a
-000003e0: 6c65 6b73 6973 2e63 6f72 652e 7574 696c  leksis.core.util
-000003f0: 2e61 7070 7372 0200 0000 7203 0000 0072  .appsr....r....r
-00000400: 1200 0000 7212 0000 0072 1200 0000 7213  ....r....r....r.
-00000410: 0000 00da 083c 6d6f 6475 6c65 3e01 0000  .....<module>...
-00000420: 0073 0400 0000 0c00 1403                 .s........
+00000000: a70d 0d0a 0000 0000 24a8 ff63 1503 0000  ........$..c....
+00000010: e300 0000 0000 0000 0000 0000 0005 0000  ................
+00000020: 0000 0000 00f3 2e00 0000 9700 6400 6401  ............d.d.
+00000030: 6c00 6d01 5a01 0100 0200 4700 6402 8400  l.m.Z.....G.d...
+00000040: 6403 6501 a603 0000 ab03 0000 0000 0000  d.e.............
+00000050: 0000 5a02 6404 5300 2905 e900 0000 0029  ..Z.d.S.)......)
+00000060: 01da 0941 7070 436f 6e66 6967 6300 0000  ...AppConfigc...
+00000070: 0000 0000 0000 0000 0009 0000 0000 0000  ................
+00000080: 00f3 7600 0000 9700 6500 5a01 6400 5a02  ..v.....e.Z.d.Z.
+00000090: 6401 5a03 6402 5a04 6403 6404 6901 5a05  d.Z.d.Z.d.d.i.Z.
+000000a0: 6405 5a06 6406 6407 6702 6408 6409 6603  d.Z.d.d.g.d.d.f.
+000000b0: 6406 640a 6702 640b 640c 6603 6406 6701  d.d.g.d.d.f.d.g.
+000000c0: 640d 640e 6603 6700 640f a201 6410 6411  d.d.f.g.d...d.d.
+000000d0: 6603 640a 6407 6702 6412 6413 6603 640a  f.d.d.g.d.d.f.d.
+000000e0: 6414 6702 6415 6416 6603 6407 6701 6417  d.g.d.d.f.d.g.d.
+000000f0: 6418 6603 6607 5a07 6419 5300 291a da0d  d.f.f.Z.d.S.)...
+00000100: 416c 7369 6a69 6c43 6f6e 6669 677a 1461  AlsijilConfigz.a
+00000110: 6c65 6b73 6973 2e61 7070 732e 616c 7369  leksis.apps.alsi
+00000120: 6a69 6c75 2400 0000 416c 656b 5349 5320  jilu$...AlekSIS 
+00000130: e280 9420 416c 7369 6a69 6c20 2843 6c61  ... Alsijil (Cla
+00000140: 7373 2072 6567 6973 7465 7229 da0a 5265  ss register)..Re
+00000150: 706f 7369 746f 7279 7a38 6874 7470 733a  positoryz8https:
+00000160: 2f2f 6564 7567 6974 2e6f 7267 2f41 6c65  //edugit.org/Ale
+00000170: 6b53 4953 2f6f 6666 6963 6961 6c2f 416c  kSIS/official/Al
+00000180: 656b 5349 532d 4170 702d 416c 7369 6a69  ekSIS-App-Alsiji
+00000190: 6c2f 7a09 4555 504c 2d31 2e32 2b69 e307  l/z.EUPL-1.2+i..
+000001a0: 0000 e9e5 0700 007a 0e44 6f6d 696e 696b  .......z.Dominik
+000001b0: 2047 656f 7267 657a 1a64 6f6d 696e 696b   Georgez.dominik
+000001c0: 2e67 656f 7267 6540 7465 636b 6964 732e  .george@teckids.
+000001d0: 6f72 67e9 e407 0000 7a0c 546f 6d20 5465  org.....z.Tom Te
+000001e0: 6963 686c 6572 7a18 746f 6d2e 7465 6963  ichlerz.tom.teic
+000001f0: 686c 6572 4074 6563 6b69 6473 2e6f 7267  hler@teckids.org
+00000200: da09 6d69 7261 6269 6c6f 737a 1b74 686f  ..mirabilosz.tho
+00000210: 7273 7465 6e2e 676c 6173 6572 4074 6563  rsten.glaser@tec
+00000220: 6b69 6473 2e6f 7267 2903 7208 0000 0072  kids.org).r....r
+00000230: 0700 0000 e9e6 0700 007a 0d4a 6f6e 6174  .........z.Jonat
+00000240: 6861 6e20 5765 7468 7a13 6465 7640 6a6f  han Wethz.dev@jo
+00000250: 6e61 7468 616e 7765 7468 2e64 657a 0e4a  nathanweth.dez.J
+00000260: 756c 6961 6e20 4c65 7563 6b65 727a 176c  ulian Leuckerz.l
+00000270: 6575 636b 656a 7540 6b61 7468 6172 696e  euckeju@katharin
+00000280: 6575 6d2e 6465 720a 0000 007a 0a48 616e  eum.der....z.Han
+00000290: 677a 6869 2059 757a 1379 7568 6140 6b61  gzhi Yuz.yuha@ka
+000002a0: 7468 6172 696e 6575 6d2e 6465 7a0b 4c6c  tharineum.dez.Ll
+000002b0: 6f79 6420 4d65 696e 737a 166d 6569 6e73  oyd Meinsz.meins
+000002c0: 6c6c 406b 6174 6861 7269 6e65 756d 2e64  ll@katharineum.d
+000002d0: 654e 2908 da08 5f5f 6e61 6d65 5f5f da0a  eN)...__name__..
+000002e0: 5f5f 6d6f 6475 6c65 5f5f da0c 5f5f 7175  __module__..__qu
+000002f0: 616c 6e61 6d65 5f5f da04 6e61 6d65 da0c  alname__..name..
+00000300: 7665 7262 6f73 655f 6e61 6d65 da04 7572  verbose_name..ur
+00000310: 6c73 da07 6c69 6365 6e63 65da 0e63 6f70  ls..licence..cop
+00000320: 7972 6967 6874 5f69 6e66 6fa9 00f3 0000  yright_info.....
+00000330: 0000 fa49 2f62 7569 6c64 732f 416c 656b  ...I/builds/Alek
+00000340: 5349 532f 6f66 6669 6369 616c 2f41 6c65  SIS/official/Ale
+00000350: 6b53 4953 2d41 7070 2d41 6c73 696a 696c  kSIS-App-Alsijil
+00000360: 2f61 6c65 6b73 6973 2f61 7070 732f 616c  /aleksis/apps/al
+00000370: 7369 6a69 6c2f 6170 7073 2e70 7972 0500  sijil/apps.pyr..
+00000380: 0000 7205 0000 0004 0000 0073 9e00 0000  ..r........s....
+00000390: 8000 8000 8000 8000 8000 d80b 2180 44d8  ............!.D.
+000003a0: 1339 804c f006 0009 15d0 1650 f003 020c  .9.L.......P....
+000003b0: 0680 44f0 0600 0f1a 8047 e00a 0e90 0488  ..D......G......
+000003c0: 1cd0 1727 d029 45d0 0846 d80a 0e90 0488  ...'.)E..F......
+000003d0: 1c90 7ed0 2741 d008 42d8 0a0e 8816 901b  ..~.'A..B.......
+000003e0: d01e 3bd0 083c d809 1bd0 091b d009 1b98  ..;..<..........
+000003f0: 5fd0 2e43 d008 44d8 0a0e 9004 881c d017  _..C..D.........
+00000400: 27d0 2942 d008 43d8 0a0e 9004 881c 907c  '.)B..C........|
+00000410: d025 3ad0 083b d80a 0e88 1690 1dd0 2038  .%:..;........ 8
+00000420: d008 39f0 0f08 1606 804e 804e 804e 7214  ..9......N.N.Nr.
+00000430: 0000 0072 0500 0000 4e29 03da 1661 6c65  ...r....N)...ale
+00000440: 6b73 6973 2e63 6f72 652e 7574 696c 2e61  ksis.core.util.a
+00000450: 7070 7372 0300 0000 7205 0000 0072 1300  ppsr....r....r..
+00000460: 0000 7214 0000 0072 1500 0000 fa08 3c6d  ..r....r......<m
+00000470: 6f64 756c 653e 7217 0000 0001 0000 0073  odule>r........s
+00000480: 4b00 0000 f003 0101 01d8 002c d000 2cd0  K..........,..,.
+00000490: 002c d000 2cd0 002c d000 2cf0 0610 0106  .,..,..,..,.....
+000004a0: f000 1001 06f0 0010 0106 f000 1001 06f0  ................
+000004b0: 0010 0106 9049 f100 1001 06f4 0010 0106  .....I..........
+000004c0: f000 1001 06f0 0010 0106 f000 1001 0672  ...............r
+000004d0: 1400 0000                                ....
```

### Comparing `AlekSIS-App-Alsijil-3.0.dev0/aleksis/apps/alsijil/actions.py` & `aleksis_app_alsijil-3.0b0/aleksis/apps/alsijil/actions.py`

 * *Files 1% similar despite different names*

```diff
@@ -37,15 +37,15 @@
 
 def delete_personal_note(modeladmin, request, queryset):
     notes = []
     for personal_note in queryset:
         personal_note.reset_values()
         notes.append(personal_note)
     PersonalNote.objects.bulk_update(
-        notes, fields=["absent", "excused", "late", "excuse_type", "remarks"]
+        notes, fields=["absent", "excused", "tardiness", "excuse_type", "remarks"]
     )
 
 
 delete_personal_note.short_description = _("Delete")
 
 
 def send_request_to_check_entry(modeladmin, request: HttpRequest, selected_items: Sequence[dict]):
```

### Comparing `AlekSIS-App-Alsijil-3.0.dev0/aleksis/apps/alsijil/apps.py` & `aleksis_app_alsijil-3.0b0/aleksis/apps/alsijil/apps.py`

 * *Files 6% similar despite different names*

```diff
@@ -13,9 +13,8 @@
         ([2019, 2021], "Dominik George", "dominik.george@teckids.org"),
         ([2019, 2020], "Tom Teichler", "tom.teichler@teckids.org"),
         ([2019], "mirabilos", "thorsten.glaser@teckids.org"),
         ([2020, 2021, 2022], "Jonathan Weth", "dev@jonathanweth.de"),
         ([2020, 2021], "Julian Leucker", "leuckeju@katharineum.de"),
         ([2020, 2022], "Hangzhi Yu", "yuha@katharineum.de"),
         ([2021], "Lloyd Meins", "meinsll@katharineum.de"),
-        ([2022], "magicfelix", "felix@felix-zauberer.de"),
     )
```

### Comparing `AlekSIS-App-Alsijil-3.0.dev0/aleksis/apps/alsijil/data_checks.py` & `aleksis_app_alsijil-3.0b0/aleksis/apps/alsijil/data_checks.py`

 * *Files 0% similar despite different names*

```diff
@@ -109,15 +109,15 @@
 
         from .models import LessonDocumentation
 
         holidays = Holiday.objects.all()
 
         documentations = LessonDocumentation.objects.not_empty().annotate_date_range()
 
-        q = Q()
+        q = Q(pk__in=[])
         for holiday in holidays:
             q = q | Q(day_end__gte=holiday.date_start, day_start__lte=holiday.date_end)
         documentations = documentations.filter(q)
 
         for doc in documentations:
             logging.info(f"Lesson documentation {doc} is on holidays")
             cls.register_result(doc)
@@ -143,15 +143,15 @@
 
         from .models import PersonalNote
 
         holidays = Holiday.objects.all()
 
         personal_notes = PersonalNote.objects.not_empty().annotate_date_range()
 
-        q = Q()
+        q = Q(pk__in=[])
         for holiday in holidays:
             q = q | Q(day_end__gte=holiday.date_start, day_start__lte=holiday.date_end)
         personal_notes = personal_notes.filter(q)
 
         for note in personal_notes:
             logging.info(f"Personal note {note} is on holidays")
             cls.register_result(note)
```

### Comparing `AlekSIS-App-Alsijil-3.0.dev0/aleksis/apps/alsijil/forms.py` & `aleksis_app_alsijil-3.0b0/aleksis/apps/alsijil/forms.py`

 * *Files 2% similar despite different names*

```diff
@@ -43,43 +43,43 @@
 
     def __init__(self, *args, **kwargs):
         super().__init__(*args, **kwargs)
 
         self.fields["homework"].label = _("Homework for the next lesson")
         if (
             self.instance.lesson_period
-            and get_site_preferences()["alsijil__save_lesson_documentations_by_week"]
+            and get_site_preferences()["alsijil__allow_carry_over_same_week"]
         ):
             self.fields["carry_over_week"] = forms.BooleanField(
                 label=_("Carry over data to all other lessons with the same subject in this week"),
                 initial=True,
                 required=False,
             )
 
     def save(self, **kwargs):
         lesson_documentation = super(LessonDocumentationForm, self).save(commit=True)
         if (
-            get_site_preferences()["alsijil__save_lesson_documentations_by_week"]
+            get_site_preferences()["alsijil__allow_carry_over_same_week"]
             and self.cleaned_data["carry_over_week"]
             and (
                 lesson_documentation.topic
                 or lesson_documentation.homework
                 or lesson_documentation.group_note
             )
             and lesson_documentation.lesson_period
         ):
             lesson_documentation.carry_over_data(
-                LessonPeriod.objects.filter(lesson=lesson_documentation.lesson_period.lesson), True
+                LessonPeriod.objects.filter(lesson=lesson_documentation.lesson_period.lesson)
             )
 
 
 class PersonalNoteForm(forms.ModelForm):
     class Meta:
         model = PersonalNote
-        fields = ["absent", "late", "excused", "excuse_type", "extra_marks", "remarks"]
+        fields = ["absent", "tardiness", "excused", "excuse_type", "extra_marks", "remarks"]
 
     person_name = forms.CharField(disabled=True)
 
     def __init__(self, *args, **kwargs):
         super().__init__(*args, **kwargs)
         self.fields["person_name"].widget.attrs.update(
             {"class": "alsijil-lesson-personal-note-name"}
@@ -182,35 +182,57 @@
 PersonalNoteFormSet = forms.modelformset_factory(
     PersonalNote, form=PersonalNoteForm, max_num=0, extra=0
 )
 
 
 class RegisterAbsenceForm(forms.Form):
     layout = Layout(
+        Fieldset("", "person"),
         Fieldset("", Row("date_start", "date_end"), Row("from_period", "to_period")),
         Fieldset("", Row("absent", "excused"), Row("excuse_type"), Row("remarks")),
     )
+    person = forms.ModelChoiceField(label=_("Person"), queryset=None, widget=Select2Widget)
     date_start = forms.DateField(label=_("Start date"), initial=datetime.today)
     date_end = forms.DateField(label=_("End date"), initial=datetime.today)
     from_period = forms.ChoiceField(label=_("Start period"))
     to_period = forms.ChoiceField(label=_("End period"))
     absent = forms.BooleanField(label=_("Absent"), initial=True, required=False)
     excused = forms.BooleanField(label=_("Excused"), initial=True, required=False)
     excuse_type = forms.ModelChoiceField(
         label=_("Excuse type"),
         queryset=ExcuseType.objects.all(),
         widget=Select2Widget,
         required=False,
     )
     remarks = forms.CharField(label=_("Remarks"), max_length=30, required=False)
 
-    def __init__(self, *args, **kwargs):
+    def __init__(self, request, *args, **kwargs):
+        self.request = request
         super().__init__(*args, **kwargs)
         period_choices = TimePeriod.period_choices
 
+        if self.request.user.has_perm("alsijil.register_absence"):
+            self.fields["person"].queryset = Person.objects.all()
+        else:
+            persons_qs = Person.objects.filter(
+                Q(
+                    pk__in=get_objects_for_user(
+                        self.request.user, "core.register_absence_person", Person
+                    )
+                )
+                | Q(primary_group__owners=self.request.user.person)
+                | Q(
+                    member_of__in=get_objects_for_user(
+                        self.request.user, "core.register_absence_group", Group
+                    )
+                )
+            ).distinct()
+
+            self.fields["person"].queryset = persons_qs
+
         self.fields["from_period"].choices = period_choices
         self.fields["to_period"].choices = period_choices
         self.fields["from_period"].initial = TimePeriod.period_min
         self.fields["to_period"].initial = TimePeriod.period_max
 
 
 class ExtraMarkForm(forms.ModelForm):
```

### Comparing `AlekSIS-App-Alsijil-3.0.dev0/aleksis/apps/alsijil/locale/ar/LC_MESSAGES/django.po` & `aleksis_app_alsijil-3.0b0/aleksis/apps/alsijil/locale/ar/LC_MESSAGES/django.po`

 * *Files identical despite different names*

### Comparing `AlekSIS-App-Alsijil-3.0.dev0/aleksis/apps/alsijil/locale/de_DE/LC_MESSAGES/django.mo` & `aleksis_app_alsijil-3.0b0/aleksis/apps/alsijil/locale/de_DE/LC_MESSAGES/django.mo`

 * *Files identical despite different names*

### Comparing `AlekSIS-App-Alsijil-3.0.dev0/aleksis/apps/alsijil/locale/de_DE/LC_MESSAGES/django.po` & `aleksis_app_alsijil-3.0b0/aleksis/apps/alsijil/locale/de_DE/LC_MESSAGES/django.po`

 * *Files identical despite different names*

### Comparing `AlekSIS-App-Alsijil-3.0.dev0/aleksis/apps/alsijil/locale/fr/LC_MESSAGES/django.mo` & `aleksis_app_alsijil-3.0b0/aleksis/apps/alsijil/locale/fr/LC_MESSAGES/django.mo`

 * *Files identical despite different names*

### Comparing `AlekSIS-App-Alsijil-3.0.dev0/aleksis/apps/alsijil/locale/fr/LC_MESSAGES/django.po` & `aleksis_app_alsijil-3.0b0/aleksis/apps/alsijil/locale/fr/LC_MESSAGES/django.po`

 * *Files identical despite different names*

### Comparing `AlekSIS-App-Alsijil-3.0.dev0/aleksis/apps/alsijil/locale/la/LC_MESSAGES/django.mo` & `aleksis_app_alsijil-3.0b0/aleksis/apps/alsijil/locale/la/LC_MESSAGES/django.mo`

 * *Files identical despite different names*

### Comparing `AlekSIS-App-Alsijil-3.0.dev0/aleksis/apps/alsijil/locale/la/LC_MESSAGES/django.po` & `aleksis_app_alsijil-3.0b0/aleksis/apps/alsijil/locale/la/LC_MESSAGES/django.po`

 * *Files identical despite different names*

### Comparing `AlekSIS-App-Alsijil-3.0.dev0/aleksis/apps/alsijil/locale/nb_NO/LC_MESSAGES/django.po` & `aleksis_app_alsijil-3.0b0/aleksis/apps/alsijil/locale/nb_NO/LC_MESSAGES/django.po`

 * *Files identical despite different names*

### Comparing `AlekSIS-App-Alsijil-3.0.dev0/aleksis/apps/alsijil/locale/ru/LC_MESSAGES/django.mo` & `aleksis_app_alsijil-3.0b0/aleksis/apps/alsijil/locale/ru/LC_MESSAGES/django.mo`

 * *Files 4% similar despite different names*

#### msgunfmt {}

```diff
@@ -1,12 +1,12 @@
 msgid ""
 msgstr ""
 "Project-Id-Version: PACKAGE VERSION\n"
 "Report-Msgid-Bugs-To: \n"
-"PO-Revision-Date: 2022-06-22 19:59+0000\n"
+"PO-Revision-Date: 2022-07-03 02:56+0000\n"
 "Last-Translator: Serhii Horichenko <m@sgg.im>\n"
 "Language-Team: Russian <https://translate.edugit.org/projects/aleksis/"
 "aleksis-app-alsijil/ru/>\n"
 "Language: ru\n"
 "MIME-Version: 1.0\n"
 "Content-Type: text/plain; charset=UTF-8\n"
 "Content-Transfer-Encoding: 8bit\n"
@@ -17,25 +17,25 @@
 
 msgid ""
 "\n"
 "                    Create a new seating plan for %(group)s in %(room)s\n"
 "                  "
 msgstr ""
 "\n"
-"                    Создать новый план размещения %(group)s в %(room)s\n"
+"                    Создать новый план рассадки %(group)s в %(room)s\n"
 "                  "
 
 msgid ""
 "\n"
 "                  Create a new seating plan for %(group)s (%(subject)s) in "
 "%(room)s\n"
 "                "
 msgstr ""
 "\n"
-"                  Создать новый план размещения %(group)s (%(subject)s) в "
+"                  Создать новый план рассадки %(group)s (%(subject)s) в "
 "%(room)s\n"
 "                "
 
 msgid ""
 "\n"
 "                  There are no affected lessons. Registering this absence "
 "won't have any effect.\n"
@@ -92,16 +92,15 @@
 "            This seating plan is taken from the parent group of "
 "%(child_group)s.\n"
 "            If you want, you can take it over for your group and then "
 "customize it.\n"
 "          "
 msgstr ""
 "\n"
-"            Этот план размещения взят из родительской группы "
-"%(child_group)s.\n"
+"            Этот план рассадки взят из родительской группы %(child_group)s.\n"
 "            При необходимости Вы можете настроить его под свою группу.\n"
 "          "
 
 msgid ""
 "\n"
 "        Copies of the class register, both digital and as printout, must\n"
 "        only be kept inside the school and/or on devices authorised by the\n"
@@ -244,14 +243,21 @@
 msgid "All assignments"
 msgstr "Все назначения"
 
 msgid "All lessons"
 msgstr "Все уроки"
 
 msgid ""
+"Allow carrying over data from any lesson period to all other "
+"lesson                 periods with the same lesson and in the same week"
+msgstr ""
+"Разрешить перенос данных с любого урока на все такие же "
+"уроки                 с таким же номером в расписании на той же неделе"
+
+msgid ""
 "Allow group owners to assign group roles to the parents of the group's "
 "members"
 msgstr ""
 "Разрешить владельцам групп назначать роли групп родителям участников групп"
 
 msgid ""
 "Allow original teachers to edit their lessons although they are substituted"
@@ -293,15 +299,15 @@
 msgid "Assign group role"
 msgstr "Назначить роль группы"
 
 msgid "Assign group role for %(group)s"
 msgstr "Назначить роль группы для %(group)s"
 
 msgid "Assigned person"
-msgstr "Назначенное лицо"
+msgstr "Назначенное физлицо"
 
 msgid "Available extra marks"
 msgstr "Доступные дополнительные отметки"
 
 msgid "Back"
 msgstr "Назад"
 
@@ -378,29 +384,32 @@
 msgid ""
 "Carry over data from first lesson period to the following lesson periods in "
 "lessons over multiple periods"
 msgstr ""
 "Переносить данные с первого урока в расписании на текущие уроки через "
 "несколько уроков"
 
+msgid "Carry over data to all other lessons with the same subject in this week"
+msgstr "Перенести данные на все другие уроки с тем же предметом на этой неделе"
+
 msgid ""
 "Carry over personal notes to all following lesson periods on the same day."
 msgstr "Переносить личные заметки на все последующие уроки того же дня."
 
 msgid "Change history"
 msgstr "Изменить историю"
 
 msgid "Class register"
 msgstr "Классный журнал"
 
 msgid "Class register:"
 msgstr "Классный журнал:"
 
 msgid "Class register: person"
-msgstr "Классный журнал: лицо"
+msgstr "Классный журнал: физлицо"
 
 msgid "Clear all filters"
 msgstr "Очистить фильтры"
 
 msgid "Close"
 msgstr "Закрыть"
 
@@ -479,15 +488,15 @@
 msgid "Edit group role"
 msgstr "Редактировать роль группы"
 
 msgid "Edit group role assignment"
 msgstr "Редактировать назначение роли группы"
 
 msgid "Edit seating plan"
-msgstr "Редактировать план размещения"
+msgstr "Редактировать план рассадки"
 
 msgid "End date"
 msgstr "Дата окончания"
 
 msgid "End period"
 msgstr "Окончание уроков"
 
@@ -550,14 +559,21 @@
 
 msgid "General"
 msgstr "Общее"
 
 msgid "Generate printout"
 msgstr "Подготовить к печати"
 
+msgid ""
+"Grant the owner of a parent group the same privileges as the owners of the "
+"respective child groups"
+msgstr ""
+"Наделить владельца родительской группы такими же правами, как у владельца "
+"соответствующих дочерних групп"
+
 msgid "Group"
 msgstr "Группа"
 
 msgid "Group note"
 msgstr "Групповая заметка"
 
 msgid "Group notes for previous lesson:"
@@ -733,15 +749,15 @@
 msgid "Per week"
 msgstr "На неделю"
 
 msgid "Period"
 msgstr "Урок"
 
 msgid "Person"
-msgstr "Лицо"
+msgstr "Физлицо"
 
 msgid "Personal note"
 msgstr "Личная заметка"
 
 msgid "Personal notes"
 msgstr "Личные заметки"
 
@@ -797,21 +813,21 @@
 msgid "Save"
 msgstr "Сохранить"
 
 msgid "School term"
 msgstr "Учебный год"
 
 msgid "Seating plan"
-msgstr "План размещения"
+msgstr "План рассадки"
 
 msgid ""
 "Seating plan for %(group)s in\n"
 "          %(room)s"
 msgstr ""
-"План размещения %(group)s в\n"
+"План рассадки %(group)s в\n"
 "          %(room)s"
 
 msgid "Select"
 msgstr "Отметить"
 
 msgid "Set current groups"
 msgstr "Установить текущие группы"
@@ -969,15 +985,22 @@
 msgid "The personal note is related to a cancelled lesson."
 msgstr "У отмененного урока есть связанные личные заметки."
 
 msgid "The personal notes have been saved."
 msgstr "Личные заметки сохранены."
 
 msgid "There is no seating plan for this lesson."
-msgstr "Для этого урока нет плана размещения."
+msgstr "Для этого урока нет плана рассадки."
+
+msgid ""
+"This will carry over data only if the data in the aforementioned periods are "
+"empty."
+msgstr ""
+"Это перенесёт данные только если в упомянутых выше уроках данные не "
+"заполнены."
 
 msgid ""
 "This will carry over data only if the data in the following periods are "
 "empty."
 msgstr ""
 "Это перенесёт данные только в случае отсутствия данных в последующих уроках."
```

### Comparing `AlekSIS-App-Alsijil-3.0.dev0/aleksis/apps/alsijil/locale/ru/LC_MESSAGES/django.po` & `aleksis_app_alsijil-3.0b0/aleksis/apps/alsijil/locale/ru/LC_MESSAGES/django.po`

 * *Files 1% similar despite different names*

```diff
@@ -4,22 +4,25 @@
 # FIRST AUTHOR <EMAIL@ADDRESS>, YEAR.
 #
 msgid ""
 msgstr ""
 "Project-Id-Version: PACKAGE VERSION\n"
 "Report-Msgid-Bugs-To: \n"
 "POT-Creation-Date: 2022-06-25 15:28+0200\n"
-"PO-Revision-Date: 2022-06-22 19:59+0000\n"
+"PO-Revision-Date: 2022-07-03 02:56+0000\n"
 "Last-Translator: Serhii Horichenko <m@sgg.im>\n"
-"Language-Team: Russian <https://translate.edugit.org/projects/aleksis/aleksis-app-alsijil/ru/>\n"
+"Language-Team: Russian <https://translate.edugit.org/projects/aleksis/"
+"aleksis-app-alsijil/ru/>\n"
 "Language: ru\n"
 "MIME-Version: 1.0\n"
 "Content-Type: text/plain; charset=UTF-8\n"
 "Content-Transfer-Encoding: 8bit\n"
-"Plural-Forms: nplurals=4; plural=(n%10==1 && n%100!=11 ? 0 : n%10>=2 && n%10<=4 && (n%100<12 || n%100>14) ? 1 : n%10==0 || (n%10>=5 && n%10<=9) || (n%100>=11 && n%100<=14)? 2 : 3);\n"
+"Plural-Forms: nplurals=4; plural=(n%10==1 && n%100!=11 ? 0 : n%10>=2 && n"
+"%10<=4 && (n%100<12 || n%100>14) ? 1 : n%10==0 || (n%10>=5 && n%10<=9) || (n"
+"%100>=11 && n%100<=14)? 2 : 3);\n"
 "X-Generator: Weblate 4.12.1\n"
 
 #: aleksis/apps/alsijil/actions.py:18
 msgid "Mark as excused"
 msgstr "Отметить как уважительный"
 
 #: aleksis/apps/alsijil/actions.py:25
@@ -129,15 +132,15 @@
 
 #: aleksis/apps/alsijil/forms.py:47
 msgid "Homework for the next lesson"
 msgstr "Домашняя работа на следующий урок"
 
 #: aleksis/apps/alsijil/forms.py:53
 msgid "Carry over data to all other lessons with the same subject in this week"
-msgstr ""
+msgstr "Перенести данные на все другие уроки с тем же предметом на этой неделе"
 
 #: aleksis/apps/alsijil/forms.py:98 aleksis/apps/alsijil/forms.py:256
 #: aleksis/apps/alsijil/forms.py:348
 #: aleksis/apps/alsijil/templates/alsijil/print/full_register.html:219
 msgid "Group"
 msgstr "Группа"
 
@@ -206,15 +209,15 @@
 msgstr "Замечания"
 
 #: aleksis/apps/alsijil/forms.py:269
 #: aleksis/apps/alsijil/templates/alsijil/absences/register.html:9
 #: aleksis/apps/alsijil/templates/alsijil/group_role/assigned_list.html:63
 #: aleksis/apps/alsijil/templates/alsijil/partials/lesson/tabs/notes.html:28
 msgid "Person"
-msgstr "Лицо"
+msgstr "Физлицо"
 
 #: aleksis/apps/alsijil/forms.py:346
 msgid "School term"
 msgstr "Учебный год"
 
 #: aleksis/apps/alsijil/forms.py:347
 msgid "Has lesson documentation"
@@ -433,15 +436,15 @@
 
 #: aleksis/apps/alsijil/models.py:468
 msgid "Can assign group role"
 msgstr "Может назначать роль группы"
 
 #: aleksis/apps/alsijil/models.py:484
 msgid "Assigned person"
-msgstr "Назначенное лицо"
+msgstr "Назначенное физлицо"
 
 #: aleksis/apps/alsijil/models.py:489 aleksis/apps/alsijil/tables.py:105
 #: aleksis/apps/alsijil/templates/alsijil/class_register/week_view.html:128
 #: aleksis/apps/alsijil/templates/alsijil/class_register/week_view.html:246
 #: aleksis/apps/alsijil/templates/alsijil/class_register/week_view.html:326
 msgid "Groups"
 msgstr "Группы"
@@ -489,38 +492,40 @@
 #: aleksis/apps/alsijil/preferences.py:34
 msgid "Allow primary group owners to register future absences for students in their groups"
 msgstr "Разрешить владельцам основных групп регистрировать будущие пропуски студентов в своих группах"
 
 #: aleksis/apps/alsijil/preferences.py:44
 msgid "Grant the owner of a parent group the same privileges as the owners of the respective child groups"
 msgstr ""
+"Наделить владельца родительской группы такими же правами, как у владельца "
+"соответствующих дочерних групп"
 
 #: aleksis/apps/alsijil/preferences.py:54
 msgid "Allow original teachers to edit their lessons although they are substituted"
 msgstr "Разрешить изначальным преподавателям редактировать свои уроки даже после их замены"
 
 #: aleksis/apps/alsijil/preferences.py:63
 msgid "Carry over data from first lesson period to the following lesson periods in lessons over multiple periods"
 msgstr "Переносить данные с первого урока в расписании на текущие уроки через несколько уроков"
 
 #: aleksis/apps/alsijil/preferences.py:66
 msgid "This will carry over data only if the data in the following periods are empty."
 msgstr "Это перенесёт данные только в случае отсутствия данных в последующих уроках."
 
 #: aleksis/apps/alsijil/preferences.py:75
-#, fuzzy
-#| msgid "Carry over data from first lesson period to the following lesson periods in lessons over multiple periods"
 msgid "Allow carrying over data from any lesson period to all other lesson                 periods with the same lesson and in the same week"
-msgstr "Переносить данные с первого урока в расписании на текущие уроки через несколько уроков"
+msgstr ""
+"Разрешить перенос данных с любого урока на все такие же "
+"уроки                 с таким же номером в расписании на той же неделе"
 
 #: aleksis/apps/alsijil/preferences.py:79
-#, fuzzy
-#| msgid "This will carry over data only if the data in the following periods are empty."
 msgid "This will carry over data only if the data in the aforementioned periods are empty."
-msgstr "Это перенесёт данные только в случае отсутствия данных в последующих уроках."
+msgstr ""
+"Это перенесёт данные только если в упомянутых выше уроках данные не "
+"заполнены."
 
 #: aleksis/apps/alsijil/preferences.py:88
 msgid "Carry over personal notes to all following lesson periods on the same day."
 msgstr "Переносить личные заметки на все последующие уроки того же дня."
 
 #: aleksis/apps/alsijil/preferences.py:97
 msgid "Allow teachers to open lesson periods on the same day and not just at the beginning of the period"
@@ -718,15 +723,15 @@
 #: aleksis/apps/alsijil/templates/alsijil/class_register/lesson.html:28
 #: aleksis/apps/alsijil/templates/alsijil/class_register/week_view.html:27
 msgid "Persons"
 msgstr "Люди"
 
 #: aleksis/apps/alsijil/templates/alsijil/class_register/lesson.html:36
 msgid "Seating plan"
-msgstr "План размещения"
+msgstr "План рассадки"
 
 #: aleksis/apps/alsijil/templates/alsijil/class_register/lesson.html:46
 #: aleksis/apps/alsijil/templates/alsijil/class_register/lesson.html:94
 msgid "Previous"
 msgstr "Предыдущий"
 
 #: aleksis/apps/alsijil/templates/alsijil/class_register/lesson.html:54
@@ -755,15 +760,15 @@
 msgstr ""
 "\n"
 "                  Этот урок перекрывает выходные и его нельзя редактировать.\n"
 "                "
 
 #: aleksis/apps/alsijil/templates/alsijil/class_register/person.html:10
 msgid "Class register: person"
-msgstr "Классный журнал: лицо"
+msgstr "Классный журнал: физлицо"
 
 #: aleksis/apps/alsijil/templates/alsijil/class_register/person.html:18
 #: aleksis/apps/alsijil/templates/alsijil/class_register/students_list.html:10
 msgid "Back"
 msgstr "Назад"
 
 #: aleksis/apps/alsijil/templates/alsijil/class_register/person.html:22
@@ -1140,62 +1145,63 @@
 
 #: aleksis/apps/alsijil/templates/alsijil/partials/lesson/tabs/seating_plan.html:8
 #, python-format
 msgid ""
 "Seating plan for %(group)s in\n"
 "          %(room)s"
 msgstr ""
-"План размещения %(group)s в\n"
+"План рассадки %(group)s в\n"
 "          %(room)s"
 
 #: aleksis/apps/alsijil/templates/alsijil/partials/lesson/tabs/seating_plan.html:14
 #, python-format
 msgid ""
 "\n"
 "            This seating plan is taken from the parent group of %(child_group)s.\n"
 "            If you want, you can take it over for your group and then customize it.\n"
 "          "
 msgstr ""
 "\n"
-"            Этот план размещения взят из родительской группы %(child_group)s.\n"
+"            Этот план рассадки взят из родительской группы %(child_group)s.\n"
 "            При необходимости Вы можете настроить его под свою группу.\n"
 "          "
 
 #: aleksis/apps/alsijil/templates/alsijil/partials/lesson/tabs/seating_plan.html:30
 msgid "Edit seating plan"
-msgstr "Редактировать план размещения"
+msgstr "Редактировать план рассадки"
 
 #: aleksis/apps/alsijil/templates/alsijil/partials/lesson/tabs/seating_plan.html:37
 msgid "Copy plan and edit"
 msgstr "Скопировать план и отредактировать"
 
 #: aleksis/apps/alsijil/templates/alsijil/partials/lesson/tabs/seating_plan.html:56
 msgid "There is no seating plan for this lesson."
-msgstr "Для этого урока нет плана размещения."
+msgstr "Для этого урока нет плана рассадки."
 
 #: aleksis/apps/alsijil/templates/alsijil/partials/lesson/tabs/seating_plan.html:64
 #, python-format
 msgid ""
 "\n"
 "                  Create a new seating plan for %(group)s (%(subject)s) in %(room)s\n"
 "                "
 msgstr ""
 "\n"
-"                  Создать новый план размещения %(group)s (%(subject)s) в %(room)s\n"
+"                  Создать новый план рассадки %(group)s (%(subject)s) в "
+"%(room)s\n"
 "                "
 
 #: aleksis/apps/alsijil/templates/alsijil/partials/lesson/tabs/seating_plan.html:78
 #, python-format
 msgid ""
 "\n"
 "                    Create a new seating plan for %(group)s in %(room)s\n"
 "                  "
 msgstr ""
 "\n"
-"                    Создать новый план размещения %(group)s в %(room)s\n"
+"                    Создать новый план рассадки %(group)s в %(room)s\n"
 "                  "
 
 #: aleksis/apps/alsijil/templates/alsijil/partials/lesson_status.html:6
 msgid "Data complete"
 msgstr "Данные заполнены"
 
 #: aleksis/apps/alsijil/templates/alsijil/partials/lesson_status.html:17
```

### Comparing `AlekSIS-App-Alsijil-3.0.dev0/aleksis/apps/alsijil/locale/tr_TR/LC_MESSAGES/django.po` & `aleksis_app_alsijil-3.0b0/aleksis/apps/alsijil/locale/tr_TR/LC_MESSAGES/django.po`

 * *Files identical despite different names*

### Comparing `AlekSIS-App-Alsijil-3.0.dev0/aleksis/apps/alsijil/locale/uk/LC_MESSAGES/django.mo` & `aleksis_app_alsijil-3.0b0/aleksis/apps/alsijil/locale/uk/LC_MESSAGES/django.mo`

 * *Files 1% similar despite different names*

#### msgunfmt {}

```diff
@@ -1,12 +1,12 @@
 msgid ""
 msgstr ""
 "Project-Id-Version: PACKAGE VERSION\n"
 "Report-Msgid-Bugs-To: \n"
-"PO-Revision-Date: 2022-06-22 19:59+0000\n"
+"PO-Revision-Date: 2023-01-25 05:58+0000\n"
 "Last-Translator: Serhii Horichenko <m@sgg.im>\n"
 "Language-Team: Ukrainian <https://translate.edugit.org/projects/aleksis/"
 "aleksis-app-alsijil/uk/>\n"
 "Language: uk\n"
 "MIME-Version: 1.0\n"
 "Content-Type: text/plain; charset=UTF-8\n"
 "Content-Transfer-Encoding: 8bit\n"
@@ -18,25 +18,25 @@
 
 msgid ""
 "\n"
 "                    Create a new seating plan for %(group)s in %(room)s\n"
 "                  "
 msgstr ""
 "\n"
-"                    Створити новий план розміщення %(group)s у %(room)s\n"
+"                    Створити новий план розсадження %(group)s у %(room)s\n"
 "                  "
 
 msgid ""
 "\n"
 "                  Create a new seating plan for %(group)s (%(subject)s) in "
 "%(room)s\n"
 "                "
 msgstr ""
 "\n"
-"                  Створити новий план розміщення %(group)s (%(subject)s) у "
+"                  Створити новий план розсадження %(group)s (%(subject)s) у "
 "%(room)s\n"
 "                "
 
 msgid ""
 "\n"
 "                  There are no affected lessons. Registering this absence "
 "won't have any effect.\n"
@@ -91,15 +91,15 @@
 "            This seating plan is taken from the parent group of "
 "%(child_group)s.\n"
 "            If you want, you can take it over for your group and then "
 "customize it.\n"
 "          "
 msgstr ""
 "\n"
-"            Цей план розміщення взятий із батьківської групи "
+"            Цей план розсадження взятий із батьківської групи "
 "%(child_group)s.\n"
 "            При необхідності, Ви можете його налаштувати під свою групу.\n"
 "          "
 
 msgid ""
 "\n"
 "        Copies of the class register, both digital and as printout, must\n"
@@ -243,14 +243,21 @@
 msgid "All assignments"
 msgstr "Усі призначення"
 
 msgid "All lessons"
 msgstr "Усі уроки"
 
 msgid ""
+"Allow carrying over data from any lesson period to all other "
+"lesson                 periods with the same lesson and in the same week"
+msgstr ""
+"Дозволити переносити дані з будь-якого уроку на усі інші                 "
+"уроки з таким самим номером урока на тому самому тижні"
+
+msgid ""
 "Allow group owners to assign group roles to the parents of the group's "
 "members"
 msgstr "Дозволити власникам груп призначати ролі груп батькам учасників груп"
 
 msgid ""
 "Allow original teachers to edit their lessons although they are substituted"
 msgstr ""
@@ -375,14 +382,18 @@
 msgid ""
 "Carry over data from first lesson period to the following lesson periods in "
 "lessons over multiple periods"
 msgstr ""
 "Переносити дані з першого уроку в розкладі на поточні уроки через декілька "
 "уроків"
 
+msgid "Carry over data to all other lessons with the same subject in this week"
+msgstr ""
+"Перенести дані на усі інші уроки з таким самим предметом на цьому тижні"
+
 msgid ""
 "Carry over personal notes to all following lesson periods on the same day."
 msgstr "Переносити особисті нотатки до всіх наступних уроків того ж дня."
 
 msgid "Change history"
 msgstr "Змінити історію"
 
@@ -476,15 +487,15 @@
 msgid "Edit group role"
 msgstr "Редагувати роль групи"
 
 msgid "Edit group role assignment"
 msgstr "Редагувати призначення ролі групи"
 
 msgid "Edit seating plan"
-msgstr "Редагувати план розміщення"
+msgstr "Редагувати план розсадження"
 
 msgid "End date"
 msgstr "Дата закінчення"
 
 msgid "End period"
 msgstr "Закінчення уроків"
 
@@ -549,14 +560,21 @@
 
 msgid "General"
 msgstr "Загальне"
 
 msgid "Generate printout"
 msgstr "Підготувати для друку"
 
+msgid ""
+"Grant the owner of a parent group the same privileges as the owners of the "
+"respective child groups"
+msgstr ""
+"Надати власнику батьківської групи такі самі повноваження, як і власникам "
+"відповідних підлеглих груп"
+
 msgid "Group"
 msgstr "Група"
 
 msgid "Group note"
 msgstr "Групова нотатка"
 
 msgid "Group notes for previous lesson:"
@@ -592,15 +610,15 @@
 msgid "Homework for the next lesson"
 msgstr "Домашня робота на наступний урок"
 
 msgid "Homework for this lesson:"
 msgstr "Домашня робота на цей урок:"
 
 msgid "Icon"
-msgstr "Іконка"
+msgstr "Піктограма"
 
 msgid ""
 "If checked, this excuse type will be counted as a missed lesson. If not "
 "checked,it won't show up in the absence report."
 msgstr ""
 "Якщо відмічено, цей тип пояснення буде зарахований як пропущений урок. Якщо "
 "не відмічено, то без запису у звіт відсутності."
@@ -795,21 +813,21 @@
 msgid "Save"
 msgstr "Зберегти"
 
 msgid "School term"
 msgstr "Навчальний рік"
 
 msgid "Seating plan"
-msgstr "План розміщення"
+msgstr "План розсадження"
 
 msgid ""
 "Seating plan for %(group)s in\n"
 "          %(room)s"
 msgstr ""
-"План розміщення %(group)s у\n"
+"План розсадження %(group)s у\n"
 "          %(room)s"
 
 msgid "Select"
 msgstr "Обрати"
 
 msgid "Set current groups"
 msgstr "Встановити поточні групи"
@@ -967,15 +985,21 @@
 msgid "The personal note is related to a cancelled lesson."
 msgstr "У скасованого уроку є пов'язані особисті нотатки."
 
 msgid "The personal notes have been saved."
 msgstr "Особисті нотатки збережені."
 
 msgid "There is no seating plan for this lesson."
-msgstr "Для цього уроку немає плану розміщення."
+msgstr "Для цього уроку немає плану розсадження."
+
+msgid ""
+"This will carry over data only if the data in the aforementioned periods are "
+"empty."
+msgstr ""
+"Це перенесе дані лише в тому разі, коли у вищезгаданих уроках даних немає."
 
 msgid ""
 "This will carry over data only if the data in the following periods are "
 "empty."
 msgstr "Це перенесе дані лише в тому разі, коли в поточних уроках даних немає."
 
 msgid "Toggle filters"
```

### Comparing `AlekSIS-App-Alsijil-3.0.dev0/aleksis/apps/alsijil/locale/uk/LC_MESSAGES/django.po` & `aleksis_app_alsijil-3.0b0/aleksis/apps/alsijil/locale/uk/LC_MESSAGES/django.po`

 * *Files 1% similar despite different names*

```diff
@@ -4,26 +4,22 @@
 # FIRST AUTHOR <EMAIL@ADDRESS>, YEAR.
 #
 msgid ""
 msgstr ""
 "Project-Id-Version: PACKAGE VERSION\n"
 "Report-Msgid-Bugs-To: \n"
 "POT-Creation-Date: 2022-06-25 15:28+0200\n"
-"PO-Revision-Date: 2022-06-22 19:59+0000\n"
+"PO-Revision-Date: 2023-01-25 05:58+0000\n"
 "Last-Translator: Serhii Horichenko <m@sgg.im>\n"
-"Language-Team: Ukrainian <https://translate.edugit.org/projects/aleksis/"
-"aleksis-app-alsijil/uk/>\n"
+"Language-Team: Ukrainian <https://translate.edugit.org/projects/aleksis/aleksis-app-alsijil/uk/>\n"
 "Language: uk\n"
 "MIME-Version: 1.0\n"
 "Content-Type: text/plain; charset=UTF-8\n"
 "Content-Transfer-Encoding: 8bit\n"
-"Plural-Forms: nplurals=4; plural=(n % 1 == 0 && n % 10 == 1 && n % 100 != "
-"11 ? 0 : n % 1 == 0 && n % 10 >= 2 && n % 10 <= 4 && (n % 100 < 12 || n % "
-"100 > 14) ? 1 : n % 1 == 0 && (n % 10 ==0 || (n % 10 >=5 && n % 10 <=9) || "
-"(n % 100 >=11 && n % 100 <=14 )) ? 2: 3);\n"
+"Plural-Forms: nplurals=4; plural=(n % 1 == 0 && n % 10 == 1 && n % 100 != 11 ? 0 : n % 1 == 0 && n % 10 >= 2 && n % 10 <= 4 && (n % 100 < 12 || n % 100 > 14) ? 1 : n % 1 == 0 && (n % 10 ==0 || (n % 10 >=5 && n % 10 <=9) || (n % 100 >=11 && n % 100 <=14 )) ? 2: 3);\n"
 "X-Generator: Weblate 4.12.1\n"
 
 #: aleksis/apps/alsijil/actions.py:18
 msgid "Mark as excused"
 msgstr "Позначити як пояснений"
 
 #: aleksis/apps/alsijil/actions.py:25
@@ -139,15 +135,15 @@
 
 #: aleksis/apps/alsijil/forms.py:47
 msgid "Homework for the next lesson"
 msgstr "Домашня робота на наступний урок"
 
 #: aleksis/apps/alsijil/forms.py:53
 msgid "Carry over data to all other lessons with the same subject in this week"
-msgstr ""
+msgstr "Перенести дані на усі інші уроки з таким самим предметом на цьому тижні"
 
 #: aleksis/apps/alsijil/forms.py:98 aleksis/apps/alsijil/forms.py:256
 #: aleksis/apps/alsijil/forms.py:348
 #: aleksis/apps/alsijil/templates/alsijil/print/full_register.html:219
 #: aleksis/apps/alsijil/forms.py:73 aleksis/apps/alsijil/forms.py:214
 #: aleksis/apps/alsijil/forms.py:301
 msgid "Group"
@@ -456,15 +452,15 @@
 
 #: aleksis/apps/alsijil/models.py:442 aleksis/apps/alsijil/models.py:431
 msgid "Extra mark"
 msgstr "Додаткова відмітка"
 
 #: aleksis/apps/alsijil/models.py:456 aleksis/apps/alsijil/models.py:445
 msgid "Icon"
-msgstr "Іконка"
+msgstr "Піктограма"
 
 #: aleksis/apps/alsijil/models.py:457 aleksis/apps/alsijil/models.py:446
 msgid "Colour"
 msgstr "Колір"
 
 #: aleksis/apps/alsijil/models.py:463 aleksis/apps/alsijil/models.py:478
 #: aleksis/apps/alsijil/templates/alsijil/group_role/assigned_list.html:62
@@ -545,14 +541,16 @@
 "своїх групах"
 
 #: aleksis/apps/alsijil/preferences.py:44
 msgid ""
 "Grant the owner of a parent group the same privileges as the owners of the "
 "respective child groups"
 msgstr ""
+"Надати власнику батьківської групи такі самі повноваження, як і власникам "
+"відповідних підлеглих груп"
 
 #: aleksis/apps/alsijil/preferences.py:54
 #: aleksis/apps/alsijil/preferences.py:43
 msgid ""
 "Allow original teachers to edit their lessons although they are substituted"
 msgstr ""
 "Дозволити початковим викладачам редагувати свої уроки навіть після їх заміни"
@@ -570,28 +568,27 @@
 #: aleksis/apps/alsijil/preferences.py:55
 msgid ""
 "This will carry over data only if the data in the following periods are "
 "empty."
 msgstr "Це перенесе дані лише в тому разі, коли в поточних уроках даних немає."
 
 #: aleksis/apps/alsijil/preferences.py:75
-#, fuzzy
 msgid ""
 "Allow carrying over data from any lesson period to all other "
 "lesson                 periods with the same lesson and in the same week"
 msgstr ""
-"Переносити дані з першого уроку в розкладі на поточні уроки через декілька "
-"уроків"
+"Дозволити переносити дані з будь-якого уроку на усі інші                 "
+"уроки з таким самим номером урока на тому самому тижні"
 
 #: aleksis/apps/alsijil/preferences.py:79
-#, fuzzy
 msgid ""
 "This will carry over data only if the data in the aforementioned periods are "
 "empty."
-msgstr "Це перенесе дані лише в тому разі, коли в поточних уроках даних немає."
+msgstr ""
+"Це перенесе дані лише в тому разі, коли у вищезгаданих уроках даних немає."
 
 #: aleksis/apps/alsijil/preferences.py:88
 #: aleksis/apps/alsijil/preferences.py:63
 msgid ""
 "Carry over personal notes to all following lesson periods on the same day."
 msgstr "Переносити особисті нотатки до всіх наступних уроків того ж дня."
 
@@ -815,15 +812,15 @@
 #: aleksis/apps/alsijil/templates/alsijil/class_register/lesson.html:28
 #: aleksis/apps/alsijil/templates/alsijil/class_register/week_view.html:27
 msgid "Persons"
 msgstr "Особи"
 
 #: aleksis/apps/alsijil/templates/alsijil/class_register/lesson.html:36
 msgid "Seating plan"
-msgstr "План розміщення"
+msgstr "План розсадження"
 
 #: aleksis/apps/alsijil/templates/alsijil/class_register/lesson.html:46
 #: aleksis/apps/alsijil/templates/alsijil/class_register/lesson.html:94
 msgid "Previous"
 msgstr "Попередній"
 
 #: aleksis/apps/alsijil/templates/alsijil/class_register/lesson.html:54
@@ -1247,67 +1244,67 @@
 
 #: aleksis/apps/alsijil/templates/alsijil/partials/lesson/tabs/seating_plan.html:8
 #, python-format
 msgid ""
 "Seating plan for %(group)s in\n"
 "          %(room)s"
 msgstr ""
-"План розміщення %(group)s у\n"
+"План розсадження %(group)s у\n"
 "          %(room)s"
 
 #: aleksis/apps/alsijil/templates/alsijil/partials/lesson/tabs/seating_plan.html:14
 #, python-format
 msgid ""
 "\n"
 "            This seating plan is taken from the parent group of "
 "%(child_group)s.\n"
 "            If you want, you can take it over for your group and then "
 "customize it.\n"
 "          "
 msgstr ""
 "\n"
-"            Цей план розміщення взятий із батьківської групи "
+"            Цей план розсадження взятий із батьківської групи "
 "%(child_group)s.\n"
 "            При необхідності, Ви можете його налаштувати під свою групу.\n"
 "          "
 
 #: aleksis/apps/alsijil/templates/alsijil/partials/lesson/tabs/seating_plan.html:30
 msgid "Edit seating plan"
-msgstr "Редагувати план розміщення"
+msgstr "Редагувати план розсадження"
 
 #: aleksis/apps/alsijil/templates/alsijil/partials/lesson/tabs/seating_plan.html:37
 msgid "Copy plan and edit"
 msgstr "Скопіювати план та відредагувати"
 
 #: aleksis/apps/alsijil/templates/alsijil/partials/lesson/tabs/seating_plan.html:56
 msgid "There is no seating plan for this lesson."
-msgstr "Для цього уроку немає плану розміщення."
+msgstr "Для цього уроку немає плану розсадження."
 
 #: aleksis/apps/alsijil/templates/alsijil/partials/lesson/tabs/seating_plan.html:64
 #, python-format
 msgid ""
 "\n"
 "                  Create a new seating plan for %(group)s (%(subject)s) in "
 "%(room)s\n"
 "                "
 msgstr ""
 "\n"
-"                  Створити новий план розміщення %(group)s (%(subject)s) у "
+"                  Створити новий план розсадження %(group)s (%(subject)s) у "
 "%(room)s\n"
 "                "
 
 #: aleksis/apps/alsijil/templates/alsijil/partials/lesson/tabs/seating_plan.html:78
 #, python-format
 msgid ""
 "\n"
 "                    Create a new seating plan for %(group)s in %(room)s\n"
 "                  "
 msgstr ""
 "\n"
-"                    Створити новий план розміщення %(group)s у %(room)s\n"
+"                    Створити новий план розсадження %(group)s у %(room)s\n"
 "                  "
 
 #: aleksis/apps/alsijil/templates/alsijil/partials/lesson_status.html:6
 msgid "Data complete"
 msgstr "Дані заповнені"
 
 #: aleksis/apps/alsijil/templates/alsijil/partials/lesson_status.html:17
```

### Comparing `AlekSIS-App-Alsijil-3.0.dev0/aleksis/apps/alsijil/managers.py` & `aleksis_app_alsijil-3.0b0/aleksis/apps/alsijil/managers.py`

 * *Files 0% similar despite different names*

```diff
@@ -115,15 +115,15 @@
         )
 
 
 class PersonalNoteQuerySet(RegisterObjectRelatedQuerySet, QuerySet):
     def not_empty(self):
         """Get all not empty personal notes."""
         return self.filter(
-            ~Q(remarks="") | Q(absent=True) | ~Q(late=0) | Q(extra_marks__isnull=False)
+            ~Q(remarks="") | Q(absent=True) | ~Q(tardiness=0) | Q(extra_marks__isnull=False)
         )
 
 
 class LessonDocumentationManager(CurrentSiteManagerWithoutMigrations):
     pass
```

### Comparing `AlekSIS-App-Alsijil-3.0.dev0/aleksis/apps/alsijil/migrations/0001_initial.py` & `aleksis_app_alsijil-3.0b0/aleksis/apps/alsijil/migrations/0001_initial.py`

 * *Files identical despite different names*

### Comparing `AlekSIS-App-Alsijil-3.0.dev0/aleksis/apps/alsijil/migrations/0002_excuse_type.py` & `aleksis_app_alsijil-3.0b0/aleksis/apps/alsijil/migrations/0002_excuse_type.py`

 * *Files identical despite different names*

### Comparing `AlekSIS-App-Alsijil-3.0.dev0/aleksis/apps/alsijil/migrations/0003_extra_mark.py` & `aleksis_app_alsijil-3.0b0/aleksis/apps/alsijil/migrations/0003_extra_mark.py`

 * *Files identical despite different names*

### Comparing `AlekSIS-App-Alsijil-3.0.dev0/aleksis/apps/alsijil/migrations/0005_groups_of_person.py` & `aleksis_app_alsijil-3.0b0/aleksis/apps/alsijil/migrations/0005_groups_of_person.py`

 * *Files identical despite different names*

### Comparing `AlekSIS-App-Alsijil-3.0.dev0/aleksis/apps/alsijil/migrations/0007_personal_note_lesson_documentation_year.py` & `aleksis_app_alsijil-3.0b0/aleksis/apps/alsijil/migrations/0007_personal_note_lesson_documentation_year.py`

 * *Files identical despite different names*

### Comparing `AlekSIS-App-Alsijil-3.0.dev0/aleksis/apps/alsijil/migrations/0008_global_permissions.py` & `aleksis_app_alsijil-3.0b0/aleksis/apps/alsijil/migrations/0008_global_permissions.py`

 * *Files identical despite different names*

### Comparing `AlekSIS-App-Alsijil-3.0.dev0/aleksis/apps/alsijil/migrations/0009_group_roles.py` & `aleksis_app_alsijil-3.0b0/aleksis/apps/alsijil/migrations/0009_group_roles.py`

 * *Files identical despite different names*

### Comparing `AlekSIS-App-Alsijil-3.0.dev0/aleksis/apps/alsijil/migrations/0010_events_extra_lessons.py` & `aleksis_app_alsijil-3.0b0/aleksis/apps/alsijil/migrations/0010_events_extra_lessons.py`

 * *Files identical despite different names*

### Comparing `AlekSIS-App-Alsijil-3.0.dev0/aleksis/apps/alsijil/migrations/0011_tardiness_positive.py` & `aleksis_app_alsijil-3.0b0/aleksis/apps/alsijil/migrations/0011_tardiness_positive.py`

 * *Files identical despite different names*

### Comparing `AlekSIS-App-Alsijil-3.0.dev0/aleksis/apps/alsijil/migrations/0012_unique_relation.py` & `aleksis_app_alsijil-3.0b0/aleksis/apps/alsijil/migrations/0012_unique_relation.py`

 * *Files identical despite different names*

### Comparing `AlekSIS-App-Alsijil-3.0.dev0/aleksis/apps/alsijil/migrations/0013_fix_uniqueness_per_site.py` & `aleksis_app_alsijil-3.0b0/aleksis/apps/alsijil/migrations/0013_fix_uniqueness_per_site.py`

 * *Files identical despite different names*

### Comparing `AlekSIS-App-Alsijil-3.0.dev0/aleksis/apps/alsijil/migrations/0014_fix_unique_lesson_documentation.py` & `aleksis_app_alsijil-3.0b0/aleksis/apps/alsijil/migrations/0014_fix_unique_lesson_documentation.py`

 * *Files identical despite different names*

### Comparing `AlekSIS-App-Alsijil-3.0.dev0/aleksis/apps/alsijil/migrations/0015_fix_unique_personal_note.py` & `aleksis_app_alsijil-3.0b0/aleksis/apps/alsijil/migrations/0015_fix_unique_personal_note.py`

 * *Files identical despite different names*

### Comparing `AlekSIS-App-Alsijil-3.0.dev0/aleksis/apps/alsijil/migrations/0016_add_not_counted_excuse_types.py` & `aleksis_app_alsijil-3.0b0/aleksis/apps/alsijil/migrations/0016_add_not_counted_excuse_types.py`

 * *Files identical despite different names*

### Comparing `AlekSIS-App-Alsijil-3.0.dev0/aleksis/apps/alsijil/model_extensions.py` & `aleksis_app_alsijil-3.0b0/aleksis/apps/alsijil/model_extensions.py`

 * *Files 2% similar despite different names*

```diff
@@ -322,20 +322,20 @@
 
 
 @LessonPeriod.method
 def get_tardinesses(self, week: Optional[CalendarWeek] = None) -> QuerySet:
     """Get all personal notes of late persons for this lesson."""
     if not week:
         week = self.week
-    return self.personal_notes.filter(week=week.week, year=week.year, late__gt=0)
+    return self.personal_notes.filter(week=week.week, year=week.year, tardiness__gt=0)
 
 
 def get_tardinesses_simple(self, week: Optional[CalendarWeek] = None) -> QuerySet:
     """Get all personal notes of late persons for this event/extra lesson."""
-    return self.personal_notes.filter(late__gt=0)
+    return self.personal_notes.filter(tardiness__gt=0)
 
 
 Event.method(get_tardinesses_simple, "get_tardinesses")
 ExtraLesson.method(get_tardinesses_simple, "get_tardinesses")
 
 
 @LessonPeriod.method
@@ -430,59 +430,66 @@
             ),
         )
     ).annotate(
         absences_count=Count(
             "filtered_personal_notes",
             filter=Q(filtered_personal_notes__absent=True)
             & ~Q(filtered_personal_notes__excuse_type__count_as_absent=False),
+            distinct=True,
         ),
         excused=Count(
             "filtered_personal_notes",
             filter=Q(
                 filtered_personal_notes__absent=True,
                 filtered_personal_notes__excused=True,
             )
             & ~Q(filtered_personal_notes__excuse_type__count_as_absent=False),
+            distinct=True,
         ),
         excused_without_excuse_type=Count(
             "filtered_personal_notes",
             filter=Q(
                 filtered_personal_notes__absent=True,
                 filtered_personal_notes__excused=True,
                 filtered_personal_notes__excuse_type__isnull=True,
             ),
+            distinct=True,
         ),
         unexcused=Count(
             "filtered_personal_notes",
             filter=Q(filtered_personal_notes__absent=True, filtered_personal_notes__excused=False),
+            distinct=True,
         ),
-        tardiness=Sum("filtered_personal_notes__late"),
+        tardiness=Sum("filtered_personal_notes__tardiness"),
         tardiness_count=Count(
             "filtered_personal_notes",
-            filter=Q(filtered_personal_notes__late__gt=0),
+            filter=Q(filtered_personal_notes__tardiness__gt=0),
+            distinct=True,
         ),
     )
 
     for extra_mark in ExtraMark.objects.all():
         persons = persons.annotate(
             **{
                 extra_mark.count_label: Count(
                     "filtered_personal_notes",
                     filter=Q(filtered_personal_notes__extra_marks=extra_mark),
+                    distinct=True,
                 )
             }
         )
 
     for excuse_type in ExcuseType.objects.all():
         persons = persons.annotate(
             **{
                 excuse_type.count_label: Count(
                     "filtered_personal_notes__absent",
                     filter=Q(
                         filtered_personal_notes__absent=True,
                         filtered_personal_notes__excuse_type=excuse_type,
                     ),
+                    distinct=True,
                 )
             }
         )
 
     return persons
```

### Comparing `AlekSIS-App-Alsijil-3.0.dev0/aleksis/apps/alsijil/models.py` & `aleksis_app_alsijil-3.0b0/aleksis/apps/alsijil/models.py`

 * *Files 5% similar despite different names*

```diff
@@ -1,14 +1,15 @@
 from datetime import date
 from typing import Optional, Union
 from urllib.parse import urlparse
 
 from django.db import models
 from django.db.models.constraints import CheckConstraint
 from django.db.models.query_utils import Q
+from django.urls import reverse
 from django.utils.formats import date_format
 from django.utils.translation import gettext_lazy as _
 
 from calendarweek import CalendarWeek
 from colorfield.fields import ColorField
 
 from aleksis.apps.alsijil.data_checks import (
@@ -27,14 +28,15 @@
     LessonDocumentationQuerySet,
     PersonalNoteManager,
     PersonalNoteQuerySet,
 )
 from aleksis.apps.chronos.managers import GroupPropertiesMixin
 from aleksis.apps.chronos.mixins import WeekRelatedMixin
 from aleksis.apps.chronos.models import Event, ExtraLesson, LessonPeriod, TimePeriod
+from aleksis.core.data_checks import field_validation_data_check_factory
 from aleksis.core.mixins import ExtensibleModel, GlobalPermissionModel
 from aleksis.core.models import SchoolTerm
 from aleksis.core.util.core_helpers import get_site_preferences
 from aleksis.core.util.model_helpers import ICONS
 
 
 def isidentifier(value: str) -> bool:
@@ -239,15 +241,15 @@
         "chronos.Event", models.CASCADE, related_name="personal_notes", blank=True, null=True
     )
     extra_lesson = models.ForeignKey(
         "chronos.ExtraLesson", models.CASCADE, related_name="personal_notes", blank=True, null=True
     )
 
     absent = models.BooleanField(default=False)
-    late = models.PositiveSmallIntegerField(default=0)
+    tardiness = models.PositiveSmallIntegerField(default=0)
     excused = models.BooleanField(default=False)
     excuse_type = models.ForeignKey(
         ExcuseType,
         on_delete=models.SET_NULL,
         null=True,
         blank=True,
         verbose_name=_("Excuse type"),
@@ -271,15 +273,15 @@
         .. warning ::
 
             This won't save the data, please execute ``save`` extra.
         """
         defaults = PersonalNote()
 
         self.absent = defaults.absent
-        self.late = defaults.late
+        self.tardiness = defaults.tardiness
         self.excused = defaults.excused
         self.excuse_type = defaults.excuse_type
         self.remarks = defaults.remarks
         self.extra_marks.clear()
 
     def __str__(self) -> str:
         return f"{self.date_formatted}, {self.lesson_period}, {self.person}"
@@ -341,39 +343,37 @@
         "chronos.ExtraLesson", models.CASCADE, related_name="documentations", blank=True, null=True
     )
 
     topic = models.CharField(verbose_name=_("Lesson topic"), max_length=200, blank=True)
     homework = models.CharField(verbose_name=_("Homework"), max_length=200, blank=True)
     group_note = models.CharField(verbose_name=_("Group note"), max_length=200, blank=True)
 
-    def carry_over_data(self, all_periods_of_lesson: LessonPeriod, force: bool):
-        """Carry over data to given periods in this lesson.
-
-        Does overwrite existing data in case ``force`` is set to ``True``.
+    def carry_over_data(self, all_periods_of_lesson: LessonPeriod):
+        """Carry over data to given periods in this lesson if data is not already set.
 
         Both forms of carrying over data can be deactivated using site preferences
-        ``alsijil__carry_over_next_periods`` and ``alsijil__save_lesson_documentations_by_week``
+        ``alsijil__carry_over_next_periods`` and ``alsijil__allow_carry_over_same_week``
         respectively.
         """
         for period in all_periods_of_lesson:
             lesson_documentation = period.get_or_create_lesson_documentation(
                 CalendarWeek(week=self.week, year=self.year)
             )
 
             changed = False
 
-            if not lesson_documentation.topic or force:
+            if not lesson_documentation.topic:
                 lesson_documentation.topic = self.topic
                 changed = True
 
-            if not lesson_documentation.homework or force:
+            if not lesson_documentation.homework:
                 lesson_documentation.homework = self.homework
                 changed = True
 
-            if not lesson_documentation.group_note or force:
+            if not lesson_documentation.group_note:
                 lesson_documentation.group_note = self.group_note
                 changed = True
 
             if changed:
                 lesson_documentation.save(carry_over_next_periods=False)
 
     def __str__(self) -> str:
@@ -386,16 +386,15 @@
             and self.lesson_period
             and carry_over_next_periods
         ):
             self.carry_over_data(
                 LessonPeriod.objects.filter(
                     lesson=self.lesson_period.lesson,
                     period__weekday=self.lesson_period.period.weekday,
-                ),
-                False,
+                )
             )
         super().save(*args, **kwargs)
 
     class Meta:
         verbose_name = _("Lesson documentation")
         verbose_name_plural = _("Lesson documentations")
         ordering = [
@@ -449,14 +448,16 @@
                 fields=("site_id", "short_name"), name="unique_mark_short_name"
             ),
             models.UniqueConstraint(fields=("site_id", "name"), name="unique_mark_name"),
         ]
 
 
 class GroupRole(ExtensibleModel):
+    data_checks = [field_validation_data_check_factory("alsijil", "GroupRole", "icon")]
+
     objects = GroupRoleManager.from_queryset(GroupRoleQuerySet)()
 
     name = models.CharField(max_length=255, verbose_name=_("Name"))
     icon = models.CharField(max_length=50, blank=True, choices=ICONS, verbose_name=_("Icon"))
     colour = ColorField(blank=True, verbose_name=_("Colour"))
 
     def __str__(self):
@@ -466,14 +467,17 @@
         verbose_name = _("Group role")
         verbose_name_plural = _("Group roles")
         constraints = [
             models.UniqueConstraint(fields=("site_id", "name"), name="unique_role_per_site"),
         ]
         permissions = (("assign_group_role", _("Can assign group role")),)
 
+    def get_absolute_url(self) -> str:
+        return reverse("edit_group_role", args=[self.id])
+
 
 class GroupRoleAssignment(GroupPropertiesMixin, ExtensibleModel):
     objects = GroupRoleAssignmentManager.from_queryset(GroupRoleAssignmentQuerySet)()
 
     role = models.ForeignKey(
         GroupRole,
         on_delete=models.CASCADE,
```

### Comparing `AlekSIS-App-Alsijil-3.0.dev0/aleksis/apps/alsijil/preferences.py` & `aleksis_app_alsijil-3.0b0/aleksis/apps/alsijil/preferences.py`

 * *Files 8% similar despite different names*

```diff
@@ -63,19 +63,25 @@
         "Carry over data from first lesson period to the "
         "following lesson periods in lessons over multiple periods"
     )
     help_text = _("This will carry over data only if the data in the following periods are empty.")
 
 
 @site_preferences_registry.register
-class SaveLessonDocumentationsPerWeek(BooleanPreference):
+class AllowCarryOverLessonDocumentationToCurrentWeek(BooleanPreference):
     section = alsijil
-    name = "save_lesson_documentations_by_week"
+    name = "allow_carry_over_same_week"
     default = False
-    verbose_name = _("Save lesson documentations per week instead of per lesson period")
+    verbose_name = _(
+        "Allow carrying over data from any lesson period to all other lesson \
+                periods with the same lesson and in the same week"
+    )
+    help_text = _(
+        "This will carry over data only if the data in the aforementioned periods are empty."
+    )
 
 
 @site_preferences_registry.register
 class CarryOverPersonalNotesToNextPeriods(BooleanPreference):
     section = alsijil
     name = "carry_over_personal_notes"
     default = True
```

### Comparing `AlekSIS-App-Alsijil-3.0.dev0/aleksis/apps/alsijil/rules.py` & `aleksis_app_alsijil-3.0b0/aleksis/apps/alsijil/rules.py`

 * *Files 2% similar despite different names*

```diff
@@ -152,23 +152,28 @@
     )
     | has_global_perm("alsijil.view_personalnote")
     | has_object_perm("core.view_personalnote_group")
 )
 add_perm("alsijil.view_week_personalnote_rule", view_week_personal_notes_predicate)
 
 # Register absence
-register_absence_predicate = has_person & (
+view_register_absence_predicate = has_person & (
     (
         is_person_group_owner
         & is_site_preference_set("alsijil", "register_absence_as_primary_group_owner")
     )
     | has_global_perm("alsijil.register_absence")
+)
+
+register_absence_predicate = has_person & (
+    view_register_absence_predicate
     | has_object_perm("core.register_absence_person")
     | has_person_group_object_perm("core.register_absence_group")
 )
+add_perm("alsijil.view_register_absence_rule", view_register_absence_predicate)
 add_perm("alsijil.register_absence_rule", register_absence_predicate)
 
 # View full register for group
 view_full_register_predicate = has_person & (
     is_group_owner
     | (
         is_parent_group_owner
@@ -195,19 +200,14 @@
         & is_site_preference_set("alsijil", "inherit_privileges_from_parent_group")
     )
     | has_global_perm("alsijil.view_personalnote")
     | has_object_perm("core.view_personalnote_group")
 )
 add_perm("alsijil.view_students_list_rule", view_students_list_predicate)
 
-# View CourseBook
-view_coursebook_predicate = has_person & is_teacher
-add_perm("alsijil.view_coursebook_rule", view_my_students_predicate)
-
-
 # View person overview
 view_person_overview_predicate = has_person & (
     (is_current_person & is_site_preference_set("alsijil", "view_own_personal_notes"))
     | is_person_group_owner
 )
 add_perm("alsijil.view_person_overview_rule", view_person_overview_predicate)
```

### Comparing `AlekSIS-App-Alsijil-3.0.dev0/aleksis/apps/alsijil/static/css/alsijil/alsijil.css` & `aleksis_app_alsijil-3.0b0/aleksis/apps/alsijil/static/css/alsijil/alsijil.css`

 * *Files 18% similar despite different names*

```diff
@@ -5,56 +5,56 @@
 table a.tr-link {
   display: block;
   width: inherit;
   height: inherit;
 }
 
 .collapsible-icon-right {
-	align-self: end;
-	flex-grow: 100;
-	text-align: right!important;
+  align-self: end;
+  flex-grow: 100;
+  text-align: right !important;
 }
 
 @media only screen and (min-width: 1201px) {
-    .hide-on-extra-large-only {
-        display: none;
-    }
+  .hide-on-extra-large-only {
+    display: none;
+  }
 }
 
 @media only screen and (max-width: 1200px) {
-    .show-on-extra-large {
-        display: none;
-    }
+  .show-on-extra-large {
+    display: none;
+  }
 }
 
 @media only screen and (max-width: 600px) {
-    .collection .collection-item.avatar {
-        padding-left: 20px;
-    }
-    .collection .collection-item.avatar:not(.circle-clipper) > .circle {
-        position: relative;
-        margin-bottom: 10px;
-    }
+  .collection .collection-item.avatar {
+    padding-left: 20px;
+  }
+  .collection .collection-item.avatar:not(.circle-clipper) > .circle {
+    position: relative;
+    margin-bottom: 10px;
+  }
 }
 
 .collapsible li .show-on-active {
-    display: none;
+  display: none;
 }
 
 .collapsible li.active .show-on-active {
-    display: block;
+  display: block;
 }
 
 th.chip-height {
-    height: 67px;
-    line-height: 2.2;
+  height: 67px;
+  line-height: 2.2;
 }
 
 .collection-item.chip-height {
-    height: 52px;
-    line-height: 2.2;
+  height: 52px;
+  line-height: 2.2;
 }
 
 li.collection-item.button-height {
-    height: 58px;
-    line-height: 2.5;
+  height: 58px;
+  line-height: 2.5;
 }
```

### Comparing `AlekSIS-App-Alsijil-3.0.dev0/aleksis/apps/alsijil/static/css/alsijil/full_register.css` & `aleksis_app_alsijil-3.0b0/aleksis/apps/alsijil/static/css/alsijil/full_register.css`

 * *Files 10% similar despite different names*

```diff
@@ -1,72 +1,76 @@
-table.small-print, td.small-print, th.small-print {
-    font-size: 10pt;
+table.small-print,
+td.small-print,
+th.small-print {
+  font-size: 10pt;
 }
 
 #signatures {
-    padding-top: 3em;
+  padding-top: 3em;
 }
 
 #signatures .signature {
-    display: inline-block;
-    width: 12em;
-    border-top: 1px solid;
-    margin-right: 20px;
+  display: inline-block;
+  width: 12em;
+  border-top: 1px solid;
+  margin-right: 20px;
 }
 
 tr {
-    border-bottom: 1px solid rgba(0, 0, 0, 0.3);
+  border-bottom: 1px solid rgba(0, 0, 0, 0.3);
 }
 
-td, th {
-    padding: 1px;
+td,
+th {
+  padding: 1px;
 }
 
 tr.lessons-day-first {
-    border-top: 3px solid rgba(0, 0, 0, 0.3);
+  border-top: 3px solid rgba(0, 0, 0, 0.3);
 }
 
-td.rotate, th.rotate {
-    text-align: center;
-    transform: rotate(-90deg);
+td.rotate,
+th.rotate {
+  text-align: center;
+  transform: rotate(-90deg);
 }
 
 tr.lesson-cancelled td {
-    background-color: #EF9A9A;
+  background-color: #ef9a9a;
 }
 
 tr.lesson-substituted td {
-    background-color: #ffb74d;
+  background-color: #ffb74d;
 }
 
 td.lesson-notes {
-    font-size: 80%;
+  font-size: 80%;
 }
 
 td.lesson-notes span.lesson-note-absent {
-    color: #cc0000;
+  color: #cc0000;
 }
 
 td.lesson-notes span.lesson-note-late {
-    color: #ff9933;
+  color: #ff9933;
 }
 
 td.lesson-notes span.lesson-note-excused {
-    color: #009933;
+  color: #009933;
 }
 
 table.person-info {
-    border: none;
+  border: none;
 }
 
 table.person-info td.person-img {
-    text-align: center;
+  text-align: center;
 }
 
 table.person-info td.person-img img {
-    max-height: 30mm;
+  max-height: 30mm;
 }
 
 img.max-size-600 {
-    max-width: 600px;
-    max-height: 600px;
+  max-width: 600px;
+  max-height: 600px;
 }
```

### Comparing `AlekSIS-App-Alsijil-3.0.dev0/aleksis/apps/alsijil/static/css/alsijil/lesson.css` & `aleksis_app_alsijil-3.0b0/aleksis/apps/alsijil/static/css/alsijil/lesson.css`

 * *Files 12% similar despite different names*

```diff
@@ -1,133 +1,138 @@
 .alsijil-check-box {
-    margin-right: 10px;
+  margin-right: 10px;
 }
 
 .alsijil-check-box [type="checkbox"] {
-    padding-left: 30px;
+  padding-left: 30px;
 }
 
 .alsijil-lesson-cancelled {
-    text-decoration: line-through;
+  text-decoration: line-through;
 }
 
-.alsijil-tardiness-text{
-    vertical-align: super;
+.alsijil-tardiness-text {
+  vertical-align: super;
 }
 
-
 @media only screen and (max-width: 992px) {
-    .no-mobile-card {
-        border: unset;
-        padding: unset;
-        margin: unset;
-        box-shadow: unset;
-    }
-    .no-mobile-card .card-content {
-        padding: unset;
-    }
-    table.alsijil-table.horizontal-on-small {
-        display: block;
-        max-width: calc(100vw - 40px);
-    }
-    table.alsijil-table.horizontal-on-small thead {
-        display: none;
-    }
-    table.alsijil-table.horizontal-on-small tbody {
-        overflow-x: scroll;
-        display: flex;
-        column-gap: 1rem;
-        flex-wrap: nowrap;
-        align-items: stretch;
-        scroll-snap-type: x proximity;
-    }
-
-    table.alsijil-table.horizontal-on-small tr {
-        flex-basis: min(75vw, 400px);
-        flex-shrink: 0;
-        flex-grow: 1;
-        border-radius: 8px;
-        display: flex;
-        flex-direction: column;
-        justify-content: space-between;
-        scroll-snap-align: center;
-        transition: all .5s;
-        margin: 0.5rem 0 1rem 0;
-        background-color: #fff!important;
-    	box-shadow: 0 2px 2px 0 rgba(0, 0, 0, 0.14), 0 3px 1px -2px rgba(0, 0, 0, 0.12), 0 1px 5px 0 rgba(0, 0, 0, 0.2);
-        padding: 24px;
-    }
-    table.alsijil-table.horizontal-on-small tr:first-of-type {
-        margin-inline-start: .4rem;
-        -moz-margin-start: .4rem;
-        -webkit-margin-start: .4rem;
-    }
-
-    table.alsijil-table.horizontal-on-small tr:last-of-type {
-        margin-inline-end: .4rem;
-        -moz-margin-end: .4rem;
-        -webkit-margin-end: .4rem;
-    }
-    table.alsijil-table.horizontal-on-small td.center-align {
-        text-align: left;
-    }
-    table.alsijil-table.horizontal-on-small .person-name {
-        font-size: 24px;
-        font-weight: 300;
-        display: block;
-        line-height: 32px;
-        margin-bottom: 8px;
-    }
+  .no-mobile-card {
+    border: unset;
+    padding: unset;
+    margin: unset;
+    box-shadow: unset;
+  }
+  .no-mobile-card .card-content {
+    padding: unset;
+  }
+  table.alsijil-table.horizontal-on-small {
+    display: block;
+    max-width: calc(100vw - 40px);
+  }
+  table.alsijil-table.horizontal-on-small thead {
+    display: none;
+  }
+  table.alsijil-table.horizontal-on-small tbody {
+    overflow-x: scroll;
+    display: flex;
+    column-gap: 1rem;
+    flex-wrap: nowrap;
+    align-items: stretch;
+    scroll-snap-type: x proximity;
+  }
+
+  table.alsijil-table.horizontal-on-small tr {
+    flex-basis: min(75vw, 400px);
+    flex-shrink: 0;
+    flex-grow: 1;
+    border-radius: 8px;
+    display: flex;
+    flex-direction: column;
+    justify-content: space-between;
+    scroll-snap-align: center;
+    transition: all 0.5s;
+    margin: 0.5rem 0 1rem 0;
+    background-color: #fff !important;
+    box-shadow: 0 2px 2px 0 rgba(0, 0, 0, 0.14),
+      0 3px 1px -2px rgba(0, 0, 0, 0.12), 0 1px 5px 0 rgba(0, 0, 0, 0.2);
+    padding: 24px;
+  }
+  table.alsijil-table.horizontal-on-small tr:first-of-type {
+    margin-inline-start: 0.4rem;
+    -moz-margin-start: 0.4rem;
+    -webkit-margin-start: 0.4rem;
+  }
+
+  table.alsijil-table.horizontal-on-small tr:last-of-type {
+    margin-inline-end: 0.4rem;
+    -moz-margin-end: 0.4rem;
+    -webkit-margin-end: 0.4rem;
+  }
+  table.alsijil-table.horizontal-on-small td.center-align {
+    text-align: left;
+  }
+  table.alsijil-table.horizontal-on-small .person-name {
+    font-size: 24px;
+    font-weight: 300;
+    display: block;
+    line-height: 32px;
+    margin-bottom: 8px;
+  }
 }
 
-.alsijil-time-head, .alsijil-object-head {
-    display: block;
+.alsijil-time-head,
+.alsijil-object-head {
+  display: block;
 }
 
 .alsijil-time-head {
-    font-size: 2rem;
-    line-height: 1.1;
+  font-size: 2rem;
+  line-height: 1.1;
 }
 
 .alsijil-object-head {
-    font-size: 3rem;
+  font-size: 3rem;
 }
 
 @media only screen and (max-width: 600px) {
-    .alsijil-time-head {
-        font-size: 1.5rem;
-    }
-
-    .alsijil-object-head {
-        font-size: 2.2rem;
-        line-height: 1.4;
-    }
+  .alsijil-time-head {
+    font-size: 1.5rem;
+  }
+
+  .alsijil-object-head {
+    font-size: 2.2rem;
+    line-height: 1.4;
+  }
 }
 
 .alsijil-nav {
-    line-height: 36px;
+  line-height: 36px;
 }
 
 .alsijil-header-nav-button {
-    height: 66px;
-    padding: 0;
+  height: 66px;
+  padding: 0;
 }
 
 .alsijil-header-nav-button.left {
-    margin-right: 5px;
+  margin-right: 5px;
 }
 
 .alsijil-header-nav-button.right {
-    margin-left: 5px;
+  margin-left: 5px;
 }
 
 .alsijil-header-nav-button i.material-icons {
-    line-height: 60px;
-    height: 60px;
-    font-size: 40px;
+  line-height: 60px;
+  height: 60px;
+  font-size: 40px;
 }
 
 .alsijil-nav-header {
-    width: calc(100% + 40px);
-    padding: 10px 20px;
-    margin: -10px -20px 0;
-}
+  width: calc(100% + 40px);
+  padding: 10px 20px;
+  margin: -10px -20px 0;
+}
+
+.tabs-icons .tab svg.iconify {
+  display: block;
+}
```

### Comparing `AlekSIS-App-Alsijil-3.0.dev0/aleksis/apps/alsijil/static/css/alsijil/person.css` & `aleksis_app_alsijil-3.0b0/aleksis/apps/alsijil/static/css/alsijil/person.css`

 * *Files 15% similar despite different names*

```diff
@@ -1,101 +1,100 @@
 span.input-field.inline > .select-wrapper > input {
-    color: red;
-    padding: 14px 0 0 0;
-    line-height: 2px;
-    height: 36px;
-    vertical-align: middle;
+  color: red;
+  padding: 14px 0 0 0;
+  line-height: 2px;
+  height: 36px;
+  vertical-align: middle;
 }
 
 span.input-field.inline > .select-wrapper .caret {
-    top: 12px !important;
+  top: 12px !important;
 }
 
 @media screen and (min-width: 1400px) {
-    li.collection-item form {
-        margin: -30px 0 -30px 0;
-    }
-
-    li.collection-item#title #select_all_span {
-        margin-top: 5px;
-    }
+  li.collection-item form {
+    margin: -30px 0 -30px 0;
+  }
+
+  li.collection-item#title #select_all_span {
+    margin-top: 5px;
+  }
 }
 
 .collection {
-    overflow: visible;
-    overflow-x: hidden;
+  overflow: visible;
+  overflow-x: hidden;
 }
 
 #select_all_container {
-    display: none;
+  display: none;
 }
 
 #select_all_box:indeterminate + span:not(.lever):before {
-    top: -4px;
-    left: -6px;
-    width: 10px;
-    height: 12px;
-    border-top: none;
-    border-left: none;
-    border-right: white 2px solid;
-    border-bottom: none;
-    transform: rotate(90deg);
-    backface-visibility: hidden;
-    transform-origin: 100% 100%;
-
+  top: -4px;
+  left: -6px;
+  width: 10px;
+  height: 12px;
+  border-top: none;
+  border-left: none;
+  border-right: white 2px solid;
+  border-bottom: none;
+  transform: rotate(90deg);
+  backface-visibility: hidden;
+  transform-origin: 100% 100%;
 }
 
 #select_all_box:indeterminate + span:not(.lever):after {
-    top: 0;
-    width: 20px;
-    height: 20px;
-    border: 2px solid currentColor;
-    background-color: currentColor;
-    z-index: 0;
+  top: 0;
+  width: 20px;
+  height: 20px;
+  border: 2px solid currentColor;
+  background-color: currentColor;
+  z-index: 0;
 }
 
 #select_all_box_text {
-    color: #9e9e9e !important;
+  color: #9e9e9e !important;
 }
 
 td.material-icons {
-    display: table-cell;
+  display: table-cell;
 }
 
 .medium-high {
-    position: relative;
-    top: 50%;
-    left: 50%;
-    transform: translate(-50%, 50%);
+  position: relative;
+  top: 50%;
+  left: 50%;
+  transform: translate(-50%, 50%);
 }
 
 @media screen and (min-width: 600px) {
-    /* On medium and up devices */
-    .medium-high-right {
-        float: right;
-        transform: translate(0%, 50%);
-    }
+  /* On medium and up devices */
+  .medium-high-right {
+    float: right;
+    transform: translate(0%, 50%);
+  }
 }
 
 @media screen and (max-width: 600px) {
-    /* Only on small devices */
-    .full-width-s {
-        width: 100%;
-    }
-
-    #heading {
-        display: block;
-    }
-    #heading + a {
-        float: none!important;
-    }
+  /* Only on small devices */
+  .full-width-s {
+    width: 100%;
+  }
+
+  #heading {
+    display: block;
+  }
+  #heading + a {
+    float: none !important;
+  }
 }
 
 .overflow-x-scroll {
-    overflow-x: scroll;
+  overflow-x: scroll;
 }
 
 figure.modal-content figcaption {
-    font-weight: 300;
-    font-size: 2.28rem;
-    line-height: 110%;
+  font-weight: 300;
+  font-size: 2.28rem;
+  line-height: 110%;
 }
```

### Comparing `AlekSIS-App-Alsijil-3.0.dev0/aleksis/apps/alsijil/static/css/alsijil/week_view.css` & `aleksis_app_alsijil-3.0b0/aleksis/apps/alsijil/static/css/alsijil/week_view.css`

 * *Files 22% similar despite different names*

```diff
@@ -1,116 +1,118 @@
 @media screen and (max-width: 600px) {
-    #toggle-row button[type=submit] {
-        width: 100%;
-        margin-bottom: 1em;
-    }
+  #toggle-row button[type="submit"] {
+    width: 100%;
+    margin-bottom: 1em;
+  }
 }
 
 .horizontal-scroll-container {
-    overflow-x: scroll;
-    display: flex;
-    column-gap: 1rem;
-    flex-wrap: nowrap;
-    align-items: stretch;
-    scroll-snap-type: x proximity;
+  overflow-x: scroll;
+  display: flex;
+  column-gap: 1rem;
+  flex-wrap: nowrap;
+  align-items: stretch;
+  scroll-snap-type: x proximity;
 }
 
 .horizontal-scroll-container.vertical {
-    flex-wrap: wrap;
-    overflow-x: inherit;
+  flex-wrap: wrap;
+  overflow-x: inherit;
 }
 
 .horizontal-scroll-container.vertical .horizontal-scroll-card {
-    margin-inline: 0;
+  margin-inline: 0;
 }
 
 dl {
-    margin: 0;
-    padding: 0;
+  margin: 0;
+  padding: 0;
 }
 
 dt {
-    font-weight: bold;
+  font-weight: bold;
 }
 
 dd {
-    margin: 0;
-    padding: unset;
+  margin: 0;
+  padding: unset;
 }
 
 .horizontal-scroll-card {
-    flex-basis: min(75vw, 400px);
-    flex-shrink: 0;
-    flex-grow: 1;
-    border-radius: 8px;
-    display: flex;
-    flex-direction: column;
-    justify-content: space-between;
-    scroll-snap-align: center;
-    transition: all .5s;
+  flex-basis: min(75vw, 400px);
+  flex-shrink: 0;
+  flex-grow: 1;
+  border-radius: 8px;
+  display: flex;
+  flex-direction: column;
+  justify-content: space-between;
+  scroll-snap-align: center;
+  transition: all 0.5s;
 }
 
 .horizontal-scroll-card:first-of-type {
-    margin-inline-start: .4rem;
-    -moz-margin-start: .4rem;
-    -webkit-margin-start: .4rem;
+  margin-inline-start: 0.4rem;
+  -moz-margin-start: 0.4rem;
+  -webkit-margin-start: 0.4rem;
 }
 
 .horizontal-scroll-card:last-of-type {
-    margin-inline-end: .4rem;
-    -moz-margin-end: .4rem;
-    -webkit-margin-end: .4rem;
+  margin-inline-end: 0.4rem;
+  -moz-margin-end: 0.4rem;
+  -webkit-margin-end: 0.4rem;
 }
 
 .horizontal-scroll-card .card-action {
-    margin-bottom: 5px;
+  margin-bottom: 5px;
 }
 
 .horizontal-scroll-card .card-content .card-title {
-    display: flex;
-    justify-content: space-between;
+  display: flex;
+  justify-content: space-between;
 }
 
 .horizontal-scroll-card .card-content .card-title .subject {
-    flex-grow: 5;
+  flex-grow: 5;
 }
 
 .horizontal-scroll-card .one-line {
-   display: grid;
-    grid-auto-flow: column;
-    grid-template-rows: 1fr 1fr;
+  display: grid;
+  grid-auto-flow: column;
+  grid-template-rows: 1fr 1fr;
 }
 
 p.subtitle {
-    display: flex;
-    justify-content: space-between;
-    align-items: flex-end;
+  display: flex;
+  justify-content: space-between;
+  align-items: flex-end;
 }
 
 .btn-superflat ~ span {
-    line-height: 24px;
+  line-height: 24px;
 }
 
-.btn-superflat, .btn-superflat:focus, .btn-superflat:active {
-    border: none;
-    line-height: 1;
-    height: 24px;
-    background: none;
-    font-weight: normal;
+.btn-superflat,
+.btn-superflat:focus,
+.btn-superflat:active {
+  border: none;
+  line-height: 1;
+  height: 24px;
+  background: none;
+  font-weight: normal;
 }
 
 .btn-superflat i.material-icons {
-    vertical-align: middle;
+  vertical-align: middle;
 }
 
 .btn-superflat:hover {
-    cursor: pointer;
+  cursor: pointer;
 }
 
 .unfold-trigger i.material-icons {
-    transition: transform .5s 0s ease-in-out;
-    transform: rotate(-90deg);
+  transition: transform 0.5s 0s ease-in-out;
+  transform: rotate(-90deg);
 }
 
 .unfold-trigger.vertical i.material-icons {
-    transform: rotate(-180deg);
+  transform: rotate(-180deg);
 }
```

### Comparing `AlekSIS-App-Alsijil-3.0.dev0/aleksis/apps/alsijil/static/js/alsijil/week_view.js` & `aleksis_app_alsijil-3.0b0/aleksis/apps/alsijil/static/js/alsijil/week_view.js`

 * *Files 19% similar despite different names*

#### js-beautify {}

```diff
@@ -2,20 +2,19 @@
     $("#id_group").change(function() {
         $("#id_teacher").val("").formSelect();
     });
     $("#id_teacher").change(function() {
         $("#id_group").val("").formSelect();
     });
     $("#toggle-row.pre-hidden").hide();
-
 });
 $("#toggle-button").click(function() {
     $("#toggle-row").toggle();
-})
+});
 $(".unfold-trigger").click(function(event) {
     let target = event.target;
     target.classList.toggle("vertical");
     let next_container = $(target).parent().next(".horizontal-scroll-container");
     if (next_container.length >= 1) {
         next_container[0].classList.toggle("vertical");
     }
-})
+});
```

### Comparing `AlekSIS-App-Alsijil-3.0.dev0/aleksis/apps/alsijil/tables.py` & `aleksis_app_alsijil-3.0b0/aleksis/apps/alsijil/tables.py`

 * *Files 1% similar despite different names*

```diff
@@ -111,15 +111,15 @@
         verbose_name=_("Teachers"),
         accessor=A("register_object__teacher_names"),
         order_by=A("order_teachers"),
         linkify=True,
     )
     subject = tables.Column(verbose_name=_("Subject"), accessor=A("subject"), linkify=True)
     absent = tables.Column(verbose_name=_("Absent"))
-    late = tables.Column(verbose_name=_("Tardiness"))
+    tardiness = tables.Column(verbose_name=_("Tardiness"))
     excused = tables.Column(verbose_name=_("Excuse"))
     extra_marks = tables.Column(verbose_name=_("Extra marks"), accessor=A("extra_marks__all"))
 
     def render_groups(self, value, record):
         if isinstance(record.register_object, LessonPeriod):
             return record.register_object.lesson.group_names
         else:
@@ -147,17 +147,17 @@
             badge = render_to_string("components/materialize-chips.html", context)
             if record.excuse_type:
                 context = dict(content=record.excuse_type.name, classes="green white-text")
                 badge = render_to_string("components/materialize-chips.html", context)
             return badge
         return "–"
 
-    def render_late(self, value):
+    def render_tardiness(self, value):
         if value:
-            content = _(f"{value}' late")
+            content = _(f"{value}' tardiness")
             context = dict(content=content, classes="orange white-text")
             return render_to_string("components/materialize-chips.html", context)
         else:
             return "–"
 
     def render_extra_marks(self, value):
         if value:
```

### Comparing `AlekSIS-App-Alsijil-3.0.dev0/aleksis/apps/alsijil/templates/alsijil/absences/register.html` & `aleksis_app_alsijil-3.0b0/aleksis/apps/alsijil/templates/alsijil/absences/register.html`

 * *Files 18% similar despite different names*

```diff
@@ -1,25 +1,31 @@
 {# -*- engine:django -*- #}
 {% extends "core/base.html" %}
-{% load material_form i18n static %}
+{% load material_form i18n static any_js %}
 
 {% block browser_title %}{% blocktrans %}Register absence{% endblocktrans %}{% endblock %}
 {% block page_title %}{% blocktrans %}Register absence{% endblocktrans %}{% endblock %}
 
-{% block content %}
-  <h6>{% trans "Person" %}: {{ person }}</h6>
+{% block extra_head %}
+  {{ form.media.css }}
+  {% include_css "select2-materialize" %}
+{% endblock %}
 
+{% block content %}
   <form method="post">
     {% csrf_token %}
     {% form form=register_absence_form %}{% endform %}
     {% include "core/partials/save_button.html" %}
   </form>
 
   <script>
     $(document).ready(function () {
       $("#id_date_start").change(function () {
         $("#id_date_end").val($("#id_date_start").val());
         initDatePicker("#id_date_end");
       });
     });
   </script>
+
+  {% include_js "select2-materialize" %}
+  {{ form.media.js }}
 {% endblock %}
```

### Comparing `AlekSIS-App-Alsijil-3.0.dev0/aleksis/apps/alsijil/templates/alsijil/class_register/all_objects.html` & `aleksis_app_alsijil-3.0b0/aleksis/apps/alsijil/templates/alsijil/class_register/all_objects.html`

 * *Files identical despite different names*

### Comparing `AlekSIS-App-Alsijil-3.0.dev0/aleksis/apps/alsijil/templates/alsijil/class_register/groups.html` & `aleksis_app_alsijil-3.0b0/aleksis/apps/alsijil/templates/alsijil/class_register/groups.html`

 * *Files 25% similar despite different names*

```diff
@@ -27,31 +27,31 @@
         <td>
           {{ group }}
         </td>
         <td>{{ group.students_count }}</td>
         <td>
           <div class="right">
             <a class="btn primary-color waves-effect waves-light" href="{% url "students_list" group.pk %}">
-              <i class="material-icons left">people</i>
+              <i class="material-icons iconify left" data-icon="mdi:account-multiple-outline"></i>
               {% trans "Students list" %}
             </a>
             <a class="btn secondary-color waves-effect waves-light" href="{% url "week_view" "group" group.pk %}">
-              <i class="material-icons left">view_week</i>
+              <i class="material-icons iconify left" data-icon="mdi:view-week-outline"></i>
               {% trans "Week view" %}
             </a>
             {% has_perm "alsijil.view_assigned_grouproles_rule" user group as can_view_assigned_group_roles %}
             {% if can_view_assigned_group_roles %}
               <a class="btn primary waves-effect waves-light" href="{% url 'assigned_group_roles' group.pk %}">
-                <i class="material-icons left">assignment_ind</i>
+                <i class="material-icons iconify left" data-icon="mdi:clipboard-account-outline"></i>
                 {% trans "Roles" %}
               </a>
             {% endif %}
             <a class="btn primary waves-effect waves-light" href="{% url "full_register_group" group.pk %}"
                target="_blank">
-              <i class="material-icons left">print</i>
+              <i class="material-icons iconify left" data-icon="mdi:printer-outline"></i>
               {% trans "Generate printout" %}
             </a>
           </div>
         </td>
       </tr>
     {% empty %}
       <tr>
@@ -68,37 +68,37 @@
         <li class="collection-item">
           <span class="title">{{ group }}</span>
           <p>
             {{ group.students_count }} {% trans "students" %}
           </p>
           <p>
             <a class="btn primary-color waves-effect waves-light" href="{% url "week_view" "group" group.pk %}">
-              <i class="material-icons left">people</i>
+              <i class="material-icons iconify left" data-icon="mdi:account-multiple-outline"></i>
               {% trans "Students list" %}
             </a>
           </p>
           <p>
             <a class="btn secondary-color waves-effect waves-light" href="{% url "week_view" "group" group.pk %}">
-              <i class="material-icons left">view_week</i>
+              <i class="material-icons iconify left" data-icon="mdi:view-week-outline"></i>
               {% trans "Week view" %}
             </a>
           </p>
           {% has_perm "alsijil.view_assigned_grouproles_rule" user group as can_view_assigned_group_roles %}
           {% if can_view_assigned_group_roles %}
             <p>
               <a class="btn primary waves-effect waves-light" href="{% url 'assigned_group_roles' group.pk %}">
-                <i class="material-icons left">assignment_ind</i>
+                <i class="material-icons iconify left" data-icon="mdi:clipboard-account-outline"></i>
                 {% trans "Roles" %}
               </a>
             </p>
           {% endif %}
           <p>
             <a class="btn primary waves-effect waves-light" href="{% url "full_register_group" group.pk %}"
                target="_blank">
-              <i class="material-icons left">print</i>
+              <i class="material-icons iconify left" data-icon="mdi:printer-outline"></i>
               {% trans "Generate printout" %}
             </a>
           </p>
         </li>
       {% empty %}
           <li class="collection-item flow-text">
             {% blocktrans %}No groups available.{% endblocktrans %}
```

#### html2text {}

```diff
@@ -1,36 +1,36 @@
 {# -*- engine:django -*- #} {% extends "core/base.html" %} {% load i18n static
 rules %} {% block browser_title %}{% blocktrans %}My groups{% endblocktrans %}
 {% endblock %} {% block page_title %} {% blocktrans %}My groups{% endblocktrans
 %} {% endblock %} {% block extra_head %} {{ block.super }}
  {% endblock %} {% block content %}
 {% trans "Name" %} {% trans "Students"
                    %}
-                                         group.pk %}"> people {% trans
-                                        "Students list" %}
+                                         group.pk %}">  {% trans "Students
+                                        list" %}
 
-                                         "group" group.pk %}"> view_week {%
-                                        trans "Week view" %}
+                                         "group" group.pk %}">  {% trans "Week
+                                        view" %}
                    {                     {% has_perm
 {{ group }}        {                    "alsijil.view_assigned_grouproles_rule"
                    group.students_count user group as
                    }}                   can_view_assigned_group_roles %} {% if
                                         can_view_assigned_group_roles %}
-                                        assignment_ind_{%_trans_"Roles"_%} {%
-                                        endif %}
-                                         group.pk %}" target="_blank"> print {%
+                                         {%_trans_"Roles"_%}
+                                         {% endif %}
+                                         group.pk %}" target="_blank">  {%
                                         trans "Generate printout" %}
 {% blocktrans %}No groups available.{% endblocktrans %}
     * {% for group in groups %}
     * {{ group }}
       {{ group.students_count }} {% trans "students" %}
-       "group" group.pk %}"> people {% trans "Students list" %}
- "group" group.pk %}"> view_week {% trans "Week view" %}
+       "group" group.pk %}">  {% trans "Students list" %}
+ "group" group.pk %}">  {% trans "Week view" %}
 {% has_perm "alsijil.view_assigned_grouproles_rule" user group as
 can_view_assigned_group_roles %} {% if can_view_assigned_group_roles %}
-assignment_ind_{%_trans_"Roles"_%}
+ {%_trans_"Roles"_%}
 {% endif %}
- group.pk %}" target="_blank"> print {% trans "Generate printout" %}
+ group.pk %}" target="_blank">  {% trans "Generate printout" %}
 {% empty %}
 {% blocktrans %}No groups available.{% endblocktrans %}
 {% endfor %}
 {% endblock %}
```

### Comparing `AlekSIS-App-Alsijil-3.0.dev0/aleksis/apps/alsijil/templates/alsijil/class_register/person.html` & `aleksis_app_alsijil-3.0b0/aleksis/apps/alsijil/templates/alsijil/class_register/person.html`

 * *Files 8% similar despite different names*

```diff
@@ -11,26 +11,26 @@
 
 
 {% block page_title %}
   {% has_perm "alsijil.view_my_students_rule" user as has_students %}
   {% if has_students %}
     <a href="{% url "my_students" %}"
        class="btn-flat primary-color-text waves-light waves-effect">
-      <i class="material-icons left">chevron_left</i> {% trans "Back" %}
+      <i class="material-icons iconify left" data-icon="mdi:chevron-left"></i> {% trans "Back" %}
     </a>
   {% endif %}
   <span id="heading">
     {% blocktrans with person=person %}
       Class register overview for {{ person }}
     {% endblocktrans %}
   </span>
   {% has_perm "alsijil.register_absence_rule" user person as can_register_absence %}
   {% if can_register_absence %}
     <a class="btn primary-color waves-effect waves-light right" href="{% url "register_absence" person.pk %}">
-      <i class="material-icons left">rate_review</i>
+      <i class="material-icons iconify left" data-icon="mdi:message-draw"></i>
       {% trans "Register absence" %}
     </a>
   {% endif %}
 {% endblock %}
 
 {% block content %}
   <div class="row">
@@ -66,45 +66,46 @@
       <form class="modal" id="filter-modal">
         <figure class="modal-content">
           <figcaption>{% trans "Filter personal notes" %}</figcaption>
           {% form form=personal_note_filter_form %}{% endform %}
         </figure>
         <div class="modal-footer">
           <button type="button" class="btn-flat secondary-color-text waves-effect waves-ripple" id="remove-filters">
-            <i class="material-icons left">clear</i>{% trans "Clear all filters" %}
+            <i class="material-icons iconify left" data-icon="mdi:close"></i>{% trans "Clear all filters" %}
           </button>
           <button type="button" class="modal-close btn-flat red-text waves-effect waves-ripple waves-red">
-            <i class="material-icons left">cancel</i>{% trans "Close" %}
+            <i class="material-icons iconify left" data-icon="mdi:close-circle-outline"></i>{% trans "Close" %}
           </button>
           <button type="submit" class="modal-close btn-flat primary-color-text waves-effect waves-ripple waves-light">
-            <i class="material-icons left">filter_alt</i>{% trans "Filter" %}
+            <i class="material-icons iconify left" data-icon="mdi:filter-outline"></i>{% trans "Filter" %}
           </button>
         </div>
       </form>
       {% has_perm "alsijil.edit_person_overview_personalnote_rule" user person as can_mark_all_as_excused %}
       <div class="row">
         <div class="col s12 m3 l5 push-m9 push-l7">
           <button
               class="modal-trigger btn primary-color waves-effect waves-light
               {% if can_mark_all_as_excused %} medium-high-right {% endif %}"
               data-target="filter-modal"
               type="button">
-            {% trans "Filter results" %} ({{ num_filters }})<i class="material-icons right">filter_alt</i>
+            {% trans "Filter results" %} ({{ num_filters }})
+            <i class="material-icons iconify right" data-icon="mdi:filter-outline"></i>
           </button>
         </div>
         <form action="" method="post" class="">
           {% csrf_token %}
           <div class="col s12 m9 l7 pull-m3 pull-l5 row">
             {% if can_mark_all_as_excused %}
               <div class="col s12 m9">
                 {% form form=action_form %}{% endform %}
               </div>
               <div class="col s12 m3">
                 <button type="submit" class="btn waves-effect waves-light medium-high full-width-s">
-                  Run <i class="material-icons right">send</i>
+                  Run <i class="material-icons iconify right" data-icon="mdi:send-outline"></i>
                 </button>
               </div>
             {% endif %}
           </div>
           <div class="col s12 overflow-x-scroll">
             {% render_table personal_notes_table %}
           </div>
@@ -117,15 +118,15 @@
   {% if stats %}
     <div class="col s12" id="statistics">
       <h2>{% trans "Statistics on absences, tardiness and remarks" %}</h2>
       <ul class="collapsible">
         {% for school_term, stat in stats %}
           <li {% if forloop.first %}class="active"{% endif %}>
             <div class="collapsible-header">
-              <i class="material-icons">date_range</i>{{ school_term }}</div>
+              <i class="material-icons iconify" data-icon="mdi:calendar-range"></i>{{ school_term }}</div>
             <div class="collapsible-body">
               <table>
                 <tr>
                   <th colspan="3">{% trans 'Absences' %}</th>
                   <td>{{ stat.absences_count }}</td>
                 </tr>
                 <tr>
```

### Comparing `AlekSIS-App-Alsijil-3.0.dev0/aleksis/apps/alsijil/templates/alsijil/class_register/persons.html` & `aleksis_app_alsijil-3.0b0/aleksis/apps/alsijil/templates/alsijil/class_register/students_list.html`

 * *Files 20% similar despite different names*

```diff
@@ -1,145 +1,127 @@
 00000000: 7b23 202d 2a2d 2065 6e67 696e 653a 646a  {# -*- engine:dj
 00000010: 616e 676f 202d 2a2d 2023 7d0a 7b25 2065  ango -*- #}.{% e
 00000020: 7874 656e 6473 2022 636f 7265 2f62 6173  xtends "core/bas
 00000030: 652e 6874 6d6c 2220 257d 0a7b 2520 6c6f  e.html" %}.{% lo
-00000040: 6164 2069 3138 6e20 7765 656b 5f68 656c  ad i18n week_hel
-00000050: 7065 7273 2064 6174 615f 6865 6c70 6572  pers data_helper
-00000060: 7320 7374 6174 6963 2074 696d 655f 6865  s static time_he
-00000070: 6c70 6572 7320 257d 0a0a 7b25 2062 6c6f  lpers %}..{% blo
+00000040: 6164 2073 7461 7469 6320 7469 6d65 5f68  ad static time_h
+00000050: 656c 7065 7273 2064 6174 615f 6865 6c70  elpers data_help
+00000060: 6572 7320 7765 656b 5f68 656c 7065 7273  ers week_helpers
+00000070: 2069 3138 6e20 257d 0a0a 7b25 2062 6c6f   i18n %}..{% blo
 00000080: 636b 2062 726f 7773 6572 5f74 6974 6c65  ck browser_title
 00000090: 2025 7d7b 2520 626c 6f63 6b74 7261 6e73   %}{% blocktrans
-000000a0: 2025 7d4d 7920 7374 7564 656e 7473 7b25   %}My students{%
-000000b0: 2065 6e64 626c 6f63 6b74 7261 6e73 2025   endblocktrans %
-000000c0: 7d7b 2520 656e 6462 6c6f 636b 2025 7d0a  }{% endblock %}.
-000000d0: 0a0a 7b25 2062 6c6f 636b 2070 6167 655f  ..{% block page_
-000000e0: 7469 746c 6520 257d 0a20 207b 2520 626c  title %}.  {% bl
-000000f0: 6f63 6b74 7261 6e73 2025 7d4d 7920 7374  ocktrans %}My st
-00000100: 7564 656e 7473 7b25 2065 6e64 626c 6f63  udents{% endbloc
-00000110: 6b74 7261 6e73 2025 7d0a 7b25 2065 6e64  ktrans %}.{% end
-00000120: 626c 6f63 6b20 257d 0a0a 7b25 2062 6c6f  block %}..{% blo
-00000130: 636b 2065 7874 7261 5f68 6561 6420 257d  ck extra_head %}
-00000140: 0a20 207b 7b20 626c 6f63 6b2e 7375 7065  .  {{ block.supe
-00000150: 7220 7d7d 0a20 203c 6c69 6e6b 2072 656c  r }}.  <link rel
-00000160: 3d22 7374 796c 6573 6865 6574 2220 6872  ="stylesheet" hr
-00000170: 6566 3d22 7b25 2073 7461 7469 6320 2763  ef="{% static 'c
-00000180: 7373 2f61 6c73 696a 696c 2f61 6c73 696a  ss/alsijil/alsij
-00000190: 696c 2e63 7373 2720 257d 222f 3e0a 7b25  il.css' %}"/>.{%
-000001a0: 2065 6e64 626c 6f63 6b20 257d 0a0a 0a7b   endblock %}...{
-000001b0: 2520 626c 6f63 6b20 636f 6e74 656e 7420  % block content 
-000001c0: 257d 0a20 203c 756c 2063 6c61 7373 3d22  %}.  <ul class="
-000001d0: 636f 6c6c 6170 7369 626c 6522 3e0a 2020  collapsible">.  
-000001e0: 2020 7b25 2066 6f72 2067 726f 7570 2c20    {% for group, 
-000001f0: 7065 7273 6f6e 7320 696e 2067 726f 7570  persons in group
-00000200: 7320 257d 0a20 2020 2020 203c 6c69 207b  s %}.      <li {
-00000210: 2520 6966 2066 6f72 6c6f 6f70 2e66 6972  % if forloop.fir
-00000220: 7374 2025 7d63 6c61 7373 3d22 6163 7469  st %}class="acti
-00000230: 7665 227b 2520 656e 6469 6620 257d 3e0a  ve"{% endif %}>.
-00000240: 2020 2020 2020 2020 3c64 6976 2063 6c61          <div cla
-00000250: 7373 3d22 636f 6c6c 6170 7369 626c 652d  ss="collapsible-
-00000260: 6865 6164 6572 223e 0a20 2020 2020 2020  header">.       
-00000270: 2020 203c 6469 7620 636c 6173 733d 2268     <div class="h
-00000280: 756e 6472 6564 2d70 6572 6365 6e74 223e  undred-percent">
-00000290: 0a20 2020 2020 2020 2020 2020 203c 7370  .            <sp
-000002a0: 616e 2063 6c61 7373 3d22 7269 6768 7420  an class="right 
-000002b0: 7368 6f77 2d6f 6e2d 6163 7469 7665 2068  show-on-active h
-000002c0: 6964 652d 6f6e 2d73 6d61 6c6c 2d61 6e64  ide-on-small-and
-000002d0: 2d64 6f77 6e22 3e0a 2020 2020 2020 2020  -down">.        
-000002e0: 2020 2020 2020 3c61 2063 6c61 7373 3d22        <a class="
-000002f0: 6274 6e20 7072 696d 6172 792d 636f 6c6f  btn primary-colo
-00000300: 7220 7761 7665 732d 6566 6665 6374 2077  r waves-effect w
-00000310: 6176 6573 2d6c 6967 6874 2220 6872 6566  aves-light" href
-00000320: 3d22 7b25 2075 726c 2022 7765 656b 5f76  ="{% url "week_v
-00000330: 6965 7722 2022 6772 6f75 7022 2067 726f  iew" "group" gro
-00000340: 7570 2e70 6b20 257d 223e 0a20 2020 2020  up.pk %}">.     
-00000350: 2020 2020 2020 2020 2020 203c 6920 636c             <i cl
-00000360: 6173 733d 226d 6174 6572 6961 6c2d 6963  ass="material-ic
-00000370: 6f6e 7320 6c65 6674 223e 7669 6577 5f77  ons left">view_w
-00000380: 6565 6b3c 2f69 3e0a 2020 2020 2020 2020  eek</i>.        
-00000390: 2020 2020 2020 2020 7b25 2074 7261 6e73          {% trans
-000003a0: 2022 5765 656b 2076 6965 7722 2025 7d0a   "Week view" %}.
-000003b0: 2020 2020 2020 2020 2020 2020 2020 3c2f                </
-000003c0: 613e 0a20 2020 2020 2020 2020 2020 2020  a>.             
-000003d0: 203c 6120 636c 6173 733d 2262 746e 2077   <a class="btn w
-000003e0: 6176 6573 2d65 6666 6563 7420 7761 7665  aves-effect wave
-000003f0: 732d 6c69 6768 7422 2068 7265 663d 227b  s-light" href="{
-00000400: 2520 7572 6c20 2266 756c 6c5f 7265 6769  % url "full_regi
-00000410: 7374 6572 5f67 726f 7570 2220 6772 6f75  ster_group" grou
-00000420: 702e 706b 2025 7d22 2074 6172 6765 743d  p.pk %}" target=
-00000430: 225f 626c 616e 6b22 3e0a 2020 2020 2020  "_blank">.      
-00000440: 2020 2020 2020 2020 2020 3c69 2063 6c61            <i cla
-00000450: 7373 3d22 6d61 7465 7269 616c 2d69 636f  ss="material-ico
-00000460: 6e73 206c 6566 7422 3e70 7269 6e74 3c2f  ns left">print</
-00000470: 693e 0a20 2020 2020 2020 2020 2020 2020  i>.             
-00000480: 2020 207b 2520 7472 616e 7320 2247 656e     {% trans "Gen
-00000490: 6572 6174 6520 7072 696e 746f 7574 2220  erate printout" 
-000004a0: 257d 0a20 2020 2020 2020 2020 2020 2020  %}.             
-000004b0: 203c 2f61 3e0a 2020 2020 2020 2020 2020   </a>.          
-000004c0: 2020 3c2f 7370 616e 3e0a 0a20 2020 2020    </span>..     
-000004d0: 2020 2020 2020 203c 6832 3e7b 7b20 6772         <h2>{{ gr
-000004e0: 6f75 702e 6e61 6d65 207d 7d0a 2020 2020  oup.name }}.    
-000004f0: 2020 2020 2020 2020 2020 3c73 7061 6e20            <span 
-00000500: 636c 6173 733d 2263 6869 7022 3e7b 7b20  class="chip">{{ 
-00000510: 6772 6f75 702e 7363 686f 6f6c 5f74 6572  group.school_ter
-00000520: 6d20 7d7d 3c2f 7370 616e 3e0a 2020 2020  m }}</span>.    
-00000530: 2020 2020 2020 2020 3c2f 6832 3e0a 0a20          </h2>.. 
-00000540: 2020 2020 2020 2020 2020 203c 7020 636c             <p cl
-00000550: 6173 733d 2273 686f 772d 6f6e 2d61 6374  ass="show-on-act
-00000560: 6976 6520 6869 6465 2d6f 6e2d 6d65 642d  ive hide-on-med-
-00000570: 616e 642d 7570 223e 0a20 2020 2020 2020  and-up">.       
-00000580: 2020 2020 2020 203c 6120 636c 6173 733d         <a class=
-00000590: 2262 746e 2070 7269 6d61 7279 2d63 6f6c  "btn primary-col
-000005a0: 6f72 2077 6176 6573 2d65 6666 6563 7420  or waves-effect 
-000005b0: 7761 7665 732d 6c69 6768 7420 6875 6e64  waves-light hund
-000005c0: 7265 642d 7065 7263 656e 7422 0a20 2020  red-percent".   
-000005d0: 2020 2020 2020 2020 2020 2020 2020 6872                hr
-000005e0: 6566 3d22 7b25 2075 726c 2022 7765 656b  ef="{% url "week
-000005f0: 5f76 6965 7722 2022 6772 6f75 7022 2067  _view" "group" g
-00000600: 726f 7570 2e70 6b20 257d 223e 0a20 2020  roup.pk %}">.   
-00000610: 2020 2020 2020 2020 2020 2020 203c 6920               <i 
-00000620: 636c 6173 733d 226d 6174 6572 6961 6c2d  class="material-
-00000630: 6963 6f6e 7320 6c65 6674 223e 7669 6577  icons left">view
-00000640: 5f77 6565 6b3c 2f69 3e0a 2020 2020 2020  _week</i>.      
-00000650: 2020 2020 2020 2020 2020 7b25 2074 7261            {% tra
-00000660: 6e73 2022 5765 656b 2076 6965 7722 2025  ns "Week view" %
-00000670: 7d0a 2020 2020 2020 2020 2020 2020 2020  }.              
-00000680: 3c2f 613e 0a20 2020 2020 2020 2020 2020  </a>.           
-00000690: 203c 2f70 3e0a 2020 2020 2020 2020 2020   </p>.          
-000006a0: 2020 3c70 2063 6c61 7373 3d22 7368 6f77    <p class="show
-000006b0: 2d6f 6e2d 6163 7469 7665 2068 6964 652d  -on-active hide-
-000006c0: 6f6e 2d6d 6564 2d61 6e64 2d75 7022 3e0a  on-med-and-up">.
-000006d0: 2020 2020 2020 2020 2020 2020 2020 3c61                <a
-000006e0: 2063 6c61 7373 3d22 6274 6e20 7761 7665   class="btn wave
-000006f0: 732d 6566 6665 6374 2077 6176 6573 2d6c  s-effect waves-l
-00000700: 6967 6874 2068 756e 6472 6564 2d70 6572  ight hundred-per
-00000710: 6365 6e74 2220 6872 6566 3d22 7b25 2075  cent" href="{% u
-00000720: 726c 2022 6675 6c6c 5f72 6567 6973 7465  rl "full_registe
-00000730: 725f 6772 6f75 7022 2067 726f 7570 2e70  r_group" group.p
-00000740: 6b20 257d 220a 2020 2020 2020 2020 2020  k %}".          
-00000750: 2020 2020 2020 2074 6172 6765 743d 225f         target="_
-00000760: 626c 616e 6b22 3e0a 2020 2020 2020 2020  blank">.        
-00000770: 2020 2020 2020 2020 3c69 2063 6c61 7373          <i class
-00000780: 3d22 6d61 7465 7269 616c 2d69 636f 6e73  ="material-icons
-00000790: 206c 6566 7422 3e70 7269 6e74 3c2f 693e   left">print</i>
-000007a0: 0a20 2020 2020 2020 2020 2020 2020 2020  .               
-000007b0: 207b 2520 7472 616e 7320 2247 656e 6572   {% trans "Gener
-000007c0: 6174 6520 7072 696e 746f 7574 2220 257d  ate printout" %}
-000007d0: 0a20 2020 2020 2020 2020 2020 2020 203c  .              <
-000007e0: 2f61 3e0a 2020 2020 2020 2020 2020 2020  /a>.            
-000007f0: 3c2f 703e 0a20 2020 2020 2020 2020 203c  </p>.          <
-00000800: 2f64 6976 3e0a 2020 2020 2020 2020 3c2f  /div>.        </
-00000810: 6469 763e 0a0a 2020 2020 2020 2020 3c64  div>..        <d
-00000820: 6976 2063 6c61 7373 3d22 636f 6c6c 6170  iv class="collap
-00000830: 7369 626c 652d 626f 6479 223e 0a20 2020  sible-body">.   
-00000840: 2020 2020 2020 207b 2520 696e 636c 7564         {% includ
-00000850: 6520 2261 6c73 696a 696c 2f70 6172 7469  e "alsijil/parti
-00000860: 616c 732f 7065 7273 6f6e 735f 7769 7468  als/persons_with
-00000870: 5f73 7461 7473 2e68 746d 6c22 2077 6974  _stats.html" wit
-00000880: 6820 7065 7273 6f6e 733d 7065 7273 6f6e  h persons=person
-00000890: 7320 257d 0a20 2020 2020 2020 203c 2f64  s %}.        </d
-000008a0: 6976 3e0a 2020 2020 2020 3c2f 6c69 3e0a  iv>.      </li>.
-000008b0: 2020 2020 7b25 2065 6e64 666f 7220 257d      {% endfor %}
-000008c0: 0a20 203c 2f75 6c3e 0a0a 2020 7b25 2069  .  </ul>..  {% i
-000008d0: 6e63 6c75 6465 2022 616c 7369 6a69 6c2f  nclude "alsijil/
-000008e0: 7061 7274 6961 6c73 2f6c 6567 656e 642e  partials/legend.
-000008f0: 6874 6d6c 2220 257d 0a7b 2520 656e 6462  html" %}.{% endb
-00000900: 6c6f 636b 2025 7d0a                      lock %}.
+000000a0: 2077 6974 6820 6772 6f75 703d 6772 6f75   with group=grou
+000000b0: 7020 257d 5374 7564 656e 7473 206c 6973  p %}Students lis
+000000c0: 743a 207b 7b20 6772 6f75 7020 7d7d 7b25  t: {{ group }}{%
+000000d0: 2065 6e64 626c 6f63 6b74 7261 6e73 2025   endblocktrans %
+000000e0: 7d7b 2520 656e 6462 6c6f 636b 2025 7d0a  }{% endblock %}.
+000000f0: 0a7b 2520 626c 6f63 6b20 7061 6765 5f74  .{% block page_t
+00000100: 6974 6c65 2025 7d0a 2020 3c61 2068 7265  itle %}.  <a hre
+00000110: 663d 227b 2520 7572 6c20 226d 795f 6772  f="{% url "my_gr
+00000120: 6f75 7073 2220 257d 220a 2020 2020 2063  oups" %}".     c
+00000130: 6c61 7373 3d22 6274 6e2d 666c 6174 2070  lass="btn-flat p
+00000140: 7269 6d61 7279 2d63 6f6c 6f72 2d74 6578  rimary-color-tex
+00000150: 7420 7761 7665 732d 6c69 6768 7420 7761  t waves-light wa
+00000160: 7665 732d 6566 6665 6374 223e 0a20 2020  ves-effect">.   
+00000170: 203c 6920 636c 6173 733d 226d 6174 6572   <i class="mater
+00000180: 6961 6c2d 6963 6f6e 7320 6963 6f6e 6966  ial-icons iconif
+00000190: 7920 6c65 6674 2220 6461 7461 2d69 636f  y left" data-ico
+000001a0: 6e3d 226d 6469 3a63 6865 7672 6f6e 2d6c  n="mdi:chevron-l
+000001b0: 6566 7422 3e3c 2f69 3e20 7b25 2074 7261  eft"></i> {% tra
+000001c0: 6e73 2022 4261 636b 2220 257d 0a20 203c  ns "Back" %}.  <
+000001d0: 2f61 3e0a 2020 7b25 2062 6c6f 636b 7472  /a>.  {% blocktr
+000001e0: 616e 7320 7769 7468 2067 726f 7570 3d67  ans with group=g
+000001f0: 726f 7570 2025 7d53 7475 6465 6e74 7320  roup %}Students 
+00000200: 6c69 7374 3a20 7b7b 2067 726f 7570 207d  list: {{ group }
+00000210: 7d7b 2520 656e 6462 6c6f 636b 7472 616e  }{% endblocktran
+00000220: 7320 257d 0a20 203c 7370 616e 2063 6c61  s %}.  <span cla
+00000230: 7373 3d22 7269 6768 7420 7368 6f77 2d6f  ss="right show-o
+00000240: 6e2d 6163 7469 7665 2068 6964 652d 6f6e  n-active hide-on
+00000250: 2d73 6d61 6c6c 2d61 6e64 2d64 6f77 6e22  -small-and-down"
+00000260: 3e0a 2020 2020 3c61 2063 6c61 7373 3d22  >.    <a class="
+00000270: 6274 6e20 7072 696d 6172 792d 636f 6c6f  btn primary-colo
+00000280: 7220 7761 7665 732d 6566 6665 6374 2077  r waves-effect w
+00000290: 6176 6573 2d6c 6967 6874 2220 6872 6566  aves-light" href
+000002a0: 3d22 7b25 2075 726c 2022 7765 656b 5f76  ="{% url "week_v
+000002b0: 6965 7722 2022 6772 6f75 7022 2067 726f  iew" "group" gro
+000002c0: 7570 2e70 6b20 257d 223e 0a20 2020 2020  up.pk %}">.     
+000002d0: 203c 6920 636c 6173 733d 226d 6174 6572   <i class="mater
+000002e0: 6961 6c2d 6963 6f6e 7320 6963 6f6e 6966  ial-icons iconif
+000002f0: 7920 6c65 6674 2220 6461 7461 2d69 636f  y left" data-ico
+00000300: 6e3d 226d 6469 3a76 6965 772d 7765 656b  n="mdi:view-week
+00000310: 2d6f 7574 6c69 6e65 223e 3c2f 693e 0a20  -outline"></i>. 
+00000320: 2020 2020 207b 2520 7472 616e 7320 2257       {% trans "W
+00000330: 6565 6b20 7669 6577 2220 257d 0a20 2020  eek view" %}.   
+00000340: 203c 2f61 3e0a 2020 2020 3c61 2063 6c61   </a>.    <a cla
+00000350: 7373 3d22 6274 6e20 7761 7665 732d 6566  ss="btn waves-ef
+00000360: 6665 6374 2077 6176 6573 2d6c 6967 6874  fect waves-light
+00000370: 2220 6872 6566 3d22 7b25 2075 726c 2022  " href="{% url "
+00000380: 6675 6c6c 5f72 6567 6973 7465 725f 6772  full_register_gr
+00000390: 6f75 7022 2067 726f 7570 2e70 6b20 257d  oup" group.pk %}
+000003a0: 2220 7461 7267 6574 3d22 5f62 6c61 6e6b  " target="_blank
+000003b0: 223e 0a20 2020 2020 203c 6920 636c 6173  ">.      <i clas
+000003c0: 733d 226d 6174 6572 6961 6c2d 6963 6f6e  s="material-icon
+000003d0: 7320 6963 6f6e 6966 7920 6c65 6674 2220  s iconify left" 
+000003e0: 6461 7461 2d69 636f 6e3d 226d 6469 3a70  data-icon="mdi:p
+000003f0: 7269 6e74 6572 2d6f 7574 6c69 6e65 223e  rinter-outline">
+00000400: 3c2f 693e 0a20 2020 2020 207b 2520 7472  </i>.      {% tr
+00000410: 616e 7320 2247 656e 6572 6174 6520 7072  ans "Generate pr
+00000420: 696e 746f 7574 2220 257d 0a20 2020 203c  intout" %}.    <
+00000430: 2f61 3e0a 2020 3c2f 7370 616e 3e0a 7b25  /a>.  </span>.{%
+00000440: 2065 6e64 626c 6f63 6b20 257d 0a0a 7b25   endblock %}..{%
+00000450: 2062 6c6f 636b 2065 7874 7261 5f68 6561   block extra_hea
+00000460: 6420 257d 0a20 207b 7b20 626c 6f63 6b2e  d %}.  {{ block.
+00000470: 7375 7065 7220 7d7d 0a20 203c 6c69 6e6b  super }}.  <link
+00000480: 2072 656c 3d22 7374 796c 6573 6865 6574   rel="stylesheet
+00000490: 2220 6872 6566 3d22 7b25 2073 7461 7469  " href="{% stati
+000004a0: 6320 2763 7373 2f61 6c73 696a 696c 2f61  c 'css/alsijil/a
+000004b0: 6c73 696a 696c 2e63 7373 2720 257d 222f  lsijil.css' %}"/
+000004c0: 3e0a 7b25 2065 6e64 626c 6f63 6b20 257d  >.{% endblock %}
+000004d0: 0a0a 7b25 2062 6c6f 636b 2063 6f6e 7465  ..{% block conte
+000004e0: 6e74 2025 7d0a 2020 3c70 2063 6c61 7373  nt %}.  <p class
+000004f0: 3d22 7368 6f77 2d6f 6e2d 6163 7469 7665  ="show-on-active
+00000500: 2068 6964 652d 6f6e 2d6d 6564 2d61 6e64   hide-on-med-and
+00000510: 2d75 7022 3e0a 2020 2020 3c61 2063 6c61  -up">.    <a cla
+00000520: 7373 3d22 6274 6e20 7072 696d 6172 792d  ss="btn primary-
+00000530: 636f 6c6f 7220 7761 7665 732d 6566 6665  color waves-effe
+00000540: 6374 2077 6176 6573 2d6c 6967 6874 2068  ct waves-light h
+00000550: 756e 6472 6564 2d70 6572 6365 6e74 220a  undred-percent".
+00000560: 2020 2020 2020 2068 7265 663d 227b 2520         href="{% 
+00000570: 7572 6c20 2277 6565 6b5f 7669 6577 2220  url "week_view" 
+00000580: 2267 726f 7570 2220 6772 6f75 702e 706b  "group" group.pk
+00000590: 2025 7d22 3e0a 2020 2020 2020 203c 6920   %}">.       <i 
+000005a0: 636c 6173 733d 226d 6174 6572 6961 6c2d  class="material-
+000005b0: 6963 6f6e 7320 6963 6f6e 6966 7920 6c65  icons iconify le
+000005c0: 6674 2220 6461 7461 2d69 636f 6e3d 226d  ft" data-icon="m
+000005d0: 6469 3a76 6965 772d 7765 656b 2d6f 7574  di:view-week-out
+000005e0: 6c69 6e65 223e 3c2f 693e 0a20 2020 2020  line"></i>.     
+000005f0: 207b 2520 7472 616e 7320 2257 6565 6b20   {% trans "Week 
+00000600: 7669 6577 2220 257d 0a20 2020 203c 2f61  view" %}.    </a
+00000610: 3e0a 2020 3c2f 703e 0a20 203c 7020 636c  >.  </p>.  <p cl
+00000620: 6173 733d 2273 686f 772d 6f6e 2d61 6374  ass="show-on-act
+00000630: 6976 6520 6869 6465 2d6f 6e2d 6d65 642d  ive hide-on-med-
+00000640: 616e 642d 7570 223e 0a20 2020 203c 6120  and-up">.    <a 
+00000650: 636c 6173 733d 2262 746e 2077 6176 6573  class="btn waves
+00000660: 2d65 6666 6563 7420 7761 7665 732d 6c69  -effect waves-li
+00000670: 6768 7420 6875 6e64 7265 642d 7065 7263  ght hundred-perc
+00000680: 656e 7422 2068 7265 663d 227b 2520 7572  ent" href="{% ur
+00000690: 6c20 2266 756c 6c5f 7265 6769 7374 6572  l "full_register
+000006a0: 5f67 726f 7570 2220 6772 6f75 702e 706b  _group" group.pk
+000006b0: 2025 7d22 0a20 2020 2020 2020 7461 7267   %}".       targ
+000006c0: 6574 3d22 5f62 6c61 6e6b 223e 0a20 2020  et="_blank">.   
+000006d0: 2020 203c 6920 636c 6173 733d 226d 6174     <i class="mat
+000006e0: 6572 6961 6c2d 6963 6f6e 7320 6963 6f6e  erial-icons icon
+000006f0: 6966 7920 6c65 6674 2220 6461 7461 2d69  ify left" data-i
+00000700: 636f 6e3d 226d 6469 3a70 7269 6e74 6572  con="mdi:printer
+00000710: 2d6f 7574 6c69 6e65 223e 3c2f 693e 0a20  -outline"></i>. 
+00000720: 2020 2020 207b 2520 7472 616e 7320 2247       {% trans "G
+00000730: 656e 6572 6174 6520 7072 696e 746f 7574  enerate printout
+00000740: 2220 257d 0a20 2020 203c 2f61 3e0a 2020  " %}.    </a>.  
+00000750: 3c2f 703e 0a0a 2020 7b25 2069 6e63 6c75  </p>..  {% inclu
+00000760: 6465 2022 616c 7369 6a69 6c2f 7061 7274  de "alsijil/part
+00000770: 6961 6c73 2f70 6572 736f 6e73 5f77 6974  ials/persons_wit
+00000780: 685f 7374 6174 732e 6874 6d6c 2220 7769  h_stats.html" wi
+00000790: 7468 2070 6572 736f 6e73 3d70 6572 736f  th persons=perso
+000007a0: 6e73 2025 7d0a 0a20 207b 2520 696e 636c  ns %}..  {% incl
+000007b0: 7564 6520 2261 6c73 696a 696c 2f70 6172  ude "alsijil/par
+000007c0: 7469 616c 732f 6c65 6765 6e64 2e68 746d  tials/legend.htm
+000007d0: 6c22 2025 7d0a 7b25 2065 6e64 626c 6f63  l" %}.{% endbloc
+000007e0: 6b20 257d 0a                             k %}.
```

### Comparing `AlekSIS-App-Alsijil-3.0.dev0/aleksis/apps/alsijil/templates/alsijil/class_register/week_view.html` & `aleksis_app_alsijil-3.0b0/aleksis/apps/alsijil/templates/alsijil/class_register/week_view.html`

 * *Files 4% similar despite different names*

```diff
@@ -13,28 +13,28 @@
 
 {% block nav_content %}
   {% if lesson_periods %}
     <div class="">
       <ul class="tabs tabs-transparent tabs-icons tabs-fixed-width">
         <li class="tab col">
           <a class="active" href="#week-overview">
-            <i class="material-icons">speaker_notes</i>
+            <i class="material-icons iconify" data-icon="mdi:message-bulleted"></i>
             {% trans "Lesson documentations" %}
           </a>
         </li>
         <li class="tab col">
           <a href="#personal-notes">
-            <i class="material-icons">people</i>
+            <i class="material-icons iconify" data-icon="mdi:account-multiple-outline"></i>
             {% trans "Persons" %}
           </a>
         </li>
         {% if group_roles %}
           <li class="tab col">
             <a href="#group-roles">
-              <i class="material-icons">assignment_ind</i>
+              <i class="material-icons iconify" data-icon="mdi:clipboard-account-outline"></i>
               {% trans "Group roles" %}
             </a>
           </li>
         {% endif %}
       </ul>
     </div>
   {% endif %}
@@ -46,58 +46,56 @@
   <script type="text/javascript" src="{% static "js/chronos/week_select.js" %}"></script>
   <div class="row">
     <div id="toggle-row" class="col s12 m8 l10 {% if lesson_periods %}pre-hidden{% endif %}">
       <form method="post" action="">
         {% csrf_token %}
         {% form form=select_form %}{% endform %}
         <button type="submit" class="btn waves-effect waves-light primary-color">
-          <i class="material-icons left">check</i>
+          <i class="material-icons iconify left" data-icon="mdi:check"></i>
           {% blocktrans %}Select{% endblocktrans %}
         </button>
       </form>
     </div>
     <div class="col s12 m4 l2 right">
       <button type="button" class="btn waves-effect waves-light hundred-percent" id="toggle-button">
-        <i class="material-icons left">
-          filter_alt
-        </i> {% trans "Toggle filters" %}
+        <i class="material-icons iconify left" data-icon="mdi:filter-outline"></i> {% trans "Toggle filters" %}
       </button>
     </div>
   </div>
 
 
   <div class="row no-margin">
     <h4 class="col s12 m6">{% blocktrans with el=el week=week.week %}CW {{ week }}:
       {{ instance }}{% endblocktrans %} </h4>
     {% include "chronos/partials/week_select.html" with wanted_week=week %}
   </div>
 
   {% if group %}
     <p class="hide-on-med-and-down">
       <a class="btn primary-color waves-effect waves-light" href="{% url "students_list" group.pk %}">
-        <i class="material-icons left">people</i>
+        <i class="material-icons iconify left" data-icon="mdi:account-multiple-outline"></i>
         {% trans "Students list" %}
       </a>
       <a class="btn waves-effect waves-light" href="{% url "full_register_group" group.pk %}" target="_blank">
-        <i class="material-icons left">print</i>
+        <i class="material-icons iconify left" data-icon="mdi:printer-outline"></i>
         {% trans "Generate printout" %}
       </a>
     </p>
 
     <p class="hide-on-med-and-up">
       <a class="btn primary-color waves-effect waves-light hundred-percent"
          href="{% url "students_list" group.pk %}">
-        <i class="material-icons left">people</i>
+        <i class="material-icons iconify left" data-icon="mdi:account-multiple-outline"></i>
         {% trans "Students list" %}
       </a>
     </p>
     <p class="hide-on-med-and-up">
       <a class="btn waves-effect waves-light hundred-percent" href="{% url "full_register_group" group.pk %}"
          target="_blank">
-        <i class="material-icons left">print</i>
+        <i class="material-icons iconify left" data-icon="mdi:printer-outline"></i>
         {% trans "Generate printout" %}
       </a>
     </p>
   {% endif %}
 
   {% if lesson_periods %}
     <div class="row">
@@ -208,15 +206,15 @@
                   </table>
                 </div>
               </div>
               <ul class="collapsible hide-on-extra-large-only hide-on-small-only">
                 <li class="">
                   <div class="collapsible-header flow-text">
                     {{ advanced_weekday.name }}, {{ advanced_weekday.date }} <i
-                    class="material-icons collapsible-icon-right">expand_more</i>
+                    class="material-icons iconify collapsible-icon-right" data-icon="mdi:unfold-more-horizontal"></i>
                   </div>
                   <div class="collapsible-body">
                     <div class="collection">
                       {% for register_object in objects %}
                         {% has_perm "alsijil.view_lessondocumentation_rule" user register_object as can_view_lesson_documentation %}
                         {% if can_view_lesson_documentation %}
                           <a class="collection-item avatar"
@@ -286,17 +284,16 @@
                 </li>
               </ul>
               <div class="hide-on-med-and-up">
                 <h3>{{ advanced_weekday.name }}</h3>
                 <p class="subtitle">
                   <span>{{ advanced_weekday.date }}</span>
                   <button class="btn-superflat right waves-effect unfold-trigger">
-                    {% trans "Unfold" %} <i class="material-icons">
-                    expand_less
-                  </i>
+                    {% trans "Unfold" %}
+                    <i class="material-icons iconify" data-icon="mdi:unfold-less-horizontal"></i>
                   </button>
                 </p>
                 <div class="horizontal-scroll-container">
                   {% for register_object in objects %}
                     <div class="card horizontal-scroll-card">
                       <div class="card-content">
                         <span class="card-title">
@@ -377,15 +374,15 @@
             {% for person in persons %}
               <h5 class="card-title">
                 <a href="{% url "overview_person" person.person.pk %}">{{ person.person.full_name }}</a>
                 {% has_perm "alsijil.register_absence_rule" user person.person as can_register_absence %}
                 {% if can_register_absence %}
                   <a class="btn primary-color waves-effect waves-light right"
                      href="{% url "register_absence" person.person.pk %}">
-                    <i class="material-icons left">rate_review</i>
+                    <i class="material-icons iconify left" data-icon="mdi:message-draw"></i>
                     {% trans "Register absence" %}
                   </a>
                 {% endif %}
               </h5>
               {% if group_roles %}
                 <p>
                   {% for assignment in person.group_roles %}
@@ -428,15 +425,15 @@
         </div>
       {% endif %}
     </div>
   {% else %}
     <div class="card">
       <div class="card-content">
         <span class="card-title">
-          <i class="material-icons red-text left">warning</i>
+          <i class="material-icons iconify red-text left" data-icon="mdi:alert-outline"></i>
           {% blocktrans %}No lessons available{% endblocktrans %}
         </span>
         <p>
           {% blocktrans %}
             There are no lessons for the selected group or teacher in this week.
           {% endblocktrans %}
         </p>
```

#### html2text {}

```diff
@@ -1,34 +1,34 @@
 {# -*- engine:django -*- #} {% extends "core/base.html" %} {% load
 material_form i18n week_helpers static data_helpers rules time_helpers %} {%
 block browser_title %}{% blocktrans %}Week view{% endblocktrans %}{% endblock
 %} {% block extra_head %} {{ block.super }}
 
  {% endblock %} {% block nav_content %} {% if lesson_periods %}
-    * speaker_notes_{%_trans_"Lesson_documentations"_%}
-    * people_{%_trans_"Persons"_%}
+    *  {%_trans_"Lesson_documentations"_%}
+    *  {%_trans_"Persons"_%}
     * {% if group_roles %}
-    * assignment_ind_{%_trans_"Group_roles"_%}
+    *  {%_trans_"Group_roles"_%}
     * {% endif %}
 {% endif %} {% endblock %} {% block content %}
 elper.js" %}">
 {{ week_select|json_script:"week_select" }}
 hronos/week_select.js" %}">
-{% csrf_token %} {% form form=select_form %}{% endform %}  check {% blocktrans
+{% csrf_token %} {% form form=select_form %}{% endform %}   {% blocktrans
 %}Select{% endblocktrans %}
- filter_alt {% trans "Toggle filters" %}
+  {% trans "Toggle filters" %}
 *** {% blocktrans with el=el week=week.week %}CW {{ week }}: {{ instance }}{%
 endblocktrans %} ***
 {% include "chronos/partials/week_select.html" with wanted_week=week %}
 {% if group %}
- group.pk %}"> people {% trans "Students list" %}
+ group.pk %}">  {% trans "Students list" %}
 
- group.pk %}" target="_blank"> print {% trans "Generate printout" %}
- group.pk %}"> people {% trans "Students list" %}
- group.pk %}" target="_blank"> print {% trans "Generate printout" %}
+ group.pk %}" target="_blank">  {% trans "Generate printout" %}
+ group.pk %}">  {% trans "Students list" %}
+ group.pk %}" target="_blank">  {% trans "Generate printout" %}
 {% endif %} {% if lesson_periods %}
 {% for weekday, objects in regrouped_objects.items %} {% with
 weekdays|get_dict:objects.0.weekday as advanced_weekday %} {% if
 advanced_weekday.holiday and not
 request.site.preferences.alsijil__allow_entries_in_holidays %}
  {{ advanced_weekday.name }}, {{ advanced_weekday.date }} {
 { advanced_weekday.holiday }}
@@ -42,15 +42,15 @@
 {% include "alsijil/partials/   {_register_object.period.period_}}._{%_else_%}_{  {                                  register_object.get_subject.name {
 lesson_status.html" with        {_register_object.period_from_on_day_}}.â_{  register_object.lesson.group_names }}_{%_elif                       {                             {%_firstof_register_object.get_lesson_documentation.topic_"â"_{%_firstof_register_object.get_lesson_documentation.homework_"â"_{%_firstof_register_object.get_lesson_documentation.group_note_"â"_%}
 register_object=register_object {_register_object.period_to_on_day_}}._{%_endif   }}_{%_else_%}_{                    register_object.subject_%}_{     register_object.teacher_names
 %}                              %}                                                {_register_object.group_names_}}_  {_register_object.subject_}}_{%  }}
                                                                                   {%_endif_%}                        else_%}_{%_trans_"Event"_%}_({
                                                                                                                      {_register_object.title_}})_{%
                                                                                                                      endif_%}
-    * {{ advanced_weekday.name }}, {{ advanced_weekday.date }} expand_more
+    * {{ advanced_weekday.name }}, {{ advanced_weekday.date }}
       {% for register_object in objects %} {% has_perm
       "alsijil.view_lessondocumentation_rule" user register_object as
       can_view_lesson_documentation %} {% if can_view_lesson_documentation %}
       {%_include_"alsijil/partials/lesson_status.html"_with
       register_object=register_object_css_class="materialize-circle"
       color_suffix="_"_%}
                  {%_if_register_object.period_%}_{{_register_object.period.period_}}._{%
@@ -72,32 +72,32 @@
       "Homework"_{%_firstof_register_object.get_lesson_documentation.homework_"â"_%}
       %}
       {%_trans
       "Group_____{%_firstof_register_object.get_lesson_documentation.group_note_"â"_%}
       note"_%}
        {% endif %} {% endfor %}
 **** {{ advanced_weekday.name }} ****
-{{ advanced_weekday.date }}  {% trans "Unfold" %} expand_less
+{{ advanced_weekday.date }}  {% trans "Unfold" %}
 {% for register_object in objects %}
   {% if register_object.period %} {{ register_object.period.period }}. {% else
 %} {{ register_object.period_from_on_day }}.â{
 { register_object.period_to_on_day }}. {% endif %}   {% if
 register_object.get_subject %} {{ register_object.get_subject.name }} {% elif
 register_object.subject %} {{ register_object.subject }} {% else %} {% trans
 "Event" %} {% endif %}   {% include "alsijil/partials/lesson_status.html" with
 register_object=register_object %}
 {% if not group %}
 {%_trans_"Visit_lesson_overview"_%}
 {% endfor %}
 {% endif %} {% endwith %} {% endfor %}
  {% blocktrans %}Personal notes{% endblocktrans %}  {% for person in persons %}
-**  person.person.pk %}">{{ person.person.full_name }} {% has_perm
+ person.person.pk %}">{{ person.person.full_name }} {% has_perm
 "alsijil.register_absence_rule" user person.person as can_register_absence %}
-{% if can_register_absence %}  person.person.pk %}"> rate_review {% trans
-"Register absence" %} {% endif %} **
+{% if can_register_absence %}  person.person.pk %}">  {% trans "Register
+absence" %} {% endif %}
 {% if group_roles %}
 {% for assignment in person.group_roles %} {% include "alsijil/group_role/
 chip.html" with role=assignment.role small=assignment.date_range %} {% endfor
 %}
 {% endif %}
 {% trans "Absent" %}: {{ person.person.absences_count }} ({
 { person.person.unexcused_count }} {% trans "unexcused" %})
@@ -111,12 +111,12 @@
      {_note.register_object.get_subject.name_}}
 {% endfor %} {% endfor %}
 {% if group_roles %}
 {% include "alsijil/group_role/partials/assigned_roles.html" with
 roles=group_roles group=group back_url=back_url %}
 {% endif %}
 {% else %}
- warning {% blocktrans %}No lessons available{% endblocktrans %}
+  {% blocktrans %}No lessons available{% endblocktrans %}
 {% blocktrans %} There are no lessons for the selected group or teacher in this
 week. {% endblocktrans %}
 {% endif %}
  {% endblock %}
```

### Comparing `AlekSIS-App-Alsijil-3.0.dev0/aleksis/apps/alsijil/templates/alsijil/excuse_type/list.html` & `aleksis_app_alsijil-3.0b0/aleksis/apps/alsijil/templates/alsijil/excuse_type/list.html`

 * *Files 16% similar despite different names*

```diff
@@ -10,14 +10,14 @@
 
 {% block content %}
   {% include "alsijil/excuse_type/warning.html" %}
 
   {% has_perm "alsijil.add_excusetype_rule" user as add_excusetype %}
   {% if add_excusetype %}
     <a class="btn green waves-effect waves-light" href="{% url 'create_excuse_type' %}">
-      <i class="material-icons left">add</i>
+      <i class="material-icons iconify left"data-icon="mdi:plus"></i>
       {% trans "Create excuse type" %}
     </a>
   {% endif %}
 
   {% render_table table %}
 {% endblock %}
```

### Comparing `AlekSIS-App-Alsijil-3.0.dev0/aleksis/apps/alsijil/templates/alsijil/extra_mark/list.html` & `aleksis_app_alsijil-3.0b0/aleksis/apps/alsijil/templates/alsijil/extra_mark/list.html`

 * *Files 10% similar despite different names*

```diff
@@ -6,13 +6,13 @@
 {% load render_table from django_tables2 %}
 
 {% block browser_title %}{% blocktrans %}Extra marks{% endblocktrans %}{% endblock %}
 {% block page_title %}{% blocktrans %}Extra marks{% endblocktrans %}{% endblock %}
 
 {% block content %}
   <a class="btn green waves-effect waves-light" href="{% url 'create_extra_mark' %}">
-    <i class="material-icons left">add</i>
+    <i class="material-icons iconify left" data-icon="mdi:plus"></i>
     {% trans "Create extra mark" %}
   </a>
 
   {% render_table table %}
 {% endblock %}
```

### Comparing `AlekSIS-App-Alsijil-3.0.dev0/aleksis/apps/alsijil/templates/alsijil/group_role/assign.html` & `aleksis_app_alsijil-3.0b0/aleksis/apps/alsijil/templates/alsijil/group_role/assign.html`

 * *Files 7% similar despite different names*

```diff
@@ -26,15 +26,15 @@
 
 {% block content %}
   <form action="" method="post">
     {% csrf_token %}
     {% form form=form %}{% endform %}
 
     <button type="submit" class="btn green waves-effect waves-light">
-      <i class="material-icons left">assignment_ind</i>
+      <i class="material-icons iconify left" data-icon="mdi:clipboard-account-outline"></i>
       {% trans "Assign" %}
     </button>
   </form>
 
   {% include_js "select2-materialize" %}
   {{ form.media.js }}
 {% endblock %}
```

### Comparing `AlekSIS-App-Alsijil-3.0.dev0/aleksis/apps/alsijil/templates/alsijil/group_role/assigned_list.html` & `aleksis_app_alsijil-3.0b0/aleksis/apps/alsijil/templates/alsijil/group_role/assigned_list.html`

 * *Files 14% similar despite different names*

```diff
@@ -20,23 +20,23 @@
 {% block content %}
   {% url "assigned_group_roles" object.pk as back_url %}
 
   <p>
     {% has_perm "alsijil.view_my_groups_rule" user as can_view_group_overview %}
     {% if can_view_group_overview %}
       <a class="btn waves-effect waves-light" href="{% url "my_groups" %}">
-        <i class="material-icons left">arrow_back</i>
+        <i class="material-icons iconify left" data-icon="mdi:arrow-left"></i>
         {% trans "Back to my groups" %}
       </a>
     {% endif %}
 
     {% has_perm "alsijil.assign_grouprole_for_group_rule" user object as can_assign_group_role %}
     {% if can_assign_group_role %}
       <a class="btn green waves-effect waves-light" href="{% url "assign_group_role" object.pk %}">
-        <i class="material-icons left">assignment_ind</i>
+        <i class="material-icons iconify left" data-icon="mdi:clipboard-account-outline"></i>
         {% trans "Assign a role to a person" %}
       </a>
     {% endif %}
   </p>
 
   <div class="row">
     <div class="col s12">
@@ -75,15 +75,15 @@
               {{ assignment.person }}
             </td>
             <td>{{ assignment.date_start }}</td>
             <td>{{ assignment.date_end|default:"–" }}</td>
             <td>
               <a class="btn waves-effect waves-light dropdown-trigger" href="#"
                  data-target="dropdown-{{ assignment.pk }}-d2">
-                <i class="material-icons left">list</i>
+                <i class="material-icons iconify left" data-icon="mdi:format-list-bulleted"></i>
                 {% trans "Actions" %}
               </a>
               {% include "alsijil/group_role/partials/assignment_options.html" with assignment=assignment back_url=back_url suffix="-d2" %}
             </td>
           </tr>
         {% endfor %}
       </table>
```

#### html2text {}

```diff
@@ -3,27 +3,27 @@
 block browser_title %} {% blocktrans with group=object.name %}Group roles for {
 { group }}{% endblocktrans %} {% endblock %} {% block page_title %} {%
 blocktrans with group=object.name %}Group roles for {{ group }}{% endblocktrans
 %} {% endblock %} {% block extra_head %} {{ block.super }}
 lsijil/alsijil.css" %}"/> {% endblock %} {% block content %} {% url
 "assigned_group_roles" object.pk as back_url %}
 {% has_perm "alsijil.view_my_groups_rule" user as can_view_group_overview %} {%
-if can_view_group_overview %}  %}"> arrow_back {% trans "Back to my groups" %}
+if can_view_group_overview %}  %}">  {% trans "Back to my groups" %}
  {% endif %} {% has_perm "alsijil.assign_grouprole_for_group_rule" user object
 as can_assign_group_role %} {% if can_assign_group_role %}
- object.pk %}"> assignment_ind {% trans "Assign a role to a person" %}
+ object.pk %}">  {% trans "Assign a role to a person" %}
  {% endif %}
     * {%_trans_"Current_roles"_%}_({{_today|date:"SHORT_DATE_FORMAT"_}})
     * {%_trans_"All_assignments"_%}
 {% include "alsijil/group_role/partials/assigned_roles.html" with roles=roles
 group=object back_url=back_url %}
 {% trans "Group      {% trans "Person" {% trans "Start date" {% trans "End date" %}                  {% trans "Actions" %}
 role" %}             %}                %}
-                                                                                                     list_{%_trans_"Actions"
-{% include "alsijil/                                                                                 %} {% include "alsijil/
+                                                                                                      {%_trans_"Actions"_%}
+{% include "alsijil/                                                                                  {% include "alsijil/
 group_role/          {                 {                                                             group_role/partials/
 chip.html" with      {                 {                     {{ assignment.date_end|default:"â" assignment_options.html"
 role=assignment.role assignment.person assignment.date_start                                         with
 %}                   }}                }}                                                            assignment=assignment
                                                                                                      back_url=back_url
                                                                                                      suffix="-d2" %}
 {% endblock %}
```

### Comparing `AlekSIS-App-Alsijil-3.0.dev0/aleksis/apps/alsijil/templates/alsijil/group_role/list.html` & `aleksis_app_alsijil-3.0b0/aleksis/apps/alsijil/templates/alsijil/group_role/list.html`

 * *Files 17% similar despite different names*

```diff
@@ -8,15 +8,15 @@
 {% block browser_title %}{% blocktrans %}Group roles{% endblocktrans %}{% endblock %}
 {% block page_title %}{% blocktrans %}Group roles{% endblocktrans %}{% endblock %}
 
 {% block content %}
   {% has_perm "alsijil.add_grouprole_rule" user as add_group_role %}
   {% if add_group_role %}
     <a class="btn green waves-effect waves-light" href="{% url 'create_group_role' %}">
-      <i class="material-icons left">add</i>
+      <i class="material-icons iconify left" data-icon="mdi:plus"></i>
       {% trans "Create group role" %}
     </a>
   {% endif %}
 
   {% render_table table %}
 {% endblock %}
```

### Comparing `AlekSIS-App-Alsijil-3.0.dev0/aleksis/apps/alsijil/templates/alsijil/group_role/partials/assigned_roles.html` & `aleksis_app_alsijil-3.0b0/aleksis/apps/alsijil/templates/alsijil/group_role/partials/assigned_roles.html`

 * *Files 14% similar despite different names*

```diff
@@ -4,28 +4,28 @@
   {% for role in roles %}
     <div class="collection-item">
       <div class="row no-margin">
         <div class="col s12 m5 l4 xl3 no-padding">
           {% if can_assign_group_role %}
             <a class="btn waves-effect waves-light right hide-on-med-and-up"
                href="{% url "assign_group_role" group.pk role.pk %}?next={{ back_url }}">
-              <i class="material-icons center">add</i>
+              <i class="material-icons iconify center" data-icon="mdi:plus"></i>
             </a>
           {% endif %}
 
           <div class="btn-margin">
             {% include "alsijil/group_role/chip.html" with role=role %}
           </div>
         </div>
 
         <div class="col s12 m7 l8 xl9 no-padding">
           {% if can_assign_group_role %}
             <a class="btn waves-effect waves-light right hide-on-small-only"
                href="{% url "assign_group_role" group.pk role.pk %}?next={{ back_url }}">
-              <i class="material-icons center">add</i>
+              <i class="material-icons iconify center" data-icon="mdi:plus"></i>
             </a>
           {% endif %}
 
           {% for assignment in role.assignments.all %}
             {% include "alsijil/group_role/partials/assignment.html" with assignment=assignment group=group back_url=back_url %}
             {% empty %}
             <div class="grey-text darken-3">{% trans "No one assigned." %}</div>
@@ -33,13 +33,13 @@
         </div>
       </div>
     </div>
   {% endfor %}
 </div>
 
 <figure class="alert primary">
-  <i class="material-icons left">info</i>
+  <i class="material-icons iconify left" data-icon="information-outline"></i>
   {% blocktrans %}
     You can get some additional actions for each group role assignment if you click on the name of the
     corresponding person.
   {% endblocktrans %}
 </figure>
```

### Comparing `AlekSIS-App-Alsijil-3.0.dev0/aleksis/apps/alsijil/templates/alsijil/group_role/partials/assignment_options.html` & `aleksis_app_alsijil-3.0b0/aleksis/apps/alsijil/templates/alsijil/group_role/partials/assignment_options.html`

 * *Files 27% similar despite different names*

```diff
@@ -6,28 +6,28 @@
 {% has_perm "alsijil.stop_grouproleassignment_rule" user assignment as can_stop %}
 {% has_perm "alsijil.delete_grouproleassignment_rule" user assignment as can_delete %}
 
 <ul id="dropdown-{{ assignment.pk }}{{ suffix }}" class="dropdown-content">
   {% if can_edit %}
     <li>
       <a href="{% url "edit_group_role_assignment" assignment.pk %}?next={{ back_url }}">
-        <i class="material-icons left">edit</i> {% trans "Edit" %}
+        <i class="material-icons iconify left" data-icon="mdi:pencil-outline"></i> {% trans "Edit" %}
       </a>
     </li>
   {% endif %}
 
   {% if not assignment.date_end and can_stop %}
     <li>
       <a href="#">
-        <i class="material-icons left">stop</i> {% trans "Stop" %}
+        <i class="material-icons iconify left" data-icon="mdi:stop"></i> {% trans "Stop" %}
       </a>
     </li>
   {% endif %}
 
   {% if can_delete %}
     <li>
       <a href="{% url "delete_group_role_assignment" assignment.pk %}?next={{ back_url }}" class="red-text">
-        <i class="material-icons left">delete</i> {% trans "Delete" %}
+        <i class="material-icons iconify left" data-icon="mdi:delete-outline"></i> {% trans "Delete" %}
       </a>
     </li>
   {% endif %}
 </ul>
```

#### html2text {}

```diff
@@ -1,13 +1,12 @@
 {# -*- engine:django -*- #} {% load i18n rules %} {% has_perm
 "alsijil.edit_grouproleassignment_rule" user assignment as can_edit %} {%
 has_perm "alsijil.stop_grouproleassignment_rule" user assignment as can_stop %}
 {% has_perm "alsijil.delete_grouproleassignment_rule" user assignment as
 can_delete %}
     * {% if can_edit %}
-    *  assignment.pk %}?next={{ back_url }}"> edit {% trans "Edit" %}
+    *  assignment.pk %}?next={{ back_url }}">  {% trans "Edit" %}
 {% endif %} {% if not assignment.date_end and can_stop %}
-stop_{%_trans_"Stop"_%}
+ {%_trans_"Stop"_%}
 {% endif %} {% if can_delete %}
- assignment.pk %}?next={{ back_url }}" class="red-text"> delete {% trans
-"Delete" %}
+ assignment.pk %}?next={{ back_url }}" class="red-text">  {% trans "Delete" %}
 {% endif %}
```

### Comparing `AlekSIS-App-Alsijil-3.0.dev0/aleksis/apps/alsijil/templates/alsijil/partials/legend.html` & `aleksis_app_alsijil-3.0b0/aleksis/apps/alsijil/templates/alsijil/partials/legend.html`

 * *Files identical despite different names*

### Comparing `AlekSIS-App-Alsijil-3.0.dev0/aleksis/apps/alsijil/templates/alsijil/partials/lesson/prev_next.html` & `aleksis_app_alsijil-3.0b0/aleksis/apps/alsijil/templates/alsijil/partials/lesson/prev_next.html`

 * *Files 13% similar despite different names*

```diff
@@ -1,36 +1,37 @@
 {% load i18n %}
 
 <div class="row no-margin hide-on-small-only">
   <div class="col s12 no-padding">
     {% if not blocked_because_holidays and with_save %}
       {% if can_edit_lesson_documentation or can_edit_register_object_personalnote %}
         <button type="submit" class="btn waves-effect waves-light green margin-bottom">
-          <i class="material-icons left">save</i> {% trans "Save" %}
+          <i class="material-icons iconify left" data-icon="mdi:content-save-outline"></i>
+          {% trans "Save" %}
         </button>
       {% endif %}
     {% endif %}
 
     <a class="btn waves-effect waves-light primary margin-bottom {% if not prev_lesson %}disabled{% endif %}"
         {% if prev_lesson %}
        href="{% url "lesson_period" prev_lesson.week.year prev_lesson.week.week prev_lesson.id %}"
         {% endif %}
     >
-      <i class="material-icons left">arrow_back</i>
+      <i class="material-icons iconify left" data-icon="mdi:arrow-left"></i>
       {% blocktrans with subject=register_object.get_subject.short_name %}
         Previous {{ subject }} lesson
       {% endblocktrans %}
     </a>
 
     <a class="btn right waves-effect waves-light primary margin-bottom {% if not next_lesson %}disabled{% endif %}"
         {% if next_lesson %}
        href="{% url "lesson_period" next_lesson.week.year next_lesson.week.week next_lesson.id %}"
         {% endif %}
     >
-      <i class="material-icons right">arrow_forward</i>
+      <i class="material-icons iconify right" data-icon="mdi:arrow-right"></i>
       {% blocktrans with subject=register_object.get_subject.short_name %}
         Next {{ subject }} lesson
       {% endblocktrans %}
     </a>
   </div>
 </div>
```

### Comparing `AlekSIS-App-Alsijil-3.0.dev0/aleksis/apps/alsijil/templates/alsijil/partials/lesson/tabs/documentation.html` & `aleksis_app_alsijil-3.0b0/aleksis/apps/alsijil/templates/alsijil/partials/lesson/tabs/documentation.html`

 * *Files 2% similar despite different names*

```diff
@@ -1,10 +1,9 @@
 {% load i18n material_form_internal material_form %}
 
-{% include "alsijil/partials/lesson/heading.html" %}
 {% include "alsijil/partials/lesson/prev_next.html" with with_save=0 %}
 
 <div class="hide-on-med-and-up margin-bottom">
   {% if not blocked_because_holidays %}
     {% if can_edit_lesson_documentation or can_edit_register_object_personalnote %}
       {% include "core/partials/save_button.html" %}
     {% endif %}
```

#### html2text {}

```diff
@@ -1,10 +1,9 @@
 {% load i18n material_form_internal material_form %} {% include "alsijil/
-partials/lesson/heading.html" %} {% include "alsijil/partials/lesson/
-prev_next.html" with with_save=0 %}
+partials/lesson/prev_next.html" with with_save=0 %}
 {% if not blocked_because_holidays %} {% if can_edit_lesson_documentation or
 can_edit_register_object_personalnote %} {% include "core/partials/
 save_button.html" %} {% endif %} {% endif %}
  {% blocktrans %}Lesson documentation{% endblocktrans %}  {% if
 can_edit_lesson_documentation %} {% form form=lesson_documentation_form %}{%
 endform %} {% elif can_view_lesson_documentation %}
 {% trans "Lesson topic" %} {{ lesson_documentation.topic }}
```

### Comparing `AlekSIS-App-Alsijil-3.0.dev0/aleksis/apps/alsijil/templates/alsijil/partials/lesson/tabs/notes.html` & `aleksis_app_alsijil-3.0b0/aleksis/apps/alsijil/templates/alsijil/partials/lesson/tabs/notes.html`

 * *Files 12% similar despite different names*

```diff
@@ -1,17 +1,16 @@
 {% load i18n material_form_internal material_form time_helpers %}
 
-{% include "alsijil/partials/lesson/heading.html" %}
 {% include "alsijil/partials/lesson/prev_next.html" with with_save=1 %}
 
 {% if not blocked_because_holidays %}
   {% if can_edit_lesson_documentation or can_edit_register_object_personalnote %}
     <button type="submit"
             class="btn waves-effect waves-light green margin-bottom hundred-percent hide-on-med-and-up">
-      <i class="material-icons left">save</i> {% trans "Save" %}
+      <i class="material-icons iconify left" data-icon="mdi:content-save-outline"></i> {% trans "Save" %}
     </button>
   {% endif %}
 {% endif %}
 
 {% if can_edit_register_object_personalnote %}
   {% form form=personal_note_formset.management_form %}{% endform %}
 {% endif %}
@@ -50,15 +49,15 @@
               <label>
                 {{ form.absent }}
                 <span><span class="hide-on-large-only">{{ form.absent.label }}</span></span>
               </label>
             </td>
             <td>
               <div class="input-field">
-                {{ form.late }}
+                {{ form.tardiness }}
                 <label for="{{ form.absent.id_for_label }}">
                   {% trans "Tardiness (in m)" %}
                 </label>
               </div>
             </td>
             <td class="center-align">
               <label>
@@ -101,22 +100,26 @@
             <td>{{ form.person_name.value }}
               <p>
                 {% for assignment in form.instance.person.group_roles.all %}
                   {% include "alsijil/group_role/chip.html" with role=assignment.role %}
                 {% endfor %}
               </p>
             </td>
-            <td><i class="material-icons center">{{ form.absent.value|yesno:"check,clear" }}</i></td>
             <td>
-              <i class="material-icons center">{{ form.late.value|yesno:"check,clear" }}</i>
+              <i class="material-icons iconify center" data-icon="mdi:{{ form.absent.value|yesno:"check,close" }}"></i>
+            </td>
+            <td>
+              <i class="material-icons iconify center" data-icon="mdi:{{ form.tardiness.value|yesno:"check,close" }}"></i>
               <span class="alsijil-tardiness-text">
-                {% if form.late.value %}{{ form.late.value|to_time|time:"i\m" }}{% endif %}
+                {% if form.tardiness.value %}{{ form.tardiness.value|to_time|time:"i\m" }}{% endif %}
               </span>
             </td>
-            <td><i class="material-icons center">{{ form.excused.value|yesno:"check,clear" }}</i></td>
+            <td>
+              <i class="material-icons iconify center" data-icon="mdi:{{ form.excused.value|yesno:"check,close" }}"></i>
+              </td>
             <td>{% firstof form.instance.excuse_type "–" %}</td>
             <td>
               {% for extra_mark in form.instance.extra_marks.all %}
                 {{ extra_mark }}{% if not forloop.last %},{% endif %}
               {% empty %}
                 –
               {% endfor %}
@@ -129,11 +132,11 @@
     </table>
   </div>
 </div>
 {% if not blocked_because_holidays %}
   {% if can_edit_lesson_documentation or can_edit_register_object_personalnote %}
     <button type="submit"
             class="btn waves-effect waves-light green margin-bottom hundred-percent hide-on-med-and-up">
-      <i class="material-icons left">save</i> {% trans "Save" %}
+      <i class="material-icons iconify left" data-icon="mdi:content-save-outline"></i> {% trans "Save" %}
     </button>
   {% endif %}
 {% endif %}
```

#### html2text {}

```diff
@@ -1,26 +1,26 @@
 {% load i18n material_form_internal material_form time_helpers %} {% include
-"alsijil/partials/lesson/heading.html" %} {% include "alsijil/partials/lesson/
-prev_next.html" with with_save=1 %} {% if not blocked_because_holidays %} {% if
-can_edit_lesson_documentation or can_edit_register_object_personalnote %}  save
-{% trans "Save" %}  {% endif %} {% endif %} {% if
-can_edit_register_object_personalnote %} {% form
+"alsijil/partials/lesson/prev_next.html" with with_save=1 %} {% if not
+blocked_because_holidays %} {% if can_edit_lesson_documentation or
+can_edit_register_object_personalnote %}   {% trans "Save" %}  {% endif %} {%
+endif %} {% if can_edit_register_object_personalnote %} {% form
 form=personal_note_formset.management_form %}{% endform %} {% endif %}
  {% blocktrans %}Personal notes{% endblocktrans %}
-{% blocktrans %}Person{%             {% blocktrans %}Absent{% {% blocktrans %}Tardiness{%   {% blocktrans %}Excused{% {% blocktrans %}Excuse type{% endblocktrans   {% blocktrans %}Extra marks{% endblocktrans %}                          {% blocktrans %}Remarks{%
-endblocktrans %}                     endblocktrans %}         endblocktrans %}              endblocktrans %}          %}                                                                                                                    endblocktrans %}
-{{ form.person_name }}{                                                                                                                                             {% for group, items in form.extra_marks|select_options %} {% for
-{ form.person_name.value }}                                                                                                                                         choice, value, selected in items %}
-{% for assignment in                  {{ form.absent }} {     {{ form.late }}  {% trans      {{ form.excused }} {     {{ form.excuse_type }}  {% trans "Excuse      % if value == None or value == '' %}disabled{% else %}value="{{ value   {{ form.remarks }}  {% trans "Remarks"
-form.instance.person.group_roles.all { form.absent.label }}   "Tardiness (in m)" %}         { form.excused.label }}   type" %}                                      }}"{% endif %} {% if selected %} checked="checked"{% endif %} name="{   %}
-%} {% include "alsijil/group_role/                                                                                                                                  { form.extra_marks.html_name }}"> {{ choice }}  {% endfor %} {% endfor
-chip.html" with role=assignment.role                                                                                                                                %}
+{% blocktrans %}Person{%             {% blocktrans     {% blocktrans %}Tardiness{%        {% blocktrans      {% blocktrans %}Excuse type{% endblocktrans                                                                           {% blocktrans %}Remarks{%
+endblocktrans %}                     %}Absent{%        endblocktrans %}                   %}Excused{%        %}                                            {% blocktrans %}Extra marks{% endblocktrans %}                          endblocktrans %}
+                                     endblocktrans %}                                     endblocktrans %}
+{{ form.person_name }}{                                                                                                                                    {% for group, items in form.extra_marks|select_options %} {% for
+{ form.person_name.value }}           {{ form.absent                                       {{ form.excused                                                 choice, value, selected in items %}
+{% for assignment in                 }} {              {{ form.tardiness }}  {% trans     }} {               {{ form.excuse_type }}  {% trans "Excuse      % if value == None or value == '' %}disabled{% else %}value="{{ value   {{ form.remarks }}  {% trans "Remarks"
+form.instance.person.group_roles.all {                 "Tardiness (in m)" %}              {                  type" %}                                      }}"{% endif %} {% if selected %} checked="checked"{% endif %} name="{   %}
+%} {% include "alsijil/group_role/   form.absent.label                                    form.excused.label                                               { form.extra_marks.html_name }}"> {{ choice }}  {% endfor %} {% endfor
+chip.html" with role=assignment.role }}                                                   }}                                                               %}
+%} {% endfor %}
+{{ form.person_name.value }}                           close" }}">
+{% for assignment in                                     {% if form.tardiness.value %}{
+form.instance.person.group_roles.all close" }}">       {                                  close" }}">        {% firstof form.instance.excuse_type "â" {% for extra_mark in form.instance.extra_marks.all %} {{ extra_mark }}  {% firstof form.remarks.value "â" %}
+%} {% include "alsijil/group_role/                     form.tardiness.value|to_time|time:                                                                  {% if not forloop.last %},{% endif %} {% empty %} â {% endfor %}
+chip.html" with role=assignment.role                   "i\m" }}{% endif %}
 %} {% endfor %}
-{{ form.person_name.value }}                                  {{ form.late.value|yesno:
-{% for assignment in                 {                        "check,clear" }}  {% if       {
-form.instance.person.group_roles.all {                        form.late.value %}{           {                         {% firstof form.instance.excuse_type "â" {% for extra_mark in form.instance.extra_marks.all %} {{ extra_mark }}  {% firstof form.remarks.value "â" %}
-%} {% include "alsijil/group_role/   form.absent.value|yesno: {                             form.excused.value|yesno:                                               {% if not forloop.last %},{% endif %} {% empty %} â {% endfor %}
-chip.html" with role=assignment.role "check,clear" }}         form.late.value|to_time|time: "check,clear" }}
-%} {% endfor %}                                               "i\m" }}{% endif %}
 {% if not blocked_because_holidays %} {% if can_edit_lesson_documentation or
-can_edit_register_object_personalnote %}  save {% trans "Save" %}  {% endif %}
-{% endif %}
+can_edit_register_object_personalnote %}   {% trans "Save" %}  {% endif %} {%
+endif %}
```

### Comparing `AlekSIS-App-Alsijil-3.0.dev0/aleksis/apps/alsijil/templates/alsijil/partials/lesson/tabs/previous_lesson.html` & `aleksis_app_alsijil-3.0b0/aleksis/apps/alsijil/templates/alsijil/partials/lesson/tabs/previous_lesson.html`

 * *Files identical despite different names*

### Comparing `AlekSIS-App-Alsijil-3.0.dev0/aleksis/apps/alsijil/templates/alsijil/partials/lesson/tabs/seating_plan.html` & `aleksis_app_alsijil-3.0b0/aleksis/apps/alsijil/templates/alsijil/partials/lesson/tabs/seating_plan.html`

 * *Files 13% similar despite different names*

```diff
@@ -6,15 +6,15 @@
     <div class="card-content">
       <div class="card-title margin-bottom">
         {% blocktrans with group=seating_plan.group room=seating_plan.room %}Seating plan for {{ group }} in
           {{ room }}{% endblocktrans %}
       </div>
       {% if seating_plan_parent %}
         <figure class="alert primary">
-          <i class="material-icons left">info</i>
+          <i class="material-icons iconify left" data-icon="information-outline"></i>
           {% blocktrans with child_group=first_group %}
             This seating plan is taken from the parent group of {{ child_group }}.
             If you want, you can take it over for your group and then customize it.
           {% endblocktrans %}
         </figure>
       {% endif %}
 
@@ -22,22 +22,22 @@
         <div class="col s12 no-padding">
           {% has_perm "stoelindeling.edit_seatingplan_rule" user seating_plan as can_edit %}
           {% has_perm "stoelindeling.copy_seatingplan_for_group_rule" user first_group as can_copy %}
 
           {% if can_edit %}
             <a class="btn orange waves-effect waves-light"
                href="{% url "edit_seating_plan" seating_plan.pk %}?next={{ back_url }}#seating-plan">
-              <i class="material-icons left">edit</i>
+              <i class="material-icons iconify left" data-icon="mdi:pencil-outline"></i>
               {% trans "Edit seating plan" %}
             </a>
           {% endif %}
           {% if can_copy and seating_plan_parent %}
             <a class="btn orange waves-effect waves-light"
                href="{% url "copy_seating_plan" seating_plan.pk %}?next={{ back_url }}#seating-plan">
-              <i class="material-icons left">content_copy</i>
+              <i class="material-icons iconify left" data-icon="mdi:content-copy"></i>
               {% trans "Copy plan and edit" %}
             </a>
           {% endif %}
         </div>
       </div>
 
       <div class="row">
@@ -48,37 +48,37 @@
     </div>
   </div>
 {% else %}
   <div class="container">
     <div class="card">
       <div class="card-content">
         <div class="card-title">
-          <i class="material-icons left small orange-text">warning</i>
+          <i class="material-icons iconify left small orange-text" data-icon="mdi:alert-outline"></i>
           {% trans "There is no seating plan for this lesson." %}
         </div>
-        {% has_perm "stoelindeling.add_seatingplan_rule" user first_group as can_add %}
+        {% has_perm "stoelindeling.create_seatingplan_rule" user first_group as can_add %}
         {% if can_add %}
           <div class="row margin-bottom">
             <div class="col s12">
               <a class="btn waves-effect waves-light" href="{% url "create_seating_plan" %}?group={{ first_group.pk }}&subject={{ register_object.get_subject.pk }}&room={{ register_object.get_room.pk }}&next={{ back_url }}#seating-plan">
-                <i class="material-icons left">add</i>
+                <i class="material-icons iconify left" data-icon="mdi:plus"></i>
                 {% blocktrans with group=first_group.name subject=register_object.get_subject.name room=register_object.get_room.name %}
                   Create a new seating plan for {{ group }} ({{ subject }}) in {{ room }}
                 {% endblocktrans %}
               </a>
             </div>
           </div>
         {% endif %}
         {% for parent_group in first_group.parent_groups.all %}
-          {% has_perm "stoelindeling.add_seatingplan_rule" user parent_group as can_add %}
+          {% has_perm "stoelindeling.create_seatingplan_rule" user parent_group as can_add %}
           {% if can_add %}
             <div class="row">
               <div class="col s12">
                 <a class="btn waves-effect waves-light" href="{% url "create_seating_plan" %}?group={{ parent_group.pk }}&subject={{ register_object.get_subject.pk }}&room={{ register_object.get_room.pk }}&next={{ back_url }}#seating-plan">
-                  <i class="material-icons left">add</i>
+                  <i class="material-icons iconify left" data-icon="mdi:plus"></i>
                   {% blocktrans with group=parent_group.name room=register_object.get_room.name %}
                     Create a new seating plan for {{ group }} in {{ room }}
                   {% endblocktrans %}
                 </a>
               </div>
             </div>
           {% endif %}
```

### Comparing `AlekSIS-App-Alsijil-3.0.dev0/aleksis/apps/alsijil/templates/alsijil/partials/lesson_status.html` & `aleksis_app_alsijil-3.0b0/aleksis/apps/alsijil/templates/alsijil/partials/lesson_status.html`

 * *Files 4% similar despite different names*

```diff
@@ -1,36 +1,36 @@
 {% load i18n week_helpers %}
 
 {% now_datetime as now_dt %}
 
 {% if has_documentation or register_object.has_documentation %}
-  {% include "alsijil/partials/lesson_status_icon.html" with text=_("Data complete") icon="check_circle" color="green" %}
+  {% include "alsijil/partials/lesson_status_icon.html" with text=_("Data complete") icon="mdi:check-circle-outline" color="green" %}
 {% elif not register_object.period %}
   {% if week %}
     {% period_to_time_start week register_object.raw_period_from_on_day as time_start %}
     {% period_to_time_end week register_object.raw_period_to_on_day as time_end %}
   {% else %}
     {% period_to_time_start register_object.date_start register_object.period_from as time_start %}
     {% period_to_time_end register_object.date_end register_object.period_to as time_end %}
   {% endif %}
 
   {% if now_dt > time_end %}
-    {% include "alsijil/partials/lesson_status_icon.html" with text=_("Missing data") icon="warning" color="red" %}
+    {% include "alsijil/partials/lesson_status_icon.html" with text=_("Missing data") icon="mdi:alert-outline" color="red" %}
   {% elif now_dt > time_start and now_dt < time_end %}
-    {% include "alsijil/partials/lesson_status_icon.html" with text=_("Pending") icon="more_horiz" color="orange" %}
+    {% include "alsijil/partials/lesson_status_icon.html" with text=_("Pending") icon="mdi:dots-horizontal" color="orange" %}
   {% else %}
-    {% include "alsijil/partials/lesson_status_icon.html" with text=_("Event") icon="event" color="purple" %}
+    {% include "alsijil/partials/lesson_status_icon.html" with text=_("Event") icon="mdi:calendar" color="purple" %}
   {% endif %}
 {% else %}
   {% period_to_time_start week register_object.period as time_start %}
   {% period_to_time_end week register_object.period as time_end %}
 
   {% if substitution.cancelled or register_object.get_substitution.cancelled %}
-    {% include "alsijil/partials/lesson_status_icon.html" with text=_("Lesson cancelled") icon="cancel" color="red" %}
+    {% include "alsijil/partials/lesson_status_icon.html" with text=_("Lesson cancelled") icon="mdi:close" color="red" %}
   {% elif now_dt > time_end %}
-    {% include "alsijil/partials/lesson_status_icon.html" with text=_("Missing data") icon="warning" color="red" %}
+    {% include "alsijil/partials/lesson_status_icon.html" with text=_("Missing data") icon="mdi:alert-outline" color="red" %}
   {% elif now_dt > time_start and now_dt < time_end %}
-    {% include "alsijil/partials/lesson_status_icon.html" with text=_("Pending") icon="more_horiz" color="orange" %}
+    {% include "alsijil/partials/lesson_status_icon.html" with text=_("Pending") icon="mdi:dots-horizontal" color="orange" %}
   {% elif substitution or register_object.get_substitution %}
-    {% include "alsijil/partials/lesson_status_icon.html" with text=_("Substitution") icon="update" color="orange" %}
+    {% include "alsijil/partials/lesson_status_icon.html" with text=_("Substitution") icon="mdi:update" color="orange" %}
   {% endif %}
 {% endif %}
```

### Comparing `AlekSIS-App-Alsijil-3.0.dev0/aleksis/apps/alsijil/templates/alsijil/partials/objects_table.html` & `aleksis_app_alsijil-3.0b0/aleksis/apps/alsijil/templates/alsijil/partials/objects_table.html`

 * *Files 11% similar despite different names*

```diff
@@ -1,15 +1,15 @@
 {% load i18n material_form django_tables2 %}
 <div class="card">
   <div class="card-content">
     <div class="card-title">{% trans "Lesson filter" %}</div>
     <form action="" method="get">
       {% form form=filter_form %}{% endform %}
       <button type="submit" class="btn waves-effect waves-light">
-        <i class="material-icons left">refresh</i>
+        <i class="material-icons iconify left" data-icon="mdi:refresh"></i>
         {% trans "Update filters" %}
       </button>
     </form>
   </div>
 </div>
 
 {% if table %}
@@ -25,15 +25,15 @@
             <div class="col s12 m8 l8 xl6">
               <div class="col s12 m8">
                 {% form form=action_form %}{% endform %}
               </div>
               <div class="col s12 m4">
                 <button type="submit" class="btn waves-effect waves-primary">
                   {% trans "Execute" %}
-                  <i class="material-icons right">send</i>
+                  <i class="material-icons iconify right" data-icon="mdi:send-outline"></i>
                 </button>
               </div>
             </div>
           {% endif %}
         </div>
         {% render_table table %}
```

### Comparing `AlekSIS-App-Alsijil-3.0.dev0/aleksis/apps/alsijil/templates/alsijil/partials/persons_with_stats.html` & `aleksis_app_alsijil-3.0b0/aleksis/apps/alsijil/templates/alsijil/partials/persons_with_stats.html`

 * *Files 12% similar despite different names*

```diff
@@ -1,12 +1,12 @@
 {% load data_helpers time_helpers i18n rules %}
 
 {% if not persons %}
   <figure class="alert primary">
-    <i class="material-icons left">warning</i>
+    <i class="material-icons iconify left" data-icon="mdi:alert-outline"></i>
     {% blocktrans %}No students available.{% endblocktrans %}
   </figure>
 {% else %}
   <table class="highlight responsive-table">
   <thead>
   <tr class="hide-on-med-and-down">
     <th rowspan="2">{% trans "Name" %}</th>
@@ -122,23 +122,23 @@
             {{ person|get_dict:extra_mark.count_label }}
           </span>
         </td>
       {% endfor %}
 
       <td>
         <a class="btn primary waves-effect waves-light" href="{% url "overview_person" person.pk %}">
-          <i class="material-icons left">insert_chart</i>
+          <i class="material-icons iconify left" data-icon="mdi:chart-box-outline"></i>
           <span class="hide-on-med-and-down"> {% trans "Show more details" %}</span>
           <span class="hide-on-large-only">{% trans "Details" %}</span>
         </a>
 
         {% has_perm "alsijil.register_absence_rule" user person as can_register_absence %}
         {% if can_register_absence %}
           <a class="btn primary-color waves-effect waves-light" href="{% url "register_absence" person.pk %}">
-            <i class="material-icons left">rate_review</i>
+            <i class="material-icons iconify left" data-icon="mdi:message-draw"></i>
             {% trans "Register absence" %}
           </a>
         {% endif %}
       </td>
     </tr>
   {% endfor %}
 {% endif %}
```

#### html2text {}

```diff
@@ -1,23 +1,23 @@
-{% load data_helpers time_helpers i18n rules %} {% if not persons %}  warning
-{% blocktrans %}No students available.{% endblocktrans %}  {% else %}
+{% load data_helpers time_helpers i18n rules %} {% if not persons %}   {%
+blocktrans %}No students available.{% endblocktrans %}  {% else %}
                                                     {% trans "Absences"   {% trans "Uncounted                                       {% trans "Extra marks"
                                                     %}                    Absences" %}                                              %}
 {% trans   {% trans "Primary group" %}                                                           {% trans "Tardiness" %}                                                                                                                                                        ({                                                     ({                     {% trans    {
 "Name" %}                                           {% trans "Name" %}    {% trans "Primary                                         {% trans "Absences" %}                        {% trans "Sum (e)" %}   {% trans "(e)" %}                                                     {                      {% trans "(u)" %}               {                      "Tardiness" {
                                                                           group" %}                                                                                                                                                                                             excuse_type.short_name                                 excuse_type.short_name %}          extra_mark.short_name
                                                                                                                                                                                                                                                                                 }})                                                    }})                                }}
                                                                           ({                                                        ({                      {
 {% trans   {% trans "Sum (e)" %}                    {% trans "(e)" %}     {                      {% trans "(u)" %}                  {                       {
 "Sum" %}                                                                  excuse_type.short_name                                    excuse_type.short_name  extra_mark.short_name
                                                                           }})                                                       }})                     }}
-                                                                                                                                                                                                                                                                                                        person.pk %}"> insert_chart
-                                                                                                                                                                                                                                                                                                       {% trans "Show more details" %}
-                                                                                                                                                                                                                                                                                                       {% trans "Details" %}
+                                                                                                                                                                                                                                                                                                        person.pk %}">   {% trans
+                                                                                                                                                                                                                                                                                                       "Show more details" %} {% trans
+                                                                                                                                                                                                                                                                                                       "Details" %}
  person.pk                                           %}"> {                                       %}"> {                                                                                                                                                                                                {% has_perm
 %}"> {                                              {                      %}"> {                {                                   {{ person|get_dict:     %}"> {                {{ person|get_dict:     %}"> {% firstof person.tardiness|to_time|time:"H\h i\m" "â" %}   {{ person|get_dict:   "alsijil.register_absence_rule"
 { person   {% firstof person.primary_group "â" person.absences_count { person.excused }}    person.excused_without_excuse_type excuse_type.count_label { person.unexcused }} excuse_type.count_label  %}">{{ person.tardiness_count }} ×                                  extra_mark.count_label user person as
 }}                                                  }}                                           }}                                 }}                                            }}                                                                                            }}                     can_register_absence %} {% if
                                                                                                                                                                                                                                                                                                        can_register_absence %}
-                                                                                                                                                                                                                                                                                                        person.pk %}"> rate_review {%
-                                                                                                                                                                                                                                                                                                       trans "Register absence" %}
+                                                                                                                                                                                                                                                                                                        person.pk %}">  {% trans
+                                                                                                                                                                                                                                                                                                       "Register absence" %}
                                                                                                                                                                                                                                                                                                         {% endif %}
```

### Comparing `AlekSIS-App-Alsijil-3.0.dev0/aleksis/apps/alsijil/templates/alsijil/print/full_register.html` & `aleksis_app_alsijil-3.0b0/aleksis/apps/alsijil/templates/alsijil/print/full_register.html`

 * *Files 3% similar despite different names*

```diff
@@ -13,16 +13,16 @@
 {% block content %}
 
   <div class="center-align">
     <h1>{% trans 'Class register' %}</h1>
     <h5>{{ school_term }}</h5>
     <p>({{ school_term.date_start }}–{{ school_term.date_end }})</p>
     {% static "img/aleksis-banner.svg" as aleksis_banner %}
-    <img src="{% firstof request.site.preferences.theme__logo.url aleksis_banner %}"
-         alt="{{ request.site.preferences.general__title }} – Logo" class="max-size-600 center">
+    <img src="{% firstof SITE_PREFERENCES.theme__logo.url aleksis_banner %}"
+         alt="{{ SITE_PREFERENCES.general__title }} – Logo" class="max-size-600 center">
     <h4 id="group-desc">
       {{ group.name }}
     </h4>
     <p id="group-owners" class="flow-text">
       {% trans 'Owners' %}:
       {{ group.owners.all|join:', ' }}
     </p>
@@ -252,37 +252,37 @@
         <td rowspan="6" class="person-img">
           {% if person.photo %}
             <img src="{{ person.photo.url }}" alt="{{ person.first_name }} {{ person.last_name }}"/>
           {% else %}
             <img src="{% static 'img/fallback.png' %}" alt="{{ person.first_name }} {{ person.last_name }}"/>
           {% endif %}
         </td>
-        <td><i class="material-icons">person</i></td>
+        <td><i class="material-icons iconify" data-icon="mdi:account-outline"></i></td>
         <td colspan="2">{{ person.first_name }} {{ person.additional_name }} {{ person.last_name }}</td>
       </tr>
       <tr>
-        <td><i class="material-icons">face</i></td>
+        <td><i class="material-icons iconify" data-icon="mdi:human-non-binary"></i></td>
         <td colspan="2">{{ person.get_sex_display }}</td>
       </tr>
       <tr>
-        <td><i class="material-icons">home</i></td>
+        <td><i class="material-icons iconify" data-icon="mdi:map-marker-outline"></i></td>
         <td>{{ person.street }} {{ person.housenumber }}</td>
         <td>{{ person.postal_code }} {{ person.place }}</td>
       </tr>
       <tr>
-        <td><i class="material-icons">phone</i></td>
+        <td><i class="material-icons iconify" data-icon="mdi:phone-outline"></i></td>
         <td>{{ person.phone_number }}</td>
         <td>{{ person.mobile_number }}</td>
       </tr>
       <tr>
-        <td><i class="material-icons">email</i></td>
+        <td><i class="material-icons iconify" data-icon="mdi:email-outline"></i></td>
         <td colspan="2">{{ person.email }}</td>
       </tr>
       <tr>
-        <td><i class="material-icons">cake</i></td>
+        <td><i class="material-icons iconify" data-icon="mdi:cake"></i></td>
         <td colspan="2">{{ person.date_of_birth|date }}</td>
       </tr>
     </table>
 
     <div class="row">
       <div class="col s6">
         <h5>{% trans 'Absences and tardiness' %}</h5>
@@ -353,15 +353,15 @@
         <th>{% trans 'Tard.' %}</th>
         <th colspan="2">{% trans 'Remarks' %}</th>
       </tr>
       </thead>
 
       <tbody>
       {% for note in person.filtered_notes %}
-        {% if note.absent or note.late or note.remarks or note.extra_marks.all %}
+        {% if note.absent or note.tardiness or note.remarks or note.extra_marks.all %}
           <tr>
             {% if note.date %}
               <td>{{ note.date }}</td>
               <td>{{ note.register_object.period.period }}</td>
             {% else %}
               <td colspan="2">
                 {{ note.register_object.date_start }} {{ note.register_object.period_from.period }}.–{{ note.register_object.date_end }}
@@ -385,16 +385,16 @@
                   {% else %}
                     ({% trans 'e' %})
                   {% endif %}
                 {% endif %}
               {% endif %}
             </td>
             <td>
-              {% if note.late %}
-                {{ note.late }}'
+              {% if note.tardiness %}
+                {{ note.tardiness }}'
               {% endif %}
             </td>
             <td>
               {% for extra_mark in note.extra_marks.all %}
                 {{ extra_mark.short_name }}{% if not forloop.last %},{% endif %}
               {% endfor %}
             </td>
@@ -482,18 +482,18 @@
                           {% else %}
                             ({% trans 'e' %})
                           {% endif %}
                         </span>
                       {% endif %}
                     </span>
                   {% endif %}
-                  {% if note.late %}
+                  {% if note.tardiness %}
                     <span class="lesson-note-late">
                       {{ note.person.last_name }}, {{ note.person.first_name|slice:"0:1" }}.
-                      ({{ note.late }}′)
+                      ({{ note.tardiness }}′)
                       {% if note.excused %}
                         <span class="lesson-note-excused">
                           {% if note.excuse_type %}
                             ({{ note.excuse_type.short_name }})
                           {% else %}
                             ({% trans 'e' %})
                           {% endif %}
```

#### html2text {}

```diff
@@ -2,15 +2,15 @@
 week_helpers %} {% block page_title %} {% trans "Class register:" %} {
 { group.name }} {% endblock %} {% block extra_head %}
  {% endblock %} {% block content %}
 ****** {% trans 'Class register' %} ******
 ** {{ school_term }} **
 ({{ school_term.date_start }}â{{ school_term.date_end }})
 {% static "img/aleksis-banner.svg" as aleksis_banner %} [{
-{ request.site.preferences.general__title }} â Logo]
+{ SITE_PREFERENCES.general__title }} â Logo]
 *** {{ group.name }} ***
 {% trans 'Owners' %}: {{ group.owners.all|join:', ' }}
 {% trans 'Printed on' %} {{ today }}
 ===============================================================================
 {% blocktrans %} This printout is intended for archival purposes. The main copy
 of the class register is stored in the AlekSIS School Information System. {%
 endblocktrans %}
@@ -73,24 +73,22 @@
 child_group.name lesson.subject.name lesson.teachers.all|join: lesson.validity.date_start lesson.validity.date_end lesson.lesson_periods.count
 }}               }}                  ', ' }}                   }}                         }}                       }}
  
 {% endif %} {% for person in persons %}
 *** {% trans 'Personal overview' %}: {{ person.last_name }}, {
 { person.first_name }} ***
 ** {% blocktrans %}Contact details{% endblocktrans %} **
-                               {{ person.first_name }} {
-{% if person.photo %} [ person { person.additional_name }} {{ person.last_name
-{{ person.first_name }}        }}
-{{ person.last_name }}] face   {{ person.get_sex_display }}
-{% else %} [{           home   {{ person.street }} {   {{ person.postal_code }}
-{ person.first_name }}         { person.housenumber }} {{ person.place }}
-{{ person.last_name }}] phone  {{ person.phone_number  {{ person.mobile_number
-{% endif %}                    }}                      }}
-                        email  {{ person.email }}
-                        cake   {{ person.date_of_birth|date }}
+{% if person.photo %} [{   {{ person.first_name }} {{ person.additional_name }}
+{ person.first_name }} {   {{ person.last_name }}
+{ person.last_name }}] {%  {{ person.get_sex_display }}
+else %} [{                 {{ person.street }} {     {{ person.postal_code }} {
+{ person.first_name }} {   { person.housenumber }}   { person.place }}
+{ person.last_name }}] {%  {{ person.phone_number }} {{ person.mobile_number }}
+endif %}                   {{ person.email }}
+                           {{ person.date_of_birth|date }}
 ** {% trans 'Absences and tardiness' %} **
 {% trans 'Absences' %}                                                      {{ person.absences_count }}
 {% trans         {% trans 'Excused' %}                                      {{ person.excused }}
 "thereof" %}
                                          {
 {% trans         {% trans "Without       {
 "thereof" %}     excuse type" %}         person.excused_without_excuse_type
@@ -109,37 +107,37 @@
 {{ extra_mark.name }} {{ person|get_dict:extra_mark.count_label }}
 {% endif %}
 ** {% trans 'Relevant personal notes' %} **
                                              {%
 {% trans  {% trans 'Pe.' %}                  trans   {% trans 'Te.' %}                {% trans 'Absent' %}                        {% trans 'Tard.' %}                      {% trans 'Remarks' %}
 'Date' %}                                    'Subj.'
                                              %}
-                                                                                                                                                                           {% if note.absent %} {%               {% for extra_mark in
-                                             {{ note.register_object.date_start }} {  {% if note.register_object.label_ !=                                                 trans 'Yes' %} {% if        {% if     note.extra_marks.all
-{         {                                  {                                        "event" %} {                                {                                        note.excused %} {% if       note.late %} {                  {
-{         {                                  note.register_object.period_from.period  {                                           {                                        note.excuse_type %} ({      %} {      {                     {
-note.date note.register_object.period.period }}.â{{ note.register_object.date_endnote.register_object.get_subject.short_name note.register_object.teacher_short_names {                           {         extra_mark.short_name note.remarks
-}}        }}                                 }} {                                     }} {% else %} {% trans "Event" %} {% endif  }}                                       note.excuse_type.short_name note.late }}{% if not           }}
-                                             { note.register_object.period_to.period  %}                                                                                   }}) {% else %} ({% trans    }}' {%    forloop.last %},{%
-                                             }}.                                                                                                                           'e' %}) {% endif %} {%      endif %}  endif %} {% endfor %}
+                                                                                                                                                                           {% if note.absent %} {%                    {% for extra_mark in
+                                             {{ note.register_object.date_start }} {  {% if note.register_object.label_ !=                                                 trans 'Yes' %} {% if        {% if          note.extra_marks.all
+{         {                                  {                                        "event" %} {                                {                                        note.excused %} {% if       note.tardiness %} {                  {
+{         {                                  note.register_object.period_from.period  {                                           {                                        note.excuse_type %} ({      %} {           {                     {
+note.date note.register_object.period.period }}.â{{ note.register_object.date_endnote.register_object.get_subject.short_name note.register_object.teacher_short_names {                           {              extra_mark.short_name note.remarks
+}}        }}                                 }} {                                     }} {% else %} {% trans "Event" %} {% endif  }}                                       note.excuse_type.short_name note.tardiness }}{% if not           }}
+                                             { note.register_object.period_to.period  %}                                                                                   }}) {% else %} ({% trans    }}' {% endif   forloop.last %},{%
+                                             }}.                                                                                                                           'e' %}) {% endif %} {%      %}             endif %} {% endfor %}
                                                                                                                                                                            endif %} {% endif %}
  
 {% endfor %} {% for week in weeks %}
 *** {% trans 'Week' %} {{ week.week }}: {{ week.0 }}â{{ week.6 }} ***
-          {% trans 'Pe.' %}                                {% trans 'Subj.' %}                 {% trans 'Lesson       {% trans 'Homework' %} {% trans 'Notes' %}                                                         {% trans 'Te.' %}
+          {% trans 'Pe.' %}                                {% trans 'Subj.' %}                 {% trans 'Lesson       {% trans 'Homework' %} {% trans 'Notes' %}                                                          {% trans 'Te.' %}
                                                                                                topic' %}
                                                                                                {% if
                                                                                                register_object.label_                        {{ documentation.group_note }} {% for note in notes %} {% if note.absent %}
-                                                           {% if register_object.label_ ==     == "event" %} {                               {{ note.person.last_name }}, {{ note.person.first_name|slice:"0:1" }}. {%
-                                                           "event" %} {% trans "Event" %} {%   {                                             if note.excused %}  {% if note.excuse_type %} ({
-          {% if register_object.label_ != "event" %} {     elif substitution %} {% include     register_object.title                         { note.excuse_type.short_name }}) {% else %} ({% trans 'e' %}) {% endif %}
-{         { register_object.period.period }} {% else %} {  "chronos/partials/subs/             }}: {                  {                      {% endif %}  {% endif %} {% if note.late %}  {{ note.person.last_name }}, { {% if documentation.topic %} {
-{         { register_object.period_from_on_day }}.â{  subject.html" with                  { documentation.topic  {                      { note.person.first_name|slice:"0:1" }}. ({{ note.late }}â²) {% if      {
-day|date: { register_object.period_to_on_day }}. {% endif  type="substitution" el=substitution }} {% elif             documentation.homework note.excused %}  {% if note.excuse_type %} ({{ note.excuse_type.short_name  register_object.get_teachers.first.short_name
-"D" }}    %}                                               %} {% else %} {% include "chronos/  substitution.cancelled }}                     }}) {% else %} ({% trans 'e' %}) {% endif %}  {% endif %}  {% endif %} {%   }} {% endif %}
+                                                           {% if register_object.label_ ==     == "event" %} {                               {{ note.person.last_name }}, {{ note.person.first_name|slice:"0:1" }}. {% if
+                                                           "event" %} {% trans "Event" %} {%   {                                             note.excused %}  {% if note.excuse_type %} ({{ note.excuse_type.short_name
+          {% if register_object.label_ != "event" %} {     elif substitution %} {% include     register_object.title                         }}) {% else %} ({% trans 'e' %}) {% endif %}  {% endif %}  {% endif %} {% if
+{         { register_object.period.period }} {% else %} {  "chronos/partials/subs/             }}: {                  {                      note.tardiness %}  {{ note.person.last_name }}, {                            {% if documentation.topic %} {
+{         { register_object.period_from_on_day }}.â{  subject.html" with                  { documentation.topic  {                      { note.person.first_name|slice:"0:1" }}. ({{ note.tardiness }}â²) {% if  {
+day|date: { register_object.period_to_on_day }}. {% endif  type="substitution" el=substitution }} {% elif             documentation.homework note.excused %}  {% if note.excuse_type %} ({{ note.excuse_type.short_name   register_object.get_teachers.first.short_name
+"D" }}    %}                                               %} {% else %} {% include "chronos/  substitution.cancelled }}                     }}) {% else %} ({% trans 'e' %}) {% endif %}  {% endif %}  {% endif %} {%    }} {% endif %}
                                                            partials/subject.html" with         %} {% trans 'Lesson                           for extra_mark in note.extra_marks.all %}  {{ note.person.last_name }}, {
                                                            subject=register_object.get_subject cancelled' %} {% else                         { note.person.first_name|slice:"0:1" }}. ({{ extra_mark.short_name }})  {%
                                                            %} {% endif %}                      %} {                                          endfor %} {% endfor %}
                                                                                                { documentation.topic
                                                                                                }} {% endif %}
  
 {% endfor %} {% endblock %}
```

### Comparing `AlekSIS-App-Alsijil-3.0.dev0/aleksis/apps/alsijil/tests/test_actions.py` & `aleksis_app_alsijil-3.0b0/aleksis/apps/alsijil/tests/test_actions.py`

 * *Files 1% similar despite different names*

```diff
@@ -48,15 +48,15 @@
         PersonalNote(
             person=person,
             event=_generate_event(date(2021, 3, 1)),
             absent=True,
             excused=True,
             excuse_type=excuse_type,
         ),
-        PersonalNote(person=person, event=_generate_event(date(2021, 10, 4)), late=10),
+        PersonalNote(person=person, event=_generate_event(date(2021, 10, 4)), tardiness=10),
         PersonalNote(
             person=person, event=_generate_event(date(2032, 10, 11)), remarks="Good work!"
         ),
         PersonalNote(person=person, event=_generate_event(date(2032, 10, 11))),
     ]
     PersonalNote.objects.bulk_create(notes)
     return notes
```

### Comparing `AlekSIS-App-Alsijil-3.0.dev0/aleksis/apps/alsijil/urls.py` & `aleksis_app_alsijil-3.0b0/aleksis/apps/alsijil/urls.py`

 * *Files 3% similar despite different names*

```diff
@@ -1,14 +1,12 @@
 from django.urls import path
 
 from . import views
 
 urlpatterns = [
-    path("coursebook/", views.SelectCoursebookView.as_view(), name="select_coursebook"),
-    path("coursebook/<int:pk>/", views.CoursebookView.as_view(), name="coursebook"),
     path("lesson", views.register_object, {"model": "lesson"}, name="lesson_period"),
     path(
         "lesson/<int:year>/<int:week>/<int:id_>",
         views.register_object,
         {"model": "lesson"},
         name="lesson_period",
     ),
@@ -46,14 +44,15 @@
     path("me/", views.overview_person, name="overview_me"),
     path(
         "notes/<int:pk>/delete/",
         views.DeletePersonalNoteView.as_view(),
         name="delete_personal_note",
     ),
     path("absence/new/<int:id_>/", views.register_absence, name="register_absence"),
+    path("absence/new/", views.register_absence, name="register_absence"),
     path("extra_marks/", views.ExtraMarkListView.as_view(), name="extra_marks"),
     path(
         "extra_marks/create/",
         views.ExtraMarkCreateView.as_view(),
         name="create_extra_mark",
     ),
     path(
```

### Comparing `AlekSIS-App-Alsijil-3.0.dev0/aleksis/apps/alsijil/util/alsijil_helpers.py` & `aleksis_app_alsijil-3.0b0/aleksis/apps/alsijil/util/alsijil_helpers.py`

 * *Files identical despite different names*

### Comparing `AlekSIS-App-Alsijil-3.0.dev0/aleksis/apps/alsijil/util/predicates.py` & `aleksis_app_alsijil-3.0b0/aleksis/apps/alsijil/util/predicates.py`

 * *Files identical despite different names*

### Comparing `AlekSIS-App-Alsijil-3.0.dev0/aleksis/apps/alsijil/views.py` & `aleksis_app_alsijil-3.0b0/aleksis/apps/alsijil/views.py`

 * *Files 4% similar despite different names*

```diff
@@ -1,61 +1,51 @@
 from contextlib import nullcontext
 from copy import deepcopy
-from datetime import date, datetime, timedelta
+from datetime import datetime, timedelta
 from typing import Any, Dict, Optional
 
 from django.apps import apps
 from django.core.exceptions import PermissionDenied
 from django.db.models import Count, Exists, FilteredRelation, OuterRef, Prefetch, Q, Sum
 from django.db.models.expressions import Case, When
 from django.db.models.functions import Extract
 from django.http import Http404, HttpRequest, HttpResponse, HttpResponseNotFound
 from django.shortcuts import get_object_or_404, redirect, render
 from django.urls import reverse, reverse_lazy
 from django.utils import timezone
 from django.utils.decorators import method_decorator
 from django.utils.http import url_has_allowed_host_and_scheme
-from django.utils.translation import ugettext as _
+from django.utils.translation import gettext as _
 from django.views import View
 from django.views.decorators.cache import never_cache
-from django.views.generic import DetailView, TemplateView
+from django.views.generic import DetailView
 
 import reversion
 from calendarweek import CalendarWeek
 from django_tables2 import RequestConfig, SingleTableView
 from guardian.core import ObjectPermissionChecker
 from guardian.shortcuts import get_objects_for_user
 from reversion.views import RevisionMixin
 from rules.contrib.views import PermissionRequiredMixin, permission_required
 
 from aleksis.apps.chronos.managers import TimetableType
-from aleksis.apps.chronos.models import (
-    Event,
-    ExtraLesson,
-    Holiday,
-    Lesson,
-    LessonPeriod,
-    TimePeriod,
-)
+from aleksis.apps.chronos.models import Event, ExtraLesson, Holiday, LessonPeriod, TimePeriod
 from aleksis.apps.chronos.util.build import build_weekdays
-from aleksis.apps.chronos.util.date import (
-    get_current_year,
-    get_weeks_for_year,
-    week_weekday_to_date,
-)
+from aleksis.apps.chronos.util.date import get_weeks_for_year, week_weekday_to_date
+from aleksis.core.decorators import pwa_cache
 from aleksis.core.mixins import (
     AdvancedCreateView,
     AdvancedDeleteView,
     AdvancedEditView,
     SuccessNextMixin,
 )
-from aleksis.core.models import Group, Person, SchoolTerm
+from aleksis.core.models import Group, PDFFile, Person, SchoolTerm
 from aleksis.core.util import messages
+from aleksis.core.util.celery_progress import render_progress_page
 from aleksis.core.util.core_helpers import get_site_preferences, objectgetter_optional
-from aleksis.core.util.pdf import render_pdf
 from aleksis.core.util.predicates import check_global_permission
 
 from .filters import PersonalNoteFilter
 from .forms import (
     AssignGroupRoleForm,
     ExcuseTypeForm,
     ExtraMarkForm,
@@ -65,39 +55,34 @@
     LessonDocumentationForm,
     PersonalNoteFormSet,
     PersonOverviewForm,
     RegisterAbsenceForm,
     RegisterObjectActionForm,
     SelectForm,
 )
-from .models import (
-    ExcuseType,
-    ExtraMark,
-    GroupRole,
-    GroupRoleAssignment,
-    LessonDocumentation,
-    PersonalNote,
-)
+from .models import ExcuseType, ExtraMark, GroupRole, GroupRoleAssignment, PersonalNote
 from .tables import (
     ExcuseTypeTable,
     ExtraMarkTable,
     GroupRoleTable,
     PersonalNoteTable,
     RegisterObjectSelectTable,
     RegisterObjectTable,
 )
+from .tasks import generate_full_register_printout
 from .util.alsijil_helpers import (
     annotate_documentations,
     generate_list_of_all_register_objects,
     get_register_object_by_pk,
     get_timetable_instance_by_pk,
     register_objects_sorter,
 )
 
 
+@pwa_cache
 @permission_required("alsijil.view_register_object_rule", fn=get_register_object_by_pk)  # FIXME
 def register_object(
     request: HttpRequest,
     model: Optional[str] = None,
     year: Optional[int] = None,
     week: Optional[int] = None,
     id_: Optional[int] = None,
@@ -243,21 +228,21 @@
         checker.prefetch_perms(register_object.get_groups().all())
         register_object.set_object_permission_checker(checker)
 
         # Create a formset that holds all personal notes for all persons in this lesson
         if not request.user.has_perm(
             "alsijil.view_register_object_personalnote_rule", register_object
         ):
-            persons = Person.objects.filter(pk=request.user.person.pk)
+            persons = Person.objects.filter(
+                Q(pk=request.user.person.pk) | Q(member_of__in=request.user.person.owner_of.all())
+            ).distinct()
         else:
             persons = Person.objects.all()
 
-        persons_qs = register_object.get_personal_notes(persons, wanted_week).filter(
-            person__member_of__in=request.user.person.owner_of.all()
-        )
+        persons_qs = register_object.get_personal_notes(persons, wanted_week).distinct()
 
         # Annotate group roles
         if show_group_roles:
             persons_qs = persons_qs.prefetch_related(
                 Prefetch(
                     "person__group_roles",
                     queryset=GroupRoleAssignment.objects.on_day(date_of_lesson).for_groups(groups),
@@ -339,14 +324,15 @@
         context["lesson_documentation"] = lesson_documentation
         context["lesson_documentation_form"] = lesson_documentation_form
         context["personal_note_formset"] = personal_note_formset
 
     return render(request, "alsijil/class_register/lesson.html", context)
 
 
+@pwa_cache
 @permission_required("alsijil.view_week_rule", fn=get_timetable_instance_by_pk)
 def week_view(
     request: HttpRequest,
     year: Optional[int] = None,
     week: Optional[int] = None,
     type_: Optional[str] = None,
     id_: Optional[int] = None,
@@ -483,20 +469,24 @@
     if lesson_periods_pk or events_pk or extra_lessons_pk:
         # Aggregate all personal notes for this group and week
         persons_qs = Person.objects.all()
 
         if not request.user.has_perm("alsijil.view_week_personalnote_rule", instance):
             persons_qs = persons_qs.filter(pk=request.user.person.pk)
         elif group:
-            persons_qs = persons_qs.filter(member_of=group).filter(
-                member_of__in=request.user.person.owner_of.all()
+            persons_qs = (
+                persons_qs.filter(member_of=group)
+                .filter(member_of__in=request.user.person.owner_of.all())
+                .distinct()
             )
         else:
-            persons_qs = persons_qs.filter(member_of__in=groups).filter(
-                member_of__in=request.user.person.owner_of.all()
+            persons_qs = (
+                persons_qs.filter(member_of__in=groups)
+                .filter(member_of__in=request.user.person.owner_of.all())
+                .distinct()
             )
 
         # Prefetch object permissions for persons and groups the persons are members of
         # because the object permissions are checked for both persons and groups
         checker = ObjectPermissionChecker(request.user)
         checker.prefetch_perms(persons_qs.prefetch_related(None))
         checker.prefetch_perms(groups)
@@ -545,18 +535,18 @@
             ),
             unexcused_count=Count(
                 "filtered_personal_notes",
                 filter=Q(
                     filtered_personal_notes__absent=True, filtered_personal_notes__excused=False
                 ),
             ),
-            tardiness_sum=Sum("filtered_personal_notes__late"),
+            tardiness_sum=Sum("filtered_personal_notes__tardiness"),
             tardiness_count=Count(
                 "filtered_personal_notes",
-                filter=Q(filtered_personal_notes__late__gt=0),
+                filter=Q(filtered_personal_notes__tardiness__gt=0),
             ),
         )
 
         for extra_mark in extra_marks:
             persons_qs = persons_qs.annotate(
                 **{
                     extra_mark.count_label: Count(
@@ -640,152 +630,52 @@
 
     context["url_prev"] = reverse("week_view_by_week", args=args_prev)
     context["url_next"] = reverse("week_view_by_week", args=args_next)
 
     return render(request, "alsijil/class_register/week_view.html", context)
 
 
+@pwa_cache
 @permission_required(
     "alsijil.view_full_register_rule", fn=objectgetter_optional(Group, None, False)
 )
 def full_register_group(request: HttpRequest, id_: int) -> HttpResponse:
-    context = {}
-
     group = get_object_or_404(Group, pk=id_)
-    groups_q = (
-        Q(lesson_period__lesson__groups=group)
-        | Q(lesson_period__lesson__groups__parent_groups=group)
-        | Q(extra_lesson__groups=group)
-        | Q(extra_lesson__groups__parent_groups=group)
-        | Q(event__groups=group)
-        | Q(event__groups__parent_groups=group)
-    )
-    personal_notes = (
-        PersonalNote.objects.prefetch_related(
-            "lesson_period__substitutions", "lesson_period__lesson__teachers"
-        )
-        .not_empty()
-        .filter(groups_q)
-        .filter(groups_of_person=group)
-    )
-    documentations = LessonDocumentation.objects.not_empty().filter(groups_q)
 
-    sorted_documentations = {"extra_lesson": {}, "event": {}, "lesson_period": {}}
-    sorted_personal_notes = {"extra_lesson": {}, "event": {}, "lesson_period": {}, "person": {}}
-    for documentation in documentations:
-        key = documentation.register_object.label_
-        sorted_documentations[key][documentation.register_object_key] = documentation
+    file_object = PDFFile.objects.create()
 
-    for note in personal_notes:
-        key = note.register_object.label_
-        sorted_personal_notes[key].setdefault(note.register_object_key, [])
-        sorted_personal_notes[key][note.register_object_key].append(note)
-        sorted_personal_notes["person"].setdefault(note.person.pk, [])
-        sorted_personal_notes["person"][note.person.pk].append(note)
-
-    # Get all lesson periods for the selected group
-    lesson_periods = LessonPeriod.objects.filter_group(group).distinct()
-    events = Event.objects.filter_group(group).distinct()
-    extra_lessons = ExtraLesson.objects.filter_group(group).distinct()
-    weeks = CalendarWeek.weeks_within(group.school_term.date_start, group.school_term.date_end)
-
-    register_objects_by_day = {}
-    for extra_lesson in extra_lessons:
-        day = extra_lesson.date
-        register_objects_by_day.setdefault(day, []).append(
-            (
-                extra_lesson,
-                sorted_documentations["extra_lesson"].get(extra_lesson.pk),
-                sorted_personal_notes["extra_lesson"].get(extra_lesson.pk, []),
-                None,
-            )
-        )
+    redirect_url = reverse("redirect_to_pdf_file", args=[file_object.pk])
 
-    for event in events:
-        day_number = (event.date_end - event.date_start).days + 1
-        for i in range(day_number):
-            day = event.date_start + timedelta(days=i)
-            event_copy = deepcopy(event)
-            event_copy.annotate_day(day)
-            register_objects_by_day.setdefault(day, []).append(
-                (
-                    event_copy,
-                    sorted_documentations["event"].get(event.pk),
-                    sorted_personal_notes["event"].get(event.pk, []),
-                    None,
-                )
-            )
+    result = generate_full_register_printout.delay(group.pk, file_object.pk)
 
-    weeks = CalendarWeek.weeks_within(
-        group.school_term.date_start,
-        group.school_term.date_end,
+    back_url = request.GET.get("back", "")
+    back_url_is_safe = url_has_allowed_host_and_scheme(
+        url=back_url,
+        allowed_hosts={request.get_host()},
+        require_https=request.is_secure(),
     )
+    if not back_url_is_safe:
+        back_url = reverse("my_groups")
 
-    for lesson_period in lesson_periods:
-        for week in weeks:
-            day = week[lesson_period.period.weekday]
-
-            if (
-                lesson_period.lesson.validity.date_start
-                <= day
-                <= lesson_period.lesson.validity.date_end
-            ):
-                filtered_documentation = sorted_documentations["lesson_period"].get(
-                    f"{lesson_period.pk}_{week.week}_{week.year}"
-                )
-                filtered_personal_notes = sorted_personal_notes["lesson_period"].get(
-                    f"{lesson_period.pk}_{week.week}_{week.year}", []
-                )
-
-                substitution = lesson_period.get_substitution(week)
-
-                register_objects_by_day.setdefault(day, []).append(
-                    (lesson_period, filtered_documentation, filtered_personal_notes, substitution)
-                )
-
-    persons = group.members.prefetch_related(None).select_related(None)
-    persons = group.generate_person_list_with_class_register_statistics(persons)
-
-    prefetched_persons = []
-    for person in persons:
-        person.filtered_notes = sorted_personal_notes["person"][person.pk]
-        prefetched_persons.append(person)
-
-    context["school_term"] = group.school_term
-    context["persons"] = prefetched_persons
-    context["excuse_types"] = ExcuseType.objects.filter(count_as_absent=True)
-    context["excuse_types_not_absent"] = ExcuseType.objects.filter(count_as_absent=False)
-    context["extra_marks"] = ExtraMark.objects.all()
-    context["group"] = group
-    context["weeks"] = weeks
-    context["register_objects_by_day"] = register_objects_by_day
-    context["register_objects"] = list(lesson_periods) + list(events) + list(extra_lessons)
-    context["today"] = date.today()
-    context["lessons"] = (
-        group.lessons.all()
-        .select_related(None)
-        .prefetch_related(None)
-        .select_related("validity", "subject")
-        .prefetch_related("teachers", "lesson_periods")
-    )
-    context["child_groups"] = (
-        group.child_groups.all()
-        .select_related(None)
-        .prefetch_related(None)
-        .prefetch_related(
-            "lessons",
-            "lessons__validity",
-            "lessons__subject",
-            "lessons__teachers",
-            "lessons__lesson_periods",
-        )
+    return render_progress_page(
+        request,
+        result,
+        title=_("Generate full register printout for {}").format(group),
+        progress_title=_("Generate full register printout …"),
+        success_message=_("The printout has been generated successfully."),
+        error_message=_("There was a problem while generating the printout."),
+        redirect_on_success_url=redirect_url,
+        back_url=back_url,
+        button_title=_("Download PDF"),
+        button_url=redirect_url,
+        button_icon="picture_as_pdf",
     )
-    return render_pdf(request, "alsijil/print/full_register.html", context)
 
 
+@pwa_cache
 @permission_required("alsijil.view_my_students_rule")
 def my_students(request: HttpRequest) -> HttpResponse:
     context = {}
     relevant_groups = (
         request.user.person.get_owner_groups_with_lessons()
         .annotate(has_parents=Exists(Group.objects.filter(child_groups=OuterRef("pk"))))
         .filter(members__isnull=False)
@@ -804,58 +694,61 @@
     new_groups = []
     for group in relevant_groups:
         persons = group.generate_person_list_with_class_register_statistics(
             group.members.prefetch_related(
                 "primary_group__owners",
                 Prefetch("member_of", queryset=relevant_groups, to_attr="member_of_prefetched"),
             )
-        ).filter(member_of__in=request.user.person.owner_of.all())
+        ).distinct()
         persons_for_group = []
         for person in persons:
             person.set_object_permission_checker(checker)
             persons_for_group.append(person)
         new_groups.append((group, persons_for_group))
 
     context["groups"] = new_groups
     context["excuse_types"] = ExcuseType.objects.filter(count_as_absent=True)
     context["excuse_types_not_absent"] = ExcuseType.objects.filter(count_as_absent=False)
     context["extra_marks"] = ExtraMark.objects.all()
     return render(request, "alsijil/class_register/persons.html", context)
 
 
+@pwa_cache
 @permission_required(
     "alsijil.view_my_groups_rule",
 )
 def my_groups(request: HttpRequest) -> HttpResponse:
     context = {}
     context["groups"] = request.user.person.get_owner_groups_with_lessons().annotate(
         students_count=Count("members", distinct=True)
     )
     return render(request, "alsijil/class_register/groups.html", context)
 
 
+@method_decorator(pwa_cache, "dispatch")
 class StudentsList(PermissionRequiredMixin, DetailView):
     model = Group
     template_name = "alsijil/class_register/students_list.html"
     permission_required = "alsijil.view_students_list_rule"
 
     def get_context_data(self, **kwargs):
         context = super().get_context_data(**kwargs)
         context["group"] = self.object
-        context[
-            "persons"
-        ] = self.object.generate_person_list_with_class_register_statistics().filter(
-            member_of__in=self.request.user.person.owner_of.all()
+        context["persons"] = (
+            self.object.generate_person_list_with_class_register_statistics()
+            .filter(member_of__in=self.request.user.person.owner_of.all())
+            .distinct()
         )
         context["extra_marks"] = ExtraMark.objects.all()
         context["excuse_types"] = ExcuseType.objects.filter(count_as_absent=True)
         context["excuse_types_not_absent"] = ExcuseType.objects.filter(count_as_absent=False)
         return context
 
 
+@pwa_cache
 @permission_required(
     "alsijil.view_person_overview_rule",
     fn=objectgetter_optional(
         Person.objects.prefetch_related("member_of__owners"), "request.user.person", True
     ),
 )
 def overview_person(request: HttpRequest, id_: Optional[int] = None) -> HttpResponse:
@@ -895,15 +788,15 @@
         )
 
     unexcused_absences = allowed_personal_notes.filter(absent=True, excused=False)
     context["unexcused_absences"] = unexcused_absences
 
     personal_notes = (
         allowed_personal_notes.not_empty()
-        .filter(Q(absent=True) | Q(late__gt=0) | ~Q(remarks="") | Q(extra_marks__isnull=False))
+        .filter(Q(absent=True) | Q(tardiness__gt=0) | ~Q(remarks="") | Q(extra_marks__isnull=False))
         .annotate(
             school_term_start=Case(
                 When(event__isnull=False, then="event__school_term__date_start"),
                 When(extra_lesson__isnull=False, then="extra_lesson__school_term__date_start"),
                 When(
                     lesson_period__isnull=False,
                     then="lesson_period__lesson__validity__school_term__date_start",
@@ -986,15 +879,17 @@
     extra_marks = ExtraMark.objects.all()
     excuse_types = ExcuseType.objects.all()
     if request.user.has_perm("alsijil.view_person_statistics_personalnote_rule", person):
         school_terms = SchoolTerm.objects.all().order_by("-date_start")
         stats = []
         for school_term in school_terms:
             stat = {}
-            personal_notes = PersonalNote.objects.filter(person=person,).filter(
+            personal_notes = PersonalNote.objects.filter(
+                person=person,
+            ).filter(
                 Q(lesson_period__lesson__validity__school_term=school_term)
                 | Q(extra_lesson__school_term=school_term)
                 | Q(event__school_term=school_term)
             )
 
             if not personal_notes.exists():
                 continue
@@ -1015,16 +910,18 @@
                 .aggregate(excused_no_excuse_type=Count("absent"))
             )
             stat.update(
                 personal_notes.filter(absent=True, excused=False).aggregate(
                     unexcused=Count("absent")
                 )
             )
-            stat.update(personal_notes.aggregate(tardiness=Sum("late")))
-            stat.update(personal_notes.filter(~Q(late=0)).aggregate(tardiness_count=Count("late")))
+            stat.update(personal_notes.aggregate(tardiness=Sum("tardiness")))
+            stat.update(
+                personal_notes.filter(~Q(tardiness=0)).aggregate(tardiness_count=Count("tardiness"))
+            )
 
             for extra_mark in extra_marks:
                 stat.update(
                     personal_notes.filter(extra_marks=extra_mark).aggregate(
                         **{extra_mark.count_label: Count("pk")}
                     )
                 )
@@ -1067,26 +964,35 @@
         RequestConfig(request, paginate={"per_page": items_per_page}).configure(table)
         context["register_object_table"] = table
     return render(request, "alsijil/class_register/person.html", context)
 
 
 @never_cache
 @permission_required("alsijil.register_absence_rule", fn=objectgetter_optional(Person))
-def register_absence(request: HttpRequest, id_: int) -> HttpResponse:
+def register_absence(request: HttpRequest, id_: int = None) -> HttpResponse:
     context = {}
 
-    person = get_object_or_404(Person, pk=id_)
+    if id_:
+        person = get_object_or_404(Person, pk=id_)
+    else:
+        person = None
 
-    register_absence_form = RegisterAbsenceForm(request.POST or None)
+    register_absence_form = RegisterAbsenceForm(
+        request, request.POST or None, initial={"person": person}
+    )
 
-    if request.method == "POST" and register_absence_form.is_valid():
+    if (
+        request.method == "POST"
+        and register_absence_form.is_valid()
+        and request.user.has_perm("alsijil.register_absence_rule", person)
+    ):
         confirmed = request.POST.get("confirmed", "0") == "1"
 
         # Get data from form
-        # person = register_absence_form.cleaned_data["person"]
+        person = register_absence_form.cleaned_data["person"]
         start_date = register_absence_form.cleaned_data["date_start"]
         end_date = register_absence_form.cleaned_data["date_end"]
         from_period = register_absence_form.cleaned_data["from_period"]
         to_period = register_absence_form.cleaned_data["to_period"]
         absent = register_absence_form.cleaned_data["absent"]
         excused = register_absence_form.cleaned_data["excused"]
         excuse_type = register_absence_form.cleaned_data["excuse_type"]
@@ -1148,14 +1054,15 @@
             reversion.set_user(request.user)
             note.reset_values()
             note.save()
         messages.success(request, _("The personal note has been deleted."))
         return redirect("overview_person", note.person.pk)
 
 
+@method_decorator(pwa_cache, "dispatch")
 class ExtraMarkListView(PermissionRequiredMixin, SingleTableView):
     """Table of all extra marks."""
 
     model = ExtraMark
     table_class = ExtraMarkTable
     permission_required = "alsijil.view_extramarks_rule"
     template_name = "alsijil/extra_mark/list.html"
@@ -1192,14 +1099,15 @@
     model = ExtraMark
     permission_required = "alsijil.delete_extramark_rule"
     template_name = "core/pages/delete.html"
     success_url = reverse_lazy("extra_marks")
     success_message = _("The extra mark has been deleted.")
 
 
+@method_decorator(pwa_cache, "dispatch")
 class ExcuseTypeListView(PermissionRequiredMixin, SingleTableView):
     """Table of all excuse types."""
 
     model = ExcuseType
     table_class = ExcuseTypeTable
     permission_required = "alsijil.view_excusetypes_rule"
     template_name = "alsijil/excuse_type/list.html"
@@ -1236,14 +1144,15 @@
     model = ExcuseType
     permission_required = "alsijil.delete_excusetype_rule"
     template_name = "core/pages/delete.html"
     success_url = reverse_lazy("excuse_types")
     success_message = _("The excuse type has been deleted.")
 
 
+@method_decorator(pwa_cache, "dispatch")
 class GroupRoleListView(PermissionRequiredMixin, SingleTableView):
     """Table of all group roles."""
 
     model = GroupRole
     table_class = GroupRoleTable
     permission_required = "alsijil.view_grouproles_rule"
     template_name = "alsijil/group_role/list.html"
@@ -1280,14 +1189,15 @@
     model = GroupRole
     permission_required = "alsijil.delete_grouprole_rule"
     template_name = "core/pages/delete.html"
     success_url = reverse_lazy("group_roles")
     success_message = _("The group role has been deleted.")
 
 
+@method_decorator(pwa_cache, "dispatch")
 class AssignedGroupRolesView(PermissionRequiredMixin, DetailView):
     permission_required = "alsijil.view_assigned_grouproles_rule"
     model = Group
     template_name = "alsijil/group_role/assigned_list.html"
 
     def get_context_data(self, **kwargs: Any) -> Dict[str, Any]:
         context = super().get_context_data()
@@ -1402,14 +1312,15 @@
     success_message = _("The group role assignment has been deleted.")
 
     def get_success_url(self) -> str:
         pk = self.object.groups.first().pk
         return reverse("assigned_group_roles", args=[pk])
 
 
+@method_decorator(pwa_cache, "dispatch")
 class AllRegisterObjectsView(PermissionRequiredMixin, View):
     """Provide overview of all register objects for coordinators."""
 
     permission_required = "alsijil.view_register_objects_list_rule"
 
     def get_context_data(self, request):
         context = {}
@@ -1448,54 +1359,7 @@
         return render(request, "alsijil/class_register/all_objects.html", context)
 
     def post(self, request: HttpRequest):
         context = self.get_context_data(request)
         if self.action_form.is_valid():
             self.action_form.execute()
         return render(request, "alsijil/class_register/all_objects.html", context)
-
-
-class CoursebookView(PermissionRequiredMixin, DetailView):
-    model = Lesson
-    template_name = "alsijil/class_register/coursebook.html"
-    permission_required = "alsijil.view_coursebook_rule"
-
-    def get_context_data(self, **kwargs):
-        context = super().get_context_data(**kwargs)
-        return context
-
-
-class SelectCoursebookView(PermissionRequiredMixin, TemplateView):
-    template_name = "alsijil/class_register/select_coursebook.html"
-    permission_required = "alsijil.view_coursebook_rule"  # FIXME
-
-    def get_context_data(self, **kwargs):
-        context = super().get_context_data(**kwargs)
-        person = self.request.user.person
-
-        current_week = CalendarWeek.current_week()
-        current_year = get_current_year()
-        # Show all future and the ones of last week
-
-        last_week, last_week_year = (
-            (current_week - 1, current_year)
-            if current_week >= 2
-            else (CalendarWeek.get_last_week_of_year(current_year - 1), current_year - 1)
-        )
-
-        last_week_query = Q(
-            lesson_periods__substitutions__week=last_week,
-            lesson_periods__substitutions__year=last_week_year,
-        )
-        this_week_query = Q(
-            lesson_periods__substitutions__week__gte=current_week,
-            lesson_periods__substitutions__year=current_year,
-        )
-        next_year_query = Q(lesson_periods__substitutions__year__gt=current_year)
-        context["lessons"] = Lesson.objects.filter(
-            Q(teachers=person)
-            | (
-                Q(lesson_periods__substitutions__teachers=person)
-                & (last_week_query | this_week_query | next_year_query)
-            )
-        ).for_current_or_all()
-        return context
```

#### encoding

```diff
@@ -1 +1 @@
-us-ascii
+utf-8
```

### Comparing `AlekSIS-App-Alsijil-3.0.dev0/docs/Makefile` & `aleksis_app_alsijil-3.0b0/docs/Makefile`

 * *Files identical despite different names*

### Comparing `AlekSIS-App-Alsijil-3.0.dev0/docs/_static/assign_group_role.png` & `aleksis_app_alsijil-3.0b0/docs/_static/assign_group_role.png`

 * *Files identical despite different names*

### Comparing `AlekSIS-App-Alsijil-3.0.dev0/docs/_static/create_excuse_type.png` & `aleksis_app_alsijil-3.0b0/docs/_static/create_excuse_type.png`

 * *Files identical despite different names*

### Comparing `AlekSIS-App-Alsijil-3.0.dev0/docs/_static/create_extra_mark.png` & `aleksis_app_alsijil-3.0b0/docs/_static/create_extra_mark.png`

 * *Files identical despite different names*

### Comparing `AlekSIS-App-Alsijil-3.0.dev0/docs/_static/edit_group_role.png` & `aleksis_app_alsijil-3.0b0/docs/_static/edit_group_role.png`

 * *Files identical despite different names*

### Comparing `AlekSIS-App-Alsijil-3.0.dev0/docs/_static/excuse_types.png` & `aleksis_app_alsijil-3.0b0/docs/_static/excuse_types.png`

 * *Files identical despite different names*

### Comparing `AlekSIS-App-Alsijil-3.0.dev0/docs/_static/extra_marks.png` & `aleksis_app_alsijil-3.0b0/docs/_static/extra_marks.png`

 * *Files identical despite different names*

### Comparing `AlekSIS-App-Alsijil-3.0.dev0/docs/_static/group_roles.png` & `aleksis_app_alsijil-3.0b0/docs/_static/group_roles.png`

 * *Files identical despite different names*

### Comparing `AlekSIS-App-Alsijil-3.0.dev0/docs/_static/lesson_documentation.png` & `aleksis_app_alsijil-3.0b0/docs/_static/lesson_documentation.png`

 * *Files identical despite different names*

### Comparing `AlekSIS-App-Alsijil-3.0.dev0/docs/_static/lesson_personal_notes.png` & `aleksis_app_alsijil-3.0b0/docs/_static/lesson_personal_notes.png`

 * *Files identical despite different names*

### Comparing `AlekSIS-App-Alsijil-3.0.dev0/docs/_static/lesson_version_history.png` & `aleksis_app_alsijil-3.0b0/docs/_static/lesson_version_history.png`

 * *Files identical despite different names*

### Comparing `AlekSIS-App-Alsijil-3.0.dev0/docs/_static/my_groups.png` & `aleksis_app_alsijil-3.0b0/docs/_static/my_groups.png`

 * *Files identical despite different names*

### Comparing `AlekSIS-App-Alsijil-3.0.dev0/docs/_static/my_students.png` & `aleksis_app_alsijil-3.0b0/docs/_static/my_students.png`

 * *Files identical despite different names*

### Comparing `AlekSIS-App-Alsijil-3.0.dev0/docs/_static/overview_lessons.png` & `aleksis_app_alsijil-3.0b0/docs/_static/overview_lessons.png`

 * *Files identical despite different names*

### Comparing `AlekSIS-App-Alsijil-3.0.dev0/docs/_static/overview_person.png` & `aleksis_app_alsijil-3.0b0/docs/_static/overview_person.png`

 * *Files identical despite different names*

### Comparing `AlekSIS-App-Alsijil-3.0.dev0/docs/_static/register_absence.png` & `aleksis_app_alsijil-3.0b0/docs/_static/register_absence.png`

 * *Files identical despite different names*

### Comparing `AlekSIS-App-Alsijil-3.0.dev0/docs/_static/register_absence_confirm.png` & `aleksis_app_alsijil-3.0b0/docs/_static/register_absence_confirm.png`

 * *Files identical despite different names*

### Comparing `AlekSIS-App-Alsijil-3.0.dev0/docs/_static/students_list.png` & `aleksis_app_alsijil-3.0b0/docs/_static/students_list.png`

 * *Files identical despite different names*

### Comparing `AlekSIS-App-Alsijil-3.0.dev0/docs/_static/week_view.png` & `aleksis_app_alsijil-3.0b0/docs/_static/week_view.png`

 * *Files identical despite different names*

### Comparing `AlekSIS-App-Alsijil-3.0.dev0/docs/_static/week_view_personal_notes.png` & `aleksis_app_alsijil-3.0b0/docs/_static/week_view_personal_notes.png`

 * *Files identical despite different names*

### Comparing `AlekSIS-App-Alsijil-3.0.dev0/docs/admin/30_configure.rst` & `aleksis_app_alsijil-3.0b0/docs/admin/30_configure.rst`

 * *Files identical despite different names*

### Comparing `AlekSIS-App-Alsijil-3.0.dev0/docs/admin/40_preferences.rst` & `aleksis_app_alsijil-3.0b0/docs/admin/40_preferences.rst`

 * *Files identical despite different names*

### Comparing `AlekSIS-App-Alsijil-3.0.dev0/docs/conf.py` & `aleksis_app_alsijil-3.0b0/docs/conf.py`

 * *Files 0% similar despite different names*

```diff
@@ -27,15 +27,15 @@
 project = "AlekSIS-App-Alsijil"
 copyright = "2019-2022 The AlekSIS team"
 author = "The AlekSIS Team"
 
 # The short X.Y version
 version = "3.0"
 # The full version, including alpha/beta/rc tags
-release = "3.0.dev1"
+release = "3.0b0"
 
 
 # -- General configuration ---------------------------------------------------
 
 # If your documentation needs a minimal Sphinx version, state it here.
 #
 # needs_sphinx = '1.0'
```

### Comparing `AlekSIS-App-Alsijil-3.0.dev0/docs/index.rst` & `aleksis_app_alsijil-3.0b0/docs/index.rst`

 * *Files identical despite different names*

### Comparing `AlekSIS-App-Alsijil-3.0.dev0/docs/make.bat` & `aleksis_app_alsijil-3.0b0/docs/make.bat`

 * *Files identical despite different names*

### Comparing `AlekSIS-App-Alsijil-3.0.dev0/docs/user/10_basic.rst` & `aleksis_app_alsijil-3.0b0/docs/user/10_basic.rst`

 * *Files identical despite different names*

### Comparing `AlekSIS-App-Alsijil-3.0.dev0/docs/user/15_concepts.rst` & `aleksis_app_alsijil-3.0b0/docs/user/15_concepts.rst`

 * *Files identical despite different names*

### Comparing `AlekSIS-App-Alsijil-3.0.dev0/docs/user/20_overview.rst` & `aleksis_app_alsijil-3.0b0/docs/user/20_overview.rst`

 * *Files identical despite different names*

### Comparing `AlekSIS-App-Alsijil-3.0.dev0/docs/user/21_lesson.rst` & `aleksis_app_alsijil-3.0b0/docs/user/21_lesson.rst`

 * *Files identical despite different names*

### Comparing `AlekSIS-App-Alsijil-3.0.dev0/docs/user/40_export.rst` & `aleksis_app_alsijil-3.0b0/docs/user/40_export.rst`

 * *Files identical despite different names*

### Comparing `AlekSIS-App-Alsijil-3.0.dev0/pyproject.toml` & `aleksis_app_alsijil-3.0b0/pyproject.toml`

 * *Files 7% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 [tool.poetry]
 name = "AlekSIS-App-Alsijil"
-version = "3.0.dev0"
+version = "3.0b0"
 packages = [
     { include = "aleksis" }
 ]
 readme = "README.rst"
 include = [
     { path = "aleksis/**/*.mo", format = ["sdist", "wheel"] },
     { path = "*.rst", format = "sdist" },
@@ -18,44 +18,43 @@
 authors = [
     "Dominik George <dominik.george@teckids.org>",
     "Julian Leucker <leuckeju@katharineum.de>",
     "Jonathan Weth <dev@jonathanweth.de>",
     "Hangzhi Yu <yuha@katharineum.de>",
     "Lloyd Meins <meinsll@katharineum.de>",
     "mirabilos <thorsten.glaser@teckids.org>",
-    "Tom Teichler <tom.teichler@teckids.org>",
-    "magicfelix <felix@felix-zauberer.de>"
+    "Tom Teichler <tom.teichler@teckids.org>"
 ]
 maintainers = [
     "Dominik George <dominik.george@teckids.org>",
     "Jonathan Weth <dev@jonathanweth.de>",
 ]
 license = "EUPL-1.2"
-homepage = "https://aleksis.edugit.io/"
-repository = "https://edugit.org/AlekSIS/Official/AlekSIS-App-Alsijil"
+homepage = "https://aleksis.org/"
+repository = "https://edugit.org/AlekSIS/official/AlekSIS-App-Alsijil"
 documentation = "https://aleksis.edugit.io/AlekSIS/docs/html/"
 classifiers = [
-    "Development Status :: 4 - Beta",
+    "Development Status :: 5 - Production/Stable",
     "Environment :: Web Environment",
-    "Framework :: Django :: 3.0",
+    "Framework :: Django :: 4.0",
     "Intended Audience :: Education",
     "Topic :: Education",
     "Typing :: Typed",
 ]
 
 [[tool.poetry.source]]
 name = "gitlab"
 url = "https://edugit.org/api/v4/projects/461/packages/pypi/simple"
 secondary = true
 
 [tool.poetry.dependencies]
 python = "^3.9"
-aleksis-core = "^3.0.0.dev0"
-aleksis-app-chronos = "^3.0.0.dev0"
-aleksis-app-stoelindeling = { version = "^2.0.0.dev0", optional = true }
+aleksis-core = "^3.0b0"
+aleksis-app-chronos = "^3.0b0"
+aleksis-app-stoelindeling = { version = "^2.0b0", optional = true }
 
 [tool.poetry.dev-dependencies]
 aleksis-builddeps = "*"
 
 [tool.poetry.extras]
 seatingplans = ["aleksis-app-stoelindeling"]
```

### Comparing `AlekSIS-App-Alsijil-3.0.dev0/tox.ini` & `aleksis_app_alsijil-3.0b0/tox.ini`

 * *Files 22% similar despite different names*

```diff
@@ -1,20 +1,19 @@
 [tox]
 skipsdist = True
 skip_missing_interpreters = true
-envlist = py37,py38,py39
+envlist = py39,py310,py311
 
 [testenv]
 whitelist_externals = poetry
-		      sudo
 skip_install = true
 envdir = {toxworkdir}/globalenv
 commands_pre =
      poetry install
-     poetry run aleksis-admin webpack_bundle
+     poetry run aleksis-admin vite build
      poetry run aleksis-admin collectstatic --no-input
 commands =
     poetry run pytest --cov=. {posargs} aleksis/
 
 [testenv:selenium]
 setenv =
     TEST_SCREENSHOT_PATH = {env:TEST_SCREENSHOT_PATH:.tox/screenshots}
@@ -23,14 +22,16 @@
     TEST_HOST = {env:TEST_HOST:172.17.0.1}
 
 [testenv:lint]
 commands =
     poetry run black --check --diff aleksis/
     poetry run isort -c --diff --stdout aleksis/
     poetry run flake8 {posargs} aleksis/
+    poetry run sh -c "aleksis-admin yarn run prettier --check --ignore-path={toxinidir}/.prettierignore {toxinidir}"
+    poetry run sh -c "aleksis-admin yarn run eslint {toxinidir}/aleksis/**/*/frontend/**/*.{js,vue} --config={toxinidir}/.eslintrc.js --resolve-plugins-relative-to=."
 
 [testenv:security]
 commands =
     poetry show --no-dev
     poetry run safety check --full-report
 
 [testenv:build]
@@ -42,14 +43,15 @@
 [testenv:docs]
 commands = poetry run make -C docs/ html {posargs}
 
 [testenv:reformat]
 commands =
     poetry run isort aleksis/
     poetry run black aleksis/
+    poetry run sh -c "aleksis-admin yarn run prettier --write --ignore-path={toxinidir}/.prettierignore {toxinidir}"
 
 [testenv:makemessages]
 commands =
     poetry run aleksis-admin makemessages --no-wrap -e html,txt,py,email -i static -l ar -l de_DE -l fr -l nb_NO -l tr_TR -l la -l uk -l ru
     poetry run aleksis-admin makemessages --no-wrap -d djangojs -i **/node_modules -l ar -l de_DE -l fr -l nb_NO -l tr_TR -l la -l uk -l ru
 
 [flake8]
```

### Comparing `AlekSIS-App-Alsijil-3.0.dev0/setup.py` & `aleksis_app_alsijil-3.0b0/setup.py`

 * *Files 2% similar despite different names*

```diff
@@ -7,16 +7,16 @@
  'aleksis.apps.alsijil.migrations',
  'aleksis.apps.alsijil.templatetags',
  'aleksis.apps.alsijil.tests',
  'aleksis.apps.alsijil.util']
 
 package_data = \
 {'': ['*'],
- 'aleksis.apps.alsijil': ['assets/*',
-                          'assets/components/coursebook/*',
+ 'aleksis.apps.alsijil': ['frontend/*',
+                          'frontend/messages/*',
                           'locale/ar/LC_MESSAGES/*',
                           'locale/de_DE/LC_MESSAGES/*',
                           'locale/fr/LC_MESSAGES/*',
                           'locale/la/LC_MESSAGES/*',
                           'locale/nb_NO/LC_MESSAGES/*',
                           'locale/ru/LC_MESSAGES/*',
                           'locale/tr_TR/LC_MESSAGES/*',
@@ -32,32 +32,32 @@
                           'templates/alsijil/notifications/*',
                           'templates/alsijil/partials/*',
                           'templates/alsijil/partials/lesson/*',
                           'templates/alsijil/partials/lesson/tabs/*',
                           'templates/alsijil/print/*']}
 
 install_requires = \
-['aleksis-app-chronos>=3.0.0.dev0,<4.0.0', 'aleksis-core>=3.0.0.dev0,<4.0.0']
+['aleksis-app-chronos>=3.0b0,<4.0', 'aleksis-core>=3.0b0,<4.0']
 
 extras_require = \
-{'seatingplans': ['aleksis-app-stoelindeling>=2.0.0.dev0,<3.0.0']}
+{'seatingplans': ['aleksis-app-stoelindeling>=2.0b0,<3.0']}
 
 entry_points = \
 {'aleksis.app': ['alsijil = aleksis.apps.alsijil.apps:AlsijilConfig']}
 
 setup_kwargs = {
     'name': 'aleksis-app-alsijil',
-    'version': '3.0.dev0',
+    'version': '3.0b0',
     'description': 'AlekSIS (School Information System)\u200a—\u200aApp كتاب السجل (class register and school records)',
-    'long_description': 'AlekSIS (School Information System)\u200a—\u200aApp كتاب السجل (class register and school records)\n========================================================================================\n\nAlekSIS\n-------\n\nThis is an application for use with the `AlekSIS®`_ platform.\n\nFeatures\n--------\n\nThis AlekSIS app currently provides the following features for managing digital class registers:\n\n* For users:\n\n * Manage and assign group roles\n * Manage custom excuse types\n * Manage extra marks (e. g. forgotten homework)\n * Manage group notes for every lesson\n * Manage lesson documentations for every lesson\n * Manage personal notes for every lesson\n * Show all owned groups of the current person\n * Show all students of the current person\n * Show filterable (week) overview for lesson documentations and personal/group notes\n * Manage absence of persons\n * Show overview of all students with statistics\n \n\nLicence\n-------\n\n::\n\n  Copyright © 2019, 2021 Dominik George <dominik.george@teckids.org>\n  Copyright © 2019, 2020 Tom Teichler <tom.teichler@teckids.org>\n  Copyright © 2019 mirabilos <thorsten.glaser@teckids.org>\n  Copyright © 2020, 2021, 2022 Jonathan Weth <dev@jonathanweth.de>\n  Copyright © 2020, 2021 Julian Leucker <leuckeju@katharineum.de>\n  Copyright © 2020, 2022 Hangzhi Yu <yuha@katharineum.de>\n  Copyright © 2021 Lloyd Meins <meinsll@katharineum.de>\n  Copyright © 2022 magicfelix <felix@felix-zauberer.de>\n\n\n  Licenced under the EUPL, version 1.2 or later, by Teckids e.V. (Bonn, Germany).\n\nPlease see the LICENCE.rst file accompanying this distribution for the\nfull licence text or on the `European Union Public Licence`_ website\nhttps://joinup.ec.europa.eu/collection/eupl/guidelines-users-and-developers\n(including all other official language versions).\n\nTrademark\n---------\n\nAlekSIS® is a registered trademark of the AlekSIS open source project, represented\nby Teckids e.V. Please refer to the `trademark policy`_ for hints on using the trademark\nAlekSIS®.\n\n.. _AlekSIS®: https://edugit.org/AlekSIS/Official/AlekSIS\n.. _European Union Public Licence: https://eupl.eu/\n.. _trademark policy: https://aleksis.org/pages/about\n',
+    'long_description': 'AlekSIS (School Information System)\u200a—\u200aApp كتاب السجل (class register and school records)\n========================================================================================\n\nAlekSIS\n-------\n\nThis is an application for use with the `AlekSIS®`_ platform.\n\nFeatures\n--------\n\nThis AlekSIS app currently provides the following features for managing digital class registers:\n\n* For users:\n\n * Manage and assign group roles\n * Manage custom excuse types\n * Manage extra marks (e. g. forgotten homework)\n * Manage group notes for every lesson\n * Manage lesson documentations for every lesson\n * Manage personal notes for every lesson\n * Show all owned groups of the current person\n * Show all students of the current person\n * Show filterable (week) overview for lesson documentations and personal/group notes\n * Manage absence of persons\n * Show overview of all students with statistics\n \n\nLicence\n-------\n\n::\n\n  Copyright © 2019, 2021 Dominik George <dominik.george@teckids.org>\n  Copyright © 2019, 2020 Tom Teichler <tom.teichler@teckids.org>\n  Copyright © 2019 mirabilos <thorsten.glaser@teckids.org>\n  Copyright © 2020, 2021, 2022 Jonathan Weth <dev@jonathanweth.de>\n  Copyright © 2020, 2021 Julian Leucker <leuckeju@katharineum.de>\n  Copyright © 2020, 2022 Hangzhi Yu <yuha@katharineum.de>\n  Copyright © 2021 Lloyd Meins <meinsll@katharineum.de>\n\n\n  Licenced under the EUPL, version 1.2 or later, by Teckids e.V. (Bonn, Germany).\n\nPlease see the LICENCE.rst file accompanying this distribution for the\nfull licence text or on the `European Union Public Licence`_ website\nhttps://joinup.ec.europa.eu/collection/eupl/guidelines-users-and-developers\n(including all other official language versions).\n\nTrademark\n---------\n\nAlekSIS® is a registered trademark of the AlekSIS open source project, represented\nby Teckids e.V. Please refer to the `trademark policy`_ for hints on using the trademark\nAlekSIS®.\n\n.. _AlekSIS®: https://edugit.org/AlekSIS/Official/AlekSIS\n.. _European Union Public Licence: https://eupl.eu/\n.. _trademark policy: https://aleksis.org/pages/about\n',
     'author': 'Dominik George',
     'author_email': 'dominik.george@teckids.org',
     'maintainer': 'Dominik George',
     'maintainer_email': 'dominik.george@teckids.org',
-    'url': 'https://aleksis.edugit.io/',
+    'url': 'https://aleksis.org/',
     'packages': packages,
     'package_data': package_data,
     'install_requires': install_requires,
     'extras_require': extras_require,
     'entry_points': entry_points,
     'python_requires': '>=3.9,<4.0',
 }
```

### Comparing `AlekSIS-App-Alsijil-3.0.dev0/PKG-INFO` & `aleksis_app_alsijil-3.0b0/PKG-INFO`

 * *Files 5% similar despite different names*

```diff
@@ -1,34 +1,35 @@
 Metadata-Version: 2.1
 Name: aleksis-app-alsijil
-Version: 3.0.dev0
+Version: 3.0b0
 Summary: AlekSIS (School Information System) — App كتاب السجل (class register and school records)
-Home-page: https://aleksis.edugit.io/
+Home-page: https://aleksis.org/
 License: EUPL-1.2
 Author: Dominik George
 Author-email: dominik.george@teckids.org
 Maintainer: Dominik George
 Maintainer-email: dominik.george@teckids.org
 Requires-Python: >=3.9,<4.0
-Classifier: Development Status :: 4 - Beta
+Classifier: Development Status :: 5 - Production/Stable
 Classifier: Environment :: Web Environment
-Classifier: Framework :: Django :: 3.0
+Classifier: Framework :: Django :: 4.0
 Classifier: Intended Audience :: Education
 Classifier: License :: OSI Approved :: European Union Public Licence 1.2 (EUPL 1.2)
 Classifier: Programming Language :: Python :: 3
-Classifier: Programming Language :: Python :: 3.10
 Classifier: Programming Language :: Python :: 3.9
+Classifier: Programming Language :: Python :: 3.10
+Classifier: Programming Language :: Python :: 3.11
 Classifier: Topic :: Education
 Classifier: Typing :: Typed
 Provides-Extra: seatingplans
-Requires-Dist: aleksis-app-chronos (>=3.0.0.dev0,<4.0.0)
-Requires-Dist: aleksis-app-stoelindeling (>=2.0.0.dev0,<3.0.0); extra == "seatingplans"
-Requires-Dist: aleksis-core (>=3.0.0.dev0,<4.0.0)
+Requires-Dist: aleksis-app-chronos (>=3.0b0,<4.0)
+Requires-Dist: aleksis-app-stoelindeling (>=2.0b0,<3.0) ; extra == "seatingplans"
+Requires-Dist: aleksis-core (>=3.0b0,<4.0)
 Project-URL: Documentation, https://aleksis.edugit.io/AlekSIS/docs/html/
-Project-URL: Repository, https://edugit.org/AlekSIS/Official/AlekSIS-App-Alsijil
+Project-URL: Repository, https://edugit.org/AlekSIS/official/AlekSIS-App-Alsijil
 Description-Content-Type: text/x-rst
 
 AlekSIS (School Information System) — App كتاب السجل (class register and school records)
 ========================================================================================
 
 AlekSIS
 -------
@@ -63,15 +64,14 @@
   Copyright © 2019, 2021 Dominik George <dominik.george@teckids.org>
   Copyright © 2019, 2020 Tom Teichler <tom.teichler@teckids.org>
   Copyright © 2019 mirabilos <thorsten.glaser@teckids.org>
   Copyright © 2020, 2021, 2022 Jonathan Weth <dev@jonathanweth.de>
   Copyright © 2020, 2021 Julian Leucker <leuckeju@katharineum.de>
   Copyright © 2020, 2022 Hangzhi Yu <yuha@katharineum.de>
   Copyright © 2021 Lloyd Meins <meinsll@katharineum.de>
-  Copyright © 2022 magicfelix <felix@felix-zauberer.de>
 
 
   Licenced under the EUPL, version 1.2 or later, by Teckids e.V. (Bonn, Germany).
 
 Please see the LICENCE.rst file accompanying this distribution for the
 full licence text or on the `European Union Public Licence`_ website
 https://joinup.ec.europa.eu/collection/eupl/guidelines-users-and-developers
```

