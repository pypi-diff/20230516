# Comparing `tmp/aioqui-2.0.0.tar.gz` & `tmp/aioqui-2.0.1.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "aioqui-2.0.0.tar", last modified: Mon May 15 09:05:51 2023, max compression
+gzip compressed data, was "aioqui-2.0.1.tar", last modified: Tue May 16 21:21:00 2023, max compression
```

## Comparing `aioqui-2.0.0.tar` & `aioqui-2.0.1.tar`

### file list

```diff
@@ -1,368 +1,377 @@
-drwxrwxrwx   0        0        0        0 2023-05-15 09:05:51.529507 aioqui-2.0.0/
--rw-rw-rw-   0        0        0     1093 2023-02-26 16:41:50.000000 aioqui-2.0.0/LICENSE.txt
--rw-rw-rw-   0        0        0     2629 2023-05-15 09:05:51.528507 aioqui-2.0.0/PKG-INFO
--rw-rw-rw-   0        0        0      282 2023-05-15 08:21:18.000000 aioqui-2.0.0/README.md
--rw-rw-rw-   0        0        0     1488 2023-05-15 09:05:20.000000 aioqui-2.0.0/pyproject.toml
--rw-rw-rw-   0        0        0       42 2023-05-15 09:05:51.529507 aioqui-2.0.0/setup.cfg
-drwxrwxrwx   0        0        0        0 2023-05-15 09:05:51.219508 aioqui-2.0.0/src/
--rw-rw-rw-   0        0        0        0 2023-03-20 19:19:08.000000 aioqui-2.0.0/src/__init__.py
-drwxrwxrwx   0        0        0        0 2023-05-15 09:05:51.221513 aioqui-2.0.0/src/aioqui/
-drwxrwxrwx   0        0        0        0 2023-05-15 09:05:51.214507 aioqui-2.0.0/src/aioqui/.assets/
-drwxrwxrwx   0        0        0        0 2023-05-15 09:05:51.484507 aioqui-2.0.0/src/aioqui/.assets/icons/
--rw-rw-rw-   0        0        0      277 2023-03-18 18:50:21.000000 aioqui-2.0.0/src/aioqui/.assets/icons/activity.svg
--rw-rw-rw-   0        0        0      357 2023-03-18 18:50:21.000000 aioqui-2.0.0/src/aioqui/.assets/icons/airplay.svg
--rw-rw-rw-   0        0        0      351 2023-03-18 18:50:21.000000 aioqui-2.0.0/src/aioqui/.assets/icons/alert-circle.svg
--rw-rw-rw-   0        0        0      411 2023-03-18 18:50:21.000000 aioqui-2.0.0/src/aioqui/.assets/icons/alert-octagon.svg
--rw-rw-rw-   0        0        0      419 2023-03-18 18:50:21.000000 aioqui-2.0.0/src/aioqui/.assets/icons/alert-triangle.svg
--rw-rw-rw-   0        0        0      393 2023-03-18 18:50:21.000000 aioqui-2.0.0/src/aioqui/.assets/icons/align-center.svg
--rw-rw-rw-   0        0        0      394 2023-03-18 18:50:21.000000 aioqui-2.0.0/src/aioqui/.assets/icons/align-justify.svg
--rw-rw-rw-   0        0        0      391 2023-03-18 18:50:21.000000 aioqui-2.0.0/src/aioqui/.assets/icons/align-left.svg
--rw-rw-rw-   0        0        0      392 2023-03-18 18:50:21.000000 aioqui-2.0.0/src/aioqui/.assets/icons/align-right.svg
--rw-rw-rw-   0        0        0      340 2023-03-18 18:50:21.000000 aioqui-2.0.0/src/aioqui/.assets/icons/anchor.svg
--rw-rw-rw-   0        0        0      563 2023-03-18 18:50:21.000000 aioqui-2.0.0/src/aioqui/.assets/icons/aperture.svg
--rw-rw-rw-   0        0        0      356 2023-03-18 18:50:21.000000 aioqui-2.0.0/src/aioqui/.assets/icons/archive.svg
--rw-rw-rw-   0        0        0      355 2023-03-18 18:50:21.000000 aioqui-2.0.0/src/aioqui/.assets/icons/arrow-down-circle.svg
--rw-rw-rw-   0        0        0      310 2023-03-18 18:50:21.000000 aioqui-2.0.0/src/aioqui/.assets/icons/arrow-down-left.svg
--rw-rw-rw-   0        0        0      312 2023-03-18 18:50:21.000000 aioqui-2.0.0/src/aioqui/.assets/icons/arrow-down-right.svg
--rw-rw-rw-   0        0        0      308 2023-03-18 18:50:21.000000 aioqui-2.0.0/src/aioqui/.assets/icons/arrow-down.svg
--rw-rw-rw-   0        0        0      354 2023-03-18 18:50:21.000000 aioqui-2.0.0/src/aioqui/.assets/icons/arrow-left-circle.svg
--rw-rw-rw-   0        0        0      307 2023-03-18 18:50:21.000000 aioqui-2.0.0/src/aioqui/.assets/icons/arrow-left.svg
--rw-rw-rw-   0        0        0      356 2023-03-18 18:50:21.000000 aioqui-2.0.0/src/aioqui/.assets/icons/arrow-right-circle.svg
--rw-rw-rw-   0        0        0      309 2023-03-18 18:50:21.000000 aioqui-2.0.0/src/aioqui/.assets/icons/arrow-right.svg
--rw-rw-rw-   0        0        0      352 2023-03-18 18:50:21.000000 aioqui-2.0.0/src/aioqui/.assets/icons/arrow-up-circle.svg
--rw-rw-rw-   0        0        0      307 2023-03-18 18:50:21.000000 aioqui-2.0.0/src/aioqui/.assets/icons/arrow-up-left.svg
--rw-rw-rw-   0        0        0      309 2023-03-18 18:50:21.000000 aioqui-2.0.0/src/aioqui/.assets/icons/arrow-up-right.svg
--rw-rw-rw-   0        0        0      305 2023-03-18 18:50:21.000000 aioqui-2.0.0/src/aioqui/.assets/icons/arrow-up.svg
--rw-rw-rw-   0        0        0      317 2023-03-18 18:50:21.000000 aioqui-2.0.0/src/aioqui/.assets/icons/at-sign.svg
--rw-rw-rw-   0        0        0      320 2023-03-18 18:50:21.000000 aioqui-2.0.0/src/aioqui/.assets/icons/award.svg
--rw-rw-rw-   0        0        0      350 2023-03-18 18:50:21.000000 aioqui-2.0.0/src/aioqui/.assets/icons/bar-chart-2.svg
--rw-rw-rw-   0        0        0      348 2023-03-18 18:50:21.000000 aioqui-2.0.0/src/aioqui/.assets/icons/bar-chart.svg
--rw-rw-rw-   0        0        0      422 2023-03-18 18:50:21.000000 aioqui-2.0.0/src/aioqui/.assets/icons/battery-charging.svg
--rw-rw-rw-   0        0        0      321 2023-03-18 18:50:21.000000 aioqui-2.0.0/src/aioqui/.assets/icons/battery.svg
--rw-rw-rw-   0        0        0      455 2023-03-18 18:50:21.000000 aioqui-2.0.0/src/aioqui/.assets/icons/bell-off.svg
--rw-rw-rw-   0        0        0      316 2023-03-18 18:50:21.000000 aioqui-2.0.0/src/aioqui/.assets/icons/bell.svg
--rw-rw-rw-   0        0        0      293 2023-03-18 18:50:21.000000 aioqui-2.0.0/src/aioqui/.assets/icons/bluetooth.svg
--rw-rw-rw-   0        0        0      322 2023-03-18 18:50:21.000000 aioqui-2.0.0/src/aioqui/.assets/icons/bold.svg
--rw-rw-rw-   0        0        0      334 2023-03-18 18:50:21.000000 aioqui-2.0.0/src/aioqui/.assets/icons/book-open.svg
--rw-rw-rw-   0        0        0      340 2023-03-18 18:50:21.000000 aioqui-2.0.0/src/aioqui/.assets/icons/book.svg
--rw-rw-rw-   0        0        0      282 2023-03-18 18:50:21.000000 aioqui-2.0.0/src/aioqui/.assets/icons/bookmark.svg
--rw-rw-rw-   0        0        0      457 2023-03-18 18:50:21.000000 aioqui-2.0.0/src/aioqui/.assets/icons/box.svg
--rw-rw-rw-   0        0        0      338 2023-03-18 18:50:21.000000 aioqui-2.0.0/src/aioqui/.assets/icons/briefcase.svg
--rw-rw-rw-   0        0        0      405 2023-03-18 18:50:21.000000 aioqui-2.0.0/src/aioqui/.assets/icons/calendar.svg
--rw-rw-rw-   0        0        0      380 2023-03-18 18:50:21.000000 aioqui-2.0.0/src/aioqui/.assets/icons/camera-off.svg
--rw-rw-rw-   0        0        0      351 2023-03-18 18:50:21.000000 aioqui-2.0.0/src/aioqui/.assets/icons/camera.svg
--rw-rw-rw-   0        0        0      382 2023-03-18 18:50:21.000000 aioqui-2.0.0/src/aioqui/.assets/icons/cast.svg
--rw-rw-rw-   0        0        0      323 2023-03-18 18:50:21.000000 aioqui-2.0.0/src/aioqui/.assets/icons/check-circle.svg
--rw-rw-rw-   0        0        0      340 2023-03-18 18:50:21.000000 aioqui-2.0.0/src/aioqui/.assets/icons/check-square.svg
--rw-rw-rw-   0        0        0      257 2023-03-18 18:50:21.000000 aioqui-2.0.0/src/aioqui/.assets/icons/check.svg
--rw-rw-rw-   0        0        0      264 2023-03-18 18:50:21.000000 aioqui-2.0.0/src/aioqui/.assets/icons/chevron-down.svg
--rw-rw-rw-   0        0        0      265 2023-03-18 18:50:21.000000 aioqui-2.0.0/src/aioqui/.assets/icons/chevron-left.svg
--rw-rw-rw-   0        0        0      265 2023-03-18 18:50:21.000000 aioqui-2.0.0/src/aioqui/.assets/icons/chevron-right.svg
--rw-rw-rw-   0        0        0      263 2023-03-18 18:50:21.000000 aioqui-2.0.0/src/aioqui/.assets/icons/chevron-up.svg
--rw-rw-rw-   0        0        0      312 2023-03-18 18:50:21.000000 aioqui-2.0.0/src/aioqui/.assets/icons/chevrons-down.svg
--rw-rw-rw-   0        0        0      313 2023-03-18 18:50:21.000000 aioqui-2.0.0/src/aioqui/.assets/icons/chevrons-left.svg
--rw-rw-rw-   0        0        0      313 2023-03-18 18:50:21.000000 aioqui-2.0.0/src/aioqui/.assets/icons/chevrons-right.svg
--rw-rw-rw-   0        0        0      311 2023-03-18 18:50:21.000000 aioqui-2.0.0/src/aioqui/.assets/icons/chevrons-up.svg
--rw-rw-rw-   0        0        0      443 2023-03-18 18:50:21.000000 aioqui-2.0.0/src/aioqui/.assets/icons/chrome.svg
--rw-rw-rw-   0        0        0      253 2023-03-18 18:50:21.000000 aioqui-2.0.0/src/aioqui/.assets/icons/circle.svg
--rw-rw-rw-   0        0        0      366 2023-03-18 18:50:21.000000 aioqui-2.0.0/src/aioqui/.assets/icons/clipboard.svg
--rw-rw-rw-   0        0        0      299 2023-03-18 18:50:21.000000 aioqui-2.0.0/src/aioqui/.assets/icons/clock.svg
--rw-rw-rw-   0        0        0      552 2023-03-18 18:50:21.000000 aioqui-2.0.0/src/aioqui/.assets/icons/cloud-drizzle.svg
--rw-rw-rw-   0        0        0      340 2023-03-18 18:50:21.000000 aioqui-2.0.0/src/aioqui/.assets/icons/cloud-lightning.svg
--rw-rw-rw-   0        0        0      366 2023-03-18 18:50:21.000000 aioqui-2.0.0/src/aioqui/.assets/icons/cloud-off.svg
--rw-rw-rw-   0        0        0      416 2023-03-18 18:50:21.000000 aioqui-2.0.0/src/aioqui/.assets/icons/cloud-rain.svg
--rw-rw-rw-   0        0        0      567 2023-03-18 18:50:21.000000 aioqui-2.0.0/src/aioqui/.assets/icons/cloud-snow.svg
--rw-rw-rw-   0        0        0      275 2023-03-18 18:50:21.000000 aioqui-2.0.0/src/aioqui/.assets/icons/cloud.svg
--rw-rw-rw-   0        0        0      302 2023-03-18 18:50:21.000000 aioqui-2.0.0/src/aioqui/.assets/icons/code.svg
--rw-rw-rw-   0        0        0      481 2023-03-18 18:50:21.000000 aioqui-2.0.0/src/aioqui/.assets/icons/codepen.svg
--rw-rw-rw-   0        0        0      633 2023-03-18 18:50:21.000000 aioqui-2.0.0/src/aioqui/.assets/icons/codesandbox.svg
--rw-rw-rw-   0        0        0      442 2023-03-18 18:50:21.000000 aioqui-2.0.0/src/aioqui/.assets/icons/coffee.svg
--rw-rw-rw-   0        0        0      321 2023-03-18 18:50:21.000000 aioqui-2.0.0/src/aioqui/.assets/icons/columns.svg
--rw-rw-rw-   0        0        0      416 2023-03-18 18:50:21.000000 aioqui-2.0.0/src/aioqui/.assets/icons/command.svg
--rw-rw-rw-   0        0        0      337 2023-03-18 18:50:21.000000 aioqui-2.0.0/src/aioqui/.assets/icons/compass.svg
--rw-rw-rw-   0        0        0      346 2023-03-18 18:50:21.000000 aioqui-2.0.0/src/aioqui/.assets/icons/copy.svg
--rw-rw-rw-   0        0        0      309 2023-03-18 18:50:21.000000 aioqui-2.0.0/src/aioqui/.assets/icons/corner-down-left.svg
--rw-rw-rw-   0        0        0      313 2023-03-18 18:50:21.000000 aioqui-2.0.0/src/aioqui/.assets/icons/corner-down-right.svg
--rw-rw-rw-   0        0        0      312 2023-03-18 18:50:21.000000 aioqui-2.0.0/src/aioqui/.assets/icons/corner-left-down.svg
--rw-rw-rw-   0        0        0      307 2023-03-18 18:50:21.000000 aioqui-2.0.0/src/aioqui/.assets/icons/corner-left-up.svg
--rw-rw-rw-   0        0        0      313 2023-03-18 18:50:21.000000 aioqui-2.0.0/src/aioqui/.assets/icons/corner-right-down.svg
--rw-rw-rw-   0        0        0      308 2023-03-18 18:50:21.000000 aioqui-2.0.0/src/aioqui/.assets/icons/corner-right-up.svg
--rw-rw-rw-   0        0        0      307 2023-03-18 18:50:21.000000 aioqui-2.0.0/src/aioqui/.assets/icons/corner-up-left.svg
--rw-rw-rw-   0        0        0      311 2023-03-18 18:50:21.000000 aioqui-2.0.0/src/aioqui/.assets/icons/corner-up-right.svg
--rw-rw-rw-   0        0        0      662 2023-03-18 18:50:21.000000 aioqui-2.0.0/src/aioqui/.assets/icons/cpu.svg
--rw-rw-rw-   0        0        0      324 2023-03-18 18:50:21.000000 aioqui-2.0.0/src/aioqui/.assets/icons/credit-card.svg
--rw-rw-rw-   0        0        0      305 2023-03-18 18:50:21.000000 aioqui-2.0.0/src/aioqui/.assets/icons/crop.svg
--rw-rw-rw-   0        0        0      432 2023-03-18 18:50:21.000000 aioqui-2.0.0/src/aioqui/.assets/icons/crosshair.svg
--rw-rw-rw-   0        0        0      367 2023-03-18 18:50:21.000000 aioqui-2.0.0/src/aioqui/.assets/icons/database.svg
--rw-rw-rw-   0        0        0      369 2023-03-18 18:50:21.000000 aioqui-2.0.0/src/aioqui/.assets/icons/delete.svg
--rw-rw-rw-   0        0        0      290 2023-03-18 18:50:21.000000 aioqui-2.0.0/src/aioqui/.assets/icons/disc.svg
--rw-rw-rw-   0        0        0      392 2023-03-18 18:50:21.000000 aioqui-2.0.0/src/aioqui/.assets/icons/divide-circle.svg
--rw-rw-rw-   0        0        0      414 2023-03-18 18:50:21.000000 aioqui-2.0.0/src/aioqui/.assets/icons/divide-square.svg
--rw-rw-rw-   0        0        0      334 2023-03-18 18:50:21.000000 aioqui-2.0.0/src/aioqui/.assets/icons/divide.svg
--rw-rw-rw-   0        0        0      329 2023-03-18 18:50:21.000000 aioqui-2.0.0/src/aioqui/.assets/icons/dollar-sign.svg
--rw-rw-rw-   0        0        0      382 2023-03-18 18:50:21.000000 aioqui-2.0.0/src/aioqui/.assets/icons/download-cloud.svg
--rw-rw-rw-   0        0        0      365 2023-03-18 18:50:21.000000 aioqui-2.0.0/src/aioqui/.assets/icons/download.svg
--rw-rw-rw-   0        0        0      419 2023-03-18 18:50:21.000000 aioqui-2.0.0/src/aioqui/.assets/icons/dribbble.svg
--rw-rw-rw-   0        0        0      269 2023-03-18 18:50:21.000000 aioqui-2.0.0/src/aioqui/.assets/icons/droplet.svg
--rw-rw-rw-   0        0        0      286 2023-03-18 18:50:21.000000 aioqui-2.0.0/src/aioqui/.assets/icons/edit-2.svg
--rw-rw-rw-   0        0        0      312 2023-03-18 18:50:21.000000 aioqui-2.0.0/src/aioqui/.assets/icons/edit-3.svg
--rw-rw-rw-   0        0        0      360 2023-03-18 18:50:21.000000 aioqui-2.0.0/src/aioqui/.assets/icons/edit.svg
--rw-rw-rw-   0        0        0      383 2023-03-18 18:50:21.000000 aioqui-2.0.0/src/aioqui/.assets/icons/external-link.svg
--rw-rw-rw-   0        0        0      455 2023-03-18 18:50:21.000000 aioqui-2.0.0/src/aioqui/.assets/icons/eye-off.svg
--rw-rw-rw-   0        0        0      311 2023-03-18 18:50:21.000000 aioqui-2.0.0/src/aioqui/.assets/icons/eye.svg
--rw-rw-rw-   0        0        0      298 2023-03-18 18:50:21.000000 aioqui-2.0.0/src/aioqui/.assets/icons/facebook.svg
--rw-rw-rw-   0        0        0      318 2023-03-18 18:50:21.000000 aioqui-2.0.0/src/aioqui/.assets/icons/fast-forward.svg
--rw-rw-rw-   0        0        0      368 2023-03-18 18:50:21.000000 aioqui-2.0.0/src/aioqui/.assets/icons/feather.svg
--rw-rw-rw-   0        0        0      548 2023-03-18 18:50:21.000000 aioqui-2.0.0/src/aioqui/.assets/icons/figma.svg
--rw-rw-rw-   0        0        0      382 2023-03-18 18:50:21.000000 aioqui-2.0.0/src/aioqui/.assets/icons/file-minus.svg
--rw-rw-rw-   0        0        0      426 2023-03-18 18:50:21.000000 aioqui-2.0.0/src/aioqui/.assets/icons/file-plus.svg
--rw-rw-rw-   0        0        0      468 2023-03-18 18:50:21.000000 aioqui-2.0.0/src/aioqui/.assets/icons/file-text.svg
--rw-rw-rw-   0        0        0      332 2023-03-18 18:50:21.000000 aioqui-2.0.0/src/aioqui/.assets/icons/file.svg
--rw-rw-rw-   0        0        0      581 2023-03-18 18:50:21.000000 aioqui-2.0.0/src/aioqui/.assets/icons/film.svg
--rw-rw-rw-   0        0        0      285 2023-03-18 18:50:21.000000 aioqui-2.0.0/src/aioqui/.assets/icons/filter.svg
--rw-rw-rw-   0        0        0      329 2023-03-18 18:50:21.000000 aioqui-2.0.0/src/aioqui/.assets/icons/flag.svg
--rw-rw-rw-   0        0        0      356 2023-03-18 18:50:21.000000 aioqui-2.0.0/src/aioqui/.assets/icons/folder-minus.svg
--rw-rw-rw-   0        0        0      400 2023-03-18 18:50:21.000000 aioqui-2.0.0/src/aioqui/.assets/icons/folder-plus.svg
--rw-rw-rw-   0        0        0      306 2023-03-18 18:50:21.000000 aioqui-2.0.0/src/aioqui/.assets/icons/folder.svg
--rw-rw-rw-   0        0        0      273 2023-03-18 18:50:21.000000 aioqui-2.0.0/src/aioqui/.assets/icons/framer.svg
--rw-rw-rw-   0        0        0      385 2023-03-18 18:50:21.000000 aioqui-2.0.0/src/aioqui/.assets/icons/frown.svg
--rw-rw-rw-   0        0        0      476 2023-03-18 18:50:21.000000 aioqui-2.0.0/src/aioqui/.assets/icons/gift.svg
--rw-rw-rw-   0        0        0      372 2023-03-18 18:50:21.000000 aioqui-2.0.0/src/aioqui/.assets/icons/git-branch.svg
--rw-rw-rw-   0        0        0      353 2023-03-18 18:50:21.000000 aioqui-2.0.0/src/aioqui/.assets/icons/git-commit.svg
--rw-rw-rw-   0        0        0      331 2023-03-18 18:50:21.000000 aioqui-2.0.0/src/aioqui/.assets/icons/git-merge.svg
--rw-rw-rw-   0        0        0      382 2023-03-18 18:50:21.000000 aioqui-2.0.0/src/aioqui/.assets/icons/git-pull-request.svg
--rw-rw-rw-   0        0        0      522 2023-03-18 18:50:21.000000 aioqui-2.0.0/src/aioqui/.assets/icons/github.svg
--rw-rw-rw-   0        0        0      485 2023-03-18 18:50:21.000000 aioqui-2.0.0/src/aioqui/.assets/icons/gitlab.svg
--rw-rw-rw-   0        0        0      404 2023-03-18 18:50:21.000000 aioqui-2.0.0/src/aioqui/.assets/icons/globe.svg
--rw-rw-rw-   0        0        0      399 2023-03-18 18:50:21.000000 aioqui-2.0.0/src/aioqui/.assets/icons/grid.svg
--rw-rw-rw-   0        0        0      479 2023-03-18 18:50:21.000000 aioqui-2.0.0/src/aioqui/.assets/icons/hard-drive.svg
--rw-rw-rw-   0        0        0      384 2023-03-18 18:50:21.000000 aioqui-2.0.0/src/aioqui/.assets/icons/hash.svg
--rw-rw-rw-   0        0        0      390 2023-03-18 18:50:21.000000 aioqui-2.0.0/src/aioqui/.assets/icons/headphones.svg
--rw-rw-rw-   0        0        0      366 2023-03-18 18:50:21.000000 aioqui-2.0.0/src/aioqui/.assets/icons/heart.svg
--rw-rw-rw-   0        0        0      360 2023-03-18 18:50:21.000000 aioqui-2.0.0/src/aioqui/.assets/icons/help-circle.svg
--rw-rw-rw-   0        0        0      353 2023-03-18 18:50:21.000000 aioqui-2.0.0/src/aioqui/.assets/icons/hexagon.svg
--rw-rw-rw-   0        0        0      327 2023-03-18 18:50:21.000000 aioqui-2.0.0/src/aioqui/.assets/icons/home.svg
--rw-rw-rw-   0        0        0      364 2023-03-18 18:50:21.000000 aioqui-2.0.0/src/aioqui/.assets/icons/image.svg
--rw-rw-rw-   0        0        0      400 2023-03-18 18:50:21.000000 aioqui-2.0.0/src/aioqui/.assets/icons/inbox.svg
--rw-rw-rw-   0        0        0      342 2023-03-18 18:50:21.000000 aioqui-2.0.0/src/aioqui/.assets/icons/info.svg
--rw-rw-rw-   0        0        0      395 2023-03-18 18:50:21.000000 aioqui-2.0.0/src/aioqui/.assets/icons/instagram.svg
--rw-rw-rw-   0        0        0      343 2023-03-18 18:50:21.000000 aioqui-2.0.0/src/aioqui/.assets/icons/italic.svg
--rw-rw-rw-   0        0        0      347 2023-03-18 18:50:21.000000 aioqui-2.0.0/src/aioqui/.assets/icons/key.svg
--rw-rw-rw-   0        0        0      360 2023-03-18 18:50:21.000000 aioqui-2.0.0/src/aioqui/.assets/icons/layers.svg
--rw-rw-rw-   0        0        0      359 2023-03-18 18:50:21.000000 aioqui-2.0.0/src/aioqui/.assets/icons/layout.svg
--rw-rw-rw-   0        0        0      570 2023-03-18 18:50:21.000000 aioqui-2.0.0/src/aioqui/.assets/icons/life-buoy.svg
--rw-rw-rw-   0        0        0      350 2023-03-18 18:50:21.000000 aioqui-2.0.0/src/aioqui/.assets/icons/link-2.svg
--rw-rw-rw-   0        0        0      366 2023-03-18 18:50:21.000000 aioqui-2.0.0/src/aioqui/.assets/icons/link.svg
--rw-rw-rw-   0        0        0      395 2023-03-18 18:50:21.000000 aioqui-2.0.0/src/aioqui/.assets/icons/linkedin.svg
--rw-rw-rw-   0        0        0      477 2023-03-18 18:50:21.000000 aioqui-2.0.0/src/aioqui/.assets/icons/list.svg
--rw-rw-rw-   0        0        0      609 2023-03-18 18:50:21.000000 aioqui-2.0.0/src/aioqui/.assets/icons/loader.svg
--rw-rw-rw-   0        0        0      316 2023-03-18 18:50:21.000000 aioqui-2.0.0/src/aioqui/.assets/icons/lock.svg
--rw-rw-rw-   0        0        0      363 2023-03-18 18:50:21.000000 aioqui-2.0.0/src/aioqui/.assets/icons/log-in.svg
--rw-rw-rw-   0        0        0      362 2023-03-18 18:50:21.000000 aioqui-2.0.0/src/aioqui/.assets/icons/log-out.svg
--rw-rw-rw-   0        0        0      349 2023-03-18 18:50:21.000000 aioqui-2.0.0/src/aioqui/.assets/icons/mail.svg
--rw-rw-rw-   0        0        0      317 2023-03-18 18:50:21.000000 aioqui-2.0.0/src/aioqui/.assets/icons/map-pin.svg
--rw-rw-rw-   0        0        0      368 2023-03-18 18:50:21.000000 aioqui-2.0.0/src/aioqui/.assets/icons/map.svg
--rw-rw-rw-   0        0        0      395 2023-03-18 18:50:21.000000 aioqui-2.0.0/src/aioqui/.assets/icons/maximize-2.svg
--rw-rw-rw-   0        0        0      326 2023-03-18 18:50:21.000000 aioqui-2.0.0/src/aioqui/.assets/icons/maximize.svg
--rw-rw-rw-   0        0        0      384 2023-03-18 18:50:21.000000 aioqui-2.0.0/src/aioqui/.assets/icons/meh.svg
--rw-rw-rw-   0        0        0      341 2023-03-18 18:50:21.000000 aioqui-2.0.0/src/aioqui/.assets/icons/menu.svg
--rw-rw-rw-   0        0        0      423 2023-03-18 18:50:21.000000 aioqui-2.0.0/src/aioqui/.assets/icons/message-circle.svg
--rw-rw-rw-   0        0        0      300 2023-03-18 18:50:21.000000 aioqui-2.0.0/src/aioqui/.assets/icons/message-square.svg
--rw-rw-rw-   0        0        0      489 2023-03-18 18:50:21.000000 aioqui-2.0.0/src/aioqui/.assets/icons/mic-off.svg
--rw-rw-rw-   0        0        0      413 2023-03-18 18:50:21.000000 aioqui-2.0.0/src/aioqui/.assets/icons/mic.svg
--rw-rw-rw-   0        0        0      399 2023-03-18 18:50:21.000000 aioqui-2.0.0/src/aioqui/.assets/icons/minimize-2.svg
--rw-rw-rw-   0        0        0      326 2023-03-18 18:50:21.000000 aioqui-2.0.0/src/aioqui/.assets/icons/minimize.svg
--rw-rw-rw-   0        0        0      303 2023-03-18 18:50:21.000000 aioqui-2.0.0/src/aioqui/.assets/icons/minus-circle.svg
--rw-rw-rw-   0        0        0      325 2023-03-18 18:50:21.000000 aioqui-2.0.0/src/aioqui/.assets/icons/minus-square.svg
--rw-rw-rw-   0        0        0      256 2023-03-18 18:50:21.000000 aioqui-2.0.0/src/aioqui/.assets/icons/minus.svg
--rw-rw-rw-   0        0        0      365 2023-03-18 18:50:21.000000 aioqui-2.0.0/src/aioqui/.assets/icons/monitor.svg
--rw-rw-rw-   0        0        0      276 2023-03-18 18:50:21.000000 aioqui-2.0.0/src/aioqui/.assets/icons/moon.svg
--rw-rw-rw-   0        0        0      338 2023-03-18 18:50:21.000000 aioqui-2.0.0/src/aioqui/.assets/icons/more-horizontal.svg
--rw-rw-rw-   0        0        0      336 2023-03-18 18:50:21.000000 aioqui-2.0.0/src/aioqui/.assets/icons/more-vertical.svg
--rw-rw-rw-   0        0        0      306 2023-03-18 18:50:21.000000 aioqui-2.0.0/src/aioqui/.assets/icons/mouse-pointer.svg
--rw-rw-rw-   0        0        0      481 2023-03-18 18:50:21.000000 aioqui-2.0.0/src/aioqui/.assets/icons/move.svg
--rw-rw-rw-   0        0        0      322 2023-03-18 18:50:21.000000 aioqui-2.0.0/src/aioqui/.assets/icons/music.svg
--rw-rw-rw-   0        0        0      274 2023-03-18 18:50:21.000000 aioqui-2.0.0/src/aioqui/.assets/icons/navigation-2.svg
--rw-rw-rw-   0        0        0      272 2023-03-18 18:50:21.000000 aioqui-2.0.0/src/aioqui/.assets/icons/navigation.svg
--rw-rw-rw-   0        0        0      313 2023-03-18 18:50:21.000000 aioqui-2.0.0/src/aioqui/.assets/icons/octagon.svg
--rw-rw-rw-   0        0        0      512 2023-03-18 18:50:21.000000 aioqui-2.0.0/src/aioqui/.assets/icons/package.svg
--rw-rw-rw-   0        0        0      347 2023-03-18 18:50:21.000000 aioqui-2.0.0/src/aioqui/.assets/icons/paperclip.svg
--rw-rw-rw-   0        0        0      347 2023-03-18 18:50:21.000000 aioqui-2.0.0/src/aioqui/.assets/icons/pause-circle.svg
--rw-rw-rw-   0        0        0      307 2023-03-18 18:50:21.000000 aioqui-2.0.0/src/aioqui/.assets/icons/pause.svg
--rw-rw-rw-   0        0        0      386 2023-03-18 18:50:21.000000 aioqui-2.0.0/src/aioqui/.assets/icons/pen-tool.svg
--rw-rw-rw-   0        0        0      345 2023-03-18 18:50:21.000000 aioqui-2.0.0/src/aioqui/.assets/icons/percent.svg
--rw-rw-rw-   0        0        0      571 2023-03-18 18:50:21.000000 aioqui-2.0.0/src/aioqui/.assets/icons/phone-call.svg
--rw-rw-rw-   0        0        0      613 2023-03-18 18:50:21.000000 aioqui-2.0.0/src/aioqui/.assets/icons/phone-forwarded.svg
--rw-rw-rw-   0        0        0      612 2023-03-18 18:50:21.000000 aioqui-2.0.0/src/aioqui/.assets/icons/phone-incoming.svg
--rw-rw-rw-   0        0        0      608 2023-03-18 18:50:21.000000 aioqui-2.0.0/src/aioqui/.assets/icons/phone-missed.svg
--rw-rw-rw-   0        0        0      586 2023-03-18 18:50:21.000000 aioqui-2.0.0/src/aioqui/.assets/icons/phone-off.svg
--rw-rw-rw-   0        0        0      612 2023-03-18 18:50:21.000000 aioqui-2.0.0/src/aioqui/.assets/icons/phone-outgoing.svg
--rw-rw-rw-   0        0        0      515 2023-03-18 18:50:21.000000 aioqui-2.0.0/src/aioqui/.assets/icons/phone.svg
--rw-rw-rw-   0        0        0      310 2023-03-18 18:50:21.000000 aioqui-2.0.0/src/aioqui/.assets/icons/pie-chart.svg
--rw-rw-rw-   0        0        0      308 2023-03-18 18:50:21.000000 aioqui-2.0.0/src/aioqui/.assets/icons/play-circle.svg
--rw-rw-rw-   0        0        0      258 2023-03-18 18:50:21.000000 aioqui-2.0.0/src/aioqui/.assets/icons/play.svg
--rw-rw-rw-   0        0        0      345 2023-03-18 18:50:21.000000 aioqui-2.0.0/src/aioqui/.assets/icons/plus-circle-gray.svg
--rw-rw-rw-   0        0        0      346 2023-03-18 18:50:21.000000 aioqui-2.0.0/src/aioqui/.assets/icons/plus-circle.svg
--rw-rw-rw-   0        0        0      368 2023-03-18 18:50:21.000000 aioqui-2.0.0/src/aioqui/.assets/icons/plus-square.svg
--rw-rw-rw-   0        0        0      299 2023-03-18 18:50:21.000000 aioqui-2.0.0/src/aioqui/.assets/icons/plus.svg
--rw-rw-rw-   0        0        0      353 2023-03-18 18:50:21.000000 aioqui-2.0.0/src/aioqui/.assets/icons/pocket.svg
--rw-rw-rw-   0        0        0      303 2023-03-18 18:50:21.000000 aioqui-2.0.0/src/aioqui/.assets/icons/power.svg
--rw-rw-rw-   0        0        0      402 2023-03-18 18:50:21.000000 aioqui-2.0.0/src/aioqui/.assets/icons/printer.svg
--rw-rw-rw-   0        0        0      384 2023-03-18 18:50:21.000000 aioqui-2.0.0/src/aioqui/.assets/icons/radio.svg
--rw-rw-rw-   0        0        0      395 2023-03-18 18:50:21.000000 aioqui-2.0.0/src/aioqui/.assets/icons/refresh-ccw.svg
--rw-rw-rw-   0        0        0      395 2023-03-18 18:50:21.000000 aioqui-2.0.0/src/aioqui/.assets/icons/refresh-cw.svg
--rw-rw-rw-   0        0        0      387 2023-03-18 18:50:21.000000 aioqui-2.0.0/src/aioqui/.assets/icons/repeat.svg
--rw-rw-rw-   0        0        0      314 2023-03-18 18:50:21.000000 aioqui-2.0.0/src/aioqui/.assets/icons/rewind.svg
--rw-rw-rw-   0        0        0      312 2023-03-18 18:50:21.000000 aioqui-2.0.0/src/aioqui/.assets/icons/rotate-ccw.svg
--rw-rw-rw-   0        0        0      316 2023-03-18 18:50:21.000000 aioqui-2.0.0/src/aioqui/.assets/icons/rotate-cw.svg
--rw-rw-rw-   0        0        0      325 2023-03-18 18:50:21.000000 aioqui-2.0.0/src/aioqui/.assets/icons/rss.svg
--rw-rw-rw-   0        0        0      387 2023-03-18 18:50:21.000000 aioqui-2.0.0/src/aioqui/.assets/icons/save.svg
--rw-rw-rw-   0        0        0      366 2023-03-18 18:50:21.000000 aioqui-2.0.0/src/aioqui/.assets/icons/schedule.svg
--rw-rw-rw-   0        0        0      439 2023-03-18 18:50:21.000000 aioqui-2.0.0/src/aioqui/.assets/icons/scissors.svg
--rw-rw-rw-   0        0        0      303 2023-03-18 18:50:21.000000 aioqui-2.0.0/src/aioqui/.assets/icons/search.svg
--rw-rw-rw-   0        0        0      309 2023-03-18 18:50:21.000000 aioqui-2.0.0/src/aioqui/.assets/icons/send.svg
--rw-rw-rw-   0        0        0      426 2023-03-18 18:50:21.000000 aioqui-2.0.0/src/aioqui/.assets/icons/server.svg
--rw-rw-rw-   0        0        0     1006 2023-03-18 18:50:21.000000 aioqui-2.0.0/src/aioqui/.assets/icons/settings.svg
--rw-rw-rw-   0        0        0      440 2023-03-18 18:50:21.000000 aioqui-2.0.0/src/aioqui/.assets/icons/share-2.svg
--rw-rw-rw-   0        0        0      359 2023-03-18 18:50:21.000000 aioqui-2.0.0/src/aioqui/.assets/icons/share.svg
--rw-rw-rw-   0        0        0      400 2023-03-18 18:50:21.000000 aioqui-2.0.0/src/aioqui/.assets/icons/shield-off.svg
--rw-rw-rw-   0        0        0      274 2023-03-18 18:50:21.000000 aioqui-2.0.0/src/aioqui/.assets/icons/shield.svg
--rw-rw-rw-   0        0        0      367 2023-03-18 18:50:21.000000 aioqui-2.0.0/src/aioqui/.assets/icons/shopping-bag.svg
--rw-rw-rw-   0        0        0      378 2023-03-18 18:50:21.000000 aioqui-2.0.0/src/aioqui/.assets/icons/shopping-cart.svg
--rw-rw-rw-   0        0        0      436 2023-03-18 18:50:21.000000 aioqui-2.0.0/src/aioqui/.assets/icons/shuffle.svg
--rw-rw-rw-   0        0        0      318 2023-03-18 18:50:21.000000 aioqui-2.0.0/src/aioqui/.assets/icons/sidebar.svg
--rw-rw-rw-   0        0        0      308 2023-03-18 18:50:21.000000 aioqui-2.0.0/src/aioqui/.assets/icons/skip-back.svg
--rw-rw-rw-   0        0        0      310 2023-03-18 18:50:21.000000 aioqui-2.0.0/src/aioqui/.assets/icons/skip-forward.svg
--rw-rw-rw-   0        0        0      994 2023-03-18 18:50:21.000000 aioqui-2.0.0/src/aioqui/.assets/icons/slack.svg
--rw-rw-rw-   0        0        0      307 2023-03-18 18:50:21.000000 aioqui-2.0.0/src/aioqui/.assets/icons/slash.svg
--rw-rw-rw-   0        0        0      606 2023-03-18 18:50:21.000000 aioqui-2.0.0/src/aioqui/.assets/icons/sliders.svg
--rw-rw-rw-   0        0        0      327 2023-03-18 18:50:21.000000 aioqui-2.0.0/src/aioqui/.assets/icons/smartphone.svg
--rw-rw-rw-   0        0        0      383 2023-03-18 18:50:21.000000 aioqui-2.0.0/src/aioqui/.assets/icons/smile.svg
--rw-rw-rw-   0        0        0      361 2023-03-18 18:50:21.000000 aioqui-2.0.0/src/aioqui/.assets/icons/speaker.svg
--rw-rw-rw-   0        0        0      275 2023-03-18 18:50:21.000000 aioqui-2.0.0/src/aioqui/.assets/icons/square.svg
--rw-rw-rw-   0        0        0      391 2023-04-06 21:10:35.000000 aioqui-2.0.0/src/aioqui/.assets/icons/star-fill.svg
--rw-rw-rw-   0        0        0      334 2023-03-18 18:50:21.000000 aioqui-2.0.0/src/aioqui/.assets/icons/star.svg
--rw-rw-rw-   0        0        0      304 2023-03-18 18:50:21.000000 aioqui-2.0.0/src/aioqui/.assets/icons/stop-circle.svg
--rw-rw-rw-   0        0        0      645 2023-03-18 18:50:21.000000 aioqui-2.0.0/src/aioqui/.assets/icons/sun.svg
--rw-rw-rw-   0        0        0      584 2023-03-18 18:50:21.000000 aioqui-2.0.0/src/aioqui/.assets/icons/sunrise.svg
--rw-rw-rw-   0        0        0      583 2023-03-18 18:50:21.000000 aioqui-2.0.0/src/aioqui/.assets/icons/sunset.svg
--rw-rw-rw-   0        0        0      335 2023-03-18 18:50:21.000000 aioqui-2.0.0/src/aioqui/.assets/icons/table.svg
--rw-rw-rw-   0        0        0      323 2023-03-18 18:50:21.000000 aioqui-2.0.0/src/aioqui/.assets/icons/tablet.svg
--rw-rw-rw-   0        0        0      350 2023-03-18 18:50:21.000000 aioqui-2.0.0/src/aioqui/.assets/icons/tag.svg
--rw-rw-rw-   0        0        0      331 2023-03-18 18:50:21.000000 aioqui-2.0.0/src/aioqui/.assets/icons/target.svg
--rw-rw-rw-   0        0        0      305 2023-03-18 18:50:21.000000 aioqui-2.0.0/src/aioqui/.assets/icons/terminal.svg
--rw-rw-rw-   0        0        0      292 2023-03-18 18:50:21.000000 aioqui-2.0.0/src/aioqui/.assets/icons/thermometer.svg
--rw-rw-rw-   0        0        0      369 2023-03-18 18:50:21.000000 aioqui-2.0.0/src/aioqui/.assets/icons/thumbs-down.svg
--rw-rw-rw-   0        0        0      349 2023-03-18 18:50:21.000000 aioqui-2.0.0/src/aioqui/.assets/icons/thumbs-up.svg
--rw-rw-rw-   0        0        0      318 2023-03-18 18:50:21.000000 aioqui-2.0.0/src/aioqui/.assets/icons/toggle-left.svg
--rw-rw-rw-   0        0        0      320 2023-03-18 18:50:21.000000 aioqui-2.0.0/src/aioqui/.assets/icons/toggle-right.svg
--rw-rw-rw-   0        0        0      381 2023-03-18 18:50:21.000000 aioqui-2.0.0/src/aioqui/.assets/icons/tool.svg
--rw-rw-rw-   0        0        0      443 2023-03-18 18:50:21.000000 aioqui-2.0.0/src/aioqui/.assets/icons/trash-2.svg
--rw-rw-rw-   0        0        0      351 2023-03-18 18:50:21.000000 aioqui-2.0.0/src/aioqui/.assets/icons/trash.svg
--rw-rw-rw-   0        0        0      368 2023-03-18 18:50:21.000000 aioqui-2.0.0/src/aioqui/.assets/icons/trello.svg
--rw-rw-rw-   0        0        0      326 2023-03-18 18:50:21.000000 aioqui-2.0.0/src/aioqui/.assets/icons/trending-down.svg
--rw-rw-rw-   0        0        0      323 2023-03-18 18:50:21.000000 aioqui-2.0.0/src/aioqui/.assets/icons/trending-up.svg
--rw-rw-rw-   0        0        0      321 2023-03-18 18:50:21.000000 aioqui-2.0.0/src/aioqui/.assets/icons/triangle.svg
--rw-rw-rw-   0        0        0      410 2023-03-18 18:50:21.000000 aioqui-2.0.0/src/aioqui/.assets/icons/truck.svg
--rw-rw-rw-   0        0        0      315 2023-03-18 18:50:21.000000 aioqui-2.0.0/src/aioqui/.assets/icons/tv.svg
--rw-rw-rw-   0        0        0      272 2023-03-18 18:50:21.000000 aioqui-2.0.0/src/aioqui/.assets/icons/twitch.svg
--rw-rw-rw-   0        0        0      403 2023-03-18 18:50:21.000000 aioqui-2.0.0/src/aioqui/.assets/icons/twitter.svg
--rw-rw-rw-   0        0        0      347 2023-03-18 18:50:21.000000 aioqui-2.0.0/src/aioqui/.assets/icons/type.svg
--rw-rw-rw-   0        0        0      285 2023-03-18 18:50:21.000000 aioqui-2.0.0/src/aioqui/.assets/icons/umbrella.svg
--rw-rw-rw-   0        0        0      314 2023-03-18 18:50:21.000000 aioqui-2.0.0/src/aioqui/.assets/icons/underline.svg
--rw-rw-rw-   0        0        0      317 2023-03-18 18:50:21.000000 aioqui-2.0.0/src/aioqui/.assets/icons/unlock.svg
--rw-rw-rw-   0        0        0      426 2023-03-18 18:50:21.000000 aioqui-2.0.0/src/aioqui/.assets/icons/upload-cloud.svg
--rw-rw-rw-   0        0        0      360 2023-03-18 18:50:21.000000 aioqui-2.0.0/src/aioqui/.assets/icons/upload.svg
--rw-rw-rw-   0        0        0      362 2023-03-18 18:50:21.000000 aioqui-2.0.0/src/aioqui/.assets/icons/user-check.svg
--rw-rw-rw-   0        0        0      360 2023-03-18 18:50:21.000000 aioqui-2.0.0/src/aioqui/.assets/icons/user-minus.svg
--rw-rw-rw-   0        0        0      403 2023-03-18 18:50:21.000000 aioqui-2.0.0/src/aioqui/.assets/icons/user-plus.svg
--rw-rw-rw-   0        0        0      399 2023-03-18 18:50:21.000000 aioqui-2.0.0/src/aioqui/.assets/icons/user-x.svg
--rw-rw-rw-   0        0        0      308 2023-03-18 18:50:21.000000 aioqui-2.0.0/src/aioqui/.assets/icons/user.svg
--rw-rw-rw-   0        0        0      395 2023-03-18 18:50:21.000000 aioqui-2.0.0/src/aioqui/.assets/icons/users.svg
--rw-rw-rw-   0        0        0      374 2023-03-18 18:50:21.000000 aioqui-2.0.0/src/aioqui/.assets/icons/video-off.svg
--rw-rw-rw-   0        0        0      324 2023-03-18 18:50:21.000000 aioqui-2.0.0/src/aioqui/.assets/icons/video.svg
--rw-rw-rw-   0        0        0      353 2023-03-18 18:50:21.000000 aioqui-2.0.0/src/aioqui/.assets/icons/voicemail.svg
--rw-rw-rw-   0        0        0      323 2023-03-18 18:50:21.000000 aioqui-2.0.0/src/aioqui/.assets/icons/volume-1.svg
--rw-rw-rw-   0        0        0      354 2023-03-18 18:50:21.000000 aioqui-2.0.0/src/aioqui/.assets/icons/volume-2.svg
--rw-rw-rw-   0        0        0      365 2023-03-18 18:50:21.000000 aioqui-2.0.0/src/aioqui/.assets/icons/volume-x.svg
--rw-rw-rw-   0        0        0      275 2023-03-18 18:50:21.000000 aioqui-2.0.0/src/aioqui/.assets/icons/volume.svg
--rw-rw-rw-   0        0        0      457 2023-03-18 18:50:21.000000 aioqui-2.0.0/src/aioqui/.assets/icons/watch.svg
--rw-rw-rw-   0        0        0      564 2023-03-18 18:50:21.000000 aioqui-2.0.0/src/aioqui/.assets/icons/wifi-off.svg
--rw-rw-rw-   0        0        0      396 2023-03-18 18:50:21.000000 aioqui-2.0.0/src/aioqui/.assets/icons/wifi.svg
--rw-rw-rw-   0        0        0      321 2023-03-18 18:50:21.000000 aioqui-2.0.0/src/aioqui/.assets/icons/wind.svg
--rw-rw-rw-   0        0        0      340 2023-03-18 18:50:21.000000 aioqui-2.0.0/src/aioqui/.assets/icons/x-circle-gray.svg
--rw-rw-rw-   0        0        0      341 2023-03-18 18:50:21.000000 aioqui-2.0.0/src/aioqui/.assets/icons/x-circle.svg
--rw-rw-rw-   0        0        0      401 2023-03-18 18:50:21.000000 aioqui-2.0.0/src/aioqui/.assets/icons/x-octagon.svg
--rw-rw-rw-   0        0        0      363 2023-03-18 18:50:21.000000 aioqui-2.0.0/src/aioqui/.assets/icons/x-square.svg
--rw-rw-rw-   0        0        0      294 2023-03-18 18:50:21.000000 aioqui-2.0.0/src/aioqui/.assets/icons/x.svg
--rw-rw-rw-   0        0        0      560 2023-03-18 18:50:21.000000 aioqui-2.0.0/src/aioqui/.assets/icons/youtube.svg
--rw-rw-rw-   0        0        0      428 2023-03-18 18:50:21.000000 aioqui-2.0.0/src/aioqui/.assets/icons/zap-off.svg
--rw-rw-rw-   0        0        0      277 2023-03-18 18:50:21.000000 aioqui-2.0.0/src/aioqui/.assets/icons/zap.svg
--rw-rw-rw-   0        0        0      392 2023-03-18 18:50:21.000000 aioqui-2.0.0/src/aioqui/.assets/icons/zoom-in.svg
--rw-rw-rw-   0        0        0      349 2023-03-18 18:50:21.000000 aioqui-2.0.0/src/aioqui/.assets/icons/zoom-out.svg
--rw-rw-rw-   0        0        0      158 2023-05-15 07:06:29.000000 aioqui-2.0.0/src/aioqui/__init__.py
-drwxrwxrwx   0        0        0        0 2023-05-15 09:05:51.487507 aioqui-2.0.0/src/aioqui/context/
--rw-rw-rw-   0        0        0       70 2023-05-15 07:06:13.000000 aioqui-2.0.0/src/aioqui/context/__init__.py
--rw-rw-rw-   0        0        0     8784 2023-05-15 08:45:31.000000 aioqui-2.0.0/src/aioqui/context/context_obj.py
--rw-rw-rw-   0        0        0      443 2023-05-14 00:18:53.000000 aioqui-2.0.0/src/aioqui/context/contextapi.py
-drwxrwxrwx   0        0        0        0 2023-05-15 09:05:51.493507 aioqui-2.0.0/src/aioqui/enums/
--rw-rw-rw-   0        0        0      255 2023-05-15 05:17:48.000000 aioqui-2.0.0/src/aioqui/enums/__init__.py
--rw-rw-rw-   0        0        0      687 2023-05-13 23:00:29.000000 aioqui-2.0.0/src/aioqui/enums/alignment.py
--rw-rw-rw-   0        0        0      182 2023-05-15 05:17:48.000000 aioqui-2.0.0/src/aioqui/enums/echo_mode.py
--rw-rw-rw-   0        0        0      227 2023-05-14 07:18:50.000000 aioqui-2.0.0/src/aioqui/enums/elide_mode.py
--rw-rw-rw-   0        0        0      151 2023-05-13 23:00:29.000000 aioqui-2.0.0/src/aioqui/enums/orientation.py
--rw-rw-rw-   0        0        0      264 2023-05-14 00:48:52.000000 aioqui-2.0.0/src/aioqui/enums/scroll_policy.py
--rw-rw-rw-   0        0        0      235 2023-05-15 05:48:40.000000 aioqui-2.0.0/src/aioqui/enums/size_policy.py
--rw-rw-rw-   0        0        0      105 2023-05-13 23:00:29.000000 aioqui-2.0.0/src/aioqui/enums/window_hint.py
-drwxrwxrwx   0        0        0        0 2023-05-15 09:05:51.500507 aioqui-2.0.0/src/aioqui/misc/
--rw-rw-rw-   0        0        0      128 2023-05-15 08:51:32.000000 aioqui-2.0.0/src/aioqui/misc/__init__.py
--rw-rw-rw-   0        0        0     3736 2023-05-15 04:39:08.000000 aioqui-2.0.0/src/aioqui/misc/aiorequest.py
--rw-rw-rw-   0        0        0     1014 2023-05-15 09:02:15.000000 aioqui-2.0.0/src/aioqui/misc/animation.py
--rw-rw-rw-   0        0        0     1130 2023-05-15 08:41:25.000000 aioqui-2.0.0/src/aioqui/misc/conthrq.py
--rw-rw-rw-   0        0        0     1386 2023-05-14 18:16:30.000000 aioqui-2.0.0/src/aioqui/misc/fileops.py
--rw-rw-rw-   0        0        0     2181 2023-05-14 00:12:50.000000 aioqui-2.0.0/src/aioqui/misc/qss_parser.py
--rw-rw-rw-   0        0        0      319 2023-05-15 08:04:15.000000 aioqui-2.0.0/src/aioqui/misc/utils.py
--rw-rw-rw-   0        0        0      701 2023-05-14 00:40:28.000000 aioqui-2.0.0/src/aioqui/misc/uvithread.py
--rw-rw-rw-   0        0        0     1151 2023-05-15 05:37:56.000000 aioqui-2.0.0/src/aioqui/qasyncio.py
-drwxrwxrwx   0        0        0        0 2023-05-15 09:05:51.503507 aioqui-2.0.0/src/aioqui/types/
--rw-rw-rw-   0        0        0       71 2023-05-14 03:02:21.000000 aioqui-2.0.0/src/aioqui/types/__init__.py
--rw-rw-rw-   0        0        0      192 2023-05-15 07:18:29.000000 aioqui-2.0.0/src/aioqui/types/common.py
--rw-rw-rw-   0        0        0     3539 2023-05-14 00:07:05.000000 aioqui-2.0.0/src/aioqui/types/icon.py
--rw-rw-rw-   0        0        0      274 2023-04-20 15:54:13.000000 aioqui-2.0.0/src/aioqui/types/size.py
-drwxrwxrwx   0        0        0        0 2023-05-15 09:05:51.516509 aioqui-2.0.0/src/aioqui/widgets/
--rw-rw-rw-   0        0        0      616 2023-05-15 07:39:02.000000 aioqui-2.0.0/src/aioqui/widgets/__init__.py
--rw-rw-rw-   0        0        0      524 2023-05-15 08:10:27.000000 aioqui-2.0.0/src/aioqui/widgets/button.py
-drwxrwxrwx   0        0        0        0 2023-05-15 09:05:51.523514 aioqui-2.0.0/src/aioqui/widgets/custom/
--rw-rw-rw-   0        0        0      259 2023-05-15 07:57:18.000000 aioqui-2.0.0/src/aioqui/widgets/custom/__init__.py
--rw-rw-rw-   0        0        0     5695 2023-05-15 08:00:01.000000 aioqui-2.0.0/src/aioqui/widgets/custom/date_picker.py
--rw-rw-rw-   0        0        0     1939 2023-05-15 09:01:44.000000 aioqui-2.0.0/src/aioqui/widgets/custom/error_label.py
--rw-rw-rw-   0        0        0     2648 2023-05-15 07:57:46.000000 aioqui-2.0.0/src/aioqui/widgets/custom/image_button.py
--rw-rw-rw-   0        0        0     1423 2023-05-15 07:46:33.000000 aioqui-2.0.0/src/aioqui/widgets/custom/menu_button.py
--rw-rw-rw-   0        0        0     3961 2023-05-15 07:38:01.000000 aioqui-2.0.0/src/aioqui/widgets/custom/popup.py
--rw-rw-rw-   0        0        0     1027 2023-05-15 07:42:41.000000 aioqui-2.0.0/src/aioqui/widgets/custom/searchbar.py
--rw-rw-rw-   0        0        0     1877 2023-05-15 07:56:53.000000 aioqui-2.0.0/src/aioqui/widgets/custom/state_icon_btn.py
-drwxrwxrwx   0        0        0        0 2023-05-15 09:05:51.527508 aioqui-2.0.0/src/aioqui/widgets/extensions/
--rw-rw-rw-   0        0        0      160 2023-05-15 06:44:59.000000 aioqui-2.0.0/src/aioqui/widgets/extensions/__init__.py
--rw-rw-rw-   0        0        0      746 2023-05-15 06:52:42.000000 aioqui-2.0.0/src/aioqui/widgets/extensions/input_ext.py
--rw-rw-rw-   0        0        0     1944 2023-05-15 06:42:58.000000 aioqui-2.0.0/src/aioqui/widgets/extensions/layout_ext.py
--rw-rw-rw-   0        0        0      710 2023-05-15 06:28:17.000000 aioqui-2.0.0/src/aioqui/widgets/extensions/side_menu_ext.py
--rw-rw-rw-   0        0        0     1925 2023-05-15 05:30:53.000000 aioqui-2.0.0/src/aioqui/widgets/extensions/splitter_widget_ext.py
--rw-rw-rw-   0        0        0      667 2023-05-15 07:22:27.000000 aioqui-2.0.0/src/aioqui/widgets/frame.py
--rw-rw-rw-   0        0        0     2369 2023-05-15 07:40:44.000000 aioqui-2.0.0/src/aioqui/widgets/input.py
--rw-rw-rw-   0        0        0     1367 2023-05-15 07:43:50.000000 aioqui-2.0.0/src/aioqui/widgets/label.py
--rw-rw-rw-   0        0        0     1348 2023-05-15 07:41:20.000000 aioqui-2.0.0/src/aioqui/widgets/layout.py
--rw-rw-rw-   0        0        0     1736 2023-05-15 07:22:47.000000 aioqui-2.0.0/src/aioqui/widgets/scroll_area.py
--rw-rw-rw-   0        0        0     1184 2023-05-15 07:23:03.000000 aioqui-2.0.0/src/aioqui/widgets/selector.py
--rw-rw-rw-   0        0        0      862 2023-05-15 07:33:52.000000 aioqui-2.0.0/src/aioqui/widgets/slider.py
--rw-rw-rw-   0        0        0      270 2023-05-15 05:49:01.000000 aioqui-2.0.0/src/aioqui/widgets/spacer.py
--rw-rw-rw-   0        0        0     1580 2023-05-15 07:23:37.000000 aioqui-2.0.0/src/aioqui/widgets/splitter.py
--rw-rw-rw-   0        0        0     1159 2023-05-15 07:23:57.000000 aioqui-2.0.0/src/aioqui/widgets/stacked_widget.py
--rw-rw-rw-   0        0        0      327 2023-05-15 07:24:09.000000 aioqui-2.0.0/src/aioqui/widgets/statusbar.py
--rw-rw-rw-   0        0        0      587 2023-05-15 07:24:24.000000 aioqui-2.0.0/src/aioqui/widgets/widget.py
--rw-rw-rw-   0        0        0      516 2023-05-15 07:29:59.000000 aioqui-2.0.0/src/aioqui/widgets/window.py
-drwxrwxrwx   0        0        0        0 2023-05-15 09:05:51.227507 aioqui-2.0.0/src/aioqui.egg-info/
--rw-rw-rw-   0        0        0     2629 2023-05-15 09:05:51.000000 aioqui-2.0.0/src/aioqui.egg-info/PKG-INFO
--rw-rw-rw-   0        0        0    13091 2023-05-15 09:05:51.000000 aioqui-2.0.0/src/aioqui.egg-info/SOURCES.txt
--rw-rw-rw-   0        0        0        1 2023-05-15 09:05:51.000000 aioqui-2.0.0/src/aioqui.egg-info/dependency_links.txt
--rw-rw-rw-   0        0        0       44 2023-05-15 09:05:51.000000 aioqui-2.0.0/src/aioqui.egg-info/requires.txt
--rw-rw-rw-   0        0        0       16 2023-05-15 09:05:51.000000 aioqui-2.0.0/src/aioqui.egg-info/top_level.txt
+drwxrwxrwx   0        0        0        0 2023-05-16 21:21:00.701551 aioqui-2.0.1/
+-rw-rw-rw-   0        0        0     1093 2023-02-26 16:41:50.000000 aioqui-2.0.1/LICENSE.txt
+-rw-rw-rw-   0        0        0     2629 2023-05-16 21:21:00.701551 aioqui-2.0.1/PKG-INFO
+-rw-rw-rw-   0        0        0      282 2023-05-15 08:21:18.000000 aioqui-2.0.1/README.md
+-rw-rw-rw-   0        0        0     1488 2023-05-16 21:13:23.000000 aioqui-2.0.1/pyproject.toml
+-rw-rw-rw-   0        0        0       42 2023-05-16 21:21:00.701551 aioqui-2.0.1/setup.cfg
+drwxrwxrwx   0        0        0        0 2023-05-16 21:21:00.345984 aioqui-2.0.1/src/
+-rw-rw-rw-   0        0        0        0 2023-03-20 19:19:08.000000 aioqui-2.0.1/src/__init__.py
+drwxrwxrwx   0        0        0        0 2023-05-16 21:21:00.348982 aioqui-2.0.1/src/aioqui/
+drwxrwxrwx   0        0        0        0 2023-05-16 21:21:00.338985 aioqui-2.0.1/src/aioqui/.assets/
+drwxrwxrwx   0        0        0        0 2023-05-16 21:21:00.648549 aioqui-2.0.1/src/aioqui/.assets/icons/
+-rw-rw-rw-   0        0        0      277 2023-03-18 18:50:21.000000 aioqui-2.0.1/src/aioqui/.assets/icons/activity.svg
+-rw-rw-rw-   0        0        0      357 2023-03-18 18:50:21.000000 aioqui-2.0.1/src/aioqui/.assets/icons/airplay.svg
+-rw-rw-rw-   0        0        0      351 2023-03-18 18:50:21.000000 aioqui-2.0.1/src/aioqui/.assets/icons/alert-circle.svg
+-rw-rw-rw-   0        0        0      411 2023-03-18 18:50:21.000000 aioqui-2.0.1/src/aioqui/.assets/icons/alert-octagon.svg
+-rw-rw-rw-   0        0        0      419 2023-03-18 18:50:21.000000 aioqui-2.0.1/src/aioqui/.assets/icons/alert-triangle.svg
+-rw-rw-rw-   0        0        0      393 2023-03-18 18:50:21.000000 aioqui-2.0.1/src/aioqui/.assets/icons/align-center.svg
+-rw-rw-rw-   0        0        0      394 2023-03-18 18:50:21.000000 aioqui-2.0.1/src/aioqui/.assets/icons/align-justify.svg
+-rw-rw-rw-   0        0        0      391 2023-03-18 18:50:21.000000 aioqui-2.0.1/src/aioqui/.assets/icons/align-left.svg
+-rw-rw-rw-   0        0        0      392 2023-03-18 18:50:21.000000 aioqui-2.0.1/src/aioqui/.assets/icons/align-right.svg
+-rw-rw-rw-   0        0        0      340 2023-03-18 18:50:21.000000 aioqui-2.0.1/src/aioqui/.assets/icons/anchor.svg
+-rw-rw-rw-   0        0        0      563 2023-03-18 18:50:21.000000 aioqui-2.0.1/src/aioqui/.assets/icons/aperture.svg
+-rw-rw-rw-   0        0        0      356 2023-03-18 18:50:21.000000 aioqui-2.0.1/src/aioqui/.assets/icons/archive.svg
+-rw-rw-rw-   0        0        0      355 2023-03-18 18:50:21.000000 aioqui-2.0.1/src/aioqui/.assets/icons/arrow-down-circle.svg
+-rw-rw-rw-   0        0        0      310 2023-03-18 18:50:21.000000 aioqui-2.0.1/src/aioqui/.assets/icons/arrow-down-left.svg
+-rw-rw-rw-   0        0        0      312 2023-03-18 18:50:21.000000 aioqui-2.0.1/src/aioqui/.assets/icons/arrow-down-right.svg
+-rw-rw-rw-   0        0        0      308 2023-03-18 18:50:21.000000 aioqui-2.0.1/src/aioqui/.assets/icons/arrow-down.svg
+-rw-rw-rw-   0        0        0      354 2023-03-18 18:50:21.000000 aioqui-2.0.1/src/aioqui/.assets/icons/arrow-left-circle.svg
+-rw-rw-rw-   0        0        0      307 2023-03-18 18:50:21.000000 aioqui-2.0.1/src/aioqui/.assets/icons/arrow-left.svg
+-rw-rw-rw-   0        0        0      356 2023-03-18 18:50:21.000000 aioqui-2.0.1/src/aioqui/.assets/icons/arrow-right-circle.svg
+-rw-rw-rw-   0        0        0      309 2023-03-18 18:50:21.000000 aioqui-2.0.1/src/aioqui/.assets/icons/arrow-right.svg
+-rw-rw-rw-   0        0        0      352 2023-03-18 18:50:21.000000 aioqui-2.0.1/src/aioqui/.assets/icons/arrow-up-circle.svg
+-rw-rw-rw-   0        0        0      307 2023-03-18 18:50:21.000000 aioqui-2.0.1/src/aioqui/.assets/icons/arrow-up-left.svg
+-rw-rw-rw-   0        0        0      309 2023-03-18 18:50:21.000000 aioqui-2.0.1/src/aioqui/.assets/icons/arrow-up-right.svg
+-rw-rw-rw-   0        0        0      305 2023-03-18 18:50:21.000000 aioqui-2.0.1/src/aioqui/.assets/icons/arrow-up.svg
+-rw-rw-rw-   0        0        0      317 2023-03-18 18:50:21.000000 aioqui-2.0.1/src/aioqui/.assets/icons/at-sign.svg
+-rw-rw-rw-   0        0        0      320 2023-03-18 18:50:21.000000 aioqui-2.0.1/src/aioqui/.assets/icons/award.svg
+-rw-rw-rw-   0        0        0      350 2023-03-18 18:50:21.000000 aioqui-2.0.1/src/aioqui/.assets/icons/bar-chart-2.svg
+-rw-rw-rw-   0        0        0      348 2023-03-18 18:50:21.000000 aioqui-2.0.1/src/aioqui/.assets/icons/bar-chart.svg
+-rw-rw-rw-   0        0        0      422 2023-03-18 18:50:21.000000 aioqui-2.0.1/src/aioqui/.assets/icons/battery-charging.svg
+-rw-rw-rw-   0        0        0      321 2023-03-18 18:50:21.000000 aioqui-2.0.1/src/aioqui/.assets/icons/battery.svg
+-rw-rw-rw-   0        0        0      455 2023-03-18 18:50:21.000000 aioqui-2.0.1/src/aioqui/.assets/icons/bell-off.svg
+-rw-rw-rw-   0        0        0      316 2023-03-18 18:50:21.000000 aioqui-2.0.1/src/aioqui/.assets/icons/bell.svg
+-rw-rw-rw-   0        0        0      293 2023-03-18 18:50:21.000000 aioqui-2.0.1/src/aioqui/.assets/icons/bluetooth.svg
+-rw-rw-rw-   0        0        0      322 2023-03-18 18:50:21.000000 aioqui-2.0.1/src/aioqui/.assets/icons/bold.svg
+-rw-rw-rw-   0        0        0      334 2023-03-18 18:50:21.000000 aioqui-2.0.1/src/aioqui/.assets/icons/book-open.svg
+-rw-rw-rw-   0        0        0      340 2023-03-18 18:50:21.000000 aioqui-2.0.1/src/aioqui/.assets/icons/book.svg
+-rw-rw-rw-   0        0        0      282 2023-03-18 18:50:21.000000 aioqui-2.0.1/src/aioqui/.assets/icons/bookmark.svg
+-rw-rw-rw-   0        0        0      457 2023-03-18 18:50:21.000000 aioqui-2.0.1/src/aioqui/.assets/icons/box.svg
+-rw-rw-rw-   0        0        0      338 2023-03-18 18:50:21.000000 aioqui-2.0.1/src/aioqui/.assets/icons/briefcase.svg
+-rw-rw-rw-   0        0        0      405 2023-03-18 18:50:21.000000 aioqui-2.0.1/src/aioqui/.assets/icons/calendar.svg
+-rw-rw-rw-   0        0        0      380 2023-03-18 18:50:21.000000 aioqui-2.0.1/src/aioqui/.assets/icons/camera-off.svg
+-rw-rw-rw-   0        0        0      351 2023-03-18 18:50:21.000000 aioqui-2.0.1/src/aioqui/.assets/icons/camera.svg
+-rw-rw-rw-   0        0        0      382 2023-03-18 18:50:21.000000 aioqui-2.0.1/src/aioqui/.assets/icons/cast.svg
+-rw-rw-rw-   0        0        0      323 2023-03-18 18:50:21.000000 aioqui-2.0.1/src/aioqui/.assets/icons/check-circle.svg
+-rw-rw-rw-   0        0        0      340 2023-03-18 18:50:21.000000 aioqui-2.0.1/src/aioqui/.assets/icons/check-square.svg
+-rw-rw-rw-   0        0        0      257 2023-03-18 18:50:21.000000 aioqui-2.0.1/src/aioqui/.assets/icons/check.svg
+-rw-rw-rw-   0        0        0      264 2023-03-18 18:50:21.000000 aioqui-2.0.1/src/aioqui/.assets/icons/chevron-down.svg
+-rw-rw-rw-   0        0        0      265 2023-03-18 18:50:21.000000 aioqui-2.0.1/src/aioqui/.assets/icons/chevron-left.svg
+-rw-rw-rw-   0        0        0      265 2023-03-18 18:50:21.000000 aioqui-2.0.1/src/aioqui/.assets/icons/chevron-right.svg
+-rw-rw-rw-   0        0        0      263 2023-03-18 18:50:21.000000 aioqui-2.0.1/src/aioqui/.assets/icons/chevron-up.svg
+-rw-rw-rw-   0        0        0      312 2023-03-18 18:50:21.000000 aioqui-2.0.1/src/aioqui/.assets/icons/chevrons-down.svg
+-rw-rw-rw-   0        0        0      313 2023-03-18 18:50:21.000000 aioqui-2.0.1/src/aioqui/.assets/icons/chevrons-left.svg
+-rw-rw-rw-   0        0        0      313 2023-03-18 18:50:21.000000 aioqui-2.0.1/src/aioqui/.assets/icons/chevrons-right.svg
+-rw-rw-rw-   0        0        0      311 2023-03-18 18:50:21.000000 aioqui-2.0.1/src/aioqui/.assets/icons/chevrons-up.svg
+-rw-rw-rw-   0        0        0      443 2023-03-18 18:50:21.000000 aioqui-2.0.1/src/aioqui/.assets/icons/chrome.svg
+-rw-rw-rw-   0        0        0      253 2023-03-18 18:50:21.000000 aioqui-2.0.1/src/aioqui/.assets/icons/circle.svg
+-rw-rw-rw-   0        0        0      366 2023-03-18 18:50:21.000000 aioqui-2.0.1/src/aioqui/.assets/icons/clipboard.svg
+-rw-rw-rw-   0        0        0      299 2023-03-18 18:50:21.000000 aioqui-2.0.1/src/aioqui/.assets/icons/clock.svg
+-rw-rw-rw-   0        0        0      552 2023-03-18 18:50:21.000000 aioqui-2.0.1/src/aioqui/.assets/icons/cloud-drizzle.svg
+-rw-rw-rw-   0        0        0      340 2023-03-18 18:50:21.000000 aioqui-2.0.1/src/aioqui/.assets/icons/cloud-lightning.svg
+-rw-rw-rw-   0        0        0      366 2023-03-18 18:50:21.000000 aioqui-2.0.1/src/aioqui/.assets/icons/cloud-off.svg
+-rw-rw-rw-   0        0        0      416 2023-03-18 18:50:21.000000 aioqui-2.0.1/src/aioqui/.assets/icons/cloud-rain.svg
+-rw-rw-rw-   0        0        0      567 2023-03-18 18:50:21.000000 aioqui-2.0.1/src/aioqui/.assets/icons/cloud-snow.svg
+-rw-rw-rw-   0        0        0      275 2023-03-18 18:50:21.000000 aioqui-2.0.1/src/aioqui/.assets/icons/cloud.svg
+-rw-rw-rw-   0        0        0      302 2023-03-18 18:50:21.000000 aioqui-2.0.1/src/aioqui/.assets/icons/code.svg
+-rw-rw-rw-   0        0        0      481 2023-03-18 18:50:21.000000 aioqui-2.0.1/src/aioqui/.assets/icons/codepen.svg
+-rw-rw-rw-   0        0        0      633 2023-03-18 18:50:21.000000 aioqui-2.0.1/src/aioqui/.assets/icons/codesandbox.svg
+-rw-rw-rw-   0        0        0      442 2023-03-18 18:50:21.000000 aioqui-2.0.1/src/aioqui/.assets/icons/coffee.svg
+-rw-rw-rw-   0        0        0      321 2023-03-18 18:50:21.000000 aioqui-2.0.1/src/aioqui/.assets/icons/columns.svg
+-rw-rw-rw-   0        0        0      416 2023-03-18 18:50:21.000000 aioqui-2.0.1/src/aioqui/.assets/icons/command.svg
+-rw-rw-rw-   0        0        0      337 2023-03-18 18:50:21.000000 aioqui-2.0.1/src/aioqui/.assets/icons/compass.svg
+-rw-rw-rw-   0        0        0      346 2023-03-18 18:50:21.000000 aioqui-2.0.1/src/aioqui/.assets/icons/copy.svg
+-rw-rw-rw-   0        0        0      309 2023-03-18 18:50:21.000000 aioqui-2.0.1/src/aioqui/.assets/icons/corner-down-left.svg
+-rw-rw-rw-   0        0        0      313 2023-03-18 18:50:21.000000 aioqui-2.0.1/src/aioqui/.assets/icons/corner-down-right.svg
+-rw-rw-rw-   0        0        0      312 2023-03-18 18:50:21.000000 aioqui-2.0.1/src/aioqui/.assets/icons/corner-left-down.svg
+-rw-rw-rw-   0        0        0      307 2023-03-18 18:50:21.000000 aioqui-2.0.1/src/aioqui/.assets/icons/corner-left-up.svg
+-rw-rw-rw-   0        0        0      313 2023-03-18 18:50:21.000000 aioqui-2.0.1/src/aioqui/.assets/icons/corner-right-down.svg
+-rw-rw-rw-   0        0        0      308 2023-03-18 18:50:21.000000 aioqui-2.0.1/src/aioqui/.assets/icons/corner-right-up.svg
+-rw-rw-rw-   0        0        0      307 2023-03-18 18:50:21.000000 aioqui-2.0.1/src/aioqui/.assets/icons/corner-up-left.svg
+-rw-rw-rw-   0        0        0      311 2023-03-18 18:50:21.000000 aioqui-2.0.1/src/aioqui/.assets/icons/corner-up-right.svg
+-rw-rw-rw-   0        0        0      662 2023-03-18 18:50:21.000000 aioqui-2.0.1/src/aioqui/.assets/icons/cpu.svg
+-rw-rw-rw-   0        0        0      324 2023-03-18 18:50:21.000000 aioqui-2.0.1/src/aioqui/.assets/icons/credit-card.svg
+-rw-rw-rw-   0        0        0      305 2023-03-18 18:50:21.000000 aioqui-2.0.1/src/aioqui/.assets/icons/crop.svg
+-rw-rw-rw-   0        0        0      432 2023-03-18 18:50:21.000000 aioqui-2.0.1/src/aioqui/.assets/icons/crosshair.svg
+-rw-rw-rw-   0        0        0      367 2023-03-18 18:50:21.000000 aioqui-2.0.1/src/aioqui/.assets/icons/database.svg
+-rw-rw-rw-   0        0        0      369 2023-03-18 18:50:21.000000 aioqui-2.0.1/src/aioqui/.assets/icons/delete.svg
+-rw-rw-rw-   0        0        0      290 2023-03-18 18:50:21.000000 aioqui-2.0.1/src/aioqui/.assets/icons/disc.svg
+-rw-rw-rw-   0        0        0      392 2023-03-18 18:50:21.000000 aioqui-2.0.1/src/aioqui/.assets/icons/divide-circle.svg
+-rw-rw-rw-   0        0        0      414 2023-03-18 18:50:21.000000 aioqui-2.0.1/src/aioqui/.assets/icons/divide-square.svg
+-rw-rw-rw-   0        0        0      334 2023-03-18 18:50:21.000000 aioqui-2.0.1/src/aioqui/.assets/icons/divide.svg
+-rw-rw-rw-   0        0        0      329 2023-03-18 18:50:21.000000 aioqui-2.0.1/src/aioqui/.assets/icons/dollar-sign.svg
+-rw-rw-rw-   0        0        0      382 2023-03-18 18:50:21.000000 aioqui-2.0.1/src/aioqui/.assets/icons/download-cloud.svg
+-rw-rw-rw-   0        0        0      365 2023-03-18 18:50:21.000000 aioqui-2.0.1/src/aioqui/.assets/icons/download.svg
+-rw-rw-rw-   0        0        0      419 2023-03-18 18:50:21.000000 aioqui-2.0.1/src/aioqui/.assets/icons/dribbble.svg
+-rw-rw-rw-   0        0        0      269 2023-03-18 18:50:21.000000 aioqui-2.0.1/src/aioqui/.assets/icons/droplet.svg
+-rw-rw-rw-   0        0        0      286 2023-03-18 18:50:21.000000 aioqui-2.0.1/src/aioqui/.assets/icons/edit-2.svg
+-rw-rw-rw-   0        0        0      312 2023-03-18 18:50:21.000000 aioqui-2.0.1/src/aioqui/.assets/icons/edit-3.svg
+-rw-rw-rw-   0        0        0      360 2023-03-18 18:50:21.000000 aioqui-2.0.1/src/aioqui/.assets/icons/edit.svg
+-rw-rw-rw-   0        0        0      383 2023-03-18 18:50:21.000000 aioqui-2.0.1/src/aioqui/.assets/icons/external-link.svg
+-rw-rw-rw-   0        0        0      455 2023-03-18 18:50:21.000000 aioqui-2.0.1/src/aioqui/.assets/icons/eye-off.svg
+-rw-rw-rw-   0        0        0      311 2023-03-18 18:50:21.000000 aioqui-2.0.1/src/aioqui/.assets/icons/eye.svg
+-rw-rw-rw-   0        0        0      298 2023-03-18 18:50:21.000000 aioqui-2.0.1/src/aioqui/.assets/icons/facebook.svg
+-rw-rw-rw-   0        0        0      318 2023-03-18 18:50:21.000000 aioqui-2.0.1/src/aioqui/.assets/icons/fast-forward.svg
+-rw-rw-rw-   0        0        0      368 2023-03-18 18:50:21.000000 aioqui-2.0.1/src/aioqui/.assets/icons/feather.svg
+-rw-rw-rw-   0        0        0      548 2023-03-18 18:50:21.000000 aioqui-2.0.1/src/aioqui/.assets/icons/figma.svg
+-rw-rw-rw-   0        0        0      382 2023-03-18 18:50:21.000000 aioqui-2.0.1/src/aioqui/.assets/icons/file-minus.svg
+-rw-rw-rw-   0        0        0      426 2023-03-18 18:50:21.000000 aioqui-2.0.1/src/aioqui/.assets/icons/file-plus.svg
+-rw-rw-rw-   0        0        0      468 2023-03-18 18:50:21.000000 aioqui-2.0.1/src/aioqui/.assets/icons/file-text.svg
+-rw-rw-rw-   0        0        0      332 2023-03-18 18:50:21.000000 aioqui-2.0.1/src/aioqui/.assets/icons/file.svg
+-rw-rw-rw-   0        0        0      581 2023-03-18 18:50:21.000000 aioqui-2.0.1/src/aioqui/.assets/icons/film.svg
+-rw-rw-rw-   0        0        0      285 2023-03-18 18:50:21.000000 aioqui-2.0.1/src/aioqui/.assets/icons/filter.svg
+-rw-rw-rw-   0        0        0      329 2023-03-18 18:50:21.000000 aioqui-2.0.1/src/aioqui/.assets/icons/flag.svg
+-rw-rw-rw-   0        0        0      356 2023-03-18 18:50:21.000000 aioqui-2.0.1/src/aioqui/.assets/icons/folder-minus.svg
+-rw-rw-rw-   0        0        0      400 2023-03-18 18:50:21.000000 aioqui-2.0.1/src/aioqui/.assets/icons/folder-plus.svg
+-rw-rw-rw-   0        0        0      306 2023-03-18 18:50:21.000000 aioqui-2.0.1/src/aioqui/.assets/icons/folder.svg
+-rw-rw-rw-   0        0        0      273 2023-03-18 18:50:21.000000 aioqui-2.0.1/src/aioqui/.assets/icons/framer.svg
+-rw-rw-rw-   0        0        0      385 2023-03-18 18:50:21.000000 aioqui-2.0.1/src/aioqui/.assets/icons/frown.svg
+-rw-rw-rw-   0        0        0      476 2023-03-18 18:50:21.000000 aioqui-2.0.1/src/aioqui/.assets/icons/gift.svg
+-rw-rw-rw-   0        0        0      372 2023-03-18 18:50:21.000000 aioqui-2.0.1/src/aioqui/.assets/icons/git-branch.svg
+-rw-rw-rw-   0        0        0      353 2023-03-18 18:50:21.000000 aioqui-2.0.1/src/aioqui/.assets/icons/git-commit.svg
+-rw-rw-rw-   0        0        0      331 2023-03-18 18:50:21.000000 aioqui-2.0.1/src/aioqui/.assets/icons/git-merge.svg
+-rw-rw-rw-   0        0        0      382 2023-03-18 18:50:21.000000 aioqui-2.0.1/src/aioqui/.assets/icons/git-pull-request.svg
+-rw-rw-rw-   0        0        0      522 2023-03-18 18:50:21.000000 aioqui-2.0.1/src/aioqui/.assets/icons/github.svg
+-rw-rw-rw-   0        0        0      485 2023-03-18 18:50:21.000000 aioqui-2.0.1/src/aioqui/.assets/icons/gitlab.svg
+-rw-rw-rw-   0        0        0      404 2023-03-18 18:50:21.000000 aioqui-2.0.1/src/aioqui/.assets/icons/globe.svg
+-rw-rw-rw-   0        0        0      399 2023-03-18 18:50:21.000000 aioqui-2.0.1/src/aioqui/.assets/icons/grid.svg
+-rw-rw-rw-   0        0        0      479 2023-03-18 18:50:21.000000 aioqui-2.0.1/src/aioqui/.assets/icons/hard-drive.svg
+-rw-rw-rw-   0        0        0      384 2023-03-18 18:50:21.000000 aioqui-2.0.1/src/aioqui/.assets/icons/hash.svg
+-rw-rw-rw-   0        0        0      390 2023-03-18 18:50:21.000000 aioqui-2.0.1/src/aioqui/.assets/icons/headphones.svg
+-rw-rw-rw-   0        0        0      366 2023-03-18 18:50:21.000000 aioqui-2.0.1/src/aioqui/.assets/icons/heart.svg
+-rw-rw-rw-   0        0        0      360 2023-03-18 18:50:21.000000 aioqui-2.0.1/src/aioqui/.assets/icons/help-circle.svg
+-rw-rw-rw-   0        0        0      353 2023-03-18 18:50:21.000000 aioqui-2.0.1/src/aioqui/.assets/icons/hexagon.svg
+-rw-rw-rw-   0        0        0      327 2023-03-18 18:50:21.000000 aioqui-2.0.1/src/aioqui/.assets/icons/home.svg
+-rw-rw-rw-   0        0        0      364 2023-03-18 18:50:21.000000 aioqui-2.0.1/src/aioqui/.assets/icons/image.svg
+-rw-rw-rw-   0        0        0      400 2023-03-18 18:50:21.000000 aioqui-2.0.1/src/aioqui/.assets/icons/inbox.svg
+-rw-rw-rw-   0        0        0      342 2023-03-18 18:50:21.000000 aioqui-2.0.1/src/aioqui/.assets/icons/info.svg
+-rw-rw-rw-   0        0        0      395 2023-03-18 18:50:21.000000 aioqui-2.0.1/src/aioqui/.assets/icons/instagram.svg
+-rw-rw-rw-   0        0        0      343 2023-03-18 18:50:21.000000 aioqui-2.0.1/src/aioqui/.assets/icons/italic.svg
+-rw-rw-rw-   0        0        0      347 2023-03-18 18:50:21.000000 aioqui-2.0.1/src/aioqui/.assets/icons/key.svg
+-rw-rw-rw-   0        0        0      360 2023-03-18 18:50:21.000000 aioqui-2.0.1/src/aioqui/.assets/icons/layers.svg
+-rw-rw-rw-   0        0        0      359 2023-03-18 18:50:21.000000 aioqui-2.0.1/src/aioqui/.assets/icons/layout.svg
+-rw-rw-rw-   0        0        0      570 2023-03-18 18:50:21.000000 aioqui-2.0.1/src/aioqui/.assets/icons/life-buoy.svg
+-rw-rw-rw-   0        0        0      350 2023-03-18 18:50:21.000000 aioqui-2.0.1/src/aioqui/.assets/icons/link-2.svg
+-rw-rw-rw-   0        0        0      366 2023-03-18 18:50:21.000000 aioqui-2.0.1/src/aioqui/.assets/icons/link.svg
+-rw-rw-rw-   0        0        0      395 2023-03-18 18:50:21.000000 aioqui-2.0.1/src/aioqui/.assets/icons/linkedin.svg
+-rw-rw-rw-   0        0        0      477 2023-03-18 18:50:21.000000 aioqui-2.0.1/src/aioqui/.assets/icons/list.svg
+-rw-rw-rw-   0        0        0      609 2023-03-18 18:50:21.000000 aioqui-2.0.1/src/aioqui/.assets/icons/loader.svg
+-rw-rw-rw-   0        0        0      316 2023-03-18 18:50:21.000000 aioqui-2.0.1/src/aioqui/.assets/icons/lock.svg
+-rw-rw-rw-   0        0        0      363 2023-03-18 18:50:21.000000 aioqui-2.0.1/src/aioqui/.assets/icons/log-in.svg
+-rw-rw-rw-   0        0        0      362 2023-03-18 18:50:21.000000 aioqui-2.0.1/src/aioqui/.assets/icons/log-out.svg
+-rw-rw-rw-   0        0        0      349 2023-03-18 18:50:21.000000 aioqui-2.0.1/src/aioqui/.assets/icons/mail.svg
+-rw-rw-rw-   0        0        0      317 2023-03-18 18:50:21.000000 aioqui-2.0.1/src/aioqui/.assets/icons/map-pin.svg
+-rw-rw-rw-   0        0        0      368 2023-03-18 18:50:21.000000 aioqui-2.0.1/src/aioqui/.assets/icons/map.svg
+-rw-rw-rw-   0        0        0      395 2023-03-18 18:50:21.000000 aioqui-2.0.1/src/aioqui/.assets/icons/maximize-2.svg
+-rw-rw-rw-   0        0        0      326 2023-03-18 18:50:21.000000 aioqui-2.0.1/src/aioqui/.assets/icons/maximize.svg
+-rw-rw-rw-   0        0        0      384 2023-03-18 18:50:21.000000 aioqui-2.0.1/src/aioqui/.assets/icons/meh.svg
+-rw-rw-rw-   0        0        0      341 2023-03-18 18:50:21.000000 aioqui-2.0.1/src/aioqui/.assets/icons/menu.svg
+-rw-rw-rw-   0        0        0      423 2023-03-18 18:50:21.000000 aioqui-2.0.1/src/aioqui/.assets/icons/message-circle.svg
+-rw-rw-rw-   0        0        0      300 2023-03-18 18:50:21.000000 aioqui-2.0.1/src/aioqui/.assets/icons/message-square.svg
+-rw-rw-rw-   0        0        0      489 2023-03-18 18:50:21.000000 aioqui-2.0.1/src/aioqui/.assets/icons/mic-off.svg
+-rw-rw-rw-   0        0        0      413 2023-03-18 18:50:21.000000 aioqui-2.0.1/src/aioqui/.assets/icons/mic.svg
+-rw-rw-rw-   0        0        0      399 2023-03-18 18:50:21.000000 aioqui-2.0.1/src/aioqui/.assets/icons/minimize-2.svg
+-rw-rw-rw-   0        0        0      326 2023-03-18 18:50:21.000000 aioqui-2.0.1/src/aioqui/.assets/icons/minimize.svg
+-rw-rw-rw-   0        0        0      303 2023-03-18 18:50:21.000000 aioqui-2.0.1/src/aioqui/.assets/icons/minus-circle.svg
+-rw-rw-rw-   0        0        0      325 2023-03-18 18:50:21.000000 aioqui-2.0.1/src/aioqui/.assets/icons/minus-square.svg
+-rw-rw-rw-   0        0        0      256 2023-03-18 18:50:21.000000 aioqui-2.0.1/src/aioqui/.assets/icons/minus.svg
+-rw-rw-rw-   0        0        0      365 2023-03-18 18:50:21.000000 aioqui-2.0.1/src/aioqui/.assets/icons/monitor.svg
+-rw-rw-rw-   0        0        0      276 2023-03-18 18:50:21.000000 aioqui-2.0.1/src/aioqui/.assets/icons/moon.svg
+-rw-rw-rw-   0        0        0      338 2023-03-18 18:50:21.000000 aioqui-2.0.1/src/aioqui/.assets/icons/more-horizontal.svg
+-rw-rw-rw-   0        0        0      336 2023-03-18 18:50:21.000000 aioqui-2.0.1/src/aioqui/.assets/icons/more-vertical.svg
+-rw-rw-rw-   0        0        0      306 2023-03-18 18:50:21.000000 aioqui-2.0.1/src/aioqui/.assets/icons/mouse-pointer.svg
+-rw-rw-rw-   0        0        0      481 2023-03-18 18:50:21.000000 aioqui-2.0.1/src/aioqui/.assets/icons/move.svg
+-rw-rw-rw-   0        0        0      322 2023-03-18 18:50:21.000000 aioqui-2.0.1/src/aioqui/.assets/icons/music.svg
+-rw-rw-rw-   0        0        0      274 2023-03-18 18:50:21.000000 aioqui-2.0.1/src/aioqui/.assets/icons/navigation-2.svg
+-rw-rw-rw-   0        0        0      272 2023-03-18 18:50:21.000000 aioqui-2.0.1/src/aioqui/.assets/icons/navigation.svg
+-rw-rw-rw-   0        0        0      313 2023-03-18 18:50:21.000000 aioqui-2.0.1/src/aioqui/.assets/icons/octagon.svg
+-rw-rw-rw-   0        0        0      512 2023-03-18 18:50:21.000000 aioqui-2.0.1/src/aioqui/.assets/icons/package.svg
+-rw-rw-rw-   0        0        0      347 2023-03-18 18:50:21.000000 aioqui-2.0.1/src/aioqui/.assets/icons/paperclip.svg
+-rw-rw-rw-   0        0        0      347 2023-03-18 18:50:21.000000 aioqui-2.0.1/src/aioqui/.assets/icons/pause-circle.svg
+-rw-rw-rw-   0        0        0      307 2023-03-18 18:50:21.000000 aioqui-2.0.1/src/aioqui/.assets/icons/pause.svg
+-rw-rw-rw-   0        0        0      386 2023-03-18 18:50:21.000000 aioqui-2.0.1/src/aioqui/.assets/icons/pen-tool.svg
+-rw-rw-rw-   0        0        0      345 2023-03-18 18:50:21.000000 aioqui-2.0.1/src/aioqui/.assets/icons/percent.svg
+-rw-rw-rw-   0        0        0      571 2023-03-18 18:50:21.000000 aioqui-2.0.1/src/aioqui/.assets/icons/phone-call.svg
+-rw-rw-rw-   0        0        0      613 2023-03-18 18:50:21.000000 aioqui-2.0.1/src/aioqui/.assets/icons/phone-forwarded.svg
+-rw-rw-rw-   0        0        0      612 2023-03-18 18:50:21.000000 aioqui-2.0.1/src/aioqui/.assets/icons/phone-incoming.svg
+-rw-rw-rw-   0        0        0      608 2023-03-18 18:50:21.000000 aioqui-2.0.1/src/aioqui/.assets/icons/phone-missed.svg
+-rw-rw-rw-   0        0        0      586 2023-03-18 18:50:21.000000 aioqui-2.0.1/src/aioqui/.assets/icons/phone-off.svg
+-rw-rw-rw-   0        0        0      612 2023-03-18 18:50:21.000000 aioqui-2.0.1/src/aioqui/.assets/icons/phone-outgoing.svg
+-rw-rw-rw-   0        0        0      515 2023-03-18 18:50:21.000000 aioqui-2.0.1/src/aioqui/.assets/icons/phone.svg
+-rw-rw-rw-   0        0        0      310 2023-03-18 18:50:21.000000 aioqui-2.0.1/src/aioqui/.assets/icons/pie-chart.svg
+-rw-rw-rw-   0        0        0      308 2023-03-18 18:50:21.000000 aioqui-2.0.1/src/aioqui/.assets/icons/play-circle.svg
+-rw-rw-rw-   0        0        0      258 2023-03-18 18:50:21.000000 aioqui-2.0.1/src/aioqui/.assets/icons/play.svg
+-rw-rw-rw-   0        0        0      345 2023-03-18 18:50:21.000000 aioqui-2.0.1/src/aioqui/.assets/icons/plus-circle-gray.svg
+-rw-rw-rw-   0        0        0      346 2023-03-18 18:50:21.000000 aioqui-2.0.1/src/aioqui/.assets/icons/plus-circle.svg
+-rw-rw-rw-   0        0        0      368 2023-03-18 18:50:21.000000 aioqui-2.0.1/src/aioqui/.assets/icons/plus-square.svg
+-rw-rw-rw-   0        0        0      299 2023-03-18 18:50:21.000000 aioqui-2.0.1/src/aioqui/.assets/icons/plus.svg
+-rw-rw-rw-   0        0        0      353 2023-03-18 18:50:21.000000 aioqui-2.0.1/src/aioqui/.assets/icons/pocket.svg
+-rw-rw-rw-   0        0        0      303 2023-03-18 18:50:21.000000 aioqui-2.0.1/src/aioqui/.assets/icons/power.svg
+-rw-rw-rw-   0        0        0      402 2023-03-18 18:50:21.000000 aioqui-2.0.1/src/aioqui/.assets/icons/printer.svg
+-rw-rw-rw-   0        0        0      384 2023-03-18 18:50:21.000000 aioqui-2.0.1/src/aioqui/.assets/icons/radio.svg
+-rw-rw-rw-   0        0        0      395 2023-03-18 18:50:21.000000 aioqui-2.0.1/src/aioqui/.assets/icons/refresh-ccw.svg
+-rw-rw-rw-   0        0        0      395 2023-03-18 18:50:21.000000 aioqui-2.0.1/src/aioqui/.assets/icons/refresh-cw.svg
+-rw-rw-rw-   0        0        0      387 2023-03-18 18:50:21.000000 aioqui-2.0.1/src/aioqui/.assets/icons/repeat.svg
+-rw-rw-rw-   0        0        0      314 2023-03-18 18:50:21.000000 aioqui-2.0.1/src/aioqui/.assets/icons/rewind.svg
+-rw-rw-rw-   0        0        0      312 2023-03-18 18:50:21.000000 aioqui-2.0.1/src/aioqui/.assets/icons/rotate-ccw.svg
+-rw-rw-rw-   0        0        0      316 2023-03-18 18:50:21.000000 aioqui-2.0.1/src/aioqui/.assets/icons/rotate-cw.svg
+-rw-rw-rw-   0        0        0      325 2023-03-18 18:50:21.000000 aioqui-2.0.1/src/aioqui/.assets/icons/rss.svg
+-rw-rw-rw-   0        0        0      387 2023-03-18 18:50:21.000000 aioqui-2.0.1/src/aioqui/.assets/icons/save.svg
+-rw-rw-rw-   0        0        0      366 2023-03-18 18:50:21.000000 aioqui-2.0.1/src/aioqui/.assets/icons/schedule.svg
+-rw-rw-rw-   0        0        0      439 2023-03-18 18:50:21.000000 aioqui-2.0.1/src/aioqui/.assets/icons/scissors.svg
+-rw-rw-rw-   0        0        0      303 2023-03-18 18:50:21.000000 aioqui-2.0.1/src/aioqui/.assets/icons/search.svg
+-rw-rw-rw-   0        0        0      309 2023-03-18 18:50:21.000000 aioqui-2.0.1/src/aioqui/.assets/icons/send.svg
+-rw-rw-rw-   0        0        0      426 2023-03-18 18:50:21.000000 aioqui-2.0.1/src/aioqui/.assets/icons/server.svg
+-rw-rw-rw-   0        0        0     1006 2023-03-18 18:50:21.000000 aioqui-2.0.1/src/aioqui/.assets/icons/settings.svg
+-rw-rw-rw-   0        0        0      440 2023-03-18 18:50:21.000000 aioqui-2.0.1/src/aioqui/.assets/icons/share-2.svg
+-rw-rw-rw-   0        0        0      359 2023-03-18 18:50:21.000000 aioqui-2.0.1/src/aioqui/.assets/icons/share.svg
+-rw-rw-rw-   0        0        0      400 2023-03-18 18:50:21.000000 aioqui-2.0.1/src/aioqui/.assets/icons/shield-off.svg
+-rw-rw-rw-   0        0        0      274 2023-03-18 18:50:21.000000 aioqui-2.0.1/src/aioqui/.assets/icons/shield.svg
+-rw-rw-rw-   0        0        0      367 2023-03-18 18:50:21.000000 aioqui-2.0.1/src/aioqui/.assets/icons/shopping-bag.svg
+-rw-rw-rw-   0        0        0      378 2023-03-18 18:50:21.000000 aioqui-2.0.1/src/aioqui/.assets/icons/shopping-cart.svg
+-rw-rw-rw-   0        0        0      436 2023-03-18 18:50:21.000000 aioqui-2.0.1/src/aioqui/.assets/icons/shuffle.svg
+-rw-rw-rw-   0        0        0      318 2023-03-18 18:50:21.000000 aioqui-2.0.1/src/aioqui/.assets/icons/sidebar.svg
+-rw-rw-rw-   0        0        0      308 2023-03-18 18:50:21.000000 aioqui-2.0.1/src/aioqui/.assets/icons/skip-back.svg
+-rw-rw-rw-   0        0        0      310 2023-03-18 18:50:21.000000 aioqui-2.0.1/src/aioqui/.assets/icons/skip-forward.svg
+-rw-rw-rw-   0        0        0      994 2023-03-18 18:50:21.000000 aioqui-2.0.1/src/aioqui/.assets/icons/slack.svg
+-rw-rw-rw-   0        0        0      307 2023-03-18 18:50:21.000000 aioqui-2.0.1/src/aioqui/.assets/icons/slash.svg
+-rw-rw-rw-   0        0        0      606 2023-03-18 18:50:21.000000 aioqui-2.0.1/src/aioqui/.assets/icons/sliders.svg
+-rw-rw-rw-   0        0        0      327 2023-03-18 18:50:21.000000 aioqui-2.0.1/src/aioqui/.assets/icons/smartphone.svg
+-rw-rw-rw-   0        0        0      383 2023-03-18 18:50:21.000000 aioqui-2.0.1/src/aioqui/.assets/icons/smile.svg
+-rw-rw-rw-   0        0        0      361 2023-03-18 18:50:21.000000 aioqui-2.0.1/src/aioqui/.assets/icons/speaker.svg
+-rw-rw-rw-   0        0        0      275 2023-03-18 18:50:21.000000 aioqui-2.0.1/src/aioqui/.assets/icons/square.svg
+-rw-rw-rw-   0        0        0      391 2023-04-06 21:10:35.000000 aioqui-2.0.1/src/aioqui/.assets/icons/star-fill.svg
+-rw-rw-rw-   0        0        0      334 2023-03-18 18:50:21.000000 aioqui-2.0.1/src/aioqui/.assets/icons/star.svg
+-rw-rw-rw-   0        0        0      304 2023-03-18 18:50:21.000000 aioqui-2.0.1/src/aioqui/.assets/icons/stop-circle.svg
+-rw-rw-rw-   0        0        0      645 2023-03-18 18:50:21.000000 aioqui-2.0.1/src/aioqui/.assets/icons/sun.svg
+-rw-rw-rw-   0        0        0      584 2023-03-18 18:50:21.000000 aioqui-2.0.1/src/aioqui/.assets/icons/sunrise.svg
+-rw-rw-rw-   0        0        0      583 2023-03-18 18:50:21.000000 aioqui-2.0.1/src/aioqui/.assets/icons/sunset.svg
+-rw-rw-rw-   0        0        0      335 2023-03-18 18:50:21.000000 aioqui-2.0.1/src/aioqui/.assets/icons/table.svg
+-rw-rw-rw-   0        0        0      323 2023-03-18 18:50:21.000000 aioqui-2.0.1/src/aioqui/.assets/icons/tablet.svg
+-rw-rw-rw-   0        0        0      350 2023-03-18 18:50:21.000000 aioqui-2.0.1/src/aioqui/.assets/icons/tag.svg
+-rw-rw-rw-   0        0        0      331 2023-03-18 18:50:21.000000 aioqui-2.0.1/src/aioqui/.assets/icons/target.svg
+-rw-rw-rw-   0        0        0      305 2023-03-18 18:50:21.000000 aioqui-2.0.1/src/aioqui/.assets/icons/terminal.svg
+-rw-rw-rw-   0        0        0      292 2023-03-18 18:50:21.000000 aioqui-2.0.1/src/aioqui/.assets/icons/thermometer.svg
+-rw-rw-rw-   0        0        0      369 2023-03-18 18:50:21.000000 aioqui-2.0.1/src/aioqui/.assets/icons/thumbs-down.svg
+-rw-rw-rw-   0        0        0      349 2023-03-18 18:50:21.000000 aioqui-2.0.1/src/aioqui/.assets/icons/thumbs-up.svg
+-rw-rw-rw-   0        0        0      318 2023-03-18 18:50:21.000000 aioqui-2.0.1/src/aioqui/.assets/icons/toggle-left.svg
+-rw-rw-rw-   0        0        0      320 2023-03-18 18:50:21.000000 aioqui-2.0.1/src/aioqui/.assets/icons/toggle-right.svg
+-rw-rw-rw-   0        0        0      381 2023-03-18 18:50:21.000000 aioqui-2.0.1/src/aioqui/.assets/icons/tool.svg
+-rw-rw-rw-   0        0        0      443 2023-03-18 18:50:21.000000 aioqui-2.0.1/src/aioqui/.assets/icons/trash-2.svg
+-rw-rw-rw-   0        0        0      351 2023-03-18 18:50:21.000000 aioqui-2.0.1/src/aioqui/.assets/icons/trash.svg
+-rw-rw-rw-   0        0        0      368 2023-03-18 18:50:21.000000 aioqui-2.0.1/src/aioqui/.assets/icons/trello.svg
+-rw-rw-rw-   0        0        0      326 2023-03-18 18:50:21.000000 aioqui-2.0.1/src/aioqui/.assets/icons/trending-down.svg
+-rw-rw-rw-   0        0        0      323 2023-03-18 18:50:21.000000 aioqui-2.0.1/src/aioqui/.assets/icons/trending-up.svg
+-rw-rw-rw-   0        0        0      321 2023-03-18 18:50:21.000000 aioqui-2.0.1/src/aioqui/.assets/icons/triangle.svg
+-rw-rw-rw-   0        0        0      410 2023-03-18 18:50:21.000000 aioqui-2.0.1/src/aioqui/.assets/icons/truck.svg
+-rw-rw-rw-   0        0        0      315 2023-03-18 18:50:21.000000 aioqui-2.0.1/src/aioqui/.assets/icons/tv.svg
+-rw-rw-rw-   0        0        0      272 2023-03-18 18:50:21.000000 aioqui-2.0.1/src/aioqui/.assets/icons/twitch.svg
+-rw-rw-rw-   0        0        0      403 2023-03-18 18:50:21.000000 aioqui-2.0.1/src/aioqui/.assets/icons/twitter.svg
+-rw-rw-rw-   0        0        0      347 2023-03-18 18:50:21.000000 aioqui-2.0.1/src/aioqui/.assets/icons/type.svg
+-rw-rw-rw-   0        0        0      285 2023-03-18 18:50:21.000000 aioqui-2.0.1/src/aioqui/.assets/icons/umbrella.svg
+-rw-rw-rw-   0        0        0      314 2023-03-18 18:50:21.000000 aioqui-2.0.1/src/aioqui/.assets/icons/underline.svg
+-rw-rw-rw-   0        0        0      317 2023-03-18 18:50:21.000000 aioqui-2.0.1/src/aioqui/.assets/icons/unlock.svg
+-rw-rw-rw-   0        0        0      426 2023-03-18 18:50:21.000000 aioqui-2.0.1/src/aioqui/.assets/icons/upload-cloud.svg
+-rw-rw-rw-   0        0        0      360 2023-03-18 18:50:21.000000 aioqui-2.0.1/src/aioqui/.assets/icons/upload.svg
+-rw-rw-rw-   0        0        0      362 2023-03-18 18:50:21.000000 aioqui-2.0.1/src/aioqui/.assets/icons/user-check.svg
+-rw-rw-rw-   0        0        0      360 2023-03-18 18:50:21.000000 aioqui-2.0.1/src/aioqui/.assets/icons/user-minus.svg
+-rw-rw-rw-   0        0        0      403 2023-03-18 18:50:21.000000 aioqui-2.0.1/src/aioqui/.assets/icons/user-plus.svg
+-rw-rw-rw-   0        0        0      399 2023-03-18 18:50:21.000000 aioqui-2.0.1/src/aioqui/.assets/icons/user-x.svg
+-rw-rw-rw-   0        0        0      308 2023-03-18 18:50:21.000000 aioqui-2.0.1/src/aioqui/.assets/icons/user.svg
+-rw-rw-rw-   0        0        0      395 2023-03-18 18:50:21.000000 aioqui-2.0.1/src/aioqui/.assets/icons/users.svg
+-rw-rw-rw-   0        0        0      374 2023-03-18 18:50:21.000000 aioqui-2.0.1/src/aioqui/.assets/icons/video-off.svg
+-rw-rw-rw-   0        0        0      324 2023-03-18 18:50:21.000000 aioqui-2.0.1/src/aioqui/.assets/icons/video.svg
+-rw-rw-rw-   0        0        0      353 2023-03-18 18:50:21.000000 aioqui-2.0.1/src/aioqui/.assets/icons/voicemail.svg
+-rw-rw-rw-   0        0        0      323 2023-03-18 18:50:21.000000 aioqui-2.0.1/src/aioqui/.assets/icons/volume-1.svg
+-rw-rw-rw-   0        0        0      354 2023-03-18 18:50:21.000000 aioqui-2.0.1/src/aioqui/.assets/icons/volume-2.svg
+-rw-rw-rw-   0        0        0      365 2023-03-18 18:50:21.000000 aioqui-2.0.1/src/aioqui/.assets/icons/volume-x.svg
+-rw-rw-rw-   0        0        0      275 2023-03-18 18:50:21.000000 aioqui-2.0.1/src/aioqui/.assets/icons/volume.svg
+-rw-rw-rw-   0        0        0      457 2023-03-18 18:50:21.000000 aioqui-2.0.1/src/aioqui/.assets/icons/watch.svg
+-rw-rw-rw-   0        0        0      564 2023-03-18 18:50:21.000000 aioqui-2.0.1/src/aioqui/.assets/icons/wifi-off.svg
+-rw-rw-rw-   0        0        0      396 2023-03-18 18:50:21.000000 aioqui-2.0.1/src/aioqui/.assets/icons/wifi.svg
+-rw-rw-rw-   0        0        0      321 2023-03-18 18:50:21.000000 aioqui-2.0.1/src/aioqui/.assets/icons/wind.svg
+-rw-rw-rw-   0        0        0      340 2023-03-18 18:50:21.000000 aioqui-2.0.1/src/aioqui/.assets/icons/x-circle-gray.svg
+-rw-rw-rw-   0        0        0      341 2023-03-18 18:50:21.000000 aioqui-2.0.1/src/aioqui/.assets/icons/x-circle.svg
+-rw-rw-rw-   0        0        0      401 2023-03-18 18:50:21.000000 aioqui-2.0.1/src/aioqui/.assets/icons/x-octagon.svg
+-rw-rw-rw-   0        0        0      363 2023-03-18 18:50:21.000000 aioqui-2.0.1/src/aioqui/.assets/icons/x-square.svg
+-rw-rw-rw-   0        0        0      294 2023-03-18 18:50:21.000000 aioqui-2.0.1/src/aioqui/.assets/icons/x.svg
+-rw-rw-rw-   0        0        0      560 2023-03-18 18:50:21.000000 aioqui-2.0.1/src/aioqui/.assets/icons/youtube.svg
+-rw-rw-rw-   0        0        0      428 2023-03-18 18:50:21.000000 aioqui-2.0.1/src/aioqui/.assets/icons/zap-off.svg
+-rw-rw-rw-   0        0        0      277 2023-03-18 18:50:21.000000 aioqui-2.0.1/src/aioqui/.assets/icons/zap.svg
+-rw-rw-rw-   0        0        0      392 2023-03-18 18:50:21.000000 aioqui-2.0.1/src/aioqui/.assets/icons/zoom-in.svg
+-rw-rw-rw-   0        0        0      349 2023-03-18 18:50:21.000000 aioqui-2.0.1/src/aioqui/.assets/icons/zoom-out.svg
+-rw-rw-rw-   0        0        0      177 2023-05-16 21:16:03.000000 aioqui-2.0.1/src/aioqui/__init__.py
+drwxrwxrwx   0        0        0        0 2023-05-16 21:21:00.651550 aioqui-2.0.1/src/aioqui/context/
+-rw-rw-rw-   0        0        0       70 2023-05-15 07:06:13.000000 aioqui-2.0.1/src/aioqui/context/__init__.py
+-rw-rw-rw-   0        0        0     9795 2023-05-16 21:16:03.000000 aioqui-2.0.1/src/aioqui/context/context_obj.py
+-rw-rw-rw-   0        0        0      528 2023-05-15 15:53:26.000000 aioqui-2.0.1/src/aioqui/context/contextapi.py
+drwxrwxrwx   0        0        0        0 2023-05-16 21:21:00.658551 aioqui-2.0.1/src/aioqui/misc/
+-rw-rw-rw-   0        0        0      128 2023-05-15 08:51:32.000000 aioqui-2.0.1/src/aioqui/misc/__init__.py
+-rw-rw-rw-   0        0        0     3736 2023-05-15 04:39:08.000000 aioqui-2.0.1/src/aioqui/misc/aiorequest.py
+-rw-rw-rw-   0        0        0      978 2023-05-16 18:20:57.000000 aioqui-2.0.1/src/aioqui/misc/animation.py
+-rw-rw-rw-   0        0        0     1130 2023-05-15 08:41:25.000000 aioqui-2.0.1/src/aioqui/misc/conthrq.py
+-rw-rw-rw-   0        0        0     1386 2023-05-14 18:16:30.000000 aioqui-2.0.1/src/aioqui/misc/fileops.py
+-rw-rw-rw-   0        0        0     2181 2023-05-14 00:12:50.000000 aioqui-2.0.1/src/aioqui/misc/qss_parser.py
+-rw-rw-rw-   0        0        0      319 2023-05-15 08:04:15.000000 aioqui-2.0.1/src/aioqui/misc/utils.py
+-rw-rw-rw-   0        0        0      701 2023-05-14 00:40:28.000000 aioqui-2.0.1/src/aioqui/misc/uvithread.py
+-rw-rw-rw-   0        0        0     1151 2023-05-15 05:37:56.000000 aioqui-2.0.1/src/aioqui/qasyncio.py
+drwxrwxrwx   0        0        0        0 2023-05-16 21:21:00.662551 aioqui-2.0.1/src/aioqui/types/
+-rw-rw-rw-   0        0        0       93 2023-05-16 21:16:03.000000 aioqui-2.0.1/src/aioqui/types/__init__.py
+-rw-rw-rw-   0        0        0      257 2023-05-16 18:47:39.000000 aioqui-2.0.1/src/aioqui/types/common.py
+drwxrwxrwx   0        0        0        0 2023-05-16 21:21:00.670550 aioqui-2.0.1/src/aioqui/types/enums/
+-rw-rw-rw-   0        0        0      294 2023-05-16 17:41:17.000000 aioqui-2.0.1/src/aioqui/types/enums/__init__.py
+-rw-rw-rw-   0        0        0      687 2023-05-13 23:00:29.000000 aioqui-2.0.1/src/aioqui/types/enums/alignment.py
+-rw-rw-rw-   0        0        0      182 2023-05-15 05:17:48.000000 aioqui-2.0.1/src/aioqui/types/enums/echo_mode.py
+-rw-rw-rw-   0        0        0      227 2023-05-14 07:18:50.000000 aioqui-2.0.1/src/aioqui/types/enums/elide_mode.py
+-rw-rw-rw-   0        0        0      283 2023-05-16 17:57:41.000000 aioqui-2.0.1/src/aioqui/types/enums/logic_button.py
+-rw-rw-rw-   0        0        0      151 2023-05-13 23:00:29.000000 aioqui-2.0.1/src/aioqui/types/enums/orientation.py
+-rw-rw-rw-   0        0        0      264 2023-05-14 00:48:52.000000 aioqui-2.0.1/src/aioqui/types/enums/scroll_policy.py
+-rw-rw-rw-   0        0        0      235 2023-05-15 05:48:40.000000 aioqui-2.0.1/src/aioqui/types/enums/size_policy.py
+-rw-rw-rw-   0        0        0      105 2023-05-13 23:00:29.000000 aioqui-2.0.1/src/aioqui/types/enums/window_hint.py
+-rw-rw-rw-   0        0        0     3503 2023-05-15 16:06:33.000000 aioqui-2.0.1/src/aioqui/types/icon.py
+-rw-rw-rw-   0        0        0      331 2023-05-15 15:26:00.000000 aioqui-2.0.1/src/aioqui/types/size.py
+drwxrwxrwx   0        0        0        0 2023-05-16 21:21:00.683550 aioqui-2.0.1/src/aioqui/widgets/
+-rw-rw-rw-   0        0        0      668 2023-05-16 20:12:13.000000 aioqui-2.0.1/src/aioqui/widgets/__init__.py
+-rw-rw-rw-   0        0        0      524 2023-05-16 18:48:54.000000 aioqui-2.0.1/src/aioqui/widgets/button.py
+drwxrwxrwx   0        0        0        0 2023-05-16 21:21:00.689550 aioqui-2.0.1/src/aioqui/widgets/custom/
+-rw-rw-rw-   0        0        0      218 2023-05-16 21:12:59.000000 aioqui-2.0.1/src/aioqui/widgets/custom/__init__.py
+-rw-rw-rw-   0        0        0     1939 2023-05-16 18:22:11.000000 aioqui-2.0.1/src/aioqui/widgets/custom/error_label.py
+-rw-rw-rw-   0        0        0     2492 2023-05-16 21:10:31.000000 aioqui-2.0.1/src/aioqui/widgets/custom/image_button.py
+-rw-rw-rw-   0        0        0     1423 2023-05-15 07:46:33.000000 aioqui-2.0.1/src/aioqui/widgets/custom/menu_button.py
+-rw-rw-rw-   0        0        0     3079 2023-05-16 21:17:28.000000 aioqui-2.0.1/src/aioqui/widgets/custom/popup.py
+-rw-rw-rw-   0        0        0     1027 2023-05-15 07:42:41.000000 aioqui-2.0.1/src/aioqui/widgets/custom/searchbar.py
+-rw-rw-rw-   0        0        0     1887 2023-05-16 18:51:40.000000 aioqui-2.0.1/src/aioqui/widgets/custom/state_icon_btn.py
+-rw-rw-rw-   0        0        0      712 2023-05-16 21:04:40.000000 aioqui-2.0.1/src/aioqui/widgets/date_time.py
+drwxrwxrwx   0        0        0        0 2023-05-16 21:21:00.693550 aioqui-2.0.1/src/aioqui/widgets/extensions/
+-rw-rw-rw-   0        0        0      160 2023-05-15 06:44:59.000000 aioqui-2.0.1/src/aioqui/widgets/extensions/__init__.py
+-rw-rw-rw-   0        0        0      746 2023-05-16 21:18:22.000000 aioqui-2.0.1/src/aioqui/widgets/extensions/input_ext.py
+-rw-rw-rw-   0        0        0     1944 2023-05-16 21:18:22.000000 aioqui-2.0.1/src/aioqui/widgets/extensions/layout_ext.py
+-rw-rw-rw-   0        0        0      710 2023-05-16 21:18:22.000000 aioqui-2.0.1/src/aioqui/widgets/extensions/side_menu_ext.py
+-rw-rw-rw-   0        0        0     1925 2023-05-16 21:18:22.000000 aioqui-2.0.1/src/aioqui/widgets/extensions/splitter_widget_ext.py
+-rw-rw-rw-   0        0        0      667 2023-05-15 07:22:27.000000 aioqui-2.0.1/src/aioqui/widgets/frame.py
+-rw-rw-rw-   0        0        0     2349 2023-05-16 21:16:28.000000 aioqui-2.0.1/src/aioqui/widgets/input.py
+-rw-rw-rw-   0        0        0     1347 2023-05-16 21:16:28.000000 aioqui-2.0.1/src/aioqui/widgets/label.py
+-rw-rw-rw-   0        0        0     1328 2023-05-16 21:18:22.000000 aioqui-2.0.1/src/aioqui/widgets/layout.py
+drwxrwxrwx   0        0        0        0 2023-05-16 21:21:00.699550 aioqui-2.0.1/src/aioqui/widgets/qss/
+-rw-rw-rw-   0        0        0      160 2023-05-16 20:13:01.000000 aioqui-2.0.1/src/aioqui/widgets/qss/__init__.py
+-rw-rw-rw-   0        0        0      653 2023-05-16 20:25:11.000000 aioqui-2.0.1/src/aioqui/widgets/qss/colors.py
+-rw-rw-rw-   0        0        0     1491 2023-05-16 20:59:19.000000 aioqui-2.0.1/src/aioqui/widgets/qss/date_time.py
+-rw-rw-rw-   0        0        0      306 2023-05-16 21:06:26.000000 aioqui-2.0.1/src/aioqui/widgets/qss/image_button.py
+-rw-rw-rw-   0        0        0      829 2023-05-16 21:12:30.000000 aioqui-2.0.1/src/aioqui/widgets/qss/popup.py
+-rw-rw-rw-   0        0        0       24 2023-05-16 20:13:39.000000 aioqui-2.0.1/src/aioqui/widgets/qss/scrollbar.py
+-rw-rw-rw-   0        0        0      436 2023-05-16 20:17:25.000000 aioqui-2.0.1/src/aioqui/widgets/qss/searchbar.py
+-rw-rw-rw-   0        0        0     1716 2023-05-16 21:16:52.000000 aioqui-2.0.1/src/aioqui/widgets/scroll_area.py
+-rw-rw-rw-   0        0        0     1184 2023-05-15 07:23:03.000000 aioqui-2.0.1/src/aioqui/widgets/selector.py
+-rw-rw-rw-   0        0        0      842 2023-05-16 21:16:52.000000 aioqui-2.0.1/src/aioqui/widgets/slider.py
+-rw-rw-rw-   0        0        0      270 2023-05-16 21:16:52.000000 aioqui-2.0.1/src/aioqui/widgets/spacer.py
+-rw-rw-rw-   0        0        0     1560 2023-05-16 21:16:52.000000 aioqui-2.0.1/src/aioqui/widgets/splitter.py
+-rw-rw-rw-   0        0        0     1139 2023-05-16 21:16:57.000000 aioqui-2.0.1/src/aioqui/widgets/stacked_widget.py
+-rw-rw-rw-   0        0        0      327 2023-05-15 07:24:09.000000 aioqui-2.0.1/src/aioqui/widgets/statusbar.py
+-rw-rw-rw-   0        0        0      587 2023-05-15 07:24:24.000000 aioqui-2.0.1/src/aioqui/widgets/widget.py
+-rw-rw-rw-   0        0        0      516 2023-05-16 21:17:28.000000 aioqui-2.0.1/src/aioqui/widgets/window.py
+drwxrwxrwx   0        0        0        0 2023-05-16 21:21:00.354984 aioqui-2.0.1/src/aioqui.egg-info/
+-rw-rw-rw-   0        0        0     2629 2023-05-16 21:21:00.000000 aioqui-2.0.1/src/aioqui.egg-info/PKG-INFO
+-rw-rw-rw-   0        0        0    13416 2023-05-16 21:21:00.000000 aioqui-2.0.1/src/aioqui.egg-info/SOURCES.txt
+-rw-rw-rw-   0        0        0        1 2023-05-16 21:21:00.000000 aioqui-2.0.1/src/aioqui.egg-info/dependency_links.txt
+-rw-rw-rw-   0        0        0       44 2023-05-16 21:21:00.000000 aioqui-2.0.1/src/aioqui.egg-info/requires.txt
+-rw-rw-rw-   0        0        0       16 2023-05-16 21:21:00.000000 aioqui-2.0.1/src/aioqui.egg-info/top_level.txt
```

### Comparing `aioqui-2.0.0/LICENSE.txt` & `aioqui-2.0.1/LICENSE.txt`

 * *Files identical despite different names*

### Comparing `aioqui-2.0.0/PKG-INFO` & `aioqui-2.0.1/PKG-INFO`

 * *Files 5% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: aioqui
-Version: 2.0.0
+Version: 2.0.1
 Summary: Asynchronous GUI framework based on PySide6
 Author-email: cxllmerichie <cxllmerichie@gmail.com>
 Maintainer-email: cxllmerichie <cxllmerichie@gmail.com>
 License: MIT License
         
         Copyright (c) 2022-2023 cxllmerichie
```

