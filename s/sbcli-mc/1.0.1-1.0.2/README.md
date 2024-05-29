# Comparing `tmp/sbcli_mc-1.0.1.zip` & `tmp/sbcli_mc-1.0.2.zip`

## zipinfo {}

```diff
@@ -1,150 +1,150 @@
-Zip file size: 215819 bytes, number of entries: 148
-drwxr-xr-x  2.0 unx        0 b- stor 24-May-24 01:01 sbcli_mc-1.0.1/
-drwxr-xr-x  2.0 unx        0 b- stor 24-May-24 01:01 sbcli_mc-1.0.1/simplyblock_cli/
-drwxr-xr-x  2.0 unx        0 b- stor 24-May-24 01:01 sbcli_mc-1.0.1/simplyblock_web/
-drwxr-xr-x  2.0 unx        0 b- stor 24-May-24 01:01 sbcli_mc-1.0.1/simplyblock_core/
-drwxr-xr-x  2.0 unx        0 b- stor 24-May-24 01:01 sbcli_mc-1.0.1/sbcli_mc.egg-info/
--rw-r--r--  2.0 unx     1068 b- defN 24-May-24 01:00 sbcli_mc-1.0.1/README.md
--rw-r--r--  2.0 unx       84 b- defN 24-May-24 01:00 sbcli_mc-1.0.1/pyproject.toml
--rw-r--r--  2.0 unx     1488 b- defN 24-May-24 01:01 sbcli_mc-1.0.1/PKG-INFO
--rw-r--r--  2.0 unx      157 b- defN 24-May-24 01:00 sbcli_mc-1.0.1/env_var
--rw-r--r--  2.0 unx       38 b- defN 24-May-24 01:01 sbcli_mc-1.0.1/setup.cfg
--rw-r--r--  2.0 unx     2269 b- defN 24-May-24 01:00 sbcli_mc-1.0.1/setup.py
--rw-r--r--  2.0 unx    79056 b- defN 24-May-24 01:00 sbcli_mc-1.0.1/simplyblock_cli/cli.py
--rw-r--r--  2.0 unx      357 b- defN 24-May-24 01:00 sbcli_mc-1.0.1/simplyblock_cli/main.py
-drwxr-xr-x  2.0 unx        0 b- stor 24-May-24 01:01 sbcli_mc-1.0.1/simplyblock_web/static/
-drwxr-xr-x  2.0 unx        0 b- stor 24-May-24 01:01 sbcli_mc-1.0.1/simplyblock_web/blueprints/
-drwxr-xr-x  2.0 unx        0 b- stor 24-May-24 01:01 sbcli_mc-1.0.1/simplyblock_web/templates/
--rw-r--r--  2.0 unx        0 b- defN 24-May-24 01:00 sbcli_mc-1.0.1/simplyblock_web/__init__.py
--rw-r--r--  2.0 unx     1434 b- defN 24-May-24 01:00 sbcli_mc-1.0.1/simplyblock_web/node_webapp.py
--rw-r--r--  2.0 unx      703 b- defN 24-May-24 01:00 sbcli_mc-1.0.1/simplyblock_web/snode_app.py
--rw-r--r--  2.0 unx      717 b- defN 24-May-24 01:00 sbcli_mc-1.0.1/simplyblock_web/caching_node_app.py
--rw-r--r--  2.0 unx     1638 b- defN 24-May-24 01:00 sbcli_mc-1.0.1/simplyblock_web/auth_middleware.py
--rw-r--r--  2.0 unx     5098 b- defN 24-May-24 01:00 sbcli_mc-1.0.1/simplyblock_web/node_utils.py
--rw-r--r--  2.0 unx     2715 b- defN 24-May-24 01:00 sbcli_mc-1.0.1/simplyblock_web/utils.py
--rw-r--r--  2.0 unx     1263 b- defN 24-May-24 01:00 sbcli_mc-1.0.1/simplyblock_web/app.py
--rw-r--r--  2.0 unx      725 b- defN 24-May-24 01:00 sbcli_mc-1.0.1/simplyblock_web/caching_node_app_k8s.py
--rw-r--r--  2.0 unx      322 b- defN 24-May-24 01:00 sbcli_mc-1.0.1/simplyblock_web/static/tst.py
--rw-r--r--  2.0 unx      827 b- defN 24-May-24 01:00 sbcli_mc-1.0.1/simplyblock_web/static/delete.py
--rw-r--r--  2.0 unx      507 b- defN 24-May-24 01:00 sbcli_mc-1.0.1/simplyblock_web/static/deploy_cnode.yaml
--rw-r--r--  2.0 unx      434 b- defN 24-May-24 01:00 sbcli_mc-1.0.1/simplyblock_web/static/is_up.py
--rw-r--r--  2.0 unx     1466 b- defN 24-May-24 01:00 sbcli_mc-1.0.1/simplyblock_web/static/deploy_spdk.yaml
--rw-r--r--  2.0 unx      463 b- defN 24-May-24 01:00 sbcli_mc-1.0.1/simplyblock_web/static/rpac.yaml
--rw-r--r--  2.0 unx      417 b- defN 24-May-24 01:00 sbcli_mc-1.0.1/simplyblock_web/static/list_deps.py
--rw-r--r--  2.0 unx     1302 b- defN 24-May-24 01:00 sbcli_mc-1.0.1/simplyblock_web/static/deploy.py
--rw-r--r--  2.0 unx     6206 b- defN 24-May-24 01:00 sbcli_mc-1.0.1/simplyblock_web/blueprints/web_api_pool.py
--rw-r--r--  2.0 unx        0 b- defN 24-May-24 01:00 sbcli_mc-1.0.1/simplyblock_web/blueprints/__init__.py
--rw-r--r--  2.0 unx     3118 b- defN 24-May-24 01:00 sbcli_mc-1.0.1/simplyblock_web/blueprints/web_api_device.py
--rw-r--r--  2.0 unx     8685 b- defN 24-May-24 01:00 sbcli_mc-1.0.1/simplyblock_web/blueprints/web_api_lvol.py
--rw-r--r--  2.0 unx     9713 b- defN 24-May-24 01:00 sbcli_mc-1.0.1/simplyblock_web/blueprints/snode_ops.py
--rw-r--r--  2.0 unx    12385 b- defN 24-May-24 01:00 sbcli_mc-1.0.1/simplyblock_web/blueprints/caching_node_ops.py
--rw-r--r--  2.0 unx     6401 b- defN 24-May-24 01:00 sbcli_mc-1.0.1/simplyblock_web/blueprints/web_api_storage_node.py
--rw-r--r--  2.0 unx     6209 b- defN 24-May-24 01:00 sbcli_mc-1.0.1/simplyblock_web/blueprints/web_api_cluster.py
--rw-r--r--  2.0 unx     8075 b- defN 24-May-24 01:00 sbcli_mc-1.0.1/simplyblock_web/blueprints/caching_node_ops_k8s.py
--rw-r--r--  2.0 unx     4883 b- defN 24-May-24 01:00 sbcli_mc-1.0.1/simplyblock_web/blueprints/node_api_caching_ks.py
--rw-r--r--  2.0 unx     5746 b- defN 24-May-24 01:00 sbcli_mc-1.0.1/simplyblock_web/blueprints/node_api_caching_docker.py
--rw-r--r--  2.0 unx     5491 b- defN 24-May-24 01:00 sbcli_mc-1.0.1/simplyblock_web/blueprints/web_api_caching_node.py
--rw-r--r--  2.0 unx     3103 b- defN 24-May-24 01:00 sbcli_mc-1.0.1/simplyblock_web/blueprints/node_api_basic.py
--rw-r--r--  2.0 unx    11244 b- defN 24-May-24 01:00 sbcli_mc-1.0.1/simplyblock_web/blueprints/csi.py
--rw-r--r--  2.0 unx      975 b- defN 24-May-24 01:00 sbcli_mc-1.0.1/simplyblock_web/blueprints/web_api_mgmt_node.py
--rw-r--r--  2.0 unx     2905 b- defN 24-May-24 01:00 sbcli_mc-1.0.1/simplyblock_web/templates/deploy_spdk.yaml.j2
-drwxr-xr-x  2.0 unx        0 b- stor 24-May-24 01:01 sbcli_mc-1.0.1/simplyblock_core/services/
-drwxr-xr-x  2.0 unx        0 b- stor 24-May-24 01:01 sbcli_mc-1.0.1/simplyblock_core/controllers/
-drwxr-xr-x  2.0 unx        0 b- stor 24-May-24 01:01 sbcli_mc-1.0.1/simplyblock_core/models/
-drwxr-xr-x  2.0 unx        0 b- stor 24-May-24 01:01 sbcli_mc-1.0.1/simplyblock_core/scripts/
--rw-r--r--  2.0 unx    25582 b- defN 24-May-24 01:00 sbcli_mc-1.0.1/simplyblock_core/cluster_ops.py
--rw-r--r--  2.0 unx      938 b- defN 24-May-24 01:00 sbcli_mc-1.0.1/simplyblock_core/pci_utils.py
--rw-r--r--  2.0 unx        0 b- defN 24-May-24 01:00 sbcli_mc-1.0.1/simplyblock_core/__init__.py
--rw-r--r--  2.0 unx     3193 b- defN 24-May-24 01:00 sbcli_mc-1.0.1/simplyblock_core/snode_client.py
--rw-r--r--  2.0 unx     8799 b- defN 24-May-24 01:00 sbcli_mc-1.0.1/simplyblock_core/kv_store.py
--rw-r--r--  2.0 unx     5112 b- defN 24-May-24 01:00 sbcli_mc-1.0.1/simplyblock_core/compute_node_ops.py
--rw-r--r--  2.0 unx    22010 b- defN 24-May-24 01:00 sbcli_mc-1.0.1/simplyblock_core/rpc_client.py
--rw-r--r--  2.0 unx     3153 b- defN 24-May-24 01:00 sbcli_mc-1.0.1/simplyblock_core/mgmt_node_ops.py
--rw-r--r--  2.0 unx     7640 b- defN 24-May-24 01:00 sbcli_mc-1.0.1/simplyblock_core/utils.py
--rw-r--r--  2.0 unx     7725 b- defN 24-May-24 01:00 sbcli_mc-1.0.1/simplyblock_core/distr_controller.py
--rw-r--r--  2.0 unx      279 b- defN 24-May-24 01:00 sbcli_mc-1.0.1/simplyblock_core/shell_utils.py
--rw-r--r--  2.0 unx     3638 b- defN 24-May-24 01:00 sbcli_mc-1.0.1/simplyblock_core/cnode_client.py
--rw-r--r--  2.0 unx    66705 b- defN 24-May-24 01:00 sbcli_mc-1.0.1/simplyblock_core/storage_node_ops.py
--rw-r--r--  2.0 unx     1511 b- defN 24-May-24 01:00 sbcli_mc-1.0.1/simplyblock_core/constants.py
--rw-r--r--  2.0 unx     3444 b- defN 24-May-24 01:00 sbcli_mc-1.0.1/simplyblock_core/services/job_tasks.py
--rw-r--r--  2.0 unx     3203 b- defN 24-May-24 01:00 sbcli_mc-1.0.1/simplyblock_core/services/caching_node_monitor.py
--rw-r--r--  2.0 unx      229 b- defN 24-May-24 01:00 sbcli_mc-1.0.1/simplyblock_core/services/service_template.service
--rw-r--r--  2.0 unx      837 b- defN 24-May-24 01:00 sbcli_mc-1.0.1/simplyblock_core/services/install_service.sh
--rw-r--r--  2.0 unx     4118 b- defN 24-May-24 01:00 sbcli_mc-1.0.1/simplyblock_core/services/__init__.py
--rw-r--r--  2.0 unx     2410 b- defN 24-May-24 01:00 sbcli_mc-1.0.1/simplyblock_core/services/log_agg_service.py
--rw-r--r--  2.0 unx     5751 b- defN 24-May-24 01:00 sbcli_mc-1.0.1/simplyblock_core/services/health_check_service.py
--rw-r--r--  2.0 unx     7439 b- defN 24-May-24 01:00 sbcli_mc-1.0.1/simplyblock_core/services/capacity_and_stats_collector.py
--rw-r--r--  2.0 unx     3169 b- defN 24-May-24 01:00 sbcli_mc-1.0.1/simplyblock_core/services/device_monitor.py
--rw-r--r--  2.0 unx     5268 b- defN 24-May-24 01:00 sbcli_mc-1.0.1/simplyblock_core/services/lvol_stat_collector.py
--rw-r--r--  2.0 unx     2671 b- defN 24-May-24 01:00 sbcli_mc-1.0.1/simplyblock_core/services/cap_monitor.py
--rw-r--r--  2.0 unx     6822 b- defN 24-May-24 01:00 sbcli_mc-1.0.1/simplyblock_core/services/storage_node_monitor.py
--rw-r--r--  2.0 unx     2428 b- defN 24-May-24 01:00 sbcli_mc-1.0.1/simplyblock_core/services/port_stat_collector.py
--rw-r--r--  2.0 unx     5146 b- defN 24-May-24 01:00 sbcli_mc-1.0.1/simplyblock_core/services/distr_event_collector.py
--rw-r--r--  2.0 unx      173 b- defN 24-May-24 01:00 sbcli_mc-1.0.1/simplyblock_core/services/remove_service.sh
--rw-r--r--  2.0 unx     3003 b- defN 24-May-24 01:00 sbcli_mc-1.0.1/simplyblock_core/services/mgmt_node_monitor.py
--rw-r--r--  2.0 unx     2189 b- defN 24-May-24 01:00 sbcli_mc-1.0.1/simplyblock_core/services/lvol_monitor.py
--rw-r--r--  2.0 unx    10594 b- defN 24-May-24 01:00 sbcli_mc-1.0.1/simplyblock_core/controllers/pool_controller.py
--rw-r--r--  2.0 unx        0 b- defN 24-May-24 01:00 sbcli_mc-1.0.1/simplyblock_core/controllers/__init__.py
--rw-r--r--  2.0 unx     1521 b- defN 24-May-24 01:00 sbcli_mc-1.0.1/simplyblock_core/controllers/storage_events.py
--rw-r--r--  2.0 unx    49032 b- defN 24-May-24 01:00 sbcli_mc-1.0.1/simplyblock_core/controllers/lvol_controller.py
--rw-r--r--  2.0 unx     1568 b- defN 24-May-24 01:00 sbcli_mc-1.0.1/simplyblock_core/controllers/device_events.py
--rw-r--r--  2.0 unx     1630 b- defN 24-May-24 01:00 sbcli_mc-1.0.1/simplyblock_core/controllers/lvol_events.py
--rw-r--r--  2.0 unx    10598 b- defN 24-May-24 01:00 sbcli_mc-1.0.1/simplyblock_core/controllers/snapshot_controller.py
--rw-r--r--  2.0 unx     1122 b- defN 24-May-24 01:00 sbcli_mc-1.0.1/simplyblock_core/controllers/snapshot_events.py
--rw-r--r--  2.0 unx     3191 b- defN 24-May-24 01:00 sbcli_mc-1.0.1/simplyblock_core/controllers/events_controller.py
--rw-r--r--  2.0 unx    10890 b- defN 24-May-24 01:00 sbcli_mc-1.0.1/simplyblock_core/controllers/health_controller.py
--rw-r--r--  2.0 unx    13932 b- defN 24-May-24 01:00 sbcli_mc-1.0.1/simplyblock_core/controllers/device_controller.py
--rw-r--r--  2.0 unx      695 b- defN 24-May-24 01:00 sbcli_mc-1.0.1/simplyblock_core/controllers/pool_events.py
--rw-r--r--  2.0 unx    23440 b- defN 24-May-24 01:00 sbcli_mc-1.0.1/simplyblock_core/controllers/caching_node_controller.py
--rw-r--r--  2.0 unx     1900 b- defN 24-May-24 01:00 sbcli_mc-1.0.1/simplyblock_core/controllers/cluster_events.py
--rw-r--r--  2.0 unx     1120 b- defN 24-May-24 01:00 sbcli_mc-1.0.1/simplyblock_core/controllers/mgmt_events.py
--rw-r--r--  2.0 unx     3766 b- defN 24-May-24 01:00 sbcli_mc-1.0.1/simplyblock_core/models/caching_node.py
--rw-r--r--  2.0 unx     2094 b- defN 24-May-24 01:00 sbcli_mc-1.0.1/simplyblock_core/models/nvme_device.py
--rw-r--r--  2.0 unx     1466 b- defN 24-May-24 01:00 sbcli_mc-1.0.1/simplyblock_core/models/mgmt_node.py
--rw-r--r--  2.0 unx      917 b- defN 24-May-24 01:00 sbcli_mc-1.0.1/simplyblock_core/models/compute_node.py
--rw-r--r--  2.0 unx        0 b- defN 24-May-24 01:00 sbcli_mc-1.0.1/simplyblock_core/models/__init__.py
--rw-r--r--  2.0 unx     1500 b- defN 24-May-24 01:00 sbcli_mc-1.0.1/simplyblock_core/models/events.py
--rw-r--r--  2.0 unx     1228 b- defN 24-May-24 01:00 sbcli_mc-1.0.1/simplyblock_core/models/global_settings.py
--rw-r--r--  2.0 unx      973 b- defN 24-May-24 01:00 sbcli_mc-1.0.1/simplyblock_core/models/job_schedule.py
--rw-r--r--  2.0 unx     4846 b- defN 24-May-24 01:00 sbcli_mc-1.0.1/simplyblock_core/models/base_model.py
--rw-r--r--  2.0 unx     2579 b- defN 24-May-24 01:00 sbcli_mc-1.0.1/simplyblock_core/models/lvol_model.py
--rw-r--r--  2.0 unx      736 b- defN 24-May-24 01:00 sbcli_mc-1.0.1/simplyblock_core/models/snapshot.py
--rw-r--r--  2.0 unx     3696 b- defN 24-May-24 01:00 sbcli_mc-1.0.1/simplyblock_core/models/storage_node.py
--rw-r--r--  2.0 unx     4242 b- defN 24-May-24 01:00 sbcli_mc-1.0.1/simplyblock_core/models/stats.py
--rw-r--r--  2.0 unx     1602 b- defN 24-May-24 01:00 sbcli_mc-1.0.1/simplyblock_core/models/pool.py
--rw-r--r--  2.0 unx      806 b- defN 24-May-24 01:00 sbcli_mc-1.0.1/simplyblock_core/models/iface.py
--rw-r--r--  2.0 unx     2565 b- defN 24-May-24 01:00 sbcli_mc-1.0.1/simplyblock_core/models/cluster.py
--rw-r--r--  2.0 unx     1020 b- defN 24-May-24 01:00 sbcli_mc-1.0.1/simplyblock_core/models/port_stat.py
-drwxr-xr-x  2.0 unx        0 b- stor 24-May-24 01:01 sbcli_mc-1.0.1/simplyblock_core/scripts/alerting/
-drwxr-xr-x  2.0 unx        0 b- stor 24-May-24 01:01 sbcli_mc-1.0.1/simplyblock_core/scripts/dashboards/
--rw-r--r--  2.0 unx     1420 b- defN 24-May-24 01:00 sbcli_mc-1.0.1/simplyblock_core/scripts/install_deps.sh
--rw-r--r--  2.0 unx     1782 b- defN 24-May-24 01:00 sbcli_mc-1.0.1/simplyblock_core/scripts/__init__.py
--rw-r--r--  2.0 unx       43 b- defN 24-May-24 01:00 sbcli_mc-1.0.1/simplyblock_core/scripts/run_ssh.sh
--rw-r--r--  2.0 unx     1163 b- defN 24-May-24 01:00 sbcli_mc-1.0.1/simplyblock_core/scripts/haproxy.cfg
--rw-r--r--  2.0 unx      118 b- defN 24-May-24 01:00 sbcli_mc-1.0.1/simplyblock_core/scripts/db_config_double.sh
--rw-r--r--  2.0 unx     5305 b- defN 24-May-24 01:00 sbcli_mc-1.0.1/simplyblock_core/scripts/stack_deploy_wait.sh
--rw-r--r--  2.0 unx      360 b- defN 24-May-24 01:00 sbcli_mc-1.0.1/simplyblock_core/scripts/datasource.yml
--rw-r--r--  2.0 unx     5611 b- defN 24-May-24 01:00 sbcli_mc-1.0.1/simplyblock_core/scripts/docker-compose-swarm.yml
--rw-r--r--  2.0 unx      152 b- defN 24-May-24 01:00 sbcli_mc-1.0.1/simplyblock_core/scripts/set_db_config.sh
--rwxr-xr-x  2.0 unx      657 b- defN 24-May-24 01:00 sbcli_mc-1.0.1/simplyblock_core/scripts/apply_dashboard.sh
--rw-r--r--  2.0 unx      311 b- defN 24-May-24 01:00 sbcli_mc-1.0.1/simplyblock_core/scripts/prometheus.yml
--rw-r--r--  2.0 unx      311 b- defN 24-May-24 01:00 sbcli_mc-1.0.1/simplyblock_core/scripts/clean_local_storage_deploy.sh
--rw-r--r--  2.0 unx     4409 b- defN 24-May-24 01:00 sbcli_mc-1.0.1/simplyblock_core/scripts/docker-compose-swarm-monitoring.yml
--rw-r--r--  2.0 unx      930 b- defN 24-May-24 01:00 sbcli_mc-1.0.1/simplyblock_core/scripts/deploy_stack.sh
--rw-r--r--  2.0 unx       54 b- defN 24-May-24 01:00 sbcli_mc-1.0.1/simplyblock_core/scripts/db_config_single.sh
--rw-r--r--  2.0 unx      453 b- defN 24-May-24 01:00 sbcli_mc-1.0.1/simplyblock_core/scripts/config_docker.sh
--rw-r--r--  2.0 unx    25433 b- defN 24-May-24 01:00 sbcli_mc-1.0.1/simplyblock_core/scripts/alerting/alert_rules.yaml
--rw-r--r--  2.0 unx     1856 b- defN 24-May-24 01:00 sbcli_mc-1.0.1/simplyblock_core/scripts/alerting/alert_resources.yaml
--rw-r--r--  2.0 unx    88820 b- defN 24-May-24 01:00 sbcli_mc-1.0.1/simplyblock_core/scripts/dashboards/nodes.json
--rw-r--r--  2.0 unx    88911 b- defN 24-May-24 01:00 sbcli_mc-1.0.1/simplyblock_core/scripts/dashboards/cluster.json
--rw-r--r--  2.0 unx    88776 b- defN 24-May-24 01:00 sbcli_mc-1.0.1/simplyblock_core/scripts/dashboards/lvols.json
--rw-r--r--  2.0 unx    88868 b- defN 24-May-24 01:00 sbcli_mc-1.0.1/simplyblock_core/scripts/dashboards/devices.json
--rw-r--r--  2.0 unx    99707 b- defN 24-May-24 01:00 sbcli_mc-1.0.1/simplyblock_core/scripts/dashboards/pools.json
--rw-r--r--  2.0 unx   799409 b- defN 24-May-24 01:00 sbcli_mc-1.0.1/simplyblock_core/scripts/dashboards/node-exporter.json
--rw-r--r--  2.0 unx     5261 b- defN 24-May-24 01:01 sbcli_mc-1.0.1/sbcli_mc.egg-info/SOURCES.txt
--rw-r--r--  2.0 unx       73 b- defN 24-May-24 01:01 sbcli_mc-1.0.1/sbcli_mc.egg-info/requires.txt
--rw-r--r--  2.0 unx     1488 b- defN 24-May-24 01:01 sbcli_mc-1.0.1/sbcli_mc.egg-info/PKG-INFO
--rw-r--r--  2.0 unx       49 b- defN 24-May-24 01:01 sbcli_mc-1.0.1/sbcli_mc.egg-info/top_level.txt
--rw-r--r--  2.0 unx       54 b- defN 24-May-24 01:01 sbcli_mc-1.0.1/sbcli_mc.egg-info/entry_points.txt
--rw-r--r--  2.0 unx        1 b- defN 24-May-24 01:01 sbcli_mc-1.0.1/sbcli_mc.egg-info/dependency_links.txt
-148 files, 1891326 bytes uncompressed, 189181 bytes compressed:  90.0%
+Zip file size: 212499 bytes, number of entries: 148
+drwxr-xr-x  2.0 unx        0 b- stor 24-May-29 02:25 sbcli_mc-1.0.2/
+drwxr-xr-x  2.0 unx        0 b- stor 24-May-29 02:25 sbcli_mc-1.0.2/simplyblock_cli/
+drwxr-xr-x  2.0 unx        0 b- stor 24-May-29 02:25 sbcli_mc-1.0.2/simplyblock_web/
+drwxr-xr-x  2.0 unx        0 b- stor 24-May-29 02:25 sbcli_mc-1.0.2/simplyblock_core/
+drwxr-xr-x  2.0 unx        0 b- stor 24-May-29 02:25 sbcli_mc-1.0.2/sbcli_mc.egg-info/
+-rw-r--r--  2.0 unx     1068 b- defN 24-May-29 02:25 sbcli_mc-1.0.2/README.md
+-rw-r--r--  2.0 unx       84 b- defN 24-May-29 02:25 sbcli_mc-1.0.2/pyproject.toml
+-rw-r--r--  2.0 unx     1488 b- defN 24-May-29 02:25 sbcli_mc-1.0.2/PKG-INFO
+-rw-r--r--  2.0 unx      157 b- defN 24-May-29 02:25 sbcli_mc-1.0.2/env_var
+-rw-r--r--  2.0 unx       38 b- defN 24-May-29 02:25 sbcli_mc-1.0.2/setup.cfg
+-rw-r--r--  2.0 unx     2269 b- defN 24-May-29 02:25 sbcli_mc-1.0.2/setup.py
+-rw-r--r--  2.0 unx    64564 b- defN 24-May-29 02:25 sbcli_mc-1.0.2/simplyblock_cli/cli.py
+-rw-r--r--  2.0 unx      357 b- defN 24-May-29 02:25 sbcli_mc-1.0.2/simplyblock_cli/main.py
+drwxr-xr-x  2.0 unx        0 b- stor 24-May-29 02:25 sbcli_mc-1.0.2/simplyblock_web/static/
+drwxr-xr-x  2.0 unx        0 b- stor 24-May-29 02:25 sbcli_mc-1.0.2/simplyblock_web/blueprints/
+drwxr-xr-x  2.0 unx        0 b- stor 24-May-29 02:25 sbcli_mc-1.0.2/simplyblock_web/templates/
+-rw-r--r--  2.0 unx        0 b- defN 24-May-29 02:25 sbcli_mc-1.0.2/simplyblock_web/__init__.py
+-rw-r--r--  2.0 unx     1434 b- defN 24-May-29 02:25 sbcli_mc-1.0.2/simplyblock_web/node_webapp.py
+-rw-r--r--  2.0 unx      703 b- defN 24-May-29 02:25 sbcli_mc-1.0.2/simplyblock_web/snode_app.py
+-rw-r--r--  2.0 unx      717 b- defN 24-May-29 02:25 sbcli_mc-1.0.2/simplyblock_web/caching_node_app.py
+-rw-r--r--  2.0 unx     1638 b- defN 24-May-29 02:25 sbcli_mc-1.0.2/simplyblock_web/auth_middleware.py
+-rw-r--r--  2.0 unx     5098 b- defN 24-May-29 02:25 sbcli_mc-1.0.2/simplyblock_web/node_utils.py
+-rw-r--r--  2.0 unx     2715 b- defN 24-May-29 02:25 sbcli_mc-1.0.2/simplyblock_web/utils.py
+-rw-r--r--  2.0 unx     1284 b- defN 24-May-29 02:25 sbcli_mc-1.0.2/simplyblock_web/app.py
+-rw-r--r--  2.0 unx      725 b- defN 24-May-29 02:25 sbcli_mc-1.0.2/simplyblock_web/caching_node_app_k8s.py
+-rw-r--r--  2.0 unx      322 b- defN 24-May-29 02:25 sbcli_mc-1.0.2/simplyblock_web/static/tst.py
+-rw-r--r--  2.0 unx      827 b- defN 24-May-29 02:25 sbcli_mc-1.0.2/simplyblock_web/static/delete.py
+-rw-r--r--  2.0 unx      507 b- defN 24-May-29 02:25 sbcli_mc-1.0.2/simplyblock_web/static/deploy_cnode.yaml
+-rw-r--r--  2.0 unx      434 b- defN 24-May-29 02:25 sbcli_mc-1.0.2/simplyblock_web/static/is_up.py
+-rw-r--r--  2.0 unx     1466 b- defN 24-May-29 02:25 sbcli_mc-1.0.2/simplyblock_web/static/deploy_spdk.yaml
+-rw-r--r--  2.0 unx      463 b- defN 24-May-29 02:25 sbcli_mc-1.0.2/simplyblock_web/static/rpac.yaml
+-rw-r--r--  2.0 unx      417 b- defN 24-May-29 02:25 sbcli_mc-1.0.2/simplyblock_web/static/list_deps.py
+-rw-r--r--  2.0 unx     1302 b- defN 24-May-29 02:25 sbcli_mc-1.0.2/simplyblock_web/static/deploy.py
+-rw-r--r--  2.0 unx     6806 b- defN 24-May-29 02:25 sbcli_mc-1.0.2/simplyblock_web/blueprints/web_api_pool.py
+-rw-r--r--  2.0 unx        0 b- defN 24-May-29 02:25 sbcli_mc-1.0.2/simplyblock_web/blueprints/__init__.py
+-rw-r--r--  2.0 unx     3118 b- defN 24-May-29 02:25 sbcli_mc-1.0.2/simplyblock_web/blueprints/web_api_device.py
+-rw-r--r--  2.0 unx     8685 b- defN 24-May-29 02:25 sbcli_mc-1.0.2/simplyblock_web/blueprints/web_api_lvol.py
+-rw-r--r--  2.0 unx     9713 b- defN 24-May-29 02:25 sbcli_mc-1.0.2/simplyblock_web/blueprints/snode_ops.py
+-rw-r--r--  2.0 unx    12385 b- defN 24-May-29 02:25 sbcli_mc-1.0.2/simplyblock_web/blueprints/caching_node_ops.py
+-rw-r--r--  2.0 unx     6401 b- defN 24-May-29 02:25 sbcli_mc-1.0.2/simplyblock_web/blueprints/web_api_storage_node.py
+-rw-r--r--  2.0 unx     5931 b- defN 24-May-29 02:25 sbcli_mc-1.0.2/simplyblock_web/blueprints/web_api_cluster.py
+-rw-r--r--  2.0 unx     8075 b- defN 24-May-29 02:25 sbcli_mc-1.0.2/simplyblock_web/blueprints/caching_node_ops_k8s.py
+-rw-r--r--  2.0 unx     4883 b- defN 24-May-29 02:25 sbcli_mc-1.0.2/simplyblock_web/blueprints/node_api_caching_ks.py
+-rw-r--r--  2.0 unx     5746 b- defN 24-May-29 02:25 sbcli_mc-1.0.2/simplyblock_web/blueprints/node_api_caching_docker.py
+-rw-r--r--  2.0 unx     5491 b- defN 24-May-29 02:25 sbcli_mc-1.0.2/simplyblock_web/blueprints/web_api_caching_node.py
+-rw-r--r--  2.0 unx     3103 b- defN 24-May-29 02:25 sbcli_mc-1.0.2/simplyblock_web/blueprints/node_api_basic.py
+-rw-r--r--  2.0 unx    11244 b- defN 24-May-29 02:25 sbcli_mc-1.0.2/simplyblock_web/blueprints/csi.py
+-rw-r--r--  2.0 unx      975 b- defN 24-May-29 02:25 sbcli_mc-1.0.2/simplyblock_web/blueprints/web_api_mgmt_node.py
+-rw-r--r--  2.0 unx     2905 b- defN 24-May-29 02:25 sbcli_mc-1.0.2/simplyblock_web/templates/deploy_spdk.yaml.j2
+drwxr-xr-x  2.0 unx        0 b- stor 24-May-29 02:25 sbcli_mc-1.0.2/simplyblock_core/services/
+drwxr-xr-x  2.0 unx        0 b- stor 24-May-29 02:25 sbcli_mc-1.0.2/simplyblock_core/controllers/
+drwxr-xr-x  2.0 unx        0 b- stor 24-May-29 02:25 sbcli_mc-1.0.2/simplyblock_core/models/
+drwxr-xr-x  2.0 unx        0 b- stor 24-May-29 02:25 sbcli_mc-1.0.2/simplyblock_core/scripts/
+-rw-r--r--  2.0 unx    25885 b- defN 24-May-29 02:25 sbcli_mc-1.0.2/simplyblock_core/cluster_ops.py
+-rw-r--r--  2.0 unx      938 b- defN 24-May-29 02:25 sbcli_mc-1.0.2/simplyblock_core/pci_utils.py
+-rw-r--r--  2.0 unx        0 b- defN 24-May-29 02:25 sbcli_mc-1.0.2/simplyblock_core/__init__.py
+-rw-r--r--  2.0 unx     3193 b- defN 24-May-29 02:25 sbcli_mc-1.0.2/simplyblock_core/snode_client.py
+-rw-r--r--  2.0 unx     8799 b- defN 24-May-29 02:25 sbcli_mc-1.0.2/simplyblock_core/kv_store.py
+-rw-r--r--  2.0 unx     5112 b- defN 24-May-29 02:25 sbcli_mc-1.0.2/simplyblock_core/compute_node_ops.py
+-rw-r--r--  2.0 unx    20829 b- defN 24-May-29 02:25 sbcli_mc-1.0.2/simplyblock_core/rpc_client.py
+-rw-r--r--  2.0 unx     1986 b- defN 24-May-29 02:25 sbcli_mc-1.0.2/simplyblock_core/mgmt_node_ops.py
+-rw-r--r--  2.0 unx     7640 b- defN 24-May-29 02:25 sbcli_mc-1.0.2/simplyblock_core/utils.py
+-rw-r--r--  2.0 unx     7725 b- defN 24-May-29 02:25 sbcli_mc-1.0.2/simplyblock_core/distr_controller.py
+-rw-r--r--  2.0 unx      279 b- defN 24-May-29 02:25 sbcli_mc-1.0.2/simplyblock_core/shell_utils.py
+-rw-r--r--  2.0 unx     3638 b- defN 24-May-29 02:25 sbcli_mc-1.0.2/simplyblock_core/cnode_client.py
+-rw-r--r--  2.0 unx    65242 b- defN 24-May-29 02:25 sbcli_mc-1.0.2/simplyblock_core/storage_node_ops.py
+-rw-r--r--  2.0 unx     1575 b- defN 24-May-29 02:25 sbcli_mc-1.0.2/simplyblock_core/constants.py
+-rw-r--r--  2.0 unx     3542 b- defN 24-May-29 02:25 sbcli_mc-1.0.2/simplyblock_core/services/job_tasks.py
+-rw-r--r--  2.0 unx     3203 b- defN 24-May-29 02:25 sbcli_mc-1.0.2/simplyblock_core/services/caching_node_monitor.py
+-rw-r--r--  2.0 unx      229 b- defN 24-May-29 02:25 sbcli_mc-1.0.2/simplyblock_core/services/service_template.service
+-rw-r--r--  2.0 unx      837 b- defN 24-May-29 02:25 sbcli_mc-1.0.2/simplyblock_core/services/install_service.sh
+-rw-r--r--  2.0 unx     4118 b- defN 24-May-29 02:25 sbcli_mc-1.0.2/simplyblock_core/services/__init__.py
+-rw-r--r--  2.0 unx     2410 b- defN 24-May-29 02:25 sbcli_mc-1.0.2/simplyblock_core/services/log_agg_service.py
+-rw-r--r--  2.0 unx     5751 b- defN 24-May-29 02:25 sbcli_mc-1.0.2/simplyblock_core/services/health_check_service.py
+-rw-r--r--  2.0 unx     7439 b- defN 24-May-29 02:25 sbcli_mc-1.0.2/simplyblock_core/services/capacity_and_stats_collector.py
+-rw-r--r--  2.0 unx     3169 b- defN 24-May-29 02:25 sbcli_mc-1.0.2/simplyblock_core/services/device_monitor.py
+-rw-r--r--  2.0 unx     5268 b- defN 24-May-29 02:25 sbcli_mc-1.0.2/simplyblock_core/services/lvol_stat_collector.py
+-rw-r--r--  2.0 unx     2671 b- defN 24-May-29 02:25 sbcli_mc-1.0.2/simplyblock_core/services/cap_monitor.py
+-rw-r--r--  2.0 unx     6822 b- defN 24-May-29 02:25 sbcli_mc-1.0.2/simplyblock_core/services/storage_node_monitor.py
+-rw-r--r--  2.0 unx     2428 b- defN 24-May-29 02:25 sbcli_mc-1.0.2/simplyblock_core/services/port_stat_collector.py
+-rw-r--r--  2.0 unx     5146 b- defN 24-May-29 02:25 sbcli_mc-1.0.2/simplyblock_core/services/distr_event_collector.py
+-rw-r--r--  2.0 unx      173 b- defN 24-May-29 02:25 sbcli_mc-1.0.2/simplyblock_core/services/remove_service.sh
+-rw-r--r--  2.0 unx     3003 b- defN 24-May-29 02:25 sbcli_mc-1.0.2/simplyblock_core/services/mgmt_node_monitor.py
+-rw-r--r--  2.0 unx     2189 b- defN 24-May-29 02:25 sbcli_mc-1.0.2/simplyblock_core/services/lvol_monitor.py
+-rw-r--r--  2.0 unx    10594 b- defN 24-May-29 02:25 sbcli_mc-1.0.2/simplyblock_core/controllers/pool_controller.py
+-rw-r--r--  2.0 unx        0 b- defN 24-May-29 02:25 sbcli_mc-1.0.2/simplyblock_core/controllers/__init__.py
+-rw-r--r--  2.0 unx     1521 b- defN 24-May-29 02:25 sbcli_mc-1.0.2/simplyblock_core/controllers/storage_events.py
+-rw-r--r--  2.0 unx    48560 b- defN 24-May-29 02:25 sbcli_mc-1.0.2/simplyblock_core/controllers/lvol_controller.py
+-rw-r--r--  2.0 unx     1568 b- defN 24-May-29 02:25 sbcli_mc-1.0.2/simplyblock_core/controllers/device_events.py
+-rw-r--r--  2.0 unx     1630 b- defN 24-May-29 02:25 sbcli_mc-1.0.2/simplyblock_core/controllers/lvol_events.py
+-rw-r--r--  2.0 unx    10874 b- defN 24-May-29 02:25 sbcli_mc-1.0.2/simplyblock_core/controllers/snapshot_controller.py
+-rw-r--r--  2.0 unx     1122 b- defN 24-May-29 02:25 sbcli_mc-1.0.2/simplyblock_core/controllers/snapshot_events.py
+-rw-r--r--  2.0 unx     3191 b- defN 24-May-29 02:25 sbcli_mc-1.0.2/simplyblock_core/controllers/events_controller.py
+-rw-r--r--  2.0 unx    10852 b- defN 24-May-29 02:25 sbcli_mc-1.0.2/simplyblock_core/controllers/health_controller.py
+-rw-r--r--  2.0 unx    13932 b- defN 24-May-29 02:25 sbcli_mc-1.0.2/simplyblock_core/controllers/device_controller.py
+-rw-r--r--  2.0 unx      695 b- defN 24-May-29 02:25 sbcli_mc-1.0.2/simplyblock_core/controllers/pool_events.py
+-rw-r--r--  2.0 unx    23440 b- defN 24-May-29 02:25 sbcli_mc-1.0.2/simplyblock_core/controllers/caching_node_controller.py
+-rw-r--r--  2.0 unx     1900 b- defN 24-May-29 02:25 sbcli_mc-1.0.2/simplyblock_core/controllers/cluster_events.py
+-rw-r--r--  2.0 unx     1120 b- defN 24-May-29 02:25 sbcli_mc-1.0.2/simplyblock_core/controllers/mgmt_events.py
+-rw-r--r--  2.0 unx     3766 b- defN 24-May-29 02:25 sbcli_mc-1.0.2/simplyblock_core/models/caching_node.py
+-rw-r--r--  2.0 unx     2094 b- defN 24-May-29 02:25 sbcli_mc-1.0.2/simplyblock_core/models/nvme_device.py
+-rw-r--r--  2.0 unx     1452 b- defN 24-May-29 02:25 sbcli_mc-1.0.2/simplyblock_core/models/mgmt_node.py
+-rw-r--r--  2.0 unx      917 b- defN 24-May-29 02:25 sbcli_mc-1.0.2/simplyblock_core/models/compute_node.py
+-rw-r--r--  2.0 unx        0 b- defN 24-May-29 02:25 sbcli_mc-1.0.2/simplyblock_core/models/__init__.py
+-rw-r--r--  2.0 unx     1500 b- defN 24-May-29 02:25 sbcli_mc-1.0.2/simplyblock_core/models/events.py
+-rw-r--r--  2.0 unx     1228 b- defN 24-May-29 02:25 sbcli_mc-1.0.2/simplyblock_core/models/global_settings.py
+-rw-r--r--  2.0 unx      973 b- defN 24-May-29 02:25 sbcli_mc-1.0.2/simplyblock_core/models/job_schedule.py
+-rw-r--r--  2.0 unx     4846 b- defN 24-May-29 02:25 sbcli_mc-1.0.2/simplyblock_core/models/base_model.py
+-rw-r--r--  2.0 unx     2579 b- defN 24-May-29 02:25 sbcli_mc-1.0.2/simplyblock_core/models/lvol_model.py
+-rw-r--r--  2.0 unx      736 b- defN 24-May-29 02:25 sbcli_mc-1.0.2/simplyblock_core/models/snapshot.py
+-rw-r--r--  2.0 unx     3696 b- defN 24-May-29 02:25 sbcli_mc-1.0.2/simplyblock_core/models/storage_node.py
+-rw-r--r--  2.0 unx     4242 b- defN 24-May-29 02:25 sbcli_mc-1.0.2/simplyblock_core/models/stats.py
+-rw-r--r--  2.0 unx     1602 b- defN 24-May-29 02:25 sbcli_mc-1.0.2/simplyblock_core/models/pool.py
+-rw-r--r--  2.0 unx      806 b- defN 24-May-29 02:25 sbcli_mc-1.0.2/simplyblock_core/models/iface.py
+-rw-r--r--  2.0 unx     2565 b- defN 24-May-29 02:25 sbcli_mc-1.0.2/simplyblock_core/models/cluster.py
+-rw-r--r--  2.0 unx     1020 b- defN 24-May-29 02:25 sbcli_mc-1.0.2/simplyblock_core/models/port_stat.py
+drwxr-xr-x  2.0 unx        0 b- stor 24-May-29 02:25 sbcli_mc-1.0.2/simplyblock_core/scripts/alerting/
+drwxr-xr-x  2.0 unx        0 b- stor 24-May-29 02:25 sbcli_mc-1.0.2/simplyblock_core/scripts/dashboards/
+-rw-r--r--  2.0 unx     1420 b- defN 24-May-29 02:25 sbcli_mc-1.0.2/simplyblock_core/scripts/install_deps.sh
+-rw-r--r--  2.0 unx     1782 b- defN 24-May-29 02:25 sbcli_mc-1.0.2/simplyblock_core/scripts/__init__.py
+-rw-r--r--  2.0 unx       43 b- defN 24-May-29 02:25 sbcli_mc-1.0.2/simplyblock_core/scripts/run_ssh.sh
+-rw-r--r--  2.0 unx     1163 b- defN 24-May-29 02:25 sbcli_mc-1.0.2/simplyblock_core/scripts/haproxy.cfg
+-rw-r--r--  2.0 unx      118 b- defN 24-May-29 02:25 sbcli_mc-1.0.2/simplyblock_core/scripts/db_config_double.sh
+-rw-r--r--  2.0 unx     5305 b- defN 24-May-29 02:25 sbcli_mc-1.0.2/simplyblock_core/scripts/stack_deploy_wait.sh
+-rw-r--r--  2.0 unx      360 b- defN 24-May-29 02:25 sbcli_mc-1.0.2/simplyblock_core/scripts/datasource.yml
+-rw-r--r--  2.0 unx     5611 b- defN 24-May-29 02:25 sbcli_mc-1.0.2/simplyblock_core/scripts/docker-compose-swarm.yml
+-rw-r--r--  2.0 unx      152 b- defN 24-May-29 02:25 sbcli_mc-1.0.2/simplyblock_core/scripts/set_db_config.sh
+-rwxr-xr-x  2.0 unx      657 b- defN 24-May-29 02:25 sbcli_mc-1.0.2/simplyblock_core/scripts/apply_dashboard.sh
+-rw-r--r--  2.0 unx      311 b- defN 24-May-29 02:25 sbcli_mc-1.0.2/simplyblock_core/scripts/prometheus.yml
+-rw-r--r--  2.0 unx      311 b- defN 24-May-29 02:25 sbcli_mc-1.0.2/simplyblock_core/scripts/clean_local_storage_deploy.sh
+-rw-r--r--  2.0 unx     4409 b- defN 24-May-29 02:25 sbcli_mc-1.0.2/simplyblock_core/scripts/docker-compose-swarm-monitoring.yml
+-rw-r--r--  2.0 unx      930 b- defN 24-May-29 02:25 sbcli_mc-1.0.2/simplyblock_core/scripts/deploy_stack.sh
+-rw-r--r--  2.0 unx       54 b- defN 24-May-29 02:25 sbcli_mc-1.0.2/simplyblock_core/scripts/db_config_single.sh
+-rw-r--r--  2.0 unx      453 b- defN 24-May-29 02:25 sbcli_mc-1.0.2/simplyblock_core/scripts/config_docker.sh
+-rw-r--r--  2.0 unx    25433 b- defN 24-May-29 02:25 sbcli_mc-1.0.2/simplyblock_core/scripts/alerting/alert_rules.yaml
+-rw-r--r--  2.0 unx     1856 b- defN 24-May-29 02:25 sbcli_mc-1.0.2/simplyblock_core/scripts/alerting/alert_resources.yaml
+-rw-r--r--  2.0 unx    88820 b- defN 24-May-29 02:25 sbcli_mc-1.0.2/simplyblock_core/scripts/dashboards/nodes.json
+-rw-r--r--  2.0 unx    88911 b- defN 24-May-29 02:25 sbcli_mc-1.0.2/simplyblock_core/scripts/dashboards/cluster.json
+-rw-r--r--  2.0 unx    88776 b- defN 24-May-29 02:25 sbcli_mc-1.0.2/simplyblock_core/scripts/dashboards/lvols.json
+-rw-r--r--  2.0 unx    88868 b- defN 24-May-29 02:25 sbcli_mc-1.0.2/simplyblock_core/scripts/dashboards/devices.json
+-rw-r--r--  2.0 unx    99707 b- defN 24-May-29 02:25 sbcli_mc-1.0.2/simplyblock_core/scripts/dashboards/pools.json
+-rw-r--r--  2.0 unx   799409 b- defN 24-May-29 02:25 sbcli_mc-1.0.2/simplyblock_core/scripts/dashboards/node-exporter.json
+-rw-r--r--  2.0 unx     5261 b- defN 24-May-29 02:25 sbcli_mc-1.0.2/sbcli_mc.egg-info/SOURCES.txt
+-rw-r--r--  2.0 unx       73 b- defN 24-May-29 02:25 sbcli_mc-1.0.2/sbcli_mc.egg-info/requires.txt
+-rw-r--r--  2.0 unx     1488 b- defN 24-May-29 02:25 sbcli_mc-1.0.2/sbcli_mc.egg-info/PKG-INFO
+-rw-r--r--  2.0 unx       49 b- defN 24-May-29 02:25 sbcli_mc-1.0.2/sbcli_mc.egg-info/top_level.txt
+-rw-r--r--  2.0 unx       54 b- defN 24-May-29 02:25 sbcli_mc-1.0.2/sbcli_mc.egg-info/entry_points.txt
+-rw-r--r--  2.0 unx        1 b- defN 24-May-29 02:25 sbcli_mc-1.0.2/sbcli_mc.egg-info/dependency_links.txt
+148 files, 1873583 bytes uncompressed, 185861 bytes compressed:  90.1%
```

