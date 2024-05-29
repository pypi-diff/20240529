# Comparing `tmp/pytest_robotframework-4.2.0.tar.gz` & `tmp/pytest_robotframework-4.2.1.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "pytest_robotframework-4.2.0.tar", last modified: Fri May 24 04:48:03 2024, max compression
+gzip compressed data, was "pytest_robotframework-4.2.1.tar", last modified: Wed May 29 08:03:58 2024, max compression
```

## Comparing `pytest_robotframework-4.2.0.tar` & `pytest_robotframework-4.2.1.tar`

### file list

```diff
@@ -1,277 +1,278 @@
--rw-r--r--   0        0        0     1067 2024-05-24 04:47:50.211513 pytest_robotframework-4.2.0/LICENSE
--rw-r--r--   0        0        0    17559 2024-05-24 04:47:50.211513 pytest_robotframework-4.2.0/README.md
--rw-r--r--   0        0        0     8026 2024-05-24 04:48:03.739571 pytest_robotframework-4.2.0/pyproject.toml
--rw-r--r--   0        0        0    28462 2024-05-24 04:47:50.215513 pytest_robotframework-4.2.0/pytest_robotframework/__init__.py
--rw-r--r--   0        0        0        0 2024-05-24 04:47:50.215513 pytest_robotframework-4.2.0/pytest_robotframework/_internal/__init__.py
--rw-r--r--   0        0        0      559 2024-05-24 04:47:50.215513 pytest_robotframework-4.2.0/pytest_robotframework/_internal/cringe_globals.py
--rw-r--r--   0        0        0      921 2024-05-24 04:47:50.215513 pytest_robotframework-4.2.0/pytest_robotframework/_internal/errors.py
--rw-r--r--   0        0        0        0 2024-05-24 04:47:50.215513 pytest_robotframework-4.2.0/pytest_robotframework/_internal/pytest/__init__.py
--rw-r--r--   0        0        0      230 2024-05-24 04:47:50.215513 pytest_robotframework-4.2.0/pytest_robotframework/_internal/pytest/exception_getter.py
--rw-r--r--   0        0        0    26433 2024-05-24 04:47:50.215513 pytest_robotframework-4.2.0/pytest_robotframework/_internal/pytest/plugin.py
--rw-r--r--   0        0        0     7021 2024-05-24 04:47:50.215513 pytest_robotframework-4.2.0/pytest_robotframework/_internal/pytest/robot_file_support.py
--rw-r--r--   0        0        0     1181 2024-05-24 04:47:50.215513 pytest_robotframework-4.2.0/pytest_robotframework/_internal/pytest/xdist_utils.py
--rw-r--r--   0        0        0        0 2024-05-24 04:47:50.215513 pytest_robotframework-4.2.0/pytest_robotframework/_internal/robot/__init__.py
--rw-r--r--   0        0        0     4528 2024-05-24 04:47:50.215513 pytest_robotframework-4.2.0/pytest_robotframework/_internal/robot/library.py
--rw-r--r--   0        0        0    26358 2024-05-24 04:47:50.215513 pytest_robotframework-4.2.0/pytest_robotframework/_internal/robot/listeners_and_suite_visitors.py
--rw-r--r--   0        0        0     9785 2024-05-24 04:47:50.215513 pytest_robotframework-4.2.0/pytest_robotframework/_internal/robot/utils.py
--rw-r--r--   0        0        0     2045 2024-05-24 04:47:50.215513 pytest_robotframework-4.2.0/pytest_robotframework/_internal/utils.py
--rw-r--r--   0        0        0     3240 2024-05-24 04:47:50.215513 pytest_robotframework-4.2.0/pytest_robotframework/hooks.py
--rw-r--r--   0        0        0        0 2024-05-24 04:47:50.215513 pytest_robotframework-4.2.0/pytest_robotframework/py.typed
--rw-r--r--   0        0        0        0 2024-05-24 04:47:50.215513 pytest_robotframework-4.2.0/scripts/__init__.py
--rw-r--r--   0        0        0      177 2024-05-24 04:47:50.215513 pytest_robotframework-4.2.0/scripts/clear_pycache.py
--rw-r--r--   0        0        0        0 2024-05-24 04:47:50.215513 pytest_robotframework-4.2.0/tests/__init__.py
--rw-r--r--   0        0        0    13801 2024-05-24 04:47:50.215513 pytest_robotframework-4.2.0/tests/conftest.py
--rw-r--r--   0        0        0      230 2024-05-24 04:47:50.215513 pytest_robotframework-4.2.0/tests/fixtures/__init__.py
--rw-r--r--   0        0        0        0 2024-05-24 04:47:50.215513 pytest_robotframework-4.2.0/tests/fixtures/test_common/test_no_tests_found_no_files/.gitkeep
--rw-r--r--   0        0        0        0 2024-05-24 04:47:50.215513 pytest_robotframework-4.2.0/tests/fixtures/test_common/test_robot_file_and_python_file/__init__.py
--rw-r--r--   0        0        0       40 2024-05-24 04:47:50.215513 pytest_robotframework-4.2.0/tests/fixtures/test_common/test_robot_file_and_python_file/foo.robot
--rw-r--r--   0        0        0       57 2024-05-24 04:47:50.215513 pytest_robotframework-4.2.0/tests/fixtures/test_common/test_robot_file_and_python_file/test_bar.py
--rw-r--r--   0        0        0        0 2024-05-24 04:47:50.215513 pytest_robotframework-4.2.0/tests/fixtures/test_python/__init__.py
--rw-r--r--   0        0        0      104 2024-05-24 04:47:50.215513 pytest_robotframework-4.2.0/tests/fixtures/test_python/test_ansi.py
--rw-r--r--   0        0        0      186 2024-05-24 04:47:50.215513 pytest_robotframework-4.2.0/tests/fixtures/test_python/test_as_keyword_args_and_kwargs.py
--rw-r--r--   0        0        0      296 2024-05-24 04:47:50.215513 pytest_robotframework-4.2.0/tests/fixtures/test_python/test_as_keyword_context_manager_try_except.py
--rw-r--r--   0        0        0      105 2024-05-24 04:47:50.215513 pytest_robotframework-4.2.0/tests/fixtures/test_python/test_assertion_fails.py
--rw-r--r--   0        0        0      105 2024-05-24 04:47:50.215513 pytest_robotframework-4.2.0/tests/fixtures/test_python/test_assertion_fails_with_assertion_hook.py
--rw-r--r--   0        0        0      195 2024-05-24 04:47:50.215513 pytest_robotframework-4.2.0/tests/fixtures/test_python/test_assertion_fails_with_description.py
--rw-r--r--   0        0        0      196 2024-05-24 04:47:50.215513 pytest_robotframework-4.2.0/tests/fixtures/test_python/test_assertion_fails_with_fail_message_hide_assert.py
--rw-r--r--   0        0        0      175 2024-05-24 04:47:50.215513 pytest_robotframework-4.2.0/tests/fixtures/test_python/test_assertion_pass_hook_multiple_tests.py
--rw-r--r--   0        0        0      105 2024-05-24 04:47:50.215513 pytest_robotframework-4.2.0/tests/fixtures/test_python/test_assertion_passes.py
--rw-r--r--   0        0        0      435 2024-05-24 04:47:50.215513 pytest_robotframework-4.2.0/tests/fixtures/test_python/test_assertion_passes_custom_messages.py
--rw-r--r--   0        0        0      253 2024-05-24 04:47:50.215513 pytest_robotframework-4.2.0/tests/fixtures/test_python/test_assertion_passes_hide_assert.py
--rw-r--r--   0        0        0      359 2024-05-24 04:47:50.215513 pytest_robotframework-4.2.0/tests/fixtures/test_python/test_assertion_passes_hide_asserts_context_manager.py
--rw-r--r--   0        0        0      292 2024-05-24 04:47:50.215513 pytest_robotframework-4.2.0/tests/fixtures/test_python/test_assertion_passes_show_assert_when_no_assertions_in_robot_log.py
--rw-r--r--   0        0        0        0 2024-05-24 04:47:50.215513 pytest_robotframework-4.2.0/tests/fixtures/test_python/test_assertion_rewritten_in_conftest_when_assertion_hook_enabled/__init__.py
--rw-r--r--   0        0        0       80 2024-05-24 04:47:50.215513 pytest_robotframework-4.2.0/tests/fixtures/test_python/test_assertion_rewritten_in_conftest_when_assertion_hook_enabled/conftest.py
--rw-r--r--   0        0        0       57 2024-05-24 04:47:50.215513 pytest_robotframework-4.2.0/tests/fixtures/test_python/test_assertion_rewritten_in_conftest_when_assertion_hook_enabled/test_foo.py
--rw-r--r--   0        0        0        0 2024-05-24 04:47:50.215513 pytest_robotframework-4.2.0/tests/fixtures/test_python/test_catch_errors_decorator/__init__.py
--rw-r--r--   0        0        0      536 2024-05-24 04:47:50.215513 pytest_robotframework-4.2.0/tests/fixtures/test_python/test_catch_errors_decorator/conftest.py
--rw-r--r--   0        0        0       67 2024-05-24 04:47:50.215513 pytest_robotframework-4.2.0/tests/fixtures/test_python/test_catch_errors_decorator/test_foo.py
--rw-r--r--   0        0        0        0 2024-05-24 04:47:50.215513 pytest_robotframework-4.2.0/tests/fixtures/test_python/test_catch_errors_decorator_with_non_instance_method/__init__.py
--rw-r--r--   0        0        0      678 2024-05-24 04:47:50.215513 pytest_robotframework-4.2.0/tests/fixtures/test_python/test_catch_errors_decorator_with_non_instance_method/conftest.py
--rw-r--r--   0        0        0       67 2024-05-24 04:47:50.215513 pytest_robotframework-4.2.0/tests/fixtures/test_python/test_catch_errors_decorator_with_non_instance_method/test_foo.py
--rw-r--r--   0        0        0      163 2024-05-24 04:47:50.215513 pytest_robotframework-4.2.0/tests/fixtures/test_python/test_class_has_separate_suite.py
--rw-r--r--   0        0        0        0 2024-05-24 04:47:50.215513 pytest_robotframework-4.2.0/tests/fixtures/test_python/test_class_separate_files/__init__.py
--rw-r--r--   0        0        0      121 2024-05-24 04:47:50.215513 pytest_robotframework-4.2.0/tests/fixtures/test_python/test_class_separate_files/test_suite1.py
--rw-r--r--   0        0        0      121 2024-05-24 04:47:50.215513 pytest_robotframework-4.2.0/tests/fixtures/test_python/test_class_separate_files/test_suite2.py
--rw-r--r--   0        0        0      228 2024-05-24 04:47:50.215513 pytest_robotframework-4.2.0/tests/fixtures/test_python/test_class_three_tests_one_fail.py
--rw-r--r--   0        0        0        0 2024-05-24 04:47:50.215513 pytest_robotframework-4.2.0/tests/fixtures/test_python/test_collect_only_nested_suites/asdf/__init__.py
--rw-r--r--   0        0        0       64 2024-05-24 04:47:50.215513 pytest_robotframework-4.2.0/tests/fixtures/test_python/test_collect_only_nested_suites/asdf/test_bar.py
--rw-r--r--   0        0        0       64 2024-05-24 04:47:50.215513 pytest_robotframework-4.2.0/tests/fixtures/test_python/test_collect_only_nested_suites/asdf/test_foo.py
--rw-r--r--   0        0        0        8 2024-05-24 04:47:50.215513 pytest_robotframework-4.2.0/tests/fixtures/test_python/test_config_file_and_cwd_in_different_location/config/tox.ini
--rw-r--r--   0        0        0        0 2024-05-24 04:47:50.215513 pytest_robotframework-4.2.0/tests/fixtures/test_python/test_config_file_and_cwd_in_different_location/foo/.gitkeep
--rw-r--r--   0        0        0        0 2024-05-24 04:47:50.215513 pytest_robotframework-4.2.0/tests/fixtures/test_python/test_config_file_and_cwd_in_different_location/tests/__init__.py
--rw-r--r--   0        0        0       57 2024-05-24 04:47:50.215513 pytest_robotframework-4.2.0/tests/fixtures/test_python/test_config_file_and_cwd_in_different_location/tests/test_foo.py
--rw-r--r--   0        0        0        0 2024-05-24 04:47:50.215513 pytest_robotframework-4.2.0/tests/fixtures/test_python/test_config_file_in_different_location/__init__.py
--rw-r--r--   0        0        0        8 2024-05-24 04:47:50.215513 pytest_robotframework-4.2.0/tests/fixtures/test_python/test_config_file_in_different_location/asdf/tox.ini
--rw-r--r--   0        0        0       57 2024-05-24 04:47:50.215513 pytest_robotframework-4.2.0/tests/fixtures/test_python/test_config_file_in_different_location/test_asdf.py
--rw-r--r--   0        0        0      254 2024-05-24 04:47:50.215513 pytest_robotframework-4.2.0/tests/fixtures/test_python/test_console_output.py
--rw-r--r--   0        0        0       66 2024-05-24 04:47:50.215513 pytest_robotframework-4.2.0/tests/fixtures/test_python/test_console_summary.py
--rw-r--r--   0        0        0        0 2024-05-24 04:47:50.215513 pytest_robotframework-4.2.0/tests/fixtures/test_python/test_correct_items_collected_when_collect_only/__init__.py
--rw-r--r--   0        0        0       64 2024-05-24 04:47:50.215513 pytest_robotframework-4.2.0/tests/fixtures/test_python/test_correct_items_collected_when_collect_only/test_bar.py
--rw-r--r--   0        0        0       64 2024-05-24 04:47:50.215513 pytest_robotframework-4.2.0/tests/fixtures/test_python/test_correct_items_collected_when_collect_only/test_foo.py
--rw-r--r--   0        0        0       87 2024-05-24 04:47:50.215513 pytest_robotframework-4.2.0/tests/fixtures/test_python/test_doesnt_run_when_collecting.py
--rw-r--r--   0        0        0      130 2024-05-24 04:47:50.215513 pytest_robotframework-4.2.0/tests/fixtures/test_python/test_error_moment.py
--rw-r--r--   0        0        0      148 2024-05-24 04:47:50.215513 pytest_robotframework-4.2.0/tests/fixtures/test_python/test_error_moment_and_second_test.py
--rw-r--r--   0        0        0      130 2024-05-24 04:47:50.215513 pytest_robotframework-4.2.0/tests/fixtures/test_python/test_error_moment_exitonerror.py
--rw-r--r--   0        0        0      171 2024-05-24 04:47:50.215513 pytest_robotframework-4.2.0/tests/fixtures/test_python/test_error_moment_exitonerror_multiple_tests.py
--rw-r--r--   0        0        0        0 2024-05-24 04:47:50.215513 pytest_robotframework-4.2.0/tests/fixtures/test_python/test_error_moment_setup/__init__.py
--rw-r--r--   0        0        0      142 2024-05-24 04:47:50.215513 pytest_robotframework-4.2.0/tests/fixtures/test_python/test_error_moment_setup/conftest.py
--rw-r--r--   0        0        0      106 2024-05-24 04:47:50.215513 pytest_robotframework-4.2.0/tests/fixtures/test_python/test_error_moment_setup/test_foo.py
--rw-r--r--   0        0        0        0 2024-05-24 04:47:50.215513 pytest_robotframework-4.2.0/tests/fixtures/test_python/test_error_moment_teardown/__init__.py
--rw-r--r--   0        0        0      145 2024-05-24 04:47:50.215513 pytest_robotframework-4.2.0/tests/fixtures/test_python/test_error_moment_teardown/conftest.py
--rw-r--r--   0        0        0      106 2024-05-24 04:47:50.215513 pytest_robotframework-4.2.0/tests/fixtures/test_python/test_error_moment_teardown/test_foo.py
--rw-r--r--   0        0        0      163 2024-05-24 04:47:50.215513 pytest_robotframework-4.2.0/tests/fixtures/test_python/test_fixture.py
--rw-r--r--   0        0        0      625 2024-05-24 04:47:50.215513 pytest_robotframework-4.2.0/tests/fixtures/test_python/test_fixture_scope.py
--rw-r--r--   0        0        0      225 2024-05-24 04:47:50.219513 pytest_robotframework-4.2.0/tests/fixtures/test_python/test_full_stack_keyword_context_manager.py
--rw-r--r--   0        0        0      152 2024-05-24 04:47:50.219513 pytest_robotframework-4.2.0/tests/fixtures/test_python/test_full_stack_keyword_decorator.py
--rw-r--r--   0        0        0       82 2024-05-24 04:47:50.219513 pytest_robotframework-4.2.0/tests/fixtures/test_python/test_invalid_fixture.py
--rw-r--r--   0        0        0      243 2024-05-24 04:47:50.219513 pytest_robotframework-4.2.0/tests/fixtures/test_python/test_keyword_and_pytest_raises.py
--rw-r--r--   0        0        0      218 2024-05-24 04:47:50.219513 pytest_robotframework-4.2.0/tests/fixtures/test_python/test_keyword_decorator_args.py
--rw-r--r--   0        0        0      554 2024-05-24 04:47:50.219513 pytest_robotframework-4.2.0/tests/fixtures/test_python/test_keyword_decorator_context_manager_that_doesnt_suppress.py
--rw-r--r--   0        0        0      542 2024-05-24 04:47:50.219513 pytest_robotframework-4.2.0/tests/fixtures/test_python/test_keyword_decorator_context_manager_that_raises_in_body_and_exit.py
--rw-r--r--   0        0        0      468 2024-05-24 04:47:50.219513 pytest_robotframework-4.2.0/tests/fixtures/test_python/test_keyword_decorator_context_manager_that_raises_in_exit.py
--rw-r--r--   0        0        0      171 2024-05-24 04:47:50.219513 pytest_robotframework-4.2.0/tests/fixtures/test_python/test_keyword_decorator_custom_name_and_tags.py
--rw-r--r--   0        0        0      148 2024-05-24 04:47:50.219513 pytest_robotframework-4.2.0/tests/fixtures/test_python/test_keyword_decorator_docstring.py
--rw-r--r--   0        0        0      178 2024-05-24 04:47:50.219513 pytest_robotframework-4.2.0/tests/fixtures/test_python/test_keyword_decorator_docstring_on_next_line.py
--rw-r--r--   0        0        0      445 2024-05-24 04:47:50.219513 pytest_robotframework-4.2.0/tests/fixtures/test_python/test_keyword_decorator_returns_context_manager_that_isnt_used.py
--rw-r--r--   0        0        0      275 2024-05-24 04:47:50.219513 pytest_robotframework-4.2.0/tests/fixtures/test_python/test_keyword_decorator_try_except.py
--rw-r--r--   0        0        0       85 2024-05-24 04:47:50.219513 pytest_robotframework-4.2.0/tests/fixtures/test_python/test_keyword_names.py
--rw-r--r--   0        0        0      273 2024-05-24 04:47:50.219513 pytest_robotframework-4.2.0/tests/fixtures/test_python/test_keyword_raises.py
--rw-r--r--   0        0        0      166 2024-05-24 04:47:50.219513 pytest_robotframework-4.2.0/tests/fixtures/test_python/test_keywordify_context_manager.py
--rw-r--r--   0        0        0      127 2024-05-24 04:47:50.219513 pytest_robotframework-4.2.0/tests/fixtures/test_python/test_keywordify_function.py
--rw-r--r--   0        0        0      280 2024-05-24 04:47:50.219513 pytest_robotframework-4.2.0/tests/fixtures/test_python/test_keywordify_keyword_inside_context_manager.py
--rw-r--r--   0        0        0      545 2024-05-24 04:47:50.219513 pytest_robotframework-4.2.0/tests/fixtures/test_python/test_listener_calls_log_file/Listener.py
--rw-r--r--   0        0        0        0 2024-05-24 04:47:50.219513 pytest_robotframework-4.2.0/tests/fixtures/test_python/test_listener_calls_log_file/__init__.py
--rw-r--r--   0        0        0       64 2024-05-24 04:47:50.219513 pytest_robotframework-4.2.0/tests/fixtures/test_python/test_listener_calls_log_file/test_foo.py
--rw-r--r--   0        0        0        0 2024-05-24 04:47:50.219513 pytest_robotframework-4.2.0/tests/fixtures/test_python/test_listener_not_run_during_collection/__init__.py
--rw-r--r--   0        0        0      597 2024-05-24 04:47:50.219513 pytest_robotframework-4.2.0/tests/fixtures/test_python/test_listener_not_run_during_collection/conftest.py
--rw-r--r--   0        0        0      105 2024-05-24 04:47:50.219513 pytest_robotframework-4.2.0/tests/fixtures/test_python/test_listener_not_run_during_collection/test_foo.py
--rw-r--r--   0        0        0       77 2024-05-24 04:47:50.219513 pytest_robotframework-4.2.0/tests/fixtures/test_python/test_module_docstring.py
--rw-r--r--   0        0        0       62 2024-05-24 04:47:50.219513 pytest_robotframework-4.2.0/tests/fixtures/test_python/test_multiple_runs.py
--rw-r--r--   0        0        0      186 2024-05-24 04:47:50.219513 pytest_robotframework-4.2.0/tests/fixtures/test_python/test_nested_class.py
--rw-r--r--   0        0        0      188 2024-05-24 04:47:50.219513 pytest_robotframework-4.2.0/tests/fixtures/test_python/test_nested_keyword_that_fails.py
--rw-r--r--   0        0        0      107 2024-05-24 04:47:50.219513 pytest_robotframework-4.2.0/tests/fixtures/test_python/test_nested_suites/suite1/suite2/test_asdf.py
--rw-r--r--   0        0        0      107 2024-05-24 04:47:50.219513 pytest_robotframework-4.2.0/tests/fixtures/test_python/test_nested_suites/suite1/suite3/test_asdf2.py
--rw-r--r--   0        0        0      126 2024-05-24 04:47:50.219513 pytest_robotframework-4.2.0/tests/fixtures/test_python/test_nested_suites/test_top_level.py
--rw-r--r--   0        0        0       63 2024-05-24 04:47:50.219513 pytest_robotframework-4.2.0/tests/fixtures/test_python/test_no_tests_found_when_tests_exist.py
--rw-r--r--   0        0        0       92 2024-05-24 04:47:50.219513 pytest_robotframework-4.2.0/tests/fixtures/test_python/test_one_test_fails.py
--rw-r--r--   0        0        0       73 2024-05-24 04:47:50.219513 pytest_robotframework-4.2.0/tests/fixtures/test_python/test_one_test_passes.py
--rw-r--r--   0        0        0      162 2024-05-24 04:47:50.219513 pytest_robotframework-4.2.0/tests/fixtures/test_python/test_one_test_skipped.py
--rw-r--r--   0        0        0      100 2024-05-24 04:47:50.219513 pytest_robotframework-4.2.0/tests/fixtures/test_python/test_parameterized_tags.py
--rw-r--r--   0        0        0      207 2024-05-24 04:47:50.219513 pytest_robotframework-4.2.0/tests/fixtures/test_python/test_parametrize.py
--rw-r--r--   0        0        0        0 2024-05-24 04:47:50.219513 pytest_robotframework-4.2.0/tests/fixtures/test_python/test_pytest_runtest_protocol_hook_in_different_suite/a/__init__.py
--rw-r--r--   0        0        0      185 2024-05-24 04:47:50.219513 pytest_robotframework-4.2.0/tests/fixtures/test_python/test_pytest_runtest_protocol_hook_in_different_suite/a/test_c.py
--rw-r--r--   0        0        0        0 2024-05-24 04:47:50.219513 pytest_robotframework-4.2.0/tests/fixtures/test_python/test_pytest_runtest_protocol_hook_in_different_suite/b/__init__.py
--rw-r--r--   0        0        0       72 2024-05-24 04:47:50.219513 pytest_robotframework-4.2.0/tests/fixtures/test_python/test_pytest_runtest_protocol_hook_in_different_suite/b/conftest.py
--rw-r--r--   0        0        0        0 2024-05-24 04:47:50.219513 pytest_robotframework-4.2.0/tests/fixtures/test_python/test_pytest_runtest_protocol_item_hook/foo/__init__.py
--rw-r--r--   0        0        0      398 2024-05-24 04:47:50.219513 pytest_robotframework-4.2.0/tests/fixtures/test_python/test_pytest_runtest_protocol_item_hook/foo/conftest.py
--rw-r--r--   0        0        0       67 2024-05-24 04:47:50.219513 pytest_robotframework-4.2.0/tests/fixtures/test_python/test_pytest_runtest_protocol_item_hook/foo/test_foo.py
--rw-r--r--   0        0        0        0 2024-05-24 04:47:50.219513 pytest_robotframework-4.2.0/tests/fixtures/test_python/test_pytest_runtest_protocol_session_hook/__init__.py
--rw-r--r--   0        0        0      471 2024-05-24 04:47:50.219513 pytest_robotframework-4.2.0/tests/fixtures/test_python/test_pytest_runtest_protocol_session_hook/conftest.py
--rw-r--r--   0        0        0       67 2024-05-24 04:47:50.219513 pytest_robotframework-4.2.0/tests/fixtures/test_python/test_pytest_runtest_protocol_session_hook/test_foo.py
--rw-r--r--   0        0        0      296 2024-05-24 04:47:50.219513 pytest_robotframework-4.2.0/tests/fixtures/test_python/test_python_file_doesnt_get_parsed_as_robot_file.py
--rw-r--r--   0        0        0       64 2024-05-24 04:47:50.219513 pytest_robotframework-4.2.0/tests/fixtures/test_python/test_robot_args.py
--rw-r--r--   0        0        0        0 2024-05-24 04:47:50.219513 pytest_robotframework-4.2.0/tests/fixtures/test_python/test_robot_keyword_in_python_test/__init__.py
--rw-r--r--   0        0        0       34 2024-05-24 04:47:50.219513 pytest_robotframework-4.2.0/tests/fixtures/test_python/test_robot_keyword_in_python_test/bar/bar.resource
--rw-r--r--   0        0        0      262 2024-05-24 04:47:50.219513 pytest_robotframework-4.2.0/tests/fixtures/test_python/test_robot_keyword_in_python_test/test_foo.py
--rw-r--r--   0        0        0        0 2024-05-24 04:47:50.219513 pytest_robotframework-4.2.0/tests/fixtures/test_python/test_robot_modify_args_hook/__init__.py
--rw-r--r--   0        0        0      119 2024-05-24 04:47:50.219513 pytest_robotframework-4.2.0/tests/fixtures/test_python/test_robot_modify_args_hook/conftest.py
--rw-r--r--   0        0        0      222 2024-05-24 04:47:50.219513 pytest_robotframework-4.2.0/tests/fixtures/test_python/test_robot_modify_args_hook/test_foo.py
--rw-r--r--   0        0        0        0 2024-05-24 04:47:50.219513 pytest_robotframework-4.2.0/tests/fixtures/test_python/test_robot_modify_args_hook_collect_only/__init__.py
--rw-r--r--   0        0        0      175 2024-05-24 04:47:50.219513 pytest_robotframework-4.2.0/tests/fixtures/test_python/test_robot_modify_args_hook_collect_only/conftest.py
--rw-r--r--   0        0        0      221 2024-05-24 04:47:50.219513 pytest_robotframework-4.2.0/tests/fixtures/test_python/test_robot_modify_args_hook_collect_only/test_foo.py
--rw-r--r--   0        0        0        0 2024-05-24 04:47:50.219513 pytest_robotframework-4.2.0/tests/fixtures/test_python/test_robot_modify_options_hook/__init__.py
--rw-r--r--   0        0        0      235 2024-05-24 04:47:50.219513 pytest_robotframework-4.2.0/tests/fixtures/test_python/test_robot_modify_options_hook/conftest.py
--rw-r--r--   0        0        0      222 2024-05-24 04:47:50.219513 pytest_robotframework-4.2.0/tests/fixtures/test_python/test_robot_modify_options_hook/test_foo.py
--rw-r--r--   0        0        0        0 2024-05-24 04:47:50.219513 pytest_robotframework-4.2.0/tests/fixtures/test_python/test_robot_modify_options_hook_listener_instance/__init__.py
--rw-r--r--   0        0        0      630 2024-05-24 04:47:50.219513 pytest_robotframework-4.2.0/tests/fixtures/test_python/test_robot_modify_options_hook_listener_instance/conftest.py
--rw-r--r--   0        0        0       62 2024-05-24 04:47:50.219513 pytest_robotframework-4.2.0/tests/fixtures/test_python/test_robot_modify_options_hook_listener_instance/test_foo.py
--rw-r--r--   0        0        0      498 2024-05-24 04:47:50.219513 pytest_robotframework-4.2.0/tests/fixtures/test_python/test_robot_options_merge_listeners/Listener.py
--rw-r--r--   0        0        0        0 2024-05-24 04:47:50.219513 pytest_robotframework-4.2.0/tests/fixtures/test_python/test_robot_options_merge_listeners/__init__.py
--rw-r--r--   0        0        0      322 2024-05-24 04:47:50.219513 pytest_robotframework-4.2.0/tests/fixtures/test_python/test_robot_options_merge_listeners/test_foo.py
--rw-r--r--   0        0        0       64 2024-05-24 04:47:50.219513 pytest_robotframework-4.2.0/tests/fixtures/test_python/test_robot_options_variable.py
--rw-r--r--   0        0        0      498 2024-05-24 04:47:50.219513 pytest_robotframework-4.2.0/tests/fixtures/test_python/test_robot_options_variable_merge_listeners/Listener.py
--rw-r--r--   0        0        0        0 2024-05-24 04:47:50.219513 pytest_robotframework-4.2.0/tests/fixtures/test_python/test_robot_options_variable_merge_listeners/__init__.py
--rw-r--r--   0        0        0      322 2024-05-24 04:47:50.219513 pytest_robotframework-4.2.0/tests/fixtures/test_python/test_robot_options_variable_merge_listeners/test_foo.py
--rw-r--r--   0        0        0        0 2024-05-24 04:47:50.219513 pytest_robotframework-4.2.0/tests/fixtures/test_python/test_run_two_files/__init__.py
--rw-r--r--   0        0        0       55 2024-05-24 04:47:50.219513 pytest_robotframework-4.2.0/tests/fixtures/test_python/test_run_two_files/test_a.py
--rw-r--r--   0        0        0       55 2024-05-24 04:47:50.219513 pytest_robotframework-4.2.0/tests/fixtures/test_python/test_run_two_files/test_b.py
--rw-r--r--   0        0        0      236 2024-05-24 04:47:50.219513 pytest_robotframework-4.2.0/tests/fixtures/test_python/test_set_log_level.py
--rw-r--r--   0        0        0        0 2024-05-24 04:47:50.219513 pytest_robotframework-4.2.0/tests/fixtures/test_python/test_setup_fails/__init__.py
--rw-r--r--   0        0        0       90 2024-05-24 04:47:50.219513 pytest_robotframework-4.2.0/tests/fixtures/test_python/test_setup_fails/conftest.py
--rw-r--r--   0        0        0       73 2024-05-24 04:47:50.219513 pytest_robotframework-4.2.0/tests/fixtures/test_python/test_setup_fails/test_foo.py
--rw-r--r--   0        0        0        0 2024-05-24 04:47:50.219513 pytest_robotframework-4.2.0/tests/fixtures/test_python/test_setup_passes/__init__.py
--rw-r--r--   0        0        0      116 2024-05-24 04:47:50.219513 pytest_robotframework-4.2.0/tests/fixtures/test_python/test_setup_passes/conftest.py
--rw-r--r--   0        0        0      116 2024-05-24 04:47:50.219513 pytest_robotframework-4.2.0/tests/fixtures/test_python/test_setup_passes/test_foo.py
--rw-r--r--   0        0        0        0 2024-05-24 04:47:50.219513 pytest_robotframework-4.2.0/tests/fixtures/test_python/test_setup_skipped/__init__.py
--rw-r--r--   0        0        0      101 2024-05-24 04:47:50.219513 pytest_robotframework-4.2.0/tests/fixtures/test_python/test_setup_skipped/conftest.py
--rw-r--r--   0        0        0       73 2024-05-24 04:47:50.219513 pytest_robotframework-4.2.0/tests/fixtures/test_python/test_setup_skipped/test_foo.py
--rw-r--r--   0        0        0      305 2024-05-24 04:47:50.219513 pytest_robotframework-4.2.0/tests/fixtures/test_python/test_suite_variables.py
--rw-r--r--   0        0        0      313 2024-05-24 04:47:50.219513 pytest_robotframework-4.2.0/tests/fixtures/test_python/test_suite_variables_with_slash.py
--rw-r--r--   0        0        0      107 2024-05-24 04:47:50.219513 pytest_robotframework-4.2.0/tests/fixtures/test_python/test_suites/suite1/test_asdf.py
--rw-r--r--   0        0        0       94 2024-05-24 04:47:50.219513 pytest_robotframework-4.2.0/tests/fixtures/test_python/test_tags.py
--rw-r--r--   0        0        0        0 2024-05-24 04:47:50.219513 pytest_robotframework-4.2.0/tests/fixtures/test_python/test_teardown_fails/__init__.py
--rw-r--r--   0        0        0       93 2024-05-24 04:47:50.219513 pytest_robotframework-4.2.0/tests/fixtures/test_python/test_teardown_fails/conftest.py
--rw-r--r--   0        0        0       73 2024-05-24 04:47:50.219513 pytest_robotframework-4.2.0/tests/fixtures/test_python/test_teardown_fails/test_foo.py
--rw-r--r--   0        0        0        0 2024-05-24 04:47:50.219513 pytest_robotframework-4.2.0/tests/fixtures/test_python/test_teardown_passes/__init__.py
--rw-r--r--   0        0        0      119 2024-05-24 04:47:50.219513 pytest_robotframework-4.2.0/tests/fixtures/test_python/test_teardown_passes/conftest.py
--rw-r--r--   0        0        0      115 2024-05-24 04:47:50.219513 pytest_robotframework-4.2.0/tests/fixtures/test_python/test_teardown_passes/test_foo.py
--rw-r--r--   0        0        0        0 2024-05-24 04:47:50.219513 pytest_robotframework-4.2.0/tests/fixtures/test_python/test_teardown_skipped/__init__.py
--rw-r--r--   0        0        0      104 2024-05-24 04:47:50.219513 pytest_robotframework-4.2.0/tests/fixtures/test_python/test_teardown_skipped/conftest.py
--rw-r--r--   0        0        0       73 2024-05-24 04:47:50.219513 pytest_robotframework-4.2.0/tests/fixtures/test_python/test_teardown_skipped/test_foo.py
--rw-r--r--   0        0        0       78 2024-05-24 04:47:50.219513 pytest_robotframework-4.2.0/tests/fixtures/test_python/test_test_case_docstring.py
--rw-r--r--   0        0        0       80 2024-05-24 04:47:50.219513 pytest_robotframework-4.2.0/tests/fixtures/test_python/test_trace_ricing.py
--rw-r--r--   0        0        0      106 2024-05-24 04:47:50.219513 pytest_robotframework-4.2.0/tests/fixtures/test_python/test_traceback.py
--rw-r--r--   0        0        0      108 2024-05-24 04:47:50.219513 pytest_robotframework-4.2.0/tests/fixtures/test_python/test_two_tests_one_fail_one_pass.py
--rw-r--r--   0        0        0       77 2024-05-24 04:47:50.219513 pytest_robotframework-4.2.0/tests/fixtures/test_python/test_two_tests_specified_by_full_path.py
--rw-r--r--   0        0        0        0 2024-05-24 04:47:50.223513 pytest_robotframework-4.2.0/tests/fixtures/test_python/test_two_tests_specified_by_full_path_in_different_files/__init__.py
--rw-r--r--   0        0        0       62 2024-05-24 04:47:50.223513 pytest_robotframework-4.2.0/tests/fixtures/test_python/test_two_tests_specified_by_full_path_in_different_files/test_bar.py
--rw-r--r--   0        0        0       62 2024-05-24 04:47:50.223513 pytest_robotframework-4.2.0/tests/fixtures/test_python/test_two_tests_specified_by_full_path_in_different_files/test_foo.py
--rw-r--r--   0        0        0        0 2024-05-24 04:47:50.223513 pytest_robotframework-4.2.0/tests/fixtures/test_python/test_two_tests_two_files_one_fail_one_pass/__init__.py
--rw-r--r--   0        0        0       64 2024-05-24 04:47:50.223513 pytest_robotframework-4.2.0/tests/fixtures/test_python/test_two_tests_two_files_one_fail_one_pass/test_one.py
--rw-r--r--   0        0        0       83 2024-05-24 04:47:50.223513 pytest_robotframework-4.2.0/tests/fixtures/test_python/test_two_tests_two_files_one_fail_one_pass/test_two.py
--rw-r--r--   0        0        0        0 2024-05-24 04:47:50.223513 pytest_robotframework-4.2.0/tests/fixtures/test_python/test_two_tests_with_same_name_one_fail_one_pass/__init__.py
--rw-r--r--   0        0        0       63 2024-05-24 04:47:50.223513 pytest_robotframework-4.2.0/tests/fixtures/test_python/test_two_tests_with_same_name_one_fail_one_pass/test_one.py
--rw-r--r--   0        0        0       82 2024-05-24 04:47:50.223513 pytest_robotframework-4.2.0/tests/fixtures/test_python/test_two_tests_with_same_name_one_fail_one_pass/test_two.py
--rw-r--r--   0        0        0      121 2024-05-24 04:47:50.223513 pytest_robotframework-4.2.0/tests/fixtures/test_python/test_unittest_class.py
--rw-r--r--   0        0        0      311 2024-05-24 04:47:50.223513 pytest_robotframework-4.2.0/tests/fixtures/test_python/test_variables_list.py
--rw-r--r--   0        0        0        0 2024-05-24 04:47:50.223513 pytest_robotframework-4.2.0/tests/fixtures/test_python/test_variables_not_in_scope_in_other_suites/__init__.py
--rw-r--r--   0        0        0      303 2024-05-24 04:47:50.223513 pytest_robotframework-4.2.0/tests/fixtures/test_python/test_variables_not_in_scope_in_other_suites/test_one.py
--rw-r--r--   0        0        0      222 2024-05-24 04:47:50.223513 pytest_robotframework-4.2.0/tests/fixtures/test_python/test_variables_not_in_scope_in_other_suites/test_two.py
--rw-r--r--   0        0        0       57 2024-05-24 04:47:50.223513 pytest_robotframework-4.2.0/tests/fixtures/test_python/test_xdist_n_0.py
--rw-r--r--   0        0        0        0 2024-05-24 04:47:50.223513 pytest_robotframework-4.2.0/tests/fixtures/test_python/test_xfail_fails/__init__.py
--rw-r--r--   0        0        0      133 2024-05-24 04:47:50.223513 pytest_robotframework-4.2.0/tests/fixtures/test_python/test_xfail_fails/test_foo.py
--rw-r--r--   0        0        0       28 2024-05-24 04:47:50.223513 pytest_robotframework-4.2.0/tests/fixtures/test_python/test_xfail_fails/tox.ini
--rw-r--r--   0        0        0        0 2024-05-24 04:47:50.223513 pytest_robotframework-4.2.0/tests/fixtures/test_python/test_xfail_fails_no_reason/__init__.py
--rw-r--r--   0        0        0      118 2024-05-24 04:47:50.223513 pytest_robotframework-4.2.0/tests/fixtures/test_python/test_xfail_fails_no_reason/test_foo.py
--rw-r--r--   0        0        0       28 2024-05-24 04:47:50.223513 pytest_robotframework-4.2.0/tests/fixtures/test_python/test_xfail_fails_no_reason/tox.ini
--rw-r--r--   0        0        0        0 2024-05-24 04:47:50.223513 pytest_robotframework-4.2.0/tests/fixtures/test_python/test_xfail_passes/__init__.py
--rw-r--r--   0        0        0      123 2024-05-24 04:47:50.223513 pytest_robotframework-4.2.0/tests/fixtures/test_python/test_xfail_passes/test_foo.py
--rw-r--r--   0        0        0       28 2024-05-24 04:47:50.223513 pytest_robotframework-4.2.0/tests/fixtures/test_python/test_xfail_passes/tox.ini
--rw-r--r--   0        0        0        0 2024-05-24 04:47:50.223513 pytest_robotframework-4.2.0/tests/fixtures/test_python/test_xfail_passes_no_reason/__init__.py
--rw-r--r--   0        0        0      107 2024-05-24 04:47:50.223513 pytest_robotframework-4.2.0/tests/fixtures/test_python/test_xfail_passes_no_reason/test_foo.py
--rw-r--r--   0        0        0       28 2024-05-24 04:47:50.223513 pytest_robotframework-4.2.0/tests/fixtures/test_python/test_xfail_passes_no_reason/tox.ini
--rw-r--r--   0        0        0       32 2024-05-24 04:47:50.223513 pytest_robotframework-4.2.0/tests/fixtures/test_robot/test_collect_only_nested_suites/bar.robot
--rw-r--r--   0        0        0       32 2024-05-24 04:47:50.223513 pytest_robotframework-4.2.0/tests/fixtures/test_robot/test_collect_only_nested_suites/foo.robot
--rw-r--r--   0        0        0       32 2024-05-24 04:47:50.223513 pytest_robotframework-4.2.0/tests/fixtures/test_robot/test_correct_items_collected_when_collect_only/bar.robot
--rw-r--r--   0        0        0       32 2024-05-24 04:47:50.223513 pytest_robotframework-4.2.0/tests/fixtures/test_robot/test_correct_items_collected_when_collect_only/foo.robot
--rw-r--r--   0        0        0       36 2024-05-24 04:47:50.223513 pytest_robotframework-4.2.0/tests/fixtures/test_robot/test_doesnt_run_tests_outside_path/bar/asdf.robot
--rw-r--r--   0        0        0       36 2024-05-24 04:47:50.223513 pytest_robotframework-4.2.0/tests/fixtures/test_robot/test_doesnt_run_tests_outside_path/foo/asdf.robot
--rw-r--r--   0        0        0       44 2024-05-24 04:47:50.223513 pytest_robotframework-4.2.0/tests/fixtures/test_robot/test_doesnt_run_when_collecting.robot
--rw-r--r--   0        0        0       99 2024-05-24 04:47:50.223513 pytest_robotframework-4.2.0/tests/fixtures/test_robot/test_fails_when_import_error_and_exit_on_error.robot
--rw-r--r--   0        0        0        0 2024-05-24 04:47:50.223513 pytest_robotframework-4.2.0/tests/fixtures/test_robot/test_init_file/__init__.py
--rw-r--r--   0        0        0       40 2024-05-24 04:47:50.223513 pytest_robotframework-4.2.0/tests/fixtures/test_robot/test_init_file/foo.robot
--rw-r--r--   0        0        0        0 2024-05-24 04:47:50.223513 pytest_robotframework-4.2.0/tests/fixtures/test_robot/test_init_file_nested/__init__.py
--rw-r--r--   0        0        0        0 2024-05-24 04:47:50.223513 pytest_robotframework-4.2.0/tests/fixtures/test_robot/test_init_file_nested/foo/__init__.py
--rw-r--r--   0        0        0       40 2024-05-24 04:47:50.223513 pytest_robotframework-4.2.0/tests/fixtures/test_robot/test_init_file_nested/foo/bar.robot
--rw-r--r--   0        0        0       40 2024-05-24 04:47:50.223513 pytest_robotframework-4.2.0/tests/fixtures/test_robot/test_init_file_nested/foo/foo.robot
--rw-r--r--   0        0        0        0 2024-05-24 04:47:50.223513 pytest_robotframework-4.2.0/tests/fixtures/test_robot/test_keyword_decorator/__init__.py
--rw-r--r--   0        0        0       71 2024-05-24 04:47:50.223513 pytest_robotframework-4.2.0/tests/fixtures/test_robot/test_keyword_decorator/bar.robot
--rw-r--r--   0        0        0      151 2024-05-24 04:47:50.223513 pytest_robotframework-4.2.0/tests/fixtures/test_robot/test_keyword_decorator/foo.py
--rw-r--r--   0        0        0        0 2024-05-24 04:47:50.223513 pytest_robotframework-4.2.0/tests/fixtures/test_robot/test_keyword_decorator_and_other_decorator/__init__.py
--rw-r--r--   0        0        0       71 2024-05-24 04:47:50.223513 pytest_robotframework-4.2.0/tests/fixtures/test_robot/test_keyword_decorator_and_other_decorator/bar.robot
--rw-r--r--   0        0        0      468 2024-05-24 04:47:50.223513 pytest_robotframework-4.2.0/tests/fixtures/test_robot/test_keyword_decorator_and_other_decorator/foo.py
--rw-r--r--   0        0        0      162 2024-05-24 04:47:50.223513 pytest_robotframework-4.2.0/tests/fixtures/test_robot/test_keyword_with_conflicting_name.robot
--rw-r--r--   0        0        0       62 2024-05-24 04:47:50.223513 pytest_robotframework-4.2.0/tests/fixtures/test_robot/test_line_number.robot
--rw-r--r--   0        0        0      535 2024-05-24 04:47:50.223513 pytest_robotframework-4.2.0/tests/fixtures/test_robot/test_listener_calls_log_file/Listener.py
--rw-r--r--   0        0        0        0 2024-05-24 04:47:50.223513 pytest_robotframework-4.2.0/tests/fixtures/test_robot/test_listener_calls_log_file/__init__.py
--rw-r--r--   0        0        0       40 2024-05-24 04:47:50.223513 pytest_robotframework-4.2.0/tests/fixtures/test_robot/test_listener_calls_log_file/foo.robot
--rw-r--r--   0        0        0        0 2024-05-24 04:47:50.223513 pytest_robotframework-4.2.0/tests/fixtures/test_robot/test_nested_keyword_that_fails/__init__.py
--rw-r--r--   0        0        0       71 2024-05-24 04:47:50.223513 pytest_robotframework-4.2.0/tests/fixtures/test_robot/test_nested_keyword_that_fails/bar.robot
--rw-r--r--   0        0        0      160 2024-05-24 04:47:50.223513 pytest_robotframework-4.2.0/tests/fixtures/test_robot/test_nested_keyword_that_fails/foo.py
--rw-r--r--   0        0        0       40 2024-05-24 04:47:50.223513 pytest_robotframework-4.2.0/tests/fixtures/test_robot/test_no_tests_found_when_tests_exist.robot
--rw-r--r--   0        0        0       32 2024-05-24 04:47:50.223513 pytest_robotframework-4.2.0/tests/fixtures/test_robot/test_one_test_fails.robot
--rw-r--r--   0        0        0       36 2024-05-24 04:47:50.223513 pytest_robotframework-4.2.0/tests/fixtures/test_robot/test_one_test_passes.robot
--rw-r--r--   0        0        0       32 2024-05-24 04:47:50.223513 pytest_robotframework-4.2.0/tests/fixtures/test_robot/test_one_test_skipped.robot
--rw-r--r--   0        0        0       61 2024-05-24 04:47:50.223513 pytest_robotframework-4.2.0/tests/fixtures/test_robot/test_parameterized_tags/foo.robot
--rw-r--r--   0        0        0       34 2024-05-24 04:47:50.223513 pytest_robotframework-4.2.0/tests/fixtures/test_robot/test_parameterized_tags/tox.ini
--rw-r--r--   0        0        0       95 2024-05-24 04:47:50.223513 pytest_robotframework-4.2.0/tests/fixtures/test_robot/test_run_keyword_and_ignore_error.robot
--rw-r--r--   0        0        0       38 2024-05-24 04:47:50.223513 pytest_robotframework-4.2.0/tests/fixtures/test_robot/test_run_two_files/a.robot
--rw-r--r--   0        0        0       38 2024-05-24 04:47:50.223513 pytest_robotframework-4.2.0/tests/fixtures/test_robot/test_run_two_files/b.robot
--rw-r--r--   0        0        0      115 2024-05-24 04:47:50.223513 pytest_robotframework-4.2.0/tests/fixtures/test_robot/test_setup_fails.robot
--rw-r--r--   0        0        0      111 2024-05-24 04:47:50.223513 pytest_robotframework-4.2.0/tests/fixtures/test_robot/test_setup_passes.robot
--rw-r--r--   0        0        0      107 2024-05-24 04:47:50.223513 pytest_robotframework-4.2.0/tests/fixtures/test_robot/test_setup_skipped.robot
--rw-r--r--   0        0        0      163 2024-05-24 04:47:50.223513 pytest_robotframework-4.2.0/tests/fixtures/test_robot/test_setup_with_args.robot
--rw-r--r--   0        0        0       96 2024-05-24 04:47:50.223513 pytest_robotframework-4.2.0/tests/fixtures/test_robot/test_tags.robot
--rw-r--r--   0        0        0      100 2024-05-24 04:47:50.223513 pytest_robotframework-4.2.0/tests/fixtures/test_robot/test_tags_in_settings.robot
--rw-r--r--   0        0        0        0 2024-05-24 04:47:50.223513 pytest_robotframework-4.2.0/tests/fixtures/test_robot/test_tags_with_kwargs/__init__.py
--rw-r--r--   0        0        0      722 2024-05-24 04:47:50.223513 pytest_robotframework-4.2.0/tests/fixtures/test_robot/test_tags_with_kwargs/conftest.py
--rw-r--r--   0        0        0       93 2024-05-24 04:47:50.223513 pytest_robotframework-4.2.0/tests/fixtures/test_robot/test_tags_with_kwargs/test_tags_with_kwargs.robot
--rw-r--r--   0        0        0      119 2024-05-24 04:47:50.223513 pytest_robotframework-4.2.0/tests/fixtures/test_robot/test_teardown_fails.robot
--rw-r--r--   0        0        0      115 2024-05-24 04:47:50.223513 pytest_robotframework-4.2.0/tests/fixtures/test_robot/test_teardown_passes.robot
--rw-r--r--   0        0        0      111 2024-05-24 04:47:50.223513 pytest_robotframework-4.2.0/tests/fixtures/test_robot/test_teardown_skipped.robot
--rw-r--r--   0        0        0        0 2024-05-24 04:47:50.223513 pytest_robotframework-4.2.0/tests/fixtures/test_robot/test_traceback/__init__.py
--rw-r--r--   0        0        0       72 2024-05-24 04:47:50.223513 pytest_robotframework-4.2.0/tests/fixtures/test_robot/test_traceback/test.robot
--rw-r--r--   0        0        0       78 2024-05-24 04:47:50.223513 pytest_robotframework-4.2.0/tests/fixtures/test_robot/test_traceback/util.py
--rw-r--r--   0        0        0       36 2024-05-24 04:47:50.223513 pytest_robotframework-4.2.0/tests/fixtures/test_robot/test_two_files_run_one_test/bar.robot
--rw-r--r--   0        0        0       54 2024-05-24 04:47:50.223513 pytest_robotframework-4.2.0/tests/fixtures/test_robot/test_two_files_run_one_test/foo.robot
--rw-r--r--   0        0        0       54 2024-05-24 04:47:50.223513 pytest_robotframework-4.2.0/tests/fixtures/test_robot/test_two_files_run_test_from_second_suite/asdf/foo.robot
--rw-r--r--   0        0        0       36 2024-05-24 04:47:50.223513 pytest_robotframework-4.2.0/tests/fixtures/test_robot/test_two_files_run_test_from_second_suite/fdsa/bar.robot
--rw-r--r--   0        0        0       55 2024-05-24 04:47:50.223513 pytest_robotframework-4.2.0/tests/fixtures/test_robot/test_two_tests_one_fail_one_pass.robot
--rw-r--r--   0        0        0       57 2024-05-24 04:47:50.223513 pytest_robotframework-4.2.0/tests/fixtures/test_robot/test_warning_on_unknown_tag.robot
--rw-r--r--   0        0        0     1035 2024-05-24 04:47:50.223513 pytest_robotframework-4.2.0/tests/test_common.py
--rw-r--r--   0        0        0    34386 2024-05-24 04:47:50.223513 pytest_robotframework-4.2.0/tests/test_python.py
--rw-r--r--   0        0        0    10909 2024-05-24 04:47:50.223513 pytest_robotframework-4.2.0/tests/test_robot.py
--rw-r--r--   0        0        0     1286 2024-05-24 04:47:50.223513 pytest_robotframework-4.2.0/tests/test_robot_utils.py
--rw-r--r--   0        0        0     1776 2024-05-24 04:47:50.223513 pytest_robotframework-4.2.0/tests/type_tests.py
--rw-r--r--   0        0        0    18102 1970-01-01 00:00:00.000000 pytest_robotframework-4.2.0/PKG-INFO
+-rw-r--r--   0        0        0     1067 2024-05-29 08:03:44.727269 pytest_robotframework-4.2.1/LICENSE
+-rw-r--r--   0        0        0    17559 2024-05-29 08:03:44.727269 pytest_robotframework-4.2.1/README.md
+-rw-r--r--   0        0        0     8026 2024-05-29 08:03:58.931345 pytest_robotframework-4.2.1/pyproject.toml
+-rw-r--r--   0        0        0    28462 2024-05-29 08:03:44.727269 pytest_robotframework-4.2.1/pytest_robotframework/__init__.py
+-rw-r--r--   0        0        0        0 2024-05-29 08:03:44.727269 pytest_robotframework-4.2.1/pytest_robotframework/_internal/__init__.py
+-rw-r--r--   0        0        0      559 2024-05-29 08:03:44.727269 pytest_robotframework-4.2.1/pytest_robotframework/_internal/cringe_globals.py
+-rw-r--r--   0        0        0      921 2024-05-29 08:03:44.727269 pytest_robotframework-4.2.1/pytest_robotframework/_internal/errors.py
+-rw-r--r--   0        0        0        0 2024-05-29 08:03:44.727269 pytest_robotframework-4.2.1/pytest_robotframework/_internal/pytest/__init__.py
+-rw-r--r--   0        0        0      230 2024-05-29 08:03:44.727269 pytest_robotframework-4.2.1/pytest_robotframework/_internal/pytest/exception_getter.py
+-rw-r--r--   0        0        0    26514 2024-05-29 08:03:44.727269 pytest_robotframework-4.2.1/pytest_robotframework/_internal/pytest/plugin.py
+-rw-r--r--   0        0        0     7085 2024-05-29 08:03:44.727269 pytest_robotframework-4.2.1/pytest_robotframework/_internal/pytest/robot_file_support.py
+-rw-r--r--   0        0        0     1181 2024-05-29 08:03:44.727269 pytest_robotframework-4.2.1/pytest_robotframework/_internal/pytest/xdist_utils.py
+-rw-r--r--   0        0        0        0 2024-05-29 08:03:44.727269 pytest_robotframework-4.2.1/pytest_robotframework/_internal/robot/__init__.py
+-rw-r--r--   0        0        0     4528 2024-05-29 08:03:44.727269 pytest_robotframework-4.2.1/pytest_robotframework/_internal/robot/library.py
+-rw-r--r--   0        0        0    26358 2024-05-29 08:03:44.727269 pytest_robotframework-4.2.1/pytest_robotframework/_internal/robot/listeners_and_suite_visitors.py
+-rw-r--r--   0        0        0     9785 2024-05-29 08:03:44.727269 pytest_robotframework-4.2.1/pytest_robotframework/_internal/robot/utils.py
+-rw-r--r--   0        0        0     2045 2024-05-29 08:03:44.727269 pytest_robotframework-4.2.1/pytest_robotframework/_internal/utils.py
+-rw-r--r--   0        0        0     3240 2024-05-29 08:03:44.727269 pytest_robotframework-4.2.1/pytest_robotframework/hooks.py
+-rw-r--r--   0        0        0        0 2024-05-29 08:03:44.727269 pytest_robotframework-4.2.1/pytest_robotframework/py.typed
+-rw-r--r--   0        0        0        0 2024-05-29 08:03:44.727269 pytest_robotframework-4.2.1/scripts/__init__.py
+-rw-r--r--   0        0        0      177 2024-05-29 08:03:44.727269 pytest_robotframework-4.2.1/scripts/clear_pycache.py
+-rw-r--r--   0        0        0        0 2024-05-29 08:03:44.727269 pytest_robotframework-4.2.1/tests/__init__.py
+-rw-r--r--   0        0        0    13801 2024-05-29 08:03:44.727269 pytest_robotframework-4.2.1/tests/conftest.py
+-rw-r--r--   0        0        0      230 2024-05-29 08:03:44.727269 pytest_robotframework-4.2.1/tests/fixtures/__init__.py
+-rw-r--r--   0        0        0        0 2024-05-29 08:03:44.727269 pytest_robotframework-4.2.1/tests/fixtures/test_common/test_no_tests_found_no_files/.gitkeep
+-rw-r--r--   0        0        0        0 2024-05-29 08:03:44.727269 pytest_robotframework-4.2.1/tests/fixtures/test_common/test_robot_file_and_python_file/__init__.py
+-rw-r--r--   0        0        0       40 2024-05-29 08:03:44.727269 pytest_robotframework-4.2.1/tests/fixtures/test_common/test_robot_file_and_python_file/foo.robot
+-rw-r--r--   0        0        0       57 2024-05-29 08:03:44.727269 pytest_robotframework-4.2.1/tests/fixtures/test_common/test_robot_file_and_python_file/test_bar.py
+-rw-r--r--   0        0        0        0 2024-05-29 08:03:44.727269 pytest_robotframework-4.2.1/tests/fixtures/test_python/__init__.py
+-rw-r--r--   0        0        0      104 2024-05-29 08:03:44.727269 pytest_robotframework-4.2.1/tests/fixtures/test_python/test_ansi.py
+-rw-r--r--   0        0        0      186 2024-05-29 08:03:44.727269 pytest_robotframework-4.2.1/tests/fixtures/test_python/test_as_keyword_args_and_kwargs.py
+-rw-r--r--   0        0        0      296 2024-05-29 08:03:44.727269 pytest_robotframework-4.2.1/tests/fixtures/test_python/test_as_keyword_context_manager_try_except.py
+-rw-r--r--   0        0        0      105 2024-05-29 08:03:44.731269 pytest_robotframework-4.2.1/tests/fixtures/test_python/test_assertion_fails.py
+-rw-r--r--   0        0        0      105 2024-05-29 08:03:44.731269 pytest_robotframework-4.2.1/tests/fixtures/test_python/test_assertion_fails_with_assertion_hook.py
+-rw-r--r--   0        0        0      195 2024-05-29 08:03:44.731269 pytest_robotframework-4.2.1/tests/fixtures/test_python/test_assertion_fails_with_description.py
+-rw-r--r--   0        0        0      196 2024-05-29 08:03:44.731269 pytest_robotframework-4.2.1/tests/fixtures/test_python/test_assertion_fails_with_fail_message_hide_assert.py
+-rw-r--r--   0        0        0      175 2024-05-29 08:03:44.731269 pytest_robotframework-4.2.1/tests/fixtures/test_python/test_assertion_pass_hook_multiple_tests.py
+-rw-r--r--   0        0        0      105 2024-05-29 08:03:44.731269 pytest_robotframework-4.2.1/tests/fixtures/test_python/test_assertion_passes.py
+-rw-r--r--   0        0        0      435 2024-05-29 08:03:44.731269 pytest_robotframework-4.2.1/tests/fixtures/test_python/test_assertion_passes_custom_messages.py
+-rw-r--r--   0        0        0      253 2024-05-29 08:03:44.731269 pytest_robotframework-4.2.1/tests/fixtures/test_python/test_assertion_passes_hide_assert.py
+-rw-r--r--   0        0        0      359 2024-05-29 08:03:44.731269 pytest_robotframework-4.2.1/tests/fixtures/test_python/test_assertion_passes_hide_asserts_context_manager.py
+-rw-r--r--   0        0        0      292 2024-05-29 08:03:44.731269 pytest_robotframework-4.2.1/tests/fixtures/test_python/test_assertion_passes_show_assert_when_no_assertions_in_robot_log.py
+-rw-r--r--   0        0        0        0 2024-05-29 08:03:44.731269 pytest_robotframework-4.2.1/tests/fixtures/test_python/test_assertion_rewritten_in_conftest_when_assertion_hook_enabled/__init__.py
+-rw-r--r--   0        0        0       80 2024-05-29 08:03:44.731269 pytest_robotframework-4.2.1/tests/fixtures/test_python/test_assertion_rewritten_in_conftest_when_assertion_hook_enabled/conftest.py
+-rw-r--r--   0        0        0       57 2024-05-29 08:03:44.731269 pytest_robotframework-4.2.1/tests/fixtures/test_python/test_assertion_rewritten_in_conftest_when_assertion_hook_enabled/test_foo.py
+-rw-r--r--   0        0        0        0 2024-05-29 08:03:44.731269 pytest_robotframework-4.2.1/tests/fixtures/test_python/test_catch_errors_decorator/__init__.py
+-rw-r--r--   0        0        0      536 2024-05-29 08:03:44.731269 pytest_robotframework-4.2.1/tests/fixtures/test_python/test_catch_errors_decorator/conftest.py
+-rw-r--r--   0        0        0       67 2024-05-29 08:03:44.731269 pytest_robotframework-4.2.1/tests/fixtures/test_python/test_catch_errors_decorator/test_foo.py
+-rw-r--r--   0        0        0        0 2024-05-29 08:03:44.731269 pytest_robotframework-4.2.1/tests/fixtures/test_python/test_catch_errors_decorator_with_non_instance_method/__init__.py
+-rw-r--r--   0        0        0      678 2024-05-29 08:03:44.731269 pytest_robotframework-4.2.1/tests/fixtures/test_python/test_catch_errors_decorator_with_non_instance_method/conftest.py
+-rw-r--r--   0        0        0       67 2024-05-29 08:03:44.731269 pytest_robotframework-4.2.1/tests/fixtures/test_python/test_catch_errors_decorator_with_non_instance_method/test_foo.py
+-rw-r--r--   0        0        0      163 2024-05-29 08:03:44.731269 pytest_robotframework-4.2.1/tests/fixtures/test_python/test_class_has_separate_suite.py
+-rw-r--r--   0        0        0        0 2024-05-29 08:03:44.731269 pytest_robotframework-4.2.1/tests/fixtures/test_python/test_class_separate_files/__init__.py
+-rw-r--r--   0        0        0      121 2024-05-29 08:03:44.731269 pytest_robotframework-4.2.1/tests/fixtures/test_python/test_class_separate_files/test_suite1.py
+-rw-r--r--   0        0        0      121 2024-05-29 08:03:44.731269 pytest_robotframework-4.2.1/tests/fixtures/test_python/test_class_separate_files/test_suite2.py
+-rw-r--r--   0        0        0      228 2024-05-29 08:03:44.731269 pytest_robotframework-4.2.1/tests/fixtures/test_python/test_class_three_tests_one_fail.py
+-rw-r--r--   0        0        0        0 2024-05-29 08:03:44.731269 pytest_robotframework-4.2.1/tests/fixtures/test_python/test_collect_only_nested_suites/asdf/__init__.py
+-rw-r--r--   0        0        0       64 2024-05-29 08:03:44.731269 pytest_robotframework-4.2.1/tests/fixtures/test_python/test_collect_only_nested_suites/asdf/test_bar.py
+-rw-r--r--   0        0        0       64 2024-05-29 08:03:44.731269 pytest_robotframework-4.2.1/tests/fixtures/test_python/test_collect_only_nested_suites/asdf/test_foo.py
+-rw-r--r--   0        0        0        8 2024-05-29 08:03:44.731269 pytest_robotframework-4.2.1/tests/fixtures/test_python/test_config_file_and_cwd_in_different_location/config/tox.ini
+-rw-r--r--   0        0        0        0 2024-05-29 08:03:44.731269 pytest_robotframework-4.2.1/tests/fixtures/test_python/test_config_file_and_cwd_in_different_location/foo/.gitkeep
+-rw-r--r--   0        0        0        0 2024-05-29 08:03:44.731269 pytest_robotframework-4.2.1/tests/fixtures/test_python/test_config_file_and_cwd_in_different_location/tests/__init__.py
+-rw-r--r--   0        0        0       57 2024-05-29 08:03:44.731269 pytest_robotframework-4.2.1/tests/fixtures/test_python/test_config_file_and_cwd_in_different_location/tests/test_foo.py
+-rw-r--r--   0        0        0        0 2024-05-29 08:03:44.731269 pytest_robotframework-4.2.1/tests/fixtures/test_python/test_config_file_in_different_location/__init__.py
+-rw-r--r--   0        0        0        8 2024-05-29 08:03:44.731269 pytest_robotframework-4.2.1/tests/fixtures/test_python/test_config_file_in_different_location/asdf/tox.ini
+-rw-r--r--   0        0        0       57 2024-05-29 08:03:44.731269 pytest_robotframework-4.2.1/tests/fixtures/test_python/test_config_file_in_different_location/test_asdf.py
+-rw-r--r--   0        0        0      254 2024-05-29 08:03:44.731269 pytest_robotframework-4.2.1/tests/fixtures/test_python/test_console_output.py
+-rw-r--r--   0        0        0       66 2024-05-29 08:03:44.731269 pytest_robotframework-4.2.1/tests/fixtures/test_python/test_console_summary.py
+-rw-r--r--   0        0        0        0 2024-05-29 08:03:44.731269 pytest_robotframework-4.2.1/tests/fixtures/test_python/test_correct_items_collected_when_collect_only/__init__.py
+-rw-r--r--   0        0        0       64 2024-05-29 08:03:44.731269 pytest_robotframework-4.2.1/tests/fixtures/test_python/test_correct_items_collected_when_collect_only/test_bar.py
+-rw-r--r--   0        0        0       64 2024-05-29 08:03:44.731269 pytest_robotframework-4.2.1/tests/fixtures/test_python/test_correct_items_collected_when_collect_only/test_foo.py
+-rw-r--r--   0        0        0       87 2024-05-29 08:03:44.731269 pytest_robotframework-4.2.1/tests/fixtures/test_python/test_doesnt_run_when_collecting.py
+-rw-r--r--   0        0        0      130 2024-05-29 08:03:44.731269 pytest_robotframework-4.2.1/tests/fixtures/test_python/test_error_moment.py
+-rw-r--r--   0        0        0      148 2024-05-29 08:03:44.731269 pytest_robotframework-4.2.1/tests/fixtures/test_python/test_error_moment_and_second_test.py
+-rw-r--r--   0        0        0      130 2024-05-29 08:03:44.731269 pytest_robotframework-4.2.1/tests/fixtures/test_python/test_error_moment_exitonerror.py
+-rw-r--r--   0        0        0      171 2024-05-29 08:03:44.731269 pytest_robotframework-4.2.1/tests/fixtures/test_python/test_error_moment_exitonerror_multiple_tests.py
+-rw-r--r--   0        0        0        0 2024-05-29 08:03:44.731269 pytest_robotframework-4.2.1/tests/fixtures/test_python/test_error_moment_setup/__init__.py
+-rw-r--r--   0        0        0      142 2024-05-29 08:03:44.731269 pytest_robotframework-4.2.1/tests/fixtures/test_python/test_error_moment_setup/conftest.py
+-rw-r--r--   0        0        0      106 2024-05-29 08:03:44.731269 pytest_robotframework-4.2.1/tests/fixtures/test_python/test_error_moment_setup/test_foo.py
+-rw-r--r--   0        0        0        0 2024-05-29 08:03:44.731269 pytest_robotframework-4.2.1/tests/fixtures/test_python/test_error_moment_teardown/__init__.py
+-rw-r--r--   0        0        0      145 2024-05-29 08:03:44.731269 pytest_robotframework-4.2.1/tests/fixtures/test_python/test_error_moment_teardown/conftest.py
+-rw-r--r--   0        0        0      106 2024-05-29 08:03:44.731269 pytest_robotframework-4.2.1/tests/fixtures/test_python/test_error_moment_teardown/test_foo.py
+-rw-r--r--   0        0        0      163 2024-05-29 08:03:44.731269 pytest_robotframework-4.2.1/tests/fixtures/test_python/test_fixture.py
+-rw-r--r--   0        0        0      625 2024-05-29 08:03:44.731269 pytest_robotframework-4.2.1/tests/fixtures/test_python/test_fixture_scope.py
+-rw-r--r--   0        0        0      225 2024-05-29 08:03:44.731269 pytest_robotframework-4.2.1/tests/fixtures/test_python/test_full_stack_keyword_context_manager.py
+-rw-r--r--   0        0        0      152 2024-05-29 08:03:44.731269 pytest_robotframework-4.2.1/tests/fixtures/test_python/test_full_stack_keyword_decorator.py
+-rw-r--r--   0        0        0       82 2024-05-29 08:03:44.731269 pytest_robotframework-4.2.1/tests/fixtures/test_python/test_invalid_fixture.py
+-rw-r--r--   0        0        0      243 2024-05-29 08:03:44.731269 pytest_robotframework-4.2.1/tests/fixtures/test_python/test_keyword_and_pytest_raises.py
+-rw-r--r--   0        0        0      218 2024-05-29 08:03:44.731269 pytest_robotframework-4.2.1/tests/fixtures/test_python/test_keyword_decorator_args.py
+-rw-r--r--   0        0        0      554 2024-05-29 08:03:44.731269 pytest_robotframework-4.2.1/tests/fixtures/test_python/test_keyword_decorator_context_manager_that_doesnt_suppress.py
+-rw-r--r--   0        0        0      542 2024-05-29 08:03:44.731269 pytest_robotframework-4.2.1/tests/fixtures/test_python/test_keyword_decorator_context_manager_that_raises_in_body_and_exit.py
+-rw-r--r--   0        0        0      468 2024-05-29 08:03:44.731269 pytest_robotframework-4.2.1/tests/fixtures/test_python/test_keyword_decorator_context_manager_that_raises_in_exit.py
+-rw-r--r--   0        0        0      171 2024-05-29 08:03:44.731269 pytest_robotframework-4.2.1/tests/fixtures/test_python/test_keyword_decorator_custom_name_and_tags.py
+-rw-r--r--   0        0        0      148 2024-05-29 08:03:44.731269 pytest_robotframework-4.2.1/tests/fixtures/test_python/test_keyword_decorator_docstring.py
+-rw-r--r--   0        0        0      178 2024-05-29 08:03:44.731269 pytest_robotframework-4.2.1/tests/fixtures/test_python/test_keyword_decorator_docstring_on_next_line.py
+-rw-r--r--   0        0        0      445 2024-05-29 08:03:44.731269 pytest_robotframework-4.2.1/tests/fixtures/test_python/test_keyword_decorator_returns_context_manager_that_isnt_used.py
+-rw-r--r--   0        0        0      275 2024-05-29 08:03:44.731269 pytest_robotframework-4.2.1/tests/fixtures/test_python/test_keyword_decorator_try_except.py
+-rw-r--r--   0        0        0       85 2024-05-29 08:03:44.731269 pytest_robotframework-4.2.1/tests/fixtures/test_python/test_keyword_names.py
+-rw-r--r--   0        0        0      273 2024-05-29 08:03:44.731269 pytest_robotframework-4.2.1/tests/fixtures/test_python/test_keyword_raises.py
+-rw-r--r--   0        0        0      166 2024-05-29 08:03:44.731269 pytest_robotframework-4.2.1/tests/fixtures/test_python/test_keywordify_context_manager.py
+-rw-r--r--   0        0        0      127 2024-05-29 08:03:44.731269 pytest_robotframework-4.2.1/tests/fixtures/test_python/test_keywordify_function.py
+-rw-r--r--   0        0        0      280 2024-05-29 08:03:44.731269 pytest_robotframework-4.2.1/tests/fixtures/test_python/test_keywordify_keyword_inside_context_manager.py
+-rw-r--r--   0        0        0      545 2024-05-29 08:03:44.731269 pytest_robotframework-4.2.1/tests/fixtures/test_python/test_listener_calls_log_file/Listener.py
+-rw-r--r--   0        0        0        0 2024-05-29 08:03:44.731269 pytest_robotframework-4.2.1/tests/fixtures/test_python/test_listener_calls_log_file/__init__.py
+-rw-r--r--   0        0        0       64 2024-05-29 08:03:44.731269 pytest_robotframework-4.2.1/tests/fixtures/test_python/test_listener_calls_log_file/test_foo.py
+-rw-r--r--   0        0        0        0 2024-05-29 08:03:44.731269 pytest_robotframework-4.2.1/tests/fixtures/test_python/test_listener_not_run_during_collection/__init__.py
+-rw-r--r--   0        0        0      597 2024-05-29 08:03:44.731269 pytest_robotframework-4.2.1/tests/fixtures/test_python/test_listener_not_run_during_collection/conftest.py
+-rw-r--r--   0        0        0      105 2024-05-29 08:03:44.731269 pytest_robotframework-4.2.1/tests/fixtures/test_python/test_listener_not_run_during_collection/test_foo.py
+-rw-r--r--   0        0        0       77 2024-05-29 08:03:44.731269 pytest_robotframework-4.2.1/tests/fixtures/test_python/test_module_docstring.py
+-rw-r--r--   0        0        0       62 2024-05-29 08:03:44.731269 pytest_robotframework-4.2.1/tests/fixtures/test_python/test_multiple_runs.py
+-rw-r--r--   0        0        0      186 2024-05-29 08:03:44.731269 pytest_robotframework-4.2.1/tests/fixtures/test_python/test_nested_class.py
+-rw-r--r--   0        0        0      188 2024-05-29 08:03:44.731269 pytest_robotframework-4.2.1/tests/fixtures/test_python/test_nested_keyword_that_fails.py
+-rw-r--r--   0        0        0      107 2024-05-29 08:03:44.731269 pytest_robotframework-4.2.1/tests/fixtures/test_python/test_nested_suites/suite1/suite2/test_asdf.py
+-rw-r--r--   0        0        0      107 2024-05-29 08:03:44.731269 pytest_robotframework-4.2.1/tests/fixtures/test_python/test_nested_suites/suite1/suite3/test_asdf2.py
+-rw-r--r--   0        0        0      126 2024-05-29 08:03:44.731269 pytest_robotframework-4.2.1/tests/fixtures/test_python/test_nested_suites/test_top_level.py
+-rw-r--r--   0        0        0       63 2024-05-29 08:03:44.731269 pytest_robotframework-4.2.1/tests/fixtures/test_python/test_no_tests_found_when_tests_exist.py
+-rw-r--r--   0        0        0       92 2024-05-29 08:03:44.731269 pytest_robotframework-4.2.1/tests/fixtures/test_python/test_one_test_fails.py
+-rw-r--r--   0        0        0       73 2024-05-29 08:03:44.731269 pytest_robotframework-4.2.1/tests/fixtures/test_python/test_one_test_passes.py
+-rw-r--r--   0        0        0      162 2024-05-29 08:03:44.731269 pytest_robotframework-4.2.1/tests/fixtures/test_python/test_one_test_skipped.py
+-rw-r--r--   0        0        0      100 2024-05-29 08:03:44.731269 pytest_robotframework-4.2.1/tests/fixtures/test_python/test_parameterized_tags.py
+-rw-r--r--   0        0        0      207 2024-05-29 08:03:44.731269 pytest_robotframework-4.2.1/tests/fixtures/test_python/test_parametrize.py
+-rw-r--r--   0        0        0        0 2024-05-29 08:03:44.731269 pytest_robotframework-4.2.1/tests/fixtures/test_python/test_pytest_runtest_protocol_hook_in_different_suite/a/__init__.py
+-rw-r--r--   0        0        0      185 2024-05-29 08:03:44.731269 pytest_robotframework-4.2.1/tests/fixtures/test_python/test_pytest_runtest_protocol_hook_in_different_suite/a/test_c.py
+-rw-r--r--   0        0        0        0 2024-05-29 08:03:44.731269 pytest_robotframework-4.2.1/tests/fixtures/test_python/test_pytest_runtest_protocol_hook_in_different_suite/b/__init__.py
+-rw-r--r--   0        0        0       72 2024-05-29 08:03:44.731269 pytest_robotframework-4.2.1/tests/fixtures/test_python/test_pytest_runtest_protocol_hook_in_different_suite/b/conftest.py
+-rw-r--r--   0        0        0        0 2024-05-29 08:03:44.731269 pytest_robotframework-4.2.1/tests/fixtures/test_python/test_pytest_runtest_protocol_item_hook/foo/__init__.py
+-rw-r--r--   0        0        0      398 2024-05-29 08:03:44.731269 pytest_robotframework-4.2.1/tests/fixtures/test_python/test_pytest_runtest_protocol_item_hook/foo/conftest.py
+-rw-r--r--   0        0        0       67 2024-05-29 08:03:44.731269 pytest_robotframework-4.2.1/tests/fixtures/test_python/test_pytest_runtest_protocol_item_hook/foo/test_foo.py
+-rw-r--r--   0        0        0        0 2024-05-29 08:03:44.731269 pytest_robotframework-4.2.1/tests/fixtures/test_python/test_pytest_runtest_protocol_session_hook/__init__.py
+-rw-r--r--   0        0        0      471 2024-05-29 08:03:44.731269 pytest_robotframework-4.2.1/tests/fixtures/test_python/test_pytest_runtest_protocol_session_hook/conftest.py
+-rw-r--r--   0        0        0       67 2024-05-29 08:03:44.731269 pytest_robotframework-4.2.1/tests/fixtures/test_python/test_pytest_runtest_protocol_session_hook/test_foo.py
+-rw-r--r--   0        0        0      296 2024-05-29 08:03:44.731269 pytest_robotframework-4.2.1/tests/fixtures/test_python/test_python_file_doesnt_get_parsed_as_robot_file.py
+-rw-r--r--   0        0        0       64 2024-05-29 08:03:44.735269 pytest_robotframework-4.2.1/tests/fixtures/test_python/test_robot_args.py
+-rw-r--r--   0        0        0        0 2024-05-29 08:03:44.735269 pytest_robotframework-4.2.1/tests/fixtures/test_python/test_robot_keyword_in_python_test/__init__.py
+-rw-r--r--   0        0        0       34 2024-05-29 08:03:44.735269 pytest_robotframework-4.2.1/tests/fixtures/test_python/test_robot_keyword_in_python_test/bar/bar.resource
+-rw-r--r--   0        0        0      262 2024-05-29 08:03:44.735269 pytest_robotframework-4.2.1/tests/fixtures/test_python/test_robot_keyword_in_python_test/test_foo.py
+-rw-r--r--   0        0        0        0 2024-05-29 08:03:44.735269 pytest_robotframework-4.2.1/tests/fixtures/test_python/test_robot_modify_args_hook/__init__.py
+-rw-r--r--   0        0        0      119 2024-05-29 08:03:44.735269 pytest_robotframework-4.2.1/tests/fixtures/test_python/test_robot_modify_args_hook/conftest.py
+-rw-r--r--   0        0        0      222 2024-05-29 08:03:44.735269 pytest_robotframework-4.2.1/tests/fixtures/test_python/test_robot_modify_args_hook/test_foo.py
+-rw-r--r--   0        0        0        0 2024-05-29 08:03:44.735269 pytest_robotframework-4.2.1/tests/fixtures/test_python/test_robot_modify_args_hook_collect_only/__init__.py
+-rw-r--r--   0        0        0      175 2024-05-29 08:03:44.735269 pytest_robotframework-4.2.1/tests/fixtures/test_python/test_robot_modify_args_hook_collect_only/conftest.py
+-rw-r--r--   0        0        0      221 2024-05-29 08:03:44.735269 pytest_robotframework-4.2.1/tests/fixtures/test_python/test_robot_modify_args_hook_collect_only/test_foo.py
+-rw-r--r--   0        0        0        0 2024-05-29 08:03:44.735269 pytest_robotframework-4.2.1/tests/fixtures/test_python/test_robot_modify_options_hook/__init__.py
+-rw-r--r--   0        0        0      235 2024-05-29 08:03:44.735269 pytest_robotframework-4.2.1/tests/fixtures/test_python/test_robot_modify_options_hook/conftest.py
+-rw-r--r--   0        0        0      222 2024-05-29 08:03:44.735269 pytest_robotframework-4.2.1/tests/fixtures/test_python/test_robot_modify_options_hook/test_foo.py
+-rw-r--r--   0        0        0        0 2024-05-29 08:03:44.735269 pytest_robotframework-4.2.1/tests/fixtures/test_python/test_robot_modify_options_hook_listener_instance/__init__.py
+-rw-r--r--   0        0        0      630 2024-05-29 08:03:44.735269 pytest_robotframework-4.2.1/tests/fixtures/test_python/test_robot_modify_options_hook_listener_instance/conftest.py
+-rw-r--r--   0        0        0       62 2024-05-29 08:03:44.735269 pytest_robotframework-4.2.1/tests/fixtures/test_python/test_robot_modify_options_hook_listener_instance/test_foo.py
+-rw-r--r--   0        0        0      498 2024-05-29 08:03:44.735269 pytest_robotframework-4.2.1/tests/fixtures/test_python/test_robot_options_merge_listeners/Listener.py
+-rw-r--r--   0        0        0        0 2024-05-29 08:03:44.735269 pytest_robotframework-4.2.1/tests/fixtures/test_python/test_robot_options_merge_listeners/__init__.py
+-rw-r--r--   0        0        0      322 2024-05-29 08:03:44.735269 pytest_robotframework-4.2.1/tests/fixtures/test_python/test_robot_options_merge_listeners/test_foo.py
+-rw-r--r--   0        0        0       64 2024-05-29 08:03:44.735269 pytest_robotframework-4.2.1/tests/fixtures/test_python/test_robot_options_variable.py
+-rw-r--r--   0        0        0      498 2024-05-29 08:03:44.735269 pytest_robotframework-4.2.1/tests/fixtures/test_python/test_robot_options_variable_merge_listeners/Listener.py
+-rw-r--r--   0        0        0        0 2024-05-29 08:03:44.735269 pytest_robotframework-4.2.1/tests/fixtures/test_python/test_robot_options_variable_merge_listeners/__init__.py
+-rw-r--r--   0        0        0      322 2024-05-29 08:03:44.735269 pytest_robotframework-4.2.1/tests/fixtures/test_python/test_robot_options_variable_merge_listeners/test_foo.py
+-rw-r--r--   0        0        0        0 2024-05-29 08:03:44.735269 pytest_robotframework-4.2.1/tests/fixtures/test_python/test_run_two_files/__init__.py
+-rw-r--r--   0        0        0       55 2024-05-29 08:03:44.735269 pytest_robotframework-4.2.1/tests/fixtures/test_python/test_run_two_files/test_a.py
+-rw-r--r--   0        0        0       55 2024-05-29 08:03:44.735269 pytest_robotframework-4.2.1/tests/fixtures/test_python/test_run_two_files/test_b.py
+-rw-r--r--   0        0        0      236 2024-05-29 08:03:44.735269 pytest_robotframework-4.2.1/tests/fixtures/test_python/test_set_log_level.py
+-rw-r--r--   0        0        0        0 2024-05-29 08:03:44.735269 pytest_robotframework-4.2.1/tests/fixtures/test_python/test_setup_fails/__init__.py
+-rw-r--r--   0        0        0       90 2024-05-29 08:03:44.735269 pytest_robotframework-4.2.1/tests/fixtures/test_python/test_setup_fails/conftest.py
+-rw-r--r--   0        0        0       73 2024-05-29 08:03:44.735269 pytest_robotframework-4.2.1/tests/fixtures/test_python/test_setup_fails/test_foo.py
+-rw-r--r--   0        0        0        0 2024-05-29 08:03:44.735269 pytest_robotframework-4.2.1/tests/fixtures/test_python/test_setup_passes/__init__.py
+-rw-r--r--   0        0        0      116 2024-05-29 08:03:44.735269 pytest_robotframework-4.2.1/tests/fixtures/test_python/test_setup_passes/conftest.py
+-rw-r--r--   0        0        0      116 2024-05-29 08:03:44.735269 pytest_robotframework-4.2.1/tests/fixtures/test_python/test_setup_passes/test_foo.py
+-rw-r--r--   0        0        0        0 2024-05-29 08:03:44.735269 pytest_robotframework-4.2.1/tests/fixtures/test_python/test_setup_skipped/__init__.py
+-rw-r--r--   0        0        0      101 2024-05-29 08:03:44.735269 pytest_robotframework-4.2.1/tests/fixtures/test_python/test_setup_skipped/conftest.py
+-rw-r--r--   0        0        0       73 2024-05-29 08:03:44.735269 pytest_robotframework-4.2.1/tests/fixtures/test_python/test_setup_skipped/test_foo.py
+-rw-r--r--   0        0        0      305 2024-05-29 08:03:44.735269 pytest_robotframework-4.2.1/tests/fixtures/test_python/test_suite_variables.py
+-rw-r--r--   0        0        0      313 2024-05-29 08:03:44.735269 pytest_robotframework-4.2.1/tests/fixtures/test_python/test_suite_variables_with_slash.py
+-rw-r--r--   0        0        0      107 2024-05-29 08:03:44.735269 pytest_robotframework-4.2.1/tests/fixtures/test_python/test_suites/suite1/test_asdf.py
+-rw-r--r--   0        0        0       94 2024-05-29 08:03:44.735269 pytest_robotframework-4.2.1/tests/fixtures/test_python/test_tags.py
+-rw-r--r--   0        0        0        0 2024-05-29 08:03:44.735269 pytest_robotframework-4.2.1/tests/fixtures/test_python/test_teardown_fails/__init__.py
+-rw-r--r--   0        0        0       93 2024-05-29 08:03:44.735269 pytest_robotframework-4.2.1/tests/fixtures/test_python/test_teardown_fails/conftest.py
+-rw-r--r--   0        0        0       73 2024-05-29 08:03:44.735269 pytest_robotframework-4.2.1/tests/fixtures/test_python/test_teardown_fails/test_foo.py
+-rw-r--r--   0        0        0        0 2024-05-29 08:03:44.735269 pytest_robotframework-4.2.1/tests/fixtures/test_python/test_teardown_passes/__init__.py
+-rw-r--r--   0        0        0      119 2024-05-29 08:03:44.735269 pytest_robotframework-4.2.1/tests/fixtures/test_python/test_teardown_passes/conftest.py
+-rw-r--r--   0        0        0      115 2024-05-29 08:03:44.735269 pytest_robotframework-4.2.1/tests/fixtures/test_python/test_teardown_passes/test_foo.py
+-rw-r--r--   0        0        0        0 2024-05-29 08:03:44.735269 pytest_robotframework-4.2.1/tests/fixtures/test_python/test_teardown_skipped/__init__.py
+-rw-r--r--   0        0        0      104 2024-05-29 08:03:44.735269 pytest_robotframework-4.2.1/tests/fixtures/test_python/test_teardown_skipped/conftest.py
+-rw-r--r--   0        0        0       73 2024-05-29 08:03:44.735269 pytest_robotframework-4.2.1/tests/fixtures/test_python/test_teardown_skipped/test_foo.py
+-rw-r--r--   0        0        0       78 2024-05-29 08:03:44.735269 pytest_robotframework-4.2.1/tests/fixtures/test_python/test_test_case_docstring.py
+-rw-r--r--   0        0        0       80 2024-05-29 08:03:44.735269 pytest_robotframework-4.2.1/tests/fixtures/test_python/test_trace_ricing.py
+-rw-r--r--   0        0        0      106 2024-05-29 08:03:44.735269 pytest_robotframework-4.2.1/tests/fixtures/test_python/test_traceback.py
+-rw-r--r--   0        0        0      108 2024-05-29 08:03:44.735269 pytest_robotframework-4.2.1/tests/fixtures/test_python/test_two_tests_one_fail_one_pass.py
+-rw-r--r--   0        0        0       77 2024-05-29 08:03:44.735269 pytest_robotframework-4.2.1/tests/fixtures/test_python/test_two_tests_specified_by_full_path.py
+-rw-r--r--   0        0        0        0 2024-05-29 08:03:44.735269 pytest_robotframework-4.2.1/tests/fixtures/test_python/test_two_tests_specified_by_full_path_in_different_files/__init__.py
+-rw-r--r--   0        0        0       62 2024-05-29 08:03:44.735269 pytest_robotframework-4.2.1/tests/fixtures/test_python/test_two_tests_specified_by_full_path_in_different_files/test_bar.py
+-rw-r--r--   0        0        0       62 2024-05-29 08:03:44.735269 pytest_robotframework-4.2.1/tests/fixtures/test_python/test_two_tests_specified_by_full_path_in_different_files/test_foo.py
+-rw-r--r--   0        0        0        0 2024-05-29 08:03:44.735269 pytest_robotframework-4.2.1/tests/fixtures/test_python/test_two_tests_two_files_one_fail_one_pass/__init__.py
+-rw-r--r--   0        0        0       64 2024-05-29 08:03:44.735269 pytest_robotframework-4.2.1/tests/fixtures/test_python/test_two_tests_two_files_one_fail_one_pass/test_one.py
+-rw-r--r--   0        0        0       83 2024-05-29 08:03:44.735269 pytest_robotframework-4.2.1/tests/fixtures/test_python/test_two_tests_two_files_one_fail_one_pass/test_two.py
+-rw-r--r--   0        0        0        0 2024-05-29 08:03:44.735269 pytest_robotframework-4.2.1/tests/fixtures/test_python/test_two_tests_with_same_name_one_fail_one_pass/__init__.py
+-rw-r--r--   0        0        0       63 2024-05-29 08:03:44.735269 pytest_robotframework-4.2.1/tests/fixtures/test_python/test_two_tests_with_same_name_one_fail_one_pass/test_one.py
+-rw-r--r--   0        0        0       82 2024-05-29 08:03:44.735269 pytest_robotframework-4.2.1/tests/fixtures/test_python/test_two_tests_with_same_name_one_fail_one_pass/test_two.py
+-rw-r--r--   0        0        0      121 2024-05-29 08:03:44.735269 pytest_robotframework-4.2.1/tests/fixtures/test_python/test_unittest_class.py
+-rw-r--r--   0        0        0      311 2024-05-29 08:03:44.735269 pytest_robotframework-4.2.1/tests/fixtures/test_python/test_variables_list.py
+-rw-r--r--   0        0        0        0 2024-05-29 08:03:44.735269 pytest_robotframework-4.2.1/tests/fixtures/test_python/test_variables_not_in_scope_in_other_suites/__init__.py
+-rw-r--r--   0        0        0      303 2024-05-29 08:03:44.735269 pytest_robotframework-4.2.1/tests/fixtures/test_python/test_variables_not_in_scope_in_other_suites/test_one.py
+-rw-r--r--   0        0        0      222 2024-05-29 08:03:44.735269 pytest_robotframework-4.2.1/tests/fixtures/test_python/test_variables_not_in_scope_in_other_suites/test_two.py
+-rw-r--r--   0        0        0       57 2024-05-29 08:03:44.735269 pytest_robotframework-4.2.1/tests/fixtures/test_python/test_xdist_n_0.py
+-rw-r--r--   0        0        0        0 2024-05-29 08:03:44.735269 pytest_robotframework-4.2.1/tests/fixtures/test_python/test_xfail_fails/__init__.py
+-rw-r--r--   0        0        0      133 2024-05-29 08:03:44.735269 pytest_robotframework-4.2.1/tests/fixtures/test_python/test_xfail_fails/test_foo.py
+-rw-r--r--   0        0        0       28 2024-05-29 08:03:44.735269 pytest_robotframework-4.2.1/tests/fixtures/test_python/test_xfail_fails/tox.ini
+-rw-r--r--   0        0        0        0 2024-05-29 08:03:44.735269 pytest_robotframework-4.2.1/tests/fixtures/test_python/test_xfail_fails_no_reason/__init__.py
+-rw-r--r--   0        0        0      118 2024-05-29 08:03:44.735269 pytest_robotframework-4.2.1/tests/fixtures/test_python/test_xfail_fails_no_reason/test_foo.py
+-rw-r--r--   0        0        0       28 2024-05-29 08:03:44.735269 pytest_robotframework-4.2.1/tests/fixtures/test_python/test_xfail_fails_no_reason/tox.ini
+-rw-r--r--   0        0        0        0 2024-05-29 08:03:44.735269 pytest_robotframework-4.2.1/tests/fixtures/test_python/test_xfail_passes/__init__.py
+-rw-r--r--   0        0        0      123 2024-05-29 08:03:44.735269 pytest_robotframework-4.2.1/tests/fixtures/test_python/test_xfail_passes/test_foo.py
+-rw-r--r--   0        0        0       28 2024-05-29 08:03:44.735269 pytest_robotframework-4.2.1/tests/fixtures/test_python/test_xfail_passes/tox.ini
+-rw-r--r--   0        0        0        0 2024-05-29 08:03:44.735269 pytest_robotframework-4.2.1/tests/fixtures/test_python/test_xfail_passes_no_reason/__init__.py
+-rw-r--r--   0        0        0      107 2024-05-29 08:03:44.735269 pytest_robotframework-4.2.1/tests/fixtures/test_python/test_xfail_passes_no_reason/test_foo.py
+-rw-r--r--   0        0        0       28 2024-05-29 08:03:44.735269 pytest_robotframework-4.2.1/tests/fixtures/test_python/test_xfail_passes_no_reason/tox.ini
+-rw-r--r--   0        0        0       32 2024-05-29 08:03:44.735269 pytest_robotframework-4.2.1/tests/fixtures/test_robot/test_collect_only_nested_suites/bar.robot
+-rw-r--r--   0        0        0       32 2024-05-29 08:03:44.735269 pytest_robotframework-4.2.1/tests/fixtures/test_robot/test_collect_only_nested_suites/foo.robot
+-rw-r--r--   0        0        0       32 2024-05-29 08:03:44.735269 pytest_robotframework-4.2.1/tests/fixtures/test_robot/test_correct_items_collected_when_collect_only/bar.robot
+-rw-r--r--   0        0        0       32 2024-05-29 08:03:44.735269 pytest_robotframework-4.2.1/tests/fixtures/test_robot/test_correct_items_collected_when_collect_only/foo.robot
+-rw-r--r--   0        0        0       36 2024-05-29 08:03:44.735269 pytest_robotframework-4.2.1/tests/fixtures/test_robot/test_doesnt_run_tests_outside_path/bar/asdf.robot
+-rw-r--r--   0        0        0       36 2024-05-29 08:03:44.735269 pytest_robotframework-4.2.1/tests/fixtures/test_robot/test_doesnt_run_tests_outside_path/foo/asdf.robot
+-rw-r--r--   0        0        0       44 2024-05-29 08:03:44.735269 pytest_robotframework-4.2.1/tests/fixtures/test_robot/test_doesnt_run_when_collecting.robot
+-rw-r--r--   0        0        0      283 2024-05-29 08:03:44.735269 pytest_robotframework-4.2.1/tests/fixtures/test_robot/test_empty_setup_or_teardown.robot
+-rw-r--r--   0        0        0       99 2024-05-29 08:03:44.735269 pytest_robotframework-4.2.1/tests/fixtures/test_robot/test_fails_when_import_error_and_exit_on_error.robot
+-rw-r--r--   0        0        0        0 2024-05-29 08:03:44.735269 pytest_robotframework-4.2.1/tests/fixtures/test_robot/test_init_file/__init__.py
+-rw-r--r--   0        0        0       40 2024-05-29 08:03:44.735269 pytest_robotframework-4.2.1/tests/fixtures/test_robot/test_init_file/foo.robot
+-rw-r--r--   0        0        0        0 2024-05-29 08:03:44.735269 pytest_robotframework-4.2.1/tests/fixtures/test_robot/test_init_file_nested/__init__.py
+-rw-r--r--   0        0        0        0 2024-05-29 08:03:44.735269 pytest_robotframework-4.2.1/tests/fixtures/test_robot/test_init_file_nested/foo/__init__.py
+-rw-r--r--   0        0        0       40 2024-05-29 08:03:44.735269 pytest_robotframework-4.2.1/tests/fixtures/test_robot/test_init_file_nested/foo/bar.robot
+-rw-r--r--   0        0        0       40 2024-05-29 08:03:44.735269 pytest_robotframework-4.2.1/tests/fixtures/test_robot/test_init_file_nested/foo/foo.robot
+-rw-r--r--   0        0        0        0 2024-05-29 08:03:44.735269 pytest_robotframework-4.2.1/tests/fixtures/test_robot/test_keyword_decorator/__init__.py
+-rw-r--r--   0        0        0       71 2024-05-29 08:03:44.735269 pytest_robotframework-4.2.1/tests/fixtures/test_robot/test_keyword_decorator/bar.robot
+-rw-r--r--   0        0        0      151 2024-05-29 08:03:44.735269 pytest_robotframework-4.2.1/tests/fixtures/test_robot/test_keyword_decorator/foo.py
+-rw-r--r--   0        0        0        0 2024-05-29 08:03:44.735269 pytest_robotframework-4.2.1/tests/fixtures/test_robot/test_keyword_decorator_and_other_decorator/__init__.py
+-rw-r--r--   0        0        0       71 2024-05-29 08:03:44.739269 pytest_robotframework-4.2.1/tests/fixtures/test_robot/test_keyword_decorator_and_other_decorator/bar.robot
+-rw-r--r--   0        0        0      468 2024-05-29 08:03:44.739269 pytest_robotframework-4.2.1/tests/fixtures/test_robot/test_keyword_decorator_and_other_decorator/foo.py
+-rw-r--r--   0        0        0      162 2024-05-29 08:03:44.739269 pytest_robotframework-4.2.1/tests/fixtures/test_robot/test_keyword_with_conflicting_name.robot
+-rw-r--r--   0        0        0       62 2024-05-29 08:03:44.739269 pytest_robotframework-4.2.1/tests/fixtures/test_robot/test_line_number.robot
+-rw-r--r--   0        0        0      535 2024-05-29 08:03:44.739269 pytest_robotframework-4.2.1/tests/fixtures/test_robot/test_listener_calls_log_file/Listener.py
+-rw-r--r--   0        0        0        0 2024-05-29 08:03:44.739269 pytest_robotframework-4.2.1/tests/fixtures/test_robot/test_listener_calls_log_file/__init__.py
+-rw-r--r--   0        0        0       40 2024-05-29 08:03:44.739269 pytest_robotframework-4.2.1/tests/fixtures/test_robot/test_listener_calls_log_file/foo.robot
+-rw-r--r--   0        0        0        0 2024-05-29 08:03:44.739269 pytest_robotframework-4.2.1/tests/fixtures/test_robot/test_nested_keyword_that_fails/__init__.py
+-rw-r--r--   0        0        0       71 2024-05-29 08:03:44.739269 pytest_robotframework-4.2.1/tests/fixtures/test_robot/test_nested_keyword_that_fails/bar.robot
+-rw-r--r--   0        0        0      160 2024-05-29 08:03:44.739269 pytest_robotframework-4.2.1/tests/fixtures/test_robot/test_nested_keyword_that_fails/foo.py
+-rw-r--r--   0        0        0       40 2024-05-29 08:03:44.739269 pytest_robotframework-4.2.1/tests/fixtures/test_robot/test_no_tests_found_when_tests_exist.robot
+-rw-r--r--   0        0        0       32 2024-05-29 08:03:44.739269 pytest_robotframework-4.2.1/tests/fixtures/test_robot/test_one_test_fails.robot
+-rw-r--r--   0        0        0       36 2024-05-29 08:03:44.739269 pytest_robotframework-4.2.1/tests/fixtures/test_robot/test_one_test_passes.robot
+-rw-r--r--   0        0        0       32 2024-05-29 08:03:44.739269 pytest_robotframework-4.2.1/tests/fixtures/test_robot/test_one_test_skipped.robot
+-rw-r--r--   0        0        0       61 2024-05-29 08:03:44.739269 pytest_robotframework-4.2.1/tests/fixtures/test_robot/test_parameterized_tags/foo.robot
+-rw-r--r--   0        0        0       34 2024-05-29 08:03:44.739269 pytest_robotframework-4.2.1/tests/fixtures/test_robot/test_parameterized_tags/tox.ini
+-rw-r--r--   0        0        0       95 2024-05-29 08:03:44.739269 pytest_robotframework-4.2.1/tests/fixtures/test_robot/test_run_keyword_and_ignore_error.robot
+-rw-r--r--   0        0        0       38 2024-05-29 08:03:44.739269 pytest_robotframework-4.2.1/tests/fixtures/test_robot/test_run_two_files/a.robot
+-rw-r--r--   0        0        0       38 2024-05-29 08:03:44.739269 pytest_robotframework-4.2.1/tests/fixtures/test_robot/test_run_two_files/b.robot
+-rw-r--r--   0        0        0      115 2024-05-29 08:03:44.739269 pytest_robotframework-4.2.1/tests/fixtures/test_robot/test_setup_fails.robot
+-rw-r--r--   0        0        0      111 2024-05-29 08:03:44.739269 pytest_robotframework-4.2.1/tests/fixtures/test_robot/test_setup_passes.robot
+-rw-r--r--   0        0        0      107 2024-05-29 08:03:44.739269 pytest_robotframework-4.2.1/tests/fixtures/test_robot/test_setup_skipped.robot
+-rw-r--r--   0        0        0      163 2024-05-29 08:03:44.739269 pytest_robotframework-4.2.1/tests/fixtures/test_robot/test_setup_with_args.robot
+-rw-r--r--   0        0        0       96 2024-05-29 08:03:44.739269 pytest_robotframework-4.2.1/tests/fixtures/test_robot/test_tags.robot
+-rw-r--r--   0        0        0      100 2024-05-29 08:03:44.739269 pytest_robotframework-4.2.1/tests/fixtures/test_robot/test_tags_in_settings.robot
+-rw-r--r--   0        0        0        0 2024-05-29 08:03:44.739269 pytest_robotframework-4.2.1/tests/fixtures/test_robot/test_tags_with_kwargs/__init__.py
+-rw-r--r--   0        0        0      722 2024-05-29 08:03:44.739269 pytest_robotframework-4.2.1/tests/fixtures/test_robot/test_tags_with_kwargs/conftest.py
+-rw-r--r--   0        0        0       93 2024-05-29 08:03:44.739269 pytest_robotframework-4.2.1/tests/fixtures/test_robot/test_tags_with_kwargs/test_tags_with_kwargs.robot
+-rw-r--r--   0        0        0      119 2024-05-29 08:03:44.739269 pytest_robotframework-4.2.1/tests/fixtures/test_robot/test_teardown_fails.robot
+-rw-r--r--   0        0        0      115 2024-05-29 08:03:44.739269 pytest_robotframework-4.2.1/tests/fixtures/test_robot/test_teardown_passes.robot
+-rw-r--r--   0        0        0      111 2024-05-29 08:03:44.739269 pytest_robotframework-4.2.1/tests/fixtures/test_robot/test_teardown_skipped.robot
+-rw-r--r--   0        0        0        0 2024-05-29 08:03:44.739269 pytest_robotframework-4.2.1/tests/fixtures/test_robot/test_traceback/__init__.py
+-rw-r--r--   0        0        0       72 2024-05-29 08:03:44.739269 pytest_robotframework-4.2.1/tests/fixtures/test_robot/test_traceback/test.robot
+-rw-r--r--   0        0        0       78 2024-05-29 08:03:44.739269 pytest_robotframework-4.2.1/tests/fixtures/test_robot/test_traceback/util.py
+-rw-r--r--   0        0        0       36 2024-05-29 08:03:44.739269 pytest_robotframework-4.2.1/tests/fixtures/test_robot/test_two_files_run_one_test/bar.robot
+-rw-r--r--   0        0        0       54 2024-05-29 08:03:44.739269 pytest_robotframework-4.2.1/tests/fixtures/test_robot/test_two_files_run_one_test/foo.robot
+-rw-r--r--   0        0        0       54 2024-05-29 08:03:44.739269 pytest_robotframework-4.2.1/tests/fixtures/test_robot/test_two_files_run_test_from_second_suite/asdf/foo.robot
+-rw-r--r--   0        0        0       36 2024-05-29 08:03:44.739269 pytest_robotframework-4.2.1/tests/fixtures/test_robot/test_two_files_run_test_from_second_suite/fdsa/bar.robot
+-rw-r--r--   0        0        0       55 2024-05-29 08:03:44.739269 pytest_robotframework-4.2.1/tests/fixtures/test_robot/test_two_tests_one_fail_one_pass.robot
+-rw-r--r--   0        0        0       57 2024-05-29 08:03:44.739269 pytest_robotframework-4.2.1/tests/fixtures/test_robot/test_warning_on_unknown_tag.robot
+-rw-r--r--   0        0        0     1035 2024-05-29 08:03:44.739269 pytest_robotframework-4.2.1/tests/test_common.py
+-rw-r--r--   0        0        0    34551 2024-05-29 08:03:44.739269 pytest_robotframework-4.2.1/tests/test_python.py
+-rw-r--r--   0        0        0    11600 2024-05-29 08:03:44.739269 pytest_robotframework-4.2.1/tests/test_robot.py
+-rw-r--r--   0        0        0     1286 2024-05-29 08:03:44.739269 pytest_robotframework-4.2.1/tests/test_robot_utils.py
+-rw-r--r--   0        0        0     1776 2024-05-29 08:03:44.739269 pytest_robotframework-4.2.1/tests/type_tests.py
+-rw-r--r--   0        0        0    18102 1970-01-01 00:00:00.000000 pytest_robotframework-4.2.1/PKG-INFO
```

### Comparing `pytest_robotframework-4.2.0/LICENSE` & `pytest_robotframework-4.2.1/LICENSE`

 * *Files identical despite different names*

### Comparing `pytest_robotframework-4.2.0/README.md` & `pytest_robotframework-4.2.1/README.md`

 * *Files identical despite different names*

### Comparing `pytest_robotframework-4.2.0/pyproject.toml` & `pytest_robotframework-4.2.1/pyproject.toml`

 * *Files 1% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 [project]
 name = "pytest_robotframework"
-version = "4.2.0"
+version = "4.2.1"
 description = "a pytest plugin that can run both python and robotframework tests while generating robot reports for them"
 authors = [
     { name = "DetachHead", email = "detachhead@users.noreply.github.com" },
 ]
 dependencies = [
     "pytest<9,>=7",
     "robotframework<8.0.0,>=6.1",
```