### Comparing `aioqui-2.0.0/pyproject.toml` & `aioqui-2.0.1/pyproject.toml`

 * *Files 0% similar despite different names*

```diff
@@ -1,14 +1,14 @@
 [build-system]
 requires = ["setuptools>=63.2"]
 build-backend = "setuptools.build_meta"
 
 [project]
 name = "aioqui"
-version = "2.0.0"
+version = "2.0.1"
 authors = [
     { name="cxllmerichie", email="cxllmerichie@gmail.com" },
 ]
 maintainers = [
     { name="cxllmerichie", email="cxllmerichie@gmail.com" },
 ]
 description = "Asynchronous GUI framework based on PySide6"
```

### Comparing `aioqui-2.0.0/src/aioqui/.assets/icons/aperture.svg` & `aioqui-2.0.1/src/aioqui/.assets/icons/aperture.svg`

 * *Files identical despite different names*

### Comparing `aioqui-2.0.0/src/aioqui/.assets/icons/cloud-drizzle.svg` & `aioqui-2.0.1/src/aioqui/.assets/icons/cloud-drizzle.svg`

 * *Files identical despite different names*

### Comparing `aioqui-2.0.0/src/aioqui/.assets/icons/cloud-snow.svg` & `aioqui-2.0.1/src/aioqui/.assets/icons/cloud-snow.svg`

 * *Files identical despite different names*

