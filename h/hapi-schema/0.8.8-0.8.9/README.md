# Comparing `tmp/hapi_schema-0.8.8.tar.gz` & `tmp/hapi_schema-0.8.9.tar.gz`

## Comparing `hapi_schema-0.8.8.tar` & `hapi_schema-0.8.9.tar`

### file list

```diff
@@ -1,97 +1,97 @@
--rw-r--r--   0        0        0     4034 2020-02-02 00:00:00.000000 hapi_schema-0.8.8/changelog.md
--rw-r--r--   0        0        0     2735 2020-02-02 00:00:00.000000 hapi_schema-0.8.8/contributing.md
--rw-r--r--   0        0        0       48 2020-02-02 00:00:00.000000 hapi_schema-0.8.8/initialize_test_db.sh
--rw-r--r--   0        0        0      937 2020-02-02 00:00:00.000000 hapi_schema-0.8.8/requirements.txt
--rw-r--r--   0        0        0      289 2020-02-02 00:00:00.000000 hapi_schema-0.8.8/.config/coveragerc
--rw-r--r--   0        0        0      809 2020-02-02 00:00:00.000000 hapi_schema-0.8.8/.config/pre-commit-config.yaml
--rw-r--r--   0        0        0       65 2020-02-02 00:00:00.000000 hapi_schema-0.8.8/.config/pytest.ini
--rw-r--r--   0        0        0      420 2020-02-02 00:00:00.000000 hapi_schema-0.8.8/.config/ruff.toml
--rw-r--r--   0        0        0      819 2020-02-02 00:00:00.000000 hapi_schema-0.8.8/.github/workflows/publish.yaml
--rw-r--r--   0        0        0     1662 2020-02-02 00:00:00.000000 hapi_schema-0.8.8/.github/workflows/run-python-tests.yaml
--rw-r--r--   0        0        0      237 2020-02-02 00:00:00.000000 hapi_schema-0.8.8/docker/docker-compose.yml
--rw-r--r--   0        0        0       59 2020-02-02 00:00:00.000000 hapi_schema-0.8.8/src/hapi_schema/__init__.py
--rw-r--r--   0        0        0      411 2020-02-02 00:00:00.000000 hapi_schema-0.8.8/src/hapi_schema/_version.py
--rw-r--r--   0        0        0     2059 2020-02-02 00:00:00.000000 hapi_schema-0.8.8/src/hapi_schema/db_admin1.py
--rw-r--r--   0        0        0     2369 2020-02-02 00:00:00.000000 hapi_schema-0.8.8/src/hapi_schema/db_admin2.py
--rw-r--r--   0        0        0     2979 2020-02-02 00:00:00.000000 hapi_schema-0.8.8/src/hapi_schema/db_conflict_event.py
--rw-r--r--   0        0        0      565 2020-02-02 00:00:00.000000 hapi_schema-0.8.8/src/hapi_schema/db_currency.py
--rw-r--r--   0        0        0      860 2020-02-02 00:00:00.000000 hapi_schema-0.8.8/src/hapi_schema/db_dataset.py
--rw-r--r--   0        0        0     3970 2020-02-02 00:00:00.000000 hapi_schema-0.8.8/src/hapi_schema/db_food_price.py
--rw-r--r--   0        0        0     3042 2020-02-02 00:00:00.000000 hapi_schema-0.8.8/src/hapi_schema/db_food_security.py
--rw-r--r--   0        0        0     2517 2020-02-02 00:00:00.000000 hapi_schema-0.8.8/src/hapi_schema/db_funding.py
--rw-r--r--   0        0        0     3939 2020-02-02 00:00:00.000000 hapi_schema-0.8.8/src/hapi_schema/db_humanitarian_needs.py
--rw-r--r--   0        0        0     1398 2020-02-02 00:00:00.000000 hapi_schema-0.8.8/src/hapi_schema/db_location.py
--rw-r--r--   0        0        0     3134 2020-02-02 00:00:00.000000 hapi_schema-0.8.8/src/hapi_schema/db_national_risk.py
--rw-r--r--   0        0        0     3919 2020-02-02 00:00:00.000000 hapi_schema-0.8.8/src/hapi_schema/db_operational_presence.py
--rw-r--r--   0        0        0     1018 2020-02-02 00:00:00.000000 hapi_schema-0.8.8/src/hapi_schema/db_org.py
--rw-r--r--   0        0        0      583 2020-02-02 00:00:00.000000 hapi_schema-0.8.8/src/hapi_schema/db_org_type.py
--rw-r--r--   0        0        0     2430 2020-02-02 00:00:00.000000 hapi_schema-0.8.8/src/hapi_schema/db_patch.py
--rw-r--r--   0        0        0     3030 2020-02-02 00:00:00.000000 hapi_schema-0.8.8/src/hapi_schema/db_population.py
--rw-r--r--   0        0        0     3269 2020-02-02 00:00:00.000000 hapi_schema-0.8.8/src/hapi_schema/db_poverty_rate.py
--rw-r--r--   0        0        0     3322 2020-02-02 00:00:00.000000 hapi_schema-0.8.8/src/hapi_schema/db_refugees.py
--rw-r--r--   0        0        0     1669 2020-02-02 00:00:00.000000 hapi_schema-0.8.8/src/hapi_schema/db_resource.py
--rw-r--r--   0        0        0      553 2020-02-02 00:00:00.000000 hapi_schema-0.8.8/src/hapi_schema/db_sector.py
--rw-r--r--   0        0        0    19527 2020-02-02 00:00:00.000000 hapi_schema-0.8.8/src/hapi_schema/db_views_as_tables.py
--rw-r--r--   0        0        0      760 2020-02-02 00:00:00.000000 hapi_schema-0.8.8/src/hapi_schema/db_wfp_commodity.py
--rw-r--r--   0        0        0     2166 2020-02-02 00:00:00.000000 hapi_schema-0.8.8/src/hapi_schema/db_wfp_market.py
--rw-r--r--   0        0        0     1013 2020-02-02 00:00:00.000000 hapi_schema-0.8.8/src/hapi_schema/views.py
--rw-r--r--   0        0        0        0 2020-02-02 00:00:00.000000 hapi_schema-0.8.8/src/hapi_schema/utils/__init__.py
--rw-r--r--   0        0        0      166 2020-02-02 00:00:00.000000 hapi_schema-0.8.8/src/hapi_schema/utils/base.py
--rw-r--r--   0        0        0     2798 2020-02-02 00:00:00.000000 hapi_schema-0.8.8/src/hapi_schema/utils/constraints.py
--rw-r--r--   0        0        0     2358 2020-02-02 00:00:00.000000 hapi_schema-0.8.8/src/hapi_schema/utils/enums.py
--rw-r--r--   0        0        0     6851 2020-02-02 00:00:00.000000 hapi_schema-0.8.8/src/hapi_schema/utils/hapi_views_code_generator.py
--rw-r--r--   0        0        0     6259 2020-02-02 00:00:00.000000 hapi_schema-0.8.8/src/hapi_schema/utils/view_as_table_code_generator.py
--rw-r--r--   0        0        0     7656 2020-02-02 00:00:00.000000 hapi_schema-0.8.8/src/hapi_schema/utils/view_as_table_definitions.toml
--rw-r--r--   0        0        0      280 2020-02-02 00:00:00.000000 hapi_schema-0.8.8/src/hapi_schema/utils/view_params.py
--rw-r--r--   0        0        0     7175 2020-02-02 00:00:00.000000 hapi_schema-0.8.8/tests/conftest.py
--rw-r--r--   0        0        0     2086 2020-02-02 00:00:00.000000 hapi_schema-0.8.8/tests/test_admin1.py
--rw-r--r--   0        0        0     2149 2020-02-02 00:00:00.000000 hapi_schema-0.8.8/tests/test_admin2.py
--rw-r--r--   0        0        0     2167 2020-02-02 00:00:00.000000 hapi_schema-0.8.8/tests/test_conflict_event.py
--rw-r--r--   0        0        0      446 2020-02-02 00:00:00.000000 hapi_schema-0.8.8/tests/test_currency.py
--rw-r--r--   0        0        0      642 2020-02-02 00:00:00.000000 hapi_schema-0.8.8/tests/test_dataset.py
--rw-r--r--   0        0        0     2514 2020-02-02 00:00:00.000000 hapi_schema-0.8.8/tests/test_food_price.py
--rw-r--r--   0        0        0     2075 2020-02-02 00:00:00.000000 hapi_schema-0.8.8/tests/test_food_security.py
--rw-r--r--   0        0        0     3942 2020-02-02 00:00:00.000000 hapi_schema-0.8.8/tests/test_funding.py
--rw-r--r--   0        0        0     3963 2020-02-02 00:00:00.000000 hapi_schema-0.8.8/tests/test_humanitarian_needs.py
--rw-r--r--   0        0        0     1938 2020-02-02 00:00:00.000000 hapi_schema-0.8.8/tests/test_location.py
--rw-r--r--   0        0        0     5310 2020-02-02 00:00:00.000000 hapi_schema-0.8.8/tests/test_national_risk.py
--rw-r--r--   0        0        0     1762 2020-02-02 00:00:00.000000 hapi_schema-0.8.8/tests/test_operational_presence.py
--rw-r--r--   0        0        0      416 2020-02-02 00:00:00.000000 hapi_schema-0.8.8/tests/test_org.py
--rw-r--r--   0        0        0      478 2020-02-02 00:00:00.000000 hapi_schema-0.8.8/tests/test_org_type.py
--rw-r--r--   0        0        0     1384 2020-02-02 00:00:00.000000 hapi_schema-0.8.8/tests/test_patch.py
--rw-r--r--   0        0        0     3296 2020-02-02 00:00:00.000000 hapi_schema-0.8.8/tests/test_population.py
--rw-r--r--   0        0        0     3266 2020-02-02 00:00:00.000000 hapi_schema-0.8.8/tests/test_poverty_rate.py
--rw-r--r--   0        0        0     3529 2020-02-02 00:00:00.000000 hapi_schema-0.8.8/tests/test_refugees.py
--rw-r--r--   0        0        0      481 2020-02-02 00:00:00.000000 hapi_schema-0.8.8/tests/test_resource.py
--rw-r--r--   0        0        0      437 2020-02-02 00:00:00.000000 hapi_schema-0.8.8/tests/test_sector.py
--rw-r--r--   0        0        0    15338 2020-02-02 00:00:00.000000 hapi_schema-0.8.8/tests/test_views_as_tables.py
--rw-r--r--   0        0        0      571 2020-02-02 00:00:00.000000 hapi_schema-0.8.8/tests/test_wfp_commodity.py
--rw-r--r--   0        0        0     1567 2020-02-02 00:00:00.000000 hapi_schema-0.8.8/tests/test_wfp_market.py
--rw-r--r--   0        0        0        0 2020-02-02 00:00:00.000000 hapi_schema-0.8.8/tests/sample_data/__init__.py
--rw-r--r--   0        0        0      411 2020-02-02 00:00:00.000000 hapi_schema-0.8.8/tests/sample_data/data_admin1.py
--rw-r--r--   0        0        0      831 2020-02-02 00:00:00.000000 hapi_schema-0.8.8/tests/sample_data/data_admin2.py
--rw-r--r--   0        0        0      636 2020-02-02 00:00:00.000000 hapi_schema-0.8.8/tests/sample_data/data_conflict_event.py
--rw-r--r--   0        0        0      153 2020-02-02 00:00:00.000000 hapi_schema-0.8.8/tests/sample_data/data_currency.py
--rw-r--r--   0        0        0      441 2020-02-02 00:00:00.000000 hapi_schema-0.8.8/tests/sample_data/data_dataset.py
--rw-r--r--   0        0        0      851 2020-02-02 00:00:00.000000 hapi_schema-0.8.8/tests/sample_data/data_food_price.py
--rw-r--r--   0        0        0     1195 2020-02-02 00:00:00.000000 hapi_schema-0.8.8/tests/sample_data/data_food_security.py
--rw-r--r--   0        0        0      448 2020-02-02 00:00:00.000000 hapi_schema-0.8.8/tests/sample_data/data_funding.py
--rw-r--r--   0        0        0     1903 2020-02-02 00:00:00.000000 hapi_schema-0.8.8/tests/sample_data/data_humanitarian_needs.py
--rw-r--r--   0        0        0      376 2020-02-02 00:00:00.000000 hapi_schema-0.8.8/tests/sample_data/data_location.py
--rw-r--r--   0        0        0      519 2020-02-02 00:00:00.000000 hapi_schema-0.8.8/tests/sample_data/data_national_risk.py
--rw-r--r--   0        0        0     1333 2020-02-02 00:00:00.000000 hapi_schema-0.8.8/tests/sample_data/data_operational_presence.py
--rw-r--r--   0        0        0      292 2020-02-02 00:00:00.000000 hapi_schema-0.8.8/tests/sample_data/data_org.py
--rw-r--r--   0        0        0      170 2020-02-02 00:00:00.000000 hapi_schema-0.8.8/tests/sample_data/data_org_type.py
--rw-r--r--   0        0        0     1641 2020-02-02 00:00:00.000000 hapi_schema-0.8.8/tests/sample_data/data_patch.py
--rw-r--r--   0        0        0     1329 2020-02-02 00:00:00.000000 hapi_schema-0.8.8/tests/sample_data/data_population.py
--rw-r--r--   0        0        0      488 2020-02-02 00:00:00.000000 hapi_schema-0.8.8/tests/sample_data/data_poverty_rate.py
--rw-r--r--   0        0        0      861 2020-02-02 00:00:00.000000 hapi_schema-0.8.8/tests/sample_data/data_refugees.py
--rw-r--r--   0        0        0     1510 2020-02-02 00:00:00.000000 hapi_schema-0.8.8/tests/sample_data/data_resource.py
--rw-r--r--   0        0        0      379 2020-02-02 00:00:00.000000 hapi_schema-0.8.8/tests/sample_data/data_sector.py
--rw-r--r--   0        0        0      238 2020-02-02 00:00:00.000000 hapi_schema-0.8.8/tests/sample_data/data_wfp_commodity.py
--rw-r--r--   0        0        0      197 2020-02-02 00:00:00.000000 hapi_schema-0.8.8/tests/sample_data/data_wfp_market.py
--rw-r--r--   0        0        0     3164 2020-02-02 00:00:00.000000 hapi_schema-0.8.8/.gitignore
--rw-r--r--   0        0        0     1099 2020-02-02 00:00:00.000000 hapi_schema-0.8.8/LICENSE
--rw-r--r--   0        0        0       64 2020-02-02 00:00:00.000000 hapi_schema-0.8.8/README.md
--rw-r--r--   0        0        0     2479 2020-02-02 00:00:00.000000 hapi_schema-0.8.8/pyproject.toml
--rw-r--r--   0        0        0     1582 2020-02-02 00:00:00.000000 hapi_schema-0.8.8/PKG-INFO
+-rw-r--r--   0        0        0     4102 2020-02-02 00:00:00.000000 hapi_schema-0.8.9/changelog.md
+-rw-r--r--   0        0        0     2735 2020-02-02 00:00:00.000000 hapi_schema-0.8.9/contributing.md
+-rw-r--r--   0        0        0       48 2020-02-02 00:00:00.000000 hapi_schema-0.8.9/initialize_test_db.sh
+-rw-r--r--   0        0        0      937 2020-02-02 00:00:00.000000 hapi_schema-0.8.9/requirements.txt
+-rw-r--r--   0        0        0      289 2020-02-02 00:00:00.000000 hapi_schema-0.8.9/.config/coveragerc
+-rw-r--r--   0        0        0      809 2020-02-02 00:00:00.000000 hapi_schema-0.8.9/.config/pre-commit-config.yaml
+-rw-r--r--   0        0        0       65 2020-02-02 00:00:00.000000 hapi_schema-0.8.9/.config/pytest.ini
+-rw-r--r--   0        0        0      420 2020-02-02 00:00:00.000000 hapi_schema-0.8.9/.config/ruff.toml
+-rw-r--r--   0        0        0      819 2020-02-02 00:00:00.000000 hapi_schema-0.8.9/.github/workflows/publish.yaml
+-rw-r--r--   0        0        0     1662 2020-02-02 00:00:00.000000 hapi_schema-0.8.9/.github/workflows/run-python-tests.yaml
+-rw-r--r--   0        0        0      237 2020-02-02 00:00:00.000000 hapi_schema-0.8.9/docker/docker-compose.yml
+-rw-r--r--   0        0        0       59 2020-02-02 00:00:00.000000 hapi_schema-0.8.9/src/hapi_schema/__init__.py
+-rw-r--r--   0        0        0      411 2020-02-02 00:00:00.000000 hapi_schema-0.8.9/src/hapi_schema/_version.py
+-rw-r--r--   0        0        0     2059 2020-02-02 00:00:00.000000 hapi_schema-0.8.9/src/hapi_schema/db_admin1.py
+-rw-r--r--   0        0        0     2369 2020-02-02 00:00:00.000000 hapi_schema-0.8.9/src/hapi_schema/db_admin2.py
+-rw-r--r--   0        0        0     2979 2020-02-02 00:00:00.000000 hapi_schema-0.8.9/src/hapi_schema/db_conflict_event.py
+-rw-r--r--   0        0        0      565 2020-02-02 00:00:00.000000 hapi_schema-0.8.9/src/hapi_schema/db_currency.py
+-rw-r--r--   0        0        0      860 2020-02-02 00:00:00.000000 hapi_schema-0.8.9/src/hapi_schema/db_dataset.py
+-rw-r--r--   0        0        0     4040 2020-02-02 00:00:00.000000 hapi_schema-0.8.9/src/hapi_schema/db_food_price.py
+-rw-r--r--   0        0        0     3109 2020-02-02 00:00:00.000000 hapi_schema-0.8.9/src/hapi_schema/db_food_security.py
+-rw-r--r--   0        0        0     2517 2020-02-02 00:00:00.000000 hapi_schema-0.8.9/src/hapi_schema/db_funding.py
+-rw-r--r--   0        0        0     4048 2020-02-02 00:00:00.000000 hapi_schema-0.8.9/src/hapi_schema/db_humanitarian_needs.py
+-rw-r--r--   0        0        0     1398 2020-02-02 00:00:00.000000 hapi_schema-0.8.9/src/hapi_schema/db_location.py
+-rw-r--r--   0        0        0     3168 2020-02-02 00:00:00.000000 hapi_schema-0.8.9/src/hapi_schema/db_national_risk.py
+-rw-r--r--   0        0        0     3919 2020-02-02 00:00:00.000000 hapi_schema-0.8.9/src/hapi_schema/db_operational_presence.py
+-rw-r--r--   0        0        0     1018 2020-02-02 00:00:00.000000 hapi_schema-0.8.9/src/hapi_schema/db_org.py
+-rw-r--r--   0        0        0      583 2020-02-02 00:00:00.000000 hapi_schema-0.8.9/src/hapi_schema/db_org_type.py
+-rw-r--r--   0        0        0     2430 2020-02-02 00:00:00.000000 hapi_schema-0.8.9/src/hapi_schema/db_patch.py
+-rw-r--r--   0        0        0     3078 2020-02-02 00:00:00.000000 hapi_schema-0.8.9/src/hapi_schema/db_population.py
+-rw-r--r--   0        0        0     3269 2020-02-02 00:00:00.000000 hapi_schema-0.8.9/src/hapi_schema/db_poverty_rate.py
+-rw-r--r--   0        0        0     3406 2020-02-02 00:00:00.000000 hapi_schema-0.8.9/src/hapi_schema/db_refugees.py
+-rw-r--r--   0        0        0     1669 2020-02-02 00:00:00.000000 hapi_schema-0.8.9/src/hapi_schema/db_resource.py
+-rw-r--r--   0        0        0      553 2020-02-02 00:00:00.000000 hapi_schema-0.8.9/src/hapi_schema/db_sector.py
+-rw-r--r--   0        0        0    19527 2020-02-02 00:00:00.000000 hapi_schema-0.8.9/src/hapi_schema/db_views_as_tables.py
+-rw-r--r--   0        0        0      798 2020-02-02 00:00:00.000000 hapi_schema-0.8.9/src/hapi_schema/db_wfp_commodity.py
+-rw-r--r--   0        0        0     2166 2020-02-02 00:00:00.000000 hapi_schema-0.8.9/src/hapi_schema/db_wfp_market.py
+-rw-r--r--   0        0        0     1013 2020-02-02 00:00:00.000000 hapi_schema-0.8.9/src/hapi_schema/views.py
+-rw-r--r--   0        0        0        0 2020-02-02 00:00:00.000000 hapi_schema-0.8.9/src/hapi_schema/utils/__init__.py
+-rw-r--r--   0        0        0      166 2020-02-02 00:00:00.000000 hapi_schema-0.8.9/src/hapi_schema/utils/base.py
+-rw-r--r--   0        0        0     2798 2020-02-02 00:00:00.000000 hapi_schema-0.8.9/src/hapi_schema/utils/constraints.py
+-rw-r--r--   0        0        0     2376 2020-02-02 00:00:00.000000 hapi_schema-0.8.9/src/hapi_schema/utils/enums.py
+-rw-r--r--   0        0        0     6851 2020-02-02 00:00:00.000000 hapi_schema-0.8.9/src/hapi_schema/utils/hapi_views_code_generator.py
+-rw-r--r--   0        0        0     6259 2020-02-02 00:00:00.000000 hapi_schema-0.8.9/src/hapi_schema/utils/view_as_table_code_generator.py
+-rw-r--r--   0        0        0     7656 2020-02-02 00:00:00.000000 hapi_schema-0.8.9/src/hapi_schema/utils/view_as_table_definitions.toml
+-rw-r--r--   0        0        0      280 2020-02-02 00:00:00.000000 hapi_schema-0.8.9/src/hapi_schema/utils/view_params.py
+-rw-r--r--   0        0        0     7175 2020-02-02 00:00:00.000000 hapi_schema-0.8.9/tests/conftest.py
+-rw-r--r--   0        0        0     2086 2020-02-02 00:00:00.000000 hapi_schema-0.8.9/tests/test_admin1.py
+-rw-r--r--   0        0        0     2149 2020-02-02 00:00:00.000000 hapi_schema-0.8.9/tests/test_admin2.py
+-rw-r--r--   0        0        0     2167 2020-02-02 00:00:00.000000 hapi_schema-0.8.9/tests/test_conflict_event.py
+-rw-r--r--   0        0        0      446 2020-02-02 00:00:00.000000 hapi_schema-0.8.9/tests/test_currency.py
+-rw-r--r--   0        0        0      642 2020-02-02 00:00:00.000000 hapi_schema-0.8.9/tests/test_dataset.py
+-rw-r--r--   0        0        0     2514 2020-02-02 00:00:00.000000 hapi_schema-0.8.9/tests/test_food_price.py
+-rw-r--r--   0        0        0     2075 2020-02-02 00:00:00.000000 hapi_schema-0.8.9/tests/test_food_security.py
+-rw-r--r--   0        0        0     3942 2020-02-02 00:00:00.000000 hapi_schema-0.8.9/tests/test_funding.py
+-rw-r--r--   0        0        0     3963 2020-02-02 00:00:00.000000 hapi_schema-0.8.9/tests/test_humanitarian_needs.py
+-rw-r--r--   0        0        0     1938 2020-02-02 00:00:00.000000 hapi_schema-0.8.9/tests/test_location.py
+-rw-r--r--   0        0        0     5310 2020-02-02 00:00:00.000000 hapi_schema-0.8.9/tests/test_national_risk.py
+-rw-r--r--   0        0        0     1762 2020-02-02 00:00:00.000000 hapi_schema-0.8.9/tests/test_operational_presence.py
+-rw-r--r--   0        0        0      416 2020-02-02 00:00:00.000000 hapi_schema-0.8.9/tests/test_org.py
+-rw-r--r--   0        0        0      478 2020-02-02 00:00:00.000000 hapi_schema-0.8.9/tests/test_org_type.py
+-rw-r--r--   0        0        0     1384 2020-02-02 00:00:00.000000 hapi_schema-0.8.9/tests/test_patch.py
+-rw-r--r--   0        0        0     3296 2020-02-02 00:00:00.000000 hapi_schema-0.8.9/tests/test_population.py
+-rw-r--r--   0        0        0     3266 2020-02-02 00:00:00.000000 hapi_schema-0.8.9/tests/test_poverty_rate.py
+-rw-r--r--   0        0        0     3529 2020-02-02 00:00:00.000000 hapi_schema-0.8.9/tests/test_refugees.py
+-rw-r--r--   0        0        0      481 2020-02-02 00:00:00.000000 hapi_schema-0.8.9/tests/test_resource.py
+-rw-r--r--   0        0        0      437 2020-02-02 00:00:00.000000 hapi_schema-0.8.9/tests/test_sector.py
+-rw-r--r--   0        0        0    15338 2020-02-02 00:00:00.000000 hapi_schema-0.8.9/tests/test_views_as_tables.py
+-rw-r--r--   0        0        0      571 2020-02-02 00:00:00.000000 hapi_schema-0.8.9/tests/test_wfp_commodity.py
+-rw-r--r--   0        0        0     1567 2020-02-02 00:00:00.000000 hapi_schema-0.8.9/tests/test_wfp_market.py
+-rw-r--r--   0        0        0        0 2020-02-02 00:00:00.000000 hapi_schema-0.8.9/tests/sample_data/__init__.py
+-rw-r--r--   0        0        0      411 2020-02-02 00:00:00.000000 hapi_schema-0.8.9/tests/sample_data/data_admin1.py
+-rw-r--r--   0        0        0      831 2020-02-02 00:00:00.000000 hapi_schema-0.8.9/tests/sample_data/data_admin2.py
+-rw-r--r--   0        0        0      636 2020-02-02 00:00:00.000000 hapi_schema-0.8.9/tests/sample_data/data_conflict_event.py
+-rw-r--r--   0        0        0      153 2020-02-02 00:00:00.000000 hapi_schema-0.8.9/tests/sample_data/data_currency.py
+-rw-r--r--   0        0        0      441 2020-02-02 00:00:00.000000 hapi_schema-0.8.9/tests/sample_data/data_dataset.py
+-rw-r--r--   0        0        0      851 2020-02-02 00:00:00.000000 hapi_schema-0.8.9/tests/sample_data/data_food_price.py
+-rw-r--r--   0        0        0     1195 2020-02-02 00:00:00.000000 hapi_schema-0.8.9/tests/sample_data/data_food_security.py
+-rw-r--r--   0        0        0      448 2020-02-02 00:00:00.000000 hapi_schema-0.8.9/tests/sample_data/data_funding.py
+-rw-r--r--   0        0        0     1903 2020-02-02 00:00:00.000000 hapi_schema-0.8.9/tests/sample_data/data_humanitarian_needs.py
+-rw-r--r--   0        0        0      376 2020-02-02 00:00:00.000000 hapi_schema-0.8.9/tests/sample_data/data_location.py
+-rw-r--r--   0        0        0      519 2020-02-02 00:00:00.000000 hapi_schema-0.8.9/tests/sample_data/data_national_risk.py
+-rw-r--r--   0        0        0     1333 2020-02-02 00:00:00.000000 hapi_schema-0.8.9/tests/sample_data/data_operational_presence.py
+-rw-r--r--   0        0        0      292 2020-02-02 00:00:00.000000 hapi_schema-0.8.9/tests/sample_data/data_org.py
+-rw-r--r--   0        0        0      170 2020-02-02 00:00:00.000000 hapi_schema-0.8.9/tests/sample_data/data_org_type.py
+-rw-r--r--   0        0        0     1641 2020-02-02 00:00:00.000000 hapi_schema-0.8.9/tests/sample_data/data_patch.py
+-rw-r--r--   0        0        0     1329 2020-02-02 00:00:00.000000 hapi_schema-0.8.9/tests/sample_data/data_population.py
+-rw-r--r--   0        0        0      488 2020-02-02 00:00:00.000000 hapi_schema-0.8.9/tests/sample_data/data_poverty_rate.py
+-rw-r--r--   0        0        0      861 2020-02-02 00:00:00.000000 hapi_schema-0.8.9/tests/sample_data/data_refugees.py
+-rw-r--r--   0        0        0     1510 2020-02-02 00:00:00.000000 hapi_schema-0.8.9/tests/sample_data/data_resource.py
+-rw-r--r--   0        0        0      379 2020-02-02 00:00:00.000000 hapi_schema-0.8.9/tests/sample_data/data_sector.py
+-rw-r--r--   0        0        0      238 2020-02-02 00:00:00.000000 hapi_schema-0.8.9/tests/sample_data/data_wfp_commodity.py
+-rw-r--r--   0        0        0      197 2020-02-02 00:00:00.000000 hapi_schema-0.8.9/tests/sample_data/data_wfp_market.py
+-rw-r--r--   0        0        0     3164 2020-02-02 00:00:00.000000 hapi_schema-0.8.9/.gitignore
+-rw-r--r--   0        0        0     1099 2020-02-02 00:00:00.000000 hapi_schema-0.8.9/LICENSE
+-rw-r--r--   0        0        0       64 2020-02-02 00:00:00.000000 hapi_schema-0.8.9/README.md
+-rw-r--r--   0        0        0     2479 2020-02-02 00:00:00.000000 hapi_schema-0.8.9/pyproject.toml
+-rw-r--r--   0        0        0     1582 2020-02-02 00:00:00.000000 hapi_schema-0.8.9/PKG-INFO
```

