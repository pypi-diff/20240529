# Comparing `tmp/sbcli_mc-1.0.2.zip` & `tmp/sbcli_mc-1.0.4.zip`

## zipinfo {}

```diff
@@ -1,150 +1,150 @@
-Zip file size: 212499 bytes, number of entries: 148
-drwxr-xr-x  2.0 unx        0 b- stor 24-May-29 02:25 sbcli_mc-1.0.2/
-drwxr-xr-x  2.0 unx        0 b- stor 24-May-29 02:25 sbcli_mc-1.0.2/simplyblock_cli/
-drwxr-xr-x  2.0 unx        0 b- stor 24-May-29 02:25 sbcli_mc-1.0.2/simplyblock_web/
-drwxr-xr-x  2.0 unx        0 b- stor 24-May-29 02:25 sbcli_mc-1.0.2/simplyblock_core/
-drwxr-xr-x  2.0 unx        0 b- stor 24-May-29 02:25 sbcli_mc-1.0.2/sbcli_mc.egg-info/
--rw-r--r--  2.0 unx     1068 b- defN 24-May-29 02:25 sbcli_mc-1.0.2/README.md
--rw-r--r--  2.0 unx       84 b- defN 24-May-29 02:25 sbcli_mc-1.0.2/pyproject.toml
--rw-r--r--  2.0 unx     1488 b- defN 24-May-29 02:25 sbcli_mc-1.0.2/PKG-INFO
--rw-r--r--  2.0 unx      157 b- defN 24-May-29 02:25 sbcli_mc-1.0.2/env_var
--rw-r--r--  2.0 unx       38 b- defN 24-May-29 02:25 sbcli_mc-1.0.2/setup.cfg
--rw-r--r--  2.0 unx     2269 b- defN 24-May-29 02:25 sbcli_mc-1.0.2/setup.py
--rw-r--r--  2.0 unx    64564 b- defN 24-May-29 02:25 sbcli_mc-1.0.2/simplyblock_cli/cli.py
--rw-r--r--  2.0 unx      357 b- defN 24-May-29 02:25 sbcli_mc-1.0.2/simplyblock_cli/main.py
-drwxr-xr-x  2.0 unx        0 b- stor 24-May-29 02:25 sbcli_mc-1.0.2/simplyblock_web/static/
-drwxr-xr-x  2.0 unx        0 b- stor 24-May-29 02:25 sbcli_mc-1.0.2/simplyblock_web/blueprints/
-drwxr-xr-x  2.0 unx        0 b- stor 24-May-29 02:25 sbcli_mc-1.0.2/simplyblock_web/templates/
--rw-r--r--  2.0 unx        0 b- defN 24-May-29 02:25 sbcli_mc-1.0.2/simplyblock_web/__init__.py
--rw-r--r--  2.0 unx     1434 b- defN 24-May-29 02:25 sbcli_mc-1.0.2/simplyblock_web/node_webapp.py
--rw-r--r--  2.0 unx      703 b- defN 24-May-29 02:25 sbcli_mc-1.0.2/simplyblock_web/snode_app.py
--rw-r--r--  2.0 unx      717 b- defN 24-May-29 02:25 sbcli_mc-1.0.2/simplyblock_web/caching_node_app.py
--rw-r--r--  2.0 unx     1638 b- defN 24-May-29 02:25 sbcli_mc-1.0.2/simplyblock_web/auth_middleware.py
--rw-r--r--  2.0 unx     5098 b- defN 24-May-29 02:25 sbcli_mc-1.0.2/simplyblock_web/node_utils.py
--rw-r--r--  2.0 unx     2715 b- defN 24-May-29 02:25 sbcli_mc-1.0.2/simplyblock_web/utils.py
--rw-r--r--  2.0 unx     1284 b- defN 24-May-29 02:25 sbcli_mc-1.0.2/simplyblock_web/app.py
--rw-r--r--  2.0 unx      725 b- defN 24-May-29 02:25 sbcli_mc-1.0.2/simplyblock_web/caching_node_app_k8s.py
--rw-r--r--  2.0 unx      322 b- defN 24-May-29 02:25 sbcli_mc-1.0.2/simplyblock_web/static/tst.py
--rw-r--r--  2.0 unx      827 b- defN 24-May-29 02:25 sbcli_mc-1.0.2/simplyblock_web/static/delete.py
--rw-r--r--  2.0 unx      507 b- defN 24-May-29 02:25 sbcli_mc-1.0.2/simplyblock_web/static/deploy_cnode.yaml
--rw-r--r--  2.0 unx      434 b- defN 24-May-29 02:25 sbcli_mc-1.0.2/simplyblock_web/static/is_up.py
--rw-r--r--  2.0 unx     1466 b- defN 24-May-29 02:25 sbcli_mc-1.0.2/simplyblock_web/static/deploy_spdk.yaml
--rw-r--r--  2.0 unx      463 b- defN 24-May-29 02:25 sbcli_mc-1.0.2/simplyblock_web/static/rpac.yaml
--rw-r--r--  2.0 unx      417 b- defN 24-May-29 02:25 sbcli_mc-1.0.2/simplyblock_web/static/list_deps.py
--rw-r--r--  2.0 unx     1302 b- defN 24-May-29 02:25 sbcli_mc-1.0.2/simplyblock_web/static/deploy.py
--rw-r--r--  2.0 unx     6806 b- defN 24-May-29 02:25 sbcli_mc-1.0.2/simplyblock_web/blueprints/web_api_pool.py
--rw-r--r--  2.0 unx        0 b- defN 24-May-29 02:25 sbcli_mc-1.0.2/simplyblock_web/blueprints/__init__.py
--rw-r--r--  2.0 unx     3118 b- defN 24-May-29 02:25 sbcli_mc-1.0.2/simplyblock_web/blueprints/web_api_device.py
--rw-r--r--  2.0 unx     8685 b- defN 24-May-29 02:25 sbcli_mc-1.0.2/simplyblock_web/blueprints/web_api_lvol.py
--rw-r--r--  2.0 unx     9713 b- defN 24-May-29 02:25 sbcli_mc-1.0.2/simplyblock_web/blueprints/snode_ops.py
--rw-r--r--  2.0 unx    12385 b- defN 24-May-29 02:25 sbcli_mc-1.0.2/simplyblock_web/blueprints/caching_node_ops.py
--rw-r--r--  2.0 unx     6401 b- defN 24-May-29 02:25 sbcli_mc-1.0.2/simplyblock_web/blueprints/web_api_storage_node.py
--rw-r--r--  2.0 unx     5931 b- defN 24-May-29 02:25 sbcli_mc-1.0.2/simplyblock_web/blueprints/web_api_cluster.py
--rw-r--r--  2.0 unx     8075 b- defN 24-May-29 02:25 sbcli_mc-1.0.2/simplyblock_web/blueprints/caching_node_ops_k8s.py
--rw-r--r--  2.0 unx     4883 b- defN 24-May-29 02:25 sbcli_mc-1.0.2/simplyblock_web/blueprints/node_api_caching_ks.py
--rw-r--r--  2.0 unx     5746 b- defN 24-May-29 02:25 sbcli_mc-1.0.2/simplyblock_web/blueprints/node_api_caching_docker.py
--rw-r--r--  2.0 unx     5491 b- defN 24-May-29 02:25 sbcli_mc-1.0.2/simplyblock_web/blueprints/web_api_caching_node.py
--rw-r--r--  2.0 unx     3103 b- defN 24-May-29 02:25 sbcli_mc-1.0.2/simplyblock_web/blueprints/node_api_basic.py
--rw-r--r--  2.0 unx    11244 b- defN 24-May-29 02:25 sbcli_mc-1.0.2/simplyblock_web/blueprints/csi.py
--rw-r--r--  2.0 unx      975 b- defN 24-May-29 02:25 sbcli_mc-1.0.2/simplyblock_web/blueprints/web_api_mgmt_node.py
--rw-r--r--  2.0 unx     2905 b- defN 24-May-29 02:25 sbcli_mc-1.0.2/simplyblock_web/templates/deploy_spdk.yaml.j2
-drwxr-xr-x  2.0 unx        0 b- stor 24-May-29 02:25 sbcli_mc-1.0.2/simplyblock_core/services/
-drwxr-xr-x  2.0 unx        0 b- stor 24-May-29 02:25 sbcli_mc-1.0.2/simplyblock_core/controllers/
-drwxr-xr-x  2.0 unx        0 b- stor 24-May-29 02:25 sbcli_mc-1.0.2/simplyblock_core/models/
-drwxr-xr-x  2.0 unx        0 b- stor 24-May-29 02:25 sbcli_mc-1.0.2/simplyblock_core/scripts/
--rw-r--r--  2.0 unx    25885 b- defN 24-May-29 02:25 sbcli_mc-1.0.2/simplyblock_core/cluster_ops.py
--rw-r--r--  2.0 unx      938 b- defN 24-May-29 02:25 sbcli_mc-1.0.2/simplyblock_core/pci_utils.py
--rw-r--r--  2.0 unx        0 b- defN 24-May-29 02:25 sbcli_mc-1.0.2/simplyblock_core/__init__.py
--rw-r--r--  2.0 unx     3193 b- defN 24-May-29 02:25 sbcli_mc-1.0.2/simplyblock_core/snode_client.py
--rw-r--r--  2.0 unx     8799 b- defN 24-May-29 02:25 sbcli_mc-1.0.2/simplyblock_core/kv_store.py
--rw-r--r--  2.0 unx     5112 b- defN 24-May-29 02:25 sbcli_mc-1.0.2/simplyblock_core/compute_node_ops.py
--rw-r--r--  2.0 unx    20829 b- defN 24-May-29 02:25 sbcli_mc-1.0.2/simplyblock_core/rpc_client.py
--rw-r--r--  2.0 unx     1986 b- defN 24-May-29 02:25 sbcli_mc-1.0.2/simplyblock_core/mgmt_node_ops.py
--rw-r--r--  2.0 unx     7640 b- defN 24-May-29 02:25 sbcli_mc-1.0.2/simplyblock_core/utils.py
--rw-r--r--  2.0 unx     7725 b- defN 24-May-29 02:25 sbcli_mc-1.0.2/simplyblock_core/distr_controller.py
--rw-r--r--  2.0 unx      279 b- defN 24-May-29 02:25 sbcli_mc-1.0.2/simplyblock_core/shell_utils.py
--rw-r--r--  2.0 unx     3638 b- defN 24-May-29 02:25 sbcli_mc-1.0.2/simplyblock_core/cnode_client.py
--rw-r--r--  2.0 unx    65242 b- defN 24-May-29 02:25 sbcli_mc-1.0.2/simplyblock_core/storage_node_ops.py
--rw-r--r--  2.0 unx     1575 b- defN 24-May-29 02:25 sbcli_mc-1.0.2/simplyblock_core/constants.py
--rw-r--r--  2.0 unx     3542 b- defN 24-May-29 02:25 sbcli_mc-1.0.2/simplyblock_core/services/job_tasks.py
--rw-r--r--  2.0 unx     3203 b- defN 24-May-29 02:25 sbcli_mc-1.0.2/simplyblock_core/services/caching_node_monitor.py
--rw-r--r--  2.0 unx      229 b- defN 24-May-29 02:25 sbcli_mc-1.0.2/simplyblock_core/services/service_template.service
--rw-r--r--  2.0 unx      837 b- defN 24-May-29 02:25 sbcli_mc-1.0.2/simplyblock_core/services/install_service.sh
--rw-r--r--  2.0 unx     4118 b- defN 24-May-29 02:25 sbcli_mc-1.0.2/simplyblock_core/services/__init__.py
--rw-r--r--  2.0 unx     2410 b- defN 24-May-29 02:25 sbcli_mc-1.0.2/simplyblock_core/services/log_agg_service.py
--rw-r--r--  2.0 unx     5751 b- defN 24-May-29 02:25 sbcli_mc-1.0.2/simplyblock_core/services/health_check_service.py
--rw-r--r--  2.0 unx     7439 b- defN 24-May-29 02:25 sbcli_mc-1.0.2/simplyblock_core/services/capacity_and_stats_collector.py
--rw-r--r--  2.0 unx     3169 b- defN 24-May-29 02:25 sbcli_mc-1.0.2/simplyblock_core/services/device_monitor.py
--rw-r--r--  2.0 unx     5268 b- defN 24-May-29 02:25 sbcli_mc-1.0.2/simplyblock_core/services/lvol_stat_collector.py
--rw-r--r--  2.0 unx     2671 b- defN 24-May-29 02:25 sbcli_mc-1.0.2/simplyblock_core/services/cap_monitor.py
--rw-r--r--  2.0 unx     6822 b- defN 24-May-29 02:25 sbcli_mc-1.0.2/simplyblock_core/services/storage_node_monitor.py
--rw-r--r--  2.0 unx     2428 b- defN 24-May-29 02:25 sbcli_mc-1.0.2/simplyblock_core/services/port_stat_collector.py
--rw-r--r--  2.0 unx     5146 b- defN 24-May-29 02:25 sbcli_mc-1.0.2/simplyblock_core/services/distr_event_collector.py
--rw-r--r--  2.0 unx      173 b- defN 24-May-29 02:25 sbcli_mc-1.0.2/simplyblock_core/services/remove_service.sh
--rw-r--r--  2.0 unx     3003 b- defN 24-May-29 02:25 sbcli_mc-1.0.2/simplyblock_core/services/mgmt_node_monitor.py
--rw-r--r--  2.0 unx     2189 b- defN 24-May-29 02:25 sbcli_mc-1.0.2/simplyblock_core/services/lvol_monitor.py
--rw-r--r--  2.0 unx    10594 b- defN 24-May-29 02:25 sbcli_mc-1.0.2/simplyblock_core/controllers/pool_controller.py
--rw-r--r--  2.0 unx        0 b- defN 24-May-29 02:25 sbcli_mc-1.0.2/simplyblock_core/controllers/__init__.py
--rw-r--r--  2.0 unx     1521 b- defN 24-May-29 02:25 sbcli_mc-1.0.2/simplyblock_core/controllers/storage_events.py
--rw-r--r--  2.0 unx    48560 b- defN 24-May-29 02:25 sbcli_mc-1.0.2/simplyblock_core/controllers/lvol_controller.py
--rw-r--r--  2.0 unx     1568 b- defN 24-May-29 02:25 sbcli_mc-1.0.2/simplyblock_core/controllers/device_events.py
--rw-r--r--  2.0 unx     1630 b- defN 24-May-29 02:25 sbcli_mc-1.0.2/simplyblock_core/controllers/lvol_events.py
--rw-r--r--  2.0 unx    10874 b- defN 24-May-29 02:25 sbcli_mc-1.0.2/simplyblock_core/controllers/snapshot_controller.py
--rw-r--r--  2.0 unx     1122 b- defN 24-May-29 02:25 sbcli_mc-1.0.2/simplyblock_core/controllers/snapshot_events.py
--rw-r--r--  2.0 unx     3191 b- defN 24-May-29 02:25 sbcli_mc-1.0.2/simplyblock_core/controllers/events_controller.py
--rw-r--r--  2.0 unx    10852 b- defN 24-May-29 02:25 sbcli_mc-1.0.2/simplyblock_core/controllers/health_controller.py
--rw-r--r--  2.0 unx    13932 b- defN 24-May-29 02:25 sbcli_mc-1.0.2/simplyblock_core/controllers/device_controller.py
--rw-r--r--  2.0 unx      695 b- defN 24-May-29 02:25 sbcli_mc-1.0.2/simplyblock_core/controllers/pool_events.py
--rw-r--r--  2.0 unx    23440 b- defN 24-May-29 02:25 sbcli_mc-1.0.2/simplyblock_core/controllers/caching_node_controller.py
--rw-r--r--  2.0 unx     1900 b- defN 24-May-29 02:25 sbcli_mc-1.0.2/simplyblock_core/controllers/cluster_events.py
--rw-r--r--  2.0 unx     1120 b- defN 24-May-29 02:25 sbcli_mc-1.0.2/simplyblock_core/controllers/mgmt_events.py
--rw-r--r--  2.0 unx     3766 b- defN 24-May-29 02:25 sbcli_mc-1.0.2/simplyblock_core/models/caching_node.py
--rw-r--r--  2.0 unx     2094 b- defN 24-May-29 02:25 sbcli_mc-1.0.2/simplyblock_core/models/nvme_device.py
--rw-r--r--  2.0 unx     1452 b- defN 24-May-29 02:25 sbcli_mc-1.0.2/simplyblock_core/models/mgmt_node.py
--rw-r--r--  2.0 unx      917 b- defN 24-May-29 02:25 sbcli_mc-1.0.2/simplyblock_core/models/compute_node.py
--rw-r--r--  2.0 unx        0 b- defN 24-May-29 02:25 sbcli_mc-1.0.2/simplyblock_core/models/__init__.py
--rw-r--r--  2.0 unx     1500 b- defN 24-May-29 02:25 sbcli_mc-1.0.2/simplyblock_core/models/events.py
--rw-r--r--  2.0 unx     1228 b- defN 24-May-29 02:25 sbcli_mc-1.0.2/simplyblock_core/models/global_settings.py
--rw-r--r--  2.0 unx      973 b- defN 24-May-29 02:25 sbcli_mc-1.0.2/simplyblock_core/models/job_schedule.py
--rw-r--r--  2.0 unx     4846 b- defN 24-May-29 02:25 sbcli_mc-1.0.2/simplyblock_core/models/base_model.py
--rw-r--r--  2.0 unx     2579 b- defN 24-May-29 02:25 sbcli_mc-1.0.2/simplyblock_core/models/lvol_model.py
--rw-r--r--  2.0 unx      736 b- defN 24-May-29 02:25 sbcli_mc-1.0.2/simplyblock_core/models/snapshot.py
--rw-r--r--  2.0 unx     3696 b- defN 24-May-29 02:25 sbcli_mc-1.0.2/simplyblock_core/models/storage_node.py
--rw-r--r--  2.0 unx     4242 b- defN 24-May-29 02:25 sbcli_mc-1.0.2/simplyblock_core/models/stats.py
--rw-r--r--  2.0 unx     1602 b- defN 24-May-29 02:25 sbcli_mc-1.0.2/simplyblock_core/models/pool.py
--rw-r--r--  2.0 unx      806 b- defN 24-May-29 02:25 sbcli_mc-1.0.2/simplyblock_core/models/iface.py
--rw-r--r--  2.0 unx     2565 b- defN 24-May-29 02:25 sbcli_mc-1.0.2/simplyblock_core/models/cluster.py
--rw-r--r--  2.0 unx     1020 b- defN 24-May-29 02:25 sbcli_mc-1.0.2/simplyblock_core/models/port_stat.py
-drwxr-xr-x  2.0 unx        0 b- stor 24-May-29 02:25 sbcli_mc-1.0.2/simplyblock_core/scripts/alerting/
-drwxr-xr-x  2.0 unx        0 b- stor 24-May-29 02:25 sbcli_mc-1.0.2/simplyblock_core/scripts/dashboards/
--rw-r--r--  2.0 unx     1420 b- defN 24-May-29 02:25 sbcli_mc-1.0.2/simplyblock_core/scripts/install_deps.sh
--rw-r--r--  2.0 unx     1782 b- defN 24-May-29 02:25 sbcli_mc-1.0.2/simplyblock_core/scripts/__init__.py
--rw-r--r--  2.0 unx       43 b- defN 24-May-29 02:25 sbcli_mc-1.0.2/simplyblock_core/scripts/run_ssh.sh
--rw-r--r--  2.0 unx     1163 b- defN 24-May-29 02:25 sbcli_mc-1.0.2/simplyblock_core/scripts/haproxy.cfg
--rw-r--r--  2.0 unx      118 b- defN 24-May-29 02:25 sbcli_mc-1.0.2/simplyblock_core/scripts/db_config_double.sh
--rw-r--r--  2.0 unx     5305 b- defN 24-May-29 02:25 sbcli_mc-1.0.2/simplyblock_core/scripts/stack_deploy_wait.sh
--rw-r--r--  2.0 unx      360 b- defN 24-May-29 02:25 sbcli_mc-1.0.2/simplyblock_core/scripts/datasource.yml
--rw-r--r--  2.0 unx     5611 b- defN 24-May-29 02:25 sbcli_mc-1.0.2/simplyblock_core/scripts/docker-compose-swarm.yml
--rw-r--r--  2.0 unx      152 b- defN 24-May-29 02:25 sbcli_mc-1.0.2/simplyblock_core/scripts/set_db_config.sh
--rwxr-xr-x  2.0 unx      657 b- defN 24-May-29 02:25 sbcli_mc-1.0.2/simplyblock_core/scripts/apply_dashboard.sh
--rw-r--r--  2.0 unx      311 b- defN 24-May-29 02:25 sbcli_mc-1.0.2/simplyblock_core/scripts/prometheus.yml
--rw-r--r--  2.0 unx      311 b- defN 24-May-29 02:25 sbcli_mc-1.0.2/simplyblock_core/scripts/clean_local_storage_deploy.sh
--rw-r--r--  2.0 unx     4409 b- defN 24-May-29 02:25 sbcli_mc-1.0.2/simplyblock_core/scripts/docker-compose-swarm-monitoring.yml
--rw-r--r--  2.0 unx      930 b- defN 24-May-29 02:25 sbcli_mc-1.0.2/simplyblock_core/scripts/deploy_stack.sh
--rw-r--r--  2.0 unx       54 b- defN 24-May-29 02:25 sbcli_mc-1.0.2/simplyblock_core/scripts/db_config_single.sh
--rw-r--r--  2.0 unx      453 b- defN 24-May-29 02:25 sbcli_mc-1.0.2/simplyblock_core/scripts/config_docker.sh
--rw-r--r--  2.0 unx    25433 b- defN 24-May-29 02:25 sbcli_mc-1.0.2/simplyblock_core/scripts/alerting/alert_rules.yaml
--rw-r--r--  2.0 unx     1856 b- defN 24-May-29 02:25 sbcli_mc-1.0.2/simplyblock_core/scripts/alerting/alert_resources.yaml
--rw-r--r--  2.0 unx    88820 b- defN 24-May-29 02:25 sbcli_mc-1.0.2/simplyblock_core/scripts/dashboards/nodes.json
--rw-r--r--  2.0 unx    88911 b- defN 24-May-29 02:25 sbcli_mc-1.0.2/simplyblock_core/scripts/dashboards/cluster.json
--rw-r--r--  2.0 unx    88776 b- defN 24-May-29 02:25 sbcli_mc-1.0.2/simplyblock_core/scripts/dashboards/lvols.json
--rw-r--r--  2.0 unx    88868 b- defN 24-May-29 02:25 sbcli_mc-1.0.2/simplyblock_core/scripts/dashboards/devices.json
--rw-r--r--  2.0 unx    99707 b- defN 24-May-29 02:25 sbcli_mc-1.0.2/simplyblock_core/scripts/dashboards/pools.json
--rw-r--r--  2.0 unx   799409 b- defN 24-May-29 02:25 sbcli_mc-1.0.2/simplyblock_core/scripts/dashboards/node-exporter.json
--rw-r--r--  2.0 unx     5261 b- defN 24-May-29 02:25 sbcli_mc-1.0.2/sbcli_mc.egg-info/SOURCES.txt
--rw-r--r--  2.0 unx       73 b- defN 24-May-29 02:25 sbcli_mc-1.0.2/sbcli_mc.egg-info/requires.txt
--rw-r--r--  2.0 unx     1488 b- defN 24-May-29 02:25 sbcli_mc-1.0.2/sbcli_mc.egg-info/PKG-INFO
--rw-r--r--  2.0 unx       49 b- defN 24-May-29 02:25 sbcli_mc-1.0.2/sbcli_mc.egg-info/top_level.txt
--rw-r--r--  2.0 unx       54 b- defN 24-May-29 02:25 sbcli_mc-1.0.2/sbcli_mc.egg-info/entry_points.txt
--rw-r--r--  2.0 unx        1 b- defN 24-May-29 02:25 sbcli_mc-1.0.2/sbcli_mc.egg-info/dependency_links.txt
-148 files, 1873583 bytes uncompressed, 185861 bytes compressed:  90.1%
+Zip file size: 212795 bytes, number of entries: 148
+drwxr-xr-x  2.0 unx        0 b- stor 24-May-29 03:38 sbcli_mc-1.0.4/
+drwxr-xr-x  2.0 unx        0 b- stor 24-May-29 03:38 sbcli_mc-1.0.4/simplyblock_cli/
+drwxr-xr-x  2.0 unx        0 b- stor 24-May-29 03:38 sbcli_mc-1.0.4/simplyblock_web/
+drwxr-xr-x  2.0 unx        0 b- stor 24-May-29 03:38 sbcli_mc-1.0.4/simplyblock_core/
+drwxr-xr-x  2.0 unx        0 b- stor 24-May-29 03:38 sbcli_mc-1.0.4/sbcli_mc.egg-info/
+-rw-r--r--  2.0 unx     1068 b- defN 24-May-29 03:38 sbcli_mc-1.0.4/README.md
+-rw-r--r--  2.0 unx       84 b- defN 24-May-29 03:38 sbcli_mc-1.0.4/pyproject.toml
+-rw-r--r--  2.0 unx     1488 b- defN 24-May-29 03:38 sbcli_mc-1.0.4/PKG-INFO
+-rw-r--r--  2.0 unx      157 b- defN 24-May-29 03:38 sbcli_mc-1.0.4/env_var
+-rw-r--r--  2.0 unx       38 b- defN 24-May-29 03:38 sbcli_mc-1.0.4/setup.cfg
+-rw-r--r--  2.0 unx     2269 b- defN 24-May-29 03:38 sbcli_mc-1.0.4/setup.py
+-rw-r--r--  2.0 unx    64705 b- defN 24-May-29 03:38 sbcli_mc-1.0.4/simplyblock_cli/cli.py
+-rw-r--r--  2.0 unx      357 b- defN 24-May-29 03:38 sbcli_mc-1.0.4/simplyblock_cli/main.py
+drwxr-xr-x  2.0 unx        0 b- stor 24-May-29 03:38 sbcli_mc-1.0.4/simplyblock_web/static/
+drwxr-xr-x  2.0 unx        0 b- stor 24-May-29 03:38 sbcli_mc-1.0.4/simplyblock_web/blueprints/
+drwxr-xr-x  2.0 unx        0 b- stor 24-May-29 03:38 sbcli_mc-1.0.4/simplyblock_web/templates/
+-rw-r--r--  2.0 unx        0 b- defN 24-May-29 03:38 sbcli_mc-1.0.4/simplyblock_web/__init__.py
+-rw-r--r--  2.0 unx     1434 b- defN 24-May-29 03:38 sbcli_mc-1.0.4/simplyblock_web/node_webapp.py
+-rw-r--r--  2.0 unx      703 b- defN 24-May-29 03:38 sbcli_mc-1.0.4/simplyblock_web/snode_app.py
+-rw-r--r--  2.0 unx      717 b- defN 24-May-29 03:38 sbcli_mc-1.0.4/simplyblock_web/caching_node_app.py
+-rw-r--r--  2.0 unx     1638 b- defN 24-May-29 03:38 sbcli_mc-1.0.4/simplyblock_web/auth_middleware.py
+-rw-r--r--  2.0 unx     5098 b- defN 24-May-29 03:38 sbcli_mc-1.0.4/simplyblock_web/node_utils.py
+-rw-r--r--  2.0 unx     2715 b- defN 24-May-29 03:38 sbcli_mc-1.0.4/simplyblock_web/utils.py
+-rw-r--r--  2.0 unx     1284 b- defN 24-May-29 03:38 sbcli_mc-1.0.4/simplyblock_web/app.py
+-rw-r--r--  2.0 unx      725 b- defN 24-May-29 03:38 sbcli_mc-1.0.4/simplyblock_web/caching_node_app_k8s.py
+-rw-r--r--  2.0 unx      322 b- defN 24-May-29 03:38 sbcli_mc-1.0.4/simplyblock_web/static/tst.py
+-rw-r--r--  2.0 unx      827 b- defN 24-May-29 03:38 sbcli_mc-1.0.4/simplyblock_web/static/delete.py
+-rw-r--r--  2.0 unx      507 b- defN 24-May-29 03:38 sbcli_mc-1.0.4/simplyblock_web/static/deploy_cnode.yaml
+-rw-r--r--  2.0 unx      434 b- defN 24-May-29 03:38 sbcli_mc-1.0.4/simplyblock_web/static/is_up.py
+-rw-r--r--  2.0 unx     1466 b- defN 24-May-29 03:38 sbcli_mc-1.0.4/simplyblock_web/static/deploy_spdk.yaml
+-rw-r--r--  2.0 unx      463 b- defN 24-May-29 03:38 sbcli_mc-1.0.4/simplyblock_web/static/rpac.yaml
+-rw-r--r--  2.0 unx      417 b- defN 24-May-29 03:38 sbcli_mc-1.0.4/simplyblock_web/static/list_deps.py
+-rw-r--r--  2.0 unx     1302 b- defN 24-May-29 03:38 sbcli_mc-1.0.4/simplyblock_web/static/deploy.py
+-rw-r--r--  2.0 unx     6806 b- defN 24-May-29 03:38 sbcli_mc-1.0.4/simplyblock_web/blueprints/web_api_pool.py
+-rw-r--r--  2.0 unx        0 b- defN 24-May-29 03:38 sbcli_mc-1.0.4/simplyblock_web/blueprints/__init__.py
+-rw-r--r--  2.0 unx     3118 b- defN 24-May-29 03:38 sbcli_mc-1.0.4/simplyblock_web/blueprints/web_api_device.py
+-rw-r--r--  2.0 unx     8930 b- defN 24-May-29 03:38 sbcli_mc-1.0.4/simplyblock_web/blueprints/web_api_lvol.py
+-rw-r--r--  2.0 unx     9713 b- defN 24-May-29 03:38 sbcli_mc-1.0.4/simplyblock_web/blueprints/snode_ops.py
+-rw-r--r--  2.0 unx    12385 b- defN 24-May-29 03:38 sbcli_mc-1.0.4/simplyblock_web/blueprints/caching_node_ops.py
+-rw-r--r--  2.0 unx     6401 b- defN 24-May-29 03:38 sbcli_mc-1.0.4/simplyblock_web/blueprints/web_api_storage_node.py
+-rw-r--r--  2.0 unx     5931 b- defN 24-May-29 03:38 sbcli_mc-1.0.4/simplyblock_web/blueprints/web_api_cluster.py
+-rw-r--r--  2.0 unx     8075 b- defN 24-May-29 03:38 sbcli_mc-1.0.4/simplyblock_web/blueprints/caching_node_ops_k8s.py
+-rw-r--r--  2.0 unx     4883 b- defN 24-May-29 03:38 sbcli_mc-1.0.4/simplyblock_web/blueprints/node_api_caching_ks.py
+-rw-r--r--  2.0 unx     5746 b- defN 24-May-29 03:38 sbcli_mc-1.0.4/simplyblock_web/blueprints/node_api_caching_docker.py
+-rw-r--r--  2.0 unx     5491 b- defN 24-May-29 03:38 sbcli_mc-1.0.4/simplyblock_web/blueprints/web_api_caching_node.py
+-rw-r--r--  2.0 unx     3103 b- defN 24-May-29 03:38 sbcli_mc-1.0.4/simplyblock_web/blueprints/node_api_basic.py
+-rw-r--r--  2.0 unx    11244 b- defN 24-May-29 03:38 sbcli_mc-1.0.4/simplyblock_web/blueprints/csi.py
+-rw-r--r--  2.0 unx      975 b- defN 24-May-29 03:38 sbcli_mc-1.0.4/simplyblock_web/blueprints/web_api_mgmt_node.py
+-rw-r--r--  2.0 unx     2905 b- defN 24-May-29 03:38 sbcli_mc-1.0.4/simplyblock_web/templates/deploy_spdk.yaml.j2
+drwxr-xr-x  2.0 unx        0 b- stor 24-May-29 03:38 sbcli_mc-1.0.4/simplyblock_core/services/
+drwxr-xr-x  2.0 unx        0 b- stor 24-May-29 03:38 sbcli_mc-1.0.4/simplyblock_core/controllers/
+drwxr-xr-x  2.0 unx        0 b- stor 24-May-29 03:38 sbcli_mc-1.0.4/simplyblock_core/models/
+drwxr-xr-x  2.0 unx        0 b- stor 24-May-29 03:38 sbcli_mc-1.0.4/simplyblock_core/scripts/
+-rw-r--r--  2.0 unx    26004 b- defN 24-May-29 03:38 sbcli_mc-1.0.4/simplyblock_core/cluster_ops.py
+-rw-r--r--  2.0 unx      938 b- defN 24-May-29 03:38 sbcli_mc-1.0.4/simplyblock_core/pci_utils.py
+-rw-r--r--  2.0 unx        0 b- defN 24-May-29 03:38 sbcli_mc-1.0.4/simplyblock_core/__init__.py
+-rw-r--r--  2.0 unx     3193 b- defN 24-May-29 03:38 sbcli_mc-1.0.4/simplyblock_core/snode_client.py
+-rw-r--r--  2.0 unx     9031 b- defN 24-May-29 03:38 sbcli_mc-1.0.4/simplyblock_core/kv_store.py
+-rw-r--r--  2.0 unx     5112 b- defN 24-May-29 03:38 sbcli_mc-1.0.4/simplyblock_core/compute_node_ops.py
+-rw-r--r--  2.0 unx    20829 b- defN 24-May-29 03:38 sbcli_mc-1.0.4/simplyblock_core/rpc_client.py
+-rw-r--r--  2.0 unx     1986 b- defN 24-May-29 03:38 sbcli_mc-1.0.4/simplyblock_core/mgmt_node_ops.py
+-rw-r--r--  2.0 unx     7640 b- defN 24-May-29 03:38 sbcli_mc-1.0.4/simplyblock_core/utils.py
+-rw-r--r--  2.0 unx     7725 b- defN 24-May-29 03:38 sbcli_mc-1.0.4/simplyblock_core/distr_controller.py
+-rw-r--r--  2.0 unx      279 b- defN 24-May-29 03:38 sbcli_mc-1.0.4/simplyblock_core/shell_utils.py
+-rw-r--r--  2.0 unx     3638 b- defN 24-May-29 03:38 sbcli_mc-1.0.4/simplyblock_core/cnode_client.py
+-rw-r--r--  2.0 unx    65258 b- defN 24-May-29 03:38 sbcli_mc-1.0.4/simplyblock_core/storage_node_ops.py
+-rw-r--r--  2.0 unx     1575 b- defN 24-May-29 03:38 sbcli_mc-1.0.4/simplyblock_core/constants.py
+-rw-r--r--  2.0 unx     3542 b- defN 24-May-29 03:38 sbcli_mc-1.0.4/simplyblock_core/services/job_tasks.py
+-rw-r--r--  2.0 unx     3203 b- defN 24-May-29 03:38 sbcli_mc-1.0.4/simplyblock_core/services/caching_node_monitor.py
+-rw-r--r--  2.0 unx      229 b- defN 24-May-29 03:38 sbcli_mc-1.0.4/simplyblock_core/services/service_template.service
+-rw-r--r--  2.0 unx      837 b- defN 24-May-29 03:38 sbcli_mc-1.0.4/simplyblock_core/services/install_service.sh
+-rw-r--r--  2.0 unx     4118 b- defN 24-May-29 03:38 sbcli_mc-1.0.4/simplyblock_core/services/__init__.py
+-rw-r--r--  2.0 unx     2410 b- defN 24-May-29 03:38 sbcli_mc-1.0.4/simplyblock_core/services/log_agg_service.py
+-rw-r--r--  2.0 unx     5751 b- defN 24-May-29 03:38 sbcli_mc-1.0.4/simplyblock_core/services/health_check_service.py
+-rw-r--r--  2.0 unx     7439 b- defN 24-May-29 03:38 sbcli_mc-1.0.4/simplyblock_core/services/capacity_and_stats_collector.py
+-rw-r--r--  2.0 unx     3169 b- defN 24-May-29 03:38 sbcli_mc-1.0.4/simplyblock_core/services/device_monitor.py
+-rw-r--r--  2.0 unx     5276 b- defN 24-May-29 03:38 sbcli_mc-1.0.4/simplyblock_core/services/lvol_stat_collector.py
+-rw-r--r--  2.0 unx     2671 b- defN 24-May-29 03:38 sbcli_mc-1.0.4/simplyblock_core/services/cap_monitor.py
+-rw-r--r--  2.0 unx     6822 b- defN 24-May-29 03:38 sbcli_mc-1.0.4/simplyblock_core/services/storage_node_monitor.py
+-rw-r--r--  2.0 unx     2428 b- defN 24-May-29 03:38 sbcli_mc-1.0.4/simplyblock_core/services/port_stat_collector.py
+-rw-r--r--  2.0 unx     5154 b- defN 24-May-29 03:38 sbcli_mc-1.0.4/simplyblock_core/services/distr_event_collector.py
+-rw-r--r--  2.0 unx      173 b- defN 24-May-29 03:38 sbcli_mc-1.0.4/simplyblock_core/services/remove_service.sh
+-rw-r--r--  2.0 unx     3003 b- defN 24-May-29 03:38 sbcli_mc-1.0.4/simplyblock_core/services/mgmt_node_monitor.py
+-rw-r--r--  2.0 unx     2197 b- defN 24-May-29 03:38 sbcli_mc-1.0.4/simplyblock_core/services/lvol_monitor.py
+-rw-r--r--  2.0 unx    10498 b- defN 24-May-29 03:38 sbcli_mc-1.0.4/simplyblock_core/controllers/pool_controller.py
+-rw-r--r--  2.0 unx        0 b- defN 24-May-29 03:38 sbcli_mc-1.0.4/simplyblock_core/controllers/__init__.py
+-rw-r--r--  2.0 unx     1521 b- defN 24-May-29 03:38 sbcli_mc-1.0.4/simplyblock_core/controllers/storage_events.py
+-rw-r--r--  2.0 unx    49039 b- defN 24-May-29 03:38 sbcli_mc-1.0.4/simplyblock_core/controllers/lvol_controller.py
+-rw-r--r--  2.0 unx     1568 b- defN 24-May-29 03:38 sbcli_mc-1.0.4/simplyblock_core/controllers/device_events.py
+-rw-r--r--  2.0 unx     1630 b- defN 24-May-29 03:38 sbcli_mc-1.0.4/simplyblock_core/controllers/lvol_events.py
+-rw-r--r--  2.0 unx    11066 b- defN 24-May-29 03:38 sbcli_mc-1.0.4/simplyblock_core/controllers/snapshot_controller.py
+-rw-r--r--  2.0 unx     1122 b- defN 24-May-29 03:38 sbcli_mc-1.0.4/simplyblock_core/controllers/snapshot_events.py
+-rw-r--r--  2.0 unx     3191 b- defN 24-May-29 03:38 sbcli_mc-1.0.4/simplyblock_core/controllers/events_controller.py
+-rw-r--r--  2.0 unx    10852 b- defN 24-May-29 03:38 sbcli_mc-1.0.4/simplyblock_core/controllers/health_controller.py
+-rw-r--r--  2.0 unx    13948 b- defN 24-May-29 03:38 sbcli_mc-1.0.4/simplyblock_core/controllers/device_controller.py
+-rw-r--r--  2.0 unx      695 b- defN 24-May-29 03:38 sbcli_mc-1.0.4/simplyblock_core/controllers/pool_events.py
+-rw-r--r--  2.0 unx    23440 b- defN 24-May-29 03:38 sbcli_mc-1.0.4/simplyblock_core/controllers/caching_node_controller.py
+-rw-r--r--  2.0 unx     1900 b- defN 24-May-29 03:38 sbcli_mc-1.0.4/simplyblock_core/controllers/cluster_events.py
+-rw-r--r--  2.0 unx     1120 b- defN 24-May-29 03:38 sbcli_mc-1.0.4/simplyblock_core/controllers/mgmt_events.py
+-rw-r--r--  2.0 unx     3766 b- defN 24-May-29 03:38 sbcli_mc-1.0.4/simplyblock_core/models/caching_node.py
+-rw-r--r--  2.0 unx     2094 b- defN 24-May-29 03:38 sbcli_mc-1.0.4/simplyblock_core/models/nvme_device.py
+-rw-r--r--  2.0 unx     1452 b- defN 24-May-29 03:38 sbcli_mc-1.0.4/simplyblock_core/models/mgmt_node.py
+-rw-r--r--  2.0 unx      917 b- defN 24-May-29 03:38 sbcli_mc-1.0.4/simplyblock_core/models/compute_node.py
+-rw-r--r--  2.0 unx        0 b- defN 24-May-29 03:38 sbcli_mc-1.0.4/simplyblock_core/models/__init__.py
+-rw-r--r--  2.0 unx     1500 b- defN 24-May-29 03:38 sbcli_mc-1.0.4/simplyblock_core/models/events.py
+-rw-r--r--  2.0 unx     1228 b- defN 24-May-29 03:38 sbcli_mc-1.0.4/simplyblock_core/models/global_settings.py
+-rw-r--r--  2.0 unx      973 b- defN 24-May-29 03:38 sbcli_mc-1.0.4/simplyblock_core/models/job_schedule.py
+-rw-r--r--  2.0 unx     4846 b- defN 24-May-29 03:38 sbcli_mc-1.0.4/simplyblock_core/models/base_model.py
+-rw-r--r--  2.0 unx     2579 b- defN 24-May-29 03:38 sbcli_mc-1.0.4/simplyblock_core/models/lvol_model.py
+-rw-r--r--  2.0 unx      736 b- defN 24-May-29 03:38 sbcli_mc-1.0.4/simplyblock_core/models/snapshot.py
+-rw-r--r--  2.0 unx     3696 b- defN 24-May-29 03:38 sbcli_mc-1.0.4/simplyblock_core/models/storage_node.py
+-rw-r--r--  2.0 unx     4242 b- defN 24-May-29 03:38 sbcli_mc-1.0.4/simplyblock_core/models/stats.py
+-rw-r--r--  2.0 unx     1602 b- defN 24-May-29 03:38 sbcli_mc-1.0.4/simplyblock_core/models/pool.py
+-rw-r--r--  2.0 unx      806 b- defN 24-May-29 03:38 sbcli_mc-1.0.4/simplyblock_core/models/iface.py
+-rw-r--r--  2.0 unx     2565 b- defN 24-May-29 03:38 sbcli_mc-1.0.4/simplyblock_core/models/cluster.py
+-rw-r--r--  2.0 unx     1020 b- defN 24-May-29 03:38 sbcli_mc-1.0.4/simplyblock_core/models/port_stat.py
+drwxr-xr-x  2.0 unx        0 b- stor 24-May-29 03:38 sbcli_mc-1.0.4/simplyblock_core/scripts/alerting/
+drwxr-xr-x  2.0 unx        0 b- stor 24-May-29 03:38 sbcli_mc-1.0.4/simplyblock_core/scripts/dashboards/
+-rw-r--r--  2.0 unx     1420 b- defN 24-May-29 03:38 sbcli_mc-1.0.4/simplyblock_core/scripts/install_deps.sh
+-rw-r--r--  2.0 unx     1782 b- defN 24-May-29 03:38 sbcli_mc-1.0.4/simplyblock_core/scripts/__init__.py
+-rw-r--r--  2.0 unx       43 b- defN 24-May-29 03:38 sbcli_mc-1.0.4/simplyblock_core/scripts/run_ssh.sh
+-rw-r--r--  2.0 unx     1163 b- defN 24-May-29 03:38 sbcli_mc-1.0.4/simplyblock_core/scripts/haproxy.cfg
+-rw-r--r--  2.0 unx      118 b- defN 24-May-29 03:38 sbcli_mc-1.0.4/simplyblock_core/scripts/db_config_double.sh
+-rw-r--r--  2.0 unx     5305 b- defN 24-May-29 03:38 sbcli_mc-1.0.4/simplyblock_core/scripts/stack_deploy_wait.sh
+-rw-r--r--  2.0 unx      360 b- defN 24-May-29 03:38 sbcli_mc-1.0.4/simplyblock_core/scripts/datasource.yml
+-rw-r--r--  2.0 unx     5611 b- defN 24-May-29 03:38 sbcli_mc-1.0.4/simplyblock_core/scripts/docker-compose-swarm.yml
+-rw-r--r--  2.0 unx      152 b- defN 24-May-29 03:38 sbcli_mc-1.0.4/simplyblock_core/scripts/set_db_config.sh
+-rwxr-xr-x  2.0 unx      657 b- defN 24-May-29 03:38 sbcli_mc-1.0.4/simplyblock_core/scripts/apply_dashboard.sh
+-rw-r--r--  2.0 unx      311 b- defN 24-May-29 03:38 sbcli_mc-1.0.4/simplyblock_core/scripts/prometheus.yml
+-rw-r--r--  2.0 unx      311 b- defN 24-May-29 03:38 sbcli_mc-1.0.4/simplyblock_core/scripts/clean_local_storage_deploy.sh
+-rw-r--r--  2.0 unx     4409 b- defN 24-May-29 03:38 sbcli_mc-1.0.4/simplyblock_core/scripts/docker-compose-swarm-monitoring.yml
+-rw-r--r--  2.0 unx      930 b- defN 24-May-29 03:38 sbcli_mc-1.0.4/simplyblock_core/scripts/deploy_stack.sh
+-rw-r--r--  2.0 unx       54 b- defN 24-May-29 03:38 sbcli_mc-1.0.4/simplyblock_core/scripts/db_config_single.sh
+-rw-r--r--  2.0 unx      453 b- defN 24-May-29 03:38 sbcli_mc-1.0.4/simplyblock_core/scripts/config_docker.sh
+-rw-r--r--  2.0 unx    25433 b- defN 24-May-29 03:38 sbcli_mc-1.0.4/simplyblock_core/scripts/alerting/alert_rules.yaml
+-rw-r--r--  2.0 unx     1856 b- defN 24-May-29 03:38 sbcli_mc-1.0.4/simplyblock_core/scripts/alerting/alert_resources.yaml
+-rw-r--r--  2.0 unx    88820 b- defN 24-May-29 03:38 sbcli_mc-1.0.4/simplyblock_core/scripts/dashboards/nodes.json
+-rw-r--r--  2.0 unx    88911 b- defN 24-May-29 03:38 sbcli_mc-1.0.4/simplyblock_core/scripts/dashboards/cluster.json
+-rw-r--r--  2.0 unx    88776 b- defN 24-May-29 03:38 sbcli_mc-1.0.4/simplyblock_core/scripts/dashboards/lvols.json
+-rw-r--r--  2.0 unx    88868 b- defN 24-May-29 03:38 sbcli_mc-1.0.4/simplyblock_core/scripts/dashboards/devices.json
+-rw-r--r--  2.0 unx    99707 b- defN 24-May-29 03:38 sbcli_mc-1.0.4/simplyblock_core/scripts/dashboards/pools.json
+-rw-r--r--  2.0 unx   799409 b- defN 24-May-29 03:38 sbcli_mc-1.0.4/simplyblock_core/scripts/dashboards/node-exporter.json
+-rw-r--r--  2.0 unx     5261 b- defN 24-May-29 03:38 sbcli_mc-1.0.4/sbcli_mc.egg-info/SOURCES.txt
+-rw-r--r--  2.0 unx       73 b- defN 24-May-29 03:38 sbcli_mc-1.0.4/sbcli_mc.egg-info/requires.txt
+-rw-r--r--  2.0 unx     1488 b- defN 24-May-29 03:38 sbcli_mc-1.0.4/sbcli_mc.egg-info/PKG-INFO
+-rw-r--r--  2.0 unx       49 b- defN 24-May-29 03:38 sbcli_mc-1.0.4/sbcli_mc.egg-info/top_level.txt
+-rw-r--r--  2.0 unx       54 b- defN 24-May-29 03:38 sbcli_mc-1.0.4/sbcli_mc.egg-info/entry_points.txt
+-rw-r--r--  2.0 unx        1 b- defN 24-May-29 03:38 sbcli_mc-1.0.4/sbcli_mc.egg-info/dependency_links.txt
+148 files, 1874951 bytes uncompressed, 186157 bytes compressed:  90.1%
```

