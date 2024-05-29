# Comparing `tmp/nextline_schedule-0.3.2.tar.gz` & `tmp/nextline_schedule-0.3.3.tar.gz`

## Comparing `nextline_schedule-0.3.2.tar` & `nextline_schedule-0.3.3.tar`

### file list

```diff
@@ -1,107 +1,107 @@
--rw-r--r--   0        0        0       95 2020-02-02 00:00:00.000000 nextline_schedule-0.3.2/setup.cfg
--rw-r--r--   0        0        0       13 2020-02-02 00:00:00.000000 nextline_schedule-0.3.2/.github/CODEOWNERS
--rw-r--r--   0        0        0      624 2020-02-02 00:00:00.000000 nextline_schedule-0.3.2/.github/dependabot.yml
--rw-r--r--   0        0        0       79 2020-02-02 00:00:00.000000 nextline_schedule-0.3.2/.github/release.yml
--rw-r--r--   0        0        0      647 2020-02-02 00:00:00.000000 nextline_schedule-0.3.2/.github/workflows/pypi.yml
--rw-r--r--   0        0        0      577 2020-02-02 00:00:00.000000 nextline_schedule-0.3.2/.github/workflows/release.yml
--rw-r--r--   0        0        0      538 2020-02-02 00:00:00.000000 nextline_schedule-0.3.2/.github/workflows/type-check.yml
--rw-r--r--   0        0        0     1180 2020-02-02 00:00:00.000000 nextline_schedule-0.3.2/.github/workflows/unit-test-latest.yml
--rw-r--r--   0        0        0     1399 2020-02-02 00:00:00.000000 nextline_schedule-0.3.2/.github/workflows/unit-test-min.yml
--rw-r--r--   0        0        0     1431 2020-02-02 00:00:00.000000 nextline_schedule-0.3.2/.github/workflows/unit-test.yml
--rw-r--r--   0        0        0      398 2020-02-02 00:00:00.000000 nextline_schedule-0.3.2/.vscode/settings.json
--rw-r--r--   0        0        0      413 2020-02-02 00:00:00.000000 nextline_schedule-0.3.2/ci/latest/requirements.txt
--rw-r--r--   0        0        0      421 2020-02-02 00:00:00.000000 nextline_schedule-0.3.2/ci/minimum/requirements.txt
--rw-r--r--   0        0        0       22 2020-02-02 00:00:00.000000 nextline_schedule-0.3.2/src/nextline_schedule/__about__.py
--rw-r--r--   0        0        0      100 2020-02-02 00:00:00.000000 nextline_schedule-0.3.2/src/nextline_schedule/__init__.py
--rw-r--r--   0        0        0      349 2020-02-02 00:00:00.000000 nextline_schedule-0.3.2/src/nextline_schedule/default.toml
--rw-r--r--   0        0        0      473 2020-02-02 00:00:00.000000 nextline_schedule-0.3.2/src/nextline_schedule/dummy.py
--rw-r--r--   0        0        0     2452 2020-02-02 00:00:00.000000 nextline_schedule-0.3.2/src/nextline_schedule/plugin.py
--rw-r--r--   0        0        0        0 2020-02-02 00:00:00.000000 nextline_schedule-0.3.2/src/nextline_schedule/py.typed
--rw-r--r--   0        0        0     1460 2020-02-02 00:00:00.000000 nextline_schedule-0.3.2/src/nextline_schedule/scheduler.py
--rw-r--r--   0        0        0      140 2020-02-02 00:00:00.000000 nextline_schedule-0.3.2/src/nextline_schedule/types.py
--rw-r--r--   0        0        0      139 2020-02-02 00:00:00.000000 nextline_schedule-0.3.2/src/nextline_schedule/auto/__init__.py
--rw-r--r--   0        0        0     3833 2020-02-02 00:00:00.000000 nextline_schedule-0.3.2/src/nextline_schedule/auto/auto_mode.py
--rw-r--r--   0        0        0     2675 2020-02-02 00:00:00.000000 nextline_schedule-0.3.2/src/nextline_schedule/auto/callback.py
--rw-r--r--   0        0        0      148 2020-02-02 00:00:00.000000 nextline_schedule-0.3.2/src/nextline_schedule/auto/types.py
--rw-r--r--   0        0        0       85 2020-02-02 00:00:00.000000 nextline_schedule-0.3.2/src/nextline_schedule/auto/state_machine/__init__.py
--rw-r--r--   0        0        0     4687 2020-02-02 00:00:00.000000 nextline_schedule-0.3.2/src/nextline_schedule/auto/state_machine/factory.py
--rw-r--r--   0        0        0     2819 2020-02-02 00:00:00.000000 nextline_schedule-0.3.2/src/nextline_schedule/auto/state_machine/machine.py
--rw-r--r--   0        0        0     1414 2020-02-02 00:00:00.000000 nextline_schedule-0.3.2/src/nextline_schedule/graphql/__init__.py
--rw-r--r--   0        0        0      124 2020-02-02 00:00:00.000000 nextline_schedule-0.3.2/src/nextline_schedule/graphql/mutations/auto_mode/ChangeMode.gql
--rw-r--r--   0        0        0       89 2020-02-02 00:00:00.000000 nextline_schedule-0.3.2/src/nextline_schedule/graphql/mutations/auto_mode/TurnOff.gql
--rw-r--r--   0        0        0       87 2020-02-02 00:00:00.000000 nextline_schedule-0.3.2/src/nextline_schedule/graphql/mutations/auto_mode/TurnOn.gql
--rw-r--r--   0        0        0      192 2020-02-02 00:00:00.000000 nextline_schedule-0.3.2/src/nextline_schedule/graphql/mutations/queue/Push.gql
--rw-r--r--   0        0        0      101 2020-02-02 00:00:00.000000 nextline_schedule-0.3.2/src/nextline_schedule/graphql/mutations/queue/Remove.gql
--rw-r--r--   0        0        0       97 2020-02-02 00:00:00.000000 nextline_schedule-0.3.2/src/nextline_schedule/graphql/mutations/scheduler/LoadScript.gql
--rw-r--r--   0        0        0      143 2020-02-02 00:00:00.000000 nextline_schedule-0.3.2/src/nextline_schedule/graphql/mutations/scheduler/Update.gql
--rw-r--r--   0        0        0      105 2020-02-02 00:00:00.000000 nextline_schedule-0.3.2/src/nextline_schedule/graphql/queries/Scheduler.gql
--rw-r--r--   0        0        0       47 2020-02-02 00:00:00.000000 nextline_schedule-0.3.2/src/nextline_schedule/graphql/queries/Version.gql
--rw-r--r--   0        0        0       80 2020-02-02 00:00:00.000000 nextline_schedule-0.3.2/src/nextline_schedule/graphql/queries/auto_mode/Mode.gql
--rw-r--r--   0        0        0       82 2020-02-02 00:00:00.000000 nextline_schedule-0.3.2/src/nextline_schedule/graphql/queries/auto_mode/State.gql
--rw-r--r--   0        0        0      143 2020-02-02 00:00:00.000000 nextline_schedule-0.3.2/src/nextline_schedule/graphql/queries/queue/Items.gql
--rw-r--r--   0        0        0       65 2020-02-02 00:00:00.000000 nextline_schedule-0.3.2/src/nextline_schedule/graphql/subscriptions/ScheduleAutoModeMode.gql
--rw-r--r--   0        0        0       66 2020-02-02 00:00:00.000000 nextline_schedule-0.3.2/src/nextline_schedule/graphql/subscriptions/ScheduleAutoModeState.gql
--rw-r--r--   0        0        0      107 2020-02-02 00:00:00.000000 nextline_schedule-0.3.2/src/nextline_schedule/graphql/subscriptions/ScheduleQueueItems.gql
--rw-r--r--   0        0        0      200 2020-02-02 00:00:00.000000 nextline_schedule-0.3.2/src/nextline_schedule/queue/__init__.py
--rw-r--r--   0        0        0      437 2020-02-02 00:00:00.000000 nextline_schedule-0.3.2/src/nextline_schedule/queue/item.py
--rw-r--r--   0        0        0     1758 2020-02-02 00:00:00.000000 nextline_schedule-0.3.2/src/nextline_schedule/queue/queue.py
--rw-r--r--   0        0        0     1132 2020-02-02 00:00:00.000000 nextline_schedule-0.3.2/src/nextline_schedule/queue/queue_imp.py
--rw-r--r--   0        0        0     1354 2020-02-02 00:00:00.000000 nextline_schedule-0.3.2/src/nextline_schedule/queue/strategies.py
--rw-r--r--   0        0        0      144 2020-02-02 00:00:00.000000 nextline_schedule-0.3.2/src/nextline_schedule/schema/__init__.py
--rw-r--r--   0        0        0      953 2020-02-02 00:00:00.000000 nextline_schedule-0.3.2/src/nextline_schedule/schema/mutation.py
--rw-r--r--   0        0        0      711 2020-02-02 00:00:00.000000 nextline_schedule-0.3.2/src/nextline_schedule/schema/query.py
--rw-r--r--   0        0        0      681 2020-02-02 00:00:00.000000 nextline_schedule-0.3.2/src/nextline_schedule/schema/subscription.py
--rw-r--r--   0        0        0      307 2020-02-02 00:00:00.000000 nextline_schedule-0.3.2/src/nextline_schedule/schema/auto/__init__.py
--rw-r--r--   0        0        0     1029 2020-02-02 00:00:00.000000 nextline_schedule-0.3.2/src/nextline_schedule/schema/auto/mutation.py
--rw-r--r--   0        0        0      617 2020-02-02 00:00:00.000000 nextline_schedule-0.3.2/src/nextline_schedule/schema/auto/query.py
--rw-r--r--   0        0        0      526 2020-02-02 00:00:00.000000 nextline_schedule-0.3.2/src/nextline_schedule/schema/auto/subscription.py
--rw-r--r--   0        0        0      309 2020-02-02 00:00:00.000000 nextline_schedule-0.3.2/src/nextline_schedule/schema/queue/__init__.py
--rw-r--r--   0        0        0      989 2020-02-02 00:00:00.000000 nextline_schedule-0.3.2/src/nextline_schedule/schema/queue/mutation.py
--rw-r--r--   0        0        0      485 2020-02-02 00:00:00.000000 nextline_schedule-0.3.2/src/nextline_schedule/schema/queue/query.py
--rw-r--r--   0        0        0      451 2020-02-02 00:00:00.000000 nextline_schedule-0.3.2/src/nextline_schedule/schema/queue/subscription.py
--rw-r--r--   0        0        0      429 2020-02-02 00:00:00.000000 nextline_schedule-0.3.2/src/nextline_schedule/schema/queue/types.py
--rw-r--r--   0        0        0      168 2020-02-02 00:00:00.000000 nextline_schedule-0.3.2/src/nextline_schedule/schema/scheduler/__init__.py
--rw-r--r--   0        0        0     1308 2020-02-02 00:00:00.000000 nextline_schedule-0.3.2/src/nextline_schedule/schema/scheduler/mutation.py
--rw-r--r--   0        0        0      920 2020-02-02 00:00:00.000000 nextline_schedule-0.3.2/src/nextline_schedule/schema/scheduler/query.py
--rw-r--r--   0        0        0      214 2020-02-02 00:00:00.000000 nextline_schedule-0.3.2/src/nextline_schedule/utils/__init__.py
--rw-r--r--   0        0        0     2855 2020-02-02 00:00:00.000000 nextline_schedule-0.3.2/src/nextline_schedule/utils/safe.py
--rw-r--r--   0        0        0      874 2020-02-02 00:00:00.000000 nextline_schedule-0.3.2/src/nextline_schedule/utils/utc.py
--rw-r--r--   0        0        0      301 2020-02-02 00:00:00.000000 nextline_schedule-0.3.2/src/nextline_schedule/utils/strategies/__init__.py
--rw-r--r--   0        0        0      774 2020-02-02 00:00:00.000000 nextline_schedule-0.3.2/src/nextline_schedule/utils/strategies/datetime.py
--rw-r--r--   0        0        0     3790 2020-02-02 00:00:00.000000 nextline_schedule-0.3.2/src/nextline_schedule/utils/strategies/misc.py
--rw-r--r--   0        0        0      707 2020-02-02 00:00:00.000000 nextline_schedule-0.3.2/src/nextline_schedule/utils/strategies/script.py
--rw-r--r--   0        0        0        0 2020-02-02 00:00:00.000000 nextline_schedule-0.3.2/tests/__init__.py
--rw-r--r--   0        0        0      169 2020-02-02 00:00:00.000000 nextline_schedule-0.3.2/tests/conftest.py
--rw-r--r--   0        0        0     2584 2020-02-02 00:00:00.000000 nextline_schedule-0.3.2/tests/test_plugin.py
--rw-r--r--   0        0        0     2301 2020-02-02 00:00:00.000000 nextline_schedule-0.3.2/tests/test_scheduler.py
--rw-r--r--   0        0        0     1073 2020-02-02 00:00:00.000000 nextline_schedule-0.3.2/tests/test_scratch.py
--rw-r--r--   0        0        0      149 2020-02-02 00:00:00.000000 nextline_schedule-0.3.2/tests/test_version.py
--rw-r--r--   0        0        0        0 2020-02-02 00:00:00.000000 nextline_schedule-0.3.2/tests/auto/__init__.py
--rw-r--r--   0        0        0     1663 2020-02-02 00:00:00.000000 nextline_schedule-0.3.2/tests/auto/test_auto.py
--rw-r--r--   0        0        0     1805 2020-02-02 00:00:00.000000 nextline_schedule-0.3.2/tests/auto/test_auto_on_raised.py
--rw-r--r--   0        0        0     1319 2020-02-02 00:00:00.000000 nextline_schedule-0.3.2/tests/auto/test_auto_turn_off.py
--rw-r--r--   0        0        0        0 2020-02-02 00:00:00.000000 nextline_schedule-0.3.2/tests/auto/state_machine/__init__.py
--rw-r--r--   0        0        0     3710 2020-02-02 00:00:00.000000 nextline_schedule-0.3.2/tests/auto/state_machine/test_fsm.py
--rw-r--r--   0        0        0        0 2020-02-02 00:00:00.000000 nextline_schedule-0.3.2/tests/queue/__init__.py
--rw-r--r--   0        0        0     2495 2020-02-02 00:00:00.000000 nextline_schedule-0.3.2/tests/queue/test_queue.py
--rw-r--r--   0        0        0     1335 2020-02-02 00:00:00.000000 nextline_schedule-0.3.2/tests/queue/test_queue_imp.py
--rw-r--r--   0        0        0        0 2020-02-02 00:00:00.000000 nextline_schedule-0.3.2/tests/schema/__init__.py
--rw-r--r--   0        0        0      410 2020-02-02 00:00:00.000000 nextline_schedule-0.3.2/tests/schema/conftest.py
--rw-r--r--   0        0        0        0 2020-02-02 00:00:00.000000 nextline_schedule-0.3.2/tests/schema/mutations/__init__.py
--rw-r--r--   0        0        0     2592 2020-02-02 00:00:00.000000 nextline_schedule-0.3.2/tests/schema/mutations/test_queue_push.py
--rw-r--r--   0        0        0        0 2020-02-02 00:00:00.000000 nextline_schedule-0.3.2/tests/schema/queries/__init__.py
--rw-r--r--   0        0        0      568 2020-02-02 00:00:00.000000 nextline_schedule-0.3.2/tests/schema/queries/test_queue_items.py
--rw-r--r--   0        0        0      312 2020-02-02 00:00:00.000000 nextline_schedule-0.3.2/tests/schema/queries/test_version.py
--rw-r--r--   0        0        0        0 2020-02-02 00:00:00.000000 nextline_schedule-0.3.2/tests/utils/__init__.py
--rw-r--r--   0        0        0      727 2020-02-02 00:00:00.000000 nextline_schedule-0.3.2/tests/utils/test_safe_compare.py
--rw-r--r--   0        0        0     1047 2020-02-02 00:00:00.000000 nextline_schedule-0.3.2/tests/utils/test_safe_min_max.py
--rw-r--r--   0        0        0        0 2020-02-02 00:00:00.000000 nextline_schedule-0.3.2/tests/utils/strategies/__init__.py
--rw-r--r--   0        0        0      498 2020-02-02 00:00:00.000000 nextline_schedule-0.3.2/tests/utils/strategies/test_st_datetimes.py
--rw-r--r--   0        0        0      665 2020-02-02 00:00:00.000000 nextline_schedule-0.3.2/tests/utils/strategies/test_st_ints.py
--rw-r--r--   0        0        0      360 2020-02-02 00:00:00.000000 nextline_schedule-0.3.2/tests/utils/strategies/test_st_python_scripts.py
--rw-r--r--   0        0        0     2886 2020-02-02 00:00:00.000000 nextline_schedule-0.3.2/tests/utils/strategies/test_st_ranges.py
--rw-r--r--   0        0        0     3078 2020-02-02 00:00:00.000000 nextline_schedule-0.3.2/.gitignore
--rw-r--r--   0        0        0     1083 2020-02-02 00:00:00.000000 nextline_schedule-0.3.2/LICENSE.txt
--rw-r--r--   0        0        0     2035 2020-02-02 00:00:00.000000 nextline_schedule-0.3.2/README.md
--rw-r--r--   0        0        0     2570 2020-02-02 00:00:00.000000 nextline_schedule-0.3.2/pyproject.toml
--rw-r--r--   0        0        0     3399 2020-02-02 00:00:00.000000 nextline_schedule-0.3.2/PKG-INFO
+-rw-r--r--   0        0        0       95 2020-02-02 00:00:00.000000 nextline_schedule-0.3.3/setup.cfg
+-rw-r--r--   0        0        0       13 2020-02-02 00:00:00.000000 nextline_schedule-0.3.3/.github/CODEOWNERS
+-rw-r--r--   0        0        0      624 2020-02-02 00:00:00.000000 nextline_schedule-0.3.3/.github/dependabot.yml
+-rw-r--r--   0        0        0       79 2020-02-02 00:00:00.000000 nextline_schedule-0.3.3/.github/release.yml
+-rw-r--r--   0        0        0      647 2020-02-02 00:00:00.000000 nextline_schedule-0.3.3/.github/workflows/pypi.yml
+-rw-r--r--   0        0        0      577 2020-02-02 00:00:00.000000 nextline_schedule-0.3.3/.github/workflows/release.yml
+-rw-r--r--   0        0        0      538 2020-02-02 00:00:00.000000 nextline_schedule-0.3.3/.github/workflows/type-check.yml
+-rw-r--r--   0        0        0     1180 2020-02-02 00:00:00.000000 nextline_schedule-0.3.3/.github/workflows/unit-test-latest.yml
+-rw-r--r--   0        0        0     1399 2020-02-02 00:00:00.000000 nextline_schedule-0.3.3/.github/workflows/unit-test-min.yml
+-rw-r--r--   0        0        0     1431 2020-02-02 00:00:00.000000 nextline_schedule-0.3.3/.github/workflows/unit-test.yml
+-rw-r--r--   0        0        0      398 2020-02-02 00:00:00.000000 nextline_schedule-0.3.3/.vscode/settings.json
+-rw-r--r--   0        0        0      413 2020-02-02 00:00:00.000000 nextline_schedule-0.3.3/ci/latest/requirements.txt
+-rw-r--r--   0        0        0      421 2020-02-02 00:00:00.000000 nextline_schedule-0.3.3/ci/minimum/requirements.txt
+-rw-r--r--   0        0        0       22 2020-02-02 00:00:00.000000 nextline_schedule-0.3.3/src/nextline_schedule/__about__.py
+-rw-r--r--   0        0        0      100 2020-02-02 00:00:00.000000 nextline_schedule-0.3.3/src/nextline_schedule/__init__.py
+-rw-r--r--   0        0        0      349 2020-02-02 00:00:00.000000 nextline_schedule-0.3.3/src/nextline_schedule/default.toml
+-rw-r--r--   0        0        0      473 2020-02-02 00:00:00.000000 nextline_schedule-0.3.3/src/nextline_schedule/dummy.py
+-rw-r--r--   0        0        0     2452 2020-02-02 00:00:00.000000 nextline_schedule-0.3.3/src/nextline_schedule/plugin.py
+-rw-r--r--   0        0        0        0 2020-02-02 00:00:00.000000 nextline_schedule-0.3.3/src/nextline_schedule/py.typed
+-rw-r--r--   0        0        0     1460 2020-02-02 00:00:00.000000 nextline_schedule-0.3.3/src/nextline_schedule/scheduler.py
+-rw-r--r--   0        0        0      140 2020-02-02 00:00:00.000000 nextline_schedule-0.3.3/src/nextline_schedule/types.py
+-rw-r--r--   0        0        0      139 2020-02-02 00:00:00.000000 nextline_schedule-0.3.3/src/nextline_schedule/auto/__init__.py
+-rw-r--r--   0        0        0     3833 2020-02-02 00:00:00.000000 nextline_schedule-0.3.3/src/nextline_schedule/auto/auto_mode.py
+-rw-r--r--   0        0        0     2675 2020-02-02 00:00:00.000000 nextline_schedule-0.3.3/src/nextline_schedule/auto/callback.py
+-rw-r--r--   0        0        0      148 2020-02-02 00:00:00.000000 nextline_schedule-0.3.3/src/nextline_schedule/auto/types.py
+-rw-r--r--   0        0        0       85 2020-02-02 00:00:00.000000 nextline_schedule-0.3.3/src/nextline_schedule/auto/state_machine/__init__.py
+-rw-r--r--   0        0        0     4687 2020-02-02 00:00:00.000000 nextline_schedule-0.3.3/src/nextline_schedule/auto/state_machine/factory.py
+-rw-r--r--   0        0        0     2819 2020-02-02 00:00:00.000000 nextline_schedule-0.3.3/src/nextline_schedule/auto/state_machine/machine.py
+-rw-r--r--   0        0        0     1414 2020-02-02 00:00:00.000000 nextline_schedule-0.3.3/src/nextline_schedule/graphql/__init__.py
+-rw-r--r--   0        0        0      124 2020-02-02 00:00:00.000000 nextline_schedule-0.3.3/src/nextline_schedule/graphql/mutations/auto_mode/ChangeMode.gql
+-rw-r--r--   0        0        0       89 2020-02-02 00:00:00.000000 nextline_schedule-0.3.3/src/nextline_schedule/graphql/mutations/auto_mode/TurnOff.gql
+-rw-r--r--   0        0        0       87 2020-02-02 00:00:00.000000 nextline_schedule-0.3.3/src/nextline_schedule/graphql/mutations/auto_mode/TurnOn.gql
+-rw-r--r--   0        0        0      192 2020-02-02 00:00:00.000000 nextline_schedule-0.3.3/src/nextline_schedule/graphql/mutations/queue/Push.gql
+-rw-r--r--   0        0        0      101 2020-02-02 00:00:00.000000 nextline_schedule-0.3.3/src/nextline_schedule/graphql/mutations/queue/Remove.gql
+-rw-r--r--   0        0        0       97 2020-02-02 00:00:00.000000 nextline_schedule-0.3.3/src/nextline_schedule/graphql/mutations/scheduler/LoadScript.gql
+-rw-r--r--   0        0        0      143 2020-02-02 00:00:00.000000 nextline_schedule-0.3.3/src/nextline_schedule/graphql/mutations/scheduler/Update.gql
+-rw-r--r--   0        0        0      105 2020-02-02 00:00:00.000000 nextline_schedule-0.3.3/src/nextline_schedule/graphql/queries/Scheduler.gql
+-rw-r--r--   0        0        0       47 2020-02-02 00:00:00.000000 nextline_schedule-0.3.3/src/nextline_schedule/graphql/queries/Version.gql
+-rw-r--r--   0        0        0       80 2020-02-02 00:00:00.000000 nextline_schedule-0.3.3/src/nextline_schedule/graphql/queries/auto_mode/Mode.gql
+-rw-r--r--   0        0        0       82 2020-02-02 00:00:00.000000 nextline_schedule-0.3.3/src/nextline_schedule/graphql/queries/auto_mode/State.gql
+-rw-r--r--   0        0        0      143 2020-02-02 00:00:00.000000 nextline_schedule-0.3.3/src/nextline_schedule/graphql/queries/queue/Items.gql
+-rw-r--r--   0        0        0       65 2020-02-02 00:00:00.000000 nextline_schedule-0.3.3/src/nextline_schedule/graphql/subscriptions/ScheduleAutoModeMode.gql
+-rw-r--r--   0        0        0       66 2020-02-02 00:00:00.000000 nextline_schedule-0.3.3/src/nextline_schedule/graphql/subscriptions/ScheduleAutoModeState.gql
+-rw-r--r--   0        0        0      107 2020-02-02 00:00:00.000000 nextline_schedule-0.3.3/src/nextline_schedule/graphql/subscriptions/ScheduleQueueItems.gql
+-rw-r--r--   0        0        0      200 2020-02-02 00:00:00.000000 nextline_schedule-0.3.3/src/nextline_schedule/queue/__init__.py
+-rw-r--r--   0        0        0      437 2020-02-02 00:00:00.000000 nextline_schedule-0.3.3/src/nextline_schedule/queue/item.py
+-rw-r--r--   0        0        0     2586 2020-02-02 00:00:00.000000 nextline_schedule-0.3.3/src/nextline_schedule/queue/queue.py
+-rw-r--r--   0        0        0     2212 2020-02-02 00:00:00.000000 nextline_schedule-0.3.3/src/nextline_schedule/queue/queue_imp.py
+-rw-r--r--   0        0        0     1354 2020-02-02 00:00:00.000000 nextline_schedule-0.3.3/src/nextline_schedule/queue/strategies.py
+-rw-r--r--   0        0        0      144 2020-02-02 00:00:00.000000 nextline_schedule-0.3.3/src/nextline_schedule/schema/__init__.py
+-rw-r--r--   0        0        0      687 2020-02-02 00:00:00.000000 nextline_schedule-0.3.3/src/nextline_schedule/schema/mutation.py
+-rw-r--r--   0        0        0      711 2020-02-02 00:00:00.000000 nextline_schedule-0.3.3/src/nextline_schedule/schema/query.py
+-rw-r--r--   0        0        0      681 2020-02-02 00:00:00.000000 nextline_schedule-0.3.3/src/nextline_schedule/schema/subscription.py
+-rw-r--r--   0        0        0      307 2020-02-02 00:00:00.000000 nextline_schedule-0.3.3/src/nextline_schedule/schema/auto/__init__.py
+-rw-r--r--   0        0        0     1038 2020-02-02 00:00:00.000000 nextline_schedule-0.3.3/src/nextline_schedule/schema/auto/mutation.py
+-rw-r--r--   0        0        0      617 2020-02-02 00:00:00.000000 nextline_schedule-0.3.3/src/nextline_schedule/schema/auto/query.py
+-rw-r--r--   0        0        0      526 2020-02-02 00:00:00.000000 nextline_schedule-0.3.3/src/nextline_schedule/schema/auto/subscription.py
+-rw-r--r--   0        0        0      309 2020-02-02 00:00:00.000000 nextline_schedule-0.3.3/src/nextline_schedule/schema/queue/__init__.py
+-rw-r--r--   0        0        0     2221 2020-02-02 00:00:00.000000 nextline_schedule-0.3.3/src/nextline_schedule/schema/queue/mutation.py
+-rw-r--r--   0        0        0      485 2020-02-02 00:00:00.000000 nextline_schedule-0.3.3/src/nextline_schedule/schema/queue/query.py
+-rw-r--r--   0        0        0      451 2020-02-02 00:00:00.000000 nextline_schedule-0.3.3/src/nextline_schedule/schema/queue/subscription.py
+-rw-r--r--   0        0        0      429 2020-02-02 00:00:00.000000 nextline_schedule-0.3.3/src/nextline_schedule/schema/queue/types.py
+-rw-r--r--   0        0        0      168 2020-02-02 00:00:00.000000 nextline_schedule-0.3.3/src/nextline_schedule/schema/scheduler/__init__.py
+-rw-r--r--   0        0        0     1308 2020-02-02 00:00:00.000000 nextline_schedule-0.3.3/src/nextline_schedule/schema/scheduler/mutation.py
+-rw-r--r--   0        0        0      920 2020-02-02 00:00:00.000000 nextline_schedule-0.3.3/src/nextline_schedule/schema/scheduler/query.py
+-rw-r--r--   0        0        0      214 2020-02-02 00:00:00.000000 nextline_schedule-0.3.3/src/nextline_schedule/utils/__init__.py
+-rw-r--r--   0        0        0     2855 2020-02-02 00:00:00.000000 nextline_schedule-0.3.3/src/nextline_schedule/utils/safe.py
+-rw-r--r--   0        0        0      874 2020-02-02 00:00:00.000000 nextline_schedule-0.3.3/src/nextline_schedule/utils/utc.py
+-rw-r--r--   0        0        0      301 2020-02-02 00:00:00.000000 nextline_schedule-0.3.3/src/nextline_schedule/utils/strategies/__init__.py
+-rw-r--r--   0        0        0      774 2020-02-02 00:00:00.000000 nextline_schedule-0.3.3/src/nextline_schedule/utils/strategies/datetime.py
+-rw-r--r--   0        0        0     3790 2020-02-02 00:00:00.000000 nextline_schedule-0.3.3/src/nextline_schedule/utils/strategies/misc.py
+-rw-r--r--   0        0        0      707 2020-02-02 00:00:00.000000 nextline_schedule-0.3.3/src/nextline_schedule/utils/strategies/script.py
+-rw-r--r--   0        0        0        0 2020-02-02 00:00:00.000000 nextline_schedule-0.3.3/tests/__init__.py
+-rw-r--r--   0        0        0      169 2020-02-02 00:00:00.000000 nextline_schedule-0.3.3/tests/conftest.py
+-rw-r--r--   0        0        0     2584 2020-02-02 00:00:00.000000 nextline_schedule-0.3.3/tests/test_plugin.py
+-rw-r--r--   0        0        0     2301 2020-02-02 00:00:00.000000 nextline_schedule-0.3.3/tests/test_scheduler.py
+-rw-r--r--   0        0        0     1073 2020-02-02 00:00:00.000000 nextline_schedule-0.3.3/tests/test_scratch.py
+-rw-r--r--   0        0        0      149 2020-02-02 00:00:00.000000 nextline_schedule-0.3.3/tests/test_version.py
+-rw-r--r--   0        0        0        0 2020-02-02 00:00:00.000000 nextline_schedule-0.3.3/tests/auto/__init__.py
+-rw-r--r--   0        0        0     1663 2020-02-02 00:00:00.000000 nextline_schedule-0.3.3/tests/auto/test_auto.py
+-rw-r--r--   0        0        0     1805 2020-02-02 00:00:00.000000 nextline_schedule-0.3.3/tests/auto/test_auto_on_raised.py
+-rw-r--r--   0        0        0     1319 2020-02-02 00:00:00.000000 nextline_schedule-0.3.3/tests/auto/test_auto_turn_off.py
+-rw-r--r--   0        0        0        0 2020-02-02 00:00:00.000000 nextline_schedule-0.3.3/tests/auto/state_machine/__init__.py
+-rw-r--r--   0        0        0     3710 2020-02-02 00:00:00.000000 nextline_schedule-0.3.3/tests/auto/state_machine/test_fsm.py
+-rw-r--r--   0        0        0        0 2020-02-02 00:00:00.000000 nextline_schedule-0.3.3/tests/queue/__init__.py
+-rw-r--r--   0        0        0     2495 2020-02-02 00:00:00.000000 nextline_schedule-0.3.3/tests/queue/test_queue.py
+-rw-r--r--   0        0        0     1335 2020-02-02 00:00:00.000000 nextline_schedule-0.3.3/tests/queue/test_queue_imp.py
+-rw-r--r--   0        0        0        0 2020-02-02 00:00:00.000000 nextline_schedule-0.3.3/tests/schema/__init__.py
+-rw-r--r--   0        0        0      410 2020-02-02 00:00:00.000000 nextline_schedule-0.3.3/tests/schema/conftest.py
+-rw-r--r--   0        0        0        0 2020-02-02 00:00:00.000000 nextline_schedule-0.3.3/tests/schema/mutations/__init__.py
+-rw-r--r--   0        0        0     2592 2020-02-02 00:00:00.000000 nextline_schedule-0.3.3/tests/schema/mutations/test_queue_push.py
+-rw-r--r--   0        0        0        0 2020-02-02 00:00:00.000000 nextline_schedule-0.3.3/tests/schema/queries/__init__.py
+-rw-r--r--   0        0        0      568 2020-02-02 00:00:00.000000 nextline_schedule-0.3.3/tests/schema/queries/test_queue_items.py
+-rw-r--r--   0        0        0      312 2020-02-02 00:00:00.000000 nextline_schedule-0.3.3/tests/schema/queries/test_version.py
+-rw-r--r--   0        0        0        0 2020-02-02 00:00:00.000000 nextline_schedule-0.3.3/tests/utils/__init__.py
+-rw-r--r--   0        0        0      727 2020-02-02 00:00:00.000000 nextline_schedule-0.3.3/tests/utils/test_safe_compare.py
+-rw-r--r--   0        0        0     1047 2020-02-02 00:00:00.000000 nextline_schedule-0.3.3/tests/utils/test_safe_min_max.py
+-rw-r--r--   0        0        0        0 2020-02-02 00:00:00.000000 nextline_schedule-0.3.3/tests/utils/strategies/__init__.py
+-rw-r--r--   0        0        0      498 2020-02-02 00:00:00.000000 nextline_schedule-0.3.3/tests/utils/strategies/test_st_datetimes.py
+-rw-r--r--   0        0        0      665 2020-02-02 00:00:00.000000 nextline_schedule-0.3.3/tests/utils/strategies/test_st_ints.py
+-rw-r--r--   0        0        0      360 2020-02-02 00:00:00.000000 nextline_schedule-0.3.3/tests/utils/strategies/test_st_python_scripts.py
+-rw-r--r--   0        0        0     2886 2020-02-02 00:00:00.000000 nextline_schedule-0.3.3/tests/utils/strategies/test_st_ranges.py
+-rw-r--r--   0        0        0     3078 2020-02-02 00:00:00.000000 nextline_schedule-0.3.3/.gitignore
+-rw-r--r--   0        0        0     1083 2020-02-02 00:00:00.000000 nextline_schedule-0.3.3/LICENSE.txt
+-rw-r--r--   0        0        0     2035 2020-02-02 00:00:00.000000 nextline_schedule-0.3.3/README.md
+-rw-r--r--   0        0        0     2570 2020-02-02 00:00:00.000000 nextline_schedule-0.3.3/pyproject.toml
+-rw-r--r--   0        0        0     3399 2020-02-02 00:00:00.000000 nextline_schedule-0.3.3/PKG-INFO
```