## zipnote {}

```diff
@@ -1,445 +1,445 @@
-Filename: sbcli_mc-1.0.1/
+Filename: sbcli_mc-1.0.2/
 Comment: 
 
-Filename: sbcli_mc-1.0.1/simplyblock_cli/
+Filename: sbcli_mc-1.0.2/simplyblock_cli/
 Comment: 
 
-Filename: sbcli_mc-1.0.1/simplyblock_web/
+Filename: sbcli_mc-1.0.2/simplyblock_web/
 Comment: 
 
-Filename: sbcli_mc-1.0.1/simplyblock_core/
+Filename: sbcli_mc-1.0.2/simplyblock_core/
 Comment: 
 
-Filename: sbcli_mc-1.0.1/sbcli_mc.egg-info/
+Filename: sbcli_mc-1.0.2/sbcli_mc.egg-info/
 Comment: 
 
-Filename: sbcli_mc-1.0.1/README.md
+Filename: sbcli_mc-1.0.2/README.md
 Comment: 
 
-Filename: sbcli_mc-1.0.1/pyproject.toml
+Filename: sbcli_mc-1.0.2/pyproject.toml
 Comment: 
 
-Filename: sbcli_mc-1.0.1/PKG-INFO
+Filename: sbcli_mc-1.0.2/PKG-INFO
 Comment: 
 
-Filename: sbcli_mc-1.0.1/env_var
+Filename: sbcli_mc-1.0.2/env_var
 Comment: 
 
-Filename: sbcli_mc-1.0.1/setup.cfg
+Filename: sbcli_mc-1.0.2/setup.cfg
 Comment: 
 
-Filename: sbcli_mc-1.0.1/setup.py
+Filename: sbcli_mc-1.0.2/setup.py
 Comment: 
 
-Filename: sbcli_mc-1.0.1/simplyblock_cli/cli.py
+Filename: sbcli_mc-1.0.2/simplyblock_cli/cli.py
 Comment: 
 
-Filename: sbcli_mc-1.0.1/simplyblock_cli/main.py
+Filename: sbcli_mc-1.0.2/simplyblock_cli/main.py
 Comment: 
 
-Filename: sbcli_mc-1.0.1/simplyblock_web/static/
+Filename: sbcli_mc-1.0.2/simplyblock_web/static/
 Comment: 
 
-Filename: sbcli_mc-1.0.1/simplyblock_web/blueprints/
+Filename: sbcli_mc-1.0.2/simplyblock_web/blueprints/
 Comment: 
 
-Filename: sbcli_mc-1.0.1/simplyblock_web/templates/
+Filename: sbcli_mc-1.0.2/simplyblock_web/templates/
 Comment: 
 
-Filename: sbcli_mc-1.0.1/simplyblock_web/__init__.py
+Filename: sbcli_mc-1.0.2/simplyblock_web/__init__.py
 Comment: 
 
-Filename: sbcli_mc-1.0.1/simplyblock_web/node_webapp.py
+Filename: sbcli_mc-1.0.2/simplyblock_web/node_webapp.py
 Comment: 
 
-Filename: sbcli_mc-1.0.1/simplyblock_web/snode_app.py
+Filename: sbcli_mc-1.0.2/simplyblock_web/snode_app.py
 Comment: 
 
-Filename: sbcli_mc-1.0.1/simplyblock_web/caching_node_app.py
+Filename: sbcli_mc-1.0.2/simplyblock_web/caching_node_app.py
 Comment: 
 
-Filename: sbcli_mc-1.0.1/simplyblock_web/auth_middleware.py
+Filename: sbcli_mc-1.0.2/simplyblock_web/auth_middleware.py
 Comment: 
 
-Filename: sbcli_mc-1.0.1/simplyblock_web/node_utils.py
+Filename: sbcli_mc-1.0.2/simplyblock_web/node_utils.py
 Comment: 
 
-Filename: sbcli_mc-1.0.1/simplyblock_web/utils.py
+Filename: sbcli_mc-1.0.2/simplyblock_web/utils.py
 Comment: 
 
-Filename: sbcli_mc-1.0.1/simplyblock_web/app.py
+Filename: sbcli_mc-1.0.2/simplyblock_web/app.py
 Comment: 
 
-Filename: sbcli_mc-1.0.1/simplyblock_web/caching_node_app_k8s.py
+Filename: sbcli_mc-1.0.2/simplyblock_web/caching_node_app_k8s.py
 Comment: 
 
-Filename: sbcli_mc-1.0.1/simplyblock_web/static/tst.py
+Filename: sbcli_mc-1.0.2/simplyblock_web/static/tst.py
 Comment: 
 
-Filename: sbcli_mc-1.0.1/simplyblock_web/static/delete.py
+Filename: sbcli_mc-1.0.2/simplyblock_web/static/delete.py
 Comment: 
 
-Filename: sbcli_mc-1.0.1/simplyblock_web/static/deploy_cnode.yaml
+Filename: sbcli_mc-1.0.2/simplyblock_web/static/deploy_cnode.yaml
 Comment: 
 
-Filename: sbcli_mc-1.0.1/simplyblock_web/static/is_up.py
+Filename: sbcli_mc-1.0.2/simplyblock_web/static/is_up.py
 Comment: 
 
-Filename: sbcli_mc-1.0.1/simplyblock_web/static/deploy_spdk.yaml
+Filename: sbcli_mc-1.0.2/simplyblock_web/static/deploy_spdk.yaml
 Comment: 
 
-Filename: sbcli_mc-1.0.1/simplyblock_web/static/rpac.yaml
+Filename: sbcli_mc-1.0.2/simplyblock_web/static/rpac.yaml
 Comment: 
 
-Filename: sbcli_mc-1.0.1/simplyblock_web/static/list_deps.py
+Filename: sbcli_mc-1.0.2/simplyblock_web/static/list_deps.py
 Comment: 
 
-Filename: sbcli_mc-1.0.1/simplyblock_web/static/deploy.py
+Filename: sbcli_mc-1.0.2/simplyblock_web/static/deploy.py
 Comment: 
 
-Filename: sbcli_mc-1.0.1/simplyblock_web/blueprints/web_api_pool.py
+Filename: sbcli_mc-1.0.2/simplyblock_web/blueprints/web_api_pool.py
 Comment: 
 
-Filename: sbcli_mc-1.0.1/simplyblock_web/blueprints/__init__.py
+Filename: sbcli_mc-1.0.2/simplyblock_web/blueprints/__init__.py
 Comment: 
 
-Filename: sbcli_mc-1.0.1/simplyblock_web/blueprints/web_api_device.py
+Filename: sbcli_mc-1.0.2/simplyblock_web/blueprints/web_api_device.py
 Comment: 
 
-Filename: sbcli_mc-1.0.1/simplyblock_web/blueprints/web_api_lvol.py
+Filename: sbcli_mc-1.0.2/simplyblock_web/blueprints/web_api_lvol.py
 Comment: 
 
-Filename: sbcli_mc-1.0.1/simplyblock_web/blueprints/snode_ops.py
+Filename: sbcli_mc-1.0.2/simplyblock_web/blueprints/snode_ops.py
 Comment: 
 
-Filename: sbcli_mc-1.0.1/simplyblock_web/blueprints/caching_node_ops.py
+Filename: sbcli_mc-1.0.2/simplyblock_web/blueprints/caching_node_ops.py
 Comment: 
 
-Filename: sbcli_mc-1.0.1/simplyblock_web/blueprints/web_api_storage_node.py
+Filename: sbcli_mc-1.0.2/simplyblock_web/blueprints/web_api_storage_node.py
 Comment: 
 
-Filename: sbcli_mc-1.0.1/simplyblock_web/blueprints/web_api_cluster.py
+Filename: sbcli_mc-1.0.2/simplyblock_web/blueprints/web_api_cluster.py
 Comment: 
 
-Filename: sbcli_mc-1.0.1/simplyblock_web/blueprints/caching_node_ops_k8s.py
+Filename: sbcli_mc-1.0.2/simplyblock_web/blueprints/caching_node_ops_k8s.py
 Comment: 
 
-Filename: sbcli_mc-1.0.1/simplyblock_web/blueprints/node_api_caching_ks.py
+Filename: sbcli_mc-1.0.2/simplyblock_web/blueprints/node_api_caching_ks.py
 Comment: 
 
-Filename: sbcli_mc-1.0.1/simplyblock_web/blueprints/node_api_caching_docker.py
+Filename: sbcli_mc-1.0.2/simplyblock_web/blueprints/node_api_caching_docker.py
 Comment: 
 
-Filename: sbcli_mc-1.0.1/simplyblock_web/blueprints/web_api_caching_node.py
+Filename: sbcli_mc-1.0.2/simplyblock_web/blueprints/web_api_caching_node.py
 Comment: 
 
-Filename: sbcli_mc-1.0.1/simplyblock_web/blueprints/node_api_basic.py
+Filename: sbcli_mc-1.0.2/simplyblock_web/blueprints/node_api_basic.py
 Comment: 
 
-Filename: sbcli_mc-1.0.1/simplyblock_web/blueprints/csi.py
+Filename: sbcli_mc-1.0.2/simplyblock_web/blueprints/csi.py
 Comment: 
 
-Filename: sbcli_mc-1.0.1/simplyblock_web/blueprints/web_api_mgmt_node.py
+Filename: sbcli_mc-1.0.2/simplyblock_web/blueprints/web_api_mgmt_node.py
 Comment: 
 
-Filename: sbcli_mc-1.0.1/simplyblock_web/templates/deploy_spdk.yaml.j2
+Filename: sbcli_mc-1.0.2/simplyblock_web/templates/deploy_spdk.yaml.j2
 Comment: 
 
-Filename: sbcli_mc-1.0.1/simplyblock_core/services/
+Filename: sbcli_mc-1.0.2/simplyblock_core/services/
 Comment: 
 
-Filename: sbcli_mc-1.0.1/simplyblock_core/controllers/
+Filename: sbcli_mc-1.0.2/simplyblock_core/controllers/
 Comment: 
 
-Filename: sbcli_mc-1.0.1/simplyblock_core/models/
+Filename: sbcli_mc-1.0.2/simplyblock_core/models/
 Comment: 
 
-Filename: sbcli_mc-1.0.1/simplyblock_core/scripts/
+Filename: sbcli_mc-1.0.2/simplyblock_core/scripts/
 Comment: 
 
-Filename: sbcli_mc-1.0.1/simplyblock_core/cluster_ops.py
+Filename: sbcli_mc-1.0.2/simplyblock_core/cluster_ops.py
 Comment: 
 
-Filename: sbcli_mc-1.0.1/simplyblock_core/pci_utils.py
+Filename: sbcli_mc-1.0.2/simplyblock_core/pci_utils.py
 Comment: 
 
-Filename: sbcli_mc-1.0.1/simplyblock_core/__init__.py
+Filename: sbcli_mc-1.0.2/simplyblock_core/__init__.py
 Comment: 
 
-Filename: sbcli_mc-1.0.1/simplyblock_core/snode_client.py
+Filename: sbcli_mc-1.0.2/simplyblock_core/snode_client.py
 Comment: 
 
-Filename: sbcli_mc-1.0.1/simplyblock_core/kv_store.py
+Filename: sbcli_mc-1.0.2/simplyblock_core/kv_store.py
 Comment: 
 
-Filename: sbcli_mc-1.0.1/simplyblock_core/compute_node_ops.py
+Filename: sbcli_mc-1.0.2/simplyblock_core/compute_node_ops.py
 Comment: 
 
-Filename: sbcli_mc-1.0.1/simplyblock_core/rpc_client.py
+Filename: sbcli_mc-1.0.2/simplyblock_core/rpc_client.py
 Comment: 
 
-Filename: sbcli_mc-1.0.1/simplyblock_core/mgmt_node_ops.py
+Filename: sbcli_mc-1.0.2/simplyblock_core/mgmt_node_ops.py
 Comment: 
 
-Filename: sbcli_mc-1.0.1/simplyblock_core/utils.py
+Filename: sbcli_mc-1.0.2/simplyblock_core/utils.py
 Comment: 
 
-Filename: sbcli_mc-1.0.1/simplyblock_core/distr_controller.py
+Filename: sbcli_mc-1.0.2/simplyblock_core/distr_controller.py
 Comment: 
 
-Filename: sbcli_mc-1.0.1/simplyblock_core/shell_utils.py
+Filename: sbcli_mc-1.0.2/simplyblock_core/shell_utils.py
 Comment: 
 
-Filename: sbcli_mc-1.0.1/simplyblock_core/cnode_client.py
+Filename: sbcli_mc-1.0.2/simplyblock_core/cnode_client.py
 Comment: 
 
-Filename: sbcli_mc-1.0.1/simplyblock_core/storage_node_ops.py
+Filename: sbcli_mc-1.0.2/simplyblock_core/storage_node_ops.py
 Comment: 
 
-Filename: sbcli_mc-1.0.1/simplyblock_core/constants.py
+Filename: sbcli_mc-1.0.2/simplyblock_core/constants.py
 Comment: 
 
-Filename: sbcli_mc-1.0.1/simplyblock_core/services/job_tasks.py
+Filename: sbcli_mc-1.0.2/simplyblock_core/services/job_tasks.py
 Comment: 
 
-Filename: sbcli_mc-1.0.1/simplyblock_core/services/caching_node_monitor.py
+Filename: sbcli_mc-1.0.2/simplyblock_core/services/caching_node_monitor.py
 Comment: 
 
-Filename: sbcli_mc-1.0.1/simplyblock_core/services/service_template.service
+Filename: sbcli_mc-1.0.2/simplyblock_core/services/service_template.service
 Comment: 
 
-Filename: sbcli_mc-1.0.1/simplyblock_core/services/install_service.sh
+Filename: sbcli_mc-1.0.2/simplyblock_core/services/install_service.sh
 Comment: 
 
-Filename: sbcli_mc-1.0.1/simplyblock_core/services/__init__.py
+Filename: sbcli_mc-1.0.2/simplyblock_core/services/__init__.py
 Comment: 
 
-Filename: sbcli_mc-1.0.1/simplyblock_core/services/log_agg_service.py
+Filename: sbcli_mc-1.0.2/simplyblock_core/services/log_agg_service.py
 Comment: 
 
-Filename: sbcli_mc-1.0.1/simplyblock_core/services/health_check_service.py
+Filename: sbcli_mc-1.0.2/simplyblock_core/services/health_check_service.py
 Comment: 
 
-Filename: sbcli_mc-1.0.1/simplyblock_core/services/capacity_and_stats_collector.py
+Filename: sbcli_mc-1.0.2/simplyblock_core/services/capacity_and_stats_collector.py
 Comment: 
 
-Filename: sbcli_mc-1.0.1/simplyblock_core/services/device_monitor.py
+Filename: sbcli_mc-1.0.2/simplyblock_core/services/device_monitor.py
 Comment: 
 
-Filename: sbcli_mc-1.0.1/simplyblock_core/services/lvol_stat_collector.py
+Filename: sbcli_mc-1.0.2/simplyblock_core/services/lvol_stat_collector.py
 Comment: 
 
-Filename: sbcli_mc-1.0.1/simplyblock_core/services/cap_monitor.py
+Filename: sbcli_mc-1.0.2/simplyblock_core/services/cap_monitor.py
 Comment: 
 
-Filename: sbcli_mc-1.0.1/simplyblock_core/services/storage_node_monitor.py
+Filename: sbcli_mc-1.0.2/simplyblock_core/services/storage_node_monitor.py
 Comment: 
 
-Filename: sbcli_mc-1.0.1/simplyblock_core/services/port_stat_collector.py
+Filename: sbcli_mc-1.0.2/simplyblock_core/services/port_stat_collector.py
 Comment: 
 
-Filename: sbcli_mc-1.0.1/simplyblock_core/services/distr_event_collector.py
+Filename: sbcli_mc-1.0.2/simplyblock_core/services/distr_event_collector.py
 Comment: 
 
-Filename: sbcli_mc-1.0.1/simplyblock_core/services/remove_service.sh
+Filename: sbcli_mc-1.0.2/simplyblock_core/services/remove_service.sh
 Comment: 
 
-Filename: sbcli_mc-1.0.1/simplyblock_core/services/mgmt_node_monitor.py
+Filename: sbcli_mc-1.0.2/simplyblock_core/services/mgmt_node_monitor.py
 Comment: 
 
-Filename: sbcli_mc-1.0.1/simplyblock_core/services/lvol_monitor.py
+Filename: sbcli_mc-1.0.2/simplyblock_core/services/lvol_monitor.py
 Comment: 
 
-Filename: sbcli_mc-1.0.1/simplyblock_core/controllers/pool_controller.py
+Filename: sbcli_mc-1.0.2/simplyblock_core/controllers/pool_controller.py
 Comment: 
 
-Filename: sbcli_mc-1.0.1/simplyblock_core/controllers/__init__.py
+Filename: sbcli_mc-1.0.2/simplyblock_core/controllers/__init__.py
 Comment: 
 
-Filename: sbcli_mc-1.0.1/simplyblock_core/controllers/storage_events.py
+Filename: sbcli_mc-1.0.2/simplyblock_core/controllers/storage_events.py
 Comment: 
 
-Filename: sbcli_mc-1.0.1/simplyblock_core/controllers/lvol_controller.py
+Filename: sbcli_mc-1.0.2/simplyblock_core/controllers/lvol_controller.py
 Comment: 
 
-Filename: sbcli_mc-1.0.1/simplyblock_core/controllers/device_events.py
+Filename: sbcli_mc-1.0.2/simplyblock_core/controllers/device_events.py
 Comment: 
 
-Filename: sbcli_mc-1.0.1/simplyblock_core/controllers/lvol_events.py
+Filename: sbcli_mc-1.0.2/simplyblock_core/controllers/lvol_events.py
 Comment: 
 
-Filename: sbcli_mc-1.0.1/simplyblock_core/controllers/snapshot_controller.py
+Filename: sbcli_mc-1.0.2/simplyblock_core/controllers/snapshot_controller.py
 Comment: 
 
-Filename: sbcli_mc-1.0.1/simplyblock_core/controllers/snapshot_events.py
+Filename: sbcli_mc-1.0.2/simplyblock_core/controllers/snapshot_events.py
 Comment: 
 
-Filename: sbcli_mc-1.0.1/simplyblock_core/controllers/events_controller.py
+Filename: sbcli_mc-1.0.2/simplyblock_core/controllers/events_controller.py
 Comment: 
 
-Filename: sbcli_mc-1.0.1/simplyblock_core/controllers/health_controller.py
+Filename: sbcli_mc-1.0.2/simplyblock_core/controllers/health_controller.py
 Comment: 
 
-Filename: sbcli_mc-1.0.1/simplyblock_core/controllers/device_controller.py
+Filename: sbcli_mc-1.0.2/simplyblock_core/controllers/device_controller.py
 Comment: 
 
-Filename: sbcli_mc-1.0.1/simplyblock_core/controllers/pool_events.py
+Filename: sbcli_mc-1.0.2/simplyblock_core/controllers/pool_events.py
 Comment: 
 
-Filename: sbcli_mc-1.0.1/simplyblock_core/controllers/caching_node_controller.py
+Filename: sbcli_mc-1.0.2/simplyblock_core/controllers/caching_node_controller.py
 Comment: 
 
-Filename: sbcli_mc-1.0.1/simplyblock_core/controllers/cluster_events.py
+Filename: sbcli_mc-1.0.2/simplyblock_core/controllers/cluster_events.py
 Comment: 
 
-Filename: sbcli_mc-1.0.1/simplyblock_core/controllers/mgmt_events.py
+Filename: sbcli_mc-1.0.2/simplyblock_core/controllers/mgmt_events.py
 Comment: 
 
-Filename: sbcli_mc-1.0.1/simplyblock_core/models/caching_node.py
+Filename: sbcli_mc-1.0.2/simplyblock_core/models/caching_node.py
 Comment: 
 
-Filename: sbcli_mc-1.0.1/simplyblock_core/models/nvme_device.py
+Filename: sbcli_mc-1.0.2/simplyblock_core/models/nvme_device.py
 Comment: 
 
-Filename: sbcli_mc-1.0.1/simplyblock_core/models/mgmt_node.py
+Filename: sbcli_mc-1.0.2/simplyblock_core/models/mgmt_node.py
 Comment: 
 
-Filename: sbcli_mc-1.0.1/simplyblock_core/models/compute_node.py
+Filename: sbcli_mc-1.0.2/simplyblock_core/models/compute_node.py
 Comment: 
 
-Filename: sbcli_mc-1.0.1/simplyblock_core/models/__init__.py
+Filename: sbcli_mc-1.0.2/simplyblock_core/models/__init__.py
 Comment: 
 
-Filename: sbcli_mc-1.0.1/simplyblock_core/models/events.py
+Filename: sbcli_mc-1.0.2/simplyblock_core/models/events.py
 Comment: 
 
-Filename: sbcli_mc-1.0.1/simplyblock_core/models/global_settings.py
+Filename: sbcli_mc-1.0.2/simplyblock_core/models/global_settings.py
 Comment: 
 
-Filename: sbcli_mc-1.0.1/simplyblock_core/models/job_schedule.py
+Filename: sbcli_mc-1.0.2/simplyblock_core/models/job_schedule.py
 Comment: 
 
-Filename: sbcli_mc-1.0.1/simplyblock_core/models/base_model.py
+Filename: sbcli_mc-1.0.2/simplyblock_core/models/base_model.py
 Comment: 
 
-Filename: sbcli_mc-1.0.1/simplyblock_core/models/lvol_model.py
+Filename: sbcli_mc-1.0.2/simplyblock_core/models/lvol_model.py
 Comment: 
 
-Filename: sbcli_mc-1.0.1/simplyblock_core/models/snapshot.py
+Filename: sbcli_mc-1.0.2/simplyblock_core/models/snapshot.py
 Comment: 
 
-Filename: sbcli_mc-1.0.1/simplyblock_core/models/storage_node.py
+Filename: sbcli_mc-1.0.2/simplyblock_core/models/storage_node.py
 Comment: 
 
-Filename: sbcli_mc-1.0.1/simplyblock_core/models/stats.py
+Filename: sbcli_mc-1.0.2/simplyblock_core/models/stats.py
 Comment: 
 
-Filename: sbcli_mc-1.0.1/simplyblock_core/models/pool.py
+Filename: sbcli_mc-1.0.2/simplyblock_core/models/pool.py
 Comment: 
 
-Filename: sbcli_mc-1.0.1/simplyblock_core/models/iface.py
+Filename: sbcli_mc-1.0.2/simplyblock_core/models/iface.py
 Comment: 
 
-Filename: sbcli_mc-1.0.1/simplyblock_core/models/cluster.py
+Filename: sbcli_mc-1.0.2/simplyblock_core/models/cluster.py
 Comment: 
 
-Filename: sbcli_mc-1.0.1/simplyblock_core/models/port_stat.py
+Filename: sbcli_mc-1.0.2/simplyblock_core/models/port_stat.py
 Comment: 
 
-Filename: sbcli_mc-1.0.1/simplyblock_core/scripts/alerting/
+Filename: sbcli_mc-1.0.2/simplyblock_core/scripts/alerting/
 Comment: 
 
-Filename: sbcli_mc-1.0.1/simplyblock_core/scripts/dashboards/
+Filename: sbcli_mc-1.0.2/simplyblock_core/scripts/dashboards/
 Comment: 
 
-Filename: sbcli_mc-1.0.1/simplyblock_core/scripts/install_deps.sh
+Filename: sbcli_mc-1.0.2/simplyblock_core/scripts/install_deps.sh
 Comment: 
 
-Filename: sbcli_mc-1.0.1/simplyblock_core/scripts/__init__.py
+Filename: sbcli_mc-1.0.2/simplyblock_core/scripts/__init__.py
 Comment: 
 
-Filename: sbcli_mc-1.0.1/simplyblock_core/scripts/run_ssh.sh
+Filename: sbcli_mc-1.0.2/simplyblock_core/scripts/run_ssh.sh
 Comment: 
 
-Filename: sbcli_mc-1.0.1/simplyblock_core/scripts/haproxy.cfg
+Filename: sbcli_mc-1.0.2/simplyblock_core/scripts/haproxy.cfg
 Comment: 
 
-Filename: sbcli_mc-1.0.1/simplyblock_core/scripts/db_config_double.sh
+Filename: sbcli_mc-1.0.2/simplyblock_core/scripts/db_config_double.sh
 Comment: 
 
-Filename: sbcli_mc-1.0.1/simplyblock_core/scripts/stack_deploy_wait.sh
+Filename: sbcli_mc-1.0.2/simplyblock_core/scripts/stack_deploy_wait.sh
 Comment: 
 
-Filename: sbcli_mc-1.0.1/simplyblock_core/scripts/datasource.yml
+Filename: sbcli_mc-1.0.2/simplyblock_core/scripts/datasource.yml
 Comment: 
 
-Filename: sbcli_mc-1.0.1/simplyblock_core/scripts/docker-compose-swarm.yml
+Filename: sbcli_mc-1.0.2/simplyblock_core/scripts/docker-compose-swarm.yml
 Comment: 
 
-Filename: sbcli_mc-1.0.1/simplyblock_core/scripts/set_db_config.sh
+Filename: sbcli_mc-1.0.2/simplyblock_core/scripts/set_db_config.sh
 Comment: 
 
-Filename: sbcli_mc-1.0.1/simplyblock_core/scripts/apply_dashboard.sh
+Filename: sbcli_mc-1.0.2/simplyblock_core/scripts/apply_dashboard.sh
 Comment: 
 
-Filename: sbcli_mc-1.0.1/simplyblock_core/scripts/prometheus.yml
+Filename: sbcli_mc-1.0.2/simplyblock_core/scripts/prometheus.yml
 Comment: 
 
-Filename: sbcli_mc-1.0.1/simplyblock_core/scripts/clean_local_storage_deploy.sh
+Filename: sbcli_mc-1.0.2/simplyblock_core/scripts/clean_local_storage_deploy.sh
 Comment: 
 
-Filename: sbcli_mc-1.0.1/simplyblock_core/scripts/docker-compose-swarm-monitoring.yml
+Filename: sbcli_mc-1.0.2/simplyblock_core/scripts/docker-compose-swarm-monitoring.yml
 Comment: 
 
-Filename: sbcli_mc-1.0.1/simplyblock_core/scripts/deploy_stack.sh
+Filename: sbcli_mc-1.0.2/simplyblock_core/scripts/deploy_stack.sh
 Comment: 
 
-Filename: sbcli_mc-1.0.1/simplyblock_core/scripts/db_config_single.sh
+Filename: sbcli_mc-1.0.2/simplyblock_core/scripts/db_config_single.sh
 Comment: 
 
-Filename: sbcli_mc-1.0.1/simplyblock_core/scripts/config_docker.sh
+Filename: sbcli_mc-1.0.2/simplyblock_core/scripts/config_docker.sh
 Comment: 
 
-Filename: sbcli_mc-1.0.1/simplyblock_core/scripts/alerting/alert_rules.yaml
+Filename: sbcli_mc-1.0.2/simplyblock_core/scripts/alerting/alert_rules.yaml
 Comment: 
 
-Filename: sbcli_mc-1.0.1/simplyblock_core/scripts/alerting/alert_resources.yaml
+Filename: sbcli_mc-1.0.2/simplyblock_core/scripts/alerting/alert_resources.yaml
 Comment: 
 
-Filename: sbcli_mc-1.0.1/simplyblock_core/scripts/dashboards/nodes.json
+Filename: sbcli_mc-1.0.2/simplyblock_core/scripts/dashboards/nodes.json
 Comment: 
 
-Filename: sbcli_mc-1.0.1/simplyblock_core/scripts/dashboards/cluster.json
+Filename: sbcli_mc-1.0.2/simplyblock_core/scripts/dashboards/cluster.json
 Comment: 
 
-Filename: sbcli_mc-1.0.1/simplyblock_core/scripts/dashboards/lvols.json
+Filename: sbcli_mc-1.0.2/simplyblock_core/scripts/dashboards/lvols.json
 Comment: 
 
-Filename: sbcli_mc-1.0.1/simplyblock_core/scripts/dashboards/devices.json
+Filename: sbcli_mc-1.0.2/simplyblock_core/scripts/dashboards/devices.json
 Comment: 
 
-Filename: sbcli_mc-1.0.1/simplyblock_core/scripts/dashboards/pools.json
+Filename: sbcli_mc-1.0.2/simplyblock_core/scripts/dashboards/pools.json
 Comment: 
 
-Filename: sbcli_mc-1.0.1/simplyblock_core/scripts/dashboards/node-exporter.json
+Filename: sbcli_mc-1.0.2/simplyblock_core/scripts/dashboards/node-exporter.json
 Comment: 
 
-Filename: sbcli_mc-1.0.1/sbcli_mc.egg-info/SOURCES.txt
+Filename: sbcli_mc-1.0.2/sbcli_mc.egg-info/SOURCES.txt
 Comment: 
 
-Filename: sbcli_mc-1.0.1/sbcli_mc.egg-info/requires.txt
+Filename: sbcli_mc-1.0.2/sbcli_mc.egg-info/requires.txt
 Comment: 
 
-Filename: sbcli_mc-1.0.1/sbcli_mc.egg-info/PKG-INFO
+Filename: sbcli_mc-1.0.2/sbcli_mc.egg-info/PKG-INFO
 Comment: 
 
-Filename: sbcli_mc-1.0.1/sbcli_mc.egg-info/top_level.txt
+Filename: sbcli_mc-1.0.2/sbcli_mc.egg-info/top_level.txt
 Comment: 
 
-Filename: sbcli_mc-1.0.1/sbcli_mc.egg-info/entry_points.txt
+Filename: sbcli_mc-1.0.2/sbcli_mc.egg-info/entry_points.txt
 Comment: 
 
-Filename: sbcli_mc-1.0.1/sbcli_mc.egg-info/dependency_links.txt
+Filename: sbcli_mc-1.0.2/sbcli_mc.egg-info/dependency_links.txt
 Comment: 
 
 Zip file comment:
```