### Comparing `pytest_robotframework-4.2.0/pytest_robotframework/__init__.py` & `pytest_robotframework-4.2.1/pytest_robotframework/__init__.py`

 * *Files identical despite different names*

### Comparing `pytest_robotframework-4.2.0/pytest_robotframework/_internal/cringe_globals.py` & `pytest_robotframework-4.2.1/pytest_robotframework/_internal/cringe_globals.py`

 * *Files identical despite different names*

### Comparing `pytest_robotframework-4.2.0/pytest_robotframework/_internal/errors.py` & `pytest_robotframework-4.2.1/pytest_robotframework/_internal/errors.py`

 * *Files identical despite different names*

### Comparing `pytest_robotframework-4.2.0/pytest_robotframework/_internal/pytest/plugin.py` & `pytest_robotframework-4.2.1/pytest_robotframework/_internal/pytest/plugin.py`

 * *Files 2% similar despite different names*

```diff
@@ -222,15 +222,15 @@
     return frozenset(result)
 
 
 _robot_args_key = StashKey[RobotOptions]()
 
 
 def _get_robot_args(session: Session) -> RobotOptions:
-    result: RobotOptions | None = session.stash.get(_robot_args_key, None)
+    result: RobotOptions | None = session.config.stash.get(_robot_args_key, None)
     if result is not None:
         return result
     options: dict[str, object] = {}
 
     # set any robot options that were set in the pytest cli args:
     for arg_name, default_value in cli_defaults(RobotSettings).items():
         if arg_name in banned_options:
@@ -258,15 +258,15 @@
                 _get_pytest_collection_paths(session)
             )[0],
         ),
     )
     # https://github.com/DetachHead/basedpyright#note-about-casting-with-typeddicts
     result = cast(RobotOptions, options)  # pyright:ignore[reportInvalidCast]
     session.config.hook.pytest_robot_modify_options(options=result, session=session)
-    session.stash[_robot_args_key] = result
+    session.config.stash[_robot_args_key] = result
     return result
 
 
 def _run_robot(session: Session, robot_options: InternalRobotOptions):
     """runs robot with the specified `robot_options`"""
     robot_options = merge_robot_options(
         # user-specified options:
@@ -648,15 +648,18 @@
         _robot_run_tests(item.session, xdist_item=item)
         return True
     return None
 
 
 @hookimpl(tryfirst=True)
 def pytest_terminal_summary(terminalreporter: TerminalReporter, config: Config):
-    log_file = config.rootpath / cast(str, config.option.robot_log)  # pyright: ignore[reportAny]
+    args = config.stash.get(_robot_args_key, None)
+    if not args or not args["log"]:
+        return
+    log_file = Path(args["outputdir"], args["log"]).absolute()
     terminalreporter.line("")
     terminalreporter.line("Robot Framework Output Files:", bold=True)
     terminalreporter.line(f"Log:     {log_file}")
     terminalreporter.line(f"Log URI: {log_file.as_uri()}")
 
 
 @patch_method(ErrorDetails)
```