### Comparing `nextline_schedule-0.3.2/.github/dependabot.yml` & `nextline_schedule-0.3.3/.github/dependabot.yml`

 * *Files identical despite different names*

### Comparing `nextline_schedule-0.3.2/.github/workflows/pypi.yml` & `nextline_schedule-0.3.3/.github/workflows/pypi.yml`

 * *Files identical despite different names*

### Comparing `nextline_schedule-0.3.2/.github/workflows/release.yml` & `nextline_schedule-0.3.3/.github/workflows/release.yml`

 * *Files identical despite different names*

### Comparing `nextline_schedule-0.3.2/.github/workflows/type-check.yml` & `nextline_schedule-0.3.3/.github/workflows/type-check.yml`

 * *Files identical despite different names*

### Comparing `nextline_schedule-0.3.2/.github/workflows/unit-test-latest.yml` & `nextline_schedule-0.3.3/.github/workflows/unit-test-latest.yml`

 * *Files identical despite different names*

### Comparing `nextline_schedule-0.3.2/.github/workflows/unit-test-min.yml` & `nextline_schedule-0.3.3/.github/workflows/unit-test-min.yml`

 * *Files identical despite different names*

### Comparing `nextline_schedule-0.3.2/.github/workflows/unit-test.yml` & `nextline_schedule-0.3.3/.github/workflows/unit-test.yml`

 * *Files identical despite different names*

