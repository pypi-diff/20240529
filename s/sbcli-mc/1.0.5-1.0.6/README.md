# Comparing `tmp/sbcli_mc-1.0.5.zip` & `tmp/sbcli_mc-1.0.6.zip`

## zipinfo {}

```diff
@@ -1,150 +1,149 @@
-Zip file size: 212793 bytes, number of entries: 148
-drwxr-xr-x  2.0 unx        0 b- stor 24-May-29 03:49 sbcli_mc-1.0.5/
-drwxr-xr-x  2.0 unx        0 b- stor 24-May-29 03:49 sbcli_mc-1.0.5/simplyblock_cli/
-drwxr-xr-x  2.0 unx        0 b- stor 24-May-29 03:49 sbcli_mc-1.0.5/simplyblock_web/
-drwxr-xr-x  2.0 unx        0 b- stor 24-May-29 03:49 sbcli_mc-1.0.5/simplyblock_core/
-drwxr-xr-x  2.0 unx        0 b- stor 24-May-29 03:49 sbcli_mc-1.0.5/sbcli_mc.egg-info/
--rw-r--r--  2.0 unx     1068 b- defN 24-May-29 03:49 sbcli_mc-1.0.5/README.md
--rw-r--r--  2.0 unx       84 b- defN 24-May-29 03:49 sbcli_mc-1.0.5/pyproject.toml
--rw-r--r--  2.0 unx     1488 b- defN 24-May-29 03:49 sbcli_mc-1.0.5/PKG-INFO
--rw-r--r--  2.0 unx      157 b- defN 24-May-29 03:49 sbcli_mc-1.0.5/env_var
--rw-r--r--  2.0 unx       38 b- defN 24-May-29 03:49 sbcli_mc-1.0.5/setup.cfg
--rw-r--r--  2.0 unx     2269 b- defN 24-May-29 03:49 sbcli_mc-1.0.5/setup.py
--rw-r--r--  2.0 unx    64686 b- defN 24-May-29 03:49 sbcli_mc-1.0.5/simplyblock_cli/cli.py
--rw-r--r--  2.0 unx      357 b- defN 24-May-29 03:49 sbcli_mc-1.0.5/simplyblock_cli/main.py
-drwxr-xr-x  2.0 unx        0 b- stor 24-May-29 03:49 sbcli_mc-1.0.5/simplyblock_web/static/
-drwxr-xr-x  2.0 unx        0 b- stor 24-May-29 03:49 sbcli_mc-1.0.5/simplyblock_web/blueprints/
-drwxr-xr-x  2.0 unx        0 b- stor 24-May-29 03:49 sbcli_mc-1.0.5/simplyblock_web/templates/
--rw-r--r--  2.0 unx        0 b- defN 24-May-29 03:49 sbcli_mc-1.0.5/simplyblock_web/__init__.py
--rw-r--r--  2.0 unx     1434 b- defN 24-May-29 03:49 sbcli_mc-1.0.5/simplyblock_web/node_webapp.py
--rw-r--r--  2.0 unx      703 b- defN 24-May-29 03:49 sbcli_mc-1.0.5/simplyblock_web/snode_app.py
--rw-r--r--  2.0 unx      717 b- defN 24-May-29 03:49 sbcli_mc-1.0.5/simplyblock_web/caching_node_app.py
--rw-r--r--  2.0 unx     1638 b- defN 24-May-29 03:49 sbcli_mc-1.0.5/simplyblock_web/auth_middleware.py
--rw-r--r--  2.0 unx     5098 b- defN 24-May-29 03:49 sbcli_mc-1.0.5/simplyblock_web/node_utils.py
--rw-r--r--  2.0 unx     2715 b- defN 24-May-29 03:49 sbcli_mc-1.0.5/simplyblock_web/utils.py
--rw-r--r--  2.0 unx     1284 b- defN 24-May-29 03:49 sbcli_mc-1.0.5/simplyblock_web/app.py
--rw-r--r--  2.0 unx      725 b- defN 24-May-29 03:49 sbcli_mc-1.0.5/simplyblock_web/caching_node_app_k8s.py
--rw-r--r--  2.0 unx      322 b- defN 24-May-29 03:49 sbcli_mc-1.0.5/simplyblock_web/static/tst.py
--rw-r--r--  2.0 unx      827 b- defN 24-May-29 03:49 sbcli_mc-1.0.5/simplyblock_web/static/delete.py
--rw-r--r--  2.0 unx      507 b- defN 24-May-29 03:49 sbcli_mc-1.0.5/simplyblock_web/static/deploy_cnode.yaml
--rw-r--r--  2.0 unx      434 b- defN 24-May-29 03:49 sbcli_mc-1.0.5/simplyblock_web/static/is_up.py
--rw-r--r--  2.0 unx     1466 b- defN 24-May-29 03:49 sbcli_mc-1.0.5/simplyblock_web/static/deploy_spdk.yaml
--rw-r--r--  2.0 unx      463 b- defN 24-May-29 03:49 sbcli_mc-1.0.5/simplyblock_web/static/rpac.yaml
--rw-r--r--  2.0 unx      417 b- defN 24-May-29 03:49 sbcli_mc-1.0.5/simplyblock_web/static/list_deps.py
--rw-r--r--  2.0 unx     1302 b- defN 24-May-29 03:49 sbcli_mc-1.0.5/simplyblock_web/static/deploy.py
--rw-r--r--  2.0 unx     6806 b- defN 24-May-29 03:49 sbcli_mc-1.0.5/simplyblock_web/blueprints/web_api_pool.py
--rw-r--r--  2.0 unx        0 b- defN 24-May-29 03:49 sbcli_mc-1.0.5/simplyblock_web/blueprints/__init__.py
--rw-r--r--  2.0 unx     3118 b- defN 24-May-29 03:49 sbcli_mc-1.0.5/simplyblock_web/blueprints/web_api_device.py
--rw-r--r--  2.0 unx     8930 b- defN 24-May-29 03:49 sbcli_mc-1.0.5/simplyblock_web/blueprints/web_api_lvol.py
--rw-r--r--  2.0 unx     9713 b- defN 24-May-29 03:49 sbcli_mc-1.0.5/simplyblock_web/blueprints/snode_ops.py
--rw-r--r--  2.0 unx    12385 b- defN 24-May-29 03:49 sbcli_mc-1.0.5/simplyblock_web/blueprints/caching_node_ops.py
--rw-r--r--  2.0 unx     6401 b- defN 24-May-29 03:49 sbcli_mc-1.0.5/simplyblock_web/blueprints/web_api_storage_node.py
--rw-r--r--  2.0 unx     5931 b- defN 24-May-29 03:49 sbcli_mc-1.0.5/simplyblock_web/blueprints/web_api_cluster.py
--rw-r--r--  2.0 unx     8075 b- defN 24-May-29 03:49 sbcli_mc-1.0.5/simplyblock_web/blueprints/caching_node_ops_k8s.py
--rw-r--r--  2.0 unx     4883 b- defN 24-May-29 03:49 sbcli_mc-1.0.5/simplyblock_web/blueprints/node_api_caching_ks.py
--rw-r--r--  2.0 unx     5746 b- defN 24-May-29 03:49 sbcli_mc-1.0.5/simplyblock_web/blueprints/node_api_caching_docker.py
--rw-r--r--  2.0 unx     5491 b- defN 24-May-29 03:49 sbcli_mc-1.0.5/simplyblock_web/blueprints/web_api_caching_node.py
--rw-r--r--  2.0 unx     3103 b- defN 24-May-29 03:49 sbcli_mc-1.0.5/simplyblock_web/blueprints/node_api_basic.py
--rw-r--r--  2.0 unx    11244 b- defN 24-May-29 03:49 sbcli_mc-1.0.5/simplyblock_web/blueprints/csi.py
--rw-r--r--  2.0 unx      975 b- defN 24-May-29 03:49 sbcli_mc-1.0.5/simplyblock_web/blueprints/web_api_mgmt_node.py
--rw-r--r--  2.0 unx     2905 b- defN 24-May-29 03:49 sbcli_mc-1.0.5/simplyblock_web/templates/deploy_spdk.yaml.j2
-drwxr-xr-x  2.0 unx        0 b- stor 24-May-29 03:49 sbcli_mc-1.0.5/simplyblock_core/services/
-drwxr-xr-x  2.0 unx        0 b- stor 24-May-29 03:49 sbcli_mc-1.0.5/simplyblock_core/controllers/
-drwxr-xr-x  2.0 unx        0 b- stor 24-May-29 03:49 sbcli_mc-1.0.5/simplyblock_core/models/
-drwxr-xr-x  2.0 unx        0 b- stor 24-May-29 03:49 sbcli_mc-1.0.5/simplyblock_core/scripts/
--rw-r--r--  2.0 unx    26004 b- defN 24-May-29 03:49 sbcli_mc-1.0.5/simplyblock_core/cluster_ops.py
--rw-r--r--  2.0 unx      938 b- defN 24-May-29 03:49 sbcli_mc-1.0.5/simplyblock_core/pci_utils.py
--rw-r--r--  2.0 unx        0 b- defN 24-May-29 03:49 sbcli_mc-1.0.5/simplyblock_core/__init__.py
--rw-r--r--  2.0 unx     3193 b- defN 24-May-29 03:49 sbcli_mc-1.0.5/simplyblock_core/snode_client.py
--rw-r--r--  2.0 unx     9031 b- defN 24-May-29 03:49 sbcli_mc-1.0.5/simplyblock_core/kv_store.py
--rw-r--r--  2.0 unx     5112 b- defN 24-May-29 03:49 sbcli_mc-1.0.5/simplyblock_core/compute_node_ops.py
--rw-r--r--  2.0 unx    20829 b- defN 24-May-29 03:49 sbcli_mc-1.0.5/simplyblock_core/rpc_client.py
--rw-r--r--  2.0 unx     1986 b- defN 24-May-29 03:49 sbcli_mc-1.0.5/simplyblock_core/mgmt_node_ops.py
--rw-r--r--  2.0 unx     7640 b- defN 24-May-29 03:49 sbcli_mc-1.0.5/simplyblock_core/utils.py
--rw-r--r--  2.0 unx     7725 b- defN 24-May-29 03:49 sbcli_mc-1.0.5/simplyblock_core/distr_controller.py
--rw-r--r--  2.0 unx      279 b- defN 24-May-29 03:49 sbcli_mc-1.0.5/simplyblock_core/shell_utils.py
--rw-r--r--  2.0 unx     3638 b- defN 24-May-29 03:49 sbcli_mc-1.0.5/simplyblock_core/cnode_client.py
--rw-r--r--  2.0 unx    65258 b- defN 24-May-29 03:49 sbcli_mc-1.0.5/simplyblock_core/storage_node_ops.py
--rw-r--r--  2.0 unx     1575 b- defN 24-May-29 03:49 sbcli_mc-1.0.5/simplyblock_core/constants.py
--rw-r--r--  2.0 unx     3542 b- defN 24-May-29 03:49 sbcli_mc-1.0.5/simplyblock_core/services/job_tasks.py
--rw-r--r--  2.0 unx     3203 b- defN 24-May-29 03:49 sbcli_mc-1.0.5/simplyblock_core/services/caching_node_monitor.py
--rw-r--r--  2.0 unx      229 b- defN 24-May-29 03:49 sbcli_mc-1.0.5/simplyblock_core/services/service_template.service
--rw-r--r--  2.0 unx      837 b- defN 24-May-29 03:49 sbcli_mc-1.0.5/simplyblock_core/services/install_service.sh
--rw-r--r--  2.0 unx     4118 b- defN 24-May-29 03:49 sbcli_mc-1.0.5/simplyblock_core/services/__init__.py
--rw-r--r--  2.0 unx     2410 b- defN 24-May-29 03:49 sbcli_mc-1.0.5/simplyblock_core/services/log_agg_service.py
--rw-r--r--  2.0 unx     5751 b- defN 24-May-29 03:49 sbcli_mc-1.0.5/simplyblock_core/services/health_check_service.py
--rw-r--r--  2.0 unx     7439 b- defN 24-May-29 03:49 sbcli_mc-1.0.5/simplyblock_core/services/capacity_and_stats_collector.py
--rw-r--r--  2.0 unx     3169 b- defN 24-May-29 03:49 sbcli_mc-1.0.5/simplyblock_core/services/device_monitor.py
--rw-r--r--  2.0 unx     5276 b- defN 24-May-29 03:49 sbcli_mc-1.0.5/simplyblock_core/services/lvol_stat_collector.py
--rw-r--r--  2.0 unx     2671 b- defN 24-May-29 03:49 sbcli_mc-1.0.5/simplyblock_core/services/cap_monitor.py
--rw-r--r--  2.0 unx     6822 b- defN 24-May-29 03:49 sbcli_mc-1.0.5/simplyblock_core/services/storage_node_monitor.py
--rw-r--r--  2.0 unx     2428 b- defN 24-May-29 03:49 sbcli_mc-1.0.5/simplyblock_core/services/port_stat_collector.py
--rw-r--r--  2.0 unx     5154 b- defN 24-May-29 03:49 sbcli_mc-1.0.5/simplyblock_core/services/distr_event_collector.py
--rw-r--r--  2.0 unx      173 b- defN 24-May-29 03:49 sbcli_mc-1.0.5/simplyblock_core/services/remove_service.sh
--rw-r--r--  2.0 unx     3003 b- defN 24-May-29 03:49 sbcli_mc-1.0.5/simplyblock_core/services/mgmt_node_monitor.py
--rw-r--r--  2.0 unx     2197 b- defN 24-May-29 03:49 sbcli_mc-1.0.5/simplyblock_core/services/lvol_monitor.py
--rw-r--r--  2.0 unx    10498 b- defN 24-May-29 03:49 sbcli_mc-1.0.5/simplyblock_core/controllers/pool_controller.py
--rw-r--r--  2.0 unx        0 b- defN 24-May-29 03:49 sbcli_mc-1.0.5/simplyblock_core/controllers/__init__.py
--rw-r--r--  2.0 unx     1521 b- defN 24-May-29 03:49 sbcli_mc-1.0.5/simplyblock_core/controllers/storage_events.py
--rw-r--r--  2.0 unx    49039 b- defN 24-May-29 03:49 sbcli_mc-1.0.5/simplyblock_core/controllers/lvol_controller.py
--rw-r--r--  2.0 unx     1568 b- defN 24-May-29 03:49 sbcli_mc-1.0.5/simplyblock_core/controllers/device_events.py
--rw-r--r--  2.0 unx     1630 b- defN 24-May-29 03:49 sbcli_mc-1.0.5/simplyblock_core/controllers/lvol_events.py
--rw-r--r--  2.0 unx    11066 b- defN 24-May-29 03:49 sbcli_mc-1.0.5/simplyblock_core/controllers/snapshot_controller.py
--rw-r--r--  2.0 unx     1122 b- defN 24-May-29 03:49 sbcli_mc-1.0.5/simplyblock_core/controllers/snapshot_events.py
--rw-r--r--  2.0 unx     3191 b- defN 24-May-29 03:49 sbcli_mc-1.0.5/simplyblock_core/controllers/events_controller.py
--rw-r--r--  2.0 unx    10852 b- defN 24-May-29 03:49 sbcli_mc-1.0.5/simplyblock_core/controllers/health_controller.py
--rw-r--r--  2.0 unx    13948 b- defN 24-May-29 03:49 sbcli_mc-1.0.5/simplyblock_core/controllers/device_controller.py
--rw-r--r--  2.0 unx      695 b- defN 24-May-29 03:49 sbcli_mc-1.0.5/simplyblock_core/controllers/pool_events.py
--rw-r--r--  2.0 unx    23440 b- defN 24-May-29 03:49 sbcli_mc-1.0.5/simplyblock_core/controllers/caching_node_controller.py
--rw-r--r--  2.0 unx     1900 b- defN 24-May-29 03:49 sbcli_mc-1.0.5/simplyblock_core/controllers/cluster_events.py
--rw-r--r--  2.0 unx     1120 b- defN 24-May-29 03:49 sbcli_mc-1.0.5/simplyblock_core/controllers/mgmt_events.py
--rw-r--r--  2.0 unx     3766 b- defN 24-May-29 03:49 sbcli_mc-1.0.5/simplyblock_core/models/caching_node.py
--rw-r--r--  2.0 unx     2094 b- defN 24-May-29 03:49 sbcli_mc-1.0.5/simplyblock_core/models/nvme_device.py
--rw-r--r--  2.0 unx     1452 b- defN 24-May-29 03:49 sbcli_mc-1.0.5/simplyblock_core/models/mgmt_node.py
--rw-r--r--  2.0 unx      917 b- defN 24-May-29 03:49 sbcli_mc-1.0.5/simplyblock_core/models/compute_node.py
--rw-r--r--  2.0 unx        0 b- defN 24-May-29 03:49 sbcli_mc-1.0.5/simplyblock_core/models/__init__.py
--rw-r--r--  2.0 unx     1500 b- defN 24-May-29 03:49 sbcli_mc-1.0.5/simplyblock_core/models/events.py
--rw-r--r--  2.0 unx     1228 b- defN 24-May-29 03:49 sbcli_mc-1.0.5/simplyblock_core/models/global_settings.py
--rw-r--r--  2.0 unx      973 b- defN 24-May-29 03:49 sbcli_mc-1.0.5/simplyblock_core/models/job_schedule.py
--rw-r--r--  2.0 unx     4846 b- defN 24-May-29 03:49 sbcli_mc-1.0.5/simplyblock_core/models/base_model.py
--rw-r--r--  2.0 unx     2579 b- defN 24-May-29 03:49 sbcli_mc-1.0.5/simplyblock_core/models/lvol_model.py
--rw-r--r--  2.0 unx      736 b- defN 24-May-29 03:49 sbcli_mc-1.0.5/simplyblock_core/models/snapshot.py
--rw-r--r--  2.0 unx     3696 b- defN 24-May-29 03:49 sbcli_mc-1.0.5/simplyblock_core/models/storage_node.py
--rw-r--r--  2.0 unx     4242 b- defN 24-May-29 03:49 sbcli_mc-1.0.5/simplyblock_core/models/stats.py
--rw-r--r--  2.0 unx     1602 b- defN 24-May-29 03:49 sbcli_mc-1.0.5/simplyblock_core/models/pool.py
--rw-r--r--  2.0 unx      806 b- defN 24-May-29 03:49 sbcli_mc-1.0.5/simplyblock_core/models/iface.py
--rw-r--r--  2.0 unx     2565 b- defN 24-May-29 03:49 sbcli_mc-1.0.5/simplyblock_core/models/cluster.py
--rw-r--r--  2.0 unx     1020 b- defN 24-May-29 03:49 sbcli_mc-1.0.5/simplyblock_core/models/port_stat.py
-drwxr-xr-x  2.0 unx        0 b- stor 24-May-29 03:49 sbcli_mc-1.0.5/simplyblock_core/scripts/alerting/
-drwxr-xr-x  2.0 unx        0 b- stor 24-May-29 03:49 sbcli_mc-1.0.5/simplyblock_core/scripts/dashboards/
--rw-r--r--  2.0 unx     1420 b- defN 24-May-29 03:49 sbcli_mc-1.0.5/simplyblock_core/scripts/install_deps.sh
--rw-r--r--  2.0 unx     1782 b- defN 24-May-29 03:49 sbcli_mc-1.0.5/simplyblock_core/scripts/__init__.py
--rw-r--r--  2.0 unx       43 b- defN 24-May-29 03:49 sbcli_mc-1.0.5/simplyblock_core/scripts/run_ssh.sh
--rw-r--r--  2.0 unx     1163 b- defN 24-May-29 03:49 sbcli_mc-1.0.5/simplyblock_core/scripts/haproxy.cfg
--rw-r--r--  2.0 unx      118 b- defN 24-May-29 03:49 sbcli_mc-1.0.5/simplyblock_core/scripts/db_config_double.sh
--rw-r--r--  2.0 unx     5305 b- defN 24-May-29 03:49 sbcli_mc-1.0.5/simplyblock_core/scripts/stack_deploy_wait.sh
--rw-r--r--  2.0 unx      360 b- defN 24-May-29 03:49 sbcli_mc-1.0.5/simplyblock_core/scripts/datasource.yml
--rw-r--r--  2.0 unx     5611 b- defN 24-May-29 03:49 sbcli_mc-1.0.5/simplyblock_core/scripts/docker-compose-swarm.yml
--rw-r--r--  2.0 unx      152 b- defN 24-May-29 03:49 sbcli_mc-1.0.5/simplyblock_core/scripts/set_db_config.sh
--rwxr-xr-x  2.0 unx      657 b- defN 24-May-29 03:49 sbcli_mc-1.0.5/simplyblock_core/scripts/apply_dashboard.sh
--rw-r--r--  2.0 unx      311 b- defN 24-May-29 03:49 sbcli_mc-1.0.5/simplyblock_core/scripts/prometheus.yml
--rw-r--r--  2.0 unx      311 b- defN 24-May-29 03:49 sbcli_mc-1.0.5/simplyblock_core/scripts/clean_local_storage_deploy.sh
--rw-r--r--  2.0 unx     4409 b- defN 24-May-29 03:49 sbcli_mc-1.0.5/simplyblock_core/scripts/docker-compose-swarm-monitoring.yml
--rw-r--r--  2.0 unx      930 b- defN 24-May-29 03:49 sbcli_mc-1.0.5/simplyblock_core/scripts/deploy_stack.sh
--rw-r--r--  2.0 unx       54 b- defN 24-May-29 03:49 sbcli_mc-1.0.5/simplyblock_core/scripts/db_config_single.sh
--rw-r--r--  2.0 unx      453 b- defN 24-May-29 03:49 sbcli_mc-1.0.5/simplyblock_core/scripts/config_docker.sh
--rw-r--r--  2.0 unx    25433 b- defN 24-May-29 03:49 sbcli_mc-1.0.5/simplyblock_core/scripts/alerting/alert_rules.yaml
--rw-r--r--  2.0 unx     1856 b- defN 24-May-29 03:49 sbcli_mc-1.0.5/simplyblock_core/scripts/alerting/alert_resources.yaml
--rw-r--r--  2.0 unx    88820 b- defN 24-May-29 03:49 sbcli_mc-1.0.5/simplyblock_core/scripts/dashboards/nodes.json
--rw-r--r--  2.0 unx    88911 b- defN 24-May-29 03:49 sbcli_mc-1.0.5/simplyblock_core/scripts/dashboards/cluster.json
--rw-r--r--  2.0 unx    88776 b- defN 24-May-29 03:49 sbcli_mc-1.0.5/simplyblock_core/scripts/dashboards/lvols.json
--rw-r--r--  2.0 unx    88868 b- defN 24-May-29 03:49 sbcli_mc-1.0.5/simplyblock_core/scripts/dashboards/devices.json
--rw-r--r--  2.0 unx    99707 b- defN 24-May-29 03:49 sbcli_mc-1.0.5/simplyblock_core/scripts/dashboards/pools.json
--rw-r--r--  2.0 unx   799409 b- defN 24-May-29 03:49 sbcli_mc-1.0.5/simplyblock_core/scripts/dashboards/node-exporter.json
--rw-r--r--  2.0 unx     5261 b- defN 24-May-29 03:49 sbcli_mc-1.0.5/sbcli_mc.egg-info/SOURCES.txt
--rw-r--r--  2.0 unx       73 b- defN 24-May-29 03:49 sbcli_mc-1.0.5/sbcli_mc.egg-info/requires.txt
--rw-r--r--  2.0 unx     1488 b- defN 24-May-29 03:49 sbcli_mc-1.0.5/sbcli_mc.egg-info/PKG-INFO
--rw-r--r--  2.0 unx       49 b- defN 24-May-29 03:49 sbcli_mc-1.0.5/sbcli_mc.egg-info/top_level.txt
--rw-r--r--  2.0 unx       54 b- defN 24-May-29 03:49 sbcli_mc-1.0.5/sbcli_mc.egg-info/entry_points.txt
--rw-r--r--  2.0 unx        1 b- defN 24-May-29 03:49 sbcli_mc-1.0.5/sbcli_mc.egg-info/dependency_links.txt
-148 files, 1874932 bytes uncompressed, 186155 bytes compressed:  90.1%
+Zip file size: 212508 bytes, number of entries: 147
+drwxr-xr-x  2.0 unx        0 b- stor 24-May-29 16:34 sbcli_mc-1.0.6/
+drwxr-xr-x  2.0 unx        0 b- stor 24-May-29 16:34 sbcli_mc-1.0.6/simplyblock_cli/
+drwxr-xr-x  2.0 unx        0 b- stor 24-May-29 16:34 sbcli_mc-1.0.6/simplyblock_web/
+drwxr-xr-x  2.0 unx        0 b- stor 24-May-29 16:34 sbcli_mc-1.0.6/simplyblock_core/
+drwxr-xr-x  2.0 unx        0 b- stor 24-May-29 16:34 sbcli_mc-1.0.6/sbcli_mc.egg-info/
+-rw-r--r--  2.0 unx     1068 b- defN 24-May-29 16:34 sbcli_mc-1.0.6/README.md
+-rw-r--r--  2.0 unx       84 b- defN 24-May-29 16:34 sbcli_mc-1.0.6/pyproject.toml
+-rw-r--r--  2.0 unx     1488 b- defN 24-May-29 16:34 sbcli_mc-1.0.6/PKG-INFO
+-rw-r--r--  2.0 unx      157 b- defN 24-May-29 16:34 sbcli_mc-1.0.6/env_var
+-rw-r--r--  2.0 unx       38 b- defN 24-May-29 16:34 sbcli_mc-1.0.6/setup.cfg
+-rw-r--r--  2.0 unx     2269 b- defN 24-May-29 16:34 sbcli_mc-1.0.6/setup.py
+-rw-r--r--  2.0 unx    64686 b- defN 24-May-29 16:34 sbcli_mc-1.0.6/simplyblock_cli/cli.py
+-rw-r--r--  2.0 unx      357 b- defN 24-May-29 16:34 sbcli_mc-1.0.6/simplyblock_cli/main.py
+drwxr-xr-x  2.0 unx        0 b- stor 24-May-29 16:34 sbcli_mc-1.0.6/simplyblock_web/static/
+drwxr-xr-x  2.0 unx        0 b- stor 24-May-29 16:34 sbcli_mc-1.0.6/simplyblock_web/blueprints/
+drwxr-xr-x  2.0 unx        0 b- stor 24-May-29 16:34 sbcli_mc-1.0.6/simplyblock_web/templates/
+-rw-r--r--  2.0 unx        0 b- defN 24-May-29 16:34 sbcli_mc-1.0.6/simplyblock_web/__init__.py
+-rw-r--r--  2.0 unx     1434 b- defN 24-May-29 16:34 sbcli_mc-1.0.6/simplyblock_web/node_webapp.py
+-rw-r--r--  2.0 unx      703 b- defN 24-May-29 16:34 sbcli_mc-1.0.6/simplyblock_web/snode_app.py
+-rw-r--r--  2.0 unx      717 b- defN 24-May-29 16:34 sbcli_mc-1.0.6/simplyblock_web/caching_node_app.py
+-rw-r--r--  2.0 unx     1638 b- defN 24-May-29 16:34 sbcli_mc-1.0.6/simplyblock_web/auth_middleware.py
+-rw-r--r--  2.0 unx     5098 b- defN 24-May-29 16:34 sbcli_mc-1.0.6/simplyblock_web/node_utils.py
+-rw-r--r--  2.0 unx     2715 b- defN 24-May-29 16:34 sbcli_mc-1.0.6/simplyblock_web/utils.py
+-rw-r--r--  2.0 unx     1284 b- defN 24-May-29 16:34 sbcli_mc-1.0.6/simplyblock_web/app.py
+-rw-r--r--  2.0 unx      725 b- defN 24-May-29 16:34 sbcli_mc-1.0.6/simplyblock_web/caching_node_app_k8s.py
+-rw-r--r--  2.0 unx      322 b- defN 24-May-29 16:34 sbcli_mc-1.0.6/simplyblock_web/static/tst.py
+-rw-r--r--  2.0 unx      827 b- defN 24-May-29 16:34 sbcli_mc-1.0.6/simplyblock_web/static/delete.py
+-rw-r--r--  2.0 unx      507 b- defN 24-May-29 16:34 sbcli_mc-1.0.6/simplyblock_web/static/deploy_cnode.yaml
+-rw-r--r--  2.0 unx      434 b- defN 24-May-29 16:34 sbcli_mc-1.0.6/simplyblock_web/static/is_up.py
+-rw-r--r--  2.0 unx     1466 b- defN 24-May-29 16:34 sbcli_mc-1.0.6/simplyblock_web/static/deploy_spdk.yaml
+-rw-r--r--  2.0 unx      463 b- defN 24-May-29 16:34 sbcli_mc-1.0.6/simplyblock_web/static/rpac.yaml
+-rw-r--r--  2.0 unx      417 b- defN 24-May-29 16:34 sbcli_mc-1.0.6/simplyblock_web/static/list_deps.py
+-rw-r--r--  2.0 unx     1302 b- defN 24-May-29 16:34 sbcli_mc-1.0.6/simplyblock_web/static/deploy.py
+-rw-r--r--  2.0 unx     6806 b- defN 24-May-29 16:34 sbcli_mc-1.0.6/simplyblock_web/blueprints/web_api_pool.py
+-rw-r--r--  2.0 unx        0 b- defN 24-May-29 16:34 sbcli_mc-1.0.6/simplyblock_web/blueprints/__init__.py
+-rw-r--r--  2.0 unx     3118 b- defN 24-May-29 16:34 sbcli_mc-1.0.6/simplyblock_web/blueprints/web_api_device.py
+-rw-r--r--  2.0 unx     8930 b- defN 24-May-29 16:34 sbcli_mc-1.0.6/simplyblock_web/blueprints/web_api_lvol.py
+-rw-r--r--  2.0 unx     9713 b- defN 24-May-29 16:34 sbcli_mc-1.0.6/simplyblock_web/blueprints/snode_ops.py
+-rw-r--r--  2.0 unx    12385 b- defN 24-May-29 16:34 sbcli_mc-1.0.6/simplyblock_web/blueprints/caching_node_ops.py
+-rw-r--r--  2.0 unx     6401 b- defN 24-May-29 16:34 sbcli_mc-1.0.6/simplyblock_web/blueprints/web_api_storage_node.py
+-rw-r--r--  2.0 unx     4896 b- defN 24-May-29 16:34 sbcli_mc-1.0.6/simplyblock_web/blueprints/web_api_cluster.py
+-rw-r--r--  2.0 unx     8075 b- defN 24-May-29 16:34 sbcli_mc-1.0.6/simplyblock_web/blueprints/caching_node_ops_k8s.py
+-rw-r--r--  2.0 unx     4883 b- defN 24-May-29 16:34 sbcli_mc-1.0.6/simplyblock_web/blueprints/node_api_caching_ks.py
+-rw-r--r--  2.0 unx     5746 b- defN 24-May-29 16:34 sbcli_mc-1.0.6/simplyblock_web/blueprints/node_api_caching_docker.py
+-rw-r--r--  2.0 unx     5491 b- defN 24-May-29 16:34 sbcli_mc-1.0.6/simplyblock_web/blueprints/web_api_caching_node.py
+-rw-r--r--  2.0 unx     3103 b- defN 24-May-29 16:34 sbcli_mc-1.0.6/simplyblock_web/blueprints/node_api_basic.py
+-rw-r--r--  2.0 unx    11244 b- defN 24-May-29 16:34 sbcli_mc-1.0.6/simplyblock_web/blueprints/csi.py
+-rw-r--r--  2.0 unx      975 b- defN 24-May-29 16:34 sbcli_mc-1.0.6/simplyblock_web/blueprints/web_api_mgmt_node.py
+-rw-r--r--  2.0 unx     2905 b- defN 24-May-29 16:34 sbcli_mc-1.0.6/simplyblock_web/templates/deploy_spdk.yaml.j2
+drwxr-xr-x  2.0 unx        0 b- stor 24-May-29 16:34 sbcli_mc-1.0.6/simplyblock_core/services/
+drwxr-xr-x  2.0 unx        0 b- stor 24-May-29 16:34 sbcli_mc-1.0.6/simplyblock_core/controllers/
+drwxr-xr-x  2.0 unx        0 b- stor 24-May-29 16:34 sbcli_mc-1.0.6/simplyblock_core/models/
+drwxr-xr-x  2.0 unx        0 b- stor 24-May-29 16:34 sbcli_mc-1.0.6/simplyblock_core/scripts/
+-rw-r--r--  2.0 unx    26898 b- defN 24-May-29 16:34 sbcli_mc-1.0.6/simplyblock_core/cluster_ops.py
+-rw-r--r--  2.0 unx      938 b- defN 24-May-29 16:34 sbcli_mc-1.0.6/simplyblock_core/pci_utils.py
+-rw-r--r--  2.0 unx        0 b- defN 24-May-29 16:34 sbcli_mc-1.0.6/simplyblock_core/__init__.py
+-rw-r--r--  2.0 unx     3193 b- defN 24-May-29 16:34 sbcli_mc-1.0.6/simplyblock_core/snode_client.py
+-rw-r--r--  2.0 unx     9031 b- defN 24-May-29 16:34 sbcli_mc-1.0.6/simplyblock_core/kv_store.py
+-rw-r--r--  2.0 unx     5112 b- defN 24-May-29 16:34 sbcli_mc-1.0.6/simplyblock_core/compute_node_ops.py
+-rw-r--r--  2.0 unx    20829 b- defN 24-May-29 16:34 sbcli_mc-1.0.6/simplyblock_core/rpc_client.py
+-rw-r--r--  2.0 unx     1986 b- defN 24-May-29 16:34 sbcli_mc-1.0.6/simplyblock_core/mgmt_node_ops.py
+-rw-r--r--  2.0 unx     7640 b- defN 24-May-29 16:34 sbcli_mc-1.0.6/simplyblock_core/utils.py
+-rw-r--r--  2.0 unx     7725 b- defN 24-May-29 16:34 sbcli_mc-1.0.6/simplyblock_core/distr_controller.py
+-rw-r--r--  2.0 unx      279 b- defN 24-May-29 16:34 sbcli_mc-1.0.6/simplyblock_core/shell_utils.py
+-rw-r--r--  2.0 unx     3638 b- defN 24-May-29 16:34 sbcli_mc-1.0.6/simplyblock_core/cnode_client.py
+-rw-r--r--  2.0 unx    65258 b- defN 24-May-29 16:34 sbcli_mc-1.0.6/simplyblock_core/storage_node_ops.py
+-rw-r--r--  2.0 unx     1499 b- defN 24-May-29 16:34 sbcli_mc-1.0.6/simplyblock_core/constants.py
+-rw-r--r--  2.0 unx     3542 b- defN 24-May-29 16:34 sbcli_mc-1.0.6/simplyblock_core/services/job_tasks.py
+-rw-r--r--  2.0 unx     3203 b- defN 24-May-29 16:34 sbcli_mc-1.0.6/simplyblock_core/services/caching_node_monitor.py
+-rw-r--r--  2.0 unx      229 b- defN 24-May-29 16:34 sbcli_mc-1.0.6/simplyblock_core/services/service_template.service
+-rw-r--r--  2.0 unx      837 b- defN 24-May-29 16:34 sbcli_mc-1.0.6/simplyblock_core/services/install_service.sh
+-rw-r--r--  2.0 unx     4118 b- defN 24-May-29 16:34 sbcli_mc-1.0.6/simplyblock_core/services/__init__.py
+-rw-r--r--  2.0 unx     2410 b- defN 24-May-29 16:34 sbcli_mc-1.0.6/simplyblock_core/services/log_agg_service.py
+-rw-r--r--  2.0 unx     5751 b- defN 24-May-29 16:34 sbcli_mc-1.0.6/simplyblock_core/services/health_check_service.py
+-rw-r--r--  2.0 unx     7439 b- defN 24-May-29 16:34 sbcli_mc-1.0.6/simplyblock_core/services/capacity_and_stats_collector.py
+-rw-r--r--  2.0 unx     3169 b- defN 24-May-29 16:34 sbcli_mc-1.0.6/simplyblock_core/services/device_monitor.py
+-rw-r--r--  2.0 unx     5276 b- defN 24-May-29 16:34 sbcli_mc-1.0.6/simplyblock_core/services/lvol_stat_collector.py
+-rw-r--r--  2.0 unx     2671 b- defN 24-May-29 16:34 sbcli_mc-1.0.6/simplyblock_core/services/cap_monitor.py
+-rw-r--r--  2.0 unx     6822 b- defN 24-May-29 16:34 sbcli_mc-1.0.6/simplyblock_core/services/storage_node_monitor.py
+-rw-r--r--  2.0 unx     2428 b- defN 24-May-29 16:34 sbcli_mc-1.0.6/simplyblock_core/services/port_stat_collector.py
+-rw-r--r--  2.0 unx     5154 b- defN 24-May-29 16:34 sbcli_mc-1.0.6/simplyblock_core/services/distr_event_collector.py
+-rw-r--r--  2.0 unx      173 b- defN 24-May-29 16:34 sbcli_mc-1.0.6/simplyblock_core/services/remove_service.sh
+-rw-r--r--  2.0 unx     3003 b- defN 24-May-29 16:34 sbcli_mc-1.0.6/simplyblock_core/services/mgmt_node_monitor.py
+-rw-r--r--  2.0 unx     2197 b- defN 24-May-29 16:34 sbcli_mc-1.0.6/simplyblock_core/services/lvol_monitor.py
+-rw-r--r--  2.0 unx    10498 b- defN 24-May-29 16:34 sbcli_mc-1.0.6/simplyblock_core/controllers/pool_controller.py
+-rw-r--r--  2.0 unx        0 b- defN 24-May-29 16:34 sbcli_mc-1.0.6/simplyblock_core/controllers/__init__.py
+-rw-r--r--  2.0 unx     1521 b- defN 24-May-29 16:34 sbcli_mc-1.0.6/simplyblock_core/controllers/storage_events.py
+-rw-r--r--  2.0 unx    49039 b- defN 24-May-29 16:34 sbcli_mc-1.0.6/simplyblock_core/controllers/lvol_controller.py
+-rw-r--r--  2.0 unx     1568 b- defN 24-May-29 16:34 sbcli_mc-1.0.6/simplyblock_core/controllers/device_events.py
+-rw-r--r--  2.0 unx     1630 b- defN 24-May-29 16:34 sbcli_mc-1.0.6/simplyblock_core/controllers/lvol_events.py
+-rw-r--r--  2.0 unx    11066 b- defN 24-May-29 16:34 sbcli_mc-1.0.6/simplyblock_core/controllers/snapshot_controller.py
+-rw-r--r--  2.0 unx     1122 b- defN 24-May-29 16:34 sbcli_mc-1.0.6/simplyblock_core/controllers/snapshot_events.py
+-rw-r--r--  2.0 unx     3191 b- defN 24-May-29 16:34 sbcli_mc-1.0.6/simplyblock_core/controllers/events_controller.py
+-rw-r--r--  2.0 unx    10852 b- defN 24-May-29 16:34 sbcli_mc-1.0.6/simplyblock_core/controllers/health_controller.py
+-rw-r--r--  2.0 unx    13948 b- defN 24-May-29 16:34 sbcli_mc-1.0.6/simplyblock_core/controllers/device_controller.py
+-rw-r--r--  2.0 unx      695 b- defN 24-May-29 16:34 sbcli_mc-1.0.6/simplyblock_core/controllers/pool_events.py
+-rw-r--r--  2.0 unx    23440 b- defN 24-May-29 16:34 sbcli_mc-1.0.6/simplyblock_core/controllers/caching_node_controller.py
+-rw-r--r--  2.0 unx     1900 b- defN 24-May-29 16:34 sbcli_mc-1.0.6/simplyblock_core/controllers/cluster_events.py
+-rw-r--r--  2.0 unx     1120 b- defN 24-May-29 16:34 sbcli_mc-1.0.6/simplyblock_core/controllers/mgmt_events.py
+-rw-r--r--  2.0 unx     3766 b- defN 24-May-29 16:34 sbcli_mc-1.0.6/simplyblock_core/models/caching_node.py
+-rw-r--r--  2.0 unx     2094 b- defN 24-May-29 16:34 sbcli_mc-1.0.6/simplyblock_core/models/nvme_device.py
+-rw-r--r--  2.0 unx     1452 b- defN 24-May-29 16:34 sbcli_mc-1.0.6/simplyblock_core/models/mgmt_node.py
+-rw-r--r--  2.0 unx      917 b- defN 24-May-29 16:34 sbcli_mc-1.0.6/simplyblock_core/models/compute_node.py
+-rw-r--r--  2.0 unx        0 b- defN 24-May-29 16:34 sbcli_mc-1.0.6/simplyblock_core/models/__init__.py
+-rw-r--r--  2.0 unx     1500 b- defN 24-May-29 16:34 sbcli_mc-1.0.6/simplyblock_core/models/events.py
+-rw-r--r--  2.0 unx     1228 b- defN 24-May-29 16:34 sbcli_mc-1.0.6/simplyblock_core/models/global_settings.py
+-rw-r--r--  2.0 unx      973 b- defN 24-May-29 16:34 sbcli_mc-1.0.6/simplyblock_core/models/job_schedule.py
+-rw-r--r--  2.0 unx     4846 b- defN 24-May-29 16:34 sbcli_mc-1.0.6/simplyblock_core/models/base_model.py
+-rw-r--r--  2.0 unx     2579 b- defN 24-May-29 16:34 sbcli_mc-1.0.6/simplyblock_core/models/lvol_model.py
+-rw-r--r--  2.0 unx      736 b- defN 24-May-29 16:34 sbcli_mc-1.0.6/simplyblock_core/models/snapshot.py
+-rw-r--r--  2.0 unx     3696 b- defN 24-May-29 16:34 sbcli_mc-1.0.6/simplyblock_core/models/storage_node.py
+-rw-r--r--  2.0 unx     4242 b- defN 24-May-29 16:34 sbcli_mc-1.0.6/simplyblock_core/models/stats.py
+-rw-r--r--  2.0 unx     1602 b- defN 24-May-29 16:34 sbcli_mc-1.0.6/simplyblock_core/models/pool.py
+-rw-r--r--  2.0 unx      806 b- defN 24-May-29 16:34 sbcli_mc-1.0.6/simplyblock_core/models/iface.py
+-rw-r--r--  2.0 unx     2565 b- defN 24-May-29 16:34 sbcli_mc-1.0.6/simplyblock_core/models/cluster.py
+-rw-r--r--  2.0 unx     1020 b- defN 24-May-29 16:34 sbcli_mc-1.0.6/simplyblock_core/models/port_stat.py
+drwxr-xr-x  2.0 unx        0 b- stor 24-May-29 16:34 sbcli_mc-1.0.6/simplyblock_core/scripts/alerting/
+drwxr-xr-x  2.0 unx        0 b- stor 24-May-29 16:34 sbcli_mc-1.0.6/simplyblock_core/scripts/dashboards/
+-rw-r--r--  2.0 unx     1420 b- defN 24-May-29 16:34 sbcli_mc-1.0.6/simplyblock_core/scripts/install_deps.sh
+-rw-r--r--  2.0 unx     1623 b- defN 24-May-29 16:34 sbcli_mc-1.0.6/simplyblock_core/scripts/__init__.py
+-rw-r--r--  2.0 unx       43 b- defN 24-May-29 16:34 sbcli_mc-1.0.6/simplyblock_core/scripts/run_ssh.sh
+-rw-r--r--  2.0 unx     1163 b- defN 24-May-29 16:34 sbcli_mc-1.0.6/simplyblock_core/scripts/haproxy.cfg
+-rw-r--r--  2.0 unx      118 b- defN 24-May-29 16:34 sbcli_mc-1.0.6/simplyblock_core/scripts/db_config_double.sh
+-rw-r--r--  2.0 unx     5305 b- defN 24-May-29 16:34 sbcli_mc-1.0.6/simplyblock_core/scripts/stack_deploy_wait.sh
+-rw-r--r--  2.0 unx      360 b- defN 24-May-29 16:34 sbcli_mc-1.0.6/simplyblock_core/scripts/datasource.yml
+-rw-r--r--  2.0 unx     5611 b- defN 24-May-29 16:34 sbcli_mc-1.0.6/simplyblock_core/scripts/docker-compose-swarm.yml
+-rw-r--r--  2.0 unx      152 b- defN 24-May-29 16:34 sbcli_mc-1.0.6/simplyblock_core/scripts/set_db_config.sh
+-rw-r--r--  2.0 unx      311 b- defN 24-May-29 16:34 sbcli_mc-1.0.6/simplyblock_core/scripts/prometheus.yml
+-rw-r--r--  2.0 unx      311 b- defN 24-May-29 16:34 sbcli_mc-1.0.6/simplyblock_core/scripts/clean_local_storage_deploy.sh
+-rw-r--r--  2.0 unx     4409 b- defN 24-May-29 16:34 sbcli_mc-1.0.6/simplyblock_core/scripts/docker-compose-swarm-monitoring.yml
+-rw-r--r--  2.0 unx      930 b- defN 24-May-29 16:34 sbcli_mc-1.0.6/simplyblock_core/scripts/deploy_stack.sh
+-rw-r--r--  2.0 unx       54 b- defN 24-May-29 16:34 sbcli_mc-1.0.6/simplyblock_core/scripts/db_config_single.sh
+-rw-r--r--  2.0 unx      453 b- defN 24-May-29 16:34 sbcli_mc-1.0.6/simplyblock_core/scripts/config_docker.sh
+-rw-r--r--  2.0 unx    25433 b- defN 24-May-29 16:34 sbcli_mc-1.0.6/simplyblock_core/scripts/alerting/alert_rules.yaml
+-rw-r--r--  2.0 unx     1856 b- defN 24-May-29 16:34 sbcli_mc-1.0.6/simplyblock_core/scripts/alerting/alert_resources.yaml
+-rw-r--r--  2.0 unx    88820 b- defN 24-May-29 16:34 sbcli_mc-1.0.6/simplyblock_core/scripts/dashboards/nodes.json
+-rw-r--r--  2.0 unx    89701 b- defN 24-May-29 16:34 sbcli_mc-1.0.6/simplyblock_core/scripts/dashboards/cluster.json
+-rw-r--r--  2.0 unx    88776 b- defN 24-May-29 16:34 sbcli_mc-1.0.6/simplyblock_core/scripts/dashboards/lvols.json
+-rw-r--r--  2.0 unx    88868 b- defN 24-May-29 16:34 sbcli_mc-1.0.6/simplyblock_core/scripts/dashboards/devices.json
+-rw-r--r--  2.0 unx    99707 b- defN 24-May-29 16:34 sbcli_mc-1.0.6/simplyblock_core/scripts/dashboards/pools.json
+-rw-r--r--  2.0 unx   799409 b- defN 24-May-29 16:34 sbcli_mc-1.0.6/simplyblock_core/scripts/dashboards/node-exporter.json
+-rw-r--r--  2.0 unx     5217 b- defN 24-May-29 16:34 sbcli_mc-1.0.6/sbcli_mc.egg-info/SOURCES.txt
+-rw-r--r--  2.0 unx       73 b- defN 24-May-29 16:34 sbcli_mc-1.0.6/sbcli_mc.egg-info/requires.txt
+-rw-r--r--  2.0 unx     1488 b- defN 24-May-29 16:34 sbcli_mc-1.0.6/sbcli_mc.egg-info/PKG-INFO
+-rw-r--r--  2.0 unx       49 b- defN 24-May-29 16:34 sbcli_mc-1.0.6/sbcli_mc.egg-info/top_level.txt
+-rw-r--r--  2.0 unx       54 b- defN 24-May-29 16:34 sbcli_mc-1.0.6/sbcli_mc.egg-info/entry_points.txt
+-rw-r--r--  2.0 unx        1 b- defN 24-May-29 16:34 sbcli_mc-1.0.6/sbcli_mc.egg-info/dependency_links.txt
+147 files, 1874645 bytes uncompressed, 186062 bytes compressed:  90.1%
```

