# Comparing `tmp/sbcli_dev-2.8.3.zip` & `tmp/sbcli_dev-2.8.4.zip`

## zipinfo {}

```diff
@@ -1,150 +1,150 @@
-Zip file size: 212532 bytes, number of entries: 148
-drwxr-xr-x  2.0 unx        0 b- stor 24-May-29 17:23 sbcli_dev-2.8.3/
-drwxr-xr-x  2.0 unx        0 b- stor 24-May-29 17:23 sbcli_dev-2.8.3/simplyblock_cli/
-drwxr-xr-x  2.0 unx        0 b- stor 24-May-29 17:23 sbcli_dev-2.8.3/simplyblock_web/
-drwxr-xr-x  2.0 unx        0 b- stor 24-May-29 17:23 sbcli_dev-2.8.3/sbcli_dev.egg-info/
-drwxr-xr-x  2.0 unx        0 b- stor 24-May-29 17:23 sbcli_dev-2.8.3/simplyblock_core/
--rw-r--r--  2.0 unx     1068 b- defN 24-May-29 17:23 sbcli_dev-2.8.3/README.md
--rw-r--r--  2.0 unx       84 b- defN 24-May-29 17:23 sbcli_dev-2.8.3/pyproject.toml
--rw-r--r--  2.0 unx     1489 b- defN 24-May-29 17:23 sbcli_dev-2.8.3/PKG-INFO
--rw-r--r--  2.0 unx      149 b- defN 24-May-29 17:23 sbcli_dev-2.8.3/env_var
--rw-r--r--  2.0 unx       38 b- defN 24-May-29 17:23 sbcli_dev-2.8.3/setup.cfg
--rw-r--r--  2.0 unx     2269 b- defN 24-May-29 17:23 sbcli_dev-2.8.3/setup.py
--rw-r--r--  2.0 unx    63179 b- defN 24-May-29 17:23 sbcli_dev-2.8.3/simplyblock_cli/cli.py
--rw-r--r--  2.0 unx      357 b- defN 24-May-29 17:23 sbcli_dev-2.8.3/simplyblock_cli/main.py
-drwxr-xr-x  2.0 unx        0 b- stor 24-May-29 17:23 sbcli_dev-2.8.3/simplyblock_web/static/
-drwxr-xr-x  2.0 unx        0 b- stor 24-May-29 17:23 sbcli_dev-2.8.3/simplyblock_web/blueprints/
-drwxr-xr-x  2.0 unx        0 b- stor 24-May-29 17:23 sbcli_dev-2.8.3/simplyblock_web/templates/
--rw-r--r--  2.0 unx        0 b- defN 24-May-29 17:23 sbcli_dev-2.8.3/simplyblock_web/__init__.py
--rw-r--r--  2.0 unx     1434 b- defN 24-May-29 17:23 sbcli_dev-2.8.3/simplyblock_web/node_webapp.py
--rw-r--r--  2.0 unx      703 b- defN 24-May-29 17:23 sbcli_dev-2.8.3/simplyblock_web/snode_app.py
--rw-r--r--  2.0 unx      717 b- defN 24-May-29 17:23 sbcli_dev-2.8.3/simplyblock_web/caching_node_app.py
--rw-r--r--  2.0 unx     1638 b- defN 24-May-29 17:23 sbcli_dev-2.8.3/simplyblock_web/auth_middleware.py
--rw-r--r--  2.0 unx     5098 b- defN 24-May-29 17:23 sbcli_dev-2.8.3/simplyblock_web/node_utils.py
--rw-r--r--  2.0 unx     2513 b- defN 24-May-29 17:23 sbcli_dev-2.8.3/simplyblock_web/utils.py
--rw-r--r--  2.0 unx     1284 b- defN 24-May-29 17:23 sbcli_dev-2.8.3/simplyblock_web/app.py
--rw-r--r--  2.0 unx      725 b- defN 24-May-29 17:23 sbcli_dev-2.8.3/simplyblock_web/caching_node_app_k8s.py
--rw-r--r--  2.0 unx      322 b- defN 24-May-29 17:23 sbcli_dev-2.8.3/simplyblock_web/static/tst.py
--rw-r--r--  2.0 unx      827 b- defN 24-May-29 17:23 sbcli_dev-2.8.3/simplyblock_web/static/delete.py
--rw-r--r--  2.0 unx      507 b- defN 24-May-29 17:23 sbcli_dev-2.8.3/simplyblock_web/static/deploy_cnode.yaml
--rw-r--r--  2.0 unx      434 b- defN 24-May-29 17:23 sbcli_dev-2.8.3/simplyblock_web/static/is_up.py
--rw-r--r--  2.0 unx     1466 b- defN 24-May-29 17:23 sbcli_dev-2.8.3/simplyblock_web/static/deploy_spdk.yaml
--rw-r--r--  2.0 unx      463 b- defN 24-May-29 17:23 sbcli_dev-2.8.3/simplyblock_web/static/rpac.yaml
--rw-r--r--  2.0 unx      417 b- defN 24-May-29 17:23 sbcli_dev-2.8.3/simplyblock_web/static/list_deps.py
--rw-r--r--  2.0 unx     1302 b- defN 24-May-29 17:23 sbcli_dev-2.8.3/simplyblock_web/static/deploy.py
--rw-r--r--  2.0 unx     6806 b- defN 24-May-29 17:23 sbcli_dev-2.8.3/simplyblock_web/blueprints/web_api_pool.py
--rw-r--r--  2.0 unx        0 b- defN 24-May-29 17:23 sbcli_dev-2.8.3/simplyblock_web/blueprints/__init__.py
--rw-r--r--  2.0 unx     2940 b- defN 24-May-29 17:23 sbcli_dev-2.8.3/simplyblock_web/blueprints/web_api_device.py
--rw-r--r--  2.0 unx     8685 b- defN 24-May-29 17:23 sbcli_dev-2.8.3/simplyblock_web/blueprints/web_api_lvol.py
--rw-r--r--  2.0 unx     9713 b- defN 24-May-29 17:23 sbcli_dev-2.8.3/simplyblock_web/blueprints/snode_ops.py
--rw-r--r--  2.0 unx    12385 b- defN 24-May-29 17:23 sbcli_dev-2.8.3/simplyblock_web/blueprints/caching_node_ops.py
--rw-r--r--  2.0 unx     6326 b- defN 24-May-29 17:23 sbcli_dev-2.8.3/simplyblock_web/blueprints/web_api_storage_node.py
--rw-r--r--  2.0 unx     5931 b- defN 24-May-29 17:23 sbcli_dev-2.8.3/simplyblock_web/blueprints/web_api_cluster.py
--rw-r--r--  2.0 unx     8075 b- defN 24-May-29 17:23 sbcli_dev-2.8.3/simplyblock_web/blueprints/caching_node_ops_k8s.py
--rw-r--r--  2.0 unx     4883 b- defN 24-May-29 17:23 sbcli_dev-2.8.3/simplyblock_web/blueprints/node_api_caching_ks.py
--rw-r--r--  2.0 unx     5746 b- defN 24-May-29 17:23 sbcli_dev-2.8.3/simplyblock_web/blueprints/node_api_caching_docker.py
--rw-r--r--  2.0 unx     5491 b- defN 24-May-29 17:23 sbcli_dev-2.8.3/simplyblock_web/blueprints/web_api_caching_node.py
--rw-r--r--  2.0 unx     3103 b- defN 24-May-29 17:23 sbcli_dev-2.8.3/simplyblock_web/blueprints/node_api_basic.py
--rw-r--r--  2.0 unx    11244 b- defN 24-May-29 17:23 sbcli_dev-2.8.3/simplyblock_web/blueprints/csi.py
--rw-r--r--  2.0 unx      975 b- defN 24-May-29 17:23 sbcli_dev-2.8.3/simplyblock_web/blueprints/web_api_mgmt_node.py
--rw-r--r--  2.0 unx     2905 b- defN 24-May-29 17:23 sbcli_dev-2.8.3/simplyblock_web/templates/deploy_spdk.yaml.j2
--rw-r--r--  2.0 unx     5267 b- defN 24-May-29 17:23 sbcli_dev-2.8.3/sbcli_dev.egg-info/SOURCES.txt
--rw-r--r--  2.0 unx       73 b- defN 24-May-29 17:23 sbcli_dev-2.8.3/sbcli_dev.egg-info/requires.txt
--rw-r--r--  2.0 unx     1489 b- defN 24-May-29 17:23 sbcli_dev-2.8.3/sbcli_dev.egg-info/PKG-INFO
--rw-r--r--  2.0 unx       49 b- defN 24-May-29 17:23 sbcli_dev-2.8.3/sbcli_dev.egg-info/top_level.txt
--rw-r--r--  2.0 unx       55 b- defN 24-May-29 17:23 sbcli_dev-2.8.3/sbcli_dev.egg-info/entry_points.txt
--rw-r--r--  2.0 unx        1 b- defN 24-May-29 17:23 sbcli_dev-2.8.3/sbcli_dev.egg-info/dependency_links.txt
-drwxr-xr-x  2.0 unx        0 b- stor 24-May-29 17:23 sbcli_dev-2.8.3/simplyblock_core/services/
-drwxr-xr-x  2.0 unx        0 b- stor 24-May-29 17:23 sbcli_dev-2.8.3/simplyblock_core/controllers/
-drwxr-xr-x  2.0 unx        0 b- stor 24-May-29 17:23 sbcli_dev-2.8.3/simplyblock_core/models/
-drwxr-xr-x  2.0 unx        0 b- stor 24-May-29 17:23 sbcli_dev-2.8.3/simplyblock_core/scripts/
--rw-r--r--  2.0 unx    25292 b- defN 24-May-29 17:23 sbcli_dev-2.8.3/simplyblock_core/cluster_ops.py
--rw-r--r--  2.0 unx      938 b- defN 24-May-29 17:23 sbcli_dev-2.8.3/simplyblock_core/pci_utils.py
--rw-r--r--  2.0 unx        0 b- defN 24-May-29 17:23 sbcli_dev-2.8.3/simplyblock_core/__init__.py
--rw-r--r--  2.0 unx     3193 b- defN 24-May-29 17:23 sbcli_dev-2.8.3/simplyblock_core/snode_client.py
--rw-r--r--  2.0 unx     8532 b- defN 24-May-29 17:23 sbcli_dev-2.8.3/simplyblock_core/kv_store.py
--rw-r--r--  2.0 unx     5112 b- defN 24-May-29 17:23 sbcli_dev-2.8.3/simplyblock_core/compute_node_ops.py
--rw-r--r--  2.0 unx    20829 b- defN 24-May-29 17:23 sbcli_dev-2.8.3/simplyblock_core/rpc_client.py
--rw-r--r--  2.0 unx     1986 b- defN 24-May-29 17:23 sbcli_dev-2.8.3/simplyblock_core/mgmt_node_ops.py
--rw-r--r--  2.0 unx     7640 b- defN 24-May-29 17:23 sbcli_dev-2.8.3/simplyblock_core/utils.py
--rw-r--r--  2.0 unx     7504 b- defN 24-May-29 17:23 sbcli_dev-2.8.3/simplyblock_core/distr_controller.py
--rw-r--r--  2.0 unx      279 b- defN 24-May-29 17:23 sbcli_dev-2.8.3/simplyblock_core/shell_utils.py
--rw-r--r--  2.0 unx     3638 b- defN 24-May-29 17:23 sbcli_dev-2.8.3/simplyblock_core/cnode_client.py
--rw-r--r--  2.0 unx    64980 b- defN 24-May-29 17:23 sbcli_dev-2.8.3/simplyblock_core/storage_node_ops.py
--rw-r--r--  2.0 unx     1566 b- defN 24-May-29 17:23 sbcli_dev-2.8.3/simplyblock_core/constants.py
--rw-r--r--  2.0 unx     3542 b- defN 24-May-29 17:23 sbcli_dev-2.8.3/simplyblock_core/services/job_tasks.py
--rw-r--r--  2.0 unx     3203 b- defN 24-May-29 17:23 sbcli_dev-2.8.3/simplyblock_core/services/caching_node_monitor.py
--rw-r--r--  2.0 unx      229 b- defN 24-May-29 17:23 sbcli_dev-2.8.3/simplyblock_core/services/service_template.service
--rw-r--r--  2.0 unx      837 b- defN 24-May-29 17:23 sbcli_dev-2.8.3/simplyblock_core/services/install_service.sh
--rw-r--r--  2.0 unx     4118 b- defN 24-May-29 17:23 sbcli_dev-2.8.3/simplyblock_core/services/__init__.py
--rw-r--r--  2.0 unx     2410 b- defN 24-May-29 17:23 sbcli_dev-2.8.3/simplyblock_core/services/log_agg_service.py
--rw-r--r--  2.0 unx     5462 b- defN 24-May-29 17:23 sbcli_dev-2.8.3/simplyblock_core/services/health_check_service.py
--rw-r--r--  2.0 unx     7439 b- defN 24-May-29 17:23 sbcli_dev-2.8.3/simplyblock_core/services/capacity_and_stats_collector.py
--rw-r--r--  2.0 unx     3169 b- defN 24-May-29 17:23 sbcli_dev-2.8.3/simplyblock_core/services/device_monitor.py
--rw-r--r--  2.0 unx     5268 b- defN 24-May-29 17:23 sbcli_dev-2.8.3/simplyblock_core/services/lvol_stat_collector.py
--rw-r--r--  2.0 unx     2671 b- defN 24-May-29 17:23 sbcli_dev-2.8.3/simplyblock_core/services/cap_monitor.py
--rw-r--r--  2.0 unx     6577 b- defN 24-May-29 17:23 sbcli_dev-2.8.3/simplyblock_core/services/storage_node_monitor.py
--rw-r--r--  2.0 unx     2423 b- defN 24-May-29 17:23 sbcli_dev-2.8.3/simplyblock_core/services/port_stat_collector.py
--rw-r--r--  2.0 unx     5140 b- defN 24-May-29 17:23 sbcli_dev-2.8.3/simplyblock_core/services/distr_event_collector.py
--rw-r--r--  2.0 unx      173 b- defN 24-May-29 17:23 sbcli_dev-2.8.3/simplyblock_core/services/remove_service.sh
--rw-r--r--  2.0 unx     3003 b- defN 24-May-29 17:23 sbcli_dev-2.8.3/simplyblock_core/services/mgmt_node_monitor.py
--rw-r--r--  2.0 unx     2189 b- defN 24-May-29 17:23 sbcli_dev-2.8.3/simplyblock_core/services/lvol_monitor.py
--rw-r--r--  2.0 unx    10375 b- defN 24-May-29 17:23 sbcli_dev-2.8.3/simplyblock_core/controllers/pool_controller.py
--rw-r--r--  2.0 unx        0 b- defN 24-May-29 17:23 sbcli_dev-2.8.3/simplyblock_core/controllers/__init__.py
--rw-r--r--  2.0 unx     1521 b- defN 24-May-29 17:23 sbcli_dev-2.8.3/simplyblock_core/controllers/storage_events.py
--rw-r--r--  2.0 unx    48478 b- defN 24-May-29 17:23 sbcli_dev-2.8.3/simplyblock_core/controllers/lvol_controller.py
--rw-r--r--  2.0 unx     1568 b- defN 24-May-29 17:23 sbcli_dev-2.8.3/simplyblock_core/controllers/device_events.py
--rw-r--r--  2.0 unx     1630 b- defN 24-May-29 17:23 sbcli_dev-2.8.3/simplyblock_core/controllers/lvol_events.py
--rw-r--r--  2.0 unx    10874 b- defN 24-May-29 17:23 sbcli_dev-2.8.3/simplyblock_core/controllers/snapshot_controller.py
--rw-r--r--  2.0 unx     1122 b- defN 24-May-29 17:23 sbcli_dev-2.8.3/simplyblock_core/controllers/snapshot_events.py
--rw-r--r--  2.0 unx     3191 b- defN 24-May-29 17:23 sbcli_dev-2.8.3/simplyblock_core/controllers/events_controller.py
--rw-r--r--  2.0 unx    11294 b- defN 24-May-29 17:23 sbcli_dev-2.8.3/simplyblock_core/controllers/health_controller.py
--rw-r--r--  2.0 unx    13916 b- defN 24-May-29 17:23 sbcli_dev-2.8.3/simplyblock_core/controllers/device_controller.py
--rw-r--r--  2.0 unx      695 b- defN 24-May-29 17:23 sbcli_dev-2.8.3/simplyblock_core/controllers/pool_events.py
--rw-r--r--  2.0 unx    23312 b- defN 24-May-29 17:23 sbcli_dev-2.8.3/simplyblock_core/controllers/caching_node_controller.py
--rw-r--r--  2.0 unx     1900 b- defN 24-May-29 17:23 sbcli_dev-2.8.3/simplyblock_core/controllers/cluster_events.py
--rw-r--r--  2.0 unx     1120 b- defN 24-May-29 17:23 sbcli_dev-2.8.3/simplyblock_core/controllers/mgmt_events.py
--rw-r--r--  2.0 unx     3766 b- defN 24-May-29 17:23 sbcli_dev-2.8.3/simplyblock_core/models/caching_node.py
--rw-r--r--  2.0 unx     2094 b- defN 24-May-29 17:23 sbcli_dev-2.8.3/simplyblock_core/models/nvme_device.py
--rw-r--r--  2.0 unx     1452 b- defN 24-May-29 17:23 sbcli_dev-2.8.3/simplyblock_core/models/mgmt_node.py
--rw-r--r--  2.0 unx      917 b- defN 24-May-29 17:23 sbcli_dev-2.8.3/simplyblock_core/models/compute_node.py
--rw-r--r--  2.0 unx        0 b- defN 24-May-29 17:23 sbcli_dev-2.8.3/simplyblock_core/models/__init__.py
--rw-r--r--  2.0 unx     1500 b- defN 24-May-29 17:23 sbcli_dev-2.8.3/simplyblock_core/models/events.py
--rw-r--r--  2.0 unx     1228 b- defN 24-May-29 17:23 sbcli_dev-2.8.3/simplyblock_core/models/global_settings.py
--rw-r--r--  2.0 unx      973 b- defN 24-May-29 17:23 sbcli_dev-2.8.3/simplyblock_core/models/job_schedule.py
--rw-r--r--  2.0 unx     4846 b- defN 24-May-29 17:23 sbcli_dev-2.8.3/simplyblock_core/models/base_model.py
--rw-r--r--  2.0 unx     2579 b- defN 24-May-29 17:23 sbcli_dev-2.8.3/simplyblock_core/models/lvol_model.py
--rw-r--r--  2.0 unx      736 b- defN 24-May-29 17:23 sbcli_dev-2.8.3/simplyblock_core/models/snapshot.py
--rw-r--r--  2.0 unx     3696 b- defN 24-May-29 17:23 sbcli_dev-2.8.3/simplyblock_core/models/storage_node.py
--rw-r--r--  2.0 unx     4242 b- defN 24-May-29 17:23 sbcli_dev-2.8.3/simplyblock_core/models/stats.py
--rw-r--r--  2.0 unx     1602 b- defN 24-May-29 17:23 sbcli_dev-2.8.3/simplyblock_core/models/pool.py
--rw-r--r--  2.0 unx      806 b- defN 24-May-29 17:23 sbcli_dev-2.8.3/simplyblock_core/models/iface.py
--rw-r--r--  2.0 unx     2565 b- defN 24-May-29 17:23 sbcli_dev-2.8.3/simplyblock_core/models/cluster.py
--rw-r--r--  2.0 unx     1020 b- defN 24-May-29 17:23 sbcli_dev-2.8.3/simplyblock_core/models/port_stat.py
-drwxr-xr-x  2.0 unx        0 b- stor 24-May-29 17:23 sbcli_dev-2.8.3/simplyblock_core/scripts/alerting/
-drwxr-xr-x  2.0 unx        0 b- stor 24-May-29 17:23 sbcli_dev-2.8.3/simplyblock_core/scripts/dashboards/
--rw-r--r--  2.0 unx     1420 b- defN 24-May-29 17:23 sbcli_dev-2.8.3/simplyblock_core/scripts/install_deps.sh
--rw-r--r--  2.0 unx     1782 b- defN 24-May-29 17:23 sbcli_dev-2.8.3/simplyblock_core/scripts/__init__.py
--rw-r--r--  2.0 unx       43 b- defN 24-May-29 17:23 sbcli_dev-2.8.3/simplyblock_core/scripts/run_ssh.sh
--rw-r--r--  2.0 unx     1163 b- defN 24-May-29 17:23 sbcli_dev-2.8.3/simplyblock_core/scripts/haproxy.cfg
--rw-r--r--  2.0 unx      118 b- defN 24-May-29 17:23 sbcli_dev-2.8.3/simplyblock_core/scripts/db_config_double.sh
--rw-r--r--  2.0 unx     5305 b- defN 24-May-29 17:23 sbcli_dev-2.8.3/simplyblock_core/scripts/stack_deploy_wait.sh
--rw-r--r--  2.0 unx      360 b- defN 24-May-29 17:23 sbcli_dev-2.8.3/simplyblock_core/scripts/datasource.yml
--rw-r--r--  2.0 unx     5611 b- defN 24-May-29 17:23 sbcli_dev-2.8.3/simplyblock_core/scripts/docker-compose-swarm.yml
--rw-r--r--  2.0 unx      152 b- defN 24-May-29 17:23 sbcli_dev-2.8.3/simplyblock_core/scripts/set_db_config.sh
--rwxr-xr-x  2.0 unx      657 b- defN 24-May-29 17:23 sbcli_dev-2.8.3/simplyblock_core/scripts/apply_dashboard.sh
--rw-r--r--  2.0 unx      311 b- defN 24-May-29 17:23 sbcli_dev-2.8.3/simplyblock_core/scripts/prometheus.yml
--rw-r--r--  2.0 unx      342 b- defN 24-May-29 17:23 sbcli_dev-2.8.3/simplyblock_core/scripts/clean_local_storage_deploy.sh
--rw-r--r--  2.0 unx     4409 b- defN 24-May-29 17:23 sbcli_dev-2.8.3/simplyblock_core/scripts/docker-compose-swarm-monitoring.yml
--rw-r--r--  2.0 unx      930 b- defN 24-May-29 17:23 sbcli_dev-2.8.3/simplyblock_core/scripts/deploy_stack.sh
--rw-r--r--  2.0 unx       54 b- defN 24-May-29 17:23 sbcli_dev-2.8.3/simplyblock_core/scripts/db_config_single.sh
--rw-r--r--  2.0 unx      453 b- defN 24-May-29 17:23 sbcli_dev-2.8.3/simplyblock_core/scripts/config_docker.sh
--rw-r--r--  2.0 unx    25433 b- defN 24-May-29 17:23 sbcli_dev-2.8.3/simplyblock_core/scripts/alerting/alert_rules.yaml
--rw-r--r--  2.0 unx     1856 b- defN 24-May-29 17:23 sbcli_dev-2.8.3/simplyblock_core/scripts/alerting/alert_resources.yaml
--rw-r--r--  2.0 unx    88820 b- defN 24-May-29 17:23 sbcli_dev-2.8.3/simplyblock_core/scripts/dashboards/nodes.json
--rw-r--r--  2.0 unx    88911 b- defN 24-May-29 17:23 sbcli_dev-2.8.3/simplyblock_core/scripts/dashboards/cluster.json
--rw-r--r--  2.0 unx    88776 b- defN 24-May-29 17:23 sbcli_dev-2.8.3/simplyblock_core/scripts/dashboards/lvols.json
--rw-r--r--  2.0 unx    88868 b- defN 24-May-29 17:23 sbcli_dev-2.8.3/simplyblock_core/scripts/dashboards/devices.json
--rw-r--r--  2.0 unx    99707 b- defN 24-May-29 17:23 sbcli_dev-2.8.3/simplyblock_core/scripts/dashboards/pools.json
--rw-r--r--  2.0 unx   799409 b- defN 24-May-29 17:23 sbcli_dev-2.8.3/simplyblock_core/scripts/dashboards/node-exporter.json
-148 files, 1869875 bytes uncompressed, 185584 bytes compressed:  90.1%
+Zip file size: 214419 bytes, number of entries: 148
+drwxr-xr-x  2.0 unx        0 b- stor 24-May-30 17:11 sbcli_dev-2.8.4/
+drwxr-xr-x  2.0 unx        0 b- stor 24-May-30 17:11 sbcli_dev-2.8.4/simplyblock_cli/
+drwxr-xr-x  2.0 unx        0 b- stor 24-May-30 17:11 sbcli_dev-2.8.4/simplyblock_web/
+drwxr-xr-x  2.0 unx        0 b- stor 24-May-30 17:11 sbcli_dev-2.8.4/sbcli_dev.egg-info/
+drwxr-xr-x  2.0 unx        0 b- stor 24-May-30 17:11 sbcli_dev-2.8.4/simplyblock_core/
+-rw-r--r--  2.0 unx     1068 b- defN 24-May-30 17:11 sbcli_dev-2.8.4/README.md
+-rw-r--r--  2.0 unx       84 b- defN 24-May-30 17:11 sbcli_dev-2.8.4/pyproject.toml
+-rw-r--r--  2.0 unx     1489 b- defN 24-May-30 17:11 sbcli_dev-2.8.4/PKG-INFO
+-rw-r--r--  2.0 unx      149 b- defN 24-May-30 17:11 sbcli_dev-2.8.4/env_var
+-rw-r--r--  2.0 unx       38 b- defN 24-May-30 17:11 sbcli_dev-2.8.4/setup.cfg
+-rw-r--r--  2.0 unx     2269 b- defN 24-May-30 17:11 sbcli_dev-2.8.4/setup.py
+-rw-r--r--  2.0 unx    63179 b- defN 24-May-30 17:11 sbcli_dev-2.8.4/simplyblock_cli/cli.py
+-rw-r--r--  2.0 unx      357 b- defN 24-May-30 17:11 sbcli_dev-2.8.4/simplyblock_cli/main.py
+drwxr-xr-x  2.0 unx        0 b- stor 24-May-30 17:11 sbcli_dev-2.8.4/simplyblock_web/static/
+drwxr-xr-x  2.0 unx        0 b- stor 24-May-30 17:11 sbcli_dev-2.8.4/simplyblock_web/blueprints/
+drwxr-xr-x  2.0 unx        0 b- stor 24-May-30 17:11 sbcli_dev-2.8.4/simplyblock_web/templates/
+-rw-r--r--  2.0 unx        0 b- defN 24-May-30 17:11 sbcli_dev-2.8.4/simplyblock_web/__init__.py
+-rw-r--r--  2.0 unx     1434 b- defN 24-May-30 17:11 sbcli_dev-2.8.4/simplyblock_web/node_webapp.py
+-rw-r--r--  2.0 unx      703 b- defN 24-May-30 17:11 sbcli_dev-2.8.4/simplyblock_web/snode_app.py
+-rw-r--r--  2.0 unx      717 b- defN 24-May-30 17:11 sbcli_dev-2.8.4/simplyblock_web/caching_node_app.py
+-rw-r--r--  2.0 unx     1638 b- defN 24-May-30 17:11 sbcli_dev-2.8.4/simplyblock_web/auth_middleware.py
+-rw-r--r--  2.0 unx     5098 b- defN 24-May-30 17:11 sbcli_dev-2.8.4/simplyblock_web/node_utils.py
+-rw-r--r--  2.0 unx     2513 b- defN 24-May-30 17:11 sbcli_dev-2.8.4/simplyblock_web/utils.py
+-rw-r--r--  2.0 unx     1284 b- defN 24-May-30 17:11 sbcli_dev-2.8.4/simplyblock_web/app.py
+-rw-r--r--  2.0 unx      725 b- defN 24-May-30 17:11 sbcli_dev-2.8.4/simplyblock_web/caching_node_app_k8s.py
+-rw-r--r--  2.0 unx      322 b- defN 24-May-30 17:11 sbcli_dev-2.8.4/simplyblock_web/static/tst.py
+-rw-r--r--  2.0 unx      827 b- defN 24-May-30 17:11 sbcli_dev-2.8.4/simplyblock_web/static/delete.py
+-rw-r--r--  2.0 unx      507 b- defN 24-May-30 17:11 sbcli_dev-2.8.4/simplyblock_web/static/deploy_cnode.yaml
+-rw-r--r--  2.0 unx      434 b- defN 24-May-30 17:11 sbcli_dev-2.8.4/simplyblock_web/static/is_up.py
+-rw-r--r--  2.0 unx     1466 b- defN 24-May-30 17:11 sbcli_dev-2.8.4/simplyblock_web/static/deploy_spdk.yaml
+-rw-r--r--  2.0 unx      463 b- defN 24-May-30 17:11 sbcli_dev-2.8.4/simplyblock_web/static/rpac.yaml
+-rw-r--r--  2.0 unx      417 b- defN 24-May-30 17:11 sbcli_dev-2.8.4/simplyblock_web/static/list_deps.py
+-rw-r--r--  2.0 unx     1302 b- defN 24-May-30 17:11 sbcli_dev-2.8.4/simplyblock_web/static/deploy.py
+-rw-r--r--  2.0 unx     6806 b- defN 24-May-30 17:11 sbcli_dev-2.8.4/simplyblock_web/blueprints/web_api_pool.py
+-rw-r--r--  2.0 unx        0 b- defN 24-May-30 17:11 sbcli_dev-2.8.4/simplyblock_web/blueprints/__init__.py
+-rw-r--r--  2.0 unx     2940 b- defN 24-May-30 17:11 sbcli_dev-2.8.4/simplyblock_web/blueprints/web_api_device.py
+-rw-r--r--  2.0 unx     8685 b- defN 24-May-30 17:11 sbcli_dev-2.8.4/simplyblock_web/blueprints/web_api_lvol.py
+-rw-r--r--  2.0 unx     9713 b- defN 24-May-30 17:11 sbcli_dev-2.8.4/simplyblock_web/blueprints/snode_ops.py
+-rw-r--r--  2.0 unx    12385 b- defN 24-May-30 17:11 sbcli_dev-2.8.4/simplyblock_web/blueprints/caching_node_ops.py
+-rw-r--r--  2.0 unx     6326 b- defN 24-May-30 17:11 sbcli_dev-2.8.4/simplyblock_web/blueprints/web_api_storage_node.py
+-rw-r--r--  2.0 unx     5931 b- defN 24-May-30 17:11 sbcli_dev-2.8.4/simplyblock_web/blueprints/web_api_cluster.py
+-rw-r--r--  2.0 unx     8075 b- defN 24-May-30 17:11 sbcli_dev-2.8.4/simplyblock_web/blueprints/caching_node_ops_k8s.py
+-rw-r--r--  2.0 unx     4883 b- defN 24-May-30 17:11 sbcli_dev-2.8.4/simplyblock_web/blueprints/node_api_caching_ks.py
+-rw-r--r--  2.0 unx     5746 b- defN 24-May-30 17:11 sbcli_dev-2.8.4/simplyblock_web/blueprints/node_api_caching_docker.py
+-rw-r--r--  2.0 unx     5491 b- defN 24-May-30 17:11 sbcli_dev-2.8.4/simplyblock_web/blueprints/web_api_caching_node.py
+-rw-r--r--  2.0 unx     3103 b- defN 24-May-30 17:11 sbcli_dev-2.8.4/simplyblock_web/blueprints/node_api_basic.py
+-rw-r--r--  2.0 unx    11244 b- defN 24-May-30 17:11 sbcli_dev-2.8.4/simplyblock_web/blueprints/csi.py
+-rw-r--r--  2.0 unx      975 b- defN 24-May-30 17:11 sbcli_dev-2.8.4/simplyblock_web/blueprints/web_api_mgmt_node.py
+-rw-r--r--  2.0 unx     2905 b- defN 24-May-30 17:11 sbcli_dev-2.8.4/simplyblock_web/templates/deploy_spdk.yaml.j2
+-rw-r--r--  2.0 unx     5267 b- defN 24-May-30 17:11 sbcli_dev-2.8.4/sbcli_dev.egg-info/SOURCES.txt
+-rw-r--r--  2.0 unx       73 b- defN 24-May-30 17:11 sbcli_dev-2.8.4/sbcli_dev.egg-info/requires.txt
+-rw-r--r--  2.0 unx     1489 b- defN 24-May-30 17:11 sbcli_dev-2.8.4/sbcli_dev.egg-info/PKG-INFO
+-rw-r--r--  2.0 unx       49 b- defN 24-May-30 17:11 sbcli_dev-2.8.4/sbcli_dev.egg-info/top_level.txt
+-rw-r--r--  2.0 unx       55 b- defN 24-May-30 17:11 sbcli_dev-2.8.4/sbcli_dev.egg-info/entry_points.txt
+-rw-r--r--  2.0 unx        1 b- defN 24-May-30 17:11 sbcli_dev-2.8.4/sbcli_dev.egg-info/dependency_links.txt
+drwxr-xr-x  2.0 unx        0 b- stor 24-May-30 17:11 sbcli_dev-2.8.4/simplyblock_core/services/
+drwxr-xr-x  2.0 unx        0 b- stor 24-May-30 17:11 sbcli_dev-2.8.4/simplyblock_core/controllers/
+drwxr-xr-x  2.0 unx        0 b- stor 24-May-30 17:11 sbcli_dev-2.8.4/simplyblock_core/models/
+drwxr-xr-x  2.0 unx        0 b- stor 24-May-30 17:11 sbcli_dev-2.8.4/simplyblock_core/scripts/
+-rw-r--r--  2.0 unx    25331 b- defN 24-May-30 17:11 sbcli_dev-2.8.4/simplyblock_core/cluster_ops.py
+-rw-r--r--  2.0 unx      938 b- defN 24-May-30 17:11 sbcli_dev-2.8.4/simplyblock_core/pci_utils.py
+-rw-r--r--  2.0 unx        0 b- defN 24-May-30 17:11 sbcli_dev-2.8.4/simplyblock_core/__init__.py
+-rw-r--r--  2.0 unx     3193 b- defN 24-May-30 17:11 sbcli_dev-2.8.4/simplyblock_core/snode_client.py
+-rw-r--r--  2.0 unx     8532 b- defN 24-May-30 17:11 sbcli_dev-2.8.4/simplyblock_core/kv_store.py
+-rw-r--r--  2.0 unx     5112 b- defN 24-May-30 17:11 sbcli_dev-2.8.4/simplyblock_core/compute_node_ops.py
+-rw-r--r--  2.0 unx    20829 b- defN 24-May-30 17:11 sbcli_dev-2.8.4/simplyblock_core/rpc_client.py
+-rw-r--r--  2.0 unx     1986 b- defN 24-May-30 17:11 sbcli_dev-2.8.4/simplyblock_core/mgmt_node_ops.py
+-rw-r--r--  2.0 unx     7640 b- defN 24-May-30 17:11 sbcli_dev-2.8.4/simplyblock_core/utils.py
+-rw-r--r--  2.0 unx     7504 b- defN 24-May-30 17:11 sbcli_dev-2.8.4/simplyblock_core/distr_controller.py
+-rw-r--r--  2.0 unx      279 b- defN 24-May-30 17:11 sbcli_dev-2.8.4/simplyblock_core/shell_utils.py
+-rw-r--r--  2.0 unx     3638 b- defN 24-May-30 17:11 sbcli_dev-2.8.4/simplyblock_core/cnode_client.py
+-rw-r--r--  2.0 unx    64980 b- defN 24-May-30 17:11 sbcli_dev-2.8.4/simplyblock_core/storage_node_ops.py
+-rw-r--r--  2.0 unx     1592 b- defN 24-May-30 17:11 sbcli_dev-2.8.4/simplyblock_core/constants.py
+-rw-r--r--  2.0 unx     3767 b- defN 24-May-30 17:11 sbcli_dev-2.8.4/simplyblock_core/services/job_tasks.py
+-rw-r--r--  2.0 unx     3203 b- defN 24-May-30 17:11 sbcli_dev-2.8.4/simplyblock_core/services/caching_node_monitor.py
+-rw-r--r--  2.0 unx      229 b- defN 24-May-30 17:11 sbcli_dev-2.8.4/simplyblock_core/services/service_template.service
+-rw-r--r--  2.0 unx      837 b- defN 24-May-30 17:11 sbcli_dev-2.8.4/simplyblock_core/services/install_service.sh
+-rw-r--r--  2.0 unx     4118 b- defN 24-May-30 17:11 sbcli_dev-2.8.4/simplyblock_core/services/__init__.py
+-rw-r--r--  2.0 unx     2410 b- defN 24-May-30 17:11 sbcli_dev-2.8.4/simplyblock_core/services/log_agg_service.py
+-rw-r--r--  2.0 unx     5462 b- defN 24-May-30 17:11 sbcli_dev-2.8.4/simplyblock_core/services/health_check_service.py
+-rw-r--r--  2.0 unx     7439 b- defN 24-May-30 17:11 sbcli_dev-2.8.4/simplyblock_core/services/capacity_and_stats_collector.py
+-rw-r--r--  2.0 unx     3169 b- defN 24-May-30 17:11 sbcli_dev-2.8.4/simplyblock_core/services/device_monitor.py
+-rw-r--r--  2.0 unx     5268 b- defN 24-May-30 17:11 sbcli_dev-2.8.4/simplyblock_core/services/lvol_stat_collector.py
+-rw-r--r--  2.0 unx     2671 b- defN 24-May-30 17:11 sbcli_dev-2.8.4/simplyblock_core/services/cap_monitor.py
+-rw-r--r--  2.0 unx     6577 b- defN 24-May-30 17:11 sbcli_dev-2.8.4/simplyblock_core/services/storage_node_monitor.py
+-rw-r--r--  2.0 unx     2423 b- defN 24-May-30 17:11 sbcli_dev-2.8.4/simplyblock_core/services/port_stat_collector.py
+-rw-r--r--  2.0 unx     5140 b- defN 24-May-30 17:11 sbcli_dev-2.8.4/simplyblock_core/services/distr_event_collector.py
+-rw-r--r--  2.0 unx      173 b- defN 24-May-30 17:11 sbcli_dev-2.8.4/simplyblock_core/services/remove_service.sh
+-rw-r--r--  2.0 unx     3003 b- defN 24-May-30 17:11 sbcli_dev-2.8.4/simplyblock_core/services/mgmt_node_monitor.py
+-rw-r--r--  2.0 unx     2189 b- defN 24-May-30 17:11 sbcli_dev-2.8.4/simplyblock_core/services/lvol_monitor.py
+-rw-r--r--  2.0 unx    10375 b- defN 24-May-30 17:11 sbcli_dev-2.8.4/simplyblock_core/controllers/pool_controller.py
+-rw-r--r--  2.0 unx        0 b- defN 24-May-30 17:11 sbcli_dev-2.8.4/simplyblock_core/controllers/__init__.py
+-rw-r--r--  2.0 unx     1521 b- defN 24-May-30 17:11 sbcli_dev-2.8.4/simplyblock_core/controllers/storage_events.py
+-rw-r--r--  2.0 unx    48478 b- defN 24-May-30 17:11 sbcli_dev-2.8.4/simplyblock_core/controllers/lvol_controller.py
+-rw-r--r--  2.0 unx     1568 b- defN 24-May-30 17:11 sbcli_dev-2.8.4/simplyblock_core/controllers/device_events.py
+-rw-r--r--  2.0 unx     1630 b- defN 24-May-30 17:11 sbcli_dev-2.8.4/simplyblock_core/controllers/lvol_events.py
+-rw-r--r--  2.0 unx    10874 b- defN 24-May-30 17:11 sbcli_dev-2.8.4/simplyblock_core/controllers/snapshot_controller.py
+-rw-r--r--  2.0 unx     1122 b- defN 24-May-30 17:11 sbcli_dev-2.8.4/simplyblock_core/controllers/snapshot_events.py
+-rw-r--r--  2.0 unx     3191 b- defN 24-May-30 17:11 sbcli_dev-2.8.4/simplyblock_core/controllers/events_controller.py
+-rw-r--r--  2.0 unx    11294 b- defN 24-May-30 17:11 sbcli_dev-2.8.4/simplyblock_core/controllers/health_controller.py
+-rw-r--r--  2.0 unx    13916 b- defN 24-May-30 17:11 sbcli_dev-2.8.4/simplyblock_core/controllers/device_controller.py
+-rw-r--r--  2.0 unx      695 b- defN 24-May-30 17:11 sbcli_dev-2.8.4/simplyblock_core/controllers/pool_events.py
+-rw-r--r--  2.0 unx    23312 b- defN 24-May-30 17:11 sbcli_dev-2.8.4/simplyblock_core/controllers/caching_node_controller.py
+-rw-r--r--  2.0 unx     1900 b- defN 24-May-30 17:11 sbcli_dev-2.8.4/simplyblock_core/controllers/cluster_events.py
+-rw-r--r--  2.0 unx     1120 b- defN 24-May-30 17:11 sbcli_dev-2.8.4/simplyblock_core/controllers/mgmt_events.py
+-rw-r--r--  2.0 unx     3766 b- defN 24-May-30 17:11 sbcli_dev-2.8.4/simplyblock_core/models/caching_node.py
+-rw-r--r--  2.0 unx     2094 b- defN 24-May-30 17:11 sbcli_dev-2.8.4/simplyblock_core/models/nvme_device.py
+-rw-r--r--  2.0 unx     1452 b- defN 24-May-30 17:11 sbcli_dev-2.8.4/simplyblock_core/models/mgmt_node.py
+-rw-r--r--  2.0 unx      917 b- defN 24-May-30 17:11 sbcli_dev-2.8.4/simplyblock_core/models/compute_node.py
+-rw-r--r--  2.0 unx        0 b- defN 24-May-30 17:11 sbcli_dev-2.8.4/simplyblock_core/models/__init__.py
+-rw-r--r--  2.0 unx     1500 b- defN 24-May-30 17:11 sbcli_dev-2.8.4/simplyblock_core/models/events.py
+-rw-r--r--  2.0 unx     1228 b- defN 24-May-30 17:11 sbcli_dev-2.8.4/simplyblock_core/models/global_settings.py
+-rw-r--r--  2.0 unx      973 b- defN 24-May-30 17:11 sbcli_dev-2.8.4/simplyblock_core/models/job_schedule.py
+-rw-r--r--  2.0 unx     4846 b- defN 24-May-30 17:11 sbcli_dev-2.8.4/simplyblock_core/models/base_model.py
+-rw-r--r--  2.0 unx     2579 b- defN 24-May-30 17:11 sbcli_dev-2.8.4/simplyblock_core/models/lvol_model.py
+-rw-r--r--  2.0 unx      736 b- defN 24-May-30 17:11 sbcli_dev-2.8.4/simplyblock_core/models/snapshot.py
+-rw-r--r--  2.0 unx     3696 b- defN 24-May-30 17:11 sbcli_dev-2.8.4/simplyblock_core/models/storage_node.py
+-rw-r--r--  2.0 unx     4242 b- defN 24-May-30 17:11 sbcli_dev-2.8.4/simplyblock_core/models/stats.py
+-rw-r--r--  2.0 unx     1602 b- defN 24-May-30 17:11 sbcli_dev-2.8.4/simplyblock_core/models/pool.py
+-rw-r--r--  2.0 unx      806 b- defN 24-May-30 17:11 sbcli_dev-2.8.4/simplyblock_core/models/iface.py
+-rw-r--r--  2.0 unx     2565 b- defN 24-May-30 17:11 sbcli_dev-2.8.4/simplyblock_core/models/cluster.py
+-rw-r--r--  2.0 unx     1020 b- defN 24-May-30 17:11 sbcli_dev-2.8.4/simplyblock_core/models/port_stat.py
+drwxr-xr-x  2.0 unx        0 b- stor 24-May-30 17:11 sbcli_dev-2.8.4/simplyblock_core/scripts/alerting/
+drwxr-xr-x  2.0 unx        0 b- stor 24-May-30 17:11 sbcli_dev-2.8.4/simplyblock_core/scripts/dashboards/
+-rw-r--r--  2.0 unx     1420 b- defN 24-May-30 17:11 sbcli_dev-2.8.4/simplyblock_core/scripts/install_deps.sh
+-rw-r--r--  2.0 unx     1782 b- defN 24-May-30 17:11 sbcli_dev-2.8.4/simplyblock_core/scripts/__init__.py
+-rw-r--r--  2.0 unx       43 b- defN 24-May-30 17:11 sbcli_dev-2.8.4/simplyblock_core/scripts/run_ssh.sh
+-rw-r--r--  2.0 unx     1163 b- defN 24-May-30 17:11 sbcli_dev-2.8.4/simplyblock_core/scripts/haproxy.cfg
+-rw-r--r--  2.0 unx      118 b- defN 24-May-30 17:11 sbcli_dev-2.8.4/simplyblock_core/scripts/db_config_double.sh
+-rw-r--r--  2.0 unx     5305 b- defN 24-May-30 17:11 sbcli_dev-2.8.4/simplyblock_core/scripts/stack_deploy_wait.sh
+-rw-r--r--  2.0 unx      360 b- defN 24-May-30 17:11 sbcli_dev-2.8.4/simplyblock_core/scripts/datasource.yml
+-rw-r--r--  2.0 unx     5611 b- defN 24-May-30 17:11 sbcli_dev-2.8.4/simplyblock_core/scripts/docker-compose-swarm.yml
+-rw-r--r--  2.0 unx      152 b- defN 24-May-30 17:11 sbcli_dev-2.8.4/simplyblock_core/scripts/set_db_config.sh
+-rwxr-xr-x  2.0 unx      657 b- defN 24-May-30 17:11 sbcli_dev-2.8.4/simplyblock_core/scripts/apply_dashboard.sh
+-rw-r--r--  2.0 unx      311 b- defN 24-May-30 17:11 sbcli_dev-2.8.4/simplyblock_core/scripts/prometheus.yml
+-rw-r--r--  2.0 unx      342 b- defN 24-May-30 17:11 sbcli_dev-2.8.4/simplyblock_core/scripts/clean_local_storage_deploy.sh
+-rw-r--r--  2.0 unx     4409 b- defN 24-May-30 17:11 sbcli_dev-2.8.4/simplyblock_core/scripts/docker-compose-swarm-monitoring.yml
+-rw-r--r--  2.0 unx      930 b- defN 24-May-30 17:11 sbcli_dev-2.8.4/simplyblock_core/scripts/deploy_stack.sh
+-rw-r--r--  2.0 unx       54 b- defN 24-May-30 17:11 sbcli_dev-2.8.4/simplyblock_core/scripts/db_config_single.sh
+-rw-r--r--  2.0 unx      453 b- defN 24-May-30 17:11 sbcli_dev-2.8.4/simplyblock_core/scripts/config_docker.sh
+-rw-r--r--  2.0 unx    25433 b- defN 24-May-30 17:11 sbcli_dev-2.8.4/simplyblock_core/scripts/alerting/alert_rules.yaml
+-rw-r--r--  2.0 unx     1856 b- defN 24-May-30 17:11 sbcli_dev-2.8.4/simplyblock_core/scripts/alerting/alert_resources.yaml
+-rw-r--r--  2.0 unx    93436 b- defN 24-May-30 17:11 sbcli_dev-2.8.4/simplyblock_core/scripts/dashboards/nodes.json
+-rw-r--r--  2.0 unx    89702 b- defN 24-May-30 17:11 sbcli_dev-2.8.4/simplyblock_core/scripts/dashboards/cluster.json
+-rw-r--r--  2.0 unx    93720 b- defN 24-May-30 17:11 sbcli_dev-2.8.4/simplyblock_core/scripts/dashboards/lvols.json
+-rw-r--r--  2.0 unx    93794 b- defN 24-May-30 17:11 sbcli_dev-2.8.4/simplyblock_core/scripts/dashboards/devices.json
+-rw-r--r--  2.0 unx    91642 b- defN 24-May-30 17:11 sbcli_dev-2.8.4/simplyblock_core/scripts/dashboards/pools.json
+-rw-r--r--  2.0 unx   799409 b- defN 24-May-30 17:11 sbcli_dev-2.8.4/simplyblock_core/scripts/dashboards/node-exporter.json
+148 files, 1877377 bytes uncompressed, 187471 bytes compressed:  90.0%
```