### Comparing `nextline_schedule-0.3.2/src/nextline_schedule/plugin.py` & `nextline_schedule-0.3.3/src/nextline_schedule/plugin.py`

 * *Files identical despite different names*

### Comparing `nextline_schedule-0.3.2/src/nextline_schedule/scheduler.py` & `nextline_schedule-0.3.3/src/nextline_schedule/scheduler.py`

 * *Files identical despite different names*

### Comparing `nextline_schedule-0.3.2/src/nextline_schedule/auto/auto_mode.py` & `nextline_schedule-0.3.3/src/nextline_schedule/auto/auto_mode.py`

 * *Files identical despite different names*

### Comparing `nextline_schedule-0.3.2/src/nextline_schedule/auto/callback.py` & `nextline_schedule-0.3.3/src/nextline_schedule/auto/callback.py`

 * *Files identical despite different names*

### Comparing `nextline_schedule-0.3.2/src/nextline_schedule/auto/state_machine/factory.py` & `nextline_schedule-0.3.3/src/nextline_schedule/auto/state_machine/factory.py`

 * *Files identical despite different names*

### Comparing `nextline_schedule-0.3.2/src/nextline_schedule/auto/state_machine/machine.py` & `nextline_schedule-0.3.3/src/nextline_schedule/auto/state_machine/machine.py`

 * *Files identical despite different names*