## zipnote {}

```diff
@@ -1,445 +1,442 @@
-Filename: sbcli_mc-1.0.5/
+Filename: sbcli_mc-1.0.6/
 Comment: 
 
-Filename: sbcli_mc-1.0.5/simplyblock_cli/
+Filename: sbcli_mc-1.0.6/simplyblock_cli/
 Comment: 
 
-Filename: sbcli_mc-1.0.5/simplyblock_web/
+Filename: sbcli_mc-1.0.6/simplyblock_web/
 Comment: 
 
-Filename: sbcli_mc-1.0.5/simplyblock_core/
+Filename: sbcli_mc-1.0.6/simplyblock_core/
 Comment: 
 
-Filename: sbcli_mc-1.0.5/sbcli_mc.egg-info/
+Filename: sbcli_mc-1.0.6/sbcli_mc.egg-info/
 Comment: 
 
-Filename: sbcli_mc-1.0.5/README.md
+Filename: sbcli_mc-1.0.6/README.md
 Comment: 
 
-Filename: sbcli_mc-1.0.5/pyproject.toml
+Filename: sbcli_mc-1.0.6/pyproject.toml
 Comment: 
 
-Filename: sbcli_mc-1.0.5/PKG-INFO
+Filename: sbcli_mc-1.0.6/PKG-INFO
 Comment: 
 
-Filename: sbcli_mc-1.0.5/env_var
+Filename: sbcli_mc-1.0.6/env_var
 Comment: 
 
-Filename: sbcli_mc-1.0.5/setup.cfg
+Filename: sbcli_mc-1.0.6/setup.cfg
 Comment: 
 
-Filename: sbcli_mc-1.0.5/setup.py
+Filename: sbcli_mc-1.0.6/setup.py
 Comment: 
 
-Filename: sbcli_mc-1.0.5/simplyblock_cli/cli.py
+Filename: sbcli_mc-1.0.6/simplyblock_cli/cli.py
 Comment: 
 
-Filename: sbcli_mc-1.0.5/simplyblock_cli/main.py
+Filename: sbcli_mc-1.0.6/simplyblock_cli/main.py
 Comment: 
 
-Filename: sbcli_mc-1.0.5/simplyblock_web/static/
+Filename: sbcli_mc-1.0.6/simplyblock_web/static/
 Comment: 
 
-Filename: sbcli_mc-1.0.5/simplyblock_web/blueprints/
+Filename: sbcli_mc-1.0.6/simplyblock_web/blueprints/
 Comment: 
 
-Filename: sbcli_mc-1.0.5/simplyblock_web/templates/
+Filename: sbcli_mc-1.0.6/simplyblock_web/templates/
 Comment: 
 
-Filename: sbcli_mc-1.0.5/simplyblock_web/__init__.py
+Filename: sbcli_mc-1.0.6/simplyblock_web/__init__.py
 Comment: 
 
-Filename: sbcli_mc-1.0.5/simplyblock_web/node_webapp.py
+Filename: sbcli_mc-1.0.6/simplyblock_web/node_webapp.py
 Comment: 
 
-Filename: sbcli_mc-1.0.5/simplyblock_web/snode_app.py
+Filename: sbcli_mc-1.0.6/simplyblock_web/snode_app.py
 Comment: 
 
-Filename: sbcli_mc-1.0.5/simplyblock_web/caching_node_app.py
+Filename: sbcli_mc-1.0.6/simplyblock_web/caching_node_app.py
 Comment: 
 
-Filename: sbcli_mc-1.0.5/simplyblock_web/auth_middleware.py
+Filename: sbcli_mc-1.0.6/simplyblock_web/auth_middleware.py
 Comment: 
 
-Filename: sbcli_mc-1.0.5/simplyblock_web/node_utils.py
+Filename: sbcli_mc-1.0.6/simplyblock_web/node_utils.py
 Comment: 
 
-Filename: sbcli_mc-1.0.5/simplyblock_web/utils.py
+Filename: sbcli_mc-1.0.6/simplyblock_web/utils.py
 Comment: 
 
-Filename: sbcli_mc-1.0.5/simplyblock_web/app.py
+Filename: sbcli_mc-1.0.6/simplyblock_web/app.py
 Comment: 
 
-Filename: sbcli_mc-1.0.5/simplyblock_web/caching_node_app_k8s.py
+Filename: sbcli_mc-1.0.6/simplyblock_web/caching_node_app_k8s.py
 Comment: 
 
-Filename: sbcli_mc-1.0.5/simplyblock_web/static/tst.py
+Filename: sbcli_mc-1.0.6/simplyblock_web/static/tst.py
 Comment: 
 
-Filename: sbcli_mc-1.0.5/simplyblock_web/static/delete.py
+Filename: sbcli_mc-1.0.6/simplyblock_web/static/delete.py
 Comment: 
 
-Filename: sbcli_mc-1.0.5/simplyblock_web/static/deploy_cnode.yaml
+Filename: sbcli_mc-1.0.6/simplyblock_web/static/deploy_cnode.yaml
 Comment: 
 
-Filename: sbcli_mc-1.0.5/simplyblock_web/static/is_up.py
+Filename: sbcli_mc-1.0.6/simplyblock_web/static/is_up.py
 Comment: 
 
-Filename: sbcli_mc-1.0.5/simplyblock_web/static/deploy_spdk.yaml
+Filename: sbcli_mc-1.0.6/simplyblock_web/static/deploy_spdk.yaml
 Comment: 
 
-Filename: sbcli_mc-1.0.5/simplyblock_web/static/rpac.yaml
+Filename: sbcli_mc-1.0.6/simplyblock_web/static/rpac.yaml
 Comment: 
 
-Filename: sbcli_mc-1.0.5/simplyblock_web/static/list_deps.py
+Filename: sbcli_mc-1.0.6/simplyblock_web/static/list_deps.py
 Comment: 
 
-Filename: sbcli_mc-1.0.5/simplyblock_web/static/deploy.py
+Filename: sbcli_mc-1.0.6/simplyblock_web/static/deploy.py
 Comment: 
 
-Filename: sbcli_mc-1.0.5/simplyblock_web/blueprints/web_api_pool.py
+Filename: sbcli_mc-1.0.6/simplyblock_web/blueprints/web_api_pool.py
 Comment: 
 
-Filename: sbcli_mc-1.0.5/simplyblock_web/blueprints/__init__.py
+Filename: sbcli_mc-1.0.6/simplyblock_web/blueprints/__init__.py
 Comment: 
 
-Filename: sbcli_mc-1.0.5/simplyblock_web/blueprints/web_api_device.py
+Filename: sbcli_mc-1.0.6/simplyblock_web/blueprints/web_api_device.py
 Comment: 
 
-Filename: sbcli_mc-1.0.5/simplyblock_web/blueprints/web_api_lvol.py
+Filename: sbcli_mc-1.0.6/simplyblock_web/blueprints/web_api_lvol.py
 Comment: 
 
-Filename: sbcli_mc-1.0.5/simplyblock_web/blueprints/snode_ops.py
+Filename: sbcli_mc-1.0.6/simplyblock_web/blueprints/snode_ops.py
 Comment: 
 
-Filename: sbcli_mc-1.0.5/simplyblock_web/blueprints/caching_node_ops.py
+Filename: sbcli_mc-1.0.6/simplyblock_web/blueprints/caching_node_ops.py
 Comment: 
 
-Filename: sbcli_mc-1.0.5/simplyblock_web/blueprints/web_api_storage_node.py
+Filename: sbcli_mc-1.0.6/simplyblock_web/blueprints/web_api_storage_node.py
 Comment: 
 
-Filename: sbcli_mc-1.0.5/simplyblock_web/blueprints/web_api_cluster.py
+Filename: sbcli_mc-1.0.6/simplyblock_web/blueprints/web_api_cluster.py
 Comment: 
 
-Filename: sbcli_mc-1.0.5/simplyblock_web/blueprints/caching_node_ops_k8s.py
+Filename: sbcli_mc-1.0.6/simplyblock_web/blueprints/caching_node_ops_k8s.py
 Comment: 
 
-Filename: sbcli_mc-1.0.5/simplyblock_web/blueprints/node_api_caching_ks.py
+Filename: sbcli_mc-1.0.6/simplyblock_web/blueprints/node_api_caching_ks.py
 Comment: 
 
-Filename: sbcli_mc-1.0.5/simplyblock_web/blueprints/node_api_caching_docker.py
+Filename: sbcli_mc-1.0.6/simplyblock_web/blueprints/node_api_caching_docker.py
 Comment: 
 
-Filename: sbcli_mc-1.0.5/simplyblock_web/blueprints/web_api_caching_node.py
+Filename: sbcli_mc-1.0.6/simplyblock_web/blueprints/web_api_caching_node.py
 Comment: 
 
-Filename: sbcli_mc-1.0.5/simplyblock_web/blueprints/node_api_basic.py
+Filename: sbcli_mc-1.0.6/simplyblock_web/blueprints/node_api_basic.py
 Comment: 
 
-Filename: sbcli_mc-1.0.5/simplyblock_web/blueprints/csi.py
+Filename: sbcli_mc-1.0.6/simplyblock_web/blueprints/csi.py
 Comment: 
 
-Filename: sbcli_mc-1.0.5/simplyblock_web/blueprints/web_api_mgmt_node.py
+Filename: sbcli_mc-1.0.6/simplyblock_web/blueprints/web_api_mgmt_node.py
 Comment: 
 
-Filename: sbcli_mc-1.0.5/simplyblock_web/templates/deploy_spdk.yaml.j2
+Filename: sbcli_mc-1.0.6/simplyblock_web/templates/deploy_spdk.yaml.j2
 Comment: 
 
-Filename: sbcli_mc-1.0.5/simplyblock_core/services/
+Filename: sbcli_mc-1.0.6/simplyblock_core/services/
 Comment: 
 
-Filename: sbcli_mc-1.0.5/simplyblock_core/controllers/
+Filename: sbcli_mc-1.0.6/simplyblock_core/controllers/
 Comment: 
 
-Filename: sbcli_mc-1.0.5/simplyblock_core/models/
+Filename: sbcli_mc-1.0.6/simplyblock_core/models/
 Comment: 
 
-Filename: sbcli_mc-1.0.5/simplyblock_core/scripts/
+Filename: sbcli_mc-1.0.6/simplyblock_core/scripts/
 Comment: 
 
-Filename: sbcli_mc-1.0.5/simplyblock_core/cluster_ops.py
+Filename: sbcli_mc-1.0.6/simplyblock_core/cluster_ops.py
 Comment: 
 
-Filename: sbcli_mc-1.0.5/simplyblock_core/pci_utils.py
+Filename: sbcli_mc-1.0.6/simplyblock_core/pci_utils.py
 Comment: 
 
-Filename: sbcli_mc-1.0.5/simplyblock_core/__init__.py
+Filename: sbcli_mc-1.0.6/simplyblock_core/__init__.py
 Comment: 
 
-Filename: sbcli_mc-1.0.5/simplyblock_core/snode_client.py
+Filename: sbcli_mc-1.0.6/simplyblock_core/snode_client.py
 Comment: 
 
-Filename: sbcli_mc-1.0.5/simplyblock_core/kv_store.py
+Filename: sbcli_mc-1.0.6/simplyblock_core/kv_store.py
 Comment: 
 
-Filename: sbcli_mc-1.0.5/simplyblock_core/compute_node_ops.py
+Filename: sbcli_mc-1.0.6/simplyblock_core/compute_node_ops.py
 Comment: 
 
-Filename: sbcli_mc-1.0.5/simplyblock_core/rpc_client.py
+Filename: sbcli_mc-1.0.6/simplyblock_core/rpc_client.py
 Comment: 
 
-Filename: sbcli_mc-1.0.5/simplyblock_core/mgmt_node_ops.py
+Filename: sbcli_mc-1.0.6/simplyblock_core/mgmt_node_ops.py
 Comment: 
 
-Filename: sbcli_mc-1.0.5/simplyblock_core/utils.py
+Filename: sbcli_mc-1.0.6/simplyblock_core/utils.py
 Comment: 
 
-Filename: sbcli_mc-1.0.5/simplyblock_core/distr_controller.py
+Filename: sbcli_mc-1.0.6/simplyblock_core/distr_controller.py
 Comment: 
 
-Filename: sbcli_mc-1.0.5/simplyblock_core/shell_utils.py
+Filename: sbcli_mc-1.0.6/simplyblock_core/shell_utils.py
 Comment: 
 
-Filename: sbcli_mc-1.0.5/simplyblock_core/cnode_client.py
+Filename: sbcli_mc-1.0.6/simplyblock_core/cnode_client.py
 Comment: 
 
-Filename: sbcli_mc-1.0.5/simplyblock_core/storage_node_ops.py
+Filename: sbcli_mc-1.0.6/simplyblock_core/storage_node_ops.py
 Comment: 
 
-Filename: sbcli_mc-1.0.5/simplyblock_core/constants.py
+Filename: sbcli_mc-1.0.6/simplyblock_core/constants.py
 Comment: 
 
-Filename: sbcli_mc-1.0.5/simplyblock_core/services/job_tasks.py
+Filename: sbcli_mc-1.0.6/simplyblock_core/services/job_tasks.py
 Comment: 
 
-Filename: sbcli_mc-1.0.5/simplyblock_core/services/caching_node_monitor.py
+Filename: sbcli_mc-1.0.6/simplyblock_core/services/caching_node_monitor.py
 Comment: 
 
-Filename: sbcli_mc-1.0.5/simplyblock_core/services/service_template.service
+Filename: sbcli_mc-1.0.6/simplyblock_core/services/service_template.service
 Comment: 
 
-Filename: sbcli_mc-1.0.5/simplyblock_core/services/install_service.sh
+Filename: sbcli_mc-1.0.6/simplyblock_core/services/install_service.sh
 Comment: 
 
-Filename: sbcli_mc-1.0.5/simplyblock_core/services/__init__.py
+Filename: sbcli_mc-1.0.6/simplyblock_core/services/__init__.py
 Comment: 
 
-Filename: sbcli_mc-1.0.5/simplyblock_core/services/log_agg_service.py
+Filename: sbcli_mc-1.0.6/simplyblock_core/services/log_agg_service.py
 Comment: 
 
-Filename: sbcli_mc-1.0.5/simplyblock_core/services/health_check_service.py
+Filename: sbcli_mc-1.0.6/simplyblock_core/services/health_check_service.py
 Comment: 
 
-Filename: sbcli_mc-1.0.5/simplyblock_core/services/capacity_and_stats_collector.py
+Filename: sbcli_mc-1.0.6/simplyblock_core/services/capacity_and_stats_collector.py
 Comment: 
 
-Filename: sbcli_mc-1.0.5/simplyblock_core/services/device_monitor.py
+Filename: sbcli_mc-1.0.6/simplyblock_core/services/device_monitor.py
 Comment: 
 
-Filename: sbcli_mc-1.0.5/simplyblock_core/services/lvol_stat_collector.py
+Filename: sbcli_mc-1.0.6/simplyblock_core/services/lvol_stat_collector.py
 Comment: 
 
-Filename: sbcli_mc-1.0.5/simplyblock_core/services/cap_monitor.py
+Filename: sbcli_mc-1.0.6/simplyblock_core/services/cap_monitor.py
 Comment: 
 
-Filename: sbcli_mc-1.0.5/simplyblock_core/services/storage_node_monitor.py
+Filename: sbcli_mc-1.0.6/simplyblock_core/services/storage_node_monitor.py
 Comment: 
 
-Filename: sbcli_mc-1.0.5/simplyblock_core/services/port_stat_collector.py
+Filename: sbcli_mc-1.0.6/simplyblock_core/services/port_stat_collector.py
 Comment: 
 
-Filename: sbcli_mc-1.0.5/simplyblock_core/services/distr_event_collector.py
+Filename: sbcli_mc-1.0.6/simplyblock_core/services/distr_event_collector.py
 Comment: 
 
-Filename: sbcli_mc-1.0.5/simplyblock_core/services/remove_service.sh
+Filename: sbcli_mc-1.0.6/simplyblock_core/services/remove_service.sh
 Comment: 
 
-Filename: sbcli_mc-1.0.5/simplyblock_core/services/mgmt_node_monitor.py
+Filename: sbcli_mc-1.0.6/simplyblock_core/services/mgmt_node_monitor.py
 Comment: 
 
-Filename: sbcli_mc-1.0.5/simplyblock_core/services/lvol_monitor.py
+Filename: sbcli_mc-1.0.6/simplyblock_core/services/lvol_monitor.py
 Comment: 
 
-Filename: sbcli_mc-1.0.5/simplyblock_core/controllers/pool_controller.py
+Filename: sbcli_mc-1.0.6/simplyblock_core/controllers/pool_controller.py
 Comment: 
 
-Filename: sbcli_mc-1.0.5/simplyblock_core/controllers/__init__.py
+Filename: sbcli_mc-1.0.6/simplyblock_core/controllers/__init__.py
 Comment: 
 
-Filename: sbcli_mc-1.0.5/simplyblock_core/controllers/storage_events.py
+Filename: sbcli_mc-1.0.6/simplyblock_core/controllers/storage_events.py
 Comment: 
 
-Filename: sbcli_mc-1.0.5/simplyblock_core/controllers/lvol_controller.py
+Filename: sbcli_mc-1.0.6/simplyblock_core/controllers/lvol_controller.py
 Comment: 
 
-Filename: sbcli_mc-1.0.5/simplyblock_core/controllers/device_events.py
+Filename: sbcli_mc-1.0.6/simplyblock_core/controllers/device_events.py
 Comment: 
 
-Filename: sbcli_mc-1.0.5/simplyblock_core/controllers/lvol_events.py
+Filename: sbcli_mc-1.0.6/simplyblock_core/controllers/lvol_events.py
 Comment: 
 
-Filename: sbcli_mc-1.0.5/simplyblock_core/controllers/snapshot_controller.py
+Filename: sbcli_mc-1.0.6/simplyblock_core/controllers/snapshot_controller.py
 Comment: 
 
-Filename: sbcli_mc-1.0.5/simplyblock_core/controllers/snapshot_events.py
+Filename: sbcli_mc-1.0.6/simplyblock_core/controllers/snapshot_events.py
 Comment: 
 
-Filename: sbcli_mc-1.0.5/simplyblock_core/controllers/events_controller.py
+Filename: sbcli_mc-1.0.6/simplyblock_core/controllers/events_controller.py
 Comment: 
 
-Filename: sbcli_mc-1.0.5/simplyblock_core/controllers/health_controller.py
+Filename: sbcli_mc-1.0.6/simplyblock_core/controllers/health_controller.py
 Comment: 
 
-Filename: sbcli_mc-1.0.5/simplyblock_core/controllers/device_controller.py
+Filename: sbcli_mc-1.0.6/simplyblock_core/controllers/device_controller.py
 Comment: 
 
-Filename: sbcli_mc-1.0.5/simplyblock_core/controllers/pool_events.py
+Filename: sbcli_mc-1.0.6/simplyblock_core/controllers/pool_events.py
 Comment: 
 
-Filename: sbcli_mc-1.0.5/simplyblock_core/controllers/caching_node_controller.py
+Filename: sbcli_mc-1.0.6/simplyblock_core/controllers/caching_node_controller.py
 Comment: 
 
-Filename: sbcli_mc-1.0.5/simplyblock_core/controllers/cluster_events.py
+Filename: sbcli_mc-1.0.6/simplyblock_core/controllers/cluster_events.py
 Comment: 
 
-Filename: sbcli_mc-1.0.5/simplyblock_core/controllers/mgmt_events.py
+Filename: sbcli_mc-1.0.6/simplyblock_core/controllers/mgmt_events.py
 Comment: 
 
-Filename: sbcli_mc-1.0.5/simplyblock_core/models/caching_node.py
+Filename: sbcli_mc-1.0.6/simplyblock_core/models/caching_node.py
 Comment: 
 
-Filename: sbcli_mc-1.0.5/simplyblock_core/models/nvme_device.py
+Filename: sbcli_mc-1.0.6/simplyblock_core/models/nvme_device.py
 Comment: 
 
-Filename: sbcli_mc-1.0.5/simplyblock_core/models/mgmt_node.py
+Filename: sbcli_mc-1.0.6/simplyblock_core/models/mgmt_node.py
 Comment: 
 
-Filename: sbcli_mc-1.0.5/simplyblock_core/models/compute_node.py
+Filename: sbcli_mc-1.0.6/simplyblock_core/models/compute_node.py
 Comment: 
 
-Filename: sbcli_mc-1.0.5/simplyblock_core/models/__init__.py
+Filename: sbcli_mc-1.0.6/simplyblock_core/models/__init__.py
 Comment: 
 
-Filename: sbcli_mc-1.0.5/simplyblock_core/models/events.py
+Filename: sbcli_mc-1.0.6/simplyblock_core/models/events.py
 Comment: 
 
-Filename: sbcli_mc-1.0.5/simplyblock_core/models/global_settings.py
+Filename: sbcli_mc-1.0.6/simplyblock_core/models/global_settings.py
 Comment: 
 
-Filename: sbcli_mc-1.0.5/simplyblock_core/models/job_schedule.py
+Filename: sbcli_mc-1.0.6/simplyblock_core/models/job_schedule.py
 Comment: 
 
-Filename: sbcli_mc-1.0.5/simplyblock_core/models/base_model.py
+Filename: sbcli_mc-1.0.6/simplyblock_core/models/base_model.py
 Comment: 
 
-Filename: sbcli_mc-1.0.5/simplyblock_core/models/lvol_model.py
+Filename: sbcli_mc-1.0.6/simplyblock_core/models/lvol_model.py
 Comment: 
 
-Filename: sbcli_mc-1.0.5/simplyblock_core/models/snapshot.py
+Filename: sbcli_mc-1.0.6/simplyblock_core/models/snapshot.py
 Comment: 
 
-Filename: sbcli_mc-1.0.5/simplyblock_core/models/storage_node.py
+Filename: sbcli_mc-1.0.6/simplyblock_core/models/storage_node.py
 Comment: 
 
-Filename: sbcli_mc-1.0.5/simplyblock_core/models/stats.py
+Filename: sbcli_mc-1.0.6/simplyblock_core/models/stats.py
 Comment: 
 
-Filename: sbcli_mc-1.0.5/simplyblock_core/models/pool.py
+Filename: sbcli_mc-1.0.6/simplyblock_core/models/pool.py
 Comment: 
 
-Filename: sbcli_mc-1.0.5/simplyblock_core/models/iface.py
+Filename: sbcli_mc-1.0.6/simplyblock_core/models/iface.py
 Comment: 
 
-Filename: sbcli_mc-1.0.5/simplyblock_core/models/cluster.py
+Filename: sbcli_mc-1.0.6/simplyblock_core/models/cluster.py
 Comment: 
 
-Filename: sbcli_mc-1.0.5/simplyblock_core/models/port_stat.py
+Filename: sbcli_mc-1.0.6/simplyblock_core/models/port_stat.py
 Comment: 
 
-Filename: sbcli_mc-1.0.5/simplyblock_core/scripts/alerting/
+Filename: sbcli_mc-1.0.6/simplyblock_core/scripts/alerting/
 Comment: 
 
-Filename: sbcli_mc-1.0.5/simplyblock_core/scripts/dashboards/
+Filename: sbcli_mc-1.0.6/simplyblock_core/scripts/dashboards/
 Comment: 
 
-Filename: sbcli_mc-1.0.5/simplyblock_core/scripts/install_deps.sh
+Filename: sbcli_mc-1.0.6/simplyblock_core/scripts/install_deps.sh
 Comment: 
 
-Filename: sbcli_mc-1.0.5/simplyblock_core/scripts/__init__.py
+Filename: sbcli_mc-1.0.6/simplyblock_core/scripts/__init__.py
 Comment: 
 
-Filename: sbcli_mc-1.0.5/simplyblock_core/scripts/run_ssh.sh
+Filename: sbcli_mc-1.0.6/simplyblock_core/scripts/run_ssh.sh
 Comment: 
 
-Filename: sbcli_mc-1.0.5/simplyblock_core/scripts/haproxy.cfg
+Filename: sbcli_mc-1.0.6/simplyblock_core/scripts/haproxy.cfg
 Comment: 
 
-Filename: sbcli_mc-1.0.5/simplyblock_core/scripts/db_config_double.sh
+Filename: sbcli_mc-1.0.6/simplyblock_core/scripts/db_config_double.sh
 Comment: 
 
-Filename: sbcli_mc-1.0.5/simplyblock_core/scripts/stack_deploy_wait.sh
+Filename: sbcli_mc-1.0.6/simplyblock_core/scripts/stack_deploy_wait.sh
 Comment: 
 
-Filename: sbcli_mc-1.0.5/simplyblock_core/scripts/datasource.yml
+Filename: sbcli_mc-1.0.6/simplyblock_core/scripts/datasource.yml
 Comment: 
 
-Filename: sbcli_mc-1.0.5/simplyblock_core/scripts/docker-compose-swarm.yml
+Filename: sbcli_mc-1.0.6/simplyblock_core/scripts/docker-compose-swarm.yml
 Comment: 
 
-Filename: sbcli_mc-1.0.5/simplyblock_core/scripts/set_db_config.sh
+Filename: sbcli_mc-1.0.6/simplyblock_core/scripts/set_db_config.sh
 Comment: 
 
-Filename: sbcli_mc-1.0.5/simplyblock_core/scripts/apply_dashboard.sh
+Filename: sbcli_mc-1.0.6/simplyblock_core/scripts/prometheus.yml
 Comment: 
 
-Filename: sbcli_mc-1.0.5/simplyblock_core/scripts/prometheus.yml
+Filename: sbcli_mc-1.0.6/simplyblock_core/scripts/clean_local_storage_deploy.sh
 Comment: 
 
-Filename: sbcli_mc-1.0.5/simplyblock_core/scripts/clean_local_storage_deploy.sh
+Filename: sbcli_mc-1.0.6/simplyblock_core/scripts/docker-compose-swarm-monitoring.yml
 Comment: 
 
-Filename: sbcli_mc-1.0.5/simplyblock_core/scripts/docker-compose-swarm-monitoring.yml
+Filename: sbcli_mc-1.0.6/simplyblock_core/scripts/deploy_stack.sh
 Comment: 
 
-Filename: sbcli_mc-1.0.5/simplyblock_core/scripts/deploy_stack.sh
+Filename: sbcli_mc-1.0.6/simplyblock_core/scripts/db_config_single.sh
 Comment: 
 
-Filename: sbcli_mc-1.0.5/simplyblock_core/scripts/db_config_single.sh
+Filename: sbcli_mc-1.0.6/simplyblock_core/scripts/config_docker.sh
 Comment: 
 
-Filename: sbcli_mc-1.0.5/simplyblock_core/scripts/config_docker.sh
+Filename: sbcli_mc-1.0.6/simplyblock_core/scripts/alerting/alert_rules.yaml
 Comment: 
 
-Filename: sbcli_mc-1.0.5/simplyblock_core/scripts/alerting/alert_rules.yaml
+Filename: sbcli_mc-1.0.6/simplyblock_core/scripts/alerting/alert_resources.yaml
 Comment: 
 
-Filename: sbcli_mc-1.0.5/simplyblock_core/scripts/alerting/alert_resources.yaml
+Filename: sbcli_mc-1.0.6/simplyblock_core/scripts/dashboards/nodes.json
 Comment: 
 
-Filename: sbcli_mc-1.0.5/simplyblock_core/scripts/dashboards/nodes.json
+Filename: sbcli_mc-1.0.6/simplyblock_core/scripts/dashboards/cluster.json
 Comment: 
 
-Filename: sbcli_mc-1.0.5/simplyblock_core/scripts/dashboards/cluster.json
+Filename: sbcli_mc-1.0.6/simplyblock_core/scripts/dashboards/lvols.json
 Comment: 
 
-Filename: sbcli_mc-1.0.5/simplyblock_core/scripts/dashboards/lvols.json
+Filename: sbcli_mc-1.0.6/simplyblock_core/scripts/dashboards/devices.json
 Comment: 
 
-Filename: sbcli_mc-1.0.5/simplyblock_core/scripts/dashboards/devices.json
+Filename: sbcli_mc-1.0.6/simplyblock_core/scripts/dashboards/pools.json
 Comment: 
 
-Filename: sbcli_mc-1.0.5/simplyblock_core/scripts/dashboards/pools.json
+Filename: sbcli_mc-1.0.6/simplyblock_core/scripts/dashboards/node-exporter.json
 Comment: 
 
-Filename: sbcli_mc-1.0.5/simplyblock_core/scripts/dashboards/node-exporter.json
+Filename: sbcli_mc-1.0.6/sbcli_mc.egg-info/SOURCES.txt
 Comment: 
 
-Filename: sbcli_mc-1.0.5/sbcli_mc.egg-info/SOURCES.txt
+Filename: sbcli_mc-1.0.6/sbcli_mc.egg-info/requires.txt
 Comment: 
 
-Filename: sbcli_mc-1.0.5/sbcli_mc.egg-info/requires.txt
+Filename: sbcli_mc-1.0.6/sbcli_mc.egg-info/PKG-INFO
 Comment: 
 
-Filename: sbcli_mc-1.0.5/sbcli_mc.egg-info/PKG-INFO
+Filename: sbcli_mc-1.0.6/sbcli_mc.egg-info/top_level.txt
 Comment: 
 
-Filename: sbcli_mc-1.0.5/sbcli_mc.egg-info/top_level.txt
+Filename: sbcli_mc-1.0.6/sbcli_mc.egg-info/entry_points.txt
 Comment: 
 
-Filename: sbcli_mc-1.0.5/sbcli_mc.egg-info/entry_points.txt
-Comment: 
-
-Filename: sbcli_mc-1.0.5/sbcli_mc.egg-info/dependency_links.txt
+Filename: sbcli_mc-1.0.6/sbcli_mc.egg-info/dependency_links.txt
 Comment: 
 
 Zip file comment:
```