### Comparing `hapi_schema-0.8.8/changelog.md` & `hapi_schema-0.8.9/changelog.md`

 * *Files 2% similar despite different names*

```diff
@@ -1,52 +1,62 @@
 # Changelog
 
 All notable changes to this project will be documented in this file.
 
 The format is based on [Keep a Changelog](https://keepachangelog.com/en/1.0.0/),
 and this project adheres to [Semantic Versioning](https://semver.org/spec/v2.0.0.html).
 
+## 0.8.9
+
+### Fixed
+
+- Some enums missing built from values
+
 ## 0.8.8
 
-### Changes
+### Changed
 
 - Rewrite enums to use values rather than variable names
 - Switch from "*" to "all" for rollup in enums
 - Add "intersectoral" to sample sector data (distinct from "all")
 - Ensure that constraint names end consistently with "\_constraint"
 
 ## 0.8.7
 
-## Changes
+### Changed
+
 - Add unit to food\_price table primary key
 
 ## 0.8.6
 
-## Changes
+### Changed
+
 - Added food\_price view as tables by updating the toml parameter file
 - Updated poverty\_rate view as table
 - Updated operational\_presence view as table by updating the toml parameter file
 - Made a few adhoc changes to the view as table generator code to accommodate Decimal columns
 
 ## 0.8.5
 
-## Changes
+### Changed
+
 - refactor DBPovertyRate to wide instead of narrow
 - added org\_type\_description to operational\_presence\_view
 
 ## Removed
+
 - rate\_constraint and `PovertyClassification` enum
 
 ## 0.8.4
 
 ### Added
 
 - New constraints: rate\_constraint
 
-### CHanged
+### Changed
 
 - refactor DBPovertyRate to track rates rather than population, and link to
   location (with admin1\_name as a text field)
 
 ## 0.8.3
 
 ### Changed
@@ -56,48 +66,48 @@
 - change FLOAT to DECIMAL in funding, national\_risk, and food\_security
 
 ## 0.8.2
 
 Miscellaneous fixes for pipelines
 
 ### Changed
-- added from\_cods column to location, admin1, and admin2
 
+- added from\_cods column to location, admin1, and admin2
 
 ## 0.8.1
 
 Implemented the Food Prices subcategory.
 
 ### Added
+
 - New tables and views: food\_price, wfp\_commodity, wfp\_market, currency
 - New enums: PriceFlag, PriceType, CommodityCategory
 - New constraints: non\_negative\_constraint, latlon\_constraint
 
-
 ## 0.8.0
 
 ### Changed
 
 - Many small changes to align with V1 of the schema
 - `resource` and `dataset` primary keys are now the UUID
 - Use postgres instead of sqlite for testing
 - Update GitHub Actions workflow to use postgres
 - Created tables which reflect the views
 - Programmatically obtain views
 
 ### Added
+
 - New tables: humanitarian\_needs, funding, refugees, conflict\_event, poverty\_rate
 - New enums: Gender, DisabledMarker, EventType, PopulationGroup, PopulationStatus, IPCPhase, PovertyClassification, IPCType, and RiskClass
 - Generalized constraints
 
 ### Removed
 
 - ipc\_phase, ipc\_type, age\_range, and gender tables
 
-
 ## [0.7.3]
 
 ### Fixed
 
 - Incorrect constraint quotes in IPC type
 - Clashing unique constraint names in admins
```

