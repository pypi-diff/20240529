# Comparing `tmp/browsergym_core-0.3.3.tar.gz` & `tmp/browsergym_core-0.3.4.tar.gz`

## Comparing `browsergym_core-0.3.3.tar` & `browsergym_core-0.3.4.tar`

### file list

```diff
@@ -1,74 +1,74 @@
--rw-r--r--   0        0        0      108 2020-02-02 00:00:00.000000 browsergym_core-0.3.3/requirements.txt
--rw-r--r--   0        0        0      579 2020-02-02 00:00:00.000000 browsergym_core-0.3.3/src/browsergym/core/__init__.py
--rw-r--r--   0        0        0     3480 2020-02-02 00:00:00.000000 browsergym_core-0.3.3/src/browsergym/core/chat.py
--rw-r--r--   0        0        0      253 2020-02-02 00:00:00.000000 browsergym_core-0.3.3/src/browsergym/core/constants.py
--rw-r--r--   0        0        0    21895 2020-02-02 00:00:00.000000 browsergym_core-0.3.3/src/browsergym/core/env.py
--rw-r--r--   0        0        0    20773 2020-02-02 00:00:00.000000 browsergym_core-0.3.3/src/browsergym/core/observation.py
--rw-r--r--   0        0        0      926 2020-02-02 00:00:00.000000 browsergym_core-0.3.3/src/browsergym/core/registration.py
--rw-r--r--   0        0        0     3969 2020-02-02 00:00:00.000000 browsergym_core-0.3.3/src/browsergym/core/spaces.py
--rw-r--r--   0        0        0     3094 2020-02-02 00:00:00.000000 browsergym_core-0.3.3/src/browsergym/core/task.py
--rw-r--r--   0        0        0        0 2020-02-02 00:00:00.000000 browsergym_core-0.3.3/src/browsergym/core/action/__init__.py
--rw-r--r--   0        0        0     1862 2020-02-02 00:00:00.000000 browsergym_core-0.3.3/src/browsergym/core/action/base.py
--rw-r--r--   0        0        0    18196 2020-02-02 00:00:00.000000 browsergym_core-0.3.3/src/browsergym/core/action/functions.py
--rw-r--r--   0        0        0     9725 2020-02-02 00:00:00.000000 browsergym_core-0.3.3/src/browsergym/core/action/highlevel.py
--rw-r--r--   0        0        0     3596 2020-02-02 00:00:00.000000 browsergym_core-0.3.3/src/browsergym/core/action/parsers.py
--rw-r--r--   0        0        0     3872 2020-02-02 00:00:00.000000 browsergym_core-0.3.3/src/browsergym/core/action/python.py
--rw-r--r--   0        0        0     9860 2020-02-02 00:00:00.000000 browsergym_core-0.3.3/src/browsergym/core/action/utils.py
--rw-r--r--   0        0        0   133496 2020-02-02 00:00:00.000000 browsergym_core-0.3.3/src/browsergym/core/chat_files/assistant.png
--rw-r--r--   0        0        0     6687 2020-02-02 00:00:00.000000 browsergym_core-0.3.3/src/browsergym/core/chat_files/chatbox.html
--rw-r--r--   0        0        0    11244 2020-02-02 00:00:00.000000 browsergym_core-0.3.3/src/browsergym/core/chat_files/chatbox_modern.html
--rw-r--r--   0        0        0      643 2020-02-02 00:00:00.000000 browsergym_core-0.3.3/src/browsergym/core/chat_files/img/send.svg
--rw-r--r--   0        0        0    11891 2020-02-02 00:00:00.000000 browsergym_core-0.3.3/src/browsergym/core/javascript/frame_mark_elements.js
--rw-r--r--   0        0        0     1705 2020-02-02 00:00:00.000000 browsergym_core-0.3.3/src/browsergym/core/javascript/frame_unmark_elements.js
--rw-r--r--   0        0        0    19506 2020-02-02 00:00:00.000000 browsergym_core-0.3.3/src/browsergym/utils/obs.py
--rw-r--r--   0        0        0    39837 2020-02-02 00:00:00.000000 browsergym_core-0.3.3/tests/test_actions_highlevel.py
--rw-r--r--   0        0        0      776 2020-02-02 00:00:00.000000 browsergym_core-0.3.3/tests/test_actions_python.py
--rw-r--r--   0        0        0     8715 2020-02-02 00:00:00.000000 browsergym_core-0.3.3/tests/test_gym_envs.py
--rw-r--r--   0        0        0    24194 2020-02-02 00:00:00.000000 browsergym_core-0.3.3/tests/test_observation.py
--rw-r--r--   0        0        0      527 2020-02-02 00:00:00.000000 browsergym_core-0.3.3/tests/utils.py
--rw-r--r--   0        0        0     1384 2020-02-02 00:00:00.000000 browsergym_core-0.3.3/tests/data/example.html
--rw-r--r--   0        0        0      170 2020-02-02 00:00:00.000000 browsergym_core-0.3.3/tests/data/hover.html
--rw-r--r--   0        0        0     2506 2020-02-02 00:00:00.000000 browsergym_core-0.3.3/tests/data/long_page.html
--rw-r--r--   0        0        0    26054 2020-02-02 00:00:00.000000 browsergym_core-0.3.3/tests/data/screenshot.png
--rw-r--r--   0        0        0      801 2020-02-02 00:00:00.000000 browsergym_core-0.3.3/tests/data/test_page.html
--rw-r--r--   0        0        0     1205 2020-02-02 00:00:00.000000 browsergym_core-0.3.3/tests/data/test_page_2.html
--rw-r--r--   0        0        0      202 2020-02-02 00:00:00.000000 browsergym_core-0.3.3/tests/data/textbox.html
--rw-r--r--   0        0        0     1120 2020-02-02 00:00:00.000000 browsergym_core-0.3.3/tests/data/basic_iframe_site/basic_iframe.html
--rw-r--r--   0        0        0      338 2020-02-02 00:00:00.000000 browsergym_core-0.3.3/tests/data/basic_iframe_site/basic_iframe_2.html
--rw-r--r--   0        0        0      532 2020-02-02 00:00:00.000000 browsergym_core-0.3.3/tests/data/basic_iframe_site/inner-iframe.html
--rw-r--r--   0        0        0     1091 2020-02-02 00:00:00.000000 browsergym_core-0.3.3/tests/data/basic_iframe_site/outer-iframe.html
--rw-r--r--   0        0        0     2102 2020-02-02 00:00:00.000000 browsergym_core-0.3.3/tests/data/basic_shadow_dom_site/basic_shadow_dom.html
--rw-r--r--   0        0        0      600 2020-02-02 00:00:00.000000 browsergym_core-0.3.3/tests/data/basic_shadow_dom_site/simple_shadow_dom.html
--rw-r--r--   0        0        0     1120 2020-02-02 00:00:00.000000 browsergym_core-0.3.3/tests/data/basic_shadow_iframe_site/basic_iframe.html
--rw-r--r--   0        0        0      313 2020-02-02 00:00:00.000000 browsergym_core-0.3.3/tests/data/basic_shadow_iframe_site/basic_iframe_2.html
--rw-r--r--   0        0        0      265 2020-02-02 00:00:00.000000 browsergym_core-0.3.3/tests/data/basic_shadow_iframe_site/inner-iframe.html
--rw-r--r--   0        0        0     1232 2020-02-02 00:00:00.000000 browsergym_core-0.3.3/tests/data/basic_shadow_iframe_site/outer-iframe.html
--rw-r--r--   0        0        0      143 2020-02-02 00:00:00.000000 browsergym_core-0.3.3/tests/data/input_type/button_input.html
--rw-r--r--   0        0        0      606 2020-02-02 00:00:00.000000 browsergym_core-0.3.3/tests/data/input_type/checkbox_input.html
--rw-r--r--   0        0        0      517 2020-02-02 00:00:00.000000 browsergym_core-0.3.3/tests/data/input_type/color_picker_input.html
--rw-r--r--   0        0        0      474 2020-02-02 00:00:00.000000 browsergym_core-0.3.3/tests/data/input_type/date_input.html
--rw-r--r--   0        0        0      639 2020-02-02 00:00:00.000000 browsergym_core-0.3.3/tests/data/input_type/date_min_max_input.html
--rw-r--r--   0        0        0      543 2020-02-02 00:00:00.000000 browsergym_core-0.3.3/tests/data/input_type/date_time_local_input.html
--rw-r--r--   0        0        0      381 2020-02-02 00:00:00.000000 browsergym_core-0.3.3/tests/data/input_type/email_input.html
--rw-r--r--   0        0        0      353 2020-02-02 00:00:00.000000 browsergym_core-0.3.3/tests/data/input_type/file_input.html
--rw-r--r--   0        0        0      481 2020-02-02 00:00:00.000000 browsergym_core-0.3.3/tests/data/input_type/hidden_field_input.html
--rw-r--r--   0        0        0      553 2020-02-02 00:00:00.000000 browsergym_core-0.3.3/tests/data/input_type/image_input.html
--rw-r--r--   0        0        0     2256 2020-02-02 00:00:00.000000 browsergym_core-0.3.3/tests/data/input_type/img_submit.gif
--rw-r--r--   0        0        0      481 2020-02-02 00:00:00.000000 browsergym_core-0.3.3/tests/data/input_type/number_input.html
--rw-r--r--   0        0        0      393 2020-02-02 00:00:00.000000 browsergym_core-0.3.3/tests/data/input_type/number_step_input.html
--rw-r--r--   0        0        0      539 2020-02-02 00:00:00.000000 browsergym_core-0.3.3/tests/data/input_type/password_input.html
--rw-r--r--   0        0        0      394 2020-02-02 00:00:00.000000 browsergym_core-0.3.3/tests/data/input_type/radio_input.html
--rw-r--r--   0        0        0      401 2020-02-02 00:00:00.000000 browsergym_core-0.3.3/tests/data/input_type/range_input.html
--rw-r--r--   0        0        0      666 2020-02-02 00:00:00.000000 browsergym_core-0.3.3/tests/data/input_type/reset_input.html
--rw-r--r--   0        0        0      385 2020-02-02 00:00:00.000000 browsergym_core-0.3.3/tests/data/input_type/search_input.html
--rw-r--r--   0        0        0      625 2020-02-02 00:00:00.000000 browsergym_core-0.3.3/tests/data/input_type/submit_input.html
--rw-r--r--   0        0        0      356 2020-02-02 00:00:00.000000 browsergym_core-0.3.3/tests/data/input_type/submit_nn_input.html
--rw-r--r--   0        0        0      517 2020-02-02 00:00:00.000000 browsergym_core-0.3.3/tests/data/input_type/telephone_input.html
--rw-r--r--   0        0        0      574 2020-02-02 00:00:00.000000 browsergym_core-0.3.3/tests/data/input_type/text_input.html
--rw-r--r--   0        0        0      567 2020-02-02 00:00:00.000000 browsergym_core-0.3.3/tests/data/input_type/time_input.html
--rw-r--r--   0        0        0      397 2020-02-02 00:00:00.000000 browsergym_core-0.3.3/tests/data/input_type/url_input.html
--rw-r--r--   0        0        0      397 2020-02-02 00:00:00.000000 browsergym_core-0.3.3/tests/data/input_type/week_input.html
--rw-r--r--   0        0        0     1875 2020-02-02 00:00:00.000000 browsergym_core-0.3.3/.gitignore
--rw-r--r--   0        0        0      231 2020-02-02 00:00:00.000000 browsergym_core-0.3.3/README.md
--rw-r--r--   0        0        0     1148 2020-02-02 00:00:00.000000 browsergym_core-0.3.3/pyproject.toml
--rw-r--r--   0        0        0     1167 2020-02-02 00:00:00.000000 browsergym_core-0.3.3/PKG-INFO
+-rw-r--r--   0        0        0      108 2020-02-02 00:00:00.000000 browsergym_core-0.3.4/requirements.txt
+-rw-r--r--   0        0        0      579 2020-02-02 00:00:00.000000 browsergym_core-0.3.4/src/browsergym/core/__init__.py
+-rw-r--r--   0        0        0     3516 2020-02-02 00:00:00.000000 browsergym_core-0.3.4/src/browsergym/core/chat.py
+-rw-r--r--   0        0        0      253 2020-02-02 00:00:00.000000 browsergym_core-0.3.4/src/browsergym/core/constants.py
+-rw-r--r--   0        0        0    22325 2020-02-02 00:00:00.000000 browsergym_core-0.3.4/src/browsergym/core/env.py
+-rw-r--r--   0        0        0    20806 2020-02-02 00:00:00.000000 browsergym_core-0.3.4/src/browsergym/core/observation.py
+-rw-r--r--   0        0        0      926 2020-02-02 00:00:00.000000 browsergym_core-0.3.4/src/browsergym/core/registration.py
+-rw-r--r--   0        0        0     3969 2020-02-02 00:00:00.000000 browsergym_core-0.3.4/src/browsergym/core/spaces.py
+-rw-r--r--   0        0        0     3094 2020-02-02 00:00:00.000000 browsergym_core-0.3.4/src/browsergym/core/task.py
+-rw-r--r--   0        0        0        0 2020-02-02 00:00:00.000000 browsergym_core-0.3.4/src/browsergym/core/action/__init__.py
+-rw-r--r--   0        0        0     1862 2020-02-02 00:00:00.000000 browsergym_core-0.3.4/src/browsergym/core/action/base.py
+-rw-r--r--   0        0        0    18196 2020-02-02 00:00:00.000000 browsergym_core-0.3.4/src/browsergym/core/action/functions.py
+-rw-r--r--   0        0        0     9725 2020-02-02 00:00:00.000000 browsergym_core-0.3.4/src/browsergym/core/action/highlevel.py
+-rw-r--r--   0        0        0     3596 2020-02-02 00:00:00.000000 browsergym_core-0.3.4/src/browsergym/core/action/parsers.py
+-rw-r--r--   0        0        0     3872 2020-02-02 00:00:00.000000 browsergym_core-0.3.4/src/browsergym/core/action/python.py
+-rw-r--r--   0        0        0     9853 2020-02-02 00:00:00.000000 browsergym_core-0.3.4/src/browsergym/core/action/utils.py
+-rw-r--r--   0        0        0   133496 2020-02-02 00:00:00.000000 browsergym_core-0.3.4/src/browsergym/core/chat_files/assistant.png
+-rw-r--r--   0        0        0     6687 2020-02-02 00:00:00.000000 browsergym_core-0.3.4/src/browsergym/core/chat_files/chatbox.html
+-rw-r--r--   0        0        0    11459 2020-02-02 00:00:00.000000 browsergym_core-0.3.4/src/browsergym/core/chat_files/chatbox_modern.html
+-rw-r--r--   0        0        0      643 2020-02-02 00:00:00.000000 browsergym_core-0.3.4/src/browsergym/core/chat_files/img/send.svg
+-rw-r--r--   0        0        0    11891 2020-02-02 00:00:00.000000 browsergym_core-0.3.4/src/browsergym/core/javascript/frame_mark_elements.js
+-rw-r--r--   0        0        0     1705 2020-02-02 00:00:00.000000 browsergym_core-0.3.4/src/browsergym/core/javascript/frame_unmark_elements.js
+-rw-r--r--   0        0        0    19783 2020-02-02 00:00:00.000000 browsergym_core-0.3.4/src/browsergym/utils/obs.py
+-rw-r--r--   0        0        0    39837 2020-02-02 00:00:00.000000 browsergym_core-0.3.4/tests/test_actions_highlevel.py
+-rw-r--r--   0        0        0      776 2020-02-02 00:00:00.000000 browsergym_core-0.3.4/tests/test_actions_python.py
+-rw-r--r--   0        0        0     8715 2020-02-02 00:00:00.000000 browsergym_core-0.3.4/tests/test_gym_envs.py
+-rw-r--r--   0        0        0    24194 2020-02-02 00:00:00.000000 browsergym_core-0.3.4/tests/test_observation.py
+-rw-r--r--   0        0        0      527 2020-02-02 00:00:00.000000 browsergym_core-0.3.4/tests/utils.py
+-rw-r--r--   0        0        0     1384 2020-02-02 00:00:00.000000 browsergym_core-0.3.4/tests/data/example.html
+-rw-r--r--   0        0        0      170 2020-02-02 00:00:00.000000 browsergym_core-0.3.4/tests/data/hover.html
+-rw-r--r--   0        0        0     2506 2020-02-02 00:00:00.000000 browsergym_core-0.3.4/tests/data/long_page.html
+-rw-r--r--   0        0        0    26054 2020-02-02 00:00:00.000000 browsergym_core-0.3.4/tests/data/screenshot.png
+-rw-r--r--   0        0        0      801 2020-02-02 00:00:00.000000 browsergym_core-0.3.4/tests/data/test_page.html
+-rw-r--r--   0        0        0     1205 2020-02-02 00:00:00.000000 browsergym_core-0.3.4/tests/data/test_page_2.html
+-rw-r--r--   0        0        0      202 2020-02-02 00:00:00.000000 browsergym_core-0.3.4/tests/data/textbox.html
+-rw-r--r--   0        0        0     1120 2020-02-02 00:00:00.000000 browsergym_core-0.3.4/tests/data/basic_iframe_site/basic_iframe.html
+-rw-r--r--   0        0        0      338 2020-02-02 00:00:00.000000 browsergym_core-0.3.4/tests/data/basic_iframe_site/basic_iframe_2.html
+-rw-r--r--   0        0        0      532 2020-02-02 00:00:00.000000 browsergym_core-0.3.4/tests/data/basic_iframe_site/inner-iframe.html
+-rw-r--r--   0        0        0     1091 2020-02-02 00:00:00.000000 browsergym_core-0.3.4/tests/data/basic_iframe_site/outer-iframe.html
+-rw-r--r--   0        0        0     2102 2020-02-02 00:00:00.000000 browsergym_core-0.3.4/tests/data/basic_shadow_dom_site/basic_shadow_dom.html
+-rw-r--r--   0        0        0      600 2020-02-02 00:00:00.000000 browsergym_core-0.3.4/tests/data/basic_shadow_dom_site/simple_shadow_dom.html
+-rw-r--r--   0        0        0     1120 2020-02-02 00:00:00.000000 browsergym_core-0.3.4/tests/data/basic_shadow_iframe_site/basic_iframe.html
+-rw-r--r--   0        0        0      313 2020-02-02 00:00:00.000000 browsergym_core-0.3.4/tests/data/basic_shadow_iframe_site/basic_iframe_2.html
+-rw-r--r--   0        0        0      265 2020-02-02 00:00:00.000000 browsergym_core-0.3.4/tests/data/basic_shadow_iframe_site/inner-iframe.html
+-rw-r--r--   0        0        0     1232 2020-02-02 00:00:00.000000 browsergym_core-0.3.4/tests/data/basic_shadow_iframe_site/outer-iframe.html
+-rw-r--r--   0        0        0      143 2020-02-02 00:00:00.000000 browsergym_core-0.3.4/tests/data/input_type/button_input.html
+-rw-r--r--   0        0        0      606 2020-02-02 00:00:00.000000 browsergym_core-0.3.4/tests/data/input_type/checkbox_input.html
+-rw-r--r--   0        0        0      517 2020-02-02 00:00:00.000000 browsergym_core-0.3.4/tests/data/input_type/color_picker_input.html
+-rw-r--r--   0        0        0      474 2020-02-02 00:00:00.000000 browsergym_core-0.3.4/tests/data/input_type/date_input.html
+-rw-r--r--   0        0        0      639 2020-02-02 00:00:00.000000 browsergym_core-0.3.4/tests/data/input_type/date_min_max_input.html
+-rw-r--r--   0        0        0      543 2020-02-02 00:00:00.000000 browsergym_core-0.3.4/tests/data/input_type/date_time_local_input.html
+-rw-r--r--   0        0        0      381 2020-02-02 00:00:00.000000 browsergym_core-0.3.4/tests/data/input_type/email_input.html
+-rw-r--r--   0        0        0      353 2020-02-02 00:00:00.000000 browsergym_core-0.3.4/tests/data/input_type/file_input.html
+-rw-r--r--   0        0        0      481 2020-02-02 00:00:00.000000 browsergym_core-0.3.4/tests/data/input_type/hidden_field_input.html
+-rw-r--r--   0        0        0      553 2020-02-02 00:00:00.000000 browsergym_core-0.3.4/tests/data/input_type/image_input.html
+-rw-r--r--   0        0        0     2256 2020-02-02 00:00:00.000000 browsergym_core-0.3.4/tests/data/input_type/img_submit.gif
+-rw-r--r--   0        0        0      481 2020-02-02 00:00:00.000000 browsergym_core-0.3.4/tests/data/input_type/number_input.html
+-rw-r--r--   0        0        0      393 2020-02-02 00:00:00.000000 browsergym_core-0.3.4/tests/data/input_type/number_step_input.html
+-rw-r--r--   0        0        0      539 2020-02-02 00:00:00.000000 browsergym_core-0.3.4/tests/data/input_type/password_input.html
+-rw-r--r--   0        0        0      394 2020-02-02 00:00:00.000000 browsergym_core-0.3.4/tests/data/input_type/radio_input.html
+-rw-r--r--   0        0        0      401 2020-02-02 00:00:00.000000 browsergym_core-0.3.4/tests/data/input_type/range_input.html
+-rw-r--r--   0        0        0      666 2020-02-02 00:00:00.000000 browsergym_core-0.3.4/tests/data/input_type/reset_input.html
+-rw-r--r--   0        0        0      385 2020-02-02 00:00:00.000000 browsergym_core-0.3.4/tests/data/input_type/search_input.html
+-rw-r--r--   0        0        0      625 2020-02-02 00:00:00.000000 browsergym_core-0.3.4/tests/data/input_type/submit_input.html
+-rw-r--r--   0        0        0      356 2020-02-02 00:00:00.000000 browsergym_core-0.3.4/tests/data/input_type/submit_nn_input.html
+-rw-r--r--   0        0        0      517 2020-02-02 00:00:00.000000 browsergym_core-0.3.4/tests/data/input_type/telephone_input.html
+-rw-r--r--   0        0        0      574 2020-02-02 00:00:00.000000 browsergym_core-0.3.4/tests/data/input_type/text_input.html
+-rw-r--r--   0        0        0      567 2020-02-02 00:00:00.000000 browsergym_core-0.3.4/tests/data/input_type/time_input.html
+-rw-r--r--   0        0        0      397 2020-02-02 00:00:00.000000 browsergym_core-0.3.4/tests/data/input_type/url_input.html
+-rw-r--r--   0        0        0      397 2020-02-02 00:00:00.000000 browsergym_core-0.3.4/tests/data/input_type/week_input.html
+-rw-r--r--   0        0        0     1875 2020-02-02 00:00:00.000000 browsergym_core-0.3.4/.gitignore
+-rw-r--r--   0        0        0      231 2020-02-02 00:00:00.000000 browsergym_core-0.3.4/README.md
+-rw-r--r--   0        0        0     1148 2020-02-02 00:00:00.000000 browsergym_core-0.3.4/pyproject.toml
+-rw-r--r--   0        0        0     1167 2020-02-02 00:00:00.000000 browsergym_core-0.3.4/PKG-INFO
```