## Comparing `sbcli_mc-1.0.5/README.md` & `sbcli_mc-1.0.6/README.md`

 * *Files identical despite different names*

## Comparing `sbcli_mc-1.0.5/PKG-INFO` & `sbcli_mc-1.0.6/PKG-INFO`

 * *Files 1% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: sbcli-mc
-Version: 1.0.5
+Version: 1.0.6
 Summary: CLI for managing SimplyBlock cluster
 Home-page: https://www.simplyblock.io/
 Author: Hamdy
 Author-email: hamdy@simplyblock.io
 Description-Content-Type: text/markdown
 Requires-Dist: foundationdb
 Requires-Dist: requests
```

## Comparing `sbcli_mc-1.0.5/setup.py` & `sbcli_mc-1.0.6/setup.py`

 * *Files identical despite different names*

## Comparing `sbcli_mc-1.0.5/simplyblock_cli/cli.py` & `sbcli_mc-1.0.6/simplyblock_cli/cli.py`

 * *Files identical despite different names*

## Comparing `sbcli_mc-1.0.5/simplyblock_web/node_webapp.py` & `sbcli_mc-1.0.6/simplyblock_web/node_webapp.py`

 * *Files identical despite different names*

## Comparing `sbcli_mc-1.0.5/simplyblock_web/snode_app.py` & `sbcli_mc-1.0.6/simplyblock_web/snode_app.py`

 * *Files identical despite different names*

## Comparing `sbcli_mc-1.0.5/simplyblock_web/caching_node_app.py` & `sbcli_mc-1.0.6/simplyblock_web/caching_node_app.py`

 * *Files identical despite different names*

## Comparing `sbcli_mc-1.0.5/simplyblock_web/auth_middleware.py` & `sbcli_mc-1.0.6/simplyblock_web/auth_middleware.py`

 * *Files identical despite different names*

## Comparing `sbcli_mc-1.0.5/simplyblock_web/node_utils.py` & `sbcli_mc-1.0.6/simplyblock_web/node_utils.py`

 * *Files identical despite different names*

## Comparing `sbcli_mc-1.0.5/simplyblock_web/utils.py` & `sbcli_mc-1.0.6/simplyblock_web/utils.py`

 * *Files identical despite different names*

## Comparing `sbcli_mc-1.0.5/simplyblock_web/app.py` & `sbcli_mc-1.0.6/simplyblock_web/app.py`

 * *Files identical despite different names*

## Comparing `sbcli_mc-1.0.5/simplyblock_web/caching_node_app_k8s.py` & `sbcli_mc-1.0.6/simplyblock_web/caching_node_app_k8s.py`

 * *Files identical despite different names*

## Comparing `sbcli_mc-1.0.5/simplyblock_web/static/delete.py` & `sbcli_mc-1.0.6/simplyblock_web/static/delete.py`

 * *Files identical despite different names*

## Comparing `sbcli_mc-1.0.5/simplyblock_web/static/deploy_spdk.yaml` & `sbcli_mc-1.0.6/simplyblock_web/static/deploy_spdk.yaml`

 * *Files identical despite different names*

## Comparing `sbcli_mc-1.0.5/simplyblock_web/static/deploy.py` & `sbcli_mc-1.0.6/simplyblock_web/static/deploy.py`

 * *Files identical despite different names*

## Comparing `sbcli_mc-1.0.5/simplyblock_web/blueprints/web_api_pool.py` & `sbcli_mc-1.0.6/simplyblock_web/blueprints/web_api_pool.py`

 * *Files identical despite different names*

## Comparing `sbcli_mc-1.0.5/simplyblock_web/blueprints/web_api_device.py` & `sbcli_mc-1.0.6/simplyblock_web/blueprints/web_api_device.py`

 * *Files identical despite different names*

## Comparing `sbcli_mc-1.0.5/simplyblock_web/blueprints/web_api_lvol.py` & `sbcli_mc-1.0.6/simplyblock_web/blueprints/web_api_lvol.py`

 * *Files identical despite different names*

## Comparing `sbcli_mc-1.0.5/simplyblock_web/blueprints/snode_ops.py` & `sbcli_mc-1.0.6/simplyblock_web/blueprints/snode_ops.py`

 * *Files identical despite different names*

## Comparing `sbcli_mc-1.0.5/simplyblock_web/blueprints/caching_node_ops.py` & `sbcli_mc-1.0.6/simplyblock_web/blueprints/caching_node_ops.py`

 * *Files identical despite different names*

## Comparing `sbcli_mc-1.0.5/simplyblock_web/blueprints/web_api_storage_node.py` & `sbcli_mc-1.0.6/simplyblock_web/blueprints/web_api_storage_node.py`

 * *Files identical despite different names*

## Comparing `sbcli_mc-1.0.5/simplyblock_web/blueprints/web_api_cluster.py` & `sbcli_mc-1.0.6/simplyblock_web/blueprints/web_api_cluster.py`

 * *Files 18% similar despite different names*

```diff
@@ -18,58 +18,42 @@
 logger.setLevel(logging.DEBUG)
 bp = Blueprint("cluster", __name__)
 db_controller = kv_store.DBController()
 
 
 @bp.route('/cluster', methods=['POST'])
 def add_cluster():