### Comparing `hapi_schema-0.8.8/contributing.md` & `hapi_schema-0.8.9/contributing.md`

 * *Files identical despite different names*

### Comparing `hapi_schema-0.8.8/requirements.txt` & `hapi_schema-0.8.9/requirements.txt`

 * *Files identical despite different names*

### Comparing `hapi_schema-0.8.8/.config/pre-commit-config.yaml` & `hapi_schema-0.8.9/.config/pre-commit-config.yaml`

 * *Files identical despite different names*

### Comparing `hapi_schema-0.8.8/.github/workflows/publish.yaml` & `hapi_schema-0.8.9/.github/workflows/publish.yaml`

 * *Files identical despite different names*

### Comparing `hapi_schema-0.8.8/.github/workflows/run-python-tests.yaml` & `hapi_schema-0.8.9/.github/workflows/run-python-tests.yaml`

 * *Files identical despite different names*

### Comparing `hapi_schema-0.8.8/src/hapi_schema/db_admin1.py` & `hapi_schema-0.8.9/src/hapi_schema/db_admin1.py`

 * *Files identical despite different names*

### Comparing `hapi_schema-0.8.8/src/hapi_schema/db_admin2.py` & `hapi_schema-0.8.9/src/hapi_schema/db_admin2.py`

 * *Files identical despite different names*

