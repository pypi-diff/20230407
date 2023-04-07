# Comparing `tmp/custom-streamlit-1.19.0.tar.gz` & `tmp/custom-streamlit-1.20.0.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "custom-streamlit-1.19.0.tar", last modified: Wed Mar  8 13:56:50 2023, max compression
+gzip compressed data, was "custom-streamlit-1.20.0.tar", last modified: Fri Apr  7 18:36:01 2023, max compression
```

## Comparing `custom-streamlit-1.19.0.tar` & `custom-streamlit-1.20.0.tar`

### file list

```diff
@@ -1,279 +1,279 @@
-drwxrwxr-x   0 dorka     (1000) dorka     (1000)        0 2023-03-08 13:56:50.058631 custom-streamlit-1.19.0/
--rw-rw-r--   0 dorka     (1000) dorka     (1000)      116 2023-03-07 14:32:33.000000 custom-streamlit-1.19.0/MANIFEST.in
--rw-rw-r--   0 dorka     (1000) dorka     (1000)     6417 2023-03-08 13:56:50.058631 custom-streamlit-1.19.0/PKG-INFO
--rw-rw-r--   0 dorka     (1000) dorka     (1000)     1748 2023-03-07 14:32:33.000000 custom-streamlit-1.19.0/Pipfile
-drwxrwxr-x   0 dorka     (1000) dorka     (1000)        0 2023-03-08 13:56:49.954589 custom-streamlit-1.19.0/bin/
--rw-rw-r--   0 dorka     (1000) dorka     (1000)      671 2023-03-07 14:32:33.000000 custom-streamlit-1.19.0/bin/streamlit.cmd
-drwxrwxr-x   0 dorka     (1000) dorka     (1000)        0 2023-03-08 13:56:49.958591 custom-streamlit-1.19.0/custom_streamlit.egg-info/
--rw-rw-r--   0 dorka     (1000) dorka     (1000)     6417 2023-03-08 13:56:49.000000 custom-streamlit-1.19.0/custom_streamlit.egg-info/PKG-INFO
--rw-rw-r--   0 dorka     (1000) dorka     (1000)     8542 2023-03-08 13:56:49.000000 custom-streamlit-1.19.0/custom_streamlit.egg-info/SOURCES.txt
--rw-rw-r--   0 dorka     (1000) dorka     (1000)        1 2023-03-08 13:56:49.000000 custom-streamlit-1.19.0/custom_streamlit.egg-info/dependency_links.txt
--rw-rw-r--   0 dorka     (1000) dorka     (1000)       53 2023-03-08 13:56:49.000000 custom-streamlit-1.19.0/custom_streamlit.egg-info/entry_points.txt
--rw-rw-r--   0 dorka     (1000) dorka     (1000)        1 2023-03-08 13:55:57.000000 custom-streamlit-1.19.0/custom_streamlit.egg-info/not-zip-safe
--rw-rw-r--   0 dorka     (1000) dorka     (1000)      456 2023-03-08 13:56:49.000000 custom-streamlit-1.19.0/custom_streamlit.egg-info/requires.txt
--rw-rw-r--   0 dorka     (1000) dorka     (1000)       10 2023-03-08 13:56:49.000000 custom-streamlit-1.19.0/custom_streamlit.egg-info/top_level.txt
--rw-rw-r--   0 dorka     (1000) dorka     (1000)       38 2023-03-08 13:56:50.058631 custom-streamlit-1.19.0/setup.cfg
--rw-rw-r--   0 dorka     (1000) dorka     (1000)     6011 2023-03-08 13:55:45.000000 custom-streamlit-1.19.0/setup.py
-drwxrwxr-x   0 dorka     (1000) dorka     (1000)        0 2023-03-08 13:56:49.970595 custom-streamlit-1.19.0/streamlit/
--rw-rw-r--   0 dorka     (1000) dorka     (1000)     6768 2023-03-07 14:32:33.000000 custom-streamlit-1.19.0/streamlit/__init__.py
--rw-rw-r--   0 dorka     (1000) dorka     (1000)      863 2023-03-07 14:32:33.000000 custom-streamlit-1.19.0/streamlit/__main__.py
--rw-rw-r--   0 dorka     (1000) dorka     (1000)     2296 2023-03-07 14:32:33.000000 custom-streamlit-1.19.0/streamlit/case_converters.py
--rw-rw-r--   0 dorka     (1000) dorka     (1000)     2284 2023-03-07 14:32:33.000000 custom-streamlit-1.19.0/streamlit/code_util.py
-drwxrwxr-x   0 dorka     (1000) dorka     (1000)        0 2023-03-08 13:56:49.970595 custom-streamlit-1.19.0/streamlit/commands/
--rw-rw-r--   0 dorka     (1000) dorka     (1000)      611 2023-03-07 14:32:33.000000 custom-streamlit-1.19.0/streamlit/commands/__init__.py
--rw-rw-r--   0 dorka     (1000) dorka     (1000)     1970 2023-03-07 14:32:33.000000 custom-streamlit-1.19.0/streamlit/commands/execution_control.py
--rw-rw-r--   0 dorka     (1000) dorka     (1000)    11977 2023-03-07 14:32:33.000000 custom-streamlit-1.19.0/streamlit/commands/page_config.py
--rw-rw-r--   0 dorka     (1000) dorka     (1000)     4830 2023-03-07 14:32:33.000000 custom-streamlit-1.19.0/streamlit/commands/query_params.py
-drwxrwxr-x   0 dorka     (1000) dorka     (1000)        0 2023-03-08 13:56:49.970595 custom-streamlit-1.19.0/streamlit/components/
--rw-rw-r--   0 dorka     (1000) dorka     (1000)      611 2023-03-07 14:32:33.000000 custom-streamlit-1.19.0/streamlit/components/__init__.py
-drwxrwxr-x   0 dorka     (1000) dorka     (1000)        0 2023-03-08 13:56:49.974597 custom-streamlit-1.19.0/streamlit/components/v1/
--rw-rw-r--   0 dorka     (1000) dorka     (1000)     1031 2023-03-07 14:32:33.000000 custom-streamlit-1.19.0/streamlit/components/v1/__init__.py
--rw-rw-r--   0 dorka     (1000) dorka     (1000)    10898 2023-03-07 14:32:33.000000 custom-streamlit-1.19.0/streamlit/components/v1/component_arrow.py
--rw-rw-r--   0 dorka     (1000) dorka     (1000)    12966 2023-03-07 14:32:33.000000 custom-streamlit-1.19.0/streamlit/components/v1/components.py
--rw-rw-r--   0 dorka     (1000) dorka     (1000)    37021 2023-03-07 14:32:33.000000 custom-streamlit-1.19.0/streamlit/config.py
--rw-rw-r--   0 dorka     (1000) dorka     (1000)    10753 2023-03-07 14:32:33.000000 custom-streamlit-1.19.0/streamlit/config_option.py
--rw-rw-r--   0 dorka     (1000) dorka     (1000)     4515 2023-03-07 14:32:33.000000 custom-streamlit-1.19.0/streamlit/config_util.py
--rw-rw-r--   0 dorka     (1000) dorka     (1000)     5997 2023-03-07 14:32:33.000000 custom-streamlit-1.19.0/streamlit/cursor.py
--rw-rw-r--   0 dorka     (1000) dorka     (1000)    35516 2023-03-07 14:32:33.000000 custom-streamlit-1.19.0/streamlit/delta_generator.py
--rw-rw-r--   0 dorka     (1000) dorka     (1000)     5651 2023-03-07 14:32:33.000000 custom-streamlit-1.19.0/streamlit/deprecation_util.py
--rw-rw-r--   0 dorka     (1000) dorka     (1000)      808 2023-03-07 14:32:33.000000 custom-streamlit-1.19.0/streamlit/development.py
--rw-rw-r--   0 dorka     (1000) dorka     (1000)     3955 2023-03-07 14:32:33.000000 custom-streamlit-1.19.0/streamlit/echo.py
-drwxrwxr-x   0 dorka     (1000) dorka     (1000)        0 2023-03-08 13:56:49.998607 custom-streamlit-1.19.0/streamlit/elements/
--rw-rw-r--   0 dorka     (1000) dorka     (1000)     1664 2023-03-07 14:32:33.000000 custom-streamlit-1.19.0/streamlit/elements/__init__.py
--rw-rw-r--   0 dorka     (1000) dorka     (1000)     5620 2023-03-07 14:32:33.000000 custom-streamlit-1.19.0/streamlit/elements/alert.py
--rw-rw-r--   0 dorka     (1000) dorka     (1000)    14078 2023-03-07 14:32:33.000000 custom-streamlit-1.19.0/streamlit/elements/arrow.py
--rw-rw-r--   0 dorka     (1000) dorka     (1000)    21671 2023-03-07 14:33:59.000000 custom-streamlit-1.19.0/streamlit/elements/arrow_altair.py
--rw-rw-r--   0 dorka     (1000) dorka     (1000)     7196 2023-03-07 14:32:33.000000 custom-streamlit-1.19.0/streamlit/elements/arrow_vega_lite.py
--rw-rw-r--   0 dorka     (1000) dorka     (1000)     1445 2023-03-07 14:32:33.000000 custom-streamlit-1.19.0/streamlit/elements/balloons.py
--rw-rw-r--   0 dorka     (1000) dorka     (1000)     3856 2023-03-07 14:32:33.000000 custom-streamlit-1.19.0/streamlit/elements/bokeh_chart.py
--rw-rw-r--   0 dorka     (1000) dorka     (1000)    16910 2023-03-07 14:32:33.000000 custom-streamlit-1.19.0/streamlit/elements/button.py
--rw-rw-r--   0 dorka     (1000) dorka     (1000)    10040 2023-03-07 14:32:33.000000 custom-streamlit-1.19.0/streamlit/elements/camera_input.py
--rw-rw-r--   0 dorka     (1000) dorka     (1000)     6798 2023-03-07 14:32:33.000000 custom-streamlit-1.19.0/streamlit/elements/checkbox.py
--rw-rw-r--   0 dorka     (1000) dorka     (1000)     2452 2023-03-07 14:32:33.000000 custom-streamlit-1.19.0/streamlit/elements/code.py
--rw-rw-r--   0 dorka     (1000) dorka     (1000)     8606 2023-03-07 14:32:33.000000 custom-streamlit-1.19.0/streamlit/elements/color_picker.py
--rw-rw-r--   0 dorka     (1000) dorka     (1000)    22373 2023-03-07 14:32:33.000000 custom-streamlit-1.19.0/streamlit/elements/data_editor.py
--rw-rw-r--   0 dorka     (1000) dorka     (1000)    23378 2023-03-07 14:32:33.000000 custom-streamlit-1.19.0/streamlit/elements/dataframe_selector.py
--rw-rw-r--   0 dorka     (1000) dorka     (1000)     5900 2023-03-07 14:32:33.000000 custom-streamlit-1.19.0/streamlit/elements/deck_gl_json_chart.py
--rw-rw-r--   0 dorka     (1000) dorka     (1000)     4443 2023-03-07 14:32:33.000000 custom-streamlit-1.19.0/streamlit/elements/doc_string.py
--rw-rw-r--   0 dorka     (1000) dorka     (1000)     2598 2023-03-07 14:32:33.000000 custom-streamlit-1.19.0/streamlit/elements/empty.py
--rw-rw-r--   0 dorka     (1000) dorka     (1000)     9131 2023-03-07 14:32:33.000000 custom-streamlit-1.19.0/streamlit/elements/exception.py
--rw-rw-r--   0 dorka     (1000) dorka     (1000)    16905 2023-03-07 14:32:33.000000 custom-streamlit-1.19.0/streamlit/elements/file_uploader.py
--rw-rw-r--   0 dorka     (1000) dorka     (1000)    11437 2023-03-07 14:32:33.000000 custom-streamlit-1.19.0/streamlit/elements/form.py
--rw-rw-r--   0 dorka     (1000) dorka     (1000)     4461 2023-03-07 14:32:33.000000 custom-streamlit-1.19.0/streamlit/elements/graphviz_chart.py
--rw-rw-r--   0 dorka     (1000) dorka     (1000)     6351 2023-03-07 14:32:33.000000 custom-streamlit-1.19.0/streamlit/elements/heading.py
--rw-rw-r--   0 dorka     (1000) dorka     (1000)     4382 2023-03-07 14:32:33.000000 custom-streamlit-1.19.0/streamlit/elements/iframe.py
--rw-rw-r--   0 dorka     (1000) dorka     (1000)    19520 2023-03-07 14:32:33.000000 custom-streamlit-1.19.0/streamlit/elements/image.py
--rw-rw-r--   0 dorka     (1000) dorka     (1000)     3373 2023-03-07 14:32:33.000000 custom-streamlit-1.19.0/streamlit/elements/json.py
--rw-rw-r--   0 dorka     (1000) dorka     (1000)    14350 2023-03-07 14:32:33.000000 custom-streamlit-1.19.0/streamlit/elements/layouts.py
--rw-rw-r--   0 dorka     (1000) dorka     (1000)    13220 2023-03-07 14:32:33.000000 custom-streamlit-1.19.0/streamlit/elements/legacy_altair.py
--rw-rw-r--   0 dorka     (1000) dorka     (1000)    17493 2023-03-07 14:32:33.000000 custom-streamlit-1.19.0/streamlit/elements/legacy_data_frame.py
--rw-rw-r--   0 dorka     (1000) dorka     (1000)     6649 2023-03-07 14:32:33.000000 custom-streamlit-1.19.0/streamlit/elements/legacy_vega_lite.py
-drwxrwxr-x   0 dorka     (1000) dorka     (1000)        0 2023-03-08 13:56:49.998607 custom-streamlit-1.19.0/streamlit/elements/lib/
--rw-rw-r--   0 dorka     (1000) dorka     (1000)      611 2023-03-07 14:32:33.000000 custom-streamlit-1.19.0/streamlit/elements/lib/__init__.py
--rw-rw-r--   0 dorka     (1000) dorka     (1000)     3370 2023-03-07 14:32:33.000000 custom-streamlit-1.19.0/streamlit/elements/lib/dicttools.py
--rw-rw-r--   0 dorka     (1000) dorka     (1000)     6407 2023-03-07 14:32:33.000000 custom-streamlit-1.19.0/streamlit/elements/lib/streamlit_plotly_theme.py
--rw-rw-r--   0 dorka     (1000) dorka     (1000)     7968 2023-03-07 14:32:33.000000 custom-streamlit-1.19.0/streamlit/elements/map.py
--rw-rw-r--   0 dorka     (1000) dorka     (1000)     6773 2023-03-07 14:32:33.000000 custom-streamlit-1.19.0/streamlit/elements/markdown.py
--rw-rw-r--   0 dorka     (1000) dorka     (1000)    14695 2023-03-07 14:32:33.000000 custom-streamlit-1.19.0/streamlit/elements/media.py
--rw-rw-r--   0 dorka     (1000) dorka     (1000)     9846 2023-03-07 14:32:33.000000 custom-streamlit-1.19.0/streamlit/elements/metric.py
--rw-rw-r--   0 dorka     (1000) dorka     (1000)    12382 2023-03-07 14:32:33.000000 custom-streamlit-1.19.0/streamlit/elements/multiselect.py
--rw-rw-r--   0 dorka     (1000) dorka     (1000)    14312 2023-03-07 14:32:33.000000 custom-streamlit-1.19.0/streamlit/elements/number_input.py
--rw-rw-r--   0 dorka     (1000) dorka     (1000)     8822 2023-03-07 14:32:33.000000 custom-streamlit-1.19.0/streamlit/elements/plotly_chart.py
--rw-rw-r--   0 dorka     (1000) dorka     (1000)     4450 2023-03-07 14:32:33.000000 custom-streamlit-1.19.0/streamlit/elements/progress.py
--rw-rw-r--   0 dorka     (1000) dorka     (1000)     6123 2023-03-07 14:32:33.000000 custom-streamlit-1.19.0/streamlit/elements/pyplot.py
--rw-rw-r--   0 dorka     (1000) dorka     (1000)     9810 2023-03-07 14:32:33.000000 custom-streamlit-1.19.0/streamlit/elements/radio.py
--rw-rw-r--   0 dorka     (1000) dorka     (1000)    12352 2023-03-07 14:32:33.000000 custom-streamlit-1.19.0/streamlit/elements/select_slider.py
--rw-rw-r--   0 dorka     (1000) dorka     (1000)     9286 2023-03-07 14:32:33.000000 custom-streamlit-1.19.0/streamlit/elements/selectbox.py
--rw-rw-r--   0 dorka     (1000) dorka     (1000)     3546 2023-03-07 14:32:33.000000 custom-streamlit-1.19.0/streamlit/elements/show.py
--rw-rw-r--   0 dorka     (1000) dorka     (1000)    24739 2023-03-07 14:32:33.000000 custom-streamlit-1.19.0/streamlit/elements/slider.py
--rw-rw-r--   0 dorka     (1000) dorka     (1000)     1402 2023-03-07 14:32:33.000000 custom-streamlit-1.19.0/streamlit/elements/snow.py
--rw-rw-r--   0 dorka     (1000) dorka     (1000)     3076 2023-03-07 14:32:33.000000 custom-streamlit-1.19.0/streamlit/elements/spinner.py
--rw-rw-r--   0 dorka     (1000) dorka     (1000)     1585 2023-03-07 14:32:33.000000 custom-streamlit-1.19.0/streamlit/elements/text.py
--rw-rw-r--   0 dorka     (1000) dorka     (1000)    17557 2023-03-07 14:32:33.000000 custom-streamlit-1.19.0/streamlit/elements/text_widgets.py
--rw-rw-r--   0 dorka     (1000) dorka     (1000)    21020 2023-03-07 14:32:33.000000 custom-streamlit-1.19.0/streamlit/elements/time_widgets.py
--rw-rw-r--   0 dorka     (1000) dorka     (1000)     3379 2023-03-07 14:32:33.000000 custom-streamlit-1.19.0/streamlit/elements/utils.py
--rw-rw-r--   0 dorka     (1000) dorka     (1000)     9573 2023-03-07 14:32:33.000000 custom-streamlit-1.19.0/streamlit/elements/write.py
--rw-rw-r--   0 dorka     (1000) dorka     (1000)    68199 2023-03-07 14:32:33.000000 custom-streamlit-1.19.0/streamlit/emojis.py
--rw-rw-r--   0 dorka     (1000) dorka     (1000)     1750 2023-03-07 14:32:33.000000 custom-streamlit-1.19.0/streamlit/env_util.py
--rw-rw-r--   0 dorka     (1000) dorka     (1000)     3539 2023-03-07 14:32:33.000000 custom-streamlit-1.19.0/streamlit/error_util.py
--rw-rw-r--   0 dorka     (1000) dorka     (1000)     3193 2023-03-07 14:32:33.000000 custom-streamlit-1.19.0/streamlit/errors.py
--rw-rw-r--   0 dorka     (1000) dorka     (1000)     6534 2023-03-07 14:32:33.000000 custom-streamlit-1.19.0/streamlit/file_util.py
--rw-rw-r--   0 dorka     (1000) dorka     (1000)     2309 2023-03-07 14:32:33.000000 custom-streamlit-1.19.0/streamlit/folder_black_list.py
--rw-rw-r--   0 dorka     (1000) dorka     (1000)     5242 2023-03-07 14:32:33.000000 custom-streamlit-1.19.0/streamlit/git_util.py
-drwxrwxr-x   0 dorka     (1000) dorka     (1000)        0 2023-03-08 13:56:49.998607 custom-streamlit-1.19.0/streamlit/hello/
--rw-rw-r--   0 dorka     (1000) dorka     (1000)     1737 2023-03-07 14:32:33.000000 custom-streamlit-1.19.0/streamlit/hello/Hello.py
--rw-rw-r--   0 dorka     (1000) dorka     (1000)      611 2023-03-07 14:32:33.000000 custom-streamlit-1.19.0/streamlit/hello/__init__.py
-drwxrwxr-x   0 dorka     (1000) dorka     (1000)        0 2023-03-08 13:56:50.002609 custom-streamlit-1.19.0/streamlit/hello/pages/
--rw-rw-r--   0 dorka     (1000) dorka     (1000)     2951 2023-03-07 14:32:33.000000 custom-streamlit-1.19.0/streamlit/hello/pages/0_Animation_Demo.py
--rw-rw-r--   0 dorka     (1000) dorka     (1000)     1738 2023-03-07 14:32:33.000000 custom-streamlit-1.19.0/streamlit/hello/pages/1_Plotting_Demo.py
--rw-rw-r--   0 dorka     (1000) dorka     (1000)     3821 2023-03-07 14:32:33.000000 custom-streamlit-1.19.0/streamlit/hello/pages/2_Mapping_Demo.py
--rw-rw-r--   0 dorka     (1000) dorka     (1000)     2522 2023-03-07 14:32:33.000000 custom-streamlit-1.19.0/streamlit/hello/pages/3_DataFrame_Demo.py
--rw-rw-r--   0 dorka     (1000) dorka     (1000)      987 2023-03-07 14:32:33.000000 custom-streamlit-1.19.0/streamlit/hello/utils.py
--rw-rw-r--   0 dorka     (1000) dorka     (1000)     3612 2023-03-07 14:32:33.000000 custom-streamlit-1.19.0/streamlit/js_number.py
--rw-rw-r--   0 dorka     (1000) dorka     (1000)     3987 2023-03-07 14:32:33.000000 custom-streamlit-1.19.0/streamlit/logger.py
--rw-rw-r--   0 dorka     (1000) dorka     (1000)     3096 2023-03-07 14:32:33.000000 custom-streamlit-1.19.0/streamlit/net_util.py
-drwxrwxr-x   0 dorka     (1000) dorka     (1000)        0 2023-03-08 13:56:50.030620 custom-streamlit-1.19.0/streamlit/proto/
--rw-rw-r--   0 dorka     (1000) dorka     (1000)     4298 2023-03-08 13:56:40.000000 custom-streamlit-1.19.0/streamlit/proto/Alert_pb2.py
--rw-rw-r--   0 dorka     (1000) dorka     (1000)     2867 2023-03-08 13:56:40.000000 custom-streamlit-1.19.0/streamlit/proto/AppPage_pb2.py
--rw-rw-r--   0 dorka     (1000) dorka     (1000)     3282 2023-03-08 13:56:40.000000 custom-streamlit-1.19.0/streamlit/proto/ArrowNamedDataSet_pb2.py
--rw-rw-r--   0 dorka     (1000) dorka     (1000)     4623 2023-03-08 13:56:40.000000 custom-streamlit-1.19.0/streamlit/proto/ArrowVegaLiteChart_pb2.py
--rw-rw-r--   0 dorka     (1000) dorka     (1000)     9611 2023-03-08 13:56:40.000000 custom-streamlit-1.19.0/streamlit/proto/Arrow_pb2.py
--rw-rw-r--   0 dorka     (1000) dorka     (1000)     2435 2023-03-08 13:56:40.000000 custom-streamlit-1.19.0/streamlit/proto/Audio_pb2.py
--rw-rw-r--   0 dorka     (1000) dorka     (1000)     7278 2023-03-08 13:56:40.000000 custom-streamlit-1.19.0/streamlit/proto/BackMsg_pb2.py
--rw-rw-r--   0 dorka     (1000) dorka     (1000)     1993 2023-03-08 13:56:40.000000 custom-streamlit-1.19.0/streamlit/proto/Balloons_pb2.py
--rw-rw-r--   0 dorka     (1000) dorka     (1000)    16064 2023-03-08 13:56:40.000000 custom-streamlit-1.19.0/streamlit/proto/Block_pb2.py
--rw-rw-r--   0 dorka     (1000) dorka     (1000)     2922 2023-03-08 13:56:40.000000 custom-streamlit-1.19.0/streamlit/proto/BokehChart_pb2.py
--rw-rw-r--   0 dorka     (1000) dorka     (1000)     5507 2023-03-08 13:56:40.000000 custom-streamlit-1.19.0/streamlit/proto/Button_pb2.py
--rw-rw-r--   0 dorka     (1000) dorka     (1000)     4669 2023-03-08 13:56:40.000000 custom-streamlit-1.19.0/streamlit/proto/CameraInput_pb2.py
--rw-rw-r--   0 dorka     (1000) dorka     (1000)     5917 2023-03-08 13:56:40.000000 custom-streamlit-1.19.0/streamlit/proto/Checkbox_pb2.py
--rw-rw-r--   0 dorka     (1000) dorka     (1000)     3752 2023-03-08 13:56:40.000000 custom-streamlit-1.19.0/streamlit/proto/ClientState_pb2.py
--rw-rw-r--   0 dorka     (1000) dorka     (1000)     2819 2023-03-08 13:56:40.000000 custom-streamlit-1.19.0/streamlit/proto/Code_pb2.py
--rw-rw-r--   0 dorka     (1000) dorka     (1000)     6013 2023-03-08 13:56:40.000000 custom-streamlit-1.19.0/streamlit/proto/ColorPicker_pb2.py
--rw-rw-r--   0 dorka     (1000) dorka     (1000)    12039 2023-03-08 13:56:40.000000 custom-streamlit-1.19.0/streamlit/proto/Common_pb2.py
--rw-rw-r--   0 dorka     (1000) dorka     (1000)    14749 2023-03-08 13:56:40.000000 custom-streamlit-1.19.0/streamlit/proto/Components_pb2.py
--rw-rw-r--   0 dorka     (1000) dorka     (1000)    32146 2023-03-08 13:56:40.000000 custom-streamlit-1.19.0/streamlit/proto/DataFrame_pb2.py
--rw-rw-r--   0 dorka     (1000) dorka     (1000)     7244 2023-03-08 13:56:40.000000 custom-streamlit-1.19.0/streamlit/proto/DateInput_pb2.py
--rw-rw-r--   0 dorka     (1000) dorka     (1000)     3010 2023-03-08 13:56:40.000000 custom-streamlit-1.19.0/streamlit/proto/DeckGlJsonChart_pb2.py
--rw-rw-r--   0 dorka     (1000) dorka     (1000)     5385 2023-03-08 13:56:40.000000 custom-streamlit-1.19.0/streamlit/proto/Delta_pb2.py
--rw-rw-r--   0 dorka     (1000) dorka     (1000)     3764 2023-03-08 13:56:40.000000 custom-streamlit-1.19.0/streamlit/proto/DocString_pb2.py
--rw-rw-r--   0 dorka     (1000) dorka     (1000)     5223 2023-03-08 13:56:40.000000 custom-streamlit-1.19.0/streamlit/proto/DownloadButton_pb2.py
--rw-rw-r--   0 dorka     (1000) dorka     (1000)    42409 2023-03-08 13:56:40.000000 custom-streamlit-1.19.0/streamlit/proto/Element_pb2.py
--rw-rw-r--   0 dorka     (1000) dorka     (1000)     1476 2023-03-08 13:56:40.000000 custom-streamlit-1.19.0/streamlit/proto/Empty_pb2.py
--rw-rw-r--   0 dorka     (1000) dorka     (1000)     3782 2023-03-08 13:56:40.000000 custom-streamlit-1.19.0/streamlit/proto/Exception_pb2.py
--rw-rw-r--   0 dorka     (1000) dorka     (1000)     1944 2023-03-08 13:56:40.000000 custom-streamlit-1.19.0/streamlit/proto/Favicon_pb2.py
--rw-rw-r--   0 dorka     (1000) dorka     (1000)     6066 2023-03-08 13:56:40.000000 custom-streamlit-1.19.0/streamlit/proto/FileUploader_pb2.py
--rw-rw-r--   0 dorka     (1000) dorka     (1000)    19815 2023-03-08 13:56:40.000000 custom-streamlit-1.19.0/streamlit/proto/ForwardMsg_pb2.py
--rw-rw-r--   0 dorka     (1000) dorka     (1000)     5383 2023-03-08 13:56:40.000000 custom-streamlit-1.19.0/streamlit/proto/GitInfo_pb2.py
--rw-rw-r--   0 dorka     (1000) dorka     (1000)     3012 2023-03-08 13:56:40.000000 custom-streamlit-1.19.0/streamlit/proto/GraphVizChart_pb2.py
--rw-rw-r--   0 dorka     (1000) dorka     (1000)     2823 2023-03-08 13:56:40.000000 custom-streamlit-1.19.0/streamlit/proto/Heading_pb2.py
--rw-rw-r--   0 dorka     (1000) dorka     (1000)     4633 2023-03-08 13:56:40.000000 custom-streamlit-1.19.0/streamlit/proto/IFrame_pb2.py
--rw-rw-r--   0 dorka     (1000) dorka     (1000)     4509 2023-03-08 13:56:40.000000 custom-streamlit-1.19.0/streamlit/proto/Image_pb2.py
--rw-rw-r--   0 dorka     (1000) dorka     (1000)     2334 2023-03-08 13:56:40.000000 custom-streamlit-1.19.0/streamlit/proto/Json_pb2.py
--rw-rw-r--   0 dorka     (1000) dorka     (1000)     3567 2023-03-08 13:56:40.000000 custom-streamlit-1.19.0/streamlit/proto/LabelVisibilityMessage_pb2.py
--rw-rw-r--   0 dorka     (1000) dorka     (1000)     4839 2023-03-08 13:56:40.000000 custom-streamlit-1.19.0/streamlit/proto/Markdown_pb2.py
--rw-rw-r--   0 dorka     (1000) dorka     (1000)     7304 2023-03-08 13:56:40.000000 custom-streamlit-1.19.0/streamlit/proto/Metric_pb2.py
--rw-rw-r--   0 dorka     (1000) dorka     (1000)     6874 2023-03-08 13:56:40.000000 custom-streamlit-1.19.0/streamlit/proto/MultiSelect_pb2.py
--rw-rw-r--   0 dorka     (1000) dorka     (1000)     3210 2023-03-08 13:56:40.000000 custom-streamlit-1.19.0/streamlit/proto/NamedDataSet_pb2.py
--rw-rw-r--   0 dorka     (1000) dorka     (1000)    22768 2023-03-08 13:56:40.000000 custom-streamlit-1.19.0/streamlit/proto/NewSession_pb2.py
--rw-rw-r--   0 dorka     (1000) dorka     (1000)    10165 2023-03-08 13:56:40.000000 custom-streamlit-1.19.0/streamlit/proto/NumberInput_pb2.py
--rw-rw-r--   0 dorka     (1000) dorka     (1000)     9326 2023-03-08 13:56:40.000000 custom-streamlit-1.19.0/streamlit/proto/PageConfig_pb2.py
--rw-rw-r--   0 dorka     (1000) dorka     (1000)     1978 2023-03-08 13:56:40.000000 custom-streamlit-1.19.0/streamlit/proto/PageInfo_pb2.py
--rw-rw-r--   0 dorka     (1000) dorka     (1000)     2029 2023-03-08 13:56:40.000000 custom-streamlit-1.19.0/streamlit/proto/PageNotFound_pb2.py
--rw-rw-r--   0 dorka     (1000) dorka     (1000)    10218 2023-03-08 13:56:40.000000 custom-streamlit-1.19.0/streamlit/proto/PageProfile_pb2.py
--rw-rw-r--   0 dorka     (1000) dorka     (1000)     2322 2023-03-08 13:56:40.000000 custom-streamlit-1.19.0/streamlit/proto/PagesChanged_pb2.py
--rw-rw-r--   0 dorka     (1000) dorka     (1000)     5670 2023-03-08 13:56:40.000000 custom-streamlit-1.19.0/streamlit/proto/PlotlyChart_pb2.py
--rw-rw-r--   0 dorka     (1000) dorka     (1000)     2378 2023-03-08 13:56:40.000000 custom-streamlit-1.19.0/streamlit/proto/Progress_pb2.py
--rw-rw-r--   0 dorka     (1000) dorka     (1000)     6700 2023-03-08 13:56:40.000000 custom-streamlit-1.19.0/streamlit/proto/Radio_pb2.py
--rw-rw-r--   0 dorka     (1000) dorka     (1000)     1760 2023-03-08 13:56:40.000000 custom-streamlit-1.19.0/streamlit/proto/RootContainer_pb2.py
--rw-rw-r--   0 dorka     (1000) dorka     (1000)     6360 2023-03-08 13:56:40.000000 custom-streamlit-1.19.0/streamlit/proto/Selectbox_pb2.py
--rw-rw-r--   0 dorka     (1000) dorka     (1000)     4305 2023-03-08 13:56:40.000000 custom-streamlit-1.19.0/streamlit/proto/SessionEvent_pb2.py
--rw-rw-r--   0 dorka     (1000) dorka     (1000)     2513 2023-03-08 13:56:40.000000 custom-streamlit-1.19.0/streamlit/proto/SessionStatus_pb2.py
--rw-rw-r--   0 dorka     (1000) dorka     (1000)    11535 2023-03-08 13:56:40.000000 custom-streamlit-1.19.0/streamlit/proto/Slider_pb2.py
--rw-rw-r--   0 dorka     (1000) dorka     (1000)     1884 2023-03-08 13:56:40.000000 custom-streamlit-1.19.0/streamlit/proto/Snow_pb2.py
--rw-rw-r--   0 dorka     (1000) dorka     (1000)     1941 2023-03-08 13:56:40.000000 custom-streamlit-1.19.0/streamlit/proto/Spinner_pb2.py
--rw-rw-r--   0 dorka     (1000) dorka     (1000)     7264 2023-03-08 13:56:40.000000 custom-streamlit-1.19.0/streamlit/proto/TextArea_pb2.py
--rw-rw-r--   0 dorka     (1000) dorka     (1000)     8686 2023-03-08 13:56:40.000000 custom-streamlit-1.19.0/streamlit/proto/TextInput_pb2.py
--rw-rw-r--   0 dorka     (1000) dorka     (1000)     1896 2023-03-08 13:56:40.000000 custom-streamlit-1.19.0/streamlit/proto/Text_pb2.py
--rw-rw-r--   0 dorka     (1000) dorka     (1000)     5961 2023-03-08 13:56:40.000000 custom-streamlit-1.19.0/streamlit/proto/TimeInput_pb2.py
--rw-rw-r--   0 dorka     (1000) dorka     (1000)     4048 2023-03-08 13:56:40.000000 custom-streamlit-1.19.0/streamlit/proto/VegaLiteChart_pb2.py
--rw-rw-r--   0 dorka     (1000) dorka     (1000)     3953 2023-03-08 13:56:40.000000 custom-streamlit-1.19.0/streamlit/proto/Video_pb2.py
--rw-rw-r--   0 dorka     (1000) dorka     (1000)    12593 2023-03-08 13:56:40.000000 custom-streamlit-1.19.0/streamlit/proto/WidgetStates_pb2.py
--rw-rw-r--   0 dorka     (1000) dorka     (1000)      663 2023-03-07 14:32:33.000000 custom-streamlit-1.19.0/streamlit/proto/__init__.py
--rw-rw-r--   0 dorka     (1000) dorka     (1000)    45888 2023-03-08 13:56:40.000000 custom-streamlit-1.19.0/streamlit/proto/openmetrics_data_model_pb2.py
--rw-rw-r--   0 dorka     (1000) dorka     (1000)        0 2023-03-07 14:32:33.000000 custom-streamlit-1.19.0/streamlit/py.typed
-drwxrwxr-x   0 dorka     (1000) dorka     (1000)        0 2023-03-08 13:56:50.038623 custom-streamlit-1.19.0/streamlit/runtime/
--rw-rw-r--   0 dorka     (1000) dorka     (1000)     1604 2023-03-07 14:32:33.000000 custom-streamlit-1.19.0/streamlit/runtime/__init__.py
--rw-rw-r--   0 dorka     (1000) dorka     (1000)    31650 2023-03-07 14:32:33.000000 custom-streamlit-1.19.0/streamlit/runtime/app_session.py
-drwxrwxr-x   0 dorka     (1000) dorka     (1000)        0 2023-03-08 13:56:50.042625 custom-streamlit-1.19.0/streamlit/runtime/caching/
--rw-rw-r--   0 dorka     (1000) dorka     (1000)     4700 2023-03-07 14:32:33.000000 custom-streamlit-1.19.0/streamlit/runtime/caching/__init__.py
--rw-rw-r--   0 dorka     (1000) dorka     (1000)    23805 2023-03-07 14:32:33.000000 custom-streamlit-1.19.0/streamlit/runtime/caching/cache_data_api.py
--rw-rw-r--   0 dorka     (1000) dorka     (1000)     5992 2023-03-07 14:32:33.000000 custom-streamlit-1.19.0/streamlit/runtime/caching/cache_errors.py
--rw-rw-r--   0 dorka     (1000) dorka     (1000)    18797 2023-03-07 14:32:33.000000 custom-streamlit-1.19.0/streamlit/runtime/caching/cache_resource_api.py
--rw-rw-r--   0 dorka     (1000) dorka     (1000)     1090 2023-03-07 14:32:33.000000 custom-streamlit-1.19.0/streamlit/runtime/caching/cache_type.py
--rw-rw-r--   0 dorka     (1000) dorka     (1000)    16653 2023-03-07 14:32:33.000000 custom-streamlit-1.19.0/streamlit/runtime/caching/cache_utils.py
--rw-rw-r--   0 dorka     (1000) dorka     (1000)    18475 2023-03-07 14:32:33.000000 custom-streamlit-1.19.0/streamlit/runtime/caching/cached_message_replay.py
--rw-rw-r--   0 dorka     (1000) dorka     (1000)    13106 2023-03-07 14:32:33.000000 custom-streamlit-1.19.0/streamlit/runtime/caching/hashing.py
-drwxrwxr-x   0 dorka     (1000) dorka     (1000)        0 2023-03-08 13:56:50.042625 custom-streamlit-1.19.0/streamlit/runtime/caching/storage/
--rw-rw-r--   0 dorka     (1000) dorka     (1000)     1217 2023-03-07 14:32:33.000000 custom-streamlit-1.19.0/streamlit/runtime/caching/storage/__init__.py
--rw-rw-r--   0 dorka     (1000) dorka     (1000)     7764 2023-03-07 14:32:33.000000 custom-streamlit-1.19.0/streamlit/runtime/caching/storage/cache_storage_protocol.py
--rw-rw-r--   0 dorka     (1000) dorka     (1000)     1940 2023-03-07 14:32:33.000000 custom-streamlit-1.19.0/streamlit/runtime/caching/storage/dummy_cache_storage.py
--rw-rw-r--   0 dorka     (1000) dorka     (1000)     5384 2023-03-07 14:32:33.000000 custom-streamlit-1.19.0/streamlit/runtime/caching/storage/in_memory_cache_storage_wrapper.py
--rw-rw-r--   0 dorka     (1000) dorka     (1000)     7609 2023-03-07 14:32:33.000000 custom-streamlit-1.19.0/streamlit/runtime/caching/storage/local_disk_cache_storage.py
--rw-rw-r--   0 dorka     (1000) dorka     (1000)     9401 2023-03-07 14:32:33.000000 custom-streamlit-1.19.0/streamlit/runtime/credentials.py
--rw-rw-r--   0 dorka     (1000) dorka     (1000)     8790 2023-03-07 14:32:33.000000 custom-streamlit-1.19.0/streamlit/runtime/forward_msg_cache.py
--rw-rw-r--   0 dorka     (1000) dorka     (1000)     5549 2023-03-07 14:32:33.000000 custom-streamlit-1.19.0/streamlit/runtime/forward_msg_queue.py
-drwxrwxr-x   0 dorka     (1000) dorka     (1000)        0 2023-03-08 13:56:50.042625 custom-streamlit-1.19.0/streamlit/runtime/legacy_caching/
--rw-rw-r--   0 dorka     (1000) dorka     (1000)      987 2023-03-07 14:32:33.000000 custom-streamlit-1.19.0/streamlit/runtime/legacy_caching/__init__.py
--rw-rw-r--   0 dorka     (1000) dorka     (1000)    30548 2023-03-07 14:32:33.000000 custom-streamlit-1.19.0/streamlit/runtime/legacy_caching/caching.py
--rw-rw-r--   0 dorka     (1000) dorka     (1000)    35123 2023-03-07 14:32:33.000000 custom-streamlit-1.19.0/streamlit/runtime/legacy_caching/hashing.py
--rw-rw-r--   0 dorka     (1000) dorka     (1000)     8489 2023-03-07 14:32:33.000000 custom-streamlit-1.19.0/streamlit/runtime/media_file_manager.py
--rw-rw-r--   0 dorka     (1000) dorka     (1000)     4396 2023-03-07 14:32:33.000000 custom-streamlit-1.19.0/streamlit/runtime/media_file_storage.py
--rw-rw-r--   0 dorka     (1000) dorka     (1000)     6251 2023-03-07 14:32:33.000000 custom-streamlit-1.19.0/streamlit/runtime/memory_media_file_storage.py
--rw-rw-r--   0 dorka     (1000) dorka     (1000)     2918 2023-03-07 14:32:33.000000 custom-streamlit-1.19.0/streamlit/runtime/memory_session_storage.py
--rw-rw-r--   0 dorka     (1000) dorka     (1000)    12208 2023-03-07 14:32:33.000000 custom-streamlit-1.19.0/streamlit/runtime/metrics_util.py
--rw-rw-r--   0 dorka     (1000) dorka     (1000)    26047 2023-03-07 15:27:59.000000 custom-streamlit-1.19.0/streamlit/runtime/runtime.py
--rw-rw-r--   0 dorka     (1000) dorka     (1000)     3790 2023-03-07 14:32:33.000000 custom-streamlit-1.19.0/streamlit/runtime/runtime_util.py
--rw-rw-r--   0 dorka     (1000) dorka     (1000)     1703 2023-03-07 14:32:33.000000 custom-streamlit-1.19.0/streamlit/runtime/script_data.py
-drwxrwxr-x   0 dorka     (1000) dorka     (1000)        0 2023-03-08 13:56:50.046626 custom-streamlit-1.19.0/streamlit/runtime/scriptrunner/
--rw-rw-r--   0 dorka     (1000) dorka     (1000)     1439 2023-03-07 14:32:33.000000 custom-streamlit-1.19.0/streamlit/runtime/scriptrunner/__init__.py
--rw-rw-r--   0 dorka     (1000) dorka     (1000)     6079 2023-03-07 14:32:33.000000 custom-streamlit-1.19.0/streamlit/runtime/scriptrunner/magic.py
--rw-rw-r--   0 dorka     (1000) dorka     (1000)     1015 2023-03-07 14:32:33.000000 custom-streamlit-1.19.0/streamlit/runtime/scriptrunner/magic_funcs.py
--rw-rw-r--   0 dorka     (1000) dorka     (1000)     6965 2023-03-07 14:32:33.000000 custom-streamlit-1.19.0/streamlit/runtime/scriptrunner/script_requests.py
--rw-rw-r--   0 dorka     (1000) dorka     (1000)     6242 2023-03-07 14:32:33.000000 custom-streamlit-1.19.0/streamlit/runtime/scriptrunner/script_run_context.py
--rw-rw-r--   0 dorka     (1000) dorka     (1000)    26966 2023-03-07 14:32:33.000000 custom-streamlit-1.19.0/streamlit/runtime/scriptrunner/script_runner.py
--rw-rw-r--   0 dorka     (1000) dorka     (1000)    10630 2023-03-07 14:32:33.000000 custom-streamlit-1.19.0/streamlit/runtime/secrets.py
--rw-rw-r--   0 dorka     (1000) dorka     (1000)    12404 2023-03-07 14:32:33.000000 custom-streamlit-1.19.0/streamlit/runtime/session_manager.py
-drwxrwxr-x   0 dorka     (1000) dorka     (1000)        0 2023-03-08 13:56:50.046626 custom-streamlit-1.19.0/streamlit/runtime/state/
--rw-rw-r--   0 dorka     (1000) dorka     (1000)     1733 2023-03-07 14:32:33.000000 custom-streamlit-1.19.0/streamlit/runtime/state/__init__.py
--rw-rw-r--   0 dorka     (1000) dorka     (1000)     6512 2023-03-07 14:32:33.000000 custom-streamlit-1.19.0/streamlit/runtime/state/common.py
--rw-rw-r--   0 dorka     (1000) dorka     (1000)     4624 2023-03-07 14:32:33.000000 custom-streamlit-1.19.0/streamlit/runtime/state/safe_session_state.py
--rw-rw-r--   0 dorka     (1000) dorka     (1000)    23365 2023-03-07 14:32:33.000000 custom-streamlit-1.19.0/streamlit/runtime/state/session_state.py
--rw-rw-r--   0 dorka     (1000) dorka     (1000)     5098 2023-03-07 14:32:33.000000 custom-streamlit-1.19.0/streamlit/runtime/state/session_state_proxy.py
--rw-rw-r--   0 dorka     (1000) dorka     (1000)    10808 2023-03-07 14:32:33.000000 custom-streamlit-1.19.0/streamlit/runtime/state/widgets.py
--rw-rw-r--   0 dorka     (1000) dorka     (1000)     3044 2023-03-07 14:32:33.000000 custom-streamlit-1.19.0/streamlit/runtime/stats.py
--rw-rw-r--   0 dorka     (1000) dorka     (1000)    11423 2023-03-07 14:32:33.000000 custom-streamlit-1.19.0/streamlit/runtime/uploaded_file_manager.py
--rw-rw-r--   0 dorka     (1000) dorka     (1000)     5844 2023-03-07 14:32:33.000000 custom-streamlit-1.19.0/streamlit/runtime/websocket_session_manager.py
--rw-rw-r--   0 dorka     (1000) dorka     (1000)     5688 2023-03-07 14:32:33.000000 custom-streamlit-1.19.0/streamlit/source_util.py
--rw-rw-r--   0 dorka     (1000) dorka     (1000)     5408 2023-03-07 14:32:33.000000 custom-streamlit-1.19.0/streamlit/string_util.py
--rw-rw-r--   0 dorka     (1000) dorka     (1000)     1594 2023-03-07 14:32:33.000000 custom-streamlit-1.19.0/streamlit/temporary_directory.py
-drwxrwxr-x   0 dorka     (1000) dorka     (1000)        0 2023-03-08 13:56:50.050628 custom-streamlit-1.19.0/streamlit/testing/
--rw-rw-r--   0 dorka     (1000) dorka     (1000)      611 2023-03-07 14:32:33.000000 custom-streamlit-1.19.0/streamlit/testing/__init__.py
--rw-rw-r--   0 dorka     (1000) dorka     (1000)    28101 2023-03-07 14:32:33.000000 custom-streamlit-1.19.0/streamlit/testing/element_tree.py
--rw-rw-r--   0 dorka     (1000) dorka     (1000)     5300 2023-03-07 14:32:33.000000 custom-streamlit-1.19.0/streamlit/testing/local_script_runner.py
--rw-rw-r--   0 dorka     (1000) dorka     (1000)     2852 2023-03-07 14:32:33.000000 custom-streamlit-1.19.0/streamlit/testing/script_interactions.py
--rw-rw-r--   0 dorka     (1000) dorka     (1000)    31285 2023-03-07 14:32:33.000000 custom-streamlit-1.19.0/streamlit/type_util.py
--rw-rw-r--   0 dorka     (1000) dorka     (1000)     2289 2023-03-07 14:32:33.000000 custom-streamlit-1.19.0/streamlit/url_util.py
--rw-rw-r--   0 dorka     (1000) dorka     (1000)     1981 2023-03-07 14:32:33.000000 custom-streamlit-1.19.0/streamlit/user_info.py
--rw-rw-r--   0 dorka     (1000) dorka     (1000)     5581 2023-03-07 14:32:33.000000 custom-streamlit-1.19.0/streamlit/util.py
-drwxrwxr-x   0 dorka     (1000) dorka     (1000)        0 2023-03-08 13:56:50.050628 custom-streamlit-1.19.0/streamlit/vendor/
--rw-rw-r--   0 dorka     (1000) dorka     (1000)        0 2023-03-07 14:32:33.000000 custom-streamlit-1.19.0/streamlit/vendor/__init__.py
-drwxrwxr-x   0 dorka     (1000) dorka     (1000)        0 2023-03-08 13:56:50.050628 custom-streamlit-1.19.0/streamlit/vendor/ipython/
--rw-rw-r--   0 dorka     (1000) dorka     (1000)        0 2023-03-07 14:32:33.000000 custom-streamlit-1.19.0/streamlit/vendor/ipython/__init__.py
--rw-rw-r--   0 dorka     (1000) dorka     (1000)     2746 2023-03-07 14:32:33.000000 custom-streamlit-1.19.0/streamlit/vendor/ipython/modified_sys_path.py
--rw-rw-r--   0 dorka     (1000) dorka     (1000)     3347 2023-03-07 14:32:33.000000 custom-streamlit-1.19.0/streamlit/version.py
-drwxrwxr-x   0 dorka     (1000) dorka     (1000)        0 2023-03-08 13:56:50.054629 custom-streamlit-1.19.0/streamlit/watcher/
--rw-rw-r--   0 dorka     (1000) dorka     (1000)      963 2023-03-07 14:32:33.000000 custom-streamlit-1.19.0/streamlit/watcher/__init__.py
--rw-rw-r--   0 dorka     (1000) dorka     (1000)    13689 2023-03-07 14:32:33.000000 custom-streamlit-1.19.0/streamlit/watcher/event_based_path_watcher.py
--rw-rw-r--   0 dorka     (1000) dorka     (1000)     7617 2023-03-07 14:32:33.000000 custom-streamlit-1.19.0/streamlit/watcher/local_sources_watcher.py
--rw-rw-r--   0 dorka     (1000) dorka     (1000)     5673 2023-03-07 14:32:33.000000 custom-streamlit-1.19.0/streamlit/watcher/path_watcher.py
--rw-rw-r--   0 dorka     (1000) dorka     (1000)     3570 2023-03-07 14:32:33.000000 custom-streamlit-1.19.0/streamlit/watcher/polling_path_watcher.py
--rw-rw-r--   0 dorka     (1000) dorka     (1000)     5134 2023-03-07 14:32:33.000000 custom-streamlit-1.19.0/streamlit/watcher/util.py
-drwxrwxr-x   0 dorka     (1000) dorka     (1000)        0 2023-03-08 13:56:50.054629 custom-streamlit-1.19.0/streamlit/web/
--rw-rw-r--   0 dorka     (1000) dorka     (1000)      611 2023-03-07 14:32:33.000000 custom-streamlit-1.19.0/streamlit/web/__init__.py
--rw-rw-r--   0 dorka     (1000) dorka     (1000)    14779 2023-03-07 14:32:33.000000 custom-streamlit-1.19.0/streamlit/web/bootstrap.py
--rw-rw-r--   0 dorka     (1000) dorka     (1000)     1117 2023-03-07 14:32:33.000000 custom-streamlit-1.19.0/streamlit/web/cache_storage_manager_config.py
--rw-rw-r--   0 dorka     (1000) dorka     (1000)    10384 2023-03-07 14:32:33.000000 custom-streamlit-1.19.0/streamlit/web/cli.py
-drwxrwxr-x   0 dorka     (1000) dorka     (1000)        0 2023-03-08 13:56:50.058631 custom-streamlit-1.19.0/streamlit/web/server/
--rw-rw-r--   0 dorka     (1000) dorka     (1000)     1047 2023-03-07 14:32:33.000000 custom-streamlit-1.19.0/streamlit/web/server/__init__.py
--rw-rw-r--   0 dorka     (1000) dorka     (1000)     2666 2023-03-07 14:32:33.000000 custom-streamlit-1.19.0/streamlit/web/server/app_static_file_handler.py
--rw-rw-r--   0 dorka     (1000) dorka     (1000)     7671 2023-03-07 14:32:33.000000 custom-streamlit-1.19.0/streamlit/web/server/browser_websocket_handler.py
--rw-rw-r--   0 dorka     (1000) dorka     (1000)     4205 2023-03-07 14:32:33.000000 custom-streamlit-1.19.0/streamlit/web/server/component_request_handler.py
--rw-rw-r--   0 dorka     (1000) dorka     (1000)     5574 2023-03-07 14:32:33.000000 custom-streamlit-1.19.0/streamlit/web/server/media_file_handler.py
--rw-rw-r--   0 dorka     (1000) dorka     (1000)     9303 2023-03-07 14:32:33.000000 custom-streamlit-1.19.0/streamlit/web/server/routes.py
--rw-rw-r--   0 dorka     (1000) dorka     (1000)    14583 2023-03-07 14:32:33.000000 custom-streamlit-1.19.0/streamlit/web/server/server.py
--rw-rw-r--   0 dorka     (1000) dorka     (1000)     4033 2023-03-07 14:32:33.000000 custom-streamlit-1.19.0/streamlit/web/server/server_util.py
--rw-rw-r--   0 dorka     (1000) dorka     (1000)     3405 2023-03-07 14:32:33.000000 custom-streamlit-1.19.0/streamlit/web/server/stats_request_handler.py
--rw-rw-r--   0 dorka     (1000) dorka     (1000)     5964 2023-03-07 14:32:33.000000 custom-streamlit-1.19.0/streamlit/web/server/upload_file_request_handler.py
--rw-rw-r--   0 dorka     (1000) dorka     (1000)     1867 2023-03-07 14:32:33.000000 custom-streamlit-1.19.0/streamlit/web/server/websocket_headers.py
-drwxrwxr-x   0 dorka     (1000) dorka     (1000)        0 2023-03-08 13:56:50.058631 custom-streamlit-1.19.0/tests/
--rw-rw-r--   0 dorka     (1000) dorka     (1000)     4900 2023-03-07 14:32:33.000000 custom-streamlit-1.19.0/tests/testutil.py
+drwxrwxr-x   0 dorka     (1000) dorka     (1000)        0 2023-04-07 18:36:01.530182 custom-streamlit-1.20.0/
+-rw-rw-r--   0 dorka     (1000) dorka     (1000)      116 2023-03-07 14:32:33.000000 custom-streamlit-1.20.0/MANIFEST.in
+-rw-rw-r--   0 dorka     (1000) dorka     (1000)     1640 2023-04-07 18:36:01.530182 custom-streamlit-1.20.0/PKG-INFO
+-rw-rw-r--   0 dorka     (1000) dorka     (1000)     1748 2023-03-07 14:32:33.000000 custom-streamlit-1.20.0/Pipfile
+drwxrwxr-x   0 dorka     (1000) dorka     (1000)        0 2023-04-07 18:36:01.482182 custom-streamlit-1.20.0/bin/
+-rw-rw-r--   0 dorka     (1000) dorka     (1000)      671 2023-03-07 14:32:33.000000 custom-streamlit-1.20.0/bin/streamlit.cmd
+drwxrwxr-x   0 dorka     (1000) dorka     (1000)        0 2023-04-07 18:36:01.482182 custom-streamlit-1.20.0/custom_streamlit.egg-info/
+-rw-rw-r--   0 dorka     (1000) dorka     (1000)     1640 2023-04-07 18:36:01.000000 custom-streamlit-1.20.0/custom_streamlit.egg-info/PKG-INFO
+-rw-rw-r--   0 dorka     (1000) dorka     (1000)     8542 2023-04-07 18:36:01.000000 custom-streamlit-1.20.0/custom_streamlit.egg-info/SOURCES.txt
+-rw-rw-r--   0 dorka     (1000) dorka     (1000)        1 2023-04-07 18:36:01.000000 custom-streamlit-1.20.0/custom_streamlit.egg-info/dependency_links.txt
+-rw-rw-r--   0 dorka     (1000) dorka     (1000)       53 2023-04-07 18:36:01.000000 custom-streamlit-1.20.0/custom_streamlit.egg-info/entry_points.txt
+-rw-rw-r--   0 dorka     (1000) dorka     (1000)        1 2023-03-08 13:55:57.000000 custom-streamlit-1.20.0/custom_streamlit.egg-info/not-zip-safe
+-rw-rw-r--   0 dorka     (1000) dorka     (1000)      456 2023-04-07 18:36:01.000000 custom-streamlit-1.20.0/custom_streamlit.egg-info/requires.txt
+-rw-rw-r--   0 dorka     (1000) dorka     (1000)       10 2023-04-07 18:36:01.000000 custom-streamlit-1.20.0/custom_streamlit.egg-info/top_level.txt
+-rw-rw-r--   0 dorka     (1000) dorka     (1000)       38 2023-04-07 18:36:01.530182 custom-streamlit-1.20.0/setup.cfg
+-rw-rw-r--   0 dorka     (1000) dorka     (1000)     6011 2023-04-07 18:35:36.000000 custom-streamlit-1.20.0/setup.py
+drwxrwxr-x   0 dorka     (1000) dorka     (1000)        0 2023-04-07 18:36:01.490182 custom-streamlit-1.20.0/streamlit/
+-rw-rw-r--   0 dorka     (1000) dorka     (1000)     6768 2023-03-07 14:32:33.000000 custom-streamlit-1.20.0/streamlit/__init__.py
+-rw-rw-r--   0 dorka     (1000) dorka     (1000)      863 2023-03-07 14:32:33.000000 custom-streamlit-1.20.0/streamlit/__main__.py
+-rw-rw-r--   0 dorka     (1000) dorka     (1000)     2296 2023-03-07 14:32:33.000000 custom-streamlit-1.20.0/streamlit/case_converters.py
+-rw-rw-r--   0 dorka     (1000) dorka     (1000)     2284 2023-03-07 14:32:33.000000 custom-streamlit-1.20.0/streamlit/code_util.py
+drwxrwxr-x   0 dorka     (1000) dorka     (1000)        0 2023-04-07 18:36:01.490182 custom-streamlit-1.20.0/streamlit/commands/
+-rw-rw-r--   0 dorka     (1000) dorka     (1000)      611 2023-03-07 14:32:33.000000 custom-streamlit-1.20.0/streamlit/commands/__init__.py
+-rw-rw-r--   0 dorka     (1000) dorka     (1000)     1970 2023-03-07 14:32:33.000000 custom-streamlit-1.20.0/streamlit/commands/execution_control.py
+-rw-rw-r--   0 dorka     (1000) dorka     (1000)    11977 2023-03-07 14:32:33.000000 custom-streamlit-1.20.0/streamlit/commands/page_config.py
+-rw-rw-r--   0 dorka     (1000) dorka     (1000)     4830 2023-03-07 14:32:33.000000 custom-streamlit-1.20.0/streamlit/commands/query_params.py
+drwxrwxr-x   0 dorka     (1000) dorka     (1000)        0 2023-04-07 18:36:01.490182 custom-streamlit-1.20.0/streamlit/components/
+-rw-rw-r--   0 dorka     (1000) dorka     (1000)      611 2023-03-07 14:32:33.000000 custom-streamlit-1.20.0/streamlit/components/__init__.py
+drwxrwxr-x   0 dorka     (1000) dorka     (1000)        0 2023-04-07 18:36:01.490182 custom-streamlit-1.20.0/streamlit/components/v1/
+-rw-rw-r--   0 dorka     (1000) dorka     (1000)     1031 2023-03-07 14:32:33.000000 custom-streamlit-1.20.0/streamlit/components/v1/__init__.py
+-rw-rw-r--   0 dorka     (1000) dorka     (1000)    10898 2023-03-07 14:32:33.000000 custom-streamlit-1.20.0/streamlit/components/v1/component_arrow.py
+-rw-rw-r--   0 dorka     (1000) dorka     (1000)    12966 2023-03-07 14:32:33.000000 custom-streamlit-1.20.0/streamlit/components/v1/components.py
+-rw-rw-r--   0 dorka     (1000) dorka     (1000)    37021 2023-03-07 14:32:33.000000 custom-streamlit-1.20.0/streamlit/config.py
+-rw-rw-r--   0 dorka     (1000) dorka     (1000)    10753 2023-03-07 14:32:33.000000 custom-streamlit-1.20.0/streamlit/config_option.py
+-rw-rw-r--   0 dorka     (1000) dorka     (1000)     4515 2023-03-07 14:32:33.000000 custom-streamlit-1.20.0/streamlit/config_util.py
+-rw-rw-r--   0 dorka     (1000) dorka     (1000)     5997 2023-03-07 14:32:33.000000 custom-streamlit-1.20.0/streamlit/cursor.py
+-rw-rw-r--   0 dorka     (1000) dorka     (1000)    35516 2023-03-07 14:32:33.000000 custom-streamlit-1.20.0/streamlit/delta_generator.py
+-rw-rw-r--   0 dorka     (1000) dorka     (1000)     5651 2023-03-07 14:32:33.000000 custom-streamlit-1.20.0/streamlit/deprecation_util.py
+-rw-rw-r--   0 dorka     (1000) dorka     (1000)      808 2023-03-07 14:32:33.000000 custom-streamlit-1.20.0/streamlit/development.py
+-rw-rw-r--   0 dorka     (1000) dorka     (1000)     3955 2023-03-07 14:32:33.000000 custom-streamlit-1.20.0/streamlit/echo.py
+drwxrwxr-x   0 dorka     (1000) dorka     (1000)        0 2023-04-07 18:36:01.498182 custom-streamlit-1.20.0/streamlit/elements/
+-rw-rw-r--   0 dorka     (1000) dorka     (1000)     1664 2023-03-07 14:32:33.000000 custom-streamlit-1.20.0/streamlit/elements/__init__.py
+-rw-rw-r--   0 dorka     (1000) dorka     (1000)     5620 2023-03-07 14:32:33.000000 custom-streamlit-1.20.0/streamlit/elements/alert.py
+-rw-rw-r--   0 dorka     (1000) dorka     (1000)    14078 2023-03-07 14:32:33.000000 custom-streamlit-1.20.0/streamlit/elements/arrow.py
+-rw-rw-r--   0 dorka     (1000) dorka     (1000)    21671 2023-03-07 14:33:59.000000 custom-streamlit-1.20.0/streamlit/elements/arrow_altair.py
+-rw-rw-r--   0 dorka     (1000) dorka     (1000)     7196 2023-03-07 14:32:33.000000 custom-streamlit-1.20.0/streamlit/elements/arrow_vega_lite.py
+-rw-rw-r--   0 dorka     (1000) dorka     (1000)     1445 2023-03-07 14:32:33.000000 custom-streamlit-1.20.0/streamlit/elements/balloons.py
+-rw-rw-r--   0 dorka     (1000) dorka     (1000)     3856 2023-03-07 14:32:33.000000 custom-streamlit-1.20.0/streamlit/elements/bokeh_chart.py
+-rw-rw-r--   0 dorka     (1000) dorka     (1000)    16910 2023-03-07 14:32:33.000000 custom-streamlit-1.20.0/streamlit/elements/button.py
+-rw-rw-r--   0 dorka     (1000) dorka     (1000)    10040 2023-03-07 14:32:33.000000 custom-streamlit-1.20.0/streamlit/elements/camera_input.py
+-rw-rw-r--   0 dorka     (1000) dorka     (1000)     6798 2023-03-07 14:32:33.000000 custom-streamlit-1.20.0/streamlit/elements/checkbox.py
+-rw-rw-r--   0 dorka     (1000) dorka     (1000)     2452 2023-03-07 14:32:33.000000 custom-streamlit-1.20.0/streamlit/elements/code.py
+-rw-rw-r--   0 dorka     (1000) dorka     (1000)     8606 2023-03-07 14:32:33.000000 custom-streamlit-1.20.0/streamlit/elements/color_picker.py
+-rw-rw-r--   0 dorka     (1000) dorka     (1000)    22373 2023-03-07 14:32:33.000000 custom-streamlit-1.20.0/streamlit/elements/data_editor.py
+-rw-rw-r--   0 dorka     (1000) dorka     (1000)    23378 2023-03-07 14:32:33.000000 custom-streamlit-1.20.0/streamlit/elements/dataframe_selector.py
+-rw-rw-r--   0 dorka     (1000) dorka     (1000)     5900 2023-03-07 14:32:33.000000 custom-streamlit-1.20.0/streamlit/elements/deck_gl_json_chart.py
+-rw-rw-r--   0 dorka     (1000) dorka     (1000)     4443 2023-03-07 14:32:33.000000 custom-streamlit-1.20.0/streamlit/elements/doc_string.py
+-rw-rw-r--   0 dorka     (1000) dorka     (1000)     2598 2023-03-07 14:32:33.000000 custom-streamlit-1.20.0/streamlit/elements/empty.py
+-rw-rw-r--   0 dorka     (1000) dorka     (1000)     9131 2023-03-07 14:32:33.000000 custom-streamlit-1.20.0/streamlit/elements/exception.py
+-rw-rw-r--   0 dorka     (1000) dorka     (1000)    16905 2023-03-07 14:32:33.000000 custom-streamlit-1.20.0/streamlit/elements/file_uploader.py
+-rw-rw-r--   0 dorka     (1000) dorka     (1000)    11437 2023-03-07 14:32:33.000000 custom-streamlit-1.20.0/streamlit/elements/form.py
+-rw-rw-r--   0 dorka     (1000) dorka     (1000)     4461 2023-03-07 14:32:33.000000 custom-streamlit-1.20.0/streamlit/elements/graphviz_chart.py
+-rw-rw-r--   0 dorka     (1000) dorka     (1000)     6351 2023-03-07 14:32:33.000000 custom-streamlit-1.20.0/streamlit/elements/heading.py
+-rw-rw-r--   0 dorka     (1000) dorka     (1000)     4382 2023-03-07 14:32:33.000000 custom-streamlit-1.20.0/streamlit/elements/iframe.py
+-rw-rw-r--   0 dorka     (1000) dorka     (1000)    19520 2023-03-07 14:32:33.000000 custom-streamlit-1.20.0/streamlit/elements/image.py
+-rw-rw-r--   0 dorka     (1000) dorka     (1000)     3373 2023-03-07 14:32:33.000000 custom-streamlit-1.20.0/streamlit/elements/json.py
+-rw-rw-r--   0 dorka     (1000) dorka     (1000)    14350 2023-03-07 14:32:33.000000 custom-streamlit-1.20.0/streamlit/elements/layouts.py
+-rw-rw-r--   0 dorka     (1000) dorka     (1000)    13220 2023-03-07 14:32:33.000000 custom-streamlit-1.20.0/streamlit/elements/legacy_altair.py
+-rw-rw-r--   0 dorka     (1000) dorka     (1000)    17493 2023-03-07 14:32:33.000000 custom-streamlit-1.20.0/streamlit/elements/legacy_data_frame.py
+-rw-rw-r--   0 dorka     (1000) dorka     (1000)     6649 2023-03-07 14:32:33.000000 custom-streamlit-1.20.0/streamlit/elements/legacy_vega_lite.py
+drwxrwxr-x   0 dorka     (1000) dorka     (1000)        0 2023-04-07 18:36:01.498182 custom-streamlit-1.20.0/streamlit/elements/lib/
+-rw-rw-r--   0 dorka     (1000) dorka     (1000)      611 2023-03-07 14:32:33.000000 custom-streamlit-1.20.0/streamlit/elements/lib/__init__.py
+-rw-rw-r--   0 dorka     (1000) dorka     (1000)     3370 2023-03-07 14:32:33.000000 custom-streamlit-1.20.0/streamlit/elements/lib/dicttools.py
+-rw-rw-r--   0 dorka     (1000) dorka     (1000)     6407 2023-03-07 14:32:33.000000 custom-streamlit-1.20.0/streamlit/elements/lib/streamlit_plotly_theme.py
+-rw-rw-r--   0 dorka     (1000) dorka     (1000)     7968 2023-03-07 14:32:33.000000 custom-streamlit-1.20.0/streamlit/elements/map.py
+-rw-rw-r--   0 dorka     (1000) dorka     (1000)     6773 2023-03-07 14:32:33.000000 custom-streamlit-1.20.0/streamlit/elements/markdown.py
+-rw-rw-r--   0 dorka     (1000) dorka     (1000)    14695 2023-03-07 14:32:33.000000 custom-streamlit-1.20.0/streamlit/elements/media.py
+-rw-rw-r--   0 dorka     (1000) dorka     (1000)     9846 2023-03-07 14:32:33.000000 custom-streamlit-1.20.0/streamlit/elements/metric.py
+-rw-rw-r--   0 dorka     (1000) dorka     (1000)    12382 2023-03-07 14:32:33.000000 custom-streamlit-1.20.0/streamlit/elements/multiselect.py
+-rw-rw-r--   0 dorka     (1000) dorka     (1000)    14312 2023-03-07 14:32:33.000000 custom-streamlit-1.20.0/streamlit/elements/number_input.py
+-rw-rw-r--   0 dorka     (1000) dorka     (1000)     8822 2023-03-07 14:32:33.000000 custom-streamlit-1.20.0/streamlit/elements/plotly_chart.py
+-rw-rw-r--   0 dorka     (1000) dorka     (1000)     4450 2023-03-07 14:32:33.000000 custom-streamlit-1.20.0/streamlit/elements/progress.py
+-rw-rw-r--   0 dorka     (1000) dorka     (1000)     6123 2023-03-07 14:32:33.000000 custom-streamlit-1.20.0/streamlit/elements/pyplot.py
+-rw-rw-r--   0 dorka     (1000) dorka     (1000)     9810 2023-03-07 14:32:33.000000 custom-streamlit-1.20.0/streamlit/elements/radio.py
+-rw-rw-r--   0 dorka     (1000) dorka     (1000)    12352 2023-03-07 14:32:33.000000 custom-streamlit-1.20.0/streamlit/elements/select_slider.py
+-rw-rw-r--   0 dorka     (1000) dorka     (1000)     9286 2023-03-07 14:32:33.000000 custom-streamlit-1.20.0/streamlit/elements/selectbox.py
+-rw-rw-r--   0 dorka     (1000) dorka     (1000)     3546 2023-03-07 14:32:33.000000 custom-streamlit-1.20.0/streamlit/elements/show.py
+-rw-rw-r--   0 dorka     (1000) dorka     (1000)    24739 2023-03-07 14:32:33.000000 custom-streamlit-1.20.0/streamlit/elements/slider.py
+-rw-rw-r--   0 dorka     (1000) dorka     (1000)     1402 2023-03-07 14:32:33.000000 custom-streamlit-1.20.0/streamlit/elements/snow.py
+-rw-rw-r--   0 dorka     (1000) dorka     (1000)     3076 2023-03-07 14:32:33.000000 custom-streamlit-1.20.0/streamlit/elements/spinner.py
+-rw-rw-r--   0 dorka     (1000) dorka     (1000)     1585 2023-03-07 14:32:33.000000 custom-streamlit-1.20.0/streamlit/elements/text.py
+-rw-rw-r--   0 dorka     (1000) dorka     (1000)    17557 2023-03-07 14:32:33.000000 custom-streamlit-1.20.0/streamlit/elements/text_widgets.py
+-rw-rw-r--   0 dorka     (1000) dorka     (1000)    21020 2023-03-07 14:32:33.000000 custom-streamlit-1.20.0/streamlit/elements/time_widgets.py
+-rw-rw-r--   0 dorka     (1000) dorka     (1000)     3379 2023-03-07 14:32:33.000000 custom-streamlit-1.20.0/streamlit/elements/utils.py
+-rw-rw-r--   0 dorka     (1000) dorka     (1000)     9573 2023-03-07 14:32:33.000000 custom-streamlit-1.20.0/streamlit/elements/write.py
+-rw-rw-r--   0 dorka     (1000) dorka     (1000)    68199 2023-03-07 14:32:33.000000 custom-streamlit-1.20.0/streamlit/emojis.py
+-rw-rw-r--   0 dorka     (1000) dorka     (1000)     1750 2023-03-07 14:32:33.000000 custom-streamlit-1.20.0/streamlit/env_util.py
+-rw-rw-r--   0 dorka     (1000) dorka     (1000)     3539 2023-03-07 14:32:33.000000 custom-streamlit-1.20.0/streamlit/error_util.py
+-rw-rw-r--   0 dorka     (1000) dorka     (1000)     3193 2023-03-07 14:32:33.000000 custom-streamlit-1.20.0/streamlit/errors.py
+-rw-rw-r--   0 dorka     (1000) dorka     (1000)     6534 2023-03-07 14:32:33.000000 custom-streamlit-1.20.0/streamlit/file_util.py
+-rw-rw-r--   0 dorka     (1000) dorka     (1000)     2309 2023-03-07 14:32:33.000000 custom-streamlit-1.20.0/streamlit/folder_black_list.py
+-rw-rw-r--   0 dorka     (1000) dorka     (1000)     5242 2023-03-07 14:32:33.000000 custom-streamlit-1.20.0/streamlit/git_util.py
+drwxrwxr-x   0 dorka     (1000) dorka     (1000)        0 2023-04-07 18:36:01.498182 custom-streamlit-1.20.0/streamlit/hello/
+-rw-rw-r--   0 dorka     (1000) dorka     (1000)     1737 2023-03-07 14:32:33.000000 custom-streamlit-1.20.0/streamlit/hello/Hello.py
+-rw-rw-r--   0 dorka     (1000) dorka     (1000)      611 2023-03-07 14:32:33.000000 custom-streamlit-1.20.0/streamlit/hello/__init__.py
+drwxrwxr-x   0 dorka     (1000) dorka     (1000)        0 2023-04-07 18:36:01.498182 custom-streamlit-1.20.0/streamlit/hello/pages/
+-rw-rw-r--   0 dorka     (1000) dorka     (1000)     2951 2023-03-07 14:32:33.000000 custom-streamlit-1.20.0/streamlit/hello/pages/0_Animation_Demo.py
+-rw-rw-r--   0 dorka     (1000) dorka     (1000)     1738 2023-03-07 14:32:33.000000 custom-streamlit-1.20.0/streamlit/hello/pages/1_Plotting_Demo.py
+-rw-rw-r--   0 dorka     (1000) dorka     (1000)     3821 2023-03-07 14:32:33.000000 custom-streamlit-1.20.0/streamlit/hello/pages/2_Mapping_Demo.py
+-rw-rw-r--   0 dorka     (1000) dorka     (1000)     2522 2023-03-07 14:32:33.000000 custom-streamlit-1.20.0/streamlit/hello/pages/3_DataFrame_Demo.py
+-rw-rw-r--   0 dorka     (1000) dorka     (1000)      987 2023-03-07 14:32:33.000000 custom-streamlit-1.20.0/streamlit/hello/utils.py
+-rw-rw-r--   0 dorka     (1000) dorka     (1000)     3612 2023-03-07 14:32:33.000000 custom-streamlit-1.20.0/streamlit/js_number.py
+-rw-rw-r--   0 dorka     (1000) dorka     (1000)     3987 2023-03-07 14:32:33.000000 custom-streamlit-1.20.0/streamlit/logger.py
+-rw-rw-r--   0 dorka     (1000) dorka     (1000)     3096 2023-03-07 14:32:33.000000 custom-streamlit-1.20.0/streamlit/net_util.py
+drwxrwxr-x   0 dorka     (1000) dorka     (1000)        0 2023-04-07 18:36:01.514182 custom-streamlit-1.20.0/streamlit/proto/
+-rw-rw-r--   0 dorka     (1000) dorka     (1000)     4298 2023-03-08 13:56:40.000000 custom-streamlit-1.20.0/streamlit/proto/Alert_pb2.py
+-rw-rw-r--   0 dorka     (1000) dorka     (1000)     2867 2023-03-08 13:56:40.000000 custom-streamlit-1.20.0/streamlit/proto/AppPage_pb2.py
+-rw-rw-r--   0 dorka     (1000) dorka     (1000)     3282 2023-03-08 13:56:40.000000 custom-streamlit-1.20.0/streamlit/proto/ArrowNamedDataSet_pb2.py
+-rw-rw-r--   0 dorka     (1000) dorka     (1000)     4623 2023-03-08 13:56:40.000000 custom-streamlit-1.20.0/streamlit/proto/ArrowVegaLiteChart_pb2.py
+-rw-rw-r--   0 dorka     (1000) dorka     (1000)     9611 2023-03-08 13:56:40.000000 custom-streamlit-1.20.0/streamlit/proto/Arrow_pb2.py
+-rw-rw-r--   0 dorka     (1000) dorka     (1000)     2435 2023-03-08 13:56:40.000000 custom-streamlit-1.20.0/streamlit/proto/Audio_pb2.py
+-rw-rw-r--   0 dorka     (1000) dorka     (1000)     7278 2023-03-08 13:56:40.000000 custom-streamlit-1.20.0/streamlit/proto/BackMsg_pb2.py
+-rw-rw-r--   0 dorka     (1000) dorka     (1000)     1993 2023-03-08 13:56:40.000000 custom-streamlit-1.20.0/streamlit/proto/Balloons_pb2.py
+-rw-rw-r--   0 dorka     (1000) dorka     (1000)    16064 2023-03-08 13:56:40.000000 custom-streamlit-1.20.0/streamlit/proto/Block_pb2.py
+-rw-rw-r--   0 dorka     (1000) dorka     (1000)     2922 2023-03-08 13:56:40.000000 custom-streamlit-1.20.0/streamlit/proto/BokehChart_pb2.py
+-rw-rw-r--   0 dorka     (1000) dorka     (1000)     5507 2023-03-08 13:56:40.000000 custom-streamlit-1.20.0/streamlit/proto/Button_pb2.py
+-rw-rw-r--   0 dorka     (1000) dorka     (1000)     4669 2023-03-08 13:56:40.000000 custom-streamlit-1.20.0/streamlit/proto/CameraInput_pb2.py
+-rw-rw-r--   0 dorka     (1000) dorka     (1000)     5917 2023-03-08 13:56:40.000000 custom-streamlit-1.20.0/streamlit/proto/Checkbox_pb2.py
+-rw-rw-r--   0 dorka     (1000) dorka     (1000)     3752 2023-03-08 13:56:40.000000 custom-streamlit-1.20.0/streamlit/proto/ClientState_pb2.py
+-rw-rw-r--   0 dorka     (1000) dorka     (1000)     2819 2023-03-08 13:56:40.000000 custom-streamlit-1.20.0/streamlit/proto/Code_pb2.py
+-rw-rw-r--   0 dorka     (1000) dorka     (1000)     6013 2023-03-08 13:56:40.000000 custom-streamlit-1.20.0/streamlit/proto/ColorPicker_pb2.py
+-rw-rw-r--   0 dorka     (1000) dorka     (1000)    12039 2023-03-08 13:56:40.000000 custom-streamlit-1.20.0/streamlit/proto/Common_pb2.py
+-rw-rw-r--   0 dorka     (1000) dorka     (1000)    14749 2023-03-08 13:56:40.000000 custom-streamlit-1.20.0/streamlit/proto/Components_pb2.py
+-rw-rw-r--   0 dorka     (1000) dorka     (1000)    32146 2023-03-08 13:56:40.000000 custom-streamlit-1.20.0/streamlit/proto/DataFrame_pb2.py
+-rw-rw-r--   0 dorka     (1000) dorka     (1000)     7244 2023-03-08 13:56:40.000000 custom-streamlit-1.20.0/streamlit/proto/DateInput_pb2.py
+-rw-rw-r--   0 dorka     (1000) dorka     (1000)     3010 2023-03-08 13:56:40.000000 custom-streamlit-1.20.0/streamlit/proto/DeckGlJsonChart_pb2.py
+-rw-rw-r--   0 dorka     (1000) dorka     (1000)     5385 2023-03-08 13:56:40.000000 custom-streamlit-1.20.0/streamlit/proto/Delta_pb2.py
+-rw-rw-r--   0 dorka     (1000) dorka     (1000)     3764 2023-03-08 13:56:40.000000 custom-streamlit-1.20.0/streamlit/proto/DocString_pb2.py
+-rw-rw-r--   0 dorka     (1000) dorka     (1000)     5223 2023-03-08 13:56:40.000000 custom-streamlit-1.20.0/streamlit/proto/DownloadButton_pb2.py
+-rw-rw-r--   0 dorka     (1000) dorka     (1000)    42409 2023-03-08 13:56:40.000000 custom-streamlit-1.20.0/streamlit/proto/Element_pb2.py
+-rw-rw-r--   0 dorka     (1000) dorka     (1000)     1476 2023-03-08 13:56:40.000000 custom-streamlit-1.20.0/streamlit/proto/Empty_pb2.py
+-rw-rw-r--   0 dorka     (1000) dorka     (1000)     3782 2023-03-08 13:56:40.000000 custom-streamlit-1.20.0/streamlit/proto/Exception_pb2.py
+-rw-rw-r--   0 dorka     (1000) dorka     (1000)     1944 2023-03-08 13:56:40.000000 custom-streamlit-1.20.0/streamlit/proto/Favicon_pb2.py
+-rw-rw-r--   0 dorka     (1000) dorka     (1000)     6066 2023-03-08 13:56:40.000000 custom-streamlit-1.20.0/streamlit/proto/FileUploader_pb2.py
+-rw-rw-r--   0 dorka     (1000) dorka     (1000)    19815 2023-03-08 13:56:40.000000 custom-streamlit-1.20.0/streamlit/proto/ForwardMsg_pb2.py
+-rw-rw-r--   0 dorka     (1000) dorka     (1000)     5383 2023-03-08 13:56:40.000000 custom-streamlit-1.20.0/streamlit/proto/GitInfo_pb2.py
+-rw-rw-r--   0 dorka     (1000) dorka     (1000)     3012 2023-03-08 13:56:40.000000 custom-streamlit-1.20.0/streamlit/proto/GraphVizChart_pb2.py
+-rw-rw-r--   0 dorka     (1000) dorka     (1000)     2823 2023-03-08 13:56:40.000000 custom-streamlit-1.20.0/streamlit/proto/Heading_pb2.py
+-rw-rw-r--   0 dorka     (1000) dorka     (1000)     4633 2023-03-08 13:56:40.000000 custom-streamlit-1.20.0/streamlit/proto/IFrame_pb2.py
+-rw-rw-r--   0 dorka     (1000) dorka     (1000)     4509 2023-03-08 13:56:40.000000 custom-streamlit-1.20.0/streamlit/proto/Image_pb2.py
+-rw-rw-r--   0 dorka     (1000) dorka     (1000)     2334 2023-03-08 13:56:40.000000 custom-streamlit-1.20.0/streamlit/proto/Json_pb2.py
+-rw-rw-r--   0 dorka     (1000) dorka     (1000)     3567 2023-03-08 13:56:40.000000 custom-streamlit-1.20.0/streamlit/proto/LabelVisibilityMessage_pb2.py
+-rw-rw-r--   0 dorka     (1000) dorka     (1000)     4839 2023-03-08 13:56:40.000000 custom-streamlit-1.20.0/streamlit/proto/Markdown_pb2.py
+-rw-rw-r--   0 dorka     (1000) dorka     (1000)     7304 2023-03-08 13:56:40.000000 custom-streamlit-1.20.0/streamlit/proto/Metric_pb2.py
+-rw-rw-r--   0 dorka     (1000) dorka     (1000)     6874 2023-03-08 13:56:40.000000 custom-streamlit-1.20.0/streamlit/proto/MultiSelect_pb2.py
+-rw-rw-r--   0 dorka     (1000) dorka     (1000)     3210 2023-03-08 13:56:40.000000 custom-streamlit-1.20.0/streamlit/proto/NamedDataSet_pb2.py
+-rw-rw-r--   0 dorka     (1000) dorka     (1000)    22768 2023-03-08 13:56:40.000000 custom-streamlit-1.20.0/streamlit/proto/NewSession_pb2.py
+-rw-rw-r--   0 dorka     (1000) dorka     (1000)    10165 2023-03-08 13:56:40.000000 custom-streamlit-1.20.0/streamlit/proto/NumberInput_pb2.py
+-rw-rw-r--   0 dorka     (1000) dorka     (1000)     9326 2023-03-08 13:56:40.000000 custom-streamlit-1.20.0/streamlit/proto/PageConfig_pb2.py
+-rw-rw-r--   0 dorka     (1000) dorka     (1000)     1978 2023-03-08 13:56:40.000000 custom-streamlit-1.20.0/streamlit/proto/PageInfo_pb2.py
+-rw-rw-r--   0 dorka     (1000) dorka     (1000)     2029 2023-03-08 13:56:40.000000 custom-streamlit-1.20.0/streamlit/proto/PageNotFound_pb2.py
+-rw-rw-r--   0 dorka     (1000) dorka     (1000)    10218 2023-03-08 13:56:40.000000 custom-streamlit-1.20.0/streamlit/proto/PageProfile_pb2.py
+-rw-rw-r--   0 dorka     (1000) dorka     (1000)     2322 2023-03-08 13:56:40.000000 custom-streamlit-1.20.0/streamlit/proto/PagesChanged_pb2.py
+-rw-rw-r--   0 dorka     (1000) dorka     (1000)     5670 2023-03-08 13:56:40.000000 custom-streamlit-1.20.0/streamlit/proto/PlotlyChart_pb2.py
+-rw-rw-r--   0 dorka     (1000) dorka     (1000)     2378 2023-03-08 13:56:40.000000 custom-streamlit-1.20.0/streamlit/proto/Progress_pb2.py
+-rw-rw-r--   0 dorka     (1000) dorka     (1000)     6700 2023-03-08 13:56:40.000000 custom-streamlit-1.20.0/streamlit/proto/Radio_pb2.py
+-rw-rw-r--   0 dorka     (1000) dorka     (1000)     1760 2023-03-08 13:56:40.000000 custom-streamlit-1.20.0/streamlit/proto/RootContainer_pb2.py
+-rw-rw-r--   0 dorka     (1000) dorka     (1000)     6360 2023-03-08 13:56:40.000000 custom-streamlit-1.20.0/streamlit/proto/Selectbox_pb2.py
+-rw-rw-r--   0 dorka     (1000) dorka     (1000)     4305 2023-03-08 13:56:40.000000 custom-streamlit-1.20.0/streamlit/proto/SessionEvent_pb2.py
+-rw-rw-r--   0 dorka     (1000) dorka     (1000)     2513 2023-03-08 13:56:40.000000 custom-streamlit-1.20.0/streamlit/proto/SessionStatus_pb2.py
+-rw-rw-r--   0 dorka     (1000) dorka     (1000)    11535 2023-03-08 13:56:40.000000 custom-streamlit-1.20.0/streamlit/proto/Slider_pb2.py
+-rw-rw-r--   0 dorka     (1000) dorka     (1000)     1884 2023-03-08 13:56:40.000000 custom-streamlit-1.20.0/streamlit/proto/Snow_pb2.py
+-rw-rw-r--   0 dorka     (1000) dorka     (1000)     1941 2023-03-08 13:56:40.000000 custom-streamlit-1.20.0/streamlit/proto/Spinner_pb2.py
+-rw-rw-r--   0 dorka     (1000) dorka     (1000)     7264 2023-03-08 13:56:40.000000 custom-streamlit-1.20.0/streamlit/proto/TextArea_pb2.py
+-rw-rw-r--   0 dorka     (1000) dorka     (1000)     8686 2023-03-08 13:56:40.000000 custom-streamlit-1.20.0/streamlit/proto/TextInput_pb2.py
+-rw-rw-r--   0 dorka     (1000) dorka     (1000)     1896 2023-03-08 13:56:40.000000 custom-streamlit-1.20.0/streamlit/proto/Text_pb2.py
+-rw-rw-r--   0 dorka     (1000) dorka     (1000)     5961 2023-03-08 13:56:40.000000 custom-streamlit-1.20.0/streamlit/proto/TimeInput_pb2.py
+-rw-rw-r--   0 dorka     (1000) dorka     (1000)     4048 2023-03-08 13:56:40.000000 custom-streamlit-1.20.0/streamlit/proto/VegaLiteChart_pb2.py
+-rw-rw-r--   0 dorka     (1000) dorka     (1000)     3953 2023-03-08 13:56:40.000000 custom-streamlit-1.20.0/streamlit/proto/Video_pb2.py
+-rw-rw-r--   0 dorka     (1000) dorka     (1000)    12593 2023-03-08 13:56:40.000000 custom-streamlit-1.20.0/streamlit/proto/WidgetStates_pb2.py
+-rw-rw-r--   0 dorka     (1000) dorka     (1000)      663 2023-03-07 14:32:33.000000 custom-streamlit-1.20.0/streamlit/proto/__init__.py
+-rw-rw-r--   0 dorka     (1000) dorka     (1000)    45888 2023-03-08 13:56:40.000000 custom-streamlit-1.20.0/streamlit/proto/openmetrics_data_model_pb2.py
+-rw-rw-r--   0 dorka     (1000) dorka     (1000)        0 2023-03-07 14:32:33.000000 custom-streamlit-1.20.0/streamlit/py.typed
+drwxrwxr-x   0 dorka     (1000) dorka     (1000)        0 2023-04-07 18:36:01.518182 custom-streamlit-1.20.0/streamlit/runtime/
+-rw-rw-r--   0 dorka     (1000) dorka     (1000)     1604 2023-03-07 14:32:33.000000 custom-streamlit-1.20.0/streamlit/runtime/__init__.py
+-rw-rw-r--   0 dorka     (1000) dorka     (1000)    31650 2023-03-07 14:32:33.000000 custom-streamlit-1.20.0/streamlit/runtime/app_session.py
+drwxrwxr-x   0 dorka     (1000) dorka     (1000)        0 2023-04-07 18:36:01.518182 custom-streamlit-1.20.0/streamlit/runtime/caching/
+-rw-rw-r--   0 dorka     (1000) dorka     (1000)     4700 2023-03-07 14:32:33.000000 custom-streamlit-1.20.0/streamlit/runtime/caching/__init__.py
+-rw-rw-r--   0 dorka     (1000) dorka     (1000)    23805 2023-03-07 14:32:33.000000 custom-streamlit-1.20.0/streamlit/runtime/caching/cache_data_api.py
+-rw-rw-r--   0 dorka     (1000) dorka     (1000)     5992 2023-03-07 14:32:33.000000 custom-streamlit-1.20.0/streamlit/runtime/caching/cache_errors.py
+-rw-rw-r--   0 dorka     (1000) dorka     (1000)    18797 2023-03-07 14:32:33.000000 custom-streamlit-1.20.0/streamlit/runtime/caching/cache_resource_api.py
+-rw-rw-r--   0 dorka     (1000) dorka     (1000)     1090 2023-03-07 14:32:33.000000 custom-streamlit-1.20.0/streamlit/runtime/caching/cache_type.py
+-rw-rw-r--   0 dorka     (1000) dorka     (1000)    16653 2023-03-07 14:32:33.000000 custom-streamlit-1.20.0/streamlit/runtime/caching/cache_utils.py
+-rw-rw-r--   0 dorka     (1000) dorka     (1000)    18475 2023-03-07 14:32:33.000000 custom-streamlit-1.20.0/streamlit/runtime/caching/cached_message_replay.py
+-rw-rw-r--   0 dorka     (1000) dorka     (1000)    13106 2023-03-07 14:32:33.000000 custom-streamlit-1.20.0/streamlit/runtime/caching/hashing.py
+drwxrwxr-x   0 dorka     (1000) dorka     (1000)        0 2023-04-07 18:36:01.518182 custom-streamlit-1.20.0/streamlit/runtime/caching/storage/
+-rw-rw-r--   0 dorka     (1000) dorka     (1000)     1217 2023-03-07 14:32:33.000000 custom-streamlit-1.20.0/streamlit/runtime/caching/storage/__init__.py
+-rw-rw-r--   0 dorka     (1000) dorka     (1000)     7764 2023-03-07 14:32:33.000000 custom-streamlit-1.20.0/streamlit/runtime/caching/storage/cache_storage_protocol.py
+-rw-rw-r--   0 dorka     (1000) dorka     (1000)     1940 2023-03-07 14:32:33.000000 custom-streamlit-1.20.0/streamlit/runtime/caching/storage/dummy_cache_storage.py
+-rw-rw-r--   0 dorka     (1000) dorka     (1000)     5384 2023-03-07 14:32:33.000000 custom-streamlit-1.20.0/streamlit/runtime/caching/storage/in_memory_cache_storage_wrapper.py
+-rw-rw-r--   0 dorka     (1000) dorka     (1000)     7609 2023-03-07 14:32:33.000000 custom-streamlit-1.20.0/streamlit/runtime/caching/storage/local_disk_cache_storage.py
+-rw-rw-r--   0 dorka     (1000) dorka     (1000)     9401 2023-03-07 14:32:33.000000 custom-streamlit-1.20.0/streamlit/runtime/credentials.py
+-rw-rw-r--   0 dorka     (1000) dorka     (1000)     8790 2023-03-07 14:32:33.000000 custom-streamlit-1.20.0/streamlit/runtime/forward_msg_cache.py
+-rw-rw-r--   0 dorka     (1000) dorka     (1000)     5549 2023-03-07 14:32:33.000000 custom-streamlit-1.20.0/streamlit/runtime/forward_msg_queue.py
+drwxrwxr-x   0 dorka     (1000) dorka     (1000)        0 2023-04-07 18:36:01.518182 custom-streamlit-1.20.0/streamlit/runtime/legacy_caching/
+-rw-rw-r--   0 dorka     (1000) dorka     (1000)      987 2023-03-07 14:32:33.000000 custom-streamlit-1.20.0/streamlit/runtime/legacy_caching/__init__.py
+-rw-rw-r--   0 dorka     (1000) dorka     (1000)    30548 2023-03-07 14:32:33.000000 custom-streamlit-1.20.0/streamlit/runtime/legacy_caching/caching.py
+-rw-rw-r--   0 dorka     (1000) dorka     (1000)    35123 2023-03-07 14:32:33.000000 custom-streamlit-1.20.0/streamlit/runtime/legacy_caching/hashing.py
+-rw-rw-r--   0 dorka     (1000) dorka     (1000)     8489 2023-03-07 14:32:33.000000 custom-streamlit-1.20.0/streamlit/runtime/media_file_manager.py
+-rw-rw-r--   0 dorka     (1000) dorka     (1000)     4396 2023-03-07 14:32:33.000000 custom-streamlit-1.20.0/streamlit/runtime/media_file_storage.py
+-rw-rw-r--   0 dorka     (1000) dorka     (1000)     6251 2023-03-07 14:32:33.000000 custom-streamlit-1.20.0/streamlit/runtime/memory_media_file_storage.py
+-rw-rw-r--   0 dorka     (1000) dorka     (1000)     2918 2023-03-07 14:32:33.000000 custom-streamlit-1.20.0/streamlit/runtime/memory_session_storage.py
+-rw-rw-r--   0 dorka     (1000) dorka     (1000)    12208 2023-03-07 14:32:33.000000 custom-streamlit-1.20.0/streamlit/runtime/metrics_util.py
+-rw-rw-r--   0 dorka     (1000) dorka     (1000)    26047 2023-03-07 15:27:59.000000 custom-streamlit-1.20.0/streamlit/runtime/runtime.py
+-rw-rw-r--   0 dorka     (1000) dorka     (1000)     3790 2023-03-07 14:32:33.000000 custom-streamlit-1.20.0/streamlit/runtime/runtime_util.py
+-rw-rw-r--   0 dorka     (1000) dorka     (1000)     1703 2023-03-07 14:32:33.000000 custom-streamlit-1.20.0/streamlit/runtime/script_data.py
+drwxrwxr-x   0 dorka     (1000) dorka     (1000)        0 2023-04-07 18:36:01.518182 custom-streamlit-1.20.0/streamlit/runtime/scriptrunner/
+-rw-rw-r--   0 dorka     (1000) dorka     (1000)     1439 2023-03-07 14:32:33.000000 custom-streamlit-1.20.0/streamlit/runtime/scriptrunner/__init__.py
+-rw-rw-r--   0 dorka     (1000) dorka     (1000)     6079 2023-03-07 14:32:33.000000 custom-streamlit-1.20.0/streamlit/runtime/scriptrunner/magic.py
+-rw-rw-r--   0 dorka     (1000) dorka     (1000)     1015 2023-03-07 14:32:33.000000 custom-streamlit-1.20.0/streamlit/runtime/scriptrunner/magic_funcs.py
+-rw-rw-r--   0 dorka     (1000) dorka     (1000)     6965 2023-03-07 14:32:33.000000 custom-streamlit-1.20.0/streamlit/runtime/scriptrunner/script_requests.py
+-rw-rw-r--   0 dorka     (1000) dorka     (1000)     6242 2023-03-07 14:32:33.000000 custom-streamlit-1.20.0/streamlit/runtime/scriptrunner/script_run_context.py
+-rw-rw-r--   0 dorka     (1000) dorka     (1000)    26966 2023-03-07 14:32:33.000000 custom-streamlit-1.20.0/streamlit/runtime/scriptrunner/script_runner.py
+-rw-rw-r--   0 dorka     (1000) dorka     (1000)    10630 2023-03-07 14:32:33.000000 custom-streamlit-1.20.0/streamlit/runtime/secrets.py
+-rw-rw-r--   0 dorka     (1000) dorka     (1000)    12404 2023-03-07 14:32:33.000000 custom-streamlit-1.20.0/streamlit/runtime/session_manager.py
+drwxrwxr-x   0 dorka     (1000) dorka     (1000)        0 2023-04-07 18:36:01.522182 custom-streamlit-1.20.0/streamlit/runtime/state/
+-rw-rw-r--   0 dorka     (1000) dorka     (1000)     1733 2023-03-07 14:32:33.000000 custom-streamlit-1.20.0/streamlit/runtime/state/__init__.py
+-rw-rw-r--   0 dorka     (1000) dorka     (1000)     6512 2023-03-07 14:32:33.000000 custom-streamlit-1.20.0/streamlit/runtime/state/common.py
+-rw-rw-r--   0 dorka     (1000) dorka     (1000)     4624 2023-03-07 14:32:33.000000 custom-streamlit-1.20.0/streamlit/runtime/state/safe_session_state.py
+-rw-rw-r--   0 dorka     (1000) dorka     (1000)    23365 2023-03-07 14:32:33.000000 custom-streamlit-1.20.0/streamlit/runtime/state/session_state.py
+-rw-rw-r--   0 dorka     (1000) dorka     (1000)     5098 2023-03-07 14:32:33.000000 custom-streamlit-1.20.0/streamlit/runtime/state/session_state_proxy.py
+-rw-rw-r--   0 dorka     (1000) dorka     (1000)    10808 2023-03-07 14:32:33.000000 custom-streamlit-1.20.0/streamlit/runtime/state/widgets.py
+-rw-rw-r--   0 dorka     (1000) dorka     (1000)     3044 2023-03-07 14:32:33.000000 custom-streamlit-1.20.0/streamlit/runtime/stats.py
+-rw-rw-r--   0 dorka     (1000) dorka     (1000)    11423 2023-03-07 14:32:33.000000 custom-streamlit-1.20.0/streamlit/runtime/uploaded_file_manager.py
+-rw-rw-r--   0 dorka     (1000) dorka     (1000)     5844 2023-03-07 14:32:33.000000 custom-streamlit-1.20.0/streamlit/runtime/websocket_session_manager.py
+-rw-rw-r--   0 dorka     (1000) dorka     (1000)     5688 2023-03-07 14:32:33.000000 custom-streamlit-1.20.0/streamlit/source_util.py
+-rw-rw-r--   0 dorka     (1000) dorka     (1000)     5408 2023-03-07 14:32:33.000000 custom-streamlit-1.20.0/streamlit/string_util.py
+-rw-rw-r--   0 dorka     (1000) dorka     (1000)     1594 2023-03-07 14:32:33.000000 custom-streamlit-1.20.0/streamlit/temporary_directory.py
+drwxrwxr-x   0 dorka     (1000) dorka     (1000)        0 2023-04-07 18:36:01.522182 custom-streamlit-1.20.0/streamlit/testing/
+-rw-rw-r--   0 dorka     (1000) dorka     (1000)      611 2023-03-07 14:32:33.000000 custom-streamlit-1.20.0/streamlit/testing/__init__.py
+-rw-rw-r--   0 dorka     (1000) dorka     (1000)    28101 2023-03-07 14:32:33.000000 custom-streamlit-1.20.0/streamlit/testing/element_tree.py
+-rw-rw-r--   0 dorka     (1000) dorka     (1000)     5300 2023-03-07 14:32:33.000000 custom-streamlit-1.20.0/streamlit/testing/local_script_runner.py
+-rw-rw-r--   0 dorka     (1000) dorka     (1000)     2852 2023-03-07 14:32:33.000000 custom-streamlit-1.20.0/streamlit/testing/script_interactions.py
+-rw-rw-r--   0 dorka     (1000) dorka     (1000)    31285 2023-03-07 14:32:33.000000 custom-streamlit-1.20.0/streamlit/type_util.py
+-rw-rw-r--   0 dorka     (1000) dorka     (1000)     2289 2023-03-07 14:32:33.000000 custom-streamlit-1.20.0/streamlit/url_util.py
+-rw-rw-r--   0 dorka     (1000) dorka     (1000)     1981 2023-03-07 14:32:33.000000 custom-streamlit-1.20.0/streamlit/user_info.py
+-rw-rw-r--   0 dorka     (1000) dorka     (1000)     5581 2023-03-07 14:32:33.000000 custom-streamlit-1.20.0/streamlit/util.py
+drwxrwxr-x   0 dorka     (1000) dorka     (1000)        0 2023-04-07 18:36:01.522182 custom-streamlit-1.20.0/streamlit/vendor/
+-rw-rw-r--   0 dorka     (1000) dorka     (1000)        0 2023-03-07 14:32:33.000000 custom-streamlit-1.20.0/streamlit/vendor/__init__.py
+drwxrwxr-x   0 dorka     (1000) dorka     (1000)        0 2023-04-07 18:36:01.522182 custom-streamlit-1.20.0/streamlit/vendor/ipython/
+-rw-rw-r--   0 dorka     (1000) dorka     (1000)        0 2023-03-07 14:32:33.000000 custom-streamlit-1.20.0/streamlit/vendor/ipython/__init__.py
+-rw-rw-r--   0 dorka     (1000) dorka     (1000)     2746 2023-03-07 14:32:33.000000 custom-streamlit-1.20.0/streamlit/vendor/ipython/modified_sys_path.py
+-rw-rw-r--   0 dorka     (1000) dorka     (1000)     3347 2023-03-07 14:32:33.000000 custom-streamlit-1.20.0/streamlit/version.py
+drwxrwxr-x   0 dorka     (1000) dorka     (1000)        0 2023-04-07 18:36:01.526182 custom-streamlit-1.20.0/streamlit/watcher/
+-rw-rw-r--   0 dorka     (1000) dorka     (1000)      963 2023-03-07 14:32:33.000000 custom-streamlit-1.20.0/streamlit/watcher/__init__.py
+-rw-rw-r--   0 dorka     (1000) dorka     (1000)    13689 2023-03-07 14:32:33.000000 custom-streamlit-1.20.0/streamlit/watcher/event_based_path_watcher.py
+-rw-rw-r--   0 dorka     (1000) dorka     (1000)     7617 2023-03-07 14:32:33.000000 custom-streamlit-1.20.0/streamlit/watcher/local_sources_watcher.py
+-rw-rw-r--   0 dorka     (1000) dorka     (1000)     5673 2023-03-07 14:32:33.000000 custom-streamlit-1.20.0/streamlit/watcher/path_watcher.py
+-rw-rw-r--   0 dorka     (1000) dorka     (1000)     3570 2023-03-07 14:32:33.000000 custom-streamlit-1.20.0/streamlit/watcher/polling_path_watcher.py
+-rw-rw-r--   0 dorka     (1000) dorka     (1000)     5134 2023-03-07 14:32:33.000000 custom-streamlit-1.20.0/streamlit/watcher/util.py
+drwxrwxr-x   0 dorka     (1000) dorka     (1000)        0 2023-04-07 18:36:01.526182 custom-streamlit-1.20.0/streamlit/web/
+-rw-rw-r--   0 dorka     (1000) dorka     (1000)      611 2023-03-07 14:32:33.000000 custom-streamlit-1.20.0/streamlit/web/__init__.py
+-rw-rw-r--   0 dorka     (1000) dorka     (1000)    14779 2023-03-07 14:32:33.000000 custom-streamlit-1.20.0/streamlit/web/bootstrap.py
+-rw-rw-r--   0 dorka     (1000) dorka     (1000)     1117 2023-03-07 14:32:33.000000 custom-streamlit-1.20.0/streamlit/web/cache_storage_manager_config.py
+-rw-rw-r--   0 dorka     (1000) dorka     (1000)    10384 2023-03-07 14:32:33.000000 custom-streamlit-1.20.0/streamlit/web/cli.py
+drwxrwxr-x   0 dorka     (1000) dorka     (1000)        0 2023-04-07 18:36:01.530182 custom-streamlit-1.20.0/streamlit/web/server/
+-rw-rw-r--   0 dorka     (1000) dorka     (1000)     1047 2023-03-07 14:32:33.000000 custom-streamlit-1.20.0/streamlit/web/server/__init__.py
+-rw-rw-r--   0 dorka     (1000) dorka     (1000)     2666 2023-03-07 14:32:33.000000 custom-streamlit-1.20.0/streamlit/web/server/app_static_file_handler.py
+-rw-rw-r--   0 dorka     (1000) dorka     (1000)     7671 2023-03-07 14:32:33.000000 custom-streamlit-1.20.0/streamlit/web/server/browser_websocket_handler.py
+-rw-rw-r--   0 dorka     (1000) dorka     (1000)     4205 2023-03-07 14:32:33.000000 custom-streamlit-1.20.0/streamlit/web/server/component_request_handler.py
+-rw-rw-r--   0 dorka     (1000) dorka     (1000)     5574 2023-03-07 14:32:33.000000 custom-streamlit-1.20.0/streamlit/web/server/media_file_handler.py
+-rw-rw-r--   0 dorka     (1000) dorka     (1000)     9303 2023-03-07 14:32:33.000000 custom-streamlit-1.20.0/streamlit/web/server/routes.py
+-rw-rw-r--   0 dorka     (1000) dorka     (1000)    14583 2023-03-07 14:32:33.000000 custom-streamlit-1.20.0/streamlit/web/server/server.py
+-rw-rw-r--   0 dorka     (1000) dorka     (1000)     4033 2023-03-07 14:32:33.000000 custom-streamlit-1.20.0/streamlit/web/server/server_util.py
+-rw-rw-r--   0 dorka     (1000) dorka     (1000)     3405 2023-03-07 14:32:33.000000 custom-streamlit-1.20.0/streamlit/web/server/stats_request_handler.py
+-rw-rw-r--   0 dorka     (1000) dorka     (1000)     5964 2023-03-07 14:32:33.000000 custom-streamlit-1.20.0/streamlit/web/server/upload_file_request_handler.py
+-rw-rw-r--   0 dorka     (1000) dorka     (1000)     1867 2023-03-07 14:32:33.000000 custom-streamlit-1.20.0/streamlit/web/server/websocket_headers.py
+drwxrwxr-x   0 dorka     (1000) dorka     (1000)        0 2023-04-07 18:36:01.530182 custom-streamlit-1.20.0/tests/
+-rw-rw-r--   0 dorka     (1000) dorka     (1000)     4900 2023-03-07 14:32:33.000000 custom-streamlit-1.20.0/tests/testutil.py
```

### Comparing `custom-streamlit-1.19.0/Pipfile` & `custom-streamlit-1.20.0/Pipfile`

 * *Files identical despite different names*

### Comparing `custom-streamlit-1.19.0/bin/streamlit.cmd` & `custom-streamlit-1.20.0/bin/streamlit.cmd`

 * *Files identical despite different names*

### Comparing `custom-streamlit-1.19.0/custom_streamlit.egg-info/SOURCES.txt` & `custom-streamlit-1.20.0/custom_streamlit.egg-info/SOURCES.txt`

 * *Files identical despite different names*

### Comparing `custom-streamlit-1.19.0/setup.py` & `custom-streamlit-1.20.0/setup.py`

 * *Files 0% similar despite different names*

```diff
@@ -17,15 +17,15 @@
 from pathlib import Path
 
 import setuptools
 from setuptools.command.install import install
 
 THIS_DIRECTORY = Path(__file__).parent
 