+
+    blk_size = 512
+    page_size_in_blocks = 2097152
+    ha_type = "single"
+    cap_warn = 0
+    cap_crit = 0
+    prov_cap_warn = 0
+    prov_cap_crit = 0
+
     cl_data = request.get_json()
-    if 'blk_size' not in cl_data:
-        return utils.get_response_error("missing required param: blk_size", 400)
-    if 'page_size_in_blocks' not in cl_data:
-        return utils.get_response_error("missing required param: page_size_in_blocks", 400)
-    if 'model_ids' not in cl_data:
-        return utils.get_response_error("missing required param: model_ids", 400)
-    if 'ha_type' not in cl_data:
-        return utils.get_response_error("missing required param: ha_type", 400)
-    if 'tls' not in cl_data:
-        return utils.get_response_error("missing required param: tls", 400)
-    if 'auth-hosts-only' not in cl_data:
-        return utils.get_response_error("missing required param: auth-hosts-only", 400)
-    if 'dhchap' not in cl_data:
-        return utils.get_response_error("missing required param: dhchap", 400)
-    if 'NQN' not in cl_data:
-        return utils.get_response_error("missing required param: NQN", 400)
-
-    c = Cluster()
-    c.uuid = str(uuid.uuid4())
-
-    if cl_data['blk_size'] not in [512, 4096]:
-        return utils.get_response_error("blk_size can be 512 or 4096", 400)
-
-    if cl_data['ha_type'] not in ["single", "ha"]:
-        return utils.get_response_error("ha_type can be single or ha", 400)
-
-    if cl_data['dhchap'] not in ["off", "one-way", "bi-direct"]:
-        return utils.get_response_error("dhchap can be off, one-way or bi-direct", 400)
-
-    c.blk_size = cl_data['blk_size']
-    c.page_size_in_blocks = cl_data['page_size_in_blocks']
-    c.model_ids = cl_data['model_ids']
-    c.ha_type = cl_data['ha_type']
-    c.tls = cl_data['tls']
-    c.auth_hosts_only = cl_data['auth-hosts-only']
-    c.nqn = cl_data['nqn']
-    c.iscsi = cl_data['iscsi'] or False
-    c.dhchap = cl_data['dhchap']
-    c.cluster_status = Cluster.STATUS_ACTIVE
-    c.updated_at = int(time.time())
-    c.write_to_db(db_controller.kv_store)
+    if 'blk_size' in cl_data:
+        if cl_data['blk_size'] not in [512, 4096]:
+            return utils.get_response_error("blk_size can be 512 or 4096", 400)
+        else:
+            blk_size = cl_data['blk_size']
+
+    if 'page_size_in_blocks' in cl_data:
+        page_size_in_blocks = cl_data['page_size_in_blocks']
+
+    if 'ha_type' in cl_data:
+        if cl_data['ha_type'] not in ["single", "ha"]:
+            return utils.get_response_error("ha_type can be single or ha", 400)
+        ha_type = cl_data['ha_type']
+
+    ret = cluster_ops.add_cluster(blk_size, page_size_in_blocks, ha_type,
+                                  cap_warn, cap_crit, prov_cap_warn, prov_cap_crit)
 
-    return utils.get_response(c.to_dict()), 201
+    return utils.get_response(ret)
 
 
 @bp.route('/cluster', methods=['GET'], defaults={'uuid': None})
 @bp.route('/cluster/<string:uuid>', methods=['GET'])
 def list_clusters(uuid):
     clusters_list = []
     if uuid:
```

## Comparing `sbcli_mc-1.0.5/simplyblock_web/blueprints/caching_node_ops_k8s.py` & `sbcli_mc-1.0.6/simplyblock_web/blueprints/caching_node_ops_k8s.py`

 * *Files identical despite different names*

## Comparing `sbcli_mc-1.0.5/simplyblock_web/blueprints/node_api_caching_ks.py` & `sbcli_mc-1.0.6/simplyblock_web/blueprints/node_api_caching_ks.py`

 * *Files identical despite different names*

## Comparing `sbcli_mc-1.0.5/simplyblock_web/blueprints/node_api_caching_docker.py` & `sbcli_mc-1.0.6/simplyblock_web/blueprints/node_api_caching_docker.py`

 * *Files identical despite different names*

## Comparing `sbcli_mc-1.0.5/simplyblock_web/blueprints/web_api_caching_node.py` & `sbcli_mc-1.0.6/simplyblock_web/blueprints/web_api_caching_node.py`

 * *Files identical despite different names*

## Comparing `sbcli_mc-1.0.5/simplyblock_web/blueprints/node_api_basic.py` & `sbcli_mc-1.0.6/simplyblock_web/blueprints/node_api_basic.py`

 * *Files identical despite different names*

## Comparing `sbcli_mc-1.0.5/simplyblock_web/blueprints/csi.py` & `sbcli_mc-1.0.6/simplyblock_web/blueprints/csi.py`

 * *Files identical despite different names*

## Comparing `sbcli_mc-1.0.5/simplyblock_web/blueprints/web_api_mgmt_node.py` & `sbcli_mc-1.0.6/simplyblock_web/blueprints/web_api_mgmt_node.py`

 * *Files identical despite different names*

## Comparing `sbcli_mc-1.0.5/simplyblock_web/templates/deploy_spdk.yaml.j2` & `sbcli_mc-1.0.6/simplyblock_web/templates/deploy_spdk.yaml.j2`

 * *Files identical despite different names*

## Comparing `sbcli_mc-1.0.5/simplyblock_core/cluster_ops.py` & `sbcli_mc-1.0.6/simplyblock_core/cluster_ops.py`

 * *Files 2% similar despite different names*

```diff
@@ -15,14 +15,32 @@
 from simplyblock_core.models.cluster import Cluster
 from simplyblock_core.models.nvme_device import NVMeDevice
 from simplyblock_core.models.storage_node import StorageNode
 
 logger = logging.getLogger()
 
 
+def _add_grafana_dashboards(username, password, cluster_id):
+    url = f"http://${username}:${password}@0.0.0.0:3000/api/dashboards/import"
+    headers = {
+        'Content-Type': 'application/json',
+    }
+    dirpath, _, filenames = next(os.walk(os.path.join(constants.INSTALL_DIR, "scripts", "dashboards")))
+    for filename in filenames:
+        with open(os.path.join(dirpath, filename), 'r') as f:
+            st = f.read()
+            st = st.replace("$Cluster", cluster_id)
+        payload = json.dumps(st)
+        response = requests.post(url, headers=headers, data=payload)
+        logger.debug(response.status_code)
+        logger.debug(response.text)
+
+    return True
+
+
 def _add_graylog_input(cluster_ip, password):
     url = f"http://{cluster_ip}:9000/api/system/inputs"
     payload = json.dumps({
         "title": "spdk log input",
         "type": "org.graylog2.inputs.gelf.udp.GELFUDPInput",
         "configuration": {
             "bind_address": "0.0.0.0",
@@ -120,16 +138,16 @@
     c.write_to_db(db_controller.kv_store)
 
     cluster_events.cluster_create(c)
 
     mgmt_node_ops.add_mgmt_node(DEV_IP, c.uuid)
 
     logger.info("Applying dashboard...")
-    ret = scripts.apply_dashboard(c.secret)
-    logger.info("Applying dashboard > Done")
+    ret = _add_grafana_dashboards("admin", c.secret, c.uuid)
+    logger.info(f"Applying dashboard > {ret}")
 
     logger.info("New Cluster has been created")
     logger.info(c.uuid)
     return c.uuid
 
 
 # Deprecated
@@ -382,14 +400,20 @@
     if prov_cap_crit and prov_cap_crit > 0:
         cluster.prov_cap_crit = prov_cap_crit
 
     cluster.status = Cluster.STATUS_ACTIVE
     cluster.updated_at = int(time.time())
     cluster.write_to_db(db_controller.kv_store)
     cluster_events.cluster_create(cluster)
+
+    # todo: do it multi thread
+    logger.info("Applying dashboard...")
+    ret = _add_grafana_dashboards("admin", cluster.secret, cluster.uuid)
+    logger.info(f"Applying dashboard > {ret}")
+
     return cluster.get_id()
 
 
 def show_cluster(cl_id, is_json=False):
     db_controller = DBController()
     cluster = db_controller.get_cluster_by_id(cl_id)
     if not cluster:
```

## Comparing `sbcli_mc-1.0.5/simplyblock_core/pci_utils.py` & `sbcli_mc-1.0.6/simplyblock_core/pci_utils.py`

 * *Files identical despite different names*

## Comparing `sbcli_mc-1.0.5/simplyblock_core/snode_client.py` & `sbcli_mc-1.0.6/simplyblock_core/snode_client.py`

 * *Files identical despite different names*

## Comparing `sbcli_mc-1.0.5/simplyblock_core/kv_store.py` & `sbcli_mc-1.0.6/simplyblock_core/kv_store.py`

 * *Files identical despite different names*

## Comparing `sbcli_mc-1.0.5/simplyblock_core/compute_node_ops.py` & `sbcli_mc-1.0.6/simplyblock_core/compute_node_ops.py`

 * *Files identical despite different names*

## Comparing `sbcli_mc-1.0.5/simplyblock_core/rpc_client.py` & `sbcli_mc-1.0.6/simplyblock_core/rpc_client.py`

 * *Files identical despite different names*

## Comparing `sbcli_mc-1.0.5/simplyblock_core/mgmt_node_ops.py` & `sbcli_mc-1.0.6/simplyblock_core/mgmt_node_ops.py`

 * *Files identical despite different names*

## Comparing `sbcli_mc-1.0.5/simplyblock_core/utils.py` & `sbcli_mc-1.0.6/simplyblock_core/utils.py`

 * *Files identical despite different names*

## Comparing `sbcli_mc-1.0.5/simplyblock_core/distr_controller.py` & `sbcli_mc-1.0.6/simplyblock_core/distr_controller.py`

 * *Files identical despite different names*

## Comparing `sbcli_mc-1.0.5/simplyblock_core/cnode_client.py` & `sbcli_mc-1.0.6/simplyblock_core/cnode_client.py`

 * *Files identical despite different names*

## Comparing `sbcli_mc-1.0.5/simplyblock_core/storage_node_ops.py` & `sbcli_mc-1.0.6/simplyblock_core/storage_node_ops.py`

 * *Files identical despite different names*

## Comparing `sbcli_mc-1.0.5/simplyblock_core/constants.py` & `sbcli_mc-1.0.6/simplyblock_core/constants.py`

 * *Files 16% similar despite different names*

```diff
@@ -5,17 +5,15 @@
 KVD_DB_FILE_PATH = '/etc/foundationdb/fdb.cluster'
 KVD_DB_TIMEOUT_MS = 10000
 SPK_DIR = '/home/ec2-user/spdk'
 RPC_HTTP_PROXY_PORT = 8080
 LOG_LEVEL = logging.INFO
 LOG_WEB_DEBUG = True
 
-FILE_DIR = os.path.dirname(os.path.realpath(__file__))
-INSTALL_DIR = os.path.dirname(FILE_DIR)
-TOP_DIR = os.path.dirname(INSTALL_DIR)
+INSTALL_DIR = os.path.dirname(os.path.realpath(__file__))
 
 NODE_MONITOR_INTERVAL_SEC = 3
 DEVICE_MONITOR_INTERVAL_SEC = 5
 STAT_COLLECTOR_INTERVAL_SEC = 60*5  # 5 minutes
 LVOL_STAT_COLLECTOR_INTERVAL_SEC = 2
 LVOL_MONITOR_INTERVAL_SEC = 60
 DEV_MONITOR_INTERVAL_SEC = 10
```

## Comparing `sbcli_mc-1.0.5/simplyblock_core/services/job_tasks.py` & `sbcli_mc-1.0.6/simplyblock_core/services/job_tasks.py`

 * *Files identical despite different names*

## Comparing `sbcli_mc-1.0.5/simplyblock_core/services/caching_node_monitor.py` & `sbcli_mc-1.0.6/simplyblock_core/services/caching_node_monitor.py`

 * *Files identical despite different names*

## Comparing `sbcli_mc-1.0.5/simplyblock_core/services/install_service.sh` & `sbcli_mc-1.0.6/simplyblock_core/services/install_service.sh`

 * *Files identical despite different names*

## Comparing `sbcli_mc-1.0.5/simplyblock_core/services/__init__.py` & `sbcli_mc-1.0.6/simplyblock_core/services/__init__.py`

 * *Files identical despite different names*

## Comparing `sbcli_mc-1.0.5/simplyblock_core/services/log_agg_service.py` & `sbcli_mc-1.0.6/simplyblock_core/services/log_agg_service.py`

 * *Files identical despite different names*

## Comparing `sbcli_mc-1.0.5/simplyblock_core/services/health_check_service.py` & `sbcli_mc-1.0.6/simplyblock_core/services/health_check_service.py`

 * *Files identical despite different names*

## Comparing `sbcli_mc-1.0.5/simplyblock_core/services/capacity_and_stats_collector.py` & `sbcli_mc-1.0.6/simplyblock_core/services/capacity_and_stats_collector.py`

 * *Files identical despite different names*

## Comparing `sbcli_mc-1.0.5/simplyblock_core/services/device_monitor.py` & `sbcli_mc-1.0.6/simplyblock_core/services/device_monitor.py`

 * *Files identical despite different names*

## Comparing `sbcli_mc-1.0.5/simplyblock_core/services/lvol_stat_collector.py` & `sbcli_mc-1.0.6/simplyblock_core/services/lvol_stat_collector.py`

 * *Files identical despite different names*

## Comparing `sbcli_mc-1.0.5/simplyblock_core/services/cap_monitor.py` & `sbcli_mc-1.0.6/simplyblock_core/services/cap_monitor.py`

 * *Files identical despite different names*

## Comparing `sbcli_mc-1.0.5/simplyblock_core/services/storage_node_monitor.py` & `sbcli_mc-1.0.6/simplyblock_core/services/storage_node_monitor.py`

 * *Files identical despite different names*

## Comparing `sbcli_mc-1.0.5/simplyblock_core/services/port_stat_collector.py` & `sbcli_mc-1.0.6/simplyblock_core/services/port_stat_collector.py`

 * *Files identical despite different names*

## Comparing `sbcli_mc-1.0.5/simplyblock_core/services/distr_event_collector.py` & `sbcli_mc-1.0.6/simplyblock_core/services/distr_event_collector.py`

 * *Files identical despite different names*

## Comparing `sbcli_mc-1.0.5/simplyblock_core/services/mgmt_node_monitor.py` & `sbcli_mc-1.0.6/simplyblock_core/services/mgmt_node_monitor.py`

 * *Files identical despite different names*

## Comparing `sbcli_mc-1.0.5/simplyblock_core/services/lvol_monitor.py` & `sbcli_mc-1.0.6/simplyblock_core/services/lvol_monitor.py`

 * *Files identical despite different names*

## Comparing `sbcli_mc-1.0.5/simplyblock_core/controllers/pool_controller.py` & `sbcli_mc-1.0.6/simplyblock_core/controllers/pool_controller.py`

 * *Files identical despite different names*

## Comparing `sbcli_mc-1.0.5/simplyblock_core/controllers/storage_events.py` & `sbcli_mc-1.0.6/simplyblock_core/controllers/storage_events.py`

 * *Files identical despite different names*

## Comparing `sbcli_mc-1.0.5/simplyblock_core/controllers/lvol_controller.py` & `sbcli_mc-1.0.6/simplyblock_core/controllers/lvol_controller.py`

 * *Files identical despite different names*

## Comparing `sbcli_mc-1.0.5/simplyblock_core/controllers/device_events.py` & `sbcli_mc-1.0.6/simplyblock_core/controllers/device_events.py`

 * *Files identical despite different names*

## Comparing `sbcli_mc-1.0.5/simplyblock_core/controllers/lvol_events.py` & `sbcli_mc-1.0.6/simplyblock_core/controllers/lvol_events.py`

 * *Files identical despite different names*

## Comparing `sbcli_mc-1.0.5/simplyblock_core/controllers/snapshot_controller.py` & `sbcli_mc-1.0.6/simplyblock_core/controllers/snapshot_controller.py`

 * *Files identical despite different names*

## Comparing `sbcli_mc-1.0.5/simplyblock_core/controllers/snapshot_events.py` & `sbcli_mc-1.0.6/simplyblock_core/controllers/snapshot_events.py`

 * *Files identical despite different names*

## Comparing `sbcli_mc-1.0.5/simplyblock_core/controllers/events_controller.py` & `sbcli_mc-1.0.6/simplyblock_core/controllers/events_controller.py`

 * *Files identical despite different names*

## Comparing `sbcli_mc-1.0.5/simplyblock_core/controllers/health_controller.py` & `sbcli_mc-1.0.6/simplyblock_core/controllers/health_controller.py`

 * *Files identical despite different names*

## Comparing `sbcli_mc-1.0.5/simplyblock_core/controllers/device_controller.py` & `sbcli_mc-1.0.6/simplyblock_core/controllers/device_controller.py`

 * *Files identical despite different names*

## Comparing `sbcli_mc-1.0.5/simplyblock_core/controllers/pool_events.py` & `sbcli_mc-1.0.6/simplyblock_core/controllers/pool_events.py`

 * *Files identical despite different names*

## Comparing `sbcli_mc-1.0.5/simplyblock_core/controllers/caching_node_controller.py` & `sbcli_mc-1.0.6/simplyblock_core/controllers/caching_node_controller.py`

 * *Files identical despite different names*

## Comparing `sbcli_mc-1.0.5/simplyblock_core/controllers/cluster_events.py` & `sbcli_mc-1.0.6/simplyblock_core/controllers/cluster_events.py`

 * *Files identical despite different names*

## Comparing `sbcli_mc-1.0.5/simplyblock_core/controllers/mgmt_events.py` & `sbcli_mc-1.0.6/simplyblock_core/controllers/mgmt_events.py`

 * *Files identical despite different names*

## Comparing `sbcli_mc-1.0.5/simplyblock_core/models/caching_node.py` & `sbcli_mc-1.0.6/simplyblock_core/models/caching_node.py`

 * *Files identical despite different names*

## Comparing `sbcli_mc-1.0.5/simplyblock_core/models/nvme_device.py` & `sbcli_mc-1.0.6/simplyblock_core/models/nvme_device.py`

 * *Files identical despite different names*

## Comparing `sbcli_mc-1.0.5/simplyblock_core/models/mgmt_node.py` & `sbcli_mc-1.0.6/simplyblock_core/models/mgmt_node.py`

 * *Files identical despite different names*

## Comparing `sbcli_mc-1.0.5/simplyblock_core/models/compute_node.py` & `sbcli_mc-1.0.6/simplyblock_core/models/compute_node.py`

 * *Files identical despite different names*

## Comparing `sbcli_mc-1.0.5/simplyblock_core/models/events.py` & `sbcli_mc-1.0.6/simplyblock_core/models/events.py`

 * *Files identical despite different names*

## Comparing `sbcli_mc-1.0.5/simplyblock_core/models/global_settings.py` & `sbcli_mc-1.0.6/simplyblock_core/models/global_settings.py`

 * *Files identical despite different names*

## Comparing `sbcli_mc-1.0.5/simplyblock_core/models/job_schedule.py` & `sbcli_mc-1.0.6/simplyblock_core/models/job_schedule.py`

 * *Files identical despite different names*

## Comparing `sbcli_mc-1.0.5/simplyblock_core/models/base_model.py` & `sbcli_mc-1.0.6/simplyblock_core/models/base_model.py`

 * *Files identical despite different names*

## Comparing `sbcli_mc-1.0.5/simplyblock_core/models/lvol_model.py` & `sbcli_mc-1.0.6/simplyblock_core/models/lvol_model.py`

 * *Files identical despite different names*

## Comparing `sbcli_mc-1.0.5/simplyblock_core/models/snapshot.py` & `sbcli_mc-1.0.6/simplyblock_core/models/snapshot.py`

 * *Files identical despite different names*

## Comparing `sbcli_mc-1.0.5/simplyblock_core/models/storage_node.py` & `sbcli_mc-1.0.6/simplyblock_core/models/storage_node.py`

 * *Files identical despite different names*

## Comparing `sbcli_mc-1.0.5/simplyblock_core/models/stats.py` & `sbcli_mc-1.0.6/simplyblock_core/models/stats.py`

 * *Files identical despite different names*

## Comparing `sbcli_mc-1.0.5/simplyblock_core/models/pool.py` & `sbcli_mc-1.0.6/simplyblock_core/models/pool.py`

 * *Files identical despite different names*

## Comparing `sbcli_mc-1.0.5/simplyblock_core/models/iface.py` & `sbcli_mc-1.0.6/simplyblock_core/models/iface.py`

 * *Files identical despite different names*

## Comparing `sbcli_mc-1.0.5/simplyblock_core/models/cluster.py` & `sbcli_mc-1.0.6/simplyblock_core/models/cluster.py`

 * *Files identical despite different names*

## Comparing `sbcli_mc-1.0.5/simplyblock_core/models/port_stat.py` & `sbcli_mc-1.0.6/simplyblock_core/models/port_stat.py`

 * *Files identical despite different names*

## Comparing `sbcli_mc-1.0.5/simplyblock_core/scripts/install_deps.sh` & `sbcli_mc-1.0.6/simplyblock_core/scripts/install_deps.sh`

 * *Files identical despite different names*

## Comparing `sbcli_mc-1.0.5/simplyblock_core/scripts/__init__.py` & `sbcli_mc-1.0.6/simplyblock_core/scripts/__init__.py`

 * *Files 4% similar despite different names*

```diff
@@ -31,18 +31,14 @@
 
 
 def deploy_stack(cli_pass, dev_ip, image_name, graylog_password, cluster_id, log_del_interval, metrics_retention_period):
     pass_hash = hashlib.sha256(graylog_password.encode('utf-8')).hexdigest()
     return __run_script(
         ['sudo', 'bash', '-x', os.path.join(DIR_PATH, 'deploy_stack.sh'), cli_pass, dev_ip, image_name, pass_hash, graylog_password, cluster_id, log_del_interval, metrics_retention_period])
 
-def apply_dashboard(grafanaPassword):
-    return __run_script(
-        ['sudo', 'bash', '-x', os.path.join(DIR_PATH, 'apply_dashboard.sh'), grafanaPassword])
-
 
 def deploy_cleaner():
     return __run_script(['sudo', 'bash', '-x', os.path.join(DIR_PATH, 'clean_local_storage_deploy.sh')])
 
 
 def set_db_config(DEV_IP):
     return __run_script(['bash', os.path.join(DIR_PATH, 'set_db_config.sh'), DEV_IP])
```

## Comparing `sbcli_mc-1.0.5/simplyblock_core/scripts/haproxy.cfg` & `sbcli_mc-1.0.6/simplyblock_core/scripts/haproxy.cfg`

 * *Files identical despite different names*

## Comparing `sbcli_mc-1.0.5/simplyblock_core/scripts/stack_deploy_wait.sh` & `sbcli_mc-1.0.6/simplyblock_core/scripts/stack_deploy_wait.sh`

 * *Files identical despite different names*

## Comparing `sbcli_mc-1.0.5/simplyblock_core/scripts/docker-compose-swarm.yml` & `sbcli_mc-1.0.6/simplyblock_core/scripts/docker-compose-swarm.yml`

 * *Files identical despite different names*

## Comparing `sbcli_mc-1.0.5/simplyblock_core/scripts/docker-compose-swarm-monitoring.yml` & `sbcli_mc-1.0.6/simplyblock_core/scripts/docker-compose-swarm-monitoring.yml`

 * *Files identical despite different names*

## Comparing `sbcli_mc-1.0.5/simplyblock_core/scripts/deploy_stack.sh` & `sbcli_mc-1.0.6/simplyblock_core/scripts/deploy_stack.sh`

 * *Files identical despite different names*

## Comparing `sbcli_mc-1.0.5/simplyblock_core/scripts/alerting/alert_rules.yaml` & `sbcli_mc-1.0.6/simplyblock_core/scripts/alerting/alert_rules.yaml`

 * *Files identical despite different names*

## Comparing `sbcli_mc-1.0.5/simplyblock_core/scripts/alerting/alert_resources.yaml` & `sbcli_mc-1.0.6/simplyblock_core/scripts/alerting/alert_resources.yaml`

 * *Files identical despite different names*

## Comparing `sbcli_mc-1.0.5/simplyblock_core/scripts/dashboards/nodes.json` & `sbcli_mc-1.0.6/simplyblock_core/scripts/dashboards/nodes.json`

 * *Files identical despite different names*

## Comparing `sbcli_mc-1.0.5/simplyblock_core/scripts/dashboards/cluster.json` & `sbcli_mc-1.0.6/simplyblock_core/scripts/dashboards/devices.json`

 * *Files 3% similar despite different names*

### Pretty-printed

 * *Similarity: 0.9742784183239811%*

 * *Differences: {"'dashboard'": "{'panels': {1: {'targets': {0: {'expr': 'device_size_total'}}, 'title': "*

 * *                "'device_size_total'}, 2: {'targets': {0: {'expr': 'device_size_free'}}, 'title': "*

 * *                "'device_size_free'}, 3: {'gridPos': {'w': 8}, 'targets': {0: {'expr': "*

 * *                "'device_size_used'}}, 'title': 'device_size_used'}, 4: {'targets': {0: {'expr': "*

 * *                "'device_size_prov'}}, 'title': 'device_size_prov'}, 5: {'targets': {0: {'expr': "*

 * *                "'device_size_prov […]*

```diff
@@ -116,21 +116,21 @@
                 "targets": [
                     {
                         "datasource": {
                             "type": "prometheus",
                             "uid": "PBFA97CFB590B2093"
                         },
                         "editorMode": "builder",
-                        "expr": "cluster_size_total",
+                        "expr": "device_size_total",
                         "legendFormat": "__auto",
                         "range": true,
                         "refId": "A"
                     }
                 ],
-                "title": "cluster_size_total",
+                "title": "device_size_total",
                 "type": "timeseries"
             },
             {
                 "datasource": {
                     "type": "prometheus",
                     "uid": "PBFA97CFB590B2093"
                 },
@@ -209,21 +209,21 @@
                 "targets": [
                     {
                         "datasource": {
                             "type": "prometheus",
                             "uid": "PBFA97CFB590B2093"
                         },
                         "editorMode": "builder",
-                        "expr": "cluster_size_free",
+                        "expr": "device_size_free",
                         "legendFormat": "__auto",
                         "range": true,
                         "refId": "A"
                     }
                 ],
-                "title": "cluster_size_free",
+                "title": "device_size_free",
                 "type": "timeseries"
             },
             {
                 "datasource": {
                     "type": "prometheus",
                     "uid": "PBFA97CFB590B2093"
                 },
@@ -278,15 +278,15 @@
                         },
                         "unit": "bytes"
                     },
                     "overrides": []
                 },
                 "gridPos": {
                     "h": 7,
-                    "w": 7,
+                    "w": 8,
                     "x": 14,
                     "y": 1
                 },
                 "id": 14,
                 "options": {
                     "legend": {
                         "calcs": [],
@@ -302,21 +302,21 @@
                 "targets": [
                     {
                         "datasource": {
                             "type": "prometheus",
                             "uid": "PBFA97CFB590B2093"
                         },
                         "editorMode": "builder",
-                        "expr": "cluster_size_used",
+                        "expr": "device_size_used",
                         "legendFormat": "__auto",
                         "range": true,
                         "refId": "A"
                     }
                 ],
-                "title": "cluster_size_used",
+                "title": "device_size_used",
                 "type": "timeseries"
             },
             {
                 "datasource": {
                     "type": "prometheus",
                     "uid": "PBFA97CFB590B2093"
                 },
@@ -395,21 +395,21 @@
                 "targets": [
                     {
                         "datasource": {
                             "type": "prometheus",
                             "uid": "PBFA97CFB590B2093"
                         },
                         "editorMode": "builder",
-                        "expr": "cluster_size_prov",
+                        "expr": "device_size_prov",
                         "legendFormat": "__auto",
                         "range": true,
                         "refId": "A"
                     }
                 ],
-                "title": "cluster_size_prov",
+                "title": "device_size_prov",
                 "type": "timeseries"
             },
             {
                 "datasource": {
                     "type": "prometheus",
                     "uid": "PBFA97CFB590B2093"
                 },
@@ -488,21 +488,21 @@
                 "targets": [
                     {
                         "datasource": {
                             "type": "prometheus",
                             "uid": "PBFA97CFB590B2093"
                         },
                         "editorMode": "builder",
-                        "expr": "cluster_size_prov_util",
+                        "expr": "device_size_prov_util",
                         "legendFormat": "__auto",
                         "range": true,
                         "refId": "A"
                     }
                 ],
-                "title": "cluster_size_prov_util",
+                "title": "device_size_prov_util",
                 "type": "timeseries"
             },
             {
                 "datasource": {
                     "type": "prometheus",
                     "uid": "PBFA97CFB590B2093"
                 },
@@ -557,15 +557,15 @@
                         },
                         "unit": "percent"
                     },
                     "overrides": []
                 },
                 "gridPos": {
                     "h": 7,
-                    "w": 7,
+                    "w": 8,
                     "x": 14,
                     "y": 8
                 },
                 "id": 15,
                 "options": {
                     "legend": {
                         "calcs": [],
@@ -581,21 +581,21 @@
                 "targets": [
                     {
                         "datasource": {
                             "type": "prometheus",
                             "uid": "PBFA97CFB590B2093"
                         },
                         "editorMode": "builder",
-                        "expr": "cluster_size_util",
+                        "expr": "device_size_util",
                         "legendFormat": "__auto",
                         "range": true,
                         "refId": "A"
                     }
                 ],
-                "title": "cluster_size_util",
+                "title": "device_size_util",
                 "type": "timeseries"
             },
             {
                 "collapsed": false,
                 "gridPos": {
                     "h": 1,
                     "w": 24,
@@ -662,15 +662,15 @@
                             ]
                         },
                         "unit": "bytes"
                     },
                     "overrides": []
                 },
                 "gridPos": {
-                    "h": 7,
+                    "h": 8,
                     "w": 7,
                     "x": 0,
                     "y": 16
                 },
                 "id": 22,
                 "options": {
                     "legend": {
@@ -687,21 +687,21 @@
                 "targets": [
                     {
                         "datasource": {
                             "type": "prometheus",
                             "uid": "PBFA97CFB590B2093"
                         },
                         "editorMode": "builder",
-                        "expr": "cluster_write_bytes",
+                        "expr": "device_write_bytes",
                         "legendFormat": "__auto",
                         "range": true,
                         "refId": "A"
                     }
                 ],
-                "title": "cluster_write_bytes",
+                "title": "device_write_bytes",
                 "type": "timeseries"
             },
             {
                 "datasource": {
                     "type": "prometheus",
                     "uid": "PBFA97CFB590B2093"
                 },
@@ -750,20 +750,20 @@
                                 },
                                 {
                                     "color": "red",
                                     "value": 80
                                 }
                             ]
                         },