### Comparing `nextline_schedule-0.3.2/src/nextline_schedule/graphql/__init__.py` & `nextline_schedule-0.3.3/src/nextline_schedule/graphql/__init__.py`

 * *Files identical despite different names*

### Comparing `nextline_schedule-0.3.2/src/nextline_schedule/queue/queue.py` & `nextline_schedule-0.3.3/src/nextline_schedule/queue/queue.py`

 * *Files 26% similar despite different names*

```diff
@@ -49,14 +49,38 @@
 
     async def remove(self, id: int) -> bool:
         if not self._queue.remove(id):
             return False
         await self._pubsub.publish(list(self._queue.items))
         return True
 
+    async def move_to_first(self, id: int) -> bool:
+        if not self._queue.move_to_first(id):
+            return False
+        await self._pubsub.publish(list(self._queue.items))
+        return True
+
+    async def move_to_last(self, id: int) -> bool:
+        if not self._queue.move_to_last(id):
+            return False
+        await self._pubsub.publish(list(self._queue.items))
+        return True
+
+    async def move_one_forward(self, id: int) -> bool:
+        if not self._queue.move_one_forward(id):
+            return False
+        await self._pubsub.publish(list(self._queue.items))
+        return True
+
+    async def move_one_backward(self, id: int) -> bool:
+        if not self._queue.move_one_backward(id):
+            return False
+        await self._pubsub.publish(list(self._queue.items))
+        return True
+
     async def aclose(self) -> None:
         await self._pubsub.close()
 
     async def __aenter__(self) -> 'Queue':
         await self._pubsub.publish(list(self._queue.items))
         return self
```