### Comparing `pytest_robotframework-4.2.0/pytest_robotframework/_internal/pytest/robot_file_support.py` & `pytest_robotframework-4.2.1/pytest_robotframework/_internal/pytest/robot_file_support.py`

 * *Files 2% similar despite different names*

```diff
@@ -112,15 +112,15 @@
             yield
         except ExecutionFailed as e:
             if e.status == "SKIP":
                 skip(e.message)
             raise
 
     def _run_keyword(self, keyword: model.Keyword | None):
-        if keyword:
+        if keyword and keyword.name is not None and keyword.name.lower() != "none":
             with self._check_skipped():
                 BuiltIn().run_keyword(  # pyright:ignore[reportUnknownMemberType]
                     keyword.name, *keyword.args
                 )
 
     @override
     def setup(self):
```

### Comparing `pytest_robotframework-4.2.0/pytest_robotframework/_internal/pytest/xdist_utils.py` & `pytest_robotframework-4.2.1/pytest_robotframework/_internal/pytest/xdist_utils.py`

 * *Files identical despite different names*

### Comparing `pytest_robotframework-4.2.0/pytest_robotframework/_internal/robot/library.py` & `pytest_robotframework-4.2.1/pytest_robotframework/_internal/robot/library.py`

 * *Files identical despite different names*