## zipnote {}

```diff
@@ -1,445 +1,445 @@
-Filename: sbcli_dev-2.8.3/
+Filename: sbcli_dev-2.8.4/
 Comment: 
 
-Filename: sbcli_dev-2.8.3/simplyblock_cli/
+Filename: sbcli_dev-2.8.4/simplyblock_cli/
 Comment: 
 
-Filename: sbcli_dev-2.8.3/simplyblock_web/
+Filename: sbcli_dev-2.8.4/simplyblock_web/
 Comment: 
 
-Filename: sbcli_dev-2.8.3/sbcli_dev.egg-info/
+Filename: sbcli_dev-2.8.4/sbcli_dev.egg-info/
 Comment: 
 
-Filename: sbcli_dev-2.8.3/simplyblock_core/
+Filename: sbcli_dev-2.8.4/simplyblock_core/
 Comment: 
 
-Filename: sbcli_dev-2.8.3/README.md
+Filename: sbcli_dev-2.8.4/README.md
 Comment: 
 
-Filename: sbcli_dev-2.8.3/pyproject.toml
+Filename: sbcli_dev-2.8.4/pyproject.toml
 Comment: 
 
-Filename: sbcli_dev-2.8.3/PKG-INFO
+Filename: sbcli_dev-2.8.4/PKG-INFO
 Comment: 
 
-Filename: sbcli_dev-2.8.3/env_var
+Filename: sbcli_dev-2.8.4/env_var
 Comment: 
 
-Filename: sbcli_dev-2.8.3/setup.cfg
+Filename: sbcli_dev-2.8.4/setup.cfg
 Comment: 
 
-Filename: sbcli_dev-2.8.3/setup.py
+Filename: sbcli_dev-2.8.4/setup.py
 Comment: 
 
-Filename: sbcli_dev-2.8.3/simplyblock_cli/cli.py
+Filename: sbcli_dev-2.8.4/simplyblock_cli/cli.py
 Comment: 
 
-Filename: sbcli_dev-2.8.3/simplyblock_cli/main.py
+Filename: sbcli_dev-2.8.4/simplyblock_cli/main.py
 Comment: 
 
-Filename: sbcli_dev-2.8.3/simplyblock_web/static/
+Filename: sbcli_dev-2.8.4/simplyblock_web/static/
 Comment: 
 
-Filename: sbcli_dev-2.8.3/simplyblock_web/blueprints/
+Filename: sbcli_dev-2.8.4/simplyblock_web/blueprints/
 Comment: 
 
-Filename: sbcli_dev-2.8.3/simplyblock_web/templates/
+Filename: sbcli_dev-2.8.4/simplyblock_web/templates/
 Comment: 
 
-Filename: sbcli_dev-2.8.3/simplyblock_web/__init__.py
+Filename: sbcli_dev-2.8.4/simplyblock_web/__init__.py
 Comment: 
 
-Filename: sbcli_dev-2.8.3/simplyblock_web/node_webapp.py
+Filename: sbcli_dev-2.8.4/simplyblock_web/node_webapp.py
 Comment: 
 
-Filename: sbcli_dev-2.8.3/simplyblock_web/snode_app.py
+Filename: sbcli_dev-2.8.4/simplyblock_web/snode_app.py
 Comment: 
 
-Filename: sbcli_dev-2.8.3/simplyblock_web/caching_node_app.py
+Filename: sbcli_dev-2.8.4/simplyblock_web/caching_node_app.py
 Comment: 
 
-Filename: sbcli_dev-2.8.3/simplyblock_web/auth_middleware.py
+Filename: sbcli_dev-2.8.4/simplyblock_web/auth_middleware.py
 Comment: 
 
-Filename: sbcli_dev-2.8.3/simplyblock_web/node_utils.py
+Filename: sbcli_dev-2.8.4/simplyblock_web/node_utils.py
 Comment: 
 
-Filename: sbcli_dev-2.8.3/simplyblock_web/utils.py
+Filename: sbcli_dev-2.8.4/simplyblock_web/utils.py
 Comment: 
 
-Filename: sbcli_dev-2.8.3/simplyblock_web/app.py
+Filename: sbcli_dev-2.8.4/simplyblock_web/app.py
 Comment: 
 
-Filename: sbcli_dev-2.8.3/simplyblock_web/caching_node_app_k8s.py
+Filename: sbcli_dev-2.8.4/simplyblock_web/caching_node_app_k8s.py
 Comment: 
 
-Filename: sbcli_dev-2.8.3/simplyblock_web/static/tst.py
+Filename: sbcli_dev-2.8.4/simplyblock_web/static/tst.py
 Comment: 
 
-Filename: sbcli_dev-2.8.3/simplyblock_web/static/delete.py
+Filename: sbcli_dev-2.8.4/simplyblock_web/static/delete.py
 Comment: 
 
-Filename: sbcli_dev-2.8.3/simplyblock_web/static/deploy_cnode.yaml
+Filename: sbcli_dev-2.8.4/simplyblock_web/static/deploy_cnode.yaml
 Comment: 
 
-Filename: sbcli_dev-2.8.3/simplyblock_web/static/is_up.py
+Filename: sbcli_dev-2.8.4/simplyblock_web/static/is_up.py
 Comment: 
 
-Filename: sbcli_dev-2.8.3/simplyblock_web/static/deploy_spdk.yaml
+Filename: sbcli_dev-2.8.4/simplyblock_web/static/deploy_spdk.yaml
 Comment: 
 
-Filename: sbcli_dev-2.8.3/simplyblock_web/static/rpac.yaml
+Filename: sbcli_dev-2.8.4/simplyblock_web/static/rpac.yaml
 Comment: 
 
-Filename: sbcli_dev-2.8.3/simplyblock_web/static/list_deps.py
+Filename: sbcli_dev-2.8.4/simplyblock_web/static/list_deps.py
 Comment: 
 
-Filename: sbcli_dev-2.8.3/simplyblock_web/static/deploy.py
+Filename: sbcli_dev-2.8.4/simplyblock_web/static/deploy.py
 Comment: 
 
-Filename: sbcli_dev-2.8.3/simplyblock_web/blueprints/web_api_pool.py
+Filename: sbcli_dev-2.8.4/simplyblock_web/blueprints/web_api_pool.py
 Comment: 
 
-Filename: sbcli_dev-2.8.3/simplyblock_web/blueprints/__init__.py
+Filename: sbcli_dev-2.8.4/simplyblock_web/blueprints/__init__.py
 Comment: 
 
-Filename: sbcli_dev-2.8.3/simplyblock_web/blueprints/web_api_device.py
+Filename: sbcli_dev-2.8.4/simplyblock_web/blueprints/web_api_device.py
 Comment: 
 
-Filename: sbcli_dev-2.8.3/simplyblock_web/blueprints/web_api_lvol.py
+Filename: sbcli_dev-2.8.4/simplyblock_web/blueprints/web_api_lvol.py
 Comment: 
 
-Filename: sbcli_dev-2.8.3/simplyblock_web/blueprints/snode_ops.py
+Filename: sbcli_dev-2.8.4/simplyblock_web/blueprints/snode_ops.py
 Comment: 
 
-Filename: sbcli_dev-2.8.3/simplyblock_web/blueprints/caching_node_ops.py
+Filename: sbcli_dev-2.8.4/simplyblock_web/blueprints/caching_node_ops.py
 Comment: 
 
-Filename: sbcli_dev-2.8.3/simplyblock_web/blueprints/web_api_storage_node.py
+Filename: sbcli_dev-2.8.4/simplyblock_web/blueprints/web_api_storage_node.py
 Comment: 
 
-Filename: sbcli_dev-2.8.3/simplyblock_web/blueprints/web_api_cluster.py
+Filename: sbcli_dev-2.8.4/simplyblock_web/blueprints/web_api_cluster.py
 Comment: 
 
-Filename: sbcli_dev-2.8.3/simplyblock_web/blueprints/caching_node_ops_k8s.py
+Filename: sbcli_dev-2.8.4/simplyblock_web/blueprints/caching_node_ops_k8s.py
 Comment: 
 
-Filename: sbcli_dev-2.8.3/simplyblock_web/blueprints/node_api_caching_ks.py
+Filename: sbcli_dev-2.8.4/simplyblock_web/blueprints/node_api_caching_ks.py
 Comment: 
 
-Filename: sbcli_dev-2.8.3/simplyblock_web/blueprints/node_api_caching_docker.py
+Filename: sbcli_dev-2.8.4/simplyblock_web/blueprints/node_api_caching_docker.py
 Comment: 
 
-Filename: sbcli_dev-2.8.3/simplyblock_web/blueprints/web_api_caching_node.py
+Filename: sbcli_dev-2.8.4/simplyblock_web/blueprints/web_api_caching_node.py
 Comment: 
 
-Filename: sbcli_dev-2.8.3/simplyblock_web/blueprints/node_api_basic.py
+Filename: sbcli_dev-2.8.4/simplyblock_web/blueprints/node_api_basic.py
 Comment: 
 
-Filename: sbcli_dev-2.8.3/simplyblock_web/blueprints/csi.py
+Filename: sbcli_dev-2.8.4/simplyblock_web/blueprints/csi.py
 Comment: 
 
-Filename: sbcli_dev-2.8.3/simplyblock_web/blueprints/web_api_mgmt_node.py
+Filename: sbcli_dev-2.8.4/simplyblock_web/blueprints/web_api_mgmt_node.py
 Comment: 
 
-Filename: sbcli_dev-2.8.3/simplyblock_web/templates/deploy_spdk.yaml.j2
+Filename: sbcli_dev-2.8.4/simplyblock_web/templates/deploy_spdk.yaml.j2
 Comment: 
 
-Filename: sbcli_dev-2.8.3/sbcli_dev.egg-info/SOURCES.txt
+Filename: sbcli_dev-2.8.4/sbcli_dev.egg-info/SOURCES.txt
 Comment: 
 
-Filename: sbcli_dev-2.8.3/sbcli_dev.egg-info/requires.txt
+Filename: sbcli_dev-2.8.4/sbcli_dev.egg-info/requires.txt
 Comment: 
 
-Filename: sbcli_dev-2.8.3/sbcli_dev.egg-info/PKG-INFO
+Filename: sbcli_dev-2.8.4/sbcli_dev.egg-info/PKG-INFO
 Comment: 
 
-Filename: sbcli_dev-2.8.3/sbcli_dev.egg-info/top_level.txt
+Filename: sbcli_dev-2.8.4/sbcli_dev.egg-info/top_level.txt
 Comment: 
 
-Filename: sbcli_dev-2.8.3/sbcli_dev.egg-info/entry_points.txt
+Filename: sbcli_dev-2.8.4/sbcli_dev.egg-info/entry_points.txt
 Comment: 
 
-Filename: sbcli_dev-2.8.3/sbcli_dev.egg-info/dependency_links.txt
+Filename: sbcli_dev-2.8.4/sbcli_dev.egg-info/dependency_links.txt
 Comment: 
 
-Filename: sbcli_dev-2.8.3/simplyblock_core/services/
+Filename: sbcli_dev-2.8.4/simplyblock_core/services/
 Comment: 
 
-Filename: sbcli_dev-2.8.3/simplyblock_core/controllers/
+Filename: sbcli_dev-2.8.4/simplyblock_core/controllers/
 Comment: 
 
-Filename: sbcli_dev-2.8.3/simplyblock_core/models/
+Filename: sbcli_dev-2.8.4/simplyblock_core/models/
 Comment: 
 
-Filename: sbcli_dev-2.8.3/simplyblock_core/scripts/
+Filename: sbcli_dev-2.8.4/simplyblock_core/scripts/
 Comment: 
 
-Filename: sbcli_dev-2.8.3/simplyblock_core/cluster_ops.py
+Filename: sbcli_dev-2.8.4/simplyblock_core/cluster_ops.py
 Comment: 
 
-Filename: sbcli_dev-2.8.3/simplyblock_core/pci_utils.py
+Filename: sbcli_dev-2.8.4/simplyblock_core/pci_utils.py
 Comment: 
 
-Filename: sbcli_dev-2.8.3/simplyblock_core/__init__.py
+Filename: sbcli_dev-2.8.4/simplyblock_core/__init__.py
 Comment: 
 
-Filename: sbcli_dev-2.8.3/simplyblock_core/snode_client.py
+Filename: sbcli_dev-2.8.4/simplyblock_core/snode_client.py
 Comment: 
 
-Filename: sbcli_dev-2.8.3/simplyblock_core/kv_store.py
+Filename: sbcli_dev-2.8.4/simplyblock_core/kv_store.py
 Comment: 
 
-Filename: sbcli_dev-2.8.3/simplyblock_core/compute_node_ops.py
+Filename: sbcli_dev-2.8.4/simplyblock_core/compute_node_ops.py
 Comment: 
 
-Filename: sbcli_dev-2.8.3/simplyblock_core/rpc_client.py
+Filename: sbcli_dev-2.8.4/simplyblock_core/rpc_client.py
 Comment: 
 
-Filename: sbcli_dev-2.8.3/simplyblock_core/mgmt_node_ops.py
+Filename: sbcli_dev-2.8.4/simplyblock_core/mgmt_node_ops.py
 Comment: 
 
-Filename: sbcli_dev-2.8.3/simplyblock_core/utils.py
+Filename: sbcli_dev-2.8.4/simplyblock_core/utils.py
 Comment: 
 
-Filename: sbcli_dev-2.8.3/simplyblock_core/distr_controller.py
+Filename: sbcli_dev-2.8.4/simplyblock_core/distr_controller.py
 Comment: 
 
-Filename: sbcli_dev-2.8.3/simplyblock_core/shell_utils.py
+Filename: sbcli_dev-2.8.4/simplyblock_core/shell_utils.py
 Comment: 
 
-Filename: sbcli_dev-2.8.3/simplyblock_core/cnode_client.py
+Filename: sbcli_dev-2.8.4/simplyblock_core/cnode_client.py
 Comment: 
 
-Filename: sbcli_dev-2.8.3/simplyblock_core/storage_node_ops.py
+Filename: sbcli_dev-2.8.4/simplyblock_core/storage_node_ops.py
 Comment: 
 
-Filename: sbcli_dev-2.8.3/simplyblock_core/constants.py
+Filename: sbcli_dev-2.8.4/simplyblock_core/constants.py
 Comment: 
 
-Filename: sbcli_dev-2.8.3/simplyblock_core/services/job_tasks.py
+Filename: sbcli_dev-2.8.4/simplyblock_core/services/job_tasks.py
 Comment: 
 
-Filename: sbcli_dev-2.8.3/simplyblock_core/services/caching_node_monitor.py
+Filename: sbcli_dev-2.8.4/simplyblock_core/services/caching_node_monitor.py
 Comment: 
 
-Filename: sbcli_dev-2.8.3/simplyblock_core/services/service_template.service
+Filename: sbcli_dev-2.8.4/simplyblock_core/services/service_template.service
 Comment: 
 
-Filename: sbcli_dev-2.8.3/simplyblock_core/services/install_service.sh
+Filename: sbcli_dev-2.8.4/simplyblock_core/services/install_service.sh
 Comment: 
 
-Filename: sbcli_dev-2.8.3/simplyblock_core/services/__init__.py
+Filename: sbcli_dev-2.8.4/simplyblock_core/services/__init__.py
 Comment: 
 
-Filename: sbcli_dev-2.8.3/simplyblock_core/services/log_agg_service.py
+Filename: sbcli_dev-2.8.4/simplyblock_core/services/log_agg_service.py
 Comment: 
 
-Filename: sbcli_dev-2.8.3/simplyblock_core/services/health_check_service.py
+Filename: sbcli_dev-2.8.4/simplyblock_core/services/health_check_service.py
 Comment: 
 
-Filename: sbcli_dev-2.8.3/simplyblock_core/services/capacity_and_stats_collector.py
+Filename: sbcli_dev-2.8.4/simplyblock_core/services/capacity_and_stats_collector.py
 Comment: 
 
-Filename: sbcli_dev-2.8.3/simplyblock_core/services/device_monitor.py
+Filename: sbcli_dev-2.8.4/simplyblock_core/services/device_monitor.py
 Comment: 
 
-Filename: sbcli_dev-2.8.3/simplyblock_core/services/lvol_stat_collector.py
+Filename: sbcli_dev-2.8.4/simplyblock_core/services/lvol_stat_collector.py
 Comment: 
 
-Filename: sbcli_dev-2.8.3/simplyblock_core/services/cap_monitor.py
+Filename: sbcli_dev-2.8.4/simplyblock_core/services/cap_monitor.py
 Comment: 
 
-Filename: sbcli_dev-2.8.3/simplyblock_core/services/storage_node_monitor.py
+Filename: sbcli_dev-2.8.4/simplyblock_core/services/storage_node_monitor.py
 Comment: 
 
-Filename: sbcli_dev-2.8.3/simplyblock_core/services/port_stat_collector.py
+Filename: sbcli_dev-2.8.4/simplyblock_core/services/port_stat_collector.py
 Comment: 
 
-Filename: sbcli_dev-2.8.3/simplyblock_core/services/distr_event_collector.py
+Filename: sbcli_dev-2.8.4/simplyblock_core/services/distr_event_collector.py
 Comment: 
 
-Filename: sbcli_dev-2.8.3/simplyblock_core/services/remove_service.sh
+Filename: sbcli_dev-2.8.4/simplyblock_core/services/remove_service.sh
 Comment: 
 
-Filename: sbcli_dev-2.8.3/simplyblock_core/services/mgmt_node_monitor.py
+Filename: sbcli_dev-2.8.4/simplyblock_core/services/mgmt_node_monitor.py
 Comment: 
 
-Filename: sbcli_dev-2.8.3/simplyblock_core/services/lvol_monitor.py
+Filename: sbcli_dev-2.8.4/simplyblock_core/services/lvol_monitor.py
 Comment: 
 
-Filename: sbcli_dev-2.8.3/simplyblock_core/controllers/pool_controller.py
+Filename: sbcli_dev-2.8.4/simplyblock_core/controllers/pool_controller.py
 Comment: 
 
-Filename: sbcli_dev-2.8.3/simplyblock_core/controllers/__init__.py
+Filename: sbcli_dev-2.8.4/simplyblock_core/controllers/__init__.py
 Comment: 
 
-Filename: sbcli_dev-2.8.3/simplyblock_core/controllers/storage_events.py
+Filename: sbcli_dev-2.8.4/simplyblock_core/controllers/storage_events.py
 Comment: 
 
-Filename: sbcli_dev-2.8.3/simplyblock_core/controllers/lvol_controller.py
+Filename: sbcli_dev-2.8.4/simplyblock_core/controllers/lvol_controller.py
 Comment: 
 
-Filename: sbcli_dev-2.8.3/simplyblock_core/controllers/device_events.py
+Filename: sbcli_dev-2.8.4/simplyblock_core/controllers/device_events.py
 Comment: 
 
-Filename: sbcli_dev-2.8.3/simplyblock_core/controllers/lvol_events.py
+Filename: sbcli_dev-2.8.4/simplyblock_core/controllers/lvol_events.py
 Comment: 
 
-Filename: sbcli_dev-2.8.3/simplyblock_core/controllers/snapshot_controller.py
+Filename: sbcli_dev-2.8.4/simplyblock_core/controllers/snapshot_controller.py
 Comment: 
 
-Filename: sbcli_dev-2.8.3/simplyblock_core/controllers/snapshot_events.py
+Filename: sbcli_dev-2.8.4/simplyblock_core/controllers/snapshot_events.py
 Comment: 
 
-Filename: sbcli_dev-2.8.3/simplyblock_core/controllers/events_controller.py
+Filename: sbcli_dev-2.8.4/simplyblock_core/controllers/events_controller.py
 Comment: 
 
-Filename: sbcli_dev-2.8.3/simplyblock_core/controllers/health_controller.py
+Filename: sbcli_dev-2.8.4/simplyblock_core/controllers/health_controller.py
 Comment: 
 
-Filename: sbcli_dev-2.8.3/simplyblock_core/controllers/device_controller.py
+Filename: sbcli_dev-2.8.4/simplyblock_core/controllers/device_controller.py
 Comment: 
 
-Filename: sbcli_dev-2.8.3/simplyblock_core/controllers/pool_events.py
+Filename: sbcli_dev-2.8.4/simplyblock_core/controllers/pool_events.py
 Comment: 
 
-Filename: sbcli_dev-2.8.3/simplyblock_core/controllers/caching_node_controller.py
+Filename: sbcli_dev-2.8.4/simplyblock_core/controllers/caching_node_controller.py
 Comment: 
 
-Filename: sbcli_dev-2.8.3/simplyblock_core/controllers/cluster_events.py
+Filename: sbcli_dev-2.8.4/simplyblock_core/controllers/cluster_events.py
 Comment: 
 
-Filename: sbcli_dev-2.8.3/simplyblock_core/controllers/mgmt_events.py
+Filename: sbcli_dev-2.8.4/simplyblock_core/controllers/mgmt_events.py
 Comment: 
 
-Filename: sbcli_dev-2.8.3/simplyblock_core/models/caching_node.py
+Filename: sbcli_dev-2.8.4/simplyblock_core/models/caching_node.py
 Comment: 
 
-Filename: sbcli_dev-2.8.3/simplyblock_core/models/nvme_device.py
+Filename: sbcli_dev-2.8.4/simplyblock_core/models/nvme_device.py
 Comment: 
 
-Filename: sbcli_dev-2.8.3/simplyblock_core/models/mgmt_node.py
+Filename: sbcli_dev-2.8.4/simplyblock_core/models/mgmt_node.py
 Comment: 
 
-Filename: sbcli_dev-2.8.3/simplyblock_core/models/compute_node.py
+Filename: sbcli_dev-2.8.4/simplyblock_core/models/compute_node.py
 Comment: 
 
-Filename: sbcli_dev-2.8.3/simplyblock_core/models/__init__.py
+Filename: sbcli_dev-2.8.4/simplyblock_core/models/__init__.py
 Comment: 
 
-Filename: sbcli_dev-2.8.3/simplyblock_core/models/events.py
+Filename: sbcli_dev-2.8.4/simplyblock_core/models/events.py
 Comment: 
 
-Filename: sbcli_dev-2.8.3/simplyblock_core/models/global_settings.py
+Filename: sbcli_dev-2.8.4/simplyblock_core/models/global_settings.py
 Comment: 
 
-Filename: sbcli_dev-2.8.3/simplyblock_core/models/job_schedule.py
+Filename: sbcli_dev-2.8.4/simplyblock_core/models/job_schedule.py
 Comment: 
 
-Filename: sbcli_dev-2.8.3/simplyblock_core/models/base_model.py
+Filename: sbcli_dev-2.8.4/simplyblock_core/models/base_model.py
 Comment: 
 
-Filename: sbcli_dev-2.8.3/simplyblock_core/models/lvol_model.py
+Filename: sbcli_dev-2.8.4/simplyblock_core/models/lvol_model.py
 Comment: 
 
-Filename: sbcli_dev-2.8.3/simplyblock_core/models/snapshot.py
+Filename: sbcli_dev-2.8.4/simplyblock_core/models/snapshot.py
 Comment: 
 
-Filename: sbcli_dev-2.8.3/simplyblock_core/models/storage_node.py
+Filename: sbcli_dev-2.8.4/simplyblock_core/models/storage_node.py
 Comment: 
 
-Filename: sbcli_dev-2.8.3/simplyblock_core/models/stats.py
+Filename: sbcli_dev-2.8.4/simplyblock_core/models/stats.py
 Comment: 
 
-Filename: sbcli_dev-2.8.3/simplyblock_core/models/pool.py
+Filename: sbcli_dev-2.8.4/simplyblock_core/models/pool.py
 Comment: 
 
-Filename: sbcli_dev-2.8.3/simplyblock_core/models/iface.py
+Filename: sbcli_dev-2.8.4/simplyblock_core/models/iface.py
 Comment: 
 
-Filename: sbcli_dev-2.8.3/simplyblock_core/models/cluster.py
+Filename: sbcli_dev-2.8.4/simplyblock_core/models/cluster.py
 Comment: 
 
-Filename: sbcli_dev-2.8.3/simplyblock_core/models/port_stat.py
+Filename: sbcli_dev-2.8.4/simplyblock_core/models/port_stat.py
 Comment: 
 
-Filename: sbcli_dev-2.8.3/simplyblock_core/scripts/alerting/
+Filename: sbcli_dev-2.8.4/simplyblock_core/scripts/alerting/
 Comment: 
 
-Filename: sbcli_dev-2.8.3/simplyblock_core/scripts/dashboards/
+Filename: sbcli_dev-2.8.4/simplyblock_core/scripts/dashboards/
 Comment: 
 
-Filename: sbcli_dev-2.8.3/simplyblock_core/scripts/install_deps.sh
+Filename: sbcli_dev-2.8.4/simplyblock_core/scripts/install_deps.sh
 Comment: 
 
-Filename: sbcli_dev-2.8.3/simplyblock_core/scripts/__init__.py
+Filename: sbcli_dev-2.8.4/simplyblock_core/scripts/__init__.py
 Comment: 
 
-Filename: sbcli_dev-2.8.3/simplyblock_core/scripts/run_ssh.sh
+Filename: sbcli_dev-2.8.4/simplyblock_core/scripts/run_ssh.sh
 Comment: 
 
-Filename: sbcli_dev-2.8.3/simplyblock_core/scripts/haproxy.cfg
+Filename: sbcli_dev-2.8.4/simplyblock_core/scripts/haproxy.cfg
 Comment: 
 
-Filename: sbcli_dev-2.8.3/simplyblock_core/scripts/db_config_double.sh
+Filename: sbcli_dev-2.8.4/simplyblock_core/scripts/db_config_double.sh
 Comment: 
 
-Filename: sbcli_dev-2.8.3/simplyblock_core/scripts/stack_deploy_wait.sh
+Filename: sbcli_dev-2.8.4/simplyblock_core/scripts/stack_deploy_wait.sh
 Comment: 
 
-Filename: sbcli_dev-2.8.3/simplyblock_core/scripts/datasource.yml
+Filename: sbcli_dev-2.8.4/simplyblock_core/scripts/datasource.yml
 Comment: 
 
-Filename: sbcli_dev-2.8.3/simplyblock_core/scripts/docker-compose-swarm.yml
+Filename: sbcli_dev-2.8.4/simplyblock_core/scripts/docker-compose-swarm.yml
 Comment: 
 
-Filename: sbcli_dev-2.8.3/simplyblock_core/scripts/set_db_config.sh
+Filename: sbcli_dev-2.8.4/simplyblock_core/scripts/set_db_config.sh
 Comment: 
 
-Filename: sbcli_dev-2.8.3/simplyblock_core/scripts/apply_dashboard.sh
+Filename: sbcli_dev-2.8.4/simplyblock_core/scripts/apply_dashboard.sh
 Comment: 
 
-Filename: sbcli_dev-2.8.3/simplyblock_core/scripts/prometheus.yml
+Filename: sbcli_dev-2.8.4/simplyblock_core/scripts/prometheus.yml
 Comment: 
 
-Filename: sbcli_dev-2.8.3/simplyblock_core/scripts/clean_local_storage_deploy.sh
+Filename: sbcli_dev-2.8.4/simplyblock_core/scripts/clean_local_storage_deploy.sh
 Comment: 
 
-Filename: sbcli_dev-2.8.3/simplyblock_core/scripts/docker-compose-swarm-monitoring.yml
+Filename: sbcli_dev-2.8.4/simplyblock_core/scripts/docker-compose-swarm-monitoring.yml
 Comment: 
 
-Filename: sbcli_dev-2.8.3/simplyblock_core/scripts/deploy_stack.sh
+Filename: sbcli_dev-2.8.4/simplyblock_core/scripts/deploy_stack.sh
 Comment: 
 
-Filename: sbcli_dev-2.8.3/simplyblock_core/scripts/db_config_single.sh
+Filename: sbcli_dev-2.8.4/simplyblock_core/scripts/db_config_single.sh
 Comment: 
 
-Filename: sbcli_dev-2.8.3/simplyblock_core/scripts/config_docker.sh
+Filename: sbcli_dev-2.8.4/simplyblock_core/scripts/config_docker.sh
 Comment: 
 
-Filename: sbcli_dev-2.8.3/simplyblock_core/scripts/alerting/alert_rules.yaml
+Filename: sbcli_dev-2.8.4/simplyblock_core/scripts/alerting/alert_rules.yaml
 Comment: 
 
-Filename: sbcli_dev-2.8.3/simplyblock_core/scripts/alerting/alert_resources.yaml
+Filename: sbcli_dev-2.8.4/simplyblock_core/scripts/alerting/alert_resources.yaml
 Comment: 
 
-Filename: sbcli_dev-2.8.3/simplyblock_core/scripts/dashboards/nodes.json
+Filename: sbcli_dev-2.8.4/simplyblock_core/scripts/dashboards/nodes.json
 Comment: 
 
-Filename: sbcli_dev-2.8.3/simplyblock_core/scripts/dashboards/cluster.json
+Filename: sbcli_dev-2.8.4/simplyblock_core/scripts/dashboards/cluster.json
 Comment: 
 
-Filename: sbcli_dev-2.8.3/simplyblock_core/scripts/dashboards/lvols.json
+Filename: sbcli_dev-2.8.4/simplyblock_core/scripts/dashboards/lvols.json
 Comment: 
 
-Filename: sbcli_dev-2.8.3/simplyblock_core/scripts/dashboards/devices.json
+Filename: sbcli_dev-2.8.4/simplyblock_core/scripts/dashboards/devices.json
 Comment: 
 
-Filename: sbcli_dev-2.8.3/simplyblock_core/scripts/dashboards/pools.json
+Filename: sbcli_dev-2.8.4/simplyblock_core/scripts/dashboards/pools.json
 Comment: 
 
-Filename: sbcli_dev-2.8.3/simplyblock_core/scripts/dashboards/node-exporter.json
+Filename: sbcli_dev-2.8.4/simplyblock_core/scripts/dashboards/node-exporter.json
 Comment: 
 
 Zip file comment:
```