### Comparing `nextline_schedule-0.3.2/src/nextline_schedule/queue/strategies.py` & `nextline_schedule-0.3.3/src/nextline_schedule/queue/strategies.py`

 * *Files identical despite different names*

### Comparing `nextline_schedule-0.3.2/src/nextline_schedule/schema/query.py` & `nextline_schedule-0.3.3/src/nextline_schedule/schema/query.py`

 * *Files identical despite different names*

### Comparing `nextline_schedule-0.3.2/src/nextline_schedule/schema/subscription.py` & `nextline_schedule-0.3.3/src/nextline_schedule/schema/subscription.py`

 * *Files identical despite different names*

### Comparing `nextline_schedule-0.3.2/src/nextline_schedule/schema/auto/mutation.py` & `nextline_schedule-0.3.3/src/nextline_schedule/schema/auto/mutation.py`

 * *Files 15% similar despite different names*

```diff
@@ -25,10 +25,10 @@
         return False
     await auto_mode.change_mode(mode)  # type: ignore
     return True
 
 
 @strawberry.type
 class MutationScheduleAutoMode:
-    turn_on: bool = strawberry.field(resolver=mutate_turn_on)
-    turn_off: bool = strawberry.field(resolver=mutate_turn_off)
-    change_mode: bool = strawberry.field(resolver=mutate_change_mode)
+    turn_on: bool = strawberry.mutation(resolver=mutate_turn_on)
+    turn_off: bool = strawberry.mutation(resolver=mutate_turn_off)
+    change_mode: bool = strawberry.mutation(resolver=mutate_change_mode)
```