### Comparing `pytest_robotframework-4.2.0/pytest_robotframework/_internal/robot/listeners_and_suite_visitors.py` & `pytest_robotframework-4.2.1/pytest_robotframework/_internal/robot/listeners_and_suite_visitors.py`

 * *Files identical despite different names*

### Comparing `pytest_robotframework-4.2.0/pytest_robotframework/_internal/robot/utils.py` & `pytest_robotframework-4.2.1/pytest_robotframework/_internal/robot/utils.py`

 * *Files identical despite different names*

### Comparing `pytest_robotframework-4.2.0/pytest_robotframework/_internal/utils.py` & `pytest_robotframework-4.2.1/pytest_robotframework/_internal/utils.py`

 * *Files identical despite different names*

### Comparing `pytest_robotframework-4.2.0/pytest_robotframework/hooks.py` & `pytest_robotframework-4.2.1/pytest_robotframework/hooks.py`

 * *Files identical despite different names*

### Comparing `pytest_robotframework-4.2.0/tests/conftest.py` & `pytest_robotframework-4.2.1/tests/conftest.py`

 * *Files identical despite different names*

### Comparing `pytest_robotframework-4.2.0/tests/fixtures/test_python/test_catch_errors_decorator/conftest.py` & `pytest_robotframework-4.2.1/tests/fixtures/test_python/test_catch_errors_decorator/conftest.py`

 * *Files identical despite different names*