### Comparing `browsergym_core-0.3.3/src/browsergym/core/__init__.py` & `browsergym_core-0.3.4/src/browsergym/core/__init__.py`

 * *Files 1% similar despite different names*

```diff
@@ -1,8 +1,8 @@
-__version__ = "0.3.3"
+__version__ = "0.3.4"
 
 import playwright.sync_api
 
 # we use a global playwright instance
 _PLAYWRIGHT = None
```

### Comparing `browsergym_core-0.3.3/src/browsergym/core/chat.py` & `browsergym_core-0.3.4/src/browsergym/core/chat.py`

 * *Files 16% similar despite different names*

```diff
@@ -9,14 +9,16 @@
 from importlib import resources
 
 from . import _get_global_playwright, chat_files
 
 
 CHATBOX_DIR = resources.files(chat_files)
 
+logger = logging.getLogger(__name__)
+
 
 class Chat:
     def __init__(
         self, headless: bool, chat_size=(500, 800), record_video_dir=None, modern=True
     ) -> None:
         self.messages = []
 
@@ -57,20 +59,20 @@
             raise ValueError(f"Invalid role: {role}")
         if role in ("user", "assistant", "infeasible"):
             self.messages.append({"role": role, "timestamp": utc_time, "message": msg})
         timestamp = time.strftime("%H:%M:%S", time.localtime(utc_time))
         self.page.evaluate(f"addChatMessage({repr(role)}, {repr(timestamp)}, {repr(msg)});")
 
     def wait_for_user_message(self):
-        logging.info("Waiting for message from user...")
+        logger.info("Waiting for message from user...")
         # reset flag
         self.page.evaluate("USER_MESSAGE_RECEIVED = false;")
         # wait for flag to be raised
         self.page.wait_for_function("USER_MESSAGE_RECEIVED", polling=100, timeout=0)
-        logging.info("Message received.")
+        logger.info("Message received.")
 
     def close(self):
         self.context.close()
         self.browser.close()
 
 
 def get_chatbox_modern(chatbox_dir) -> str:
```