### Comparing `nextline_schedule-0.3.2/src/nextline_schedule/schema/auto/query.py` & `nextline_schedule-0.3.3/src/nextline_schedule/schema/auto/query.py`

 * *Files identical despite different names*

### Comparing `nextline_schedule-0.3.2/src/nextline_schedule/schema/auto/subscription.py` & `nextline_schedule-0.3.3/src/nextline_schedule/schema/auto/subscription.py`

 * *Files identical despite different names*

### Comparing `nextline_schedule-0.3.2/src/nextline_schedule/schema/scheduler/mutation.py` & `nextline_schedule-0.3.3/src/nextline_schedule/schema/scheduler/mutation.py`

 * *Files identical despite different names*

### Comparing `nextline_schedule-0.3.2/src/nextline_schedule/schema/scheduler/query.py` & `nextline_schedule-0.3.3/src/nextline_schedule/schema/scheduler/query.py`

 * *Files identical despite different names*

### Comparing `nextline_schedule-0.3.2/src/nextline_schedule/utils/safe.py` & `nextline_schedule-0.3.3/src/nextline_schedule/utils/safe.py`

 * *Files identical despite different names*

### Comparing `nextline_schedule-0.3.2/src/nextline_schedule/utils/utc.py` & `nextline_schedule-0.3.3/src/nextline_schedule/utils/utc.py`

 * *Files identical despite different names*