### Comparing `pytest_robotframework-4.2.0/tests/fixtures/test_python/test_catch_errors_decorator_with_non_instance_method/conftest.py` & `pytest_robotframework-4.2.1/tests/fixtures/test_python/test_catch_errors_decorator_with_non_instance_method/conftest.py`

 * *Files identical despite different names*

### Comparing `pytest_robotframework-4.2.0/tests/fixtures/test_python/test_fixture_scope.py` & `pytest_robotframework-4.2.1/tests/fixtures/test_python/test_fixture_scope.py`

 * *Files identical despite different names*

### Comparing `pytest_robotframework-4.2.0/tests/fixtures/test_python/test_keyword_decorator_context_manager_that_doesnt_suppress.py` & `pytest_robotframework-4.2.1/tests/fixtures/test_python/test_keyword_decorator_context_manager_that_doesnt_suppress.py`

 * *Files identical despite different names*

### Comparing `pytest_robotframework-4.2.0/tests/fixtures/test_python/test_keyword_decorator_context_manager_that_raises_in_body_and_exit.py` & `pytest_robotframework-4.2.1/tests/fixtures/test_python/test_keyword_decorator_context_manager_that_raises_in_body_and_exit.py`

 * *Files identical despite different names*

### Comparing `pytest_robotframework-4.2.0/tests/fixtures/test_python/test_listener_calls_log_file/Listener.py` & `pytest_robotframework-4.2.1/tests/fixtures/test_python/test_listener_calls_log_file/Listener.py`

 * *Files identical despite different names*

