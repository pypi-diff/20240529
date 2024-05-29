# Comparing `tmp/apysc-4.4.2.tar.gz` & `tmp/apysc-4.4.3.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "apysc-4.4.2.tar", last modified: Thu May 23 14:24:13 2024, max compression
+gzip compressed data, was "apysc-4.4.3.tar", last modified: Wed May 29 12:25:10 2024, max compression
```

## Comparing `apysc-4.4.2.tar` & `apysc-4.4.3.tar`

### file list

```diff
@@ -1,1910 +1,1915 @@
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-23 14:24:13.510301 apysc-4.4.2/
--rw-r--r--   0 runner    (1001) docker     (127)     1064 2024-05-23 14:23:55.000000 apysc-4.4.2/LICENSE
--rw-r--r--   0 runner    (1001) docker     (127)       24 2024-05-23 14:23:55.000000 apysc-4.4.2/MANIFEST.in
--rw-r--r--   0 runner    (1001) docker     (127)      828 2024-05-23 14:24:13.510301 apysc-4.4.2/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (127)     6982 2024-05-23 14:23:55.000000 apysc-4.4.2/README.md
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-23 14:24:13.274299 apysc-4.4.2/apysc/
--rw-r--r--   0 runner    (1001) docker     (127)   120458 2024-05-23 14:23:55.000000 apysc-4.4.2/apysc/__init__.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-23 14:24:13.282299 apysc-4.4.2/apysc/_animation/
--rw-r--r--   0 runner    (1001) docker     (127)        0 2024-05-23 14:23:55.000000 apysc-4.4.2/apysc/_animation/__init__.py
--rw-r--r--   0 runner    (1001) docker     (127)    10351 2024-05-23 14:23:55.000000 apysc-4.4.2/apysc/_animation/animation_base.py
--rw-r--r--   0 runner    (1001) docker     (127)     4646 2024-05-23 14:23:55.000000 apysc-4.4.2/apysc/_animation/animation_cx.py
--rw-r--r--   0 runner    (1001) docker     (127)     3350 2024-05-23 14:23:55.000000 apysc-4.4.2/apysc/_animation/animation_cx_mixin.py
--rw-r--r--   0 runner    (1001) docker     (127)     4646 2024-05-23 14:23:55.000000 apysc-4.4.2/apysc/_animation/animation_cy.py
--rw-r--r--   0 runner    (1001) docker     (127)     3353 2024-05-23 14:23:55.000000 apysc-4.4.2/apysc/_animation/animation_cy_mixin.py
--rw-r--r--   0 runner    (1001) docker     (127)     4809 2024-05-23 14:23:55.000000 apysc-4.4.2/apysc/_animation/animation_fill_alpha.py
--rw-r--r--   0 runner    (1001) docker     (127)     3406 2024-05-23 14:23:55.000000 apysc-4.4.2/apysc/_animation/animation_fill_alpha_mixin.py
--rw-r--r--   0 runner    (1001) docker     (127)     4613 2024-05-23 14:23:55.000000 apysc-4.4.2/apysc/_animation/animation_fill_color.py
--rw-r--r--   0 runner    (1001) docker     (127)     3553 2024-05-23 14:23:55.000000 apysc-4.4.2/apysc/_animation/animation_fill_color_mixin.py
--rw-r--r--   0 runner    (1001) docker     (127)     1851 2024-05-23 14:23:55.000000 apysc-4.4.2/apysc/_animation/animation_finish_mixin.py
--rw-r--r--   0 runner    (1001) docker     (127)     4744 2024-05-23 14:23:55.000000 apysc-4.4.2/apysc/_animation/animation_height.py
--rw-r--r--   0 runner    (1001) docker     (127)     4942 2024-05-23 14:23:55.000000 apysc-4.4.2/apysc/_animation/animation_height_for_ellipse.py
--rw-r--r--   0 runner    (1001) docker     (127)     3245 2024-05-23 14:23:55.000000 apysc-4.4.2/apysc/_animation/animation_height_for_ellipse_mixin.py
--rw-r--r--   0 runner    (1001) docker     (127)     3504 2024-05-23 14:23:55.000000 apysc-4.4.2/apysc/_animation/animation_height_mixin.py
--rw-r--r--   0 runner    (1001) docker     (127)     4974 2024-05-23 14:23:55.000000 apysc-4.4.2/apysc/_animation/animation_line_alpha.py
--rw-r--r--   0 runner    (1001) docker     (127)     3659 2024-05-23 14:23:55.000000 apysc-4.4.2/apysc/_animation/animation_line_alpha_mixin.py
--rw-r--r--   0 runner    (1001) docker     (127)     4663 2024-05-23 14:23:55.000000 apysc-4.4.2/apysc/_animation/animation_line_color.py
--rw-r--r--   0 runner    (1001) docker     (127)     3630 2024-05-23 14:23:55.000000 apysc-4.4.2/apysc/_animation/animation_line_color_mixin.py
--rw-r--r--   0 runner    (1001) docker     (127)     5038 2024-05-23 14:23:55.000000 apysc-4.4.2/apysc/_animation/animation_line_thickness.py
--rw-r--r--   0 runner    (1001) docker     (127)     3746 2024-05-23 14:23:55.000000 apysc-4.4.2/apysc/_animation/animation_line_thickness_mixin.py
--rw-r--r--   0 runner    (1001) docker     (127)      721 2024-05-23 14:23:55.000000 apysc-4.4.2/apysc/_animation/animation_mixins.py
--rw-r--r--   0 runner    (1001) docker     (127)     5340 2024-05-23 14:23:55.000000 apysc-4.4.2/apysc/_animation/animation_move.py
--rw-r--r--   0 runner    (1001) docker     (127)     3674 2024-05-23 14:23:55.000000 apysc-4.4.2/apysc/_animation/animation_move_mixin.py
--rw-r--r--   0 runner    (1001) docker     (127)    10250 2024-05-23 14:23:55.000000 apysc-4.4.2/apysc/_animation/animation_parallel.py
--rw-r--r--   0 runner    (1001) docker     (127)     4186 2024-05-23 14:23:55.000000 apysc-4.4.2/apysc/_animation/animation_parallel_mixin.py
--rw-r--r--   0 runner    (1001) docker     (127)     1818 2024-05-23 14:23:55.000000 apysc-4.4.2/apysc/_animation/animation_pause_mixin.py
--rw-r--r--   0 runner    (1001) docker     (127)     2084 2024-05-23 14:23:55.000000 apysc-4.4.2/apysc/_animation/animation_play_mixin.py
--rw-r--r--   0 runner    (1001) docker     (127)     4678 2024-05-23 14:23:55.000000 apysc-4.4.2/apysc/_animation/animation_radius.py
--rw-r--r--   0 runner    (1001) docker     (127)     3418 2024-05-23 14:23:55.000000 apysc-4.4.2/apysc/_animation/animation_radius_mixin.py
--rw-r--r--   0 runner    (1001) docker     (127)     1790 2024-05-23 14:23:55.000000 apysc-4.4.2/apysc/_animation/animation_reset_mixin.py
--rw-r--r--   0 runner    (1001) docker     (127)     2220 2024-05-23 14:23:55.000000 apysc-4.4.2/apysc/_animation/animation_reverse_mixin.py
--rw-r--r--   0 runner    (1001) docker     (127)     6189 2024-05-23 14:23:55.000000 apysc-4.4.2/apysc/_animation/animation_rotation_around_center.py
--rw-r--r--   0 runner    (1001) docker     (127)     3836 2024-05-23 14:23:55.000000 apysc-4.4.2/apysc/_animation/animation_rotation_around_center_mixin.py
--rw-r--r--   0 runner    (1001) docker     (127)     7607 2024-05-23 14:23:55.000000 apysc-4.4.2/apysc/_animation/animation_rotation_around_point.py
--rw-r--r--   0 runner    (1001) docker     (127)     4292 2024-05-23 14:23:55.000000 apysc-4.4.2/apysc/_animation/animation_rotation_around_point_mixin.py
--rw-r--r--   0 runner    (1001) docker     (127)     6052 2024-05-23 14:23:55.000000 apysc-4.4.2/apysc/_animation/animation_scale_x_from_center.py
--rw-r--r--   0 runner    (1001) docker     (127)     3816 2024-05-23 14:23:55.000000 apysc-4.4.2/apysc/_animation/animation_scale_x_from_center_mixin.py
--rw-r--r--   0 runner    (1001) docker     (127)     6911 2024-05-23 14:23:55.000000 apysc-4.4.2/apysc/_animation/animation_scale_x_from_point.py
--rw-r--r--   0 runner    (1001) docker     (127)     4032 2024-05-23 14:23:55.000000 apysc-4.4.2/apysc/_animation/animation_scale_x_from_point_mixin.py
--rw-r--r--   0 runner    (1001) docker     (127)     6052 2024-05-23 14:23:55.000000 apysc-4.4.2/apysc/_animation/animation_scale_y_from_center.py
--rw-r--r--   0 runner    (1001) docker     (127)     3813 2024-05-23 14:23:55.000000 apysc-4.4.2/apysc/_animation/animation_scale_y_from_center_mixin.py
--rw-r--r--   0 runner    (1001) docker     (127)     6921 2024-05-23 14:23:55.000000 apysc-4.4.2/apysc/_animation/animation_scale_y_from_point.py
--rw-r--r--   0 runner    (1001) docker     (127)     4034 2024-05-23 14:23:55.000000 apysc-4.4.2/apysc/_animation/animation_scale_y_from_point_mixin.py
--rw-r--r--   0 runner    (1001) docker     (127)     2192 2024-05-23 14:23:55.000000 apysc-4.4.2/apysc/_animation/animation_time_mixin.py
--rw-r--r--   0 runner    (1001) docker     (127)     4730 2024-05-23 14:23:55.000000 apysc-4.4.2/apysc/_animation/animation_width.py
--rw-r--r--   0 runner    (1001) docker     (127)     4922 2024-05-23 14:23:55.000000 apysc-4.4.2/apysc/_animation/animation_width_for_ellipse.py
--rw-r--r--   0 runner    (1001) docker     (127)     3653 2024-05-23 14:23:55.000000 apysc-4.4.2/apysc/_animation/animation_width_for_ellipse_mixin.py
--rw-r--r--   0 runner    (1001) docker     (127)     3484 2024-05-23 14:23:55.000000 apysc-4.4.2/apysc/_animation/animation_width_mixin.py
--rw-r--r--   0 runner    (1001) docker     (127)     4654 2024-05-23 14:23:55.000000 apysc-4.4.2/apysc/_animation/animation_x.py
--rw-r--r--   0 runner    (1001) docker     (127)     3333 2024-05-23 14:23:55.000000 apysc-4.4.2/apysc/_animation/animation_x_mixin.py
--rw-r--r--   0 runner    (1001) docker     (127)     4645 2024-05-23 14:23:55.000000 apysc-4.4.2/apysc/_animation/animation_y.py
--rw-r--r--   0 runner    (1001) docker     (127)     3333 2024-05-23 14:23:55.000000 apysc-4.4.2/apysc/_animation/animation_y_mixin.py
--rw-r--r--   0 runner    (1001) docker     (127)     5409 2024-05-23 14:23:55.000000 apysc-4.4.2/apysc/_animation/easing.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-23 14:24:13.282299 apysc-4.4.2/apysc/_auto_reloading/
--rw-r--r--   0 runner    (1001) docker     (127)        0 2024-05-23 14:23:55.000000 apysc-4.4.2/apysc/_auto_reloading/__init__.py
--rw-r--r--   0 runner    (1001) docker     (127)     3700 2024-05-23 14:23:55.000000 apysc-4.4.2/apysc/_auto_reloading/auto_reloading_decorator.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-23 14:24:13.286299 apysc-4.4.2/apysc/_branch/
--rw-r--r--   0 runner    (1001) docker     (127)        0 2024-05-23 14:23:55.000000 apysc-4.4.2/apysc/_branch/__init__.py
--rw-r--r--   0 runner    (1001) docker     (127)     5575 2024-05-23 14:23:55.000000 apysc-4.4.2/apysc/_branch/_elif.py
--rw-r--r--   0 runner    (1001) docker     (127)     3981 2024-05-23 14:23:55.000000 apysc-4.4.2/apysc/_branch/_else.py
--rw-r--r--   0 runner    (1001) docker     (127)     3781 2024-05-23 14:23:55.000000 apysc-4.4.2/apysc/_branch/_if.py
--rw-r--r--   0 runner    (1001) docker     (127)     4806 2024-05-23 14:23:55.000000 apysc-4.4.2/apysc/_branch/if_base.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-23 14:24:13.286299 apysc-4.4.2/apysc/_callable/
--rw-r--r--   0 runner    (1001) docker     (127)        0 2024-05-23 14:23:55.000000 apysc-4.4.2/apysc/_callable/__init__.py
--rw-r--r--   0 runner    (1001) docker     (127)     3444 2024-05-23 14:23:55.000000 apysc-4.4.2/apysc/_callable/callable_util.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-23 14:24:13.290299 apysc-4.4.2/apysc/_chart/
--rw-r--r--   0 runner    (1001) docker     (127)        0 2024-05-23 14:23:55.000000 apysc-4.4.2/apysc/_chart/__init__.py
--rw-r--r--   0 runner    (1001) docker     (127)     2177 2024-05-23 14:23:55.000000 apysc-4.4.2/apysc/_chart/add_background_mixin.py
--rw-r--r--   0 runner    (1001) docker     (127)     1768 2024-05-23 14:23:55.000000 apysc-4.4.2/apysc/_chart/add_border_mixin.py
--rw-r--r--   0 runner    (1001) docker     (127)     1516 2024-05-23 14:23:55.000000 apysc-4.4.2/apysc/_chart/axis_label_bold_mixin.py
--rw-r--r--   0 runner    (1001) docker     (127)     1538 2024-05-23 14:23:55.000000 apysc-4.4.2/apysc/_chart/axis_label_fill_alpha_mixin.py
--rw-r--r--   0 runner    (1001) docker     (127)      871 2024-05-23 14:23:55.000000 apysc-4.4.2/apysc/_chart/axis_label_fill_color_mixin.py
--rw-r--r--   0 runner    (1001) docker     (127)     1896 2024-05-23 14:23:55.000000 apysc-4.4.2/apysc/_chart/axis_label_font_family_mixin.py
--rw-r--r--   0 runner    (1001) docker     (127)     1578 2024-05-23 14:23:55.000000 apysc-4.4.2/apysc/_chart/axis_label_font_size_mixin.py
--rw-r--r--   0 runner    (1001) docker     (127)     1557 2024-05-23 14:23:55.000000 apysc-4.4.2/apysc/_chart/axis_label_italic_mixin.py
--rw-r--r--   0 runner    (1001) docker     (127)     1477 2024-05-23 14:23:55.000000 apysc-4.4.2/apysc/_chart/axis_line_alpha_mixin.py
--rw-r--r--   0 runner    (1001) docker     (127)      757 2024-05-23 14:23:55.000000 apysc-4.4.2/apysc/_chart/axis_line_color_mixin.py
--rw-r--r--   0 runner    (1001) docker     (127)     1535 2024-05-23 14:23:55.000000 apysc-4.4.2/apysc/_chart/axis_line_thickness_mixin.py
--rw-r--r--   0 runner    (1001) docker     (127)     1277 2024-05-23 14:23:55.000000 apysc-4.4.2/apysc/_chart/background_container_mixin.py
--rw-r--r--   0 runner    (1001) docker     (127)     1249 2024-05-23 14:23:55.000000 apysc-4.4.2/apysc/_chart/border_container_mixin.py
--rw-r--r--   0 runner    (1001) docker     (127)      118 2024-05-23 14:23:55.000000 apysc-4.4.2/apysc/_chart/chart_const.py
--rw-r--r--   0 runner    (1001) docker     (127)     1242 2024-05-23 14:23:55.000000 apysc-4.4.2/apysc/_chart/chart_container_mixin.py
--rw-r--r--   0 runner    (1001) docker     (127)    22705 2024-05-23 14:23:55.000000 apysc-4.4.2/apysc/_chart/create_single_column_y_axis_mixin.py
--rw-r--r--   0 runner    (1001) docker     (127)     2975 2024-05-23 14:23:55.000000 apysc-4.4.2/apysc/_chart/initialize_each_container_mixin.py
--rw-r--r--   0 runner    (1001) docker     (127)     1583 2024-05-23 14:23:55.000000 apysc-4.4.2/apysc/_chart/is_display_axis_label_mixin.py
--rw-r--r--   0 runner    (1001) docker     (127)      935 2024-05-23 14:23:55.000000 apysc-4.4.2/apysc/_chart/overall_container_mixin.py
--rw-r--r--   0 runner    (1001) docker     (127)     1649 2024-05-23 14:23:55.000000 apysc-4.4.2/apysc/_chart/set_initial_background_fill_alpha_mixin.py
--rw-r--r--   0 runner    (1001) docker     (127)      905 2024-05-23 14:23:55.000000 apysc-4.4.2/apysc/_chart/set_initial_background_fill_color_mixin.py
--rw-r--r--   0 runner    (1001) docker     (127)     1488 2024-05-23 14:23:55.000000 apysc-4.4.2/apysc/_chart/set_initial_border_alpha_mixin.py
--rw-r--r--   0 runner    (1001) docker     (127)      815 2024-05-23 14:23:55.000000 apysc-4.4.2/apysc/_chart/set_initial_border_color_mixin.py
--rw-r--r--   0 runner    (1001) docker     (127)     1521 2024-05-23 14:23:55.000000 apysc-4.4.2/apysc/_chart/set_initial_border_thickness_mixin.py
--rw-r--r--   0 runner    (1001) docker     (127)     1266 2024-05-23 14:23:55.000000 apysc-4.4.2/apysc/_chart/set_initial_height_mixin.py
--rw-r--r--   0 runner    (1001) docker     (127)     1502 2024-05-23 14:23:55.000000 apysc-4.4.2/apysc/_chart/set_initial_horizontal_padding_mixin.py
--rw-r--r--   0 runner    (1001) docker     (127)     3859 2024-05-23 14:23:55.000000 apysc-4.4.2/apysc/_chart/set_initial_matrix_data_mixin.py
--rw-r--r--   0 runner    (1001) docker     (127)     1236 2024-05-23 14:23:55.000000 apysc-4.4.2/apysc/_chart/set_initial_overall_container_coordinates_mixin.py
--rw-r--r--   0 runner    (1001) docker     (127)     1472 2024-05-23 14:23:55.000000 apysc-4.4.2/apysc/_chart/set_initial_vertical_padding_mixin.py
--rw-r--r--   0 runner    (1001) docker     (127)     1253 2024-05-23 14:23:55.000000 apysc-4.4.2/apysc/_chart/set_initial_width_mixin.py
--rw-r--r--   0 runner    (1001) docker     (127)     1238 2024-05-23 14:23:55.000000 apysc-4.4.2/apysc/_chart/set_initial_x_mixin.py
--rw-r--r--   0 runner    (1001) docker     (127)     1238 2024-05-23 14:23:55.000000 apysc-4.4.2/apysc/_chart/set_initial_y_mixin.py
--rw-r--r--   0 runner    (1001) docker     (127)     1461 2024-05-23 14:23:55.000000 apysc-4.4.2/apysc/_chart/tick_max_num_mixin.py
--rw-r--r--   0 runner    (1001) docker     (127)     1422 2024-05-23 14:23:55.000000 apysc-4.4.2/apysc/_chart/tick_text_bold_mixin.py
--rw-r--r--   0 runner    (1001) docker     (127)     1450 2024-05-23 14:23:55.000000 apysc-4.4.2/apysc/_chart/tick_text_fill_alpha_mixin.py
--rw-r--r--   0 runner    (1001) docker     (127)      866 2024-05-23 14:23:55.000000 apysc-4.4.2/apysc/_chart/tick_text_fill_color_mixin.py
--rw-r--r--   0 runner    (1001) docker     (127)     1879 2024-05-23 14:23:55.000000 apysc-4.4.2/apysc/_chart/tick_text_font_family_mixin.py
--rw-r--r--   0 runner    (1001) docker     (127)     1463 2024-05-23 14:23:55.000000 apysc-4.4.2/apysc/_chart/tick_text_font_size_mixin.py
--rw-r--r--   0 runner    (1001) docker     (127)     1481 2024-05-23 14:23:55.000000 apysc-4.4.2/apysc/_chart/tick_text_italic_mixin.py
--rw-r--r--   0 runner    (1001) docker     (127)     1634 2024-05-23 14:23:55.000000 apysc-4.4.2/apysc/_chart/tick_text_max_num_of_decimal_places_mixin.py
--rw-r--r--   0 runner    (1001) docker     (127)     9647 2024-05-23 14:23:55.000000 apysc-4.4.2/apysc/_chart/vertical_bar_chart.py
--rw-r--r--   0 runner    (1001) docker     (127)      793 2024-05-23 14:23:55.000000 apysc-4.4.2/apysc/_chart/x_axis_column_name_mixin.py
--rw-r--r--   0 runner    (1001) docker     (127)     1249 2024-05-23 14:23:55.000000 apysc-4.4.2/apysc/_chart/x_axis_container_mixin.py
--rw-r--r--   0 runner    (1001) docker     (127)      316 2024-05-23 14:23:55.000000 apysc-4.4.2/apysc/_chart/x_axis_label_position.py
--rw-r--r--   0 runner    (1001) docker     (127)      939 2024-05-23 14:23:55.000000 apysc-4.4.2/apysc/_chart/x_axis_label_position_mixin.py
--rw-r--r--   0 runner    (1001) docker     (127)    11482 2024-05-23 14:23:55.000000 apysc-4.4.2/apysc/_chart/x_axis_settings.py
--rw-r--r--   0 runner    (1001) docker     (127)     1023 2024-05-23 14:23:55.000000 apysc-4.4.2/apysc/_chart/y_axis_column_name_mixin.py
--rw-r--r--   0 runner    (1001) docker     (127)     1248 2024-05-23 14:23:55.000000 apysc-4.4.2/apysc/_chart/y_axis_container_mixin.py
--rw-r--r--   0 runner    (1001) docker     (127)      314 2024-05-23 14:23:55.000000 apysc-4.4.2/apysc/_chart/y_axis_label_position.py
--rw-r--r--   0 runner    (1001) docker     (127)      944 2024-05-23 14:23:55.000000 apysc-4.4.2/apysc/_chart/y_axis_label_position_mixin.py
--rw-r--r--   0 runner    (1001) docker     (127)    13296 2024-05-23 14:23:55.000000 apysc-4.4.2/apysc/_chart/y_axis_single_column_settings.py
--rw-r--r--   0 runner    (1001) docker     (127)     1398 2024-05-23 14:23:55.000000 apysc-4.4.2/apysc/_chart/y_max_mixin.py
--rw-r--r--   0 runner    (1001) docker     (127)     1398 2024-05-23 14:23:55.000000 apysc-4.4.2/apysc/_chart/y_min_mixin.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-23 14:24:13.294299 apysc-4.4.2/apysc/_color/
--rw-r--r--   0 runner    (1001) docker     (127)        0 2024-05-23 14:23:55.000000 apysc-4.4.2/apysc/_color/__init__.py
--rw-r--r--   0 runner    (1001) docker     (127)     4857 2024-05-23 14:23:55.000000 apysc-4.4.2/apysc/_color/blue_color_mixin.py
--rw-r--r--   0 runner    (1001) docker     (127)     6496 2024-05-23 14:23:55.000000 apysc-4.4.2/apysc/_color/color.py
--rw-r--r--   0 runner    (1001) docker     (127)     2473 2024-05-23 14:23:55.000000 apysc-4.4.2/apysc/_color/color_copy_mixin.py
--rw-r--r--   0 runner    (1001) docker     (127)     7843 2024-05-23 14:23:55.000000 apysc-4.4.2/apysc/_color/color_util.py
--rw-r--r--   0 runner    (1001) docker     (127)      477 2024-05-23 14:23:55.000000 apysc-4.4.2/apysc/_color/colorless.py
--rw-r--r--   0 runner    (1001) docker     (127)    84071 2024-05-23 14:23:55.000000 apysc-4.4.2/apysc/_color/colors.py
--rw-r--r--   0 runner    (1001) docker     (127)     1164 2024-05-23 14:23:55.000000 apysc-4.4.2/apysc/_color/copy_color_if_default_value_specified_mixin.py
--rw-r--r--   0 runner    (1001) docker     (127)     4056 2024-05-23 14:23:55.000000 apysc-4.4.2/apysc/_color/from_rgb_mixin.py
--rw-r--r--   0 runner    (1001) docker     (127)      924 2024-05-23 14:23:55.000000 apysc-4.4.2/apysc/_color/get_colors_members_mixin.py
--rw-r--r--   0 runner    (1001) docker     (127)     5114 2024-05-23 14:23:55.000000 apysc-4.4.2/apysc/_color/green_color_mixin.py
--rw-r--r--   0 runner    (1001) docker     (127)     4249 2024-05-23 14:23:55.000000 apysc-4.4.2/apysc/_color/red_color_mixin.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-23 14:24:13.294299 apysc-4.4.2/apysc/_console/
--rw-r--r--   0 runner    (1001) docker     (127)        0 2024-05-23 14:23:55.000000 apysc-4.4.2/apysc/_console/__init__.py
--rw-r--r--   0 runner    (1001) docker     (127)     4573 2024-05-23 14:23:55.000000 apysc-4.4.2/apysc/_console/_trace.py
--rw-r--r--   0 runner    (1001) docker     (127)    32116 2024-05-23 14:23:55.000000 apysc-4.4.2/apysc/_console/assertion.py
--rw-r--r--   0 runner    (1001) docker     (127)     1004 2024-05-23 14:23:55.000000 apysc-4.4.2/apysc/_console/loggers.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-23 14:24:13.294299 apysc-4.4.2/apysc/_converter/
--rw-r--r--   0 runner    (1001) docker     (127)        0 2024-05-23 14:23:55.000000 apysc-4.4.2/apysc/_converter/__init__.py
--rw-r--r--   0 runner    (1001) docker     (127)     2458 2024-05-23 14:23:55.000000 apysc-4.4.2/apysc/_converter/cast.py
--rw-r--r--   0 runner    (1001) docker     (127)     3431 2024-05-23 14:23:55.000000 apysc-4.4.2/apysc/_converter/to_apysc_val_from_builtin.py
--rw-r--r--   0 runner    (1001) docker     (127)      698 2024-05-23 14:23:55.000000 apysc-4.4.2/apysc/_converter/to_builtin_val_from_apysc.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-23 14:24:13.314299 apysc-4.4.2/apysc/_display/
--rw-r--r--   0 runner    (1001) docker     (127)        0 2024-05-23 14:23:55.000000 apysc-4.4.2/apysc/_display/__init__.py
--rw-r--r--   0 runner    (1001) docker     (127)      523 2024-05-23 14:23:55.000000 apysc-4.4.2/apysc/_display/_document.py
--rw-r--r--   0 runner    (1001) docker     (127)     1218 2024-05-23 14:23:55.000000 apysc-4.4.2/apysc/_display/add_foreign_object_child_mixin.py
--rw-r--r--   0 runner    (1001) docker     (127)     1238 2024-05-23 14:23:55.000000 apysc-4.4.2/apysc/_display/add_to_parent_mixin.py
--rw-r--r--   0 runner    (1001) docker     (127)     2142 2024-05-23 14:23:55.000000 apysc-4.4.2/apysc/_display/any_display_object.py
--rw-r--r--   0 runner    (1001) docker     (127)     1787 2024-05-23 14:23:55.000000 apysc-4.4.2/apysc/_display/append_fill_alpha_attr_expression_mixin.py
--rw-r--r--   0 runner    (1001) docker     (127)     1768 2024-05-23 14:23:55.000000 apysc-4.4.2/apysc/_display/append_fill_color_expression_mixin.py
--rw-r--r--   0 runner    (1001) docker     (127)     1224 2024-05-23 14:23:55.000000 apysc-4.4.2/apysc/_display/append_foreign_object_constructor_expression_mixin.py
--rw-r--r--   0 runner    (1001) docker     (127)     1778 2024-05-23 14:23:55.000000 apysc-4.4.2/apysc/_display/append_line_alpha_attr_expression_mixin.py
--rw-r--r--   0 runner    (1001) docker     (127)     1725 2024-05-23 14:23:55.000000 apysc-4.4.2/apysc/_display/append_line_cap_attr_expression_mixin.py
--rw-r--r--   0 runner    (1001) docker     (127)     1772 2024-05-23 14:23:55.000000 apysc-4.4.2/apysc/_display/append_line_color_attr_expression_mixin.py
--rw-r--r--   0 runner    (1001) docker     (127)     1791 2024-05-23 14:23:55.000000 apysc-4.4.2/apysc/_display/append_line_joints_attr_expression_mixin.py
--rw-r--r--   0 runner    (1001) docker     (127)     3056 2024-05-23 14:23:55.000000 apysc-4.4.2/apysc/_display/append_line_point_mixin.py
--rw-r--r--   0 runner    (1001) docker     (127)     1824 2024-05-23 14:23:55.000000 apysc-4.4.2/apysc/_display/append_line_thickness_attr_expression_mixin.py
--rw-r--r--   0 runner    (1001) docker     (127)     1657 2024-05-23 14:23:55.000000 apysc-4.4.2/apysc/_display/append_x_attr_expression_mixin.py
--rw-r--r--   0 runner    (1001) docker     (127)     1655 2024-05-23 14:23:55.000000 apysc-4.4.2/apysc/_display/append_y_attr_expression_mixin.py
--rw-r--r--   0 runner    (1001) docker     (127)     7031 2024-05-23 14:23:55.000000 apysc-4.4.2/apysc/_display/begin_fill_mixin.py
--rw-r--r--   0 runner    (1001) docker     (127)    15676 2024-05-23 14:23:55.000000 apysc-4.4.2/apysc/_display/child_mixin.py
--rw-r--r--   0 runner    (1001) docker     (127)    17462 2024-05-23 14:23:55.000000 apysc-4.4.2/apysc/_display/circle.py
--rw-r--r--   0 runner    (1001) docker     (127)     1295 2024-05-23 14:23:55.000000 apysc-4.4.2/apysc/_display/css_interface.py
--rw-r--r--   0 runner    (1001) docker     (127)     6651 2024-05-23 14:23:55.000000 apysc-4.4.2/apysc/_display/css_mixin.py
--rw-r--r--   0 runner    (1001) docker     (127)      415 2024-05-23 14:23:55.000000 apysc-4.4.2/apysc/_display/css_text_align.py
--rw-r--r--   0 runner    (1001) docker     (127)      379 2024-05-23 14:23:55.000000 apysc-4.4.2/apysc/_display/css_text_align_last.py
--rw-r--r--   0 runner    (1001) docker     (127)     5404 2024-05-23 14:23:55.000000 apysc-4.4.2/apysc/_display/cx_mixin.py
--rw-r--r--   0 runner    (1001) docker     (127)     5454 2024-05-23 14:23:55.000000 apysc-4.4.2/apysc/_display/cy_mixin.py
--rw-r--r--   0 runner    (1001) docker     (127)     1511 2024-05-23 14:23:55.000000 apysc-4.4.2/apysc/_display/display_object.py
--rw-r--r--   0 runner    (1001) docker     (127)    17384 2024-05-23 14:23:55.000000 apysc-4.4.2/apysc/_display/ellipse.py
--rw-r--r--   0 runner    (1001) docker     (127)     5438 2024-05-23 14:23:55.000000 apysc-4.4.2/apysc/_display/ellipse_height_mixin.py
--rw-r--r--   0 runner    (1001) docker     (127)     5411 2024-05-23 14:23:55.000000 apysc-4.4.2/apysc/_display/ellipse_width_mixin.py
--rw-r--r--   0 runner    (1001) docker     (127)     6246 2024-05-23 14:23:55.000000 apysc-4.4.2/apysc/_display/fill_alpha_mixin.py
--rw-r--r--   0 runner    (1001) docker     (127)     6544 2024-05-23 14:23:55.000000 apysc-4.4.2/apysc/_display/fill_color_mixin.py
--rw-r--r--   0 runner    (1001) docker     (127)     2321 2024-05-23 14:23:55.000000 apysc-4.4.2/apysc/_display/fixed_html_svg_icon_base.py
--rw-r--r--   0 runner    (1001) docker     (127)     1354 2024-05-23 14:23:55.000000 apysc-4.4.2/apysc/_display/flip_interface_helper.py
--rw-r--r--   0 runner    (1001) docker     (127)     5692 2024-05-23 14:23:55.000000 apysc-4.4.2/apysc/_display/flip_x_mixin.py
--rw-r--r--   0 runner    (1001) docker     (127)     5690 2024-05-23 14:23:55.000000 apysc-4.4.2/apysc/_display/flip_y_mixin.py
--rw-r--r--   0 runner    (1001) docker     (127)     5452 2024-05-23 14:23:55.000000 apysc-4.4.2/apysc/_display/get_bounds_mixin.py
--rw-r--r--   0 runner    (1001) docker     (127)    49066 2024-05-23 14:23:55.000000 apysc-4.4.2/apysc/_display/graphics.py
--rw-r--r--   0 runner    (1001) docker     (127)     7012 2024-05-23 14:23:55.000000 apysc-4.4.2/apysc/_display/graphics_base.py
--rw-r--r--   0 runner    (1001) docker     (127)     4265 2024-05-23 14:23:55.000000 apysc-4.4.2/apysc/_display/graphics_clear_mixin.py
--rw-r--r--   0 runner    (1001) docker     (127)     7731 2024-05-23 14:23:55.000000 apysc-4.4.2/apysc/_display/graphics_expression.py
--rw-r--r--   0 runner    (1001) docker     (127)     5533 2024-05-23 14:23:55.000000 apysc-4.4.2/apysc/_display/height_mixin.py
--rw-r--r--   0 runner    (1001) docker     (127)    15906 2024-05-23 14:23:55.000000 apysc-4.4.2/apysc/_display/line.py
--rw-r--r--   0 runner    (1001) docker     (127)     6178 2024-05-23 14:23:55.000000 apysc-4.4.2/apysc/_display/line_alpha_mixin.py
--rw-r--r--   0 runner    (1001) docker     (127)     4752 2024-05-23 14:23:55.000000 apysc-4.4.2/apysc/_display/line_cap_mixin.py
--rw-r--r--   0 runner    (1001) docker     (127)      597 2024-05-23 14:23:55.000000 apysc-4.4.2/apysc/_display/line_caps.py
--rw-r--r--   0 runner    (1001) docker     (127)     6753 2024-05-23 14:23:55.000000 apysc-4.4.2/apysc/_display/line_color_mixin.py
--rw-r--r--   0 runner    (1001) docker     (127)     7036 2024-05-23 14:23:55.000000 apysc-4.4.2/apysc/_display/line_dash_dot_setting.py
--rw-r--r--   0 runner    (1001) docker     (127)     6757 2024-05-23 14:23:55.000000 apysc-4.4.2/apysc/_display/line_dash_dot_setting_mixin.py
--rw-r--r--   0 runner    (1001) docker     (127)     5383 2024-05-23 14:23:55.000000 apysc-4.4.2/apysc/_display/line_dash_setting.py
--rw-r--r--   0 runner    (1001) docker     (127)     6059 2024-05-23 14:23:55.000000 apysc-4.4.2/apysc/_display/line_dash_setting_mixin.py
--rw-r--r--   0 runner    (1001) docker     (127)     3855 2024-05-23 14:23:55.000000 apysc-4.4.2/apysc/_display/line_dot_setting.py
--rw-r--r--   0 runner    (1001) docker     (127)     5722 2024-05-23 14:23:55.000000 apysc-4.4.2/apysc/_display/line_dot_setting_mixin.py
--rw-r--r--   0 runner    (1001) docker     (127)      618 2024-05-23 14:23:55.000000 apysc-4.4.2/apysc/_display/line_joints.py
--rw-r--r--   0 runner    (1001) docker     (127)     5226 2024-05-23 14:23:55.000000 apysc-4.4.2/apysc/_display/line_joints_mixin.py
--rw-r--r--   0 runner    (1001) docker     (127)     5652 2024-05-23 14:23:55.000000 apysc-4.4.2/apysc/_display/line_round_dot_setting.py
--rw-r--r--   0 runner    (1001) docker     (127)     6639 2024-05-23 14:23:55.000000 apysc-4.4.2/apysc/_display/line_round_dot_setting_mixin.py
--rw-r--r--   0 runner    (1001) docker     (127)    26709 2024-05-23 14:23:55.000000 apysc-4.4.2/apysc/_display/line_style_mixin.py
--rw-r--r--   0 runner    (1001) docker     (127)     6187 2024-05-23 14:23:55.000000 apysc-4.4.2/apysc/_display/line_thickness_mixin.py
--rw-r--r--   0 runner    (1001) docker     (127)    12333 2024-05-23 14:23:55.000000 apysc-4.4.2/apysc/_display/multi_line_text.py
--rw-r--r--   0 runner    (1001) docker     (127)     3736 2024-05-23 14:23:55.000000 apysc-4.4.2/apysc/_display/opacity_css_mixin.py
--rw-r--r--   0 runner    (1001) docker     (127)     4338 2024-05-23 14:23:55.000000 apysc-4.4.2/apysc/_display/parent_mixin.py
--rw-r--r--   0 runner    (1001) docker     (127)    18730 2024-05-23 14:23:55.000000 apysc-4.4.2/apysc/_display/path.py
--rw-r--r--   0 runner    (1001) docker     (127)     5865 2024-05-23 14:23:55.000000 apysc-4.4.2/apysc/_display/points_2d_mixin.py
--rw-r--r--   0 runner    (1001) docker     (127)       54 2024-05-23 14:23:55.000000 apysc-4.4.2/apysc/_display/points_var_name_mixin.py
--rw-r--r--   0 runner    (1001) docker     (127)    15565 2024-05-23 14:23:55.000000 apysc-4.4.2/apysc/_display/polygon.py
--rw-r--r--   0 runner    (1001) docker     (127)     4334 2024-05-23 14:23:55.000000 apysc-4.4.2/apysc/_display/polygon_append_constructor_expression_mixin.py
--rw-r--r--   0 runner    (1001) docker     (127)      747 2024-05-23 14:23:55.000000 apysc-4.4.2/apysc/_display/polygon_apply_current_points_mixin.py
--rw-r--r--   0 runner    (1001) docker     (127)     1177 2024-05-23 14:23:55.000000 apysc-4.4.2/apysc/_display/polygon_x1_mixin.py
--rw-r--r--   0 runner    (1001) docker     (127)     1180 2024-05-23 14:23:55.000000 apysc-4.4.2/apysc/_display/polygon_x2_mixin.py
--rw-r--r--   0 runner    (1001) docker     (127)     1177 2024-05-23 14:23:55.000000 apysc-4.4.2/apysc/_display/polygon_x3_mixin.py
--rw-r--r--   0 runner    (1001) docker     (127)     1177 2024-05-23 14:23:55.000000 apysc-4.4.2/apysc/_display/polygon_y1_mixin.py
--rw-r--r--   0 runner    (1001) docker     (127)     1180 2024-05-23 14:23:55.000000 apysc-4.4.2/apysc/_display/polygon_y2_mixin.py
--rw-r--r--   0 runner    (1001) docker     (127)     1126 2024-05-23 14:23:55.000000 apysc-4.4.2/apysc/_display/polygon_y3_mixin.py
--rw-r--r--   0 runner    (1001) docker     (127)    17466 2024-05-23 14:23:55.000000 apysc-4.4.2/apysc/_display/polyline.py
--rw-r--r--   0 runner    (1001) docker     (127)     5272 2024-05-23 14:23:55.000000 apysc-4.4.2/apysc/_display/radius_mixin.py
--rw-r--r--   0 runner    (1001) docker     (127)    19494 2024-05-23 14:23:55.000000 apysc-4.4.2/apysc/_display/rectangle.py
--rw-r--r--   0 runner    (1001) docker     (127)     6400 2024-05-23 14:23:55.000000 apysc-4.4.2/apysc/_display/rotation_around_center_mixin.py
--rw-r--r--   0 runner    (1001) docker     (127)     9157 2024-05-23 14:23:55.000000 apysc-4.4.2/apysc/_display/rotation_around_point_mixin.py
--rw-r--r--   0 runner    (1001) docker     (127)     1108 2024-05-23 14:23:55.000000 apysc-4.4.2/apysc/_display/rotation_interface_helper.py
--rw-r--r--   0 runner    (1001) docker     (127)     3799 2024-05-23 14:23:55.000000 apysc-4.4.2/apysc/_display/scale_interface_helper.py
--rw-r--r--   0 runner    (1001) docker     (127)     6769 2024-05-23 14:23:55.000000 apysc-4.4.2/apysc/_display/scale_x_from_center_mixin.py
--rw-r--r--   0 runner    (1001) docker     (127)     7293 2024-05-23 14:23:55.000000 apysc-4.4.2/apysc/_display/scale_x_from_point_mixin.py
--rw-r--r--   0 runner    (1001) docker     (127)     6764 2024-05-23 14:23:55.000000 apysc-4.4.2/apysc/_display/scale_y_from_center_mixin.py
--rw-r--r--   0 runner    (1001) docker     (127)     6988 2024-05-23 14:23:55.000000 apysc-4.4.2/apysc/_display/scale_y_from_point_mixin.py
--rw-r--r--   0 runner    (1001) docker     (127)      650 2024-05-23 14:23:55.000000 apysc-4.4.2/apysc/_display/set_lower_scale_limit_mixin.py
--rw-r--r--   0 runner    (1001) docker     (127)      563 2024-05-23 14:23:55.000000 apysc-4.4.2/apysc/_display/set_overflow_visible_setting_mixin.py
--rw-r--r--   0 runner    (1001) docker     (127)      390 2024-05-23 14:23:55.000000 apysc-4.4.2/apysc/_display/set_x_and_y_with_minimum_point_interface_base.py
--rw-r--r--   0 runner    (1001) docker     (127)     5479 2024-05-23 14:23:55.000000 apysc-4.4.2/apysc/_display/skew_x_mixin.py
--rw-r--r--   0 runner    (1001) docker     (127)     5478 2024-05-23 14:23:55.000000 apysc-4.4.2/apysc/_display/skew_y_mixin.py
--rw-r--r--   0 runner    (1001) docker     (127)     7453 2024-05-23 14:23:55.000000 apysc-4.4.2/apysc/_display/sprite.py
--rw-r--r--   0 runner    (1001) docker     (127)    12655 2024-05-23 14:23:55.000000 apysc-4.4.2/apysc/_display/stage.py
--rw-r--r--   0 runner    (1001) docker     (127)     3721 2024-05-23 14:23:55.000000 apysc-4.4.2/apysc/_display/svg_foreign_object_child.py
--rw-r--r--   0 runner    (1001) docker     (127)     1447 2024-05-23 14:23:55.000000 apysc-4.4.2/apysc/_display/svg_foreign_object_child_mixin.py
--rw-r--r--   0 runner    (1001) docker     (127)     1249 2024-05-23 14:23:55.000000 apysc-4.4.2/apysc/_display/svg_foreign_object_initialize_width_mixin.py
--rw-r--r--   0 runner    (1001) docker     (127)     1478 2024-05-23 14:23:55.000000 apysc-4.4.2/apysc/_display/svg_foreign_object_text_mixin.py
--rw-r--r--   0 runner    (1001) docker     (127)     5737 2024-05-23 14:23:55.000000 apysc-4.4.2/apysc/_display/svg_icon.py
--rw-r--r--   0 runner    (1001) docker     (127)    23384 2024-05-23 14:23:55.000000 apysc-4.4.2/apysc/_display/svg_text.py
--rw-r--r--   0 runner    (1001) docker     (127)     2705 2024-05-23 14:23:55.000000 apysc-4.4.2/apysc/_display/svg_text_align_mixin.py
--rw-r--r--   0 runner    (1001) docker     (127)     2980 2024-05-23 14:23:55.000000 apysc-4.4.2/apysc/_display/svg_text_bold_mixin.py
--rw-r--r--   0 runner    (1001) docker     (127)     2993 2024-05-23 14:23:55.000000 apysc-4.4.2/apysc/_display/svg_text_delta_x_mixin.py
--rw-r--r--   0 runner    (1001) docker     (127)     2993 2024-05-23 14:23:55.000000 apysc-4.4.2/apysc/_display/svg_text_delta_y_mixin.py
--rw-r--r--   0 runner    (1001) docker     (127)     2873 2024-05-23 14:23:55.000000 apysc-4.4.2/apysc/_display/svg_text_font_family_mixin.py
--rw-r--r--   0 runner    (1001) docker     (127)     3378 2024-05-23 14:23:55.000000 apysc-4.4.2/apysc/_display/svg_text_font_size_mixin.py
--rw-r--r--   0 runner    (1001) docker     (127)     3008 2024-05-23 14:23:55.000000 apysc-4.4.2/apysc/_display/svg_text_italic_mixin.py
--rw-r--r--   0 runner    (1001) docker     (127)     2916 2024-05-23 14:23:55.000000 apysc-4.4.2/apysc/_display/svg_text_leading_mixin.py
--rw-r--r--   0 runner    (1001) docker     (127)      907 2024-05-23 14:23:55.000000 apysc-4.4.2/apysc/_display/svg_text_set_align_mixin.py
--rw-r--r--   0 runner    (1001) docker     (127)     1555 2024-05-23 14:23:55.000000 apysc-4.4.2/apysc/_display/svg_text_set_bold_mixin.py
--rw-r--r--   0 runner    (1001) docker     (127)     1372 2024-05-23 14:23:55.000000 apysc-4.4.2/apysc/_display/svg_text_set_delta_x_mixin.py
--rw-r--r--   0 runner    (1001) docker     (127)     1372 2024-05-23 14:23:55.000000 apysc-4.4.2/apysc/_display/svg_text_set_delta_y_mixin.py
--rw-r--r--   0 runner    (1001) docker     (127)     1747 2024-05-23 14:23:55.000000 apysc-4.4.2/apysc/_display/svg_text_set_font_family_mixin.py
--rw-r--r--   0 runner    (1001) docker     (127)     1574 2024-05-23 14:23:55.000000 apysc-4.4.2/apysc/_display/svg_text_set_font_size_value_mixin.py
--rw-r--r--   0 runner    (1001) docker     (127)     1634 2024-05-23 14:23:55.000000 apysc-4.4.2/apysc/_display/svg_text_set_italic_mixin.py
--rw-r--r--   0 runner    (1001) docker     (127)     1404 2024-05-23 14:23:55.000000 apysc-4.4.2/apysc/_display/svg_text_set_leading_mixin.py
--rw-r--r--   0 runner    (1001) docker     (127)     1486 2024-05-23 14:23:55.000000 apysc-4.4.2/apysc/_display/svg_text_set_text_value_mixin.py
--rw-r--r--   0 runner    (1001) docker     (127)     1108 2024-05-23 14:23:55.000000 apysc-4.4.2/apysc/_display/svg_text_singleton_for_text_span.py
--rw-r--r--   0 runner    (1001) docker     (127)     1062 2024-05-23 14:23:55.000000 apysc-4.4.2/apysc/_display/svg_text_skip_fill_alpha_exp_appending_mixin.py
--rw-r--r--   0 runner    (1001) docker     (127)     1005 2024-05-23 14:23:55.000000 apysc-4.4.2/apysc/_display/svg_text_skip_fill_color_exp_appending_mixin.py
--rw-r--r--   0 runner    (1001) docker     (127)     1062 2024-05-23 14:23:55.000000 apysc-4.4.2/apysc/_display/svg_text_skip_line_alpha_exp_appending_mixin.py
--rw-r--r--   0 runner    (1001) docker     (127)     1005 2024-05-23 14:23:55.000000 apysc-4.4.2/apysc/_display/svg_text_skip_line_color_exp_appending_mixin.py
--rw-r--r--   0 runner    (1001) docker     (127)     1090 2024-05-23 14:23:55.000000 apysc-4.4.2/apysc/_display/svg_text_skip_line_thickness_exp_appending_mixin.py
--rw-r--r--   0 runner    (1001) docker     (127)    16986 2024-05-23 14:23:55.000000 apysc-4.4.2/apysc/_display/svg_text_span.py
--rw-r--r--   0 runner    (1001) docker     (127)     3564 2024-05-23 14:23:55.000000 apysc-4.4.2/apysc/_display/svg_text_text_mixin.py
--rw-r--r--   0 runner    (1001) docker     (127)     3222 2024-05-23 14:23:55.000000 apysc-4.4.2/apysc/_display/text_align_css_mixin.py
--rw-r--r--   0 runner    (1001) docker     (127)     3493 2024-05-23 14:23:55.000000 apysc-4.4.2/apysc/_display/text_align_last_css_mixin.py
--rw-r--r--   0 runner    (1001) docker     (127)     3885 2024-05-23 14:23:55.000000 apysc-4.4.2/apysc/_display/text_bold_css_mixin.py
--rw-r--r--   0 runner    (1001) docker     (127)     3951 2024-05-23 14:23:55.000000 apysc-4.4.2/apysc/_display/text_decoration_underline_css_mixin.py
--rw-r--r--   0 runner    (1001) docker     (127)     3905 2024-05-23 14:23:55.000000 apysc-4.4.2/apysc/_display/text_fill_color_css_mixin.py
--rw-r--r--   0 runner    (1001) docker     (127)     3463 2024-05-23 14:23:55.000000 apysc-4.4.2/apysc/_display/text_font_size_css_mixin.py
--rw-r--r--   0 runner    (1001) docker     (127)     4005 2024-05-23 14:23:55.000000 apysc-4.4.2/apysc/_display/text_italic_css_mixin.py
--rw-r--r--   0 runner    (1001) docker     (127)     3638 2024-05-23 14:23:55.000000 apysc-4.4.2/apysc/_display/text_line_height_css_mixin.py
--rw-r--r--   0 runner    (1001) docker     (127)    17673 2024-05-23 14:23:55.000000 apysc-4.4.2/apysc/_display/triangle.py
--rw-r--r--   0 runner    (1001) docker     (127)     4763 2024-05-23 14:23:55.000000 apysc-4.4.2/apysc/_display/visible_mixin.py
--rw-r--r--   0 runner    (1001) docker     (127)     8204 2024-05-23 14:23:55.000000 apysc-4.4.2/apysc/_display/width_and_height_mixin_for_ellipse.py
--rw-r--r--   0 runner    (1001) docker     (127)     5453 2024-05-23 14:23:55.000000 apysc-4.4.2/apysc/_display/width_mixin.py
--rw-r--r--   0 runner    (1001) docker     (127)     1083 2024-05-23 14:23:55.000000 apysc-4.4.2/apysc/_display/x_interface.py
--rw-r--r--   0 runner    (1001) docker     (127)     5661 2024-05-23 14:23:55.000000 apysc-4.4.2/apysc/_display/x_mixin.py
--rw-r--r--   0 runner    (1001) docker     (127)     1081 2024-05-23 14:23:55.000000 apysc-4.4.2/apysc/_display/y_interface.py
--rw-r--r--   0 runner    (1001) docker     (127)     5652 2024-05-23 14:23:55.000000 apysc-4.4.2/apysc/_display/y_mixin.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-23 14:24:13.314299 apysc-4.4.2/apysc/_event/
--rw-r--r--   0 runner    (1001) docker     (127)        0 2024-05-23 14:23:55.000000 apysc-4.4.2/apysc/_event/__init__.py
--rw-r--r--   0 runner    (1001) docker     (127)     3255 2024-05-23 14:23:55.000000 apysc-4.4.2/apysc/_event/animation_event.py
--rw-r--r--   0 runner    (1001) docker     (127)     6521 2024-05-23 14:23:55.000000 apysc-4.4.2/apysc/_event/click_mixin.py
--rw-r--r--   0 runner    (1001) docker     (127)    14746 2024-05-23 14:23:55.000000 apysc-4.4.2/apysc/_event/custom_event_mixin.py
--rw-r--r--   0 runner    (1001) docker     (127)      217 2024-05-23 14:23:55.000000 apysc-4.4.2/apysc/_event/custom_event_type.py
--rw-r--r--   0 runner    (1001) docker     (127)     3394 2024-05-23 14:23:55.000000 apysc-4.4.2/apysc/_event/document_mouse_wheel_func.py
--rw-r--r--   0 runner    (1001) docker     (127)     6450 2024-05-23 14:23:55.000000 apysc-4.4.2/apysc/_event/double_click_mixin.py
--rw-r--r--   0 runner    (1001) docker     (127)     1099 2024-05-23 14:23:55.000000 apysc-4.4.2/apysc/_event/enter_frame_event.py
--rw-r--r--   0 runner    (1001) docker     (127)    15687 2024-05-23 14:23:55.000000 apysc-4.4.2/apysc/_event/enter_frame_mixin.py
--rw-r--r--   0 runner    (1001) docker     (127)     5617 2024-05-23 14:23:55.000000 apysc-4.4.2/apysc/_event/event.py
--rw-r--r--   0 runner    (1001) docker     (127)     6331 2024-05-23 14:23:55.000000 apysc-4.4.2/apysc/_event/handler.py
--rw-r--r--   0 runner    (1001) docker     (127)     9989 2024-05-23 14:23:55.000000 apysc-4.4.2/apysc/_event/handler_circular_calling_util.py
--rw-r--r--   0 runner    (1001) docker     (127)     6870 2024-05-23 14:23:55.000000 apysc-4.4.2/apysc/_event/mouse_down_mixin.py
--rw-r--r--   0 runner    (1001) docker     (127)    10068 2024-05-23 14:23:55.000000 apysc-4.4.2/apysc/_event/mouse_event.py
--rw-r--r--   0 runner    (1001) docker     (127)     1284 2024-05-23 14:23:55.000000 apysc-4.4.2/apysc/_event/mouse_event_binding_expression_mixin.py
--rw-r--r--   0 runner    (1001) docker     (127)      744 2024-05-23 14:23:55.000000 apysc-4.4.2/apysc/_event/mouse_event_mixins.py
--rw-r--r--   0 runner    (1001) docker     (127)      371 2024-05-23 14:23:55.000000 apysc-4.4.2/apysc/_event/mouse_event_type.py
--rw-r--r--   0 runner    (1001) docker     (127)     2964 2024-05-23 14:23:55.000000 apysc-4.4.2/apysc/_event/mouse_event_unbinding_mixin.py
--rw-r--r--   0 runner    (1001) docker     (127)     7056 2024-05-23 14:23:55.000000 apysc-4.4.2/apysc/_event/mouse_move_mixin.py
--rw-r--r--   0 runner    (1001) docker     (127)     6824 2024-05-23 14:23:55.000000 apysc-4.4.2/apysc/_event/mouse_out_mixin.py
--rw-r--r--   0 runner    (1001) docker     (127)     6852 2024-05-23 14:23:55.000000 apysc-4.4.2/apysc/_event/mouse_over_mixin.py
--rw-r--r--   0 runner    (1001) docker     (127)     6782 2024-05-23 14:23:55.000000 apysc-4.4.2/apysc/_event/mouse_up_mixin.py
--rw-r--r--   0 runner    (1001) docker     (127)     1550 2024-05-23 14:23:55.000000 apysc-4.4.2/apysc/_event/prevent_default_mixin.py
--rw-r--r--   0 runner    (1001) docker     (127)     1826 2024-05-23 14:23:55.000000 apysc-4.4.2/apysc/_event/set_handler_data_mixin.py
--rw-r--r--   0 runner    (1001) docker     (127)     1453 2024-05-23 14:23:55.000000 apysc-4.4.2/apysc/_event/stop_propagation_mixin.py
--rw-r--r--   0 runner    (1001) docker     (127)     4218 2024-05-23 14:23:55.000000 apysc-4.4.2/apysc/_event/timer_event.py
--rw-r--r--   0 runner    (1001) docker     (127)     2853 2024-05-23 14:23:55.000000 apysc-4.4.2/apysc/_event/wheel_event.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-23 14:24:13.318299 apysc-4.4.2/apysc/_expression/
--rw-r--r--   0 runner    (1001) docker     (127)        0 2024-05-23 14:23:55.000000 apysc-4.4.2/apysc/_expression/__init__.py
--rw-r--r--   0 runner    (1001) docker     (127)     6871 2024-05-23 14:23:55.000000 apysc-4.4.2/apysc/_expression/event_handler_scope.py
--rw-r--r--   0 runner    (1001) docker     (127)    17851 2024-05-23 14:23:55.000000 apysc-4.4.2/apysc/_expression/expression_data_util.py
--rw-r--r--   0 runner    (1001) docker     (127)     4794 2024-05-23 14:23:55.000000 apysc-4.4.2/apysc/_expression/expression_variables_util.py
--rw-r--r--   0 runner    (1001) docker     (127)      358 2024-05-23 14:23:55.000000 apysc-4.4.2/apysc/_expression/get_last_scope_interface.py
--rw-r--r--   0 runner    (1001) docker     (127)     3812 2024-05-23 14:23:55.000000 apysc-4.4.2/apysc/_expression/indent_num.py
--rw-r--r--   0 runner    (1001) docker     (127)     1996 2024-05-23 14:23:55.000000 apysc-4.4.2/apysc/_expression/js_functions.py
--rw-r--r--   0 runner    (1001) docker     (127)     1936 2024-05-23 14:23:55.000000 apysc-4.4.2/apysc/_expression/last_scope.py
--rw-r--r--   0 runner    (1001) docker     (127)     2590 2024-05-23 14:23:55.000000 apysc-4.4.2/apysc/_expression/var_names.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-23 14:24:13.318299 apysc-4.4.2/apysc/_file/
--rw-r--r--   0 runner    (1001) docker     (127)        0 2024-05-23 14:23:55.000000 apysc-4.4.2/apysc/_file/__init__.py
--rw-r--r--   0 runner    (1001) docker     (127)     8021 2024-05-23 14:23:55.000000 apysc-4.4.2/apysc/_file/file_util.py
--rw-r--r--   0 runner    (1001) docker     (127)     4475 2024-05-23 14:23:55.000000 apysc-4.4.2/apysc/_file/module_util.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-23 14:24:13.322299 apysc-4.4.2/apysc/_geom/
--rw-r--r--   0 runner    (1001) docker     (127)        0 2024-05-23 14:23:55.000000 apysc-4.4.2/apysc/_geom/__init__.py
--rw-r--r--   0 runner    (1001) docker     (127)    10201 2024-05-23 14:23:55.000000 apysc-4.4.2/apysc/_geom/path_bezier_2d.py
--rw-r--r--   0 runner    (1001) docker     (127)     7960 2024-05-23 14:23:55.000000 apysc-4.4.2/apysc/_geom/path_bezier_2d_continual.py
--rw-r--r--   0 runner    (1001) docker     (127)    13379 2024-05-23 14:23:55.000000 apysc-4.4.2/apysc/_geom/path_bezier_3d.py
--rw-r--r--   0 runner    (1001) docker     (127)    11011 2024-05-23 14:23:55.000000 apysc-4.4.2/apysc/_geom/path_bezier_3d_continual.py
--rw-r--r--   0 runner    (1001) docker     (127)     2928 2024-05-23 14:23:55.000000 apysc-4.4.2/apysc/_geom/path_close.py
--rw-r--r--   0 runner    (1001) docker     (127)     4294 2024-05-23 14:23:55.000000 apysc-4.4.2/apysc/_geom/path_control_x1_mixin.py
--rw-r--r--   0 runner    (1001) docker     (127)     4298 2024-05-23 14:23:55.000000 apysc-4.4.2/apysc/_geom/path_control_x2_mixin.py
--rw-r--r--   0 runner    (1001) docker     (127)     4018 2024-05-23 14:23:55.000000 apysc-4.4.2/apysc/_geom/path_control_x_mixin.py
--rw-r--r--   0 runner    (1001) docker     (127)     4285 2024-05-23 14:23:55.000000 apysc-4.4.2/apysc/_geom/path_control_y1_mixin.py
--rw-r--r--   0 runner    (1001) docker     (127)     4293 2024-05-23 14:23:55.000000 apysc-4.4.2/apysc/_geom/path_control_y2_mixin.py
--rw-r--r--   0 runner    (1001) docker     (127)     4080 2024-05-23 14:23:55.000000 apysc-4.4.2/apysc/_geom/path_control_y_mixin.py
--rw-r--r--   0 runner    (1001) docker     (127)      972 2024-05-23 14:23:55.000000 apysc-4.4.2/apysc/_geom/path_data.py
--rw-r--r--   0 runner    (1001) docker     (127)     2572 2024-05-23 14:23:55.000000 apysc-4.4.2/apysc/_geom/path_data_base.py
--rw-r--r--   0 runner    (1001) docker     (127)      874 2024-05-23 14:23:55.000000 apysc-4.4.2/apysc/_geom/path_data_util.py
--rw-r--r--   0 runner    (1001) docker     (127)     3984 2024-05-23 14:23:55.000000 apysc-4.4.2/apysc/_geom/path_dest_x_mixin.py
--rw-r--r--   0 runner    (1001) docker     (127)     3968 2024-05-23 14:23:55.000000 apysc-4.4.2/apysc/_geom/path_dest_y_mixin.py
--rw-r--r--   0 runner    (1001) docker     (127)     6540 2024-05-23 14:23:55.000000 apysc-4.4.2/apysc/_geom/path_horizontal.py
--rw-r--r--   0 runner    (1001) docker     (127)      366 2024-05-23 14:23:55.000000 apysc-4.4.2/apysc/_geom/path_label.py
--rw-r--r--   0 runner    (1001) docker     (127)     7385 2024-05-23 14:23:55.000000 apysc-4.4.2/apysc/_geom/path_line_to.py
--rw-r--r--   0 runner    (1001) docker     (127)     7161 2024-05-23 14:23:55.000000 apysc-4.4.2/apysc/_geom/path_move_to.py
--rw-r--r--   0 runner    (1001) docker     (127)     6482 2024-05-23 14:23:55.000000 apysc-4.4.2/apysc/_geom/path_vertical.py
--rw-r--r--   0 runner    (1001) docker     (127)     3662 2024-05-23 14:23:55.000000 apysc-4.4.2/apysc/_geom/path_x_mixin.py
--rw-r--r--   0 runner    (1001) docker     (127)     3655 2024-05-23 14:23:55.000000 apysc-4.4.2/apysc/_geom/path_y_mixin.py
--rw-r--r--   0 runner    (1001) docker     (127)    12328 2024-05-23 14:23:55.000000 apysc-4.4.2/apysc/_geom/point2d.py
--rw-r--r--   0 runner    (1001) docker     (127)     4230 2024-05-23 14:23:55.000000 apysc-4.4.2/apysc/_geom/rectangle_geom.py
--rw-r--r--   0 runner    (1001) docker     (127)      558 2024-05-23 14:23:55.000000 apysc-4.4.2/apysc/_geom/rectangle_geom_bottom_y_mixin.py
--rw-r--r--   0 runner    (1001) docker     (127)      558 2024-05-23 14:23:55.000000 apysc-4.4.2/apysc/_geom/rectangle_geom_center_x_mixin.py
--rw-r--r--   0 runner    (1001) docker     (127)      558 2024-05-23 14:23:55.000000 apysc-4.4.2/apysc/_geom/rectangle_geom_center_y_mixin.py
--rw-r--r--   0 runner    (1001) docker     (127)      524 2024-05-23 14:23:55.000000 apysc-4.4.2/apysc/_geom/rectangle_geom_height_mixin.py
--rw-r--r--   0 runner    (1001) docker     (127)      542 2024-05-23 14:23:55.000000 apysc-4.4.2/apysc/_geom/rectangle_geom_left_x_mixin.py
--rw-r--r--   0 runner    (1001) docker     (127)      550 2024-05-23 14:23:55.000000 apysc-4.4.2/apysc/_geom/rectangle_geom_right_x_mixin.py
--rw-r--r--   0 runner    (1001) docker     (127)      534 2024-05-23 14:23:55.000000 apysc-4.4.2/apysc/_geom/rectangle_geom_top_y_mixin.py
--rw-r--r--   0 runner    (1001) docker     (127)      516 2024-05-23 14:23:55.000000 apysc-4.4.2/apysc/_geom/rectangle_geom_width_mixin.py
--rw-r--r--   0 runner    (1001) docker     (127)     3392 2024-05-23 14:23:55.000000 apysc-4.4.2/apysc/_geom/relative_mixin.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-23 14:24:13.322299 apysc-4.4.2/apysc/_html/
--rw-r--r--   0 runner    (1001) docker     (127)        0 2024-05-23 14:23:55.000000 apysc-4.4.2/apysc/_html/__init__.py
--rw-r--r--   0 runner    (1001) docker     (127)    14617 2024-05-23 14:23:55.000000 apysc-4.4.2/apysc/_html/debug_mode.py
--rw-r--r--   0 runner    (1001) docker     (127)    20660 2024-05-23 14:23:55.000000 apysc-4.4.2/apysc/_html/exporter.py
--rw-r--r--   0 runner    (1001) docker     (127)      129 2024-05-23 14:23:55.000000 apysc-4.4.2/apysc/_html/html_const.py
--rw-r--r--   0 runner    (1001) docker     (127)     8721 2024-05-23 14:23:55.000000 apysc-4.4.2/apysc/_html/html_util.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-23 14:24:13.322299 apysc-4.4.2/apysc/_jslib/
--rw-r--r--   0 runner    (1001) docker     (127)        0 2024-05-23 14:23:55.000000 apysc-4.4.2/apysc/_jslib/__init__.py
--rw-r--r--   0 runner    (1001) docker     (127)    70264 2024-05-23 14:23:55.000000 apysc-4.4.2/apysc/_jslib/jquery-3.7.1.slim.min.js
--rw-r--r--   0 runner    (1001) docker     (127)     2752 2024-05-23 14:23:55.000000 apysc-4.4.2/apysc/_jslib/jquery.mousewheel-3.1.13.min.js
--rw-r--r--   0 runner    (1001) docker     (127)     5134 2024-05-23 14:23:55.000000 apysc-4.4.2/apysc/_jslib/jslib_util.py
--rw-r--r--   0 runner    (1001) docker     (127)    78572 2024-05-23 14:23:55.000000 apysc-4.4.2/apysc/_jslib/svg-3.1.2.min.js
--rw-r--r--   0 runner    (1001) docker     (127)    19431 2024-05-23 14:23:55.000000 apysc-4.4.2/apysc/_jslib/underscore-1.12.0.min.js
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-23 14:24:13.322299 apysc-4.4.2/apysc/_jupyter/
--rw-r--r--   0 runner    (1001) docker     (127)        0 2024-05-23 14:23:55.000000 apysc-4.4.2/apysc/_jupyter/__init__.py
--rw-r--r--   0 runner    (1001) docker     (127)     3824 2024-05-23 14:23:55.000000 apysc-4.4.2/apysc/_jupyter/jupyter_util.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-23 14:24:13.326300 apysc-4.4.2/apysc/_lint_and_doc/
--rw-r--r--   0 runner    (1001) docker     (127)        0 2024-05-23 14:23:55.000000 apysc-4.4.2/apysc/_lint_and_doc/__init__.py
--rw-r--r--   0 runner    (1001) docker     (127)    17625 2024-05-23 14:23:55.000000 apysc-4.4.2/apysc/_lint_and_doc/add_doc_translation_mapping_blank_data.py
--rw-r--r--   0 runner    (1001) docker     (127)     1265 2024-05-23 14:23:55.000000 apysc-4.4.2/apysc/_lint_and_doc/conf_common.py
--rw-r--r--   0 runner    (1001) docker     (127)    10316 2024-05-23 14:23:55.000000 apysc-4.4.2/apysc/_lint_and_doc/docs_keyword_link_mapping.py
--rw-r--r--   0 runner    (1001) docker     (127)      861 2024-05-23 14:23:55.000000 apysc-4.4.2/apysc/_lint_and_doc/docs_lang.py
--rw-r--r--   0 runner    (1001) docker     (127)     7966 2024-05-23 14:23:55.000000 apysc-4.4.2/apysc/_lint_and_doc/docs_toctree_util.py
--rw-r--r--   0 runner    (1001) docker     (127)    17282 2024-05-23 14:23:55.000000 apysc-4.4.2/apysc/_lint_and_doc/docs_translation_converter.py
--rw-r--r--   0 runner    (1001) docker     (127)    13722 2024-05-23 14:23:55.000000 apysc-4.4.2/apysc/_lint_and_doc/docstring_to_markdown_converter.py
--rw-r--r--   0 runner    (1001) docker     (127)    51969 2024-05-23 14:23:55.000000 apysc-4.4.2/apysc/_lint_and_doc/docstring_util.py
--rw-r--r--   0 runner    (1001) docker     (127)     7636 2024-05-23 14:23:55.000000 apysc-4.4.2/apysc/_lint_and_doc/document_text_split_util.py
--rw-r--r--   0 runner    (1001) docker     (127)     1805 2024-05-23 14:23:55.000000 apysc-4.4.2/apysc/_lint_and_doc/document_util.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-23 14:24:13.326300 apysc-4.4.2/apysc/_lint_and_doc/fixed_translation_mapping/
--rw-r--r--   0 runner    (1001) docker     (127)        0 2024-05-23 14:23:55.000000 apysc-4.4.2/apysc/_lint_and_doc/fixed_translation_mapping/__init__.py
--rw-r--r--   0 runner    (1001) docker     (127)     5760 2024-05-23 14:23:55.000000 apysc-4.4.2/apysc/_lint_and_doc/fixed_translation_mapping/data_model.py
--rw-r--r--   0 runner    (1001) docker     (127)   247888 2024-05-23 14:23:55.000000 apysc-4.4.2/apysc/_lint_and_doc/fixed_translation_mapping/jp.py
--rw-r--r--   0 runner    (1001) docker     (127)     9404 2024-05-23 14:23:55.000000 apysc-4.4.2/apysc/_lint_and_doc/lint_and_doc_hash_util.py
--rw-r--r--   0 runner    (1001) docker     (127)    11174 2024-05-23 14:23:55.000000 apysc-4.4.2/apysc/_lint_and_doc/translation_mapping_utils.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-23 14:24:13.326300 apysc-4.4.2/apysc/_loop/
--rw-r--r--   0 runner    (1001) docker     (127)        0 2024-05-23 14:23:55.000000 apysc-4.4.2/apysc/_loop/__init__.py
--rw-r--r--   0 runner    (1001) docker     (127)     2023 2024-05-23 14:23:55.000000 apysc-4.4.2/apysc/_loop/_continue.py
--rw-r--r--   0 runner    (1001) docker     (127)     4121 2024-05-23 14:23:55.000000 apysc-4.4.2/apysc/_loop/_range.py
--rw-r--r--   0 runner    (1001) docker     (127)     6079 2024-05-23 14:23:55.000000 apysc-4.4.2/apysc/_loop/for_array_indices.py
--rw-r--r--   0 runner    (1001) docker     (127)     6913 2024-05-23 14:23:55.000000 apysc-4.4.2/apysc/_loop/for_array_indices_and_values.py
--rw-r--r--   0 runner    (1001) docker     (127)     6128 2024-05-23 14:23:55.000000 apysc-4.4.2/apysc/_loop/for_array_values.py
--rw-r--r--   0 runner    (1001) docker     (127)     6156 2024-05-23 14:23:55.000000 apysc-4.4.2/apysc/_loop/for_dict_keys.py
--rw-r--r--   0 runner    (1001) docker     (127)     7806 2024-05-23 14:23:55.000000 apysc-4.4.2/apysc/_loop/for_dict_keys_and_values.py
--rw-r--r--   0 runner    (1001) docker     (127)     6732 2024-05-23 14:23:55.000000 apysc-4.4.2/apysc/_loop/for_dict_values.py
--rw-r--r--   0 runner    (1001) docker     (127)     1551 2024-05-23 14:23:55.000000 apysc-4.4.2/apysc/_loop/for_loop_exit_mixin.py
--rw-r--r--   0 runner    (1001) docker     (127)      486 2024-05-23 14:23:55.000000 apysc-4.4.2/apysc/_loop/initialize_with_base_value_interface.py
--rw-r--r--   0 runner    (1001) docker     (127)     1799 2024-05-23 14:23:55.000000 apysc-4.4.2/apysc/_loop/loop_count.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-23 14:24:13.326300 apysc-4.4.2/apysc/_material_design/
--rw-r--r--   0 runner    (1001) docker     (127)        0 2024-05-23 14:23:55.000000 apysc-4.4.2/apysc/_material_design/__init__.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-23 14:24:13.466301 apysc-4.4.2/apysc/_material_design/icon/
--rw-r--r--   0 runner    (1001) docker     (127)        0 2024-05-23 14:23:55.000000 apysc-4.4.2/apysc/_material_design/icon/__init__.py
--rw-r--r--   0 runner    (1001) docker     (127)     1294 2024-05-23 14:23:55.000000 apysc-4.4.2/apysc/_material_design/icon/material_10k_icon.py
--rw-r--r--   0 runner    (1001) docker     (127)     1189 2024-05-23 14:23:55.000000 apysc-4.4.2/apysc/_material_design/icon/material_1k_icon.py
--rw-r--r--   0 runner    (1001) docker     (127)     1253 2024-05-23 14:23:55.000000 apysc-4.4.2/apysc/_material_design/icon/material_1k_plus_icon.py
--rw-r--r--   0 runner    (1001) docker     (127)     1253 2024-05-23 14:23:55.000000 apysc-4.4.2/apysc/_material_design/icon/material_2k_icon.py
--rw-r--r--   0 runner    (1001) docker     (127)     1320 2024-05-23 14:23:55.000000 apysc-4.4.2/apysc/_material_design/icon/material_2k_plus_icon.py
--rw-r--r--   0 runner    (1001) docker     (127)     2513 2024-05-23 14:23:55.000000 apysc-4.4.2/apysc/_material_design/icon/material_3d_rotation_icon.py
--rw-r--r--   0 runner    (1001) docker     (127)     2493 2024-05-23 14:23:55.000000 apysc-4.4.2/apysc/_material_design/icon/material_3d_rotation_outlined_icon.py
--rw-r--r--   0 runner    (1001) docker     (127)     1235 2024-05-23 14:23:55.000000 apysc-4.4.2/apysc/_material_design/icon/material_3k_icon.py
--rw-r--r--   0 runner    (1001) docker     (127)     1296 2024-05-23 14:23:55.000000 apysc-4.4.2/apysc/_material_design/icon/material_3k_plus_icon.py
--rw-r--r--   0 runner    (1001) docker     (127)     1213 2024-05-23 14:23:55.000000 apysc-4.4.2/apysc/_material_design/icon/material_4k_icon.py
--rw-r--r--   0 runner    (1001) docker     (127)     1237 2024-05-23 14:23:55.000000 apysc-4.4.2/apysc/_material_design/icon/material_4k_outlined_icon.py
--rw-r--r--   0 runner    (1001) docker     (127)     1274 2024-05-23 14:23:55.000000 apysc-4.4.2/apysc/_material_design/icon/material_4k_plus_icon.py
--rw-r--r--   0 runner    (1001) docker     (127)     1254 2024-05-23 14:23:55.000000 apysc-4.4.2/apysc/_material_design/icon/material_5g_icon.py
--rw-r--r--   0 runner    (1001) docker     (127)     1285 2024-05-23 14:23:55.000000 apysc-4.4.2/apysc/_material_design/icon/material_5g_outlined_icon.py
--rw-r--r--   0 runner    (1001) docker     (127)     1238 2024-05-23 14:23:55.000000 apysc-4.4.2/apysc/_material_design/icon/material_5k_icon.py
--rw-r--r--   0 runner    (1001) docker     (127)     1300 2024-05-23 14:23:55.000000 apysc-4.4.2/apysc/_material_design/icon/material_5k_plus_icon.py
--rw-r--r--   0 runner    (1001) docker     (127)     1275 2024-05-23 14:23:55.000000 apysc-4.4.2/apysc/_material_design/icon/material_6k_icon.py
--rw-r--r--   0 runner    (1001) docker     (127)     1340 2024-05-23 14:23:55.000000 apysc-4.4.2/apysc/_material_design/icon/material_6k_plus_icon.py
--rw-r--r--   0 runner    (1001) docker     (127)     1223 2024-05-23 14:23:55.000000 apysc-4.4.2/apysc/_material_design/icon/material_7k_icon.py
--rw-r--r--   0 runner    (1001) docker     (127)     1277 2024-05-23 14:23:55.000000 apysc-4.4.2/apysc/_material_design/icon/material_7k_plus_icon.py
--rw-r--r--   0 runner    (1001) docker     (127)     1277 2024-05-23 14:23:55.000000 apysc-4.4.2/apysc/_material_design/icon/material_8k_icon.py
--rw-r--r--   0 runner    (1001) docker     (127)     1343 2024-05-23 14:23:55.000000 apysc-4.4.2/apysc/_material_design/icon/material_8k_plus_icon.py
--rw-r--r--   0 runner    (1001) docker     (127)     1273 2024-05-23 14:23:55.000000 apysc-4.4.2/apysc/_material_design/icon/material_9k_icon.py
--rw-r--r--   0 runner    (1001) docker     (127)     1337 2024-05-23 14:23:55.000000 apysc-4.4.2/apysc/_material_design/icon/material_9k_plus_icon.py
--rw-r--r--   0 runner    (1001) docker     (127)     1136 2024-05-23 14:23:55.000000 apysc-4.4.2/apysc/_material_design/icon/material_accessibility_icon.py
--rw-r--r--   0 runner    (1001) docker     (127)     1217 2024-05-23 14:23:55.000000 apysc-4.4.2/apysc/_material_design/icon/material_accessibility_new_icon.py
--rw-r--r--   0 runner    (1001) docker     (127)     1245 2024-05-23 14:23:55.000000 apysc-4.4.2/apysc/_material_design/icon/material_accessibility_new_outlined_icon.py
--rw-r--r--   0 runner    (1001) docker     (127)     1164 2024-05-23 14:23:55.000000 apysc-4.4.2/apysc/_material_design/icon/material_accessibility_outlined_icon.py
--rw-r--r--   0 runner    (1001) docker     (127)     1360 2024-05-23 14:23:55.000000 apysc-4.4.2/apysc/_material_design/icon/material_accessible_forward_icon.py
--rw-r--r--   0 runner    (1001) docker     (127)     1389 2024-05-23 14:23:55.000000 apysc-4.4.2/apysc/_material_design/icon/material_accessible_forward_outlined_icon.py
--rw-r--r--   0 runner    (1001) docker     (127)     1449 2024-05-23 14:23:55.000000 apysc-4.4.2/apysc/_material_design/icon/material_accessible_icon.py
--rw-r--r--   0 runner    (1001) docker     (127)     1475 2024-05-23 14:23:55.000000 apysc-4.4.2/apysc/_material_design/icon/material_accessible_outlined_icon.py
--rw-r--r--   0 runner    (1001) docker     (127)     1316 2024-05-23 14:23:55.000000 apysc-4.4.2/apysc/_material_design/icon/material_account_balance_icon.py
--rw-r--r--   0 runner    (1001) docker     (127)     1210 2024-05-23 14:23:55.000000 apysc-4.4.2/apysc/_material_design/icon/material_account_balance_outlined_icon.py
--rw-r--r--   0 runner    (1001) docker     (127)     1289 2024-05-23 14:23:55.000000 apysc-4.4.2/apysc/_material_design/icon/material_account_balance_wallet_icon.py
--rw-r--r--   0 runner    (1001) docker     (127)     1339 2024-05-23 14:23:55.000000 apysc-4.4.2/apysc/_material_design/icon/material_account_balance_wallet_outlined_icon.py
--rw-r--r--   0 runner    (1001) docker     (127)     1221 2024-05-23 14:23:55.000000 apysc-4.4.2/apysc/_material_design/icon/material_account_box_icon.py
--rw-r--r--   0 runner    (1001) docker     (127)     1391 2024-05-23 14:23:55.000000 apysc-4.4.2/apysc/_material_design/icon/material_account_box_outlined_icon.py
--rw-r--r--   0 runner    (1001) docker     (127)     1281 2024-05-23 14:23:55.000000 apysc-4.4.2/apysc/_material_design/icon/material_account_circle_icon.py
--rw-r--r--   0 runner    (1001) docker     (127)     1539 2024-05-23 14:23:55.000000 apysc-4.4.2/apysc/_material_design/icon/material_account_circle_outlined_icon.py
--rw-r--r--   0 runner    (1001) docker     (127)     1301 2024-05-23 14:23:55.000000 apysc-4.4.2/apysc/_material_design/icon/material_add_alert_icon.py
--rw-r--r--   0 runner    (1001) docker     (127)     1300 2024-05-23 14:23:55.000000 apysc-4.4.2/apysc/_material_design/icon/material_add_alert_outlined_icon.py
--rw-r--r--   0 runner    (1001) docker     (127)     1146 2024-05-23 14:23:55.000000 apysc-4.4.2/apysc/_material_design/icon/material_add_box_icon.py
--rw-r--r--   0 runner    (1001) docker     (127)     1187 2024-05-23 14:23:55.000000 apysc-4.4.2/apysc/_material_design/icon/material_add_box_outlined_icon.py
--rw-r--r--   0 runner    (1001) docker     (127)     1142 2024-05-23 14:23:55.000000 apysc-4.4.2/apysc/_material_design/icon/material_add_circle_icon.py
--rw-r--r--   0 runner    (1001) docker     (127)     1223 2024-05-23 14:23:55.000000 apysc-4.4.2/apysc/_material_design/icon/material_add_circle_outline_icon.py
--rw-r--r--   0 runner    (1001) docker     (127)     1251 2024-05-23 14:23:55.000000 apysc-4.4.2/apysc/_material_design/icon/material_add_circle_outline_outlined_icon.py
--rw-r--r--   0 runner    (1001) docker     (127)     1170 2024-05-23 14:23:55.000000 apysc-4.4.2/apysc/_material_design/icon/material_add_circle_outlined_icon.py
--rw-r--r--   0 runner    (1001) docker     (127)     1319 2024-05-23 14:23:55.000000 apysc-4.4.2/apysc/_material_design/icon/material_add_ic_call_icon.py
--rw-r--r--   0 runner    (1001) docker     (127)     1518 2024-05-23 14:23:55.000000 apysc-4.4.2/apysc/_material_design/icon/material_add_ic_call_outlined_icon.py
--rw-r--r--   0 runner    (1001) docker     (127)     1057 2024-05-23 14:23:55.000000 apysc-4.4.2/apysc/_material_design/icon/material_add_icon.py
--rw-r--r--   0 runner    (1001) docker     (127)     1245 2024-05-23 14:23:55.000000 apysc-4.4.2/apysc/_material_design/icon/material_add_link_icon.py
--rw-r--r--   0 runner    (1001) docker     (127)     1085 2024-05-23 14:23:55.000000 apysc-4.4.2/apysc/_material_design/icon/material_add_outlined_icon.py
--rw-r--r--   0 runner    (1001) docker     (127)     1449 2024-05-23 14:23:55.000000 apysc-4.4.2/apysc/_material_design/icon/material_add_shopping_cart_icon.py
--rw-r--r--   0 runner    (1001) docker     (127)     1376 2024-05-23 14:23:55.000000 apysc-4.4.2/apysc/_material_design/icon/material_add_shopping_cart_outlined_icon.py
--rw-r--r--   0 runner    (1001) docker     (127)     1375 2024-05-23 14:23:55.000000 apysc-4.4.2/apysc/_material_design/icon/material_add_task_icon.py
--rw-r--r--   0 runner    (1001) docker     (127)     1401 2024-05-23 14:23:55.000000 apysc-4.4.2/apysc/_material_design/icon/material_add_task_outlined_icon.py
--rw-r--r--   0 runner    (1001) docker     (127)     1292 2024-05-23 14:23:55.000000 apysc-4.4.2/apysc/_material_design/icon/material_add_to_drive_icon.py
--rw-r--r--   0 runner    (1001) docker     (127)     1196 2024-05-23 14:23:55.000000 apysc-4.4.2/apysc/_material_design/icon/material_add_to_queue_icon.py
--rw-r--r--   0 runner    (1001) docker     (127)     1212 2024-05-23 14:23:55.000000 apysc-4.4.2/apysc/_material_design/icon/material_add_to_queue_outlined_icon.py
--rw-r--r--   0 runner    (1001) docker     (127)     1192 2024-05-23 14:23:55.000000 apysc-4.4.2/apysc/_material_design/icon/material_addchart_icon.py
--rw-r--r--   0 runner    (1001) docker     (127)     1276 2024-05-23 14:23:55.000000 apysc-4.4.2/apysc/_material_design/icon/material_addchart_outlined_icon.py
--rw-r--r--   0 runner    (1001) docker     (127)     1608 2024-05-23 14:23:55.000000 apysc-4.4.2/apysc/_material_design/icon/material_admin_panel_settings_icon.py
--rw-r--r--   0 runner    (1001) docker     (127)     1773 2024-05-23 14:23:55.000000 apysc-4.4.2/apysc/_material_design/icon/material_admin_panel_settings_outlined_icon.py
--rw-r--r--   0 runner    (1001) docker     (127)     1218 2024-05-23 14:23:55.000000 apysc-4.4.2/apysc/_material_design/icon/material_airplay_icon.py
--rw-r--r--   0 runner    (1001) docker     (127)     1346 2024-05-23 14:23:55.000000 apysc-4.4.2/apysc/_material_design/icon/material_airplay_outlined_icon.py
--rw-r--r--   0 runner    (1001) docker     (127)     1290 2024-05-23 14:23:55.000000 apysc-4.4.2/apysc/_material_design/icon/material_alarm_add_icon.py
--rw-r--r--   0 runner    (1001) docker     (127)     1308 2024-05-23 14:23:55.000000 apysc-4.4.2/apysc/_material_design/icon/material_alarm_add_outlined_icon.py
--rw-r--r--   0 runner    (1001) docker     (127)     1285 2024-05-23 14:23:55.000000 apysc-4.4.2/apysc/_material_design/icon/material_alarm_icon.py
--rw-r--r--   0 runner    (1001) docker     (127)     1541 2024-05-23 14:23:55.000000 apysc-4.4.2/apysc/_material_design/icon/material_alarm_off_icon.py
--rw-r--r--   0 runner    (1001) docker     (127)     1550 2024-05-23 14:23:55.000000 apysc-4.4.2/apysc/_material_design/icon/material_alarm_off_outlined_icon.py
--rw-r--r--   0 runner    (1001) docker     (127)     1320 2024-05-23 14:23:55.000000 apysc-4.4.2/apysc/_material_design/icon/material_alarm_on_icon.py
--rw-r--r--   0 runner    (1001) docker     (127)     1331 2024-05-23 14:23:55.000000 apysc-4.4.2/apysc/_material_design/icon/material_alarm_on_outlined_icon.py
--rw-r--r--   0 runner    (1001) docker     (127)     1302 2024-05-23 14:23:55.000000 apysc-4.4.2/apysc/_material_design/icon/material_alarm_outlined_icon.py
--rw-r--r--   0 runner    (1001) docker     (127)     1231 2024-05-23 14:23:55.000000 apysc-4.4.2/apysc/_material_design/icon/material_album_icon.py
--rw-r--r--   0 runner    (1001) docker     (127)     1318 2024-05-23 14:23:55.000000 apysc-4.4.2/apysc/_material_design/icon/material_album_outlined_icon.py
--rw-r--r--   0 runner    (1001) docker     (127)     1240 2024-05-23 14:23:55.000000 apysc-4.4.2/apysc/_material_design/icon/material_all_inbox_icon.py
--rw-r--r--   0 runner    (1001) docker     (127)     1534 2024-05-23 14:23:55.000000 apysc-4.4.2/apysc/_material_design/icon/material_all_inbox_outlined_icon.py
--rw-r--r--   0 runner    (1001) docker     (127)     1271 2024-05-23 14:23:55.000000 apysc-4.4.2/apysc/_material_design/icon/material_all_out_icon.py
--rw-r--r--   0 runner    (1001) docker     (127)     1227 2024-05-23 14:23:55.000000 apysc-4.4.2/apysc/_material_design/icon/material_all_out_outlined_icon.py
--rw-r--r--   0 runner    (1001) docker     (127)     1394 2024-05-23 14:23:55.000000 apysc-4.4.2/apysc/_material_design/icon/material_alternate_email_icon.py
--rw-r--r--   0 runner    (1001) docker     (127)     1434 2024-05-23 14:23:55.000000 apysc-4.4.2/apysc/_material_design/icon/material_alternate_email_outlined_icon.py
--rw-r--r--   0 runner    (1001) docker     (127)     1222 2024-05-23 14:23:55.000000 apysc-4.4.2/apysc/_material_design/icon/material_amp_stories_icon.py
--rw-r--r--   0 runner    (1001) docker     (127)     1249 2024-05-23 14:23:55.000000 apysc-4.4.2/apysc/_material_design/icon/material_amp_stories_outlined_icon.py
--rw-r--r--   0 runner    (1001) docker     (127)     1176 2024-05-23 14:23:55.000000 apysc-4.4.2/apysc/_material_design/icon/material_analytics_icon.py
--rw-r--r--   0 runner    (1001) docker     (127)     1387 2024-05-23 14:23:55.000000 apysc-4.4.2/apysc/_material_design/icon/material_analytics_outlined_icon.py
--rw-r--r--   0 runner    (1001) docker     (127)     1371 2024-05-23 14:23:55.000000 apysc-4.4.2/apysc/_material_design/icon/material_anchor_icon.py
--rw-r--r--   0 runner    (1001) docker     (127)     1397 2024-05-23 14:23:55.000000 apysc-4.4.2/apysc/_material_design/icon/material_anchor_outlined_icon.py
--rw-r--r--   0 runner    (1001) docker     (127)     1577 2024-05-23 14:23:55.000000 apysc-4.4.2/apysc/_material_design/icon/material_android_icon.py
--rw-r--r--   0 runner    (1001) docker     (127)     1623 2024-05-23 14:23:55.000000 apysc-4.4.2/apysc/_material_design/icon/material_android_outlined_icon.py
--rw-r--r--   0 runner    (1001) docker     (127)     1152 2024-05-23 14:23:55.000000 apysc-4.4.2/apysc/_material_design/icon/material_announcement_icon.py
--rw-r--r--   0 runner    (1001) docker     (127)     1195 2024-05-23 14:23:55.000000 apysc-4.4.2/apysc/_material_design/icon/material_announcement_outlined_icon.py
--rw-r--r--   0 runner    (1001) docker     (127)     1322 2024-05-23 14:23:55.000000 apysc-4.4.2/apysc/_material_design/icon/material_api_icon.py
--rw-r--r--   0 runner    (1001) docker     (127)     1348 2024-05-23 14:23:55.000000 apysc-4.4.2/apysc/_material_design/icon/material_api_outlined_icon.py
--rw-r--r--   0 runner    (1001) docker     (127)     1377 2024-05-23 14:23:55.000000 apysc-4.4.2/apysc/_material_design/icon/material_app_blocking_icon.py
--rw-r--r--   0 runner    (1001) docker     (127)     1570 2024-05-23 14:23:55.000000 apysc-4.4.2/apysc/_material_design/icon/material_app_blocking_outlined_icon.py
--rw-r--r--   0 runner    (1001) docker     (127)     1562 2024-05-23 14:23:55.000000 apysc-4.4.2/apysc/_material_design/icon/material_app_registration_icon.py
--rw-r--r--   0 runner    (1001) docker     (127)     1266 2024-05-23 14:23:55.000000 apysc-4.4.2/apysc/_material_design/icon/material_archive_icon.py
--rw-r--r--   0 runner    (1001) docker     (127)     1308 2024-05-23 14:23:55.000000 apysc-4.4.2/apysc/_material_design/icon/material_archive_outlined_icon.py
--rw-r--r--   0 runner    (1001) docker     (127)     1294 2024-05-23 14:23:55.000000 apysc-4.4.2/apysc/_material_design/icon/material_arrow_circle_down_icon.py
--rw-r--r--   0 runner    (1001) docker     (127)     1320 2024-05-23 14:23:55.000000 apysc-4.4.2/apysc/_material_design/icon/material_arrow_circle_down_outlined_icon.py
--rw-r--r--   0 runner    (1001) docker     (127)     1295 2024-05-23 14:23:55.000000 apysc-4.4.2/apysc/_material_design/icon/material_arrow_circle_up_icon.py
--rw-r--r--   0 runner    (1001) docker     (127)     1321 2024-05-23 14:23:55.000000 apysc-4.4.2/apysc/_material_design/icon/material_arrow_circle_up_outlined_icon.py
--rw-r--r--   0 runner    (1001) docker     (127)     1092 2024-05-23 14:23:55.000000 apysc-4.4.2/apysc/_material_design/icon/material_arrow_right_alt_icon.py
--rw-r--r--   0 runner    (1001) docker     (127)     1122 2024-05-23 14:23:55.000000 apysc-4.4.2/apysc/_material_design/icon/material_arrow_right_alt_outlined_icon.py
--rw-r--r--   0 runner    (1001) docker     (127)     1206 2024-05-23 14:23:55.000000 apysc-4.4.2/apysc/_material_design/icon/material_art_track_icon.py
--rw-r--r--   0 runner    (1001) docker     (127)     1234 2024-05-23 14:23:55.000000 apysc-4.4.2/apysc/_material_design/icon/material_art_track_outlined_icon.py
--rw-r--r--   0 runner    (1001) docker     (127)     1155 2024-05-23 14:23:55.000000 apysc-4.4.2/apysc/_material_design/icon/material_article_icon.py
--rw-r--r--   0 runner    (1001) docker     (127)     1281 2024-05-23 14:23:55.000000 apysc-4.4.2/apysc/_material_design/icon/material_article_outlined_icon.py
--rw-r--r--   0 runner    (1001) docker     (127)     1188 2024-05-23 14:23:55.000000 apysc-4.4.2/apysc/_material_design/icon/material_aspect_ratio_icon.py
--rw-r--r--   0 runner    (1001) docker     (127)     1216 2024-05-23 14:23:55.000000 apysc-4.4.2/apysc/_material_design/icon/material_aspect_ratio_outlined_icon.py
--rw-r--r--   0 runner    (1001) docker     (127)     1164 2024-05-23 14:23:55.000000 apysc-4.4.2/apysc/_material_design/icon/material_assessment_icon.py
--rw-r--r--   0 runner    (1001) docker     (127)     1200 2024-05-23 14:23:55.000000 apysc-4.4.2/apysc/_material_design/icon/material_assessment_outlined_icon.py
--rw-r--r--   0 runner    (1001) docker     (127)     1265 2024-05-23 14:23:55.000000 apysc-4.4.2/apysc/_material_design/icon/material_assignment_icon.py
--rw-r--r--   0 runner    (1001) docker     (127)     1333 2024-05-23 14:23:55.000000 apysc-4.4.2/apysc/_material_design/icon/material_assignment_ind_icon.py
--rw-r--r--   0 runner    (1001) docker     (127)     1564 2024-05-23 14:23:55.000000 apysc-4.4.2/apysc/_material_design/icon/material_assignment_ind_outlined_icon.py
--rw-r--r--   0 runner    (1001) docker     (127)     1266 2024-05-23 14:23:55.000000 apysc-4.4.2/apysc/_material_design/icon/material_assignment_late_icon.py
--rw-r--r--   0 runner    (1001) docker     (127)     1445 2024-05-23 14:23:55.000000 apysc-4.4.2/apysc/_material_design/icon/material_assignment_late_outlined_icon.py
--rw-r--r--   0 runner    (1001) docker     (127)     1442 2024-05-23 14:23:55.000000 apysc-4.4.2/apysc/_material_design/icon/material_assignment_outlined_icon.py
--rw-r--r--   0 runner    (1001) docker     (127)     1267 2024-05-23 14:23:55.000000 apysc-4.4.2/apysc/_material_design/icon/material_assignment_return_icon.py
--rw-r--r--   0 runner    (1001) docker     (127)     1452 2024-05-23 14:23:55.000000 apysc-4.4.2/apysc/_material_design/icon/material_assignment_return_outlined_icon.py
--rw-r--r--   0 runner    (1001) docker     (127)     1273 2024-05-23 14:23:55.000000 apysc-4.4.2/apysc/_material_design/icon/material_assignment_returned_icon.py
--rw-r--r--   0 runner    (1001) docker     (127)     1454 2024-05-23 14:23:55.000000 apysc-4.4.2/apysc/_material_design/icon/material_assignment_returned_outlined_icon.py
--rw-r--r--   0 runner    (1001) docker     (127)     1300 2024-05-23 14:23:55.000000 apysc-4.4.2/apysc/_material_design/icon/material_assignment_turned_in_icon.py
--rw-r--r--   0 runner    (1001) docker     (127)     1479 2024-05-23 14:23:55.000000 apysc-4.4.2/apysc/_material_design/icon/material_assignment_turned_in_outlined_icon.py
--rw-r--r--   0 runner    (1001) docker     (127)     1321 2024-05-23 14:23:55.000000 apysc-4.4.2/apysc/_material_design/icon/material_attribution_outlined_icon.py
--rw-r--r--   0 runner    (1001) docker     (127)     1423 2024-05-23 14:23:55.000000 apysc-4.4.2/apysc/_material_design/icon/material_auto_delete_icon.py
--rw-r--r--   0 runner    (1001) docker     (127)     1517 2024-05-23 14:23:55.000000 apysc-4.4.2/apysc/_material_design/icon/material_auto_delete_outlined_icon.py
--rw-r--r--   0 runner    (1001) docker     (127)     1270 2024-05-23 14:23:55.000000 apysc-4.4.2/apysc/_material_design/icon/material_autorenew_icon.py
--rw-r--r--   0 runner    (1001) docker     (127)     1298 2024-05-23 14:23:55.000000 apysc-4.4.2/apysc/_material_design/icon/material_autorenew_outlined_icon.py
--rw-r--r--   0 runner    (1001) docker     (127)     1384 2024-05-23 14:23:55.000000 apysc-4.4.2/apysc/_material_design/icon/material_av_timer_icon.py
--rw-r--r--   0 runner    (1001) docker     (127)     1412 2024-05-23 14:23:55.000000 apysc-4.4.2/apysc/_material_design/icon/material_av_timer_outlined_icon.py
--rw-r--r--   0 runner    (1001) docker     (127)     1253 2024-05-23 14:23:55.000000 apysc-4.4.2/apysc/_material_design/icon/material_backspace_icon.py
--rw-r--r--   0 runner    (1001) docker     (127)     1303 2024-05-23 14:23:55.000000 apysc-4.4.2/apysc/_material_design/icon/material_backspace_outlined_icon.py
--rw-r--r--   0 runner    (1001) docker     (127)     1211 2024-05-23 14:23:55.000000 apysc-4.4.2/apysc/_material_design/icon/material_backup_icon.py
--rw-r--r--   0 runner    (1001) docker     (127)     1418 2024-05-23 14:23:55.000000 apysc-4.4.2/apysc/_material_design/icon/material_backup_outlined_icon.py
--rw-r--r--   0 runner    (1001) docker     (127)     1293 2024-05-23 14:23:55.000000 apysc-4.4.2/apysc/_material_design/icon/material_backup_table_icon.py
--rw-r--r--   0 runner    (1001) docker     (127)     1319 2024-05-23 14:23:55.000000 apysc-4.4.2/apysc/_material_design/icon/material_backup_table_outlined_icon.py
--rw-r--r--   0 runner    (1001) docker     (127)     1306 2024-05-23 14:23:55.000000 apysc-4.4.2/apysc/_material_design/icon/material_ballot_icon.py
--rw-r--r--   0 runner    (1001) docker     (127)     1235 2024-05-23 14:23:55.000000 apysc-4.4.2/apysc/_material_design/icon/material_ballot_outlined_icon.py
--rw-r--r--   0 runner    (1001) docker     (127)     1451 2024-05-23 14:23:55.000000 apysc-4.4.2/apysc/_material_design/icon/material_batch_prediction_icon.py
--rw-r--r--   0 runner    (1001) docker     (127)     1477 2024-05-23 14:23:55.000000 apysc-4.4.2/apysc/_material_design/icon/material_batch_prediction_outlined_icon.py
--rw-r--r--   0 runner    (1001) docker     (127)     1541 2024-05-23 14:23:55.000000 apysc-4.4.2/apysc/_material_design/icon/material_biotech_icon.py
--rw-r--r--   0 runner    (1001) docker     (127)     1631 2024-05-23 14:23:55.000000 apysc-4.4.2/apysc/_material_design/icon/material_biotech_outlined_icon.py
--rw-r--r--   0 runner    (1001) docker     (127)     1330 2024-05-23 14:23:55.000000 apysc-4.4.2/apysc/_material_design/icon/material_block_flipped_icon.py
--rw-r--r--   0 runner    (1001) docker     (127)     1261 2024-05-23 14:23:55.000000 apysc-4.4.2/apysc/_material_design/icon/material_block_icon.py
--rw-r--r--   0 runner    (1001) docker     (127)     1289 2024-05-23 14:23:55.000000 apysc-4.4.2/apysc/_material_design/icon/material_block_outlined_icon.py
--rw-r--r--   0 runner    (1001) docker     (127)     1139 2024-05-23 14:23:55.000000 apysc-4.4.2/apysc/_material_design/icon/material_bolt_icon.py
--rw-r--r--   0 runner    (1001) docker     (127)     1126 2024-05-23 14:23:55.000000 apysc-4.4.2/apysc/_material_design/icon/material_book_icon.py
--rw-r--r--   0 runner    (1001) docker     (127)     1465 2024-05-23 14:23:55.000000 apysc-4.4.2/apysc/_material_design/icon/material_book_online_icon.py
--rw-r--r--   0 runner    (1001) docker     (127)     1523 2024-05-23 14:23:55.000000 apysc-4.4.2/apysc/_material_design/icon/material_book_online_outlined_icon.py
--rw-r--r--   0 runner    (1001) docker     (127)     1185 2024-05-23 14:23:55.000000 apysc-4.4.2/apysc/_material_design/icon/material_book_outlined_icon.py
--rw-r--r--   0 runner    (1001) docker     (127)     1143 2024-05-23 14:23:55.000000 apysc-4.4.2/apysc/_material_design/icon/material_bookmark_border_icon.py
--rw-r--r--   0 runner    (1001) docker     (127)     1164 2024-05-23 14:23:55.000000 apysc-4.4.2/apysc/_material_design/icon/material_bookmark_border_outlined_icon.py
--rw-r--r--   0 runner    (1001) docker     (127)     1096 2024-05-23 14:23:55.000000 apysc-4.4.2/apysc/_material_design/icon/material_bookmark_icon.py
--rw-r--r--   0 runner    (1001) docker     (127)     1117 2024-05-23 14:23:55.000000 apysc-4.4.2/apysc/_material_design/icon/material_bookmark_outlined_icon.py
--rw-r--r--   0 runner    (1001) docker     (127)     1165 2024-05-23 14:23:55.000000 apysc-4.4.2/apysc/_material_design/icon/material_bookmarks_icon.py
--rw-r--r--   0 runner    (1001) docker     (127)     1239 2024-05-23 14:23:55.000000 apysc-4.4.2/apysc/_material_design/icon/material_bookmarks_outlined_icon.py
--rw-r--r--   0 runner    (1001) docker     (127)     1160 2024-05-23 14:23:55.000000 apysc-4.4.2/apysc/_material_design/icon/material_branding_watermark_icon.py
--rw-r--r--   0 runner    (1001) docker     (127)     1200 2024-05-23 14:23:55.000000 apysc-4.4.2/apysc/_material_design/icon/material_branding_watermark_outlined_icon.py
--rw-r--r--   0 runner    (1001) docker     (127)     1416 2024-05-23 14:23:55.000000 apysc-4.4.2/apysc/_material_design/icon/material_bug_report_icon.py
--rw-r--r--   0 runner    (1001) docker     (127)     1737 2024-05-23 14:23:55.000000 apysc-4.4.2/apysc/_material_design/icon/material_bug_report_outlined_icon.py
--rw-r--r--   0 runner    (1001) docker     (127)     1462 2024-05-23 14:23:55.000000 apysc-4.4.2/apysc/_material_design/icon/material_build_circle_icon.py
--rw-r--r--   0 runner    (1001) docker     (127)     1590 2024-05-23 14:23:55.000000 apysc-4.4.2/apysc/_material_design/icon/material_build_circle_outlined_icon.py
--rw-r--r--   0 runner    (1001) docker     (127)     1216 2024-05-23 14:23:55.000000 apysc-4.4.2/apysc/_material_design/icon/material_build_icon.py
--rw-r--r--   0 runner    (1001) docker     (127)     1496 2024-05-23 14:23:55.000000 apysc-4.4.2/apysc/_material_design/icon/material_build_outlined_icon.py
--rw-r--r--   0 runner    (1001) docker     (127)     1238 2024-05-23 14:23:55.000000 apysc-4.4.2/apysc/_material_design/icon/material_business_icon.py
--rw-r--r--   0 runner    (1001) docker     (127)     1266 2024-05-23 14:23:55.000000 apysc-4.4.2/apysc/_material_design/icon/material_business_outlined_icon.py
--rw-r--r--   0 runner    (1001) docker     (127)     1257 2024-05-23 14:23:55.000000 apysc-4.4.2/apysc/_material_design/icon/material_cached_icon.py
--rw-r--r--   0 runner    (1001) docker     (127)     1285 2024-05-23 14:23:55.000000 apysc-4.4.2/apysc/_material_design/icon/material_cached_outlined_icon.py
--rw-r--r--   0 runner    (1001) docker     (127)     1435 2024-05-23 14:23:55.000000 apysc-4.4.2/apysc/_material_design/icon/material_calculate_icon.py
--rw-r--r--   0 runner    (1001) docker     (127)     1619 2024-05-23 14:23:55.000000 apysc-4.4.2/apysc/_material_design/icon/material_calculate_outlined_icon.py
--rw-r--r--   0 runner    (1001) docker     (127)     1164 2024-05-23 14:23:55.000000 apysc-4.4.2/apysc/_material_design/icon/material_calendar_today_icon.py
--rw-r--r--   0 runner    (1001) docker     (127)     1208 2024-05-23 14:23:55.000000 apysc-4.4.2/apysc/_material_design/icon/material_calendar_today_outlined_icon.py
--rw-r--r--   0 runner    (1001) docker     (127)     1099 2024-05-23 14:23:55.000000 apysc-4.4.2/apysc/_material_design/icon/material_calendar_view_day_icon.py
--rw-r--r--   0 runner    (1001) docker     (127)     1145 2024-05-23 14:23:55.000000 apysc-4.4.2/apysc/_material_design/icon/material_calendar_view_day_outlined_icon.py
--rw-r--r--   0 runner    (1001) docker     (127)     1424 2024-05-23 14:23:55.000000 apysc-4.4.2/apysc/_material_design/icon/material_call_end_icon.py
--rw-r--r--   0 runner    (1001) docker     (127)     1583 2024-05-23 14:23:55.000000 apysc-4.4.2/apysc/_material_design/icon/material_call_end_outlined_icon.py
--rw-r--r--   0 runner    (1001) docker     (127)     1311 2024-05-23 14:23:55.000000 apysc-4.4.2/apysc/_material_design/icon/material_call_icon.py
--rw-r--r--   0 runner    (1001) docker     (127)     1082 2024-05-23 14:23:55.000000 apysc-4.4.2/apysc/_material_design/icon/material_call_made_icon.py
--rw-r--r--   0 runner    (1001) docker     (127)     1112 2024-05-23 14:23:55.000000 apysc-4.4.2/apysc/_material_design/icon/material_call_made_outlined_icon.py
--rw-r--r--   0 runner    (1001) docker     (127)     1142 2024-05-23 14:23:55.000000 apysc-4.4.2/apysc/_material_design/icon/material_call_merge_icon.py
--rw-r--r--   0 runner    (1001) docker     (127)     1170 2024-05-23 14:23:55.000000 apysc-4.4.2/apysc/_material_design/icon/material_call_merge_outlined_icon.py
--rw-r--r--   0 runner    (1001) docker     (127)     1095 2024-05-23 14:23:55.000000 apysc-4.4.2/apysc/_material_design/icon/material_call_missed_icon.py
--rw-r--r--   0 runner    (1001) docker     (127)     1200 2024-05-23 14:23:55.000000 apysc-4.4.2/apysc/_material_design/icon/material_call_missed_outgoing_icon.py
--rw-r--r--   0 runner    (1001) docker     (127)     1153 2024-05-23 14:23:55.000000 apysc-4.4.2/apysc/_material_design/icon/material_call_missed_outgoing_outlined_icon.py
--rw-r--r--   0 runner    (1001) docker     (127)     1131 2024-05-23 14:23:55.000000 apysc-4.4.2/apysc/_material_design/icon/material_call_missed_outlined_icon.py
--rw-r--r--   0 runner    (1001) docker     (127)     1460 2024-05-23 14:23:55.000000 apysc-4.4.2/apysc/_material_design/icon/material_call_outlined_icon.py
--rw-r--r--   0 runner    (1001) docker     (127)     1094 2024-05-23 14:23:55.000000 apysc-4.4.2/apysc/_material_design/icon/material_call_received_icon.py
--rw-r--r--   0 runner    (1001) docker     (127)     1130 2024-05-23 14:23:55.000000 apysc-4.4.2/apysc/_material_design/icon/material_call_received_outlined_icon.py
--rw-r--r--   0 runner    (1001) docker     (127)     1146 2024-05-23 14:23:55.000000 apysc-4.4.2/apysc/_material_design/icon/material_call_split_icon.py
--rw-r--r--   0 runner    (1001) docker     (127)     1182 2024-05-23 14:23:55.000000 apysc-4.4.2/apysc/_material_design/icon/material_call_split_outlined_icon.py
--rw-r--r--   0 runner    (1001) docker     (127)     1147 2024-05-23 14:23:55.000000 apysc-4.4.2/apysc/_material_design/icon/material_call_to_action_icon.py
--rw-r--r--   0 runner    (1001) docker     (127)     1186 2024-05-23 14:23:55.000000 apysc-4.4.2/apysc/_material_design/icon/material_call_to_action_outlined_icon.py
--rw-r--r--   0 runner    (1001) docker     (127)     1286 2024-05-23 14:23:55.000000 apysc-4.4.2/apysc/_material_design/icon/material_camera_enhance_icon.py
--rw-r--r--   0 runner    (1001) docker     (127)     1410 2024-05-23 14:23:55.000000 apysc-4.4.2/apysc/_material_design/icon/material_camera_enhance_outlined_icon.py
--rw-r--r--   0 runner    (1001) docker     (127)     1400 2024-05-23 14:23:55.000000 apysc-4.4.2/apysc/_material_design/icon/material_cancel_presentation_icon.py
--rw-r--r--   0 runner    (1001) docker     (127)     1303 2024-05-23 14:23:55.000000 apysc-4.4.2/apysc/_material_design/icon/material_cancel_presentation_outlined_icon.py
--rw-r--r--   0 runner    (1001) docker     (127)     1519 2024-05-23 14:23:55.000000 apysc-4.4.2/apysc/_material_design/icon/material_cancel_schedule_send_icon.py
--rw-r--r--   0 runner    (1001) docker     (127)     1688 2024-05-23 14:23:55.000000 apysc-4.4.2/apysc/_material_design/icon/material_cancel_schedule_send_outlined_icon.py
--rw-r--r--   0 runner    (1001) docker     (127)     1487 2024-05-23 14:23:55.000000 apysc-4.4.2/apysc/_material_design/icon/material_card_giftcard_icon.py
--rw-r--r--   0 runner    (1001) docker     (127)     1500 2024-05-23 14:23:55.000000 apysc-4.4.2/apysc/_material_design/icon/material_card_giftcard_outlined_icon.py
--rw-r--r--   0 runner    (1001) docker     (127)     1185 2024-05-23 14:23:55.000000 apysc-4.4.2/apysc/_material_design/icon/material_card_membership_icon.py
--rw-r--r--   0 runner    (1001) docker     (127)     1213 2024-05-23 14:23:55.000000 apysc-4.4.2/apysc/_material_design/icon/material_card_membership_outlined_icon.py
--rw-r--r--   0 runner    (1001) docker     (127)     1232 2024-05-23 14:23:55.000000 apysc-4.4.2/apysc/_material_design/icon/material_card_travel_icon.py
--rw-r--r--   0 runner    (1001) docker     (127)     1260 2024-05-23 14:23:55.000000 apysc-4.4.2/apysc/_material_design/icon/material_card_travel_outlined_icon.py
--rw-r--r--   0 runner    (1001) docker     (127)     1378 2024-05-23 14:23:55.000000 apysc-4.4.2/apysc/_material_design/icon/material_cell_wifi_icon.py
--rw-r--r--   0 runner    (1001) docker     (127)     1105 2024-05-23 14:23:55.000000 apysc-4.4.2/apysc/_material_design/icon/material_change_history_icon.py
--rw-r--r--   0 runner    (1001) docker     (127)     1131 2024-05-23 14:23:55.000000 apysc-4.4.2/apysc/_material_design/icon/material_change_history_outlined_icon.py
--rw-r--r--   0 runner    (1001) docker     (127)     1111 2024-05-23 14:23:55.000000 apysc-4.4.2/apysc/_material_design/icon/material_chat_bubble_icon.py
--rw-r--r--   0 runner    (1001) docker     (127)     1157 2024-05-23 14:23:55.000000 apysc-4.4.2/apysc/_material_design/icon/material_chat_bubble_outline_icon.py
--rw-r--r--   0 runner    (1001) docker     (127)     1183 2024-05-23 14:23:55.000000 apysc-4.4.2/apysc/_material_design/icon/material_chat_bubble_outline_outlined_icon.py
--rw-r--r--   0 runner    (1001) docker     (127)     1139 2024-05-23 14:23:55.000000 apysc-4.4.2/apysc/_material_design/icon/material_chat_bubble_outlined_icon.py
--rw-r--r--   0 runner    (1001) docker     (127)     1140 2024-05-23 14:23:55.000000 apysc-4.4.2/apysc/_material_design/icon/material_chat_icon.py
--rw-r--r--   0 runner    (1001) docker     (127)     1193 2024-05-23 14:23:55.000000 apysc-4.4.2/apysc/_material_design/icon/material_chat_outlined_icon.py
--rw-r--r--   0 runner    (1001) docker     (127)     1165 2024-05-23 14:23:55.000000 apysc-4.4.2/apysc/_material_design/icon/material_check_circle_icon.py
--rw-r--r--   0 runner    (1001) docker     (127)     1257 2024-05-23 14:23:55.000000 apysc-4.4.2/apysc/_material_design/icon/material_check_circle_outline_icon.py
--rw-r--r--   0 runner    (1001) docker     (127)     1268 2024-05-23 14:23:55.000000 apysc-4.4.2/apysc/_material_design/icon/material_check_circle_outline_outlined_icon.py
--rw-r--r--   0 runner    (1001) docker     (127)     1245 2024-05-23 14:23:55.000000 apysc-4.4.2/apysc/_material_design/icon/material_check_circle_outlined_icon.py
--rw-r--r--   0 runner    (1001) docker     (127)     1239 2024-05-23 14:23:55.000000 apysc-4.4.2/apysc/_material_design/icon/material_chrome_reader_mode_icon.py
--rw-r--r--   0 runner    (1001) docker     (127)     1247 2024-05-23 14:23:55.000000 apysc-4.4.2/apysc/_material_design/icon/material_chrome_reader_mode_outlined_icon.py
--rw-r--r--   0 runner    (1001) docker     (127)     1299 2024-05-23 14:23:55.000000 apysc-4.4.2/apysc/_material_design/icon/material_circle_notifications_icon.py
--rw-r--r--   0 runner    (1001) docker     (127)     1129 2024-05-23 14:23:55.000000 apysc-4.4.2/apysc/_material_design/icon/material_class_icon.py
--rw-r--r--   0 runner    (1001) docker     (127)     1188 2024-05-23 14:23:55.000000 apysc-4.4.2/apysc/_material_design/icon/material_class_outlined_icon.py
--rw-r--r--   0 runner    (1001) docker     (127)     1085 2024-05-23 14:23:55.000000 apysc-4.4.2/apysc/_material_design/icon/material_clear_all_icon.py
--rw-r--r--   0 runner    (1001) docker     (127)     1113 2024-05-23 14:23:55.000000 apysc-4.4.2/apysc/_material_design/icon/material_clear_all_outlined_icon.py
--rw-r--r--   0 runner    (1001) docker     (127)     1129 2024-05-23 14:23:55.000000 apysc-4.4.2/apysc/_material_design/icon/material_clear_icon.py
--rw-r--r--   0 runner    (1001) docker     (127)     1165 2024-05-23 14:23:55.000000 apysc-4.4.2/apysc/_material_design/icon/material_clear_outlined_icon.py
--rw-r--r--   0 runner    (1001) docker     (127)     1213 2024-05-23 14:23:55.000000 apysc-4.4.2/apysc/_material_design/icon/material_close_fullscreen_icon.py
--rw-r--r--   0 runner    (1001) docker     (127)     1239 2024-05-23 14:23:55.000000 apysc-4.4.2/apysc/_material_design/icon/material_close_fullscreen_outlined_icon.py
--rw-r--r--   0 runner    (1001) docker     (127)     1544 2024-05-23 14:23:55.000000 apysc-4.4.2/apysc/_material_design/icon/material_closed_caption_disabled_icon.py
--rw-r--r--   0 runner    (1001) docker     (127)     1623 2024-05-23 14:23:55.000000 apysc-4.4.2/apysc/_material_design/icon/material_closed_caption_disabled_outlined_icon.py
--rw-r--r--   0 runner    (1001) docker     (127)     1337 2024-05-23 14:23:55.000000 apysc-4.4.2/apysc/_material_design/icon/material_closed_caption_icon.py
--rw-r--r--   0 runner    (1001) docker     (127)     1374 2024-05-23 14:23:55.000000 apysc-4.4.2/apysc/_material_design/icon/material_closed_caption_off_icon.py
--rw-r--r--   0 runner    (1001) docker     (127)     1383 2024-05-23 14:23:55.000000 apysc-4.4.2/apysc/_material_design/icon/material_closed_caption_outlined_icon.py
--rw-r--r--   0 runner    (1001) docker     (127)     1117 2024-05-23 14:23:55.000000 apysc-4.4.2/apysc/_material_design/icon/material_code_icon.py
--rw-r--r--   0 runner    (1001) docker     (127)     1143 2024-05-23 14:23:55.000000 apysc-4.4.2/apysc/_material_design/icon/material_code_outlined_icon.py
--rw-r--r--   0 runner    (1001) docker     (127)     1202 2024-05-23 14:23:55.000000 apysc-4.4.2/apysc/_material_design/icon/material_comment_bank_icon.py
--rw-r--r--   0 runner    (1001) docker     (127)     1279 2024-05-23 14:23:55.000000 apysc-4.4.2/apysc/_material_design/icon/material_comment_bank_outlined_icon.py
--rw-r--r--   0 runner    (1001) docker     (127)     1156 2024-05-23 14:23:55.000000 apysc-4.4.2/apysc/_material_design/icon/material_comment_icon.py
--rw-r--r--   0 runner    (1001) docker     (127)     1204 2024-05-23 14:23:55.000000 apysc-4.4.2/apysc/_material_design/icon/material_comment_outlined_icon.py
--rw-r--r--   0 runner    (1001) docker     (127)     1537 2024-05-23 14:23:55.000000 apysc-4.4.2/apysc/_material_design/icon/material_commute_icon.py
--rw-r--r--   0 runner    (1001) docker     (127)     1551 2024-05-23 14:23:55.000000 apysc-4.4.2/apysc/_material_design/icon/material_commute_outlined_icon.py
--rw-r--r--   0 runner    (1001) docker     (127)     1205 2024-05-23 14:23:55.000000 apysc-4.4.2/apysc/_material_design/icon/material_compare_arrows_icon.py
--rw-r--r--   0 runner    (1001) docker     (127)     1154 2024-05-23 14:23:55.000000 apysc-4.4.2/apysc/_material_design/icon/material_compare_arrows_outlined_icon.py
--rw-r--r--   0 runner    (1001) docker     (127)     1167 2024-05-23 14:23:55.000000 apysc-4.4.2/apysc/_material_design/icon/material_compress_icon.py
--rw-r--r--   0 runner    (1001) docker     (127)     1307 2024-05-23 14:23:55.000000 apysc-4.4.2/apysc/_material_design/icon/material_contact_mail_icon.py
--rw-r--r--   0 runner    (1001) docker     (127)     1446 2024-05-23 14:23:55.000000 apysc-4.4.2/apysc/_material_design/icon/material_contact_mail_outlined_icon.py
--rw-r--r--   0 runner    (1001) docker     (127)     1360 2024-05-23 14:23:55.000000 apysc-4.4.2/apysc/_material_design/icon/material_contact_page_icon.py
--rw-r--r--   0 runner    (1001) docker     (127)     1422 2024-05-23 14:23:55.000000 apysc-4.4.2/apysc/_material_design/icon/material_contact_page_outlined_icon.py
--rw-r--r--   0 runner    (1001) docker     (127)     1413 2024-05-23 14:23:55.000000 apysc-4.4.2/apysc/_material_design/icon/material_contact_phone_icon.py
--rw-r--r--   0 runner    (1001) docker     (127)     1580 2024-05-23 14:23:55.000000 apysc-4.4.2/apysc/_material_design/icon/material_contact_phone_outlined_icon.py
--rw-r--r--   0 runner    (1001) docker     (127)     1268 2024-05-23 14:23:55.000000 apysc-4.4.2/apysc/_material_design/icon/material_contact_support_icon.py
--rw-r--r--   0 runner    (1001) docker     (127)     1409 2024-05-23 14:23:55.000000 apysc-4.4.2/apysc/_material_design/icon/material_contact_support_outlined_icon.py
--rw-r--r--   0 runner    (1001) docker     (127)     1643 2024-05-23 14:23:55.000000 apysc-4.4.2/apysc/_material_design/icon/material_contactless_icon.py
--rw-r--r--   0 runner    (1001) docker     (127)     1751 2024-05-23 14:23:55.000000 apysc-4.4.2/apysc/_material_design/icon/material_contactless_outlined_icon.py
--rw-r--r--   0 runner    (1001) docker     (127)     1315 2024-05-23 14:23:55.000000 apysc-4.4.2/apysc/_material_design/icon/material_contacts_icon.py
--rw-r--r--   0 runner    (1001) docker     (127)     1426 2024-05-23 14:23:55.000000 apysc-4.4.2/apysc/_material_design/icon/material_contacts_outlined_icon.py
--rw-r--r--   0 runner    (1001) docker     (127)     1175 2024-05-23 14:23:55.000000 apysc-4.4.2/apysc/_material_design/icon/material_content_copy_icon.py
--rw-r--r--   0 runner    (1001) docker     (127)     1203 2024-05-23 14:23:55.000000 apysc-4.4.2/apysc/_material_design/icon/material_content_copy_outlined_icon.py
--rw-r--r--   0 runner    (1001) docker     (127)     1582 2024-05-23 14:23:55.000000 apysc-4.4.2/apysc/_material_design/icon/material_content_cut_icon.py
--rw-r--r--   0 runner    (1001) docker     (127)     1486 2024-05-23 14:23:55.000000 apysc-4.4.2/apysc/_material_design/icon/material_content_cut_outlined_icon.py
--rw-r--r--   0 runner    (1001) docker     (127)     1251 2024-05-23 14:23:55.000000 apysc-4.4.2/apysc/_material_design/icon/material_content_paste_icon.py
--rw-r--r--   0 runner    (1001) docker     (127)     1272 2024-05-23 14:23:55.000000 apysc-4.4.2/apysc/_material_design/icon/material_content_paste_outlined_icon.py
--rw-r--r--   0 runner    (1001) docker     (127)     1304 2024-05-23 14:23:55.000000 apysc-4.4.2/apysc/_material_design/icon/material_control_camera_icon.py
--rw-r--r--   0 runner    (1001) docker     (127)     1332 2024-05-23 14:23:55.000000 apysc-4.4.2/apysc/_material_design/icon/material_control_camera_outlined_icon.py
--rw-r--r--   0 runner    (1001) docker     (127)     1498 2024-05-23 14:23:55.000000 apysc-4.4.2/apysc/_material_design/icon/material_copyright_icon.py
--rw-r--r--   0 runner    (1001) docker     (127)     1793 2024-05-23 14:23:55.000000 apysc-4.4.2/apysc/_material_design/icon/material_copyright_outlined_icon.py
--rw-r--r--   0 runner    (1001) docker     (127)     1180 2024-05-23 14:23:55.000000 apysc-4.4.2/apysc/_material_design/icon/material_create_icon.py
--rw-r--r--   0 runner    (1001) docker     (127)     1259 2024-05-23 14:23:55.000000 apysc-4.4.2/apysc/_material_design/icon/material_create_outlined_icon.py
--rw-r--r--   0 runner    (1001) docker     (127)     1167 2024-05-23 14:23:55.000000 apysc-4.4.2/apysc/_material_design/icon/material_credit_card_icon.py
--rw-r--r--   0 runner    (1001) docker     (127)     1195 2024-05-23 14:23:55.000000 apysc-4.4.2/apysc/_material_design/icon/material_credit_card_outlined_icon.py
--rw-r--r--   0 runner    (1001) docker     (127)     1211 2024-05-23 14:23:55.000000 apysc-4.4.2/apysc/_material_design/icon/material_dangerous_icon.py
--rw-r--r--   0 runner    (1001) docker     (127)     1138 2024-05-23 14:23:55.000000 apysc-4.4.2/apysc/_material_design/icon/material_dashboard_customize_icon.py
--rw-r--r--   0 runner    (1001) docker     (127)     1101 2024-05-23 14:23:55.000000 apysc-4.4.2/apysc/_material_design/icon/material_dashboard_icon.py
--rw-r--r--   0 runner    (1001) docker     (127)     1186 2024-05-23 14:23:55.000000 apysc-4.4.2/apysc/_material_design/icon/material_dashboard_outlined_icon.py
--rw-r--r--   0 runner    (1001) docker     (127)     1205 2024-05-23 14:23:55.000000 apysc-4.4.2/apysc/_material_design/icon/material_date_range_icon.py
--rw-r--r--   0 runner    (1001) docker     (127)     1250 2024-05-23 14:23:55.000000 apysc-4.4.2/apysc/_material_design/icon/material_date_range_outlined_icon.py
--rw-r--r--   0 runner    (1001) docker     (127)     1296 2024-05-23 14:23:55.000000 apysc-4.4.2/apysc/_material_design/icon/material_delete_forever_icon.py
--rw-r--r--   0 runner    (1001) docker     (127)     1291 2024-05-23 14:23:55.000000 apysc-4.4.2/apysc/_material_design/icon/material_delete_forever_outlined_icon.py
--rw-r--r--   0 runner    (1001) docker     (127)     1108 2024-05-23 14:23:55.000000 apysc-4.4.2/apysc/_material_design/icon/material_delete_icon.py
--rw-r--r--   0 runner    (1001) docker     (127)     1143 2024-05-23 14:23:55.000000 apysc-4.4.2/apysc/_material_design/icon/material_delete_outline_icon.py
--rw-r--r--   0 runner    (1001) docker     (127)     1174 2024-05-23 14:23:55.000000 apysc-4.4.2/apysc/_material_design/icon/material_delete_outline_outlined_icon.py
--rw-r--r--   0 runner    (1001) docker     (127)     1152 2024-05-23 14:23:55.000000 apysc-4.4.2/apysc/_material_design/icon/material_delete_outlined_icon.py
--rw-r--r--   0 runner    (1001) docker     (127)     1157 2024-05-23 14:23:55.000000 apysc-4.4.2/apysc/_material_design/icon/material_delete_sweep_icon.py
--rw-r--r--   0 runner    (1001) docker     (127)     1195 2024-05-23 14:23:55.000000 apysc-4.4.2/apysc/_material_design/icon/material_delete_sweep_outlined_icon.py
--rw-r--r--   0 runner    (1001) docker     (127)     1172 2024-05-23 14:23:55.000000 apysc-4.4.2/apysc/_material_design/icon/material_description_icon.py
--rw-r--r--   0 runner    (1001) docker     (127)     1186 2024-05-23 14:23:55.000000 apysc-4.4.2/apysc/_material_design/icon/material_description_outlined_icon.py
--rw-r--r--   0 runner    (1001) docker     (127)     1265 2024-05-23 14:23:55.000000 apysc-4.4.2/apysc/_material_design/icon/material_desktop_access_disabled_icon.py
--rw-r--r--   0 runner    (1001) docker     (127)     1295 2024-05-23 14:23:55.000000 apysc-4.4.2/apysc/_material_design/icon/material_desktop_access_disabled_outlined_icon.py
--rw-r--r--   0 runner    (1001) docker     (127)     1365 2024-05-23 14:23:55.000000 apysc-4.4.2/apysc/_material_design/icon/material_dialer_sip_icon.py
--rw-r--r--   0 runner    (1001) docker     (127)     1549 2024-05-23 14:23:55.000000 apysc-4.4.2/apysc/_material_design/icon/material_dialer_sip_outlined_icon.py
--rw-r--r--   0 runner    (1001) docker     (127)     1519 2024-05-23 14:23:55.000000 apysc-4.4.2/apysc/_material_design/icon/material_dialpad_icon.py
--rw-r--r--   0 runner    (1001) docker     (127)     1547 2024-05-23 14:23:55.000000 apysc-4.4.2/apysc/_material_design/icon/material_dialpad_outlined_icon.py
--rw-r--r--   0 runner    (1001) docker     (127)     1234 2024-05-23 14:23:55.000000 apysc-4.4.2/apysc/_material_design/icon/material_disabled_by_default_icon.py
--rw-r--r--   0 runner    (1001) docker     (127)     1278 2024-05-23 14:23:55.000000 apysc-4.4.2/apysc/_material_design/icon/material_disabled_by_default_outlined_icon.py
--rw-r--r--   0 runner    (1001) docker     (127)     1279 2024-05-23 14:23:55.000000 apysc-4.4.2/apysc/_material_design/icon/material_dns_icon.py
--rw-r--r--   0 runner    (1001) docker     (127)     1390 2024-05-23 14:23:55.000000 apysc-4.4.2/apysc/_material_design/icon/material_dns_outlined_icon.py
--rw-r--r--   0 runner    (1001) docker     (127)     1268 2024-05-23 14:23:55.000000 apysc-4.4.2/apysc/_material_design/icon/material_domain_disabled_icon.py
--rw-r--r--   0 runner    (1001) docker     (127)     1295 2024-05-23 14:23:55.000000 apysc-4.4.2/apysc/_material_design/icon/material_domain_disabled_outlined_icon.py
--rw-r--r--   0 runner    (1001) docker     (127)     1316 2024-05-23 14:23:55.000000 apysc-4.4.2/apysc/_material_design/icon/material_domain_verification_icon.py
--rw-r--r--   0 runner    (1001) docker     (127)     1342 2024-05-23 14:23:55.000000 apysc-4.4.2/apysc/_material_design/icon/material_domain_verification_outlined_icon.py
--rw-r--r--   0 runner    (1001) docker     (127)     1189 2024-05-23 14:23:55.000000 apysc-4.4.2/apysc/_material_design/icon/material_done_all_icon.py
--rw-r--r--   0 runner    (1001) docker     (127)     1217 2024-05-23 14:23:55.000000 apysc-4.4.2/apysc/_material_design/icon/material_done_all_outlined_icon.py
--rw-r--r--   0 runner    (1001) docker     (127)     1075 2024-05-23 14:23:55.000000 apysc-4.4.2/apysc/_material_design/icon/material_done_icon.py
--rw-r--r--   0 runner    (1001) docker     (127)     1178 2024-05-23 14:23:55.000000 apysc-4.4.2/apysc/_material_design/icon/material_done_outline_icon.py
--rw-r--r--   0 runner    (1001) docker     (127)     1206 2024-05-23 14:23:55.000000 apysc-4.4.2/apysc/_material_design/icon/material_done_outline_outlined_icon.py
--rw-r--r--   0 runner    (1001) docker     (127)     1103 2024-05-23 14:23:55.000000 apysc-4.4.2/apysc/_material_design/icon/material_done_outlined_icon.py
--rw-r--r--   0 runner    (1001) docker     (127)     1323 2024-05-23 14:23:55.000000 apysc-4.4.2/apysc/_material_design/icon/material_donut_large_icon.py
--rw-r--r--   0 runner    (1001) docker     (127)     1337 2024-05-23 14:23:55.000000 apysc-4.4.2/apysc/_material_design/icon/material_donut_large_outlined_icon.py
--rw-r--r--   0 runner    (1001) docker     (127)     1254 2024-05-23 14:23:55.000000 apysc-4.4.2/apysc/_material_design/icon/material_donut_small_icon.py
--rw-r--r--   0 runner    (1001) docker     (127)     1573 2024-05-23 14:23:55.000000 apysc-4.4.2/apysc/_material_design/icon/material_donut_small_outlined_icon.py
--rw-r--r--   0 runner    (1001) docker     (127)     1179 2024-05-23 14:23:55.000000 apysc-4.4.2/apysc/_material_design/icon/material_drafts_icon.py
--rw-r--r--   0 runner    (1001) docker     (127)     1241 2024-05-23 14:23:55.000000 apysc-4.4.2/apysc/_material_design/icon/material_drafts_outlined_icon.py
--rw-r--r--   0 runner    (1001) docker     (127)     1347 2024-05-23 14:23:55.000000 apysc-4.4.2/apysc/_material_design/icon/material_drag_indicator_icon.py
--rw-r--r--   0 runner    (1001) docker     (127)     1373 2024-05-23 14:23:55.000000 apysc-4.4.2/apysc/_material_design/icon/material_drag_indicator_outlined_icon.py
--rw-r--r--   0 runner    (1001) docker     (127)     1146 2024-05-23 14:23:55.000000 apysc-4.4.2/apysc/_material_design/icon/material_duo_icon.py
--rw-r--r--   0 runner    (1001) docker     (127)     1174 2024-05-23 14:23:55.000000 apysc-4.4.2/apysc/_material_design/icon/material_duo_outlined_icon.py
--rw-r--r--   0 runner    (1001) docker     (127)     1581 2024-05-23 14:23:55.000000 apysc-4.4.2/apysc/_material_design/icon/material_dynamic_feed_icon.py
--rw-r--r--   0 runner    (1001) docker     (127)     1607 2024-05-23 14:23:55.000000 apysc-4.4.2/apysc/_material_design/icon/material_dynamic_feed_outlined_icon.py
--rw-r--r--   0 runner    (1001) docker     (127)     1286 2024-05-23 14:23:55.000000 apysc-4.4.2/apysc/_material_design/icon/material_dynamic_form_icon.py
--rw-r--r--   0 runner    (1001) docker     (127)     1344 2024-05-23 14:23:55.000000 apysc-4.4.2/apysc/_material_design/icon/material_dynamic_form_outlined_icon.py
--rw-r--r--   0 runner    (1001) docker     (127)     1255 2024-05-23 14:23:55.000000 apysc-4.4.2/apysc/_material_design/icon/material_eco_icon.py
--rw-r--r--   0 runner    (1001) docker     (127)     1451 2024-05-23 14:23:55.000000 apysc-4.4.2/apysc/_material_design/icon/material_eco_outlined_icon.py
--rw-r--r--   0 runner    (1001) docker     (127)     1275 2024-05-23 14:23:55.000000 apysc-4.4.2/apysc/_material_design/icon/material_edit_off_icon.py
--rw-r--r--   0 runner    (1001) docker     (127)     1064 2024-05-23 14:23:55.000000 apysc-4.4.2/apysc/_material_design/icon/material_eject_icon.py
--rw-r--r--   0 runner    (1001) docker     (127)     1122 2024-05-23 14:23:55.000000 apysc-4.4.2/apysc/_material_design/icon/material_eject_outlined_icon.py
--rw-r--r--   0 runner    (1001) docker     (127)     1137 2024-05-23 14:23:55.000000 apysc-4.4.2/apysc/_material_design/icon/material_email_icon.py
--rw-r--r--   0 runner    (1001) docker     (127)     1171 2024-05-23 14:23:55.000000 apysc-4.4.2/apysc/_material_design/icon/material_email_outlined_icon.py
--rw-r--r--   0 runner    (1001) docker     (127)     1088 2024-05-23 14:23:55.000000 apysc-4.4.2/apysc/_material_design/icon/material_equalizer_icon.py
--rw-r--r--   0 runner    (1001) docker     (127)     1116 2024-05-23 14:23:55.000000 apysc-4.4.2/apysc/_material_design/icon/material_equalizer_outlined_icon.py
--rw-r--r--   0 runner    (1001) docker     (127)     1124 2024-05-23 14:23:55.000000 apysc-4.4.2/apysc/_material_design/icon/material_error_icon.py
--rw-r--r--   0 runner    (1001) docker     (127)     1220 2024-05-23 14:23:55.000000 apysc-4.4.2/apysc/_material_design/icon/material_error_outline_icon.py
--rw-r--r--   0 runner    (1001) docker     (127)     1212 2024-05-23 14:23:55.000000 apysc-4.4.2/apysc/_material_design/icon/material_error_outline_outlined_icon.py
--rw-r--r--   0 runner    (1001) docker     (127)     1113 2024-05-23 14:23:55.000000 apysc-4.4.2/apysc/_material_design/icon/material_error_outlined_icon.py
--rw-r--r--   0 runner    (1001) docker     (127)     1386 2024-05-23 14:23:55.000000 apysc-4.4.2/apysc/_material_design/icon/material_euro_symbol_icon.py
--rw-r--r--   0 runner    (1001) docker     (127)     1409 2024-05-23 14:23:55.000000 apysc-4.4.2/apysc/_material_design/icon/material_euro_symbol_outlined_icon.py
--rw-r--r--   0 runner    (1001) docker     (127)     1164 2024-05-23 14:23:55.000000 apysc-4.4.2/apysc/_material_design/icon/material_event_icon.py
--rw-r--r--   0 runner    (1001) docker     (127)     1204 2024-05-23 14:23:55.000000 apysc-4.4.2/apysc/_material_design/icon/material_event_outlined_icon.py
--rw-r--r--   0 runner    (1001) docker     (127)     1226 2024-05-23 14:23:55.000000 apysc-4.4.2/apysc/_material_design/icon/material_event_seat_icon.py
--rw-r--r--   0 runner    (1001) docker     (127)     1183 2024-05-23 14:23:55.000000 apysc-4.4.2/apysc/_material_design/icon/material_event_seat_outlined_icon.py
--rw-r--r--   0 runner    (1001) docker     (127)     1208 2024-05-23 14:23:55.000000 apysc-4.4.2/apysc/_material_design/icon/material_exit_to_app_icon.py
--rw-r--r--   0 runner    (1001) docker     (127)     1236 2024-05-23 14:23:55.000000 apysc-4.4.2/apysc/_material_design/icon/material_exit_to_app_outlined_icon.py
--rw-r--r--   0 runner    (1001) docker     (127)     1128 2024-05-23 14:23:55.000000 apysc-4.4.2/apysc/_material_design/icon/material_expand_icon.py
--rw-r--r--   0 runner    (1001) docker     (127)     1145 2024-05-23 14:23:55.000000 apysc-4.4.2/apysc/_material_design/icon/material_explicit_icon.py
--rw-r--r--   0 runner    (1001) docker     (127)     1190 2024-05-23 14:23:55.000000 apysc-4.4.2/apysc/_material_design/icon/material_explicit_outlined_icon.py
--rw-r--r--   0 runner    (1001) docker     (127)     1229 2024-05-23 14:23:55.000000 apysc-4.4.2/apysc/_material_design/icon/material_explore_icon.py
--rw-r--r--   0 runner    (1001) docker     (127)     2205 2024-05-23 14:23:55.000000 apysc-4.4.2/apysc/_material_design/icon/material_explore_off_icon.py
--rw-r--r--   0 runner    (1001) docker     (127)     1528 2024-05-23 14:23:55.000000 apysc-4.4.2/apysc/_material_design/icon/material_explore_off_outlined_icon.py
--rw-r--r--   0 runner    (1001) docker     (127)     1312 2024-05-23 14:23:55.000000 apysc-4.4.2/apysc/_material_design/icon/material_explore_outlined_icon.py
--rw-r--r--   0 runner    (1001) docker     (127)     1332 2024-05-23 14:23:55.000000 apysc-4.4.2/apysc/_material_design/icon/material_extension_icon.py
--rw-r--r--   0 runner    (1001) docker     (127)     1536 2024-05-23 14:23:55.000000 apysc-4.4.2/apysc/_material_design/icon/material_extension_outlined_icon.py
--rw-r--r--   0 runner    (1001) docker     (127)     1437 2024-05-23 14:23:55.000000 apysc-4.4.2/apysc/_material_design/icon/material_face_icon.py
--rw-r--r--   0 runner    (1001) docker     (127)     1631 2024-05-23 14:23:55.000000 apysc-4.4.2/apysc/_material_design/icon/material_face_outlined_icon.py
--rw-r--r--   0 runner    (1001) docker     (127)     1651 2024-05-23 14:23:55.000000 apysc-4.4.2/apysc/_material_design/icon/material_face_unlock_outlined_icon.py
--rw-r--r--   0 runner    (1001) docker     (127)     1325 2024-05-23 14:23:55.000000 apysc-4.4.2/apysc/_material_design/icon/material_fact_check_icon.py
--rw-r--r--   0 runner    (1001) docker     (127)     1533 2024-05-23 14:23:55.000000 apysc-4.4.2/apysc/_material_design/icon/material_fact_check_outlined_icon.py
--rw-r--r--   0 runner    (1001) docker     (127)     1087 2024-05-23 14:23:55.000000 apysc-4.4.2/apysc/_material_design/icon/material_fast_forward_icon.py
--rw-r--r--   0 runner    (1001) docker     (127)     1324 2024-05-23 14:23:55.000000 apysc-4.4.2/apysc/_material_design/icon/material_fast_forward_outlined_icon.py
--rw-r--r--   0 runner    (1001) docker     (127)     1088 2024-05-23 14:23:55.000000 apysc-4.4.2/apysc/_material_design/icon/material_fast_rewind_icon.py
--rw-r--r--   0 runner    (1001) docker     (127)     1170 2024-05-23 14:23:55.000000 apysc-4.4.2/apysc/_material_design/icon/material_fast_rewind_outlined_icon.py
--rw-r--r--   0 runner    (1001) docker     (127)     1400 2024-05-23 14:23:55.000000 apysc-4.4.2/apysc/_material_design/icon/material_favorite_border_icon.py
--rw-r--r--   0 runner    (1001) docker     (127)     1428 2024-05-23 14:23:55.000000 apysc-4.4.2/apysc/_material_design/icon/material_favorite_border_outlined_icon.py
--rw-r--r--   0 runner    (1001) docker     (127)     1211 2024-05-23 14:23:55.000000 apysc-4.4.2/apysc/_material_design/icon/material_favorite_icon.py
--rw-r--r--   0 runner    (1001) docker     (127)     1239 2024-05-23 14:23:55.000000 apysc-4.4.2/apysc/_material_design/icon/material_favorite_outlined_icon.py
--rw-r--r--   0 runner    (1001) docker     (127)     1170 2024-05-23 14:23:55.000000 apysc-4.4.2/apysc/_material_design/icon/material_featured_play_list_icon.py
--rw-r--r--   0 runner    (1001) docker     (127)     1208 2024-05-23 14:23:55.000000 apysc-4.4.2/apysc/_material_design/icon/material_featured_play_list_outlined_icon.py
--rw-r--r--   0 runner    (1001) docker     (127)     1146 2024-05-23 14:23:55.000000 apysc-4.4.2/apysc/_material_design/icon/material_featured_video_icon.py
--rw-r--r--   0 runner    (1001) docker     (127)     1185 2024-05-23 14:23:55.000000 apysc-4.4.2/apysc/_material_design/icon/material_featured_video_outlined_icon.py
--rw-r--r--   0 runner    (1001) docker     (127)     1141 2024-05-23 14:23:55.000000 apysc-4.4.2/apysc/_material_design/icon/material_feedback_icon.py
--rw-r--r--   0 runner    (1001) docker     (127)     1197 2024-05-23 14:23:55.000000 apysc-4.4.2/apysc/_material_design/icon/material_feedback_outlined_icon.py
--rw-r--r--   0 runner    (1001) docker     (127)     1467 2024-05-23 14:23:55.000000 apysc-4.4.2/apysc/_material_design/icon/material_fiber_dvr_icon.py
--rw-r--r--   0 runner    (1001) docker     (127)     1297 2024-05-23 14:23:55.000000 apysc-4.4.2/apysc/_material_design/icon/material_fiber_dvr_outlined_icon.py
--rw-r--r--   0 runner    (1001) docker     (127)     1091 2024-05-23 14:23:55.000000 apysc-4.4.2/apysc/_material_design/icon/material_fiber_manual_record_icon.py
--rw-r--r--   0 runner    (1001) docker     (127)     1210 2024-05-23 14:23:55.000000 apysc-4.4.2/apysc/_material_design/icon/material_fiber_manual_record_outlined_icon.py
--rw-r--r--   0 runner    (1001) docker     (127)     1422 2024-05-23 14:23:55.000000 apysc-4.4.2/apysc/_material_design/icon/material_fiber_new_icon.py
--rw-r--r--   0 runner    (1001) docker     (127)     1262 2024-05-23 14:23:55.000000 apysc-4.4.2/apysc/_material_design/icon/material_fiber_new_outlined_icon.py
--rw-r--r--   0 runner    (1001) docker     (127)     1283 2024-05-23 14:23:55.000000 apysc-4.4.2/apysc/_material_design/icon/material_fiber_pin_icon.py
--rw-r--r--   0 runner    (1001) docker     (127)     1221 2024-05-23 14:23:55.000000 apysc-4.4.2/apysc/_material_design/icon/material_fiber_pin_outlined_icon.py
--rw-r--r--   0 runner    (1001) docker     (127)     1206 2024-05-23 14:23:55.000000 apysc-4.4.2/apysc/_material_design/icon/material_fiber_smart_record_icon.py
--rw-r--r--   0 runner    (1001) docker     (127)     1314 2024-05-23 14:23:55.000000 apysc-4.4.2/apysc/_material_design/icon/material_fiber_smart_record_outlined_icon.py
--rw-r--r--   0 runner    (1001) docker     (127)     1175 2024-05-23 14:23:55.000000 apysc-4.4.2/apysc/_material_design/icon/material_file_copy_icon.py
--rw-r--r--   0 runner    (1001) docker     (127)     1199 2024-05-23 14:23:55.000000 apysc-4.4.2/apysc/_material_design/icon/material_file_copy_outlined_icon.py
--rw-r--r--   0 runner    (1001) docker     (127)     1304 2024-05-23 14:23:55.000000 apysc-4.4.2/apysc/_material_design/icon/material_file_present_icon.py
--rw-r--r--   0 runner    (1001) docker     (127)     1283 2024-05-23 14:23:55.000000 apysc-4.4.2/apysc/_material_design/icon/material_filter_alt_icon.py
--rw-r--r--   0 runner    (1001) docker     (127)     1332 2024-05-23 14:23:55.000000 apysc-4.4.2/apysc/_material_design/icon/material_filter_alt_outlined_icon.py
--rw-r--r--   0 runner    (1001) docker     (127)     1286 2024-05-23 14:23:55.000000 apysc-4.4.2/apysc/_material_design/icon/material_filter_list_alt_icon.py
--rw-r--r--   0 runner    (1001) docker     (127)     1091 2024-05-23 14:23:55.000000 apysc-4.4.2/apysc/_material_design/icon/material_filter_list_icon.py
--rw-r--r--   0 runner    (1001) docker     (127)     1119 2024-05-23 14:23:55.000000 apysc-4.4.2/apysc/_material_design/icon/material_filter_list_outlined_icon.py
--rw-r--r--   0 runner    (1001) docker     (127)     1300 2024-05-23 14:23:55.000000 apysc-4.4.2/apysc/_material_design/icon/material_find_in_page_icon.py
--rw-r--r--   0 runner    (1001) docker     (127)     1528 2024-05-23 14:23:55.000000 apysc-4.4.2/apysc/_material_design/icon/material_find_in_page_outlined_icon.py
--rw-r--r--   0 runner    (1001) docker     (127)     1367 2024-05-23 14:23:55.000000 apysc-4.4.2/apysc/_material_design/icon/material_find_replace_icon.py
--rw-r--r--   0 runner    (1001) docker     (127)     1395 2024-05-23 14:23:55.000000 apysc-4.4.2/apysc/_material_design/icon/material_find_replace_outlined_icon.py
--rw-r--r--   0 runner    (1001) docker     (127)     2687 2024-05-23 14:23:55.000000 apysc-4.4.2/apysc/_material_design/icon/material_fingerprint_icon.py
--rw-r--r--   0 runner    (1001) docker     (127)     2703 2024-05-23 14:23:55.000000 apysc-4.4.2/apysc/_material_design/icon/material_fingerprint_outlined_icon.py
--rw-r--r--   0 runner    (1001) docker     (127)     1195 2024-05-23 14:23:55.000000 apysc-4.4.2/apysc/_material_design/icon/material_fit_screen_icon.py
--rw-r--r--   0 runner    (1001) docker     (127)     1061 2024-05-23 14:23:55.000000 apysc-4.4.2/apysc/_material_design/icon/material_flag_icon.py
--rw-r--r--   0 runner    (1001) docker     (127)     1131 2024-05-23 14:23:55.000000 apysc-4.4.2/apysc/_material_design/icon/material_flag_outlined_icon.py
--rw-r--r--   0 runner    (1001) docker     (127)     1480 2024-05-23 14:23:55.000000 apysc-4.4.2/apysc/_material_design/icon/material_flaky_icon.py
--rw-r--r--   0 runner    (1001) docker     (127)     1506 2024-05-23 14:23:55.000000 apysc-4.4.2/apysc/_material_design/icon/material_flaky_outlined_icon.py
--rw-r--r--   0 runner    (1001) docker     (127)     1287 2024-05-23 14:23:55.000000 apysc-4.4.2/apysc/_material_design/icon/material_flight_land_icon.py
--rw-r--r--   0 runner    (1001) docker     (127)     1234 2024-05-23 14:23:55.000000 apysc-4.4.2/apysc/_material_design/icon/material_flight_land_outlined_icon.py
--rw-r--r--   0 runner    (1001) docker     (127)     1326 2024-05-23 14:23:55.000000 apysc-4.4.2/apysc/_material_design/icon/material_flight_takeoff_icon.py
--rw-r--r--   0 runner    (1001) docker     (127)     1254 2024-05-23 14:23:55.000000 apysc-4.4.2/apysc/_material_design/icon/material_flight_takeoff_outlined_icon.py
--rw-r--r--   0 runner    (1001) docker     (127)     1303 2024-05-23 14:23:55.000000 apysc-4.4.2/apysc/_material_design/icon/material_flip_to_back_icon.py
--rw-r--r--   0 runner    (1001) docker     (127)     1331 2024-05-23 14:23:55.000000 apysc-4.4.2/apysc/_material_design/icon/material_flip_to_back_outlined_icon.py
--rw-r--r--   0 runner    (1001) docker     (127)     1259 2024-05-23 14:23:55.000000 apysc-4.4.2/apysc/_material_design/icon/material_flip_to_front_icon.py
--rw-r--r--   0 runner    (1001) docker     (127)     1287 2024-05-23 14:23:55.000000 apysc-4.4.2/apysc/_material_design/icon/material_flip_to_front_outlined_icon.py
--rw-r--r--   0 runner    (1001) docker     (127)     1237 2024-05-23 14:23:55.000000 apysc-4.4.2/apysc/_material_design/icon/material_font_download_icon.py
--rw-r--r--   0 runner    (1001) docker     (127)     1267 2024-05-23 14:23:55.000000 apysc-4.4.2/apysc/_material_design/icon/material_font_download_outlined_icon.py
--rw-r--r--   0 runner    (1001) docker     (127)     1152 2024-05-23 14:23:55.000000 apysc-4.4.2/apysc/_material_design/icon/material_forum_icon.py
--rw-r--r--   0 runner    (1001) docker     (127)     1203 2024-05-23 14:23:55.000000 apysc-4.4.2/apysc/_material_design/icon/material_forum_outlined_icon.py
--rw-r--r--   0 runner    (1001) docker     (127)     1601 2024-05-23 14:23:55.000000 apysc-4.4.2/apysc/_material_design/icon/material_forward_10_icon.py
--rw-r--r--   0 runner    (1001) docker     (127)     2167 2024-05-23 14:23:55.000000 apysc-4.4.2/apysc/_material_design/icon/material_forward_10_outlined_icon.py
--rw-r--r--   0 runner    (1001) docker     (127)     1878 2024-05-23 14:23:55.000000 apysc-4.4.2/apysc/_material_design/icon/material_forward_30_icon.py
--rw-r--r--   0 runner    (1001) docker     (127)     2407 2024-05-23 14:23:55.000000 apysc-4.4.2/apysc/_material_design/icon/material_forward_30_outlined_icon.py
--rw-r--r--   0 runner    (1001) docker     (127)     1528 2024-05-23 14:23:55.000000 apysc-4.4.2/apysc/_material_design/icon/material_forward_5_icon.py
--rw-r--r--   0 runner    (1001) docker     (127)     1699 2024-05-23 14:23:55.000000 apysc-4.4.2/apysc/_material_design/icon/material_forward_5_outlined_icon.py
--rw-r--r--   0 runner    (1001) docker     (127)     1057 2024-05-23 14:23:55.000000 apysc-4.4.2/apysc/_material_design/icon/material_forward_icon.py
--rw-r--r--   0 runner    (1001) docker     (127)     1127 2024-05-23 14:23:55.000000 apysc-4.4.2/apysc/_material_design/icon/material_forward_outlined_icon.py
--rw-r--r--   0 runner    (1001) docker     (127)     1243 2024-05-23 14:23:55.000000 apysc-4.4.2/apysc/_material_design/icon/material_forward_to_inbox_icon.py
--rw-r--r--   0 runner    (1001) docker     (127)     1269 2024-05-23 14:23:55.000000 apysc-4.4.2/apysc/_material_design/icon/material_forward_to_inbox_outlined_icon.py
--rw-r--r--   0 runner    (1001) docker     (127)     1624 2024-05-23 14:23:55.000000 apysc-4.4.2/apysc/_material_design/icon/material_g_translate_icon.py
--rw-r--r--   0 runner    (1001) docker     (127)     1726 2024-05-23 14:23:55.000000 apysc-4.4.2/apysc/_material_design/icon/material_g_translate_outlined_icon.py
--rw-r--r--   0 runner    (1001) docker     (127)     1129 2024-05-23 14:23:55.000000 apysc-4.4.2/apysc/_material_design/icon/material_games_icon.py
--rw-r--r--   0 runner    (1001) docker     (127)     1256 2024-05-23 14:23:55.000000 apysc-4.4.2/apysc/_material_design/icon/material_games_outlined_icon.py
--rw-r--r--   0 runner    (1001) docker     (127)     1455 2024-05-23 14:23:55.000000 apysc-4.4.2/apysc/_material_design/icon/material_gavel_icon.py
--rw-r--r--   0 runner    (1001) docker     (127)     1221 2024-05-23 14:23:55.000000 apysc-4.4.2/apysc/_material_design/icon/material_gavel_outlined_icon.py
--rw-r--r--   0 runner    (1001) docker     (127)     1687 2024-05-23 14:23:55.000000 apysc-4.4.2/apysc/_material_design/icon/material_gesture_icon.py
--rw-r--r--   0 runner    (1001) docker     (127)     1715 2024-05-23 14:23:55.000000 apysc-4.4.2/apysc/_material_design/icon/material_gesture_outlined_icon.py
--rw-r--r--   0 runner    (1001) docker     (127)     1074 2024-05-23 14:23:55.000000 apysc-4.4.2/apysc/_material_design/icon/material_get_app_icon.py
--rw-r--r--   0 runner    (1001) docker     (127)     1137 2024-05-23 14:23:55.000000 apysc-4.4.2/apysc/_material_design/icon/material_get_app_outlined_icon.py
--rw-r--r--   0 runner    (1001) docker     (127)     1322 2024-05-23 14:23:55.000000 apysc-4.4.2/apysc/_material_design/icon/material_gif_icon.py
--rw-r--r--   0 runner    (1001) docker     (127)     1198 2024-05-23 14:23:55.000000 apysc-4.4.2/apysc/_material_design/icon/material_gif_outlined_icon.py
--rw-r--r--   0 runner    (1001) docker     (127)     1116 2024-05-23 14:23:55.000000 apysc-4.4.2/apysc/_material_design/icon/material_grade_icon.py
--rw-r--r--   0 runner    (1001) docker     (127)     1324 2024-05-23 14:23:55.000000 apysc-4.4.2/apysc/_material_design/icon/material_grade_outlined_icon.py
--rw-r--r--   0 runner    (1001) docker     (127)     1242 2024-05-23 14:23:55.000000 apysc-4.4.2/apysc/_material_design/icon/material_grading_icon.py
--rw-r--r--   0 runner    (1001) docker     (127)     1268 2024-05-23 14:23:55.000000 apysc-4.4.2/apysc/_material_design/icon/material_grading_outlined_icon.py
--rw-r--r--   0 runner    (1001) docker     (127)     1357 2024-05-23 14:23:55.000000 apysc-4.4.2/apysc/_material_design/icon/material_group_work_icon.py
--rw-r--r--   0 runner    (1001) docker     (127)     1285 2024-05-23 14:23:55.000000 apysc-4.4.2/apysc/_material_design/icon/material_group_work_outlined_icon.py
--rw-r--r--   0 runner    (1001) docker     (127)     1202 2024-05-23 14:23:55.000000 apysc-4.4.2/apysc/_material_design/icon/material_hd_icon.py
--rw-r--r--   0 runner    (1001) docker     (127)     1247 2024-05-23 14:23:55.000000 apysc-4.4.2/apysc/_material_design/icon/material_hd_outlined_icon.py
--rw-r--r--   0 runner    (1001) docker     (127)     1909 2024-05-23 14:23:55.000000 apysc-4.4.2/apysc/_material_design/icon/material_hearing_disabled_icon.py
--rw-r--r--   0 runner    (1001) docker     (127)     1935 2024-05-23 14:23:55.000000 apysc-4.4.2/apysc/_material_design/icon/material_hearing_disabled_outlined_icon.py
--rw-r--r--   0 runner    (1001) docker     (127)     1585 2024-05-23 14:23:55.000000 apysc-4.4.2/apysc/_material_design/icon/material_hearing_icon.py
--rw-r--r--   0 runner    (1001) docker     (127)     1613 2024-05-23 14:23:55.000000 apysc-4.4.2/apysc/_material_design/icon/material_hearing_outlined_icon.py
--rw-r--r--   0 runner    (1001) docker     (127)     1589 2024-05-23 14:23:55.000000 apysc-4.4.2/apysc/_material_design/icon/material_help_center_icon.py
--rw-r--r--   0 runner    (1001) docker     (127)     1636 2024-05-23 14:23:55.000000 apysc-4.4.2/apysc/_material_design/icon/material_help_center_outlined_icon.py
--rw-r--r--   0 runner    (1001) docker     (127)     1293 2024-05-23 14:23:55.000000 apysc-4.4.2/apysc/_material_design/icon/material_help_icon.py
--rw-r--r--   0 runner    (1001) docker     (127)     1291 2024-05-23 14:23:55.000000 apysc-4.4.2/apysc/_material_design/icon/material_help_outline_icon.py
--rw-r--r--   0 runner    (1001) docker     (127)     1319 2024-05-23 14:23:55.000000 apysc-4.4.2/apysc/_material_design/icon/material_help_outline_outlined_icon.py
--rw-r--r--   0 runner    (1001) docker     (127)     1321 2024-05-23 14:23:55.000000 apysc-4.4.2/apysc/_material_design/icon/material_help_outlined_icon.py
--rw-r--r--   0 runner    (1001) docker     (127)     1281 2024-05-23 14:23:55.000000 apysc-4.4.2/apysc/_material_design/icon/material_high_quality_icon.py
--rw-r--r--   0 runner    (1001) docker     (127)     1323 2024-05-23 14:23:55.000000 apysc-4.4.2/apysc/_material_design/icon/material_high_quality_outlined_icon.py
--rw-r--r--   0 runner    (1001) docker     (127)     1325 2024-05-23 14:23:55.000000 apysc-4.4.2/apysc/_material_design/icon/material_highlight_alt_icon.py
--rw-r--r--   0 runner    (1001) docker     (127)     1434 2024-05-23 14:23:55.000000 apysc-4.4.2/apysc/_material_design/icon/material_highlight_alt_outlined_icon.py
--rw-r--r--   0 runner    (1001) docker     (127)     1284 2024-05-23 14:23:55.000000 apysc-4.4.2/apysc/_material_design/icon/material_highlight_off_icon.py
--rw-r--r--   0 runner    (1001) docker     (127)     1312 2024-05-23 14:23:55.000000 apysc-4.4.2/apysc/_material_design/icon/material_highlight_off_outlined_icon.py
--rw-r--r--   0 runner    (1001) docker     (127)     1258 2024-05-23 14:23:55.000000 apysc-4.4.2/apysc/_material_design/icon/material_history_icon.py
--rw-r--r--   0 runner    (1001) docker     (127)     1284 2024-05-23 14:23:55.000000 apysc-4.4.2/apysc/_material_design/icon/material_history_outlined_icon.py
--rw-r--r--   0 runner    (1001) docker     (127)     2216 2024-05-23 14:23:55.000000 apysc-4.4.2/apysc/_material_design/icon/material_history_toggle_off_icon.py
--rw-r--r--   0 runner    (1001) docker     (127)     2242 2024-05-23 14:23:55.000000 apysc-4.4.2/apysc/_material_design/icon/material_history_toggle_off_outlined_icon.py
--rw-r--r--   0 runner    (1001) docker     (127)     1071 2024-05-23 14:23:55.000000 apysc-4.4.2/apysc/_material_design/icon/material_home_filled_icon.py
--rw-r--r--   0 runner    (1001) docker     (127)     1060 2024-05-23 14:23:55.000000 apysc-4.4.2/apysc/_material_design/icon/material_home_icon.py
--rw-r--r--   0 runner    (1001) docker     (127)     1130 2024-05-23 14:23:55.000000 apysc-4.4.2/apysc/_material_design/icon/material_home_outlined_icon.py
--rw-r--r--   0 runner    (1001) docker     (127)     1106 2024-05-23 14:23:55.000000 apysc-4.4.2/apysc/_material_design/icon/material_horizontal_split_icon.py
--rw-r--r--   0 runner    (1001) docker     (127)     1148 2024-05-23 14:23:55.000000 apysc-4.4.2/apysc/_material_design/icon/material_horizontal_split_outlined_icon.py
--rw-r--r--   0 runner    (1001) docker     (127)     1198 2024-05-23 14:23:55.000000 apysc-4.4.2/apysc/_material_design/icon/material_hourglass_bottom_icon.py
--rw-r--r--   0 runner    (1001) docker     (127)     1224 2024-05-23 14:23:55.000000 apysc-4.4.2/apysc/_material_design/icon/material_hourglass_bottom_outlined_icon.py
--rw-r--r--   0 runner    (1001) docker     (127)     1351 2024-05-23 14:23:55.000000 apysc-4.4.2/apysc/_material_design/icon/material_hourglass_disabled_icon.py
--rw-r--r--   0 runner    (1001) docker     (127)     1377 2024-05-23 14:23:55.000000 apysc-4.4.2/apysc/_material_design/icon/material_hourglass_disabled_outlined_icon.py
--rw-r--r--   0 runner    (1001) docker     (127)     1198 2024-05-23 14:23:55.000000 apysc-4.4.2/apysc/_material_design/icon/material_hourglass_empty_icon.py
--rw-r--r--   0 runner    (1001) docker     (127)     1224 2024-05-23 14:23:55.000000 apysc-4.4.2/apysc/_material_design/icon/material_hourglass_empty_outlined_icon.py
--rw-r--r--   0 runner    (1001) docker     (127)     1144 2024-05-23 14:23:55.000000 apysc-4.4.2/apysc/_material_design/icon/material_hourglass_full_icon.py
--rw-r--r--   0 runner    (1001) docker     (127)     1170 2024-05-23 14:23:55.000000 apysc-4.4.2/apysc/_material_design/icon/material_hourglass_full_outlined_icon.py
--rw-r--r--   0 runner    (1001) docker     (127)     1192 2024-05-23 14:23:55.000000 apysc-4.4.2/apysc/_material_design/icon/material_hourglass_top_icon.py
--rw-r--r--   0 runner    (1001) docker     (127)     1218 2024-05-23 14:23:55.000000 apysc-4.4.2/apysc/_material_design/icon/material_hourglass_top_outlined_icon.py
--rw-r--r--   0 runner    (1001) docker     (127)     1275 2024-05-23 14:23:55.000000 apysc-4.4.2/apysc/_material_design/icon/material_how_to_reg_icon.py
--rw-r--r--   0 runner    (1001) docker     (127)     1323 2024-05-23 14:23:55.000000 apysc-4.4.2/apysc/_material_design/icon/material_how_to_reg_outlined_icon.py
--rw-r--r--   0 runner    (1001) docker     (127)     1340 2024-05-23 14:23:55.000000 apysc-4.4.2/apysc/_material_design/icon/material_how_to_vote_icon.py
--rw-r--r--   0 runner    (1001) docker     (127)     1384 2024-05-23 14:23:55.000000 apysc-4.4.2/apysc/_material_design/icon/material_how_to_vote_outlined_icon.py
--rw-r--r--   0 runner    (1001) docker     (127)     1222 2024-05-23 14:23:55.000000 apysc-4.4.2/apysc/_material_design/icon/material_http_icon.py
--rw-r--r--   0 runner    (1001) docker     (127)     1262 2024-05-23 14:23:55.000000 apysc-4.4.2/apysc/_material_design/icon/material_http_outlined_icon.py
--rw-r--r--   0 runner    (1001) docker     (127)     1253 2024-05-23 14:23:55.000000 apysc-4.4.2/apysc/_material_design/icon/material_https_icon.py
--rw-r--r--   0 runner    (1001) docker     (127)     1275 2024-05-23 14:23:55.000000 apysc-4.4.2/apysc/_material_design/icon/material_https_outlined_icon.py
--rw-r--r--   0 runner    (1001) docker     (127)     1514 2024-05-23 14:23:55.000000 apysc-4.4.2/apysc/_material_design/icon/material_import_contacts_icon.py
--rw-r--r--   0 runner    (1001) docker     (127)     1472 2024-05-23 14:23:55.000000 apysc-4.4.2/apysc/_material_design/icon/material_import_contacts_outlined_icon.py
--rw-r--r--   0 runner    (1001) docker     (127)     1120 2024-05-23 14:23:55.000000 apysc-4.4.2/apysc/_material_design/icon/material_import_export_icon.py
--rw-r--r--   0 runner    (1001) docker     (127)     1148 2024-05-23 14:23:55.000000 apysc-4.4.2/apysc/_material_design/icon/material_import_export_outlined_icon.py
--rw-r--r--   0 runner    (1001) docker     (127)     1349 2024-05-23 14:23:55.000000 apysc-4.4.2/apysc/_material_design/icon/material_important_devices_icon.py
--rw-r--r--   0 runner    (1001) docker     (127)     1375 2024-05-23 14:23:55.000000 apysc-4.4.2/apysc/_material_design/icon/material_important_devices_outlined_icon.py
--rw-r--r--   0 runner    (1001) docker     (127)     1175 2024-05-23 14:23:55.000000 apysc-4.4.2/apysc/_material_design/icon/material_inbox_icon.py
--rw-r--r--   0 runner    (1001) docker     (127)     1238 2024-05-23 14:23:55.000000 apysc-4.4.2/apysc/_material_design/icon/material_inbox_outlined_icon.py
--rw-r--r--   0 runner    (1001) docker     (127)     1121 2024-05-23 14:23:55.000000 apysc-4.4.2/apysc/_material_design/icon/material_info_icon.py
--rw-r--r--   0 runner    (1001) docker     (127)     1256 2024-05-23 14:23:55.000000 apysc-4.4.2/apysc/_material_design/icon/material_info_outline_icon.py
--rw-r--r--   0 runner    (1001) docker     (127)     1201 2024-05-23 14:23:55.000000 apysc-4.4.2/apysc/_material_design/icon/material_info_outlined_icon.py
--rw-r--r--   0 runner    (1001) docker     (127)     1173 2024-05-23 14:23:55.000000 apysc-4.4.2/apysc/_material_design/icon/material_input_icon.py
--rw-r--r--   0 runner    (1001) docker     (127)     1394 2024-05-23 14:23:55.000000 apysc-4.4.2/apysc/_material_design/icon/material_input_outlined_icon.py
--rw-r--r--   0 runner    (1001) docker     (127)     1613 2024-05-23 14:23:55.000000 apysc-4.4.2/apysc/_material_design/icon/material_insights_icon.py
--rw-r--r--   0 runner    (1001) docker     (127)     1639 2024-05-23 14:23:55.000000 apysc-4.4.2/apysc/_material_design/icon/material_insights_outlined_icon.py
--rw-r--r--   0 runner    (1001) docker     (127)     1810 2024-05-23 14:23:55.000000 apysc-4.4.2/apysc/_material_design/icon/material_integration_instructions_icon.py
--rw-r--r--   0 runner    (1001) docker     (127)     1921 2024-05-23 14:23:55.000000 apysc-4.4.2/apysc/_material_design/icon/material_integration_instructions_outlined_icon.py
--rw-r--r--   0 runner    (1001) docker     (127)     1201 2024-05-23 14:23:55.000000 apysc-4.4.2/apysc/_material_design/icon/material_inventory_icon.py
--rw-r--r--   0 runner    (1001) docker     (127)     1288 2024-05-23 14:23:55.000000 apysc-4.4.2/apysc/_material_design/icon/material_invert_colors_icon.py
--rw-r--r--   0 runner    (1001) docker     (127)     1450 2024-05-23 14:23:55.000000 apysc-4.4.2/apysc/_material_design/icon/material_invert_colors_off_icon.py
--rw-r--r--   0 runner    (1001) docker     (127)     1417 2024-05-23 14:23:55.000000 apysc-4.4.2/apysc/_material_design/icon/material_invert_colors_off_outlined_icon.py
--rw-r--r--   0 runner    (1001) docker     (127)     1309 2024-05-23 14:23:55.000000 apysc-4.4.2/apysc/_material_design/icon/material_invert_colors_outlined_icon.py
--rw-r--r--   0 runner    (1001) docker     (127)     1160 2024-05-23 14:23:55.000000 apysc-4.4.2/apysc/_material_design/icon/material_label_icon.py
--rw-r--r--   0 runner    (1001) docker     (127)     1172 2024-05-23 14:23:55.000000 apysc-4.4.2/apysc/_material_design/icon/material_label_important_icon.py
--rw-r--r--   0 runner    (1001) docker     (127)     1204 2024-05-23 14:23:55.000000 apysc-4.4.2/apysc/_material_design/icon/material_label_important_outline_icon.py
--rw-r--r--   0 runner    (1001) docker     (127)     1175 2024-05-23 14:23:55.000000 apysc-4.4.2/apysc/_material_design/icon/material_label_important_outlined_icon.py
--rw-r--r--   0 runner    (1001) docker     (127)     1179 2024-05-23 14:23:55.000000 apysc-4.4.2/apysc/_material_design/icon/material_label_off_icon.py
--rw-r--r--   0 runner    (1001) docker     (127)     1311 2024-05-23 14:23:55.000000 apysc-4.4.2/apysc/_material_design/icon/material_label_off_outlined_icon.py
--rw-r--r--   0 runner    (1001) docker     (127)     1210 2024-05-23 14:23:55.000000 apysc-4.4.2/apysc/_material_design/icon/material_label_outline_icon.py
--rw-r--r--   0 runner    (1001) docker     (127)     1215 2024-05-23 14:23:55.000000 apysc-4.4.2/apysc/_material_design/icon/material_label_outlined_icon.py
--rw-r--r--   0 runner    (1001) docker     (127)     1846 2024-05-23 14:23:55.000000 apysc-4.4.2/apysc/_material_design/icon/material_language_icon.py
--rw-r--r--   0 runner    (1001) docker     (127)     1854 2024-05-23 14:23:55.000000 apysc-4.4.2/apysc/_material_design/icon/material_language_outlined_icon.py
--rw-r--r--   0 runner    (1001) docker     (127)     1161 2024-05-23 14:23:55.000000 apysc-4.4.2/apysc/_material_design/icon/material_launch_icon.py
--rw-r--r--   0 runner    (1001) docker     (127)     1189 2024-05-23 14:23:55.000000 apysc-4.4.2/apysc/_material_design/icon/material_launch_outlined_icon.py
--rw-r--r--   0 runner    (1001) docker     (127)     1157 2024-05-23 14:23:55.000000 apysc-4.4.2/apysc/_material_design/icon/material_leaderboard_icon.py
--rw-r--r--   0 runner    (1001) docker     (127)     1197 2024-05-23 14:23:55.000000 apysc-4.4.2/apysc/_material_design/icon/material_leaderboard_outlined_icon.py
--rw-r--r--   0 runner    (1001) docker     (127)     1232 2024-05-23 14:23:55.000000 apysc-4.4.2/apysc/_material_design/icon/material_library_add_check_icon.py
--rw-r--r--   0 runner    (1001) docker     (127)     1334 2024-05-23 14:23:55.000000 apysc-4.4.2/apysc/_material_design/icon/material_library_add_check_outlined_icon.py
--rw-r--r--   0 runner    (1001) docker     (127)     1188 2024-05-23 14:23:55.000000 apysc-4.4.2/apysc/_material_design/icon/material_library_add_icon.py
--rw-r--r--   0 runner    (1001) docker     (127)     1231 2024-05-23 14:23:55.000000 apysc-4.4.2/apysc/_material_design/icon/material_library_add_outlined_icon.py
--rw-r--r--   0 runner    (1001) docker     (127)     1205 2024-05-23 14:23:55.000000 apysc-4.4.2/apysc/_material_design/icon/material_library_books_icon.py
--rw-r--r--   0 runner    (1001) docker     (127)     1242 2024-05-23 14:23:55.000000 apysc-4.4.2/apysc/_material_design/icon/material_library_books_outlined_icon.py
--rw-r--r--   0 runner    (1001) docker     (127)     1259 2024-05-23 14:23:55.000000 apysc-4.4.2/apysc/_material_design/icon/material_library_music_icon.py
--rw-r--r--   0 runner    (1001) docker     (127)     1317 2024-05-23 14:23:55.000000 apysc-4.4.2/apysc/_material_design/icon/material_library_music_outlined_icon.py
--rw-r--r--   0 runner    (1001) docker     (127)     1197 2024-05-23 14:23:55.000000 apysc-4.4.2/apysc/_material_design/icon/material_lightbulb_icon.py
--rw-r--r--   0 runner    (1001) docker     (127)     1427 2024-05-23 14:23:55.000000 apysc-4.4.2/apysc/_material_design/icon/material_lightbulb_outline_icon.py
--rw-r--r--   0 runner    (1001) docker     (127)     1356 2024-05-23 14:23:55.000000 apysc-4.4.2/apysc/_material_design/icon/material_lightbulb_outlined_icon.py
--rw-r--r--   0 runner    (1001) docker     (127)     1307 2024-05-23 14:23:55.000000 apysc-4.4.2/apysc/_material_design/icon/material_line_style_icon.py
--rw-r--r--   0 runner    (1001) docker     (127)     1236 2024-05-23 14:23:55.000000 apysc-4.4.2/apysc/_material_design/icon/material_line_style_outlined_icon.py
--rw-r--r--   0 runner    (1001) docker     (127)     1186 2024-05-23 14:23:55.000000 apysc-4.4.2/apysc/_material_design/icon/material_line_weight_icon.py
--rw-r--r--   0 runner    (1001) docker     (127)     1131 2024-05-23 14:23:55.000000 apysc-4.4.2/apysc/_material_design/icon/material_line_weight_outlined_icon.py
--rw-r--r--   0 runner    (1001) docker     (127)     1236 2024-05-23 14:23:55.000000 apysc-4.4.2/apysc/_material_design/icon/material_link_icon.py
--rw-r--r--   0 runner    (1001) docker     (127)     1390 2024-05-23 14:23:55.000000 apysc-4.4.2/apysc/_material_design/icon/material_link_off_icon.py
--rw-r--r--   0 runner    (1001) docker     (127)     1393 2024-05-23 14:23:55.000000 apysc-4.4.2/apysc/_material_design/icon/material_link_off_outlined_icon.py
--rw-r--r--   0 runner    (1001) docker     (127)     1224 2024-05-23 14:23:55.000000 apysc-4.4.2/apysc/_material_design/icon/material_link_outlined_icon.py
--rw-r--r--   0 runner    (1001) docker     (127)     1213 2024-05-23 14:23:55.000000 apysc-4.4.2/apysc/_material_design/icon/material_list_alt_icon.py
--rw-r--r--   0 runner    (1001) docker     (127)     1239 2024-05-23 14:23:55.000000 apysc-4.4.2/apysc/_material_design/icon/material_list_alt_outlined_icon.py
--rw-r--r--   0 runner    (1001) docker     (127)     1111 2024-05-23 14:23:55.000000 apysc-4.4.2/apysc/_material_design/icon/material_list_icon.py
--rw-r--r--   0 runner    (1001) docker     (127)     1273 2024-05-23 14:23:55.000000 apysc-4.4.2/apysc/_material_design/icon/material_list_outlined_icon.py
--rw-r--r--   0 runner    (1001) docker     (127)     1329 2024-05-23 14:23:55.000000 apysc-4.4.2/apysc/_material_design/icon/material_live_help_icon.py
--rw-r--r--   0 runner    (1001) docker     (127)     1324 2024-05-23 14:23:55.000000 apysc-4.4.2/apysc/_material_design/icon/material_live_help_outlined_icon.py
--rw-r--r--   0 runner    (1001) docker     (127)     1381 2024-05-23 14:23:55.000000 apysc-4.4.2/apysc/_material_design/icon/material_location_off_icon.py
--rw-r--r--   0 runner    (1001) docker     (127)     1511 2024-05-23 14:23:55.000000 apysc-4.4.2/apysc/_material_design/icon/material_location_off_outlined_icon.py
--rw-r--r--   0 runner    (1001) docker     (127)     1199 2024-05-23 14:23:55.000000 apysc-4.4.2/apysc/_material_design/icon/material_location_on_icon.py
--rw-r--r--   0 runner    (1001) docker     (127)     1257 2024-05-23 14:23:55.000000 apysc-4.4.2/apysc/_material_design/icon/material_location_on_outlined_icon.py
--rw-r--r--   0 runner    (1001) docker     (127)     1383 2024-05-23 14:23:55.000000 apysc-4.4.2/apysc/_material_design/icon/material_lock_clock_icon.py
--rw-r--r--   0 runner    (1001) docker     (127)     1250 2024-05-23 14:23:55.000000 apysc-4.4.2/apysc/_material_design/icon/material_lock_icon.py
--rw-r--r--   0 runner    (1001) docker     (127)     1270 2024-05-23 14:23:55.000000 apysc-4.4.2/apysc/_material_design/icon/material_lock_open_icon.py
--rw-r--r--   0 runner    (1001) docker     (127)     1277 2024-05-23 14:23:55.000000 apysc-4.4.2/apysc/_material_design/icon/material_lock_open_outlined_icon.py
--rw-r--r--   0 runner    (1001) docker     (127)     1380 2024-05-23 14:23:55.000000 apysc-4.4.2/apysc/_material_design/icon/material_lock_outline_icon.py
--rw-r--r--   0 runner    (1001) docker     (127)     1320 2024-05-23 14:23:55.000000 apysc-4.4.2/apysc/_material_design/icon/material_lock_outlined_icon.py
--rw-r--r--   0 runner    (1001) docker     (127)     1195 2024-05-23 14:23:55.000000 apysc-4.4.2/apysc/_material_design/icon/material_login_icon.py
--rw-r--r--   0 runner    (1001) docker     (127)     1221 2024-05-23 14:23:55.000000 apysc-4.4.2/apysc/_material_design/icon/material_login_outlined_icon.py
--rw-r--r--   0 runner    (1001) docker     (127)     1141 2024-05-23 14:23:55.000000 apysc-4.4.2/apysc/_material_design/icon/material_logout_icon.py
--rw-r--r--   0 runner    (1001) docker     (127)     1248 2024-05-23 14:23:55.000000 apysc-4.4.2/apysc/_material_design/icon/material_loop_icon.py
--rw-r--r--   0 runner    (1001) docker     (127)     1276 2024-05-23 14:23:55.000000 apysc-4.4.2/apysc/_material_design/icon/material_loop_outlined_icon.py
--rw-r--r--   0 runner    (1001) docker     (127)     1204 2024-05-23 14:23:55.000000 apysc-4.4.2/apysc/_material_design/icon/material_low_priority_icon.py
--rw-r--r--   0 runner    (1001) docker     (127)     1240 2024-05-23 14:23:55.000000 apysc-4.4.2/apysc/_material_design/icon/material_low_priority_outlined_icon.py
--rw-r--r--   0 runner    (1001) docker     (127)     1474 2024-05-23 14:23:55.000000 apysc-4.4.2/apysc/_material_design/icon/material_loyalty_icon.py
--rw-r--r--   0 runner    (1001) docker     (127)     1497 2024-05-23 14:23:55.000000 apysc-4.4.2/apysc/_material_design/icon/material_loyalty_outlined_icon.py
--rw-r--r--   0 runner    (1001) docker     (127)     1134 2024-05-23 14:23:55.000000 apysc-4.4.2/apysc/_material_design/icon/material_mail_icon.py
--rw-r--r--   0 runner    (1001) docker     (127)     1170 2024-05-23 14:23:55.000000 apysc-4.4.2/apysc/_material_design/icon/material_mail_outline_icon.py
--rw-r--r--   0 runner    (1001) docker     (127)     1198 2024-05-23 14:23:55.000000 apysc-4.4.2/apysc/_material_design/icon/material_mail_outline_outlined_icon.py
--rw-r--r--   0 runner    (1001) docker     (127)     1171 2024-05-23 14:23:55.000000 apysc-4.4.2/apysc/_material_design/icon/material_mail_outlined_icon.py
--rw-r--r--   0 runner    (1001) docker     (127)     1287 2024-05-23 14:23:55.000000 apysc-4.4.2/apysc/_material_design/icon/material_mark_as_unread_icon.py
--rw-r--r--   0 runner    (1001) docker     (127)     1325 2024-05-23 14:23:55.000000 apysc-4.4.2/apysc/_material_design/icon/material_mark_chat_read_icon.py
--rw-r--r--   0 runner    (1001) docker     (127)     1274 2024-05-23 14:23:55.000000 apysc-4.4.2/apysc/_material_design/icon/material_mark_chat_read_outlined_icon.py
--rw-r--r--   0 runner    (1001) docker     (127)     1300 2024-05-23 14:23:55.000000 apysc-4.4.2/apysc/_material_design/icon/material_mark_chat_unread_icon.py
--rw-r--r--   0 runner    (1001) docker     (127)     1345 2024-05-23 14:23:55.000000 apysc-4.4.2/apysc/_material_design/icon/material_mark_chat_unread_outlined_icon.py
--rw-r--r--   0 runner    (1001) docker     (127)     1342 2024-05-23 14:23:55.000000 apysc-4.4.2/apysc/_material_design/icon/material_mark_email_read_icon.py
--rw-r--r--   0 runner    (1001) docker     (127)     1313 2024-05-23 14:23:55.000000 apysc-4.4.2/apysc/_material_design/icon/material_mark_email_read_outlined_icon.py
--rw-r--r--   0 runner    (1001) docker     (127)     1370 2024-05-23 14:23:55.000000 apysc-4.4.2/apysc/_material_design/icon/material_mark_email_unread_icon.py
--rw-r--r--   0 runner    (1001) docker     (127)     1417 2024-05-23 14:23:55.000000 apysc-4.4.2/apysc/_material_design/icon/material_mark_email_unread_outlined_icon.py
--rw-r--r--   0 runner    (1001) docker     (127)     1152 2024-05-23 14:23:55.000000 apysc-4.4.2/apysc/_material_design/icon/material_markunread_icon.py
--rw-r--r--   0 runner    (1001) docker     (127)     1183 2024-05-23 14:23:55.000000 apysc-4.4.2/apysc/_material_design/icon/material_markunread_mailbox_icon.py
--rw-r--r--   0 runner    (1001) docker     (127)     1199 2024-05-23 14:23:55.000000 apysc-4.4.2/apysc/_material_design/icon/material_markunread_mailbox_outlined_icon.py
--rw-r--r--   0 runner    (1001) docker     (127)     1186 2024-05-23 14:23:55.000000 apysc-4.4.2/apysc/_material_design/icon/material_markunread_outlined_icon.py
--rw-r--r--   0 runner    (1001) docker     (127)     1051 2024-05-23 14:23:55.000000 apysc-4.4.2/apysc/_material_design/icon/material_maximize_icon.py
--rw-r--r--   0 runner    (1001) docker     (127)     1079 2024-05-23 14:23:55.000000 apysc-4.4.2/apysc/_material_design/icon/material_maximize_outlined_icon.py
--rw-r--r--   0 runner    (1001) docker     (127)     1454 2024-05-23 14:23:55.000000 apysc-4.4.2/apysc/_material_design/icon/material_mediation_icon.py
--rw-r--r--   0 runner    (1001) docker     (127)     1500 2024-05-23 14:23:55.000000 apysc-4.4.2/apysc/_material_design/icon/material_mediation_outlined_icon.py
--rw-r--r--   0 runner    (1001) docker     (127)     1152 2024-05-23 14:23:55.000000 apysc-4.4.2/apysc/_material_design/icon/material_message_icon.py
--rw-r--r--   0 runner    (1001) docker     (127)     1203 2024-05-23 14:23:55.000000 apysc-4.4.2/apysc/_material_design/icon/material_message_outlined_icon.py
--rw-r--r--   0 runner    (1001) docker     (127)     1213 2024-05-23 14:23:55.000000 apysc-4.4.2/apysc/_material_design/icon/material_mic_icon.py
--rw-r--r--   0 runner    (1001) docker     (127)     1338 2024-05-23 14:23:55.000000 apysc-4.4.2/apysc/_material_design/icon/material_mic_none_icon.py
--rw-r--r--   0 runner    (1001) docker     (127)     1300 2024-05-23 14:23:55.000000 apysc-4.4.2/apysc/_material_design/icon/material_mic_none_outlined_icon.py
--rw-r--r--   0 runner    (1001) docker     (127)     1402 2024-05-23 14:23:55.000000 apysc-4.4.2/apysc/_material_design/icon/material_mic_off_icon.py
--rw-r--r--   0 runner    (1001) docker     (127)     1463 2024-05-23 14:23:55.000000 apysc-4.4.2/apysc/_material_design/icon/material_mic_off_outlined_icon.py
--rw-r--r--   0 runner    (1001) docker     (127)     1390 2024-05-23 14:23:55.000000 apysc-4.4.2/apysc/_material_design/icon/material_mic_outlined_icon.py
--rw-r--r--   0 runner    (1001) docker     (127)     1052 2024-05-23 14:23:55.000000 apysc-4.4.2/apysc/_material_design/icon/material_minimize_icon.py
--rw-r--r--   0 runner    (1001) docker     (127)     1081 2024-05-23 14:23:55.000000 apysc-4.4.2/apysc/_material_design/icon/material_minimize_outlined_icon.py
--rw-r--r--   0 runner    (1001) docker     (127)     1239 2024-05-23 14:23:55.000000 apysc-4.4.2/apysc/_material_design/icon/material_missed_video_call_icon.py
--rw-r--r--   0 runner    (1001) docker     (127)     1291 2024-05-23 14:23:55.000000 apysc-4.4.2/apysc/_material_design/icon/material_missed_video_call_outlined_icon.py
--rw-r--r--   0 runner    (1001) docker     (127)     1274 2024-05-23 14:23:55.000000 apysc-4.4.2/apysc/_material_design/icon/material_mobile_screen_share_icon.py
--rw-r--r--   0 runner    (1001) docker     (127)     1308 2024-05-23 14:23:55.000000 apysc-4.4.2/apysc/_material_design/icon/material_mobile_screen_share_outlined_icon.py
--rw-r--r--   0 runner    (1001) docker     (127)     1511 2024-05-23 14:23:55.000000 apysc-4.4.2/apysc/_material_design/icon/material_model_training_icon.py
--rw-r--r--   0 runner    (1001) docker     (127)     1537 2024-05-23 14:23:55.000000 apysc-4.4.2/apysc/_material_design/icon/material_model_training_outlined_icon.py
--rw-r--r--   0 runner    (1001) docker     (127)     1438 2024-05-23 14:23:55.000000 apysc-4.4.2/apysc/_material_design/icon/material_more_time_icon.py
--rw-r--r--   0 runner    (1001) docker     (127)     1464 2024-05-23 14:23:55.000000 apysc-4.4.2/apysc/_material_design/icon/material_more_time_outlined_icon.py
--rw-r--r--   0 runner    (1001) docker     (127)     1221 2024-05-23 14:23:55.000000 apysc-4.4.2/apysc/_material_design/icon/material_move_to_inbox_icon.py
--rw-r--r--   0 runner    (1001) docker     (127)     1298 2024-05-23 14:23:55.000000 apysc-4.4.2/apysc/_material_design/icon/material_move_to_inbox_outlined_icon.py
--rw-r--r--   0 runner    (1001) docker     (127)     1138 2024-05-23 14:23:55.000000 apysc-4.4.2/apysc/_material_design/icon/material_movie_icon.py
--rw-r--r--   0 runner    (1001) docker     (127)     1193 2024-05-23 14:23:55.000000 apysc-4.4.2/apysc/_material_design/icon/material_movie_outlined_icon.py
--rw-r--r--   0 runner    (1001) docker     (127)     1241 2024-05-23 14:23:55.000000 apysc-4.4.2/apysc/_material_design/icon/material_music_video_icon.py
--rw-r--r--   0 runner    (1001) docker     (127)     1267 2024-05-23 14:23:55.000000 apysc-4.4.2/apysc/_material_design/icon/material_music_video_outlined_icon.py
--rw-r--r--   0 runner    (1001) docker     (127)     1377 2024-05-23 14:23:55.000000 apysc-4.4.2/apysc/_material_design/icon/material_nat_icon.py
--rw-r--r--   0 runner    (1001) docker     (127)     1403 2024-05-23 14:23:55.000000 apysc-4.4.2/apysc/_material_design/icon/material_nat_outlined_icon.py
--rw-r--r--   0 runner    (1001) docker     (127)     1256 2024-05-23 14:23:55.000000 apysc-4.4.2/apysc/_material_design/icon/material_new_releases_icon.py
--rw-r--r--   0 runner    (1001) docker     (127)     1475 2024-05-23 14:23:55.000000 apysc-4.4.2/apysc/_material_design/icon/material_new_releases_outlined_icon.py
--rw-r--r--   0 runner    (1001) docker     (127)     1337 2024-05-23 14:23:55.000000 apysc-4.4.2/apysc/_material_design/icon/material_next_plan_icon.py
--rw-r--r--   0 runner    (1001) docker     (127)     1437 2024-05-23 14:23:55.000000 apysc-4.4.2/apysc/_material_design/icon/material_next_plan_outlined_icon.py
--rw-r--r--   0 runner    (1001) docker     (127)     1329 2024-05-23 14:23:55.000000 apysc-4.4.2/apysc/_material_design/icon/material_next_week_icon.py
--rw-r--r--   0 runner    (1001) docker     (127)     1278 2024-05-23 14:23:55.000000 apysc-4.4.2/apysc/_material_design/icon/material_next_week_outlined_icon.py
--rw-r--r--   0 runner    (1001) docker     (127)     1277 2024-05-23 14:23:55.000000 apysc-4.4.2/apysc/_material_design/icon/material_nightlight_round_icon.py
--rw-r--r--   0 runner    (1001) docker     (127)     1189 2024-05-23 14:23:55.000000 apysc-4.4.2/apysc/_material_design/icon/material_no_sim_icon.py
--rw-r--r--   0 runner    (1001) docker     (127)     1260 2024-05-23 14:23:55.000000 apysc-4.4.2/apysc/_material_design/icon/material_no_sim_outlined_icon.py
--rw-r--r--   0 runner    (1001) docker     (127)     1590 2024-05-23 14:23:55.000000 apysc-4.4.2/apysc/_material_design/icon/material_not_accessible_icon.py
--rw-r--r--   0 runner    (1001) docker     (127)     1606 2024-05-23 14:23:55.000000 apysc-4.4.2/apysc/_material_design/icon/material_not_accessible_outlined_icon.py
--rw-r--r--   0 runner    (1001) docker     (127)     1292 2024-05-23 14:23:55.000000 apysc-4.4.2/apysc/_material_design/icon/material_not_interested_icon.py
--rw-r--r--   0 runner    (1001) docker     (127)     1320 2024-05-23 14:23:55.000000 apysc-4.4.2/apysc/_material_design/icon/material_not_interested_outlined_icon.py
--rw-r--r--   0 runner    (1001) docker     (127)     1209 2024-05-23 14:23:55.000000 apysc-4.4.2/apysc/_material_design/icon/material_not_started_icon.py
--rw-r--r--   0 runner    (1001) docker     (127)     1300 2024-05-23 14:23:55.000000 apysc-4.4.2/apysc/_material_design/icon/material_not_started_outlined_icon.py
--rw-r--r--   0 runner    (1001) docker     (127)     1168 2024-05-23 14:23:55.000000 apysc-4.4.2/apysc/_material_design/icon/material_note_add_icon.py
--rw-r--r--   0 runner    (1001) docker     (127)     1185 2024-05-23 14:23:55.000000 apysc-4.4.2/apysc/_material_design/icon/material_note_add_outlined_icon.py
--rw-r--r--   0 runner    (1001) docker     (127)     1135 2024-05-23 14:23:55.000000 apysc-4.4.2/apysc/_material_design/icon/material_note_icon.py
--rw-r--r--   0 runner    (1001) docker     (127)     1154 2024-05-23 14:23:55.000000 apysc-4.4.2/apysc/_material_design/icon/material_note_outlined_icon.py
--rw-r--r--   0 runner    (1001) docker     (127)     1272 2024-05-23 14:23:55.000000 apysc-4.4.2/apysc/_material_design/icon/material_notification_important_icon.py
--rw-r--r--   0 runner    (1001) docker     (127)     1332 2024-05-23 14:23:55.000000 apysc-4.4.2/apysc/_material_design/icon/material_notification_important_outlined_icon.py
--rw-r--r--   0 runner    (1001) docker     (127)     1186 2024-05-23 14:23:55.000000 apysc-4.4.2/apysc/_material_design/icon/material_offline_bolt_icon.py
--rw-r--r--   0 runner    (1001) docker     (127)     1300 2024-05-23 14:23:55.000000 apysc-4.4.2/apysc/_material_design/icon/material_offline_bolt_outlined_icon.py
--rw-r--r--   0 runner    (1001) docker     (127)     1249 2024-05-23 14:23:55.000000 apysc-4.4.2/apysc/_material_design/icon/material_offline_pin_icon.py
--rw-r--r--   0 runner    (1001) docker     (127)     1251 2024-05-23 14:23:55.000000 apysc-4.4.2/apysc/_material_design/icon/material_offline_pin_outlined_icon.py
--rw-r--r--   0 runner    (1001) docker     (127)     1780 2024-05-23 14:23:55.000000 apysc-4.4.2/apysc/_material_design/icon/material_online_prediction_icon.py
--rw-r--r--   0 runner    (1001) docker     (127)     1806 2024-05-23 14:23:55.000000 apysc-4.4.2/apysc/_material_design/icon/material_online_prediction_outlined_icon.py
--rw-r--r--   0 runner    (1001) docker     (127)     1289 2024-05-23 14:23:55.000000 apysc-4.4.2/apysc/_material_design/icon/material_opacity_icon.py
--rw-r--r--   0 runner    (1001) docker     (127)     1315 2024-05-23 14:23:55.000000 apysc-4.4.2/apysc/_material_design/icon/material_opacity_outlined_icon.py
--rw-r--r--   0 runner    (1001) docker     (127)     1181 2024-05-23 14:23:55.000000 apysc-4.4.2/apysc/_material_design/icon/material_open_in_browser_icon.py
--rw-r--r--   0 runner    (1001) docker     (127)     1209 2024-05-23 14:23:55.000000 apysc-4.4.2/apysc/_material_design/icon/material_open_in_browser_outlined_icon.py
--rw-r--r--   0 runner    (1001) docker     (127)     1169 2024-05-23 14:23:55.000000 apysc-4.4.2/apysc/_material_design/icon/material_open_in_full_icon.py
--rw-r--r--   0 runner    (1001) docker     (127)     1195 2024-05-23 14:23:55.000000 apysc-4.4.2/apysc/_material_design/icon/material_open_in_full_outlined_icon.py
--rw-r--r--   0 runner    (1001) docker     (127)     1174 2024-05-23 14:23:55.000000 apysc-4.4.2/apysc/_material_design/icon/material_open_in_new_icon.py
--rw-r--r--   0 runner    (1001) docker     (127)     1202 2024-05-23 14:23:55.000000 apysc-4.4.2/apysc/_material_design/icon/material_open_in_new_outlined_icon.py
--rw-r--r--   0 runner    (1001) docker     (127)     1144 2024-05-23 14:23:55.000000 apysc-4.4.2/apysc/_material_design/icon/material_open_with_icon.py
--rw-r--r--   0 runner    (1001) docker     (127)     1172 2024-05-23 14:23:55.000000 apysc-4.4.2/apysc/_material_design/icon/material_open_with_outlined_icon.py
--rw-r--r--   0 runner    (1001) docker     (127)     1252 2024-05-23 14:23:55.000000 apysc-4.4.2/apysc/_material_design/icon/material_outbond_icon.py
--rw-r--r--   0 runner    (1001) docker     (127)     1343 2024-05-23 14:23:55.000000 apysc-4.4.2/apysc/_material_design/icon/material_outbond_outlined_icon.py
--rw-r--r--   0 runner    (1001) docker     (127)     1202 2024-05-23 14:23:55.000000 apysc-4.4.2/apysc/_material_design/icon/material_outbox_icon.py
--rw-r--r--   0 runner    (1001) docker     (127)     1441 2024-05-23 14:23:55.000000 apysc-4.4.2/apysc/_material_design/icon/material_outgoing_mail_icon.py
--rw-r--r--   0 runner    (1001) docker     (127)     1369 2024-05-23 14:23:55.000000 apysc-4.4.2/apysc/_material_design/icon/material_outlet_icon.py
--rw-r--r--   0 runner    (1001) docker     (127)     1468 2024-05-23 14:23:55.000000 apysc-4.4.2/apysc/_material_design/icon/material_outlet_outlined_icon.py
--rw-r--r--   0 runner    (1001) docker     (127)     1112 2024-05-23 14:23:55.000000 apysc-4.4.2/apysc/_material_design/icon/material_outlined_flag_icon.py
--rw-r--r--   0 runner    (1001) docker     (127)     1140 2024-05-23 14:23:55.000000 apysc-4.4.2/apysc/_material_design/icon/material_outlined_flag_outlined_icon.py
--rw-r--r--   0 runner    (1001) docker     (127)     1334 2024-05-23 14:23:55.000000 apysc-4.4.2/apysc/_material_design/icon/material_pageview_icon.py
--rw-r--r--   0 runner    (1001) docker     (127)     1372 2024-05-23 14:23:55.000000 apysc-4.4.2/apysc/_material_design/icon/material_pageview_outlined_icon.py
--rw-r--r--   0 runner    (1001) docker     (127)     1458 2024-05-23 14:23:55.000000 apysc-4.4.2/apysc/_material_design/icon/material_pan_tool_icon.py
--rw-r--r--   0 runner    (1001) docker     (127)     1613 2024-05-23 14:23:55.000000 apysc-4.4.2/apysc/_material_design/icon/material_pan_tool_outlined_icon.py
--rw-r--r--   0 runner    (1001) docker     (127)     1163 2024-05-23 14:23:55.000000 apysc-4.4.2/apysc/_material_design/icon/material_pause_circle_filled_icon.py
--rw-r--r--   0 runner    (1001) docker     (127)     1336 2024-05-23 14:23:55.000000 apysc-4.4.2/apysc/_material_design/icon/material_pause_circle_filled_outlined_icon.py
--rw-r--r--   0 runner    (1001) docker     (127)     1223 2024-05-23 14:23:55.000000 apysc-4.4.2/apysc/_material_design/icon/material_pause_circle_outline_icon.py
--rw-r--r--   0 runner    (1001) docker     (127)     1251 2024-05-23 14:23:55.000000 apysc-4.4.2/apysc/_material_design/icon/material_pause_circle_outline_outlined_icon.py
--rw-r--r--   0 runner    (1001) docker     (127)     1059 2024-05-23 14:23:55.000000 apysc-4.4.2/apysc/_material_design/icon/material_pause_icon.py
--rw-r--r--   0 runner    (1001) docker     (127)     1087 2024-05-23 14:23:55.000000 apysc-4.4.2/apysc/_material_design/icon/material_pause_outlined_icon.py
--rw-r--r--   0 runner    (1001) docker     (127)     1319 2024-05-23 14:23:55.000000 apysc-4.4.2/apysc/_material_design/icon/material_pause_presentation_icon.py
--rw-r--r--   0 runner    (1001) docker     (127)     1230 2024-05-23 14:23:55.000000 apysc-4.4.2/apysc/_material_design/icon/material_pause_presentation_outlined_icon.py
--rw-r--r--   0 runner    (1001) docker     (127)     1156 2024-05-23 14:23:55.000000 apysc-4.4.2/apysc/_material_design/icon/material_payment_icon.py
--rw-r--r--   0 runner    (1001) docker     (127)     1184 2024-05-23 14:23:55.000000 apysc-4.4.2/apysc/_material_design/icon/material_payment_outlined_icon.py
--rw-r--r--   0 runner    (1001) docker     (127)     1502 2024-05-23 14:23:55.000000 apysc-4.4.2/apysc/_material_design/icon/material_pending_actions_icon.py
--rw-r--r--   0 runner    (1001) docker     (127)     1528 2024-05-23 14:23:55.000000 apysc-4.4.2/apysc/_material_design/icon/material_pending_actions_outlined_icon.py
--rw-r--r--   0 runner    (1001) docker     (127)     1485 2024-05-23 14:23:55.000000 apysc-4.4.2/apysc/_material_design/icon/material_pending_icon.py
--rw-r--r--   0 runner    (1001) docker     (127)     1380 2024-05-23 14:23:55.000000 apysc-4.4.2/apysc/_material_design/icon/material_pending_outlined_icon.py
--rw-r--r--   0 runner    (1001) docker     (127)     1301 2024-05-23 14:23:55.000000 apysc-4.4.2/apysc/_material_design/icon/material_perm_camera_mic_icon.py
--rw-r--r--   0 runner    (1001) docker     (127)     1401 2024-05-23 14:23:55.000000 apysc-4.4.2/apysc/_material_design/icon/material_perm_camera_mic_outlined_icon.py
--rw-r--r--   0 runner    (1001) docker     (127)     1269 2024-05-23 14:23:55.000000 apysc-4.4.2/apysc/_material_design/icon/material_perm_contact_calendar_icon.py
--rw-r--r--   0 runner    (1001) docker     (127)     1691 2024-05-23 14:23:55.000000 apysc-4.4.2/apysc/_material_design/icon/material_perm_contact_calendar_outlined_icon.py
--rw-r--r--   0 runner    (1001) docker     (127)     1818 2024-05-23 14:23:55.000000 apysc-4.4.2/apysc/_material_design/icon/material_perm_data_setting_icon.py
--rw-r--r--   0 runner    (1001) docker     (127)     1803 2024-05-23 14:23:55.000000 apysc-4.4.2/apysc/_material_design/icon/material_perm_data_setting_outlined_icon.py
--rw-r--r--   0 runner    (1001) docker     (127)     1213 2024-05-23 14:23:55.000000 apysc-4.4.2/apysc/_material_design/icon/material_perm_device_information_icon.py
--rw-r--r--   0 runner    (1001) docker     (127)     1265 2024-05-23 14:23:55.000000 apysc-4.4.2/apysc/_material_design/icon/material_perm_device_information_outlined_icon.py
--rw-r--r--   0 runner    (1001) docker     (127)     1297 2024-05-23 14:23:55.000000 apysc-4.4.2/apysc/_material_design/icon/material_perm_identity_icon.py
--rw-r--r--   0 runner    (1001) docker     (127)     1289 2024-05-23 14:23:55.000000 apysc-4.4.2/apysc/_material_design/icon/material_perm_identity_outlined_icon.py
--rw-r--r--   0 runner    (1001) docker     (127)     1213 2024-05-23 14:23:55.000000 apysc-4.4.2/apysc/_material_design/icon/material_perm_media_icon.py
--rw-r--r--   0 runner    (1001) docker     (127)     1273 2024-05-23 14:23:55.000000 apysc-4.4.2/apysc/_material_design/icon/material_perm_media_outlined_icon.py
--rw-r--r--   0 runner    (1001) docker     (127)     1320 2024-05-23 14:23:55.000000 apysc-4.4.2/apysc/_material_design/icon/material_perm_phone_msg_icon.py
--rw-r--r--   0 runner    (1001) docker     (127)     1522 2024-05-23 14:23:55.000000 apysc-4.4.2/apysc/_material_design/icon/material_perm_phone_msg_outlined_icon.py
--rw-r--r--   0 runner    (1001) docker     (127)     1152 2024-05-23 14:23:55.000000 apysc-4.4.2/apysc/_material_design/icon/material_perm_scan_wifi_icon.py
--rw-r--r--   0 runner    (1001) docker     (127)     1251 2024-05-23 14:23:55.000000 apysc-4.4.2/apysc/_material_design/icon/material_perm_scan_wifi_outlined_icon.py
--rw-r--r--   0 runner    (1001) docker     (127)     1254 2024-05-23 14:23:55.000000 apysc-4.4.2/apysc/_material_design/icon/material_person_add_disabled_icon.py
--rw-r--r--   0 runner    (1001) docker     (127)     1512 2024-05-23 14:23:55.000000 apysc-4.4.2/apysc/_material_design/icon/material_person_add_disabled_outlined_icon.py
--rw-r--r--   0 runner    (1001) docker     (127)     1451 2024-05-23 14:23:55.000000 apysc-4.4.2/apysc/_material_design/icon/material_person_search_icon.py
--rw-r--r--   0 runner    (1001) docker     (127)     1682 2024-05-23 14:23:55.000000 apysc-4.4.2/apysc/_material_design/icon/material_person_search_outlined_icon.py
--rw-r--r--   0 runner    (1001) docker     (127)     1533 2024-05-23 14:23:55.000000 apysc-4.4.2/apysc/_material_design/icon/material_pets_icon.py
--rw-r--r--   0 runner    (1001) docker     (127)     1561 2024-05-23 14:23:55.000000 apysc-4.4.2/apysc/_material_design/icon/material_pets_outlined_icon.py
--rw-r--r--   0 runner    (1001) docker     (127)     1432 2024-05-23 14:23:55.000000 apysc-4.4.2/apysc/_material_design/icon/material_phone_disabled_icon.py
--rw-r--r--   0 runner    (1001) docker     (127)     1751 2024-05-23 14:23:55.000000 apysc-4.4.2/apysc/_material_design/icon/material_phone_disabled_outlined_icon.py
--rw-r--r--   0 runner    (1001) docker     (127)     1299 2024-05-23 14:23:55.000000 apysc-4.4.2/apysc/_material_design/icon/material_phone_enabled_icon.py
--rw-r--r--   0 runner    (1001) docker     (127)     1608 2024-05-23 14:23:55.000000 apysc-4.4.2/apysc/_material_design/icon/material_phone_enabled_outlined_icon.py
--rw-r--r--   0 runner    (1001) docker     (127)     1268 2024-05-23 14:23:55.000000 apysc-4.4.2/apysc/_material_design/icon/material_phone_icon.py
--rw-r--r--   0 runner    (1001) docker     (127)     1463 2024-05-23 14:23:55.000000 apysc-4.4.2/apysc/_material_design/icon/material_phone_outlined_icon.py
--rw-r--r--   0 runner    (1001) docker     (127)     1210 2024-05-23 14:23:55.000000 apysc-4.4.2/apysc/_material_design/icon/material_phonelink_erase_icon.py
--rw-r--r--   0 runner    (1001) docker     (127)     1236 2024-05-23 14:23:55.000000 apysc-4.4.2/apysc/_material_design/icon/material_phonelink_erase_outlined_icon.py
--rw-r--r--   0 runner    (1001) docker     (127)     1344 2024-05-23 14:23:55.000000 apysc-4.4.2/apysc/_material_design/icon/material_phonelink_lock_icon.py
--rw-r--r--   0 runner    (1001) docker     (127)     1370 2024-05-23 14:23:55.000000 apysc-4.4.2/apysc/_material_design/icon/material_phonelink_lock_outlined_icon.py
--rw-r--r--   0 runner    (1001) docker     (127)     1265 2024-05-23 14:23:55.000000 apysc-4.4.2/apysc/_material_design/icon/material_phonelink_ring_icon.py
--rw-r--r--   0 runner    (1001) docker     (127)     1291 2024-05-23 14:23:55.000000 apysc-4.4.2/apysc/_material_design/icon/material_phonelink_ring_outlined_icon.py
--rw-r--r--   0 runner    (1001) docker     (127)     1830 2024-05-23 14:23:55.000000 apysc-4.4.2/apysc/_material_design/icon/material_phonelink_setup_icon.py
--rw-r--r--   0 runner    (1001) docker     (127)     1860 2024-05-23 14:23:55.000000 apysc-4.4.2/apysc/_material_design/icon/material_phonelink_setup_outlined_icon.py
--rw-r--r--   0 runner    (1001) docker     (127)     1206 2024-05-23 14:23:55.000000 apysc-4.4.2/apysc/_material_design/icon/material_picture_in_picture_alt_icon.py
--rw-r--r--   0 runner    (1001) docker     (127)     1250 2024-05-23 14:23:55.000000 apysc-4.4.2/apysc/_material_design/icon/material_picture_in_picture_alt_outlined_icon.py
--rw-r--r--   0 runner    (1001) docker     (127)     1190 2024-05-23 14:23:55.000000 apysc-4.4.2/apysc/_material_design/icon/material_picture_in_picture_icon.py
--rw-r--r--   0 runner    (1001) docker     (127)     1233 2024-05-23 14:23:55.000000 apysc-4.4.2/apysc/_material_design/icon/material_picture_in_picture_outlined_icon.py
--rw-r--r--   0 runner    (1001) docker     (127)     1398 2024-05-23 14:23:55.000000 apysc-4.4.2/apysc/_material_design/icon/material_plagiarism_icon.py
--rw-r--r--   0 runner    (1001) docker     (127)     1536 2024-05-23 14:23:55.000000 apysc-4.4.2/apysc/_material_design/icon/material_plagiarism_outlined_icon.py
--rw-r--r--   0 runner    (1001) docker     (127)     1055 2024-05-23 14:23:55.000000 apysc-4.4.2/apysc/_material_design/icon/material_play_arrow_icon.py
--rw-r--r--   0 runner    (1001) docker     (127)     1118 2024-05-23 14:23:55.000000 apysc-4.4.2/apysc/_material_design/icon/material_play_arrow_outlined_icon.py
--rw-r--r--   0 runner    (1001) docker     (127)     1155 2024-05-23 14:23:55.000000 apysc-4.4.2/apysc/_material_design/icon/material_play_circle_filled_icon.py
--rw-r--r--   0 runner    (1001) docker     (127)     1183 2024-05-23 14:23:55.000000 apysc-4.4.2/apysc/_material_design/icon/material_play_circle_filled_outlined_icon.py
--rw-r--r--   0 runner    (1001) docker     (127)     1215 2024-05-23 14:23:55.000000 apysc-4.4.2/apysc/_material_design/icon/material_play_circle_outline_icon.py
--rw-r--r--   0 runner    (1001) docker     (127)     1241 2024-05-23 14:23:55.000000 apysc-4.4.2/apysc/_material_design/icon/material_play_circle_outline_outlined_icon.py
--rw-r--r--   0 runner    (1001) docker     (127)     1203 2024-05-23 14:23:55.000000 apysc-4.4.2/apysc/_material_design/icon/material_play_disabled_icon.py
--rw-r--r--   0 runner    (1001) docker     (127)     1159 2024-05-23 14:23:55.000000 apysc-4.4.2/apysc/_material_design/icon/material_play_for_work_icon.py
--rw-r--r--   0 runner    (1001) docker     (127)     1187 2024-05-23 14:23:55.000000 apysc-4.4.2/apysc/_material_design/icon/material_play_for_work_outlined_icon.py
--rw-r--r--   0 runner    (1001) docker     (127)     1241 2024-05-23 14:23:55.000000 apysc-4.4.2/apysc/_material_design/icon/material_playlist_add_check_icon.py
--rw-r--r--   0 runner    (1001) docker     (127)     1194 2024-05-23 14:23:55.000000 apysc-4.4.2/apysc/_material_design/icon/material_playlist_add_check_outlined_icon.py
--rw-r--r--   0 runner    (1001) docker     (127)     1129 2024-05-23 14:23:55.000000 apysc-4.4.2/apysc/_material_design/icon/material_playlist_add_icon.py
--rw-r--r--   0 runner    (1001) docker     (127)     1157 2024-05-23 14:23:55.000000 apysc-4.4.2/apysc/_material_design/icon/material_playlist_add_outlined_icon.py
--rw-r--r--   0 runner    (1001) docker     (127)     1101 2024-05-23 14:23:55.000000 apysc-4.4.2/apysc/_material_design/icon/material_playlist_play_icon.py
--rw-r--r--   0 runner    (1001) docker     (127)     1127 2024-05-23 14:23:55.000000 apysc-4.4.2/apysc/_material_design/icon/material_playlist_play_outlined_icon.py
--rw-r--r--   0 runner    (1001) docker     (127)     1359 2024-05-23 14:23:55.000000 apysc-4.4.2/apysc/_material_design/icon/material_policy_icon.py
--rw-r--r--   0 runner    (1001) docker     (127)     1500 2024-05-23 14:23:55.000000 apysc-4.4.2/apysc/_material_design/icon/material_policy_outlined_icon.py
--rw-r--r--   0 runner    (1001) docker     (127)     1113 2024-05-23 14:23:55.000000 apysc-4.4.2/apysc/_material_design/icon/material_polymer_icon.py
--rw-r--r--   0 runner    (1001) docker     (127)     1146 2024-05-23 14:23:55.000000 apysc-4.4.2/apysc/_material_design/icon/material_polymer_outlined_icon.py
--rw-r--r--   0 runner    (1001) docker     (127)     1710 2024-05-23 14:23:55.000000 apysc-4.4.2/apysc/_material_design/icon/material_portable_wifi_off_icon.py
--rw-r--r--   0 runner    (1001) docker     (127)     1716 2024-05-23 14:23:55.000000 apysc-4.4.2/apysc/_material_design/icon/material_portable_wifi_off_outlined_icon.py
--rw-r--r--   0 runner    (1001) docker     (127)     1273 2024-05-23 14:23:55.000000 apysc-4.4.2/apysc/_material_design/icon/material_power_settings_new_icon.py
--rw-r--r--   0 runner    (1001) docker     (127)     1301 2024-05-23 14:23:55.000000 apysc-4.4.2/apysc/_material_design/icon/material_power_settings_new_outlined_icon.py
--rw-r--r--   0 runner    (1001) docker     (127)     1264 2024-05-23 14:23:55.000000 apysc-4.4.2/apysc/_material_design/icon/material_pregnant_woman_icon.py
--rw-r--r--   0 runner    (1001) docker     (127)     1205 2024-05-23 14:23:55.000000 apysc-4.4.2/apysc/_material_design/icon/material_pregnant_woman_outlined_icon.py
--rw-r--r--   0 runner    (1001) docker     (127)     1192 2024-05-23 14:23:55.000000 apysc-4.4.2/apysc/_material_design/icon/material_present_to_all_icon.py
--rw-r--r--   0 runner    (1001) docker     (127)     1218 2024-05-23 14:23:55.000000 apysc-4.4.2/apysc/_material_design/icon/material_present_to_all_outlined_icon.py
--rw-r--r--   0 runner    (1001) docker     (127)     1484 2024-05-23 14:23:55.000000 apysc-4.4.2/apysc/_material_design/icon/material_preview_icon.py
--rw-r--r--   0 runner    (1001) docker     (127)     1507 2024-05-23 14:23:55.000000 apysc-4.4.2/apysc/_material_design/icon/material_preview_outlined_icon.py
--rw-r--r--   0 runner    (1001) docker     (127)     1256 2024-05-23 14:23:55.000000 apysc-4.4.2/apysc/_material_design/icon/material_print_disabled_icon.py
--rw-r--r--   0 runner    (1001) docker     (127)     1345 2024-05-23 14:23:55.000000 apysc-4.4.2/apysc/_material_design/icon/material_print_disabled_outlined_icon.py
--rw-r--r--   0 runner    (1001) docker     (127)     1173 2024-05-23 14:23:55.000000 apysc-4.4.2/apysc/_material_design/icon/material_print_icon.py
--rw-r--r--   0 runner    (1001) docker     (127)     1246 2024-05-23 14:23:55.000000 apysc-4.4.2/apysc/_material_design/icon/material_print_outlined_icon.py
--rw-r--r--   0 runner    (1001) docker     (127)     1194 2024-05-23 14:23:55.000000 apysc-4.4.2/apysc/_material_design/icon/material_privacy_tip_icon.py
--rw-r--r--   0 runner    (1001) docker     (127)     1300 2024-05-23 14:23:55.000000 apysc-4.4.2/apysc/_material_design/icon/material_privacy_tip_outlined_icon.py
--rw-r--r--   0 runner    (1001) docker     (127)     1458 2024-05-23 14:23:55.000000 apysc-4.4.2/apysc/_material_design/icon/material_published_with_changes_icon.py
--rw-r--r--   0 runner    (1001) docker     (127)     1481 2024-05-23 14:23:55.000000 apysc-4.4.2/apysc/_material_design/icon/material_published_with_changes_outlined_icon.py
--rw-r--r--   0 runner    (1001) docker     (127)     1277 2024-05-23 14:23:55.000000 apysc-4.4.2/apysc/_material_design/icon/material_push_pin_icon.py
--rw-r--r--   0 runner    (1001) docker     (127)     1372 2024-05-23 14:23:55.000000 apysc-4.4.2/apysc/_material_design/icon/material_push_pin_outlined_icon.py
--rw-r--r--   0 runner    (1001) docker     (127)     1545 2024-05-23 14:23:55.000000 apysc-4.4.2/apysc/_material_design/icon/material_qr_code_icon.py
--rw-r--r--   0 runner    (1001) docker     (127)     1571 2024-05-23 14:23:55.000000 apysc-4.4.2/apysc/_material_design/icon/material_qr_code_outlined_icon.py
--rw-r--r--   0 runner    (1001) docker     (127)     1512 2024-05-23 14:23:55.000000 apysc-4.4.2/apysc/_material_design/icon/material_qr_code_scanner_icon.py
--rw-r--r--   0 runner    (1001) docker     (127)     1538 2024-05-23 14:23:55.000000 apysc-4.4.2/apysc/_material_design/icon/material_qr_code_scanner_outlined_icon.py
--rw-r--r--   0 runner    (1001) docker     (127)     1246 2024-05-23 14:23:55.000000 apysc-4.4.2/apysc/_material_design/icon/material_query_builder_icon.py
--rw-r--r--   0 runner    (1001) docker     (127)     1261 2024-05-23 14:23:55.000000 apysc-4.4.2/apysc/_material_design/icon/material_query_builder_outlined_icon.py
--rw-r--r--   0 runner    (1001) docker     (127)     1181 2024-05-23 14:23:55.000000 apysc-4.4.2/apysc/_material_design/icon/material_question_answer_icon.py
--rw-r--r--   0 runner    (1001) docker     (127)     1239 2024-05-23 14:23:55.000000 apysc-4.4.2/apysc/_material_design/icon/material_question_answer_outlined_icon.py
--rw-r--r--   0 runner    (1001) docker     (127)     1171 2024-05-23 14:23:55.000000 apysc-4.4.2/apysc/_material_design/icon/material_queue_icon.py
--rw-r--r--   0 runner    (1001) docker     (127)     1173 2024-05-23 14:23:55.000000 apysc-4.4.2/apysc/_material_design/icon/material_queue_music_icon.py
--rw-r--r--   0 runner    (1001) docker     (127)     1560 2024-05-23 14:23:55.000000 apysc-4.4.2/apysc/_material_design/icon/material_queue_music_outlined_icon.py
--rw-r--r--   0 runner    (1001) docker     (127)     1213 2024-05-23 14:23:55.000000 apysc-4.4.2/apysc/_material_design/icon/material_queue_outlined_icon.py
--rw-r--r--   0 runner    (1001) docker     (127)     1305 2024-05-23 14:23:55.000000 apysc-4.4.2/apysc/_material_design/icon/material_queue_play_next_icon.py
--rw-r--r--   0 runner    (1001) docker     (127)     1248 2024-05-23 14:23:55.000000 apysc-4.4.2/apysc/_material_design/icon/material_queue_play_next_outlined_icon.py
--rw-r--r--   0 runner    (1001) docker     (127)     1246 2024-05-23 14:23:55.000000 apysc-4.4.2/apysc/_material_design/icon/material_quickreply_icon.py
--rw-r--r--   0 runner    (1001) docker     (127)     1295 2024-05-23 14:23:55.000000 apysc-4.4.2/apysc/_material_design/icon/material_quickreply_outlined_icon.py
--rw-r--r--   0 runner    (1001) docker     (127)     1232 2024-05-23 14:23:55.000000 apysc-4.4.2/apysc/_material_design/icon/material_radio_icon.py
--rw-r--r--   0 runner    (1001) docker     (127)     1246 2024-05-23 14:23:55.000000 apysc-4.4.2/apysc/_material_design/icon/material_radio_outlined_icon.py
--rw-r--r--   0 runner    (1001) docker     (127)     1266 2024-05-23 14:23:55.000000 apysc-4.4.2/apysc/_material_design/icon/material_read_more_icon.py
--rw-r--r--   0 runner    (1001) docker     (127)     1292 2024-05-23 14:23:55.000000 apysc-4.4.2/apysc/_material_design/icon/material_read_more_outlined_icon.py
--rw-r--r--   0 runner    (1001) docker     (127)     1252 2024-05-23 14:23:55.000000 apysc-4.4.2/apysc/_material_design/icon/material_receipt_icon.py
--rw-r--r--   0 runner    (1001) docker     (127)     1301 2024-05-23 14:23:55.000000 apysc-4.4.2/apysc/_material_design/icon/material_receipt_outlined_icon.py
--rw-r--r--   0 runner    (1001) docker     (127)     1312 2024-05-23 14:23:55.000000 apysc-4.4.2/apysc/_material_design/icon/material_recent_actors_icon.py
--rw-r--r--   0 runner    (1001) docker     (127)     1322 2024-05-23 14:23:55.000000 apysc-4.4.2/apysc/_material_design/icon/material_recent_actors_outlined_icon.py
--rw-r--r--   0 runner    (1001) docker     (127)     1306 2024-05-23 14:23:55.000000 apysc-4.4.2/apysc/_material_design/icon/material_record_voice_over_icon.py
--rw-r--r--   0 runner    (1001) docker     (127)     1457 2024-05-23 14:23:55.000000 apysc-4.4.2/apysc/_material_design/icon/material_record_voice_over_outlined_icon.py
--rw-r--r--   0 runner    (1001) docker     (127)     1467 2024-05-23 14:23:55.000000 apysc-4.4.2/apysc/_material_design/icon/material_redeem_icon.py
--rw-r--r--   0 runner    (1001) docker     (127)     1495 2024-05-23 14:23:55.000000 apysc-4.4.2/apysc/_material_design/icon/material_redeem_outlined_icon.py
--rw-r--r--   0 runner    (1001) docker     (127)     1168 2024-05-23 14:23:55.000000 apysc-4.4.2/apysc/_material_design/icon/material_redo_icon.py
--rw-r--r--   0 runner    (1001) docker     (127)     1196 2024-05-23 14:23:55.000000 apysc-4.4.2/apysc/_material_design/icon/material_redo_outlined_icon.py
--rw-r--r--   0 runner    (1001) docker     (127)     1133 2024-05-23 14:23:55.000000 apysc-4.4.2/apysc/_material_design/icon/material_remove_circle_icon.py
--rw-r--r--   0 runner    (1001) docker     (127)     1213 2024-05-23 14:23:55.000000 apysc-4.4.2/apysc/_material_design/icon/material_remove_circle_outline_icon.py
--rw-r--r--   0 runner    (1001) docker     (127)     1241 2024-05-23 14:23:55.000000 apysc-4.4.2/apysc/_material_design/icon/material_remove_circle_outline_outlined_icon.py
--rw-r--r--   0 runner    (1001) docker     (127)     1161 2024-05-23 14:23:55.000000 apysc-4.4.2/apysc/_material_design/icon/material_remove_circle_outlined_icon.py
--rw-r--r--   0 runner    (1001) docker     (127)     1313 2024-05-23 14:23:55.000000 apysc-4.4.2/apysc/_material_design/icon/material_remove_done_icon.py
--rw-r--r--   0 runner    (1001) docker     (127)     1276 2024-05-23 14:23:55.000000 apysc-4.4.2/apysc/_material_design/icon/material_remove_from_queue_icon.py
--rw-r--r--   0 runner    (1001) docker     (127)     1209 2024-05-23 14:23:55.000000 apysc-4.4.2/apysc/_material_design/icon/material_remove_from_queue_outlined_icon.py
--rw-r--r--   0 runner    (1001) docker     (127)     1048 2024-05-23 14:23:55.000000 apysc-4.4.2/apysc/_material_design/icon/material_remove_icon.py
--rw-r--r--   0 runner    (1001) docker     (127)     1076 2024-05-23 14:23:55.000000 apysc-4.4.2/apysc/_material_design/icon/material_remove_outlined_icon.py
--rw-r--r--   0 runner    (1001) docker     (127)     1490 2024-05-23 14:23:55.000000 apysc-4.4.2/apysc/_material_design/icon/material_remove_shopping_cart_icon.py
--rw-r--r--   0 runner    (1001) docker     (127)     1474 2024-05-23 14:23:55.000000 apysc-4.4.2/apysc/_material_design/icon/material_remove_shopping_cart_outlined_icon.py
--rw-r--r--   0 runner    (1001) docker     (127)     1093 2024-05-23 14:23:55.000000 apysc-4.4.2/apysc/_material_design/icon/material_reorder_icon.py
--rw-r--r--   0 runner    (1001) docker     (127)     1121 2024-05-23 14:23:55.000000 apysc-4.4.2/apysc/_material_design/icon/material_reorder_outlined_icon.py
--rw-r--r--   0 runner    (1001) docker     (127)     1094 2024-05-23 14:23:55.000000 apysc-4.4.2/apysc/_material_design/icon/material_repeat_icon.py
--rw-r--r--   0 runner    (1001) docker     (127)     1200 2024-05-23 14:23:55.000000 apysc-4.4.2/apysc/_material_design/icon/material_repeat_on_icon.py
--rw-r--r--   0 runner    (1001) docker     (127)     1132 2024-05-23 14:23:55.000000 apysc-4.4.2/apysc/_material_design/icon/material_repeat_one_icon.py
--rw-r--r--   0 runner    (1001) docker     (127)     1238 2024-05-23 14:23:55.000000 apysc-4.4.2/apysc/_material_design/icon/material_repeat_one_on_icon.py
--rw-r--r--   0 runner    (1001) docker     (127)     1160 2024-05-23 14:23:55.000000 apysc-4.4.2/apysc/_material_design/icon/material_repeat_one_outlined_icon.py
--rw-r--r--   0 runner    (1001) docker     (127)     1122 2024-05-23 14:23:55.000000 apysc-4.4.2/apysc/_material_design/icon/material_repeat_outlined_icon.py
--rw-r--r--   0 runner    (1001) docker     (127)     2032 2024-05-23 14:23:55.000000 apysc-4.4.2/apysc/_material_design/icon/material_replay_10_icon.py
--rw-r--r--   0 runner    (1001) docker     (127)     1724 2024-05-23 14:23:55.000000 apysc-4.4.2/apysc/_material_design/icon/material_replay_10_outlined_icon.py
--rw-r--r--   0 runner    (1001) docker     (127)     2997 2024-05-23 14:23:55.000000 apysc-4.4.2/apysc/_material_design/icon/material_replay_30_icon.py
--rw-r--r--   0 runner    (1001) docker     (127)     2408 2024-05-23 14:23:55.000000 apysc-4.4.2/apysc/_material_design/icon/material_replay_30_outlined_icon.py
--rw-r--r--   0 runner    (1001) docker     (127)     1948 2024-05-23 14:23:55.000000 apysc-4.4.2/apysc/_material_design/icon/material_replay_5_icon.py
--rw-r--r--   0 runner    (1001) docker     (127)     1689 2024-05-23 14:23:55.000000 apysc-4.4.2/apysc/_material_design/icon/material_replay_5_outlined_icon.py
--rw-r--r--   0 runner    (1001) docker     (127)     1267 2024-05-23 14:23:55.000000 apysc-4.4.2/apysc/_material_design/icon/material_replay_circle_filled_icon.py
--rw-r--r--   0 runner    (1001) docker     (127)     1132 2024-05-23 14:23:55.000000 apysc-4.4.2/apysc/_material_design/icon/material_replay_icon.py
--rw-r--r--   0 runner    (1001) docker     (127)     1302 2024-05-23 14:23:55.000000 apysc-4.4.2/apysc/_material_design/icon/material_replay_outlined_icon.py
--rw-r--r--   0 runner    (1001) docker     (127)     1122 2024-05-23 14:23:55.000000 apysc-4.4.2/apysc/_material_design/icon/material_reply_all_icon.py
--rw-r--r--   0 runner    (1001) docker     (127)     1150 2024-05-23 14:23:55.000000 apysc-4.4.2/apysc/_material_design/icon/material_reply_all_outlined_icon.py
--rw-r--r--   0 runner    (1001) docker     (127)     1084 2024-05-23 14:23:55.000000 apysc-4.4.2/apysc/_material_design/icon/material_reply_icon.py
--rw-r--r--   0 runner    (1001) docker     (127)     1112 2024-05-23 14:23:55.000000 apysc-4.4.2/apysc/_material_design/icon/material_reply_outlined_icon.py
--rw-r--r--   0 runner    (1001) docker     (127)     1270 2024-05-23 14:23:55.000000 apysc-4.4.2/apysc/_material_design/icon/material_report_gmailerrorred_outlined_icon.py
--rw-r--r--   0 runner    (1001) docker     (127)     1203 2024-05-23 14:23:55.000000 apysc-4.4.2/apysc/_material_design/icon/material_report_icon.py
--rw-r--r--   0 runner    (1001) docker     (127)     1279 2024-05-23 14:23:55.000000 apysc-4.4.2/apysc/_material_design/icon/material_report_off_icon.py
--rw-r--r--   0 runner    (1001) docker     (127)     1352 2024-05-23 14:23:55.000000 apysc-4.4.2/apysc/_material_design/icon/material_report_off_outlined_icon.py
--rw-r--r--   0 runner    (1001) docker     (127)     1229 2024-05-23 14:23:55.000000 apysc-4.4.2/apysc/_material_design/icon/material_report_outlined_icon.py
--rw-r--r--   0 runner    (1001) docker     (127)     1104 2024-05-23 14:23:55.000000 apysc-4.4.2/apysc/_material_design/icon/material_report_problem_icon.py
--rw-r--r--   0 runner    (1001) docker     (127)     1162 2024-05-23 14:23:55.000000 apysc-4.4.2/apysc/_material_design/icon/material_report_problem_outlined_icon.py
--rw-r--r--   0 runner    (1001) docker     (127)     1287 2024-05-23 14:23:55.000000 apysc-4.4.2/apysc/_material_design/icon/material_request_page_icon.py
--rw-r--r--   0 runner    (1001) docker     (127)     1348 2024-05-23 14:23:55.000000 apysc-4.4.2/apysc/_material_design/icon/material_request_page_outlined_icon.py
--rw-r--r--   0 runner    (1001) docker     (127)     1165 2024-05-23 14:23:55.000000 apysc-4.4.2/apysc/_material_design/icon/material_restore_from_trash_icon.py
--rw-r--r--   0 runner    (1001) docker     (127)     1207 2024-05-23 14:23:55.000000 apysc-4.4.2/apysc/_material_design/icon/material_restore_from_trash_outlined_icon.py
--rw-r--r--   0 runner    (1001) docker     (127)     1258 2024-05-23 14:23:55.000000 apysc-4.4.2/apysc/_material_design/icon/material_restore_icon.py
--rw-r--r--   0 runner    (1001) docker     (127)     1275 2024-05-23 14:23:55.000000 apysc-4.4.2/apysc/_material_design/icon/material_restore_outlined_icon.py
--rw-r--r--   0 runner    (1001) docker     (127)     1325 2024-05-23 14:23:55.000000 apysc-4.4.2/apysc/_material_design/icon/material_restore_page_icon.py
--rw-r--r--   0 runner    (1001) docker     (127)     1421 2024-05-23 14:23:55.000000 apysc-4.4.2/apysc/_material_design/icon/material_restore_page_outlined_icon.py
--rw-r--r--   0 runner    (1001) docker     (127)     1571 2024-05-23 14:23:55.000000 apysc-4.4.2/apysc/_material_design/icon/material_ring_volume_icon.py
--rw-r--r--   0 runner    (1001) docker     (127)     1761 2024-05-23 14:23:55.000000 apysc-4.4.2/apysc/_material_design/icon/material_ring_volume_outlined_icon.py
--rw-r--r--   0 runner    (1001) docker     (127)     1179 2024-05-23 14:23:55.000000 apysc-4.4.2/apysc/_material_design/icon/material_room_icon.py
--rw-r--r--   0 runner    (1001) docker     (127)     1237 2024-05-23 14:23:55.000000 apysc-4.4.2/apysc/_material_design/icon/material_room_outlined_icon.py
--rw-r--r--   0 runner    (1001) docker     (127)     1381 2024-05-23 14:23:55.000000 apysc-4.4.2/apysc/_material_design/icon/material_rounded_corner_icon.py
--rw-r--r--   0 runner    (1001) docker     (127)     1312 2024-05-23 14:23:55.000000 apysc-4.4.2/apysc/_material_design/icon/material_rounded_corner_outlined_icon.py
--rw-r--r--   0 runner    (1001) docker     (127)     1471 2024-05-23 14:23:55.000000 apysc-4.4.2/apysc/_material_design/icon/material_rowing_icon.py
--rw-r--r--   0 runner    (1001) docker     (127)     1415 2024-05-23 14:23:55.000000 apysc-4.4.2/apysc/_material_design/icon/material_rowing_outlined_icon.py
--rw-r--r--   0 runner    (1001) docker     (127)     1220 2024-05-23 14:23:55.000000 apysc-4.4.2/apysc/_material_design/icon/material_rss_feed_icon.py
--rw-r--r--   0 runner    (1001) docker     (127)     1248 2024-05-23 14:23:55.000000 apysc-4.4.2/apysc/_material_design/icon/material_rss_feed_outlined_icon.py
--rw-r--r--   0 runner    (1001) docker     (127)     1275 2024-05-23 14:23:55.000000 apysc-4.4.2/apysc/_material_design/icon/material_rtt_icon.py
--rw-r--r--   0 runner    (1001) docker     (127)     1290 2024-05-23 14:23:55.000000 apysc-4.4.2/apysc/_material_design/icon/material_rule_icon.py
--rw-r--r--   0 runner    (1001) docker     (127)     1316 2024-05-23 14:23:55.000000 apysc-4.4.2/apysc/_material_design/icon/material_rule_outlined_icon.py
--rw-r--r--   0 runner    (1001) docker     (127)     1150 2024-05-23 14:23:55.000000 apysc-4.4.2/apysc/_material_design/icon/material_save_alt_icon.py
--rw-r--r--   0 runner    (1001) docker     (127)     1183 2024-05-23 14:23:55.000000 apysc-4.4.2/apysc/_material_design/icon/material_save_alt_outlined_icon.py
--rw-r--r--   0 runner    (1001) docker     (127)     1167 2024-05-23 14:23:55.000000 apysc-4.4.2/apysc/_material_design/icon/material_save_icon.py
--rw-r--r--   0 runner    (1001) docker     (127)     1217 2024-05-23 14:23:55.000000 apysc-4.4.2/apysc/_material_design/icon/material_save_outlined_icon.py
--rw-r--r--   0 runner    (1001) docker     (127)     1366 2024-05-23 14:23:55.000000 apysc-4.4.2/apysc/_material_design/icon/material_saved_search_icon.py
--rw-r--r--   0 runner    (1001) docker     (127)     1232 2024-05-23 14:23:55.000000 apysc-4.4.2/apysc/_material_design/icon/material_schedule_icon.py
--rw-r--r--   0 runner    (1001) docker     (127)     1247 2024-05-23 14:23:55.000000 apysc-4.4.2/apysc/_material_design/icon/material_schedule_outlined_icon.py
--rw-r--r--   0 runner    (1001) docker     (127)     1281 2024-05-23 14:23:55.000000 apysc-4.4.2/apysc/_material_design/icon/material_schedule_send_icon.py
--rw-r--r--   0 runner    (1001) docker     (127)     1229 2024-05-23 14:23:55.000000 apysc-4.4.2/apysc/_material_design/icon/material_screen_share_icon.py
--rw-r--r--   0 runner    (1001) docker     (127)     1280 2024-05-23 14:23:55.000000 apysc-4.4.2/apysc/_material_design/icon/material_screen_share_outlined_icon.py
--rw-r--r--   0 runner    (1001) docker     (127)     1313 2024-05-23 14:23:55.000000 apysc-4.4.2/apysc/_material_design/icon/material_sd_icon.py
--rw-r--r--   0 runner    (1001) docker     (127)     1265 2024-05-23 14:23:55.000000 apysc-4.4.2/apysc/_material_design/icon/material_search_icon.py
--rw-r--r--   0 runner    (1001) docker     (127)     1532 2024-05-23 14:23:55.000000 apysc-4.4.2/apysc/_material_design/icon/material_search_off_icon.py
--rw-r--r--   0 runner    (1001) docker     (127)     1558 2024-05-23 14:23:55.000000 apysc-4.4.2/apysc/_material_design/icon/material_search_off_outlined_icon.py
--rw-r--r--   0 runner    (1001) docker     (127)     1293 2024-05-23 14:23:55.000000 apysc-4.4.2/apysc/_material_design/icon/material_search_outlined_icon.py
--rw-r--r--   0 runner    (1001) docker     (127)     1081 2024-05-23 14:23:55.000000 apysc-4.4.2/apysc/_material_design/icon/material_segment_icon.py
--rw-r--r--   0 runner    (1001) docker     (127)     1346 2024-05-23 14:23:55.000000 apysc-4.4.2/apysc/_material_design/icon/material_select_all_icon.py
--rw-r--r--   0 runner    (1001) docker     (127)     1374 2024-05-23 14:23:55.000000 apysc-4.4.2/apysc/_material_design/icon/material_select_all_outlined_icon.py
--rw-r--r--   0 runner    (1001) docker     (127)     1193 2024-05-23 14:23:55.000000 apysc-4.4.2/apysc/_material_design/icon/material_send_and_archive_icon.py
--rw-r--r--   0 runner    (1001) docker     (127)     1062 2024-05-23 14:23:55.000000 apysc-4.4.2/apysc/_material_design/icon/material_send_icon.py
--rw-r--r--   0 runner    (1001) docker     (127)     1161 2024-05-23 14:23:55.000000 apysc-4.4.2/apysc/_material_design/icon/material_send_outlined_icon.py
--rw-r--r--   0 runner    (1001) docker     (127)     1517 2024-05-23 14:23:55.000000 apysc-4.4.2/apysc/_material_design/icon/material_sentiment_satisfied_alt_icon.py
--rw-r--r--   0 runner    (1001) docker     (127)     1433 2024-05-23 14:23:55.000000 apysc-4.4.2/apysc/_material_design/icon/material_sentiment_satisfied_alt_outlined_icon.py
--rw-r--r--   0 runner    (1001) docker     (127)     1804 2024-05-23 14:23:55.000000 apysc-4.4.2/apysc/_material_design/icon/material_settings_applications_icon.py
--rw-r--r--   0 runner    (1001) docker     (127)     1884 2024-05-23 14:23:55.000000 apysc-4.4.2/apysc/_material_design/icon/material_settings_applications_outlined_icon.py
--rw-r--r--   0 runner    (1001) docker     (127)     1298 2024-05-23 14:23:55.000000 apysc-4.4.2/apysc/_material_design/icon/material_settings_backup_restore_icon.py
--rw-r--r--   0 runner    (1001) docker     (127)     1326 2024-05-23 14:23:55.000000 apysc-4.4.2/apysc/_material_design/icon/material_settings_backup_restore_outlined_icon.py
--rw-r--r--   0 runner    (1001) docker     (127)     1288 2024-05-23 14:23:55.000000 apysc-4.4.2/apysc/_material_design/icon/material_settings_bluetooth_icon.py
--rw-r--r--   0 runner    (1001) docker     (127)     1316 2024-05-23 14:23:55.000000 apysc-4.4.2/apysc/_material_design/icon/material_settings_bluetooth_outlined_icon.py
--rw-r--r--   0 runner    (1001) docker     (127)     1301 2024-05-23 14:23:55.000000 apysc-4.4.2/apysc/_material_design/icon/material_settings_brightness_icon.py
--rw-r--r--   0 runner    (1001) docker     (127)     1329 2024-05-23 14:23:55.000000 apysc-4.4.2/apysc/_material_design/icon/material_settings_brightness_outlined_icon.py
--rw-r--r--   0 runner    (1001) docker     (127)     1196 2024-05-23 14:23:55.000000 apysc-4.4.2/apysc/_material_design/icon/material_settings_cell_icon.py
--rw-r--r--   0 runner    (1001) docker     (127)     1243 2024-05-23 14:23:55.000000 apysc-4.4.2/apysc/_material_design/icon/material_settings_cell_outlined_icon.py
--rw-r--r--   0 runner    (1001) docker     (127)     1247 2024-05-23 14:23:55.000000 apysc-4.4.2/apysc/_material_design/icon/material_settings_ethernet_icon.py
--rw-r--r--   0 runner    (1001) docker     (127)     1275 2024-05-23 14:23:55.000000 apysc-4.4.2/apysc/_material_design/icon/material_settings_ethernet_outlined_icon.py
--rw-r--r--   0 runner    (1001) docker     (127)     1938 2024-05-23 14:23:55.000000 apysc-4.4.2/apysc/_material_design/icon/material_settings_icon.py
--rw-r--r--   0 runner    (1001) docker     (127)     1381 2024-05-23 14:23:55.000000 apysc-4.4.2/apysc/_material_design/icon/material_settings_input_antenna_icon.py
--rw-r--r--   0 runner    (1001) docker     (127)     1409 2024-05-23 14:23:55.000000 apysc-4.4.2/apysc/_material_design/icon/material_settings_input_antenna_outlined_icon.py
--rw-r--r--   0 runner    (1001) docker     (127)     1427 2024-05-23 14:23:55.000000 apysc-4.4.2/apysc/_material_design/icon/material_settings_input_component_icon.py
--rw-r--r--   0 runner    (1001) docker     (127)     1596 2024-05-23 14:23:55.000000 apysc-4.4.2/apysc/_material_design/icon/material_settings_input_component_outlined_icon.py
--rw-r--r--   0 runner    (1001) docker     (127)     1427 2024-05-23 14:23:55.000000 apysc-4.4.2/apysc/_material_design/icon/material_settings_input_composite_icon.py
--rw-r--r--   0 runner    (1001) docker     (127)     1596 2024-05-23 14:23:55.000000 apysc-4.4.2/apysc/_material_design/icon/material_settings_input_composite_outlined_icon.py
--rw-r--r--   0 runner    (1001) docker     (127)     1168 2024-05-23 14:23:55.000000 apysc-4.4.2/apysc/_material_design/icon/material_settings_input_hdmi_icon.py
--rw-r--r--   0 runner    (1001) docker     (127)     1239 2024-05-23 14:23:55.000000 apysc-4.4.2/apysc/_material_design/icon/material_settings_input_hdmi_outlined_icon.py
--rw-r--r--   0 runner    (1001) docker     (127)     1591 2024-05-23 14:23:55.000000 apysc-4.4.2/apysc/_material_design/icon/material_settings_input_svideo_icon.py
--rw-r--r--   0 runner    (1001) docker     (127)     1619 2024-05-23 14:23:55.000000 apysc-4.4.2/apysc/_material_design/icon/material_settings_input_svideo_outlined_icon.py
--rw-r--r--   0 runner    (1001) docker     (127)     2368 2024-05-23 14:23:55.000000 apysc-4.4.2/apysc/_material_design/icon/material_settings_outlined_icon.py
--rw-r--r--   0 runner    (1001) docker     (127)     1263 2024-05-23 14:23:55.000000 apysc-4.4.2/apysc/_material_design/icon/material_settings_overscan_icon.py
--rw-r--r--   0 runner    (1001) docker     (127)     1291 2024-05-23 14:23:55.000000 apysc-4.4.2/apysc/_material_design/icon/material_settings_overscan_outlined_icon.py
--rw-r--r--   0 runner    (1001) docker     (127)     1343 2024-05-23 14:23:55.000000 apysc-4.4.2/apysc/_material_design/icon/material_settings_phone_icon.py
--rw-r--r--   0 runner    (1001) docker     (127)     1525 2024-05-23 14:23:55.000000 apysc-4.4.2/apysc/_material_design/icon/material_settings_phone_outlined_icon.py
--rw-r--r--   0 runner    (1001) docker     (127)     1309 2024-05-23 14:23:55.000000 apysc-4.4.2/apysc/_material_design/icon/material_settings_power_icon.py
--rw-r--r--   0 runner    (1001) docker     (127)     1337 2024-05-23 14:23:55.000000 apysc-4.4.2/apysc/_material_design/icon/material_settings_power_outlined_icon.py
--rw-r--r--   0 runner    (1001) docker     (127)     1420 2024-05-23 14:23:55.000000 apysc-4.4.2/apysc/_material_design/icon/material_settings_remote_icon.py
--rw-r--r--   0 runner    (1001) docker     (127)     1460 2024-05-23 14:23:55.000000 apysc-4.4.2/apysc/_material_design/icon/material_settings_remote_outlined_icon.py
--rw-r--r--   0 runner    (1001) docker     (127)     1291 2024-05-23 14:23:55.000000 apysc-4.4.2/apysc/_material_design/icon/material_settings_voice_icon.py
--rw-r--r--   0 runner    (1001) docker     (127)     1366 2024-05-23 14:23:55.000000 apysc-4.4.2/apysc/_material_design/icon/material_settings_voice_outlined_icon.py
--rw-r--r--   0 runner    (1001) docker     (127)     1153 2024-05-23 14:23:55.000000 apysc-4.4.2/apysc/_material_design/icon/material_shop_icon.py
--rw-r--r--   0 runner    (1001) docker     (127)     1195 2024-05-23 14:23:55.000000 apysc-4.4.2/apysc/_material_design/icon/material_shop_outlined_icon.py
--rw-r--r--   0 runner    (1001) docker     (127)     1215 2024-05-23 14:23:55.000000 apysc-4.4.2/apysc/_material_design/icon/material_shop_two_icon.py
--rw-r--r--   0 runner    (1001) docker     (127)     1255 2024-05-23 14:23:55.000000 apysc-4.4.2/apysc/_material_design/icon/material_shop_two_outlined_icon.py
--rw-r--r--   0 runner    (1001) docker     (127)     1345 2024-05-23 14:23:55.000000 apysc-4.4.2/apysc/_material_design/icon/material_shopping_bag_icon.py
--rw-r--r--   0 runner    (1001) docker     (127)     1368 2024-05-23 14:23:55.000000 apysc-4.4.2/apysc/_material_design/icon/material_shopping_bag_outlined_icon.py
--rw-r--r--   0 runner    (1001) docker     (127)     1332 2024-05-23 14:23:55.000000 apysc-4.4.2/apysc/_material_design/icon/material_shopping_basket_icon.py
--rw-r--r--   0 runner    (1001) docker     (127)     1401 2024-05-23 14:23:55.000000 apysc-4.4.2/apysc/_material_design/icon/material_shopping_basket_outlined_icon.py
--rw-r--r--   0 runner    (1001) docker     (127)     1372 2024-05-23 14:23:55.000000 apysc-4.4.2/apysc/_material_design/icon/material_shopping_cart_icon.py
--rw-r--r--   0 runner    (1001) docker     (127)     1379 2024-05-23 14:23:55.000000 apysc-4.4.2/apysc/_material_design/icon/material_shopping_cart_outlined_icon.py
--rw-r--r--   0 runner    (1001) docker     (127)     1207 2024-05-23 14:23:55.000000 apysc-4.4.2/apysc/_material_design/icon/material_shuffle_icon.py
--rw-r--r--   0 runner    (1001) docker     (127)     1313 2024-05-23 14:23:55.000000 apysc-4.4.2/apysc/_material_design/icon/material_shuffle_on_icon.py
--rw-r--r--   0 runner    (1001) docker     (127)     1235 2024-05-23 14:23:55.000000 apysc-4.4.2/apysc/_material_design/icon/material_shuffle_outlined_icon.py
--rw-r--r--   0 runner    (1001) docker     (127)     1074 2024-05-23 14:23:55.000000 apysc-4.4.2/apysc/_material_design/icon/material_skip_next_icon.py
--rw-r--r--   0 runner    (1001) docker     (127)     1130 2024-05-23 14:23:55.000000 apysc-4.4.2/apysc/_material_design/icon/material_skip_next_outlined_icon.py
--rw-r--r--   0 runner    (1001) docker     (127)     1078 2024-05-23 14:23:55.000000 apysc-4.4.2/apysc/_material_design/icon/material_skip_previous_icon.py
--rw-r--r--   0 runner    (1001) docker     (127)     1145 2024-05-23 14:23:55.000000 apysc-4.4.2/apysc/_material_design/icon/material_skip_previous_outlined_icon.py
--rw-r--r--   0 runner    (1001) docker     (127)     1596 2024-05-23 14:23:55.000000 apysc-4.4.2/apysc/_material_design/icon/material_slow_motion_video_icon.py
--rw-r--r--   0 runner    (1001) docker     (127)     1655 2024-05-23 14:23:55.000000 apysc-4.4.2/apysc/_material_design/icon/material_slow_motion_video_outlined_icon.py
--rw-r--r--   0 runner    (1001) docker     (127)     1515 2024-05-23 14:23:55.000000 apysc-4.4.2/apysc/_material_design/icon/material_smart_button_icon.py
--rw-r--r--   0 runner    (1001) docker     (127)     1541 2024-05-23 14:23:55.000000 apysc-4.4.2/apysc/_material_design/icon/material_smart_button_outlined_icon.py
--rw-r--r--   0 runner    (1001) docker     (127)     1294 2024-05-23 14:23:55.000000 apysc-4.4.2/apysc/_material_design/icon/material_snooze_icon.py
--rw-r--r--   0 runner    (1001) docker     (127)     1311 2024-05-23 14:23:55.000000 apysc-4.4.2/apysc/_material_design/icon/material_snooze_outlined_icon.py
--rw-r--r--   0 runner    (1001) docker     (127)     1323 2024-05-23 14:23:55.000000 apysc-4.4.2/apysc/_material_design/icon/material_sort_by_alpha_icon.py
--rw-r--r--   0 runner    (1001) docker     (127)     1332 2024-05-23 14:23:55.000000 apysc-4.4.2/apysc/_material_design/icon/material_sort_by_alpha_outlined_icon.py
--rw-r--r--   0 runner    (1001) docker     (127)     1213 2024-05-23 14:23:55.000000 apysc-4.4.2/apysc/_material_design/icon/material_source_icon.py
--rw-r--r--   0 runner    (1001) docker     (127)     1270 2024-05-23 14:23:55.000000 apysc-4.4.2/apysc/_material_design/icon/material_source_outlined_icon.py
--rw-r--r--   0 runner    (1001) docker     (127)     1208 2024-05-23 14:23:55.000000 apysc-4.4.2/apysc/_material_design/icon/material_speaker_notes_icon.py
--rw-r--r--   0 runner    (1001) docker     (127)     1302 2024-05-23 14:23:55.000000 apysc-4.4.2/apysc/_material_design/icon/material_speaker_notes_off_icon.py
--rw-r--r--   0 runner    (1001) docker     (127)     1326 2024-05-23 14:23:55.000000 apysc-4.4.2/apysc/_material_design/icon/material_speaker_notes_off_outlined_icon.py
--rw-r--r--   0 runner    (1001) docker     (127)     1256 2024-05-23 14:23:55.000000 apysc-4.4.2/apysc/_material_design/icon/material_speaker_notes_outlined_icon.py
--rw-r--r--   0 runner    (1001) docker     (127)     1442 2024-05-23 14:23:55.000000 apysc-4.4.2/apysc/_material_design/icon/material_speaker_phone_icon.py
--rw-r--r--   0 runner    (1001) docker     (127)     1453 2024-05-23 14:23:55.000000 apysc-4.4.2/apysc/_material_design/icon/material_speaker_phone_outlined_icon.py
--rw-r--r--   0 runner    (1001) docker     (127)     1254 2024-05-23 14:23:55.000000 apysc-4.4.2/apysc/_material_design/icon/material_speed_icon.py
--rw-r--r--   0 runner    (1001) docker     (127)     1293 2024-05-23 14:23:55.000000 apysc-4.4.2/apysc/_material_design/icon/material_speed_outlined_icon.py
--rw-r--r--   0 runner    (1001) docker     (127)     1201 2024-05-23 14:23:55.000000 apysc-4.4.2/apysc/_material_design/icon/material_spellcheck_icon.py
--rw-r--r--   0 runner    (1001) docker     (127)     1229 2024-05-23 14:23:55.000000 apysc-4.4.2/apysc/_material_design/icon/material_spellcheck_outlined_icon.py
--rw-r--r--   0 runner    (1001) docker     (127)     1180 2024-05-23 14:23:55.000000 apysc-4.4.2/apysc/_material_design/icon/material_star_rate_icon.py
--rw-r--r--   0 runner    (1001) docker     (127)     1298 2024-05-23 14:23:55.000000 apysc-4.4.2/apysc/_material_design/icon/material_star_rate_outlined_icon.py
--rw-r--r--   0 runner    (1001) docker     (127)     1209 2024-05-23 14:23:55.000000 apysc-4.4.2/apysc/_material_design/icon/material_stars_icon.py
--rw-r--r--   0 runner    (1001) docker     (127)     1590 2024-05-23 14:23:55.000000 apysc-4.4.2/apysc/_material_design/icon/material_stars_outlined_icon.py
--rw-r--r--   0 runner    (1001) docker     (127)     1178 2024-05-23 14:23:55.000000 apysc-4.4.2/apysc/_material_design/icon/material_stay_current_landscape_icon.py
--rw-r--r--   0 runner    (1001) docker     (127)     1206 2024-05-23 14:23:55.000000 apysc-4.4.2/apysc/_material_design/icon/material_stay_current_landscape_outlined_icon.py
--rw-r--r--   0 runner    (1001) docker     (127)     1187 2024-05-23 14:23:55.000000 apysc-4.4.2/apysc/_material_design/icon/material_stay_current_portrait_icon.py
--rw-r--r--   0 runner    (1001) docker     (127)     1215 2024-05-23 14:23:55.000000 apysc-4.4.2/apysc/_material_design/icon/material_stay_current_portrait_outlined_icon.py
--rw-r--r--   0 runner    (1001) docker     (127)     1178 2024-05-23 14:23:55.000000 apysc-4.4.2/apysc/_material_design/icon/material_stay_primary_landscape_icon.py
--rw-r--r--   0 runner    (1001) docker     (127)     1206 2024-05-23 14:23:55.000000 apysc-4.4.2/apysc/_material_design/icon/material_stay_primary_landscape_outlined_icon.py
--rw-r--r--   0 runner    (1001) docker     (127)     1187 2024-05-23 14:23:55.000000 apysc-4.4.2/apysc/_material_design/icon/material_stay_primary_portrait_icon.py
--rw-r--r--   0 runner    (1001) docker     (127)     1215 2024-05-23 14:23:55.000000 apysc-4.4.2/apysc/_material_design/icon/material_stay_primary_portrait_outlined_icon.py
--rw-r--r--   0 runner    (1001) docker     (127)     1231 2024-05-23 14:23:55.000000 apysc-4.4.2/apysc/_material_design/icon/material_sticky_note_2_icon.py
--rw-r--r--   0 runner    (1001) docker     (127)     1246 2024-05-23 14:23:55.000000 apysc-4.4.2/apysc/_material_design/icon/material_sticky_note_2_outlined_icon.py
--rw-r--r--   0 runner    (1001) docker     (127)     1206 2024-05-23 14:23:55.000000 apysc-4.4.2/apysc/_material_design/icon/material_stop_circle_icon.py
--rw-r--r--   0 runner    (1001) docker     (127)     1318 2024-05-23 14:23:55.000000 apysc-4.4.2/apysc/_material_design/icon/material_stop_circle_outlined_icon.py
--rw-r--r--   0 runner    (1001) docker     (127)     1038 2024-05-23 14:23:55.000000 apysc-4.4.2/apysc/_material_design/icon/material_stop_icon.py
--rw-r--r--   0 runner    (1001) docker     (127)     1081 2024-05-23 14:23:55.000000 apysc-4.4.2/apysc/_material_design/icon/material_stop_outlined_icon.py
--rw-r--r--   0 runner    (1001) docker     (127)     1401 2024-05-23 14:23:55.000000 apysc-4.4.2/apysc/_material_design/icon/material_stop_screen_share_icon.py
--rw-r--r--   0 runner    (1001) docker     (127)     1444 2024-05-23 14:23:55.000000 apysc-4.4.2/apysc/_material_design/icon/material_stop_screen_share_outlined_icon.py
--rw-r--r--   0 runner    (1001) docker     (127)     1102 2024-05-23 14:23:55.000000 apysc-4.4.2/apysc/_material_design/icon/material_store_icon.py
--rw-r--r--   0 runner    (1001) docker     (127)     1158 2024-05-23 14:23:55.000000 apysc-4.4.2/apysc/_material_design/icon/material_store_outlined_icon.py
--rw-r--r--   0 runner    (1001) docker     (127)     1095 2024-05-23 14:23:55.000000 apysc-4.4.2/apysc/_material_design/icon/material_subject_icon.py
--rw-r--r--   0 runner    (1001) docker     (127)     1123 2024-05-23 14:23:55.000000 apysc-4.4.2/apysc/_material_design/icon/material_subject_outlined_icon.py
--rw-r--r--   0 runner    (1001) docker     (127)     1183 2024-05-23 14:23:55.000000 apysc-4.4.2/apysc/_material_design/icon/material_subscriptions_icon.py
--rw-r--r--   0 runner    (1001) docker     (127)     1217 2024-05-23 14:23:55.000000 apysc-4.4.2/apysc/_material_design/icon/material_subscriptions_outlined_icon.py
--rw-r--r--   0 runner    (1001) docker     (127)     1178 2024-05-23 14:23:55.000000 apysc-4.4.2/apysc/_material_design/icon/material_subtitles_icon.py
--rw-r--r--   0 runner    (1001) docker     (127)     1362 2024-05-23 14:23:55.000000 apysc-4.4.2/apysc/_material_design/icon/material_subtitles_off_icon.py
--rw-r--r--   0 runner    (1001) docker     (127)     1444 2024-05-23 14:23:55.000000 apysc-4.4.2/apysc/_material_design/icon/material_subtitles_off_outlined_icon.py
--rw-r--r--   0 runner    (1001) docker     (127)     1209 2024-05-23 14:23:55.000000 apysc-4.4.2/apysc/_material_design/icon/material_subtitles_outlined_icon.py
--rw-r--r--   0 runner    (1001) docker     (127)     1609 2024-05-23 14:23:55.000000 apysc-4.4.2/apysc/_material_design/icon/material_supervised_user_circle_icon.py
--rw-r--r--   0 runner    (1001) docker     (127)     1661 2024-05-23 14:23:55.000000 apysc-4.4.2/apysc/_material_design/icon/material_supervised_user_circle_outlined_icon.py
--rw-r--r--   0 runner    (1001) docker     (127)     1381 2024-05-23 14:23:55.000000 apysc-4.4.2/apysc/_material_design/icon/material_supervisor_account_icon.py
--rw-r--r--   0 runner    (1001) docker     (127)     1585 2024-05-23 14:23:55.000000 apysc-4.4.2/apysc/_material_design/icon/material_supervisor_account_outlined_icon.py
--rw-r--r--   0 runner    (1001) docker     (127)     1624 2024-05-23 14:23:55.000000 apysc-4.4.2/apysc/_material_design/icon/material_support_icon.py
--rw-r--r--   0 runner    (1001) docker     (127)     1650 2024-05-23 14:23:55.000000 apysc-4.4.2/apysc/_material_design/icon/material_support_outlined_icon.py
--rw-r--r--   0 runner    (1001) docker     (127)     1489 2024-05-23 14:23:55.000000 apysc-4.4.2/apysc/_material_design/icon/material_surround_sound_icon.py
--rw-r--r--   0 runner    (1001) docker     (127)     1848 2024-05-23 14:23:55.000000 apysc-4.4.2/apysc/_material_design/icon/material_surround_sound_outlined_icon.py
--rw-r--r--   0 runner    (1001) docker     (127)     1192 2024-05-23 14:23:55.000000 apysc-4.4.2/apysc/_material_design/icon/material_swap_calls_icon.py
--rw-r--r--   0 runner    (1001) docker     (127)     1220 2024-05-23 14:23:55.000000 apysc-4.4.2/apysc/_material_design/icon/material_swap_calls_outlined_icon.py
--rw-r--r--   0 runner    (1001) docker     (127)     1113 2024-05-23 14:23:55.000000 apysc-4.4.2/apysc/_material_design/icon/material_swap_horiz_icon.py
--rw-r--r--   0 runner    (1001) docker     (127)     1141 2024-05-23 14:23:55.000000 apysc-4.4.2/apysc/_material_design/icon/material_swap_horiz_outlined_icon.py
--rw-r--r--   0 runner    (1001) docker     (127)     1219 2024-05-23 14:23:55.000000 apysc-4.4.2/apysc/_material_design/icon/material_swap_horizontal_circle_icon.py
--rw-r--r--   0 runner    (1001) docker     (127)     1288 2024-05-23 14:23:55.000000 apysc-4.4.2/apysc/_material_design/icon/material_swap_horizontal_circle_outlined_icon.py
--rw-r--r--   0 runner    (1001) docker     (127)     1109 2024-05-23 14:23:55.000000 apysc-4.4.2/apysc/_material_design/icon/material_swap_vert_icon.py
--rw-r--r--   0 runner    (1001) docker     (127)     1206 2024-05-23 14:23:55.000000 apysc-4.4.2/apysc/_material_design/icon/material_swap_vert_outlined_icon.py
--rw-r--r--   0 runner    (1001) docker     (127)     1207 2024-05-23 14:23:55.000000 apysc-4.4.2/apysc/_material_design/icon/material_swap_vertical_circle_icon.py
--rw-r--r--   0 runner    (1001) docker     (127)     1285 2024-05-23 14:23:55.000000 apysc-4.4.2/apysc/_material_design/icon/material_swap_vertical_circle_outlined_icon.py
--rw-r--r--   0 runner    (1001) docker     (127)     1426 2024-05-23 14:23:55.000000 apysc-4.4.2/apysc/_material_design/icon/material_swipe_icon.py
--rw-r--r--   0 runner    (1001) docker     (127)     1168 2024-05-23 14:23:55.000000 apysc-4.4.2/apysc/_material_design/icon/material_sync_alt_icon.py
--rw-r--r--   0 runner    (1001) docker     (127)     1194 2024-05-23 14:23:55.000000 apysc-4.4.2/apysc/_material_design/icon/material_sync_alt_outlined_icon.py
--rw-r--r--   0 runner    (1001) docker     (127)     1200 2024-05-23 14:23:55.000000 apysc-4.4.2/apysc/_material_design/icon/material_system_update_alt_icon.py
--rw-r--r--   0 runner    (1001) docker     (127)     1365 2024-05-23 14:23:55.000000 apysc-4.4.2/apysc/_material_design/icon/material_system_update_alt_outlined_icon.py
--rw-r--r--   0 runner    (1001) docker     (127)     1118 2024-05-23 14:23:55.000000 apysc-4.4.2/apysc/_material_design/icon/material_tab_icon.py
--rw-r--r--   0 runner    (1001) docker     (127)     1161 2024-05-23 14:23:55.000000 apysc-4.4.2/apysc/_material_design/icon/material_tab_outlined_icon.py
--rw-r--r--   0 runner    (1001) docker     (127)     1321 2024-05-23 14:23:55.000000 apysc-4.4.2/apysc/_material_design/icon/material_tab_unselected_icon.py
--rw-r--r--   0 runner    (1001) docker     (127)     1349 2024-05-23 14:23:55.000000 apysc-4.4.2/apysc/_material_design/icon/material_tab_unselected_outlined_icon.py
--rw-r--r--   0 runner    (1001) docker     (127)     1375 2024-05-23 14:23:55.000000 apysc-4.4.2/apysc/_material_design/icon/material_table_view_icon.py
--rw-r--r--   0 runner    (1001) docker     (127)     1401 2024-05-23 14:23:55.000000 apysc-4.4.2/apysc/_material_design/icon/material_table_view_outlined_icon.py
--rw-r--r--   0 runner    (1001) docker     (127)     1172 2024-05-23 14:23:55.000000 apysc-4.4.2/apysc/_material_design/icon/material_text_rotate_up_icon.py
--rw-r--r--   0 runner    (1001) docker     (127)     1227 2024-05-23 14:23:55.000000 apysc-4.4.2/apysc/_material_design/icon/material_text_rotate_up_outlined_icon.py
--rw-r--r--   0 runner    (1001) docker     (127)     1189 2024-05-23 14:23:55.000000 apysc-4.4.2/apysc/_material_design/icon/material_text_rotate_vertical_icon.py
--rw-r--r--   0 runner    (1001) docker     (127)     1239 2024-05-23 14:23:55.000000 apysc-4.4.2/apysc/_material_design/icon/material_text_rotate_vertical_outlined_icon.py
--rw-r--r--   0 runner    (1001) docker     (127)     1281 2024-05-23 14:23:55.000000 apysc-4.4.2/apysc/_material_design/icon/material_text_rotation_angledown_icon.py
--rw-r--r--   0 runner    (1001) docker     (127)     1335 2024-05-23 14:23:55.000000 apysc-4.4.2/apysc/_material_design/icon/material_text_rotation_angledown_outlined_icon.py
--rw-r--r--   0 runner    (1001) docker     (127)     1274 2024-05-23 14:23:55.000000 apysc-4.4.2/apysc/_material_design/icon/material_text_rotation_angleup_icon.py
--rw-r--r--   0 runner    (1001) docker     (127)     1327 2024-05-23 14:23:55.000000 apysc-4.4.2/apysc/_material_design/icon/material_text_rotation_angleup_outlined_icon.py
--rw-r--r--   0 runner    (1001) docker     (127)     1180 2024-05-23 14:23:55.000000 apysc-4.4.2/apysc/_material_design/icon/material_text_rotation_down_icon.py
--rw-r--r--   0 runner    (1001) docker     (127)     1234 2024-05-23 14:23:55.000000 apysc-4.4.2/apysc/_material_design/icon/material_text_rotation_down_outlined_icon.py
--rw-r--r--   0 runner    (1001) docker     (127)     1181 2024-05-23 14:23:55.000000 apysc-4.4.2/apysc/_material_design/icon/material_text_rotation_none_icon.py
--rw-r--r--   0 runner    (1001) docker     (127)     1206 2024-05-23 14:23:55.000000 apysc-4.4.2/apysc/_material_design/icon/material_text_rotation_none_outlined_icon.py
--rw-r--r--   0 runner    (1001) docker     (127)     1149 2024-05-23 14:23:55.000000 apysc-4.4.2/apysc/_material_design/icon/material_textsms_icon.py
--rw-r--r--   0 runner    (1001) docker     (127)     1184 2024-05-23 14:23:55.000000 apysc-4.4.2/apysc/_material_design/icon/material_textsms_outlined_icon.py
--rw-r--r--   0 runner    (1001) docker     (127)     1175 2024-05-23 14:23:55.000000 apysc-4.4.2/apysc/_material_design/icon/material_theaters_icon.py
--rw-r--r--   0 runner    (1001) docker     (127)     1218 2024-05-23 14:23:55.000000 apysc-4.4.2/apysc/_material_design/icon/material_theaters_outlined_icon.py
--rw-r--r--   0 runner    (1001) docker     (127)     1238 2024-05-23 14:23:55.000000 apysc-4.4.2/apysc/_material_design/icon/material_thumb_down_icon.py
--rw-r--r--   0 runner    (1001) docker     (127)     1447 2024-05-23 14:23:55.000000 apysc-4.4.2/apysc/_material_design/icon/material_thumb_down_off_alt_icon.py
--rw-r--r--   0 runner    (1001) docker     (127)     1317 2024-05-23 14:23:55.000000 apysc-4.4.2/apysc/_material_design/icon/material_thumb_down_outlined_icon.py
--rw-r--r--   0 runner    (1001) docker     (127)     1237 2024-05-23 14:23:55.000000 apysc-4.4.2/apysc/_material_design/icon/material_thumb_up_icon.py
--rw-r--r--   0 runner    (1001) docker     (127)     1442 2024-05-23 14:23:55.000000 apysc-4.4.2/apysc/_material_design/icon/material_thumb_up_off_alt_icon.py
--rw-r--r--   0 runner    (1001) docker     (127)     1308 2024-05-23 14:23:55.000000 apysc-4.4.2/apysc/_material_design/icon/material_thumb_up_outlined_icon.py
--rw-r--r--   0 runner    (1001) docker     (127)     1435 2024-05-23 14:23:55.000000 apysc-4.4.2/apysc/_material_design/icon/material_thumbs_up_down_icon.py
--rw-r--r--   0 runner    (1001) docker     (127)     1581 2024-05-23 14:23:55.000000 apysc-4.4.2/apysc/_material_design/icon/material_thumbs_up_down_outlined_icon.py
--rw-r--r--   0 runner    (1001) docker     (127)     1611 2024-05-23 14:23:55.000000 apysc-4.4.2/apysc/_material_design/icon/material_timeline_icon.py
--rw-r--r--   0 runner    (1001) docker     (127)     1650 2024-05-23 14:23:55.000000 apysc-4.4.2/apysc/_material_design/icon/material_timeline_outlined_icon.py
--rw-r--r--   0 runner    (1001) docker     (127)     1112 2024-05-23 14:23:55.000000 apysc-4.4.2/apysc/_material_design/icon/material_toc_icon.py
--rw-r--r--   0 runner    (1001) docker     (127)     1155 2024-05-23 14:23:55.000000 apysc-4.4.2/apysc/_material_design/icon/material_toc_outlined_icon.py
--rw-r--r--   0 runner    (1001) docker     (127)     1159 2024-05-23 14:23:55.000000 apysc-4.4.2/apysc/_material_design/icon/material_today_icon.py
--rw-r--r--   0 runner    (1001) docker     (127)     1195 2024-05-23 14:23:55.000000 apysc-4.4.2/apysc/_material_design/icon/material_today_outlined_icon.py
--rw-r--r--   0 runner    (1001) docker     (127)     1259 2024-05-23 14:23:55.000000 apysc-4.4.2/apysc/_material_design/icon/material_toll_icon.py
--rw-r--r--   0 runner    (1001) docker     (127)     1273 2024-05-23 14:23:55.000000 apysc-4.4.2/apysc/_material_design/icon/material_toll_outlined_icon.py
--rw-r--r--   0 runner    (1001) docker     (127)     1577 2024-05-23 14:23:55.000000 apysc-4.4.2/apysc/_material_design/icon/material_touch_app_icon.py
--rw-r--r--   0 runner    (1001) docker     (127)     1777 2024-05-23 14:23:55.000000 apysc-4.4.2/apysc/_material_design/icon/material_touch_app_outlined_icon.py
--rw-r--r--   0 runner    (1001) docker     (127)     1106 2024-05-23 14:23:55.000000 apysc-4.4.2/apysc/_material_design/icon/material_tour_icon.py
--rw-r--r--   0 runner    (1001) docker     (127)     1269 2024-05-23 14:23:55.000000 apysc-4.4.2/apysc/_material_design/icon/material_tour_outlined_icon.py
--rw-r--r--   0 runner    (1001) docker     (127)     1473 2024-05-23 14:23:55.000000 apysc-4.4.2/apysc/_material_design/icon/material_track_changes_icon.py
--rw-r--r--   0 runner    (1001) docker     (127)     1499 2024-05-23 14:23:55.000000 apysc-4.4.2/apysc/_material_design/icon/material_track_changes_outlined_icon.py
--rw-r--r--   0 runner    (1001) docker     (127)     1336 2024-05-23 14:23:55.000000 apysc-4.4.2/apysc/_material_design/icon/material_translate_icon.py
--rw-r--r--   0 runner    (1001) docker     (127)     1364 2024-05-23 14:23:55.000000 apysc-4.4.2/apysc/_material_design/icon/material_translate_outlined_icon.py
--rw-r--r--   0 runner    (1001) docker     (127)     1121 2024-05-23 14:23:55.000000 apysc-4.4.2/apysc/_material_design/icon/material_trending_down_icon.py
--rw-r--r--   0 runner    (1001) docker     (127)     1152 2024-05-23 14:23:55.000000 apysc-4.4.2/apysc/_material_design/icon/material_trending_down_outlined_icon.py
--rw-r--r--   0 runner    (1001) docker     (127)     1074 2024-05-23 14:23:55.000000 apysc-4.4.2/apysc/_material_design/icon/material_trending_flat_icon.py
--rw-r--r--   0 runner    (1001) docker     (127)     1106 2024-05-23 14:23:55.000000 apysc-4.4.2/apysc/_material_design/icon/material_trending_flat_outlined_icon.py
--rw-r--r--   0 runner    (1001) docker     (127)     1116 2024-05-23 14:23:55.000000 apysc-4.4.2/apysc/_material_design/icon/material_trending_up_icon.py
--rw-r--r--   0 runner    (1001) docker     (127)     1147 2024-05-23 14:23:55.000000 apysc-4.4.2/apysc/_material_design/icon/material_trending_up_outlined_icon.py
--rw-r--r--   0 runner    (1001) docker     (127)     1098 2024-05-23 14:23:55.000000 apysc-4.4.2/apysc/_material_design/icon/material_turned_in_icon.py
--rw-r--r--   0 runner    (1001) docker     (127)     1136 2024-05-23 14:23:55.000000 apysc-4.4.2/apysc/_material_design/icon/material_turned_in_not_icon.py
--rw-r--r--   0 runner    (1001) docker     (127)     1164 2024-05-23 14:23:55.000000 apysc-4.4.2/apysc/_material_design/icon/material_turned_in_not_outlined_icon.py
--rw-r--r--   0 runner    (1001) docker     (127)     1126 2024-05-23 14:23:55.000000 apysc-4.4.2/apysc/_material_design/icon/material_turned_in_outlined_icon.py
--rw-r--r--   0 runner    (1001) docker     (127)     1434 2024-05-23 14:23:55.000000 apysc-4.4.2/apysc/_material_design/icon/material_unpublished_icon.py
--rw-r--r--   0 runner    (1001) docker     (127)     1651 2024-05-23 14:23:55.000000 apysc-4.4.2/apysc/_material_design/icon/material_unpublished_outlined_icon.py
--rw-r--r--   0 runner    (1001) docker     (127)     1273 2024-05-23 14:23:55.000000 apysc-4.4.2/apysc/_material_design/icon/material_unsubscribe_icon.py
--rw-r--r--   0 runner    (1001) docker     (127)     1347 2024-05-23 14:23:55.000000 apysc-4.4.2/apysc/_material_design/icon/material_unsubscribe_outlined_icon.py
--rw-r--r--   0 runner    (1001) docker     (127)     1399 2024-05-23 14:23:55.000000 apysc-4.4.2/apysc/_material_design/icon/material_update_icon.py
--rw-r--r--   0 runner    (1001) docker     (127)     1328 2024-05-23 14:23:55.000000 apysc-4.4.2/apysc/_material_design/icon/material_update_outlined_icon.py
--rw-r--r--   0 runner    (1001) docker     (127)     1134 2024-05-23 14:23:55.000000 apysc-4.4.2/apysc/_material_design/icon/material_upgrade_icon.py
--rw-r--r--   0 runner    (1001) docker     (127)     1160 2024-05-23 14:23:55.000000 apysc-4.4.2/apysc/_material_design/icon/material_upgrade_outlined_icon.py
--rw-r--r--   0 runner    (1001) docker     (127)     1358 2024-05-23 14:23:55.000000 apysc-4.4.2/apysc/_material_design/icon/material_verified_icon.py
--rw-r--r--   0 runner    (1001) docker     (127)     1839 2024-05-23 14:23:55.000000 apysc-4.4.2/apysc/_material_design/icon/material_verified_outlined_icon.py
--rw-r--r--   0 runner    (1001) docker     (127)     1166 2024-05-23 14:23:55.000000 apysc-4.4.2/apysc/_material_design/icon/material_verified_user_icon.py
--rw-r--r--   0 runner    (1001) docker     (127)     1261 2024-05-23 14:23:55.000000 apysc-4.4.2/apysc/_material_design/icon/material_verified_user_outlined_icon.py
--rw-r--r--   0 runner    (1001) docker     (127)     1127 2024-05-23 14:23:55.000000 apysc-4.4.2/apysc/_material_design/icon/material_vertical_split_icon.py
--rw-r--r--   0 runner    (1001) docker     (127)     1157 2024-05-23 14:23:55.000000 apysc-4.4.2/apysc/_material_design/icon/material_vertical_split_outlined_icon.py
--rw-r--r--   0 runner    (1001) docker     (127)     1179 2024-05-23 14:23:55.000000 apysc-4.4.2/apysc/_material_design/icon/material_video_call_icon.py
--rw-r--r--   0 runner    (1001) docker     (127)     1218 2024-05-23 14:23:55.000000 apysc-4.4.2/apysc/_material_design/icon/material_video_call_outlined_icon.py
--rw-r--r--   0 runner    (1001) docker     (127)     1139 2024-05-23 14:23:55.000000 apysc-4.4.2/apysc/_material_design/icon/material_video_label_icon.py
--rw-r--r--   0 runner    (1001) docker     (127)     1165 2024-05-23 14:23:55.000000 apysc-4.4.2/apysc/_material_design/icon/material_video_label_outlined_icon.py
--rw-r--r--   0 runner    (1001) docker     (127)     1185 2024-05-23 14:23:55.000000 apysc-4.4.2/apysc/_material_design/icon/material_video_library_icon.py
--rw-r--r--   0 runner    (1001) docker     (127)     1221 2024-05-23 14:23:55.000000 apysc-4.4.2/apysc/_material_design/icon/material_video_library_outlined_icon.py
--rw-r--r--   0 runner    (1001) docker     (127)     2049 2024-05-23 14:23:55.000000 apysc-4.4.2/apysc/_material_design/icon/material_video_settings_icon.py
--rw-r--r--   0 runner    (1001) docker     (127)     2075 2024-05-23 14:23:55.000000 apysc-4.4.2/apysc/_material_design/icon/material_video_settings_outlined_icon.py
--rw-r--r--   0 runner    (1001) docker     (127)     1138 2024-05-23 14:23:55.000000 apysc-4.4.2/apysc/_material_design/icon/material_videocam_icon.py
--rw-r--r--   0 runner    (1001) docker     (127)     1218 2024-05-23 14:23:55.000000 apysc-4.4.2/apysc/_material_design/icon/material_videocam_off_icon.py
--rw-r--r--   0 runner    (1001) docker     (127)     1284 2024-05-23 14:23:55.000000 apysc-4.4.2/apysc/_material_design/icon/material_videocam_off_outlined_icon.py
--rw-r--r--   0 runner    (1001) docker     (127)     1176 2024-05-23 14:23:55.000000 apysc-4.4.2/apysc/_material_design/icon/material_videocam_outlined_icon.py
--rw-r--r--   0 runner    (1001) docker     (127)     1205 2024-05-23 14:23:55.000000 apysc-4.4.2/apysc/_material_design/icon/material_view_agenda_icon.py
--rw-r--r--   0 runner    (1001) docker     (127)     1261 2024-05-23 14:23:55.000000 apysc-4.4.2/apysc/_material_design/icon/material_view_agenda_outlined_icon.py
--rw-r--r--   0 runner    (1001) docker     (127)     1088 2024-05-23 14:23:55.000000 apysc-4.4.2/apysc/_material_design/icon/material_view_array_icon.py
--rw-r--r--   0 runner    (1001) docker     (127)     1128 2024-05-23 14:23:55.000000 apysc-4.4.2/apysc/_material_design/icon/material_view_array_outlined_icon.py
--rw-r--r--   0 runner    (1001) docker     (127)     1098 2024-05-23 14:23:55.000000 apysc-4.4.2/apysc/_material_design/icon/material_view_carousel_icon.py
--rw-r--r--   0 runner    (1001) docker     (127)     1134 2024-05-23 14:23:55.000000 apysc-4.4.2/apysc/_material_design/icon/material_view_carousel_outlined_icon.py
--rw-r--r--   0 runner    (1001) docker     (127)     1093 2024-05-23 14:23:55.000000 apysc-4.4.2/apysc/_material_design/icon/material_view_column_icon.py
--rw-r--r--   0 runner    (1001) docker     (127)     1131 2024-05-23 14:23:55.000000 apysc-4.4.2/apysc/_material_design/icon/material_view_column_outlined_icon.py
--rw-r--r--   0 runner    (1001) docker     (127)     1145 2024-05-23 14:23:55.000000 apysc-4.4.2/apysc/_material_design/icon/material_view_day_icon.py
--rw-r--r--   0 runner    (1001) docker     (127)     1188 2024-05-23 14:23:55.000000 apysc-4.4.2/apysc/_material_design/icon/material_view_day_outlined_icon.py
--rw-r--r--   0 runner    (1001) docker     (127)     1112 2024-05-23 14:23:55.000000 apysc-4.4.2/apysc/_material_design/icon/material_view_headline_icon.py
--rw-r--r--   0 runner    (1001) docker     (127)     1138 2024-05-23 14:23:55.000000 apysc-4.4.2/apysc/_material_design/icon/material_view_headline_outlined_icon.py
--rw-r--r--   0 runner    (1001) docker     (127)     1508 2024-05-23 14:23:55.000000 apysc-4.4.2/apysc/_material_design/icon/material_view_in_ar_icon.py
--rw-r--r--   0 runner    (1001) docker     (127)     1125 2024-05-23 14:23:55.000000 apysc-4.4.2/apysc/_material_design/icon/material_view_list_icon.py
--rw-r--r--   0 runner    (1001) docker     (127)     1180 2024-05-23 14:23:55.000000 apysc-4.4.2/apysc/_material_design/icon/material_view_list_outlined_icon.py
--rw-r--r--   0 runner    (1001) docker     (127)     1132 2024-05-23 14:23:55.000000 apysc-4.4.2/apysc/_material_design/icon/material_view_module_icon.py
--rw-r--r--   0 runner    (1001) docker     (127)     1192 2024-05-23 14:23:55.000000 apysc-4.4.2/apysc/_material_design/icon/material_view_module_outlined_icon.py
--rw-r--r--   0 runner    (1001) docker     (127)     1106 2024-05-23 14:23:55.000000 apysc-4.4.2/apysc/_material_design/icon/material_view_quilt_icon.py
--rw-r--r--   0 runner    (1001) docker     (127)     1154 2024-05-23 14:23:55.000000 apysc-4.4.2/apysc/_material_design/icon/material_view_quilt_outlined_icon.py
--rw-r--r--   0 runner    (1001) docker     (127)     1165 2024-05-23 14:23:55.000000 apysc-4.4.2/apysc/_material_design/icon/material_view_sidebar_icon.py
--rw-r--r--   0 runner    (1001) docker     (127)     1244 2024-05-23 14:23:55.000000 apysc-4.4.2/apysc/_material_design/icon/material_view_sidebar_outlined_icon.py
--rw-r--r--   0 runner    (1001) docker     (127)     1075 2024-05-23 14:23:55.000000 apysc-4.4.2/apysc/_material_design/icon/material_view_stream_icon.py
--rw-r--r--   0 runner    (1001) docker     (127)     1120 2024-05-23 14:23:55.000000 apysc-4.4.2/apysc/_material_design/icon/material_view_stream_outlined_icon.py
--rw-r--r--   0 runner    (1001) docker     (127)     1277 2024-05-23 14:23:55.000000 apysc-4.4.2/apysc/_material_design/icon/material_view_week_icon.py
--rw-r--r--   0 runner    (1001) docker     (127)     1192 2024-05-23 14:23:55.000000 apysc-4.4.2/apysc/_material_design/icon/material_view_week_outlined_icon.py
--rw-r--r--   0 runner    (1001) docker     (127)     1252 2024-05-23 14:23:55.000000 apysc-4.4.2/apysc/_material_design/icon/material_visibility_icon.py
--rw-r--r--   0 runner    (1001) docker     (127)     1598 2024-05-23 14:23:55.000000 apysc-4.4.2/apysc/_material_design/icon/material_visibility_off_icon.py
--rw-r--r--   0 runner    (1001) docker     (127)     1824 2024-05-23 14:23:55.000000 apysc-4.4.2/apysc/_material_design/icon/material_visibility_off_outlined_icon.py
--rw-r--r--   0 runner    (1001) docker     (127)     1405 2024-05-23 14:23:55.000000 apysc-4.4.2/apysc/_material_design/icon/material_visibility_outlined_icon.py
--rw-r--r--   0 runner    (1001) docker     (127)     1485 2024-05-23 14:23:55.000000 apysc-4.4.2/apysc/_material_design/icon/material_voice_over_off_icon.py
--rw-r--r--   0 runner    (1001) docker     (127)     1620 2024-05-23 14:23:55.000000 apysc-4.4.2/apysc/_material_design/icon/material_voice_over_off_outlined_icon.py
--rw-r--r--   0 runner    (1001) docker     (127)     1371 2024-05-23 14:23:55.000000 apysc-4.4.2/apysc/_material_design/icon/material_voicemail_icon.py
--rw-r--r--   0 runner    (1001) docker     (127)     1399 2024-05-23 14:23:55.000000 apysc-4.4.2/apysc/_material_design/icon/material_voicemail_outlined_icon.py
--rw-r--r--   0 runner    (1001) docker     (127)     1133 2024-05-23 14:23:55.000000 apysc-4.4.2/apysc/_material_design/icon/material_volume_down_icon.py
--rw-r--r--   0 runner    (1001) docker     (127)     1199 2024-05-23 14:23:55.000000 apysc-4.4.2/apysc/_material_design/icon/material_volume_down_outlined_icon.py
--rw-r--r--   0 runner    (1001) docker     (127)     1067 2024-05-23 14:23:55.000000 apysc-4.4.2/apysc/_material_design/icon/material_volume_mute_icon.py
--rw-r--r--   0 runner    (1001) docker     (127)     1136 2024-05-23 14:23:55.000000 apysc-4.4.2/apysc/_material_design/icon/material_volume_mute_outlined_icon.py
--rw-r--r--   0 runner    (1001) docker     (127)     1393 2024-05-23 14:23:55.000000 apysc-4.4.2/apysc/_material_design/icon/material_volume_off_icon.py
--rw-r--r--   0 runner    (1001) docker     (127)     1480 2024-05-23 14:23:55.000000 apysc-4.4.2/apysc/_material_design/icon/material_volume_off_outlined_icon.py
--rw-r--r--   0 runner    (1001) docker     (127)     1226 2024-05-23 14:23:55.000000 apysc-4.4.2/apysc/_material_design/icon/material_volume_up_icon.py
--rw-r--r--   0 runner    (1001) docker     (127)     1299 2024-05-23 14:23:55.000000 apysc-4.4.2/apysc/_material_design/icon/material_volume_up_outlined_icon.py
--rw-r--r--   0 runner    (1001) docker     (127)     1189 2024-05-23 14:23:55.000000 apysc-4.4.2/apysc/_material_design/icon/material_vpn_key_icon.py
--rw-r--r--   0 runner    (1001) docker     (127)     1400 2024-05-23 14:23:55.000000 apysc-4.4.2/apysc/_material_design/icon/material_vpn_key_outlined_icon.py
--rw-r--r--   0 runner    (1001) docker     (127)     1120 2024-05-23 14:23:55.000000 apysc-4.4.2/apysc/_material_design/icon/material_warning_amber_outlined_icon.py
--rw-r--r--   0 runner    (1001) docker     (127)     1084 2024-05-23 14:23:55.000000 apysc-4.4.2/apysc/_material_design/icon/material_warning_icon.py
--rw-r--r--   0 runner    (1001) docker     (127)     1073 2024-05-23 14:23:55.000000 apysc-4.4.2/apysc/_material_design/icon/material_warning_outlined_icon.py
--rw-r--r--   0 runner    (1001) docker     (127)     1219 2024-05-23 14:23:55.000000 apysc-4.4.2/apysc/_material_design/icon/material_watch_later_icon.py
--rw-r--r--   0 runner    (1001) docker     (127)     1304 2024-05-23 14:23:55.000000 apysc-4.4.2/apysc/_material_design/icon/material_watch_later_outlined_icon.py
--rw-r--r--   0 runner    (1001) docker     (127)     1134 2024-05-23 14:23:55.000000 apysc-4.4.2/apysc/_material_design/icon/material_web_asset_icon.py
--rw-r--r--   0 runner    (1001) docker     (127)     1162 2024-05-23 14:23:55.000000 apysc-4.4.2/apysc/_material_design/icon/material_web_asset_outlined_icon.py
--rw-r--r--   0 runner    (1001) docker     (127)     1150 2024-05-23 14:23:55.000000 apysc-4.4.2/apysc/_material_design/icon/material_web_icon.py
--rw-r--r--   0 runner    (1001) docker     (127)     1350 2024-05-23 14:23:55.000000 apysc-4.4.2/apysc/_material_design/icon/material_web_outlined_icon.py
--rw-r--r--   0 runner    (1001) docker     (127)     1482 2024-05-23 14:23:55.000000 apysc-4.4.2/apysc/_material_design/icon/material_wifi_calling_icon.py
--rw-r--r--   0 runner    (1001) docker     (127)     1714 2024-05-23 14:23:55.000000 apysc-4.4.2/apysc/_material_design/icon/material_wifi_calling_outlined_icon.py
--rw-r--r--   0 runner    (1001) docker     (127)     1451 2024-05-23 14:23:55.000000 apysc-4.4.2/apysc/_material_design/icon/material_wifi_protected_setup_icon.py
--rw-r--r--   0 runner    (1001) docker     (127)     1477 2024-05-23 14:23:55.000000 apysc-4.4.2/apysc/_material_design/icon/material_wifi_protected_setup_outlined_icon.py
--rw-r--r--   0 runner    (1001) docker     (127)     1176 2024-05-23 14:23:55.000000 apysc-4.4.2/apysc/_material_design/icon/material_work_icon.py
--rw-r--r--   0 runner    (1001) docker     (127)     1301 2024-05-23 14:23:55.000000 apysc-4.4.2/apysc/_material_design/icon/material_work_off_icon.py
--rw-r--r--   0 runner    (1001) docker     (127)     1293 2024-05-23 14:23:55.000000 apysc-4.4.2/apysc/_material_design/icon/material_work_off_outlined_icon.py
--rw-r--r--   0 runner    (1001) docker     (127)     1230 2024-05-23 14:23:55.000000 apysc-4.4.2/apysc/_material_design/icon/material_work_outline_icon.py
--rw-r--r--   0 runner    (1001) docker     (127)     1238 2024-05-23 14:23:55.000000 apysc-4.4.2/apysc/_material_design/icon/material_work_outline_outlined_icon.py
--rw-r--r--   0 runner    (1001) docker     (127)     1204 2024-05-23 14:23:55.000000 apysc-4.4.2/apysc/_material_design/icon/material_work_outlined_icon.py
--rw-r--r--   0 runner    (1001) docker     (127)     1222 2024-05-23 14:23:55.000000 apysc-4.4.2/apysc/_material_design/icon/material_wysiwyg_icon.py
--rw-r--r--   0 runner    (1001) docker     (127)     1248 2024-05-23 14:23:55.000000 apysc-4.4.2/apysc/_material_design/icon/material_wysiwyg_outlined_icon.py
--rw-r--r--   0 runner    (1001) docker     (127)     1378 2024-05-23 14:23:55.000000 apysc-4.4.2/apysc/_material_design/icon/material_youtube_searched_for_icon.py
--rw-r--r--   0 runner    (1001) docker     (127)     1404 2024-05-23 14:23:55.000000 apysc-4.4.2/apysc/_material_design/icon/material_youtube_searched_for_outlined_icon.py
--rw-r--r--   0 runner    (1001) docker     (127)     1314 2024-05-23 14:23:55.000000 apysc-4.4.2/apysc/_material_design/icon/material_zoom_in_icon.py
--rw-r--r--   0 runner    (1001) docker     (127)     1325 2024-05-23 14:23:55.000000 apysc-4.4.2/apysc/_material_design/icon/material_zoom_in_outlined_icon.py
--rw-r--r--   0 runner    (1001) docker     (127)     1283 2024-05-23 14:23:55.000000 apysc-4.4.2/apysc/_material_design/icon/material_zoom_out_icon.py
--rw-r--r--   0 runner    (1001) docker     (127)     1309 2024-05-23 14:23:55.000000 apysc-4.4.2/apysc/_material_design/icon/material_zoom_out_outlined_icon.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-23 14:24:13.466301 apysc-4.4.2/apysc/_math/
--rw-r--r--   0 runner    (1001) docker     (127)        0 2024-05-23 14:23:55.000000 apysc-4.4.2/apysc/_math/__init__.py
--rw-r--r--   0 runner    (1001) docker     (127)      315 2024-05-23 14:23:55.000000 apysc-4.4.2/apysc/_math/math.py
--rw-r--r--   0 runner    (1001) docker     (127)     3458 2024-05-23 14:23:55.000000 apysc-4.4.2/apysc/_math/max_mixin.py
--rw-r--r--   0 runner    (1001) docker     (127)     3471 2024-05-23 14:23:55.000000 apysc-4.4.2/apysc/_math/min_mixin.py
--rw-r--r--   0 runner    (1001) docker     (127)     2510 2024-05-23 14:23:55.000000 apysc-4.4.2/apysc/_math/trunc_mixin.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-23 14:24:13.466301 apysc-4.4.2/apysc/_string/
--rw-r--r--   0 runner    (1001) docker     (127)        0 2024-05-23 14:23:55.000000 apysc-4.4.2/apysc/_string/__init__.py
--rw-r--r--   0 runner    (1001) docker     (127)     1596 2024-05-23 14:23:55.000000 apysc-4.4.2/apysc/_string/indent_util.py
--rw-r--r--   0 runner    (1001) docker     (127)     3453 2024-05-23 14:23:55.000000 apysc-4.4.2/apysc/_string/string_util.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-23 14:24:13.466301 apysc-4.4.2/apysc/_testing/
--rw-r--r--   0 runner    (1001) docker     (127)        0 2024-05-23 14:23:55.000000 apysc-4.4.2/apysc/_testing/__init__.py
--rw-r--r--   0 runner    (1001) docker     (127)     9001 2024-05-23 14:23:55.000000 apysc-4.4.2/apysc/_testing/e2e_testing_helper.py
--rw-r--r--   0 runner    (1001) docker     (127)     6350 2024-05-23 14:23:55.000000 apysc-4.4.2/apysc/_testing/testing_helper.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-23 14:24:13.470301 apysc-4.4.2/apysc/_time/
--rw-r--r--   0 runner    (1001) docker     (127)        0 2024-05-23 14:23:55.000000 apysc-4.4.2/apysc/_time/__init__.py
--rw-r--r--   0 runner    (1001) docker     (127)    10971 2024-05-23 14:23:55.000000 apysc-4.4.2/apysc/_time/datetime_.py
--rw-r--r--   0 runner    (1001) docker     (127)     5188 2024-05-23 14:23:55.000000 apysc-4.4.2/apysc/_time/day_mixin.py
--rw-r--r--   0 runner    (1001) docker     (127)     3556 2024-05-23 14:23:55.000000 apysc-4.4.2/apysc/_time/days_mixin.py
--rw-r--r--   0 runner    (1001) docker     (127)     2181 2024-05-23 14:23:55.000000 apysc-4.4.2/apysc/_time/fps.py
--rw-r--r--   0 runner    (1001) docker     (127)     5426 2024-05-23 14:23:55.000000 apysc-4.4.2/apysc/_time/hour_mixin.py
--rw-r--r--   0 runner    (1001) docker     (127)     2097 2024-05-23 14:23:55.000000 apysc-4.4.2/apysc/_time/left_and_right_datetimes_mixin.py
--rw-r--r--   0 runner    (1001) docker     (127)     5976 2024-05-23 14:23:55.000000 apysc-4.4.2/apysc/_time/millisecond_mixin.py
--rw-r--r--   0 runner    (1001) docker     (127)     5639 2024-05-23 14:23:55.000000 apysc-4.4.2/apysc/_time/minute_mixin.py
--rw-r--r--   0 runner    (1001) docker     (127)     1541 2024-05-23 14:23:55.000000 apysc-4.4.2/apysc/_time/month_end_mixin.py
--rw-r--r--   0 runner    (1001) docker     (127)     5423 2024-05-23 14:23:55.000000 apysc-4.4.2/apysc/_time/month_mixin.py
--rw-r--r--   0 runner    (1001) docker     (127)     2567 2024-05-23 14:23:55.000000 apysc-4.4.2/apysc/_time/now_mixin.py
--rw-r--r--   0 runner    (1001) docker     (127)     5610 2024-05-23 14:23:55.000000 apysc-4.4.2/apysc/_time/second_mixin.py
--rw-r--r--   0 runner    (1001) docker     (127)     5857 2024-05-23 14:23:55.000000 apysc-4.4.2/apysc/_time/timedelta_.py
--rw-r--r--   0 runner    (1001) docker     (127)    22600 2024-05-23 14:23:55.000000 apysc-4.4.2/apysc/_time/timer.py
--rw-r--r--   0 runner    (1001) docker     (127)     3884 2024-05-23 14:23:55.000000 apysc-4.4.2/apysc/_time/total_seconds_mixin.py
--rw-r--r--   0 runner    (1001) docker     (127)     5685 2024-05-23 14:23:55.000000 apysc-4.4.2/apysc/_time/weekday_mixin.py
--rw-r--r--   0 runner    (1001) docker     (127)     5502 2024-05-23 14:23:55.000000 apysc-4.4.2/apysc/_time/year_mixin.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-23 14:24:13.470301 apysc-4.4.2/apysc/_translation/
--rw-r--r--   0 runner    (1001) docker     (127)        0 2024-05-23 14:23:55.000000 apysc-4.4.2/apysc/_translation/__init__.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-23 14:24:13.502302 apysc-4.4.2/apysc/_translation/jp/
--rw-r--r--   0 runner    (1001) docker     (127)        0 2024-05-23 14:23:55.000000 apysc-4.4.2/apysc/_translation/jp/__init__.py
--rw-r--r--   0 runner    (1001) docker     (127)     4745 2024-05-23 14:23:55.000000 apysc-4.4.2/apysc/_translation/jp/about_handler_options_type.py
--rw-r--r--   0 runner    (1001) docker     (127)    15519 2024-05-23 14:23:55.000000 apysc-4.4.2/apysc/_translation/jp/add_child_and_remove_child.py
--rw-r--r--   0 runner    (1001) docker     (127)     7887 2024-05-23 14:23:55.000000 apysc-4.4.2/apysc/_translation/jp/add_debug_info_setting.py
--rw-r--r--   0 runner    (1001) docker     (127)     6631 2024-05-23 14:23:55.000000 apysc-4.4.2/apysc/_translation/jp/animation_base_start.py
--rw-r--r--   0 runner    (1001) docker     (127)     9539 2024-05-23 14:23:55.000000 apysc-4.4.2/apysc/_translation/jp/animation_base_target.py
--rw-r--r--   0 runner    (1001) docker     (127)    15615 2024-05-23 14:23:55.000000 apysc-4.4.2/apysc/_translation/jp/animation_complete.py
--rw-r--r--   0 runner    (1001) docker     (127)     5762 2024-05-23 14:23:55.000000 apysc-4.4.2/apysc/_translation/jp/animation_delay.py
--rw-r--r--   0 runner    (1001) docker     (127)     5628 2024-05-23 14:23:55.000000 apysc-4.4.2/apysc/_translation/jp/animation_duration.py
--rw-r--r--   0 runner    (1001) docker     (127)    14570 2024-05-23 14:23:55.000000 apysc-4.4.2/apysc/_translation/jp/animation_event.py
--rw-r--r--   0 runner    (1001) docker     (127)    11149 2024-05-23 14:23:55.000000 apysc-4.4.2/apysc/_translation/jp/animation_fill_alpha.py
--rw-r--r--   0 runner    (1001) docker     (127)    11581 2024-05-23 14:23:55.000000 apysc-4.4.2/apysc/_translation/jp/animation_fill_color.py
--rw-r--r--   0 runner    (1001) docker     (127)     8243 2024-05-23 14:23:55.000000 apysc-4.4.2/apysc/_translation/jp/animation_finish.py
--rw-r--r--   0 runner    (1001) docker     (127)   148271 2024-05-23 14:23:55.000000 apysc-4.4.2/apysc/_translation/jp/animation_interfaces_abstract.py
--rw-r--r--   0 runner    (1001) docker     (127)    11617 2024-05-23 14:23:55.000000 apysc-4.4.2/apysc/_translation/jp/animation_line_alpha.py
--rw-r--r--   0 runner    (1001) docker     (127)    11991 2024-05-23 14:23:55.000000 apysc-4.4.2/apysc/_translation/jp/animation_line_color.py
--rw-r--r--   0 runner    (1001) docker     (127)    11675 2024-05-23 14:23:55.000000 apysc-4.4.2/apysc/_translation/jp/animation_line_thickness.py
--rw-r--r--   0 runner    (1001) docker     (127)     6146 2024-05-23 14:23:55.000000 apysc-4.4.2/apysc/_translation/jp/animation_method_chaining.py
--rw-r--r--   0 runner    (1001) docker     (127)    11840 2024-05-23 14:23:55.000000 apysc-4.4.2/apysc/_translation/jp/animation_move.py
--rw-r--r--   0 runner    (1001) docker     (127)    13951 2024-05-23 14:23:55.000000 apysc-4.4.2/apysc/_translation/jp/animation_parallel.py
--rw-r--r--   0 runner    (1001) docker     (127)    11297 2024-05-23 14:23:55.000000 apysc-4.4.2/apysc/_translation/jp/animation_pause_and_play.py
--rw-r--r--   0 runner    (1001) docker     (127)    11296 2024-05-23 14:23:55.000000 apysc-4.4.2/apysc/_translation/jp/animation_radius.py
--rw-r--r--   0 runner    (1001) docker     (127)     7758 2024-05-23 14:23:55.000000 apysc-4.4.2/apysc/_translation/jp/animation_reset.py
--rw-r--r--   0 runner    (1001) docker     (127)     6721 2024-05-23 14:23:55.000000 apysc-4.4.2/apysc/_translation/jp/animation_return_value.py
--rw-r--r--   0 runner    (1001) docker     (127)    11605 2024-05-23 14:23:55.000000 apysc-4.4.2/apysc/_translation/jp/animation_reverse.py
--rw-r--r--   0 runner    (1001) docker     (127)    12223 2024-05-23 14:23:55.000000 apysc-4.4.2/apysc/_translation/jp/animation_rotation_around_center.py
--rw-r--r--   0 runner    (1001) docker     (127)    13242 2024-05-23 14:23:55.000000 apysc-4.4.2/apysc/_translation/jp/animation_rotation_around_point.py
--rw-r--r--   0 runner    (1001) docker     (127)    22762 2024-05-23 14:23:55.000000 apysc-4.4.2/apysc/_translation/jp/animation_scale_x_and_y_from_center.py
--rw-r--r--   0 runner    (1001) docker     (127)    10821 2024-05-23 14:23:55.000000 apysc-4.4.2/apysc/_translation/jp/animation_scale_x_and_y_from_point.py
--rw-r--r--   0 runner    (1001) docker     (127)     7337 2024-05-23 14:23:55.000000 apysc-4.4.2/apysc/_translation/jp/animation_time.py
--rw-r--r--   0 runner    (1001) docker     (127)    24560 2024-05-23 14:23:55.000000 apysc-4.4.2/apysc/_translation/jp/animation_width_and_height.py
--rw-r--r--   0 runner    (1001) docker     (127)    13175 2024-05-23 14:23:55.000000 apysc-4.4.2/apysc/_translation/jp/animation_x.py
--rw-r--r--   0 runner    (1001) docker     (127)    13195 2024-05-23 14:23:55.000000 apysc-4.4.2/apysc/_translation/jp/animation_y.py
--rw-r--r--   0 runner    (1001) docker     (127)     6108 2024-05-23 14:23:55.000000 apysc-4.4.2/apysc/_translation/jp/append_js_expression.py
--rw-r--r--   0 runner    (1001) docker     (127)    16267 2024-05-23 14:23:55.000000 apysc-4.4.2/apysc/_translation/jp/array.py
--rw-r--r--   0 runner    (1001) docker     (127)     6138 2024-05-23 14:23:55.000000 apysc-4.4.2/apysc/_translation/jp/array_append_and_push.py
--rw-r--r--   0 runner    (1001) docker     (127)     1546 2024-05-23 14:23:55.000000 apysc-4.4.2/apysc/_translation/jp/array_clear.py
--rw-r--r--   0 runner    (1001) docker     (127)     2627 2024-05-23 14:23:55.000000 apysc-4.4.2/apysc/_translation/jp/array_comparison.py
--rw-r--r--   0 runner    (1001) docker     (127)     8204 2024-05-23 14:23:55.000000 apysc-4.4.2/apysc/_translation/jp/array_extend_and_concat.py
--rw-r--r--   0 runner    (1001) docker     (127)     4822 2024-05-23 14:23:55.000000 apysc-4.4.2/apysc/_translation/jp/array_index_of.py
--rw-r--r--   0 runner    (1001) docker     (127)     6996 2024-05-23 14:23:55.000000 apysc-4.4.2/apysc/_translation/jp/array_insert_and_insert_at.py
--rw-r--r--   0 runner    (1001) docker     (127)     4052 2024-05-23 14:23:55.000000 apysc-4.4.2/apysc/_translation/jp/array_join.py
--rw-r--r--   0 runner    (1001) docker     (127)     6552 2024-05-23 14:23:55.000000 apysc-4.4.2/apysc/_translation/jp/array_last_value.py
--rw-r--r--   0 runner    (1001) docker     (127)     4648 2024-05-23 14:23:55.000000 apysc-4.4.2/apysc/_translation/jp/array_length.py
--rw-r--r--   0 runner    (1001) docker     (127)     3648 2024-05-23 14:23:55.000000 apysc-4.4.2/apysc/_translation/jp/array_pop.py
--rw-r--r--   0 runner    (1001) docker     (127)     6355 2024-05-23 14:23:55.000000 apysc-4.4.2/apysc/_translation/jp/array_remove_and_remove_at.py
--rw-r--r--   0 runner    (1001) docker     (127)     3330 2024-05-23 14:23:55.000000 apysc-4.4.2/apysc/_translation/jp/array_reverse.py
--rw-r--r--   0 runner    (1001) docker     (127)     5547 2024-05-23 14:23:55.000000 apysc-4.4.2/apysc/_translation/jp/array_slice.py
--rw-r--r--   0 runner    (1001) docker     (127)     4882 2024-05-23 14:23:55.000000 apysc-4.4.2/apysc/_translation/jp/array_sort.py
--rw-r--r--   0 runner    (1001) docker     (127)    16401 2024-05-23 14:23:55.000000 apysc-4.4.2/apysc/_translation/jp/assert_arrays_equal_and_arrays_not_equal.py
--rw-r--r--   0 runner    (1001) docker     (127)    11293 2024-05-23 14:23:55.000000 apysc-4.4.2/apysc/_translation/jp/assert_defined_and_undefined.py
--rw-r--r--   0 runner    (1001) docker     (127)    16989 2024-05-23 14:23:55.000000 apysc-4.4.2/apysc/_translation/jp/assert_dicts_equal_and_dicts_not_equal.py
--rw-r--r--   0 runner    (1001) docker     (127)    11725 2024-05-23 14:23:55.000000 apysc-4.4.2/apysc/_translation/jp/assert_equal_and_not_equal.py
--rw-r--r--   0 runner    (1001) docker     (127)    11091 2024-05-23 14:23:55.000000 apysc-4.4.2/apysc/_translation/jp/assert_greater_and_greater_equal.py
--rw-r--r--   0 runner    (1001) docker     (127)    10904 2024-05-23 14:23:55.000000 apysc-4.4.2/apysc/_translation/jp/assert_less_and_less_equal.py
--rw-r--r--   0 runner    (1001) docker     (127)    16034 2024-05-23 14:23:55.000000 apysc-4.4.2/apysc/_translation/jp/assert_true_and_false.py
--rw-r--r--   0 runner    (1001) docker     (127)     6554 2024-05-23 14:23:55.000000 apysc-4.4.2/apysc/_translation/jp/assertion_basic_behavior.py
--rw-r--r--   0 runner    (1001) docker     (127)    25796 2024-05-23 14:23:55.000000 apysc-4.4.2/apysc/_translation/jp/bind_and_trigger_custom_event.py
--rw-r--r--   0 runner    (1001) docker     (127)     5543 2024-05-23 14:23:55.000000 apysc-4.4.2/apysc/_translation/jp/blue_color.py
--rw-r--r--   0 runner    (1001) docker     (127)    15021 2024-05-23 14:23:55.000000 apysc-4.4.2/apysc/_translation/jp/boolean.py
--rw-r--r--   0 runner    (1001) docker     (127)     4715 2024-05-23 14:23:55.000000 apysc-4.4.2/apysc/_translation/jp/branch_instruction_variables_reverting_setting.py
--rw-r--r--   0 runner    (1001) docker     (127)    50491 2024-05-23 14:23:55.000000 apysc-4.4.2/apysc/_translation/jp/circle.py
--rw-r--r--   0 runner    (1001) docker     (127)    19083 2024-05-23 14:23:55.000000 apysc-4.4.2/apysc/_translation/jp/click.py
--rw-r--r--   0 runner    (1001) docker     (127)     8517 2024-05-23 14:23:55.000000 apysc-4.4.2/apysc/_translation/jp/color.py
--rw-r--r--   0 runner    (1001) docker     (127)     7228 2024-05-23 14:23:55.000000 apysc-4.4.2/apysc/_translation/jp/color_from_rgb.py
--rw-r--r--   0 runner    (1001) docker     (127)     2891 2024-05-23 14:23:55.000000 apysc-4.4.2/apysc/_translation/jp/colorless.py
--rw-r--r--   0 runner    (1001) docker     (127)     6468 2024-05-23 14:23:55.000000 apysc-4.4.2/apysc/_translation/jp/colors.py
--rw-r--r--   0 runner    (1001) docker     (127)     7940 2024-05-23 14:23:55.000000 apysc-4.4.2/apysc/_translation/jp/contains.py
--rw-r--r--   0 runner    (1001) docker     (127)     6579 2024-05-23 14:23:55.000000 apysc-4.4.2/apysc/_translation/jp/continue.py
--rw-r--r--   0 runner    (1001) docker     (127)    14038 2024-05-23 14:23:55.000000 apysc-4.4.2/apysc/_translation/jp/datetime.py
--rw-r--r--   0 runner    (1001) docker     (127)     4592 2024-05-23 14:23:55.000000 apysc-4.4.2/apysc/_translation/jp/datetime_day.py
--rw-r--r--   0 runner    (1001) docker     (127)     4705 2024-05-23 14:23:55.000000 apysc-4.4.2/apysc/_translation/jp/datetime_hour.py
--rw-r--r--   0 runner    (1001) docker     (127)     4883 2024-05-23 14:23:55.000000 apysc-4.4.2/apysc/_translation/jp/datetime_millisecond.py
--rw-r--r--   0 runner    (1001) docker     (127)     4779 2024-05-23 14:23:55.000000 apysc-4.4.2/apysc/_translation/jp/datetime_minute.py
--rw-r--r--   0 runner    (1001) docker     (127)     4636 2024-05-23 14:23:55.000000 apysc-4.4.2/apysc/_translation/jp/datetime_month.py
--rw-r--r--   0 runner    (1001) docker     (127)     6808 2024-05-23 14:23:55.000000 apysc-4.4.2/apysc/_translation/jp/datetime_now.py
--rw-r--r--   0 runner    (1001) docker     (127)     4776 2024-05-23 14:23:55.000000 apysc-4.4.2/apysc/_translation/jp/datetime_second.py
--rw-r--r--   0 runner    (1001) docker     (127)     2008 2024-05-23 14:23:55.000000 apysc-4.4.2/apysc/_translation/jp/datetime_set_month_end.py
--rw-r--r--   0 runner    (1001) docker     (127)     9075 2024-05-23 14:23:55.000000 apysc-4.4.2/apysc/_translation/jp/datetime_weekday_js_and_weekday_py.py
--rw-r--r--   0 runner    (1001) docker     (127)     4677 2024-05-23 14:23:55.000000 apysc-4.4.2/apysc/_translation/jp/datetime_year.py
--rw-r--r--   0 runner    (1001) docker     (127)    16704 2024-05-23 14:23:55.000000 apysc-4.4.2/apysc/_translation/jp/dblclick.py
--rw-r--r--   0 runner    (1001) docker     (127)     4735 2024-05-23 14:23:55.000000 apysc-4.4.2/apysc/_translation/jp/delete.py
--rw-r--r--   0 runner    (1001) docker     (127)    12341 2024-05-23 14:23:55.000000 apysc-4.4.2/apysc/_translation/jp/dictionary.py
--rw-r--r--   0 runner    (1001) docker     (127)     5460 2024-05-23 14:23:55.000000 apysc-4.4.2/apysc/_translation/jp/dictionary_generic.py
--rw-r--r--   0 runner    (1001) docker     (127)     5787 2024-05-23 14:23:55.000000 apysc-4.4.2/apysc/_translation/jp/dictionary_get.py
--rw-r--r--   0 runner    (1001) docker     (127)     4594 2024-05-23 14:23:55.000000 apysc-4.4.2/apysc/_translation/jp/dictionary_length.py
--rw-r--r--   0 runner    (1001) docker     (127)     4304 2024-05-23 14:23:55.000000 apysc-4.4.2/apysc/_translation/jp/display_object.py
--rw-r--r--   0 runner    (1001) docker     (127)    23638 2024-05-23 14:23:55.000000 apysc-4.4.2/apysc/_translation/jp/display_object_and_graphics_base_prop_abstract.py
--rw-r--r--   0 runner    (1001) docker     (127)     9845 2024-05-23 14:23:55.000000 apysc-4.4.2/apysc/_translation/jp/display_object_get_and_set_css.py
--rw-r--r--   0 runner    (1001) docker     (127)     5401 2024-05-23 14:23:55.000000 apysc-4.4.2/apysc/_translation/jp/display_object_mouse_event.py
--rw-r--r--   0 runner    (1001) docker     (127)     9053 2024-05-23 14:23:55.000000 apysc-4.4.2/apysc/_translation/jp/display_object_parent.py
--rw-r--r--   0 runner    (1001) docker     (127)     8567 2024-05-23 14:23:55.000000 apysc-4.4.2/apysc/_translation/jp/display_object_visible.py
--rw-r--r--   0 runner    (1001) docker     (127)     9188 2024-05-23 14:23:55.000000 apysc-4.4.2/apysc/_translation/jp/display_object_x_and_y.py
--rw-r--r--   0 runner    (1001) docker     (127)     5691 2024-05-23 14:23:55.000000 apysc-4.4.2/apysc/_translation/jp/display_on_colaboratory.py
--rw-r--r--   0 runner    (1001) docker     (127)     7937 2024-05-23 14:23:55.000000 apysc-4.4.2/apysc/_translation/jp/display_on_jupyter.py
--rw-r--r--   0 runner    (1001) docker     (127)    12092 2024-05-23 14:23:55.000000 apysc-4.4.2/apysc/_translation/jp/draw_interfaces_abstract.py
--rw-r--r--   0 runner    (1001) docker     (127)    85549 2024-05-23 14:23:55.000000 apysc-4.4.2/apysc/_translation/jp/easing_enum.py
--rw-r--r--   0 runner    (1001) docker     (127)    12136 2024-05-23 14:23:55.000000 apysc-4.4.2/apysc/_translation/jp/elif.py
--rw-r--r--   0 runner    (1001) docker     (127)    51515 2024-05-23 14:23:55.000000 apysc-4.4.2/apysc/_translation/jp/ellipse.py
--rw-r--r--   0 runner    (1001) docker     (127)     9150 2024-05-23 14:23:55.000000 apysc-4.4.2/apysc/_translation/jp/else.py
--rw-r--r--   0 runner    (1001) docker     (127)     9718 2024-05-23 14:23:55.000000 apysc-4.4.2/apysc/_translation/jp/enter_frame.py
--rw-r--r--   0 runner    (1001) docker     (127)    12970 2024-05-23 14:23:55.000000 apysc-4.4.2/apysc/_translation/jp/event_prevent_default_and_stop_propagation.py
--rw-r--r--   0 runner    (1001) docker     (127)    10715 2024-05-23 14:23:55.000000 apysc-4.4.2/apysc/_translation/jp/for_array_indices.py
--rw-r--r--   0 runner    (1001) docker     (127)     9997 2024-05-23 14:23:55.000000 apysc-4.4.2/apysc/_translation/jp/for_array_indices_and_values.py
--rw-r--r--   0 runner    (1001) docker     (127)     9557 2024-05-23 14:23:55.000000 apysc-4.4.2/apysc/_translation/jp/for_array_values.py
--rw-r--r--   0 runner    (1001) docker     (127)     9783 2024-05-23 14:23:55.000000 apysc-4.4.2/apysc/_translation/jp/for_dict_keys.py
--rw-r--r--   0 runner    (1001) docker     (127)    11463 2024-05-23 14:23:55.000000 apysc-4.4.2/apysc/_translation/jp/for_dict_keys_and_values.py
--rw-r--r--   0 runner    (1001) docker     (127)     8642 2024-05-23 14:23:55.000000 apysc-4.4.2/apysc/_translation/jp/for_dict_values.py
--rw-r--r--   0 runner    (1001) docker     (127)     5183 2024-05-23 14:23:55.000000 apysc-4.4.2/apysc/_translation/jp/fps.py
--rw-r--r--   0 runner    (1001) docker     (127)     3950 2024-05-23 14:23:55.000000 apysc-4.4.2/apysc/_translation/jp/fundamental_data_classes_value_interface.py
--rw-r--r--   0 runner    (1001) docker     (127)     6667 2024-05-23 14:23:55.000000 apysc-4.4.2/apysc/_translation/jp/get_bounds.py
--rw-r--r--   0 runner    (1001) docker     (127)     6338 2024-05-23 14:23:55.000000 apysc-4.4.2/apysc/_translation/jp/get_child_at.py
--rw-r--r--   0 runner    (1001) docker     (127)    11113 2024-05-23 14:23:55.000000 apysc-4.4.2/apysc/_translation/jp/graphics.py
--rw-r--r--   0 runner    (1001) docker     (127)     5532 2024-05-23 14:23:55.000000 apysc-4.4.2/apysc/_translation/jp/graphics_base_fill_alpha.py
--rw-r--r--   0 runner    (1001) docker     (127)     6524 2024-05-23 14:23:55.000000 apysc-4.4.2/apysc/_translation/jp/graphics_base_fill_color.py
--rw-r--r--   0 runner    (1001) docker     (127)    10271 2024-05-23 14:23:55.000000 apysc-4.4.2/apysc/_translation/jp/graphics_base_flip_interfaces.py
--rw-r--r--   0 runner    (1001) docker     (127)     5622 2024-05-23 14:23:55.000000 apysc-4.4.2/apysc/_translation/jp/graphics_base_line_alpha.py
--rw-r--r--   0 runner    (1001) docker     (127)     6715 2024-05-23 14:23:55.000000 apysc-4.4.2/apysc/_translation/jp/graphics_base_line_color.py
--rw-r--r--   0 runner    (1001) docker     (127)     9355 2024-05-23 14:23:55.000000 apysc-4.4.2/apysc/_translation/jp/graphics_base_line_dash_dot_setting.py
--rw-r--r--   0 runner    (1001) docker     (127)     8863 2024-05-23 14:23:55.000000 apysc-4.4.2/apysc/_translation/jp/graphics_base_line_dash_setting.py
--rw-r--r--   0 runner    (1001) docker     (127)     9053 2024-05-23 14:23:55.000000 apysc-4.4.2/apysc/_translation/jp/graphics_base_line_dot_setting.py
--rw-r--r--   0 runner    (1001) docker     (127)     9250 2024-05-23 14:23:55.000000 apysc-4.4.2/apysc/_translation/jp/graphics_base_line_round_dot_setting.py
--rw-r--r--   0 runner    (1001) docker     (127)     5281 2024-05-23 14:23:55.000000 apysc-4.4.2/apysc/_translation/jp/graphics_base_line_thickness.py
--rw-r--r--   0 runner    (1001) docker     (127)     6753 2024-05-23 14:23:55.000000 apysc-4.4.2/apysc/_translation/jp/graphics_base_rotation_around_center.py
--rw-r--r--   0 runner    (1001) docker     (127)    11688 2024-05-23 14:23:55.000000 apysc-4.4.2/apysc/_translation/jp/graphics_base_rotation_around_point.py
--rw-r--r--   0 runner    (1001) docker     (127)    16144 2024-05-23 14:23:55.000000 apysc-4.4.2/apysc/_translation/jp/graphics_base_scale_from_center.py
--rw-r--r--   0 runner    (1001) docker     (127)    24463 2024-05-23 14:23:55.000000 apysc-4.4.2/apysc/_translation/jp/graphics_base_scale_from_point.py
--rw-r--r--   0 runner    (1001) docker     (127)    10099 2024-05-23 14:23:55.000000 apysc-4.4.2/apysc/_translation/jp/graphics_base_skew.py
--rw-r--r--   0 runner    (1001) docker     (127)    19456 2024-05-23 14:23:55.000000 apysc-4.4.2/apysc/_translation/jp/graphics_begin_fill.py
--rw-r--r--   0 runner    (1001) docker     (127)     3461 2024-05-23 14:23:55.000000 apysc-4.4.2/apysc/_translation/jp/graphics_clear.py
--rw-r--r--   0 runner    (1001) docker     (127)     8915 2024-05-23 14:23:55.000000 apysc-4.4.2/apysc/_translation/jp/graphics_draw_circle.py
--rw-r--r--   0 runner    (1001) docker     (127)     9154 2024-05-23 14:23:55.000000 apysc-4.4.2/apysc/_translation/jp/graphics_draw_dash_dotted_line.py
--rw-r--r--   0 runner    (1001) docker     (127)     8546 2024-05-23 14:23:55.000000 apysc-4.4.2/apysc/_translation/jp/graphics_draw_dashed_line.py
--rw-r--r--   0 runner    (1001) docker     (127)     8098 2024-05-23 14:23:55.000000 apysc-4.4.2/apysc/_translation/jp/graphics_draw_dotted_line.py
--rw-r--r--   0 runner    (1001) docker     (127)    10266 2024-05-23 14:23:55.000000 apysc-4.4.2/apysc/_translation/jp/graphics_draw_ellipse.py
--rw-r--r--   0 runner    (1001) docker     (127)    11252 2024-05-23 14:23:55.000000 apysc-4.4.2/apysc/_translation/jp/graphics_draw_line.py
--rw-r--r--   0 runner    (1001) docker     (127)    10592 2024-05-23 14:23:55.000000 apysc-4.4.2/apysc/_translation/jp/graphics_draw_path.py
--rw-r--r--   0 runner    (1001) docker     (127)    15102 2024-05-23 14:23:55.000000 apysc-4.4.2/apysc/_translation/jp/graphics_draw_polygon.py
--rw-r--r--   0 runner    (1001) docker     (127)    10632 2024-05-23 14:23:55.000000 apysc-4.4.2/apysc/_translation/jp/graphics_draw_rect.py
--rw-r--r--   0 runner    (1001) docker     (127)    11078 2024-05-23 14:23:55.000000 apysc-4.4.2/apysc/_translation/jp/graphics_draw_round_dotted_line.py
--rw-r--r--   0 runner    (1001) docker     (127)    10286 2024-05-23 14:23:55.000000 apysc-4.4.2/apysc/_translation/jp/graphics_draw_round_rect.py
--rw-r--r--   0 runner    (1001) docker     (127)    10974 2024-05-23 14:23:55.000000 apysc-4.4.2/apysc/_translation/jp/graphics_draw_triangle.py
--rw-r--r--   0 runner    (1001) docker     (127)    64374 2024-05-23 14:23:55.000000 apysc-4.4.2/apysc/_translation/jp/graphics_line_style.py
--rw-r--r--   0 runner    (1001) docker     (127)    18270 2024-05-23 14:23:55.000000 apysc-4.4.2/apysc/_translation/jp/graphics_move_to_and_line_to.py
--rw-r--r--   0 runner    (1001) docker     (127)     5571 2024-05-23 14:23:55.000000 apysc-4.4.2/apysc/_translation/jp/green_color.py
--rw-r--r--   0 runner    (1001) docker     (127)     7571 2024-05-23 14:23:55.000000 apysc-4.4.2/apysc/_translation/jp/if.py
--rw-r--r--   0 runner    (1001) docker     (127)     2013 2024-05-23 14:23:55.000000 apysc-4.4.2/apysc/_translation/jp/import_conventions.py
--rw-r--r--   0 runner    (1001) docker     (127)    21046 2024-05-23 14:23:55.000000 apysc-4.4.2/apysc/_translation/jp/index.py
--rw-r--r--   0 runner    (1001) docker     (127)    18347 2024-05-23 14:23:55.000000 apysc-4.4.2/apysc/_translation/jp/int_and_number.py
--rw-r--r--   0 runner    (1001) docker     (127)    11684 2024-05-23 14:23:55.000000 apysc-4.4.2/apysc/_translation/jp/int_and_number_arithmetic_operations.py
--rw-r--r--   0 runner    (1001) docker     (127)     8328 2024-05-23 14:23:55.000000 apysc-4.4.2/apysc/_translation/jp/int_and_number_comparison_operations.py
--rw-r--r--   0 runner    (1001) docker     (127)     7200 2024-05-23 14:23:55.000000 apysc-4.4.2/apysc/_translation/jp/int_and_number_to_fixed.py
--rw-r--r--   0 runner    (1001) docker     (127)     5897 2024-05-23 14:23:55.000000 apysc-4.4.2/apysc/_translation/jp/int_and_number_to_hex.py
--rw-r--r--   0 runner    (1001) docker     (127)    48186 2024-05-23 14:23:55.000000 apysc-4.4.2/apysc/_translation/jp/line.py
--rw-r--r--   0 runner    (1001) docker     (127)     7040 2024-05-23 14:23:55.000000 apysc-4.4.2/apysc/_translation/jp/material_design_colors.py
--rw-r--r--   0 runner    (1001) docker     (127)     9561 2024-05-23 14:23:55.000000 apysc-4.4.2/apysc/_translation/jp/material_icon.py
--rw-r--r--   0 runner    (1001) docker     (127)     4775 2024-05-23 14:23:55.000000 apysc-4.4.2/apysc/_translation/jp/math_max.py
--rw-r--r--   0 runner    (1001) docker     (127)     4765 2024-05-23 14:23:55.000000 apysc-4.4.2/apysc/_translation/jp/math_min.py
--rw-r--r--   0 runner    (1001) docker     (127)     6272 2024-05-23 14:23:55.000000 apysc-4.4.2/apysc/_translation/jp/math_trunc.py
--rw-r--r--   0 runner    (1001) docker     (127)     5815 2024-05-23 14:23:55.000000 apysc-4.4.2/apysc/_translation/jp/mouse_event_abstract.py
--rw-r--r--   0 runner    (1001) docker     (127)    38153 2024-05-23 14:23:55.000000 apysc-4.4.2/apysc/_translation/jp/mouse_event_basic.py
--rw-r--r--   0 runner    (1001) docker     (127)    27701 2024-05-23 14:23:55.000000 apysc-4.4.2/apysc/_translation/jp/mousedown_and_mouseup.py
--rw-r--r--   0 runner    (1001) docker     (127)    17541 2024-05-23 14:23:55.000000 apysc-4.4.2/apysc/_translation/jp/mousemove.py
--rw-r--r--   0 runner    (1001) docker     (127)    28272 2024-05-23 14:23:55.000000 apysc-4.4.2/apysc/_translation/jp/mouseover_and_mouseout.py
--rw-r--r--   0 runner    (1001) docker     (127)    12910 2024-05-23 14:23:55.000000 apysc-4.4.2/apysc/_translation/jp/multi_line_text.py
--rw-r--r--   0 runner    (1001) docker     (127)     7536 2024-05-23 14:23:55.000000 apysc-4.4.2/apysc/_translation/jp/num_children.py
--rw-r--r--   0 runner    (1001) docker     (127)    62153 2024-05-23 14:23:55.000000 apysc-4.4.2/apysc/_translation/jp/path.py
--rw-r--r--   0 runner    (1001) docker     (127)    13516 2024-05-23 14:23:55.000000 apysc-4.4.2/apysc/_translation/jp/path_bezier_2d.py
--rw-r--r--   0 runner    (1001) docker     (127)    11122 2024-05-23 14:23:55.000000 apysc-4.4.2/apysc/_translation/jp/path_bezier_2d_continual.py
--rw-r--r--   0 runner    (1001) docker     (127)    16364 2024-05-23 14:23:55.000000 apysc-4.4.2/apysc/_translation/jp/path_bezier_3d.py
--rw-r--r--   0 runner    (1001) docker     (127)    16314 2024-05-23 14:23:55.000000 apysc-4.4.2/apysc/_translation/jp/path_bezier_3d_continual.py
--rw-r--r--   0 runner    (1001) docker     (127)     6991 2024-05-23 14:23:55.000000 apysc-4.4.2/apysc/_translation/jp/path_close.py
--rw-r--r--   0 runner    (1001) docker     (127)     9572 2024-05-23 14:23:55.000000 apysc-4.4.2/apysc/_translation/jp/path_horizontal.py
--rw-r--r--   0 runner    (1001) docker     (127)     9504 2024-05-23 14:23:55.000000 apysc-4.4.2/apysc/_translation/jp/path_line_to.py
--rw-r--r--   0 runner    (1001) docker     (127)     9884 2024-05-23 14:23:55.000000 apysc-4.4.2/apysc/_translation/jp/path_move_to.py
--rw-r--r--   0 runner    (1001) docker     (127)     9522 2024-05-23 14:23:55.000000 apysc-4.4.2/apysc/_translation/jp/path_vertical.py
--rw-r--r--   0 runner    (1001) docker     (127)    12222 2024-05-23 14:23:55.000000 apysc-4.4.2/apysc/_translation/jp/point2d.py
--rw-r--r--   0 runner    (1001) docker     (127)    50966 2024-05-23 14:23:55.000000 apysc-4.4.2/apysc/_translation/jp/polygon.py
--rw-r--r--   0 runner    (1001) docker     (127)    53243 2024-05-23 14:23:55.000000 apysc-4.4.2/apysc/_translation/jp/polyline.py
--rw-r--r--   0 runner    (1001) docker     (127)     6717 2024-05-23 14:23:55.000000 apysc-4.4.2/apysc/_translation/jp/quick_start.py
--rw-r--r--   0 runner    (1001) docker     (127)     6242 2024-05-23 14:23:55.000000 apysc-4.4.2/apysc/_translation/jp/range.py
--rw-r--r--   0 runner    (1001) docker     (127)     2842 2024-05-23 14:23:55.000000 apysc-4.4.2/apysc/_translation/jp/recommended_type_checker_settings.py
--rw-r--r--   0 runner    (1001) docker     (127)    54921 2024-05-23 14:23:55.000000 apysc-4.4.2/apysc/_translation/jp/rectangle.py
--rw-r--r--   0 runner    (1001) docker     (127)    25542 2024-05-23 14:23:55.000000 apysc-4.4.2/apysc/_translation/jp/rectangle_geom.py
--rw-r--r--   0 runner    (1001) docker     (127)     5008 2024-05-23 14:23:55.000000 apysc-4.4.2/apysc/_translation/jp/red_color.py
--rw-r--r--   0 runner    (1001) docker     (127)     5482 2024-05-23 14:23:55.000000 apysc-4.4.2/apysc/_translation/jp/remove_children.py
--rw-r--r--   0 runner    (1001) docker     (127)     7088 2024-05-23 14:23:55.000000 apysc-4.4.2/apysc/_translation/jp/return.py
--rw-r--r--   0 runner    (1001) docker     (127)    17504 2024-05-23 14:23:55.000000 apysc-4.4.2/apysc/_translation/jp/save_overall_html.py
--rw-r--r--   0 runner    (1001) docker     (127)     4685 2024-05-23 14:23:55.000000 apysc-4.4.2/apysc/_translation/jp/sequential_animation.py
--rw-r--r--   0 runner    (1001) docker     (127)    10214 2024-05-23 14:23:55.000000 apysc-4.4.2/apysc/_translation/jp/set_debug_mode.py
--rw-r--r--   0 runner    (1001) docker     (127)    12228 2024-05-23 14:23:55.000000 apysc-4.4.2/apysc/_translation/jp/sprite.py
--rw-r--r--   0 runner    (1001) docker     (127)    31274 2024-05-23 14:23:55.000000 apysc-4.4.2/apysc/_translation/jp/stage.py
--rw-r--r--   0 runner    (1001) docker     (127)     9480 2024-05-23 14:23:55.000000 apysc-4.4.2/apysc/_translation/jp/string.py
--rw-r--r--   0 runner    (1001) docker     (127)     5468 2024-05-23 14:23:55.000000 apysc-4.4.2/apysc/_translation/jp/string_addition_and_multiplication.py
--rw-r--r--   0 runner    (1001) docker     (127)     6953 2024-05-23 14:23:55.000000 apysc-4.4.2/apysc/_translation/jp/string_apply_max_num_of_decimal_places.py
--rw-r--r--   0 runner    (1001) docker     (127)     6761 2024-05-23 14:23:55.000000 apysc-4.4.2/apysc/_translation/jp/string_comparison_operations.py
--rw-r--r--   0 runner    (1001) docker     (127)     6800 2024-05-23 14:23:55.000000 apysc-4.4.2/apysc/_translation/jp/string_length.py
--rw-r--r--   0 runner    (1001) docker     (127)     3841 2024-05-23 14:23:55.000000 apysc-4.4.2/apysc/_translation/jp/string_lower.py
--rw-r--r--   0 runner    (1001) docker     (127)     7143 2024-05-23 14:23:55.000000 apysc-4.4.2/apysc/_translation/jp/string_lstrip.py
--rw-r--r--   0 runner    (1001) docker     (127)     7074 2024-05-23 14:23:55.000000 apysc-4.4.2/apysc/_translation/jp/string_rstrip.py
--rw-r--r--   0 runner    (1001) docker     (127)     8198 2024-05-23 14:23:55.000000 apysc-4.4.2/apysc/_translation/jp/string_slice.py
--rw-r--r--   0 runner    (1001) docker     (127)     4910 2024-05-23 14:23:55.000000 apysc-4.4.2/apysc/_translation/jp/string_split.py
--rw-r--r--   0 runner    (1001) docker     (127)     7150 2024-05-23 14:23:55.000000 apysc-4.4.2/apysc/_translation/jp/string_strip.py
--rw-r--r--   0 runner    (1001) docker     (127)     3847 2024-05-23 14:23:55.000000 apysc-4.4.2/apysc/_translation/jp/string_upper.py
--rw-r--r--   0 runner    (1001) docker     (127)     5282 2024-05-23 14:23:55.000000 apysc-4.4.2/apysc/_translation/jp/string_zfill.py
--rw-r--r--   0 runner    (1001) docker     (127)    49436 2024-05-23 14:23:55.000000 apysc-4.4.2/apysc/_translation/jp/svg_text.py
--rw-r--r--   0 runner    (1001) docker     (127)    45588 2024-05-23 14:23:55.000000 apysc-4.4.2/apysc/_translation/jp/svg_text_span.py
--rw-r--r--   0 runner    (1001) docker     (127)    11135 2024-05-23 14:23:55.000000 apysc-4.4.2/apysc/_translation/jp/text_align.py
--rw-r--r--   0 runner    (1001) docker     (127)    14274 2024-05-23 14:23:55.000000 apysc-4.4.2/apysc/_translation/jp/text_align_last.py
--rw-r--r--   0 runner    (1001) docker     (127)     5702 2024-05-23 14:23:55.000000 apysc-4.4.2/apysc/_translation/jp/text_bold.py
--rw-r--r--   0 runner    (1001) docker     (127)     5673 2024-05-23 14:23:55.000000 apysc-4.4.2/apysc/_translation/jp/text_fill_alpha.py
--rw-r--r--   0 runner    (1001) docker     (127)     6046 2024-05-23 14:23:55.000000 apysc-4.4.2/apysc/_translation/jp/text_fill_color.py
--rw-r--r--   0 runner    (1001) docker     (127)     5818 2024-05-23 14:23:55.000000 apysc-4.4.2/apysc/_translation/jp/text_font_size.py
--rw-r--r--   0 runner    (1001) docker     (127)     5809 2024-05-23 14:23:55.000000 apysc-4.4.2/apysc/_translation/jp/text_italic.py
--rw-r--r--   0 runner    (1001) docker     (127)     5708 2024-05-23 14:23:55.000000 apysc-4.4.2/apysc/_translation/jp/text_line_height.py
--rw-r--r--   0 runner    (1001) docker     (127)     5755 2024-05-23 14:23:55.000000 apysc-4.4.2/apysc/_translation/jp/text_underline.py
--rw-r--r--   0 runner    (1001) docker     (127)     8047 2024-05-23 14:23:55.000000 apysc-4.4.2/apysc/_translation/jp/timedelta.py
--rw-r--r--   0 runner    (1001) docker     (127)     4820 2024-05-23 14:23:55.000000 apysc-4.4.2/apysc/_translation/jp/timedelta_days.py
--rw-r--r--   0 runner    (1001) docker     (127)     5042 2024-05-23 14:23:55.000000 apysc-4.4.2/apysc/_translation/jp/timedelta_total_seconds.py
--rw-r--r--   0 runner    (1001) docker     (127)    12931 2024-05-23 14:23:55.000000 apysc-4.4.2/apysc/_translation/jp/timer.py
--rw-r--r--   0 runner    (1001) docker     (127)    12198 2024-05-23 14:23:55.000000 apysc-4.4.2/apysc/_translation/jp/timer_complete.py
--rw-r--r--   0 runner    (1001) docker     (127)    17339 2024-05-23 14:23:55.000000 apysc-4.4.2/apysc/_translation/jp/timer_delay.py
--rw-r--r--   0 runner    (1001) docker     (127)    13318 2024-05-23 14:23:55.000000 apysc-4.4.2/apysc/_translation/jp/timer_event.py
--rw-r--r--   0 runner    (1001) docker     (127)    13574 2024-05-23 14:23:55.000000 apysc-4.4.2/apysc/_translation/jp/timer_repeat_count.py
--rw-r--r--   0 runner    (1001) docker     (127)     9013 2024-05-23 14:23:55.000000 apysc-4.4.2/apysc/_translation/jp/timer_reset.py
--rw-r--r--   0 runner    (1001) docker     (127)     9087 2024-05-23 14:23:55.000000 apysc-4.4.2/apysc/_translation/jp/timer_start_and_stop.py
--rw-r--r--   0 runner    (1001) docker     (127)     6814 2024-05-23 14:23:55.000000 apysc-4.4.2/apysc/_translation/jp/to_string.py
--rw-r--r--   0 runner    (1001) docker     (127)     6728 2024-05-23 14:23:55.000000 apysc-4.4.2/apysc/_translation/jp/trace.py
--rw-r--r--   0 runner    (1001) docker     (127)    66343 2024-05-23 14:23:55.000000 apysc-4.4.2/apysc/_translation/jp/triangle.py
--rw-r--r--   0 runner    (1001) docker     (127)     2751 2024-05-23 14:23:55.000000 apysc-4.4.2/apysc/_translation/jp/true_and_false.py
--rw-r--r--   0 runner    (1001) docker     (127)    14525 2024-05-23 14:23:55.000000 apysc-4.4.2/apysc/_translation/jp/unbind_enter_frame_and_unbind_enter_frame_all.py
--rw-r--r--   0 runner    (1001) docker     (127)    10005 2024-05-23 14:23:55.000000 apysc-4.4.2/apysc/_translation/jp/unset_debug_mode.py
--rw-r--r--   0 runner    (1001) docker     (127)     6307 2024-05-23 14:23:55.000000 apysc-4.4.2/apysc/_translation/jp/variable_name_suffix.py
--rw-r--r--   0 runner    (1001) docker     (127)    19570 2024-05-23 14:23:55.000000 apysc-4.4.2/apysc/_translation/jp/what_apysc_can_do.py
--rw-r--r--   0 runner    (1001) docker     (127)     3509 2024-05-23 14:23:55.000000 apysc-4.4.2/apysc/_translation/jp/why_apysc_doesnt_use_python_builtin_data_type.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-23 14:24:13.506301 apysc-4.4.2/apysc/_type/
--rw-r--r--   0 runner    (1001) docker     (127)        0 2024-05-23 14:23:55.000000 apysc-4.4.2/apysc/_type/__init__.py
--rw-r--r--   0 runner    (1001) docker     (127)     1491 2024-05-23 14:23:55.000000 apysc-4.4.2/apysc/_type/_delete.py
--rw-r--r--   0 runner    (1001) docker     (127)     1947 2024-05-23 14:23:55.000000 apysc-4.4.2/apysc/_type/_return.py
--rw-r--r--   0 runner    (1001) docker     (127)    17556 2024-05-23 14:23:55.000000 apysc-4.4.2/apysc/_type/any_value.py
--rw-r--r--   0 runner    (1001) docker     (127)    50943 2024-05-23 14:23:55.000000 apysc-4.4.2/apysc/_type/array.py
--rw-r--r--   0 runner    (1001) docker     (127)     4699 2024-05-23 14:23:55.000000 apysc-4.4.2/apysc/_type/attr_linking_mixin.py
--rw-r--r--   0 runner    (1001) docker     (127)     5282 2024-05-23 14:23:55.000000 apysc-4.4.2/apysc/_type/attr_to_apysc_val_from_builtin_mixin.py
--rw-r--r--   0 runner    (1001) docker     (127)     1817 2024-05-23 14:23:55.000000 apysc-4.4.2/apysc/_type/blank_object_mixin.py
--rw-r--r--   0 runner    (1001) docker     (127)     3445 2024-05-23 14:23:55.000000 apysc-4.4.2/apysc/_type/bool_const_mixin.py
--rw-r--r--   0 runner    (1001) docker     (127)    17955 2024-05-23 14:23:55.000000 apysc-4.4.2/apysc/_type/boolean.py
--rw-r--r--   0 runner    (1001) docker     (127)      389 2024-05-23 14:23:55.000000 apysc-4.4.2/apysc/_type/copy_interface.py
--rw-r--r--   0 runner    (1001) docker     (127)     3259 2024-05-23 14:23:55.000000 apysc-4.4.2/apysc/_type/copy_mixin.py
--rw-r--r--   0 runner    (1001) docker     (127)     3330 2024-05-23 14:23:55.000000 apysc-4.4.2/apysc/_type/deleted_object_mixin.py
--rw-r--r--   0 runner    (1001) docker     (127)    24160 2024-05-23 14:23:55.000000 apysc-4.4.2/apysc/_type/dictionary.py
--rw-r--r--   0 runner    (1001) docker     (127)      391 2024-05-23 14:23:55.000000 apysc-4.4.2/apysc/_type/dictionary_structure.py
--rw-r--r--   0 runner    (1001) docker     (127)     1707 2024-05-23 14:23:55.000000 apysc-4.4.2/apysc/_type/expression_string.py
--rw-r--r--   0 runner    (1001) docker     (127)      803 2024-05-23 14:23:55.000000 apysc-4.4.2/apysc/_type/false.py
--rw-r--r--   0 runner    (1001) docker     (127)      237 2024-05-23 14:23:55.000000 apysc-4.4.2/apysc/_type/hashable_interface.py
--rw-r--r--   0 runner    (1001) docker     (127)     1360 2024-05-23 14:23:55.000000 apysc-4.4.2/apysc/_type/initial_substitution_exp_mixin.py
--rw-r--r--   0 runner    (1001) docker     (127)      975 2024-05-23 14:23:55.000000 apysc-4.4.2/apysc/_type/initialize_locals_and_globals_mixin.py
--rw-r--r--   0 runner    (1001) docker     (127)     7428 2024-05-23 14:23:55.000000 apysc-4.4.2/apysc/_type/int.py
--rw-r--r--   0 runner    (1001) docker     (127)     6739 2024-05-23 14:23:55.000000 apysc-4.4.2/apysc/_type/number.py
--rw-r--r--   0 runner    (1001) docker     (127)    35138 2024-05-23 14:23:55.000000 apysc-4.4.2/apysc/_type/number_value_mixin.py
--rw-r--r--   0 runner    (1001) docker     (127)      569 2024-05-23 14:23:55.000000 apysc-4.4.2/apysc/_type/py_builtin_iter_disabling_mixin.py
--rw-r--r--   0 runner    (1001) docker     (127)      324 2024-05-23 14:23:55.000000 apysc-4.4.2/apysc/_type/repr_interface.py
--rw-r--r--   0 runner    (1001) docker     (127)      656 2024-05-23 14:23:55.000000 apysc-4.4.2/apysc/_type/revert_interface.py
--rw-r--r--   0 runner    (1001) docker     (127)    10223 2024-05-23 14:23:55.000000 apysc-4.4.2/apysc/_type/revert_mixin.py
--rw-r--r--   0 runner    (1001) docker     (127)    28760 2024-05-23 14:23:55.000000 apysc-4.4.2/apysc/_type/string.py
--rw-r--r--   0 runner    (1001) docker     (127)     4666 2024-05-23 14:23:55.000000 apysc-4.4.2/apysc/_type/string_apply_max_num_of_decimal_places_mixin.py
--rw-r--r--   0 runner    (1001) docker     (127)     1774 2024-05-23 14:23:55.000000 apysc-4.4.2/apysc/_type/string_length_mixin.py
--rw-r--r--   0 runner    (1001) docker     (127)     1489 2024-05-23 14:23:55.000000 apysc-4.4.2/apysc/_type/string_lower_mixin.py
--rw-r--r--   0 runner    (1001) docker     (127)     6682 2024-05-23 14:23:55.000000 apysc-4.4.2/apysc/_type/string_lstrip_mixin.py
--rw-r--r--   0 runner    (1001) docker     (127)     6652 2024-05-23 14:23:55.000000 apysc-4.4.2/apysc/_type/string_rstrip_mixin.py
--rw-r--r--   0 runner    (1001) docker     (127)     4204 2024-05-23 14:23:55.000000 apysc-4.4.2/apysc/_type/string_slice_mixin.py
--rw-r--r--   0 runner    (1001) docker     (127)     2364 2024-05-23 14:23:55.000000 apysc-4.4.2/apysc/_type/string_split_mixin.py
--rw-r--r--   0 runner    (1001) docker     (127)     6806 2024-05-23 14:23:55.000000 apysc-4.4.2/apysc/_type/string_strip_mixin.py
--rw-r--r--   0 runner    (1001) docker     (127)     1497 2024-05-23 14:23:55.000000 apysc-4.4.2/apysc/_type/string_upper_mixin.py
--rw-r--r--   0 runner    (1001) docker     (127)     2361 2024-05-23 14:23:55.000000 apysc-4.4.2/apysc/_type/string_zfill_mixin.py
--rw-r--r--   0 runner    (1001) docker     (127)     3083 2024-05-23 14:23:55.000000 apysc-4.4.2/apysc/_type/to_fixed_mixin.py
--rw-r--r--   0 runner    (1001) docker     (127)     2358 2024-05-23 14:23:55.000000 apysc-4.4.2/apysc/_type/to_hex_mixin.py
--rw-r--r--   0 runner    (1001) docker     (127)     1737 2024-05-23 14:23:55.000000 apysc-4.4.2/apysc/_type/to_number_mixin.py
--rw-r--r--   0 runner    (1001) docker     (127)     1637 2024-05-23 14:23:55.000000 apysc-4.4.2/apysc/_type/to_string_mixin.py
--rw-r--r--   0 runner    (1001) docker     (127)      796 2024-05-23 14:23:55.000000 apysc-4.4.2/apysc/_type/true.py
--rw-r--r--   0 runner    (1001) docker     (127)      370 2024-05-23 14:23:55.000000 apysc-4.4.2/apysc/_type/type_name_mixin.py
--rw-r--r--   0 runner    (1001) docker     (127)     3940 2024-05-23 14:23:55.000000 apysc-4.4.2/apysc/_type/type_util.py
--rw-r--r--   0 runner    (1001) docker     (127)     5295 2024-05-23 14:23:55.000000 apysc-4.4.2/apysc/_type/value_util.py
--rw-r--r--   0 runner    (1001) docker     (127)     2244 2024-05-23 14:23:55.000000 apysc-4.4.2/apysc/_type/variable_name_mixin.py
--rw-r--r--   0 runner    (1001) docker     (127)     1382 2024-05-23 14:23:55.000000 apysc-4.4.2/apysc/_type/variable_name_suffix_attr_or_var_mixin.py
--rw-r--r--   0 runner    (1001) docker     (127)      747 2024-05-23 14:23:55.000000 apysc-4.4.2/apysc/_type/variable_name_suffix_mixin.py
--rw-r--r--   0 runner    (1001) docker     (127)     1255 2024-05-23 14:23:55.000000 apysc-4.4.2/apysc/_type/variable_name_suffix_utils.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-23 14:24:13.510301 apysc-4.4.2/apysc/_validation/
--rw-r--r--   0 runner    (1001) docker     (127)        0 2024-05-23 14:23:55.000000 apysc-4.4.2/apysc/_validation/__init__.py
--rw-r--r--   0 runner    (1001) docker     (127)   119148 2024-05-23 14:23:55.000000 apysc-4.4.2/apysc/_validation/arg_validation_decos.py
--rw-r--r--   0 runner    (1001) docker     (127)     1847 2024-05-23 14:23:55.000000 apysc-4.4.2/apysc/_validation/bool_validation.py
--rw-r--r--   0 runner    (1001) docker     (127)     2393 2024-05-23 14:23:55.000000 apysc-4.4.2/apysc/_validation/color_validation.py
--rw-r--r--   0 runner    (1001) docker     (127)    10661 2024-05-23 14:23:55.000000 apysc-4.4.2/apysc/_validation/display_validation.py
--rw-r--r--   0 runner    (1001) docker     (127)     1725 2024-05-23 14:23:55.000000 apysc-4.4.2/apysc/_validation/event_validation.py
--rw-r--r--   0 runner    (1001) docker     (127)      949 2024-05-23 14:23:55.000000 apysc-4.4.2/apysc/_validation/geom_validation.py
--rw-r--r--   0 runner    (1001) docker     (127)     2700 2024-05-23 14:23:55.000000 apysc-4.4.2/apysc/_validation/handler_validation.py
--rw-r--r--   0 runner    (1001) docker     (127)     5682 2024-05-23 14:23:55.000000 apysc-4.4.2/apysc/_validation/matrix_data_validation.py
--rw-r--r--   0 runner    (1001) docker     (127)     8629 2024-05-23 14:23:55.000000 apysc-4.4.2/apysc/_validation/number_validation.py
--rw-r--r--   0 runner    (1001) docker     (127)     1081 2024-05-23 14:23:55.000000 apysc-4.4.2/apysc/_validation/parent_validation.py
--rw-r--r--   0 runner    (1001) docker     (127)     4619 2024-05-23 14:23:55.000000 apysc-4.4.2/apysc/_validation/path_validation.py
--rw-r--r--   0 runner    (1001) docker     (127)     3405 2024-05-23 14:23:55.000000 apysc-4.4.2/apysc/_validation/string_validation.py
--rw-r--r--   0 runner    (1001) docker     (127)      595 2024-05-23 14:23:55.000000 apysc-4.4.2/apysc/_validation/validation_common_utils.py
--rw-r--r--   0 runner    (1001) docker     (127)     1151 2024-05-23 14:23:55.000000 apysc-4.4.2/apysc/_validation/variable_name_validation.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-23 14:24:13.278299 apysc-4.4.2/apysc.egg-info/
--rw-r--r--   0 runner    (1001) docker     (127)      828 2024-05-23 14:24:13.000000 apysc-4.4.2/apysc.egg-info/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (127)    99030 2024-05-23 14:24:13.000000 apysc-4.4.2/apysc.egg-info/SOURCES.txt
--rw-r--r--   0 runner    (1001) docker     (127)        1 2024-05-23 14:24:13.000000 apysc-4.4.2/apysc.egg-info/dependency_links.txt
--rw-r--r--   0 runner    (1001) docker     (127)       32 2024-05-23 14:24:13.000000 apysc-4.4.2/apysc.egg-info/requires.txt
--rw-r--r--   0 runner    (1001) docker     (127)        6 2024-05-23 14:24:13.000000 apysc-4.4.2/apysc.egg-info/top_level.txt
--rw-r--r--   0 runner    (1001) docker     (127)       38 2024-05-23 14:24:13.510301 apysc-4.4.2/setup.cfg
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-29 12:25:10.195791 apysc-4.4.3/
+-rw-r--r--   0 runner    (1001) docker     (127)     1064 2024-05-29 12:24:48.000000 apysc-4.4.3/LICENSE
+-rw-r--r--   0 runner    (1001) docker     (127)       24 2024-05-29 12:24:48.000000 apysc-4.4.3/MANIFEST.in
+-rw-r--r--   0 runner    (1001) docker     (127)      828 2024-05-29 12:25:10.195791 apysc-4.4.3/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (127)     6982 2024-05-29 12:24:48.000000 apysc-4.4.3/README.md
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-29 12:25:09.975790 apysc-4.4.3/apysc/
+-rw-r--r--   0 runner    (1001) docker     (127)   121550 2024-05-29 12:24:48.000000 apysc-4.4.3/apysc/__init__.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-29 12:25:09.983790 apysc-4.4.3/apysc/_animation/
+-rw-r--r--   0 runner    (1001) docker     (127)        0 2024-05-29 12:24:48.000000 apysc-4.4.3/apysc/_animation/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (127)    10351 2024-05-29 12:24:48.000000 apysc-4.4.3/apysc/_animation/animation_base.py
+-rw-r--r--   0 runner    (1001) docker     (127)     4646 2024-05-29 12:24:48.000000 apysc-4.4.3/apysc/_animation/animation_cx.py
+-rw-r--r--   0 runner    (1001) docker     (127)     3350 2024-05-29 12:24:48.000000 apysc-4.4.3/apysc/_animation/animation_cx_mixin.py
+-rw-r--r--   0 runner    (1001) docker     (127)     4646 2024-05-29 12:24:48.000000 apysc-4.4.3/apysc/_animation/animation_cy.py
+-rw-r--r--   0 runner    (1001) docker     (127)     3353 2024-05-29 12:24:48.000000 apysc-4.4.3/apysc/_animation/animation_cy_mixin.py
+-rw-r--r--   0 runner    (1001) docker     (127)     4809 2024-05-29 12:24:48.000000 apysc-4.4.3/apysc/_animation/animation_fill_alpha.py
+-rw-r--r--   0 runner    (1001) docker     (127)     3406 2024-05-29 12:24:48.000000 apysc-4.4.3/apysc/_animation/animation_fill_alpha_mixin.py
+-rw-r--r--   0 runner    (1001) docker     (127)     4613 2024-05-29 12:24:48.000000 apysc-4.4.3/apysc/_animation/animation_fill_color.py
+-rw-r--r--   0 runner    (1001) docker     (127)     3553 2024-05-29 12:24:48.000000 apysc-4.4.3/apysc/_animation/animation_fill_color_mixin.py
+-rw-r--r--   0 runner    (1001) docker     (127)     1851 2024-05-29 12:24:48.000000 apysc-4.4.3/apysc/_animation/animation_finish_mixin.py
+-rw-r--r--   0 runner    (1001) docker     (127)     4744 2024-05-29 12:24:48.000000 apysc-4.4.3/apysc/_animation/animation_height.py
+-rw-r--r--   0 runner    (1001) docker     (127)     4942 2024-05-29 12:24:48.000000 apysc-4.4.3/apysc/_animation/animation_height_for_ellipse.py
+-rw-r--r--   0 runner    (1001) docker     (127)     3245 2024-05-29 12:24:48.000000 apysc-4.4.3/apysc/_animation/animation_height_for_ellipse_mixin.py
+-rw-r--r--   0 runner    (1001) docker     (127)     3504 2024-05-29 12:24:48.000000 apysc-4.4.3/apysc/_animation/animation_height_mixin.py
+-rw-r--r--   0 runner    (1001) docker     (127)     4974 2024-05-29 12:24:48.000000 apysc-4.4.3/apysc/_animation/animation_line_alpha.py
+-rw-r--r--   0 runner    (1001) docker     (127)     3659 2024-05-29 12:24:48.000000 apysc-4.4.3/apysc/_animation/animation_line_alpha_mixin.py
+-rw-r--r--   0 runner    (1001) docker     (127)     4663 2024-05-29 12:24:48.000000 apysc-4.4.3/apysc/_animation/animation_line_color.py
+-rw-r--r--   0 runner    (1001) docker     (127)     3630 2024-05-29 12:24:48.000000 apysc-4.4.3/apysc/_animation/animation_line_color_mixin.py
+-rw-r--r--   0 runner    (1001) docker     (127)     5038 2024-05-29 12:24:48.000000 apysc-4.4.3/apysc/_animation/animation_line_thickness.py
+-rw-r--r--   0 runner    (1001) docker     (127)     3746 2024-05-29 12:24:48.000000 apysc-4.4.3/apysc/_animation/animation_line_thickness_mixin.py
+-rw-r--r--   0 runner    (1001) docker     (127)      721 2024-05-29 12:24:48.000000 apysc-4.4.3/apysc/_animation/animation_mixins.py
+-rw-r--r--   0 runner    (1001) docker     (127)     5340 2024-05-29 12:24:48.000000 apysc-4.4.3/apysc/_animation/animation_move.py
+-rw-r--r--   0 runner    (1001) docker     (127)     3674 2024-05-29 12:24:48.000000 apysc-4.4.3/apysc/_animation/animation_move_mixin.py
+-rw-r--r--   0 runner    (1001) docker     (127)    10250 2024-05-29 12:24:48.000000 apysc-4.4.3/apysc/_animation/animation_parallel.py
+-rw-r--r--   0 runner    (1001) docker     (127)     4186 2024-05-29 12:24:48.000000 apysc-4.4.3/apysc/_animation/animation_parallel_mixin.py
+-rw-r--r--   0 runner    (1001) docker     (127)     1818 2024-05-29 12:24:48.000000 apysc-4.4.3/apysc/_animation/animation_pause_mixin.py
+-rw-r--r--   0 runner    (1001) docker     (127)     2084 2024-05-29 12:24:48.000000 apysc-4.4.3/apysc/_animation/animation_play_mixin.py
+-rw-r--r--   0 runner    (1001) docker     (127)     4678 2024-05-29 12:24:48.000000 apysc-4.4.3/apysc/_animation/animation_radius.py
+-rw-r--r--   0 runner    (1001) docker     (127)     3418 2024-05-29 12:24:48.000000 apysc-4.4.3/apysc/_animation/animation_radius_mixin.py
+-rw-r--r--   0 runner    (1001) docker     (127)     1790 2024-05-29 12:24:48.000000 apysc-4.4.3/apysc/_animation/animation_reset_mixin.py
+-rw-r--r--   0 runner    (1001) docker     (127)     2220 2024-05-29 12:24:48.000000 apysc-4.4.3/apysc/_animation/animation_reverse_mixin.py
+-rw-r--r--   0 runner    (1001) docker     (127)     6189 2024-05-29 12:24:48.000000 apysc-4.4.3/apysc/_animation/animation_rotation_around_center.py
+-rw-r--r--   0 runner    (1001) docker     (127)     3836 2024-05-29 12:24:48.000000 apysc-4.4.3/apysc/_animation/animation_rotation_around_center_mixin.py
+-rw-r--r--   0 runner    (1001) docker     (127)     7607 2024-05-29 12:24:48.000000 apysc-4.4.3/apysc/_animation/animation_rotation_around_point.py
+-rw-r--r--   0 runner    (1001) docker     (127)     4292 2024-05-29 12:24:48.000000 apysc-4.4.3/apysc/_animation/animation_rotation_around_point_mixin.py
+-rw-r--r--   0 runner    (1001) docker     (127)     6052 2024-05-29 12:24:48.000000 apysc-4.4.3/apysc/_animation/animation_scale_x_from_center.py
+-rw-r--r--   0 runner    (1001) docker     (127)     3816 2024-05-29 12:24:48.000000 apysc-4.4.3/apysc/_animation/animation_scale_x_from_center_mixin.py
+-rw-r--r--   0 runner    (1001) docker     (127)     6911 2024-05-29 12:24:48.000000 apysc-4.4.3/apysc/_animation/animation_scale_x_from_point.py
+-rw-r--r--   0 runner    (1001) docker     (127)     4032 2024-05-29 12:24:48.000000 apysc-4.4.3/apysc/_animation/animation_scale_x_from_point_mixin.py
+-rw-r--r--   0 runner    (1001) docker     (127)     6052 2024-05-29 12:24:48.000000 apysc-4.4.3/apysc/_animation/animation_scale_y_from_center.py
+-rw-r--r--   0 runner    (1001) docker     (127)     3813 2024-05-29 12:24:48.000000 apysc-4.4.3/apysc/_animation/animation_scale_y_from_center_mixin.py
+-rw-r--r--   0 runner    (1001) docker     (127)     6921 2024-05-29 12:24:48.000000 apysc-4.4.3/apysc/_animation/animation_scale_y_from_point.py
+-rw-r--r--   0 runner    (1001) docker     (127)     4034 2024-05-29 12:24:48.000000 apysc-4.4.3/apysc/_animation/animation_scale_y_from_point_mixin.py
+-rw-r--r--   0 runner    (1001) docker     (127)     2192 2024-05-29 12:24:48.000000 apysc-4.4.3/apysc/_animation/animation_time_mixin.py
+-rw-r--r--   0 runner    (1001) docker     (127)     4730 2024-05-29 12:24:48.000000 apysc-4.4.3/apysc/_animation/animation_width.py
+-rw-r--r--   0 runner    (1001) docker     (127)     4922 2024-05-29 12:24:48.000000 apysc-4.4.3/apysc/_animation/animation_width_for_ellipse.py
+-rw-r--r--   0 runner    (1001) docker     (127)     3653 2024-05-29 12:24:48.000000 apysc-4.4.3/apysc/_animation/animation_width_for_ellipse_mixin.py
+-rw-r--r--   0 runner    (1001) docker     (127)     3484 2024-05-29 12:24:48.000000 apysc-4.4.3/apysc/_animation/animation_width_mixin.py
+-rw-r--r--   0 runner    (1001) docker     (127)     4654 2024-05-29 12:24:48.000000 apysc-4.4.3/apysc/_animation/animation_x.py
+-rw-r--r--   0 runner    (1001) docker     (127)     3333 2024-05-29 12:24:48.000000 apysc-4.4.3/apysc/_animation/animation_x_mixin.py
+-rw-r--r--   0 runner    (1001) docker     (127)     4645 2024-05-29 12:24:48.000000 apysc-4.4.3/apysc/_animation/animation_y.py
+-rw-r--r--   0 runner    (1001) docker     (127)     3333 2024-05-29 12:24:48.000000 apysc-4.4.3/apysc/_animation/animation_y_mixin.py
+-rw-r--r--   0 runner    (1001) docker     (127)     5409 2024-05-29 12:24:48.000000 apysc-4.4.3/apysc/_animation/easing.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-29 12:25:09.983790 apysc-4.4.3/apysc/_auto_reloading/
+-rw-r--r--   0 runner    (1001) docker     (127)        0 2024-05-29 12:24:48.000000 apysc-4.4.3/apysc/_auto_reloading/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (127)     3700 2024-05-29 12:24:48.000000 apysc-4.4.3/apysc/_auto_reloading/auto_reloading_decorator.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-29 12:25:09.983790 apysc-4.4.3/apysc/_branch/
+-rw-r--r--   0 runner    (1001) docker     (127)        0 2024-05-29 12:24:48.000000 apysc-4.4.3/apysc/_branch/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (127)     5575 2024-05-29 12:24:48.000000 apysc-4.4.3/apysc/_branch/_elif.py
+-rw-r--r--   0 runner    (1001) docker     (127)     3981 2024-05-29 12:24:48.000000 apysc-4.4.3/apysc/_branch/_else.py
+-rw-r--r--   0 runner    (1001) docker     (127)     3781 2024-05-29 12:24:48.000000 apysc-4.4.3/apysc/_branch/_if.py
+-rw-r--r--   0 runner    (1001) docker     (127)     4806 2024-05-29 12:24:48.000000 apysc-4.4.3/apysc/_branch/if_base.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-29 12:25:09.983790 apysc-4.4.3/apysc/_callable/
+-rw-r--r--   0 runner    (1001) docker     (127)        0 2024-05-29 12:24:48.000000 apysc-4.4.3/apysc/_callable/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (127)     3444 2024-05-29 12:24:48.000000 apysc-4.4.3/apysc/_callable/callable_util.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-29 12:25:09.991790 apysc-4.4.3/apysc/_chart/
+-rw-r--r--   0 runner    (1001) docker     (127)        0 2024-05-29 12:24:48.000000 apysc-4.4.3/apysc/_chart/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (127)     2177 2024-05-29 12:24:48.000000 apysc-4.4.3/apysc/_chart/add_background_mixin.py
+-rw-r--r--   0 runner    (1001) docker     (127)     1768 2024-05-29 12:24:48.000000 apysc-4.4.3/apysc/_chart/add_border_mixin.py
+-rw-r--r--   0 runner    (1001) docker     (127)     1516 2024-05-29 12:24:48.000000 apysc-4.4.3/apysc/_chart/axis_label_bold_mixin.py
+-rw-r--r--   0 runner    (1001) docker     (127)     1538 2024-05-29 12:24:48.000000 apysc-4.4.3/apysc/_chart/axis_label_fill_alpha_mixin.py
+-rw-r--r--   0 runner    (1001) docker     (127)      871 2024-05-29 12:24:48.000000 apysc-4.4.3/apysc/_chart/axis_label_fill_color_mixin.py
+-rw-r--r--   0 runner    (1001) docker     (127)     1896 2024-05-29 12:24:48.000000 apysc-4.4.3/apysc/_chart/axis_label_font_family_mixin.py
+-rw-r--r--   0 runner    (1001) docker     (127)     1578 2024-05-29 12:24:48.000000 apysc-4.4.3/apysc/_chart/axis_label_font_size_mixin.py
+-rw-r--r--   0 runner    (1001) docker     (127)     1557 2024-05-29 12:24:48.000000 apysc-4.4.3/apysc/_chart/axis_label_italic_mixin.py
+-rw-r--r--   0 runner    (1001) docker     (127)     1477 2024-05-29 12:24:48.000000 apysc-4.4.3/apysc/_chart/axis_line_alpha_mixin.py
+-rw-r--r--   0 runner    (1001) docker     (127)      757 2024-05-29 12:24:48.000000 apysc-4.4.3/apysc/_chart/axis_line_color_mixin.py
+-rw-r--r--   0 runner    (1001) docker     (127)     1535 2024-05-29 12:24:48.000000 apysc-4.4.3/apysc/_chart/axis_line_thickness_mixin.py
+-rw-r--r--   0 runner    (1001) docker     (127)     1277 2024-05-29 12:24:48.000000 apysc-4.4.3/apysc/_chart/background_container_mixin.py
+-rw-r--r--   0 runner    (1001) docker     (127)     1249 2024-05-29 12:24:48.000000 apysc-4.4.3/apysc/_chart/border_container_mixin.py
+-rw-r--r--   0 runner    (1001) docker     (127)      118 2024-05-29 12:24:48.000000 apysc-4.4.3/apysc/_chart/chart_const.py
+-rw-r--r--   0 runner    (1001) docker     (127)     1242 2024-05-29 12:24:48.000000 apysc-4.4.3/apysc/_chart/chart_container_mixin.py
+-rw-r--r--   0 runner    (1001) docker     (127)    22705 2024-05-29 12:24:48.000000 apysc-4.4.3/apysc/_chart/create_single_column_y_axis_mixin.py
+-rw-r--r--   0 runner    (1001) docker     (127)     2975 2024-05-29 12:24:48.000000 apysc-4.4.3/apysc/_chart/initialize_each_container_mixin.py
+-rw-r--r--   0 runner    (1001) docker     (127)     1583 2024-05-29 12:24:48.000000 apysc-4.4.3/apysc/_chart/is_display_axis_label_mixin.py
+-rw-r--r--   0 runner    (1001) docker     (127)      935 2024-05-29 12:24:48.000000 apysc-4.4.3/apysc/_chart/overall_container_mixin.py
+-rw-r--r--   0 runner    (1001) docker     (127)     1649 2024-05-29 12:24:48.000000 apysc-4.4.3/apysc/_chart/set_initial_background_fill_alpha_mixin.py
+-rw-r--r--   0 runner    (1001) docker     (127)      905 2024-05-29 12:24:48.000000 apysc-4.4.3/apysc/_chart/set_initial_background_fill_color_mixin.py
+-rw-r--r--   0 runner    (1001) docker     (127)     1488 2024-05-29 12:24:48.000000 apysc-4.4.3/apysc/_chart/set_initial_border_alpha_mixin.py
+-rw-r--r--   0 runner    (1001) docker     (127)      815 2024-05-29 12:24:48.000000 apysc-4.4.3/apysc/_chart/set_initial_border_color_mixin.py
+-rw-r--r--   0 runner    (1001) docker     (127)     1521 2024-05-29 12:24:48.000000 apysc-4.4.3/apysc/_chart/set_initial_border_thickness_mixin.py
+-rw-r--r--   0 runner    (1001) docker     (127)     1266 2024-05-29 12:24:48.000000 apysc-4.4.3/apysc/_chart/set_initial_height_mixin.py
+-rw-r--r--   0 runner    (1001) docker     (127)     1502 2024-05-29 12:24:48.000000 apysc-4.4.3/apysc/_chart/set_initial_horizontal_padding_mixin.py
+-rw-r--r--   0 runner    (1001) docker     (127)     3859 2024-05-29 12:24:48.000000 apysc-4.4.3/apysc/_chart/set_initial_matrix_data_mixin.py
+-rw-r--r--   0 runner    (1001) docker     (127)     1236 2024-05-29 12:24:48.000000 apysc-4.4.3/apysc/_chart/set_initial_overall_container_coordinates_mixin.py
+-rw-r--r--   0 runner    (1001) docker     (127)     1472 2024-05-29 12:24:48.000000 apysc-4.4.3/apysc/_chart/set_initial_vertical_padding_mixin.py
+-rw-r--r--   0 runner    (1001) docker     (127)     1253 2024-05-29 12:24:48.000000 apysc-4.4.3/apysc/_chart/set_initial_width_mixin.py
+-rw-r--r--   0 runner    (1001) docker     (127)     1238 2024-05-29 12:24:48.000000 apysc-4.4.3/apysc/_chart/set_initial_x_mixin.py
+-rw-r--r--   0 runner    (1001) docker     (127)     1238 2024-05-29 12:24:48.000000 apysc-4.4.3/apysc/_chart/set_initial_y_mixin.py
+-rw-r--r--   0 runner    (1001) docker     (127)     1461 2024-05-29 12:24:48.000000 apysc-4.4.3/apysc/_chart/tick_max_num_mixin.py
+-rw-r--r--   0 runner    (1001) docker     (127)     1422 2024-05-29 12:24:48.000000 apysc-4.4.3/apysc/_chart/tick_text_bold_mixin.py
+-rw-r--r--   0 runner    (1001) docker     (127)     1450 2024-05-29 12:24:48.000000 apysc-4.4.3/apysc/_chart/tick_text_fill_alpha_mixin.py
+-rw-r--r--   0 runner    (1001) docker     (127)      866 2024-05-29 12:24:48.000000 apysc-4.4.3/apysc/_chart/tick_text_fill_color_mixin.py
+-rw-r--r--   0 runner    (1001) docker     (127)     1879 2024-05-29 12:24:48.000000 apysc-4.4.3/apysc/_chart/tick_text_font_family_mixin.py
+-rw-r--r--   0 runner    (1001) docker     (127)     1463 2024-05-29 12:24:48.000000 apysc-4.4.3/apysc/_chart/tick_text_font_size_mixin.py
+-rw-r--r--   0 runner    (1001) docker     (127)     1481 2024-05-29 12:24:48.000000 apysc-4.4.3/apysc/_chart/tick_text_italic_mixin.py
+-rw-r--r--   0 runner    (1001) docker     (127)     1634 2024-05-29 12:24:48.000000 apysc-4.4.3/apysc/_chart/tick_text_max_num_of_decimal_places_mixin.py
+-rw-r--r--   0 runner    (1001) docker     (127)     9647 2024-05-29 12:24:48.000000 apysc-4.4.3/apysc/_chart/vertical_bar_chart.py
+-rw-r--r--   0 runner    (1001) docker     (127)      793 2024-05-29 12:24:48.000000 apysc-4.4.3/apysc/_chart/x_axis_column_name_mixin.py
+-rw-r--r--   0 runner    (1001) docker     (127)     1249 2024-05-29 12:24:48.000000 apysc-4.4.3/apysc/_chart/x_axis_container_mixin.py
+-rw-r--r--   0 runner    (1001) docker     (127)      316 2024-05-29 12:24:48.000000 apysc-4.4.3/apysc/_chart/x_axis_label_position.py
+-rw-r--r--   0 runner    (1001) docker     (127)      939 2024-05-29 12:24:48.000000 apysc-4.4.3/apysc/_chart/x_axis_label_position_mixin.py
+-rw-r--r--   0 runner    (1001) docker     (127)    11482 2024-05-29 12:24:48.000000 apysc-4.4.3/apysc/_chart/x_axis_settings.py
+-rw-r--r--   0 runner    (1001) docker     (127)     1023 2024-05-29 12:24:48.000000 apysc-4.4.3/apysc/_chart/y_axis_column_name_mixin.py
+-rw-r--r--   0 runner    (1001) docker     (127)     1248 2024-05-29 12:24:48.000000 apysc-4.4.3/apysc/_chart/y_axis_container_mixin.py
+-rw-r--r--   0 runner    (1001) docker     (127)      314 2024-05-29 12:24:48.000000 apysc-4.4.3/apysc/_chart/y_axis_label_position.py
+-rw-r--r--   0 runner    (1001) docker     (127)      944 2024-05-29 12:24:48.000000 apysc-4.4.3/apysc/_chart/y_axis_label_position_mixin.py
+-rw-r--r--   0 runner    (1001) docker     (127)    13296 2024-05-29 12:24:48.000000 apysc-4.4.3/apysc/_chart/y_axis_single_column_settings.py
+-rw-r--r--   0 runner    (1001) docker     (127)     1398 2024-05-29 12:24:48.000000 apysc-4.4.3/apysc/_chart/y_max_mixin.py
+-rw-r--r--   0 runner    (1001) docker     (127)     1398 2024-05-29 12:24:48.000000 apysc-4.4.3/apysc/_chart/y_min_mixin.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-29 12:25:09.991790 apysc-4.4.3/apysc/_color/
+-rw-r--r--   0 runner    (1001) docker     (127)        0 2024-05-29 12:24:48.000000 apysc-4.4.3/apysc/_color/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (127)     4857 2024-05-29 12:24:48.000000 apysc-4.4.3/apysc/_color/blue_color_mixin.py
+-rw-r--r--   0 runner    (1001) docker     (127)     6496 2024-05-29 12:24:48.000000 apysc-4.4.3/apysc/_color/color.py
+-rw-r--r--   0 runner    (1001) docker     (127)     2473 2024-05-29 12:24:48.000000 apysc-4.4.3/apysc/_color/color_copy_mixin.py
+-rw-r--r--   0 runner    (1001) docker     (127)     7843 2024-05-29 12:24:48.000000 apysc-4.4.3/apysc/_color/color_util.py
+-rw-r--r--   0 runner    (1001) docker     (127)      477 2024-05-29 12:24:48.000000 apysc-4.4.3/apysc/_color/colorless.py
+-rw-r--r--   0 runner    (1001) docker     (127)    84071 2024-05-29 12:24:48.000000 apysc-4.4.3/apysc/_color/colors.py
+-rw-r--r--   0 runner    (1001) docker     (127)     1164 2024-05-29 12:24:48.000000 apysc-4.4.3/apysc/_color/copy_color_if_default_value_specified_mixin.py
+-rw-r--r--   0 runner    (1001) docker     (127)     4056 2024-05-29 12:24:48.000000 apysc-4.4.3/apysc/_color/from_rgb_mixin.py
+-rw-r--r--   0 runner    (1001) docker     (127)      924 2024-05-29 12:24:48.000000 apysc-4.4.3/apysc/_color/get_colors_members_mixin.py
+-rw-r--r--   0 runner    (1001) docker     (127)     5114 2024-05-29 12:24:48.000000 apysc-4.4.3/apysc/_color/green_color_mixin.py
+-rw-r--r--   0 runner    (1001) docker     (127)     4249 2024-05-29 12:24:48.000000 apysc-4.4.3/apysc/_color/red_color_mixin.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-29 12:25:09.995790 apysc-4.4.3/apysc/_console/
+-rw-r--r--   0 runner    (1001) docker     (127)        0 2024-05-29 12:24:48.000000 apysc-4.4.3/apysc/_console/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (127)     4573 2024-05-29 12:24:48.000000 apysc-4.4.3/apysc/_console/_trace.py
+-rw-r--r--   0 runner    (1001) docker     (127)    32116 2024-05-29 12:24:48.000000 apysc-4.4.3/apysc/_console/assertion.py
+-rw-r--r--   0 runner    (1001) docker     (127)     1004 2024-05-29 12:24:48.000000 apysc-4.4.3/apysc/_console/loggers.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-29 12:25:09.995790 apysc-4.4.3/apysc/_converter/
+-rw-r--r--   0 runner    (1001) docker     (127)        0 2024-05-29 12:24:48.000000 apysc-4.4.3/apysc/_converter/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (127)     2458 2024-05-29 12:24:48.000000 apysc-4.4.3/apysc/_converter/cast.py
+-rw-r--r--   0 runner    (1001) docker     (127)     3431 2024-05-29 12:24:48.000000 apysc-4.4.3/apysc/_converter/to_apysc_val_from_builtin.py
+-rw-r--r--   0 runner    (1001) docker     (127)      698 2024-05-29 12:24:48.000000 apysc-4.4.3/apysc/_converter/to_builtin_val_from_apysc.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-29 12:25:10.011790 apysc-4.4.3/apysc/_display/
+-rw-r--r--   0 runner    (1001) docker     (127)        0 2024-05-29 12:24:48.000000 apysc-4.4.3/apysc/_display/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (127)      523 2024-05-29 12:24:48.000000 apysc-4.4.3/apysc/_display/_document.py
+-rw-r--r--   0 runner    (1001) docker     (127)     1218 2024-05-29 12:24:48.000000 apysc-4.4.3/apysc/_display/add_foreign_object_child_mixin.py
+-rw-r--r--   0 runner    (1001) docker     (127)     1238 2024-05-29 12:24:48.000000 apysc-4.4.3/apysc/_display/add_to_parent_mixin.py
+-rw-r--r--   0 runner    (1001) docker     (127)     2142 2024-05-29 12:24:48.000000 apysc-4.4.3/apysc/_display/any_display_object.py
+-rw-r--r--   0 runner    (1001) docker     (127)     1787 2024-05-29 12:24:48.000000 apysc-4.4.3/apysc/_display/append_fill_alpha_attr_expression_mixin.py
+-rw-r--r--   0 runner    (1001) docker     (127)     1768 2024-05-29 12:24:48.000000 apysc-4.4.3/apysc/_display/append_fill_color_expression_mixin.py
+-rw-r--r--   0 runner    (1001) docker     (127)     1224 2024-05-29 12:24:48.000000 apysc-4.4.3/apysc/_display/append_foreign_object_constructor_expression_mixin.py
+-rw-r--r--   0 runner    (1001) docker     (127)     1778 2024-05-29 12:24:48.000000 apysc-4.4.3/apysc/_display/append_line_alpha_attr_expression_mixin.py
+-rw-r--r--   0 runner    (1001) docker     (127)     1725 2024-05-29 12:24:48.000000 apysc-4.4.3/apysc/_display/append_line_cap_attr_expression_mixin.py
+-rw-r--r--   0 runner    (1001) docker     (127)     1772 2024-05-29 12:24:48.000000 apysc-4.4.3/apysc/_display/append_line_color_attr_expression_mixin.py
+-rw-r--r--   0 runner    (1001) docker     (127)     1791 2024-05-29 12:24:48.000000 apysc-4.4.3/apysc/_display/append_line_joints_attr_expression_mixin.py
+-rw-r--r--   0 runner    (1001) docker     (127)     3056 2024-05-29 12:24:48.000000 apysc-4.4.3/apysc/_display/append_line_point_mixin.py
+-rw-r--r--   0 runner    (1001) docker     (127)     1824 2024-05-29 12:24:48.000000 apysc-4.4.3/apysc/_display/append_line_thickness_attr_expression_mixin.py
+-rw-r--r--   0 runner    (1001) docker     (127)     1657 2024-05-29 12:24:48.000000 apysc-4.4.3/apysc/_display/append_x_attr_expression_mixin.py
+-rw-r--r--   0 runner    (1001) docker     (127)     1655 2024-05-29 12:24:48.000000 apysc-4.4.3/apysc/_display/append_y_attr_expression_mixin.py
+-rw-r--r--   0 runner    (1001) docker     (127)     7031 2024-05-29 12:24:48.000000 apysc-4.4.3/apysc/_display/begin_fill_mixin.py
+-rw-r--r--   0 runner    (1001) docker     (127)    15676 2024-05-29 12:24:48.000000 apysc-4.4.3/apysc/_display/child_mixin.py
+-rw-r--r--   0 runner    (1001) docker     (127)    17462 2024-05-29 12:24:48.000000 apysc-4.4.3/apysc/_display/circle.py
+-rw-r--r--   0 runner    (1001) docker     (127)     1295 2024-05-29 12:24:48.000000 apysc-4.4.3/apysc/_display/css_interface.py
+-rw-r--r--   0 runner    (1001) docker     (127)     6651 2024-05-29 12:24:48.000000 apysc-4.4.3/apysc/_display/css_mixin.py
+-rw-r--r--   0 runner    (1001) docker     (127)      415 2024-05-29 12:24:48.000000 apysc-4.4.3/apysc/_display/css_text_align.py
+-rw-r--r--   0 runner    (1001) docker     (127)      379 2024-05-29 12:24:48.000000 apysc-4.4.3/apysc/_display/css_text_align_last.py
+-rw-r--r--   0 runner    (1001) docker     (127)     5404 2024-05-29 12:24:48.000000 apysc-4.4.3/apysc/_display/cx_mixin.py
+-rw-r--r--   0 runner    (1001) docker     (127)     5454 2024-05-29 12:24:48.000000 apysc-4.4.3/apysc/_display/cy_mixin.py
+-rw-r--r--   0 runner    (1001) docker     (127)     1510 2024-05-29 12:24:48.000000 apysc-4.4.3/apysc/_display/display_object.py
+-rw-r--r--   0 runner    (1001) docker     (127)    17384 2024-05-29 12:24:48.000000 apysc-4.4.3/apysc/_display/ellipse.py
+-rw-r--r--   0 runner    (1001) docker     (127)     5438 2024-05-29 12:24:48.000000 apysc-4.4.3/apysc/_display/ellipse_height_mixin.py
+-rw-r--r--   0 runner    (1001) docker     (127)     5411 2024-05-29 12:24:48.000000 apysc-4.4.3/apysc/_display/ellipse_width_mixin.py
+-rw-r--r--   0 runner    (1001) docker     (127)     6246 2024-05-29 12:24:48.000000 apysc-4.4.3/apysc/_display/fill_alpha_mixin.py
+-rw-r--r--   0 runner    (1001) docker     (127)     6544 2024-05-29 12:24:48.000000 apysc-4.4.3/apysc/_display/fill_color_mixin.py
+-rw-r--r--   0 runner    (1001) docker     (127)     2321 2024-05-29 12:24:48.000000 apysc-4.4.3/apysc/_display/fixed_html_svg_icon_base.py
+-rw-r--r--   0 runner    (1001) docker     (127)     1354 2024-05-29 12:24:48.000000 apysc-4.4.3/apysc/_display/flip_interface_helper.py
+-rw-r--r--   0 runner    (1001) docker     (127)     5692 2024-05-29 12:24:48.000000 apysc-4.4.3/apysc/_display/flip_x_mixin.py
+-rw-r--r--   0 runner    (1001) docker     (127)     5690 2024-05-29 12:24:48.000000 apysc-4.4.3/apysc/_display/flip_y_mixin.py
+-rw-r--r--   0 runner    (1001) docker     (127)     5452 2024-05-29 12:24:48.000000 apysc-4.4.3/apysc/_display/get_bounds_mixin.py
+-rw-r--r--   0 runner    (1001) docker     (127)    49066 2024-05-29 12:24:48.000000 apysc-4.4.3/apysc/_display/graphics.py
+-rw-r--r--   0 runner    (1001) docker     (127)     7012 2024-05-29 12:24:48.000000 apysc-4.4.3/apysc/_display/graphics_base.py
+-rw-r--r--   0 runner    (1001) docker     (127)     4265 2024-05-29 12:24:48.000000 apysc-4.4.3/apysc/_display/graphics_clear_mixin.py
+-rw-r--r--   0 runner    (1001) docker     (127)     7731 2024-05-29 12:24:48.000000 apysc-4.4.3/apysc/_display/graphics_expression.py
+-rw-r--r--   0 runner    (1001) docker     (127)     5533 2024-05-29 12:24:48.000000 apysc-4.4.3/apysc/_display/height_mixin.py
+-rw-r--r--   0 runner    (1001) docker     (127)    15906 2024-05-29 12:24:48.000000 apysc-4.4.3/apysc/_display/line.py
+-rw-r--r--   0 runner    (1001) docker     (127)     6178 2024-05-29 12:24:48.000000 apysc-4.4.3/apysc/_display/line_alpha_mixin.py
+-rw-r--r--   0 runner    (1001) docker     (127)     4752 2024-05-29 12:24:48.000000 apysc-4.4.3/apysc/_display/line_cap_mixin.py
+-rw-r--r--   0 runner    (1001) docker     (127)      597 2024-05-29 12:24:48.000000 apysc-4.4.3/apysc/_display/line_caps.py
+-rw-r--r--   0 runner    (1001) docker     (127)     6753 2024-05-29 12:24:48.000000 apysc-4.4.3/apysc/_display/line_color_mixin.py
+-rw-r--r--   0 runner    (1001) docker     (127)     7036 2024-05-29 12:24:48.000000 apysc-4.4.3/apysc/_display/line_dash_dot_setting.py
+-rw-r--r--   0 runner    (1001) docker     (127)     6757 2024-05-29 12:24:48.000000 apysc-4.4.3/apysc/_display/line_dash_dot_setting_mixin.py
+-rw-r--r--   0 runner    (1001) docker     (127)     5383 2024-05-29 12:24:48.000000 apysc-4.4.3/apysc/_display/line_dash_setting.py
+-rw-r--r--   0 runner    (1001) docker     (127)     6059 2024-05-29 12:24:48.000000 apysc-4.4.3/apysc/_display/line_dash_setting_mixin.py
+-rw-r--r--   0 runner    (1001) docker     (127)     3855 2024-05-29 12:24:48.000000 apysc-4.4.3/apysc/_display/line_dot_setting.py
+-rw-r--r--   0 runner    (1001) docker     (127)     5722 2024-05-29 12:24:48.000000 apysc-4.4.3/apysc/_display/line_dot_setting_mixin.py
+-rw-r--r--   0 runner    (1001) docker     (127)      618 2024-05-29 12:24:48.000000 apysc-4.4.3/apysc/_display/line_joints.py
+-rw-r--r--   0 runner    (1001) docker     (127)     5226 2024-05-29 12:24:48.000000 apysc-4.4.3/apysc/_display/line_joints_mixin.py
+-rw-r--r--   0 runner    (1001) docker     (127)     5652 2024-05-29 12:24:48.000000 apysc-4.4.3/apysc/_display/line_round_dot_setting.py
+-rw-r--r--   0 runner    (1001) docker     (127)     6639 2024-05-29 12:24:48.000000 apysc-4.4.3/apysc/_display/line_round_dot_setting_mixin.py
+-rw-r--r--   0 runner    (1001) docker     (127)    26709 2024-05-29 12:24:48.000000 apysc-4.4.3/apysc/_display/line_style_mixin.py
+-rw-r--r--   0 runner    (1001) docker     (127)     6187 2024-05-29 12:24:48.000000 apysc-4.4.3/apysc/_display/line_thickness_mixin.py
+-rw-r--r--   0 runner    (1001) docker     (127)    12333 2024-05-29 12:24:48.000000 apysc-4.4.3/apysc/_display/multi_line_text.py
+-rw-r--r--   0 runner    (1001) docker     (127)     3736 2024-05-29 12:24:48.000000 apysc-4.4.3/apysc/_display/opacity_css_mixin.py
+-rw-r--r--   0 runner    (1001) docker     (127)     4338 2024-05-29 12:24:48.000000 apysc-4.4.3/apysc/_display/parent_mixin.py
+-rw-r--r--   0 runner    (1001) docker     (127)    18730 2024-05-29 12:24:48.000000 apysc-4.4.3/apysc/_display/path.py
+-rw-r--r--   0 runner    (1001) docker     (127)     5865 2024-05-29 12:24:48.000000 apysc-4.4.3/apysc/_display/points_2d_mixin.py
+-rw-r--r--   0 runner    (1001) docker     (127)       54 2024-05-29 12:24:48.000000 apysc-4.4.3/apysc/_display/points_var_name_mixin.py
+-rw-r--r--   0 runner    (1001) docker     (127)    15565 2024-05-29 12:24:48.000000 apysc-4.4.3/apysc/_display/polygon.py
+-rw-r--r--   0 runner    (1001) docker     (127)     4334 2024-05-29 12:24:48.000000 apysc-4.4.3/apysc/_display/polygon_append_constructor_expression_mixin.py
+-rw-r--r--   0 runner    (1001) docker     (127)      747 2024-05-29 12:24:48.000000 apysc-4.4.3/apysc/_display/polygon_apply_current_points_mixin.py
+-rw-r--r--   0 runner    (1001) docker     (127)     1177 2024-05-29 12:24:48.000000 apysc-4.4.3/apysc/_display/polygon_x1_mixin.py
+-rw-r--r--   0 runner    (1001) docker     (127)     1180 2024-05-29 12:24:48.000000 apysc-4.4.3/apysc/_display/polygon_x2_mixin.py
+-rw-r--r--   0 runner    (1001) docker     (127)     1177 2024-05-29 12:24:48.000000 apysc-4.4.3/apysc/_display/polygon_x3_mixin.py
+-rw-r--r--   0 runner    (1001) docker     (127)     1177 2024-05-29 12:24:48.000000 apysc-4.4.3/apysc/_display/polygon_y1_mixin.py
+-rw-r--r--   0 runner    (1001) docker     (127)     1180 2024-05-29 12:24:48.000000 apysc-4.4.3/apysc/_display/polygon_y2_mixin.py
+-rw-r--r--   0 runner    (1001) docker     (127)     1126 2024-05-29 12:24:48.000000 apysc-4.4.3/apysc/_display/polygon_y3_mixin.py
+-rw-r--r--   0 runner    (1001) docker     (127)    17466 2024-05-29 12:24:48.000000 apysc-4.4.3/apysc/_display/polyline.py
+-rw-r--r--   0 runner    (1001) docker     (127)     5272 2024-05-29 12:24:48.000000 apysc-4.4.3/apysc/_display/radius_mixin.py
+-rw-r--r--   0 runner    (1001) docker     (127)    19494 2024-05-29 12:24:48.000000 apysc-4.4.3/apysc/_display/rectangle.py
+-rw-r--r--   0 runner    (1001) docker     (127)     6400 2024-05-29 12:24:48.000000 apysc-4.4.3/apysc/_display/rotation_around_center_mixin.py
+-rw-r--r--   0 runner    (1001) docker     (127)     9157 2024-05-29 12:24:48.000000 apysc-4.4.3/apysc/_display/rotation_around_point_mixin.py
+-rw-r--r--   0 runner    (1001) docker     (127)     1108 2024-05-29 12:24:48.000000 apysc-4.4.3/apysc/_display/rotation_interface_helper.py
+-rw-r--r--   0 runner    (1001) docker     (127)     3799 2024-05-29 12:24:48.000000 apysc-4.4.3/apysc/_display/scale_interface_helper.py
+-rw-r--r--   0 runner    (1001) docker     (127)     6769 2024-05-29 12:24:48.000000 apysc-4.4.3/apysc/_display/scale_x_from_center_mixin.py
+-rw-r--r--   0 runner    (1001) docker     (127)     7293 2024-05-29 12:24:48.000000 apysc-4.4.3/apysc/_display/scale_x_from_point_mixin.py
+-rw-r--r--   0 runner    (1001) docker     (127)     6764 2024-05-29 12:24:48.000000 apysc-4.4.3/apysc/_display/scale_y_from_center_mixin.py
+-rw-r--r--   0 runner    (1001) docker     (127)     6988 2024-05-29 12:24:48.000000 apysc-4.4.3/apysc/_display/scale_y_from_point_mixin.py
+-rw-r--r--   0 runner    (1001) docker     (127)      650 2024-05-29 12:24:48.000000 apysc-4.4.3/apysc/_display/set_lower_scale_limit_mixin.py
+-rw-r--r--   0 runner    (1001) docker     (127)      563 2024-05-29 12:24:48.000000 apysc-4.4.3/apysc/_display/set_overflow_visible_setting_mixin.py
+-rw-r--r--   0 runner    (1001) docker     (127)      390 2024-05-29 12:24:48.000000 apysc-4.4.3/apysc/_display/set_x_and_y_with_minimum_point_interface_base.py
+-rw-r--r--   0 runner    (1001) docker     (127)     5479 2024-05-29 12:24:48.000000 apysc-4.4.3/apysc/_display/skew_x_mixin.py
+-rw-r--r--   0 runner    (1001) docker     (127)     5478 2024-05-29 12:24:48.000000 apysc-4.4.3/apysc/_display/skew_y_mixin.py
+-rw-r--r--   0 runner    (1001) docker     (127)     7453 2024-05-29 12:24:48.000000 apysc-4.4.3/apysc/_display/sprite.py
+-rw-r--r--   0 runner    (1001) docker     (127)    12655 2024-05-29 12:24:48.000000 apysc-4.4.3/apysc/_display/stage.py
+-rw-r--r--   0 runner    (1001) docker     (127)     3721 2024-05-29 12:24:48.000000 apysc-4.4.3/apysc/_display/svg_foreign_object_child.py
+-rw-r--r--   0 runner    (1001) docker     (127)     1447 2024-05-29 12:24:48.000000 apysc-4.4.3/apysc/_display/svg_foreign_object_child_mixin.py
+-rw-r--r--   0 runner    (1001) docker     (127)     1249 2024-05-29 12:24:48.000000 apysc-4.4.3/apysc/_display/svg_foreign_object_initialize_width_mixin.py
+-rw-r--r--   0 runner    (1001) docker     (127)     1478 2024-05-29 12:24:48.000000 apysc-4.4.3/apysc/_display/svg_foreign_object_text_mixin.py
+-rw-r--r--   0 runner    (1001) docker     (127)     5737 2024-05-29 12:24:48.000000 apysc-4.4.3/apysc/_display/svg_icon.py
+-rw-r--r--   0 runner    (1001) docker     (127)    23384 2024-05-29 12:24:48.000000 apysc-4.4.3/apysc/_display/svg_text.py
+-rw-r--r--   0 runner    (1001) docker     (127)     2705 2024-05-29 12:24:48.000000 apysc-4.4.3/apysc/_display/svg_text_align_mixin.py
+-rw-r--r--   0 runner    (1001) docker     (127)     2980 2024-05-29 12:24:48.000000 apysc-4.4.3/apysc/_display/svg_text_bold_mixin.py
+-rw-r--r--   0 runner    (1001) docker     (127)     2993 2024-05-29 12:24:48.000000 apysc-4.4.3/apysc/_display/svg_text_delta_x_mixin.py
+-rw-r--r--   0 runner    (1001) docker     (127)     2993 2024-05-29 12:24:48.000000 apysc-4.4.3/apysc/_display/svg_text_delta_y_mixin.py
+-rw-r--r--   0 runner    (1001) docker     (127)     2873 2024-05-29 12:24:48.000000 apysc-4.4.3/apysc/_display/svg_text_font_family_mixin.py
+-rw-r--r--   0 runner    (1001) docker     (127)     3378 2024-05-29 12:24:48.000000 apysc-4.4.3/apysc/_display/svg_text_font_size_mixin.py
+-rw-r--r--   0 runner    (1001) docker     (127)     3008 2024-05-29 12:24:48.000000 apysc-4.4.3/apysc/_display/svg_text_italic_mixin.py
+-rw-r--r--   0 runner    (1001) docker     (127)     2916 2024-05-29 12:24:48.000000 apysc-4.4.3/apysc/_display/svg_text_leading_mixin.py
+-rw-r--r--   0 runner    (1001) docker     (127)      907 2024-05-29 12:24:48.000000 apysc-4.4.3/apysc/_display/svg_text_set_align_mixin.py
+-rw-r--r--   0 runner    (1001) docker     (127)     1555 2024-05-29 12:24:48.000000 apysc-4.4.3/apysc/_display/svg_text_set_bold_mixin.py
+-rw-r--r--   0 runner    (1001) docker     (127)     1372 2024-05-29 12:24:48.000000 apysc-4.4.3/apysc/_display/svg_text_set_delta_x_mixin.py
+-rw-r--r--   0 runner    (1001) docker     (127)     1372 2024-05-29 12:24:48.000000 apysc-4.4.3/apysc/_display/svg_text_set_delta_y_mixin.py
+-rw-r--r--   0 runner    (1001) docker     (127)     1747 2024-05-29 12:24:48.000000 apysc-4.4.3/apysc/_display/svg_text_set_font_family_mixin.py
+-rw-r--r--   0 runner    (1001) docker     (127)     1574 2024-05-29 12:24:48.000000 apysc-4.4.3/apysc/_display/svg_text_set_font_size_value_mixin.py
+-rw-r--r--   0 runner    (1001) docker     (127)     1634 2024-05-29 12:24:48.000000 apysc-4.4.3/apysc/_display/svg_text_set_italic_mixin.py
+-rw-r--r--   0 runner    (1001) docker     (127)     1404 2024-05-29 12:24:48.000000 apysc-4.4.3/apysc/_display/svg_text_set_leading_mixin.py
+-rw-r--r--   0 runner    (1001) docker     (127)     1486 2024-05-29 12:24:48.000000 apysc-4.4.3/apysc/_display/svg_text_set_text_value_mixin.py
+-rw-r--r--   0 runner    (1001) docker     (127)     1108 2024-05-29 12:24:48.000000 apysc-4.4.3/apysc/_display/svg_text_singleton_for_text_span.py
+-rw-r--r--   0 runner    (1001) docker     (127)     1062 2024-05-29 12:24:48.000000 apysc-4.4.3/apysc/_display/svg_text_skip_fill_alpha_exp_appending_mixin.py
+-rw-r--r--   0 runner    (1001) docker     (127)     1005 2024-05-29 12:24:48.000000 apysc-4.4.3/apysc/_display/svg_text_skip_fill_color_exp_appending_mixin.py
+-rw-r--r--   0 runner    (1001) docker     (127)     1062 2024-05-29 12:24:48.000000 apysc-4.4.3/apysc/_display/svg_text_skip_line_alpha_exp_appending_mixin.py
+-rw-r--r--   0 runner    (1001) docker     (127)     1005 2024-05-29 12:24:48.000000 apysc-4.4.3/apysc/_display/svg_text_skip_line_color_exp_appending_mixin.py
+-rw-r--r--   0 runner    (1001) docker     (127)     1090 2024-05-29 12:24:48.000000 apysc-4.4.3/apysc/_display/svg_text_skip_line_thickness_exp_appending_mixin.py
+-rw-r--r--   0 runner    (1001) docker     (127)    16986 2024-05-29 12:24:48.000000 apysc-4.4.3/apysc/_display/svg_text_span.py
+-rw-r--r--   0 runner    (1001) docker     (127)     3564 2024-05-29 12:24:48.000000 apysc-4.4.3/apysc/_display/svg_text_text_mixin.py
+-rw-r--r--   0 runner    (1001) docker     (127)     3222 2024-05-29 12:24:48.000000 apysc-4.4.3/apysc/_display/text_align_css_mixin.py
+-rw-r--r--   0 runner    (1001) docker     (127)     3493 2024-05-29 12:24:48.000000 apysc-4.4.3/apysc/_display/text_align_last_css_mixin.py
+-rw-r--r--   0 runner    (1001) docker     (127)     3885 2024-05-29 12:24:48.000000 apysc-4.4.3/apysc/_display/text_bold_css_mixin.py
+-rw-r--r--   0 runner    (1001) docker     (127)     3951 2024-05-29 12:24:48.000000 apysc-4.4.3/apysc/_display/text_decoration_underline_css_mixin.py
+-rw-r--r--   0 runner    (1001) docker     (127)     3905 2024-05-29 12:24:48.000000 apysc-4.4.3/apysc/_display/text_fill_color_css_mixin.py
+-rw-r--r--   0 runner    (1001) docker     (127)     3463 2024-05-29 12:24:48.000000 apysc-4.4.3/apysc/_display/text_font_size_css_mixin.py
+-rw-r--r--   0 runner    (1001) docker     (127)     4005 2024-05-29 12:24:48.000000 apysc-4.4.3/apysc/_display/text_italic_css_mixin.py
+-rw-r--r--   0 runner    (1001) docker     (127)     3638 2024-05-29 12:24:48.000000 apysc-4.4.3/apysc/_display/text_line_height_css_mixin.py
+-rw-r--r--   0 runner    (1001) docker     (127)    17673 2024-05-29 12:24:48.000000 apysc-4.4.3/apysc/_display/triangle.py
+-rw-r--r--   0 runner    (1001) docker     (127)     4763 2024-05-29 12:24:48.000000 apysc-4.4.3/apysc/_display/visible_mixin.py
+-rw-r--r--   0 runner    (1001) docker     (127)     8204 2024-05-29 12:24:48.000000 apysc-4.4.3/apysc/_display/width_and_height_mixin_for_ellipse.py
+-rw-r--r--   0 runner    (1001) docker     (127)     5453 2024-05-29 12:24:48.000000 apysc-4.4.3/apysc/_display/width_mixin.py
+-rw-r--r--   0 runner    (1001) docker     (127)     1083 2024-05-29 12:24:48.000000 apysc-4.4.3/apysc/_display/x_interface.py
+-rw-r--r--   0 runner    (1001) docker     (127)     5661 2024-05-29 12:24:48.000000 apysc-4.4.3/apysc/_display/x_mixin.py
+-rw-r--r--   0 runner    (1001) docker     (127)     1081 2024-05-29 12:24:48.000000 apysc-4.4.3/apysc/_display/y_interface.py
+-rw-r--r--   0 runner    (1001) docker     (127)     5652 2024-05-29 12:24:48.000000 apysc-4.4.3/apysc/_display/y_mixin.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-29 12:25:10.015790 apysc-4.4.3/apysc/_event/
+-rw-r--r--   0 runner    (1001) docker     (127)        0 2024-05-29 12:24:48.000000 apysc-4.4.3/apysc/_event/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (127)     3255 2024-05-29 12:24:48.000000 apysc-4.4.3/apysc/_event/animation_event.py
+-rw-r--r--   0 runner    (1001) docker     (127)     6521 2024-05-29 12:24:48.000000 apysc-4.4.3/apysc/_event/click_mixin.py
+-rw-r--r--   0 runner    (1001) docker     (127)    14746 2024-05-29 12:24:48.000000 apysc-4.4.3/apysc/_event/custom_event_mixin.py
+-rw-r--r--   0 runner    (1001) docker     (127)      217 2024-05-29 12:24:48.000000 apysc-4.4.3/apysc/_event/custom_event_type.py
+-rw-r--r--   0 runner    (1001) docker     (127)     3394 2024-05-29 12:24:48.000000 apysc-4.4.3/apysc/_event/document_mouse_wheel_func.py
+-rw-r--r--   0 runner    (1001) docker     (127)     6450 2024-05-29 12:24:48.000000 apysc-4.4.3/apysc/_event/double_click_mixin.py
+-rw-r--r--   0 runner    (1001) docker     (127)     1099 2024-05-29 12:24:48.000000 apysc-4.4.3/apysc/_event/enter_frame_event.py
+-rw-r--r--   0 runner    (1001) docker     (127)    15687 2024-05-29 12:24:48.000000 apysc-4.4.3/apysc/_event/enter_frame_mixin.py
+-rw-r--r--   0 runner    (1001) docker     (127)     5617 2024-05-29 12:24:48.000000 apysc-4.4.3/apysc/_event/event.py
+-rw-r--r--   0 runner    (1001) docker     (127)     6331 2024-05-29 12:24:48.000000 apysc-4.4.3/apysc/_event/handler.py
+-rw-r--r--   0 runner    (1001) docker     (127)     9989 2024-05-29 12:24:48.000000 apysc-4.4.3/apysc/_event/handler_circular_calling_util.py
+-rw-r--r--   0 runner    (1001) docker     (127)     6870 2024-05-29 12:24:48.000000 apysc-4.4.3/apysc/_event/mouse_down_mixin.py
+-rw-r--r--   0 runner    (1001) docker     (127)    10068 2024-05-29 12:24:48.000000 apysc-4.4.3/apysc/_event/mouse_event.py
+-rw-r--r--   0 runner    (1001) docker     (127)     1284 2024-05-29 12:24:48.000000 apysc-4.4.3/apysc/_event/mouse_event_binding_expression_mixin.py
+-rw-r--r--   0 runner    (1001) docker     (127)      744 2024-05-29 12:24:48.000000 apysc-4.4.3/apysc/_event/mouse_event_mixins.py
+-rw-r--r--   0 runner    (1001) docker     (127)      371 2024-05-29 12:24:48.000000 apysc-4.4.3/apysc/_event/mouse_event_type.py
+-rw-r--r--   0 runner    (1001) docker     (127)     2964 2024-05-29 12:24:48.000000 apysc-4.4.3/apysc/_event/mouse_event_unbinding_mixin.py
+-rw-r--r--   0 runner    (1001) docker     (127)     7056 2024-05-29 12:24:48.000000 apysc-4.4.3/apysc/_event/mouse_move_mixin.py
+-rw-r--r--   0 runner    (1001) docker     (127)     6824 2024-05-29 12:24:48.000000 apysc-4.4.3/apysc/_event/mouse_out_mixin.py
+-rw-r--r--   0 runner    (1001) docker     (127)     6852 2024-05-29 12:24:48.000000 apysc-4.4.3/apysc/_event/mouse_over_mixin.py
+-rw-r--r--   0 runner    (1001) docker     (127)     6782 2024-05-29 12:24:48.000000 apysc-4.4.3/apysc/_event/mouse_up_mixin.py
+-rw-r--r--   0 runner    (1001) docker     (127)     1550 2024-05-29 12:24:48.000000 apysc-4.4.3/apysc/_event/prevent_default_mixin.py
+-rw-r--r--   0 runner    (1001) docker     (127)     1826 2024-05-29 12:24:48.000000 apysc-4.4.3/apysc/_event/set_handler_data_mixin.py
+-rw-r--r--   0 runner    (1001) docker     (127)     1453 2024-05-29 12:24:48.000000 apysc-4.4.3/apysc/_event/stop_propagation_mixin.py
+-rw-r--r--   0 runner    (1001) docker     (127)     4218 2024-05-29 12:24:48.000000 apysc-4.4.3/apysc/_event/timer_event.py
+-rw-r--r--   0 runner    (1001) docker     (127)     2853 2024-05-29 12:24:48.000000 apysc-4.4.3/apysc/_event/wheel_event.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-29 12:25:10.015790 apysc-4.4.3/apysc/_expression/
+-rw-r--r--   0 runner    (1001) docker     (127)        0 2024-05-29 12:24:48.000000 apysc-4.4.3/apysc/_expression/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (127)     6871 2024-05-29 12:24:48.000000 apysc-4.4.3/apysc/_expression/event_handler_scope.py
+-rw-r--r--   0 runner    (1001) docker     (127)    17851 2024-05-29 12:24:48.000000 apysc-4.4.3/apysc/_expression/expression_data_util.py
+-rw-r--r--   0 runner    (1001) docker     (127)     4794 2024-05-29 12:24:48.000000 apysc-4.4.3/apysc/_expression/expression_variables_util.py
+-rw-r--r--   0 runner    (1001) docker     (127)      358 2024-05-29 12:24:48.000000 apysc-4.4.3/apysc/_expression/get_last_scope_interface.py
+-rw-r--r--   0 runner    (1001) docker     (127)     3812 2024-05-29 12:24:48.000000 apysc-4.4.3/apysc/_expression/indent_num.py
+-rw-r--r--   0 runner    (1001) docker     (127)     1996 2024-05-29 12:24:48.000000 apysc-4.4.3/apysc/_expression/js_functions.py
+-rw-r--r--   0 runner    (1001) docker     (127)     1936 2024-05-29 12:24:48.000000 apysc-4.4.3/apysc/_expression/last_scope.py
+-rw-r--r--   0 runner    (1001) docker     (127)     2617 2024-05-29 12:24:48.000000 apysc-4.4.3/apysc/_expression/var_names.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-29 12:25:10.015790 apysc-4.4.3/apysc/_file/
+-rw-r--r--   0 runner    (1001) docker     (127)        0 2024-05-29 12:24:48.000000 apysc-4.4.3/apysc/_file/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (127)     8021 2024-05-29 12:24:48.000000 apysc-4.4.3/apysc/_file/file_util.py
+-rw-r--r--   0 runner    (1001) docker     (127)     4475 2024-05-29 12:24:48.000000 apysc-4.4.3/apysc/_file/module_util.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-29 12:25:10.019790 apysc-4.4.3/apysc/_geom/
+-rw-r--r--   0 runner    (1001) docker     (127)        0 2024-05-29 12:24:48.000000 apysc-4.4.3/apysc/_geom/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (127)    10201 2024-05-29 12:24:48.000000 apysc-4.4.3/apysc/_geom/path_bezier_2d.py
+-rw-r--r--   0 runner    (1001) docker     (127)     7960 2024-05-29 12:24:48.000000 apysc-4.4.3/apysc/_geom/path_bezier_2d_continual.py
+-rw-r--r--   0 runner    (1001) docker     (127)    13379 2024-05-29 12:24:48.000000 apysc-4.4.3/apysc/_geom/path_bezier_3d.py
+-rw-r--r--   0 runner    (1001) docker     (127)    11011 2024-05-29 12:24:48.000000 apysc-4.4.3/apysc/_geom/path_bezier_3d_continual.py
+-rw-r--r--   0 runner    (1001) docker     (127)     2928 2024-05-29 12:24:48.000000 apysc-4.4.3/apysc/_geom/path_close.py
+-rw-r--r--   0 runner    (1001) docker     (127)     4294 2024-05-29 12:24:48.000000 apysc-4.4.3/apysc/_geom/path_control_x1_mixin.py
+-rw-r--r--   0 runner    (1001) docker     (127)     4298 2024-05-29 12:24:48.000000 apysc-4.4.3/apysc/_geom/path_control_x2_mixin.py
+-rw-r--r--   0 runner    (1001) docker     (127)     4018 2024-05-29 12:24:48.000000 apysc-4.4.3/apysc/_geom/path_control_x_mixin.py
+-rw-r--r--   0 runner    (1001) docker     (127)     4285 2024-05-29 12:24:48.000000 apysc-4.4.3/apysc/_geom/path_control_y1_mixin.py
+-rw-r--r--   0 runner    (1001) docker     (127)     4293 2024-05-29 12:24:48.000000 apysc-4.4.3/apysc/_geom/path_control_y2_mixin.py
+-rw-r--r--   0 runner    (1001) docker     (127)     4080 2024-05-29 12:24:48.000000 apysc-4.4.3/apysc/_geom/path_control_y_mixin.py
+-rw-r--r--   0 runner    (1001) docker     (127)      972 2024-05-29 12:24:48.000000 apysc-4.4.3/apysc/_geom/path_data.py
+-rw-r--r--   0 runner    (1001) docker     (127)     2572 2024-05-29 12:24:48.000000 apysc-4.4.3/apysc/_geom/path_data_base.py
+-rw-r--r--   0 runner    (1001) docker     (127)      874 2024-05-29 12:24:48.000000 apysc-4.4.3/apysc/_geom/path_data_util.py
+-rw-r--r--   0 runner    (1001) docker     (127)     3984 2024-05-29 12:24:48.000000 apysc-4.4.3/apysc/_geom/path_dest_x_mixin.py
+-rw-r--r--   0 runner    (1001) docker     (127)     3968 2024-05-29 12:24:48.000000 apysc-4.4.3/apysc/_geom/path_dest_y_mixin.py
+-rw-r--r--   0 runner    (1001) docker     (127)     6540 2024-05-29 12:24:48.000000 apysc-4.4.3/apysc/_geom/path_horizontal.py
+-rw-r--r--   0 runner    (1001) docker     (127)      366 2024-05-29 12:24:48.000000 apysc-4.4.3/apysc/_geom/path_label.py
+-rw-r--r--   0 runner    (1001) docker     (127)     7385 2024-05-29 12:24:48.000000 apysc-4.4.3/apysc/_geom/path_line_to.py
+-rw-r--r--   0 runner    (1001) docker     (127)     7161 2024-05-29 12:24:48.000000 apysc-4.4.3/apysc/_geom/path_move_to.py
+-rw-r--r--   0 runner    (1001) docker     (127)     6482 2024-05-29 12:24:48.000000 apysc-4.4.3/apysc/_geom/path_vertical.py
+-rw-r--r--   0 runner    (1001) docker     (127)     3662 2024-05-29 12:24:48.000000 apysc-4.4.3/apysc/_geom/path_x_mixin.py
+-rw-r--r--   0 runner    (1001) docker     (127)     3655 2024-05-29 12:24:48.000000 apysc-4.4.3/apysc/_geom/path_y_mixin.py
+-rw-r--r--   0 runner    (1001) docker     (127)    12328 2024-05-29 12:24:48.000000 apysc-4.4.3/apysc/_geom/point2d.py
+-rw-r--r--   0 runner    (1001) docker     (127)     4230 2024-05-29 12:24:48.000000 apysc-4.4.3/apysc/_geom/rectangle_geom.py
+-rw-r--r--   0 runner    (1001) docker     (127)      558 2024-05-29 12:24:48.000000 apysc-4.4.3/apysc/_geom/rectangle_geom_bottom_y_mixin.py
+-rw-r--r--   0 runner    (1001) docker     (127)      558 2024-05-29 12:24:48.000000 apysc-4.4.3/apysc/_geom/rectangle_geom_center_x_mixin.py
+-rw-r--r--   0 runner    (1001) docker     (127)      558 2024-05-29 12:24:48.000000 apysc-4.4.3/apysc/_geom/rectangle_geom_center_y_mixin.py
+-rw-r--r--   0 runner    (1001) docker     (127)      524 2024-05-29 12:24:48.000000 apysc-4.4.3/apysc/_geom/rectangle_geom_height_mixin.py
+-rw-r--r--   0 runner    (1001) docker     (127)      542 2024-05-29 12:24:48.000000 apysc-4.4.3/apysc/_geom/rectangle_geom_left_x_mixin.py
+-rw-r--r--   0 runner    (1001) docker     (127)      550 2024-05-29 12:24:48.000000 apysc-4.4.3/apysc/_geom/rectangle_geom_right_x_mixin.py
+-rw-r--r--   0 runner    (1001) docker     (127)      534 2024-05-29 12:24:48.000000 apysc-4.4.3/apysc/_geom/rectangle_geom_top_y_mixin.py
+-rw-r--r--   0 runner    (1001) docker     (127)      516 2024-05-29 12:24:48.000000 apysc-4.4.3/apysc/_geom/rectangle_geom_width_mixin.py
+-rw-r--r--   0 runner    (1001) docker     (127)     3392 2024-05-29 12:24:48.000000 apysc-4.4.3/apysc/_geom/relative_mixin.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-29 12:25:10.023790 apysc-4.4.3/apysc/_html/
+-rw-r--r--   0 runner    (1001) docker     (127)        0 2024-05-29 12:24:48.000000 apysc-4.4.3/apysc/_html/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (127)    14617 2024-05-29 12:24:48.000000 apysc-4.4.3/apysc/_html/debug_mode.py
+-rw-r--r--   0 runner    (1001) docker     (127)    20660 2024-05-29 12:24:48.000000 apysc-4.4.3/apysc/_html/exporter.py
+-rw-r--r--   0 runner    (1001) docker     (127)      129 2024-05-29 12:24:48.000000 apysc-4.4.3/apysc/_html/html_const.py
+-rw-r--r--   0 runner    (1001) docker     (127)     8721 2024-05-29 12:24:48.000000 apysc-4.4.3/apysc/_html/html_util.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-29 12:25:10.023790 apysc-4.4.3/apysc/_jslib/
+-rw-r--r--   0 runner    (1001) docker     (127)        0 2024-05-29 12:24:48.000000 apysc-4.4.3/apysc/_jslib/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (127)    70264 2024-05-29 12:24:48.000000 apysc-4.4.3/apysc/_jslib/jquery-3.7.1.slim.min.js
+-rw-r--r--   0 runner    (1001) docker     (127)     2752 2024-05-29 12:24:48.000000 apysc-4.4.3/apysc/_jslib/jquery.mousewheel-3.1.13.min.js
+-rw-r--r--   0 runner    (1001) docker     (127)     5134 2024-05-29 12:24:48.000000 apysc-4.4.3/apysc/_jslib/jslib_util.py
+-rw-r--r--   0 runner    (1001) docker     (127)    78572 2024-05-29 12:24:48.000000 apysc-4.4.3/apysc/_jslib/svg-3.1.2.min.js
+-rw-r--r--   0 runner    (1001) docker     (127)    19431 2024-05-29 12:24:48.000000 apysc-4.4.3/apysc/_jslib/underscore-1.12.0.min.js
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-29 12:25:10.023790 apysc-4.4.3/apysc/_jupyter/
+-rw-r--r--   0 runner    (1001) docker     (127)        0 2024-05-29 12:24:48.000000 apysc-4.4.3/apysc/_jupyter/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (127)     3824 2024-05-29 12:24:48.000000 apysc-4.4.3/apysc/_jupyter/jupyter_util.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-29 12:25:10.023790 apysc-4.4.3/apysc/_lint_and_doc/
+-rw-r--r--   0 runner    (1001) docker     (127)        0 2024-05-29 12:24:48.000000 apysc-4.4.3/apysc/_lint_and_doc/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (127)    17625 2024-05-29 12:24:48.000000 apysc-4.4.3/apysc/_lint_and_doc/add_doc_translation_mapping_blank_data.py
+-rw-r--r--   0 runner    (1001) docker     (127)     1265 2024-05-29 12:24:48.000000 apysc-4.4.3/apysc/_lint_and_doc/conf_common.py
+-rw-r--r--   0 runner    (1001) docker     (127)    10413 2024-05-29 12:24:48.000000 apysc-4.4.3/apysc/_lint_and_doc/docs_keyword_link_mapping.py
+-rw-r--r--   0 runner    (1001) docker     (127)      861 2024-05-29 12:24:48.000000 apysc-4.4.3/apysc/_lint_and_doc/docs_lang.py
+-rw-r--r--   0 runner    (1001) docker     (127)     7966 2024-05-29 12:24:48.000000 apysc-4.4.3/apysc/_lint_and_doc/docs_toctree_util.py
+-rw-r--r--   0 runner    (1001) docker     (127)    17282 2024-05-29 12:24:48.000000 apysc-4.4.3/apysc/_lint_and_doc/docs_translation_converter.py
+-rw-r--r--   0 runner    (1001) docker     (127)    13722 2024-05-29 12:24:48.000000 apysc-4.4.3/apysc/_lint_and_doc/docstring_to_markdown_converter.py
+-rw-r--r--   0 runner    (1001) docker     (127)    51969 2024-05-29 12:24:48.000000 apysc-4.4.3/apysc/_lint_and_doc/docstring_util.py
+-rw-r--r--   0 runner    (1001) docker     (127)     7636 2024-05-29 12:24:48.000000 apysc-4.4.3/apysc/_lint_and_doc/document_text_split_util.py
+-rw-r--r--   0 runner    (1001) docker     (127)     1805 2024-05-29 12:24:48.000000 apysc-4.4.3/apysc/_lint_and_doc/document_util.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-29 12:25:10.023790 apysc-4.4.3/apysc/_lint_and_doc/fixed_translation_mapping/
+-rw-r--r--   0 runner    (1001) docker     (127)        0 2024-05-29 12:24:48.000000 apysc-4.4.3/apysc/_lint_and_doc/fixed_translation_mapping/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (127)     5760 2024-05-29 12:24:48.000000 apysc-4.4.3/apysc/_lint_and_doc/fixed_translation_mapping/data_model.py
+-rw-r--r--   0 runner    (1001) docker     (127)   249077 2024-05-29 12:24:48.000000 apysc-4.4.3/apysc/_lint_and_doc/fixed_translation_mapping/jp.py
+-rw-r--r--   0 runner    (1001) docker     (127)     9404 2024-05-29 12:24:48.000000 apysc-4.4.3/apysc/_lint_and_doc/lint_and_doc_hash_util.py
+-rw-r--r--   0 runner    (1001) docker     (127)    11174 2024-05-29 12:24:48.000000 apysc-4.4.3/apysc/_lint_and_doc/translation_mapping_utils.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-29 12:25:10.027790 apysc-4.4.3/apysc/_loop/
+-rw-r--r--   0 runner    (1001) docker     (127)        0 2024-05-29 12:24:48.000000 apysc-4.4.3/apysc/_loop/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (127)     2023 2024-05-29 12:24:48.000000 apysc-4.4.3/apysc/_loop/_continue.py
+-rw-r--r--   0 runner    (1001) docker     (127)     4121 2024-05-29 12:24:48.000000 apysc-4.4.3/apysc/_loop/_range.py
+-rw-r--r--   0 runner    (1001) docker     (127)     6079 2024-05-29 12:24:48.000000 apysc-4.4.3/apysc/_loop/for_array_indices.py
+-rw-r--r--   0 runner    (1001) docker     (127)     6913 2024-05-29 12:24:48.000000 apysc-4.4.3/apysc/_loop/for_array_indices_and_values.py
+-rw-r--r--   0 runner    (1001) docker     (127)     6128 2024-05-29 12:24:48.000000 apysc-4.4.3/apysc/_loop/for_array_values.py
+-rw-r--r--   0 runner    (1001) docker     (127)     6156 2024-05-29 12:24:48.000000 apysc-4.4.3/apysc/_loop/for_dict_keys.py
+-rw-r--r--   0 runner    (1001) docker     (127)     7806 2024-05-29 12:24:48.000000 apysc-4.4.3/apysc/_loop/for_dict_keys_and_values.py
+-rw-r--r--   0 runner    (1001) docker     (127)     6732 2024-05-29 12:24:48.000000 apysc-4.4.3/apysc/_loop/for_dict_values.py
+-rw-r--r--   0 runner    (1001) docker     (127)     1551 2024-05-29 12:24:48.000000 apysc-4.4.3/apysc/_loop/for_loop_exit_mixin.py
+-rw-r--r--   0 runner    (1001) docker     (127)      486 2024-05-29 12:24:48.000000 apysc-4.4.3/apysc/_loop/initialize_with_base_value_interface.py
+-rw-r--r--   0 runner    (1001) docker     (127)     1799 2024-05-29 12:24:48.000000 apysc-4.4.3/apysc/_loop/loop_count.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-29 12:25:10.027790 apysc-4.4.3/apysc/_mask/
+-rw-r--r--   0 runner    (1001) docker     (127)        0 2024-05-29 12:24:48.000000 apysc-4.4.3/apysc/_mask/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (127)     1644 2024-05-29 12:24:48.000000 apysc-4.4.3/apysc/_mask/mask.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-29 12:25:10.027790 apysc-4.4.3/apysc/_material_design/
+-rw-r--r--   0 runner    (1001) docker     (127)        0 2024-05-29 12:24:48.000000 apysc-4.4.3/apysc/_material_design/__init__.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-29 12:25:10.155791 apysc-4.4.3/apysc/_material_design/icon/
+-rw-r--r--   0 runner    (1001) docker     (127)        0 2024-05-29 12:24:48.000000 apysc-4.4.3/apysc/_material_design/icon/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (127)     1294 2024-05-29 12:24:48.000000 apysc-4.4.3/apysc/_material_design/icon/material_10k_icon.py
+-rw-r--r--   0 runner    (1001) docker     (127)     1189 2024-05-29 12:24:48.000000 apysc-4.4.3/apysc/_material_design/icon/material_1k_icon.py
+-rw-r--r--   0 runner    (1001) docker     (127)     1253 2024-05-29 12:24:48.000000 apysc-4.4.3/apysc/_material_design/icon/material_1k_plus_icon.py
+-rw-r--r--   0 runner    (1001) docker     (127)     1253 2024-05-29 12:24:48.000000 apysc-4.4.3/apysc/_material_design/icon/material_2k_icon.py
+-rw-r--r--   0 runner    (1001) docker     (127)     1320 2024-05-29 12:24:48.000000 apysc-4.4.3/apysc/_material_design/icon/material_2k_plus_icon.py
+-rw-r--r--   0 runner    (1001) docker     (127)     2513 2024-05-29 12:24:48.000000 apysc-4.4.3/apysc/_material_design/icon/material_3d_rotation_icon.py
+-rw-r--r--   0 runner    (1001) docker     (127)     2493 2024-05-29 12:24:48.000000 apysc-4.4.3/apysc/_material_design/icon/material_3d_rotation_outlined_icon.py
+-rw-r--r--   0 runner    (1001) docker     (127)     1235 2024-05-29 12:24:48.000000 apysc-4.4.3/apysc/_material_design/icon/material_3k_icon.py
+-rw-r--r--   0 runner    (1001) docker     (127)     1296 2024-05-29 12:24:48.000000 apysc-4.4.3/apysc/_material_design/icon/material_3k_plus_icon.py
+-rw-r--r--   0 runner    (1001) docker     (127)     1213 2024-05-29 12:24:48.000000 apysc-4.4.3/apysc/_material_design/icon/material_4k_icon.py
+-rw-r--r--   0 runner    (1001) docker     (127)     1237 2024-05-29 12:24:48.000000 apysc-4.4.3/apysc/_material_design/icon/material_4k_outlined_icon.py
+-rw-r--r--   0 runner    (1001) docker     (127)     1274 2024-05-29 12:24:48.000000 apysc-4.4.3/apysc/_material_design/icon/material_4k_plus_icon.py
+-rw-r--r--   0 runner    (1001) docker     (127)     1254 2024-05-29 12:24:48.000000 apysc-4.4.3/apysc/_material_design/icon/material_5g_icon.py
+-rw-r--r--   0 runner    (1001) docker     (127)     1285 2024-05-29 12:24:48.000000 apysc-4.4.3/apysc/_material_design/icon/material_5g_outlined_icon.py
+-rw-r--r--   0 runner    (1001) docker     (127)     1238 2024-05-29 12:24:48.000000 apysc-4.4.3/apysc/_material_design/icon/material_5k_icon.py
+-rw-r--r--   0 runner    (1001) docker     (127)     1300 2024-05-29 12:24:48.000000 apysc-4.4.3/apysc/_material_design/icon/material_5k_plus_icon.py
+-rw-r--r--   0 runner    (1001) docker     (127)     1275 2024-05-29 12:24:48.000000 apysc-4.4.3/apysc/_material_design/icon/material_6k_icon.py
+-rw-r--r--   0 runner    (1001) docker     (127)     1340 2024-05-29 12:24:48.000000 apysc-4.4.3/apysc/_material_design/icon/material_6k_plus_icon.py
+-rw-r--r--   0 runner    (1001) docker     (127)     1223 2024-05-29 12:24:48.000000 apysc-4.4.3/apysc/_material_design/icon/material_7k_icon.py
+-rw-r--r--   0 runner    (1001) docker     (127)     1277 2024-05-29 12:24:48.000000 apysc-4.4.3/apysc/_material_design/icon/material_7k_plus_icon.py
+-rw-r--r--   0 runner    (1001) docker     (127)     1277 2024-05-29 12:24:48.000000 apysc-4.4.3/apysc/_material_design/icon/material_8k_icon.py
+-rw-r--r--   0 runner    (1001) docker     (127)     1343 2024-05-29 12:24:48.000000 apysc-4.4.3/apysc/_material_design/icon/material_8k_plus_icon.py
+-rw-r--r--   0 runner    (1001) docker     (127)     1273 2024-05-29 12:24:48.000000 apysc-4.4.3/apysc/_material_design/icon/material_9k_icon.py
+-rw-r--r--   0 runner    (1001) docker     (127)     1337 2024-05-29 12:24:48.000000 apysc-4.4.3/apysc/_material_design/icon/material_9k_plus_icon.py
+-rw-r--r--   0 runner    (1001) docker     (127)     1136 2024-05-29 12:24:48.000000 apysc-4.4.3/apysc/_material_design/icon/material_accessibility_icon.py
+-rw-r--r--   0 runner    (1001) docker     (127)     1217 2024-05-29 12:24:48.000000 apysc-4.4.3/apysc/_material_design/icon/material_accessibility_new_icon.py
+-rw-r--r--   0 runner    (1001) docker     (127)     1245 2024-05-29 12:24:48.000000 apysc-4.4.3/apysc/_material_design/icon/material_accessibility_new_outlined_icon.py
+-rw-r--r--   0 runner    (1001) docker     (127)     1164 2024-05-29 12:24:48.000000 apysc-4.4.3/apysc/_material_design/icon/material_accessibility_outlined_icon.py
+-rw-r--r--   0 runner    (1001) docker     (127)     1360 2024-05-29 12:24:48.000000 apysc-4.4.3/apysc/_material_design/icon/material_accessible_forward_icon.py
+-rw-r--r--   0 runner    (1001) docker     (127)     1389 2024-05-29 12:24:48.000000 apysc-4.4.3/apysc/_material_design/icon/material_accessible_forward_outlined_icon.py
+-rw-r--r--   0 runner    (1001) docker     (127)     1449 2024-05-29 12:24:48.000000 apysc-4.4.3/apysc/_material_design/icon/material_accessible_icon.py
+-rw-r--r--   0 runner    (1001) docker     (127)     1475 2024-05-29 12:24:48.000000 apysc-4.4.3/apysc/_material_design/icon/material_accessible_outlined_icon.py
+-rw-r--r--   0 runner    (1001) docker     (127)     1316 2024-05-29 12:24:48.000000 apysc-4.4.3/apysc/_material_design/icon/material_account_balance_icon.py
+-rw-r--r--   0 runner    (1001) docker     (127)     1210 2024-05-29 12:24:48.000000 apysc-4.4.3/apysc/_material_design/icon/material_account_balance_outlined_icon.py
+-rw-r--r--   0 runner    (1001) docker     (127)     1289 2024-05-29 12:24:48.000000 apysc-4.4.3/apysc/_material_design/icon/material_account_balance_wallet_icon.py
+-rw-r--r--   0 runner    (1001) docker     (127)     1339 2024-05-29 12:24:48.000000 apysc-4.4.3/apysc/_material_design/icon/material_account_balance_wallet_outlined_icon.py
+-rw-r--r--   0 runner    (1001) docker     (127)     1221 2024-05-29 12:24:48.000000 apysc-4.4.3/apysc/_material_design/icon/material_account_box_icon.py
+-rw-r--r--   0 runner    (1001) docker     (127)     1391 2024-05-29 12:24:48.000000 apysc-4.4.3/apysc/_material_design/icon/material_account_box_outlined_icon.py
+-rw-r--r--   0 runner    (1001) docker     (127)     1281 2024-05-29 12:24:48.000000 apysc-4.4.3/apysc/_material_design/icon/material_account_circle_icon.py
+-rw-r--r--   0 runner    (1001) docker     (127)     1539 2024-05-29 12:24:48.000000 apysc-4.4.3/apysc/_material_design/icon/material_account_circle_outlined_icon.py
+-rw-r--r--   0 runner    (1001) docker     (127)     1301 2024-05-29 12:24:48.000000 apysc-4.4.3/apysc/_material_design/icon/material_add_alert_icon.py
+-rw-r--r--   0 runner    (1001) docker     (127)     1300 2024-05-29 12:24:48.000000 apysc-4.4.3/apysc/_material_design/icon/material_add_alert_outlined_icon.py
+-rw-r--r--   0 runner    (1001) docker     (127)     1146 2024-05-29 12:24:48.000000 apysc-4.4.3/apysc/_material_design/icon/material_add_box_icon.py
+-rw-r--r--   0 runner    (1001) docker     (127)     1187 2024-05-29 12:24:48.000000 apysc-4.4.3/apysc/_material_design/icon/material_add_box_outlined_icon.py
+-rw-r--r--   0 runner    (1001) docker     (127)     1142 2024-05-29 12:24:48.000000 apysc-4.4.3/apysc/_material_design/icon/material_add_circle_icon.py
+-rw-r--r--   0 runner    (1001) docker     (127)     1223 2024-05-29 12:24:48.000000 apysc-4.4.3/apysc/_material_design/icon/material_add_circle_outline_icon.py
+-rw-r--r--   0 runner    (1001) docker     (127)     1251 2024-05-29 12:24:48.000000 apysc-4.4.3/apysc/_material_design/icon/material_add_circle_outline_outlined_icon.py
+-rw-r--r--   0 runner    (1001) docker     (127)     1170 2024-05-29 12:24:48.000000 apysc-4.4.3/apysc/_material_design/icon/material_add_circle_outlined_icon.py
+-rw-r--r--   0 runner    (1001) docker     (127)     1319 2024-05-29 12:24:48.000000 apysc-4.4.3/apysc/_material_design/icon/material_add_ic_call_icon.py
+-rw-r--r--   0 runner    (1001) docker     (127)     1518 2024-05-29 12:24:48.000000 apysc-4.4.3/apysc/_material_design/icon/material_add_ic_call_outlined_icon.py
+-rw-r--r--   0 runner    (1001) docker     (127)     1057 2024-05-29 12:24:48.000000 apysc-4.4.3/apysc/_material_design/icon/material_add_icon.py
+-rw-r--r--   0 runner    (1001) docker     (127)     1245 2024-05-29 12:24:48.000000 apysc-4.4.3/apysc/_material_design/icon/material_add_link_icon.py
+-rw-r--r--   0 runner    (1001) docker     (127)     1085 2024-05-29 12:24:48.000000 apysc-4.4.3/apysc/_material_design/icon/material_add_outlined_icon.py
+-rw-r--r--   0 runner    (1001) docker     (127)     1449 2024-05-29 12:24:48.000000 apysc-4.4.3/apysc/_material_design/icon/material_add_shopping_cart_icon.py
+-rw-r--r--   0 runner    (1001) docker     (127)     1376 2024-05-29 12:24:48.000000 apysc-4.4.3/apysc/_material_design/icon/material_add_shopping_cart_outlined_icon.py
+-rw-r--r--   0 runner    (1001) docker     (127)     1375 2024-05-29 12:24:48.000000 apysc-4.4.3/apysc/_material_design/icon/material_add_task_icon.py
+-rw-r--r--   0 runner    (1001) docker     (127)     1401 2024-05-29 12:24:48.000000 apysc-4.4.3/apysc/_material_design/icon/material_add_task_outlined_icon.py
+-rw-r--r--   0 runner    (1001) docker     (127)     1292 2024-05-29 12:24:48.000000 apysc-4.4.3/apysc/_material_design/icon/material_add_to_drive_icon.py
+-rw-r--r--   0 runner    (1001) docker     (127)     1196 2024-05-29 12:24:48.000000 apysc-4.4.3/apysc/_material_design/icon/material_add_to_queue_icon.py
+-rw-r--r--   0 runner    (1001) docker     (127)     1212 2024-05-29 12:24:48.000000 apysc-4.4.3/apysc/_material_design/icon/material_add_to_queue_outlined_icon.py
+-rw-r--r--   0 runner    (1001) docker     (127)     1192 2024-05-29 12:24:48.000000 apysc-4.4.3/apysc/_material_design/icon/material_addchart_icon.py
+-rw-r--r--   0 runner    (1001) docker     (127)     1276 2024-05-29 12:24:48.000000 apysc-4.4.3/apysc/_material_design/icon/material_addchart_outlined_icon.py
+-rw-r--r--   0 runner    (1001) docker     (127)     1608 2024-05-29 12:24:48.000000 apysc-4.4.3/apysc/_material_design/icon/material_admin_panel_settings_icon.py
+-rw-r--r--   0 runner    (1001) docker     (127)     1773 2024-05-29 12:24:48.000000 apysc-4.4.3/apysc/_material_design/icon/material_admin_panel_settings_outlined_icon.py
+-rw-r--r--   0 runner    (1001) docker     (127)     1218 2024-05-29 12:24:48.000000 apysc-4.4.3/apysc/_material_design/icon/material_airplay_icon.py
+-rw-r--r--   0 runner    (1001) docker     (127)     1346 2024-05-29 12:24:48.000000 apysc-4.4.3/apysc/_material_design/icon/material_airplay_outlined_icon.py
+-rw-r--r--   0 runner    (1001) docker     (127)     1290 2024-05-29 12:24:48.000000 apysc-4.4.3/apysc/_material_design/icon/material_alarm_add_icon.py
+-rw-r--r--   0 runner    (1001) docker     (127)     1308 2024-05-29 12:24:48.000000 apysc-4.4.3/apysc/_material_design/icon/material_alarm_add_outlined_icon.py
+-rw-r--r--   0 runner    (1001) docker     (127)     1285 2024-05-29 12:24:48.000000 apysc-4.4.3/apysc/_material_design/icon/material_alarm_icon.py
+-rw-r--r--   0 runner    (1001) docker     (127)     1541 2024-05-29 12:24:48.000000 apysc-4.4.3/apysc/_material_design/icon/material_alarm_off_icon.py
+-rw-r--r--   0 runner    (1001) docker     (127)     1550 2024-05-29 12:24:48.000000 apysc-4.4.3/apysc/_material_design/icon/material_alarm_off_outlined_icon.py
+-rw-r--r--   0 runner    (1001) docker     (127)     1320 2024-05-29 12:24:48.000000 apysc-4.4.3/apysc/_material_design/icon/material_alarm_on_icon.py
+-rw-r--r--   0 runner    (1001) docker     (127)     1331 2024-05-29 12:24:48.000000 apysc-4.4.3/apysc/_material_design/icon/material_alarm_on_outlined_icon.py
+-rw-r--r--   0 runner    (1001) docker     (127)     1302 2024-05-29 12:24:48.000000 apysc-4.4.3/apysc/_material_design/icon/material_alarm_outlined_icon.py
+-rw-r--r--   0 runner    (1001) docker     (127)     1231 2024-05-29 12:24:48.000000 apysc-4.4.3/apysc/_material_design/icon/material_album_icon.py
+-rw-r--r--   0 runner    (1001) docker     (127)     1318 2024-05-29 12:24:48.000000 apysc-4.4.3/apysc/_material_design/icon/material_album_outlined_icon.py
+-rw-r--r--   0 runner    (1001) docker     (127)     1240 2024-05-29 12:24:48.000000 apysc-4.4.3/apysc/_material_design/icon/material_all_inbox_icon.py
+-rw-r--r--   0 runner    (1001) docker     (127)     1534 2024-05-29 12:24:48.000000 apysc-4.4.3/apysc/_material_design/icon/material_all_inbox_outlined_icon.py
+-rw-r--r--   0 runner    (1001) docker     (127)     1271 2024-05-29 12:24:48.000000 apysc-4.4.3/apysc/_material_design/icon/material_all_out_icon.py
+-rw-r--r--   0 runner    (1001) docker     (127)     1227 2024-05-29 12:24:48.000000 apysc-4.4.3/apysc/_material_design/icon/material_all_out_outlined_icon.py
+-rw-r--r--   0 runner    (1001) docker     (127)     1394 2024-05-29 12:24:48.000000 apysc-4.4.3/apysc/_material_design/icon/material_alternate_email_icon.py
+-rw-r--r--   0 runner    (1001) docker     (127)     1434 2024-05-29 12:24:48.000000 apysc-4.4.3/apysc/_material_design/icon/material_alternate_email_outlined_icon.py
+-rw-r--r--   0 runner    (1001) docker     (127)     1222 2024-05-29 12:24:48.000000 apysc-4.4.3/apysc/_material_design/icon/material_amp_stories_icon.py
+-rw-r--r--   0 runner    (1001) docker     (127)     1249 2024-05-29 12:24:48.000000 apysc-4.4.3/apysc/_material_design/icon/material_amp_stories_outlined_icon.py
+-rw-r--r--   0 runner    (1001) docker     (127)     1176 2024-05-29 12:24:48.000000 apysc-4.4.3/apysc/_material_design/icon/material_analytics_icon.py
+-rw-r--r--   0 runner    (1001) docker     (127)     1387 2024-05-29 12:24:48.000000 apysc-4.4.3/apysc/_material_design/icon/material_analytics_outlined_icon.py
+-rw-r--r--   0 runner    (1001) docker     (127)     1371 2024-05-29 12:24:48.000000 apysc-4.4.3/apysc/_material_design/icon/material_anchor_icon.py
+-rw-r--r--   0 runner    (1001) docker     (127)     1397 2024-05-29 12:24:48.000000 apysc-4.4.3/apysc/_material_design/icon/material_anchor_outlined_icon.py
+-rw-r--r--   0 runner    (1001) docker     (127)     1577 2024-05-29 12:24:48.000000 apysc-4.4.3/apysc/_material_design/icon/material_android_icon.py
+-rw-r--r--   0 runner    (1001) docker     (127)     1623 2024-05-29 12:24:48.000000 apysc-4.4.3/apysc/_material_design/icon/material_android_outlined_icon.py
+-rw-r--r--   0 runner    (1001) docker     (127)     1152 2024-05-29 12:24:48.000000 apysc-4.4.3/apysc/_material_design/icon/material_announcement_icon.py
+-rw-r--r--   0 runner    (1001) docker     (127)     1195 2024-05-29 12:24:48.000000 apysc-4.4.3/apysc/_material_design/icon/material_announcement_outlined_icon.py
+-rw-r--r--   0 runner    (1001) docker     (127)     1322 2024-05-29 12:24:48.000000 apysc-4.4.3/apysc/_material_design/icon/material_api_icon.py
+-rw-r--r--   0 runner    (1001) docker     (127)     1348 2024-05-29 12:24:48.000000 apysc-4.4.3/apysc/_material_design/icon/material_api_outlined_icon.py
+-rw-r--r--   0 runner    (1001) docker     (127)     1377 2024-05-29 12:24:48.000000 apysc-4.4.3/apysc/_material_design/icon/material_app_blocking_icon.py
+-rw-r--r--   0 runner    (1001) docker     (127)     1570 2024-05-29 12:24:48.000000 apysc-4.4.3/apysc/_material_design/icon/material_app_blocking_outlined_icon.py
+-rw-r--r--   0 runner    (1001) docker     (127)     1562 2024-05-29 12:24:48.000000 apysc-4.4.3/apysc/_material_design/icon/material_app_registration_icon.py
+-rw-r--r--   0 runner    (1001) docker     (127)     1266 2024-05-29 12:24:48.000000 apysc-4.4.3/apysc/_material_design/icon/material_archive_icon.py
+-rw-r--r--   0 runner    (1001) docker     (127)     1308 2024-05-29 12:24:48.000000 apysc-4.4.3/apysc/_material_design/icon/material_archive_outlined_icon.py
+-rw-r--r--   0 runner    (1001) docker     (127)     1294 2024-05-29 12:24:48.000000 apysc-4.4.3/apysc/_material_design/icon/material_arrow_circle_down_icon.py
+-rw-r--r--   0 runner    (1001) docker     (127)     1320 2024-05-29 12:24:48.000000 apysc-4.4.3/apysc/_material_design/icon/material_arrow_circle_down_outlined_icon.py
+-rw-r--r--   0 runner    (1001) docker     (127)     1295 2024-05-29 12:24:48.000000 apysc-4.4.3/apysc/_material_design/icon/material_arrow_circle_up_icon.py
+-rw-r--r--   0 runner    (1001) docker     (127)     1321 2024-05-29 12:24:48.000000 apysc-4.4.3/apysc/_material_design/icon/material_arrow_circle_up_outlined_icon.py
+-rw-r--r--   0 runner    (1001) docker     (127)     1092 2024-05-29 12:24:48.000000 apysc-4.4.3/apysc/_material_design/icon/material_arrow_right_alt_icon.py
+-rw-r--r--   0 runner    (1001) docker     (127)     1122 2024-05-29 12:24:48.000000 apysc-4.4.3/apysc/_material_design/icon/material_arrow_right_alt_outlined_icon.py
+-rw-r--r--   0 runner    (1001) docker     (127)     1206 2024-05-29 12:24:48.000000 apysc-4.4.3/apysc/_material_design/icon/material_art_track_icon.py
+-rw-r--r--   0 runner    (1001) docker     (127)     1234 2024-05-29 12:24:48.000000 apysc-4.4.3/apysc/_material_design/icon/material_art_track_outlined_icon.py
+-rw-r--r--   0 runner    (1001) docker     (127)     1155 2024-05-29 12:24:48.000000 apysc-4.4.3/apysc/_material_design/icon/material_article_icon.py
+-rw-r--r--   0 runner    (1001) docker     (127)     1281 2024-05-29 12:24:48.000000 apysc-4.4.3/apysc/_material_design/icon/material_article_outlined_icon.py
+-rw-r--r--   0 runner    (1001) docker     (127)     1188 2024-05-29 12:24:48.000000 apysc-4.4.3/apysc/_material_design/icon/material_aspect_ratio_icon.py
+-rw-r--r--   0 runner    (1001) docker     (127)     1216 2024-05-29 12:24:48.000000 apysc-4.4.3/apysc/_material_design/icon/material_aspect_ratio_outlined_icon.py
+-rw-r--r--   0 runner    (1001) docker     (127)     1164 2024-05-29 12:24:48.000000 apysc-4.4.3/apysc/_material_design/icon/material_assessment_icon.py
+-rw-r--r--   0 runner    (1001) docker     (127)     1200 2024-05-29 12:24:48.000000 apysc-4.4.3/apysc/_material_design/icon/material_assessment_outlined_icon.py
+-rw-r--r--   0 runner    (1001) docker     (127)     1265 2024-05-29 12:24:48.000000 apysc-4.4.3/apysc/_material_design/icon/material_assignment_icon.py
+-rw-r--r--   0 runner    (1001) docker     (127)     1333 2024-05-29 12:24:48.000000 apysc-4.4.3/apysc/_material_design/icon/material_assignment_ind_icon.py
+-rw-r--r--   0 runner    (1001) docker     (127)     1564 2024-05-29 12:24:48.000000 apysc-4.4.3/apysc/_material_design/icon/material_assignment_ind_outlined_icon.py
+-rw-r--r--   0 runner    (1001) docker     (127)     1266 2024-05-29 12:24:48.000000 apysc-4.4.3/apysc/_material_design/icon/material_assignment_late_icon.py
+-rw-r--r--   0 runner    (1001) docker     (127)     1445 2024-05-29 12:24:48.000000 apysc-4.4.3/apysc/_material_design/icon/material_assignment_late_outlined_icon.py
+-rw-r--r--   0 runner    (1001) docker     (127)     1442 2024-05-29 12:24:48.000000 apysc-4.4.3/apysc/_material_design/icon/material_assignment_outlined_icon.py
+-rw-r--r--   0 runner    (1001) docker     (127)     1267 2024-05-29 12:24:48.000000 apysc-4.4.3/apysc/_material_design/icon/material_assignment_return_icon.py
+-rw-r--r--   0 runner    (1001) docker     (127)     1452 2024-05-29 12:24:48.000000 apysc-4.4.3/apysc/_material_design/icon/material_assignment_return_outlined_icon.py
+-rw-r--r--   0 runner    (1001) docker     (127)     1273 2024-05-29 12:24:48.000000 apysc-4.4.3/apysc/_material_design/icon/material_assignment_returned_icon.py
+-rw-r--r--   0 runner    (1001) docker     (127)     1454 2024-05-29 12:24:48.000000 apysc-4.4.3/apysc/_material_design/icon/material_assignment_returned_outlined_icon.py
+-rw-r--r--   0 runner    (1001) docker     (127)     1300 2024-05-29 12:24:48.000000 apysc-4.4.3/apysc/_material_design/icon/material_assignment_turned_in_icon.py
+-rw-r--r--   0 runner    (1001) docker     (127)     1479 2024-05-29 12:24:48.000000 apysc-4.4.3/apysc/_material_design/icon/material_assignment_turned_in_outlined_icon.py
+-rw-r--r--   0 runner    (1001) docker     (127)     1321 2024-05-29 12:24:48.000000 apysc-4.4.3/apysc/_material_design/icon/material_attribution_outlined_icon.py
+-rw-r--r--   0 runner    (1001) docker     (127)     1423 2024-05-29 12:24:48.000000 apysc-4.4.3/apysc/_material_design/icon/material_auto_delete_icon.py
+-rw-r--r--   0 runner    (1001) docker     (127)     1517 2024-05-29 12:24:48.000000 apysc-4.4.3/apysc/_material_design/icon/material_auto_delete_outlined_icon.py
+-rw-r--r--   0 runner    (1001) docker     (127)     1270 2024-05-29 12:24:48.000000 apysc-4.4.3/apysc/_material_design/icon/material_autorenew_icon.py
+-rw-r--r--   0 runner    (1001) docker     (127)     1298 2024-05-29 12:24:48.000000 apysc-4.4.3/apysc/_material_design/icon/material_autorenew_outlined_icon.py
+-rw-r--r--   0 runner    (1001) docker     (127)     1384 2024-05-29 12:24:48.000000 apysc-4.4.3/apysc/_material_design/icon/material_av_timer_icon.py
+-rw-r--r--   0 runner    (1001) docker     (127)     1412 2024-05-29 12:24:48.000000 apysc-4.4.3/apysc/_material_design/icon/material_av_timer_outlined_icon.py
+-rw-r--r--   0 runner    (1001) docker     (127)     1253 2024-05-29 12:24:48.000000 apysc-4.4.3/apysc/_material_design/icon/material_backspace_icon.py
+-rw-r--r--   0 runner    (1001) docker     (127)     1303 2024-05-29 12:24:48.000000 apysc-4.4.3/apysc/_material_design/icon/material_backspace_outlined_icon.py
+-rw-r--r--   0 runner    (1001) docker     (127)     1211 2024-05-29 12:24:48.000000 apysc-4.4.3/apysc/_material_design/icon/material_backup_icon.py
+-rw-r--r--   0 runner    (1001) docker     (127)     1418 2024-05-29 12:24:48.000000 apysc-4.4.3/apysc/_material_design/icon/material_backup_outlined_icon.py
+-rw-r--r--   0 runner    (1001) docker     (127)     1293 2024-05-29 12:24:48.000000 apysc-4.4.3/apysc/_material_design/icon/material_backup_table_icon.py
+-rw-r--r--   0 runner    (1001) docker     (127)     1319 2024-05-29 12:24:48.000000 apysc-4.4.3/apysc/_material_design/icon/material_backup_table_outlined_icon.py
+-rw-r--r--   0 runner    (1001) docker     (127)     1306 2024-05-29 12:24:48.000000 apysc-4.4.3/apysc/_material_design/icon/material_ballot_icon.py
+-rw-r--r--   0 runner    (1001) docker     (127)     1235 2024-05-29 12:24:48.000000 apysc-4.4.3/apysc/_material_design/icon/material_ballot_outlined_icon.py
+-rw-r--r--   0 runner    (1001) docker     (127)     1451 2024-05-29 12:24:48.000000 apysc-4.4.3/apysc/_material_design/icon/material_batch_prediction_icon.py
+-rw-r--r--   0 runner    (1001) docker     (127)     1477 2024-05-29 12:24:48.000000 apysc-4.4.3/apysc/_material_design/icon/material_batch_prediction_outlined_icon.py
+-rw-r--r--   0 runner    (1001) docker     (127)     1541 2024-05-29 12:24:48.000000 apysc-4.4.3/apysc/_material_design/icon/material_biotech_icon.py
+-rw-r--r--   0 runner    (1001) docker     (127)     1631 2024-05-29 12:24:48.000000 apysc-4.4.3/apysc/_material_design/icon/material_biotech_outlined_icon.py
+-rw-r--r--   0 runner    (1001) docker     (127)     1330 2024-05-29 12:24:48.000000 apysc-4.4.3/apysc/_material_design/icon/material_block_flipped_icon.py
+-rw-r--r--   0 runner    (1001) docker     (127)     1261 2024-05-29 12:24:48.000000 apysc-4.4.3/apysc/_material_design/icon/material_block_icon.py
+-rw-r--r--   0 runner    (1001) docker     (127)     1289 2024-05-29 12:24:48.000000 apysc-4.4.3/apysc/_material_design/icon/material_block_outlined_icon.py
+-rw-r--r--   0 runner    (1001) docker     (127)     1139 2024-05-29 12:24:48.000000 apysc-4.4.3/apysc/_material_design/icon/material_bolt_icon.py
+-rw-r--r--   0 runner    (1001) docker     (127)     1126 2024-05-29 12:24:48.000000 apysc-4.4.3/apysc/_material_design/icon/material_book_icon.py
+-rw-r--r--   0 runner    (1001) docker     (127)     1465 2024-05-29 12:24:48.000000 apysc-4.4.3/apysc/_material_design/icon/material_book_online_icon.py
+-rw-r--r--   0 runner    (1001) docker     (127)     1523 2024-05-29 12:24:48.000000 apysc-4.4.3/apysc/_material_design/icon/material_book_online_outlined_icon.py
+-rw-r--r--   0 runner    (1001) docker     (127)     1185 2024-05-29 12:24:48.000000 apysc-4.4.3/apysc/_material_design/icon/material_book_outlined_icon.py
+-rw-r--r--   0 runner    (1001) docker     (127)     1143 2024-05-29 12:24:48.000000 apysc-4.4.3/apysc/_material_design/icon/material_bookmark_border_icon.py
+-rw-r--r--   0 runner    (1001) docker     (127)     1164 2024-05-29 12:24:48.000000 apysc-4.4.3/apysc/_material_design/icon/material_bookmark_border_outlined_icon.py
+-rw-r--r--   0 runner    (1001) docker     (127)     1096 2024-05-29 12:24:48.000000 apysc-4.4.3/apysc/_material_design/icon/material_bookmark_icon.py
+-rw-r--r--   0 runner    (1001) docker     (127)     1117 2024-05-29 12:24:48.000000 apysc-4.4.3/apysc/_material_design/icon/material_bookmark_outlined_icon.py
+-rw-r--r--   0 runner    (1001) docker     (127)     1165 2024-05-29 12:24:48.000000 apysc-4.4.3/apysc/_material_design/icon/material_bookmarks_icon.py
+-rw-r--r--   0 runner    (1001) docker     (127)     1239 2024-05-29 12:24:48.000000 apysc-4.4.3/apysc/_material_design/icon/material_bookmarks_outlined_icon.py
+-rw-r--r--   0 runner    (1001) docker     (127)     1160 2024-05-29 12:24:48.000000 apysc-4.4.3/apysc/_material_design/icon/material_branding_watermark_icon.py
+-rw-r--r--   0 runner    (1001) docker     (127)     1200 2024-05-29 12:24:48.000000 apysc-4.4.3/apysc/_material_design/icon/material_branding_watermark_outlined_icon.py
+-rw-r--r--   0 runner    (1001) docker     (127)     1416 2024-05-29 12:24:48.000000 apysc-4.4.3/apysc/_material_design/icon/material_bug_report_icon.py
+-rw-r--r--   0 runner    (1001) docker     (127)     1737 2024-05-29 12:24:48.000000 apysc-4.4.3/apysc/_material_design/icon/material_bug_report_outlined_icon.py
+-rw-r--r--   0 runner    (1001) docker     (127)     1462 2024-05-29 12:24:48.000000 apysc-4.4.3/apysc/_material_design/icon/material_build_circle_icon.py
+-rw-r--r--   0 runner    (1001) docker     (127)     1590 2024-05-29 12:24:48.000000 apysc-4.4.3/apysc/_material_design/icon/material_build_circle_outlined_icon.py
+-rw-r--r--   0 runner    (1001) docker     (127)     1216 2024-05-29 12:24:48.000000 apysc-4.4.3/apysc/_material_design/icon/material_build_icon.py
+-rw-r--r--   0 runner    (1001) docker     (127)     1496 2024-05-29 12:24:48.000000 apysc-4.4.3/apysc/_material_design/icon/material_build_outlined_icon.py
+-rw-r--r--   0 runner    (1001) docker     (127)     1238 2024-05-29 12:24:48.000000 apysc-4.4.3/apysc/_material_design/icon/material_business_icon.py
+-rw-r--r--   0 runner    (1001) docker     (127)     1266 2024-05-29 12:24:48.000000 apysc-4.4.3/apysc/_material_design/icon/material_business_outlined_icon.py
+-rw-r--r--   0 runner    (1001) docker     (127)     1257 2024-05-29 12:24:48.000000 apysc-4.4.3/apysc/_material_design/icon/material_cached_icon.py
+-rw-r--r--   0 runner    (1001) docker     (127)     1285 2024-05-29 12:24:48.000000 apysc-4.4.3/apysc/_material_design/icon/material_cached_outlined_icon.py
+-rw-r--r--   0 runner    (1001) docker     (127)     1435 2024-05-29 12:24:48.000000 apysc-4.4.3/apysc/_material_design/icon/material_calculate_icon.py
+-rw-r--r--   0 runner    (1001) docker     (127)     1619 2024-05-29 12:24:48.000000 apysc-4.4.3/apysc/_material_design/icon/material_calculate_outlined_icon.py
+-rw-r--r--   0 runner    (1001) docker     (127)     1164 2024-05-29 12:24:48.000000 apysc-4.4.3/apysc/_material_design/icon/material_calendar_today_icon.py
+-rw-r--r--   0 runner    (1001) docker     (127)     1208 2024-05-29 12:24:48.000000 apysc-4.4.3/apysc/_material_design/icon/material_calendar_today_outlined_icon.py
+-rw-r--r--   0 runner    (1001) docker     (127)     1099 2024-05-29 12:24:48.000000 apysc-4.4.3/apysc/_material_design/icon/material_calendar_view_day_icon.py
+-rw-r--r--   0 runner    (1001) docker     (127)     1145 2024-05-29 12:24:48.000000 apysc-4.4.3/apysc/_material_design/icon/material_calendar_view_day_outlined_icon.py
+-rw-r--r--   0 runner    (1001) docker     (127)     1424 2024-05-29 12:24:48.000000 apysc-4.4.3/apysc/_material_design/icon/material_call_end_icon.py
+-rw-r--r--   0 runner    (1001) docker     (127)     1583 2024-05-29 12:24:48.000000 apysc-4.4.3/apysc/_material_design/icon/material_call_end_outlined_icon.py
+-rw-r--r--   0 runner    (1001) docker     (127)     1311 2024-05-29 12:24:48.000000 apysc-4.4.3/apysc/_material_design/icon/material_call_icon.py
+-rw-r--r--   0 runner    (1001) docker     (127)     1082 2024-05-29 12:24:48.000000 apysc-4.4.3/apysc/_material_design/icon/material_call_made_icon.py
+-rw-r--r--   0 runner    (1001) docker     (127)     1112 2024-05-29 12:24:48.000000 apysc-4.4.3/apysc/_material_design/icon/material_call_made_outlined_icon.py
+-rw-r--r--   0 runner    (1001) docker     (127)     1142 2024-05-29 12:24:48.000000 apysc-4.4.3/apysc/_material_design/icon/material_call_merge_icon.py
+-rw-r--r--   0 runner    (1001) docker     (127)     1170 2024-05-29 12:24:48.000000 apysc-4.4.3/apysc/_material_design/icon/material_call_merge_outlined_icon.py
+-rw-r--r--   0 runner    (1001) docker     (127)     1095 2024-05-29 12:24:48.000000 apysc-4.4.3/apysc/_material_design/icon/material_call_missed_icon.py
+-rw-r--r--   0 runner    (1001) docker     (127)     1200 2024-05-29 12:24:48.000000 apysc-4.4.3/apysc/_material_design/icon/material_call_missed_outgoing_icon.py
+-rw-r--r--   0 runner    (1001) docker     (127)     1153 2024-05-29 12:24:48.000000 apysc-4.4.3/apysc/_material_design/icon/material_call_missed_outgoing_outlined_icon.py
+-rw-r--r--   0 runner    (1001) docker     (127)     1131 2024-05-29 12:24:48.000000 apysc-4.4.3/apysc/_material_design/icon/material_call_missed_outlined_icon.py
+-rw-r--r--   0 runner    (1001) docker     (127)     1460 2024-05-29 12:24:48.000000 apysc-4.4.3/apysc/_material_design/icon/material_call_outlined_icon.py
+-rw-r--r--   0 runner    (1001) docker     (127)     1094 2024-05-29 12:24:48.000000 apysc-4.4.3/apysc/_material_design/icon/material_call_received_icon.py
+-rw-r--r--   0 runner    (1001) docker     (127)     1130 2024-05-29 12:24:48.000000 apysc-4.4.3/apysc/_material_design/icon/material_call_received_outlined_icon.py
+-rw-r--r--   0 runner    (1001) docker     (127)     1146 2024-05-29 12:24:48.000000 apysc-4.4.3/apysc/_material_design/icon/material_call_split_icon.py
+-rw-r--r--   0 runner    (1001) docker     (127)     1182 2024-05-29 12:24:48.000000 apysc-4.4.3/apysc/_material_design/icon/material_call_split_outlined_icon.py
+-rw-r--r--   0 runner    (1001) docker     (127)     1147 2024-05-29 12:24:48.000000 apysc-4.4.3/apysc/_material_design/icon/material_call_to_action_icon.py
+-rw-r--r--   0 runner    (1001) docker     (127)     1186 2024-05-29 12:24:48.000000 apysc-4.4.3/apysc/_material_design/icon/material_call_to_action_outlined_icon.py
+-rw-r--r--   0 runner    (1001) docker     (127)     1286 2024-05-29 12:24:48.000000 apysc-4.4.3/apysc/_material_design/icon/material_camera_enhance_icon.py
+-rw-r--r--   0 runner    (1001) docker     (127)     1410 2024-05-29 12:24:48.000000 apysc-4.4.3/apysc/_material_design/icon/material_camera_enhance_outlined_icon.py
+-rw-r--r--   0 runner    (1001) docker     (127)     1400 2024-05-29 12:24:48.000000 apysc-4.4.3/apysc/_material_design/icon/material_cancel_presentation_icon.py
+-rw-r--r--   0 runner    (1001) docker     (127)     1303 2024-05-29 12:24:48.000000 apysc-4.4.3/apysc/_material_design/icon/material_cancel_presentation_outlined_icon.py
+-rw-r--r--   0 runner    (1001) docker     (127)     1519 2024-05-29 12:24:48.000000 apysc-4.4.3/apysc/_material_design/icon/material_cancel_schedule_send_icon.py
+-rw-r--r--   0 runner    (1001) docker     (127)     1688 2024-05-29 12:24:48.000000 apysc-4.4.3/apysc/_material_design/icon/material_cancel_schedule_send_outlined_icon.py
+-rw-r--r--   0 runner    (1001) docker     (127)     1487 2024-05-29 12:24:48.000000 apysc-4.4.3/apysc/_material_design/icon/material_card_giftcard_icon.py
+-rw-r--r--   0 runner    (1001) docker     (127)     1500 2024-05-29 12:24:48.000000 apysc-4.4.3/apysc/_material_design/icon/material_card_giftcard_outlined_icon.py
+-rw-r--r--   0 runner    (1001) docker     (127)     1185 2024-05-29 12:24:48.000000 apysc-4.4.3/apysc/_material_design/icon/material_card_membership_icon.py
+-rw-r--r--   0 runner    (1001) docker     (127)     1213 2024-05-29 12:24:48.000000 apysc-4.4.3/apysc/_material_design/icon/material_card_membership_outlined_icon.py
+-rw-r--r--   0 runner    (1001) docker     (127)     1232 2024-05-29 12:24:48.000000 apysc-4.4.3/apysc/_material_design/icon/material_card_travel_icon.py
+-rw-r--r--   0 runner    (1001) docker     (127)     1260 2024-05-29 12:24:48.000000 apysc-4.4.3/apysc/_material_design/icon/material_card_travel_outlined_icon.py
+-rw-r--r--   0 runner    (1001) docker     (127)     1378 2024-05-29 12:24:48.000000 apysc-4.4.3/apysc/_material_design/icon/material_cell_wifi_icon.py
+-rw-r--r--   0 runner    (1001) docker     (127)     1105 2024-05-29 12:24:48.000000 apysc-4.4.3/apysc/_material_design/icon/material_change_history_icon.py
+-rw-r--r--   0 runner    (1001) docker     (127)     1131 2024-05-29 12:24:48.000000 apysc-4.4.3/apysc/_material_design/icon/material_change_history_outlined_icon.py
+-rw-r--r--   0 runner    (1001) docker     (127)     1111 2024-05-29 12:24:48.000000 apysc-4.4.3/apysc/_material_design/icon/material_chat_bubble_icon.py
+-rw-r--r--   0 runner    (1001) docker     (127)     1157 2024-05-29 12:24:48.000000 apysc-4.4.3/apysc/_material_design/icon/material_chat_bubble_outline_icon.py
+-rw-r--r--   0 runner    (1001) docker     (127)     1183 2024-05-29 12:24:48.000000 apysc-4.4.3/apysc/_material_design/icon/material_chat_bubble_outline_outlined_icon.py
+-rw-r--r--   0 runner    (1001) docker     (127)     1139 2024-05-29 12:24:48.000000 apysc-4.4.3/apysc/_material_design/icon/material_chat_bubble_outlined_icon.py
+-rw-r--r--   0 runner    (1001) docker     (127)     1140 2024-05-29 12:24:48.000000 apysc-4.4.3/apysc/_material_design/icon/material_chat_icon.py
+-rw-r--r--   0 runner    (1001) docker     (127)     1193 2024-05-29 12:24:48.000000 apysc-4.4.3/apysc/_material_design/icon/material_chat_outlined_icon.py
+-rw-r--r--   0 runner    (1001) docker     (127)     1165 2024-05-29 12:24:48.000000 apysc-4.4.3/apysc/_material_design/icon/material_check_circle_icon.py
+-rw-r--r--   0 runner    (1001) docker     (127)     1257 2024-05-29 12:24:48.000000 apysc-4.4.3/apysc/_material_design/icon/material_check_circle_outline_icon.py
+-rw-r--r--   0 runner    (1001) docker     (127)     1268 2024-05-29 12:24:48.000000 apysc-4.4.3/apysc/_material_design/icon/material_check_circle_outline_outlined_icon.py
+-rw-r--r--   0 runner    (1001) docker     (127)     1245 2024-05-29 12:24:48.000000 apysc-4.4.3/apysc/_material_design/icon/material_check_circle_outlined_icon.py
+-rw-r--r--   0 runner    (1001) docker     (127)     1239 2024-05-29 12:24:48.000000 apysc-4.4.3/apysc/_material_design/icon/material_chrome_reader_mode_icon.py
+-rw-r--r--   0 runner    (1001) docker     (127)     1247 2024-05-29 12:24:48.000000 apysc-4.4.3/apysc/_material_design/icon/material_chrome_reader_mode_outlined_icon.py
+-rw-r--r--   0 runner    (1001) docker     (127)     1299 2024-05-29 12:24:48.000000 apysc-4.4.3/apysc/_material_design/icon/material_circle_notifications_icon.py
+-rw-r--r--   0 runner    (1001) docker     (127)     1129 2024-05-29 12:24:48.000000 apysc-4.4.3/apysc/_material_design/icon/material_class_icon.py
+-rw-r--r--   0 runner    (1001) docker     (127)     1188 2024-05-29 12:24:48.000000 apysc-4.4.3/apysc/_material_design/icon/material_class_outlined_icon.py
+-rw-r--r--   0 runner    (1001) docker     (127)     1085 2024-05-29 12:24:48.000000 apysc-4.4.3/apysc/_material_design/icon/material_clear_all_icon.py
+-rw-r--r--   0 runner    (1001) docker     (127)     1113 2024-05-29 12:24:48.000000 apysc-4.4.3/apysc/_material_design/icon/material_clear_all_outlined_icon.py
+-rw-r--r--   0 runner    (1001) docker     (127)     1129 2024-05-29 12:24:48.000000 apysc-4.4.3/apysc/_material_design/icon/material_clear_icon.py
+-rw-r--r--   0 runner    (1001) docker     (127)     1165 2024-05-29 12:24:48.000000 apysc-4.4.3/apysc/_material_design/icon/material_clear_outlined_icon.py
+-rw-r--r--   0 runner    (1001) docker     (127)     1213 2024-05-29 12:24:48.000000 apysc-4.4.3/apysc/_material_design/icon/material_close_fullscreen_icon.py
+-rw-r--r--   0 runner    (1001) docker     (127)     1239 2024-05-29 12:24:48.000000 apysc-4.4.3/apysc/_material_design/icon/material_close_fullscreen_outlined_icon.py
+-rw-r--r--   0 runner    (1001) docker     (127)     1544 2024-05-29 12:24:48.000000 apysc-4.4.3/apysc/_material_design/icon/material_closed_caption_disabled_icon.py
+-rw-r--r--   0 runner    (1001) docker     (127)     1623 2024-05-29 12:24:48.000000 apysc-4.4.3/apysc/_material_design/icon/material_closed_caption_disabled_outlined_icon.py
+-rw-r--r--   0 runner    (1001) docker     (127)     1337 2024-05-29 12:24:48.000000 apysc-4.4.3/apysc/_material_design/icon/material_closed_caption_icon.py
+-rw-r--r--   0 runner    (1001) docker     (127)     1374 2024-05-29 12:24:48.000000 apysc-4.4.3/apysc/_material_design/icon/material_closed_caption_off_icon.py
+-rw-r--r--   0 runner    (1001) docker     (127)     1383 2024-05-29 12:24:48.000000 apysc-4.4.3/apysc/_material_design/icon/material_closed_caption_outlined_icon.py
+-rw-r--r--   0 runner    (1001) docker     (127)     1117 2024-05-29 12:24:48.000000 apysc-4.4.3/apysc/_material_design/icon/material_code_icon.py
+-rw-r--r--   0 runner    (1001) docker     (127)     1143 2024-05-29 12:24:48.000000 apysc-4.4.3/apysc/_material_design/icon/material_code_outlined_icon.py
+-rw-r--r--   0 runner    (1001) docker     (127)     1202 2024-05-29 12:24:48.000000 apysc-4.4.3/apysc/_material_design/icon/material_comment_bank_icon.py
+-rw-r--r--   0 runner    (1001) docker     (127)     1279 2024-05-29 12:24:48.000000 apysc-4.4.3/apysc/_material_design/icon/material_comment_bank_outlined_icon.py
+-rw-r--r--   0 runner    (1001) docker     (127)     1156 2024-05-29 12:24:48.000000 apysc-4.4.3/apysc/_material_design/icon/material_comment_icon.py
+-rw-r--r--   0 runner    (1001) docker     (127)     1204 2024-05-29 12:24:48.000000 apysc-4.4.3/apysc/_material_design/icon/material_comment_outlined_icon.py
+-rw-r--r--   0 runner    (1001) docker     (127)     1537 2024-05-29 12:24:48.000000 apysc-4.4.3/apysc/_material_design/icon/material_commute_icon.py
+-rw-r--r--   0 runner    (1001) docker     (127)     1551 2024-05-29 12:24:48.000000 apysc-4.4.3/apysc/_material_design/icon/material_commute_outlined_icon.py
+-rw-r--r--   0 runner    (1001) docker     (127)     1205 2024-05-29 12:24:48.000000 apysc-4.4.3/apysc/_material_design/icon/material_compare_arrows_icon.py
+-rw-r--r--   0 runner    (1001) docker     (127)     1154 2024-05-29 12:24:48.000000 apysc-4.4.3/apysc/_material_design/icon/material_compare_arrows_outlined_icon.py
+-rw-r--r--   0 runner    (1001) docker     (127)     1167 2024-05-29 12:24:48.000000 apysc-4.4.3/apysc/_material_design/icon/material_compress_icon.py
+-rw-r--r--   0 runner    (1001) docker     (127)     1307 2024-05-29 12:24:48.000000 apysc-4.4.3/apysc/_material_design/icon/material_contact_mail_icon.py
+-rw-r--r--   0 runner    (1001) docker     (127)     1446 2024-05-29 12:24:48.000000 apysc-4.4.3/apysc/_material_design/icon/material_contact_mail_outlined_icon.py
+-rw-r--r--   0 runner    (1001) docker     (127)     1360 2024-05-29 12:24:48.000000 apysc-4.4.3/apysc/_material_design/icon/material_contact_page_icon.py
+-rw-r--r--   0 runner    (1001) docker     (127)     1422 2024-05-29 12:24:48.000000 apysc-4.4.3/apysc/_material_design/icon/material_contact_page_outlined_icon.py
+-rw-r--r--   0 runner    (1001) docker     (127)     1413 2024-05-29 12:24:48.000000 apysc-4.4.3/apysc/_material_design/icon/material_contact_phone_icon.py
+-rw-r--r--   0 runner    (1001) docker     (127)     1580 2024-05-29 12:24:48.000000 apysc-4.4.3/apysc/_material_design/icon/material_contact_phone_outlined_icon.py
+-rw-r--r--   0 runner    (1001) docker     (127)     1268 2024-05-29 12:24:48.000000 apysc-4.4.3/apysc/_material_design/icon/material_contact_support_icon.py
+-rw-r--r--   0 runner    (1001) docker     (127)     1409 2024-05-29 12:24:48.000000 apysc-4.4.3/apysc/_material_design/icon/material_contact_support_outlined_icon.py
+-rw-r--r--   0 runner    (1001) docker     (127)     1643 2024-05-29 12:24:48.000000 apysc-4.4.3/apysc/_material_design/icon/material_contactless_icon.py
+-rw-r--r--   0 runner    (1001) docker     (127)     1751 2024-05-29 12:24:48.000000 apysc-4.4.3/apysc/_material_design/icon/material_contactless_outlined_icon.py
+-rw-r--r--   0 runner    (1001) docker     (127)     1315 2024-05-29 12:24:48.000000 apysc-4.4.3/apysc/_material_design/icon/material_contacts_icon.py
+-rw-r--r--   0 runner    (1001) docker     (127)     1426 2024-05-29 12:24:48.000000 apysc-4.4.3/apysc/_material_design/icon/material_contacts_outlined_icon.py
+-rw-r--r--   0 runner    (1001) docker     (127)     1175 2024-05-29 12:24:48.000000 apysc-4.4.3/apysc/_material_design/icon/material_content_copy_icon.py
+-rw-r--r--   0 runner    (1001) docker     (127)     1203 2024-05-29 12:24:48.000000 apysc-4.4.3/apysc/_material_design/icon/material_content_copy_outlined_icon.py
+-rw-r--r--   0 runner    (1001) docker     (127)     1582 2024-05-29 12:24:48.000000 apysc-4.4.3/apysc/_material_design/icon/material_content_cut_icon.py
+-rw-r--r--   0 runner    (1001) docker     (127)     1486 2024-05-29 12:24:48.000000 apysc-4.4.3/apysc/_material_design/icon/material_content_cut_outlined_icon.py
+-rw-r--r--   0 runner    (1001) docker     (127)     1251 2024-05-29 12:24:48.000000 apysc-4.4.3/apysc/_material_design/icon/material_content_paste_icon.py
+-rw-r--r--   0 runner    (1001) docker     (127)     1272 2024-05-29 12:24:48.000000 apysc-4.4.3/apysc/_material_design/icon/material_content_paste_outlined_icon.py
+-rw-r--r--   0 runner    (1001) docker     (127)     1304 2024-05-29 12:24:48.000000 apysc-4.4.3/apysc/_material_design/icon/material_control_camera_icon.py
+-rw-r--r--   0 runner    (1001) docker     (127)     1332 2024-05-29 12:24:48.000000 apysc-4.4.3/apysc/_material_design/icon/material_control_camera_outlined_icon.py
+-rw-r--r--   0 runner    (1001) docker     (127)     1498 2024-05-29 12:24:48.000000 apysc-4.4.3/apysc/_material_design/icon/material_copyright_icon.py
+-rw-r--r--   0 runner    (1001) docker     (127)     1793 2024-05-29 12:24:48.000000 apysc-4.4.3/apysc/_material_design/icon/material_copyright_outlined_icon.py
+-rw-r--r--   0 runner    (1001) docker     (127)     1180 2024-05-29 12:24:48.000000 apysc-4.4.3/apysc/_material_design/icon/material_create_icon.py
+-rw-r--r--   0 runner    (1001) docker     (127)     1259 2024-05-29 12:24:48.000000 apysc-4.4.3/apysc/_material_design/icon/material_create_outlined_icon.py
+-rw-r--r--   0 runner    (1001) docker     (127)     1167 2024-05-29 12:24:48.000000 apysc-4.4.3/apysc/_material_design/icon/material_credit_card_icon.py
+-rw-r--r--   0 runner    (1001) docker     (127)     1195 2024-05-29 12:24:48.000000 apysc-4.4.3/apysc/_material_design/icon/material_credit_card_outlined_icon.py
+-rw-r--r--   0 runner    (1001) docker     (127)     1211 2024-05-29 12:24:48.000000 apysc-4.4.3/apysc/_material_design/icon/material_dangerous_icon.py
+-rw-r--r--   0 runner    (1001) docker     (127)     1138 2024-05-29 12:24:48.000000 apysc-4.4.3/apysc/_material_design/icon/material_dashboard_customize_icon.py
+-rw-r--r--   0 runner    (1001) docker     (127)     1101 2024-05-29 12:24:48.000000 apysc-4.4.3/apysc/_material_design/icon/material_dashboard_icon.py
+-rw-r--r--   0 runner    (1001) docker     (127)     1186 2024-05-29 12:24:48.000000 apysc-4.4.3/apysc/_material_design/icon/material_dashboard_outlined_icon.py
+-rw-r--r--   0 runner    (1001) docker     (127)     1205 2024-05-29 12:24:48.000000 apysc-4.4.3/apysc/_material_design/icon/material_date_range_icon.py
+-rw-r--r--   0 runner    (1001) docker     (127)     1250 2024-05-29 12:24:48.000000 apysc-4.4.3/apysc/_material_design/icon/material_date_range_outlined_icon.py
+-rw-r--r--   0 runner    (1001) docker     (127)     1296 2024-05-29 12:24:48.000000 apysc-4.4.3/apysc/_material_design/icon/material_delete_forever_icon.py
+-rw-r--r--   0 runner    (1001) docker     (127)     1291 2024-05-29 12:24:48.000000 apysc-4.4.3/apysc/_material_design/icon/material_delete_forever_outlined_icon.py
+-rw-r--r--   0 runner    (1001) docker     (127)     1108 2024-05-29 12:24:48.000000 apysc-4.4.3/apysc/_material_design/icon/material_delete_icon.py
+-rw-r--r--   0 runner    (1001) docker     (127)     1143 2024-05-29 12:24:48.000000 apysc-4.4.3/apysc/_material_design/icon/material_delete_outline_icon.py
+-rw-r--r--   0 runner    (1001) docker     (127)     1174 2024-05-29 12:24:48.000000 apysc-4.4.3/apysc/_material_design/icon/material_delete_outline_outlined_icon.py
+-rw-r--r--   0 runner    (1001) docker     (127)     1152 2024-05-29 12:24:48.000000 apysc-4.4.3/apysc/_material_design/icon/material_delete_outlined_icon.py
+-rw-r--r--   0 runner    (1001) docker     (127)     1157 2024-05-29 12:24:48.000000 apysc-4.4.3/apysc/_material_design/icon/material_delete_sweep_icon.py
+-rw-r--r--   0 runner    (1001) docker     (127)     1195 2024-05-29 12:24:48.000000 apysc-4.4.3/apysc/_material_design/icon/material_delete_sweep_outlined_icon.py
+-rw-r--r--   0 runner    (1001) docker     (127)     1172 2024-05-29 12:24:48.000000 apysc-4.4.3/apysc/_material_design/icon/material_description_icon.py
+-rw-r--r--   0 runner    (1001) docker     (127)     1186 2024-05-29 12:24:48.000000 apysc-4.4.3/apysc/_material_design/icon/material_description_outlined_icon.py
+-rw-r--r--   0 runner    (1001) docker     (127)     1265 2024-05-29 12:24:48.000000 apysc-4.4.3/apysc/_material_design/icon/material_desktop_access_disabled_icon.py
+-rw-r--r--   0 runner    (1001) docker     (127)     1295 2024-05-29 12:24:48.000000 apysc-4.4.3/apysc/_material_design/icon/material_desktop_access_disabled_outlined_icon.py
+-rw-r--r--   0 runner    (1001) docker     (127)     1365 2024-05-29 12:24:48.000000 apysc-4.4.3/apysc/_material_design/icon/material_dialer_sip_icon.py
+-rw-r--r--   0 runner    (1001) docker     (127)     1549 2024-05-29 12:24:48.000000 apysc-4.4.3/apysc/_material_design/icon/material_dialer_sip_outlined_icon.py
+-rw-r--r--   0 runner    (1001) docker     (127)     1519 2024-05-29 12:24:48.000000 apysc-4.4.3/apysc/_material_design/icon/material_dialpad_icon.py
+-rw-r--r--   0 runner    (1001) docker     (127)     1547 2024-05-29 12:24:48.000000 apysc-4.4.3/apysc/_material_design/icon/material_dialpad_outlined_icon.py
+-rw-r--r--   0 runner    (1001) docker     (127)     1234 2024-05-29 12:24:48.000000 apysc-4.4.3/apysc/_material_design/icon/material_disabled_by_default_icon.py
+-rw-r--r--   0 runner    (1001) docker     (127)     1278 2024-05-29 12:24:48.000000 apysc-4.4.3/apysc/_material_design/icon/material_disabled_by_default_outlined_icon.py
+-rw-r--r--   0 runner    (1001) docker     (127)     1279 2024-05-29 12:24:48.000000 apysc-4.4.3/apysc/_material_design/icon/material_dns_icon.py
+-rw-r--r--   0 runner    (1001) docker     (127)     1390 2024-05-29 12:24:48.000000 apysc-4.4.3/apysc/_material_design/icon/material_dns_outlined_icon.py
+-rw-r--r--   0 runner    (1001) docker     (127)     1268 2024-05-29 12:24:48.000000 apysc-4.4.3/apysc/_material_design/icon/material_domain_disabled_icon.py
+-rw-r--r--   0 runner    (1001) docker     (127)     1295 2024-05-29 12:24:48.000000 apysc-4.4.3/apysc/_material_design/icon/material_domain_disabled_outlined_icon.py
+-rw-r--r--   0 runner    (1001) docker     (127)     1316 2024-05-29 12:24:48.000000 apysc-4.4.3/apysc/_material_design/icon/material_domain_verification_icon.py
+-rw-r--r--   0 runner    (1001) docker     (127)     1342 2024-05-29 12:24:48.000000 apysc-4.4.3/apysc/_material_design/icon/material_domain_verification_outlined_icon.py
+-rw-r--r--   0 runner    (1001) docker     (127)     1189 2024-05-29 12:24:48.000000 apysc-4.4.3/apysc/_material_design/icon/material_done_all_icon.py
+-rw-r--r--   0 runner    (1001) docker     (127)     1217 2024-05-29 12:24:48.000000 apysc-4.4.3/apysc/_material_design/icon/material_done_all_outlined_icon.py
+-rw-r--r--   0 runner    (1001) docker     (127)     1075 2024-05-29 12:24:48.000000 apysc-4.4.3/apysc/_material_design/icon/material_done_icon.py
+-rw-r--r--   0 runner    (1001) docker     (127)     1178 2024-05-29 12:24:48.000000 apysc-4.4.3/apysc/_material_design/icon/material_done_outline_icon.py
+-rw-r--r--   0 runner    (1001) docker     (127)     1206 2024-05-29 12:24:48.000000 apysc-4.4.3/apysc/_material_design/icon/material_done_outline_outlined_icon.py
+-rw-r--r--   0 runner    (1001) docker     (127)     1103 2024-05-29 12:24:48.000000 apysc-4.4.3/apysc/_material_design/icon/material_done_outlined_icon.py
+-rw-r--r--   0 runner    (1001) docker     (127)     1323 2024-05-29 12:24:48.000000 apysc-4.4.3/apysc/_material_design/icon/material_donut_large_icon.py
+-rw-r--r--   0 runner    (1001) docker     (127)     1337 2024-05-29 12:24:48.000000 apysc-4.4.3/apysc/_material_design/icon/material_donut_large_outlined_icon.py
+-rw-r--r--   0 runner    (1001) docker     (127)     1254 2024-05-29 12:24:48.000000 apysc-4.4.3/apysc/_material_design/icon/material_donut_small_icon.py
+-rw-r--r--   0 runner    (1001) docker     (127)     1573 2024-05-29 12:24:48.000000 apysc-4.4.3/apysc/_material_design/icon/material_donut_small_outlined_icon.py
+-rw-r--r--   0 runner    (1001) docker     (127)     1179 2024-05-29 12:24:48.000000 apysc-4.4.3/apysc/_material_design/icon/material_drafts_icon.py
+-rw-r--r--   0 runner    (1001) docker     (127)     1241 2024-05-29 12:24:48.000000 apysc-4.4.3/apysc/_material_design/icon/material_drafts_outlined_icon.py
+-rw-r--r--   0 runner    (1001) docker     (127)     1347 2024-05-29 12:24:48.000000 apysc-4.4.3/apysc/_material_design/icon/material_drag_indicator_icon.py
+-rw-r--r--   0 runner    (1001) docker     (127)     1373 2024-05-29 12:24:48.000000 apysc-4.4.3/apysc/_material_design/icon/material_drag_indicator_outlined_icon.py
+-rw-r--r--   0 runner    (1001) docker     (127)     1146 2024-05-29 12:24:48.000000 apysc-4.4.3/apysc/_material_design/icon/material_duo_icon.py
+-rw-r--r--   0 runner    (1001) docker     (127)     1174 2024-05-29 12:24:48.000000 apysc-4.4.3/apysc/_material_design/icon/material_duo_outlined_icon.py
+-rw-r--r--   0 runner    (1001) docker     (127)     1581 2024-05-29 12:24:48.000000 apysc-4.4.3/apysc/_material_design/icon/material_dynamic_feed_icon.py
+-rw-r--r--   0 runner    (1001) docker     (127)     1607 2024-05-29 12:24:48.000000 apysc-4.4.3/apysc/_material_design/icon/material_dynamic_feed_outlined_icon.py
+-rw-r--r--   0 runner    (1001) docker     (127)     1286 2024-05-29 12:24:48.000000 apysc-4.4.3/apysc/_material_design/icon/material_dynamic_form_icon.py
+-rw-r--r--   0 runner    (1001) docker     (127)     1344 2024-05-29 12:24:48.000000 apysc-4.4.3/apysc/_material_design/icon/material_dynamic_form_outlined_icon.py
+-rw-r--r--   0 runner    (1001) docker     (127)     1255 2024-05-29 12:24:48.000000 apysc-4.4.3/apysc/_material_design/icon/material_eco_icon.py
+-rw-r--r--   0 runner    (1001) docker     (127)     1451 2024-05-29 12:24:48.000000 apysc-4.4.3/apysc/_material_design/icon/material_eco_outlined_icon.py
+-rw-r--r--   0 runner    (1001) docker     (127)     1275 2024-05-29 12:24:48.000000 apysc-4.4.3/apysc/_material_design/icon/material_edit_off_icon.py
+-rw-r--r--   0 runner    (1001) docker     (127)     1064 2024-05-29 12:24:48.000000 apysc-4.4.3/apysc/_material_design/icon/material_eject_icon.py
+-rw-r--r--   0 runner    (1001) docker     (127)     1122 2024-05-29 12:24:48.000000 apysc-4.4.3/apysc/_material_design/icon/material_eject_outlined_icon.py
+-rw-r--r--   0 runner    (1001) docker     (127)     1137 2024-05-29 12:24:48.000000 apysc-4.4.3/apysc/_material_design/icon/material_email_icon.py
+-rw-r--r--   0 runner    (1001) docker     (127)     1171 2024-05-29 12:24:48.000000 apysc-4.4.3/apysc/_material_design/icon/material_email_outlined_icon.py
+-rw-r--r--   0 runner    (1001) docker     (127)     1088 2024-05-29 12:24:48.000000 apysc-4.4.3/apysc/_material_design/icon/material_equalizer_icon.py
+-rw-r--r--   0 runner    (1001) docker     (127)     1116 2024-05-29 12:24:48.000000 apysc-4.4.3/apysc/_material_design/icon/material_equalizer_outlined_icon.py
+-rw-r--r--   0 runner    (1001) docker     (127)     1124 2024-05-29 12:24:48.000000 apysc-4.4.3/apysc/_material_design/icon/material_error_icon.py
+-rw-r--r--   0 runner    (1001) docker     (127)     1220 2024-05-29 12:24:48.000000 apysc-4.4.3/apysc/_material_design/icon/material_error_outline_icon.py
+-rw-r--r--   0 runner    (1001) docker     (127)     1212 2024-05-29 12:24:48.000000 apysc-4.4.3/apysc/_material_design/icon/material_error_outline_outlined_icon.py
+-rw-r--r--   0 runner    (1001) docker     (127)     1113 2024-05-29 12:24:48.000000 apysc-4.4.3/apysc/_material_design/icon/material_error_outlined_icon.py
+-rw-r--r--   0 runner    (1001) docker     (127)     1386 2024-05-29 12:24:48.000000 apysc-4.4.3/apysc/_material_design/icon/material_euro_symbol_icon.py
+-rw-r--r--   0 runner    (1001) docker     (127)     1409 2024-05-29 12:24:48.000000 apysc-4.4.3/apysc/_material_design/icon/material_euro_symbol_outlined_icon.py
+-rw-r--r--   0 runner    (1001) docker     (127)     1164 2024-05-29 12:24:48.000000 apysc-4.4.3/apysc/_material_design/icon/material_event_icon.py
+-rw-r--r--   0 runner    (1001) docker     (127)     1204 2024-05-29 12:24:48.000000 apysc-4.4.3/apysc/_material_design/icon/material_event_outlined_icon.py
+-rw-r--r--   0 runner    (1001) docker     (127)     1226 2024-05-29 12:24:48.000000 apysc-4.4.3/apysc/_material_design/icon/material_event_seat_icon.py
+-rw-r--r--   0 runner    (1001) docker     (127)     1183 2024-05-29 12:24:48.000000 apysc-4.4.3/apysc/_material_design/icon/material_event_seat_outlined_icon.py
+-rw-r--r--   0 runner    (1001) docker     (127)     1208 2024-05-29 12:24:48.000000 apysc-4.4.3/apysc/_material_design/icon/material_exit_to_app_icon.py
+-rw-r--r--   0 runner    (1001) docker     (127)     1236 2024-05-29 12:24:48.000000 apysc-4.4.3/apysc/_material_design/icon/material_exit_to_app_outlined_icon.py
+-rw-r--r--   0 runner    (1001) docker     (127)     1128 2024-05-29 12:24:48.000000 apysc-4.4.3/apysc/_material_design/icon/material_expand_icon.py
+-rw-r--r--   0 runner    (1001) docker     (127)     1145 2024-05-29 12:24:48.000000 apysc-4.4.3/apysc/_material_design/icon/material_explicit_icon.py
+-rw-r--r--   0 runner    (1001) docker     (127)     1190 2024-05-29 12:24:48.000000 apysc-4.4.3/apysc/_material_design/icon/material_explicit_outlined_icon.py
+-rw-r--r--   0 runner    (1001) docker     (127)     1229 2024-05-29 12:24:48.000000 apysc-4.4.3/apysc/_material_design/icon/material_explore_icon.py
+-rw-r--r--   0 runner    (1001) docker     (127)     2205 2024-05-29 12:24:48.000000 apysc-4.4.3/apysc/_material_design/icon/material_explore_off_icon.py
+-rw-r--r--   0 runner    (1001) docker     (127)     1528 2024-05-29 12:24:48.000000 apysc-4.4.3/apysc/_material_design/icon/material_explore_off_outlined_icon.py
+-rw-r--r--   0 runner    (1001) docker     (127)     1312 2024-05-29 12:24:48.000000 apysc-4.4.3/apysc/_material_design/icon/material_explore_outlined_icon.py
+-rw-r--r--   0 runner    (1001) docker     (127)     1332 2024-05-29 12:24:48.000000 apysc-4.4.3/apysc/_material_design/icon/material_extension_icon.py
+-rw-r--r--   0 runner    (1001) docker     (127)     1536 2024-05-29 12:24:48.000000 apysc-4.4.3/apysc/_material_design/icon/material_extension_outlined_icon.py
+-rw-r--r--   0 runner    (1001) docker     (127)     1437 2024-05-29 12:24:48.000000 apysc-4.4.3/apysc/_material_design/icon/material_face_icon.py
+-rw-r--r--   0 runner    (1001) docker     (127)     1631 2024-05-29 12:24:48.000000 apysc-4.4.3/apysc/_material_design/icon/material_face_outlined_icon.py
+-rw-r--r--   0 runner    (1001) docker     (127)     1651 2024-05-29 12:24:48.000000 apysc-4.4.3/apysc/_material_design/icon/material_face_unlock_outlined_icon.py
+-rw-r--r--   0 runner    (1001) docker     (127)     1325 2024-05-29 12:24:48.000000 apysc-4.4.3/apysc/_material_design/icon/material_fact_check_icon.py
+-rw-r--r--   0 runner    (1001) docker     (127)     1533 2024-05-29 12:24:48.000000 apysc-4.4.3/apysc/_material_design/icon/material_fact_check_outlined_icon.py
+-rw-r--r--   0 runner    (1001) docker     (127)     1087 2024-05-29 12:24:48.000000 apysc-4.4.3/apysc/_material_design/icon/material_fast_forward_icon.py
+-rw-r--r--   0 runner    (1001) docker     (127)     1324 2024-05-29 12:24:48.000000 apysc-4.4.3/apysc/_material_design/icon/material_fast_forward_outlined_icon.py
+-rw-r--r--   0 runner    (1001) docker     (127)     1088 2024-05-29 12:24:48.000000 apysc-4.4.3/apysc/_material_design/icon/material_fast_rewind_icon.py
+-rw-r--r--   0 runner    (1001) docker     (127)     1170 2024-05-29 12:24:48.000000 apysc-4.4.3/apysc/_material_design/icon/material_fast_rewind_outlined_icon.py
+-rw-r--r--   0 runner    (1001) docker     (127)     1400 2024-05-29 12:24:48.000000 apysc-4.4.3/apysc/_material_design/icon/material_favorite_border_icon.py
+-rw-r--r--   0 runner    (1001) docker     (127)     1428 2024-05-29 12:24:48.000000 apysc-4.4.3/apysc/_material_design/icon/material_favorite_border_outlined_icon.py
+-rw-r--r--   0 runner    (1001) docker     (127)     1211 2024-05-29 12:24:48.000000 apysc-4.4.3/apysc/_material_design/icon/material_favorite_icon.py
+-rw-r--r--   0 runner    (1001) docker     (127)     1239 2024-05-29 12:24:48.000000 apysc-4.4.3/apysc/_material_design/icon/material_favorite_outlined_icon.py
+-rw-r--r--   0 runner    (1001) docker     (127)     1170 2024-05-29 12:24:48.000000 apysc-4.4.3/apysc/_material_design/icon/material_featured_play_list_icon.py
+-rw-r--r--   0 runner    (1001) docker     (127)     1208 2024-05-29 12:24:48.000000 apysc-4.4.3/apysc/_material_design/icon/material_featured_play_list_outlined_icon.py
+-rw-r--r--   0 runner    (1001) docker     (127)     1146 2024-05-29 12:24:48.000000 apysc-4.4.3/apysc/_material_design/icon/material_featured_video_icon.py
+-rw-r--r--   0 runner    (1001) docker     (127)     1185 2024-05-29 12:24:48.000000 apysc-4.4.3/apysc/_material_design/icon/material_featured_video_outlined_icon.py
+-rw-r--r--   0 runner    (1001) docker     (127)     1141 2024-05-29 12:24:48.000000 apysc-4.4.3/apysc/_material_design/icon/material_feedback_icon.py
+-rw-r--r--   0 runner    (1001) docker     (127)     1197 2024-05-29 12:24:48.000000 apysc-4.4.3/apysc/_material_design/icon/material_feedback_outlined_icon.py
+-rw-r--r--   0 runner    (1001) docker     (127)     1467 2024-05-29 12:24:48.000000 apysc-4.4.3/apysc/_material_design/icon/material_fiber_dvr_icon.py
+-rw-r--r--   0 runner    (1001) docker     (127)     1297 2024-05-29 12:24:48.000000 apysc-4.4.3/apysc/_material_design/icon/material_fiber_dvr_outlined_icon.py
+-rw-r--r--   0 runner    (1001) docker     (127)     1091 2024-05-29 12:24:48.000000 apysc-4.4.3/apysc/_material_design/icon/material_fiber_manual_record_icon.py
+-rw-r--r--   0 runner    (1001) docker     (127)     1210 2024-05-29 12:24:48.000000 apysc-4.4.3/apysc/_material_design/icon/material_fiber_manual_record_outlined_icon.py
+-rw-r--r--   0 runner    (1001) docker     (127)     1422 2024-05-29 12:24:48.000000 apysc-4.4.3/apysc/_material_design/icon/material_fiber_new_icon.py
+-rw-r--r--   0 runner    (1001) docker     (127)     1262 2024-05-29 12:24:48.000000 apysc-4.4.3/apysc/_material_design/icon/material_fiber_new_outlined_icon.py
+-rw-r--r--   0 runner    (1001) docker     (127)     1283 2024-05-29 12:24:48.000000 apysc-4.4.3/apysc/_material_design/icon/material_fiber_pin_icon.py
+-rw-r--r--   0 runner    (1001) docker     (127)     1221 2024-05-29 12:24:48.000000 apysc-4.4.3/apysc/_material_design/icon/material_fiber_pin_outlined_icon.py
+-rw-r--r--   0 runner    (1001) docker     (127)     1206 2024-05-29 12:24:48.000000 apysc-4.4.3/apysc/_material_design/icon/material_fiber_smart_record_icon.py
+-rw-r--r--   0 runner    (1001) docker     (127)     1314 2024-05-29 12:24:48.000000 apysc-4.4.3/apysc/_material_design/icon/material_fiber_smart_record_outlined_icon.py
+-rw-r--r--   0 runner    (1001) docker     (127)     1175 2024-05-29 12:24:48.000000 apysc-4.4.3/apysc/_material_design/icon/material_file_copy_icon.py
+-rw-r--r--   0 runner    (1001) docker     (127)     1199 2024-05-29 12:24:48.000000 apysc-4.4.3/apysc/_material_design/icon/material_file_copy_outlined_icon.py
+-rw-r--r--   0 runner    (1001) docker     (127)     1304 2024-05-29 12:24:48.000000 apysc-4.4.3/apysc/_material_design/icon/material_file_present_icon.py
+-rw-r--r--   0 runner    (1001) docker     (127)     1283 2024-05-29 12:24:48.000000 apysc-4.4.3/apysc/_material_design/icon/material_filter_alt_icon.py
+-rw-r--r--   0 runner    (1001) docker     (127)     1332 2024-05-29 12:24:48.000000 apysc-4.4.3/apysc/_material_design/icon/material_filter_alt_outlined_icon.py
+-rw-r--r--   0 runner    (1001) docker     (127)     1286 2024-05-29 12:24:48.000000 apysc-4.4.3/apysc/_material_design/icon/material_filter_list_alt_icon.py
+-rw-r--r--   0 runner    (1001) docker     (127)     1091 2024-05-29 12:24:48.000000 apysc-4.4.3/apysc/_material_design/icon/material_filter_list_icon.py
+-rw-r--r--   0 runner    (1001) docker     (127)     1119 2024-05-29 12:24:48.000000 apysc-4.4.3/apysc/_material_design/icon/material_filter_list_outlined_icon.py
+-rw-r--r--   0 runner    (1001) docker     (127)     1300 2024-05-29 12:24:48.000000 apysc-4.4.3/apysc/_material_design/icon/material_find_in_page_icon.py
+-rw-r--r--   0 runner    (1001) docker     (127)     1528 2024-05-29 12:24:48.000000 apysc-4.4.3/apysc/_material_design/icon/material_find_in_page_outlined_icon.py
+-rw-r--r--   0 runner    (1001) docker     (127)     1367 2024-05-29 12:24:48.000000 apysc-4.4.3/apysc/_material_design/icon/material_find_replace_icon.py
+-rw-r--r--   0 runner    (1001) docker     (127)     1395 2024-05-29 12:24:48.000000 apysc-4.4.3/apysc/_material_design/icon/material_find_replace_outlined_icon.py
+-rw-r--r--   0 runner    (1001) docker     (127)     2687 2024-05-29 12:24:48.000000 apysc-4.4.3/apysc/_material_design/icon/material_fingerprint_icon.py
+-rw-r--r--   0 runner    (1001) docker     (127)     2703 2024-05-29 12:24:48.000000 apysc-4.4.3/apysc/_material_design/icon/material_fingerprint_outlined_icon.py
+-rw-r--r--   0 runner    (1001) docker     (127)     1195 2024-05-29 12:24:48.000000 apysc-4.4.3/apysc/_material_design/icon/material_fit_screen_icon.py
+-rw-r--r--   0 runner    (1001) docker     (127)     1061 2024-05-29 12:24:48.000000 apysc-4.4.3/apysc/_material_design/icon/material_flag_icon.py
+-rw-r--r--   0 runner    (1001) docker     (127)     1131 2024-05-29 12:24:48.000000 apysc-4.4.3/apysc/_material_design/icon/material_flag_outlined_icon.py
+-rw-r--r--   0 runner    (1001) docker     (127)     1480 2024-05-29 12:24:48.000000 apysc-4.4.3/apysc/_material_design/icon/material_flaky_icon.py
+-rw-r--r--   0 runner    (1001) docker     (127)     1506 2024-05-29 12:24:48.000000 apysc-4.4.3/apysc/_material_design/icon/material_flaky_outlined_icon.py
+-rw-r--r--   0 runner    (1001) docker     (127)     1287 2024-05-29 12:24:48.000000 apysc-4.4.3/apysc/_material_design/icon/material_flight_land_icon.py
+-rw-r--r--   0 runner    (1001) docker     (127)     1234 2024-05-29 12:24:48.000000 apysc-4.4.3/apysc/_material_design/icon/material_flight_land_outlined_icon.py
+-rw-r--r--   0 runner    (1001) docker     (127)     1326 2024-05-29 12:24:48.000000 apysc-4.4.3/apysc/_material_design/icon/material_flight_takeoff_icon.py
+-rw-r--r--   0 runner    (1001) docker     (127)     1254 2024-05-29 12:24:48.000000 apysc-4.4.3/apysc/_material_design/icon/material_flight_takeoff_outlined_icon.py
+-rw-r--r--   0 runner    (1001) docker     (127)     1303 2024-05-29 12:24:48.000000 apysc-4.4.3/apysc/_material_design/icon/material_flip_to_back_icon.py
+-rw-r--r--   0 runner    (1001) docker     (127)     1331 2024-05-29 12:24:48.000000 apysc-4.4.3/apysc/_material_design/icon/material_flip_to_back_outlined_icon.py
+-rw-r--r--   0 runner    (1001) docker     (127)     1259 2024-05-29 12:24:48.000000 apysc-4.4.3/apysc/_material_design/icon/material_flip_to_front_icon.py
+-rw-r--r--   0 runner    (1001) docker     (127)     1287 2024-05-29 12:24:48.000000 apysc-4.4.3/apysc/_material_design/icon/material_flip_to_front_outlined_icon.py
+-rw-r--r--   0 runner    (1001) docker     (127)     1237 2024-05-29 12:24:48.000000 apysc-4.4.3/apysc/_material_design/icon/material_font_download_icon.py
+-rw-r--r--   0 runner    (1001) docker     (127)     1267 2024-05-29 12:24:48.000000 apysc-4.4.3/apysc/_material_design/icon/material_font_download_outlined_icon.py
+-rw-r--r--   0 runner    (1001) docker     (127)     1152 2024-05-29 12:24:48.000000 apysc-4.4.3/apysc/_material_design/icon/material_forum_icon.py
+-rw-r--r--   0 runner    (1001) docker     (127)     1203 2024-05-29 12:24:48.000000 apysc-4.4.3/apysc/_material_design/icon/material_forum_outlined_icon.py
+-rw-r--r--   0 runner    (1001) docker     (127)     1601 2024-05-29 12:24:48.000000 apysc-4.4.3/apysc/_material_design/icon/material_forward_10_icon.py
+-rw-r--r--   0 runner    (1001) docker     (127)     2167 2024-05-29 12:24:48.000000 apysc-4.4.3/apysc/_material_design/icon/material_forward_10_outlined_icon.py
+-rw-r--r--   0 runner    (1001) docker     (127)     1878 2024-05-29 12:24:48.000000 apysc-4.4.3/apysc/_material_design/icon/material_forward_30_icon.py
+-rw-r--r--   0 runner    (1001) docker     (127)     2407 2024-05-29 12:24:48.000000 apysc-4.4.3/apysc/_material_design/icon/material_forward_30_outlined_icon.py
+-rw-r--r--   0 runner    (1001) docker     (127)     1528 2024-05-29 12:24:48.000000 apysc-4.4.3/apysc/_material_design/icon/material_forward_5_icon.py
+-rw-r--r--   0 runner    (1001) docker     (127)     1699 2024-05-29 12:24:48.000000 apysc-4.4.3/apysc/_material_design/icon/material_forward_5_outlined_icon.py
+-rw-r--r--   0 runner    (1001) docker     (127)     1057 2024-05-29 12:24:48.000000 apysc-4.4.3/apysc/_material_design/icon/material_forward_icon.py
+-rw-r--r--   0 runner    (1001) docker     (127)     1127 2024-05-29 12:24:48.000000 apysc-4.4.3/apysc/_material_design/icon/material_forward_outlined_icon.py
+-rw-r--r--   0 runner    (1001) docker     (127)     1243 2024-05-29 12:24:48.000000 apysc-4.4.3/apysc/_material_design/icon/material_forward_to_inbox_icon.py
+-rw-r--r--   0 runner    (1001) docker     (127)     1269 2024-05-29 12:24:48.000000 apysc-4.4.3/apysc/_material_design/icon/material_forward_to_inbox_outlined_icon.py
+-rw-r--r--   0 runner    (1001) docker     (127)     1624 2024-05-29 12:24:48.000000 apysc-4.4.3/apysc/_material_design/icon/material_g_translate_icon.py
+-rw-r--r--   0 runner    (1001) docker     (127)     1726 2024-05-29 12:24:48.000000 apysc-4.4.3/apysc/_material_design/icon/material_g_translate_outlined_icon.py
+-rw-r--r--   0 runner    (1001) docker     (127)     1129 2024-05-29 12:24:48.000000 apysc-4.4.3/apysc/_material_design/icon/material_games_icon.py
+-rw-r--r--   0 runner    (1001) docker     (127)     1256 2024-05-29 12:24:48.000000 apysc-4.4.3/apysc/_material_design/icon/material_games_outlined_icon.py
+-rw-r--r--   0 runner    (1001) docker     (127)     1455 2024-05-29 12:24:48.000000 apysc-4.4.3/apysc/_material_design/icon/material_gavel_icon.py
+-rw-r--r--   0 runner    (1001) docker     (127)     1221 2024-05-29 12:24:48.000000 apysc-4.4.3/apysc/_material_design/icon/material_gavel_outlined_icon.py
+-rw-r--r--   0 runner    (1001) docker     (127)     1687 2024-05-29 12:24:48.000000 apysc-4.4.3/apysc/_material_design/icon/material_gesture_icon.py
+-rw-r--r--   0 runner    (1001) docker     (127)     1715 2024-05-29 12:24:48.000000 apysc-4.4.3/apysc/_material_design/icon/material_gesture_outlined_icon.py
+-rw-r--r--   0 runner    (1001) docker     (127)     1074 2024-05-29 12:24:48.000000 apysc-4.4.3/apysc/_material_design/icon/material_get_app_icon.py
+-rw-r--r--   0 runner    (1001) docker     (127)     1137 2024-05-29 12:24:48.000000 apysc-4.4.3/apysc/_material_design/icon/material_get_app_outlined_icon.py
+-rw-r--r--   0 runner    (1001) docker     (127)     1322 2024-05-29 12:24:48.000000 apysc-4.4.3/apysc/_material_design/icon/material_gif_icon.py
+-rw-r--r--   0 runner    (1001) docker     (127)     1198 2024-05-29 12:24:48.000000 apysc-4.4.3/apysc/_material_design/icon/material_gif_outlined_icon.py
+-rw-r--r--   0 runner    (1001) docker     (127)     1116 2024-05-29 12:24:48.000000 apysc-4.4.3/apysc/_material_design/icon/material_grade_icon.py
+-rw-r--r--   0 runner    (1001) docker     (127)     1324 2024-05-29 12:24:48.000000 apysc-4.4.3/apysc/_material_design/icon/material_grade_outlined_icon.py
+-rw-r--r--   0 runner    (1001) docker     (127)     1242 2024-05-29 12:24:48.000000 apysc-4.4.3/apysc/_material_design/icon/material_grading_icon.py
+-rw-r--r--   0 runner    (1001) docker     (127)     1268 2024-05-29 12:24:48.000000 apysc-4.4.3/apysc/_material_design/icon/material_grading_outlined_icon.py
+-rw-r--r--   0 runner    (1001) docker     (127)     1357 2024-05-29 12:24:48.000000 apysc-4.4.3/apysc/_material_design/icon/material_group_work_icon.py
+-rw-r--r--   0 runner    (1001) docker     (127)     1285 2024-05-29 12:24:48.000000 apysc-4.4.3/apysc/_material_design/icon/material_group_work_outlined_icon.py
+-rw-r--r--   0 runner    (1001) docker     (127)     1202 2024-05-29 12:24:48.000000 apysc-4.4.3/apysc/_material_design/icon/material_hd_icon.py
+-rw-r--r--   0 runner    (1001) docker     (127)     1247 2024-05-29 12:24:48.000000 apysc-4.4.3/apysc/_material_design/icon/material_hd_outlined_icon.py
+-rw-r--r--   0 runner    (1001) docker     (127)     1909 2024-05-29 12:24:48.000000 apysc-4.4.3/apysc/_material_design/icon/material_hearing_disabled_icon.py
+-rw-r--r--   0 runner    (1001) docker     (127)     1935 2024-05-29 12:24:48.000000 apysc-4.4.3/apysc/_material_design/icon/material_hearing_disabled_outlined_icon.py
+-rw-r--r--   0 runner    (1001) docker     (127)     1585 2024-05-29 12:24:48.000000 apysc-4.4.3/apysc/_material_design/icon/material_hearing_icon.py
+-rw-r--r--   0 runner    (1001) docker     (127)     1613 2024-05-29 12:24:48.000000 apysc-4.4.3/apysc/_material_design/icon/material_hearing_outlined_icon.py
+-rw-r--r--   0 runner    (1001) docker     (127)     1589 2024-05-29 12:24:48.000000 apysc-4.4.3/apysc/_material_design/icon/material_help_center_icon.py
+-rw-r--r--   0 runner    (1001) docker     (127)     1636 2024-05-29 12:24:48.000000 apysc-4.4.3/apysc/_material_design/icon/material_help_center_outlined_icon.py
+-rw-r--r--   0 runner    (1001) docker     (127)     1293 2024-05-29 12:24:48.000000 apysc-4.4.3/apysc/_material_design/icon/material_help_icon.py
+-rw-r--r--   0 runner    (1001) docker     (127)     1291 2024-05-29 12:24:48.000000 apysc-4.4.3/apysc/_material_design/icon/material_help_outline_icon.py
+-rw-r--r--   0 runner    (1001) docker     (127)     1319 2024-05-29 12:24:48.000000 apysc-4.4.3/apysc/_material_design/icon/material_help_outline_outlined_icon.py
+-rw-r--r--   0 runner    (1001) docker     (127)     1321 2024-05-29 12:24:48.000000 apysc-4.4.3/apysc/_material_design/icon/material_help_outlined_icon.py
+-rw-r--r--   0 runner    (1001) docker     (127)     1281 2024-05-29 12:24:48.000000 apysc-4.4.3/apysc/_material_design/icon/material_high_quality_icon.py
+-rw-r--r--   0 runner    (1001) docker     (127)     1323 2024-05-29 12:24:48.000000 apysc-4.4.3/apysc/_material_design/icon/material_high_quality_outlined_icon.py
+-rw-r--r--   0 runner    (1001) docker     (127)     1325 2024-05-29 12:24:48.000000 apysc-4.4.3/apysc/_material_design/icon/material_highlight_alt_icon.py
+-rw-r--r--   0 runner    (1001) docker     (127)     1434 2024-05-29 12:24:48.000000 apysc-4.4.3/apysc/_material_design/icon/material_highlight_alt_outlined_icon.py
+-rw-r--r--   0 runner    (1001) docker     (127)     1284 2024-05-29 12:24:48.000000 apysc-4.4.3/apysc/_material_design/icon/material_highlight_off_icon.py
+-rw-r--r--   0 runner    (1001) docker     (127)     1312 2024-05-29 12:24:48.000000 apysc-4.4.3/apysc/_material_design/icon/material_highlight_off_outlined_icon.py
+-rw-r--r--   0 runner    (1001) docker     (127)     1258 2024-05-29 12:24:48.000000 apysc-4.4.3/apysc/_material_design/icon/material_history_icon.py
+-rw-r--r--   0 runner    (1001) docker     (127)     1284 2024-05-29 12:24:48.000000 apysc-4.4.3/apysc/_material_design/icon/material_history_outlined_icon.py
+-rw-r--r--   0 runner    (1001) docker     (127)     2216 2024-05-29 12:24:48.000000 apysc-4.4.3/apysc/_material_design/icon/material_history_toggle_off_icon.py
+-rw-r--r--   0 runner    (1001) docker     (127)     2242 2024-05-29 12:24:48.000000 apysc-4.4.3/apysc/_material_design/icon/material_history_toggle_off_outlined_icon.py
+-rw-r--r--   0 runner    (1001) docker     (127)     1071 2024-05-29 12:24:48.000000 apysc-4.4.3/apysc/_material_design/icon/material_home_filled_icon.py
+-rw-r--r--   0 runner    (1001) docker     (127)     1060 2024-05-29 12:24:48.000000 apysc-4.4.3/apysc/_material_design/icon/material_home_icon.py
+-rw-r--r--   0 runner    (1001) docker     (127)     1130 2024-05-29 12:24:48.000000 apysc-4.4.3/apysc/_material_design/icon/material_home_outlined_icon.py
+-rw-r--r--   0 runner    (1001) docker     (127)     1106 2024-05-29 12:24:48.000000 apysc-4.4.3/apysc/_material_design/icon/material_horizontal_split_icon.py
+-rw-r--r--   0 runner    (1001) docker     (127)     1148 2024-05-29 12:24:48.000000 apysc-4.4.3/apysc/_material_design/icon/material_horizontal_split_outlined_icon.py
+-rw-r--r--   0 runner    (1001) docker     (127)     1198 2024-05-29 12:24:48.000000 apysc-4.4.3/apysc/_material_design/icon/material_hourglass_bottom_icon.py
+-rw-r--r--   0 runner    (1001) docker     (127)     1224 2024-05-29 12:24:48.000000 apysc-4.4.3/apysc/_material_design/icon/material_hourglass_bottom_outlined_icon.py
+-rw-r--r--   0 runner    (1001) docker     (127)     1351 2024-05-29 12:24:48.000000 apysc-4.4.3/apysc/_material_design/icon/material_hourglass_disabled_icon.py
+-rw-r--r--   0 runner    (1001) docker     (127)     1377 2024-05-29 12:24:48.000000 apysc-4.4.3/apysc/_material_design/icon/material_hourglass_disabled_outlined_icon.py
+-rw-r--r--   0 runner    (1001) docker     (127)     1198 2024-05-29 12:24:48.000000 apysc-4.4.3/apysc/_material_design/icon/material_hourglass_empty_icon.py
+-rw-r--r--   0 runner    (1001) docker     (127)     1224 2024-05-29 12:24:48.000000 apysc-4.4.3/apysc/_material_design/icon/material_hourglass_empty_outlined_icon.py
+-rw-r--r--   0 runner    (1001) docker     (127)     1144 2024-05-29 12:24:48.000000 apysc-4.4.3/apysc/_material_design/icon/material_hourglass_full_icon.py
+-rw-r--r--   0 runner    (1001) docker     (127)     1170 2024-05-29 12:24:48.000000 apysc-4.4.3/apysc/_material_design/icon/material_hourglass_full_outlined_icon.py
+-rw-r--r--   0 runner    (1001) docker     (127)     1192 2024-05-29 12:24:48.000000 apysc-4.4.3/apysc/_material_design/icon/material_hourglass_top_icon.py
+-rw-r--r--   0 runner    (1001) docker     (127)     1218 2024-05-29 12:24:48.000000 apysc-4.4.3/apysc/_material_design/icon/material_hourglass_top_outlined_icon.py
+-rw-r--r--   0 runner    (1001) docker     (127)     1275 2024-05-29 12:24:48.000000 apysc-4.4.3/apysc/_material_design/icon/material_how_to_reg_icon.py
+-rw-r--r--   0 runner    (1001) docker     (127)     1323 2024-05-29 12:24:48.000000 apysc-4.4.3/apysc/_material_design/icon/material_how_to_reg_outlined_icon.py
+-rw-r--r--   0 runner    (1001) docker     (127)     1340 2024-05-29 12:24:48.000000 apysc-4.4.3/apysc/_material_design/icon/material_how_to_vote_icon.py
+-rw-r--r--   0 runner    (1001) docker     (127)     1384 2024-05-29 12:24:48.000000 apysc-4.4.3/apysc/_material_design/icon/material_how_to_vote_outlined_icon.py
+-rw-r--r--   0 runner    (1001) docker     (127)     1222 2024-05-29 12:24:48.000000 apysc-4.4.3/apysc/_material_design/icon/material_http_icon.py
+-rw-r--r--   0 runner    (1001) docker     (127)     1262 2024-05-29 12:24:48.000000 apysc-4.4.3/apysc/_material_design/icon/material_http_outlined_icon.py
+-rw-r--r--   0 runner    (1001) docker     (127)     1253 2024-05-29 12:24:48.000000 apysc-4.4.3/apysc/_material_design/icon/material_https_icon.py
+-rw-r--r--   0 runner    (1001) docker     (127)     1275 2024-05-29 12:24:48.000000 apysc-4.4.3/apysc/_material_design/icon/material_https_outlined_icon.py
+-rw-r--r--   0 runner    (1001) docker     (127)     1514 2024-05-29 12:24:48.000000 apysc-4.4.3/apysc/_material_design/icon/material_import_contacts_icon.py
+-rw-r--r--   0 runner    (1001) docker     (127)     1472 2024-05-29 12:24:48.000000 apysc-4.4.3/apysc/_material_design/icon/material_import_contacts_outlined_icon.py
+-rw-r--r--   0 runner    (1001) docker     (127)     1120 2024-05-29 12:24:48.000000 apysc-4.4.3/apysc/_material_design/icon/material_import_export_icon.py
+-rw-r--r--   0 runner    (1001) docker     (127)     1148 2024-05-29 12:24:48.000000 apysc-4.4.3/apysc/_material_design/icon/material_import_export_outlined_icon.py
+-rw-r--r--   0 runner    (1001) docker     (127)     1349 2024-05-29 12:24:48.000000 apysc-4.4.3/apysc/_material_design/icon/material_important_devices_icon.py
+-rw-r--r--   0 runner    (1001) docker     (127)     1375 2024-05-29 12:24:48.000000 apysc-4.4.3/apysc/_material_design/icon/material_important_devices_outlined_icon.py
+-rw-r--r--   0 runner    (1001) docker     (127)     1175 2024-05-29 12:24:48.000000 apysc-4.4.3/apysc/_material_design/icon/material_inbox_icon.py
+-rw-r--r--   0 runner    (1001) docker     (127)     1238 2024-05-29 12:24:48.000000 apysc-4.4.3/apysc/_material_design/icon/material_inbox_outlined_icon.py
+-rw-r--r--   0 runner    (1001) docker     (127)     1121 2024-05-29 12:24:48.000000 apysc-4.4.3/apysc/_material_design/icon/material_info_icon.py
+-rw-r--r--   0 runner    (1001) docker     (127)     1256 2024-05-29 12:24:48.000000 apysc-4.4.3/apysc/_material_design/icon/material_info_outline_icon.py
+-rw-r--r--   0 runner    (1001) docker     (127)     1201 2024-05-29 12:24:48.000000 apysc-4.4.3/apysc/_material_design/icon/material_info_outlined_icon.py
+-rw-r--r--   0 runner    (1001) docker     (127)     1173 2024-05-29 12:24:48.000000 apysc-4.4.3/apysc/_material_design/icon/material_input_icon.py
+-rw-r--r--   0 runner    (1001) docker     (127)     1394 2024-05-29 12:24:48.000000 apysc-4.4.3/apysc/_material_design/icon/material_input_outlined_icon.py
+-rw-r--r--   0 runner    (1001) docker     (127)     1613 2024-05-29 12:24:48.000000 apysc-4.4.3/apysc/_material_design/icon/material_insights_icon.py
+-rw-r--r--   0 runner    (1001) docker     (127)     1639 2024-05-29 12:24:48.000000 apysc-4.4.3/apysc/_material_design/icon/material_insights_outlined_icon.py
+-rw-r--r--   0 runner    (1001) docker     (127)     1810 2024-05-29 12:24:48.000000 apysc-4.4.3/apysc/_material_design/icon/material_integration_instructions_icon.py
+-rw-r--r--   0 runner    (1001) docker     (127)     1921 2024-05-29 12:24:48.000000 apysc-4.4.3/apysc/_material_design/icon/material_integration_instructions_outlined_icon.py
+-rw-r--r--   0 runner    (1001) docker     (127)     1201 2024-05-29 12:24:48.000000 apysc-4.4.3/apysc/_material_design/icon/material_inventory_icon.py
+-rw-r--r--   0 runner    (1001) docker     (127)     1288 2024-05-29 12:24:48.000000 apysc-4.4.3/apysc/_material_design/icon/material_invert_colors_icon.py
+-rw-r--r--   0 runner    (1001) docker     (127)     1450 2024-05-29 12:24:48.000000 apysc-4.4.3/apysc/_material_design/icon/material_invert_colors_off_icon.py
+-rw-r--r--   0 runner    (1001) docker     (127)     1417 2024-05-29 12:24:48.000000 apysc-4.4.3/apysc/_material_design/icon/material_invert_colors_off_outlined_icon.py
+-rw-r--r--   0 runner    (1001) docker     (127)     1309 2024-05-29 12:24:48.000000 apysc-4.4.3/apysc/_material_design/icon/material_invert_colors_outlined_icon.py
+-rw-r--r--   0 runner    (1001) docker     (127)     1160 2024-05-29 12:24:48.000000 apysc-4.4.3/apysc/_material_design/icon/material_label_icon.py
+-rw-r--r--   0 runner    (1001) docker     (127)     1172 2024-05-29 12:24:48.000000 apysc-4.4.3/apysc/_material_design/icon/material_label_important_icon.py
+-rw-r--r--   0 runner    (1001) docker     (127)     1204 2024-05-29 12:24:48.000000 apysc-4.4.3/apysc/_material_design/icon/material_label_important_outline_icon.py
+-rw-r--r--   0 runner    (1001) docker     (127)     1175 2024-05-29 12:24:48.000000 apysc-4.4.3/apysc/_material_design/icon/material_label_important_outlined_icon.py
+-rw-r--r--   0 runner    (1001) docker     (127)     1179 2024-05-29 12:24:48.000000 apysc-4.4.3/apysc/_material_design/icon/material_label_off_icon.py
+-rw-r--r--   0 runner    (1001) docker     (127)     1311 2024-05-29 12:24:48.000000 apysc-4.4.3/apysc/_material_design/icon/material_label_off_outlined_icon.py
+-rw-r--r--   0 runner    (1001) docker     (127)     1210 2024-05-29 12:24:48.000000 apysc-4.4.3/apysc/_material_design/icon/material_label_outline_icon.py
+-rw-r--r--   0 runner    (1001) docker     (127)     1215 2024-05-29 12:24:48.000000 apysc-4.4.3/apysc/_material_design/icon/material_label_outlined_icon.py
+-rw-r--r--   0 runner    (1001) docker     (127)     1846 2024-05-29 12:24:48.000000 apysc-4.4.3/apysc/_material_design/icon/material_language_icon.py
+-rw-r--r--   0 runner    (1001) docker     (127)     1854 2024-05-29 12:24:48.000000 apysc-4.4.3/apysc/_material_design/icon/material_language_outlined_icon.py
+-rw-r--r--   0 runner    (1001) docker     (127)     1161 2024-05-29 12:24:48.000000 apysc-4.4.3/apysc/_material_design/icon/material_launch_icon.py
+-rw-r--r--   0 runner    (1001) docker     (127)     1189 2024-05-29 12:24:48.000000 apysc-4.4.3/apysc/_material_design/icon/material_launch_outlined_icon.py
+-rw-r--r--   0 runner    (1001) docker     (127)     1157 2024-05-29 12:24:48.000000 apysc-4.4.3/apysc/_material_design/icon/material_leaderboard_icon.py
+-rw-r--r--   0 runner    (1001) docker     (127)     1197 2024-05-29 12:24:48.000000 apysc-4.4.3/apysc/_material_design/icon/material_leaderboard_outlined_icon.py
+-rw-r--r--   0 runner    (1001) docker     (127)     1232 2024-05-29 12:24:48.000000 apysc-4.4.3/apysc/_material_design/icon/material_library_add_check_icon.py
+-rw-r--r--   0 runner    (1001) docker     (127)     1334 2024-05-29 12:24:48.000000 apysc-4.4.3/apysc/_material_design/icon/material_library_add_check_outlined_icon.py
+-rw-r--r--   0 runner    (1001) docker     (127)     1188 2024-05-29 12:24:48.000000 apysc-4.4.3/apysc/_material_design/icon/material_library_add_icon.py
+-rw-r--r--   0 runner    (1001) docker     (127)     1231 2024-05-29 12:24:48.000000 apysc-4.4.3/apysc/_material_design/icon/material_library_add_outlined_icon.py
+-rw-r--r--   0 runner    (1001) docker     (127)     1205 2024-05-29 12:24:48.000000 apysc-4.4.3/apysc/_material_design/icon/material_library_books_icon.py
+-rw-r--r--   0 runner    (1001) docker     (127)     1242 2024-05-29 12:24:48.000000 apysc-4.4.3/apysc/_material_design/icon/material_library_books_outlined_icon.py
+-rw-r--r--   0 runner    (1001) docker     (127)     1259 2024-05-29 12:24:48.000000 apysc-4.4.3/apysc/_material_design/icon/material_library_music_icon.py
+-rw-r--r--   0 runner    (1001) docker     (127)     1317 2024-05-29 12:24:48.000000 apysc-4.4.3/apysc/_material_design/icon/material_library_music_outlined_icon.py
+-rw-r--r--   0 runner    (1001) docker     (127)     1197 2024-05-29 12:24:48.000000 apysc-4.4.3/apysc/_material_design/icon/material_lightbulb_icon.py
+-rw-r--r--   0 runner    (1001) docker     (127)     1427 2024-05-29 12:24:48.000000 apysc-4.4.3/apysc/_material_design/icon/material_lightbulb_outline_icon.py
+-rw-r--r--   0 runner    (1001) docker     (127)     1356 2024-05-29 12:24:48.000000 apysc-4.4.3/apysc/_material_design/icon/material_lightbulb_outlined_icon.py
+-rw-r--r--   0 runner    (1001) docker     (127)     1307 2024-05-29 12:24:48.000000 apysc-4.4.3/apysc/_material_design/icon/material_line_style_icon.py
+-rw-r--r--   0 runner    (1001) docker     (127)     1236 2024-05-29 12:24:48.000000 apysc-4.4.3/apysc/_material_design/icon/material_line_style_outlined_icon.py
+-rw-r--r--   0 runner    (1001) docker     (127)     1186 2024-05-29 12:24:48.000000 apysc-4.4.3/apysc/_material_design/icon/material_line_weight_icon.py
+-rw-r--r--   0 runner    (1001) docker     (127)     1131 2024-05-29 12:24:48.000000 apysc-4.4.3/apysc/_material_design/icon/material_line_weight_outlined_icon.py
+-rw-r--r--   0 runner    (1001) docker     (127)     1236 2024-05-29 12:24:48.000000 apysc-4.4.3/apysc/_material_design/icon/material_link_icon.py
+-rw-r--r--   0 runner    (1001) docker     (127)     1390 2024-05-29 12:24:48.000000 apysc-4.4.3/apysc/_material_design/icon/material_link_off_icon.py
+-rw-r--r--   0 runner    (1001) docker     (127)     1393 2024-05-29 12:24:48.000000 apysc-4.4.3/apysc/_material_design/icon/material_link_off_outlined_icon.py
+-rw-r--r--   0 runner    (1001) docker     (127)     1224 2024-05-29 12:24:48.000000 apysc-4.4.3/apysc/_material_design/icon/material_link_outlined_icon.py
+-rw-r--r--   0 runner    (1001) docker     (127)     1213 2024-05-29 12:24:48.000000 apysc-4.4.3/apysc/_material_design/icon/material_list_alt_icon.py
+-rw-r--r--   0 runner    (1001) docker     (127)     1239 2024-05-29 12:24:48.000000 apysc-4.4.3/apysc/_material_design/icon/material_list_alt_outlined_icon.py
+-rw-r--r--   0 runner    (1001) docker     (127)     1111 2024-05-29 12:24:48.000000 apysc-4.4.3/apysc/_material_design/icon/material_list_icon.py
+-rw-r--r--   0 runner    (1001) docker     (127)     1273 2024-05-29 12:24:48.000000 apysc-4.4.3/apysc/_material_design/icon/material_list_outlined_icon.py
+-rw-r--r--   0 runner    (1001) docker     (127)     1329 2024-05-29 12:24:48.000000 apysc-4.4.3/apysc/_material_design/icon/material_live_help_icon.py
+-rw-r--r--   0 runner    (1001) docker     (127)     1324 2024-05-29 12:24:48.000000 apysc-4.4.3/apysc/_material_design/icon/material_live_help_outlined_icon.py
+-rw-r--r--   0 runner    (1001) docker     (127)     1381 2024-05-29 12:24:48.000000 apysc-4.4.3/apysc/_material_design/icon/material_location_off_icon.py
+-rw-r--r--   0 runner    (1001) docker     (127)     1511 2024-05-29 12:24:48.000000 apysc-4.4.3/apysc/_material_design/icon/material_location_off_outlined_icon.py
+-rw-r--r--   0 runner    (1001) docker     (127)     1199 2024-05-29 12:24:48.000000 apysc-4.4.3/apysc/_material_design/icon/material_location_on_icon.py
+-rw-r--r--   0 runner    (1001) docker     (127)     1257 2024-05-29 12:24:48.000000 apysc-4.4.3/apysc/_material_design/icon/material_location_on_outlined_icon.py
+-rw-r--r--   0 runner    (1001) docker     (127)     1383 2024-05-29 12:24:48.000000 apysc-4.4.3/apysc/_material_design/icon/material_lock_clock_icon.py
+-rw-r--r--   0 runner    (1001) docker     (127)     1250 2024-05-29 12:24:48.000000 apysc-4.4.3/apysc/_material_design/icon/material_lock_icon.py
+-rw-r--r--   0 runner    (1001) docker     (127)     1270 2024-05-29 12:24:48.000000 apysc-4.4.3/apysc/_material_design/icon/material_lock_open_icon.py
+-rw-r--r--   0 runner    (1001) docker     (127)     1277 2024-05-29 12:24:48.000000 apysc-4.4.3/apysc/_material_design/icon/material_lock_open_outlined_icon.py
+-rw-r--r--   0 runner    (1001) docker     (127)     1380 2024-05-29 12:24:48.000000 apysc-4.4.3/apysc/_material_design/icon/material_lock_outline_icon.py
+-rw-r--r--   0 runner    (1001) docker     (127)     1320 2024-05-29 12:24:48.000000 apysc-4.4.3/apysc/_material_design/icon/material_lock_outlined_icon.py
+-rw-r--r--   0 runner    (1001) docker     (127)     1195 2024-05-29 12:24:48.000000 apysc-4.4.3/apysc/_material_design/icon/material_login_icon.py
+-rw-r--r--   0 runner    (1001) docker     (127)     1221 2024-05-29 12:24:48.000000 apysc-4.4.3/apysc/_material_design/icon/material_login_outlined_icon.py
+-rw-r--r--   0 runner    (1001) docker     (127)     1141 2024-05-29 12:24:48.000000 apysc-4.4.3/apysc/_material_design/icon/material_logout_icon.py
+-rw-r--r--   0 runner    (1001) docker     (127)     1248 2024-05-29 12:24:48.000000 apysc-4.4.3/apysc/_material_design/icon/material_loop_icon.py
+-rw-r--r--   0 runner    (1001) docker     (127)     1276 2024-05-29 12:24:48.000000 apysc-4.4.3/apysc/_material_design/icon/material_loop_outlined_icon.py
+-rw-r--r--   0 runner    (1001) docker     (127)     1204 2024-05-29 12:24:48.000000 apysc-4.4.3/apysc/_material_design/icon/material_low_priority_icon.py
+-rw-r--r--   0 runner    (1001) docker     (127)     1240 2024-05-29 12:24:48.000000 apysc-4.4.3/apysc/_material_design/icon/material_low_priority_outlined_icon.py
+-rw-r--r--   0 runner    (1001) docker     (127)     1474 2024-05-29 12:24:48.000000 apysc-4.4.3/apysc/_material_design/icon/material_loyalty_icon.py
+-rw-r--r--   0 runner    (1001) docker     (127)     1497 2024-05-29 12:24:48.000000 apysc-4.4.3/apysc/_material_design/icon/material_loyalty_outlined_icon.py
+-rw-r--r--   0 runner    (1001) docker     (127)     1134 2024-05-29 12:24:48.000000 apysc-4.4.3/apysc/_material_design/icon/material_mail_icon.py
+-rw-r--r--   0 runner    (1001) docker     (127)     1170 2024-05-29 12:24:48.000000 apysc-4.4.3/apysc/_material_design/icon/material_mail_outline_icon.py
+-rw-r--r--   0 runner    (1001) docker     (127)     1198 2024-05-29 12:24:48.000000 apysc-4.4.3/apysc/_material_design/icon/material_mail_outline_outlined_icon.py
+-rw-r--r--   0 runner    (1001) docker     (127)     1171 2024-05-29 12:24:48.000000 apysc-4.4.3/apysc/_material_design/icon/material_mail_outlined_icon.py
+-rw-r--r--   0 runner    (1001) docker     (127)     1287 2024-05-29 12:24:48.000000 apysc-4.4.3/apysc/_material_design/icon/material_mark_as_unread_icon.py
+-rw-r--r--   0 runner    (1001) docker     (127)     1325 2024-05-29 12:24:48.000000 apysc-4.4.3/apysc/_material_design/icon/material_mark_chat_read_icon.py
+-rw-r--r--   0 runner    (1001) docker     (127)     1274 2024-05-29 12:24:48.000000 apysc-4.4.3/apysc/_material_design/icon/material_mark_chat_read_outlined_icon.py
+-rw-r--r--   0 runner    (1001) docker     (127)     1300 2024-05-29 12:24:48.000000 apysc-4.4.3/apysc/_material_design/icon/material_mark_chat_unread_icon.py
+-rw-r--r--   0 runner    (1001) docker     (127)     1345 2024-05-29 12:24:48.000000 apysc-4.4.3/apysc/_material_design/icon/material_mark_chat_unread_outlined_icon.py
+-rw-r--r--   0 runner    (1001) docker     (127)     1342 2024-05-29 12:24:48.000000 apysc-4.4.3/apysc/_material_design/icon/material_mark_email_read_icon.py
+-rw-r--r--   0 runner    (1001) docker     (127)     1313 2024-05-29 12:24:48.000000 apysc-4.4.3/apysc/_material_design/icon/material_mark_email_read_outlined_icon.py
+-rw-r--r--   0 runner    (1001) docker     (127)     1370 2024-05-29 12:24:48.000000 apysc-4.4.3/apysc/_material_design/icon/material_mark_email_unread_icon.py
+-rw-r--r--   0 runner    (1001) docker     (127)     1417 2024-05-29 12:24:48.000000 apysc-4.4.3/apysc/_material_design/icon/material_mark_email_unread_outlined_icon.py
+-rw-r--r--   0 runner    (1001) docker     (127)     1152 2024-05-29 12:24:48.000000 apysc-4.4.3/apysc/_material_design/icon/material_markunread_icon.py
+-rw-r--r--   0 runner    (1001) docker     (127)     1183 2024-05-29 12:24:48.000000 apysc-4.4.3/apysc/_material_design/icon/material_markunread_mailbox_icon.py
+-rw-r--r--   0 runner    (1001) docker     (127)     1199 2024-05-29 12:24:48.000000 apysc-4.4.3/apysc/_material_design/icon/material_markunread_mailbox_outlined_icon.py
+-rw-r--r--   0 runner    (1001) docker     (127)     1186 2024-05-29 12:24:48.000000 apysc-4.4.3/apysc/_material_design/icon/material_markunread_outlined_icon.py
+-rw-r--r--   0 runner    (1001) docker     (127)     1051 2024-05-29 12:24:48.000000 apysc-4.4.3/apysc/_material_design/icon/material_maximize_icon.py
+-rw-r--r--   0 runner    (1001) docker     (127)     1079 2024-05-29 12:24:48.000000 apysc-4.4.3/apysc/_material_design/icon/material_maximize_outlined_icon.py
+-rw-r--r--   0 runner    (1001) docker     (127)     1454 2024-05-29 12:24:48.000000 apysc-4.4.3/apysc/_material_design/icon/material_mediation_icon.py
+-rw-r--r--   0 runner    (1001) docker     (127)     1500 2024-05-29 12:24:48.000000 apysc-4.4.3/apysc/_material_design/icon/material_mediation_outlined_icon.py
+-rw-r--r--   0 runner    (1001) docker     (127)     1152 2024-05-29 12:24:48.000000 apysc-4.4.3/apysc/_material_design/icon/material_message_icon.py
+-rw-r--r--   0 runner    (1001) docker     (127)     1203 2024-05-29 12:24:48.000000 apysc-4.4.3/apysc/_material_design/icon/material_message_outlined_icon.py
+-rw-r--r--   0 runner    (1001) docker     (127)     1213 2024-05-29 12:24:48.000000 apysc-4.4.3/apysc/_material_design/icon/material_mic_icon.py
+-rw-r--r--   0 runner    (1001) docker     (127)     1338 2024-05-29 12:24:48.000000 apysc-4.4.3/apysc/_material_design/icon/material_mic_none_icon.py
+-rw-r--r--   0 runner    (1001) docker     (127)     1300 2024-05-29 12:24:48.000000 apysc-4.4.3/apysc/_material_design/icon/material_mic_none_outlined_icon.py
+-rw-r--r--   0 runner    (1001) docker     (127)     1402 2024-05-29 12:24:48.000000 apysc-4.4.3/apysc/_material_design/icon/material_mic_off_icon.py
+-rw-r--r--   0 runner    (1001) docker     (127)     1463 2024-05-29 12:24:48.000000 apysc-4.4.3/apysc/_material_design/icon/material_mic_off_outlined_icon.py
+-rw-r--r--   0 runner    (1001) docker     (127)     1390 2024-05-29 12:24:48.000000 apysc-4.4.3/apysc/_material_design/icon/material_mic_outlined_icon.py
+-rw-r--r--   0 runner    (1001) docker     (127)     1052 2024-05-29 12:24:48.000000 apysc-4.4.3/apysc/_material_design/icon/material_minimize_icon.py
+-rw-r--r--   0 runner    (1001) docker     (127)     1081 2024-05-29 12:24:48.000000 apysc-4.4.3/apysc/_material_design/icon/material_minimize_outlined_icon.py
+-rw-r--r--   0 runner    (1001) docker     (127)     1239 2024-05-29 12:24:48.000000 apysc-4.4.3/apysc/_material_design/icon/material_missed_video_call_icon.py
+-rw-r--r--   0 runner    (1001) docker     (127)     1291 2024-05-29 12:24:48.000000 apysc-4.4.3/apysc/_material_design/icon/material_missed_video_call_outlined_icon.py
+-rw-r--r--   0 runner    (1001) docker     (127)     1274 2024-05-29 12:24:48.000000 apysc-4.4.3/apysc/_material_design/icon/material_mobile_screen_share_icon.py
+-rw-r--r--   0 runner    (1001) docker     (127)     1308 2024-05-29 12:24:48.000000 apysc-4.4.3/apysc/_material_design/icon/material_mobile_screen_share_outlined_icon.py
+-rw-r--r--   0 runner    (1001) docker     (127)     1511 2024-05-29 12:24:48.000000 apysc-4.4.3/apysc/_material_design/icon/material_model_training_icon.py
+-rw-r--r--   0 runner    (1001) docker     (127)     1537 2024-05-29 12:24:48.000000 apysc-4.4.3/apysc/_material_design/icon/material_model_training_outlined_icon.py
+-rw-r--r--   0 runner    (1001) docker     (127)     1438 2024-05-29 12:24:48.000000 apysc-4.4.3/apysc/_material_design/icon/material_more_time_icon.py
+-rw-r--r--   0 runner    (1001) docker     (127)     1464 2024-05-29 12:24:48.000000 apysc-4.4.3/apysc/_material_design/icon/material_more_time_outlined_icon.py
+-rw-r--r--   0 runner    (1001) docker     (127)     1221 2024-05-29 12:24:48.000000 apysc-4.4.3/apysc/_material_design/icon/material_move_to_inbox_icon.py
+-rw-r--r--   0 runner    (1001) docker     (127)     1298 2024-05-29 12:24:48.000000 apysc-4.4.3/apysc/_material_design/icon/material_move_to_inbox_outlined_icon.py
+-rw-r--r--   0 runner    (1001) docker     (127)     1138 2024-05-29 12:24:48.000000 apysc-4.4.3/apysc/_material_design/icon/material_movie_icon.py
+-rw-r--r--   0 runner    (1001) docker     (127)     1193 2024-05-29 12:24:48.000000 apysc-4.4.3/apysc/_material_design/icon/material_movie_outlined_icon.py
+-rw-r--r--   0 runner    (1001) docker     (127)     1241 2024-05-29 12:24:48.000000 apysc-4.4.3/apysc/_material_design/icon/material_music_video_icon.py
+-rw-r--r--   0 runner    (1001) docker     (127)     1267 2024-05-29 12:24:48.000000 apysc-4.4.3/apysc/_material_design/icon/material_music_video_outlined_icon.py
+-rw-r--r--   0 runner    (1001) docker     (127)     1377 2024-05-29 12:24:48.000000 apysc-4.4.3/apysc/_material_design/icon/material_nat_icon.py
+-rw-r--r--   0 runner    (1001) docker     (127)     1403 2024-05-29 12:24:48.000000 apysc-4.4.3/apysc/_material_design/icon/material_nat_outlined_icon.py
+-rw-r--r--   0 runner    (1001) docker     (127)     1256 2024-05-29 12:24:48.000000 apysc-4.4.3/apysc/_material_design/icon/material_new_releases_icon.py
+-rw-r--r--   0 runner    (1001) docker     (127)     1475 2024-05-29 12:24:48.000000 apysc-4.4.3/apysc/_material_design/icon/material_new_releases_outlined_icon.py
+-rw-r--r--   0 runner    (1001) docker     (127)     1337 2024-05-29 12:24:48.000000 apysc-4.4.3/apysc/_material_design/icon/material_next_plan_icon.py
+-rw-r--r--   0 runner    (1001) docker     (127)     1437 2024-05-29 12:24:48.000000 apysc-4.4.3/apysc/_material_design/icon/material_next_plan_outlined_icon.py
+-rw-r--r--   0 runner    (1001) docker     (127)     1329 2024-05-29 12:24:48.000000 apysc-4.4.3/apysc/_material_design/icon/material_next_week_icon.py
+-rw-r--r--   0 runner    (1001) docker     (127)     1278 2024-05-29 12:24:48.000000 apysc-4.4.3/apysc/_material_design/icon/material_next_week_outlined_icon.py
+-rw-r--r--   0 runner    (1001) docker     (127)     1277 2024-05-29 12:24:48.000000 apysc-4.4.3/apysc/_material_design/icon/material_nightlight_round_icon.py
+-rw-r--r--   0 runner    (1001) docker     (127)     1189 2024-05-29 12:24:48.000000 apysc-4.4.3/apysc/_material_design/icon/material_no_sim_icon.py
+-rw-r--r--   0 runner    (1001) docker     (127)     1260 2024-05-29 12:24:48.000000 apysc-4.4.3/apysc/_material_design/icon/material_no_sim_outlined_icon.py
+-rw-r--r--   0 runner    (1001) docker     (127)     1590 2024-05-29 12:24:48.000000 apysc-4.4.3/apysc/_material_design/icon/material_not_accessible_icon.py
+-rw-r--r--   0 runner    (1001) docker     (127)     1606 2024-05-29 12:24:48.000000 apysc-4.4.3/apysc/_material_design/icon/material_not_accessible_outlined_icon.py
+-rw-r--r--   0 runner    (1001) docker     (127)     1292 2024-05-29 12:24:48.000000 apysc-4.4.3/apysc/_material_design/icon/material_not_interested_icon.py
+-rw-r--r--   0 runner    (1001) docker     (127)     1320 2024-05-29 12:24:48.000000 apysc-4.4.3/apysc/_material_design/icon/material_not_interested_outlined_icon.py
+-rw-r--r--   0 runner    (1001) docker     (127)     1209 2024-05-29 12:24:48.000000 apysc-4.4.3/apysc/_material_design/icon/material_not_started_icon.py
+-rw-r--r--   0 runner    (1001) docker     (127)     1300 2024-05-29 12:24:48.000000 apysc-4.4.3/apysc/_material_design/icon/material_not_started_outlined_icon.py
+-rw-r--r--   0 runner    (1001) docker     (127)     1168 2024-05-29 12:24:48.000000 apysc-4.4.3/apysc/_material_design/icon/material_note_add_icon.py
+-rw-r--r--   0 runner    (1001) docker     (127)     1185 2024-05-29 12:24:48.000000 apysc-4.4.3/apysc/_material_design/icon/material_note_add_outlined_icon.py
+-rw-r--r--   0 runner    (1001) docker     (127)     1135 2024-05-29 12:24:48.000000 apysc-4.4.3/apysc/_material_design/icon/material_note_icon.py
+-rw-r--r--   0 runner    (1001) docker     (127)     1154 2024-05-29 12:24:48.000000 apysc-4.4.3/apysc/_material_design/icon/material_note_outlined_icon.py
+-rw-r--r--   0 runner    (1001) docker     (127)     1272 2024-05-29 12:24:48.000000 apysc-4.4.3/apysc/_material_design/icon/material_notification_important_icon.py
+-rw-r--r--   0 runner    (1001) docker     (127)     1332 2024-05-29 12:24:48.000000 apysc-4.4.3/apysc/_material_design/icon/material_notification_important_outlined_icon.py
+-rw-r--r--   0 runner    (1001) docker     (127)     1186 2024-05-29 12:24:48.000000 apysc-4.4.3/apysc/_material_design/icon/material_offline_bolt_icon.py
+-rw-r--r--   0 runner    (1001) docker     (127)     1300 2024-05-29 12:24:48.000000 apysc-4.4.3/apysc/_material_design/icon/material_offline_bolt_outlined_icon.py
+-rw-r--r--   0 runner    (1001) docker     (127)     1249 2024-05-29 12:24:48.000000 apysc-4.4.3/apysc/_material_design/icon/material_offline_pin_icon.py
+-rw-r--r--   0 runner    (1001) docker     (127)     1251 2024-05-29 12:24:48.000000 apysc-4.4.3/apysc/_material_design/icon/material_offline_pin_outlined_icon.py
+-rw-r--r--   0 runner    (1001) docker     (127)     1780 2024-05-29 12:24:48.000000 apysc-4.4.3/apysc/_material_design/icon/material_online_prediction_icon.py
+-rw-r--r--   0 runner    (1001) docker     (127)     1806 2024-05-29 12:24:48.000000 apysc-4.4.3/apysc/_material_design/icon/material_online_prediction_outlined_icon.py
+-rw-r--r--   0 runner    (1001) docker     (127)     1289 2024-05-29 12:24:48.000000 apysc-4.4.3/apysc/_material_design/icon/material_opacity_icon.py
+-rw-r--r--   0 runner    (1001) docker     (127)     1315 2024-05-29 12:24:48.000000 apysc-4.4.3/apysc/_material_design/icon/material_opacity_outlined_icon.py
+-rw-r--r--   0 runner    (1001) docker     (127)     1181 2024-05-29 12:24:48.000000 apysc-4.4.3/apysc/_material_design/icon/material_open_in_browser_icon.py
+-rw-r--r--   0 runner    (1001) docker     (127)     1209 2024-05-29 12:24:48.000000 apysc-4.4.3/apysc/_material_design/icon/material_open_in_browser_outlined_icon.py
+-rw-r--r--   0 runner    (1001) docker     (127)     1169 2024-05-29 12:24:48.000000 apysc-4.4.3/apysc/_material_design/icon/material_open_in_full_icon.py
+-rw-r--r--   0 runner    (1001) docker     (127)     1195 2024-05-29 12:24:48.000000 apysc-4.4.3/apysc/_material_design/icon/material_open_in_full_outlined_icon.py
+-rw-r--r--   0 runner    (1001) docker     (127)     1174 2024-05-29 12:24:48.000000 apysc-4.4.3/apysc/_material_design/icon/material_open_in_new_icon.py
+-rw-r--r--   0 runner    (1001) docker     (127)     1202 2024-05-29 12:24:48.000000 apysc-4.4.3/apysc/_material_design/icon/material_open_in_new_outlined_icon.py
+-rw-r--r--   0 runner    (1001) docker     (127)     1144 2024-05-29 12:24:48.000000 apysc-4.4.3/apysc/_material_design/icon/material_open_with_icon.py
+-rw-r--r--   0 runner    (1001) docker     (127)     1172 2024-05-29 12:24:48.000000 apysc-4.4.3/apysc/_material_design/icon/material_open_with_outlined_icon.py
+-rw-r--r--   0 runner    (1001) docker     (127)     1252 2024-05-29 12:24:48.000000 apysc-4.4.3/apysc/_material_design/icon/material_outbond_icon.py
+-rw-r--r--   0 runner    (1001) docker     (127)     1343 2024-05-29 12:24:48.000000 apysc-4.4.3/apysc/_material_design/icon/material_outbond_outlined_icon.py
+-rw-r--r--   0 runner    (1001) docker     (127)     1202 2024-05-29 12:24:48.000000 apysc-4.4.3/apysc/_material_design/icon/material_outbox_icon.py
+-rw-r--r--   0 runner    (1001) docker     (127)     1441 2024-05-29 12:24:48.000000 apysc-4.4.3/apysc/_material_design/icon/material_outgoing_mail_icon.py
+-rw-r--r--   0 runner    (1001) docker     (127)     1369 2024-05-29 12:24:48.000000 apysc-4.4.3/apysc/_material_design/icon/material_outlet_icon.py
+-rw-r--r--   0 runner    (1001) docker     (127)     1468 2024-05-29 12:24:48.000000 apysc-4.4.3/apysc/_material_design/icon/material_outlet_outlined_icon.py
+-rw-r--r--   0 runner    (1001) docker     (127)     1112 2024-05-29 12:24:48.000000 apysc-4.4.3/apysc/_material_design/icon/material_outlined_flag_icon.py
+-rw-r--r--   0 runner    (1001) docker     (127)     1140 2024-05-29 12:24:48.000000 apysc-4.4.3/apysc/_material_design/icon/material_outlined_flag_outlined_icon.py
+-rw-r--r--   0 runner    (1001) docker     (127)     1334 2024-05-29 12:24:48.000000 apysc-4.4.3/apysc/_material_design/icon/material_pageview_icon.py
+-rw-r--r--   0 runner    (1001) docker     (127)     1372 2024-05-29 12:24:48.000000 apysc-4.4.3/apysc/_material_design/icon/material_pageview_outlined_icon.py
+-rw-r--r--   0 runner    (1001) docker     (127)     1458 2024-05-29 12:24:48.000000 apysc-4.4.3/apysc/_material_design/icon/material_pan_tool_icon.py
+-rw-r--r--   0 runner    (1001) docker     (127)     1613 2024-05-29 12:24:48.000000 apysc-4.4.3/apysc/_material_design/icon/material_pan_tool_outlined_icon.py
+-rw-r--r--   0 runner    (1001) docker     (127)     1163 2024-05-29 12:24:48.000000 apysc-4.4.3/apysc/_material_design/icon/material_pause_circle_filled_icon.py
+-rw-r--r--   0 runner    (1001) docker     (127)     1336 2024-05-29 12:24:48.000000 apysc-4.4.3/apysc/_material_design/icon/material_pause_circle_filled_outlined_icon.py
+-rw-r--r--   0 runner    (1001) docker     (127)     1223 2024-05-29 12:24:48.000000 apysc-4.4.3/apysc/_material_design/icon/material_pause_circle_outline_icon.py
+-rw-r--r--   0 runner    (1001) docker     (127)     1251 2024-05-29 12:24:48.000000 apysc-4.4.3/apysc/_material_design/icon/material_pause_circle_outline_outlined_icon.py
+-rw-r--r--   0 runner    (1001) docker     (127)     1059 2024-05-29 12:24:48.000000 apysc-4.4.3/apysc/_material_design/icon/material_pause_icon.py
+-rw-r--r--   0 runner    (1001) docker     (127)     1087 2024-05-29 12:24:48.000000 apysc-4.4.3/apysc/_material_design/icon/material_pause_outlined_icon.py
+-rw-r--r--   0 runner    (1001) docker     (127)     1319 2024-05-29 12:24:48.000000 apysc-4.4.3/apysc/_material_design/icon/material_pause_presentation_icon.py
+-rw-r--r--   0 runner    (1001) docker     (127)     1230 2024-05-29 12:24:48.000000 apysc-4.4.3/apysc/_material_design/icon/material_pause_presentation_outlined_icon.py
+-rw-r--r--   0 runner    (1001) docker     (127)     1156 2024-05-29 12:24:48.000000 apysc-4.4.3/apysc/_material_design/icon/material_payment_icon.py
+-rw-r--r--   0 runner    (1001) docker     (127)     1184 2024-05-29 12:24:48.000000 apysc-4.4.3/apysc/_material_design/icon/material_payment_outlined_icon.py
+-rw-r--r--   0 runner    (1001) docker     (127)     1502 2024-05-29 12:24:48.000000 apysc-4.4.3/apysc/_material_design/icon/material_pending_actions_icon.py
+-rw-r--r--   0 runner    (1001) docker     (127)     1528 2024-05-29 12:24:48.000000 apysc-4.4.3/apysc/_material_design/icon/material_pending_actions_outlined_icon.py
+-rw-r--r--   0 runner    (1001) docker     (127)     1485 2024-05-29 12:24:48.000000 apysc-4.4.3/apysc/_material_design/icon/material_pending_icon.py
+-rw-r--r--   0 runner    (1001) docker     (127)     1380 2024-05-29 12:24:48.000000 apysc-4.4.3/apysc/_material_design/icon/material_pending_outlined_icon.py
+-rw-r--r--   0 runner    (1001) docker     (127)     1301 2024-05-29 12:24:48.000000 apysc-4.4.3/apysc/_material_design/icon/material_perm_camera_mic_icon.py
+-rw-r--r--   0 runner    (1001) docker     (127)     1401 2024-05-29 12:24:48.000000 apysc-4.4.3/apysc/_material_design/icon/material_perm_camera_mic_outlined_icon.py
+-rw-r--r--   0 runner    (1001) docker     (127)     1269 2024-05-29 12:24:48.000000 apysc-4.4.3/apysc/_material_design/icon/material_perm_contact_calendar_icon.py
+-rw-r--r--   0 runner    (1001) docker     (127)     1691 2024-05-29 12:24:48.000000 apysc-4.4.3/apysc/_material_design/icon/material_perm_contact_calendar_outlined_icon.py
+-rw-r--r--   0 runner    (1001) docker     (127)     1818 2024-05-29 12:24:48.000000 apysc-4.4.3/apysc/_material_design/icon/material_perm_data_setting_icon.py
+-rw-r--r--   0 runner    (1001) docker     (127)     1803 2024-05-29 12:24:48.000000 apysc-4.4.3/apysc/_material_design/icon/material_perm_data_setting_outlined_icon.py
+-rw-r--r--   0 runner    (1001) docker     (127)     1213 2024-05-29 12:24:48.000000 apysc-4.4.3/apysc/_material_design/icon/material_perm_device_information_icon.py
+-rw-r--r--   0 runner    (1001) docker     (127)     1265 2024-05-29 12:24:48.000000 apysc-4.4.3/apysc/_material_design/icon/material_perm_device_information_outlined_icon.py
+-rw-r--r--   0 runner    (1001) docker     (127)     1297 2024-05-29 12:24:48.000000 apysc-4.4.3/apysc/_material_design/icon/material_perm_identity_icon.py
+-rw-r--r--   0 runner    (1001) docker     (127)     1289 2024-05-29 12:24:48.000000 apysc-4.4.3/apysc/_material_design/icon/material_perm_identity_outlined_icon.py
+-rw-r--r--   0 runner    (1001) docker     (127)     1213 2024-05-29 12:24:48.000000 apysc-4.4.3/apysc/_material_design/icon/material_perm_media_icon.py
+-rw-r--r--   0 runner    (1001) docker     (127)     1273 2024-05-29 12:24:48.000000 apysc-4.4.3/apysc/_material_design/icon/material_perm_media_outlined_icon.py
+-rw-r--r--   0 runner    (1001) docker     (127)     1320 2024-05-29 12:24:48.000000 apysc-4.4.3/apysc/_material_design/icon/material_perm_phone_msg_icon.py
+-rw-r--r--   0 runner    (1001) docker     (127)     1522 2024-05-29 12:24:48.000000 apysc-4.4.3/apysc/_material_design/icon/material_perm_phone_msg_outlined_icon.py
+-rw-r--r--   0 runner    (1001) docker     (127)     1152 2024-05-29 12:24:48.000000 apysc-4.4.3/apysc/_material_design/icon/material_perm_scan_wifi_icon.py
+-rw-r--r--   0 runner    (1001) docker     (127)     1251 2024-05-29 12:24:48.000000 apysc-4.4.3/apysc/_material_design/icon/material_perm_scan_wifi_outlined_icon.py
+-rw-r--r--   0 runner    (1001) docker     (127)     1254 2024-05-29 12:24:48.000000 apysc-4.4.3/apysc/_material_design/icon/material_person_add_disabled_icon.py
+-rw-r--r--   0 runner    (1001) docker     (127)     1512 2024-05-29 12:24:48.000000 apysc-4.4.3/apysc/_material_design/icon/material_person_add_disabled_outlined_icon.py
+-rw-r--r--   0 runner    (1001) docker     (127)     1451 2024-05-29 12:24:48.000000 apysc-4.4.3/apysc/_material_design/icon/material_person_search_icon.py
+-rw-r--r--   0 runner    (1001) docker     (127)     1682 2024-05-29 12:24:48.000000 apysc-4.4.3/apysc/_material_design/icon/material_person_search_outlined_icon.py
+-rw-r--r--   0 runner    (1001) docker     (127)     1533 2024-05-29 12:24:48.000000 apysc-4.4.3/apysc/_material_design/icon/material_pets_icon.py
+-rw-r--r--   0 runner    (1001) docker     (127)     1561 2024-05-29 12:24:48.000000 apysc-4.4.3/apysc/_material_design/icon/material_pets_outlined_icon.py
+-rw-r--r--   0 runner    (1001) docker     (127)     1432 2024-05-29 12:24:48.000000 apysc-4.4.3/apysc/_material_design/icon/material_phone_disabled_icon.py
+-rw-r--r--   0 runner    (1001) docker     (127)     1751 2024-05-29 12:24:48.000000 apysc-4.4.3/apysc/_material_design/icon/material_phone_disabled_outlined_icon.py
+-rw-r--r--   0 runner    (1001) docker     (127)     1299 2024-05-29 12:24:48.000000 apysc-4.4.3/apysc/_material_design/icon/material_phone_enabled_icon.py
+-rw-r--r--   0 runner    (1001) docker     (127)     1608 2024-05-29 12:24:48.000000 apysc-4.4.3/apysc/_material_design/icon/material_phone_enabled_outlined_icon.py
+-rw-r--r--   0 runner    (1001) docker     (127)     1268 2024-05-29 12:24:48.000000 apysc-4.4.3/apysc/_material_design/icon/material_phone_icon.py
+-rw-r--r--   0 runner    (1001) docker     (127)     1463 2024-05-29 12:24:48.000000 apysc-4.4.3/apysc/_material_design/icon/material_phone_outlined_icon.py
+-rw-r--r--   0 runner    (1001) docker     (127)     1210 2024-05-29 12:24:48.000000 apysc-4.4.3/apysc/_material_design/icon/material_phonelink_erase_icon.py
+-rw-r--r--   0 runner    (1001) docker     (127)     1236 2024-05-29 12:24:48.000000 apysc-4.4.3/apysc/_material_design/icon/material_phonelink_erase_outlined_icon.py
+-rw-r--r--   0 runner    (1001) docker     (127)     1344 2024-05-29 12:24:48.000000 apysc-4.4.3/apysc/_material_design/icon/material_phonelink_lock_icon.py
+-rw-r--r--   0 runner    (1001) docker     (127)     1370 2024-05-29 12:24:48.000000 apysc-4.4.3/apysc/_material_design/icon/material_phonelink_lock_outlined_icon.py
+-rw-r--r--   0 runner    (1001) docker     (127)     1265 2024-05-29 12:24:48.000000 apysc-4.4.3/apysc/_material_design/icon/material_phonelink_ring_icon.py
+-rw-r--r--   0 runner    (1001) docker     (127)     1291 2024-05-29 12:24:48.000000 apysc-4.4.3/apysc/_material_design/icon/material_phonelink_ring_outlined_icon.py
+-rw-r--r--   0 runner    (1001) docker     (127)     1830 2024-05-29 12:24:48.000000 apysc-4.4.3/apysc/_material_design/icon/material_phonelink_setup_icon.py
+-rw-r--r--   0 runner    (1001) docker     (127)     1860 2024-05-29 12:24:48.000000 apysc-4.4.3/apysc/_material_design/icon/material_phonelink_setup_outlined_icon.py
+-rw-r--r--   0 runner    (1001) docker     (127)     1206 2024-05-29 12:24:48.000000 apysc-4.4.3/apysc/_material_design/icon/material_picture_in_picture_alt_icon.py
+-rw-r--r--   0 runner    (1001) docker     (127)     1250 2024-05-29 12:24:48.000000 apysc-4.4.3/apysc/_material_design/icon/material_picture_in_picture_alt_outlined_icon.py
+-rw-r--r--   0 runner    (1001) docker     (127)     1190 2024-05-29 12:24:48.000000 apysc-4.4.3/apysc/_material_design/icon/material_picture_in_picture_icon.py
+-rw-r--r--   0 runner    (1001) docker     (127)     1233 2024-05-29 12:24:48.000000 apysc-4.4.3/apysc/_material_design/icon/material_picture_in_picture_outlined_icon.py
+-rw-r--r--   0 runner    (1001) docker     (127)     1398 2024-05-29 12:24:48.000000 apysc-4.4.3/apysc/_material_design/icon/material_plagiarism_icon.py
+-rw-r--r--   0 runner    (1001) docker     (127)     1536 2024-05-29 12:24:48.000000 apysc-4.4.3/apysc/_material_design/icon/material_plagiarism_outlined_icon.py
+-rw-r--r--   0 runner    (1001) docker     (127)     1055 2024-05-29 12:24:48.000000 apysc-4.4.3/apysc/_material_design/icon/material_play_arrow_icon.py
+-rw-r--r--   0 runner    (1001) docker     (127)     1118 2024-05-29 12:24:48.000000 apysc-4.4.3/apysc/_material_design/icon/material_play_arrow_outlined_icon.py
+-rw-r--r--   0 runner    (1001) docker     (127)     1155 2024-05-29 12:24:48.000000 apysc-4.4.3/apysc/_material_design/icon/material_play_circle_filled_icon.py
+-rw-r--r--   0 runner    (1001) docker     (127)     1183 2024-05-29 12:24:48.000000 apysc-4.4.3/apysc/_material_design/icon/material_play_circle_filled_outlined_icon.py
+-rw-r--r--   0 runner    (1001) docker     (127)     1215 2024-05-29 12:24:48.000000 apysc-4.4.3/apysc/_material_design/icon/material_play_circle_outline_icon.py
+-rw-r--r--   0 runner    (1001) docker     (127)     1241 2024-05-29 12:24:48.000000 apysc-4.4.3/apysc/_material_design/icon/material_play_circle_outline_outlined_icon.py
+-rw-r--r--   0 runner    (1001) docker     (127)     1203 2024-05-29 12:24:48.000000 apysc-4.4.3/apysc/_material_design/icon/material_play_disabled_icon.py
+-rw-r--r--   0 runner    (1001) docker     (127)     1159 2024-05-29 12:24:48.000000 apysc-4.4.3/apysc/_material_design/icon/material_play_for_work_icon.py
+-rw-r--r--   0 runner    (1001) docker     (127)     1187 2024-05-29 12:24:48.000000 apysc-4.4.3/apysc/_material_design/icon/material_play_for_work_outlined_icon.py
+-rw-r--r--   0 runner    (1001) docker     (127)     1241 2024-05-29 12:24:48.000000 apysc-4.4.3/apysc/_material_design/icon/material_playlist_add_check_icon.py
+-rw-r--r--   0 runner    (1001) docker     (127)     1194 2024-05-29 12:24:48.000000 apysc-4.4.3/apysc/_material_design/icon/material_playlist_add_check_outlined_icon.py
+-rw-r--r--   0 runner    (1001) docker     (127)     1129 2024-05-29 12:24:48.000000 apysc-4.4.3/apysc/_material_design/icon/material_playlist_add_icon.py
+-rw-r--r--   0 runner    (1001) docker     (127)     1157 2024-05-29 12:24:48.000000 apysc-4.4.3/apysc/_material_design/icon/material_playlist_add_outlined_icon.py
+-rw-r--r--   0 runner    (1001) docker     (127)     1101 2024-05-29 12:24:48.000000 apysc-4.4.3/apysc/_material_design/icon/material_playlist_play_icon.py
+-rw-r--r--   0 runner    (1001) docker     (127)     1127 2024-05-29 12:24:48.000000 apysc-4.4.3/apysc/_material_design/icon/material_playlist_play_outlined_icon.py
+-rw-r--r--   0 runner    (1001) docker     (127)     1359 2024-05-29 12:24:48.000000 apysc-4.4.3/apysc/_material_design/icon/material_policy_icon.py
+-rw-r--r--   0 runner    (1001) docker     (127)     1500 2024-05-29 12:24:48.000000 apysc-4.4.3/apysc/_material_design/icon/material_policy_outlined_icon.py
+-rw-r--r--   0 runner    (1001) docker     (127)     1113 2024-05-29 12:24:48.000000 apysc-4.4.3/apysc/_material_design/icon/material_polymer_icon.py
+-rw-r--r--   0 runner    (1001) docker     (127)     1146 2024-05-29 12:24:48.000000 apysc-4.4.3/apysc/_material_design/icon/material_polymer_outlined_icon.py
+-rw-r--r--   0 runner    (1001) docker     (127)     1710 2024-05-29 12:24:48.000000 apysc-4.4.3/apysc/_material_design/icon/material_portable_wifi_off_icon.py
+-rw-r--r--   0 runner    (1001) docker     (127)     1716 2024-05-29 12:24:48.000000 apysc-4.4.3/apysc/_material_design/icon/material_portable_wifi_off_outlined_icon.py
+-rw-r--r--   0 runner    (1001) docker     (127)     1273 2024-05-29 12:24:48.000000 apysc-4.4.3/apysc/_material_design/icon/material_power_settings_new_icon.py
+-rw-r--r--   0 runner    (1001) docker     (127)     1301 2024-05-29 12:24:48.000000 apysc-4.4.3/apysc/_material_design/icon/material_power_settings_new_outlined_icon.py
+-rw-r--r--   0 runner    (1001) docker     (127)     1264 2024-05-29 12:24:48.000000 apysc-4.4.3/apysc/_material_design/icon/material_pregnant_woman_icon.py
+-rw-r--r--   0 runner    (1001) docker     (127)     1205 2024-05-29 12:24:48.000000 apysc-4.4.3/apysc/_material_design/icon/material_pregnant_woman_outlined_icon.py
+-rw-r--r--   0 runner    (1001) docker     (127)     1192 2024-05-29 12:24:48.000000 apysc-4.4.3/apysc/_material_design/icon/material_present_to_all_icon.py
+-rw-r--r--   0 runner    (1001) docker     (127)     1218 2024-05-29 12:24:48.000000 apysc-4.4.3/apysc/_material_design/icon/material_present_to_all_outlined_icon.py
+-rw-r--r--   0 runner    (1001) docker     (127)     1484 2024-05-29 12:24:48.000000 apysc-4.4.3/apysc/_material_design/icon/material_preview_icon.py
+-rw-r--r--   0 runner    (1001) docker     (127)     1507 2024-05-29 12:24:48.000000 apysc-4.4.3/apysc/_material_design/icon/material_preview_outlined_icon.py
+-rw-r--r--   0 runner    (1001) docker     (127)     1256 2024-05-29 12:24:48.000000 apysc-4.4.3/apysc/_material_design/icon/material_print_disabled_icon.py
+-rw-r--r--   0 runner    (1001) docker     (127)     1345 2024-05-29 12:24:48.000000 apysc-4.4.3/apysc/_material_design/icon/material_print_disabled_outlined_icon.py
+-rw-r--r--   0 runner    (1001) docker     (127)     1173 2024-05-29 12:24:48.000000 apysc-4.4.3/apysc/_material_design/icon/material_print_icon.py
+-rw-r--r--   0 runner    (1001) docker     (127)     1246 2024-05-29 12:24:48.000000 apysc-4.4.3/apysc/_material_design/icon/material_print_outlined_icon.py
+-rw-r--r--   0 runner    (1001) docker     (127)     1194 2024-05-29 12:24:48.000000 apysc-4.4.3/apysc/_material_design/icon/material_privacy_tip_icon.py
+-rw-r--r--   0 runner    (1001) docker     (127)     1300 2024-05-29 12:24:48.000000 apysc-4.4.3/apysc/_material_design/icon/material_privacy_tip_outlined_icon.py
+-rw-r--r--   0 runner    (1001) docker     (127)     1458 2024-05-29 12:24:48.000000 apysc-4.4.3/apysc/_material_design/icon/material_published_with_changes_icon.py
+-rw-r--r--   0 runner    (1001) docker     (127)     1481 2024-05-29 12:24:48.000000 apysc-4.4.3/apysc/_material_design/icon/material_published_with_changes_outlined_icon.py
+-rw-r--r--   0 runner    (1001) docker     (127)     1277 2024-05-29 12:24:48.000000 apysc-4.4.3/apysc/_material_design/icon/material_push_pin_icon.py
+-rw-r--r--   0 runner    (1001) docker     (127)     1372 2024-05-29 12:24:48.000000 apysc-4.4.3/apysc/_material_design/icon/material_push_pin_outlined_icon.py
+-rw-r--r--   0 runner    (1001) docker     (127)     1545 2024-05-29 12:24:48.000000 apysc-4.4.3/apysc/_material_design/icon/material_qr_code_icon.py
+-rw-r--r--   0 runner    (1001) docker     (127)     1571 2024-05-29 12:24:48.000000 apysc-4.4.3/apysc/_material_design/icon/material_qr_code_outlined_icon.py
+-rw-r--r--   0 runner    (1001) docker     (127)     1512 2024-05-29 12:24:48.000000 apysc-4.4.3/apysc/_material_design/icon/material_qr_code_scanner_icon.py
+-rw-r--r--   0 runner    (1001) docker     (127)     1538 2024-05-29 12:24:48.000000 apysc-4.4.3/apysc/_material_design/icon/material_qr_code_scanner_outlined_icon.py
+-rw-r--r--   0 runner    (1001) docker     (127)     1246 2024-05-29 12:24:48.000000 apysc-4.4.3/apysc/_material_design/icon/material_query_builder_icon.py
+-rw-r--r--   0 runner    (1001) docker     (127)     1261 2024-05-29 12:24:48.000000 apysc-4.4.3/apysc/_material_design/icon/material_query_builder_outlined_icon.py
+-rw-r--r--   0 runner    (1001) docker     (127)     1181 2024-05-29 12:24:48.000000 apysc-4.4.3/apysc/_material_design/icon/material_question_answer_icon.py
+-rw-r--r--   0 runner    (1001) docker     (127)     1239 2024-05-29 12:24:48.000000 apysc-4.4.3/apysc/_material_design/icon/material_question_answer_outlined_icon.py
+-rw-r--r--   0 runner    (1001) docker     (127)     1171 2024-05-29 12:24:48.000000 apysc-4.4.3/apysc/_material_design/icon/material_queue_icon.py
+-rw-r--r--   0 runner    (1001) docker     (127)     1173 2024-05-29 12:24:48.000000 apysc-4.4.3/apysc/_material_design/icon/material_queue_music_icon.py
+-rw-r--r--   0 runner    (1001) docker     (127)     1560 2024-05-29 12:24:48.000000 apysc-4.4.3/apysc/_material_design/icon/material_queue_music_outlined_icon.py
+-rw-r--r--   0 runner    (1001) docker     (127)     1213 2024-05-29 12:24:48.000000 apysc-4.4.3/apysc/_material_design/icon/material_queue_outlined_icon.py
+-rw-r--r--   0 runner    (1001) docker     (127)     1305 2024-05-29 12:24:48.000000 apysc-4.4.3/apysc/_material_design/icon/material_queue_play_next_icon.py
+-rw-r--r--   0 runner    (1001) docker     (127)     1248 2024-05-29 12:24:48.000000 apysc-4.4.3/apysc/_material_design/icon/material_queue_play_next_outlined_icon.py
+-rw-r--r--   0 runner    (1001) docker     (127)     1246 2024-05-29 12:24:48.000000 apysc-4.4.3/apysc/_material_design/icon/material_quickreply_icon.py
+-rw-r--r--   0 runner    (1001) docker     (127)     1295 2024-05-29 12:24:48.000000 apysc-4.4.3/apysc/_material_design/icon/material_quickreply_outlined_icon.py
+-rw-r--r--   0 runner    (1001) docker     (127)     1232 2024-05-29 12:24:48.000000 apysc-4.4.3/apysc/_material_design/icon/material_radio_icon.py
+-rw-r--r--   0 runner    (1001) docker     (127)     1246 2024-05-29 12:24:48.000000 apysc-4.4.3/apysc/_material_design/icon/material_radio_outlined_icon.py
+-rw-r--r--   0 runner    (1001) docker     (127)     1266 2024-05-29 12:24:48.000000 apysc-4.4.3/apysc/_material_design/icon/material_read_more_icon.py
+-rw-r--r--   0 runner    (1001) docker     (127)     1292 2024-05-29 12:24:48.000000 apysc-4.4.3/apysc/_material_design/icon/material_read_more_outlined_icon.py
+-rw-r--r--   0 runner    (1001) docker     (127)     1252 2024-05-29 12:24:48.000000 apysc-4.4.3/apysc/_material_design/icon/material_receipt_icon.py
+-rw-r--r--   0 runner    (1001) docker     (127)     1301 2024-05-29 12:24:48.000000 apysc-4.4.3/apysc/_material_design/icon/material_receipt_outlined_icon.py
+-rw-r--r--   0 runner    (1001) docker     (127)     1312 2024-05-29 12:24:48.000000 apysc-4.4.3/apysc/_material_design/icon/material_recent_actors_icon.py
+-rw-r--r--   0 runner    (1001) docker     (127)     1322 2024-05-29 12:24:48.000000 apysc-4.4.3/apysc/_material_design/icon/material_recent_actors_outlined_icon.py
+-rw-r--r--   0 runner    (1001) docker     (127)     1306 2024-05-29 12:24:48.000000 apysc-4.4.3/apysc/_material_design/icon/material_record_voice_over_icon.py
+-rw-r--r--   0 runner    (1001) docker     (127)     1457 2024-05-29 12:24:48.000000 apysc-4.4.3/apysc/_material_design/icon/material_record_voice_over_outlined_icon.py
+-rw-r--r--   0 runner    (1001) docker     (127)     1467 2024-05-29 12:24:48.000000 apysc-4.4.3/apysc/_material_design/icon/material_redeem_icon.py
+-rw-r--r--   0 runner    (1001) docker     (127)     1495 2024-05-29 12:24:48.000000 apysc-4.4.3/apysc/_material_design/icon/material_redeem_outlined_icon.py
+-rw-r--r--   0 runner    (1001) docker     (127)     1168 2024-05-29 12:24:48.000000 apysc-4.4.3/apysc/_material_design/icon/material_redo_icon.py
+-rw-r--r--   0 runner    (1001) docker     (127)     1196 2024-05-29 12:24:48.000000 apysc-4.4.3/apysc/_material_design/icon/material_redo_outlined_icon.py
+-rw-r--r--   0 runner    (1001) docker     (127)     1133 2024-05-29 12:24:48.000000 apysc-4.4.3/apysc/_material_design/icon/material_remove_circle_icon.py
+-rw-r--r--   0 runner    (1001) docker     (127)     1213 2024-05-29 12:24:48.000000 apysc-4.4.3/apysc/_material_design/icon/material_remove_circle_outline_icon.py
+-rw-r--r--   0 runner    (1001) docker     (127)     1241 2024-05-29 12:24:48.000000 apysc-4.4.3/apysc/_material_design/icon/material_remove_circle_outline_outlined_icon.py
+-rw-r--r--   0 runner    (1001) docker     (127)     1161 2024-05-29 12:24:48.000000 apysc-4.4.3/apysc/_material_design/icon/material_remove_circle_outlined_icon.py
+-rw-r--r--   0 runner    (1001) docker     (127)     1313 2024-05-29 12:24:48.000000 apysc-4.4.3/apysc/_material_design/icon/material_remove_done_icon.py
+-rw-r--r--   0 runner    (1001) docker     (127)     1276 2024-05-29 12:24:48.000000 apysc-4.4.3/apysc/_material_design/icon/material_remove_from_queue_icon.py
+-rw-r--r--   0 runner    (1001) docker     (127)     1209 2024-05-29 12:24:48.000000 apysc-4.4.3/apysc/_material_design/icon/material_remove_from_queue_outlined_icon.py
+-rw-r--r--   0 runner    (1001) docker     (127)     1048 2024-05-29 12:24:48.000000 apysc-4.4.3/apysc/_material_design/icon/material_remove_icon.py
+-rw-r--r--   0 runner    (1001) docker     (127)     1076 2024-05-29 12:24:48.000000 apysc-4.4.3/apysc/_material_design/icon/material_remove_outlined_icon.py
+-rw-r--r--   0 runner    (1001) docker     (127)     1490 2024-05-29 12:24:48.000000 apysc-4.4.3/apysc/_material_design/icon/material_remove_shopping_cart_icon.py
+-rw-r--r--   0 runner    (1001) docker     (127)     1474 2024-05-29 12:24:48.000000 apysc-4.4.3/apysc/_material_design/icon/material_remove_shopping_cart_outlined_icon.py
+-rw-r--r--   0 runner    (1001) docker     (127)     1093 2024-05-29 12:24:48.000000 apysc-4.4.3/apysc/_material_design/icon/material_reorder_icon.py
+-rw-r--r--   0 runner    (1001) docker     (127)     1121 2024-05-29 12:24:48.000000 apysc-4.4.3/apysc/_material_design/icon/material_reorder_outlined_icon.py
+-rw-r--r--   0 runner    (1001) docker     (127)     1094 2024-05-29 12:24:48.000000 apysc-4.4.3/apysc/_material_design/icon/material_repeat_icon.py
+-rw-r--r--   0 runner    (1001) docker     (127)     1200 2024-05-29 12:24:48.000000 apysc-4.4.3/apysc/_material_design/icon/material_repeat_on_icon.py
+-rw-r--r--   0 runner    (1001) docker     (127)     1132 2024-05-29 12:24:48.000000 apysc-4.4.3/apysc/_material_design/icon/material_repeat_one_icon.py
+-rw-r--r--   0 runner    (1001) docker     (127)     1238 2024-05-29 12:24:48.000000 apysc-4.4.3/apysc/_material_design/icon/material_repeat_one_on_icon.py
+-rw-r--r--   0 runner    (1001) docker     (127)     1160 2024-05-29 12:24:48.000000 apysc-4.4.3/apysc/_material_design/icon/material_repeat_one_outlined_icon.py
+-rw-r--r--   0 runner    (1001) docker     (127)     1122 2024-05-29 12:24:48.000000 apysc-4.4.3/apysc/_material_design/icon/material_repeat_outlined_icon.py
+-rw-r--r--   0 runner    (1001) docker     (127)     2032 2024-05-29 12:24:48.000000 apysc-4.4.3/apysc/_material_design/icon/material_replay_10_icon.py
+-rw-r--r--   0 runner    (1001) docker     (127)     1724 2024-05-29 12:24:48.000000 apysc-4.4.3/apysc/_material_design/icon/material_replay_10_outlined_icon.py
+-rw-r--r--   0 runner    (1001) docker     (127)     2997 2024-05-29 12:24:48.000000 apysc-4.4.3/apysc/_material_design/icon/material_replay_30_icon.py
+-rw-r--r--   0 runner    (1001) docker     (127)     2408 2024-05-29 12:24:48.000000 apysc-4.4.3/apysc/_material_design/icon/material_replay_30_outlined_icon.py
+-rw-r--r--   0 runner    (1001) docker     (127)     1948 2024-05-29 12:24:48.000000 apysc-4.4.3/apysc/_material_design/icon/material_replay_5_icon.py
+-rw-r--r--   0 runner    (1001) docker     (127)     1689 2024-05-29 12:24:48.000000 apysc-4.4.3/apysc/_material_design/icon/material_replay_5_outlined_icon.py
+-rw-r--r--   0 runner    (1001) docker     (127)     1267 2024-05-29 12:24:48.000000 apysc-4.4.3/apysc/_material_design/icon/material_replay_circle_filled_icon.py
+-rw-r--r--   0 runner    (1001) docker     (127)     1132 2024-05-29 12:24:48.000000 apysc-4.4.3/apysc/_material_design/icon/material_replay_icon.py
+-rw-r--r--   0 runner    (1001) docker     (127)     1302 2024-05-29 12:24:48.000000 apysc-4.4.3/apysc/_material_design/icon/material_replay_outlined_icon.py
+-rw-r--r--   0 runner    (1001) docker     (127)     1122 2024-05-29 12:24:48.000000 apysc-4.4.3/apysc/_material_design/icon/material_reply_all_icon.py
+-rw-r--r--   0 runner    (1001) docker     (127)     1150 2024-05-29 12:24:48.000000 apysc-4.4.3/apysc/_material_design/icon/material_reply_all_outlined_icon.py
+-rw-r--r--   0 runner    (1001) docker     (127)     1084 2024-05-29 12:24:48.000000 apysc-4.4.3/apysc/_material_design/icon/material_reply_icon.py
+-rw-r--r--   0 runner    (1001) docker     (127)     1112 2024-05-29 12:24:48.000000 apysc-4.4.3/apysc/_material_design/icon/material_reply_outlined_icon.py
+-rw-r--r--   0 runner    (1001) docker     (127)     1270 2024-05-29 12:24:48.000000 apysc-4.4.3/apysc/_material_design/icon/material_report_gmailerrorred_outlined_icon.py
+-rw-r--r--   0 runner    (1001) docker     (127)     1203 2024-05-29 12:24:48.000000 apysc-4.4.3/apysc/_material_design/icon/material_report_icon.py
+-rw-r--r--   0 runner    (1001) docker     (127)     1279 2024-05-29 12:24:48.000000 apysc-4.4.3/apysc/_material_design/icon/material_report_off_icon.py
+-rw-r--r--   0 runner    (1001) docker     (127)     1352 2024-05-29 12:24:48.000000 apysc-4.4.3/apysc/_material_design/icon/material_report_off_outlined_icon.py
+-rw-r--r--   0 runner    (1001) docker     (127)     1229 2024-05-29 12:24:48.000000 apysc-4.4.3/apysc/_material_design/icon/material_report_outlined_icon.py
+-rw-r--r--   0 runner    (1001) docker     (127)     1104 2024-05-29 12:24:48.000000 apysc-4.4.3/apysc/_material_design/icon/material_report_problem_icon.py
+-rw-r--r--   0 runner    (1001) docker     (127)     1162 2024-05-29 12:24:48.000000 apysc-4.4.3/apysc/_material_design/icon/material_report_problem_outlined_icon.py
+-rw-r--r--   0 runner    (1001) docker     (127)     1287 2024-05-29 12:24:48.000000 apysc-4.4.3/apysc/_material_design/icon/material_request_page_icon.py
+-rw-r--r--   0 runner    (1001) docker     (127)     1348 2024-05-29 12:24:48.000000 apysc-4.4.3/apysc/_material_design/icon/material_request_page_outlined_icon.py
+-rw-r--r--   0 runner    (1001) docker     (127)     1165 2024-05-29 12:24:48.000000 apysc-4.4.3/apysc/_material_design/icon/material_restore_from_trash_icon.py
+-rw-r--r--   0 runner    (1001) docker     (127)     1207 2024-05-29 12:24:48.000000 apysc-4.4.3/apysc/_material_design/icon/material_restore_from_trash_outlined_icon.py
+-rw-r--r--   0 runner    (1001) docker     (127)     1258 2024-05-29 12:24:48.000000 apysc-4.4.3/apysc/_material_design/icon/material_restore_icon.py
+-rw-r--r--   0 runner    (1001) docker     (127)     1275 2024-05-29 12:24:48.000000 apysc-4.4.3/apysc/_material_design/icon/material_restore_outlined_icon.py
+-rw-r--r--   0 runner    (1001) docker     (127)     1325 2024-05-29 12:24:48.000000 apysc-4.4.3/apysc/_material_design/icon/material_restore_page_icon.py
+-rw-r--r--   0 runner    (1001) docker     (127)     1421 2024-05-29 12:24:48.000000 apysc-4.4.3/apysc/_material_design/icon/material_restore_page_outlined_icon.py
+-rw-r--r--   0 runner    (1001) docker     (127)     1571 2024-05-29 12:24:48.000000 apysc-4.4.3/apysc/_material_design/icon/material_ring_volume_icon.py
+-rw-r--r--   0 runner    (1001) docker     (127)     1761 2024-05-29 12:24:48.000000 apysc-4.4.3/apysc/_material_design/icon/material_ring_volume_outlined_icon.py
+-rw-r--r--   0 runner    (1001) docker     (127)     1179 2024-05-29 12:24:48.000000 apysc-4.4.3/apysc/_material_design/icon/material_room_icon.py
+-rw-r--r--   0 runner    (1001) docker     (127)     1237 2024-05-29 12:24:48.000000 apysc-4.4.3/apysc/_material_design/icon/material_room_outlined_icon.py
+-rw-r--r--   0 runner    (1001) docker     (127)     1381 2024-05-29 12:24:48.000000 apysc-4.4.3/apysc/_material_design/icon/material_rounded_corner_icon.py
+-rw-r--r--   0 runner    (1001) docker     (127)     1312 2024-05-29 12:24:48.000000 apysc-4.4.3/apysc/_material_design/icon/material_rounded_corner_outlined_icon.py
+-rw-r--r--   0 runner    (1001) docker     (127)     1471 2024-05-29 12:24:48.000000 apysc-4.4.3/apysc/_material_design/icon/material_rowing_icon.py
+-rw-r--r--   0 runner    (1001) docker     (127)     1415 2024-05-29 12:24:48.000000 apysc-4.4.3/apysc/_material_design/icon/material_rowing_outlined_icon.py
+-rw-r--r--   0 runner    (1001) docker     (127)     1220 2024-05-29 12:24:48.000000 apysc-4.4.3/apysc/_material_design/icon/material_rss_feed_icon.py
+-rw-r--r--   0 runner    (1001) docker     (127)     1248 2024-05-29 12:24:48.000000 apysc-4.4.3/apysc/_material_design/icon/material_rss_feed_outlined_icon.py
+-rw-r--r--   0 runner    (1001) docker     (127)     1275 2024-05-29 12:24:48.000000 apysc-4.4.3/apysc/_material_design/icon/material_rtt_icon.py
+-rw-r--r--   0 runner    (1001) docker     (127)     1290 2024-05-29 12:24:48.000000 apysc-4.4.3/apysc/_material_design/icon/material_rule_icon.py
+-rw-r--r--   0 runner    (1001) docker     (127)     1316 2024-05-29 12:24:48.000000 apysc-4.4.3/apysc/_material_design/icon/material_rule_outlined_icon.py
+-rw-r--r--   0 runner    (1001) docker     (127)     1150 2024-05-29 12:24:48.000000 apysc-4.4.3/apysc/_material_design/icon/material_save_alt_icon.py
+-rw-r--r--   0 runner    (1001) docker     (127)     1183 2024-05-29 12:24:48.000000 apysc-4.4.3/apysc/_material_design/icon/material_save_alt_outlined_icon.py
+-rw-r--r--   0 runner    (1001) docker     (127)     1167 2024-05-29 12:24:48.000000 apysc-4.4.3/apysc/_material_design/icon/material_save_icon.py
+-rw-r--r--   0 runner    (1001) docker     (127)     1217 2024-05-29 12:24:48.000000 apysc-4.4.3/apysc/_material_design/icon/material_save_outlined_icon.py
+-rw-r--r--   0 runner    (1001) docker     (127)     1366 2024-05-29 12:24:48.000000 apysc-4.4.3/apysc/_material_design/icon/material_saved_search_icon.py
+-rw-r--r--   0 runner    (1001) docker     (127)     1232 2024-05-29 12:24:48.000000 apysc-4.4.3/apysc/_material_design/icon/material_schedule_icon.py
+-rw-r--r--   0 runner    (1001) docker     (127)     1247 2024-05-29 12:24:48.000000 apysc-4.4.3/apysc/_material_design/icon/material_schedule_outlined_icon.py
+-rw-r--r--   0 runner    (1001) docker     (127)     1281 2024-05-29 12:24:48.000000 apysc-4.4.3/apysc/_material_design/icon/material_schedule_send_icon.py
+-rw-r--r--   0 runner    (1001) docker     (127)     1229 2024-05-29 12:24:48.000000 apysc-4.4.3/apysc/_material_design/icon/material_screen_share_icon.py
+-rw-r--r--   0 runner    (1001) docker     (127)     1280 2024-05-29 12:24:48.000000 apysc-4.4.3/apysc/_material_design/icon/material_screen_share_outlined_icon.py
+-rw-r--r--   0 runner    (1001) docker     (127)     1313 2024-05-29 12:24:48.000000 apysc-4.4.3/apysc/_material_design/icon/material_sd_icon.py
+-rw-r--r--   0 runner    (1001) docker     (127)     1265 2024-05-29 12:24:48.000000 apysc-4.4.3/apysc/_material_design/icon/material_search_icon.py
+-rw-r--r--   0 runner    (1001) docker     (127)     1532 2024-05-29 12:24:48.000000 apysc-4.4.3/apysc/_material_design/icon/material_search_off_icon.py
+-rw-r--r--   0 runner    (1001) docker     (127)     1558 2024-05-29 12:24:48.000000 apysc-4.4.3/apysc/_material_design/icon/material_search_off_outlined_icon.py
+-rw-r--r--   0 runner    (1001) docker     (127)     1293 2024-05-29 12:24:48.000000 apysc-4.4.3/apysc/_material_design/icon/material_search_outlined_icon.py
+-rw-r--r--   0 runner    (1001) docker     (127)     1081 2024-05-29 12:24:48.000000 apysc-4.4.3/apysc/_material_design/icon/material_segment_icon.py
+-rw-r--r--   0 runner    (1001) docker     (127)     1346 2024-05-29 12:24:48.000000 apysc-4.4.3/apysc/_material_design/icon/material_select_all_icon.py
+-rw-r--r--   0 runner    (1001) docker     (127)     1374 2024-05-29 12:24:48.000000 apysc-4.4.3/apysc/_material_design/icon/material_select_all_outlined_icon.py
+-rw-r--r--   0 runner    (1001) docker     (127)     1193 2024-05-29 12:24:48.000000 apysc-4.4.3/apysc/_material_design/icon/material_send_and_archive_icon.py
+-rw-r--r--   0 runner    (1001) docker     (127)     1062 2024-05-29 12:24:48.000000 apysc-4.4.3/apysc/_material_design/icon/material_send_icon.py
+-rw-r--r--   0 runner    (1001) docker     (127)     1161 2024-05-29 12:24:48.000000 apysc-4.4.3/apysc/_material_design/icon/material_send_outlined_icon.py
+-rw-r--r--   0 runner    (1001) docker     (127)     1517 2024-05-29 12:24:48.000000 apysc-4.4.3/apysc/_material_design/icon/material_sentiment_satisfied_alt_icon.py
+-rw-r--r--   0 runner    (1001) docker     (127)     1433 2024-05-29 12:24:48.000000 apysc-4.4.3/apysc/_material_design/icon/material_sentiment_satisfied_alt_outlined_icon.py
+-rw-r--r--   0 runner    (1001) docker     (127)     1804 2024-05-29 12:24:48.000000 apysc-4.4.3/apysc/_material_design/icon/material_settings_applications_icon.py
+-rw-r--r--   0 runner    (1001) docker     (127)     1884 2024-05-29 12:24:48.000000 apysc-4.4.3/apysc/_material_design/icon/material_settings_applications_outlined_icon.py
+-rw-r--r--   0 runner    (1001) docker     (127)     1298 2024-05-29 12:24:48.000000 apysc-4.4.3/apysc/_material_design/icon/material_settings_backup_restore_icon.py
+-rw-r--r--   0 runner    (1001) docker     (127)     1326 2024-05-29 12:24:48.000000 apysc-4.4.3/apysc/_material_design/icon/material_settings_backup_restore_outlined_icon.py
+-rw-r--r--   0 runner    (1001) docker     (127)     1288 2024-05-29 12:24:48.000000 apysc-4.4.3/apysc/_material_design/icon/material_settings_bluetooth_icon.py
+-rw-r--r--   0 runner    (1001) docker     (127)     1316 2024-05-29 12:24:48.000000 apysc-4.4.3/apysc/_material_design/icon/material_settings_bluetooth_outlined_icon.py
+-rw-r--r--   0 runner    (1001) docker     (127)     1301 2024-05-29 12:24:48.000000 apysc-4.4.3/apysc/_material_design/icon/material_settings_brightness_icon.py
+-rw-r--r--   0 runner    (1001) docker     (127)     1329 2024-05-29 12:24:48.000000 apysc-4.4.3/apysc/_material_design/icon/material_settings_brightness_outlined_icon.py
+-rw-r--r--   0 runner    (1001) docker     (127)     1196 2024-05-29 12:24:48.000000 apysc-4.4.3/apysc/_material_design/icon/material_settings_cell_icon.py
+-rw-r--r--   0 runner    (1001) docker     (127)     1243 2024-05-29 12:24:48.000000 apysc-4.4.3/apysc/_material_design/icon/material_settings_cell_outlined_icon.py
+-rw-r--r--   0 runner    (1001) docker     (127)     1247 2024-05-29 12:24:48.000000 apysc-4.4.3/apysc/_material_design/icon/material_settings_ethernet_icon.py
+-rw-r--r--   0 runner    (1001) docker     (127)     1275 2024-05-29 12:24:48.000000 apysc-4.4.3/apysc/_material_design/icon/material_settings_ethernet_outlined_icon.py
+-rw-r--r--   0 runner    (1001) docker     (127)     1938 2024-05-29 12:24:48.000000 apysc-4.4.3/apysc/_material_design/icon/material_settings_icon.py
+-rw-r--r--   0 runner    (1001) docker     (127)     1381 2024-05-29 12:24:48.000000 apysc-4.4.3/apysc/_material_design/icon/material_settings_input_antenna_icon.py
+-rw-r--r--   0 runner    (1001) docker     (127)     1409 2024-05-29 12:24:48.000000 apysc-4.4.3/apysc/_material_design/icon/material_settings_input_antenna_outlined_icon.py
+-rw-r--r--   0 runner    (1001) docker     (127)     1427 2024-05-29 12:24:48.000000 apysc-4.4.3/apysc/_material_design/icon/material_settings_input_component_icon.py
+-rw-r--r--   0 runner    (1001) docker     (127)     1596 2024-05-29 12:24:48.000000 apysc-4.4.3/apysc/_material_design/icon/material_settings_input_component_outlined_icon.py
+-rw-r--r--   0 runner    (1001) docker     (127)     1427 2024-05-29 12:24:48.000000 apysc-4.4.3/apysc/_material_design/icon/material_settings_input_composite_icon.py
+-rw-r--r--   0 runner    (1001) docker     (127)     1596 2024-05-29 12:24:48.000000 apysc-4.4.3/apysc/_material_design/icon/material_settings_input_composite_outlined_icon.py
+-rw-r--r--   0 runner    (1001) docker     (127)     1168 2024-05-29 12:24:48.000000 apysc-4.4.3/apysc/_material_design/icon/material_settings_input_hdmi_icon.py
+-rw-r--r--   0 runner    (1001) docker     (127)     1239 2024-05-29 12:24:48.000000 apysc-4.4.3/apysc/_material_design/icon/material_settings_input_hdmi_outlined_icon.py
+-rw-r--r--   0 runner    (1001) docker     (127)     1591 2024-05-29 12:24:48.000000 apysc-4.4.3/apysc/_material_design/icon/material_settings_input_svideo_icon.py
+-rw-r--r--   0 runner    (1001) docker     (127)     1619 2024-05-29 12:24:48.000000 apysc-4.4.3/apysc/_material_design/icon/material_settings_input_svideo_outlined_icon.py
+-rw-r--r--   0 runner    (1001) docker     (127)     2368 2024-05-29 12:24:48.000000 apysc-4.4.3/apysc/_material_design/icon/material_settings_outlined_icon.py
+-rw-r--r--   0 runner    (1001) docker     (127)     1263 2024-05-29 12:24:48.000000 apysc-4.4.3/apysc/_material_design/icon/material_settings_overscan_icon.py
+-rw-r--r--   0 runner    (1001) docker     (127)     1291 2024-05-29 12:24:48.000000 apysc-4.4.3/apysc/_material_design/icon/material_settings_overscan_outlined_icon.py
+-rw-r--r--   0 runner    (1001) docker     (127)     1343 2024-05-29 12:24:48.000000 apysc-4.4.3/apysc/_material_design/icon/material_settings_phone_icon.py
+-rw-r--r--   0 runner    (1001) docker     (127)     1525 2024-05-29 12:24:48.000000 apysc-4.4.3/apysc/_material_design/icon/material_settings_phone_outlined_icon.py
+-rw-r--r--   0 runner    (1001) docker     (127)     1309 2024-05-29 12:24:48.000000 apysc-4.4.3/apysc/_material_design/icon/material_settings_power_icon.py
+-rw-r--r--   0 runner    (1001) docker     (127)     1337 2024-05-29 12:24:48.000000 apysc-4.4.3/apysc/_material_design/icon/material_settings_power_outlined_icon.py
+-rw-r--r--   0 runner    (1001) docker     (127)     1420 2024-05-29 12:24:48.000000 apysc-4.4.3/apysc/_material_design/icon/material_settings_remote_icon.py
+-rw-r--r--   0 runner    (1001) docker     (127)     1460 2024-05-29 12:24:48.000000 apysc-4.4.3/apysc/_material_design/icon/material_settings_remote_outlined_icon.py
+-rw-r--r--   0 runner    (1001) docker     (127)     1291 2024-05-29 12:24:48.000000 apysc-4.4.3/apysc/_material_design/icon/material_settings_voice_icon.py
+-rw-r--r--   0 runner    (1001) docker     (127)     1366 2024-05-29 12:24:48.000000 apysc-4.4.3/apysc/_material_design/icon/material_settings_voice_outlined_icon.py
+-rw-r--r--   0 runner    (1001) docker     (127)     1153 2024-05-29 12:24:48.000000 apysc-4.4.3/apysc/_material_design/icon/material_shop_icon.py
+-rw-r--r--   0 runner    (1001) docker     (127)     1195 2024-05-29 12:24:48.000000 apysc-4.4.3/apysc/_material_design/icon/material_shop_outlined_icon.py
+-rw-r--r--   0 runner    (1001) docker     (127)     1215 2024-05-29 12:24:48.000000 apysc-4.4.3/apysc/_material_design/icon/material_shop_two_icon.py
+-rw-r--r--   0 runner    (1001) docker     (127)     1255 2024-05-29 12:24:48.000000 apysc-4.4.3/apysc/_material_design/icon/material_shop_two_outlined_icon.py
+-rw-r--r--   0 runner    (1001) docker     (127)     1345 2024-05-29 12:24:48.000000 apysc-4.4.3/apysc/_material_design/icon/material_shopping_bag_icon.py
+-rw-r--r--   0 runner    (1001) docker     (127)     1368 2024-05-29 12:24:48.000000 apysc-4.4.3/apysc/_material_design/icon/material_shopping_bag_outlined_icon.py
+-rw-r--r--   0 runner    (1001) docker     (127)     1332 2024-05-29 12:24:48.000000 apysc-4.4.3/apysc/_material_design/icon/material_shopping_basket_icon.py
+-rw-r--r--   0 runner    (1001) docker     (127)     1401 2024-05-29 12:24:48.000000 apysc-4.4.3/apysc/_material_design/icon/material_shopping_basket_outlined_icon.py
+-rw-r--r--   0 runner    (1001) docker     (127)     1372 2024-05-29 12:24:48.000000 apysc-4.4.3/apysc/_material_design/icon/material_shopping_cart_icon.py
+-rw-r--r--   0 runner    (1001) docker     (127)     1379 2024-05-29 12:24:48.000000 apysc-4.4.3/apysc/_material_design/icon/material_shopping_cart_outlined_icon.py
+-rw-r--r--   0 runner    (1001) docker     (127)     1207 2024-05-29 12:24:48.000000 apysc-4.4.3/apysc/_material_design/icon/material_shuffle_icon.py
+-rw-r--r--   0 runner    (1001) docker     (127)     1313 2024-05-29 12:24:48.000000 apysc-4.4.3/apysc/_material_design/icon/material_shuffle_on_icon.py
+-rw-r--r--   0 runner    (1001) docker     (127)     1235 2024-05-29 12:24:48.000000 apysc-4.4.3/apysc/_material_design/icon/material_shuffle_outlined_icon.py
+-rw-r--r--   0 runner    (1001) docker     (127)     1074 2024-05-29 12:24:48.000000 apysc-4.4.3/apysc/_material_design/icon/material_skip_next_icon.py
+-rw-r--r--   0 runner    (1001) docker     (127)     1130 2024-05-29 12:24:48.000000 apysc-4.4.3/apysc/_material_design/icon/material_skip_next_outlined_icon.py
+-rw-r--r--   0 runner    (1001) docker     (127)     1078 2024-05-29 12:24:48.000000 apysc-4.4.3/apysc/_material_design/icon/material_skip_previous_icon.py
+-rw-r--r--   0 runner    (1001) docker     (127)     1145 2024-05-29 12:24:48.000000 apysc-4.4.3/apysc/_material_design/icon/material_skip_previous_outlined_icon.py
+-rw-r--r--   0 runner    (1001) docker     (127)     1596 2024-05-29 12:24:48.000000 apysc-4.4.3/apysc/_material_design/icon/material_slow_motion_video_icon.py
+-rw-r--r--   0 runner    (1001) docker     (127)     1655 2024-05-29 12:24:48.000000 apysc-4.4.3/apysc/_material_design/icon/material_slow_motion_video_outlined_icon.py
+-rw-r--r--   0 runner    (1001) docker     (127)     1515 2024-05-29 12:24:48.000000 apysc-4.4.3/apysc/_material_design/icon/material_smart_button_icon.py
+-rw-r--r--   0 runner    (1001) docker     (127)     1541 2024-05-29 12:24:48.000000 apysc-4.4.3/apysc/_material_design/icon/material_smart_button_outlined_icon.py
+-rw-r--r--   0 runner    (1001) docker     (127)     1294 2024-05-29 12:24:48.000000 apysc-4.4.3/apysc/_material_design/icon/material_snooze_icon.py
+-rw-r--r--   0 runner    (1001) docker     (127)     1311 2024-05-29 12:24:48.000000 apysc-4.4.3/apysc/_material_design/icon/material_snooze_outlined_icon.py
+-rw-r--r--   0 runner    (1001) docker     (127)     1323 2024-05-29 12:24:48.000000 apysc-4.4.3/apysc/_material_design/icon/material_sort_by_alpha_icon.py
+-rw-r--r--   0 runner    (1001) docker     (127)     1332 2024-05-29 12:24:48.000000 apysc-4.4.3/apysc/_material_design/icon/material_sort_by_alpha_outlined_icon.py
+-rw-r--r--   0 runner    (1001) docker     (127)     1213 2024-05-29 12:24:48.000000 apysc-4.4.3/apysc/_material_design/icon/material_source_icon.py
+-rw-r--r--   0 runner    (1001) docker     (127)     1270 2024-05-29 12:24:48.000000 apysc-4.4.3/apysc/_material_design/icon/material_source_outlined_icon.py
+-rw-r--r--   0 runner    (1001) docker     (127)     1208 2024-05-29 12:24:48.000000 apysc-4.4.3/apysc/_material_design/icon/material_speaker_notes_icon.py
+-rw-r--r--   0 runner    (1001) docker     (127)     1302 2024-05-29 12:24:48.000000 apysc-4.4.3/apysc/_material_design/icon/material_speaker_notes_off_icon.py
+-rw-r--r--   0 runner    (1001) docker     (127)     1326 2024-05-29 12:24:48.000000 apysc-4.4.3/apysc/_material_design/icon/material_speaker_notes_off_outlined_icon.py
+-rw-r--r--   0 runner    (1001) docker     (127)     1256 2024-05-29 12:24:48.000000 apysc-4.4.3/apysc/_material_design/icon/material_speaker_notes_outlined_icon.py
+-rw-r--r--   0 runner    (1001) docker     (127)     1442 2024-05-29 12:24:48.000000 apysc-4.4.3/apysc/_material_design/icon/material_speaker_phone_icon.py
+-rw-r--r--   0 runner    (1001) docker     (127)     1453 2024-05-29 12:24:48.000000 apysc-4.4.3/apysc/_material_design/icon/material_speaker_phone_outlined_icon.py
+-rw-r--r--   0 runner    (1001) docker     (127)     1254 2024-05-29 12:24:48.000000 apysc-4.4.3/apysc/_material_design/icon/material_speed_icon.py
+-rw-r--r--   0 runner    (1001) docker     (127)     1293 2024-05-29 12:24:48.000000 apysc-4.4.3/apysc/_material_design/icon/material_speed_outlined_icon.py
+-rw-r--r--   0 runner    (1001) docker     (127)     1201 2024-05-29 12:24:48.000000 apysc-4.4.3/apysc/_material_design/icon/material_spellcheck_icon.py
+-rw-r--r--   0 runner    (1001) docker     (127)     1229 2024-05-29 12:24:48.000000 apysc-4.4.3/apysc/_material_design/icon/material_spellcheck_outlined_icon.py
+-rw-r--r--   0 runner    (1001) docker     (127)     1180 2024-05-29 12:24:48.000000 apysc-4.4.3/apysc/_material_design/icon/material_star_rate_icon.py
+-rw-r--r--   0 runner    (1001) docker     (127)     1298 2024-05-29 12:24:48.000000 apysc-4.4.3/apysc/_material_design/icon/material_star_rate_outlined_icon.py
+-rw-r--r--   0 runner    (1001) docker     (127)     1209 2024-05-29 12:24:48.000000 apysc-4.4.3/apysc/_material_design/icon/material_stars_icon.py
+-rw-r--r--   0 runner    (1001) docker     (127)     1590 2024-05-29 12:24:48.000000 apysc-4.4.3/apysc/_material_design/icon/material_stars_outlined_icon.py
+-rw-r--r--   0 runner    (1001) docker     (127)     1178 2024-05-29 12:24:48.000000 apysc-4.4.3/apysc/_material_design/icon/material_stay_current_landscape_icon.py
+-rw-r--r--   0 runner    (1001) docker     (127)     1206 2024-05-29 12:24:48.000000 apysc-4.4.3/apysc/_material_design/icon/material_stay_current_landscape_outlined_icon.py
+-rw-r--r--   0 runner    (1001) docker     (127)     1187 2024-05-29 12:24:48.000000 apysc-4.4.3/apysc/_material_design/icon/material_stay_current_portrait_icon.py
+-rw-r--r--   0 runner    (1001) docker     (127)     1215 2024-05-29 12:24:48.000000 apysc-4.4.3/apysc/_material_design/icon/material_stay_current_portrait_outlined_icon.py
+-rw-r--r--   0 runner    (1001) docker     (127)     1178 2024-05-29 12:24:48.000000 apysc-4.4.3/apysc/_material_design/icon/material_stay_primary_landscape_icon.py
+-rw-r--r--   0 runner    (1001) docker     (127)     1206 2024-05-29 12:24:48.000000 apysc-4.4.3/apysc/_material_design/icon/material_stay_primary_landscape_outlined_icon.py
+-rw-r--r--   0 runner    (1001) docker     (127)     1187 2024-05-29 12:24:48.000000 apysc-4.4.3/apysc/_material_design/icon/material_stay_primary_portrait_icon.py
+-rw-r--r--   0 runner    (1001) docker     (127)     1215 2024-05-29 12:24:48.000000 apysc-4.4.3/apysc/_material_design/icon/material_stay_primary_portrait_outlined_icon.py
+-rw-r--r--   0 runner    (1001) docker     (127)     1231 2024-05-29 12:24:48.000000 apysc-4.4.3/apysc/_material_design/icon/material_sticky_note_2_icon.py
+-rw-r--r--   0 runner    (1001) docker     (127)     1246 2024-05-29 12:24:48.000000 apysc-4.4.3/apysc/_material_design/icon/material_sticky_note_2_outlined_icon.py
+-rw-r--r--   0 runner    (1001) docker     (127)     1206 2024-05-29 12:24:48.000000 apysc-4.4.3/apysc/_material_design/icon/material_stop_circle_icon.py
+-rw-r--r--   0 runner    (1001) docker     (127)     1318 2024-05-29 12:24:48.000000 apysc-4.4.3/apysc/_material_design/icon/material_stop_circle_outlined_icon.py
+-rw-r--r--   0 runner    (1001) docker     (127)     1038 2024-05-29 12:24:48.000000 apysc-4.4.3/apysc/_material_design/icon/material_stop_icon.py
+-rw-r--r--   0 runner    (1001) docker     (127)     1081 2024-05-29 12:24:48.000000 apysc-4.4.3/apysc/_material_design/icon/material_stop_outlined_icon.py
+-rw-r--r--   0 runner    (1001) docker     (127)     1401 2024-05-29 12:24:48.000000 apysc-4.4.3/apysc/_material_design/icon/material_stop_screen_share_icon.py
+-rw-r--r--   0 runner    (1001) docker     (127)     1444 2024-05-29 12:24:48.000000 apysc-4.4.3/apysc/_material_design/icon/material_stop_screen_share_outlined_icon.py
+-rw-r--r--   0 runner    (1001) docker     (127)     1102 2024-05-29 12:24:48.000000 apysc-4.4.3/apysc/_material_design/icon/material_store_icon.py
+-rw-r--r--   0 runner    (1001) docker     (127)     1158 2024-05-29 12:24:48.000000 apysc-4.4.3/apysc/_material_design/icon/material_store_outlined_icon.py
+-rw-r--r--   0 runner    (1001) docker     (127)     1095 2024-05-29 12:24:48.000000 apysc-4.4.3/apysc/_material_design/icon/material_subject_icon.py
+-rw-r--r--   0 runner    (1001) docker     (127)     1123 2024-05-29 12:24:48.000000 apysc-4.4.3/apysc/_material_design/icon/material_subject_outlined_icon.py
+-rw-r--r--   0 runner    (1001) docker     (127)     1183 2024-05-29 12:24:48.000000 apysc-4.4.3/apysc/_material_design/icon/material_subscriptions_icon.py
+-rw-r--r--   0 runner    (1001) docker     (127)     1217 2024-05-29 12:24:48.000000 apysc-4.4.3/apysc/_material_design/icon/material_subscriptions_outlined_icon.py
+-rw-r--r--   0 runner    (1001) docker     (127)     1178 2024-05-29 12:24:48.000000 apysc-4.4.3/apysc/_material_design/icon/material_subtitles_icon.py
+-rw-r--r--   0 runner    (1001) docker     (127)     1362 2024-05-29 12:24:48.000000 apysc-4.4.3/apysc/_material_design/icon/material_subtitles_off_icon.py
+-rw-r--r--   0 runner    (1001) docker     (127)     1444 2024-05-29 12:24:48.000000 apysc-4.4.3/apysc/_material_design/icon/material_subtitles_off_outlined_icon.py
+-rw-r--r--   0 runner    (1001) docker     (127)     1209 2024-05-29 12:24:48.000000 apysc-4.4.3/apysc/_material_design/icon/material_subtitles_outlined_icon.py
+-rw-r--r--   0 runner    (1001) docker     (127)     1609 2024-05-29 12:24:48.000000 apysc-4.4.3/apysc/_material_design/icon/material_supervised_user_circle_icon.py
+-rw-r--r--   0 runner    (1001) docker     (127)     1661 2024-05-29 12:24:48.000000 apysc-4.4.3/apysc/_material_design/icon/material_supervised_user_circle_outlined_icon.py
+-rw-r--r--   0 runner    (1001) docker     (127)     1381 2024-05-29 12:24:48.000000 apysc-4.4.3/apysc/_material_design/icon/material_supervisor_account_icon.py
+-rw-r--r--   0 runner    (1001) docker     (127)     1585 2024-05-29 12:24:48.000000 apysc-4.4.3/apysc/_material_design/icon/material_supervisor_account_outlined_icon.py
+-rw-r--r--   0 runner    (1001) docker     (127)     1624 2024-05-29 12:24:48.000000 apysc-4.4.3/apysc/_material_design/icon/material_support_icon.py
+-rw-r--r--   0 runner    (1001) docker     (127)     1650 2024-05-29 12:24:48.000000 apysc-4.4.3/apysc/_material_design/icon/material_support_outlined_icon.py
+-rw-r--r--   0 runner    (1001) docker     (127)     1489 2024-05-29 12:24:48.000000 apysc-4.4.3/apysc/_material_design/icon/material_surround_sound_icon.py
+-rw-r--r--   0 runner    (1001) docker     (127)     1848 2024-05-29 12:24:48.000000 apysc-4.4.3/apysc/_material_design/icon/material_surround_sound_outlined_icon.py
+-rw-r--r--   0 runner    (1001) docker     (127)     1192 2024-05-29 12:24:48.000000 apysc-4.4.3/apysc/_material_design/icon/material_swap_calls_icon.py
+-rw-r--r--   0 runner    (1001) docker     (127)     1220 2024-05-29 12:24:48.000000 apysc-4.4.3/apysc/_material_design/icon/material_swap_calls_outlined_icon.py
+-rw-r--r--   0 runner    (1001) docker     (127)     1113 2024-05-29 12:24:48.000000 apysc-4.4.3/apysc/_material_design/icon/material_swap_horiz_icon.py
+-rw-r--r--   0 runner    (1001) docker     (127)     1141 2024-05-29 12:24:48.000000 apysc-4.4.3/apysc/_material_design/icon/material_swap_horiz_outlined_icon.py
+-rw-r--r--   0 runner    (1001) docker     (127)     1219 2024-05-29 12:24:48.000000 apysc-4.4.3/apysc/_material_design/icon/material_swap_horizontal_circle_icon.py
+-rw-r--r--   0 runner    (1001) docker     (127)     1288 2024-05-29 12:24:48.000000 apysc-4.4.3/apysc/_material_design/icon/material_swap_horizontal_circle_outlined_icon.py
+-rw-r--r--   0 runner    (1001) docker     (127)     1109 2024-05-29 12:24:48.000000 apysc-4.4.3/apysc/_material_design/icon/material_swap_vert_icon.py
+-rw-r--r--   0 runner    (1001) docker     (127)     1206 2024-05-29 12:24:48.000000 apysc-4.4.3/apysc/_material_design/icon/material_swap_vert_outlined_icon.py
+-rw-r--r--   0 runner    (1001) docker     (127)     1207 2024-05-29 12:24:48.000000 apysc-4.4.3/apysc/_material_design/icon/material_swap_vertical_circle_icon.py
+-rw-r--r--   0 runner    (1001) docker     (127)     1285 2024-05-29 12:24:48.000000 apysc-4.4.3/apysc/_material_design/icon/material_swap_vertical_circle_outlined_icon.py
+-rw-r--r--   0 runner    (1001) docker     (127)     1426 2024-05-29 12:24:48.000000 apysc-4.4.3/apysc/_material_design/icon/material_swipe_icon.py
+-rw-r--r--   0 runner    (1001) docker     (127)     1168 2024-05-29 12:24:48.000000 apysc-4.4.3/apysc/_material_design/icon/material_sync_alt_icon.py
+-rw-r--r--   0 runner    (1001) docker     (127)     1194 2024-05-29 12:24:48.000000 apysc-4.4.3/apysc/_material_design/icon/material_sync_alt_outlined_icon.py
+-rw-r--r--   0 runner    (1001) docker     (127)     1200 2024-05-29 12:24:48.000000 apysc-4.4.3/apysc/_material_design/icon/material_system_update_alt_icon.py
+-rw-r--r--   0 runner    (1001) docker     (127)     1365 2024-05-29 12:24:48.000000 apysc-4.4.3/apysc/_material_design/icon/material_system_update_alt_outlined_icon.py
+-rw-r--r--   0 runner    (1001) docker     (127)     1118 2024-05-29 12:24:48.000000 apysc-4.4.3/apysc/_material_design/icon/material_tab_icon.py
+-rw-r--r--   0 runner    (1001) docker     (127)     1161 2024-05-29 12:24:48.000000 apysc-4.4.3/apysc/_material_design/icon/material_tab_outlined_icon.py
+-rw-r--r--   0 runner    (1001) docker     (127)     1321 2024-05-29 12:24:48.000000 apysc-4.4.3/apysc/_material_design/icon/material_tab_unselected_icon.py
+-rw-r--r--   0 runner    (1001) docker     (127)     1349 2024-05-29 12:24:48.000000 apysc-4.4.3/apysc/_material_design/icon/material_tab_unselected_outlined_icon.py
+-rw-r--r--   0 runner    (1001) docker     (127)     1375 2024-05-29 12:24:48.000000 apysc-4.4.3/apysc/_material_design/icon/material_table_view_icon.py
+-rw-r--r--   0 runner    (1001) docker     (127)     1401 2024-05-29 12:24:48.000000 apysc-4.4.3/apysc/_material_design/icon/material_table_view_outlined_icon.py
+-rw-r--r--   0 runner    (1001) docker     (127)     1172 2024-05-29 12:24:48.000000 apysc-4.4.3/apysc/_material_design/icon/material_text_rotate_up_icon.py
+-rw-r--r--   0 runner    (1001) docker     (127)     1227 2024-05-29 12:24:48.000000 apysc-4.4.3/apysc/_material_design/icon/material_text_rotate_up_outlined_icon.py
+-rw-r--r--   0 runner    (1001) docker     (127)     1189 2024-05-29 12:24:48.000000 apysc-4.4.3/apysc/_material_design/icon/material_text_rotate_vertical_icon.py
+-rw-r--r--   0 runner    (1001) docker     (127)     1239 2024-05-29 12:24:48.000000 apysc-4.4.3/apysc/_material_design/icon/material_text_rotate_vertical_outlined_icon.py
+-rw-r--r--   0 runner    (1001) docker     (127)     1281 2024-05-29 12:24:48.000000 apysc-4.4.3/apysc/_material_design/icon/material_text_rotation_angledown_icon.py
+-rw-r--r--   0 runner    (1001) docker     (127)     1335 2024-05-29 12:24:48.000000 apysc-4.4.3/apysc/_material_design/icon/material_text_rotation_angledown_outlined_icon.py
+-rw-r--r--   0 runner    (1001) docker     (127)     1274 2024-05-29 12:24:48.000000 apysc-4.4.3/apysc/_material_design/icon/material_text_rotation_angleup_icon.py
+-rw-r--r--   0 runner    (1001) docker     (127)     1327 2024-05-29 12:24:48.000000 apysc-4.4.3/apysc/_material_design/icon/material_text_rotation_angleup_outlined_icon.py
+-rw-r--r--   0 runner    (1001) docker     (127)     1180 2024-05-29 12:24:48.000000 apysc-4.4.3/apysc/_material_design/icon/material_text_rotation_down_icon.py
+-rw-r--r--   0 runner    (1001) docker     (127)     1234 2024-05-29 12:24:48.000000 apysc-4.4.3/apysc/_material_design/icon/material_text_rotation_down_outlined_icon.py
+-rw-r--r--   0 runner    (1001) docker     (127)     1181 2024-05-29 12:24:48.000000 apysc-4.4.3/apysc/_material_design/icon/material_text_rotation_none_icon.py
+-rw-r--r--   0 runner    (1001) docker     (127)     1206 2024-05-29 12:24:48.000000 apysc-4.4.3/apysc/_material_design/icon/material_text_rotation_none_outlined_icon.py
+-rw-r--r--   0 runner    (1001) docker     (127)     1149 2024-05-29 12:24:48.000000 apysc-4.4.3/apysc/_material_design/icon/material_textsms_icon.py
+-rw-r--r--   0 runner    (1001) docker     (127)     1184 2024-05-29 12:24:48.000000 apysc-4.4.3/apysc/_material_design/icon/material_textsms_outlined_icon.py
+-rw-r--r--   0 runner    (1001) docker     (127)     1175 2024-05-29 12:24:48.000000 apysc-4.4.3/apysc/_material_design/icon/material_theaters_icon.py
+-rw-r--r--   0 runner    (1001) docker     (127)     1218 2024-05-29 12:24:48.000000 apysc-4.4.3/apysc/_material_design/icon/material_theaters_outlined_icon.py
+-rw-r--r--   0 runner    (1001) docker     (127)     1238 2024-05-29 12:24:48.000000 apysc-4.4.3/apysc/_material_design/icon/material_thumb_down_icon.py
+-rw-r--r--   0 runner    (1001) docker     (127)     1447 2024-05-29 12:24:48.000000 apysc-4.4.3/apysc/_material_design/icon/material_thumb_down_off_alt_icon.py
+-rw-r--r--   0 runner    (1001) docker     (127)     1317 2024-05-29 12:24:48.000000 apysc-4.4.3/apysc/_material_design/icon/material_thumb_down_outlined_icon.py
+-rw-r--r--   0 runner    (1001) docker     (127)     1237 2024-05-29 12:24:48.000000 apysc-4.4.3/apysc/_material_design/icon/material_thumb_up_icon.py
+-rw-r--r--   0 runner    (1001) docker     (127)     1442 2024-05-29 12:24:48.000000 apysc-4.4.3/apysc/_material_design/icon/material_thumb_up_off_alt_icon.py
+-rw-r--r--   0 runner    (1001) docker     (127)     1308 2024-05-29 12:24:48.000000 apysc-4.4.3/apysc/_material_design/icon/material_thumb_up_outlined_icon.py
+-rw-r--r--   0 runner    (1001) docker     (127)     1435 2024-05-29 12:24:48.000000 apysc-4.4.3/apysc/_material_design/icon/material_thumbs_up_down_icon.py
+-rw-r--r--   0 runner    (1001) docker     (127)     1581 2024-05-29 12:24:48.000000 apysc-4.4.3/apysc/_material_design/icon/material_thumbs_up_down_outlined_icon.py
+-rw-r--r--   0 runner    (1001) docker     (127)     1611 2024-05-29 12:24:48.000000 apysc-4.4.3/apysc/_material_design/icon/material_timeline_icon.py
+-rw-r--r--   0 runner    (1001) docker     (127)     1650 2024-05-29 12:24:48.000000 apysc-4.4.3/apysc/_material_design/icon/material_timeline_outlined_icon.py
+-rw-r--r--   0 runner    (1001) docker     (127)     1112 2024-05-29 12:24:48.000000 apysc-4.4.3/apysc/_material_design/icon/material_toc_icon.py
+-rw-r--r--   0 runner    (1001) docker     (127)     1155 2024-05-29 12:24:48.000000 apysc-4.4.3/apysc/_material_design/icon/material_toc_outlined_icon.py
+-rw-r--r--   0 runner    (1001) docker     (127)     1159 2024-05-29 12:24:48.000000 apysc-4.4.3/apysc/_material_design/icon/material_today_icon.py
+-rw-r--r--   0 runner    (1001) docker     (127)     1195 2024-05-29 12:24:48.000000 apysc-4.4.3/apysc/_material_design/icon/material_today_outlined_icon.py
+-rw-r--r--   0 runner    (1001) docker     (127)     1259 2024-05-29 12:24:48.000000 apysc-4.4.3/apysc/_material_design/icon/material_toll_icon.py
+-rw-r--r--   0 runner    (1001) docker     (127)     1273 2024-05-29 12:24:48.000000 apysc-4.4.3/apysc/_material_design/icon/material_toll_outlined_icon.py
+-rw-r--r--   0 runner    (1001) docker     (127)     1577 2024-05-29 12:24:48.000000 apysc-4.4.3/apysc/_material_design/icon/material_touch_app_icon.py
+-rw-r--r--   0 runner    (1001) docker     (127)     1777 2024-05-29 12:24:48.000000 apysc-4.4.3/apysc/_material_design/icon/material_touch_app_outlined_icon.py
+-rw-r--r--   0 runner    (1001) docker     (127)     1106 2024-05-29 12:24:48.000000 apysc-4.4.3/apysc/_material_design/icon/material_tour_icon.py
+-rw-r--r--   0 runner    (1001) docker     (127)     1269 2024-05-29 12:24:48.000000 apysc-4.4.3/apysc/_material_design/icon/material_tour_outlined_icon.py
+-rw-r--r--   0 runner    (1001) docker     (127)     1473 2024-05-29 12:24:48.000000 apysc-4.4.3/apysc/_material_design/icon/material_track_changes_icon.py
+-rw-r--r--   0 runner    (1001) docker     (127)     1499 2024-05-29 12:24:48.000000 apysc-4.4.3/apysc/_material_design/icon/material_track_changes_outlined_icon.py
+-rw-r--r--   0 runner    (1001) docker     (127)     1336 2024-05-29 12:24:48.000000 apysc-4.4.3/apysc/_material_design/icon/material_translate_icon.py
+-rw-r--r--   0 runner    (1001) docker     (127)     1364 2024-05-29 12:24:48.000000 apysc-4.4.3/apysc/_material_design/icon/material_translate_outlined_icon.py
+-rw-r--r--   0 runner    (1001) docker     (127)     1121 2024-05-29 12:24:48.000000 apysc-4.4.3/apysc/_material_design/icon/material_trending_down_icon.py
+-rw-r--r--   0 runner    (1001) docker     (127)     1152 2024-05-29 12:24:48.000000 apysc-4.4.3/apysc/_material_design/icon/material_trending_down_outlined_icon.py
+-rw-r--r--   0 runner    (1001) docker     (127)     1074 2024-05-29 12:24:48.000000 apysc-4.4.3/apysc/_material_design/icon/material_trending_flat_icon.py
+-rw-r--r--   0 runner    (1001) docker     (127)     1106 2024-05-29 12:24:48.000000 apysc-4.4.3/apysc/_material_design/icon/material_trending_flat_outlined_icon.py
+-rw-r--r--   0 runner    (1001) docker     (127)     1116 2024-05-29 12:24:48.000000 apysc-4.4.3/apysc/_material_design/icon/material_trending_up_icon.py
+-rw-r--r--   0 runner    (1001) docker     (127)     1147 2024-05-29 12:24:48.000000 apysc-4.4.3/apysc/_material_design/icon/material_trending_up_outlined_icon.py
+-rw-r--r--   0 runner    (1001) docker     (127)     1098 2024-05-29 12:24:48.000000 apysc-4.4.3/apysc/_material_design/icon/material_turned_in_icon.py
+-rw-r--r--   0 runner    (1001) docker     (127)     1136 2024-05-29 12:24:48.000000 apysc-4.4.3/apysc/_material_design/icon/material_turned_in_not_icon.py
+-rw-r--r--   0 runner    (1001) docker     (127)     1164 2024-05-29 12:24:48.000000 apysc-4.4.3/apysc/_material_design/icon/material_turned_in_not_outlined_icon.py
+-rw-r--r--   0 runner    (1001) docker     (127)     1126 2024-05-29 12:24:48.000000 apysc-4.4.3/apysc/_material_design/icon/material_turned_in_outlined_icon.py
+-rw-r--r--   0 runner    (1001) docker     (127)     1434 2024-05-29 12:24:48.000000 apysc-4.4.3/apysc/_material_design/icon/material_unpublished_icon.py
+-rw-r--r--   0 runner    (1001) docker     (127)     1651 2024-05-29 12:24:48.000000 apysc-4.4.3/apysc/_material_design/icon/material_unpublished_outlined_icon.py
+-rw-r--r--   0 runner    (1001) docker     (127)     1273 2024-05-29 12:24:48.000000 apysc-4.4.3/apysc/_material_design/icon/material_unsubscribe_icon.py
+-rw-r--r--   0 runner    (1001) docker     (127)     1347 2024-05-29 12:24:48.000000 apysc-4.4.3/apysc/_material_design/icon/material_unsubscribe_outlined_icon.py
+-rw-r--r--   0 runner    (1001) docker     (127)     1399 2024-05-29 12:24:48.000000 apysc-4.4.3/apysc/_material_design/icon/material_update_icon.py
+-rw-r--r--   0 runner    (1001) docker     (127)     1328 2024-05-29 12:24:48.000000 apysc-4.4.3/apysc/_material_design/icon/material_update_outlined_icon.py
+-rw-r--r--   0 runner    (1001) docker     (127)     1134 2024-05-29 12:24:48.000000 apysc-4.4.3/apysc/_material_design/icon/material_upgrade_icon.py
+-rw-r--r--   0 runner    (1001) docker     (127)     1160 2024-05-29 12:24:48.000000 apysc-4.4.3/apysc/_material_design/icon/material_upgrade_outlined_icon.py
+-rw-r--r--   0 runner    (1001) docker     (127)     1358 2024-05-29 12:24:48.000000 apysc-4.4.3/apysc/_material_design/icon/material_verified_icon.py
+-rw-r--r--   0 runner    (1001) docker     (127)     1839 2024-05-29 12:24:48.000000 apysc-4.4.3/apysc/_material_design/icon/material_verified_outlined_icon.py
+-rw-r--r--   0 runner    (1001) docker     (127)     1166 2024-05-29 12:24:48.000000 apysc-4.4.3/apysc/_material_design/icon/material_verified_user_icon.py
+-rw-r--r--   0 runner    (1001) docker     (127)     1261 2024-05-29 12:24:48.000000 apysc-4.4.3/apysc/_material_design/icon/material_verified_user_outlined_icon.py
+-rw-r--r--   0 runner    (1001) docker     (127)     1127 2024-05-29 12:24:48.000000 apysc-4.4.3/apysc/_material_design/icon/material_vertical_split_icon.py
+-rw-r--r--   0 runner    (1001) docker     (127)     1157 2024-05-29 12:24:48.000000 apysc-4.4.3/apysc/_material_design/icon/material_vertical_split_outlined_icon.py
+-rw-r--r--   0 runner    (1001) docker     (127)     1179 2024-05-29 12:24:48.000000 apysc-4.4.3/apysc/_material_design/icon/material_video_call_icon.py
+-rw-r--r--   0 runner    (1001) docker     (127)     1218 2024-05-29 12:24:48.000000 apysc-4.4.3/apysc/_material_design/icon/material_video_call_outlined_icon.py
+-rw-r--r--   0 runner    (1001) docker     (127)     1139 2024-05-29 12:24:48.000000 apysc-4.4.3/apysc/_material_design/icon/material_video_label_icon.py
+-rw-r--r--   0 runner    (1001) docker     (127)     1165 2024-05-29 12:24:48.000000 apysc-4.4.3/apysc/_material_design/icon/material_video_label_outlined_icon.py
+-rw-r--r--   0 runner    (1001) docker     (127)     1185 2024-05-29 12:24:48.000000 apysc-4.4.3/apysc/_material_design/icon/material_video_library_icon.py
+-rw-r--r--   0 runner    (1001) docker     (127)     1221 2024-05-29 12:24:48.000000 apysc-4.4.3/apysc/_material_design/icon/material_video_library_outlined_icon.py
+-rw-r--r--   0 runner    (1001) docker     (127)     2049 2024-05-29 12:24:48.000000 apysc-4.4.3/apysc/_material_design/icon/material_video_settings_icon.py
+-rw-r--r--   0 runner    (1001) docker     (127)     2075 2024-05-29 12:24:48.000000 apysc-4.4.3/apysc/_material_design/icon/material_video_settings_outlined_icon.py
+-rw-r--r--   0 runner    (1001) docker     (127)     1138 2024-05-29 12:24:48.000000 apysc-4.4.3/apysc/_material_design/icon/material_videocam_icon.py
+-rw-r--r--   0 runner    (1001) docker     (127)     1218 2024-05-29 12:24:48.000000 apysc-4.4.3/apysc/_material_design/icon/material_videocam_off_icon.py
+-rw-r--r--   0 runner    (1001) docker     (127)     1284 2024-05-29 12:24:48.000000 apysc-4.4.3/apysc/_material_design/icon/material_videocam_off_outlined_icon.py
+-rw-r--r--   0 runner    (1001) docker     (127)     1176 2024-05-29 12:24:48.000000 apysc-4.4.3/apysc/_material_design/icon/material_videocam_outlined_icon.py
+-rw-r--r--   0 runner    (1001) docker     (127)     1205 2024-05-29 12:24:48.000000 apysc-4.4.3/apysc/_material_design/icon/material_view_agenda_icon.py
+-rw-r--r--   0 runner    (1001) docker     (127)     1261 2024-05-29 12:24:48.000000 apysc-4.4.3/apysc/_material_design/icon/material_view_agenda_outlined_icon.py
+-rw-r--r--   0 runner    (1001) docker     (127)     1088 2024-05-29 12:24:48.000000 apysc-4.4.3/apysc/_material_design/icon/material_view_array_icon.py
+-rw-r--r--   0 runner    (1001) docker     (127)     1128 2024-05-29 12:24:48.000000 apysc-4.4.3/apysc/_material_design/icon/material_view_array_outlined_icon.py
+-rw-r--r--   0 runner    (1001) docker     (127)     1098 2024-05-29 12:24:48.000000 apysc-4.4.3/apysc/_material_design/icon/material_view_carousel_icon.py
+-rw-r--r--   0 runner    (1001) docker     (127)     1134 2024-05-29 12:24:48.000000 apysc-4.4.3/apysc/_material_design/icon/material_view_carousel_outlined_icon.py
+-rw-r--r--   0 runner    (1001) docker     (127)     1093 2024-05-29 12:24:48.000000 apysc-4.4.3/apysc/_material_design/icon/material_view_column_icon.py
+-rw-r--r--   0 runner    (1001) docker     (127)     1131 2024-05-29 12:24:48.000000 apysc-4.4.3/apysc/_material_design/icon/material_view_column_outlined_icon.py
+-rw-r--r--   0 runner    (1001) docker     (127)     1145 2024-05-29 12:24:48.000000 apysc-4.4.3/apysc/_material_design/icon/material_view_day_icon.py
+-rw-r--r--   0 runner    (1001) docker     (127)     1188 2024-05-29 12:24:48.000000 apysc-4.4.3/apysc/_material_design/icon/material_view_day_outlined_icon.py
+-rw-r--r--   0 runner    (1001) docker     (127)     1112 2024-05-29 12:24:48.000000 apysc-4.4.3/apysc/_material_design/icon/material_view_headline_icon.py
+-rw-r--r--   0 runner    (1001) docker     (127)     1138 2024-05-29 12:24:48.000000 apysc-4.4.3/apysc/_material_design/icon/material_view_headline_outlined_icon.py
+-rw-r--r--   0 runner    (1001) docker     (127)     1508 2024-05-29 12:24:48.000000 apysc-4.4.3/apysc/_material_design/icon/material_view_in_ar_icon.py
+-rw-r--r--   0 runner    (1001) docker     (127)     1125 2024-05-29 12:24:48.000000 apysc-4.4.3/apysc/_material_design/icon/material_view_list_icon.py
+-rw-r--r--   0 runner    (1001) docker     (127)     1180 2024-05-29 12:24:48.000000 apysc-4.4.3/apysc/_material_design/icon/material_view_list_outlined_icon.py
+-rw-r--r--   0 runner    (1001) docker     (127)     1132 2024-05-29 12:24:48.000000 apysc-4.4.3/apysc/_material_design/icon/material_view_module_icon.py
+-rw-r--r--   0 runner    (1001) docker     (127)     1192 2024-05-29 12:24:48.000000 apysc-4.4.3/apysc/_material_design/icon/material_view_module_outlined_icon.py
+-rw-r--r--   0 runner    (1001) docker     (127)     1106 2024-05-29 12:24:48.000000 apysc-4.4.3/apysc/_material_design/icon/material_view_quilt_icon.py
+-rw-r--r--   0 runner    (1001) docker     (127)     1154 2024-05-29 12:24:48.000000 apysc-4.4.3/apysc/_material_design/icon/material_view_quilt_outlined_icon.py
+-rw-r--r--   0 runner    (1001) docker     (127)     1165 2024-05-29 12:24:48.000000 apysc-4.4.3/apysc/_material_design/icon/material_view_sidebar_icon.py
+-rw-r--r--   0 runner    (1001) docker     (127)     1244 2024-05-29 12:24:48.000000 apysc-4.4.3/apysc/_material_design/icon/material_view_sidebar_outlined_icon.py
+-rw-r--r--   0 runner    (1001) docker     (127)     1075 2024-05-29 12:24:48.000000 apysc-4.4.3/apysc/_material_design/icon/material_view_stream_icon.py
+-rw-r--r--   0 runner    (1001) docker     (127)     1120 2024-05-29 12:24:48.000000 apysc-4.4.3/apysc/_material_design/icon/material_view_stream_outlined_icon.py
+-rw-r--r--   0 runner    (1001) docker     (127)     1277 2024-05-29 12:24:48.000000 apysc-4.4.3/apysc/_material_design/icon/material_view_week_icon.py
+-rw-r--r--   0 runner    (1001) docker     (127)     1192 2024-05-29 12:24:48.000000 apysc-4.4.3/apysc/_material_design/icon/material_view_week_outlined_icon.py
+-rw-r--r--   0 runner    (1001) docker     (127)     1252 2024-05-29 12:24:48.000000 apysc-4.4.3/apysc/_material_design/icon/material_visibility_icon.py
+-rw-r--r--   0 runner    (1001) docker     (127)     1598 2024-05-29 12:24:48.000000 apysc-4.4.3/apysc/_material_design/icon/material_visibility_off_icon.py
+-rw-r--r--   0 runner    (1001) docker     (127)     1824 2024-05-29 12:24:48.000000 apysc-4.4.3/apysc/_material_design/icon/material_visibility_off_outlined_icon.py
+-rw-r--r--   0 runner    (1001) docker     (127)     1405 2024-05-29 12:24:48.000000 apysc-4.4.3/apysc/_material_design/icon/material_visibility_outlined_icon.py
+-rw-r--r--   0 runner    (1001) docker     (127)     1485 2024-05-29 12:24:48.000000 apysc-4.4.3/apysc/_material_design/icon/material_voice_over_off_icon.py
+-rw-r--r--   0 runner    (1001) docker     (127)     1620 2024-05-29 12:24:48.000000 apysc-4.4.3/apysc/_material_design/icon/material_voice_over_off_outlined_icon.py
+-rw-r--r--   0 runner    (1001) docker     (127)     1371 2024-05-29 12:24:48.000000 apysc-4.4.3/apysc/_material_design/icon/material_voicemail_icon.py
+-rw-r--r--   0 runner    (1001) docker     (127)     1399 2024-05-29 12:24:48.000000 apysc-4.4.3/apysc/_material_design/icon/material_voicemail_outlined_icon.py
+-rw-r--r--   0 runner    (1001) docker     (127)     1133 2024-05-29 12:24:48.000000 apysc-4.4.3/apysc/_material_design/icon/material_volume_down_icon.py
+-rw-r--r--   0 runner    (1001) docker     (127)     1199 2024-05-29 12:24:48.000000 apysc-4.4.3/apysc/_material_design/icon/material_volume_down_outlined_icon.py
+-rw-r--r--   0 runner    (1001) docker     (127)     1067 2024-05-29 12:24:48.000000 apysc-4.4.3/apysc/_material_design/icon/material_volume_mute_icon.py
+-rw-r--r--   0 runner    (1001) docker     (127)     1136 2024-05-29 12:24:48.000000 apysc-4.4.3/apysc/_material_design/icon/material_volume_mute_outlined_icon.py
+-rw-r--r--   0 runner    (1001) docker     (127)     1393 2024-05-29 12:24:48.000000 apysc-4.4.3/apysc/_material_design/icon/material_volume_off_icon.py
+-rw-r--r--   0 runner    (1001) docker     (127)     1480 2024-05-29 12:24:48.000000 apysc-4.4.3/apysc/_material_design/icon/material_volume_off_outlined_icon.py
+-rw-r--r--   0 runner    (1001) docker     (127)     1226 2024-05-29 12:24:48.000000 apysc-4.4.3/apysc/_material_design/icon/material_volume_up_icon.py
+-rw-r--r--   0 runner    (1001) docker     (127)     1299 2024-05-29 12:24:48.000000 apysc-4.4.3/apysc/_material_design/icon/material_volume_up_outlined_icon.py
+-rw-r--r--   0 runner    (1001) docker     (127)     1189 2024-05-29 12:24:48.000000 apysc-4.4.3/apysc/_material_design/icon/material_vpn_key_icon.py
+-rw-r--r--   0 runner    (1001) docker     (127)     1400 2024-05-29 12:24:48.000000 apysc-4.4.3/apysc/_material_design/icon/material_vpn_key_outlined_icon.py
+-rw-r--r--   0 runner    (1001) docker     (127)     1120 2024-05-29 12:24:48.000000 apysc-4.4.3/apysc/_material_design/icon/material_warning_amber_outlined_icon.py
+-rw-r--r--   0 runner    (1001) docker     (127)     1084 2024-05-29 12:24:48.000000 apysc-4.4.3/apysc/_material_design/icon/material_warning_icon.py
+-rw-r--r--   0 runner    (1001) docker     (127)     1073 2024-05-29 12:24:48.000000 apysc-4.4.3/apysc/_material_design/icon/material_warning_outlined_icon.py
+-rw-r--r--   0 runner    (1001) docker     (127)     1219 2024-05-29 12:24:48.000000 apysc-4.4.3/apysc/_material_design/icon/material_watch_later_icon.py
+-rw-r--r--   0 runner    (1001) docker     (127)     1304 2024-05-29 12:24:48.000000 apysc-4.4.3/apysc/_material_design/icon/material_watch_later_outlined_icon.py
+-rw-r--r--   0 runner    (1001) docker     (127)     1134 2024-05-29 12:24:48.000000 apysc-4.4.3/apysc/_material_design/icon/material_web_asset_icon.py
+-rw-r--r--   0 runner    (1001) docker     (127)     1162 2024-05-29 12:24:48.000000 apysc-4.4.3/apysc/_material_design/icon/material_web_asset_outlined_icon.py
+-rw-r--r--   0 runner    (1001) docker     (127)     1150 2024-05-29 12:24:48.000000 apysc-4.4.3/apysc/_material_design/icon/material_web_icon.py
+-rw-r--r--   0 runner    (1001) docker     (127)     1350 2024-05-29 12:24:48.000000 apysc-4.4.3/apysc/_material_design/icon/material_web_outlined_icon.py
+-rw-r--r--   0 runner    (1001) docker     (127)     1482 2024-05-29 12:24:48.000000 apysc-4.4.3/apysc/_material_design/icon/material_wifi_calling_icon.py
+-rw-r--r--   0 runner    (1001) docker     (127)     1714 2024-05-29 12:24:48.000000 apysc-4.4.3/apysc/_material_design/icon/material_wifi_calling_outlined_icon.py
+-rw-r--r--   0 runner    (1001) docker     (127)     1451 2024-05-29 12:24:48.000000 apysc-4.4.3/apysc/_material_design/icon/material_wifi_protected_setup_icon.py
+-rw-r--r--   0 runner    (1001) docker     (127)     1477 2024-05-29 12:24:48.000000 apysc-4.4.3/apysc/_material_design/icon/material_wifi_protected_setup_outlined_icon.py
+-rw-r--r--   0 runner    (1001) docker     (127)     1176 2024-05-29 12:24:48.000000 apysc-4.4.3/apysc/_material_design/icon/material_work_icon.py
+-rw-r--r--   0 runner    (1001) docker     (127)     1301 2024-05-29 12:24:48.000000 apysc-4.4.3/apysc/_material_design/icon/material_work_off_icon.py
+-rw-r--r--   0 runner    (1001) docker     (127)     1293 2024-05-29 12:24:48.000000 apysc-4.4.3/apysc/_material_design/icon/material_work_off_outlined_icon.py
+-rw-r--r--   0 runner    (1001) docker     (127)     1230 2024-05-29 12:24:48.000000 apysc-4.4.3/apysc/_material_design/icon/material_work_outline_icon.py
+-rw-r--r--   0 runner    (1001) docker     (127)     1238 2024-05-29 12:24:48.000000 apysc-4.4.3/apysc/_material_design/icon/material_work_outline_outlined_icon.py
+-rw-r--r--   0 runner    (1001) docker     (127)     1204 2024-05-29 12:24:48.000000 apysc-4.4.3/apysc/_material_design/icon/material_work_outlined_icon.py
+-rw-r--r--   0 runner    (1001) docker     (127)     1222 2024-05-29 12:24:48.000000 apysc-4.4.3/apysc/_material_design/icon/material_wysiwyg_icon.py
+-rw-r--r--   0 runner    (1001) docker     (127)     1248 2024-05-29 12:24:48.000000 apysc-4.4.3/apysc/_material_design/icon/material_wysiwyg_outlined_icon.py
+-rw-r--r--   0 runner    (1001) docker     (127)     1378 2024-05-29 12:24:48.000000 apysc-4.4.3/apysc/_material_design/icon/material_youtube_searched_for_icon.py
+-rw-r--r--   0 runner    (1001) docker     (127)     1404 2024-05-29 12:24:48.000000 apysc-4.4.3/apysc/_material_design/icon/material_youtube_searched_for_outlined_icon.py
+-rw-r--r--   0 runner    (1001) docker     (127)     1314 2024-05-29 12:24:48.000000 apysc-4.4.3/apysc/_material_design/icon/material_zoom_in_icon.py
+-rw-r--r--   0 runner    (1001) docker     (127)     1325 2024-05-29 12:24:48.000000 apysc-4.4.3/apysc/_material_design/icon/material_zoom_in_outlined_icon.py
+-rw-r--r--   0 runner    (1001) docker     (127)     1283 2024-05-29 12:24:48.000000 apysc-4.4.3/apysc/_material_design/icon/material_zoom_out_icon.py
+-rw-r--r--   0 runner    (1001) docker     (127)     1309 2024-05-29 12:24:48.000000 apysc-4.4.3/apysc/_material_design/icon/material_zoom_out_outlined_icon.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-29 12:25:10.155791 apysc-4.4.3/apysc/_math/
+-rw-r--r--   0 runner    (1001) docker     (127)        0 2024-05-29 12:24:48.000000 apysc-4.4.3/apysc/_math/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (127)     2476 2024-05-29 12:24:48.000000 apysc-4.4.3/apysc/_math/clamp_mixin.py
+-rw-r--r--   0 runner    (1001) docker     (127)      375 2024-05-29 12:24:48.000000 apysc-4.4.3/apysc/_math/math.py
+-rw-r--r--   0 runner    (1001) docker     (127)     3458 2024-05-29 12:24:48.000000 apysc-4.4.3/apysc/_math/max_mixin.py
+-rw-r--r--   0 runner    (1001) docker     (127)     3471 2024-05-29 12:24:48.000000 apysc-4.4.3/apysc/_math/min_mixin.py
+-rw-r--r--   0 runner    (1001) docker     (127)     2510 2024-05-29 12:24:48.000000 apysc-4.4.3/apysc/_math/trunc_mixin.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-29 12:25:10.155791 apysc-4.4.3/apysc/_string/
+-rw-r--r--   0 runner    (1001) docker     (127)        0 2024-05-29 12:24:48.000000 apysc-4.4.3/apysc/_string/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (127)     1596 2024-05-29 12:24:48.000000 apysc-4.4.3/apysc/_string/indent_util.py
+-rw-r--r--   0 runner    (1001) docker     (127)     3453 2024-05-29 12:24:48.000000 apysc-4.4.3/apysc/_string/string_util.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-29 12:25:10.155791 apysc-4.4.3/apysc/_testing/
+-rw-r--r--   0 runner    (1001) docker     (127)        0 2024-05-29 12:24:48.000000 apysc-4.4.3/apysc/_testing/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (127)     9001 2024-05-29 12:24:48.000000 apysc-4.4.3/apysc/_testing/e2e_testing_helper.py
+-rw-r--r--   0 runner    (1001) docker     (127)     6350 2024-05-29 12:24:48.000000 apysc-4.4.3/apysc/_testing/testing_helper.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-29 12:25:10.159791 apysc-4.4.3/apysc/_time/
+-rw-r--r--   0 runner    (1001) docker     (127)        0 2024-05-29 12:24:48.000000 apysc-4.4.3/apysc/_time/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (127)    10971 2024-05-29 12:24:48.000000 apysc-4.4.3/apysc/_time/datetime_.py
+-rw-r--r--   0 runner    (1001) docker     (127)     5188 2024-05-29 12:24:48.000000 apysc-4.4.3/apysc/_time/day_mixin.py
+-rw-r--r--   0 runner    (1001) docker     (127)     3556 2024-05-29 12:24:48.000000 apysc-4.4.3/apysc/_time/days_mixin.py
+-rw-r--r--   0 runner    (1001) docker     (127)     2181 2024-05-29 12:24:48.000000 apysc-4.4.3/apysc/_time/fps.py
+-rw-r--r--   0 runner    (1001) docker     (127)     5426 2024-05-29 12:24:48.000000 apysc-4.4.3/apysc/_time/hour_mixin.py
+-rw-r--r--   0 runner    (1001) docker     (127)     2097 2024-05-29 12:24:48.000000 apysc-4.4.3/apysc/_time/left_and_right_datetimes_mixin.py
+-rw-r--r--   0 runner    (1001) docker     (127)     5976 2024-05-29 12:24:48.000000 apysc-4.4.3/apysc/_time/millisecond_mixin.py
+-rw-r--r--   0 runner    (1001) docker     (127)     5639 2024-05-29 12:24:48.000000 apysc-4.4.3/apysc/_time/minute_mixin.py
+-rw-r--r--   0 runner    (1001) docker     (127)     1541 2024-05-29 12:24:48.000000 apysc-4.4.3/apysc/_time/month_end_mixin.py
+-rw-r--r--   0 runner    (1001) docker     (127)     5423 2024-05-29 12:24:48.000000 apysc-4.4.3/apysc/_time/month_mixin.py
+-rw-r--r--   0 runner    (1001) docker     (127)     2567 2024-05-29 12:24:48.000000 apysc-4.4.3/apysc/_time/now_mixin.py
+-rw-r--r--   0 runner    (1001) docker     (127)     5610 2024-05-29 12:24:48.000000 apysc-4.4.3/apysc/_time/second_mixin.py
+-rw-r--r--   0 runner    (1001) docker     (127)     5857 2024-05-29 12:24:48.000000 apysc-4.4.3/apysc/_time/timedelta_.py
+-rw-r--r--   0 runner    (1001) docker     (127)    22600 2024-05-29 12:24:48.000000 apysc-4.4.3/apysc/_time/timer.py
+-rw-r--r--   0 runner    (1001) docker     (127)     3884 2024-05-29 12:24:48.000000 apysc-4.4.3/apysc/_time/total_seconds_mixin.py
+-rw-r--r--   0 runner    (1001) docker     (127)     5685 2024-05-29 12:24:48.000000 apysc-4.4.3/apysc/_time/weekday_mixin.py
+-rw-r--r--   0 runner    (1001) docker     (127)     5502 2024-05-29 12:24:48.000000 apysc-4.4.3/apysc/_time/year_mixin.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-29 12:25:10.159791 apysc-4.4.3/apysc/_translation/
+-rw-r--r--   0 runner    (1001) docker     (127)        0 2024-05-29 12:24:48.000000 apysc-4.4.3/apysc/_translation/__init__.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-29 12:25:10.187791 apysc-4.4.3/apysc/_translation/jp/
+-rw-r--r--   0 runner    (1001) docker     (127)        0 2024-05-29 12:24:48.000000 apysc-4.4.3/apysc/_translation/jp/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (127)     4745 2024-05-29 12:24:48.000000 apysc-4.4.3/apysc/_translation/jp/about_handler_options_type.py
+-rw-r--r--   0 runner    (1001) docker     (127)    15519 2024-05-29 12:24:48.000000 apysc-4.4.3/apysc/_translation/jp/add_child_and_remove_child.py
+-rw-r--r--   0 runner    (1001) docker     (127)     7887 2024-05-29 12:24:48.000000 apysc-4.4.3/apysc/_translation/jp/add_debug_info_setting.py
+-rw-r--r--   0 runner    (1001) docker     (127)     6631 2024-05-29 12:24:48.000000 apysc-4.4.3/apysc/_translation/jp/animation_base_start.py
+-rw-r--r--   0 runner    (1001) docker     (127)     9539 2024-05-29 12:24:48.000000 apysc-4.4.3/apysc/_translation/jp/animation_base_target.py
+-rw-r--r--   0 runner    (1001) docker     (127)    15615 2024-05-29 12:24:48.000000 apysc-4.4.3/apysc/_translation/jp/animation_complete.py
+-rw-r--r--   0 runner    (1001) docker     (127)     5762 2024-05-29 12:24:48.000000 apysc-4.4.3/apysc/_translation/jp/animation_delay.py
+-rw-r--r--   0 runner    (1001) docker     (127)     5628 2024-05-29 12:24:48.000000 apysc-4.4.3/apysc/_translation/jp/animation_duration.py
+-rw-r--r--   0 runner    (1001) docker     (127)    14570 2024-05-29 12:24:48.000000 apysc-4.4.3/apysc/_translation/jp/animation_event.py
+-rw-r--r--   0 runner    (1001) docker     (127)    11149 2024-05-29 12:24:48.000000 apysc-4.4.3/apysc/_translation/jp/animation_fill_alpha.py
+-rw-r--r--   0 runner    (1001) docker     (127)    11581 2024-05-29 12:24:48.000000 apysc-4.4.3/apysc/_translation/jp/animation_fill_color.py
+-rw-r--r--   0 runner    (1001) docker     (127)     8243 2024-05-29 12:24:48.000000 apysc-4.4.3/apysc/_translation/jp/animation_finish.py
+-rw-r--r--   0 runner    (1001) docker     (127)   148271 2024-05-29 12:24:48.000000 apysc-4.4.3/apysc/_translation/jp/animation_interfaces_abstract.py
+-rw-r--r--   0 runner    (1001) docker     (127)    11617 2024-05-29 12:24:48.000000 apysc-4.4.3/apysc/_translation/jp/animation_line_alpha.py
+-rw-r--r--   0 runner    (1001) docker     (127)    11991 2024-05-29 12:24:48.000000 apysc-4.4.3/apysc/_translation/jp/animation_line_color.py
+-rw-r--r--   0 runner    (1001) docker     (127)    11675 2024-05-29 12:24:48.000000 apysc-4.4.3/apysc/_translation/jp/animation_line_thickness.py
+-rw-r--r--   0 runner    (1001) docker     (127)     6146 2024-05-29 12:24:48.000000 apysc-4.4.3/apysc/_translation/jp/animation_method_chaining.py
+-rw-r--r--   0 runner    (1001) docker     (127)    11840 2024-05-29 12:24:48.000000 apysc-4.4.3/apysc/_translation/jp/animation_move.py
+-rw-r--r--   0 runner    (1001) docker     (127)    13951 2024-05-29 12:24:48.000000 apysc-4.4.3/apysc/_translation/jp/animation_parallel.py
+-rw-r--r--   0 runner    (1001) docker     (127)    11297 2024-05-29 12:24:48.000000 apysc-4.4.3/apysc/_translation/jp/animation_pause_and_play.py
+-rw-r--r--   0 runner    (1001) docker     (127)    11296 2024-05-29 12:24:48.000000 apysc-4.4.3/apysc/_translation/jp/animation_radius.py
+-rw-r--r--   0 runner    (1001) docker     (127)     7758 2024-05-29 12:24:48.000000 apysc-4.4.3/apysc/_translation/jp/animation_reset.py
+-rw-r--r--   0 runner    (1001) docker     (127)     6721 2024-05-29 12:24:48.000000 apysc-4.4.3/apysc/_translation/jp/animation_return_value.py
+-rw-r--r--   0 runner    (1001) docker     (127)    11605 2024-05-29 12:24:48.000000 apysc-4.4.3/apysc/_translation/jp/animation_reverse.py
+-rw-r--r--   0 runner    (1001) docker     (127)    12223 2024-05-29 12:24:48.000000 apysc-4.4.3/apysc/_translation/jp/animation_rotation_around_center.py
+-rw-r--r--   0 runner    (1001) docker     (127)    13242 2024-05-29 12:24:48.000000 apysc-4.4.3/apysc/_translation/jp/animation_rotation_around_point.py
+-rw-r--r--   0 runner    (1001) docker     (127)    22762 2024-05-29 12:24:48.000000 apysc-4.4.3/apysc/_translation/jp/animation_scale_x_and_y_from_center.py
+-rw-r--r--   0 runner    (1001) docker     (127)    10821 2024-05-29 12:24:48.000000 apysc-4.4.3/apysc/_translation/jp/animation_scale_x_and_y_from_point.py
+-rw-r--r--   0 runner    (1001) docker     (127)     7337 2024-05-29 12:24:48.000000 apysc-4.4.3/apysc/_translation/jp/animation_time.py
+-rw-r--r--   0 runner    (1001) docker     (127)    24560 2024-05-29 12:24:48.000000 apysc-4.4.3/apysc/_translation/jp/animation_width_and_height.py
+-rw-r--r--   0 runner    (1001) docker     (127)    13175 2024-05-29 12:24:48.000000 apysc-4.4.3/apysc/_translation/jp/animation_x.py
+-rw-r--r--   0 runner    (1001) docker     (127)    13195 2024-05-29 12:24:48.000000 apysc-4.4.3/apysc/_translation/jp/animation_y.py
+-rw-r--r--   0 runner    (1001) docker     (127)     6108 2024-05-29 12:24:48.000000 apysc-4.4.3/apysc/_translation/jp/append_js_expression.py
+-rw-r--r--   0 runner    (1001) docker     (127)    16267 2024-05-29 12:24:48.000000 apysc-4.4.3/apysc/_translation/jp/array.py
+-rw-r--r--   0 runner    (1001) docker     (127)     6138 2024-05-29 12:24:48.000000 apysc-4.4.3/apysc/_translation/jp/array_append_and_push.py
+-rw-r--r--   0 runner    (1001) docker     (127)     1546 2024-05-29 12:24:48.000000 apysc-4.4.3/apysc/_translation/jp/array_clear.py
+-rw-r--r--   0 runner    (1001) docker     (127)     2627 2024-05-29 12:24:48.000000 apysc-4.4.3/apysc/_translation/jp/array_comparison.py
+-rw-r--r--   0 runner    (1001) docker     (127)     8204 2024-05-29 12:24:48.000000 apysc-4.4.3/apysc/_translation/jp/array_extend_and_concat.py
+-rw-r--r--   0 runner    (1001) docker     (127)     4822 2024-05-29 12:24:48.000000 apysc-4.4.3/apysc/_translation/jp/array_index_of.py
+-rw-r--r--   0 runner    (1001) docker     (127)     6996 2024-05-29 12:24:48.000000 apysc-4.4.3/apysc/_translation/jp/array_insert_and_insert_at.py
+-rw-r--r--   0 runner    (1001) docker     (127)     4052 2024-05-29 12:24:48.000000 apysc-4.4.3/apysc/_translation/jp/array_join.py
+-rw-r--r--   0 runner    (1001) docker     (127)     6552 2024-05-29 12:24:48.000000 apysc-4.4.3/apysc/_translation/jp/array_last_value.py
+-rw-r--r--   0 runner    (1001) docker     (127)     4648 2024-05-29 12:24:48.000000 apysc-4.4.3/apysc/_translation/jp/array_length.py
+-rw-r--r--   0 runner    (1001) docker     (127)     3648 2024-05-29 12:24:48.000000 apysc-4.4.3/apysc/_translation/jp/array_pop.py
+-rw-r--r--   0 runner    (1001) docker     (127)     6355 2024-05-29 12:24:48.000000 apysc-4.4.3/apysc/_translation/jp/array_remove_and_remove_at.py
+-rw-r--r--   0 runner    (1001) docker     (127)     3330 2024-05-29 12:24:48.000000 apysc-4.4.3/apysc/_translation/jp/array_reverse.py
+-rw-r--r--   0 runner    (1001) docker     (127)     5547 2024-05-29 12:24:48.000000 apysc-4.4.3/apysc/_translation/jp/array_slice.py
+-rw-r--r--   0 runner    (1001) docker     (127)     4882 2024-05-29 12:24:48.000000 apysc-4.4.3/apysc/_translation/jp/array_sort.py
+-rw-r--r--   0 runner    (1001) docker     (127)    16401 2024-05-29 12:24:48.000000 apysc-4.4.3/apysc/_translation/jp/assert_arrays_equal_and_arrays_not_equal.py
+-rw-r--r--   0 runner    (1001) docker     (127)    11293 2024-05-29 12:24:48.000000 apysc-4.4.3/apysc/_translation/jp/assert_defined_and_undefined.py
+-rw-r--r--   0 runner    (1001) docker     (127)    16989 2024-05-29 12:24:48.000000 apysc-4.4.3/apysc/_translation/jp/assert_dicts_equal_and_dicts_not_equal.py
+-rw-r--r--   0 runner    (1001) docker     (127)    11725 2024-05-29 12:24:48.000000 apysc-4.4.3/apysc/_translation/jp/assert_equal_and_not_equal.py
+-rw-r--r--   0 runner    (1001) docker     (127)    11091 2024-05-29 12:24:48.000000 apysc-4.4.3/apysc/_translation/jp/assert_greater_and_greater_equal.py
+-rw-r--r--   0 runner    (1001) docker     (127)    10904 2024-05-29 12:24:48.000000 apysc-4.4.3/apysc/_translation/jp/assert_less_and_less_equal.py
+-rw-r--r--   0 runner    (1001) docker     (127)    16034 2024-05-29 12:24:48.000000 apysc-4.4.3/apysc/_translation/jp/assert_true_and_false.py
+-rw-r--r--   0 runner    (1001) docker     (127)     6554 2024-05-29 12:24:48.000000 apysc-4.4.3/apysc/_translation/jp/assertion_basic_behavior.py
+-rw-r--r--   0 runner    (1001) docker     (127)    25796 2024-05-29 12:24:48.000000 apysc-4.4.3/apysc/_translation/jp/bind_and_trigger_custom_event.py
+-rw-r--r--   0 runner    (1001) docker     (127)     5543 2024-05-29 12:24:48.000000 apysc-4.4.3/apysc/_translation/jp/blue_color.py
+-rw-r--r--   0 runner    (1001) docker     (127)    15021 2024-05-29 12:24:48.000000 apysc-4.4.3/apysc/_translation/jp/boolean.py
+-rw-r--r--   0 runner    (1001) docker     (127)     4715 2024-05-29 12:24:48.000000 apysc-4.4.3/apysc/_translation/jp/branch_instruction_variables_reverting_setting.py
+-rw-r--r--   0 runner    (1001) docker     (127)    50491 2024-05-29 12:24:48.000000 apysc-4.4.3/apysc/_translation/jp/circle.py
+-rw-r--r--   0 runner    (1001) docker     (127)    19083 2024-05-29 12:24:48.000000 apysc-4.4.3/apysc/_translation/jp/click.py
+-rw-r--r--   0 runner    (1001) docker     (127)     8517 2024-05-29 12:24:48.000000 apysc-4.4.3/apysc/_translation/jp/color.py
+-rw-r--r--   0 runner    (1001) docker     (127)     7228 2024-05-29 12:24:48.000000 apysc-4.4.3/apysc/_translation/jp/color_from_rgb.py
+-rw-r--r--   0 runner    (1001) docker     (127)     2891 2024-05-29 12:24:48.000000 apysc-4.4.3/apysc/_translation/jp/colorless.py
+-rw-r--r--   0 runner    (1001) docker     (127)     6468 2024-05-29 12:24:48.000000 apysc-4.4.3/apysc/_translation/jp/colors.py
+-rw-r--r--   0 runner    (1001) docker     (127)     7940 2024-05-29 12:24:48.000000 apysc-4.4.3/apysc/_translation/jp/contains.py
+-rw-r--r--   0 runner    (1001) docker     (127)     6579 2024-05-29 12:24:48.000000 apysc-4.4.3/apysc/_translation/jp/continue.py
+-rw-r--r--   0 runner    (1001) docker     (127)    14038 2024-05-29 12:24:48.000000 apysc-4.4.3/apysc/_translation/jp/datetime.py
+-rw-r--r--   0 runner    (1001) docker     (127)     4592 2024-05-29 12:24:48.000000 apysc-4.4.3/apysc/_translation/jp/datetime_day.py
+-rw-r--r--   0 runner    (1001) docker     (127)     4705 2024-05-29 12:24:48.000000 apysc-4.4.3/apysc/_translation/jp/datetime_hour.py
+-rw-r--r--   0 runner    (1001) docker     (127)     4883 2024-05-29 12:24:48.000000 apysc-4.4.3/apysc/_translation/jp/datetime_millisecond.py
+-rw-r--r--   0 runner    (1001) docker     (127)     4779 2024-05-29 12:24:48.000000 apysc-4.4.3/apysc/_translation/jp/datetime_minute.py
+-rw-r--r--   0 runner    (1001) docker     (127)     4636 2024-05-29 12:24:48.000000 apysc-4.4.3/apysc/_translation/jp/datetime_month.py
+-rw-r--r--   0 runner    (1001) docker     (127)     6808 2024-05-29 12:24:48.000000 apysc-4.4.3/apysc/_translation/jp/datetime_now.py
+-rw-r--r--   0 runner    (1001) docker     (127)     4776 2024-05-29 12:24:48.000000 apysc-4.4.3/apysc/_translation/jp/datetime_second.py
+-rw-r--r--   0 runner    (1001) docker     (127)     2008 2024-05-29 12:24:48.000000 apysc-4.4.3/apysc/_translation/jp/datetime_set_month_end.py
+-rw-r--r--   0 runner    (1001) docker     (127)     9075 2024-05-29 12:24:48.000000 apysc-4.4.3/apysc/_translation/jp/datetime_weekday_js_and_weekday_py.py
+-rw-r--r--   0 runner    (1001) docker     (127)     4677 2024-05-29 12:24:48.000000 apysc-4.4.3/apysc/_translation/jp/datetime_year.py
+-rw-r--r--   0 runner    (1001) docker     (127)    16704 2024-05-29 12:24:48.000000 apysc-4.4.3/apysc/_translation/jp/dblclick.py
+-rw-r--r--   0 runner    (1001) docker     (127)     4735 2024-05-29 12:24:48.000000 apysc-4.4.3/apysc/_translation/jp/delete.py
+-rw-r--r--   0 runner    (1001) docker     (127)    12341 2024-05-29 12:24:48.000000 apysc-4.4.3/apysc/_translation/jp/dictionary.py
+-rw-r--r--   0 runner    (1001) docker     (127)     5460 2024-05-29 12:24:48.000000 apysc-4.4.3/apysc/_translation/jp/dictionary_generic.py
+-rw-r--r--   0 runner    (1001) docker     (127)     5787 2024-05-29 12:24:48.000000 apysc-4.4.3/apysc/_translation/jp/dictionary_get.py
+-rw-r--r--   0 runner    (1001) docker     (127)     4594 2024-05-29 12:24:48.000000 apysc-4.4.3/apysc/_translation/jp/dictionary_length.py
+-rw-r--r--   0 runner    (1001) docker     (127)     4304 2024-05-29 12:24:48.000000 apysc-4.4.3/apysc/_translation/jp/display_object.py
+-rw-r--r--   0 runner    (1001) docker     (127)    23638 2024-05-29 12:24:48.000000 apysc-4.4.3/apysc/_translation/jp/display_object_and_graphics_base_prop_abstract.py
+-rw-r--r--   0 runner    (1001) docker     (127)     9845 2024-05-29 12:24:48.000000 apysc-4.4.3/apysc/_translation/jp/display_object_get_and_set_css.py
+-rw-r--r--   0 runner    (1001) docker     (127)     5401 2024-05-29 12:24:48.000000 apysc-4.4.3/apysc/_translation/jp/display_object_mouse_event.py
+-rw-r--r--   0 runner    (1001) docker     (127)     9053 2024-05-29 12:24:48.000000 apysc-4.4.3/apysc/_translation/jp/display_object_parent.py
+-rw-r--r--   0 runner    (1001) docker     (127)     8567 2024-05-29 12:24:48.000000 apysc-4.4.3/apysc/_translation/jp/display_object_visible.py
+-rw-r--r--   0 runner    (1001) docker     (127)     9188 2024-05-29 12:24:48.000000 apysc-4.4.3/apysc/_translation/jp/display_object_x_and_y.py
+-rw-r--r--   0 runner    (1001) docker     (127)     5691 2024-05-29 12:24:48.000000 apysc-4.4.3/apysc/_translation/jp/display_on_colaboratory.py
+-rw-r--r--   0 runner    (1001) docker     (127)     7937 2024-05-29 12:24:48.000000 apysc-4.4.3/apysc/_translation/jp/display_on_jupyter.py
+-rw-r--r--   0 runner    (1001) docker     (127)    12092 2024-05-29 12:24:48.000000 apysc-4.4.3/apysc/_translation/jp/draw_interfaces_abstract.py
+-rw-r--r--   0 runner    (1001) docker     (127)    85549 2024-05-29 12:24:48.000000 apysc-4.4.3/apysc/_translation/jp/easing_enum.py
+-rw-r--r--   0 runner    (1001) docker     (127)    12136 2024-05-29 12:24:48.000000 apysc-4.4.3/apysc/_translation/jp/elif.py
+-rw-r--r--   0 runner    (1001) docker     (127)    51515 2024-05-29 12:24:48.000000 apysc-4.4.3/apysc/_translation/jp/ellipse.py
+-rw-r--r--   0 runner    (1001) docker     (127)     9150 2024-05-29 12:24:48.000000 apysc-4.4.3/apysc/_translation/jp/else.py
+-rw-r--r--   0 runner    (1001) docker     (127)     9718 2024-05-29 12:24:48.000000 apysc-4.4.3/apysc/_translation/jp/enter_frame.py
+-rw-r--r--   0 runner    (1001) docker     (127)    12970 2024-05-29 12:24:48.000000 apysc-4.4.3/apysc/_translation/jp/event_prevent_default_and_stop_propagation.py
+-rw-r--r--   0 runner    (1001) docker     (127)    10715 2024-05-29 12:24:48.000000 apysc-4.4.3/apysc/_translation/jp/for_array_indices.py
+-rw-r--r--   0 runner    (1001) docker     (127)     9997 2024-05-29 12:24:48.000000 apysc-4.4.3/apysc/_translation/jp/for_array_indices_and_values.py
+-rw-r--r--   0 runner    (1001) docker     (127)     9557 2024-05-29 12:24:48.000000 apysc-4.4.3/apysc/_translation/jp/for_array_values.py
+-rw-r--r--   0 runner    (1001) docker     (127)     9783 2024-05-29 12:24:48.000000 apysc-4.4.3/apysc/_translation/jp/for_dict_keys.py
+-rw-r--r--   0 runner    (1001) docker     (127)    11463 2024-05-29 12:24:48.000000 apysc-4.4.3/apysc/_translation/jp/for_dict_keys_and_values.py
+-rw-r--r--   0 runner    (1001) docker     (127)     8642 2024-05-29 12:24:48.000000 apysc-4.4.3/apysc/_translation/jp/for_dict_values.py
+-rw-r--r--   0 runner    (1001) docker     (127)     5183 2024-05-29 12:24:48.000000 apysc-4.4.3/apysc/_translation/jp/fps.py
+-rw-r--r--   0 runner    (1001) docker     (127)     3950 2024-05-29 12:24:48.000000 apysc-4.4.3/apysc/_translation/jp/fundamental_data_classes_value_interface.py
+-rw-r--r--   0 runner    (1001) docker     (127)     6667 2024-05-29 12:24:48.000000 apysc-4.4.3/apysc/_translation/jp/get_bounds.py
+-rw-r--r--   0 runner    (1001) docker     (127)     6338 2024-05-29 12:24:48.000000 apysc-4.4.3/apysc/_translation/jp/get_child_at.py
+-rw-r--r--   0 runner    (1001) docker     (127)    11113 2024-05-29 12:24:48.000000 apysc-4.4.3/apysc/_translation/jp/graphics.py
+-rw-r--r--   0 runner    (1001) docker     (127)     5532 2024-05-29 12:24:48.000000 apysc-4.4.3/apysc/_translation/jp/graphics_base_fill_alpha.py
+-rw-r--r--   0 runner    (1001) docker     (127)     6524 2024-05-29 12:24:48.000000 apysc-4.4.3/apysc/_translation/jp/graphics_base_fill_color.py
+-rw-r--r--   0 runner    (1001) docker     (127)    10271 2024-05-29 12:24:48.000000 apysc-4.4.3/apysc/_translation/jp/graphics_base_flip_interfaces.py
+-rw-r--r--   0 runner    (1001) docker     (127)     5622 2024-05-29 12:24:48.000000 apysc-4.4.3/apysc/_translation/jp/graphics_base_line_alpha.py
+-rw-r--r--   0 runner    (1001) docker     (127)     6715 2024-05-29 12:24:48.000000 apysc-4.4.3/apysc/_translation/jp/graphics_base_line_color.py
+-rw-r--r--   0 runner    (1001) docker     (127)     9355 2024-05-29 12:24:48.000000 apysc-4.4.3/apysc/_translation/jp/graphics_base_line_dash_dot_setting.py
+-rw-r--r--   0 runner    (1001) docker     (127)     8863 2024-05-29 12:24:48.000000 apysc-4.4.3/apysc/_translation/jp/graphics_base_line_dash_setting.py
+-rw-r--r--   0 runner    (1001) docker     (127)     9053 2024-05-29 12:24:48.000000 apysc-4.4.3/apysc/_translation/jp/graphics_base_line_dot_setting.py
+-rw-r--r--   0 runner    (1001) docker     (127)     9250 2024-05-29 12:24:48.000000 apysc-4.4.3/apysc/_translation/jp/graphics_base_line_round_dot_setting.py
+-rw-r--r--   0 runner    (1001) docker     (127)     5281 2024-05-29 12:24:48.000000 apysc-4.4.3/apysc/_translation/jp/graphics_base_line_thickness.py
+-rw-r--r--   0 runner    (1001) docker     (127)     6753 2024-05-29 12:24:48.000000 apysc-4.4.3/apysc/_translation/jp/graphics_base_rotation_around_center.py
+-rw-r--r--   0 runner    (1001) docker     (127)    11688 2024-05-29 12:24:48.000000 apysc-4.4.3/apysc/_translation/jp/graphics_base_rotation_around_point.py
+-rw-r--r--   0 runner    (1001) docker     (127)    16144 2024-05-29 12:24:48.000000 apysc-4.4.3/apysc/_translation/jp/graphics_base_scale_from_center.py
+-rw-r--r--   0 runner    (1001) docker     (127)    24463 2024-05-29 12:24:48.000000 apysc-4.4.3/apysc/_translation/jp/graphics_base_scale_from_point.py
+-rw-r--r--   0 runner    (1001) docker     (127)    10099 2024-05-29 12:24:48.000000 apysc-4.4.3/apysc/_translation/jp/graphics_base_skew.py
+-rw-r--r--   0 runner    (1001) docker     (127)    19456 2024-05-29 12:24:48.000000 apysc-4.4.3/apysc/_translation/jp/graphics_begin_fill.py
+-rw-r--r--   0 runner    (1001) docker     (127)     3461 2024-05-29 12:24:48.000000 apysc-4.4.3/apysc/_translation/jp/graphics_clear.py
+-rw-r--r--   0 runner    (1001) docker     (127)     8915 2024-05-29 12:24:48.000000 apysc-4.4.3/apysc/_translation/jp/graphics_draw_circle.py
+-rw-r--r--   0 runner    (1001) docker     (127)     9154 2024-05-29 12:24:48.000000 apysc-4.4.3/apysc/_translation/jp/graphics_draw_dash_dotted_line.py
+-rw-r--r--   0 runner    (1001) docker     (127)     8546 2024-05-29 12:24:48.000000 apysc-4.4.3/apysc/_translation/jp/graphics_draw_dashed_line.py
+-rw-r--r--   0 runner    (1001) docker     (127)     8098 2024-05-29 12:24:48.000000 apysc-4.4.3/apysc/_translation/jp/graphics_draw_dotted_line.py
+-rw-r--r--   0 runner    (1001) docker     (127)    10266 2024-05-29 12:24:48.000000 apysc-4.4.3/apysc/_translation/jp/graphics_draw_ellipse.py
+-rw-r--r--   0 runner    (1001) docker     (127)    11252 2024-05-29 12:24:48.000000 apysc-4.4.3/apysc/_translation/jp/graphics_draw_line.py
+-rw-r--r--   0 runner    (1001) docker     (127)    10592 2024-05-29 12:24:48.000000 apysc-4.4.3/apysc/_translation/jp/graphics_draw_path.py
+-rw-r--r--   0 runner    (1001) docker     (127)    15102 2024-05-29 12:24:48.000000 apysc-4.4.3/apysc/_translation/jp/graphics_draw_polygon.py
+-rw-r--r--   0 runner    (1001) docker     (127)    10632 2024-05-29 12:24:48.000000 apysc-4.4.3/apysc/_translation/jp/graphics_draw_rect.py
+-rw-r--r--   0 runner    (1001) docker     (127)    11078 2024-05-29 12:24:48.000000 apysc-4.4.3/apysc/_translation/jp/graphics_draw_round_dotted_line.py
+-rw-r--r--   0 runner    (1001) docker     (127)    10286 2024-05-29 12:24:48.000000 apysc-4.4.3/apysc/_translation/jp/graphics_draw_round_rect.py
+-rw-r--r--   0 runner    (1001) docker     (127)    10974 2024-05-29 12:24:48.000000 apysc-4.4.3/apysc/_translation/jp/graphics_draw_triangle.py
+-rw-r--r--   0 runner    (1001) docker     (127)    64374 2024-05-29 12:24:48.000000 apysc-4.4.3/apysc/_translation/jp/graphics_line_style.py
+-rw-r--r--   0 runner    (1001) docker     (127)    18270 2024-05-29 12:24:48.000000 apysc-4.4.3/apysc/_translation/jp/graphics_move_to_and_line_to.py
+-rw-r--r--   0 runner    (1001) docker     (127)     5571 2024-05-29 12:24:48.000000 apysc-4.4.3/apysc/_translation/jp/green_color.py
+-rw-r--r--   0 runner    (1001) docker     (127)     7571 2024-05-29 12:24:48.000000 apysc-4.4.3/apysc/_translation/jp/if.py
+-rw-r--r--   0 runner    (1001) docker     (127)     2013 2024-05-29 12:24:48.000000 apysc-4.4.3/apysc/_translation/jp/import_conventions.py
+-rw-r--r--   0 runner    (1001) docker     (127)    21073 2024-05-29 12:24:48.000000 apysc-4.4.3/apysc/_translation/jp/index.py
+-rw-r--r--   0 runner    (1001) docker     (127)    18347 2024-05-29 12:24:48.000000 apysc-4.4.3/apysc/_translation/jp/int_and_number.py
+-rw-r--r--   0 runner    (1001) docker     (127)    11684 2024-05-29 12:24:48.000000 apysc-4.4.3/apysc/_translation/jp/int_and_number_arithmetic_operations.py
+-rw-r--r--   0 runner    (1001) docker     (127)     8328 2024-05-29 12:24:48.000000 apysc-4.4.3/apysc/_translation/jp/int_and_number_comparison_operations.py
+-rw-r--r--   0 runner    (1001) docker     (127)     7200 2024-05-29 12:24:48.000000 apysc-4.4.3/apysc/_translation/jp/int_and_number_to_fixed.py
+-rw-r--r--   0 runner    (1001) docker     (127)     5897 2024-05-29 12:24:48.000000 apysc-4.4.3/apysc/_translation/jp/int_and_number_to_hex.py
+-rw-r--r--   0 runner    (1001) docker     (127)    48186 2024-05-29 12:24:48.000000 apysc-4.4.3/apysc/_translation/jp/line.py
+-rw-r--r--   0 runner    (1001) docker     (127)     7040 2024-05-29 12:24:48.000000 apysc-4.4.3/apysc/_translation/jp/material_design_colors.py
+-rw-r--r--   0 runner    (1001) docker     (127)     9561 2024-05-29 12:24:48.000000 apysc-4.4.3/apysc/_translation/jp/material_icon.py
+-rw-r--r--   0 runner    (1001) docker     (127)     7014 2024-05-29 12:24:48.000000 apysc-4.4.3/apysc/_translation/jp/math_clamp.py
+-rw-r--r--   0 runner    (1001) docker     (127)     4775 2024-05-29 12:24:48.000000 apysc-4.4.3/apysc/_translation/jp/math_max.py
+-rw-r--r--   0 runner    (1001) docker     (127)     4765 2024-05-29 12:24:48.000000 apysc-4.4.3/apysc/_translation/jp/math_min.py
+-rw-r--r--   0 runner    (1001) docker     (127)     6272 2024-05-29 12:24:48.000000 apysc-4.4.3/apysc/_translation/jp/math_trunc.py
+-rw-r--r--   0 runner    (1001) docker     (127)     5815 2024-05-29 12:24:48.000000 apysc-4.4.3/apysc/_translation/jp/mouse_event_abstract.py
+-rw-r--r--   0 runner    (1001) docker     (127)    38153 2024-05-29 12:24:48.000000 apysc-4.4.3/apysc/_translation/jp/mouse_event_basic.py
+-rw-r--r--   0 runner    (1001) docker     (127)    27701 2024-05-29 12:24:48.000000 apysc-4.4.3/apysc/_translation/jp/mousedown_and_mouseup.py
+-rw-r--r--   0 runner    (1001) docker     (127)    17541 2024-05-29 12:24:48.000000 apysc-4.4.3/apysc/_translation/jp/mousemove.py
+-rw-r--r--   0 runner    (1001) docker     (127)    28272 2024-05-29 12:24:48.000000 apysc-4.4.3/apysc/_translation/jp/mouseover_and_mouseout.py
+-rw-r--r--   0 runner    (1001) docker     (127)    12910 2024-05-29 12:24:48.000000 apysc-4.4.3/apysc/_translation/jp/multi_line_text.py
+-rw-r--r--   0 runner    (1001) docker     (127)     7536 2024-05-29 12:24:48.000000 apysc-4.4.3/apysc/_translation/jp/num_children.py
+-rw-r--r--   0 runner    (1001) docker     (127)    62153 2024-05-29 12:24:48.000000 apysc-4.4.3/apysc/_translation/jp/path.py
+-rw-r--r--   0 runner    (1001) docker     (127)    13516 2024-05-29 12:24:48.000000 apysc-4.4.3/apysc/_translation/jp/path_bezier_2d.py
+-rw-r--r--   0 runner    (1001) docker     (127)    11122 2024-05-29 12:24:48.000000 apysc-4.4.3/apysc/_translation/jp/path_bezier_2d_continual.py
+-rw-r--r--   0 runner    (1001) docker     (127)    16364 2024-05-29 12:24:48.000000 apysc-4.4.3/apysc/_translation/jp/path_bezier_3d.py
+-rw-r--r--   0 runner    (1001) docker     (127)    16314 2024-05-29 12:24:48.000000 apysc-4.4.3/apysc/_translation/jp/path_bezier_3d_continual.py
+-rw-r--r--   0 runner    (1001) docker     (127)     6991 2024-05-29 12:24:48.000000 apysc-4.4.3/apysc/_translation/jp/path_close.py
+-rw-r--r--   0 runner    (1001) docker     (127)     9572 2024-05-29 12:24:48.000000 apysc-4.4.3/apysc/_translation/jp/path_horizontal.py
+-rw-r--r--   0 runner    (1001) docker     (127)     9504 2024-05-29 12:24:48.000000 apysc-4.4.3/apysc/_translation/jp/path_line_to.py
+-rw-r--r--   0 runner    (1001) docker     (127)     9884 2024-05-29 12:24:48.000000 apysc-4.4.3/apysc/_translation/jp/path_move_to.py
+-rw-r--r--   0 runner    (1001) docker     (127)     9522 2024-05-29 12:24:48.000000 apysc-4.4.3/apysc/_translation/jp/path_vertical.py
+-rw-r--r--   0 runner    (1001) docker     (127)    12222 2024-05-29 12:24:48.000000 apysc-4.4.3/apysc/_translation/jp/point2d.py
+-rw-r--r--   0 runner    (1001) docker     (127)    50966 2024-05-29 12:24:48.000000 apysc-4.4.3/apysc/_translation/jp/polygon.py
+-rw-r--r--   0 runner    (1001) docker     (127)    53243 2024-05-29 12:24:48.000000 apysc-4.4.3/apysc/_translation/jp/polyline.py
+-rw-r--r--   0 runner    (1001) docker     (127)     6717 2024-05-29 12:24:48.000000 apysc-4.4.3/apysc/_translation/jp/quick_start.py
+-rw-r--r--   0 runner    (1001) docker     (127)     6242 2024-05-29 12:24:48.000000 apysc-4.4.3/apysc/_translation/jp/range.py
+-rw-r--r--   0 runner    (1001) docker     (127)     2842 2024-05-29 12:24:48.000000 apysc-4.4.3/apysc/_translation/jp/recommended_type_checker_settings.py
+-rw-r--r--   0 runner    (1001) docker     (127)    54921 2024-05-29 12:24:48.000000 apysc-4.4.3/apysc/_translation/jp/rectangle.py
+-rw-r--r--   0 runner    (1001) docker     (127)    25542 2024-05-29 12:24:48.000000 apysc-4.4.3/apysc/_translation/jp/rectangle_geom.py
+-rw-r--r--   0 runner    (1001) docker     (127)     5008 2024-05-29 12:24:48.000000 apysc-4.4.3/apysc/_translation/jp/red_color.py
+-rw-r--r--   0 runner    (1001) docker     (127)     5482 2024-05-29 12:24:48.000000 apysc-4.4.3/apysc/_translation/jp/remove_children.py
+-rw-r--r--   0 runner    (1001) docker     (127)     7088 2024-05-29 12:24:48.000000 apysc-4.4.3/apysc/_translation/jp/return.py
+-rw-r--r--   0 runner    (1001) docker     (127)    17504 2024-05-29 12:24:48.000000 apysc-4.4.3/apysc/_translation/jp/save_overall_html.py
+-rw-r--r--   0 runner    (1001) docker     (127)     4685 2024-05-29 12:24:48.000000 apysc-4.4.3/apysc/_translation/jp/sequential_animation.py
+-rw-r--r--   0 runner    (1001) docker     (127)    10214 2024-05-29 12:24:48.000000 apysc-4.4.3/apysc/_translation/jp/set_debug_mode.py
+-rw-r--r--   0 runner    (1001) docker     (127)    12228 2024-05-29 12:24:48.000000 apysc-4.4.3/apysc/_translation/jp/sprite.py
+-rw-r--r--   0 runner    (1001) docker     (127)    31274 2024-05-29 12:24:48.000000 apysc-4.4.3/apysc/_translation/jp/stage.py
+-rw-r--r--   0 runner    (1001) docker     (127)     9480 2024-05-29 12:24:48.000000 apysc-4.4.3/apysc/_translation/jp/string.py
+-rw-r--r--   0 runner    (1001) docker     (127)     5468 2024-05-29 12:24:48.000000 apysc-4.4.3/apysc/_translation/jp/string_addition_and_multiplication.py
+-rw-r--r--   0 runner    (1001) docker     (127)     6953 2024-05-29 12:24:48.000000 apysc-4.4.3/apysc/_translation/jp/string_apply_max_num_of_decimal_places.py
+-rw-r--r--   0 runner    (1001) docker     (127)     6761 2024-05-29 12:24:48.000000 apysc-4.4.3/apysc/_translation/jp/string_comparison_operations.py
+-rw-r--r--   0 runner    (1001) docker     (127)     6800 2024-05-29 12:24:48.000000 apysc-4.4.3/apysc/_translation/jp/string_length.py
+-rw-r--r--   0 runner    (1001) docker     (127)     3841 2024-05-29 12:24:48.000000 apysc-4.4.3/apysc/_translation/jp/string_lower.py
+-rw-r--r--   0 runner    (1001) docker     (127)     7143 2024-05-29 12:24:48.000000 apysc-4.4.3/apysc/_translation/jp/string_lstrip.py
+-rw-r--r--   0 runner    (1001) docker     (127)     7074 2024-05-29 12:24:48.000000 apysc-4.4.3/apysc/_translation/jp/string_rstrip.py
+-rw-r--r--   0 runner    (1001) docker     (127)     8198 2024-05-29 12:24:48.000000 apysc-4.4.3/apysc/_translation/jp/string_slice.py
+-rw-r--r--   0 runner    (1001) docker     (127)     4910 2024-05-29 12:24:48.000000 apysc-4.4.3/apysc/_translation/jp/string_split.py
+-rw-r--r--   0 runner    (1001) docker     (127)     7150 2024-05-29 12:24:48.000000 apysc-4.4.3/apysc/_translation/jp/string_strip.py
+-rw-r--r--   0 runner    (1001) docker     (127)     3847 2024-05-29 12:24:48.000000 apysc-4.4.3/apysc/_translation/jp/string_upper.py
+-rw-r--r--   0 runner    (1001) docker     (127)     5282 2024-05-29 12:24:48.000000 apysc-4.4.3/apysc/_translation/jp/string_zfill.py
+-rw-r--r--   0 runner    (1001) docker     (127)    49436 2024-05-29 12:24:48.000000 apysc-4.4.3/apysc/_translation/jp/svg_text.py
+-rw-r--r--   0 runner    (1001) docker     (127)    45588 2024-05-29 12:24:48.000000 apysc-4.4.3/apysc/_translation/jp/svg_text_span.py
+-rw-r--r--   0 runner    (1001) docker     (127)    11135 2024-05-29 12:24:48.000000 apysc-4.4.3/apysc/_translation/jp/text_align.py
+-rw-r--r--   0 runner    (1001) docker     (127)    14274 2024-05-29 12:24:48.000000 apysc-4.4.3/apysc/_translation/jp/text_align_last.py
+-rw-r--r--   0 runner    (1001) docker     (127)     5702 2024-05-29 12:24:48.000000 apysc-4.4.3/apysc/_translation/jp/text_bold.py
+-rw-r--r--   0 runner    (1001) docker     (127)     5673 2024-05-29 12:24:48.000000 apysc-4.4.3/apysc/_translation/jp/text_fill_alpha.py
+-rw-r--r--   0 runner    (1001) docker     (127)     6046 2024-05-29 12:24:48.000000 apysc-4.4.3/apysc/_translation/jp/text_fill_color.py
+-rw-r--r--   0 runner    (1001) docker     (127)     5818 2024-05-29 12:24:48.000000 apysc-4.4.3/apysc/_translation/jp/text_font_size.py
+-rw-r--r--   0 runner    (1001) docker     (127)     5809 2024-05-29 12:24:48.000000 apysc-4.4.3/apysc/_translation/jp/text_italic.py
+-rw-r--r--   0 runner    (1001) docker     (127)     5708 2024-05-29 12:24:48.000000 apysc-4.4.3/apysc/_translation/jp/text_line_height.py
+-rw-r--r--   0 runner    (1001) docker     (127)     5755 2024-05-29 12:24:48.000000 apysc-4.4.3/apysc/_translation/jp/text_underline.py
+-rw-r--r--   0 runner    (1001) docker     (127)     8047 2024-05-29 12:24:48.000000 apysc-4.4.3/apysc/_translation/jp/timedelta.py
+-rw-r--r--   0 runner    (1001) docker     (127)     4820 2024-05-29 12:24:48.000000 apysc-4.4.3/apysc/_translation/jp/timedelta_days.py
+-rw-r--r--   0 runner    (1001) docker     (127)     5042 2024-05-29 12:24:48.000000 apysc-4.4.3/apysc/_translation/jp/timedelta_total_seconds.py
+-rw-r--r--   0 runner    (1001) docker     (127)    12931 2024-05-29 12:24:48.000000 apysc-4.4.3/apysc/_translation/jp/timer.py
+-rw-r--r--   0 runner    (1001) docker     (127)    12198 2024-05-29 12:24:48.000000 apysc-4.4.3/apysc/_translation/jp/timer_complete.py
+-rw-r--r--   0 runner    (1001) docker     (127)    17339 2024-05-29 12:24:48.000000 apysc-4.4.3/apysc/_translation/jp/timer_delay.py
+-rw-r--r--   0 runner    (1001) docker     (127)    13318 2024-05-29 12:24:48.000000 apysc-4.4.3/apysc/_translation/jp/timer_event.py
+-rw-r--r--   0 runner    (1001) docker     (127)    13574 2024-05-29 12:24:48.000000 apysc-4.4.3/apysc/_translation/jp/timer_repeat_count.py
+-rw-r--r--   0 runner    (1001) docker     (127)     9013 2024-05-29 12:24:48.000000 apysc-4.4.3/apysc/_translation/jp/timer_reset.py
+-rw-r--r--   0 runner    (1001) docker     (127)     9087 2024-05-29 12:24:48.000000 apysc-4.4.3/apysc/_translation/jp/timer_start_and_stop.py
+-rw-r--r--   0 runner    (1001) docker     (127)     6814 2024-05-29 12:24:48.000000 apysc-4.4.3/apysc/_translation/jp/to_string.py
+-rw-r--r--   0 runner    (1001) docker     (127)     6728 2024-05-29 12:24:48.000000 apysc-4.4.3/apysc/_translation/jp/trace.py
+-rw-r--r--   0 runner    (1001) docker     (127)    66343 2024-05-29 12:24:48.000000 apysc-4.4.3/apysc/_translation/jp/triangle.py
+-rw-r--r--   0 runner    (1001) docker     (127)     2751 2024-05-29 12:24:48.000000 apysc-4.4.3/apysc/_translation/jp/true_and_false.py
+-rw-r--r--   0 runner    (1001) docker     (127)    14525 2024-05-29 12:24:48.000000 apysc-4.4.3/apysc/_translation/jp/unbind_enter_frame_and_unbind_enter_frame_all.py
+-rw-r--r--   0 runner    (1001) docker     (127)    10005 2024-05-29 12:24:48.000000 apysc-4.4.3/apysc/_translation/jp/unset_debug_mode.py
+-rw-r--r--   0 runner    (1001) docker     (127)     6307 2024-05-29 12:24:48.000000 apysc-4.4.3/apysc/_translation/jp/variable_name_suffix.py
+-rw-r--r--   0 runner    (1001) docker     (127)    19570 2024-05-29 12:24:48.000000 apysc-4.4.3/apysc/_translation/jp/what_apysc_can_do.py
+-rw-r--r--   0 runner    (1001) docker     (127)     3509 2024-05-29 12:24:48.000000 apysc-4.4.3/apysc/_translation/jp/why_apysc_doesnt_use_python_builtin_data_type.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-29 12:25:10.191791 apysc-4.4.3/apysc/_type/
+-rw-r--r--   0 runner    (1001) docker     (127)        0 2024-05-29 12:24:48.000000 apysc-4.4.3/apysc/_type/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (127)     1491 2024-05-29 12:24:48.000000 apysc-4.4.3/apysc/_type/_delete.py
+-rw-r--r--   0 runner    (1001) docker     (127)     1947 2024-05-29 12:24:48.000000 apysc-4.4.3/apysc/_type/_return.py
+-rw-r--r--   0 runner    (1001) docker     (127)    17556 2024-05-29 12:24:48.000000 apysc-4.4.3/apysc/_type/any_value.py
+-rw-r--r--   0 runner    (1001) docker     (127)    50943 2024-05-29 12:24:48.000000 apysc-4.4.3/apysc/_type/array.py
+-rw-r--r--   0 runner    (1001) docker     (127)     4699 2024-05-29 12:24:48.000000 apysc-4.4.3/apysc/_type/attr_linking_mixin.py
+-rw-r--r--   0 runner    (1001) docker     (127)     5282 2024-05-29 12:24:48.000000 apysc-4.4.3/apysc/_type/attr_to_apysc_val_from_builtin_mixin.py
+-rw-r--r--   0 runner    (1001) docker     (127)     1817 2024-05-29 12:24:48.000000 apysc-4.4.3/apysc/_type/blank_object_mixin.py
+-rw-r--r--   0 runner    (1001) docker     (127)     3445 2024-05-29 12:24:48.000000 apysc-4.4.3/apysc/_type/bool_const_mixin.py
+-rw-r--r--   0 runner    (1001) docker     (127)    17955 2024-05-29 12:24:48.000000 apysc-4.4.3/apysc/_type/boolean.py
+-rw-r--r--   0 runner    (1001) docker     (127)      389 2024-05-29 12:24:48.000000 apysc-4.4.3/apysc/_type/copy_interface.py
+-rw-r--r--   0 runner    (1001) docker     (127)     3259 2024-05-29 12:24:48.000000 apysc-4.4.3/apysc/_type/copy_mixin.py
+-rw-r--r--   0 runner    (1001) docker     (127)     3330 2024-05-29 12:24:48.000000 apysc-4.4.3/apysc/_type/deleted_object_mixin.py
+-rw-r--r--   0 runner    (1001) docker     (127)    24160 2024-05-29 12:24:48.000000 apysc-4.4.3/apysc/_type/dictionary.py
+-rw-r--r--   0 runner    (1001) docker     (127)      391 2024-05-29 12:24:48.000000 apysc-4.4.3/apysc/_type/dictionary_structure.py
+-rw-r--r--   0 runner    (1001) docker     (127)     1707 2024-05-29 12:24:48.000000 apysc-4.4.3/apysc/_type/expression_string.py
+-rw-r--r--   0 runner    (1001) docker     (127)      803 2024-05-29 12:24:48.000000 apysc-4.4.3/apysc/_type/false.py
+-rw-r--r--   0 runner    (1001) docker     (127)      237 2024-05-29 12:24:48.000000 apysc-4.4.3/apysc/_type/hashable_interface.py
+-rw-r--r--   0 runner    (1001) docker     (127)     1360 2024-05-29 12:24:48.000000 apysc-4.4.3/apysc/_type/initial_substitution_exp_mixin.py
+-rw-r--r--   0 runner    (1001) docker     (127)      975 2024-05-29 12:24:48.000000 apysc-4.4.3/apysc/_type/initialize_locals_and_globals_mixin.py
+-rw-r--r--   0 runner    (1001) docker     (127)     7428 2024-05-29 12:24:48.000000 apysc-4.4.3/apysc/_type/int.py
+-rw-r--r--   0 runner    (1001) docker     (127)     6739 2024-05-29 12:24:48.000000 apysc-4.4.3/apysc/_type/number.py
+-rw-r--r--   0 runner    (1001) docker     (127)    35138 2024-05-29 12:24:48.000000 apysc-4.4.3/apysc/_type/number_value_mixin.py
+-rw-r--r--   0 runner    (1001) docker     (127)      569 2024-05-29 12:24:48.000000 apysc-4.4.3/apysc/_type/py_builtin_iter_disabling_mixin.py
+-rw-r--r--   0 runner    (1001) docker     (127)      324 2024-05-29 12:24:48.000000 apysc-4.4.3/apysc/_type/repr_interface.py
+-rw-r--r--   0 runner    (1001) docker     (127)      656 2024-05-29 12:24:48.000000 apysc-4.4.3/apysc/_type/revert_interface.py
+-rw-r--r--   0 runner    (1001) docker     (127)    10223 2024-05-29 12:24:48.000000 apysc-4.4.3/apysc/_type/revert_mixin.py
+-rw-r--r--   0 runner    (1001) docker     (127)    28760 2024-05-29 12:24:48.000000 apysc-4.4.3/apysc/_type/string.py
+-rw-r--r--   0 runner    (1001) docker     (127)     4666 2024-05-29 12:24:48.000000 apysc-4.4.3/apysc/_type/string_apply_max_num_of_decimal_places_mixin.py
+-rw-r--r--   0 runner    (1001) docker     (127)     1774 2024-05-29 12:24:48.000000 apysc-4.4.3/apysc/_type/string_length_mixin.py
+-rw-r--r--   0 runner    (1001) docker     (127)     1489 2024-05-29 12:24:48.000000 apysc-4.4.3/apysc/_type/string_lower_mixin.py
+-rw-r--r--   0 runner    (1001) docker     (127)     6682 2024-05-29 12:24:48.000000 apysc-4.4.3/apysc/_type/string_lstrip_mixin.py
+-rw-r--r--   0 runner    (1001) docker     (127)     6652 2024-05-29 12:24:48.000000 apysc-4.4.3/apysc/_type/string_rstrip_mixin.py
+-rw-r--r--   0 runner    (1001) docker     (127)     4204 2024-05-29 12:24:48.000000 apysc-4.4.3/apysc/_type/string_slice_mixin.py
+-rw-r--r--   0 runner    (1001) docker     (127)     2364 2024-05-29 12:24:48.000000 apysc-4.4.3/apysc/_type/string_split_mixin.py
+-rw-r--r--   0 runner    (1001) docker     (127)     6806 2024-05-29 12:24:48.000000 apysc-4.4.3/apysc/_type/string_strip_mixin.py
+-rw-r--r--   0 runner    (1001) docker     (127)     1497 2024-05-29 12:24:48.000000 apysc-4.4.3/apysc/_type/string_upper_mixin.py
+-rw-r--r--   0 runner    (1001) docker     (127)     2361 2024-05-29 12:24:48.000000 apysc-4.4.3/apysc/_type/string_zfill_mixin.py
+-rw-r--r--   0 runner    (1001) docker     (127)     3083 2024-05-29 12:24:48.000000 apysc-4.4.3/apysc/_type/to_fixed_mixin.py
+-rw-r--r--   0 runner    (1001) docker     (127)     2358 2024-05-29 12:24:48.000000 apysc-4.4.3/apysc/_type/to_hex_mixin.py
+-rw-r--r--   0 runner    (1001) docker     (127)     1737 2024-05-29 12:24:48.000000 apysc-4.4.3/apysc/_type/to_number_mixin.py
+-rw-r--r--   0 runner    (1001) docker     (127)     1637 2024-05-29 12:24:48.000000 apysc-4.4.3/apysc/_type/to_string_mixin.py
+-rw-r--r--   0 runner    (1001) docker     (127)      796 2024-05-29 12:24:48.000000 apysc-4.4.3/apysc/_type/true.py
+-rw-r--r--   0 runner    (1001) docker     (127)      370 2024-05-29 12:24:48.000000 apysc-4.4.3/apysc/_type/type_name_mixin.py
+-rw-r--r--   0 runner    (1001) docker     (127)     3940 2024-05-29 12:24:48.000000 apysc-4.4.3/apysc/_type/type_util.py
+-rw-r--r--   0 runner    (1001) docker     (127)     5295 2024-05-29 12:24:48.000000 apysc-4.4.3/apysc/_type/value_util.py
+-rw-r--r--   0 runner    (1001) docker     (127)     2244 2024-05-29 12:24:48.000000 apysc-4.4.3/apysc/_type/variable_name_mixin.py
+-rw-r--r--   0 runner    (1001) docker     (127)     1382 2024-05-29 12:24:48.000000 apysc-4.4.3/apysc/_type/variable_name_suffix_attr_or_var_mixin.py
+-rw-r--r--   0 runner    (1001) docker     (127)      747 2024-05-29 12:24:48.000000 apysc-4.4.3/apysc/_type/variable_name_suffix_mixin.py
+-rw-r--r--   0 runner    (1001) docker     (127)     1255 2024-05-29 12:24:48.000000 apysc-4.4.3/apysc/_type/variable_name_suffix_utils.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-29 12:25:10.195791 apysc-4.4.3/apysc/_validation/
+-rw-r--r--   0 runner    (1001) docker     (127)        0 2024-05-29 12:24:48.000000 apysc-4.4.3/apysc/_validation/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (127)   119148 2024-05-29 12:24:48.000000 apysc-4.4.3/apysc/_validation/arg_validation_decos.py
+-rw-r--r--   0 runner    (1001) docker     (127)     1847 2024-05-29 12:24:48.000000 apysc-4.4.3/apysc/_validation/bool_validation.py
+-rw-r--r--   0 runner    (1001) docker     (127)     2393 2024-05-29 12:24:48.000000 apysc-4.4.3/apysc/_validation/color_validation.py
+-rw-r--r--   0 runner    (1001) docker     (127)    10661 2024-05-29 12:24:48.000000 apysc-4.4.3/apysc/_validation/display_validation.py
+-rw-r--r--   0 runner    (1001) docker     (127)     1725 2024-05-29 12:24:48.000000 apysc-4.4.3/apysc/_validation/event_validation.py
+-rw-r--r--   0 runner    (1001) docker     (127)      949 2024-05-29 12:24:48.000000 apysc-4.4.3/apysc/_validation/geom_validation.py
+-rw-r--r--   0 runner    (1001) docker     (127)     2700 2024-05-29 12:24:48.000000 apysc-4.4.3/apysc/_validation/handler_validation.py
+-rw-r--r--   0 runner    (1001) docker     (127)     5682 2024-05-29 12:24:48.000000 apysc-4.4.3/apysc/_validation/matrix_data_validation.py
+-rw-r--r--   0 runner    (1001) docker     (127)     8629 2024-05-29 12:24:48.000000 apysc-4.4.3/apysc/_validation/number_validation.py
+-rw-r--r--   0 runner    (1001) docker     (127)     1081 2024-05-29 12:24:48.000000 apysc-4.4.3/apysc/_validation/parent_validation.py
+-rw-r--r--   0 runner    (1001) docker     (127)     4619 2024-05-29 12:24:48.000000 apysc-4.4.3/apysc/_validation/path_validation.py
+-rw-r--r--   0 runner    (1001) docker     (127)     3405 2024-05-29 12:24:48.000000 apysc-4.4.3/apysc/_validation/string_validation.py
+-rw-r--r--   0 runner    (1001) docker     (127)      595 2024-05-29 12:24:48.000000 apysc-4.4.3/apysc/_validation/validation_common_utils.py
+-rw-r--r--   0 runner    (1001) docker     (127)     1151 2024-05-29 12:24:48.000000 apysc-4.4.3/apysc/_validation/variable_name_validation.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-29 12:25:09.975790 apysc-4.4.3/apysc.egg-info/
+-rw-r--r--   0 runner    (1001) docker     (127)      828 2024-05-29 12:25:09.000000 apysc-4.4.3/apysc.egg-info/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (127)    99137 2024-05-29 12:25:09.000000 apysc-4.4.3/apysc.egg-info/SOURCES.txt
+-rw-r--r--   0 runner    (1001) docker     (127)        1 2024-05-29 12:25:09.000000 apysc-4.4.3/apysc.egg-info/dependency_links.txt
+-rw-r--r--   0 runner    (1001) docker     (127)       32 2024-05-29 12:25:09.000000 apysc-4.4.3/apysc.egg-info/requires.txt
+-rw-r--r--   0 runner    (1001) docker     (127)        6 2024-05-29 12:25:09.000000 apysc-4.4.3/apysc.egg-info/top_level.txt
+-rw-r--r--   0 runner    (1001) docker     (127)       38 2024-05-29 12:25:10.195791 apysc-4.4.3/setup.cfg
```

### Comparing `apysc-4.4.2/LICENSE` & `apysc-4.4.3/LICENSE`

 * *Files identical despite different names*

### Comparing `apysc-4.4.2/PKG-INFO` & `apysc-4.4.3/PKG-INFO`

 * *Files 12% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: apysc
-Version: 4.4.2
+Version: 4.4.3
 Summary: apysc is the Python's frontend library to create html and js file, that has the ActionScript 3 (as3)-like interface.
 Home-page: https://github.com/simon-ritchie/apysc
 Maintainer: simon-ritchie
 Maintainer-email: 
 License: MIT
 Platform: UNKNOWN
 Classifier: Programming Language :: Python :: 3
```

### Comparing `apysc-4.4.2/README.md` & `apysc-4.4.3/README.md`

 * *Files identical despite different names*

### Comparing `apysc-4.4.2/apysc/__init__.py` & `apysc-4.4.3/apysc/__init__.py`

 * *Files 1% similar despite different names*

```diff
@@ -1,11 +1,15 @@
 """isort:skip_file"""
 
 # flake8: noqa
 
+from apysc._console.loggers import get_info_logger as _get_info_logger
+_logger = _get_info_logger()
+_logger.info("apysc packages importing has been started.")
+
 from apysc._type.int import Int
 from apysc._type.number import Number
 from apysc._type.number import Number as Float
 from apysc._type.boolean import Boolean
 from apysc._type.boolean import Boolean as Bool
 from apysc._type.string import String
 from apysc._type.string import String as Str
@@ -46,14 +50,15 @@
 from apysc._display.svg_text import SvgText
 from apysc._display.svg_text_align_mixin import SvgTextAlign
 from apysc._display.svg_text_span import SvgTextSpan
 from apysc._display.multi_line_text import MultiLineText
 from apysc._display.css_text_align import CssTextAlign
 from apysc._display.css_text_align_last import CssTextAlignLast
 from apysc._display.svg_icon import SvgIcon
+from apysc._mask.mask import Mask
 from apysc._geom.point2d import Point2D
 from apysc._geom.path_label import PathLabel
 from apysc._geom.path_data_base import PathDataBase
 from apysc._geom.path_move_to import PathMoveTo
 from apysc._geom.path_line_to import PathLineTo
 from apysc._geom.path_horizontal import PathHorizontal
 from apysc._geom.path_vertical import PathVertical
@@ -88,14 +93,17 @@
 from apysc._console.assertion import assert_defined
 from apysc._console.assertion import assert_undefined
 from apysc._event.document_mouse_wheel_func import bind_wheel_event_to_document
 from apysc._event.document_mouse_wheel_func import unbind_wheel_event_all_from_document
 from apysc._event.document_mouse_wheel_func import unbind_wheel_event_from_document
 from apysc._html.exporter import save_overall_html
 from apysc._expression.expression_data_util import append_js_expression
+
+_logger.info("Roughly 100 packages have been imported...")
+
 from apysc._jupyter.jupyter_util import display_on_jupyter
 from apysc._jupyter.jupyter_util import display_on_colaboratory
 from apysc._time.fps import FPS
 from apysc._time.timer import Timer
 from apysc._time.datetime_ import DateTime
 from apysc._time.timedelta_ import TimeDelta
 from apysc._html.debug_mode import set_debug_mode
@@ -186,14 +194,17 @@
 from apysc._material_design.icon.material_add_alert_outlined_icon import MaterialAddAlertOutlinedIcon
 from apysc._material_design.icon.material_add_box_icon import MaterialAddBoxIcon
 from apysc._material_design.icon.material_add_box_outlined_icon import MaterialAddBoxOutlinedIcon
 from apysc._material_design.icon.material_add_circle_icon import MaterialAddCircleIcon
 from apysc._material_design.icon.material_add_circle_outlined_icon import MaterialAddCircleOutlinedIcon
 from apysc._material_design.icon.material_add_circle_outline_icon import MaterialAddCircleOutlineIcon
 from apysc._material_design.icon.material_add_circle_outline_outlined_icon import MaterialAddCircleOutlineOutlinedIcon
+
+_logger.info("Roughly 200 packages have been imported...")
+
 from apysc._material_design.icon.material_add_icon import MaterialAddIcon
 from apysc._material_design.icon.material_add_ic_call_icon import MaterialAddIcCallIcon
 from apysc._material_design.icon.material_add_ic_call_outlined_icon import MaterialAddIcCallOutlinedIcon
 from apysc._material_design.icon.material_add_link_icon import MaterialAddLinkIcon
 from apysc._material_design.icon.material_add_outlined_icon import MaterialAddOutlinedIcon
 from apysc._material_design.icon.material_add_shopping_cart_icon import MaterialAddShoppingCartIcon
 from apysc._material_design.icon.material_add_shopping_cart_outlined_icon import MaterialAddShoppingCartOutlinedIcon
@@ -283,14 +294,17 @@
 from apysc._material_design.icon.material_batch_prediction_icon import MaterialBatchPredictionIcon
 from apysc._material_design.icon.material_batch_prediction_outlined_icon import MaterialBatchPredictionOutlinedIcon
 from apysc._material_design.icon.material_biotech_icon import MaterialBiotechIcon
 from apysc._material_design.icon.material_biotech_outlined_icon import MaterialBiotechOutlinedIcon
 from apysc._material_design.icon.material_block_flipped_icon import MaterialBlockFlippedIcon
 from apysc._material_design.icon.material_block_icon import MaterialBlockIcon
 from apysc._material_design.icon.material_block_outlined_icon import MaterialBlockOutlinedIcon
+
+_logger.info("Roughly 300 packages have been imported...")
+
 from apysc._material_design.icon.material_bolt_icon import MaterialBoltIcon
 from apysc._material_design.icon.material_bookmarks_icon import MaterialBookmarksIcon
 from apysc._material_design.icon.material_bookmarks_outlined_icon import MaterialBookmarksOutlinedIcon
 from apysc._material_design.icon.material_bookmark_border_icon import MaterialBookmarkBorderIcon
 from apysc._material_design.icon.material_bookmark_border_outlined_icon import MaterialBookmarkBorderOutlinedIcon
 from apysc._material_design.icon.material_bookmark_icon import MaterialBookmarkIcon
 from apysc._material_design.icon.material_bookmark_outlined_icon import MaterialBookmarkOutlinedIcon
@@ -380,14 +394,17 @@
 from apysc._material_design.icon.material_comment_bank_icon import MaterialCommentBankIcon
 from apysc._material_design.icon.material_comment_bank_outlined_icon import MaterialCommentBankOutlinedIcon
 from apysc._material_design.icon.material_comment_icon import MaterialCommentIcon
 from apysc._material_design.icon.material_comment_outlined_icon import MaterialCommentOutlinedIcon
 from apysc._material_design.icon.material_commute_icon import MaterialCommuteIcon
 from apysc._material_design.icon.material_commute_outlined_icon import MaterialCommuteOutlinedIcon
 from apysc._material_design.icon.material_compare_arrows_icon import MaterialCompareArrowsIcon
+
+_logger.info("Roughly 400 packages have been imported...")
+
 from apysc._material_design.icon.material_compare_arrows_outlined_icon import MaterialCompareArrowsOutlinedIcon
 from apysc._material_design.icon.material_compress_icon import MaterialCompressIcon
 from apysc._material_design.icon.material_contactless_icon import MaterialContactlessIcon
 from apysc._material_design.icon.material_contactless_outlined_icon import MaterialContactlessOutlinedIcon
 from apysc._material_design.icon.material_contacts_icon import MaterialContactsIcon
 from apysc._material_design.icon.material_contacts_outlined_icon import MaterialContactsOutlinedIcon
 from apysc._material_design.icon.material_contact_mail_icon import MaterialContactMailIcon
@@ -477,14 +494,17 @@
 from apysc._material_design.icon.material_error_outline_outlined_icon import MaterialErrorOutlineOutlinedIcon
 from apysc._material_design.icon.material_euro_symbol_icon import MaterialEuroSymbolIcon
 from apysc._material_design.icon.material_euro_symbol_outlined_icon import MaterialEuroSymbolOutlinedIcon
 from apysc._material_design.icon.material_event_icon import MaterialEventIcon
 from apysc._material_design.icon.material_event_outlined_icon import MaterialEventOutlinedIcon
 from apysc._material_design.icon.material_event_seat_icon import MaterialEventSeatIcon
 from apysc._material_design.icon.material_event_seat_outlined_icon import MaterialEventSeatOutlinedIcon
+
+_logger.info("Roughly 500 packages have been imported...")
+
 from apysc._material_design.icon.material_exit_to_app_icon import MaterialExitToAppIcon
 from apysc._material_design.icon.material_exit_to_app_outlined_icon import MaterialExitToAppOutlinedIcon
 from apysc._material_design.icon.material_expand_icon import MaterialExpandIcon
 from apysc._material_design.icon.material_explicit_icon import MaterialExplicitIcon
 from apysc._material_design.icon.material_explicit_outlined_icon import MaterialExplicitOutlinedIcon
 from apysc._material_design.icon.material_explore_icon import MaterialExploreIcon
 from apysc._material_design.icon.material_explore_off_icon import MaterialExploreOffIcon
@@ -574,14 +594,17 @@
 from apysc._material_design.icon.material_gif_outlined_icon import MaterialGifOutlinedIcon
 from apysc._material_design.icon.material_grade_icon import MaterialGradeIcon
 from apysc._material_design.icon.material_grade_outlined_icon import MaterialGradeOutlinedIcon
 from apysc._material_design.icon.material_grading_icon import MaterialGradingIcon
 from apysc._material_design.icon.material_grading_outlined_icon import MaterialGradingOutlinedIcon
 from apysc._material_design.icon.material_group_work_icon import MaterialGroupWorkIcon
 from apysc._material_design.icon.material_group_work_outlined_icon import MaterialGroupWorkOutlinedIcon
+
+_logger.info("Roughly 600 packages have been imported...")
+
 from apysc._material_design.icon.material_g_translate_icon import MaterialGTranslateIcon
 from apysc._material_design.icon.material_g_translate_outlined_icon import MaterialGTranslateOutlinedIcon
 from apysc._material_design.icon.material_hd_icon import MaterialHdIcon
 from apysc._material_design.icon.material_hd_outlined_icon import MaterialHdOutlinedIcon
 from apysc._material_design.icon.material_hearing_disabled_icon import MaterialHearingDisabledIcon
 from apysc._material_design.icon.material_hearing_disabled_outlined_icon import MaterialHearingDisabledOutlinedIcon
 from apysc._material_design.icon.material_hearing_icon import MaterialHearingIcon
@@ -671,14 +694,17 @@
 from apysc._material_design.icon.material_library_music_outlined_icon import MaterialLibraryMusicOutlinedIcon
 from apysc._material_design.icon.material_lightbulb_icon import MaterialLightbulbIcon
 from apysc._material_design.icon.material_lightbulb_outlined_icon import MaterialLightbulbOutlinedIcon
 from apysc._material_design.icon.material_lightbulb_outline_icon import MaterialLightbulbOutlineIcon
 from apysc._material_design.icon.material_line_style_icon import MaterialLineStyleIcon
 from apysc._material_design.icon.material_line_style_outlined_icon import MaterialLineStyleOutlinedIcon
 from apysc._material_design.icon.material_line_weight_icon import MaterialLineWeightIcon
+
+_logger.info("Roughly 700 packages have been imported...")
+
 from apysc._material_design.icon.material_line_weight_outlined_icon import MaterialLineWeightOutlinedIcon
 from apysc._material_design.icon.material_link_icon import MaterialLinkIcon
 from apysc._material_design.icon.material_link_off_icon import MaterialLinkOffIcon
 from apysc._material_design.icon.material_link_off_outlined_icon import MaterialLinkOffOutlinedIcon
 from apysc._material_design.icon.material_link_outlined_icon import MaterialLinkOutlinedIcon
 from apysc._material_design.icon.material_list_alt_icon import MaterialListAltIcon
 from apysc._material_design.icon.material_list_alt_outlined_icon import MaterialListAltOutlinedIcon
@@ -768,14 +794,17 @@
 from apysc._material_design.icon.material_not_accessible_icon import MaterialNotAccessibleIcon
 from apysc._material_design.icon.material_not_accessible_outlined_icon import MaterialNotAccessibleOutlinedIcon
 from apysc._material_design.icon.material_not_interested_icon import MaterialNotInterestedIcon
 from apysc._material_design.icon.material_not_interested_outlined_icon import MaterialNotInterestedOutlinedIcon
 from apysc._material_design.icon.material_not_started_icon import MaterialNotStartedIcon
 from apysc._material_design.icon.material_not_started_outlined_icon import MaterialNotStartedOutlinedIcon
 from apysc._material_design.icon.material_no_sim_icon import MaterialNoSimIcon
+
+_logger.info("Roughly 800 packages have been imported...")
+
 from apysc._material_design.icon.material_no_sim_outlined_icon import MaterialNoSimOutlinedIcon
 from apysc._material_design.icon.material_offline_bolt_icon import MaterialOfflineBoltIcon
 from apysc._material_design.icon.material_offline_bolt_outlined_icon import MaterialOfflineBoltOutlinedIcon
 from apysc._material_design.icon.material_offline_pin_icon import MaterialOfflinePinIcon
 from apysc._material_design.icon.material_offline_pin_outlined_icon import MaterialOfflinePinOutlinedIcon
 from apysc._material_design.icon.material_online_prediction_icon import MaterialOnlinePredictionIcon
 from apysc._material_design.icon.material_online_prediction_outlined_icon import MaterialOnlinePredictionOutlinedIcon
@@ -865,14 +894,17 @@
 from apysc._material_design.icon.material_playlist_play_outlined_icon import MaterialPlaylistPlayOutlinedIcon
 from apysc._material_design.icon.material_play_arrow_icon import MaterialPlayArrowIcon
 from apysc._material_design.icon.material_play_arrow_outlined_icon import MaterialPlayArrowOutlinedIcon
 from apysc._material_design.icon.material_play_circle_filled_icon import MaterialPlayCircleFilledIcon
 from apysc._material_design.icon.material_play_circle_filled_outlined_icon import MaterialPlayCircleFilledOutlinedIcon
 from apysc._material_design.icon.material_play_circle_outline_icon import MaterialPlayCircleOutlineIcon
 from apysc._material_design.icon.material_play_circle_outline_outlined_icon import MaterialPlayCircleOutlineOutlinedIcon
+
+_logger.info("Roughly 900 packages have been imported...")
+
 from apysc._material_design.icon.material_play_disabled_icon import MaterialPlayDisabledIcon
 from apysc._material_design.icon.material_play_for_work_icon import MaterialPlayForWorkIcon
 from apysc._material_design.icon.material_play_for_work_outlined_icon import MaterialPlayForWorkOutlinedIcon
 from apysc._material_design.icon.material_policy_icon import MaterialPolicyIcon
 from apysc._material_design.icon.material_policy_outlined_icon import MaterialPolicyOutlinedIcon
 from apysc._material_design.icon.material_polymer_icon import MaterialPolymerIcon
 from apysc._material_design.icon.material_polymer_outlined_icon import MaterialPolymerOutlinedIcon
@@ -962,14 +994,17 @@
 from apysc._material_design.icon.material_report_icon import MaterialReportIcon
 from apysc._material_design.icon.material_report_off_icon import MaterialReportOffIcon
 from apysc._material_design.icon.material_report_off_outlined_icon import MaterialReportOffOutlinedIcon
 from apysc._material_design.icon.material_report_outlined_icon import MaterialReportOutlinedIcon
 from apysc._material_design.icon.material_report_problem_icon import MaterialReportProblemIcon
 from apysc._material_design.icon.material_report_problem_outlined_icon import MaterialReportProblemOutlinedIcon
 from apysc._material_design.icon.material_request_page_icon import MaterialRequestPageIcon
+
+_logger.info("Roughly 1000 packages have been imported...")
+
 from apysc._material_design.icon.material_request_page_outlined_icon import MaterialRequestPageOutlinedIcon
 from apysc._material_design.icon.material_restore_from_trash_icon import MaterialRestoreFromTrashIcon
 from apysc._material_design.icon.material_restore_from_trash_outlined_icon import MaterialRestoreFromTrashOutlinedIcon
 from apysc._material_design.icon.material_restore_icon import MaterialRestoreIcon
 from apysc._material_design.icon.material_restore_outlined_icon import MaterialRestoreOutlinedIcon
 from apysc._material_design.icon.material_restore_page_icon import MaterialRestorePageIcon
 from apysc._material_design.icon.material_restore_page_outlined_icon import MaterialRestorePageOutlinedIcon
@@ -1059,14 +1094,17 @@
 from apysc._material_design.icon.material_skip_next_icon import MaterialSkipNextIcon
 from apysc._material_design.icon.material_skip_next_outlined_icon import MaterialSkipNextOutlinedIcon
 from apysc._material_design.icon.material_skip_previous_icon import MaterialSkipPreviousIcon
 from apysc._material_design.icon.material_skip_previous_outlined_icon import MaterialSkipPreviousOutlinedIcon
 from apysc._material_design.icon.material_slow_motion_video_icon import MaterialSlowMotionVideoIcon
 from apysc._material_design.icon.material_slow_motion_video_outlined_icon import MaterialSlowMotionVideoOutlinedIcon
 from apysc._material_design.icon.material_smart_button_icon import MaterialSmartButtonIcon
+
+_logger.info("Roughly 1100 packages have been imported...")
+
 from apysc._material_design.icon.material_smart_button_outlined_icon import MaterialSmartButtonOutlinedIcon
 from apysc._material_design.icon.material_snooze_icon import MaterialSnoozeIcon
 from apysc._material_design.icon.material_snooze_outlined_icon import MaterialSnoozeOutlinedIcon
 from apysc._material_design.icon.material_sort_by_alpha_icon import MaterialSortByAlphaIcon
 from apysc._material_design.icon.material_sort_by_alpha_outlined_icon import MaterialSortByAlphaOutlinedIcon
 from apysc._material_design.icon.material_source_icon import MaterialSourceIcon
 from apysc._material_design.icon.material_source_outlined_icon import MaterialSourceOutlinedIcon
@@ -1156,14 +1194,17 @@
 from apysc._material_design.icon.material_theaters_icon import MaterialTheatersIcon
 from apysc._material_design.icon.material_theaters_outlined_icon import MaterialTheatersOutlinedIcon
 from apysc._material_design.icon.material_thumbs_up_down_icon import MaterialThumbsUpDownIcon
 from apysc._material_design.icon.material_thumbs_up_down_outlined_icon import MaterialThumbsUpDownOutlinedIcon
 from apysc._material_design.icon.material_thumb_down_icon import MaterialThumbDownIcon
 from apysc._material_design.icon.material_thumb_down_off_alt_icon import MaterialThumbDownOffAltIcon
 from apysc._material_design.icon.material_thumb_down_outlined_icon import MaterialThumbDownOutlinedIcon
+
+_logger.info("Roughly 1200 packages have been imported...")
+
 from apysc._material_design.icon.material_thumb_up_icon import MaterialThumbUpIcon
 from apysc._material_design.icon.material_thumb_up_off_alt_icon import MaterialThumbUpOffAltIcon
 from apysc._material_design.icon.material_thumb_up_outlined_icon import MaterialThumbUpOutlinedIcon
 from apysc._material_design.icon.material_timeline_icon import MaterialTimelineIcon
 from apysc._material_design.icon.material_timeline_outlined_icon import MaterialTimelineOutlinedIcon
 from apysc._material_design.icon.material_toc_icon import MaterialTocIcon
 from apysc._material_design.icon.material_toc_outlined_icon import MaterialTocOutlinedIcon
@@ -1263,14 +1304,17 @@
 from apysc._material_design.icon.material_warning_outlined_icon import MaterialWarningOutlinedIcon
 from apysc._material_design.icon.material_watch_later_icon import MaterialWatchLaterIcon
 from apysc._material_design.icon.material_watch_later_outlined_icon import MaterialWatchLaterOutlinedIcon
 from apysc._material_design.icon.material_web_asset_icon import MaterialWebAssetIcon
 from apysc._material_design.icon.material_web_asset_outlined_icon import MaterialWebAssetOutlinedIcon
 from apysc._material_design.icon.material_web_icon import MaterialWebIcon
 from apysc._material_design.icon.material_web_outlined_icon import MaterialWebOutlinedIcon
+
+_logger.info("Roughly 1300 packages have been imported...")
+
 from apysc._material_design.icon.material_wifi_calling_icon import MaterialWifiCallingIcon
 from apysc._material_design.icon.material_wifi_calling_outlined_icon import MaterialWifiCallingOutlinedIcon
 from apysc._material_design.icon.material_wifi_protected_setup_icon import MaterialWifiProtectedSetupIcon
 from apysc._material_design.icon.material_wifi_protected_setup_outlined_icon import MaterialWifiProtectedSetupOutlinedIcon
 from apysc._material_design.icon.material_work_icon import MaterialWorkIcon
 from apysc._material_design.icon.material_work_off_icon import MaterialWorkOffIcon
 from apysc._material_design.icon.material_work_off_outlined_icon import MaterialWorkOffOutlinedIcon
@@ -1285,8 +1329,10 @@
 from apysc._material_design.icon.material_zoom_in_outlined_icon import MaterialZoomInOutlinedIcon
 from apysc._material_design.icon.material_zoom_out_icon import MaterialZoomOutIcon
 from apysc._material_design.icon.material_zoom_out_outlined_icon import MaterialZoomOutOutlinedIcon
 
 True_: __True = __True()
 False_: __False = __False()
 
-__version__: str = "4.4.2"
+__version__: str = "4.4.3"
+
+_logger.info("apysc packages imported successfully!")
```

### Comparing `apysc-4.4.2/apysc/_animation/animation_base.py` & `apysc-4.4.3/apysc/_animation/animation_base.py`

 * *Files identical despite different names*

### Comparing `apysc-4.4.2/apysc/_animation/animation_cx.py` & `apysc-4.4.3/apysc/_animation/animation_cx.py`

 * *Files identical despite different names*

### Comparing `apysc-4.4.2/apysc/_animation/animation_cx_mixin.py` & `apysc-4.4.3/apysc/_animation/animation_cx_mixin.py`

 * *Files identical despite different names*

### Comparing `apysc-4.4.2/apysc/_animation/animation_cy.py` & `apysc-4.4.3/apysc/_animation/animation_cy.py`

 * *Files identical despite different names*

### Comparing `apysc-4.4.2/apysc/_animation/animation_cy_mixin.py` & `apysc-4.4.3/apysc/_animation/animation_cy_mixin.py`

 * *Files identical despite different names*

### Comparing `apysc-4.4.2/apysc/_animation/animation_fill_alpha.py` & `apysc-4.4.3/apysc/_animation/animation_fill_alpha.py`

 * *Files identical despite different names*

### Comparing `apysc-4.4.2/apysc/_animation/animation_fill_alpha_mixin.py` & `apysc-4.4.3/apysc/_animation/animation_fill_alpha_mixin.py`

 * *Files identical despite different names*

### Comparing `apysc-4.4.2/apysc/_animation/animation_fill_color.py` & `apysc-4.4.3/apysc/_animation/animation_fill_color.py`

 * *Files identical despite different names*

### Comparing `apysc-4.4.2/apysc/_animation/animation_fill_color_mixin.py` & `apysc-4.4.3/apysc/_animation/animation_fill_color_mixin.py`

 * *Files identical despite different names*

### Comparing `apysc-4.4.2/apysc/_animation/animation_finish_mixin.py` & `apysc-4.4.3/apysc/_animation/animation_finish_mixin.py`

 * *Files identical despite different names*

### Comparing `apysc-4.4.2/apysc/_animation/animation_height.py` & `apysc-4.4.3/apysc/_animation/animation_height.py`

 * *Files identical despite different names*

### Comparing `apysc-4.4.2/apysc/_animation/animation_height_for_ellipse.py` & `apysc-4.4.3/apysc/_animation/animation_height_for_ellipse.py`

 * *Files identical despite different names*

### Comparing `apysc-4.4.2/apysc/_animation/animation_height_for_ellipse_mixin.py` & `apysc-4.4.3/apysc/_animation/animation_height_for_ellipse_mixin.py`

 * *Files identical despite different names*

### Comparing `apysc-4.4.2/apysc/_animation/animation_height_mixin.py` & `apysc-4.4.3/apysc/_animation/animation_height_mixin.py`

 * *Files identical despite different names*

### Comparing `apysc-4.4.2/apysc/_animation/animation_line_alpha.py` & `apysc-4.4.3/apysc/_animation/animation_line_alpha.py`

 * *Files identical despite different names*

### Comparing `apysc-4.4.2/apysc/_animation/animation_line_alpha_mixin.py` & `apysc-4.4.3/apysc/_animation/animation_line_alpha_mixin.py`

 * *Files identical despite different names*

### Comparing `apysc-4.4.2/apysc/_animation/animation_line_color.py` & `apysc-4.4.3/apysc/_animation/animation_line_color.py`

 * *Files identical despite different names*

### Comparing `apysc-4.4.2/apysc/_animation/animation_line_color_mixin.py` & `apysc-4.4.3/apysc/_animation/animation_line_color_mixin.py`

 * *Files identical despite different names*

### Comparing `apysc-4.4.2/apysc/_animation/animation_line_thickness.py` & `apysc-4.4.3/apysc/_animation/animation_line_thickness.py`

 * *Files identical despite different names*

### Comparing `apysc-4.4.2/apysc/_animation/animation_line_thickness_mixin.py` & `apysc-4.4.3/apysc/_animation/animation_line_thickness_mixin.py`

 * *Files identical despite different names*

### Comparing `apysc-4.4.2/apysc/_animation/animation_mixins.py` & `apysc-4.4.3/apysc/_animation/animation_mixins.py`

 * *Files identical despite different names*

### Comparing `apysc-4.4.2/apysc/_animation/animation_move.py` & `apysc-4.4.3/apysc/_animation/animation_move.py`

 * *Files identical despite different names*

### Comparing `apysc-4.4.2/apysc/_animation/animation_move_mixin.py` & `apysc-4.4.3/apysc/_animation/animation_move_mixin.py`

 * *Files identical despite different names*

### Comparing `apysc-4.4.2/apysc/_animation/animation_parallel.py` & `apysc-4.4.3/apysc/_animation/animation_parallel.py`

 * *Files identical despite different names*

### Comparing `apysc-4.4.2/apysc/_animation/animation_parallel_mixin.py` & `apysc-4.4.3/apysc/_animation/animation_parallel_mixin.py`

 * *Files identical despite different names*

### Comparing `apysc-4.4.2/apysc/_animation/animation_pause_mixin.py` & `apysc-4.4.3/apysc/_animation/animation_pause_mixin.py`

 * *Files identical despite different names*

### Comparing `apysc-4.4.2/apysc/_animation/animation_play_mixin.py` & `apysc-4.4.3/apysc/_animation/animation_play_mixin.py`

 * *Files identical despite different names*

### Comparing `apysc-4.4.2/apysc/_animation/animation_radius.py` & `apysc-4.4.3/apysc/_animation/animation_radius.py`

 * *Files identical despite different names*

### Comparing `apysc-4.4.2/apysc/_animation/animation_radius_mixin.py` & `apysc-4.4.3/apysc/_animation/animation_radius_mixin.py`

 * *Files identical despite different names*

### Comparing `apysc-4.4.2/apysc/_animation/animation_reset_mixin.py` & `apysc-4.4.3/apysc/_animation/animation_reset_mixin.py`

 * *Files identical despite different names*

### Comparing `apysc-4.4.2/apysc/_animation/animation_reverse_mixin.py` & `apysc-4.4.3/apysc/_animation/animation_reverse_mixin.py`

 * *Files identical despite different names*

### Comparing `apysc-4.4.2/apysc/_animation/animation_rotation_around_center.py` & `apysc-4.4.3/apysc/_animation/animation_rotation_around_center.py`

 * *Files identical despite different names*

### Comparing `apysc-4.4.2/apysc/_animation/animation_rotation_around_center_mixin.py` & `apysc-4.4.3/apysc/_animation/animation_rotation_around_center_mixin.py`

 * *Files identical despite different names*

### Comparing `apysc-4.4.2/apysc/_animation/animation_rotation_around_point.py` & `apysc-4.4.3/apysc/_animation/animation_rotation_around_point.py`

 * *Files identical despite different names*

### Comparing `apysc-4.4.2/apysc/_animation/animation_rotation_around_point_mixin.py` & `apysc-4.4.3/apysc/_animation/animation_rotation_around_point_mixin.py`

 * *Files identical despite different names*

### Comparing `apysc-4.4.2/apysc/_animation/animation_scale_x_from_center.py` & `apysc-4.4.3/apysc/_animation/animation_scale_x_from_center.py`

 * *Files identical despite different names*

### Comparing `apysc-4.4.2/apysc/_animation/animation_scale_x_from_center_mixin.py` & `apysc-4.4.3/apysc/_animation/animation_scale_x_from_center_mixin.py`

 * *Files identical despite different names*

### Comparing `apysc-4.4.2/apysc/_animation/animation_scale_x_from_point.py` & `apysc-4.4.3/apysc/_animation/animation_scale_x_from_point.py`

 * *Files identical despite different names*

### Comparing `apysc-4.4.2/apysc/_animation/animation_scale_x_from_point_mixin.py` & `apysc-4.4.3/apysc/_animation/animation_scale_x_from_point_mixin.py`

 * *Files identical despite different names*

### Comparing `apysc-4.4.2/apysc/_animation/animation_scale_y_from_center.py` & `apysc-4.4.3/apysc/_animation/animation_scale_y_from_center.py`

 * *Files identical despite different names*

### Comparing `apysc-4.4.2/apysc/_animation/animation_scale_y_from_center_mixin.py` & `apysc-4.4.3/apysc/_animation/animation_scale_y_from_center_mixin.py`

 * *Files identical despite different names*

### Comparing `apysc-4.4.2/apysc/_animation/animation_scale_y_from_point.py` & `apysc-4.4.3/apysc/_animation/animation_scale_y_from_point.py`

 * *Files identical despite different names*

### Comparing `apysc-4.4.2/apysc/_animation/animation_scale_y_from_point_mixin.py` & `apysc-4.4.3/apysc/_animation/animation_scale_y_from_point_mixin.py`

 * *Files identical despite different names*

### Comparing `apysc-4.4.2/apysc/_animation/animation_time_mixin.py` & `apysc-4.4.3/apysc/_animation/animation_time_mixin.py`

 * *Files identical despite different names*

### Comparing `apysc-4.4.2/apysc/_animation/animation_width.py` & `apysc-4.4.3/apysc/_animation/animation_width.py`

 * *Files identical despite different names*

### Comparing `apysc-4.4.2/apysc/_animation/animation_width_for_ellipse.py` & `apysc-4.4.3/apysc/_animation/animation_width_for_ellipse.py`

 * *Files identical despite different names*

### Comparing `apysc-4.4.2/apysc/_animation/animation_width_for_ellipse_mixin.py` & `apysc-4.4.3/apysc/_animation/animation_width_for_ellipse_mixin.py`

 * *Files identical despite different names*

### Comparing `apysc-4.4.2/apysc/_animation/animation_width_mixin.py` & `apysc-4.4.3/apysc/_animation/animation_width_mixin.py`

 * *Files identical despite different names*

### Comparing `apysc-4.4.2/apysc/_animation/animation_x.py` & `apysc-4.4.3/apysc/_animation/animation_x.py`

 * *Files identical despite different names*

### Comparing `apysc-4.4.2/apysc/_animation/animation_x_mixin.py` & `apysc-4.4.3/apysc/_animation/animation_x_mixin.py`

 * *Files identical despite different names*

### Comparing `apysc-4.4.2/apysc/_animation/animation_y.py` & `apysc-4.4.3/apysc/_animation/animation_y.py`

 * *Files identical despite different names*

### Comparing `apysc-4.4.2/apysc/_animation/animation_y_mixin.py` & `apysc-4.4.3/apysc/_animation/animation_y_mixin.py`

 * *Files identical despite different names*

### Comparing `apysc-4.4.2/apysc/_animation/easing.py` & `apysc-4.4.3/apysc/_animation/easing.py`

 * *Files identical despite different names*

### Comparing `apysc-4.4.2/apysc/_auto_reloading/auto_reloading_decorator.py` & `apysc-4.4.3/apysc/_auto_reloading/auto_reloading_decorator.py`

 * *Files identical despite different names*

### Comparing `apysc-4.4.2/apysc/_branch/_elif.py` & `apysc-4.4.3/apysc/_branch/_elif.py`

 * *Files identical despite different names*

### Comparing `apysc-4.4.2/apysc/_branch/_else.py` & `apysc-4.4.3/apysc/_branch/_else.py`

 * *Files identical despite different names*

### Comparing `apysc-4.4.2/apysc/_branch/_if.py` & `apysc-4.4.3/apysc/_branch/_if.py`

 * *Files identical despite different names*

### Comparing `apysc-4.4.2/apysc/_branch/if_base.py` & `apysc-4.4.3/apysc/_branch/if_base.py`

 * *Files identical despite different names*

### Comparing `apysc-4.4.2/apysc/_callable/callable_util.py` & `apysc-4.4.3/apysc/_callable/callable_util.py`

 * *Files identical despite different names*

### Comparing `apysc-4.4.2/apysc/_chart/add_background_mixin.py` & `apysc-4.4.3/apysc/_chart/add_background_mixin.py`

 * *Files identical despite different names*

### Comparing `apysc-4.4.2/apysc/_chart/add_border_mixin.py` & `apysc-4.4.3/apysc/_chart/add_border_mixin.py`

 * *Files identical despite different names*

### Comparing `apysc-4.4.2/apysc/_chart/axis_label_bold_mixin.py` & `apysc-4.4.3/apysc/_chart/axis_label_bold_mixin.py`

 * *Files identical despite different names*

### Comparing `apysc-4.4.2/apysc/_chart/axis_label_fill_alpha_mixin.py` & `apysc-4.4.3/apysc/_chart/axis_label_fill_alpha_mixin.py`

 * *Files identical despite different names*

### Comparing `apysc-4.4.2/apysc/_chart/axis_label_fill_color_mixin.py` & `apysc-4.4.3/apysc/_chart/axis_label_fill_color_mixin.py`

 * *Files identical despite different names*

### Comparing `apysc-4.4.2/apysc/_chart/axis_label_font_family_mixin.py` & `apysc-4.4.3/apysc/_chart/axis_label_font_family_mixin.py`

 * *Files identical despite different names*

### Comparing `apysc-4.4.2/apysc/_chart/axis_label_font_size_mixin.py` & `apysc-4.4.3/apysc/_chart/axis_label_font_size_mixin.py`

 * *Files identical despite different names*

### Comparing `apysc-4.4.2/apysc/_chart/axis_label_italic_mixin.py` & `apysc-4.4.3/apysc/_chart/axis_label_italic_mixin.py`

 * *Files identical despite different names*

### Comparing `apysc-4.4.2/apysc/_chart/axis_line_alpha_mixin.py` & `apysc-4.4.3/apysc/_chart/axis_line_alpha_mixin.py`

 * *Files identical despite different names*

### Comparing `apysc-4.4.2/apysc/_chart/axis_line_color_mixin.py` & `apysc-4.4.3/apysc/_chart/axis_line_color_mixin.py`

 * *Files identical despite different names*

### Comparing `apysc-4.4.2/apysc/_chart/axis_line_thickness_mixin.py` & `apysc-4.4.3/apysc/_chart/axis_line_thickness_mixin.py`

 * *Files identical despite different names*

### Comparing `apysc-4.4.2/apysc/_chart/background_container_mixin.py` & `apysc-4.4.3/apysc/_chart/background_container_mixin.py`

 * *Files identical despite different names*

### Comparing `apysc-4.4.2/apysc/_chart/border_container_mixin.py` & `apysc-4.4.3/apysc/_chart/border_container_mixin.py`

 * *Files identical despite different names*

### Comparing `apysc-4.4.2/apysc/_chart/chart_container_mixin.py` & `apysc-4.4.3/apysc/_chart/chart_container_mixin.py`

 * *Files identical despite different names*

### Comparing `apysc-4.4.2/apysc/_chart/create_single_column_y_axis_mixin.py` & `apysc-4.4.3/apysc/_chart/create_single_column_y_axis_mixin.py`

 * *Files identical despite different names*

### Comparing `apysc-4.4.2/apysc/_chart/initialize_each_container_mixin.py` & `apysc-4.4.3/apysc/_chart/initialize_each_container_mixin.py`

 * *Files identical despite different names*

### Comparing `apysc-4.4.2/apysc/_chart/is_display_axis_label_mixin.py` & `apysc-4.4.3/apysc/_chart/is_display_axis_label_mixin.py`

 * *Files identical despite different names*

### Comparing `apysc-4.4.2/apysc/_chart/overall_container_mixin.py` & `apysc-4.4.3/apysc/_chart/overall_container_mixin.py`

 * *Files identical despite different names*

### Comparing `apysc-4.4.2/apysc/_chart/set_initial_background_fill_alpha_mixin.py` & `apysc-4.4.3/apysc/_chart/set_initial_background_fill_alpha_mixin.py`

 * *Files identical despite different names*

### Comparing `apysc-4.4.2/apysc/_chart/set_initial_background_fill_color_mixin.py` & `apysc-4.4.3/apysc/_chart/set_initial_background_fill_color_mixin.py`

 * *Files identical despite different names*

### Comparing `apysc-4.4.2/apysc/_chart/set_initial_border_alpha_mixin.py` & `apysc-4.4.3/apysc/_chart/set_initial_border_alpha_mixin.py`

 * *Files identical despite different names*

### Comparing `apysc-4.4.2/apysc/_chart/set_initial_border_color_mixin.py` & `apysc-4.4.3/apysc/_chart/set_initial_border_color_mixin.py`

 * *Files identical despite different names*

### Comparing `apysc-4.4.2/apysc/_chart/set_initial_border_thickness_mixin.py` & `apysc-4.4.3/apysc/_chart/set_initial_border_thickness_mixin.py`

 * *Files identical despite different names*

### Comparing `apysc-4.4.2/apysc/_chart/set_initial_height_mixin.py` & `apysc-4.4.3/apysc/_chart/set_initial_height_mixin.py`

 * *Files identical despite different names*

### Comparing `apysc-4.4.2/apysc/_chart/set_initial_horizontal_padding_mixin.py` & `apysc-4.4.3/apysc/_chart/set_initial_horizontal_padding_mixin.py`

 * *Files identical despite different names*

### Comparing `apysc-4.4.2/apysc/_chart/set_initial_matrix_data_mixin.py` & `apysc-4.4.3/apysc/_chart/set_initial_matrix_data_mixin.py`

 * *Files identical despite different names*

### Comparing `apysc-4.4.2/apysc/_chart/set_initial_overall_container_coordinates_mixin.py` & `apysc-4.4.3/apysc/_chart/set_initial_overall_container_coordinates_mixin.py`

 * *Files identical despite different names*

### Comparing `apysc-4.4.2/apysc/_chart/set_initial_vertical_padding_mixin.py` & `apysc-4.4.3/apysc/_chart/set_initial_vertical_padding_mixin.py`

 * *Files identical despite different names*

### Comparing `apysc-4.4.2/apysc/_chart/set_initial_width_mixin.py` & `apysc-4.4.3/apysc/_chart/set_initial_width_mixin.py`

 * *Files identical despite different names*

### Comparing `apysc-4.4.2/apysc/_chart/set_initial_x_mixin.py` & `apysc-4.4.3/apysc/_chart/set_initial_x_mixin.py`

 * *Files identical despite different names*

### Comparing `apysc-4.4.2/apysc/_chart/set_initial_y_mixin.py` & `apysc-4.4.3/apysc/_chart/set_initial_y_mixin.py`

 * *Files identical despite different names*

### Comparing `apysc-4.4.2/apysc/_chart/tick_max_num_mixin.py` & `apysc-4.4.3/apysc/_chart/tick_max_num_mixin.py`

 * *Files identical despite different names*

### Comparing `apysc-4.4.2/apysc/_chart/tick_text_bold_mixin.py` & `apysc-4.4.3/apysc/_chart/tick_text_bold_mixin.py`

 * *Files identical despite different names*

### Comparing `apysc-4.4.2/apysc/_chart/tick_text_fill_alpha_mixin.py` & `apysc-4.4.3/apysc/_chart/tick_text_fill_alpha_mixin.py`

 * *Files identical despite different names*

### Comparing `apysc-4.4.2/apysc/_chart/tick_text_fill_color_mixin.py` & `apysc-4.4.3/apysc/_chart/tick_text_fill_color_mixin.py`

 * *Files identical despite different names*

### Comparing `apysc-4.4.2/apysc/_chart/tick_text_font_family_mixin.py` & `apysc-4.4.3/apysc/_chart/tick_text_font_family_mixin.py`

 * *Files identical despite different names*

### Comparing `apysc-4.4.2/apysc/_chart/tick_text_font_size_mixin.py` & `apysc-4.4.3/apysc/_chart/tick_text_font_size_mixin.py`

 * *Files identical despite different names*

### Comparing `apysc-4.4.2/apysc/_chart/tick_text_italic_mixin.py` & `apysc-4.4.3/apysc/_chart/tick_text_italic_mixin.py`

 * *Files identical despite different names*

### Comparing `apysc-4.4.2/apysc/_chart/tick_text_max_num_of_decimal_places_mixin.py` & `apysc-4.4.3/apysc/_chart/tick_text_max_num_of_decimal_places_mixin.py`

 * *Files identical despite different names*

### Comparing `apysc-4.4.2/apysc/_chart/vertical_bar_chart.py` & `apysc-4.4.3/apysc/_chart/vertical_bar_chart.py`

 * *Files identical despite different names*

### Comparing `apysc-4.4.2/apysc/_chart/x_axis_column_name_mixin.py` & `apysc-4.4.3/apysc/_chart/x_axis_column_name_mixin.py`

 * *Files identical despite different names*

### Comparing `apysc-4.4.2/apysc/_chart/x_axis_container_mixin.py` & `apysc-4.4.3/apysc/_chart/x_axis_container_mixin.py`

 * *Files identical despite different names*

### Comparing `apysc-4.4.2/apysc/_chart/x_axis_label_position_mixin.py` & `apysc-4.4.3/apysc/_chart/x_axis_label_position_mixin.py`

 * *Files identical despite different names*

### Comparing `apysc-4.4.2/apysc/_chart/x_axis_settings.py` & `apysc-4.4.3/apysc/_chart/x_axis_settings.py`

 * *Files identical despite different names*

### Comparing `apysc-4.4.2/apysc/_chart/y_axis_column_name_mixin.py` & `apysc-4.4.3/apysc/_chart/y_axis_column_name_mixin.py`

 * *Files identical despite different names*

### Comparing `apysc-4.4.2/apysc/_chart/y_axis_container_mixin.py` & `apysc-4.4.3/apysc/_chart/y_axis_container_mixin.py`

 * *Files identical despite different names*

### Comparing `apysc-4.4.2/apysc/_chart/y_axis_label_position_mixin.py` & `apysc-4.4.3/apysc/_chart/y_axis_label_position_mixin.py`

 * *Files identical despite different names*

### Comparing `apysc-4.4.2/apysc/_chart/y_axis_single_column_settings.py` & `apysc-4.4.3/apysc/_chart/y_axis_single_column_settings.py`

 * *Files 0% similar despite different names*

```diff
@@ -156,15 +156,15 @@
         Parameters
         ----------
         y_axis_column_name : Union[str, String]
             Y-axis column name.
             Only a number (integer or float) column is a selectable
             value (for example, price, sales, or percentage column).
         y_min : Optional[Union[float, Number]], optional
-            A minumum y-axis value.
+            A minimum y-axis value.
         y_max : Optional[Union[float, Number]], optional
             A maximum y-axis value.
         tick_max_num : Optional[Union[int, Int]], optional
             A tick max display number. Often tick display number
             becomes under this value.
         tick_text_font_size : Union[int, Int], optional
             A tick text font-size setting.
```

### Comparing `apysc-4.4.2/apysc/_chart/y_max_mixin.py` & `apysc-4.4.3/apysc/_chart/y_max_mixin.py`

 * *Files identical despite different names*

### Comparing `apysc-4.4.2/apysc/_chart/y_min_mixin.py` & `apysc-4.4.3/apysc/_chart/y_min_mixin.py`

 * *Files identical despite different names*

### Comparing `apysc-4.4.2/apysc/_color/blue_color_mixin.py` & `apysc-4.4.3/apysc/_color/blue_color_mixin.py`

 * *Files identical despite different names*

### Comparing `apysc-4.4.2/apysc/_color/color.py` & `apysc-4.4.3/apysc/_color/color.py`

 * *Files identical despite different names*

### Comparing `apysc-4.4.2/apysc/_color/color_copy_mixin.py` & `apysc-4.4.3/apysc/_color/color_copy_mixin.py`

 * *Files identical despite different names*

### Comparing `apysc-4.4.2/apysc/_color/color_util.py` & `apysc-4.4.3/apysc/_color/color_util.py`

 * *Files identical despite different names*

### Comparing `apysc-4.4.2/apysc/_color/colors.py` & `apysc-4.4.3/apysc/_color/colors.py`

 * *Files identical despite different names*

### Comparing `apysc-4.4.2/apysc/_color/copy_color_if_default_value_specified_mixin.py` & `apysc-4.4.3/apysc/_color/copy_color_if_default_value_specified_mixin.py`

 * *Files identical despite different names*

### Comparing `apysc-4.4.2/apysc/_color/from_rgb_mixin.py` & `apysc-4.4.3/apysc/_color/from_rgb_mixin.py`

 * *Files identical despite different names*

### Comparing `apysc-4.4.2/apysc/_color/get_colors_members_mixin.py` & `apysc-4.4.3/apysc/_color/get_colors_members_mixin.py`

 * *Files identical despite different names*

### Comparing `apysc-4.4.2/apysc/_color/green_color_mixin.py` & `apysc-4.4.3/apysc/_color/green_color_mixin.py`

 * *Files identical despite different names*

### Comparing `apysc-4.4.2/apysc/_color/red_color_mixin.py` & `apysc-4.4.3/apysc/_color/red_color_mixin.py`

 * *Files identical despite different names*

### Comparing `apysc-4.4.2/apysc/_console/_trace.py` & `apysc-4.4.3/apysc/_console/_trace.py`

 * *Files identical despite different names*

### Comparing `apysc-4.4.2/apysc/_console/assertion.py` & `apysc-4.4.3/apysc/_console/assertion.py`

 * *Files identical despite different names*

### Comparing `apysc-4.4.2/apysc/_console/loggers.py` & `apysc-4.4.3/apysc/_console/loggers.py`

 * *Files identical despite different names*

### Comparing `apysc-4.4.2/apysc/_converter/cast.py` & `apysc-4.4.3/apysc/_converter/cast.py`

 * *Files identical despite different names*

### Comparing `apysc-4.4.2/apysc/_converter/to_apysc_val_from_builtin.py` & `apysc-4.4.3/apysc/_converter/to_apysc_val_from_builtin.py`

 * *Files identical despite different names*

### Comparing `apysc-4.4.2/apysc/_converter/to_builtin_val_from_apysc.py` & `apysc-4.4.3/apysc/_converter/to_builtin_val_from_apysc.py`

 * *Files identical despite different names*

### Comparing `apysc-4.4.2/apysc/_display/_document.py` & `apysc-4.4.3/apysc/_display/_document.py`

 * *Files identical despite different names*

### Comparing `apysc-4.4.2/apysc/_display/add_foreign_object_child_mixin.py` & `apysc-4.4.3/apysc/_display/add_foreign_object_child_mixin.py`

 * *Files identical despite different names*

### Comparing `apysc-4.4.2/apysc/_display/add_to_parent_mixin.py` & `apysc-4.4.3/apysc/_display/add_to_parent_mixin.py`

 * *Files identical despite different names*

### Comparing `apysc-4.4.2/apysc/_display/any_display_object.py` & `apysc-4.4.3/apysc/_display/any_display_object.py`

 * *Files identical despite different names*

### Comparing `apysc-4.4.2/apysc/_display/append_fill_alpha_attr_expression_mixin.py` & `apysc-4.4.3/apysc/_display/append_fill_alpha_attr_expression_mixin.py`

 * *Files identical despite different names*

### Comparing `apysc-4.4.2/apysc/_display/append_fill_color_expression_mixin.py` & `apysc-4.4.3/apysc/_display/append_fill_color_expression_mixin.py`

 * *Files identical despite different names*

### Comparing `apysc-4.4.2/apysc/_display/append_foreign_object_constructor_expression_mixin.py` & `apysc-4.4.3/apysc/_display/append_foreign_object_constructor_expression_mixin.py`

 * *Files identical despite different names*

### Comparing `apysc-4.4.2/apysc/_display/append_line_alpha_attr_expression_mixin.py` & `apysc-4.4.3/apysc/_display/append_line_alpha_attr_expression_mixin.py`

 * *Files identical despite different names*

### Comparing `apysc-4.4.2/apysc/_display/append_line_cap_attr_expression_mixin.py` & `apysc-4.4.3/apysc/_display/append_line_cap_attr_expression_mixin.py`

 * *Files identical despite different names*

### Comparing `apysc-4.4.2/apysc/_display/append_line_color_attr_expression_mixin.py` & `apysc-4.4.3/apysc/_display/append_line_color_attr_expression_mixin.py`

 * *Files identical despite different names*

### Comparing `apysc-4.4.2/apysc/_display/append_line_joints_attr_expression_mixin.py` & `apysc-4.4.3/apysc/_display/append_line_joints_attr_expression_mixin.py`

 * *Files identical despite different names*

### Comparing `apysc-4.4.2/apysc/_display/append_line_point_mixin.py` & `apysc-4.4.3/apysc/_display/append_line_point_mixin.py`

 * *Files identical despite different names*

### Comparing `apysc-4.4.2/apysc/_display/append_line_thickness_attr_expression_mixin.py` & `apysc-4.4.3/apysc/_display/append_line_thickness_attr_expression_mixin.py`

 * *Files identical despite different names*

### Comparing `apysc-4.4.2/apysc/_display/append_x_attr_expression_mixin.py` & `apysc-4.4.3/apysc/_display/append_x_attr_expression_mixin.py`

 * *Files identical despite different names*

### Comparing `apysc-4.4.2/apysc/_display/append_y_attr_expression_mixin.py` & `apysc-4.4.3/apysc/_display/append_y_attr_expression_mixin.py`

 * *Files identical despite different names*

### Comparing `apysc-4.4.2/apysc/_display/begin_fill_mixin.py` & `apysc-4.4.3/apysc/_display/begin_fill_mixin.py`

 * *Files identical despite different names*

### Comparing `apysc-4.4.2/apysc/_display/child_mixin.py` & `apysc-4.4.3/apysc/_display/child_mixin.py`

 * *Files identical despite different names*

### Comparing `apysc-4.4.2/apysc/_display/circle.py` & `apysc-4.4.3/apysc/_display/circle.py`

 * *Files identical despite different names*

### Comparing `apysc-4.4.2/apysc/_display/css_interface.py` & `apysc-4.4.3/apysc/_display/css_interface.py`

 * *Files identical despite different names*

### Comparing `apysc-4.4.2/apysc/_display/css_mixin.py` & `apysc-4.4.3/apysc/_display/css_mixin.py`

 * *Files identical despite different names*

### Comparing `apysc-4.4.2/apysc/_display/cx_mixin.py` & `apysc-4.4.3/apysc/_display/cx_mixin.py`

 * *Files identical despite different names*

### Comparing `apysc-4.4.2/apysc/_display/cy_mixin.py` & `apysc-4.4.3/apysc/_display/cy_mixin.py`

 * *Files identical despite different names*

### Comparing `apysc-4.4.2/apysc/_display/display_object.py` & `apysc-4.4.3/apysc/_display/display_object.py`

 * *Files 2% similar despite different names*

```diff
@@ -1,8 +1,8 @@
-"""Implementations for DisplayObject class.
+"""Implementation for DisplayObject class.
 """
 
 from apysc._animation.animation_parallel_mixin import AnimationParallelMixIn
 from apysc._display.css_interface import CssInterface
 from apysc._display.parent_mixin import ParentMixIn
 from apysc._display.visible_mixin import VisibleMixIn
 from apysc._event.custom_event_mixin import CustomEventMixIn
```

### Comparing `apysc-4.4.2/apysc/_display/ellipse.py` & `apysc-4.4.3/apysc/_display/ellipse.py`

 * *Files identical despite different names*

### Comparing `apysc-4.4.2/apysc/_display/ellipse_height_mixin.py` & `apysc-4.4.3/apysc/_display/ellipse_height_mixin.py`

 * *Files identical despite different names*

### Comparing `apysc-4.4.2/apysc/_display/ellipse_width_mixin.py` & `apysc-4.4.3/apysc/_display/ellipse_width_mixin.py`

 * *Files identical despite different names*

### Comparing `apysc-4.4.2/apysc/_display/fill_alpha_mixin.py` & `apysc-4.4.3/apysc/_display/fill_alpha_mixin.py`

 * *Files identical despite different names*

### Comparing `apysc-4.4.2/apysc/_display/fill_color_mixin.py` & `apysc-4.4.3/apysc/_display/fill_color_mixin.py`

 * *Files identical despite different names*

### Comparing `apysc-4.4.2/apysc/_display/fixed_html_svg_icon_base.py` & `apysc-4.4.3/apysc/_display/fixed_html_svg_icon_base.py`

 * *Files identical despite different names*

### Comparing `apysc-4.4.2/apysc/_display/flip_interface_helper.py` & `apysc-4.4.3/apysc/_display/flip_interface_helper.py`

 * *Files identical despite different names*

### Comparing `apysc-4.4.2/apysc/_display/flip_x_mixin.py` & `apysc-4.4.3/apysc/_display/flip_x_mixin.py`

 * *Files identical despite different names*

### Comparing `apysc-4.4.2/apysc/_display/flip_y_mixin.py` & `apysc-4.4.3/apysc/_display/flip_y_mixin.py`

 * *Files identical despite different names*

### Comparing `apysc-4.4.2/apysc/_display/get_bounds_mixin.py` & `apysc-4.4.3/apysc/_display/get_bounds_mixin.py`

 * *Files identical despite different names*

### Comparing `apysc-4.4.2/apysc/_display/graphics.py` & `apysc-4.4.3/apysc/_display/graphics.py`

 * *Files identical despite different names*

### Comparing `apysc-4.4.2/apysc/_display/graphics_base.py` & `apysc-4.4.3/apysc/_display/graphics_base.py`

 * *Files identical despite different names*

### Comparing `apysc-4.4.2/apysc/_display/graphics_clear_mixin.py` & `apysc-4.4.3/apysc/_display/graphics_clear_mixin.py`

 * *Files identical despite different names*

### Comparing `apysc-4.4.2/apysc/_display/graphics_expression.py` & `apysc-4.4.3/apysc/_display/graphics_expression.py`

 * *Files identical despite different names*

### Comparing `apysc-4.4.2/apysc/_display/height_mixin.py` & `apysc-4.4.3/apysc/_display/height_mixin.py`

 * *Files identical despite different names*

### Comparing `apysc-4.4.2/apysc/_display/line.py` & `apysc-4.4.3/apysc/_display/line.py`

 * *Files identical despite different names*

### Comparing `apysc-4.4.2/apysc/_display/line_alpha_mixin.py` & `apysc-4.4.3/apysc/_display/line_alpha_mixin.py`

 * *Files identical despite different names*

### Comparing `apysc-4.4.2/apysc/_display/line_cap_mixin.py` & `apysc-4.4.3/apysc/_display/line_cap_mixin.py`

 * *Files identical despite different names*

### Comparing `apysc-4.4.2/apysc/_display/line_caps.py` & `apysc-4.4.3/apysc/_display/line_caps.py`

 * *Files identical despite different names*

### Comparing `apysc-4.4.2/apysc/_display/line_color_mixin.py` & `apysc-4.4.3/apysc/_display/line_color_mixin.py`

 * *Files identical despite different names*

### Comparing `apysc-4.4.2/apysc/_display/line_dash_dot_setting.py` & `apysc-4.4.3/apysc/_display/line_dash_dot_setting.py`

 * *Files identical despite different names*

### Comparing `apysc-4.4.2/apysc/_display/line_dash_dot_setting_mixin.py` & `apysc-4.4.3/apysc/_display/line_dash_dot_setting_mixin.py`

 * *Files identical despite different names*

### Comparing `apysc-4.4.2/apysc/_display/line_dash_setting.py` & `apysc-4.4.3/apysc/_display/line_dash_setting.py`

 * *Files identical despite different names*

### Comparing `apysc-4.4.2/apysc/_display/line_dash_setting_mixin.py` & `apysc-4.4.3/apysc/_display/line_dash_setting_mixin.py`

 * *Files identical despite different names*

### Comparing `apysc-4.4.2/apysc/_display/line_dot_setting.py` & `apysc-4.4.3/apysc/_display/line_dot_setting.py`

 * *Files identical despite different names*

### Comparing `apysc-4.4.2/apysc/_display/line_dot_setting_mixin.py` & `apysc-4.4.3/apysc/_display/line_dot_setting_mixin.py`

 * *Files identical despite different names*

### Comparing `apysc-4.4.2/apysc/_display/line_joints.py` & `apysc-4.4.3/apysc/_display/line_joints.py`

 * *Files identical despite different names*

### Comparing `apysc-4.4.2/apysc/_display/line_joints_mixin.py` & `apysc-4.4.3/apysc/_display/line_joints_mixin.py`

 * *Files identical despite different names*

### Comparing `apysc-4.4.2/apysc/_display/line_round_dot_setting.py` & `apysc-4.4.3/apysc/_display/line_round_dot_setting.py`

 * *Files identical despite different names*

### Comparing `apysc-4.4.2/apysc/_display/line_round_dot_setting_mixin.py` & `apysc-4.4.3/apysc/_display/line_round_dot_setting_mixin.py`

 * *Files identical despite different names*

### Comparing `apysc-4.4.2/apysc/_display/line_style_mixin.py` & `apysc-4.4.3/apysc/_display/line_style_mixin.py`

 * *Files identical despite different names*

### Comparing `apysc-4.4.2/apysc/_display/line_thickness_mixin.py` & `apysc-4.4.3/apysc/_display/line_thickness_mixin.py`

 * *Files identical despite different names*

### Comparing `apysc-4.4.2/apysc/_display/multi_line_text.py` & `apysc-4.4.3/apysc/_display/multi_line_text.py`

 * *Files identical despite different names*

### Comparing `apysc-4.4.2/apysc/_display/opacity_css_mixin.py` & `apysc-4.4.3/apysc/_display/opacity_css_mixin.py`

 * *Files identical despite different names*

### Comparing `apysc-4.4.2/apysc/_display/parent_mixin.py` & `apysc-4.4.3/apysc/_display/parent_mixin.py`

 * *Files identical despite different names*

### Comparing `apysc-4.4.2/apysc/_display/path.py` & `apysc-4.4.3/apysc/_display/path.py`

 * *Files identical despite different names*

### Comparing `apysc-4.4.2/apysc/_display/points_2d_mixin.py` & `apysc-4.4.3/apysc/_display/points_2d_mixin.py`

 * *Files identical despite different names*

### Comparing `apysc-4.4.2/apysc/_display/polygon.py` & `apysc-4.4.3/apysc/_display/polygon.py`

 * *Files identical despite different names*

### Comparing `apysc-4.4.2/apysc/_display/polygon_append_constructor_expression_mixin.py` & `apysc-4.4.3/apysc/_display/polygon_append_constructor_expression_mixin.py`

 * *Files identical despite different names*

### Comparing `apysc-4.4.2/apysc/_display/polygon_apply_current_points_mixin.py` & `apysc-4.4.3/apysc/_display/polygon_apply_current_points_mixin.py`

 * *Files identical despite different names*

### Comparing `apysc-4.4.2/apysc/_display/polygon_x1_mixin.py` & `apysc-4.4.3/apysc/_display/polygon_x1_mixin.py`

 * *Files identical despite different names*

### Comparing `apysc-4.4.2/apysc/_display/polygon_x2_mixin.py` & `apysc-4.4.3/apysc/_display/polygon_x2_mixin.py`

 * *Files identical despite different names*

### Comparing `apysc-4.4.2/apysc/_display/polygon_x3_mixin.py` & `apysc-4.4.3/apysc/_display/polygon_x3_mixin.py`

 * *Files identical despite different names*

### Comparing `apysc-4.4.2/apysc/_display/polygon_y1_mixin.py` & `apysc-4.4.3/apysc/_display/polygon_y1_mixin.py`

 * *Files identical despite different names*

### Comparing `apysc-4.4.2/apysc/_display/polygon_y2_mixin.py` & `apysc-4.4.3/apysc/_display/polygon_y2_mixin.py`

 * *Files identical despite different names*

### Comparing `apysc-4.4.2/apysc/_display/polygon_y3_mixin.py` & `apysc-4.4.3/apysc/_display/polygon_y3_mixin.py`

 * *Files identical despite different names*

### Comparing `apysc-4.4.2/apysc/_display/polyline.py` & `apysc-4.4.3/apysc/_display/polyline.py`

 * *Files identical despite different names*

### Comparing `apysc-4.4.2/apysc/_display/radius_mixin.py` & `apysc-4.4.3/apysc/_display/radius_mixin.py`

 * *Files identical despite different names*

### Comparing `apysc-4.4.2/apysc/_display/rectangle.py` & `apysc-4.4.3/apysc/_display/rectangle.py`

 * *Files identical despite different names*

### Comparing `apysc-4.4.2/apysc/_display/rotation_around_center_mixin.py` & `apysc-4.4.3/apysc/_display/rotation_around_center_mixin.py`

 * *Files identical despite different names*

### Comparing `apysc-4.4.2/apysc/_display/rotation_around_point_mixin.py` & `apysc-4.4.3/apysc/_display/rotation_around_point_mixin.py`

 * *Files identical despite different names*

### Comparing `apysc-4.4.2/apysc/_display/rotation_interface_helper.py` & `apysc-4.4.3/apysc/_display/rotation_interface_helper.py`

 * *Files identical despite different names*

### Comparing `apysc-4.4.2/apysc/_display/scale_interface_helper.py` & `apysc-4.4.3/apysc/_display/scale_interface_helper.py`

 * *Files identical despite different names*

### Comparing `apysc-4.4.2/apysc/_display/scale_x_from_center_mixin.py` & `apysc-4.4.3/apysc/_display/scale_x_from_center_mixin.py`

 * *Files identical despite different names*

### Comparing `apysc-4.4.2/apysc/_display/scale_x_from_point_mixin.py` & `apysc-4.4.3/apysc/_display/scale_x_from_point_mixin.py`

 * *Files identical despite different names*

### Comparing `apysc-4.4.2/apysc/_display/scale_y_from_center_mixin.py` & `apysc-4.4.3/apysc/_display/scale_y_from_center_mixin.py`

 * *Files identical despite different names*

### Comparing `apysc-4.4.2/apysc/_display/scale_y_from_point_mixin.py` & `apysc-4.4.3/apysc/_display/scale_y_from_point_mixin.py`

 * *Files identical despite different names*

### Comparing `apysc-4.4.2/apysc/_display/set_lower_scale_limit_mixin.py` & `apysc-4.4.3/apysc/_display/set_lower_scale_limit_mixin.py`

 * *Files identical despite different names*

### Comparing `apysc-4.4.2/apysc/_display/set_overflow_visible_setting_mixin.py` & `apysc-4.4.3/apysc/_display/set_overflow_visible_setting_mixin.py`

 * *Files identical despite different names*

### Comparing `apysc-4.4.2/apysc/_display/skew_x_mixin.py` & `apysc-4.4.3/apysc/_display/skew_x_mixin.py`

 * *Files identical despite different names*

### Comparing `apysc-4.4.2/apysc/_display/skew_y_mixin.py` & `apysc-4.4.3/apysc/_display/skew_y_mixin.py`

 * *Files identical despite different names*

### Comparing `apysc-4.4.2/apysc/_display/sprite.py` & `apysc-4.4.3/apysc/_display/sprite.py`

 * *Files identical despite different names*

### Comparing `apysc-4.4.2/apysc/_display/stage.py` & `apysc-4.4.3/apysc/_display/stage.py`

 * *Files identical despite different names*

### Comparing `apysc-4.4.2/apysc/_display/svg_foreign_object_child.py` & `apysc-4.4.3/apysc/_display/svg_foreign_object_child.py`

 * *Files identical despite different names*

### Comparing `apysc-4.4.2/apysc/_display/svg_foreign_object_child_mixin.py` & `apysc-4.4.3/apysc/_display/svg_foreign_object_child_mixin.py`

 * *Files identical despite different names*

### Comparing `apysc-4.4.2/apysc/_display/svg_foreign_object_initialize_width_mixin.py` & `apysc-4.4.3/apysc/_display/svg_foreign_object_initialize_width_mixin.py`

 * *Files identical despite different names*

### Comparing `apysc-4.4.2/apysc/_display/svg_foreign_object_text_mixin.py` & `apysc-4.4.3/apysc/_display/svg_foreign_object_text_mixin.py`

 * *Files identical despite different names*

### Comparing `apysc-4.4.2/apysc/_display/svg_icon.py` & `apysc-4.4.3/apysc/_display/svg_icon.py`

 * *Files identical despite different names*

### Comparing `apysc-4.4.2/apysc/_display/svg_text.py` & `apysc-4.4.3/apysc/_display/svg_text.py`

 * *Files identical despite different names*

### Comparing `apysc-4.4.2/apysc/_display/svg_text_align_mixin.py` & `apysc-4.4.3/apysc/_display/svg_text_align_mixin.py`

 * *Files identical despite different names*

### Comparing `apysc-4.4.2/apysc/_display/svg_text_bold_mixin.py` & `apysc-4.4.3/apysc/_display/svg_text_bold_mixin.py`

 * *Files identical despite different names*

### Comparing `apysc-4.4.2/apysc/_display/svg_text_delta_x_mixin.py` & `apysc-4.4.3/apysc/_display/svg_text_delta_x_mixin.py`

 * *Files identical despite different names*

### Comparing `apysc-4.4.2/apysc/_display/svg_text_delta_y_mixin.py` & `apysc-4.4.3/apysc/_display/svg_text_delta_y_mixin.py`

 * *Files identical despite different names*

### Comparing `apysc-4.4.2/apysc/_display/svg_text_font_family_mixin.py` & `apysc-4.4.3/apysc/_display/svg_text_font_family_mixin.py`

 * *Files identical despite different names*

### Comparing `apysc-4.4.2/apysc/_display/svg_text_font_size_mixin.py` & `apysc-4.4.3/apysc/_display/svg_text_font_size_mixin.py`

 * *Files identical despite different names*

### Comparing `apysc-4.4.2/apysc/_display/svg_text_italic_mixin.py` & `apysc-4.4.3/apysc/_display/svg_text_italic_mixin.py`

 * *Files identical despite different names*

### Comparing `apysc-4.4.2/apysc/_display/svg_text_leading_mixin.py` & `apysc-4.4.3/apysc/_display/svg_text_leading_mixin.py`

 * *Files identical despite different names*

### Comparing `apysc-4.4.2/apysc/_display/svg_text_set_align_mixin.py` & `apysc-4.4.3/apysc/_display/svg_text_set_align_mixin.py`

 * *Files identical despite different names*

### Comparing `apysc-4.4.2/apysc/_display/svg_text_set_bold_mixin.py` & `apysc-4.4.3/apysc/_display/svg_text_set_bold_mixin.py`

 * *Files identical despite different names*

### Comparing `apysc-4.4.2/apysc/_display/svg_text_set_delta_x_mixin.py` & `apysc-4.4.3/apysc/_display/svg_text_set_delta_x_mixin.py`

 * *Files identical despite different names*

### Comparing `apysc-4.4.2/apysc/_display/svg_text_set_delta_y_mixin.py` & `apysc-4.4.3/apysc/_display/svg_text_set_delta_y_mixin.py`

 * *Files identical despite different names*

### Comparing `apysc-4.4.2/apysc/_display/svg_text_set_font_family_mixin.py` & `apysc-4.4.3/apysc/_display/svg_text_set_font_family_mixin.py`

 * *Files identical despite different names*

### Comparing `apysc-4.4.2/apysc/_display/svg_text_set_font_size_value_mixin.py` & `apysc-4.4.3/apysc/_display/svg_text_set_font_size_value_mixin.py`

 * *Files identical despite different names*

### Comparing `apysc-4.4.2/apysc/_display/svg_text_set_italic_mixin.py` & `apysc-4.4.3/apysc/_display/svg_text_set_italic_mixin.py`

 * *Files identical despite different names*

### Comparing `apysc-4.4.2/apysc/_display/svg_text_set_leading_mixin.py` & `apysc-4.4.3/apysc/_display/svg_text_set_leading_mixin.py`

 * *Files identical despite different names*

### Comparing `apysc-4.4.2/apysc/_display/svg_text_set_text_value_mixin.py` & `apysc-4.4.3/apysc/_display/svg_text_set_text_value_mixin.py`

 * *Files identical despite different names*

### Comparing `apysc-4.4.2/apysc/_display/svg_text_singleton_for_text_span.py` & `apysc-4.4.3/apysc/_display/svg_text_singleton_for_text_span.py`

 * *Files identical despite different names*

### Comparing `apysc-4.4.2/apysc/_display/svg_text_skip_fill_alpha_exp_appending_mixin.py` & `apysc-4.4.3/apysc/_display/svg_text_skip_fill_alpha_exp_appending_mixin.py`

 * *Files identical despite different names*

### Comparing `apysc-4.4.2/apysc/_display/svg_text_skip_fill_color_exp_appending_mixin.py` & `apysc-4.4.3/apysc/_display/svg_text_skip_fill_color_exp_appending_mixin.py`

 * *Files identical despite different names*

### Comparing `apysc-4.4.2/apysc/_display/svg_text_skip_line_alpha_exp_appending_mixin.py` & `apysc-4.4.3/apysc/_display/svg_text_skip_line_alpha_exp_appending_mixin.py`

 * *Files identical despite different names*

### Comparing `apysc-4.4.2/apysc/_display/svg_text_skip_line_color_exp_appending_mixin.py` & `apysc-4.4.3/apysc/_display/svg_text_skip_line_color_exp_appending_mixin.py`

 * *Files identical despite different names*

### Comparing `apysc-4.4.2/apysc/_display/svg_text_skip_line_thickness_exp_appending_mixin.py` & `apysc-4.4.3/apysc/_display/svg_text_skip_line_thickness_exp_appending_mixin.py`

 * *Files identical despite different names*

### Comparing `apysc-4.4.2/apysc/_display/svg_text_span.py` & `apysc-4.4.3/apysc/_display/svg_text_span.py`

 * *Files identical despite different names*

### Comparing `apysc-4.4.2/apysc/_display/svg_text_text_mixin.py` & `apysc-4.4.3/apysc/_display/svg_text_text_mixin.py`

 * *Files identical despite different names*

### Comparing `apysc-4.4.2/apysc/_display/text_align_css_mixin.py` & `apysc-4.4.3/apysc/_display/text_align_css_mixin.py`

 * *Files identical despite different names*

### Comparing `apysc-4.4.2/apysc/_display/text_align_last_css_mixin.py` & `apysc-4.4.3/apysc/_display/text_align_last_css_mixin.py`

 * *Files identical despite different names*

### Comparing `apysc-4.4.2/apysc/_display/text_bold_css_mixin.py` & `apysc-4.4.3/apysc/_display/text_bold_css_mixin.py`

 * *Files identical despite different names*

### Comparing `apysc-4.4.2/apysc/_display/text_decoration_underline_css_mixin.py` & `apysc-4.4.3/apysc/_display/text_decoration_underline_css_mixin.py`

 * *Files identical despite different names*

### Comparing `apysc-4.4.2/apysc/_display/text_fill_color_css_mixin.py` & `apysc-4.4.3/apysc/_display/text_fill_color_css_mixin.py`

 * *Files identical despite different names*

### Comparing `apysc-4.4.2/apysc/_display/text_font_size_css_mixin.py` & `apysc-4.4.3/apysc/_display/text_font_size_css_mixin.py`

 * *Files identical despite different names*

### Comparing `apysc-4.4.2/apysc/_display/text_italic_css_mixin.py` & `apysc-4.4.3/apysc/_display/text_italic_css_mixin.py`

 * *Files identical despite different names*

### Comparing `apysc-4.4.2/apysc/_display/text_line_height_css_mixin.py` & `apysc-4.4.3/apysc/_display/text_line_height_css_mixin.py`

 * *Files identical despite different names*

### Comparing `apysc-4.4.2/apysc/_display/triangle.py` & `apysc-4.4.3/apysc/_display/triangle.py`

 * *Files identical despite different names*

### Comparing `apysc-4.4.2/apysc/_display/visible_mixin.py` & `apysc-4.4.3/apysc/_display/visible_mixin.py`

 * *Files identical despite different names*

### Comparing `apysc-4.4.2/apysc/_display/width_and_height_mixin_for_ellipse.py` & `apysc-4.4.3/apysc/_display/width_and_height_mixin_for_ellipse.py`

 * *Files identical despite different names*

### Comparing `apysc-4.4.2/apysc/_display/width_mixin.py` & `apysc-4.4.3/apysc/_display/width_mixin.py`

 * *Files identical despite different names*

### Comparing `apysc-4.4.2/apysc/_display/x_interface.py` & `apysc-4.4.3/apysc/_display/x_interface.py`

 * *Files identical despite different names*

### Comparing `apysc-4.4.2/apysc/_display/x_mixin.py` & `apysc-4.4.3/apysc/_display/x_mixin.py`

 * *Files identical despite different names*

### Comparing `apysc-4.4.2/apysc/_display/y_interface.py` & `apysc-4.4.3/apysc/_display/y_interface.py`

 * *Files identical despite different names*

### Comparing `apysc-4.4.2/apysc/_display/y_mixin.py` & `apysc-4.4.3/apysc/_display/y_mixin.py`

 * *Files identical despite different names*

### Comparing `apysc-4.4.2/apysc/_event/animation_event.py` & `apysc-4.4.3/apysc/_event/animation_event.py`

 * *Files identical despite different names*

### Comparing `apysc-4.4.2/apysc/_event/click_mixin.py` & `apysc-4.4.3/apysc/_event/click_mixin.py`

 * *Files identical despite different names*

### Comparing `apysc-4.4.2/apysc/_event/custom_event_mixin.py` & `apysc-4.4.3/apysc/_event/custom_event_mixin.py`

 * *Files identical despite different names*

### Comparing `apysc-4.4.2/apysc/_event/document_mouse_wheel_func.py` & `apysc-4.4.3/apysc/_event/document_mouse_wheel_func.py`

 * *Files identical despite different names*

### Comparing `apysc-4.4.2/apysc/_event/double_click_mixin.py` & `apysc-4.4.3/apysc/_event/double_click_mixin.py`

 * *Files identical despite different names*

### Comparing `apysc-4.4.2/apysc/_event/enter_frame_event.py` & `apysc-4.4.3/apysc/_event/enter_frame_event.py`

 * *Files identical despite different names*

### Comparing `apysc-4.4.2/apysc/_event/enter_frame_mixin.py` & `apysc-4.4.3/apysc/_event/enter_frame_mixin.py`

 * *Files identical despite different names*

### Comparing `apysc-4.4.2/apysc/_event/event.py` & `apysc-4.4.3/apysc/_event/event.py`

 * *Files identical despite different names*

### Comparing `apysc-4.4.2/apysc/_event/handler.py` & `apysc-4.4.3/apysc/_event/handler.py`

 * *Files identical despite different names*

### Comparing `apysc-4.4.2/apysc/_event/handler_circular_calling_util.py` & `apysc-4.4.3/apysc/_event/handler_circular_calling_util.py`

 * *Files identical despite different names*

### Comparing `apysc-4.4.2/apysc/_event/mouse_down_mixin.py` & `apysc-4.4.3/apysc/_event/mouse_down_mixin.py`

 * *Files identical despite different names*

### Comparing `apysc-4.4.2/apysc/_event/mouse_event.py` & `apysc-4.4.3/apysc/_event/mouse_event.py`

 * *Files identical despite different names*

### Comparing `apysc-4.4.2/apysc/_event/mouse_event_binding_expression_mixin.py` & `apysc-4.4.3/apysc/_event/mouse_event_binding_expression_mixin.py`

 * *Files identical despite different names*

### Comparing `apysc-4.4.2/apysc/_event/mouse_event_mixins.py` & `apysc-4.4.3/apysc/_event/mouse_event_mixins.py`

 * *Files identical despite different names*

### Comparing `apysc-4.4.2/apysc/_event/mouse_event_unbinding_mixin.py` & `apysc-4.4.3/apysc/_event/mouse_event_unbinding_mixin.py`

 * *Files identical despite different names*

### Comparing `apysc-4.4.2/apysc/_event/mouse_move_mixin.py` & `apysc-4.4.3/apysc/_event/mouse_move_mixin.py`

 * *Files identical despite different names*

### Comparing `apysc-4.4.2/apysc/_event/mouse_out_mixin.py` & `apysc-4.4.3/apysc/_event/mouse_out_mixin.py`

 * *Files identical despite different names*

### Comparing `apysc-4.4.2/apysc/_event/mouse_over_mixin.py` & `apysc-4.4.3/apysc/_event/mouse_over_mixin.py`

 * *Files identical despite different names*

### Comparing `apysc-4.4.2/apysc/_event/mouse_up_mixin.py` & `apysc-4.4.3/apysc/_event/mouse_up_mixin.py`

 * *Files identical despite different names*

### Comparing `apysc-4.4.2/apysc/_event/prevent_default_mixin.py` & `apysc-4.4.3/apysc/_event/prevent_default_mixin.py`

 * *Files identical despite different names*

### Comparing `apysc-4.4.2/apysc/_event/set_handler_data_mixin.py` & `apysc-4.4.3/apysc/_event/set_handler_data_mixin.py`

 * *Files identical despite different names*

### Comparing `apysc-4.4.2/apysc/_event/stop_propagation_mixin.py` & `apysc-4.4.3/apysc/_event/stop_propagation_mixin.py`

 * *Files identical despite different names*

### Comparing `apysc-4.4.2/apysc/_event/timer_event.py` & `apysc-4.4.3/apysc/_event/timer_event.py`

 * *Files identical despite different names*

### Comparing `apysc-4.4.2/apysc/_event/wheel_event.py` & `apysc-4.4.3/apysc/_event/wheel_event.py`

 * *Files identical despite different names*

### Comparing `apysc-4.4.2/apysc/_expression/event_handler_scope.py` & `apysc-4.4.3/apysc/_expression/event_handler_scope.py`

 * *Files identical despite different names*

### Comparing `apysc-4.4.2/apysc/_expression/expression_data_util.py` & `apysc-4.4.3/apysc/_expression/expression_data_util.py`

 * *Files identical despite different names*

### Comparing `apysc-4.4.2/apysc/_expression/expression_variables_util.py` & `apysc-4.4.3/apysc/_expression/expression_variables_util.py`

 * *Files identical despite different names*

### Comparing `apysc-4.4.2/apysc/_expression/indent_num.py` & `apysc-4.4.3/apysc/_expression/indent_num.py`

 * *Files identical despite different names*

### Comparing `apysc-4.4.2/apysc/_expression/js_functions.py` & `apysc-4.4.3/apysc/_expression/js_functions.py`

 * *Files identical despite different names*

### Comparing `apysc-4.4.2/apysc/_expression/last_scope.py` & `apysc-4.4.3/apysc/_expression/last_scope.py`

 * *Files identical despite different names*

### Comparing `apysc-4.4.2/apysc/_expression/var_names.py` & `apysc-4.4.3/apysc/_expression/var_names.py`

 * *Files 1% similar despite different names*

```diff
@@ -63,7 +63,8 @@
 ANIMATION_ROTATION_AROUND_POINT: Final[str] = "animrotardpoint"
 ANIMATION_SCALE_X_FROM_CENTER: Final[str] = "animscalexfromcenter"
 ANIMATION_SCALE_Y_FROM_CENTER: Final[str] = "animscaleyfromcenter"
 ANIMATION_SCALE_X_FROM_POINT: Final[str] = "animscalexfrompoint"
 ANIMATION_SCALE_Y_FROM_POINT: Final[str] = "animscaleyfrompoint"
 ANIMATION_PARALLEL: Final[str] = "animparallel"
 MATCHED: Final[str] = "matched"
+MASK: Final[str] = "mask"
```

### Comparing `apysc-4.4.2/apysc/_file/file_util.py` & `apysc-4.4.3/apysc/_file/file_util.py`

 * *Files identical despite different names*

### Comparing `apysc-4.4.2/apysc/_file/module_util.py` & `apysc-4.4.3/apysc/_file/module_util.py`

 * *Files identical despite different names*

### Comparing `apysc-4.4.2/apysc/_geom/path_bezier_2d.py` & `apysc-4.4.3/apysc/_geom/path_bezier_2d.py`

 * *Files identical despite different names*

### Comparing `apysc-4.4.2/apysc/_geom/path_bezier_2d_continual.py` & `apysc-4.4.3/apysc/_geom/path_bezier_2d_continual.py`

 * *Files identical despite different names*

### Comparing `apysc-4.4.2/apysc/_geom/path_bezier_3d.py` & `apysc-4.4.3/apysc/_geom/path_bezier_3d.py`

 * *Files identical despite different names*

### Comparing `apysc-4.4.2/apysc/_geom/path_bezier_3d_continual.py` & `apysc-4.4.3/apysc/_geom/path_bezier_3d_continual.py`

 * *Files identical despite different names*

### Comparing `apysc-4.4.2/apysc/_geom/path_close.py` & `apysc-4.4.3/apysc/_geom/path_close.py`

 * *Files identical despite different names*

### Comparing `apysc-4.4.2/apysc/_geom/path_control_x1_mixin.py` & `apysc-4.4.3/apysc/_geom/path_control_x1_mixin.py`

 * *Files identical despite different names*

### Comparing `apysc-4.4.2/apysc/_geom/path_control_x2_mixin.py` & `apysc-4.4.3/apysc/_geom/path_control_x2_mixin.py`

 * *Files identical despite different names*

### Comparing `apysc-4.4.2/apysc/_geom/path_control_x_mixin.py` & `apysc-4.4.3/apysc/_geom/path_control_x_mixin.py`

 * *Files identical despite different names*

### Comparing `apysc-4.4.2/apysc/_geom/path_control_y1_mixin.py` & `apysc-4.4.3/apysc/_geom/path_control_y1_mixin.py`

 * *Files identical despite different names*

### Comparing `apysc-4.4.2/apysc/_geom/path_control_y2_mixin.py` & `apysc-4.4.3/apysc/_geom/path_control_y2_mixin.py`

 * *Files identical despite different names*

### Comparing `apysc-4.4.2/apysc/_geom/path_control_y_mixin.py` & `apysc-4.4.3/apysc/_geom/path_control_y_mixin.py`

 * *Files identical despite different names*

### Comparing `apysc-4.4.2/apysc/_geom/path_data.py` & `apysc-4.4.3/apysc/_geom/path_data.py`

 * *Files identical despite different names*

### Comparing `apysc-4.4.2/apysc/_geom/path_data_base.py` & `apysc-4.4.3/apysc/_geom/path_data_base.py`

 * *Files identical despite different names*

### Comparing `apysc-4.4.2/apysc/_geom/path_data_util.py` & `apysc-4.4.3/apysc/_geom/path_data_util.py`

 * *Files identical despite different names*

### Comparing `apysc-4.4.2/apysc/_geom/path_dest_x_mixin.py` & `apysc-4.4.3/apysc/_geom/path_dest_x_mixin.py`

 * *Files identical despite different names*

### Comparing `apysc-4.4.2/apysc/_geom/path_dest_y_mixin.py` & `apysc-4.4.3/apysc/_geom/path_dest_y_mixin.py`

 * *Files identical despite different names*

### Comparing `apysc-4.4.2/apysc/_geom/path_horizontal.py` & `apysc-4.4.3/apysc/_geom/path_horizontal.py`

 * *Files identical despite different names*

### Comparing `apysc-4.4.2/apysc/_geom/path_line_to.py` & `apysc-4.4.3/apysc/_geom/path_line_to.py`

 * *Files identical despite different names*

### Comparing `apysc-4.4.2/apysc/_geom/path_move_to.py` & `apysc-4.4.3/apysc/_geom/path_move_to.py`

 * *Files identical despite different names*

### Comparing `apysc-4.4.2/apysc/_geom/path_vertical.py` & `apysc-4.4.3/apysc/_geom/path_vertical.py`

 * *Files identical despite different names*

### Comparing `apysc-4.4.2/apysc/_geom/path_x_mixin.py` & `apysc-4.4.3/apysc/_geom/path_x_mixin.py`

 * *Files identical despite different names*

### Comparing `apysc-4.4.2/apysc/_geom/path_y_mixin.py` & `apysc-4.4.3/apysc/_geom/path_y_mixin.py`

 * *Files identical despite different names*

### Comparing `apysc-4.4.2/apysc/_geom/point2d.py` & `apysc-4.4.3/apysc/_geom/point2d.py`

 * *Files identical despite different names*

### Comparing `apysc-4.4.2/apysc/_geom/rectangle_geom.py` & `apysc-4.4.3/apysc/_geom/rectangle_geom.py`

 * *Files identical despite different names*

### Comparing `apysc-4.4.2/apysc/_geom/rectangle_geom_bottom_y_mixin.py` & `apysc-4.4.3/apysc/_geom/rectangle_geom_bottom_y_mixin.py`

 * *Files identical despite different names*

### Comparing `apysc-4.4.2/apysc/_geom/rectangle_geom_center_x_mixin.py` & `apysc-4.4.3/apysc/_geom/rectangle_geom_center_x_mixin.py`

 * *Files identical despite different names*

### Comparing `apysc-4.4.2/apysc/_geom/rectangle_geom_center_y_mixin.py` & `apysc-4.4.3/apysc/_geom/rectangle_geom_center_y_mixin.py`

 * *Files identical despite different names*

### Comparing `apysc-4.4.2/apysc/_geom/rectangle_geom_height_mixin.py` & `apysc-4.4.3/apysc/_geom/rectangle_geom_height_mixin.py`

 * *Files identical despite different names*

### Comparing `apysc-4.4.2/apysc/_geom/rectangle_geom_left_x_mixin.py` & `apysc-4.4.3/apysc/_geom/rectangle_geom_left_x_mixin.py`

 * *Files identical despite different names*

### Comparing `apysc-4.4.2/apysc/_geom/rectangle_geom_right_x_mixin.py` & `apysc-4.4.3/apysc/_geom/rectangle_geom_right_x_mixin.py`

 * *Files identical despite different names*

### Comparing `apysc-4.4.2/apysc/_geom/rectangle_geom_top_y_mixin.py` & `apysc-4.4.3/apysc/_geom/rectangle_geom_top_y_mixin.py`

 * *Files identical despite different names*

### Comparing `apysc-4.4.2/apysc/_geom/rectangle_geom_width_mixin.py` & `apysc-4.4.3/apysc/_geom/rectangle_geom_width_mixin.py`

 * *Files identical despite different names*

### Comparing `apysc-4.4.2/apysc/_geom/relative_mixin.py` & `apysc-4.4.3/apysc/_geom/relative_mixin.py`

 * *Files identical despite different names*

### Comparing `apysc-4.4.2/apysc/_html/debug_mode.py` & `apysc-4.4.3/apysc/_html/debug_mode.py`

 * *Files identical despite different names*

### Comparing `apysc-4.4.2/apysc/_html/exporter.py` & `apysc-4.4.3/apysc/_html/exporter.py`

 * *Files identical despite different names*

### Comparing `apysc-4.4.2/apysc/_html/html_util.py` & `apysc-4.4.3/apysc/_html/html_util.py`

 * *Files identical despite different names*

### Comparing `apysc-4.4.2/apysc/_jslib/jquery-3.7.1.slim.min.js` & `apysc-4.4.3/apysc/_jslib/jquery-3.7.1.slim.min.js`

 * *Files identical despite different names*

### Comparing `apysc-4.4.2/apysc/_jslib/jquery.mousewheel-3.1.13.min.js` & `apysc-4.4.3/apysc/_jslib/jquery.mousewheel-3.1.13.min.js`

 * *Files identical despite different names*

### Comparing `apysc-4.4.2/apysc/_jslib/jslib_util.py` & `apysc-4.4.3/apysc/_jslib/jslib_util.py`

 * *Files identical despite different names*

### Comparing `apysc-4.4.2/apysc/_jslib/svg-3.1.2.min.js` & `apysc-4.4.3/apysc/_jslib/svg-3.1.2.min.js`

 * *Files identical despite different names*

### Comparing `apysc-4.4.2/apysc/_jslib/underscore-1.12.0.min.js` & `apysc-4.4.3/apysc/_jslib/underscore-1.12.0.min.js`

 * *Files identical despite different names*

### Comparing `apysc-4.4.2/apysc/_jupyter/jupyter_util.py` & `apysc-4.4.3/apysc/_jupyter/jupyter_util.py`

 * *Files identical despite different names*

### Comparing `apysc-4.4.2/apysc/_lint_and_doc/add_doc_translation_mapping_blank_data.py` & `apysc-4.4.3/apysc/_lint_and_doc/add_doc_translation_mapping_blank_data.py`

 * *Files identical despite different names*

### Comparing `apysc-4.4.2/apysc/_lint_and_doc/conf_common.py` & `apysc-4.4.3/apysc/_lint_and_doc/conf_common.py`

 * *Files identical despite different names*

### Comparing `apysc-4.4.2/apysc/_lint_and_doc/docs_keyword_link_mapping.py` & `apysc-4.4.3/apysc/_lint_and_doc/docs_keyword_link_mapping.py`

 * *Files 0% similar despite different names*

```diff
@@ -233,8 +233,11 @@
     "ap.String": "string",
     "ap.Str": "string",
     "ap.Array": "array",
     "ap.Dictionary": "dictionary",
     "ap.Dictionary": "dictionary",
     "MultiLineText": "multi_line_text",
     "ap.MultiLineText": "multi_line_text",
+    "clamp": "math_clamp",
+    "Math.clamp": "math_clamp",
+    "ap.Math.clamp": "math_clamp",
 }
```

### Comparing `apysc-4.4.2/apysc/_lint_and_doc/docs_lang.py` & `apysc-4.4.3/apysc/_lint_and_doc/docs_lang.py`

 * *Files identical despite different names*

### Comparing `apysc-4.4.2/apysc/_lint_and_doc/docs_toctree_util.py` & `apysc-4.4.3/apysc/_lint_and_doc/docs_toctree_util.py`

 * *Files identical despite different names*

### Comparing `apysc-4.4.2/apysc/_lint_and_doc/docs_translation_converter.py` & `apysc-4.4.3/apysc/_lint_and_doc/docs_translation_converter.py`

 * *Files identical despite different names*

### Comparing `apysc-4.4.2/apysc/_lint_and_doc/docstring_to_markdown_converter.py` & `apysc-4.4.3/apysc/_lint_and_doc/docstring_to_markdown_converter.py`

 * *Files identical despite different names*

### Comparing `apysc-4.4.2/apysc/_lint_and_doc/docstring_util.py` & `apysc-4.4.3/apysc/_lint_and_doc/docstring_util.py`

 * *Files identical despite different names*

### Comparing `apysc-4.4.2/apysc/_lint_and_doc/document_text_split_util.py` & `apysc-4.4.3/apysc/_lint_and_doc/document_text_split_util.py`

 * *Files identical despite different names*

### Comparing `apysc-4.4.2/apysc/_lint_and_doc/document_util.py` & `apysc-4.4.3/apysc/_lint_and_doc/document_util.py`

 * *Files identical despite different names*

### Comparing `apysc-4.4.2/apysc/_lint_and_doc/fixed_translation_mapping/data_model.py` & `apysc-4.4.3/apysc/_lint_and_doc/fixed_translation_mapping/data_model.py`

 * *Files identical despite different names*

### Comparing `apysc-4.4.2/apysc/_lint_and_doc/fixed_translation_mapping/jp.py` & `apysc-4.4.3/apysc/_lint_and_doc/fixed_translation_mapping/jp.py`

 * *Files 0% similar despite different names*

```diff
@@ -4960,9 +4960,33 @@
             key="  - Fill-alpha of the icon.",
             val="  - アイコンの塗りの透明度。",
         ),
         Mapping(
             key="The class implementation for the SVG icon's class.<hr>",
             val="SVGアイコンのためのクラスの実装。<hr>",
         ),
+        Mapping(
+            key="## clamp method API",
+            val="## clamp メソッドのAPI",
+        ),
+        Mapping(
+            key="Sets the value within a specified minimum and maximum range. If the value is less than the minimum, this method returns the minimum value. If the value is greater than the maximum, this method returns the maximum value.<hr>",
+            val="指定された最小値と最大値の範囲内で値を設定します。もし値が最小値未満であればこのメソッドは最小値を返却します。もし値が最大値よりも大きければこのメソッドは最大値を返却します。<hr>",
+        ),
+        Mapping(
+            key="  - Target `Int` or `Number` value.",
+            val="  - 対象の`Int`もしくは`Number`型の値。",
+        ),
+        Mapping(
+            key="  - Minimum value.",
+            val="  - 最小値。",
+        ),
+        Mapping(
+            key="  - Maximum value.",
+            val="  - 最大値。",
+        ),
+        Mapping(
+            key="  - Clamped value.",
+            val="  - 最小値と最大値範囲の反映後の値。",
+        ),
     ]
 )
```

### Comparing `apysc-4.4.2/apysc/_lint_and_doc/lint_and_doc_hash_util.py` & `apysc-4.4.3/apysc/_lint_and_doc/lint_and_doc_hash_util.py`

 * *Files identical despite different names*

### Comparing `apysc-4.4.2/apysc/_lint_and_doc/translation_mapping_utils.py` & `apysc-4.4.3/apysc/_lint_and_doc/translation_mapping_utils.py`

 * *Files identical despite different names*

### Comparing `apysc-4.4.2/apysc/_loop/_continue.py` & `apysc-4.4.3/apysc/_loop/_continue.py`

 * *Files identical despite different names*

### Comparing `apysc-4.4.2/apysc/_loop/_range.py` & `apysc-4.4.3/apysc/_loop/_range.py`

 * *Files identical despite different names*

### Comparing `apysc-4.4.2/apysc/_loop/for_array_indices.py` & `apysc-4.4.3/apysc/_loop/for_array_indices.py`

 * *Files identical despite different names*

### Comparing `apysc-4.4.2/apysc/_loop/for_array_indices_and_values.py` & `apysc-4.4.3/apysc/_loop/for_array_indices_and_values.py`

 * *Files identical despite different names*

### Comparing `apysc-4.4.2/apysc/_loop/for_array_values.py` & `apysc-4.4.3/apysc/_loop/for_array_values.py`

 * *Files identical despite different names*

### Comparing `apysc-4.4.2/apysc/_loop/for_dict_keys.py` & `apysc-4.4.3/apysc/_loop/for_dict_keys.py`

 * *Files identical despite different names*

### Comparing `apysc-4.4.2/apysc/_loop/for_dict_keys_and_values.py` & `apysc-4.4.3/apysc/_loop/for_dict_keys_and_values.py`

 * *Files identical despite different names*

### Comparing `apysc-4.4.2/apysc/_loop/for_dict_values.py` & `apysc-4.4.3/apysc/_loop/for_dict_values.py`

 * *Files identical despite different names*

### Comparing `apysc-4.4.2/apysc/_loop/for_loop_exit_mixin.py` & `apysc-4.4.3/apysc/_loop/for_loop_exit_mixin.py`

 * *Files identical despite different names*

### Comparing `apysc-4.4.2/apysc/_loop/loop_count.py` & `apysc-4.4.3/apysc/_loop/loop_count.py`

 * *Files identical despite different names*

### Comparing `apysc-4.4.2/apysc/_material_design/icon/material_10k_icon.py` & `apysc-4.4.3/apysc/_material_design/icon/material_10k_icon.py`

 * *Files identical despite different names*

### Comparing `apysc-4.4.2/apysc/_material_design/icon/material_1k_icon.py` & `apysc-4.4.3/apysc/_material_design/icon/material_1k_icon.py`

 * *Files identical despite different names*

### Comparing `apysc-4.4.2/apysc/_material_design/icon/material_1k_plus_icon.py` & `apysc-4.4.3/apysc/_material_design/icon/material_1k_plus_icon.py`

 * *Files identical despite different names*

### Comparing `apysc-4.4.2/apysc/_material_design/icon/material_2k_icon.py` & `apysc-4.4.3/apysc/_material_design/icon/material_2k_icon.py`

 * *Files identical despite different names*

### Comparing `apysc-4.4.2/apysc/_material_design/icon/material_2k_plus_icon.py` & `apysc-4.4.3/apysc/_material_design/icon/material_2k_plus_icon.py`

 * *Files identical despite different names*

### Comparing `apysc-4.4.2/apysc/_material_design/icon/material_3d_rotation_icon.py` & `apysc-4.4.3/apysc/_material_design/icon/material_3d_rotation_icon.py`

 * *Files identical despite different names*

### Comparing `apysc-4.4.2/apysc/_material_design/icon/material_3d_rotation_outlined_icon.py` & `apysc-4.4.3/apysc/_material_design/icon/material_3d_rotation_outlined_icon.py`

 * *Files identical despite different names*

### Comparing `apysc-4.4.2/apysc/_material_design/icon/material_3k_icon.py` & `apysc-4.4.3/apysc/_material_design/icon/material_3k_icon.py`

 * *Files identical despite different names*

### Comparing `apysc-4.4.2/apysc/_material_design/icon/material_3k_plus_icon.py` & `apysc-4.4.3/apysc/_material_design/icon/material_3k_plus_icon.py`

 * *Files identical despite different names*

### Comparing `apysc-4.4.2/apysc/_material_design/icon/material_4k_icon.py` & `apysc-4.4.3/apysc/_material_design/icon/material_4k_icon.py`

 * *Files identical despite different names*

### Comparing `apysc-4.4.2/apysc/_material_design/icon/material_4k_outlined_icon.py` & `apysc-4.4.3/apysc/_material_design/icon/material_4k_outlined_icon.py`

 * *Files identical despite different names*

### Comparing `apysc-4.4.2/apysc/_material_design/icon/material_4k_plus_icon.py` & `apysc-4.4.3/apysc/_material_design/icon/material_4k_plus_icon.py`

 * *Files identical despite different names*

### Comparing `apysc-4.4.2/apysc/_material_design/icon/material_5g_icon.py` & `apysc-4.4.3/apysc/_material_design/icon/material_5g_icon.py`

 * *Files identical despite different names*

### Comparing `apysc-4.4.2/apysc/_material_design/icon/material_5g_outlined_icon.py` & `apysc-4.4.3/apysc/_material_design/icon/material_5g_outlined_icon.py`

 * *Files identical despite different names*

### Comparing `apysc-4.4.2/apysc/_material_design/icon/material_5k_icon.py` & `apysc-4.4.3/apysc/_material_design/icon/material_5k_icon.py`

 * *Files identical despite different names*

### Comparing `apysc-4.4.2/apysc/_material_design/icon/material_5k_plus_icon.py` & `apysc-4.4.3/apysc/_material_design/icon/material_5k_plus_icon.py`

 * *Files identical despite different names*

### Comparing `apysc-4.4.2/apysc/_material_design/icon/material_6k_icon.py` & `apysc-4.4.3/apysc/_material_design/icon/material_6k_icon.py`

 * *Files identical despite different names*

### Comparing `apysc-4.4.2/apysc/_material_design/icon/material_6k_plus_icon.py` & `apysc-4.4.3/apysc/_material_design/icon/material_6k_plus_icon.py`

 * *Files identical despite different names*

### Comparing `apysc-4.4.2/apysc/_material_design/icon/material_7k_icon.py` & `apysc-4.4.3/apysc/_material_design/icon/material_7k_icon.py`

 * *Files identical despite different names*

### Comparing `apysc-4.4.2/apysc/_material_design/icon/material_7k_plus_icon.py` & `apysc-4.4.3/apysc/_material_design/icon/material_7k_plus_icon.py`

 * *Files identical despite different names*

### Comparing `apysc-4.4.2/apysc/_material_design/icon/material_8k_icon.py` & `apysc-4.4.3/apysc/_material_design/icon/material_8k_icon.py`

 * *Files identical despite different names*

### Comparing `apysc-4.4.2/apysc/_material_design/icon/material_8k_plus_icon.py` & `apysc-4.4.3/apysc/_material_design/icon/material_8k_plus_icon.py`

 * *Files identical despite different names*

### Comparing `apysc-4.4.2/apysc/_material_design/icon/material_9k_icon.py` & `apysc-4.4.3/apysc/_material_design/icon/material_9k_icon.py`

 * *Files identical despite different names*

### Comparing `apysc-4.4.2/apysc/_material_design/icon/material_9k_plus_icon.py` & `apysc-4.4.3/apysc/_material_design/icon/material_9k_plus_icon.py`

 * *Files identical despite different names*

### Comparing `apysc-4.4.2/apysc/_material_design/icon/material_accessibility_icon.py` & `apysc-4.4.3/apysc/_material_design/icon/material_accessibility_icon.py`

 * *Files identical despite different names*

### Comparing `apysc-4.4.2/apysc/_material_design/icon/material_accessibility_new_icon.py` & `apysc-4.4.3/apysc/_material_design/icon/material_accessibility_new_icon.py`

 * *Files identical despite different names*

### Comparing `apysc-4.4.2/apysc/_material_design/icon/material_accessibility_new_outlined_icon.py` & `apysc-4.4.3/apysc/_material_design/icon/material_accessibility_new_outlined_icon.py`

 * *Files identical despite different names*

### Comparing `apysc-4.4.2/apysc/_material_design/icon/material_accessibility_outlined_icon.py` & `apysc-4.4.3/apysc/_material_design/icon/material_accessibility_outlined_icon.py`

 * *Files identical despite different names*

### Comparing `apysc-4.4.2/apysc/_material_design/icon/material_accessible_forward_icon.py` & `apysc-4.4.3/apysc/_material_design/icon/material_accessible_forward_icon.py`

 * *Files identical despite different names*

### Comparing `apysc-4.4.2/apysc/_material_design/icon/material_accessible_forward_outlined_icon.py` & `apysc-4.4.3/apysc/_material_design/icon/material_accessible_forward_outlined_icon.py`

 * *Files identical despite different names*

### Comparing `apysc-4.4.2/apysc/_material_design/icon/material_accessible_icon.py` & `apysc-4.4.3/apysc/_material_design/icon/material_accessible_icon.py`

 * *Files identical despite different names*

### Comparing `apysc-4.4.2/apysc/_material_design/icon/material_accessible_outlined_icon.py` & `apysc-4.4.3/apysc/_material_design/icon/material_accessible_outlined_icon.py`

 * *Files identical despite different names*

### Comparing `apysc-4.4.2/apysc/_material_design/icon/material_account_balance_icon.py` & `apysc-4.4.3/apysc/_material_design/icon/material_account_balance_icon.py`

 * *Files identical despite different names*

### Comparing `apysc-4.4.2/apysc/_material_design/icon/material_account_balance_outlined_icon.py` & `apysc-4.4.3/apysc/_material_design/icon/material_account_balance_outlined_icon.py`

 * *Files identical despite different names*

### Comparing `apysc-4.4.2/apysc/_material_design/icon/material_account_balance_wallet_icon.py` & `apysc-4.4.3/apysc/_material_design/icon/material_account_balance_wallet_icon.py`

 * *Files identical despite different names*

### Comparing `apysc-4.4.2/apysc/_material_design/icon/material_account_balance_wallet_outlined_icon.py` & `apysc-4.4.3/apysc/_material_design/icon/material_account_balance_wallet_outlined_icon.py`

 * *Files identical despite different names*

### Comparing `apysc-4.4.2/apysc/_material_design/icon/material_account_box_icon.py` & `apysc-4.4.3/apysc/_material_design/icon/material_account_box_icon.py`

 * *Files identical despite different names*

### Comparing `apysc-4.4.2/apysc/_material_design/icon/material_account_box_outlined_icon.py` & `apysc-4.4.3/apysc/_material_design/icon/material_account_box_outlined_icon.py`

 * *Files identical despite different names*

### Comparing `apysc-4.4.2/apysc/_material_design/icon/material_account_circle_icon.py` & `apysc-4.4.3/apysc/_material_design/icon/material_account_circle_icon.py`

 * *Files identical despite different names*

### Comparing `apysc-4.4.2/apysc/_material_design/icon/material_account_circle_outlined_icon.py` & `apysc-4.4.3/apysc/_material_design/icon/material_account_circle_outlined_icon.py`

 * *Files identical despite different names*

### Comparing `apysc-4.4.2/apysc/_material_design/icon/material_add_alert_icon.py` & `apysc-4.4.3/apysc/_material_design/icon/material_add_alert_icon.py`

 * *Files identical despite different names*

### Comparing `apysc-4.4.2/apysc/_material_design/icon/material_add_alert_outlined_icon.py` & `apysc-4.4.3/apysc/_material_design/icon/material_add_alert_outlined_icon.py`

 * *Files identical despite different names*

### Comparing `apysc-4.4.2/apysc/_material_design/icon/material_add_box_icon.py` & `apysc-4.4.3/apysc/_material_design/icon/material_add_box_icon.py`

 * *Files identical despite different names*

### Comparing `apysc-4.4.2/apysc/_material_design/icon/material_add_box_outlined_icon.py` & `apysc-4.4.3/apysc/_material_design/icon/material_add_box_outlined_icon.py`

 * *Files identical despite different names*

### Comparing `apysc-4.4.2/apysc/_material_design/icon/material_add_circle_icon.py` & `apysc-4.4.3/apysc/_material_design/icon/material_add_circle_icon.py`

 * *Files identical despite different names*

### Comparing `apysc-4.4.2/apysc/_material_design/icon/material_add_circle_outline_icon.py` & `apysc-4.4.3/apysc/_material_design/icon/material_add_circle_outline_icon.py`

 * *Files identical despite different names*

### Comparing `apysc-4.4.2/apysc/_material_design/icon/material_add_circle_outline_outlined_icon.py` & `apysc-4.4.3/apysc/_material_design/icon/material_add_circle_outline_outlined_icon.py`

 * *Files identical despite different names*

### Comparing `apysc-4.4.2/apysc/_material_design/icon/material_add_circle_outlined_icon.py` & `apysc-4.4.3/apysc/_material_design/icon/material_add_circle_outlined_icon.py`

 * *Files identical despite different names*

### Comparing `apysc-4.4.2/apysc/_material_design/icon/material_add_ic_call_icon.py` & `apysc-4.4.3/apysc/_material_design/icon/material_add_ic_call_icon.py`

 * *Files identical despite different names*

### Comparing `apysc-4.4.2/apysc/_material_design/icon/material_add_ic_call_outlined_icon.py` & `apysc-4.4.3/apysc/_material_design/icon/material_add_ic_call_outlined_icon.py`

 * *Files identical despite different names*

### Comparing `apysc-4.4.2/apysc/_material_design/icon/material_add_icon.py` & `apysc-4.4.3/apysc/_material_design/icon/material_add_icon.py`

 * *Files identical despite different names*

### Comparing `apysc-4.4.2/apysc/_material_design/icon/material_add_link_icon.py` & `apysc-4.4.3/apysc/_material_design/icon/material_add_link_icon.py`

 * *Files identical despite different names*

### Comparing `apysc-4.4.2/apysc/_material_design/icon/material_add_outlined_icon.py` & `apysc-4.4.3/apysc/_material_design/icon/material_add_outlined_icon.py`

 * *Files identical despite different names*

### Comparing `apysc-4.4.2/apysc/_material_design/icon/material_add_shopping_cart_icon.py` & `apysc-4.4.3/apysc/_material_design/icon/material_add_shopping_cart_icon.py`

 * *Files identical despite different names*

### Comparing `apysc-4.4.2/apysc/_material_design/icon/material_add_shopping_cart_outlined_icon.py` & `apysc-4.4.3/apysc/_material_design/icon/material_add_shopping_cart_outlined_icon.py`

 * *Files identical despite different names*

### Comparing `apysc-4.4.2/apysc/_material_design/icon/material_add_task_icon.py` & `apysc-4.4.3/apysc/_material_design/icon/material_add_task_icon.py`

 * *Files identical despite different names*

### Comparing `apysc-4.4.2/apysc/_material_design/icon/material_add_task_outlined_icon.py` & `apysc-4.4.3/apysc/_material_design/icon/material_add_task_outlined_icon.py`

 * *Files identical despite different names*

### Comparing `apysc-4.4.2/apysc/_material_design/icon/material_add_to_drive_icon.py` & `apysc-4.4.3/apysc/_material_design/icon/material_add_to_drive_icon.py`

 * *Files identical despite different names*

### Comparing `apysc-4.4.2/apysc/_material_design/icon/material_add_to_queue_icon.py` & `apysc-4.4.3/apysc/_material_design/icon/material_add_to_queue_icon.py`

 * *Files identical despite different names*

### Comparing `apysc-4.4.2/apysc/_material_design/icon/material_add_to_queue_outlined_icon.py` & `apysc-4.4.3/apysc/_material_design/icon/material_add_to_queue_outlined_icon.py`

 * *Files identical despite different names*

### Comparing `apysc-4.4.2/apysc/_material_design/icon/material_addchart_icon.py` & `apysc-4.4.3/apysc/_material_design/icon/material_addchart_icon.py`

 * *Files identical despite different names*

### Comparing `apysc-4.4.2/apysc/_material_design/icon/material_addchart_outlined_icon.py` & `apysc-4.4.3/apysc/_material_design/icon/material_addchart_outlined_icon.py`

 * *Files identical despite different names*

### Comparing `apysc-4.4.2/apysc/_material_design/icon/material_admin_panel_settings_icon.py` & `apysc-4.4.3/apysc/_material_design/icon/material_admin_panel_settings_icon.py`

 * *Files identical despite different names*

### Comparing `apysc-4.4.2/apysc/_material_design/icon/material_admin_panel_settings_outlined_icon.py` & `apysc-4.4.3/apysc/_material_design/icon/material_admin_panel_settings_outlined_icon.py`

 * *Files identical despite different names*

### Comparing `apysc-4.4.2/apysc/_material_design/icon/material_airplay_icon.py` & `apysc-4.4.3/apysc/_material_design/icon/material_airplay_icon.py`

 * *Files identical despite different names*

### Comparing `apysc-4.4.2/apysc/_material_design/icon/material_airplay_outlined_icon.py` & `apysc-4.4.3/apysc/_material_design/icon/material_airplay_outlined_icon.py`

 * *Files identical despite different names*

### Comparing `apysc-4.4.2/apysc/_material_design/icon/material_alarm_add_icon.py` & `apysc-4.4.3/apysc/_material_design/icon/material_alarm_add_icon.py`

 * *Files identical despite different names*

### Comparing `apysc-4.4.2/apysc/_material_design/icon/material_alarm_add_outlined_icon.py` & `apysc-4.4.3/apysc/_material_design/icon/material_alarm_add_outlined_icon.py`

 * *Files identical despite different names*

### Comparing `apysc-4.4.2/apysc/_material_design/icon/material_alarm_icon.py` & `apysc-4.4.3/apysc/_material_design/icon/material_alarm_icon.py`

 * *Files identical despite different names*

### Comparing `apysc-4.4.2/apysc/_material_design/icon/material_alarm_off_icon.py` & `apysc-4.4.3/apysc/_material_design/icon/material_alarm_off_icon.py`

 * *Files identical despite different names*

### Comparing `apysc-4.4.2/apysc/_material_design/icon/material_alarm_off_outlined_icon.py` & `apysc-4.4.3/apysc/_material_design/icon/material_alarm_off_outlined_icon.py`

 * *Files identical despite different names*

### Comparing `apysc-4.4.2/apysc/_material_design/icon/material_alarm_on_icon.py` & `apysc-4.4.3/apysc/_material_design/icon/material_alarm_on_icon.py`

 * *Files identical despite different names*

### Comparing `apysc-4.4.2/apysc/_material_design/icon/material_alarm_on_outlined_icon.py` & `apysc-4.4.3/apysc/_material_design/icon/material_alarm_on_outlined_icon.py`

 * *Files identical despite different names*

### Comparing `apysc-4.4.2/apysc/_material_design/icon/material_alarm_outlined_icon.py` & `apysc-4.4.3/apysc/_material_design/icon/material_alarm_outlined_icon.py`

 * *Files identical despite different names*

### Comparing `apysc-4.4.2/apysc/_material_design/icon/material_album_icon.py` & `apysc-4.4.3/apysc/_material_design/icon/material_album_icon.py`

 * *Files identical despite different names*

### Comparing `apysc-4.4.2/apysc/_material_design/icon/material_album_outlined_icon.py` & `apysc-4.4.3/apysc/_material_design/icon/material_album_outlined_icon.py`

 * *Files identical despite different names*

### Comparing `apysc-4.4.2/apysc/_material_design/icon/material_all_inbox_icon.py` & `apysc-4.4.3/apysc/_material_design/icon/material_all_inbox_icon.py`

 * *Files identical despite different names*

### Comparing `apysc-4.4.2/apysc/_material_design/icon/material_all_inbox_outlined_icon.py` & `apysc-4.4.3/apysc/_material_design/icon/material_all_inbox_outlined_icon.py`

 * *Files identical despite different names*

### Comparing `apysc-4.4.2/apysc/_material_design/icon/material_all_out_icon.py` & `apysc-4.4.3/apysc/_material_design/icon/material_all_out_icon.py`

 * *Files identical despite different names*

### Comparing `apysc-4.4.2/apysc/_material_design/icon/material_all_out_outlined_icon.py` & `apysc-4.4.3/apysc/_material_design/icon/material_all_out_outlined_icon.py`

 * *Files identical despite different names*

### Comparing `apysc-4.4.2/apysc/_material_design/icon/material_alternate_email_icon.py` & `apysc-4.4.3/apysc/_material_design/icon/material_alternate_email_icon.py`

 * *Files identical despite different names*

### Comparing `apysc-4.4.2/apysc/_material_design/icon/material_alternate_email_outlined_icon.py` & `apysc-4.4.3/apysc/_material_design/icon/material_alternate_email_outlined_icon.py`

 * *Files identical despite different names*

### Comparing `apysc-4.4.2/apysc/_material_design/icon/material_amp_stories_icon.py` & `apysc-4.4.3/apysc/_material_design/icon/material_amp_stories_icon.py`

 * *Files identical despite different names*

### Comparing `apysc-4.4.2/apysc/_material_design/icon/material_amp_stories_outlined_icon.py` & `apysc-4.4.3/apysc/_material_design/icon/material_amp_stories_outlined_icon.py`

 * *Files identical despite different names*

### Comparing `apysc-4.4.2/apysc/_material_design/icon/material_analytics_icon.py` & `apysc-4.4.3/apysc/_material_design/icon/material_analytics_icon.py`

 * *Files identical despite different names*

### Comparing `apysc-4.4.2/apysc/_material_design/icon/material_analytics_outlined_icon.py` & `apysc-4.4.3/apysc/_material_design/icon/material_analytics_outlined_icon.py`

 * *Files identical despite different names*

### Comparing `apysc-4.4.2/apysc/_material_design/icon/material_anchor_icon.py` & `apysc-4.4.3/apysc/_material_design/icon/material_anchor_icon.py`

 * *Files identical despite different names*

### Comparing `apysc-4.4.2/apysc/_material_design/icon/material_anchor_outlined_icon.py` & `apysc-4.4.3/apysc/_material_design/icon/material_anchor_outlined_icon.py`

 * *Files identical despite different names*

### Comparing `apysc-4.4.2/apysc/_material_design/icon/material_android_icon.py` & `apysc-4.4.3/apysc/_material_design/icon/material_android_icon.py`

 * *Files identical despite different names*

### Comparing `apysc-4.4.2/apysc/_material_design/icon/material_android_outlined_icon.py` & `apysc-4.4.3/apysc/_material_design/icon/material_android_outlined_icon.py`

 * *Files identical despite different names*

### Comparing `apysc-4.4.2/apysc/_material_design/icon/material_announcement_icon.py` & `apysc-4.4.3/apysc/_material_design/icon/material_announcement_icon.py`

 * *Files identical despite different names*

### Comparing `apysc-4.4.2/apysc/_material_design/icon/material_announcement_outlined_icon.py` & `apysc-4.4.3/apysc/_material_design/icon/material_announcement_outlined_icon.py`

 * *Files identical despite different names*

### Comparing `apysc-4.4.2/apysc/_material_design/icon/material_api_icon.py` & `apysc-4.4.3/apysc/_material_design/icon/material_api_icon.py`

 * *Files identical despite different names*

### Comparing `apysc-4.4.2/apysc/_material_design/icon/material_api_outlined_icon.py` & `apysc-4.4.3/apysc/_material_design/icon/material_api_outlined_icon.py`

 * *Files identical despite different names*

### Comparing `apysc-4.4.2/apysc/_material_design/icon/material_app_blocking_icon.py` & `apysc-4.4.3/apysc/_material_design/icon/material_app_blocking_icon.py`

 * *Files identical despite different names*

### Comparing `apysc-4.4.2/apysc/_material_design/icon/material_app_blocking_outlined_icon.py` & `apysc-4.4.3/apysc/_material_design/icon/material_app_blocking_outlined_icon.py`

 * *Files identical despite different names*

### Comparing `apysc-4.4.2/apysc/_material_design/icon/material_app_registration_icon.py` & `apysc-4.4.3/apysc/_material_design/icon/material_app_registration_icon.py`

 * *Files identical despite different names*

### Comparing `apysc-4.4.2/apysc/_material_design/icon/material_archive_icon.py` & `apysc-4.4.3/apysc/_material_design/icon/material_archive_icon.py`

 * *Files identical despite different names*

### Comparing `apysc-4.4.2/apysc/_material_design/icon/material_archive_outlined_icon.py` & `apysc-4.4.3/apysc/_material_design/icon/material_archive_outlined_icon.py`

 * *Files identical despite different names*

### Comparing `apysc-4.4.2/apysc/_material_design/icon/material_arrow_circle_down_icon.py` & `apysc-4.4.3/apysc/_material_design/icon/material_arrow_circle_down_icon.py`

 * *Files identical despite different names*

### Comparing `apysc-4.4.2/apysc/_material_design/icon/material_arrow_circle_down_outlined_icon.py` & `apysc-4.4.3/apysc/_material_design/icon/material_arrow_circle_down_outlined_icon.py`

 * *Files identical despite different names*

### Comparing `apysc-4.4.2/apysc/_material_design/icon/material_arrow_circle_up_icon.py` & `apysc-4.4.3/apysc/_material_design/icon/material_arrow_circle_up_icon.py`

 * *Files identical despite different names*

### Comparing `apysc-4.4.2/apysc/_material_design/icon/material_arrow_circle_up_outlined_icon.py` & `apysc-4.4.3/apysc/_material_design/icon/material_arrow_circle_up_outlined_icon.py`

 * *Files identical despite different names*

### Comparing `apysc-4.4.2/apysc/_material_design/icon/material_arrow_right_alt_icon.py` & `apysc-4.4.3/apysc/_material_design/icon/material_arrow_right_alt_icon.py`

 * *Files identical despite different names*

### Comparing `apysc-4.4.2/apysc/_material_design/icon/material_arrow_right_alt_outlined_icon.py` & `apysc-4.4.3/apysc/_material_design/icon/material_arrow_right_alt_outlined_icon.py`

 * *Files identical despite different names*

### Comparing `apysc-4.4.2/apysc/_material_design/icon/material_art_track_icon.py` & `apysc-4.4.3/apysc/_material_design/icon/material_art_track_icon.py`

 * *Files identical despite different names*

### Comparing `apysc-4.4.2/apysc/_material_design/icon/material_art_track_outlined_icon.py` & `apysc-4.4.3/apysc/_material_design/icon/material_art_track_outlined_icon.py`

 * *Files identical despite different names*

### Comparing `apysc-4.4.2/apysc/_material_design/icon/material_article_icon.py` & `apysc-4.4.3/apysc/_material_design/icon/material_article_icon.py`

 * *Files identical despite different names*

### Comparing `apysc-4.4.2/apysc/_material_design/icon/material_article_outlined_icon.py` & `apysc-4.4.3/apysc/_material_design/icon/material_article_outlined_icon.py`

 * *Files identical despite different names*

### Comparing `apysc-4.4.2/apysc/_material_design/icon/material_aspect_ratio_icon.py` & `apysc-4.4.3/apysc/_material_design/icon/material_aspect_ratio_icon.py`

 * *Files identical despite different names*

### Comparing `apysc-4.4.2/apysc/_material_design/icon/material_aspect_ratio_outlined_icon.py` & `apysc-4.4.3/apysc/_material_design/icon/material_aspect_ratio_outlined_icon.py`

 * *Files identical despite different names*

### Comparing `apysc-4.4.2/apysc/_material_design/icon/material_assessment_icon.py` & `apysc-4.4.3/apysc/_material_design/icon/material_assessment_icon.py`

 * *Files identical despite different names*

### Comparing `apysc-4.4.2/apysc/_material_design/icon/material_assessment_outlined_icon.py` & `apysc-4.4.3/apysc/_material_design/icon/material_assessment_outlined_icon.py`

 * *Files identical despite different names*

### Comparing `apysc-4.4.2/apysc/_material_design/icon/material_assignment_icon.py` & `apysc-4.4.3/apysc/_material_design/icon/material_assignment_icon.py`

 * *Files identical despite different names*

### Comparing `apysc-4.4.2/apysc/_material_design/icon/material_assignment_ind_icon.py` & `apysc-4.4.3/apysc/_material_design/icon/material_assignment_ind_icon.py`

 * *Files identical despite different names*

### Comparing `apysc-4.4.2/apysc/_material_design/icon/material_assignment_ind_outlined_icon.py` & `apysc-4.4.3/apysc/_material_design/icon/material_assignment_ind_outlined_icon.py`

 * *Files identical despite different names*

### Comparing `apysc-4.4.2/apysc/_material_design/icon/material_assignment_late_icon.py` & `apysc-4.4.3/apysc/_material_design/icon/material_assignment_late_icon.py`

 * *Files identical despite different names*

### Comparing `apysc-4.4.2/apysc/_material_design/icon/material_assignment_late_outlined_icon.py` & `apysc-4.4.3/apysc/_material_design/icon/material_assignment_late_outlined_icon.py`

 * *Files identical despite different names*

### Comparing `apysc-4.4.2/apysc/_material_design/icon/material_assignment_outlined_icon.py` & `apysc-4.4.3/apysc/_material_design/icon/material_assignment_outlined_icon.py`

 * *Files identical despite different names*

### Comparing `apysc-4.4.2/apysc/_material_design/icon/material_assignment_return_icon.py` & `apysc-4.4.3/apysc/_material_design/icon/material_assignment_return_icon.py`

 * *Files identical despite different names*

### Comparing `apysc-4.4.2/apysc/_material_design/icon/material_assignment_return_outlined_icon.py` & `apysc-4.4.3/apysc/_material_design/icon/material_assignment_return_outlined_icon.py`

 * *Files identical despite different names*

### Comparing `apysc-4.4.2/apysc/_material_design/icon/material_assignment_returned_icon.py` & `apysc-4.4.3/apysc/_material_design/icon/material_assignment_returned_icon.py`

 * *Files identical despite different names*

### Comparing `apysc-4.4.2/apysc/_material_design/icon/material_assignment_returned_outlined_icon.py` & `apysc-4.4.3/apysc/_material_design/icon/material_assignment_returned_outlined_icon.py`

 * *Files identical despite different names*

### Comparing `apysc-4.4.2/apysc/_material_design/icon/material_assignment_turned_in_icon.py` & `apysc-4.4.3/apysc/_material_design/icon/material_assignment_turned_in_icon.py`

 * *Files identical despite different names*

### Comparing `apysc-4.4.2/apysc/_material_design/icon/material_assignment_turned_in_outlined_icon.py` & `apysc-4.4.3/apysc/_material_design/icon/material_assignment_turned_in_outlined_icon.py`

 * *Files identical despite different names*

### Comparing `apysc-4.4.2/apysc/_material_design/icon/material_attribution_outlined_icon.py` & `apysc-4.4.3/apysc/_material_design/icon/material_attribution_outlined_icon.py`

 * *Files identical despite different names*

### Comparing `apysc-4.4.2/apysc/_material_design/icon/material_auto_delete_icon.py` & `apysc-4.4.3/apysc/_material_design/icon/material_auto_delete_icon.py`

 * *Files identical despite different names*

### Comparing `apysc-4.4.2/apysc/_material_design/icon/material_auto_delete_outlined_icon.py` & `apysc-4.4.3/apysc/_material_design/icon/material_auto_delete_outlined_icon.py`

 * *Files identical despite different names*

### Comparing `apysc-4.4.2/apysc/_material_design/icon/material_autorenew_icon.py` & `apysc-4.4.3/apysc/_material_design/icon/material_autorenew_icon.py`

 * *Files identical despite different names*

### Comparing `apysc-4.4.2/apysc/_material_design/icon/material_autorenew_outlined_icon.py` & `apysc-4.4.3/apysc/_material_design/icon/material_autorenew_outlined_icon.py`

 * *Files identical despite different names*

### Comparing `apysc-4.4.2/apysc/_material_design/icon/material_av_timer_icon.py` & `apysc-4.4.3/apysc/_material_design/icon/material_av_timer_icon.py`

 * *Files identical despite different names*

### Comparing `apysc-4.4.2/apysc/_material_design/icon/material_av_timer_outlined_icon.py` & `apysc-4.4.3/apysc/_material_design/icon/material_av_timer_outlined_icon.py`

 * *Files identical despite different names*

### Comparing `apysc-4.4.2/apysc/_material_design/icon/material_backspace_icon.py` & `apysc-4.4.3/apysc/_material_design/icon/material_backspace_icon.py`

 * *Files identical despite different names*

### Comparing `apysc-4.4.2/apysc/_material_design/icon/material_backspace_outlined_icon.py` & `apysc-4.4.3/apysc/_material_design/icon/material_backspace_outlined_icon.py`

 * *Files identical despite different names*

### Comparing `apysc-4.4.2/apysc/_material_design/icon/material_backup_icon.py` & `apysc-4.4.3/apysc/_material_design/icon/material_backup_icon.py`

 * *Files identical despite different names*

### Comparing `apysc-4.4.2/apysc/_material_design/icon/material_backup_outlined_icon.py` & `apysc-4.4.3/apysc/_material_design/icon/material_backup_outlined_icon.py`

 * *Files identical despite different names*

### Comparing `apysc-4.4.2/apysc/_material_design/icon/material_backup_table_icon.py` & `apysc-4.4.3/apysc/_material_design/icon/material_backup_table_icon.py`

 * *Files identical despite different names*

### Comparing `apysc-4.4.2/apysc/_material_design/icon/material_backup_table_outlined_icon.py` & `apysc-4.4.3/apysc/_material_design/icon/material_backup_table_outlined_icon.py`

 * *Files identical despite different names*

### Comparing `apysc-4.4.2/apysc/_material_design/icon/material_ballot_icon.py` & `apysc-4.4.3/apysc/_material_design/icon/material_ballot_icon.py`

 * *Files identical despite different names*

### Comparing `apysc-4.4.2/apysc/_material_design/icon/material_ballot_outlined_icon.py` & `apysc-4.4.3/apysc/_material_design/icon/material_ballot_outlined_icon.py`

 * *Files identical despite different names*

### Comparing `apysc-4.4.2/apysc/_material_design/icon/material_batch_prediction_icon.py` & `apysc-4.4.3/apysc/_material_design/icon/material_batch_prediction_icon.py`

 * *Files identical despite different names*

### Comparing `apysc-4.4.2/apysc/_material_design/icon/material_batch_prediction_outlined_icon.py` & `apysc-4.4.3/apysc/_material_design/icon/material_batch_prediction_outlined_icon.py`

 * *Files identical despite different names*

### Comparing `apysc-4.4.2/apysc/_material_design/icon/material_biotech_icon.py` & `apysc-4.4.3/apysc/_material_design/icon/material_biotech_icon.py`

 * *Files identical despite different names*

### Comparing `apysc-4.4.2/apysc/_material_design/icon/material_biotech_outlined_icon.py` & `apysc-4.4.3/apysc/_material_design/icon/material_biotech_outlined_icon.py`

 * *Files identical despite different names*

### Comparing `apysc-4.4.2/apysc/_material_design/icon/material_block_flipped_icon.py` & `apysc-4.4.3/apysc/_material_design/icon/material_block_flipped_icon.py`

 * *Files identical despite different names*

### Comparing `apysc-4.4.2/apysc/_material_design/icon/material_block_icon.py` & `apysc-4.4.3/apysc/_material_design/icon/material_block_icon.py`

 * *Files identical despite different names*

### Comparing `apysc-4.4.2/apysc/_material_design/icon/material_block_outlined_icon.py` & `apysc-4.4.3/apysc/_material_design/icon/material_block_outlined_icon.py`

 * *Files identical despite different names*

### Comparing `apysc-4.4.2/apysc/_material_design/icon/material_bolt_icon.py` & `apysc-4.4.3/apysc/_material_design/icon/material_bolt_icon.py`

 * *Files identical despite different names*

### Comparing `apysc-4.4.2/apysc/_material_design/icon/material_book_icon.py` & `apysc-4.4.3/apysc/_material_design/icon/material_book_icon.py`

 * *Files identical despite different names*

### Comparing `apysc-4.4.2/apysc/_material_design/icon/material_book_online_icon.py` & `apysc-4.4.3/apysc/_material_design/icon/material_book_online_icon.py`

 * *Files identical despite different names*

### Comparing `apysc-4.4.2/apysc/_material_design/icon/material_book_online_outlined_icon.py` & `apysc-4.4.3/apysc/_material_design/icon/material_book_online_outlined_icon.py`

 * *Files identical despite different names*

### Comparing `apysc-4.4.2/apysc/_material_design/icon/material_book_outlined_icon.py` & `apysc-4.4.3/apysc/_material_design/icon/material_book_outlined_icon.py`

 * *Files identical despite different names*

### Comparing `apysc-4.4.2/apysc/_material_design/icon/material_bookmark_border_icon.py` & `apysc-4.4.3/apysc/_material_design/icon/material_bookmark_border_icon.py`

 * *Files identical despite different names*

### Comparing `apysc-4.4.2/apysc/_material_design/icon/material_bookmark_border_outlined_icon.py` & `apysc-4.4.3/apysc/_material_design/icon/material_bookmark_border_outlined_icon.py`

 * *Files identical despite different names*

### Comparing `apysc-4.4.2/apysc/_material_design/icon/material_bookmark_icon.py` & `apysc-4.4.3/apysc/_material_design/icon/material_bookmark_icon.py`

 * *Files identical despite different names*

### Comparing `apysc-4.4.2/apysc/_material_design/icon/material_bookmark_outlined_icon.py` & `apysc-4.4.3/apysc/_material_design/icon/material_bookmark_outlined_icon.py`

 * *Files identical despite different names*

### Comparing `apysc-4.4.2/apysc/_material_design/icon/material_bookmarks_icon.py` & `apysc-4.4.3/apysc/_material_design/icon/material_bookmarks_icon.py`

 * *Files identical despite different names*

### Comparing `apysc-4.4.2/apysc/_material_design/icon/material_bookmarks_outlined_icon.py` & `apysc-4.4.3/apysc/_material_design/icon/material_bookmarks_outlined_icon.py`

 * *Files identical despite different names*

### Comparing `apysc-4.4.2/apysc/_material_design/icon/material_branding_watermark_icon.py` & `apysc-4.4.3/apysc/_material_design/icon/material_branding_watermark_icon.py`

 * *Files identical despite different names*

### Comparing `apysc-4.4.2/apysc/_material_design/icon/material_branding_watermark_outlined_icon.py` & `apysc-4.4.3/apysc/_material_design/icon/material_branding_watermark_outlined_icon.py`

 * *Files identical despite different names*

### Comparing `apysc-4.4.2/apysc/_material_design/icon/material_bug_report_icon.py` & `apysc-4.4.3/apysc/_material_design/icon/material_bug_report_icon.py`

 * *Files identical despite different names*

### Comparing `apysc-4.4.2/apysc/_material_design/icon/material_bug_report_outlined_icon.py` & `apysc-4.4.3/apysc/_material_design/icon/material_bug_report_outlined_icon.py`

 * *Files identical despite different names*

### Comparing `apysc-4.4.2/apysc/_material_design/icon/material_build_circle_icon.py` & `apysc-4.4.3/apysc/_material_design/icon/material_build_circle_icon.py`

 * *Files identical despite different names*

### Comparing `apysc-4.4.2/apysc/_material_design/icon/material_build_circle_outlined_icon.py` & `apysc-4.4.3/apysc/_material_design/icon/material_build_circle_outlined_icon.py`

 * *Files identical despite different names*

### Comparing `apysc-4.4.2/apysc/_material_design/icon/material_build_icon.py` & `apysc-4.4.3/apysc/_material_design/icon/material_build_icon.py`

 * *Files identical despite different names*

### Comparing `apysc-4.4.2/apysc/_material_design/icon/material_build_outlined_icon.py` & `apysc-4.4.3/apysc/_material_design/icon/material_build_outlined_icon.py`

 * *Files identical despite different names*

### Comparing `apysc-4.4.2/apysc/_material_design/icon/material_business_icon.py` & `apysc-4.4.3/apysc/_material_design/icon/material_business_icon.py`

 * *Files identical despite different names*

### Comparing `apysc-4.4.2/apysc/_material_design/icon/material_business_outlined_icon.py` & `apysc-4.4.3/apysc/_material_design/icon/material_business_outlined_icon.py`

 * *Files identical despite different names*

### Comparing `apysc-4.4.2/apysc/_material_design/icon/material_cached_icon.py` & `apysc-4.4.3/apysc/_material_design/icon/material_cached_icon.py`

 * *Files identical despite different names*

### Comparing `apysc-4.4.2/apysc/_material_design/icon/material_cached_outlined_icon.py` & `apysc-4.4.3/apysc/_material_design/icon/material_cached_outlined_icon.py`

 * *Files identical despite different names*

### Comparing `apysc-4.4.2/apysc/_material_design/icon/material_calculate_icon.py` & `apysc-4.4.3/apysc/_material_design/icon/material_calculate_icon.py`

 * *Files identical despite different names*

### Comparing `apysc-4.4.2/apysc/_material_design/icon/material_calculate_outlined_icon.py` & `apysc-4.4.3/apysc/_material_design/icon/material_calculate_outlined_icon.py`

 * *Files identical despite different names*

### Comparing `apysc-4.4.2/apysc/_material_design/icon/material_calendar_today_icon.py` & `apysc-4.4.3/apysc/_material_design/icon/material_calendar_today_icon.py`

 * *Files identical despite different names*

### Comparing `apysc-4.4.2/apysc/_material_design/icon/material_calendar_today_outlined_icon.py` & `apysc-4.4.3/apysc/_material_design/icon/material_calendar_today_outlined_icon.py`

 * *Files identical despite different names*

### Comparing `apysc-4.4.2/apysc/_material_design/icon/material_calendar_view_day_icon.py` & `apysc-4.4.3/apysc/_material_design/icon/material_calendar_view_day_icon.py`

 * *Files identical despite different names*

### Comparing `apysc-4.4.2/apysc/_material_design/icon/material_calendar_view_day_outlined_icon.py` & `apysc-4.4.3/apysc/_material_design/icon/material_calendar_view_day_outlined_icon.py`

 * *Files identical despite different names*

### Comparing `apysc-4.4.2/apysc/_material_design/icon/material_call_end_icon.py` & `apysc-4.4.3/apysc/_material_design/icon/material_call_end_icon.py`

 * *Files identical despite different names*

### Comparing `apysc-4.4.2/apysc/_material_design/icon/material_call_end_outlined_icon.py` & `apysc-4.4.3/apysc/_material_design/icon/material_call_end_outlined_icon.py`

 * *Files identical despite different names*

### Comparing `apysc-4.4.2/apysc/_material_design/icon/material_call_icon.py` & `apysc-4.4.3/apysc/_material_design/icon/material_call_icon.py`

 * *Files identical despite different names*

### Comparing `apysc-4.4.2/apysc/_material_design/icon/material_call_made_icon.py` & `apysc-4.4.3/apysc/_material_design/icon/material_call_made_icon.py`

 * *Files identical despite different names*

### Comparing `apysc-4.4.2/apysc/_material_design/icon/material_call_made_outlined_icon.py` & `apysc-4.4.3/apysc/_material_design/icon/material_call_made_outlined_icon.py`

 * *Files identical despite different names*

### Comparing `apysc-4.4.2/apysc/_material_design/icon/material_call_merge_icon.py` & `apysc-4.4.3/apysc/_material_design/icon/material_call_merge_icon.py`

 * *Files identical despite different names*

### Comparing `apysc-4.4.2/apysc/_material_design/icon/material_call_merge_outlined_icon.py` & `apysc-4.4.3/apysc/_material_design/icon/material_call_merge_outlined_icon.py`

 * *Files identical despite different names*

### Comparing `apysc-4.4.2/apysc/_material_design/icon/material_call_missed_icon.py` & `apysc-4.4.3/apysc/_material_design/icon/material_call_missed_icon.py`

 * *Files identical despite different names*

### Comparing `apysc-4.4.2/apysc/_material_design/icon/material_call_missed_outgoing_icon.py` & `apysc-4.4.3/apysc/_material_design/icon/material_call_missed_outgoing_icon.py`

 * *Files identical despite different names*

### Comparing `apysc-4.4.2/apysc/_material_design/icon/material_call_missed_outgoing_outlined_icon.py` & `apysc-4.4.3/apysc/_material_design/icon/material_call_missed_outgoing_outlined_icon.py`

 * *Files identical despite different names*

### Comparing `apysc-4.4.2/apysc/_material_design/icon/material_call_missed_outlined_icon.py` & `apysc-4.4.3/apysc/_material_design/icon/material_call_missed_outlined_icon.py`

 * *Files identical despite different names*

### Comparing `apysc-4.4.2/apysc/_material_design/icon/material_call_outlined_icon.py` & `apysc-4.4.3/apysc/_material_design/icon/material_call_outlined_icon.py`

 * *Files identical despite different names*

### Comparing `apysc-4.4.2/apysc/_material_design/icon/material_call_received_icon.py` & `apysc-4.4.3/apysc/_material_design/icon/material_call_received_icon.py`

 * *Files identical despite different names*

### Comparing `apysc-4.4.2/apysc/_material_design/icon/material_call_received_outlined_icon.py` & `apysc-4.4.3/apysc/_material_design/icon/material_call_received_outlined_icon.py`

 * *Files identical despite different names*

### Comparing `apysc-4.4.2/apysc/_material_design/icon/material_call_split_icon.py` & `apysc-4.4.3/apysc/_material_design/icon/material_call_split_icon.py`

 * *Files identical despite different names*

### Comparing `apysc-4.4.2/apysc/_material_design/icon/material_call_split_outlined_icon.py` & `apysc-4.4.3/apysc/_material_design/icon/material_call_split_outlined_icon.py`

 * *Files identical despite different names*

### Comparing `apysc-4.4.2/apysc/_material_design/icon/material_call_to_action_icon.py` & `apysc-4.4.3/apysc/_material_design/icon/material_call_to_action_icon.py`

 * *Files identical despite different names*

### Comparing `apysc-4.4.2/apysc/_material_design/icon/material_call_to_action_outlined_icon.py` & `apysc-4.4.3/apysc/_material_design/icon/material_call_to_action_outlined_icon.py`

 * *Files identical despite different names*

### Comparing `apysc-4.4.2/apysc/_material_design/icon/material_camera_enhance_icon.py` & `apysc-4.4.3/apysc/_material_design/icon/material_camera_enhance_icon.py`

 * *Files identical despite different names*

### Comparing `apysc-4.4.2/apysc/_material_design/icon/material_camera_enhance_outlined_icon.py` & `apysc-4.4.3/apysc/_material_design/icon/material_camera_enhance_outlined_icon.py`

 * *Files identical despite different names*

### Comparing `apysc-4.4.2/apysc/_material_design/icon/material_cancel_presentation_icon.py` & `apysc-4.4.3/apysc/_material_design/icon/material_cancel_presentation_icon.py`

 * *Files identical despite different names*

### Comparing `apysc-4.4.2/apysc/_material_design/icon/material_cancel_presentation_outlined_icon.py` & `apysc-4.4.3/apysc/_material_design/icon/material_cancel_presentation_outlined_icon.py`

 * *Files identical despite different names*

### Comparing `apysc-4.4.2/apysc/_material_design/icon/material_cancel_schedule_send_icon.py` & `apysc-4.4.3/apysc/_material_design/icon/material_cancel_schedule_send_icon.py`

 * *Files identical despite different names*

### Comparing `apysc-4.4.2/apysc/_material_design/icon/material_cancel_schedule_send_outlined_icon.py` & `apysc-4.4.3/apysc/_material_design/icon/material_cancel_schedule_send_outlined_icon.py`

 * *Files identical despite different names*

### Comparing `apysc-4.4.2/apysc/_material_design/icon/material_card_giftcard_icon.py` & `apysc-4.4.3/apysc/_material_design/icon/material_card_giftcard_icon.py`

 * *Files identical despite different names*

### Comparing `apysc-4.4.2/apysc/_material_design/icon/material_card_giftcard_outlined_icon.py` & `apysc-4.4.3/apysc/_material_design/icon/material_card_giftcard_outlined_icon.py`

 * *Files identical despite different names*

### Comparing `apysc-4.4.2/apysc/_material_design/icon/material_card_membership_icon.py` & `apysc-4.4.3/apysc/_material_design/icon/material_card_membership_icon.py`

 * *Files identical despite different names*

### Comparing `apysc-4.4.2/apysc/_material_design/icon/material_card_membership_outlined_icon.py` & `apysc-4.4.3/apysc/_material_design/icon/material_card_membership_outlined_icon.py`

 * *Files identical despite different names*

### Comparing `apysc-4.4.2/apysc/_material_design/icon/material_card_travel_icon.py` & `apysc-4.4.3/apysc/_material_design/icon/material_card_travel_icon.py`

 * *Files identical despite different names*

### Comparing `apysc-4.4.2/apysc/_material_design/icon/material_card_travel_outlined_icon.py` & `apysc-4.4.3/apysc/_material_design/icon/material_card_travel_outlined_icon.py`

 * *Files identical despite different names*

### Comparing `apysc-4.4.2/apysc/_material_design/icon/material_cell_wifi_icon.py` & `apysc-4.4.3/apysc/_material_design/icon/material_cell_wifi_icon.py`

 * *Files identical despite different names*

### Comparing `apysc-4.4.2/apysc/_material_design/icon/material_change_history_icon.py` & `apysc-4.4.3/apysc/_material_design/icon/material_change_history_icon.py`

 * *Files identical despite different names*

### Comparing `apysc-4.4.2/apysc/_material_design/icon/material_change_history_outlined_icon.py` & `apysc-4.4.3/apysc/_material_design/icon/material_change_history_outlined_icon.py`

 * *Files identical despite different names*

### Comparing `apysc-4.4.2/apysc/_material_design/icon/material_chat_bubble_icon.py` & `apysc-4.4.3/apysc/_material_design/icon/material_chat_bubble_icon.py`

 * *Files identical despite different names*

### Comparing `apysc-4.4.2/apysc/_material_design/icon/material_chat_bubble_outline_icon.py` & `apysc-4.4.3/apysc/_material_design/icon/material_chat_bubble_outline_icon.py`

 * *Files identical despite different names*

### Comparing `apysc-4.4.2/apysc/_material_design/icon/material_chat_bubble_outline_outlined_icon.py` & `apysc-4.4.3/apysc/_material_design/icon/material_chat_bubble_outline_outlined_icon.py`

 * *Files identical despite different names*

### Comparing `apysc-4.4.2/apysc/_material_design/icon/material_chat_bubble_outlined_icon.py` & `apysc-4.4.3/apysc/_material_design/icon/material_chat_bubble_outlined_icon.py`

 * *Files identical despite different names*

### Comparing `apysc-4.4.2/apysc/_material_design/icon/material_chat_icon.py` & `apysc-4.4.3/apysc/_material_design/icon/material_chat_icon.py`

 * *Files identical despite different names*

### Comparing `apysc-4.4.2/apysc/_material_design/icon/material_chat_outlined_icon.py` & `apysc-4.4.3/apysc/_material_design/icon/material_chat_outlined_icon.py`

 * *Files identical despite different names*

### Comparing `apysc-4.4.2/apysc/_material_design/icon/material_check_circle_icon.py` & `apysc-4.4.3/apysc/_material_design/icon/material_check_circle_icon.py`

 * *Files identical despite different names*

### Comparing `apysc-4.4.2/apysc/_material_design/icon/material_check_circle_outline_icon.py` & `apysc-4.4.3/apysc/_material_design/icon/material_check_circle_outline_icon.py`

 * *Files identical despite different names*

### Comparing `apysc-4.4.2/apysc/_material_design/icon/material_check_circle_outline_outlined_icon.py` & `apysc-4.4.3/apysc/_material_design/icon/material_check_circle_outline_outlined_icon.py`

 * *Files identical despite different names*

### Comparing `apysc-4.4.2/apysc/_material_design/icon/material_check_circle_outlined_icon.py` & `apysc-4.4.3/apysc/_material_design/icon/material_check_circle_outlined_icon.py`

 * *Files identical despite different names*

### Comparing `apysc-4.4.2/apysc/_material_design/icon/material_chrome_reader_mode_icon.py` & `apysc-4.4.3/apysc/_material_design/icon/material_chrome_reader_mode_icon.py`

 * *Files identical despite different names*

### Comparing `apysc-4.4.2/apysc/_material_design/icon/material_chrome_reader_mode_outlined_icon.py` & `apysc-4.4.3/apysc/_material_design/icon/material_chrome_reader_mode_outlined_icon.py`

 * *Files identical despite different names*

### Comparing `apysc-4.4.2/apysc/_material_design/icon/material_circle_notifications_icon.py` & `apysc-4.4.3/apysc/_material_design/icon/material_circle_notifications_icon.py`

 * *Files identical despite different names*

### Comparing `apysc-4.4.2/apysc/_material_design/icon/material_class_icon.py` & `apysc-4.4.3/apysc/_material_design/icon/material_class_icon.py`

 * *Files identical despite different names*

### Comparing `apysc-4.4.2/apysc/_material_design/icon/material_class_outlined_icon.py` & `apysc-4.4.3/apysc/_material_design/icon/material_class_outlined_icon.py`

 * *Files identical despite different names*

### Comparing `apysc-4.4.2/apysc/_material_design/icon/material_clear_all_icon.py` & `apysc-4.4.3/apysc/_material_design/icon/material_clear_all_icon.py`

 * *Files identical despite different names*

### Comparing `apysc-4.4.2/apysc/_material_design/icon/material_clear_all_outlined_icon.py` & `apysc-4.4.3/apysc/_material_design/icon/material_clear_all_outlined_icon.py`

 * *Files identical despite different names*

### Comparing `apysc-4.4.2/apysc/_material_design/icon/material_clear_icon.py` & `apysc-4.4.3/apysc/_material_design/icon/material_clear_icon.py`

 * *Files identical despite different names*

### Comparing `apysc-4.4.2/apysc/_material_design/icon/material_clear_outlined_icon.py` & `apysc-4.4.3/apysc/_material_design/icon/material_clear_outlined_icon.py`

 * *Files identical despite different names*

### Comparing `apysc-4.4.2/apysc/_material_design/icon/material_close_fullscreen_icon.py` & `apysc-4.4.3/apysc/_material_design/icon/material_close_fullscreen_icon.py`

 * *Files identical despite different names*

### Comparing `apysc-4.4.2/apysc/_material_design/icon/material_close_fullscreen_outlined_icon.py` & `apysc-4.4.3/apysc/_material_design/icon/material_close_fullscreen_outlined_icon.py`

 * *Files identical despite different names*

### Comparing `apysc-4.4.2/apysc/_material_design/icon/material_closed_caption_disabled_icon.py` & `apysc-4.4.3/apysc/_material_design/icon/material_closed_caption_disabled_icon.py`

 * *Files identical despite different names*

### Comparing `apysc-4.4.2/apysc/_material_design/icon/material_closed_caption_disabled_outlined_icon.py` & `apysc-4.4.3/apysc/_material_design/icon/material_closed_caption_disabled_outlined_icon.py`

 * *Files identical despite different names*

### Comparing `apysc-4.4.2/apysc/_material_design/icon/material_closed_caption_icon.py` & `apysc-4.4.3/apysc/_material_design/icon/material_closed_caption_icon.py`

 * *Files identical despite different names*

### Comparing `apysc-4.4.2/apysc/_material_design/icon/material_closed_caption_off_icon.py` & `apysc-4.4.3/apysc/_material_design/icon/material_closed_caption_off_icon.py`

 * *Files identical despite different names*

### Comparing `apysc-4.4.2/apysc/_material_design/icon/material_closed_caption_outlined_icon.py` & `apysc-4.4.3/apysc/_material_design/icon/material_closed_caption_outlined_icon.py`

 * *Files identical despite different names*

### Comparing `apysc-4.4.2/apysc/_material_design/icon/material_code_icon.py` & `apysc-4.4.3/apysc/_material_design/icon/material_code_icon.py`

 * *Files identical despite different names*

### Comparing `apysc-4.4.2/apysc/_material_design/icon/material_code_outlined_icon.py` & `apysc-4.4.3/apysc/_material_design/icon/material_code_outlined_icon.py`

 * *Files identical despite different names*

### Comparing `apysc-4.4.2/apysc/_material_design/icon/material_comment_bank_icon.py` & `apysc-4.4.3/apysc/_material_design/icon/material_comment_bank_icon.py`

 * *Files identical despite different names*

### Comparing `apysc-4.4.2/apysc/_material_design/icon/material_comment_bank_outlined_icon.py` & `apysc-4.4.3/apysc/_material_design/icon/material_comment_bank_outlined_icon.py`

 * *Files identical despite different names*

### Comparing `apysc-4.4.2/apysc/_material_design/icon/material_comment_icon.py` & `apysc-4.4.3/apysc/_material_design/icon/material_comment_icon.py`

 * *Files identical despite different names*

### Comparing `apysc-4.4.2/apysc/_material_design/icon/material_comment_outlined_icon.py` & `apysc-4.4.3/apysc/_material_design/icon/material_comment_outlined_icon.py`

 * *Files identical despite different names*

### Comparing `apysc-4.4.2/apysc/_material_design/icon/material_commute_icon.py` & `apysc-4.4.3/apysc/_material_design/icon/material_commute_icon.py`

 * *Files identical despite different names*

### Comparing `apysc-4.4.2/apysc/_material_design/icon/material_commute_outlined_icon.py` & `apysc-4.4.3/apysc/_material_design/icon/material_commute_outlined_icon.py`

 * *Files identical despite different names*

### Comparing `apysc-4.4.2/apysc/_material_design/icon/material_compare_arrows_icon.py` & `apysc-4.4.3/apysc/_material_design/icon/material_compare_arrows_icon.py`

 * *Files identical despite different names*

### Comparing `apysc-4.4.2/apysc/_material_design/icon/material_compare_arrows_outlined_icon.py` & `apysc-4.4.3/apysc/_material_design/icon/material_compare_arrows_outlined_icon.py`

 * *Files identical despite different names*

### Comparing `apysc-4.4.2/apysc/_material_design/icon/material_compress_icon.py` & `apysc-4.4.3/apysc/_material_design/icon/material_compress_icon.py`

 * *Files identical despite different names*

### Comparing `apysc-4.4.2/apysc/_material_design/icon/material_contact_mail_icon.py` & `apysc-4.4.3/apysc/_material_design/icon/material_contact_mail_icon.py`

 * *Files identical despite different names*

### Comparing `apysc-4.4.2/apysc/_material_design/icon/material_contact_mail_outlined_icon.py` & `apysc-4.4.3/apysc/_material_design/icon/material_contact_mail_outlined_icon.py`

 * *Files identical despite different names*

### Comparing `apysc-4.4.2/apysc/_material_design/icon/material_contact_page_icon.py` & `apysc-4.4.3/apysc/_material_design/icon/material_contact_page_icon.py`

 * *Files identical despite different names*

### Comparing `apysc-4.4.2/apysc/_material_design/icon/material_contact_page_outlined_icon.py` & `apysc-4.4.3/apysc/_material_design/icon/material_contact_page_outlined_icon.py`

 * *Files identical despite different names*

### Comparing `apysc-4.4.2/apysc/_material_design/icon/material_contact_phone_icon.py` & `apysc-4.4.3/apysc/_material_design/icon/material_contact_phone_icon.py`

 * *Files identical despite different names*

### Comparing `apysc-4.4.2/apysc/_material_design/icon/material_contact_phone_outlined_icon.py` & `apysc-4.4.3/apysc/_material_design/icon/material_contact_phone_outlined_icon.py`

 * *Files identical despite different names*

### Comparing `apysc-4.4.2/apysc/_material_design/icon/material_contact_support_icon.py` & `apysc-4.4.3/apysc/_material_design/icon/material_contact_support_icon.py`

 * *Files identical despite different names*

### Comparing `apysc-4.4.2/apysc/_material_design/icon/material_contact_support_outlined_icon.py` & `apysc-4.4.3/apysc/_material_design/icon/material_contact_support_outlined_icon.py`

 * *Files identical despite different names*

### Comparing `apysc-4.4.2/apysc/_material_design/icon/material_contactless_icon.py` & `apysc-4.4.3/apysc/_material_design/icon/material_contactless_icon.py`

 * *Files identical despite different names*

### Comparing `apysc-4.4.2/apysc/_material_design/icon/material_contactless_outlined_icon.py` & `apysc-4.4.3/apysc/_material_design/icon/material_contactless_outlined_icon.py`

 * *Files identical despite different names*

### Comparing `apysc-4.4.2/apysc/_material_design/icon/material_contacts_icon.py` & `apysc-4.4.3/apysc/_material_design/icon/material_contacts_icon.py`

 * *Files identical despite different names*

### Comparing `apysc-4.4.2/apysc/_material_design/icon/material_contacts_outlined_icon.py` & `apysc-4.4.3/apysc/_material_design/icon/material_contacts_outlined_icon.py`

 * *Files identical despite different names*

### Comparing `apysc-4.4.2/apysc/_material_design/icon/material_content_copy_icon.py` & `apysc-4.4.3/apysc/_material_design/icon/material_content_copy_icon.py`

 * *Files identical despite different names*

### Comparing `apysc-4.4.2/apysc/_material_design/icon/material_content_copy_outlined_icon.py` & `apysc-4.4.3/apysc/_material_design/icon/material_content_copy_outlined_icon.py`

 * *Files identical despite different names*

### Comparing `apysc-4.4.2/apysc/_material_design/icon/material_content_cut_icon.py` & `apysc-4.4.3/apysc/_material_design/icon/material_content_cut_icon.py`

 * *Files identical despite different names*

### Comparing `apysc-4.4.2/apysc/_material_design/icon/material_content_cut_outlined_icon.py` & `apysc-4.4.3/apysc/_material_design/icon/material_content_cut_outlined_icon.py`

 * *Files identical despite different names*

### Comparing `apysc-4.4.2/apysc/_material_design/icon/material_content_paste_icon.py` & `apysc-4.4.3/apysc/_material_design/icon/material_content_paste_icon.py`

 * *Files identical despite different names*

### Comparing `apysc-4.4.2/apysc/_material_design/icon/material_content_paste_outlined_icon.py` & `apysc-4.4.3/apysc/_material_design/icon/material_content_paste_outlined_icon.py`

 * *Files identical despite different names*

### Comparing `apysc-4.4.2/apysc/_material_design/icon/material_control_camera_icon.py` & `apysc-4.4.3/apysc/_material_design/icon/material_control_camera_icon.py`

 * *Files identical despite different names*

### Comparing `apysc-4.4.2/apysc/_material_design/icon/material_control_camera_outlined_icon.py` & `apysc-4.4.3/apysc/_material_design/icon/material_control_camera_outlined_icon.py`

 * *Files identical despite different names*

### Comparing `apysc-4.4.2/apysc/_material_design/icon/material_copyright_icon.py` & `apysc-4.4.3/apysc/_material_design/icon/material_copyright_icon.py`

 * *Files identical despite different names*

### Comparing `apysc-4.4.2/apysc/_material_design/icon/material_copyright_outlined_icon.py` & `apysc-4.4.3/apysc/_material_design/icon/material_copyright_outlined_icon.py`

 * *Files identical despite different names*

### Comparing `apysc-4.4.2/apysc/_material_design/icon/material_create_icon.py` & `apysc-4.4.3/apysc/_material_design/icon/material_create_icon.py`

 * *Files identical despite different names*

### Comparing `apysc-4.4.2/apysc/_material_design/icon/material_create_outlined_icon.py` & `apysc-4.4.3/apysc/_material_design/icon/material_create_outlined_icon.py`

 * *Files identical despite different names*

### Comparing `apysc-4.4.2/apysc/_material_design/icon/material_credit_card_icon.py` & `apysc-4.4.3/apysc/_material_design/icon/material_credit_card_icon.py`

 * *Files identical despite different names*

### Comparing `apysc-4.4.2/apysc/_material_design/icon/material_credit_card_outlined_icon.py` & `apysc-4.4.3/apysc/_material_design/icon/material_credit_card_outlined_icon.py`

 * *Files identical despite different names*

### Comparing `apysc-4.4.2/apysc/_material_design/icon/material_dangerous_icon.py` & `apysc-4.4.3/apysc/_material_design/icon/material_dangerous_icon.py`

 * *Files identical despite different names*

### Comparing `apysc-4.4.2/apysc/_material_design/icon/material_dashboard_customize_icon.py` & `apysc-4.4.3/apysc/_material_design/icon/material_dashboard_customize_icon.py`

 * *Files identical despite different names*

### Comparing `apysc-4.4.2/apysc/_material_design/icon/material_dashboard_icon.py` & `apysc-4.4.3/apysc/_material_design/icon/material_dashboard_icon.py`

 * *Files identical despite different names*

### Comparing `apysc-4.4.2/apysc/_material_design/icon/material_dashboard_outlined_icon.py` & `apysc-4.4.3/apysc/_material_design/icon/material_dashboard_outlined_icon.py`

 * *Files identical despite different names*

### Comparing `apysc-4.4.2/apysc/_material_design/icon/material_date_range_icon.py` & `apysc-4.4.3/apysc/_material_design/icon/material_date_range_icon.py`

 * *Files identical despite different names*

### Comparing `apysc-4.4.2/apysc/_material_design/icon/material_date_range_outlined_icon.py` & `apysc-4.4.3/apysc/_material_design/icon/material_date_range_outlined_icon.py`

 * *Files identical despite different names*

### Comparing `apysc-4.4.2/apysc/_material_design/icon/material_delete_forever_icon.py` & `apysc-4.4.3/apysc/_material_design/icon/material_delete_forever_icon.py`

 * *Files identical despite different names*

### Comparing `apysc-4.4.2/apysc/_material_design/icon/material_delete_forever_outlined_icon.py` & `apysc-4.4.3/apysc/_material_design/icon/material_delete_forever_outlined_icon.py`

 * *Files identical despite different names*

### Comparing `apysc-4.4.2/apysc/_material_design/icon/material_delete_icon.py` & `apysc-4.4.3/apysc/_material_design/icon/material_delete_icon.py`

 * *Files identical despite different names*

### Comparing `apysc-4.4.2/apysc/_material_design/icon/material_delete_outline_icon.py` & `apysc-4.4.3/apysc/_material_design/icon/material_delete_outline_icon.py`

 * *Files identical despite different names*

### Comparing `apysc-4.4.2/apysc/_material_design/icon/material_delete_outline_outlined_icon.py` & `apysc-4.4.3/apysc/_material_design/icon/material_delete_outline_outlined_icon.py`

 * *Files identical despite different names*

### Comparing `apysc-4.4.2/apysc/_material_design/icon/material_delete_outlined_icon.py` & `apysc-4.4.3/apysc/_material_design/icon/material_delete_outlined_icon.py`

 * *Files identical despite different names*

### Comparing `apysc-4.4.2/apysc/_material_design/icon/material_delete_sweep_icon.py` & `apysc-4.4.3/apysc/_material_design/icon/material_delete_sweep_icon.py`

 * *Files identical despite different names*

### Comparing `apysc-4.4.2/apysc/_material_design/icon/material_delete_sweep_outlined_icon.py` & `apysc-4.4.3/apysc/_material_design/icon/material_delete_sweep_outlined_icon.py`

 * *Files identical despite different names*

### Comparing `apysc-4.4.2/apysc/_material_design/icon/material_description_icon.py` & `apysc-4.4.3/apysc/_material_design/icon/material_description_icon.py`

 * *Files identical despite different names*

### Comparing `apysc-4.4.2/apysc/_material_design/icon/material_description_outlined_icon.py` & `apysc-4.4.3/apysc/_material_design/icon/material_description_outlined_icon.py`

 * *Files identical despite different names*

### Comparing `apysc-4.4.2/apysc/_material_design/icon/material_desktop_access_disabled_icon.py` & `apysc-4.4.3/apysc/_material_design/icon/material_desktop_access_disabled_icon.py`

 * *Files identical despite different names*

### Comparing `apysc-4.4.2/apysc/_material_design/icon/material_desktop_access_disabled_outlined_icon.py` & `apysc-4.4.3/apysc/_material_design/icon/material_desktop_access_disabled_outlined_icon.py`

 * *Files identical despite different names*

### Comparing `apysc-4.4.2/apysc/_material_design/icon/material_dialer_sip_icon.py` & `apysc-4.4.3/apysc/_material_design/icon/material_dialer_sip_icon.py`

 * *Files identical despite different names*

### Comparing `apysc-4.4.2/apysc/_material_design/icon/material_dialer_sip_outlined_icon.py` & `apysc-4.4.3/apysc/_material_design/icon/material_dialer_sip_outlined_icon.py`

 * *Files identical despite different names*

### Comparing `apysc-4.4.2/apysc/_material_design/icon/material_dialpad_icon.py` & `apysc-4.4.3/apysc/_material_design/icon/material_dialpad_icon.py`

 * *Files identical despite different names*

### Comparing `apysc-4.4.2/apysc/_material_design/icon/material_dialpad_outlined_icon.py` & `apysc-4.4.3/apysc/_material_design/icon/material_dialpad_outlined_icon.py`

 * *Files identical despite different names*

### Comparing `apysc-4.4.2/apysc/_material_design/icon/material_disabled_by_default_icon.py` & `apysc-4.4.3/apysc/_material_design/icon/material_disabled_by_default_icon.py`

 * *Files identical despite different names*

### Comparing `apysc-4.4.2/apysc/_material_design/icon/material_disabled_by_default_outlined_icon.py` & `apysc-4.4.3/apysc/_material_design/icon/material_disabled_by_default_outlined_icon.py`

 * *Files identical despite different names*

### Comparing `apysc-4.4.2/apysc/_material_design/icon/material_dns_icon.py` & `apysc-4.4.3/apysc/_material_design/icon/material_dns_icon.py`

 * *Files identical despite different names*

### Comparing `apysc-4.4.2/apysc/_material_design/icon/material_dns_outlined_icon.py` & `apysc-4.4.3/apysc/_material_design/icon/material_dns_outlined_icon.py`

 * *Files identical despite different names*

### Comparing `apysc-4.4.2/apysc/_material_design/icon/material_domain_disabled_icon.py` & `apysc-4.4.3/apysc/_material_design/icon/material_domain_disabled_icon.py`

 * *Files identical despite different names*

### Comparing `apysc-4.4.2/apysc/_material_design/icon/material_domain_disabled_outlined_icon.py` & `apysc-4.4.3/apysc/_material_design/icon/material_domain_disabled_outlined_icon.py`

 * *Files identical despite different names*

### Comparing `apysc-4.4.2/apysc/_material_design/icon/material_domain_verification_icon.py` & `apysc-4.4.3/apysc/_material_design/icon/material_domain_verification_icon.py`

 * *Files identical despite different names*

### Comparing `apysc-4.4.2/apysc/_material_design/icon/material_domain_verification_outlined_icon.py` & `apysc-4.4.3/apysc/_material_design/icon/material_domain_verification_outlined_icon.py`

 * *Files identical despite different names*

### Comparing `apysc-4.4.2/apysc/_material_design/icon/material_done_all_icon.py` & `apysc-4.4.3/apysc/_material_design/icon/material_done_all_icon.py`

 * *Files identical despite different names*

### Comparing `apysc-4.4.2/apysc/_material_design/icon/material_done_all_outlined_icon.py` & `apysc-4.4.3/apysc/_material_design/icon/material_done_all_outlined_icon.py`

 * *Files identical despite different names*

### Comparing `apysc-4.4.2/apysc/_material_design/icon/material_done_icon.py` & `apysc-4.4.3/apysc/_material_design/icon/material_done_icon.py`

 * *Files identical despite different names*

### Comparing `apysc-4.4.2/apysc/_material_design/icon/material_done_outline_icon.py` & `apysc-4.4.3/apysc/_material_design/icon/material_done_outline_icon.py`

 * *Files identical despite different names*

### Comparing `apysc-4.4.2/apysc/_material_design/icon/material_done_outline_outlined_icon.py` & `apysc-4.4.3/apysc/_material_design/icon/material_done_outline_outlined_icon.py`

 * *Files identical despite different names*

### Comparing `apysc-4.4.2/apysc/_material_design/icon/material_done_outlined_icon.py` & `apysc-4.4.3/apysc/_material_design/icon/material_done_outlined_icon.py`

 * *Files identical despite different names*

### Comparing `apysc-4.4.2/apysc/_material_design/icon/material_donut_large_icon.py` & `apysc-4.4.3/apysc/_material_design/icon/material_donut_large_icon.py`

 * *Files identical despite different names*

### Comparing `apysc-4.4.2/apysc/_material_design/icon/material_donut_large_outlined_icon.py` & `apysc-4.4.3/apysc/_material_design/icon/material_donut_large_outlined_icon.py`

 * *Files identical despite different names*

### Comparing `apysc-4.4.2/apysc/_material_design/icon/material_donut_small_icon.py` & `apysc-4.4.3/apysc/_material_design/icon/material_donut_small_icon.py`

 * *Files identical despite different names*

### Comparing `apysc-4.4.2/apysc/_material_design/icon/material_donut_small_outlined_icon.py` & `apysc-4.4.3/apysc/_material_design/icon/material_donut_small_outlined_icon.py`

 * *Files identical despite different names*

### Comparing `apysc-4.4.2/apysc/_material_design/icon/material_drafts_icon.py` & `apysc-4.4.3/apysc/_material_design/icon/material_drafts_icon.py`

 * *Files identical despite different names*

### Comparing `apysc-4.4.2/apysc/_material_design/icon/material_drafts_outlined_icon.py` & `apysc-4.4.3/apysc/_material_design/icon/material_drafts_outlined_icon.py`

 * *Files identical despite different names*

### Comparing `apysc-4.4.2/apysc/_material_design/icon/material_drag_indicator_icon.py` & `apysc-4.4.3/apysc/_material_design/icon/material_drag_indicator_icon.py`

 * *Files identical despite different names*

### Comparing `apysc-4.4.2/apysc/_material_design/icon/material_drag_indicator_outlined_icon.py` & `apysc-4.4.3/apysc/_material_design/icon/material_drag_indicator_outlined_icon.py`

 * *Files identical despite different names*

### Comparing `apysc-4.4.2/apysc/_material_design/icon/material_duo_icon.py` & `apysc-4.4.3/apysc/_material_design/icon/material_duo_icon.py`

 * *Files identical despite different names*

### Comparing `apysc-4.4.2/apysc/_material_design/icon/material_duo_outlined_icon.py` & `apysc-4.4.3/apysc/_material_design/icon/material_duo_outlined_icon.py`

 * *Files identical despite different names*

### Comparing `apysc-4.4.2/apysc/_material_design/icon/material_dynamic_feed_icon.py` & `apysc-4.4.3/apysc/_material_design/icon/material_dynamic_feed_icon.py`

 * *Files identical despite different names*

### Comparing `apysc-4.4.2/apysc/_material_design/icon/material_dynamic_feed_outlined_icon.py` & `apysc-4.4.3/apysc/_material_design/icon/material_dynamic_feed_outlined_icon.py`

 * *Files identical despite different names*

### Comparing `apysc-4.4.2/apysc/_material_design/icon/material_dynamic_form_icon.py` & `apysc-4.4.3/apysc/_material_design/icon/material_dynamic_form_icon.py`

 * *Files identical despite different names*

### Comparing `apysc-4.4.2/apysc/_material_design/icon/material_dynamic_form_outlined_icon.py` & `apysc-4.4.3/apysc/_material_design/icon/material_dynamic_form_outlined_icon.py`

 * *Files identical despite different names*

### Comparing `apysc-4.4.2/apysc/_material_design/icon/material_eco_icon.py` & `apysc-4.4.3/apysc/_material_design/icon/material_eco_icon.py`

 * *Files identical despite different names*

### Comparing `apysc-4.4.2/apysc/_material_design/icon/material_eco_outlined_icon.py` & `apysc-4.4.3/apysc/_material_design/icon/material_eco_outlined_icon.py`

 * *Files identical despite different names*

### Comparing `apysc-4.4.2/apysc/_material_design/icon/material_edit_off_icon.py` & `apysc-4.4.3/apysc/_material_design/icon/material_edit_off_icon.py`

 * *Files identical despite different names*

### Comparing `apysc-4.4.2/apysc/_material_design/icon/material_eject_icon.py` & `apysc-4.4.3/apysc/_material_design/icon/material_eject_icon.py`

 * *Files identical despite different names*

### Comparing `apysc-4.4.2/apysc/_material_design/icon/material_eject_outlined_icon.py` & `apysc-4.4.3/apysc/_material_design/icon/material_eject_outlined_icon.py`

 * *Files identical despite different names*

### Comparing `apysc-4.4.2/apysc/_material_design/icon/material_email_icon.py` & `apysc-4.4.3/apysc/_material_design/icon/material_email_icon.py`

 * *Files identical despite different names*

### Comparing `apysc-4.4.2/apysc/_material_design/icon/material_email_outlined_icon.py` & `apysc-4.4.3/apysc/_material_design/icon/material_email_outlined_icon.py`

 * *Files identical despite different names*

### Comparing `apysc-4.4.2/apysc/_material_design/icon/material_equalizer_icon.py` & `apysc-4.4.3/apysc/_material_design/icon/material_equalizer_icon.py`

 * *Files identical despite different names*

### Comparing `apysc-4.4.2/apysc/_material_design/icon/material_equalizer_outlined_icon.py` & `apysc-4.4.3/apysc/_material_design/icon/material_equalizer_outlined_icon.py`

 * *Files identical despite different names*

### Comparing `apysc-4.4.2/apysc/_material_design/icon/material_error_icon.py` & `apysc-4.4.3/apysc/_material_design/icon/material_error_icon.py`

 * *Files identical despite different names*

### Comparing `apysc-4.4.2/apysc/_material_design/icon/material_error_outline_icon.py` & `apysc-4.4.3/apysc/_material_design/icon/material_error_outline_icon.py`

 * *Files identical despite different names*

### Comparing `apysc-4.4.2/apysc/_material_design/icon/material_error_outline_outlined_icon.py` & `apysc-4.4.3/apysc/_material_design/icon/material_error_outline_outlined_icon.py`

 * *Files identical despite different names*

### Comparing `apysc-4.4.2/apysc/_material_design/icon/material_error_outlined_icon.py` & `apysc-4.4.3/apysc/_material_design/icon/material_error_outlined_icon.py`

 * *Files identical despite different names*

### Comparing `apysc-4.4.2/apysc/_material_design/icon/material_euro_symbol_icon.py` & `apysc-4.4.3/apysc/_material_design/icon/material_euro_symbol_icon.py`

 * *Files identical despite different names*

### Comparing `apysc-4.4.2/apysc/_material_design/icon/material_euro_symbol_outlined_icon.py` & `apysc-4.4.3/apysc/_material_design/icon/material_euro_symbol_outlined_icon.py`

 * *Files identical despite different names*

### Comparing `apysc-4.4.2/apysc/_material_design/icon/material_event_icon.py` & `apysc-4.4.3/apysc/_material_design/icon/material_event_icon.py`

 * *Files identical despite different names*

### Comparing `apysc-4.4.2/apysc/_material_design/icon/material_event_outlined_icon.py` & `apysc-4.4.3/apysc/_material_design/icon/material_event_outlined_icon.py`

 * *Files identical despite different names*

### Comparing `apysc-4.4.2/apysc/_material_design/icon/material_event_seat_icon.py` & `apysc-4.4.3/apysc/_material_design/icon/material_event_seat_icon.py`

 * *Files identical despite different names*

### Comparing `apysc-4.4.2/apysc/_material_design/icon/material_event_seat_outlined_icon.py` & `apysc-4.4.3/apysc/_material_design/icon/material_event_seat_outlined_icon.py`

 * *Files identical despite different names*

### Comparing `apysc-4.4.2/apysc/_material_design/icon/material_exit_to_app_icon.py` & `apysc-4.4.3/apysc/_material_design/icon/material_exit_to_app_icon.py`

 * *Files identical despite different names*

### Comparing `apysc-4.4.2/apysc/_material_design/icon/material_exit_to_app_outlined_icon.py` & `apysc-4.4.3/apysc/_material_design/icon/material_exit_to_app_outlined_icon.py`

 * *Files identical despite different names*

### Comparing `apysc-4.4.2/apysc/_material_design/icon/material_expand_icon.py` & `apysc-4.4.3/apysc/_material_design/icon/material_expand_icon.py`

 * *Files identical despite different names*

### Comparing `apysc-4.4.2/apysc/_material_design/icon/material_explicit_icon.py` & `apysc-4.4.3/apysc/_material_design/icon/material_explicit_icon.py`

 * *Files identical despite different names*

### Comparing `apysc-4.4.2/apysc/_material_design/icon/material_explicit_outlined_icon.py` & `apysc-4.4.3/apysc/_material_design/icon/material_explicit_outlined_icon.py`

 * *Files identical despite different names*

### Comparing `apysc-4.4.2/apysc/_material_design/icon/material_explore_icon.py` & `apysc-4.4.3/apysc/_material_design/icon/material_explore_icon.py`

 * *Files identical despite different names*

### Comparing `apysc-4.4.2/apysc/_material_design/icon/material_explore_off_icon.py` & `apysc-4.4.3/apysc/_material_design/icon/material_explore_off_icon.py`

 * *Files identical despite different names*

### Comparing `apysc-4.4.2/apysc/_material_design/icon/material_explore_off_outlined_icon.py` & `apysc-4.4.3/apysc/_material_design/icon/material_explore_off_outlined_icon.py`

 * *Files identical despite different names*

### Comparing `apysc-4.4.2/apysc/_material_design/icon/material_explore_outlined_icon.py` & `apysc-4.4.3/apysc/_material_design/icon/material_explore_outlined_icon.py`

 * *Files identical despite different names*

### Comparing `apysc-4.4.2/apysc/_material_design/icon/material_extension_icon.py` & `apysc-4.4.3/apysc/_material_design/icon/material_extension_icon.py`

 * *Files identical despite different names*

### Comparing `apysc-4.4.2/apysc/_material_design/icon/material_extension_outlined_icon.py` & `apysc-4.4.3/apysc/_material_design/icon/material_extension_outlined_icon.py`

 * *Files identical despite different names*

### Comparing `apysc-4.4.2/apysc/_material_design/icon/material_face_icon.py` & `apysc-4.4.3/apysc/_material_design/icon/material_face_icon.py`

 * *Files identical despite different names*

### Comparing `apysc-4.4.2/apysc/_material_design/icon/material_face_outlined_icon.py` & `apysc-4.4.3/apysc/_material_design/icon/material_face_outlined_icon.py`

 * *Files identical despite different names*

### Comparing `apysc-4.4.2/apysc/_material_design/icon/material_face_unlock_outlined_icon.py` & `apysc-4.4.3/apysc/_material_design/icon/material_face_unlock_outlined_icon.py`

 * *Files identical despite different names*

### Comparing `apysc-4.4.2/apysc/_material_design/icon/material_fact_check_icon.py` & `apysc-4.4.3/apysc/_material_design/icon/material_fact_check_icon.py`

 * *Files identical despite different names*

### Comparing `apysc-4.4.2/apysc/_material_design/icon/material_fact_check_outlined_icon.py` & `apysc-4.4.3/apysc/_material_design/icon/material_fact_check_outlined_icon.py`

 * *Files identical despite different names*

### Comparing `apysc-4.4.2/apysc/_material_design/icon/material_fast_forward_icon.py` & `apysc-4.4.3/apysc/_material_design/icon/material_fast_forward_icon.py`

 * *Files identical despite different names*

### Comparing `apysc-4.4.2/apysc/_material_design/icon/material_fast_forward_outlined_icon.py` & `apysc-4.4.3/apysc/_material_design/icon/material_fast_forward_outlined_icon.py`

 * *Files identical despite different names*

### Comparing `apysc-4.4.2/apysc/_material_design/icon/material_fast_rewind_icon.py` & `apysc-4.4.3/apysc/_material_design/icon/material_fast_rewind_icon.py`

 * *Files identical despite different names*

### Comparing `apysc-4.4.2/apysc/_material_design/icon/material_fast_rewind_outlined_icon.py` & `apysc-4.4.3/apysc/_material_design/icon/material_fast_rewind_outlined_icon.py`

 * *Files identical despite different names*

### Comparing `apysc-4.4.2/apysc/_material_design/icon/material_favorite_border_icon.py` & `apysc-4.4.3/apysc/_material_design/icon/material_favorite_border_icon.py`

 * *Files identical despite different names*

### Comparing `apysc-4.4.2/apysc/_material_design/icon/material_favorite_border_outlined_icon.py` & `apysc-4.4.3/apysc/_material_design/icon/material_favorite_border_outlined_icon.py`

 * *Files identical despite different names*

### Comparing `apysc-4.4.2/apysc/_material_design/icon/material_favorite_icon.py` & `apysc-4.4.3/apysc/_material_design/icon/material_favorite_icon.py`

 * *Files identical despite different names*

### Comparing `apysc-4.4.2/apysc/_material_design/icon/material_favorite_outlined_icon.py` & `apysc-4.4.3/apysc/_material_design/icon/material_favorite_outlined_icon.py`

 * *Files identical despite different names*

### Comparing `apysc-4.4.2/apysc/_material_design/icon/material_featured_play_list_icon.py` & `apysc-4.4.3/apysc/_material_design/icon/material_featured_play_list_icon.py`

 * *Files identical despite different names*

### Comparing `apysc-4.4.2/apysc/_material_design/icon/material_featured_play_list_outlined_icon.py` & `apysc-4.4.3/apysc/_material_design/icon/material_featured_play_list_outlined_icon.py`

 * *Files identical despite different names*

### Comparing `apysc-4.4.2/apysc/_material_design/icon/material_featured_video_icon.py` & `apysc-4.4.3/apysc/_material_design/icon/material_featured_video_icon.py`

 * *Files identical despite different names*

### Comparing `apysc-4.4.2/apysc/_material_design/icon/material_featured_video_outlined_icon.py` & `apysc-4.4.3/apysc/_material_design/icon/material_featured_video_outlined_icon.py`

 * *Files identical despite different names*

### Comparing `apysc-4.4.2/apysc/_material_design/icon/material_feedback_icon.py` & `apysc-4.4.3/apysc/_material_design/icon/material_feedback_icon.py`

 * *Files identical despite different names*

### Comparing `apysc-4.4.2/apysc/_material_design/icon/material_feedback_outlined_icon.py` & `apysc-4.4.3/apysc/_material_design/icon/material_feedback_outlined_icon.py`

 * *Files identical despite different names*

### Comparing `apysc-4.4.2/apysc/_material_design/icon/material_fiber_dvr_icon.py` & `apysc-4.4.3/apysc/_material_design/icon/material_fiber_dvr_icon.py`

 * *Files identical despite different names*

### Comparing `apysc-4.4.2/apysc/_material_design/icon/material_fiber_dvr_outlined_icon.py` & `apysc-4.4.3/apysc/_material_design/icon/material_fiber_dvr_outlined_icon.py`

 * *Files identical despite different names*

### Comparing `apysc-4.4.2/apysc/_material_design/icon/material_fiber_manual_record_icon.py` & `apysc-4.4.3/apysc/_material_design/icon/material_fiber_manual_record_icon.py`

 * *Files identical despite different names*

### Comparing `apysc-4.4.2/apysc/_material_design/icon/material_fiber_manual_record_outlined_icon.py` & `apysc-4.4.3/apysc/_material_design/icon/material_fiber_manual_record_outlined_icon.py`

 * *Files identical despite different names*

### Comparing `apysc-4.4.2/apysc/_material_design/icon/material_fiber_new_icon.py` & `apysc-4.4.3/apysc/_material_design/icon/material_fiber_new_icon.py`

 * *Files identical despite different names*

### Comparing `apysc-4.4.2/apysc/_material_design/icon/material_fiber_new_outlined_icon.py` & `apysc-4.4.3/apysc/_material_design/icon/material_fiber_new_outlined_icon.py`

 * *Files identical despite different names*

### Comparing `apysc-4.4.2/apysc/_material_design/icon/material_fiber_pin_icon.py` & `apysc-4.4.3/apysc/_material_design/icon/material_fiber_pin_icon.py`

 * *Files identical despite different names*

### Comparing `apysc-4.4.2/apysc/_material_design/icon/material_fiber_pin_outlined_icon.py` & `apysc-4.4.3/apysc/_material_design/icon/material_fiber_pin_outlined_icon.py`

 * *Files identical despite different names*

### Comparing `apysc-4.4.2/apysc/_material_design/icon/material_fiber_smart_record_icon.py` & `apysc-4.4.3/apysc/_material_design/icon/material_fiber_smart_record_icon.py`

 * *Files identical despite different names*

### Comparing `apysc-4.4.2/apysc/_material_design/icon/material_fiber_smart_record_outlined_icon.py` & `apysc-4.4.3/apysc/_material_design/icon/material_fiber_smart_record_outlined_icon.py`

 * *Files identical despite different names*

### Comparing `apysc-4.4.2/apysc/_material_design/icon/material_file_copy_icon.py` & `apysc-4.4.3/apysc/_material_design/icon/material_file_copy_icon.py`

 * *Files identical despite different names*

### Comparing `apysc-4.4.2/apysc/_material_design/icon/material_file_copy_outlined_icon.py` & `apysc-4.4.3/apysc/_material_design/icon/material_file_copy_outlined_icon.py`

 * *Files identical despite different names*

### Comparing `apysc-4.4.2/apysc/_material_design/icon/material_file_present_icon.py` & `apysc-4.4.3/apysc/_material_design/icon/material_file_present_icon.py`

 * *Files identical despite different names*

### Comparing `apysc-4.4.2/apysc/_material_design/icon/material_filter_alt_icon.py` & `apysc-4.4.3/apysc/_material_design/icon/material_filter_alt_icon.py`

 * *Files identical despite different names*

### Comparing `apysc-4.4.2/apysc/_material_design/icon/material_filter_alt_outlined_icon.py` & `apysc-4.4.3/apysc/_material_design/icon/material_filter_alt_outlined_icon.py`

 * *Files identical despite different names*

### Comparing `apysc-4.4.2/apysc/_material_design/icon/material_filter_list_alt_icon.py` & `apysc-4.4.3/apysc/_material_design/icon/material_filter_list_alt_icon.py`

 * *Files identical despite different names*

### Comparing `apysc-4.4.2/apysc/_material_design/icon/material_filter_list_icon.py` & `apysc-4.4.3/apysc/_material_design/icon/material_filter_list_icon.py`

 * *Files identical despite different names*

### Comparing `apysc-4.4.2/apysc/_material_design/icon/material_filter_list_outlined_icon.py` & `apysc-4.4.3/apysc/_material_design/icon/material_filter_list_outlined_icon.py`

 * *Files identical despite different names*

### Comparing `apysc-4.4.2/apysc/_material_design/icon/material_find_in_page_icon.py` & `apysc-4.4.3/apysc/_material_design/icon/material_find_in_page_icon.py`

 * *Files identical despite different names*

### Comparing `apysc-4.4.2/apysc/_material_design/icon/material_find_in_page_outlined_icon.py` & `apysc-4.4.3/apysc/_material_design/icon/material_find_in_page_outlined_icon.py`

 * *Files identical despite different names*

### Comparing `apysc-4.4.2/apysc/_material_design/icon/material_find_replace_icon.py` & `apysc-4.4.3/apysc/_material_design/icon/material_find_replace_icon.py`

 * *Files identical despite different names*

### Comparing `apysc-4.4.2/apysc/_material_design/icon/material_find_replace_outlined_icon.py` & `apysc-4.4.3/apysc/_material_design/icon/material_find_replace_outlined_icon.py`

 * *Files identical despite different names*

### Comparing `apysc-4.4.2/apysc/_material_design/icon/material_fingerprint_icon.py` & `apysc-4.4.3/apysc/_material_design/icon/material_fingerprint_icon.py`

 * *Files identical despite different names*

### Comparing `apysc-4.4.2/apysc/_material_design/icon/material_fingerprint_outlined_icon.py` & `apysc-4.4.3/apysc/_material_design/icon/material_fingerprint_outlined_icon.py`

 * *Files identical despite different names*

### Comparing `apysc-4.4.2/apysc/_material_design/icon/material_fit_screen_icon.py` & `apysc-4.4.3/apysc/_material_design/icon/material_fit_screen_icon.py`

 * *Files identical despite different names*

### Comparing `apysc-4.4.2/apysc/_material_design/icon/material_flag_icon.py` & `apysc-4.4.3/apysc/_material_design/icon/material_flag_icon.py`

 * *Files identical despite different names*

### Comparing `apysc-4.4.2/apysc/_material_design/icon/material_flag_outlined_icon.py` & `apysc-4.4.3/apysc/_material_design/icon/material_flag_outlined_icon.py`

 * *Files identical despite different names*

### Comparing `apysc-4.4.2/apysc/_material_design/icon/material_flaky_icon.py` & `apysc-4.4.3/apysc/_material_design/icon/material_flaky_icon.py`

 * *Files identical despite different names*

### Comparing `apysc-4.4.2/apysc/_material_design/icon/material_flaky_outlined_icon.py` & `apysc-4.4.3/apysc/_material_design/icon/material_flaky_outlined_icon.py`

 * *Files identical despite different names*

### Comparing `apysc-4.4.2/apysc/_material_design/icon/material_flight_land_icon.py` & `apysc-4.4.3/apysc/_material_design/icon/material_flight_land_icon.py`

 * *Files identical despite different names*

### Comparing `apysc-4.4.2/apysc/_material_design/icon/material_flight_land_outlined_icon.py` & `apysc-4.4.3/apysc/_material_design/icon/material_flight_land_outlined_icon.py`

 * *Files identical despite different names*

### Comparing `apysc-4.4.2/apysc/_material_design/icon/material_flight_takeoff_icon.py` & `apysc-4.4.3/apysc/_material_design/icon/material_flight_takeoff_icon.py`

 * *Files identical despite different names*

### Comparing `apysc-4.4.2/apysc/_material_design/icon/material_flight_takeoff_outlined_icon.py` & `apysc-4.4.3/apysc/_material_design/icon/material_flight_takeoff_outlined_icon.py`

 * *Files identical despite different names*

### Comparing `apysc-4.4.2/apysc/_material_design/icon/material_flip_to_back_icon.py` & `apysc-4.4.3/apysc/_material_design/icon/material_flip_to_back_icon.py`

 * *Files identical despite different names*

### Comparing `apysc-4.4.2/apysc/_material_design/icon/material_flip_to_back_outlined_icon.py` & `apysc-4.4.3/apysc/_material_design/icon/material_flip_to_back_outlined_icon.py`

 * *Files identical despite different names*

### Comparing `apysc-4.4.2/apysc/_material_design/icon/material_flip_to_front_icon.py` & `apysc-4.4.3/apysc/_material_design/icon/material_flip_to_front_icon.py`

 * *Files identical despite different names*

### Comparing `apysc-4.4.2/apysc/_material_design/icon/material_flip_to_front_outlined_icon.py` & `apysc-4.4.3/apysc/_material_design/icon/material_flip_to_front_outlined_icon.py`

 * *Files identical despite different names*

### Comparing `apysc-4.4.2/apysc/_material_design/icon/material_font_download_icon.py` & `apysc-4.4.3/apysc/_material_design/icon/material_font_download_icon.py`

 * *Files identical despite different names*

### Comparing `apysc-4.4.2/apysc/_material_design/icon/material_font_download_outlined_icon.py` & `apysc-4.4.3/apysc/_material_design/icon/material_font_download_outlined_icon.py`

 * *Files identical despite different names*

### Comparing `apysc-4.4.2/apysc/_material_design/icon/material_forum_icon.py` & `apysc-4.4.3/apysc/_material_design/icon/material_forum_icon.py`

 * *Files identical despite different names*

### Comparing `apysc-4.4.2/apysc/_material_design/icon/material_forum_outlined_icon.py` & `apysc-4.4.3/apysc/_material_design/icon/material_forum_outlined_icon.py`

 * *Files identical despite different names*

### Comparing `apysc-4.4.2/apysc/_material_design/icon/material_forward_10_icon.py` & `apysc-4.4.3/apysc/_material_design/icon/material_forward_10_icon.py`

 * *Files identical despite different names*

### Comparing `apysc-4.4.2/apysc/_material_design/icon/material_forward_10_outlined_icon.py` & `apysc-4.4.3/apysc/_material_design/icon/material_forward_10_outlined_icon.py`

 * *Files identical despite different names*

### Comparing `apysc-4.4.2/apysc/_material_design/icon/material_forward_30_icon.py` & `apysc-4.4.3/apysc/_material_design/icon/material_forward_30_icon.py`

 * *Files identical despite different names*

### Comparing `apysc-4.4.2/apysc/_material_design/icon/material_forward_30_outlined_icon.py` & `apysc-4.4.3/apysc/_material_design/icon/material_forward_30_outlined_icon.py`

 * *Files identical despite different names*

### Comparing `apysc-4.4.2/apysc/_material_design/icon/material_forward_5_icon.py` & `apysc-4.4.3/apysc/_material_design/icon/material_forward_5_icon.py`

 * *Files identical despite different names*

### Comparing `apysc-4.4.2/apysc/_material_design/icon/material_forward_5_outlined_icon.py` & `apysc-4.4.3/apysc/_material_design/icon/material_forward_5_outlined_icon.py`

 * *Files identical despite different names*

### Comparing `apysc-4.4.2/apysc/_material_design/icon/material_forward_icon.py` & `apysc-4.4.3/apysc/_material_design/icon/material_forward_icon.py`

 * *Files identical despite different names*

### Comparing `apysc-4.4.2/apysc/_material_design/icon/material_forward_outlined_icon.py` & `apysc-4.4.3/apysc/_material_design/icon/material_forward_outlined_icon.py`

 * *Files identical despite different names*

### Comparing `apysc-4.4.2/apysc/_material_design/icon/material_forward_to_inbox_icon.py` & `apysc-4.4.3/apysc/_material_design/icon/material_forward_to_inbox_icon.py`

 * *Files identical despite different names*

### Comparing `apysc-4.4.2/apysc/_material_design/icon/material_forward_to_inbox_outlined_icon.py` & `apysc-4.4.3/apysc/_material_design/icon/material_forward_to_inbox_outlined_icon.py`

 * *Files identical despite different names*

### Comparing `apysc-4.4.2/apysc/_material_design/icon/material_g_translate_icon.py` & `apysc-4.4.3/apysc/_material_design/icon/material_g_translate_icon.py`

 * *Files identical despite different names*

### Comparing `apysc-4.4.2/apysc/_material_design/icon/material_g_translate_outlined_icon.py` & `apysc-4.4.3/apysc/_material_design/icon/material_g_translate_outlined_icon.py`

 * *Files identical despite different names*

### Comparing `apysc-4.4.2/apysc/_material_design/icon/material_games_icon.py` & `apysc-4.4.3/apysc/_material_design/icon/material_games_icon.py`

 * *Files identical despite different names*

### Comparing `apysc-4.4.2/apysc/_material_design/icon/material_games_outlined_icon.py` & `apysc-4.4.3/apysc/_material_design/icon/material_games_outlined_icon.py`

 * *Files identical despite different names*

### Comparing `apysc-4.4.2/apysc/_material_design/icon/material_gavel_icon.py` & `apysc-4.4.3/apysc/_material_design/icon/material_gavel_icon.py`

 * *Files identical despite different names*

### Comparing `apysc-4.4.2/apysc/_material_design/icon/material_gavel_outlined_icon.py` & `apysc-4.4.3/apysc/_material_design/icon/material_gavel_outlined_icon.py`

 * *Files identical despite different names*

### Comparing `apysc-4.4.2/apysc/_material_design/icon/material_gesture_icon.py` & `apysc-4.4.3/apysc/_material_design/icon/material_gesture_icon.py`

 * *Files identical despite different names*

### Comparing `apysc-4.4.2/apysc/_material_design/icon/material_gesture_outlined_icon.py` & `apysc-4.4.3/apysc/_material_design/icon/material_gesture_outlined_icon.py`

 * *Files identical despite different names*

### Comparing `apysc-4.4.2/apysc/_material_design/icon/material_get_app_icon.py` & `apysc-4.4.3/apysc/_material_design/icon/material_get_app_icon.py`

 * *Files identical despite different names*

### Comparing `apysc-4.4.2/apysc/_material_design/icon/material_get_app_outlined_icon.py` & `apysc-4.4.3/apysc/_material_design/icon/material_get_app_outlined_icon.py`

 * *Files identical despite different names*

### Comparing `apysc-4.4.2/apysc/_material_design/icon/material_gif_icon.py` & `apysc-4.4.3/apysc/_material_design/icon/material_gif_icon.py`

 * *Files identical despite different names*

### Comparing `apysc-4.4.2/apysc/_material_design/icon/material_gif_outlined_icon.py` & `apysc-4.4.3/apysc/_material_design/icon/material_gif_outlined_icon.py`

 * *Files identical despite different names*

### Comparing `apysc-4.4.2/apysc/_material_design/icon/material_grade_icon.py` & `apysc-4.4.3/apysc/_material_design/icon/material_grade_icon.py`

 * *Files identical despite different names*

### Comparing `apysc-4.4.2/apysc/_material_design/icon/material_grade_outlined_icon.py` & `apysc-4.4.3/apysc/_material_design/icon/material_grade_outlined_icon.py`

 * *Files identical despite different names*

### Comparing `apysc-4.4.2/apysc/_material_design/icon/material_grading_icon.py` & `apysc-4.4.3/apysc/_material_design/icon/material_grading_icon.py`

 * *Files identical despite different names*

### Comparing `apysc-4.4.2/apysc/_material_design/icon/material_grading_outlined_icon.py` & `apysc-4.4.3/apysc/_material_design/icon/material_grading_outlined_icon.py`

 * *Files identical despite different names*

### Comparing `apysc-4.4.2/apysc/_material_design/icon/material_group_work_icon.py` & `apysc-4.4.3/apysc/_material_design/icon/material_group_work_icon.py`

 * *Files identical despite different names*

### Comparing `apysc-4.4.2/apysc/_material_design/icon/material_group_work_outlined_icon.py` & `apysc-4.4.3/apysc/_material_design/icon/material_group_work_outlined_icon.py`

 * *Files identical despite different names*

### Comparing `apysc-4.4.2/apysc/_material_design/icon/material_hd_icon.py` & `apysc-4.4.3/apysc/_material_design/icon/material_hd_icon.py`

 * *Files identical despite different names*

### Comparing `apysc-4.4.2/apysc/_material_design/icon/material_hd_outlined_icon.py` & `apysc-4.4.3/apysc/_material_design/icon/material_hd_outlined_icon.py`

 * *Files identical despite different names*

### Comparing `apysc-4.4.2/apysc/_material_design/icon/material_hearing_disabled_icon.py` & `apysc-4.4.3/apysc/_material_design/icon/material_hearing_disabled_icon.py`

 * *Files identical despite different names*

### Comparing `apysc-4.4.2/apysc/_material_design/icon/material_hearing_disabled_outlined_icon.py` & `apysc-4.4.3/apysc/_material_design/icon/material_hearing_disabled_outlined_icon.py`

 * *Files identical despite different names*

### Comparing `apysc-4.4.2/apysc/_material_design/icon/material_hearing_icon.py` & `apysc-4.4.3/apysc/_material_design/icon/material_hearing_icon.py`

 * *Files identical despite different names*

### Comparing `apysc-4.4.2/apysc/_material_design/icon/material_hearing_outlined_icon.py` & `apysc-4.4.3/apysc/_material_design/icon/material_hearing_outlined_icon.py`

 * *Files identical despite different names*

### Comparing `apysc-4.4.2/apysc/_material_design/icon/material_help_center_icon.py` & `apysc-4.4.3/apysc/_material_design/icon/material_help_center_icon.py`

 * *Files identical despite different names*

### Comparing `apysc-4.4.2/apysc/_material_design/icon/material_help_center_outlined_icon.py` & `apysc-4.4.3/apysc/_material_design/icon/material_help_center_outlined_icon.py`

 * *Files identical despite different names*

### Comparing `apysc-4.4.2/apysc/_material_design/icon/material_help_icon.py` & `apysc-4.4.3/apysc/_material_design/icon/material_help_icon.py`

 * *Files identical despite different names*

### Comparing `apysc-4.4.2/apysc/_material_design/icon/material_help_outline_icon.py` & `apysc-4.4.3/apysc/_material_design/icon/material_help_outline_icon.py`

 * *Files identical despite different names*

### Comparing `apysc-4.4.2/apysc/_material_design/icon/material_help_outline_outlined_icon.py` & `apysc-4.4.3/apysc/_material_design/icon/material_help_outline_outlined_icon.py`

 * *Files identical despite different names*

### Comparing `apysc-4.4.2/apysc/_material_design/icon/material_help_outlined_icon.py` & `apysc-4.4.3/apysc/_material_design/icon/material_help_outlined_icon.py`

 * *Files identical despite different names*

### Comparing `apysc-4.4.2/apysc/_material_design/icon/material_high_quality_icon.py` & `apysc-4.4.3/apysc/_material_design/icon/material_high_quality_icon.py`

 * *Files identical despite different names*

### Comparing `apysc-4.4.2/apysc/_material_design/icon/material_high_quality_outlined_icon.py` & `apysc-4.4.3/apysc/_material_design/icon/material_high_quality_outlined_icon.py`

 * *Files identical despite different names*

### Comparing `apysc-4.4.2/apysc/_material_design/icon/material_highlight_alt_icon.py` & `apysc-4.4.3/apysc/_material_design/icon/material_highlight_alt_icon.py`

 * *Files identical despite different names*

### Comparing `apysc-4.4.2/apysc/_material_design/icon/material_highlight_alt_outlined_icon.py` & `apysc-4.4.3/apysc/_material_design/icon/material_highlight_alt_outlined_icon.py`

 * *Files identical despite different names*

### Comparing `apysc-4.4.2/apysc/_material_design/icon/material_highlight_off_icon.py` & `apysc-4.4.3/apysc/_material_design/icon/material_highlight_off_icon.py`

 * *Files identical despite different names*

### Comparing `apysc-4.4.2/apysc/_material_design/icon/material_highlight_off_outlined_icon.py` & `apysc-4.4.3/apysc/_material_design/icon/material_highlight_off_outlined_icon.py`

 * *Files identical despite different names*

### Comparing `apysc-4.4.2/apysc/_material_design/icon/material_history_icon.py` & `apysc-4.4.3/apysc/_material_design/icon/material_history_icon.py`

 * *Files identical despite different names*

### Comparing `apysc-4.4.2/apysc/_material_design/icon/material_history_outlined_icon.py` & `apysc-4.4.3/apysc/_material_design/icon/material_history_outlined_icon.py`

 * *Files identical despite different names*

### Comparing `apysc-4.4.2/apysc/_material_design/icon/material_history_toggle_off_icon.py` & `apysc-4.4.3/apysc/_material_design/icon/material_history_toggle_off_icon.py`

 * *Files identical despite different names*

### Comparing `apysc-4.4.2/apysc/_material_design/icon/material_history_toggle_off_outlined_icon.py` & `apysc-4.4.3/apysc/_material_design/icon/material_history_toggle_off_outlined_icon.py`

 * *Files identical despite different names*

### Comparing `apysc-4.4.2/apysc/_material_design/icon/material_home_filled_icon.py` & `apysc-4.4.3/apysc/_material_design/icon/material_home_filled_icon.py`

 * *Files identical despite different names*

### Comparing `apysc-4.4.2/apysc/_material_design/icon/material_home_icon.py` & `apysc-4.4.3/apysc/_material_design/icon/material_home_icon.py`

 * *Files identical despite different names*

### Comparing `apysc-4.4.2/apysc/_material_design/icon/material_home_outlined_icon.py` & `apysc-4.4.3/apysc/_material_design/icon/material_home_outlined_icon.py`

 * *Files identical despite different names*

### Comparing `apysc-4.4.2/apysc/_material_design/icon/material_horizontal_split_icon.py` & `apysc-4.4.3/apysc/_material_design/icon/material_horizontal_split_icon.py`

 * *Files identical despite different names*

### Comparing `apysc-4.4.2/apysc/_material_design/icon/material_horizontal_split_outlined_icon.py` & `apysc-4.4.3/apysc/_material_design/icon/material_horizontal_split_outlined_icon.py`

 * *Files identical despite different names*

### Comparing `apysc-4.4.2/apysc/_material_design/icon/material_hourglass_bottom_icon.py` & `apysc-4.4.3/apysc/_material_design/icon/material_hourglass_bottom_icon.py`

 * *Files identical despite different names*

### Comparing `apysc-4.4.2/apysc/_material_design/icon/material_hourglass_bottom_outlined_icon.py` & `apysc-4.4.3/apysc/_material_design/icon/material_hourglass_bottom_outlined_icon.py`

 * *Files identical despite different names*

### Comparing `apysc-4.4.2/apysc/_material_design/icon/material_hourglass_disabled_icon.py` & `apysc-4.4.3/apysc/_material_design/icon/material_hourglass_disabled_icon.py`

 * *Files identical despite different names*

### Comparing `apysc-4.4.2/apysc/_material_design/icon/material_hourglass_disabled_outlined_icon.py` & `apysc-4.4.3/apysc/_material_design/icon/material_hourglass_disabled_outlined_icon.py`

 * *Files identical despite different names*

### Comparing `apysc-4.4.2/apysc/_material_design/icon/material_hourglass_empty_icon.py` & `apysc-4.4.3/apysc/_material_design/icon/material_hourglass_empty_icon.py`

 * *Files identical despite different names*

### Comparing `apysc-4.4.2/apysc/_material_design/icon/material_hourglass_empty_outlined_icon.py` & `apysc-4.4.3/apysc/_material_design/icon/material_hourglass_empty_outlined_icon.py`

 * *Files identical despite different names*

### Comparing `apysc-4.4.2/apysc/_material_design/icon/material_hourglass_full_icon.py` & `apysc-4.4.3/apysc/_material_design/icon/material_hourglass_full_icon.py`

 * *Files identical despite different names*

### Comparing `apysc-4.4.2/apysc/_material_design/icon/material_hourglass_full_outlined_icon.py` & `apysc-4.4.3/apysc/_material_design/icon/material_hourglass_full_outlined_icon.py`

 * *Files identical despite different names*

### Comparing `apysc-4.4.2/apysc/_material_design/icon/material_hourglass_top_icon.py` & `apysc-4.4.3/apysc/_material_design/icon/material_hourglass_top_icon.py`

 * *Files identical despite different names*

### Comparing `apysc-4.4.2/apysc/_material_design/icon/material_hourglass_top_outlined_icon.py` & `apysc-4.4.3/apysc/_material_design/icon/material_hourglass_top_outlined_icon.py`

 * *Files identical despite different names*

### Comparing `apysc-4.4.2/apysc/_material_design/icon/material_how_to_reg_icon.py` & `apysc-4.4.3/apysc/_material_design/icon/material_how_to_reg_icon.py`

 * *Files identical despite different names*

### Comparing `apysc-4.4.2/apysc/_material_design/icon/material_how_to_reg_outlined_icon.py` & `apysc-4.4.3/apysc/_material_design/icon/material_how_to_reg_outlined_icon.py`

 * *Files identical despite different names*

### Comparing `apysc-4.4.2/apysc/_material_design/icon/material_how_to_vote_icon.py` & `apysc-4.4.3/apysc/_material_design/icon/material_how_to_vote_icon.py`

 * *Files identical despite different names*

### Comparing `apysc-4.4.2/apysc/_material_design/icon/material_how_to_vote_outlined_icon.py` & `apysc-4.4.3/apysc/_material_design/icon/material_how_to_vote_outlined_icon.py`

 * *Files identical despite different names*

### Comparing `apysc-4.4.2/apysc/_material_design/icon/material_http_icon.py` & `apysc-4.4.3/apysc/_material_design/icon/material_http_icon.py`

 * *Files identical despite different names*

### Comparing `apysc-4.4.2/apysc/_material_design/icon/material_http_outlined_icon.py` & `apysc-4.4.3/apysc/_material_design/icon/material_http_outlined_icon.py`

 * *Files identical despite different names*

### Comparing `apysc-4.4.2/apysc/_material_design/icon/material_https_icon.py` & `apysc-4.4.3/apysc/_material_design/icon/material_https_icon.py`

 * *Files identical despite different names*

### Comparing `apysc-4.4.2/apysc/_material_design/icon/material_https_outlined_icon.py` & `apysc-4.4.3/apysc/_material_design/icon/material_https_outlined_icon.py`

 * *Files identical despite different names*

### Comparing `apysc-4.4.2/apysc/_material_design/icon/material_import_contacts_icon.py` & `apysc-4.4.3/apysc/_material_design/icon/material_import_contacts_icon.py`

 * *Files identical despite different names*

### Comparing `apysc-4.4.2/apysc/_material_design/icon/material_import_contacts_outlined_icon.py` & `apysc-4.4.3/apysc/_material_design/icon/material_import_contacts_outlined_icon.py`

 * *Files identical despite different names*

### Comparing `apysc-4.4.2/apysc/_material_design/icon/material_import_export_icon.py` & `apysc-4.4.3/apysc/_material_design/icon/material_import_export_icon.py`

 * *Files identical despite different names*

### Comparing `apysc-4.4.2/apysc/_material_design/icon/material_import_export_outlined_icon.py` & `apysc-4.4.3/apysc/_material_design/icon/material_import_export_outlined_icon.py`

 * *Files identical despite different names*

### Comparing `apysc-4.4.2/apysc/_material_design/icon/material_important_devices_icon.py` & `apysc-4.4.3/apysc/_material_design/icon/material_important_devices_icon.py`

 * *Files identical despite different names*

### Comparing `apysc-4.4.2/apysc/_material_design/icon/material_important_devices_outlined_icon.py` & `apysc-4.4.3/apysc/_material_design/icon/material_important_devices_outlined_icon.py`

 * *Files identical despite different names*

### Comparing `apysc-4.4.2/apysc/_material_design/icon/material_inbox_icon.py` & `apysc-4.4.3/apysc/_material_design/icon/material_inbox_icon.py`

 * *Files identical despite different names*

### Comparing `apysc-4.4.2/apysc/_material_design/icon/material_inbox_outlined_icon.py` & `apysc-4.4.3/apysc/_material_design/icon/material_inbox_outlined_icon.py`

 * *Files identical despite different names*

### Comparing `apysc-4.4.2/apysc/_material_design/icon/material_info_icon.py` & `apysc-4.4.3/apysc/_material_design/icon/material_info_icon.py`

 * *Files identical despite different names*

### Comparing `apysc-4.4.2/apysc/_material_design/icon/material_info_outline_icon.py` & `apysc-4.4.3/apysc/_material_design/icon/material_info_outline_icon.py`

 * *Files identical despite different names*

### Comparing `apysc-4.4.2/apysc/_material_design/icon/material_info_outlined_icon.py` & `apysc-4.4.3/apysc/_material_design/icon/material_info_outlined_icon.py`

 * *Files identical despite different names*

### Comparing `apysc-4.4.2/apysc/_material_design/icon/material_input_icon.py` & `apysc-4.4.3/apysc/_material_design/icon/material_input_icon.py`

 * *Files identical despite different names*

### Comparing `apysc-4.4.2/apysc/_material_design/icon/material_input_outlined_icon.py` & `apysc-4.4.3/apysc/_material_design/icon/material_input_outlined_icon.py`

 * *Files identical despite different names*

### Comparing `apysc-4.4.2/apysc/_material_design/icon/material_insights_icon.py` & `apysc-4.4.3/apysc/_material_design/icon/material_insights_icon.py`

 * *Files identical despite different names*

### Comparing `apysc-4.4.2/apysc/_material_design/icon/material_insights_outlined_icon.py` & `apysc-4.4.3/apysc/_material_design/icon/material_insights_outlined_icon.py`

 * *Files identical despite different names*

### Comparing `apysc-4.4.2/apysc/_material_design/icon/material_integration_instructions_icon.py` & `apysc-4.4.3/apysc/_material_design/icon/material_integration_instructions_icon.py`

 * *Files identical despite different names*

### Comparing `apysc-4.4.2/apysc/_material_design/icon/material_integration_instructions_outlined_icon.py` & `apysc-4.4.3/apysc/_material_design/icon/material_integration_instructions_outlined_icon.py`

 * *Files identical despite different names*

### Comparing `apysc-4.4.2/apysc/_material_design/icon/material_inventory_icon.py` & `apysc-4.4.3/apysc/_material_design/icon/material_inventory_icon.py`

 * *Files identical despite different names*

### Comparing `apysc-4.4.2/apysc/_material_design/icon/material_invert_colors_icon.py` & `apysc-4.4.3/apysc/_material_design/icon/material_invert_colors_icon.py`

 * *Files identical despite different names*

### Comparing `apysc-4.4.2/apysc/_material_design/icon/material_invert_colors_off_icon.py` & `apysc-4.4.3/apysc/_material_design/icon/material_invert_colors_off_icon.py`

 * *Files identical despite different names*

### Comparing `apysc-4.4.2/apysc/_material_design/icon/material_invert_colors_off_outlined_icon.py` & `apysc-4.4.3/apysc/_material_design/icon/material_invert_colors_off_outlined_icon.py`

 * *Files identical despite different names*

### Comparing `apysc-4.4.2/apysc/_material_design/icon/material_invert_colors_outlined_icon.py` & `apysc-4.4.3/apysc/_material_design/icon/material_invert_colors_outlined_icon.py`

 * *Files identical despite different names*

### Comparing `apysc-4.4.2/apysc/_material_design/icon/material_label_icon.py` & `apysc-4.4.3/apysc/_material_design/icon/material_label_icon.py`

 * *Files identical despite different names*

### Comparing `apysc-4.4.2/apysc/_material_design/icon/material_label_important_icon.py` & `apysc-4.4.3/apysc/_material_design/icon/material_label_important_icon.py`

 * *Files identical despite different names*

### Comparing `apysc-4.4.2/apysc/_material_design/icon/material_label_important_outline_icon.py` & `apysc-4.4.3/apysc/_material_design/icon/material_label_important_outline_icon.py`

 * *Files identical despite different names*

### Comparing `apysc-4.4.2/apysc/_material_design/icon/material_label_important_outlined_icon.py` & `apysc-4.4.3/apysc/_material_design/icon/material_label_important_outlined_icon.py`

 * *Files identical despite different names*

### Comparing `apysc-4.4.2/apysc/_material_design/icon/material_label_off_icon.py` & `apysc-4.4.3/apysc/_material_design/icon/material_label_off_icon.py`

 * *Files identical despite different names*

### Comparing `apysc-4.4.2/apysc/_material_design/icon/material_label_off_outlined_icon.py` & `apysc-4.4.3/apysc/_material_design/icon/material_label_off_outlined_icon.py`

 * *Files identical despite different names*

### Comparing `apysc-4.4.2/apysc/_material_design/icon/material_label_outline_icon.py` & `apysc-4.4.3/apysc/_material_design/icon/material_label_outline_icon.py`

 * *Files identical despite different names*

### Comparing `apysc-4.4.2/apysc/_material_design/icon/material_label_outlined_icon.py` & `apysc-4.4.3/apysc/_material_design/icon/material_label_outlined_icon.py`

 * *Files identical despite different names*

### Comparing `apysc-4.4.2/apysc/_material_design/icon/material_language_icon.py` & `apysc-4.4.3/apysc/_material_design/icon/material_language_icon.py`

 * *Files identical despite different names*

### Comparing `apysc-4.4.2/apysc/_material_design/icon/material_language_outlined_icon.py` & `apysc-4.4.3/apysc/_material_design/icon/material_language_outlined_icon.py`

 * *Files identical despite different names*

### Comparing `apysc-4.4.2/apysc/_material_design/icon/material_launch_icon.py` & `apysc-4.4.3/apysc/_material_design/icon/material_launch_icon.py`

 * *Files identical despite different names*

### Comparing `apysc-4.4.2/apysc/_material_design/icon/material_launch_outlined_icon.py` & `apysc-4.4.3/apysc/_material_design/icon/material_launch_outlined_icon.py`

 * *Files identical despite different names*

### Comparing `apysc-4.4.2/apysc/_material_design/icon/material_leaderboard_icon.py` & `apysc-4.4.3/apysc/_material_design/icon/material_leaderboard_icon.py`

 * *Files identical despite different names*

### Comparing `apysc-4.4.2/apysc/_material_design/icon/material_leaderboard_outlined_icon.py` & `apysc-4.4.3/apysc/_material_design/icon/material_leaderboard_outlined_icon.py`

 * *Files identical despite different names*

### Comparing `apysc-4.4.2/apysc/_material_design/icon/material_library_add_check_icon.py` & `apysc-4.4.3/apysc/_material_design/icon/material_library_add_check_icon.py`

 * *Files identical despite different names*

### Comparing `apysc-4.4.2/apysc/_material_design/icon/material_library_add_check_outlined_icon.py` & `apysc-4.4.3/apysc/_material_design/icon/material_library_add_check_outlined_icon.py`

 * *Files identical despite different names*

### Comparing `apysc-4.4.2/apysc/_material_design/icon/material_library_add_icon.py` & `apysc-4.4.3/apysc/_material_design/icon/material_library_add_icon.py`

 * *Files identical despite different names*

### Comparing `apysc-4.4.2/apysc/_material_design/icon/material_library_add_outlined_icon.py` & `apysc-4.4.3/apysc/_material_design/icon/material_library_add_outlined_icon.py`

 * *Files identical despite different names*

### Comparing `apysc-4.4.2/apysc/_material_design/icon/material_library_books_icon.py` & `apysc-4.4.3/apysc/_material_design/icon/material_library_books_icon.py`

 * *Files identical despite different names*

### Comparing `apysc-4.4.2/apysc/_material_design/icon/material_library_books_outlined_icon.py` & `apysc-4.4.3/apysc/_material_design/icon/material_library_books_outlined_icon.py`

 * *Files identical despite different names*

### Comparing `apysc-4.4.2/apysc/_material_design/icon/material_library_music_icon.py` & `apysc-4.4.3/apysc/_material_design/icon/material_library_music_icon.py`

 * *Files identical despite different names*

### Comparing `apysc-4.4.2/apysc/_material_design/icon/material_library_music_outlined_icon.py` & `apysc-4.4.3/apysc/_material_design/icon/material_library_music_outlined_icon.py`

 * *Files identical despite different names*

### Comparing `apysc-4.4.2/apysc/_material_design/icon/material_lightbulb_icon.py` & `apysc-4.4.3/apysc/_material_design/icon/material_lightbulb_icon.py`

 * *Files identical despite different names*

### Comparing `apysc-4.4.2/apysc/_material_design/icon/material_lightbulb_outline_icon.py` & `apysc-4.4.3/apysc/_material_design/icon/material_lightbulb_outline_icon.py`

 * *Files identical despite different names*

### Comparing `apysc-4.4.2/apysc/_material_design/icon/material_lightbulb_outlined_icon.py` & `apysc-4.4.3/apysc/_material_design/icon/material_lightbulb_outlined_icon.py`

 * *Files identical despite different names*

### Comparing `apysc-4.4.2/apysc/_material_design/icon/material_line_style_icon.py` & `apysc-4.4.3/apysc/_material_design/icon/material_line_style_icon.py`

 * *Files identical despite different names*

### Comparing `apysc-4.4.2/apysc/_material_design/icon/material_line_style_outlined_icon.py` & `apysc-4.4.3/apysc/_material_design/icon/material_line_style_outlined_icon.py`

 * *Files identical despite different names*

### Comparing `apysc-4.4.2/apysc/_material_design/icon/material_line_weight_icon.py` & `apysc-4.4.3/apysc/_material_design/icon/material_line_weight_icon.py`

 * *Files identical despite different names*

### Comparing `apysc-4.4.2/apysc/_material_design/icon/material_line_weight_outlined_icon.py` & `apysc-4.4.3/apysc/_material_design/icon/material_line_weight_outlined_icon.py`

 * *Files identical despite different names*

### Comparing `apysc-4.4.2/apysc/_material_design/icon/material_link_icon.py` & `apysc-4.4.3/apysc/_material_design/icon/material_link_icon.py`

 * *Files identical despite different names*

### Comparing `apysc-4.4.2/apysc/_material_design/icon/material_link_off_icon.py` & `apysc-4.4.3/apysc/_material_design/icon/material_link_off_icon.py`

 * *Files identical despite different names*

### Comparing `apysc-4.4.2/apysc/_material_design/icon/material_link_off_outlined_icon.py` & `apysc-4.4.3/apysc/_material_design/icon/material_link_off_outlined_icon.py`

 * *Files identical despite different names*

### Comparing `apysc-4.4.2/apysc/_material_design/icon/material_link_outlined_icon.py` & `apysc-4.4.3/apysc/_material_design/icon/material_link_outlined_icon.py`

 * *Files identical despite different names*

### Comparing `apysc-4.4.2/apysc/_material_design/icon/material_list_alt_icon.py` & `apysc-4.4.3/apysc/_material_design/icon/material_list_alt_icon.py`

 * *Files identical despite different names*

### Comparing `apysc-4.4.2/apysc/_material_design/icon/material_list_alt_outlined_icon.py` & `apysc-4.4.3/apysc/_material_design/icon/material_list_alt_outlined_icon.py`

 * *Files identical despite different names*

### Comparing `apysc-4.4.2/apysc/_material_design/icon/material_list_icon.py` & `apysc-4.4.3/apysc/_material_design/icon/material_list_icon.py`

 * *Files identical despite different names*

### Comparing `apysc-4.4.2/apysc/_material_design/icon/material_list_outlined_icon.py` & `apysc-4.4.3/apysc/_material_design/icon/material_list_outlined_icon.py`

 * *Files identical despite different names*

### Comparing `apysc-4.4.2/apysc/_material_design/icon/material_live_help_icon.py` & `apysc-4.4.3/apysc/_material_design/icon/material_live_help_icon.py`

 * *Files identical despite different names*

### Comparing `apysc-4.4.2/apysc/_material_design/icon/material_live_help_outlined_icon.py` & `apysc-4.4.3/apysc/_material_design/icon/material_live_help_outlined_icon.py`

 * *Files identical despite different names*

### Comparing `apysc-4.4.2/apysc/_material_design/icon/material_location_off_icon.py` & `apysc-4.4.3/apysc/_material_design/icon/material_location_off_icon.py`

 * *Files identical despite different names*

### Comparing `apysc-4.4.2/apysc/_material_design/icon/material_location_off_outlined_icon.py` & `apysc-4.4.3/apysc/_material_design/icon/material_location_off_outlined_icon.py`

 * *Files identical despite different names*

### Comparing `apysc-4.4.2/apysc/_material_design/icon/material_location_on_icon.py` & `apysc-4.4.3/apysc/_material_design/icon/material_location_on_icon.py`

 * *Files identical despite different names*

### Comparing `apysc-4.4.2/apysc/_material_design/icon/material_location_on_outlined_icon.py` & `apysc-4.4.3/apysc/_material_design/icon/material_location_on_outlined_icon.py`

 * *Files identical despite different names*

### Comparing `apysc-4.4.2/apysc/_material_design/icon/material_lock_clock_icon.py` & `apysc-4.4.3/apysc/_material_design/icon/material_lock_clock_icon.py`

 * *Files identical despite different names*

### Comparing `apysc-4.4.2/apysc/_material_design/icon/material_lock_icon.py` & `apysc-4.4.3/apysc/_material_design/icon/material_lock_icon.py`

 * *Files identical despite different names*

### Comparing `apysc-4.4.2/apysc/_material_design/icon/material_lock_open_icon.py` & `apysc-4.4.3/apysc/_material_design/icon/material_lock_open_icon.py`

 * *Files identical despite different names*

### Comparing `apysc-4.4.2/apysc/_material_design/icon/material_lock_open_outlined_icon.py` & `apysc-4.4.3/apysc/_material_design/icon/material_lock_open_outlined_icon.py`

 * *Files identical despite different names*

### Comparing `apysc-4.4.2/apysc/_material_design/icon/material_lock_outline_icon.py` & `apysc-4.4.3/apysc/_material_design/icon/material_lock_outline_icon.py`

 * *Files identical despite different names*

### Comparing `apysc-4.4.2/apysc/_material_design/icon/material_lock_outlined_icon.py` & `apysc-4.4.3/apysc/_material_design/icon/material_lock_outlined_icon.py`

 * *Files identical despite different names*

### Comparing `apysc-4.4.2/apysc/_material_design/icon/material_login_icon.py` & `apysc-4.4.3/apysc/_material_design/icon/material_login_icon.py`

 * *Files identical despite different names*

### Comparing `apysc-4.4.2/apysc/_material_design/icon/material_login_outlined_icon.py` & `apysc-4.4.3/apysc/_material_design/icon/material_login_outlined_icon.py`

 * *Files identical despite different names*

### Comparing `apysc-4.4.2/apysc/_material_design/icon/material_logout_icon.py` & `apysc-4.4.3/apysc/_material_design/icon/material_logout_icon.py`

 * *Files identical despite different names*

### Comparing `apysc-4.4.2/apysc/_material_design/icon/material_loop_icon.py` & `apysc-4.4.3/apysc/_material_design/icon/material_loop_icon.py`

 * *Files identical despite different names*

### Comparing `apysc-4.4.2/apysc/_material_design/icon/material_loop_outlined_icon.py` & `apysc-4.4.3/apysc/_material_design/icon/material_loop_outlined_icon.py`

 * *Files identical despite different names*

### Comparing `apysc-4.4.2/apysc/_material_design/icon/material_low_priority_icon.py` & `apysc-4.4.3/apysc/_material_design/icon/material_low_priority_icon.py`

 * *Files identical despite different names*

### Comparing `apysc-4.4.2/apysc/_material_design/icon/material_low_priority_outlined_icon.py` & `apysc-4.4.3/apysc/_material_design/icon/material_low_priority_outlined_icon.py`

 * *Files identical despite different names*

### Comparing `apysc-4.4.2/apysc/_material_design/icon/material_loyalty_icon.py` & `apysc-4.4.3/apysc/_material_design/icon/material_loyalty_icon.py`

 * *Files identical despite different names*

### Comparing `apysc-4.4.2/apysc/_material_design/icon/material_loyalty_outlined_icon.py` & `apysc-4.4.3/apysc/_material_design/icon/material_loyalty_outlined_icon.py`

 * *Files identical despite different names*

### Comparing `apysc-4.4.2/apysc/_material_design/icon/material_mail_icon.py` & `apysc-4.4.3/apysc/_material_design/icon/material_mail_icon.py`

 * *Files identical despite different names*

### Comparing `apysc-4.4.2/apysc/_material_design/icon/material_mail_outline_icon.py` & `apysc-4.4.3/apysc/_material_design/icon/material_mail_outline_icon.py`

 * *Files identical despite different names*

### Comparing `apysc-4.4.2/apysc/_material_design/icon/material_mail_outline_outlined_icon.py` & `apysc-4.4.3/apysc/_material_design/icon/material_mail_outline_outlined_icon.py`

 * *Files identical despite different names*

### Comparing `apysc-4.4.2/apysc/_material_design/icon/material_mail_outlined_icon.py` & `apysc-4.4.3/apysc/_material_design/icon/material_mail_outlined_icon.py`

 * *Files identical despite different names*

### Comparing `apysc-4.4.2/apysc/_material_design/icon/material_mark_as_unread_icon.py` & `apysc-4.4.3/apysc/_material_design/icon/material_mark_as_unread_icon.py`

 * *Files identical despite different names*

### Comparing `apysc-4.4.2/apysc/_material_design/icon/material_mark_chat_read_icon.py` & `apysc-4.4.3/apysc/_material_design/icon/material_mark_chat_read_icon.py`

 * *Files identical despite different names*

### Comparing `apysc-4.4.2/apysc/_material_design/icon/material_mark_chat_read_outlined_icon.py` & `apysc-4.4.3/apysc/_material_design/icon/material_mark_chat_read_outlined_icon.py`

 * *Files identical despite different names*

### Comparing `apysc-4.4.2/apysc/_material_design/icon/material_mark_chat_unread_icon.py` & `apysc-4.4.3/apysc/_material_design/icon/material_mark_chat_unread_icon.py`

 * *Files identical despite different names*

### Comparing `apysc-4.4.2/apysc/_material_design/icon/material_mark_chat_unread_outlined_icon.py` & `apysc-4.4.3/apysc/_material_design/icon/material_mark_chat_unread_outlined_icon.py`

 * *Files identical despite different names*

### Comparing `apysc-4.4.2/apysc/_material_design/icon/material_mark_email_read_icon.py` & `apysc-4.4.3/apysc/_material_design/icon/material_mark_email_read_icon.py`

 * *Files identical despite different names*

### Comparing `apysc-4.4.2/apysc/_material_design/icon/material_mark_email_read_outlined_icon.py` & `apysc-4.4.3/apysc/_material_design/icon/material_mark_email_read_outlined_icon.py`

 * *Files identical despite different names*

### Comparing `apysc-4.4.2/apysc/_material_design/icon/material_mark_email_unread_icon.py` & `apysc-4.4.3/apysc/_material_design/icon/material_mark_email_unread_icon.py`

 * *Files identical despite different names*

### Comparing `apysc-4.4.2/apysc/_material_design/icon/material_mark_email_unread_outlined_icon.py` & `apysc-4.4.3/apysc/_material_design/icon/material_mark_email_unread_outlined_icon.py`

 * *Files identical despite different names*

### Comparing `apysc-4.4.2/apysc/_material_design/icon/material_markunread_icon.py` & `apysc-4.4.3/apysc/_material_design/icon/material_markunread_icon.py`

 * *Files identical despite different names*

### Comparing `apysc-4.4.2/apysc/_material_design/icon/material_markunread_mailbox_icon.py` & `apysc-4.4.3/apysc/_material_design/icon/material_markunread_mailbox_icon.py`

 * *Files identical despite different names*

### Comparing `apysc-4.4.2/apysc/_material_design/icon/material_markunread_mailbox_outlined_icon.py` & `apysc-4.4.3/apysc/_material_design/icon/material_markunread_mailbox_outlined_icon.py`

 * *Files identical despite different names*

### Comparing `apysc-4.4.2/apysc/_material_design/icon/material_markunread_outlined_icon.py` & `apysc-4.4.3/apysc/_material_design/icon/material_markunread_outlined_icon.py`

 * *Files identical despite different names*

### Comparing `apysc-4.4.2/apysc/_material_design/icon/material_maximize_icon.py` & `apysc-4.4.3/apysc/_material_design/icon/material_maximize_icon.py`

 * *Files identical despite different names*

### Comparing `apysc-4.4.2/apysc/_material_design/icon/material_maximize_outlined_icon.py` & `apysc-4.4.3/apysc/_material_design/icon/material_maximize_outlined_icon.py`

 * *Files identical despite different names*

### Comparing `apysc-4.4.2/apysc/_material_design/icon/material_mediation_icon.py` & `apysc-4.4.3/apysc/_material_design/icon/material_mediation_icon.py`

 * *Files identical despite different names*

### Comparing `apysc-4.4.2/apysc/_material_design/icon/material_mediation_outlined_icon.py` & `apysc-4.4.3/apysc/_material_design/icon/material_mediation_outlined_icon.py`

 * *Files identical despite different names*

### Comparing `apysc-4.4.2/apysc/_material_design/icon/material_message_icon.py` & `apysc-4.4.3/apysc/_material_design/icon/material_message_icon.py`

 * *Files identical despite different names*

### Comparing `apysc-4.4.2/apysc/_material_design/icon/material_message_outlined_icon.py` & `apysc-4.4.3/apysc/_material_design/icon/material_message_outlined_icon.py`

 * *Files identical despite different names*

### Comparing `apysc-4.4.2/apysc/_material_design/icon/material_mic_icon.py` & `apysc-4.4.3/apysc/_material_design/icon/material_mic_icon.py`

 * *Files identical despite different names*

### Comparing `apysc-4.4.2/apysc/_material_design/icon/material_mic_none_icon.py` & `apysc-4.4.3/apysc/_material_design/icon/material_mic_none_icon.py`

 * *Files identical despite different names*

### Comparing `apysc-4.4.2/apysc/_material_design/icon/material_mic_none_outlined_icon.py` & `apysc-4.4.3/apysc/_material_design/icon/material_mic_none_outlined_icon.py`

 * *Files identical despite different names*

### Comparing `apysc-4.4.2/apysc/_material_design/icon/material_mic_off_icon.py` & `apysc-4.4.3/apysc/_material_design/icon/material_mic_off_icon.py`

 * *Files identical despite different names*

### Comparing `apysc-4.4.2/apysc/_material_design/icon/material_mic_off_outlined_icon.py` & `apysc-4.4.3/apysc/_material_design/icon/material_mic_off_outlined_icon.py`

 * *Files identical despite different names*

### Comparing `apysc-4.4.2/apysc/_material_design/icon/material_mic_outlined_icon.py` & `apysc-4.4.3/apysc/_material_design/icon/material_mic_outlined_icon.py`

 * *Files identical despite different names*

### Comparing `apysc-4.4.2/apysc/_material_design/icon/material_minimize_icon.py` & `apysc-4.4.3/apysc/_material_design/icon/material_minimize_icon.py`

 * *Files identical despite different names*

### Comparing `apysc-4.4.2/apysc/_material_design/icon/material_minimize_outlined_icon.py` & `apysc-4.4.3/apysc/_material_design/icon/material_minimize_outlined_icon.py`

 * *Files identical despite different names*

### Comparing `apysc-4.4.2/apysc/_material_design/icon/material_missed_video_call_icon.py` & `apysc-4.4.3/apysc/_material_design/icon/material_missed_video_call_icon.py`

 * *Files identical despite different names*

### Comparing `apysc-4.4.2/apysc/_material_design/icon/material_missed_video_call_outlined_icon.py` & `apysc-4.4.3/apysc/_material_design/icon/material_missed_video_call_outlined_icon.py`

 * *Files identical despite different names*

### Comparing `apysc-4.4.2/apysc/_material_design/icon/material_mobile_screen_share_icon.py` & `apysc-4.4.3/apysc/_material_design/icon/material_mobile_screen_share_icon.py`

 * *Files identical despite different names*

### Comparing `apysc-4.4.2/apysc/_material_design/icon/material_mobile_screen_share_outlined_icon.py` & `apysc-4.4.3/apysc/_material_design/icon/material_mobile_screen_share_outlined_icon.py`

 * *Files identical despite different names*

### Comparing `apysc-4.4.2/apysc/_material_design/icon/material_model_training_icon.py` & `apysc-4.4.3/apysc/_material_design/icon/material_model_training_icon.py`

 * *Files identical despite different names*

### Comparing `apysc-4.4.2/apysc/_material_design/icon/material_model_training_outlined_icon.py` & `apysc-4.4.3/apysc/_material_design/icon/material_model_training_outlined_icon.py`

 * *Files identical despite different names*

### Comparing `apysc-4.4.2/apysc/_material_design/icon/material_more_time_icon.py` & `apysc-4.4.3/apysc/_material_design/icon/material_more_time_icon.py`

 * *Files identical despite different names*

### Comparing `apysc-4.4.2/apysc/_material_design/icon/material_more_time_outlined_icon.py` & `apysc-4.4.3/apysc/_material_design/icon/material_more_time_outlined_icon.py`

 * *Files identical despite different names*

### Comparing `apysc-4.4.2/apysc/_material_design/icon/material_move_to_inbox_icon.py` & `apysc-4.4.3/apysc/_material_design/icon/material_move_to_inbox_icon.py`

 * *Files identical despite different names*

### Comparing `apysc-4.4.2/apysc/_material_design/icon/material_move_to_inbox_outlined_icon.py` & `apysc-4.4.3/apysc/_material_design/icon/material_move_to_inbox_outlined_icon.py`

 * *Files identical despite different names*

### Comparing `apysc-4.4.2/apysc/_material_design/icon/material_movie_icon.py` & `apysc-4.4.3/apysc/_material_design/icon/material_movie_icon.py`

 * *Files identical despite different names*

### Comparing `apysc-4.4.2/apysc/_material_design/icon/material_movie_outlined_icon.py` & `apysc-4.4.3/apysc/_material_design/icon/material_movie_outlined_icon.py`

 * *Files identical despite different names*

### Comparing `apysc-4.4.2/apysc/_material_design/icon/material_music_video_icon.py` & `apysc-4.4.3/apysc/_material_design/icon/material_music_video_icon.py`

 * *Files identical despite different names*

### Comparing `apysc-4.4.2/apysc/_material_design/icon/material_music_video_outlined_icon.py` & `apysc-4.4.3/apysc/_material_design/icon/material_music_video_outlined_icon.py`

 * *Files identical despite different names*

### Comparing `apysc-4.4.2/apysc/_material_design/icon/material_nat_icon.py` & `apysc-4.4.3/apysc/_material_design/icon/material_nat_icon.py`

 * *Files identical despite different names*

### Comparing `apysc-4.4.2/apysc/_material_design/icon/material_nat_outlined_icon.py` & `apysc-4.4.3/apysc/_material_design/icon/material_nat_outlined_icon.py`

 * *Files identical despite different names*

### Comparing `apysc-4.4.2/apysc/_material_design/icon/material_new_releases_icon.py` & `apysc-4.4.3/apysc/_material_design/icon/material_new_releases_icon.py`

 * *Files identical despite different names*

### Comparing `apysc-4.4.2/apysc/_material_design/icon/material_new_releases_outlined_icon.py` & `apysc-4.4.3/apysc/_material_design/icon/material_new_releases_outlined_icon.py`

 * *Files identical despite different names*

### Comparing `apysc-4.4.2/apysc/_material_design/icon/material_next_plan_icon.py` & `apysc-4.4.3/apysc/_material_design/icon/material_next_plan_icon.py`

 * *Files identical despite different names*

### Comparing `apysc-4.4.2/apysc/_material_design/icon/material_next_plan_outlined_icon.py` & `apysc-4.4.3/apysc/_material_design/icon/material_next_plan_outlined_icon.py`

 * *Files identical despite different names*

### Comparing `apysc-4.4.2/apysc/_material_design/icon/material_next_week_icon.py` & `apysc-4.4.3/apysc/_material_design/icon/material_next_week_icon.py`

 * *Files identical despite different names*

### Comparing `apysc-4.4.2/apysc/_material_design/icon/material_next_week_outlined_icon.py` & `apysc-4.4.3/apysc/_material_design/icon/material_next_week_outlined_icon.py`

 * *Files identical despite different names*

### Comparing `apysc-4.4.2/apysc/_material_design/icon/material_nightlight_round_icon.py` & `apysc-4.4.3/apysc/_material_design/icon/material_nightlight_round_icon.py`

 * *Files identical despite different names*

### Comparing `apysc-4.4.2/apysc/_material_design/icon/material_no_sim_icon.py` & `apysc-4.4.3/apysc/_material_design/icon/material_no_sim_icon.py`

 * *Files identical despite different names*

### Comparing `apysc-4.4.2/apysc/_material_design/icon/material_no_sim_outlined_icon.py` & `apysc-4.4.3/apysc/_material_design/icon/material_no_sim_outlined_icon.py`

 * *Files identical despite different names*

### Comparing `apysc-4.4.2/apysc/_material_design/icon/material_not_accessible_icon.py` & `apysc-4.4.3/apysc/_material_design/icon/material_not_accessible_icon.py`

 * *Files identical despite different names*

### Comparing `apysc-4.4.2/apysc/_material_design/icon/material_not_accessible_outlined_icon.py` & `apysc-4.4.3/apysc/_material_design/icon/material_not_accessible_outlined_icon.py`

 * *Files identical despite different names*

### Comparing `apysc-4.4.2/apysc/_material_design/icon/material_not_interested_icon.py` & `apysc-4.4.3/apysc/_material_design/icon/material_not_interested_icon.py`

 * *Files identical despite different names*

### Comparing `apysc-4.4.2/apysc/_material_design/icon/material_not_interested_outlined_icon.py` & `apysc-4.4.3/apysc/_material_design/icon/material_not_interested_outlined_icon.py`

 * *Files identical despite different names*

### Comparing `apysc-4.4.2/apysc/_material_design/icon/material_not_started_icon.py` & `apysc-4.4.3/apysc/_material_design/icon/material_not_started_icon.py`

 * *Files identical despite different names*

### Comparing `apysc-4.4.2/apysc/_material_design/icon/material_not_started_outlined_icon.py` & `apysc-4.4.3/apysc/_material_design/icon/material_not_started_outlined_icon.py`

 * *Files identical despite different names*

### Comparing `apysc-4.4.2/apysc/_material_design/icon/material_note_add_icon.py` & `apysc-4.4.3/apysc/_material_design/icon/material_note_add_icon.py`

 * *Files identical despite different names*

### Comparing `apysc-4.4.2/apysc/_material_design/icon/material_note_add_outlined_icon.py` & `apysc-4.4.3/apysc/_material_design/icon/material_note_add_outlined_icon.py`

 * *Files identical despite different names*

### Comparing `apysc-4.4.2/apysc/_material_design/icon/material_note_icon.py` & `apysc-4.4.3/apysc/_material_design/icon/material_note_icon.py`

 * *Files identical despite different names*

### Comparing `apysc-4.4.2/apysc/_material_design/icon/material_note_outlined_icon.py` & `apysc-4.4.3/apysc/_material_design/icon/material_note_outlined_icon.py`

 * *Files identical despite different names*

### Comparing `apysc-4.4.2/apysc/_material_design/icon/material_notification_important_icon.py` & `apysc-4.4.3/apysc/_material_design/icon/material_notification_important_icon.py`

 * *Files identical despite different names*

### Comparing `apysc-4.4.2/apysc/_material_design/icon/material_notification_important_outlined_icon.py` & `apysc-4.4.3/apysc/_material_design/icon/material_notification_important_outlined_icon.py`

 * *Files identical despite different names*

### Comparing `apysc-4.4.2/apysc/_material_design/icon/material_offline_bolt_icon.py` & `apysc-4.4.3/apysc/_material_design/icon/material_offline_bolt_icon.py`

 * *Files identical despite different names*

### Comparing `apysc-4.4.2/apysc/_material_design/icon/material_offline_bolt_outlined_icon.py` & `apysc-4.4.3/apysc/_material_design/icon/material_offline_bolt_outlined_icon.py`

 * *Files identical despite different names*

### Comparing `apysc-4.4.2/apysc/_material_design/icon/material_offline_pin_icon.py` & `apysc-4.4.3/apysc/_material_design/icon/material_offline_pin_icon.py`

 * *Files identical despite different names*

### Comparing `apysc-4.4.2/apysc/_material_design/icon/material_offline_pin_outlined_icon.py` & `apysc-4.4.3/apysc/_material_design/icon/material_offline_pin_outlined_icon.py`

 * *Files identical despite different names*

### Comparing `apysc-4.4.2/apysc/_material_design/icon/material_online_prediction_icon.py` & `apysc-4.4.3/apysc/_material_design/icon/material_online_prediction_icon.py`

 * *Files identical despite different names*

### Comparing `apysc-4.4.2/apysc/_material_design/icon/material_online_prediction_outlined_icon.py` & `apysc-4.4.3/apysc/_material_design/icon/material_online_prediction_outlined_icon.py`

 * *Files identical despite different names*

### Comparing `apysc-4.4.2/apysc/_material_design/icon/material_opacity_icon.py` & `apysc-4.4.3/apysc/_material_design/icon/material_opacity_icon.py`

 * *Files identical despite different names*

### Comparing `apysc-4.4.2/apysc/_material_design/icon/material_opacity_outlined_icon.py` & `apysc-4.4.3/apysc/_material_design/icon/material_opacity_outlined_icon.py`

 * *Files identical despite different names*

### Comparing `apysc-4.4.2/apysc/_material_design/icon/material_open_in_browser_icon.py` & `apysc-4.4.3/apysc/_material_design/icon/material_open_in_browser_icon.py`

 * *Files identical despite different names*

### Comparing `apysc-4.4.2/apysc/_material_design/icon/material_open_in_browser_outlined_icon.py` & `apysc-4.4.3/apysc/_material_design/icon/material_open_in_browser_outlined_icon.py`

 * *Files identical despite different names*

### Comparing `apysc-4.4.2/apysc/_material_design/icon/material_open_in_full_icon.py` & `apysc-4.4.3/apysc/_material_design/icon/material_open_in_full_icon.py`

 * *Files identical despite different names*

### Comparing `apysc-4.4.2/apysc/_material_design/icon/material_open_in_full_outlined_icon.py` & `apysc-4.4.3/apysc/_material_design/icon/material_open_in_full_outlined_icon.py`

 * *Files identical despite different names*

### Comparing `apysc-4.4.2/apysc/_material_design/icon/material_open_in_new_icon.py` & `apysc-4.4.3/apysc/_material_design/icon/material_open_in_new_icon.py`

 * *Files identical despite different names*

### Comparing `apysc-4.4.2/apysc/_material_design/icon/material_open_in_new_outlined_icon.py` & `apysc-4.4.3/apysc/_material_design/icon/material_open_in_new_outlined_icon.py`

 * *Files identical despite different names*

### Comparing `apysc-4.4.2/apysc/_material_design/icon/material_open_with_icon.py` & `apysc-4.4.3/apysc/_material_design/icon/material_open_with_icon.py`

 * *Files identical despite different names*

### Comparing `apysc-4.4.2/apysc/_material_design/icon/material_open_with_outlined_icon.py` & `apysc-4.4.3/apysc/_material_design/icon/material_open_with_outlined_icon.py`

 * *Files identical despite different names*

### Comparing `apysc-4.4.2/apysc/_material_design/icon/material_outbond_icon.py` & `apysc-4.4.3/apysc/_material_design/icon/material_outbond_icon.py`

 * *Files identical despite different names*

### Comparing `apysc-4.4.2/apysc/_material_design/icon/material_outbond_outlined_icon.py` & `apysc-4.4.3/apysc/_material_design/icon/material_outbond_outlined_icon.py`

 * *Files identical despite different names*

### Comparing `apysc-4.4.2/apysc/_material_design/icon/material_outbox_icon.py` & `apysc-4.4.3/apysc/_material_design/icon/material_outbox_icon.py`

 * *Files identical despite different names*

### Comparing `apysc-4.4.2/apysc/_material_design/icon/material_outgoing_mail_icon.py` & `apysc-4.4.3/apysc/_material_design/icon/material_outgoing_mail_icon.py`

 * *Files identical despite different names*

### Comparing `apysc-4.4.2/apysc/_material_design/icon/material_outlet_icon.py` & `apysc-4.4.3/apysc/_material_design/icon/material_outlet_icon.py`

 * *Files identical despite different names*

### Comparing `apysc-4.4.2/apysc/_material_design/icon/material_outlet_outlined_icon.py` & `apysc-4.4.3/apysc/_material_design/icon/material_outlet_outlined_icon.py`

 * *Files identical despite different names*

### Comparing `apysc-4.4.2/apysc/_material_design/icon/material_outlined_flag_icon.py` & `apysc-4.4.3/apysc/_material_design/icon/material_outlined_flag_icon.py`

 * *Files identical despite different names*

### Comparing `apysc-4.4.2/apysc/_material_design/icon/material_outlined_flag_outlined_icon.py` & `apysc-4.4.3/apysc/_material_design/icon/material_outlined_flag_outlined_icon.py`

 * *Files identical despite different names*

### Comparing `apysc-4.4.2/apysc/_material_design/icon/material_pageview_icon.py` & `apysc-4.4.3/apysc/_material_design/icon/material_pageview_icon.py`

 * *Files identical despite different names*

### Comparing `apysc-4.4.2/apysc/_material_design/icon/material_pageview_outlined_icon.py` & `apysc-4.4.3/apysc/_material_design/icon/material_pageview_outlined_icon.py`

 * *Files identical despite different names*

### Comparing `apysc-4.4.2/apysc/_material_design/icon/material_pan_tool_icon.py` & `apysc-4.4.3/apysc/_material_design/icon/material_pan_tool_icon.py`

 * *Files identical despite different names*

### Comparing `apysc-4.4.2/apysc/_material_design/icon/material_pan_tool_outlined_icon.py` & `apysc-4.4.3/apysc/_material_design/icon/material_pan_tool_outlined_icon.py`

 * *Files identical despite different names*

### Comparing `apysc-4.4.2/apysc/_material_design/icon/material_pause_circle_filled_icon.py` & `apysc-4.4.3/apysc/_material_design/icon/material_pause_circle_filled_icon.py`

 * *Files identical despite different names*

### Comparing `apysc-4.4.2/apysc/_material_design/icon/material_pause_circle_filled_outlined_icon.py` & `apysc-4.4.3/apysc/_material_design/icon/material_pause_circle_filled_outlined_icon.py`

 * *Files identical despite different names*

### Comparing `apysc-4.4.2/apysc/_material_design/icon/material_pause_circle_outline_icon.py` & `apysc-4.4.3/apysc/_material_design/icon/material_pause_circle_outline_icon.py`

 * *Files identical despite different names*

### Comparing `apysc-4.4.2/apysc/_material_design/icon/material_pause_circle_outline_outlined_icon.py` & `apysc-4.4.3/apysc/_material_design/icon/material_pause_circle_outline_outlined_icon.py`

 * *Files identical despite different names*

### Comparing `apysc-4.4.2/apysc/_material_design/icon/material_pause_icon.py` & `apysc-4.4.3/apysc/_material_design/icon/material_pause_icon.py`

 * *Files identical despite different names*

### Comparing `apysc-4.4.2/apysc/_material_design/icon/material_pause_outlined_icon.py` & `apysc-4.4.3/apysc/_material_design/icon/material_pause_outlined_icon.py`

 * *Files identical despite different names*

### Comparing `apysc-4.4.2/apysc/_material_design/icon/material_pause_presentation_icon.py` & `apysc-4.4.3/apysc/_material_design/icon/material_pause_presentation_icon.py`

 * *Files identical despite different names*

### Comparing `apysc-4.4.2/apysc/_material_design/icon/material_pause_presentation_outlined_icon.py` & `apysc-4.4.3/apysc/_material_design/icon/material_pause_presentation_outlined_icon.py`

 * *Files identical despite different names*

### Comparing `apysc-4.4.2/apysc/_material_design/icon/material_payment_icon.py` & `apysc-4.4.3/apysc/_material_design/icon/material_payment_icon.py`

 * *Files identical despite different names*

### Comparing `apysc-4.4.2/apysc/_material_design/icon/material_payment_outlined_icon.py` & `apysc-4.4.3/apysc/_material_design/icon/material_payment_outlined_icon.py`

 * *Files identical despite different names*

### Comparing `apysc-4.4.2/apysc/_material_design/icon/material_pending_actions_icon.py` & `apysc-4.4.3/apysc/_material_design/icon/material_pending_actions_icon.py`

 * *Files identical despite different names*

### Comparing `apysc-4.4.2/apysc/_material_design/icon/material_pending_actions_outlined_icon.py` & `apysc-4.4.3/apysc/_material_design/icon/material_pending_actions_outlined_icon.py`

 * *Files identical despite different names*

### Comparing `apysc-4.4.2/apysc/_material_design/icon/material_pending_icon.py` & `apysc-4.4.3/apysc/_material_design/icon/material_pending_icon.py`

 * *Files identical despite different names*

### Comparing `apysc-4.4.2/apysc/_material_design/icon/material_pending_outlined_icon.py` & `apysc-4.4.3/apysc/_material_design/icon/material_pending_outlined_icon.py`

 * *Files identical despite different names*

### Comparing `apysc-4.4.2/apysc/_material_design/icon/material_perm_camera_mic_icon.py` & `apysc-4.4.3/apysc/_material_design/icon/material_perm_camera_mic_icon.py`

 * *Files identical despite different names*

### Comparing `apysc-4.4.2/apysc/_material_design/icon/material_perm_camera_mic_outlined_icon.py` & `apysc-4.4.3/apysc/_material_design/icon/material_perm_camera_mic_outlined_icon.py`

 * *Files identical despite different names*

### Comparing `apysc-4.4.2/apysc/_material_design/icon/material_perm_contact_calendar_icon.py` & `apysc-4.4.3/apysc/_material_design/icon/material_perm_contact_calendar_icon.py`

 * *Files identical despite different names*

### Comparing `apysc-4.4.2/apysc/_material_design/icon/material_perm_contact_calendar_outlined_icon.py` & `apysc-4.4.3/apysc/_material_design/icon/material_perm_contact_calendar_outlined_icon.py`

 * *Files identical despite different names*

### Comparing `apysc-4.4.2/apysc/_material_design/icon/material_perm_data_setting_icon.py` & `apysc-4.4.3/apysc/_material_design/icon/material_perm_data_setting_icon.py`

 * *Files identical despite different names*

### Comparing `apysc-4.4.2/apysc/_material_design/icon/material_perm_data_setting_outlined_icon.py` & `apysc-4.4.3/apysc/_material_design/icon/material_perm_data_setting_outlined_icon.py`

 * *Files identical despite different names*

### Comparing `apysc-4.4.2/apysc/_material_design/icon/material_perm_device_information_icon.py` & `apysc-4.4.3/apysc/_material_design/icon/material_perm_device_information_icon.py`

 * *Files identical despite different names*

### Comparing `apysc-4.4.2/apysc/_material_design/icon/material_perm_device_information_outlined_icon.py` & `apysc-4.4.3/apysc/_material_design/icon/material_perm_device_information_outlined_icon.py`

 * *Files identical despite different names*

### Comparing `apysc-4.4.2/apysc/_material_design/icon/material_perm_identity_icon.py` & `apysc-4.4.3/apysc/_material_design/icon/material_perm_identity_icon.py`

 * *Files identical despite different names*

### Comparing `apysc-4.4.2/apysc/_material_design/icon/material_perm_identity_outlined_icon.py` & `apysc-4.4.3/apysc/_material_design/icon/material_perm_identity_outlined_icon.py`

 * *Files identical despite different names*

### Comparing `apysc-4.4.2/apysc/_material_design/icon/material_perm_media_icon.py` & `apysc-4.4.3/apysc/_material_design/icon/material_perm_media_icon.py`

 * *Files identical despite different names*

### Comparing `apysc-4.4.2/apysc/_material_design/icon/material_perm_media_outlined_icon.py` & `apysc-4.4.3/apysc/_material_design/icon/material_perm_media_outlined_icon.py`

 * *Files identical despite different names*

### Comparing `apysc-4.4.2/apysc/_material_design/icon/material_perm_phone_msg_icon.py` & `apysc-4.4.3/apysc/_material_design/icon/material_perm_phone_msg_icon.py`

 * *Files identical despite different names*

### Comparing `apysc-4.4.2/apysc/_material_design/icon/material_perm_phone_msg_outlined_icon.py` & `apysc-4.4.3/apysc/_material_design/icon/material_perm_phone_msg_outlined_icon.py`

 * *Files identical despite different names*

### Comparing `apysc-4.4.2/apysc/_material_design/icon/material_perm_scan_wifi_icon.py` & `apysc-4.4.3/apysc/_material_design/icon/material_perm_scan_wifi_icon.py`

 * *Files identical despite different names*

### Comparing `apysc-4.4.2/apysc/_material_design/icon/material_perm_scan_wifi_outlined_icon.py` & `apysc-4.4.3/apysc/_material_design/icon/material_perm_scan_wifi_outlined_icon.py`

 * *Files identical despite different names*

### Comparing `apysc-4.4.2/apysc/_material_design/icon/material_person_add_disabled_icon.py` & `apysc-4.4.3/apysc/_material_design/icon/material_person_add_disabled_icon.py`

 * *Files identical despite different names*

### Comparing `apysc-4.4.2/apysc/_material_design/icon/material_person_add_disabled_outlined_icon.py` & `apysc-4.4.3/apysc/_material_design/icon/material_person_add_disabled_outlined_icon.py`

 * *Files identical despite different names*

### Comparing `apysc-4.4.2/apysc/_material_design/icon/material_person_search_icon.py` & `apysc-4.4.3/apysc/_material_design/icon/material_person_search_icon.py`

 * *Files identical despite different names*

### Comparing `apysc-4.4.2/apysc/_material_design/icon/material_person_search_outlined_icon.py` & `apysc-4.4.3/apysc/_material_design/icon/material_person_search_outlined_icon.py`

 * *Files identical despite different names*

### Comparing `apysc-4.4.2/apysc/_material_design/icon/material_pets_icon.py` & `apysc-4.4.3/apysc/_material_design/icon/material_pets_icon.py`

 * *Files identical despite different names*

### Comparing `apysc-4.4.2/apysc/_material_design/icon/material_pets_outlined_icon.py` & `apysc-4.4.3/apysc/_material_design/icon/material_pets_outlined_icon.py`

 * *Files identical despite different names*

### Comparing `apysc-4.4.2/apysc/_material_design/icon/material_phone_disabled_icon.py` & `apysc-4.4.3/apysc/_material_design/icon/material_phone_disabled_icon.py`

 * *Files identical despite different names*

### Comparing `apysc-4.4.2/apysc/_material_design/icon/material_phone_disabled_outlined_icon.py` & `apysc-4.4.3/apysc/_material_design/icon/material_phone_disabled_outlined_icon.py`

 * *Files identical despite different names*

### Comparing `apysc-4.4.2/apysc/_material_design/icon/material_phone_enabled_icon.py` & `apysc-4.4.3/apysc/_material_design/icon/material_phone_enabled_icon.py`

 * *Files identical despite different names*

### Comparing `apysc-4.4.2/apysc/_material_design/icon/material_phone_enabled_outlined_icon.py` & `apysc-4.4.3/apysc/_material_design/icon/material_phone_enabled_outlined_icon.py`

 * *Files identical despite different names*

### Comparing `apysc-4.4.2/apysc/_material_design/icon/material_phone_icon.py` & `apysc-4.4.3/apysc/_material_design/icon/material_phone_icon.py`

 * *Files identical despite different names*

### Comparing `apysc-4.4.2/apysc/_material_design/icon/material_phone_outlined_icon.py` & `apysc-4.4.3/apysc/_material_design/icon/material_phone_outlined_icon.py`

 * *Files identical despite different names*

### Comparing `apysc-4.4.2/apysc/_material_design/icon/material_phonelink_erase_icon.py` & `apysc-4.4.3/apysc/_material_design/icon/material_phonelink_erase_icon.py`

 * *Files identical despite different names*

### Comparing `apysc-4.4.2/apysc/_material_design/icon/material_phonelink_erase_outlined_icon.py` & `apysc-4.4.3/apysc/_material_design/icon/material_phonelink_erase_outlined_icon.py`

 * *Files identical despite different names*

### Comparing `apysc-4.4.2/apysc/_material_design/icon/material_phonelink_lock_icon.py` & `apysc-4.4.3/apysc/_material_design/icon/material_phonelink_lock_icon.py`

 * *Files identical despite different names*

### Comparing `apysc-4.4.2/apysc/_material_design/icon/material_phonelink_lock_outlined_icon.py` & `apysc-4.4.3/apysc/_material_design/icon/material_phonelink_lock_outlined_icon.py`

 * *Files identical despite different names*

### Comparing `apysc-4.4.2/apysc/_material_design/icon/material_phonelink_ring_icon.py` & `apysc-4.4.3/apysc/_material_design/icon/material_phonelink_ring_icon.py`

 * *Files identical despite different names*

### Comparing `apysc-4.4.2/apysc/_material_design/icon/material_phonelink_ring_outlined_icon.py` & `apysc-4.4.3/apysc/_material_design/icon/material_phonelink_ring_outlined_icon.py`

 * *Files identical despite different names*

### Comparing `apysc-4.4.2/apysc/_material_design/icon/material_phonelink_setup_icon.py` & `apysc-4.4.3/apysc/_material_design/icon/material_phonelink_setup_icon.py`

 * *Files identical despite different names*

### Comparing `apysc-4.4.2/apysc/_material_design/icon/material_phonelink_setup_outlined_icon.py` & `apysc-4.4.3/apysc/_material_design/icon/material_phonelink_setup_outlined_icon.py`

 * *Files identical despite different names*

### Comparing `apysc-4.4.2/apysc/_material_design/icon/material_picture_in_picture_alt_icon.py` & `apysc-4.4.3/apysc/_material_design/icon/material_picture_in_picture_alt_icon.py`

 * *Files identical despite different names*

### Comparing `apysc-4.4.2/apysc/_material_design/icon/material_picture_in_picture_alt_outlined_icon.py` & `apysc-4.4.3/apysc/_material_design/icon/material_picture_in_picture_alt_outlined_icon.py`

 * *Files identical despite different names*

### Comparing `apysc-4.4.2/apysc/_material_design/icon/material_picture_in_picture_icon.py` & `apysc-4.4.3/apysc/_material_design/icon/material_picture_in_picture_icon.py`

 * *Files identical despite different names*

### Comparing `apysc-4.4.2/apysc/_material_design/icon/material_picture_in_picture_outlined_icon.py` & `apysc-4.4.3/apysc/_material_design/icon/material_picture_in_picture_outlined_icon.py`

 * *Files identical despite different names*

### Comparing `apysc-4.4.2/apysc/_material_design/icon/material_plagiarism_icon.py` & `apysc-4.4.3/apysc/_material_design/icon/material_plagiarism_icon.py`

 * *Files identical despite different names*

### Comparing `apysc-4.4.2/apysc/_material_design/icon/material_plagiarism_outlined_icon.py` & `apysc-4.4.3/apysc/_material_design/icon/material_plagiarism_outlined_icon.py`

 * *Files identical despite different names*

### Comparing `apysc-4.4.2/apysc/_material_design/icon/material_play_arrow_icon.py` & `apysc-4.4.3/apysc/_material_design/icon/material_play_arrow_icon.py`

 * *Files identical despite different names*

### Comparing `apysc-4.4.2/apysc/_material_design/icon/material_play_arrow_outlined_icon.py` & `apysc-4.4.3/apysc/_material_design/icon/material_play_arrow_outlined_icon.py`

 * *Files identical despite different names*

### Comparing `apysc-4.4.2/apysc/_material_design/icon/material_play_circle_filled_icon.py` & `apysc-4.4.3/apysc/_material_design/icon/material_play_circle_filled_icon.py`

 * *Files identical despite different names*

### Comparing `apysc-4.4.2/apysc/_material_design/icon/material_play_circle_filled_outlined_icon.py` & `apysc-4.4.3/apysc/_material_design/icon/material_play_circle_filled_outlined_icon.py`

 * *Files identical despite different names*

### Comparing `apysc-4.4.2/apysc/_material_design/icon/material_play_circle_outline_icon.py` & `apysc-4.4.3/apysc/_material_design/icon/material_play_circle_outline_icon.py`

 * *Files identical despite different names*

### Comparing `apysc-4.4.2/apysc/_material_design/icon/material_play_circle_outline_outlined_icon.py` & `apysc-4.4.3/apysc/_material_design/icon/material_play_circle_outline_outlined_icon.py`

 * *Files identical despite different names*

### Comparing `apysc-4.4.2/apysc/_material_design/icon/material_play_disabled_icon.py` & `apysc-4.4.3/apysc/_material_design/icon/material_play_disabled_icon.py`

 * *Files identical despite different names*

### Comparing `apysc-4.4.2/apysc/_material_design/icon/material_play_for_work_icon.py` & `apysc-4.4.3/apysc/_material_design/icon/material_play_for_work_icon.py`

 * *Files identical despite different names*

### Comparing `apysc-4.4.2/apysc/_material_design/icon/material_play_for_work_outlined_icon.py` & `apysc-4.4.3/apysc/_material_design/icon/material_play_for_work_outlined_icon.py`

 * *Files identical despite different names*

### Comparing `apysc-4.4.2/apysc/_material_design/icon/material_playlist_add_check_icon.py` & `apysc-4.4.3/apysc/_material_design/icon/material_playlist_add_check_icon.py`

 * *Files identical despite different names*

### Comparing `apysc-4.4.2/apysc/_material_design/icon/material_playlist_add_check_outlined_icon.py` & `apysc-4.4.3/apysc/_material_design/icon/material_playlist_add_check_outlined_icon.py`

 * *Files identical despite different names*

### Comparing `apysc-4.4.2/apysc/_material_design/icon/material_playlist_add_icon.py` & `apysc-4.4.3/apysc/_material_design/icon/material_playlist_add_icon.py`

 * *Files identical despite different names*

### Comparing `apysc-4.4.2/apysc/_material_design/icon/material_playlist_add_outlined_icon.py` & `apysc-4.4.3/apysc/_material_design/icon/material_playlist_add_outlined_icon.py`

 * *Files identical despite different names*

### Comparing `apysc-4.4.2/apysc/_material_design/icon/material_playlist_play_icon.py` & `apysc-4.4.3/apysc/_material_design/icon/material_playlist_play_icon.py`

 * *Files identical despite different names*

### Comparing `apysc-4.4.2/apysc/_material_design/icon/material_playlist_play_outlined_icon.py` & `apysc-4.4.3/apysc/_material_design/icon/material_playlist_play_outlined_icon.py`

 * *Files identical despite different names*

### Comparing `apysc-4.4.2/apysc/_material_design/icon/material_policy_icon.py` & `apysc-4.4.3/apysc/_material_design/icon/material_policy_icon.py`

 * *Files identical despite different names*

### Comparing `apysc-4.4.2/apysc/_material_design/icon/material_policy_outlined_icon.py` & `apysc-4.4.3/apysc/_material_design/icon/material_policy_outlined_icon.py`

 * *Files identical despite different names*

### Comparing `apysc-4.4.2/apysc/_material_design/icon/material_polymer_icon.py` & `apysc-4.4.3/apysc/_material_design/icon/material_polymer_icon.py`

 * *Files identical despite different names*

### Comparing `apysc-4.4.2/apysc/_material_design/icon/material_polymer_outlined_icon.py` & `apysc-4.4.3/apysc/_material_design/icon/material_polymer_outlined_icon.py`

 * *Files identical despite different names*

### Comparing `apysc-4.4.2/apysc/_material_design/icon/material_portable_wifi_off_icon.py` & `apysc-4.4.3/apysc/_material_design/icon/material_portable_wifi_off_icon.py`

 * *Files identical despite different names*

### Comparing `apysc-4.4.2/apysc/_material_design/icon/material_portable_wifi_off_outlined_icon.py` & `apysc-4.4.3/apysc/_material_design/icon/material_portable_wifi_off_outlined_icon.py`

 * *Files identical despite different names*

### Comparing `apysc-4.4.2/apysc/_material_design/icon/material_power_settings_new_icon.py` & `apysc-4.4.3/apysc/_material_design/icon/material_power_settings_new_icon.py`

 * *Files identical despite different names*

### Comparing `apysc-4.4.2/apysc/_material_design/icon/material_power_settings_new_outlined_icon.py` & `apysc-4.4.3/apysc/_material_design/icon/material_power_settings_new_outlined_icon.py`

 * *Files identical despite different names*

### Comparing `apysc-4.4.2/apysc/_material_design/icon/material_pregnant_woman_icon.py` & `apysc-4.4.3/apysc/_material_design/icon/material_pregnant_woman_icon.py`

 * *Files identical despite different names*

### Comparing `apysc-4.4.2/apysc/_material_design/icon/material_pregnant_woman_outlined_icon.py` & `apysc-4.4.3/apysc/_material_design/icon/material_pregnant_woman_outlined_icon.py`

 * *Files identical despite different names*

### Comparing `apysc-4.4.2/apysc/_material_design/icon/material_present_to_all_icon.py` & `apysc-4.4.3/apysc/_material_design/icon/material_present_to_all_icon.py`

 * *Files identical despite different names*

### Comparing `apysc-4.4.2/apysc/_material_design/icon/material_present_to_all_outlined_icon.py` & `apysc-4.4.3/apysc/_material_design/icon/material_present_to_all_outlined_icon.py`

 * *Files identical despite different names*

### Comparing `apysc-4.4.2/apysc/_material_design/icon/material_preview_icon.py` & `apysc-4.4.3/apysc/_material_design/icon/material_preview_icon.py`

 * *Files identical despite different names*

### Comparing `apysc-4.4.2/apysc/_material_design/icon/material_preview_outlined_icon.py` & `apysc-4.4.3/apysc/_material_design/icon/material_preview_outlined_icon.py`

 * *Files identical despite different names*

### Comparing `apysc-4.4.2/apysc/_material_design/icon/material_print_disabled_icon.py` & `apysc-4.4.3/apysc/_material_design/icon/material_print_disabled_icon.py`

 * *Files identical despite different names*

### Comparing `apysc-4.4.2/apysc/_material_design/icon/material_print_disabled_outlined_icon.py` & `apysc-4.4.3/apysc/_material_design/icon/material_print_disabled_outlined_icon.py`

 * *Files identical despite different names*

### Comparing `apysc-4.4.2/apysc/_material_design/icon/material_print_icon.py` & `apysc-4.4.3/apysc/_material_design/icon/material_print_icon.py`

 * *Files identical despite different names*

### Comparing `apysc-4.4.2/apysc/_material_design/icon/material_print_outlined_icon.py` & `apysc-4.4.3/apysc/_material_design/icon/material_print_outlined_icon.py`

 * *Files identical despite different names*

### Comparing `apysc-4.4.2/apysc/_material_design/icon/material_privacy_tip_icon.py` & `apysc-4.4.3/apysc/_material_design/icon/material_privacy_tip_icon.py`

 * *Files identical despite different names*

### Comparing `apysc-4.4.2/apysc/_material_design/icon/material_privacy_tip_outlined_icon.py` & `apysc-4.4.3/apysc/_material_design/icon/material_privacy_tip_outlined_icon.py`

 * *Files identical despite different names*

### Comparing `apysc-4.4.2/apysc/_material_design/icon/material_published_with_changes_icon.py` & `apysc-4.4.3/apysc/_material_design/icon/material_published_with_changes_icon.py`

 * *Files identical despite different names*

### Comparing `apysc-4.4.2/apysc/_material_design/icon/material_published_with_changes_outlined_icon.py` & `apysc-4.4.3/apysc/_material_design/icon/material_published_with_changes_outlined_icon.py`

 * *Files identical despite different names*

### Comparing `apysc-4.4.2/apysc/_material_design/icon/material_push_pin_icon.py` & `apysc-4.4.3/apysc/_material_design/icon/material_push_pin_icon.py`

 * *Files identical despite different names*

### Comparing `apysc-4.4.2/apysc/_material_design/icon/material_push_pin_outlined_icon.py` & `apysc-4.4.3/apysc/_material_design/icon/material_push_pin_outlined_icon.py`

 * *Files identical despite different names*

### Comparing `apysc-4.4.2/apysc/_material_design/icon/material_qr_code_icon.py` & `apysc-4.4.3/apysc/_material_design/icon/material_qr_code_icon.py`

 * *Files identical despite different names*

### Comparing `apysc-4.4.2/apysc/_material_design/icon/material_qr_code_outlined_icon.py` & `apysc-4.4.3/apysc/_material_design/icon/material_qr_code_outlined_icon.py`

 * *Files identical despite different names*

### Comparing `apysc-4.4.2/apysc/_material_design/icon/material_qr_code_scanner_icon.py` & `apysc-4.4.3/apysc/_material_design/icon/material_qr_code_scanner_icon.py`

 * *Files identical despite different names*

### Comparing `apysc-4.4.2/apysc/_material_design/icon/material_qr_code_scanner_outlined_icon.py` & `apysc-4.4.3/apysc/_material_design/icon/material_qr_code_scanner_outlined_icon.py`

 * *Files identical despite different names*

### Comparing `apysc-4.4.2/apysc/_material_design/icon/material_query_builder_icon.py` & `apysc-4.4.3/apysc/_material_design/icon/material_query_builder_icon.py`

 * *Files identical despite different names*

### Comparing `apysc-4.4.2/apysc/_material_design/icon/material_query_builder_outlined_icon.py` & `apysc-4.4.3/apysc/_material_design/icon/material_query_builder_outlined_icon.py`

 * *Files identical despite different names*

### Comparing `apysc-4.4.2/apysc/_material_design/icon/material_question_answer_icon.py` & `apysc-4.4.3/apysc/_material_design/icon/material_question_answer_icon.py`

 * *Files identical despite different names*

### Comparing `apysc-4.4.2/apysc/_material_design/icon/material_question_answer_outlined_icon.py` & `apysc-4.4.3/apysc/_material_design/icon/material_question_answer_outlined_icon.py`

 * *Files identical despite different names*

### Comparing `apysc-4.4.2/apysc/_material_design/icon/material_queue_icon.py` & `apysc-4.4.3/apysc/_material_design/icon/material_queue_icon.py`

 * *Files identical despite different names*

### Comparing `apysc-4.4.2/apysc/_material_design/icon/material_queue_music_icon.py` & `apysc-4.4.3/apysc/_material_design/icon/material_queue_music_icon.py`

 * *Files identical despite different names*

### Comparing `apysc-4.4.2/apysc/_material_design/icon/material_queue_music_outlined_icon.py` & `apysc-4.4.3/apysc/_material_design/icon/material_queue_music_outlined_icon.py`

 * *Files identical despite different names*

### Comparing `apysc-4.4.2/apysc/_material_design/icon/material_queue_outlined_icon.py` & `apysc-4.4.3/apysc/_material_design/icon/material_queue_outlined_icon.py`

 * *Files identical despite different names*

### Comparing `apysc-4.4.2/apysc/_material_design/icon/material_queue_play_next_icon.py` & `apysc-4.4.3/apysc/_material_design/icon/material_queue_play_next_icon.py`

 * *Files identical despite different names*

### Comparing `apysc-4.4.2/apysc/_material_design/icon/material_queue_play_next_outlined_icon.py` & `apysc-4.4.3/apysc/_material_design/icon/material_queue_play_next_outlined_icon.py`

 * *Files identical despite different names*

### Comparing `apysc-4.4.2/apysc/_material_design/icon/material_quickreply_icon.py` & `apysc-4.4.3/apysc/_material_design/icon/material_quickreply_icon.py`

 * *Files identical despite different names*

### Comparing `apysc-4.4.2/apysc/_material_design/icon/material_quickreply_outlined_icon.py` & `apysc-4.4.3/apysc/_material_design/icon/material_quickreply_outlined_icon.py`

 * *Files identical despite different names*

### Comparing `apysc-4.4.2/apysc/_material_design/icon/material_radio_icon.py` & `apysc-4.4.3/apysc/_material_design/icon/material_radio_icon.py`

 * *Files identical despite different names*

### Comparing `apysc-4.4.2/apysc/_material_design/icon/material_radio_outlined_icon.py` & `apysc-4.4.3/apysc/_material_design/icon/material_radio_outlined_icon.py`

 * *Files identical despite different names*

### Comparing `apysc-4.4.2/apysc/_material_design/icon/material_read_more_icon.py` & `apysc-4.4.3/apysc/_material_design/icon/material_read_more_icon.py`

 * *Files identical despite different names*

### Comparing `apysc-4.4.2/apysc/_material_design/icon/material_read_more_outlined_icon.py` & `apysc-4.4.3/apysc/_material_design/icon/material_read_more_outlined_icon.py`

 * *Files identical despite different names*

### Comparing `apysc-4.4.2/apysc/_material_design/icon/material_receipt_icon.py` & `apysc-4.4.3/apysc/_material_design/icon/material_receipt_icon.py`

 * *Files identical despite different names*

### Comparing `apysc-4.4.2/apysc/_material_design/icon/material_receipt_outlined_icon.py` & `apysc-4.4.3/apysc/_material_design/icon/material_receipt_outlined_icon.py`

 * *Files identical despite different names*

### Comparing `apysc-4.4.2/apysc/_material_design/icon/material_recent_actors_icon.py` & `apysc-4.4.3/apysc/_material_design/icon/material_recent_actors_icon.py`

 * *Files identical despite different names*

### Comparing `apysc-4.4.2/apysc/_material_design/icon/material_recent_actors_outlined_icon.py` & `apysc-4.4.3/apysc/_material_design/icon/material_recent_actors_outlined_icon.py`

 * *Files identical despite different names*

### Comparing `apysc-4.4.2/apysc/_material_design/icon/material_record_voice_over_icon.py` & `apysc-4.4.3/apysc/_material_design/icon/material_record_voice_over_icon.py`

 * *Files identical despite different names*

### Comparing `apysc-4.4.2/apysc/_material_design/icon/material_record_voice_over_outlined_icon.py` & `apysc-4.4.3/apysc/_material_design/icon/material_record_voice_over_outlined_icon.py`

 * *Files identical despite different names*

### Comparing `apysc-4.4.2/apysc/_material_design/icon/material_redeem_icon.py` & `apysc-4.4.3/apysc/_material_design/icon/material_redeem_icon.py`

 * *Files identical despite different names*

### Comparing `apysc-4.4.2/apysc/_material_design/icon/material_redeem_outlined_icon.py` & `apysc-4.4.3/apysc/_material_design/icon/material_redeem_outlined_icon.py`

 * *Files identical despite different names*

### Comparing `apysc-4.4.2/apysc/_material_design/icon/material_redo_icon.py` & `apysc-4.4.3/apysc/_material_design/icon/material_redo_icon.py`

 * *Files identical despite different names*

### Comparing `apysc-4.4.2/apysc/_material_design/icon/material_redo_outlined_icon.py` & `apysc-4.4.3/apysc/_material_design/icon/material_redo_outlined_icon.py`

 * *Files identical despite different names*

### Comparing `apysc-4.4.2/apysc/_material_design/icon/material_remove_circle_icon.py` & `apysc-4.4.3/apysc/_material_design/icon/material_remove_circle_icon.py`

 * *Files identical despite different names*

### Comparing `apysc-4.4.2/apysc/_material_design/icon/material_remove_circle_outline_icon.py` & `apysc-4.4.3/apysc/_material_design/icon/material_remove_circle_outline_icon.py`

 * *Files identical despite different names*

### Comparing `apysc-4.4.2/apysc/_material_design/icon/material_remove_circle_outline_outlined_icon.py` & `apysc-4.4.3/apysc/_material_design/icon/material_remove_circle_outline_outlined_icon.py`

 * *Files identical despite different names*

### Comparing `apysc-4.4.2/apysc/_material_design/icon/material_remove_circle_outlined_icon.py` & `apysc-4.4.3/apysc/_material_design/icon/material_remove_circle_outlined_icon.py`

 * *Files identical despite different names*

### Comparing `apysc-4.4.2/apysc/_material_design/icon/material_remove_done_icon.py` & `apysc-4.4.3/apysc/_material_design/icon/material_remove_done_icon.py`

 * *Files identical despite different names*

### Comparing `apysc-4.4.2/apysc/_material_design/icon/material_remove_from_queue_icon.py` & `apysc-4.4.3/apysc/_material_design/icon/material_remove_from_queue_icon.py`

 * *Files identical despite different names*

### Comparing `apysc-4.4.2/apysc/_material_design/icon/material_remove_from_queue_outlined_icon.py` & `apysc-4.4.3/apysc/_material_design/icon/material_remove_from_queue_outlined_icon.py`

 * *Files identical despite different names*

### Comparing `apysc-4.4.2/apysc/_material_design/icon/material_remove_icon.py` & `apysc-4.4.3/apysc/_material_design/icon/material_remove_icon.py`

 * *Files identical despite different names*

### Comparing `apysc-4.4.2/apysc/_material_design/icon/material_remove_outlined_icon.py` & `apysc-4.4.3/apysc/_material_design/icon/material_remove_outlined_icon.py`

 * *Files identical despite different names*

### Comparing `apysc-4.4.2/apysc/_material_design/icon/material_remove_shopping_cart_icon.py` & `apysc-4.4.3/apysc/_material_design/icon/material_remove_shopping_cart_icon.py`

 * *Files identical despite different names*

### Comparing `apysc-4.4.2/apysc/_material_design/icon/material_remove_shopping_cart_outlined_icon.py` & `apysc-4.4.3/apysc/_material_design/icon/material_remove_shopping_cart_outlined_icon.py`

 * *Files identical despite different names*

### Comparing `apysc-4.4.2/apysc/_material_design/icon/material_reorder_icon.py` & `apysc-4.4.3/apysc/_material_design/icon/material_reorder_icon.py`

 * *Files identical despite different names*

### Comparing `apysc-4.4.2/apysc/_material_design/icon/material_reorder_outlined_icon.py` & `apysc-4.4.3/apysc/_material_design/icon/material_reorder_outlined_icon.py`

 * *Files identical despite different names*

### Comparing `apysc-4.4.2/apysc/_material_design/icon/material_repeat_icon.py` & `apysc-4.4.3/apysc/_material_design/icon/material_repeat_icon.py`

 * *Files identical despite different names*

### Comparing `apysc-4.4.2/apysc/_material_design/icon/material_repeat_on_icon.py` & `apysc-4.4.3/apysc/_material_design/icon/material_repeat_on_icon.py`

 * *Files identical despite different names*

### Comparing `apysc-4.4.2/apysc/_material_design/icon/material_repeat_one_icon.py` & `apysc-4.4.3/apysc/_material_design/icon/material_repeat_one_icon.py`

 * *Files identical despite different names*

### Comparing `apysc-4.4.2/apysc/_material_design/icon/material_repeat_one_on_icon.py` & `apysc-4.4.3/apysc/_material_design/icon/material_repeat_one_on_icon.py`

 * *Files identical despite different names*

### Comparing `apysc-4.4.2/apysc/_material_design/icon/material_repeat_one_outlined_icon.py` & `apysc-4.4.3/apysc/_material_design/icon/material_repeat_one_outlined_icon.py`

 * *Files identical despite different names*

### Comparing `apysc-4.4.2/apysc/_material_design/icon/material_repeat_outlined_icon.py` & `apysc-4.4.3/apysc/_material_design/icon/material_repeat_outlined_icon.py`

 * *Files identical despite different names*

### Comparing `apysc-4.4.2/apysc/_material_design/icon/material_replay_10_icon.py` & `apysc-4.4.3/apysc/_material_design/icon/material_replay_10_icon.py`

 * *Files identical despite different names*

### Comparing `apysc-4.4.2/apysc/_material_design/icon/material_replay_10_outlined_icon.py` & `apysc-4.4.3/apysc/_material_design/icon/material_replay_10_outlined_icon.py`

 * *Files identical despite different names*

### Comparing `apysc-4.4.2/apysc/_material_design/icon/material_replay_30_icon.py` & `apysc-4.4.3/apysc/_material_design/icon/material_replay_30_icon.py`

 * *Files identical despite different names*

### Comparing `apysc-4.4.2/apysc/_material_design/icon/material_replay_30_outlined_icon.py` & `apysc-4.4.3/apysc/_material_design/icon/material_replay_30_outlined_icon.py`

 * *Files identical despite different names*

### Comparing `apysc-4.4.2/apysc/_material_design/icon/material_replay_5_icon.py` & `apysc-4.4.3/apysc/_material_design/icon/material_replay_5_icon.py`

 * *Files identical despite different names*

### Comparing `apysc-4.4.2/apysc/_material_design/icon/material_replay_5_outlined_icon.py` & `apysc-4.4.3/apysc/_material_design/icon/material_replay_5_outlined_icon.py`

 * *Files identical despite different names*

### Comparing `apysc-4.4.2/apysc/_material_design/icon/material_replay_circle_filled_icon.py` & `apysc-4.4.3/apysc/_material_design/icon/material_replay_circle_filled_icon.py`

 * *Files identical despite different names*

### Comparing `apysc-4.4.2/apysc/_material_design/icon/material_replay_icon.py` & `apysc-4.4.3/apysc/_material_design/icon/material_replay_icon.py`

 * *Files identical despite different names*

### Comparing `apysc-4.4.2/apysc/_material_design/icon/material_replay_outlined_icon.py` & `apysc-4.4.3/apysc/_material_design/icon/material_replay_outlined_icon.py`

 * *Files identical despite different names*

### Comparing `apysc-4.4.2/apysc/_material_design/icon/material_reply_all_icon.py` & `apysc-4.4.3/apysc/_material_design/icon/material_reply_all_icon.py`

 * *Files identical despite different names*

### Comparing `apysc-4.4.2/apysc/_material_design/icon/material_reply_all_outlined_icon.py` & `apysc-4.4.3/apysc/_material_design/icon/material_reply_all_outlined_icon.py`

 * *Files identical despite different names*

### Comparing `apysc-4.4.2/apysc/_material_design/icon/material_reply_icon.py` & `apysc-4.4.3/apysc/_material_design/icon/material_reply_icon.py`

 * *Files identical despite different names*

### Comparing `apysc-4.4.2/apysc/_material_design/icon/material_reply_outlined_icon.py` & `apysc-4.4.3/apysc/_material_design/icon/material_reply_outlined_icon.py`

 * *Files identical despite different names*

### Comparing `apysc-4.4.2/apysc/_material_design/icon/material_report_gmailerrorred_outlined_icon.py` & `apysc-4.4.3/apysc/_material_design/icon/material_report_gmailerrorred_outlined_icon.py`

 * *Files identical despite different names*

### Comparing `apysc-4.4.2/apysc/_material_design/icon/material_report_icon.py` & `apysc-4.4.3/apysc/_material_design/icon/material_report_icon.py`

 * *Files identical despite different names*

### Comparing `apysc-4.4.2/apysc/_material_design/icon/material_report_off_icon.py` & `apysc-4.4.3/apysc/_material_design/icon/material_report_off_icon.py`

 * *Files identical despite different names*

### Comparing `apysc-4.4.2/apysc/_material_design/icon/material_report_off_outlined_icon.py` & `apysc-4.4.3/apysc/_material_design/icon/material_report_off_outlined_icon.py`

 * *Files identical despite different names*

### Comparing `apysc-4.4.2/apysc/_material_design/icon/material_report_outlined_icon.py` & `apysc-4.4.3/apysc/_material_design/icon/material_report_outlined_icon.py`

 * *Files identical despite different names*

### Comparing `apysc-4.4.2/apysc/_material_design/icon/material_report_problem_icon.py` & `apysc-4.4.3/apysc/_material_design/icon/material_report_problem_icon.py`

 * *Files identical despite different names*

### Comparing `apysc-4.4.2/apysc/_material_design/icon/material_report_problem_outlined_icon.py` & `apysc-4.4.3/apysc/_material_design/icon/material_report_problem_outlined_icon.py`

 * *Files identical despite different names*

### Comparing `apysc-4.4.2/apysc/_material_design/icon/material_request_page_icon.py` & `apysc-4.4.3/apysc/_material_design/icon/material_request_page_icon.py`

 * *Files identical despite different names*

### Comparing `apysc-4.4.2/apysc/_material_design/icon/material_request_page_outlined_icon.py` & `apysc-4.4.3/apysc/_material_design/icon/material_request_page_outlined_icon.py`

 * *Files identical despite different names*

### Comparing `apysc-4.4.2/apysc/_material_design/icon/material_restore_from_trash_icon.py` & `apysc-4.4.3/apysc/_material_design/icon/material_restore_from_trash_icon.py`

 * *Files identical despite different names*

### Comparing `apysc-4.4.2/apysc/_material_design/icon/material_restore_from_trash_outlined_icon.py` & `apysc-4.4.3/apysc/_material_design/icon/material_restore_from_trash_outlined_icon.py`

 * *Files identical despite different names*

### Comparing `apysc-4.4.2/apysc/_material_design/icon/material_restore_icon.py` & `apysc-4.4.3/apysc/_material_design/icon/material_restore_icon.py`

 * *Files identical despite different names*

### Comparing `apysc-4.4.2/apysc/_material_design/icon/material_restore_outlined_icon.py` & `apysc-4.4.3/apysc/_material_design/icon/material_restore_outlined_icon.py`

 * *Files identical despite different names*

### Comparing `apysc-4.4.2/apysc/_material_design/icon/material_restore_page_icon.py` & `apysc-4.4.3/apysc/_material_design/icon/material_restore_page_icon.py`

 * *Files identical despite different names*

### Comparing `apysc-4.4.2/apysc/_material_design/icon/material_restore_page_outlined_icon.py` & `apysc-4.4.3/apysc/_material_design/icon/material_restore_page_outlined_icon.py`

 * *Files identical despite different names*

### Comparing `apysc-4.4.2/apysc/_material_design/icon/material_ring_volume_icon.py` & `apysc-4.4.3/apysc/_material_design/icon/material_ring_volume_icon.py`

 * *Files identical despite different names*

### Comparing `apysc-4.4.2/apysc/_material_design/icon/material_ring_volume_outlined_icon.py` & `apysc-4.4.3/apysc/_material_design/icon/material_ring_volume_outlined_icon.py`

 * *Files identical despite different names*

### Comparing `apysc-4.4.2/apysc/_material_design/icon/material_room_icon.py` & `apysc-4.4.3/apysc/_material_design/icon/material_room_icon.py`

 * *Files identical despite different names*

### Comparing `apysc-4.4.2/apysc/_material_design/icon/material_room_outlined_icon.py` & `apysc-4.4.3/apysc/_material_design/icon/material_room_outlined_icon.py`

 * *Files identical despite different names*

### Comparing `apysc-4.4.2/apysc/_material_design/icon/material_rounded_corner_icon.py` & `apysc-4.4.3/apysc/_material_design/icon/material_rounded_corner_icon.py`

 * *Files identical despite different names*

### Comparing `apysc-4.4.2/apysc/_material_design/icon/material_rounded_corner_outlined_icon.py` & `apysc-4.4.3/apysc/_material_design/icon/material_rounded_corner_outlined_icon.py`

 * *Files identical despite different names*

### Comparing `apysc-4.4.2/apysc/_material_design/icon/material_rowing_icon.py` & `apysc-4.4.3/apysc/_material_design/icon/material_rowing_icon.py`

 * *Files identical despite different names*

### Comparing `apysc-4.4.2/apysc/_material_design/icon/material_rowing_outlined_icon.py` & `apysc-4.4.3/apysc/_material_design/icon/material_rowing_outlined_icon.py`

 * *Files identical despite different names*

### Comparing `apysc-4.4.2/apysc/_material_design/icon/material_rss_feed_icon.py` & `apysc-4.4.3/apysc/_material_design/icon/material_rss_feed_icon.py`

 * *Files identical despite different names*

### Comparing `apysc-4.4.2/apysc/_material_design/icon/material_rss_feed_outlined_icon.py` & `apysc-4.4.3/apysc/_material_design/icon/material_rss_feed_outlined_icon.py`

 * *Files identical despite different names*

### Comparing `apysc-4.4.2/apysc/_material_design/icon/material_rtt_icon.py` & `apysc-4.4.3/apysc/_material_design/icon/material_rtt_icon.py`

 * *Files identical despite different names*

### Comparing `apysc-4.4.2/apysc/_material_design/icon/material_rule_icon.py` & `apysc-4.4.3/apysc/_material_design/icon/material_rule_icon.py`

 * *Files identical despite different names*

### Comparing `apysc-4.4.2/apysc/_material_design/icon/material_rule_outlined_icon.py` & `apysc-4.4.3/apysc/_material_design/icon/material_rule_outlined_icon.py`

 * *Files identical despite different names*

### Comparing `apysc-4.4.2/apysc/_material_design/icon/material_save_alt_icon.py` & `apysc-4.4.3/apysc/_material_design/icon/material_save_alt_icon.py`

 * *Files identical despite different names*

### Comparing `apysc-4.4.2/apysc/_material_design/icon/material_save_alt_outlined_icon.py` & `apysc-4.4.3/apysc/_material_design/icon/material_save_alt_outlined_icon.py`

 * *Files identical despite different names*

### Comparing `apysc-4.4.2/apysc/_material_design/icon/material_save_icon.py` & `apysc-4.4.3/apysc/_material_design/icon/material_save_icon.py`

 * *Files identical despite different names*

### Comparing `apysc-4.4.2/apysc/_material_design/icon/material_save_outlined_icon.py` & `apysc-4.4.3/apysc/_material_design/icon/material_save_outlined_icon.py`

 * *Files identical despite different names*

### Comparing `apysc-4.4.2/apysc/_material_design/icon/material_saved_search_icon.py` & `apysc-4.4.3/apysc/_material_design/icon/material_saved_search_icon.py`

 * *Files identical despite different names*

### Comparing `apysc-4.4.2/apysc/_material_design/icon/material_schedule_icon.py` & `apysc-4.4.3/apysc/_material_design/icon/material_schedule_icon.py`

 * *Files identical despite different names*

### Comparing `apysc-4.4.2/apysc/_material_design/icon/material_schedule_outlined_icon.py` & `apysc-4.4.3/apysc/_material_design/icon/material_schedule_outlined_icon.py`

 * *Files identical despite different names*

### Comparing `apysc-4.4.2/apysc/_material_design/icon/material_schedule_send_icon.py` & `apysc-4.4.3/apysc/_material_design/icon/material_schedule_send_icon.py`

 * *Files identical despite different names*

### Comparing `apysc-4.4.2/apysc/_material_design/icon/material_screen_share_icon.py` & `apysc-4.4.3/apysc/_material_design/icon/material_screen_share_icon.py`

 * *Files identical despite different names*

### Comparing `apysc-4.4.2/apysc/_material_design/icon/material_screen_share_outlined_icon.py` & `apysc-4.4.3/apysc/_material_design/icon/material_screen_share_outlined_icon.py`

 * *Files identical despite different names*

### Comparing `apysc-4.4.2/apysc/_material_design/icon/material_sd_icon.py` & `apysc-4.4.3/apysc/_material_design/icon/material_sd_icon.py`

 * *Files identical despite different names*

### Comparing `apysc-4.4.2/apysc/_material_design/icon/material_search_icon.py` & `apysc-4.4.3/apysc/_material_design/icon/material_search_icon.py`

 * *Files identical despite different names*

### Comparing `apysc-4.4.2/apysc/_material_design/icon/material_search_off_icon.py` & `apysc-4.4.3/apysc/_material_design/icon/material_search_off_icon.py`

 * *Files identical despite different names*

### Comparing `apysc-4.4.2/apysc/_material_design/icon/material_search_off_outlined_icon.py` & `apysc-4.4.3/apysc/_material_design/icon/material_search_off_outlined_icon.py`

 * *Files identical despite different names*

### Comparing `apysc-4.4.2/apysc/_material_design/icon/material_search_outlined_icon.py` & `apysc-4.4.3/apysc/_material_design/icon/material_search_outlined_icon.py`

 * *Files identical despite different names*

### Comparing `apysc-4.4.2/apysc/_material_design/icon/material_segment_icon.py` & `apysc-4.4.3/apysc/_material_design/icon/material_segment_icon.py`

 * *Files identical despite different names*

### Comparing `apysc-4.4.2/apysc/_material_design/icon/material_select_all_icon.py` & `apysc-4.4.3/apysc/_material_design/icon/material_select_all_icon.py`

 * *Files identical despite different names*

### Comparing `apysc-4.4.2/apysc/_material_design/icon/material_select_all_outlined_icon.py` & `apysc-4.4.3/apysc/_material_design/icon/material_select_all_outlined_icon.py`

 * *Files identical despite different names*

### Comparing `apysc-4.4.2/apysc/_material_design/icon/material_send_and_archive_icon.py` & `apysc-4.4.3/apysc/_material_design/icon/material_send_and_archive_icon.py`

 * *Files identical despite different names*

### Comparing `apysc-4.4.2/apysc/_material_design/icon/material_send_icon.py` & `apysc-4.4.3/apysc/_material_design/icon/material_send_icon.py`

 * *Files identical despite different names*

### Comparing `apysc-4.4.2/apysc/_material_design/icon/material_send_outlined_icon.py` & `apysc-4.4.3/apysc/_material_design/icon/material_send_outlined_icon.py`

 * *Files identical despite different names*

### Comparing `apysc-4.4.2/apysc/_material_design/icon/material_sentiment_satisfied_alt_icon.py` & `apysc-4.4.3/apysc/_material_design/icon/material_sentiment_satisfied_alt_icon.py`

 * *Files identical despite different names*

### Comparing `apysc-4.4.2/apysc/_material_design/icon/material_sentiment_satisfied_alt_outlined_icon.py` & `apysc-4.4.3/apysc/_material_design/icon/material_sentiment_satisfied_alt_outlined_icon.py`

 * *Files identical despite different names*

### Comparing `apysc-4.4.2/apysc/_material_design/icon/material_settings_applications_icon.py` & `apysc-4.4.3/apysc/_material_design/icon/material_settings_applications_icon.py`

 * *Files identical despite different names*

### Comparing `apysc-4.4.2/apysc/_material_design/icon/material_settings_applications_outlined_icon.py` & `apysc-4.4.3/apysc/_material_design/icon/material_settings_applications_outlined_icon.py`

 * *Files identical despite different names*

### Comparing `apysc-4.4.2/apysc/_material_design/icon/material_settings_backup_restore_icon.py` & `apysc-4.4.3/apysc/_material_design/icon/material_settings_backup_restore_icon.py`

 * *Files identical despite different names*

### Comparing `apysc-4.4.2/apysc/_material_design/icon/material_settings_backup_restore_outlined_icon.py` & `apysc-4.4.3/apysc/_material_design/icon/material_settings_backup_restore_outlined_icon.py`

 * *Files identical despite different names*

### Comparing `apysc-4.4.2/apysc/_material_design/icon/material_settings_bluetooth_icon.py` & `apysc-4.4.3/apysc/_material_design/icon/material_settings_bluetooth_icon.py`

 * *Files identical despite different names*

### Comparing `apysc-4.4.2/apysc/_material_design/icon/material_settings_bluetooth_outlined_icon.py` & `apysc-4.4.3/apysc/_material_design/icon/material_settings_bluetooth_outlined_icon.py`

 * *Files identical despite different names*

### Comparing `apysc-4.4.2/apysc/_material_design/icon/material_settings_brightness_icon.py` & `apysc-4.4.3/apysc/_material_design/icon/material_settings_brightness_icon.py`

 * *Files identical despite different names*

### Comparing `apysc-4.4.2/apysc/_material_design/icon/material_settings_brightness_outlined_icon.py` & `apysc-4.4.3/apysc/_material_design/icon/material_settings_brightness_outlined_icon.py`

 * *Files identical despite different names*

### Comparing `apysc-4.4.2/apysc/_material_design/icon/material_settings_cell_icon.py` & `apysc-4.4.3/apysc/_material_design/icon/material_settings_cell_icon.py`

 * *Files identical despite different names*

### Comparing `apysc-4.4.2/apysc/_material_design/icon/material_settings_cell_outlined_icon.py` & `apysc-4.4.3/apysc/_material_design/icon/material_settings_cell_outlined_icon.py`

 * *Files identical despite different names*

### Comparing `apysc-4.4.2/apysc/_material_design/icon/material_settings_ethernet_icon.py` & `apysc-4.4.3/apysc/_material_design/icon/material_settings_ethernet_icon.py`

 * *Files identical despite different names*

### Comparing `apysc-4.4.2/apysc/_material_design/icon/material_settings_ethernet_outlined_icon.py` & `apysc-4.4.3/apysc/_material_design/icon/material_settings_ethernet_outlined_icon.py`

 * *Files identical despite different names*

### Comparing `apysc-4.4.2/apysc/_material_design/icon/material_settings_icon.py` & `apysc-4.4.3/apysc/_material_design/icon/material_settings_icon.py`

 * *Files identical despite different names*

### Comparing `apysc-4.4.2/apysc/_material_design/icon/material_settings_input_antenna_icon.py` & `apysc-4.4.3/apysc/_material_design/icon/material_settings_input_antenna_icon.py`

 * *Files identical despite different names*

### Comparing `apysc-4.4.2/apysc/_material_design/icon/material_settings_input_antenna_outlined_icon.py` & `apysc-4.4.3/apysc/_material_design/icon/material_settings_input_antenna_outlined_icon.py`

 * *Files identical despite different names*

### Comparing `apysc-4.4.2/apysc/_material_design/icon/material_settings_input_component_icon.py` & `apysc-4.4.3/apysc/_material_design/icon/material_settings_input_component_icon.py`

 * *Files identical despite different names*

### Comparing `apysc-4.4.2/apysc/_material_design/icon/material_settings_input_component_outlined_icon.py` & `apysc-4.4.3/apysc/_material_design/icon/material_settings_input_component_outlined_icon.py`

 * *Files identical despite different names*

### Comparing `apysc-4.4.2/apysc/_material_design/icon/material_settings_input_composite_icon.py` & `apysc-4.4.3/apysc/_material_design/icon/material_settings_input_composite_icon.py`

 * *Files identical despite different names*

### Comparing `apysc-4.4.2/apysc/_material_design/icon/material_settings_input_composite_outlined_icon.py` & `apysc-4.4.3/apysc/_material_design/icon/material_settings_input_composite_outlined_icon.py`

 * *Files identical despite different names*

### Comparing `apysc-4.4.2/apysc/_material_design/icon/material_settings_input_hdmi_icon.py` & `apysc-4.4.3/apysc/_material_design/icon/material_settings_input_hdmi_icon.py`

 * *Files identical despite different names*

### Comparing `apysc-4.4.2/apysc/_material_design/icon/material_settings_input_hdmi_outlined_icon.py` & `apysc-4.4.3/apysc/_material_design/icon/material_settings_input_hdmi_outlined_icon.py`

 * *Files identical despite different names*

### Comparing `apysc-4.4.2/apysc/_material_design/icon/material_settings_input_svideo_icon.py` & `apysc-4.4.3/apysc/_material_design/icon/material_settings_input_svideo_icon.py`

 * *Files identical despite different names*

### Comparing `apysc-4.4.2/apysc/_material_design/icon/material_settings_input_svideo_outlined_icon.py` & `apysc-4.4.3/apysc/_material_design/icon/material_settings_input_svideo_outlined_icon.py`

 * *Files identical despite different names*

### Comparing `apysc-4.4.2/apysc/_material_design/icon/material_settings_outlined_icon.py` & `apysc-4.4.3/apysc/_material_design/icon/material_settings_outlined_icon.py`

 * *Files identical despite different names*

### Comparing `apysc-4.4.2/apysc/_material_design/icon/material_settings_overscan_icon.py` & `apysc-4.4.3/apysc/_material_design/icon/material_settings_overscan_icon.py`

 * *Files identical despite different names*

### Comparing `apysc-4.4.2/apysc/_material_design/icon/material_settings_overscan_outlined_icon.py` & `apysc-4.4.3/apysc/_material_design/icon/material_settings_overscan_outlined_icon.py`

 * *Files identical despite different names*

### Comparing `apysc-4.4.2/apysc/_material_design/icon/material_settings_phone_icon.py` & `apysc-4.4.3/apysc/_material_design/icon/material_settings_phone_icon.py`

 * *Files identical despite different names*

### Comparing `apysc-4.4.2/apysc/_material_design/icon/material_settings_phone_outlined_icon.py` & `apysc-4.4.3/apysc/_material_design/icon/material_settings_phone_outlined_icon.py`

 * *Files identical despite different names*

### Comparing `apysc-4.4.2/apysc/_material_design/icon/material_settings_power_icon.py` & `apysc-4.4.3/apysc/_material_design/icon/material_settings_power_icon.py`

 * *Files identical despite different names*

### Comparing `apysc-4.4.2/apysc/_material_design/icon/material_settings_power_outlined_icon.py` & `apysc-4.4.3/apysc/_material_design/icon/material_settings_power_outlined_icon.py`

 * *Files identical despite different names*

### Comparing `apysc-4.4.2/apysc/_material_design/icon/material_settings_remote_icon.py` & `apysc-4.4.3/apysc/_material_design/icon/material_settings_remote_icon.py`

 * *Files identical despite different names*

### Comparing `apysc-4.4.2/apysc/_material_design/icon/material_settings_remote_outlined_icon.py` & `apysc-4.4.3/apysc/_material_design/icon/material_settings_remote_outlined_icon.py`

 * *Files identical despite different names*

### Comparing `apysc-4.4.2/apysc/_material_design/icon/material_settings_voice_icon.py` & `apysc-4.4.3/apysc/_material_design/icon/material_settings_voice_icon.py`

 * *Files identical despite different names*

### Comparing `apysc-4.4.2/apysc/_material_design/icon/material_settings_voice_outlined_icon.py` & `apysc-4.4.3/apysc/_material_design/icon/material_settings_voice_outlined_icon.py`

 * *Files identical despite different names*

### Comparing `apysc-4.4.2/apysc/_material_design/icon/material_shop_icon.py` & `apysc-4.4.3/apysc/_material_design/icon/material_shop_icon.py`

 * *Files identical despite different names*

### Comparing `apysc-4.4.2/apysc/_material_design/icon/material_shop_outlined_icon.py` & `apysc-4.4.3/apysc/_material_design/icon/material_shop_outlined_icon.py`

 * *Files identical despite different names*

### Comparing `apysc-4.4.2/apysc/_material_design/icon/material_shop_two_icon.py` & `apysc-4.4.3/apysc/_material_design/icon/material_shop_two_icon.py`

 * *Files identical despite different names*

### Comparing `apysc-4.4.2/apysc/_material_design/icon/material_shop_two_outlined_icon.py` & `apysc-4.4.3/apysc/_material_design/icon/material_shop_two_outlined_icon.py`

 * *Files identical despite different names*

### Comparing `apysc-4.4.2/apysc/_material_design/icon/material_shopping_bag_icon.py` & `apysc-4.4.3/apysc/_material_design/icon/material_shopping_bag_icon.py`

 * *Files identical despite different names*

### Comparing `apysc-4.4.2/apysc/_material_design/icon/material_shopping_bag_outlined_icon.py` & `apysc-4.4.3/apysc/_material_design/icon/material_shopping_bag_outlined_icon.py`

 * *Files identical despite different names*

### Comparing `apysc-4.4.2/apysc/_material_design/icon/material_shopping_basket_icon.py` & `apysc-4.4.3/apysc/_material_design/icon/material_shopping_basket_icon.py`

 * *Files identical despite different names*

### Comparing `apysc-4.4.2/apysc/_material_design/icon/material_shopping_basket_outlined_icon.py` & `apysc-4.4.3/apysc/_material_design/icon/material_shopping_basket_outlined_icon.py`

 * *Files identical despite different names*

### Comparing `apysc-4.4.2/apysc/_material_design/icon/material_shopping_cart_icon.py` & `apysc-4.4.3/apysc/_material_design/icon/material_shopping_cart_icon.py`

 * *Files identical despite different names*

### Comparing `apysc-4.4.2/apysc/_material_design/icon/material_shopping_cart_outlined_icon.py` & `apysc-4.4.3/apysc/_material_design/icon/material_shopping_cart_outlined_icon.py`

 * *Files identical despite different names*

### Comparing `apysc-4.4.2/apysc/_material_design/icon/material_shuffle_icon.py` & `apysc-4.4.3/apysc/_material_design/icon/material_shuffle_icon.py`

 * *Files identical despite different names*

### Comparing `apysc-4.4.2/apysc/_material_design/icon/material_shuffle_on_icon.py` & `apysc-4.4.3/apysc/_material_design/icon/material_shuffle_on_icon.py`

 * *Files identical despite different names*

### Comparing `apysc-4.4.2/apysc/_material_design/icon/material_shuffle_outlined_icon.py` & `apysc-4.4.3/apysc/_material_design/icon/material_shuffle_outlined_icon.py`

 * *Files identical despite different names*

### Comparing `apysc-4.4.2/apysc/_material_design/icon/material_skip_next_icon.py` & `apysc-4.4.3/apysc/_material_design/icon/material_skip_next_icon.py`

 * *Files identical despite different names*

### Comparing `apysc-4.4.2/apysc/_material_design/icon/material_skip_next_outlined_icon.py` & `apysc-4.4.3/apysc/_material_design/icon/material_skip_next_outlined_icon.py`

 * *Files identical despite different names*

### Comparing `apysc-4.4.2/apysc/_material_design/icon/material_skip_previous_icon.py` & `apysc-4.4.3/apysc/_material_design/icon/material_skip_previous_icon.py`

 * *Files identical despite different names*

### Comparing `apysc-4.4.2/apysc/_material_design/icon/material_skip_previous_outlined_icon.py` & `apysc-4.4.3/apysc/_material_design/icon/material_skip_previous_outlined_icon.py`

 * *Files identical despite different names*

### Comparing `apysc-4.4.2/apysc/_material_design/icon/material_slow_motion_video_icon.py` & `apysc-4.4.3/apysc/_material_design/icon/material_slow_motion_video_icon.py`

 * *Files identical despite different names*

### Comparing `apysc-4.4.2/apysc/_material_design/icon/material_slow_motion_video_outlined_icon.py` & `apysc-4.4.3/apysc/_material_design/icon/material_slow_motion_video_outlined_icon.py`

 * *Files identical despite different names*

### Comparing `apysc-4.4.2/apysc/_material_design/icon/material_smart_button_icon.py` & `apysc-4.4.3/apysc/_material_design/icon/material_smart_button_icon.py`

 * *Files identical despite different names*

### Comparing `apysc-4.4.2/apysc/_material_design/icon/material_smart_button_outlined_icon.py` & `apysc-4.4.3/apysc/_material_design/icon/material_smart_button_outlined_icon.py`

 * *Files identical despite different names*

### Comparing `apysc-4.4.2/apysc/_material_design/icon/material_snooze_icon.py` & `apysc-4.4.3/apysc/_material_design/icon/material_snooze_icon.py`

 * *Files identical despite different names*

### Comparing `apysc-4.4.2/apysc/_material_design/icon/material_snooze_outlined_icon.py` & `apysc-4.4.3/apysc/_material_design/icon/material_snooze_outlined_icon.py`

 * *Files identical despite different names*

### Comparing `apysc-4.4.2/apysc/_material_design/icon/material_sort_by_alpha_icon.py` & `apysc-4.4.3/apysc/_material_design/icon/material_sort_by_alpha_icon.py`

 * *Files identical despite different names*

### Comparing `apysc-4.4.2/apysc/_material_design/icon/material_sort_by_alpha_outlined_icon.py` & `apysc-4.4.3/apysc/_material_design/icon/material_sort_by_alpha_outlined_icon.py`

 * *Files identical despite different names*

### Comparing `apysc-4.4.2/apysc/_material_design/icon/material_source_icon.py` & `apysc-4.4.3/apysc/_material_design/icon/material_source_icon.py`

 * *Files identical despite different names*

### Comparing `apysc-4.4.2/apysc/_material_design/icon/material_source_outlined_icon.py` & `apysc-4.4.3/apysc/_material_design/icon/material_source_outlined_icon.py`

 * *Files identical despite different names*

### Comparing `apysc-4.4.2/apysc/_material_design/icon/material_speaker_notes_icon.py` & `apysc-4.4.3/apysc/_material_design/icon/material_speaker_notes_icon.py`

 * *Files identical despite different names*

### Comparing `apysc-4.4.2/apysc/_material_design/icon/material_speaker_notes_off_icon.py` & `apysc-4.4.3/apysc/_material_design/icon/material_speaker_notes_off_icon.py`

 * *Files identical despite different names*

### Comparing `apysc-4.4.2/apysc/_material_design/icon/material_speaker_notes_off_outlined_icon.py` & `apysc-4.4.3/apysc/_material_design/icon/material_speaker_notes_off_outlined_icon.py`

 * *Files identical despite different names*

### Comparing `apysc-4.4.2/apysc/_material_design/icon/material_speaker_notes_outlined_icon.py` & `apysc-4.4.3/apysc/_material_design/icon/material_speaker_notes_outlined_icon.py`

 * *Files identical despite different names*

### Comparing `apysc-4.4.2/apysc/_material_design/icon/material_speaker_phone_icon.py` & `apysc-4.4.3/apysc/_material_design/icon/material_speaker_phone_icon.py`

 * *Files identical despite different names*

### Comparing `apysc-4.4.2/apysc/_material_design/icon/material_speaker_phone_outlined_icon.py` & `apysc-4.4.3/apysc/_material_design/icon/material_speaker_phone_outlined_icon.py`

 * *Files identical despite different names*

### Comparing `apysc-4.4.2/apysc/_material_design/icon/material_speed_icon.py` & `apysc-4.4.3/apysc/_material_design/icon/material_speed_icon.py`

 * *Files identical despite different names*

### Comparing `apysc-4.4.2/apysc/_material_design/icon/material_speed_outlined_icon.py` & `apysc-4.4.3/apysc/_material_design/icon/material_speed_outlined_icon.py`

 * *Files identical despite different names*

### Comparing `apysc-4.4.2/apysc/_material_design/icon/material_spellcheck_icon.py` & `apysc-4.4.3/apysc/_material_design/icon/material_spellcheck_icon.py`

 * *Files identical despite different names*

### Comparing `apysc-4.4.2/apysc/_material_design/icon/material_spellcheck_outlined_icon.py` & `apysc-4.4.3/apysc/_material_design/icon/material_spellcheck_outlined_icon.py`

 * *Files identical despite different names*

### Comparing `apysc-4.4.2/apysc/_material_design/icon/material_star_rate_icon.py` & `apysc-4.4.3/apysc/_material_design/icon/material_star_rate_icon.py`

 * *Files identical despite different names*

### Comparing `apysc-4.4.2/apysc/_material_design/icon/material_star_rate_outlined_icon.py` & `apysc-4.4.3/apysc/_material_design/icon/material_star_rate_outlined_icon.py`

 * *Files identical despite different names*

### Comparing `apysc-4.4.2/apysc/_material_design/icon/material_stars_icon.py` & `apysc-4.4.3/apysc/_material_design/icon/material_stars_icon.py`

 * *Files identical despite different names*

### Comparing `apysc-4.4.2/apysc/_material_design/icon/material_stars_outlined_icon.py` & `apysc-4.4.3/apysc/_material_design/icon/material_stars_outlined_icon.py`

 * *Files identical despite different names*

### Comparing `apysc-4.4.2/apysc/_material_design/icon/material_stay_current_landscape_icon.py` & `apysc-4.4.3/apysc/_material_design/icon/material_stay_current_landscape_icon.py`

 * *Files identical despite different names*

### Comparing `apysc-4.4.2/apysc/_material_design/icon/material_stay_current_landscape_outlined_icon.py` & `apysc-4.4.3/apysc/_material_design/icon/material_stay_current_landscape_outlined_icon.py`

 * *Files identical despite different names*

### Comparing `apysc-4.4.2/apysc/_material_design/icon/material_stay_current_portrait_icon.py` & `apysc-4.4.3/apysc/_material_design/icon/material_stay_current_portrait_icon.py`

 * *Files identical despite different names*

### Comparing `apysc-4.4.2/apysc/_material_design/icon/material_stay_current_portrait_outlined_icon.py` & `apysc-4.4.3/apysc/_material_design/icon/material_stay_current_portrait_outlined_icon.py`

 * *Files identical despite different names*

### Comparing `apysc-4.4.2/apysc/_material_design/icon/material_stay_primary_landscape_icon.py` & `apysc-4.4.3/apysc/_material_design/icon/material_stay_primary_landscape_icon.py`

 * *Files identical despite different names*

### Comparing `apysc-4.4.2/apysc/_material_design/icon/material_stay_primary_landscape_outlined_icon.py` & `apysc-4.4.3/apysc/_material_design/icon/material_stay_primary_landscape_outlined_icon.py`

 * *Files identical despite different names*

### Comparing `apysc-4.4.2/apysc/_material_design/icon/material_stay_primary_portrait_icon.py` & `apysc-4.4.3/apysc/_material_design/icon/material_stay_primary_portrait_icon.py`

 * *Files identical despite different names*

### Comparing `apysc-4.4.2/apysc/_material_design/icon/material_stay_primary_portrait_outlined_icon.py` & `apysc-4.4.3/apysc/_material_design/icon/material_stay_primary_portrait_outlined_icon.py`

 * *Files identical despite different names*

### Comparing `apysc-4.4.2/apysc/_material_design/icon/material_sticky_note_2_icon.py` & `apysc-4.4.3/apysc/_material_design/icon/material_sticky_note_2_icon.py`

 * *Files identical despite different names*

### Comparing `apysc-4.4.2/apysc/_material_design/icon/material_sticky_note_2_outlined_icon.py` & `apysc-4.4.3/apysc/_material_design/icon/material_sticky_note_2_outlined_icon.py`

 * *Files identical despite different names*

### Comparing `apysc-4.4.2/apysc/_material_design/icon/material_stop_circle_icon.py` & `apysc-4.4.3/apysc/_material_design/icon/material_stop_circle_icon.py`

 * *Files identical despite different names*

### Comparing `apysc-4.4.2/apysc/_material_design/icon/material_stop_circle_outlined_icon.py` & `apysc-4.4.3/apysc/_material_design/icon/material_stop_circle_outlined_icon.py`

 * *Files identical despite different names*

### Comparing `apysc-4.4.2/apysc/_material_design/icon/material_stop_icon.py` & `apysc-4.4.3/apysc/_material_design/icon/material_stop_icon.py`

 * *Files identical despite different names*

### Comparing `apysc-4.4.2/apysc/_material_design/icon/material_stop_outlined_icon.py` & `apysc-4.4.3/apysc/_material_design/icon/material_stop_outlined_icon.py`

 * *Files identical despite different names*

### Comparing `apysc-4.4.2/apysc/_material_design/icon/material_stop_screen_share_icon.py` & `apysc-4.4.3/apysc/_material_design/icon/material_stop_screen_share_icon.py`

 * *Files identical despite different names*

### Comparing `apysc-4.4.2/apysc/_material_design/icon/material_stop_screen_share_outlined_icon.py` & `apysc-4.4.3/apysc/_material_design/icon/material_stop_screen_share_outlined_icon.py`

 * *Files identical despite different names*

### Comparing `apysc-4.4.2/apysc/_material_design/icon/material_store_icon.py` & `apysc-4.4.3/apysc/_material_design/icon/material_store_icon.py`

 * *Files identical despite different names*

### Comparing `apysc-4.4.2/apysc/_material_design/icon/material_store_outlined_icon.py` & `apysc-4.4.3/apysc/_material_design/icon/material_store_outlined_icon.py`

 * *Files identical despite different names*

### Comparing `apysc-4.4.2/apysc/_material_design/icon/material_subject_icon.py` & `apysc-4.4.3/apysc/_material_design/icon/material_subject_icon.py`

 * *Files identical despite different names*

### Comparing `apysc-4.4.2/apysc/_material_design/icon/material_subject_outlined_icon.py` & `apysc-4.4.3/apysc/_material_design/icon/material_subject_outlined_icon.py`

 * *Files identical despite different names*

### Comparing `apysc-4.4.2/apysc/_material_design/icon/material_subscriptions_icon.py` & `apysc-4.4.3/apysc/_material_design/icon/material_subscriptions_icon.py`

 * *Files identical despite different names*

### Comparing `apysc-4.4.2/apysc/_material_design/icon/material_subscriptions_outlined_icon.py` & `apysc-4.4.3/apysc/_material_design/icon/material_subscriptions_outlined_icon.py`

 * *Files identical despite different names*

### Comparing `apysc-4.4.2/apysc/_material_design/icon/material_subtitles_icon.py` & `apysc-4.4.3/apysc/_material_design/icon/material_subtitles_icon.py`

 * *Files identical despite different names*

### Comparing `apysc-4.4.2/apysc/_material_design/icon/material_subtitles_off_icon.py` & `apysc-4.4.3/apysc/_material_design/icon/material_subtitles_off_icon.py`

 * *Files identical despite different names*

### Comparing `apysc-4.4.2/apysc/_material_design/icon/material_subtitles_off_outlined_icon.py` & `apysc-4.4.3/apysc/_material_design/icon/material_subtitles_off_outlined_icon.py`

 * *Files identical despite different names*

### Comparing `apysc-4.4.2/apysc/_material_design/icon/material_subtitles_outlined_icon.py` & `apysc-4.4.3/apysc/_material_design/icon/material_subtitles_outlined_icon.py`

 * *Files identical despite different names*

### Comparing `apysc-4.4.2/apysc/_material_design/icon/material_supervised_user_circle_icon.py` & `apysc-4.4.3/apysc/_material_design/icon/material_supervised_user_circle_icon.py`

 * *Files identical despite different names*

### Comparing `apysc-4.4.2/apysc/_material_design/icon/material_supervised_user_circle_outlined_icon.py` & `apysc-4.4.3/apysc/_material_design/icon/material_supervised_user_circle_outlined_icon.py`

 * *Files identical despite different names*

### Comparing `apysc-4.4.2/apysc/_material_design/icon/material_supervisor_account_icon.py` & `apysc-4.4.3/apysc/_material_design/icon/material_supervisor_account_icon.py`

 * *Files identical despite different names*

### Comparing `apysc-4.4.2/apysc/_material_design/icon/material_supervisor_account_outlined_icon.py` & `apysc-4.4.3/apysc/_material_design/icon/material_supervisor_account_outlined_icon.py`

 * *Files identical despite different names*

### Comparing `apysc-4.4.2/apysc/_material_design/icon/material_support_icon.py` & `apysc-4.4.3/apysc/_material_design/icon/material_support_icon.py`

 * *Files identical despite different names*

### Comparing `apysc-4.4.2/apysc/_material_design/icon/material_support_outlined_icon.py` & `apysc-4.4.3/apysc/_material_design/icon/material_support_outlined_icon.py`

 * *Files identical despite different names*

### Comparing `apysc-4.4.2/apysc/_material_design/icon/material_surround_sound_icon.py` & `apysc-4.4.3/apysc/_material_design/icon/material_surround_sound_icon.py`

 * *Files identical despite different names*

### Comparing `apysc-4.4.2/apysc/_material_design/icon/material_surround_sound_outlined_icon.py` & `apysc-4.4.3/apysc/_material_design/icon/material_surround_sound_outlined_icon.py`

 * *Files identical despite different names*

### Comparing `apysc-4.4.2/apysc/_material_design/icon/material_swap_calls_icon.py` & `apysc-4.4.3/apysc/_material_design/icon/material_swap_calls_icon.py`

 * *Files identical despite different names*

### Comparing `apysc-4.4.2/apysc/_material_design/icon/material_swap_calls_outlined_icon.py` & `apysc-4.4.3/apysc/_material_design/icon/material_swap_calls_outlined_icon.py`

 * *Files identical despite different names*

### Comparing `apysc-4.4.2/apysc/_material_design/icon/material_swap_horiz_icon.py` & `apysc-4.4.3/apysc/_material_design/icon/material_swap_horiz_icon.py`

 * *Files identical despite different names*

### Comparing `apysc-4.4.2/apysc/_material_design/icon/material_swap_horiz_outlined_icon.py` & `apysc-4.4.3/apysc/_material_design/icon/material_swap_horiz_outlined_icon.py`

 * *Files identical despite different names*

### Comparing `apysc-4.4.2/apysc/_material_design/icon/material_swap_horizontal_circle_icon.py` & `apysc-4.4.3/apysc/_material_design/icon/material_swap_horizontal_circle_icon.py`

 * *Files identical despite different names*

### Comparing `apysc-4.4.2/apysc/_material_design/icon/material_swap_horizontal_circle_outlined_icon.py` & `apysc-4.4.3/apysc/_material_design/icon/material_swap_horizontal_circle_outlined_icon.py`

 * *Files identical despite different names*

### Comparing `apysc-4.4.2/apysc/_material_design/icon/material_swap_vert_icon.py` & `apysc-4.4.3/apysc/_material_design/icon/material_swap_vert_icon.py`

 * *Files identical despite different names*

### Comparing `apysc-4.4.2/apysc/_material_design/icon/material_swap_vert_outlined_icon.py` & `apysc-4.4.3/apysc/_material_design/icon/material_swap_vert_outlined_icon.py`

 * *Files identical despite different names*

### Comparing `apysc-4.4.2/apysc/_material_design/icon/material_swap_vertical_circle_icon.py` & `apysc-4.4.3/apysc/_material_design/icon/material_swap_vertical_circle_icon.py`

 * *Files identical despite different names*

### Comparing `apysc-4.4.2/apysc/_material_design/icon/material_swap_vertical_circle_outlined_icon.py` & `apysc-4.4.3/apysc/_material_design/icon/material_swap_vertical_circle_outlined_icon.py`

 * *Files identical despite different names*

### Comparing `apysc-4.4.2/apysc/_material_design/icon/material_swipe_icon.py` & `apysc-4.4.3/apysc/_material_design/icon/material_swipe_icon.py`

 * *Files identical despite different names*

### Comparing `apysc-4.4.2/apysc/_material_design/icon/material_sync_alt_icon.py` & `apysc-4.4.3/apysc/_material_design/icon/material_sync_alt_icon.py`

 * *Files identical despite different names*

### Comparing `apysc-4.4.2/apysc/_material_design/icon/material_sync_alt_outlined_icon.py` & `apysc-4.4.3/apysc/_material_design/icon/material_sync_alt_outlined_icon.py`

 * *Files identical despite different names*

### Comparing `apysc-4.4.2/apysc/_material_design/icon/material_system_update_alt_icon.py` & `apysc-4.4.3/apysc/_material_design/icon/material_system_update_alt_icon.py`

 * *Files identical despite different names*

### Comparing `apysc-4.4.2/apysc/_material_design/icon/material_system_update_alt_outlined_icon.py` & `apysc-4.4.3/apysc/_material_design/icon/material_system_update_alt_outlined_icon.py`

 * *Files identical despite different names*

### Comparing `apysc-4.4.2/apysc/_material_design/icon/material_tab_icon.py` & `apysc-4.4.3/apysc/_material_design/icon/material_tab_icon.py`

 * *Files identical despite different names*

### Comparing `apysc-4.4.2/apysc/_material_design/icon/material_tab_outlined_icon.py` & `apysc-4.4.3/apysc/_material_design/icon/material_tab_outlined_icon.py`

 * *Files identical despite different names*

### Comparing `apysc-4.4.2/apysc/_material_design/icon/material_tab_unselected_icon.py` & `apysc-4.4.3/apysc/_material_design/icon/material_tab_unselected_icon.py`

 * *Files identical despite different names*

### Comparing `apysc-4.4.2/apysc/_material_design/icon/material_tab_unselected_outlined_icon.py` & `apysc-4.4.3/apysc/_material_design/icon/material_tab_unselected_outlined_icon.py`

 * *Files identical despite different names*

### Comparing `apysc-4.4.2/apysc/_material_design/icon/material_table_view_icon.py` & `apysc-4.4.3/apysc/_material_design/icon/material_table_view_icon.py`

 * *Files identical despite different names*

### Comparing `apysc-4.4.2/apysc/_material_design/icon/material_table_view_outlined_icon.py` & `apysc-4.4.3/apysc/_material_design/icon/material_table_view_outlined_icon.py`

 * *Files identical despite different names*

### Comparing `apysc-4.4.2/apysc/_material_design/icon/material_text_rotate_up_icon.py` & `apysc-4.4.3/apysc/_material_design/icon/material_text_rotate_up_icon.py`

 * *Files identical despite different names*

### Comparing `apysc-4.4.2/apysc/_material_design/icon/material_text_rotate_up_outlined_icon.py` & `apysc-4.4.3/apysc/_material_design/icon/material_text_rotate_up_outlined_icon.py`

 * *Files identical despite different names*

### Comparing `apysc-4.4.2/apysc/_material_design/icon/material_text_rotate_vertical_icon.py` & `apysc-4.4.3/apysc/_material_design/icon/material_text_rotate_vertical_icon.py`

 * *Files identical despite different names*

### Comparing `apysc-4.4.2/apysc/_material_design/icon/material_text_rotate_vertical_outlined_icon.py` & `apysc-4.4.3/apysc/_material_design/icon/material_text_rotate_vertical_outlined_icon.py`

 * *Files identical despite different names*

### Comparing `apysc-4.4.2/apysc/_material_design/icon/material_text_rotation_angledown_icon.py` & `apysc-4.4.3/apysc/_material_design/icon/material_text_rotation_angledown_icon.py`

 * *Files identical despite different names*

### Comparing `apysc-4.4.2/apysc/_material_design/icon/material_text_rotation_angledown_outlined_icon.py` & `apysc-4.4.3/apysc/_material_design/icon/material_text_rotation_angledown_outlined_icon.py`

 * *Files identical despite different names*

### Comparing `apysc-4.4.2/apysc/_material_design/icon/material_text_rotation_angleup_icon.py` & `apysc-4.4.3/apysc/_material_design/icon/material_text_rotation_angleup_icon.py`

 * *Files identical despite different names*

### Comparing `apysc-4.4.2/apysc/_material_design/icon/material_text_rotation_angleup_outlined_icon.py` & `apysc-4.4.3/apysc/_material_design/icon/material_text_rotation_angleup_outlined_icon.py`

 * *Files identical despite different names*

### Comparing `apysc-4.4.2/apysc/_material_design/icon/material_text_rotation_down_icon.py` & `apysc-4.4.3/apysc/_material_design/icon/material_text_rotation_down_icon.py`

 * *Files identical despite different names*

### Comparing `apysc-4.4.2/apysc/_material_design/icon/material_text_rotation_down_outlined_icon.py` & `apysc-4.4.3/apysc/_material_design/icon/material_text_rotation_down_outlined_icon.py`

 * *Files identical despite different names*

### Comparing `apysc-4.4.2/apysc/_material_design/icon/material_text_rotation_none_icon.py` & `apysc-4.4.3/apysc/_material_design/icon/material_text_rotation_none_icon.py`

 * *Files identical despite different names*

### Comparing `apysc-4.4.2/apysc/_material_design/icon/material_text_rotation_none_outlined_icon.py` & `apysc-4.4.3/apysc/_material_design/icon/material_text_rotation_none_outlined_icon.py`

 * *Files identical despite different names*

### Comparing `apysc-4.4.2/apysc/_material_design/icon/material_textsms_icon.py` & `apysc-4.4.3/apysc/_material_design/icon/material_textsms_icon.py`

 * *Files identical despite different names*

### Comparing `apysc-4.4.2/apysc/_material_design/icon/material_textsms_outlined_icon.py` & `apysc-4.4.3/apysc/_material_design/icon/material_textsms_outlined_icon.py`

 * *Files identical despite different names*

### Comparing `apysc-4.4.2/apysc/_material_design/icon/material_theaters_icon.py` & `apysc-4.4.3/apysc/_material_design/icon/material_theaters_icon.py`

 * *Files identical despite different names*

### Comparing `apysc-4.4.2/apysc/_material_design/icon/material_theaters_outlined_icon.py` & `apysc-4.4.3/apysc/_material_design/icon/material_theaters_outlined_icon.py`

 * *Files identical despite different names*

### Comparing `apysc-4.4.2/apysc/_material_design/icon/material_thumb_down_icon.py` & `apysc-4.4.3/apysc/_material_design/icon/material_thumb_down_icon.py`

 * *Files identical despite different names*

### Comparing `apysc-4.4.2/apysc/_material_design/icon/material_thumb_down_off_alt_icon.py` & `apysc-4.4.3/apysc/_material_design/icon/material_thumb_down_off_alt_icon.py`

 * *Files identical despite different names*

### Comparing `apysc-4.4.2/apysc/_material_design/icon/material_thumb_down_outlined_icon.py` & `apysc-4.4.3/apysc/_material_design/icon/material_thumb_down_outlined_icon.py`

 * *Files identical despite different names*

### Comparing `apysc-4.4.2/apysc/_material_design/icon/material_thumb_up_icon.py` & `apysc-4.4.3/apysc/_material_design/icon/material_thumb_up_icon.py`

 * *Files identical despite different names*

### Comparing `apysc-4.4.2/apysc/_material_design/icon/material_thumb_up_off_alt_icon.py` & `apysc-4.4.3/apysc/_material_design/icon/material_thumb_up_off_alt_icon.py`

 * *Files identical despite different names*

### Comparing `apysc-4.4.2/apysc/_material_design/icon/material_thumb_up_outlined_icon.py` & `apysc-4.4.3/apysc/_material_design/icon/material_thumb_up_outlined_icon.py`

 * *Files identical despite different names*

### Comparing `apysc-4.4.2/apysc/_material_design/icon/material_thumbs_up_down_icon.py` & `apysc-4.4.3/apysc/_material_design/icon/material_thumbs_up_down_icon.py`

 * *Files identical despite different names*

### Comparing `apysc-4.4.2/apysc/_material_design/icon/material_thumbs_up_down_outlined_icon.py` & `apysc-4.4.3/apysc/_material_design/icon/material_thumbs_up_down_outlined_icon.py`

 * *Files identical despite different names*

### Comparing `apysc-4.4.2/apysc/_material_design/icon/material_timeline_icon.py` & `apysc-4.4.3/apysc/_material_design/icon/material_timeline_icon.py`

 * *Files identical despite different names*

### Comparing `apysc-4.4.2/apysc/_material_design/icon/material_timeline_outlined_icon.py` & `apysc-4.4.3/apysc/_material_design/icon/material_timeline_outlined_icon.py`

 * *Files identical despite different names*

### Comparing `apysc-4.4.2/apysc/_material_design/icon/material_toc_icon.py` & `apysc-4.4.3/apysc/_material_design/icon/material_toc_icon.py`

 * *Files identical despite different names*

### Comparing `apysc-4.4.2/apysc/_material_design/icon/material_toc_outlined_icon.py` & `apysc-4.4.3/apysc/_material_design/icon/material_toc_outlined_icon.py`

 * *Files identical despite different names*

### Comparing `apysc-4.4.2/apysc/_material_design/icon/material_today_icon.py` & `apysc-4.4.3/apysc/_material_design/icon/material_today_icon.py`

 * *Files identical despite different names*

### Comparing `apysc-4.4.2/apysc/_material_design/icon/material_today_outlined_icon.py` & `apysc-4.4.3/apysc/_material_design/icon/material_today_outlined_icon.py`

 * *Files identical despite different names*

### Comparing `apysc-4.4.2/apysc/_material_design/icon/material_toll_icon.py` & `apysc-4.4.3/apysc/_material_design/icon/material_toll_icon.py`

 * *Files identical despite different names*

### Comparing `apysc-4.4.2/apysc/_material_design/icon/material_toll_outlined_icon.py` & `apysc-4.4.3/apysc/_material_design/icon/material_toll_outlined_icon.py`

 * *Files identical despite different names*

### Comparing `apysc-4.4.2/apysc/_material_design/icon/material_touch_app_icon.py` & `apysc-4.4.3/apysc/_material_design/icon/material_touch_app_icon.py`

 * *Files identical despite different names*

### Comparing `apysc-4.4.2/apysc/_material_design/icon/material_touch_app_outlined_icon.py` & `apysc-4.4.3/apysc/_material_design/icon/material_touch_app_outlined_icon.py`

 * *Files identical despite different names*

### Comparing `apysc-4.4.2/apysc/_material_design/icon/material_tour_icon.py` & `apysc-4.4.3/apysc/_material_design/icon/material_tour_icon.py`

 * *Files identical despite different names*

### Comparing `apysc-4.4.2/apysc/_material_design/icon/material_tour_outlined_icon.py` & `apysc-4.4.3/apysc/_material_design/icon/material_tour_outlined_icon.py`

 * *Files identical despite different names*

### Comparing `apysc-4.4.2/apysc/_material_design/icon/material_track_changes_icon.py` & `apysc-4.4.3/apysc/_material_design/icon/material_track_changes_icon.py`

 * *Files identical despite different names*

### Comparing `apysc-4.4.2/apysc/_material_design/icon/material_track_changes_outlined_icon.py` & `apysc-4.4.3/apysc/_material_design/icon/material_track_changes_outlined_icon.py`

 * *Files identical despite different names*

### Comparing `apysc-4.4.2/apysc/_material_design/icon/material_translate_icon.py` & `apysc-4.4.3/apysc/_material_design/icon/material_translate_icon.py`

 * *Files identical despite different names*

### Comparing `apysc-4.4.2/apysc/_material_design/icon/material_translate_outlined_icon.py` & `apysc-4.4.3/apysc/_material_design/icon/material_translate_outlined_icon.py`

 * *Files identical despite different names*

### Comparing `apysc-4.4.2/apysc/_material_design/icon/material_trending_down_icon.py` & `apysc-4.4.3/apysc/_material_design/icon/material_trending_down_icon.py`

 * *Files identical despite different names*

### Comparing `apysc-4.4.2/apysc/_material_design/icon/material_trending_down_outlined_icon.py` & `apysc-4.4.3/apysc/_material_design/icon/material_trending_down_outlined_icon.py`

 * *Files identical despite different names*

### Comparing `apysc-4.4.2/apysc/_material_design/icon/material_trending_flat_icon.py` & `apysc-4.4.3/apysc/_material_design/icon/material_trending_flat_icon.py`

 * *Files identical despite different names*

### Comparing `apysc-4.4.2/apysc/_material_design/icon/material_trending_flat_outlined_icon.py` & `apysc-4.4.3/apysc/_material_design/icon/material_trending_flat_outlined_icon.py`

 * *Files identical despite different names*

### Comparing `apysc-4.4.2/apysc/_material_design/icon/material_trending_up_icon.py` & `apysc-4.4.3/apysc/_material_design/icon/material_trending_up_icon.py`

 * *Files identical despite different names*

### Comparing `apysc-4.4.2/apysc/_material_design/icon/material_trending_up_outlined_icon.py` & `apysc-4.4.3/apysc/_material_design/icon/material_trending_up_outlined_icon.py`

 * *Files identical despite different names*

### Comparing `apysc-4.4.2/apysc/_material_design/icon/material_turned_in_icon.py` & `apysc-4.4.3/apysc/_material_design/icon/material_turned_in_icon.py`

 * *Files identical despite different names*

### Comparing `apysc-4.4.2/apysc/_material_design/icon/material_turned_in_not_icon.py` & `apysc-4.4.3/apysc/_material_design/icon/material_turned_in_not_icon.py`

 * *Files identical despite different names*

### Comparing `apysc-4.4.2/apysc/_material_design/icon/material_turned_in_not_outlined_icon.py` & `apysc-4.4.3/apysc/_material_design/icon/material_turned_in_not_outlined_icon.py`

 * *Files identical despite different names*

### Comparing `apysc-4.4.2/apysc/_material_design/icon/material_turned_in_outlined_icon.py` & `apysc-4.4.3/apysc/_material_design/icon/material_turned_in_outlined_icon.py`

 * *Files identical despite different names*

### Comparing `apysc-4.4.2/apysc/_material_design/icon/material_unpublished_icon.py` & `apysc-4.4.3/apysc/_material_design/icon/material_unpublished_icon.py`

 * *Files identical despite different names*

### Comparing `apysc-4.4.2/apysc/_material_design/icon/material_unpublished_outlined_icon.py` & `apysc-4.4.3/apysc/_material_design/icon/material_unpublished_outlined_icon.py`

 * *Files identical despite different names*

### Comparing `apysc-4.4.2/apysc/_material_design/icon/material_unsubscribe_icon.py` & `apysc-4.4.3/apysc/_material_design/icon/material_unsubscribe_icon.py`

 * *Files identical despite different names*

### Comparing `apysc-4.4.2/apysc/_material_design/icon/material_unsubscribe_outlined_icon.py` & `apysc-4.4.3/apysc/_material_design/icon/material_unsubscribe_outlined_icon.py`

 * *Files identical despite different names*

### Comparing `apysc-4.4.2/apysc/_material_design/icon/material_update_icon.py` & `apysc-4.4.3/apysc/_material_design/icon/material_update_icon.py`

 * *Files identical despite different names*

### Comparing `apysc-4.4.2/apysc/_material_design/icon/material_update_outlined_icon.py` & `apysc-4.4.3/apysc/_material_design/icon/material_update_outlined_icon.py`

 * *Files identical despite different names*

### Comparing `apysc-4.4.2/apysc/_material_design/icon/material_upgrade_icon.py` & `apysc-4.4.3/apysc/_material_design/icon/material_upgrade_icon.py`

 * *Files identical despite different names*

### Comparing `apysc-4.4.2/apysc/_material_design/icon/material_upgrade_outlined_icon.py` & `apysc-4.4.3/apysc/_material_design/icon/material_upgrade_outlined_icon.py`

 * *Files identical despite different names*

### Comparing `apysc-4.4.2/apysc/_material_design/icon/material_verified_icon.py` & `apysc-4.4.3/apysc/_material_design/icon/material_verified_icon.py`

 * *Files identical despite different names*

### Comparing `apysc-4.4.2/apysc/_material_design/icon/material_verified_outlined_icon.py` & `apysc-4.4.3/apysc/_material_design/icon/material_verified_outlined_icon.py`

 * *Files identical despite different names*

### Comparing `apysc-4.4.2/apysc/_material_design/icon/material_verified_user_icon.py` & `apysc-4.4.3/apysc/_material_design/icon/material_verified_user_icon.py`

 * *Files identical despite different names*

### Comparing `apysc-4.4.2/apysc/_material_design/icon/material_verified_user_outlined_icon.py` & `apysc-4.4.3/apysc/_material_design/icon/material_verified_user_outlined_icon.py`

 * *Files identical despite different names*

### Comparing `apysc-4.4.2/apysc/_material_design/icon/material_vertical_split_icon.py` & `apysc-4.4.3/apysc/_material_design/icon/material_vertical_split_icon.py`

 * *Files identical despite different names*

### Comparing `apysc-4.4.2/apysc/_material_design/icon/material_vertical_split_outlined_icon.py` & `apysc-4.4.3/apysc/_material_design/icon/material_vertical_split_outlined_icon.py`

 * *Files identical despite different names*

### Comparing `apysc-4.4.2/apysc/_material_design/icon/material_video_call_icon.py` & `apysc-4.4.3/apysc/_material_design/icon/material_video_call_icon.py`

 * *Files identical despite different names*

### Comparing `apysc-4.4.2/apysc/_material_design/icon/material_video_call_outlined_icon.py` & `apysc-4.4.3/apysc/_material_design/icon/material_video_call_outlined_icon.py`

 * *Files identical despite different names*

### Comparing `apysc-4.4.2/apysc/_material_design/icon/material_video_label_icon.py` & `apysc-4.4.3/apysc/_material_design/icon/material_video_label_icon.py`

 * *Files identical despite different names*

### Comparing `apysc-4.4.2/apysc/_material_design/icon/material_video_label_outlined_icon.py` & `apysc-4.4.3/apysc/_material_design/icon/material_video_label_outlined_icon.py`

 * *Files identical despite different names*

### Comparing `apysc-4.4.2/apysc/_material_design/icon/material_video_library_icon.py` & `apysc-4.4.3/apysc/_material_design/icon/material_video_library_icon.py`

 * *Files identical despite different names*

### Comparing `apysc-4.4.2/apysc/_material_design/icon/material_video_library_outlined_icon.py` & `apysc-4.4.3/apysc/_material_design/icon/material_video_library_outlined_icon.py`

 * *Files identical despite different names*

### Comparing `apysc-4.4.2/apysc/_material_design/icon/material_video_settings_icon.py` & `apysc-4.4.3/apysc/_material_design/icon/material_video_settings_icon.py`

 * *Files identical despite different names*

### Comparing `apysc-4.4.2/apysc/_material_design/icon/material_video_settings_outlined_icon.py` & `apysc-4.4.3/apysc/_material_design/icon/material_video_settings_outlined_icon.py`

 * *Files identical despite different names*

### Comparing `apysc-4.4.2/apysc/_material_design/icon/material_videocam_icon.py` & `apysc-4.4.3/apysc/_material_design/icon/material_videocam_icon.py`

 * *Files identical despite different names*

### Comparing `apysc-4.4.2/apysc/_material_design/icon/material_videocam_off_icon.py` & `apysc-4.4.3/apysc/_material_design/icon/material_videocam_off_icon.py`

 * *Files identical despite different names*

### Comparing `apysc-4.4.2/apysc/_material_design/icon/material_videocam_off_outlined_icon.py` & `apysc-4.4.3/apysc/_material_design/icon/material_videocam_off_outlined_icon.py`

 * *Files identical despite different names*

### Comparing `apysc-4.4.2/apysc/_material_design/icon/material_videocam_outlined_icon.py` & `apysc-4.4.3/apysc/_material_design/icon/material_videocam_outlined_icon.py`

 * *Files identical despite different names*

### Comparing `apysc-4.4.2/apysc/_material_design/icon/material_view_agenda_icon.py` & `apysc-4.4.3/apysc/_material_design/icon/material_view_agenda_icon.py`

 * *Files identical despite different names*

### Comparing `apysc-4.4.2/apysc/_material_design/icon/material_view_agenda_outlined_icon.py` & `apysc-4.4.3/apysc/_material_design/icon/material_view_agenda_outlined_icon.py`

 * *Files identical despite different names*

### Comparing `apysc-4.4.2/apysc/_material_design/icon/material_view_array_icon.py` & `apysc-4.4.3/apysc/_material_design/icon/material_view_array_icon.py`

 * *Files identical despite different names*

### Comparing `apysc-4.4.2/apysc/_material_design/icon/material_view_array_outlined_icon.py` & `apysc-4.4.3/apysc/_material_design/icon/material_view_array_outlined_icon.py`

 * *Files identical despite different names*

### Comparing `apysc-4.4.2/apysc/_material_design/icon/material_view_carousel_icon.py` & `apysc-4.4.3/apysc/_material_design/icon/material_view_carousel_icon.py`

 * *Files identical despite different names*

### Comparing `apysc-4.4.2/apysc/_material_design/icon/material_view_carousel_outlined_icon.py` & `apysc-4.4.3/apysc/_material_design/icon/material_view_carousel_outlined_icon.py`

 * *Files identical despite different names*

### Comparing `apysc-4.4.2/apysc/_material_design/icon/material_view_column_icon.py` & `apysc-4.4.3/apysc/_material_design/icon/material_view_column_icon.py`

 * *Files identical despite different names*

### Comparing `apysc-4.4.2/apysc/_material_design/icon/material_view_column_outlined_icon.py` & `apysc-4.4.3/apysc/_material_design/icon/material_view_column_outlined_icon.py`

 * *Files identical despite different names*

### Comparing `apysc-4.4.2/apysc/_material_design/icon/material_view_day_icon.py` & `apysc-4.4.3/apysc/_material_design/icon/material_view_day_icon.py`

 * *Files identical despite different names*

### Comparing `apysc-4.4.2/apysc/_material_design/icon/material_view_day_outlined_icon.py` & `apysc-4.4.3/apysc/_material_design/icon/material_view_day_outlined_icon.py`

 * *Files identical despite different names*

### Comparing `apysc-4.4.2/apysc/_material_design/icon/material_view_headline_icon.py` & `apysc-4.4.3/apysc/_material_design/icon/material_view_headline_icon.py`

 * *Files identical despite different names*

### Comparing `apysc-4.4.2/apysc/_material_design/icon/material_view_headline_outlined_icon.py` & `apysc-4.4.3/apysc/_material_design/icon/material_view_headline_outlined_icon.py`

 * *Files identical despite different names*

### Comparing `apysc-4.4.2/apysc/_material_design/icon/material_view_in_ar_icon.py` & `apysc-4.4.3/apysc/_material_design/icon/material_view_in_ar_icon.py`

 * *Files identical despite different names*

### Comparing `apysc-4.4.2/apysc/_material_design/icon/material_view_list_icon.py` & `apysc-4.4.3/apysc/_material_design/icon/material_view_list_icon.py`

 * *Files identical despite different names*

### Comparing `apysc-4.4.2/apysc/_material_design/icon/material_view_list_outlined_icon.py` & `apysc-4.4.3/apysc/_material_design/icon/material_view_list_outlined_icon.py`

 * *Files identical despite different names*

### Comparing `apysc-4.4.2/apysc/_material_design/icon/material_view_module_icon.py` & `apysc-4.4.3/apysc/_material_design/icon/material_view_module_icon.py`

 * *Files identical despite different names*

### Comparing `apysc-4.4.2/apysc/_material_design/icon/material_view_module_outlined_icon.py` & `apysc-4.4.3/apysc/_material_design/icon/material_view_module_outlined_icon.py`

 * *Files identical despite different names*

### Comparing `apysc-4.4.2/apysc/_material_design/icon/material_view_quilt_icon.py` & `apysc-4.4.3/apysc/_material_design/icon/material_view_quilt_icon.py`

 * *Files identical despite different names*

### Comparing `apysc-4.4.2/apysc/_material_design/icon/material_view_quilt_outlined_icon.py` & `apysc-4.4.3/apysc/_material_design/icon/material_view_quilt_outlined_icon.py`

 * *Files identical despite different names*

### Comparing `apysc-4.4.2/apysc/_material_design/icon/material_view_sidebar_icon.py` & `apysc-4.4.3/apysc/_material_design/icon/material_view_sidebar_icon.py`

 * *Files identical despite different names*

### Comparing `apysc-4.4.2/apysc/_material_design/icon/material_view_sidebar_outlined_icon.py` & `apysc-4.4.3/apysc/_material_design/icon/material_view_sidebar_outlined_icon.py`

 * *Files identical despite different names*

### Comparing `apysc-4.4.2/apysc/_material_design/icon/material_view_stream_icon.py` & `apysc-4.4.3/apysc/_material_design/icon/material_view_stream_icon.py`

 * *Files identical despite different names*

### Comparing `apysc-4.4.2/apysc/_material_design/icon/material_view_stream_outlined_icon.py` & `apysc-4.4.3/apysc/_material_design/icon/material_view_stream_outlined_icon.py`

 * *Files identical despite different names*

### Comparing `apysc-4.4.2/apysc/_material_design/icon/material_view_week_icon.py` & `apysc-4.4.3/apysc/_material_design/icon/material_view_week_icon.py`

 * *Files identical despite different names*

### Comparing `apysc-4.4.2/apysc/_material_design/icon/material_view_week_outlined_icon.py` & `apysc-4.4.3/apysc/_material_design/icon/material_view_week_outlined_icon.py`

 * *Files identical despite different names*

### Comparing `apysc-4.4.2/apysc/_material_design/icon/material_visibility_icon.py` & `apysc-4.4.3/apysc/_material_design/icon/material_visibility_icon.py`

 * *Files identical despite different names*

### Comparing `apysc-4.4.2/apysc/_material_design/icon/material_visibility_off_icon.py` & `apysc-4.4.3/apysc/_material_design/icon/material_visibility_off_icon.py`

 * *Files identical despite different names*

### Comparing `apysc-4.4.2/apysc/_material_design/icon/material_visibility_off_outlined_icon.py` & `apysc-4.4.3/apysc/_material_design/icon/material_visibility_off_outlined_icon.py`

 * *Files identical despite different names*

### Comparing `apysc-4.4.2/apysc/_material_design/icon/material_visibility_outlined_icon.py` & `apysc-4.4.3/apysc/_material_design/icon/material_visibility_outlined_icon.py`

 * *Files identical despite different names*

### Comparing `apysc-4.4.2/apysc/_material_design/icon/material_voice_over_off_icon.py` & `apysc-4.4.3/apysc/_material_design/icon/material_voice_over_off_icon.py`

 * *Files identical despite different names*

### Comparing `apysc-4.4.2/apysc/_material_design/icon/material_voice_over_off_outlined_icon.py` & `apysc-4.4.3/apysc/_material_design/icon/material_voice_over_off_outlined_icon.py`

 * *Files identical despite different names*

### Comparing `apysc-4.4.2/apysc/_material_design/icon/material_voicemail_icon.py` & `apysc-4.4.3/apysc/_material_design/icon/material_voicemail_icon.py`

 * *Files identical despite different names*

### Comparing `apysc-4.4.2/apysc/_material_design/icon/material_voicemail_outlined_icon.py` & `apysc-4.4.3/apysc/_material_design/icon/material_voicemail_outlined_icon.py`

 * *Files identical despite different names*

### Comparing `apysc-4.4.2/apysc/_material_design/icon/material_volume_down_icon.py` & `apysc-4.4.3/apysc/_material_design/icon/material_volume_down_icon.py`

 * *Files identical despite different names*

### Comparing `apysc-4.4.2/apysc/_material_design/icon/material_volume_down_outlined_icon.py` & `apysc-4.4.3/apysc/_material_design/icon/material_volume_down_outlined_icon.py`

 * *Files identical despite different names*

### Comparing `apysc-4.4.2/apysc/_material_design/icon/material_volume_mute_icon.py` & `apysc-4.4.3/apysc/_material_design/icon/material_volume_mute_icon.py`

 * *Files identical despite different names*

### Comparing `apysc-4.4.2/apysc/_material_design/icon/material_volume_mute_outlined_icon.py` & `apysc-4.4.3/apysc/_material_design/icon/material_volume_mute_outlined_icon.py`

 * *Files identical despite different names*

### Comparing `apysc-4.4.2/apysc/_material_design/icon/material_volume_off_icon.py` & `apysc-4.4.3/apysc/_material_design/icon/material_volume_off_icon.py`

 * *Files identical despite different names*

### Comparing `apysc-4.4.2/apysc/_material_design/icon/material_volume_off_outlined_icon.py` & `apysc-4.4.3/apysc/_material_design/icon/material_volume_off_outlined_icon.py`

 * *Files identical despite different names*

### Comparing `apysc-4.4.2/apysc/_material_design/icon/material_volume_up_icon.py` & `apysc-4.4.3/apysc/_material_design/icon/material_volume_up_icon.py`

 * *Files identical despite different names*

### Comparing `apysc-4.4.2/apysc/_material_design/icon/material_volume_up_outlined_icon.py` & `apysc-4.4.3/apysc/_material_design/icon/material_volume_up_outlined_icon.py`

 * *Files identical despite different names*

### Comparing `apysc-4.4.2/apysc/_material_design/icon/material_vpn_key_icon.py` & `apysc-4.4.3/apysc/_material_design/icon/material_vpn_key_icon.py`

 * *Files identical despite different names*

### Comparing `apysc-4.4.2/apysc/_material_design/icon/material_vpn_key_outlined_icon.py` & `apysc-4.4.3/apysc/_material_design/icon/material_vpn_key_outlined_icon.py`

 * *Files identical despite different names*

### Comparing `apysc-4.4.2/apysc/_material_design/icon/material_warning_amber_outlined_icon.py` & `apysc-4.4.3/apysc/_material_design/icon/material_warning_amber_outlined_icon.py`

 * *Files identical despite different names*

### Comparing `apysc-4.4.2/apysc/_material_design/icon/material_warning_icon.py` & `apysc-4.4.3/apysc/_material_design/icon/material_warning_icon.py`

 * *Files identical despite different names*

### Comparing `apysc-4.4.2/apysc/_material_design/icon/material_warning_outlined_icon.py` & `apysc-4.4.3/apysc/_material_design/icon/material_warning_outlined_icon.py`

 * *Files identical despite different names*

### Comparing `apysc-4.4.2/apysc/_material_design/icon/material_watch_later_icon.py` & `apysc-4.4.3/apysc/_material_design/icon/material_watch_later_icon.py`

 * *Files identical despite different names*

### Comparing `apysc-4.4.2/apysc/_material_design/icon/material_watch_later_outlined_icon.py` & `apysc-4.4.3/apysc/_material_design/icon/material_watch_later_outlined_icon.py`

 * *Files identical despite different names*

### Comparing `apysc-4.4.2/apysc/_material_design/icon/material_web_asset_icon.py` & `apysc-4.4.3/apysc/_material_design/icon/material_web_asset_icon.py`

 * *Files identical despite different names*

### Comparing `apysc-4.4.2/apysc/_material_design/icon/material_web_asset_outlined_icon.py` & `apysc-4.4.3/apysc/_material_design/icon/material_web_asset_outlined_icon.py`

 * *Files identical despite different names*

### Comparing `apysc-4.4.2/apysc/_material_design/icon/material_web_icon.py` & `apysc-4.4.3/apysc/_material_design/icon/material_web_icon.py`

 * *Files identical despite different names*

### Comparing `apysc-4.4.2/apysc/_material_design/icon/material_web_outlined_icon.py` & `apysc-4.4.3/apysc/_material_design/icon/material_web_outlined_icon.py`

 * *Files identical despite different names*

### Comparing `apysc-4.4.2/apysc/_material_design/icon/material_wifi_calling_icon.py` & `apysc-4.4.3/apysc/_material_design/icon/material_wifi_calling_icon.py`

 * *Files identical despite different names*

### Comparing `apysc-4.4.2/apysc/_material_design/icon/material_wifi_calling_outlined_icon.py` & `apysc-4.4.3/apysc/_material_design/icon/material_wifi_calling_outlined_icon.py`

 * *Files identical despite different names*

### Comparing `apysc-4.4.2/apysc/_material_design/icon/material_wifi_protected_setup_icon.py` & `apysc-4.4.3/apysc/_material_design/icon/material_wifi_protected_setup_icon.py`

 * *Files identical despite different names*

### Comparing `apysc-4.4.2/apysc/_material_design/icon/material_wifi_protected_setup_outlined_icon.py` & `apysc-4.4.3/apysc/_material_design/icon/material_wifi_protected_setup_outlined_icon.py`

 * *Files identical despite different names*

### Comparing `apysc-4.4.2/apysc/_material_design/icon/material_work_icon.py` & `apysc-4.4.3/apysc/_material_design/icon/material_work_icon.py`

 * *Files identical despite different names*

### Comparing `apysc-4.4.2/apysc/_material_design/icon/material_work_off_icon.py` & `apysc-4.4.3/apysc/_material_design/icon/material_work_off_icon.py`

 * *Files identical despite different names*

### Comparing `apysc-4.4.2/apysc/_material_design/icon/material_work_off_outlined_icon.py` & `apysc-4.4.3/apysc/_material_design/icon/material_work_off_outlined_icon.py`

 * *Files identical despite different names*

### Comparing `apysc-4.4.2/apysc/_material_design/icon/material_work_outline_icon.py` & `apysc-4.4.3/apysc/_material_design/icon/material_work_outline_icon.py`

 * *Files identical despite different names*

### Comparing `apysc-4.4.2/apysc/_material_design/icon/material_work_outline_outlined_icon.py` & `apysc-4.4.3/apysc/_material_design/icon/material_work_outline_outlined_icon.py`

 * *Files identical despite different names*

### Comparing `apysc-4.4.2/apysc/_material_design/icon/material_work_outlined_icon.py` & `apysc-4.4.3/apysc/_material_design/icon/material_work_outlined_icon.py`

 * *Files identical despite different names*

### Comparing `apysc-4.4.2/apysc/_material_design/icon/material_wysiwyg_icon.py` & `apysc-4.4.3/apysc/_material_design/icon/material_wysiwyg_icon.py`

 * *Files identical despite different names*

### Comparing `apysc-4.4.2/apysc/_material_design/icon/material_wysiwyg_outlined_icon.py` & `apysc-4.4.3/apysc/_material_design/icon/material_wysiwyg_outlined_icon.py`

 * *Files identical despite different names*

### Comparing `apysc-4.4.2/apysc/_material_design/icon/material_youtube_searched_for_icon.py` & `apysc-4.4.3/apysc/_material_design/icon/material_youtube_searched_for_icon.py`

 * *Files identical despite different names*

### Comparing `apysc-4.4.2/apysc/_material_design/icon/material_youtube_searched_for_outlined_icon.py` & `apysc-4.4.3/apysc/_material_design/icon/material_youtube_searched_for_outlined_icon.py`

 * *Files identical despite different names*

### Comparing `apysc-4.4.2/apysc/_material_design/icon/material_zoom_in_icon.py` & `apysc-4.4.3/apysc/_material_design/icon/material_zoom_in_icon.py`

 * *Files identical despite different names*

### Comparing `apysc-4.4.2/apysc/_material_design/icon/material_zoom_in_outlined_icon.py` & `apysc-4.4.3/apysc/_material_design/icon/material_zoom_in_outlined_icon.py`

 * *Files identical despite different names*

### Comparing `apysc-4.4.2/apysc/_material_design/icon/material_zoom_out_icon.py` & `apysc-4.4.3/apysc/_material_design/icon/material_zoom_out_icon.py`

 * *Files identical despite different names*

### Comparing `apysc-4.4.2/apysc/_material_design/icon/material_zoom_out_outlined_icon.py` & `apysc-4.4.3/apysc/_material_design/icon/material_zoom_out_outlined_icon.py`

 * *Files identical despite different names*

### Comparing `apysc-4.4.2/apysc/_math/max_mixin.py` & `apysc-4.4.3/apysc/_math/max_mixin.py`

 * *Files identical despite different names*

### Comparing `apysc-4.4.2/apysc/_math/min_mixin.py` & `apysc-4.4.3/apysc/_math/min_mixin.py`

 * *Files identical despite different names*

### Comparing `apysc-4.4.2/apysc/_math/trunc_mixin.py` & `apysc-4.4.3/apysc/_math/trunc_mixin.py`

 * *Files identical despite different names*

### Comparing `apysc-4.4.2/apysc/_string/indent_util.py` & `apysc-4.4.3/apysc/_string/indent_util.py`

 * *Files identical despite different names*

### Comparing `apysc-4.4.2/apysc/_string/string_util.py` & `apysc-4.4.3/apysc/_string/string_util.py`

 * *Files identical despite different names*

### Comparing `apysc-4.4.2/apysc/_testing/e2e_testing_helper.py` & `apysc-4.4.3/apysc/_testing/e2e_testing_helper.py`

 * *Files identical despite different names*

### Comparing `apysc-4.4.2/apysc/_testing/testing_helper.py` & `apysc-4.4.3/apysc/_testing/testing_helper.py`

 * *Files identical despite different names*

### Comparing `apysc-4.4.2/apysc/_time/datetime_.py` & `apysc-4.4.3/apysc/_time/datetime_.py`

 * *Files identical despite different names*

### Comparing `apysc-4.4.2/apysc/_time/day_mixin.py` & `apysc-4.4.3/apysc/_time/day_mixin.py`

 * *Files identical despite different names*

### Comparing `apysc-4.4.2/apysc/_time/days_mixin.py` & `apysc-4.4.3/apysc/_time/days_mixin.py`

 * *Files identical despite different names*

### Comparing `apysc-4.4.2/apysc/_time/fps.py` & `apysc-4.4.3/apysc/_time/fps.py`

 * *Files identical despite different names*

### Comparing `apysc-4.4.2/apysc/_time/hour_mixin.py` & `apysc-4.4.3/apysc/_time/hour_mixin.py`

 * *Files identical despite different names*

### Comparing `apysc-4.4.2/apysc/_time/left_and_right_datetimes_mixin.py` & `apysc-4.4.3/apysc/_time/left_and_right_datetimes_mixin.py`

 * *Files identical despite different names*

### Comparing `apysc-4.4.2/apysc/_time/millisecond_mixin.py` & `apysc-4.4.3/apysc/_time/millisecond_mixin.py`

 * *Files identical despite different names*

### Comparing `apysc-4.4.2/apysc/_time/minute_mixin.py` & `apysc-4.4.3/apysc/_time/minute_mixin.py`

 * *Files identical despite different names*

### Comparing `apysc-4.4.2/apysc/_time/month_end_mixin.py` & `apysc-4.4.3/apysc/_time/month_end_mixin.py`

 * *Files identical despite different names*

### Comparing `apysc-4.4.2/apysc/_time/month_mixin.py` & `apysc-4.4.3/apysc/_time/month_mixin.py`

 * *Files identical despite different names*

### Comparing `apysc-4.4.2/apysc/_time/now_mixin.py` & `apysc-4.4.3/apysc/_time/now_mixin.py`

 * *Files identical despite different names*

### Comparing `apysc-4.4.2/apysc/_time/second_mixin.py` & `apysc-4.4.3/apysc/_time/second_mixin.py`

 * *Files identical despite different names*

### Comparing `apysc-4.4.2/apysc/_time/timedelta_.py` & `apysc-4.4.3/apysc/_time/timedelta_.py`

 * *Files identical despite different names*

### Comparing `apysc-4.4.2/apysc/_time/timer.py` & `apysc-4.4.3/apysc/_time/timer.py`

 * *Files identical despite different names*

### Comparing `apysc-4.4.2/apysc/_time/total_seconds_mixin.py` & `apysc-4.4.3/apysc/_time/total_seconds_mixin.py`

 * *Files identical despite different names*

### Comparing `apysc-4.4.2/apysc/_time/weekday_mixin.py` & `apysc-4.4.3/apysc/_time/weekday_mixin.py`

 * *Files identical despite different names*

### Comparing `apysc-4.4.2/apysc/_time/year_mixin.py` & `apysc-4.4.3/apysc/_time/year_mixin.py`

 * *Files identical despite different names*

### Comparing `apysc-4.4.2/apysc/_translation/jp/about_handler_options_type.py` & `apysc-4.4.3/apysc/_translation/jp/about_handler_options_type.py`

 * *Files identical despite different names*

### Comparing `apysc-4.4.2/apysc/_translation/jp/add_child_and_remove_child.py` & `apysc-4.4.3/apysc/_translation/jp/add_child_and_remove_child.py`

 * *Files identical despite different names*

### Comparing `apysc-4.4.2/apysc/_translation/jp/add_debug_info_setting.py` & `apysc-4.4.3/apysc/_translation/jp/add_debug_info_setting.py`

 * *Files identical despite different names*

### Comparing `apysc-4.4.2/apysc/_translation/jp/animation_base_start.py` & `apysc-4.4.3/apysc/_translation/jp/animation_base_start.py`

 * *Files identical despite different names*

### Comparing `apysc-4.4.2/apysc/_translation/jp/animation_base_target.py` & `apysc-4.4.3/apysc/_translation/jp/animation_base_target.py`

 * *Files identical despite different names*

### Comparing `apysc-4.4.2/apysc/_translation/jp/animation_complete.py` & `apysc-4.4.3/apysc/_translation/jp/animation_complete.py`

 * *Files identical despite different names*

### Comparing `apysc-4.4.2/apysc/_translation/jp/animation_delay.py` & `apysc-4.4.3/apysc/_translation/jp/animation_delay.py`

 * *Files identical despite different names*

### Comparing `apysc-4.4.2/apysc/_translation/jp/animation_duration.py` & `apysc-4.4.3/apysc/_translation/jp/animation_duration.py`

 * *Files identical despite different names*

### Comparing `apysc-4.4.2/apysc/_translation/jp/animation_event.py` & `apysc-4.4.3/apysc/_translation/jp/animation_event.py`

 * *Files identical despite different names*

### Comparing `apysc-4.4.2/apysc/_translation/jp/animation_fill_alpha.py` & `apysc-4.4.3/apysc/_translation/jp/animation_fill_alpha.py`

 * *Files identical despite different names*

### Comparing `apysc-4.4.2/apysc/_translation/jp/animation_fill_color.py` & `apysc-4.4.3/apysc/_translation/jp/animation_fill_color.py`

 * *Files identical despite different names*

### Comparing `apysc-4.4.2/apysc/_translation/jp/animation_finish.py` & `apysc-4.4.3/apysc/_translation/jp/animation_finish.py`

 * *Files identical despite different names*

### Comparing `apysc-4.4.2/apysc/_translation/jp/animation_interfaces_abstract.py` & `apysc-4.4.3/apysc/_translation/jp/animation_interfaces_abstract.py`

 * *Files identical despite different names*

### Comparing `apysc-4.4.2/apysc/_translation/jp/animation_line_alpha.py` & `apysc-4.4.3/apysc/_translation/jp/animation_line_alpha.py`

 * *Files identical despite different names*

### Comparing `apysc-4.4.2/apysc/_translation/jp/animation_line_color.py` & `apysc-4.4.3/apysc/_translation/jp/animation_line_color.py`

 * *Files identical despite different names*

### Comparing `apysc-4.4.2/apysc/_translation/jp/animation_line_thickness.py` & `apysc-4.4.3/apysc/_translation/jp/animation_line_thickness.py`

 * *Files identical despite different names*

### Comparing `apysc-4.4.2/apysc/_translation/jp/animation_method_chaining.py` & `apysc-4.4.3/apysc/_translation/jp/animation_method_chaining.py`

 * *Files identical despite different names*

### Comparing `apysc-4.4.2/apysc/_translation/jp/animation_move.py` & `apysc-4.4.3/apysc/_translation/jp/animation_move.py`

 * *Files identical despite different names*

### Comparing `apysc-4.4.2/apysc/_translation/jp/animation_parallel.py` & `apysc-4.4.3/apysc/_translation/jp/animation_parallel.py`

 * *Files identical despite different names*

### Comparing `apysc-4.4.2/apysc/_translation/jp/animation_pause_and_play.py` & `apysc-4.4.3/apysc/_translation/jp/animation_pause_and_play.py`

 * *Files identical despite different names*

### Comparing `apysc-4.4.2/apysc/_translation/jp/animation_radius.py` & `apysc-4.4.3/apysc/_translation/jp/animation_radius.py`

 * *Files identical despite different names*

### Comparing `apysc-4.4.2/apysc/_translation/jp/animation_reset.py` & `apysc-4.4.3/apysc/_translation/jp/animation_reset.py`

 * *Files identical despite different names*

### Comparing `apysc-4.4.2/apysc/_translation/jp/animation_return_value.py` & `apysc-4.4.3/apysc/_translation/jp/animation_return_value.py`

 * *Files identical despite different names*

### Comparing `apysc-4.4.2/apysc/_translation/jp/animation_reverse.py` & `apysc-4.4.3/apysc/_translation/jp/animation_reverse.py`

 * *Files identical despite different names*

### Comparing `apysc-4.4.2/apysc/_translation/jp/animation_rotation_around_center.py` & `apysc-4.4.3/apysc/_translation/jp/animation_rotation_around_center.py`

 * *Files identical despite different names*

### Comparing `apysc-4.4.2/apysc/_translation/jp/animation_rotation_around_point.py` & `apysc-4.4.3/apysc/_translation/jp/animation_rotation_around_point.py`

 * *Files identical despite different names*

### Comparing `apysc-4.4.2/apysc/_translation/jp/animation_scale_x_and_y_from_center.py` & `apysc-4.4.3/apysc/_translation/jp/animation_scale_x_and_y_from_center.py`

 * *Files identical despite different names*

### Comparing `apysc-4.4.2/apysc/_translation/jp/animation_scale_x_and_y_from_point.py` & `apysc-4.4.3/apysc/_translation/jp/animation_scale_x_and_y_from_point.py`

 * *Files identical despite different names*

### Comparing `apysc-4.4.2/apysc/_translation/jp/animation_time.py` & `apysc-4.4.3/apysc/_translation/jp/animation_time.py`

 * *Files identical despite different names*

### Comparing `apysc-4.4.2/apysc/_translation/jp/animation_width_and_height.py` & `apysc-4.4.3/apysc/_translation/jp/animation_width_and_height.py`

 * *Files identical despite different names*

### Comparing `apysc-4.4.2/apysc/_translation/jp/animation_x.py` & `apysc-4.4.3/apysc/_translation/jp/animation_x.py`

 * *Files identical despite different names*

### Comparing `apysc-4.4.2/apysc/_translation/jp/animation_y.py` & `apysc-4.4.3/apysc/_translation/jp/animation_y.py`

 * *Files identical despite different names*

### Comparing `apysc-4.4.2/apysc/_translation/jp/append_js_expression.py` & `apysc-4.4.3/apysc/_translation/jp/append_js_expression.py`

 * *Files identical despite different names*

### Comparing `apysc-4.4.2/apysc/_translation/jp/array.py` & `apysc-4.4.3/apysc/_translation/jp/array.py`

 * *Files identical despite different names*

### Comparing `apysc-4.4.2/apysc/_translation/jp/array_append_and_push.py` & `apysc-4.4.3/apysc/_translation/jp/array_append_and_push.py`

 * *Files identical despite different names*

### Comparing `apysc-4.4.2/apysc/_translation/jp/array_clear.py` & `apysc-4.4.3/apysc/_translation/jp/array_clear.py`

 * *Files identical despite different names*

### Comparing `apysc-4.4.2/apysc/_translation/jp/array_comparison.py` & `apysc-4.4.3/apysc/_translation/jp/array_comparison.py`

 * *Files identical despite different names*

### Comparing `apysc-4.4.2/apysc/_translation/jp/array_extend_and_concat.py` & `apysc-4.4.3/apysc/_translation/jp/array_extend_and_concat.py`

 * *Files identical despite different names*

### Comparing `apysc-4.4.2/apysc/_translation/jp/array_index_of.py` & `apysc-4.4.3/apysc/_translation/jp/array_index_of.py`

 * *Files identical despite different names*

### Comparing `apysc-4.4.2/apysc/_translation/jp/array_insert_and_insert_at.py` & `apysc-4.4.3/apysc/_translation/jp/array_insert_and_insert_at.py`

 * *Files identical despite different names*

### Comparing `apysc-4.4.2/apysc/_translation/jp/array_join.py` & `apysc-4.4.3/apysc/_translation/jp/array_join.py`

 * *Files identical despite different names*

### Comparing `apysc-4.4.2/apysc/_translation/jp/array_last_value.py` & `apysc-4.4.3/apysc/_translation/jp/array_last_value.py`

 * *Files identical despite different names*

### Comparing `apysc-4.4.2/apysc/_translation/jp/array_length.py` & `apysc-4.4.3/apysc/_translation/jp/array_length.py`

 * *Files identical despite different names*

### Comparing `apysc-4.4.2/apysc/_translation/jp/array_pop.py` & `apysc-4.4.3/apysc/_translation/jp/array_pop.py`

 * *Files identical despite different names*

### Comparing `apysc-4.4.2/apysc/_translation/jp/array_remove_and_remove_at.py` & `apysc-4.4.3/apysc/_translation/jp/array_remove_and_remove_at.py`

 * *Files identical despite different names*

### Comparing `apysc-4.4.2/apysc/_translation/jp/array_reverse.py` & `apysc-4.4.3/apysc/_translation/jp/array_reverse.py`

 * *Files identical despite different names*

### Comparing `apysc-4.4.2/apysc/_translation/jp/array_slice.py` & `apysc-4.4.3/apysc/_translation/jp/array_slice.py`

 * *Files identical despite different names*

### Comparing `apysc-4.4.2/apysc/_translation/jp/array_sort.py` & `apysc-4.4.3/apysc/_translation/jp/array_sort.py`

 * *Files identical despite different names*

### Comparing `apysc-4.4.2/apysc/_translation/jp/assert_arrays_equal_and_arrays_not_equal.py` & `apysc-4.4.3/apysc/_translation/jp/assert_arrays_equal_and_arrays_not_equal.py`

 * *Files identical despite different names*

### Comparing `apysc-4.4.2/apysc/_translation/jp/assert_defined_and_undefined.py` & `apysc-4.4.3/apysc/_translation/jp/assert_defined_and_undefined.py`

 * *Files identical despite different names*

### Comparing `apysc-4.4.2/apysc/_translation/jp/assert_dicts_equal_and_dicts_not_equal.py` & `apysc-4.4.3/apysc/_translation/jp/assert_dicts_equal_and_dicts_not_equal.py`

 * *Files identical despite different names*

### Comparing `apysc-4.4.2/apysc/_translation/jp/assert_equal_and_not_equal.py` & `apysc-4.4.3/apysc/_translation/jp/assert_equal_and_not_equal.py`

 * *Files identical despite different names*

### Comparing `apysc-4.4.2/apysc/_translation/jp/assert_greater_and_greater_equal.py` & `apysc-4.4.3/apysc/_translation/jp/assert_greater_and_greater_equal.py`

 * *Files identical despite different names*

### Comparing `apysc-4.4.2/apysc/_translation/jp/assert_less_and_less_equal.py` & `apysc-4.4.3/apysc/_translation/jp/assert_less_and_less_equal.py`

 * *Files identical despite different names*

### Comparing `apysc-4.4.2/apysc/_translation/jp/assert_true_and_false.py` & `apysc-4.4.3/apysc/_translation/jp/assert_true_and_false.py`

 * *Files identical despite different names*

### Comparing `apysc-4.4.2/apysc/_translation/jp/assertion_basic_behavior.py` & `apysc-4.4.3/apysc/_translation/jp/assertion_basic_behavior.py`

 * *Files identical despite different names*

### Comparing `apysc-4.4.2/apysc/_translation/jp/bind_and_trigger_custom_event.py` & `apysc-4.4.3/apysc/_translation/jp/bind_and_trigger_custom_event.py`

 * *Files identical despite different names*

### Comparing `apysc-4.4.2/apysc/_translation/jp/blue_color.py` & `apysc-4.4.3/apysc/_translation/jp/blue_color.py`

 * *Files identical despite different names*

### Comparing `apysc-4.4.2/apysc/_translation/jp/boolean.py` & `apysc-4.4.3/apysc/_translation/jp/boolean.py`

 * *Files identical despite different names*

### Comparing `apysc-4.4.2/apysc/_translation/jp/branch_instruction_variables_reverting_setting.py` & `apysc-4.4.3/apysc/_translation/jp/branch_instruction_variables_reverting_setting.py`

 * *Files identical despite different names*

### Comparing `apysc-4.4.2/apysc/_translation/jp/circle.py` & `apysc-4.4.3/apysc/_translation/jp/circle.py`

 * *Files identical despite different names*

### Comparing `apysc-4.4.2/apysc/_translation/jp/click.py` & `apysc-4.4.3/apysc/_translation/jp/click.py`

 * *Files identical despite different names*

### Comparing `apysc-4.4.2/apysc/_translation/jp/color.py` & `apysc-4.4.3/apysc/_translation/jp/color.py`

 * *Files identical despite different names*

### Comparing `apysc-4.4.2/apysc/_translation/jp/color_from_rgb.py` & `apysc-4.4.3/apysc/_translation/jp/color_from_rgb.py`

 * *Files identical despite different names*

### Comparing `apysc-4.4.2/apysc/_translation/jp/colorless.py` & `apysc-4.4.3/apysc/_translation/jp/colorless.py`

 * *Files identical despite different names*

### Comparing `apysc-4.4.2/apysc/_translation/jp/colors.py` & `apysc-4.4.3/apysc/_translation/jp/colors.py`

 * *Files identical despite different names*

### Comparing `apysc-4.4.2/apysc/_translation/jp/contains.py` & `apysc-4.4.3/apysc/_translation/jp/contains.py`

 * *Files identical despite different names*

### Comparing `apysc-4.4.2/apysc/_translation/jp/continue.py` & `apysc-4.4.3/apysc/_translation/jp/continue.py`

 * *Files identical despite different names*

### Comparing `apysc-4.4.2/apysc/_translation/jp/datetime.py` & `apysc-4.4.3/apysc/_translation/jp/datetime.py`

 * *Files identical despite different names*

### Comparing `apysc-4.4.2/apysc/_translation/jp/datetime_day.py` & `apysc-4.4.3/apysc/_translation/jp/datetime_day.py`

 * *Files identical despite different names*

### Comparing `apysc-4.4.2/apysc/_translation/jp/datetime_hour.py` & `apysc-4.4.3/apysc/_translation/jp/datetime_hour.py`

 * *Files identical despite different names*

### Comparing `apysc-4.4.2/apysc/_translation/jp/datetime_millisecond.py` & `apysc-4.4.3/apysc/_translation/jp/datetime_millisecond.py`

 * *Files identical despite different names*

### Comparing `apysc-4.4.2/apysc/_translation/jp/datetime_minute.py` & `apysc-4.4.3/apysc/_translation/jp/datetime_minute.py`

 * *Files identical despite different names*

### Comparing `apysc-4.4.2/apysc/_translation/jp/datetime_month.py` & `apysc-4.4.3/apysc/_translation/jp/datetime_month.py`

 * *Files identical despite different names*

### Comparing `apysc-4.4.2/apysc/_translation/jp/datetime_now.py` & `apysc-4.4.3/apysc/_translation/jp/datetime_now.py`

 * *Files identical despite different names*

### Comparing `apysc-4.4.2/apysc/_translation/jp/datetime_second.py` & `apysc-4.4.3/apysc/_translation/jp/datetime_second.py`

 * *Files identical despite different names*

### Comparing `apysc-4.4.2/apysc/_translation/jp/datetime_set_month_end.py` & `apysc-4.4.3/apysc/_translation/jp/datetime_set_month_end.py`

 * *Files identical despite different names*

### Comparing `apysc-4.4.2/apysc/_translation/jp/datetime_weekday_js_and_weekday_py.py` & `apysc-4.4.3/apysc/_translation/jp/datetime_weekday_js_and_weekday_py.py`

 * *Files identical despite different names*

### Comparing `apysc-4.4.2/apysc/_translation/jp/datetime_year.py` & `apysc-4.4.3/apysc/_translation/jp/datetime_year.py`

 * *Files identical despite different names*

### Comparing `apysc-4.4.2/apysc/_translation/jp/dblclick.py` & `apysc-4.4.3/apysc/_translation/jp/dblclick.py`

 * *Files identical despite different names*

### Comparing `apysc-4.4.2/apysc/_translation/jp/delete.py` & `apysc-4.4.3/apysc/_translation/jp/delete.py`

 * *Files identical despite different names*

### Comparing `apysc-4.4.2/apysc/_translation/jp/dictionary.py` & `apysc-4.4.3/apysc/_translation/jp/dictionary.py`

 * *Files identical despite different names*

### Comparing `apysc-4.4.2/apysc/_translation/jp/dictionary_generic.py` & `apysc-4.4.3/apysc/_translation/jp/dictionary_generic.py`

 * *Files identical despite different names*

### Comparing `apysc-4.4.2/apysc/_translation/jp/dictionary_get.py` & `apysc-4.4.3/apysc/_translation/jp/dictionary_get.py`

 * *Files identical despite different names*

### Comparing `apysc-4.4.2/apysc/_translation/jp/dictionary_length.py` & `apysc-4.4.3/apysc/_translation/jp/dictionary_length.py`

 * *Files identical despite different names*

### Comparing `apysc-4.4.2/apysc/_translation/jp/display_object.py` & `apysc-4.4.3/apysc/_translation/jp/display_object.py`

 * *Files identical despite different names*

### Comparing `apysc-4.4.2/apysc/_translation/jp/display_object_and_graphics_base_prop_abstract.py` & `apysc-4.4.3/apysc/_translation/jp/display_object_and_graphics_base_prop_abstract.py`

 * *Files identical despite different names*

### Comparing `apysc-4.4.2/apysc/_translation/jp/display_object_get_and_set_css.py` & `apysc-4.4.3/apysc/_translation/jp/display_object_get_and_set_css.py`

 * *Files identical despite different names*

### Comparing `apysc-4.4.2/apysc/_translation/jp/display_object_mouse_event.py` & `apysc-4.4.3/apysc/_translation/jp/display_object_mouse_event.py`

 * *Files identical despite different names*

### Comparing `apysc-4.4.2/apysc/_translation/jp/display_object_parent.py` & `apysc-4.4.3/apysc/_translation/jp/display_object_parent.py`

 * *Files identical despite different names*

### Comparing `apysc-4.4.2/apysc/_translation/jp/display_object_visible.py` & `apysc-4.4.3/apysc/_translation/jp/display_object_visible.py`

 * *Files identical despite different names*

### Comparing `apysc-4.4.2/apysc/_translation/jp/display_object_x_and_y.py` & `apysc-4.4.3/apysc/_translation/jp/display_object_x_and_y.py`

 * *Files identical despite different names*

### Comparing `apysc-4.4.2/apysc/_translation/jp/display_on_colaboratory.py` & `apysc-4.4.3/apysc/_translation/jp/display_on_colaboratory.py`

 * *Files identical despite different names*

### Comparing `apysc-4.4.2/apysc/_translation/jp/display_on_jupyter.py` & `apysc-4.4.3/apysc/_translation/jp/display_on_jupyter.py`

 * *Files identical despite different names*

### Comparing `apysc-4.4.2/apysc/_translation/jp/draw_interfaces_abstract.py` & `apysc-4.4.3/apysc/_translation/jp/draw_interfaces_abstract.py`

 * *Files identical despite different names*

### Comparing `apysc-4.4.2/apysc/_translation/jp/easing_enum.py` & `apysc-4.4.3/apysc/_translation/jp/easing_enum.py`

 * *Files identical despite different names*

### Comparing `apysc-4.4.2/apysc/_translation/jp/elif.py` & `apysc-4.4.3/apysc/_translation/jp/elif.py`

 * *Files identical despite different names*

### Comparing `apysc-4.4.2/apysc/_translation/jp/ellipse.py` & `apysc-4.4.3/apysc/_translation/jp/ellipse.py`

 * *Files identical despite different names*

### Comparing `apysc-4.4.2/apysc/_translation/jp/else.py` & `apysc-4.4.3/apysc/_translation/jp/else.py`

 * *Files identical despite different names*

### Comparing `apysc-4.4.2/apysc/_translation/jp/enter_frame.py` & `apysc-4.4.3/apysc/_translation/jp/enter_frame.py`

 * *Files identical despite different names*

### Comparing `apysc-4.4.2/apysc/_translation/jp/event_prevent_default_and_stop_propagation.py` & `apysc-4.4.3/apysc/_translation/jp/event_prevent_default_and_stop_propagation.py`

 * *Files identical despite different names*

### Comparing `apysc-4.4.2/apysc/_translation/jp/for_array_indices.py` & `apysc-4.4.3/apysc/_translation/jp/for_array_indices.py`

 * *Files identical despite different names*

### Comparing `apysc-4.4.2/apysc/_translation/jp/for_array_indices_and_values.py` & `apysc-4.4.3/apysc/_translation/jp/for_array_indices_and_values.py`

 * *Files identical despite different names*

### Comparing `apysc-4.4.2/apysc/_translation/jp/for_array_values.py` & `apysc-4.4.3/apysc/_translation/jp/for_array_values.py`

 * *Files identical despite different names*

### Comparing `apysc-4.4.2/apysc/_translation/jp/for_dict_keys.py` & `apysc-4.4.3/apysc/_translation/jp/for_dict_keys.py`

 * *Files identical despite different names*

### Comparing `apysc-4.4.2/apysc/_translation/jp/for_dict_keys_and_values.py` & `apysc-4.4.3/apysc/_translation/jp/for_dict_keys_and_values.py`

 * *Files identical despite different names*

### Comparing `apysc-4.4.2/apysc/_translation/jp/for_dict_values.py` & `apysc-4.4.3/apysc/_translation/jp/for_dict_values.py`

 * *Files identical despite different names*

### Comparing `apysc-4.4.2/apysc/_translation/jp/fps.py` & `apysc-4.4.3/apysc/_translation/jp/fps.py`

 * *Files identical despite different names*

### Comparing `apysc-4.4.2/apysc/_translation/jp/fundamental_data_classes_value_interface.py` & `apysc-4.4.3/apysc/_translation/jp/fundamental_data_classes_value_interface.py`

 * *Files identical despite different names*

### Comparing `apysc-4.4.2/apysc/_translation/jp/get_bounds.py` & `apysc-4.4.3/apysc/_translation/jp/get_bounds.py`

 * *Files identical despite different names*

### Comparing `apysc-4.4.2/apysc/_translation/jp/get_child_at.py` & `apysc-4.4.3/apysc/_translation/jp/get_child_at.py`

 * *Files identical despite different names*

### Comparing `apysc-4.4.2/apysc/_translation/jp/graphics.py` & `apysc-4.4.3/apysc/_translation/jp/graphics.py`

 * *Files identical despite different names*

### Comparing `apysc-4.4.2/apysc/_translation/jp/graphics_base_fill_alpha.py` & `apysc-4.4.3/apysc/_translation/jp/graphics_base_fill_alpha.py`

 * *Files identical despite different names*

### Comparing `apysc-4.4.2/apysc/_translation/jp/graphics_base_fill_color.py` & `apysc-4.4.3/apysc/_translation/jp/graphics_base_fill_color.py`

 * *Files identical despite different names*

### Comparing `apysc-4.4.2/apysc/_translation/jp/graphics_base_flip_interfaces.py` & `apysc-4.4.3/apysc/_translation/jp/graphics_base_flip_interfaces.py`

 * *Files identical despite different names*

### Comparing `apysc-4.4.2/apysc/_translation/jp/graphics_base_line_alpha.py` & `apysc-4.4.3/apysc/_translation/jp/graphics_base_line_alpha.py`

 * *Files identical despite different names*

### Comparing `apysc-4.4.2/apysc/_translation/jp/graphics_base_line_color.py` & `apysc-4.4.3/apysc/_translation/jp/graphics_base_line_color.py`

 * *Files identical despite different names*

### Comparing `apysc-4.4.2/apysc/_translation/jp/graphics_base_line_dash_dot_setting.py` & `apysc-4.4.3/apysc/_translation/jp/graphics_base_line_dash_dot_setting.py`

 * *Files identical despite different names*

### Comparing `apysc-4.4.2/apysc/_translation/jp/graphics_base_line_dash_setting.py` & `apysc-4.4.3/apysc/_translation/jp/graphics_base_line_dash_setting.py`

 * *Files identical despite different names*

### Comparing `apysc-4.4.2/apysc/_translation/jp/graphics_base_line_dot_setting.py` & `apysc-4.4.3/apysc/_translation/jp/graphics_base_line_dot_setting.py`

 * *Files identical despite different names*

### Comparing `apysc-4.4.2/apysc/_translation/jp/graphics_base_line_round_dot_setting.py` & `apysc-4.4.3/apysc/_translation/jp/graphics_base_line_round_dot_setting.py`

 * *Files identical despite different names*

### Comparing `apysc-4.4.2/apysc/_translation/jp/graphics_base_line_thickness.py` & `apysc-4.4.3/apysc/_translation/jp/graphics_base_line_thickness.py`

 * *Files identical despite different names*

### Comparing `apysc-4.4.2/apysc/_translation/jp/graphics_base_rotation_around_center.py` & `apysc-4.4.3/apysc/_translation/jp/graphics_base_rotation_around_center.py`

 * *Files identical despite different names*

### Comparing `apysc-4.4.2/apysc/_translation/jp/graphics_base_rotation_around_point.py` & `apysc-4.4.3/apysc/_translation/jp/graphics_base_rotation_around_point.py`

 * *Files identical despite different names*

### Comparing `apysc-4.4.2/apysc/_translation/jp/graphics_base_scale_from_center.py` & `apysc-4.4.3/apysc/_translation/jp/graphics_base_scale_from_center.py`

 * *Files identical despite different names*

### Comparing `apysc-4.4.2/apysc/_translation/jp/graphics_base_scale_from_point.py` & `apysc-4.4.3/apysc/_translation/jp/graphics_base_scale_from_point.py`

 * *Files identical despite different names*

### Comparing `apysc-4.4.2/apysc/_translation/jp/graphics_base_skew.py` & `apysc-4.4.3/apysc/_translation/jp/graphics_base_skew.py`

 * *Files identical despite different names*

### Comparing `apysc-4.4.2/apysc/_translation/jp/graphics_begin_fill.py` & `apysc-4.4.3/apysc/_translation/jp/graphics_begin_fill.py`

 * *Files identical despite different names*

### Comparing `apysc-4.4.2/apysc/_translation/jp/graphics_clear.py` & `apysc-4.4.3/apysc/_translation/jp/graphics_clear.py`

 * *Files identical despite different names*

### Comparing `apysc-4.4.2/apysc/_translation/jp/graphics_draw_circle.py` & `apysc-4.4.3/apysc/_translation/jp/graphics_draw_circle.py`

 * *Files identical despite different names*

### Comparing `apysc-4.4.2/apysc/_translation/jp/graphics_draw_dash_dotted_line.py` & `apysc-4.4.3/apysc/_translation/jp/graphics_draw_dash_dotted_line.py`

 * *Files identical despite different names*

### Comparing `apysc-4.4.2/apysc/_translation/jp/graphics_draw_dashed_line.py` & `apysc-4.4.3/apysc/_translation/jp/graphics_draw_dashed_line.py`

 * *Files identical despite different names*

### Comparing `apysc-4.4.2/apysc/_translation/jp/graphics_draw_dotted_line.py` & `apysc-4.4.3/apysc/_translation/jp/graphics_draw_dotted_line.py`

 * *Files identical despite different names*

### Comparing `apysc-4.4.2/apysc/_translation/jp/graphics_draw_ellipse.py` & `apysc-4.4.3/apysc/_translation/jp/graphics_draw_ellipse.py`

 * *Files identical despite different names*

### Comparing `apysc-4.4.2/apysc/_translation/jp/graphics_draw_line.py` & `apysc-4.4.3/apysc/_translation/jp/graphics_draw_line.py`

 * *Files identical despite different names*

### Comparing `apysc-4.4.2/apysc/_translation/jp/graphics_draw_path.py` & `apysc-4.4.3/apysc/_translation/jp/graphics_draw_path.py`

 * *Files identical despite different names*

### Comparing `apysc-4.4.2/apysc/_translation/jp/graphics_draw_polygon.py` & `apysc-4.4.3/apysc/_translation/jp/graphics_draw_polygon.py`

 * *Files identical despite different names*

### Comparing `apysc-4.4.2/apysc/_translation/jp/graphics_draw_rect.py` & `apysc-4.4.3/apysc/_translation/jp/graphics_draw_rect.py`

 * *Files identical despite different names*

### Comparing `apysc-4.4.2/apysc/_translation/jp/graphics_draw_round_dotted_line.py` & `apysc-4.4.3/apysc/_translation/jp/graphics_draw_round_dotted_line.py`

 * *Files identical despite different names*

### Comparing `apysc-4.4.2/apysc/_translation/jp/graphics_draw_round_rect.py` & `apysc-4.4.3/apysc/_translation/jp/graphics_draw_round_rect.py`

 * *Files identical despite different names*

### Comparing `apysc-4.4.2/apysc/_translation/jp/graphics_draw_triangle.py` & `apysc-4.4.3/apysc/_translation/jp/graphics_draw_triangle.py`

 * *Files identical despite different names*

### Comparing `apysc-4.4.2/apysc/_translation/jp/graphics_line_style.py` & `apysc-4.4.3/apysc/_translation/jp/graphics_line_style.py`

 * *Files identical despite different names*

### Comparing `apysc-4.4.2/apysc/_translation/jp/graphics_move_to_and_line_to.py` & `apysc-4.4.3/apysc/_translation/jp/graphics_move_to_and_line_to.py`

 * *Files identical despite different names*

### Comparing `apysc-4.4.2/apysc/_translation/jp/green_color.py` & `apysc-4.4.3/apysc/_translation/jp/green_color.py`

 * *Files identical despite different names*

### Comparing `apysc-4.4.2/apysc/_translation/jp/if.py` & `apysc-4.4.3/apysc/_translation/jp/if.py`

 * *Files identical despite different names*

### Comparing `apysc-4.4.2/apysc/_translation/jp/import_conventions.py` & `apysc-4.4.3/apysc/_translation/jp/import_conventions.py`

 * *Files identical despite different names*

### Comparing `apysc-4.4.2/apysc/_translation/jp/index.py` & `apysc-4.4.3/apysc/_translation/jp/index.py`

 * *Files 0% similar despite different names*

```diff
@@ -131,15 +131,15 @@
     ##################################################
     "## Animation": "## アニメーション",
     ##################################################
     "```{toctree}\n:maxdepth: 1\nanimation_interfaces_abstract\nanimation_event\nanimation_duration\nanimation_delay\nanimation_return_value\nanimation_base_start\nanimation_complete\nanimation_method_chaining\nanimation_base_target\nanimation_pause_and_play\nanimation_reset\nanimation_finish\nanimation_reverse\nanimation_time\neasing_enum\nsequential_animation\nanimation_parallel\nanimation_move\nanimation_x\nanimation_y\nanimation_width_and_height\nanimation_fill_color\nanimation_fill_alpha\nanimation_line_color\nanimation_line_alpha\nanimation_line_thickness\nanimation_radius\nanimation_rotation_around_center\nanimation_rotation_around_point\nanimation_scale_x_and_y_from_center\nanimation_scale_x_and_y_from_point\n```": "```{toctree}\n:maxdepth: 1\njp_animation_interfaces_abstract\njp_animation_event\njp_animation_duration\njp_animation_delay\njp_animation_return_value\njp_animation_base_start\njp_animation_complete\njp_animation_method_chaining\njp_animation_base_target\njp_animation_pause_and_play\njp_animation_reset\njp_animation_finish\njp_animation_reverse\njp_animation_time\njp_easing_enum\njp_sequential_animation\njp_animation_parallel\njp_animation_move\njp_animation_x\njp_animation_y\njp_animation_width_and_height\njp_animation_fill_color\njp_animation_fill_alpha\njp_animation_line_color\njp_animation_line_alpha\njp_animation_line_thickness\njp_animation_radius\njp_animation_rotation_around_center\njp_animation_rotation_around_point\njp_animation_scale_x_and_y_from_center\njp_animation_scale_x_and_y_from_point\n```",  # noqa
     ##################################################
     "## Mathematics": "## 数学",
     ##################################################
-    "```{toctree}\n:maxdepth: 1\nmath_min\nmath_max\nmath_trunc\n```": "```{toctree}\n:maxdepth: 1\njp_math_min\njp_math_max\njp_math_trunc\n```",  # noqa
+    "```{toctree}\n:maxdepth: 1\nmath_min\nmath_max\nmath_trunc\nmath_clamp\n```": "```{toctree}\n:maxdepth: 1\njp_math_min\njp_math_max\njp_math_trunc\njp_math_clamp\n```",  # noqa
     ##################################################
     "## Other manipulation interfaces": "## その他の操作関係の各インターフェイス",
     ##################################################
     "```{toctree}\n:maxdepth: 1\ndelete\n```": "```{toctree}\n:maxdepth: 1\njp_delete\n```",  # noqa
     ##################################################
     "## Debugging": "## デバッグ",
     ##################################################
```

### Comparing `apysc-4.4.2/apysc/_translation/jp/int_and_number.py` & `apysc-4.4.3/apysc/_translation/jp/int_and_number.py`

 * *Files identical despite different names*

### Comparing `apysc-4.4.2/apysc/_translation/jp/int_and_number_arithmetic_operations.py` & `apysc-4.4.3/apysc/_translation/jp/int_and_number_arithmetic_operations.py`

 * *Files identical despite different names*

### Comparing `apysc-4.4.2/apysc/_translation/jp/int_and_number_comparison_operations.py` & `apysc-4.4.3/apysc/_translation/jp/int_and_number_comparison_operations.py`

 * *Files identical despite different names*

### Comparing `apysc-4.4.2/apysc/_translation/jp/int_and_number_to_fixed.py` & `apysc-4.4.3/apysc/_translation/jp/int_and_number_to_fixed.py`

 * *Files identical despite different names*

### Comparing `apysc-4.4.2/apysc/_translation/jp/int_and_number_to_hex.py` & `apysc-4.4.3/apysc/_translation/jp/int_and_number_to_hex.py`

 * *Files identical despite different names*

### Comparing `apysc-4.4.2/apysc/_translation/jp/line.py` & `apysc-4.4.3/apysc/_translation/jp/line.py`

 * *Files identical despite different names*

### Comparing `apysc-4.4.2/apysc/_translation/jp/material_design_colors.py` & `apysc-4.4.3/apysc/_translation/jp/material_design_colors.py`

 * *Files identical despite different names*

### Comparing `apysc-4.4.2/apysc/_translation/jp/material_icon.py` & `apysc-4.4.3/apysc/_translation/jp/material_icon.py`

 * *Files identical despite different names*

### Comparing `apysc-4.4.2/apysc/_translation/jp/math_max.py` & `apysc-4.4.3/apysc/_translation/jp/math_max.py`

 * *Files identical despite different names*

### Comparing `apysc-4.4.2/apysc/_translation/jp/math_min.py` & `apysc-4.4.3/apysc/_translation/jp/math_min.py`

 * *Files identical despite different names*

### Comparing `apysc-4.4.2/apysc/_translation/jp/math_trunc.py` & `apysc-4.4.3/apysc/_translation/jp/math_trunc.py`

 * *Files identical despite different names*

### Comparing `apysc-4.4.2/apysc/_translation/jp/mouse_event_abstract.py` & `apysc-4.4.3/apysc/_translation/jp/mouse_event_abstract.py`

 * *Files identical despite different names*

### Comparing `apysc-4.4.2/apysc/_translation/jp/mouse_event_basic.py` & `apysc-4.4.3/apysc/_translation/jp/mouse_event_basic.py`

 * *Files identical despite different names*

### Comparing `apysc-4.4.2/apysc/_translation/jp/mousedown_and_mouseup.py` & `apysc-4.4.3/apysc/_translation/jp/mousedown_and_mouseup.py`

 * *Files identical despite different names*

### Comparing `apysc-4.4.2/apysc/_translation/jp/mousemove.py` & `apysc-4.4.3/apysc/_translation/jp/mousemove.py`

 * *Files identical despite different names*

### Comparing `apysc-4.4.2/apysc/_translation/jp/mouseover_and_mouseout.py` & `apysc-4.4.3/apysc/_translation/jp/mouseover_and_mouseout.py`

 * *Files identical despite different names*

### Comparing `apysc-4.4.2/apysc/_translation/jp/multi_line_text.py` & `apysc-4.4.3/apysc/_translation/jp/multi_line_text.py`

 * *Files identical despite different names*

### Comparing `apysc-4.4.2/apysc/_translation/jp/num_children.py` & `apysc-4.4.3/apysc/_translation/jp/num_children.py`

 * *Files identical despite different names*

### Comparing `apysc-4.4.2/apysc/_translation/jp/path.py` & `apysc-4.4.3/apysc/_translation/jp/path.py`

 * *Files identical despite different names*

### Comparing `apysc-4.4.2/apysc/_translation/jp/path_bezier_2d.py` & `apysc-4.4.3/apysc/_translation/jp/path_bezier_2d.py`

 * *Files identical despite different names*

### Comparing `apysc-4.4.2/apysc/_translation/jp/path_bezier_2d_continual.py` & `apysc-4.4.3/apysc/_translation/jp/path_bezier_2d_continual.py`

 * *Files identical despite different names*

### Comparing `apysc-4.4.2/apysc/_translation/jp/path_bezier_3d.py` & `apysc-4.4.3/apysc/_translation/jp/path_bezier_3d.py`

 * *Files identical despite different names*

### Comparing `apysc-4.4.2/apysc/_translation/jp/path_bezier_3d_continual.py` & `apysc-4.4.3/apysc/_translation/jp/path_bezier_3d_continual.py`

 * *Files identical despite different names*

### Comparing `apysc-4.4.2/apysc/_translation/jp/path_close.py` & `apysc-4.4.3/apysc/_translation/jp/path_close.py`

 * *Files identical despite different names*

### Comparing `apysc-4.4.2/apysc/_translation/jp/path_horizontal.py` & `apysc-4.4.3/apysc/_translation/jp/path_horizontal.py`

 * *Files identical despite different names*

### Comparing `apysc-4.4.2/apysc/_translation/jp/path_line_to.py` & `apysc-4.4.3/apysc/_translation/jp/path_line_to.py`

 * *Files identical despite different names*

### Comparing `apysc-4.4.2/apysc/_translation/jp/path_move_to.py` & `apysc-4.4.3/apysc/_translation/jp/path_move_to.py`

 * *Files identical despite different names*

### Comparing `apysc-4.4.2/apysc/_translation/jp/path_vertical.py` & `apysc-4.4.3/apysc/_translation/jp/path_vertical.py`

 * *Files identical despite different names*

### Comparing `apysc-4.4.2/apysc/_translation/jp/point2d.py` & `apysc-4.4.3/apysc/_translation/jp/point2d.py`

 * *Files identical despite different names*

### Comparing `apysc-4.4.2/apysc/_translation/jp/polygon.py` & `apysc-4.4.3/apysc/_translation/jp/polygon.py`

 * *Files identical despite different names*

### Comparing `apysc-4.4.2/apysc/_translation/jp/polyline.py` & `apysc-4.4.3/apysc/_translation/jp/polyline.py`

 * *Files identical despite different names*

### Comparing `apysc-4.4.2/apysc/_translation/jp/quick_start.py` & `apysc-4.4.3/apysc/_translation/jp/quick_start.py`

 * *Files identical despite different names*

### Comparing `apysc-4.4.2/apysc/_translation/jp/range.py` & `apysc-4.4.3/apysc/_translation/jp/range.py`

 * *Files identical despite different names*

### Comparing `apysc-4.4.2/apysc/_translation/jp/recommended_type_checker_settings.py` & `apysc-4.4.3/apysc/_translation/jp/recommended_type_checker_settings.py`

 * *Files identical despite different names*

### Comparing `apysc-4.4.2/apysc/_translation/jp/rectangle.py` & `apysc-4.4.3/apysc/_translation/jp/rectangle.py`

 * *Files identical despite different names*

### Comparing `apysc-4.4.2/apysc/_translation/jp/rectangle_geom.py` & `apysc-4.4.3/apysc/_translation/jp/rectangle_geom.py`

 * *Files identical despite different names*

### Comparing `apysc-4.4.2/apysc/_translation/jp/red_color.py` & `apysc-4.4.3/apysc/_translation/jp/red_color.py`

 * *Files identical despite different names*

### Comparing `apysc-4.4.2/apysc/_translation/jp/remove_children.py` & `apysc-4.4.3/apysc/_translation/jp/remove_children.py`

 * *Files identical despite different names*

### Comparing `apysc-4.4.2/apysc/_translation/jp/return.py` & `apysc-4.4.3/apysc/_translation/jp/return.py`

 * *Files identical despite different names*

### Comparing `apysc-4.4.2/apysc/_translation/jp/save_overall_html.py` & `apysc-4.4.3/apysc/_translation/jp/save_overall_html.py`

 * *Files identical despite different names*

### Comparing `apysc-4.4.2/apysc/_translation/jp/sequential_animation.py` & `apysc-4.4.3/apysc/_translation/jp/sequential_animation.py`

 * *Files identical despite different names*

### Comparing `apysc-4.4.2/apysc/_translation/jp/set_debug_mode.py` & `apysc-4.4.3/apysc/_translation/jp/set_debug_mode.py`

 * *Files identical despite different names*

### Comparing `apysc-4.4.2/apysc/_translation/jp/sprite.py` & `apysc-4.4.3/apysc/_translation/jp/sprite.py`

 * *Files identical despite different names*

### Comparing `apysc-4.4.2/apysc/_translation/jp/stage.py` & `apysc-4.4.3/apysc/_translation/jp/stage.py`

 * *Files identical despite different names*

### Comparing `apysc-4.4.2/apysc/_translation/jp/string.py` & `apysc-4.4.3/apysc/_translation/jp/string.py`

 * *Files identical despite different names*

### Comparing `apysc-4.4.2/apysc/_translation/jp/string_addition_and_multiplication.py` & `apysc-4.4.3/apysc/_translation/jp/string_addition_and_multiplication.py`

 * *Files identical despite different names*

### Comparing `apysc-4.4.2/apysc/_translation/jp/string_apply_max_num_of_decimal_places.py` & `apysc-4.4.3/apysc/_translation/jp/string_apply_max_num_of_decimal_places.py`

 * *Files identical despite different names*

### Comparing `apysc-4.4.2/apysc/_translation/jp/string_comparison_operations.py` & `apysc-4.4.3/apysc/_translation/jp/string_comparison_operations.py`

 * *Files identical despite different names*

### Comparing `apysc-4.4.2/apysc/_translation/jp/string_length.py` & `apysc-4.4.3/apysc/_translation/jp/string_length.py`

 * *Files identical despite different names*

### Comparing `apysc-4.4.2/apysc/_translation/jp/string_lower.py` & `apysc-4.4.3/apysc/_translation/jp/string_lower.py`

 * *Files identical despite different names*

### Comparing `apysc-4.4.2/apysc/_translation/jp/string_lstrip.py` & `apysc-4.4.3/apysc/_translation/jp/string_lstrip.py`

 * *Files identical despite different names*

### Comparing `apysc-4.4.2/apysc/_translation/jp/string_rstrip.py` & `apysc-4.4.3/apysc/_translation/jp/string_rstrip.py`

 * *Files identical despite different names*

### Comparing `apysc-4.4.2/apysc/_translation/jp/string_slice.py` & `apysc-4.4.3/apysc/_translation/jp/string_slice.py`

 * *Files identical despite different names*

### Comparing `apysc-4.4.2/apysc/_translation/jp/string_split.py` & `apysc-4.4.3/apysc/_translation/jp/string_split.py`

 * *Files identical despite different names*

### Comparing `apysc-4.4.2/apysc/_translation/jp/string_strip.py` & `apysc-4.4.3/apysc/_translation/jp/string_strip.py`

 * *Files identical despite different names*

### Comparing `apysc-4.4.2/apysc/_translation/jp/string_upper.py` & `apysc-4.4.3/apysc/_translation/jp/string_upper.py`

 * *Files identical despite different names*

### Comparing `apysc-4.4.2/apysc/_translation/jp/string_zfill.py` & `apysc-4.4.3/apysc/_translation/jp/string_zfill.py`

 * *Files identical despite different names*

### Comparing `apysc-4.4.2/apysc/_translation/jp/svg_text.py` & `apysc-4.4.3/apysc/_translation/jp/svg_text.py`

 * *Files identical despite different names*

### Comparing `apysc-4.4.2/apysc/_translation/jp/svg_text_span.py` & `apysc-4.4.3/apysc/_translation/jp/svg_text_span.py`

 * *Files identical despite different names*

### Comparing `apysc-4.4.2/apysc/_translation/jp/text_align.py` & `apysc-4.4.3/apysc/_translation/jp/text_align.py`

 * *Files identical despite different names*

### Comparing `apysc-4.4.2/apysc/_translation/jp/text_align_last.py` & `apysc-4.4.3/apysc/_translation/jp/text_align_last.py`

 * *Files identical despite different names*

### Comparing `apysc-4.4.2/apysc/_translation/jp/text_bold.py` & `apysc-4.4.3/apysc/_translation/jp/text_bold.py`

 * *Files identical despite different names*

### Comparing `apysc-4.4.2/apysc/_translation/jp/text_fill_alpha.py` & `apysc-4.4.3/apysc/_translation/jp/text_fill_alpha.py`

 * *Files identical despite different names*

### Comparing `apysc-4.4.2/apysc/_translation/jp/text_fill_color.py` & `apysc-4.4.3/apysc/_translation/jp/text_fill_color.py`

 * *Files identical despite different names*

### Comparing `apysc-4.4.2/apysc/_translation/jp/text_font_size.py` & `apysc-4.4.3/apysc/_translation/jp/text_font_size.py`

 * *Files identical despite different names*

### Comparing `apysc-4.4.2/apysc/_translation/jp/text_italic.py` & `apysc-4.4.3/apysc/_translation/jp/text_italic.py`

 * *Files identical despite different names*

### Comparing `apysc-4.4.2/apysc/_translation/jp/text_line_height.py` & `apysc-4.4.3/apysc/_translation/jp/text_line_height.py`

 * *Files identical despite different names*

### Comparing `apysc-4.4.2/apysc/_translation/jp/text_underline.py` & `apysc-4.4.3/apysc/_translation/jp/text_underline.py`

 * *Files identical despite different names*

### Comparing `apysc-4.4.2/apysc/_translation/jp/timedelta.py` & `apysc-4.4.3/apysc/_translation/jp/timedelta.py`

 * *Files identical despite different names*

### Comparing `apysc-4.4.2/apysc/_translation/jp/timedelta_days.py` & `apysc-4.4.3/apysc/_translation/jp/timedelta_days.py`

 * *Files identical despite different names*

### Comparing `apysc-4.4.2/apysc/_translation/jp/timedelta_total_seconds.py` & `apysc-4.4.3/apysc/_translation/jp/timedelta_total_seconds.py`

 * *Files identical despite different names*

### Comparing `apysc-4.4.2/apysc/_translation/jp/timer.py` & `apysc-4.4.3/apysc/_translation/jp/timer.py`

 * *Files identical despite different names*

### Comparing `apysc-4.4.2/apysc/_translation/jp/timer_complete.py` & `apysc-4.4.3/apysc/_translation/jp/timer_complete.py`

 * *Files identical despite different names*

### Comparing `apysc-4.4.2/apysc/_translation/jp/timer_delay.py` & `apysc-4.4.3/apysc/_translation/jp/timer_delay.py`

 * *Files identical despite different names*

### Comparing `apysc-4.4.2/apysc/_translation/jp/timer_event.py` & `apysc-4.4.3/apysc/_translation/jp/timer_event.py`

 * *Files identical despite different names*

### Comparing `apysc-4.4.2/apysc/_translation/jp/timer_repeat_count.py` & `apysc-4.4.3/apysc/_translation/jp/timer_repeat_count.py`

 * *Files identical despite different names*

### Comparing `apysc-4.4.2/apysc/_translation/jp/timer_reset.py` & `apysc-4.4.3/apysc/_translation/jp/timer_reset.py`

 * *Files identical despite different names*

### Comparing `apysc-4.4.2/apysc/_translation/jp/timer_start_and_stop.py` & `apysc-4.4.3/apysc/_translation/jp/timer_start_and_stop.py`

 * *Files identical despite different names*

### Comparing `apysc-4.4.2/apysc/_translation/jp/to_string.py` & `apysc-4.4.3/apysc/_translation/jp/to_string.py`

 * *Files identical despite different names*

### Comparing `apysc-4.4.2/apysc/_translation/jp/trace.py` & `apysc-4.4.3/apysc/_translation/jp/trace.py`

 * *Files identical despite different names*

### Comparing `apysc-4.4.2/apysc/_translation/jp/triangle.py` & `apysc-4.4.3/apysc/_translation/jp/triangle.py`

 * *Files identical despite different names*

### Comparing `apysc-4.4.2/apysc/_translation/jp/true_and_false.py` & `apysc-4.4.3/apysc/_translation/jp/true_and_false.py`

 * *Files identical despite different names*

### Comparing `apysc-4.4.2/apysc/_translation/jp/unbind_enter_frame_and_unbind_enter_frame_all.py` & `apysc-4.4.3/apysc/_translation/jp/unbind_enter_frame_and_unbind_enter_frame_all.py`

 * *Files identical despite different names*

### Comparing `apysc-4.4.2/apysc/_translation/jp/unset_debug_mode.py` & `apysc-4.4.3/apysc/_translation/jp/unset_debug_mode.py`

 * *Files identical despite different names*

### Comparing `apysc-4.4.2/apysc/_translation/jp/variable_name_suffix.py` & `apysc-4.4.3/apysc/_translation/jp/variable_name_suffix.py`

 * *Files identical despite different names*

### Comparing `apysc-4.4.2/apysc/_translation/jp/what_apysc_can_do.py` & `apysc-4.4.3/apysc/_translation/jp/what_apysc_can_do.py`

 * *Files identical despite different names*

### Comparing `apysc-4.4.2/apysc/_translation/jp/why_apysc_doesnt_use_python_builtin_data_type.py` & `apysc-4.4.3/apysc/_translation/jp/why_apysc_doesnt_use_python_builtin_data_type.py`

 * *Files identical despite different names*

### Comparing `apysc-4.4.2/apysc/_type/_delete.py` & `apysc-4.4.3/apysc/_type/_delete.py`

 * *Files identical despite different names*

### Comparing `apysc-4.4.2/apysc/_type/_return.py` & `apysc-4.4.3/apysc/_type/_return.py`

 * *Files identical despite different names*

### Comparing `apysc-4.4.2/apysc/_type/any_value.py` & `apysc-4.4.3/apysc/_type/any_value.py`

 * *Files identical despite different names*

### Comparing `apysc-4.4.2/apysc/_type/array.py` & `apysc-4.4.3/apysc/_type/array.py`

 * *Files identical despite different names*

### Comparing `apysc-4.4.2/apysc/_type/attr_linking_mixin.py` & `apysc-4.4.3/apysc/_type/attr_linking_mixin.py`

 * *Files identical despite different names*

### Comparing `apysc-4.4.2/apysc/_type/attr_to_apysc_val_from_builtin_mixin.py` & `apysc-4.4.3/apysc/_type/attr_to_apysc_val_from_builtin_mixin.py`

 * *Files identical despite different names*

### Comparing `apysc-4.4.2/apysc/_type/blank_object_mixin.py` & `apysc-4.4.3/apysc/_type/blank_object_mixin.py`

 * *Files identical despite different names*

### Comparing `apysc-4.4.2/apysc/_type/bool_const_mixin.py` & `apysc-4.4.3/apysc/_type/bool_const_mixin.py`

 * *Files identical despite different names*

### Comparing `apysc-4.4.2/apysc/_type/boolean.py` & `apysc-4.4.3/apysc/_type/boolean.py`

 * *Files identical despite different names*

### Comparing `apysc-4.4.2/apysc/_type/copy_mixin.py` & `apysc-4.4.3/apysc/_type/copy_mixin.py`

 * *Files identical despite different names*

### Comparing `apysc-4.4.2/apysc/_type/deleted_object_mixin.py` & `apysc-4.4.3/apysc/_type/deleted_object_mixin.py`

 * *Files identical despite different names*

### Comparing `apysc-4.4.2/apysc/_type/dictionary.py` & `apysc-4.4.3/apysc/_type/dictionary.py`

 * *Files identical despite different names*

### Comparing `apysc-4.4.2/apysc/_type/expression_string.py` & `apysc-4.4.3/apysc/_type/expression_string.py`

 * *Files identical despite different names*

### Comparing `apysc-4.4.2/apysc/_type/false.py` & `apysc-4.4.3/apysc/_type/false.py`

 * *Files identical despite different names*

### Comparing `apysc-4.4.2/apysc/_type/initial_substitution_exp_mixin.py` & `apysc-4.4.3/apysc/_type/initial_substitution_exp_mixin.py`

 * *Files identical despite different names*

### Comparing `apysc-4.4.2/apysc/_type/initialize_locals_and_globals_mixin.py` & `apysc-4.4.3/apysc/_type/initialize_locals_and_globals_mixin.py`

 * *Files identical despite different names*

### Comparing `apysc-4.4.2/apysc/_type/int.py` & `apysc-4.4.3/apysc/_type/int.py`

 * *Files identical despite different names*

### Comparing `apysc-4.4.2/apysc/_type/number.py` & `apysc-4.4.3/apysc/_type/number.py`

 * *Files identical despite different names*

### Comparing `apysc-4.4.2/apysc/_type/number_value_mixin.py` & `apysc-4.4.3/apysc/_type/number_value_mixin.py`

 * *Files identical despite different names*

### Comparing `apysc-4.4.2/apysc/_type/py_builtin_iter_disabling_mixin.py` & `apysc-4.4.3/apysc/_type/py_builtin_iter_disabling_mixin.py`

 * *Files identical despite different names*

### Comparing `apysc-4.4.2/apysc/_type/revert_interface.py` & `apysc-4.4.3/apysc/_type/revert_interface.py`

 * *Files identical despite different names*

### Comparing `apysc-4.4.2/apysc/_type/revert_mixin.py` & `apysc-4.4.3/apysc/_type/revert_mixin.py`

 * *Files identical despite different names*

### Comparing `apysc-4.4.2/apysc/_type/string.py` & `apysc-4.4.3/apysc/_type/string.py`

 * *Files identical despite different names*

### Comparing `apysc-4.4.2/apysc/_type/string_apply_max_num_of_decimal_places_mixin.py` & `apysc-4.4.3/apysc/_type/string_apply_max_num_of_decimal_places_mixin.py`

 * *Files identical despite different names*

### Comparing `apysc-4.4.2/apysc/_type/string_length_mixin.py` & `apysc-4.4.3/apysc/_type/string_length_mixin.py`

 * *Files identical despite different names*

### Comparing `apysc-4.4.2/apysc/_type/string_lower_mixin.py` & `apysc-4.4.3/apysc/_type/string_lower_mixin.py`

 * *Files identical despite different names*

### Comparing `apysc-4.4.2/apysc/_type/string_lstrip_mixin.py` & `apysc-4.4.3/apysc/_type/string_lstrip_mixin.py`

 * *Files identical despite different names*

### Comparing `apysc-4.4.2/apysc/_type/string_rstrip_mixin.py` & `apysc-4.4.3/apysc/_type/string_rstrip_mixin.py`

 * *Files identical despite different names*

### Comparing `apysc-4.4.2/apysc/_type/string_slice_mixin.py` & `apysc-4.4.3/apysc/_type/string_slice_mixin.py`

 * *Files identical despite different names*

### Comparing `apysc-4.4.2/apysc/_type/string_split_mixin.py` & `apysc-4.4.3/apysc/_type/string_split_mixin.py`

 * *Files identical despite different names*

### Comparing `apysc-4.4.2/apysc/_type/string_strip_mixin.py` & `apysc-4.4.3/apysc/_type/string_strip_mixin.py`

 * *Files identical despite different names*

### Comparing `apysc-4.4.2/apysc/_type/string_upper_mixin.py` & `apysc-4.4.3/apysc/_type/string_upper_mixin.py`

 * *Files identical despite different names*

### Comparing `apysc-4.4.2/apysc/_type/string_zfill_mixin.py` & `apysc-4.4.3/apysc/_type/string_zfill_mixin.py`

 * *Files identical despite different names*

### Comparing `apysc-4.4.2/apysc/_type/to_fixed_mixin.py` & `apysc-4.4.3/apysc/_type/to_fixed_mixin.py`

 * *Files identical despite different names*

### Comparing `apysc-4.4.2/apysc/_type/to_hex_mixin.py` & `apysc-4.4.3/apysc/_type/to_hex_mixin.py`

 * *Files identical despite different names*

### Comparing `apysc-4.4.2/apysc/_type/to_number_mixin.py` & `apysc-4.4.3/apysc/_type/to_number_mixin.py`

 * *Files identical despite different names*

### Comparing `apysc-4.4.2/apysc/_type/to_string_mixin.py` & `apysc-4.4.3/apysc/_type/to_string_mixin.py`

 * *Files identical despite different names*

### Comparing `apysc-4.4.2/apysc/_type/true.py` & `apysc-4.4.3/apysc/_type/true.py`

 * *Files identical despite different names*

### Comparing `apysc-4.4.2/apysc/_type/type_util.py` & `apysc-4.4.3/apysc/_type/type_util.py`

 * *Files identical despite different names*

### Comparing `apysc-4.4.2/apysc/_type/value_util.py` & `apysc-4.4.3/apysc/_type/value_util.py`

 * *Files identical despite different names*

### Comparing `apysc-4.4.2/apysc/_type/variable_name_mixin.py` & `apysc-4.4.3/apysc/_type/variable_name_mixin.py`

 * *Files identical despite different names*

### Comparing `apysc-4.4.2/apysc/_type/variable_name_suffix_attr_or_var_mixin.py` & `apysc-4.4.3/apysc/_type/variable_name_suffix_attr_or_var_mixin.py`

 * *Files identical despite different names*

### Comparing `apysc-4.4.2/apysc/_type/variable_name_suffix_mixin.py` & `apysc-4.4.3/apysc/_type/variable_name_suffix_mixin.py`

 * *Files identical despite different names*

### Comparing `apysc-4.4.2/apysc/_type/variable_name_suffix_utils.py` & `apysc-4.4.3/apysc/_type/variable_name_suffix_utils.py`

 * *Files identical despite different names*

### Comparing `apysc-4.4.2/apysc/_validation/arg_validation_decos.py` & `apysc-4.4.3/apysc/_validation/arg_validation_decos.py`

 * *Files identical despite different names*

### Comparing `apysc-4.4.2/apysc/_validation/bool_validation.py` & `apysc-4.4.3/apysc/_validation/bool_validation.py`

 * *Files identical despite different names*

### Comparing `apysc-4.4.2/apysc/_validation/color_validation.py` & `apysc-4.4.3/apysc/_validation/color_validation.py`

 * *Files identical despite different names*

### Comparing `apysc-4.4.2/apysc/_validation/display_validation.py` & `apysc-4.4.3/apysc/_validation/display_validation.py`

 * *Files identical despite different names*

### Comparing `apysc-4.4.2/apysc/_validation/event_validation.py` & `apysc-4.4.3/apysc/_validation/event_validation.py`

 * *Files identical despite different names*

### Comparing `apysc-4.4.2/apysc/_validation/geom_validation.py` & `apysc-4.4.3/apysc/_validation/geom_validation.py`

 * *Files identical despite different names*

### Comparing `apysc-4.4.2/apysc/_validation/handler_validation.py` & `apysc-4.4.3/apysc/_validation/handler_validation.py`

 * *Files identical despite different names*

### Comparing `apysc-4.4.2/apysc/_validation/matrix_data_validation.py` & `apysc-4.4.3/apysc/_validation/matrix_data_validation.py`

 * *Files identical despite different names*

### Comparing `apysc-4.4.2/apysc/_validation/number_validation.py` & `apysc-4.4.3/apysc/_validation/number_validation.py`

 * *Files identical despite different names*

### Comparing `apysc-4.4.2/apysc/_validation/parent_validation.py` & `apysc-4.4.3/apysc/_validation/parent_validation.py`

 * *Files identical despite different names*

### Comparing `apysc-4.4.2/apysc/_validation/path_validation.py` & `apysc-4.4.3/apysc/_validation/path_validation.py`

 * *Files identical despite different names*

### Comparing `apysc-4.4.2/apysc/_validation/string_validation.py` & `apysc-4.4.3/apysc/_validation/string_validation.py`

 * *Files identical despite different names*

### Comparing `apysc-4.4.2/apysc/_validation/validation_common_utils.py` & `apysc-4.4.3/apysc/_validation/validation_common_utils.py`

 * *Files identical despite different names*

### Comparing `apysc-4.4.2/apysc/_validation/variable_name_validation.py` & `apysc-4.4.3/apysc/_validation/variable_name_validation.py`

 * *Files identical despite different names*

### Comparing `apysc-4.4.2/apysc.egg-info/PKG-INFO` & `apysc-4.4.3/apysc.egg-info/PKG-INFO`

 * *Files 12% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: apysc
-Version: 4.4.2
+Version: 4.4.3
 Summary: apysc is the Python's frontend library to create html and js file, that has the ActionScript 3 (as3)-like interface.
 Home-page: https://github.com/simon-ritchie/apysc
 Maintainer: simon-ritchie
 Maintainer-email: 
 License: MIT
 Platform: UNKNOWN
 Classifier: Programming Language :: Python :: 3
```

### Comparing `apysc-4.4.2/apysc.egg-info/SOURCES.txt` & `apysc-4.4.3/apysc.egg-info/SOURCES.txt`

 * *Files 1% similar despite different names*

```diff
@@ -393,14 +393,16 @@
 apysc/_loop/for_array_values.py
 apysc/_loop/for_dict_keys.py
 apysc/_loop/for_dict_keys_and_values.py
 apysc/_loop/for_dict_values.py
 apysc/_loop/for_loop_exit_mixin.py
 apysc/_loop/initialize_with_base_value_interface.py
 apysc/_loop/loop_count.py
+apysc/_mask/__init__.py
+apysc/_mask/mask.py
 apysc/_material_design/__init__.py
 apysc/_material_design/icon/__init__.py
 apysc/_material_design/icon/material_10k_icon.py
 apysc/_material_design/icon/material_1k_icon.py
 apysc/_material_design/icon/material_1k_plus_icon.py
 apysc/_material_design/icon/material_2k_icon.py
 apysc/_material_design/icon/material_2k_plus_icon.py
@@ -1541,14 +1543,15 @@
 apysc/_material_design/icon/material_youtube_searched_for_icon.py
 apysc/_material_design/icon/material_youtube_searched_for_outlined_icon.py
 apysc/_material_design/icon/material_zoom_in_icon.py
 apysc/_material_design/icon/material_zoom_in_outlined_icon.py
 apysc/_material_design/icon/material_zoom_out_icon.py
 apysc/_material_design/icon/material_zoom_out_outlined_icon.py
 apysc/_math/__init__.py
+apysc/_math/clamp_mixin.py
 apysc/_math/math.py
 apysc/_math/max_mixin.py
 apysc/_math/min_mixin.py
 apysc/_math/trunc_mixin.py
 apysc/_string/__init__.py
 apysc/_string/indent_util.py
 apysc/_string/string_util.py
@@ -1726,14 +1729,15 @@
 apysc/_translation/jp/int_and_number_arithmetic_operations.py
 apysc/_translation/jp/int_and_number_comparison_operations.py
 apysc/_translation/jp/int_and_number_to_fixed.py
 apysc/_translation/jp/int_and_number_to_hex.py
 apysc/_translation/jp/line.py
 apysc/_translation/jp/material_design_colors.py
 apysc/_translation/jp/material_icon.py
+apysc/_translation/jp/math_clamp.py
 apysc/_translation/jp/math_max.py
 apysc/_translation/jp/math_min.py
 apysc/_translation/jp/math_trunc.py
 apysc/_translation/jp/mouse_event_abstract.py
 apysc/_translation/jp/mouse_event_basic.py
 apysc/_translation/jp/mousedown_and_mouseup.py
 apysc/_translation/jp/mousemove.py
```