### Comparing `aioqui-2.0.0/src/aioqui/.assets/icons/codesandbox.svg` & `aioqui-2.0.1/src/aioqui/.assets/icons/codesandbox.svg`

 * *Files identical despite different names*

### Comparing `aioqui-2.0.0/src/aioqui/.assets/icons/cpu.svg` & `aioqui-2.0.1/src/aioqui/.assets/icons/cpu.svg`

 * *Files identical despite different names*

### Comparing `aioqui-2.0.0/src/aioqui/.assets/icons/figma.svg` & `aioqui-2.0.1/src/aioqui/.assets/icons/figma.svg`

 * *Files identical despite different names*

### Comparing `aioqui-2.0.0/src/aioqui/.assets/icons/film.svg` & `aioqui-2.0.1/src/aioqui/.assets/icons/film.svg`

 * *Files identical despite different names*

### Comparing `aioqui-2.0.0/src/aioqui/.assets/icons/github.svg` & `aioqui-2.0.1/src/aioqui/.assets/icons/github.svg`

 * *Files identical despite different names*

### Comparing `aioqui-2.0.0/src/aioqui/.assets/icons/life-buoy.svg` & `aioqui-2.0.1/src/aioqui/.assets/icons/life-buoy.svg`

 * *Files identical despite different names*