### Comparing `hapi_schema-0.8.8/src/hapi_schema/db_conflict_event.py` & `hapi_schema-0.8.9/src/hapi_schema/db_conflict_event.py`

 * *Files identical despite different names*

### Comparing `hapi_schema-0.8.8/src/hapi_schema/db_currency.py` & `hapi_schema-0.8.9/src/hapi_schema/db_currency.py`

 * *Files identical despite different names*

### Comparing `hapi_schema-0.8.8/src/hapi_schema/db_dataset.py` & `hapi_schema-0.8.9/src/hapi_schema/db_dataset.py`

 * *Files identical despite different names*

### Comparing `hapi_schema-0.8.8/src/hapi_schema/db_food_price.py` & `hapi_schema-0.8.9/src/hapi_schema/db_food_price.py`

 * *Files 6% similar despite different names*

```diff
@@ -1,15 +1,14 @@
 """FoodPrice table and view."""
 
 from datetime import datetime
 from decimal import Decimal
 
 from sqlalchemy import (
     DateTime,
-    Enum,
     ForeignKey,
     String,
     select,
 )
 from sqlalchemy.orm import Mapped, mapped_column, relationship
 
 from hapi_schema.db_admin2 import DBAdmin1, DBAdmin2, DBLocation
@@ -18,15 +17,19 @@
 from hapi_schema.db_wfp_commodity import DBWFPCommodity
 from hapi_schema.db_wfp_market import DBWFPMarket
 from hapi_schema.utils.base import Base
 from hapi_schema.utils.constraints import (
     non_negative_constraint,
     reference_period_constraint,
 )
-from hapi_schema.utils.enums import PriceFlag, PriceType
+from hapi_schema.utils.enums import (
+    PriceFlag,
+    PriceType,
+    build_enum_using_values,
+)
 from hapi_schema.utils.view_params import ViewParams
 
 # normalised table
 
 
 class DBFoodPrice(Base):
     __tablename__ = "food_price"
@@ -48,18 +51,18 @@
     currency_code: Mapped[str] = mapped_column(
         ForeignKey("currency.code", onupdate="CASCADE"),
         nullable=False,
         index=True,
     )
     unit: Mapped[str] = mapped_column(String(32), primary_key=True)
     price_flag: Mapped[PriceFlag] = mapped_column(
-        Enum(PriceFlag), primary_key=True
+        build_enum_using_values(PriceFlag), primary_key=True
     )
     price_type: Mapped[PriceType] = mapped_column(
-        Enum(PriceType), primary_key=True
+        build_enum_using_values(PriceType), primary_key=True
     )
     price: Mapped[Decimal] = mapped_column(nullable=False)
     reference_period_start: Mapped[datetime] = mapped_column(
         DateTime, primary_key=True
     )
     reference_period_end: Mapped[datetime] = mapped_column(
         DateTime, nullable=False, index=True
```

