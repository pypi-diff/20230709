# Comparing `tmp/flet_lite-1.7.tar.gz` & `tmp/flet_lite-1.7.2.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "flet_lite-1.7.tar", last modified: Sun Jul  9 13:59:07 2023, max compression
+gzip compressed data, was "flet_lite-1.7.2.tar", last modified: Sun Jul  9 17:31:31 2023, max compression
```

## Comparing `flet_lite-1.7.tar` & `flet_lite-1.7.2.tar`

### file list

```diff
@@ -1,190 +1,194 @@
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-09 13:59:07.965749 flet_lite-1.7/
--rw-r--r--   0 runner    (1001) docker     (123)     1071 2023-07-09 13:58:58.000000 flet_lite-1.7/LICENSE
--rw-r--r--   0 runner    (1001) docker     (123)      285 2023-07-09 13:58:58.000000 flet_lite-1.7/MANIFEST.in
--rw-r--r--   0 runner    (1001) docker     (123)     3274 2023-07-09 13:59:07.965749 flet_lite-1.7/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (123)     2881 2023-07-09 13:58:58.000000 flet_lite-1.7/README.md
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-09 13:59:07.933749 flet_lite-1.7/flet/
--rw-r--r--   0 runner    (1001) docker     (123)     8196 2023-07-09 13:58:58.000000 flet_lite-1.7/flet/.DS_Store
--rw-r--r--   0 runner    (1001) docker     (123)      270 2023-07-09 13:58:58.000000 flet_lite-1.7/flet/__init__.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-09 13:59:07.937749 flet_lite-1.7/flet/api/
--rw-r--r--   0 runner    (1001) docker     (123)        0 2023-07-09 13:58:58.000000 flet_lite-1.7/flet/api/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)      788 2023-07-09 13:58:58.000000 flet_lite-1.7/flet/api/manage_client_pushes.py
--rw-r--r--   0 runner    (1001) docker     (123)      443 2023-07-09 13:58:58.000000 flet_lite-1.7/flet/api/push_add_request.py
--rw-r--r--   0 runner    (1001) docker     (123)      309 2023-07-09 13:58:58.000000 flet_lite-1.7/flet/api/push_clean_request.py
--rw-r--r--   0 runner    (1001) docker     (123)      307 2023-07-09 13:58:58.000000 flet_lite-1.7/flet/api/push_go_route_request.py
--rw-r--r--   0 runner    (1001) docker     (123)     1208 2023-07-09 13:58:58.000000 flet_lite-1.7/flet/api/push_page_update_request.py
--rw-r--r--   0 runner    (1001) docker     (123)      348 2023-07-09 13:58:58.000000 flet_lite-1.7/flet/api/push_remove_request.py
--rw-r--r--   0 runner    (1001) docker     (123)      507 2023-07-09 13:58:58.000000 flet_lite-1.7/flet/api/push_update_request.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-09 13:59:07.937749 flet_lite-1.7/flet/cli_tools/
--rw-r--r--   0 runner    (1001) docker     (123)        0 2023-07-09 13:58:58.000000 flet_lite-1.7/flet/cli_tools/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)     3175 2023-07-09 13:58:58.000000 flet_lite-1.7/flet/cli_tools/publish.py
--rw-r--r--   0 runner    (1001) docker     (123)     1114 2023-07-09 13:58:58.000000 flet_lite-1.7/flet/flet.py
--rw-r--r--   0 runner    (1001) docker     (123)     6922 2023-07-09 13:58:58.000000 flet_lite-1.7/flet/page.py
--rw-r--r--   0 runner    (1001) docker     (123)     1057 2023-07-09 13:58:58.000000 flet_lite-1.7/flet/publish.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-09 13:59:07.937749 flet_lite-1.7/flet/tools/
--rw-r--r--   0 runner    (1001) docker     (123)        0 2023-07-09 13:58:58.000000 flet_lite-1.7/flet/tools/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)     1426 2023-07-09 13:58:58.000000 flet_lite-1.7/flet/tools/append_assets_to_dist.py
--rw-r--r--   0 runner    (1001) docker     (123)      347 2023-07-09 13:58:58.000000 flet_lite-1.7/flet/tools/edit_control_props.py
--rw-r--r--   0 runner    (1001) docker     (123)     1361 2023-07-09 13:58:58.000000 flet_lite-1.7/flet/tools/run_event_function.py
--rw-r--r--   0 runner    (1001) docker     (123)     2402 2023-07-09 13:58:58.000000 flet_lite-1.7/flet/tools/setup_web.py
--rw-r--r--   0 runner    (1001) docker     (123)      521 2023-07-09 13:58:58.000000 flet_lite-1.7/flet/tools/update_control_on_event.py
--rw-r--r--   0 runner    (1001) docker     (123)     1084 2023-07-09 13:58:58.000000 flet_lite-1.7/flet/tools/update_page_info.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-09 13:59:07.937749 flet_lite-1.7/flet/utils/
--rw-r--r--   0 runner    (1001) docker     (123)        0 2023-07-09 13:58:58.000000 flet_lite-1.7/flet/utils/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)      860 2023-07-09 13:58:58.000000 flet_lite-1.7/flet/utils/all_props_posible.py
--rw-r--r--   0 runner    (1001) docker     (123)     2375 2023-07-09 13:58:58.000000 flet_lite-1.7/flet/utils/api_host.py
--rw-r--r--   0 runner    (1001) docker     (123)     2857 2023-07-09 13:58:58.000000 flet_lite-1.7/flet/utils/appbar_coder.py
--rw-r--r--   0 runner    (1001) docker     (123)     1892 2023-07-09 13:58:58.000000 flet_lite-1.7/flet/utils/control_coder.py
--rw-r--r--   0 runner    (1001) docker     (123)     1507 2023-07-09 13:58:58.000000 flet_lite-1.7/flet/utils/get_all_subcontrols.py
--rw-r--r--   0 runner    (1001) docker     (123)      616 2023-07-09 13:58:58.000000 flet_lite-1.7/flet/utils/get_control_data.py
--rw-r--r--   0 runner    (1001) docker     (123)      176 2023-07-09 13:58:58.000000 flet_lite-1.7/flet/utils/get_free_port.py
--rw-r--r--   0 runner    (1001) docker     (123)      722 2023-07-09 13:58:58.000000 flet_lite-1.7/flet/utils/page_posible_props.py
--rw-r--r--   0 runner    (1001) docker     (123)     2334 2023-07-09 13:58:58.000000 flet_lite-1.7/flet/utils/view_coder.py
--rw-r--r--   0 runner    (1001) docker     (123)      663 2023-07-09 13:58:58.000000 flet_lite-1.7/flet/utils/web_host.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-09 13:59:07.941749 flet_lite-1.7/flet/web/
--rw-r--r--   0 runner    (1001) docker     (123)     6148 2023-07-09 13:58:58.000000 flet_lite-1.7/flet/web/.DS_Store
--rw-r--r--   0 runner    (1001) docker     (123)        0 2023-07-09 13:58:58.000000 flet_lite-1.7/flet/web/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)  4313577 2023-07-09 13:58:58.000000 flet_lite-1.7/flet/web/development.zip
--rw-r--r--   0 runner    (1001) docker     (123)  4292224 2023-07-09 13:58:58.000000 flet_lite-1.7/flet/web/dist.zip
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-09 13:59:07.961749 flet_lite-1.7/flet_core/
--rw-r--r--   0 runner    (1001) docker     (123)     6457 2023-07-09 13:58:58.000000 flet_lite-1.7/flet_core/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)     6774 2023-07-09 13:58:58.000000 flet_lite-1.7/flet_core/alert_dialog.py
--rw-r--r--   0 runner    (1001) docker     (123)      407 2023-07-09 13:58:58.000000 flet_lite-1.7/flet_core/alignment.py
--rw-r--r--   0 runner    (1001) docker     (123)     7226 2023-07-09 13:58:58.000000 flet_lite-1.7/flet_core/animated_switcher.py
--rw-r--r--   0 runner    (1001) docker     (123)     2806 2023-07-09 13:58:58.000000 flet_lite-1.7/flet_core/animation.py
--rw-r--r--   0 runner    (1001) docker     (123)     5403 2023-07-09 13:58:58.000000 flet_lite-1.7/flet_core/app_bar.py
--rw-r--r--   0 runner    (1001) docker     (123)     7301 2023-07-09 13:58:58.000000 flet_lite-1.7/flet_core/audio.py
--rw-r--r--   0 runner    (1001) docker     (123)     5446 2023-07-09 13:58:58.000000 flet_lite-1.7/flet_core/banner.py
--rw-r--r--   0 runner    (1001) docker     (123)      326 2023-07-09 13:58:58.000000 flet_lite-1.7/flet_core/blur.py
--rw-r--r--   0 runner    (1001) docker     (123)     1079 2023-07-09 13:58:58.000000 flet_lite-1.7/flet_core/border.py
--rw-r--r--   0 runner    (1001) docker     (123)      958 2023-07-09 13:58:58.000000 flet_lite-1.7/flet_core/border_radius.py
--rw-r--r--   0 runner    (1001) docker     (123)     2826 2023-07-09 13:58:58.000000 flet_lite-1.7/flet_core/bottom_sheet.py
--rw-r--r--   0 runner    (1001) docker     (123)     2202 2023-07-09 13:58:58.000000 flet_lite-1.7/flet_core/buttons.py
--rw-r--r--   0 runner    (1001) docker     (123)     3044 2023-07-09 13:58:58.000000 flet_lite-1.7/flet_core/callable_control.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-09 13:59:07.961749 flet_lite-1.7/flet_core/canvas/
--rw-r--r--   0 runner    (1001) docker     (123)      514 2023-07-09 13:58:58.000000 flet_lite-1.7/flet_core/canvas/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)     2903 2023-07-09 13:58:58.000000 flet_lite-1.7/flet_core/canvas/arc.py
--rw-r--r--   0 runner    (1001) docker     (123)     4629 2023-07-09 13:58:58.000000 flet_lite-1.7/flet_core/canvas/canvas.py
--rw-r--r--   0 runner    (1001) docker     (123)     1639 2023-07-09 13:58:58.000000 flet_lite-1.7/flet_core/canvas/circle.py
--rw-r--r--   0 runner    (1001) docker     (123)     1361 2023-07-09 13:58:58.000000 flet_lite-1.7/flet_core/canvas/color.py
--rw-r--r--   0 runner    (1001) docker     (123)      837 2023-07-09 13:58:58.000000 flet_lite-1.7/flet_core/canvas/fill.py
--rw-r--r--   0 runner    (1001) docker     (123)     1862 2023-07-09 13:58:58.000000 flet_lite-1.7/flet_core/canvas/line.py
--rw-r--r--   0 runner    (1001) docker     (123)     1907 2023-07-09 13:58:58.000000 flet_lite-1.7/flet_core/canvas/oval.py
--rw-r--r--   0 runner    (1001) docker     (123)     3486 2023-07-09 13:58:58.000000 flet_lite-1.7/flet_core/canvas/path.py
--rw-r--r--   0 runner    (1001) docker     (123)     1772 2023-07-09 13:58:58.000000 flet_lite-1.7/flet_core/canvas/points.py
--rw-r--r--   0 runner    (1001) docker     (123)     2361 2023-07-09 13:58:58.000000 flet_lite-1.7/flet_core/canvas/rect.py
--rw-r--r--   0 runner    (1001) docker     (123)     1963 2023-07-09 13:58:58.000000 flet_lite-1.7/flet_core/canvas/shadow.py
--rw-r--r--   0 runner    (1001) docker     (123)      347 2023-07-09 13:58:58.000000 flet_lite-1.7/flet_core/canvas/shape.py
--rw-r--r--   0 runner    (1001) docker     (123)     4172 2023-07-09 13:58:58.000000 flet_lite-1.7/flet_core/canvas/text.py
--rw-r--r--   0 runner    (1001) docker     (123)     5695 2023-07-09 13:58:58.000000 flet_lite-1.7/flet_core/card.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-09 13:59:07.961749 flet_lite-1.7/flet_core/charts/
--rw-r--r--   0 runner    (1001) docker     (123)        0 2023-07-09 13:58:58.000000 flet_lite-1.7/flet_core/charts/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)     9855 2023-07-09 13:58:58.000000 flet_lite-1.7/flet_core/charts/bar_chart.py
--rw-r--r--   0 runner    (1001) docker     (123)     2061 2023-07-09 13:58:58.000000 flet_lite-1.7/flet_core/charts/bar_chart_group.py
--rw-r--r--   0 runner    (1001) docker     (123)     6837 2023-07-09 13:58:58.000000 flet_lite-1.7/flet_core/charts/bar_chart_rod.py
--rw-r--r--   0 runner    (1001) docker     (123)     1949 2023-07-09 13:58:58.000000 flet_lite-1.7/flet_core/charts/bar_chart_rod_stack_item.py
--rw-r--r--   0 runner    (1001) docker     (123)     2924 2023-07-09 13:58:58.000000 flet_lite-1.7/flet_core/charts/chart_axis.py
--rw-r--r--   0 runner    (1001) docker     (123)     1293 2023-07-09 13:58:58.000000 flet_lite-1.7/flet_core/charts/chart_axis_label.py
--rw-r--r--   0 runner    (1001) docker     (123)      338 2023-07-09 13:58:58.000000 flet_lite-1.7/flet_core/charts/chart_grid_lines.py
--rw-r--r--   0 runner    (1001) docker     (123)      286 2023-07-09 13:58:58.000000 flet_lite-1.7/flet_core/charts/chart_point_line.py
--rw-r--r--   0 runner    (1001) docker     (123)     1006 2023-07-09 13:58:58.000000 flet_lite-1.7/flet_core/charts/chart_point_shape.py
--rw-r--r--   0 runner    (1001) docker     (123)    11228 2023-07-09 13:58:58.000000 flet_lite-1.7/flet_core/charts/line_chart.py
--rw-r--r--   0 runner    (1001) docker     (123)     8258 2023-07-09 13:58:58.000000 flet_lite-1.7/flet_core/charts/line_chart_data.py
--rw-r--r--   0 runner    (1001) docker     (123)     5496 2023-07-09 13:58:58.000000 flet_lite-1.7/flet_core/charts/line_chart_data_point.py
--rw-r--r--   0 runner    (1001) docker     (123)     5888 2023-07-09 13:58:58.000000 flet_lite-1.7/flet_core/charts/pie_chart.py
--rw-r--r--   0 runner    (1001) docker     (123)     3824 2023-07-09 13:58:58.000000 flet_lite-1.7/flet_core/charts/pie_chart_section.py
--rw-r--r--   0 runner    (1001) docker     (123)     7156 2023-07-09 13:58:58.000000 flet_lite-1.7/flet_core/checkbox.py
--rw-r--r--   0 runner    (1001) docker     (123)     6795 2023-07-09 13:58:58.000000 flet_lite-1.7/flet_core/circle_avatar.py
--rw-r--r--   0 runner    (1001) docker     (123)     3085 2023-07-09 13:58:58.000000 flet_lite-1.7/flet_core/client_storage.py
--rw-r--r--   0 runner    (1001) docker     (123)     1002 2023-07-09 13:58:58.000000 flet_lite-1.7/flet_core/clipboard.py
--rw-r--r--   0 runner    (1001) docker     (123)    10708 2023-07-09 13:58:58.000000 flet_lite-1.7/flet_core/colors.py
--rw-r--r--   0 runner    (1001) docker     (123)     6924 2023-07-09 13:58:58.000000 flet_lite-1.7/flet_core/column.py
--rw-r--r--   0 runner    (1001) docker     (123)     1132 2023-07-09 13:58:58.000000 flet_lite-1.7/flet_core/connection.py
--rw-r--r--   0 runner    (1001) docker     (123)     7099 2023-07-09 13:58:58.000000 flet_lite-1.7/flet_core/constrained_control.py
--rw-r--r--   0 runner    (1001) docker     (123)    14684 2023-07-09 13:58:58.000000 flet_lite-1.7/flet_core/container.py
--rw-r--r--   0 runner    (1001) docker     (123)    14133 2023-07-09 13:58:58.000000 flet_lite-1.7/flet_core/control.py
--rw-r--r--   0 runner    (1001) docker     (123)      260 2023-07-09 13:58:58.000000 flet_lite-1.7/flet_core/control_event.py
--rw-r--r--   0 runner    (1001) docker     (123)    20707 2023-07-09 13:58:58.000000 flet_lite-1.7/flet_core/datatable.py
--rw-r--r--   0 runner    (1001) docker     (123)     2263 2023-07-09 13:58:58.000000 flet_lite-1.7/flet_core/divider.py
--rw-r--r--   0 runner    (1001) docker     (123)     6270 2023-07-09 13:58:58.000000 flet_lite-1.7/flet_core/drag_target.py
--rw-r--r--   0 runner    (1001) docker     (123)     6063 2023-07-09 13:58:58.000000 flet_lite-1.7/flet_core/draggable.py
--rw-r--r--   0 runner    (1001) docker     (123)     9177 2023-07-09 13:58:58.000000 flet_lite-1.7/flet_core/dropdown.py
--rw-r--r--   0 runner    (1001) docker     (123)     8804 2023-07-09 13:58:58.000000 flet_lite-1.7/flet_core/elevated_button.py
--rw-r--r--   0 runner    (1001) docker     (123)     1978 2023-07-09 13:58:58.000000 flet_lite-1.7/flet_core/embed_json_encoder.py
--rw-r--r--   0 runner    (1001) docker     (123)      166 2023-07-09 13:58:58.000000 flet_lite-1.7/flet_core/event.py
--rw-r--r--   0 runner    (1001) docker     (123)     1839 2023-07-09 13:58:58.000000 flet_lite-1.7/flet_core/event_handler.py
--rw-r--r--   0 runner    (1001) docker     (123)     9777 2023-07-09 13:58:58.000000 flet_lite-1.7/flet_core/file_picker.py
--rw-r--r--   0 runner    (1001) docker     (123)     2694 2023-07-09 13:58:58.000000 flet_lite-1.7/flet_core/filled_button.py
--rw-r--r--   0 runner    (1001) docker     (123)     2828 2023-07-09 13:58:58.000000 flet_lite-1.7/flet_core/filled_tonal_button.py
--rw-r--r--   0 runner    (1001) docker     (123)     2542 2023-07-09 13:58:58.000000 flet_lite-1.7/flet_core/flet_app.py
--rw-r--r--   0 runner    (1001) docker     (123)     7111 2023-07-09 13:58:58.000000 flet_lite-1.7/flet_core/floating_action_button.py
--rw-r--r--   0 runner    (1001) docker     (123)    13981 2023-07-09 13:58:58.000000 flet_lite-1.7/flet_core/form_field_control.py
--rw-r--r--   0 runner    (1001) docker     (123)    28044 2023-07-09 13:58:58.000000 flet_lite-1.7/flet_core/gesture_detector.py
--rw-r--r--   0 runner    (1001) docker     (123)     1531 2023-07-09 13:58:58.000000 flet_lite-1.7/flet_core/gradients.py
--rw-r--r--   0 runner    (1001) docker     (123)     6804 2023-07-09 13:58:58.000000 flet_lite-1.7/flet_core/grid_view.py
--rw-r--r--   0 runner    (1001) docker     (123)     2134 2023-07-09 13:58:58.000000 flet_lite-1.7/flet_core/haptic_feedback.py
--rw-r--r--   0 runner    (1001) docker     (123)     3430 2023-07-09 13:58:58.000000 flet_lite-1.7/flet_core/icon.py
--rw-r--r--   0 runner    (1001) docker     (123)     8438 2023-07-09 13:58:58.000000 flet_lite-1.7/flet_core/icon_button.py
--rw-r--r--   0 runner    (1001) docker     (123)   362652 2023-07-09 13:58:58.000000 flet_lite-1.7/flet_core/icons.py
--rw-r--r--   0 runner    (1001) docker     (123)     6585 2023-07-09 13:58:58.000000 flet_lite-1.7/flet_core/image.py
--rw-r--r--   0 runner    (1001) docker     (123)      367 2023-07-09 13:58:58.000000 flet_lite-1.7/flet_core/inline_span.py
--rw-r--r--   0 runner    (1001) docker     (123)     8360 2023-07-09 13:58:58.000000 flet_lite-1.7/flet_core/list_tile.py
--rw-r--r--   0 runner    (1001) docker     (123)     6401 2023-07-09 13:58:58.000000 flet_lite-1.7/flet_core/list_view.py
--rw-r--r--   0 runner    (1001) docker     (123)     8644 2023-07-09 13:58:58.000000 flet_lite-1.7/flet_core/local_connection.py
--rw-r--r--   0 runner    (1001) docker     (123)      223 2023-07-09 13:58:58.000000 flet_lite-1.7/flet_core/locks.py
--rw-r--r--   0 runner    (1001) docker     (123)      583 2023-07-09 13:58:58.000000 flet_lite-1.7/flet_core/margin.py
--rw-r--r--   0 runner    (1001) docker     (123)     6129 2023-07-09 13:58:58.000000 flet_lite-1.7/flet_core/markdown.py
--rw-r--r--   0 runner    (1001) docker     (123)     5180 2023-07-09 13:58:58.000000 flet_lite-1.7/flet_core/matplotlib_chart.py
--rw-r--r--   0 runner    (1001) docker     (123)     8322 2023-07-09 13:58:58.000000 flet_lite-1.7/flet_core/navigation_bar.py
--rw-r--r--   0 runner    (1001) docker     (123)    11986 2023-07-09 13:58:58.000000 flet_lite-1.7/flet_core/navigation_rail.py
--rw-r--r--   0 runner    (1001) docker     (123)     7489 2023-07-09 13:58:58.000000 flet_lite-1.7/flet_core/outlined_button.py
--rw-r--r--   0 runner    (1001) docker     (123)      587 2023-07-09 13:58:58.000000 flet_lite-1.7/flet_core/padding.py
--rw-r--r--   0 runner    (1001) docker     (123)    53719 2023-07-09 13:58:58.000000 flet_lite-1.7/flet_core/page.py
--rw-r--r--   0 runner    (1001) docker     (123)     2674 2023-07-09 13:58:58.000000 flet_lite-1.7/flet_core/painting.py
--rw-r--r--   0 runner    (1001) docker     (123)     4410 2023-07-09 13:58:58.000000 flet_lite-1.7/flet_core/plotly_chart.py
--rw-r--r--   0 runner    (1001) docker     (123)     6811 2023-07-09 13:58:58.000000 flet_lite-1.7/flet_core/popup_menu_button.py
--rw-r--r--   0 runner    (1001) docker     (123)     4293 2023-07-09 13:58:58.000000 flet_lite-1.7/flet_core/progress_bar.py
--rw-r--r--   0 runner    (1001) docker     (123)     4491 2023-07-09 13:58:58.000000 flet_lite-1.7/flet_core/progress_ring.py
--rw-r--r--   0 runner    (1001) docker     (123)     4088 2023-07-09 13:58:58.000000 flet_lite-1.7/flet_core/protocol.py
--rw-r--r--   0 runner    (1001) docker     (123)     3419 2023-07-09 13:58:58.000000 flet_lite-1.7/flet_core/querystring.py
--rw-r--r--   0 runner    (1001) docker     (123)     5765 2023-07-09 13:58:58.000000 flet_lite-1.7/flet_core/radio.py
--rw-r--r--   0 runner    (1001) docker     (123)     2389 2023-07-09 13:58:58.000000 flet_lite-1.7/flet_core/radio_group.py
--rw-r--r--   0 runner    (1001) docker     (123)      291 2023-07-09 13:58:58.000000 flet_lite-1.7/flet_core/ref.py
--rw-r--r--   0 runner    (1001) docker     (123)     6344 2023-07-09 13:58:58.000000 flet_lite-1.7/flet_core/responsive_row.py
--rw-r--r--   0 runner    (1001) docker     (123)     6908 2023-07-09 13:58:58.000000 flet_lite-1.7/flet_core/row.py
--rw-r--r--   0 runner    (1001) docker     (123)     4486 2023-07-09 13:58:58.000000 flet_lite-1.7/flet_core/scrollable_control.py
--rw-r--r--   0 runner    (1001) docker     (123)     1637 2023-07-09 13:58:58.000000 flet_lite-1.7/flet_core/semantics.py
--rw-r--r--   0 runner    (1001) docker     (123)      576 2023-07-09 13:58:58.000000 flet_lite-1.7/flet_core/session_storage.py
--rw-r--r--   0 runner    (1001) docker     (123)     5318 2023-07-09 13:58:58.000000 flet_lite-1.7/flet_core/shader_mask.py
--rw-r--r--   0 runner    (1001) docker     (123)      572 2023-07-09 13:58:58.000000 flet_lite-1.7/flet_core/shadow.py
--rw-r--r--   0 runner    (1001) docker     (123)     2919 2023-07-09 13:58:58.000000 flet_lite-1.7/flet_core/shake_detector.py
--rw-r--r--   0 runner    (1001) docker     (123)     7382 2023-07-09 13:58:58.000000 flet_lite-1.7/flet_core/slider.py
--rw-r--r--   0 runner    (1001) docker     (123)     3971 2023-07-09 13:58:58.000000 flet_lite-1.7/flet_core/snack_bar.py
--rw-r--r--   0 runner    (1001) docker     (123)     4889 2023-07-09 13:58:58.000000 flet_lite-1.7/flet_core/stack.py
--rw-r--r--   0 runner    (1001) docker     (123)     8104 2023-07-09 13:58:58.000000 flet_lite-1.7/flet_core/switch.py
--rw-r--r--   0 runner    (1001) docker     (123)    10820 2023-07-09 13:58:58.000000 flet_lite-1.7/flet_core/tabs.py
--rw-r--r--   0 runner    (1001) docker     (123)      632 2023-07-09 13:58:58.000000 flet_lite-1.7/flet_core/template_route.py
--rw-r--r--   0 runner    (1001) docker     (123)    10568 2023-07-09 13:58:58.000000 flet_lite-1.7/flet_core/text.py
--rw-r--r--   0 runner    (1001) docker     (123)     7462 2023-07-09 13:58:58.000000 flet_lite-1.7/flet_core/text_button.py
--rw-r--r--   0 runner    (1001) docker     (123)     3092 2023-07-09 13:58:58.000000 flet_lite-1.7/flet_core/text_span.py
--rw-r--r--   0 runner    (1001) docker     (123)     1260 2023-07-09 13:58:58.000000 flet_lite-1.7/flet_core/text_style.py
--rw-r--r--   0 runner    (1001) docker     (123)    15444 2023-07-09 13:58:58.000000 flet_lite-1.7/flet_core/textfield.py
--rw-r--r--   0 runner    (1001) docker     (123)     6172 2023-07-09 13:58:58.000000 flet_lite-1.7/flet_core/theme.py
--rw-r--r--   0 runner    (1001) docker     (123)     8362 2023-07-09 13:58:58.000000 flet_lite-1.7/flet_core/tooltip.py
--rw-r--r--   0 runner    (1001) docker     (123)      544 2023-07-09 13:58:58.000000 flet_lite-1.7/flet_core/transform.py
--rw-r--r--   0 runner    (1001) docker     (123)     2753 2023-07-09 13:58:58.000000 flet_lite-1.7/flet_core/transparent_pointer.py
--rw-r--r--   0 runner    (1001) docker     (123)     5186 2023-07-09 13:58:58.000000 flet_lite-1.7/flet_core/types.py
--rw-r--r--   0 runner    (1001) docker     (123)      684 2023-07-09 13:58:58.000000 flet_lite-1.7/flet_core/user_control.py
--rw-r--r--   0 runner    (1001) docker     (123)      409 2023-07-09 13:58:58.000000 flet_lite-1.7/flet_core/utils.py
--rw-r--r--   0 runner    (1001) docker     (123)     2337 2023-07-09 13:58:58.000000 flet_lite-1.7/flet_core/vertical_divider.py
--rw-r--r--   0 runner    (1001) docker     (123)     5852 2023-07-09 13:58:58.000000 flet_lite-1.7/flet_core/view.py
--rw-r--r--   0 runner    (1001) docker     (123)     4049 2023-07-09 13:58:58.000000 flet_lite-1.7/flet_core/window_drag_area.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-09 13:59:07.965749 flet_lite-1.7/flet_lite.egg-info/
--rw-r--r--   0 runner    (1001) docker     (123)     3274 2023-07-09 13:59:07.000000 flet_lite-1.7/flet_lite.egg-info/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (123)     4528 2023-07-09 13:59:07.000000 flet_lite-1.7/flet_lite.egg-info/SOURCES.txt
--rw-r--r--   0 runner    (1001) docker     (123)        1 2023-07-09 13:59:07.000000 flet_lite-1.7/flet_lite.egg-info/dependency_links.txt
--rw-r--r--   0 runner    (1001) docker     (123)       35 2023-07-09 13:59:07.000000 flet_lite-1.7/flet_lite.egg-info/requires.txt
--rw-r--r--   0 runner    (1001) docker     (123)       15 2023-07-09 13:59:07.000000 flet_lite-1.7/flet_lite.egg-info/top_level.txt
--rw-r--r--   0 runner    (1001) docker     (123)      103 2023-07-09 13:58:58.000000 flet_lite-1.7/pyproject.toml
--rw-r--r--   0 runner    (1001) docker     (123)       38 2023-07-09 13:59:07.965749 flet_lite-1.7/setup.cfg
--rw-r--r--   0 runner    (1001) docker     (123)      832 2023-07-09 13:58:58.000000 flet_lite-1.7/setup.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-09 17:31:31.924562 flet_lite-1.7.2/
+-rw-r--r--   0 runner    (1001) docker     (123)     1071 2023-07-09 17:31:22.000000 flet_lite-1.7.2/LICENSE
+-rw-r--r--   0 runner    (1001) docker     (123)      325 2023-07-09 17:31:22.000000 flet_lite-1.7.2/MANIFEST.in
+-rw-r--r--   0 runner    (1001) docker     (123)     3276 2023-07-09 17:31:31.924562 flet_lite-1.7.2/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (123)     2881 2023-07-09 17:31:22.000000 flet_lite-1.7.2/README.md
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-09 17:31:31.896563 flet_lite-1.7.2/flet/
+-rw-r--r--   0 runner    (1001) docker     (123)     8196 2023-07-09 17:31:22.000000 flet_lite-1.7.2/flet/.DS_Store
+-rw-r--r--   0 runner    (1001) docker     (123)      270 2023-07-09 17:31:22.000000 flet_lite-1.7.2/flet/__init__.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-09 17:31:31.896563 flet_lite-1.7.2/flet/api/
+-rw-r--r--   0 runner    (1001) docker     (123)        0 2023-07-09 17:31:22.000000 flet_lite-1.7.2/flet/api/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)      788 2023-07-09 17:31:22.000000 flet_lite-1.7.2/flet/api/manage_client_pushes.py
+-rw-r--r--   0 runner    (1001) docker     (123)      443 2023-07-09 17:31:22.000000 flet_lite-1.7.2/flet/api/push_add_request.py
+-rw-r--r--   0 runner    (1001) docker     (123)      309 2023-07-09 17:31:22.000000 flet_lite-1.7.2/flet/api/push_clean_request.py
+-rw-r--r--   0 runner    (1001) docker     (123)      307 2023-07-09 17:31:22.000000 flet_lite-1.7.2/flet/api/push_go_route_request.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1208 2023-07-09 17:31:22.000000 flet_lite-1.7.2/flet/api/push_page_update_request.py
+-rw-r--r--   0 runner    (1001) docker     (123)      348 2023-07-09 17:31:22.000000 flet_lite-1.7.2/flet/api/push_remove_request.py
+-rw-r--r--   0 runner    (1001) docker     (123)      507 2023-07-09 17:31:22.000000 flet_lite-1.7.2/flet/api/push_update_request.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-09 17:31:31.896563 flet_lite-1.7.2/flet/cli_tools/
+-rw-r--r--   0 runner    (1001) docker     (123)        0 2023-07-09 17:31:22.000000 flet_lite-1.7.2/flet/cli_tools/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)     3175 2023-07-09 17:31:22.000000 flet_lite-1.7.2/flet/cli_tools/publish.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1285 2023-07-09 17:31:22.000000 flet_lite-1.7.2/flet/flet.py
+-rw-r--r--   0 runner    (1001) docker     (123)     7161 2023-07-09 17:31:22.000000 flet_lite-1.7.2/flet/page.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1057 2023-07-09 17:31:22.000000 flet_lite-1.7.2/flet/publish.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-09 17:31:31.896563 flet_lite-1.7.2/flet/tools/
+-rw-r--r--   0 runner    (1001) docker     (123)        0 2023-07-09 17:31:22.000000 flet_lite-1.7.2/flet/tools/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1426 2023-07-09 17:31:22.000000 flet_lite-1.7.2/flet/tools/append_assets_to_dist.py
+-rw-r--r--   0 runner    (1001) docker     (123)      347 2023-07-09 17:31:22.000000 flet_lite-1.7.2/flet/tools/edit_control_props.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-09 17:31:31.896563 flet_lite-1.7.2/flet/tools/platform_specifics/
+-rw-r--r--   0 runner    (1001) docker     (123)        0 2023-07-09 17:31:22.000000 flet_lite-1.7.2/flet/tools/platform_specifics/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)      175 2023-07-09 17:31:22.000000 flet_lite-1.7.2/flet/tools/platform_specifics/get_platform_name.py
+-rw-r--r--   0 runner    (1001) docker     (123)     2100 2023-07-09 17:31:22.000000 flet_lite-1.7.2/flet/tools/platform_specifics/pythonista_webview.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1361 2023-07-09 17:31:22.000000 flet_lite-1.7.2/flet/tools/run_event_function.py
+-rw-r--r--   0 runner    (1001) docker     (123)     2402 2023-07-09 17:31:22.000000 flet_lite-1.7.2/flet/tools/setup_web.py
+-rw-r--r--   0 runner    (1001) docker     (123)      521 2023-07-09 17:31:22.000000 flet_lite-1.7.2/flet/tools/update_control_on_event.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1084 2023-07-09 17:31:22.000000 flet_lite-1.7.2/flet/tools/update_page_info.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-09 17:31:31.900563 flet_lite-1.7.2/flet/utils/
+-rw-r--r--   0 runner    (1001) docker     (123)        0 2023-07-09 17:31:22.000000 flet_lite-1.7.2/flet/utils/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)      860 2023-07-09 17:31:22.000000 flet_lite-1.7.2/flet/utils/all_props_posible.py
+-rw-r--r--   0 runner    (1001) docker     (123)     2375 2023-07-09 17:31:22.000000 flet_lite-1.7.2/flet/utils/api_host.py
+-rw-r--r--   0 runner    (1001) docker     (123)     2857 2023-07-09 17:31:22.000000 flet_lite-1.7.2/flet/utils/appbar_coder.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1892 2023-07-09 17:31:22.000000 flet_lite-1.7.2/flet/utils/control_coder.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1507 2023-07-09 17:31:22.000000 flet_lite-1.7.2/flet/utils/get_all_subcontrols.py
+-rw-r--r--   0 runner    (1001) docker     (123)      616 2023-07-09 17:31:22.000000 flet_lite-1.7.2/flet/utils/get_control_data.py
+-rw-r--r--   0 runner    (1001) docker     (123)      176 2023-07-09 17:31:22.000000 flet_lite-1.7.2/flet/utils/get_free_port.py
+-rw-r--r--   0 runner    (1001) docker     (123)      722 2023-07-09 17:31:22.000000 flet_lite-1.7.2/flet/utils/page_posible_props.py
+-rw-r--r--   0 runner    (1001) docker     (123)     2334 2023-07-09 17:31:22.000000 flet_lite-1.7.2/flet/utils/view_coder.py
+-rw-r--r--   0 runner    (1001) docker     (123)      663 2023-07-09 17:31:22.000000 flet_lite-1.7.2/flet/utils/web_host.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-09 17:31:31.904563 flet_lite-1.7.2/flet/web/
+-rw-r--r--   0 runner    (1001) docker     (123)     6148 2023-07-09 17:31:22.000000 flet_lite-1.7.2/flet/web/.DS_Store
+-rw-r--r--   0 runner    (1001) docker     (123)        0 2023-07-09 17:31:22.000000 flet_lite-1.7.2/flet/web/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)  4313577 2023-07-09 17:31:22.000000 flet_lite-1.7.2/flet/web/development.zip
+-rw-r--r--   0 runner    (1001) docker     (123)  4292224 2023-07-09 17:31:22.000000 flet_lite-1.7.2/flet/web/dist.zip
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-09 17:31:31.920562 flet_lite-1.7.2/flet_core/
+-rw-r--r--   0 runner    (1001) docker     (123)     6457 2023-07-09 17:31:22.000000 flet_lite-1.7.2/flet_core/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)     6774 2023-07-09 17:31:22.000000 flet_lite-1.7.2/flet_core/alert_dialog.py
+-rw-r--r--   0 runner    (1001) docker     (123)      407 2023-07-09 17:31:22.000000 flet_lite-1.7.2/flet_core/alignment.py
+-rw-r--r--   0 runner    (1001) docker     (123)     7226 2023-07-09 17:31:22.000000 flet_lite-1.7.2/flet_core/animated_switcher.py
+-rw-r--r--   0 runner    (1001) docker     (123)     2806 2023-07-09 17:31:22.000000 flet_lite-1.7.2/flet_core/animation.py
+-rw-r--r--   0 runner    (1001) docker     (123)     5403 2023-07-09 17:31:22.000000 flet_lite-1.7.2/flet_core/app_bar.py
+-rw-r--r--   0 runner    (1001) docker     (123)     7301 2023-07-09 17:31:22.000000 flet_lite-1.7.2/flet_core/audio.py
+-rw-r--r--   0 runner    (1001) docker     (123)     5446 2023-07-09 17:31:22.000000 flet_lite-1.7.2/flet_core/banner.py
+-rw-r--r--   0 runner    (1001) docker     (123)      326 2023-07-09 17:31:22.000000 flet_lite-1.7.2/flet_core/blur.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1079 2023-07-09 17:31:22.000000 flet_lite-1.7.2/flet_core/border.py
+-rw-r--r--   0 runner    (1001) docker     (123)      958 2023-07-09 17:31:22.000000 flet_lite-1.7.2/flet_core/border_radius.py
+-rw-r--r--   0 runner    (1001) docker     (123)     2826 2023-07-09 17:31:22.000000 flet_lite-1.7.2/flet_core/bottom_sheet.py
+-rw-r--r--   0 runner    (1001) docker     (123)     2202 2023-07-09 17:31:22.000000 flet_lite-1.7.2/flet_core/buttons.py
+-rw-r--r--   0 runner    (1001) docker     (123)     3044 2023-07-09 17:31:22.000000 flet_lite-1.7.2/flet_core/callable_control.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-09 17:31:31.920562 flet_lite-1.7.2/flet_core/canvas/
+-rw-r--r--   0 runner    (1001) docker     (123)      514 2023-07-09 17:31:22.000000 flet_lite-1.7.2/flet_core/canvas/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)     2903 2023-07-09 17:31:22.000000 flet_lite-1.7.2/flet_core/canvas/arc.py
+-rw-r--r--   0 runner    (1001) docker     (123)     4629 2023-07-09 17:31:22.000000 flet_lite-1.7.2/flet_core/canvas/canvas.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1639 2023-07-09 17:31:22.000000 flet_lite-1.7.2/flet_core/canvas/circle.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1361 2023-07-09 17:31:22.000000 flet_lite-1.7.2/flet_core/canvas/color.py
+-rw-r--r--   0 runner    (1001) docker     (123)      837 2023-07-09 17:31:22.000000 flet_lite-1.7.2/flet_core/canvas/fill.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1862 2023-07-09 17:31:22.000000 flet_lite-1.7.2/flet_core/canvas/line.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1907 2023-07-09 17:31:22.000000 flet_lite-1.7.2/flet_core/canvas/oval.py
+-rw-r--r--   0 runner    (1001) docker     (123)     3486 2023-07-09 17:31:22.000000 flet_lite-1.7.2/flet_core/canvas/path.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1772 2023-07-09 17:31:22.000000 flet_lite-1.7.2/flet_core/canvas/points.py
+-rw-r--r--   0 runner    (1001) docker     (123)     2361 2023-07-09 17:31:22.000000 flet_lite-1.7.2/flet_core/canvas/rect.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1963 2023-07-09 17:31:22.000000 flet_lite-1.7.2/flet_core/canvas/shadow.py
+-rw-r--r--   0 runner    (1001) docker     (123)      347 2023-07-09 17:31:22.000000 flet_lite-1.7.2/flet_core/canvas/shape.py
+-rw-r--r--   0 runner    (1001) docker     (123)     4172 2023-07-09 17:31:22.000000 flet_lite-1.7.2/flet_core/canvas/text.py
+-rw-r--r--   0 runner    (1001) docker     (123)     5695 2023-07-09 17:31:22.000000 flet_lite-1.7.2/flet_core/card.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-09 17:31:31.924562 flet_lite-1.7.2/flet_core/charts/
+-rw-r--r--   0 runner    (1001) docker     (123)        0 2023-07-09 17:31:22.000000 flet_lite-1.7.2/flet_core/charts/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)     9855 2023-07-09 17:31:22.000000 flet_lite-1.7.2/flet_core/charts/bar_chart.py
+-rw-r--r--   0 runner    (1001) docker     (123)     2061 2023-07-09 17:31:22.000000 flet_lite-1.7.2/flet_core/charts/bar_chart_group.py
+-rw-r--r--   0 runner    (1001) docker     (123)     6837 2023-07-09 17:31:22.000000 flet_lite-1.7.2/flet_core/charts/bar_chart_rod.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1949 2023-07-09 17:31:22.000000 flet_lite-1.7.2/flet_core/charts/bar_chart_rod_stack_item.py
+-rw-r--r--   0 runner    (1001) docker     (123)     2924 2023-07-09 17:31:22.000000 flet_lite-1.7.2/flet_core/charts/chart_axis.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1293 2023-07-09 17:31:22.000000 flet_lite-1.7.2/flet_core/charts/chart_axis_label.py
+-rw-r--r--   0 runner    (1001) docker     (123)      338 2023-07-09 17:31:22.000000 flet_lite-1.7.2/flet_core/charts/chart_grid_lines.py
+-rw-r--r--   0 runner    (1001) docker     (123)      286 2023-07-09 17:31:22.000000 flet_lite-1.7.2/flet_core/charts/chart_point_line.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1006 2023-07-09 17:31:22.000000 flet_lite-1.7.2/flet_core/charts/chart_point_shape.py
+-rw-r--r--   0 runner    (1001) docker     (123)    11228 2023-07-09 17:31:22.000000 flet_lite-1.7.2/flet_core/charts/line_chart.py
+-rw-r--r--   0 runner    (1001) docker     (123)     8258 2023-07-09 17:31:22.000000 flet_lite-1.7.2/flet_core/charts/line_chart_data.py
+-rw-r--r--   0 runner    (1001) docker     (123)     5496 2023-07-09 17:31:22.000000 flet_lite-1.7.2/flet_core/charts/line_chart_data_point.py
+-rw-r--r--   0 runner    (1001) docker     (123)     5888 2023-07-09 17:31:22.000000 flet_lite-1.7.2/flet_core/charts/pie_chart.py
+-rw-r--r--   0 runner    (1001) docker     (123)     3824 2023-07-09 17:31:22.000000 flet_lite-1.7.2/flet_core/charts/pie_chart_section.py
+-rw-r--r--   0 runner    (1001) docker     (123)     7156 2023-07-09 17:31:22.000000 flet_lite-1.7.2/flet_core/checkbox.py
+-rw-r--r--   0 runner    (1001) docker     (123)     6795 2023-07-09 17:31:22.000000 flet_lite-1.7.2/flet_core/circle_avatar.py
+-rw-r--r--   0 runner    (1001) docker     (123)     3085 2023-07-09 17:31:22.000000 flet_lite-1.7.2/flet_core/client_storage.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1002 2023-07-09 17:31:22.000000 flet_lite-1.7.2/flet_core/clipboard.py
+-rw-r--r--   0 runner    (1001) docker     (123)    10708 2023-07-09 17:31:22.000000 flet_lite-1.7.2/flet_core/colors.py
+-rw-r--r--   0 runner    (1001) docker     (123)     6924 2023-07-09 17:31:22.000000 flet_lite-1.7.2/flet_core/column.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1132 2023-07-09 17:31:22.000000 flet_lite-1.7.2/flet_core/connection.py
+-rw-r--r--   0 runner    (1001) docker     (123)     7099 2023-07-09 17:31:22.000000 flet_lite-1.7.2/flet_core/constrained_control.py
+-rw-r--r--   0 runner    (1001) docker     (123)    14684 2023-07-09 17:31:22.000000 flet_lite-1.7.2/flet_core/container.py
+-rw-r--r--   0 runner    (1001) docker     (123)    14133 2023-07-09 17:31:22.000000 flet_lite-1.7.2/flet_core/control.py
+-rw-r--r--   0 runner    (1001) docker     (123)      260 2023-07-09 17:31:22.000000 flet_lite-1.7.2/flet_core/control_event.py
+-rw-r--r--   0 runner    (1001) docker     (123)    20707 2023-07-09 17:31:22.000000 flet_lite-1.7.2/flet_core/datatable.py
+-rw-r--r--   0 runner    (1001) docker     (123)     2263 2023-07-09 17:31:22.000000 flet_lite-1.7.2/flet_core/divider.py
+-rw-r--r--   0 runner    (1001) docker     (123)     6270 2023-07-09 17:31:22.000000 flet_lite-1.7.2/flet_core/drag_target.py
+-rw-r--r--   0 runner    (1001) docker     (123)     6063 2023-07-09 17:31:22.000000 flet_lite-1.7.2/flet_core/draggable.py
+-rw-r--r--   0 runner    (1001) docker     (123)     9177 2023-07-09 17:31:22.000000 flet_lite-1.7.2/flet_core/dropdown.py
+-rw-r--r--   0 runner    (1001) docker     (123)     8804 2023-07-09 17:31:22.000000 flet_lite-1.7.2/flet_core/elevated_button.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1978 2023-07-09 17:31:22.000000 flet_lite-1.7.2/flet_core/embed_json_encoder.py
+-rw-r--r--   0 runner    (1001) docker     (123)      166 2023-07-09 17:31:22.000000 flet_lite-1.7.2/flet_core/event.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1839 2023-07-09 17:31:22.000000 flet_lite-1.7.2/flet_core/event_handler.py
+-rw-r--r--   0 runner    (1001) docker     (123)     9777 2023-07-09 17:31:22.000000 flet_lite-1.7.2/flet_core/file_picker.py
+-rw-r--r--   0 runner    (1001) docker     (123)     2694 2023-07-09 17:31:22.000000 flet_lite-1.7.2/flet_core/filled_button.py
+-rw-r--r--   0 runner    (1001) docker     (123)     2828 2023-07-09 17:31:22.000000 flet_lite-1.7.2/flet_core/filled_tonal_button.py
+-rw-r--r--   0 runner    (1001) docker     (123)     2542 2023-07-09 17:31:22.000000 flet_lite-1.7.2/flet_core/flet_app.py
+-rw-r--r--   0 runner    (1001) docker     (123)     7111 2023-07-09 17:31:22.000000 flet_lite-1.7.2/flet_core/floating_action_button.py
+-rw-r--r--   0 runner    (1001) docker     (123)    13981 2023-07-09 17:31:22.000000 flet_lite-1.7.2/flet_core/form_field_control.py
+-rw-r--r--   0 runner    (1001) docker     (123)    28044 2023-07-09 17:31:22.000000 flet_lite-1.7.2/flet_core/gesture_detector.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1531 2023-07-09 17:31:22.000000 flet_lite-1.7.2/flet_core/gradients.py
+-rw-r--r--   0 runner    (1001) docker     (123)     6804 2023-07-09 17:31:22.000000 flet_lite-1.7.2/flet_core/grid_view.py
+-rw-r--r--   0 runner    (1001) docker     (123)     2134 2023-07-09 17:31:22.000000 flet_lite-1.7.2/flet_core/haptic_feedback.py
+-rw-r--r--   0 runner    (1001) docker     (123)     3430 2023-07-09 17:31:22.000000 flet_lite-1.7.2/flet_core/icon.py
+-rw-r--r--   0 runner    (1001) docker     (123)     8438 2023-07-09 17:31:22.000000 flet_lite-1.7.2/flet_core/icon_button.py
+-rw-r--r--   0 runner    (1001) docker     (123)   362652 2023-07-09 17:31:22.000000 flet_lite-1.7.2/flet_core/icons.py
+-rw-r--r--   0 runner    (1001) docker     (123)     6585 2023-07-09 17:31:22.000000 flet_lite-1.7.2/flet_core/image.py
+-rw-r--r--   0 runner    (1001) docker     (123)      367 2023-07-09 17:31:22.000000 flet_lite-1.7.2/flet_core/inline_span.py
+-rw-r--r--   0 runner    (1001) docker     (123)     8360 2023-07-09 17:31:22.000000 flet_lite-1.7.2/flet_core/list_tile.py
+-rw-r--r--   0 runner    (1001) docker     (123)     6401 2023-07-09 17:31:22.000000 flet_lite-1.7.2/flet_core/list_view.py
+-rw-r--r--   0 runner    (1001) docker     (123)     8644 2023-07-09 17:31:22.000000 flet_lite-1.7.2/flet_core/local_connection.py
+-rw-r--r--   0 runner    (1001) docker     (123)      223 2023-07-09 17:31:22.000000 flet_lite-1.7.2/flet_core/locks.py
+-rw-r--r--   0 runner    (1001) docker     (123)      583 2023-07-09 17:31:22.000000 flet_lite-1.7.2/flet_core/margin.py
+-rw-r--r--   0 runner    (1001) docker     (123)     6129 2023-07-09 17:31:22.000000 flet_lite-1.7.2/flet_core/markdown.py
+-rw-r--r--   0 runner    (1001) docker     (123)     5180 2023-07-09 17:31:22.000000 flet_lite-1.7.2/flet_core/matplotlib_chart.py
+-rw-r--r--   0 runner    (1001) docker     (123)     8322 2023-07-09 17:31:22.000000 flet_lite-1.7.2/flet_core/navigation_bar.py
+-rw-r--r--   0 runner    (1001) docker     (123)    11986 2023-07-09 17:31:22.000000 flet_lite-1.7.2/flet_core/navigation_rail.py
+-rw-r--r--   0 runner    (1001) docker     (123)     7489 2023-07-09 17:31:22.000000 flet_lite-1.7.2/flet_core/outlined_button.py
+-rw-r--r--   0 runner    (1001) docker     (123)      587 2023-07-09 17:31:22.000000 flet_lite-1.7.2/flet_core/padding.py
+-rw-r--r--   0 runner    (1001) docker     (123)    53719 2023-07-09 17:31:22.000000 flet_lite-1.7.2/flet_core/page.py
+-rw-r--r--   0 runner    (1001) docker     (123)     2674 2023-07-09 17:31:22.000000 flet_lite-1.7.2/flet_core/painting.py
+-rw-r--r--   0 runner    (1001) docker     (123)     4410 2023-07-09 17:31:22.000000 flet_lite-1.7.2/flet_core/plotly_chart.py
+-rw-r--r--   0 runner    (1001) docker     (123)     6811 2023-07-09 17:31:22.000000 flet_lite-1.7.2/flet_core/popup_menu_button.py
+-rw-r--r--   0 runner    (1001) docker     (123)     4293 2023-07-09 17:31:22.000000 flet_lite-1.7.2/flet_core/progress_bar.py
+-rw-r--r--   0 runner    (1001) docker     (123)     4491 2023-07-09 17:31:22.000000 flet_lite-1.7.2/flet_core/progress_ring.py
+-rw-r--r--   0 runner    (1001) docker     (123)     4088 2023-07-09 17:31:22.000000 flet_lite-1.7.2/flet_core/protocol.py
+-rw-r--r--   0 runner    (1001) docker     (123)     3419 2023-07-09 17:31:22.000000 flet_lite-1.7.2/flet_core/querystring.py
+-rw-r--r--   0 runner    (1001) docker     (123)     5765 2023-07-09 17:31:22.000000 flet_lite-1.7.2/flet_core/radio.py
+-rw-r--r--   0 runner    (1001) docker     (123)     2389 2023-07-09 17:31:22.000000 flet_lite-1.7.2/flet_core/radio_group.py
+-rw-r--r--   0 runner    (1001) docker     (123)      291 2023-07-09 17:31:22.000000 flet_lite-1.7.2/flet_core/ref.py
+-rw-r--r--   0 runner    (1001) docker     (123)     6344 2023-07-09 17:31:22.000000 flet_lite-1.7.2/flet_core/responsive_row.py
+-rw-r--r--   0 runner    (1001) docker     (123)     6908 2023-07-09 17:31:22.000000 flet_lite-1.7.2/flet_core/row.py
+-rw-r--r--   0 runner    (1001) docker     (123)     4486 2023-07-09 17:31:22.000000 flet_lite-1.7.2/flet_core/scrollable_control.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1637 2023-07-09 17:31:22.000000 flet_lite-1.7.2/flet_core/semantics.py
+-rw-r--r--   0 runner    (1001) docker     (123)      576 2023-07-09 17:31:22.000000 flet_lite-1.7.2/flet_core/session_storage.py
+-rw-r--r--   0 runner    (1001) docker     (123)     5318 2023-07-09 17:31:22.000000 flet_lite-1.7.2/flet_core/shader_mask.py
+-rw-r--r--   0 runner    (1001) docker     (123)      572 2023-07-09 17:31:22.000000 flet_lite-1.7.2/flet_core/shadow.py
+-rw-r--r--   0 runner    (1001) docker     (123)     2919 2023-07-09 17:31:22.000000 flet_lite-1.7.2/flet_core/shake_detector.py
+-rw-r--r--   0 runner    (1001) docker     (123)     7382 2023-07-09 17:31:22.000000 flet_lite-1.7.2/flet_core/slider.py
+-rw-r--r--   0 runner    (1001) docker     (123)     3971 2023-07-09 17:31:22.000000 flet_lite-1.7.2/flet_core/snack_bar.py
+-rw-r--r--   0 runner    (1001) docker     (123)     4889 2023-07-09 17:31:22.000000 flet_lite-1.7.2/flet_core/stack.py
+-rw-r--r--   0 runner    (1001) docker     (123)     8104 2023-07-09 17:31:22.000000 flet_lite-1.7.2/flet_core/switch.py
+-rw-r--r--   0 runner    (1001) docker     (123)    10820 2023-07-09 17:31:22.000000 flet_lite-1.7.2/flet_core/tabs.py
+-rw-r--r--   0 runner    (1001) docker     (123)      632 2023-07-09 17:31:22.000000 flet_lite-1.7.2/flet_core/template_route.py
+-rw-r--r--   0 runner    (1001) docker     (123)    10568 2023-07-09 17:31:22.000000 flet_lite-1.7.2/flet_core/text.py
+-rw-r--r--   0 runner    (1001) docker     (123)     7462 2023-07-09 17:31:22.000000 flet_lite-1.7.2/flet_core/text_button.py
+-rw-r--r--   0 runner    (1001) docker     (123)     3092 2023-07-09 17:31:22.000000 flet_lite-1.7.2/flet_core/text_span.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1260 2023-07-09 17:31:22.000000 flet_lite-1.7.2/flet_core/text_style.py
+-rw-r--r--   0 runner    (1001) docker     (123)    15444 2023-07-09 17:31:22.000000 flet_lite-1.7.2/flet_core/textfield.py
+-rw-r--r--   0 runner    (1001) docker     (123)     6172 2023-07-09 17:31:22.000000 flet_lite-1.7.2/flet_core/theme.py
+-rw-r--r--   0 runner    (1001) docker     (123)     8362 2023-07-09 17:31:22.000000 flet_lite-1.7.2/flet_core/tooltip.py
+-rw-r--r--   0 runner    (1001) docker     (123)      544 2023-07-09 17:31:22.000000 flet_lite-1.7.2/flet_core/transform.py
+-rw-r--r--   0 runner    (1001) docker     (123)     2753 2023-07-09 17:31:22.000000 flet_lite-1.7.2/flet_core/transparent_pointer.py
+-rw-r--r--   0 runner    (1001) docker     (123)     5186 2023-07-09 17:31:22.000000 flet_lite-1.7.2/flet_core/types.py
+-rw-r--r--   0 runner    (1001) docker     (123)      684 2023-07-09 17:31:22.000000 flet_lite-1.7.2/flet_core/user_control.py
+-rw-r--r--   0 runner    (1001) docker     (123)      409 2023-07-09 17:31:22.000000 flet_lite-1.7.2/flet_core/utils.py
+-rw-r--r--   0 runner    (1001) docker     (123)     2337 2023-07-09 17:31:22.000000 flet_lite-1.7.2/flet_core/vertical_divider.py
+-rw-r--r--   0 runner    (1001) docker     (123)     5852 2023-07-09 17:31:22.000000 flet_lite-1.7.2/flet_core/view.py
+-rw-r--r--   0 runner    (1001) docker     (123)     4049 2023-07-09 17:31:22.000000 flet_lite-1.7.2/flet_core/window_drag_area.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-09 17:31:31.924562 flet_lite-1.7.2/flet_lite.egg-info/
+-rw-r--r--   0 runner    (1001) docker     (123)     3276 2023-07-09 17:31:31.000000 flet_lite-1.7.2/flet_lite.egg-info/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (123)     4673 2023-07-09 17:31:31.000000 flet_lite-1.7.2/flet_lite.egg-info/SOURCES.txt
+-rw-r--r--   0 runner    (1001) docker     (123)        1 2023-07-09 17:31:31.000000 flet_lite-1.7.2/flet_lite.egg-info/dependency_links.txt
+-rw-r--r--   0 runner    (1001) docker     (123)       35 2023-07-09 17:31:31.000000 flet_lite-1.7.2/flet_lite.egg-info/requires.txt
+-rw-r--r--   0 runner    (1001) docker     (123)       15 2023-07-09 17:31:31.000000 flet_lite-1.7.2/flet_lite.egg-info/top_level.txt
+-rw-r--r--   0 runner    (1001) docker     (123)      103 2023-07-09 17:31:22.000000 flet_lite-1.7.2/pyproject.toml
+-rw-r--r--   0 runner    (1001) docker     (123)       38 2023-07-09 17:31:31.924562 flet_lite-1.7.2/setup.cfg
+-rw-r--r--   0 runner    (1001) docker     (123)      834 2023-07-09 17:31:22.000000 flet_lite-1.7.2/setup.py
```

### Comparing `flet_lite-1.7/LICENSE` & `flet_lite-1.7.2/LICENSE`

 * *Files identical despite different names*

### Comparing `flet_lite-1.7/PKG-INFO` & `flet_lite-1.7.2/PKG-INFO`

 * *Files 0% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: flet_lite
-Version: 1.7
+Version: 1.7.2
 Summary: A tiny version of flet to work on mobile development
 Home-page: https://github.com/SKbarbon/flet_lite
 Author: SKbarbon
 Classifier: Programming Language :: Python :: 3
 Classifier: Operating System :: MacOS :: MacOS X
 Classifier: Operating System :: Microsoft :: Windows
 Description-Content-Type: text/markdown
```