### Comparing `aioqui-2.0.0/src/aioqui/.assets/icons/loader.svg` & `aioqui-2.0.1/src/aioqui/.assets/icons/loader.svg`

 * *Files identical despite different names*

### Comparing `aioqui-2.0.0/src/aioqui/.assets/icons/package.svg` & `aioqui-2.0.1/src/aioqui/.assets/icons/package.svg`

 * *Files identical despite different names*

### Comparing `aioqui-2.0.0/src/aioqui/.assets/icons/phone-call.svg` & `aioqui-2.0.1/src/aioqui/.assets/icons/phone-call.svg`

 * *Files identical despite different names*

### Comparing `aioqui-2.0.0/src/aioqui/.assets/icons/phone-forwarded.svg` & `aioqui-2.0.1/src/aioqui/.assets/icons/phone-forwarded.svg`

 * *Files identical despite different names*

### Comparing `aioqui-2.0.0/src/aioqui/.assets/icons/phone-incoming.svg` & `aioqui-2.0.1/src/aioqui/.assets/icons/phone-incoming.svg`

 * *Files identical despite different names*

### Comparing `aioqui-2.0.0/src/aioqui/.assets/icons/phone-missed.svg` & `aioqui-2.0.1/src/aioqui/.assets/icons/phone-missed.svg`

 * *Files identical despite different names*