### Comparing `hapi_schema-0.8.8/src/hapi_schema/db_food_security.py` & `hapi_schema-0.8.9/src/hapi_schema/db_food_security.py`

 * *Files 6% similar despite different names*

```diff
@@ -1,15 +1,14 @@
 """Food security table and view."""
 
 from datetime import datetime
 from decimal import Decimal
 
 from sqlalchemy import (
     DateTime,
-    Enum,
     Float,
     ForeignKey,
     Integer,
     select,
 )
 from sqlalchemy.orm import Mapped, mapped_column, relationship
 
@@ -18,15 +17,15 @@
 from hapi_schema.db_location import DBLocation
 from hapi_schema.db_resource import DBResource
 from hapi_schema.utils.base import Base
 from hapi_schema.utils.constraints import (
     population_constraint,
     reference_period_constraint,
 )
-from hapi_schema.utils.enums import IPCPhase, IPCType
+from hapi_schema.utils.enums import IPCPhase, IPCType, build_enum_using_values
 from hapi_schema.utils.view_params import ViewParams
 
 
 class DBFoodSecurity(Base):
     __tablename__ = "food_security"
     __table_args__ = (
         reference_period_constraint(),
@@ -37,17 +36,19 @@
         ForeignKey("resource.hdx_id", onupdate="CASCADE", ondelete="CASCADE"),
         nullable=False,
     )
     admin2_ref: Mapped[int] = mapped_column(
         ForeignKey("admin2.id", onupdate="CASCADE"), primary_key=True
     )
     ipc_phase: Mapped[IPCPhase] = mapped_column(
-        Enum(IPCPhase), primary_key=True
+        build_enum_using_values(IPCPhase), primary_key=True
+    )
+    ipc_type: Mapped[IPCType] = mapped_column(
+        build_enum_using_values(IPCType), primary_key=True
     )
-    ipc_type: Mapped[IPCType] = mapped_column(Enum(IPCType), primary_key=True)
     population_in_phase: Mapped[int] = mapped_column(
         Integer, nullable=False, index=True
     )
     population_fraction_in_phase: Mapped[Decimal] = mapped_column(
         Float, nullable=False, index=True
     )
     reference_period_start: Mapped[datetime] = mapped_column(
```