### Comparing `flet_lite-1.7/README.md` & `flet_lite-1.7.2/README.md`

 * *Files identical despite different names*

### Comparing `flet_lite-1.7/flet/.DS_Store` & `flet_lite-1.7.2/flet/.DS_Store`

 * *Files identical despite different names*

### Comparing `flet_lite-1.7/flet/api/manage_client_pushes.py` & `flet_lite-1.7.2/flet/api/manage_client_pushes.py`

 * *Files identical despite different names*

### Comparing `flet_lite-1.7/flet/api/push_page_update_request.py` & `flet_lite-1.7.2/flet/api/push_page_update_request.py`

 * *Files identical despite different names*

### Comparing `flet_lite-1.7/flet/cli_tools/publish.py` & `flet_lite-1.7.2/flet/cli_tools/publish.py`

 * *Files identical despite different names*

### Comparing `flet_lite-1.7/flet/flet.py` & `flet_lite-1.7.2/flet/flet.py`

 * *Files 25% similar despite different names*

```diff
@@ -20,24 +20,28 @@
     port=0,
     view: AppViewer = FLET_APP,
     assets_dir=None,
     upload_dir=None,
     web_renderer="canvaskit",
     use_color_emoji=False,
     route_url_strategy="path",
-    auth_token=None,
-    debug=False
+    auth_token=None
     ):
     if view != FLET_APP:
         print("WARNING: flet-lite will always work on web_browser view mode.")
     
-    the_page = Page(target_function=target, assets_dir_path=assets_dir, debug=debug)
+    Page(target_function=target, assets_dir_path=assets_dir)
 
     # Define a signal handler function
     def signal_handler(signal, frame):
+        print("""
+Program is closed!
+Give the project a rate at github if you did like it: https://github.com/SKbarbon/flet_lite
+Create an issue if there is one: https://github.com/SKbarbon/flet_lite/issues
+""")
         sys.exit()
 
     # Set the signal handler for SIGINT (Ctrl+C)
     signal.signal(signal.SIGINT, signal_handler)
 
     # open a loop so the threads of the two hosts not closed.
     still_open = True
```