## zipnote {}

```diff
@@ -1,445 +1,445 @@
-Filename: sbcli_mc-1.0.2/
+Filename: sbcli_mc-1.0.4/
 Comment: 
 
-Filename: sbcli_mc-1.0.2/simplyblock_cli/
+Filename: sbcli_mc-1.0.4/simplyblock_cli/
 Comment: 
 
-Filename: sbcli_mc-1.0.2/simplyblock_web/
+Filename: sbcli_mc-1.0.4/simplyblock_web/
 Comment: 
 
-Filename: sbcli_mc-1.0.2/simplyblock_core/
+Filename: sbcli_mc-1.0.4/simplyblock_core/
 Comment: 
 
-Filename: sbcli_mc-1.0.2/sbcli_mc.egg-info/
+Filename: sbcli_mc-1.0.4/sbcli_mc.egg-info/
 Comment: 
 
-Filename: sbcli_mc-1.0.2/README.md
+Filename: sbcli_mc-1.0.4/README.md
 Comment: 
 
-Filename: sbcli_mc-1.0.2/pyproject.toml
+Filename: sbcli_mc-1.0.4/pyproject.toml
 Comment: 
 
-Filename: sbcli_mc-1.0.2/PKG-INFO
+Filename: sbcli_mc-1.0.4/PKG-INFO
 Comment: 
 
-Filename: sbcli_mc-1.0.2/env_var
+Filename: sbcli_mc-1.0.4/env_var
 Comment: 
 
-Filename: sbcli_mc-1.0.2/setup.cfg
+Filename: sbcli_mc-1.0.4/setup.cfg
 Comment: 
 
-Filename: sbcli_mc-1.0.2/setup.py
+Filename: sbcli_mc-1.0.4/setup.py
 Comment: 
 
-Filename: sbcli_mc-1.0.2/simplyblock_cli/cli.py
+Filename: sbcli_mc-1.0.4/simplyblock_cli/cli.py
 Comment: 
 
-Filename: sbcli_mc-1.0.2/simplyblock_cli/main.py
+Filename: sbcli_mc-1.0.4/simplyblock_cli/main.py
 Comment: 
 
-Filename: sbcli_mc-1.0.2/simplyblock_web/static/
+Filename: sbcli_mc-1.0.4/simplyblock_web/static/
 Comment: 
 
-Filename: sbcli_mc-1.0.2/simplyblock_web/blueprints/
+Filename: sbcli_mc-1.0.4/simplyblock_web/blueprints/
 Comment: 
 
-Filename: sbcli_mc-1.0.2/simplyblock_web/templates/
+Filename: sbcli_mc-1.0.4/simplyblock_web/templates/
 Comment: 
 
-Filename: sbcli_mc-1.0.2/simplyblock_web/__init__.py
+Filename: sbcli_mc-1.0.4/simplyblock_web/__init__.py
 Comment: 
 
-Filename: sbcli_mc-1.0.2/simplyblock_web/node_webapp.py
+Filename: sbcli_mc-1.0.4/simplyblock_web/node_webapp.py
 Comment: 
 
-Filename: sbcli_mc-1.0.2/simplyblock_web/snode_app.py
+Filename: sbcli_mc-1.0.4/simplyblock_web/snode_app.py
 Comment: 
 
-Filename: sbcli_mc-1.0.2/simplyblock_web/caching_node_app.py
+Filename: sbcli_mc-1.0.4/simplyblock_web/caching_node_app.py
 Comment: 
 
-Filename: sbcli_mc-1.0.2/simplyblock_web/auth_middleware.py
+Filename: sbcli_mc-1.0.4/simplyblock_web/auth_middleware.py
 Comment: 
 
-Filename: sbcli_mc-1.0.2/simplyblock_web/node_utils.py
+Filename: sbcli_mc-1.0.4/simplyblock_web/node_utils.py
 Comment: 
 
-Filename: sbcli_mc-1.0.2/simplyblock_web/utils.py
+Filename: sbcli_mc-1.0.4/simplyblock_web/utils.py
 Comment: 
 
-Filename: sbcli_mc-1.0.2/simplyblock_web/app.py
+Filename: sbcli_mc-1.0.4/simplyblock_web/app.py
 Comment: 
 
-Filename: sbcli_mc-1.0.2/simplyblock_web/caching_node_app_k8s.py
+Filename: sbcli_mc-1.0.4/simplyblock_web/caching_node_app_k8s.py
 Comment: 
 
-Filename: sbcli_mc-1.0.2/simplyblock_web/static/tst.py
+Filename: sbcli_mc-1.0.4/simplyblock_web/static/tst.py
 Comment: 
 
-Filename: sbcli_mc-1.0.2/simplyblock_web/static/delete.py
+Filename: sbcli_mc-1.0.4/simplyblock_web/static/delete.py
 Comment: 
 
-Filename: sbcli_mc-1.0.2/simplyblock_web/static/deploy_cnode.yaml
+Filename: sbcli_mc-1.0.4/simplyblock_web/static/deploy_cnode.yaml
 Comment: 
 
-Filename: sbcli_mc-1.0.2/simplyblock_web/static/is_up.py
+Filename: sbcli_mc-1.0.4/simplyblock_web/static/is_up.py
 Comment: 
 
-Filename: sbcli_mc-1.0.2/simplyblock_web/static/deploy_spdk.yaml
+Filename: sbcli_mc-1.0.4/simplyblock_web/static/deploy_spdk.yaml
 Comment: 
 
-Filename: sbcli_mc-1.0.2/simplyblock_web/static/rpac.yaml
+Filename: sbcli_mc-1.0.4/simplyblock_web/static/rpac.yaml
 Comment: 
 
-Filename: sbcli_mc-1.0.2/simplyblock_web/static/list_deps.py
+Filename: sbcli_mc-1.0.4/simplyblock_web/static/list_deps.py
 Comment: 
 
-Filename: sbcli_mc-1.0.2/simplyblock_web/static/deploy.py
+Filename: sbcli_mc-1.0.4/simplyblock_web/static/deploy.py
 Comment: 
 
-Filename: sbcli_mc-1.0.2/simplyblock_web/blueprints/web_api_pool.py
+Filename: sbcli_mc-1.0.4/simplyblock_web/blueprints/web_api_pool.py
 Comment: 
 
-Filename: sbcli_mc-1.0.2/simplyblock_web/blueprints/__init__.py
+Filename: sbcli_mc-1.0.4/simplyblock_web/blueprints/__init__.py
 Comment: 
 
-Filename: sbcli_mc-1.0.2/simplyblock_web/blueprints/web_api_device.py
+Filename: sbcli_mc-1.0.4/simplyblock_web/blueprints/web_api_device.py
 Comment: 
 
-Filename: sbcli_mc-1.0.2/simplyblock_web/blueprints/web_api_lvol.py
+Filename: sbcli_mc-1.0.4/simplyblock_web/blueprints/web_api_lvol.py
 Comment: 
 
-Filename: sbcli_mc-1.0.2/simplyblock_web/blueprints/snode_ops.py
+Filename: sbcli_mc-1.0.4/simplyblock_web/blueprints/snode_ops.py
 Comment: 
 
-Filename: sbcli_mc-1.0.2/simplyblock_web/blueprints/caching_node_ops.py
+Filename: sbcli_mc-1.0.4/simplyblock_web/blueprints/caching_node_ops.py
 Comment: 
 
-Filename: sbcli_mc-1.0.2/simplyblock_web/blueprints/web_api_storage_node.py
+Filename: sbcli_mc-1.0.4/simplyblock_web/blueprints/web_api_storage_node.py
 Comment: 
 
-Filename: sbcli_mc-1.0.2/simplyblock_web/blueprints/web_api_cluster.py
+Filename: sbcli_mc-1.0.4/simplyblock_web/blueprints/web_api_cluster.py
 Comment: 
 
-Filename: sbcli_mc-1.0.2/simplyblock_web/blueprints/caching_node_ops_k8s.py
+Filename: sbcli_mc-1.0.4/simplyblock_web/blueprints/caching_node_ops_k8s.py
 Comment: 
 
-Filename: sbcli_mc-1.0.2/simplyblock_web/blueprints/node_api_caching_ks.py
+Filename: sbcli_mc-1.0.4/simplyblock_web/blueprints/node_api_caching_ks.py
 Comment: 
 
-Filename: sbcli_mc-1.0.2/simplyblock_web/blueprints/node_api_caching_docker.py
+Filename: sbcli_mc-1.0.4/simplyblock_web/blueprints/node_api_caching_docker.py
 Comment: 
 
-Filename: sbcli_mc-1.0.2/simplyblock_web/blueprints/web_api_caching_node.py
+Filename: sbcli_mc-1.0.4/simplyblock_web/blueprints/web_api_caching_node.py
 Comment: 
 
-Filename: sbcli_mc-1.0.2/simplyblock_web/blueprints/node_api_basic.py
+Filename: sbcli_mc-1.0.4/simplyblock_web/blueprints/node_api_basic.py
 Comment: 
 
-Filename: sbcli_mc-1.0.2/simplyblock_web/blueprints/csi.py
+Filename: sbcli_mc-1.0.4/simplyblock_web/blueprints/csi.py
 Comment: 
 
-Filename: sbcli_mc-1.0.2/simplyblock_web/blueprints/web_api_mgmt_node.py
+Filename: sbcli_mc-1.0.4/simplyblock_web/blueprints/web_api_mgmt_node.py
 Comment: 
 
-Filename: sbcli_mc-1.0.2/simplyblock_web/templates/deploy_spdk.yaml.j2
+Filename: sbcli_mc-1.0.4/simplyblock_web/templates/deploy_spdk.yaml.j2
 Comment: 
 
-Filename: sbcli_mc-1.0.2/simplyblock_core/services/
+Filename: sbcli_mc-1.0.4/simplyblock_core/services/
 Comment: 
 
-Filename: sbcli_mc-1.0.2/simplyblock_core/controllers/
+Filename: sbcli_mc-1.0.4/simplyblock_core/controllers/
 Comment: 
 
-Filename: sbcli_mc-1.0.2/simplyblock_core/models/
+Filename: sbcli_mc-1.0.4/simplyblock_core/models/
 Comment: 
 
-Filename: sbcli_mc-1.0.2/simplyblock_core/scripts/
+Filename: sbcli_mc-1.0.4/simplyblock_core/scripts/
 Comment: 
 
-Filename: sbcli_mc-1.0.2/simplyblock_core/cluster_ops.py
+Filename: sbcli_mc-1.0.4/simplyblock_core/cluster_ops.py
 Comment: 
 
-Filename: sbcli_mc-1.0.2/simplyblock_core/pci_utils.py
+Filename: sbcli_mc-1.0.4/simplyblock_core/pci_utils.py
 Comment: 
 
-Filename: sbcli_mc-1.0.2/simplyblock_core/__init__.py
+Filename: sbcli_mc-1.0.4/simplyblock_core/__init__.py
 Comment: 
 
-Filename: sbcli_mc-1.0.2/simplyblock_core/snode_client.py
+Filename: sbcli_mc-1.0.4/simplyblock_core/snode_client.py
 Comment: 
 
-Filename: sbcli_mc-1.0.2/simplyblock_core/kv_store.py
+Filename: sbcli_mc-1.0.4/simplyblock_core/kv_store.py
 Comment: 
 
-Filename: sbcli_mc-1.0.2/simplyblock_core/compute_node_ops.py
+Filename: sbcli_mc-1.0.4/simplyblock_core/compute_node_ops.py
 Comment: 
 
-Filename: sbcli_mc-1.0.2/simplyblock_core/rpc_client.py
+Filename: sbcli_mc-1.0.4/simplyblock_core/rpc_client.py
 Comment: 
 
-Filename: sbcli_mc-1.0.2/simplyblock_core/mgmt_node_ops.py
+Filename: sbcli_mc-1.0.4/simplyblock_core/mgmt_node_ops.py
 Comment: 
 
-Filename: sbcli_mc-1.0.2/simplyblock_core/utils.py
+Filename: sbcli_mc-1.0.4/simplyblock_core/utils.py
 Comment: 
 
-Filename: sbcli_mc-1.0.2/simplyblock_core/distr_controller.py
+Filename: sbcli_mc-1.0.4/simplyblock_core/distr_controller.py
 Comment: 
 
-Filename: sbcli_mc-1.0.2/simplyblock_core/shell_utils.py
+Filename: sbcli_mc-1.0.4/simplyblock_core/shell_utils.py
 Comment: 
 
-Filename: sbcli_mc-1.0.2/simplyblock_core/cnode_client.py
+Filename: sbcli_mc-1.0.4/simplyblock_core/cnode_client.py
 Comment: 
 
-Filename: sbcli_mc-1.0.2/simplyblock_core/storage_node_ops.py
+Filename: sbcli_mc-1.0.4/simplyblock_core/storage_node_ops.py
 Comment: 
 
-Filename: sbcli_mc-1.0.2/simplyblock_core/constants.py
+Filename: sbcli_mc-1.0.4/simplyblock_core/constants.py
 Comment: 
 
-Filename: sbcli_mc-1.0.2/simplyblock_core/services/job_tasks.py
+Filename: sbcli_mc-1.0.4/simplyblock_core/services/job_tasks.py
 Comment: 
 
-Filename: sbcli_mc-1.0.2/simplyblock_core/services/caching_node_monitor.py
+Filename: sbcli_mc-1.0.4/simplyblock_core/services/caching_node_monitor.py
 Comment: 
 
-Filename: sbcli_mc-1.0.2/simplyblock_core/services/service_template.service
+Filename: sbcli_mc-1.0.4/simplyblock_core/services/service_template.service
 Comment: 
 
-Filename: sbcli_mc-1.0.2/simplyblock_core/services/install_service.sh
+Filename: sbcli_mc-1.0.4/simplyblock_core/services/install_service.sh
 Comment: 
 
-Filename: sbcli_mc-1.0.2/simplyblock_core/services/__init__.py
+Filename: sbcli_mc-1.0.4/simplyblock_core/services/__init__.py
 Comment: 
 
-Filename: sbcli_mc-1.0.2/simplyblock_core/services/log_agg_service.py
+Filename: sbcli_mc-1.0.4/simplyblock_core/services/log_agg_service.py
 Comment: 
 
-Filename: sbcli_mc-1.0.2/simplyblock_core/services/health_check_service.py
+Filename: sbcli_mc-1.0.4/simplyblock_core/services/health_check_service.py
 Comment: 
 
-Filename: sbcli_mc-1.0.2/simplyblock_core/services/capacity_and_stats_collector.py
+Filename: sbcli_mc-1.0.4/simplyblock_core/services/capacity_and_stats_collector.py
 Comment: 
 
-Filename: sbcli_mc-1.0.2/simplyblock_core/services/device_monitor.py
+Filename: sbcli_mc-1.0.4/simplyblock_core/services/device_monitor.py
 Comment: 
 
-Filename: sbcli_mc-1.0.2/simplyblock_core/services/lvol_stat_collector.py
+Filename: sbcli_mc-1.0.4/simplyblock_core/services/lvol_stat_collector.py
 Comment: 
 
-Filename: sbcli_mc-1.0.2/simplyblock_core/services/cap_monitor.py
+Filename: sbcli_mc-1.0.4/simplyblock_core/services/cap_monitor.py
 Comment: 
 
-Filename: sbcli_mc-1.0.2/simplyblock_core/services/storage_node_monitor.py
+Filename: sbcli_mc-1.0.4/simplyblock_core/services/storage_node_monitor.py
 Comment: 
 
-Filename: sbcli_mc-1.0.2/simplyblock_core/services/port_stat_collector.py
+Filename: sbcli_mc-1.0.4/simplyblock_core/services/port_stat_collector.py
 Comment: 
 
-Filename: sbcli_mc-1.0.2/simplyblock_core/services/distr_event_collector.py
+Filename: sbcli_mc-1.0.4/simplyblock_core/services/distr_event_collector.py
 Comment: 
 
-Filename: sbcli_mc-1.0.2/simplyblock_core/services/remove_service.sh
+Filename: sbcli_mc-1.0.4/simplyblock_core/services/remove_service.sh
 Comment: 
 
-Filename: sbcli_mc-1.0.2/simplyblock_core/services/mgmt_node_monitor.py
+Filename: sbcli_mc-1.0.4/simplyblock_core/services/mgmt_node_monitor.py
 Comment: 
 
-Filename: sbcli_mc-1.0.2/simplyblock_core/services/lvol_monitor.py
+Filename: sbcli_mc-1.0.4/simplyblock_core/services/lvol_monitor.py
 Comment: 
 
-Filename: sbcli_mc-1.0.2/simplyblock_core/controllers/pool_controller.py
+Filename: sbcli_mc-1.0.4/simplyblock_core/controllers/pool_controller.py
 Comment: 
 
-Filename: sbcli_mc-1.0.2/simplyblock_core/controllers/__init__.py
+Filename: sbcli_mc-1.0.4/simplyblock_core/controllers/__init__.py
 Comment: 
 
-Filename: sbcli_mc-1.0.2/simplyblock_core/controllers/storage_events.py
+Filename: sbcli_mc-1.0.4/simplyblock_core/controllers/storage_events.py
 Comment: 
 
-Filename: sbcli_mc-1.0.2/simplyblock_core/controllers/lvol_controller.py
+Filename: sbcli_mc-1.0.4/simplyblock_core/controllers/lvol_controller.py
 Comment: 
 
-Filename: sbcli_mc-1.0.2/simplyblock_core/controllers/device_events.py
+Filename: sbcli_mc-1.0.4/simplyblock_core/controllers/device_events.py
 Comment: 
 
-Filename: sbcli_mc-1.0.2/simplyblock_core/controllers/lvol_events.py
+Filename: sbcli_mc-1.0.4/simplyblock_core/controllers/lvol_events.py
 Comment: 
 
-Filename: sbcli_mc-1.0.2/simplyblock_core/controllers/snapshot_controller.py
+Filename: sbcli_mc-1.0.4/simplyblock_core/controllers/snapshot_controller.py
 Comment: 
 
-Filename: sbcli_mc-1.0.2/simplyblock_core/controllers/snapshot_events.py
+Filename: sbcli_mc-1.0.4/simplyblock_core/controllers/snapshot_events.py
 Comment: 
 
-Filename: sbcli_mc-1.0.2/simplyblock_core/controllers/events_controller.py
+Filename: sbcli_mc-1.0.4/simplyblock_core/controllers/events_controller.py
 Comment: 
 
-Filename: sbcli_mc-1.0.2/simplyblock_core/controllers/health_controller.py
+Filename: sbcli_mc-1.0.4/simplyblock_core/controllers/health_controller.py
 Comment: 
 
-Filename: sbcli_mc-1.0.2/simplyblock_core/controllers/device_controller.py
+Filename: sbcli_mc-1.0.4/simplyblock_core/controllers/device_controller.py
 Comment: 
 
-Filename: sbcli_mc-1.0.2/simplyblock_core/controllers/pool_events.py
+Filename: sbcli_mc-1.0.4/simplyblock_core/controllers/pool_events.py
 Comment: 
 
-Filename: sbcli_mc-1.0.2/simplyblock_core/controllers/caching_node_controller.py
+Filename: sbcli_mc-1.0.4/simplyblock_core/controllers/caching_node_controller.py
 Comment: 
 
-Filename: sbcli_mc-1.0.2/simplyblock_core/controllers/cluster_events.py
+Filename: sbcli_mc-1.0.4/simplyblock_core/controllers/cluster_events.py
 Comment: 
 
-Filename: sbcli_mc-1.0.2/simplyblock_core/controllers/mgmt_events.py
+Filename: sbcli_mc-1.0.4/simplyblock_core/controllers/mgmt_events.py
 Comment: 
 
-Filename: sbcli_mc-1.0.2/simplyblock_core/models/caching_node.py
+Filename: sbcli_mc-1.0.4/simplyblock_core/models/caching_node.py
 Comment: 
 
-Filename: sbcli_mc-1.0.2/simplyblock_core/models/nvme_device.py
+Filename: sbcli_mc-1.0.4/simplyblock_core/models/nvme_device.py
 Comment: 
 
-Filename: sbcli_mc-1.0.2/simplyblock_core/models/mgmt_node.py
+Filename: sbcli_mc-1.0.4/simplyblock_core/models/mgmt_node.py
 Comment: 
 
-Filename: sbcli_mc-1.0.2/simplyblock_core/models/compute_node.py
+Filename: sbcli_mc-1.0.4/simplyblock_core/models/compute_node.py
 Comment: 
 
-Filename: sbcli_mc-1.0.2/simplyblock_core/models/__init__.py
+Filename: sbcli_mc-1.0.4/simplyblock_core/models/__init__.py
 Comment: 
 
-Filename: sbcli_mc-1.0.2/simplyblock_core/models/events.py
+Filename: sbcli_mc-1.0.4/simplyblock_core/models/events.py
 Comment: 
 
-Filename: sbcli_mc-1.0.2/simplyblock_core/models/global_settings.py
+Filename: sbcli_mc-1.0.4/simplyblock_core/models/global_settings.py
 Comment: 
 
-Filename: sbcli_mc-1.0.2/simplyblock_core/models/job_schedule.py
+Filename: sbcli_mc-1.0.4/simplyblock_core/models/job_schedule.py
 Comment: 
 
-Filename: sbcli_mc-1.0.2/simplyblock_core/models/base_model.py
+Filename: sbcli_mc-1.0.4/simplyblock_core/models/base_model.py
 Comment: 
 
-Filename: sbcli_mc-1.0.2/simplyblock_core/models/lvol_model.py
+Filename: sbcli_mc-1.0.4/simplyblock_core/models/lvol_model.py
 Comment: 
 
-Filename: sbcli_mc-1.0.2/simplyblock_core/models/snapshot.py
+Filename: sbcli_mc-1.0.4/simplyblock_core/models/snapshot.py
 Comment: 
 
-Filename: sbcli_mc-1.0.2/simplyblock_core/models/storage_node.py
+Filename: sbcli_mc-1.0.4/simplyblock_core/models/storage_node.py
 Comment: 
 
-Filename: sbcli_mc-1.0.2/simplyblock_core/models/stats.py
+Filename: sbcli_mc-1.0.4/simplyblock_core/models/stats.py
 Comment: 
 
-Filename: sbcli_mc-1.0.2/simplyblock_core/models/pool.py
+Filename: sbcli_mc-1.0.4/simplyblock_core/models/pool.py
 Comment: 
 
-Filename: sbcli_mc-1.0.2/simplyblock_core/models/iface.py
+Filename: sbcli_mc-1.0.4/simplyblock_core/models/iface.py
 Comment: 
 
-Filename: sbcli_mc-1.0.2/simplyblock_core/models/cluster.py
+Filename: sbcli_mc-1.0.4/simplyblock_core/models/cluster.py
 Comment: 
 
-Filename: sbcli_mc-1.0.2/simplyblock_core/models/port_stat.py
+Filename: sbcli_mc-1.0.4/simplyblock_core/models/port_stat.py
 Comment: 
 
-Filename: sbcli_mc-1.0.2/simplyblock_core/scripts/alerting/
+Filename: sbcli_mc-1.0.4/simplyblock_core/scripts/alerting/
 Comment: 
 
-Filename: sbcli_mc-1.0.2/simplyblock_core/scripts/dashboards/
+Filename: sbcli_mc-1.0.4/simplyblock_core/scripts/dashboards/
 Comment: 
 
-Filename: sbcli_mc-1.0.2/simplyblock_core/scripts/install_deps.sh
+Filename: sbcli_mc-1.0.4/simplyblock_core/scripts/install_deps.sh
 Comment: 
 
-Filename: sbcli_mc-1.0.2/simplyblock_core/scripts/__init__.py
+Filename: sbcli_mc-1.0.4/simplyblock_core/scripts/__init__.py
 Comment: 
 
-Filename: sbcli_mc-1.0.2/simplyblock_core/scripts/run_ssh.sh
+Filename: sbcli_mc-1.0.4/simplyblock_core/scripts/run_ssh.sh
 Comment: 
 
-Filename: sbcli_mc-1.0.2/simplyblock_core/scripts/haproxy.cfg
+Filename: sbcli_mc-1.0.4/simplyblock_core/scripts/haproxy.cfg
 Comment: 
 
-Filename: sbcli_mc-1.0.2/simplyblock_core/scripts/db_config_double.sh
+Filename: sbcli_mc-1.0.4/simplyblock_core/scripts/db_config_double.sh
 Comment: 
 
-Filename: sbcli_mc-1.0.2/simplyblock_core/scripts/stack_deploy_wait.sh
+Filename: sbcli_mc-1.0.4/simplyblock_core/scripts/stack_deploy_wait.sh
 Comment: 
 
-Filename: sbcli_mc-1.0.2/simplyblock_core/scripts/datasource.yml
+Filename: sbcli_mc-1.0.4/simplyblock_core/scripts/datasource.yml
 Comment: 
 
-Filename: sbcli_mc-1.0.2/simplyblock_core/scripts/docker-compose-swarm.yml
+Filename: sbcli_mc-1.0.4/simplyblock_core/scripts/docker-compose-swarm.yml
 Comment: 
 
-Filename: sbcli_mc-1.0.2/simplyblock_core/scripts/set_db_config.sh
+Filename: sbcli_mc-1.0.4/simplyblock_core/scripts/set_db_config.sh
 Comment: 
 
-Filename: sbcli_mc-1.0.2/simplyblock_core/scripts/apply_dashboard.sh
+Filename: sbcli_mc-1.0.4/simplyblock_core/scripts/apply_dashboard.sh
 Comment: 
 
-Filename: sbcli_mc-1.0.2/simplyblock_core/scripts/prometheus.yml
+Filename: sbcli_mc-1.0.4/simplyblock_core/scripts/prometheus.yml
 Comment: 
 
-Filename: sbcli_mc-1.0.2/simplyblock_core/scripts/clean_local_storage_deploy.sh
+Filename: sbcli_mc-1.0.4/simplyblock_core/scripts/clean_local_storage_deploy.sh
 Comment: 
 
-Filename: sbcli_mc-1.0.2/simplyblock_core/scripts/docker-compose-swarm-monitoring.yml
+Filename: sbcli_mc-1.0.4/simplyblock_core/scripts/docker-compose-swarm-monitoring.yml
 Comment: 
 
-Filename: sbcli_mc-1.0.2/simplyblock_core/scripts/deploy_stack.sh
+Filename: sbcli_mc-1.0.4/simplyblock_core/scripts/deploy_stack.sh
 Comment: 
 
-Filename: sbcli_mc-1.0.2/simplyblock_core/scripts/db_config_single.sh
+Filename: sbcli_mc-1.0.4/simplyblock_core/scripts/db_config_single.sh
 Comment: 
 
-Filename: sbcli_mc-1.0.2/simplyblock_core/scripts/config_docker.sh
+Filename: sbcli_mc-1.0.4/simplyblock_core/scripts/config_docker.sh
 Comment: 
 
-Filename: sbcli_mc-1.0.2/simplyblock_core/scripts/alerting/alert_rules.yaml
+Filename: sbcli_mc-1.0.4/simplyblock_core/scripts/alerting/alert_rules.yaml
 Comment: 
 
-Filename: sbcli_mc-1.0.2/simplyblock_core/scripts/alerting/alert_resources.yaml
+Filename: sbcli_mc-1.0.4/simplyblock_core/scripts/alerting/alert_resources.yaml
 Comment: 
 
-Filename: sbcli_mc-1.0.2/simplyblock_core/scripts/dashboards/nodes.json
+Filename: sbcli_mc-1.0.4/simplyblock_core/scripts/dashboards/nodes.json
 Comment: 
 
-Filename: sbcli_mc-1.0.2/simplyblock_core/scripts/dashboards/cluster.json
+Filename: sbcli_mc-1.0.4/simplyblock_core/scripts/dashboards/cluster.json
 Comment: 
 
-Filename: sbcli_mc-1.0.2/simplyblock_core/scripts/dashboards/lvols.json
+Filename: sbcli_mc-1.0.4/simplyblock_core/scripts/dashboards/lvols.json
 Comment: 
 
-Filename: sbcli_mc-1.0.2/simplyblock_core/scripts/dashboards/devices.json
+Filename: sbcli_mc-1.0.4/simplyblock_core/scripts/dashboards/devices.json
 Comment: 
 
-Filename: sbcli_mc-1.0.2/simplyblock_core/scripts/dashboards/pools.json
+Filename: sbcli_mc-1.0.4/simplyblock_core/scripts/dashboards/pools.json
 Comment: 
 
-Filename: sbcli_mc-1.0.2/simplyblock_core/scripts/dashboards/node-exporter.json
+Filename: sbcli_mc-1.0.4/simplyblock_core/scripts/dashboards/node-exporter.json
 Comment: 
 
-Filename: sbcli_mc-1.0.2/sbcli_mc.egg-info/SOURCES.txt
+Filename: sbcli_mc-1.0.4/sbcli_mc.egg-info/SOURCES.txt
 Comment: 
 
-Filename: sbcli_mc-1.0.2/sbcli_mc.egg-info/requires.txt
+Filename: sbcli_mc-1.0.4/sbcli_mc.egg-info/requires.txt
 Comment: 
 
-Filename: sbcli_mc-1.0.2/sbcli_mc.egg-info/PKG-INFO
+Filename: sbcli_mc-1.0.4/sbcli_mc.egg-info/PKG-INFO
 Comment: 
 
-Filename: sbcli_mc-1.0.2/sbcli_mc.egg-info/top_level.txt
+Filename: sbcli_mc-1.0.4/sbcli_mc.egg-info/top_level.txt
 Comment: 
 
-Filename: sbcli_mc-1.0.2/sbcli_mc.egg-info/entry_points.txt
+Filename: sbcli_mc-1.0.4/sbcli_mc.egg-info/entry_points.txt
 Comment: 
 
-Filename: sbcli_mc-1.0.2/sbcli_mc.egg-info/dependency_links.txt
+Filename: sbcli_mc-1.0.4/sbcli_mc.egg-info/dependency_links.txt
 Comment: 
 
 Zip file comment:
```