## Comparing `sbcli_dev-2.8.3/README.md` & `sbcli_dev-2.8.4/README.md`

 * *Files identical despite different names*

## Comparing `sbcli_dev-2.8.3/PKG-INFO` & `sbcli_dev-2.8.4/PKG-INFO`

 * *Files 4% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: sbcli-dev
-Version: 2.8.3
+Version: 2.8.4
 Summary: CLI for managing SimplyBlock cluster
 Home-page: https://www.simplyblock.io/
 Author: Hamdy
 Author-email: hamdy@simplyblock.io
 Description-Content-Type: text/markdown
 Requires-Dist: foundationdb
 Requires-Dist: requests
```

## Comparing `sbcli_dev-2.8.3/setup.py` & `sbcli_dev-2.8.4/setup.py`

 * *Files identical despite different names*

## Comparing `sbcli_dev-2.8.3/simplyblock_cli/cli.py` & `sbcli_dev-2.8.4/simplyblock_cli/cli.py`

 * *Files identical despite different names*

## Comparing `sbcli_dev-2.8.3/simplyblock_web/node_webapp.py` & `sbcli_dev-2.8.4/simplyblock_web/node_webapp.py`

 * *Files identical despite different names*

## Comparing `sbcli_dev-2.8.3/simplyblock_web/snode_app.py` & `sbcli_dev-2.8.4/simplyblock_web/snode_app.py`

 * *Files identical despite different names*

## Comparing `sbcli_dev-2.8.3/simplyblock_web/caching_node_app.py` & `sbcli_dev-2.8.4/simplyblock_web/caching_node_app.py`

 * *Files identical despite different names*

## Comparing `sbcli_dev-2.8.3/simplyblock_web/auth_middleware.py` & `sbcli_dev-2.8.4/simplyblock_web/auth_middleware.py`

 * *Files identical despite different names*

## Comparing `sbcli_dev-2.8.3/simplyblock_web/node_utils.py` & `sbcli_dev-2.8.4/simplyblock_web/node_utils.py`

 * *Files identical despite different names*

## Comparing `sbcli_dev-2.8.3/simplyblock_web/utils.py` & `sbcli_dev-2.8.4/simplyblock_web/utils.py`

 * *Files identical despite different names*

## Comparing `sbcli_dev-2.8.3/simplyblock_web/app.py` & `sbcli_dev-2.8.4/simplyblock_web/app.py`

 * *Files identical despite different names*

## Comparing `sbcli_dev-2.8.3/simplyblock_web/caching_node_app_k8s.py` & `sbcli_dev-2.8.4/simplyblock_web/caching_node_app_k8s.py`

 * *Files identical despite different names*

## Comparing `sbcli_dev-2.8.3/simplyblock_web/static/delete.py` & `sbcli_dev-2.8.4/simplyblock_web/static/delete.py`

 * *Files identical despite different names*

## Comparing `sbcli_dev-2.8.3/simplyblock_web/static/deploy_spdk.yaml` & `sbcli_dev-2.8.4/simplyblock_web/static/deploy_spdk.yaml`

 * *Files identical despite different names*

## Comparing `sbcli_dev-2.8.3/simplyblock_web/static/deploy.py` & `sbcli_dev-2.8.4/simplyblock_web/static/deploy.py`

 * *Files identical despite different names*

## Comparing `sbcli_dev-2.8.3/simplyblock_web/blueprints/web_api_pool.py` & `sbcli_dev-2.8.4/simplyblock_web/blueprints/web_api_pool.py`

 * *Files identical despite different names*

## Comparing `sbcli_dev-2.8.3/simplyblock_web/blueprints/web_api_device.py` & `sbcli_dev-2.8.4/simplyblock_web/blueprints/web_api_device.py`

 * *Files identical despite different names*

## Comparing `sbcli_dev-2.8.3/simplyblock_web/blueprints/web_api_lvol.py` & `sbcli_dev-2.8.4/simplyblock_web/blueprints/web_api_lvol.py`

 * *Files identical despite different names*

## Comparing `sbcli_dev-2.8.3/simplyblock_web/blueprints/snode_ops.py` & `sbcli_dev-2.8.4/simplyblock_web/blueprints/snode_ops.py`

 * *Files identical despite different names*

## Comparing `sbcli_dev-2.8.3/simplyblock_web/blueprints/caching_node_ops.py` & `sbcli_dev-2.8.4/simplyblock_web/blueprints/caching_node_ops.py`

 * *Files identical despite different names*

## Comparing `sbcli_dev-2.8.3/simplyblock_web/blueprints/web_api_storage_node.py` & `sbcli_dev-2.8.4/simplyblock_web/blueprints/web_api_storage_node.py`

 * *Files identical despite different names*

## Comparing `sbcli_dev-2.8.3/simplyblock_web/blueprints/web_api_cluster.py` & `sbcli_dev-2.8.4/simplyblock_web/blueprints/web_api_cluster.py`

 * *Files identical despite different names*

## Comparing `sbcli_dev-2.8.3/simplyblock_web/blueprints/caching_node_ops_k8s.py` & `sbcli_dev-2.8.4/simplyblock_web/blueprints/caching_node_ops_k8s.py`

 * *Files identical despite different names*

## Comparing `sbcli_dev-2.8.3/simplyblock_web/blueprints/node_api_caching_ks.py` & `sbcli_dev-2.8.4/simplyblock_web/blueprints/node_api_caching_ks.py`

 * *Files identical despite different names*

## Comparing `sbcli_dev-2.8.3/simplyblock_web/blueprints/node_api_caching_docker.py` & `sbcli_dev-2.8.4/simplyblock_web/blueprints/node_api_caching_docker.py`

 * *Files identical despite different names*

## Comparing `sbcli_dev-2.8.3/simplyblock_web/blueprints/web_api_caching_node.py` & `sbcli_dev-2.8.4/simplyblock_web/blueprints/web_api_caching_node.py`

 * *Files identical despite different names*

## Comparing `sbcli_dev-2.8.3/simplyblock_web/blueprints/node_api_basic.py` & `sbcli_dev-2.8.4/simplyblock_web/blueprints/node_api_basic.py`

 * *Files identical despite different names*

## Comparing `sbcli_dev-2.8.3/simplyblock_web/blueprints/csi.py` & `sbcli_dev-2.8.4/simplyblock_web/blueprints/csi.py`

 * *Files identical despite different names*

## Comparing `sbcli_dev-2.8.3/simplyblock_web/blueprints/web_api_mgmt_node.py` & `sbcli_dev-2.8.4/simplyblock_web/blueprints/web_api_mgmt_node.py`

 * *Files identical despite different names*

## Comparing `sbcli_dev-2.8.3/simplyblock_web/templates/deploy_spdk.yaml.j2` & `sbcli_dev-2.8.4/simplyblock_web/templates/deploy_spdk.yaml.j2`

 * *Files identical despite different names*

## Comparing `sbcli_dev-2.8.3/sbcli_dev.egg-info/SOURCES.txt` & `sbcli_dev-2.8.4/sbcli_dev.egg-info/SOURCES.txt`

 * *Files identical despite different names*

## Comparing `sbcli_dev-2.8.3/sbcli_dev.egg-info/PKG-INFO` & `sbcli_dev-2.8.4/sbcli_dev.egg-info/PKG-INFO`

 * *Files 4% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: sbcli-dev
-Version: 2.8.3
+Version: 2.8.4
 Summary: CLI for managing SimplyBlock cluster
 Home-page: https://www.simplyblock.io/
 Author: Hamdy
 Author-email: hamdy@simplyblock.io
 Description-Content-Type: text/markdown
 Requires-Dist: foundationdb
 Requires-Dist: requests
```