### Comparing `flet_lite-1.7/flet/page.py` & `flet_lite-1.7.2/flet/page.py`

 * *Files 6% similar despite different names*

```diff
@@ -6,22 +6,24 @@
 from .api.push_update_request import push_update_request
 from .api.push_remove_request import push_remove_request
 from .api.push_page_update_request import push_page_update_request
 from .api.push_clean_request import push_clean_request
 from .api.push_go_route_request import push_go_route_request
 from .utils.page_posible_props import all_page_posible_props
 from .utils.get_all_subcontrols import get_all_subControls_on_the_page
+from .tools.platform_specifics.get_platform_name import get_platform_name
+from .tools.platform_specifics.pythonista_webview import safari_in_app_view
 import threading
 import webbrowser
 import time, asyncio, traceback
 import flet
 
 
 class Page (object):
-    def __init__ (self, target_function, assets_dir_path:str, debug):
+    def __init__ (self, target_function, assets_dir_path:str):
         self.target_function = target_function
 
         # set all hosts without starting them.
         self.api_host = ApiHost(page=self)
         self.web_files_host = WebFilesHost()
         
         # Set the development web directory
@@ -30,20 +32,21 @@
         # Start the host API
         threading.Thread(target=self.api_host.host, daemon=True).start()
 
         # start the web development dir for browser
         threading.Thread(target=self.web_files_host.start, daemon=True).start()
 
         time.sleep(1)
-        if debug == False:
-            print(self.web_files_host.web_url)
-            webbrowser.open(self.web_files_host.web_url)
+
+        # start opening the localhost URL in the browser, or platform specific view.
+        print(self.web_files_host.web_url) #? print the URL of the app
+        if get_platform_name() == "pythonista":
+            safari_in_app_view(str(self.web_files_host.web_url))
         else:
-            open("localhost_api_url.txt", "w+", encoding="utf-8").write(self.api_host.url)
-        
+            webbrowser.open(self.web_files_host.web_url)
 
         # set all page props
         for i in all_page_posible_props:
             setattr(self, i, None)
         
         # page class's flet props
         self.appbar = None
```