### Comparing `aioqui-2.0.0/src/aioqui/.assets/icons/phone-off.svg` & `aioqui-2.0.1/src/aioqui/.assets/icons/phone-off.svg`

 * *Files identical despite different names*

### Comparing `aioqui-2.0.0/src/aioqui/.assets/icons/phone-outgoing.svg` & `aioqui-2.0.1/src/aioqui/.assets/icons/phone-outgoing.svg`

 * *Files identical despite different names*

### Comparing `aioqui-2.0.0/src/aioqui/.assets/icons/phone.svg` & `aioqui-2.0.1/src/aioqui/.assets/icons/phone.svg`

 * *Files identical despite different names*

### Comparing `aioqui-2.0.0/src/aioqui/.assets/icons/settings.svg` & `aioqui-2.0.1/src/aioqui/.assets/icons/settings.svg`

 * *Files identical despite different names*

### Comparing `aioqui-2.0.0/src/aioqui/.assets/icons/slack.svg` & `aioqui-2.0.1/src/aioqui/.assets/icons/slack.svg`

 * *Files identical despite different names*

### Comparing `aioqui-2.0.0/src/aioqui/.assets/icons/sliders.svg` & `aioqui-2.0.1/src/aioqui/.assets/icons/sliders.svg`

 * *Files identical despite different names*