## Comparing `sbcli_mc-1.0.1/README.md` & `sbcli_mc-1.0.2/README.md`

 * *Files identical despite different names*

## Comparing `sbcli_mc-1.0.1/PKG-INFO` & `sbcli_mc-1.0.2/PKG-INFO`

 * *Files 4% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: sbcli-mc
-Version: 1.0.1
+Version: 1.0.2
 Summary: CLI for managing SimplyBlock cluster
 Home-page: https://www.simplyblock.io/
 Author: Hamdy
 Author-email: hamdy@simplyblock.io
 Description-Content-Type: text/markdown
 Requires-Dist: foundationdb
 Requires-Dist: requests
```

## Comparing `sbcli_mc-1.0.1/setup.py` & `sbcli_mc-1.0.2/setup.py`

 * *Files identical despite different names*

## Comparing `sbcli_mc-1.0.1/simplyblock_cli/cli.py` & `sbcli_mc-1.0.2/simplyblock_cli/cli.py`

 * *Files 8% similar despite different names*

```diff
@@ -19,38 +19,34 @@
 
     def __init__(self):
         self.logger = logging.getLogger()
         self.logger.setLevel(constants.LOG_LEVEL)
         self.db_store = kv_store.KVStore()
         self.init_parser()
 
-        # storage-node command
+        #
+        #----------------- storage-node -----------------
+        #
+
         subparser = self.add_command('storage-node', 'Storage node commands', aliases=['sn'])
         # Add storage node
         sub_command = self.add_sub_command(subparser, "deploy", 'Deploy local services for remote ops (local run)')
         sub_command.add_argument("--ifname", help='Management interface name, default: eth0')
 