-VERSION = "1.19.0"  # PEP-440
+VERSION = "1.20.0"  # PEP-440
 
 NAME = "custom-streamlit"
 
 # IMPORTANT: We should try very hard *not* to add dependencies to Streamlit.
 # And if you do add one, make the required version as general as possible.
 # But include relevant lower bounds for any features we use from our dependencies.
 INSTALL_REQUIRES = [
```

### Comparing `custom-streamlit-1.19.0/streamlit/__init__.py` & `custom-streamlit-1.20.0/streamlit/__init__.py`

 * *Files identical despite different names*

### Comparing `custom-streamlit-1.19.0/streamlit/__main__.py` & `custom-streamlit-1.20.0/streamlit/__main__.py`

 * *Files identical despite different names*

### Comparing `custom-streamlit-1.19.0/streamlit/case_converters.py` & `custom-streamlit-1.20.0/streamlit/case_converters.py`

 * *Files identical despite different names*

### Comparing `custom-streamlit-1.19.0/streamlit/code_util.py` & `custom-streamlit-1.20.0/streamlit/code_util.py`

 * *Files identical despite different names*

### Comparing `custom-streamlit-1.19.0/streamlit/commands/__init__.py` & `custom-streamlit-1.20.0/streamlit/commands/__init__.py`

 * *Files identical despite different names*

### Comparing `custom-streamlit-1.19.0/streamlit/commands/execution_control.py` & `custom-streamlit-1.20.0/streamlit/commands/execution_control.py`

 * *Files identical despite different names*

### Comparing `custom-streamlit-1.19.0/streamlit/commands/page_config.py` & `custom-streamlit-1.20.0/streamlit/commands/page_config.py`

 * *Files identical despite different names*

### Comparing `custom-streamlit-1.19.0/streamlit/commands/query_params.py` & `custom-streamlit-1.20.0/streamlit/commands/query_params.py`

 * *Files identical despite different names*

### Comparing `custom-streamlit-1.19.0/streamlit/components/__init__.py` & `custom-streamlit-1.20.0/streamlit/components/__init__.py`

 * *Files identical despite different names*

### Comparing `custom-streamlit-1.19.0/streamlit/components/v1/__init__.py` & `custom-streamlit-1.20.0/streamlit/components/v1/__init__.py`

 * *Files identical despite different names*

### Comparing `custom-streamlit-1.19.0/streamlit/components/v1/component_arrow.py` & `custom-streamlit-1.20.0/streamlit/components/v1/component_arrow.py`

 * *Files identical despite different names*

### Comparing `custom-streamlit-1.19.0/streamlit/components/v1/components.py` & `custom-streamlit-1.20.0/streamlit/components/v1/components.py`

 * *Files identical despite different names*

### Comparing `custom-streamlit-1.19.0/streamlit/config.py` & `custom-streamlit-1.20.0/streamlit/config.py`

 * *Files identical despite different names*

### Comparing `custom-streamlit-1.19.0/streamlit/config_option.py` & `custom-streamlit-1.20.0/streamlit/config_option.py`

 * *Files identical despite different names*

### Comparing `custom-streamlit-1.19.0/streamlit/config_util.py` & `custom-streamlit-1.20.0/streamlit/config_util.py`

 * *Files identical despite different names*

### Comparing `custom-streamlit-1.19.0/streamlit/cursor.py` & `custom-streamlit-1.20.0/streamlit/cursor.py`

 * *Files identical despite different names*

### Comparing `custom-streamlit-1.19.0/streamlit/delta_generator.py` & `custom-streamlit-1.20.0/streamlit/delta_generator.py`

 * *Files identical despite different names*

### Comparing `custom-streamlit-1.19.0/streamlit/deprecation_util.py` & `custom-streamlit-1.20.0/streamlit/deprecation_util.py`

 * *Files identical despite different names*

### Comparing `custom-streamlit-1.19.0/streamlit/development.py` & `custom-streamlit-1.20.0/streamlit/development.py`

 * *Files identical despite different names*

### Comparing `custom-streamlit-1.19.0/streamlit/echo.py` & `custom-streamlit-1.20.0/streamlit/echo.py`

 * *Files identical despite different names*

### Comparing `custom-streamlit-1.19.0/streamlit/elements/__init__.py` & `custom-streamlit-1.20.0/streamlit/elements/__init__.py`

 * *Files identical despite different names*

### Comparing `custom-streamlit-1.19.0/streamlit/elements/alert.py` & `custom-streamlit-1.20.0/streamlit/elements/alert.py`

 * *Files identical despite different names*

### Comparing `custom-streamlit-1.19.0/streamlit/elements/arrow.py` & `custom-streamlit-1.20.0/streamlit/elements/arrow.py`

 * *Files identical despite different names*

### Comparing `custom-streamlit-1.19.0/streamlit/elements/arrow_altair.py` & `custom-streamlit-1.20.0/streamlit/elements/arrow_altair.py`

 * *Files identical despite different names*

### Comparing `custom-streamlit-1.19.0/streamlit/elements/arrow_vega_lite.py` & `custom-streamlit-1.20.0/streamlit/elements/arrow_vega_lite.py`

 * *Files identical despite different names*

### Comparing `custom-streamlit-1.19.0/streamlit/elements/balloons.py` & `custom-streamlit-1.20.0/streamlit/elements/balloons.py`

 * *Files identical despite different names*

### Comparing `custom-streamlit-1.19.0/streamlit/elements/bokeh_chart.py` & `custom-streamlit-1.20.0/streamlit/elements/bokeh_chart.py`

 * *Files identical despite different names*

### Comparing `custom-streamlit-1.19.0/streamlit/elements/button.py` & `custom-streamlit-1.20.0/streamlit/elements/button.py`

 * *Files identical despite different names*

### Comparing `custom-streamlit-1.19.0/streamlit/elements/camera_input.py` & `custom-streamlit-1.20.0/streamlit/elements/camera_input.py`

 * *Files identical despite different names*

### Comparing `custom-streamlit-1.19.0/streamlit/elements/checkbox.py` & `custom-streamlit-1.20.0/streamlit/elements/checkbox.py`

 * *Files identical despite different names*

### Comparing `custom-streamlit-1.19.0/streamlit/elements/code.py` & `custom-streamlit-1.20.0/streamlit/elements/code.py`

 * *Files identical despite different names*

### Comparing `custom-streamlit-1.19.0/streamlit/elements/color_picker.py` & `custom-streamlit-1.20.0/streamlit/elements/color_picker.py`

 * *Files identical despite different names*

### Comparing `custom-streamlit-1.19.0/streamlit/elements/data_editor.py` & `custom-streamlit-1.20.0/streamlit/elements/data_editor.py`

 * *Files identical despite different names*

### Comparing `custom-streamlit-1.19.0/streamlit/elements/dataframe_selector.py` & `custom-streamlit-1.20.0/streamlit/elements/dataframe_selector.py`

 * *Files identical despite different names*

### Comparing `custom-streamlit-1.19.0/streamlit/elements/deck_gl_json_chart.py` & `custom-streamlit-1.20.0/streamlit/elements/deck_gl_json_chart.py`

 * *Files identical despite different names*

### Comparing `custom-streamlit-1.19.0/streamlit/elements/doc_string.py` & `custom-streamlit-1.20.0/streamlit/elements/doc_string.py`

 * *Files identical despite different names*

### Comparing `custom-streamlit-1.19.0/streamlit/elements/empty.py` & `custom-streamlit-1.20.0/streamlit/elements/empty.py`

 * *Files identical despite different names*

### Comparing `custom-streamlit-1.19.0/streamlit/elements/exception.py` & `custom-streamlit-1.20.0/streamlit/elements/exception.py`

 * *Files identical despite different names*

### Comparing `custom-streamlit-1.19.0/streamlit/elements/file_uploader.py` & `custom-streamlit-1.20.0/streamlit/elements/file_uploader.py`

 * *Files identical despite different names*

### Comparing `custom-streamlit-1.19.0/streamlit/elements/form.py` & `custom-streamlit-1.20.0/streamlit/elements/form.py`

 * *Files identical despite different names*

### Comparing `custom-streamlit-1.19.0/streamlit/elements/graphviz_chart.py` & `custom-streamlit-1.20.0/streamlit/elements/graphviz_chart.py`

 * *Files identical despite different names*

### Comparing `custom-streamlit-1.19.0/streamlit/elements/heading.py` & `custom-streamlit-1.20.0/streamlit/elements/heading.py`

 * *Files identical despite different names*

### Comparing `custom-streamlit-1.19.0/streamlit/elements/iframe.py` & `custom-streamlit-1.20.0/streamlit/elements/iframe.py`

 * *Files identical despite different names*

### Comparing `custom-streamlit-1.19.0/streamlit/elements/image.py` & `custom-streamlit-1.20.0/streamlit/elements/image.py`

 * *Files identical despite different names*

### Comparing `custom-streamlit-1.19.0/streamlit/elements/json.py` & `custom-streamlit-1.20.0/streamlit/elements/json.py`

 * *Files identical despite different names*

### Comparing `custom-streamlit-1.19.0/streamlit/elements/layouts.py` & `custom-streamlit-1.20.0/streamlit/elements/layouts.py`

 * *Files identical despite different names*

### Comparing `custom-streamlit-1.19.0/streamlit/elements/legacy_altair.py` & `custom-streamlit-1.20.0/streamlit/elements/legacy_altair.py`

 * *Files identical despite different names*

### Comparing `custom-streamlit-1.19.0/streamlit/elements/legacy_data_frame.py` & `custom-streamlit-1.20.0/streamlit/elements/legacy_data_frame.py`

 * *Files identical despite different names*

### Comparing `custom-streamlit-1.19.0/streamlit/elements/legacy_vega_lite.py` & `custom-streamlit-1.20.0/streamlit/elements/legacy_vega_lite.py`

 * *Files identical despite different names*

### Comparing `custom-streamlit-1.19.0/streamlit/elements/lib/__init__.py` & `custom-streamlit-1.20.0/streamlit/elements/lib/__init__.py`

 * *Files identical despite different names*

### Comparing `custom-streamlit-1.19.0/streamlit/elements/lib/dicttools.py` & `custom-streamlit-1.20.0/streamlit/elements/lib/dicttools.py`

 * *Files identical despite different names*

### Comparing `custom-streamlit-1.19.0/streamlit/elements/lib/streamlit_plotly_theme.py` & `custom-streamlit-1.20.0/streamlit/elements/lib/streamlit_plotly_theme.py`

 * *Files identical despite different names*

### Comparing `custom-streamlit-1.19.0/streamlit/elements/map.py` & `custom-streamlit-1.20.0/streamlit/elements/map.py`

 * *Files identical despite different names*

### Comparing `custom-streamlit-1.19.0/streamlit/elements/markdown.py` & `custom-streamlit-1.20.0/streamlit/elements/markdown.py`

 * *Files identical despite different names*

### Comparing `custom-streamlit-1.19.0/streamlit/elements/media.py` & `custom-streamlit-1.20.0/streamlit/elements/media.py`

 * *Files identical despite different names*

### Comparing `custom-streamlit-1.19.0/streamlit/elements/metric.py` & `custom-streamlit-1.20.0/streamlit/elements/metric.py`

 * *Files identical despite different names*

### Comparing `custom-streamlit-1.19.0/streamlit/elements/multiselect.py` & `custom-streamlit-1.20.0/streamlit/elements/multiselect.py`

 * *Files identical despite different names*

### Comparing `custom-streamlit-1.19.0/streamlit/elements/number_input.py` & `custom-streamlit-1.20.0/streamlit/elements/number_input.py`

 * *Files identical despite different names*

### Comparing `custom-streamlit-1.19.0/streamlit/elements/plotly_chart.py` & `custom-streamlit-1.20.0/streamlit/elements/plotly_chart.py`

 * *Files identical despite different names*

### Comparing `custom-streamlit-1.19.0/streamlit/elements/progress.py` & `custom-streamlit-1.20.0/streamlit/elements/progress.py`

 * *Files identical despite different names*

### Comparing `custom-streamlit-1.19.0/streamlit/elements/pyplot.py` & `custom-streamlit-1.20.0/streamlit/elements/pyplot.py`

 * *Files identical despite different names*

### Comparing `custom-streamlit-1.19.0/streamlit/elements/radio.py` & `custom-streamlit-1.20.0/streamlit/elements/radio.py`

 * *Files identical despite different names*

### Comparing `custom-streamlit-1.19.0/streamlit/elements/select_slider.py` & `custom-streamlit-1.20.0/streamlit/elements/select_slider.py`

 * *Files identical despite different names*

### Comparing `custom-streamlit-1.19.0/streamlit/elements/selectbox.py` & `custom-streamlit-1.20.0/streamlit/elements/selectbox.py`

 * *Files identical despite different names*

### Comparing `custom-streamlit-1.19.0/streamlit/elements/show.py` & `custom-streamlit-1.20.0/streamlit/elements/show.py`

 * *Files identical despite different names*

### Comparing `custom-streamlit-1.19.0/streamlit/elements/slider.py` & `custom-streamlit-1.20.0/streamlit/elements/slider.py`

 * *Files identical despite different names*

### Comparing `custom-streamlit-1.19.0/streamlit/elements/snow.py` & `custom-streamlit-1.20.0/streamlit/elements/snow.py`

 * *Files identical despite different names*

### Comparing `custom-streamlit-1.19.0/streamlit/elements/spinner.py` & `custom-streamlit-1.20.0/streamlit/elements/spinner.py`

 * *Files identical despite different names*

### Comparing `custom-streamlit-1.19.0/streamlit/elements/text.py` & `custom-streamlit-1.20.0/streamlit/elements/text.py`

 * *Files identical despite different names*

### Comparing `custom-streamlit-1.19.0/streamlit/elements/text_widgets.py` & `custom-streamlit-1.20.0/streamlit/elements/text_widgets.py`

 * *Files identical despite different names*

### Comparing `custom-streamlit-1.19.0/streamlit/elements/time_widgets.py` & `custom-streamlit-1.20.0/streamlit/elements/time_widgets.py`

 * *Files identical despite different names*

### Comparing `custom-streamlit-1.19.0/streamlit/elements/utils.py` & `custom-streamlit-1.20.0/streamlit/elements/utils.py`

 * *Files identical despite different names*

### Comparing `custom-streamlit-1.19.0/streamlit/elements/write.py` & `custom-streamlit-1.20.0/streamlit/elements/write.py`

 * *Files identical despite different names*

### Comparing `custom-streamlit-1.19.0/streamlit/emojis.py` & `custom-streamlit-1.20.0/streamlit/emojis.py`

 * *Files identical despite different names*

### Comparing `custom-streamlit-1.19.0/streamlit/env_util.py` & `custom-streamlit-1.20.0/streamlit/env_util.py`

 * *Files identical despite different names*

### Comparing `custom-streamlit-1.19.0/streamlit/error_util.py` & `custom-streamlit-1.20.0/streamlit/error_util.py`

 * *Files identical despite different names*

### Comparing `custom-streamlit-1.19.0/streamlit/errors.py` & `custom-streamlit-1.20.0/streamlit/errors.py`

 * *Files identical despite different names*

### Comparing `custom-streamlit-1.19.0/streamlit/file_util.py` & `custom-streamlit-1.20.0/streamlit/file_util.py`

 * *Files identical despite different names*

### Comparing `custom-streamlit-1.19.0/streamlit/folder_black_list.py` & `custom-streamlit-1.20.0/streamlit/folder_black_list.py`

 * *Files identical despite different names*

### Comparing `custom-streamlit-1.19.0/streamlit/git_util.py` & `custom-streamlit-1.20.0/streamlit/git_util.py`

 * *Files identical despite different names*

### Comparing `custom-streamlit-1.19.0/streamlit/hello/Hello.py` & `custom-streamlit-1.20.0/streamlit/hello/Hello.py`

 * *Files identical despite different names*

### Comparing `custom-streamlit-1.19.0/streamlit/hello/__init__.py` & `custom-streamlit-1.20.0/streamlit/hello/__init__.py`

 * *Files identical despite different names*

### Comparing `custom-streamlit-1.19.0/streamlit/hello/pages/0_Animation_Demo.py` & `custom-streamlit-1.20.0/streamlit/hello/pages/0_Animation_Demo.py`

 * *Files identical despite different names*

### Comparing `custom-streamlit-1.19.0/streamlit/hello/pages/1_Plotting_Demo.py` & `custom-streamlit-1.20.0/streamlit/hello/pages/1_Plotting_Demo.py`

 * *Files identical despite different names*

### Comparing `custom-streamlit-1.19.0/streamlit/hello/pages/2_Mapping_Demo.py` & `custom-streamlit-1.20.0/streamlit/hello/pages/2_Mapping_Demo.py`

 * *Files identical despite different names*

### Comparing `custom-streamlit-1.19.0/streamlit/hello/pages/3_DataFrame_Demo.py` & `custom-streamlit-1.20.0/streamlit/hello/pages/3_DataFrame_Demo.py`

 * *Files identical despite different names*

### Comparing `custom-streamlit-1.19.0/streamlit/hello/utils.py` & `custom-streamlit-1.20.0/streamlit/hello/utils.py`

 * *Files identical despite different names*

### Comparing `custom-streamlit-1.19.0/streamlit/js_number.py` & `custom-streamlit-1.20.0/streamlit/js_number.py`

 * *Files identical despite different names*

### Comparing `custom-streamlit-1.19.0/streamlit/logger.py` & `custom-streamlit-1.20.0/streamlit/logger.py`

 * *Files identical despite different names*

### Comparing `custom-streamlit-1.19.0/streamlit/net_util.py` & `custom-streamlit-1.20.0/streamlit/net_util.py`

 * *Files identical despite different names*

### Comparing `custom-streamlit-1.19.0/streamlit/proto/Alert_pb2.py` & `custom-streamlit-1.20.0/streamlit/proto/Alert_pb2.py`

 * *Files identical despite different names*

### Comparing `custom-streamlit-1.19.0/streamlit/proto/AppPage_pb2.py` & `custom-streamlit-1.20.0/streamlit/proto/AppPage_pb2.py`

 * *Files identical despite different names*

### Comparing `custom-streamlit-1.19.0/streamlit/proto/ArrowNamedDataSet_pb2.py` & `custom-streamlit-1.20.0/streamlit/proto/ArrowNamedDataSet_pb2.py`

 * *Files identical despite different names*

### Comparing `custom-streamlit-1.19.0/streamlit/proto/ArrowVegaLiteChart_pb2.py` & `custom-streamlit-1.20.0/streamlit/proto/ArrowVegaLiteChart_pb2.py`

 * *Files identical despite different names*

### Comparing `custom-streamlit-1.19.0/streamlit/proto/Arrow_pb2.py` & `custom-streamlit-1.20.0/streamlit/proto/Arrow_pb2.py`

 * *Files identical despite different names*

### Comparing `custom-streamlit-1.19.0/streamlit/proto/Audio_pb2.py` & `custom-streamlit-1.20.0/streamlit/proto/Audio_pb2.py`

 * *Files identical despite different names*

### Comparing `custom-streamlit-1.19.0/streamlit/proto/BackMsg_pb2.py` & `custom-streamlit-1.20.0/streamlit/proto/BackMsg_pb2.py`

 * *Files identical despite different names*

### Comparing `custom-streamlit-1.19.0/streamlit/proto/Balloons_pb2.py` & `custom-streamlit-1.20.0/streamlit/proto/Balloons_pb2.py`

 * *Files identical despite different names*

### Comparing `custom-streamlit-1.19.0/streamlit/proto/Block_pb2.py` & `custom-streamlit-1.20.0/streamlit/proto/Block_pb2.py`

 * *Files identical despite different names*

### Comparing `custom-streamlit-1.19.0/streamlit/proto/BokehChart_pb2.py` & `custom-streamlit-1.20.0/streamlit/proto/BokehChart_pb2.py`

 * *Files identical despite different names*

### Comparing `custom-streamlit-1.19.0/streamlit/proto/Button_pb2.py` & `custom-streamlit-1.20.0/streamlit/proto/Button_pb2.py`

 * *Files identical despite different names*

### Comparing `custom-streamlit-1.19.0/streamlit/proto/CameraInput_pb2.py` & `custom-streamlit-1.20.0/streamlit/proto/CameraInput_pb2.py`

 * *Files identical despite different names*

### Comparing `custom-streamlit-1.19.0/streamlit/proto/Checkbox_pb2.py` & `custom-streamlit-1.20.0/streamlit/proto/Checkbox_pb2.py`

 * *Files identical despite different names*

### Comparing `custom-streamlit-1.19.0/streamlit/proto/ClientState_pb2.py` & `custom-streamlit-1.20.0/streamlit/proto/ClientState_pb2.py`

 * *Files identical despite different names*

### Comparing `custom-streamlit-1.19.0/streamlit/proto/Code_pb2.py` & `custom-streamlit-1.20.0/streamlit/proto/Code_pb2.py`

 * *Files identical despite different names*

### Comparing `custom-streamlit-1.19.0/streamlit/proto/ColorPicker_pb2.py` & `custom-streamlit-1.20.0/streamlit/proto/ColorPicker_pb2.py`

 * *Files identical despite different names*

### Comparing `custom-streamlit-1.19.0/streamlit/proto/Common_pb2.py` & `custom-streamlit-1.20.0/streamlit/proto/Common_pb2.py`

 * *Files identical despite different names*

### Comparing `custom-streamlit-1.19.0/streamlit/proto/Components_pb2.py` & `custom-streamlit-1.20.0/streamlit/proto/Components_pb2.py`

 * *Files identical despite different names*

### Comparing `custom-streamlit-1.19.0/streamlit/proto/DataFrame_pb2.py` & `custom-streamlit-1.20.0/streamlit/proto/DataFrame_pb2.py`

 * *Files identical despite different names*

### Comparing `custom-streamlit-1.19.0/streamlit/proto/DateInput_pb2.py` & `custom-streamlit-1.20.0/streamlit/proto/DateInput_pb2.py`

 * *Files identical despite different names*

### Comparing `custom-streamlit-1.19.0/streamlit/proto/DeckGlJsonChart_pb2.py` & `custom-streamlit-1.20.0/streamlit/proto/DeckGlJsonChart_pb2.py`

 * *Files identical despite different names*

### Comparing `custom-streamlit-1.19.0/streamlit/proto/Delta_pb2.py` & `custom-streamlit-1.20.0/streamlit/proto/Delta_pb2.py`

 * *Files identical despite different names*

### Comparing `custom-streamlit-1.19.0/streamlit/proto/DocString_pb2.py` & `custom-streamlit-1.20.0/streamlit/proto/DocString_pb2.py`

 * *Files identical despite different names*

### Comparing `custom-streamlit-1.19.0/streamlit/proto/DownloadButton_pb2.py` & `custom-streamlit-1.20.0/streamlit/proto/DownloadButton_pb2.py`

 * *Files identical despite different names*

### Comparing `custom-streamlit-1.19.0/streamlit/proto/Element_pb2.py` & `custom-streamlit-1.20.0/streamlit/proto/Element_pb2.py`

 * *Files identical despite different names*

### Comparing `custom-streamlit-1.19.0/streamlit/proto/Empty_pb2.py` & `custom-streamlit-1.20.0/streamlit/proto/Empty_pb2.py`

 * *Files identical despite different names*

### Comparing `custom-streamlit-1.19.0/streamlit/proto/Exception_pb2.py` & `custom-streamlit-1.20.0/streamlit/proto/Exception_pb2.py`

 * *Files identical despite different names*

### Comparing `custom-streamlit-1.19.0/streamlit/proto/Favicon_pb2.py` & `custom-streamlit-1.20.0/streamlit/proto/Favicon_pb2.py`

 * *Files identical despite different names*

### Comparing `custom-streamlit-1.19.0/streamlit/proto/FileUploader_pb2.py` & `custom-streamlit-1.20.0/streamlit/proto/FileUploader_pb2.py`

 * *Files identical despite different names*

### Comparing `custom-streamlit-1.19.0/streamlit/proto/ForwardMsg_pb2.py` & `custom-streamlit-1.20.0/streamlit/proto/ForwardMsg_pb2.py`

 * *Files identical despite different names*

### Comparing `custom-streamlit-1.19.0/streamlit/proto/GitInfo_pb2.py` & `custom-streamlit-1.20.0/streamlit/proto/GitInfo_pb2.py`

 * *Files identical despite different names*

### Comparing `custom-streamlit-1.19.0/streamlit/proto/GraphVizChart_pb2.py` & `custom-streamlit-1.20.0/streamlit/proto/GraphVizChart_pb2.py`

 * *Files identical despite different names*

### Comparing `custom-streamlit-1.19.0/streamlit/proto/Heading_pb2.py` & `custom-streamlit-1.20.0/streamlit/proto/Heading_pb2.py`

 * *Files identical despite different names*

### Comparing `custom-streamlit-1.19.0/streamlit/proto/IFrame_pb2.py` & `custom-streamlit-1.20.0/streamlit/proto/IFrame_pb2.py`

 * *Files identical despite different names*

### Comparing `custom-streamlit-1.19.0/streamlit/proto/Image_pb2.py` & `custom-streamlit-1.20.0/streamlit/proto/Image_pb2.py`

 * *Files identical despite different names*

### Comparing `custom-streamlit-1.19.0/streamlit/proto/Json_pb2.py` & `custom-streamlit-1.20.0/streamlit/proto/Json_pb2.py`

 * *Files identical despite different names*

### Comparing `custom-streamlit-1.19.0/streamlit/proto/LabelVisibilityMessage_pb2.py` & `custom-streamlit-1.20.0/streamlit/proto/LabelVisibilityMessage_pb2.py`

 * *Files identical despite different names*

### Comparing `custom-streamlit-1.19.0/streamlit/proto/Markdown_pb2.py` & `custom-streamlit-1.20.0/streamlit/proto/Markdown_pb2.py`

 * *Files identical despite different names*

### Comparing `custom-streamlit-1.19.0/streamlit/proto/Metric_pb2.py` & `custom-streamlit-1.20.0/streamlit/proto/Metric_pb2.py`

 * *Files identical despite different names*

### Comparing `custom-streamlit-1.19.0/streamlit/proto/MultiSelect_pb2.py` & `custom-streamlit-1.20.0/streamlit/proto/MultiSelect_pb2.py`

 * *Files identical despite different names*

### Comparing `custom-streamlit-1.19.0/streamlit/proto/NamedDataSet_pb2.py` & `custom-streamlit-1.20.0/streamlit/proto/NamedDataSet_pb2.py`

 * *Files identical despite different names*

### Comparing `custom-streamlit-1.19.0/streamlit/proto/NewSession_pb2.py` & `custom-streamlit-1.20.0/streamlit/proto/NewSession_pb2.py`

 * *Files identical despite different names*

### Comparing `custom-streamlit-1.19.0/streamlit/proto/NumberInput_pb2.py` & `custom-streamlit-1.20.0/streamlit/proto/NumberInput_pb2.py`

 * *Files identical despite different names*

### Comparing `custom-streamlit-1.19.0/streamlit/proto/PageConfig_pb2.py` & `custom-streamlit-1.20.0/streamlit/proto/PageConfig_pb2.py`

 * *Files identical despite different names*

### Comparing `custom-streamlit-1.19.0/streamlit/proto/PageInfo_pb2.py` & `custom-streamlit-1.20.0/streamlit/proto/PageInfo_pb2.py`

 * *Files identical despite different names*

### Comparing `custom-streamlit-1.19.0/streamlit/proto/PageNotFound_pb2.py` & `custom-streamlit-1.20.0/streamlit/proto/PageNotFound_pb2.py`

 * *Files identical despite different names*

### Comparing `custom-streamlit-1.19.0/streamlit/proto/PageProfile_pb2.py` & `custom-streamlit-1.20.0/streamlit/proto/PageProfile_pb2.py`

 * *Files identical despite different names*

### Comparing `custom-streamlit-1.19.0/streamlit/proto/PagesChanged_pb2.py` & `custom-streamlit-1.20.0/streamlit/proto/PagesChanged_pb2.py`

 * *Files identical despite different names*

### Comparing `custom-streamlit-1.19.0/streamlit/proto/PlotlyChart_pb2.py` & `custom-streamlit-1.20.0/streamlit/proto/PlotlyChart_pb2.py`

 * *Files identical despite different names*

### Comparing `custom-streamlit-1.19.0/streamlit/proto/Progress_pb2.py` & `custom-streamlit-1.20.0/streamlit/proto/Progress_pb2.py`

 * *Files identical despite different names*

### Comparing `custom-streamlit-1.19.0/streamlit/proto/Radio_pb2.py` & `custom-streamlit-1.20.0/streamlit/proto/Radio_pb2.py`

 * *Files identical despite different names*

### Comparing `custom-streamlit-1.19.0/streamlit/proto/RootContainer_pb2.py` & `custom-streamlit-1.20.0/streamlit/proto/RootContainer_pb2.py`

 * *Files identical despite different names*

### Comparing `custom-streamlit-1.19.0/streamlit/proto/Selectbox_pb2.py` & `custom-streamlit-1.20.0/streamlit/proto/Selectbox_pb2.py`

 * *Files identical despite different names*

### Comparing `custom-streamlit-1.19.0/streamlit/proto/SessionEvent_pb2.py` & `custom-streamlit-1.20.0/streamlit/proto/SessionEvent_pb2.py`

 * *Files identical despite different names*

### Comparing `custom-streamlit-1.19.0/streamlit/proto/SessionStatus_pb2.py` & `custom-streamlit-1.20.0/streamlit/proto/SessionStatus_pb2.py`

 * *Files identical despite different names*

### Comparing `custom-streamlit-1.19.0/streamlit/proto/Slider_pb2.py` & `custom-streamlit-1.20.0/streamlit/proto/Slider_pb2.py`

 * *Files identical despite different names*

### Comparing `custom-streamlit-1.19.0/streamlit/proto/Snow_pb2.py` & `custom-streamlit-1.20.0/streamlit/proto/Snow_pb2.py`

 * *Files identical despite different names*

### Comparing `custom-streamlit-1.19.0/streamlit/proto/Spinner_pb2.py` & `custom-streamlit-1.20.0/streamlit/proto/Spinner_pb2.py`

 * *Files identical despite different names*

### Comparing `custom-streamlit-1.19.0/streamlit/proto/TextArea_pb2.py` & `custom-streamlit-1.20.0/streamlit/proto/TextArea_pb2.py`

 * *Files identical despite different names*

### Comparing `custom-streamlit-1.19.0/streamlit/proto/TextInput_pb2.py` & `custom-streamlit-1.20.0/streamlit/proto/TextInput_pb2.py`

 * *Files identical despite different names*

### Comparing `custom-streamlit-1.19.0/streamlit/proto/Text_pb2.py` & `custom-streamlit-1.20.0/streamlit/proto/Text_pb2.py`

 * *Files identical despite different names*

### Comparing `custom-streamlit-1.19.0/streamlit/proto/TimeInput_pb2.py` & `custom-streamlit-1.20.0/streamlit/proto/TimeInput_pb2.py`

 * *Files identical despite different names*

### Comparing `custom-streamlit-1.19.0/streamlit/proto/VegaLiteChart_pb2.py` & `custom-streamlit-1.20.0/streamlit/proto/VegaLiteChart_pb2.py`

 * *Files identical despite different names*

### Comparing `custom-streamlit-1.19.0/streamlit/proto/Video_pb2.py` & `custom-streamlit-1.20.0/streamlit/proto/Video_pb2.py`

 * *Files identical despite different names*

### Comparing `custom-streamlit-1.19.0/streamlit/proto/WidgetStates_pb2.py` & `custom-streamlit-1.20.0/streamlit/proto/WidgetStates_pb2.py`

 * *Files identical despite different names*

### Comparing `custom-streamlit-1.19.0/streamlit/proto/__init__.py` & `custom-streamlit-1.20.0/streamlit/proto/__init__.py`

 * *Files identical despite different names*

### Comparing `custom-streamlit-1.19.0/streamlit/proto/openmetrics_data_model_pb2.py` & `custom-streamlit-1.20.0/streamlit/proto/openmetrics_data_model_pb2.py`

 * *Files identical despite different names*

### Comparing `custom-streamlit-1.19.0/streamlit/runtime/__init__.py` & `custom-streamlit-1.20.0/streamlit/runtime/__init__.py`

 * *Files identical despite different names*

### Comparing `custom-streamlit-1.19.0/streamlit/runtime/app_session.py` & `custom-streamlit-1.20.0/streamlit/runtime/app_session.py`

 * *Files identical despite different names*

### Comparing `custom-streamlit-1.19.0/streamlit/runtime/caching/__init__.py` & `custom-streamlit-1.20.0/streamlit/runtime/caching/__init__.py`

 * *Files identical despite different names*

### Comparing `custom-streamlit-1.19.0/streamlit/runtime/caching/cache_data_api.py` & `custom-streamlit-1.20.0/streamlit/runtime/caching/cache_data_api.py`

 * *Files identical despite different names*

### Comparing `custom-streamlit-1.19.0/streamlit/runtime/caching/cache_errors.py` & `custom-streamlit-1.20.0/streamlit/runtime/caching/cache_errors.py`

 * *Files identical despite different names*

### Comparing `custom-streamlit-1.19.0/streamlit/runtime/caching/cache_resource_api.py` & `custom-streamlit-1.20.0/streamlit/runtime/caching/cache_resource_api.py`

 * *Files identical despite different names*

### Comparing `custom-streamlit-1.19.0/streamlit/runtime/caching/cache_type.py` & `custom-streamlit-1.20.0/streamlit/runtime/caching/cache_type.py`

 * *Files identical despite different names*

### Comparing `custom-streamlit-1.19.0/streamlit/runtime/caching/cache_utils.py` & `custom-streamlit-1.20.0/streamlit/runtime/caching/cache_utils.py`

 * *Files identical despite different names*

### Comparing `custom-streamlit-1.19.0/streamlit/runtime/caching/cached_message_replay.py` & `custom-streamlit-1.20.0/streamlit/runtime/caching/cached_message_replay.py`

 * *Files identical despite different names*

### Comparing `custom-streamlit-1.19.0/streamlit/runtime/caching/hashing.py` & `custom-streamlit-1.20.0/streamlit/runtime/caching/hashing.py`

 * *Files identical despite different names*

### Comparing `custom-streamlit-1.19.0/streamlit/runtime/caching/storage/__init__.py` & `custom-streamlit-1.20.0/streamlit/runtime/caching/storage/__init__.py`

 * *Files identical despite different names*

### Comparing `custom-streamlit-1.19.0/streamlit/runtime/caching/storage/cache_storage_protocol.py` & `custom-streamlit-1.20.0/streamlit/runtime/caching/storage/cache_storage_protocol.py`

 * *Files identical despite different names*

### Comparing `custom-streamlit-1.19.0/streamlit/runtime/caching/storage/dummy_cache_storage.py` & `custom-streamlit-1.20.0/streamlit/runtime/caching/storage/dummy_cache_storage.py`

 * *Files identical despite different names*

### Comparing `custom-streamlit-1.19.0/streamlit/runtime/caching/storage/in_memory_cache_storage_wrapper.py` & `custom-streamlit-1.20.0/streamlit/runtime/caching/storage/in_memory_cache_storage_wrapper.py`

 * *Files identical despite different names*

### Comparing `custom-streamlit-1.19.0/streamlit/runtime/caching/storage/local_disk_cache_storage.py` & `custom-streamlit-1.20.0/streamlit/runtime/caching/storage/local_disk_cache_storage.py`

 * *Files identical despite different names*

### Comparing `custom-streamlit-1.19.0/streamlit/runtime/credentials.py` & `custom-streamlit-1.20.0/streamlit/runtime/credentials.py`

 * *Files identical despite different names*

### Comparing `custom-streamlit-1.19.0/streamlit/runtime/forward_msg_cache.py` & `custom-streamlit-1.20.0/streamlit/runtime/forward_msg_cache.py`

 * *Files identical despite different names*

### Comparing `custom-streamlit-1.19.0/streamlit/runtime/forward_msg_queue.py` & `custom-streamlit-1.20.0/streamlit/runtime/forward_msg_queue.py`

 * *Files identical despite different names*

### Comparing `custom-streamlit-1.19.0/streamlit/runtime/legacy_caching/__init__.py` & `custom-streamlit-1.20.0/streamlit/runtime/legacy_caching/__init__.py`

 * *Files identical despite different names*

### Comparing `custom-streamlit-1.19.0/streamlit/runtime/legacy_caching/caching.py` & `custom-streamlit-1.20.0/streamlit/runtime/legacy_caching/caching.py`

 * *Files identical despite different names*

### Comparing `custom-streamlit-1.19.0/streamlit/runtime/legacy_caching/hashing.py` & `custom-streamlit-1.20.0/streamlit/runtime/legacy_caching/hashing.py`

 * *Files identical despite different names*

### Comparing `custom-streamlit-1.19.0/streamlit/runtime/media_file_manager.py` & `custom-streamlit-1.20.0/streamlit/runtime/media_file_manager.py`

 * *Files identical despite different names*

### Comparing `custom-streamlit-1.19.0/streamlit/runtime/media_file_storage.py` & `custom-streamlit-1.20.0/streamlit/runtime/media_file_storage.py`

 * *Files identical despite different names*

### Comparing `custom-streamlit-1.19.0/streamlit/runtime/memory_media_file_storage.py` & `custom-streamlit-1.20.0/streamlit/runtime/memory_media_file_storage.py`

 * *Files identical despite different names*

### Comparing `custom-streamlit-1.19.0/streamlit/runtime/memory_session_storage.py` & `custom-streamlit-1.20.0/streamlit/runtime/memory_session_storage.py`

 * *Files identical despite different names*

### Comparing `custom-streamlit-1.19.0/streamlit/runtime/metrics_util.py` & `custom-streamlit-1.20.0/streamlit/runtime/metrics_util.py`

 * *Files identical despite different names*

### Comparing `custom-streamlit-1.19.0/streamlit/runtime/runtime.py` & `custom-streamlit-1.20.0/streamlit/runtime/runtime.py`

 * *Files identical despite different names*

### Comparing `custom-streamlit-1.19.0/streamlit/runtime/runtime_util.py` & `custom-streamlit-1.20.0/streamlit/runtime/runtime_util.py`

 * *Files identical despite different names*

### Comparing `custom-streamlit-1.19.0/streamlit/runtime/script_data.py` & `custom-streamlit-1.20.0/streamlit/runtime/script_data.py`

 * *Files identical despite different names*

### Comparing `custom-streamlit-1.19.0/streamlit/runtime/scriptrunner/__init__.py` & `custom-streamlit-1.20.0/streamlit/runtime/scriptrunner/__init__.py`

 * *Files identical despite different names*

### Comparing `custom-streamlit-1.19.0/streamlit/runtime/scriptrunner/magic.py` & `custom-streamlit-1.20.0/streamlit/runtime/scriptrunner/magic.py`

 * *Files identical despite different names*

### Comparing `custom-streamlit-1.19.0/streamlit/runtime/scriptrunner/magic_funcs.py` & `custom-streamlit-1.20.0/streamlit/runtime/scriptrunner/magic_funcs.py`

 * *Files identical despite different names*

### Comparing `custom-streamlit-1.19.0/streamlit/runtime/scriptrunner/script_requests.py` & `custom-streamlit-1.20.0/streamlit/runtime/scriptrunner/script_requests.py`

 * *Files identical despite different names*

### Comparing `custom-streamlit-1.19.0/streamlit/runtime/scriptrunner/script_run_context.py` & `custom-streamlit-1.20.0/streamlit/runtime/scriptrunner/script_run_context.py`

 * *Files identical despite different names*

### Comparing `custom-streamlit-1.19.0/streamlit/runtime/scriptrunner/script_runner.py` & `custom-streamlit-1.20.0/streamlit/runtime/scriptrunner/script_runner.py`

 * *Files identical despite different names*

### Comparing `custom-streamlit-1.19.0/streamlit/runtime/secrets.py` & `custom-streamlit-1.20.0/streamlit/runtime/secrets.py`

 * *Files identical despite different names*

### Comparing `custom-streamlit-1.19.0/streamlit/runtime/session_manager.py` & `custom-streamlit-1.20.0/streamlit/runtime/session_manager.py`

 * *Files identical despite different names*

### Comparing `custom-streamlit-1.19.0/streamlit/runtime/state/__init__.py` & `custom-streamlit-1.20.0/streamlit/runtime/state/__init__.py`

 * *Files identical despite different names*

### Comparing `custom-streamlit-1.19.0/streamlit/runtime/state/common.py` & `custom-streamlit-1.20.0/streamlit/runtime/state/common.py`

 * *Files identical despite different names*

### Comparing `custom-streamlit-1.19.0/streamlit/runtime/state/safe_session_state.py` & `custom-streamlit-1.20.0/streamlit/runtime/state/safe_session_state.py`

 * *Files identical despite different names*

### Comparing `custom-streamlit-1.19.0/streamlit/runtime/state/session_state.py` & `custom-streamlit-1.20.0/streamlit/runtime/state/session_state.py`

 * *Files identical despite different names*

### Comparing `custom-streamlit-1.19.0/streamlit/runtime/state/session_state_proxy.py` & `custom-streamlit-1.20.0/streamlit/runtime/state/session_state_proxy.py`

 * *Files identical despite different names*

### Comparing `custom-streamlit-1.19.0/streamlit/runtime/state/widgets.py` & `custom-streamlit-1.20.0/streamlit/runtime/state/widgets.py`

 * *Files identical despite different names*

### Comparing `custom-streamlit-1.19.0/streamlit/runtime/stats.py` & `custom-streamlit-1.20.0/streamlit/runtime/stats.py`

 * *Files identical despite different names*

### Comparing `custom-streamlit-1.19.0/streamlit/runtime/uploaded_file_manager.py` & `custom-streamlit-1.20.0/streamlit/runtime/uploaded_file_manager.py`

 * *Files identical despite different names*

### Comparing `custom-streamlit-1.19.0/streamlit/runtime/websocket_session_manager.py` & `custom-streamlit-1.20.0/streamlit/runtime/websocket_session_manager.py`

 * *Files identical despite different names*

### Comparing `custom-streamlit-1.19.0/streamlit/source_util.py` & `custom-streamlit-1.20.0/streamlit/source_util.py`

 * *Files identical despite different names*

### Comparing `custom-streamlit-1.19.0/streamlit/string_util.py` & `custom-streamlit-1.20.0/streamlit/string_util.py`

 * *Files identical despite different names*

### Comparing `custom-streamlit-1.19.0/streamlit/temporary_directory.py` & `custom-streamlit-1.20.0/streamlit/temporary_directory.py`

 * *Files identical despite different names*

### Comparing `custom-streamlit-1.19.0/streamlit/testing/__init__.py` & `custom-streamlit-1.20.0/streamlit/testing/__init__.py`

 * *Files identical despite different names*

### Comparing `custom-streamlit-1.19.0/streamlit/testing/element_tree.py` & `custom-streamlit-1.20.0/streamlit/testing/element_tree.py`

 * *Files identical despite different names*

### Comparing `custom-streamlit-1.19.0/streamlit/testing/local_script_runner.py` & `custom-streamlit-1.20.0/streamlit/testing/local_script_runner.py`

 * *Files identical despite different names*

### Comparing `custom-streamlit-1.19.0/streamlit/testing/script_interactions.py` & `custom-streamlit-1.20.0/streamlit/testing/script_interactions.py`

 * *Files identical despite different names*

### Comparing `custom-streamlit-1.19.0/streamlit/type_util.py` & `custom-streamlit-1.20.0/streamlit/type_util.py`

 * *Files identical despite different names*

### Comparing `custom-streamlit-1.19.0/streamlit/url_util.py` & `custom-streamlit-1.20.0/streamlit/url_util.py`

 * *Files identical despite different names*

### Comparing `custom-streamlit-1.19.0/streamlit/user_info.py` & `custom-streamlit-1.20.0/streamlit/user_info.py`

 * *Files identical despite different names*

### Comparing `custom-streamlit-1.19.0/streamlit/util.py` & `custom-streamlit-1.20.0/streamlit/util.py`

 * *Files identical despite different names*

### Comparing `custom-streamlit-1.19.0/streamlit/vendor/ipython/modified_sys_path.py` & `custom-streamlit-1.20.0/streamlit/vendor/ipython/modified_sys_path.py`

 * *Files identical despite different names*

### Comparing `custom-streamlit-1.19.0/streamlit/version.py` & `custom-streamlit-1.20.0/streamlit/version.py`

 * *Files identical despite different names*

### Comparing `custom-streamlit-1.19.0/streamlit/watcher/__init__.py` & `custom-streamlit-1.20.0/streamlit/watcher/__init__.py`

 * *Files identical despite different names*

### Comparing `custom-streamlit-1.19.0/streamlit/watcher/event_based_path_watcher.py` & `custom-streamlit-1.20.0/streamlit/watcher/event_based_path_watcher.py`

 * *Files identical despite different names*

### Comparing `custom-streamlit-1.19.0/streamlit/watcher/local_sources_watcher.py` & `custom-streamlit-1.20.0/streamlit/watcher/local_sources_watcher.py`

 * *Files identical despite different names*

### Comparing `custom-streamlit-1.19.0/streamlit/watcher/path_watcher.py` & `custom-streamlit-1.20.0/streamlit/watcher/path_watcher.py`

 * *Files identical despite different names*

### Comparing `custom-streamlit-1.19.0/streamlit/watcher/polling_path_watcher.py` & `custom-streamlit-1.20.0/streamlit/watcher/polling_path_watcher.py`

 * *Files identical despite different names*

### Comparing `custom-streamlit-1.19.0/streamlit/watcher/util.py` & `custom-streamlit-1.20.0/streamlit/watcher/util.py`

 * *Files identical despite different names*

### Comparing `custom-streamlit-1.19.0/streamlit/web/__init__.py` & `custom-streamlit-1.20.0/streamlit/web/__init__.py`

 * *Files identical despite different names*

### Comparing `custom-streamlit-1.19.0/streamlit/web/bootstrap.py` & `custom-streamlit-1.20.0/streamlit/web/bootstrap.py`

 * *Files identical despite different names*

### Comparing `custom-streamlit-1.19.0/streamlit/web/cache_storage_manager_config.py` & `custom-streamlit-1.20.0/streamlit/web/cache_storage_manager_config.py`

 * *Files identical despite different names*

### Comparing `custom-streamlit-1.19.0/streamlit/web/cli.py` & `custom-streamlit-1.20.0/streamlit/web/cli.py`

 * *Files identical despite different names*

### Comparing `custom-streamlit-1.19.0/streamlit/web/server/__init__.py` & `custom-streamlit-1.20.0/streamlit/web/server/__init__.py`

 * *Files identical despite different names*

### Comparing `custom-streamlit-1.19.0/streamlit/web/server/app_static_file_handler.py` & `custom-streamlit-1.20.0/streamlit/web/server/app_static_file_handler.py`

 * *Files identical despite different names*

### Comparing `custom-streamlit-1.19.0/streamlit/web/server/browser_websocket_handler.py` & `custom-streamlit-1.20.0/streamlit/web/server/browser_websocket_handler.py`

 * *Files identical despite different names*

### Comparing `custom-streamlit-1.19.0/streamlit/web/server/component_request_handler.py` & `custom-streamlit-1.20.0/streamlit/web/server/component_request_handler.py`

 * *Files identical despite different names*

### Comparing `custom-streamlit-1.19.0/streamlit/web/server/media_file_handler.py` & `custom-streamlit-1.20.0/streamlit/web/server/media_file_handler.py`

 * *Files identical despite different names*

### Comparing `custom-streamlit-1.19.0/streamlit/web/server/routes.py` & `custom-streamlit-1.20.0/streamlit/web/server/routes.py`

 * *Files identical despite different names*

### Comparing `custom-streamlit-1.19.0/streamlit/web/server/server.py` & `custom-streamlit-1.20.0/streamlit/web/server/server.py`

 * *Files identical despite different names*

### Comparing `custom-streamlit-1.19.0/streamlit/web/server/server_util.py` & `custom-streamlit-1.20.0/streamlit/web/server/server_util.py`

 * *Files identical despite different names*

### Comparing `custom-streamlit-1.19.0/streamlit/web/server/stats_request_handler.py` & `custom-streamlit-1.20.0/streamlit/web/server/stats_request_handler.py`

 * *Files identical despite different names*

### Comparing `custom-streamlit-1.19.0/streamlit/web/server/upload_file_request_handler.py` & `custom-streamlit-1.20.0/streamlit/web/server/upload_file_request_handler.py`

 * *Files identical despite different names*

### Comparing `custom-streamlit-1.19.0/streamlit/web/server/websocket_headers.py` & `custom-streamlit-1.20.0/streamlit/web/server/websocket_headers.py`

 * *Files identical despite different names*

### Comparing `custom-streamlit-1.19.0/tests/testutil.py` & `custom-streamlit-1.20.0/tests/testutil.py`

 * *Files identical despite different names*