-                        "unit": "binBps"
+                        "unit": "bytes"
                     },
                     "overrides": []
                 },
                 "gridPos": {
-                    "h": 7,
+                    "h": 8,
                     "w": 7,
                     "x": 7,
                     "y": 16
                 },
                 "id": 23,
                 "options": {
                     "legend": {
@@ -780,15 +780,15 @@
                 "targets": [
                     {
                         "datasource": {
                             "type": "prometheus",
                             "uid": "PBFA97CFB590B2093"
                         },
                         "editorMode": "builder",
-                        "expr": "cluster_write_bytes_ps",
+                        "expr": "device_write_bytes_ps",
                         "legendFormat": "__auto",
                         "range": true,
                         "refId": "A"
                     }
                 ],
                 "title": "write_speed",
                 "type": "timeseries"
@@ -848,16 +848,16 @@
                             ]
                         },
                         "unit": "\u00b5s"
                     },
                     "overrides": []
                 },
                 "gridPos": {
-                    "h": 7,
-                    "w": 7,
+                    "h": 8,
+                    "w": 8,
                     "x": 14,
                     "y": 16
                 },
                 "id": 26,
                 "options": {
                     "legend": {
                         "calcs": [],
@@ -873,21 +873,21 @@
                 "targets": [
                     {
                         "datasource": {
                             "type": "prometheus",
                             "uid": "PBFA97CFB590B2093"
                         },
                         "editorMode": "builder",
-                        "expr": "cluster_write_latency_ps / 1000",
+                        "expr": "device_write_latency_ps / 1000",
                         "legendFormat": "__auto",
                         "range": true,
                         "refId": "A"
                     }
                 ],
-                "title": "cluster_write_latency_ps",
+                "title": "device_write_latency_ps",
                 "type": "timeseries"
             },
             {
                 "datasource": {
                     "type": "prometheus",
                     "uid": "PBFA97CFB590B2093"
                 },
@@ -940,18 +940,18 @@
                                 }
                             ]
                         }
                     },
                     "overrides": []
                 },
                 "gridPos": {
-                    "h": 7,
+                    "h": 8,
                     "w": 7,
                     "x": 0,
-                    "y": 23
+                    "y": 24
                 },
                 "id": 24,
                 "options": {
                     "legend": {
                         "calcs": [],
                         "displayMode": "list",
                         "placement": "bottom",
@@ -965,21 +965,21 @@
                 "targets": [
                     {
                         "datasource": {
                             "type": "prometheus",
                             "uid": "PBFA97CFB590B2093"
                         },
                         "editorMode": "builder",
-                        "expr": "cluster_write_io",
+                        "expr": "device_write_io",
                         "legendFormat": "__auto",
                         "range": true,
                         "refId": "A"
                     }
                 ],
-                "title": "cluster_write_io",
+                "title": "device_write_io",
                 "type": "timeseries"
             },
             {
                 "datasource": {
                     "type": "prometheus",
                     "uid": "PBFA97CFB590B2093"
                 },
@@ -1032,18 +1032,18 @@
                                 }
                             ]
                         }
                     },
                     "overrides": []
                 },
                 "gridPos": {
-                    "h": 7,
+                    "h": 8,
                     "w": 7,
                     "x": 7,
-                    "y": 23
+                    "y": 24
                 },
                 "id": 25,
                 "options": {
                     "legend": {
                         "calcs": [],
                         "displayMode": "list",
                         "placement": "bottom",
@@ -1057,15 +1057,15 @@
                 "targets": [
                     {
                         "datasource": {
                             "type": "prometheus",
                             "uid": "PBFA97CFB590B2093"
                         },
                         "editorMode": "builder",
-                        "expr": "cluster_write_io_ps",
+                        "expr": "device_write_io_ps",
                         "legendFormat": "__auto",
                         "range": true,
                         "refId": "A"
                     }
                 ],
                 "title": "write_iops",
                 "type": "timeseries"
@@ -1124,18 +1124,18 @@
                                 }
                             ]
                         }
                     },
                     "overrides": []
                 },
                 "gridPos": {
-                    "h": 7,
-                    "w": 7,
+                    "h": 8,
+                    "w": 8,
                     "x": 14,
-                    "y": 23
+                    "y": 24
                 },
                 "id": 33,
                 "options": {
                     "legend": {
                         "calcs": [],
                         "displayMode": "list",
                         "placement": "bottom",
@@ -1149,30 +1149,30 @@
                 "targets": [
                     {
                         "datasource": {
                             "type": "prometheus",
                             "uid": "PBFA97CFB590B2093"
                         },
                         "editorMode": "builder",
-                        "expr": "cluster_write_latency_ticks",
+                        "expr": "device_write_latency_ticks",
                         "legendFormat": "__auto",
                         "range": true,
                         "refId": "A"
                     }
                 ],
-                "title": "cluster_wite_latency_ticks",
+                "title": "device_wite_latency_ticks",
                 "type": "timeseries"
             },
             {
                 "collapsed": false,
                 "gridPos": {
                     "h": 1,
                     "w": 24,
                     "x": 0,
-                    "y": 30
+                    "y": 32
                 },
                 "id": 30,
                 "panels": [],
                 "title": "Reads",
                 "type": "row"
             },
             {
@@ -1233,15 +1233,15 @@
                     },
                     "overrides": []
                 },
                 "gridPos": {
                     "h": 8,
                     "w": 7,
                     "x": 0,
-                    "y": 31
+                    "y": 33
                 },
                 "id": 1,
                 "options": {
                     "legend": {
                         "calcs": [],
                         "displayMode": "list",
                         "placement": "bottom",
@@ -1255,21 +1255,21 @@
                 "targets": [
                     {
                         "datasource": {
                             "type": "prometheus",
                             "uid": "PBFA97CFB590B2093"
                         },
                         "editorMode": "builder",
-                        "expr": "cluster_read_bytes",
+                        "expr": "device_read_bytes",
                         "legendFormat": "__auto",
                         "range": true,
                         "refId": "A"
                     }
                 ],
-                "title": "cluster_read_bytes",
+                "title": "device_read_bytes",
                 "type": "timeseries"
             },
             {
                 "datasource": {
                     "type": "prometheus",
                     "uid": "PBFA97CFB590B2093"
                 },
@@ -1326,15 +1326,15 @@
                     },
                     "overrides": []
                 },
                 "gridPos": {
                     "h": 8,
                     "w": 7,
                     "x": 7,
-                    "y": 31
+                    "y": 33
                 },
                 "id": 2,
                 "options": {
                     "legend": {
                         "calcs": [],
                         "displayMode": "list",
                         "placement": "bottom",
@@ -1348,15 +1348,15 @@
                 "targets": [
                     {
                         "datasource": {
                             "type": "prometheus",
                             "uid": "PBFA97CFB590B2093"
                         },
                         "editorMode": "builder",
-                        "expr": "cluster_read_bytes_ps",
+                        "expr": "device_read_bytes_ps",
                         "legendFormat": "__auto",
                         "range": true,
                         "refId": "A"
                     }
                 ],
                 "title": "read_speed",
                 "type": "timeseries"
@@ -1417,17 +1417,17 @@
                         },
                         "unit": "\u00b5s"
                     },
                     "overrides": []
                 },
                 "gridPos": {
                     "h": 8,
-                    "w": 7,
+                    "w": 8,
                     "x": 14,
-                    "y": 31
+                    "y": 33
                 },
                 "id": 5,
                 "options": {
                     "legend": {
                         "calcs": [],
                         "displayMode": "list",
                         "placement": "bottom",
@@ -1441,21 +1441,21 @@
                 "targets": [
                     {
                         "datasource": {
                             "type": "prometheus",
                             "uid": "PBFA97CFB590B2093"
                         },
                         "editorMode": "builder",
-                        "expr": "cluster_read_latency_ps",
+                        "expr": "device_read_latency_ps",
                         "legendFormat": "__auto",
                         "range": true,
                         "refId": "A"
                     }
                 ],
-                "title": "cluster_read_latency_ps",
+                "title": "device_read_latency_ps",
                 "type": "timeseries"
             },
             {
                 "datasource": {
                     "type": "prometheus",
                     "uid": "PBFA97CFB590B2093"
                 },
@@ -1511,15 +1511,15 @@
                     },
                     "overrides": []
                 },
                 "gridPos": {
                     "h": 7,
                     "w": 7,
                     "x": 0,
-                    "y": 39
+                    "y": 41
                 },
                 "id": 3,
                 "options": {
                     "legend": {
                         "calcs": [],
                         "displayMode": "list",
                         "placement": "bottom",
@@ -1533,21 +1533,21 @@
                 "targets": [
                     {
                         "datasource": {
                             "type": "prometheus",
                             "uid": "PBFA97CFB590B2093"
                         },
                         "editorMode": "builder",
-                        "expr": "cluster_read_io",
+                        "expr": "device_read_io",
                         "legendFormat": "__auto",
                         "range": true,
                         "refId": "A"
                     }
                 ],
-                "title": "cluster_read_io",
+                "title": "device_read_io",
                 "type": "timeseries"
             },
             {
                 "datasource": {
                     "type": "prometheus",
                     "uid": "PBFA97CFB590B2093"
                 },
@@ -1603,15 +1603,15 @@
                     },
                     "overrides": []
                 },
                 "gridPos": {
                     "h": 7,
                     "w": 7,
                     "x": 7,
-                    "y": 39
+                    "y": 41
                 },
                 "id": 4,
                 "options": {
                     "legend": {
                         "calcs": [],
                         "displayMode": "list",
                         "placement": "bottom",
@@ -1625,15 +1625,15 @@
                 "targets": [
                     {
                         "datasource": {
                             "type": "prometheus",
                             "uid": "PBFA97CFB590B2093"
                         },
                         "editorMode": "builder",
-                        "expr": "cluster_read_io_ps",
+                        "expr": "device_read_io_ps",
                         "legendFormat": "__auto",
                         "range": true,
                         "refId": "A"
                     }
                 ],
                 "title": "read_iops",
                 "type": "timeseries"
@@ -1693,17 +1693,17 @@
                             ]
                         }
                     },
                     "overrides": []
                 },
                 "gridPos": {
                     "h": 7,
-                    "w": 7,
+                    "w": 8,
                     "x": 14,
-                    "y": 39
+                    "y": 41
                 },
                 "id": 6,
                 "options": {
                     "legend": {
                         "calcs": [],
                         "displayMode": "list",
                         "placement": "bottom",
@@ -1717,30 +1717,30 @@
                 "targets": [
                     {
                         "datasource": {
                             "type": "prometheus",
                             "uid": "PBFA97CFB590B2093"
                         },
                         "editorMode": "builder",
-                        "expr": "cluster_read_latency_ticks",
+                        "expr": "device_read_latency_ticks",
                         "legendFormat": "__auto",
                         "range": true,
                         "refId": "A"
                     }
                 ],
-                "title": "cluster_read_latency_ticks",
+                "title": "device_read_latency_ticks",
                 "type": "timeseries"
             },
             {
                 "collapsed": false,
                 "gridPos": {
                     "h": 1,
                     "w": 24,
                     "x": 0,
-                    "y": 46
+                    "y": 48
                 },
                 "id": 29,
                 "panels": [],
                 "title": "unmap",
                 "type": "row"
             },
             {
@@ -1800,15 +1800,15 @@
                     },
                     "overrides": []
                 },
                 "gridPos": {
                     "h": 7,
                     "w": 7,
                     "x": 0,
-                    "y": 47
+                    "y": 49
                 },
                 "id": 21,
                 "options": {
                     "legend": {
                         "calcs": [],
                         "displayMode": "list",
                         "placement": "bottom",
@@ -1822,21 +1822,21 @@
                 "targets": [
                     {
                         "datasource": {
                             "type": "prometheus",
                             "uid": "PBFA97CFB590B2093"
                         },
                         "editorMode": "builder",
-                        "expr": "cluster_unmap_latency_ticks",
+                        "expr": "device_unmap_latency_ticks",
                         "legendFormat": "__auto",
                         "range": true,
                         "refId": "A"
                     }
                 ],
-                "title": "cluster_unmap_latency_ticks",
+                "title": "device_unmap_latency_ticks",
                 "type": "timeseries"
             },
             {
                 "datasource": {
                     "type": "prometheus",
                     "uid": "PBFA97CFB590B2093"
                 },
@@ -1893,15 +1893,15 @@
                     },
                     "overrides": []
                 },
                 "gridPos": {
                     "h": 7,
                     "w": 7,
                     "x": 7,
-                    "y": 47
+                    "y": 49
                 },
                 "id": 17,
                 "options": {
                     "legend": {
                         "calcs": [],
                         "displayMode": "list",
                         "placement": "bottom",
@@ -1915,21 +1915,21 @@
                 "targets": [
                     {
                         "datasource": {
                             "type": "prometheus",
                             "uid": "PBFA97CFB590B2093"
                         },
                         "editorMode": "builder",
-                        "expr": "cluster_unmap_bytes_ps",
+                        "expr": "device_unmap_bytes_ps",
                         "legendFormat": "__auto",
                         "range": true,
                         "refId": "A"
                     }
                 ],
-                "title": "cluster_unmap_bytes_ps",
+                "title": "device_unmap_bytes_ps",
                 "type": "timeseries"
             },
             {
                 "datasource": {
                     "type": "prometheus",
                     "uid": "PBFA97CFB590B2093"
                 },
@@ -1985,17 +1985,17 @@
                         },
                         "unit": "\u00b5s"
                     },
                     "overrides": []
                 },
                 "gridPos": {
                     "h": 7,
-                    "w": 7,
+                    "w": 8,
                     "x": 14,
-                    "y": 47
+                    "y": 49
                 },
                 "id": 20,
                 "options": {
                     "legend": {
                         "calcs": [],
                         "displayMode": "list",
                         "placement": "bottom",
@@ -2009,21 +2009,21 @@
                 "targets": [
                     {
                         "datasource": {
                             "type": "prometheus",
                             "uid": "PBFA97CFB590B2093"
                         },
                         "editorMode": "builder",
-                        "expr": "cluster_unmap_latency_ps",
+                        "expr": "device_unmap_latency_ps",
                         "legendFormat": "__auto",
                         "range": true,
                         "refId": "A"
                     }
                 ],
-                "title": "cluster_unmap_latency_ps",
+                "title": "device_unmap_latency_ps",
                 "type": "timeseries"
             },
             {
                 "datasource": {
                     "type": "prometheus",
                     "uid": "PBFA97CFB590B2093"
                 },
@@ -2081,15 +2081,15 @@
                         {
                             "__systemRef": "hideSeriesFrom",
                             "matcher": {
                                 "id": "byNames",
                                 "options": {
                                     "mode": "exclude",
                                     "names": [
-                                        "{__name__=\"cluster_unmap_io_ps\", cluster=\"c3663938-6610-44d5-9897-d7bfa60a43e1\", exported_job=\"collector\", instance=\"192.168.178.52:9091\", job=\"metricsgateway\"}"
+                                        "{__name__=\"device_unmap_io_ps\", cluster=\"c3663938-6610-44d5-9897-d7bfa60a43e1\", exported_job=\"collector\", instance=\"192.168.178.52:9091\", job=\"metricsgateway\"}"
                                     ],
                                     "prefix": "All except:",
                                     "readOnly": true
                                 }
                             },
                             "properties": [
                                 {
@@ -2104,15 +2104,15 @@
                         }
                     ]
                 },
                 "gridPos": {
                     "h": 7,
                     "w": 7,
                     "x": 0,
-                    "y": 54
+                    "y": 56
                 },
                 "id": 19,
                 "options": {
                     "legend": {
                         "calcs": [],
                         "displayMode": "list",
                         "placement": "bottom",
@@ -2126,21 +2126,21 @@
                 "targets": [
                     {
                         "datasource": {
                             "type": "prometheus",
                             "uid": "PBFA97CFB590B2093"
                         },
                         "editorMode": "builder",
-                        "expr": "cluster_unmap_io_ps",
+                        "expr": "device_unmap_io_ps",
                         "legendFormat": "__auto",
                         "range": true,
                         "refId": "A"
                     }
                 ],
-                "title": "cluster_unmap_io_ps",
+                "title": "device_unmap_io_ps",
                 "type": "timeseries"
             },
             {
                 "datasource": {
                     "type": "prometheus",
                     "uid": "PBFA97CFB590B2093"
                 },
@@ -2196,15 +2196,15 @@
                     },
                     "overrides": []
                 },
                 "gridPos": {
                     "h": 7,
                     "w": 7,
                     "x": 7,
-                    "y": 54
+                    "y": 56
                 },
                 "id": 18,
                 "options": {
                     "legend": {
                         "calcs": [],
                         "displayMode": "list",
                         "placement": "bottom",
@@ -2218,21 +2218,21 @@
                 "targets": [
                     {
                         "datasource": {
                             "type": "prometheus",
                             "uid": "PBFA97CFB590B2093"
                         },
                         "editorMode": "builder",
-                        "expr": "cluster_unmap_io",
+                        "expr": "device_unmap_io",
                         "legendFormat": "__auto",
                         "range": true,
                         "refId": "A"
                     }
                 ],
-                "title": "cluster_unmap_io",
+                "title": "device_unmap_io",
                 "type": "timeseries"
             },
             {
                 "datasource": {
                     "type": "prometheus",
                     "uid": "PBFA97CFB590B2093"
                 },
@@ -2281,23 +2281,23 @@
                                 },
                                 {
                                     "color": "red",
                                     "value": 80
                                 }
                             ]
                         },
-                        "unit": "bytes"
+                        "unit": "decbytes"
                     },
                     "overrides": []
                 },
                 "gridPos": {
                     "h": 7,
-                    "w": 7,
+                    "w": 8,
                     "x": 14,
-                    "y": 54
+                    "y": 56
                 },
                 "id": 16,
                 "options": {
                     "legend": {
                         "calcs": [],
                         "displayMode": "list",
                         "placement": "bottom",
@@ -2311,21 +2311,21 @@
                 "targets": [
                     {
                         "datasource": {
                             "type": "prometheus",
                             "uid": "PBFA97CFB590B2093"
                         },
                         "editorMode": "builder",
-                        "expr": "cluster_unmap_bytes",
+                        "expr": "device_unmap_bytes",
                         "legendFormat": "__auto",
                         "range": true,
                         "refId": "A"
                     }
                 ],
-                "title": "cluster_unmap_bytes",
+                "title": "device_unmap_bytes",
                 "type": "timeseries"
             }
         ],
         "refresh": "",
         "schemaVersion": 38,
         "style": "dark",
         "tags": [],