### Comparing `hapi_schema-0.8.8/src/hapi_schema/db_funding.py` & `hapi_schema-0.8.9/src/hapi_schema/db_funding.py`

 * *Files identical despite different names*

### Comparing `hapi_schema-0.8.8/src/hapi_schema/db_humanitarian_needs.py` & `hapi_schema-0.8.9/src/hapi_schema/db_humanitarian_needs.py`

 * *Files 5% similar despite different names*

```diff
@@ -1,14 +1,13 @@
 """HumanitarianNeeds table and view."""
 
 from datetime import datetime
 
 from sqlalchemy import (
     DateTime,
-    Enum,
     ForeignKey,
     Integer,
     String,
     select,
 )
 from sqlalchemy.orm import Mapped, mapped_column, relationship
 
@@ -24,14 +23,15 @@
     reference_period_constraint,
 )
 from hapi_schema.utils.enums import (
     DisabledMarker,
     Gender,
     PopulationGroup,
     PopulationStatus,
+    build_enum_using_values,
 )
 from hapi_schema.utils.view_params import ViewParams
 
 
 class DBHumanitarianNeeds(Base):
     __tablename__ = "humanitarian_needs"
     __table_args__ = (
@@ -45,34 +45,36 @@
         ForeignKey("resource.hdx_id", onupdate="CASCADE", ondelete="CASCADE"),
         nullable=False,
     )
     admin2_ref: Mapped[int] = mapped_column(
         ForeignKey("admin2.id", onupdate="CASCADE"),
         primary_key=True,
     )
-    gender: Mapped[Gender] = mapped_column(Enum(Gender), primary_key=True)
+    gender: Mapped[Gender] = mapped_column(
+        build_enum_using_values(Gender), primary_key=True
+    )
     age_range: Mapped[str] = mapped_column(String(32), primary_key=True)
     min_age: Mapped[int] = mapped_column(Integer, nullable=True, index=True)
     max_age: Mapped[int] = mapped_column(Integer, nullable=True, index=True)
     sector_code: Mapped[str] = mapped_column(
         ForeignKey("sector.code", onupdate="CASCADE"),
         primary_key=True,
     )
     population_group: Mapped[PopulationGroup] = mapped_column(
-        Enum(PopulationGroup),
+        build_enum_using_values(PopulationGroup),
         primary_key=True,
     )
 
     population_status: Mapped[PopulationStatus] = mapped_column(
-        Enum(PopulationStatus),
+        build_enum_using_values(PopulationStatus),
         primary_key=True,
     )
 
     disabled_marker: Mapped[DisabledMarker] = mapped_column(
-        Enum(DisabledMarker), primary_key=True
+        build_enum_using_values(DisabledMarker), primary_key=True
     )
     population: Mapped[int] = mapped_column(Integer, nullable=False)
     reference_period_start: Mapped[datetime] = mapped_column(
         DateTime,
         primary_key=True,
     )
     reference_period_end: Mapped[datetime] = mapped_column(
```

### Comparing `hapi_schema-0.8.8/src/hapi_schema/db_location.py` & `hapi_schema-0.8.9/src/hapi_schema/db_location.py`

 * *Files identical despite different names*

### Comparing `hapi_schema-0.8.8/src/hapi_schema/db_national_risk.py` & `hapi_schema-0.8.9/src/hapi_schema/db_national_risk.py`

 * *Files 2% similar despite different names*

```diff
@@ -2,29 +2,28 @@
 
 from datetime import datetime
 from decimal import Decimal
 
 from sqlalchemy import (
     CheckConstraint,
     DateTime,
-    Enum,
     Float,
     ForeignKey,
     Integer,
     select,
 )
 from sqlalchemy.orm import Mapped, mapped_column, relationship
 
 from hapi_schema.db_location import DBLocation
 from hapi_schema.utils.base import Base
 from hapi_schema.utils.constraints import (
     general_risk_constraint,
     reference_period_constraint,
 )
-from hapi_schema.utils.enums import RiskClass
+from hapi_schema.utils.enums import RiskClass, build_enum_using_values
 from hapi_schema.utils.view_params import ViewParams
 
 
 class DBNationalRisk(Base):
     __tablename__ = "national_risk"
     __table_args__ = (
         general_risk_constraint("overall"),
@@ -50,15 +49,15 @@
         ForeignKey("resource.hdx_id", onupdate="CASCADE", ondelete="CASCADE"),
         nullable=False,
     )
     location_ref: Mapped[int] = mapped_column(
         ForeignKey("location.id", onupdate="CASCADE"), primary_key=True
     )
     risk_class: Mapped[RiskClass] = mapped_column(
-        Enum(RiskClass), nullable=False
+        build_enum_using_values(RiskClass), nullable=False
     )
     global_rank: Mapped[int] = mapped_column(Integer, nullable=False)
     overall_risk: Mapped[Decimal] = mapped_column(Float, nullable=False)
     hazard_exposure_risk: Mapped[Decimal] = mapped_column(
         Float, nullable=False
     )
     vulnerability_risk: Mapped[Decimal] = mapped_column(Float, nullable=False)
```

### Comparing `hapi_schema-0.8.8/src/hapi_schema/db_operational_presence.py` & `hapi_schema-0.8.9/src/hapi_schema/db_operational_presence.py`

 * *Files identical despite different names*

### Comparing `hapi_schema-0.8.8/src/hapi_schema/db_org.py` & `hapi_schema-0.8.9/src/hapi_schema/db_org.py`

 * *Files identical despite different names*

### Comparing `hapi_schema-0.8.8/src/hapi_schema/db_org_type.py` & `hapi_schema-0.8.9/src/hapi_schema/db_org_type.py`

 * *Files identical despite different names*

### Comparing `hapi_schema-0.8.8/src/hapi_schema/db_patch.py` & `hapi_schema-0.8.9/src/hapi_schema/db_patch.py`

 * *Files identical despite different names*

### Comparing `hapi_schema-0.8.8/src/hapi_schema/db_population.py` & `hapi_schema-0.8.9/src/hapi_schema/db_population.py`

 * *Files 11% similar despite different names*