### Comparing `flet_lite-1.7/flet/publish.py` & `flet_lite-1.7.2/flet/publish.py`

 * *Files identical despite different names*

### Comparing `flet_lite-1.7/flet/tools/append_assets_to_dist.py` & `flet_lite-1.7.2/flet/tools/append_assets_to_dist.py`

 * *Files identical despite different names*

### Comparing `flet_lite-1.7/flet/tools/run_event_function.py` & `flet_lite-1.7.2/flet/tools/run_event_function.py`

 * *Files identical despite different names*

### Comparing `flet_lite-1.7/flet/tools/setup_web.py` & `flet_lite-1.7.2/flet/tools/setup_web.py`

 * *Files identical despite different names*

### Comparing `flet_lite-1.7/flet/tools/update_control_on_event.py` & `flet_lite-1.7.2/flet/tools/update_control_on_event.py`

 * *Files identical despite different names*

### Comparing `flet_lite-1.7/flet/tools/update_page_info.py` & `flet_lite-1.7.2/flet/tools/update_page_info.py`

 * *Files identical despite different names*

### Comparing `flet_lite-1.7/flet/utils/all_props_posible.py` & `flet_lite-1.7.2/flet/utils/all_props_posible.py`

 * *Files identical despite different names*

### Comparing `flet_lite-1.7/flet/utils/api_host.py` & `flet_lite-1.7.2/flet/utils/api_host.py`

 * *Files identical despite different names*