### Comparing `nextline_schedule-0.3.2/src/nextline_schedule/utils/strategies/datetime.py` & `nextline_schedule-0.3.3/src/nextline_schedule/utils/strategies/datetime.py`

 * *Files identical despite different names*

### Comparing `nextline_schedule-0.3.2/src/nextline_schedule/utils/strategies/misc.py` & `nextline_schedule-0.3.3/src/nextline_schedule/utils/strategies/misc.py`

 * *Files identical despite different names*

### Comparing `nextline_schedule-0.3.2/src/nextline_schedule/utils/strategies/script.py` & `nextline_schedule-0.3.3/src/nextline_schedule/utils/strategies/script.py`

 * *Files identical despite different names*

### Comparing `nextline_schedule-0.3.2/tests/test_plugin.py` & `nextline_schedule-0.3.3/tests/test_plugin.py`

 * *Files identical despite different names*

### Comparing `nextline_schedule-0.3.2/tests/test_scheduler.py` & `nextline_schedule-0.3.3/tests/test_scheduler.py`

 * *Files identical despite different names*

### Comparing `nextline_schedule-0.3.2/tests/test_scratch.py` & `nextline_schedule-0.3.3/tests/test_scratch.py`

 * *Files identical despite different names*

### Comparing `nextline_schedule-0.3.2/tests/auto/test_auto.py` & `nextline_schedule-0.3.3/tests/auto/test_auto.py`

 * *Files identical despite different names*

