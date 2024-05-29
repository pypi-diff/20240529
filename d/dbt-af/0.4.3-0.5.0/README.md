# Comparing `tmp/dbt_af-0.4.3.tar.gz` & `tmp/dbt_af-0.5.0.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "dbt_af-0.4.3.tar", max compression
+gzip compressed data, was "dbt_af-0.5.0.tar", max compression
```

## Comparing `dbt_af-0.4.3.tar` & `dbt_af-0.5.0.tar`

### file list

```diff
@@ -1,47 +1,52 @@
--rw-r--r--   0        0        0      193 2024-05-16 14:49:41.064149 dbt_af-0.4.3/AUTHORS
--rw-r--r--   0        0        0      580 2024-05-16 14:49:41.064149 dbt_af-0.4.3/LICENSE
--rw-r--r--   0        0        0     3551 2024-05-16 14:49:41.064149 dbt_af-0.4.3/README.md
--rw-r--r--   0        0        0       95 2024-05-16 14:49:41.064149 dbt_af-0.4.3/dbt_af/__init__.py
--rw-r--r--   0        0        0      809 2024-05-16 14:49:41.064149 dbt_af-0.4.3/dbt_af/builder/__init__.py
--rw-r--r--   0        0        0     1076 2024-05-16 14:49:41.064149 dbt_af-0.4.3/dbt_af/builder/backfill_dag_components.py
--rw-r--r--   0        0        0    15978 2024-05-16 14:49:41.064149 dbt_af-0.4.3/dbt_af/builder/dag_components.py
--rw-r--r--   0        0        0    10831 2024-05-16 14:49:41.064149 dbt_af-0.4.3/dbt_af/builder/dbt_af_builder.py
--rw-r--r--   0        0        0     2695 2024-05-16 14:49:41.064149 dbt_af-0.4.3/dbt_af/builder/dbt_model_path_graph_builder.py
--rw-r--r--   0        0        0     5878 2024-05-16 14:49:41.064149 dbt_af-0.4.3/dbt_af/builder/domain_dag.py
--rw-r--r--   0        0        0     1507 2024-05-16 14:49:41.064149 dbt_af-0.4.3/dbt_af/builder/maintenance_dag_components.py
--rw-r--r--   0        0        0     4504 2024-05-16 14:49:41.064149 dbt_af-0.4.3/dbt_af/builder/task_dependencies.py
--rw-r--r--   0        0        0        0 2024-05-16 14:49:41.064149 dbt_af-0.4.3/dbt_af/common/__init__.py
--rw-r--r--   0        0        0      552 2024-05-16 14:49:41.064149 dbt_af-0.4.3/dbt_af/common/constants.py
--rw-r--r--   0        0        0     7473 2024-05-16 14:49:41.064149 dbt_af-0.4.3/dbt_af/common/scheduling.py
--rw-r--r--   0        0        0     1703 2024-05-16 14:49:41.064149 dbt_af-0.4.3/dbt_af/common/utils.py
--rw-r--r--   0        0        0      240 2024-05-16 14:49:41.064149 dbt_af-0.4.3/dbt_af/conf/__init__.py
--rw-r--r--   0        0        0     8134 2024-05-16 14:49:41.064149 dbt_af-0.4.3/dbt_af/conf/config.py
--rw-r--r--   0        0        0     4238 2024-05-16 14:49:41.064149 dbt_af-0.4.3/dbt_af/dags.py
--rw-r--r--   0        0        0        0 2024-05-16 14:49:41.064149 dbt_af-0.4.3/dbt_af/integrations/__init__.py
--rw-r--r--   0        0        0      200 2024-05-16 14:49:41.064149 dbt_af-0.4.3/dbt_af/integrations/mcd/__init__.py
--rw-r--r--   0        0        0      864 2024-05-16 14:49:41.064149 dbt_af-0.4.3/dbt_af/integrations/mcd/callbacks.py
--rw-r--r--   0        0        0     1610 2024-05-16 14:49:41.064149 dbt_af-0.4.3/dbt_af/integrations/mcd/dbt_core.py
--rw-r--r--   0        0        0        0 2024-05-16 14:49:41.064149 dbt_af-0.4.3/dbt_af/operators/__init__.py
--rw-r--r--   0        0        0     9544 2024-05-16 14:49:41.064149 dbt_af-0.4.3/dbt_af/operators/base.py
--rw-r--r--   0        0        0     1804 2024-05-16 14:49:41.064149 dbt_af-0.4.3/dbt_af/operators/branch.py
--rw-r--r--   0        0        0     4865 2024-05-16 14:49:41.064149 dbt_af-0.4.3/dbt_af/operators/kubernetes_pod.py
--rw-r--r--   0        0        0     6238 2024-05-16 14:49:41.064149 dbt_af-0.4.3/dbt_af/operators/macros.py
--rw-r--r--   0        0        0     2416 2024-05-16 14:49:41.064149 dbt_af-0.4.3/dbt_af/operators/run.py
--rw-r--r--   0        0        0    18787 2024-05-16 14:49:41.064149 dbt_af-0.4.3/dbt_af/operators/sensors.py
--rw-r--r--   0        0        0        0 2024-05-16 14:49:41.064149 dbt_af-0.4.3/dbt_af/parser/__init__.py
--rw-r--r--   0        0        0    13163 2024-05-16 14:49:41.064149 dbt_af-0.4.3/dbt_af/parser/dbt_node_model.py
--rw-r--r--   0        0        0     1731 2024-05-16 14:49:41.068149 dbt_af-0.4.3/dbt_af/parser/dbt_profiles.py
--rw-r--r--   0        0        0     2023 2024-05-16 14:49:41.068149 dbt_af-0.4.3/dbt_af/parser/dbt_source_model.py
--rw-r--r--   0        0        0       56 2024-05-16 14:49:41.068149 dbt_af-0.4.3/dbt_af_functional_tests/__init__.py
--rw-r--r--   0        0        0     2880 2024-05-16 14:49:41.068149 dbt_af-0.4.3/dbt_af_functional_tests/conftest.py
--rw-r--r--   0        0        0      791 2024-05-16 14:49:41.068149 dbt_af-0.4.3/dbt_af_functional_tests/main.py
--rw-r--r--   0        0        0      316 2024-05-16 14:49:41.068149 dbt_af-0.4.3/dbt_af_functional_tests/pyproject.toml
--rw-r--r--   0        0        0      923 2024-05-16 14:49:41.068149 dbt_af-0.4.3/dbt_af_functional_tests/test_af_wait_name_too_long.py
--rw-r--r--   0        0        0     2242 2024-05-16 14:49:41.068149 dbt_af-0.4.3/dbt_af_functional_tests/test_all_dbt_models_exist.py
--rw-r--r--   0        0        0      183 2024-05-16 14:49:41.068149 dbt_af-0.4.3/dbt_af_functional_tests/test_dbt_node_model.py
--rw-r--r--   0        0        0      924 2024-05-16 14:49:41.068149 dbt_af-0.4.3/dbt_af_functional_tests/test_dbt_nodes_general_constrains.py
--rw-r--r--   0        0        0      717 2024-05-16 14:49:41.068149 dbt_af-0.4.3/dbt_af_functional_tests/test_kubernetes_profiles.py
--rw-r--r--   0        0        0     2555 2024-05-16 14:49:41.084149 dbt_af-0.4.3/pyproject.toml
--rw-r--r--   0        0        0        0 2024-05-16 14:49:41.084149 dbt_af-0.4.3/scripts/__init__.py
--rw-r--r--   0        0        0     3492 2024-05-16 14:49:41.084149 dbt_af-0.4.3/scripts/mini_dbt_project_generator.py
--rw-r--r--   0        0        0     5003 1970-01-01 00:00:00.000000 dbt_af-0.4.3/PKG-INFO
+-rw-r--r--   0        0        0      193 2024-05-29 11:52:30.173820 dbt_af-0.5.0/AUTHORS
+-rw-r--r--   0        0        0      580 2024-05-29 11:52:30.173820 dbt_af-0.5.0/LICENSE
+-rw-r--r--   0        0        0     4722 2024-05-29 11:52:30.173820 dbt_af-0.5.0/README.md
+-rw-r--r--   0        0        0       95 2024-05-29 11:52:30.173820 dbt_af-0.5.0/dbt_af/__init__.py
+-rw-r--r--   0        0        0      809 2024-05-29 11:52:30.173820 dbt_af-0.5.0/dbt_af/builder/__init__.py
+-rw-r--r--   0        0        0     1076 2024-05-29 11:52:30.173820 dbt_af-0.5.0/dbt_af/builder/backfill_dag_components.py
+-rw-r--r--   0        0        0    16775 2024-05-29 11:52:30.173820 dbt_af-0.5.0/dbt_af/builder/dag_components.py
+-rw-r--r--   0        0        0    10831 2024-05-29 11:52:30.173820 dbt_af-0.5.0/dbt_af/builder/dbt_af_builder.py
+-rw-r--r--   0        0        0     2695 2024-05-29 11:52:30.173820 dbt_af-0.5.0/dbt_af/builder/dbt_model_path_graph_builder.py
+-rw-r--r--   0        0        0     5878 2024-05-29 11:52:30.173820 dbt_af-0.5.0/dbt_af/builder/domain_dag.py
+-rw-r--r--   0        0        0     1507 2024-05-29 11:52:30.173820 dbt_af-0.5.0/dbt_af/builder/maintenance_dag_components.py
+-rw-r--r--   0        0        0     4504 2024-05-29 11:52:30.173820 dbt_af-0.5.0/dbt_af/builder/task_dependencies.py
+-rw-r--r--   0        0        0        0 2024-05-29 11:52:30.173820 dbt_af-0.5.0/dbt_af/common/__init__.py
+-rw-r--r--   0        0        0      552 2024-05-29 11:52:30.173820 dbt_af-0.5.0/dbt_af/common/constants.py
+-rw-r--r--   0        0        0     7473 2024-05-29 11:52:30.173820 dbt_af-0.5.0/dbt_af/common/scheduling.py
+-rw-r--r--   0        0        0     1703 2024-05-29 11:52:30.173820 dbt_af-0.5.0/dbt_af/common/utils.py
+-rw-r--r--   0        0        0      330 2024-05-29 11:52:30.173820 dbt_af-0.5.0/dbt_af/conf/__init__.py
+-rw-r--r--   0        0        0    10498 2024-05-29 11:52:30.173820 dbt_af-0.5.0/dbt_af/conf/config.py
+-rw-r--r--   0        0        0     4238 2024-05-29 11:52:30.173820 dbt_af-0.5.0/dbt_af/dags.py
+-rw-r--r--   0        0        0        0 2024-05-29 11:52:30.173820 dbt_af-0.5.0/dbt_af/integrations/__init__.py
+-rw-r--r--   0        0        0      200 2024-05-29 11:52:30.173820 dbt_af-0.5.0/dbt_af/integrations/mcd/__init__.py
+-rw-r--r--   0        0        0      864 2024-05-29 11:52:30.173820 dbt_af-0.5.0/dbt_af/integrations/mcd/callbacks.py
+-rw-r--r--   0        0        0     1610 2024-05-29 11:52:30.173820 dbt_af-0.5.0/dbt_af/integrations/mcd/dbt_core.py
+-rw-r--r--   0        0        0      274 2024-05-29 11:52:30.173820 dbt_af-0.5.0/dbt_af/integrations/tableau/__init__.py
+-rw-r--r--   0        0        0     1273 2024-05-29 11:52:30.173820 dbt_af-0.5.0/dbt_af/integrations/tableau/auth.py
+-rw-r--r--   0        0        0      127 2024-05-29 11:52:30.173820 dbt_af-0.5.0/dbt_af/integrations/tableau/exceptions.py
+-rw-r--r--   0        0        0     3612 2024-05-29 11:52:30.173820 dbt_af-0.5.0/dbt_af/integrations/tableau/extracts.py
+-rw-r--r--   0        0        0        0 2024-05-29 11:52:30.173820 dbt_af-0.5.0/dbt_af/operators/__init__.py
+-rw-r--r--   0        0        0     9544 2024-05-29 11:52:30.173820 dbt_af-0.5.0/dbt_af/operators/base.py
+-rw-r--r--   0        0        0     1804 2024-05-29 11:52:30.173820 dbt_af-0.5.0/dbt_af/operators/branch.py
+-rw-r--r--   0        0        0     4865 2024-05-29 11:52:30.173820 dbt_af-0.5.0/dbt_af/operators/kubernetes_pod.py
+-rw-r--r--   0        0        0     6238 2024-05-29 11:52:30.173820 dbt_af-0.5.0/dbt_af/operators/macros.py
+-rw-r--r--   0        0        0     2416 2024-05-29 11:52:30.173820 dbt_af-0.5.0/dbt_af/operators/run.py
+-rw-r--r--   0        0        0    18787 2024-05-29 11:52:30.173820 dbt_af-0.5.0/dbt_af/operators/sensors.py
+-rw-r--r--   0        0        0     1021 2024-05-29 11:52:30.173820 dbt_af-0.5.0/dbt_af/operators/supplemental.py
+-rw-r--r--   0        0        0        0 2024-05-29 11:52:30.173820 dbt_af-0.5.0/dbt_af/parser/__init__.py
+-rw-r--r--   0        0        0    13514 2024-05-29 11:52:30.173820 dbt_af-0.5.0/dbt_af/parser/dbt_node_model.py
+-rw-r--r--   0        0        0     1731 2024-05-29 11:52:30.173820 dbt_af-0.5.0/dbt_af/parser/dbt_profiles.py
+-rw-r--r--   0        0        0     2023 2024-05-29 11:52:30.173820 dbt_af-0.5.0/dbt_af/parser/dbt_source_model.py
+-rw-r--r--   0        0        0       56 2024-05-29 11:52:30.173820 dbt_af-0.5.0/dbt_af_functional_tests/__init__.py
+-rw-r--r--   0        0        0     2880 2024-05-29 11:52:30.173820 dbt_af-0.5.0/dbt_af_functional_tests/conftest.py
+-rw-r--r--   0        0        0      791 2024-05-29 11:52:30.173820 dbt_af-0.5.0/dbt_af_functional_tests/main.py
+-rw-r--r--   0        0        0      316 2024-05-29 11:52:30.173820 dbt_af-0.5.0/dbt_af_functional_tests/pyproject.toml
+-rw-r--r--   0        0        0      923 2024-05-29 11:52:30.173820 dbt_af-0.5.0/dbt_af_functional_tests/test_af_wait_name_too_long.py
+-rw-r--r--   0        0        0     2242 2024-05-29 11:52:30.173820 dbt_af-0.5.0/dbt_af_functional_tests/test_all_dbt_models_exist.py
+-rw-r--r--   0        0        0      183 2024-05-29 11:52:30.173820 dbt_af-0.5.0/dbt_af_functional_tests/test_dbt_node_model.py
+-rw-r--r--   0        0        0      924 2024-05-29 11:52:30.173820 dbt_af-0.5.0/dbt_af_functional_tests/test_dbt_nodes_general_constrains.py
+-rw-r--r--   0        0        0      717 2024-05-29 11:52:30.173820 dbt_af-0.5.0/dbt_af_functional_tests/test_kubernetes_profiles.py
+-rw-r--r--   0        0        0     2982 2024-05-29 11:52:30.193821 dbt_af-0.5.0/pyproject.toml
+-rw-r--r--   0        0        0        0 2024-05-29 11:52:30.193821 dbt_af-0.5.0/scripts/__init__.py
+-rw-r--r--   0        0        0     3492 2024-05-29 11:52:30.193821 dbt_af-0.5.0/scripts/mini_dbt_project_generator.py
+-rw-r--r--   0        0        0     6433 1970-01-01 00:00:00.000000 dbt_af-0.5.0/PKG-INFO
```

### Comparing `dbt_af-0.4.3/LICENSE` & `dbt_af-0.5.0/LICENSE`

 * *Files identical despite different names*

### Comparing `dbt_af-0.4.3/README.md` & `dbt_af-0.5.0/README.md`

 * *Files 21% similar despite different names*

```diff
@@ -8,30 +8,34 @@
 [![Poetry](https://img.shields.io/endpoint?url=https://python-poetry.org/badge/v0.json)](https://python-poetry.org/)
 [![Code style: black](https://img.shields.io/badge/code%20style-black-000000.svg)](https://github.com/psf/black)
 
 # dbt-af: distributed run of dbt models using Airflow
 
 ## Overview
 
-_dbt-af_ is a tool that allows you to run dbt models in a distributed manner using Airflow.
+**_dbt-af_** is a tool that allows you to run dbt models in a distributed manner using Airflow.
 It acts as a wrapper around the Airflow DAG,
 allowing you to run the models independently while preserving their dependencies.
 
 ![dbt-af](docs/static/airflow_dag_layout.png)
 
 ### Why?
 
-1. _dbt-af_ is [domain-driven](https://www.datamesh-architecture.com/#what-is-data-mesh).
+1. **_dbt-af_** is [domain-driven](https://www.datamesh-architecture.com/#what-is-data-mesh).
    It is designed to separate models from different domains into different DAGs.
    This allows you to run models from different domains in parallel.
-2. _dbt-af_ brings scheduling to dbt. You can schedule your dbt models to run at a specific time.
-3. _dbt-af_ is an ETL-driven tool.
+2. **_dbt-af_** is **dbt-first** solution.
+   It is designed to make analytics' life easier.
+   End-users could even not know that Airflow is used to schedule their models.
+   dbt-model's config is an entry point for all your settings and customizations.
+3. **_dbt-af_** brings scheduling to dbt. From `@monthly` to `@hourly` and even [more](examples/manual_scheduling.md).
+4. **_dbt-af_** is an ETL-driven tool.
    You can separate your models into tiers or ETL stages
    and build graphs showing the dependencies between models within each tier or stage.
-4. _dbt-af_ brings additional features to use different dbt targets simultaneously, different tests scenarios, and
+5. **_dbt-af_** brings additional features to use different dbt targets simultaneously, different tests scenarios, and
    maintenance tasks.
 
 ## Installation
 
 To install `dbt-af` run `pip install dbt-af`.
 
 To contribute we recommend to use `poetry` to install package dependencies. Run `poetry install --with=dev` to install
@@ -64,24 +68,38 @@
 )
 
 dags = compile_dbt_af_dags(manifest_path='/path/to/my_dbt_project/target/manifest.json', config=config)
 for dag_name, dag in dags.items():
     globals()[dag_name] = dag
 ```
 
-In _dbt_project.yml_ you need to set up default targets for all nodes in your project 
+In _dbt_project.yml_ you need to set up default targets for all nodes in your project
 (see [example](examples/dags/dbt_project.yml)):
 
 ```yaml
 sql_cluster: "dev"
 daily_sql_cluster: "dev"
 py_cluster: "dev"
 bf_cluster: "dev"
 ```
 
 This will create Airflow DAGs for your dbt project.
 
+## Features
+
+1. **_dbt-af_** is essentially designed to work with large projects (1000+ models).
+   When dealing with a significant number of dbt objects across different domains,
+   it becomes crucial to have all DAGs auto-generated.
+   **_dbt-af_** takes care of this by generating all the necessary DAGs for your dbt project and structuring them by
+   domains.
+2. Each dbt run is separated into a different Airflow task. All tasks receive a date interval from the Airflow DAG
+   context. By using the passed date interval in your dbt models, you ensure the *idempotency* of your dbt runs.
+3. _**dbt-af**_ lowers the entry threshold for non-infrastructure team members.
+   This means that analytics professionals, data scientists,
+   and data engineers can focus on their dbt models and important business logic
+   rather than spending time on Airflow DAGs.
+
 ## Project Information
 
 - [Docs](examples/README.md)
 - [PyPI](https://pypi.org/project/dbt-af/)
-- Contributing
+- [Contributing](CONTRIBUTING.md)
```

### Comparing `dbt_af-0.4.3/dbt_af/builder/__init__.py` & `dbt_af-0.5.0/dbt_af/builder/__init__.py`

 * *Files identical despite different names*

### Comparing `dbt_af-0.4.3/dbt_af/builder/backfill_dag_components.py` & `dbt_af-0.5.0/dbt_af/builder/backfill_dag_components.py`

 * *Files identical despite different names*

### Comparing `dbt_af-0.4.3/dbt_af/builder/dag_components.py` & `dbt_af-0.5.0/dbt_af/builder/dag_components.py`

 * *Files 6% similar despite different names*

```diff
@@ -7,14 +7,15 @@
 from dbt_af.builder.domain_dag import DomainDag
 from dbt_af.builder.task_dependencies import DagDelayedDependencyRegistry
 from dbt_af.common.scheduling import ScheduleTag
 from dbt_af.operators.branch import DbtBranchOperator, create_decision_path_function
 from dbt_af.operators.kubernetes_pod import DbtKubernetesPodOperator
 from dbt_af.operators.run import DbtRun, DbtSeed, DbtSnapshot, DbtTest
 from dbt_af.operators.sensors import AfExecutionDateFn, DbtExternalSensor, DbtSourceFreshnessSensor
+from dbt_af.operators.supplemental import TableauExtractsRefreshOperator
 from dbt_af.parser.dbt_node_model import DbtNode, DbtNodeConfig
 from dbt_af.parser.dbt_profiles import KubernetesTarget
 from dbt_af.parser.dbt_source_model import DbtSource
 
 
 class DagComponent:
     add_external_dependencies = True
@@ -179,22 +180,23 @@
 
     def _get_source_deps_with_freshness_check(self) -> list[DbtSource]:
         return [dep for dep in self._depends_on_sources if dep.need_to_check_freshness()]
 
     def _create_task_group(self) -> Optional[TaskGroup]:
         """
         Create a task group for the model if it has external dependencies or small tests. If waits for all external
-        dependencies are built per domain, task group is not needed
+        dependencies are built per domain, a task group is not needed
         """
         if (
             not self._small_tests
             and (not self._get_ext_deps() or self.domain_dag.config.model_dependencies.wait_policy.per_domain)
             and not self._get_source_deps_with_freshness_check()
             and not self.node_config.enable_from_dttm
             and not self.node_config.disable_from_dttm
+            and not self.node_config.tableau_refresh_tasks
         ):
             return None
 
         return TaskGroup(f'{self.safe_name}__group', dag=self.domain_dag.af_dag)
 
     def init_af(self):
         raise NotImplementedError
@@ -300,14 +302,25 @@
                     source_name=source_dep.source_name,
                     source_identifier=source_dep.identifier,
                     dbt_af_config=self.domain_dag.config,
                 )
 
                 delayed_deps(source_wait) >> delayed_deps(self.model_task)
 
+    def _init_supplemental_dependencies_af(self, delayed_deps: DagDelayedDependencyRegistry):
+        if self.dbt_node.config.tableau_refresh_tasks:
+            tableau_refresh_task = TableauExtractsRefreshOperator(
+                task_id=f'tableau_refresh__{self.safe_name}',
+                task_group=self.task_group,
+                dag=self.domain_dag.af_dag,
+                tableau_refresh_tasks=self.dbt_node.config.tableau_refresh_tasks,
+                dbt_af_config=self.domain_dag.config,
+            )
+            delayed_deps(self.model_task) >> delayed_deps(tableau_refresh_task)
+
     def init_af(self):
         """
         Initialize all Airflow components for the dbt-model and it's dependencies
         """
         if self.domain_dag.af_dag is None:
             raise ValueError(f'{self!r}: dag not set')
 
@@ -317,14 +330,15 @@
             endpoint_task = self._init_small_tests_af(delayed_deps)
 
             self.af_component = self.task_group or self.model_task
             self.af_sensor_endpoint = endpoint_task or self.model_task
 
             self._init_dependencies_af(delayed_deps)
             self._init_source_dependencies_af(delayed_deps)
+            self._init_supplemental_dependencies_af(delayed_deps)
 
 
 class DagSnapshot(DagModel):
     runner_class = DbtSnapshot
 
 
 class DagSeed(DagModel):
```

### Comparing `dbt_af-0.4.3/dbt_af/builder/dbt_af_builder.py` & `dbt_af-0.5.0/dbt_af/builder/dbt_af_builder.py`

 * *Files identical despite different names*

### Comparing `dbt_af-0.4.3/dbt_af/builder/dbt_model_path_graph_builder.py` & `dbt_af-0.5.0/dbt_af/builder/dbt_model_path_graph_builder.py`

 * *Files identical despite different names*

### Comparing `dbt_af-0.4.3/dbt_af/builder/domain_dag.py` & `dbt_af-0.5.0/dbt_af/builder/domain_dag.py`

 * *Files identical despite different names*

### Comparing `dbt_af-0.4.3/dbt_af/builder/maintenance_dag_components.py` & `dbt_af-0.5.0/dbt_af/builder/maintenance_dag_components.py`

 * *Files identical despite different names*

### Comparing `dbt_af-0.4.3/dbt_af/builder/task_dependencies.py` & `dbt_af-0.5.0/dbt_af/builder/task_dependencies.py`

 * *Files identical despite different names*

### Comparing `dbt_af-0.4.3/dbt_af/common/constants.py` & `dbt_af-0.5.0/dbt_af/common/constants.py`

 * *Files identical despite different names*

### Comparing `dbt_af-0.4.3/dbt_af/common/scheduling.py` & `dbt_af-0.5.0/dbt_af/common/scheduling.py`

 * *Files identical despite different names*

### Comparing `dbt_af-0.4.3/dbt_af/common/utils.py` & `dbt_af-0.5.0/dbt_af/common/utils.py`

 * *Files identical despite different names*

### Comparing `dbt_af-0.4.3/dbt_af/conf/config.py` & `dbt_af-0.5.0/dbt_af/conf/config.py`

 * *Files 24% similar despite different names*

```diff
@@ -51,14 +51,69 @@
     callbacks_enabled: bool = attrs.field(default=False)
     artifacts_export_enabled: bool = attrs.field(default=False)
     success_required: bool = attrs.field(default=False)
     metastore_name: str = attrs.field(default='')
 
 
 @attrs.define(frozen=True)
+class TableauIntegrationConfig:
+    """
+    Config for Tableau integration.
+    There are two ways to authenticate:
+        - with username and password
+        - with token name and personal access token (PAT)
+    You can use only one of them. If both are specified, then username and password will be used.
+
+    :param server_address: The address of the Tableau Server or Tableau Online instance.
+
+    :param username: The name of the user whose credentials will be used to sign in
+    :param password: The password of the user.
+    :param user_id_to_impersonate: Specifies the id (not the name) of the user to sign in as.
+
+    :param token_name: The personal access token name.
+    :param pat: The personal access token.
+
+    :param site_id: This corresponds to the contentUrl attribute in the Tableau REST API.
+        The site_id is the portion of the URL that follows the /site/ in the URL. For example,
+        “MarketingTeam” is the site_id in the following URL MyServer/#/site/MarketingTeam/projects.
+        To specify the default site on Tableau Server, you can use an empty string '' (single quotes, no space).
+        For Tableau Cloud, you must provide a value for the site_id.
+    """
+
+    server_address: str = attrs.field(validator=attrs.validators.instance_of(str))
+
+    username: Optional[str] = attrs.field(
+        default=None,
+        validator=attrs.validators.optional(attrs.validators.instance_of(str)),
+    )
+    password: Optional[str] = attrs.field(
+        default=None,
+        validator=attrs.validators.optional(attrs.validators.instance_of(str)),
+    )
+    user_id_to_impersonate: Optional[str] = attrs.field(
+        default=None,
+        validator=attrs.validators.optional(attrs.validators.instance_of(str)),
+    )
+
+    token_name: Optional[str] = attrs.field(
+        default=None,
+        validator=attrs.validators.optional(attrs.validators.instance_of(str)),
+    )
+    pat: Optional[str] = attrs.field(
+        default=None,
+        validator=attrs.validators.optional(attrs.validators.instance_of(str)),
+    )
+
+    site_id: Optional[str] = attrs.field(
+        default=None,
+        validator=attrs.validators.optional(attrs.validators.instance_of(str)),
+    )
+
+
+@attrs.define(frozen=True)
 class DbtProjectConfig:
     """
     Config for dbt project.
 
     :param dbt_project_name: name of dbt project; refer to field `name` in dbt_project.yml
     # TODO: read from dbt_project.yml
     :param dbt_models_path: path to dbt models; it's used in k8s operators to find raw models code
@@ -154,19 +209,22 @@
     dbt_project: DbtProjectConfig = attrs.field()
 
     # dbt-af specific params
     dbt_default_targets: DbtDefaultTargetsConfig = attrs.field()
     model_dependencies: ModelDependenciesSection = attrs.field(factory=ModelDependenciesSection)
     include_single_model_manual_dag: bool = attrs.field(default=True)
 
-    # airflow specific params
+    # airflow-specific params
     max_active_dag_runs: int = attrs.field(default=50)
     af_dag_description: str = attrs.field(default='https://www.buymeacoffee.com/tolokadataplatform')
     dag_start_date: pendulum.datetime = attrs.field(default=pendulum.datetime(2023, 10, 1, 0, 0, 0, tz='UTC'))
     is_dev: bool = attrs.field(default=False)
     use_dbt_target_specific_pools: bool = attrs.field(default=True)
 
-    # mcd
+    # Monte Carlo Data integration
     mcd: Optional[MCDIntegrationConfig] = attrs.field(default=None)
 
+    # Tableau integration
+    tableau: Optional[TableauIntegrationConfig] = attrs.field(default=None)
+
     # k8s
     k8s: K8sConfig = attrs.field(factory=K8sConfig)
```

#### encoding

```diff
@@ -1 +1 @@
-us-ascii
+utf-8
```

### Comparing `dbt_af-0.4.3/dbt_af/dags.py` & `dbt_af-0.5.0/dbt_af/dags.py`

 * *Files identical despite different names*

### Comparing `dbt_af-0.4.3/dbt_af/integrations/mcd/callbacks.py` & `dbt_af-0.5.0/dbt_af/integrations/mcd/callbacks.py`

 * *Files identical despite different names*

### Comparing `dbt_af-0.4.3/dbt_af/integrations/mcd/dbt_core.py` & `dbt_af-0.5.0/dbt_af/integrations/mcd/dbt_core.py`

 * *Files identical despite different names*

### Comparing `dbt_af-0.4.3/dbt_af/operators/base.py` & `dbt_af-0.5.0/dbt_af/operators/base.py`

 * *Files identical despite different names*

### Comparing `dbt_af-0.4.3/dbt_af/operators/branch.py` & `dbt_af-0.5.0/dbt_af/operators/branch.py`

 * *Files identical despite different names*

### Comparing `dbt_af-0.4.3/dbt_af/operators/kubernetes_pod.py` & `dbt_af-0.5.0/dbt_af/operators/kubernetes_pod.py`

 * *Files identical despite different names*

### Comparing `dbt_af-0.4.3/dbt_af/operators/macros.py` & `dbt_af-0.5.0/dbt_af/operators/macros.py`

 * *Files identical despite different names*

### Comparing `dbt_af-0.4.3/dbt_af/operators/run.py` & `dbt_af-0.5.0/dbt_af/operators/run.py`

 * *Files identical despite different names*

### Comparing `dbt_af-0.4.3/dbt_af/operators/sensors.py` & `dbt_af-0.5.0/dbt_af/operators/sensors.py`

 * *Files identical despite different names*

### Comparing `dbt_af-0.4.3/dbt_af/parser/dbt_node_model.py` & `dbt_af-0.5.0/dbt_af/parser/dbt_node_model.py`

 * *Files 2% similar despite different names*

```diff
@@ -76,14 +76,25 @@
             maintenance_types.append(DbtModelMaintenanceType.VACUUM_TABLE)
         if self.deduplicate_table:
             maintenance_types.append(DbtModelMaintenanceType.DEDUPLICATE_TABLE)
 
         return maintenance_types
 
 
+class TableauRefreshResourceType(str, enum.Enum):
+    workbook = 'workbook'
+    datasource = 'datasource'
+
+
+class TableauRefreshTaskConfig(pydantic.BaseModel):
+    resource_name: str
+    project_name: str
+    resource_type: TableauRefreshResourceType
+
+
 class DbtNodeConfig(pydantic.BaseModel):
     enabled: bool
     alias: Optional[str]
     node_schema: Optional[str] = pydantic.Field(..., alias='schema')
     database: Optional[str]
     tags: List[str]
     meta: Dict[str, Any]
@@ -122,15 +133,17 @@
     disable_from_dttm: Optional[str] = pydantic.Field(default='')
 
     airflow_parallelism: int = pydantic.Field(default=1)
     domain_start_date: Optional[str] = pydantic.Field(default='')
 
     dbt_target: Optional[str] = pydantic.Field(default='')
 
-    maintenance: Optional[DbtAFMaintenanceConfig] = pydantic.Field(default_factory=DbtAFMaintenanceConfig)
+    maintenance: DbtAFMaintenanceConfig = pydantic.Field(default_factory=DbtAFMaintenanceConfig)
+
+    tableau_refresh_tasks: Optional[List[TableauRefreshTaskConfig]] = pydantic.Field(default_factory=list)
 
     class Config:
         arbitrary_types_allowed = True
 
     @pydantic.root_validator(pre=True)
     def validate_clusters(cls, values):
         if values['materialized'] not in ('test', 'seed'):
```

### Comparing `dbt_af-0.4.3/dbt_af/parser/dbt_profiles.py` & `dbt_af-0.5.0/dbt_af/parser/dbt_profiles.py`

 * *Files identical despite different names*

### Comparing `dbt_af-0.4.3/dbt_af/parser/dbt_source_model.py` & `dbt_af-0.5.0/dbt_af/parser/dbt_source_model.py`

 * *Files identical despite different names*

### Comparing `dbt_af-0.4.3/dbt_af_functional_tests/conftest.py` & `dbt_af-0.5.0/dbt_af_functional_tests/conftest.py`

 * *Files identical despite different names*

### Comparing `dbt_af-0.4.3/dbt_af_functional_tests/main.py` & `dbt_af-0.5.0/dbt_af_functional_tests/main.py`

 * *Files identical despite different names*

### Comparing `dbt_af-0.4.3/dbt_af_functional_tests/test_af_wait_name_too_long.py` & `dbt_af-0.5.0/dbt_af_functional_tests/test_af_wait_name_too_long.py`

 * *Files identical despite different names*

### Comparing `dbt_af-0.4.3/dbt_af_functional_tests/test_all_dbt_models_exist.py` & `dbt_af-0.5.0/dbt_af_functional_tests/test_all_dbt_models_exist.py`

 * *Files identical despite different names*

### Comparing `dbt_af-0.4.3/dbt_af_functional_tests/test_dbt_nodes_general_constrains.py` & `dbt_af-0.5.0/dbt_af_functional_tests/test_dbt_nodes_general_constrains.py`

 * *Files identical despite different names*

### Comparing `dbt_af-0.4.3/dbt_af_functional_tests/test_kubernetes_profiles.py` & `dbt_af-0.5.0/dbt_af_functional_tests/test_kubernetes_profiles.py`

 * *Files identical despite different names*

### Comparing `dbt_af-0.4.3/pyproject.toml` & `dbt_af-0.5.0/pyproject.toml`

 * *Files 23% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 [tool.poetry]
 name = "dbt-af"
-version = "0.4.3"
+version = "0.5.0"
 description = "Distibuted dbt runs on Apache Airflow"
 authors = [
     "Nikita Yurasov <nikitayurasov@toloka.ai>",
     "Igor Safonov <igsaf@toloka.ai>",
     "Evgeny Ermakov <jkermakov@toloka.ai>",
     "Leonid Kozhinov <lkozhinov@toloka.ai>",
 ]
@@ -18,52 +18,60 @@
     { include = "dbt_af" },
     { include = "dbt_af_functional_tests" },
     { include = "scripts" },
 ]
 
 [tool.poetry.dependencies]
 python = ">=3.10,<3.12"
-attrs = "~23.1"
+attrs = "^23.1"
 apache-airflow = ">=2.6"
 pydantic = ">=1.10,<3.0.0"
 apache-airflow-providers-cncf-kubernetes = ">=7.0.0"
 cachetools = "~5.3"
 typer = "~0.9"
-dbt-core = "~1.7"
+dbt-core = "^1.7"
 pendulum = "^2"
 
 pytest = { version = "*", optional = true }
 pytest-env = { version = "*", optional = true }
 pytest-socket = { version = "*", optional = true }
 pytest-mock = { version = "*", optional = true }
 
-airflow-mcd = { version = "~0.2", optional = true }
-pycarlo = { version = "~0.8", optional = true }
+airflow-mcd = { version = "^0.2", optional = true }
+pycarlo = { version = "^0.8", optional = true }
 
-dbt-postgres = { version = "~1.7", optional = true }
+tableauserverclient = { version = "^0.30", optional = true }
+
+dbt-postgres = { version = "^1.7", optional = true }
 
 [tool.poetry.group.dev.dependencies]
-isort = "~5.12"
-black = "~23.7"
 ruff = "^0.3"
-twine = "*"
 pytest = "^8"
 pytest-env = "*"
 pytest-cov = "~4.1"
 pytest-socket = "*"
 pytest-mock = "*"
-dbt-postgres = "~1.7"
-dbt-databricks = "1.7.8"
+dbt-postgres = "^1.7"
+psycopg2-binary = { version = "^2.9", markers = "sys_platform == 'linux'" }  # due to bug https://github.com/dbt-labs/dbt-postgres/issues/96
+dbt-databricks = "^1.7"
 pre-commit = "3.6.2"
+ipython = "^8"
 
 [tool.poetry.extras]
 mcd = ["airflow-mcd", "pycarlo"]
 tests = ["pytest", "pytest-env", "pytest-socket", "pytest-mock"]
 minidbt = []
-examples = ["dbt-postgres"]
+examples = ["dbt-postgres", "psycopg2-binary"]
+tableau = ["tableauserverclient"]
+all = [
+    "airflow-mcd", "pycarlo", # mcd
+    "pytest", "pytest-env", "pytest-socket", "pytest-mock", # tests
+    "dbt-postgres", "psycopg2-binary", # examples
+    "tableauserverclient", # tableau
+]
 
 [tool.poetry.scripts]
 dbt-af-manifest-tests = { callable = "dbt_af_functional_tests:cli", extras = ["tests"] }
 mini_dbt_project_generator = { callable = "scripts.mini_dbt_project_generator:cli", extras = ["minidbt"] }
 
 [build-system]
 requires = ["poetry-core"]
```

### Comparing `dbt_af-0.4.3/scripts/mini_dbt_project_generator.py` & `dbt_af-0.5.0/scripts/mini_dbt_project_generator.py`

 * *Files identical despite different names*