-        sub_command = self.add_sub_command(subparser, "deploy-cleaner", 'clean local deploy (local run)')
-
-        # sub_command = self.add_sub_command(subparser, "add", 'Add storage node')
-        # sub_command.add_argument("cluster_id", help='UUID of the cluster to which the node will belong')
-        # sub_command.add_argument("ifname", help='Management interface name')
-        # sub_command.add_argument("--data-nics", help='Data interface names', nargs='+', dest='data_nics')
+        self.add_sub_command(subparser, "deploy-cleaner", 'clean local deploy (local run)')
 
         sub_command = self.add_sub_command(subparser, "add-node", 'Add storage node by ip')
         sub_command.add_argument("cluster_id", help='UUID of the cluster to which the node will belong')
         sub_command.add_argument("node_ip", help='IP of storage node to add')
         sub_command.add_argument("ifname", help='Management interface name')
         sub_command.add_argument("--jm-pcie", help='JM device address', dest='jm_pcie')
         sub_command.add_argument("--data-nics", help='Data interface names', nargs='+', dest='data_nics')
         sub_command.add_argument("--cpu-mask", help='SPDK app CPU mask, default is all cores found',
                                  dest='spdk_cpu_mask')
         sub_command.add_argument("--memory", help='SPDK huge memory allocation, default is 4G', dest='spdk_mem')
-        sub_command.add_argument("--dev-split", help='Split nvme devices by this factor, can be 2 or more',
-                                 dest='dev_split', type=int, default=1)
         sub_command.add_argument("--spdk-image", help='SPDK image uri', dest='spdk_image')
         sub_command.add_argument("--spdk-debug", help='Enable spdk debug logs', dest='spdk_debug', required=False, action='store_true')
 
         sub_command.add_argument("--iobuf_small_pool_count", help='bdev_set_options param', dest='small_pool_count',  type=int, default=0)
         sub_command.add_argument("--iobuf_large_pool_count", help='bdev_set_options param', dest='large_pool_count',  type=int, default=0)
         sub_command.add_argument("--iobuf_small_bufsize", help='bdev_set_options param', dest='small_bufsize',  type=int, default=0)
         sub_command.add_argument("--iobuf_large_bufsize", help='bdev_set_options param', dest='large_bufsize',  type=int, default=0)
@@ -70,19 +66,14 @@
         sub_command = self.add_sub_command(subparser, "list", 'List storage nodes')
         sub_command.add_argument("--cluster-id", help='id of the cluster for which nodes are listed', dest='cluster_id')
         sub_command.add_argument("--json", help='Print outputs in json format', action='store_true')
 
         sub_command = self.add_sub_command(subparser, "get", 'Get storage node info')
         sub_command.add_argument("id", help='UUID of storage node')
 
-        sub_command = self.add_sub_command(subparser, "update", 'Update storage node db info')
-        sub_command.add_argument("id", help='UUID of storage node')
-        sub_command.add_argument("key", help='Key')
-        sub_command.add_argument("value", help='Value')
-
         # Restart storage node
         sub_command = self.add_sub_command(
             subparser, "restart", 'Restart a storage node. All functions and device drivers will be reset. '
                                   'During restart, the node does not accept IO. In a high-availability setup, '
                                   'this will not impact operations.')
         sub_command.add_argument("node_id", help='UUID of storage node')
         sub_command.add_argument("--cpu-mask", help='SPDK app CPU mask, default is all cores found', dest='spdk_cpu_mask')
@@ -149,59 +140,31 @@
         sub_command = self.add_sub_command(subparser, "reset-device", 'Reset storage device')
         sub_command.add_argument("device_id", help='the devices\'s UUID')
 
         # Reset storage device
         sub_command = self.add_sub_command(subparser, "restart-device", 'Re add "removed" storage device')
         sub_command.add_argument("id", help='the devices\'s UUID')
 
-        # run tests against storage device
-        sub_command = self.add_sub_command(subparser, 'run-smart', 'Run tests against storage device')
-        sub_command.add_argument("device_id", help='the devices\'s UUID')
-
         # Add a new storage device
         sub_command = self.add_sub_command(subparser, 'add-device', 'Add a new storage device')
-        sub_command.add_argument("name", help='Storage device name (as listed in the operating system). '
-                                              'The device will be de-attached from the operating system and '
-                                              'attached to the storage node')
-        sub_command.add_argument("node_id", help='UUID of the node')
-        sub_command.add_argument("cluster_id", help='UUID of the cluster')
-
-        # Replace storage node
-        # sub_command = self.add_sub_command(
-        #     subparser, 'replace', 'Replace a storage node. This command is run on the new physical server, which is '
-        #                           'expected to replace the old server. Attention!!! All the nvme devices, '
-        #                           'which are part of the cluster to which the node belongs, must be inserted into '
-        #                           'the new server before this command is run. The old node will be de-commissioned '
-        #                           'and cannot be used any more.')
-        # sub_command.add_argument("node_id", help='UUID of the node to be replaced')
-        # sub_command.add_argument("ifname", help='Management interface name')
-        # sub_command.add_argument("--data-nics", help='Data interface names', nargs='+', dest='data_nics')
-
         sub_command = self.add_sub_command(
             subparser, 'remove-device', 'Remove a storage device. The device will become unavailable, independently '
                                         'if it was physically removed from the server. This function can be used if '
                                         'auto-detection of removal did not work or if the device must be maintained '
                                         'otherwise while remaining inserted into the server. ')
         sub_command.add_argument("device_id", help='Storage device ID')
         sub_command.add_argument("--force", help='Force device remove', required=False, action='store_true')
 
-        sub_command = self.add_sub_command(subparser, 'set-ro-device', 'Set storage device read only')
-        sub_command.add_argument("device_id", help='Storage device ID')
-
         sub_command = self.add_sub_command(
-            subparser, 'set-failed-device', 'Set storage device to failed state. This command can be used, '
+            subparser, 'set-failed-device', 'Set storage device to failed state. ', usage='This command can be used, '
                                             'if an administrator believes that the device must be changed, '
                                             'but its status and health state do not lead to an automatic detection '
                                             'of the failure state. Attention!!! The failed state is final, all data '
                                             'on the device will be automatically recovered to other devices '
                                             'in the cluster. ')
-        sub_command.add_argument("device_id", help='Storage device ID')
-
-        sub_command = self.add_sub_command(subparser, 'set-online-device', 'Set storage device to online state')
-        sub_command.add_argument("device_id", help='Storage device ID')
 
         sub_command = self.add_sub_command(
             subparser, 'get-capacity-device', 'Returns the size, absolute and relative utilization of '
                                               'the device in bytes')
         sub_command.add_argument("device_id", help='Storage device ID')
         sub_command.add_argument("--history", help='list history records -one for every 15 minutes- '
                                                    'for XX days and YY hours -up to 10 days in total-, format: XXdYYh')
@@ -211,56 +174,23 @@
                                               'a monitor, which updates current statistics records every two seconds '
                                               '(similar to ping):read-iops write-iops total-iops read-mbs '
                                               'write-mbs total-mbs')
         sub_command.add_argument("device_id", help='Storage device ID')
         sub_command.add_argument("--history", help='list history records -one for every 15 minutes- '
                                                    'for XX days and YY hours -up to 10 days in total-, format: XXdYYh')
 
-        sub_command = self.add_sub_command(
-            subparser, 'get-event-log', 'Returns storage node event log in syslog format. This includes events from '
-                                        'the storage node itself, the network interfaces and all devices on the node, '
-                                        'including health status information and updates.')
-        sub_command.add_argument("node_id", help='Storage node ID')
-        sub_command.add_argument("--from", help='from time, format: dd-mm-yy hh:mm')
-        sub_command.add_argument("--to", help='to time, format: dd-mm-yy hh:mm')
-
-        sub_command = self.add_sub_command(
-            subparser, 'get-log-page-device', 'Get nvme log-page information from the device. Attention! The '
-                                              'availability of particular log pages depends on the device model. '
-                                              'For more information, see nvme specification. ')
-        sub_command.add_argument("device-id", help='Storage device ID')
-        sub_command.add_argument(
-            "log-page", help='Can be [error , smart , telemetry , dev-self-test , endurance , persistent-event]',
-            choices=["error", "smart", "telemetry", "dev-self-test", "endurance", "persistent-event"])
-
         sub_command = self.add_sub_command(subparser, 'port-list', 'Get Data interfaces list for a node')
         sub_command.add_argument("node_id", help='Storage node ID')
 
         sub_command = self.add_sub_command(subparser, 'port-io-stats', 'Get Data interfaces IO stats')
         sub_command.add_argument("port_id", help='Data port ID')
         sub_command.add_argument("--history", help='list history records -one for every 15 minutes- '
                                                    'for XX days and YY hours -up to 10 days in total, format: XXdYYh',
                                  type=int, default=20)
 
-        #  get-host-secret
-        sub_command = self.add_sub_command(
-            subparser, 'get-host-secret', 'Returns the auto-generated host secret required for the nvmeof '
-                                          'connection between host and cluster')
-        sub_command.add_argument("id", help='Storage node ID')
-
-        #  get-ctrl-secret
-        sub_command = self.add_sub_command(
-            subparser, 'get-ctrl-secret', 'Returns the auto-generated controller secret required for the nvmeof '
-                                          'connection between host and cluster')
-        sub_command.add_argument("id", help='Storage node ID')
-
-        # #  run health ckecks
-        # sub_command = self.add_sub_command(subparser, 'health-check', 'Run health checks')
-        # sub_command.add_argument("id", help='Storage node ID')
-
         # check storage node
         sub_command = self.add_sub_command(subparser, "check", 'Health check storage node')
         sub_command.add_argument("id", help='UUID of storage node')
 
         # check device
         sub_command = self.add_sub_command(subparser, "check-device", 'Health check device')
         sub_command.add_argument("id", help='device UUID')
@@ -269,120 +199,81 @@
         sub_command = self.add_sub_command(subparser, "info", 'Get node information')
         sub_command.add_argument("id", help='Node UUID')
 
         # node info-spdk
         sub_command = self.add_sub_command(subparser, "info-spdk", 'Get SPDK memory information')
         sub_command.add_argument("id", help='Node UUID')
 
-        # Initialize cluster parser
+        #
+        # ----------------- cluster -----------------
+        #
+
         subparser = self.add_command('cluster', 'Cluster commands')
 
         sub_command = self.add_sub_command(subparser, 'create',
                                            'Create an new cluster with this node as mgmt (local run)')
         sub_command.add_argument(
             "--blk_size", help='The block size in bytes', type=int, choices=[512, 4096], default=512)
 
         sub_command.add_argument(
             "--page_size", help='The size of a data page in bytes', type=int, default=2097152)
 
         sub_command.add_argument(
             "--ha_type", help='Can be "single" for single node clusters or  "HA", which requires at least 3 nodes',
             choices=["single", "ha"], default='single')
-        sub_command.add_argument(
-            "--tls", help='TCP/IP transport security can be turned on and off. '
-                          'If turned on, both hosts and storage nodes must '
-                          'authenticate the connection via TLS certificates',
-            choices=["on", "off"], default='off')
-        sub_command.add_argument(
-            "--auth-hosts-only", help='if turned on, hosts must be explicitely added to the '
-                                      'cluster to be able to connect to any NVMEoF subsystem in the cluster',
-            choices=["on", "off"], default='off')
-        sub_command.add_argument(
-            "--model_ids", help='a list of supported NVMe device model-ids', nargs='+',
-            default=['Amazon EC2 NVMe Instance Storage'])
         sub_command.add_argument("--CLI_PASS", help='Password for CLI SSH connection', required=False)
-        # cap-warn ( % ), cap-crit ( % ), prov-cap-warn ( % ), prov-cap-crit. ( % )
         sub_command.add_argument("--cap-warn", help='Capacity warning level in percent, default=80',
                                  type=int, required=False, dest="cap_warn")
         sub_command.add_argument("--cap-crit", help='Capacity critical level in percent, default=90',
                                  type=int, required=False, dest="cap_crit")
         sub_command.add_argument("--prov-cap-warn", help='Capacity warning level in percent, default=180',
                                  type=int, required=False, dest="prov_cap_warn")
         sub_command.add_argument("--prov-cap-crit", help='Capacity critical level in percent, default=190',
                                  type=int, required=False, dest="prov_cap_crit")
         sub_command.add_argument("--ifname", help='Management interface name, default: eth0')
         sub_command.add_argument("--log-del-interval", help='graylog deletion interval, default: 7d',
                                  dest='log_del_interval', default='7d')
         sub_command.add_argument("--metrics-retention-period", help='retention period for prometheus metrics, default: 7d',
                                  dest='metrics_retention_period', default='7d')
 
-        # show cluster list
-        sub_command = self.add_sub_command(subparser, 'list', 'Show clusters list')
+        # add cluster
+        sub_command = self.add_sub_command(subparser, 'add', 'Add new cluster')
+        sub_command.add_argument("--blk_size", help='The block size in bytes', type=int, choices=[512, 4096], default=512)
+        sub_command.add_argument("--page_size", help='The size of a data page in bytes', type=int, default=2097152)
+        sub_command.add_argument("--ha_type",
+                                 help='Can be "single" for single node clusters or  "HA", which requires at least 3 nodes',
+                                 choices=["single", "ha"], default='single')
+        sub_command.add_argument("--cap-warn", help='Capacity warning level in percent, default=80',
+                                 type=int, required=False, dest="cap_warn")
+        sub_command.add_argument("--cap-crit", help='Capacity critical level in percent, default=90',
+                                 type=int, required=False, dest="cap_crit")
+        sub_command.add_argument("--prov-cap-warn", help='Capacity warning level in percent, default=180',
+                                 type=int, required=False, dest="prov_cap_warn")
+        sub_command.add_argument("--prov-cap-crit", help='Capacity critical level in percent, default=190',
+                                 type=int, required=False, dest="prov_cap_crit")
 
-        # # join cluster
-        # sub_command = self.add_sub_command(subparser, 'join', 'join cluster')
-        # sub_command.add_argument("cluster_ip", help='the cluster IP address')
-        # sub_command.add_argument("cluster_id", help='the cluster UUID')
-        # sub_command.add_argument("role", help='Choose the node role in the cluster', choices=["management", "storage", "storage-alloc"])
-        # sub_command.add_argument("ifname", help='Management interface name')
-        # sub_command.add_argument("--data-nics", help='Data interface names', nargs='+', dest='data_nics')
-        # sub_command.add_argument("--cpu-mask", help='SPDK app CPU mask, default is all cores found',  dest='spdk_cpu_mask')
-        # sub_command.add_argument("--memory", help='SPDK huge memory allocation, default is 4G',  dest='spdk_mem')
+        # show cluster list
+        self.add_sub_command(subparser, 'list', 'Show clusters list')
 
         # show cluster info
         sub_command = self.add_sub_command(
             subparser, 'status', 'Show cluster status')
         sub_command.add_argument("cluster_id", help='the cluster UUID')
 
         # show cluster info
         sub_command = self.add_sub_command(subparser, 'get', 'Show cluster info')
         sub_command.add_argument("id", help='the cluster UUID')
 
         sub_command = self.add_sub_command(
-            subparser, 'suspend', 'Suspend cluster. The cluster will stop processing all IO. '
-                                  'Attention! This will cause an "all paths down" event for nvmeof/iscsi volumes '
-                                  'on all hosts connected to the cluster.')
-        sub_command.add_argument("cluster_id", help='the cluster UUID')
-
-        sub_command = self.add_sub_command(
-            subparser, 'unsuspend', 'Unsuspend cluster. The cluster will start processing IO again.')
-        sub_command.add_argument("cluster_id", help='the cluster UUID')
-
-        sub_command = self.add_sub_command(
-            subparser, 'add-dev-model', 'Add a device to the white list by the device model id. '
-                                        'When adding nodes to the cluster later on, all devices of the specified '
-                                        'model-ids, which are present on the node to be added to the cluster, '
-                                        'are added to the storage node for the cluster. This does not apply for '
-                                        'already added devices, but only affect devices on additional nodes, '
-                                        'which will be added to the cluster. It is always possible to also add '
-                                        'devices present on a server to a node manually.')
+            subparser, 'suspend', 'Suspend cluster')
         sub_command.add_argument("cluster_id", help='the cluster UUID')