### Comparing `nextline_schedule-0.3.2/tests/auto/test_auto_on_raised.py` & `nextline_schedule-0.3.3/tests/auto/test_auto_on_raised.py`

 * *Files identical despite different names*

### Comparing `nextline_schedule-0.3.2/tests/auto/test_auto_turn_off.py` & `nextline_schedule-0.3.3/tests/auto/test_auto_turn_off.py`

 * *Files identical despite different names*

### Comparing `nextline_schedule-0.3.2/tests/auto/state_machine/test_fsm.py` & `nextline_schedule-0.3.3/tests/auto/state_machine/test_fsm.py`

 * *Files identical despite different names*

### Comparing `nextline_schedule-0.3.2/tests/queue/test_queue.py` & `nextline_schedule-0.3.3/tests/queue/test_queue.py`

 * *Files identical despite different names*

### Comparing `nextline_schedule-0.3.2/tests/queue/test_queue_imp.py` & `nextline_schedule-0.3.3/tests/queue/test_queue_imp.py`

 * *Files identical despite different names*

### Comparing `nextline_schedule-0.3.2/tests/schema/mutations/test_queue_push.py` & `nextline_schedule-0.3.3/tests/schema/mutations/test_queue_push.py`

 * *Files identical despite different names*

### Comparing `nextline_schedule-0.3.2/tests/schema/queries/test_queue_items.py` & `nextline_schedule-0.3.3/tests/schema/queries/test_queue_items.py`

 * *Files identical despite different names*

### Comparing `nextline_schedule-0.3.2/tests/utils/test_safe_compare.py` & `nextline_schedule-0.3.3/tests/utils/test_safe_compare.py`

 * *Files identical despite different names*

### Comparing `nextline_schedule-0.3.2/tests/utils/test_safe_min_max.py` & `nextline_schedule-0.3.3/tests/utils/test_safe_min_max.py`

 * *Files identical despite different names*

### Comparing `nextline_schedule-0.3.2/tests/utils/strategies/test_st_ints.py` & `nextline_schedule-0.3.3/tests/utils/strategies/test_st_ints.py`

 * *Files identical despite different names*

### Comparing `nextline_schedule-0.3.2/tests/utils/strategies/test_st_ranges.py` & `nextline_schedule-0.3.3/tests/utils/strategies/test_st_ranges.py`

 * *Files identical despite different names*

### Comparing `nextline_schedule-0.3.2/.gitignore` & `nextline_schedule-0.3.3/.gitignore`

 * *Files identical despite different names*

### Comparing `nextline_schedule-0.3.2/LICENSE.txt` & `nextline_schedule-0.3.3/LICENSE.txt`

 * *Files identical despite different names*

### Comparing `nextline_schedule-0.3.2/README.md` & `nextline_schedule-0.3.3/README.md`

 * *Files identical despite different names*

### Comparing `nextline_schedule-0.3.2/pyproject.toml` & `nextline_schedule-0.3.3/pyproject.toml`

 * *Files identical despite different names*

### Comparing `nextline_schedule-0.3.2/PKG-INFO` & `nextline_schedule-0.3.3/PKG-INFO`

 * *Files 1% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.3
 Name: nextline-schedule
-Version: 0.3.2
+Version: 0.3.3
 Summary: A plugin of nextline-graphql. An interface to the SO scheduler.
 Project-URL: Documentation, https://github.com/simonsobs/nextline-schedule#readme
 Project-URL: Issues, https://github.com/simonsobs/nextline-schedule/issues
 Project-URL: Source, https://github.com/simonsobs/nextline-schedule
 Author-email: Simons Observatory <so_software@simonsobservatory.org>
 License-Expression: MIT
 License-File: LICENSE.txt
```