@@ -2334,13 +2334,13 @@
         },
         "time": {
             "from": "now-1h",
             "to": "now"
         },
         "timepicker": {},
         "timezone": "",
-        "title": "ClusterDashboard",
-        "uid": "d56e0ae7-48d5-481d-a2ea-3192da4d9e39",
+        "title": "DevicesDashboard",
+        "uid": "d56e0ae7-48d5-481d-a2ea-3192da4d9e38",
         "version": 5,
         "weekStart": ""
     }
 }
```

## Comparing `sbcli_mc-1.0.5/simplyblock_core/scripts/dashboards/lvols.json` & `sbcli_mc-1.0.6/simplyblock_core/scripts/dashboards/lvols.json`

 * *Files identical despite different names*

## Comparing `sbcli_mc-1.0.5/simplyblock_core/scripts/dashboards/devices.json` & `sbcli_mc-1.0.6/simplyblock_core/scripts/dashboards/pools.json`

 * *Files 6% similar despite different names*

### Pretty-printed

 * *Similarity: 0.9728189334162959%*

 * *Differences: {"'dashboard'": "{'panels': {1: {'fieldConfig': {'defaults': {'unit': 'decbytes'}}, 'targets': {0: "*

 * *                "{'expr': 'pool_size_total'}}, 'title': 'pool_size_total'}, 2: {'fieldConfig': "*

 * *                "{'defaults': {'unit': 'decbytes'}}, 'targets': {0: {'expr': 'pool_size_free'}}, "*

 * *                "'title': 'pool_size_free'}, 3: {'fieldConfig': {'defaults': {'unit': "*

 * *                "'decbytes'}}, 'gridPos': {'w': 7}, 'targets': {0: {'expr': 'pool_size_used'}}, "*

 * *                "'title': 'po […]*

```diff
@@ -86,15 +86,15 @@
                                 },
                                 {
                                     "color": "red",
                                     "value": 80
                                 }
                             ]
                         },
-                        "unit": "bytes"
+                        "unit": "decbytes"
                     },
                     "overrides": []
                 },
                 "gridPos": {
                     "h": 7,
                     "w": 7,
                     "x": 0,
@@ -116,21 +116,21 @@
                 "targets": [
                     {
                         "datasource": {
                             "type": "prometheus",
                             "uid": "PBFA97CFB590B2093"
                         },
                         "editorMode": "builder",
-                        "expr": "device_size_total",
+                        "expr": "pool_size_total",
                         "legendFormat": "__auto",
                         "range": true,
                         "refId": "A"
                     }
                 ],
-                "title": "device_size_total",
+                "title": "pool_size_total",
                 "type": "timeseries"
             },
             {
                 "datasource": {
                     "type": "prometheus",
                     "uid": "PBFA97CFB590B2093"
                 },
@@ -179,15 +179,15 @@
                                 },
                                 {
                                     "color": "red",
                                     "value": 80
                                 }
                             ]
                         },
-                        "unit": "bytes"
+                        "unit": "decbytes"
                     },
                     "overrides": []
                 },
                 "gridPos": {
                     "h": 7,
                     "w": 7,
                     "x": 7,
@@ -209,21 +209,21 @@
                 "targets": [
                     {
                         "datasource": {
                             "type": "prometheus",
                             "uid": "PBFA97CFB590B2093"
                         },
                         "editorMode": "builder",
-                        "expr": "device_size_free",
+                        "expr": "pool_size_free",
                         "legendFormat": "__auto",
                         "range": true,
                         "refId": "A"
                     }
                 ],
-                "title": "device_size_free",
+                "title": "pool_size_free",
                 "type": "timeseries"
             },
             {
                 "datasource": {
                     "type": "prometheus",
                     "uid": "PBFA97CFB590B2093"
                 },
@@ -272,21 +272,21 @@
                                 },
                                 {
                                     "color": "red",
                                     "value": 80
                                 }
                             ]
                         },
-                        "unit": "bytes"
+                        "unit": "decbytes"
                     },
                     "overrides": []
                 },
                 "gridPos": {
                     "h": 7,
-                    "w": 8,
+                    "w": 7,
                     "x": 14,
                     "y": 1
                 },
                 "id": 14,
                 "options": {
                     "legend": {
                         "calcs": [],
@@ -302,21 +302,21 @@
                 "targets": [
                     {
                         "datasource": {
                             "type": "prometheus",
                             "uid": "PBFA97CFB590B2093"
                         },
                         "editorMode": "builder",
-                        "expr": "device_size_used",
+                        "expr": "pool_size_used",
                         "legendFormat": "__auto",
                         "range": true,
                         "refId": "A"
                     }
                 ],
-                "title": "device_size_used",
+                "title": "pool_size_used",
                 "type": "timeseries"
             },
             {
                 "datasource": {
                     "type": "prometheus",
                     "uid": "PBFA97CFB590B2093"
                 },
@@ -365,15 +365,15 @@
                                 },
                                 {
                                     "color": "red",
                                     "value": 80
                                 }
                             ]
                         },
-                        "unit": "bytes"
+                        "unit": "decbytes"
                     },
                     "overrides": []
                 },
                 "gridPos": {
                     "h": 7,
                     "w": 7,
                     "x": 0,
@@ -395,21 +395,21 @@
                 "targets": [
                     {
                         "datasource": {
                             "type": "prometheus",
                             "uid": "PBFA97CFB590B2093"
                         },
                         "editorMode": "builder",
-                        "expr": "device_size_prov",
+                        "expr": "pool_size_prov",
                         "legendFormat": "__auto",
                         "range": true,
                         "refId": "A"
                     }
                 ],
-                "title": "device_size_prov",
+                "title": "pool_size_prov",
                 "type": "timeseries"
             },
             {
                 "datasource": {
                     "type": "prometheus",
                     "uid": "PBFA97CFB590B2093"
                 },
@@ -458,15 +458,15 @@
                                 },
                                 {
                                     "color": "red",
                                     "value": 80
                                 }
                             ]
                         },
-                        "unit": "percent"
+                        "unit": "decbytes"
                     },
                     "overrides": []
                 },
                 "gridPos": {
                     "h": 7,
                     "w": 7,
                     "x": 7,
@@ -488,21 +488,21 @@
                 "targets": [
                     {
                         "datasource": {
                             "type": "prometheus",
                             "uid": "PBFA97CFB590B2093"
                         },
                         "editorMode": "builder",
-                        "expr": "device_size_prov_util",
+                        "expr": "pool_size_prov_util",
                         "legendFormat": "__auto",
                         "range": true,
                         "refId": "A"
                     }
                 ],
-                "title": "device_size_prov_util",
+                "title": "pool_size_prov_util",
                 "type": "timeseries"
             },
             {
                 "datasource": {
                     "type": "prometheus",
                     "uid": "PBFA97CFB590B2093"
                 },
@@ -551,21 +551,21 @@
                                 },
                                 {
                                     "color": "red",
                                     "value": 80
                                 }
                             ]
                         },
-                        "unit": "percent"
+                        "unit": "decbytes"
                     },
                     "overrides": []
                 },
                 "gridPos": {
                     "h": 7,
-                    "w": 8,
+                    "w": 7,
                     "x": 14,
                     "y": 8
                 },
                 "id": 15,
                 "options": {
                     "legend": {
                         "calcs": [],
@@ -581,21 +581,21 @@
                 "targets": [
                     {
                         "datasource": {
                             "type": "prometheus",
                             "uid": "PBFA97CFB590B2093"
                         },
                         "editorMode": "builder",
-                        "expr": "device_size_util",
+                        "expr": "pool_size_util",
                         "legendFormat": "__auto",
                         "range": true,
                         "refId": "A"
                     }
                 ],
-                "title": "device_size_util",
+                "title": "pool_size_util",
                 "type": "timeseries"
             },
             {
                 "collapsed": false,
                 "gridPos": {
                     "h": 1,
                     "w": 24,
@@ -657,15 +657,15 @@
                                 },
                                 {
                                     "color": "red",
                                     "value": 80
                                 }
                             ]
                         },
-                        "unit": "bytes"
+                        "unit": "decbytes"
                     },
                     "overrides": []
                 },
                 "gridPos": {
                     "h": 8,
                     "w": 7,
                     "x": 0,
@@ -687,21 +687,21 @@
                 "targets": [
                     {
                         "datasource": {
                             "type": "prometheus",
                             "uid": "PBFA97CFB590B2093"
                         },
                         "editorMode": "builder",
-                        "expr": "device_write_bytes",
+                        "expr": "pool_write_bytes",
                         "legendFormat": "__auto",
                         "range": true,
                         "refId": "A"
                     }
                 ],
-                "title": "device_write_bytes",
+                "title": "pool_write_bytes",
                 "type": "timeseries"
             },
             {
                 "datasource": {
                     "type": "prometheus",
                     "uid": "PBFA97CFB590B2093"
                 },
@@ -750,15 +750,15 @@
                                 },
                                 {
                                     "color": "red",
                                     "value": 80
                                 }
                             ]
                         },
-                        "unit": "bytes"
+                        "unit": "Bps"
                     },
                     "overrides": []
                 },
                 "gridPos": {
                     "h": 8,
                     "w": 7,
                     "x": 7,
@@ -780,15 +780,15 @@
                 "targets": [
                     {
                         "datasource": {
                             "type": "prometheus",
                             "uid": "PBFA97CFB590B2093"
                         },
                         "editorMode": "builder",
-                        "expr": "device_write_bytes_ps",
+                        "expr": "pool_write_bytes_ps",
                         "legendFormat": "__auto",
                         "range": true,
                         "refId": "A"
                     }
                 ],
                 "title": "write_speed",
                 "type": "timeseries"
@@ -842,26 +842,25 @@
                                     "value": null
                                 },
                                 {
                                     "color": "red",
                                     "value": 80
                                 }
                             ]
-                        },
-                        "unit": "\u00b5s"
+                        }
                     },
                     "overrides": []
                 },
                 "gridPos": {
                     "h": 8,
-                    "w": 8,
+                    "w": 7,
                     "x": 14,
                     "y": 16
                 },
-                "id": 26,
+                "id": 33,
                 "options": {
                     "legend": {
                         "calcs": [],
                         "displayMode": "list",
                         "placement": "bottom",
                         "showLegend": true
                     },
@@ -873,21 +872,21 @@
                 "targets": [
                     {
                         "datasource": {
                             "type": "prometheus",
                             "uid": "PBFA97CFB590B2093"
                         },
                         "editorMode": "builder",
-                        "expr": "device_write_latency_ps / 1000",
+                        "expr": "pool_write_latency_ticks",
                         "legendFormat": "__auto",
                         "range": true,
                         "refId": "A"
                     }
                 ],
-                "title": "device_write_latency_ps",
+                "title": "pool_wite_latency_ticks",
                 "type": "timeseries"
             },
             {
                 "datasource": {
                     "type": "prometheus",
                     "uid": "PBFA97CFB590B2093"
                 },
@@ -965,21 +964,21 @@
                 "targets": [
                     {
                         "datasource": {
                             "type": "prometheus",
                             "uid": "PBFA97CFB590B2093"
                         },
                         "editorMode": "builder",
-                        "expr": "device_write_io",
+                        "expr": "pool_write_io",
                         "legendFormat": "__auto",
                         "range": true,
                         "refId": "A"
                     }
                 ],
-                "title": "device_write_io",
+                "title": "pool_write_io",
                 "type": "timeseries"
             },
             {
                 "datasource": {
                     "type": "prometheus",
                     "uid": "PBFA97CFB590B2093"
                 },
@@ -1057,15 +1056,15 @@
                 "targets": [
                     {
                         "datasource": {
                             "type": "prometheus",
                             "uid": "PBFA97CFB590B2093"
                         },
                         "editorMode": "builder",
-                        "expr": "device_write_io_ps",
+                        "expr": "pool_write_io_ps",
                         "legendFormat": "__auto",
                         "range": true,
                         "refId": "A"
                     }
                 ],
                 "title": "write_iops",
                 "type": "timeseries"
@@ -1119,25 +1118,26 @@
                                     "value": null
                                 },
                                 {
                                     "color": "red",
                                     "value": 80
                                 }
                             ]
-                        }
+                        },
+                        "unit": "ns"
                     },
                     "overrides": []
                 },
                 "gridPos": {
                     "h": 8,
-                    "w": 8,
+                    "w": 7,
                     "x": 14,
                     "y": 24
                 },
-                "id": 33,
+                "id": 26,
                 "options": {
                     "legend": {
                         "calcs": [],
                         "displayMode": "list",
                         "placement": "bottom",
                         "showLegend": true
                     },
@@ -1149,21 +1149,21 @@
                 "targets": [
                     {
                         "datasource": {
                             "type": "prometheus",
                             "uid": "PBFA97CFB590B2093"
                         },
                         "editorMode": "builder",
-                        "expr": "device_write_latency_ticks",
+                        "expr": "pool_write_latency_ps / 1000",
                         "legendFormat": "__auto",
                         "range": true,
                         "refId": "A"
                     }
                 ],
-                "title": "device_wite_latency_ticks",
+                "title": "pool_write_latency_ps",
                 "type": "timeseries"
             },
             {
                 "collapsed": false,
                 "gridPos": {
                     "h": 1,
                     "w": 24,
@@ -1225,15 +1225,15 @@
                                 },
                                 {
                                     "color": "red",
                                     "value": 80
                                 }
                             ]
                         },
-                        "unit": "bytes"
+                        "unit": "decbytes"
                     },
                     "overrides": []
                 },
                 "gridPos": {
                     "h": 8,
                     "w": 7,
                     "x": 0,
@@ -1255,21 +1255,21 @@
                 "targets": [
                     {
                         "datasource": {
                             "type": "prometheus",
                             "uid": "PBFA97CFB590B2093"
                         },
                         "editorMode": "builder",
-                        "expr": "device_read_bytes",
+                        "expr": "pool_read_bytes",
                         "legendFormat": "__auto",
                         "range": true,
                         "refId": "A"
                     }
                 ],
-                "title": "device_read_bytes",
+                "title": "pool_read_bytes",
                 "type": "timeseries"
             },
             {
                 "datasource": {
                     "type": "prometheus",
                     "uid": "PBFA97CFB590B2093"
                 },
@@ -1318,15 +1318,15 @@
                                 },
                                 {
                                     "color": "red",
                                     "value": 80
                                 }
                             ]
                         },
-                        "unit": "bytes"
+                        "unit": "Bps"
                     },
                     "overrides": []
                 },
                 "gridPos": {
                     "h": 8,
                     "w": 7,
                     "x": 7,
@@ -1348,15 +1348,15 @@
                 "targets": [
                     {
                         "datasource": {
                             "type": "prometheus",
                             "uid": "PBFA97CFB590B2093"
                         },
                         "editorMode": "builder",
-                        "expr": "device_read_bytes_ps",
+                        "expr": "pool_read_bytes_ps",
                         "legendFormat": "__auto",
                         "range": true,
                         "refId": "A"
                     }
                 ],
                 "title": "read_speed",
                 "type": "timeseries"
@@ -1410,22 +1410,21 @@
                                     "value": null
                                 },
                                 {
                                     "color": "red",
                                     "value": 80
                                 }
                             ]
-                        },
-                        "unit": "\u00b5s"
+                        }
                     },
                     "overrides": []
                 },
                 "gridPos": {
                     "h": 8,
-                    "w": 8,
+                    "w": 7,
                     "x": 14,
                     "y": 33
                 },
                 "id": 5,
                 "options": {
                     "legend": {
                         "calcs": [],
@@ -1441,21 +1440,21 @@
                 "targets": [
                     {
                         "datasource": {
                             "type": "prometheus",
                             "uid": "PBFA97CFB590B2093"
                         },
                         "editorMode": "builder",
-                        "expr": "device_read_latency_ps",
+                        "expr": "pool_read_latency_ps",
                         "legendFormat": "__auto",
                         "range": true,
                         "refId": "A"
                     }
                 ],
-                "title": "device_read_latency_ps",
+                "title": "pool_read_latency_ps",
                 "type": "timeseries"
             },
             {
                 "datasource": {
                     "type": "prometheus",
                     "uid": "PBFA97CFB590B2093"
                 },
@@ -1533,21 +1532,21 @@
                 "targets": [
                     {
                         "datasource": {
                             "type": "prometheus",
                             "uid": "PBFA97CFB590B2093"
                         },
                         "editorMode": "builder",
-                        "expr": "device_read_io",
+                        "expr": "pool_read_io",
                         "legendFormat": "__auto",
                         "range": true,
                         "refId": "A"
                     }
                 ],
-                "title": "device_read_io",
+                "title": "pool_read_io",
                 "type": "timeseries"
             },
             {
                 "datasource": {
                     "type": "prometheus",
                     "uid": "PBFA97CFB590B2093"
                 },
@@ -1625,15 +1624,15 @@
                 "targets": [
                     {
                         "datasource": {
                             "type": "prometheus",
                             "uid": "PBFA97CFB590B2093"
                         },
                         "editorMode": "builder",
-                        "expr": "device_read_io_ps",
+                        "expr": "pool_read_io_ps",
                         "legendFormat": "__auto",
                         "range": true,
                         "refId": "A"
                     }
                 ],
                 "title": "read_iops",
                 "type": "timeseries"
@@ -1693,15 +1692,15 @@
                             ]
                         }
                     },
                     "overrides": []
                 },
                 "gridPos": {
                     "h": 7,
-                    "w": 8,
+                    "w": 7,
                     "x": 14,
                     "y": 41
                 },
                 "id": 6,
                 "options": {
                     "legend": {
                         "calcs": [],
@@ -1717,21 +1716,21 @@
                 "targets": [
                     {
                         "datasource": {
                             "type": "prometheus",
                             "uid": "PBFA97CFB590B2093"
                         },
                         "editorMode": "builder",
-                        "expr": "device_read_latency_ticks",
+                        "expr": "pool_read_latency_ticks",
                         "legendFormat": "__auto",
                         "range": true,
                         "refId": "A"
                     }
                 ],
-                "title": "device_read_latency_ticks",
+                "title": "pool_read_latency_ticks",
                 "type": "timeseries"
             },
             {
                 "collapsed": false,
                 "gridPos": {
                     "h": 1,
                     "w": 24,
@@ -1822,21 +1821,21 @@
                 "targets": [
                     {
                         "datasource": {
                             "type": "prometheus",
                             "uid": "PBFA97CFB590B2093"
                         },
                         "editorMode": "builder",
-                        "expr": "device_unmap_latency_ticks",
+                        "expr": "pool_unmap_latency_ticks",
                         "legendFormat": "__auto",
                         "range": true,
                         "refId": "A"
                     }
                 ],
-                "title": "device_unmap_latency_ticks",
+                "title": "pool_unmap_latency_ticks",
                 "type": "timeseries"
             },
             {
                 "datasource": {
                     "type": "prometheus",
                     "uid": "PBFA97CFB590B2093"
                 },
@@ -1885,15 +1884,15 @@
                                 },
                                 {
                                     "color": "red",
                                     "value": 80
                                 }
                             ]
                         },
-                        "unit": "bytes"
+                        "unit": "decbytes"
                     },
                     "overrides": []
                 },
                 "gridPos": {
                     "h": 7,
                     "w": 7,
                     "x": 7,
@@ -1915,21 +1914,21 @@
                 "targets": [
                     {
                         "datasource": {
                             "type": "prometheus",
                             "uid": "PBFA97CFB590B2093"
                         },
                         "editorMode": "builder",
-                        "expr": "device_unmap_bytes_ps",
+                        "expr": "pool_unmap_bytes_ps",
                         "legendFormat": "__auto",
                         "range": true,
                         "refId": "A"
                     }
                 ],
-                "title": "device_unmap_bytes_ps",
+                "title": "pool_unmap_bytes_ps",
                 "type": "timeseries"
             },
             {
                 "datasource": {
                     "type": "prometheus",
                     "uid": "PBFA97CFB590B2093"
                 },
@@ -1978,22 +1977,21 @@
                                     "value": null
                                 },
                                 {
                                     "color": "red",
                                     "value": 80
                                 }
                             ]