### Comparing `flet_lite-1.7/flet/utils/appbar_coder.py` & `flet_lite-1.7.2/flet/utils/appbar_coder.py`

 * *Files identical despite different names*

### Comparing `flet_lite-1.7/flet/utils/control_coder.py` & `flet_lite-1.7.2/flet/utils/control_coder.py`

 * *Files identical despite different names*

### Comparing `flet_lite-1.7/flet/utils/get_all_subcontrols.py` & `flet_lite-1.7.2/flet/utils/get_all_subcontrols.py`

 * *Files identical despite different names*

### Comparing `flet_lite-1.7/flet/utils/get_control_data.py` & `flet_lite-1.7.2/flet/utils/get_control_data.py`

 * *Files identical despite different names*

### Comparing `flet_lite-1.7/flet/utils/page_posible_props.py` & `flet_lite-1.7.2/flet/utils/page_posible_props.py`

 * *Files identical despite different names*

### Comparing `flet_lite-1.7/flet/utils/view_coder.py` & `flet_lite-1.7.2/flet/utils/view_coder.py`

 * *Files identical despite different names*

### Comparing `flet_lite-1.7/flet/utils/web_host.py` & `flet_lite-1.7.2/flet/utils/web_host.py`

 * *Files identical despite different names*

### Comparing `flet_lite-1.7/flet/web/.DS_Store` & `flet_lite-1.7.2/flet/web/.DS_Store`

 * *Files identical despite different names*