## Comparing `sbcli_mc-1.0.2/README.md` & `sbcli_mc-1.0.4/README.md`

 * *Files identical despite different names*

## Comparing `sbcli_mc-1.0.2/PKG-INFO` & `sbcli_mc-1.0.4/PKG-INFO`

 * *Files 5% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: sbcli-mc
-Version: 1.0.2
+Version: 1.0.4
 Summary: CLI for managing SimplyBlock cluster
 Home-page: https://www.simplyblock.io/
 Author: Hamdy
 Author-email: hamdy@simplyblock.io
 Description-Content-Type: text/markdown
 Requires-Dist: foundationdb
 Requires-Dist: requests
```

## Comparing `sbcli_mc-1.0.2/setup.py` & `sbcli_mc-1.0.4/setup.py`

 * *Files identical despite different names*

## Comparing `sbcli_mc-1.0.2/simplyblock_cli/cli.py` & `sbcli_mc-1.0.4/simplyblock_cli/cli.py`

 * *Files 0% similar despite different names*

```diff
@@ -373,16 +373,17 @@
         sub_command.add_argument("id", help='LVol id')
         sub_command.add_argument("--max-rw-iops", help='Maximum Read Write IO Per Second', type=int)
         sub_command.add_argument("--max-rw-mbytes", help='Maximum Read Write Mega Bytes Per Second', type=int)
         sub_command.add_argument("--max-r-mbytes", help='Maximum Read Mega Bytes Per Second', type=int)
         sub_command.add_argument("--max-w-mbytes", help='Maximum Write Mega Bytes Per Second', type=int)
 
         # list lvols