-                        },
-                        "unit": "\u00b5s"
+                        }
                     },
                     "overrides": []
                 },
                 "gridPos": {
                     "h": 7,
-                    "w": 8,
+                    "w": 7,
                     "x": 14,
                     "y": 49
                 },
                 "id": 20,
                 "options": {
                     "legend": {
                         "calcs": [],
@@ -2009,21 +2007,21 @@
                 "targets": [
                     {
                         "datasource": {
                             "type": "prometheus",
                             "uid": "PBFA97CFB590B2093"
                         },
                         "editorMode": "builder",
-                        "expr": "device_unmap_latency_ps",
+                        "expr": "pool_unmap_latency_ps",
                         "legendFormat": "__auto",
                         "range": true,
                         "refId": "A"
                     }
                 ],
-                "title": "device_unmap_latency_ps",
+                "title": "pool_unmap_latency_ps",
                 "type": "timeseries"
             },
             {
                 "datasource": {
                     "type": "prometheus",
                     "uid": "PBFA97CFB590B2093"
                 },
@@ -2081,15 +2079,15 @@
                         {
                             "__systemRef": "hideSeriesFrom",
                             "matcher": {
                                 "id": "byNames",
                                 "options": {
                                     "mode": "exclude",
                                     "names": [
-                                        "{__name__=\"device_unmap_io_ps\", cluster=\"c3663938-6610-44d5-9897-d7bfa60a43e1\", exported_job=\"collector\", instance=\"192.168.178.52:9091\", job=\"metricsgateway\"}"
+                                        "{__name__=\"pool_unmap_io_ps\", cluster=\"c3663938-6610-44d5-9897-d7bfa60a43e1\", exported_job=\"collector\", instance=\"192.168.178.52:9091\", job=\"metricsgateway\"}"
                                     ],
                                     "prefix": "All except:",
                                     "readOnly": true
                                 }
                             },
                             "properties": [
                                 {
@@ -2126,21 +2124,21 @@
                 "targets": [
                     {
                         "datasource": {
                             "type": "prometheus",
                             "uid": "PBFA97CFB590B2093"
                         },
                         "editorMode": "builder",
-                        "expr": "device_unmap_io_ps",
+                        "expr": "pool_unmap_io_ps",
                         "legendFormat": "__auto",
                         "range": true,
                         "refId": "A"
                     }
                 ],
-                "title": "device_unmap_io_ps",
+                "title": "pool_unmap_io_ps",
                 "type": "timeseries"
             },
             {
                 "datasource": {
                     "type": "prometheus",
                     "uid": "PBFA97CFB590B2093"
                 },
@@ -2218,21 +2216,21 @@
                 "targets": [
                     {
                         "datasource": {
                             "type": "prometheus",
                             "uid": "PBFA97CFB590B2093"
                         },
                         "editorMode": "builder",
-                        "expr": "device_unmap_io",
+                        "expr": "pool_unmap_io",
                         "legendFormat": "__auto",
                         "range": true,
                         "refId": "A"
                     }
                 ],
-                "title": "device_unmap_io",
+                "title": "pool_unmap_io",
                 "type": "timeseries"
             },
             {
                 "datasource": {
                     "type": "prometheus",
                     "uid": "PBFA97CFB590B2093"
                 },
@@ -2287,15 +2285,15 @@
                         },
                         "unit": "decbytes"
                     },
                     "overrides": []
                 },
                 "gridPos": {
                     "h": 7,
-                    "w": 8,
+                    "w": 7,
                     "x": 14,
                     "y": 56
                 },
                 "id": 16,
                 "options": {
                     "legend": {
                         "calcs": [],
@@ -2311,21 +2309,312 @@
                 "targets": [
                     {
                         "datasource": {
                             "type": "prometheus",
                             "uid": "PBFA97CFB590B2093"
                         },
                         "editorMode": "builder",
-                        "expr": "device_unmap_bytes",
+                        "expr": "pool_unmap_bytes",
+                        "legendFormat": "__auto",
+                        "range": true,
+                        "refId": "A"
+                    }
+                ],
+                "title": "pool_unmap_bytes",
+                "type": "timeseries"
+            },
+            {
+                "collapsed": false,
+                "gridPos": {
+                    "h": 1,
+                    "w": 24,
+                    "x": 0,
+                    "y": 63
+                },
+                "id": 32,
+                "panels": [],
+                "title": "others",
+                "type": "row"
+            },
+            {
+                "datasource": {
+                    "type": "prometheus",
+                    "uid": "PBFA97CFB590B2093"
+                },
+                "fieldConfig": {
+                    "defaults": {
+                        "color": {
+                            "mode": "palette-classic"
+                        },
+                        "custom": {
+                            "axisCenteredZero": false,
+                            "axisColorMode": "text",
+                            "axisLabel": "",
+                            "axisPlacement": "auto",
+                            "barAlignment": 0,
+                            "drawStyle": "line",
+                            "fillOpacity": 0,
+                            "gradientMode": "none",
+                            "hideFrom": {
+                                "legend": false,
+                                "tooltip": false,
+                                "viz": false
+                            },
+                            "lineInterpolation": "linear",
+                            "lineWidth": 1,
+                            "pointSize": 5,
+                            "scaleDistribution": {
+                                "type": "linear"
+                            },
+                            "showPoints": "auto",
+                            "spanNulls": false,
+                            "stacking": {
+                                "group": "A",
+                                "mode": "none"
+                            },
+                            "thresholdsStyle": {
+                                "mode": "off"
+                            }
+                        },
+                        "mappings": [],
+                        "thresholds": {
+                            "mode": "absolute",
+                            "steps": [
+                                {
+                                    "color": "green",
+                                    "value": null
+                                },
+                                {
+                                    "color": "red",
+                                    "value": 80
+                                }
+                            ]
+                        }
+                    },
+                    "overrides": []
+                },
+                "gridPos": {
+                    "h": 7,
+                    "w": 7,
+                    "x": 0,
+                    "y": 64
+                },
+                "id": 8,
+                "options": {
+                    "legend": {
+                        "calcs": [],
+                        "displayMode": "list",
+                        "placement": "bottom",
+                        "showLegend": true
+                    },
+                    "tooltip": {
+                        "mode": "single",
+                        "sort": "none"
+                    }
+                },
+                "targets": [
+                    {
+                        "datasource": {
+                            "type": "prometheus",
+                            "uid": "PBFA97CFB590B2093"
+                        },
+                        "editorMode": "builder",
+                        "expr": "pool_record_end_time",
+                        "legendFormat": "__auto",
+                        "range": true,
+                        "refId": "A"
+                    }
+                ],
+                "title": "pool_record_end_time",
+                "type": "timeseries"
+            },
+            {
+                "datasource": {
+                    "type": "prometheus",
+                    "uid": "PBFA97CFB590B2093"
+                },
+                "description": "",
+                "fieldConfig": {
+                    "defaults": {
+                        "color": {
+                            "mode": "palette-classic"
+                        },
+                        "custom": {
+                            "axisCenteredZero": false,
+                            "axisColorMode": "text",
+                            "axisLabel": "",
+                            "axisPlacement": "auto",
+                            "barAlignment": 0,
+                            "drawStyle": "line",
+                            "fillOpacity": 0,
+                            "gradientMode": "none",
+                            "hideFrom": {
+                                "legend": false,
+                                "tooltip": false,
+                                "viz": false
+                            },
+                            "lineInterpolation": "linear",
+                            "lineWidth": 1,
+                            "pointSize": 5,
+                            "scaleDistribution": {
+                                "type": "linear"
+                            },
+                            "showPoints": "auto",
+                            "spanNulls": false,
+                            "stacking": {
+                                "group": "A",
+                                "mode": "none"
+                            },
+                            "thresholdsStyle": {
+                                "mode": "off"
+                            }
+                        },
+                        "mappings": [],
+                        "thresholds": {
+                            "mode": "absolute",
+                            "steps": [
+                                {
+                                    "color": "green",
+                                    "value": null
+                                },
+                                {
+                                    "color": "red",
+                                    "value": 80
+                                }
+                            ]
+                        }
+                    },
+                    "overrides": []
+                },
+                "gridPos": {
+                    "h": 7,
+                    "w": 7,
+                    "x": 7,
+                    "y": 64
+                },
+                "id": 7,
+                "options": {
+                    "legend": {
+                        "calcs": [],
+                        "displayMode": "list",
+                        "placement": "bottom",
+                        "showLegend": true
+                    },
+                    "tooltip": {
+                        "mode": "single",
+                        "sort": "none"
+                    }
+                },
+                "targets": [
+                    {
+                        "datasource": {
+                            "type": "prometheus",
+                            "uid": "PBFA97CFB590B2093"
+                        },
+                        "editorMode": "builder",
+                        "expr": "pool_record_duration",
+                        "legendFormat": "__auto",
+                        "range": true,
+                        "refId": "A"
+                    }
+                ],
+                "title": "pool_record_duration",
+                "type": "timeseries"
+            },
+            {
+                "datasource": {
+                    "type": "prometheus",
+                    "uid": "PBFA97CFB590B2093"
+                },
+                "fieldConfig": {
+                    "defaults": {
+                        "color": {
+                            "mode": "palette-classic"
+                        },
+                        "custom": {
+                            "axisCenteredZero": false,
+                            "axisColorMode": "text",
+                            "axisLabel": "",
+                            "axisPlacement": "auto",
+                            "barAlignment": 0,
+                            "drawStyle": "line",
+                            "fillOpacity": 0,
+                            "gradientMode": "none",
+                            "hideFrom": {
+                                "legend": false,
+                                "tooltip": false,
+                                "viz": false
+                            },
+                            "lineInterpolation": "linear",
+                            "lineWidth": 1,
+                            "pointSize": 5,
+                            "scaleDistribution": {
+                                "type": "linear"
+                            },
+                            "showPoints": "auto",
+                            "spanNulls": false,
+                            "stacking": {
+                                "group": "A",
+                                "mode": "none"
+                            },
+                            "thresholdsStyle": {
+                                "mode": "off"
+                            }
+                        },
+                        "mappings": [],
+                        "thresholds": {
+                            "mode": "absolute",
+                            "steps": [
+                                {
+                                    "color": "green",
+                                    "value": null
+                                },
+                                {
+                                    "color": "red",
+                                    "value": 80
+                                }
+                            ]
+                        },
+                        "unit": "decbytes"
+                    },
+                    "overrides": []
+                },
+                "gridPos": {
+                    "h": 7,
+                    "w": 7,
+                    "x": 14,
+                    "y": 64
+                },
+                "id": 9,
+                "options": {
+                    "legend": {
+                        "calcs": [],
+                        "displayMode": "list",
+                        "placement": "bottom",
+                        "showLegend": true
+                    },
+                    "tooltip": {
+                        "mode": "single",
+                        "sort": "none"
+                    }
+                },
+                "targets": [
+                    {
+                        "datasource": {
+                            "type": "prometheus",
+                            "uid": "PBFA97CFB590B2093"
+                        },
+                        "editorMode": "builder",
+                        "expr": "pool_record_start_time",
                         "legendFormat": "__auto",
                         "range": true,
                         "refId": "A"
                     }
                 ],
-                "title": "device_unmap_bytes",
+                "title": "pool_record_start_time",
                 "type": "timeseries"
             }
         ],
         "refresh": "",
         "schemaVersion": 38,
         "style": "dark",
         "tags": [],
@@ -2334,13 +2623,13 @@
         },
         "time": {
             "from": "now-1h",
             "to": "now"
         },
         "timepicker": {},
         "timezone": "",
-        "title": "DevicesDashboard",
-        "uid": "d56e0ae7-48d5-481d-a2ea-3192da4d9e38",
+        "title": "PoolsDashboard",
+        "uid": "d56e0ae7-48d5-481d-a2ea-3192da4d9e40",
         "version": 5,
         "weekStart": ""
     }
 }
```

## Comparing `sbcli_mc-1.0.5/simplyblock_core/scripts/dashboards/pools.json` & `sbcli_mc-1.0.6/simplyblock_core/scripts/dashboards/cluster.json`

 * *Files 17% similar despite different names*

### Pretty-printed

 * *Similarity: 0.9665197534914369%*

 * *Differences: {"'dashboard'": "{'panels': {1: {'fieldConfig': {'defaults': {'unit': 'bytes'}}, 'targets': {0: "*

 * *                '{\'expr\': \'cluster_size_total{cluster="$Cluster"}\'}}, \'title\': '*

 * *                "'cluster_size_total'}, 2: {'fieldConfig': {'defaults': {'unit': 'bytes'}}, "*

 * *                '\'targets\': {0: {\'expr\': \'cluster_size_free{cluster="$Cluster"}\'}}, '*

 * *                "'title': 'cluster_size_free'}, 3: {'fieldConfig': {'defaults': {'unit': "*

 * *                "'bytes'}}, 'targets': {0: {'expr' […]*

```diff
@@ -86,15 +86,15 @@
                                 },
                                 {
                                     "color": "red",
                                     "value": 80
                                 }
                             ]
                         },
-                        "unit": "decbytes"
+                        "unit": "bytes"
                     },
                     "overrides": []
                 },
                 "gridPos": {
                     "h": 7,
                     "w": 7,
                     "x": 0,
@@ -116,21 +116,21 @@
                 "targets": [
                     {
                         "datasource": {
                             "type": "prometheus",
                             "uid": "PBFA97CFB590B2093"
                         },
                         "editorMode": "builder",
-                        "expr": "pool_size_total",
+                        "expr": "cluster_size_total{cluster=\"$Cluster\"}",
                         "legendFormat": "__auto",
                         "range": true,
                         "refId": "A"
                     }
                 ],
-                "title": "pool_size_total",
+                "title": "cluster_size_total",
                 "type": "timeseries"
             },
             {
                 "datasource": {
                     "type": "prometheus",
                     "uid": "PBFA97CFB590B2093"
                 },
@@ -179,15 +179,15 @@
                                 },
                                 {
                                     "color": "red",
                                     "value": 80
                                 }
                             ]
                         },
-                        "unit": "decbytes"
+                        "unit": "bytes"
                     },
                     "overrides": []
                 },
                 "gridPos": {
                     "h": 7,
                     "w": 7,
                     "x": 7,
@@ -209,21 +209,21 @@
                 "targets": [
                     {
                         "datasource": {
                             "type": "prometheus",
                             "uid": "PBFA97CFB590B2093"
                         },
                         "editorMode": "builder",
-                        "expr": "pool_size_free",
+                        "expr": "cluster_size_free{cluster=\"$Cluster\"}",
                         "legendFormat": "__auto",
                         "range": true,
                         "refId": "A"
                     }
                 ],
-                "title": "pool_size_free",
+                "title": "cluster_size_free",
                 "type": "timeseries"
             },
             {
                 "datasource": {
                     "type": "prometheus",
                     "uid": "PBFA97CFB590B2093"
                 },
@@ -272,15 +272,15 @@
                                 },
                                 {
                                     "color": "red",
                                     "value": 80
                                 }
                             ]
                         },
-                        "unit": "decbytes"
+                        "unit": "bytes"
                     },
                     "overrides": []
                 },
                 "gridPos": {
                     "h": 7,
                     "w": 7,
                     "x": 14,
@@ -302,21 +302,21 @@
                 "targets": [
                     {
                         "datasource": {
                             "type": "prometheus",
                             "uid": "PBFA97CFB590B2093"
                         },
                         "editorMode": "builder",
-                        "expr": "pool_size_used",
+                        "expr": "cluster_size_used{cluster=\"$Cluster\"}",
                         "legendFormat": "__auto",
                         "range": true,
                         "refId": "A"
                     }
                 ],
-                "title": "pool_size_used",
+                "title": "cluster_size_used",
                 "type": "timeseries"
             },
             {
                 "datasource": {
                     "type": "prometheus",
                     "uid": "PBFA97CFB590B2093"
                 },
@@ -365,15 +365,15 @@
                                 },
                                 {
                                     "color": "red",
                                     "value": 80
                                 }
                             ]
                         },
-                        "unit": "decbytes"
+                        "unit": "bytes"
                     },
                     "overrides": []
                 },
                 "gridPos": {
                     "h": 7,
                     "w": 7,
                     "x": 0,
@@ -395,21 +395,21 @@
                 "targets": [
                     {
                         "datasource": {
                             "type": "prometheus",
                             "uid": "PBFA97CFB590B2093"
                         },
                         "editorMode": "builder",
-                        "expr": "pool_size_prov",
+                        "expr": "cluster_size_prov{cluster=\"$Cluster\"}",
                         "legendFormat": "__auto",
                         "range": true,
                         "refId": "A"
                     }
                 ],
-                "title": "pool_size_prov",
+                "title": "cluster_size_prov",
                 "type": "timeseries"
             },
             {
                 "datasource": {
                     "type": "prometheus",
                     "uid": "PBFA97CFB590B2093"
                 },
@@ -458,15 +458,15 @@
                                 },
                                 {
                                     "color": "red",
                                     "value": 80
                                 }
                             ]
                         },
-                        "unit": "decbytes"
+                        "unit": "percent"
                     },
                     "overrides": []
                 },
                 "gridPos": {
                     "h": 7,
                     "w": 7,
                     "x": 7,
@@ -488,21 +488,21 @@
                 "targets": [
                     {
                         "datasource": {
                             "type": "prometheus",
                             "uid": "PBFA97CFB590B2093"
                         },
                         "editorMode": "builder",
-                        "expr": "pool_size_prov_util",
+                        "expr": "cluster_size_prov_util{cluster=\"$Cluster\"}",
                         "legendFormat": "__auto",
                         "range": true,
                         "refId": "A"
                     }
                 ],
-                "title": "pool_size_prov_util",
+                "title": "cluster_size_prov_util",
                 "type": "timeseries"
             },
             {
                 "datasource": {
                     "type": "prometheus",
                     "uid": "PBFA97CFB590B2093"
                 },
@@ -551,15 +551,15 @@
                                 },
                                 {
                                     "color": "red",
                                     "value": 80
                                 }
                             ]
                         },
-                        "unit": "decbytes"
+                        "unit": "percent"
                     },
                     "overrides": []
                 },
                 "gridPos": {
                     "h": 7,
                     "w": 7,
                     "x": 14,
@@ -581,21 +581,21 @@
                 "targets": [
                     {
                         "datasource": {
                             "type": "prometheus",
                             "uid": "PBFA97CFB590B2093"
                         },
                         "editorMode": "builder",
-                        "expr": "pool_size_util",
+                        "expr": "cluster_size_util{cluster=\"$Cluster\"}",
                         "legendFormat": "__auto",
                         "range": true,
                         "refId": "A"
                     }
                 ],
-                "title": "pool_size_util",
+                "title": "cluster_size_util",
                 "type": "timeseries"
             },
             {
                 "collapsed": false,
                 "gridPos": {
                     "h": 1,
                     "w": 24,
@@ -648,29 +648,28 @@
                             }
                         },
                         "mappings": [],
                         "thresholds": {
                             "mode": "absolute",
                             "steps": [
                                 {
-                                    "color": "green",
-                                    "value": null
+                                    "color": "green"
                                 },
                                 {
                                     "color": "red",
                                     "value": 80
                                 }
                             ]
                         },
-                        "unit": "decbytes"
+                        "unit": "bytes"
                     },
                     "overrides": []
                 },
                 "gridPos": {
-                    "h": 8,
+                    "h": 7,
                     "w": 7,
                     "x": 0,
                     "y": 16
                 },
                 "id": 22,
                 "options": {
                     "legend": {
@@ -687,21 +686,21 @@
                 "targets": [
                     {
                         "datasource": {
                             "type": "prometheus",
                             "uid": "PBFA97CFB590B2093"
                         },
                         "editorMode": "builder",
-                        "expr": "pool_write_bytes",
+                        "expr": "cluster_write_bytes{cluster=\"$Cluster\"}",
                         "legendFormat": "__auto",
                         "range": true,
                         "refId": "A"
                     }
                 ],
-                "title": "pool_write_bytes",
+                "title": "cluster_write_bytes",
                 "type": "timeseries"
             },
             {
                 "datasource": {
                     "type": "prometheus",
                     "uid": "PBFA97CFB590B2093"
                 },
@@ -741,29 +740,28 @@
                             }
                         },
                         "mappings": [],
                         "thresholds": {
                             "mode": "absolute",
                             "steps": [
                                 {
-                                    "color": "green",
-                                    "value": null
+                                    "color": "green"
                                 },
                                 {
                                     "color": "red",
                                     "value": 80
                                 }
                             ]
                         },
-                        "unit": "Bps"
+                        "unit": "binBps"
                     },
                     "overrides": []
                 },
                 "gridPos": {
-                    "h": 8,
+                    "h": 7,
                     "w": 7,
                     "x": 7,
                     "y": 16
                 },
                 "id": 23,
                 "options": {
                     "legend": {
@@ -780,15 +778,15 @@
                 "targets": [
                     {
                         "datasource": {
                             "type": "prometheus",
                             "uid": "PBFA97CFB590B2093"
                         },
                         "editorMode": "builder",
-                        "expr": "pool_write_bytes_ps",
+                        "expr": "cluster_write_bytes_ps{cluster=\"$Cluster\"}",
                         "legendFormat": "__auto",
                         "range": true,
                         "refId": "A"
                     }
                 ],
                 "title": "write_speed",
                 "type": "timeseries"
@@ -834,33 +832,33 @@
                             }
                         },
                         "mappings": [],
                         "thresholds": {
                             "mode": "absolute",
                             "steps": [
                                 {
-                                    "color": "green",
-                                    "value": null
+                                    "color": "green"
                                 },
                                 {
                                     "color": "red",
                                     "value": 80
                                 }
                             ]
-                        }
+                        },
+                        "unit": "\u00b5s"
                     },
                     "overrides": []
                 },
                 "gridPos": {
-                    "h": 8,
+                    "h": 7,
                     "w": 7,
                     "x": 14,
                     "y": 16
                 },
-                "id": 33,
+                "id": 26,
                 "options": {
                     "legend": {
                         "calcs": [],
                         "displayMode": "list",
                         "placement": "bottom",
                         "showLegend": true
                     },
@@ -872,21 +870,21 @@
                 "targets": [
                     {
                         "datasource": {
                             "type": "prometheus",
                             "uid": "PBFA97CFB590B2093"
                         },
                         "editorMode": "builder",
-                        "expr": "pool_write_latency_ticks",
+                        "expr": "cluster_write_latency_ps{cluster=\"$Cluster\"} / 1000",
                         "legendFormat": "__auto",
                         "range": true,
                         "refId": "A"
                     }
                 ],
-                "title": "pool_wite_latency_ticks",
+                "title": "cluster_write_latency_ps",
                 "type": "timeseries"
             },
             {
                 "datasource": {
                     "type": "prometheus",
                     "uid": "PBFA97CFB590B2093"
                 },
@@ -926,31 +924,30 @@
                             }
                         },
                         "mappings": [],
                         "thresholds": {
                             "mode": "absolute",
                             "steps": [
                                 {
-                                    "color": "green",
-                                    "value": null
+                                    "color": "green"
                                 },
                                 {
                                     "color": "red",
                                     "value": 80
                                 }
                             ]
                         }
                     },
                     "overrides": []
                 },
                 "gridPos": {
-                    "h": 8,
+                    "h": 7,
                     "w": 7,
                     "x": 0,
-                    "y": 24
+                    "y": 23
                 },
                 "id": 24,
                 "options": {
                     "legend": {
                         "calcs": [],
                         "displayMode": "list",
                         "placement": "bottom",
@@ -964,21 +961,21 @@
                 "targets": [
                     {
                         "datasource": {
                             "type": "prometheus",
                             "uid": "PBFA97CFB590B2093"
                         },
                         "editorMode": "builder",
-                        "expr": "pool_write_io",
+                        "expr": "cluster_write_io{cluster=\"$Cluster\"}",
                         "legendFormat": "__auto",
                         "range": true,
                         "refId": "A"
                     }
                 ],
-                "title": "pool_write_io",
+                "title": "cluster_write_io",
                 "type": "timeseries"
             },
             {
                 "datasource": {
                     "type": "prometheus",
                     "uid": "PBFA97CFB590B2093"
                 },
@@ -1018,31 +1015,30 @@
                             }
                         },
                         "mappings": [],
                         "thresholds": {
                             "mode": "absolute",
                             "steps": [
                                 {
-                                    "color": "green",
-                                    "value": null
+                                    "color": "green"
                                 },
                                 {
                                     "color": "red",
                                     "value": 80
                                 }
                             ]
                         }
                     },
                     "overrides": []
                 },
                 "gridPos": {
-                    "h": 8,
+                    "h": 7,
                     "w": 7,
                     "x": 7,
-                    "y": 24
+                    "y": 23
                 },
                 "id": 25,
                 "options": {
                     "legend": {
                         "calcs": [],
                         "displayMode": "list",
                         "placement": "bottom",
@@ -1056,15 +1052,15 @@
                 "targets": [
                     {
                         "datasource": {
                             "type": "prometheus",
                             "uid": "PBFA97CFB590B2093"
                         },
                         "editorMode": "builder",
-                        "expr": "pool_write_io_ps",
+                        "expr": "cluster_write_io_ps{cluster=\"$Cluster\"}",
                         "legendFormat": "__auto",
                         "range": true,
                         "refId": "A"
                     }
                 ],
                 "title": "write_iops",
                 "type": "timeseries"
@@ -1110,34 +1106,32 @@
                             }
                         },
                         "mappings": [],
                         "thresholds": {
                             "mode": "absolute",
                             "steps": [
                                 {
-                                    "color": "green",
-                                    "value": null
+                                    "color": "green"
                                 },
                                 {
                                     "color": "red",
                                     "value": 80
                                 }
                             ]
-                        },
-                        "unit": "ns"
+                        }
                     },
                     "overrides": []
                 },
                 "gridPos": {
-                    "h": 8,
+                    "h": 7,
                     "w": 7,
                     "x": 14,
-                    "y": 24
+                    "y": 23
                 },
-                "id": 26,
+                "id": 33,
                 "options": {
                     "legend": {
                         "calcs": [],
                         "displayMode": "list",
                         "placement": "bottom",
                         "showLegend": true
                     },
@@ -1149,30 +1143,30 @@
                 "targets": [
                     {
                         "datasource": {
                             "type": "prometheus",
                             "uid": "PBFA97CFB590B2093"
                         },
                         "editorMode": "builder",
-                        "expr": "pool_write_latency_ps / 1000",
+                        "expr": "cluster_write_latency_ticks{cluster=\"$Cluster\"}",
                         "legendFormat": "__auto",
                         "range": true,
                         "refId": "A"
                     }
                 ],
-                "title": "pool_write_latency_ps",
+                "title": "cluster_wite_latency_ticks",
                 "type": "timeseries"
             },
             {
                 "collapsed": false,
                 "gridPos": {
                     "h": 1,
                     "w": 24,
                     "x": 0,
-                    "y": 32
+                    "y": 30
                 },
                 "id": 30,
                 "panels": [],
                 "title": "Reads",
                 "type": "row"
             },
             {
@@ -1216,32 +1210,31 @@
                             }
                         },
                         "mappings": [],
                         "thresholds": {
                             "mode": "absolute",
                             "steps": [
                                 {
-                                    "color": "green",
-                                    "value": null
+                                    "color": "green"
                                 },
                                 {
                                     "color": "red",
                                     "value": 80
                                 }
                             ]
                         },
-                        "unit": "decbytes"
+                        "unit": "bytes"
                     },
                     "overrides": []
                 },
                 "gridPos": {
                     "h": 8,
                     "w": 7,
                     "x": 0,
-                    "y": 33
+                    "y": 31
                 },
                 "id": 1,
                 "options": {
                     "legend": {
                         "calcs": [],
                         "displayMode": "list",
                         "placement": "bottom",
@@ -1255,21 +1248,21 @@
                 "targets": [
                     {
                         "datasource": {
                             "type": "prometheus",
                             "uid": "PBFA97CFB590B2093"
                         },
                         "editorMode": "builder",
-                        "expr": "pool_read_bytes",
+                        "expr": "cluster_read_bytes{cluster=\"$Cluster\"}",
                         "legendFormat": "__auto",
                         "range": true,
                         "refId": "A"
                     }
                 ],
-                "title": "pool_read_bytes",
+                "title": "cluster_read_bytes",
                 "type": "timeseries"
             },
             {
                 "datasource": {
                     "type": "prometheus",
                     "uid": "PBFA97CFB590B2093"
                 },
@@ -1309,32 +1302,31 @@
                             }
                         },
                         "mappings": [],
                         "thresholds": {
                             "mode": "absolute",
                             "steps": [
                                 {
-                                    "color": "green",
-                                    "value": null
+                                    "color": "green"
                                 },
                                 {
                                     "color": "red",
                                     "value": 80
                                 }
                             ]
                         },