-        sub_command.add_argument("model_ids", help='a list of supported NVMe device model-ids', nargs='+')
 
         sub_command = self.add_sub_command(
-            subparser, 'rm-dev-model', 'Remove device from the white list by the device model id. This does not apply '
-                                       'for already added devices, but only affect devices on additional nodes, '
-                                       'which will be added to the cluster. ')
+            subparser, 'unsuspend', 'Unsuspend cluster')
         sub_command.add_argument("cluster_id", help='the cluster UUID')
-        sub_command.add_argument("model-ids", help='a list of NVMe device model-ids', nargs='+')
-
-        sub_command = self.add_sub_command(
-            subparser, 'add-host-auth', 'If the "authorized hosts only" security feature is turned on, '
-                                        'hosts must be explicitly added to the cluster via their nqn before '
-                                        'they can discover the subsystem initiate a connection.')
-        sub_command.add_argument("cluster_id", help='the cluster UUID')
-        sub_command.add_argument("host-nqn", help='NQN of the host to allow to discover and connect to teh cluster')
-
-        sub_command = self.add_sub_command(
-            subparser, 'rm-host-auth', 'If the "authorized hosts only" security feature is turned on, '
-                                       'this function removes hosts, which have been added to the cluster '
-                                       'via their nqn, from the list of authorized hosts. After a host has '
-                                       'been removed, it cannot connect any longer to the subsystem and cluster.')
-        sub_command.add_argument("cluster_id", help='the cluster UUID')
-        sub_command.add_argument("host-nqn", help='NQN of the host to remove from the allowed hosts list')
 
         sub_command = self.add_sub_command(
             subparser, 'get-capacity', 'Returns the current total available capacity, utilized capacity '
                                        '(in percent and absolute) and provisioned capacity (in percent and absolute) '
                                        'in GB in the cluster.')
         sub_command.add_argument("cluster_id", help='the cluster UUID')
         sub_command.add_argument("--json", help='Print json output', required=False, action='store_true')
@@ -393,41 +284,29 @@
             subparser, 'get-io-stats', 'Returns the io statistics. If --history is not selected, this is a monitor, '
                                        'which updates current statistics records every two seconds '
                                        '(similar to ping):read-iops write-iops total-iops read-mbs write-mbs total-mbs')
         sub_command.add_argument("cluster_id", help='the cluster UUID')
         sub_command.add_argument("--records", help='Number of records, default: 20', type=int, default=20)
         sub_command.add_argument("--history", help='(XXdYYh), list history records (one for every 15 minutes) '
                                                    'for XX days and YY hours (up to 10 days in total).')
-        sub_command.add_argument("--random", help='Generate random data', action='store_true')
-
-        sub_command = self.add_sub_command(
-            subparser, 'set-log-level', 'Defines the detail of the log information collected and stored')
-        sub_command.add_argument("cluster_id", help='the cluster UUID')
-        sub_command.add_argument("level", help='Log level', choices=["debug", "test", "prod"])
-
-        # sub_command = self.add_sub_command(
-        #     subparser, 'get-event-log', 'returns cluster event log in syslog format')
-        # sub_command.add_argument("cluster-id", help='the cluster UUID')
-        # sub_command.add_argument("--from", help='from time, format: dd-mm-yy hh:mm')
-        # sub_command.add_argument("--to", help='to time, format: dd-mm-yy hh:mm')
 
         sub_command = self.add_sub_command(
             subparser, 'get-cli-ssh-pass', 'returns the ssh password for the CLI ssh connection')
         sub_command.add_argument("cluster_id", help='the cluster UUID')
 
         # get-logs
         sub_command = self.add_sub_command(subparser, 'get-logs', 'Returns distr logs')
         sub_command.add_argument("cluster_id", help='cluster uuid')
 
         # get-secret
         sub_command = self.add_sub_command(subparser, 'get-secret', 'Returns auto generated, 20 characters secret.')
         sub_command.add_argument("cluster_id", help='cluster uuid')
 
         # set-secret