### Comparing `browsergym_core-0.3.3/src/browsergym/core/env.py` & `browsergym_core-0.3.4/src/browsergym/core/env.py`

 * *Files 4% similar despite different names*

```diff
@@ -26,14 +26,17 @@
 )
 from .action.base import execute_python_code
 from .action.highlevel import HighLevelActionSet
 from .action.base import execute_python_code
 from . import _get_global_playwright
 
 
+logger = logging.getLogger(__name__)
+
+
 class BrowserEnv(gym.Env, ABC):
     """The main BrowserGym class, which encapsulates instruction-following Web browsing into a Gymnasium environment."""
 
     # gym metadata
     metadata = {"render_modes": None}
 
     def __init__(
@@ -165,15 +168,15 @@
         def override_property(task, env, property):
             """Extract property value from env if not None, otherwise from task."""
             env_value = getattr(env, property)
             task_value = getattr(task, property)
             if env_value is None:
                 return task_value
             else:
-                logging.warning(
+                logger.warning(
                     f"Overriding the task's {property} parameter ({repr(task_value)} => {repr(env_value)}). This might change the task's behaviour and difficulty."
                 )
                 return env_value
 
         # fetch task's desired parameters for browser setup
         viewport = override_property(self.task, self, "viewport")
         slow_mo = override_property(self.task, self, "slow_mo")
@@ -296,28 +299,30 @@
                 "recording_start_time": self.chat.recording_start_time,
                 "recording_file": str(self.chat.page.video.path()),
             }
 
         return obs, info
 
     def step(self, action: str) -> tuple:
+
         self.last_action = action
 
         info = {}
         info["action_exec_start"] = time.time()
         info["action_exec_timeout"] = 0
 
         def send_message_to_user(text: str):
             self.chat.add_message(role="assistant", msg=text)
 
         def report_infeasible_instructions(reason: str):
             self.chat.add_message(role="infeasible", msg=reason)
             self.infeasible_message_received = True
 
         # try to execute the action
+        logger.debug(f"Executing action")
         try:
             if self.action_mapping:
                 code = self.action_mapping(action)
             else:
                 code = action
             execute_python_code(
                 code,
@@ -327,41 +332,46 @@
             )
             self.last_action_error = ""
         except Exception as e:
             self.last_action_error = f"{type(e).__name__}: {e}"
             match = re.match("TimeoutError: Timeout ([0-9]+)ms exceeded.", self.last_action_error)
             if match:
                 info["action_exec_timeout"] = float(match.groups()[0]) / 1000  # ms to sec
-
+        logger.debug(f"Action executed")
         info["action_exec_stop"] = time.time()
 
         # wait a bit (for the JavaScript callback to set the active page)
         time.sleep(0.5)  # wait for JS events to be fired (half a second)
         self.context.cookies()  # trigger all waiting Playwright callbacks on the stack (hack, see https://playwright.dev/java/docs/multithreading)
 
         # wait for the network to idle before extracting the observation, reward etc.
         self._wait_dom_loaded()
 
         # after the action is executed, the active page might have changed
         # perform a safety check
         self._active_page_check()
+        logger.debug(f"Active page checked")
 
         # if asked, wait for user message
         self._wait_for_user_message()
+        logger.debug(f"User message done")
 
+        logger.debug(f"Initiating task validation")
         # extract reward, done, user_message, info (task-specific)
         reward, done, user_message, task_info = self._task_validate()
         info["task_info"] = task_info
+        logger.debug(f"Task validation done")
 
         # add any user message sent by the task to the chat
         if user_message:
             self.chat.add_message(role="user", msg=user_message)
 
         # extract observation (generic)
         obs = self._get_obs()
+        logger.debug(f"Observation extracted")
 
         # new step API wants a 5-tuple (gymnasium)
         terminated = done or (
             self.terminate_on_infeasible and self.infeasible_message_received
         )  # task or agent can terminate the episode
         truncated = False
 
@@ -373,15 +383,15 @@
         prev_page_history = self.page_history.copy()
 
         # call validate
         reward, done, user_message, info = self.task.validate(self.page, self.chat.messages)
 
         # safety fix, in case validate() did mess up the active page and/or page history
         if prev_active_page != self.page or prev_page_history != self.page_history:
-            logging.info(
+            logger.info(
                 "The active page and / or page history has changed during task.validate(). A recovery fix will be applied."
             )
             self.page = prev_active_page
             self.page_history = prev_page_history
 
         return reward, done, user_message, info
 
@@ -400,14 +410,15 @@
             for frame in page.frames:
                 try:
                     frame.wait_for_load_state("domcontentloaded", timeout=3000)
                 except playwright.sync_api.TimeoutError:
                     pass
 
     def _activate_page_from_js(self, page: playwright.sync_api.Page):
+        logger.debug(f"_activate_page_from_js(page) called, page={str(page)}")
         if not page.context == self.context:
             raise RuntimeError(
                 f"Unexpected: activating a page that belongs to a different browser context ({page})."
             )
 
         # add the activated page to the page history (or move it to last which is the most recent)
         if page in self.page_history:
@@ -419,15 +430,15 @@
 
         self.page = page
 
     def _active_page_check(self):
         # make sure there is always a page open
         # if all pages have been closed, create a new page
         if len(self.context.pages) == 0:
-            logging.warning(f"All pages are closed, opening a new page.")
+            logger.warning(f"All pages are closed, opening a new page.")
             self.page = self.context.new_page()
 
         # if the active page got closed, get the last active page from the history
         while self.page_history and (self.page.is_closed() or self.page not in self.context.pages):
             self.page_history.pop(self.page)  # remove active page from history
             self.page = list(self.page_history.keys())[
                 -1
@@ -460,15 +471,15 @@
                 if retries_left > 0 and (
                     "Frame was detached" in err_msg
                     or "Frame with the given frameId is not found" in err_msg
                     or "Execution context was destroyed" in err_msg
                     or "Frame has been detached" in err_msg
                     or "Cannot mark a child frame without a bid" in err_msg
                 ):
-                    logging.warning(
+                    logger.warning(
                         f"An error occured while extracting the dom and axtree. Retrying ({retries_left}/{EXTRACT_OBS_MAX_TRIES} tries left).\n{repr(e)}"
                     )
                     # post-extract cleanup (aria-roledescription attribute)
                     _post_extract(self.page)
                     time.sleep(0.5)
                     continue
                 else:
```

