# Comparing `tmp/QT-PyQt-PySide-Custom-Widgets-0.6.5.tar.gz` & `tmp/QT-PyQt-PySide-Custom-Widgets-0.6.6.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "dist\QT-PyQt-PySide-Custom-Widgets-0.6.5.tar", last modified: Wed Jun 21 21:13:08 2023, max compression
+gzip compressed data, was "dist\QT-PyQt-PySide-Custom-Widgets-0.6.6.tar", last modified: Sat Jun 24 14:28:52 2023, max compression
```

## Comparing `QT-PyQt-PySide-Custom-Widgets-0.6.5.tar` & `QT-PyQt-PySide-Custom-Widgets-0.6.6.tar`

### file list

```diff
@@ -1,389 +1,393 @@
-drwxrwxrwx   0        0        0        0 2023-06-21 21:13:08.168026 QT-PyQt-PySide-Custom-Widgets-0.6.5/
-drwxrwxrwx   0        0        0        0 2023-06-21 21:13:06.819338 QT-PyQt-PySide-Custom-Widgets-0.6.5/Custom_Widgets/
--rw-rw-rw-   0        0        0    66370 2023-06-21 20:45:30.000000 QT-PyQt-PySide-Custom-Widgets-0.6.5/Custom_Widgets/AnalogGaugeWidget.py
-drwxrwxrwx   0        0        0        0 2023-06-21 21:13:06.828332 QT-PyQt-PySide-Custom-Widgets-0.6.5/Custom_Widgets/ProgressIndicator/
--rw-rw-rw-   0        0        0        0 2023-06-21 20:45:30.000000 QT-PyQt-PySide-Custom-Widgets-0.6.5/Custom_Widgets/ProgressIndicator/__init__.py
-drwxrwxrwx   0        0        0        0 2023-06-21 21:13:06.881634 QT-PyQt-PySide-Custom-Widgets-0.6.5/Custom_Widgets/ProgressIndicator/__pycache__/
--rw-rw-rw-   0        0        0      185 2023-06-21 20:45:30.000000 QT-PyQt-PySide-Custom-Widgets-0.6.5/Custom_Widgets/ProgressIndicator/__pycache__/__init__.cpython-310.pyc
--rw-rw-rw-   0        0        0      178 2023-06-21 20:45:31.000000 QT-PyQt-PySide-Custom-Widgets-0.6.5/Custom_Widgets/ProgressIndicator/__pycache__/__init__.cpython-38.pyc
--rw-rw-rw-   0        0        0     3840 2023-06-21 20:45:30.000000 QT-PyQt-PySide-Custom-Widgets-0.6.5/Custom_Widgets/ProgressIndicator/__pycache__/test.cpython-310.pyc
--rw-rw-rw-   0        0        0     3948 2023-06-21 20:45:31.000000 QT-PyQt-PySide-Custom-Widgets-0.6.5/Custom_Widgets/ProgressIndicator/__pycache__/test.cpython-38.pyc
--rw-rw-rw-   0        0        0     5285 2023-06-21 20:45:30.000000 QT-PyQt-PySide-Custom-Widgets-0.6.5/Custom_Widgets/ProgressIndicator/__pycache__/ui_interface.cpython-310.pyc
--rw-rw-rw-   0        0        0     5276 2023-06-21 20:45:31.000000 QT-PyQt-PySide-Custom-Widgets-0.6.5/Custom_Widgets/ProgressIndicator/__pycache__/ui_interface.cpython-38.pyc
--rw-rw-rw-   0        0        0     5297 2023-06-21 20:45:30.000000 QT-PyQt-PySide-Custom-Widgets-0.6.5/Custom_Widgets/ProgressIndicator/__pycache__/ui_interface.cpython-39.pyc
--rw-rw-rw-   0        0        0     8502 2023-06-21 20:45:30.000000 QT-PyQt-PySide-Custom-Widgets-0.6.5/Custom_Widgets/ProgressIndicator/interface.ui
--rw-rw-rw-   0        0        0     9452 2023-06-21 20:45:30.000000 QT-PyQt-PySide-Custom-Widgets-0.6.5/Custom_Widgets/ProgressIndicator/test.py
--rw-rw-rw-   0        0        0     9629 2023-06-21 20:45:30.000000 QT-PyQt-PySide-Custom-Widgets-0.6.5/Custom_Widgets/ProgressIndicator/ui_interface.py
--rw-rw-rw-   0        0        0    14071 2023-06-21 20:45:30.000000 QT-PyQt-PySide-Custom-Widgets-0.6.5/Custom_Widgets/ProjectMaker.py
-drwxrwxrwx   0        0        0        0 2023-06-21 21:13:06.949614 QT-PyQt-PySide-Custom-Widgets-0.6.5/Custom_Widgets/Qss/
--rw-rw-rw-   0        0        0    39288 2023-06-21 20:45:30.000000 QT-PyQt-PySide-Custom-Widgets-0.6.5/Custom_Widgets/Qss/QSS_Resources.qrc
--rw-rw-rw-   0        0        0     5505 2023-06-21 20:45:30.000000 QT-PyQt-PySide-Custom-Widgets-0.6.5/Custom_Widgets/Qss/SassCompiler.py
--rw-rw-rw-   0        0        0    14615 2023-06-21 20:45:30.000000 QT-PyQt-PySide-Custom-Widgets-0.6.5/Custom_Widgets/Qss/SvgToPngIcons.py
--rw-rw-rw-   0        0        0       39 2023-06-21 20:45:30.000000 QT-PyQt-PySide-Custom-Widgets-0.6.5/Custom_Widgets/Qss/__init__.py
-drwxrwxrwx   0        0        0        0 2023-06-21 21:13:07.072648 QT-PyQt-PySide-Custom-Widgets-0.6.5/Custom_Widgets/Qss/__pycache__/
--rw-rw-rw-   0        0        0   630113 2023-06-21 20:45:30.000000 QT-PyQt-PySide-Custom-Widgets-0.6.5/Custom_Widgets/Qss/__pycache__/QSS_Resources.cpython-39.pyc
--rw-rw-rw-   0        0        0     3122 2023-06-21 20:45:30.000000 QT-PyQt-PySide-Custom-Widgets-0.6.5/Custom_Widgets/Qss/__pycache__/SassCompiler.cpython-310.pyc
--rw-rw-rw-   0        0        0     3089 2023-06-21 20:45:31.000000 QT-PyQt-PySide-Custom-Widgets-0.6.5/Custom_Widgets/Qss/__pycache__/SassCompiler.cpython-38.pyc
--rw-rw-rw-   0        0        0     6895 2023-06-21 20:45:30.000000 QT-PyQt-PySide-Custom-Widgets-0.6.5/Custom_Widgets/Qss/__pycache__/SvgToPngIcons.cpython-310.pyc
--rw-rw-rw-   0        0        0     6680 2023-06-21 20:45:31.000000 QT-PyQt-PySide-Custom-Widgets-0.6.5/Custom_Widgets/Qss/__pycache__/SvgToPngIcons.cpython-38.pyc
--rw-rw-rw-   0        0        0     3158 2023-06-21 20:45:30.000000 QT-PyQt-PySide-Custom-Widgets-0.6.5/Custom_Widgets/Qss/__pycache__/SvgToPngIcons.cpython-39.pyc
--rw-rw-rw-   0        0        0      192 2023-06-21 20:45:30.000000 QT-PyQt-PySide-Custom-Widgets-0.6.5/Custom_Widgets/Qss/__pycache__/__init__.cpython-310.pyc
--rw-rw-rw-   0        0        0      177 2023-06-21 20:45:30.000000 QT-PyQt-PySide-Custom-Widgets-0.6.5/Custom_Widgets/Qss/__pycache__/__init__.cpython-37.pyc
--rw-rw-rw-   0        0        0      185 2023-06-21 20:45:31.000000 QT-PyQt-PySide-Custom-Widgets-0.6.5/Custom_Widgets/Qss/__pycache__/__init__.cpython-38.pyc
--rw-rw-rw-   0        0        0      188 2023-06-21 20:45:30.000000 QT-PyQt-PySide-Custom-Widgets-0.6.5/Custom_Widgets/Qss/__pycache__/__init__.cpython-39.pyc
--rw-rw-rw-   0        0        0     6166 2023-06-21 20:45:30.000000 QT-PyQt-PySide-Custom-Widgets-0.6.5/Custom_Widgets/Qss/__pycache__/colorsystem.cpython-310.pyc
--rw-rw-rw-   0        0        0     6168 2023-06-21 20:45:30.000000 QT-PyQt-PySide-Custom-Widgets-0.6.5/Custom_Widgets/Qss/__pycache__/colorsystem.cpython-37.pyc
--rw-rw-rw-   0        0        0     6481 2023-06-21 21:05:22.000000 QT-PyQt-PySide-Custom-Widgets-0.6.5/Custom_Widgets/Qss/__pycache__/colorsystem.cpython-38.pyc
--rw-rw-rw-   0        0        0     6064 2023-06-21 20:45:30.000000 QT-PyQt-PySide-Custom-Widgets-0.6.5/Custom_Widgets/Qss/__pycache__/colorsystem.cpython-39.pyc
--rw-rw-rw-   0        0        0   630112 2023-06-21 20:45:30.000000 QT-PyQt-PySide-Custom-Widgets-0.6.5/Custom_Widgets/Qss/__pycache__/resources_rc.cpython-39.pyc
--rw-rw-rw-   0        0        0     2764 2023-06-21 20:45:30.000000 QT-PyQt-PySide-Custom-Widgets-0.6.5/Custom_Widgets/Qss/__pycache__/sassCompiler.cpython-39.pyc
--rw-rw-rw-   0        0        0    60079 2023-06-21 20:45:30.000000 QT-PyQt-PySide-Custom-Widgets-0.6.5/Custom_Widgets/Qss/_styles.scss
--rw-rw-rw-   0        0        0    10048 2023-06-21 21:05:04.000000 QT-PyQt-PySide-Custom-Widgets-0.6.5/Custom_Widgets/Qss/colorsystem.py
-drwxrwxrwx   0        0        0        0 2023-06-21 21:13:06.736609 QT-PyQt-PySide-Custom-Widgets-0.6.5/Custom_Widgets/Qss/icons/
-drwxrwxrwx   0        0        0        0 2023-06-21 21:13:07.997122 QT-PyQt-PySide-Custom-Widgets-0.6.5/Custom_Widgets/Qss/icons/original_svg/
--rw-rw-rw-   0        0        0      276 2023-06-21 20:45:30.000000 QT-PyQt-PySide-Custom-Widgets-0.6.5/Custom_Widgets/Qss/icons/original_svg/activity.svg
--rw-rw-rw-   0        0        0      356 2023-06-21 20:45:30.000000 QT-PyQt-PySide-Custom-Widgets-0.6.5/Custom_Widgets/Qss/icons/original_svg/airplay.svg
--rw-rw-rw-   0        0        0      350 2023-06-21 20:45:30.000000 QT-PyQt-PySide-Custom-Widgets-0.6.5/Custom_Widgets/Qss/icons/original_svg/alert-circle.svg
--rw-rw-rw-   0        0        0      410 2023-06-21 20:45:30.000000 QT-PyQt-PySide-Custom-Widgets-0.6.5/Custom_Widgets/Qss/icons/original_svg/alert-octagon.svg
--rw-rw-rw-   0        0        0      418 2023-06-21 20:45:30.000000 QT-PyQt-PySide-Custom-Widgets-0.6.5/Custom_Widgets/Qss/icons/original_svg/alert-triangle.svg
--rw-rw-rw-   0        0        0      392 2023-06-21 20:45:30.000000 QT-PyQt-PySide-Custom-Widgets-0.6.5/Custom_Widgets/Qss/icons/original_svg/align-center.svg
--rw-rw-rw-   0        0        0      393 2023-06-21 20:45:30.000000 QT-PyQt-PySide-Custom-Widgets-0.6.5/Custom_Widgets/Qss/icons/original_svg/align-justify.svg
--rw-rw-rw-   0        0        0      390 2023-06-21 20:45:30.000000 QT-PyQt-PySide-Custom-Widgets-0.6.5/Custom_Widgets/Qss/icons/original_svg/align-left.svg
--rw-rw-rw-   0        0        0      391 2023-06-21 20:45:30.000000 QT-PyQt-PySide-Custom-Widgets-0.6.5/Custom_Widgets/Qss/icons/original_svg/align-right.svg
--rw-rw-rw-   0        0        0      339 2023-06-21 20:45:30.000000 QT-PyQt-PySide-Custom-Widgets-0.6.5/Custom_Widgets/Qss/icons/original_svg/anchor.svg
--rw-rw-rw-   0        0        0      562 2023-06-21 20:45:30.000000 QT-PyQt-PySide-Custom-Widgets-0.6.5/Custom_Widgets/Qss/icons/original_svg/aperture.svg
--rw-rw-rw-   0        0        0      355 2023-06-21 20:45:30.000000 QT-PyQt-PySide-Custom-Widgets-0.6.5/Custom_Widgets/Qss/icons/original_svg/archive.svg
--rw-rw-rw-   0        0        0      354 2023-06-21 20:45:30.000000 QT-PyQt-PySide-Custom-Widgets-0.6.5/Custom_Widgets/Qss/icons/original_svg/arrow-down-circle.svg
--rw-rw-rw-   0        0        0      309 2023-06-21 20:45:30.000000 QT-PyQt-PySide-Custom-Widgets-0.6.5/Custom_Widgets/Qss/icons/original_svg/arrow-down-left.svg
--rw-rw-rw-   0        0        0      311 2023-06-21 20:45:30.000000 QT-PyQt-PySide-Custom-Widgets-0.6.5/Custom_Widgets/Qss/icons/original_svg/arrow-down-right.svg
--rw-rw-rw-   0        0        0      307 2023-06-21 20:45:30.000000 QT-PyQt-PySide-Custom-Widgets-0.6.5/Custom_Widgets/Qss/icons/original_svg/arrow-down.svg
--rw-rw-rw-   0        0        0      353 2023-06-21 20:45:30.000000 QT-PyQt-PySide-Custom-Widgets-0.6.5/Custom_Widgets/Qss/icons/original_svg/arrow-left-circle.svg
--rw-rw-rw-   0        0        0      306 2023-06-21 20:45:30.000000 QT-PyQt-PySide-Custom-Widgets-0.6.5/Custom_Widgets/Qss/icons/original_svg/arrow-left.svg
--rw-rw-rw-   0        0        0      355 2023-06-21 20:45:30.000000 QT-PyQt-PySide-Custom-Widgets-0.6.5/Custom_Widgets/Qss/icons/original_svg/arrow-right-circle.svg
--rw-rw-rw-   0        0        0      308 2023-06-21 20:45:30.000000 QT-PyQt-PySide-Custom-Widgets-0.6.5/Custom_Widgets/Qss/icons/original_svg/arrow-right.svg
--rw-rw-rw-   0        0        0      351 2023-06-21 20:45:30.000000 QT-PyQt-PySide-Custom-Widgets-0.6.5/Custom_Widgets/Qss/icons/original_svg/arrow-up-circle.svg
--rw-rw-rw-   0        0        0      306 2023-06-21 20:45:30.000000 QT-PyQt-PySide-Custom-Widgets-0.6.5/Custom_Widgets/Qss/icons/original_svg/arrow-up-left.svg
--rw-rw-rw-   0        0        0      308 2023-06-21 20:45:30.000000 QT-PyQt-PySide-Custom-Widgets-0.6.5/Custom_Widgets/Qss/icons/original_svg/arrow-up-right.svg
--rw-rw-rw-   0        0        0      304 2023-06-21 20:45:30.000000 QT-PyQt-PySide-Custom-Widgets-0.6.5/Custom_Widgets/Qss/icons/original_svg/arrow-up.svg
--rw-rw-rw-   0        0        0     3022 2023-06-21 20:45:30.000000 QT-PyQt-PySide-Custom-Widgets-0.6.5/Custom_Widgets/Qss/icons/original_svg/arrow_down.svg
--rw-rw-rw-   0        0        0     3023 2023-06-21 20:45:30.000000 QT-PyQt-PySide-Custom-Widgets-0.6.5/Custom_Widgets/Qss/icons/original_svg/arrow_left.svg
--rw-rw-rw-   0        0        0     3026 2023-06-21 20:45:30.000000 QT-PyQt-PySide-Custom-Widgets-0.6.5/Custom_Widgets/Qss/icons/original_svg/arrow_right.svg
--rw-rw-rw-   0        0        0     3021 2023-06-21 20:45:30.000000 QT-PyQt-PySide-Custom-Widgets-0.6.5/Custom_Widgets/Qss/icons/original_svg/arrow_up.svg
--rw-rw-rw-   0        0        0      316 2023-06-21 20:45:30.000000 QT-PyQt-PySide-Custom-Widgets-0.6.5/Custom_Widgets/Qss/icons/original_svg/at-sign.svg
--rw-rw-rw-   0        0        0      319 2023-06-21 20:45:30.000000 QT-PyQt-PySide-Custom-Widgets-0.6.5/Custom_Widgets/Qss/icons/original_svg/award.svg
--rw-rw-rw-   0        0        0      349 2023-06-21 20:45:30.000000 QT-PyQt-PySide-Custom-Widgets-0.6.5/Custom_Widgets/Qss/icons/original_svg/bar-chart-2.svg
--rw-rw-rw-   0        0        0      347 2023-06-21 20:45:30.000000 QT-PyQt-PySide-Custom-Widgets-0.6.5/Custom_Widgets/Qss/icons/original_svg/bar-chart.svg
--rw-rw-rw-   0        0        0     7594 2023-06-21 20:45:30.000000 QT-PyQt-PySide-Custom-Widgets-0.6.5/Custom_Widgets/Qss/icons/original_svg/base_icon.svg
--rw-rw-rw-   0        0        0    33666 2023-06-21 20:45:30.000000 QT-PyQt-PySide-Custom-Widgets-0.6.5/Custom_Widgets/Qss/icons/original_svg/base_palette.svg
--rw-rw-rw-   0        0        0      421 2023-06-21 20:45:30.000000 QT-PyQt-PySide-Custom-Widgets-0.6.5/Custom_Widgets/Qss/icons/original_svg/battery-charging.svg
--rw-rw-rw-   0        0        0      320 2023-06-21 20:45:30.000000 QT-PyQt-PySide-Custom-Widgets-0.6.5/Custom_Widgets/Qss/icons/original_svg/battery.svg
--rw-rw-rw-   0        0        0      454 2023-06-21 20:45:30.000000 QT-PyQt-PySide-Custom-Widgets-0.6.5/Custom_Widgets/Qss/icons/original_svg/bell-off.svg
--rw-rw-rw-   0        0        0      315 2023-06-21 20:45:30.000000 QT-PyQt-PySide-Custom-Widgets-0.6.5/Custom_Widgets/Qss/icons/original_svg/bell.svg
--rw-rw-rw-   0        0        0      292 2023-06-21 20:45:30.000000 QT-PyQt-PySide-Custom-Widgets-0.6.5/Custom_Widgets/Qss/icons/original_svg/bluetooth.svg
--rw-rw-rw-   0        0        0      321 2023-06-21 20:45:30.000000 QT-PyQt-PySide-Custom-Widgets-0.6.5/Custom_Widgets/Qss/icons/original_svg/bold.svg
--rw-rw-rw-   0        0        0      333 2023-06-21 20:45:30.000000 QT-PyQt-PySide-Custom-Widgets-0.6.5/Custom_Widgets/Qss/icons/original_svg/book-open.svg
--rw-rw-rw-   0        0        0      339 2023-06-21 20:45:30.000000 QT-PyQt-PySide-Custom-Widgets-0.6.5/Custom_Widgets/Qss/icons/original_svg/book.svg
--rw-rw-rw-   0        0        0      281 2023-06-21 20:45:30.000000 QT-PyQt-PySide-Custom-Widgets-0.6.5/Custom_Widgets/Qss/icons/original_svg/bookmark.svg
--rw-rw-rw-   0        0        0      456 2023-06-21 20:45:30.000000 QT-PyQt-PySide-Custom-Widgets-0.6.5/Custom_Widgets/Qss/icons/original_svg/box.svg
--rw-rw-rw-   0        0        0     2755 2023-06-21 20:45:30.000000 QT-PyQt-PySide-Custom-Widgets-0.6.5/Custom_Widgets/Qss/icons/original_svg/branch_closed.svg
--rw-rw-rw-   0        0        0     2902 2023-06-21 20:45:30.000000 QT-PyQt-PySide-Custom-Widgets-0.6.5/Custom_Widgets/Qss/icons/original_svg/branch_end.svg
--rw-rw-rw-   0        0        0     3508 2023-06-21 20:45:30.000000 QT-PyQt-PySide-Custom-Widgets-0.6.5/Custom_Widgets/Qss/icons/original_svg/branch_line.svg
--rw-rw-rw-   0        0        0     2678 2023-06-21 20:45:30.000000 QT-PyQt-PySide-Custom-Widgets-0.6.5/Custom_Widgets/Qss/icons/original_svg/branch_more.svg
--rw-rw-rw-   0        0        0     2711 2023-06-21 20:45:30.000000 QT-PyQt-PySide-Custom-Widgets-0.6.5/Custom_Widgets/Qss/icons/original_svg/branch_open.svg
--rw-rw-rw-   0        0        0      337 2023-06-21 20:45:30.000000 QT-PyQt-PySide-Custom-Widgets-0.6.5/Custom_Widgets/Qss/icons/original_svg/briefcase.svg
--rw-rw-rw-   0        0        0      404 2023-06-21 20:45:30.000000 QT-PyQt-PySide-Custom-Widgets-0.6.5/Custom_Widgets/Qss/icons/original_svg/calendar.svg
--rw-rw-rw-   0        0        0      379 2023-06-21 20:45:30.000000 QT-PyQt-PySide-Custom-Widgets-0.6.5/Custom_Widgets/Qss/icons/original_svg/camera-off.svg
--rw-rw-rw-   0        0        0      350 2023-06-21 20:45:30.000000 QT-PyQt-PySide-Custom-Widgets-0.6.5/Custom_Widgets/Qss/icons/original_svg/camera.svg
--rw-rw-rw-   0        0        0      381 2023-06-21 20:45:30.000000 QT-PyQt-PySide-Custom-Widgets-0.6.5/Custom_Widgets/Qss/icons/original_svg/cast.svg
--rw-rw-rw-   0        0        0      322 2023-06-21 20:45:30.000000 QT-PyQt-PySide-Custom-Widgets-0.6.5/Custom_Widgets/Qss/icons/original_svg/check-circle.svg
--rw-rw-rw-   0        0        0      339 2023-06-21 20:45:30.000000 QT-PyQt-PySide-Custom-Widgets-0.6.5/Custom_Widgets/Qss/icons/original_svg/check-square.svg
--rw-rw-rw-   0        0        0      256 2023-06-21 20:45:30.000000 QT-PyQt-PySide-Custom-Widgets-0.6.5/Custom_Widgets/Qss/icons/original_svg/check.svg
--rw-rw-rw-   0        0        0     2799 2023-06-21 20:45:30.000000 QT-PyQt-PySide-Custom-Widgets-0.6.5/Custom_Widgets/Qss/icons/original_svg/checkbox_checked.svg
--rw-rw-rw-   0        0        0     2781 2023-06-21 20:45:30.000000 QT-PyQt-PySide-Custom-Widgets-0.6.5/Custom_Widgets/Qss/icons/original_svg/checkbox_indeterminate.svg
--rw-rw-rw-   0        0        0     2598 2023-06-21 20:45:30.000000 QT-PyQt-PySide-Custom-Widgets-0.6.5/Custom_Widgets/Qss/icons/original_svg/checkbox_unchecked.svg
--rw-rw-rw-   0        0        0      263 2023-06-21 20:45:30.000000 QT-PyQt-PySide-Custom-Widgets-0.6.5/Custom_Widgets/Qss/icons/original_svg/chevron-down.svg
--rw-rw-rw-   0        0        0      264 2023-06-21 20:45:30.000000 QT-PyQt-PySide-Custom-Widgets-0.6.5/Custom_Widgets/Qss/icons/original_svg/chevron-left.svg
--rw-rw-rw-   0        0        0      264 2023-06-21 20:45:30.000000 QT-PyQt-PySide-Custom-Widgets-0.6.5/Custom_Widgets/Qss/icons/original_svg/chevron-right.svg
--rw-rw-rw-   0        0        0      262 2023-06-21 20:45:30.000000 QT-PyQt-PySide-Custom-Widgets-0.6.5/Custom_Widgets/Qss/icons/original_svg/chevron-up.svg
--rw-rw-rw-   0        0        0      311 2023-06-21 20:45:30.000000 QT-PyQt-PySide-Custom-Widgets-0.6.5/Custom_Widgets/Qss/icons/original_svg/chevrons-down.svg
--rw-rw-rw-   0        0        0      312 2023-06-21 20:45:30.000000 QT-PyQt-PySide-Custom-Widgets-0.6.5/Custom_Widgets/Qss/icons/original_svg/chevrons-left.svg
--rw-rw-rw-   0        0        0      312 2023-06-21 20:45:30.000000 QT-PyQt-PySide-Custom-Widgets-0.6.5/Custom_Widgets/Qss/icons/original_svg/chevrons-right.svg
--rw-rw-rw-   0        0        0      310 2023-06-21 20:45:30.000000 QT-PyQt-PySide-Custom-Widgets-0.6.5/Custom_Widgets/Qss/icons/original_svg/chevrons-up.svg
--rw-rw-rw-   0        0        0      442 2023-06-21 20:45:30.000000 QT-PyQt-PySide-Custom-Widgets-0.6.5/Custom_Widgets/Qss/icons/original_svg/chrome.svg
--rw-rw-rw-   0        0        0      252 2023-06-21 20:45:30.000000 QT-PyQt-PySide-Custom-Widgets-0.6.5/Custom_Widgets/Qss/icons/original_svg/circle.svg
--rw-rw-rw-   0        0        0      365 2023-06-21 20:45:30.000000 QT-PyQt-PySide-Custom-Widgets-0.6.5/Custom_Widgets/Qss/icons/original_svg/clipboard.svg
--rw-rw-rw-   0        0        0      298 2023-06-21 20:45:30.000000 QT-PyQt-PySide-Custom-Widgets-0.6.5/Custom_Widgets/Qss/icons/original_svg/clock.svg
--rw-rw-rw-   0        0        0      551 2023-06-21 20:45:30.000000 QT-PyQt-PySide-Custom-Widgets-0.6.5/Custom_Widgets/Qss/icons/original_svg/cloud-drizzle.svg
--rw-rw-rw-   0        0        0      339 2023-06-21 20:45:30.000000 QT-PyQt-PySide-Custom-Widgets-0.6.5/Custom_Widgets/Qss/icons/original_svg/cloud-lightning.svg
--rw-rw-rw-   0        0        0      365 2023-06-21 20:45:30.000000 QT-PyQt-PySide-Custom-Widgets-0.6.5/Custom_Widgets/Qss/icons/original_svg/cloud-off.svg
--rw-rw-rw-   0        0        0      415 2023-06-21 20:45:30.000000 QT-PyQt-PySide-Custom-Widgets-0.6.5/Custom_Widgets/Qss/icons/original_svg/cloud-rain.svg
--rw-rw-rw-   0        0        0      566 2023-06-21 20:45:30.000000 QT-PyQt-PySide-Custom-Widgets-0.6.5/Custom_Widgets/Qss/icons/original_svg/cloud-snow.svg
--rw-rw-rw-   0        0        0      274 2023-06-21 20:45:30.000000 QT-PyQt-PySide-Custom-Widgets-0.6.5/Custom_Widgets/Qss/icons/original_svg/cloud.svg
--rw-rw-rw-   0        0        0      301 2023-06-21 20:45:30.000000 QT-PyQt-PySide-Custom-Widgets-0.6.5/Custom_Widgets/Qss/icons/original_svg/code.svg
--rw-rw-rw-   0        0        0      480 2023-06-21 20:45:30.000000 QT-PyQt-PySide-Custom-Widgets-0.6.5/Custom_Widgets/Qss/icons/original_svg/codepen.svg
--rw-rw-rw-   0        0        0      632 2023-06-21 20:45:30.000000 QT-PyQt-PySide-Custom-Widgets-0.6.5/Custom_Widgets/Qss/icons/original_svg/codesandbox.svg
--rw-rw-rw-   0        0        0      441 2023-06-21 20:45:30.000000 QT-PyQt-PySide-Custom-Widgets-0.6.5/Custom_Widgets/Qss/icons/original_svg/coffee.svg
--rw-rw-rw-   0        0        0      320 2023-06-21 20:45:30.000000 QT-PyQt-PySide-Custom-Widgets-0.6.5/Custom_Widgets/Qss/icons/original_svg/columns.svg
--rw-rw-rw-   0        0        0      415 2023-06-21 20:45:30.000000 QT-PyQt-PySide-Custom-Widgets-0.6.5/Custom_Widgets/Qss/icons/original_svg/command.svg
--rw-rw-rw-   0        0        0      336 2023-06-21 20:45:30.000000 QT-PyQt-PySide-Custom-Widgets-0.6.5/Custom_Widgets/Qss/icons/original_svg/compass.svg
--rw-rw-rw-   0        0        0      345 2023-06-21 20:45:30.000000 QT-PyQt-PySide-Custom-Widgets-0.6.5/Custom_Widgets/Qss/icons/original_svg/copy.svg
--rw-rw-rw-   0        0        0      308 2023-06-21 20:45:30.000000 QT-PyQt-PySide-Custom-Widgets-0.6.5/Custom_Widgets/Qss/icons/original_svg/corner-down-left.svg
--rw-rw-rw-   0        0        0      312 2023-06-21 20:45:30.000000 QT-PyQt-PySide-Custom-Widgets-0.6.5/Custom_Widgets/Qss/icons/original_svg/corner-down-right.svg
--rw-rw-rw-   0        0        0      311 2023-06-21 20:45:30.000000 QT-PyQt-PySide-Custom-Widgets-0.6.5/Custom_Widgets/Qss/icons/original_svg/corner-left-down.svg
--rw-rw-rw-   0        0        0      306 2023-06-21 20:45:30.000000 QT-PyQt-PySide-Custom-Widgets-0.6.5/Custom_Widgets/Qss/icons/original_svg/corner-left-up.svg
--rw-rw-rw-   0        0        0      312 2023-06-21 20:45:30.000000 QT-PyQt-PySide-Custom-Widgets-0.6.5/Custom_Widgets/Qss/icons/original_svg/corner-right-down.svg
--rw-rw-rw-   0        0        0      307 2023-06-21 20:45:30.000000 QT-PyQt-PySide-Custom-Widgets-0.6.5/Custom_Widgets/Qss/icons/original_svg/corner-right-up.svg
--rw-rw-rw-   0        0        0      306 2023-06-21 20:45:30.000000 QT-PyQt-PySide-Custom-Widgets-0.6.5/Custom_Widgets/Qss/icons/original_svg/corner-up-left.svg
--rw-rw-rw-   0        0        0      310 2023-06-21 20:45:30.000000 QT-PyQt-PySide-Custom-Widgets-0.6.5/Custom_Widgets/Qss/icons/original_svg/corner-up-right.svg
--rw-rw-rw-   0        0        0      661 2023-06-21 20:45:30.000000 QT-PyQt-PySide-Custom-Widgets-0.6.5/Custom_Widgets/Qss/icons/original_svg/cpu.svg
--rw-rw-rw-   0        0        0      323 2023-06-21 20:45:30.000000 QT-PyQt-PySide-Custom-Widgets-0.6.5/Custom_Widgets/Qss/icons/original_svg/credit-card.svg
--rw-rw-rw-   0        0        0      304 2023-06-21 20:45:30.000000 QT-PyQt-PySide-Custom-Widgets-0.6.5/Custom_Widgets/Qss/icons/original_svg/crop.svg
--rw-rw-rw-   0        0        0      431 2023-06-21 20:45:30.000000 QT-PyQt-PySide-Custom-Widgets-0.6.5/Custom_Widgets/Qss/icons/original_svg/crosshair.svg
--rw-rw-rw-   0        0        0      366 2023-06-21 20:45:30.000000 QT-PyQt-PySide-Custom-Widgets-0.6.5/Custom_Widgets/Qss/icons/original_svg/database.svg
--rw-rw-rw-   0        0        0      368 2023-06-21 20:45:30.000000 QT-PyQt-PySide-Custom-Widgets-0.6.5/Custom_Widgets/Qss/icons/original_svg/delete.svg
--rw-rw-rw-   0        0        0      289 2023-06-21 20:45:30.000000 QT-PyQt-PySide-Custom-Widgets-0.6.5/Custom_Widgets/Qss/icons/original_svg/disc.svg
--rw-rw-rw-   0        0        0      391 2023-06-21 20:45:30.000000 QT-PyQt-PySide-Custom-Widgets-0.6.5/Custom_Widgets/Qss/icons/original_svg/divide-circle.svg
--rw-rw-rw-   0        0        0      413 2023-06-21 20:45:30.000000 QT-PyQt-PySide-Custom-Widgets-0.6.5/Custom_Widgets/Qss/icons/original_svg/divide-square.svg
--rw-rw-rw-   0        0        0      333 2023-06-21 20:45:30.000000 QT-PyQt-PySide-Custom-Widgets-0.6.5/Custom_Widgets/Qss/icons/original_svg/divide.svg
--rw-rw-rw-   0        0        0      328 2023-06-21 20:45:30.000000 QT-PyQt-PySide-Custom-Widgets-0.6.5/Custom_Widgets/Qss/icons/original_svg/dollar-sign.svg
--rw-rw-rw-   0        0        0      381 2023-06-21 20:45:30.000000 QT-PyQt-PySide-Custom-Widgets-0.6.5/Custom_Widgets/Qss/icons/original_svg/download-cloud.svg
--rw-rw-rw-   0        0        0      364 2023-06-21 20:45:30.000000 QT-PyQt-PySide-Custom-Widgets-0.6.5/Custom_Widgets/Qss/icons/original_svg/download.svg
--rw-rw-rw-   0        0        0      418 2023-06-21 20:45:30.000000 QT-PyQt-PySide-Custom-Widgets-0.6.5/Custom_Widgets/Qss/icons/original_svg/dribbble.svg
--rw-rw-rw-   0        0        0      268 2023-06-21 20:45:30.000000 QT-PyQt-PySide-Custom-Widgets-0.6.5/Custom_Widgets/Qss/icons/original_svg/droplet.svg
--rw-rw-rw-   0        0        0      285 2023-06-21 20:45:30.000000 QT-PyQt-PySide-Custom-Widgets-0.6.5/Custom_Widgets/Qss/icons/original_svg/edit-2.svg
--rw-rw-rw-   0        0        0      311 2023-06-21 20:45:30.000000 QT-PyQt-PySide-Custom-Widgets-0.6.5/Custom_Widgets/Qss/icons/original_svg/edit-3.svg
--rw-rw-rw-   0        0        0      359 2023-06-21 20:45:30.000000 QT-PyQt-PySide-Custom-Widgets-0.6.5/Custom_Widgets/Qss/icons/original_svg/edit.svg
--rw-rw-rw-   0        0        0      382 2023-06-21 20:45:30.000000 QT-PyQt-PySide-Custom-Widgets-0.6.5/Custom_Widgets/Qss/icons/original_svg/external-link.svg
--rw-rw-rw-   0        0        0      454 2023-06-21 20:45:30.000000 QT-PyQt-PySide-Custom-Widgets-0.6.5/Custom_Widgets/Qss/icons/original_svg/eye-off.svg
--rw-rw-rw-   0        0        0      310 2023-06-21 20:45:30.000000 QT-PyQt-PySide-Custom-Widgets-0.6.5/Custom_Widgets/Qss/icons/original_svg/eye.svg
--rw-rw-rw-   0        0        0      297 2023-06-21 20:45:30.000000 QT-PyQt-PySide-Custom-Widgets-0.6.5/Custom_Widgets/Qss/icons/original_svg/facebook.svg
--rw-rw-rw-   0        0        0      317 2023-06-21 20:45:30.000000 QT-PyQt-PySide-Custom-Widgets-0.6.5/Custom_Widgets/Qss/icons/original_svg/fast-forward.svg
--rw-rw-rw-   0        0        0      367 2023-06-21 20:45:30.000000 QT-PyQt-PySide-Custom-Widgets-0.6.5/Custom_Widgets/Qss/icons/original_svg/feather.svg
--rw-rw-rw-   0        0        0      547 2023-06-21 20:45:30.000000 QT-PyQt-PySide-Custom-Widgets-0.6.5/Custom_Widgets/Qss/icons/original_svg/figma.svg
--rw-rw-rw-   0        0        0      381 2023-06-21 20:45:30.000000 QT-PyQt-PySide-Custom-Widgets-0.6.5/Custom_Widgets/Qss/icons/original_svg/file-minus.svg
--rw-rw-rw-   0        0        0      425 2023-06-21 20:45:30.000000 QT-PyQt-PySide-Custom-Widgets-0.6.5/Custom_Widgets/Qss/icons/original_svg/file-plus.svg
--rw-rw-rw-   0        0        0      467 2023-06-21 20:45:30.000000 QT-PyQt-PySide-Custom-Widgets-0.6.5/Custom_Widgets/Qss/icons/original_svg/file-text.svg
--rw-rw-rw-   0        0        0      331 2023-06-21 20:45:30.000000 QT-PyQt-PySide-Custom-Widgets-0.6.5/Custom_Widgets/Qss/icons/original_svg/file.svg
--rw-rw-rw-   0        0        0      580 2023-06-21 20:45:30.000000 QT-PyQt-PySide-Custom-Widgets-0.6.5/Custom_Widgets/Qss/icons/original_svg/film.svg
--rw-rw-rw-   0        0        0      284 2023-06-21 20:45:30.000000 QT-PyQt-PySide-Custom-Widgets-0.6.5/Custom_Widgets/Qss/icons/original_svg/filter.svg
--rw-rw-rw-   0        0        0      328 2023-06-21 20:45:30.000000 QT-PyQt-PySide-Custom-Widgets-0.6.5/Custom_Widgets/Qss/icons/original_svg/flag.svg
--rw-rw-rw-   0        0        0      355 2023-06-21 20:45:30.000000 QT-PyQt-PySide-Custom-Widgets-0.6.5/Custom_Widgets/Qss/icons/original_svg/folder-minus.svg
--rw-rw-rw-   0        0        0      399 2023-06-21 20:45:30.000000 QT-PyQt-PySide-Custom-Widgets-0.6.5/Custom_Widgets/Qss/icons/original_svg/folder-plus.svg
--rw-rw-rw-   0        0        0      305 2023-06-21 20:45:30.000000 QT-PyQt-PySide-Custom-Widgets-0.6.5/Custom_Widgets/Qss/icons/original_svg/folder.svg
--rw-rw-rw-   0        0        0      272 2023-06-21 20:45:30.000000 QT-PyQt-PySide-Custom-Widgets-0.6.5/Custom_Widgets/Qss/icons/original_svg/framer.svg
--rw-rw-rw-   0        0        0      384 2023-06-21 20:45:30.000000 QT-PyQt-PySide-Custom-Widgets-0.6.5/Custom_Widgets/Qss/icons/original_svg/frown.svg
--rw-rw-rw-   0        0        0      475 2023-06-21 20:45:30.000000 QT-PyQt-PySide-Custom-Widgets-0.6.5/Custom_Widgets/Qss/icons/original_svg/gift.svg
--rw-rw-rw-   0        0        0      371 2023-06-21 20:45:30.000000 QT-PyQt-PySide-Custom-Widgets-0.6.5/Custom_Widgets/Qss/icons/original_svg/git-branch.svg
--rw-rw-rw-   0        0        0      352 2023-06-21 20:45:30.000000 QT-PyQt-PySide-Custom-Widgets-0.6.5/Custom_Widgets/Qss/icons/original_svg/git-commit.svg
--rw-rw-rw-   0        0        0      330 2023-06-21 20:45:30.000000 QT-PyQt-PySide-Custom-Widgets-0.6.5/Custom_Widgets/Qss/icons/original_svg/git-merge.svg
--rw-rw-rw-   0        0        0      381 2023-06-21 20:45:30.000000 QT-PyQt-PySide-Custom-Widgets-0.6.5/Custom_Widgets/Qss/icons/original_svg/git-pull-request.svg
--rw-rw-rw-   0        0        0      521 2023-06-21 20:45:30.000000 QT-PyQt-PySide-Custom-Widgets-0.6.5/Custom_Widgets/Qss/icons/original_svg/github.svg
--rw-rw-rw-   0        0        0      484 2023-06-21 20:45:30.000000 QT-PyQt-PySide-Custom-Widgets-0.6.5/Custom_Widgets/Qss/icons/original_svg/gitlab.svg
--rw-rw-rw-   0        0        0      403 2023-06-21 20:45:30.000000 QT-PyQt-PySide-Custom-Widgets-0.6.5/Custom_Widgets/Qss/icons/original_svg/globe.svg
--rw-rw-rw-   0        0        0      398 2023-06-21 20:45:30.000000 QT-PyQt-PySide-Custom-Widgets-0.6.5/Custom_Widgets/Qss/icons/original_svg/grid.svg
--rw-rw-rw-   0        0        0      478 2023-06-21 20:45:30.000000 QT-PyQt-PySide-Custom-Widgets-0.6.5/Custom_Widgets/Qss/icons/original_svg/hard-drive.svg
--rw-rw-rw-   0        0        0      383 2023-06-21 20:45:30.000000 QT-PyQt-PySide-Custom-Widgets-0.6.5/Custom_Widgets/Qss/icons/original_svg/hash.svg
--rw-rw-rw-   0        0        0      389 2023-06-21 20:45:30.000000 QT-PyQt-PySide-Custom-Widgets-0.6.5/Custom_Widgets/Qss/icons/original_svg/headphones.svg
--rw-rw-rw-   0        0        0      365 2023-06-21 20:45:30.000000 QT-PyQt-PySide-Custom-Widgets-0.6.5/Custom_Widgets/Qss/icons/original_svg/heart.svg
--rw-rw-rw-   0        0        0      359 2023-06-21 20:45:30.000000 QT-PyQt-PySide-Custom-Widgets-0.6.5/Custom_Widgets/Qss/icons/original_svg/help-circle.svg
--rw-rw-rw-   0        0        0      352 2023-06-21 20:45:30.000000 QT-PyQt-PySide-Custom-Widgets-0.6.5/Custom_Widgets/Qss/icons/original_svg/hexagon.svg
--rw-rw-rw-   0        0        0      326 2023-06-21 20:45:30.000000 QT-PyQt-PySide-Custom-Widgets-0.6.5/Custom_Widgets/Qss/icons/original_svg/home.svg
--rw-rw-rw-   0        0        0      363 2023-06-21 20:45:30.000000 QT-PyQt-PySide-Custom-Widgets-0.6.5/Custom_Widgets/Qss/icons/original_svg/image.svg
--rw-rw-rw-   0        0        0      399 2023-06-21 20:45:30.000000 QT-PyQt-PySide-Custom-Widgets-0.6.5/Custom_Widgets/Qss/icons/original_svg/inbox.svg
--rw-rw-rw-   0        0        0      341 2023-06-21 20:45:30.000000 QT-PyQt-PySide-Custom-Widgets-0.6.5/Custom_Widgets/Qss/icons/original_svg/info.svg
--rw-rw-rw-   0        0        0      394 2023-06-21 20:45:30.000000 QT-PyQt-PySide-Custom-Widgets-0.6.5/Custom_Widgets/Qss/icons/original_svg/instagram.svg
--rw-rw-rw-   0        0        0      342 2023-06-21 20:45:30.000000 QT-PyQt-PySide-Custom-Widgets-0.6.5/Custom_Widgets/Qss/icons/original_svg/italic.svg
--rw-rw-rw-   0        0        0      346 2023-06-21 20:45:30.000000 QT-PyQt-PySide-Custom-Widgets-0.6.5/Custom_Widgets/Qss/icons/original_svg/key.svg
--rw-rw-rw-   0        0        0      359 2023-06-21 20:45:30.000000 QT-PyQt-PySide-Custom-Widgets-0.6.5/Custom_Widgets/Qss/icons/original_svg/layers.svg
--rw-rw-rw-   0        0        0      358 2023-06-21 20:45:30.000000 QT-PyQt-PySide-Custom-Widgets-0.6.5/Custom_Widgets/Qss/icons/original_svg/layout.svg
--rw-rw-rw-   0        0        0      569 2023-06-21 20:45:30.000000 QT-PyQt-PySide-Custom-Widgets-0.6.5/Custom_Widgets/Qss/icons/original_svg/life-buoy.svg
--rw-rw-rw-   0        0        0     2445 2023-06-21 20:45:30.000000 QT-PyQt-PySide-Custom-Widgets-0.6.5/Custom_Widgets/Qss/icons/original_svg/line_horizontal.svg
--rw-rw-rw-   0        0        0     2454 2023-06-21 20:45:30.000000 QT-PyQt-PySide-Custom-Widgets-0.6.5/Custom_Widgets/Qss/icons/original_svg/line_vertical.svg
--rw-rw-rw-   0        0        0      349 2023-06-21 20:45:30.000000 QT-PyQt-PySide-Custom-Widgets-0.6.5/Custom_Widgets/Qss/icons/original_svg/link-2.svg
--rw-rw-rw-   0        0        0      365 2023-06-21 20:45:30.000000 QT-PyQt-PySide-Custom-Widgets-0.6.5/Custom_Widgets/Qss/icons/original_svg/link.svg
--rw-rw-rw-   0        0        0      394 2023-06-21 20:45:30.000000 QT-PyQt-PySide-Custom-Widgets-0.6.5/Custom_Widgets/Qss/icons/original_svg/linkedin.svg
--rw-rw-rw-   0        0        0      476 2023-06-21 20:45:30.000000 QT-PyQt-PySide-Custom-Widgets-0.6.5/Custom_Widgets/Qss/icons/original_svg/list.svg
--rw-rw-rw-   0        0        0      608 2023-06-21 20:45:30.000000 QT-PyQt-PySide-Custom-Widgets-0.6.5/Custom_Widgets/Qss/icons/original_svg/loader.svg
--rw-rw-rw-   0        0        0      315 2023-06-21 20:45:30.000000 QT-PyQt-PySide-Custom-Widgets-0.6.5/Custom_Widgets/Qss/icons/original_svg/lock.svg
--rw-rw-rw-   0        0        0      362 2023-06-21 20:45:30.000000 QT-PyQt-PySide-Custom-Widgets-0.6.5/Custom_Widgets/Qss/icons/original_svg/log-in.svg
--rw-rw-rw-   0        0        0      361 2023-06-21 20:45:30.000000 QT-PyQt-PySide-Custom-Widgets-0.6.5/Custom_Widgets/Qss/icons/original_svg/log-out.svg
--rw-rw-rw-   0        0        0      348 2023-06-21 20:45:30.000000 QT-PyQt-PySide-Custom-Widgets-0.6.5/Custom_Widgets/Qss/icons/original_svg/mail.svg
--rw-rw-rw-   0        0        0      316 2023-06-21 20:45:30.000000 QT-PyQt-PySide-Custom-Widgets-0.6.5/Custom_Widgets/Qss/icons/original_svg/map-pin.svg
--rw-rw-rw-   0        0        0      367 2023-06-21 20:45:30.000000 QT-PyQt-PySide-Custom-Widgets-0.6.5/Custom_Widgets/Qss/icons/original_svg/map.svg
--rw-rw-rw-   0        0        0      394 2023-06-21 20:45:31.000000 QT-PyQt-PySide-Custom-Widgets-0.6.5/Custom_Widgets/Qss/icons/original_svg/maximize-2.svg
--rw-rw-rw-   0        0        0      325 2023-06-21 20:45:31.000000 QT-PyQt-PySide-Custom-Widgets-0.6.5/Custom_Widgets/Qss/icons/original_svg/maximize.svg
--rw-rw-rw-   0        0        0      383 2023-06-21 20:45:31.000000 QT-PyQt-PySide-Custom-Widgets-0.6.5/Custom_Widgets/Qss/icons/original_svg/meh.svg
--rw-rw-rw-   0        0        0      340 2023-06-21 20:45:31.000000 QT-PyQt-PySide-Custom-Widgets-0.6.5/Custom_Widgets/Qss/icons/original_svg/menu.svg
--rw-rw-rw-   0        0        0      422 2023-06-21 20:45:31.000000 QT-PyQt-PySide-Custom-Widgets-0.6.5/Custom_Widgets/Qss/icons/original_svg/message-circle.svg
--rw-rw-rw-   0        0        0      299 2023-06-21 20:45:31.000000 QT-PyQt-PySide-Custom-Widgets-0.6.5/Custom_Widgets/Qss/icons/original_svg/message-square.svg
--rw-rw-rw-   0        0        0      488 2023-06-21 20:45:31.000000 QT-PyQt-PySide-Custom-Widgets-0.6.5/Custom_Widgets/Qss/icons/original_svg/mic-off.svg
--rw-rw-rw-   0        0        0      412 2023-06-21 20:45:31.000000 QT-PyQt-PySide-Custom-Widgets-0.6.5/Custom_Widgets/Qss/icons/original_svg/mic.svg
--rw-rw-rw-   0        0        0      398 2023-06-21 20:45:31.000000 QT-PyQt-PySide-Custom-Widgets-0.6.5/Custom_Widgets/Qss/icons/original_svg/minimize-2.svg
--rw-rw-rw-   0        0        0      325 2023-06-21 20:45:31.000000 QT-PyQt-PySide-Custom-Widgets-0.6.5/Custom_Widgets/Qss/icons/original_svg/minimize.svg
--rw-rw-rw-   0        0        0      302 2023-06-21 20:45:31.000000 QT-PyQt-PySide-Custom-Widgets-0.6.5/Custom_Widgets/Qss/icons/original_svg/minus-circle.svg
--rw-rw-rw-   0        0        0      324 2023-06-21 20:45:31.000000 QT-PyQt-PySide-Custom-Widgets-0.6.5/Custom_Widgets/Qss/icons/original_svg/minus-square.svg
--rw-rw-rw-   0        0        0      255 2023-06-21 20:45:31.000000 QT-PyQt-PySide-Custom-Widgets-0.6.5/Custom_Widgets/Qss/icons/original_svg/minus.svg
--rw-rw-rw-   0        0        0      364 2023-06-21 20:45:31.000000 QT-PyQt-PySide-Custom-Widgets-0.6.5/Custom_Widgets/Qss/icons/original_svg/monitor.svg
--rw-rw-rw-   0        0        0      275 2023-06-21 20:45:31.000000 QT-PyQt-PySide-Custom-Widgets-0.6.5/Custom_Widgets/Qss/icons/original_svg/moon.svg
--rw-rw-rw-   0        0        0      337 2023-06-21 20:45:31.000000 QT-PyQt-PySide-Custom-Widgets-0.6.5/Custom_Widgets/Qss/icons/original_svg/more-horizontal.svg
--rw-rw-rw-   0        0        0      335 2023-06-21 20:45:31.000000 QT-PyQt-PySide-Custom-Widgets-0.6.5/Custom_Widgets/Qss/icons/original_svg/more-vertical.svg
--rw-rw-rw-   0        0        0      305 2023-06-21 20:45:31.000000 QT-PyQt-PySide-Custom-Widgets-0.6.5/Custom_Widgets/Qss/icons/original_svg/mouse-pointer.svg
--rw-rw-rw-   0        0        0      480 2023-06-21 20:45:31.000000 QT-PyQt-PySide-Custom-Widgets-0.6.5/Custom_Widgets/Qss/icons/original_svg/move.svg
--rw-rw-rw-   0        0        0      321 2023-06-21 20:45:31.000000 QT-PyQt-PySide-Custom-Widgets-0.6.5/Custom_Widgets/Qss/icons/original_svg/music.svg
--rw-rw-rw-   0        0        0      273 2023-06-21 20:45:31.000000 QT-PyQt-PySide-Custom-Widgets-0.6.5/Custom_Widgets/Qss/icons/original_svg/navigation-2.svg
--rw-rw-rw-   0        0        0      271 2023-06-21 20:45:31.000000 QT-PyQt-PySide-Custom-Widgets-0.6.5/Custom_Widgets/Qss/icons/original_svg/navigation.svg
--rw-rw-rw-   0        0        0      312 2023-06-21 20:45:31.000000 QT-PyQt-PySide-Custom-Widgets-0.6.5/Custom_Widgets/Qss/icons/original_svg/octagon.svg
--rw-rw-rw-   0        0        0      511 2023-06-21 20:45:31.000000 QT-PyQt-PySide-Custom-Widgets-0.6.5/Custom_Widgets/Qss/icons/original_svg/package.svg
--rw-rw-rw-   0        0        0      346 2023-06-21 20:45:31.000000 QT-PyQt-PySide-Custom-Widgets-0.6.5/Custom_Widgets/Qss/icons/original_svg/paperclip.svg
--rw-rw-rw-   0        0        0      346 2023-06-21 20:45:31.000000 QT-PyQt-PySide-Custom-Widgets-0.6.5/Custom_Widgets/Qss/icons/original_svg/pause-circle.svg
--rw-rw-rw-   0        0        0      306 2023-06-21 20:45:31.000000 QT-PyQt-PySide-Custom-Widgets-0.6.5/Custom_Widgets/Qss/icons/original_svg/pause.svg
--rw-rw-rw-   0        0        0      385 2023-06-21 20:45:31.000000 QT-PyQt-PySide-Custom-Widgets-0.6.5/Custom_Widgets/Qss/icons/original_svg/pen-tool.svg
--rw-rw-rw-   0        0        0      344 2023-06-21 20:45:31.000000 QT-PyQt-PySide-Custom-Widgets-0.6.5/Custom_Widgets/Qss/icons/original_svg/percent.svg
--rw-rw-rw-   0        0        0      570 2023-06-21 20:45:31.000000 QT-PyQt-PySide-Custom-Widgets-0.6.5/Custom_Widgets/Qss/icons/original_svg/phone-call.svg
--rw-rw-rw-   0        0        0      612 2023-06-21 20:45:31.000000 QT-PyQt-PySide-Custom-Widgets-0.6.5/Custom_Widgets/Qss/icons/original_svg/phone-forwarded.svg
--rw-rw-rw-   0        0        0      611 2023-06-21 20:45:31.000000 QT-PyQt-PySide-Custom-Widgets-0.6.5/Custom_Widgets/Qss/icons/original_svg/phone-incoming.svg
--rw-rw-rw-   0        0        0      607 2023-06-21 20:45:31.000000 QT-PyQt-PySide-Custom-Widgets-0.6.5/Custom_Widgets/Qss/icons/original_svg/phone-missed.svg
--rw-rw-rw-   0        0        0      585 2023-06-21 20:45:31.000000 QT-PyQt-PySide-Custom-Widgets-0.6.5/Custom_Widgets/Qss/icons/original_svg/phone-off.svg
--rw-rw-rw-   0        0        0      611 2023-06-21 20:45:31.000000 QT-PyQt-PySide-Custom-Widgets-0.6.5/Custom_Widgets/Qss/icons/original_svg/phone-outgoing.svg
--rw-rw-rw-   0        0        0      514 2023-06-21 20:45:31.000000 QT-PyQt-PySide-Custom-Widgets-0.6.5/Custom_Widgets/Qss/icons/original_svg/phone.svg
--rw-rw-rw-   0        0        0      309 2023-06-21 20:45:31.000000 QT-PyQt-PySide-Custom-Widgets-0.6.5/Custom_Widgets/Qss/icons/original_svg/pie-chart.svg
--rw-rw-rw-   0        0        0      307 2023-06-21 20:45:31.000000 QT-PyQt-PySide-Custom-Widgets-0.6.5/Custom_Widgets/Qss/icons/original_svg/play-circle.svg
--rw-rw-rw-   0        0        0      257 2023-06-21 20:45:31.000000 QT-PyQt-PySide-Custom-Widgets-0.6.5/Custom_Widgets/Qss/icons/original_svg/play.svg
--rw-rw-rw-   0        0        0      345 2023-06-21 20:45:31.000000 QT-PyQt-PySide-Custom-Widgets-0.6.5/Custom_Widgets/Qss/icons/original_svg/plus-circle.svg
--rw-rw-rw-   0        0        0      367 2023-06-21 20:45:31.000000 QT-PyQt-PySide-Custom-Widgets-0.6.5/Custom_Widgets/Qss/icons/original_svg/plus-square.svg
--rw-rw-rw-   0        0        0      298 2023-06-21 20:45:31.000000 QT-PyQt-PySide-Custom-Widgets-0.6.5/Custom_Widgets/Qss/icons/original_svg/plus.svg
--rw-rw-rw-   0        0        0      352 2023-06-21 20:45:31.000000 QT-PyQt-PySide-Custom-Widgets-0.6.5/Custom_Widgets/Qss/icons/original_svg/pocket.svg
--rw-rw-rw-   0        0        0      302 2023-06-21 20:45:31.000000 QT-PyQt-PySide-Custom-Widgets-0.6.5/Custom_Widgets/Qss/icons/original_svg/power.svg
--rw-rw-rw-   0        0        0      401 2023-06-21 20:45:31.000000 QT-PyQt-PySide-Custom-Widgets-0.6.5/Custom_Widgets/Qss/icons/original_svg/printer.svg
--rw-rw-rw-   0        0        0      383 2023-06-21 20:45:31.000000 QT-PyQt-PySide-Custom-Widgets-0.6.5/Custom_Widgets/Qss/icons/original_svg/radio.svg
--rw-rw-rw-   0        0        0     2714 2023-06-21 20:45:31.000000 QT-PyQt-PySide-Custom-Widgets-0.6.5/Custom_Widgets/Qss/icons/original_svg/radio_checked.svg
--rw-rw-rw-   0        0        0     2419 2023-06-21 20:45:31.000000 QT-PyQt-PySide-Custom-Widgets-0.6.5/Custom_Widgets/Qss/icons/original_svg/radio_unchecked.svg
--rw-rw-rw-   0        0        0      394 2023-06-21 20:45:31.000000 QT-PyQt-PySide-Custom-Widgets-0.6.5/Custom_Widgets/Qss/icons/original_svg/refresh-ccw.svg
--rw-rw-rw-   0        0        0      394 2023-06-21 20:45:31.000000 QT-PyQt-PySide-Custom-Widgets-0.6.5/Custom_Widgets/Qss/icons/original_svg/refresh-cw.svg
--rw-rw-rw-   0        0        0      386 2023-06-21 20:45:31.000000 QT-PyQt-PySide-Custom-Widgets-0.6.5/Custom_Widgets/Qss/icons/original_svg/repeat.svg
--rw-rw-rw-   0        0        0      313 2023-06-21 20:45:31.000000 QT-PyQt-PySide-Custom-Widgets-0.6.5/Custom_Widgets/Qss/icons/original_svg/rewind.svg
--rw-rw-rw-   0        0        0      311 2023-06-21 20:45:31.000000 QT-PyQt-PySide-Custom-Widgets-0.6.5/Custom_Widgets/Qss/icons/original_svg/rotate-ccw.svg
--rw-rw-rw-   0        0        0      315 2023-06-21 20:45:31.000000 QT-PyQt-PySide-Custom-Widgets-0.6.5/Custom_Widgets/Qss/icons/original_svg/rotate-cw.svg
--rw-rw-rw-   0        0        0      324 2023-06-21 20:45:31.000000 QT-PyQt-PySide-Custom-Widgets-0.6.5/Custom_Widgets/Qss/icons/original_svg/rss.svg
--rw-rw-rw-   0        0        0      386 2023-06-21 20:45:31.000000 QT-PyQt-PySide-Custom-Widgets-0.6.5/Custom_Widgets/Qss/icons/original_svg/save.svg
--rw-rw-rw-   0        0        0      438 2023-06-21 20:45:31.000000 QT-PyQt-PySide-Custom-Widgets-0.6.5/Custom_Widgets/Qss/icons/original_svg/scissors.svg
--rw-rw-rw-   0        0        0      302 2023-06-21 20:45:31.000000 QT-PyQt-PySide-Custom-Widgets-0.6.5/Custom_Widgets/Qss/icons/original_svg/search.svg
--rw-rw-rw-   0        0        0      308 2023-06-21 20:45:31.000000 QT-PyQt-PySide-Custom-Widgets-0.6.5/Custom_Widgets/Qss/icons/original_svg/send.svg
--rw-rw-rw-   0        0        0      425 2023-06-21 20:45:31.000000 QT-PyQt-PySide-Custom-Widgets-0.6.5/Custom_Widgets/Qss/icons/original_svg/server.svg
--rw-rw-rw-   0        0        0     1005 2023-06-21 20:45:31.000000 QT-PyQt-PySide-Custom-Widgets-0.6.5/Custom_Widgets/Qss/icons/original_svg/settings.svg
--rw-rw-rw-   0        0        0      439 2023-06-21 20:45:31.000000 QT-PyQt-PySide-Custom-Widgets-0.6.5/Custom_Widgets/Qss/icons/original_svg/share-2.svg
--rw-rw-rw-   0        0        0      358 2023-06-21 20:45:31.000000 QT-PyQt-PySide-Custom-Widgets-0.6.5/Custom_Widgets/Qss/icons/original_svg/share.svg
--rw-rw-rw-   0        0        0      399 2023-06-21 20:45:31.000000 QT-PyQt-PySide-Custom-Widgets-0.6.5/Custom_Widgets/Qss/icons/original_svg/shield-off.svg
--rw-rw-rw-   0        0        0      273 2023-06-21 20:45:31.000000 QT-PyQt-PySide-Custom-Widgets-0.6.5/Custom_Widgets/Qss/icons/original_svg/shield.svg
--rw-rw-rw-   0        0        0      366 2023-06-21 20:45:31.000000 QT-PyQt-PySide-Custom-Widgets-0.6.5/Custom_Widgets/Qss/icons/original_svg/shopping-bag.svg
--rw-rw-rw-   0        0        0      377 2023-06-21 20:45:31.000000 QT-PyQt-PySide-Custom-Widgets-0.6.5/Custom_Widgets/Qss/icons/original_svg/shopping-cart.svg
--rw-rw-rw-   0        0        0      435 2023-06-21 20:45:31.000000 QT-PyQt-PySide-Custom-Widgets-0.6.5/Custom_Widgets/Qss/icons/original_svg/shuffle.svg
--rw-rw-rw-   0        0        0      317 2023-06-21 20:45:31.000000 QT-PyQt-PySide-Custom-Widgets-0.6.5/Custom_Widgets/Qss/icons/original_svg/sidebar.svg
--rw-rw-rw-   0        0        0      307 2023-06-21 20:45:31.000000 QT-PyQt-PySide-Custom-Widgets-0.6.5/Custom_Widgets/Qss/icons/original_svg/skip-back.svg
--rw-rw-rw-   0        0        0      309 2023-06-21 20:45:31.000000 QT-PyQt-PySide-Custom-Widgets-0.6.5/Custom_Widgets/Qss/icons/original_svg/skip-forward.svg
--rw-rw-rw-   0        0        0      993 2023-06-21 20:45:31.000000 QT-PyQt-PySide-Custom-Widgets-0.6.5/Custom_Widgets/Qss/icons/original_svg/slack.svg
--rw-rw-rw-   0        0        0      306 2023-06-21 20:45:31.000000 QT-PyQt-PySide-Custom-Widgets-0.6.5/Custom_Widgets/Qss/icons/original_svg/slash.svg
--rw-rw-rw-   0        0        0      605 2023-06-21 20:45:31.000000 QT-PyQt-PySide-Custom-Widgets-0.6.5/Custom_Widgets/Qss/icons/original_svg/sliders.svg
--rw-rw-rw-   0        0        0      326 2023-06-21 20:45:31.000000 QT-PyQt-PySide-Custom-Widgets-0.6.5/Custom_Widgets/Qss/icons/original_svg/smartphone.svg
--rw-rw-rw-   0        0        0      382 2023-06-21 20:45:31.000000 QT-PyQt-PySide-Custom-Widgets-0.6.5/Custom_Widgets/Qss/icons/original_svg/smile.svg
--rw-rw-rw-   0        0        0      360 2023-06-21 20:45:31.000000 QT-PyQt-PySide-Custom-Widgets-0.6.5/Custom_Widgets/Qss/icons/original_svg/speaker.svg
--rw-rw-rw-   0        0        0      274 2023-06-21 20:45:31.000000 QT-PyQt-PySide-Custom-Widgets-0.6.5/Custom_Widgets/Qss/icons/original_svg/square.svg
--rw-rw-rw-   0        0        0      333 2023-06-21 20:45:31.000000 QT-PyQt-PySide-Custom-Widgets-0.6.5/Custom_Widgets/Qss/icons/original_svg/star.svg
--rw-rw-rw-   0        0        0      303 2023-06-21 20:45:31.000000 QT-PyQt-PySide-Custom-Widgets-0.6.5/Custom_Widgets/Qss/icons/original_svg/stop-circle.svg
--rw-rw-rw-   0        0        0      644 2023-06-21 20:45:31.000000 QT-PyQt-PySide-Custom-Widgets-0.6.5/Custom_Widgets/Qss/icons/original_svg/sun.svg
--rw-rw-rw-   0        0        0      583 2023-06-21 20:45:31.000000 QT-PyQt-PySide-Custom-Widgets-0.6.5/Custom_Widgets/Qss/icons/original_svg/sunrise.svg
--rw-rw-rw-   0        0        0      582 2023-06-21 20:45:31.000000 QT-PyQt-PySide-Custom-Widgets-0.6.5/Custom_Widgets/Qss/icons/original_svg/sunset.svg
--rw-rw-rw-   0        0        0      322 2023-06-21 20:45:31.000000 QT-PyQt-PySide-Custom-Widgets-0.6.5/Custom_Widgets/Qss/icons/original_svg/tablet.svg
--rw-rw-rw-   0        0        0      349 2023-06-21 20:45:31.000000 QT-PyQt-PySide-Custom-Widgets-0.6.5/Custom_Widgets/Qss/icons/original_svg/tag.svg
--rw-rw-rw-   0        0        0      330 2023-06-21 20:45:31.000000 QT-PyQt-PySide-Custom-Widgets-0.6.5/Custom_Widgets/Qss/icons/original_svg/target.svg
--rw-rw-rw-   0        0        0      304 2023-06-21 20:45:31.000000 QT-PyQt-PySide-Custom-Widgets-0.6.5/Custom_Widgets/Qss/icons/original_svg/terminal.svg
--rw-rw-rw-   0        0        0      291 2023-06-21 20:45:31.000000 QT-PyQt-PySide-Custom-Widgets-0.6.5/Custom_Widgets/Qss/icons/original_svg/thermometer.svg
--rw-rw-rw-   0        0        0      368 2023-06-21 20:45:31.000000 QT-PyQt-PySide-Custom-Widgets-0.6.5/Custom_Widgets/Qss/icons/original_svg/thumbs-down.svg
--rw-rw-rw-   0        0        0      348 2023-06-21 20:45:31.000000 QT-PyQt-PySide-Custom-Widgets-0.6.5/Custom_Widgets/Qss/icons/original_svg/thumbs-up.svg
--rw-rw-rw-   0        0        0      317 2023-06-21 20:45:31.000000 QT-PyQt-PySide-Custom-Widgets-0.6.5/Custom_Widgets/Qss/icons/original_svg/toggle-left.svg
--rw-rw-rw-   0        0        0      319 2023-06-21 20:45:31.000000 QT-PyQt-PySide-Custom-Widgets-0.6.5/Custom_Widgets/Qss/icons/original_svg/toggle-right.svg
--rw-rw-rw-   0        0        0      380 2023-06-21 20:45:31.000000 QT-PyQt-PySide-Custom-Widgets-0.6.5/Custom_Widgets/Qss/icons/original_svg/tool.svg
--rw-rw-rw-   0        0        0     2703 2023-06-21 20:45:31.000000 QT-PyQt-PySide-Custom-Widgets-0.6.5/Custom_Widgets/Qss/icons/original_svg/toolbar_move_horizontal.svg
--rw-rw-rw-   0        0        0     2710 2023-06-21 20:45:31.000000 QT-PyQt-PySide-Custom-Widgets-0.6.5/Custom_Widgets/Qss/icons/original_svg/toolbar_move_vertical.svg
--rw-rw-rw-   0        0        0     2464 2023-06-21 20:45:31.000000 QT-PyQt-PySide-Custom-Widgets-0.6.5/Custom_Widgets/Qss/icons/original_svg/toolbar_separator_horizontal.svg
--rw-rw-rw-   0        0        0     2463 2023-06-21 20:45:31.000000 QT-PyQt-PySide-Custom-Widgets-0.6.5/Custom_Widgets/Qss/icons/original_svg/toolbar_separator_vertical.svg
--rw-rw-rw-   0        0        0     2347 2023-06-21 20:45:31.000000 QT-PyQt-PySide-Custom-Widgets-0.6.5/Custom_Widgets/Qss/icons/original_svg/transparent.svg
--rw-rw-rw-   0        0        0      442 2023-06-21 20:45:31.000000 QT-PyQt-PySide-Custom-Widgets-0.6.5/Custom_Widgets/Qss/icons/original_svg/trash-2.svg
--rw-rw-rw-   0        0        0      350 2023-06-21 20:45:31.000000 QT-PyQt-PySide-Custom-Widgets-0.6.5/Custom_Widgets/Qss/icons/original_svg/trash.svg
--rw-rw-rw-   0        0        0      367 2023-06-21 20:45:31.000000 QT-PyQt-PySide-Custom-Widgets-0.6.5/Custom_Widgets/Qss/icons/original_svg/trello.svg
--rw-rw-rw-   0        0        0      325 2023-06-21 20:45:31.000000 QT-PyQt-PySide-Custom-Widgets-0.6.5/Custom_Widgets/Qss/icons/original_svg/trending-down.svg
--rw-rw-rw-   0        0        0      322 2023-06-21 20:45:31.000000 QT-PyQt-PySide-Custom-Widgets-0.6.5/Custom_Widgets/Qss/icons/original_svg/trending-up.svg
--rw-rw-rw-   0        0        0      320 2023-06-21 20:45:31.000000 QT-PyQt-PySide-Custom-Widgets-0.6.5/Custom_Widgets/Qss/icons/original_svg/triangle.svg
--rw-rw-rw-   0        0        0      409 2023-06-21 20:45:31.000000 QT-PyQt-PySide-Custom-Widgets-0.6.5/Custom_Widgets/Qss/icons/original_svg/truck.svg
--rw-rw-rw-   0        0        0      314 2023-06-21 20:45:31.000000 QT-PyQt-PySide-Custom-Widgets-0.6.5/Custom_Widgets/Qss/icons/original_svg/tv.svg
--rw-rw-rw-   0        0        0      271 2023-06-21 20:45:31.000000 QT-PyQt-PySide-Custom-Widgets-0.6.5/Custom_Widgets/Qss/icons/original_svg/twitch.svg
--rw-rw-rw-   0        0        0      402 2023-06-21 20:45:31.000000 QT-PyQt-PySide-Custom-Widgets-0.6.5/Custom_Widgets/Qss/icons/original_svg/twitter.svg
--rw-rw-rw-   0        0        0      346 2023-06-21 20:45:31.000000 QT-PyQt-PySide-Custom-Widgets-0.6.5/Custom_Widgets/Qss/icons/original_svg/type.svg
--rw-rw-rw-   0        0        0      284 2023-06-21 20:45:31.000000 QT-PyQt-PySide-Custom-Widgets-0.6.5/Custom_Widgets/Qss/icons/original_svg/umbrella.svg
--rw-rw-rw-   0        0        0      313 2023-06-21 20:45:31.000000 QT-PyQt-PySide-Custom-Widgets-0.6.5/Custom_Widgets/Qss/icons/original_svg/underline.svg
--rw-rw-rw-   0        0        0      316 2023-06-21 20:45:31.000000 QT-PyQt-PySide-Custom-Widgets-0.6.5/Custom_Widgets/Qss/icons/original_svg/unlock.svg
--rw-rw-rw-   0        0        0      425 2023-06-21 20:45:31.000000 QT-PyQt-PySide-Custom-Widgets-0.6.5/Custom_Widgets/Qss/icons/original_svg/upload-cloud.svg
--rw-rw-rw-   0        0        0      359 2023-06-21 20:45:31.000000 QT-PyQt-PySide-Custom-Widgets-0.6.5/Custom_Widgets/Qss/icons/original_svg/upload.svg
--rw-rw-rw-   0        0        0      361 2023-06-21 20:45:31.000000 QT-PyQt-PySide-Custom-Widgets-0.6.5/Custom_Widgets/Qss/icons/original_svg/user-check.svg
--rw-rw-rw-   0        0        0      359 2023-06-21 20:45:31.000000 QT-PyQt-PySide-Custom-Widgets-0.6.5/Custom_Widgets/Qss/icons/original_svg/user-minus.svg
--rw-rw-rw-   0        0        0      402 2023-06-21 20:45:31.000000 QT-PyQt-PySide-Custom-Widgets-0.6.5/Custom_Widgets/Qss/icons/original_svg/user-plus.svg
--rw-rw-rw-   0        0        0      398 2023-06-21 20:45:31.000000 QT-PyQt-PySide-Custom-Widgets-0.6.5/Custom_Widgets/Qss/icons/original_svg/user-x.svg
--rw-rw-rw-   0        0        0      307 2023-06-21 20:45:31.000000 QT-PyQt-PySide-Custom-Widgets-0.6.5/Custom_Widgets/Qss/icons/original_svg/user.svg
--rw-rw-rw-   0        0        0      394 2023-06-21 20:45:31.000000 QT-PyQt-PySide-Custom-Widgets-0.6.5/Custom_Widgets/Qss/icons/original_svg/users.svg
--rw-rw-rw-   0        0        0      373 2023-06-21 20:45:31.000000 QT-PyQt-PySide-Custom-Widgets-0.6.5/Custom_Widgets/Qss/icons/original_svg/video-off.svg
--rw-rw-rw-   0        0        0      323 2023-06-21 20:45:31.000000 QT-PyQt-PySide-Custom-Widgets-0.6.5/Custom_Widgets/Qss/icons/original_svg/video.svg
--rw-rw-rw-   0        0        0      352 2023-06-21 20:45:31.000000 QT-PyQt-PySide-Custom-Widgets-0.6.5/Custom_Widgets/Qss/icons/original_svg/voicemail.svg
--rw-rw-rw-   0        0        0      322 2023-06-21 20:45:31.000000 QT-PyQt-PySide-Custom-Widgets-0.6.5/Custom_Widgets/Qss/icons/original_svg/volume-1.svg
--rw-rw-rw-   0        0        0      353 2023-06-21 20:45:31.000000 QT-PyQt-PySide-Custom-Widgets-0.6.5/Custom_Widgets/Qss/icons/original_svg/volume-2.svg
--rw-rw-rw-   0        0        0      364 2023-06-21 20:45:31.000000 QT-PyQt-PySide-Custom-Widgets-0.6.5/Custom_Widgets/Qss/icons/original_svg/volume-x.svg
--rw-rw-rw-   0        0        0      274 2023-06-21 20:45:31.000000 QT-PyQt-PySide-Custom-Widgets-0.6.5/Custom_Widgets/Qss/icons/original_svg/volume.svg
--rw-rw-rw-   0        0        0      456 2023-06-21 20:45:31.000000 QT-PyQt-PySide-Custom-Widgets-0.6.5/Custom_Widgets/Qss/icons/original_svg/watch.svg
--rw-rw-rw-   0        0        0      563 2023-06-21 20:45:31.000000 QT-PyQt-PySide-Custom-Widgets-0.6.5/Custom_Widgets/Qss/icons/original_svg/wifi-off.svg
--rw-rw-rw-   0        0        0      395 2023-06-21 20:45:31.000000 QT-PyQt-PySide-Custom-Widgets-0.6.5/Custom_Widgets/Qss/icons/original_svg/wifi.svg
--rw-rw-rw-   0        0        0      320 2023-06-21 20:45:31.000000 QT-PyQt-PySide-Custom-Widgets-0.6.5/Custom_Widgets/Qss/icons/original_svg/wind.svg
--rw-rw-rw-   0        0        0     2953 2023-06-21 20:45:31.000000 QT-PyQt-PySide-Custom-Widgets-0.6.5/Custom_Widgets/Qss/icons/original_svg/window_close.svg
--rw-rw-rw-   0        0        0     3018 2023-06-21 20:45:31.000000 QT-PyQt-PySide-Custom-Widgets-0.6.5/Custom_Widgets/Qss/icons/original_svg/window_grip.svg
--rw-rw-rw-   0        0        0     2465 2023-06-21 20:45:31.000000 QT-PyQt-PySide-Custom-Widgets-0.6.5/Custom_Widgets/Qss/icons/original_svg/window_minimize.svg
--rw-rw-rw-   0        0        0     2979 2023-06-21 20:45:31.000000 QT-PyQt-PySide-Custom-Widgets-0.6.5/Custom_Widgets/Qss/icons/original_svg/window_undock.svg
--rw-rw-rw-   0        0        0      340 2023-06-21 20:45:31.000000 QT-PyQt-PySide-Custom-Widgets-0.6.5/Custom_Widgets/Qss/icons/original_svg/x-circle.svg
--rw-rw-rw-   0        0        0      400 2023-06-21 20:45:31.000000 QT-PyQt-PySide-Custom-Widgets-0.6.5/Custom_Widgets/Qss/icons/original_svg/x-octagon.svg
--rw-rw-rw-   0        0        0      362 2023-06-21 20:45:31.000000 QT-PyQt-PySide-Custom-Widgets-0.6.5/Custom_Widgets/Qss/icons/original_svg/x-square.svg
--rw-rw-rw-   0        0        0      293 2023-06-21 20:45:31.000000 QT-PyQt-PySide-Custom-Widgets-0.6.5/Custom_Widgets/Qss/icons/original_svg/x.svg
--rw-rw-rw-   0        0        0      559 2023-06-21 20:45:31.000000 QT-PyQt-PySide-Custom-Widgets-0.6.5/Custom_Widgets/Qss/icons/original_svg/youtube.svg
--rw-rw-rw-   0        0        0      427 2023-06-21 20:45:31.000000 QT-PyQt-PySide-Custom-Widgets-0.6.5/Custom_Widgets/Qss/icons/original_svg/zap-off.svg
--rw-rw-rw-   0        0        0      276 2023-06-21 20:45:31.000000 QT-PyQt-PySide-Custom-Widgets-0.6.5/Custom_Widgets/Qss/icons/original_svg/zap.svg
--rw-rw-rw-   0        0        0      391 2023-06-21 20:45:31.000000 QT-PyQt-PySide-Custom-Widgets-0.6.5/Custom_Widgets/Qss/icons/original_svg/zoom-in.svg
--rw-rw-rw-   0        0        0      348 2023-06-21 20:45:31.000000 QT-PyQt-PySide-Custom-Widgets-0.6.5/Custom_Widgets/Qss/icons/original_svg/zoom-out.svg
--rw-rw-rw-   0        0        0      134 2023-06-21 20:45:30.000000 QT-PyQt-PySide-Custom-Widgets-0.6.5/Custom_Widgets/Qss/main.scss
--rw-rw-rw-   0        0        0    30871 2023-06-21 20:45:30.000000 QT-PyQt-PySide-Custom-Widgets-0.6.5/Custom_Widgets/RoundProgressBar.py
--rw-rw-rw-   0        0        0    40717 2023-06-21 20:45:30.000000 QT-PyQt-PySide-Custom-Widgets-0.6.5/Custom_Widgets/SpiralProgressBar.py
--rw-rw-rw-   0        0        0   156605 2023-06-21 20:45:30.000000 QT-PyQt-PySide-Custom-Widgets-0.6.5/Custom_Widgets/Widgets.py
--rw-rw-rw-   0        0        0     4824 2023-06-21 20:45:30.000000 QT-PyQt-PySide-Custom-Widgets-0.6.5/Custom_Widgets/WidgetsWorker.py
--rw-rw-rw-   0        0        0       39 2023-06-21 20:45:30.000000 QT-PyQt-PySide-Custom-Widgets-0.6.5/Custom_Widgets/__init__.py
-drwxrwxrwx   0        0        0        0 2023-06-21 21:13:06.739545 QT-PyQt-PySide-Custom-Widgets-0.6.5/Custom_Widgets/components/
-drwxrwxrwx   0        0        0        0 2023-06-21 21:13:08.003119 QT-PyQt-PySide-Custom-Widgets-0.6.5/Custom_Widgets/components/json/
--rw-rw-rw-   0        0        0      344 2023-06-21 20:45:31.000000 QT-PyQt-PySide-Custom-Widgets-0.6.5/Custom_Widgets/components/json/style.json
-drwxrwxrwx   0        0        0        0 2023-06-21 21:13:08.025113 QT-PyQt-PySide-Custom-Widgets-0.6.5/Custom_Widgets/components/python/
-drwxrwxrwx   0        0        0        0 2023-06-21 21:13:08.062085 QT-PyQt-PySide-Custom-Widgets-0.6.5/Custom_Widgets/components/python/__pycache__/
--rw-rw-rw-   0        0        0      853 2023-06-21 20:45:31.000000 QT-PyQt-PySide-Custom-Widgets-0.6.5/Custom_Widgets/components/python/__pycache__/main.cpython-310.pyc
--rw-rw-rw-   0        0        0      836 2023-06-21 20:45:31.000000 QT-PyQt-PySide-Custom-Widgets-0.6.5/Custom_Widgets/components/python/__pycache__/main.cpython-38.pyc
--rw-rw-rw-   0        0        0     2561 2023-06-21 20:45:31.000000 QT-PyQt-PySide-Custom-Widgets-0.6.5/Custom_Widgets/components/python/__pycache__/ui_interface.cpython-310.pyc
--rw-rw-rw-   0        0        0     2552 2023-06-21 20:45:31.000000 QT-PyQt-PySide-Custom-Widgets-0.6.5/Custom_Widgets/components/python/__pycache__/ui_interface.cpython-38.pyc
--rw-rw-rw-   0        0        0     2679 2023-06-21 20:45:31.000000 QT-PyQt-PySide-Custom-Widgets-0.6.5/Custom_Widgets/components/python/main.py
--rw-rw-rw-   0        0        0     3127 2023-06-21 20:45:31.000000 QT-PyQt-PySide-Custom-Widgets-0.6.5/Custom_Widgets/components/python/ui_interface.py
-drwxrwxrwx   0        0        0        0 2023-06-21 21:13:08.067082 QT-PyQt-PySide-Custom-Widgets-0.6.5/Custom_Widgets/components/uis/
--rw-rw-rw-   0        0        0     2691 2023-06-21 20:45:31.000000 QT-PyQt-PySide-Custom-Widgets-0.6.5/Custom_Widgets/components/uis/interface.ui
--rw-rw-rw-   0        0        0     1242 2023-06-21 20:45:30.000000 QT-PyQt-PySide-Custom-Widgets-0.6.5/Custom_Widgets/interface.ui
--rw-rw-rw-   0        0        0     2368 2023-06-21 20:45:30.000000 QT-PyQt-PySide-Custom-Widgets-0.6.5/Custom_Widgets/main.py
--rw-rw-rw-   0        0        0    35149 2021-06-11 19:06:36.000000 QT-PyQt-PySide-Custom-Widgets-0.6.5/LICENSE
--rw-rw-rw-   0        0        0       82 2022-02-17 19:32:18.000000 QT-PyQt-PySide-Custom-Widgets-0.6.5/MANIFEST.in
--rw-rw-rw-   0        0        0     4158 2023-06-21 21:13:08.167031 QT-PyQt-PySide-Custom-Widgets-0.6.5/PKG-INFO
-drwxrwxrwx   0        0        0        0 2023-06-21 21:13:08.163028 QT-PyQt-PySide-Custom-Widgets-0.6.5/QT_PyQt_PySide_Custom_Widgets.egg-info/
--rw-rw-rw-   0        0        0     4158 2023-06-21 21:13:03.000000 QT-PyQt-PySide-Custom-Widgets-0.6.5/QT_PyQt_PySide_Custom_Widgets.egg-info/PKG-INFO
--rw-rw-rw-   0        0        0    19073 2023-06-21 21:13:04.000000 QT-PyQt-PySide-Custom-Widgets-0.6.5/QT_PyQt_PySide_Custom_Widgets.egg-info/SOURCES.txt
--rw-rw-rw-   0        0        0        1 2023-06-21 21:13:03.000000 QT-PyQt-PySide-Custom-Widgets-0.6.5/QT_PyQt_PySide_Custom_Widgets.egg-info/dependency_links.txt
--rw-rw-rw-   0        0        0       45 2023-06-21 21:13:03.000000 QT-PyQt-PySide-Custom-Widgets-0.6.5/QT_PyQt_PySide_Custom_Widgets.egg-info/requires.txt
--rw-rw-rw-   0        0        0       15 2023-06-21 21:13:03.000000 QT-PyQt-PySide-Custom-Widgets-0.6.5/QT_PyQt_PySide_Custom_Widgets.egg-info/top_level.txt
--rw-rw-rw-   0        0        0     3169 2022-08-11 03:08:01.000000 QT-PyQt-PySide-Custom-Widgets-0.6.5/README.md
--rw-rw-rw-   0        0        0       42 2023-06-21 21:13:08.169023 QT-PyQt-PySide-Custom-Widgets-0.6.5/setup.cfg
--rw-rw-rw-   0        0        0     2253 2023-06-21 21:09:53.000000 QT-PyQt-PySide-Custom-Widgets-0.6.5/setup.py
+drwxrwxrwx   0        0        0        0 2023-06-24 14:28:52.611738 QT-PyQt-PySide-Custom-Widgets-0.6.6/
+drwxrwxrwx   0        0        0        0 2023-06-24 14:28:47.780965 QT-PyQt-PySide-Custom-Widgets-0.6.6/Custom_Widgets/
+-rw-rw-rw-   0        0        0    66370 2023-06-21 21:32:18.000000 QT-PyQt-PySide-Custom-Widgets-0.6.6/Custom_Widgets/AnalogGaugeWidget.py
+drwxrwxrwx   0        0        0        0 2023-06-24 14:28:47.830021 QT-PyQt-PySide-Custom-Widgets-0.6.6/Custom_Widgets/ProgressIndicator/
+-rw-rw-rw-   0        0        0        0 2023-06-21 21:32:18.000000 QT-PyQt-PySide-Custom-Widgets-0.6.6/Custom_Widgets/ProgressIndicator/__init__.py
+drwxrwxrwx   0        0        0        0 2023-06-24 14:28:47.847546 QT-PyQt-PySide-Custom-Widgets-0.6.6/Custom_Widgets/ProgressIndicator/__pycache__/
+-rw-rw-rw-   0        0        0      185 2023-06-21 21:32:18.000000 QT-PyQt-PySide-Custom-Widgets-0.6.6/Custom_Widgets/ProgressIndicator/__pycache__/__init__.cpython-310.pyc
+-rw-rw-rw-   0        0        0      178 2023-06-21 21:32:18.000000 QT-PyQt-PySide-Custom-Widgets-0.6.6/Custom_Widgets/ProgressIndicator/__pycache__/__init__.cpython-38.pyc
+-rw-rw-rw-   0        0        0     3840 2023-06-21 21:32:18.000000 QT-PyQt-PySide-Custom-Widgets-0.6.6/Custom_Widgets/ProgressIndicator/__pycache__/test.cpython-310.pyc
+-rw-rw-rw-   0        0        0     3948 2023-06-21 21:32:18.000000 QT-PyQt-PySide-Custom-Widgets-0.6.6/Custom_Widgets/ProgressIndicator/__pycache__/test.cpython-38.pyc
+-rw-rw-rw-   0        0        0     5285 2023-06-21 21:32:18.000000 QT-PyQt-PySide-Custom-Widgets-0.6.6/Custom_Widgets/ProgressIndicator/__pycache__/ui_interface.cpython-310.pyc
+-rw-rw-rw-   0        0        0     5276 2023-06-21 21:32:18.000000 QT-PyQt-PySide-Custom-Widgets-0.6.6/Custom_Widgets/ProgressIndicator/__pycache__/ui_interface.cpython-38.pyc
+-rw-rw-rw-   0        0        0     5297 2023-06-21 21:32:18.000000 QT-PyQt-PySide-Custom-Widgets-0.6.6/Custom_Widgets/ProgressIndicator/__pycache__/ui_interface.cpython-39.pyc
+-rw-rw-rw-   0        0        0     8502 2023-06-21 21:32:18.000000 QT-PyQt-PySide-Custom-Widgets-0.6.6/Custom_Widgets/ProgressIndicator/interface.ui
+-rw-rw-rw-   0        0        0     9452 2023-06-21 21:32:18.000000 QT-PyQt-PySide-Custom-Widgets-0.6.6/Custom_Widgets/ProgressIndicator/test.py
+-rw-rw-rw-   0        0        0     9629 2023-06-21 21:32:18.000000 QT-PyQt-PySide-Custom-Widgets-0.6.6/Custom_Widgets/ProgressIndicator/ui_interface.py
+-rw-rw-rw-   0        0        0    14071 2023-06-21 21:32:18.000000 QT-PyQt-PySide-Custom-Widgets-0.6.6/Custom_Widgets/ProjectMaker.py
+drwxrwxrwx   0        0        0        0 2023-06-24 14:28:47.933631 QT-PyQt-PySide-Custom-Widgets-0.6.6/Custom_Widgets/Qss/
+-rw-rw-rw-   0        0        0    39288 2023-06-21 21:32:18.000000 QT-PyQt-PySide-Custom-Widgets-0.6.6/Custom_Widgets/Qss/QSS_Resources.qrc
+-rw-rw-rw-   0        0        0     6351 2023-06-22 15:51:45.000000 QT-PyQt-PySide-Custom-Widgets-0.6.6/Custom_Widgets/Qss/SassCompiler.py
+-rw-rw-rw-   0        0        0    15602 2023-06-24 12:21:15.000000 QT-PyQt-PySide-Custom-Widgets-0.6.6/Custom_Widgets/Qss/SvgToPngIcons.py
+-rw-rw-rw-   0        0        0       39 2023-06-21 21:32:18.000000 QT-PyQt-PySide-Custom-Widgets-0.6.6/Custom_Widgets/Qss/__init__.py
+drwxrwxrwx   0        0        0        0 2023-06-24 14:28:48.001951 QT-PyQt-PySide-Custom-Widgets-0.6.6/Custom_Widgets/Qss/__pycache__/
+-rw-rw-rw-   0        0        0   630113 2023-06-21 21:32:18.000000 QT-PyQt-PySide-Custom-Widgets-0.6.6/Custom_Widgets/Qss/__pycache__/QSS_Resources.cpython-39.pyc
+-rw-rw-rw-   0        0        0     3122 2023-06-21 21:32:18.000000 QT-PyQt-PySide-Custom-Widgets-0.6.6/Custom_Widgets/Qss/__pycache__/SassCompiler.cpython-310.pyc
+-rw-rw-rw-   0        0        0     8339 2023-06-22 09:04:23.000000 QT-PyQt-PySide-Custom-Widgets-0.6.6/Custom_Widgets/Qss/__pycache__/SassCompiler.cpython-311.pyc
+-rw-rw-rw-   0        0        0     3459 2023-06-24 11:32:42.000000 QT-PyQt-PySide-Custom-Widgets-0.6.6/Custom_Widgets/Qss/__pycache__/SassCompiler.cpython-38.pyc
+-rw-rw-rw-   0        0        0     6895 2023-06-21 21:32:18.000000 QT-PyQt-PySide-Custom-Widgets-0.6.6/Custom_Widgets/Qss/__pycache__/SvgToPngIcons.cpython-310.pyc
+-rw-rw-rw-   0        0        0    22615 2023-06-22 09:04:25.000000 QT-PyQt-PySide-Custom-Widgets-0.6.6/Custom_Widgets/Qss/__pycache__/SvgToPngIcons.cpython-311.pyc
+-rw-rw-rw-   0        0        0     7271 2023-06-24 12:21:39.000000 QT-PyQt-PySide-Custom-Widgets-0.6.6/Custom_Widgets/Qss/__pycache__/SvgToPngIcons.cpython-38.pyc
+-rw-rw-rw-   0        0        0     3158 2023-06-21 21:32:18.000000 QT-PyQt-PySide-Custom-Widgets-0.6.6/Custom_Widgets/Qss/__pycache__/SvgToPngIcons.cpython-39.pyc
+-rw-rw-rw-   0        0        0      192 2023-06-21 21:32:18.000000 QT-PyQt-PySide-Custom-Widgets-0.6.6/Custom_Widgets/Qss/__pycache__/__init__.cpython-310.pyc
+-rw-rw-rw-   0        0        0      221 2023-06-22 09:04:23.000000 QT-PyQt-PySide-Custom-Widgets-0.6.6/Custom_Widgets/Qss/__pycache__/__init__.cpython-311.pyc
+-rw-rw-rw-   0        0        0      177 2023-06-21 21:32:18.000000 QT-PyQt-PySide-Custom-Widgets-0.6.6/Custom_Widgets/Qss/__pycache__/__init__.cpython-37.pyc
+-rw-rw-rw-   0        0        0      185 2023-06-21 21:32:18.000000 QT-PyQt-PySide-Custom-Widgets-0.6.6/Custom_Widgets/Qss/__pycache__/__init__.cpython-38.pyc
+-rw-rw-rw-   0        0        0      188 2023-06-21 21:32:18.000000 QT-PyQt-PySide-Custom-Widgets-0.6.6/Custom_Widgets/Qss/__pycache__/__init__.cpython-39.pyc
+-rw-rw-rw-   0        0        0     6166 2023-06-21 21:32:18.000000 QT-PyQt-PySide-Custom-Widgets-0.6.6/Custom_Widgets/Qss/__pycache__/colorsystem.cpython-310.pyc
+-rw-rw-rw-   0        0        0    12628 2023-06-22 09:04:23.000000 QT-PyQt-PySide-Custom-Widgets-0.6.6/Custom_Widgets/Qss/__pycache__/colorsystem.cpython-311.pyc
+-rw-rw-rw-   0        0        0     6168 2023-06-21 21:32:18.000000 QT-PyQt-PySide-Custom-Widgets-0.6.6/Custom_Widgets/Qss/__pycache__/colorsystem.cpython-37.pyc
+-rw-rw-rw-   0        0        0     6491 2023-06-24 14:25:53.000000 QT-PyQt-PySide-Custom-Widgets-0.6.6/Custom_Widgets/Qss/__pycache__/colorsystem.cpython-38.pyc
+-rw-rw-rw-   0        0        0     6064 2023-06-21 21:32:18.000000 QT-PyQt-PySide-Custom-Widgets-0.6.6/Custom_Widgets/Qss/__pycache__/colorsystem.cpython-39.pyc
+-rw-rw-rw-   0        0        0   630112 2023-06-21 21:32:18.000000 QT-PyQt-PySide-Custom-Widgets-0.6.6/Custom_Widgets/Qss/__pycache__/resources_rc.cpython-39.pyc
+-rw-rw-rw-   0        0        0     2764 2023-06-21 21:32:18.000000 QT-PyQt-PySide-Custom-Widgets-0.6.6/Custom_Widgets/Qss/__pycache__/sassCompiler.cpython-39.pyc
+-rw-rw-rw-   0        0        0    60079 2023-06-21 21:32:18.000000 QT-PyQt-PySide-Custom-Widgets-0.6.6/Custom_Widgets/Qss/_styles.scss
+-rw-rw-rw-   0        0        0    10333 2023-06-24 14:27:11.000000 QT-PyQt-PySide-Custom-Widgets-0.6.6/Custom_Widgets/Qss/colorsystem.py
+drwxrwxrwx   0        0        0        0 2023-06-24 14:28:47.630917 QT-PyQt-PySide-Custom-Widgets-0.6.6/Custom_Widgets/Qss/icons/
+drwxrwxrwx   0        0        0        0 2023-06-24 14:28:52.434022 QT-PyQt-PySide-Custom-Widgets-0.6.6/Custom_Widgets/Qss/icons/original_svg/
+-rw-rw-rw-   0        0        0      276 2023-06-21 21:32:18.000000 QT-PyQt-PySide-Custom-Widgets-0.6.6/Custom_Widgets/Qss/icons/original_svg/activity.svg
+-rw-rw-rw-   0        0        0      356 2023-06-21 21:32:18.000000 QT-PyQt-PySide-Custom-Widgets-0.6.6/Custom_Widgets/Qss/icons/original_svg/airplay.svg
+-rw-rw-rw-   0        0        0      350 2023-06-21 21:32:18.000000 QT-PyQt-PySide-Custom-Widgets-0.6.6/Custom_Widgets/Qss/icons/original_svg/alert-circle.svg
+-rw-rw-rw-   0        0        0      410 2023-06-21 21:32:18.000000 QT-PyQt-PySide-Custom-Widgets-0.6.6/Custom_Widgets/Qss/icons/original_svg/alert-octagon.svg
+-rw-rw-rw-   0        0        0      418 2023-06-21 21:32:18.000000 QT-PyQt-PySide-Custom-Widgets-0.6.6/Custom_Widgets/Qss/icons/original_svg/alert-triangle.svg
+-rw-rw-rw-   0        0        0      392 2023-06-21 21:32:18.000000 QT-PyQt-PySide-Custom-Widgets-0.6.6/Custom_Widgets/Qss/icons/original_svg/align-center.svg
+-rw-rw-rw-   0        0        0      393 2023-06-21 21:32:18.000000 QT-PyQt-PySide-Custom-Widgets-0.6.6/Custom_Widgets/Qss/icons/original_svg/align-justify.svg
+-rw-rw-rw-   0        0        0      390 2023-06-21 21:32:18.000000 QT-PyQt-PySide-Custom-Widgets-0.6.6/Custom_Widgets/Qss/icons/original_svg/align-left.svg
+-rw-rw-rw-   0        0        0      391 2023-06-21 21:32:18.000000 QT-PyQt-PySide-Custom-Widgets-0.6.6/Custom_Widgets/Qss/icons/original_svg/align-right.svg
+-rw-rw-rw-   0        0        0      339 2023-06-21 21:32:18.000000 QT-PyQt-PySide-Custom-Widgets-0.6.6/Custom_Widgets/Qss/icons/original_svg/anchor.svg
+-rw-rw-rw-   0        0        0      562 2023-06-21 21:32:18.000000 QT-PyQt-PySide-Custom-Widgets-0.6.6/Custom_Widgets/Qss/icons/original_svg/aperture.svg
+-rw-rw-rw-   0        0        0      355 2023-06-21 21:32:18.000000 QT-PyQt-PySide-Custom-Widgets-0.6.6/Custom_Widgets/Qss/icons/original_svg/archive.svg
+-rw-rw-rw-   0        0        0      354 2023-06-21 21:32:18.000000 QT-PyQt-PySide-Custom-Widgets-0.6.6/Custom_Widgets/Qss/icons/original_svg/arrow-down-circle.svg
+-rw-rw-rw-   0        0        0      309 2023-06-21 21:32:18.000000 QT-PyQt-PySide-Custom-Widgets-0.6.6/Custom_Widgets/Qss/icons/original_svg/arrow-down-left.svg
+-rw-rw-rw-   0        0        0      311 2023-06-21 21:32:18.000000 QT-PyQt-PySide-Custom-Widgets-0.6.6/Custom_Widgets/Qss/icons/original_svg/arrow-down-right.svg
+-rw-rw-rw-   0        0        0      307 2023-06-21 21:32:18.000000 QT-PyQt-PySide-Custom-Widgets-0.6.6/Custom_Widgets/Qss/icons/original_svg/arrow-down.svg
+-rw-rw-rw-   0        0        0      353 2023-06-21 21:32:18.000000 QT-PyQt-PySide-Custom-Widgets-0.6.6/Custom_Widgets/Qss/icons/original_svg/arrow-left-circle.svg
+-rw-rw-rw-   0        0        0      306 2023-06-21 21:32:18.000000 QT-PyQt-PySide-Custom-Widgets-0.6.6/Custom_Widgets/Qss/icons/original_svg/arrow-left.svg
+-rw-rw-rw-   0        0        0      355 2023-06-21 21:32:18.000000 QT-PyQt-PySide-Custom-Widgets-0.6.6/Custom_Widgets/Qss/icons/original_svg/arrow-right-circle.svg
+-rw-rw-rw-   0        0        0      308 2023-06-21 21:32:18.000000 QT-PyQt-PySide-Custom-Widgets-0.6.6/Custom_Widgets/Qss/icons/original_svg/arrow-right.svg
+-rw-rw-rw-   0        0        0      351 2023-06-21 21:32:18.000000 QT-PyQt-PySide-Custom-Widgets-0.6.6/Custom_Widgets/Qss/icons/original_svg/arrow-up-circle.svg
+-rw-rw-rw-   0        0        0      306 2023-06-21 21:32:18.000000 QT-PyQt-PySide-Custom-Widgets-0.6.6/Custom_Widgets/Qss/icons/original_svg/arrow-up-left.svg
+-rw-rw-rw-   0        0        0      308 2023-06-21 21:32:18.000000 QT-PyQt-PySide-Custom-Widgets-0.6.6/Custom_Widgets/Qss/icons/original_svg/arrow-up-right.svg
+-rw-rw-rw-   0        0        0      304 2023-06-21 21:32:18.000000 QT-PyQt-PySide-Custom-Widgets-0.6.6/Custom_Widgets/Qss/icons/original_svg/arrow-up.svg
+-rw-rw-rw-   0        0        0     3022 2023-06-21 21:32:18.000000 QT-PyQt-PySide-Custom-Widgets-0.6.6/Custom_Widgets/Qss/icons/original_svg/arrow_down.svg
+-rw-rw-rw-   0        0        0     3023 2023-06-21 21:32:18.000000 QT-PyQt-PySide-Custom-Widgets-0.6.6/Custom_Widgets/Qss/icons/original_svg/arrow_left.svg
+-rw-rw-rw-   0        0        0     3026 2023-06-21 21:32:18.000000 QT-PyQt-PySide-Custom-Widgets-0.6.6/Custom_Widgets/Qss/icons/original_svg/arrow_right.svg
+-rw-rw-rw-   0        0        0     3021 2023-06-21 21:32:18.000000 QT-PyQt-PySide-Custom-Widgets-0.6.6/Custom_Widgets/Qss/icons/original_svg/arrow_up.svg
+-rw-rw-rw-   0        0        0      316 2023-06-21 21:32:18.000000 QT-PyQt-PySide-Custom-Widgets-0.6.6/Custom_Widgets/Qss/icons/original_svg/at-sign.svg
+-rw-rw-rw-   0        0        0      319 2023-06-21 21:32:18.000000 QT-PyQt-PySide-Custom-Widgets-0.6.6/Custom_Widgets/Qss/icons/original_svg/award.svg
+-rw-rw-rw-   0        0        0      349 2023-06-21 21:32:18.000000 QT-PyQt-PySide-Custom-Widgets-0.6.6/Custom_Widgets/Qss/icons/original_svg/bar-chart-2.svg
+-rw-rw-rw-   0        0        0      347 2023-06-21 21:32:18.000000 QT-PyQt-PySide-Custom-Widgets-0.6.6/Custom_Widgets/Qss/icons/original_svg/bar-chart.svg
+-rw-rw-rw-   0        0        0     7594 2023-06-21 21:32:18.000000 QT-PyQt-PySide-Custom-Widgets-0.6.6/Custom_Widgets/Qss/icons/original_svg/base_icon.svg
+-rw-rw-rw-   0        0        0    33666 2023-06-21 21:32:18.000000 QT-PyQt-PySide-Custom-Widgets-0.6.6/Custom_Widgets/Qss/icons/original_svg/base_palette.svg
+-rw-rw-rw-   0        0        0      421 2023-06-21 21:32:18.000000 QT-PyQt-PySide-Custom-Widgets-0.6.6/Custom_Widgets/Qss/icons/original_svg/battery-charging.svg
+-rw-rw-rw-   0        0        0      320 2023-06-21 21:32:18.000000 QT-PyQt-PySide-Custom-Widgets-0.6.6/Custom_Widgets/Qss/icons/original_svg/battery.svg
+-rw-rw-rw-   0        0        0      454 2023-06-21 21:32:18.000000 QT-PyQt-PySide-Custom-Widgets-0.6.6/Custom_Widgets/Qss/icons/original_svg/bell-off.svg
+-rw-rw-rw-   0        0        0      315 2023-06-21 21:32:18.000000 QT-PyQt-PySide-Custom-Widgets-0.6.6/Custom_Widgets/Qss/icons/original_svg/bell.svg
+-rw-rw-rw-   0        0        0      292 2023-06-21 21:32:18.000000 QT-PyQt-PySide-Custom-Widgets-0.6.6/Custom_Widgets/Qss/icons/original_svg/bluetooth.svg
+-rw-rw-rw-   0        0        0      321 2023-06-21 21:32:18.000000 QT-PyQt-PySide-Custom-Widgets-0.6.6/Custom_Widgets/Qss/icons/original_svg/bold.svg
+-rw-rw-rw-   0        0        0      333 2023-06-21 21:32:18.000000 QT-PyQt-PySide-Custom-Widgets-0.6.6/Custom_Widgets/Qss/icons/original_svg/book-open.svg
+-rw-rw-rw-   0        0        0      339 2023-06-21 21:32:18.000000 QT-PyQt-PySide-Custom-Widgets-0.6.6/Custom_Widgets/Qss/icons/original_svg/book.svg
+-rw-rw-rw-   0        0        0      281 2023-06-21 21:32:18.000000 QT-PyQt-PySide-Custom-Widgets-0.6.6/Custom_Widgets/Qss/icons/original_svg/bookmark.svg
+-rw-rw-rw-   0        0        0      456 2023-06-21 21:32:18.000000 QT-PyQt-PySide-Custom-Widgets-0.6.6/Custom_Widgets/Qss/icons/original_svg/box.svg
+-rw-rw-rw-   0        0        0     2755 2023-06-21 21:32:18.000000 QT-PyQt-PySide-Custom-Widgets-0.6.6/Custom_Widgets/Qss/icons/original_svg/branch_closed.svg
+-rw-rw-rw-   0        0        0     2902 2023-06-21 21:32:18.000000 QT-PyQt-PySide-Custom-Widgets-0.6.6/Custom_Widgets/Qss/icons/original_svg/branch_end.svg
+-rw-rw-rw-   0        0        0     3508 2023-06-21 21:32:18.000000 QT-PyQt-PySide-Custom-Widgets-0.6.6/Custom_Widgets/Qss/icons/original_svg/branch_line.svg
+-rw-rw-rw-   0        0        0     2678 2023-06-21 21:32:18.000000 QT-PyQt-PySide-Custom-Widgets-0.6.6/Custom_Widgets/Qss/icons/original_svg/branch_more.svg
+-rw-rw-rw-   0        0        0     2711 2023-06-21 21:32:18.000000 QT-PyQt-PySide-Custom-Widgets-0.6.6/Custom_Widgets/Qss/icons/original_svg/branch_open.svg
+-rw-rw-rw-   0        0        0      337 2023-06-21 21:32:18.000000 QT-PyQt-PySide-Custom-Widgets-0.6.6/Custom_Widgets/Qss/icons/original_svg/briefcase.svg
+-rw-rw-rw-   0        0        0      404 2023-06-21 21:32:18.000000 QT-PyQt-PySide-Custom-Widgets-0.6.6/Custom_Widgets/Qss/icons/original_svg/calendar.svg
+-rw-rw-rw-   0        0        0      379 2023-06-21 21:32:18.000000 QT-PyQt-PySide-Custom-Widgets-0.6.6/Custom_Widgets/Qss/icons/original_svg/camera-off.svg
+-rw-rw-rw-   0        0        0      350 2023-06-21 21:32:18.000000 QT-PyQt-PySide-Custom-Widgets-0.6.6/Custom_Widgets/Qss/icons/original_svg/camera.svg
+-rw-rw-rw-   0        0        0      381 2023-06-21 21:32:18.000000 QT-PyQt-PySide-Custom-Widgets-0.6.6/Custom_Widgets/Qss/icons/original_svg/cast.svg
+-rw-rw-rw-   0        0        0      322 2023-06-21 21:32:18.000000 QT-PyQt-PySide-Custom-Widgets-0.6.6/Custom_Widgets/Qss/icons/original_svg/check-circle.svg
+-rw-rw-rw-   0        0        0      339 2023-06-21 21:32:18.000000 QT-PyQt-PySide-Custom-Widgets-0.6.6/Custom_Widgets/Qss/icons/original_svg/check-square.svg
+-rw-rw-rw-   0        0        0      256 2023-06-21 21:32:18.000000 QT-PyQt-PySide-Custom-Widgets-0.6.6/Custom_Widgets/Qss/icons/original_svg/check.svg
+-rw-rw-rw-   0        0        0     2799 2023-06-21 21:32:18.000000 QT-PyQt-PySide-Custom-Widgets-0.6.6/Custom_Widgets/Qss/icons/original_svg/checkbox_checked.svg
+-rw-rw-rw-   0        0        0     2781 2023-06-21 21:32:18.000000 QT-PyQt-PySide-Custom-Widgets-0.6.6/Custom_Widgets/Qss/icons/original_svg/checkbox_indeterminate.svg
+-rw-rw-rw-   0        0        0     2598 2023-06-21 21:32:18.000000 QT-PyQt-PySide-Custom-Widgets-0.6.6/Custom_Widgets/Qss/icons/original_svg/checkbox_unchecked.svg
+-rw-rw-rw-   0        0        0      263 2023-06-21 21:32:18.000000 QT-PyQt-PySide-Custom-Widgets-0.6.6/Custom_Widgets/Qss/icons/original_svg/chevron-down.svg
+-rw-rw-rw-   0        0        0      264 2023-06-21 21:32:18.000000 QT-PyQt-PySide-Custom-Widgets-0.6.6/Custom_Widgets/Qss/icons/original_svg/chevron-left.svg
+-rw-rw-rw-   0        0        0      264 2023-06-21 21:32:18.000000 QT-PyQt-PySide-Custom-Widgets-0.6.6/Custom_Widgets/Qss/icons/original_svg/chevron-right.svg
+-rw-rw-rw-   0        0        0      262 2023-06-21 21:32:18.000000 QT-PyQt-PySide-Custom-Widgets-0.6.6/Custom_Widgets/Qss/icons/original_svg/chevron-up.svg
+-rw-rw-rw-   0        0        0      311 2023-06-21 21:32:18.000000 QT-PyQt-PySide-Custom-Widgets-0.6.6/Custom_Widgets/Qss/icons/original_svg/chevrons-down.svg
+-rw-rw-rw-   0        0        0      312 2023-06-21 21:32:18.000000 QT-PyQt-PySide-Custom-Widgets-0.6.6/Custom_Widgets/Qss/icons/original_svg/chevrons-left.svg
+-rw-rw-rw-   0        0        0      312 2023-06-21 21:32:18.000000 QT-PyQt-PySide-Custom-Widgets-0.6.6/Custom_Widgets/Qss/icons/original_svg/chevrons-right.svg
+-rw-rw-rw-   0        0        0      310 2023-06-21 21:32:18.000000 QT-PyQt-PySide-Custom-Widgets-0.6.6/Custom_Widgets/Qss/icons/original_svg/chevrons-up.svg
+-rw-rw-rw-   0        0        0      442 2023-06-21 21:32:18.000000 QT-PyQt-PySide-Custom-Widgets-0.6.6/Custom_Widgets/Qss/icons/original_svg/chrome.svg
+-rw-rw-rw-   0        0        0      252 2023-06-21 21:32:18.000000 QT-PyQt-PySide-Custom-Widgets-0.6.6/Custom_Widgets/Qss/icons/original_svg/circle.svg
+-rw-rw-rw-   0        0        0      365 2023-06-21 21:32:18.000000 QT-PyQt-PySide-Custom-Widgets-0.6.6/Custom_Widgets/Qss/icons/original_svg/clipboard.svg
+-rw-rw-rw-   0        0        0      298 2023-06-21 21:32:18.000000 QT-PyQt-PySide-Custom-Widgets-0.6.6/Custom_Widgets/Qss/icons/original_svg/clock.svg
+-rw-rw-rw-   0        0        0      551 2023-06-21 21:32:18.000000 QT-PyQt-PySide-Custom-Widgets-0.6.6/Custom_Widgets/Qss/icons/original_svg/cloud-drizzle.svg
+-rw-rw-rw-   0        0        0      339 2023-06-21 21:32:18.000000 QT-PyQt-PySide-Custom-Widgets-0.6.6/Custom_Widgets/Qss/icons/original_svg/cloud-lightning.svg
+-rw-rw-rw-   0        0        0      365 2023-06-21 21:32:18.000000 QT-PyQt-PySide-Custom-Widgets-0.6.6/Custom_Widgets/Qss/icons/original_svg/cloud-off.svg
+-rw-rw-rw-   0        0        0      415 2023-06-21 21:32:18.000000 QT-PyQt-PySide-Custom-Widgets-0.6.6/Custom_Widgets/Qss/icons/original_svg/cloud-rain.svg
+-rw-rw-rw-   0        0        0      566 2023-06-21 21:32:18.000000 QT-PyQt-PySide-Custom-Widgets-0.6.6/Custom_Widgets/Qss/icons/original_svg/cloud-snow.svg
+-rw-rw-rw-   0        0        0      274 2023-06-21 21:32:18.000000 QT-PyQt-PySide-Custom-Widgets-0.6.6/Custom_Widgets/Qss/icons/original_svg/cloud.svg
+-rw-rw-rw-   0        0        0      301 2023-06-21 21:32:18.000000 QT-PyQt-PySide-Custom-Widgets-0.6.6/Custom_Widgets/Qss/icons/original_svg/code.svg
+-rw-rw-rw-   0        0        0      480 2023-06-21 21:32:18.000000 QT-PyQt-PySide-Custom-Widgets-0.6.6/Custom_Widgets/Qss/icons/original_svg/codepen.svg
+-rw-rw-rw-   0        0        0      632 2023-06-21 21:32:18.000000 QT-PyQt-PySide-Custom-Widgets-0.6.6/Custom_Widgets/Qss/icons/original_svg/codesandbox.svg
+-rw-rw-rw-   0        0        0      441 2023-06-21 21:32:18.000000 QT-PyQt-PySide-Custom-Widgets-0.6.6/Custom_Widgets/Qss/icons/original_svg/coffee.svg
+-rw-rw-rw-   0        0        0      320 2023-06-21 21:32:18.000000 QT-PyQt-PySide-Custom-Widgets-0.6.6/Custom_Widgets/Qss/icons/original_svg/columns.svg
+-rw-rw-rw-   0        0        0      415 2023-06-21 21:32:18.000000 QT-PyQt-PySide-Custom-Widgets-0.6.6/Custom_Widgets/Qss/icons/original_svg/command.svg
+-rw-rw-rw-   0        0        0      336 2023-06-21 21:32:18.000000 QT-PyQt-PySide-Custom-Widgets-0.6.6/Custom_Widgets/Qss/icons/original_svg/compass.svg
+-rw-rw-rw-   0        0        0      345 2023-06-21 21:32:18.000000 QT-PyQt-PySide-Custom-Widgets-0.6.6/Custom_Widgets/Qss/icons/original_svg/copy.svg
+-rw-rw-rw-   0        0        0      308 2023-06-21 21:32:18.000000 QT-PyQt-PySide-Custom-Widgets-0.6.6/Custom_Widgets/Qss/icons/original_svg/corner-down-left.svg
+-rw-rw-rw-   0        0        0      312 2023-06-21 21:32:18.000000 QT-PyQt-PySide-Custom-Widgets-0.6.6/Custom_Widgets/Qss/icons/original_svg/corner-down-right.svg
+-rw-rw-rw-   0        0        0      311 2023-06-21 21:32:18.000000 QT-PyQt-PySide-Custom-Widgets-0.6.6/Custom_Widgets/Qss/icons/original_svg/corner-left-down.svg
+-rw-rw-rw-   0        0        0      306 2023-06-21 21:32:18.000000 QT-PyQt-PySide-Custom-Widgets-0.6.6/Custom_Widgets/Qss/icons/original_svg/corner-left-up.svg
+-rw-rw-rw-   0        0        0      312 2023-06-21 21:32:18.000000 QT-PyQt-PySide-Custom-Widgets-0.6.6/Custom_Widgets/Qss/icons/original_svg/corner-right-down.svg
+-rw-rw-rw-   0        0        0      307 2023-06-21 21:32:18.000000 QT-PyQt-PySide-Custom-Widgets-0.6.6/Custom_Widgets/Qss/icons/original_svg/corner-right-up.svg
+-rw-rw-rw-   0        0        0      306 2023-06-21 21:32:18.000000 QT-PyQt-PySide-Custom-Widgets-0.6.6/Custom_Widgets/Qss/icons/original_svg/corner-up-left.svg
+-rw-rw-rw-   0        0        0      310 2023-06-21 21:32:18.000000 QT-PyQt-PySide-Custom-Widgets-0.6.6/Custom_Widgets/Qss/icons/original_svg/corner-up-right.svg
+-rw-rw-rw-   0        0        0      661 2023-06-21 21:32:18.000000 QT-PyQt-PySide-Custom-Widgets-0.6.6/Custom_Widgets/Qss/icons/original_svg/cpu.svg
+-rw-rw-rw-   0        0        0      323 2023-06-21 21:32:18.000000 QT-PyQt-PySide-Custom-Widgets-0.6.6/Custom_Widgets/Qss/icons/original_svg/credit-card.svg
+-rw-rw-rw-   0        0        0      304 2023-06-21 21:32:18.000000 QT-PyQt-PySide-Custom-Widgets-0.6.6/Custom_Widgets/Qss/icons/original_svg/crop.svg
+-rw-rw-rw-   0        0        0      431 2023-06-21 21:32:18.000000 QT-PyQt-PySide-Custom-Widgets-0.6.6/Custom_Widgets/Qss/icons/original_svg/crosshair.svg
+-rw-rw-rw-   0        0        0      366 2023-06-21 21:32:18.000000 QT-PyQt-PySide-Custom-Widgets-0.6.6/Custom_Widgets/Qss/icons/original_svg/database.svg
+-rw-rw-rw-   0        0        0      368 2023-06-21 21:32:18.000000 QT-PyQt-PySide-Custom-Widgets-0.6.6/Custom_Widgets/Qss/icons/original_svg/delete.svg
+-rw-rw-rw-   0        0        0      289 2023-06-21 21:32:18.000000 QT-PyQt-PySide-Custom-Widgets-0.6.6/Custom_Widgets/Qss/icons/original_svg/disc.svg
+-rw-rw-rw-   0        0        0      391 2023-06-21 21:32:18.000000 QT-PyQt-PySide-Custom-Widgets-0.6.6/Custom_Widgets/Qss/icons/original_svg/divide-circle.svg
+-rw-rw-rw-   0        0        0      413 2023-06-21 21:32:18.000000 QT-PyQt-PySide-Custom-Widgets-0.6.6/Custom_Widgets/Qss/icons/original_svg/divide-square.svg
+-rw-rw-rw-   0        0        0      333 2023-06-21 21:32:18.000000 QT-PyQt-PySide-Custom-Widgets-0.6.6/Custom_Widgets/Qss/icons/original_svg/divide.svg
+-rw-rw-rw-   0        0        0      328 2023-06-21 21:32:18.000000 QT-PyQt-PySide-Custom-Widgets-0.6.6/Custom_Widgets/Qss/icons/original_svg/dollar-sign.svg
+-rw-rw-rw-   0        0        0      381 2023-06-21 21:32:18.000000 QT-PyQt-PySide-Custom-Widgets-0.6.6/Custom_Widgets/Qss/icons/original_svg/download-cloud.svg
+-rw-rw-rw-   0        0        0      364 2023-06-21 21:32:18.000000 QT-PyQt-PySide-Custom-Widgets-0.6.6/Custom_Widgets/Qss/icons/original_svg/download.svg
+-rw-rw-rw-   0        0        0      418 2023-06-21 21:32:18.000000 QT-PyQt-PySide-Custom-Widgets-0.6.6/Custom_Widgets/Qss/icons/original_svg/dribbble.svg
+-rw-rw-rw-   0        0        0      268 2023-06-21 21:32:18.000000 QT-PyQt-PySide-Custom-Widgets-0.6.6/Custom_Widgets/Qss/icons/original_svg/droplet.svg
+-rw-rw-rw-   0        0        0      285 2023-06-21 21:32:18.000000 QT-PyQt-PySide-Custom-Widgets-0.6.6/Custom_Widgets/Qss/icons/original_svg/edit-2.svg
+-rw-rw-rw-   0        0        0      311 2023-06-21 21:32:18.000000 QT-PyQt-PySide-Custom-Widgets-0.6.6/Custom_Widgets/Qss/icons/original_svg/edit-3.svg
+-rw-rw-rw-   0        0        0      359 2023-06-21 21:32:18.000000 QT-PyQt-PySide-Custom-Widgets-0.6.6/Custom_Widgets/Qss/icons/original_svg/edit.svg
+-rw-rw-rw-   0        0        0      382 2023-06-21 21:32:18.000000 QT-PyQt-PySide-Custom-Widgets-0.6.6/Custom_Widgets/Qss/icons/original_svg/external-link.svg
+-rw-rw-rw-   0        0        0      454 2023-06-21 21:32:18.000000 QT-PyQt-PySide-Custom-Widgets-0.6.6/Custom_Widgets/Qss/icons/original_svg/eye-off.svg
+-rw-rw-rw-   0        0        0      310 2023-06-21 21:32:18.000000 QT-PyQt-PySide-Custom-Widgets-0.6.6/Custom_Widgets/Qss/icons/original_svg/eye.svg
+-rw-rw-rw-   0        0        0      297 2023-06-21 21:32:18.000000 QT-PyQt-PySide-Custom-Widgets-0.6.6/Custom_Widgets/Qss/icons/original_svg/facebook.svg
+-rw-rw-rw-   0        0        0      317 2023-06-21 21:32:18.000000 QT-PyQt-PySide-Custom-Widgets-0.6.6/Custom_Widgets/Qss/icons/original_svg/fast-forward.svg
+-rw-rw-rw-   0        0        0      367 2023-06-21 21:32:18.000000 QT-PyQt-PySide-Custom-Widgets-0.6.6/Custom_Widgets/Qss/icons/original_svg/feather.svg
+-rw-rw-rw-   0        0        0      547 2023-06-21 21:32:18.000000 QT-PyQt-PySide-Custom-Widgets-0.6.6/Custom_Widgets/Qss/icons/original_svg/figma.svg
+-rw-rw-rw-   0        0        0      381 2023-06-21 21:32:18.000000 QT-PyQt-PySide-Custom-Widgets-0.6.6/Custom_Widgets/Qss/icons/original_svg/file-minus.svg
+-rw-rw-rw-   0        0        0      425 2023-06-21 21:32:18.000000 QT-PyQt-PySide-Custom-Widgets-0.6.6/Custom_Widgets/Qss/icons/original_svg/file-plus.svg
+-rw-rw-rw-   0        0        0      467 2023-06-21 21:32:18.000000 QT-PyQt-PySide-Custom-Widgets-0.6.6/Custom_Widgets/Qss/icons/original_svg/file-text.svg
+-rw-rw-rw-   0        0        0      331 2023-06-21 21:32:18.000000 QT-PyQt-PySide-Custom-Widgets-0.6.6/Custom_Widgets/Qss/icons/original_svg/file.svg
+-rw-rw-rw-   0        0        0      580 2023-06-21 21:32:18.000000 QT-PyQt-PySide-Custom-Widgets-0.6.6/Custom_Widgets/Qss/icons/original_svg/film.svg
+-rw-rw-rw-   0        0        0      284 2023-06-21 21:32:18.000000 QT-PyQt-PySide-Custom-Widgets-0.6.6/Custom_Widgets/Qss/icons/original_svg/filter.svg
+-rw-rw-rw-   0        0        0      328 2023-06-21 21:32:18.000000 QT-PyQt-PySide-Custom-Widgets-0.6.6/Custom_Widgets/Qss/icons/original_svg/flag.svg
+-rw-rw-rw-   0        0        0      355 2023-06-21 21:32:18.000000 QT-PyQt-PySide-Custom-Widgets-0.6.6/Custom_Widgets/Qss/icons/original_svg/folder-minus.svg
+-rw-rw-rw-   0        0        0      399 2023-06-21 21:32:18.000000 QT-PyQt-PySide-Custom-Widgets-0.6.6/Custom_Widgets/Qss/icons/original_svg/folder-plus.svg
+-rw-rw-rw-   0        0        0      305 2023-06-21 21:32:18.000000 QT-PyQt-PySide-Custom-Widgets-0.6.6/Custom_Widgets/Qss/icons/original_svg/folder.svg
+-rw-rw-rw-   0        0        0      272 2023-06-21 21:32:18.000000 QT-PyQt-PySide-Custom-Widgets-0.6.6/Custom_Widgets/Qss/icons/original_svg/framer.svg
+-rw-rw-rw-   0        0        0      384 2023-06-21 21:32:18.000000 QT-PyQt-PySide-Custom-Widgets-0.6.6/Custom_Widgets/Qss/icons/original_svg/frown.svg
+-rw-rw-rw-   0        0        0      475 2023-06-21 21:32:18.000000 QT-PyQt-PySide-Custom-Widgets-0.6.6/Custom_Widgets/Qss/icons/original_svg/gift.svg
+-rw-rw-rw-   0        0        0      371 2023-06-21 21:32:18.000000 QT-PyQt-PySide-Custom-Widgets-0.6.6/Custom_Widgets/Qss/icons/original_svg/git-branch.svg
+-rw-rw-rw-   0        0        0      352 2023-06-21 21:32:18.000000 QT-PyQt-PySide-Custom-Widgets-0.6.6/Custom_Widgets/Qss/icons/original_svg/git-commit.svg
+-rw-rw-rw-   0        0        0      330 2023-06-21 21:32:18.000000 QT-PyQt-PySide-Custom-Widgets-0.6.6/Custom_Widgets/Qss/icons/original_svg/git-merge.svg
+-rw-rw-rw-   0        0        0      381 2023-06-21 21:32:18.000000 QT-PyQt-PySide-Custom-Widgets-0.6.6/Custom_Widgets/Qss/icons/original_svg/git-pull-request.svg
+-rw-rw-rw-   0        0        0      521 2023-06-21 21:32:18.000000 QT-PyQt-PySide-Custom-Widgets-0.6.6/Custom_Widgets/Qss/icons/original_svg/github.svg
+-rw-rw-rw-   0        0        0      484 2023-06-21 21:32:18.000000 QT-PyQt-PySide-Custom-Widgets-0.6.6/Custom_Widgets/Qss/icons/original_svg/gitlab.svg
+-rw-rw-rw-   0        0        0      403 2023-06-21 21:32:18.000000 QT-PyQt-PySide-Custom-Widgets-0.6.6/Custom_Widgets/Qss/icons/original_svg/globe.svg
+-rw-rw-rw-   0        0        0      398 2023-06-21 21:32:18.000000 QT-PyQt-PySide-Custom-Widgets-0.6.6/Custom_Widgets/Qss/icons/original_svg/grid.svg
+-rw-rw-rw-   0        0        0      478 2023-06-21 21:32:18.000000 QT-PyQt-PySide-Custom-Widgets-0.6.6/Custom_Widgets/Qss/icons/original_svg/hard-drive.svg
+-rw-rw-rw-   0        0        0      383 2023-06-21 21:32:18.000000 QT-PyQt-PySide-Custom-Widgets-0.6.6/Custom_Widgets/Qss/icons/original_svg/hash.svg
+-rw-rw-rw-   0        0        0      389 2023-06-21 21:32:18.000000 QT-PyQt-PySide-Custom-Widgets-0.6.6/Custom_Widgets/Qss/icons/original_svg/headphones.svg
+-rw-rw-rw-   0        0        0      365 2023-06-21 21:32:18.000000 QT-PyQt-PySide-Custom-Widgets-0.6.6/Custom_Widgets/Qss/icons/original_svg/heart.svg
+-rw-rw-rw-   0        0        0      359 2023-06-21 21:32:18.000000 QT-PyQt-PySide-Custom-Widgets-0.6.6/Custom_Widgets/Qss/icons/original_svg/help-circle.svg
+-rw-rw-rw-   0        0        0      352 2023-06-21 21:32:18.000000 QT-PyQt-PySide-Custom-Widgets-0.6.6/Custom_Widgets/Qss/icons/original_svg/hexagon.svg
+-rw-rw-rw-   0        0        0      326 2023-06-21 21:32:18.000000 QT-PyQt-PySide-Custom-Widgets-0.6.6/Custom_Widgets/Qss/icons/original_svg/home.svg
+-rw-rw-rw-   0        0        0      363 2023-06-21 21:32:18.000000 QT-PyQt-PySide-Custom-Widgets-0.6.6/Custom_Widgets/Qss/icons/original_svg/image.svg
+-rw-rw-rw-   0        0        0      399 2023-06-21 21:32:18.000000 QT-PyQt-PySide-Custom-Widgets-0.6.6/Custom_Widgets/Qss/icons/original_svg/inbox.svg
+-rw-rw-rw-   0        0        0      341 2023-06-21 21:32:18.000000 QT-PyQt-PySide-Custom-Widgets-0.6.6/Custom_Widgets/Qss/icons/original_svg/info.svg
+-rw-rw-rw-   0        0        0      394 2023-06-21 21:32:18.000000 QT-PyQt-PySide-Custom-Widgets-0.6.6/Custom_Widgets/Qss/icons/original_svg/instagram.svg
+-rw-rw-rw-   0        0        0      342 2023-06-21 21:32:18.000000 QT-PyQt-PySide-Custom-Widgets-0.6.6/Custom_Widgets/Qss/icons/original_svg/italic.svg
+-rw-rw-rw-   0        0        0      346 2023-06-21 21:32:18.000000 QT-PyQt-PySide-Custom-Widgets-0.6.6/Custom_Widgets/Qss/icons/original_svg/key.svg
+-rw-rw-rw-   0        0        0      359 2023-06-21 21:32:18.000000 QT-PyQt-PySide-Custom-Widgets-0.6.6/Custom_Widgets/Qss/icons/original_svg/layers.svg
+-rw-rw-rw-   0        0        0      358 2023-06-21 21:32:18.000000 QT-PyQt-PySide-Custom-Widgets-0.6.6/Custom_Widgets/Qss/icons/original_svg/layout.svg
+-rw-rw-rw-   0        0        0      569 2023-06-21 21:32:18.000000 QT-PyQt-PySide-Custom-Widgets-0.6.6/Custom_Widgets/Qss/icons/original_svg/life-buoy.svg
+-rw-rw-rw-   0        0        0     2445 2023-06-21 21:32:18.000000 QT-PyQt-PySide-Custom-Widgets-0.6.6/Custom_Widgets/Qss/icons/original_svg/line_horizontal.svg
+-rw-rw-rw-   0        0        0     2454 2023-06-21 21:32:18.000000 QT-PyQt-PySide-Custom-Widgets-0.6.6/Custom_Widgets/Qss/icons/original_svg/line_vertical.svg
+-rw-rw-rw-   0        0        0      349 2023-06-21 21:32:18.000000 QT-PyQt-PySide-Custom-Widgets-0.6.6/Custom_Widgets/Qss/icons/original_svg/link-2.svg
+-rw-rw-rw-   0        0        0      365 2023-06-21 21:32:18.000000 QT-PyQt-PySide-Custom-Widgets-0.6.6/Custom_Widgets/Qss/icons/original_svg/link.svg
+-rw-rw-rw-   0        0        0      394 2023-06-21 21:32:18.000000 QT-PyQt-PySide-Custom-Widgets-0.6.6/Custom_Widgets/Qss/icons/original_svg/linkedin.svg
+-rw-rw-rw-   0        0        0      476 2023-06-21 21:32:18.000000 QT-PyQt-PySide-Custom-Widgets-0.6.6/Custom_Widgets/Qss/icons/original_svg/list.svg
+-rw-rw-rw-   0        0        0      608 2023-06-21 21:32:18.000000 QT-PyQt-PySide-Custom-Widgets-0.6.6/Custom_Widgets/Qss/icons/original_svg/loader.svg
+-rw-rw-rw-   0        0        0      315 2023-06-21 21:32:18.000000 QT-PyQt-PySide-Custom-Widgets-0.6.6/Custom_Widgets/Qss/icons/original_svg/lock.svg
+-rw-rw-rw-   0        0        0      362 2023-06-21 21:32:18.000000 QT-PyQt-PySide-Custom-Widgets-0.6.6/Custom_Widgets/Qss/icons/original_svg/log-in.svg
+-rw-rw-rw-   0        0        0      361 2023-06-21 21:32:18.000000 QT-PyQt-PySide-Custom-Widgets-0.6.6/Custom_Widgets/Qss/icons/original_svg/log-out.svg
+-rw-rw-rw-   0        0        0      348 2023-06-21 21:32:18.000000 QT-PyQt-PySide-Custom-Widgets-0.6.6/Custom_Widgets/Qss/icons/original_svg/mail.svg
+-rw-rw-rw-   0        0        0      316 2023-06-21 21:32:18.000000 QT-PyQt-PySide-Custom-Widgets-0.6.6/Custom_Widgets/Qss/icons/original_svg/map-pin.svg
+-rw-rw-rw-   0        0        0      367 2023-06-21 21:32:18.000000 QT-PyQt-PySide-Custom-Widgets-0.6.6/Custom_Widgets/Qss/icons/original_svg/map.svg
+-rw-rw-rw-   0        0        0      394 2023-06-21 21:32:18.000000 QT-PyQt-PySide-Custom-Widgets-0.6.6/Custom_Widgets/Qss/icons/original_svg/maximize-2.svg
+-rw-rw-rw-   0        0        0      325 2023-06-21 21:32:18.000000 QT-PyQt-PySide-Custom-Widgets-0.6.6/Custom_Widgets/Qss/icons/original_svg/maximize.svg
+-rw-rw-rw-   0        0        0      383 2023-06-21 21:32:18.000000 QT-PyQt-PySide-Custom-Widgets-0.6.6/Custom_Widgets/Qss/icons/original_svg/meh.svg
+-rw-rw-rw-   0        0        0      340 2023-06-21 21:32:18.000000 QT-PyQt-PySide-Custom-Widgets-0.6.6/Custom_Widgets/Qss/icons/original_svg/menu.svg
+-rw-rw-rw-   0        0        0      422 2023-06-21 21:32:18.000000 QT-PyQt-PySide-Custom-Widgets-0.6.6/Custom_Widgets/Qss/icons/original_svg/message-circle.svg
+-rw-rw-rw-   0        0        0      299 2023-06-21 21:32:18.000000 QT-PyQt-PySide-Custom-Widgets-0.6.6/Custom_Widgets/Qss/icons/original_svg/message-square.svg
+-rw-rw-rw-   0        0        0      488 2023-06-21 21:32:18.000000 QT-PyQt-PySide-Custom-Widgets-0.6.6/Custom_Widgets/Qss/icons/original_svg/mic-off.svg
+-rw-rw-rw-   0        0        0      412 2023-06-21 21:32:18.000000 QT-PyQt-PySide-Custom-Widgets-0.6.6/Custom_Widgets/Qss/icons/original_svg/mic.svg
+-rw-rw-rw-   0        0        0      398 2023-06-21 21:32:18.000000 QT-PyQt-PySide-Custom-Widgets-0.6.6/Custom_Widgets/Qss/icons/original_svg/minimize-2.svg
+-rw-rw-rw-   0        0        0      325 2023-06-21 21:32:18.000000 QT-PyQt-PySide-Custom-Widgets-0.6.6/Custom_Widgets/Qss/icons/original_svg/minimize.svg
+-rw-rw-rw-   0        0        0      302 2023-06-21 21:32:18.000000 QT-PyQt-PySide-Custom-Widgets-0.6.6/Custom_Widgets/Qss/icons/original_svg/minus-circle.svg
+-rw-rw-rw-   0        0        0      324 2023-06-21 21:32:18.000000 QT-PyQt-PySide-Custom-Widgets-0.6.6/Custom_Widgets/Qss/icons/original_svg/minus-square.svg
+-rw-rw-rw-   0        0        0      255 2023-06-21 21:32:18.000000 QT-PyQt-PySide-Custom-Widgets-0.6.6/Custom_Widgets/Qss/icons/original_svg/minus.svg
+-rw-rw-rw-   0        0        0      364 2023-06-21 21:32:18.000000 QT-PyQt-PySide-Custom-Widgets-0.6.6/Custom_Widgets/Qss/icons/original_svg/monitor.svg
+-rw-rw-rw-   0        0        0      275 2023-06-21 21:32:18.000000 QT-PyQt-PySide-Custom-Widgets-0.6.6/Custom_Widgets/Qss/icons/original_svg/moon.svg
+-rw-rw-rw-   0        0        0      337 2023-06-21 21:32:18.000000 QT-PyQt-PySide-Custom-Widgets-0.6.6/Custom_Widgets/Qss/icons/original_svg/more-horizontal.svg
+-rw-rw-rw-   0        0        0      335 2023-06-21 21:32:18.000000 QT-PyQt-PySide-Custom-Widgets-0.6.6/Custom_Widgets/Qss/icons/original_svg/more-vertical.svg
+-rw-rw-rw-   0        0        0      305 2023-06-21 21:32:18.000000 QT-PyQt-PySide-Custom-Widgets-0.6.6/Custom_Widgets/Qss/icons/original_svg/mouse-pointer.svg
+-rw-rw-rw-   0        0        0      480 2023-06-21 21:32:18.000000 QT-PyQt-PySide-Custom-Widgets-0.6.6/Custom_Widgets/Qss/icons/original_svg/move.svg
+-rw-rw-rw-   0        0        0      321 2023-06-21 21:32:18.000000 QT-PyQt-PySide-Custom-Widgets-0.6.6/Custom_Widgets/Qss/icons/original_svg/music.svg
+-rw-rw-rw-   0        0        0      273 2023-06-21 21:32:18.000000 QT-PyQt-PySide-Custom-Widgets-0.6.6/Custom_Widgets/Qss/icons/original_svg/navigation-2.svg
+-rw-rw-rw-   0        0        0      271 2023-06-21 21:32:18.000000 QT-PyQt-PySide-Custom-Widgets-0.6.6/Custom_Widgets/Qss/icons/original_svg/navigation.svg
+-rw-rw-rw-   0        0        0      312 2023-06-21 21:32:18.000000 QT-PyQt-PySide-Custom-Widgets-0.6.6/Custom_Widgets/Qss/icons/original_svg/octagon.svg
+-rw-rw-rw-   0        0        0      511 2023-06-21 21:32:18.000000 QT-PyQt-PySide-Custom-Widgets-0.6.6/Custom_Widgets/Qss/icons/original_svg/package.svg
+-rw-rw-rw-   0        0        0      346 2023-06-21 21:32:18.000000 QT-PyQt-PySide-Custom-Widgets-0.6.6/Custom_Widgets/Qss/icons/original_svg/paperclip.svg
+-rw-rw-rw-   0        0        0      346 2023-06-21 21:32:18.000000 QT-PyQt-PySide-Custom-Widgets-0.6.6/Custom_Widgets/Qss/icons/original_svg/pause-circle.svg
+-rw-rw-rw-   0        0        0      306 2023-06-21 21:32:18.000000 QT-PyQt-PySide-Custom-Widgets-0.6.6/Custom_Widgets/Qss/icons/original_svg/pause.svg
+-rw-rw-rw-   0        0        0      385 2023-06-21 21:32:18.000000 QT-PyQt-PySide-Custom-Widgets-0.6.6/Custom_Widgets/Qss/icons/original_svg/pen-tool.svg
+-rw-rw-rw-   0        0        0      344 2023-06-21 21:32:18.000000 QT-PyQt-PySide-Custom-Widgets-0.6.6/Custom_Widgets/Qss/icons/original_svg/percent.svg
+-rw-rw-rw-   0        0        0      570 2023-06-21 21:32:18.000000 QT-PyQt-PySide-Custom-Widgets-0.6.6/Custom_Widgets/Qss/icons/original_svg/phone-call.svg
+-rw-rw-rw-   0        0        0      612 2023-06-21 21:32:18.000000 QT-PyQt-PySide-Custom-Widgets-0.6.6/Custom_Widgets/Qss/icons/original_svg/phone-forwarded.svg
+-rw-rw-rw-   0        0        0      611 2023-06-21 21:32:18.000000 QT-PyQt-PySide-Custom-Widgets-0.6.6/Custom_Widgets/Qss/icons/original_svg/phone-incoming.svg
+-rw-rw-rw-   0        0        0      607 2023-06-21 21:32:18.000000 QT-PyQt-PySide-Custom-Widgets-0.6.6/Custom_Widgets/Qss/icons/original_svg/phone-missed.svg
+-rw-rw-rw-   0        0        0      585 2023-06-21 21:32:18.000000 QT-PyQt-PySide-Custom-Widgets-0.6.6/Custom_Widgets/Qss/icons/original_svg/phone-off.svg
+-rw-rw-rw-   0        0        0      611 2023-06-21 21:32:18.000000 QT-PyQt-PySide-Custom-Widgets-0.6.6/Custom_Widgets/Qss/icons/original_svg/phone-outgoing.svg
+-rw-rw-rw-   0        0        0      514 2023-06-21 21:32:18.000000 QT-PyQt-PySide-Custom-Widgets-0.6.6/Custom_Widgets/Qss/icons/original_svg/phone.svg
+-rw-rw-rw-   0        0        0      309 2023-06-21 21:32:18.000000 QT-PyQt-PySide-Custom-Widgets-0.6.6/Custom_Widgets/Qss/icons/original_svg/pie-chart.svg
+-rw-rw-rw-   0        0        0      307 2023-06-21 21:32:18.000000 QT-PyQt-PySide-Custom-Widgets-0.6.6/Custom_Widgets/Qss/icons/original_svg/play-circle.svg
+-rw-rw-rw-   0        0        0      257 2023-06-21 21:32:18.000000 QT-PyQt-PySide-Custom-Widgets-0.6.6/Custom_Widgets/Qss/icons/original_svg/play.svg
+-rw-rw-rw-   0        0        0      345 2023-06-21 21:32:18.000000 QT-PyQt-PySide-Custom-Widgets-0.6.6/Custom_Widgets/Qss/icons/original_svg/plus-circle.svg
+-rw-rw-rw-   0        0        0      367 2023-06-21 21:32:18.000000 QT-PyQt-PySide-Custom-Widgets-0.6.6/Custom_Widgets/Qss/icons/original_svg/plus-square.svg
+-rw-rw-rw-   0        0        0      298 2023-06-21 21:32:18.000000 QT-PyQt-PySide-Custom-Widgets-0.6.6/Custom_Widgets/Qss/icons/original_svg/plus.svg
+-rw-rw-rw-   0        0        0      352 2023-06-21 21:32:18.000000 QT-PyQt-PySide-Custom-Widgets-0.6.6/Custom_Widgets/Qss/icons/original_svg/pocket.svg
+-rw-rw-rw-   0        0        0      302 2023-06-21 21:32:18.000000 QT-PyQt-PySide-Custom-Widgets-0.6.6/Custom_Widgets/Qss/icons/original_svg/power.svg
+-rw-rw-rw-   0        0        0      401 2023-06-21 21:32:18.000000 QT-PyQt-PySide-Custom-Widgets-0.6.6/Custom_Widgets/Qss/icons/original_svg/printer.svg
+-rw-rw-rw-   0        0        0      383 2023-06-21 21:32:18.000000 QT-PyQt-PySide-Custom-Widgets-0.6.6/Custom_Widgets/Qss/icons/original_svg/radio.svg
+-rw-rw-rw-   0        0        0     2714 2023-06-21 21:32:18.000000 QT-PyQt-PySide-Custom-Widgets-0.6.6/Custom_Widgets/Qss/icons/original_svg/radio_checked.svg
+-rw-rw-rw-   0        0        0     2419 2023-06-21 21:32:18.000000 QT-PyQt-PySide-Custom-Widgets-0.6.6/Custom_Widgets/Qss/icons/original_svg/radio_unchecked.svg
+-rw-rw-rw-   0        0        0      394 2023-06-21 21:32:18.000000 QT-PyQt-PySide-Custom-Widgets-0.6.6/Custom_Widgets/Qss/icons/original_svg/refresh-ccw.svg
+-rw-rw-rw-   0        0        0      394 2023-06-21 21:32:18.000000 QT-PyQt-PySide-Custom-Widgets-0.6.6/Custom_Widgets/Qss/icons/original_svg/refresh-cw.svg
+-rw-rw-rw-   0        0        0      386 2023-06-21 21:32:18.000000 QT-PyQt-PySide-Custom-Widgets-0.6.6/Custom_Widgets/Qss/icons/original_svg/repeat.svg
+-rw-rw-rw-   0        0        0      313 2023-06-21 21:32:18.000000 QT-PyQt-PySide-Custom-Widgets-0.6.6/Custom_Widgets/Qss/icons/original_svg/rewind.svg
+-rw-rw-rw-   0        0        0      311 2023-06-21 21:32:18.000000 QT-PyQt-PySide-Custom-Widgets-0.6.6/Custom_Widgets/Qss/icons/original_svg/rotate-ccw.svg
+-rw-rw-rw-   0        0        0      315 2023-06-21 21:32:18.000000 QT-PyQt-PySide-Custom-Widgets-0.6.6/Custom_Widgets/Qss/icons/original_svg/rotate-cw.svg
+-rw-rw-rw-   0        0        0      324 2023-06-21 21:32:18.000000 QT-PyQt-PySide-Custom-Widgets-0.6.6/Custom_Widgets/Qss/icons/original_svg/rss.svg
+-rw-rw-rw-   0        0        0      386 2023-06-21 21:32:18.000000 QT-PyQt-PySide-Custom-Widgets-0.6.6/Custom_Widgets/Qss/icons/original_svg/save.svg
+-rw-rw-rw-   0        0        0      438 2023-06-21 21:32:18.000000 QT-PyQt-PySide-Custom-Widgets-0.6.6/Custom_Widgets/Qss/icons/original_svg/scissors.svg
+-rw-rw-rw-   0        0        0      302 2023-06-21 21:32:18.000000 QT-PyQt-PySide-Custom-Widgets-0.6.6/Custom_Widgets/Qss/icons/original_svg/search.svg
+-rw-rw-rw-   0        0        0      308 2023-06-21 21:32:18.000000 QT-PyQt-PySide-Custom-Widgets-0.6.6/Custom_Widgets/Qss/icons/original_svg/send.svg
+-rw-rw-rw-   0        0        0      425 2023-06-21 21:32:18.000000 QT-PyQt-PySide-Custom-Widgets-0.6.6/Custom_Widgets/Qss/icons/original_svg/server.svg
+-rw-rw-rw-   0        0        0     1005 2023-06-21 21:32:18.000000 QT-PyQt-PySide-Custom-Widgets-0.6.6/Custom_Widgets/Qss/icons/original_svg/settings.svg
+-rw-rw-rw-   0        0        0      439 2023-06-21 21:32:18.000000 QT-PyQt-PySide-Custom-Widgets-0.6.6/Custom_Widgets/Qss/icons/original_svg/share-2.svg
+-rw-rw-rw-   0        0        0      358 2023-06-21 21:32:18.000000 QT-PyQt-PySide-Custom-Widgets-0.6.6/Custom_Widgets/Qss/icons/original_svg/share.svg
+-rw-rw-rw-   0        0        0      399 2023-06-21 21:32:18.000000 QT-PyQt-PySide-Custom-Widgets-0.6.6/Custom_Widgets/Qss/icons/original_svg/shield-off.svg
+-rw-rw-rw-   0        0        0      273 2023-06-21 21:32:18.000000 QT-PyQt-PySide-Custom-Widgets-0.6.6/Custom_Widgets/Qss/icons/original_svg/shield.svg
+-rw-rw-rw-   0        0        0      366 2023-06-21 21:32:18.000000 QT-PyQt-PySide-Custom-Widgets-0.6.6/Custom_Widgets/Qss/icons/original_svg/shopping-bag.svg
+-rw-rw-rw-   0        0        0      377 2023-06-21 21:32:18.000000 QT-PyQt-PySide-Custom-Widgets-0.6.6/Custom_Widgets/Qss/icons/original_svg/shopping-cart.svg
+-rw-rw-rw-   0        0        0      435 2023-06-21 21:32:18.000000 QT-PyQt-PySide-Custom-Widgets-0.6.6/Custom_Widgets/Qss/icons/original_svg/shuffle.svg
+-rw-rw-rw-   0        0        0      317 2023-06-21 21:32:18.000000 QT-PyQt-PySide-Custom-Widgets-0.6.6/Custom_Widgets/Qss/icons/original_svg/sidebar.svg
+-rw-rw-rw-   0        0        0      307 2023-06-21 21:32:18.000000 QT-PyQt-PySide-Custom-Widgets-0.6.6/Custom_Widgets/Qss/icons/original_svg/skip-back.svg
+-rw-rw-rw-   0        0        0      309 2023-06-21 21:32:18.000000 QT-PyQt-PySide-Custom-Widgets-0.6.6/Custom_Widgets/Qss/icons/original_svg/skip-forward.svg
+-rw-rw-rw-   0        0        0      993 2023-06-21 21:32:18.000000 QT-PyQt-PySide-Custom-Widgets-0.6.6/Custom_Widgets/Qss/icons/original_svg/slack.svg
+-rw-rw-rw-   0        0        0      306 2023-06-21 21:32:18.000000 QT-PyQt-PySide-Custom-Widgets-0.6.6/Custom_Widgets/Qss/icons/original_svg/slash.svg
+-rw-rw-rw-   0        0        0      605 2023-06-21 21:32:18.000000 QT-PyQt-PySide-Custom-Widgets-0.6.6/Custom_Widgets/Qss/icons/original_svg/sliders.svg
+-rw-rw-rw-   0        0        0      326 2023-06-21 21:32:18.000000 QT-PyQt-PySide-Custom-Widgets-0.6.6/Custom_Widgets/Qss/icons/original_svg/smartphone.svg
+-rw-rw-rw-   0        0        0      382 2023-06-21 21:32:18.000000 QT-PyQt-PySide-Custom-Widgets-0.6.6/Custom_Widgets/Qss/icons/original_svg/smile.svg
+-rw-rw-rw-   0        0        0      360 2023-06-21 21:32:18.000000 QT-PyQt-PySide-Custom-Widgets-0.6.6/Custom_Widgets/Qss/icons/original_svg/speaker.svg
+-rw-rw-rw-   0        0        0      274 2023-06-21 21:32:18.000000 QT-PyQt-PySide-Custom-Widgets-0.6.6/Custom_Widgets/Qss/icons/original_svg/square.svg
+-rw-rw-rw-   0        0        0      333 2023-06-21 21:32:18.000000 QT-PyQt-PySide-Custom-Widgets-0.6.6/Custom_Widgets/Qss/icons/original_svg/star.svg
+-rw-rw-rw-   0        0        0      303 2023-06-21 21:32:18.000000 QT-PyQt-PySide-Custom-Widgets-0.6.6/Custom_Widgets/Qss/icons/original_svg/stop-circle.svg
+-rw-rw-rw-   0        0        0      644 2023-06-21 21:32:18.000000 QT-PyQt-PySide-Custom-Widgets-0.6.6/Custom_Widgets/Qss/icons/original_svg/sun.svg
+-rw-rw-rw-   0        0        0      583 2023-06-21 21:32:18.000000 QT-PyQt-PySide-Custom-Widgets-0.6.6/Custom_Widgets/Qss/icons/original_svg/sunrise.svg
+-rw-rw-rw-   0        0        0      582 2023-06-21 21:32:18.000000 QT-PyQt-PySide-Custom-Widgets-0.6.6/Custom_Widgets/Qss/icons/original_svg/sunset.svg
+-rw-rw-rw-   0        0        0      322 2023-06-21 21:32:18.000000 QT-PyQt-PySide-Custom-Widgets-0.6.6/Custom_Widgets/Qss/icons/original_svg/tablet.svg
+-rw-rw-rw-   0        0        0      349 2023-06-21 21:32:18.000000 QT-PyQt-PySide-Custom-Widgets-0.6.6/Custom_Widgets/Qss/icons/original_svg/tag.svg
+-rw-rw-rw-   0        0        0      330 2023-06-21 21:32:18.000000 QT-PyQt-PySide-Custom-Widgets-0.6.6/Custom_Widgets/Qss/icons/original_svg/target.svg
+-rw-rw-rw-   0        0        0      304 2023-06-21 21:32:18.000000 QT-PyQt-PySide-Custom-Widgets-0.6.6/Custom_Widgets/Qss/icons/original_svg/terminal.svg
+-rw-rw-rw-   0        0        0      291 2023-06-21 21:32:18.000000 QT-PyQt-PySide-Custom-Widgets-0.6.6/Custom_Widgets/Qss/icons/original_svg/thermometer.svg
+-rw-rw-rw-   0        0        0      368 2023-06-21 21:32:18.000000 QT-PyQt-PySide-Custom-Widgets-0.6.6/Custom_Widgets/Qss/icons/original_svg/thumbs-down.svg
+-rw-rw-rw-   0        0        0      348 2023-06-21 21:32:18.000000 QT-PyQt-PySide-Custom-Widgets-0.6.6/Custom_Widgets/Qss/icons/original_svg/thumbs-up.svg
+-rw-rw-rw-   0        0        0      317 2023-06-21 21:32:18.000000 QT-PyQt-PySide-Custom-Widgets-0.6.6/Custom_Widgets/Qss/icons/original_svg/toggle-left.svg
+-rw-rw-rw-   0        0        0      319 2023-06-21 21:32:18.000000 QT-PyQt-PySide-Custom-Widgets-0.6.6/Custom_Widgets/Qss/icons/original_svg/toggle-right.svg
+-rw-rw-rw-   0        0        0      380 2023-06-21 21:32:18.000000 QT-PyQt-PySide-Custom-Widgets-0.6.6/Custom_Widgets/Qss/icons/original_svg/tool.svg
+-rw-rw-rw-   0        0        0     2703 2023-06-21 21:32:18.000000 QT-PyQt-PySide-Custom-Widgets-0.6.6/Custom_Widgets/Qss/icons/original_svg/toolbar_move_horizontal.svg
+-rw-rw-rw-   0        0        0     2710 2023-06-21 21:32:18.000000 QT-PyQt-PySide-Custom-Widgets-0.6.6/Custom_Widgets/Qss/icons/original_svg/toolbar_move_vertical.svg
+-rw-rw-rw-   0        0        0     2464 2023-06-21 21:32:18.000000 QT-PyQt-PySide-Custom-Widgets-0.6.6/Custom_Widgets/Qss/icons/original_svg/toolbar_separator_horizontal.svg
+-rw-rw-rw-   0        0        0     2463 2023-06-21 21:32:18.000000 QT-PyQt-PySide-Custom-Widgets-0.6.6/Custom_Widgets/Qss/icons/original_svg/toolbar_separator_vertical.svg
+-rw-rw-rw-   0        0        0     2347 2023-06-21 21:32:18.000000 QT-PyQt-PySide-Custom-Widgets-0.6.6/Custom_Widgets/Qss/icons/original_svg/transparent.svg
+-rw-rw-rw-   0        0        0      442 2023-06-21 21:32:18.000000 QT-PyQt-PySide-Custom-Widgets-0.6.6/Custom_Widgets/Qss/icons/original_svg/trash-2.svg
+-rw-rw-rw-   0        0        0      350 2023-06-21 21:32:18.000000 QT-PyQt-PySide-Custom-Widgets-0.6.6/Custom_Widgets/Qss/icons/original_svg/trash.svg
+-rw-rw-rw-   0        0        0      367 2023-06-21 21:32:18.000000 QT-PyQt-PySide-Custom-Widgets-0.6.6/Custom_Widgets/Qss/icons/original_svg/trello.svg
+-rw-rw-rw-   0        0        0      325 2023-06-21 21:32:18.000000 QT-PyQt-PySide-Custom-Widgets-0.6.6/Custom_Widgets/Qss/icons/original_svg/trending-down.svg
+-rw-rw-rw-   0        0        0      322 2023-06-21 21:32:18.000000 QT-PyQt-PySide-Custom-Widgets-0.6.6/Custom_Widgets/Qss/icons/original_svg/trending-up.svg
+-rw-rw-rw-   0        0        0      320 2023-06-21 21:32:18.000000 QT-PyQt-PySide-Custom-Widgets-0.6.6/Custom_Widgets/Qss/icons/original_svg/triangle.svg
+-rw-rw-rw-   0        0        0      409 2023-06-21 21:32:18.000000 QT-PyQt-PySide-Custom-Widgets-0.6.6/Custom_Widgets/Qss/icons/original_svg/truck.svg
+-rw-rw-rw-   0        0        0      314 2023-06-21 21:32:18.000000 QT-PyQt-PySide-Custom-Widgets-0.6.6/Custom_Widgets/Qss/icons/original_svg/tv.svg
+-rw-rw-rw-   0        0        0      271 2023-06-21 21:32:18.000000 QT-PyQt-PySide-Custom-Widgets-0.6.6/Custom_Widgets/Qss/icons/original_svg/twitch.svg
+-rw-rw-rw-   0        0        0      402 2023-06-21 21:32:18.000000 QT-PyQt-PySide-Custom-Widgets-0.6.6/Custom_Widgets/Qss/icons/original_svg/twitter.svg
+-rw-rw-rw-   0        0        0      346 2023-06-21 21:32:18.000000 QT-PyQt-PySide-Custom-Widgets-0.6.6/Custom_Widgets/Qss/icons/original_svg/type.svg
+-rw-rw-rw-   0        0        0      284 2023-06-21 21:32:18.000000 QT-PyQt-PySide-Custom-Widgets-0.6.6/Custom_Widgets/Qss/icons/original_svg/umbrella.svg
+-rw-rw-rw-   0        0        0      313 2023-06-21 21:32:18.000000 QT-PyQt-PySide-Custom-Widgets-0.6.6/Custom_Widgets/Qss/icons/original_svg/underline.svg
+-rw-rw-rw-   0        0        0      316 2023-06-21 21:32:18.000000 QT-PyQt-PySide-Custom-Widgets-0.6.6/Custom_Widgets/Qss/icons/original_svg/unlock.svg
+-rw-rw-rw-   0        0        0      425 2023-06-21 21:32:18.000000 QT-PyQt-PySide-Custom-Widgets-0.6.6/Custom_Widgets/Qss/icons/original_svg/upload-cloud.svg
+-rw-rw-rw-   0        0        0      359 2023-06-21 21:32:18.000000 QT-PyQt-PySide-Custom-Widgets-0.6.6/Custom_Widgets/Qss/icons/original_svg/upload.svg
+-rw-rw-rw-   0        0        0      361 2023-06-21 21:32:18.000000 QT-PyQt-PySide-Custom-Widgets-0.6.6/Custom_Widgets/Qss/icons/original_svg/user-check.svg
+-rw-rw-rw-   0        0        0      359 2023-06-21 21:32:18.000000 QT-PyQt-PySide-Custom-Widgets-0.6.6/Custom_Widgets/Qss/icons/original_svg/user-minus.svg
+-rw-rw-rw-   0        0        0      402 2023-06-21 21:32:18.000000 QT-PyQt-PySide-Custom-Widgets-0.6.6/Custom_Widgets/Qss/icons/original_svg/user-plus.svg
+-rw-rw-rw-   0        0        0      398 2023-06-21 21:32:18.000000 QT-PyQt-PySide-Custom-Widgets-0.6.6/Custom_Widgets/Qss/icons/original_svg/user-x.svg
+-rw-rw-rw-   0        0        0      307 2023-06-21 21:32:18.000000 QT-PyQt-PySide-Custom-Widgets-0.6.6/Custom_Widgets/Qss/icons/original_svg/user.svg
+-rw-rw-rw-   0        0        0      394 2023-06-21 21:32:18.000000 QT-PyQt-PySide-Custom-Widgets-0.6.6/Custom_Widgets/Qss/icons/original_svg/users.svg
+-rw-rw-rw-   0        0        0      373 2023-06-21 21:32:18.000000 QT-PyQt-PySide-Custom-Widgets-0.6.6/Custom_Widgets/Qss/icons/original_svg/video-off.svg
+-rw-rw-rw-   0        0        0      323 2023-06-21 21:32:18.000000 QT-PyQt-PySide-Custom-Widgets-0.6.6/Custom_Widgets/Qss/icons/original_svg/video.svg
+-rw-rw-rw-   0        0        0      352 2023-06-21 21:32:18.000000 QT-PyQt-PySide-Custom-Widgets-0.6.6/Custom_Widgets/Qss/icons/original_svg/voicemail.svg
+-rw-rw-rw-   0        0        0      322 2023-06-21 21:32:18.000000 QT-PyQt-PySide-Custom-Widgets-0.6.6/Custom_Widgets/Qss/icons/original_svg/volume-1.svg
+-rw-rw-rw-   0        0        0      353 2023-06-21 21:32:18.000000 QT-PyQt-PySide-Custom-Widgets-0.6.6/Custom_Widgets/Qss/icons/original_svg/volume-2.svg
+-rw-rw-rw-   0        0        0      364 2023-06-21 21:32:18.000000 QT-PyQt-PySide-Custom-Widgets-0.6.6/Custom_Widgets/Qss/icons/original_svg/volume-x.svg
+-rw-rw-rw-   0        0        0      274 2023-06-21 21:32:18.000000 QT-PyQt-PySide-Custom-Widgets-0.6.6/Custom_Widgets/Qss/icons/original_svg/volume.svg
+-rw-rw-rw-   0        0        0      456 2023-06-21 21:32:18.000000 QT-PyQt-PySide-Custom-Widgets-0.6.6/Custom_Widgets/Qss/icons/original_svg/watch.svg
+-rw-rw-rw-   0        0        0      563 2023-06-21 21:32:18.000000 QT-PyQt-PySide-Custom-Widgets-0.6.6/Custom_Widgets/Qss/icons/original_svg/wifi-off.svg
+-rw-rw-rw-   0        0        0      395 2023-06-21 21:32:18.000000 QT-PyQt-PySide-Custom-Widgets-0.6.6/Custom_Widgets/Qss/icons/original_svg/wifi.svg
+-rw-rw-rw-   0        0        0      320 2023-06-21 21:32:18.000000 QT-PyQt-PySide-Custom-Widgets-0.6.6/Custom_Widgets/Qss/icons/original_svg/wind.svg
+-rw-rw-rw-   0        0        0     2953 2023-06-21 21:32:18.000000 QT-PyQt-PySide-Custom-Widgets-0.6.6/Custom_Widgets/Qss/icons/original_svg/window_close.svg
+-rw-rw-rw-   0        0        0     3018 2023-06-21 21:32:18.000000 QT-PyQt-PySide-Custom-Widgets-0.6.6/Custom_Widgets/Qss/icons/original_svg/window_grip.svg
+-rw-rw-rw-   0        0        0     2465 2023-06-21 21:32:18.000000 QT-PyQt-PySide-Custom-Widgets-0.6.6/Custom_Widgets/Qss/icons/original_svg/window_minimize.svg
+-rw-rw-rw-   0        0        0     2979 2023-06-21 21:32:18.000000 QT-PyQt-PySide-Custom-Widgets-0.6.6/Custom_Widgets/Qss/icons/original_svg/window_undock.svg
+-rw-rw-rw-   0        0        0      340 2023-06-21 21:32:18.000000 QT-PyQt-PySide-Custom-Widgets-0.6.6/Custom_Widgets/Qss/icons/original_svg/x-circle.svg
+-rw-rw-rw-   0        0        0      400 2023-06-21 21:32:18.000000 QT-PyQt-PySide-Custom-Widgets-0.6.6/Custom_Widgets/Qss/icons/original_svg/x-octagon.svg
+-rw-rw-rw-   0        0        0      362 2023-06-21 21:32:18.000000 QT-PyQt-PySide-Custom-Widgets-0.6.6/Custom_Widgets/Qss/icons/original_svg/x-square.svg
+-rw-rw-rw-   0        0        0      293 2023-06-21 21:32:18.000000 QT-PyQt-PySide-Custom-Widgets-0.6.6/Custom_Widgets/Qss/icons/original_svg/x.svg
+-rw-rw-rw-   0        0        0      559 2023-06-21 21:32:18.000000 QT-PyQt-PySide-Custom-Widgets-0.6.6/Custom_Widgets/Qss/icons/original_svg/youtube.svg
+-rw-rw-rw-   0        0        0      427 2023-06-21 21:32:18.000000 QT-PyQt-PySide-Custom-Widgets-0.6.6/Custom_Widgets/Qss/icons/original_svg/zap-off.svg
+-rw-rw-rw-   0        0        0      276 2023-06-21 21:32:18.000000 QT-PyQt-PySide-Custom-Widgets-0.6.6/Custom_Widgets/Qss/icons/original_svg/zap.svg
+-rw-rw-rw-   0        0        0      391 2023-06-21 21:32:18.000000 QT-PyQt-PySide-Custom-Widgets-0.6.6/Custom_Widgets/Qss/icons/original_svg/zoom-in.svg
+-rw-rw-rw-   0        0        0      348 2023-06-21 21:32:18.000000 QT-PyQt-PySide-Custom-Widgets-0.6.6/Custom_Widgets/Qss/icons/original_svg/zoom-out.svg
+-rw-rw-rw-   0        0        0      134 2023-06-21 21:32:18.000000 QT-PyQt-PySide-Custom-Widgets-0.6.6/Custom_Widgets/Qss/main.scss
+-rw-rw-rw-   0        0        0    30871 2023-06-21 21:32:18.000000 QT-PyQt-PySide-Custom-Widgets-0.6.6/Custom_Widgets/RoundProgressBar.py
+-rw-rw-rw-   0        0        0    40717 2023-06-21 21:32:18.000000 QT-PyQt-PySide-Custom-Widgets-0.6.6/Custom_Widgets/SpiralProgressBar.py
+-rw-rw-rw-   0        0        0   156605 2023-06-21 21:32:18.000000 QT-PyQt-PySide-Custom-Widgets-0.6.6/Custom_Widgets/Widgets.py
+-rw-rw-rw-   0        0        0     4824 2023-06-21 21:32:18.000000 QT-PyQt-PySide-Custom-Widgets-0.6.6/Custom_Widgets/WidgetsWorker.py
+-rw-rw-rw-   0        0        0       39 2023-06-21 21:32:18.000000 QT-PyQt-PySide-Custom-Widgets-0.6.6/Custom_Widgets/__init__.py
+drwxrwxrwx   0        0        0        0 2023-06-24 14:28:47.633954 QT-PyQt-PySide-Custom-Widgets-0.6.6/Custom_Widgets/components/
+drwxrwxrwx   0        0        0        0 2023-06-24 14:28:52.480988 QT-PyQt-PySide-Custom-Widgets-0.6.6/Custom_Widgets/components/json/
+-rw-rw-rw-   0        0        0      344 2023-06-21 21:32:18.000000 QT-PyQt-PySide-Custom-Widgets-0.6.6/Custom_Widgets/components/json/style.json
+drwxrwxrwx   0        0        0        0 2023-06-24 14:28:52.506046 QT-PyQt-PySide-Custom-Widgets-0.6.6/Custom_Widgets/components/python/
+drwxrwxrwx   0        0        0        0 2023-06-24 14:28:52.517804 QT-PyQt-PySide-Custom-Widgets-0.6.6/Custom_Widgets/components/python/__pycache__/
+-rw-rw-rw-   0        0        0      853 2023-06-21 21:32:18.000000 QT-PyQt-PySide-Custom-Widgets-0.6.6/Custom_Widgets/components/python/__pycache__/main.cpython-310.pyc
+-rw-rw-rw-   0        0        0      836 2023-06-21 21:32:18.000000 QT-PyQt-PySide-Custom-Widgets-0.6.6/Custom_Widgets/components/python/__pycache__/main.cpython-38.pyc
+-rw-rw-rw-   0        0        0     2561 2023-06-21 21:32:18.000000 QT-PyQt-PySide-Custom-Widgets-0.6.6/Custom_Widgets/components/python/__pycache__/ui_interface.cpython-310.pyc
+-rw-rw-rw-   0        0        0     2552 2023-06-21 21:32:18.000000 QT-PyQt-PySide-Custom-Widgets-0.6.6/Custom_Widgets/components/python/__pycache__/ui_interface.cpython-38.pyc
+-rw-rw-rw-   0        0        0     2679 2023-06-21 21:32:18.000000 QT-PyQt-PySide-Custom-Widgets-0.6.6/Custom_Widgets/components/python/main.py
+-rw-rw-rw-   0        0        0     3127 2023-06-21 21:32:18.000000 QT-PyQt-PySide-Custom-Widgets-0.6.6/Custom_Widgets/components/python/ui_interface.py
+drwxrwxrwx   0        0        0        0 2023-06-24 14:28:52.529802 QT-PyQt-PySide-Custom-Widgets-0.6.6/Custom_Widgets/components/uis/
+-rw-rw-rw-   0        0        0     2691 2023-06-21 21:32:18.000000 QT-PyQt-PySide-Custom-Widgets-0.6.6/Custom_Widgets/components/uis/interface.ui
+-rw-rw-rw-   0        0        0     1242 2023-06-21 21:32:18.000000 QT-PyQt-PySide-Custom-Widgets-0.6.6/Custom_Widgets/interface.ui
+-rw-rw-rw-   0        0        0     2368 2023-06-21 21:32:18.000000 QT-PyQt-PySide-Custom-Widgets-0.6.6/Custom_Widgets/main.py
+-rw-rw-rw-   0        0        0    35149 2021-06-11 19:06:36.000000 QT-PyQt-PySide-Custom-Widgets-0.6.6/LICENSE
+-rw-rw-rw-   0        0        0       82 2022-02-17 19:32:18.000000 QT-PyQt-PySide-Custom-Widgets-0.6.6/MANIFEST.in
+-rw-rw-rw-   0        0        0     4179 2023-06-24 14:28:52.599805 QT-PyQt-PySide-Custom-Widgets-0.6.6/PKG-INFO
+drwxrwxrwx   0        0        0        0 2023-06-24 14:28:52.598805 QT-PyQt-PySide-Custom-Widgets-0.6.6/QT_PyQt_PySide_Custom_Widgets.egg-info/
+-rw-rw-rw-   0        0        0     4179 2023-06-24 14:28:45.000000 QT-PyQt-PySide-Custom-Widgets-0.6.6/QT_PyQt_PySide_Custom_Widgets.egg-info/PKG-INFO
+-rw-rw-rw-   0        0        0    19309 2023-06-24 14:28:46.000000 QT-PyQt-PySide-Custom-Widgets-0.6.6/QT_PyQt_PySide_Custom_Widgets.egg-info/SOURCES.txt
+-rw-rw-rw-   0        0        0        1 2023-06-24 14:28:45.000000 QT-PyQt-PySide-Custom-Widgets-0.6.6/QT_PyQt_PySide_Custom_Widgets.egg-info/dependency_links.txt
+-rw-rw-rw-   0        0        0       45 2023-06-24 14:28:45.000000 QT-PyQt-PySide-Custom-Widgets-0.6.6/QT_PyQt_PySide_Custom_Widgets.egg-info/requires.txt
+-rw-rw-rw-   0        0        0       15 2023-06-24 14:28:45.000000 QT-PyQt-PySide-Custom-Widgets-0.6.6/QT_PyQt_PySide_Custom_Widgets.egg-info/top_level.txt
+-rw-rw-rw-   0        0        0     3169 2022-08-11 03:08:01.000000 QT-PyQt-PySide-Custom-Widgets-0.6.6/README.md
+-rw-rw-rw-   0        0        0       42 2023-06-24 14:28:52.611738 QT-PyQt-PySide-Custom-Widgets-0.6.6/setup.cfg
+-rw-rw-rw-   0        0        0     2280 2023-06-24 14:27:59.000000 QT-PyQt-PySide-Custom-Widgets-0.6.6/setup.py
```

### Comparing `QT-PyQt-PySide-Custom-Widgets-0.6.5/Custom_Widgets/AnalogGaugeWidget.py` & `QT-PyQt-PySide-Custom-Widgets-0.6.6/Custom_Widgets/AnalogGaugeWidget.py`

 * *Files identical despite different names*

### Comparing `QT-PyQt-PySide-Custom-Widgets-0.6.5/Custom_Widgets/ProgressIndicator/__pycache__/test.cpython-310.pyc` & `QT-PyQt-PySide-Custom-Widgets-0.6.6/Custom_Widgets/ProgressIndicator/__pycache__/test.cpython-310.pyc`

 * *Files identical despite different names*

### Comparing `QT-PyQt-PySide-Custom-Widgets-0.6.5/Custom_Widgets/ProgressIndicator/__pycache__/test.cpython-38.pyc` & `QT-PyQt-PySide-Custom-Widgets-0.6.6/Custom_Widgets/ProgressIndicator/__pycache__/test.cpython-38.pyc`

 * *Format-specific differences are supported for Python .pyc files but no file-specific differences were detected; falling back to a binary diff. file(1) reports: Byte-compiled Python module for CPython 3.8, timestamp-based, .py timestamp: Wed Jun 21 20:45:30 2023 UTC, .py size: 9452 bytes*

 * *Could not decompile bytecode: bad marshal data (unknown type code)*

 * *Files 1% similar despite different names*

```diff
@@ -1,8 +1,8 @@
-00000000: 550d 0d0a 0000 0000 6a61 9364 ec24 0000  U.......ja.d.$..
+00000000: 550d 0d0a 0000 0000 626c 9364 ec24 0000  U.......bl.d.$..
 00000010: e300 0000 0000 0000 0000 0000 0000 0000  ................
 00000020: 0009 0000 0040 0000 0073 9800 0000 6400  .....@...s....d.
 00000030: 6401 6c00 5a00 7a18 6400 6402 6c01 6d02  d.l.Z.z.d.d.l.m.
 00000040: 5a02 0100 6400 6403 6c03 5400 5700 6e42  Z...d.d.l.T.W.nB
 00000050: 0100 0100 0100 7a18 6400 6402 6c04 6d02  ......z.d.d.l.m.
 00000060: 5a02 0100 6400 6403 6c05 5400 5700 6e1c  Z...d.d.l.T.W.n.
 00000070: 0100 0100 0100 6506 6404 8301 0100 6500  ......e.d.....e.
```

### Comparing `QT-PyQt-PySide-Custom-Widgets-0.6.5/Custom_Widgets/ProgressIndicator/__pycache__/ui_interface.cpython-310.pyc` & `QT-PyQt-PySide-Custom-Widgets-0.6.6/Custom_Widgets/ProgressIndicator/__pycache__/ui_interface.cpython-310.pyc`

 * *Files identical despite different names*

### Comparing `QT-PyQt-PySide-Custom-Widgets-0.6.5/Custom_Widgets/ProgressIndicator/__pycache__/ui_interface.cpython-38.pyc` & `QT-PyQt-PySide-Custom-Widgets-0.6.6/Custom_Widgets/ProgressIndicator/__pycache__/ui_interface.cpython-38.pyc`

 * *Format-specific differences are supported for Python .pyc files but no file-specific differences were detected; falling back to a binary diff. file(1) reports: Byte-compiled Python module for CPython 3.8, timestamp-based, .py timestamp: Wed Jun 21 20:45:30 2023 UTC, .py size: 9629 bytes*

 * *Could not decompile bytecode: bad marshal data (unknown type code)*

 * *Files 4% similar despite different names*

```diff
@@ -1,8 +1,8 @@
-00000000: 550d 0d0a 0000 0000 6a61 9364 9d25 0000  U.......ja.d.%..
+00000000: 550d 0d0a 0000 0000 626c 9364 9d25 0000  U.......bl.d.%..
 00000010: e300 0000 0000 0000 0000 0000 0000 0000  ................
 00000020: 0004 0000 0040 0000 0073 3800 0000 6400  .....@...s8...d.
 00000030: 6401 6c00 5400 6400 6401 6c01 5400 6400  d.l.T.d.d.l.T.d.
 00000040: 6401 6c02 5400 6400 6402 6c03 6d04 5a04  d.l.T.d.d.l.m.Z.
 00000050: 0100 4700 6403 6404 8400 6404 6505 8303  ..G.d.d...d.e...
 00000060: 5a06 6405 5300 2906 e900 0000 0029 01da  Z.d.S.)......)..
 00000070: 012a 2901 da15 466f 726d 5072 6f67 7265  .*)...FormProgre
@@ -194,15 +194,15 @@
 00000c10: 2200 0000 7223 0000 0072 2400 0000 7225  "...r#...r$...r%
 00000c20: 0000 0072 2600 0000 7227 0000 005a 1073  ...r&...r'...Z.s
 00000c30: 6574 4365 6e74 7261 6c57 6964 6765 74da  etCentralWidget.
 00000c40: 0d72 6574 7261 6e73 6c61 7465 5569 5a0b  .retranslateUiZ.
 00000c50: 514d 6574 614f 626a 6563 745a 1263 6f6e  QMetaObjectZ.con
 00000c60: 6e65 6374 536c 6f74 7342 794e 616d 6529  nectSlotsByName)
 00000c70: 04da 0473 656c 6672 0500 0000 7229 0000  ...selfr....r)..
-00000c80: 00da 0466 6f6e 74a9 0072 2d00 0000 fa5b  ...font..r-....[
+00000c80: 005a 0466 6f6e 74a9 0072 2c00 0000 fa5b  .Z.font..r,....[
 00000c90: 633a 5c75 7365 7273 5c6b 6962 6574 5c61  c:\users\kibet\a
 00000ca0: 6e61 636f 6e64 6133 5c4c 6962 5c73 6974  naconda3\Lib\sit
 00000cb0: 652d 7061 636b 6167 6573 5c43 7573 746f  e-packages\Custo
 00000cc0: 6d5f 5769 6467 6574 732f 5072 6f67 7265  m_Widgets/Progre
 00000cd0: 7373 496e 6469 6361 746f 722f 7569 5f69  ssIndicator/ui_i
 00000ce0: 6e74 6572 6661 6365 2e70 79da 0773 6574  nterface.py..set
 00000cf0: 7570 5569 1300 0000 73f4 0000 0000 0108  upUi....s.......
@@ -302,29 +302,29 @@
 000012d0: 6174 6572 0800 0000 5a07 7365 7454 6578  ater....Z.setTex
 000012e0: 7472 0b00 0000 720e 0000 0072 0f00 0000  tr....r....r....
 000012f0: 7211 0000 0072 1200 0000 7213 0000 0072  r....r....r....r
 00001300: 1400 0000 7218 0000 0072 1900 0000 721a  ....r....r....r.
 00001310: 0000 0072 1b00 0000 721c 0000 0072 1d00  ...r....r....r..
 00001320: 0000 7222 0000 0072 2300 0000 7224 0000  ..r"...r#...r$..
 00001330: 0072 2500 0000 7226 0000 0072 2700 0000  .r%...r&...r'...
-00001340: 2902 722b 0000 0072 0500 0000 722d 0000  ).r+...r....r-..
-00001350: 0072 2d00 0000 722e 0000 0072 2a00 0000  .r-...r....r*...
+00001340: 2902 722b 0000 0072 0500 0000 722c 0000  ).r+...r....r,..
+00001350: 0072 2c00 0000 722d 0000 0072 2a00 0000  .r,...r-...r*...
 00001360: cc00 0000 732a 0000 0000 0114 0116 0116  ....s*..........
 00001370: 0116 0116 0116 0116 0116 0116 0116 0116  ................
 00001380: 0116 0116 0116 0116 0116 0116 0116 0116  ................
 00001390: 0116 017a 1b55 695f 4d61 696e 5769 6e64  ...z.Ui_MainWind
 000013a0: 6f77 2e72 6574 7261 6e73 6c61 7465 5569  ow.retranslateUi
 000013b0: 4e29 05da 085f 5f6e 616d 655f 5fda 0a5f  N)...__name__.._
 000013c0: 5f6d 6f64 756c 655f 5fda 0c5f 5f71 7561  _module__..__qua
-000013d0: 6c6e 616d 655f 5f72 2f00 0000 722a 0000  lname__r/...r*..
-000013e0: 0072 2d00 0000 722d 0000 0072 2d00 0000  .r-...r-...r-...
-000013f0: 722e 0000 0072 0400 0000 1200 0000 7306  r....r........s.
+000013d0: 6c6e 616d 655f 5f72 2e00 0000 722a 0000  lname__r....r*..
+000013e0: 0072 2c00 0000 722c 0000 0072 2c00 0000  .r,...r,...r,...
+000013f0: 722d 0000 0072 0400 0000 1200 0000 7306  r-...r........s.
 00001400: 0000 0008 0108 7f00 3a72 0400 0000 4e29  ........:r....N)
 00001410: 075a 0e50 7953 6964 6532 2e51 7443 6f72  .Z.PySide2.QtCor
 00001420: 655a 0d50 7953 6964 6532 2e51 7447 7569  eZ.PySide2.QtGui
 00001430: 5a11 5079 5369 6465 322e 5174 5769 6467  Z.PySide2.QtWidg
 00001440: 6574 735a 1643 7573 746f 6d5f 5769 6467  etsZ.Custom_Widg
 00001450: 6574 732e 5769 6467 6574 7372 0300 0000  ets.Widgetsr....
-00001460: da06 6f62 6a65 6374 7204 0000 0072 2d00  ..objectr....r-.
-00001470: 0000 722d 0000 0072 2d00 0000 722e 0000  ..r-...r-...r...
+00001460: da06 6f62 6a65 6374 7204 0000 0072 2c00  ..objectr....r,.
+00001470: 0000 722c 0000 0072 2c00 0000 722d 0000  ..r,...r,...r-..
 00001480: 00da 083c 6d6f 6475 6c65 3e0b 0000 0073  ...<module>....s
 00001490: 0800 0000 0801 0801 0802 0c03            ............
```

### Comparing `QT-PyQt-PySide-Custom-Widgets-0.6.5/Custom_Widgets/ProgressIndicator/__pycache__/ui_interface.cpython-39.pyc` & `QT-PyQt-PySide-Custom-Widgets-0.6.6/Custom_Widgets/ProgressIndicator/__pycache__/ui_interface.cpython-39.pyc`

 * *Files identical despite different names*

### Comparing `QT-PyQt-PySide-Custom-Widgets-0.6.5/Custom_Widgets/ProgressIndicator/interface.ui` & `QT-PyQt-PySide-Custom-Widgets-0.6.6/Custom_Widgets/ProgressIndicator/interface.ui`

 * *Files identical despite different names*

### Comparing `QT-PyQt-PySide-Custom-Widgets-0.6.5/Custom_Widgets/ProgressIndicator/test.py` & `QT-PyQt-PySide-Custom-Widgets-0.6.6/Custom_Widgets/ProgressIndicator/test.py`

 * *Files identical despite different names*

### Comparing `QT-PyQt-PySide-Custom-Widgets-0.6.5/Custom_Widgets/ProgressIndicator/ui_interface.py` & `QT-PyQt-PySide-Custom-Widgets-0.6.6/Custom_Widgets/ProgressIndicator/ui_interface.py`

 * *Files identical despite different names*

### Comparing `QT-PyQt-PySide-Custom-Widgets-0.6.5/Custom_Widgets/ProjectMaker.py` & `QT-PyQt-PySide-Custom-Widgets-0.6.6/Custom_Widgets/ProjectMaker.py`

 * *Files identical despite different names*

### Comparing `QT-PyQt-PySide-Custom-Widgets-0.6.5/Custom_Widgets/Qss/QSS_Resources.qrc` & `QT-PyQt-PySide-Custom-Widgets-0.6.6/Custom_Widgets/Qss/QSS_Resources.qrc`

 * *Files identical despite different names*

### Comparing `QT-PyQt-PySide-Custom-Widgets-0.6.5/Custom_Widgets/Qss/SassCompiler.py` & `QT-PyQt-PySide-Custom-Widgets-0.6.6/Custom_Widgets/Qss/SassCompiler.py`

 * *Files 20% similar despite different names*

```diff
@@ -96,14 +96,40 @@
 
             f.close()
 
         qtsass.compile_filename(main_sass_path, css_path)
         
         with open(css_path,"r") as css:
             self.setStyleSheet(css.read())
+        
+        # QPalette
+        palette = QPalette()
+
+        # Set the background color
+        palette.setColor(QPalette.Background, QColor(self.theme.COLOR_BACKGROUND_1))
+
+        # Set the text color
+        palette.setColor(QPalette.Text, QColor(self.theme.COLOR_TEXT_1))
+
+        # Set the button color
+        palette.setColor(QPalette.Button, QColor(self.theme.COLOR_BACKGROUND_3))
+
+        # Set the button text color
+        palette.setColor(QPalette.ButtonText, QColor(self.theme.COLOR_TEXT_1))
+
+        # Set the highlight color
+        palette.setColor(QPalette.Highlight, QColor(self.theme.COLOR_BACKGROUND_6))
+
+        # Set the highlight text color
+        palette.setColor(QPalette.HighlightedText, QColor(self.theme.COLOR_ACCENT_1))
+
+        # Apply the palette to the main window
+        self.setPalette(palette)
+
+        
 
 
         ########################################################################
         ## GENERATE NEW ICONS
         # START WORKER
         # CURRENT THEME ICONS
         iconsWorker = Worker(self.compileSassTheme)
```

### Comparing `QT-PyQt-PySide-Custom-Widgets-0.6.5/Custom_Widgets/Qss/SvgToPngIcons.py` & `QT-PyQt-PySide-Custom-Widgets-0.6.6/Custom_Widgets/Qss/SvgToPngIcons.py`

 * *Files 4% similar despite different names*

```diff
@@ -1,17 +1,21 @@
 import cairosvg
 import codecs
 import os
 import sys
 import shutil
+import importlib
+import random
+import string
 from urllib.parse import urlparse
 from pathlib import Path
 import __main__
 
 
+
 from . colorsystem import *
 
 settings = QSettings()
 
 class NewIconsGenerator():
     """docstring for NewIconsGenerator"""
     def __init__(self, arg):
@@ -173,18 +177,41 @@
             try:
                 settings.setValue("ICONS-COLOR", normal_color)
                 os.system('pyrcc5 "'+resource_path+'" -o "'+py_resource_path+'"')
                 settings.setValue("ICONS-COLOR", normal_color)
             except Exception as e:
                 # raise e
                 print("error while converting resource file")  
+
+            # Reload resources:
+            resource_module = "QSS_Resources_rc"  # Replace with your resource module name
+            # NewIconsGenerator.reload_resources(self, resource_module)
+
         else:
             ## GENERATE OTHER ICONS
             NewIconsGenerator.generateAllIcons(self, progress_callback) 
 
+    def reload_resources(self, resource_module):
+        # Generate a random name for the new resource file
+        random_name = ''.join(random.choices(string.ascii_lowercase, k=8))
+        new_resource_file = f"QSS_Resources_rc_{random_name}.py"
+
+        # Copy the resource.py file to the new name
+        os.rename("QSS_Resources_rc.py", new_resource_file)
+
+        # Delete any old resource files in the directory
+        for file in os.listdir():
+            if file.startswith("QSS_Resources_rc_") and file.endswith(".py") and file != new_resource_file:
+                os.remove(file)
+
+        # Import the new resource module
+        resource_module = importlib.import_module(new_resource_file[:-3])
+
+        print("resource loaded")
+
     def generateAllIcons(self, progress_callback):
         settings = QSettings()
         # Files folder
         dirname = os.path.dirname(__file__)
         filename = os.path.join(dirname, 'icons/original_svg')
         list_of_files = []
```

### Comparing `QT-PyQt-PySide-Custom-Widgets-0.6.5/Custom_Widgets/Qss/__pycache__/QSS_Resources.cpython-39.pyc` & `QT-PyQt-PySide-Custom-Widgets-0.6.6/Custom_Widgets/Qss/__pycache__/QSS_Resources.cpython-39.pyc`

 * *Files identical despite different names*

### Comparing `QT-PyQt-PySide-Custom-Widgets-0.6.5/Custom_Widgets/Qss/__pycache__/SassCompiler.cpython-310.pyc` & `QT-PyQt-PySide-Custom-Widgets-0.6.6/Custom_Widgets/Qss/__pycache__/SassCompiler.cpython-310.pyc`

 * *Files identical despite different names*

### Comparing `QT-PyQt-PySide-Custom-Widgets-0.6.5/Custom_Widgets/Qss/__pycache__/SassCompiler.cpython-38.pyc` & `QT-PyQt-PySide-Custom-Widgets-0.6.6/Custom_Widgets/Qss/__pycache__/SassCompiler.cpython-38.pyc`

 * *Format-specific differences are supported for Python .pyc files but no file-specific differences were detected; falling back to a binary diff. file(1) reports: Byte-compiled Python module for CPython 3.8, timestamp-based, .py timestamp: Wed Jun 21 20:45:30 2023 UTC, .py size: 5505 bytes*

 * *Could not decompile bytecode: bad marshal data (unknown type code)*

 * *Files 11% similar despite different names*

```diff
@@ -1,8 +1,8 @@
-00000000: 550d 0d0a 0000 0000 6a61 9364 8115 0000  U.......ja.d....
+00000000: 550d 0d0a 0000 0000 116e 9464 cf18 0000  U........n.d....
 00000010: e300 0000 0000 0000 0000 0000 0000 0000  ................
 00000020: 0003 0000 0040 0000 0073 8000 0000 6400  .....@...s....d.
 00000030: 6401 6c00 5a00 6400 6402 6c01 5400 6400  d.l.Z.d.d.l.T.d.
 00000040: 6402 6c02 5400 6400 6402 6c03 5400 6400  d.l.T.d.d.l.T.d.
 00000050: 6401 6c04 5a04 6400 6401 6c05 5a05 6400  d.l.Z.d.d.l.Z.d.
 00000060: 6401 6c06 5a06 6403 6404 6c07 6d08 5a08  d.l.Z.d.d.l.m.Z.
 00000070: 6d09 5a09 6d0a 5a0a 0100 6403 6405 6c0b  m.Z.m.Z...d.d.l.
@@ -23,172 +23,195 @@
 00000160: 436f 6d70 696c 6553 7479 6c65 5368 6565  CompileStyleShee
 00000170: 744e 6302 0000 0000 0000 0000 0000 0002  tNc.............
 00000180: 0000 0003 0000 0003 0000 0073 1400 0000  ...........s....
 00000190: 7400 7401 7c00 8302 a002 7c01 a101 0100  t.t.|.....|.....
 000001a0: 6400 5300 2901 4e29 03da 0573 7570 6572  d.S.).N)...super
 000001b0: 720b 0000 00da 085f 5f69 6e69 745f 5f29  r......__init__)
 000001c0: 02da 0473 656c 66da 0670 6172 656e 74a9  ...self..parent.
-000001d0: 01da 095f 5f63 6c61 7373 5f5f a900 fa4d  ...__class__...M
-000001e0: 633a 5c75 7365 7273 5c6b 6962 6574 5c61  c:\users\kibet\a
-000001f0: 6e61 636f 6e64 6133 5c4c 6962 5c73 6974  naconda3\Lib\sit
-00000200: 652d 7061 636b 6167 6573 5c43 7573 746f  e-packages\Custo
-00000210: 6d5f 5769 6467 6574 732f 5173 732f 5361  m_Widgets/Qss/Sa
-00000220: 7373 436f 6d70 696c 6572 2e70 7972 0d00  ssCompiler.pyr..
-00000230: 0000 3500 0000 7302 0000 0000 017a 1a43  ..5...s......z.C
-00000240: 6f6d 7069 6c65 5374 796c 6553 6865 6574  ompileStyleSheet
-00000250: 2e5f 5f69 6e69 745f 5f63 0100 0000 0000  .__init__c......
-00000260: 0000 0000 0000 0e00 0000 0900 0000 4300  ..............C.
-00000270: 0000 7366 0200 0074 0083 007d 0174 016a  ..sf...t...}.t.j
-00000280: 02a0 0374 016a 02a0 0474 01a0 05a1 0064  ...t.j...t.....d
-00000290: 01a1 02a1 017d 0274 016a 02a0 067c 02a1  .....}.t.j...|..
-000002a0: 0173 3674 01a0 077c 02a1 0101 0074 016a  .s6t...|.....t.j
-000002b0: 02a0 0374 016a 02a0 0474 01a0 05a1 0064  ...t.j...t.....d
-000002c0: 02a1 02a1 017d 0374 016a 02a0 0374 016a  .....}.t.j...t.j
-000002d0: 02a0 0474 01a0 05a1 0064 03a1 02a1 017d  ...t.....d.....}
-000002e0: 0474 016a 02a0 0374 016a 02a0 0474 01a0  .t.j...t.j...t..
-000002f0: 05a1 0064 04a1 02a1 017d 0574 08a0 097c  ...d.....}.t...|
-00000300: 00a1 017d 0674 016a 02a0 067c 03a1 0173  ...}.t.j...|...s
-00000310: d674 0aa0 0b74 016a 02a0 0374 016a 02a0  .t...t.j...t.j..
-00000320: 0474 016a 02a0 0c74 0da1 0164 05a1 02a1  .t.j...t...d....
-00000330: 0174 016a 02a0 0374 016a 02a0 0474 01a0  .t.j...t.j...t..
-00000340: 05a1 0064 01a1 02a1 01a1 0201 0074 016a  ...d.........t.j
-00000350: 02a0 067c 04a1 0190 0173 2074 0aa0 0b74  ...|.....s t...t
-00000360: 016a 02a0 0374 016a 02a0 0474 016a 02a0  .j...t.j...t.j..
-00000370: 0c74 0da1 0164 06a1 02a1 0174 016a 02a0  .t...d.....t.j..
-00000380: 0374 016a 02a0 0474 01a0 05a1 0064 01a1  .t.j...t.....d..
-00000390: 02a1 01a1 0201 0074 016a 02a0 0374 016a  .......t.j...t.j
-000003a0: 02a0 0474 01a0 05a1 0064 07a1 02a1 017d  ...t.....d.....}
-000003b0: 0774 016a 02a0 067c 07a1 0190 0173 6674  .t.j...|.....sft
-000003c0: 0e7c 0764 0883 027d 0874 0f64 097c 0864  .|.d...}.t.d.|.d
-000003d0: 0a8d 0201 007c 08a0 10a1 0001 0074 11a0  .....|.......t..
-000003e0: 127c 037c 05a1 0201 0074 0e7c 0564 0b83  .|.|.....t.|.d..
-000003f0: 028f 147d 097c 00a0 137c 09a0 14a1 00a1  ...}.|...|......
-00000400: 0101 0057 0035 0051 0052 0058 0074 157c  ...W.5.Q.R.X.t.|
-00000410: 006a 1683 017d 0a7c 0a6a 176a 18a0 1974  .j...}.|.j.j...t
-00000420: 1a6a 1ba1 0101 007c 0a6a 176a 1ca0 197c  .j.....|.j.j...|
-00000430: 006a 1da1 0101 007c 0a6a 176a 1ea0 197c  .j.....|.j.j...|
-00000440: 006a 1fa1 0101 0074 157c 006a 2083 017d  .j.....t.|.j ..}
-00000450: 0b7c 0b6a 176a 18a0 1974 1a6a 1ba1 0101  .|.j.j...t.j....
-00000460: 007c 006a 2190 0272 047c 0b6a 176a 1ca0  .|.j!..r.|.j.j..
-00000470: 1964 0c64 0d84 00a1 0101 007c 0b6a 176a  .d.d.......|.j.j
-00000480: 1ea0 197c 006a 1fa1 0101 0074 08a0 227c  ...|.j.....t.."|
-00000490: 00a1 017d 0c74 237c 0c64 0e19 0083 017d  ...}.t#|.d.....}
-000004a0: 0d7c 01a0 2464 0fa1 017c 0d6b 0290 0273  .|..$d...|.k...s
-000004b0: 567c 0c64 0e19 0064 006b 0990 0272 567c  V|.d...d.k...rV|
-000004c0: 006a 25a0 267c 0aa1 0101 006e 0c7c 006a  .j%.&|.....n.|.j
-000004d0: 25a0 267c 0ba1 0101 0064 0053 0029 104e  %.&|.....d.S.).N
-000004e0: 5a03 5153 537a 0d51 5353 2f6d 6169 6e2e  Z.QSSz.QSS/main.
-000004f0: 7363 7373 7a10 5153 532f 5f73 7479 6c65  scssz.QSS/_style
-00000500: 732e 7363 7373 7a0c 5153 532f 6d61 696e  s.scssz.QSS/main
-00000510: 2e63 7373 7a09 6d61 696e 2e73 6373 737a  .cssz.main.scssz
-00000520: 0c5f 7374 796c 6573 2e73 6373 737a 1551  ._styles.scssz.Q
-00000530: 5353 2f64 6566 6175 6c74 5374 796c 652e  SS/defaultStyle.
-00000540: 7363 7373 da01 7761 bf01 0000 0a20 2020  scss..wa.....   
-00000550: 2020 2020 2020 2020 202f 2f3d 3d3d 3d3d           //=====
-00000560: 3d3d 3d3d 3d3d 3d3d 3d3d 3d3d 3d3d 3d3d  ================
-00000570: 3d3d 3d3d 3d3d 3d3d 3d3d 3d3d 3d3d 3d3d  ================
-00000580: 3d3d 3d3d 3d3d 3d3d 3d3d 3d3d 3d3d 2f2f  ==============//
-00000590: 0a20 2020 2020 2020 2020 2020 202f 2f20  .            // 
-000005a0: 4649 4c45 2041 5554 4f2d 4745 4e45 5241  FILE AUTO-GENERA
-000005b0: 5445 442e 2050 5554 2059 4f55 5220 4445  TED. PUT YOUR DE
-000005c0: 4641 554c 5420 5354 594c 4553 2048 4552  FAULT STYLES HER
-000005d0: 452e 200a 2020 2020 2020 2020 2020 2020  E. .            
-000005e0: 2f2f 2054 4845 5345 2053 5459 4c45 5320  // THESE STYLES 
-000005f0: 5749 4c4c 204f 5645 5249 4445 2054 4845  WILL OVERIDE THE
-00000600: 2054 4845 4d45 2053 5459 4c45 530a 2020   THEME STYLES.  
-00000610: 2020 2020 2020 2020 2020 2f2f 3d3d 3d3d            //====
-00000620: 3d3d 3d3d 3d3d 3d3d 3d3d 3d3d 3d3d 3d3d  ================
-00000630: 3d3d 3d3d 3d3d 3d3d 3d3d 3d3d 3d3d 3d3d  ================
-00000640: 3d3d 3d3d 3d3d 3d3d 3d3d 3d3d 3d3d 3d3d  ================
-00000650: 2f2f 0a20 2020 2020 2020 2020 2020 200a  //.            .
-00000660: 2020 2020 2020 2020 2020 2020 2f2f 3d3d              //==
-00000670: 3d3d 3d3d 3d3d 3d3d 3d3d 3d3d 3d3d 3d3d  ================
-00000680: 3d3d 3d3d 3d3d 3d3d 3d3d 3d3d 3d3d 3d3d  ================
-00000690: 3d3d 3d3d 3d3d 3d3d 3d3d 3d3d 3d3d 3d3d  ================
-000006a0: 3d2f 2f0a 2020 2020 2020 2020 2020 2020  =//.            
-000006b0: 2f2f 2045 4e44 202f 2f0a 2020 2020 2020  // END //.      
-000006c0: 2020 2020 2020 2f2f 3d3d 3d3d 3d3d 3d3d        //========
-000006d0: 3d3d 3d3d 3d3d 3d3d 3d3d 3d3d 3d3d 3d3d  ================
-000006e0: 3d3d 3d3d 3d3d 3d3d 3d3d 3d3d 3d3d 3d3d  ================
-000006f0: 3d3d 3d3d 3d3d 3d3d 3d3d 3d3d 2f2f 0a20  ============//. 
-00000700: 2020 2020 2020 2020 2020 2029 01da 0466             )...f
-00000710: 696c 65da 0172 6300 0000 0000 0000 0000  ile..rc.........
-00000720: 0000 0000 0000 0002 0000 0053 0000 0073  ...........S...s
-00000730: 0800 0000 7400 6401 8301 5300 2902 4e7a  ....t.d...S.).Nz
-00000740: 3861 6c6c 2069 636f 6e73 2068 6176 6520  8all icons have 
-00000750: 6265 656e 2063 6865 636b 6564 2061 6e64  been checked and
-00000760: 206d 6973 7369 6e67 2069 636f 6e73 2067   missing icons g
-00000770: 656e 6572 6174 6564 2129 01da 0570 7269  enerated!)...pri
-00000780: 6e74 7212 0000 0072 1200 0000 7212 0000  ntr....r....r...
-00000790: 0072 1300 0000 da08 3c6c 616d 6264 613e  .r......<lambda>
-000007a0: 7600 0000 f300 0000 007a 3543 6f6d 7069  v........z5Compi
-000007b0: 6c65 5374 796c 6553 6865 6574 2e61 7070  leStyleSheet.app
-000007c0: 6c79 436f 6d70 696c 6564 5361 7373 2e3c  lyCompiledSass.<
-000007d0: 6c6f 6361 6c73 3e2e 3c6c 616d 6264 613e  locals>.<lambda>
-000007e0: 7a0b 6963 6f6e 732d 636f 6c6f 727a 0b49  z.icons-colorz.I
-000007f0: 434f 4e53 2d43 4f4c 4f52 2927 da09 5153  CONS-COLOR)'..QS
-00000800: 6574 7469 6e67 73da 026f 73da 0470 6174  ettings..os..pat
-00000810: 68da 0761 6273 7061 7468 da04 6a6f 696e  h..abspath..join
-00000820: da06 6765 7463 7764 da06 6578 6973 7473  ..getcwd..exists
-00000830: da08 6d61 6b65 6469 7273 7204 0000 005a  ..makedirsr....Z
-00000840: 0f43 7265 6174 6556 6172 6961 626c 6573  .CreateVariables
-00000850: da06 7368 7574 696c da04 636f 7079 da07  ..shutil..copy..
-00000860: 6469 726e 616d 65da 085f 5f66 696c 655f  dirname..__file_
-00000870: 5fda 046f 7065 6e72 1700 0000 da05 636c  _..openr......cl
-00000880: 6f73 65da 0671 7473 6173 735a 1063 6f6d  ose..qtsassZ.com
-00000890: 7069 6c65 5f66 696c 656e 616d 655a 0d73  pile_filenameZ.s
-000008a0: 6574 5374 796c 6553 6865 6574 da04 7265  etStyleSheet..re
-000008b0: 6164 7209 0000 005a 1063 6f6d 7069 6c65  adr....Z.compile
-000008c0: 5361 7373 5468 656d 655a 0773 6967 6e61  SassThemeZ.signa
-000008d0: 6c73 da06 7265 7375 6c74 da07 636f 6e6e  ls..result..conn
-000008e0: 6563 7472 0a00 0000 5a0c 7072 696e 745f  ectr....Z.print_
-000008f0: 6f75 7470 7574 da08 6669 6e69 7368 6564  output..finished
-00000900: 5a07 7265 7374 6172 74da 0870 726f 6772  Z.restart..progr
-00000910: 6573 735a 1773 6173 7343 6f6d 7069 6c61  essZ.sassCompila
-00000920: 7469 6f6e 5072 6f67 7265 7373 5a0c 6d61  tionProgressZ.ma
-00000930: 6b65 416c 6c49 636f 6e73 5a15 7368 6f77  keAllIconsZ.show
-00000940: 4375 7374 6f6d 5769 6467 6574 734c 6f67  CustomWidgetsLog
-00000950: 735a 1367 6574 4375 7272 656e 7454 6865  sZ.getCurrentThe
-00000960: 6d65 496e 666f da03 7374 72da 0576 616c  meInfo..str..val
-00000970: 7565 5a17 6375 7374 6f6d 5769 6467 6574  ueZ.customWidget
-00000980: 7354 6872 6561 6470 6f6f 6cda 0573 7461  sThreadpool..sta
-00000990: 7274 290e 720e 0000 00da 0873 6574 7469  rt).r......setti
-000009a0: 6e67 735a 0b71 6373 735f 666f 6c64 6572  ngsZ.qcss_folder
-000009b0: 5a0e 6d61 696e 5f73 6173 735f 7061 7468  Z.main_sass_path
-000009c0: 5a10 7374 796c 6573 5f73 6173 735f 7061  Z.styles_sass_pa
-000009d0: 7468 5a08 6373 735f 7061 7468 5a0d 7661  thZ.css_pathZ.va
-000009e0: 7269 6162 6c65 7346 696c 655a 1164 6566  riablesFileZ.def
-000009f0: 6175 6c74 5f73 6373 735f 7061 7468 da01  ault_scss_path..
-00000a00: 66da 0363 7373 5a0b 6963 6f6e 7357 6f72  f..cssZ.iconsWor
-00000a10: 6b65 725a 0e61 6c6c 4963 6f6e 7357 6f72  kerZ.allIconsWor
-00000a20: 6b65 72da 0563 6f6c 6f72 5a0c 6e6f 726d  ker..colorZ.norm
-00000a30: 616c 5f63 6f6c 6f72 7212 0000 0072 1200  al_colorr....r..
-00000a40: 0000 7213 0000 00da 1161 7070 6c79 436f  ..r......applyCo
-00000a50: 6d70 696c 6564 5361 7373 4000 0000 7348  mpiledSass@...sH
-00000a60: 0000 0000 0106 021a 010c 010a 021a 011a  ................
-00000a70: 011a 020a 020c 013c 020e 013c 021a 010e  .......<...<....
-00000a80: 010a 0104 0902 f706 0b08 020c 020c 0118  ................
-00000a90: 070a 0110 0110 0110 030a 0110 0108 0112  ................
-00000aa0: 0110 020a 010c 011e 020e 027a 2343 6f6d  ...........z#Com
-00000ab0: 7069 6c65 5374 796c 6553 6865 6574 2e61  pileStyleSheet.a
-00000ac0: 7070 6c79 436f 6d70 696c 6564 5361 7373  pplyCompiledSass
-00000ad0: 2901 4e29 06da 085f 5f6e 616d 655f 5fda  ).N)...__name__.
-00000ae0: 0a5f 5f6d 6f64 756c 655f 5fda 0c5f 5f71  .__module__..__q
-00000af0: 7561 6c6e 616d 655f 5f72 0d00 0000 7235  ualname__r....r5
-00000b00: 0000 00da 0d5f 5f63 6c61 7373 6365 6c6c  .....__classcell
-00000b10: 5f5f 7212 0000 0072 1200 0000 7210 0000  __r....r....r...
-00000b20: 0072 1300 0000 720b 0000 0034 0000 0073  .r....r....4...s
-00000b30: 0400 0000 0801 0e0b 720b 0000 0029 13da  ........r....)..
-00000b40: 0373 7973 5a0b 7174 7079 2e51 7443 6f72  .sysZ.qtpy.QtCor
-00000b50: 655a 0a71 7470 792e 5174 4775 695a 0e71  eZ.qtpy.QtGuiZ.q
-00000b60: 7470 792e 5174 5769 6467 6574 7372 2800  tpy.QtWidgetsr(.
-00000b70: 0000 721b 0000 0072 2200 0000 5a0b 636f  ..r....r"...Z.co
-00000b80: 6c6f 7273 7973 7465 6d72 0400 0000 7205  lorsystemr....r.
-00000b90: 0000 0072 0600 0000 5a0d 5376 6754 6f50  ...r....Z.SvgToP
-00000ba0: 6e67 4963 6f6e 7372 0700 0000 5a0d 5769  ngIconsr....Z.Wi
-00000bb0: 6467 6574 7357 6f72 6b65 7272 0900 0000  dgetsWorkerr....
-00000bc0: 720a 0000 0072 1a00 0000 7231 0000 0072  r....r....r1...r
-00000bd0: 0b00 0000 7212 0000 0072 1200 0000 7212  ....r....r....r.
-00000be0: 0000 0072 1300 0000 da08 3c6d 6f64 756c  ...r......<modul
-00000bf0: 653e 0800 0000 7316 0000 0008 1208 0108  e>....s.........
-00000c00: 0108 0408 0308 0108 0214 010c 0410 0206  ................
-00000c10: 07                                       .
+000001d0: 01da 095f 5f63 6c61 7373 5f5f a900 fa47  ...__class__...G
+000001e0: 653a 5c53 7069 6e6e 2054 6173 6b5c 3070  e:\Spinn Task\0p
+000001f0: 6173 735c 3070 6173 732d 6170 702d 6d61  ass\0pass-app-ma
+00000200: 7374 6572 5c43 7573 746f 6d5f 5769 6467  ster\Custom_Widg
+00000210: 6574 735c 5173 735c 5361 7373 436f 6d70  ets\Qss\SassComp
+00000220: 696c 6572 2e70 7972 0d00 0000 3500 0000  iler.pyr....5...
+00000230: 7302 0000 0000 017a 1a43 6f6d 7069 6c65  s......z.Compile
+00000240: 5374 796c 6553 6865 6574 2e5f 5f69 6e69  StyleSheet.__ini
+00000250: 745f 5f63 0100 0000 0000 0000 0000 0000  t__c............
+00000260: 0f00 0000 0900 0000 4300 0000 73fa 0200  ........C...s...
+00000270: 0074 0083 007d 0174 016a 02a0 0374 016a  .t...}.t.j...t.j
+00000280: 02a0 0474 01a0 05a1 0064 01a1 02a1 017d  ...t.....d.....}
+00000290: 0274 016a 02a0 067c 02a1 0173 3674 01a0  .t.j...|...s6t..
+000002a0: 077c 02a1 0101 0074 016a 02a0 0374 016a  .|.....t.j...t.j
+000002b0: 02a0 0474 01a0 05a1 0064 02a1 02a1 017d  ...t.....d.....}
+000002c0: 0374 016a 02a0 0374 016a 02a0 0474 01a0  .t.j...t.j...t..
+000002d0: 05a1 0064 03a1 02a1 017d 0474 016a 02a0  ...d.....}.t.j..
+000002e0: 0374 016a 02a0 0474 01a0 05a1 0064 04a1  .t.j...t.....d..
+000002f0: 02a1 017d 0574 08a0 097c 00a1 017d 0674  ...}.t...|...}.t
+00000300: 016a 02a0 067c 03a1 0173 d674 0aa0 0b74  .j...|...s.t...t
+00000310: 016a 02a0 0374 016a 02a0 0474 016a 02a0  .j...t.j...t.j..
+00000320: 0c74 0da1 0164 05a1 02a1 0174 016a 02a0  .t...d.....t.j..
+00000330: 0374 016a 02a0 0474 01a0 05a1 0064 01a1  .t.j...t.....d..
+00000340: 02a1 01a1 0201 0074 016a 02a0 067c 04a1  .......t.j...|..
+00000350: 0190 0173 2074 0aa0 0b74 016a 02a0 0374  ...s t...t.j...t
+00000360: 016a 02a0 0474 016a 02a0 0c74 0da1 0164  .j...t.j...t...d
+00000370: 06a1 02a1 0174 016a 02a0 0374 016a 02a0  .....t.j...t.j..
+00000380: 0474 01a0 05a1 0064 01a1 02a1 01a1 0201  .t.....d........
+00000390: 0074 016a 02a0 0374 016a 02a0 0474 01a0  .t.j...t.j...t..
+000003a0: 05a1 0064 07a1 02a1 017d 0774 016a 02a0  ...d.....}.t.j..
+000003b0: 067c 07a1 0190 0173 6674 0e7c 0764 0883  .|.....sft.|.d..
+000003c0: 027d 0874 0f64 097c 0864 0a8d 0201 007c  .}.t.d.|.d.....|
+000003d0: 08a0 10a1 0001 0074 11a0 127c 037c 05a1  .......t...|.|..
+000003e0: 0201 0074 0e7c 0564 0b83 028f 147d 097c  ...t.|.d.....}.|
+000003f0: 00a0 137c 09a0 14a1 00a1 0101 0057 0035  ...|.........W.5
+00000400: 0051 0052 0058 0074 1583 007d 0a7c 0aa0  .Q.R.X.t...}.|..
+00000410: 1674 156a 1774 187c 006a 196a 1a83 01a1  .t.j.t.|.j.j....
+00000420: 0201 007c 0aa0 1674 156a 1b74 187c 006a  ...|...t.j.t.|.j
+00000430: 196a 1c83 01a1 0201 007c 0aa0 1674 156a  .j.......|...t.j
+00000440: 1d74 187c 006a 196a 1e83 01a1 0201 007c  .t.|.j.j.......|
+00000450: 0aa0 1674 156a 1f74 187c 006a 196a 1c83  ...t.j.t.|.j.j..
+00000460: 01a1 0201 007c 0aa0 1674 156a 2074 187c  .....|...t.j t.|
+00000470: 006a 196a 2183 01a1 0201 007c 0aa0 1674  .j.j!......|...t
+00000480: 156a 2274 187c 006a 196a 2383 01a1 0201  .j"t.|.j.j#.....
+00000490: 007c 00a0 247c 0aa1 0101 0074 257c 006a  .|..$|.....t%|.j
+000004a0: 2683 017d 0b7c 0b6a 276a 28a0 2974 2a6a  &..}.|.j'j(.)t*j
+000004b0: 2ba1 0101 007c 0b6a 276a 2ca0 297c 006a  +....|.j'j,.)|.j
+000004c0: 2da1 0101 007c 0b6a 276a 2ea0 297c 006a  -....|.j'j..)|.j
+000004d0: 2fa1 0101 0074 257c 006a 3083 017d 0c7c  /....t%|.j0..}.|
+000004e0: 0c6a 276a 28a0 2974 2a6a 2ba1 0101 007c  .j'j(.)t*j+....|
+000004f0: 006a 3190 0272 987c 0c6a 276a 2ca0 2964  .j1..r.|.j'j,.)d
+00000500: 0c64 0d84 00a1 0101 007c 0c6a 276a 2ea0  .d.......|.j'j..
+00000510: 297c 006a 2fa1 0101 0074 08a0 327c 00a1  )|.j/....t..2|..
+00000520: 017d 0d74 337c 0d64 0e19 0083 017d 0e7c  .}.t3|.d.....}.|
+00000530: 01a0 3464 0fa1 017c 0e6b 0290 0273 ea7c  ..4d...|.k...s.|
+00000540: 0d64 0e19 0064 006b 0990 0272 ea7c 006a  .d...d.k...r.|.j
+00000550: 35a0 367c 0ba1 0101 006e 0c7c 006a 35a0  5.6|.....n.|.j5.
+00000560: 367c 0ca1 0101 0064 0053 0029 104e 5a03  6|.....d.S.).NZ.
+00000570: 5153 537a 0d51 5353 2f6d 6169 6e2e 7363  QSSz.QSS/main.sc
+00000580: 7373 7a10 5153 532f 5f73 7479 6c65 732e  ssz.QSS/_styles.
+00000590: 7363 7373 7a0c 5153 532f 6d61 696e 2e63  scssz.QSS/main.c
+000005a0: 7373 7a09 6d61 696e 2e73 6373 737a 0c5f  ssz.main.scssz._
+000005b0: 7374 796c 6573 2e73 6373 737a 1551 5353  styles.scssz.QSS
+000005c0: 2f64 6566 6175 6c74 5374 796c 652e 7363  /defaultStyle.sc
+000005d0: 7373 da01 7761 bf01 0000 0a20 2020 2020  ss..wa.....     
+000005e0: 2020 2020 2020 202f 2f3d 3d3d 3d3d 3d3d         //=======
+000005f0: 3d3d 3d3d 3d3d 3d3d 3d3d 3d3d 3d3d 3d3d  ================
+00000600: 3d3d 3d3d 3d3d 3d3d 3d3d 3d3d 3d3d 3d3d  ================
+00000610: 3d3d 3d3d 3d3d 3d3d 3d3d 3d3d 2f2f 0a20  ============//. 
+00000620: 2020 2020 2020 2020 2020 202f 2f20 4649             // FI
+00000630: 4c45 2041 5554 4f2d 4745 4e45 5241 5445  LE AUTO-GENERATE
+00000640: 442e 2050 5554 2059 4f55 5220 4445 4641  D. PUT YOUR DEFA
+00000650: 554c 5420 5354 594c 4553 2048 4552 452e  ULT STYLES HERE.
+00000660: 200a 2020 2020 2020 2020 2020 2020 2f2f   .            //
+00000670: 2054 4845 5345 2053 5459 4c45 5320 5749   THESE STYLES WI
+00000680: 4c4c 204f 5645 5249 4445 2054 4845 2054  LL OVERIDE THE T
+00000690: 4845 4d45 2053 5459 4c45 530a 2020 2020  HEME STYLES.    
+000006a0: 2020 2020 2020 2020 2f2f 3d3d 3d3d 3d3d          //======
+000006b0: 3d3d 3d3d 3d3d 3d3d 3d3d 3d3d 3d3d 3d3d  ================
+000006c0: 3d3d 3d3d 3d3d 3d3d 3d3d 3d3d 3d3d 3d3d  ================
+000006d0: 3d3d 3d3d 3d3d 3d3d 3d3d 3d3d 3d3d 2f2f  ==============//
+000006e0: 0a20 2020 2020 2020 2020 2020 200a 2020  .            .  
+000006f0: 2020 2020 2020 2020 2020 2f2f 3d3d 3d3d            //====
+00000700: 3d3d 3d3d 3d3d 3d3d 3d3d 3d3d 3d3d 3d3d  ================
+00000710: 3d3d 3d3d 3d3d 3d3d 3d3d 3d3d 3d3d 3d3d  ================
+00000720: 3d3d 3d3d 3d3d 3d3d 3d3d 3d3d 3d3d 3d2f  ===============/
+00000730: 2f0a 2020 2020 2020 2020 2020 2020 2f2f  /.            //
+00000740: 2045 4e44 202f 2f0a 2020 2020 2020 2020   END //.        
+00000750: 2020 2020 2f2f 3d3d 3d3d 3d3d 3d3d 3d3d      //==========
+00000760: 3d3d 3d3d 3d3d 3d3d 3d3d 3d3d 3d3d 3d3d  ================
+00000770: 3d3d 3d3d 3d3d 3d3d 3d3d 3d3d 3d3d 3d3d  ================
+00000780: 3d3d 3d3d 3d3d 3d3d 3d3d 2f2f 0a20 2020  ==========//.   
+00000790: 2020 2020 2020 2020 2029 01da 0466 696c           )...fil
+000007a0: 65da 0172 6300 0000 0000 0000 0000 0000  e..rc...........
+000007b0: 0000 0000 0002 0000 0053 0000 0073 0800  .........S...s..
+000007c0: 0000 7400 6401 8301 5300 2902 4e7a 3861  ..t.d...S.).Nz8a
+000007d0: 6c6c 2069 636f 6e73 2068 6176 6520 6265  ll icons have be
+000007e0: 656e 2063 6865 636b 6564 2061 6e64 206d  en checked and m
+000007f0: 6973 7369 6e67 2069 636f 6e73 2067 656e  issing icons gen
+00000800: 6572 6174 6564 2129 01da 0570 7269 6e74  erated!)...print
+00000810: 7212 0000 0072 1200 0000 7212 0000 0072  r....r....r....r
+00000820: 1300 0000 da08 3c6c 616d 6264 613e 9000  ......<lambda>..
+00000830: 0000 f300 0000 007a 3543 6f6d 7069 6c65  .......z5Compile
+00000840: 5374 796c 6553 6865 6574 2e61 7070 6c79  StyleSheet.apply
+00000850: 436f 6d70 696c 6564 5361 7373 2e3c 6c6f  CompiledSass.<lo
+00000860: 6361 6c73 3e2e 3c6c 616d 6264 613e 7a0b  cals>.<lambda>z.
+00000870: 6963 6f6e 732d 636f 6c6f 727a 0b49 434f  icons-colorz.ICO
+00000880: 4e53 2d43 4f4c 4f52 2937 da09 5153 6574  NS-COLOR)7..QSet
+00000890: 7469 6e67 73da 026f 73da 0470 6174 68da  tings..os..path.
+000008a0: 0761 6273 7061 7468 da04 6a6f 696e da06  .abspath..join..
+000008b0: 6765 7463 7764 da06 6578 6973 7473 da08  getcwd..exists..
+000008c0: 6d61 6b65 6469 7273 7204 0000 005a 0f43  makedirsr....Z.C
+000008d0: 7265 6174 6556 6172 6961 626c 6573 da06  reateVariables..
+000008e0: 7368 7574 696c da04 636f 7079 da07 6469  shutil..copy..di
+000008f0: 726e 616d 65da 085f 5f66 696c 655f 5fda  rname..__file__.
+00000900: 046f 7065 6e72 1700 0000 da05 636c 6f73  .openr......clos
+00000910: 65da 0671 7473 6173 735a 1063 6f6d 7069  e..qtsassZ.compi
+00000920: 6c65 5f66 696c 656e 616d 65da 0d73 6574  le_filename..set
+00000930: 5374 796c 6553 6865 6574 da04 7265 6164  StyleSheet..read
+00000940: da08 5150 616c 6574 7465 da08 7365 7443  ..QPalette..setC
+00000950: 6f6c 6f72 da0a 4261 636b 6772 6f75 6e64  olor..Background
+00000960: da06 5143 6f6c 6f72 da05 7468 656d 655a  ..QColor..themeZ
+00000970: 1243 4f4c 4f52 5f42 4143 4b47 524f 554e  .COLOR_BACKGROUN
+00000980: 445f 31da 0454 6578 745a 0c43 4f4c 4f52  D_1..TextZ.COLOR
+00000990: 5f54 4558 545f 31da 0642 7574 746f 6e5a  _TEXT_1..ButtonZ
+000009a0: 1243 4f4c 4f52 5f42 4143 4b47 524f 554e  .COLOR_BACKGROUN
+000009b0: 445f 33da 0a42 7574 746f 6e54 6578 74da  D_3..ButtonText.
+000009c0: 0948 6967 686c 6967 6874 5a12 434f 4c4f  .HighlightZ.COLO
+000009d0: 525f 4241 434b 4752 4f55 4e44 5f36 da0f  R_BACKGROUND_6..
+000009e0: 4869 6768 6c69 6768 7465 6454 6578 745a  HighlightedTextZ
+000009f0: 0e43 4f4c 4f52 5f41 4343 454e 545f 31da  .COLOR_ACCENT_1.
+00000a00: 0a73 6574 5061 6c65 7474 6572 0900 0000  .setPaletter....
+00000a10: da10 636f 6d70 696c 6553 6173 7354 6865  ..compileSassThe
+00000a20: 6d65 5a07 7369 676e 616c 73da 0672 6573  meZ.signals..res
+00000a30: 756c 74da 0763 6f6e 6e65 6374 720a 0000  ult..connectr...
+00000a40: 005a 0c70 7269 6e74 5f6f 7574 7075 74da  .Z.print_output.
+00000a50: 0866 696e 6973 6865 64da 0772 6573 7461  .finished..resta
+00000a60: 7274 da08 7072 6f67 7265 7373 da17 7361  rt..progress..sa
+00000a70: 7373 436f 6d70 696c 6174 696f 6e50 726f  ssCompilationPro
+00000a80: 6772 6573 73da 0c6d 616b 6541 6c6c 4963  gress..makeAllIc
+00000a90: 6f6e 73da 1573 686f 7743 7573 746f 6d57  ons..showCustomW
+00000aa0: 6964 6765 7473 4c6f 6773 5a13 6765 7443  idgetsLogsZ.getC
+00000ab0: 7572 7265 6e74 5468 656d 6549 6e66 6fda  urrentThemeInfo.
+00000ac0: 0373 7472 da05 7661 6c75 65da 1763 7573  .str..value..cus
+00000ad0: 746f 6d57 6964 6765 7473 5468 7265 6164  tomWidgetsThread
+00000ae0: 706f 6f6c da05 7374 6172 7429 0f72 0e00  pool..start).r..
+00000af0: 0000 da08 7365 7474 696e 6773 5a0b 7163  ....settingsZ.qc
+00000b00: 7373 5f66 6f6c 6465 725a 0e6d 6169 6e5f  ss_folderZ.main_
+00000b10: 7361 7373 5f70 6174 685a 1073 7479 6c65  sass_pathZ.style
+00000b20: 735f 7361 7373 5f70 6174 68da 0863 7373  s_sass_path..css
+00000b30: 5f70 6174 685a 0d76 6172 6961 626c 6573  _pathZ.variables
+00000b40: 4669 6c65 5a11 6465 6661 756c 745f 7363  FileZ.default_sc
+00000b50: 7373 5f70 6174 68da 0166 da03 6373 73da  ss_path..f..css.
+00000b60: 0770 616c 6574 7465 5a0b 6963 6f6e 7357  .paletteZ.iconsW
+00000b70: 6f72 6b65 725a 0e61 6c6c 4963 6f6e 7357  orkerZ.allIconsW
+00000b80: 6f72 6b65 72da 0563 6f6c 6f72 5a0c 6e6f  orker..colorZ.no
+00000b90: 726d 616c 5f63 6f6c 6f72 7212 0000 0072  rmal_colorr....r
+00000ba0: 1200 0000 7213 0000 00da 1161 7070 6c79  ....r......apply
+00000bb0: 436f 6d70 696c 6564 5361 7373 4000 0000  CompiledSass@...
+00000bc0: 7358 0000 0000 0106 021a 010c 010a 021a  sX..............
+00000bd0: 011a 011a 020a 020c 013c 020e 013c 021a  .........<...<..
+00000be0: 010e 010a 0104 0902 f706 0b08 020c 020c  ................
+00000bf0: 0118 0306 0316 0316 0316 0316 0316 0316  ................
+00000c00: 030a 090a 0110 0110 0110 030a 0110 0108  ................
+00000c10: 0112 0110 020a 010c 011e 020e 027a 2343  .............z#C
+00000c20: 6f6d 7069 6c65 5374 796c 6553 6865 6574  ompileStyleSheet
+00000c30: 2e61 7070 6c79 436f 6d70 696c 6564 5361  .applyCompiledSa
+00000c40: 7373 2901 4e29 06da 085f 5f6e 616d 655f  ss).N)...__name_
+00000c50: 5fda 0a5f 5f6d 6f64 756c 655f 5fda 0c5f  _..__module__.._
+00000c60: 5f71 7561 6c6e 616d 655f 5f72 0d00 0000  _qualname__r....
+00000c70: 7249 0000 00da 0d5f 5f63 6c61 7373 6365  rI.....__classce
+00000c80: 6c6c 5f5f 7212 0000 0072 1200 0000 7210  ll__r....r....r.
+00000c90: 0000 0072 1300 0000 720b 0000 0034 0000  ...r....r....4..
+00000ca0: 0073 0400 0000 0801 0e0b 720b 0000 0029  .s........r....)
+00000cb0: 13da 0373 7973 da0b 7174 7079 2e51 7443  ...sys..qtpy.QtC
+00000cc0: 6f72 65da 0a71 7470 792e 5174 4775 69da  ore..qtpy.QtGui.
+00000cd0: 0e71 7470 792e 5174 5769 6467 6574 7372  .qtpy.QtWidgetsr
+00000ce0: 2800 0000 721b 0000 0072 2200 0000 5a0b  (...r....r"...Z.
+00000cf0: 636f 6c6f 7273 7973 7465 6d72 0400 0000  colorsystemr....
+00000d00: 7205 0000 0072 0600 0000 5a0d 5376 6754  r....r....Z.SvgT
+00000d10: 6f50 6e67 4963 6f6e 7372 0700 0000 da0d  oPngIconsr......
+00000d20: 5769 6467 6574 7357 6f72 6b65 7272 0900  WidgetsWorkerr..
+00000d30: 0000 720a 0000 0072 1a00 0000 7243 0000  ..r....r....rC..
+00000d40: 0072 0b00 0000 7212 0000 0072 1200 0000  .r....r....r....
+00000d50: 7212 0000 0072 1300 0000 da08 3c6d 6f64  r....r......<mod
+00000d60: 756c 653e 0800 0000 7316 0000 0008 1208  ule>....s.......
+00000d70: 0108 0108 0408 0308 0108 0214 010c 0410  ................
+00000d80: 0206 07                                  ...
```

### Comparing `QT-PyQt-PySide-Custom-Widgets-0.6.5/Custom_Widgets/Qss/__pycache__/SvgToPngIcons.cpython-310.pyc` & `QT-PyQt-PySide-Custom-Widgets-0.6.6/Custom_Widgets/Qss/__pycache__/SvgToPngIcons.cpython-310.pyc`

 * *Files identical despite different names*

### Comparing `QT-PyQt-PySide-Custom-Widgets-0.6.5/Custom_Widgets/Qss/__pycache__/SvgToPngIcons.cpython-38.pyc` & `QT-PyQt-PySide-Custom-Widgets-0.6.6/Custom_Widgets/Qss/__pycache__/SvgToPngIcons.cpython-38.pyc`

 * *Format-specific differences are supported for Python .pyc files but no file-specific differences were detected; falling back to a binary diff. file(1) reports: Byte-compiled Python module for CPython 3.8, timestamp-based, .py timestamp: Wed Jun 21 20:45:30 2023 UTC, .py size: 14615 bytes*

 * *Could not decompile bytecode: bad marshal data (unknown type code)*

 * *Files 8% similar despite different names*

```diff
@@ -1,418 +1,455 @@
-00000000: 550d 0d0a 0000 0000 6a61 9364 1739 0000  U.......ja.d.9..
+00000000: 550d 0d0a 0000 0000 bbdf 9664 f23c 0000  U..........d.<..
 00000010: e300 0000 0000 0000 0000 0000 0000 0000  ................
-00000020: 0003 0000 0040 0000 0073 6800 0000 6400  .....@...sh...d.
+00000020: 0003 0000 0040 0000 0073 8000 0000 6400  .....@...s....d.
 00000030: 6401 6c00 5a00 6400 6401 6c01 5a01 6400  d.l.Z.d.d.l.Z.d.
 00000040: 6401 6c02 5a02 6400 6401 6c03 5a03 6400  d.l.Z.d.d.l.Z.d.
-00000050: 6401 6c04 5a04 6400 6402 6c05 6d06 5a06  d.l.Z.d.d.l.m.Z.
-00000060: 0100 6400 6403 6c07 6d08 5a08 0100 6400  ..d.d.l.m.Z...d.
-00000070: 6401 6c09 5a09 6404 6405 6c0a 5400 650b  d.l.Z.d.d.l.T.e.
-00000080: 8300 5a0c 4700 6406 6407 8400 6407 8302  ..Z.G.d.d...d...
-00000090: 5a0d 6401 5300 2908 e900 0000 004e 2901  Z.d.S.)......N).
-000000a0: da08 7572 6c70 6172 7365 2901 da04 5061  ..urlparse)...Pa
-000000b0: 7468 e901 0000 0029 01da 012a 6300 0000  th.....)...*c...
-000000c0: 0000 0000 0000 0000 0000 0000 0003 0000  ................
-000000d0: 0000 0000 0073 3000 0000 6500 5a01 6400  .....s0...e.Z.d.
-000000e0: 5a02 6401 5a03 8700 6601 6402 6403 8408  Z.d.Z...f.d.d...
-000000f0: 5a04 6404 6405 8400 5a05 6406 6407 8400  Z.d.d...Z.d.d...
-00000100: 5a06 8700 0400 5a07 5300 2908 da11 4e65  Z.....Z.S.)...Ne
-00000110: 7749 636f 6e73 4765 6e65 7261 746f 727a  wIconsGeneratorz
-00000120: 1f64 6f63 7374 7269 6e67 2066 6f72 204e  .docstring for N
-00000130: 6577 4963 6f6e 7347 656e 6572 6174 6f72  ewIconsGenerator
-00000140: 6302 0000 0000 0000 0000 0000 0002 0000  c...............
-00000150: 0003 0000 0003 0000 0073 1800 0000 7400  .........s....t.
-00000160: 7401 7c00 8302 a002 a100 0100 7c01 7c00  t.|.........|.|.
-00000170: 5f03 6400 5300 2901 4e29 04da 0573 7570  _.d.S.).N)...sup
-00000180: 6572 7206 0000 00da 085f 5f69 6e69 745f  err......__init_
-00000190: 5fda 0361 7267 2902 da04 7365 6c66 7209  _..arg)...selfr.
-000001a0: 0000 00a9 01da 095f 5f63 6c61 7373 5f5f  .......__class__
-000001b0: a900 fa4e 633a 5c75 7365 7273 5c6b 6962  ...Nc:\users\kib
-000001c0: 6574 5c61 6e61 636f 6e64 6133 5c4c 6962  et\anaconda3\Lib
-000001d0: 5c73 6974 652d 7061 636b 6167 6573 5c43  \site-packages\C
-000001e0: 7573 746f 6d5f 5769 6467 6574 732f 5173  ustom_Widgets/Qs
-000001f0: 732f 5376 6754 6f50 6e67 4963 6f6e 732e  s/SvgToPngIcons.
-00000200: 7079 7208 0000 0011 0000 0073 0400 0000  pyr........s....
-00000210: 0001 0e01 7a1a 4e65 7749 636f 6e73 4765  ....z.NewIconsGe
-00000220: 6e65 7261 746f 722e 5f5f 696e 6974 5f5f  nerator.__init__
-00000230: 6302 0000 0000 0000 0000 0000 0023 0000  c............#..
-00000240: 000c 0000 0043 0000 0073 4607 0000 7400  .....C...sF...t.
-00000250: 8300 7d02 7401 6a02 a003 7404 a101 7d03  ..}.t.j...t...}.
-00000260: 7401 6a02 a005 7c03 6401 a102 7d04 6700  t.j...|.d...}.g.
-00000270: 7d05 7406 a007 7c00 a101 7d06 6402 7d07  }.t...|...}.d.}.
-00000280: 7408 7c06 6403 1900 8301 7d08 7409 7c08  t.|.d.....}.t.|.
-00000290: 6404 8302 7d09 7409 7c08 6405 8302 7d0a  d...}.t.|.d...}.
-000002a0: 7c08 a00a 6406 6407 a102 7d0b 7401 6a02  |...d.d...}.t.j.
-000002b0: a00b 7401 6a02 a005 7401 a00c a100 6408  ..t.j...t.....d.
-000002c0: 7c0b 1700 a102 a101 7d0c 7401 6a02 a00b  |.......}.t.j...
-000002d0: 7401 6a02 a005 7401 a00c a100 6409 a102  t.j...t.....d...
-000002e0: a101 7d0d 7c02 a00d 640a a101 6400 6b08  ..}.|...d...d.k.
-000002f0: 72da 7406 a007 7c00 a101 7d0e 7401 6a02  r.t...|...}.t.j.
-00000300: a00b 7401 6a02 a005 7401 a00c a100 6408  ..t.j...t.....d.
-00000310: 7c0e 6403 1900 a00a 6406 6407 a102 1700  |.d.....d.d.....
-00000320: a102 a101 7d0f 6e2c 7401 6a02 a00b 7401  ....}.n,t.j...t.
-00000330: 6a02 a005 7401 a00c a100 6408 7c02 a00d  j...t.....d.|...
-00000340: 640a a101 a00a 6406 6407 a102 1700 a102  d.....d.d.......
-00000350: a101 7d0f 7c02 a00d 640a a101 7c08 6b02  ..}.|...d...|.k.
-00000360: 9007 7336 7c06 6403 1900 6400 6b09 9007  ..s6|.d...d.k...
-00000370: 7236 7c00 6a0e 9001 7248 740f 640b 7c02  r6|.j...rHt.d.|.
-00000380: a00d 640a a101 640c 7c08 8304 0100 740f  ..d...d.|.....t.
-00000390: 640d 8301 0100 7401 a010 7c04 a101 4400  d.....t...|...D.
-000003a0: 5d2c 5c03 7d10 7d11 7d12 7c12 4400 5d1a  ],\.}.}.}.|.D.].
-000003b0: 7d13 7c05 a011 7401 6a02 a005 7c10 7c13  }.|...t.j...|.|.
-000003c0: a102 a101 0100 9001 7160 9001 7152 7412  ........q`..qRt.
-000003d0: 7c05 8301 7d14 7c05 4400 9001 5d26 7d15  |...}.|.D...]&}.
-000003e0: 7401 6a02 a013 7414 7c15 8301 6a02 a101  t.j...t.|...j...
-000003f0: a00a 640e 640f a102 7d16 7401 6a02 a015  ..d.d...}.t.j...
-00000400: 7401 6a02 a005 7c0d 7c16 a102 a101 9001  t.j...|.|.......
-00000410: 72f2 7401 6a02 a015 7401 6a02 a005 7c0f  r.t.j...t.j...|.
-00000420: 7c16 a102 a101 9001 73f2 7416 a017 7401  |.......s.t...t.
-00000430: 6a02 a005 7c0d 7c16 a102 7c0f a102 0100  j...|.|...|.....
-00000440: 7401 6a02 a013 7414 7c15 8301 6a02 a101  t.j...t.|...j...
-00000450: a00a 640e 6410 a102 7d16 7401 6a02 a015  ..d.d...}.t.j...
-00000460: 7401 6a02 a005 7c0d 7c16 a102 a101 9002  t.j...|.|.......
-00000470: 7252 7401 6a02 a015 7401 6a02 a005 7c0f  rRt.j...t.j...|.
-00000480: 7c16 a102 a101 9002 7352 7416 a017 7401  |.......sRt...t.
-00000490: 6a02 a005 7c0d 7c16 a102 7c0f a102 0100  j...|.|...|.....
-000004a0: 7401 6a02 a013 7414 7c15 8301 6a02 a101  t.j...t.|...j...
-000004b0: a00a 640e 6411 a102 7d16 7401 6a02 a015  ..d.d...}.t.j...
-000004c0: 7401 6a02 a005 7c0d 7c16 a102 a101 9001  t.j...|.|.......
-000004d0: 728c 7401 6a02 a015 7401 6a02 a005 7c0f  r.t.j...t.j...|.
-000004e0: 7c16 a102 a101 9001 738c 7416 a017 7401  |.......s.t...t.
-000004f0: 6a02 a005 7c0d 7c16 a102 7c0f a102 0100  j...|.|...|.....
-00000500: 9001 718c 7c05 4400 9002 5d92 7d15 7418  ..q.|.D...].}.t.
-00000510: 6a19 7c15 6412 6413 6414 8d03 8fba 7d17  j.|.d.d.d.....}.
-00000520: 7c17 a01a a100 7d18 7c18 a00a 7c07 7c08  |.....}.|...|.|.
-00000530: a102 7d19 7408 a01b 7c19 a101 7d1a 7401  ..}.t...|...}.t.
-00000540: 6a02 a013 7414 7c15 8301 6a02 a101 a00a  j...t.|...j.....
-00000550: 640e 640f a102 7d16 7401 6a02 a00b 7401  d.d...}.t.j...t.
-00000560: 6a02 a005 7c0c 7c16 a102 a101 7d04 7401  j...|.|.....}.t.
-00000570: 6a02 a015 7c0c a101 9003 7338 7401 a01c  j...|.....s8t...
-00000580: 7c0c a101 0100 7401 6a02 a015 7c04 a101  |.....t.j...|...
-00000590: 9003 7386 7a12 741d 6a1e 7c1a 7c04 6415  ..s.z.t.j.|.|.d.
-000005a0: 8d02 0100 5700 6e2c 0400 741f 6b0a 9003  ....W.n,..t.k...
-000005b0: 7284 0100 7d1b 0100 7a0c 740f 7c1b 8301  r...}...z.t.|...
-000005c0: 0100 5700 3500 6400 7d1b 7e1b 5800 5900  ..W.5.d.}.~.X.Y.
-000005d0: 6e02 5800 5700 3500 5100 5200 5800 7418  n.X.W.5.Q.R.X.t.
-000005e0: 6a19 7c15 6412 6413 6414 8d03 8fba 7d17  j.|.d.d.d.....}.
-000005f0: 7c17 a01a a100 7d18 7c18 a00a 7c07 7c09  |.....}.|...|.|.
-00000600: a102 7d19 7408 a01b 7c19 a101 7d1a 7401  ..}.t...|...}.t.
-00000610: 6a02 a013 7414 7c15 8301 6a02 a101 a00a  j...t.|...j.....
-00000620: 640e 6410 a102 7d16 7401 6a02 a00b 7401  d.d...}.t.j...t.
-00000630: 6a02 a005 7c0c 7c16 a102 a101 7d04 7401  j...|.|.....}.t.
-00000640: 6a02 a015 7c0c a101 9004 7308 7401 a01c  j...|.....s.t...
-00000650: 7c0c a101 0100 7401 6a02 a015 7c04 a101  |.....t.j...|...
-00000660: 9004 7356 7a12 741d 6a1e 7c1a 7c04 6415  ..sVz.t.j.|.|.d.
-00000670: 8d02 0100 5700 6e2c 0400 741f 6b0a 9004  ....W.n,..t.k...
-00000680: 7254 0100 7d1b 0100 7a0c 740f 7c1b 8301  rT..}...z.t.|...
-00000690: 0100 5700 3500 6400 7d1b 7e1b 5800 5900  ..W.5.d.}.~.X.Y.
-000006a0: 6e02 5800 5700 3500 5100 5200 5800 7418  n.X.W.5.Q.R.X.t.
-000006b0: 6a19 7c15 6412 6413 6414 8d03 8fba 7d17  j.|.d.d.d.....}.
-000006c0: 7c17 a01a a100 7d18 7c18 a00a 7c07 7c0a  |.....}.|...|.|.
-000006d0: a102 7d19 7408 a01b 7c19 a101 7d1a 7401  ..}.t...|...}.t.
-000006e0: 6a02 a013 7414 7c15 8301 6a02 a101 a00a  j...t.|...j.....
-000006f0: 640e 6411 a102 7d16 7401 6a02 a00b 7401  d.d...}.t.j...t.
-00000700: 6a02 a005 7c0c 7c16 a102 a101 7d04 7401  j...|.|.....}.t.
-00000710: 6a02 a015 7c0c a101 9004 73d8 7401 a01c  j...|.....s.t...
-00000720: 7c0c a101 0100 7401 6a02 a015 7c04 a101  |.....t.j...|...
-00000730: 9005 7326 7a12 741d 6a1e 7c1a 7c04 6415  ..s&z.t.j.|.|.d.
-00000740: 8d02 0100 5700 6e2c 0400 741f 6b0a 9005  ....W.n,..t.k...
-00000750: 7224 0100 7d1b 0100 7a0c 740f 7c1b 8301  r$..}...z.t.|...
-00000760: 0100 5700 3500 6400 7d1b 7e1b 5800 5900  ..W.5.d.}.~.X.Y.
-00000770: 6e02 5800 5700 3500 5100 5200 5800 7c01  n.X.W.5.Q.R.X.|.
-00000780: a020 7421 7c05 a022 7c15 a101 7c14 1b00  . t!|.."|...|...
-00000790: 6416 1400 8301 a101 0100 9002 71ba 7c0c  d...........q.|.
-000007a0: 7d1c 7c0d 7d1d 7401 a023 7c1c a101 7d1e  }.|.}.t..#|...}.
-000007b0: 7401 6a02 a015 7c0d a101 9005 737c 7401  t.j...|.....s|t.
-000007c0: a01c 7c0d a101 0100 6e18 7401 6a02 a015  ..|.....n.t.j...
-000007d0: 7c0d a101 9005 7394 7401 a01c 7c0d a101  |.....s.t...|...
-000007e0: 0100 6417 7d1f 7c1e 4400 5d9e 7d20 7401  ..d.}.|.D.].} t.
-000007f0: 6a24 6418 6b02 9005 72c4 7416 a025 7401  j$d.k...r.t..%t.
-00000800: 6a02 a005 7c1c 7c20 a102 7c1d a102 0100  j...|.| ..|.....
-00000810: 6e56 7a1a 7416 a017 7401 6a02 a005 7c1c  nVz.t...t.j...|.
-00000820: 7c20 a102 7c1d a102 0100 5700 6e3a 0400  | ..|.....W.n:..
-00000830: 741f 6b0a 9006 7218 0100 7d1b 0100 7a1a  t.k...r...}...z.
-00000840: 7416 a025 7401 6a02 a005 7c1c 7c20 a102  t..%t.j...|.| ..
-00000850: 7c1d a102 0100 5700 3500 6400 7d1b 7e1b  |.....W.5.d.}.~.
-00000860: 5800 5900 6e02 5800 7c1f 6419 3700 7d1f  X.Y.n.X.|.d.7.}.
-00000870: 7c01 a020 7421 7c1f 7c14 1b00 6416 1400  |.. t!|.|...d...
-00000880: 8301 a101 0100 9005 719c 7401 6a02 a00b  ........q.t.j...
-00000890: 7401 6a02 a005 7401 a00c a100 641a a102  t.j...t.....d...
-000008a0: a101 7d21 7401 6a02 a015 7c21 a101 9006  ..}!t.j...|!....
-000008b0: 73a0 7416 a025 7401 6a02 a00b 7401 6a02  s.t..%t.j...t.j.
-000008c0: a005 7401 6a02 a003 7404 a101 641b a102  ..t.j...t...d...
-000008d0: a101 7401 6a02 a00b 7401 6a02 a005 7401  ..t.j...t.j...t.
-000008e0: a00c a100 641c a102 a101 a102 0100 7c21  ....d.........|!
-000008f0: a00a 641d 641e a102 7d22 7c22 a00a 6408  ..d.d...}"|"..d.
-00000900: 6407 a102 7d22 7c22 a00a 641f 6407 a102  d...}"|"..d.d...
-00000910: 7d22 7c22 a00a 6420 6421 a102 7d22 7a36  }"|"..d d!..}"z6
-00000920: 7c02 a026 640a 7c08 a102 0100 7401 a027  |..&d.|.....t..'
-00000930: 6422 7c21 1700 6423 1700 7c22 1700 6424  d"|!..d#..|"..d$
-00000940: 1700 a101 0100 7c02 a026 640a 7c08 a102  ......|..&d.|...
-00000950: 0100 5700 6e2c 0400 741f 6b0a 9007 7232  ..W.n,..t.k...r2
-00000960: 0100 7d1b 0100 7a0c 740f 6425 8301 0100  ..}...z.t.d%....
-00000970: 5700 3500 6400 7d1b 7e1b 5800 5900 6e02  W.5.d.}.~.X.Y.n.
-00000980: 5800 6e0c 7428 a029 7c00 7c01 a102 0100  X.n.t(.)|.|.....
-00000990: 6400 5300 2926 4efa 1269 636f 6e73 2f6f  d.S.)&N..icons/o
-000009a0: 7269 6769 6e61 6c5f 7376 67fa 0423 6666  riginal_svg..#ff
-000009b0: 667a 0b69 636f 6e73 2d63 6f6c 6f72 e700  fz.icons-color..
-000009c0: 0000 0000 00f8 3fe7 0000 0000 0000 e03f  ......?........?
-000009d0: fa01 23da 00fa 0451 5353 2ffa 0951 5353  ..#....QSS/..QSS
-000009e0: 2f49 636f 6e73 fa0b 4943 4f4e 532d 434f  /Icons..ICONS-CO
-000009f0: 4c4f 527a 1443 7572 7265 6e74 2069 636f  LORz.Current ico
-00000a00: 6e73 2063 6f6c 6f72 207a 0f4e 6577 2069  ns color z.New i
-00000a10: 636f 6e73 2063 6f6c 6f72 7a40 4765 6e65  cons colorz@Gene
-00000a20: 7261 7469 6e67 2069 636f 6e73 2066 6f72  rating icons for
-00000a30: 2079 6f75 7220 7468 656d 652c 2070 6c65   your theme, ple
-00000a40: 6173 6520 7761 6974 2e20 5468 6973 206d  ase wait. This m
-00000a50: 6179 2074 616b 6520 6c6f 6e67 fa04 2e73  ay take long...s
-00000a60: 7667 fa04 2e70 6e67 fa0a 5f66 6f63 7573  vg...png.._focus
-00000a70: 2e70 6e67 fa0d 5f64 6973 6162 6c65 642e  .png.._disabled.
-00000a80: 706e 67fa 0575 7466 2d38 da06 6967 6e6f  png..utf-8..igno
-00000a90: 7265 a902 da08 656e 636f 6469 6e67 da06  re....encoding..
-00000aa0: 6572 726f 7273 a902 5a0a 6279 7465 7374  errors..Z.bytest
-00000ab0: 7269 6e67 5a08 7772 6974 655f 746f e964  ringZ.write_to.d
-00000ac0: 0000 0072 0100 0000 da02 6e74 7204 0000  ...r......ntr...
-00000ad0: 007a 1551 5353 2f51 5353 5f52 6573 6f75  .z.QSS/QSS_Resou
-00000ae0: 7263 6573 2e71 7263 7a11 5153 535f 5265  rces.qrcz.QSS_Re
-00000af0: 736f 7572 6365 732e 7172 635a 0351 5353  sources.qrcZ.QSS
-00000b00: 7a04 2e71 7263 7a03 2e70 797a 0451 5353  z..qrcz..pyz.QSS
-00000b10: 5c5a 0d51 5353 5f52 6573 6f75 7263 6573  \Z.QSS_Resources
-00000b20: 5a10 5153 535f 5265 736f 7572 6365 735f  Z.QSS_Resources_
-00000b30: 7263 7a08 7079 7263 6335 2022 7a06 2220  rcz.pyrcc5 "z." 
-00000b40: 2d6f 2022 fa01 227a 2465 7272 6f72 2077  -o ".."z$error w
-00000b50: 6869 6c65 2063 6f6e 7665 7274 696e 6720  hile converting 
-00000b60: 7265 736f 7572 6365 2066 696c 6529 2ada  resource file)*.
-00000b70: 0951 5365 7474 696e 6773 da02 6f73 da04  .QSettings..os..
-00000b80: 7061 7468 da07 6469 726e 616d 65da 085f  path..dirname.._
-00000b90: 5f66 696c 655f 5fda 046a 6f69 6e5a 1343  _file__..joinZ.C
-00000ba0: 7265 6174 6543 6f6c 6f72 5661 7269 6162  reateColorVariab
-00000bb0: 6c65 5a13 6765 7443 7572 7265 6e74 5468  leZ.getCurrentTh
-00000bc0: 656d 6549 6e66 6fda 0373 7472 da10 6164  emeInfo..str..ad
-00000bd0: 6a75 7374 5f6c 6967 6874 6e65 7373 da07  just_lightness..
-00000be0: 7265 706c 6163 65da 0761 6273 7061 7468  replace..abspath
-00000bf0: da06 6765 7463 7764 da05 7661 6c75 65da  ..getcwd..value.
-00000c00: 1573 686f 7743 7573 746f 6d57 6964 6765  .showCustomWidge
-00000c10: 7473 4c6f 6773 da05 7072 696e 74da 0477  tsLogs..print..w
-00000c20: 616c 6bda 0661 7070 656e 64da 036c 656e  alk..append..len
-00000c30: da08 6261 7365 6e61 6d65 7202 0000 00da  ..basenamer.....
-00000c40: 0665 7869 7374 73da 0673 6875 7469 6cda  .exists..shutil.
-00000c50: 046d 6f76 65da 0663 6f64 6563 73da 046f  .move..codecs..o
-00000c60: 7065 6eda 0472 6561 64da 0665 6e63 6f64  pen..read..encod
-00000c70: 65da 086d 616b 6564 6972 73da 0863 6169  e..makedirs..cai
-00000c80: 726f 7376 67da 0773 7667 3270 6e67 da09  rosvg..svg2png..
-00000c90: 4578 6365 7074 696f 6eda 0465 6d69 74da  Exception..emit.
-00000ca0: 0369 6e74 da05 696e 6465 78da 076c 6973  .int..index..lis
-00000cb0: 7464 6972 da04 6e61 6d65 da04 636f 7079  tdir..name..copy
-00000cc0: 5a08 7365 7456 616c 7565 da06 7379 7374  Z.setValue..syst
-00000cd0: 656d 7206 0000 00da 1067 656e 6572 6174  emr......generat
-00000ce0: 6541 6c6c 4963 6f6e 7329 2372 0a00 0000  eAllIcons)#r....
-00000cf0: da11 7072 6f67 7265 7373 5f63 616c 6c62  ..progress_callb
-00000d00: 6163 6bda 0873 6574 7469 6e67 7372 2800  ack..settingsr(.
-00000d10: 0000 da08 6669 6c65 6e61 6d65 da0d 6c69  ....filename..li
-00000d20: 7374 5f6f 665f 6669 6c65 73da 0563 6f6c  st_of_files..col
-00000d30: 6f72 da09 7376 675f 636f 6c6f 72da 0c6e  or..svg_color..n
-00000d40: 6f72 6d61 6c5f 636f 6c6f 72da 0d66 6f63  ormal_color..foc
-00000d50: 7573 6564 5f63 6f6c 6f72 da0e 6469 7361  used_color..disa
-00000d60: 626c 6564 5f63 6f6c 6f72 da0f 6963 6f6e  bled_color..icon
-00000d70: 7346 6f6c 6465 724e 616d 65da 0b69 636f  sFolderName..ico
-00000d80: 6e73 466f 6c64 6572 da0e 6f6c 6449 636f  nsFolder..oldIco
-00000d90: 6e73 466f 6c64 6572 5a0d 7661 7269 6162  nsFolderZ.variab
-00000da0: 6c65 7346 696c 655a 196f 6c64 4963 6f6e  lesFileZ.oldIcon
-00000db0: 7344 6573 7469 6e61 7469 6f6e 466f 6c64  sDestinationFold
-00000dc0: 6572 da04 726f 6f74 da04 6469 7273 da05  er..root..dirs..
-00000dd0: 6669 6c65 73da 0466 696c 65da 0a74 6f74  files..file..tot
-00000de0: 616c 4963 6f6e 7372 4600 0000 da06 6e61  alIconsrF.....na
-00000df0: 6d65 5f32 da01 66da 0763 6f6e 7465 6e74  me_2..f..content
-00000e00: da06 6e65 7753 5647 da08 6e65 7742 7974  ..newSVG..newByt
-00000e10: 6573 da01 65da 0a73 6f75 7263 655f 6469  es..e..source_di
-00000e20: 72da 0a74 6172 6765 745f 6469 725a 0a66  r..target_dirZ.f
-00000e30: 696c 655f 6e61 6d65 735a 0a66 696c 6573  ile_namesZ.files
-00000e40: 4d6f 7665 64da 0966 696c 655f 6e61 6d65  Moved..file_name
-00000e50: da0d 7265 736f 7572 6365 5f70 6174 685a  ..resource_pathZ
-00000e60: 1070 795f 7265 736f 7572 6365 5f70 6174  .py_resource_pat
-00000e70: 6872 0d00 0000 720d 0000 0072 0e00 0000  hr....r....r....
-00000e80: da10 6765 6e65 7261 7465 4e65 7749 636f  ..generateNewIco
-00000e90: 6e73 1500 0000 73d4 0000 0000 0106 020c  ns....s.........
-00000ea0: 010e 0104 020a 0104 010c 020a 010a 020c  ................
-00000eb0: 011e 021a 020e 010a 012c 022c 021e 0108  .........,.,....
-00000ec0: 0114 0108 0214 0108 011c 0208 020a 021a  ................
-00000ed0: 0130 0116 021a 0130 0116 021a 0130 011a  .0.....0.....0..
-00000ee0: 020a 0212 0108 020c 010a 021a 0116 020e  ................
-00000ef0: 010a 020e 0102 0212 0112 0124 0312 0108  ...........$....
-00000f00: 020c 010a 021a 0116 020e 010a 020e 0102  ................
-00000f10: 0212 0112 0124 0312 0108 020c 010a 021a  .....$..........
-00000f20: 0116 020e 010a 020e 0102 0212 0112 0124  ...............$
-00000f30: 0420 0304 0104 020a 020e 010c 020e 010a  . ..............
-00000f40: 0204 0108 010c 0118 0202 011a 0112 0128  ...............(
-00000f50: 0308 021a 041a 010e 013c 010c 010c 010c  .........<......
-00000f60: 010c 0202 010c 011a 0110 0112 021c 037a  ...............z
-00000f70: 224e 6577 4963 6f6e 7347 656e 6572 6174  "NewIconsGenerat
-00000f80: 6f72 2e67 656e 6572 6174 654e 6577 4963  or.generateNewIc
-00000f90: 6f6e 7363 0200 0000 0000 0000 0000 0000  onsc............
-00000fa0: 1c00 0000 0d00 0000 4300 0000 73ba 0500  ........C...s...
-00000fb0: 0074 0083 007d 0274 016a 02a0 0374 04a1  .t...}.t.j...t..
-00000fc0: 017d 0374 016a 02a0 057c 0364 01a1 027d  .}.t.j...|.d...}
-00000fd0: 0467 007d 0564 027d 067c 006a 066a 0744  .g.}.d.}.|.j.j.D
-00000fe0: 0090 055d 827d 077c 02a0 0864 03a1 017d  ...].}.|...d...}
-00000ff0: 087c 006a 0972 5474 0a64 047c 076a 0b17  .|.j.rTt.d.|.j..
-00001000: 0083 0101 0074 0c7c 0764 0583 0272 807c  .....t.|.d...r.|
-00001010: 076a 0d64 066b 0372 7474 0e7c 076a 0d83  .j.d.k.rtt.|.j..
-00001020: 017d 0971 f474 0e7c 076a 0f83 017d 096e  .}.q.t.|.j...}.n
-00001030: 747c 0864 076b 0272 b074 1083 007d 0a7c  t|.d.k.r.t...}.|
-00001040: 0a6a 1164 066b 0272 a474 0e7c 0a6a 1283  .j.d.k.r.t.|.j..
-00001050: 017d 0971 f474 0e7c 0a6a 1183 017d 096e  .}.q.t.|.j...}.n
-00001060: 447c 0864 086b 0272 e074 1383 007d 0a7c  D|.d.k.r.t...}.|
-00001070: 0a6a 1164 066b 0272 d474 0e7c 0a6a 1283  .j.d.k.r.t.|.j..
-00001080: 017d 0971 f474 0e7c 0a6a 1183 017d 096e  .}.q.t.|.j...}.n
-00001090: 147c 006a 0972 3074 0a64 097c 076a 0b83  .|.j.r0t.d.|.j..
-000010a0: 0201 0071 3074 147c 0964 0a83 027d 0b74  ...q0t.|.d...}.t
-000010b0: 147c 0964 0b83 027d 0c7c 09a0 1564 0c64  .|.d...}.|...d.d
-000010c0: 06a1 027d 0d74 016a 02a0 1674 016a 02a0  ...}.t.j...t.j..
-000010d0: 0574 01a0 17a1 0064 0d7c 0d17 00a1 02a1  .t.....d.|......
-000010e0: 017d 0e7c 006a 0990 0172 4674 0a64 0e7c  .}.|.j...rFt.d.|
-000010f0: 0964 0f83 0301 0074 01a0 187c 04a1 0144  .d.....t...|...D
-00001100: 005d 2c5c 037d 0f7d 107d 117c 1144 005d  .],\.}.}.}.|.D.]
-00001110: 1a7d 127c 05a0 1974 016a 02a0 057c 0f7c  .}.|...t.j...|.|
-00001120: 12a1 02a1 0101 0090 0171 5e90 0171 5074  .........q^..qPt
-00001130: 1a7c 0583 017d 137c 0544 0090 045d 267d  .|...}.|.D...]&}
-00001140: 1474 1b6a 1c7c 1464 1064 1164 128d 0390  .t.j.|.d.d.d....
-00001150: 018f 007d 157c 15a0 1da1 007d 167c 16a0  ...}.|.....}.|..
-00001160: 157c 067c 09a1 027d 1774 0ea0 1e7c 17a1  .|.|...}.t...|..
-00001170: 017d 1874 016a 02a0 1f74 207c 1483 016a  .}.t.j...t |...j
-00001180: 02a1 01a0 1564 1364 14a1 027d 1974 016a  .....d.d...}.t.j
-00001190: 02a0 1674 016a 02a0 057c 0e7c 19a1 02a1  ...t.j...|.|....
-000011a0: 017d 0474 016a 02a0 217c 0ea1 0190 0273  .}.t.j..!|.....s
-000011b0: 0a74 01a0 227c 0ea1 0101 0074 016a 02a0  .t.."|.....t.j..
-000011c0: 217c 04a1 0190 0272 2857 0035 0051 0052  !|.....r(W.5.Q.R
-000011d0: 00a3 0090 0171 8a6e 367c 02a0 0864 15a1  .....q.n6|...d..
-000011e0: 0164 006b 0990 0272 5e7c 02a0 0864 15a1  .d.k...r^|...d..
-000011f0: 01a0 1564 0c64 06a1 027c 0d6b 0290 0272  ...d.d...|.k...r
-00001200: 5e57 0035 0051 0052 00a3 0090 0171 8a7a  ^W.5.Q.R.....q.z
-00001210: 1274 236a 247c 187c 0464 168d 0201 0057  .t#j$|.|.d.....W
-00001220: 006e 2c04 0074 256b 0a90 0272 9c01 007d  .n,..t%k...r...}
-00001230: 1a01 007a 0c74 0a7c 1a83 0101 0057 0035  ...z.t.|.....W.5
-00001240: 0064 007d 1a7e 1a58 0059 006e 0258 0057  .d.}.~.X.Y.n.X.W
-00001250: 0035 0051 0052 0058 0074 1b6a 1c7c 1464  .5.Q.R.X.t.j.|.d
-00001260: 1064 1164 128d 0390 018f 5e7d 157c 15a0  .d.d......^}.|..
-00001270: 1da1 007d 167c 16a0 157c 067c 0ba1 027d  ...}.|...|.|...}
-00001280: 1774 0ea0 1e7c 17a1 017d 1874 016a 02a0  .t...|...}.t.j..
-00001290: 1f74 207c 1483 016a 02a1 01a0 1564 1364  .t |...j.....d.d
-000012a0: 17a1 027d 1974 016a 02a0 1674 016a 02a0  ...}.t.j...t.j..
-000012b0: 057c 0e7c 19a1 02a1 017d 0474 016a 02a0  .|.|.....}.t.j..
-000012c0: 217c 0ea1 0190 0373 2274 01a0 227c 0ea1  !|.....s"t.."|..
-000012d0: 0101 0074 016a 02a0 217c 04a1 0190 0372  ...t.j..!|.....r
-000012e0: 4057 0035 0051 0052 00a3 0090 0171 8a6e  @W.5.Q.R.....q.n
-000012f0: 7e7c 02a0 0864 15a1 0164 006b 0990 0372  ~|...d...d.k...r
-00001300: be7c 02a0 0864 15a1 01a0 1564 0c64 06a1  .|...d.....d.d..
-00001310: 027c 0d6b 0290 0372 be74 016a 02a0 1674  .|.k...r.t.j...t
-00001320: 016a 02a0 0574 01a0 17a1 0064 18a1 02a1  .j...t.....d....
-00001330: 017d 1b74 016a 02a0 2174 016a 02a0 057c  .}.t.j..!t.j...|
-00001340: 1b7c 19a1 02a1 0190 0372 be74 26a0 2774  .|.......r.t&.'t
-00001350: 016a 02a0 057c 1b7c 19a1 027c 0ea1 0201  .j...|.|...|....
-00001360: 0057 0035 0051 0052 00a3 0090 0171 8a74  .W.5.Q.R.....q.t
-00001370: 016a 02a0 1674 016a 02a0 057c 0e7c 19a1  .j...t.j...|.|..
-00001380: 02a1 017d 047a 1274 236a 247c 187c 0464  ...}.z.t#j$|.|.d
-00001390: 168d 0201 0057 006e 2c04 0074 256b 0a90  .....W.n,..t%k..
-000013a0: 0472 1201 007d 1a01 007a 0c74 0a7c 1a83  .r...}...z.t.|..
-000013b0: 0101 0057 0035 0064 007d 1a7e 1a58 0059  ...W.5.d.}.~.X.Y
-000013c0: 006e 0258 0057 0035 0051 0052 0058 0074  .n.X.W.5.Q.R.X.t
-000013d0: 1b6a 1c7c 1464 1064 1164 128d 0390 018f  .j.|.d.d.d......
-000013e0: 5e7d 157c 15a0 1da1 007d 167c 16a0 157c  ^}.|.....}.|...|
-000013f0: 067c 0ca1 027d 1774 0ea0 1e7c 17a1 017d  .|...}.t...|...}
-00001400: 1874 016a 02a0 1f74 207c 1483 016a 02a1  .t.j...t |...j..
-00001410: 01a0 1564 1364 19a1 027d 1974 016a 02a0  ...d.d...}.t.j..
-00001420: 1674 016a 02a0 057c 0e7c 19a1 02a1 017d  .t.j...|.|.....}
-00001430: 0474 016a 02a0 217c 0ea1 0190 0473 9874  .t.j..!|.....s.t
-00001440: 01a0 227c 0ea1 0101 0074 016a 02a0 217c  .."|.....t.j..!|
-00001450: 04a1 0190 0472 b657 0035 0051 0052 00a3  .....r.W.5.Q.R..
-00001460: 0090 0171 8a6e 7e7c 02a0 0864 15a1 0164  ...q.n~|...d...d
-00001470: 006b 0990 0572 347c 02a0 0864 15a1 01a0  .k...r4|...d....
-00001480: 1564 0c64 06a1 027c 0d6b 0290 0572 3474  .d.d...|.k...r4t
-00001490: 016a 02a0 1674 016a 02a0 0574 01a0 17a1  .j...t.j...t....
-000014a0: 0064 18a1 02a1 017d 1b74 016a 02a0 2174  .d.....}.t.j..!t
-000014b0: 016a 02a0 057c 1b7c 19a1 02a1 0190 0572  .j...|.|.......r
-000014c0: 3474 26a0 2774 016a 02a0 057c 1b7c 19a1  4t&.'t.j...|.|..
-000014d0: 027c 0ea1 0201 0057 0035 0051 0052 00a3  .|.....W.5.Q.R..
-000014e0: 0090 0171 8a74 016a 02a0 1674 016a 02a0  ...q.t.j...t.j..
-000014f0: 057c 0e7c 19a1 02a1 017d 047a 1274 236a  .|.|.....}.z.t#j
-00001500: 247c 187c 0464 168d 0201 0057 006e 2c04  $|.|.d.....W.n,.
-00001510: 0074 256b 0a90 0572 8801 007d 1a01 007a  .t%k...r...}...z
-00001520: 0c74 0a7c 1a83 0101 0057 0035 0064 007d  .t.|.....W.5.d.}
-00001530: 1a7e 1a58 0059 006e 0258 0057 0035 0051  .~.X.Y.n.X.W.5.Q
-00001540: 0052 0058 007c 01a0 2874 297c 05a0 2a7c  .R.X.|..(t)|..*|
-00001550: 14a1 017c 131b 0064 1a14 0083 01a1 0101  ...|...d........
-00001560: 0090 0171 8a71 3064 0053 0029 1b4e 720f  ...q.q0d.S.).Nr.
-00001570: 0000 0072 1000 0000 da05 5448 454d 457a  ...r......THEMEz
-00001580: 1343 6865 636b 696e 6720 6963 6f6e 7320  .Checking icons 
-00001590: 666f 7220 da0a 6963 6f6e 7343 6f6c 6f72  for ..iconsColor
-000015a0: 7214 0000 005a 054c 4947 4854 5a04 4441  r....Z.LIGHTZ.DA
-000015b0: 524b 7a22 4e6f 2069 636f 6e73 2063 6f6c  RKz"No icons col
-000015c0: 6f72 2073 7065 6369 6669 6564 2066 6f72  or specified for
-000015d0: 2074 6865 6d65 7211 0000 0072 1200 0000   themer....r....
-000015e0: 7213 0000 0072 1500 0000 7a27 4765 6e65  r....r....z'Gene
-000015f0: 7261 7469 6e67 206d 6973 7369 6e67 2069  rating missing i
-00001600: 636f 6e73 2066 6f72 2079 6f75 7220 7468  cons for your th
-00001610: 656d 657a 1f70 6c65 6173 6520 7761 6974  emez.please wait
-00001620: 2e20 5468 6973 206d 6179 2074 616b 6520  . This may take 
-00001630: 6c6f 6e67 721c 0000 0072 1d00 0000 721e  longr....r....r.
-00001640: 0000 0072 1800 0000 7219 0000 0072 1700  ...r....r....r..
-00001650: 0000 7221 0000 0072 1a00 0000 7216 0000  ..r!...r....r...
-00001660: 0072 1b00 0000 7222 0000 0029 2b72 2500  .r....r"...)+r%.
-00001670: 0000 7226 0000 0072 2700 0000 7228 0000  ..r&...r'...r(..
-00001680: 0072 2900 0000 722a 0000 005a 0275 69da  .r)...r*...Z.ui.
-00001690: 0674 6865 6d65 7372 3000 0000 7231 0000  .themesr0...r1..
-000016a0: 0072 3200 0000 7246 0000 00da 0768 6173  .r2...rF.....has
-000016b0: 6174 7472 7267 0000 0072 2b00 0000 5a0b  attrrg...r+...Z.
-000016c0: 6163 6365 6e74 436f 6c6f 725a 054c 6967  accentColorZ.Lig
-000016d0: 6874 5a0b 6963 6f6e 735f 636f 6c6f 725a  htZ.icons_colorZ
-000016e0: 0c61 6363 656e 745f 636f 6c6f 725a 0444  .accent_colorZ.D
-000016f0: 6172 6b72 2c00 0000 722d 0000 0072 2e00  arkr,...r-...r..
-00001700: 0000 722f 0000 0072 3300 0000 7234 0000  ..r/...r3...r4..
-00001710: 0072 3500 0000 723a 0000 0072 3b00 0000  .r5...r:...r;...
-00001720: 723c 0000 0072 3d00 0000 7236 0000 0072  r<...r=...r6...r
-00001730: 0200 0000 7237 0000 0072 3e00 0000 723f  ....r7...r>...r?
-00001740: 0000 0072 4000 0000 7241 0000 0072 3800  ...r@...rA...r8.
-00001750: 0000 7239 0000 0072 4200 0000 7243 0000  ..r9...rB...rC..
-00001760: 0072 4400 0000 291c 720a 0000 0072 4a00  .rD...).r....rJ.
-00001770: 0000 724b 0000 0072 2800 0000 724c 0000  ..rK...r(...rL..
-00001780: 0072 4d00 0000 724f 0000 00da 0574 6865  .rM...rO.....the
-00001790: 6d65 7266 0000 0072 5000 0000 5a0d 7468  merf...rP...Z.th
-000017a0: 656d 6550 726f 7065 7274 7972 5100 0000  emePropertyrQ...
-000017b0: 7252 0000 0072 5300 0000 7254 0000 0072  rR...rS...rT...r
-000017c0: 5600 0000 7257 0000 0072 5800 0000 7259  V...rW...rX...rY
-000017d0: 0000 0072 5a00 0000 7246 0000 0072 5c00  ...rZ...rF...r\.
-000017e0: 0000 725d 0000 0072 5e00 0000 725f 0000  ..r]...r^...r_..
-000017f0: 0072 5b00 0000 7260 0000 0072 5500 0000  .r[...r`...rU...
-00001800: 720d 0000 0072 0d00 0000 720e 0000 0072  r....r....r....r
-00001810: 4900 0000 b800 0000 73bc 0000 0000 0106  I.......s.......
-00001820: 020c 010e 0104 0204 020e 010a 0406 010e  ................
-00001830: 030a 010a 010c 020c 0208 0106 010a 010c  ................
-00001840: 020c 0208 0106 010a 010c 020c 0306 010c  ................
-00001850: 0102 020a 010a 020c 021e 0208 010c 0214  ................
-00001860: 0108 011c 0208 010a 0214 0108 020c 010a  ................
-00001870: 021a 0116 020e 010a 020e 0110 0228 010e  .............(..
-00001880: 0102 0212 0112 0124 0314 0108 020c 010a  .......$........
-00001890: 021a 0116 020e 010a 020e 0110 0228 021a  .............(..
-000018a0: 0218 0116 010e 0216 0102 0212 0112 0124  ...............$
-000018b0: 0314 0108 020c 010a 021a 0116 020e 010a  ................
-000018c0: 020e 0110 0228 021a 0218 0116 010e 0216  .....(..........
-000018d0: 0102 0112 0112 0124 047a 224e 6577 4963  .......$.z"NewIc
-000018e0: 6f6e 7347 656e 6572 6174 6f72 2e67 656e  onsGenerator.gen
-000018f0: 6572 6174 6541 6c6c 4963 6f6e 7329 08da  erateAllIcons)..
-00001900: 085f 5f6e 616d 655f 5fda 0a5f 5f6d 6f64  .__name__..__mod
-00001910: 756c 655f 5fda 0c5f 5f71 7561 6c6e 616d  ule__..__qualnam
-00001920: 655f 5fda 075f 5f64 6f63 5f5f 7208 0000  e__..__doc__r...
-00001930: 0072 6500 0000 7249 0000 00da 0d5f 5f63  .re...rI.....__c
-00001940: 6c61 7373 6365 6c6c 5f5f 720d 0000 0072  lasscell__r....r
-00001950: 0d00 0000 720b 0000 0072 0e00 0000 7206  ....r....r....r.
-00001960: 0000 000f 0000 0073 0a00 0000 0801 0401  .......s........
-00001970: 0c04 087f 0024 7206 0000 0029 0e72 3f00  .....$r....).r?.
-00001980: 0000 723a 0000 0072 2600 0000 da03 7379  ..r:...r&.....sy
-00001990: 7372 3800 0000 da0c 7572 6c6c 6962 2e70  sr8.....urllib.p
-000019a0: 6172 7365 7202 0000 00da 0770 6174 686c  arser......pathl
-000019b0: 6962 7203 0000 00da 085f 5f6d 6169 6e5f  ibr......__main_
-000019c0: 5f5a 0b63 6f6c 6f72 7379 7374 656d 7225  _Z.colorsystemr%
-000019d0: 0000 0072 4b00 0000 7206 0000 0072 0d00  ...rK...r....r..
-000019e0: 0000 720d 0000 0072 0d00 0000 720e 0000  ..r....r....r...
-000019f0: 00da 083c 6d6f 6475 6c65 3e01 0000 0073  ...<module>....s
-00001a00: 1400 0000 0801 0801 0801 0801 0801 0c01  ................
-00001a10: 0c01 0803 0802 0602                      ........
+00000050: 6401 6c04 5a04 6400 6401 6c05 5a05 6400  d.l.Z.d.d.l.Z.d.
+00000060: 6401 6c06 5a06 6400 6401 6c07 5a07 6400  d.l.Z.d.d.l.Z.d.
+00000070: 6402 6c08 6d09 5a09 0100 6400 6403 6c0a  d.l.m.Z...d.d.l.
+00000080: 6d0b 5a0b 0100 6400 6401 6c0c 5a0c 6404  m.Z...d.d.l.Z.d.
+00000090: 6405 6c0d 5400 650e 8300 5a0f 4700 6406  d.l.T.e...Z.G.d.
+000000a0: 6407 8400 6407 8302 5a10 6401 5300 2908  d...d...Z.d.S.).
+000000b0: e900 0000 004e 2901 da08 7572 6c70 6172  .....N)...urlpar
+000000c0: 7365 2901 da04 5061 7468 e901 0000 0029  se)...Path.....)
+000000d0: 01da 012a 6300 0000 0000 0000 0000 0000  ...*c...........
+000000e0: 0000 0000 0003 0000 0000 0000 0073 3800  .............s8.
+000000f0: 0000 6500 5a01 6400 5a02 6401 5a03 8700  ..e.Z.d.Z.d.Z...
+00000100: 6601 6402 6403 8408 5a04 6404 6405 8400  f.d.d...Z.d.d...
+00000110: 5a05 6406 6407 8400 5a06 6408 6409 8400  Z.d.d...Z.d.d...
+00000120: 5a07 8700 0400 5a08 5300 290a da11 4e65  Z.....Z.S.)...Ne
+00000130: 7749 636f 6e73 4765 6e65 7261 746f 727a  wIconsGeneratorz
+00000140: 1f64 6f63 7374 7269 6e67 2066 6f72 204e  .docstring for N
+00000150: 6577 4963 6f6e 7347 656e 6572 6174 6f72  ewIconsGenerator
+00000160: 6302 0000 0000 0000 0000 0000 0002 0000  c...............
+00000170: 0003 0000 0003 0000 0073 1800 0000 7400  .........s....t.
+00000180: 7401 7c00 8302 a002 a100 0100 7c01 7c00  t.|.........|.|.
+00000190: 5f03 6400 5300 2901 4e29 04da 0573 7570  _.d.S.).N)...sup
+000001a0: 6572 7206 0000 00da 085f 5f69 6e69 745f  err......__init_
+000001b0: 5fda 0361 7267 2902 da04 7365 6c66 7209  _..arg)...selfr.
+000001c0: 0000 00a9 01da 095f 5f63 6c61 7373 5f5f  .......__class__
+000001d0: a900 fa48 653a 5c53 7069 6e6e 2054 6173  ...He:\Spinn Tas
+000001e0: 6b5c 3070 6173 735c 3070 6173 732d 6170  k\0pass\0pass-ap
+000001f0: 702d 6d61 7374 6572 5c43 7573 746f 6d5f  p-master\Custom_
+00000200: 5769 6467 6574 735c 5173 735c 5376 6754  Widgets\Qss\SvgT
+00000210: 6f50 6e67 4963 6f6e 732e 7079 7208 0000  oPngIcons.pyr...
+00000220: 0015 0000 0073 0400 0000 0001 0e01 7a1a  .....s........z.
+00000230: 4e65 7749 636f 6e73 4765 6e65 7261 746f  NewIconsGenerato
+00000240: 722e 5f5f 696e 6974 5f5f 6302 0000 0000  r.__init__c.....
+00000250: 0000 0000 0000 0024 0000 000c 0000 0043  .......$.......C
+00000260: 0000 0073 4a07 0000 7400 8300 7d02 7401  ...sJ...t...}.t.
+00000270: 6a02 a003 7404 a101 7d03 7401 6a02 a005  j...t...}.t.j...
+00000280: 7c03 6401 a102 7d04 6700 7d05 7406 a007  |.d...}.g.}.t...
+00000290: 7c00 a101 7d06 6402 7d07 7408 7c06 6403  |...}.d.}.t.|.d.
+000002a0: 1900 8301 7d08 7409 7c08 6404 8302 7d09  ....}.t.|.d...}.
+000002b0: 7409 7c08 6405 8302 7d0a 7c08 a00a 6406  t.|.d...}.|...d.
+000002c0: 6407 a102 7d0b 7401 6a02 a00b 7401 6a02  d...}.t.j...t.j.
+000002d0: a005 7401 a00c a100 6408 7c0b 1700 a102  ..t.....d.|.....
+000002e0: a101 7d0c 7401 6a02 a00b 7401 6a02 a005  ..}.t.j...t.j...
+000002f0: 7401 a00c a100 6409 a102 a101 7d0d 7c02  t.....d.....}.|.
+00000300: a00d 640a a101 6400 6b08 72da 7406 a007  ..d...d.k.r.t...
+00000310: 7c00 a101 7d0e 7401 6a02 a00b 7401 6a02  |...}.t.j...t.j.
+00000320: a005 7401 a00c a100 6408 7c0e 6403 1900  ..t.....d.|.d...
+00000330: a00a 6406 6407 a102 1700 a102 a101 7d0f  ..d.d.........}.
+00000340: 6e2c 7401 6a02 a00b 7401 6a02 a005 7401  n,t.j...t.j...t.
+00000350: a00c a100 6408 7c02 a00d 640a a101 a00a  ....d.|...d.....
+00000360: 6406 6407 a102 1700 a102 a101 7d0f 7c02  d.d.........}.|.
+00000370: a00d 640a a101 7c08 6b02 9007 733a 7c06  ..d...|.k...s:|.
+00000380: 6403 1900 6400 6b09 9007 723a 7c00 6a0e  d...d.k...r:|.j.
+00000390: 9001 7248 740f 640b 7c02 a00d 640a a101  ..rHt.d.|...d...
+000003a0: 640c 7c08 8304 0100 740f 640d 8301 0100  d.|.....t.d.....
+000003b0: 7401 a010 7c04 a101 4400 5d2c 5c03 7d10  t...|...D.],\.}.
+000003c0: 7d11 7d12 7c12 4400 5d1a 7d13 7c05 a011  }.}.|.D.].}.|...
+000003d0: 7401 6a02 a005 7c10 7c13 a102 a101 0100  t.j...|.|.......
+000003e0: 9001 7160 9001 7152 7412 7c05 8301 7d14  ..q`..qRt.|...}.
+000003f0: 7c05 4400 9001 5d26 7d15 7401 6a02 a013  |.D...]&}.t.j...
+00000400: 7414 7c15 8301 6a02 a101 a00a 640e 640f  t.|...j.....d.d.
+00000410: a102 7d16 7401 6a02 a015 7401 6a02 a005  ..}.t.j...t.j...
+00000420: 7c0d 7c16 a102 a101 9001 72f2 7401 6a02  |.|.......r.t.j.
+00000430: a015 7401 6a02 a005 7c0f 7c16 a102 a101  ..t.j...|.|.....
+00000440: 9001 73f2 7416 a017 7401 6a02 a005 7c0d  ..s.t...t.j...|.
+00000450: 7c16 a102 7c0f a102 0100 7401 6a02 a013  |...|.....t.j...
+00000460: 7414 7c15 8301 6a02 a101 a00a 640e 6410  t.|...j.....d.d.
+00000470: a102 7d16 7401 6a02 a015 7401 6a02 a005  ..}.t.j...t.j...
+00000480: 7c0d 7c16 a102 a101 9002 7252 7401 6a02  |.|.......rRt.j.
+00000490: a015 7401 6a02 a005 7c0f 7c16 a102 a101  ..t.j...|.|.....
+000004a0: 9002 7352 7416 a017 7401 6a02 a005 7c0d  ..sRt...t.j...|.
+000004b0: 7c16 a102 7c0f a102 0100 7401 6a02 a013  |...|.....t.j...
+000004c0: 7414 7c15 8301 6a02 a101 a00a 640e 6411  t.|...j.....d.d.
+000004d0: a102 7d16 7401 6a02 a015 7401 6a02 a005  ..}.t.j...t.j...
+000004e0: 7c0d 7c16 a102 a101 9001 728c 7401 6a02  |.|.......r.t.j.
+000004f0: a015 7401 6a02 a005 7c0f 7c16 a102 a101  ..t.j...|.|.....
+00000500: 9001 738c 7416 a017 7401 6a02 a005 7c0d  ..s.t...t.j...|.
+00000510: 7c16 a102 7c0f a102 0100 9001 718c 7c05  |...|.......q.|.
+00000520: 4400 9002 5d92 7d15 7418 6a19 7c15 6412  D...].}.t.j.|.d.
+00000530: 6413 6414 8d03 8fba 7d17 7c17 a01a a100  d.d.....}.|.....
+00000540: 7d18 7c18 a00a 7c07 7c08 a102 7d19 7408  }.|...|.|...}.t.
+00000550: a01b 7c19 a101 7d1a 7401 6a02 a013 7414  ..|...}.t.j...t.
+00000560: 7c15 8301 6a02 a101 a00a 640e 640f a102  |...j.....d.d...
+00000570: 7d16 7401 6a02 a00b 7401 6a02 a005 7c0c  }.t.j...t.j...|.
+00000580: 7c16 a102 a101 7d04 7401 6a02 a015 7c0c  |.....}.t.j...|.
+00000590: a101 9003 7338 7401 a01c 7c0c a101 0100  ....s8t...|.....
+000005a0: 7401 6a02 a015 7c04 a101 9003 7386 7a12  t.j...|.....s.z.
+000005b0: 741d 6a1e 7c1a 7c04 6415 8d02 0100 5700  t.j.|.|.d.....W.
+000005c0: 6e2c 0400 741f 6b0a 9003 7284 0100 7d1b  n,..t.k...r...}.
+000005d0: 0100 7a0c 740f 7c1b 8301 0100 5700 3500  ..z.t.|.....W.5.
+000005e0: 6400 7d1b 7e1b 5800 5900 6e02 5800 5700  d.}.~.X.Y.n.X.W.
+000005f0: 3500 5100 5200 5800 7418 6a19 7c15 6412  5.Q.R.X.t.j.|.d.
+00000600: 6413 6414 8d03 8fba 7d17 7c17 a01a a100  d.d.....}.|.....
+00000610: 7d18 7c18 a00a 7c07 7c09 a102 7d19 7408  }.|...|.|...}.t.
+00000620: a01b 7c19 a101 7d1a 7401 6a02 a013 7414  ..|...}.t.j...t.
+00000630: 7c15 8301 6a02 a101 a00a 640e 6410 a102  |...j.....d.d...
+00000640: 7d16 7401 6a02 a00b 7401 6a02 a005 7c0c  }.t.j...t.j...|.
+00000650: 7c16 a102 a101 7d04 7401 6a02 a015 7c0c  |.....}.t.j...|.
+00000660: a101 9004 7308 7401 a01c 7c0c a101 0100  ....s.t...|.....
+00000670: 7401 6a02 a015 7c04 a101 9004 7356 7a12  t.j...|.....sVz.
+00000680: 741d 6a1e 7c1a 7c04 6415 8d02 0100 5700  t.j.|.|.d.....W.
+00000690: 6e2c 0400 741f 6b0a 9004 7254 0100 7d1b  n,..t.k...rT..}.
+000006a0: 0100 7a0c 740f 7c1b 8301 0100 5700 3500  ..z.t.|.....W.5.
+000006b0: 6400 7d1b 7e1b 5800 5900 6e02 5800 5700  d.}.~.X.Y.n.X.W.
+000006c0: 3500 5100 5200 5800 7418 6a19 7c15 6412  5.Q.R.X.t.j.|.d.
+000006d0: 6413 6414 8d03 8fba 7d17 7c17 a01a a100  d.d.....}.|.....
+000006e0: 7d18 7c18 a00a 7c07 7c0a a102 7d19 7408  }.|...|.|...}.t.
+000006f0: a01b 7c19 a101 7d1a 7401 6a02 a013 7414  ..|...}.t.j...t.
+00000700: 7c15 8301 6a02 a101 a00a 640e 6411 a102  |...j.....d.d...
+00000710: 7d16 7401 6a02 a00b 7401 6a02 a005 7c0c  }.t.j...t.j...|.
+00000720: 7c16 a102 a101 7d04 7401 6a02 a015 7c0c  |.....}.t.j...|.
+00000730: a101 9004 73d8 7401 a01c 7c0c a101 0100  ....s.t...|.....
+00000740: 7401 6a02 a015 7c04 a101 9005 7326 7a12  t.j...|.....s&z.
+00000750: 741d 6a1e 7c1a 7c04 6415 8d02 0100 5700  t.j.|.|.d.....W.
+00000760: 6e2c 0400 741f 6b0a 9005 7224 0100 7d1b  n,..t.k...r$..}.
+00000770: 0100 7a0c 740f 7c1b 8301 0100 5700 3500  ..z.t.|.....W.5.
+00000780: 6400 7d1b 7e1b 5800 5900 6e02 5800 5700  d.}.~.X.Y.n.X.W.
+00000790: 3500 5100 5200 5800 7c01 a020 7421 7c05  5.Q.R.X.|.. t!|.
+000007a0: a022 7c15 a101 7c14 1b00 6416 1400 8301  ."|...|...d.....
+000007b0: a101 0100 9002 71ba 7c0c 7d1c 7c0d 7d1d  ......q.|.}.|.}.
+000007c0: 7401 a023 7c1c a101 7d1e 7401 6a02 a015  t..#|...}.t.j...
+000007d0: 7c0d a101 9005 737c 7401 a01c 7c0d a101  |.....s|t...|...
+000007e0: 0100 6e18 7401 6a02 a015 7c0d a101 9005  ..n.t.j...|.....
+000007f0: 7394 7401 a01c 7c0d a101 0100 6417 7d1f  s.t...|.....d.}.
+00000800: 7c1e 4400 5d9e 7d20 7401 6a24 6418 6b02  |.D.].} t.j$d.k.
+00000810: 9005 72c4 7416 a025 7401 6a02 a005 7c1c  ..r.t..%t.j...|.
+00000820: 7c20 a102 7c1d a102 0100 6e56 7a1a 7416  | ..|.....nVz.t.
+00000830: a017 7401 6a02 a005 7c1c 7c20 a102 7c1d  ..t.j...|.| ..|.
+00000840: a102 0100 5700 6e3a 0400 741f 6b0a 9006  ....W.n:..t.k...
+00000850: 7218 0100 7d1b 0100 7a1a 7416 a025 7401  r...}...z.t..%t.
+00000860: 6a02 a005 7c1c 7c20 a102 7c1d a102 0100  j...|.| ..|.....
+00000870: 5700 3500 6400 7d1b 7e1b 5800 5900 6e02  W.5.d.}.~.X.Y.n.
+00000880: 5800 7c1f 6419 3700 7d1f 7c01 a020 7421  X.|.d.7.}.|.. t!
+00000890: 7c1f 7c14 1b00 6416 1400 8301 a101 0100  |.|...d.........
+000008a0: 9005 719c 7401 6a02 a00b 7401 6a02 a005  ..q.t.j...t.j...
+000008b0: 7401 a00c a100 641a a102 a101 7d21 7401  t.....d.....}!t.
+000008c0: 6a02 a015 7c21 a101 9006 73a0 7416 a025  j...|!....s.t..%
+000008d0: 7401 6a02 a00b 7401 6a02 a005 7401 6a02  t.j...t.j...t.j.
+000008e0: a003 7404 a101 641b a102 a101 7401 6a02  ..t...d.....t.j.
+000008f0: a00b 7401 6a02 a005 7401 a00c a100 641c  ..t.j...t.....d.
+00000900: a102 a101 a102 0100 7c21 a00a 641d 641e  ........|!..d.d.
+00000910: a102 7d22 7c22 a00a 6408 6407 a102 7d22  ..}"|"..d.d...}"
+00000920: 7c22 a00a 641f 6407 a102 7d22 7c22 a00a  |"..d.d...}"|"..
+00000930: 6420 6421 a102 7d22 7a36 7c02 a026 640a  d d!..}"z6|..&d.
+00000940: 7c08 a102 0100 7401 a027 6422 7c21 1700  |.....t..'d"|!..
+00000950: 6423 1700 7c22 1700 6424 1700 a101 0100  d#..|"..d$......
+00000960: 7c02 a026 640a 7c08 a102 0100 5700 6e2c  |..&d.|.....W.n,
+00000970: 0400 741f 6b0a 9007 7232 0100 7d1b 0100  ..t.k...r2..}...
+00000980: 7a0c 740f 6425 8301 0100 5700 3500 6400  z.t.d%....W.5.d.
+00000990: 7d1b 7e1b 5800 5900 6e02 5800 6421 7d23  }.~.X.Y.n.X.d!}#
+000009a0: 6e0c 7428 a029 7c00 7c01 a102 0100 6400  n.t(.)|.|.....d.
+000009b0: 5300 2926 4efa 1269 636f 6e73 2f6f 7269  S.)&N..icons/ori
+000009c0: 6769 6e61 6c5f 7376 67fa 0423 6666 667a  ginal_svg..#fffz
+000009d0: 0b69 636f 6e73 2d63 6f6c 6f72 e700 0000  .icons-color....
+000009e0: 0000 00f8 3fe7 0000 0000 0000 e03f fa01  ....?........?..
+000009f0: 23da 00fa 0451 5353 2ffa 0951 5353 2f49  #....QSS/..QSS/I
+00000a00: 636f 6e73 fa0b 4943 4f4e 532d 434f 4c4f  cons..ICONS-COLO
+00000a10: 527a 1443 7572 7265 6e74 2069 636f 6e73  Rz.Current icons
+00000a20: 2063 6f6c 6f72 207a 0f4e 6577 2069 636f   color z.New ico
+00000a30: 6e73 2063 6f6c 6f72 7a40 4765 6e65 7261  ns colorz@Genera
+00000a40: 7469 6e67 2069 636f 6e73 2066 6f72 2079  ting icons for y
+00000a50: 6f75 7220 7468 656d 652c 2070 6c65 6173  our theme, pleas
+00000a60: 6520 7761 6974 2e20 5468 6973 206d 6179  e wait. This may
+00000a70: 2074 616b 6520 6c6f 6e67 fa04 2e73 7667   take long...svg
+00000a80: fa04 2e70 6e67 fa0a 5f66 6f63 7573 2e70  ...png.._focus.p
+00000a90: 6e67 fa0d 5f64 6973 6162 6c65 642e 706e  ng.._disabled.pn
+00000aa0: 67fa 0575 7466 2d38 da06 6967 6e6f 7265  g..utf-8..ignore
+00000ab0: a902 da08 656e 636f 6469 6e67 da06 6572  ....encoding..er
+00000ac0: 726f 7273 a902 5a0a 6279 7465 7374 7269  rors..Z.bytestri
+00000ad0: 6e67 5a08 7772 6974 655f 746f e964 0000  ngZ.write_to.d..
+00000ae0: 0072 0100 0000 da02 6e74 7204 0000 007a  .r......ntr....z
+00000af0: 1551 5353 2f51 5353 5f52 6573 6f75 7263  .QSS/QSS_Resourc
+00000b00: 6573 2e71 7263 7a11 5153 535f 5265 736f  es.qrcz.QSS_Reso
+00000b10: 7572 6365 732e 7172 63da 0351 5353 7a04  urces.qrc..QSSz.
+00000b20: 2e71 7263 fa03 2e70 797a 0451 5353 5c5a  .qrc...pyz.QSS\Z
+00000b30: 0d51 5353 5f52 6573 6f75 7263 6573 5a10  .QSS_ResourcesZ.
+00000b40: 5153 535f 5265 736f 7572 6365 735f 7263  QSS_Resources_rc
+00000b50: 7a08 7079 7263 6335 2022 7a06 2220 2d6f  z.pyrcc5 "z." -o
+00000b60: 2022 fa01 227a 2465 7272 6f72 2077 6869   ".."z$error whi
+00000b70: 6c65 2063 6f6e 7665 7274 696e 6720 7265  le converting re
+00000b80: 736f 7572 6365 2066 696c 6529 2ada 0951  source file)*..Q
+00000b90: 5365 7474 696e 6773 da02 6f73 da04 7061  Settings..os..pa
+00000ba0: 7468 da07 6469 726e 616d 65da 085f 5f66  th..dirname..__f
+00000bb0: 696c 655f 5fda 046a 6f69 6eda 1343 7265  ile__..join..Cre
+00000bc0: 6174 6543 6f6c 6f72 5661 7269 6162 6c65  ateColorVariable
+00000bd0: da13 6765 7443 7572 7265 6e74 5468 656d  ..getCurrentThem
+00000be0: 6549 6e66 6fda 0373 7472 da10 6164 6a75  eInfo..str..adju
+00000bf0: 7374 5f6c 6967 6874 6e65 7373 da07 7265  st_lightness..re
+00000c00: 706c 6163 65da 0761 6273 7061 7468 da06  place..abspath..
+00000c10: 6765 7463 7764 da05 7661 6c75 65da 1573  getcwd..value..s
+00000c20: 686f 7743 7573 746f 6d57 6964 6765 7473  howCustomWidgets
+00000c30: 4c6f 6773 da05 7072 696e 74da 0477 616c  Logs..print..wal
+00000c40: 6bda 0661 7070 656e 64da 036c 656e da08  k..append..len..
+00000c50: 6261 7365 6e61 6d65 7202 0000 00da 0665  basenamer......e
+00000c60: 7869 7374 73da 0673 6875 7469 6cda 046d  xists..shutil..m
+00000c70: 6f76 65da 0663 6f64 6563 73da 046f 7065  ove..codecs..ope
+00000c80: 6eda 0472 6561 64da 0665 6e63 6f64 65da  n..read..encode.
+00000c90: 086d 616b 6564 6972 73da 0863 6169 726f  .makedirs..cairo
+00000ca0: 7376 67da 0773 7667 3270 6e67 da09 4578  svg..svg2png..Ex
+00000cb0: 6365 7074 696f 6eda 0465 6d69 74da 0369  ception..emit..i
+00000cc0: 6e74 da05 696e 6465 78da 076c 6973 7464  nt..index..listd
+00000cd0: 6972 da04 6e61 6d65 da04 636f 7079 da08  ir..name..copy..
+00000ce0: 7365 7456 616c 7565 da06 7379 7374 656d  setValue..system
+00000cf0: 7206 0000 00da 1067 656e 6572 6174 6541  r......generateA
+00000d00: 6c6c 4963 6f6e 7329 2472 0a00 0000 da11  llIcons)$r......
+00000d10: 7072 6f67 7265 7373 5f63 616c 6c62 6163  progress_callbac
+00000d20: 6bda 0873 6574 7469 6e67 7372 2a00 0000  k..settingsr*...
+00000d30: da08 6669 6c65 6e61 6d65 da0d 6c69 7374  ..filename..list
+00000d40: 5f6f 665f 6669 6c65 73da 0563 6f6c 6f72  _of_files..color
+00000d50: da09 7376 675f 636f 6c6f 72da 0c6e 6f72  ..svg_color..nor
+00000d60: 6d61 6c5f 636f 6c6f 72da 0d66 6f63 7573  mal_color..focus
+00000d70: 6564 5f63 6f6c 6f72 da0e 6469 7361 626c  ed_color..disabl
+00000d80: 6564 5f63 6f6c 6f72 da0f 6963 6f6e 7346  ed_color..iconsF
+00000d90: 6f6c 6465 724e 616d 65da 0b69 636f 6e73  olderName..icons
+00000da0: 466f 6c64 6572 da0e 6f6c 6449 636f 6e73  Folder..oldIcons
+00000db0: 466f 6c64 6572 da0d 7661 7269 6162 6c65  Folder..variable
+00000dc0: 7346 696c 655a 196f 6c64 4963 6f6e 7344  sFileZ.oldIconsD
+00000dd0: 6573 7469 6e61 7469 6f6e 466f 6c64 6572  estinationFolder
+00000de0: da04 726f 6f74 da04 6469 7273 da05 6669  ..root..dirs..fi
+00000df0: 6c65 73da 0466 696c 65da 0a74 6f74 616c  les..file..total
+00000e00: 4963 6f6e 7372 4a00 0000 da06 6e61 6d65  IconsrJ.....name
+00000e10: 5f32 da01 66da 0763 6f6e 7465 6e74 da06  _2..f..content..
+00000e20: 6e65 7753 5647 da08 6e65 7742 7974 6573  newSVG..newBytes
+00000e30: da01 655a 0a73 6f75 7263 655f 6469 725a  ..eZ.source_dirZ
+00000e40: 0a74 6172 6765 745f 6469 725a 0a66 696c  .target_dirZ.fil
+00000e50: 655f 6e61 6d65 735a 0a66 696c 6573 4d6f  e_namesZ.filesMo
+00000e60: 7665 64da 0966 696c 655f 6e61 6d65 da0d  ved..file_name..
+00000e70: 7265 736f 7572 6365 5f70 6174 685a 1070  resource_pathZ.p
+00000e80: 795f 7265 736f 7572 6365 5f70 6174 68da  y_resource_path.
+00000e90: 0f72 6573 6f75 7263 655f 6d6f 6475 6c65  .resource_module
+00000ea0: 720d 0000 0072 0d00 0000 720e 0000 00da  r....r....r.....
+00000eb0: 1067 656e 6572 6174 654e 6577 4963 6f6e  .generateNewIcon
+00000ec0: 7319 0000 0073 d600 0000 0001 0602 0c01  s....s..........
+00000ed0: 0e01 0402 0a01 0401 0c02 0a01 0a02 0c01  ................
+00000ee0: 1e02 1a02 0e01 0a01 2c02 2c02 1e01 0801  ........,.,.....
+00000ef0: 1401 0802 1401 0801 1c02 0802 0a02 1a01  ................
+00000f00: 3001 1602 1a01 3001 1602 1a01 3001 1a02  0.....0.....0...
+00000f10: 0a02 1201 0802 0c01 0a02 1a01 1602 0e01  ................
+00000f20: 0a02 0e01 0202 1201 1201 2403 1201 0802  ..........$.....
+00000f30: 0c01 0a02 1a01 1602 0e01 0a02 0e01 0202  ................
+00000f40: 1201 1201 2403 1201 0802 0c01 0a02 1a01  ....$...........
+00000f50: 1602 0e01 0a02 0e01 0202 1201 1201 2404  ..............$.
+00000f60: 2003 0401 0402 0a02 0e01 0c02 0e01 0a02   ...............
+00000f70: 0401 0801 0c01 1802 0201 1a01 1201 2803  ..............(.
+00000f80: 0802 1a04 1a01 0e01 3c01 0c01 0c01 0c01  ........<.......
+00000f90: 0c02 0201 0c01 1a01 1001 1202 1a03 0605  ................
+00000fa0: 7a22 4e65 7749 636f 6e73 4765 6e65 7261  z"NewIconsGenera
+00000fb0: 746f 722e 6765 6e65 7261 7465 4e65 7749  tor.generateNewI
+00000fc0: 636f 6e73 6302 0000 0000 0000 0000 0000  consc...........
+00000fd0: 0005 0000 0006 0000 0043 0000 0073 8000  .........C...s..
+00000fe0: 0000 6401 a000 7401 6a02 7403 6a04 6402  ..d...t.j.t.j.d.
+00000ff0: 6403 8d02 a101 7d02 6404 7c02 9b00 6405  d.....}.d.|...d.
+00001000: 9d03 7d03 7405 a006 6406 7c03 a102 0100  ..}.t...d.|.....
+00001010: 7405 a007 a100 4400 5d2a 7d04 7c04 a008  t.....D.]*}.|...
+00001020: 6404 a101 7236 7c04 a009 6405 a101 7236  d...r6|...d...r6
+00001030: 7c04 7c03 6b03 7236 7405 a00a 7c04 a101  |.|.k.r6t...|...
+00001040: 0100 7136 740b a00c 7c03 6400 6407 8502  ..q6t...|.d.d...
+00001050: 1900 a101 7d01 740d 6408 8301 0100 6400  ....}.t.d.....d.
+00001060: 5300 2909 4e72 1400 0000 e908 0000 0029  S.).Nr.........)
+00001070: 01da 016b 5a11 5153 535f 5265 736f 7572  ...kZ.QSS_Resour
+00001080: 6365 735f 7263 5f72 2500 0000 7a13 5153  ces_rc_r%...z.QS
+00001090: 535f 5265 736f 7572 6365 735f 7263 2e70  S_Resources_rc.p
+000010a0: 79e9 fdff ffff 7a0f 7265 736f 7572 6365  y.....z.resource
+000010b0: 206c 6f61 6465 6429 0e72 2c00 0000 da06   loaded).r,.....
+000010c0: 7261 6e64 6f6d da07 6368 6f69 6365 73da  random..choices.
+000010d0: 0673 7472 696e 67da 0f61 7363 6969 5f6c  .string..ascii_l
+000010e0: 6f77 6572 6361 7365 7228 0000 00da 0672  owercaser(.....r
+000010f0: 656e 616d 6572 4900 0000 da0a 7374 6172  enamerI.....star
+00001100: 7473 7769 7468 da08 656e 6473 7769 7468  tswith..endswith
+00001110: da06 7265 6d6f 7665 da09 696d 706f 7274  ..remove..import
+00001120: 6c69 62da 0d69 6d70 6f72 745f 6d6f 6475  lib..import_modu
+00001130: 6c65 7236 0000 0029 0572 0a00 0000 7269  ler6...).r....ri
+00001140: 0000 005a 0b72 616e 646f 6d5f 6e61 6d65  ...Z.random_name
+00001150: 5a11 6e65 775f 7265 736f 7572 6365 5f66  Z.new_resource_f
+00001160: 696c 6572 5f00 0000 720d 0000 0072 0d00  iler_...r....r..
+00001170: 0000 720e 0000 00da 1072 656c 6f61 645f  ..r......reload_
+00001180: 7265 736f 7572 6365 73c1 0000 0073 1000  resources....s..
+00001190: 0000 0002 1601 0c03 0c03 0c01 1c01 0c03  ................
+000011a0: 1202 7a22 4e65 7749 636f 6e73 4765 6e65  ..z"NewIconsGene
+000011b0: 7261 746f 722e 7265 6c6f 6164 5f72 6573  rator.reload_res
+000011c0: 6f75 7263 6573 6302 0000 0000 0000 0000  ourcesc.........
+000011d0: 0000 001c 0000 000d 0000 0043 0000 0073  ...........C...s
+000011e0: ba05 0000 7400 8300 7d02 7401 6a02 a003  ....t...}.t.j...
+000011f0: 7404 a101 7d03 7401 6a02 a005 7c03 6401  t...}.t.j...|.d.
+00001200: a102 7d04 6700 7d05 6402 7d06 7c00 6a06  ..}.g.}.d.}.|.j.
+00001210: 6a07 4400 9005 5d82 7d07 7c02 a008 6403  j.D...].}.|...d.
+00001220: a101 7d08 7c00 6a09 7254 740a 6404 7c07  ..}.|.j.rTt.d.|.
+00001230: 6a0b 1700 8301 0100 740c 7c07 6405 8302  j.......t.|.d...
+00001240: 7280 7c07 6a0d 6406 6b03 7274 740e 7c07  r.|.j.d.k.rtt.|.
+00001250: 6a0d 8301 7d09 71f4 740e 7c07 6a0f 8301  j...}.q.t.|.j...
+00001260: 7d09 6e74 7c08 6407 6b02 72b0 7410 8300  }.nt|.d.k.r.t...
+00001270: 7d0a 7c0a 6a11 6406 6b02 72a4 740e 7c0a  }.|.j.d.k.r.t.|.
+00001280: 6a12 8301 7d09 71f4 740e 7c0a 6a11 8301  j...}.q.t.|.j...
+00001290: 7d09 6e44 7c08 6408 6b02 72e0 7413 8300  }.nD|.d.k.r.t...
+000012a0: 7d0a 7c0a 6a11 6406 6b02 72d4 740e 7c0a  }.|.j.d.k.r.t.|.
+000012b0: 6a12 8301 7d09 71f4 740e 7c0a 6a11 8301  j...}.q.t.|.j...
+000012c0: 7d09 6e14 7c00 6a09 7230 740a 6409 7c07  }.n.|.j.r0t.d.|.
+000012d0: 6a0b 8302 0100 7130 7414 7c09 640a 8302  j.....q0t.|.d...
+000012e0: 7d0b 7414 7c09 640b 8302 7d0c 7c09 a015  }.t.|.d...}.|...
+000012f0: 640c 6406 a102 7d0d 7401 6a02 a016 7401  d.d...}.t.j...t.
+00001300: 6a02 a005 7401 a017 a100 640d 7c0d 1700  j...t.....d.|...
+00001310: a102 a101 7d0e 7c00 6a09 9001 7246 740a  ....}.|.j...rFt.
+00001320: 640e 7c09 640f 8303 0100 7401 a018 7c04  d.|.d.....t...|.
+00001330: a101 4400 5d2c 5c03 7d0f 7d10 7d11 7c11  ..D.],\.}.}.}.|.
+00001340: 4400 5d1a 7d12 7c05 a019 7401 6a02 a005  D.].}.|...t.j...
+00001350: 7c0f 7c12 a102 a101 0100 9001 715e 9001  |.|.........q^..
+00001360: 7150 741a 7c05 8301 7d13 7c05 4400 9004  qPt.|...}.|.D...
+00001370: 5d26 7d14 741b 6a1c 7c14 6410 6411 6412  ]&}.t.j.|.d.d.d.
+00001380: 8d03 9001 8f00 7d15 7c15 a01d a100 7d16  ......}.|.....}.
+00001390: 7c16 a015 7c06 7c09 a102 7d17 740e a01e  |...|.|...}.t...
+000013a0: 7c17 a101 7d18 7401 6a02 a01f 7420 7c14  |...}.t.j...t |.
+000013b0: 8301 6a02 a101 a015 6413 6414 a102 7d19  ..j.....d.d...}.
+000013c0: 7401 6a02 a016 7401 6a02 a005 7c0e 7c19  t.j...t.j...|.|.
+000013d0: a102 a101 7d04 7401 6a02 a021 7c0e a101  ....}.t.j..!|...
+000013e0: 9002 730a 7401 a022 7c0e a101 0100 7401  ..s.t.."|.....t.
+000013f0: 6a02 a021 7c04 a101 9002 7228 5700 3500  j..!|.....r(W.5.
+00001400: 5100 5200 a300 9001 718a 6e36 7c02 a008  Q.R.....q.n6|...
+00001410: 6415 a101 6400 6b09 9002 725e 7c02 a008  d...d.k...r^|...
+00001420: 6415 a101 a015 640c 6406 a102 7c0d 6b02  d.....d.d...|.k.
+00001430: 9002 725e 5700 3500 5100 5200 a300 9001  ..r^W.5.Q.R.....
+00001440: 718a 7a12 7423 6a24 7c18 7c04 6416 8d02  q.z.t#j$|.|.d...
+00001450: 0100 5700 6e2c 0400 7425 6b0a 9002 729c  ..W.n,..t%k...r.
+00001460: 0100 7d1a 0100 7a0c 740a 7c1a 8301 0100  ..}...z.t.|.....
+00001470: 5700 3500 6400 7d1a 7e1a 5800 5900 6e02  W.5.d.}.~.X.Y.n.
+00001480: 5800 5700 3500 5100 5200 5800 741b 6a1c  X.W.5.Q.R.X.t.j.
+00001490: 7c14 6410 6411 6412 8d03 9001 8f5e 7d15  |.d.d.d......^}.
+000014a0: 7c15 a01d a100 7d16 7c16 a015 7c06 7c0b  |.....}.|...|.|.
+000014b0: a102 7d17 740e a01e 7c17 a101 7d18 7401  ..}.t...|...}.t.
+000014c0: 6a02 a01f 7420 7c14 8301 6a02 a101 a015  j...t |...j.....
+000014d0: 6413 6417 a102 7d19 7401 6a02 a016 7401  d.d...}.t.j...t.
+000014e0: 6a02 a005 7c0e 7c19 a102 a101 7d04 7401  j...|.|.....}.t.
+000014f0: 6a02 a021 7c0e a101 9003 7322 7401 a022  j..!|.....s"t.."
+00001500: 7c0e a101 0100 7401 6a02 a021 7c04 a101  |.....t.j..!|...
+00001510: 9003 7240 5700 3500 5100 5200 a300 9001  ..r@W.5.Q.R.....
+00001520: 718a 6e7e 7c02 a008 6415 a101 6400 6b09  q.n~|...d...d.k.
+00001530: 9003 72be 7c02 a008 6415 a101 a015 640c  ..r.|...d.....d.
+00001540: 6406 a102 7c0d 6b02 9003 72be 7401 6a02  d...|.k...r.t.j.
+00001550: a016 7401 6a02 a005 7401 a017 a100 6418  ..t.j...t.....d.
+00001560: a102 a101 7d1b 7401 6a02 a021 7401 6a02  ....}.t.j..!t.j.
+00001570: a005 7c1b 7c19 a102 a101 9003 72be 7426  ..|.|.......r.t&
+00001580: a027 7401 6a02 a005 7c1b 7c19 a102 7c0e  .'t.j...|.|...|.
+00001590: a102 0100 5700 3500 5100 5200 a300 9001  ....W.5.Q.R.....
+000015a0: 718a 7401 6a02 a016 7401 6a02 a005 7c0e  q.t.j...t.j...|.
+000015b0: 7c19 a102 a101 7d04 7a12 7423 6a24 7c18  |.....}.z.t#j$|.
+000015c0: 7c04 6416 8d02 0100 5700 6e2c 0400 7425  |.d.....W.n,..t%
+000015d0: 6b0a 9004 7212 0100 7d1a 0100 7a0c 740a  k...r...}...z.t.
+000015e0: 7c1a 8301 0100 5700 3500 6400 7d1a 7e1a  |.....W.5.d.}.~.
+000015f0: 5800 5900 6e02 5800 5700 3500 5100 5200  X.Y.n.X.W.5.Q.R.
+00001600: 5800 741b 6a1c 7c14 6410 6411 6412 8d03  X.t.j.|.d.d.d...
+00001610: 9001 8f5e 7d15 7c15 a01d a100 7d16 7c16  ...^}.|.....}.|.
+00001620: a015 7c06 7c0c a102 7d17 740e a01e 7c17  ..|.|...}.t...|.
+00001630: a101 7d18 7401 6a02 a01f 7420 7c14 8301  ..}.t.j...t |...
+00001640: 6a02 a101 a015 6413 6419 a102 7d19 7401  j.....d.d...}.t.
+00001650: 6a02 a016 7401 6a02 a005 7c0e 7c19 a102  j...t.j...|.|...
+00001660: a101 7d04 7401 6a02 a021 7c0e a101 9004  ..}.t.j..!|.....
+00001670: 7398 7401 a022 7c0e a101 0100 7401 6a02  s.t.."|.....t.j.
+00001680: a021 7c04 a101 9004 72b6 5700 3500 5100  .!|.....r.W.5.Q.
+00001690: 5200 a300 9001 718a 6e7e 7c02 a008 6415  R.....q.n~|...d.
+000016a0: a101 6400 6b09 9005 7234 7c02 a008 6415  ..d.k...r4|...d.
+000016b0: a101 a015 640c 6406 a102 7c0d 6b02 9005  ....d.d...|.k...
+000016c0: 7234 7401 6a02 a016 7401 6a02 a005 7401  r4t.j...t.j...t.
+000016d0: a017 a100 6418 a102 a101 7d1b 7401 6a02  ....d.....}.t.j.
+000016e0: a021 7401 6a02 a005 7c1b 7c19 a102 a101  .!t.j...|.|.....
+000016f0: 9005 7234 7426 a027 7401 6a02 a005 7c1b  ..r4t&.'t.j...|.
+00001700: 7c19 a102 7c0e a102 0100 5700 3500 5100  |...|.....W.5.Q.
+00001710: 5200 a300 9001 718a 7401 6a02 a016 7401  R.....q.t.j...t.
+00001720: 6a02 a005 7c0e 7c19 a102 a101 7d04 7a12  j...|.|.....}.z.
+00001730: 7423 6a24 7c18 7c04 6416 8d02 0100 5700  t#j$|.|.d.....W.
+00001740: 6e2c 0400 7425 6b0a 9005 7288 0100 7d1a  n,..t%k...r...}.
+00001750: 0100 7a0c 740a 7c1a 8301 0100 5700 3500  ..z.t.|.....W.5.
+00001760: 6400 7d1a 7e1a 5800 5900 6e02 5800 5700  d.}.~.X.Y.n.X.W.
+00001770: 3500 5100 5200 5800 7c01 a028 7429 7c05  5.Q.R.X.|..(t)|.
+00001780: a02a 7c14 a101 7c13 1b00 641a 1400 8301  .*|...|...d.....
+00001790: a101 0100 9001 718a 7130 6400 5300 291b  ......q.q0d.S.).
+000017a0: 4e72 0f00 0000 7210 0000 00da 0554 4845  Nr....r......THE
+000017b0: 4d45 7a13 4368 6563 6b69 6e67 2069 636f  MEz.Checking ico
+000017c0: 6e73 2066 6f72 20da 0a69 636f 6e73 436f  ns for ..iconsCo
+000017d0: 6c6f 7272 1400 0000 da05 4c49 4748 54da  lorr......LIGHT.
+000017e0: 0444 4152 4b7a 224e 6f20 6963 6f6e 7320  .DARKz"No icons 
+000017f0: 636f 6c6f 7220 7370 6563 6966 6965 6420  color specified 
+00001800: 666f 7220 7468 656d 6572 1100 0000 7212  for themer....r.
+00001810: 0000 0072 1300 0000 7215 0000 007a 2747  ...r....r....z'G
+00001820: 656e 6572 6174 696e 6720 6d69 7373 696e  enerating missin
+00001830: 6720 6963 6f6e 7320 666f 7220 796f 7572  g icons for your
+00001840: 2074 6865 6d65 7a1f 706c 6561 7365 2077   themez.please w
+00001850: 6169 742e 2054 6869 7320 6d61 7920 7461  ait. This may ta
+00001860: 6b65 206c 6f6e 6772 1c00 0000 721d 0000  ke longr....r...
+00001870: 0072 1e00 0000 7218 0000 0072 1900 0000  .r....r....r....
+00001880: 7217 0000 0072 2100 0000 721a 0000 0072  r....r!...r....r
+00001890: 1600 0000 721b 0000 0072 2200 0000 292b  ....r....r"...)+
+000018a0: 7227 0000 0072 2800 0000 7229 0000 0072  r'...r(...r)...r
+000018b0: 2a00 0000 722b 0000 0072 2c00 0000 da02  *...r+...r,.....
+000018c0: 7569 da06 7468 656d 6573 7234 0000 0072  ui..themesr4...r
+000018d0: 3500 0000 7236 0000 0072 4a00 0000 da07  5...r6...rJ.....
+000018e0: 6861 7361 7474 7272 7a00 0000 722f 0000  hasattrrz...r/..
+000018f0: 00da 0b61 6363 656e 7443 6f6c 6f72 da05  ...accentColor..
+00001900: 4c69 6768 74da 0b69 636f 6e73 5f63 6f6c  Light..icons_col
+00001910: 6f72 da0c 6163 6365 6e74 5f63 6f6c 6f72  or..accent_color
+00001920: da04 4461 726b 7230 0000 0072 3100 0000  ..Darkr0...r1...
+00001930: 7232 0000 0072 3300 0000 7237 0000 0072  r2...r3...r7...r
+00001940: 3800 0000 7239 0000 0072 3e00 0000 723f  8...r9...r>...r?
+00001950: 0000 0072 4000 0000 7241 0000 0072 3a00  ...r@...rA...r:.
+00001960: 0000 7202 0000 0072 3b00 0000 7242 0000  ..r....r;...rB..
+00001970: 0072 4300 0000 7244 0000 0072 4500 0000  .rC...rD...rE...
+00001980: 723c 0000 0072 3d00 0000 7246 0000 0072  r<...r=...rF...r
+00001990: 4700 0000 7248 0000 0029 1c72 0a00 0000  G...rH...).r....
+000019a0: 724f 0000 0072 5000 0000 722a 0000 0072  rO...rP...r*...r
+000019b0: 5100 0000 7252 0000 0072 5400 0000 da05  Q...rR...rT.....
+000019c0: 7468 656d 6572 7900 0000 7255 0000 005a  themery...rU...Z
+000019d0: 0d74 6865 6d65 5072 6f70 6572 7479 7256  .themePropertyrV
+000019e0: 0000 0072 5700 0000 7258 0000 0072 5900  ...rW...rX...rY.
+000019f0: 0000 725c 0000 0072 5d00 0000 725e 0000  ..r\...r]...r^..
+00001a00: 0072 5f00 0000 7260 0000 0072 4a00 0000  .r_...r`...rJ...
+00001a10: 7262 0000 0072 6300 0000 7264 0000 0072  rb...rc...rd...r
+00001a20: 6500 0000 7261 0000 0072 6600 0000 725a  e...ra...rf...rZ
+00001a30: 0000 0072 0d00 0000 720d 0000 0072 0e00  ...r....r....r..
+00001a40: 0000 724e 0000 00d3 0000 0073 bc00 0000  ..rN.......s....
+00001a50: 0001 0602 0c01 0e01 0402 0402 0e01 0a04  ................
+00001a60: 0601 0e03 0a01 0a01 0c02 0c02 0801 0601  ................
+00001a70: 0a01 0c02 0c02 0801 0601 0a01 0c02 0c03  ................
+00001a80: 0601 0c01 0202 0a01 0a02 0c02 1e02 0801  ................
+00001a90: 0c02 1401 0801 1c02 0801 0a02 1401 0802  ................
+00001aa0: 0c01 0a02 1a01 1602 0e01 0a02 0e01 1002  ................
+00001ab0: 2801 0e01 0202 1201 1201 2403 1401 0802  (.........$.....
+00001ac0: 0c01 0a02 1a01 1602 0e01 0a02 0e01 1002  ................
+00001ad0: 2802 1a02 1801 1601 0e02 1601 0202 1201  (...............
+00001ae0: 1201 2403 1401 0802 0c01 0a02 1a01 1602  ..$.............
+00001af0: 0e01 0a02 0e01 1002 2802 1a02 1801 1601  ........(.......
+00001b00: 0e02 1601 0201 1201 1201 2404 7a22 4e65  ..........$.z"Ne
+00001b10: 7749 636f 6e73 4765 6e65 7261 746f 722e  wIconsGenerator.
+00001b20: 6765 6e65 7261 7465 416c 6c49 636f 6e73  generateAllIcons
+00001b30: 2909 da08 5f5f 6e61 6d65 5f5f da0a 5f5f  )...__name__..__
+00001b40: 6d6f 6475 6c65 5f5f da0c 5f5f 7175 616c  module__..__qual
+00001b50: 6e61 6d65 5f5f da07 5f5f 646f 635f 5f72  name__..__doc__r
+00001b60: 0800 0000 726a 0000 0072 7800 0000 724e  ....rj...rx...rN
+00001b70: 0000 00da 0d5f 5f63 6c61 7373 6365 6c6c  .....__classcell
+00001b80: 5f5f 720d 0000 0072 0d00 0000 720b 0000  __r....r....r...
+00001b90: 0072 0e00 0000 7206 0000 0013 0000 0073  .r....r........s
+00001ba0: 0c00 0000 0801 0401 0c04 087f 0029 0812  .............)..
+00001bb0: 7206 0000 0029 1172 4300 0000 723e 0000  r....).rC...r>..
+00001bc0: 0072 2800 0000 da03 7379 7372 3c00 0000  .r(.....sysr<...
+00001bd0: 7276 0000 0072 6e00 0000 7270 0000 00da  rv...rn...rp....
+00001be0: 0c75 726c 6c69 622e 7061 7273 6572 0200  .urllib.parser..
+00001bf0: 0000 da07 7061 7468 6c69 6272 0300 0000  ....pathlibr....
+00001c00: da08 5f5f 6d61 696e 5f5f da0b 636f 6c6f  ..__main__..colo
+00001c10: 7273 7973 7465 6d72 2700 0000 7250 0000  rsystemr'...rP..
+00001c20: 0072 0600 0000 720d 0000 0072 0d00 0000  .r....r....r....
+00001c30: 720d 0000 0072 0e00 0000 da08 3c6d 6f64  r....r......<mod
+00001c40: 756c 653e 0100 0000 731a 0000 0008 0108  ule>....s.......
+00001c50: 0108 0108 0108 0108 0108 0108 010c 010c  ................
+00001c60: 0108 0408 0206 02                        .......
```

### Comparing `QT-PyQt-PySide-Custom-Widgets-0.6.5/Custom_Widgets/Qss/__pycache__/SvgToPngIcons.cpython-39.pyc` & `QT-PyQt-PySide-Custom-Widgets-0.6.6/Custom_Widgets/Qss/__pycache__/SvgToPngIcons.cpython-39.pyc`

 * *Files identical despite different names*

### Comparing `QT-PyQt-PySide-Custom-Widgets-0.6.5/Custom_Widgets/Qss/__pycache__/colorsystem.cpython-310.pyc` & `QT-PyQt-PySide-Custom-Widgets-0.6.6/Custom_Widgets/Qss/__pycache__/colorsystem.cpython-310.pyc`

 * *Files identical despite different names*

### Comparing `QT-PyQt-PySide-Custom-Widgets-0.6.5/Custom_Widgets/Qss/__pycache__/colorsystem.cpython-37.pyc` & `QT-PyQt-PySide-Custom-Widgets-0.6.6/Custom_Widgets/Qss/__pycache__/colorsystem.cpython-37.pyc`

 * *Files identical despite different names*

### Comparing `QT-PyQt-PySide-Custom-Widgets-0.6.5/Custom_Widgets/Qss/__pycache__/colorsystem.cpython-38.pyc` & `QT-PyQt-PySide-Custom-Widgets-0.6.6/Custom_Widgets/Qss/__pycache__/colorsystem.cpython-38.pyc`

 * *Format-specific differences are supported for Python .pyc files but no file-specific differences were detected; falling back to a binary diff. file(1) reports: Byte-compiled Python module for CPython 3.8, timestamp-based, .py timestamp: Wed Jun 21 21:05:04 2023 UTC, .py size: 10048 bytes*

 * *Could not decompile bytecode: bad marshal data (unknown type code)*

 * *Files 7% similar despite different names*

```diff
@@ -1,406 +1,406 @@
-00000000: 550d 0d0a 0000 0000 0066 9364 4027 0000  U........f.d@'..
+00000000: 550d 0d0a 0000 0000 e5fc 9664 5d28 0000  U..........d](..
 00000010: e300 0000 0000 0000 0000 0000 0000 0000  ................
 00000020: 0004 0000 0040 0000 0073 9400 0000 6400  .....@...s....d.
 00000030: 6401 6c00 5a00 6400 6401 6c01 5a01 6400  d.l.Z.d.d.l.Z.d.
 00000040: 6402 6c02 5400 6400 6401 6c03 6d04 5a05  d.l.T.d.d.l.m.Z.
 00000050: 0100 6400 6401 6c06 5a06 6507 8300 5a08  ..d.d.l.Z.e...Z.
 00000060: 6412 6404 6405 8401 5a09 6406 6407 8400  d.d.d...Z.d.d...
 00000070: 5a0a 4700 6408 6409 8400 6409 8302 5a0b  Z.G.d.d...d...Z.
 00000080: 4700 640a 640b 8400 640b 650b 8303 5a0c  G.d.d...d.e...Z.
 00000090: 4700 640c 640d 8400 640d 650b 8303 5a0d  G.d.d...d.e...Z.
 000000a0: 4700 640e 640f 8400 640f 8302 5a0e 4700  G.d.d...d...Z.G.
 000000b0: 6410 6411 8400 6411 650f 8303 5a10 6401  d.d...d.e...Z.d.
 000000c0: 5300 2913 e900 0000 004e 2901 da01 2ae7  S.)......N)...*.
 000000d0: 0000 0000 0000 e03f 6302 0000 0000 0000  .......?c.......
-000000e0: 0000 0000 0005 0000 0008 0000 0043 0000  .............C..
-000000f0: 0073 c800 0000 7a0e 7400 6a01 7c00 1900  .s....z.t.j.|...
+000000e0: 0000 0000 0008 0000 0008 0000 0043 0000  .............C..
+000000f0: 0073 a000 0000 7a0e 7400 6a01 7c00 1900  .s....z.t.j.|...
 00000100: 7d02 5700 6e18 0400 7402 6b0a 7226 0100  }.W.n...t.k.r&..
 00000110: 0100 0100 7c00 7d02 5900 6e02 5800 7403  ....|.}.Y.n.X.t.
-00000120: 6a04 7400 a005 7c02 a101 8e00 7d02 7406  j.t...|.....}.t.
-00000130: 7c02 8301 0100 7c02 6401 1900 6402 6b04  |.....|.d...d.k.
-00000140: 726c 7403 a007 7c02 6402 1900 7c01 7c02  rlt...|.d...|.|.
-00000150: 6401 1900 1400 7c02 6403 1900 a103 7d03  d.....|.d.....}.
-00000160: 6e26 7403 a007 7c02 6402 1900 6401 7c01  n&t...|.d...d.|.
-00000170: 6401 7c02 6401 1900 1800 1400 1800 7c02  d.|.d.........|.
-00000180: 6403 1900 a103 7d03 7408 7409 7c03 6402  d.....}.t.t.|.d.
-00000190: 1900 6404 1400 8301 7409 7c03 6401 1900  ..d.....t.|.d...
-000001a0: 6404 1400 8301 7409 7c03 6403 1900 6404  d.....t.|.d...d.
-000001b0: 1400 8301 6603 8301 7d04 7c04 5300 2905  ....f...}.|.S.).
-000001c0: 4ee9 0100 0000 7201 0000 00e9 0200 0000  N.....r.........
-000001d0: e9fa 0000 0029 0ada 026d 635a 0663 6e61  .....)...mcZ.cna
-000001e0: 6d65 73da 084b 6579 4572 726f 72da 0863  mes..KeyError..c
-000001f0: 6f6c 6f72 7379 735a 0a72 6762 5f74 6f5f  olorsysZ.rgb_to_
-00000200: 686c 735a 0674 6f5f 7267 62da 0570 7269  hlsZ.to_rgb..pri
-00000210: 6e74 5a0a 686c 735f 746f 5f72 6762 da0a  ntZ.hls_to_rgb..
-00000220: 7267 625f 746f 5f68 6578 da03 696e 7429  rgb_to_hex..int)
-00000230: 05da 0563 6f6c 6f72 da06 616d 6f75 6e74  ...color..amount
-00000240: da01 63da 0372 6762 5a09 6e65 775f 636f  ..c..rgbZ.new_co
-00000250: 6c6f 72a9 0072 1100 0000 fa46 653a 5c53  lor..r.....Fe:\S
-00000260: 7069 6e6e 2054 6173 6b5c 3070 6173 735c  pinn Task\0pass\
-00000270: 3070 6173 732d 6170 702d 6d61 7374 6572  0pass-app-master
-00000280: 5c43 7573 746f 6d5f 5769 6467 6574 735c  \Custom_Widgets\
-00000290: 5173 735c 636f 6c6f 7273 7973 7465 6d2e  Qss\colorsystem.
-000002a0: 7079 da10 6164 6a75 7374 5f6c 6967 6874  py..adjust_light
-000002b0: 6e65 7373 1e00 0000 7316 0000 0000 0102  ness....s.......
-000002c0: 010e 010e 010a 0110 0108 020c 0120 0226  ............. .&
-000002d0: 0232 0172 1300 0000 6301 0000 0000 0000  .2.r....c.......
-000002e0: 0000 0000 0002 0000 0002 0000 0043 0000  .............C..
-000002f0: 0073 1000 0000 6401 7c00 1600 7d01 6402  .s....d.|...}.d.
-00000300: 7c01 1700 5300 2903 4e7a 0c25 3032 7825  |...S.).Nz.%02x%
-00000310: 3032 7825 3032 78fa 0123 7211 0000 0029  02x%02x..#r....)
-00000320: 0272 1000 0000 5a09 6865 785f 636f 6c6f  .r....Z.hex_colo
-00000330: 7272 1100 0000 7211 0000 0072 1200 0000  rr....r....r....
-00000340: 720b 0000 002f 0000 0073 0400 0000 0001  r..../...s......
-00000350: 0801 720b 0000 0063 0000 0000 0000 0000  ..r....c........
-00000360: 0000 0000 0000 0000 0300 0000 4000 0000  ............@...
-00000370: 7316 0000 0065 005a 0164 005a 0264 0564  s....e.Z.d.Z.d.d
-00000380: 0264 0384 015a 0364 0453 0029 06da 0554  .d...Z.d.S.)...T
-00000390: 6865 6d65 da00 6305 0000 0000 0000 0000  heme..c.........
-000003a0: 0000 0005 0000 0003 0000 0043 0000 0073  ...........C...s
-000003b0: ca00 0000 7c01 7c00 5f00 7c02 7c00 5f01  ....|.|._.|.|._.
-000003c0: 7c03 7c00 5f02 7c04 7c00 5f03 7404 7c01  |.|._.|.|._.t.|.
-000003d0: 6401 8302 7c00 5f05 7404 7c01 6402 8302  d...|._.t.|.d...
-000003e0: 7c00 5f06 7404 7c01 6403 8302 7c00 5f07  |._.t.|.d...|._.
-000003f0: 7404 7c01 6404 8302 7c00 5f08 7404 7c01  t.|.d...|._.t.|.
-00000400: 6405 8302 7c00 5f09 7404 7c01 6406 8302  d...|._.t.|.d...
-00000410: 7c00 5f0a 7404 7c02 6401 8302 7c00 5f0b  |._.t.|.d...|._.
-00000420: 7404 7c02 6407 8302 7c00 5f0c 7404 7c02  t.|.d...|._.t.|.
-00000430: 6403 8302 7c00 5f0d 7404 7c02 6408 8302  d...|._.t.|.d...
-00000440: 7c00 5f0e 7404 7c03 6401 8302 7c00 5f0f  |._.t.|.d...|._.
-00000450: 7404 7c03 6407 8302 7c00 5f10 7404 7c03  t.|.d...|._.t.|.
-00000460: 6403 8302 7c00 5f11 7404 7c03 6408 8302  d...|._.t.|.d...
-00000470: 7c00 5f12 6409 7c00 5f13 6400 5300 290a  |._.d.|._.d.S.).
-00000480: 4e72 0400 0000 6766 6666 6666 66ee 3fe7  Nr....gffffff.?.
-00000490: 9a99 9999 9999 e93f 6700 0000 0000 00e8  .......?g.......
-000004a0: 3fe7 3333 3333 3333 e33f 679a 9999 9999  ?.333333.?g.....
-000004b0: 99e1 3fe7 cdcc cccc cccc ec3f e766 6666  ..?........?.fff
-000004c0: 6666 66e6 3ffa 0e3a 2f69 636f 6e73 2f49  fff.?..:/icons/I
-000004d0: 636f 6e73 2f29 14da 0862 675f 636f 6c6f  cons/)...bg_colo
-000004e0: 72da 0974 7874 5f63 6f6c 6f72 da0c 6163  r..txt_color..ac
-000004f0: 6365 6e74 5f63 6f6c 6f72 da0b 6963 6f6e  cent_color..icon
-00000500: 735f 636f 6c6f 7272 1300 0000 da04 4247  s_colorr......BG
-00000510: 5f31 da04 4247 5f32 da04 4247 5f33 da04  _1..BG_2..BG_3..
-00000520: 4247 5f34 da04 4247 5f35 da04 4247 5f36  BG_4..BG_5..BG_6
-00000530: da04 4354 5f31 da04 4354 5f32 da04 4354  ..CT_1..CT_2..CT
-00000540: 5f33 da04 4354 5f34 da04 4341 5f31 da04  _3..CT_4..CA_1..
-00000550: 4341 5f32 da04 4341 5f33 da04 4341 5f34  CA_2..CA_3..CA_4
-00000560: da05 4943 4f4e 5329 05da 0473 656c 6672  ..ICONS)...selfr
-00000570: 1c00 0000 721d 0000 0072 1e00 0000 721f  ....r....r....r.
-00000580: 0000 0072 1100 0000 7211 0000 0072 1200  ...r....r....r..
-00000590: 0000 da08 5f5f 696e 6974 5f5f 3400 0000  ....__init__4...
-000005a0: 7326 0000 0000 0106 0106 0106 0106 020c  s&..............
-000005b0: 010c 010c 010c 010c 010c 020c 010c 010c  ................
-000005c0: 010c 020c 010c 010c 010c 027a 0e54 6865  ...........z.The
-000005d0: 6d65 2e5f 5f69 6e69 745f 5f4e 2901 7216  me.__init__N).r.
-000005e0: 0000 0029 04da 085f 5f6e 616d 655f 5fda  ...)...__name__.
-000005f0: 0a5f 5f6d 6f64 756c 655f 5fda 0c5f 5f71  .__module__..__q
-00000600: 7561 6c6e 616d 655f 5f72 3000 0000 7211  ualname__r0...r.
-00000610: 0000 0072 1100 0000 7211 0000 0072 1200  ...r....r....r..
-00000620: 0000 7215 0000 0033 0000 0073 0200 0000  ..r....3...s....
-00000630: 0801 7215 0000 0063 0000 0000 0000 0000  ..r....c........
-00000640: 0000 0000 0000 0000 0300 0000 0000 0000  ................
-00000650: 731c 0000 0065 005a 0164 005a 0287 0066  s....e.Z.d.Z...f
-00000660: 0164 0164 0284 085a 0387 0004 005a 0453  .d.d...Z.....Z.S
-00000670: 0029 03da 0444 6172 6b63 0100 0000 0000  .)...Darkc......
-00000680: 0000 0000 0000 0100 0000 0500 0000 0300  ................
-00000690: 0000 7314 0000 0074 0083 00a0 0164 0164  ..s....t.....d.d
-000006a0: 0264 03a1 0301 0064 0053 0029 044e 7a07  .d.....d.S.).Nz.
-000006b0: 2330 4430 4431 34fa 0423 6666 667a 0723  #0D0D14..#fffz.#
-000006c0: 4138 4239 4244 a902 da05 7375 7065 7272  A8B9BD....superr
-000006d0: 3000 0000 a901 722f 0000 00a9 01da 095f  0.....r/......._
-000006e0: 5f63 6c61 7373 5f5f 7211 0000 0072 1200  _class__r....r..
-000006f0: 0000 7230 0000 004e 0000 0073 0200 0000  ..r0...N...s....
-00000700: 0001 7a0d 4461 726b 2e5f 5f69 6e69 745f  ..z.Dark.__init_
-00000710: 5fa9 0572 3100 0000 7232 0000 0072 3300  _..r1...r2...r3.
-00000720: 0000 7230 0000 00da 0d5f 5f63 6c61 7373  ..r0.....__class
-00000730: 6365 6c6c 5f5f 7211 0000 0072 1100 0000  cell__r....r....
-00000740: 7239 0000 0072 1200 0000 7234 0000 004d  r9...r....r4...M
-00000750: 0000 0073 0200 0000 0801 7234 0000 0063  ...s......r4...c
-00000760: 0000 0000 0000 0000 0000 0000 0000 0000  ................
-00000770: 0300 0000 0000 0000 731c 0000 0065 005a  ........s....e.Z
-00000780: 0164 005a 0287 0066 0164 0164 0284 085a  .d.Z...f.d.d...Z
-00000790: 0387 0004 005a 0453 0029 03da 054c 6967  .....Z.S.)...Lig
-000007a0: 6874 6301 0000 0000 0000 0000 0000 0001  htc.............
-000007b0: 0000 0005 0000 0003 0000 0073 1400 0000  ...........s....
-000007c0: 7400 8300 a001 6401 6402 6403 a103 0100  t.....d.d.d.....
-000007d0: 6400 5300 2904 4e72 3500 0000 7a04 2330  d.S.).Nr5...z.#0
-000007e0: 3030 7a07 2330 3062 6366 6672 3600 0000  00z.#00bcffr6...
-000007f0: 7238 0000 0072 3900 0000 7211 0000 0072  r8...r9...r....r
-00000800: 1200 0000 7230 0000 0052 0000 0073 0200  ....r0...R...s..
-00000810: 0000 0001 7a0e 4c69 6768 742e 5f5f 696e  ....z.Light.__in
-00000820: 6974 5f5f 723b 0000 0072 1100 0000 7211  it__r;...r....r.
-00000830: 0000 0072 3900 0000 7212 0000 0072 3d00  ...r9...r....r=.
-00000840: 0000 5100 0000 7302 0000 0008 0172 3d00  ..Q...s......r=.
-00000850: 0000 6300 0000 0000 0000 0000 0000 0000  ..c.............
-00000860: 0000 0004 0000 0000 0000 0073 2e00 0000  ...........s....
-00000870: 6500 5a01 6400 5a02 6408 8700 6601 6402  e.Z.d.Z.d...f.d.
-00000880: 6403 8409 5a03 6404 6405 8400 5a04 6406  d...Z.d.d...Z.d.
-00000890: 6407 8400 5a05 8700 0400 5a06 5300 2909  d...Z.....Z.S.).
-000008a0: da13 4372 6561 7465 436f 6c6f 7256 6172  ..CreateColorVar
-000008b0: 6961 626c 654e 6302 0000 0000 0000 0000  iableNc.........
-000008c0: 0000 0002 0000 0003 0000 0003 0000 0073  ...............s
-000008d0: 1400 0000 7400 7401 7c00 8302 a002 7c01  ....t.t.|.....|.
-000008e0: a101 0100 6400 5300 2901 4e29 0372 3700  ....d.S.).N).r7.
-000008f0: 0000 723e 0000 0072 3000 0000 2902 722f  ..r>...r0...).r/
-00000900: 0000 00da 0670 6172 656e 7472 3900 0000  .....parentr9...
-00000910: 7211 0000 0072 1200 0000 7230 0000 005e  r....r....r0...^
-00000920: 0000 0073 0200 0000 0001 7a1c 4372 6561  ...s......z.Crea
-00000930: 7465 436f 6c6f 7256 6172 6961 626c 652e  teColorVariable.
-00000940: 5f5f 696e 6974 5f5f 6301 0000 0000 0000  __init__c.......
-00000950: 0000 0000 0009 0000 0006 0000 0043 0000  .............C..
-00000960: 0073 5001 0000 7400 8300 7d01 7c01 a001  .sP...t...}.|...
-00000970: 6401 a101 7d02 6900 7d03 7c02 6402 6b02  d...}.i.}.|.d.k.
-00000980: 7258 7402 8300 7d04 7c04 6a03 6403 6b02  rXt...}.|.j.d.k.
-00000990: 723c 7c04 6a04 7d05 7c04 6a04 7c04 5f03  r<|.j.}.|.j.|._.
-000009a0: 6e06 7c04 6a03 7d05 7c04 6a05 7c04 6a06  n.|.j.}.|.j.|.j.
-000009b0: 7c04 6a04 7c05 6404 9c04 7d03 6eb2 7c02  |.j.|.d...}.n.|.
-000009c0: 6405 6b02 729c 7407 8300 7d04 7c04 6a03  d.k.r.t...}.|.j.
-000009d0: 6403 6b02 7280 7c04 6a04 7d05 7c04 6a04  d.k.r.|.j.}.|.j.
-000009e0: 7c04 5f03 6e06 7c04 6a03 7d05 7c04 6a05  |._.n.|.j.}.|.j.
-000009f0: 7c04 6a06 7c04 6a04 7c05 6404 9c04 7d03  |.j.|.j.|.d...}.
-00000a00: 6e6e 7c00 6a08 6a09 4400 5d64 7d04 7c04  nn|.j.j.D.]d}.|.
-00000a10: 6a0a 73b8 7c04 6a0b 7c02 6b02 72a4 7c01  j.s.|.j.|.k.r.|.
-00000a20: a00c 6401 7c04 6a0b a102 0100 7c04 6a0d  ..d.|.j.....|.j.
-00000a30: 7d06 7c04 6a0e 7d07 7c04 6a0f 7d08 7c04  }.|.j.}.|.j.}.|.
-00000a40: 6a10 72f6 7c04 6a11 6403 6b02 72ee 7c08  j.r.|.j.d.k.r.|.
-00000a50: 7d05 71fa 7c04 6a11 7d05 6e04 6400 7d05  }.q.|.j.}.n.d.}.
-00000a60: 7c06 7c07 7c08 7c05 6404 9c04 7d03 71a4  |.|.|.|.d...}.q.
-00000a70: 7412 7c03 8301 6406 6b02 9001 724c 7402  t.|...d.k...rLt.
-00000a80: 8300 7d04 7c04 6a03 6403 6b02 9001 7232  ..}.|.j.d.k...r2
-00000a90: 7c04 6a04 7d05 6e06 7c04 6a03 7d05 7c04  |.j.}.n.|.j.}.|.
-00000aa0: 6a05 7c04 6a06 7c04 6a04 7c05 6404 9c04  j.|.j.|.j.|.d...
-00000ab0: 7d03 7c03 5300 2907 4eda 0554 4845 4d45  }.|.S.).N..THEME
-00000ac0: da05 4c49 4748 5472 1600 0000 2904 7a10  ..LIGHTr....).z.
-00000ad0: 6261 636b 6772 6f75 6e64 2d63 6f6c 6f72  background-color
-00000ae0: 7a0a 7465 7874 2d63 6f6c 6f72 7a0c 6163  z.text-colorz.ac
-00000af0: 6365 6e74 2d63 6f6c 6f72 7a0b 6963 6f6e  cent-colorz.icon
-00000b00: 732d 636f 6c6f 72da 0444 4152 4b72 0100  s-color..DARKr..
-00000b10: 0000 2913 da09 5153 6574 7469 6e67 73da  ..)...QSettings.
-00000b20: 0576 616c 7565 723d 0000 0072 1f00 0000  .valuer=...r....
-00000b30: 721e 0000 0072 1c00 0000 721d 0000 0072  r....r....r....r
-00000b40: 3400 0000 da02 7569 da06 7468 656d 6573  4.....ui..themes
-00000b50: da0c 6465 6661 756c 7454 6865 6d65 da04  ..defaultTheme..
-00000b60: 6e61 6d65 da08 7365 7456 616c 7565 da0f  name..setValue..
-00000b70: 6261 636b 6772 6f75 6e64 436f 6c6f 72da  backgroundColor.
-00000b80: 0974 6578 7443 6f6c 6f72 da0b 6163 6365  .textColor..acce
-00000b90: 6e74 436f 6c6f 72da 0e63 7265 6174 654e  ntColor..createN
-00000ba0: 6577 4963 6f6e 73da 0a69 636f 6e73 436f  ewIcons..iconsCo
-00000bb0: 6c6f 72da 036c 656e 2909 722f 0000 00da  lor..len).r/....
-00000bc0: 0873 6574 7469 6e67 7372 4000 0000 5a10  .settingsr@...Z.
-00000bd0: 6375 7272 656e 7454 6865 6d65 496e 666f  currentThemeInfo
-00000be0: da05 7468 656d 6572 4e00 0000 721c 0000  ..themerN...r...
-00000bf0: 0072 1d00 0000 721e 0000 0072 1100 0000  .r....r....r....
-00000c00: 7211 0000 0072 1200 0000 da13 6765 7443  r....r......getC
-00000c10: 7572 7265 6e74 5468 656d 6549 6e66 6f61  urrentThemeInfoa
-00000c20: 0000 0073 4800 0000 0001 0602 0a02 0402  ...sH...........
-00000c30: 0801 0601 0a01 0601 0a02 0602 1602 0801  ................
-00000c40: 0601 0a01 0601 0a02 0602 1603 0c01 1002  ................
-00000c50: 0e01 0601 0601 0602 0601 0a01 0602 0802  ................
-00000c60: 0402 1002 0e01 0601 0c01 0802 0602 1402  ................
-00000c70: 7a27 4372 6561 7465 436f 6c6f 7256 6172  z'CreateColorVar
-00000c80: 6961 626c 652e 6765 7443 7572 7265 6e74  iable.getCurrent
-00000c90: 5468 656d 6549 6e66 6f63 0100 0000 0000  ThemeInfoc......
-00000ca0: 0000 0000 0000 0900 0000 2000 0000 4300  .......... ...C.
-00000cb0: 0000 73e2 0200 0074 0083 007d 017c 01a0  ..s....t...}.|..
-00000cc0: 0164 01a1 017d 0264 027d 037c 0264 036b  .d...}.d.}.|.d.k
-00000cd0: 0272 2674 0283 007d 0490 016e 3a7c 0264  .r&t...}...n:|.d
-00000ce0: 046b 0272 3874 0383 007d 0490 016e 287c  .k.r8t...}...n(|
-00000cf0: 006a 046a 0544 005d 4a7d 057c 056a 0673  .j.j.D.]J}.|.j.s
-00000d00: 547c 056a 077c 026b 0272 407c 01a0 0864  T|.j.|.k.r@|...d
-00000d10: 017c 056a 07a1 0201 007c 057d 047c 056a  .|.j.....|.}.|.j
-00000d20: 097c 045f 0a7c 056a 0b7c 045f 0c7c 056a  .|._.|.j.|._.|.j
-00000d30: 0d7c 045f 0e7c 046a 0f7c 045f 1064 057d  .|._.|.j.|._.d.}
-00000d40: 0371 407c 0373 9674 0283 007d 0474 117c  .q@|.s.t...}.t.|
-00000d50: 046a 0a64 0683 027c 045f 1274 117c 046a  .j.d...|._.t.|.j
-00000d60: 0a64 0783 027c 045f 1374 117c 046a 0a64  .d...|._.t.|.j.d
-00000d70: 0883 027c 045f 1474 117c 046a 0a64 0983  ...|._.t.|.j.d..
-00000d80: 027c 045f 1574 117c 046a 0a64 0a83 027c  .|._.t.|.j.d...|
-00000d90: 045f 1674 117c 046a 0a64 0b83 027c 045f  ._.t.|.j.d...|._
-00000da0: 1774 117c 046a 0c64 0683 027c 045f 1874  .t.|.j.d...|._.t
-00000db0: 117c 046a 0c64 0783 027c 045f 1974 117c  .|.j.d...|._.t.|
-00000dc0: 046a 0c64 0883 027c 045f 1a74 117c 046a  .j.d...|._.t.|.j
-00000dd0: 0c64 0983 027c 045f 1b74 117c 046a 0e64  .d...|._.t.|.j.d
-00000de0: 0683 027c 045f 1c74 117c 046a 0e64 0783  ...|._.t.|.j.d..
-00000df0: 027c 045f 1d74 117c 046a 0e64 0883 027c  .|._.t.|.j.d...|
-00000e00: 045f 1e74 117c 046a 0e64 0983 027c 045f  ._.t.|.j.d...|._
-00000e10: 1f64 0c7c 045f 2074 2183 007c 005f 227c  .d.|._ t!..|._"|
-00000e20: 046a 127c 006a 225f 237c 046a 137c 006a  .j.|.j"_#|.j.|.j
-00000e30: 225f 247c 046a 147c 006a 225f 257c 046a  "_$|.j.|.j"_%|.j
-00000e40: 157c 006a 225f 267c 046a 167c 006a 225f  .|.j"_&|.j.|.j"_
-00000e50: 277c 046a 177c 006a 225f 287c 046a 187c  '|.j.|.j"_(|.j.|
-00000e60: 006a 225f 297c 046a 197c 006a 225f 2a7c  .j"_)|.j.|.j"_*|
-00000e70: 046a 1a7c 006a 225f 2b7c 046a 1b7c 006a  .j.|.j"_+|.j.|.j
-00000e80: 225f 2c7c 046a 1c7c 006a 225f 2d7c 046a  "_,|.j.|.j"_-|.j
-00000e90: 1d7c 006a 225f 2e7c 046a 1e7c 006a 225f  .|.j"_.|.j.|.j"_
-00000ea0: 2f7c 046a 1f7c 006a 225f 307c 046a 207c  /|.j.|.j"_0|.j |
-00000eb0: 006a 225f 3174 326a 33a0 3474 326a 33a0  .j"_1t2j3.4t2j3.
-00000ec0: 3574 32a0 36a1 0064 0da1 02a1 017d 0674  5t2.6..d.....}.t
-00000ed0: 326a 33a0 377c 06a1 0190 0273 3074 32a0  2j3.7|.....s0t2.
-00000ee0: 387c 06a1 0101 0074 326a 33a0 3474 326a  8|.....t2j3.4t2j
-00000ef0: 33a0 357c 0664 0ea1 02a1 017d 0774 397c  3.5|.d.....}.t9|
-00000f00: 0764 0f83 027d 0874 3a64 107c 046a 129b  .d...}.t:d.|.j..
-00000f10: 0064 117c 046a 139b 0064 127c 046a 149b  .d.|.j...d.|.j..
-00000f20: 0064 137c 046a 159b 0064 147c 046a 169b  .d.|.j...d.|.j..
-00000f30: 0064 157c 046a 179b 0064 167c 046a 189b  .d.|.j...d.|.j..
-00000f40: 0064 177c 046a 199b 0064 187c 046a 1a9b  .d.|.j...d.|.j..
-00000f50: 0064 197c 046a 1b9b 0064 1a7c 046a 1c9b  .d.|.j...d.|.j..
-00000f60: 0064 1b7c 046a 1d9b 0064 1c7c 046a 1e9b  .d.|.j...d.|.j..
-00000f70: 0064 1d7c 046a 1f9b 0064 1e7c 046a 209b  .d.|.j...d.|.j .
-00000f80: 0064 1f9d 1f7c 0864 208d 0201 007c 08a0  .d...|.d ....|..
-00000f90: 3ba1 0001 0064 0053 0029 214e 7240 0000  ;....d.S.)!Nr@..
-00000fa0: 0046 7241 0000 0072 4200 0000 5472 0400  .FrA...rB...Tr..
-00000fb0: 0000 7219 0000 0072 1700 0000 721a 0000  ..r....r....r...
-00000fc0: 0072 1800 0000 7203 0000 0072 1b00 0000  .r....r....r....
-00000fd0: da03 5153 537a 0f5f 7661 7269 6162 6c65  ..QSSz._variable
-00000fe0: 732e 7363 7373 da01 777a e00a 2020 2020  s.scss..wz..    
-00000ff0: 2020 2020 2f2f 3d3d 3d3d 3d3d 3d3d 3d3d      //==========
+00000120: 6a04 7400 a005 7c02 a101 8e00 7d02 7c02  j.t...|.....}.|.
+00000130: 6401 1900 7d03 7c02 6402 1900 7c01 1400  d...}.|.d...|...
+00000140: 7c01 1400 7c01 1400 7d04 7c02 6403 1900  |...|...}.|.d...
+00000150: 7d05 7403 a006 7c03 7c04 7c05 a103 7d06  }.t...|.|.|...}.
+00000160: 7407 7408 7c06 6401 1900 6404 1400 8301  t.t.|.d...d.....
+00000170: 7408 7c06 6402 1900 6404 1400 8301 7408  t.|.d...d.....t.
+00000180: 7c06 6403 1900 6404 1400 8301 6603 8301  |.d...d.....f...
+00000190: 7d07 7c07 5300 2905 4e72 0100 0000 e901  }.|.S.).Nr......
+000001a0: 0000 00e9 0200 0000 e9fa 0000 0029 09da  .............)..
+000001b0: 026d 635a 0663 6e61 6d65 73da 084b 6579  .mcZ.cnames..Key
+000001c0: 4572 726f 72da 0863 6f6c 6f72 7379 735a  Error..colorsysZ
+000001d0: 0a72 6762 5f74 6f5f 686c 735a 0674 6f5f  .rgb_to_hlsZ.to_
+000001e0: 7267 625a 0a68 6c73 5f74 6f5f 7267 62da  rgbZ.hls_to_rgb.
+000001f0: 0a72 6762 5f74 6f5f 6865 78da 0369 6e74  .rgb_to_hex..int
+00000200: 2908 da05 636f 6c6f 72da 0661 6d6f 756e  )...color..amoun
+00000210: 74da 0163 5a0c 6164 6a75 7374 6564 5f68  t..cZ.adjusted_h
+00000220: 7565 5a12 6164 6a75 7374 6564 5f6c 6967  ueZ.adjusted_lig
+00000230: 6874 6e65 7373 5a13 6164 6a75 7374 6564  htnessZ.adjusted
+00000240: 5f73 6174 7572 6174 696f 6eda 0372 6762  _saturation..rgb
+00000250: 5a09 6e65 775f 636f 6c6f 72a9 0072 1000  Z.new_color..r..
+00000260: 0000 fa46 653a 5c53 7069 6e6e 2054 6173  ...Fe:\Spinn Tas
+00000270: 6b5c 3070 6173 735c 3070 6173 732d 6170  k\0pass\0pass-ap
+00000280: 702d 6d61 7374 6572 5c43 7573 746f 6d5f  p-master\Custom_
+00000290: 5769 6467 6574 735c 5173 735c 636f 6c6f  Widgets\Qss\colo
+000002a0: 7273 7973 7465 6d2e 7079 da10 6164 6a75  rsystem.py..adju
+000002b0: 7374 5f6c 6967 6874 6e65 7373 1e00 0000  st_lightness....
+000002c0: 7316 0000 0000 0102 010e 010e 010a 0110  s...............
+000002d0: 0a08 0114 0108 020e 0132 0272 1200 0000  .........2.r....
+000002e0: 6301 0000 0000 0000 0000 0000 0002 0000  c...............
+000002f0: 0002 0000 0043 0000 0073 1000 0000 6401  .....C...s....d.
+00000300: 7c00 1600 7d01 6402 7c01 1700 5300 2903  |...}.d.|...S.).
+00000310: 4e7a 0c25 3032 7825 3032 7825 3032 78fa  Nz.%02x%02x%02x.
+00000320: 0123 7210 0000 0029 0272 0f00 0000 5a09  .#r....).r....Z.
+00000330: 6865 785f 636f 6c6f 7272 1000 0000 7210  hex_colorr....r.
+00000340: 0000 0072 1100 0000 720a 0000 0037 0000  ...r....r....7..
+00000350: 0073 0400 0000 0001 0801 720a 0000 0063  .s........r....c
+00000360: 0000 0000 0000 0000 0000 0000 0000 0000  ................
+00000370: 0300 0000 4000 0000 7316 0000 0065 005a  ....@...s....e.Z
+00000380: 0164 005a 0264 0564 0264 0384 015a 0364  .d.Z.d.d.d...Z.d
+00000390: 0453 0029 06da 0554 6865 6d65 da00 6305  .S.)...Theme..c.
+000003a0: 0000 0000 0000 0000 0000 0005 0000 0003  ................
+000003b0: 0000 0043 0000 0073 ca00 0000 7c01 7c00  ...C...s....|.|.
+000003c0: 5f00 7c02 7c00 5f01 7c03 7c00 5f02 7c04  _.|.|._.|.|._.|.
+000003d0: 7c00 5f03 7404 7c01 6401 8302 7c00 5f05  |._.t.|.d...|._.
+000003e0: 7404 7c01 6402 8302 7c00 5f06 7404 7c01  t.|.d...|._.t.|.
+000003f0: 6403 8302 7c00 5f07 7404 7c01 6404 8302  d...|._.t.|.d...
+00000400: 7c00 5f08 7404 7c01 6405 8302 7c00 5f09  |._.t.|.d...|._.
+00000410: 7404 7c01 6406 8302 7c00 5f0a 7404 7c02  t.|.d...|._.t.|.
+00000420: 6401 8302 7c00 5f0b 7404 7c02 6407 8302  d...|._.t.|.d...
+00000430: 7c00 5f0c 7404 7c02 6403 8302 7c00 5f0d  |._.t.|.d...|._.
+00000440: 7404 7c02 6408 8302 7c00 5f0e 7404 7c03  t.|.d...|._.t.|.
+00000450: 6401 8302 7c00 5f0f 7404 7c03 6407 8302  d...|._.t.|.d...
+00000460: 7c00 5f10 7404 7c03 6403 8302 7c00 5f11  |._.t.|.d...|._.
+00000470: 7404 7c03 6408 8302 7c00 5f12 6409 7c00  t.|.d...|._.d.|.
+00000480: 5f13 6400 5300 290a 4e72 0400 0000 6766  _.d.S.).Nr....gf
+00000490: 6666 6666 66ee 3fe7 9a99 9999 9999 e93f  fffff.?........?
+000004a0: 6700 0000 0000 00e8 3fe7 3333 3333 3333  g.......?.333333
+000004b0: e33f 679a 9999 9999 99e1 3fe7 cdcc cccc  .?g.......?.....
+000004c0: cccc ec3f e766 6666 6666 66e6 3ffa 0e3a  ...?.ffffff.?..:
+000004d0: 2f69 636f 6e73 2f49 636f 6e73 2f29 14da  /icons/Icons/)..
+000004e0: 0862 675f 636f 6c6f 72da 0974 7874 5f63  .bg_color..txt_c
+000004f0: 6f6c 6f72 da0c 6163 6365 6e74 5f63 6f6c  olor..accent_col
+00000500: 6f72 da0b 6963 6f6e 735f 636f 6c6f 7272  or..icons_colorr
+00000510: 1200 0000 da04 4247 5f31 da04 4247 5f32  ......BG_1..BG_2
+00000520: da04 4247 5f33 da04 4247 5f34 da04 4247  ..BG_3..BG_4..BG
+00000530: 5f35 da04 4247 5f36 da04 4354 5f31 da04  _5..BG_6..CT_1..
+00000540: 4354 5f32 da04 4354 5f33 da04 4354 5f34  CT_2..CT_3..CT_4
+00000550: da04 4341 5f31 da04 4341 5f32 da04 4341  ..CA_1..CA_2..CA
+00000560: 5f33 da04 4341 5f34 da05 4943 4f4e 5329  _3..CA_4..ICONS)
+00000570: 05da 0473 656c 6672 1b00 0000 721c 0000  ...selfr....r...
+00000580: 0072 1d00 0000 721e 0000 0072 1000 0000  .r....r....r....
+00000590: 7210 0000 0072 1100 0000 da08 5f5f 696e  r....r......__in
+000005a0: 6974 5f5f 3c00 0000 7326 0000 0000 0106  it__<...s&......
+000005b0: 0106 0106 0106 020c 010c 010c 010c 010c  ................
+000005c0: 010c 020c 010c 010c 010c 020c 010c 010c  ................
+000005d0: 010c 027a 0e54 6865 6d65 2e5f 5f69 6e69  ...z.Theme.__ini
+000005e0: 745f 5f4e 2901 7215 0000 0029 04da 085f  t__N).r....)..._
+000005f0: 5f6e 616d 655f 5fda 0a5f 5f6d 6f64 756c  _name__..__modul
+00000600: 655f 5fda 0c5f 5f71 7561 6c6e 616d 655f  e__..__qualname_
+00000610: 5f72 2f00 0000 7210 0000 0072 1000 0000  _r/...r....r....
+00000620: 7210 0000 0072 1100 0000 7214 0000 003b  r....r....r....;
+00000630: 0000 0073 0200 0000 0801 7214 0000 0063  ...s......r....c
+00000640: 0000 0000 0000 0000 0000 0000 0000 0000  ................
+00000650: 0300 0000 0000 0000 731c 0000 0065 005a  ........s....e.Z
+00000660: 0164 005a 0287 0066 0164 0164 0284 085a  .d.Z...f.d.d...Z
+00000670: 0387 0004 005a 0453 0029 03da 0444 6172  .....Z.S.)...Dar
+00000680: 6b63 0100 0000 0000 0000 0000 0000 0100  kc..............
+00000690: 0000 0500 0000 0300 0000 7314 0000 0074  ..........s....t
+000006a0: 0083 00a0 0164 0164 0264 03a1 0301 0064  .....d.d.d.....d
+000006b0: 0053 0029 044e 7a07 2330 4430 4431 34fa  .S.).Nz.#0D0D14.
+000006c0: 0423 6666 667a 0723 4138 4239 4244 a902  .#fffz.#A8B9BD..
+000006d0: da05 7375 7065 7272 2f00 0000 a901 722e  ..superr/.....r.
+000006e0: 0000 00a9 01da 095f 5f63 6c61 7373 5f5f  .......__class__
+000006f0: 7210 0000 0072 1100 0000 722f 0000 0056  r....r....r/...V
+00000700: 0000 0073 0200 0000 0001 7a0d 4461 726b  ...s......z.Dark
+00000710: 2e5f 5f69 6e69 745f 5fa9 0572 3000 0000  .__init__..r0...
+00000720: 7231 0000 0072 3200 0000 722f 0000 00da  r1...r2...r/....
+00000730: 0d5f 5f63 6c61 7373 6365 6c6c 5f5f 7210  .__classcell__r.
+00000740: 0000 0072 1000 0000 7238 0000 0072 1100  ...r....r8...r..
+00000750: 0000 7233 0000 0055 0000 0073 0200 0000  ..r3...U...s....
+00000760: 0801 7233 0000 0063 0000 0000 0000 0000  ..r3...c........
+00000770: 0000 0000 0000 0000 0300 0000 0000 0000  ................
+00000780: 731c 0000 0065 005a 0164 005a 0287 0066  s....e.Z.d.Z...f
+00000790: 0164 0164 0284 085a 0387 0004 005a 0453  .d.d...Z.....Z.S
+000007a0: 0029 03da 054c 6967 6874 6301 0000 0000  .)...Lightc.....
+000007b0: 0000 0000 0000 0001 0000 0005 0000 0003  ................
+000007c0: 0000 0073 1400 0000 7400 8300 a001 6401  ...s....t.....d.
+000007d0: 6402 6403 a103 0100 6400 5300 2904 4e72  d.d.....d.S.).Nr
+000007e0: 3400 0000 7a04 2330 3030 7a07 2330 3062  4...z.#000z.#00b
+000007f0: 6366 6672 3500 0000 7237 0000 0072 3800  cffr5...r7...r8.
+00000800: 0000 7210 0000 0072 1100 0000 722f 0000  ..r....r....r/..
+00000810: 005a 0000 0073 0200 0000 0001 7a0e 4c69  .Z...s......z.Li
+00000820: 6768 742e 5f5f 696e 6974 5f5f 723a 0000  ght.__init__r:..
+00000830: 0072 1000 0000 7210 0000 0072 3800 0000  .r....r....r8...
+00000840: 7211 0000 0072 3c00 0000 5900 0000 7302  r....r<...Y...s.
+00000850: 0000 0008 0172 3c00 0000 6300 0000 0000  .....r<...c.....
+00000860: 0000 0000 0000 0000 0000 0004 0000 0000  ................
+00000870: 0000 0073 2e00 0000 6500 5a01 6400 5a02  ...s....e.Z.d.Z.
+00000880: 6408 8700 6601 6402 6403 8409 5a03 6404  d...f.d.d...Z.d.
+00000890: 6405 8400 5a04 6406 6407 8400 5a05 8700  d...Z.d.d...Z...
+000008a0: 0400 5a06 5300 2909 da13 4372 6561 7465  ..Z.S.)...Create
+000008b0: 436f 6c6f 7256 6172 6961 626c 654e 6302  ColorVariableNc.
+000008c0: 0000 0000 0000 0000 0000 0002 0000 0003  ................
+000008d0: 0000 0003 0000 0073 1400 0000 7400 7401  .......s....t.t.
+000008e0: 7c00 8302 a002 7c01 a101 0100 6400 5300  |.....|.....d.S.
+000008f0: 2901 4e29 0372 3600 0000 723d 0000 0072  ).N).r6...r=...r
+00000900: 2f00 0000 2902 722e 0000 00da 0670 6172  /...).r......par
+00000910: 656e 7472 3800 0000 7210 0000 0072 1100  entr8...r....r..
+00000920: 0000 722f 0000 0066 0000 0073 0200 0000  ..r/...f...s....
+00000930: 0001 7a1c 4372 6561 7465 436f 6c6f 7256  ..z.CreateColorV
+00000940: 6172 6961 626c 652e 5f5f 696e 6974 5f5f  ariable.__init__
+00000950: 6301 0000 0000 0000 0000 0000 0009 0000  c...............
+00000960: 0006 0000 0043 0000 0073 5001 0000 7400  .....C...sP...t.
+00000970: 8300 7d01 7c01 a001 6401 a101 7d02 6900  ..}.|...d...}.i.
+00000980: 7d03 7c02 6402 6b02 7258 7402 8300 7d04  }.|.d.k.rXt...}.
+00000990: 7c04 6a03 6403 6b02 723c 7c04 6a04 7d05  |.j.d.k.r<|.j.}.
+000009a0: 7c04 6a04 7c04 5f03 6e06 7c04 6a03 7d05  |.j.|._.n.|.j.}.
+000009b0: 7c04 6a05 7c04 6a06 7c04 6a04 7c05 6404  |.j.|.j.|.j.|.d.
+000009c0: 9c04 7d03 6eb2 7c02 6405 6b02 729c 7407  ..}.n.|.d.k.r.t.
+000009d0: 8300 7d04 7c04 6a03 6403 6b02 7280 7c04  ..}.|.j.d.k.r.|.
+000009e0: 6a04 7d05 7c04 6a04 7c04 5f03 6e06 7c04  j.}.|.j.|._.n.|.
+000009f0: 6a03 7d05 7c04 6a05 7c04 6a06 7c04 6a04  j.}.|.j.|.j.|.j.
+00000a00: 7c05 6404 9c04 7d03 6e6e 7c00 6a08 6a09  |.d...}.nn|.j.j.
+00000a10: 4400 5d64 7d04 7c04 6a0a 73b8 7c04 6a0b  D.]d}.|.j.s.|.j.
+00000a20: 7c02 6b02 72a4 7c01 a00c 6401 7c04 6a0b  |.k.r.|...d.|.j.
+00000a30: a102 0100 7c04 6a0d 7d06 7c04 6a0e 7d07  ....|.j.}.|.j.}.
+00000a40: 7c04 6a0f 7d08 7c04 6a10 72f6 7c04 6a11  |.j.}.|.j.r.|.j.
+00000a50: 6403 6b02 72ee 7c08 7d05 71fa 7c04 6a11  d.k.r.|.}.q.|.j.
+00000a60: 7d05 6e04 6400 7d05 7c06 7c07 7c08 7c05  }.n.d.}.|.|.|.|.
+00000a70: 6404 9c04 7d03 71a4 7412 7c03 8301 6406  d...}.q.t.|...d.
+00000a80: 6b02 9001 724c 7402 8300 7d04 7c04 6a03  k...rLt...}.|.j.
+00000a90: 6403 6b02 9001 7232 7c04 6a04 7d05 6e06  d.k...r2|.j.}.n.
+00000aa0: 7c04 6a03 7d05 7c04 6a05 7c04 6a06 7c04  |.j.}.|.j.|.j.|.
+00000ab0: 6a04 7c05 6404 9c04 7d03 7c03 5300 2907  j.|.d...}.|.S.).
+00000ac0: 4eda 0554 4845 4d45 da05 4c49 4748 5472  N..THEME..LIGHTr
+00000ad0: 1500 0000 2904 7a10 6261 636b 6772 6f75  ....).z.backgrou
+00000ae0: 6e64 2d63 6f6c 6f72 7a0a 7465 7874 2d63  nd-colorz.text-c
+00000af0: 6f6c 6f72 7a0c 6163 6365 6e74 2d63 6f6c  olorz.accent-col
+00000b00: 6f72 7a0b 6963 6f6e 732d 636f 6c6f 72da  orz.icons-color.
+00000b10: 0444 4152 4b72 0100 0000 2913 da09 5153  .DARKr....)...QS
+00000b20: 6574 7469 6e67 73da 0576 616c 7565 723c  ettings..valuer<
+00000b30: 0000 0072 1e00 0000 721d 0000 0072 1b00  ...r....r....r..
+00000b40: 0000 721c 0000 0072 3300 0000 da02 7569  ..r....r3.....ui
+00000b50: da06 7468 656d 6573 da0c 6465 6661 756c  ..themes..defaul
+00000b60: 7454 6865 6d65 da04 6e61 6d65 da08 7365  tTheme..name..se
+00000b70: 7456 616c 7565 da0f 6261 636b 6772 6f75  tValue..backgrou
+00000b80: 6e64 436f 6c6f 72da 0974 6578 7443 6f6c  ndColor..textCol
+00000b90: 6f72 da0b 6163 6365 6e74 436f 6c6f 72da  or..accentColor.
+00000ba0: 0e63 7265 6174 654e 6577 4963 6f6e 73da  .createNewIcons.
+00000bb0: 0a69 636f 6e73 436f 6c6f 72da 036c 656e  .iconsColor..len
+00000bc0: 2909 722e 0000 00da 0873 6574 7469 6e67  ).r......setting
+00000bd0: 7372 3f00 0000 5a10 6375 7272 656e 7454  sr?...Z.currentT
+00000be0: 6865 6d65 496e 666f da05 7468 656d 6572  hemeInfo..themer
+00000bf0: 4d00 0000 721b 0000 0072 1c00 0000 721d  M...r....r....r.
+00000c00: 0000 0072 1000 0000 7210 0000 0072 1100  ...r....r....r..
+00000c10: 0000 da13 6765 7443 7572 7265 6e74 5468  ....getCurrentTh
+00000c20: 656d 6549 6e66 6f69 0000 0073 4800 0000  emeInfoi...sH...
+00000c30: 0001 0602 0a02 0402 0801 0601 0a01 0601  ................
+00000c40: 0a02 0602 1602 0801 0601 0a01 0601 0a02  ................
+00000c50: 0602 1603 0c01 1002 0e01 0601 0601 0602  ................
+00000c60: 0601 0a01 0602 0802 0402 1002 0e01 0601  ................
+00000c70: 0c01 0802 0602 1402 7a27 4372 6561 7465  ........z'Create
+00000c80: 436f 6c6f 7256 6172 6961 626c 652e 6765  ColorVariable.ge
+00000c90: 7443 7572 7265 6e74 5468 656d 6549 6e66  tCurrentThemeInf
+00000ca0: 6f63 0100 0000 0000 0000 0000 0000 0900  oc..............
+00000cb0: 0000 2000 0000 4300 0000 73e2 0200 0074  .. ...C...s....t
+00000cc0: 0083 007d 017c 01a0 0164 01a1 017d 0264  ...}.|...d...}.d
+00000cd0: 027d 037c 0264 036b 0272 2674 0283 007d  .}.|.d.k.r&t...}
+00000ce0: 0490 016e 3a7c 0264 046b 0272 3874 0383  ...n:|.d.k.r8t..
+00000cf0: 007d 0490 016e 287c 006a 046a 0544 005d  .}...n(|.j.j.D.]
+00000d00: 4a7d 057c 056a 0673 547c 056a 077c 026b  J}.|.j.sT|.j.|.k
+00000d10: 0272 407c 01a0 0864 017c 056a 07a1 0201  .r@|...d.|.j....
+00000d20: 007c 057d 047c 056a 097c 045f 0a7c 056a  .|.}.|.j.|._.|.j
+00000d30: 0b7c 045f 0c7c 056a 0d7c 045f 0e7c 046a  .|._.|.j.|._.|.j
+00000d40: 0f7c 045f 1064 057d 0371 407c 0373 9674  .|._.d.}.q@|.s.t
+00000d50: 0283 007d 0474 117c 046a 0a64 0683 027c  ...}.t.|.j.d...|
+00000d60: 045f 1274 117c 046a 0a64 0783 027c 045f  ._.t.|.j.d...|._
+00000d70: 1374 117c 046a 0a64 0883 027c 045f 1474  .t.|.j.d...|._.t
+00000d80: 117c 046a 0a64 0983 027c 045f 1574 117c  .|.j.d...|._.t.|
+00000d90: 046a 0a64 0a83 027c 045f 1674 117c 046a  .j.d...|._.t.|.j
+00000da0: 0a64 0b83 027c 045f 1774 117c 046a 0c64  .d...|._.t.|.j.d
+00000db0: 0683 027c 045f 1874 117c 046a 0c64 0783  ...|._.t.|.j.d..
+00000dc0: 027c 045f 1974 117c 046a 0c64 0883 027c  .|._.t.|.j.d...|
+00000dd0: 045f 1a74 117c 046a 0c64 0983 027c 045f  ._.t.|.j.d...|._
+00000de0: 1b74 117c 046a 0e64 0683 027c 045f 1c74  .t.|.j.d...|._.t
+00000df0: 117c 046a 0e64 0783 027c 045f 1d74 117c  .|.j.d...|._.t.|
+00000e00: 046a 0e64 0883 027c 045f 1e74 117c 046a  .j.d...|._.t.|.j
+00000e10: 0e64 0983 027c 045f 1f64 0c7c 045f 2074  .d...|._.d.|._ t
+00000e20: 2183 007c 005f 227c 046a 127c 006a 225f  !..|._"|.j.|.j"_
+00000e30: 237c 046a 137c 006a 225f 247c 046a 147c  #|.j.|.j"_$|.j.|
+00000e40: 006a 225f 257c 046a 157c 006a 225f 267c  .j"_%|.j.|.j"_&|
+00000e50: 046a 167c 006a 225f 277c 046a 177c 006a  .j.|.j"_'|.j.|.j
+00000e60: 225f 287c 046a 187c 006a 225f 297c 046a  "_(|.j.|.j"_)|.j
+00000e70: 197c 006a 225f 2a7c 046a 1a7c 006a 225f  .|.j"_*|.j.|.j"_
+00000e80: 2b7c 046a 1b7c 006a 225f 2c7c 046a 1c7c  +|.j.|.j"_,|.j.|
+00000e90: 006a 225f 2d7c 046a 1d7c 006a 225f 2e7c  .j"_-|.j.|.j"_.|
+00000ea0: 046a 1e7c 006a 225f 2f7c 046a 1f7c 006a  .j.|.j"_/|.j.|.j
+00000eb0: 225f 307c 046a 207c 006a 225f 3174 326a  "_0|.j |.j"_1t2j
+00000ec0: 33a0 3474 326a 33a0 3574 32a0 36a1 0064  3.4t2j3.5t2.6..d
+00000ed0: 0da1 02a1 017d 0674 326a 33a0 377c 06a1  .....}.t2j3.7|..
+00000ee0: 0190 0273 3074 32a0 387c 06a1 0101 0074  ...s0t2.8|.....t
+00000ef0: 326a 33a0 3474 326a 33a0 357c 0664 0ea1  2j3.4t2j3.5|.d..
+00000f00: 02a1 017d 0774 397c 0764 0f83 027d 0874  ...}.t9|.d...}.t
+00000f10: 3a64 107c 046a 129b 0064 117c 046a 139b  :d.|.j...d.|.j..
+00000f20: 0064 127c 046a 149b 0064 137c 046a 159b  .d.|.j...d.|.j..
+00000f30: 0064 147c 046a 169b 0064 157c 046a 179b  .d.|.j...d.|.j..
+00000f40: 0064 167c 046a 189b 0064 177c 046a 199b  .d.|.j...d.|.j..
+00000f50: 0064 187c 046a 1a9b 0064 197c 046a 1b9b  .d.|.j...d.|.j..
+00000f60: 0064 1a7c 046a 1c9b 0064 1b7c 046a 1d9b  .d.|.j...d.|.j..
+00000f70: 0064 1c7c 046a 1e9b 0064 1d7c 046a 1f9b  .d.|.j...d.|.j..
+00000f80: 0064 1e7c 046a 209b 0064 1f9d 1f7c 0864  .d.|.j ..d...|.d
+00000f90: 208d 0201 007c 08a0 3ba1 0001 0064 0053   ....|..;....d.S
+00000fa0: 0029 214e 723f 0000 0046 7240 0000 0072  .)!Nr?...Fr@...r
+00000fb0: 4100 0000 5472 0400 0000 7218 0000 0072  A...Tr....r....r
+00000fc0: 1600 0000 7219 0000 0072 1700 0000 7203  ....r....r....r.
+00000fd0: 0000 0072 1a00 0000 da03 5153 537a 0f5f  ...r......QSSz._
+00000fe0: 7661 7269 6162 6c65 732e 7363 7373 da01  variables.scss..
+00000ff0: 777a e00a 2020 2020 2020 2020 2f2f 3d3d  wz..        //==
 00001000: 3d3d 3d3d 3d3d 3d3d 3d3d 3d3d 3d3d 3d3d  ================
 00001010: 3d3d 3d3d 3d3d 3d3d 3d3d 3d3d 3d3d 3d3d  ================
-00001020: 3d3d 3d3d 3d3d 3d3d 3d2f 2f0a 2020 2020  =========//.    
-00001030: 2020 2020 2f2f 2046 494c 4520 4155 544f      // FILE AUTO
-00001040: 2d47 454e 4552 4154 4544 2c20 414e 5920  -GENERATED, ANY 
-00001050: 4348 414e 4745 5320 4d41 4445 2057 494c  CHANGES MADE WIL
-00001060: 4c20 4245 204c 4f53 5420 2f2f 0a20 2020  L BE LOST //.   
-00001070: 2020 2020 202f 2f3d 3d3d 3d3d 3d3d 3d3d       //=========
+00001020: 3d3d 3d3d 3d3d 3d3d 3d3d 3d3d 3d3d 3d3d  ================
+00001030: 3d2f 2f0a 2020 2020 2020 2020 2f2f 2046  =//.        // F
+00001040: 494c 4520 4155 544f 2d47 454e 4552 4154  ILE AUTO-GENERAT
+00001050: 4544 2c20 414e 5920 4348 414e 4745 5320  ED, ANY CHANGES 
+00001060: 4d41 4445 2057 494c 4c20 4245 204c 4f53  MADE WILL BE LOS
+00001070: 5420 2f2f 0a20 2020 2020 2020 202f 2f3d  T //.        //=
 00001080: 3d3d 3d3d 3d3d 3d3d 3d3d 3d3d 3d3d 3d3d  ================
 00001090: 3d3d 3d3d 3d3d 3d3d 3d3d 3d3d 3d3d 3d3d  ================
-000010a0: 3d3d 3d3d 3d3d 3d3d 3d3d 3d2f 2f0a 2020  ===========//.  
-000010b0: 2020 2020 2020 2443 4f4c 4f52 5f42 4143        $COLOR_BAC
-000010c0: 4b47 524f 554e 445f 313a 207a 1f3b 0a20  KGROUND_1: z.;. 
-000010d0: 2020 2020 2020 2024 434f 4c4f 525f 4241         $COLOR_BA
-000010e0: 434b 4752 4f55 4e44 5f32 3a20 7a1f 3b0a  CKGROUND_2: z.;.
-000010f0: 2020 2020 2020 2020 2443 4f4c 4f52 5f42          $COLOR_B
-00001100: 4143 4b47 524f 554e 445f 333a 207a 203b  ACKGROUND_3: z ;
-00001110: 200a 2020 2020 2020 2020 2443 4f4c 4f52   .        $COLOR
-00001120: 5f42 4143 4b47 524f 554e 445f 343a 207a  _BACKGROUND_4: z
-00001130: 203b 200a 2020 2020 2020 2020 2443 4f4c   ; .        $COL
-00001140: 4f52 5f42 4143 4b47 524f 554e 445f 353a  OR_BACKGROUND_5:
-00001150: 207a 203b 200a 2020 2020 2020 2020 2443   z ; .        $C
-00001160: 4f4c 4f52 5f42 4143 4b47 524f 554e 445f  OLOR_BACKGROUND_
-00001170: 363a 207a 1a3b 200a 2020 2020 2020 2020  6: z.; .        
-00001180: 2443 4f4c 4f52 5f54 4558 545f 313a 207a  $COLOR_TEXT_1: z
-00001190: 193b 0a20 2020 2020 2020 2024 434f 4c4f  .;.        $COLO
-000011a0: 525f 5445 5854 5f32 3a20 7a19 3b0a 2020  R_TEXT_2: z.;.  
-000011b0: 2020 2020 2020 2443 4f4c 4f52 5f54 4558        $COLOR_TEX
-000011c0: 545f 333a 207a 193b 0a20 2020 2020 2020  T_3: z.;.       
-000011d0: 2024 434f 4c4f 525f 5445 5854 5f34 3a20   $COLOR_TEXT_4: 
-000011e0: 7a1b 3b0a 2020 2020 2020 2020 2443 4f4c  z.;.        $COL
-000011f0: 4f52 5f41 4343 454e 545f 313a 207a 1b3b  OR_ACCENT_1: z.;
-00001200: 0a20 2020 2020 2020 2024 434f 4c4f 525f  .        $COLOR_
-00001210: 4143 4345 4e54 5f32 3a20 7a1b 3b0a 2020  ACCENT_2: z.;.  
-00001220: 2020 2020 2020 2443 4f4c 4f52 5f41 4343        $COLOR_ACC
-00001230: 454e 545f 333a 207a 1b3b 0a20 2020 2020  ENT_3: z.;.     
-00001240: 2020 2024 434f 4c4f 525f 4143 4345 4e54     $COLOR_ACCENT
-00001250: 5f34 3a20 619b 0100 003b 0a20 2020 2020  _4: a....;.     
-00001260: 2020 2024 4f50 4143 4954 595f 544f 4f4c     $OPACITY_TOOL
-00001270: 5449 503a 2032 3330 3b0a 2020 2020 2020  TIP: 230;.      
-00001280: 2020 2453 495a 455f 424f 5244 4552 5f52    $SIZE_BORDER_R
-00001290: 4144 4955 533a 2034 7078 3b0a 2020 2020  ADIUS: 4px;.    
-000012a0: 2020 2020 2442 4f52 4445 525f 313a 2031      $BORDER_1: 1
-000012b0: 7078 2073 6f6c 6964 2024 434f 4c4f 525f  px solid $COLOR_
-000012c0: 4241 434b 4752 4f55 4e44 5f31 3b0a 2020  BACKGROUND_1;.  
-000012d0: 2020 2020 2020 2442 4f52 4445 525f 323a        $BORDER_2:
-000012e0: 2031 7078 2073 6f6c 6964 2024 434f 4c4f   1px solid $COLO
-000012f0: 525f 4241 434b 4752 4f55 4e44 5f34 3b0a  R_BACKGROUND_4;.
-00001300: 2020 2020 2020 2020 2442 4f52 4445 525f          $BORDER_
-00001310: 333a 2031 7078 2073 6f6c 6964 2024 434f  3: 1px solid $CO
-00001320: 4c4f 525f 4241 434b 4752 4f55 4e44 5f36  LOR_BACKGROUND_6
-00001330: 3b0a 2020 2020 2020 2020 2442 4f52 4445  ;.        $BORDE
-00001340: 525f 5345 4c45 4354 494f 4e5f 333a 2031  R_SELECTION_3: 1
-00001350: 7078 2073 6f6c 6964 2024 434f 4c4f 525f  px solid $COLOR_
-00001360: 4143 4345 4e54 5f33 3b0a 2020 2020 2020  ACCENT_3;.      
-00001370: 2020 2442 4f52 4445 525f 5345 4c45 4354    $BORDER_SELECT
-00001380: 494f 4e5f 323a 2031 7078 2073 6f6c 6964  ION_2: 1px solid
-00001390: 2024 434f 4c4f 525f 4143 4345 4e54 5f32   $COLOR_ACCENT_2
-000013a0: 3b0a 2020 2020 2020 2020 2442 4f52 4445  ;.        $BORDE
-000013b0: 525f 5345 4c45 4354 494f 4e5f 313a 2031  R_SELECTION_1: 1
-000013c0: 7078 2073 6f6c 6964 2024 434f 4c4f 525f  px solid $COLOR_
-000013d0: 4143 4345 4e54 5f31 3b0a 2020 2020 2020  ACCENT_1;.      
-000013e0: 2020 2450 4154 485f 5245 534f 5552 4345    $PATH_RESOURCE
-000013f0: 533a 2027 7a9e 273b 0a20 2020 2020 2020  S: 'z.';.       
-00001400: 202f 2f3d 3d3d 3d3d 3d3d 3d3d 3d3d 3d3d   //=============
+000010a0: 3d3d 3d3d 3d3d 3d3d 3d3d 3d3d 3d3d 3d3d  ================
+000010b0: 3d3d 3d2f 2f0a 2020 2020 2020 2020 2443  ===//.        $C
+000010c0: 4f4c 4f52 5f42 4143 4b47 524f 554e 445f  OLOR_BACKGROUND_
+000010d0: 313a 207a 1f3b 0a20 2020 2020 2020 2024  1: z.;.        $
+000010e0: 434f 4c4f 525f 4241 434b 4752 4f55 4e44  COLOR_BACKGROUND
+000010f0: 5f32 3a20 7a1f 3b0a 2020 2020 2020 2020  _2: z.;.        
+00001100: 2443 4f4c 4f52 5f42 4143 4b47 524f 554e  $COLOR_BACKGROUN
+00001110: 445f 333a 207a 203b 200a 2020 2020 2020  D_3: z ; .      
+00001120: 2020 2443 4f4c 4f52 5f42 4143 4b47 524f    $COLOR_BACKGRO
+00001130: 554e 445f 343a 207a 203b 200a 2020 2020  UND_4: z ; .    
+00001140: 2020 2020 2443 4f4c 4f52 5f42 4143 4b47      $COLOR_BACKG
+00001150: 524f 554e 445f 353a 207a 203b 200a 2020  ROUND_5: z ; .  
+00001160: 2020 2020 2020 2443 4f4c 4f52 5f42 4143        $COLOR_BAC
+00001170: 4b47 524f 554e 445f 363a 207a 1a3b 200a  KGROUND_6: z.; .
+00001180: 2020 2020 2020 2020 2443 4f4c 4f52 5f54          $COLOR_T
+00001190: 4558 545f 313a 207a 193b 0a20 2020 2020  EXT_1: z.;.     
+000011a0: 2020 2024 434f 4c4f 525f 5445 5854 5f32     $COLOR_TEXT_2
+000011b0: 3a20 7a19 3b0a 2020 2020 2020 2020 2443  : z.;.        $C
+000011c0: 4f4c 4f52 5f54 4558 545f 333a 207a 193b  OLOR_TEXT_3: z.;
+000011d0: 0a20 2020 2020 2020 2024 434f 4c4f 525f  .        $COLOR_
+000011e0: 5445 5854 5f34 3a20 7a1b 3b0a 2020 2020  TEXT_4: z.;.    
+000011f0: 2020 2020 2443 4f4c 4f52 5f41 4343 454e      $COLOR_ACCEN
+00001200: 545f 313a 207a 1b3b 0a20 2020 2020 2020  T_1: z.;.       
+00001210: 2024 434f 4c4f 525f 4143 4345 4e54 5f32   $COLOR_ACCENT_2
+00001220: 3a20 7a1b 3b0a 2020 2020 2020 2020 2443  : z.;.        $C
+00001230: 4f4c 4f52 5f41 4343 454e 545f 333a 207a  OLOR_ACCENT_3: z
+00001240: 1b3b 0a20 2020 2020 2020 2024 434f 4c4f  .;.        $COLO
+00001250: 525f 4143 4345 4e54 5f34 3a20 619b 0100  R_ACCENT_4: a...
+00001260: 003b 0a20 2020 2020 2020 2024 4f50 4143  .;.        $OPAC
+00001270: 4954 595f 544f 4f4c 5449 503a 2032 3330  ITY_TOOLTIP: 230
+00001280: 3b0a 2020 2020 2020 2020 2453 495a 455f  ;.        $SIZE_
+00001290: 424f 5244 4552 5f52 4144 4955 533a 2034  BORDER_RADIUS: 4
+000012a0: 7078 3b0a 2020 2020 2020 2020 2442 4f52  px;.        $BOR
+000012b0: 4445 525f 313a 2031 7078 2073 6f6c 6964  DER_1: 1px solid
+000012c0: 2024 434f 4c4f 525f 4241 434b 4752 4f55   $COLOR_BACKGROU
+000012d0: 4e44 5f31 3b0a 2020 2020 2020 2020 2442  ND_1;.        $B
+000012e0: 4f52 4445 525f 323a 2031 7078 2073 6f6c  ORDER_2: 1px sol
+000012f0: 6964 2024 434f 4c4f 525f 4241 434b 4752  id $COLOR_BACKGR
+00001300: 4f55 4e44 5f34 3b0a 2020 2020 2020 2020  OUND_4;.        
+00001310: 2442 4f52 4445 525f 333a 2031 7078 2073  $BORDER_3: 1px s
+00001320: 6f6c 6964 2024 434f 4c4f 525f 4241 434b  olid $COLOR_BACK
+00001330: 4752 4f55 4e44 5f36 3b0a 2020 2020 2020  GROUND_6;.      
+00001340: 2020 2442 4f52 4445 525f 5345 4c45 4354    $BORDER_SELECT
+00001350: 494f 4e5f 333a 2031 7078 2073 6f6c 6964  ION_3: 1px solid
+00001360: 2024 434f 4c4f 525f 4143 4345 4e54 5f33   $COLOR_ACCENT_3
+00001370: 3b0a 2020 2020 2020 2020 2442 4f52 4445  ;.        $BORDE
+00001380: 525f 5345 4c45 4354 494f 4e5f 323a 2031  R_SELECTION_2: 1
+00001390: 7078 2073 6f6c 6964 2024 434f 4c4f 525f  px solid $COLOR_
+000013a0: 4143 4345 4e54 5f32 3b0a 2020 2020 2020  ACCENT_2;.      
+000013b0: 2020 2442 4f52 4445 525f 5345 4c45 4354    $BORDER_SELECT
+000013c0: 494f 4e5f 313a 2031 7078 2073 6f6c 6964  ION_1: 1px solid
+000013d0: 2024 434f 4c4f 525f 4143 4345 4e54 5f31   $COLOR_ACCENT_1
+000013e0: 3b0a 2020 2020 2020 2020 2450 4154 485f  ;.        $PATH_
+000013f0: 5245 534f 5552 4345 533a 2027 7a9e 273b  RESOURCES: 'z.';
+00001400: 0a20 2020 2020 2020 202f 2f3d 3d3d 3d3d  .        //=====
 00001410: 3d3d 3d3d 3d3d 3d3d 3d3d 3d3d 3d3d 3d3d  ================
 00001420: 3d3d 3d3d 3d3d 3d3d 3d3d 3d3d 3d3d 3d3d  ================
-00001430: 3d3d 3d3d 3d3d 2f2f 0a20 2020 2020 2020  ======//.       
-00001440: 202f 2f20 454e 4420 2f2f 0a20 2020 2020   // END //.     
-00001450: 2020 202f 2f3d 3d3d 3d3d 3d3d 3d3d 3d3d     //===========
+00001430: 3d3d 3d3d 3d3d 3d3d 3d3d 3d3d 3d3d 2f2f  ==============//
+00001440: 0a20 2020 2020 2020 202f 2f20 454e 4420  .        // END 
+00001450: 2f2f 0a20 2020 2020 2020 202f 2f3d 3d3d  //.        //===
 00001460: 3d3d 3d3d 3d3d 3d3d 3d3d 3d3d 3d3d 3d3d  ================
 00001470: 3d3d 3d3d 3d3d 3d3d 3d3d 3d3d 3d3d 3d3d  ================
-00001480: 3d3d 3d3d 3d3d 3d3d 3d2f 2f0a 2020 2020  =========//.    
-00001490: 2020 2020 2901 da04 6669 6c65 293c 7243      )...file)<rC
-000014a0: 0000 0072 4400 0000 723d 0000 0072 3400  ...rD...r=...r4.
-000014b0: 0000 7245 0000 0072 4600 0000 7247 0000  ..rE...rF...rG..
-000014c0: 0072 4800 0000 7249 0000 0072 4a00 0000  .rH...rI...rJ...
-000014d0: 721c 0000 0072 4b00 0000 721d 0000 0072  r....rK...r....r
-000014e0: 4c00 0000 721e 0000 0072 4e00 0000 721f  L...r....rN...r.
-000014f0: 0000 0072 1300 0000 7220 0000 0072 2100  ...r....r ...r!.
-00001500: 0000 7222 0000 0072 2300 0000 7224 0000  ..r"...r#...r$..
-00001510: 0072 2500 0000 7226 0000 0072 2700 0000  .r%...r&...r'...
-00001520: 7228 0000 0072 2900 0000 722a 0000 0072  r(...r)...r*...r
-00001530: 2b00 0000 722c 0000 0072 2d00 0000 722e  +...r,...r-...r.
-00001540: 0000 00da 064f 626a 6563 7472 5100 0000  .....ObjectrQ...
-00001550: 5a12 434f 4c4f 525f 4241 434b 4752 4f55  Z.COLOR_BACKGROU
-00001560: 4e44 5f31 5a12 434f 4c4f 525f 4241 434b  ND_1Z.COLOR_BACK
-00001570: 4752 4f55 4e44 5f32 5a12 434f 4c4f 525f  GROUND_2Z.COLOR_
-00001580: 4241 434b 4752 4f55 4e44 5f33 5a12 434f  BACKGROUND_3Z.CO
-00001590: 4c4f 525f 4241 434b 4752 4f55 4e44 5f34  LOR_BACKGROUND_4
-000015a0: 5a12 434f 4c4f 525f 4241 434b 4752 4f55  Z.COLOR_BACKGROU
-000015b0: 4e44 5f35 5a12 434f 4c4f 525f 4241 434b  ND_5Z.COLOR_BACK
-000015c0: 4752 4f55 4e44 5f36 5a0c 434f 4c4f 525f  GROUND_6Z.COLOR_
-000015d0: 5445 5854 5f31 5a0c 434f 4c4f 525f 5445  TEXT_1Z.COLOR_TE
-000015e0: 5854 5f32 5a0c 434f 4c4f 525f 5445 5854  XT_2Z.COLOR_TEXT
-000015f0: 5f33 5a0c 434f 4c4f 525f 5445 5854 5f34  _3Z.COLOR_TEXT_4
-00001600: 5a0e 434f 4c4f 525f 4143 4345 4e54 5f31  Z.COLOR_ACCENT_1
-00001610: 5a0e 434f 4c4f 525f 4143 4345 4e54 5f32  Z.COLOR_ACCENT_2
-00001620: 5a0e 434f 4c4f 525f 4143 4345 4e54 5f33  Z.COLOR_ACCENT_3
-00001630: 5a0e 434f 4c4f 525f 4143 4345 4e54 5f34  Z.COLOR_ACCENT_4
-00001640: 5a0e 5041 5448 5f52 4553 4f55 5243 4553  Z.PATH_RESOURCES
-00001650: da02 6f73 da04 7061 7468 da07 6162 7370  ..os..path..absp
-00001660: 6174 68da 046a 6f69 6eda 0667 6574 6377  ath..join..getcw
-00001670: 64da 0665 7869 7374 73da 086d 616b 6564  d..exists..maked
-00001680: 6972 73da 046f 7065 6e72 0a00 0000 da05  irs..openr......
-00001690: 636c 6f73 6529 0972 2f00 0000 7250 0000  close).r/...rP..
-000016a0: 0072 4000 0000 5a0a 7468 656d 6546 6f75  .r@...Z.themeFou
-000016b0: 6e64 7251 0000 0072 4600 0000 5a0b 7363  ndrQ...rF...Z.sc
-000016c0: 7373 5f66 6f6c 6465 72da 0973 6373 735f  ss_folder..scss_
-000016d0: 7061 7468 da01 6672 1100 0000 7211 0000  path..fr....r...
-000016e0: 0072 1200 0000 da0f 4372 6561 7465 5661  .r......CreateVa
-000016f0: 7269 6162 6c65 739a 0000 0073 b000 0000  riables....s....
-00001700: 0001 0602 0a01 0401 0801 0a02 0801 0a03  ................
-00001710: 0c01 1002 0e02 0401 0801 0801 0801 0801  ................
-00001720: 0602 0401 0603 0e01 0e01 0e01 0e01 0e01  ................
-00001730: 0e02 0e01 0e01 0e01 0e02 0e01 0e01 0e01  ................
-00001740: 0e02 0603 0801 0a01 0a01 0a01 0a01 0a01  ................
-00001750: 0a02 0a01 0a01 0a01 0a02 0a01 0a01 0a01  ................
-00001760: 0a02 0a03 1a01 0e01 0a02 1601 0a01 0404  ................
-00001770: 04fc 0405 04fb 0406 04fa 0407 04f9 0408  ................
-00001780: 04f8 0409 04f7 040a 04f6 040b 04f5 040c  ................
-00001790: 04f4 040d 04f3 040e 04f2 040f 04f1 0410  ................
-000017a0: 04f0 0411 04ef 041a 04e6 061e 02e2 0620  ............... 
-000017b0: 7a23 4372 6561 7465 436f 6c6f 7256 6172  z#CreateColorVar
-000017c0: 6961 626c 652e 4372 6561 7465 5661 7269  iable.CreateVari
-000017d0: 6162 6c65 7329 014e 2907 7231 0000 0072  ables).N).r1...r
-000017e0: 3200 0000 7233 0000 0072 3000 0000 7252  2...r3...r0...rR
-000017f0: 0000 0072 6200 0000 723c 0000 0072 1100  ...rb...r<...r..
-00001800: 0000 7211 0000 0072 3900 0000 7212 0000  ..r....r9...r...
-00001810: 0072 3e00 0000 5d00 0000 7306 0000 0008  .r>...]...s.....
-00001820: 010e 0308 3972 3e00 0000 6300 0000 0000  ....9r>...c.....
-00001830: 0000 0000 0000 0000 0000 0001 0000 0040  ...............@
-00001840: 0000 0073 0c00 0000 6500 5a01 6400 5a02  ...s....e.Z.d.Z.
-00001850: 6401 5300 2902 7256 0000 004e 2903 7231  d.S.).rV...N).r1
-00001860: 0000 0072 3200 0000 7233 0000 0072 1100  ...r2...r3...r..
-00001870: 0000 7211 0000 0072 1100 0000 7212 0000  ..r....r....r...
-00001880: 0072 5600 0000 0a01 0000 7302 0000 0008  .rV.......s.....
-00001890: 0172 5600 0000 2901 7203 0000 0029 1172  .rV...).r....).r
-000018a0: 5700 0000 da03 7379 73da 0b71 7470 792e  W.....sys..qtpy.
-000018b0: 5174 436f 7265 5a11 6d61 7470 6c6f 746c  QtCoreZ.matplotl
-000018c0: 6962 2e63 6f6c 6f72 73da 0663 6f6c 6f72  ib.colors..color
-000018d0: 7372 0700 0000 7209 0000 0072 4300 0000  sr....r....rC...
-000018e0: 7250 0000 0072 1300 0000 720b 0000 0072  rP...r....r....r
-000018f0: 1500 0000 7234 0000 0072 3d00 0000 723e  ....r4...r=...r>
-00001900: 0000 00da 066f 626a 6563 7472 5600 0000  .....objectrV...
-00001910: 7211 0000 0072 1100 0000 7211 0000 0072  r....r....r....r
-00001920: 1200 0000 da08 3c6d 6f64 756c 653e 0800  ......<module>..
-00001930: 0000 731a 0000 0008 0108 0d08 030c 0108  ..s.............
-00001940: 0206 020a 1108 040e 1a10 0410 0c0e 7f00  ................
-00001950: 2e                                       .
+00001480: 3d3d 3d3d 3d3d 3d3d 3d3d 3d3d 3d3d 3d3d  ================
+00001490: 3d2f 2f0a 2020 2020 2020 2020 2901 da04  =//.        )...
+000014a0: 6669 6c65 293c 7242 0000 0072 4300 0000  file)<rB...rC...
+000014b0: 723c 0000 0072 3300 0000 7244 0000 0072  r<...r3...rD...r
+000014c0: 4500 0000 7246 0000 0072 4700 0000 7248  E...rF...rG...rH
+000014d0: 0000 0072 4900 0000 721b 0000 0072 4a00  ...rI...r....rJ.
+000014e0: 0000 721c 0000 0072 4b00 0000 721d 0000  ..r....rK...r...
+000014f0: 0072 4d00 0000 721e 0000 0072 1200 0000  .rM...r....r....
+00001500: 721f 0000 0072 2000 0000 7221 0000 0072  r....r ...r!...r
+00001510: 2200 0000 7223 0000 0072 2400 0000 7225  "...r#...r$...r%
+00001520: 0000 0072 2600 0000 7227 0000 0072 2800  ...r&...r'...r(.
+00001530: 0000 7229 0000 0072 2a00 0000 722b 0000  ..r)...r*...r+..
+00001540: 0072 2c00 0000 722d 0000 00da 064f 626a  .r,...r-.....Obj
+00001550: 6563 7472 5000 0000 da12 434f 4c4f 525f  ectrP.....COLOR_
+00001560: 4241 434b 4752 4f55 4e44 5f31 5a12 434f  BACKGROUND_1Z.CO
+00001570: 4c4f 525f 4241 434b 4752 4f55 4e44 5f32  LOR_BACKGROUND_2
+00001580: da12 434f 4c4f 525f 4241 434b 4752 4f55  ..COLOR_BACKGROU
+00001590: 4e44 5f33 5a12 434f 4c4f 525f 4241 434b  ND_3Z.COLOR_BACK
+000015a0: 4752 4f55 4e44 5f34 5a12 434f 4c4f 525f  GROUND_4Z.COLOR_
+000015b0: 4241 434b 4752 4f55 4e44 5f35 da12 434f  BACKGROUND_5..CO
+000015c0: 4c4f 525f 4241 434b 4752 4f55 4e44 5f36  LOR_BACKGROUND_6
+000015d0: da0c 434f 4c4f 525f 5445 5854 5f31 5a0c  ..COLOR_TEXT_1Z.
+000015e0: 434f 4c4f 525f 5445 5854 5f32 5a0c 434f  COLOR_TEXT_2Z.CO
+000015f0: 4c4f 525f 5445 5854 5f33 5a0c 434f 4c4f  LOR_TEXT_3Z.COLO
+00001600: 525f 5445 5854 5f34 da0e 434f 4c4f 525f  R_TEXT_4..COLOR_
+00001610: 4143 4345 4e54 5f31 5a0e 434f 4c4f 525f  ACCENT_1Z.COLOR_
+00001620: 4143 4345 4e54 5f32 5a0e 434f 4c4f 525f  ACCENT_2Z.COLOR_
+00001630: 4143 4345 4e54 5f33 5a0e 434f 4c4f 525f  ACCENT_3Z.COLOR_
+00001640: 4143 4345 4e54 5f34 5a0e 5041 5448 5f52  ACCENT_4Z.PATH_R
+00001650: 4553 4f55 5243 4553 da02 6f73 da04 7061  ESOURCES..os..pa
+00001660: 7468 da07 6162 7370 6174 68da 046a 6f69  th..abspath..joi
+00001670: 6eda 0667 6574 6377 64da 0665 7869 7374  n..getcwd..exist
+00001680: 73da 086d 616b 6564 6972 73da 046f 7065  s..makedirs..ope
+00001690: 6eda 0570 7269 6e74 da05 636c 6f73 6529  n..print..close)
+000016a0: 0972 2e00 0000 724f 0000 0072 3f00 0000  .r....rO...r?...
+000016b0: 5a0a 7468 656d 6546 6f75 6e64 7250 0000  Z.themeFoundrP..
+000016c0: 0072 4500 0000 5a0b 7363 7373 5f66 6f6c  .rE...Z.scss_fol
+000016d0: 6465 72da 0973 6373 735f 7061 7468 da01  der..scss_path..
+000016e0: 6672 1000 0000 7210 0000 0072 1100 0000  fr....r....r....
+000016f0: da0f 4372 6561 7465 5661 7269 6162 6c65  ..CreateVariable
+00001700: 73a2 0000 0073 b000 0000 0001 0602 0a01  s....s..........
+00001710: 0401 0801 0a02 0801 0a03 0c01 1002 0e02  ................
+00001720: 0401 0801 0801 0801 0801 0602 0401 0603  ................
+00001730: 0e01 0e01 0e01 0e01 0e01 0e02 0e01 0e01  ................
+00001740: 0e01 0e02 0e01 0e01 0e01 0e02 0603 0801  ................
+00001750: 0a01 0a01 0a01 0a01 0a01 0a02 0a01 0a01  ................
+00001760: 0a01 0a02 0a01 0a01 0a01 0a02 0a03 1a01  ................
+00001770: 0e01 0a02 1601 0a01 0404 04fc 0405 04fb  ................
+00001780: 0406 04fa 0407 04f9 0408 04f8 0409 04f7  ................
+00001790: 040a 04f6 040b 04f5 040c 04f4 040d 04f3  ................
+000017a0: 040e 04f2 040f 04f1 0410 04f0 0411 04ef  ................
+000017b0: 041a 04e6 061e 02e2 0620 7a23 4372 6561  ......... z#Crea
+000017c0: 7465 436f 6c6f 7256 6172 6961 626c 652e  teColorVariable.
+000017d0: 4372 6561 7465 5661 7269 6162 6c65 7329  CreateVariables)
+000017e0: 014e 2907 7230 0000 0072 3100 0000 7232  .N).r0...r1...r2
+000017f0: 0000 0072 2f00 0000 7251 0000 0072 6700  ...r/...rQ...rg.
+00001800: 0000 723b 0000 0072 1000 0000 7210 0000  ..r;...r....r...
+00001810: 0072 3800 0000 7211 0000 0072 3d00 0000  .r8...r....r=...
+00001820: 6500 0000 7306 0000 0008 010e 0308 3972  e...s.........9r
+00001830: 3d00 0000 6300 0000 0000 0000 0000 0000  =...c...........
+00001840: 0000 0000 0001 0000 0040 0000 0073 0c00  .........@...s..
+00001850: 0000 6500 5a01 6400 5a02 6401 5300 2902  ..e.Z.d.Z.d.S.).
+00001860: 7255 0000 004e 2903 7230 0000 0072 3100  rU...N).r0...r1.
+00001870: 0000 7232 0000 0072 1000 0000 7210 0000  ..r2...r....r...
+00001880: 0072 1000 0000 7211 0000 0072 5500 0000  .r....r....rU...
+00001890: 1201 0000 7302 0000 0008 0172 5500 0000  ....s......rU...
+000018a0: 2901 7203 0000 0029 1172 5b00 0000 da03  ).r....).r[.....
+000018b0: 7379 73da 0b71 7470 792e 5174 436f 7265  sys..qtpy.QtCore
+000018c0: 5a11 6d61 7470 6c6f 746c 6962 2e63 6f6c  Z.matplotlib.col
+000018d0: 6f72 73da 0663 6f6c 6f72 7372 0700 0000  ors..colorsr....
+000018e0: 7209 0000 0072 4200 0000 724f 0000 0072  r....rB...rO...r
+000018f0: 1200 0000 720a 0000 0072 1400 0000 7233  ....r....r....r3
+00001900: 0000 0072 3c00 0000 723d 0000 00da 066f  ...r<...r=.....o
+00001910: 626a 6563 7472 5500 0000 7210 0000 0072  bjectrU...r....r
+00001920: 1000 0000 7210 0000 0072 1100 0000 da08  ....r....r......
+00001930: 3c6d 6f64 756c 653e 0800 0000 731a 0000  <module>....s...
+00001940: 0008 0108 0d08 030c 0108 0206 020a 1908  ................
+00001950: 040e 1a10 0410 0c0e 7f00 2e              ...........
```

### Comparing `QT-PyQt-PySide-Custom-Widgets-0.6.5/Custom_Widgets/Qss/__pycache__/colorsystem.cpython-39.pyc` & `QT-PyQt-PySide-Custom-Widgets-0.6.6/Custom_Widgets/Qss/__pycache__/colorsystem.cpython-39.pyc`

 * *Files identical despite different names*

### Comparing `QT-PyQt-PySide-Custom-Widgets-0.6.5/Custom_Widgets/Qss/__pycache__/resources_rc.cpython-39.pyc` & `QT-PyQt-PySide-Custom-Widgets-0.6.6/Custom_Widgets/Qss/__pycache__/resources_rc.cpython-39.pyc`

 * *Files identical despite different names*

### Comparing `QT-PyQt-PySide-Custom-Widgets-0.6.5/Custom_Widgets/Qss/__pycache__/sassCompiler.cpython-39.pyc` & `QT-PyQt-PySide-Custom-Widgets-0.6.6/Custom_Widgets/Qss/__pycache__/sassCompiler.cpython-39.pyc`

 * *Files identical despite different names*

### Comparing `QT-PyQt-PySide-Custom-Widgets-0.6.5/Custom_Widgets/Qss/_styles.scss` & `QT-PyQt-PySide-Custom-Widgets-0.6.6/Custom_Widgets/Qss/_styles.scss`

 * *Files identical despite different names*

### Comparing `QT-PyQt-PySide-Custom-Widgets-0.6.5/Custom_Widgets/Qss/colorsystem.py` & `QT-PyQt-PySide-Custom-Widgets-0.6.6/Custom_Widgets/Qss/colorsystem.py`

 * *Files 12% similar despite different names*

```diff
@@ -29,22 +29,30 @@
 
 def adjust_lightness(color, amount=0.5):
     try:
         c = mc.cnames[color]
     except KeyError:
         c = color
     c = colorsys.rgb_to_hls(*mc.to_rgb(c))
-    print(c)
+    # print(c)
 
-    if c[1] > 0:
-        rgb = colorsys.hls_to_rgb(c[0] , amount * c[1], c[2])
-    else:
-        rgb = colorsys.hls_to_rgb(c[0], 1 - (amount *  (1 - c[1])), c[2])
+    # if c[1] > 0:
+    #     # adjusted_lightness = c[1] * amount
+    #     adjusted_lightness = c[1] * amount * amount 
+    # else:
+    #     adjusted_lightness = 1 - (amount * amount)
+    #     # adjusted_lightness = 1 - c[1] * amount * amount
+
+    adjusted_hue = c[0]
+    adjusted_lightness = c[1] * amount * amount * amount
+    adjusted_saturation = c[2] 
 
+    rgb = colorsys.hls_to_rgb(adjusted_hue, adjusted_lightness, adjusted_saturation)
     new_color = rgb_to_hex((int(rgb[0] * 250), int(rgb[1] * 250), int(rgb[2] * 250)))
+
     return new_color
 
 
 def rgb_to_hex(rgb):
     hex_color = '%02x%02x%02x' % rgb
     return "#" + hex_color
```

### Comparing `QT-PyQt-PySide-Custom-Widgets-0.6.5/Custom_Widgets/Qss/icons/original_svg/aperture.svg` & `QT-PyQt-PySide-Custom-Widgets-0.6.6/Custom_Widgets/Qss/icons/original_svg/aperture.svg`

 * *Files identical despite different names*

### Comparing `QT-PyQt-PySide-Custom-Widgets-0.6.5/Custom_Widgets/Qss/icons/original_svg/arrow_down.svg` & `QT-PyQt-PySide-Custom-Widgets-0.6.6/Custom_Widgets/Qss/icons/original_svg/arrow_down.svg`

 * *Files identical despite different names*

### Comparing `QT-PyQt-PySide-Custom-Widgets-0.6.5/Custom_Widgets/Qss/icons/original_svg/arrow_left.svg` & `QT-PyQt-PySide-Custom-Widgets-0.6.6/Custom_Widgets/Qss/icons/original_svg/arrow_left.svg`

 * *Files identical despite different names*

### Comparing `QT-PyQt-PySide-Custom-Widgets-0.6.5/Custom_Widgets/Qss/icons/original_svg/arrow_right.svg` & `QT-PyQt-PySide-Custom-Widgets-0.6.6/Custom_Widgets/Qss/icons/original_svg/arrow_right.svg`

 * *Files identical despite different names*

### Comparing `QT-PyQt-PySide-Custom-Widgets-0.6.5/Custom_Widgets/Qss/icons/original_svg/arrow_up.svg` & `QT-PyQt-PySide-Custom-Widgets-0.6.6/Custom_Widgets/Qss/icons/original_svg/arrow_up.svg`

 * *Files identical despite different names*

### Comparing `QT-PyQt-PySide-Custom-Widgets-0.6.5/Custom_Widgets/Qss/icons/original_svg/base_icon.svg` & `QT-PyQt-PySide-Custom-Widgets-0.6.6/Custom_Widgets/Qss/icons/original_svg/base_icon.svg`

 * *Files identical despite different names*

### Comparing `QT-PyQt-PySide-Custom-Widgets-0.6.5/Custom_Widgets/Qss/icons/original_svg/base_palette.svg` & `QT-PyQt-PySide-Custom-Widgets-0.6.6/Custom_Widgets/Qss/icons/original_svg/base_palette.svg`

 * *Files identical despite different names*

### Comparing `QT-PyQt-PySide-Custom-Widgets-0.6.5/Custom_Widgets/Qss/icons/original_svg/branch_closed.svg` & `QT-PyQt-PySide-Custom-Widgets-0.6.6/Custom_Widgets/Qss/icons/original_svg/branch_closed.svg`

 * *Files identical despite different names*

### Comparing `QT-PyQt-PySide-Custom-Widgets-0.6.5/Custom_Widgets/Qss/icons/original_svg/branch_end.svg` & `QT-PyQt-PySide-Custom-Widgets-0.6.6/Custom_Widgets/Qss/icons/original_svg/branch_end.svg`

 * *Files identical despite different names*

### Comparing `QT-PyQt-PySide-Custom-Widgets-0.6.5/Custom_Widgets/Qss/icons/original_svg/branch_line.svg` & `QT-PyQt-PySide-Custom-Widgets-0.6.6/Custom_Widgets/Qss/icons/original_svg/branch_line.svg`

 * *Files identical despite different names*

### Comparing `QT-PyQt-PySide-Custom-Widgets-0.6.5/Custom_Widgets/Qss/icons/original_svg/branch_more.svg` & `QT-PyQt-PySide-Custom-Widgets-0.6.6/Custom_Widgets/Qss/icons/original_svg/branch_more.svg`

 * *Files identical despite different names*

### Comparing `QT-PyQt-PySide-Custom-Widgets-0.6.5/Custom_Widgets/Qss/icons/original_svg/branch_open.svg` & `QT-PyQt-PySide-Custom-Widgets-0.6.6/Custom_Widgets/Qss/icons/original_svg/branch_open.svg`

 * *Files identical despite different names*

### Comparing `QT-PyQt-PySide-Custom-Widgets-0.6.5/Custom_Widgets/Qss/icons/original_svg/checkbox_checked.svg` & `QT-PyQt-PySide-Custom-Widgets-0.6.6/Custom_Widgets/Qss/icons/original_svg/checkbox_checked.svg`

 * *Files identical despite different names*

### Comparing `QT-PyQt-PySide-Custom-Widgets-0.6.5/Custom_Widgets/Qss/icons/original_svg/checkbox_indeterminate.svg` & `QT-PyQt-PySide-Custom-Widgets-0.6.6/Custom_Widgets/Qss/icons/original_svg/checkbox_indeterminate.svg`

 * *Files identical despite different names*

### Comparing `QT-PyQt-PySide-Custom-Widgets-0.6.5/Custom_Widgets/Qss/icons/original_svg/checkbox_unchecked.svg` & `QT-PyQt-PySide-Custom-Widgets-0.6.6/Custom_Widgets/Qss/icons/original_svg/checkbox_unchecked.svg`

 * *Files identical despite different names*

### Comparing `QT-PyQt-PySide-Custom-Widgets-0.6.5/Custom_Widgets/Qss/icons/original_svg/cloud-drizzle.svg` & `QT-PyQt-PySide-Custom-Widgets-0.6.6/Custom_Widgets/Qss/icons/original_svg/cloud-drizzle.svg`

 * *Files identical despite different names*

### Comparing `QT-PyQt-PySide-Custom-Widgets-0.6.5/Custom_Widgets/Qss/icons/original_svg/cloud-snow.svg` & `QT-PyQt-PySide-Custom-Widgets-0.6.6/Custom_Widgets/Qss/icons/original_svg/cloud-snow.svg`

 * *Files identical despite different names*

### Comparing `QT-PyQt-PySide-Custom-Widgets-0.6.5/Custom_Widgets/Qss/icons/original_svg/codesandbox.svg` & `QT-PyQt-PySide-Custom-Widgets-0.6.6/Custom_Widgets/Qss/icons/original_svg/codesandbox.svg`

 * *Files identical despite different names*

### Comparing `QT-PyQt-PySide-Custom-Widgets-0.6.5/Custom_Widgets/Qss/icons/original_svg/cpu.svg` & `QT-PyQt-PySide-Custom-Widgets-0.6.6/Custom_Widgets/Qss/icons/original_svg/cpu.svg`

 * *Files identical despite different names*

### Comparing `QT-PyQt-PySide-Custom-Widgets-0.6.5/Custom_Widgets/Qss/icons/original_svg/figma.svg` & `QT-PyQt-PySide-Custom-Widgets-0.6.6/Custom_Widgets/Qss/icons/original_svg/figma.svg`

 * *Files identical despite different names*

### Comparing `QT-PyQt-PySide-Custom-Widgets-0.6.5/Custom_Widgets/Qss/icons/original_svg/film.svg` & `QT-PyQt-PySide-Custom-Widgets-0.6.6/Custom_Widgets/Qss/icons/original_svg/film.svg`

 * *Files identical despite different names*

### Comparing `QT-PyQt-PySide-Custom-Widgets-0.6.5/Custom_Widgets/Qss/icons/original_svg/github.svg` & `QT-PyQt-PySide-Custom-Widgets-0.6.6/Custom_Widgets/Qss/icons/original_svg/github.svg`

 * *Files identical despite different names*

### Comparing `QT-PyQt-PySide-Custom-Widgets-0.6.5/Custom_Widgets/Qss/icons/original_svg/life-buoy.svg` & `QT-PyQt-PySide-Custom-Widgets-0.6.6/Custom_Widgets/Qss/icons/original_svg/life-buoy.svg`

 * *Files identical despite different names*

### Comparing `QT-PyQt-PySide-Custom-Widgets-0.6.5/Custom_Widgets/Qss/icons/original_svg/line_horizontal.svg` & `QT-PyQt-PySide-Custom-Widgets-0.6.6/Custom_Widgets/Qss/icons/original_svg/line_horizontal.svg`

 * *Files identical despite different names*

### Comparing `QT-PyQt-PySide-Custom-Widgets-0.6.5/Custom_Widgets/Qss/icons/original_svg/line_vertical.svg` & `QT-PyQt-PySide-Custom-Widgets-0.6.6/Custom_Widgets/Qss/icons/original_svg/line_vertical.svg`

 * *Files identical despite different names*

### Comparing `QT-PyQt-PySide-Custom-Widgets-0.6.5/Custom_Widgets/Qss/icons/original_svg/loader.svg` & `QT-PyQt-PySide-Custom-Widgets-0.6.6/Custom_Widgets/Qss/icons/original_svg/loader.svg`

 * *Files identical despite different names*

### Comparing `QT-PyQt-PySide-Custom-Widgets-0.6.5/Custom_Widgets/Qss/icons/original_svg/phone-call.svg` & `QT-PyQt-PySide-Custom-Widgets-0.6.6/Custom_Widgets/Qss/icons/original_svg/phone-call.svg`

 * *Files identical despite different names*

### Comparing `QT-PyQt-PySide-Custom-Widgets-0.6.5/Custom_Widgets/Qss/icons/original_svg/phone-forwarded.svg` & `QT-PyQt-PySide-Custom-Widgets-0.6.6/Custom_Widgets/Qss/icons/original_svg/phone-forwarded.svg`

 * *Files identical despite different names*

### Comparing `QT-PyQt-PySide-Custom-Widgets-0.6.5/Custom_Widgets/Qss/icons/original_svg/phone-incoming.svg` & `QT-PyQt-PySide-Custom-Widgets-0.6.6/Custom_Widgets/Qss/icons/original_svg/phone-incoming.svg`

 * *Files identical despite different names*

### Comparing `QT-PyQt-PySide-Custom-Widgets-0.6.5/Custom_Widgets/Qss/icons/original_svg/phone-missed.svg` & `QT-PyQt-PySide-Custom-Widgets-0.6.6/Custom_Widgets/Qss/icons/original_svg/phone-missed.svg`

 * *Files identical despite different names*

### Comparing `QT-PyQt-PySide-Custom-Widgets-0.6.5/Custom_Widgets/Qss/icons/original_svg/phone-off.svg` & `QT-PyQt-PySide-Custom-Widgets-0.6.6/Custom_Widgets/Qss/icons/original_svg/phone-off.svg`

 * *Files identical despite different names*

### Comparing `QT-PyQt-PySide-Custom-Widgets-0.6.5/Custom_Widgets/Qss/icons/original_svg/phone-outgoing.svg` & `QT-PyQt-PySide-Custom-Widgets-0.6.6/Custom_Widgets/Qss/icons/original_svg/phone-outgoing.svg`

 * *Files identical despite different names*

### Comparing `QT-PyQt-PySide-Custom-Widgets-0.6.5/Custom_Widgets/Qss/icons/original_svg/phone.svg` & `QT-PyQt-PySide-Custom-Widgets-0.6.6/Custom_Widgets/Qss/icons/original_svg/phone.svg`

 * *Files identical despite different names*

### Comparing `QT-PyQt-PySide-Custom-Widgets-0.6.5/Custom_Widgets/Qss/icons/original_svg/radio_checked.svg` & `QT-PyQt-PySide-Custom-Widgets-0.6.6/Custom_Widgets/Qss/icons/original_svg/radio_checked.svg`

 * *Files identical despite different names*

### Comparing `QT-PyQt-PySide-Custom-Widgets-0.6.5/Custom_Widgets/Qss/icons/original_svg/radio_unchecked.svg` & `QT-PyQt-PySide-Custom-Widgets-0.6.6/Custom_Widgets/Qss/icons/original_svg/radio_unchecked.svg`

 * *Files identical despite different names*

### Comparing `QT-PyQt-PySide-Custom-Widgets-0.6.5/Custom_Widgets/Qss/icons/original_svg/settings.svg` & `QT-PyQt-PySide-Custom-Widgets-0.6.6/Custom_Widgets/Qss/icons/original_svg/settings.svg`

 * *Files identical despite different names*

### Comparing `QT-PyQt-PySide-Custom-Widgets-0.6.5/Custom_Widgets/Qss/icons/original_svg/slack.svg` & `QT-PyQt-PySide-Custom-Widgets-0.6.6/Custom_Widgets/Qss/icons/original_svg/slack.svg`

 * *Files identical despite different names*

### Comparing `QT-PyQt-PySide-Custom-Widgets-0.6.5/Custom_Widgets/Qss/icons/original_svg/sliders.svg` & `QT-PyQt-PySide-Custom-Widgets-0.6.6/Custom_Widgets/Qss/icons/original_svg/sliders.svg`

 * *Files identical despite different names*

### Comparing `QT-PyQt-PySide-Custom-Widgets-0.6.5/Custom_Widgets/Qss/icons/original_svg/sun.svg` & `QT-PyQt-PySide-Custom-Widgets-0.6.6/Custom_Widgets/Qss/icons/original_svg/sun.svg`

 * *Files identical despite different names*

### Comparing `QT-PyQt-PySide-Custom-Widgets-0.6.5/Custom_Widgets/Qss/icons/original_svg/sunrise.svg` & `QT-PyQt-PySide-Custom-Widgets-0.6.6/Custom_Widgets/Qss/icons/original_svg/sunrise.svg`

 * *Files identical despite different names*

### Comparing `QT-PyQt-PySide-Custom-Widgets-0.6.5/Custom_Widgets/Qss/icons/original_svg/sunset.svg` & `QT-PyQt-PySide-Custom-Widgets-0.6.6/Custom_Widgets/Qss/icons/original_svg/sunset.svg`

 * *Files identical despite different names*

### Comparing `QT-PyQt-PySide-Custom-Widgets-0.6.5/Custom_Widgets/Qss/icons/original_svg/toolbar_move_horizontal.svg` & `QT-PyQt-PySide-Custom-Widgets-0.6.6/Custom_Widgets/Qss/icons/original_svg/toolbar_move_horizontal.svg`

 * *Files identical despite different names*

### Comparing `QT-PyQt-PySide-Custom-Widgets-0.6.5/Custom_Widgets/Qss/icons/original_svg/toolbar_move_vertical.svg` & `QT-PyQt-PySide-Custom-Widgets-0.6.6/Custom_Widgets/Qss/icons/original_svg/toolbar_move_vertical.svg`

 * *Files identical despite different names*

### Comparing `QT-PyQt-PySide-Custom-Widgets-0.6.5/Custom_Widgets/Qss/icons/original_svg/toolbar_separator_horizontal.svg` & `QT-PyQt-PySide-Custom-Widgets-0.6.6/Custom_Widgets/Qss/icons/original_svg/toolbar_separator_horizontal.svg`

 * *Files identical despite different names*

### Comparing `QT-PyQt-PySide-Custom-Widgets-0.6.5/Custom_Widgets/Qss/icons/original_svg/toolbar_separator_vertical.svg` & `QT-PyQt-PySide-Custom-Widgets-0.6.6/Custom_Widgets/Qss/icons/original_svg/toolbar_separator_vertical.svg`

 * *Files identical despite different names*

### Comparing `QT-PyQt-PySide-Custom-Widgets-0.6.5/Custom_Widgets/Qss/icons/original_svg/transparent.svg` & `QT-PyQt-PySide-Custom-Widgets-0.6.6/Custom_Widgets/Qss/icons/original_svg/transparent.svg`

 * *Files identical despite different names*

### Comparing `QT-PyQt-PySide-Custom-Widgets-0.6.5/Custom_Widgets/Qss/icons/original_svg/wifi-off.svg` & `QT-PyQt-PySide-Custom-Widgets-0.6.6/Custom_Widgets/Qss/icons/original_svg/wifi-off.svg`

 * *Files identical despite different names*

### Comparing `QT-PyQt-PySide-Custom-Widgets-0.6.5/Custom_Widgets/Qss/icons/original_svg/window_close.svg` & `QT-PyQt-PySide-Custom-Widgets-0.6.6/Custom_Widgets/Qss/icons/original_svg/window_close.svg`

 * *Files identical despite different names*

### Comparing `QT-PyQt-PySide-Custom-Widgets-0.6.5/Custom_Widgets/Qss/icons/original_svg/window_grip.svg` & `QT-PyQt-PySide-Custom-Widgets-0.6.6/Custom_Widgets/Qss/icons/original_svg/window_grip.svg`

 * *Files identical despite different names*

### Comparing `QT-PyQt-PySide-Custom-Widgets-0.6.5/Custom_Widgets/Qss/icons/original_svg/window_minimize.svg` & `QT-PyQt-PySide-Custom-Widgets-0.6.6/Custom_Widgets/Qss/icons/original_svg/window_minimize.svg`

 * *Files identical despite different names*

### Comparing `QT-PyQt-PySide-Custom-Widgets-0.6.5/Custom_Widgets/Qss/icons/original_svg/window_undock.svg` & `QT-PyQt-PySide-Custom-Widgets-0.6.6/Custom_Widgets/Qss/icons/original_svg/window_undock.svg`

 * *Files identical despite different names*

### Comparing `QT-PyQt-PySide-Custom-Widgets-0.6.5/Custom_Widgets/Qss/icons/original_svg/youtube.svg` & `QT-PyQt-PySide-Custom-Widgets-0.6.6/Custom_Widgets/Qss/icons/original_svg/youtube.svg`

 * *Files identical despite different names*

### Comparing `QT-PyQt-PySide-Custom-Widgets-0.6.5/Custom_Widgets/RoundProgressBar.py` & `QT-PyQt-PySide-Custom-Widgets-0.6.6/Custom_Widgets/RoundProgressBar.py`

 * *Files identical despite different names*

### Comparing `QT-PyQt-PySide-Custom-Widgets-0.6.5/Custom_Widgets/SpiralProgressBar.py` & `QT-PyQt-PySide-Custom-Widgets-0.6.6/Custom_Widgets/SpiralProgressBar.py`

 * *Files identical despite different names*

### Comparing `QT-PyQt-PySide-Custom-Widgets-0.6.5/Custom_Widgets/Widgets.py` & `QT-PyQt-PySide-Custom-Widgets-0.6.6/Custom_Widgets/Widgets.py`

 * *Files identical despite different names*

### Comparing `QT-PyQt-PySide-Custom-Widgets-0.6.5/Custom_Widgets/WidgetsWorker.py` & `QT-PyQt-PySide-Custom-Widgets-0.6.6/Custom_Widgets/WidgetsWorker.py`

 * *Files identical despite different names*

### Comparing `QT-PyQt-PySide-Custom-Widgets-0.6.5/Custom_Widgets/components/python/__pycache__/main.cpython-310.pyc` & `QT-PyQt-PySide-Custom-Widgets-0.6.6/Custom_Widgets/components/python/__pycache__/main.cpython-310.pyc`

 * *Files identical despite different names*

### Comparing `QT-PyQt-PySide-Custom-Widgets-0.6.5/Custom_Widgets/components/python/__pycache__/main.cpython-38.pyc` & `QT-PyQt-PySide-Custom-Widgets-0.6.6/Custom_Widgets/components/python/__pycache__/main.cpython-38.pyc`

 * *Format-specific differences are supported for Python .pyc files but no file-specific differences were detected; falling back to a binary diff. file(1) reports: Byte-compiled Python module for CPython 3.8, timestamp-based, .py timestamp: Wed Jun 21 20:45:31 2023 UTC, .py size: 2679 bytes*

 * *Could not decompile bytecode: bad marshal data (unknown type code)*

 * *Files 0% similar despite different names*

```diff
@@ -1,8 +1,8 @@
-00000000: 550d 0d0a 0000 0000 6b61 9364 770a 0000  U.......ka.dw...
+00000000: 550d 0d0a 0000 0000 626c 9364 770a 0000  U.......bl.dw...
 00000010: e300 0000 0000 0000 0000 0000 0000 0000  ................
 00000020: 0004 0000 0040 0000 0073 6800 0000 6400  .....@...sh...d.
 00000030: 6401 6c00 5a00 6400 6401 6c01 5a01 6400  d.l.Z.d.d.l.Z.d.
 00000040: 6402 6c02 5400 6400 6402 6c03 5400 6504  d.l.T.d.d.l.T.e.
 00000050: 8300 5a05 4700 6403 6404 8400 6404 6506  ..Z.G.d.d...d.e.
 00000060: 8303 5a07 6508 6405 6b02 7264 6509 6501  ..Z.e.d.k.rde.e.
 00000070: 6a0a 8301 5a0b 6507 8300 5a0c 650c a00d  j...Z.e...Z.e...
```

### Comparing `QT-PyQt-PySide-Custom-Widgets-0.6.5/Custom_Widgets/components/python/__pycache__/ui_interface.cpython-310.pyc` & `QT-PyQt-PySide-Custom-Widgets-0.6.6/Custom_Widgets/components/python/__pycache__/ui_interface.cpython-310.pyc`

 * *Files identical despite different names*

### Comparing `QT-PyQt-PySide-Custom-Widgets-0.6.5/Custom_Widgets/components/python/__pycache__/ui_interface.cpython-38.pyc` & `QT-PyQt-PySide-Custom-Widgets-0.6.6/Custom_Widgets/components/python/__pycache__/ui_interface.cpython-38.pyc`

 * *Format-specific differences are supported for Python .pyc files but no file-specific differences were detected; falling back to a binary diff. file(1) reports: Byte-compiled Python module for CPython 3.8, timestamp-based, .py timestamp: Wed Jun 21 20:45:31 2023 UTC, .py size: 3127 bytes*

 * *Could not decompile bytecode: bad marshal data (unknown type code)*

 * *Files 2% similar despite different names*

```diff
@@ -1,8 +1,8 @@
-00000000: 550d 0d0a 0000 0000 6b61 9364 370c 0000  U.......ka.d7...
+00000000: 550d 0d0a 0000 0000 626c 9364 370c 0000  U.......bl.d7...
 00000010: e300 0000 0000 0000 0000 0000 0000 0000  ................
 00000020: 0004 0000 0040 0000 0073 3400 0000 6400  .....@...s4...d.
 00000030: 6401 6c00 5400 6400 6401 6c01 5400 6400  d.l.T.d.d.l.T.d.
 00000040: 6401 6c02 5400 6400 6402 6c03 5a03 4700  d.l.T.d.d.l.Z.G.
 00000050: 6403 6404 8400 6404 6504 8303 5a05 6402  d.d...d.e...Z.d.
 00000060: 5300 2905 e900 0000 0029 01da 012a 4e63  S.)......)...*Nc
 00000070: 0000 0000 0000 0000 0000 0000 0000 0000  ................
```

### Comparing `QT-PyQt-PySide-Custom-Widgets-0.6.5/Custom_Widgets/components/python/main.py` & `QT-PyQt-PySide-Custom-Widgets-0.6.6/Custom_Widgets/components/python/main.py`

 * *Files identical despite different names*

### Comparing `QT-PyQt-PySide-Custom-Widgets-0.6.5/Custom_Widgets/components/python/ui_interface.py` & `QT-PyQt-PySide-Custom-Widgets-0.6.6/Custom_Widgets/components/python/ui_interface.py`

 * *Files identical despite different names*

### Comparing `QT-PyQt-PySide-Custom-Widgets-0.6.5/Custom_Widgets/components/uis/interface.ui` & `QT-PyQt-PySide-Custom-Widgets-0.6.6/Custom_Widgets/components/uis/interface.ui`

 * *Files identical despite different names*

### Comparing `QT-PyQt-PySide-Custom-Widgets-0.6.5/Custom_Widgets/interface.ui` & `QT-PyQt-PySide-Custom-Widgets-0.6.6/Custom_Widgets/interface.ui`

 * *Files identical despite different names*

### Comparing `QT-PyQt-PySide-Custom-Widgets-0.6.5/Custom_Widgets/main.py` & `QT-PyQt-PySide-Custom-Widgets-0.6.6/Custom_Widgets/main.py`

 * *Files identical despite different names*

### Comparing `QT-PyQt-PySide-Custom-Widgets-0.6.5/LICENSE` & `QT-PyQt-PySide-Custom-Widgets-0.6.6/LICENSE`

 * *Files identical despite different names*

### Comparing `QT-PyQt-PySide-Custom-Widgets-0.6.5/PKG-INFO` & `QT-PyQt-PySide-Custom-Widgets-0.6.6/PKG-INFO`

 * *Files 2% similar despite different names*

```diff
@@ -1,16 +1,16 @@
 Metadata-Version: 2.1
 Name: QT-PyQt-PySide-Custom-Widgets
-Version: 0.6.5
+Version: 0.6.6
 Summary: Custom widgets and widget animations made for QT applications
 Home-page: https://github.com/KhamisiKibet/QT-PyQt-PySide-Custom-Widgets
 Author: Khamisi Kibet
 Author-email: kibetkhamisi@gmail.com
 License: GNU General Public License v3.0
-Keywords: PySide,PyQt,animation,custom,widgets,QML,C++,QT Creator
+Keywords: PySide,PyQt,animation,custom,widgets,QML,C++,QT Creator,Moderm GUI,UI Design
 Platform: UNKNOWN
 Classifier: Development Status :: 3 - Alpha
 Classifier: Intended Audience :: Developers
 Classifier: Topic :: Software Development :: Build Tools
 Classifier: License :: OSI Approved :: MIT License
 Classifier: Programming Language :: Python :: 3.6
 Classifier: Programming Language :: Python :: 3.7
```

### Comparing `QT-PyQt-PySide-Custom-Widgets-0.6.5/QT_PyQt_PySide_Custom_Widgets.egg-info/PKG-INFO` & `QT-PyQt-PySide-Custom-Widgets-0.6.6/QT_PyQt_PySide_Custom_Widgets.egg-info/PKG-INFO`

 * *Files 2% similar despite different names*

```diff
@@ -1,16 +1,16 @@
 Metadata-Version: 2.1
 Name: QT-PyQt-PySide-Custom-Widgets
-Version: 0.6.5
+Version: 0.6.6
 Summary: Custom widgets and widget animations made for QT applications
 Home-page: https://github.com/KhamisiKibet/QT-PyQt-PySide-Custom-Widgets
 Author: Khamisi Kibet
 Author-email: kibetkhamisi@gmail.com
 License: GNU General Public License v3.0
-Keywords: PySide,PyQt,animation,custom,widgets,QML,C++,QT Creator
+Keywords: PySide,PyQt,animation,custom,widgets,QML,C++,QT Creator,Moderm GUI,UI Design
 Platform: UNKNOWN
 Classifier: Development Status :: 3 - Alpha
 Classifier: Intended Audience :: Developers
 Classifier: Topic :: Software Development :: Build Tools
 Classifier: License :: OSI Approved :: MIT License
 Classifier: Programming Language :: Python :: 3.6
 Classifier: Programming Language :: Python :: 3.7
```

### Comparing `QT-PyQt-PySide-Custom-Widgets-0.6.5/QT_PyQt_PySide_Custom_Widgets.egg-info/SOURCES.txt` & `QT-PyQt-PySide-Custom-Widgets-0.6.6/QT_PyQt_PySide_Custom_Widgets.egg-info/SOURCES.txt`

 * *Files 2% similar despite different names*

```diff
@@ -27,23 +27,27 @@
 Custom_Widgets/Qss/SvgToPngIcons.py
 Custom_Widgets/Qss/__init__.py
 Custom_Widgets/Qss/_styles.scss
 Custom_Widgets/Qss/colorsystem.py
 Custom_Widgets/Qss/main.scss
 Custom_Widgets/Qss/__pycache__/QSS_Resources.cpython-39.pyc
 Custom_Widgets/Qss/__pycache__/SassCompiler.cpython-310.pyc
+Custom_Widgets/Qss/__pycache__/SassCompiler.cpython-311.pyc
 Custom_Widgets/Qss/__pycache__/SassCompiler.cpython-38.pyc
 Custom_Widgets/Qss/__pycache__/SvgToPngIcons.cpython-310.pyc
+Custom_Widgets/Qss/__pycache__/SvgToPngIcons.cpython-311.pyc
 Custom_Widgets/Qss/__pycache__/SvgToPngIcons.cpython-38.pyc
 Custom_Widgets/Qss/__pycache__/SvgToPngIcons.cpython-39.pyc
 Custom_Widgets/Qss/__pycache__/__init__.cpython-310.pyc
+Custom_Widgets/Qss/__pycache__/__init__.cpython-311.pyc
 Custom_Widgets/Qss/__pycache__/__init__.cpython-37.pyc
 Custom_Widgets/Qss/__pycache__/__init__.cpython-38.pyc
 Custom_Widgets/Qss/__pycache__/__init__.cpython-39.pyc
 Custom_Widgets/Qss/__pycache__/colorsystem.cpython-310.pyc
+Custom_Widgets/Qss/__pycache__/colorsystem.cpython-311.pyc
 Custom_Widgets/Qss/__pycache__/colorsystem.cpython-37.pyc
 Custom_Widgets/Qss/__pycache__/colorsystem.cpython-38.pyc
 Custom_Widgets/Qss/__pycache__/colorsystem.cpython-39.pyc
 Custom_Widgets/Qss/__pycache__/resources_rc.cpython-39.pyc
 Custom_Widgets/Qss/__pycache__/sassCompiler.cpython-39.pyc
 Custom_Widgets/Qss/icons/original_svg/activity.svg
 Custom_Widgets/Qss/icons/original_svg/airplay.svg
```

### Comparing `QT-PyQt-PySide-Custom-Widgets-0.6.5/README.md` & `QT-PyQt-PySide-Custom-Widgets-0.6.6/README.md`

 * *Files identical despite different names*

### Comparing `QT-PyQt-PySide-Custom-Widgets-0.6.5/setup.py` & `QT-PyQt-PySide-Custom-Widgets-0.6.6/setup.py`

 * *Files 2% similar despite different names*

```diff
@@ -12,24 +12,24 @@
     name = 'QT-PyQt-PySide-Custom-Widgets',         # How you named your package folder (MyLib)
     packages = [
         'Custom_Widgets',
         'Custom_Widgets.ProgressIndicator',
         'Custom_Widgets.Qss',
     ],
     include_package_data=True,
-    version = '0.6.5',      # Start with a small number and increase it with every change you make
+    version = '0.6.6',      # Start with a small number and increase it with every change you make
     license="GNU General Public License v3.0",        # Chose a license from here: https://help.github.com/articles/licensing-a-repository
     description = 'Custom widgets and widget animations made for QT applications',   # Give a short description about your library
     long_description=README,
     long_description_content_type="text/markdown",
     author = 'Khamisi Kibet',                   # Type in your name
     author_email = 'kibetkhamisi@gmail.com',      # Type in your E-Mail
     url = 'https://github.com/KhamisiKibet/QT-PyQt-PySide-Custom-Widgets',   # Provide either the link to your github or to your website
     # download_url = 'https://github.com/user/reponame/archive/v_01.tar.gz',    # I explain this later on
-    keywords = ['PySide', 'PyQt', 'animation', 'custom', 'widgets', "QML", "C++", "QT Creator"],   # Keywords that define your package best
+    keywords = ['PySide', 'PyQt', 'animation', 'custom', 'widgets', "QML", "C++", "QT Creator", "Moderm GUI", "UI Design"],   # Keywords that define your package best
     install_requires=[
         # "PySide2",
         # "PyQt5",
         "qtpy",
         "iconify",
         "cairosvg",
         "qtsass",
```