-        sub_command = self.add_sub_command(subparser, 'set-secret', 'Updates the secret (replaces the existing '
+        sub_command = self.add_sub_command(subparser, 'upd-secret', 'Updates the secret (replaces the existing '
                                                                     'one with a new one) and returns the new one.')
         sub_command.add_argument("cluster_id", help='cluster uuid')
         sub_command.add_argument("secret", help='new 20 characters password')
 
         # check cluster
         sub_command = self.add_sub_command(subparser, "check", 'Health check cluster')
         sub_command.add_argument("id", help='cluster UUID')
@@ -439,20 +318,24 @@
         # graceful-shutdown storage nodes
         sub_command = self.add_sub_command(subparser, "graceful-shutdown", 'Graceful shutdown of storage nodes')
         sub_command.add_argument("id", help='cluster UUID')
 
         # graceful-startup storage nodes
         sub_command = self.add_sub_command(subparser, "graceful-startup", 'Graceful startup of storage nodes')
         sub_command.add_argument("id", help='cluster UUID')
-        
+
         # get tasks list
         sub_command = self.add_sub_command(subparser, "list-tasks", 'List tasks by cluster ID')
         sub_command.add_argument("cluster_id", help='UUID of the cluster')
 
-        # lvol ops
+
+        #
+        # ----------------- lvol -----------------
+        #
+
         subparser = self.add_command('lvol', 'LVol commands')
         # add lvol
         sub_command = self.add_sub_command(subparser, 'add', 'Add a new logical volume')
         sub_command.add_argument("name", help='LVol name or id')
         sub_command.add_argument("size", help='LVol size: 10M, 10G, 10(bytes)')
         sub_command.add_argument("pool", help='Pool UUID or name')
         sub_command.add_argument("--snapshot", "-s", help='Make LVol with snapshot capability, default is False',
@@ -467,21 +350,14 @@
                                  required=False, action='store_true')
         sub_command.add_argument("--encrypt", help='Use inline data encryption and de-cryption on the logical volume',
                                  required=False, action='store_true')
         sub_command.add_argument("--crypto-key1", help='the hex value of key1 to be used for lvol encryption',
                                  dest='crypto_key1', default=None)
         sub_command.add_argument("--crypto-key2", help='the hex value of key2 to be used for lvol encryption',
                                  dest='crypto_key2', default=None)
-        sub_command.add_argument("--thick", help='Deactivate thin provisioning', required=False, action='store_true')
-        sub_command.add_argument("--node-ha",
-                                 help='The maximum amount of concurrent node failures accepted without interruption of operations',
-                                 required=False, default=1, type=int, choices=[0, 1, 2])
-        sub_command.add_argument("--dev-redundancy",
-                                 help='{1,2} supported minimal concurrent device failures without data loss',
-                                 required=False, action='store_true')
         sub_command.add_argument("--max-rw-iops", help='Maximum Read Write IO Per Second', type=int)
         sub_command.add_argument("--max-rw-mbytes", help='Maximum Read Write Mega Bytes Per Second', type=int)
         sub_command.add_argument("--max-r-mbytes", help='Maximum Read Mega Bytes Per Second', type=int)
         sub_command.add_argument("--max-w-mbytes", help='Maximum Write Mega Bytes Per Second', type=int)
         sub_command.add_argument("--distr-vuid", help='(Dev) set vuid manually, default: random (1-99999)', type=int,
                                  default=0)
         sub_command.add_argument("--distr-ndcs", help='(Dev) set ndcs manually, default: 4', type=int, default=0)
@@ -500,22 +376,25 @@
         sub_command.add_argument("--max-r-mbytes", help='Maximum Read Mega Bytes Per Second', type=int)
         sub_command.add_argument("--max-w-mbytes", help='Maximum Write Mega Bytes Per Second', type=int)
 
         # list lvols
         sub_command = self.add_sub_command(subparser, 'list', 'List all LVols')
         sub_command.add_argument("--cluster-id", help='List LVols in particular cluster')
         sub_command.add_argument("--json", help='Print outputs in json format', required=False, action='store_true')
-        # list lvols
-        sub_command = self.add_sub_command(subparser, 'list-mem', 'List all LVols')
+
+        # Get the size and max_size of the lvol
+        sub_command = self.add_sub_command(subparser, 'list-mem', 'Get the size and max_size of the lvol')
         sub_command.add_argument("--json", help='Print outputs in json format', required=False, action='store_true')
         sub_command.add_argument("--csv", help='Print outputs in csv format', required=False, action='store_true')
+
         # get lvol
         sub_command = self.add_sub_command(subparser, 'get', 'Get LVol details')
         sub_command.add_argument("id", help='LVol id or name')
         sub_command.add_argument("--json", help='Print outputs in json format', required=False, action='store_true')
+
         # delete lvol
         sub_command = self.add_sub_command(
             subparser, 'delete', 'Delete LVol. This is only possible, if no more snapshots and non-inflated clones '
                                  'of the volume exist. The volume must be suspended before it can be deleted. ')
         sub_command.add_argument("id", help='LVol id or ids', nargs='+')
         sub_command.add_argument("--force", help='Force delete LVol from the cluster', required=False,
                                  action='store_true')
@@ -530,80 +409,44 @@
         sub_command = self.add_sub_command(
             subparser, 'resize', 'Resize LVol. The lvol cannot be exceed the maximum size for lvols. It cannot '
                                  'exceed total remaining provisioned space in pool. It cannot drop below the '
                                  'current utilization.')
         sub_command.add_argument("id", help='LVol id')
         sub_command.add_argument("size", help='New LVol size size: 10M, 10G, 10(bytes)')
 
-        # lvol set read-only
-        sub_command = self.add_sub_command(
-            subparser, 'set-read-only', 'Set LVol Read-only. Current write IO in flight will still be processed, '
-                                        'but for new IO, only read and unmap IO are possible.')
-        sub_command.add_argument("id", help='LVol id')
-
-        # lvol set read-write
-        sub_command = self.add_sub_command(subparser, 'set-read-write', 'Set LVol Read-Write.')
-        sub_command.add_argument("id", help='LVol id')
-
-        # lvol suspend
-        sub_command = self.add_sub_command(
-            subparser, 'suspend', 'Suspend LVol. IO in flight will still be processed, but new IO is not accepted. '
-                                  'Make sure that the volume is detached from all hosts before '
-                                  'suspending it to avoid IO errors.')
-        sub_command.add_argument("id", help='LVol id')
-
-        # lvol unsuspend
-        sub_command = self.add_sub_command(subparser, 'unsuspend', 'Unsuspend LVol. IO may be resumed.')
-        sub_command.add_argument("id", help='LVol id')
-
         # lvol create-snapshot
         sub_command = self.add_sub_command(subparser, 'create-snapshot', 'Create snapshot from LVol')
         sub_command.add_argument("id", help='LVol id')
         sub_command.add_argument("name", help='snapshot name')
 
         # lvol clone
         sub_command = self.add_sub_command(subparser, 'clone', 'create LVol based on a snapshot')
         sub_command.add_argument("snapshot_id", help='snapshot UUID')
         sub_command.add_argument("clone_name", help='clone name')
+        sub_command.add_argument("--resize", help='New LVol size: 10M, 10G, 10(bytes)')
 
         # lvol move
         sub_command = self.add_sub_command(
             subparser, 'move', 'Moves a full copy of the logical volume between nodes')
         sub_command.add_argument("id", help='LVol UUID')
         # sub_command.add_argument("cluster-id", help='Destination Cluster ID')
         sub_command.add_argument("node_id", help='Destination Node UUID')
         sub_command.add_argument("--force", help='Force LVol delete from source node', required=False, action='store_true')
 
-        # lvol replicate
-        sub_command = self.add_sub_command(
-            subparser, 'replicate', 'Create a replication path between two volumes in two clusters')
-        sub_command.add_argument("id", help='LVol id')
-        sub_command.add_argument("cluster-a", help='A Cluster ID')
-        sub_command.add_argument("cluster-b", help='B Cluster ID')
-        sub_command.add_argument("--asynchronous",
-                                 help='Replication may be performed synchronously(default) and asynchronously',
-                                 action='store_true')
-
-        # lvol inflate
-        sub_command = self.add_sub_command(
-            subparser, 'inflate', 'Inflate a clone to "full" logical volume and disconnect it '
-                                  'from its parent snapshot.')
-        sub_command.add_argument("id", help='LVol id')
-
         # lvol get-capacity
         sub_command = self.add_sub_command(
             subparser, 'get-capacity', 'Returns the current (or historic) provisioned and utilized '
                                        '(in percent and absolute) capacity.')
         sub_command.add_argument("id", help='LVol id')
         sub_command.add_argument("--history", help='(XXdYYh), list history records (one for every 15 minutes) '
                                                    'for XX days and YY hours (up to 10 days in total).')
 
         # lvol get-io-stats
         sub_command = self.add_sub_command(
-            subparser, 'get-io-stats', 'Returns either the current or historic io statistics '
+            subparser, 'get-io-stats', help="Get Input Output stats of LVol", usage='Returns either the current or historic io statistics '
                                        '(read-IO, write-IO, total-IO, read mbs, write mbs, total mbs).')
         sub_command.add_argument("id", help='LVol id')
         sub_command.add_argument("--history", help='(XXdYYh), list history records (one for every 15 minutes) '
                                                    'for XX days and YY hours (up to 10 days in total).')
 
         sub_command = self.add_sub_command(subparser, 'send-cluster-map', 'send distr cluster map')
         sub_command.add_argument("id", help='LVol id')
@@ -624,18 +467,15 @@
         sub_command.add_argument("cluster_id", help='the cluster UUID')
         sub_command.add_argument("ifname", help='Management interface name')
 
         sub_command = self.add_sub_command(subparser, "list", 'List Management nodes')
         sub_command.add_argument("--json", help='Print outputs in json format', action='store_true')
 
         sub_command = self.add_sub_command(subparser, "remove", 'Remove Management node')
-        sub_command.add_argument("hostname", help='hostname')
-
-        sub_command = self.add_sub_command(subparser, 'show', 'List management nodes')
-        sub_command = self.add_sub_command(subparser, 'status', 'Show management cluster status')
+        sub_command.add_argument("id", help='Mgmt node uuid')
 
         # pool ops
         subparser = self.add_command('pool', 'Pool commands')
         # add pool
         sub_command = self.add_sub_command(subparser, 'add', 'Add a new Pool')
         sub_command.add_argument("name", help='Pool name')
         sub_command.add_argument("--cluster-id", help='id of the cluster', dest='cluster_id')
@@ -666,16 +506,16 @@
         # get pool
         sub_command = self.add_sub_command(subparser, 'get', 'get pool details')
         sub_command.add_argument("id", help='pool uuid')
         sub_command.add_argument("--json", help='Print outputs in json format', required=False, action='store_true')
 
         # delete pool
         sub_command = self.add_sub_command(
-            subparser, 'delete', 'delete pool. It is only possible to delete a pool if it is empty '
-                                 '(no provisioned logical volumes contained).')
+            subparser, 'delete', 'Delete Pool', usage=
+            "It is only possible to delete a pool if it is empty (no provisioned logical volumes contained).")
         sub_command.add_argument("id", help='pool uuid')
 
         # enable
         sub_command = self.add_sub_command(subparser, 'enable', 'Set pool status to Active')
         sub_command.add_argument("pool_id", help='pool uuid')
         # disable
         sub_command = self.add_sub_command(
@@ -708,22 +548,23 @@
 
         subparser = self.add_command('snapshot', 'Snapshot commands')
 
         sub_command = self.add_sub_command(subparser, 'add', 'Create new snapshot')
         sub_command.add_argument("id", help='LVol UUID')
         sub_command.add_argument("name", help='snapshot name')
 
-        sub_command = self.add_sub_command(subparser, 'list', 'List snapshots')
+        self.add_sub_command(subparser, 'list', 'List snapshots')
 
         sub_command = self.add_sub_command(subparser, 'delete', 'Delete a snapshot')
         sub_command.add_argument("id", help='snapshot UUID')
 
         sub_command = self.add_sub_command(subparser, 'clone', 'Create LVol from snapshot')
         sub_command.add_argument("id", help='snapshot UUID')
         sub_command.add_argument("lvol_name", help='LVol name')
+        sub_command.add_argument("--resize", help='New LVol size: 10M, 10G, 10(bytes)')
 
         # Caching node cli
         subparser = self.add_command('caching-node', 'Caching client node commands', aliases=['cn'])
 
         sub_command = self.add_sub_command(subparser, 'deploy', 'Deploy caching node on this machine (local exec)')
         sub_command.add_argument("--ifname", help='Management interface name, default: eth0')
 
@@ -733,85 +574,75 @@
         sub_command.add_argument("ifname", help='Management interface name')
         sub_command.add_argument("--cpu-mask", help='SPDK app CPU mask, default is all cores found',
                                  dest='spdk_cpu_mask')
         sub_command.add_argument("--memory", help='SPDK huge memory allocation, default is Max hugepages available', dest='spdk_mem')
         sub_command.add_argument("--spdk-image", help='SPDK image uri', dest='spdk_image')
         sub_command.add_argument("--namespace", help='k8s namespace to deploy on',)
 
-        sub_command = self.add_sub_command(subparser, 'list', 'List Caching nodes')
+        self.add_sub_command(subparser, 'list', 'List Caching nodes')
 
         sub_command = self.add_sub_command(subparser, 'list-lvols', 'List connected lvols')
         sub_command.add_argument("id", help='Caching Node UUID')
 
         sub_command = self.add_sub_command(subparser, 'remove', 'Remove Caching node from the cluster')
         sub_command.add_argument("id", help='Caching Node UUID')
         sub_command.add_argument("--force", help='Force remove', required=False, action='store_true')
 
-        # sub_command = self.add_sub_command(subparser, 'restart', 'Restart Caching node')
-        # sub_command.add_argument("id", help='Caching Node UUID')
-
         sub_command = self.add_sub_command(subparser, 'connect', 'Connect to LVol')
         sub_command.add_argument("node_id", help='Caching node UUID')
         sub_command.add_argument("lvol_id", help='LVol UUID')
 
         sub_command = self.add_sub_command(subparser, 'disconnect', 'Disconnect LVol from Caching node')
         sub_command.add_argument("node_id", help='Caching node UUID')
         sub_command.add_argument("lvol_id", help='LVol UUID')
 
         sub_command = self.add_sub_command(subparser, 'recreate', 'recreate Caching node bdevs ')
         sub_command.add_argument("node_id", help='Caching node UUID')
 
-
-
     def init_parser(self):
-        self.parser = argparse.ArgumentParser(description='Ultra management CLI')
+        self.parser = argparse.ArgumentParser(prog=constants.SIMPLY_BLOCK_CLI_NAME, description='SimplyBlock management CLI')
         self.parser.add_argument("-d", '--debug', help='Print debug messages', required=False, action='store_true')
         self.subparser = self.parser.add_subparsers(dest='command')
 
     def add_command(self, command, help, aliases=None):
         aliases = aliases or []
         storagenode = self.subparser.add_parser(command, description=help, help=help, aliases=aliases)
         storagenode_subparser = storagenode.add_subparsers(dest=command)
         return storagenode_subparser
 
-    def add_sub_command(self, parent_parser, command, help):
-        return parent_parser.add_parser(command, description=help, help=help)
+    def add_sub_command(self, parent_parser, command, help, usage=None):
+        return parent_parser.add_parser(command, description=help, help=help, usage=usage)
 
     def run(self):
         args = self.parser.parse_args()
         if args.debug:
             self.logger.setLevel(logging.DEBUG)
         else:
             self.logger.setLevel(constants.LOG_LEVEL)
         logging.getLogger("urllib3.connectionpool").setLevel(logging.WARNING)
 
         args_dict = args.__dict__
         ret = ""
         if args.command in ['storage-node', 'sn']:
             sub_command = args_dict['storage-node']
 
-            if sub_command in ['get-log-page-device', 'get-event-log',
-                               "get-ctrl-secret", "get-host-secret"]:
-                ret = "Not Implemented!"
-
-            elif sub_command == "deploy":
+            if sub_command == "deploy":
                 ret = storage_ops.deploy(args.ifname)
 
             elif sub_command == "deploy-cleaner":
                 ret = storage_ops.deploy_cleaner()
 
             elif sub_command == "add":
                 ret = self.storage_node_add(args)
 
             elif sub_command == "add-node":
                 cluster_id = args.cluster_id
                 node_ip = args.node_ip
                 ifname = args.ifname
                 data_nics = args.data_nics
-                dev_split = args.dev_split
                 spdk_image = args.spdk_image
                 spdk_debug = args.spdk_debug
 
                 small_pool_count = args.small_pool_count
                 large_pool_count = args.large_pool_count
                 small_bufsize = args.small_bufsize
                 large_bufsize = args.large_bufsize
@@ -826,23 +657,23 @@
                 spdk_mem = None
                 if args.spdk_mem:
                     spdk_mem = self.parse_size(args.spdk_mem)
                     if spdk_mem < 1 * 1024 * 1024:
                         return f"SPDK memory:{args.spdk_mem} must be larger than 1G"
 
                 out = storage_ops.add_node(
-                    cluster_id, node_ip, ifname, data_nics, spdk_cpu_mask, spdk_mem, dev_split, spdk_image, spdk_debug,
+                    cluster_id, node_ip, ifname, data_nics, spdk_cpu_mask, spdk_mem, spdk_image, spdk_debug,
                     small_pool_count, large_pool_count, small_bufsize, large_bufsize, args.jm_pcie)
                 return out
 
             elif sub_command == "list":
                 ret = storage_ops.list_storage_nodes(args.json, args.cluster_id)
 
             elif sub_command == "remove":
-                ret = storage_ops.remove_storage_node(args.node_id, args.force_remove, args.force_migrate)
+                ret = storage_ops.remove_storage_node(args.node_id, args.force_remove)
 
             elif sub_command == "delete":
                 ret = storage_ops.delete_storage_node(args.node_id)
 
             elif sub_command == "restart":
                 node_id = args.node_id
 
@@ -880,65 +711,56 @@
             elif sub_command == "device-testing-mode":
                 ret = device_controller.set_device_testing_mode(args.device_id, args.mode)
 
             elif sub_command == "remove-device":
                 ret = device_controller.device_remove(args.device_id, args.force)
 
             elif sub_command == "shutdown":
-                # answer = self.query_yes_no("Are you sure?", default=None)
-                # if answer is True:
                 ret = storage_ops.shutdown_storage_node(args.node_id, args.force)
 
             elif sub_command == "suspend":
                 ret = storage_ops.suspend_storage_node(args.node_id, args.force)
 
             elif sub_command == "resume":
                 ret = storage_ops.resume_storage_node(args.node_id)
 
             elif sub_command == "reset-device":
                 ret = device_controller.reset_storage_device(args.device_id)
 
             elif sub_command == "restart-device":
                 ret = device_controller.restart_device(args.id)
 
-            elif sub_command == "run-smart":
-                dev_name = args.name
-                ret = storage_ops.run_test_storage_device(self.db_store, dev_name)
-
             elif sub_command == "add-device":
-                dev_name = args.name
-                node_id = args.node_id
-                cluster_id = args.cluster_id
-                ret = storage_ops.add_storage_device(dev_name, node_id, cluster_id)
+                ret = "Not implemented!"
 
-            elif sub_command == "replace":
-                old_node_name = args.name
-                ifname = args.ifname
-                ret = storage_ops.replace_node(self.db_store, old_node_name, ifname)
+            elif sub_command == "set-failed-device":
+                ret = "Not implemented!"
 
             elif sub_command == "get-capacity-device":
                 device_id = args.device_id
                 history = args.history
                 data = device_controller.get_device_capacity(device_id, history)
                 if data:
                     ret = utils.print_table(data)
                 else:
                     return False
+
             elif sub_command == "get-device":
                 device_id = args.device_id
                 ret = device_controller.get_device(device_id)
 
             elif sub_command == "get-io-stats-device":
                 device_id = args.device_id
                 history = args.history
                 data = device_controller.get_device_iostats(device_id, history)
                 if data:
                     ret = utils.print_table(data)
                 else:
                     return False
+
             elif sub_command == "get-capacity":
                 node_id = args.node_id
                 history = args.history
                 data = storage_ops.get_node_capacity(node_id, history)
                 if data:
                     ret = utils.print_table(data)
                 else:
@@ -959,22 +781,14 @@
                 ret = storage_ops.get_node_ports(node_id)
 
             elif sub_command == "port-io-stats":
                 port_id = args.port_id
                 history = args.history
                 ret = storage_ops.get_node_port_iostats(port_id, history)
 
-            elif sub_command == "get-host-secret":
-                node_id = args.id
-                ret = storage_ops.get_host_secret(node_id)
-
-            elif sub_command == "get-ctrl-secret":
-                node_id = args.id
-                ret = storage_ops.get_ctrl_secret(node_id)
-
             elif sub_command == "check":
                 node_id = args.id
                 ret = health_controller.check_node(node_id)
 
             elif sub_command == "check-device":
                 device_id = args.id
                 ret = health_controller.check_device(device_id)
@@ -983,34 +797,28 @@
                 node_id = args.id
                 ret = storage_ops.get_info(node_id)
 
             elif sub_command == "info-spdk":
                 node_id = args.id
                 ret = storage_ops.get_spdk_info(node_id)
 
-            elif sub_command == "update":
-                ret = storage_ops.update(args.id, args.key, args.value)
-
             elif sub_command == "get":
                 ret = storage_ops.get(args.id)
 
             else:
                 self.parser.print_help()
 
         elif args.command == 'cluster':
             sub_command = args_dict[args.command]
-            if sub_command in ["add-dev-model", "rm-dev-model", "add-host-auth",
-                               "rm-host-auth", "set-log-level"]:
-                ret = "Not Implemented!"
-            elif sub_command == 'init':
-                ret = self.cluster_init(args)
-            elif sub_command == 'create':
+            if sub_command == 'create':
                 ret = self.cluster_create(args)
             elif sub_command == 'join':
                 ret = self.cluster_join(args)
+            elif sub_command == 'add':
+                ret = self.cluster_add(args)
             elif sub_command == 'status':
                 cluster_id = args.cluster_id
                 ret = cluster_ops.show_cluster(cluster_id)
             elif sub_command == 'list':
                 ret = cluster_ops.list()
             elif sub_command == 'suspend':
                 cluster_id = args.cluster_id
@@ -1056,37 +864,18 @@
                 ret = cluster_ops.update_cluster(args.id)
 
             elif sub_command == "list-tasks":
                 ret = cluster_ops.list_tasks(args.cluster_id)
 
             elif sub_command == "graceful-shutdown":
                 ret = cluster_ops.cluster_grace_shutdown(args.id)
-                
+
             elif sub_command == "graceful-startup":
                 ret = cluster_ops.cluster_grace_startup(args.id)
-                
-            else:
-                self.parser.print_help()
 
-        elif args.command == 'compute-node':
-            sub_command = args_dict[args.command]
-            if sub_command == "add":
-                ret = compute_ops.add_compute_node(self.db_store)
-            elif sub_command == "reset":
-                ret = compute_ops.reset_compute_node(self.db_store)
-            elif sub_command == "remove":
-                ret = compute_ops.remove_compute_node(self.db_store)
-            elif sub_command == "suspend":
-                ret = compute_ops.suspend_compute_node(self.db_store)
-            elif sub_command == "resume":
-                ret = compute_ops.resume_compute_node(self.db_store)
-            elif sub_command == "shutdown":
-                ret = compute_ops.shutdown_compute_node(self.db_store)
-            elif sub_command == "list":
-                ret = compute_ops.list_compute_nodes(self.db_store, args.json)
             else:
                 self.parser.print_help()
 
         elif args.command == 'lvol':
             sub_command = args_dict[args.command]
             if sub_command == "add":
                 name = args.name
@@ -1141,26 +930,23 @@
                 data = lvol_controller.connect_lvol(id)
                 if data:
                     ret = "\n".join(con['connect'] for con in data)
             elif sub_command == "resize":
                 id = args.id
                 size = self.parse_size(args.size)
                 ret = lvol_controller.resize_lvol(id, size)
-            elif sub_command == "set-read-only":
-                id = args.id
-                ret = lvol_controller.set_read_only(id)
             elif sub_command == "create-snapshot":
                 id = args.id
                 name = args.name
                 ret = lvol_controller.create_snapshot(id, name)
             elif sub_command == "clone":
-                snapshot_id = args.snapshot_id
-                clone_name = args.clone_name
-                ret = lvol_controller.clone(snapshot_id, clone_name)
-
+                new_size = 0
+                if args.resize:
+                    new_size = self.parse_size(args.resize)
+                ret = snapshot_controller.clone(args.snapshot_id, args.clone_name, new_size)
             elif sub_command == "get-io-stats":
                 id = args.id
                 history = args.history
                 data = lvol_controller.get_io_stats(id, history)
                 if data:
                     ret = utils.print_table(data)
                 else:
@@ -1189,19 +975,15 @@
                 cluster_id = args.cluster_id
                 cluster_ip = args.cluster_ip
                 ifname = args.ifname
                 ret = cluster_ops.join_cluster(cluster_ip, cluster_id, "management", ifname, [], None, None)
             elif sub_command == "list":
                 ret = mgmt_ops.list_mgmt_nodes(args.json)
             elif sub_command == "remove":
-                ret = mgmt_ops.remove_mgmt_node(args.hostname)
-            elif sub_command == "show":
-                ret = mgmt_ops.show_cluster()
-            elif sub_command == "status":
-                ret = mgmt_ops.cluster_status()
+                ret = mgmt_ops.remove_mgmt_node(args.id)
             else:
                 self.parser.print_help()
 
         elif args.command == 'pool':
             sub_command = args_dict[args.command]
             if sub_command == "add":
                 ret = pool_controller.add_pool(
@@ -1267,15 +1049,18 @@
             if sub_command == "add":
                 ret = snapshot_controller.add(args.id, args.name)
             if sub_command == "list":
                 ret = snapshot_controller.list()
             if sub_command == "delete":
                 ret = snapshot_controller.delete(args.id)
             if sub_command == "clone":
-                ret = snapshot_controller.clone(args.id, args.lvol_name)
+                new_size = 0
+                if args.resize:
+                    new_size = self.parse_size(args.resize)
+                ret = snapshot_controller.clone(args.id, args.lvol_name, new_size)
 
         elif args.command in ['caching-node', 'cn']:
             sub_command = args_dict['caching-node']
             if sub_command == "deploy":
                 ret = caching_node_controller.deploy(args.ifname)
 
             if sub_command == "add-node":
@@ -1342,51 +1127,42 @@
         sort = args.sort
         if sort:
             sort = sort[0]
         is_json = args.json
         out = storage_ops.list_storage_devices(self.db_store, node_id, sort, is_json)
         return out
 
-    def cluster_init(self, args):
-        page_size_in_blocks = args.page_size_in_blocks
+    def cluster_add(self, args):
+        page_size_in_blocks = args.page_size
         blk_size = args.blk_size
-        model_ids = args.model_ids
         ha_type = args.ha_type
-        tls = args.tls == 'on'
-        auth_hosts_only = args.auth_hosts_only == 'on'
-        dhchap = args.dhchap
-        NQN = args.NQN
-        iSCSI = args.iSCSI
-        CLI_PASS = args.CLI_PASS
+        cap_warn = args.cap_warn
+        cap_crit = args.cap_crit
+        prov_cap_warn = args.prov_cap_warn
+        prov_cap_crit = args.prov_cap_crit
 
-        # TODO: Validate the inputs
         return cluster_ops.add_cluster(
-            blk_size, page_size_in_blocks, model_ids, ha_type, tls,
-            auth_hosts_only, dhchap, NQN, iSCSI, CLI_PASS)
+            blk_size, page_size_in_blocks, ha_type, cap_warn, cap_crit, prov_cap_warn, prov_cap_crit)
 
     def cluster_create(self, args):
         page_size_in_blocks = args.page_size
         blk_size = args.blk_size
         ha_type = args.ha_type
-        tls = args.tls == 'on'
-        auth_hosts_only = args.auth_hosts_only == 'on'
         CLI_PASS = args.CLI_PASS
-        model_ids = args.model_ids
         cap_warn = args.cap_warn
         cap_crit = args.cap_crit
         prov_cap_warn = args.prov_cap_warn
         prov_cap_crit = args.prov_cap_crit
         ifname = args.ifname
         log_del_interval = args.log_del_interval
         metrics_retention_period = args.metrics_retention_period
 
-        # TODO: Validate the inputs
         return cluster_ops.create_cluster(
-            blk_size, page_size_in_blocks, ha_type, tls,
-            auth_hosts_only, CLI_PASS, model_ids, cap_warn, cap_crit, prov_cap_warn, prov_cap_crit,
+            blk_size, page_size_in_blocks, ha_type,
+            CLI_PASS, cap_warn, cap_crit, prov_cap_warn, prov_cap_crit,
             ifname, log_del_interval, metrics_retention_period)
 
     def cluster_join(self, args):
         cluster_id = args.cluster_id
         cluster_ip = args.cluster_ip
         role = args.role
         ifname = args.ifname
```

## Comparing `sbcli_mc-1.0.1/simplyblock_web/node_webapp.py` & `sbcli_mc-1.0.2/simplyblock_web/node_webapp.py`

 * *Files identical despite different names*

## Comparing `sbcli_mc-1.0.1/simplyblock_web/snode_app.py` & `sbcli_mc-1.0.2/simplyblock_web/snode_app.py`

 * *Files identical despite different names*

## Comparing `sbcli_mc-1.0.1/simplyblock_web/caching_node_app.py` & `sbcli_mc-1.0.2/simplyblock_web/caching_node_app.py`

 * *Files identical despite different names*

## Comparing `sbcli_mc-1.0.1/simplyblock_web/auth_middleware.py` & `sbcli_mc-1.0.2/simplyblock_web/auth_middleware.py`

 * *Files identical despite different names*

## Comparing `sbcli_mc-1.0.1/simplyblock_web/node_utils.py` & `sbcli_mc-1.0.2/simplyblock_web/node_utils.py`

 * *Files identical despite different names*

## Comparing `sbcli_mc-1.0.1/simplyblock_web/utils.py` & `sbcli_mc-1.0.2/simplyblock_web/utils.py`

 * *Files identical despite different names*

## Comparing `sbcli_mc-1.0.1/simplyblock_web/app.py` & `sbcli_mc-1.0.2/simplyblock_web/app.py`

 * *Files 2% similar despite different names*

```diff
@@ -1,20 +1,21 @@
 #!/usr/bin/env python
 # encoding: utf-8
 
 import logging
+import sys
 from flask import Flask
 
 import utils
 from blueprints import csi, web_api_cluster, web_api_mgmt_node, web_api_device, \
     web_api_lvol, web_api_storage_node, web_api_pool, web_api_caching_node
 from auth_middleware import token_required
 from simplyblock_core import constants
 
-logger_handler = logging.StreamHandler()
+logger_handler = logging.StreamHandler(sys.stdout)
 logger_handler.setFormatter(logging.Formatter('%(asctime)s: %(levelname)s: %(message)s'))
 logger = logging.getLogger()
 logger.addHandler(logger_handler)
 logger.setLevel(logging.DEBUG)
 
 
 app = Flask(__name__)
```

## Comparing `sbcli_mc-1.0.1/simplyblock_web/caching_node_app_k8s.py` & `sbcli_mc-1.0.2/simplyblock_web/caching_node_app_k8s.py`

 * *Files identical despite different names*

## Comparing `sbcli_mc-1.0.1/simplyblock_web/static/delete.py` & `sbcli_mc-1.0.2/simplyblock_web/static/delete.py`

 * *Files identical despite different names*

## Comparing `sbcli_mc-1.0.1/simplyblock_web/static/deploy_spdk.yaml` & `sbcli_mc-1.0.2/simplyblock_web/static/deploy_spdk.yaml`

 * *Files identical despite different names*

## Comparing `sbcli_mc-1.0.1/simplyblock_web/static/deploy.py` & `sbcli_mc-1.0.2/simplyblock_web/static/deploy.py`

 * *Files identical despite different names*

## Comparing `sbcli_mc-1.0.1/simplyblock_web/blueprints/web_api_pool.py` & `sbcli_mc-1.0.2/simplyblock_web/blueprints/web_api_pool.py`

 * *Files 6% similar despite different names*

```diff
@@ -32,39 +32,56 @@
     for pool in pools:
         data.append(pool.get_clean_dict())
     return utils.get_response(data)
 
 
 @bp.route('/pool', methods=['POST'])
 def add_pool():
+    """
+        Params:
+        | name (required) | LVol name or id
+        | pool_max        | Pool maximum size: 10M, 10G, 10(bytes)
+        | lvol_max        | LVol maximum size: 10M, 10G, 10(bytes)
+        | no_secret       | pool is created with a secret
+        | max_rw_iops     | Maximum Read Write IO Per Second
+        | max_rw_mbytes   | Maximum Read Write Mega Bytes Per Second
+        | max_r_mbytes    | Maximum Read Mega Bytes Per Second
+        | max_w_mbytes    | Maximum Write Mega Bytes Per Second
+    """
     pool_data = request.get_json()
     if 'name' not in pool_data:
         return utils.get_response_error("missing required param: name", 400)
 
     name = pool_data['name']
     for p in db_controller.get_pools():
         if p.pool_name == name:
             return utils.get_response_error(f"Pool found with the same name: {name}", 400)
 
     pool_secret = True
     if 'no_secret' in pool_data:
         pool_secret = False
 
-    pool_max_size = utils.get_int_value_or_default(pool_data, "pool-max", 0)
-    lvol_max_size = utils.get_int_value_or_default(pool_data, "lvol-max", 0)
-    max_rw_iops = utils.get_int_value_or_default(pool_data, "max-rw-iops", 0)
-    max_rw_mbytes = utils.get_int_value_or_default(pool_data, "max-rw-mbytes", 0)
-    max_r_mbytes_per_sec = utils.get_int_value_or_default(pool_data, "max-r-mbytes", 0)
-    max_w_mbytes_per_sec = utils.get_int_value_or_default(pool_data, "max-w-mbytes", 0)
+    pool_max_size = 0
+    lvol_max_size = 0
+    if 'pool_max' in pool_data:
+        pool_max_size = utils.parse_size(pool_data['pool_max'])
+
+    if 'lvol_max' in pool_data:
+        lvol_max_size = utils.parse_size(pool_data['lvol_max'])
+
+    max_rw_iops = utils.get_int_value_or_default(pool_data, "max_rw_iops", 0)
+    max_rw_mbytes = utils.get_int_value_or_default(pool_data, "max_rw_mbytes", 0)
+    max_r_mbytes_per_sec = utils.get_int_value_or_default(pool_data, "max_r_mbytes", 0)
+    max_w_mbytes_per_sec = utils.get_int_value_or_default(pool_data, "max_w_mbytes", 0)
 
     ret = pool_controller.add_pool(
         name, pool_max_size, lvol_max_size, max_rw_iops, max_rw_mbytes,
         max_r_mbytes_per_sec, max_w_mbytes_per_sec, pool_secret)
 
-    return utils.get_response(ret, "Error")
+    return utils.get_response(ret)
 
 
 @bp.route('/pool/<string:uuid>', methods=['DELETE'])
 def delete_pool(uuid):
     pool = db_controller.get_pool_by_id(uuid)
     if not pool:
         return utils.get_response_error(f"Pool not found: {uuid}", 404)
```

## Comparing `sbcli_mc-1.0.1/simplyblock_web/blueprints/web_api_device.py` & `sbcli_mc-1.0.2/simplyblock_web/blueprints/web_api_device.py`

 * *Files identical despite different names*

## Comparing `sbcli_mc-1.0.1/simplyblock_web/blueprints/web_api_lvol.py` & `sbcli_mc-1.0.2/simplyblock_web/blueprints/web_api_lvol.py`

 * *Files identical despite different names*

## Comparing `sbcli_mc-1.0.1/simplyblock_web/blueprints/snode_ops.py` & `sbcli_mc-1.0.2/simplyblock_web/blueprints/snode_ops.py`

 * *Files identical despite different names*

## Comparing `sbcli_mc-1.0.1/simplyblock_web/blueprints/caching_node_ops.py` & `sbcli_mc-1.0.2/simplyblock_web/blueprints/caching_node_ops.py`

 * *Files identical despite different names*

## Comparing `sbcli_mc-1.0.1/simplyblock_web/blueprints/web_api_storage_node.py` & `sbcli_mc-1.0.2/simplyblock_web/blueprints/web_api_storage_node.py`

 * *Files identical despite different names*

## Comparing `sbcli_mc-1.0.1/simplyblock_web/blueprints/web_api_cluster.py` & `sbcli_mc-1.0.2/simplyblock_web/blueprints/web_api_cluster.py`

 * *Files 3% similar despite different names*

```diff
@@ -121,24 +121,14 @@
     if not cluster:
         logger.error(f"Cluster not found {uuid}")
         return utils.get_response_error(f"Cluster not found: {uuid}", 404)
     data = cluster_ops.show_cluster(uuid, is_json=True)
     return utils.get_response(json.loads(data))
 
 
-@bp.route('/cluster/enable/<string:uuid>', methods=['PUT'])
-def cluster_enable(uuid):
-    return utils.get_response("Not Implemented!")
-
-
-@bp.route('/cluster/disable/<string:uuid>', methods=['PUT'])
-def cluster_disable(uuid):
-    return utils.get_response("Not Implemented!")
-
-
 @bp.route('/cluster/get-logs/<string:uuid>', methods=['GET'])
 def cluster_get_logs(uuid):
     cluster = db_controller.get_cluster_by_id(uuid)
     if not cluster:
         return utils.get_response_error(f"Cluster not found: {uuid}", 404)
     if cluster.status == Cluster.STATUS_INACTIVE:
         return utils.get_response("Cluster already inactive")
```

## Comparing `sbcli_mc-1.0.1/simplyblock_web/blueprints/caching_node_ops_k8s.py` & `sbcli_mc-1.0.2/simplyblock_web/blueprints/caching_node_ops_k8s.py`

 * *Files identical despite different names*

## Comparing `sbcli_mc-1.0.1/simplyblock_web/blueprints/node_api_caching_ks.py` & `sbcli_mc-1.0.2/simplyblock_web/blueprints/node_api_caching_ks.py`

 * *Files identical despite different names*

## Comparing `sbcli_mc-1.0.1/simplyblock_web/blueprints/node_api_caching_docker.py` & `sbcli_mc-1.0.2/simplyblock_web/blueprints/node_api_caching_docker.py`

 * *Files identical despite different names*

## Comparing `sbcli_mc-1.0.1/simplyblock_web/blueprints/web_api_caching_node.py` & `sbcli_mc-1.0.2/simplyblock_web/blueprints/web_api_caching_node.py`

 * *Files identical despite different names*

## Comparing `sbcli_mc-1.0.1/simplyblock_web/blueprints/node_api_basic.py` & `sbcli_mc-1.0.2/simplyblock_web/blueprints/node_api_basic.py`

 * *Files identical despite different names*

## Comparing `sbcli_mc-1.0.1/simplyblock_web/blueprints/csi.py` & `sbcli_mc-1.0.2/simplyblock_web/blueprints/csi.py`

 * *Files identical despite different names*

## Comparing `sbcli_mc-1.0.1/simplyblock_web/blueprints/web_api_mgmt_node.py` & `sbcli_mc-1.0.2/simplyblock_web/blueprints/web_api_mgmt_node.py`

 * *Files identical despite different names*

## Comparing `sbcli_mc-1.0.1/simplyblock_web/templates/deploy_spdk.yaml.j2` & `sbcli_mc-1.0.2/simplyblock_web/templates/deploy_spdk.yaml.j2`

 * *Files identical despite different names*

## Comparing `sbcli_mc-1.0.1/simplyblock_core/cluster_ops.py` & `sbcli_mc-1.0.2/simplyblock_core/cluster_ops.py`

 * *Files 3% similar despite different names*

```diff
@@ -41,16 +41,16 @@
     }
     session = requests.session()
     session.auth = ("admin", password)
     response = session.request("POST", url, headers=headers, data=payload)
     logger.debug(response.text)
     return response.status_code == 201
 
-def create_cluster(blk_size, page_size_in_blocks, ha_type, tls,
-                   auth_hosts_only, cli_pass, model_ids,
+
+def create_cluster(blk_size, page_size_in_blocks, ha_type, cli_pass,
                    cap_warn, cap_crit, prov_cap_warn, prov_cap_crit, ifname, log_del_interval, metrics_retention_period):
     logger.info("Installing dependencies...")
     ret = scripts.install_deps()
     logger.info("Installing dependencies > Done")
 
     if not ifname:
         ifname = "eth0"
@@ -85,18 +85,15 @@
 
     # validate cluster duplicate
     logger.info("Adding new cluster object")
     c = Cluster()
     c.uuid = str(uuid.uuid4())
     c.blk_size = blk_size
     c.page_size_in_blocks = page_size_in_blocks
-    c.model_ids = model_ids
     c.ha_type = ha_type
-    c.tls = tls
-    c.auth_hosts_only = auth_hosts_only
     c.nqn = f"{constants.CLUSTER_NQN}:{c.uuid}"
     c.cli_pass = cli_pass
     c.secret = utils.generate_string(20)
     c.db_connection = db_connection
     if cap_warn and cap_warn > 0:
         c.cap_warn = cap_warn
     if cap_crit and cap_crit > 0:
@@ -354,35 +351,41 @@
                     logger.info(f"Container status: {status}, Is Running: {is_running}")
                 break
         storage_node_ops.add_storage_node(cluster_id, ifname, data_nics)
 
     logger.info("Node joined the cluster")
 
 
-def add_cluster(blk_size, page_size_in_blocks, model_ids, ha_type, tls,
-                auth_hosts_only, dhchap, nqn, iscsi, cli_pass):
+def add_cluster(blk_size, page_size_in_blocks, ha_type, cap_warn, cap_crit, prov_cap_warn, prov_cap_crit):
     db_controller = DBController()
     logger.info("Adding new cluster")
-    c = Cluster()
-    c.uuid = str(uuid.uuid4())
-    c.blk_size = blk_size
-    c.page_size_in_blocks = page_size_in_blocks
-    c.model_ids = model_ids
-    c.ha_type = ha_type
-    c.tls = tls
-    c.auth_hosts_only = auth_hosts_only
-    c.nqn = nqn
-    c.iscsi = iscsi
-    c.dhchap = dhchap
-    c.cli_pass = cli_pass
-    c.status = Cluster.STATUS_ACTIVE
-    c.updated_at = int(time.time())
-    c.write_to_db(db_controller.kv_store)
-    logger.info("New Cluster has been created")
-    logger.info(c.uuid)
+    default_cluster = db_controller.get_clusters()[0]
+    cluster = Cluster()
+    cluster.uuid = str(uuid.uuid4())
+    cluster.blk_size = blk_size
+    cluster.page_size_in_blocks = page_size_in_blocks
+    cluster.ha_type = ha_type
+    cluster.nqn = f"{constants.CLUSTER_NQN}:{cluster.uuid}"
+    cluster.cli_pass = default_cluster.cli_pass
+    cluster.secret = utils.generate_string(20)
+    cluster.db_connection = default_cluster.db_connection
+    if cap_warn and cap_warn > 0:
+        cluster.cap_warn = cap_warn
+    if cap_crit and cap_crit > 0:
+        cluster.cap_crit = cap_crit
+    if prov_cap_warn and prov_cap_warn > 0:
+        cluster.prov_cap_warn = prov_cap_warn
+    if prov_cap_crit and prov_cap_crit > 0:
+        cluster.prov_cap_crit = prov_cap_crit
+
+    cluster.status = Cluster.STATUS_ACTIVE
+    cluster.updated_at = int(time.time())
+    cluster.write_to_db(db_controller.kv_store)
+    cluster_events.cluster_create(cluster)
+    return cluster.get_id()
 
 
 def show_cluster(cl_id, is_json=False):
     db_controller = DBController()
     cluster = db_controller.get_cluster_by_id(cl_id)
     if not cluster:
         logger.error(f"Cluster not found {cl_id}")
```

## Comparing `sbcli_mc-1.0.1/simplyblock_core/pci_utils.py` & `sbcli_mc-1.0.2/simplyblock_core/pci_utils.py`

 * *Files identical despite different names*

## Comparing `sbcli_mc-1.0.1/simplyblock_core/snode_client.py` & `sbcli_mc-1.0.2/simplyblock_core/snode_client.py`

 * *Files identical despite different names*

## Comparing `sbcli_mc-1.0.1/simplyblock_core/kv_store.py` & `sbcli_mc-1.0.2/simplyblock_core/kv_store.py`

 * *Files identical despite different names*

## Comparing `sbcli_mc-1.0.1/simplyblock_core/compute_node_ops.py` & `sbcli_mc-1.0.2/simplyblock_core/compute_node_ops.py`

 * *Files identical despite different names*

## Comparing `sbcli_mc-1.0.1/simplyblock_core/rpc_client.py` & `sbcli_mc-1.0.2/simplyblock_core/rpc_client.py`

 * *Files 8% similar despite different names*

```diff
@@ -115,17 +115,15 @@
         params = None
         if trtype:
             params = {"trtype": trtype}
         return self._request("nvmf_get_transports", params)
 
     def transport_create(self, trtype):
         params = {
-            "trtype": trtype,
-#            "max_io_qpairs_per_ctrlr": 65000,
-#            "max_queue_depth": 65000,
+            "trtype": trtype
         }
         return self._request("nvmf_create_transport", params)
 
     def listeners_list(self, nqn):
         params = {"nqn": nqn}
         return self._request("nvmf_subsystem_get_listeners", params)
 
@@ -171,24 +169,14 @@
             "ns_id": 1,
             "label": "SYSVMS84-x86",
             "desc": "A volume to keep OpenVMS/VAX/Alpha/IA64/x86 operation system data",
             "pagesz": 16384
         }
         return self._request2("ultra21_alloc_ns_init", params)
 