## Comparing `sbcli_dev-2.8.3/simplyblock_core/cluster_ops.py` & `sbcli_dev-2.8.4/simplyblock_core/cluster_ops.py`

 * *Files 0% similar despite different names*

```diff
@@ -701,15 +701,15 @@
     data = []
     tasks = db_controller.get_job_tasks(cluster_id)
     for task in tasks:
         data.append({
             "UUID": task.uuid,
             "Device": task.device_id,
             "Function": task.function_name,
-            "Retry": task.retry,
+            "Retry": f"{task.retry}/{constants.TASK_EXEC_RETRY_COUNT}",
             "Status": task.status,
             "Result": task.function_result,
             "Date": time.strftime("%Y-%m-%d %H:%M:%S", time.gmtime(task.date)),
         })
     return utils.print_table(data)
```

## Comparing `sbcli_dev-2.8.3/simplyblock_core/pci_utils.py` & `sbcli_dev-2.8.4/simplyblock_core/pci_utils.py`

 * *Files identical despite different names*

## Comparing `sbcli_dev-2.8.3/simplyblock_core/snode_client.py` & `sbcli_dev-2.8.4/simplyblock_core/snode_client.py`

 * *Files identical despite different names*

## Comparing `sbcli_dev-2.8.3/simplyblock_core/kv_store.py` & `sbcli_dev-2.8.4/simplyblock_core/kv_store.py`

 * *Files identical despite different names*

## Comparing `sbcli_dev-2.8.3/simplyblock_core/compute_node_ops.py` & `sbcli_dev-2.8.4/simplyblock_core/compute_node_ops.py`

 * *Files identical despite different names*

## Comparing `sbcli_dev-2.8.3/simplyblock_core/rpc_client.py` & `sbcli_dev-2.8.4/simplyblock_core/rpc_client.py`

 * *Files identical despite different names*

## Comparing `sbcli_dev-2.8.3/simplyblock_core/mgmt_node_ops.py` & `sbcli_dev-2.8.4/simplyblock_core/mgmt_node_ops.py`

 * *Files identical despite different names*

## Comparing `sbcli_dev-2.8.3/simplyblock_core/utils.py` & `sbcli_dev-2.8.4/simplyblock_core/utils.py`

 * *Files identical despite different names*

## Comparing `sbcli_dev-2.8.3/simplyblock_core/distr_controller.py` & `sbcli_dev-2.8.4/simplyblock_core/distr_controller.py`

 * *Files identical despite different names*

## Comparing `sbcli_dev-2.8.3/simplyblock_core/cnode_client.py` & `sbcli_dev-2.8.4/simplyblock_core/cnode_client.py`

 * *Files identical despite different names*

## Comparing `sbcli_dev-2.8.3/simplyblock_core/storage_node_ops.py` & `sbcli_dev-2.8.4/simplyblock_core/storage_node_ops.py`

 * *Files identical despite different names*

## Comparing `sbcli_dev-2.8.3/simplyblock_core/constants.py` & `sbcli_dev-2.8.4/simplyblock_core/constants.py`

 * *Files 2% similar despite different names*

```diff
@@ -51,13 +51,14 @@
 
 GRAYLOG_CHECK_INTERVAL_SEC = 60
 
 FDB_CHECK_INTERVAL_SEC = 60
 
 SIMPLY_BLOCK_CLI_NAME = "sbcli-dev"
 TASK_EXEC_INTERVAL_SEC = 30
+TASK_EXEC_RETRY_COUNT = 5
 
 SIMPLY_BLOCK_DOCKER_IMAGE = "simplyblock/simplyblock:dev"
 SIMPLY_BLOCK_SPDK_CORE_IMAGE = "simplyblock/spdk-core:latest"
 SIMPLY_BLOCK_SPDK_ULTRA_IMAGE = "simplyblock/spdk:main-latest"
 
 GELF_PORT = 12201
```

## Comparing `sbcli_dev-2.8.3/simplyblock_core/services/job_tasks.py` & `sbcli_dev-2.8.4/simplyblock_core/services/job_tasks.py`

 * *Files 20% similar despite different names*

```diff
@@ -21,65 +21,65 @@
         if dev.get_id() == task.device_id:
             return dev
 
 
 def task_runner(task):
     device = _get_device(task)
 
-    if task.retry <= 0:
-        task.function_result = "timeout"
+    if task.retry >= constants.TASK_EXEC_RETRY_COUNT:
+        task.function_result = "max retry reached"
         task.status = JobSchedule.STATUS_DONE
         task.write_to_db(db_controller.kv_store)
         device_controller.device_set_unavailable(device.get_id())
-        return
+        return True
 
     node = db_controller.get_storage_node_by_id(task.node_id)
     if node.status != StorageNode.STATUS_ONLINE:
         logger.error(f"Node is not online: {node.get_id()} , skipping task: {task.get_id()}")
         task.function_result = "Node is offline"
-        task.retry -= 1
+        task.retry += 1
         task.write_to_db(db_controller.kv_store)
-        return
+        return False
 
     if device.status == NVMeDevice.STATUS_ONLINE and device.io_error is False:
         logger.info(f"Device is online: {device.get_id()}, no restart needed")
         task.function_result = "skipped because dev is online"
         task.status = JobSchedule.STATUS_DONE
         task.write_to_db(db_controller.kv_store)
-        return
+        return True
 
     task.status = JobSchedule.STATUS_RUNNING
     task.write_to_db(db_controller.kv_store)
 
     # resetting device
     logger.info(f"Resetting device {device.get_id()}")
-    res = device_controller.reset_storage_device(device.get_id())
+    device_controller.reset_storage_device(device.get_id())
     time.sleep(5)
     device = _get_device(task)
     if device.status == NVMeDevice.STATUS_ONLINE and device.io_error is False:
         logger.info(f"Device is online: {device.get_id()}")
         task.function_result = "done"
         task.status = JobSchedule.STATUS_DONE
         task.write_to_db(db_controller.kv_store)
-        return
+        return True
 
     logger.info(f"Restarting device {device.get_id()}")
-    res = device_controller.restart_device(device.get_id(), force=True)
+    device_controller.restart_device(device.get_id(), force=True)
     time.sleep(5)
     device = _get_device(task)
     if device.status == NVMeDevice.STATUS_ONLINE and device.io_error is False:
         logger.info(f"Device is online: {device.get_id()}")
         task.function_result = "done"
         task.status = JobSchedule.STATUS_DONE
         task.write_to_db(db_controller.kv_store)
-        return
+        return True
 
-    task.retry -= 1
+    task.retry += 1
     task.write_to_db(db_controller.kv_store)
-    return
+    return False
 
 
 # configure logging
 logger_handler = logging.StreamHandler(stream=sys.stdout)
 logger_handler.setFormatter(logging.Formatter('%(asctime)s: %(levelname)s: %(message)s'))
 gelf_handler = GELFUDPHandler('0.0.0.0', constants.GELF_PORT)
 logger = logging.getLogger()
@@ -88,19 +88,21 @@
 logger.setLevel(logging.DEBUG)
 
 # get DB controller
 db_controller = kv_store.DBController()
 
 logger.info("Starting Jobs runner...")
 while True:
-
+    time.sleep(3)
     clusters = db_controller.get_clusters()
     if not clusters:
         logger.error("No clusters found!")
     else:
         for cl in clusters:
             tasks = db_controller.get_job_tasks(cl.get_id())
             for task in tasks:
-                if task.status != JobSchedule.STATUS_DONE:
+                delay_seconds = constants.TASK_EXEC_INTERVAL_SEC
+                while task.status != JobSchedule.STATUS_DONE:
                     res = task_runner(task)
-
-    time.sleep(constants.TASK_EXEC_INTERVAL_SEC)
+                    if res is False:
+                        time.sleep(delay_seconds)
+                        delay_seconds += 2
```

## Comparing `sbcli_dev-2.8.3/simplyblock_core/services/caching_node_monitor.py` & `sbcli_dev-2.8.4/simplyblock_core/services/caching_node_monitor.py`

 * *Files identical despite different names*

## Comparing `sbcli_dev-2.8.3/simplyblock_core/services/install_service.sh` & `sbcli_dev-2.8.4/simplyblock_core/services/install_service.sh`

 * *Files identical despite different names*

## Comparing `sbcli_dev-2.8.3/simplyblock_core/services/__init__.py` & `sbcli_dev-2.8.4/simplyblock_core/services/__init__.py`

 * *Files identical despite different names*

## Comparing `sbcli_dev-2.8.3/simplyblock_core/services/log_agg_service.py` & `sbcli_dev-2.8.4/simplyblock_core/services/log_agg_service.py`

 * *Files identical despite different names*

## Comparing `sbcli_dev-2.8.3/simplyblock_core/services/health_check_service.py` & `sbcli_dev-2.8.4/simplyblock_core/services/health_check_service.py`

 * *Files identical despite different names*

## Comparing `sbcli_dev-2.8.3/simplyblock_core/services/capacity_and_stats_collector.py` & `sbcli_dev-2.8.4/simplyblock_core/services/capacity_and_stats_collector.py`

 * *Files identical despite different names*

## Comparing `sbcli_dev-2.8.3/simplyblock_core/services/device_monitor.py` & `sbcli_dev-2.8.4/simplyblock_core/services/device_monitor.py`

 * *Files identical despite different names*

## Comparing `sbcli_dev-2.8.3/simplyblock_core/services/lvol_stat_collector.py` & `sbcli_dev-2.8.4/simplyblock_core/services/lvol_stat_collector.py`

 * *Files identical despite different names*

## Comparing `sbcli_dev-2.8.3/simplyblock_core/services/cap_monitor.py` & `sbcli_dev-2.8.4/simplyblock_core/services/cap_monitor.py`

 * *Files identical despite different names*

## Comparing `sbcli_dev-2.8.3/simplyblock_core/services/storage_node_monitor.py` & `sbcli_dev-2.8.4/simplyblock_core/services/storage_node_monitor.py`

 * *Files identical despite different names*

## Comparing `sbcli_dev-2.8.3/simplyblock_core/services/port_stat_collector.py` & `sbcli_dev-2.8.4/simplyblock_core/services/port_stat_collector.py`

 * *Files identical despite different names*

## Comparing `sbcli_dev-2.8.3/simplyblock_core/services/distr_event_collector.py` & `sbcli_dev-2.8.4/simplyblock_core/services/distr_event_collector.py`

 * *Files identical despite different names*

## Comparing `sbcli_dev-2.8.3/simplyblock_core/services/mgmt_node_monitor.py` & `sbcli_dev-2.8.4/simplyblock_core/services/mgmt_node_monitor.py`

 * *Files identical despite different names*

## Comparing `sbcli_dev-2.8.3/simplyblock_core/services/lvol_monitor.py` & `sbcli_dev-2.8.4/simplyblock_core/services/lvol_monitor.py`

 * *Files identical despite different names*

## Comparing `sbcli_dev-2.8.3/simplyblock_core/controllers/pool_controller.py` & `sbcli_dev-2.8.4/simplyblock_core/controllers/pool_controller.py`

 * *Files identical despite different names*

## Comparing `sbcli_dev-2.8.3/simplyblock_core/controllers/storage_events.py` & `sbcli_dev-2.8.4/simplyblock_core/controllers/storage_events.py`

 * *Files identical despite different names*

## Comparing `sbcli_dev-2.8.3/simplyblock_core/controllers/lvol_controller.py` & `sbcli_dev-2.8.4/simplyblock_core/controllers/lvol_controller.py`

 * *Files identical despite different names*

## Comparing `sbcli_dev-2.8.3/simplyblock_core/controllers/device_events.py` & `sbcli_dev-2.8.4/simplyblock_core/controllers/device_events.py`

 * *Files identical despite different names*

## Comparing `sbcli_dev-2.8.3/simplyblock_core/controllers/lvol_events.py` & `sbcli_dev-2.8.4/simplyblock_core/controllers/lvol_events.py`

 * *Files identical despite different names*

## Comparing `sbcli_dev-2.8.3/simplyblock_core/controllers/snapshot_controller.py` & `sbcli_dev-2.8.4/simplyblock_core/controllers/snapshot_controller.py`

 * *Files identical despite different names*

## Comparing `sbcli_dev-2.8.3/simplyblock_core/controllers/snapshot_events.py` & `sbcli_dev-2.8.4/simplyblock_core/controllers/snapshot_events.py`

 * *Files identical despite different names*

## Comparing `sbcli_dev-2.8.3/simplyblock_core/controllers/events_controller.py` & `sbcli_dev-2.8.4/simplyblock_core/controllers/events_controller.py`

 * *Files identical despite different names*

## Comparing `sbcli_dev-2.8.3/simplyblock_core/controllers/health_controller.py` & `sbcli_dev-2.8.4/simplyblock_core/controllers/health_controller.py`

 * *Files identical despite different names*

## Comparing `sbcli_dev-2.8.3/simplyblock_core/controllers/device_controller.py` & `sbcli_dev-2.8.4/simplyblock_core/controllers/device_controller.py`

 * *Files identical despite different names*

## Comparing `sbcli_dev-2.8.3/simplyblock_core/controllers/pool_events.py` & `sbcli_dev-2.8.4/simplyblock_core/controllers/pool_events.py`

 * *Files identical despite different names*

## Comparing `sbcli_dev-2.8.3/simplyblock_core/controllers/caching_node_controller.py` & `sbcli_dev-2.8.4/simplyblock_core/controllers/caching_node_controller.py`

 * *Files identical despite different names*

## Comparing `sbcli_dev-2.8.3/simplyblock_core/controllers/cluster_events.py` & `sbcli_dev-2.8.4/simplyblock_core/controllers/cluster_events.py`

 * *Files identical despite different names*

## Comparing `sbcli_dev-2.8.3/simplyblock_core/controllers/mgmt_events.py` & `sbcli_dev-2.8.4/simplyblock_core/controllers/mgmt_events.py`

 * *Files identical despite different names*

## Comparing `sbcli_dev-2.8.3/simplyblock_core/models/caching_node.py` & `sbcli_dev-2.8.4/simplyblock_core/models/caching_node.py`

 * *Files identical despite different names*

## Comparing `sbcli_dev-2.8.3/simplyblock_core/models/nvme_device.py` & `sbcli_dev-2.8.4/simplyblock_core/models/nvme_device.py`

 * *Files identical despite different names*

## Comparing `sbcli_dev-2.8.3/simplyblock_core/models/mgmt_node.py` & `sbcli_dev-2.8.4/simplyblock_core/models/mgmt_node.py`

 * *Files identical despite different names*

## Comparing `sbcli_dev-2.8.3/simplyblock_core/models/compute_node.py` & `sbcli_dev-2.8.4/simplyblock_core/models/compute_node.py`

 * *Files identical despite different names*

## Comparing `sbcli_dev-2.8.3/simplyblock_core/models/events.py` & `sbcli_dev-2.8.4/simplyblock_core/models/events.py`

 * *Files identical despite different names*

## Comparing `sbcli_dev-2.8.3/simplyblock_core/models/global_settings.py` & `sbcli_dev-2.8.4/simplyblock_core/models/global_settings.py`

 * *Files identical despite different names*

## Comparing `sbcli_dev-2.8.3/simplyblock_core/models/job_schedule.py` & `sbcli_dev-2.8.4/simplyblock_core/models/job_schedule.py`

 * *Files 16% similar despite different names*

```diff
@@ -15,15 +15,15 @@
         "device_id": {"type": str, 'default': ""},
         "date": {"type": int, 'default': 0},
 
         "function_name": {"type": str, 'default': ""},
         "function_params": {"type": dict, 'default': {}},
         "function_result": {"type": str, 'default': ""},
 
-        "retry": {"type": int, 'default': 5},
+        "retry": {"type": int, 'default': 0},
         "status": {"type": str, 'default': ""},
 
     }
 
     def __init__(self, data=None):
         super(JobSchedule, self).__init__()
         self.set_attrs(self.attributes, data)
```

## Comparing `sbcli_dev-2.8.3/simplyblock_core/models/base_model.py` & `sbcli_dev-2.8.4/simplyblock_core/models/base_model.py`

 * *Files identical despite different names*

## Comparing `sbcli_dev-2.8.3/simplyblock_core/models/lvol_model.py` & `sbcli_dev-2.8.4/simplyblock_core/models/lvol_model.py`

 * *Files identical despite different names*

## Comparing `sbcli_dev-2.8.3/simplyblock_core/models/snapshot.py` & `sbcli_dev-2.8.4/simplyblock_core/models/snapshot.py`

 * *Files identical despite different names*

## Comparing `sbcli_dev-2.8.3/simplyblock_core/models/storage_node.py` & `sbcli_dev-2.8.4/simplyblock_core/models/storage_node.py`

 * *Files identical despite different names*

## Comparing `sbcli_dev-2.8.3/simplyblock_core/models/stats.py` & `sbcli_dev-2.8.4/simplyblock_core/models/stats.py`

 * *Files identical despite different names*

## Comparing `sbcli_dev-2.8.3/simplyblock_core/models/pool.py` & `sbcli_dev-2.8.4/simplyblock_core/models/pool.py`

 * *Files identical despite different names*

## Comparing `sbcli_dev-2.8.3/simplyblock_core/models/iface.py` & `sbcli_dev-2.8.4/simplyblock_core/models/iface.py`

 * *Files identical despite different names*

## Comparing `sbcli_dev-2.8.3/simplyblock_core/models/cluster.py` & `sbcli_dev-2.8.4/simplyblock_core/models/cluster.py`

 * *Files identical despite different names*

## Comparing `sbcli_dev-2.8.3/simplyblock_core/models/port_stat.py` & `sbcli_dev-2.8.4/simplyblock_core/models/port_stat.py`

 * *Files identical despite different names*

## Comparing `sbcli_dev-2.8.3/simplyblock_core/scripts/install_deps.sh` & `sbcli_dev-2.8.4/simplyblock_core/scripts/install_deps.sh`

 * *Files identical despite different names*

## Comparing `sbcli_dev-2.8.3/simplyblock_core/scripts/__init__.py` & `sbcli_dev-2.8.4/simplyblock_core/scripts/__init__.py`

 * *Files identical despite different names*

## Comparing `sbcli_dev-2.8.3/simplyblock_core/scripts/haproxy.cfg` & `sbcli_dev-2.8.4/simplyblock_core/scripts/haproxy.cfg`

 * *Files identical despite different names*

## Comparing `sbcli_dev-2.8.3/simplyblock_core/scripts/stack_deploy_wait.sh` & `sbcli_dev-2.8.4/simplyblock_core/scripts/stack_deploy_wait.sh`

 * *Files identical despite different names*

## Comparing `sbcli_dev-2.8.3/simplyblock_core/scripts/docker-compose-swarm.yml` & `sbcli_dev-2.8.4/simplyblock_core/scripts/docker-compose-swarm.yml`

 * *Files identical despite different names*

## Comparing `sbcli_dev-2.8.3/simplyblock_core/scripts/apply_dashboard.sh` & `sbcli_dev-2.8.4/simplyblock_core/scripts/apply_dashboard.sh`

 * *Files identical despite different names*

## Comparing `sbcli_dev-2.8.3/simplyblock_core/scripts/docker-compose-swarm-monitoring.yml` & `sbcli_dev-2.8.4/simplyblock_core/scripts/docker-compose-swarm-monitoring.yml`

 * *Files identical despite different names*

## Comparing `sbcli_dev-2.8.3/simplyblock_core/scripts/deploy_stack.sh` & `sbcli_dev-2.8.4/simplyblock_core/scripts/deploy_stack.sh`

 * *Files identical despite different names*

## Comparing `sbcli_dev-2.8.3/simplyblock_core/scripts/alerting/alert_rules.yaml` & `sbcli_dev-2.8.4/simplyblock_core/scripts/alerting/alert_rules.yaml`

 * *Files identical despite different names*

## Comparing `sbcli_dev-2.8.3/simplyblock_core/scripts/alerting/alert_resources.yaml` & `sbcli_dev-2.8.4/simplyblock_core/scripts/alerting/alert_resources.yaml`

 * *Files identical despite different names*

## Comparing `sbcli_dev-2.8.3/simplyblock_core/scripts/dashboards/nodes.json` & `sbcli_dev-2.8.4/simplyblock_core/scripts/dashboards/lvols.json`

 * *Files 12% similar despite different names*