```diff
@@ -1,14 +1,13 @@
 """Population table and view."""
 
 from datetime import datetime
 
 from sqlalchemy import (
     DateTime,
-    Enum,
     ForeignKey,
     Integer,
     String,
     select,
 )
 from sqlalchemy.orm import Mapped, mapped_column, relationship
 
@@ -18,15 +17,15 @@
 from hapi_schema.utils.base import Base
 from hapi_schema.utils.constraints import (
     max_age_constraint,
     min_age_constraint,
     population_constraint,
     reference_period_constraint,
 )
-from hapi_schema.utils.enums import Gender
+from hapi_schema.utils.enums import Gender, build_enum_using_values
 from hapi_schema.utils.view_params import ViewParams
 
 
 class DBPopulation(Base):
     __tablename__ = "population"
     __table_args__ = (
         min_age_constraint(),
@@ -39,15 +38,17 @@
         ForeignKey("resource.hdx_id", onupdate="CASCADE", ondelete="CASCADE"),
         nullable=False,
     )
     admin2_ref: Mapped[int] = mapped_column(
         ForeignKey("admin2.id", onupdate="CASCADE"),
         primary_key=True,
     )
-    gender: Mapped[Gender] = mapped_column(Enum(Gender), primary_key=True)
+    gender: Mapped[Gender] = mapped_column(
+        build_enum_using_values(Gender), primary_key=True
+    )
     age_range: Mapped[str] = mapped_column(String(32), primary_key=True)
     min_age: Mapped[int] = mapped_column(Integer, nullable=True, index=True)
     max_age: Mapped[int] = mapped_column(Integer, nullable=True, index=True)
     population: Mapped[int] = mapped_column(
         Integer, nullable=False, index=True
     )
     reference_period_start: Mapped[datetime] = mapped_column(
```

### Comparing `hapi_schema-0.8.8/src/hapi_schema/db_poverty_rate.py` & `hapi_schema-0.8.9/src/hapi_schema/db_poverty_rate.py`

 * *Files identical despite different names*

### Comparing `hapi_schema-0.8.8/src/hapi_schema/db_refugees.py` & `hapi_schema-0.8.9/src/hapi_schema/db_refugees.py`

 * *Files 3% similar despite different names*

```diff
@@ -3,15 +3,14 @@
 # Note: this one is a bit tricky, because the view has to join with
 # the location table twice
 
 from datetime import datetime
 
 from sqlalchemy import (
     DateTime,
-    Enum,
     ForeignKey,
     Integer,
     String,
     select,
 )
 from sqlalchemy.orm import Mapped, aliased, mapped_column, relationship
 
@@ -19,15 +18,19 @@
 from hapi_schema.utils.base import Base
 from hapi_schema.utils.constraints import (
     max_age_constraint,
     min_age_constraint,
     population_constraint,
     reference_period_constraint,
 )
-from hapi_schema.utils.enums import Gender, PopulationGroup
+from hapi_schema.utils.enums import (
+    Gender,
+    PopulationGroup,
+    build_enum_using_values,
+)
 from hapi_schema.utils.view_params import ViewParams
 
 
 class DBRefugees(Base):
     __tablename__ = "refugees"
     __table_args__ = (
         min_age_constraint(),
@@ -44,17 +47,19 @@
         ForeignKey("location.id", onupdate="CASCADE"), primary_key=True
     )
     asylum_location_ref: Mapped[int] = mapped_column(
         ForeignKey("location.id", onupdate="CASCADE"), primary_key=True
     )
     # population_group is broader than we need, but it will do
     population_group: Mapped[PopulationGroup] = mapped_column(
-        Enum(PopulationGroup), primary_key=True
+        build_enum_using_values(PopulationGroup), primary_key=True
+    )
+    gender: Mapped[Gender] = mapped_column(
+        build_enum_using_values(Gender), primary_key=True
     )
-    gender: Mapped[Gender] = mapped_column(Enum(Gender), primary_key=True)
     age_range: Mapped[str] = mapped_column(String(32), primary_key=True)
     min_age: Mapped[int] = mapped_column(Integer, nullable=True, index=True)
     max_age: Mapped[int] = mapped_column(Integer, nullable=True, index=True)
     population: Mapped[int] = mapped_column(
         Integer, nullable=False, index=True
     )
     reference_period_start: Mapped[datetime] = mapped_column(
```

### Comparing `hapi_schema-0.8.8/src/hapi_schema/db_resource.py` & `hapi_schema-0.8.9/src/hapi_schema/db_resource.py`

 * *Files identical despite different names*

### Comparing `hapi_schema-0.8.8/src/hapi_schema/db_sector.py` & `hapi_schema-0.8.9/src/hapi_schema/db_sector.py`

 * *Files identical despite different names*

### Comparing `hapi_schema-0.8.8/src/hapi_schema/db_views_as_tables.py` & `hapi_schema-0.8.9/src/hapi_schema/db_views_as_tables.py`

 * *Files identical despite different names*

### Comparing `hapi_schema-0.8.8/src/hapi_schema/db_wfp_commodity.py` & `hapi_schema-0.8.9/src/hapi_schema/db_wfp_commodity.py`

 * *Files 25% similar despite different names*

```diff
@@ -1,23 +1,23 @@
 """wfp_commodity table and view."""
 
-from sqlalchemy import Enum, String, select
+from sqlalchemy import String, select
 from sqlalchemy.orm import Mapped, mapped_column
 
 from hapi_schema.utils.base import Base
-from hapi_schema.utils.enums import CommodityCategory
+from hapi_schema.utils.enums import CommodityCategory, build_enum_using_values
 from hapi_schema.utils.view_params import ViewParams
 
 
 class DBWFPCommodity(Base):
     __tablename__ = "wfp_commodity"
 
     code: Mapped[str] = mapped_column(String(32), primary_key=True)
     category: Mapped[CommodityCategory] = mapped_column(
-        Enum(CommodityCategory), index=True
+        build_enum_using_values(CommodityCategory), index=True
     )
     name: Mapped[str] = mapped_column(String(512), nullable=False, index=True)
 
 
 view_params_wfp_commodity = ViewParams(
     name="wfp_commodity_view",
     metadata=Base.metadata,
```

### Comparing `hapi_schema-0.8.8/src/hapi_schema/db_wfp_market.py` & `hapi_schema-0.8.9/src/hapi_schema/db_wfp_market.py`

 * *Files identical despite different names*

### Comparing `hapi_schema-0.8.8/src/hapi_schema/views.py` & `hapi_schema-0.8.9/src/hapi_schema/views.py`

 * *Files identical despite different names*

### Comparing `hapi_schema-0.8.8/src/hapi_schema/utils/constraints.py` & `hapi_schema-0.8.9/src/hapi_schema/utils/constraints.py`

 * *Files identical despite different names*

### Comparing `hapi_schema-0.8.8/src/hapi_schema/utils/enums.py` & `hapi_schema-0.8.9/src/hapi_schema/utils/enums.py`

 * *Files 8% similar despite different names*

```diff
@@ -1,20 +1,20 @@
 from enum import Enum as PythonEnum
-from typing import List
+from typing import List, Type
 
 from sqlalchemy import Enum as SQLAlchemyEnum
 
 """The two functions below create enums using the values rather than the keys"""
 
 
-def _get_list_of_values(enum_class: PythonEnum) -> List[str]:
+def _get_list_of_values(enum_class: Type[PythonEnum]) -> List[str]:
     return [e.value for e in enum_class]
 
 
-def build_enum_using_values(enum_class: PythonEnum) -> SQLAlchemyEnum:
+def build_enum_using_values(enum_class: Type[PythonEnum]) -> SQLAlchemyEnum:
     return SQLAlchemyEnum(enum_class, values_callable=_get_list_of_values)
 
 
 class Gender(str, PythonEnum):
     FEMALE = "f"
     MALE = "m"
     NONBINARY = "x"
```