-    def create_nvme_partitions(self, params):
-        # this is not implemented in the spdk side, will not issue a request.
-        # TODO: implement
-        return params
-
-    def allocate_bdev(self, name, sn):
-        # this is not implemented in the spdk side, will not issue a request.
-        # TODO: implement
-        return name, sn
-
     def nvmf_subsystem_add_ns(self, nqn, dev_name, uuid=None, nguid=None):
         params = {
             "nqn": nqn,
             "namespace": {
                 "bdev_name": dev_name
             }
         }
@@ -220,53 +208,18 @@
         if is_optimized:
             params['ana_state'] = "optimized"
         else:
             params['ana_state'] = "non_optimized"
 
         return self._request("nvmf_subsystem_listener_set_ana_state", params)
 
-    def get_device_status(self, device_name):
-        # TODO: to be implemented
-        return {
-            "jsonrpc": "2.0",
-            "id": 1,
-            "result": {
-                'name': device_name,
-                'status': 'live'
-            }
-        }
-
     def get_device_stats(self, uuid):
         params = {"name": uuid}
         return self._request("bdev_get_iostat", params)
 
-    def shutdown_node(self, node_id):
-        # TODO: to be implemented
-        return {
-            "jsonrpc": "2.0",
-            "id": 1,
-            "result": True
-        }
-
-    def suspend_node(self, node_id):
-        # TODO: to be implemented
-        return {
-            "jsonrpc": "2.0",
-            "id": 1,
-            "result": True
-        }
-
-    def resume_node(self, node_id):
-        # TODO: to be implemented
-        return {
-            "jsonrpc": "2.0",
-            "id": 1,
-            "result": True
-        }
-
     def reset_device(self, device_name):
         params = {"name": device_name}
         return self._request("bdev_nvme_reset_controller", params)
 
     def create_lvstore(self, name, bdev_name):
         params = {"bdev_name": bdev_name, "lvs_name": name}
         return self._request("bdev_lvol_create_lvstore", params)
@@ -472,14 +425,15 @@
             "trtype": "tcp",
             "traddr": ip,
             "adrfam": "ipv4",
             "trsvcid": str(port),
             "subnqn": nqn,
             "fabrics_connect_timeout_us": 100000,
             "fast_io_fail_timeout_sec": 0,
+            "num_io_queues": 16384,
         }
         return self._request("bdev_nvme_attach_controller", params)
 
     def bdev_split(self, base_bdev, split_count):
         params = {
             "base_bdev": base_bdev,
             "split_count": split_count
@@ -522,14 +476,16 @@
     def bdev_nvme_set_options(self):
         params = {
             "bdev_retry_count": 0,
             "transport_retry_count": 0,
             "ctrlr_loss_timeout_sec": -1,
             "fast_io_fail_timeout_sec": 5,
             "reconnect_delay_sec": 5,
+            "keep_alive_timeout_ms": 200,
+            "transport_ack_timeout": 7
         }
         return self._request("bdev_nvme_set_options", params)
 
     def bdev_set_options(self, bdev_io_pool_size, bdev_io_cache_size, iobuf_small_cache_size, iobuf_large_cache_size):
         params = {}
         if bdev_io_pool_size > 0:
             params['bdev_io_pool_size'] = bdev_io_pool_size
@@ -555,15 +511,14 @@
         if large_bufsize > 0:
             params['large_bufsize'] = large_bufsize
         if params:
             return self._request("iobuf_set_options", params)
         else:
             return False
 
-
     def distr_status_events_get(self):
         return self._request("distr_status_events_get")
 
     def alceml_get_capacity(self, name):
         params = {"name": name}
         return self._request("alceml_get_pages_usage", params)
 
@@ -602,21 +557,19 @@
             "modus": "SNAPSHOT",
             "lvol_bdev": lvol_bdev,
             "base_bdev": base_bdev,
             "snapshot_bdev": snapshot_name
         }
         return self._request("ultra21_lvol_mount", params)
 
-    def ultra21_lvol_mount_lvol(self, lvol_name, base_bdev, label, desc):
+    def ultra21_lvol_mount_lvol(self, lvol_name, base_bdev):
         params = {
             "modus": "BASE",
             "lvol_bdev": lvol_name,
-            "base_bdev": base_bdev,
-            # "label": label,
-            # "desc": desc
+            "base_bdev": base_bdev
         }
         return self._request("ultra21_lvol_mount", params)
 
     def ultra21_lvol_dismount(self, lvol_name):
         params = {
             "lvol_bdev": lvol_name
         }
```

## Comparing `sbcli_mc-1.0.1/simplyblock_core/mgmt_node_ops.py` & `sbcli_mc-1.0.2/simplyblock_core/services/mgmt_node_monitor.py`

 * *Files 24% similar despite different names*

```diff
@@ -1,116 +1,96 @@
 # coding=utf-8
-import datetime
-import json
 import logging
-import uuid
+import os
 
-import docker
+import time
+import sys
+from datetime import datetime
 
-from simplyblock_core import utils
+
+from simplyblock_core import constants, kv_store, utils
 from simplyblock_core.controllers import mgmt_events
-from simplyblock_core.kv_store import DBController
 from simplyblock_core.models.mgmt_node import MgmtNode
 
-logger = logging.getLogger()
-
+# Import the GELF logger
+from graypy import GELFUDPHandler
 
-def add_mgmt_node(mgmt_ip, cluster_id=None):
-    db_controller = DBController()
-    hostname = utils.get_hostname()
-    node = db_controller.get_mgmt_node_by_hostname(hostname)
-    if node:
-        logger.error("Node already exists in the cluster")
+# configure logging
+logger_handler = logging.StreamHandler(stream=sys.stdout)
+logger_handler.setFormatter(logging.Formatter('%(asctime)s: %(levelname)s: %(message)s'))
+gelf_handler = GELFUDPHandler('0.0.0.0', constants.GELF_PORT)
+logger = logging.getLogger()
+logger.addHandler(gelf_handler)
+logger.addHandler(logger_handler)
+logger.setLevel(logging.DEBUG)
+
+
+# get DB controller
+db_store = kv_store.KVStore()
+db_controller = kv_store.DBController(kv_store=db_store)
+
+def set_node_online(node):
+    if node.status == MgmtNode.STATUS_UNREACHABLE:
+        snode = db_controller.get_mgmt_node_by_id(node.get_id())
+        old_status = snode.status
+        snode.status = MgmtNode.STATUS_ONLINE
+        snode.updated_at = str(datetime.now())
+        snode.write_to_db(db_store)
+        mgmt_events.status_change(snode, snode.status, old_status, caused_by="monitor")
+
+
+def set_node_offline(node):
+    if node.status == MgmtNode.STATUS_ONLINE:
+        snode = db_controller.get_mgmt_node_by_id(node.get_id())
+        old_status = snode.status
+        snode.status = MgmtNode.STATUS_UNREACHABLE
+        snode.updated_at = str(datetime.now())
+        snode.write_to_db(db_store)
+        mgmt_events.status_change(snode, snode.status, old_status, caused_by="monitor")
+
+
+def ping_host(ip):
+    logger.info(f"Pinging ip {ip}")
+    response = os.system(f"ping -c 1 {ip}")
+    if response == 0:
+        logger.info(f"{ip} is UP")
+        return True
+    else:
+        logger.info(f"{ip} is DOWN")
         return False
 
-    node = MgmtNode()
-    node.system_uuid = str(uuid.uuid4())
-    node.hostname = hostname
-    node.docker_ip_port = f"{mgmt_ip}:2375"
-    node.cluster_id = cluster_id
-    node.mgmt_ip = mgmt_ip
-    node.status = MgmtNode.STATUS_ONLINE
-    node.write_to_db(db_controller.kv_store)
-
-    mgmt_events.mgmt_add(node)
-    logger.info("Done")
-    return True
 
+logger.info("Starting Mgmt node monitor")
 
-def list_mgmt_nodes(is_json):
-    db_controller = DBController()
-    nodes = db_controller.get_mgmt_nodes()
-    data = []
-    output = ""
 
+while True:
+    # get storage nodes
+    nodes = db_controller.get_mgmt_nodes()
     for node in nodes:
-        logging.debug(node)
-        logging.debug("*" * 20)
-        data.append({
-            "Hostname": node.hostname,
-            "IP": node.docker_ip_port.split(":")[0],
-            "Status": node.status,
-        })
-
-    if not data:
-        return output
-
-    if is_json:
-        output = json.dumps(data, indent=2)
-    else:
-        output = utils.print_table(data)
-    return output
-
-
-def remove_mgmt_node(hostname):
-    db_controller = DBController()
-    logging.info("removing mgmt node")
-    snode = db_controller.get_mgmt_node_by_hostname(hostname)
-    if not snode:
-        logger.error("can not find node")
-        exit(1)
-
-    snode.remove(db_controller.kv_store)
-
-    logger.info("Leaving swarm...")
-    node_docker = docker.DockerClient(base_url=f"tcp://{snode.docker_ip_port}", version="auto")
-    node_docker.swarm.leave()
-
-    mgmt_events.mgmt_remove(snode)
-    logging.info("done")
-
-
-def show_cluster():
-    c = utils.get_docker_client()
-    nl = c.nodes.list(filters={'role': 'manager'})
-    nodes = []
-    for n in nl:
-        nodes.append({
-            "Hostname": n.attrs['Description']['Hostname'],
-            "IP": n.attrs['ManagerStatus']['Addr'].split(":")[0],
-            "Status": n.attrs['Status']['State'],
-            "UpdatedAt": datetime.datetime.strptime(n.attrs['UpdatedAt'][:26], "%Y-%m-%dT%H:%M:%S.%f").strftime(
-                "%H:%M:%S, %d/%m/%Y"),
-        })
-    return utils.print_table(nodes)
-
-
-def cluster_status():
-    c = utils.get_docker_client()
-    ns = c.nodes.list(filters={'role': 'manager'})
-    total_nodes = len(ns)
-    active_nodes = 0
-    lead_node = None
-    for n in ns:
-        if n.attrs['Status']['State'] == 'ready':
-            active_nodes += 1
-        if 'Leader' in n.attrs['ManagerStatus'] and n.attrs['ManagerStatus']['Leader']:
-            lead_node = n.attrs['Description']['Hostname']
-
-    status = {
-        "Status": "Online",
-        "Active Nodes": active_nodes,
-        "Total nodes": total_nodes,
-        "Leader": lead_node
-    }
+        if node.status not in [MgmtNode.STATUS_ONLINE, MgmtNode.STATUS_UNREACHABLE]:
+            logger.info(f"Node status is: {node.status}, skipping")
+            continue
+
+        logger.info(f"Checking node {node.hostname}")
+        if not ping_host(node.mgmt_ip):
+            logger.info(f"Node {node.hostname} is offline")
+            set_node_offline(node)
+            continue
+
+        c = utils.get_docker_client()
+        nl = c.nodes.list(filters={'role': 'manager'})
+        docker_node = None
+        for n in nl:
+            if n.attrs['Description']['Hostname'] == node.hostname:
+                docker_node = n
+                break
+        if docker_node:
+            logger.error("Node is not part of the docker swarm!")
+            continue
+
+        if n.attrs['Spec']['Availability'] == 'active':
+            set_node_online(node)
+        else:
+            set_node_online(node)
 
-    return utils.print_table([status])
+    logger.info(f"Sleeping for {constants.NODE_MONITOR_INTERVAL_SEC} seconds")
+    time.sleep(constants.NODE_MONITOR_INTERVAL_SEC)
```

## Comparing `sbcli_mc-1.0.1/simplyblock_core/utils.py` & `sbcli_mc-1.0.2/simplyblock_core/utils.py`

 * *Files identical despite different names*

## Comparing `sbcli_mc-1.0.1/simplyblock_core/distr_controller.py` & `sbcli_mc-1.0.2/simplyblock_core/distr_controller.py`

 * *Files identical despite different names*

## Comparing `sbcli_mc-1.0.1/simplyblock_core/cnode_client.py` & `sbcli_mc-1.0.2/simplyblock_core/cnode_client.py`

 * *Files identical despite different names*

## Comparing `sbcli_mc-1.0.1/simplyblock_core/storage_node_ops.py` & `sbcli_mc-1.0.2/simplyblock_core/storage_node_ops.py`

 * *Files 1% similar despite different names*

```diff
@@ -323,15 +323,15 @@
                 continue
             dev.remote_bdev = f"{name}n1"
             remote_devices.append(dev)
     return remote_devices
 
 
 def add_node(cluster_id, node_ip, iface_name, data_nics_list, spdk_cpu_mask,
-             spdk_mem, dev_split=1, spdk_image=None, spdk_debug=False,
+             spdk_mem, spdk_image=None, spdk_debug=False,
              small_pool_count=0, large_pool_count=0, small_bufsize=0, large_bufsize=0, jm_device_pcie=None):
     db_controller = DBController()
     kv_store = db_controller.kv_store
 
     cluster = db_controller.get_cluster_by_id(cluster_id)
     if not cluster:
         logger.error("Cluster not found: %s", cluster_id)
@@ -515,29 +515,15 @@
     node_info, _ = snode_api.info()
     # adding devices
     nvme_devs = addNvmeDevices(cluster, rpc_client, node_info['spdk_pcie_list'], snode)
     if not nvme_devs:
         logger.error("No NVMe devices was found!")
         return False
 
-    if dev_split > 1:
-        # split devices
-        new_devices = []
-        for dev in nvme_devs:
-            ret = rpc_client.bdev_split(dev.nvme_bdev, dev_split)
-            for pt in ret:
-                dev_dict = dev.get_clean_dict()
-                dev_dict['uuid'] = str(uuid.uuid4())
-                dev_dict['device_name'] = pt
-                dev_dict['nvme_bdev'] = pt
-                dev_dict['size'] = int(dev.size / dev_split)
-                new_devices.append(NVMeDevice(dev_dict))
-        snode.nvme_devices = new_devices
-    else:
-        snode.nvme_devices = nvme_devs
+    snode.nvme_devices = nvme_devs
 
     jm_device = snode.nvme_devices[0]
     # Set device cluster order
     dev_order = get_next_cluster_device_order(db_controller, cluster_id)
     for index, nvme in enumerate(snode.nvme_devices):
         nvme.cluster_device_order = dev_order
         dev_order += 1
@@ -774,15 +760,15 @@
         logger.info(f"Sending cluster map to LVol: {lvol.get_id()}")
         lvol_controller.send_cluster_map(lvol.get_id())
 
     storage_events.snode_delete(snode)
     logger.info("done")
 
 
-def remove_storage_node(node_id, force_remove=False, force_migrate=False):
+def remove_storage_node(node_id, force_remove=False):
     db_controller = DBController()
     snode = db_controller.get_storage_node_by_id(node_id)
     if not snode:
         logger.error(f"Can not find storage node: {node_id}")
         return False
 
     if snode.status == StorageNode.STATUS_ONLINE:
@@ -1335,15 +1321,15 @@
     snode.write_to_db(db_controller.kv_store)
 
     storage_events.snode_status_change(snode, snode.status, old_status)
     logger.info("Done")
     return True
 
 
-
+# not used in AWS, must run on bare-metal servers
 def run_test_storage_device(kv_store, dev_name):
     db_controller = DBController(kv_store)
     baseboard_sn = utils.get_baseboard_sn()
     snode = db_controller.get_storage_node_by_id(baseboard_sn)
     if not snode:
         logger.error("This storage node is not part of the cluster")
         exit(1)
@@ -1462,23 +1448,14 @@
                                                  nvme_device.pcie_address)
     logger.debug(ret)
 
     logger.debug("controllers list")
     ret = rpc_client.bdev_nvme_controller_list()
     logger.debug(ret)
 
-    # # create nvme partitions
-    # device_to_partition, status_ns = create_partitions_arrays(global_settings, nvme_devs)
-    # out_data = {
-    #     'device_to_partition': device_to_partition,
-    #     'status_ns': status_ns,
-    #     'NS_LB_SIZE': global_settings.NS_LB_SIZE,
-    #     'NS_SIZE_IN_LBS': global_settings.NS_SIZE_IN_LBS}
-    # rpc_client.create_nvme_partitions(out_data)
-
     # allocate bdevs
     logger.info("Allocating bdevs")
     ret = rpc_client.allocate_bdev(nvme_device.device_name, nvme_device.sequential_number)
     logger.debug(ret)
 
     # creating namespaces
     logger.info("Creating namespaces")
@@ -1499,19 +1476,14 @@
     logger.debug(cmap)
     cmap.write_to_db(kv_store)
 
     logger.info("Done")
     return True
 
 
-def replace_node(kv_store, old_node_name, iface_name):
-    return "Not implemented!"
-
-
-
 def get_node_capacity(node_id, history, records_count=20, parse_sizes=True):
     db_controller = DBController()
     this_node = db_controller.get_storage_node_by_id(node_id)
     if not this_node:
         logger.error("Storage node Not found")
         return
 
@@ -1831,31 +1803,14 @@
             "Key": key,
             "Value": ret[key],
             "Parsed": utils.humanbytes(ret[key])
         })
     return utils.print_table(data)
 
 
-def update(node_id, key, value):
-    db_controller = DBController()
-
-    snode = db_controller.get_storage_node_by_id(node_id)
-    if not snode:
-        logger.error(f"Can not find storage node: {node_id}")
-        return False
-
-    if key in snode._attribute_map:
-        setattr(snode, key, value)
-        snode.write_to_db(db_controller.kv_store)
-        return True
-    else:
-        logger.error("Key not found")
-        return False
-
-
 def get(node_id):
     db_controller = DBController()
 
     snode = db_controller.get_storage_node_by_id(node_id)
     if not snode:
         logger.error(f"Can not find storage node: {node_id}")
         return False
```

## Comparing `sbcli_mc-1.0.1/simplyblock_core/constants.py` & `sbcli_mc-1.0.2/simplyblock_core/constants.py`

 * *Files 10% similar despite different names*

```diff
@@ -50,11 +50,14 @@
 HEALTH_CHECK_INTERVAL_SEC = 60
 
 GRAYLOG_CHECK_INTERVAL_SEC = 60
 
 FDB_CHECK_INTERVAL_SEC = 60
 
 SIMPLY_BLOCK_DOCKER_IMAGE = "simplyblock/simplyblock:multi-cluster"
+SIMPLY_BLOCK_CLI_NAME = "sbcli-mc"
+TASK_EXEC_INTERVAL_SEC = 30
+
 SIMPLY_BLOCK_SPDK_CORE_IMAGE = "simplyblock/spdk-core:latest"
 SIMPLY_BLOCK_SPDK_ULTRA_IMAGE = "simplyblock/spdk:main-latest"
 
 GELF_PORT = 12201
```

## Comparing `sbcli_mc-1.0.1/simplyblock_core/services/job_tasks.py` & `sbcli_mc-1.0.2/simplyblock_core/services/job_tasks.py`

 * *Files 6% similar despite different names*

```diff
@@ -19,29 +19,31 @@
     node = db_controller.get_storage_node_by_id(task.node_id)
     for dev in node.nvme_devices:
         if dev.get_id() == task.device_id:
             return dev
 
 
 def task_runner(task):
+    device = _get_device(task)
+
     if task.retry <= 0:
         task.function_result = "timeout"
         task.status = JobSchedule.STATUS_DONE
         task.write_to_db(db_controller.kv_store)
+        device_controller.device_set_unavailable(device.get_id())
         return
 
     node = db_controller.get_storage_node_by_id(task.node_id)
     if node.status != StorageNode.STATUS_ONLINE:
         logger.error(f"Node is not online: {node.get_id()} , skipping task: {task.get_id()}")
         task.function_result = "Node is offline"
         task.retry -= 1
         task.write_to_db(db_controller.kv_store)
         return
 
-    device = _get_device(task)
     if device.status == NVMeDevice.STATUS_ONLINE and device.io_error is False:
         logger.info(f"Device is online: {device.get_id()}, no restart needed")
         task.function_result = "skipped because dev is online"
         task.status = JobSchedule.STATUS_DONE
         task.write_to_db(db_controller.kv_store)
         return
 
@@ -97,8 +99,8 @@
     else:
         for cl in clusters:
             tasks = db_controller.get_job_tasks(cl.get_id())
             for task in tasks:
                 if task.status != JobSchedule.STATUS_DONE:
                     res = task_runner(task)
 