### Comparing `aioqui-2.0.0/src/aioqui/.assets/icons/sun.svg` & `aioqui-2.0.1/src/aioqui/.assets/icons/sun.svg`

 * *Files identical despite different names*

### Comparing `aioqui-2.0.0/src/aioqui/.assets/icons/sunrise.svg` & `aioqui-2.0.1/src/aioqui/.assets/icons/sunrise.svg`

 * *Files identical despite different names*

### Comparing `aioqui-2.0.0/src/aioqui/.assets/icons/sunset.svg` & `aioqui-2.0.1/src/aioqui/.assets/icons/sunset.svg`

 * *Files identical despite different names*

### Comparing `aioqui-2.0.0/src/aioqui/.assets/icons/wifi-off.svg` & `aioqui-2.0.1/src/aioqui/.assets/icons/wifi-off.svg`

 * *Files identical despite different names*

### Comparing `aioqui-2.0.0/src/aioqui/.assets/icons/youtube.svg` & `aioqui-2.0.1/src/aioqui/.assets/icons/youtube.svg`

 * *Files identical despite different names*

### Comparing `aioqui-2.0.0/src/aioqui/context/context_obj.py` & `aioqui-2.0.1/src/aioqui/context/context_obj.py`

 * *Files 11% similar despite different names*