### Comparing `flet_lite-1.7/flet/web/development.zip` & `flet_lite-1.7.2/flet/web/development.zip`

 * *Files identical despite different names*

### Comparing `flet_lite-1.7/flet/web/dist.zip` & `flet_lite-1.7.2/flet/web/dist.zip`

 * *Files identical despite different names*

### Comparing `flet_lite-1.7/flet_core/__init__.py` & `flet_lite-1.7.2/flet_core/__init__.py`

 * *Files identical despite different names*

### Comparing `flet_lite-1.7/flet_core/alert_dialog.py` & `flet_lite-1.7.2/flet_core/alert_dialog.py`

 * *Files identical despite different names*

### Comparing `flet_lite-1.7/flet_core/animated_switcher.py` & `flet_lite-1.7.2/flet_core/animated_switcher.py`

 * *Files identical despite different names*

### Comparing `flet_lite-1.7/flet_core/animation.py` & `flet_lite-1.7.2/flet_core/animation.py`

 * *Files identical despite different names*

### Comparing `flet_lite-1.7/flet_core/app_bar.py` & `flet_lite-1.7.2/flet_core/app_bar.py`

 * *Files identical despite different names*

### Comparing `flet_lite-1.7/flet_core/audio.py` & `flet_lite-1.7.2/flet_core/audio.py`

 * *Files identical despite different names*