-        sub_command = self.add_sub_command(subparser, 'list', 'List all LVols')
-        sub_command.add_argument("--cluster-id", help='List LVols in particular cluster')
+        sub_command = self.add_sub_command(subparser, 'list', 'List LVols')
+        sub_command.add_argument("--cluster-id", help='List LVols in particular cluster', dest="cluster_id")
+        sub_command.add_argument("--pool", help='List LVols in particular Pool ID or name', dest="pool")
         sub_command.add_argument("--json", help='Print outputs in json format', required=False, action='store_true')
 
         # Get the size and max_size of the lvol
         sub_command = self.add_sub_command(subparser, 'list-mem', 'Get the size and max_size of the lvol')
         sub_command.add_argument("--json", help='Print outputs in json format', required=False, action='store_true')
         sub_command.add_argument("--csv", help='Print outputs in csv format', required=False, action='store_true')
 
@@ -474,15 +475,15 @@
         sub_command.add_argument("id", help='Mgmt node uuid')
 
         # pool ops
         subparser = self.add_command('pool', 'Pool commands')
         # add pool
         sub_command = self.add_sub_command(subparser, 'add', 'Add a new Pool')
         sub_command.add_argument("name", help='Pool name')
-        sub_command.add_argument("--cluster-id", help='id of the cluster', dest='cluster_id')
+        sub_command.add_argument("cluster_id", help='Cluster UUID', dest='cluster_id')
         sub_command.add_argument("--pool-max", help='Pool maximum size: 20M, 20G, 0(default)', default="0")
         sub_command.add_argument("--lvol-max", help='LVol maximum size: 20M, 20G, 0(default)', default="0")
         sub_command.add_argument("--max-rw-iops", help='Maximum Read Write IO Per Second', type=int)
         sub_command.add_argument("--max-rw-mbytes", help='Maximum Read Write Mega Bytes Per Second', type=int)
         sub_command.add_argument("--max-r-mbytes", help='Maximum Read Mega Bytes Per Second', type=int)
         sub_command.add_argument("--max-w-mbytes", help='Maximum Write Mega Bytes Per Second', type=int)
         sub_command.add_argument("--has-secret", help='Pool is created with a secret (all further API interactions '
@@ -912,15 +913,15 @@
             elif sub_command == "add-distr":
                 pass
             elif sub_command == "qos-set":
                 ret = lvol_controller.set_lvol(
                     args.id, args.max_rw_iops, args.max_rw_mbytes,
                     args.max_r_mbytes, args.max_w_mbytes)
             elif sub_command == "list":
-                ret = lvol_controller.list_lvols(args.json)
+                ret = lvol_controller.list_lvols(args.json, args.cluster_id, args.pool)
             elif sub_command == "list-mem":
                 ret = lvol_controller.list_lvols_mem(args.json, args.csv)
             elif sub_command == "get":
                 ret = lvol_controller.get_lvol(args.id, args.json)
             elif sub_command == "delete":
                 for id in args.id:
                     force = args.force
```

## Comparing `sbcli_mc-1.0.2/simplyblock_web/node_webapp.py` & `sbcli_mc-1.0.4/simplyblock_web/node_webapp.py`

 * *Files identical despite different names*

## Comparing `sbcli_mc-1.0.2/simplyblock_web/snode_app.py` & `sbcli_mc-1.0.4/simplyblock_web/snode_app.py`

 * *Files identical despite different names*

## Comparing `sbcli_mc-1.0.2/simplyblock_web/caching_node_app.py` & `sbcli_mc-1.0.4/simplyblock_web/caching_node_app.py`

 * *Files identical despite different names*

## Comparing `sbcli_mc-1.0.2/simplyblock_web/auth_middleware.py` & `sbcli_mc-1.0.4/simplyblock_web/auth_middleware.py`

 * *Files identical despite different names*

## Comparing `sbcli_mc-1.0.2/simplyblock_web/node_utils.py` & `sbcli_mc-1.0.4/simplyblock_web/node_utils.py`

 * *Files identical despite different names*

## Comparing `sbcli_mc-1.0.2/simplyblock_web/utils.py` & `sbcli_mc-1.0.4/simplyblock_web/utils.py`

 * *Files identical despite different names*

## Comparing `sbcli_mc-1.0.2/simplyblock_web/app.py` & `sbcli_mc-1.0.4/simplyblock_web/app.py`

 * *Files identical despite different names*

## Comparing `sbcli_mc-1.0.2/simplyblock_web/caching_node_app_k8s.py` & `sbcli_mc-1.0.4/simplyblock_web/caching_node_app_k8s.py`

 * *Files identical despite different names*

## Comparing `sbcli_mc-1.0.2/simplyblock_web/static/delete.py` & `sbcli_mc-1.0.4/simplyblock_web/static/delete.py`

 * *Files identical despite different names*

## Comparing `sbcli_mc-1.0.2/simplyblock_web/static/deploy_spdk.yaml` & `sbcli_mc-1.0.4/simplyblock_web/static/deploy_spdk.yaml`

 * *Files identical despite different names*

## Comparing `sbcli_mc-1.0.2/simplyblock_web/static/deploy.py` & `sbcli_mc-1.0.4/simplyblock_web/static/deploy.py`

 * *Files identical despite different names*

## Comparing `sbcli_mc-1.0.2/simplyblock_web/blueprints/web_api_pool.py` & `sbcli_mc-1.0.4/simplyblock_web/blueprints/web_api_pool.py`

 * *Files identical despite different names*

## Comparing `sbcli_mc-1.0.2/simplyblock_web/blueprints/web_api_device.py` & `sbcli_mc-1.0.4/simplyblock_web/blueprints/web_api_device.py`

 * *Files identical despite different names*

## Comparing `sbcli_mc-1.0.2/simplyblock_web/blueprints/web_api_lvol.py` & `sbcli_mc-1.0.4/simplyblock_web/blueprints/web_api_lvol.py`

 * *Files 2% similar despite different names*

```diff
@@ -15,25 +15,28 @@
 
 logger = logging.getLogger(__name__)
 logger.setLevel(logging.DEBUG)
 bp = Blueprint("lvol", __name__)
 db_controller = kv_store.DBController()
 
 
-@bp.route('/lvol', defaults={'uuid': None}, methods=['GET'])
-@bp.route('/lvol/<string:uuid>', methods=['GET'])
-def list_lvols(uuid):
+@bp.route('/lvol', defaults={'uuid': None, "cluster_id": None}, methods=['GET'])
+@bp.route('/lvol/<string:uuid>', defaults={"cluster_id": None}, methods=['GET'])
+@bp.route('/lvol/cluster_id/<string:cluster_id>', defaults={'uuid': None,}, methods=['GET'])
+def list_lvols(uuid, cluster_id):
     if uuid:
         lvol = db_controller.get_lvol_by_id(uuid)
         if lvol:
             lvols = [lvol]
         else:
             return utils.get_response_error(f"LVol not found: {uuid}", 404)
+    elif cluster_id:
+        lvols = db_controller.get_lvols(cluster_id)
     else:
-        lvols = db_controller.get_lvols()
+        lvols = db_controller.get_lvols()  # pass
     data = []
     for lvol in lvols:
         data.append(lvol.get_clean_dict())
     return utils.get_response(data)
 
 
 @bp.route('/lvol/iostats/<string:uuid>/history/<string:history>', methods=['GET'])
@@ -117,15 +120,15 @@
     for p in db_controller.get_pools():
         if pool_id_or_name == p.id or pool_id_or_name == p.pool_name:
             pool = p
             break
     if not pool:
         return utils.get_csi_response(None, f"Pool not found: {pool_id_or_name}", 400)
 
-    for lvol in db_controller.get_lvols():
+    for lvol in db_controller.get_lvols():  # pass
         if lvol.pool_uuid == pool.get_id():
             if lvol.lvol_name == name:
                 return utils.get_csi_response(lvol.get_id())
 
     rw_iops = utils.get_int_value_or_default(cl_data, "max_rw_iops", 0)
     rw_mbytes = utils.get_int_value_or_default(cl_data, "max_rw_mbytes", 0)
     r_mbytes = utils.get_int_value_or_default(cl_data, "max_r_mbytes", 0)
```

## Comparing `sbcli_mc-1.0.2/simplyblock_web/blueprints/snode_ops.py` & `sbcli_mc-1.0.4/simplyblock_web/blueprints/snode_ops.py`

 * *Files identical despite different names*

## Comparing `sbcli_mc-1.0.2/simplyblock_web/blueprints/caching_node_ops.py` & `sbcli_mc-1.0.4/simplyblock_web/blueprints/caching_node_ops.py`

 * *Files identical despite different names*

## Comparing `sbcli_mc-1.0.2/simplyblock_web/blueprints/web_api_storage_node.py` & `sbcli_mc-1.0.4/simplyblock_web/blueprints/web_api_storage_node.py`

 * *Files identical despite different names*

## Comparing `sbcli_mc-1.0.2/simplyblock_web/blueprints/web_api_cluster.py` & `sbcli_mc-1.0.4/simplyblock_web/blueprints/web_api_cluster.py`

 * *Files identical despite different names*

## Comparing `sbcli_mc-1.0.2/simplyblock_web/blueprints/caching_node_ops_k8s.py` & `sbcli_mc-1.0.4/simplyblock_web/blueprints/caching_node_ops_k8s.py`

 * *Files identical despite different names*

## Comparing `sbcli_mc-1.0.2/simplyblock_web/blueprints/node_api_caching_ks.py` & `sbcli_mc-1.0.4/simplyblock_web/blueprints/node_api_caching_ks.py`

 * *Files identical despite different names*

## Comparing `sbcli_mc-1.0.2/simplyblock_web/blueprints/node_api_caching_docker.py` & `sbcli_mc-1.0.4/simplyblock_web/blueprints/node_api_caching_docker.py`

 * *Files identical despite different names*

## Comparing `sbcli_mc-1.0.2/simplyblock_web/blueprints/web_api_caching_node.py` & `sbcli_mc-1.0.4/simplyblock_web/blueprints/web_api_caching_node.py`

 * *Files identical despite different names*

## Comparing `sbcli_mc-1.0.2/simplyblock_web/blueprints/node_api_basic.py` & `sbcli_mc-1.0.4/simplyblock_web/blueprints/node_api_basic.py`

 * *Files identical despite different names*

## Comparing `sbcli_mc-1.0.2/simplyblock_web/blueprints/csi.py` & `sbcli_mc-1.0.4/simplyblock_web/blueprints/csi.py`

 * *Files identical despite different names*

## Comparing `sbcli_mc-1.0.2/simplyblock_web/blueprints/web_api_mgmt_node.py` & `sbcli_mc-1.0.4/simplyblock_web/blueprints/web_api_mgmt_node.py`

 * *Files identical despite different names*

## Comparing `sbcli_mc-1.0.2/simplyblock_web/templates/deploy_spdk.yaml.j2` & `sbcli_mc-1.0.4/simplyblock_web/templates/deploy_spdk.yaml.j2`

 * *Files identical despite different names*

## Comparing `sbcli_mc-1.0.2/simplyblock_core/cluster_ops.py` & `sbcli_mc-1.0.4/simplyblock_core/cluster_ops.py`

 * *Files 1% similar despite different names*

```diff
@@ -353,16 +353,21 @@
         storage_node_ops.add_storage_node(cluster_id, ifname, data_nics)
 
     logger.info("Node joined the cluster")
 
 
 def add_cluster(blk_size, page_size_in_blocks, ha_type, cap_warn, cap_crit, prov_cap_warn, prov_cap_crit):
     db_controller = DBController()
+    clusters = db_controller.get_clusters()
+    if not clusters:
+        logger.error("No previous clusters found!")
+        return False
+
+    default_cluster = clusters[0]
     logger.info("Adding new cluster")
-    default_cluster = db_controller.get_clusters()[0]
     cluster = Cluster()
     cluster.uuid = str(uuid.uuid4())
     cluster.blk_size = blk_size
     cluster.page_size_in_blocks = page_size_in_blocks
     cluster.ha_type = ha_type
     cluster.nqn = f"{constants.CLUSTER_NQN}:{cluster.uuid}"
     cluster.cli_pass = default_cluster.cli_pass
```

## Comparing `sbcli_mc-1.0.2/simplyblock_core/pci_utils.py` & `sbcli_mc-1.0.4/simplyblock_core/pci_utils.py`

 * *Files identical despite different names*

## Comparing `sbcli_mc-1.0.2/simplyblock_core/snode_client.py` & `sbcli_mc-1.0.4/simplyblock_core/snode_client.py`

 * *Files identical despite different names*

## Comparing `sbcli_mc-1.0.2/simplyblock_core/kv_store.py` & `sbcli_mc-1.0.4/simplyblock_core/kv_store.py`

 * *Files 2% similar despite different names*

```diff
@@ -80,15 +80,14 @@
     def clear_prefix(self, prefix):
         self.kv_store.db.clear_range_startswith(prefix)
 
     def get_cluster_map(self):
         cmap = ClusterMap().read_from_db(self.kv_store)
         return cmap[0] if cmap else None
 
-    # todo: change this function for multi cluster
     def get_storage_nodes(self):
         ret = StorageNode().read_from_db(self.kv_store)
         ret = sorted(ret, key=lambda x: x.create_dt)
         return ret
 
     def get_storage_nodes_by_cluster_id(self, cluster_id):
         ret = StorageNode().read_from_db(self.kv_store)
@@ -167,17 +166,24 @@
 
     def get_pool_by_name(self, name):
         pools = Pool().read_from_db(self.kv_store)
         for pool in pools:
             if pool.pool_name == name:
                 return pool
 
-    def get_lvols(self):
-        ret = LVol().read_from_db(self.kv_store)
-        return ret
+    def get_lvols(self, cluster_id=None):
+        lvols = []
+        if cluster_id:
+            for pool in self.get_pools():
+                if pool.cluster_id == cluster_id:
+                    for lv_id in pool.lvols:
+                        lvols.append(self.get_lvol_by_id(lv_id))
+        else:
+            lvols = LVol().read_from_db(self.kv_store)
+        return lvols
 
     def get_snapshots(self):
         ret = SnapShot().read_from_db(self.kv_store)
         return ret
 
     def get_snapshot_by_id(self, id):
         ret = SnapShot().read_from_db(self.kv_store, id)
```

## Comparing `sbcli_mc-1.0.2/simplyblock_core/compute_node_ops.py` & `sbcli_mc-1.0.4/simplyblock_core/compute_node_ops.py`

 * *Files identical despite different names*

## Comparing `sbcli_mc-1.0.2/simplyblock_core/rpc_client.py` & `sbcli_mc-1.0.4/simplyblock_core/rpc_client.py`

 * *Files identical despite different names*

## Comparing `sbcli_mc-1.0.2/simplyblock_core/mgmt_node_ops.py` & `sbcli_mc-1.0.4/simplyblock_core/mgmt_node_ops.py`

 * *Files identical despite different names*

## Comparing `sbcli_mc-1.0.2/simplyblock_core/utils.py` & `sbcli_mc-1.0.4/simplyblock_core/utils.py`

 * *Files identical despite different names*

## Comparing `sbcli_mc-1.0.2/simplyblock_core/distr_controller.py` & `sbcli_mc-1.0.4/simplyblock_core/distr_controller.py`

 * *Files identical despite different names*

## Comparing `sbcli_mc-1.0.2/simplyblock_core/cnode_client.py` & `sbcli_mc-1.0.4/simplyblock_core/cnode_client.py`

 * *Files identical despite different names*

## Comparing `sbcli_mc-1.0.2/simplyblock_core/storage_node_ops.py` & `sbcli_mc-1.0.4/simplyblock_core/storage_node_ops.py`

 * *Files 0% similar despite different names*

```diff
@@ -752,15 +752,15 @@
 
     if snode.status != StorageNode.STATUS_REMOVED:
         logger.error(f"Node must be in removed status")
         return False
 
     snode.remove(db_controller.kv_store)
 
-    for lvol in db_controller.get_lvols():
+    for lvol in db_controller.get_lvols(snode.cluster_id):
         logger.info(f"Sending cluster map to LVol: {lvol.get_id()}")
         lvol_controller.send_cluster_map(lvol.get_id())
 
     storage_events.snode_delete(snode)
     logger.info("done")
```

## Comparing `sbcli_mc-1.0.2/simplyblock_core/constants.py` & `sbcli_mc-1.0.4/simplyblock_core/constants.py`

 * *Files identical despite different names*

## Comparing `sbcli_mc-1.0.2/simplyblock_core/services/job_tasks.py` & `sbcli_mc-1.0.4/simplyblock_core/services/job_tasks.py`

 * *Files identical despite different names*

## Comparing `sbcli_mc-1.0.2/simplyblock_core/services/caching_node_monitor.py` & `sbcli_mc-1.0.4/simplyblock_core/services/caching_node_monitor.py`

 * *Files identical despite different names*

## Comparing `sbcli_mc-1.0.2/simplyblock_core/services/install_service.sh` & `sbcli_mc-1.0.4/simplyblock_core/services/install_service.sh`

 * *Files identical despite different names*

## Comparing `sbcli_mc-1.0.2/simplyblock_core/services/__init__.py` & `sbcli_mc-1.0.4/simplyblock_core/services/__init__.py`

 * *Files identical despite different names*

## Comparing `sbcli_mc-1.0.2/simplyblock_core/services/log_agg_service.py` & `sbcli_mc-1.0.4/simplyblock_core/services/log_agg_service.py`

 * *Files identical despite different names*

## Comparing `sbcli_mc-1.0.2/simplyblock_core/services/health_check_service.py` & `sbcli_mc-1.0.4/simplyblock_core/services/health_check_service.py`

 * *Files identical despite different names*

## Comparing `sbcli_mc-1.0.2/simplyblock_core/services/capacity_and_stats_collector.py` & `sbcli_mc-1.0.4/simplyblock_core/services/capacity_and_stats_collector.py`

 * *Files identical despite different names*

## Comparing `sbcli_mc-1.0.2/simplyblock_core/services/device_monitor.py` & `sbcli_mc-1.0.4/simplyblock_core/services/device_monitor.py`

 * *Files identical despite different names*

## Comparing `sbcli_mc-1.0.2/simplyblock_core/services/lvol_stat_collector.py` & `sbcli_mc-1.0.4/simplyblock_core/services/lvol_stat_collector.py`

 * *Files 1% similar despite different names*

```diff
@@ -111,15 +111,15 @@
 db_controller = kv_store.DBController()
 
 
 logger.info("Starting stats collector...")
 while True:
 
     pools = db_controller.get_pools()
-    all_lvols = db_controller.get_lvols()
+    all_lvols = db_controller.get_lvols()  # pass
     for pool in pools:
         lvols = []
         for lvol in all_lvols:
             if lvol.pool_uuid == pool.get_id():
                 lvols.append(lvol)
 
         if not lvols:
```

## Comparing `sbcli_mc-1.0.2/simplyblock_core/services/cap_monitor.py` & `sbcli_mc-1.0.4/simplyblock_core/services/cap_monitor.py`

 * *Files identical despite different names*

## Comparing `sbcli_mc-1.0.2/simplyblock_core/services/storage_node_monitor.py` & `sbcli_mc-1.0.4/simplyblock_core/services/storage_node_monitor.py`

 * *Files identical despite different names*

## Comparing `sbcli_mc-1.0.2/simplyblock_core/services/port_stat_collector.py` & `sbcli_mc-1.0.4/simplyblock_core/services/port_stat_collector.py`

 * *Files identical despite different names*

## Comparing `sbcli_mc-1.0.2/simplyblock_core/services/distr_event_collector.py` & `sbcli_mc-1.0.4/simplyblock_core/services/distr_event_collector.py`

 * *Files 1% similar despite different names*

```diff
@@ -71,15 +71,15 @@
         event.status = 'processed'
 
 
 def process_lvol_event(event):
     if event.message in ["error_open", 'error_read', "error_write", "error_unmap"]:
         vuid = event.object_dict['vuid']
         lvol = None
-        for lv in db_controller.get_lvols():
+        for lv in db_controller.get_lvols():  # pass
             if lv.vuid == vuid:
                 lvol = lv
                 break
 
         if not lvol:
             logger.error(f"LVol with vuid {vuid} not found")
             event.status = 'lvol_not_found'
```

## Comparing `sbcli_mc-1.0.2/simplyblock_core/services/mgmt_node_monitor.py` & `sbcli_mc-1.0.4/simplyblock_core/services/mgmt_node_monitor.py`

 * *Files identical despite different names*

## Comparing `sbcli_mc-1.0.2/simplyblock_core/services/lvol_monitor.py` & `sbcli_mc-1.0.4/simplyblock_core/services/lvol_monitor.py`

 * *Files 2% similar despite different names*

```diff
@@ -45,15 +45,15 @@
 # get DB controller
 db_store = kv_store.KVStore()
 db_controller = kv_store.DBController()
 
 
 logger.info("Starting LVol monitor...")
 while True:
-    lvols = db_controller.get_lvols()
+    lvols = db_controller.get_lvols()  # pass
     if not lvols:
         logger.error("LVols list is empty")
 
     for lvol in lvols:
         if lvol.io_error:
             logger.debug(f"Skipping LVol health check because of io_error {lvol.get_id()}")
             continue
```

## Comparing `sbcli_mc-1.0.2/simplyblock_core/controllers/pool_controller.py` & `sbcli_mc-1.0.4/simplyblock_core/controllers/pool_controller.py`

 * *Files 1% similar despite different names*

```diff
@@ -30,22 +30,18 @@
         return False
 
     for p in db_controller.get_pools():
         if p.pool_name == name:
             logger.error(f"Pool found with the same name: {name}")
             return False
 
-    if cluster_id:
-        cluster = db_controller.get_cluster_by_id(cluster_id)
-        if not cluster:
-            logger.error(f"Cluster not found: {cluster_id}")
-            return False
-    else:
-        cluster = db_controller.get_clusters()[0]
-
+    cluster = db_controller.get_cluster_by_id(cluster_id)
+    if not cluster:
+        logger.error(f"Cluster not found: {cluster_id}")
+        return False
 
     pool_max = pool_max or 0
     lvol_max = lvol_max or 0
     max_rw_iops = max_rw_iops or 0
     max_rw_mbytes = max_rw_mbytes or 0
     max_r_mbytes = max_r_mbytes or 0
     max_w_mbytes = max_w_mbytes or 0
```

## Comparing `sbcli_mc-1.0.2/simplyblock_core/controllers/storage_events.py` & `sbcli_mc-1.0.4/simplyblock_core/controllers/storage_events.py`

 * *Files identical despite different names*

## Comparing `sbcli_mc-1.0.2/simplyblock_core/controllers/lvol_controller.py` & `sbcli_mc-1.0.4/simplyblock_core/controllers/lvol_controller.py`

 * *Files 2% similar despite different names*

```diff
@@ -121,15 +121,15 @@
 
     if pool.pool_max_size > 0:
         total = pool_controller.get_pool_total_capacity(pool.get_id())
         if total + size > pool.pool_max_size:
             return False, f"Invalid LVol size: {utils.humanbytes(size)} " \
                           f"Pool max size has reached {utils.humanbytes(total)} of {utils.humanbytes(pool.pool_max_size)}"
 
-    for lvol in db_controller.get_lvols():
+    for lvol in db_controller.get_lvols(pool.cluster_id):
         if lvol.pool_uuid == pool.get_id():
             if lvol.lvol_name == name:
                 return False, f"LVol name must be unique: {name}"
 
     if pool.has_qos():
         if pool.max_rw_ios_per_sec > 0:
             if max_rw_iops <= 0:
@@ -502,43 +502,43 @@
 
     if error:
         logger.error(error)
         return False, error
 
     cluster_size_prov = 0
     cluster_size_total = 0
-    for lvol in db_controller.get_lvols():
+    for lvol in db_controller.get_lvols(cl.get_id()):
         cluster_size_prov += lvol.size
 
     dev_count = 0
     snodes = db_controller.get_storage_nodes_by_cluster_id(cl.get_id())
     online_nodes = []
     for node in snodes:
         if node.status == node.STATUS_ONLINE:
             online_nodes.append(node)
             for dev in node.nvme_devices:
                 if dev.status == dev.STATUS_ONLINE:
                     dev_count += 1
                     cluster_size_total += dev.size
 
+    if len(online_nodes) == 0:
+        logger.error("No online Storage nodes found")
+        return False, "No online Storage nodes found"
+
     if dev_count == 0:
         logger.error("No NVMe devices found in the cluster")
         return False, "No NVMe devices found in the cluster"
     elif dev_count < 8:
         logger.warning("Number of active cluster devices are less than 8")
         # return False, "Number of active cluster devices are less than 8"
 
     if len(online_nodes) < 3 and ha_type == "ha":
         logger.error("Storage nodes are less than 3 in ha cluster")
         return False, "Storage nodes are less than 3 in ha cluster"
 
-    if len(online_nodes) == 0:
-        logger.error("No online Storage nodes found")
-        return False, "No online Storage nodes found"
-
     cluster_size_prov_util = int(((cluster_size_prov+size) / cluster_size_total) * 100)
 
     if cl.prov_cap_crit and cl.prov_cap_crit < cluster_size_prov_util:
         msg = f"Cluster provisioned cap critical would be, util: {cluster_size_prov_util}% of cluster util: {cl.prov_cap_crit}"
         logger.error(msg)
         return False, msg
 
@@ -1016,15 +1016,15 @@
     lvol.remove(db_controller.kv_store)
 
     # if lvol is clone and snapshot is deleted, then delete snapshot
     if lvol.cloned_from_snap:
         snap = db_controller.get_snapshot_by_id(lvol.cloned_from_snap)
         if snap.deleted is True:
             lvols_count = 0
-            for lvol in db_controller.get_lvols():
+            for lvol in db_controller.get_lvols():  # pass
                 if lvol.cloned_from_snap == snap.get_id():
                     lvols_count += 1
             if lvols_count == 0:
                 snapshot_controller.delete(snap.get_id())
 
     logger.info("Done")
     return True
@@ -1077,16 +1077,28 @@
     lvol.r_mbytes_per_sec = r_mbytes_per_sec
     lvol.w_mbytes_per_sec = w_mbytes_per_sec
     lvol.write_to_db(db_controller.kv_store)
     logger.info("Done")
     return True
 
 
-def list_lvols(is_json):
-    lvols = db_controller.get_lvols()
+def list_lvols(is_json, cluster_id, pool_id_or_name):
+    lvols = []
+    if cluster_id:
+        lvols = db_controller.get_lvols(cluster_id)
+    elif pool_id_or_name:
+        pool = db_controller.get_pool_by_id(pool_id_or_name)
+        if not pool:
+            pool = db_controller.get_pool_by_name(pool_id_or_name)
+            if pool:
+                for lv_id in pool.lvols:
+                    lvols.append(db_controller.get_lvol_by_id(lv_id))
+    else:
+        lvols = db_controller.get_lvols()
+
     data = []
     for lvol in lvols:
         if lvol.deleted is True:
             continue
         logger.debug(lvol)
         data.append({
             "Id": lvol.uuid,
@@ -1129,15 +1141,15 @@
             print(";".join([str(v) for v in d.values()]))
     else:
         return utils.print_table(data)
 
 
 def get_lvol(lvol_id_or_name, is_json):
     lvol = None
-    for lv in db_controller.get_lvols():
+    for lv in db_controller.get_lvols():  # pass
         if lv.get_id() == lvol_id_or_name or lv.lvol_name == lvol_id_or_name:
             lvol = lv
             break
 
     if not lvol:
         logger.error(f"LVol id or name not found: {lvol_id_or_name}")
         return False
```

## Comparing `sbcli_mc-1.0.2/simplyblock_core/controllers/device_events.py` & `sbcli_mc-1.0.4/simplyblock_core/controllers/device_events.py`

 * *Files identical despite different names*

## Comparing `sbcli_mc-1.0.2/simplyblock_core/controllers/lvol_events.py` & `sbcli_mc-1.0.4/simplyblock_core/controllers/lvol_events.py`

 * *Files identical despite different names*

## Comparing `sbcli_mc-1.0.2/simplyblock_core/controllers/snapshot_controller.py` & `sbcli_mc-1.0.4/simplyblock_core/controllers/snapshot_controller.py`

 * *Files 2% similar despite different names*

```diff
@@ -115,15 +115,20 @@
 
 def delete(snapshot_uuid):
     snap = db_controller.get_snapshot_by_id(snapshot_uuid)
     if not snap:
         logger.error(f"Snapshot not found {snapshot_uuid}")
         return False
 
-    for lvol in db_controller.get_lvols():
+    snode = db_controller.get_storage_node_by_id(snap.lvol.node_id)
+    if not snode:
+        logger.error(f"Storage node not found {snap.lvol.node_id}")
+        return False
+
+    for lvol in db_controller.get_lvols(snode.cluster_id):
         if lvol.cloned_from_snap and lvol.cloned_from_snap == snapshot_uuid:
             logger.warning(f"Soft delete snapshot with clones, lvol ID: {lvol.get_id()}")
             snap.deleted = True
             snap.write_to_db(db_controller.kv_store)
             return True
 
     logger.info(f"Removing snapshot: {snapshot_uuid}")
```

## Comparing `sbcli_mc-1.0.2/simplyblock_core/controllers/snapshot_events.py` & `sbcli_mc-1.0.4/simplyblock_core/controllers/snapshot_events.py`

 * *Files identical despite different names*

## Comparing `sbcli_mc-1.0.2/simplyblock_core/controllers/events_controller.py` & `sbcli_mc-1.0.4/simplyblock_core/controllers/events_controller.py`

 * *Files identical despite different names*

## Comparing `sbcli_mc-1.0.2/simplyblock_core/controllers/health_controller.py` & `sbcli_mc-1.0.4/simplyblock_core/controllers/health_controller.py`

 * *Files identical despite different names*

## Comparing `sbcli_mc-1.0.2/simplyblock_core/controllers/device_controller.py` & `sbcli_mc-1.0.4/simplyblock_core/controllers/device_controller.py`

 * *Files 2% similar despite different names*

```diff
@@ -299,15 +299,15 @@
         if not force:
             return False
 
     device.status = 'removed'
     snode.write_to_db(db_controller.kv_store)
     device_events.device_delete(device)
 
-    for lvol in db_controller.get_lvols():
+    for lvol in db_controller.get_lvols(snode.cluster_id):
         lvol_controller.send_cluster_map(lvol.get_id())
 
     return True
 
 
 def get_device(device_id):
     db_controller = DBController()
```

## Comparing `sbcli_mc-1.0.2/simplyblock_core/controllers/pool_events.py` & `sbcli_mc-1.0.4/simplyblock_core/controllers/pool_events.py`

 * *Files identical despite different names*

## Comparing `sbcli_mc-1.0.2/simplyblock_core/controllers/caching_node_controller.py` & `sbcli_mc-1.0.4/simplyblock_core/controllers/caching_node_controller.py`

 * *Files identical despite different names*

## Comparing `sbcli_mc-1.0.2/simplyblock_core/controllers/cluster_events.py` & `sbcli_mc-1.0.4/simplyblock_core/controllers/cluster_events.py`

 * *Files identical despite different names*

## Comparing `sbcli_mc-1.0.2/simplyblock_core/controllers/mgmt_events.py` & `sbcli_mc-1.0.4/simplyblock_core/controllers/mgmt_events.py`

 * *Files identical despite different names*

## Comparing `sbcli_mc-1.0.2/simplyblock_core/models/caching_node.py` & `sbcli_mc-1.0.4/simplyblock_core/models/caching_node.py`

 * *Files identical despite different names*

## Comparing `sbcli_mc-1.0.2/simplyblock_core/models/nvme_device.py` & `sbcli_mc-1.0.4/simplyblock_core/models/nvme_device.py`

 * *Files identical despite different names*

## Comparing `sbcli_mc-1.0.2/simplyblock_core/models/mgmt_node.py` & `sbcli_mc-1.0.4/simplyblock_core/models/mgmt_node.py`

 * *Files identical despite different names*

## Comparing `sbcli_mc-1.0.2/simplyblock_core/models/compute_node.py` & `sbcli_mc-1.0.4/simplyblock_core/models/compute_node.py`

 * *Files identical despite different names*

## Comparing `sbcli_mc-1.0.2/simplyblock_core/models/events.py` & `sbcli_mc-1.0.4/simplyblock_core/models/events.py`

 * *Files identical despite different names*

## Comparing `sbcli_mc-1.0.2/simplyblock_core/models/global_settings.py` & `sbcli_mc-1.0.4/simplyblock_core/models/global_settings.py`

 * *Files identical despite different names*

## Comparing `sbcli_mc-1.0.2/simplyblock_core/models/job_schedule.py` & `sbcli_mc-1.0.4/simplyblock_core/models/job_schedule.py`

 * *Files identical despite different names*

## Comparing `sbcli_mc-1.0.2/simplyblock_core/models/base_model.py` & `sbcli_mc-1.0.4/simplyblock_core/models/base_model.py`

 * *Files identical despite different names*

## Comparing `sbcli_mc-1.0.2/simplyblock_core/models/lvol_model.py` & `sbcli_mc-1.0.4/simplyblock_core/models/lvol_model.py`

 * *Files identical despite different names*

## Comparing `sbcli_mc-1.0.2/simplyblock_core/models/snapshot.py` & `sbcli_mc-1.0.4/simplyblock_core/models/snapshot.py`

 * *Files identical despite different names*

## Comparing `sbcli_mc-1.0.2/simplyblock_core/models/storage_node.py` & `sbcli_mc-1.0.4/simplyblock_core/models/storage_node.py`

 * *Files identical despite different names*

## Comparing `sbcli_mc-1.0.2/simplyblock_core/models/stats.py` & `sbcli_mc-1.0.4/simplyblock_core/models/stats.py`

 * *Files identical despite different names*

## Comparing `sbcli_mc-1.0.2/simplyblock_core/models/pool.py` & `sbcli_mc-1.0.4/simplyblock_core/models/pool.py`

 * *Files identical despite different names*

## Comparing `sbcli_mc-1.0.2/simplyblock_core/models/iface.py` & `sbcli_mc-1.0.4/simplyblock_core/models/iface.py`

 * *Files identical despite different names*

## Comparing `sbcli_mc-1.0.2/simplyblock_core/models/cluster.py` & `sbcli_mc-1.0.4/simplyblock_core/models/cluster.py`

 * *Files identical despite different names*

## Comparing `sbcli_mc-1.0.2/simplyblock_core/models/port_stat.py` & `sbcli_mc-1.0.4/simplyblock_core/models/port_stat.py`

 * *Files identical despite different names*

## Comparing `sbcli_mc-1.0.2/simplyblock_core/scripts/install_deps.sh` & `sbcli_mc-1.0.4/simplyblock_core/scripts/install_deps.sh`

 * *Files identical despite different names*

## Comparing `sbcli_mc-1.0.2/simplyblock_core/scripts/__init__.py` & `sbcli_mc-1.0.4/simplyblock_core/scripts/__init__.py`

 * *Files identical despite different names*

## Comparing `sbcli_mc-1.0.2/simplyblock_core/scripts/haproxy.cfg` & `sbcli_mc-1.0.4/simplyblock_core/scripts/haproxy.cfg`

 * *Files identical despite different names*

## Comparing `sbcli_mc-1.0.2/simplyblock_core/scripts/stack_deploy_wait.sh` & `sbcli_mc-1.0.4/simplyblock_core/scripts/stack_deploy_wait.sh`

 * *Files identical despite different names*

## Comparing `sbcli_mc-1.0.2/simplyblock_core/scripts/docker-compose-swarm.yml` & `sbcli_mc-1.0.4/simplyblock_core/scripts/docker-compose-swarm.yml`

 * *Files identical despite different names*

## Comparing `sbcli_mc-1.0.2/simplyblock_core/scripts/apply_dashboard.sh` & `sbcli_mc-1.0.4/simplyblock_core/scripts/apply_dashboard.sh`

 * *Files identical despite different names*

## Comparing `sbcli_mc-1.0.2/simplyblock_core/scripts/docker-compose-swarm-monitoring.yml` & `sbcli_mc-1.0.4/simplyblock_core/scripts/docker-compose-swarm-monitoring.yml`

 * *Files identical despite different names*

## Comparing `sbcli_mc-1.0.2/simplyblock_core/scripts/deploy_stack.sh` & `sbcli_mc-1.0.4/simplyblock_core/scripts/deploy_stack.sh`

 * *Files identical despite different names*

## Comparing `sbcli_mc-1.0.2/simplyblock_core/scripts/alerting/alert_rules.yaml` & `sbcli_mc-1.0.4/simplyblock_core/scripts/alerting/alert_rules.yaml`

 * *Files identical despite different names*

## Comparing `sbcli_mc-1.0.2/simplyblock_core/scripts/alerting/alert_resources.yaml` & `sbcli_mc-1.0.4/simplyblock_core/scripts/alerting/alert_resources.yaml`

 * *Files identical despite different names*

## Comparing `sbcli_mc-1.0.2/simplyblock_core/scripts/dashboards/nodes.json` & `sbcli_mc-1.0.4/simplyblock_core/scripts/dashboards/nodes.json`

 * *Files identical despite different names*

## Comparing `sbcli_mc-1.0.2/simplyblock_core/scripts/dashboards/cluster.json` & `sbcli_mc-1.0.4/simplyblock_core/scripts/dashboards/cluster.json`

 * *Files identical despite different names*

## Comparing `sbcli_mc-1.0.2/simplyblock_core/scripts/dashboards/lvols.json` & `sbcli_mc-1.0.4/simplyblock_core/scripts/dashboards/lvols.json`

 * *Files identical despite different names*

## Comparing `sbcli_mc-1.0.2/simplyblock_core/scripts/dashboards/devices.json` & `sbcli_mc-1.0.4/simplyblock_core/scripts/dashboards/devices.json`

 * *Files identical despite different names*

## Comparing `sbcli_mc-1.0.2/simplyblock_core/scripts/dashboards/pools.json` & `sbcli_mc-1.0.4/simplyblock_core/scripts/dashboards/pools.json`

 * *Files identical despite different names*

## Comparing `sbcli_mc-1.0.2/simplyblock_core/scripts/dashboards/node-exporter.json` & `sbcli_mc-1.0.4/simplyblock_core/scripts/dashboards/node-exporter.json`

 * *Files identical despite different names*

## Comparing `sbcli_mc-1.0.2/sbcli_mc.egg-info/SOURCES.txt` & `sbcli_mc-1.0.4/sbcli_mc.egg-info/SOURCES.txt`

 * *Files identical despite different names*

## Comparing `sbcli_mc-1.0.2/sbcli_mc.egg-info/PKG-INFO` & `sbcli_mc-1.0.4/sbcli_mc.egg-info/PKG-INFO`

 * *Files 5% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: sbcli-mc
-Version: 1.0.2
+Version: 1.0.4
 Summary: CLI for managing SimplyBlock cluster
 Home-page: https://www.simplyblock.io/
 Author: Hamdy
 Author-email: hamdy@simplyblock.io
 Description-Content-Type: text/markdown
 Requires-Dist: foundationdb
 Requires-Dist: requests
```