### Comparing `pytest_robotframework-4.2.0/tests/fixtures/test_python/test_listener_not_run_during_collection/conftest.py` & `pytest_robotframework-4.2.1/tests/fixtures/test_python/test_listener_not_run_during_collection/conftest.py`

 * *Files identical despite different names*

### Comparing `pytest_robotframework-4.2.0/tests/fixtures/test_python/test_robot_modify_options_hook_listener_instance/conftest.py` & `pytest_robotframework-4.2.1/tests/fixtures/test_python/test_robot_modify_options_hook_listener_instance/conftest.py`

 * *Files identical despite different names*

### Comparing `pytest_robotframework-4.2.0/tests/fixtures/test_robot/test_listener_calls_log_file/Listener.py` & `pytest_robotframework-4.2.1/tests/fixtures/test_robot/test_listener_calls_log_file/Listener.py`

 * *Files identical despite different names*

### Comparing `pytest_robotframework-4.2.0/tests/fixtures/test_robot/test_tags_with_kwargs/conftest.py` & `pytest_robotframework-4.2.1/tests/fixtures/test_robot/test_tags_with_kwargs/conftest.py`

 * *Files identical despite different names*

### Comparing `pytest_robotframework-4.2.0/tests/test_common.py` & `pytest_robotframework-4.2.1/tests/test_common.py`

 * *Files identical despite different names*