### Comparing `browsergym_core-0.3.3/src/browsergym/core/observation.py` & `browsergym_core-0.3.4/src/browsergym/core/observation.py`

 * *Files 2% similar despite different names*

```diff
@@ -10,14 +10,17 @@
 from .constants import BROWSERGYM_ID_ATTRIBUTE as BID_ATTR
 from .constants import BROWSERGYM_VISIBILITY_ATTRIBUTE as VIS_ATTR
 from .constants import BROWSERGYM_SETOFMARKS_ATTRIBUTE as SOM_ATTR
 
 MARK_FRAMES_MAX_TRIES = 3
 
 
+logger = logging.getLogger(__name__)
+
+
 class MarkingError(Exception):
     pass
 
 
 def _pre_extract(page: playwright.sync_api.Page):
     """
     pre-extraction routine, marks dom elements (set bid and dynamic attributes like value and checked)
@@ -34,25 +37,25 @@
         # mark all DOM elements in the frame (it will use the parent frame element's bid as a prefix)
         warning_msgs = frame.evaluate(
             js_frame_mark_elements,
             [frame_bid, BID_ATTR],
         )
         # print warning messages if any
         for msg in warning_msgs:
-            logging.warning(msg)
+            logger.warning(msg)
 
         # recursively mark all descendant frames
         for child_frame in frame.child_frames:
             # deal with detached frames
             if child_frame.is_detached():
                 continue
             # deal with weird frames (pdf viewer in <embed>)
             child_frame_elem = child_frame.frame_element()
             if not child_frame_elem.content_frame() == child_frame:
-                logging.warning(
+                logger.warning(
                     f"Skipping frame '{child_frame.name}' for marking, seems problematic."
                 )
                 continue
             # deal with sandboxed frames with blocked script execution
             sandbox_attr = child_frame_elem.get_attribute("sandbox")
             if sandbox_attr is not None and "allow-scripts" not in sandbox_attr.split():
                 continue
@@ -72,15 +75,15 @@
 
     # we can't run this loop in JS due to Same-Origin Policy
     # (can't access the content of an iframe from a another one)
     for frame in page.frames:
         if not frame == page.main_frame:
             # deal with weird frames (pdf viewer in <embed>)
             if not frame.frame_element().content_frame() == frame:
-                logging.warning(f"Skipping frame '{frame.name}' for unmarking, seems problematic.")
+                logger.warning(f"Skipping frame '{frame.name}' for unmarking, seems problematic.")
                 continue
             # deal with sandboxed frames with blocked script execution
             sandbox_attr = frame.frame_element().get_attribute("sandbox")
             if sandbox_attr is not None and "allow-scripts" not in sandbox_attr.split():
                 continue
 
         try:
@@ -138,15 +141,15 @@
 def extract_data_items_from_aria(string):
     """
     Utility function to extract temporary data stored in the "aria-roledescription" attribute of a node
     """
 
     match = __DATA_REGEXP.fullmatch(string)
     if not match:
-        logging.warning(
+        logger.warning(
             f'Data items could not be extracted from "aria-roledescription" attribute: {string}'
         )
         return [], string
 
     groups = match.groups()
     data_items = groups[:-1]
     original_aria = groups[-1]
@@ -375,15 +378,15 @@
     # collect the extra properties of all nodes with a browsergym_id attribute
     extra_properties = {}
     for doc in doc_properties.keys():
         for node in doc_properties[doc]["nodes"]:
             bid = node["bid"]
             if bid:
                 if bid in extra_properties:
-                    logging.warning(f"duplicate {BID_ATTR}={repr(bid)} attribute detected")
+                    logger.warning(f"duplicate {BID_ATTR}={repr(bid)} attribute detected")
                 extra_properties[bid] = {
                     extra_prop: node[extra_prop]
                     for extra_prop in ("visibility", "bbox", "clickable", "set_of_marks")
                 }
 
     return extra_properties
 
@@ -486,15 +489,15 @@
                 # if a frame is not found in the extracted AXTrees, we just ignore it
                 if frame_id in frame_axtrees:
                     # root node should always be the first node in the AXTree
                     frame_root_node = frame_axtrees[frame_id]["nodes"][0]
                     assert frame_root_node["frameId"] == frame_id
                     node["childIds"].append(frame_root_node["nodeId"])
                 else:
-                    logging.warning(f"Extracted AXTree does not contain frameId '{frame_id}'")
+                    logger.warning(f"Extracted AXTree does not contain frameId '{frame_id}'")
 
     cdp.detach()
 
     return merged_axtree
 
 
 def extract_focused_element_bid(page: playwright.sync_api.Page):
```