```diff
@@ -1,28 +1,29 @@
-from PySide6.QtWidgets import (
-    QWidget, QPushButton, QLabel, QFrame, QLineEdit, QTextEdit, QPlainTextEdit, QStackedWidget, QComboBox, QSlider
-)
-from PySide6.QtCore import QObject, Qt
+from PySide6.QtCore import QObject, Qt, Signal
 from contextlib import suppress
 from loguru import logger
 import uuid
 
 from .contextapi import CONTEXT
-from ..types import QSS, Size, Event, Icon
-from ..enums import Alignment, SizePolicy
+from ..types import QSS, Size, Event, Icon, Parent
+from src.aioqui.types.enums import Alignment, SizePolicy
 
 
 class ContextObj:
+    _emmitable_event: Signal = Signal()
     __blacklist: dict[str, list[str]] = {}
 
-    def __init__(self, parent: QWidget = None, name: str = str(uuid.uuid4()), visible: bool = True):
+    def __init__(self: QObject, parent: Parent = None, name: str = str(uuid.uuid4()), visible: bool = True):
         if parent and name:
             self.setObjectName(name)
+            # make `self` accessible from `parent`
             self.__register(parent, name, self)
+            # make `parent` accessible from `self`
             self.__register(self, parent.objectName(), parent)
+            # make `self` accessible from global `CONTEXT`
             self.__register(CONTEXT, name, self)
 
             self.core = parent
             while p := self.core.parent():
                 self.core = p
         else:
             attributes = []
@@ -32,37 +33,36 @@
                 attributes.append('`name`')
             if CONTEXT.debug:
                 logger.warning(f"{self.__class__.__name__} not registered in `ContextAPI` since {' and '.join(attributes)} not specified")
 
         with suppress(Exception):
             self.setVisible(visible)
 
-    def __register(self, parent: object, name: str, child: QWidget) -> None:
+    def __register(self, parent: object, name: str, child: object) -> None:
         """
         Check if object not in `blacklist`, then register, otherwise show warning
         Check if object already registered, push its name to `blacklist` unregister and show warning, otherwise register
         :param parent:
         :param name:
         :param child:
         :return:
         """
         key = parent.__class__.__name__
         self.__blacklist[key] = self.__blacklist.get(key, [])
         if name not in self.__blacklist[key]:
-            try:
-                getattr(parent, name)
+            if hasattr(parent, name):
                 delattr(parent, name)
                 self.__blacklist[key].append(name)
                 if CONTEXT.debug:
                     logger.warning(f'{name} already registered in {key}')
-            except AttributeError:
+            else:
                 setattr(parent, name, child)
 
     async def _apply(
-            self,
+            self: QObject,
             *,
             # Sizes
             policy: tuple[SizePolicy.SizePolicy, SizePolicy.SizePolicy] = None,
             vpolicy: SizePolicy.SizePolicy = None,
             hpolicy: SizePolicy.SizePolicy = None,
 
             # margins: ? = ?,
@@ -91,15 +91,16 @@
             on_close: Event = None,
             on_resize: Event = None,
 
             # Common
             text: str = None,
             placeholder: str = None,
             icon: Icon = None,
-            disabled: bool = None
+            disabled: bool = None,
+            qss: QSS = None,
     ) -> 'ContextObj':
         """
         :param policy:
         :param vpolicy:
         :param hpolicy:
         :param alignment:
         :param size:
@@ -115,83 +116,89 @@
         :param fixed_width:
         :param fixed_height:
         """
         if policy:
             self.setSizePolicy(*policy)
             if vpolicy or hpolicy:
                 self._size_warning()
-        else:
+        elif vpolicy or hpolicy:
             policy = self.sizePolicy()
             if vpolicy:
                 policy.setVerticalPolicy(vpolicy)
-            elif hpolicy:
+            if hpolicy:
                 policy.setHorizontalPolicy(hpolicy)
             self.setSizePolicy(policy)
 
         if alignment:
             self.setAlignment(alignment)
 
         if size:
-            self.resize(*size.size)
+            self.resize(*size)
             if width or height:
                 self._size_warning()
         elif width:
             self.resize(width, self.height())
         elif height:
             self.resize(self.width(), height)
 
         if min_size:
-            self.setMinimumSize(*min_size.size)
+            self.setMinimumSize(*min_size)
             if min_width or min_height:
                 self._size_warning()
         elif min_width:
             self.setMinimumWidth(min_width)
         elif min_height:
             self.setMinimumHeight(min_height)
 
         if max_size:
-            self.setMaximumSize(*max_size.size)
+            self.setMaximumSize(*max_size)
             if max_width or max_height:
                 self._size_warning()
         elif max_width:
             self.setMaximumWidth(max_width)
         elif max_height:
             self.setMaximumHeight(max_height)
 
         if fixed_size:
-            self.setFixedSize(*fixed_size.size)
+            self.setFixedSize(*fixed_size)
             if fixed_width or fixed_height:
                 self._size_warning()
         elif fixed_width:
             self.setFixedWidth(fixed_width)
         elif fixed_height:
             self.setFixedHeight(fixed_height)
         """
         :param on_click:
         :param on_change:
         :param on_close:
         :param on_resize:
         """
         if on_click:
-            if isinstance(self, QPushButton):
-                await self._connect_str_signal('clicked', on_click)
-            elif isinstance(self, (QLabel, QFrame)):
-                self.mousePressEvent = lambda event: self._emit(on_click)
+            if hasattr(self, 'clicked'):  # QPushButton, ...
+                await self._connect_event(self.clicked, on_click)
+            elif hasattr(self, 'mousePressEvent'):  # QLabel, QFrame, ...
+                self.mousePressEvent = lambda event: self.emit_event(on_click)
             else:
                 self._event_error('on_click')
 
         if on_change:
-            if isinstance(self, (QLineEdit, QTextEdit, QPlainTextEdit)):
-                await self._connect_str_signal('textChanged', on_change)
-            elif isinstance(self, QStackedWidget):
-                await self._connect_str_signal('currentChanged', on_change)
-            elif isinstance(self, QComboBox):
-                await self._connect_str_signal('currentTextChanged', on_change)
-            elif isinstance(self, QSlider):
-                await self._connect_str_signal('valueChanged', on_change)
+            if hasattr(self, 'textChanged'):  # QLineEdit, QTextEdit, QPlainTextEdit, ...
+                await self._connect_event(self.textChanged, on_change)
+            elif hasattr(self, 'currentChanged'):  # QStackedWidget, ...
+                await self._connect_event(self.currentChanged, on_change)
+            elif hasattr(self, 'currentTextChanged'):  # QComboBox, ...
+                await self._connect_event(self.currentTextChanged, on_change)
+            elif hasattr(self, 'valueChanged'):  # QSlider, ...
+                await self._connect_event(self.valueChanged, on_change)
+            elif hasattr(self, 'dateTimeChanged'):  # QDateTimeEdit, ...
+                await self._connect_event(self.dateTimeChanged, on_change)
+            elif hasattr(self, 'dateChanged'):  # QDateEdit, ...
+                await self._connect_event(self.dateChanged, on_change)
+            elif hasattr(self, 'timeChanged'):  # QTimeEdit, ...
+                await self._connect_event(self.timeChanged, on_change)
             else:
                 self._event_error('on_change')
 
         # if on_close:
         #     def close(self) -> bool:
         #         print(self)
         #         rv = self.close()
@@ -206,54 +213,64 @@
         #     obj.resizeEvent = lambda event: self.emit(lambda: resizeEvent(event))
 
         """
         :param text:
         :param placeholder:
         :param icon:
         :param disabled:
+        :param qss:
         """
         if text:
-            self.setText(text)
+            if hasattr(self, 'setText'):
+                self.setText(text)
+            elif hasattr(self, 'setCurrentText'):
+                self.setCurrentText(text)
+            elif hasattr(self, 'setPlainText'):
+                self.setPlainText(text)
+
         if placeholder:
             self.setPlaceholderText(text)
+
         if icon:
-            if isinstance(self, QPushButton):
+            if hasattr(self, 'setIcon'):  # QPushButton, ...
                 self.setIcon(icon.icon)
                 self.setIconSize(icon.size)
-            elif isinstance(self, QLabel):
+            elif hasattr(self, 'setPixmap'):  # QLabel, ...
                 self.setPixmap(icon.icon.pixmap(icon.size))
+
         if disabled:
             self.setDisabled(disabled)
+
+        self.qss = qss
+
         return self
 
     def _size_warning(self: QObject) -> None:
         logger.warning(f'Review `{self.objectName()}.sized()` arguments')
 
-    async def _connect_str_signal(self: QObject, signal: str, event: Event):
-        signal = getattr(self, signal)
+    @staticmethod
+    async def _connect_event(signal: Signal, event: Event):
+        # signal.connect(slot) is faster that using getattr(self, signalName).connect(slot)
         with suppress(Exception):
             signal.disconnect()
         signal.connect(event)
 
-    @staticmethod
-    def _emit(event: Event) -> None:
-        # _emit created and used because event might be sync, async and async wrapped with asyncSlot
-        btn = QPushButton()
-        btn.setVisible(False)
-        btn.clicked.connect(event)
-        btn.click()
-        btn.deleteLater()
+    def emit_event(self, event: Event) -> None:  # created because event might be sync, async and wrapped with asyncSlot
+        with suppress(Exception):
+            self._emmitable_event.disconnect()
+        self._emmitable_event.connect(event)
+        self._emmitable_event.emit()
 
     def _event_error(self: QObject, event: str) -> None:
         logger.error(f'event `{event}` is not implemented for `{self.objectName()}\'s` type: {type(self)}')
 
     @property
-    def qss(self) -> str:
+    def qss(self: QObject) -> str:
         return self.styleSheet()
 
     @qss.setter
-    def qss(self, qss: QSS) -> None:
+    def qss(self: QObject, qss: QSS) -> None:
         if qss:
             if not isinstance(qss, str):
                 qss = ''.join(qss)
             self.setStyleSheet(qss)
             self.setAttribute(Qt.WA_StyledBackground, True)
```

### Comparing `aioqui-2.0.0/src/aioqui/enums/alignment.py` & `aioqui-2.0.1/src/aioqui/types/enums/alignment.py`

 * *Files identical despite different names*

### Comparing `aioqui-2.0.0/src/aioqui/misc/aiorequest.py` & `aioqui-2.0.1/src/aioqui/misc/aiorequest.py`

 * *Files identical despite different names*

### Comparing `aioqui-2.0.0/src/aioqui/misc/animation.py` & `aioqui-2.0.1/src/aioqui/misc/animation.py`

 * *Files 19% similar despite different names*

```diff
@@ -1,12 +1,11 @@
 from PySide6.QtCore import QPropertyAnimation, Property, QObject
 from typing import Any, Callable
 
 from ..qasyncio import asyncSlot
-from ..context import ContextObj
 
 
 async def create(  # uncompleted
         obj: QObject,
         pname: str,
         ptype: type,
         duration: float,
@@ -30,8 +29,8 @@
         obj.animation = QPropertyAnimation(obj, pname.encode())
         obj.animation.setDuration(int(duration * 1000))
         obj.animation.setStartValue(vrange[0])
         obj.animation.setEndValue(vrange[1])
         obj.animation.start()
 
     setattr(obj, pname, Property(ptype, getter, setter))
-    return lambda: ContextObj._emit(animate)
+    return lambda: obj.emit_event(animate)
```

### Comparing `aioqui-2.0.0/src/aioqui/misc/conthrq.py` & `aioqui-2.0.1/src/aioqui/misc/conthrq.py`

 * *Files identical despite different names*

### Comparing `aioqui-2.0.0/src/aioqui/misc/fileops.py` & `aioqui-2.0.1/src/aioqui/misc/fileops.py`

 * *Files identical despite different names*

### Comparing `aioqui-2.0.0/src/aioqui/misc/qss_parser.py` & `aioqui-2.0.1/src/aioqui/misc/qss_parser.py`

 * *Files identical despite different names*

### Comparing `aioqui-2.0.0/src/aioqui/misc/uvithread.py` & `aioqui-2.0.1/src/aioqui/misc/uvithread.py`

 * *Files identical despite different names*

### Comparing `aioqui-2.0.0/src/aioqui/qasyncio.py` & `aioqui-2.0.1/src/aioqui/qasyncio.py`

 * *Files identical despite different names*

### Comparing `aioqui-2.0.0/src/aioqui/types/icon.py` & `aioqui-2.0.1/src/aioqui/types/icon.py`

 * *Files 14% similar despite different names*

```diff
@@ -1,40 +1,39 @@
 from PySide6.QtGui import QPixmap, QIcon, QImage
 from PySide6.QtCore import QSize, QBuffer, QIODevice
-# from loguru import logger
+from loguru import logger
 import base64
 import os
 
 from .size import Size
 
 
 class Icon:
-    IconType = type[QIcon, str, bytes]
-    SizeType = type[Size, QSize, tuple[int, int], Ellipsis, None]
-
+    icon_t: type = QIcon | str | bytes
+    size_t: type = QSize | Size | tuple[int, int] | None
 
     root = os.path.join(os.path.dirname(__file__), os.path.pardir, '.assets', 'icons')
     __icon: QIcon = None
     __size: QSize = None
 
-    def __init__(self, instance: IconType, size: SizeType = None):
+    def __init__(self, instance: icon_t, size: size_t = None):
         self.icon = instance
         if size:
             self.size = size
 
     @property
     def icon(self) -> QIcon:
         return self.__icon
 
     @property
     def size(self) -> QSize:
         return self.__size
 
     @icon.setter
-    def icon(self, instance: IconType) -> None:
+    def icon(self, instance: icon_t) -> None:
         """
 
         :param instance: QIcon, string filename with already set Icon.root, icon bytes
         :return:
         """
         def from_bytes(icon_bytes: bytes):
             pixmap = QPixmap()
@@ -58,40 +57,40 @@
             from_bytes(instance)
         else:
             self.__icon = QIcon()
             # logger.warning(f'unknown type ({type(instance)}) of instance ({instance}), can not set Icon.icon')
         self.icon.addPixmap(self.__icon.pixmap(1000), mode=QIcon.Disabled)  # fix of `QPushButton.setDisabled()`
 
     @size.setter
-    def size(self, size: SizeType) -> None:
+    def size(self, size: size_t) -> None:
         """
 
         :param size: QSize, qcontextapi.Size, tuple[int, int]
         :return:
         """
         if isinstance(size, tuple):
             self.__size = QSize(*size)
         elif isinstance(size, Size):
             self.__size = QSize(*size.size)
         elif isinstance(size, QSize):
             self.__size = size
         else:
             raise AttributeError(f'unknown type ({type(size)}) of size ({size}), can not set Icon.size')
 
-    def adjusted(self, icon: IconType = None, size: SizeType = None) -> 'Icon':
-        # if not icon and not size:
-        #     logger.warning('Icon.adjusted() called without parameters. Redundant call.')
+    def adjusted(self, icon: icon_t = None, size: size_t = None) -> 'Icon':
+        if not icon and not size:
+            logger.info('Icon.adjusted() called without parameters. Redundant call.')
         if icon:
             self.icon = icon
         if size:
             self.size = size
         return self
 
     @staticmethod
-    def bytes(icon: IconType, size: SizeType = None) -> bytes:
+    def bytes(icon: icon_t, size: size_t = None) -> bytes:
         icon = Icon(icon, size)
         # image = QImage(icon.icon.pixmap(icon.size).toImage())
         image = QImage(icon.icon.pixmap(QSize(512, 512)).toImage())
         buffer = QBuffer()
         buffer.open(QIODevice.WriteOnly)
         image.save(buffer, 'JPG')
         image_bytes = buffer.data()
```

### Comparing `aioqui-2.0.0/src/aioqui/widgets/__init__.py` & `aioqui-2.0.1/src/aioqui/widgets/__init__.py`

 * *Files 14% similar despite different names*

```diff
@@ -1,8 +1,10 @@
-from ..types import Parent  # to be used together with other imports
+# to be used together with other imports
+from ..types import Parent
+from . import qss
 # exist normally, but added to keep context completed
 from .window import Window
 from .statusbar import StatusBar
 # standard frame-like
 from .widget import Widget
 from .frame import Frame
 # specific frame-like
@@ -11,10 +13,11 @@
 from .scroll_area import ScrollArea
 # modular
 from .button import Button
 from .label import Label
 from .input import Input
 from .selector import Selector
 from .slider import Slider
+from .date_time import DateTime
 # layout
 from .layout import Layout
 from .spacer import Spacer
```

### Comparing `aioqui-2.0.0/src/aioqui/widgets/button.py` & `aioqui-2.0.1/src/aioqui/widgets/button.py`

 * *Files identical despite different names*

### Comparing `aioqui-2.0.0/src/aioqui/widgets/custom/error_label.py` & `aioqui-2.0.1/src/aioqui/widgets/custom/error_label.py`

 * *Files 10% similar despite different names*

```diff
@@ -1,21 +1,21 @@
 from PySide6.QtCore import QPropertyAnimation, Property
-from PySide6.QtWidgets import QWidget
 from time import sleep
 
 from ...misc import ConditionalThreadQueue
 from ..label import Label
 from ...qasyncio import asyncSlot
+from ...types import Parent
 
 
 class ErrorLabel(Label):
     __duration: float = 0.5
     __ctq: ConditionalThreadQueue = ConditionalThreadQueue()
 
-    def __init__(self, parent: QWidget, name: str = None, visible: bool = True):
+    def __init__(self, parent: Parent, name: str = None, visible: bool = True):
         super().__init__(parent, name if name else self.__class__.__name__, visible)
 
     async def init(
             self, *,
             _=None,
             **kwargs
     ) -> 'ErrorLabel':
@@ -32,15 +32,15 @@
         def pre():
             self._set_opacity(1)
             Label.setText(self, text)
             self.setVisible(True)
             sleep(delay)
 
         def post():
-            Label._emit(self.reduce)
+            self.emit_event(self.reduce)
 
         self.__duration = duration
         self.__ctq.new(pre, post)
 
     @asyncSlot()
     async def reduce(self):
         self.animation = QPropertyAnimation(self, b"_opacity")
@@ -48,13 +48,13 @@
         self.animation.setStartValue(1.0)
         self.animation.setEndValue(0.0)
         self.animation.start()
 
     def _get_opacity(self):
         return self.__opacity
 
-    def _set_opacity(self, opacity):
+    def _set_opacity(self, opacity: float):
         self.__opacity = opacity
         self.setStyleSheet(f'color: rgba(255, 0, 0, {opacity});')
 
     __opacity: float = 1
     _opacity: Property = Property(float, _get_opacity, _set_opacity)
```

### Comparing `aioqui-2.0.0/src/aioqui/widgets/custom/image_button.py` & `aioqui-2.0.1/src/aioqui/widgets/input.py`

 * *Files 24% similar despite different names*

```diff
@@ -1,64 +1,73 @@
-from PySide6.QtWidgets import QWidget, QFileDialog
-from PySide6.QtGui import QIcon
-from contextlib import suppress
-
-from ..button import Button
-from src.aioqui.widgets.custom.popup import Popup
-from ...types import Icon, Size
-from ...qasyncio import asyncSlot
+from PySide6.QtWidgets import QLineEdit, QTextEdit, QPlainTextEdit
+from abc import ABC
 
+from ..types import QSS, Parent, EchoMode
+from .extensions import InputExt
+from ..context import ContextObj
 
-class ImageButton(Button):
-    def __init__(self, parent: QWidget, name: str = None, visible: bool = True):
-        super().__init__(parent, name if name else self.__class__.__name__, visible)
-        self.image_bytes = None
+
+class LineInput(ContextObj, InputExt, QLineEdit):
+    def __init__(self, parent: Parent, name: str, visible: bool = True, qss: QSS = None):
+        QLineEdit.__init__(self, parent)
+        ContextObj.__init__(self, parent, name, visible)
+        self.qss = qss
+
+    async def init(
+            self, *,
+            hidden: bool = False,
+            **kwargs
+    ) -> 'LineInput':
+        if hidden:
+            self.hide_echo()
+        return await self._apply(**kwargs)
+
+    def hide_echo(self):
+        self.setEchoMode(EchoMode.Hidden)
+
+    def show_echo(self):
+        self.setEchoMode(EchoMode.Default)
+
+    def toggle_echo(self):
+        self.hide_echo() if self.echoMode() == EchoMode.Default else self.show_echo()
+
+
+class ReachInput(ContextObj, InputExt, QTextEdit):
+    def __init__(self, parent: Parent, name: str, visible: bool = True, qss: QSS = None):
+        QTextEdit.__init__(self, parent)
+        ContextObj.__init__(self, parent, name, visible)
+        self.qss = qss
+
+    async def init(
+            self, *,
+            _,
+            **kwargs
+    ) -> 'ReachInput':
+        return await self._apply(**kwargs)
+
+
+class PlainInput(ContextObj, InputExt, QPlainTextEdit):
+    def __init__(self, parent: Parent, name: str, visible: bool = True, qss: QSS = None):
+        QPlainTextEdit.__init__(self, parent)
+        ContextObj.__init__(self, parent, name, visible)
+        self.qss = qss
 
     async def init(
             self, *,
-            icon: Icon, slot: callable = lambda: None, directory: str = ''
-    ) -> 'ImageButton':
-        await super().init(icon=icon, on_click=lambda: self.choose_image(slot, directory))
-        self.RemoveImageBtn = await Button(self, f'{self.objectName()}RemoveImageBtn').init(
-            icon=Icon('x-circle.svg', (30, 30)), fixed_size=Size(30, 30),
-            on_click=lambda: Popup(self.core).display(message=f'Remove icon?', on_success=self.remove_icon)
-        )
-        self.RemoveImageBtn.move(self.width() - 30, 0)
-        self.RemoveImageBtn.setStyleSheet(f'''
-            #{self.objectName()}RemoveImageBtn {{background-color: transparent; border-radius: 14px;}}
-            #{self.objectName()}RemoveImageBtn:hover {{background-color: rgba(255, 255, 255, 0.3);}}
-        ''')
-        return self
-
-    @property
-    def image_bytes_str(self) -> str | None:
-        return str(self.image_bytes) if self.image_bytes else None
-
-    def remove_icon(self):
-        super().setIcon(QIcon())
-        self.image_bytes = None
-        with suppress(AttributeError):
-            self.RemoveImageBtn.setVisible(False)
-
-    def setIcon(self, icon: QIcon) -> None:
-        self.image_bytes = Icon.bytes(icon, self.iconSize())
-        super().setIcon(icon)
-        with suppress(AttributeError):
-            self.RemoveImageBtn.setVisible(True)
-
-    def setDisabled(self, disabled: bool) -> None:
-        with suppress(AttributeError):
-            self.RemoveImageBtn.setVisible(not disabled)
-        super().setDisabled(disabled)
-
-    def setEnabled(self, enabled: bool) -> None:
-        with suppress(AttributeError):
-            self.RemoveImageBtn.setVisible(enabled)
-        super().setEnabled(enabled)
-
-    @asyncSlot()
-    async def choose_image(self, slot: callable = lambda: None, directory: str = ''):
-        filepath, _ = QFileDialog.getOpenFileName(self, 'Choose image', directory, 'Images (*.jpg)')
-        if filepath:
-            with open(filepath, 'rb') as file:
-                self.setIcon(Icon(file.read()).icon)
-            slot()
+            _,
+            **kwargs
+    ) -> 'PlainInput':
+        return await self._apply(**kwargs)
+
+
+class Input(ABC, EchoMode):
+    @staticmethod
+    def line(parent: Parent, name: str, visible: bool = True, qss: QSS = None) -> LineInput:
+        return LineInput(parent, name, visible, qss)
+
+    @staticmethod
+    def reach(parent: Parent, name: str, visible: bool = True, qss: QSS = None) -> ReachInput:
+        return ReachInput(parent, name, visible, qss)
+
+    @staticmethod
+    def plain(parent: Parent, name: str, visible: bool = True, qss: QSS = None) -> PlainInput:
+        return PlainInput(parent, name, visible, qss)
```

### Comparing `aioqui-2.0.0/src/aioqui/widgets/custom/menu_button.py` & `aioqui-2.0.1/src/aioqui/widgets/custom/menu_button.py`

 * *Files identical despite different names*

### Comparing `aioqui-2.0.0/src/aioqui/widgets/custom/searchbar.py` & `aioqui-2.0.1/src/aioqui/widgets/custom/searchbar.py`

 * *Files identical despite different names*

### Comparing `aioqui-2.0.0/src/aioqui/widgets/custom/state_icon_btn.py` & `aioqui-2.0.1/src/aioqui/widgets/custom/state_icon_btn.py`

 * *Files 5% similar despite different names*

```diff
@@ -22,18 +22,18 @@
         if if_unset_icon:
             self.setIcon(QIcon(if_unset_icon.icon))
             self.setIconSize(if_unset_icon.size)
         if if_set_icon:
             self.if_set_icon = if_set_icon
         if if_unset_icon:
             self.if_unset_icon = if_unset_icon