### Comparing `flet_lite-1.7/flet_core/banner.py` & `flet_lite-1.7.2/flet_core/banner.py`

 * *Files identical despite different names*

### Comparing `flet_lite-1.7/flet_core/border.py` & `flet_lite-1.7.2/flet_core/border.py`

 * *Files identical despite different names*

### Comparing `flet_lite-1.7/flet_core/border_radius.py` & `flet_lite-1.7.2/flet_core/border_radius.py`

 * *Files identical despite different names*

### Comparing `flet_lite-1.7/flet_core/bottom_sheet.py` & `flet_lite-1.7.2/flet_core/bottom_sheet.py`

 * *Files identical despite different names*

### Comparing `flet_lite-1.7/flet_core/buttons.py` & `flet_lite-1.7.2/flet_core/buttons.py`

 * *Files identical despite different names*

### Comparing `flet_lite-1.7/flet_core/callable_control.py` & `flet_lite-1.7.2/flet_core/callable_control.py`

 * *Files identical despite different names*

### Comparing `flet_lite-1.7/flet_core/canvas/__init__.py` & `flet_lite-1.7.2/flet_core/canvas/__init__.py`

 * *Files identical despite different names*

### Comparing `flet_lite-1.7/flet_core/canvas/arc.py` & `flet_lite-1.7.2/flet_core/canvas/arc.py`

 * *Files identical despite different names*

### Comparing `flet_lite-1.7/flet_core/canvas/canvas.py` & `flet_lite-1.7.2/flet_core/canvas/canvas.py`

 * *Files identical despite different names*

### Comparing `flet_lite-1.7/flet_core/canvas/circle.py` & `flet_lite-1.7.2/flet_core/canvas/circle.py`

 * *Files identical despite different names*

### Comparing `flet_lite-1.7/flet_core/canvas/color.py` & `flet_lite-1.7.2/flet_core/canvas/color.py`

 * *Files identical despite different names*

### Comparing `flet_lite-1.7/flet_core/canvas/fill.py` & `flet_lite-1.7.2/flet_core/canvas/fill.py`

 * *Files identical despite different names*

### Comparing `flet_lite-1.7/flet_core/canvas/line.py` & `flet_lite-1.7.2/flet_core/canvas/line.py`

 * *Files identical despite different names*

### Comparing `flet_lite-1.7/flet_core/canvas/oval.py` & `flet_lite-1.7.2/flet_core/canvas/oval.py`

 * *Files identical despite different names*

### Comparing `flet_lite-1.7/flet_core/canvas/path.py` & `flet_lite-1.7.2/flet_core/canvas/path.py`

 * *Files identical despite different names*

### Comparing `flet_lite-1.7/flet_core/canvas/points.py` & `flet_lite-1.7.2/flet_core/canvas/points.py`

 * *Files identical despite different names*

### Comparing `flet_lite-1.7/flet_core/canvas/rect.py` & `flet_lite-1.7.2/flet_core/canvas/rect.py`

 * *Files identical despite different names*

### Comparing `flet_lite-1.7/flet_core/canvas/shadow.py` & `flet_lite-1.7.2/flet_core/canvas/shadow.py`

 * *Files identical despite different names*

### Comparing `flet_lite-1.7/flet_core/canvas/text.py` & `flet_lite-1.7.2/flet_core/canvas/text.py`

 * *Files identical despite different names*

### Comparing `flet_lite-1.7/flet_core/card.py` & `flet_lite-1.7.2/flet_core/card.py`

 * *Files identical despite different names*

### Comparing `flet_lite-1.7/flet_core/charts/bar_chart.py` & `flet_lite-1.7.2/flet_core/charts/bar_chart.py`

 * *Files identical despite different names*

### Comparing `flet_lite-1.7/flet_core/charts/bar_chart_group.py` & `flet_lite-1.7.2/flet_core/charts/bar_chart_group.py`

 * *Files identical despite different names*

### Comparing `flet_lite-1.7/flet_core/charts/bar_chart_rod.py` & `flet_lite-1.7.2/flet_core/charts/bar_chart_rod.py`

 * *Files identical despite different names*

### Comparing `flet_lite-1.7/flet_core/charts/bar_chart_rod_stack_item.py` & `flet_lite-1.7.2/flet_core/charts/bar_chart_rod_stack_item.py`

 * *Files identical despite different names*

### Comparing `flet_lite-1.7/flet_core/charts/chart_axis.py` & `flet_lite-1.7.2/flet_core/charts/chart_axis.py`

 * *Files identical despite different names*

### Comparing `flet_lite-1.7/flet_core/charts/chart_axis_label.py` & `flet_lite-1.7.2/flet_core/charts/chart_axis_label.py`

 * *Files identical despite different names*

### Comparing `flet_lite-1.7/flet_core/charts/chart_point_shape.py` & `flet_lite-1.7.2/flet_core/charts/chart_point_shape.py`

 * *Files identical despite different names*

### Comparing `flet_lite-1.7/flet_core/charts/line_chart.py` & `flet_lite-1.7.2/flet_core/charts/line_chart.py`

 * *Files identical despite different names*

### Comparing `flet_lite-1.7/flet_core/charts/line_chart_data.py` & `flet_lite-1.7.2/flet_core/charts/line_chart_data.py`

 * *Files identical despite different names*

### Comparing `flet_lite-1.7/flet_core/charts/line_chart_data_point.py` & `flet_lite-1.7.2/flet_core/charts/line_chart_data_point.py`

 * *Files identical despite different names*

### Comparing `flet_lite-1.7/flet_core/charts/pie_chart.py` & `flet_lite-1.7.2/flet_core/charts/pie_chart.py`

 * *Files identical despite different names*

### Comparing `flet_lite-1.7/flet_core/charts/pie_chart_section.py` & `flet_lite-1.7.2/flet_core/charts/pie_chart_section.py`

 * *Files identical despite different names*

### Comparing `flet_lite-1.7/flet_core/checkbox.py` & `flet_lite-1.7.2/flet_core/checkbox.py`

 * *Files identical despite different names*

### Comparing `flet_lite-1.7/flet_core/circle_avatar.py` & `flet_lite-1.7.2/flet_core/circle_avatar.py`

 * *Files identical despite different names*

### Comparing `flet_lite-1.7/flet_core/client_storage.py` & `flet_lite-1.7.2/flet_core/client_storage.py`

 * *Files identical despite different names*

### Comparing `flet_lite-1.7/flet_core/clipboard.py` & `flet_lite-1.7.2/flet_core/clipboard.py`

 * *Files identical despite different names*

### Comparing `flet_lite-1.7/flet_core/colors.py` & `flet_lite-1.7.2/flet_core/colors.py`

 * *Files identical despite different names*

### Comparing `flet_lite-1.7/flet_core/column.py` & `flet_lite-1.7.2/flet_core/column.py`

 * *Files identical despite different names*

### Comparing `flet_lite-1.7/flet_core/connection.py` & `flet_lite-1.7.2/flet_core/connection.py`

 * *Files identical despite different names*

### Comparing `flet_lite-1.7/flet_core/constrained_control.py` & `flet_lite-1.7.2/flet_core/constrained_control.py`

 * *Files identical despite different names*

### Comparing `flet_lite-1.7/flet_core/container.py` & `flet_lite-1.7.2/flet_core/container.py`

 * *Files identical despite different names*

### Comparing `flet_lite-1.7/flet_core/control.py` & `flet_lite-1.7.2/flet_core/control.py`

 * *Files identical despite different names*

### Comparing `flet_lite-1.7/flet_core/datatable.py` & `flet_lite-1.7.2/flet_core/datatable.py`

 * *Files identical despite different names*

### Comparing `flet_lite-1.7/flet_core/divider.py` & `flet_lite-1.7.2/flet_core/divider.py`

 * *Files identical despite different names*

### Comparing `flet_lite-1.7/flet_core/drag_target.py` & `flet_lite-1.7.2/flet_core/drag_target.py`

 * *Files identical despite different names*

### Comparing `flet_lite-1.7/flet_core/draggable.py` & `flet_lite-1.7.2/flet_core/draggable.py`

 * *Files identical despite different names*

### Comparing `flet_lite-1.7/flet_core/dropdown.py` & `flet_lite-1.7.2/flet_core/dropdown.py`

 * *Files identical despite different names*

### Comparing `flet_lite-1.7/flet_core/elevated_button.py` & `flet_lite-1.7.2/flet_core/elevated_button.py`

 * *Files identical despite different names*

### Comparing `flet_lite-1.7/flet_core/embed_json_encoder.py` & `flet_lite-1.7.2/flet_core/embed_json_encoder.py`

 * *Files identical despite different names*

### Comparing `flet_lite-1.7/flet_core/event_handler.py` & `flet_lite-1.7.2/flet_core/event_handler.py`

 * *Files identical despite different names*

### Comparing `flet_lite-1.7/flet_core/file_picker.py` & `flet_lite-1.7.2/flet_core/file_picker.py`

 * *Files identical despite different names*

### Comparing `flet_lite-1.7/flet_core/filled_button.py` & `flet_lite-1.7.2/flet_core/filled_button.py`

 * *Files identical despite different names*

### Comparing `flet_lite-1.7/flet_core/filled_tonal_button.py` & `flet_lite-1.7.2/flet_core/filled_tonal_button.py`

 * *Files identical despite different names*

### Comparing `flet_lite-1.7/flet_core/flet_app.py` & `flet_lite-1.7.2/flet_core/flet_app.py`

 * *Files identical despite different names*

### Comparing `flet_lite-1.7/flet_core/floating_action_button.py` & `flet_lite-1.7.2/flet_core/floating_action_button.py`

 * *Files identical despite different names*

### Comparing `flet_lite-1.7/flet_core/form_field_control.py` & `flet_lite-1.7.2/flet_core/form_field_control.py`

 * *Files identical despite different names*

### Comparing `flet_lite-1.7/flet_core/gesture_detector.py` & `flet_lite-1.7.2/flet_core/gesture_detector.py`

 * *Files identical despite different names*

### Comparing `flet_lite-1.7/flet_core/gradients.py` & `flet_lite-1.7.2/flet_core/gradients.py`

 * *Files identical despite different names*