### Comparing `browsergym_core-0.3.3/src/browsergym/core/registration.py` & `browsergym_core-0.3.4/src/browsergym/core/registration.py`

 * *Files identical despite different names*

### Comparing `browsergym_core-0.3.3/src/browsergym/core/spaces.py` & `browsergym_core-0.3.4/src/browsergym/core/spaces.py`

 * *Files identical despite different names*

### Comparing `browsergym_core-0.3.3/src/browsergym/core/task.py` & `browsergym_core-0.3.4/src/browsergym/core/task.py`

 * *Files identical despite different names*

### Comparing `browsergym_core-0.3.3/src/browsergym/core/action/base.py` & `browsergym_core-0.3.4/src/browsergym/core/action/base.py`

 * *Files identical despite different names*

### Comparing `browsergym_core-0.3.3/src/browsergym/core/action/functions.py` & `browsergym_core-0.3.4/src/browsergym/core/action/functions.py`

 * *Files identical despite different names*

### Comparing `browsergym_core-0.3.3/src/browsergym/core/action/highlevel.py` & `browsergym_core-0.3.4/src/browsergym/core/action/highlevel.py`

 * *Files identical despite different names*

### Comparing `browsergym_core-0.3.3/src/browsergym/core/action/parsers.py` & `browsergym_core-0.3.4/src/browsergym/core/action/parsers.py`

 * *Files identical despite different names*