### Comparing `hapi_schema-0.8.8/src/hapi_schema/utils/hapi_views_code_generator.py` & `hapi_schema-0.8.9/src/hapi_schema/utils/hapi_views_code_generator.py`

 * *Files identical despite different names*

### Comparing `hapi_schema-0.8.8/src/hapi_schema/utils/view_as_table_code_generator.py` & `hapi_schema-0.8.9/src/hapi_schema/utils/view_as_table_code_generator.py`

 * *Files identical despite different names*

### Comparing `hapi_schema-0.8.8/src/hapi_schema/utils/view_as_table_definitions.toml` & `hapi_schema-0.8.9/src/hapi_schema/utils/view_as_table_definitions.toml`

 * *Files identical despite different names*

### Comparing `hapi_schema-0.8.8/tests/conftest.py` & `hapi_schema-0.8.9/tests/conftest.py`

 * *Files identical despite different names*

### Comparing `hapi_schema-0.8.8/tests/test_admin1.py` & `hapi_schema-0.8.9/tests/test_admin1.py`

 * *Files identical despite different names*

### Comparing `hapi_schema-0.8.8/tests/test_admin2.py` & `hapi_schema-0.8.9/tests/test_admin2.py`

 * *Files identical despite different names*

### Comparing `hapi_schema-0.8.8/tests/test_conflict_event.py` & `hapi_schema-0.8.9/tests/test_conflict_event.py`

 * *Files identical despite different names*

### Comparing `hapi_schema-0.8.8/tests/test_dataset.py` & `hapi_schema-0.8.9/tests/test_dataset.py`

 * *Files identical despite different names*

### Comparing `hapi_schema-0.8.8/tests/test_food_price.py` & `hapi_schema-0.8.9/tests/test_food_price.py`

 * *Files identical despite different names*

### Comparing `hapi_schema-0.8.8/tests/test_food_security.py` & `hapi_schema-0.8.9/tests/test_food_security.py`

 * *Files identical despite different names*

### Comparing `hapi_schema-0.8.8/tests/test_funding.py` & `hapi_schema-0.8.9/tests/test_funding.py`

 * *Files identical despite different names*

### Comparing `hapi_schema-0.8.8/tests/test_humanitarian_needs.py` & `hapi_schema-0.8.9/tests/test_humanitarian_needs.py`

 * *Files identical despite different names*

### Comparing `hapi_schema-0.8.8/tests/test_location.py` & `hapi_schema-0.8.9/tests/test_location.py`

 * *Files identical despite different names*

### Comparing `hapi_schema-0.8.8/tests/test_national_risk.py` & `hapi_schema-0.8.9/tests/test_national_risk.py`

 * *Files identical despite different names*

### Comparing `hapi_schema-0.8.8/tests/test_operational_presence.py` & `hapi_schema-0.8.9/tests/test_operational_presence.py`

 * *Files identical despite different names*

### Comparing `hapi_schema-0.8.8/tests/test_patch.py` & `hapi_schema-0.8.9/tests/test_patch.py`

 * *Files identical despite different names*

### Comparing `hapi_schema-0.8.8/tests/test_population.py` & `hapi_schema-0.8.9/tests/test_population.py`

 * *Files identical despite different names*

### Comparing `hapi_schema-0.8.8/tests/test_poverty_rate.py` & `hapi_schema-0.8.9/tests/test_poverty_rate.py`

 * *Files identical despite different names*

### Comparing `hapi_schema-0.8.8/tests/test_refugees.py` & `hapi_schema-0.8.9/tests/test_refugees.py`

 * *Files identical despite different names*

### Comparing `hapi_schema-0.8.8/tests/test_views_as_tables.py` & `hapi_schema-0.8.9/tests/test_views_as_tables.py`

 * *Files identical despite different names*

### Comparing `hapi_schema-0.8.8/tests/test_wfp_commodity.py` & `hapi_schema-0.8.9/tests/test_wfp_commodity.py`

 * *Files identical despite different names*

### Comparing `hapi_schema-0.8.8/tests/test_wfp_market.py` & `hapi_schema-0.8.9/tests/test_wfp_market.py`

 * *Files identical despite different names*

### Comparing `hapi_schema-0.8.8/tests/sample_data/data_admin2.py` & `hapi_schema-0.8.9/tests/sample_data/data_admin2.py`

 * *Files identical despite different names*

### Comparing `hapi_schema-0.8.8/tests/sample_data/data_conflict_event.py` & `hapi_schema-0.8.9/tests/sample_data/data_conflict_event.py`

 * *Files identical despite different names*

### Comparing `hapi_schema-0.8.8/tests/sample_data/data_food_price.py` & `hapi_schema-0.8.9/tests/sample_data/data_food_price.py`

 * *Files identical despite different names*

### Comparing `hapi_schema-0.8.8/tests/sample_data/data_food_security.py` & `hapi_schema-0.8.9/tests/sample_data/data_food_security.py`

 * *Files identical despite different names*

### Comparing `hapi_schema-0.8.8/tests/sample_data/data_humanitarian_needs.py` & `hapi_schema-0.8.9/tests/sample_data/data_humanitarian_needs.py`

 * *Files identical despite different names*

### Comparing `hapi_schema-0.8.8/tests/sample_data/data_national_risk.py` & `hapi_schema-0.8.9/tests/sample_data/data_national_risk.py`

 * *Files identical despite different names*

### Comparing `hapi_schema-0.8.8/tests/sample_data/data_operational_presence.py` & `hapi_schema-0.8.9/tests/sample_data/data_operational_presence.py`

 * *Files identical despite different names*

### Comparing `hapi_schema-0.8.8/tests/sample_data/data_patch.py` & `hapi_schema-0.8.9/tests/sample_data/data_patch.py`

 * *Files identical despite different names*

### Comparing `hapi_schema-0.8.8/tests/sample_data/data_population.py` & `hapi_schema-0.8.9/tests/sample_data/data_population.py`

 * *Files identical despite different names*

### Comparing `hapi_schema-0.8.8/tests/sample_data/data_refugees.py` & `hapi_schema-0.8.9/tests/sample_data/data_refugees.py`

 * *Files identical despite different names*

### Comparing `hapi_schema-0.8.8/tests/sample_data/data_resource.py` & `hapi_schema-0.8.9/tests/sample_data/data_resource.py`

 * *Files identical despite different names*

### Comparing `hapi_schema-0.8.8/.gitignore` & `hapi_schema-0.8.9/.gitignore`

 * *Files identical despite different names*

### Comparing `hapi_schema-0.8.8/LICENSE` & `hapi_schema-0.8.9/LICENSE`

 * *Files identical despite different names*

### Comparing `hapi_schema-0.8.8/pyproject.toml` & `hapi_schema-0.8.9/pyproject.toml`

 * *Files identical despite different names*

### Comparing `hapi_schema-0.8.8/PKG-INFO` & `hapi_schema-0.8.9/PKG-INFO`

 * *Files 0% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.3
 Name: hapi-schema
-Version: 0.8.8
+Version: 0.8.9
 Summary: HAPI database schema specified in SQLAlchemy
 Project-URL: Homepage, https://github.com/OCHA-DAP/hapi-schemas
 Author-email: Simon Johnson <simon.johnson@un.org>
 License: MIT
 License-File: LICENSE
 Keywords: HDX,hapi,schema
 Classifier: Intended Audience :: Developers
```