-    time.sleep(5)
+    time.sleep(constants.TASK_EXEC_INTERVAL_SEC)
```

## Comparing `sbcli_mc-1.0.1/simplyblock_core/services/caching_node_monitor.py` & `sbcli_mc-1.0.2/simplyblock_core/services/caching_node_monitor.py`

 * *Files identical despite different names*

## Comparing `sbcli_mc-1.0.1/simplyblock_core/services/install_service.sh` & `sbcli_mc-1.0.2/simplyblock_core/services/install_service.sh`

 * *Files identical despite different names*

## Comparing `sbcli_mc-1.0.1/simplyblock_core/services/__init__.py` & `sbcli_mc-1.0.2/simplyblock_core/services/__init__.py`

 * *Files identical despite different names*

## Comparing `sbcli_mc-1.0.1/simplyblock_core/services/log_agg_service.py` & `sbcli_mc-1.0.2/simplyblock_core/services/log_agg_service.py`

 * *Files identical despite different names*

## Comparing `sbcli_mc-1.0.1/simplyblock_core/services/health_check_service.py` & `sbcli_mc-1.0.2/simplyblock_core/services/health_check_service.py`

 * *Files identical despite different names*

## Comparing `sbcli_mc-1.0.1/simplyblock_core/services/capacity_and_stats_collector.py` & `sbcli_mc-1.0.2/simplyblock_core/services/capacity_and_stats_collector.py`

 * *Files identical despite different names*

## Comparing `sbcli_mc-1.0.1/simplyblock_core/services/device_monitor.py` & `sbcli_mc-1.0.2/simplyblock_core/services/device_monitor.py`

 * *Files identical despite different names*

## Comparing `sbcli_mc-1.0.1/simplyblock_core/services/lvol_stat_collector.py` & `sbcli_mc-1.0.2/simplyblock_core/services/lvol_stat_collector.py`

 * *Files identical despite different names*

## Comparing `sbcli_mc-1.0.1/simplyblock_core/services/cap_monitor.py` & `sbcli_mc-1.0.2/simplyblock_core/services/cap_monitor.py`

 * *Files identical despite different names*

## Comparing `sbcli_mc-1.0.1/simplyblock_core/services/storage_node_monitor.py` & `sbcli_mc-1.0.2/simplyblock_core/services/storage_node_monitor.py`

 * *Files identical despite different names*

## Comparing `sbcli_mc-1.0.1/simplyblock_core/services/port_stat_collector.py` & `sbcli_mc-1.0.2/simplyblock_core/services/port_stat_collector.py`

 * *Files identical despite different names*

## Comparing `sbcli_mc-1.0.1/simplyblock_core/services/distr_event_collector.py` & `sbcli_mc-1.0.2/simplyblock_core/services/distr_event_collector.py`

 * *Files identical despite different names*

## Comparing `sbcli_mc-1.0.1/simplyblock_core/services/lvol_monitor.py` & `sbcli_mc-1.0.2/simplyblock_core/services/lvol_monitor.py`

 * *Files identical despite different names*

## Comparing `sbcli_mc-1.0.1/simplyblock_core/controllers/pool_controller.py` & `sbcli_mc-1.0.2/simplyblock_core/controllers/pool_controller.py`

 * *Files identical despite different names*

## Comparing `sbcli_mc-1.0.1/simplyblock_core/controllers/storage_events.py` & `sbcli_mc-1.0.2/simplyblock_core/controllers/storage_events.py`

 * *Files identical despite different names*

## Comparing `sbcli_mc-1.0.1/simplyblock_core/controllers/lvol_controller.py` & `sbcli_mc-1.0.2/simplyblock_core/controllers/lvol_controller.py`

 * *Files 1% similar despite different names*

```diff
@@ -636,17 +636,15 @@
         lvol.snapshot_name = f"snapshot_{lvol.vuid}_{name}"
         lvol.top_bdev = f"lvol_{lvol.vuid}_{lvol.lvol_name}"
         lvol.bdev_stack.append({
             "type": "ultra_lvol",
             "name": lvol.top_bdev,
             "params": {
                 "lvol_name": lvol.top_bdev,
-                "base_bdev": lvol.base_bdev,
-                "label": "label",
-                "desc": "desc"
+                "base_bdev": lvol.base_bdev
             }
         })
     else:
         lvol.bdev_stack.append({
             "type": "bdev_distr",
             "name": lvol.base_bdev,
             "params": {
@@ -887,24 +885,18 @@
     for bdev in bdev_stack:
         if 'status' in bdev and bdev['status'] == 'deleted':
             continue
 
         type = bdev['type']
         name = bdev['name']
         ret = None
-        # if type == "alceml":
-        #     ret = rpc_client.bdev_alceml_delete(name)
         if type == "bdev_distr":
             ret = rpc_client.bdev_distrib_delete(name)
-        # elif type == "lvs":
-        #     ret = rpc_client.bdev_lvol_delete_lvstore(name)
-        # elif type == "lvol":
-        #     ret = rpc_client.delete_lvol(name)
-        # elif type == "ultra_pt":
-        #     ret = rpc_client.ultra21_bdev_pass_delete(name)
+        elif type == "bmap_init":
+            pass
         elif type == "ultra_lvol":
             ret = rpc_client.ultra21_lvol_dismount(name)
         elif type == "comp":
             ret = rpc_client.lvol_compress_delete(name)
         elif type == "crypto":
             ret = rpc_client.lvol_crypto_delete(name)
         else:
@@ -1016,29 +1008,28 @@
     # remove from storage node
     snode.lvols.remove(lvol.get_id())
     snode.write_to_db(db_controller.kv_store)
 
     # remove from pool
     pool.lvols.remove(lvol.get_id())
     pool.write_to_db(db_controller.kv_store)
-
+    lvol_events.lvol_delete(lvol)
     lvol.remove(db_controller.kv_store)
 
     # if lvol is clone and snapshot is deleted, then delete snapshot
     if lvol.cloned_from_snap:
         snap = db_controller.get_snapshot_by_id(lvol.cloned_from_snap)
         if snap.deleted is True:
             lvols_count = 0
             for lvol in db_controller.get_lvols():
                 if lvol.cloned_from_snap == snap.get_id():
                     lvols_count += 1
             if lvols_count == 0:
                 snapshot_controller.delete(snap.get_id())
 
-    lvol_events.lvol_delete(lvol)
     logger.info("Done")
     return True
 
 
 def set_lvol(uuid, max_rw_iops, max_rw_mbytes, max_r_mbytes, max_w_mbytes, name=None):
     lvol = db_controller.get_lvol_by_id(uuid)
     if not lvol:
@@ -1278,18 +1269,14 @@
     return True
 
 
 def create_snapshot(lvol_id, snapshot_name):
     return snapshot_controller.add(lvol_id, snapshot_name)
 
 
-def clone(snapshot_id, clone_name):
-    return snapshot_controller.clone(snapshot_id, clone_name)
-
-
 def get_capacity(id, history):
     lvol = db_controller.get_lvol_by_id(id)
     if not lvol:
         logger.error(f"lvol not found: {id}")
         return False
 
     out = [{
```

## Comparing `sbcli_mc-1.0.1/simplyblock_core/controllers/device_events.py` & `sbcli_mc-1.0.2/simplyblock_core/controllers/device_events.py`

 * *Files identical despite different names*

## Comparing `sbcli_mc-1.0.1/simplyblock_core/controllers/lvol_events.py` & `sbcli_mc-1.0.2/simplyblock_core/controllers/lvol_events.py`

 * *Files identical despite different names*

## Comparing `sbcli_mc-1.0.1/simplyblock_core/controllers/snapshot_controller.py` & `sbcli_mc-1.0.2/simplyblock_core/controllers/snapshot_controller.py`

 * *Files 4% similar despite different names*

```diff
@@ -154,15 +154,15 @@
         lvol_controller.delete_lvol(base_lvol.get_id())
 
     logger.info("Done")
     snapshot_events.snapshot_delete(snap)
     return True
 
 
-def clone(snapshot_id, clone_name):
+def clone(snapshot_id, clone_name, new_size=0):
     snap = db_controller.get_snapshot_by_id(snapshot_id)
     if not snap:
         logger.error(f"Snapshot not found {snapshot_id}")
         return False
 
     pool = db_controller.get_pool_by_id(snap.lvol.pool_uuid)
     if not pool:
@@ -181,43 +181,45 @@
         logger.error("Storage node has no nvme devices")
         return False
 
     if snode.status != snode.STATUS_ONLINE:
         logger.error("Storage node in not Online")
         return False
 
-    # creating RPCClient instance
-    rpc_client = RPCClient(
-        snode.mgmt_ip,
-        snode.rpc_port,
-        snode.rpc_username,
-        snode.rpc_password)
-
     if not snode.nvme_devices:
         logger.error("Storage node has no nvme devices")
         return False
 
     if snode.status != snode.STATUS_ONLINE:
         logger.error("Storage node in not Online")
         return False
 
+
     lvol = LVol()
     lvol.lvol_name = clone_name
     lvol.size = snap.lvol.size
-    lvol.distr_bs = snap.lvol.distr_bs
     lvol.vuid = snap.lvol.vuid
+    lvol.distr_bs = snap.lvol.distr_bs
     lvol.ndcs = snap.lvol.ndcs
     lvol.npcs = snap.lvol.npcs
     lvol.distr_chunk_bs = snap.lvol.distr_chunk_bs
     lvol.distr_page_size = snap.lvol.distr_page_size
     lvol.distr_page_size = snap.lvol.distr_page_size
+    if new_size:
+        if snap.lvol.size >= new_size:
+            logger.error(f"New size {new_size} must be higher than the original size {snap.lvol.size}")
+            return False
+
+        if snap.lvol.max_size < new_size:
+            logger.error(f"New size {new_size} must be smaller than the max size {snap.lvol.max_size}")
+            return False
+        lvol.size = new_size
 
-    bdev_stack = []
 
-    ##############################################################################
+    bdev_stack = []
     jm_names = lvol_controller.get_jm_names(snode)
     rpc_client = RPCClient(snode.mgmt_ip, snode.rpc_port, snode.rpc_username, snode.rpc_password)
     spdk_mem_info_before = rpc_client.ultra21_util_get_malloc_stats()
 
     num_blocks = int(lvol.size / lvol.distr_bs)
     new_vuid = utils.get_random_vuid()
     name = f"distr_{new_vuid}_1"
@@ -235,15 +237,15 @@
     ret = distr_controller.send_cluster_map_to_node(snode)
     if not ret:
         return False, "Failed to send cluster map"
 
     logger.info("Creating clone bdev")
     block_len = lvol.distr_bs
     page_len = int(lvol.distr_page_size / lvol.distr_bs)
-    max_num_blocks = num_blocks * 10
+    max_num_blocks = snap.lvol.max_size
     ret = rpc_client.ultra21_lvol_bmap_init(name, num_blocks, block_len, page_len, max_num_blocks)
     if not ret:
         return False, "Failed to init distr bdev"
 
     lvol_name = f"clone_{lvol.vuid+2}_{lvol.lvol_name}"
     ret = rpc_client.ultra21_lvol_mount_clone(lvol_name, snap.snap_bdev, name, num_blocks)
     if not ret:
@@ -271,40 +273,42 @@
             ret = rpc_client.transport_create(tr_type)
             logger.info("adding listener for %s on IP %s" % (subsystem_nqn, iface.ip4_address))
             ret = rpc_client.listeners_create(subsystem_nqn, tr_type, iface.ip4_address, "4420")
 
     logger.info(f"add lvol {clone_name} to subsystem")
     ret = rpc_client.nvmf_subsystem_add_ns(subsystem_nqn, top_bdev)
 
+    lvol.vuid = new_vuid
     lvol.bdev_stack = bdev_stack
     lvol.uuid = lvol_id
     lvol.lvol_bdev = lvol_name
     lvol.top_bdev = top_bdev
+    lvol.base_bdev = name
     lvol.hostname = snode.hostname
     lvol.node_id = snode.get_id()
     lvol.mode = 'read-write'
     lvol.lvol_type = lvol_type
     lvol.cloned_from_snap = snapshot_id
     lvol.nqn = subsystem_nqn
     lvol.pool_uuid = pool.id
+    lvol.ha_type = snap.lvol.ha_type
+    lvol.status = LVol.STATUS_ONLINE
 
     spdk_mem_info_after = rpc_client.ultra21_util_get_malloc_stats()
     logger.debug("ultra21_util_get_malloc_stats:")
     logger.debug(spdk_mem_info_after)
 
     diff = {}
     for key in spdk_mem_info_after.keys():
         diff[key] = spdk_mem_info_after[key] - spdk_mem_info_before[key]
 
     logger.info("spdk mem diff:")
     logger.info(json.dumps(diff, indent=2))
     lvol.mem_diff = diff
 
-
-
     pool.lvols.append(lvol_id)
     pool.write_to_db(db_controller.kv_store)
     lvol.write_to_db(db_controller.kv_store)
     snode.lvols.append(lvol_id)
     snode.write_to_db(db_controller.kv_store)
     logger.info("Done")
     snapshot_events.snapshot_clone(snap, lvol)
```

## Comparing `sbcli_mc-1.0.1/simplyblock_core/controllers/snapshot_events.py` & `sbcli_mc-1.0.2/simplyblock_core/controllers/snapshot_events.py`

 * *Files identical despite different names*

## Comparing `sbcli_mc-1.0.1/simplyblock_core/controllers/events_controller.py` & `sbcli_mc-1.0.2/simplyblock_core/controllers/events_controller.py`

 * *Files identical despite different names*

## Comparing `sbcli_mc-1.0.1/simplyblock_core/controllers/health_controller.py` & `sbcli_mc-1.0.2/simplyblock_core/controllers/health_controller.py`

 * *Files 1% similar despite different names*

```diff
@@ -35,24 +35,24 @@
             result &= ret
             print("*" * 100)
             data.append({
                 "Kind": "Device",
                 "UUID": device.get_id(),
                 "Status": "ok" if ret else "failed"
             })
-    # todo: change this function for multi cluster
-    for lvol in db_controller.get_lvols():
-        ret = check_lvol(lvol.get_id())
-        result &= ret
-        print("*" * 100)
-        data.append({
-            "Kind": "LVol",
-            "UUID": lvol.get_id(),
-            "Status": "ok" if ret else "failed"
-        })
+
+        for lvol_id in node.lvols:
+            ret = check_lvol(lvol_id)
+            result &= ret
+            print("*" * 100)
+            data.append({
+                "Kind": "LVol",
+                "UUID": lvol_id,
+                "Status": "ok" if ret else "failed"
+            })
     print(utils.print_table(data))
     return result
 
 
 def _check_node_docker_api(ip):
     try:
         node_docker = docker.DockerClient(base_url=f"tcp://{ip}:2375", version="auto")
```

## Comparing `sbcli_mc-1.0.1/simplyblock_core/controllers/device_controller.py` & `sbcli_mc-1.0.2/simplyblock_core/controllers/device_controller.py`

 * *Files identical despite different names*

## Comparing `sbcli_mc-1.0.1/simplyblock_core/controllers/pool_events.py` & `sbcli_mc-1.0.2/simplyblock_core/controllers/pool_events.py`

 * *Files identical despite different names*

## Comparing `sbcli_mc-1.0.1/simplyblock_core/controllers/caching_node_controller.py` & `sbcli_mc-1.0.2/simplyblock_core/controllers/caching_node_controller.py`

 * *Files identical despite different names*

## Comparing `sbcli_mc-1.0.1/simplyblock_core/controllers/cluster_events.py` & `sbcli_mc-1.0.2/simplyblock_core/controllers/cluster_events.py`

 * *Files identical despite different names*

## Comparing `sbcli_mc-1.0.1/simplyblock_core/controllers/mgmt_events.py` & `sbcli_mc-1.0.2/simplyblock_core/controllers/mgmt_events.py`

 * *Files identical despite different names*

## Comparing `sbcli_mc-1.0.1/simplyblock_core/models/caching_node.py` & `sbcli_mc-1.0.2/simplyblock_core/models/caching_node.py`

 * *Files identical despite different names*

## Comparing `sbcli_mc-1.0.1/simplyblock_core/models/nvme_device.py` & `sbcli_mc-1.0.2/simplyblock_core/models/nvme_device.py`

 * *Files identical despite different names*

## Comparing `sbcli_mc-1.0.1/simplyblock_core/models/mgmt_node.py` & `sbcli_mc-1.0.2/simplyblock_core/models/mgmt_node.py`

 * *Files 8% similar despite different names*

```diff
@@ -25,15 +25,15 @@
         STATUS_RESTARTING: 12,
 
         STATUS_UNREACHABLE: 20,
 
     }
     attributes = {
         "baseboard_sn": {"type": str, 'default': ""},
-        "system_uuid": {"type": str, 'default': ""},
+        "uuid": {"type": str, 'default': ""},
         "hostname": {"type": str, 'default': ""},
         "status": {"type": str, 'default': ""},
         "docker_ip_port": {"type": str, 'default': ""},
         "cluster_id": {"type": str, 'default': ""},
         "mgmt_ip": {"type": str, 'default': ""},
         "updated_at": {"type": str, 'default': str(datetime.now())},
 
@@ -41,14 +41,14 @@
 
     def __init__(self, data=None):
         super(MgmtNode, self).__init__()
         self.set_attrs(self.attributes, data)
         self.object_type = "object"
 
     def get_id(self):
-        return self.system_uuid
+        return self.uuid
 
     def get_status_code(self):
         if self.status in self.STATUS_CODE_MAP:
             return self.STATUS_CODE_MAP[self.status]
         else:
             return -1
```

## Comparing `sbcli_mc-1.0.1/simplyblock_core/models/compute_node.py` & `sbcli_mc-1.0.2/simplyblock_core/models/compute_node.py`

 * *Files identical despite different names*

## Comparing `sbcli_mc-1.0.1/simplyblock_core/models/events.py` & `sbcli_mc-1.0.2/simplyblock_core/models/events.py`

 * *Files identical despite different names*

## Comparing `sbcli_mc-1.0.1/simplyblock_core/models/global_settings.py` & `sbcli_mc-1.0.2/simplyblock_core/models/global_settings.py`

 * *Files identical despite different names*

## Comparing `sbcli_mc-1.0.1/simplyblock_core/models/job_schedule.py` & `sbcli_mc-1.0.2/simplyblock_core/models/job_schedule.py`

 * *Files identical despite different names*

## Comparing `sbcli_mc-1.0.1/simplyblock_core/models/base_model.py` & `sbcli_mc-1.0.2/simplyblock_core/models/base_model.py`

 * *Files identical despite different names*

## Comparing `sbcli_mc-1.0.1/simplyblock_core/models/lvol_model.py` & `sbcli_mc-1.0.2/simplyblock_core/models/lvol_model.py`

 * *Files identical despite different names*

## Comparing `sbcli_mc-1.0.1/simplyblock_core/models/snapshot.py` & `sbcli_mc-1.0.2/simplyblock_core/models/snapshot.py`

 * *Files identical despite different names*

## Comparing `sbcli_mc-1.0.1/simplyblock_core/models/storage_node.py` & `sbcli_mc-1.0.2/simplyblock_core/models/storage_node.py`

 * *Files identical despite different names*

## Comparing `sbcli_mc-1.0.1/simplyblock_core/models/stats.py` & `sbcli_mc-1.0.2/simplyblock_core/models/stats.py`

 * *Files identical despite different names*

## Comparing `sbcli_mc-1.0.1/simplyblock_core/models/pool.py` & `sbcli_mc-1.0.2/simplyblock_core/models/pool.py`

 * *Files identical despite different names*

## Comparing `sbcli_mc-1.0.1/simplyblock_core/models/iface.py` & `sbcli_mc-1.0.2/simplyblock_core/models/iface.py`

 * *Files identical despite different names*

## Comparing `sbcli_mc-1.0.1/simplyblock_core/models/cluster.py` & `sbcli_mc-1.0.2/simplyblock_core/models/cluster.py`

 * *Files identical despite different names*

## Comparing `sbcli_mc-1.0.1/simplyblock_core/models/port_stat.py` & `sbcli_mc-1.0.2/simplyblock_core/models/port_stat.py`

 * *Files identical despite different names*

## Comparing `sbcli_mc-1.0.1/simplyblock_core/scripts/install_deps.sh` & `sbcli_mc-1.0.2/simplyblock_core/scripts/install_deps.sh`

 * *Files identical despite different names*

## Comparing `sbcli_mc-1.0.1/simplyblock_core/scripts/__init__.py` & `sbcli_mc-1.0.2/simplyblock_core/scripts/__init__.py`

 * *Files identical despite different names*

## Comparing `sbcli_mc-1.0.1/simplyblock_core/scripts/haproxy.cfg` & `sbcli_mc-1.0.2/simplyblock_core/scripts/haproxy.cfg`

 * *Files identical despite different names*

## Comparing `sbcli_mc-1.0.1/simplyblock_core/scripts/stack_deploy_wait.sh` & `sbcli_mc-1.0.2/simplyblock_core/scripts/stack_deploy_wait.sh`

 * *Files identical despite different names*

## Comparing `sbcli_mc-1.0.1/simplyblock_core/scripts/docker-compose-swarm.yml` & `sbcli_mc-1.0.2/simplyblock_core/scripts/docker-compose-swarm.yml`

 * *Files identical despite different names*

## Comparing `sbcli_mc-1.0.1/simplyblock_core/scripts/apply_dashboard.sh` & `sbcli_mc-1.0.2/simplyblock_core/scripts/apply_dashboard.sh`

 * *Files identical despite different names*

## Comparing `sbcli_mc-1.0.1/simplyblock_core/scripts/docker-compose-swarm-monitoring.yml` & `sbcli_mc-1.0.2/simplyblock_core/scripts/docker-compose-swarm-monitoring.yml`

 * *Files identical despite different names*

## Comparing `sbcli_mc-1.0.1/simplyblock_core/scripts/deploy_stack.sh` & `sbcli_mc-1.0.2/simplyblock_core/scripts/deploy_stack.sh`

 * *Files identical despite different names*

## Comparing `sbcli_mc-1.0.1/simplyblock_core/scripts/alerting/alert_rules.yaml` & `sbcli_mc-1.0.2/simplyblock_core/scripts/alerting/alert_rules.yaml`

 * *Files identical despite different names*

## Comparing `sbcli_mc-1.0.1/simplyblock_core/scripts/alerting/alert_resources.yaml` & `sbcli_mc-1.0.2/simplyblock_core/scripts/alerting/alert_resources.yaml`

 * *Files identical despite different names*

## Comparing `sbcli_mc-1.0.1/simplyblock_core/scripts/dashboards/nodes.json` & `sbcli_mc-1.0.2/simplyblock_core/scripts/dashboards/nodes.json`

 * *Files identical despite different names*

## Comparing `sbcli_mc-1.0.1/simplyblock_core/scripts/dashboards/cluster.json` & `sbcli_mc-1.0.2/simplyblock_core/scripts/dashboards/cluster.json`

 * *Files identical despite different names*

## Comparing `sbcli_mc-1.0.1/simplyblock_core/scripts/dashboards/lvols.json` & `sbcli_mc-1.0.2/simplyblock_core/scripts/dashboards/lvols.json`

 * *Files identical despite different names*

## Comparing `sbcli_mc-1.0.1/simplyblock_core/scripts/dashboards/devices.json` & `sbcli_mc-1.0.2/simplyblock_core/scripts/dashboards/devices.json`

 * *Files identical despite different names*

## Comparing `sbcli_mc-1.0.1/simplyblock_core/scripts/dashboards/pools.json` & `sbcli_mc-1.0.2/simplyblock_core/scripts/dashboards/pools.json`

 * *Files identical despite different names*

## Comparing `sbcli_mc-1.0.1/simplyblock_core/scripts/dashboards/node-exporter.json` & `sbcli_mc-1.0.2/simplyblock_core/scripts/dashboards/node-exporter.json`

 * *Files identical despite different names*

## Comparing `sbcli_mc-1.0.1/sbcli_mc.egg-info/SOURCES.txt` & `sbcli_mc-1.0.2/sbcli_mc.egg-info/SOURCES.txt`

 * *Files identical despite different names*

## Comparing `sbcli_mc-1.0.1/sbcli_mc.egg-info/PKG-INFO` & `sbcli_mc-1.0.2/sbcli_mc.egg-info/PKG-INFO`

 * *Files 4% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: sbcli-mc
-Version: 1.0.1
+Version: 1.0.2
 Summary: CLI for managing SimplyBlock cluster
 Home-page: https://www.simplyblock.io/
 Author: Hamdy
 Author-email: hamdy@simplyblock.io
 Description-Content-Type: text/markdown
 Requires-Dist: foundationdb
 Requires-Dist: requests
```