### Comparing `pytest_robotframework-4.2.0/tests/test_python.py` & `pytest_robotframework-4.2.1/tests/test_python.py`

 * *Files 1% similar despite different names*

```diff
@@ -892,25 +892,27 @@
 def test_class_three_tests_one_fail(pr: PytestRobotTester):
     """this test is for an xdist issue. needs to have one more tests than there are workers"""
     pr.run_and_assert_result(passed=2, failed=1)
     pr.assert_log_file_exists()
 
 
 def test_console_summary(pr: PytestRobotTester):
-    result = pr.run_pytest(subprocess=True)
-    path = pr.pytester.path / "log.html"
+    result = pr.run_pytest("--robot-outputdir=a", "--robot-log=b", subprocess=True)
+    path = pr.pytester.path / "a" / "b"
     assert re.search(
         rf"""
 
 Robot Framework Output Files:
 Log:     {re.escape(str(path))}
 Log URI: {re.escape(path.as_uri())}
 """,
         "\n".join(result.outlines),
     )
+    result = pr.run_pytest("--robot-log=", subprocess=True)
+    assert "Robot Framework Output Files:" not in result.outlines
 
 
 def test_console_output(pr: PytestRobotTester):
     if pr.xdist:
         result = pr.run_pytest("--capture=no")
         assert "Output:" not in "\n".join(result.outlines)
     else:
```