-        return await Button.init(self, on_click=lambda: self.__slot(pre_slot), **kwargs)
+        return await Button.init(self, on_click=lambda: self.__mainevent(pre_slot), **kwargs)
 
     @asyncSlot()
-    async def __slot(self, pre_slot: Callable[..., bool]) -> None:
+    async def __mainevent(self, pre_slot: Callable[..., bool]) -> None:
         # toggle to change state
         self.state = not self.state
         if not await pre_slot():
             # toggle once more to come back to prev state if `pre_slot` returns `False`
             self.state = not self.state
 
     @property
```

### Comparing `aioqui-2.0.0/src/aioqui/widgets/extensions/input_ext.py` & `aioqui-2.0.1/src/aioqui/widgets/extensions/input_ext.py`

 * *Files 1% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 from PySide6.QtWidgets import QTextEdit, QLineEdit, QPlainTextEdit
 
-from ...enums import EchoMode
+from ...types import EchoMode
 
 
 class InputExt(EchoMode):
     def setText(self, text: str) -> None:
         if isinstance(self, QLineEdit):
             QLineEdit.setText(self, text)
         elif isinstance(self, QTextEdit):
```

### Comparing `aioqui-2.0.0/src/aioqui/widgets/extensions/layout_ext.py` & `aioqui-2.0.1/src/aioqui/widgets/extensions/layout_ext.py`

 * *Files 5% similar despite different names*

```diff
@@ -1,12 +1,12 @@
 from PySide6.QtWidgets import QWidget, QLayoutItem, QSpacerItem
 from PySide6.QtCore import Qt, QObject
 from typing import Sequence, Iterable
 
-from ...enums import Alignment
+from ...types import Alignment
 
 
 class LayoutExt(Alignment):
     async def init(
             self, *,
             margins: tuple[int, ...] = (0, 0, 0, 0), spacing: int = 0, alignment: Qt.Alignment = None,
             items: Sequence[QObject] = ()
```

### Comparing `aioqui-2.0.0/src/aioqui/widgets/extensions/side_menu_ext.py` & `aioqui-2.0.1/src/aioqui/widgets/extensions/side_menu_ext.py`

 * *Files 1% similar despite different names*

```diff
@@ -1,8 +1,8 @@
-from ...enums import Orientation
+from ...types import Orientation
 
 
 class SideMenuExt:
     def __init__(self, expand_to: int, expand_orientation: Orientation.Orientation):
         self.expand_to: int = expand_to
         self.__expand_orientation: Orientation.Orientation = expand_orientation
```

### Comparing `aioqui-2.0.0/src/aioqui/widgets/extensions/splitter_widget_ext.py` & `aioqui-2.0.1/src/aioqui/widgets/extensions/splitter_widget_ext.py`

 * *Files 4% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 from PySide6.QtWidgets import QSplitter
 
-from ...enums import Orientation
+from ...types import Orientation
 
 
 class SplitterWidgetExt(Orientation):
     splitter: QSplitter
     __orientation: Orientation.Orientation
 
     def __init__(self, expand_to: int, expand_min: int = None, expand_max: int = None, collapsible: bool = True):
```

### Comparing `aioqui-2.0.0/src/aioqui/widgets/frame.py` & `aioqui-2.0.1/src/aioqui/widgets/frame.py`

 * *Files identical despite different names*

### Comparing `aioqui-2.0.0/src/aioqui/widgets/input.py` & `aioqui-2.0.1/src/aioqui/widgets/splitter.py`

 * *Files 26% similar despite different names*

```diff
@@ -1,74 +1,40 @@
-from PySide6.QtWidgets import QLineEdit, QTextEdit, QPlainTextEdit
-from abc import ABC
+from PySide6.QtWidgets import QSplitter
+from typing import Iterable
 
-from ..types import QSS, Parent
-from .extensions import InputExt
-from ..enums import EchoMode
+from .frame import Frame
+from .extensions import SplitterWidgetExt
 from ..context import ContextObj
+from ..types import QSS, Parent, Orientation
 
 
-class LineInput(ContextObj, InputExt, QLineEdit):
-    def __init__(self, parent: Parent, name: str, visible: bool = True, qss: QSS = None):
-        QLineEdit.__init__(self, parent)
+class Splitter(ContextObj, Orientation, QSplitter):
+    class Handle(Frame):
+        def __init__(self, parent: Parent, name: str):
+            super().__init__(parent, name, True)
+
+    class Widget(SplitterWidgetExt, Frame):
+        def __init__(self, parent: Parent, name: str, *, collapsible: bool = True,
+                     expand_to: int, expand_min: int = None, expand_max: int = None):
+            Frame.__init__(self, parent, name, True)
+            SplitterWidgetExt.__init__(self, expand_to, expand_min, expand_max, collapsible)
+
+    def __init__(self, parent: Parent, name: str, visible: bool = True, qss: QSS = None,
+                 orientation: Orientation.Orientation = Orientation.Horizontal):
+        QSplitter.__init__(self, orientation, parent)
         ContextObj.__init__(self, parent, name, visible)
         self.qss = qss
 
     async def init(
             self, *,
-            hidden: bool = False,
+            items: Iterable[Widget] = (),
             **kwargs
-    ) -> 'LineInput':
-        if hidden:
-            self.hide_echo()
+    ) -> 'Splitter':
+        for item in items:
+            self.addWidget(item)
         return await self._apply(**kwargs)
 
-    def hide_echo(self):
-        self.setEchoMode(EchoMode.Hidden)
-
-    def show_echo(self):
-        self.setEchoMode(EchoMode.Default)
-
-    def toggle_echo(self):
-        self.hide_echo() if self.echoMode() == EchoMode.Default else self.show_echo()
-
-
-class ReachInput(ContextObj, InputExt, QTextEdit):
-    def __init__(self, parent: Parent, name: str, visible: bool = True, qss: QSS = None):
-        QTextEdit.__init__(self, parent)
-        ContextObj.__init__(self, parent, name, visible)
-        self.qss = qss
-
-    async def init(
-            self, *,
-            _,
-            **kwargs
-    ) -> 'ReachInput':
-        return await self._apply(**kwargs)
-
-
-class PlainInput(ContextObj, InputExt, QPlainTextEdit):
-    def __init__(self, parent: Parent, name: str, visible: bool = True, qss: QSS = None):
-        QPlainTextEdit.__init__(self, parent)
-        ContextObj.__init__(self, parent, name, visible)
-        self.qss = qss
-
-    async def init(
-            self, *,
-            _,
-            **kwargs
-    ) -> 'PlainInput':
-        return await self._apply(**kwargs)
-
-
-class Input(ABC, EchoMode):
-    @staticmethod
-    def line(parent: Parent, name: str, visible: bool = True, qss: QSS = None) -> LineInput:
-        return LineInput(parent, name, visible, qss)
-
-    @staticmethod
-    def reach(parent: Parent, name: str, visible: bool = True, qss: QSS = None) -> ReachInput:
-        return ReachInput(parent, name, visible, qss)
-
-    @staticmethod
-    def plain(parent: Parent, name: str, visible: bool = True, qss: QSS = None) -> PlainInput:
-        return PlainInput(parent, name, visible, qss)
+    def addWidget(self, widget: Widget) -> None:
+        super().addWidget(widget)
+        widget.splitter = self
+        widget.orientation = self.orientation()
+        self.setCollapsible(self.count() - 1, widget.collapsible)
```

### Comparing `aioqui-2.0.0/src/aioqui/widgets/label.py` & `aioqui-2.0.1/src/aioqui/widgets/label.py`

 * *Files 3% similar despite different names*

```diff
@@ -1,12 +1,11 @@
 from PySide6.QtGui import QFontMetrics, QPaintEvent
 from PySide6.QtWidgets import QLabel
 
-from ..enums import Alignment, ElideMode, SizePolicy
-from ..types import Parent, QSS
+from ..types import Parent, QSS, Alignment, ElideMode, SizePolicy
 from ..context import ContextObj
 
 
 class Label(ContextObj, Alignment, SizePolicy, ElideMode, QLabel):
     __elide_mode: ElideMode.ElideMode
     __elide_text: str
```

### Comparing `aioqui-2.0.0/src/aioqui/widgets/layout.py` & `aioqui-2.0.1/src/aioqui/widgets/layout.py`

 * *Files 9% similar despite different names*

```diff
@@ -1,15 +1,14 @@
 from PySide6.QtWidgets import QVBoxLayout, QHBoxLayout
 from typing import Union
 from abc import ABC
 
-from ..types import Parent
+from ..types import Parent, Alignment, Orientation
 from .extensions import LayoutExt
 from ..context import ContextObj
-from ..enums import Alignment, Orientation
 
 
 class VerticalLayout(ContextObj, LayoutExt, QVBoxLayout):
     def __init__(self, parent: Parent = None, name: str = None):
         QVBoxLayout.__init__(self, parent)
         ContextObj.__init__(self, parent, name, True)
```

### Comparing `aioqui-2.0.0/src/aioqui/widgets/scroll_area.py` & `aioqui-2.0.1/src/aioqui/widgets/scroll_area.py`

 * *Files 2% similar despite different names*

```diff
@@ -1,16 +1,15 @@
 from PySide6.QtWidgets import QScrollArea
 from PySide6.QtCore import QObject
 from typing import Sequence, Iterable
 
 from .frame import Frame
 from .layout import Layout
 from ..context import ContextObj
-from ..enums import Orientation, ScrollPolicy
-from ..types import QSS, Parent
+from ..types import QSS, Parent, Orientation, ScrollPolicy
 
 
 class ScrollArea(ContextObj, ScrollPolicy, Orientation, QScrollArea):
     def __init__(self, parent: Parent, name: str, visible: bool = True, qss: QSS = None):
         QScrollArea.__init__(self, parent)
         ContextObj.__init__(self, parent, name, visible)
         self.qss = qss
```

### Comparing `aioqui-2.0.0/src/aioqui/widgets/selector.py` & `aioqui-2.0.1/src/aioqui/widgets/selector.py`

 * *Files identical despite different names*

### Comparing `aioqui-2.0.0/src/aioqui/widgets/slider.py` & `aioqui-2.0.1/src/aioqui/widgets/slider.py`

 * *Files 16% similar despite different names*

```diff
@@ -1,13 +1,12 @@
 from PySide6.QtWidgets import QSlider
 from PySide6.QtCore import Qt
 
 from ..context import ContextObj
-from ..enums import Orientation
-from ..types import Parent
+from ..types import Parent, Orientation
 
 
 class Slider(ContextObj, Orientation, QSlider):
     def __init__(self, parent: Parent, name: str, visible: bool = True,
                  orientation: Orientation.Orientation = Orientation.Horizontal):
         QSlider.__init__(self, orientation, parent)
         ContextObj.__init__(self, parent, name, visible)
```

### Comparing `aioqui-2.0.0/src/aioqui/widgets/splitter.py` & `aioqui-2.0.1/src/aioqui/widgets/stacked_widget.py`

 * *Files 24% similar despite different names*

```diff
@@ -1,41 +1,29 @@
-from PySide6.QtWidgets import QSplitter
+from PySide6.QtWidgets import QStackedWidget, QFrame
+from PySide6.QtCore import QObject
 from typing import Iterable
 
-from .frame import Frame
-from .extensions import SplitterWidgetExt
 from ..context import ContextObj
-from ..enums import Orientation
-from ..types import QSS, Parent
+from ..types import QSS, Parent, Alignment, Orientation
 
 
-class Splitter(ContextObj, Orientation, QSplitter):
-    class Handle(Frame):
-        def __init__(self, parent: Parent, name: str):
-            super().__init__(parent, name, True)
-
-    class Widget(SplitterWidgetExt, Frame):
-        def __init__(self, parent: Parent, name: str, *, collapsible: bool = True,
-                     expand_to: int, expand_min: int = None, expand_max: int = None):
-            Frame.__init__(self, parent, name, True)
-            SplitterWidgetExt.__init__(self, expand_to, expand_min, expand_max, collapsible)
-
-    def __init__(self, parent: Parent, name: str, visible: bool = True, qss: QSS = None,
-                 orientation: Orientation.Orientation = Orientation.Horizontal):
-        QSplitter.__init__(self, orientation, parent)
+class StackedWidget(ContextObj, Orientation, QStackedWidget):
+    def __init__(self, parent: Parent, name: str, visible: bool = True, qss: QSS = None):
+        QStackedWidget.__init__(self, parent)
         ContextObj.__init__(self, parent, name, visible)
         self.qss = qss
 
+        # workaround which includes override of `setCurrentIndex`, otherwise problems with `parent()`
+        self.addWidget(QFrame(self))  # QFrame is likely the most lightweight QWidget in Qt6
+
     async def init(
             self, *,
-            items: Iterable[Widget] = (),
+            alignment: Alignment.Alignment = Alignment.HCenter, items: Iterable[QObject] = (),
             **kwargs
-    ) -> 'Splitter':
+    ) -> 'StackedWidget':
+        self.layout().setAlignment(alignment)
         for item in items:
             self.addWidget(item)
         return await self._apply(**kwargs)
 
-    def addWidget(self, widget: Widget) -> None:
-        super().addWidget(widget)
-        widget.splitter = self
-        widget.orientation = self.orientation()
-        self.setCollapsible(self.count() - 1, widget.collapsible)
+    def setCurrentIndex(self, index: int) -> None:
+        super().setCurrentIndex(index + 1)
```

### Comparing `aioqui-2.0.0/src/aioqui/widgets/widget.py` & `aioqui-2.0.1/src/aioqui/widgets/widget.py`

 * *Files identical despite different names*

### Comparing `aioqui-2.0.0/src/aioqui/widgets/window.py` & `aioqui-2.0.1/src/aioqui/widgets/window.py`

 * *Files 22% similar despite different names*

```diff
@@ -1,11 +1,11 @@
 from PySide6.QtWidgets import QMainWindow
 
 from ..context import ContextObj
-from ..enums import WindowHint
+from ..types import WindowHint
 
 
 class Window(ContextObj, WindowHint, QMainWindow):
     def __init__(self, name: str, stylesheet: str = None):
         QMainWindow.__init__(self)
         self.setObjectName(name)
         if stylesheet:
```

### Comparing `aioqui-2.0.0/src/aioqui.egg-info/PKG-INFO` & `aioqui-2.0.1/src/aioqui.egg-info/PKG-INFO`

 * *Files 5% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: aioqui
-Version: 2.0.0
+Version: 2.0.1
 Summary: Asynchronous GUI framework based on PySide6
 Author-email: cxllmerichie <cxllmerichie@gmail.com>
 Maintainer-email: cxllmerichie <cxllmerichie@gmail.com>
 License: MIT License
         
         Copyright (c) 2022-2023 cxllmerichie
```

### Comparing `aioqui-2.0.0/src/aioqui.egg-info/SOURCES.txt` & `aioqui-2.0.1/src/aioqui.egg-info/SOURCES.txt`

 * *Files 8% similar despite different names*

```diff
@@ -299,55 +299,63 @@
 src/aioqui/.assets/icons/zap-off.svg
 src/aioqui/.assets/icons/zap.svg
 src/aioqui/.assets/icons/zoom-in.svg
 src/aioqui/.assets/icons/zoom-out.svg
 src/aioqui/context/__init__.py
 src/aioqui/context/context_obj.py
 src/aioqui/context/contextapi.py
-src/aioqui/enums/__init__.py
-src/aioqui/enums/alignment.py
-src/aioqui/enums/echo_mode.py
-src/aioqui/enums/elide_mode.py
-src/aioqui/enums/orientation.py
-src/aioqui/enums/scroll_policy.py
-src/aioqui/enums/size_policy.py
-src/aioqui/enums/window_hint.py
 src/aioqui/misc/__init__.py
 src/aioqui/misc/aiorequest.py
 src/aioqui/misc/animation.py
 src/aioqui/misc/conthrq.py
 src/aioqui/misc/fileops.py
 src/aioqui/misc/qss_parser.py
 src/aioqui/misc/utils.py
 src/aioqui/misc/uvithread.py
 src/aioqui/types/__init__.py
 src/aioqui/types/common.py
 src/aioqui/types/icon.py
 src/aioqui/types/size.py
+src/aioqui/types/enums/__init__.py
+src/aioqui/types/enums/alignment.py
+src/aioqui/types/enums/echo_mode.py
+src/aioqui/types/enums/elide_mode.py
+src/aioqui/types/enums/logic_button.py
+src/aioqui/types/enums/orientation.py
+src/aioqui/types/enums/scroll_policy.py
+src/aioqui/types/enums/size_policy.py
+src/aioqui/types/enums/window_hint.py
 src/aioqui/widgets/__init__.py
 src/aioqui/widgets/button.py
+src/aioqui/widgets/date_time.py
 src/aioqui/widgets/frame.py
 src/aioqui/widgets/input.py
 src/aioqui/widgets/label.py
 src/aioqui/widgets/layout.py
 src/aioqui/widgets/scroll_area.py
 src/aioqui/widgets/selector.py
 src/aioqui/widgets/slider.py
 src/aioqui/widgets/spacer.py
 src/aioqui/widgets/splitter.py
 src/aioqui/widgets/stacked_widget.py
 src/aioqui/widgets/statusbar.py
 src/aioqui/widgets/widget.py
 src/aioqui/widgets/window.py
 src/aioqui/widgets/custom/__init__.py
-src/aioqui/widgets/custom/date_picker.py
 src/aioqui/widgets/custom/error_label.py
 src/aioqui/widgets/custom/image_button.py
 src/aioqui/widgets/custom/menu_button.py
 src/aioqui/widgets/custom/popup.py
 src/aioqui/widgets/custom/searchbar.py
 src/aioqui/widgets/custom/state_icon_btn.py
 src/aioqui/widgets/extensions/__init__.py
 src/aioqui/widgets/extensions/input_ext.py
 src/aioqui/widgets/extensions/layout_ext.py
 src/aioqui/widgets/extensions/side_menu_ext.py
-src/aioqui/widgets/extensions/splitter_widget_ext.py
+src/aioqui/widgets/extensions/splitter_widget_ext.py
+src/aioqui/widgets/qss/__init__.py
+src/aioqui/widgets/qss/colors.py
+src/aioqui/widgets/qss/date_time.py
+src/aioqui/widgets/qss/image_button.py
+src/aioqui/widgets/qss/popup.py
+src/aioqui/widgets/qss/scrollbar.py
+src/aioqui/widgets/qss/searchbar.py
```