-                        "unit": "Bps"
+                        "unit": "bytes"
                     },
                     "overrides": []
                 },
                 "gridPos": {
                     "h": 8,
                     "w": 7,
                     "x": 7,
-                    "y": 33
+                    "y": 31
                 },
                 "id": 2,
                 "options": {
                     "legend": {
                         "calcs": [],
                         "displayMode": "list",
                         "placement": "bottom",
@@ -1348,15 +1340,15 @@
                 "targets": [
                     {
                         "datasource": {
                             "type": "prometheus",
                             "uid": "PBFA97CFB590B2093"
                         },
                         "editorMode": "builder",
-                        "expr": "pool_read_bytes_ps",
+                        "expr": "cluster_read_bytes_ps{cluster=\"$Cluster\"}",
                         "legendFormat": "__auto",
                         "range": true,
                         "refId": "A"
                     }
                 ],
                 "title": "read_speed",
                 "type": "timeseries"
@@ -1402,31 +1394,31 @@
                             }
                         },
                         "mappings": [],
                         "thresholds": {
                             "mode": "absolute",
                             "steps": [
                                 {
-                                    "color": "green",
-                                    "value": null
+                                    "color": "green"
                                 },
                                 {
                                     "color": "red",
                                     "value": 80
                                 }
                             ]
-                        }
+                        },
+                        "unit": "\u00b5s"
                     },
                     "overrides": []
                 },
                 "gridPos": {
                     "h": 8,
                     "w": 7,
                     "x": 14,
-                    "y": 33
+                    "y": 31
                 },
                 "id": 5,
                 "options": {
                     "legend": {
                         "calcs": [],
                         "displayMode": "list",
                         "placement": "bottom",
@@ -1440,21 +1432,21 @@
                 "targets": [
                     {
                         "datasource": {
                             "type": "prometheus",
                             "uid": "PBFA97CFB590B2093"
                         },
                         "editorMode": "builder",
-                        "expr": "pool_read_latency_ps",
+                        "expr": "cluster_read_latency_ps{cluster=\"$Cluster\"}",
                         "legendFormat": "__auto",
                         "range": true,
                         "refId": "A"
                     }
                 ],
-                "title": "pool_read_latency_ps",
+                "title": "cluster_read_latency_ps",
                 "type": "timeseries"
             },
             {
                 "datasource": {
                     "type": "prometheus",
                     "uid": "PBFA97CFB590B2093"
                 },
@@ -1494,31 +1486,30 @@
                             }
                         },
                         "mappings": [],
                         "thresholds": {
                             "mode": "absolute",
                             "steps": [
                                 {
-                                    "color": "green",
-                                    "value": null
+                                    "color": "green"
                                 },
                                 {
                                     "color": "red",
                                     "value": 80
                                 }
                             ]
                         }
                     },
                     "overrides": []
                 },
                 "gridPos": {
                     "h": 7,
                     "w": 7,
                     "x": 0,
-                    "y": 41
+                    "y": 39
                 },
                 "id": 3,
                 "options": {
                     "legend": {
                         "calcs": [],
                         "displayMode": "list",
                         "placement": "bottom",
@@ -1532,21 +1523,21 @@
                 "targets": [
                     {
                         "datasource": {
                             "type": "prometheus",
                             "uid": "PBFA97CFB590B2093"
                         },
                         "editorMode": "builder",
-                        "expr": "pool_read_io",
+                        "expr": "cluster_read_io{cluster=\"$Cluster\"}",
                         "legendFormat": "__auto",
                         "range": true,
                         "refId": "A"
                     }
                 ],
-                "title": "pool_read_io",
+                "title": "cluster_read_io",
                 "type": "timeseries"
             },
             {
                 "datasource": {
                     "type": "prometheus",
                     "uid": "PBFA97CFB590B2093"
                 },
@@ -1586,31 +1577,30 @@
                             }
                         },
                         "mappings": [],
                         "thresholds": {
                             "mode": "absolute",
                             "steps": [
                                 {
-                                    "color": "green",
-                                    "value": null
+                                    "color": "green"
                                 },
                                 {
                                     "color": "red",
                                     "value": 80
                                 }
                             ]
                         }
                     },
                     "overrides": []
                 },
                 "gridPos": {
                     "h": 7,
                     "w": 7,
                     "x": 7,
-                    "y": 41
+                    "y": 39
                 },
                 "id": 4,
                 "options": {
                     "legend": {
                         "calcs": [],
                         "displayMode": "list",
                         "placement": "bottom",
@@ -1624,15 +1614,15 @@
                 "targets": [
                     {
                         "datasource": {
                             "type": "prometheus",
                             "uid": "PBFA97CFB590B2093"
                         },
                         "editorMode": "builder",
-                        "expr": "pool_read_io_ps",
+                        "expr": "cluster_read_io_ps{cluster=\"$Cluster\"}",
                         "legendFormat": "__auto",
                         "range": true,
                         "refId": "A"
                     }
                 ],
                 "title": "read_iops",
                 "type": "timeseries"
@@ -1678,31 +1668,30 @@
                             }
                         },
                         "mappings": [],
                         "thresholds": {
                             "mode": "absolute",
                             "steps": [
                                 {
-                                    "color": "green",
-                                    "value": null
+                                    "color": "green"
                                 },
                                 {
                                     "color": "red",
                                     "value": 80
                                 }
                             ]
                         }
                     },
                     "overrides": []
                 },
                 "gridPos": {
                     "h": 7,
                     "w": 7,
                     "x": 14,
-                    "y": 41
+                    "y": 39
                 },
                 "id": 6,
                 "options": {
                     "legend": {
                         "calcs": [],
                         "displayMode": "list",
                         "placement": "bottom",
@@ -1716,30 +1705,30 @@
                 "targets": [
                     {
                         "datasource": {
                             "type": "prometheus",
                             "uid": "PBFA97CFB590B2093"
                         },
                         "editorMode": "builder",
-                        "expr": "pool_read_latency_ticks",
+                        "expr": "cluster_read_latency_ticks{cluster=\"$Cluster\"}",
                         "legendFormat": "__auto",
                         "range": true,
                         "refId": "A"
                     }
                 ],
-                "title": "pool_read_latency_ticks",
+                "title": "cluster_read_latency_ticks",
                 "type": "timeseries"
             },
             {
                 "collapsed": false,
                 "gridPos": {
                     "h": 1,
                     "w": 24,
                     "x": 0,
-                    "y": 48
+                    "y": 46
                 },
                 "id": 29,
                 "panels": [],
                 "title": "unmap",
                 "type": "row"
             },
             {
@@ -1783,31 +1772,30 @@
                             }
                         },
                         "mappings": [],
                         "thresholds": {
                             "mode": "absolute",
                             "steps": [
                                 {
-                                    "color": "green",
-                                    "value": null
+                                    "color": "green"
                                 },
                                 {
                                     "color": "red",
                                     "value": 80
                                 }
                             ]
                         }
                     },
                     "overrides": []
                 },
                 "gridPos": {
                     "h": 7,
                     "w": 7,
                     "x": 0,
-                    "y": 49
+                    "y": 47
                 },
                 "id": 21,
                 "options": {
                     "legend": {
                         "calcs": [],
                         "displayMode": "list",
                         "placement": "bottom",
@@ -1821,21 +1809,21 @@
                 "targets": [
                     {
                         "datasource": {
                             "type": "prometheus",
                             "uid": "PBFA97CFB590B2093"
                         },
                         "editorMode": "builder",
-                        "expr": "pool_unmap_latency_ticks",
+                        "expr": "cluster_unmap_latency_ticks{cluster=\"$Cluster\"}",
                         "legendFormat": "__auto",
                         "range": true,
                         "refId": "A"
                     }
                 ],
-                "title": "pool_unmap_latency_ticks",
+                "title": "cluster_unmap_latency_ticks",
                 "type": "timeseries"
             },
             {
                 "datasource": {
                     "type": "prometheus",
                     "uid": "PBFA97CFB590B2093"
                 },
@@ -1875,32 +1863,31 @@
                             }
                         },
                         "mappings": [],
                         "thresholds": {
                             "mode": "absolute",
                             "steps": [
                                 {
-                                    "color": "green",
-                                    "value": null
+                                    "color": "green"
                                 },
                                 {
                                     "color": "red",
                                     "value": 80
                                 }
                             ]
                         },
-                        "unit": "decbytes"
+                        "unit": "bytes"
                     },
                     "overrides": []
                 },
                 "gridPos": {
                     "h": 7,
                     "w": 7,
                     "x": 7,
-                    "y": 49
+                    "y": 47
                 },
                 "id": 17,
                 "options": {
                     "legend": {
                         "calcs": [],
                         "displayMode": "list",
                         "placement": "bottom",
@@ -1914,21 +1901,21 @@
                 "targets": [
                     {
                         "datasource": {
                             "type": "prometheus",
                             "uid": "PBFA97CFB590B2093"
                         },
                         "editorMode": "builder",
-                        "expr": "pool_unmap_bytes_ps",
+                        "expr": "cluster_unmap_bytes_ps{cluster=\"$Cluster\"}",
                         "legendFormat": "__auto",
                         "range": true,
                         "refId": "A"
                     }
                 ],
-                "title": "pool_unmap_bytes_ps",
+                "title": "cluster_unmap_bytes_ps",
                 "type": "timeseries"
             },
             {
                 "datasource": {
                     "type": "prometheus",
                     "uid": "PBFA97CFB590B2093"
                 },
@@ -1969,31 +1956,31 @@
                             }
                         },
                         "mappings": [],
                         "thresholds": {
                             "mode": "absolute",
                             "steps": [
                                 {
-                                    "color": "green",
-                                    "value": null
+                                    "color": "green"
                                 },
                                 {
                                     "color": "red",
                                     "value": 80
                                 }
                             ]
-                        }
+                        },
+                        "unit": "\u00b5s"
                     },
                     "overrides": []
                 },
                 "gridPos": {
                     "h": 7,
                     "w": 7,
                     "x": 14,
-                    "y": 49
+                    "y": 47
                 },
                 "id": 20,
                 "options": {
                     "legend": {
                         "calcs": [],
                         "displayMode": "list",
                         "placement": "bottom",
@@ -2007,21 +1994,21 @@
                 "targets": [
                     {
                         "datasource": {
                             "type": "prometheus",
                             "uid": "PBFA97CFB590B2093"
                         },
                         "editorMode": "builder",
-                        "expr": "pool_unmap_latency_ps",
+                        "expr": "cluster_unmap_latency_ps{cluster=\"$Cluster\"}",
                         "legendFormat": "__auto",
                         "range": true,
                         "refId": "A"
                     }
                 ],
-                "title": "pool_unmap_latency_ps",
+                "title": "cluster_unmap_latency_ps",
                 "type": "timeseries"
             },
             {
                 "datasource": {
                     "type": "prometheus",
                     "uid": "PBFA97CFB590B2093"
                 },
@@ -2061,16 +2048,15 @@
                             }
                         },
                         "mappings": [],
                         "thresholds": {
                             "mode": "absolute",
                             "steps": [
                                 {
-                                    "color": "green",
-                                    "value": null
+                                    "color": "green"
                                 },
                                 {
                                     "color": "red",
                                     "value": 80
                                 }
                             ]
                         }
@@ -2079,15 +2065,15 @@
                         {
                             "__systemRef": "hideSeriesFrom",
                             "matcher": {
                                 "id": "byNames",
                                 "options": {
                                     "mode": "exclude",
                                     "names": [
-                                        "{__name__=\"pool_unmap_io_ps\", cluster=\"c3663938-6610-44d5-9897-d7bfa60a43e1\", exported_job=\"collector\", instance=\"192.168.178.52:9091\", job=\"metricsgateway\"}"
+                                        "{__name__=\"cluster_unmap_io_ps\", cluster=\"c3663938-6610-44d5-9897-d7bfa60a43e1\", exported_job=\"collector\", instance=\"192.168.178.52:9091\", job=\"metricsgateway\"}"
                                     ],
                                     "prefix": "All except:",
                                     "readOnly": true
                                 }
                             },
                             "properties": [
                                 {
@@ -2102,15 +2088,15 @@
                         }
                     ]
                 },
                 "gridPos": {
                     "h": 7,
                     "w": 7,
                     "x": 0,
-                    "y": 56
+                    "y": 54
                 },
                 "id": 19,
                 "options": {
                     "legend": {
                         "calcs": [],
                         "displayMode": "list",
                         "placement": "bottom",
@@ -2124,21 +2110,21 @@
                 "targets": [
                     {
                         "datasource": {
                             "type": "prometheus",
                             "uid": "PBFA97CFB590B2093"
                         },
                         "editorMode": "builder",
-                        "expr": "pool_unmap_io_ps",
+                        "expr": "cluster_unmap_io_ps{cluster=\"$Cluster\"}",
                         "legendFormat": "__auto",
                         "range": true,
                         "refId": "A"
                     }
                 ],
-                "title": "pool_unmap_io_ps",
+                "title": "cluster_unmap_io_ps",
                 "type": "timeseries"
             },
             {
                 "datasource": {
                     "type": "prometheus",
                     "uid": "PBFA97CFB590B2093"
                 },
@@ -2178,31 +2164,30 @@
                             }
                         },
                         "mappings": [],
                         "thresholds": {
                             "mode": "absolute",
                             "steps": [
                                 {
-                                    "color": "green",
-                                    "value": null
+                                    "color": "green"
                                 },
                                 {
                                     "color": "red",
                                     "value": 80
                                 }
                             ]
                         }
                     },
                     "overrides": []
                 },
                 "gridPos": {
                     "h": 7,
                     "w": 7,
                     "x": 7,
-                    "y": 56
+                    "y": 54
                 },
                 "id": 18,
                 "options": {
                     "legend": {
                         "calcs": [],
                         "displayMode": "list",
                         "placement": "bottom",
@@ -2216,21 +2201,21 @@
                 "targets": [
                     {
                         "datasource": {
                             "type": "prometheus",
                             "uid": "PBFA97CFB590B2093"
                         },
                         "editorMode": "builder",
-                        "expr": "pool_unmap_io",
+                        "expr": "cluster_unmap_io{cluster=\"$Cluster\"}",
                         "legendFormat": "__auto",
                         "range": true,
                         "refId": "A"
                     }
                 ],
-                "title": "pool_unmap_io",
+                "title": "cluster_unmap_io",
                 "type": "timeseries"
             },
             {
                 "datasource": {
                     "type": "prometheus",
                     "uid": "PBFA97CFB590B2093"
                 },
@@ -2270,32 +2255,31 @@
                             }
                         },
                         "mappings": [],
                         "thresholds": {
                             "mode": "absolute",
                             "steps": [
                                 {
-                                    "color": "green",
-                                    "value": null
+                                    "color": "green"
                                 },
                                 {
                                     "color": "red",
                                     "value": 80
                                 }
                             ]
                         },
-                        "unit": "decbytes"
+                        "unit": "bytes"
                     },
                     "overrides": []
                 },
                 "gridPos": {
                     "h": 7,
                     "w": 7,
                     "x": 14,
-                    "y": 56
+                    "y": 54
                 },
                 "id": 16,
                 "options": {
                     "legend": {
                         "calcs": [],
                         "displayMode": "list",
                         "placement": "bottom",
@@ -2309,327 +2293,65 @@
                 "targets": [
                     {
                         "datasource": {
                             "type": "prometheus",
                             "uid": "PBFA97CFB590B2093"
                         },
                         "editorMode": "builder",
-                        "expr": "pool_unmap_bytes",
-                        "legendFormat": "__auto",
-                        "range": true,
-                        "refId": "A"
-                    }
-                ],
-                "title": "pool_unmap_bytes",
-                "type": "timeseries"
-            },
-            {
-                "collapsed": false,
-                "gridPos": {
-                    "h": 1,
-                    "w": 24,
-                    "x": 0,
-                    "y": 63
-                },
-                "id": 32,
-                "panels": [],
-                "title": "others",
-                "type": "row"
-            },
-            {
-                "datasource": {
-                    "type": "prometheus",
-                    "uid": "PBFA97CFB590B2093"
-                },
-                "fieldConfig": {
-                    "defaults": {
-                        "color": {
-                            "mode": "palette-classic"
-                        },
-                        "custom": {
-                            "axisCenteredZero": false,
-                            "axisColorMode": "text",
-                            "axisLabel": "",
-                            "axisPlacement": "auto",
-                            "barAlignment": 0,
-                            "drawStyle": "line",
-                            "fillOpacity": 0,
-                            "gradientMode": "none",
-                            "hideFrom": {
-                                "legend": false,
-                                "tooltip": false,
-                                "viz": false
-                            },
-                            "lineInterpolation": "linear",
-                            "lineWidth": 1,
-                            "pointSize": 5,
-                            "scaleDistribution": {
-                                "type": "linear"
-                            },
-                            "showPoints": "auto",
-                            "spanNulls": false,
-                            "stacking": {
-                                "group": "A",
-                                "mode": "none"
-                            },
-                            "thresholdsStyle": {
-                                "mode": "off"
-                            }
-                        },
-                        "mappings": [],
-                        "thresholds": {
-                            "mode": "absolute",
-                            "steps": [
-                                {
-                                    "color": "green",
-                                    "value": null
-                                },
-                                {
-                                    "color": "red",
-                                    "value": 80
-                                }
-                            ]
-                        }
-                    },
-                    "overrides": []
-                },
-                "gridPos": {
-                    "h": 7,
-                    "w": 7,
-                    "x": 0,
-                    "y": 64
-                },
-                "id": 8,
-                "options": {
-                    "legend": {
-                        "calcs": [],
-                        "displayMode": "list",
-                        "placement": "bottom",
-                        "showLegend": true
-                    },
-                    "tooltip": {
-                        "mode": "single",
-                        "sort": "none"
-                    }
-                },
-                "targets": [
-                    {
-                        "datasource": {
-                            "type": "prometheus",
-                            "uid": "PBFA97CFB590B2093"
-                        },
-                        "editorMode": "builder",
-                        "expr": "pool_record_end_time",
-                        "legendFormat": "__auto",
-                        "range": true,
-                        "refId": "A"
-                    }
-                ],
-                "title": "pool_record_end_time",
-                "type": "timeseries"
-            },
-            {
-                "datasource": {
-                    "type": "prometheus",
-                    "uid": "PBFA97CFB590B2093"
-                },
-                "description": "",
-                "fieldConfig": {
-                    "defaults": {
-                        "color": {
-                            "mode": "palette-classic"
-                        },
-                        "custom": {
-                            "axisCenteredZero": false,
-                            "axisColorMode": "text",
-                            "axisLabel": "",
-                            "axisPlacement": "auto",
-                            "barAlignment": 0,
-                            "drawStyle": "line",
-                            "fillOpacity": 0,
-                            "gradientMode": "none",
-                            "hideFrom": {
-                                "legend": false,
-                                "tooltip": false,
-                                "viz": false
-                            },
-                            "lineInterpolation": "linear",
-                            "lineWidth": 1,
-                            "pointSize": 5,
-                            "scaleDistribution": {
-                                "type": "linear"
-                            },
-                            "showPoints": "auto",
-                            "spanNulls": false,
-                            "stacking": {
-                                "group": "A",
-                                "mode": "none"
-                            },
-                            "thresholdsStyle": {
-                                "mode": "off"
-                            }
-                        },
-                        "mappings": [],
-                        "thresholds": {
-                            "mode": "absolute",
-                            "steps": [
-                                {
-                                    "color": "green",
-                                    "value": null
-                                },
-                                {
-                                    "color": "red",
-                                    "value": 80
-                                }
-                            ]
-                        }
-                    },
-                    "overrides": []
-                },
-                "gridPos": {
-                    "h": 7,
-                    "w": 7,
-                    "x": 7,
-                    "y": 64
-                },
-                "id": 7,
-                "options": {
-                    "legend": {
-                        "calcs": [],
-                        "displayMode": "list",
-                        "placement": "bottom",
-                        "showLegend": true
-                    },
-                    "tooltip": {
-                        "mode": "single",
-                        "sort": "none"
-                    }
-                },
-                "targets": [
-                    {
-                        "datasource": {
-                            "type": "prometheus",
-                            "uid": "PBFA97CFB590B2093"
-                        },
-                        "editorMode": "builder",
-                        "expr": "pool_record_duration",
-                        "legendFormat": "__auto",
-                        "range": true,
-                        "refId": "A"
-                    }
-                ],
-                "title": "pool_record_duration",
-                "type": "timeseries"
-            },
-            {
-                "datasource": {
-                    "type": "prometheus",
-                    "uid": "PBFA97CFB590B2093"
-                },
-                "fieldConfig": {
-                    "defaults": {
-                        "color": {
-                            "mode": "palette-classic"
-                        },
-                        "custom": {
-                            "axisCenteredZero": false,
-                            "axisColorMode": "text",
-                            "axisLabel": "",
-                            "axisPlacement": "auto",
-                            "barAlignment": 0,
-                            "drawStyle": "line",
-                            "fillOpacity": 0,
-                            "gradientMode": "none",
-                            "hideFrom": {
-                                "legend": false,
-                                "tooltip": false,
-                                "viz": false
-                            },
-                            "lineInterpolation": "linear",
-                            "lineWidth": 1,
-                            "pointSize": 5,
-                            "scaleDistribution": {
-                                "type": "linear"
-                            },
-                            "showPoints": "auto",
-                            "spanNulls": false,
-                            "stacking": {
-                                "group": "A",
-                                "mode": "none"
-                            },
-                            "thresholdsStyle": {
-                                "mode": "off"
-                            }
-                        },
-                        "mappings": [],
-                        "thresholds": {
-                            "mode": "absolute",
-                            "steps": [
-                                {
-                                    "color": "green",
-                                    "value": null
-                                },
-                                {
-                                    "color": "red",
-                                    "value": 80
-                                }
-                            ]
-                        },
-                        "unit": "decbytes"
-                    },
-                    "overrides": []
-                },
-                "gridPos": {
-                    "h": 7,
-                    "w": 7,
-                    "x": 14,
-                    "y": 64
-                },
-                "id": 9,
-                "options": {
-                    "legend": {
-                        "calcs": [],
-                        "displayMode": "list",
-                        "placement": "bottom",
-                        "showLegend": true
-                    },
-                    "tooltip": {
-                        "mode": "single",
-                        "sort": "none"
-                    }
-                },
-                "targets": [
-                    {
-                        "datasource": {
-                            "type": "prometheus",
-                            "uid": "PBFA97CFB590B2093"
-                        },
-                        "editorMode": "builder",
-                        "expr": "pool_record_start_time",
+                        "expr": "cluster_unmap_bytes{cluster=\"$Cluster\"}",
                         "legendFormat": "__auto",
                         "range": true,
                         "refId": "A"
                     }
                 ],
-                "title": "pool_record_start_time",
+                "title": "cluster_unmap_bytes",
                 "type": "timeseries"
             }
         ],
         "refresh": "",
         "schemaVersion": 38,
         "style": "dark",
         "tags": [],
         "templating": {
-            "list": []
+            "list": [
+                {
+                    "current": {
+                        "selected": false,
+                        "text": "76aa3622-8918-4539-adb2-7c4b1852be14",
+                        "value": "76aa3622-8918-4539-adb2-7c4b1852be14"
+                    },
+                    "datasource": {
+                        "type": "prometheus",
+                        "uid": "PBFA97CFB590B2093"
+                    },
+                    "definition": "query_result(cluster_read_io)",
+                    "description": "Cluster",
+                    "hide": 0,
+                    "includeAll": false,
+                    "label": "Cluster",
+                    "multi": true,
+                    "name": "Cluster",
+                    "options": [],
+                    "query": {
+                        "query": "query_result(cluster_read_io)",
+                        "refId": "PrometheusVariableQueryEditor-VariableQuery"
+                    },
+                    "refresh": 2,
+                    "regex": "/.*cluster=\"([^\"]*).*/",
+                    "skipUrlSync": false,
+                    "sort": 1,
+                    "type": "query"
+                }
+            ]
         },
         "time": {
             "from": "now-1h",
             "to": "now"
         },
         "timepicker": {},
         "timezone": "",
-        "title": "PoolsDashboard",
-        "uid": "d56e0ae7-48d5-481d-a2ea-3192da4d9e40",
+        "title": "ClusterDashboard",
+        "uid": "d56e0ae7-48d5-481d-a2ea-3192da4d9e39",
         "version": 5,
         "weekStart": ""
     }
 }
```

## Comparing `sbcli_mc-1.0.5/simplyblock_core/scripts/dashboards/node-exporter.json` & `sbcli_mc-1.0.6/simplyblock_core/scripts/dashboards/node-exporter.json`

 * *Files identical despite different names*

## Comparing `sbcli_mc-1.0.5/sbcli_mc.egg-info/SOURCES.txt` & `sbcli_mc-1.0.6/sbcli_mc.egg-info/SOURCES.txt`

 * *Files 1% similar despite different names*

```diff
@@ -53,15 +53,14 @@
 simplyblock_core/models/nvme_device.py
 simplyblock_core/models/pool.py
 simplyblock_core/models/port_stat.py
 simplyblock_core/models/snapshot.py
 simplyblock_core/models/stats.py
 simplyblock_core/models/storage_node.py
 simplyblock_core/scripts/__init__.py
-simplyblock_core/scripts/apply_dashboard.sh
 simplyblock_core/scripts/clean_local_storage_deploy.sh
 simplyblock_core/scripts/config_docker.sh
 simplyblock_core/scripts/datasource.yml
 simplyblock_core/scripts/db_config_double.sh
 simplyblock_core/scripts/db_config_single.sh
 simplyblock_core/scripts/deploy_stack.sh
 simplyblock_core/scripts/docker-compose-swarm-monitoring.yml
```

## Comparing `sbcli_mc-1.0.5/sbcli_mc.egg-info/PKG-INFO` & `sbcli_mc-1.0.6/sbcli_mc.egg-info/PKG-INFO`

 * *Files 1% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: sbcli-mc
-Version: 1.0.5
+Version: 1.0.6
 Summary: CLI for managing SimplyBlock cluster
 Home-page: https://www.simplyblock.io/
 Author: Hamdy
 Author-email: hamdy@simplyblock.io
 Description-Content-Type: text/markdown
 Requires-Dist: foundationdb
 Requires-Dist: requests
```