### Comparing `pytest_robotframework-4.2.0/tests/test_robot.py` & `pytest_robotframework-4.2.1/tests/test_robot.py`

 * *Files 4% similar despite different names*

```diff
@@ -302,7 +302,25 @@
 def test_traceback(pr: PytestRobotTester):
     result = pr.run_pytest("--tb=short")
     assert """
 util.py:5: in thing
     raise Exception("asdf")
 E   Exception: asdf
 """ in "\n".join(result.outlines)
+
+
+def test_empty_setup_or_teardown(pr: PytestRobotTester):
+    pr.run_and_assert_result(passed=3)
+    pr.assert_log_file_exists()
+    xml = output_xml()
+    assert xpath(
+        xml,
+        "//test[@name='Runs globally defined setup and teardown']/kw[@name='Setup']/kw[@name='Log']"
+        + "/msg[.='setup ran']",
+    )
+    assert xpath(
+        xml,
+        "//test[@name='Runs globally defined setup and teardown']/kw[@name='Teardown']"
+        + "/kw[@name='Log']/msg[.='teardown ran']",
+    )
+    assert not xml.xpath("//test[@name='Disable setup']/kw[@name='Setup']/kw[@name='Log']")
+    assert not xml.xpath("//test[@name='Disable teardown']/kw[@name='Teardown']/kw[@name='Log']")
```

### Comparing `pytest_robotframework-4.2.0/tests/test_robot_utils.py` & `pytest_robotframework-4.2.1/tests/test_robot_utils.py`

 * *Files identical despite different names*

### Comparing `pytest_robotframework-4.2.0/tests/type_tests.py` & `pytest_robotframework-4.2.1/tests/type_tests.py`

 * *Files identical despite different names*

### Comparing `pytest_robotframework-4.2.0/PKG-INFO` & `pytest_robotframework-4.2.1/PKG-INFO`

 * *Files 0% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: pytest_robotframework
-Version: 4.2.0
+Version: 4.2.1
 Summary: a pytest plugin that can run both python and robotframework tests while generating robot reports for them
 Author-Email: DetachHead <detachhead@users.noreply.github.com>
 License: MIT
 Project-URL: Repository, https://github.com/detachhead/pytest-robotframework
 Requires-Python: <4.0,>=3.8
 Requires-Dist: pytest<9,>=7
 Requires-Dist: robotframework<8.0.0,>=6.1
```