### Comparing `flet_lite-1.7/flet_core/grid_view.py` & `flet_lite-1.7.2/flet_core/grid_view.py`

 * *Files identical despite different names*

### Comparing `flet_lite-1.7/flet_core/haptic_feedback.py` & `flet_lite-1.7.2/flet_core/haptic_feedback.py`

 * *Files identical despite different names*

### Comparing `flet_lite-1.7/flet_core/icon.py` & `flet_lite-1.7.2/flet_core/icon.py`

 * *Files identical despite different names*

### Comparing `flet_lite-1.7/flet_core/icon_button.py` & `flet_lite-1.7.2/flet_core/icon_button.py`

 * *Files identical despite different names*

### Comparing `flet_lite-1.7/flet_core/icons.py` & `flet_lite-1.7.2/flet_core/icons.py`

 * *Files identical despite different names*

### Comparing `flet_lite-1.7/flet_core/image.py` & `flet_lite-1.7.2/flet_core/image.py`

 * *Files identical despite different names*

### Comparing `flet_lite-1.7/flet_core/list_tile.py` & `flet_lite-1.7.2/flet_core/list_tile.py`

 * *Files identical despite different names*

### Comparing `flet_lite-1.7/flet_core/list_view.py` & `flet_lite-1.7.2/flet_core/list_view.py`

 * *Files identical despite different names*

### Comparing `flet_lite-1.7/flet_core/local_connection.py` & `flet_lite-1.7.2/flet_core/local_connection.py`

 * *Files identical despite different names*

### Comparing `flet_lite-1.7/flet_core/margin.py` & `flet_lite-1.7.2/flet_core/margin.py`

 * *Files identical despite different names*

### Comparing `flet_lite-1.7/flet_core/markdown.py` & `flet_lite-1.7.2/flet_core/markdown.py`

 * *Files identical despite different names*

### Comparing `flet_lite-1.7/flet_core/matplotlib_chart.py` & `flet_lite-1.7.2/flet_core/matplotlib_chart.py`

 * *Files identical despite different names*

### Comparing `flet_lite-1.7/flet_core/navigation_bar.py` & `flet_lite-1.7.2/flet_core/navigation_bar.py`

 * *Files identical despite different names*

### Comparing `flet_lite-1.7/flet_core/navigation_rail.py` & `flet_lite-1.7.2/flet_core/navigation_rail.py`

 * *Files identical despite different names*

### Comparing `flet_lite-1.7/flet_core/outlined_button.py` & `flet_lite-1.7.2/flet_core/outlined_button.py`

 * *Files identical despite different names*

### Comparing `flet_lite-1.7/flet_core/padding.py` & `flet_lite-1.7.2/flet_core/padding.py`

 * *Files identical despite different names*

### Comparing `flet_lite-1.7/flet_core/page.py` & `flet_lite-1.7.2/flet_core/page.py`

 * *Files identical despite different names*

### Comparing `flet_lite-1.7/flet_core/painting.py` & `flet_lite-1.7.2/flet_core/painting.py`

 * *Files identical despite different names*

### Comparing `flet_lite-1.7/flet_core/plotly_chart.py` & `flet_lite-1.7.2/flet_core/plotly_chart.py`

 * *Files identical despite different names*

### Comparing `flet_lite-1.7/flet_core/popup_menu_button.py` & `flet_lite-1.7.2/flet_core/popup_menu_button.py`

 * *Files identical despite different names*

### Comparing `flet_lite-1.7/flet_core/progress_bar.py` & `flet_lite-1.7.2/flet_core/progress_bar.py`

 * *Files identical despite different names*

### Comparing `flet_lite-1.7/flet_core/progress_ring.py` & `flet_lite-1.7.2/flet_core/progress_ring.py`

 * *Files identical despite different names*

### Comparing `flet_lite-1.7/flet_core/protocol.py` & `flet_lite-1.7.2/flet_core/protocol.py`

 * *Files identical despite different names*

### Comparing `flet_lite-1.7/flet_core/querystring.py` & `flet_lite-1.7.2/flet_core/querystring.py`

 * *Files identical despite different names*

### Comparing `flet_lite-1.7/flet_core/radio.py` & `flet_lite-1.7.2/flet_core/radio.py`

 * *Files identical despite different names*

### Comparing `flet_lite-1.7/flet_core/radio_group.py` & `flet_lite-1.7.2/flet_core/radio_group.py`

 * *Files identical despite different names*

### Comparing `flet_lite-1.7/flet_core/responsive_row.py` & `flet_lite-1.7.2/flet_core/responsive_row.py`

 * *Files identical despite different names*

### Comparing `flet_lite-1.7/flet_core/row.py` & `flet_lite-1.7.2/flet_core/row.py`

 * *Files identical despite different names*

### Comparing `flet_lite-1.7/flet_core/scrollable_control.py` & `flet_lite-1.7.2/flet_core/scrollable_control.py`

 * *Files identical despite different names*

### Comparing `flet_lite-1.7/flet_core/semantics.py` & `flet_lite-1.7.2/flet_core/semantics.py`

 * *Files identical despite different names*

### Comparing `flet_lite-1.7/flet_core/session_storage.py` & `flet_lite-1.7.2/flet_core/session_storage.py`

 * *Files identical despite different names*

### Comparing `flet_lite-1.7/flet_core/shader_mask.py` & `flet_lite-1.7.2/flet_core/shader_mask.py`

 * *Files identical despite different names*

### Comparing `flet_lite-1.7/flet_core/shadow.py` & `flet_lite-1.7.2/flet_core/shadow.py`

 * *Files identical despite different names*

### Comparing `flet_lite-1.7/flet_core/shake_detector.py` & `flet_lite-1.7.2/flet_core/shake_detector.py`

 * *Files identical despite different names*

### Comparing `flet_lite-1.7/flet_core/slider.py` & `flet_lite-1.7.2/flet_core/slider.py`

 * *Files identical despite different names*

### Comparing `flet_lite-1.7/flet_core/snack_bar.py` & `flet_lite-1.7.2/flet_core/snack_bar.py`

 * *Files identical despite different names*

### Comparing `flet_lite-1.7/flet_core/stack.py` & `flet_lite-1.7.2/flet_core/stack.py`

 * *Files identical despite different names*

### Comparing `flet_lite-1.7/flet_core/switch.py` & `flet_lite-1.7.2/flet_core/switch.py`

 * *Files identical despite different names*

### Comparing `flet_lite-1.7/flet_core/tabs.py` & `flet_lite-1.7.2/flet_core/tabs.py`

 * *Files identical despite different names*

### Comparing `flet_lite-1.7/flet_core/template_route.py` & `flet_lite-1.7.2/flet_core/template_route.py`

 * *Files identical despite different names*

### Comparing `flet_lite-1.7/flet_core/text.py` & `flet_lite-1.7.2/flet_core/text.py`

 * *Files identical despite different names*

### Comparing `flet_lite-1.7/flet_core/text_button.py` & `flet_lite-1.7.2/flet_core/text_button.py`

 * *Files identical despite different names*

### Comparing `flet_lite-1.7/flet_core/text_span.py` & `flet_lite-1.7.2/flet_core/text_span.py`

 * *Files identical despite different names*

### Comparing `flet_lite-1.7/flet_core/text_style.py` & `flet_lite-1.7.2/flet_core/text_style.py`

 * *Files identical despite different names*

### Comparing `flet_lite-1.7/flet_core/textfield.py` & `flet_lite-1.7.2/flet_core/textfield.py`

 * *Files identical despite different names*

### Comparing `flet_lite-1.7/flet_core/theme.py` & `flet_lite-1.7.2/flet_core/theme.py`

 * *Files identical despite different names*

### Comparing `flet_lite-1.7/flet_core/tooltip.py` & `flet_lite-1.7.2/flet_core/tooltip.py`

 * *Files identical despite different names*

### Comparing `flet_lite-1.7/flet_core/transform.py` & `flet_lite-1.7.2/flet_core/transform.py`

 * *Files identical despite different names*

### Comparing `flet_lite-1.7/flet_core/transparent_pointer.py` & `flet_lite-1.7.2/flet_core/transparent_pointer.py`

 * *Files identical despite different names*

### Comparing `flet_lite-1.7/flet_core/types.py` & `flet_lite-1.7.2/flet_core/types.py`

 * *Files identical despite different names*

### Comparing `flet_lite-1.7/flet_core/user_control.py` & `flet_lite-1.7.2/flet_core/user_control.py`

 * *Files identical despite different names*

### Comparing `flet_lite-1.7/flet_core/vertical_divider.py` & `flet_lite-1.7.2/flet_core/vertical_divider.py`

 * *Files identical despite different names*

### Comparing `flet_lite-1.7/flet_core/view.py` & `flet_lite-1.7.2/flet_core/view.py`

 * *Files identical despite different names*

### Comparing `flet_lite-1.7/flet_core/window_drag_area.py` & `flet_lite-1.7.2/flet_core/window_drag_area.py`

 * *Files identical despite different names*

### Comparing `flet_lite-1.7/flet_lite.egg-info/PKG-INFO` & `flet_lite-1.7.2/flet_lite.egg-info/PKG-INFO`

 * *Files 0% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: flet-lite
-Version: 1.7
+Version: 1.7.2
 Summary: A tiny version of flet to work on mobile development
 Home-page: https://github.com/SKbarbon/flet_lite
 Author: SKbarbon
 Classifier: Programming Language :: Python :: 3
 Classifier: Operating System :: MacOS :: MacOS X
 Classifier: Operating System :: Microsoft :: Windows
 Description-Content-Type: text/markdown
```

### Comparing `flet_lite-1.7/flet_lite.egg-info/SOURCES.txt` & `flet_lite-1.7.2/flet_lite.egg-info/SOURCES.txt`

 * *Files 11% similar despite different names*

```diff
@@ -21,14 +21,17 @@
 flet/tools/__init__.py
 flet/tools/append_assets_to_dist.py
 flet/tools/edit_control_props.py
 flet/tools/run_event_function.py
 flet/tools/setup_web.py
 flet/tools/update_control_on_event.py
 flet/tools/update_page_info.py
+flet/tools/platform_specifics/__init__.py
+flet/tools/platform_specifics/get_platform_name.py
+flet/tools/platform_specifics/pythonista_webview.py
 flet/utils/__init__.py
 flet/utils/all_props_posible.py
 flet/utils/api_host.py
 flet/utils/appbar_coder.py
 flet/utils/control_coder.py
 flet/utils/get_all_subcontrols.py
 flet/utils/get_control_data.py
```

### Comparing `flet_lite-1.7/setup.py` & `flet_lite-1.7.2/setup.py`

 * *Files 11% similar despite different names*

```diff
@@ -2,15 +2,15 @@
 import os
 
 with open("README.md", encoding="utf-8") as f:
     long_descibe = str(f.read())
 
 setup(
     name='flet_lite',
-    version='1.7',
+    version='1.7.2',
     author='SKbarbon',
     description='A tiny version of flet to work on mobile development',
     long_description=long_descibe,
     long_description_content_type='text/markdown',
     url='https://github.com/SKbarbon/flet_lite',
     install_requires=["flask_cors", "flask", "jsonpickle", "repath"],
     packages=find_packages(include=["flet", "flet_core", "flet.web", "flet/*", "flet.api"]),
```