### Pretty-printed

 * *Similarity: 0.9678971507561901%*

 * *Differences: {"'dashboard'": "{'panels': {1: {'targets': {0: {'editorMode': 'code', 'expr': "*

 * *                '\'lvol_size_total{cluster=~"$cluster",pool=~"$pool",lvol=~"$lvol"}\'}}, '*

 * *                "'title': 'lvol_size_total'}, 2: {'targets': {0: {'editorMode': 'code', 'expr': "*

 * *                '\'lvol_size_free{cluster=~"$cluster",pool=~"$pool",lvol=~"$lvol"}\'}}, \'title\': '*

 * *                "'lvol_size_free'}, 3: {'targets': {0: {'editorMode': 'code', 'expr': "*

 * *                '\'lvol_size_used{cluster=~"$cluster" […]*

```diff
@@ -115,22 +115,22 @@
                 },
                 "targets": [
                     {
                         "datasource": {
                             "type": "prometheus",
                             "uid": "PBFA97CFB590B2093"
                         },
-                        "editorMode": "builder",
-                        "expr": "snode_size_total",
+                        "editorMode": "code",
+                        "expr": "lvol_size_total{cluster=~\"$cluster\",pool=~\"$pool\",lvol=~\"$lvol\"}",
                         "legendFormat": "__auto",
                         "range": true,
                         "refId": "A"
                     }
                 ],
-                "title": "snode_size_total",
+                "title": "lvol_size_total",
                 "type": "timeseries"
             },
             {
                 "datasource": {
                     "type": "prometheus",
                     "uid": "PBFA97CFB590B2093"
                 },
@@ -208,22 +208,22 @@
                 },
                 "targets": [
                     {
                         "datasource": {
                             "type": "prometheus",
                             "uid": "PBFA97CFB590B2093"
                         },
-                        "editorMode": "builder",
-                        "expr": "snode_size_free",
+                        "editorMode": "code",
+                        "expr": "lvol_size_free{cluster=~\"$cluster\",pool=~\"$pool\",lvol=~\"$lvol\"}",
                         "legendFormat": "__auto",
                         "range": true,
                         "refId": "A"
                     }
                 ],
-                "title": "snode_size_free",
+                "title": "lvol_size_free",
                 "type": "timeseries"
             },
             {
                 "datasource": {
                     "type": "prometheus",
                     "uid": "PBFA97CFB590B2093"
                 },
@@ -301,22 +301,22 @@
                 },
                 "targets": [
                     {
                         "datasource": {
                             "type": "prometheus",
                             "uid": "PBFA97CFB590B2093"
                         },
-                        "editorMode": "builder",
-                        "expr": "snode_size_used",
+                        "editorMode": "code",
+                        "expr": "lvol_size_used{cluster=~\"$cluster\",pool=~\"$pool\",lvol=~\"$lvol\"}",
                         "legendFormat": "__auto",
                         "range": true,
                         "refId": "A"
                     }
                 ],
-                "title": "snode_size_used",
+                "title": "lvol_size_used",
                 "type": "timeseries"
             },
             {
                 "datasource": {
                     "type": "prometheus",
                     "uid": "PBFA97CFB590B2093"
                 },
@@ -394,22 +394,22 @@
                 },
                 "targets": [
                     {
                         "datasource": {
                             "type": "prometheus",
                             "uid": "PBFA97CFB590B2093"
                         },
-                        "editorMode": "builder",
-                        "expr": "snode_size_prov",
+                        "editorMode": "code",
+                        "expr": "lvol_size_prov{cluster=~\"$cluster\",pool=~\"$pool\",lvol=~\"$lvol\"}",
                         "legendFormat": "__auto",
                         "range": true,
                         "refId": "A"
                     }
                 ],
-                "title": "snode_size_prov",
+                "title": "lvol_size_prov",
                 "type": "timeseries"
             },
             {
                 "datasource": {
                     "type": "prometheus",
                     "uid": "PBFA97CFB590B2093"
                 },
@@ -487,22 +487,22 @@
                 },
                 "targets": [
                     {
                         "datasource": {
                             "type": "prometheus",
                             "uid": "PBFA97CFB590B2093"
                         },
-                        "editorMode": "builder",
-                        "expr": "snode_size_prov_util",
+                        "editorMode": "code",
+                        "expr": "lvol_size_prov_util{cluster=~\"$cluster\",pool=~\"$pool\",lvol=~\"$lvol\"}",
                         "legendFormat": "__auto",
                         "range": true,
                         "refId": "A"
                     }
                 ],
-                "title": "snode_size_prov_util",
+                "title": "lvol_size_prov_util",
                 "type": "timeseries"
             },
             {
                 "datasource": {
                     "type": "prometheus",
                     "uid": "PBFA97CFB590B2093"
                 },
@@ -580,22 +580,22 @@
                 },
                 "targets": [
                     {
                         "datasource": {
                             "type": "prometheus",
                             "uid": "PBFA97CFB590B2093"
                         },
-                        "editorMode": "builder",
-                        "expr": "snode_size_util",
+                        "editorMode": "code",
+                        "expr": "lvol_size_util{cluster=~\"$cluster\",pool=~\"$pool\",lvol=~\"$lvol\"}",
                         "legendFormat": "__auto",
                         "range": true,
                         "refId": "A"
                     }
                 ],
-                "title": "snode_size_util",
+                "title": "lvol_size_util",
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
@@ -686,22 +686,22 @@
                 },
                 "targets": [
                     {
                         "datasource": {
                             "type": "prometheus",
                             "uid": "PBFA97CFB590B2093"
                         },
-                        "editorMode": "builder",
-                        "expr": "snode_write_bytes",
+                        "editorMode": "code",
+                        "expr": "lvol_write_bytes{cluster=~\"$cluster\",pool=~\"$pool\",lvol=~\"$lvol\"}",
                         "legendFormat": "__auto",
                         "range": true,
                         "refId": "A"
                     }
                 ],
-                "title": "snode_write_bytes",
+                "title": "lvol_write_bytes",
                 "type": "timeseries"
             },
             {
                 "datasource": {
                     "type": "prometheus",
                     "uid": "PBFA97CFB590B2093"
                 },
@@ -749,26 +749,25 @@
                                     "value": null
                                 },
                                 {
                                     "color": "red",
                                     "value": 80
                                 }
                             ]
-                        },
-                        "unit": "binBps"
+                        }
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
-                "id": 23,
+                "id": 25,
                 "options": {
                     "legend": {
                         "calcs": [],
                         "displayMode": "list",
                         "placement": "bottom",
                         "showLegend": true
                     },
@@ -779,22 +778,22 @@
                 },
                 "targets": [
                     {
                         "datasource": {
                             "type": "prometheus",
                             "uid": "PBFA97CFB590B2093"
                         },
-                        "editorMode": "builder",
-                        "expr": "snode_write_bytes_ps",
+                        "editorMode": "code",
+                        "expr": "lvol_write_io_ps{cluster=~\"$cluster\",pool=~\"$pool\",lvol=~\"$lvol\"}",
                         "legendFormat": "__auto",
                         "range": true,
                         "refId": "A"
                     }
                 ],
-                "title": "write_speed",
+                "title": "write_iops",
                 "type": "timeseries"
             },
             {
                 "datasource": {
                     "type": "prometheus",
                     "uid": "PBFA97CFB590B2093"
                 },
@@ -847,15 +846,15 @@
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
                     "x": 14,
                     "y": 16
                 },
                 "id": 33,
                 "options": {
                     "legend": {
@@ -871,22 +870,22 @@
                 },
                 "targets": [
                     {
                         "datasource": {
                             "type": "prometheus",
                             "uid": "PBFA97CFB590B2093"
                         },
-                        "editorMode": "builder",
-                        "expr": "snode_write_latency_ticks",
+                        "editorMode": "code",
+                        "expr": "lvol_write_latency_ticks{cluster=~\"$cluster\",pool=~\"$pool\",lvol=~\"$lvol\"}",
                         "legendFormat": "__auto",
                         "range": true,
                         "refId": "A"
                     }
                 ],
-                "title": "snode_wite_latency_ticks",
+                "title": "lvol_wite_latency_ticks",
                 "type": "timeseries"
             },
             {
                 "datasource": {
                     "type": "prometheus",
                     "uid": "PBFA97CFB590B2093"
                 },
@@ -942,15 +941,15 @@
                     },
                     "overrides": []
                 },
                 "gridPos": {
                     "h": 8,
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
@@ -963,22 +962,22 @@
                 },
                 "targets": [
                     {
                         "datasource": {
                             "type": "prometheus",
                             "uid": "PBFA97CFB590B2093"
                         },
-                        "editorMode": "builder",
-                        "expr": "snode_write_io",
+                        "editorMode": "code",
+                        "expr": "lvol_write_io{cluster=~\"$cluster\",pool=~\"$pool\",lvol=~\"$lvol\"}",
                         "legendFormat": "__auto",
                         "range": true,
                         "refId": "A"
                     }
                 ],
-                "title": "snode_write_io",
+                "title": "lvol_write_io",
                 "type": "timeseries"
             },
             {
                 "datasource": {
                     "type": "prometheus",
                     "uid": "PBFA97CFB590B2093"
                 },
@@ -1026,25 +1025,26 @@
                                     "value": null
                                 },
                                 {
                                     "color": "red",
                                     "value": 80
                                 }
                             ]
-                        }
+                        },
+                        "unit": "binBps"
                     },
                     "overrides": []
                 },
                 "gridPos": {
                     "h": 8,
                     "w": 7,
                     "x": 7,
-                    "y": 23
+                    "y": 24
                 },
-                "id": 25,
+                "id": 23,
                 "options": {
                     "legend": {
                         "calcs": [],
                         "displayMode": "list",
                         "placement": "bottom",
                         "showLegend": true
                     },
@@ -1055,22 +1055,22 @@
                 },
                 "targets": [
                     {
                         "datasource": {
                             "type": "prometheus",
                             "uid": "PBFA97CFB590B2093"
                         },
-                        "editorMode": "builder",
-                        "expr": "snode_write_io_ps",
+                        "editorMode": "code",
+                        "expr": "lvol_write_bytes_ps{cluster=~\"$cluster\",pool=~\"$pool\",lvol=~\"$lvol\"}",
                         "legendFormat": "__auto",
                         "range": true,
                         "refId": "A"
                     }
                 ],
-                "title": "write_iops",
+                "title": "write_speed",
                 "type": "timeseries"
             },
             {
                 "datasource": {
                     "type": "prometheus",
                     "uid": "PBFA97CFB590B2093"
                 },
@@ -1127,15 +1127,15 @@
                     },
                     "overrides": []
                 },
                 "gridPos": {
                     "h": 8,
                     "w": 7,
                     "x": 14,
-                    "y": 23
+                    "y": 24
                 },
                 "id": 26,
                 "options": {
                     "legend": {
                         "calcs": [],
                         "displayMode": "list",
                         "placement": "bottom",
@@ -1148,31 +1148,31 @@
                 },
                 "targets": [
                     {
                         "datasource": {
                             "type": "prometheus",
                             "uid": "PBFA97CFB590B2093"
                         },
-                        "editorMode": "builder",
-                        "expr": "snode_write_latency_ps / 1000",
+                        "editorMode": "code",
+                        "expr": "lvol_write_latency_ps{cluster=~\"$cluster\",pool=~\"$pool\",lvol=~\"$lvol\"} / 1000",
                         "legendFormat": "__auto",
                         "range": true,
                         "refId": "A"
                     }
                 ],
-                "title": "snode_write_latency_ps",
+                "title": "lvol_write_latency_ps",
                 "type": "timeseries"
             },
             {
                 "collapsed": false,
                 "gridPos": {
                     "h": 1,
                     "w": 24,
                     "x": 0,
-                    "y": 31
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
-                    "y": 32
+                    "y": 33
                 },
                 "id": 1,
                 "options": {
                     "legend": {
                         "calcs": [],
                         "displayMode": "list",
                         "placement": "bottom",
@@ -1254,22 +1254,22 @@
                 },
                 "targets": [
                     {
                         "datasource": {
                             "type": "prometheus",
                             "uid": "PBFA97CFB590B2093"
                         },
-                        "editorMode": "builder",
-                        "expr": "snode_read_bytes",
+                        "editorMode": "code",
+                        "expr": "lvol_read_bytes{cluster=~\"$cluster\",pool=~\"$pool\",lvol=~\"$lvol\"}",
                         "legendFormat": "__auto",
                         "range": true,
                         "refId": "A"
                     }
                 ],
-                "title": "snode_read_bytes",
+                "title": "lvol_read_bytes",
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
-                    "y": 32
+                    "y": 33
                 },
                 "id": 2,
                 "options": {
                     "legend": {
                         "calcs": [],
                         "displayMode": "list",
                         "placement": "bottom",
@@ -1347,16 +1347,16 @@
                 },
                 "targets": [
                     {
                         "datasource": {
                             "type": "prometheus",
                             "uid": "PBFA97CFB590B2093"
                         },
-                        "editorMode": "builder",
-                        "expr": "snode_read_bytes_ps",
+                        "editorMode": "code",
+                        "expr": "lvol_read_bytes_ps{cluster=~\"$cluster\",pool=~\"$pool\",lvol=~\"$lvol\"}",
                         "legendFormat": "__auto",
                         "range": true,
                         "refId": "A"
                     }
                 ],
                 "title": "read_speed",
                 "type": "timeseries"
@@ -1419,15 +1419,15 @@
                     },
                     "overrides": []
                 },
                 "gridPos": {
                     "h": 8,
                     "w": 7,
                     "x": 14,
-                    "y": 32
+                    "y": 33
                 },
                 "id": 5,
                 "options": {
                     "legend": {
                         "calcs": [],
                         "displayMode": "list",
                         "placement": "bottom",
@@ -1440,22 +1440,22 @@
                 },
                 "targets": [
                     {
                         "datasource": {
                             "type": "prometheus",
                             "uid": "PBFA97CFB590B2093"
                         },
-                        "editorMode": "builder",
-                        "expr": "snode_read_latency_ps",
+                        "editorMode": "code",
+                        "expr": "lvol_read_latency_ps{cluster=~\"$cluster\",pool=~\"$pool\",lvol=~\"$lvol\"}",
                         "legendFormat": "__auto",
                         "range": true,
                         "refId": "A"
                     }
                 ],
-                "title": "snode_read_latency_ps",
+                "title": "lvol_read_latency_ps",
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
-                    "y": 40
+                    "y": 41
                 },
                 "id": 3,
                 "options": {
                     "legend": {
                         "calcs": [],
                         "displayMode": "list",
                         "placement": "bottom",
@@ -1532,22 +1532,22 @@
                 },
                 "targets": [
                     {
                         "datasource": {
                             "type": "prometheus",
                             "uid": "PBFA97CFB590B2093"
                         },
-                        "editorMode": "builder",
-                        "expr": "snode_read_io",
+                        "editorMode": "code",
+                        "expr": "lvol_read_io{cluster=~\"$cluster\",pool=~\"$pool\",lvol=~\"$lvol\"}",
                         "legendFormat": "__auto",
                         "range": true,
                         "refId": "A"
                     }
                 ],
-                "title": "snode_read_io",
+                "title": "lvol_read_io",
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
-                    "y": 40
+                    "y": 41
                 },
                 "id": 4,
                 "options": {
                     "legend": {
                         "calcs": [],
                         "displayMode": "list",
                         "placement": "bottom",
@@ -1624,16 +1624,16 @@
                 },
                 "targets": [
                     {
                         "datasource": {
                             "type": "prometheus",
                             "uid": "PBFA97CFB590B2093"
                         },
-                        "editorMode": "builder",
-                        "expr": "snode_read_io_ps",
+                        "editorMode": "code",
+                        "expr": "lvol_read_io_ps{cluster=~\"$cluster\",pool=~\"$pool\",lvol=~\"$lvol\"}",
                         "legendFormat": "__auto",
                         "range": true,
                         "refId": "A"
                     }
                 ],
                 "title": "read_iops",
                 "type": "timeseries"
@@ -1695,15 +1695,15 @@
                     },
                     "overrides": []
                 },
                 "gridPos": {
                     "h": 7,
                     "w": 7,
                     "x": 14,
-                    "y": 40
+                    "y": 41
                 },
                 "id": 6,
                 "options": {
                     "legend": {
                         "calcs": [],
                         "displayMode": "list",
                         "placement": "bottom",
@@ -1716,31 +1716,31 @@
                 },
                 "targets": [
                     {
                         "datasource": {
                             "type": "prometheus",
                             "uid": "PBFA97CFB590B2093"
                         },
-                        "editorMode": "builder",
-                        "expr": "snode_read_latency_ticks",
+                        "editorMode": "code",
+                        "expr": "lvol_read_latency_ticks{cluster=~\"$cluster\",pool=~\"$pool\",lvol=~\"$lvol\"}",
                         "legendFormat": "__auto",
                         "range": true,
                         "refId": "A"
                     }
                 ],
-                "title": "snode_read_latency_ticks",
+                "title": "lvol_read_latency_ticks",
                 "type": "timeseries"
             },
             {
                 "collapsed": false,
                 "gridPos": {
                     "h": 1,
                     "w": 24,
                     "x": 0,
-                    "y": 47
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
-                    "y": 48
+                    "y": 49
                 },
                 "id": 21,
                 "options": {
                     "legend": {
                         "calcs": [],
                         "displayMode": "list",
                         "placement": "bottom",
@@ -1821,22 +1821,22 @@
                 },
                 "targets": [
                     {
                         "datasource": {
                             "type": "prometheus",
                             "uid": "PBFA97CFB590B2093"
                         },
-                        "editorMode": "builder",
-                        "expr": "snode_unmap_latency_ticks",
+                        "editorMode": "code",
+                        "expr": "lvol_unmap_latency_ticks{cluster=~\"$cluster\",pool=~\"$pool\",lvol=~\"$lvol\"}",
                         "legendFormat": "__auto",
                         "range": true,
                         "refId": "A"
                     }
                 ],
-                "title": "snode_unmap_latency_ticks",
+                "title": "lvol_unmap_latency_ticks",
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
-                    "y": 48
+                    "y": 49
                 },
                 "id": 17,
                 "options": {
                     "legend": {
                         "calcs": [],
                         "displayMode": "list",
                         "placement": "bottom",
@@ -1914,22 +1914,22 @@
                 },
                 "targets": [
                     {
                         "datasource": {
                             "type": "prometheus",
                             "uid": "PBFA97CFB590B2093"
                         },
-                        "editorMode": "builder",
-                        "expr": "snode_unmap_bytes_ps",
+                        "editorMode": "code",
+                        "expr": "lvol_unmap_bytes_ps{cluster=~\"$cluster\",pool=~\"$pool\",lvol=~\"$lvol\"}",
                         "legendFormat": "__auto",
                         "range": true,
                         "refId": "A"
                     }
                 ],
-                "title": "snode_unmap_bytes_ps",
+                "title": "lvol_unmap_bytes_ps",
                 "type": "timeseries"
             },
             {
                 "datasource": {
                     "type": "prometheus",
                     "uid": "PBFA97CFB590B2093"
                 },
@@ -1987,15 +1987,15 @@
                     },
                     "overrides": []
                 },
                 "gridPos": {
                     "h": 7,
                     "w": 7,
                     "x": 14,
-                    "y": 48
+                    "y": 49
                 },
                 "id": 20,
                 "options": {
                     "legend": {
                         "calcs": [],
                         "displayMode": "list",
                         "placement": "bottom",
@@ -2008,22 +2008,22 @@
                 },
                 "targets": [
                     {
                         "datasource": {
                             "type": "prometheus",
                             "uid": "PBFA97CFB590B2093"
                         },
-                        "editorMode": "builder",
-                        "expr": "snode_unmap_latency_ps",
+                        "editorMode": "code",
+                        "expr": "lvol_unmap_latency_ps{cluster=~\"$cluster\",pool=~\"$pool\",lvol=~\"$lvol\"}",
                         "legendFormat": "__auto",
                         "range": true,
                         "refId": "A"
                     }
                 ],
-                "title": "snode_unmap_latency_ps",
+                "title": "lvol_unmap_latency_ps",
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
-                                        "{__name__=\"snode_unmap_io_ps\", cluster=\"c3663938-6610-44d5-9897-d7bfa60a43e1\", exported_job=\"collector\", instance=\"192.168.178.52:9091\", job=\"metricsgateway\"}"
+                                        "{__name__=\"lvol_unmap_io_ps\", cluster=\"c3663938-6610-44d5-9897-d7bfa60a43e1\", exported_job=\"collector\", instance=\"192.168.178.52:9091\", job=\"metricsgateway\"}"
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
-                    "y": 55
+                    "y": 56
                 },
                 "id": 19,
                 "options": {
                     "legend": {
                         "calcs": [],
                         "displayMode": "list",
                         "placement": "bottom",
@@ -2125,22 +2125,22 @@
                 },
                 "targets": [
                     {
                         "datasource": {
                             "type": "prometheus",
                             "uid": "PBFA97CFB590B2093"
                         },
-                        "editorMode": "builder",
-                        "expr": "snode_unmap_io_ps",
+                        "editorMode": "code",
+                        "expr": "lvol_unmap_io_ps{cluster=~\"$cluster\",pool=~\"$pool\",lvol=~\"$lvol\"}",
                         "legendFormat": "__auto",
                         "range": true,
                         "refId": "A"
                     }
                 ],
-                "title": "snode_unmap_io_ps",
+                "title": "lvol_unmap_io_ps",
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
-                    "y": 55
+                    "y": 56
                 },
                 "id": 18,
                 "options": {
                     "legend": {
                         "calcs": [],
                         "displayMode": "list",
                         "placement": "bottom",
@@ -2217,22 +2217,22 @@
                 },
                 "targets": [
                     {
                         "datasource": {
                             "type": "prometheus",
                             "uid": "PBFA97CFB590B2093"
                         },
-                        "editorMode": "builder",
-                        "expr": "snode_unmap_io",
+                        "editorMode": "code",
+                        "expr": "lvol_unmap_io{cluster=~\"$cluster\",pool=~\"$pool\",lvol=~\"$lvol\"}",
                         "legendFormat": "__auto",
                         "range": true,
                         "refId": "A"
                     }
                 ],
-                "title": "snode_unmap_io",
+                "title": "lvol_unmap_io",
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
+                        "unit": "binBps"
                     },
                     "overrides": []
                 },
                 "gridPos": {
                     "h": 7,
                     "w": 7,
                     "x": 14,
-                    "y": 55
+                    "y": 56
                 },
                 "id": 16,
                 "options": {
                     "legend": {
                         "calcs": [],
                         "displayMode": "list",
                         "placement": "bottom",
@@ -2310,37 +2310,134 @@
                 },
                 "targets": [
                     {
                         "datasource": {
                             "type": "prometheus",
                             "uid": "PBFA97CFB590B2093"
                         },
-                        "editorMode": "builder",
-                        "expr": "snode_unmap_bytes",
+                        "editorMode": "code",
+                        "expr": "lvol_unmap_bytes{cluster=~\"$cluster\",pool=~\"$pool\",lvol=~\"$lvol\"}",
                         "legendFormat": "__auto",
                         "range": true,
                         "refId": "A"
                     }
                 ],
-                "title": "snode_unmap_bytes",
+                "title": "lvol_unmap_bytes",
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
+                    "allValue": ".*",
+                    "current": {
+                        "selected": true,
+                        "text": [
+                            "All"
+                        ],
+                        "value": [
+                            "$__all"
+                        ]
+                    },
+                    "datasource": {
+                        "type": "prometheus",
+                        "uid": "PBFA97CFB590B2093"
+                    },
+                    "definition": "label_values(cluster)",
+                    "hide": 0,
+                    "includeAll": true,
+                    "label": "cluster",
+                    "multi": true,
+                    "name": "cluster",
+                    "options": [],
+                    "query": {
+                        "query": "label_values(cluster)",
+                        "refId": "PrometheusVariableQueryEditor-VariableQuery"
+                    },
+                    "refresh": 1,
+                    "regex": "",
+                    "skipUrlSync": false,
+                    "sort": 0,
+                    "type": "query"
+                },
+                {
+                    "allValue": ".*",
+                    "current": {
+                        "selected": true,
+                        "text": [
+                            "All"
+                        ],
+                        "value": [
+                            "$__all"
+                        ]
+                    },
+                    "datasource": {
+                        "type": "prometheus",
+                        "uid": "PBFA97CFB590B2093"
+                    },
+                    "definition": "query_result(lvol_size_total{cluster=~\"$cluster\"})",
+                    "hide": 0,
+                    "includeAll": true,
+                    "label": "pool",
+                    "multi": true,
+                    "name": "pool",
+                    "options": [],
+                    "query": {
+                        "query": "query_result(lvol_size_total{cluster=~\"$cluster\"})",
+                        "refId": "PrometheusVariableQueryEditor-VariableQuery"
+                    },
+                    "refresh": 1,
+                    "regex": ".*pool=\"(.*?)\".*",
+                    "skipUrlSync": false,
+                    "sort": 0,
+                    "type": "query"
+                },
+                {
+                    "allValue": ".*",
+                    "current": {
+                        "selected": true,
+                        "text": [
+                            "All"
+                        ],
+                        "value": [
+                            "$__all"
+                        ]
+                    },
+                    "datasource": {
+                        "type": "prometheus",
+                        "uid": "PBFA97CFB590B2093"
+                    },
+                    "definition": "query_result(lvol_size_total{cluster=~\"$cluster\",pool=~\"$pool\"})",
+                    "hide": 0,
+                    "includeAll": true,
+                    "label": "lvol",
+                    "multi": true,
+                    "name": "lvol",
+                    "options": [],
+                    "query": {
+                        "query": "query_result(lvol_size_total{cluster=~\"$cluster\",pool=~\"$pool\"})",
+                        "refId": "PrometheusVariableQueryEditor-VariableQuery"
+                    },
+                    "refresh": 1,
+                    "regex": ".*lvol=\"(.*?)\".*",
+                    "skipUrlSync": false,
+                    "sort": 0,
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
-        "title": "NodesDashboard",
-        "uid": "d56e0ae7-48d5-481d-a2ea-3192da4d9e37",
+        "title": "LvolsDashboard",
+        "uid": "d56e0ae7-48d5-481d-a2ea-3192da4d9e19",
         "version": 5,
         "weekStart": ""
     }
 }
```

## Comparing `sbcli_dev-2.8.3/simplyblock_core/scripts/dashboards/cluster.json` & `sbcli_dev-2.8.4/simplyblock_core/scripts/dashboards/cluster.json`

 * *Files 6% similar despite different names*

### Pretty-printed

 * *Similarity: 0.9936935767925605%*

 * *Differences: {"'dashboard'": "{'panels': {1: {'targets': {0: {'expr': "*

 * *                '\'cluster_size_total{cluster="$Cluster"}\'}}}, 2: {\'targets\': {0: {\'expr\': '*

 * *                '\'cluster_size_free{cluster="$Cluster"}\'}}}, 3: {\'targets\': {0: {\'expr\': '*

 * *                '\'cluster_size_used{cluster="$Cluster"}\'}}}, 4: {\'targets\': {0: {\'expr\': '*

 * *                '\'cluster_size_prov{cluster="$Cluster"}\'}}}, 5: {\'targets\': {0: {\'expr\': '*

 * *                '\'cluster_size_prov_util{cluster="$Cluster"}\'} […]*

```diff
@@ -116,15 +116,15 @@
                 "targets": [
                     {
                         "datasource": {
                             "type": "prometheus",
                             "uid": "PBFA97CFB590B2093"
                         },
                         "editorMode": "builder",
-                        "expr": "cluster_size_total",
+                        "expr": "cluster_size_total{cluster=\"$Cluster\"}",
                         "legendFormat": "__auto",
                         "range": true,
                         "refId": "A"
                     }
                 ],
                 "title": "cluster_size_total",
                 "type": "timeseries"
@@ -209,15 +209,15 @@
                 "targets": [
                     {
                         "datasource": {
                             "type": "prometheus",
                             "uid": "PBFA97CFB590B2093"
                         },
                         "editorMode": "builder",
-                        "expr": "cluster_size_free",
+                        "expr": "cluster_size_free{cluster=\"$Cluster\"}",
                         "legendFormat": "__auto",
                         "range": true,
                         "refId": "A"
                     }
                 ],
                 "title": "cluster_size_free",
                 "type": "timeseries"
@@ -302,15 +302,15 @@
                 "targets": [
                     {
                         "datasource": {
                             "type": "prometheus",
                             "uid": "PBFA97CFB590B2093"
                         },
                         "editorMode": "builder",
-                        "expr": "cluster_size_used",
+                        "expr": "cluster_size_used{cluster=\"$Cluster\"}",
                         "legendFormat": "__auto",
                         "range": true,
                         "refId": "A"
                     }
                 ],
                 "title": "cluster_size_used",
                 "type": "timeseries"
@@ -395,15 +395,15 @@
                 "targets": [
                     {
                         "datasource": {
                             "type": "prometheus",
                             "uid": "PBFA97CFB590B2093"
                         },
                         "editorMode": "builder",
-                        "expr": "cluster_size_prov",
+                        "expr": "cluster_size_prov{cluster=\"$Cluster\"}",
                         "legendFormat": "__auto",
                         "range": true,
                         "refId": "A"
                     }
                 ],
                 "title": "cluster_size_prov",
                 "type": "timeseries"
@@ -488,15 +488,15 @@
                 "targets": [
                     {
                         "datasource": {
                             "type": "prometheus",
                             "uid": "PBFA97CFB590B2093"
                         },
                         "editorMode": "builder",
-                        "expr": "cluster_size_prov_util",
+                        "expr": "cluster_size_prov_util{cluster=\"$Cluster\"}",
                         "legendFormat": "__auto",
                         "range": true,
                         "refId": "A"
                     }
                 ],
                 "title": "cluster_size_prov_util",
                 "type": "timeseries"
@@ -581,15 +581,15 @@
                 "targets": [
                     {
                         "datasource": {
                             "type": "prometheus",
                             "uid": "PBFA97CFB590B2093"
                         },
                         "editorMode": "builder",
-                        "expr": "cluster_size_util",
+                        "expr": "cluster_size_util{cluster=\"$Cluster\"}",
                         "legendFormat": "__auto",
                         "range": true,
                         "refId": "A"
                     }
                 ],
                 "title": "cluster_size_util",
                 "type": "timeseries"
@@ -648,16 +648,15 @@
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
@@ -687,15 +686,15 @@
                 "targets": [
                     {
                         "datasource": {
                             "type": "prometheus",
                             "uid": "PBFA97CFB590B2093"
                         },
                         "editorMode": "builder",
-                        "expr": "cluster_write_bytes",
+                        "expr": "cluster_write_bytes{cluster=\"$Cluster\"}",
                         "legendFormat": "__auto",
                         "range": true,
                         "refId": "A"
                     }
                 ],
                 "title": "cluster_write_bytes",
                 "type": "timeseries"
@@ -741,16 +740,15 @@
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
@@ -780,15 +778,15 @@
                 "targets": [
                     {
                         "datasource": {
                             "type": "prometheus",
                             "uid": "PBFA97CFB590B2093"
                         },
                         "editorMode": "builder",
-                        "expr": "cluster_write_bytes_ps",
+                        "expr": "cluster_write_bytes_ps{cluster=\"$Cluster\"}",
                         "legendFormat": "__auto",
                         "range": true,
                         "refId": "A"
                     }
                 ],
                 "title": "write_speed",
                 "type": "timeseries"
@@ -834,16 +832,15 @@
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
@@ -873,15 +870,15 @@
                 "targets": [
                     {
                         "datasource": {
                             "type": "prometheus",
                             "uid": "PBFA97CFB590B2093"
                         },
                         "editorMode": "builder",
-                        "expr": "cluster_write_latency_ps / 1000",
+                        "expr": "cluster_write_latency_ps{cluster=\"$Cluster\"} / 1000",
                         "legendFormat": "__auto",
                         "range": true,
                         "refId": "A"
                     }
                 ],
                 "title": "cluster_write_latency_ps",
                 "type": "timeseries"
@@ -927,16 +924,15 @@
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
@@ -965,15 +961,15 @@
                 "targets": [
                     {
                         "datasource": {
                             "type": "prometheus",
                             "uid": "PBFA97CFB590B2093"
                         },
                         "editorMode": "builder",
-                        "expr": "cluster_write_io",
+                        "expr": "cluster_write_io{cluster=\"$Cluster\"}",
                         "legendFormat": "__auto",
                         "range": true,
                         "refId": "A"
                     }
                 ],
                 "title": "cluster_write_io",
                 "type": "timeseries"
@@ -1019,16 +1015,15 @@
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
@@ -1057,15 +1052,15 @@
                 "targets": [
                     {
                         "datasource": {
                             "type": "prometheus",
                             "uid": "PBFA97CFB590B2093"
                         },
                         "editorMode": "builder",
-                        "expr": "cluster_write_io_ps",
+                        "expr": "cluster_write_io_ps{cluster=\"$Cluster\"}",
                         "legendFormat": "__auto",
                         "range": true,
                         "refId": "A"
                     }
                 ],
                 "title": "write_iops",
                 "type": "timeseries"
@@ -1111,16 +1106,15 @@
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
@@ -1149,15 +1143,15 @@
                 "targets": [
                     {
                         "datasource": {
                             "type": "prometheus",
                             "uid": "PBFA97CFB590B2093"
                         },
                         "editorMode": "builder",
-                        "expr": "cluster_write_latency_ticks",
+                        "expr": "cluster_write_latency_ticks{cluster=\"$Cluster\"}",
                         "legendFormat": "__auto",
                         "range": true,
                         "refId": "A"
                     }
                 ],
                 "title": "cluster_wite_latency_ticks",
                 "type": "timeseries"
@@ -1216,16 +1210,15 @@
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
@@ -1255,15 +1248,15 @@
                 "targets": [
                     {
                         "datasource": {
                             "type": "prometheus",
                             "uid": "PBFA97CFB590B2093"
                         },
                         "editorMode": "builder",
-                        "expr": "cluster_read_bytes",
+                        "expr": "cluster_read_bytes{cluster=\"$Cluster\"}",
                         "legendFormat": "__auto",
                         "range": true,
                         "refId": "A"
                     }
                 ],
                 "title": "cluster_read_bytes",
                 "type": "timeseries"
@@ -1309,16 +1302,15 @@
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
@@ -1348,15 +1340,15 @@
                 "targets": [
                     {
                         "datasource": {
                             "type": "prometheus",
                             "uid": "PBFA97CFB590B2093"
                         },
                         "editorMode": "builder",
-                        "expr": "cluster_read_bytes_ps",
+                        "expr": "cluster_read_bytes_ps{cluster=\"$Cluster\"}",
                         "legendFormat": "__auto",
                         "range": true,
                         "refId": "A"
                     }
                 ],
                 "title": "read_speed",
                 "type": "timeseries"
@@ -1402,16 +1394,15 @@
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
@@ -1441,15 +1432,15 @@
                 "targets": [
                     {
                         "datasource": {
                             "type": "prometheus",
                             "uid": "PBFA97CFB590B2093"
                         },
                         "editorMode": "builder",
-                        "expr": "cluster_read_latency_ps",
+                        "expr": "cluster_read_latency_ps{cluster=\"$Cluster\"}",
                         "legendFormat": "__auto",
                         "range": true,
                         "refId": "A"
                     }
                 ],
                 "title": "cluster_read_latency_ps",
                 "type": "timeseries"
@@ -1495,16 +1486,15 @@
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
@@ -1533,15 +1523,15 @@
                 "targets": [
                     {
                         "datasource": {
                             "type": "prometheus",
                             "uid": "PBFA97CFB590B2093"
                         },
                         "editorMode": "builder",
-                        "expr": "cluster_read_io",
+                        "expr": "cluster_read_io{cluster=\"$Cluster\"}",
                         "legendFormat": "__auto",
                         "range": true,
                         "refId": "A"
                     }
                 ],
                 "title": "cluster_read_io",
                 "type": "timeseries"
@@ -1587,16 +1577,15 @@
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
@@ -1625,15 +1614,15 @@
                 "targets": [
                     {
                         "datasource": {
                             "type": "prometheus",
                             "uid": "PBFA97CFB590B2093"
                         },
                         "editorMode": "builder",
-                        "expr": "cluster_read_io_ps",
+                        "expr": "cluster_read_io_ps{cluster=\"$Cluster\"}",
                         "legendFormat": "__auto",
                         "range": true,
                         "refId": "A"
                     }
                 ],
                 "title": "read_iops",
                 "type": "timeseries"
@@ -1679,16 +1668,15 @@
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
@@ -1717,15 +1705,15 @@
                 "targets": [
                     {
                         "datasource": {
                             "type": "prometheus",
                             "uid": "PBFA97CFB590B2093"
                         },
                         "editorMode": "builder",
-                        "expr": "cluster_read_latency_ticks",
+                        "expr": "cluster_read_latency_ticks{cluster=\"$Cluster\"}",
                         "legendFormat": "__auto",
                         "range": true,
                         "refId": "A"
                     }
                 ],
                 "title": "cluster_read_latency_ticks",
                 "type": "timeseries"
@@ -1784,16 +1772,15 @@
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
@@ -1822,15 +1809,15 @@
                 "targets": [
                     {
                         "datasource": {
                             "type": "prometheus",
                             "uid": "PBFA97CFB590B2093"
                         },
                         "editorMode": "builder",
-                        "expr": "cluster_unmap_latency_ticks",
+                        "expr": "cluster_unmap_latency_ticks{cluster=\"$Cluster\"}",
                         "legendFormat": "__auto",
                         "range": true,
                         "refId": "A"
                     }
                 ],
                 "title": "cluster_unmap_latency_ticks",
                 "type": "timeseries"
@@ -1876,16 +1863,15 @@
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
@@ -1915,15 +1901,15 @@
                 "targets": [
                     {
                         "datasource": {
                             "type": "prometheus",
                             "uid": "PBFA97CFB590B2093"
                         },
                         "editorMode": "builder",
-                        "expr": "cluster_unmap_bytes_ps",
+                        "expr": "cluster_unmap_bytes_ps{cluster=\"$Cluster\"}",
                         "legendFormat": "__auto",
                         "range": true,
                         "refId": "A"
                     }
                 ],
                 "title": "cluster_unmap_bytes_ps",
                 "type": "timeseries"
@@ -1970,16 +1956,15 @@
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
@@ -2009,15 +1994,15 @@
                 "targets": [
                     {
                         "datasource": {
                             "type": "prometheus",
                             "uid": "PBFA97CFB590B2093"
                         },
                         "editorMode": "builder",
-                        "expr": "cluster_unmap_latency_ps",
+                        "expr": "cluster_unmap_latency_ps{cluster=\"$Cluster\"}",
                         "legendFormat": "__auto",
                         "range": true,
                         "refId": "A"
                     }
                 ],
                 "title": "cluster_unmap_latency_ps",
                 "type": "timeseries"
@@ -2063,16 +2048,15 @@
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
@@ -2126,15 +2110,15 @@
                 "targets": [
                     {
                         "datasource": {
                             "type": "prometheus",
                             "uid": "PBFA97CFB590B2093"
                         },
                         "editorMode": "builder",
-                        "expr": "cluster_unmap_io_ps",
+                        "expr": "cluster_unmap_io_ps{cluster=\"$Cluster\"}",
                         "legendFormat": "__auto",
                         "range": true,
                         "refId": "A"
                     }
                 ],
                 "title": "cluster_unmap_io_ps",
                 "type": "timeseries"
@@ -2180,16 +2164,15 @@
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
@@ -2218,15 +2201,15 @@
                 "targets": [
                     {
                         "datasource": {
                             "type": "prometheus",
                             "uid": "PBFA97CFB590B2093"
                         },
                         "editorMode": "builder",
-                        "expr": "cluster_unmap_io",
+                        "expr": "cluster_unmap_io{cluster=\"$Cluster\"}",
                         "legendFormat": "__auto",
                         "range": true,
                         "refId": "A"
                     }
                 ],
                 "title": "cluster_unmap_io",
                 "type": "timeseries"
@@ -2272,16 +2255,15 @@
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
@@ -2311,30 +2293,59 @@
                 "targets": [
                     {
                         "datasource": {
                             "type": "prometheus",
                             "uid": "PBFA97CFB590B2093"
                         },
                         "editorMode": "builder",
-                        "expr": "cluster_unmap_bytes",
+                        "expr": "cluster_unmap_bytes{cluster=\"$Cluster\"}",
                         "legendFormat": "__auto",
                         "range": true,
                         "refId": "A"
                     }
                 ],
                 "title": "cluster_unmap_bytes",
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
```

## Comparing `sbcli_dev-2.8.3/simplyblock_core/scripts/dashboards/lvols.json` & `sbcli_dev-2.8.4/simplyblock_core/scripts/dashboards/nodes.json`

 * *Files 16% similar despite different names*

### Pretty-printed

 * *Similarity: 0.9553901753097616%*

 * *Differences: {"'dashboard'": "{'panels': {1: {'fieldConfig': {'overrides': [OrderedDict([('__systemRef', "*

 * *                "'hideSeriesFrom'), ('matcher', OrderedDict([('id', 'byNames'), ('options', "*

 * *                "OrderedDict([('mode', 'exclude'), ('names', "*

 * *                '[\'{__name__="snode_size_total", cluster="9baa11f4-0b47-47e1-9dec-20dacdda59d0", '*

 * *                'exported_job="collector", instance="pushgateway:9091", job="metricsgateway", '*

 * *                'snode="90499750-6b1e-4452-8ff5-125166f33865"}\'] […]*

```diff
@@ -88,15 +88,40 @@
                                     "color": "red",
                                     "value": 80
                                 }
                             ]
                         },
                         "unit": "bytes"
                     },
-                    "overrides": []
+                    "overrides": [
+                        {
+                            "__systemRef": "hideSeriesFrom",
+                            "matcher": {
+                                "id": "byNames",
+                                "options": {
+                                    "mode": "exclude",
+                                    "names": [
+                                        "{__name__=\"snode_size_total\", cluster=\"9baa11f4-0b47-47e1-9dec-20dacdda59d0\", exported_job=\"collector\", instance=\"pushgateway:9091\", job=\"metricsgateway\", snode=\"90499750-6b1e-4452-8ff5-125166f33865\"}"
+                                    ],
+                                    "prefix": "All except:",
+                                    "readOnly": true
+                                }
+                            },
+                            "properties": [
+                                {
+                                    "id": "custom.hideFrom",
+                                    "value": {
+                                        "legend": false,
+                                        "tooltip": false,
+                                        "viz": true
+                                    }
+                                }
+                            ]
+                        }
+                    ]
                 },
                 "gridPos": {
                     "h": 7,
                     "w": 7,
                     "x": 0,
                     "y": 1
                 },
@@ -115,22 +140,22 @@
                 },
                 "targets": [
                     {
                         "datasource": {
                             "type": "prometheus",
                             "uid": "PBFA97CFB590B2093"
                         },
-                        "editorMode": "builder",
-                        "expr": "lvol_size_total",
+                        "editorMode": "code",
+                        "expr": "snode_size_total{cluster=~\"$cluster\",snode=~\"$node\"}",
                         "legendFormat": "__auto",
                         "range": true,
                         "refId": "A"
                     }
                 ],
-                "title": "lvol_size_total",
+                "title": "snode_size_total",
                 "type": "timeseries"
             },
             {
                 "datasource": {
                     "type": "prometheus",
                     "uid": "PBFA97CFB590B2093"
                 },
@@ -208,22 +233,22 @@
                 },
                 "targets": [
                     {
                         "datasource": {
                             "type": "prometheus",
                             "uid": "PBFA97CFB590B2093"
                         },
-                        "editorMode": "builder",
-                        "expr": "lvol_size_free",
+                        "editorMode": "code",
+                        "expr": "snode_size_free{cluster=~\"$cluster\",snode=~\"$node\"}",
                         "legendFormat": "__auto",
                         "range": true,
                         "refId": "A"
                     }
                 ],
-                "title": "lvol_size_free",
+                "title": "snode_size_free",
                 "type": "timeseries"
             },
             {
                 "datasource": {
                     "type": "prometheus",
                     "uid": "PBFA97CFB590B2093"
                 },
@@ -301,22 +326,22 @@
                 },
                 "targets": [
                     {
                         "datasource": {
                             "type": "prometheus",
                             "uid": "PBFA97CFB590B2093"
                         },
-                        "editorMode": "builder",
-                        "expr": "lvol_size_used",
+                        "editorMode": "code",
+                        "expr": "snode_size_used{cluster=~\"$cluster\",snode=~\"$node\"}",
                         "legendFormat": "__auto",
                         "range": true,
                         "refId": "A"
                     }
                 ],
-                "title": "lvol_size_used",
+                "title": "snode_size_used",
                 "type": "timeseries"
             },
             {
                 "datasource": {
                     "type": "prometheus",
                     "uid": "PBFA97CFB590B2093"
                 },
@@ -394,22 +419,22 @@
                 },
                 "targets": [
                     {
                         "datasource": {
                             "type": "prometheus",
                             "uid": "PBFA97CFB590B2093"
                         },
-                        "editorMode": "builder",
-                        "expr": "lvol_size_prov",
+                        "editorMode": "code",
+                        "expr": "snode_size_prov{cluster=~\"$cluster\",snode=~\"$node\"}",
                         "legendFormat": "__auto",
                         "range": true,
                         "refId": "A"
                     }
                 ],
-                "title": "lvol_size_prov",
+                "title": "snode_size_prov",
                 "type": "timeseries"
             },
             {
                 "datasource": {
                     "type": "prometheus",
                     "uid": "PBFA97CFB590B2093"
                 },
@@ -487,22 +512,22 @@
                 },
                 "targets": [
                     {
                         "datasource": {
                             "type": "prometheus",
                             "uid": "PBFA97CFB590B2093"
                         },
-                        "editorMode": "builder",
-                        "expr": "lvol_size_prov_util",
+                        "editorMode": "code",
+                        "expr": "snode_size_prov_util{cluster=~\"$cluster\",snode=~\"$node\"}",
                         "legendFormat": "__auto",
                         "range": true,
                         "refId": "A"
                     }
                 ],
-                "title": "lvol_size_prov_util",
+                "title": "snode_size_prov_util",
                 "type": "timeseries"
             },
             {
                 "datasource": {
                     "type": "prometheus",
                     "uid": "PBFA97CFB590B2093"
                 },
@@ -580,22 +605,22 @@
                 },
                 "targets": [
                     {
                         "datasource": {
                             "type": "prometheus",
                             "uid": "PBFA97CFB590B2093"
                         },
-                        "editorMode": "builder",
-                        "expr": "lvol_size_util",
+                        "editorMode": "code",
+                        "expr": "snode_size_util{cluster=~\"$cluster\",snode=~\"$node\"}",
                         "legendFormat": "__auto",
                         "range": true,
                         "refId": "A"
                     }
                 ],
-                "title": "lvol_size_util",
+                "title": "snode_size_util",
                 "type": "timeseries"
             },
             {
                 "collapsed": false,
                 "gridPos": {
                     "h": 1,
                     "w": 24,
@@ -662,15 +687,15 @@
                             ]
                         },
                         "unit": "bytes"
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
@@ -686,22 +711,22 @@
                 },
                 "targets": [
                     {
                         "datasource": {
                             "type": "prometheus",
                             "uid": "PBFA97CFB590B2093"
                         },
-                        "editorMode": "builder",
-                        "expr": "lvol_write_bytes",
+                        "editorMode": "code",
+                        "expr": "snode_write_bytes{cluster=~\"$cluster\",snode=~\"$node\"}",
                         "legendFormat": "__auto",
                         "range": true,
                         "refId": "A"
                     }
                 ],
-                "title": "lvol_write_bytes",
+                "title": "snode_write_bytes",
                 "type": "timeseries"
             },
             {
                 "datasource": {
                     "type": "prometheus",
                     "uid": "PBFA97CFB590B2093"
                 },
@@ -749,25 +774,26 @@
                                     "value": null
                                 },
                                 {
                                     "color": "red",
                                     "value": 80
                                 }
                             ]
-                        }
+                        },
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
-                "id": 25,
+                "id": 23,
                 "options": {
                     "legend": {
                         "calcs": [],
                         "displayMode": "list",
                         "placement": "bottom",
                         "showLegend": true
                     },
@@ -778,22 +804,22 @@
                 },
                 "targets": [
                     {
                         "datasource": {
                             "type": "prometheus",
                             "uid": "PBFA97CFB590B2093"
                         },
-                        "editorMode": "builder",
-                        "expr": "lvol_write_io_ps",
+                        "editorMode": "code",
+                        "expr": "snode_write_bytes_ps{cluster=~\"$cluster\",snode=~\"$node\"}",
                         "legendFormat": "__auto",
                         "range": true,
                         "refId": "A"
                     }
                 ],
-                "title": "write_iops",
+                "title": "write_speed",
                 "type": "timeseries"
             },
             {
                 "datasource": {
                     "type": "prometheus",
                     "uid": "PBFA97CFB590B2093"
                 },
@@ -846,15 +872,15 @@
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
                     "x": 14,
                     "y": 16
                 },
                 "id": 33,
                 "options": {
                     "legend": {
@@ -870,22 +896,22 @@
                 },
                 "targets": [
                     {
                         "datasource": {
                             "type": "prometheus",
                             "uid": "PBFA97CFB590B2093"
                         },
-                        "editorMode": "builder",
-                        "expr": "lvol_write_latency_ticks",
+                        "editorMode": "code",
+                        "expr": "snode_write_latency_ticks{cluster=~\"$cluster\",snode=~\"$node\"}",
                         "legendFormat": "__auto",
                         "range": true,
                         "refId": "A"
                     }
                 ],
-                "title": "lvol_wite_latency_ticks",
+                "title": "snode_wite_latency_ticks",
                 "type": "timeseries"
             },
             {
                 "datasource": {
                     "type": "prometheus",
                     "uid": "PBFA97CFB590B2093"
                 },
@@ -941,15 +967,15 @@
                     },
                     "overrides": []
                 },
                 "gridPos": {
                     "h": 8,
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
@@ -962,22 +988,22 @@
                 },
                 "targets": [
                     {
                         "datasource": {
                             "type": "prometheus",
                             "uid": "PBFA97CFB590B2093"
                         },
-                        "editorMode": "builder",
-                        "expr": "lvol_write_io",
+                        "editorMode": "code",
+                        "expr": "snode_write_io{cluster=~\"$cluster\",snode=~\"$node\"}",
                         "legendFormat": "__auto",
                         "range": true,
                         "refId": "A"
                     }
                 ],
-                "title": "lvol_write_io",
+                "title": "snode_write_io",
                 "type": "timeseries"
             },
             {
                 "datasource": {
                     "type": "prometheus",
                     "uid": "PBFA97CFB590B2093"
                 },
@@ -1025,26 +1051,25 @@
                                     "value": null
                                 },
                                 {
                                     "color": "red",
                                     "value": 80
                                 }
                             ]
-                        },
-                        "unit": "binBps"
+                        }
                     },
                     "overrides": []
                 },
                 "gridPos": {
                     "h": 8,
                     "w": 7,
                     "x": 7,
-                    "y": 24
+                    "y": 23
                 },
-                "id": 23,
+                "id": 25,
                 "options": {
                     "legend": {
                         "calcs": [],
                         "displayMode": "list",
                         "placement": "bottom",
                         "showLegend": true
                     },
@@ -1055,22 +1080,22 @@
                 },
                 "targets": [
                     {
                         "datasource": {
                             "type": "prometheus",
                             "uid": "PBFA97CFB590B2093"
                         },
-                        "editorMode": "builder",
-                        "expr": "lvol_write_bytes_ps",
+                        "editorMode": "code",
+                        "expr": "snode_write_io_ps{cluster=~\"$cluster\",snode=~\"$node\"}",
                         "legendFormat": "__auto",
                         "range": true,
                         "refId": "A"
                     }
                 ],
-                "title": "write_speed",
+                "title": "write_iops",
                 "type": "timeseries"
             },
             {
                 "datasource": {
                     "type": "prometheus",
                     "uid": "PBFA97CFB590B2093"
                 },
@@ -1127,15 +1152,15 @@
                     },
                     "overrides": []
                 },
                 "gridPos": {
                     "h": 8,
                     "w": 7,
                     "x": 14,
-                    "y": 24
+                    "y": 23
                 },
                 "id": 26,
                 "options": {
                     "legend": {
                         "calcs": [],
                         "displayMode": "list",
                         "placement": "bottom",
@@ -1148,31 +1173,31 @@
                 },
                 "targets": [
                     {
                         "datasource": {
                             "type": "prometheus",
                             "uid": "PBFA97CFB590B2093"
                         },
-                        "editorMode": "builder",
-                        "expr": "lvol_write_latency_ps / 1000",
+                        "editorMode": "code",
+                        "expr": "snode_write_latency_ps{cluster=~\"$cluster\",snode=~\"$node\"} / 1000",
                         "legendFormat": "__auto",
                         "range": true,
                         "refId": "A"
                     }
                 ],
-                "title": "lvol_write_latency_ps",
+                "title": "snode_write_latency_ps",
                 "type": "timeseries"
             },
             {
                 "collapsed": false,
                 "gridPos": {
                     "h": 1,
                     "w": 24,
                     "x": 0,
-                    "y": 32
+                    "y": 31
                 },
                 "id": 30,
                 "panels": [],
                 "title": "Reads",
                 "type": "row"
             },
             {
@@ -1233,15 +1258,15 @@
                     },
                     "overrides": []
                 },
                 "gridPos": {
                     "h": 8,
                     "w": 7,
                     "x": 0,
-                    "y": 33
+                    "y": 32
                 },
                 "id": 1,
                 "options": {
                     "legend": {
                         "calcs": [],
                         "displayMode": "list",
                         "placement": "bottom",
@@ -1254,22 +1279,22 @@
                 },
                 "targets": [
                     {
                         "datasource": {
                             "type": "prometheus",
                             "uid": "PBFA97CFB590B2093"
                         },
-                        "editorMode": "builder",
-                        "expr": "lvol_read_bytes",
+                        "editorMode": "code",
+                        "expr": "snode_read_bytes{cluster=~\"$cluster\",snode=~\"$node\"}",
                         "legendFormat": "__auto",
                         "range": true,
                         "refId": "A"
                     }
                 ],
-                "title": "lvol_read_bytes",
+                "title": "snode_read_bytes",
                 "type": "timeseries"
             },
             {
                 "datasource": {
                     "type": "prometheus",
                     "uid": "PBFA97CFB590B2093"
                 },
@@ -1326,15 +1351,15 @@
                     },
                     "overrides": []
                 },
                 "gridPos": {
                     "h": 8,
                     "w": 7,
                     "x": 7,
-                    "y": 33
+                    "y": 32
                 },
                 "id": 2,
                 "options": {
                     "legend": {
                         "calcs": [],
                         "displayMode": "list",
                         "placement": "bottom",
@@ -1347,16 +1372,16 @@
                 },
                 "targets": [
                     {
                         "datasource": {
                             "type": "prometheus",
                             "uid": "PBFA97CFB590B2093"
                         },
-                        "editorMode": "builder",
-                        "expr": "lvol_read_bytes_ps",
+                        "editorMode": "code",
+                        "expr": "snode_read_bytes_ps{cluster=~\"$cluster\",snode=~\"$node\"}",
                         "legendFormat": "__auto",
                         "range": true,
                         "refId": "A"
                     }
                 ],
                 "title": "read_speed",
                 "type": "timeseries"
@@ -1419,15 +1444,15 @@
                     },
                     "overrides": []
                 },
                 "gridPos": {
                     "h": 8,
                     "w": 7,
                     "x": 14,
-                    "y": 33
+                    "y": 32
                 },
                 "id": 5,
                 "options": {
                     "legend": {
                         "calcs": [],
                         "displayMode": "list",
                         "placement": "bottom",
@@ -1440,22 +1465,22 @@
                 },
                 "targets": [
                     {
                         "datasource": {
                             "type": "prometheus",
                             "uid": "PBFA97CFB590B2093"
                         },
-                        "editorMode": "builder",
-                        "expr": "lvol_read_latency_ps",
+                        "editorMode": "code",
+                        "expr": "snode_read_latency_ps{cluster=~\"$cluster\",snode=~\"$node\"}",
                         "legendFormat": "__auto",
                         "range": true,
                         "refId": "A"
                     }
                 ],
-                "title": "lvol_read_latency_ps",
+                "title": "snode_read_latency_ps",
                 "type": "timeseries"
             },
             {
                 "datasource": {
                     "type": "prometheus",
                     "uid": "PBFA97CFB590B2093"
                 },
@@ -1511,15 +1536,15 @@
                     },
                     "overrides": []
                 },
                 "gridPos": {
                     "h": 7,
                     "w": 7,
                     "x": 0,
-                    "y": 41
+                    "y": 40
                 },
                 "id": 3,
                 "options": {
                     "legend": {
                         "calcs": [],
                         "displayMode": "list",
                         "placement": "bottom",
@@ -1532,22 +1557,22 @@
                 },
                 "targets": [
                     {
                         "datasource": {
                             "type": "prometheus",
                             "uid": "PBFA97CFB590B2093"
                         },
-                        "editorMode": "builder",
-                        "expr": "lvol_read_io",
+                        "editorMode": "code",
+                        "expr": "snode_read_io{cluster=~\"$cluster\",snode=~\"$node\"}",
                         "legendFormat": "__auto",
                         "range": true,
                         "refId": "A"
                     }
                 ],
-                "title": "lvol_read_io",
+                "title": "snode_read_io",
                 "type": "timeseries"
             },
             {
                 "datasource": {
                     "type": "prometheus",
                     "uid": "PBFA97CFB590B2093"
                 },
@@ -1603,15 +1628,15 @@
                     },
                     "overrides": []
                 },
                 "gridPos": {
                     "h": 7,
                     "w": 7,
                     "x": 7,
-                    "y": 41
+                    "y": 40
                 },
                 "id": 4,
                 "options": {
                     "legend": {
                         "calcs": [],
                         "displayMode": "list",
                         "placement": "bottom",
@@ -1624,16 +1649,16 @@
                 },
                 "targets": [
                     {
                         "datasource": {
                             "type": "prometheus",
                             "uid": "PBFA97CFB590B2093"
                         },
-                        "editorMode": "builder",
-                        "expr": "lvol_read_io_ps",
+                        "editorMode": "code",
+                        "expr": "snode_read_io_ps{cluster=~\"$cluster\",snode=~\"$node\"}",
                         "legendFormat": "__auto",
                         "range": true,
                         "refId": "A"
                     }
                 ],
                 "title": "read_iops",
                 "type": "timeseries"
@@ -1695,15 +1720,15 @@
                     },
                     "overrides": []
                 },
                 "gridPos": {
                     "h": 7,
                     "w": 7,
                     "x": 14,
-                    "y": 41
+                    "y": 40
                 },
                 "id": 6,
                 "options": {
                     "legend": {
                         "calcs": [],
                         "displayMode": "list",
                         "placement": "bottom",
@@ -1716,31 +1741,31 @@
                 },
                 "targets": [
                     {
                         "datasource": {
                             "type": "prometheus",
                             "uid": "PBFA97CFB590B2093"
                         },
-                        "editorMode": "builder",
-                        "expr": "lvol_read_latency_ticks",
+                        "editorMode": "code",
+                        "expr": "snode_read_latency_ticks{cluster=~\"$cluster\",snode=~\"$node\"}",
                         "legendFormat": "__auto",
                         "range": true,
                         "refId": "A"
                     }
                 ],
-                "title": "lvol_read_latency_ticks",
+                "title": "snode_read_latency_ticks",
                 "type": "timeseries"
             },
             {
                 "collapsed": false,
                 "gridPos": {
                     "h": 1,
                     "w": 24,
                     "x": 0,
-                    "y": 48
+                    "y": 47
                 },
                 "id": 29,
                 "panels": [],
                 "title": "unmap",
                 "type": "row"
             },
             {
@@ -1800,15 +1825,15 @@
                     },
                     "overrides": []
                 },
                 "gridPos": {
                     "h": 7,
                     "w": 7,
                     "x": 0,
-                    "y": 49
+                    "y": 48
                 },
                 "id": 21,
                 "options": {
                     "legend": {
                         "calcs": [],
                         "displayMode": "list",
                         "placement": "bottom",
@@ -1821,22 +1846,22 @@
                 },
                 "targets": [
                     {
                         "datasource": {
                             "type": "prometheus",
                             "uid": "PBFA97CFB590B2093"
                         },
-                        "editorMode": "builder",
-                        "expr": "lvol_unmap_latency_ticks",
+                        "editorMode": "code",
+                        "expr": "snode_unmap_latency_ticks{cluster=~\"$cluster\",snode=~\"$node\"}",
                         "legendFormat": "__auto",
                         "range": true,
                         "refId": "A"
                     }
                 ],
-                "title": "lvol_unmap_latency_ticks",
+                "title": "snode_unmap_latency_ticks",
                 "type": "timeseries"
             },
             {
                 "datasource": {
                     "type": "prometheus",
                     "uid": "PBFA97CFB590B2093"
                 },
@@ -1893,15 +1918,15 @@
                     },
                     "overrides": []
                 },
                 "gridPos": {
                     "h": 7,
                     "w": 7,
                     "x": 7,
-                    "y": 49
+                    "y": 48
                 },
                 "id": 17,
                 "options": {
                     "legend": {
                         "calcs": [],
                         "displayMode": "list",
                         "placement": "bottom",
@@ -1914,22 +1939,22 @@
                 },
                 "targets": [
                     {
                         "datasource": {
                             "type": "prometheus",
                             "uid": "PBFA97CFB590B2093"
                         },
-                        "editorMode": "builder",
-                        "expr": "lvol_unmap_bytes_ps",
+                        "editorMode": "code",
+                        "expr": "snode_unmap_bytes_ps{cluster=~\"$cluster\",snode=~\"$node\"}",
                         "legendFormat": "__auto",
                         "range": true,
                         "refId": "A"
                     }
                 ],
-                "title": "lvol_unmap_bytes_ps",
+                "title": "snode_unmap_bytes_ps",
                 "type": "timeseries"
             },
             {
                 "datasource": {
                     "type": "prometheus",
                     "uid": "PBFA97CFB590B2093"
                 },
@@ -1987,15 +2012,15 @@
                     },
                     "overrides": []
                 },
                 "gridPos": {
                     "h": 7,
                     "w": 7,
                     "x": 14,
-                    "y": 49
+                    "y": 48
                 },
                 "id": 20,
                 "options": {
                     "legend": {
                         "calcs": [],
                         "displayMode": "list",
                         "placement": "bottom",
@@ -2008,22 +2033,22 @@
                 },
                 "targets": [
                     {
                         "datasource": {
                             "type": "prometheus",
                             "uid": "PBFA97CFB590B2093"
                         },
-                        "editorMode": "builder",
-                        "expr": "lvol_unmap_latency_ps",
+                        "editorMode": "code",
+                        "expr": "snode_unmap_latency_ps{cluster=~\"$cluster\",snode=~\"$node\"}",
                         "legendFormat": "__auto",
                         "range": true,
                         "refId": "A"
                     }
                 ],
-                "title": "lvol_unmap_latency_ps",
+                "title": "snode_unmap_latency_ps",
                 "type": "timeseries"
             },
             {
                 "datasource": {
                     "type": "prometheus",
                     "uid": "PBFA97CFB590B2093"
                 },
@@ -2081,15 +2106,15 @@
                         {
                             "__systemRef": "hideSeriesFrom",
                             "matcher": {
                                 "id": "byNames",
                                 "options": {
                                     "mode": "exclude",
                                     "names": [
-                                        "{__name__=\"lvol_unmap_io_ps\", cluster=\"c3663938-6610-44d5-9897-d7bfa60a43e1\", exported_job=\"collector\", instance=\"192.168.178.52:9091\", job=\"metricsgateway\"}"
+                                        "{__name__=\"snode_unmap_io_ps\", cluster=\"c3663938-6610-44d5-9897-d7bfa60a43e1\", exported_job=\"collector\", instance=\"192.168.178.52:9091\", job=\"metricsgateway\"}"
                                     ],
                                     "prefix": "All except:",
                                     "readOnly": true
                                 }
                             },
                             "properties": [
                                 {
@@ -2104,15 +2129,15 @@
                         }
                     ]
                 },
                 "gridPos": {
                     "h": 7,
                     "w": 7,
                     "x": 0,
-                    "y": 56
+                    "y": 55
                 },
                 "id": 19,
                 "options": {
                     "legend": {
                         "calcs": [],
                         "displayMode": "list",
                         "placement": "bottom",
@@ -2125,22 +2150,22 @@
                 },
                 "targets": [
                     {
                         "datasource": {
                             "type": "prometheus",
                             "uid": "PBFA97CFB590B2093"
                         },
-                        "editorMode": "builder",
-                        "expr": "lvol_unmap_io_ps",
+                        "editorMode": "code",
+                        "expr": "snode_unmap_io_ps{cluster=~\"$cluster\",snode=~\"$node\"}",
                         "legendFormat": "__auto",
                         "range": true,
                         "refId": "A"
                     }
                 ],
-                "title": "lvol_unmap_io_ps",
+                "title": "snode_unmap_io_ps",
                 "type": "timeseries"
             },
             {
                 "datasource": {
                     "type": "prometheus",
                     "uid": "PBFA97CFB590B2093"
                 },
@@ -2196,15 +2221,15 @@
                     },
                     "overrides": []
                 },
                 "gridPos": {
                     "h": 7,
                     "w": 7,
                     "x": 7,
-                    "y": 56
+                    "y": 55
                 },
                 "id": 18,
                 "options": {
                     "legend": {
                         "calcs": [],
                         "displayMode": "list",
                         "placement": "bottom",
@@ -2217,22 +2242,22 @@
                 },
                 "targets": [
                     {
                         "datasource": {
                             "type": "prometheus",
                             "uid": "PBFA97CFB590B2093"
                         },
-                        "editorMode": "builder",
-                        "expr": "lvol_unmap_io",
+                        "editorMode": "code",
+                        "expr": "snode_unmap_io{cluster=~\"$cluster\",snode=~\"$node\"}",
                         "legendFormat": "__auto",
                         "range": true,
                         "refId": "A"
                     }
                 ],
-                "title": "lvol_unmap_io",
+                "title": "snode_unmap_io",
                 "type": "timeseries"
             },
             {
                 "datasource": {
                     "type": "prometheus",
                     "uid": "PBFA97CFB590B2093"
                 },
@@ -2281,23 +2306,23 @@
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
                     "h": 7,
                     "w": 7,
                     "x": 14,
-                    "y": 56
+                    "y": 55
                 },
                 "id": 16,
                 "options": {
                     "legend": {
                         "calcs": [],
                         "displayMode": "list",
                         "placement": "bottom",
@@ -2310,37 +2335,102 @@
                 },
                 "targets": [
                     {
                         "datasource": {
                             "type": "prometheus",
                             "uid": "PBFA97CFB590B2093"
                         },
-                        "editorMode": "builder",
-                        "expr": "lvol_unmap_bytes",
+                        "editorMode": "code",
+                        "expr": "snode_unmap_bytes{cluster=~\"$cluster\",snode=~\"$node\"}",
                         "legendFormat": "__auto",
                         "range": true,
                         "refId": "A"
                     }
                 ],
-                "title": "lvol_unmap_bytes",
+                "title": "snode_unmap_bytes",
                 "type": "timeseries"
             }
         ],
-        "refresh": "",
+        "refresh": "5s",
         "schemaVersion": 38,
         "style": "dark",
         "tags": [],
         "templating": {
-            "list": []
+            "list": [
+                {
+                    "allValue": ".*",
+                    "current": {
+                        "selected": true,
+                        "text": [
+                            "All"
+                        ],
+                        "value": [
+                            "$__all"
+                        ]
+                    },
+                    "datasource": {
+                        "type": "prometheus",
+                        "uid": "PBFA97CFB590B2093"
+                    },
+                    "definition": "label_values(cluster)",
+                    "hide": 0,
+                    "includeAll": true,
+                    "label": "cluster",
+                    "multi": true,
+                    "name": "cluster",
+                    "options": [],
+                    "query": {
+                        "query": "label_values(cluster)",
+                        "refId": "PrometheusVariableQueryEditor-VariableQuery"
+                    },
+                    "refresh": 1,
+                    "regex": "",
+                    "skipUrlSync": false,
+                    "sort": 0,
+                    "type": "query"
+                },
+                {
+                    "allValue": ".*",
+                    "current": {
+                        "selected": true,
+                        "text": [
+                            "All"
+                        ],
+                        "value": [
+                            "$__all"
+                        ]
+                    },
+                    "datasource": {
+                        "type": "prometheus",
+                        "uid": "PBFA97CFB590B2093"
+                    },
+                    "definition": "query_result(device_size_total{cluster=~\"$cluster\"})",
+                    "hide": 0,
+                    "includeAll": true,
+                    "label": "node",
+                    "multi": true,
+                    "name": "node",
+                    "options": [],
+                    "query": {
+                        "query": "query_result(device_size_total{cluster=~\"$cluster\"})",
+                        "refId": "PrometheusVariableQueryEditor-VariableQuery"
+                    },
+                    "refresh": 2,
+                    "regex": ".*snode=\"(.*?)\".*",
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
-        "title": "LvolsDashboard",
-        "uid": "d56e0ae7-48d5-481d-a2ea-3192da4d9e19",
+        "title": "NodesDashboard",
+        "uid": "d56e0ae7-48d5-481d-a2ea-3192da4d9e37",
         "version": 5,
         "weekStart": ""
     }
 }
```

## Comparing `sbcli_dev-2.8.3/simplyblock_core/scripts/dashboards/devices.json` & `sbcli_dev-2.8.4/simplyblock_core/scripts/dashboards/pools.json`

 * *Files 12% similar despite different names*

### Pretty-printed

 * *Similarity: 0.9679875215399203%*

 * *Differences: {"'dashboard'": "{'panels': {1: {'fieldConfig': {'defaults': {'unit': 'decbytes'}}, 'targets': {0: "*

 * *                "{'editorMode': 'code', 'expr': "*

 * *                '\'pool_size_total{cluster="$cluster",pool="$pool"}\'}}, \'title\': '*

 * *                "'pool_size_total'}, 2: {'fieldConfig': {'defaults': {'unit': 'decbytes'}}, "*

 * *                "'targets': {0: {'editorMode': 'code', 'expr': "*

 * *                '\'pool_size_free{cluster="$cluster",pool="$pool"}\'}}, \'title\': '*

 * *                "'pool_size_fre […]*

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
@@ -115,22 +115,22 @@
                 },
                 "targets": [
                     {
                         "datasource": {
                             "type": "prometheus",
                             "uid": "PBFA97CFB590B2093"
                         },
-                        "editorMode": "builder",
-                        "expr": "device_size_total",
+                        "editorMode": "code",
+                        "expr": "pool_size_total{cluster=\"$cluster\",pool=\"$pool\"}",
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
@@ -208,22 +208,22 @@
                 },
                 "targets": [
                     {
                         "datasource": {
                             "type": "prometheus",
                             "uid": "PBFA97CFB590B2093"
                         },
-                        "editorMode": "builder",
-                        "expr": "device_size_free",
+                        "editorMode": "code",
+                        "expr": "pool_size_free{cluster=\"$cluster\",pool=\"$pool\"}",
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
@@ -301,22 +301,22 @@
                 },
                 "targets": [
                     {
                         "datasource": {
                             "type": "prometheus",
                             "uid": "PBFA97CFB590B2093"
                         },
-                        "editorMode": "builder",
-                        "expr": "device_size_used",
+                        "editorMode": "code",
+                        "expr": "pool_size_used{cluster=\"$cluster\",pool=\"$pool\"}",
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
@@ -394,22 +394,22 @@
                 },
                 "targets": [
                     {
                         "datasource": {
                             "type": "prometheus",
                             "uid": "PBFA97CFB590B2093"
                         },
-                        "editorMode": "builder",
-                        "expr": "device_size_prov",
+                        "editorMode": "code",
+                        "expr": "pool_size_prov{cluster=\"$cluster\",pool=\"$pool\"}",
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
@@ -487,22 +487,22 @@
                 },
                 "targets": [
                     {
                         "datasource": {
                             "type": "prometheus",
                             "uid": "PBFA97CFB590B2093"
                         },
-                        "editorMode": "builder",
-                        "expr": "device_size_prov_util",
+                        "editorMode": "code",
+                        "expr": "pool_size_prov_util{cluster=\"$cluster\",pool=\"$pool\"}",
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
@@ -580,22 +580,22 @@
                 },
                 "targets": [
                     {
                         "datasource": {
                             "type": "prometheus",
                             "uid": "PBFA97CFB590B2093"
                         },
-                        "editorMode": "builder",
-                        "expr": "device_size_util",
+                        "editorMode": "code",
+                        "expr": "pool_size_util{cluster=\"$cluster\",pool=\"$pool\"}",
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
@@ -686,22 +686,22 @@
                 },
                 "targets": [
                     {
                         "datasource": {
                             "type": "prometheus",
                             "uid": "PBFA97CFB590B2093"
                         },
-                        "editorMode": "builder",
-                        "expr": "device_write_bytes",
+                        "editorMode": "code",
+                        "expr": "pool_write_bytes{cluster=\"$cluster\",pool=\"$pool\"}",
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
@@ -779,16 +779,16 @@
                 },
                 "targets": [
                     {
                         "datasource": {
                             "type": "prometheus",
                             "uid": "PBFA97CFB590B2093"
                         },
-                        "editorMode": "builder",
-                        "expr": "device_write_bytes_ps",
+                        "editorMode": "code",
+                        "expr": "pool_write_bytes_ps{cluster=\"$cluster\",pool=\"$pool\"}",
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
@@ -872,22 +871,22 @@
                 },
                 "targets": [
                     {
                         "datasource": {
                             "type": "prometheus",
                             "uid": "PBFA97CFB590B2093"
                         },
-                        "editorMode": "builder",
-                        "expr": "device_write_latency_ps / 1000",
+                        "editorMode": "code",
+                        "expr": "pool_write_latency_ticks{cluster=\"$cluster\",pool=\"$pool\"}",
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
@@ -964,22 +963,22 @@
                 },
                 "targets": [
                     {
                         "datasource": {
                             "type": "prometheus",
                             "uid": "PBFA97CFB590B2093"
                         },
-                        "editorMode": "builder",
-                        "expr": "device_write_io",
+                        "editorMode": "code",
+                        "expr": "pool_write_io{cluster=\"$cluster\",pool=\"$pool\"}",
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
@@ -1056,16 +1055,16 @@
                 },
                 "targets": [
                     {
                         "datasource": {
                             "type": "prometheus",
                             "uid": "PBFA97CFB590B2093"
                         },
-                        "editorMode": "builder",
-                        "expr": "device_write_io_ps",
+                        "editorMode": "code",
+                        "expr": "pool_write_io_ps{cluster=\"$cluster\",pool=\"$pool\"}",
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
@@ -1148,22 +1148,22 @@
                 },
                 "targets": [
                     {
                         "datasource": {
                             "type": "prometheus",
                             "uid": "PBFA97CFB590B2093"
                         },
-                        "editorMode": "builder",
-                        "expr": "device_write_latency_ticks",
+                        "editorMode": "code",
+                        "expr": "pool_write_latency_ps{cluster=\"$cluster\",pool=\"$pool\"} / 1000",
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
@@ -1254,22 +1254,22 @@
                 },
                 "targets": [
                     {
                         "datasource": {
                             "type": "prometheus",
                             "uid": "PBFA97CFB590B2093"
                         },
-                        "editorMode": "builder",
-                        "expr": "device_read_bytes",
+                        "editorMode": "code",
+                        "expr": "pool_read_bytes{cluster=\"$cluster\",pool=\"$pool\"}",
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
@@ -1347,16 +1347,16 @@
                 },
                 "targets": [
                     {
                         "datasource": {
                             "type": "prometheus",
                             "uid": "PBFA97CFB590B2093"
                         },
-                        "editorMode": "builder",
-                        "expr": "device_read_bytes_ps",
+                        "editorMode": "code",
+                        "expr": "pool_read_bytes_ps{cluster=\"$cluster\",pool=\"$pool\"}",
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
@@ -1440,22 +1439,22 @@
                 },
                 "targets": [
                     {
                         "datasource": {
                             "type": "prometheus",
                             "uid": "PBFA97CFB590B2093"
                         },
-                        "editorMode": "builder",
-                        "expr": "device_read_latency_ps",
+                        "editorMode": "code",
+                        "expr": "pool_read_latency_ps{cluster=\"$cluster\",pool=\"$pool\"}",
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
@@ -1532,22 +1531,22 @@
                 },
                 "targets": [
                     {
                         "datasource": {
                             "type": "prometheus",
                             "uid": "PBFA97CFB590B2093"
                         },
-                        "editorMode": "builder",
-                        "expr": "device_read_io",
+                        "editorMode": "code",
+                        "expr": "pool_read_io{cluster=\"$cluster\",pool=\"$pool\"}",
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
@@ -1624,16 +1623,16 @@
                 },
                 "targets": [
                     {
                         "datasource": {
                             "type": "prometheus",
                             "uid": "PBFA97CFB590B2093"
                         },
-                        "editorMode": "builder",
-                        "expr": "device_read_io_ps",
+                        "editorMode": "code",
+                        "expr": "pool_read_io_ps{cluster=\"$cluster\",pool=\"$pool\"}",
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
@@ -1716,22 +1715,22 @@
                 },
                 "targets": [
                     {
                         "datasource": {
                             "type": "prometheus",
                             "uid": "PBFA97CFB590B2093"
                         },
-                        "editorMode": "builder",
-                        "expr": "device_read_latency_ticks",
+                        "editorMode": "code",
+                        "expr": "pool_read_latency_ticks{cluster=\"$cluster\",pool=\"$pool\"}",
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
@@ -1821,22 +1820,22 @@
                 },
                 "targets": [
                     {
                         "datasource": {
                             "type": "prometheus",
                             "uid": "PBFA97CFB590B2093"
                         },
-                        "editorMode": "builder",
-                        "expr": "device_unmap_latency_ticks",
+                        "editorMode": "code",
+                        "expr": "pool_unmap_latency_ticks{cluster=\"$cluster\",pool=\"$pool\"}",
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
@@ -1914,22 +1913,22 @@
                 },
                 "targets": [
                     {
                         "datasource": {
                             "type": "prometheus",
                             "uid": "PBFA97CFB590B2093"
                         },
-                        "editorMode": "builder",
-                        "expr": "device_unmap_bytes_ps",
+                        "editorMode": "code",
+                        "expr": "pool_unmap_bytes_ps{cluster=\"$cluster\",pool=\"$pool\"}",
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
@@ -2008,22 +2006,22 @@
                 },
                 "targets": [
                     {
                         "datasource": {
                             "type": "prometheus",
                             "uid": "PBFA97CFB590B2093"
                         },
-                        "editorMode": "builder",
-                        "expr": "device_unmap_latency_ps",
+                        "editorMode": "code",
+                        "expr": "pool_unmap_latency_ps{cluster=\"$cluster\",pool=\"$pool\"}",
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
@@ -2125,22 +2123,22 @@
                 },
                 "targets": [
                     {
                         "datasource": {
                             "type": "prometheus",
                             "uid": "PBFA97CFB590B2093"
                         },
-                        "editorMode": "builder",
-                        "expr": "device_unmap_io_ps",
+                        "editorMode": "code",
+                        "expr": "pool_unmap_io_ps{cluster=\"$cluster\",pool=\"$pool\"}",
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
@@ -2217,22 +2215,22 @@
                 },
                 "targets": [
                     {
                         "datasource": {
                             "type": "prometheus",
                             "uid": "PBFA97CFB590B2093"
                         },
-                        "editorMode": "builder",
-                        "expr": "device_unmap_io",
+                        "editorMode": "code",
+                        "expr": "pool_unmap_io{cluster=\"$cluster\",pool=\"$pool\"}",
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
@@ -2310,37 +2308,94 @@
                 },
                 "targets": [
                     {
                         "datasource": {
                             "type": "prometheus",
                             "uid": "PBFA97CFB590B2093"
                         },
-                        "editorMode": "builder",
-                        "expr": "device_unmap_bytes",
+                        "editorMode": "code",
+                        "expr": "pool_unmap_bytes{cluster=\"$cluster\",pool=\"$pool\"}",
                         "legendFormat": "__auto",
                         "range": true,
                         "refId": "A"
                     }
                 ],
-                "title": "device_unmap_bytes",
+                "title": "pool_unmap_bytes",
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
+                    "allValue": ".*",
+                    "current": {
+                        "selected": true,
+                        "text": [
+                            "All"
+                        ],
+                        "value": [
+                            "$__all"
+                        ]
+                    },
+                    "definition": "label_values(cluster)",
+                    "hide": 0,
+                    "includeAll": true,
+                    "label": "cluster",
+                    "multi": true,
+                    "name": "cluster",
+                    "options": [],
+                    "query": {
+                        "query": "label_values(cluster)",
+                        "refId": "PrometheusVariableQueryEditor-VariableQuery"
+                    },
+                    "refresh": 1,
+                    "regex": "",
+                    "skipUrlSync": false,
+                    "sort": 0,
+                    "type": "query"
+                },
+                {
+                    "allValue": ".*",
+                    "current": {
+                        "selected": true,
+                        "text": [
+                            "All"
+                        ],
+                        "value": [
+                            "$__all"
+                        ]
+                    },
+                    "definition": "query_result(pool_size_total{cluster=~\"$cluster\"})",
+                    "hide": 0,
+                    "includeAll": true,
+                    "label": "pool",
+                    "multi": true,
+                    "name": "pool",
+                    "options": [],
+                    "query": {
+                        "query": "query_result(pool_size_total{cluster=~\"$cluster\"})",
+                        "refId": "PrometheusVariableQueryEditor-VariableQuery"
+                    },
+                    "refresh": 1,
+                    "regex": ".*pool=\"(.*?)\".*",
+                    "skipUrlSync": false,
+                    "sort": 0,
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
-        "title": "DevicesDashboard",
-        "uid": "d56e0ae7-48d5-481d-a2ea-3192da4d9e38",
+        "title": "PoolsDashboard",
+        "uid": "d56e0ae7-48d5-481d-a2ea-3192da4d9e40",
         "version": 5,
         "weekStart": ""
     }
 }
```

## Comparing `sbcli_dev-2.8.3/simplyblock_core/scripts/dashboards/pools.json` & `sbcli_dev-2.8.4/simplyblock_core/scripts/dashboards/devices.json`

 * *Files 21% similar despite different names*

### Pretty-printed

 * *Similarity: 0.9664832807470252%*

 * *Differences: {"'dashboard'": "{'panels': {1: {'fieldConfig': {'defaults': {'unit': 'bytes'}}, 'targets': {0: "*

 * *                "{'editorMode': 'code', 'expr': "*

 * *                '\'device_size_total{cluster=~"$cluster",snode=~"$node",device=~"$device"}\'}}, '*

 * *                "'title': 'device_size_total'}, 2: {'fieldConfig': {'defaults': {'unit': "*

 * *                "'bytes'}}, 'targets': {0: {'editorMode': 'code', 'expr': "*

 * *                '\'device_size_free{cluster=~"$cluster",snode=~"$node",device=~"$device"}\'}}, '*

 * *   […]*

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
@@ -115,22 +115,22 @@
                 },
                 "targets": [
                     {
                         "datasource": {
                             "type": "prometheus",
                             "uid": "PBFA97CFB590B2093"
                         },
-                        "editorMode": "builder",
-                        "expr": "pool_size_total",
+                        "editorMode": "code",
+                        "expr": "device_size_total{cluster=~\"$cluster\",snode=~\"$node\",device=~\"$device\"}",
                         "legendFormat": "__auto",
                         "range": true,
                         "refId": "A"
                     }
                 ],
-                "title": "pool_size_total",
+                "title": "device_size_total",
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
@@ -208,22 +208,22 @@
                 },
                 "targets": [
                     {
                         "datasource": {
                             "type": "prometheus",
                             "uid": "PBFA97CFB590B2093"
                         },
-                        "editorMode": "builder",
-                        "expr": "pool_size_free",
+                        "editorMode": "code",
+                        "expr": "device_size_free{cluster=~\"$cluster\",snode=~\"$node\",device=~\"$device\"}",
                         "legendFormat": "__auto",
                         "range": true,
                         "refId": "A"
                     }
                 ],
-                "title": "pool_size_free",
+                "title": "device_size_free",
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
-                        "unit": "decbytes"
+                        "unit": "bytes"
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
@@ -301,22 +301,22 @@
                 },
                 "targets": [
                     {
                         "datasource": {
                             "type": "prometheus",
                             "uid": "PBFA97CFB590B2093"
                         },
-                        "editorMode": "builder",
-                        "expr": "pool_size_used",
+                        "editorMode": "code",
+                        "expr": "device_size_used{cluster=~\"$cluster\",snode=~\"$node\",device=~\"$device\"}",
                         "legendFormat": "__auto",
                         "range": true,
                         "refId": "A"
                     }
                 ],
-                "title": "pool_size_used",
+                "title": "device_size_used",
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
@@ -394,22 +394,22 @@
                 },
                 "targets": [
                     {
                         "datasource": {
                             "type": "prometheus",
                             "uid": "PBFA97CFB590B2093"
                         },
-                        "editorMode": "builder",
-                        "expr": "pool_size_prov",
+                        "editorMode": "code",
+                        "expr": "device_size_prov{cluster=~\"$cluster\",snode=~\"$node\",device=~\"$device\"}",
                         "legendFormat": "__auto",
                         "range": true,
                         "refId": "A"
                     }
                 ],
-                "title": "pool_size_prov",
+                "title": "device_size_prov",
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
@@ -487,22 +487,22 @@
                 },
                 "targets": [
                     {
                         "datasource": {
                             "type": "prometheus",
                             "uid": "PBFA97CFB590B2093"
                         },
-                        "editorMode": "builder",
-                        "expr": "pool_size_prov_util",
+                        "editorMode": "code",
+                        "expr": "device_size_prov_util{cluster=~\"$cluster\",snode=~\"$node\",device=~\"$device\"}",
                         "legendFormat": "__auto",
                         "range": true,
                         "refId": "A"
                     }
                 ],
-                "title": "pool_size_prov_util",
+                "title": "device_size_prov_util",
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
-                        "unit": "decbytes"
+                        "unit": "percent"
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
@@ -580,22 +580,22 @@
                 },
                 "targets": [
                     {
                         "datasource": {
                             "type": "prometheus",
                             "uid": "PBFA97CFB590B2093"
                         },
-                        "editorMode": "builder",
-                        "expr": "pool_size_util",
+                        "editorMode": "code",
+                        "expr": "device_size_util{cluster=~\"$cluster\",snode=~\"$node\",device=~\"$device\"}",
                         "legendFormat": "__auto",
                         "range": true,
                         "refId": "A"
                     }
                 ],
-                "title": "pool_size_util",
+                "title": "device_size_util",
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
-                        "unit": "decbytes"
+                        "unit": "bytes"
                     },
                     "overrides": []
                 },
                 "gridPos": {
                     "h": 8,
                     "w": 7,
                     "x": 0,
@@ -686,22 +686,22 @@
                 },
                 "targets": [
                     {
                         "datasource": {
                             "type": "prometheus",
                             "uid": "PBFA97CFB590B2093"
                         },
-                        "editorMode": "builder",
-                        "expr": "pool_write_bytes",
+                        "editorMode": "code",
+                        "expr": "device_write_bytes{cluster=~\"$cluster\",snode=~\"$node\",device=~\"$device\"}",
                         "legendFormat": "__auto",
                         "range": true,
                         "refId": "A"
                     }
                 ],
-                "title": "pool_write_bytes",
+                "title": "device_write_bytes",
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
-                        "unit": "Bps"
+                        "unit": "bytes"
                     },
                     "overrides": []
                 },
                 "gridPos": {
                     "h": 8,
                     "w": 7,
                     "x": 7,
@@ -779,29 +779,30 @@
                 },
                 "targets": [
                     {
                         "datasource": {
                             "type": "prometheus",
                             "uid": "PBFA97CFB590B2093"
                         },
-                        "editorMode": "builder",
-                        "expr": "pool_write_bytes_ps",
+                        "editorMode": "code",
+                        "expr": "device_write_bytes_ps{cluster=~\"$cluster\",snode=~\"$node\",device=~\"$device\"}",
                         "legendFormat": "__auto",
                         "range": true,
                         "refId": "A"
                     }
                 ],
                 "title": "write_speed",
                 "type": "timeseries"
             },
             {
                 "datasource": {
                     "type": "prometheus",
                     "uid": "PBFA97CFB590B2093"
                 },
+                "description": "",
                 "fieldConfig": {
                     "defaults": {
                         "color": {
                             "mode": "palette-classic"
                         },
                         "custom": {
                             "axisCenteredZero": false,
@@ -842,25 +843,26 @@
                                     "value": null
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
-                    "w": 7,
+                    "w": 8,
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
@@ -871,22 +873,22 @@
                 },
                 "targets": [
                     {
                         "datasource": {
                             "type": "prometheus",
                             "uid": "PBFA97CFB590B2093"
                         },
-                        "editorMode": "builder",
-                        "expr": "pool_write_latency_ticks",
+                        "editorMode": "code",
+                        "expr": "device_write_latency_ps{cluster=~\"$cluster\",snode=~\"$node\",device=~\"$device\"} / 1000",
                         "legendFormat": "__auto",
                         "range": true,
                         "refId": "A"
                     }
                 ],
-                "title": "pool_wite_latency_ticks",
+                "title": "device_write_latency_ps",
                 "type": "timeseries"
             },
             {
                 "datasource": {
                     "type": "prometheus",
                     "uid": "PBFA97CFB590B2093"
                 },
@@ -963,22 +965,22 @@
                 },
                 "targets": [
                     {
                         "datasource": {
                             "type": "prometheus",
                             "uid": "PBFA97CFB590B2093"
                         },
-                        "editorMode": "builder",
-                        "expr": "pool_write_io",
+                        "editorMode": "code",
+                        "expr": "device_write_io{cluster=~\"$cluster\",snode=~\"$node\",device=~\"$device\"}",
                         "legendFormat": "__auto",
                         "range": true,
                         "refId": "A"
                     }
                 ],
-                "title": "pool_write_io",
+                "title": "device_write_io",
                 "type": "timeseries"
             },
             {
                 "datasource": {
                     "type": "prometheus",
                     "uid": "PBFA97CFB590B2093"
                 },
@@ -1055,16 +1057,16 @@
                 },
                 "targets": [
                     {
                         "datasource": {
                             "type": "prometheus",
                             "uid": "PBFA97CFB590B2093"
                         },
-                        "editorMode": "builder",
-                        "expr": "pool_write_io_ps",
+                        "editorMode": "code",
+                        "expr": "device_write_io_ps{cluster=~\"$cluster\",snode=~\"$node\",device=~\"$device\"}",
                         "legendFormat": "__auto",
                         "range": true,
                         "refId": "A"
                     }
                 ],
                 "title": "write_iops",
                 "type": "timeseries"
@@ -1118,26 +1120,25 @@
                                     "value": null
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
                     "h": 8,
-                    "w": 7,
+                    "w": 8,
                     "x": 14,
                     "y": 24
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
@@ -1148,22 +1149,22 @@
                 },
                 "targets": [
                     {
                         "datasource": {
                             "type": "prometheus",
                             "uid": "PBFA97CFB590B2093"
                         },
-                        "editorMode": "builder",
-                        "expr": "pool_write_latency_ps / 1000",
+                        "editorMode": "code",
+                        "expr": "device_write_latency_ticks{cluster=~\"$cluster\",snode=~\"$node\",device=~\"$device\"}",
                         "legendFormat": "__auto",
                         "range": true,
                         "refId": "A"
                     }
                 ],
-                "title": "pool_write_latency_ps",
+                "title": "device_wite_latency_ticks",
                 "type": "timeseries"
             },
             {
                 "collapsed": false,
                 "gridPos": {
                     "h": 1,
                     "w": 24,
@@ -1225,15 +1226,15 @@
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
@@ -1254,22 +1255,22 @@
                 },
                 "targets": [
                     {
                         "datasource": {
                             "type": "prometheus",
                             "uid": "PBFA97CFB590B2093"
                         },
-                        "editorMode": "builder",
-                        "expr": "pool_read_bytes",
+                        "editorMode": "code",
+                        "expr": "device_read_bytes{cluster=~\"$cluster\",snode=~\"$node\",device=~\"$device\"}",
                         "legendFormat": "__auto",
                         "range": true,
                         "refId": "A"
                     }
                 ],
-                "title": "pool_read_bytes",
+                "title": "device_read_bytes",
                 "type": "timeseries"
             },
             {
                 "datasource": {
                     "type": "prometheus",
                     "uid": "PBFA97CFB590B2093"
                 },
@@ -1318,15 +1319,15 @@
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
@@ -1347,16 +1348,16 @@
                 },
                 "targets": [
                     {
                         "datasource": {
                             "type": "prometheus",
                             "uid": "PBFA97CFB590B2093"
                         },
-                        "editorMode": "builder",
-                        "expr": "pool_read_bytes_ps",
+                        "editorMode": "code",
+                        "expr": "device_read_bytes_ps{cluster=~\"$cluster\",snode=~\"$node\",device=~\"$device\"}",
                         "legendFormat": "__auto",
                         "range": true,
                         "refId": "A"
                     }
                 ],
                 "title": "read_speed",
                 "type": "timeseries"
@@ -1410,21 +1411,22 @@
                                     "value": null
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
-                    "w": 7,
+                    "w": 8,
                     "x": 14,
                     "y": 33
                 },
                 "id": 5,
                 "options": {
                     "legend": {
                         "calcs": [],
@@ -1439,22 +1441,22 @@
                 },
                 "targets": [
                     {
                         "datasource": {
                             "type": "prometheus",
                             "uid": "PBFA97CFB590B2093"
                         },
-                        "editorMode": "builder",
-                        "expr": "pool_read_latency_ps",
+                        "editorMode": "code",
+                        "expr": "device_read_latency_ps{cluster=~\"$cluster\",snode=~\"$node\",device=~\"$device\"}",
                         "legendFormat": "__auto",
                         "range": true,
                         "refId": "A"
                     }
                 ],
-                "title": "pool_read_latency_ps",
+                "title": "device_read_latency_ps",
                 "type": "timeseries"
             },
             {
                 "datasource": {
                     "type": "prometheus",
                     "uid": "PBFA97CFB590B2093"
                 },
@@ -1531,22 +1533,22 @@
                 },
                 "targets": [
                     {
                         "datasource": {
                             "type": "prometheus",
                             "uid": "PBFA97CFB590B2093"
                         },
-                        "editorMode": "builder",
-                        "expr": "pool_read_io",
+                        "editorMode": "code",
+                        "expr": "device_read_io{cluster=~\"$cluster\",snode=~\"$node\",device=~\"$device\"}",
                         "legendFormat": "__auto",
                         "range": true,
                         "refId": "A"
                     }
                 ],
-                "title": "pool_read_io",
+                "title": "device_read_io",
                 "type": "timeseries"
             },
             {
                 "datasource": {
                     "type": "prometheus",
                     "uid": "PBFA97CFB590B2093"
                 },
@@ -1623,16 +1625,16 @@
                 },
                 "targets": [
                     {
                         "datasource": {
                             "type": "prometheus",
                             "uid": "PBFA97CFB590B2093"
                         },
-                        "editorMode": "builder",
-                        "expr": "pool_read_io_ps",
+                        "editorMode": "code",
+                        "expr": "device_read_io_ps{cluster=~\"$cluster\",snode=~\"$node\",device=~\"$device\"}",
                         "legendFormat": "__auto",
                         "range": true,
                         "refId": "A"
                     }
                 ],
                 "title": "read_iops",
                 "type": "timeseries"
@@ -1692,15 +1694,15 @@
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
                     "y": 41
                 },
                 "id": 6,
                 "options": {
                     "legend": {
                         "calcs": [],
@@ -1715,22 +1717,22 @@
                 },
                 "targets": [
                     {
                         "datasource": {
                             "type": "prometheus",
                             "uid": "PBFA97CFB590B2093"
                         },
-                        "editorMode": "builder",
-                        "expr": "pool_read_latency_ticks",
+                        "editorMode": "code",
+                        "expr": "device_read_latency_ticks{cluster=~\"$cluster\",snode=~\"$node\",device=~\"$device\"}",
                         "legendFormat": "__auto",
                         "range": true,
                         "refId": "A"
                     }
                 ],
-                "title": "pool_read_latency_ticks",
+                "title": "device_read_latency_ticks",
                 "type": "timeseries"
             },
             {
                 "collapsed": false,
                 "gridPos": {
                     "h": 1,
                     "w": 24,
@@ -1820,22 +1822,22 @@
                 },
                 "targets": [
                     {
                         "datasource": {
                             "type": "prometheus",
                             "uid": "PBFA97CFB590B2093"
                         },
-                        "editorMode": "builder",
-                        "expr": "pool_unmap_latency_ticks",
+                        "editorMode": "code",
+                        "expr": "device_unmap_latency_ticks{cluster=~\"$cluster\",snode=~\"$node\",device=~\"$device\"}",
                         "legendFormat": "__auto",
                         "range": true,
                         "refId": "A"
                     }
                 ],
-                "title": "pool_unmap_latency_ticks",
+                "title": "device_unmap_latency_ticks",
                 "type": "timeseries"
             },
             {
                 "datasource": {
                     "type": "prometheus",
                     "uid": "PBFA97CFB590B2093"
                 },
@@ -1884,15 +1886,15 @@
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
@@ -1913,22 +1915,22 @@
                 },
                 "targets": [
                     {
                         "datasource": {
                             "type": "prometheus",
                             "uid": "PBFA97CFB590B2093"
                         },
-                        "editorMode": "builder",
-                        "expr": "pool_unmap_bytes_ps",
+                        "editorMode": "code",
+                        "expr": "device_unmap_bytes_ps{cluster=~\"$cluster\",snode=~\"$node\",device=~\"$device\"}",
                         "legendFormat": "__auto",
                         "range": true,
                         "refId": "A"
                     }
                 ],
-                "title": "pool_unmap_bytes_ps",
+                "title": "device_unmap_bytes_ps",
                 "type": "timeseries"
             },
             {
                 "datasource": {
                     "type": "prometheus",
                     "uid": "PBFA97CFB590B2093"
                 },
@@ -1977,21 +1979,22 @@
                                     "value": null
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
-                    "w": 7,
+                    "w": 8,
                     "x": 14,
                     "y": 49
                 },
                 "id": 20,
                 "options": {
                     "legend": {
                         "calcs": [],
@@ -2006,22 +2009,22 @@
                 },
                 "targets": [
                     {
                         "datasource": {
                             "type": "prometheus",
                             "uid": "PBFA97CFB590B2093"
                         },
-                        "editorMode": "builder",
-                        "expr": "pool_unmap_latency_ps",
+                        "editorMode": "code",
+                        "expr": "device_unmap_latency_ps{cluster=~\"$cluster\",snode=~\"$node\",device=~\"$device\"}",
                         "legendFormat": "__auto",
                         "range": true,
                         "refId": "A"
                     }
                 ],
-                "title": "pool_unmap_latency_ps",
+                "title": "device_unmap_latency_ps",
                 "type": "timeseries"
             },
             {
                 "datasource": {
                     "type": "prometheus",
                     "uid": "PBFA97CFB590B2093"
                 },
@@ -2079,15 +2082,15 @@
                         {
                             "__systemRef": "hideSeriesFrom",
                             "matcher": {
                                 "id": "byNames",
                                 "options": {
                                     "mode": "exclude",
                                     "names": [
-                                        "{__name__=\"pool_unmap_io_ps\", cluster=\"c3663938-6610-44d5-9897-d7bfa60a43e1\", exported_job=\"collector\", instance=\"192.168.178.52:9091\", job=\"metricsgateway\"}"
+                                        "{__name__=\"device_unmap_io_ps\", cluster=\"c3663938-6610-44d5-9897-d7bfa60a43e1\", exported_job=\"collector\", instance=\"192.168.178.52:9091\", job=\"metricsgateway\"}"
                                     ],
                                     "prefix": "All except:",
                                     "readOnly": true
                                 }
                             },
                             "properties": [
                                 {
@@ -2123,22 +2126,22 @@
                 },
                 "targets": [
                     {
                         "datasource": {
                             "type": "prometheus",
                             "uid": "PBFA97CFB590B2093"
                         },
-                        "editorMode": "builder",
-                        "expr": "pool_unmap_io_ps",
+                        "editorMode": "code",
+                        "expr": "device_unmap_io_ps{cluster=~\"$cluster\",snode=~\"$node\",device=~\"$device\"}",
                         "legendFormat": "__auto",
                         "range": true,
                         "refId": "A"
                     }
                 ],
-                "title": "pool_unmap_io_ps",
+                "title": "device_unmap_io_ps",
                 "type": "timeseries"
             },
             {
                 "datasource": {
                     "type": "prometheus",
                     "uid": "PBFA97CFB590B2093"
                 },
@@ -2215,22 +2218,22 @@
                 },
                 "targets": [
                     {
                         "datasource": {
                             "type": "prometheus",
                             "uid": "PBFA97CFB590B2093"
                         },
-                        "editorMode": "builder",
-                        "expr": "pool_unmap_io",
+                        "editorMode": "code",
+                        "expr": "device_unmap_io{cluster=~\"$cluster\",snode=~\"$node\",device=~\"$device\"}",
                         "legendFormat": "__auto",
                         "range": true,
                         "refId": "A"
                     }
                 ],
-                "title": "pool_unmap_io",
+                "title": "device_unmap_io",
                 "type": "timeseries"
             },
             {
                 "datasource": {
                     "type": "prometheus",
                     "uid": "PBFA97CFB590B2093"
                 },
@@ -2285,15 +2288,15 @@
                         },
                         "unit": "decbytes"
                     },
                     "overrides": []
                 },
                 "gridPos": {
                     "h": 7,
-                    "w": 7,
+                    "w": 8,
                     "x": 14,
                     "y": 56
                 },
                 "id": 16,
                 "options": {
                     "legend": {
                         "calcs": [],
@@ -2308,328 +2311,128 @@
                 },
                 "targets": [
                     {
                         "datasource": {
                             "type": "prometheus",
                             "uid": "PBFA97CFB590B2093"
                         },
-                        "editorMode": "builder",
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
+                        "editorMode": "code",
+                        "expr": "device_unmap_bytes{cluster=~\"$cluster\",snode=~\"$node\",device=~\"$device\"}",
                         "legendFormat": "__auto",
                         "range": true,
                         "refId": "A"
                     }
                 ],
-                "title": "pool_record_start_time",
+                "title": "device_unmap_bytes",
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
+                    "allValue": ".*",
+                    "current": {
+                        "selected": true,
+                        "text": [
+                            "All"
+                        ],
+                        "value": [
+                            "$__all"
+                        ]
+                    },
+                    "datasource": {
+                        "type": "prometheus",
+                        "uid": "PBFA97CFB590B2093"
+                    },
+                    "definition": "label_values(cluster)",
+                    "hide": 0,
+                    "includeAll": true,
+                    "multi": true,
+                    "name": "cluster",
+                    "options": [],
+                    "query": {
+                        "query": "label_values(cluster)",
+                        "refId": "PrometheusVariableQueryEditor-VariableQuery"
+                    },
+                    "refresh": 1,
+                    "regex": "",
+                    "skipUrlSync": false,
+                    "sort": 1,
+                    "type": "query"
+                },
+                {
+                    "allValue": ".*",
+                    "current": {
+                        "selected": true,
+                        "text": [
+                            "All"
+                        ],
+                        "value": [
+                            "$__all"
+                        ]
+                    },
+                    "datasource": {
+                        "type": "prometheus",
+                        "uid": "PBFA97CFB590B2093"
+                    },
+                    "definition": "query_result(device_size_total{cluster=~\"$cluster\"})",
+                    "hide": 0,
+                    "includeAll": true,
+                    "label": "node",
+                    "multi": true,
+                    "name": "node",
+                    "options": [],
+                    "query": {
+                        "query": "query_result(device_size_total{cluster=~\"$cluster\"})",
+                        "refId": "PrometheusVariableQueryEditor-VariableQuery"
+                    },
+                    "refresh": 1,
+                    "regex": ".*snode=\"(.*?)\".*",
+                    "skipUrlSync": false,
+                    "sort": 0,
+                    "type": "query"
+                },
+                {
+                    "allValue": ".*",
+                    "current": {
+                        "selected": false,
+                        "text": "All",
+                        "value": "$__all"
+                    },
+                    "datasource": {
+                        "type": "prometheus",
+                        "uid": "PBFA97CFB590B2093"
+                    },
+                    "definition": "query_result(device_size_total{cluster=~\"$cluster\",snode=~\"$node\"})",
+                    "hide": 0,
+                    "includeAll": true,
+                    "multi": true,
+                    "name": "device",
+                    "options": [],
+                    "query": {
+                        "query": "query_result(device_size_total{cluster=~\"$cluster\",snode=~\"$node\"})",
+                        "refId": "PrometheusVariableQueryEditor-VariableQuery"
+                    },
+                    "refresh": 1,
+                    "regex": ".*device=\"(.*?)\".*",
+                    "skipUrlSync": false,
+                    "sort": 0,
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
+        "title": "DevicesDashboard",
+        "uid": "d56e0ae7-48d5-481d-a2ea-3192da4d9e38",
         "version": 5,
         "weekStart": ""
     }
 }
```

## Comparing `sbcli_dev-2.8.3/simplyblock_core/scripts/dashboards/node-exporter.json` & `sbcli_dev-2.8.4/simplyblock_core/scripts/dashboards/node-exporter.json`

 * *Files identical despite different names*