### Comparing `browsergym_core-0.3.3/src/browsergym/core/action/python.py` & `browsergym_core-0.3.4/src/browsergym/core/action/python.py`

 * *Files identical despite different names*

### Comparing `browsergym_core-0.3.3/src/browsergym/core/action/utils.py` & `browsergym_core-0.3.4/src/browsergym/core/action/utils.py`

 * *Files 1% similar despite different names*

```diff
@@ -27,23 +27,23 @@
     # dive into each nested frame, to the frame where the element is located
     i = 0
     while bid[i:] and not bid[i:].isnumeric():
         i += 1
         frame_bid = bid[:i]  # bid of the next frame to select
         frame_elem = current_frame.get_by_test_id(frame_bid)
         if not frame_elem.count():
-            raise ValueError(f'could not find element with bid "{frame_bid}"')
+            raise ValueError(f'Could not find element with bid "{bid}"')
         if scroll_into_view:
             frame_elem.scroll_into_view_if_needed(timeout=500)
         current_frame = frame_elem.frame_locator(":scope")
 
     # finally, we should have selected the frame where the target element is
     elem = current_frame.get_by_test_id(bid)
     if not elem.count():
-        raise ValueError(f'Could not find element with bid "{bid}".')
+        raise ValueError(f'Could not find element with bid "{bid}"')
     if scroll_into_view:
         elem.scroll_into_view_if_needed(timeout=500)
     return elem
 
 
 def highlight_by_box(
     page: playwright.sync_api.Page, box: dict, color: Literal["blue", "red"] = "blue"
```

### Comparing `browsergym_core-0.3.3/src/browsergym/core/chat_files/assistant.png` & `browsergym_core-0.3.4/src/browsergym/core/chat_files/assistant.png`

 * *Files identical despite different names*

### Comparing `browsergym_core-0.3.3/src/browsergym/core/chat_files/chatbox.html` & `browsergym_core-0.3.4/src/browsergym/core/chat_files/chatbox.html`

 * *Files identical despite different names*

### Comparing `browsergym_core-0.3.3/src/browsergym/core/chat_files/chatbox_modern.html` & `browsergym_core-0.3.4/src/browsergym/core/chat_files/chatbox_modern.html`

 * *Files 1% similar despite different names*

```diff
@@ -276,43 +276,46 @@
         function addChatMessage(role, timeString, msg) {
             const chatBody = document.getElementById('chatBody');
             const chatDebug = document.getElementById('chatDebug');
             const msgContainer = document.createElement('div');
             msgContainer.className = 'message';
 
             const text = document.createElement('div');
-            text.innerHTML = addHtmlLineBreaks(escapeHtml(msg));
 
             // const assistant_img = document.createElement('img');
             // assistant_img.src = assistant_image_data;
             // assistant_img.alt = 'Assistant';
             // assistant_img.className = 'assistant-image';
 
             switch (role) {
                 case "user":
                     text.className = 'user-message';
+                    text.innerHTML = addHtmlLineBreaks(msg);
                     text.style.setProperty('--before-content', `"${timeString} - You"`);
                     msgContainer.appendChild(text);
                     chatBody.appendChild(msgContainer);
                     break;
                 case "assistant":
                     text.className = 'assistant-message';
+                    text.innerHTML = addHtmlLineBreaks(escapeHtml(msg));
                     text.style.setProperty('--before-content', `"${timeString} - Bot"`);
                     // msgContainer.appendChild(assistant_img); // Add the image to the message container
                     msgContainer.appendChild(text);
                     chatBody.appendChild(msgContainer);
                     break;
                 case "infeasible":
                     text.className = 'assistant-message';
+                    text.innerHTML = addHtmlLineBreaks(escapeHtml(msg));
                     text.style.setProperty('--before-content', `"${timeString} - Bot (abort)"`);
                     msgContainer.appendChild(text);
                     chatBody.appendChild(msgContainer);
                     break;
                 case "info":
                     text.className = 'info-message';
+                    text.innerHTML = addHtmlLineBreaks(escapeHtml(msg));
                     msgContainer.appendChild(text);
                     // hide previous debug messages
                     for (const msg of chatDebug.children) {
                         msg.style.display = 'none';
                     }
                     chatDebug.appendChild(msgContainer);
                     break;
```

### Comparing `browsergym_core-0.3.3/src/browsergym/core/chat_files/img/send.svg` & `browsergym_core-0.3.4/src/browsergym/core/chat_files/img/send.svg`

 * *Files identical despite different names*

### Comparing `browsergym_core-0.3.3/src/browsergym/core/javascript/frame_mark_elements.js` & `browsergym_core-0.3.4/src/browsergym/core/javascript/frame_mark_elements.js`

 * *Files identical despite different names*

### Comparing `browsergym_core-0.3.3/src/browsergym/core/javascript/frame_unmark_elements.js` & `browsergym_core-0.3.4/src/browsergym/core/javascript/frame_unmark_elements.js`

 * *Files identical despite different names*

### Comparing `browsergym_core-0.3.3/src/browsergym/utils/obs.py` & `browsergym_core-0.3.4/src/browsergym/utils/obs.py`

 * *Files 6% similar despite different names*

```diff
@@ -1,21 +1,24 @@
 import ast
+import logging
 import numpy as np
 import PIL.Image
 import PIL.ImageDraw
 import PIL.ImageFont
 import re
 
 from collections import defaultdict
 from bs4 import BeautifulSoup
 
 from browsergym.core.constants import BROWSERGYM_ID_ATTRIBUTE as BID_ATTR
 from browsergym.core.constants import BROWSERGYM_VISIBILITY_ATTRIBUTE as VIS_ATTR
 from browsergym.core.constants import BROWSERGYM_SETOFMARKS_ATTRIBUTE as SOM_ATTR
 
+logger = logging.getLogger(__name__)
+
 IGNORED_AXTREE_ROLES = ["LineBreak"]
 
 IGNORED_AXTREE_PROPERTIES = (
     "editable",
     "readonly",
     "level",
     "settable",
@@ -456,24 +459,30 @@
                 (x0 + xa * a0, y0 + ya * a0, x0 + xa * a1, y0 + ya * a1), fill=fill, width=width
             )
             a0 += step
 
     for bid, properties in extra_properties.items():
         if properties["set_of_marks"] and properties["bbox"]:
             x, y, width, height = properties["bbox"]
+            x0, y0 = x, y
+            x1, y1 = x + width, y + height
+
+            # skip small boxes
+            area = (x1 - x0) * (y1 - y0)
+            if area < 20:
+                logger.warning(
+                    f'som overlay: skipping bid "{bid}" due to bbox too small (area={area})'
+                )
+                continue
 
             # draw bounding box with dashed lines
-            linedashed(draw, x, y, x + width, y, fill=(0, 0, 0, 255), width=linewidth)
-            linedashed(
-                draw, x + width, y, x + width, y + height, fill=(0, 0, 0, 255), width=linewidth
-            )
-            linedashed(
-                draw, x, y + height, x + width, y + height, fill=(0, 0, 0, 255), width=linewidth
-            )
-            linedashed(draw, x, y, x, y + height, fill=(0, 0, 0, 255), width=linewidth)
+            linedashed(draw, x0, y0, x1, y0, fill=(0, 0, 0, 255), width=linewidth)
+            linedashed(draw, x1, y0, x1, y1, fill=(0, 0, 0, 255), width=linewidth)
+            linedashed(draw, x1, y1, x0, y1, fill=(0, 0, 0, 255), width=linewidth)
+            linedashed(draw, x0, y1, x0, y0, fill=(0, 0, 0, 255), width=linewidth)
 
             # get text box size (left, top, right, bottom)
             tag_box = font.getbbox(
                 bid,
             )
 
             # set tag size, including margins
```

### Comparing `browsergym_core-0.3.3/tests/test_actions_highlevel.py` & `browsergym_core-0.3.4/tests/test_actions_highlevel.py`

 * *Files identical despite different names*

### Comparing `browsergym_core-0.3.3/tests/test_actions_python.py` & `browsergym_core-0.3.4/tests/test_actions_python.py`

 * *Files identical despite different names*

### Comparing `browsergym_core-0.3.3/tests/test_gym_envs.py` & `browsergym_core-0.3.4/tests/test_gym_envs.py`

 * *Files identical despite different names*

### Comparing `browsergym_core-0.3.3/tests/test_observation.py` & `browsergym_core-0.3.4/tests/test_observation.py`

 * *Files identical despite different names*

### Comparing `browsergym_core-0.3.3/tests/utils.py` & `browsergym_core-0.3.4/tests/utils.py`

 * *Files identical despite different names*

### Comparing `browsergym_core-0.3.3/tests/data/example.html` & `browsergym_core-0.3.4/tests/data/example.html`

 * *Files identical despite different names*

### Comparing `browsergym_core-0.3.3/tests/data/long_page.html` & `browsergym_core-0.3.4/tests/data/long_page.html`

 * *Files identical despite different names*

### Comparing `browsergym_core-0.3.3/tests/data/screenshot.png` & `browsergym_core-0.3.4/tests/data/screenshot.png`

 * *Files identical despite different names*

### Comparing `browsergym_core-0.3.3/tests/data/test_page.html` & `browsergym_core-0.3.4/tests/data/test_page.html`

 * *Files identical despite different names*

### Comparing `browsergym_core-0.3.3/tests/data/test_page_2.html` & `browsergym_core-0.3.4/tests/data/test_page_2.html`

 * *Files identical despite different names*

### Comparing `browsergym_core-0.3.3/tests/data/basic_iframe_site/basic_iframe.html` & `browsergym_core-0.3.4/tests/data/basic_iframe_site/basic_iframe.html`

 * *Files identical despite different names*

### Comparing `browsergym_core-0.3.3/tests/data/basic_iframe_site/inner-iframe.html` & `browsergym_core-0.3.4/tests/data/basic_iframe_site/inner-iframe.html`

 * *Files identical despite different names*

### Comparing `browsergym_core-0.3.3/tests/data/basic_iframe_site/outer-iframe.html` & `browsergym_core-0.3.4/tests/data/basic_iframe_site/outer-iframe.html`

 * *Files identical despite different names*

### Comparing `browsergym_core-0.3.3/tests/data/basic_shadow_dom_site/basic_shadow_dom.html` & `browsergym_core-0.3.4/tests/data/basic_shadow_dom_site/basic_shadow_dom.html`

 * *Files identical despite different names*

### Comparing `browsergym_core-0.3.3/tests/data/basic_shadow_dom_site/simple_shadow_dom.html` & `browsergym_core-0.3.4/tests/data/basic_shadow_dom_site/simple_shadow_dom.html`

 * *Files identical despite different names*

### Comparing `browsergym_core-0.3.3/tests/data/basic_shadow_iframe_site/basic_iframe.html` & `browsergym_core-0.3.4/tests/data/basic_shadow_iframe_site/basic_iframe.html`

 * *Files identical despite different names*

### Comparing `browsergym_core-0.3.3/tests/data/basic_shadow_iframe_site/outer-iframe.html` & `browsergym_core-0.3.4/tests/data/basic_shadow_iframe_site/outer-iframe.html`

 * *Files identical despite different names*

### Comparing `browsergym_core-0.3.3/tests/data/input_type/checkbox_input.html` & `browsergym_core-0.3.4/tests/data/input_type/checkbox_input.html`

 * *Files identical despite different names*

### Comparing `browsergym_core-0.3.3/tests/data/input_type/color_picker_input.html` & `browsergym_core-0.3.4/tests/data/input_type/color_picker_input.html`

 * *Files identical despite different names*

### Comparing `browsergym_core-0.3.3/tests/data/input_type/date_min_max_input.html` & `browsergym_core-0.3.4/tests/data/input_type/date_min_max_input.html`

 * *Files identical despite different names*

### Comparing `browsergym_core-0.3.3/tests/data/input_type/date_time_local_input.html` & `browsergym_core-0.3.4/tests/data/input_type/date_time_local_input.html`

 * *Files identical despite different names*

### Comparing `browsergym_core-0.3.3/tests/data/input_type/image_input.html` & `browsergym_core-0.3.4/tests/data/input_type/image_input.html`

 * *Files identical despite different names*

### Comparing `browsergym_core-0.3.3/tests/data/input_type/img_submit.gif` & `browsergym_core-0.3.4/tests/data/input_type/img_submit.gif`

 * *Files identical despite different names*

### Comparing `browsergym_core-0.3.3/tests/data/input_type/password_input.html` & `browsergym_core-0.3.4/tests/data/input_type/password_input.html`

 * *Files identical despite different names*

### Comparing `browsergym_core-0.3.3/tests/data/input_type/reset_input.html` & `browsergym_core-0.3.4/tests/data/input_type/reset_input.html`

 * *Files identical despite different names*

### Comparing `browsergym_core-0.3.3/tests/data/input_type/submit_input.html` & `browsergym_core-0.3.4/tests/data/input_type/submit_input.html`

 * *Files identical despite different names*

### Comparing `browsergym_core-0.3.3/tests/data/input_type/telephone_input.html` & `browsergym_core-0.3.4/tests/data/input_type/telephone_input.html`

 * *Files identical despite different names*

### Comparing `browsergym_core-0.3.3/tests/data/input_type/text_input.html` & `browsergym_core-0.3.4/tests/data/input_type/text_input.html`

 * *Files identical despite different names*

### Comparing `browsergym_core-0.3.3/tests/data/input_type/time_input.html` & `browsergym_core-0.3.4/tests/data/input_type/time_input.html`

 * *Files identical despite different names*

### Comparing `browsergym_core-0.3.3/.gitignore` & `browsergym_core-0.3.4/.gitignore`

 * *Files identical despite different names*

### Comparing `browsergym_core-0.3.3/pyproject.toml` & `browsergym_core-0.3.4/pyproject.toml`

 * *Files identical despite different names*

### Comparing `browsergym_core-0.3.3/PKG-INFO` & `browsergym_core-0.3.4/PKG-INFO`

 * *Files 1% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.3
 Name: browsergym-core
-Version: 0.3.3
+Version: 0.3.4
 Summary: BrowserGym: a gym environment for web task automation in the Chromium browser
 Project-URL: homepage, https://github.com/ServiceNow/BrowserGym
 Author: Rim Assouel, Léo Boisvert, Massimo Caccia, Alex Drouin, Maxime Gasse, Alex Lacoste, Tom Marty
 License: Apache-2.0
 Classifier: Development Status :: 2 - Pre-Alpha
 Classifier: Intended Audience :: Science/Research
 Classifier: License :: OSI Approved :: Apache Software License
```

