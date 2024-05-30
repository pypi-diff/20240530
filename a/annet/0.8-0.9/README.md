# Comparing `tmp/annet-0.8.tar.gz` & `tmp/annet-0.9.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "annet-0.8.tar", last modified: Wed Apr 10 09:06:44 2024, max compression
+gzip compressed data, was "annet-0.9.tar", last modified: Wed Apr 10 14:33:35 2024, max compression
```

## Comparing `annet-0.8.tar` & `annet-0.9.tar`

### file list

```diff
@@ -1,166 +1,166 @@
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-10 09:06:44.052765 annet-0.8/
--rw-r--r--   0 runner    (1001) docker     (127)      878 2024-04-10 09:06:40.000000 annet-0.8/AUTHORS
--rw-r--r--   0 runner    (1001) docker     (127)     1079 2024-04-10 09:06:40.000000 annet-0.8/LICENSE
--rw-r--r--   0 runner    (1001) docker     (127)       25 2024-04-10 09:06:40.000000 annet-0.8/MANIFEST.in
--rw-r--r--   0 runner    (1001) docker     (127)      674 2024-04-10 09:06:44.048766 annet-0.8/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (127)     4794 2024-04-10 09:06:40.000000 annet-0.8/README.md
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-10 09:06:44.036765 annet-0.8/annet/
--rw-r--r--   0 runner    (1001) docker     (127)     2139 2024-04-10 09:06:40.000000 annet-0.8/annet/__init__.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-10 09:06:44.036765 annet-0.8/annet/adapters/
--rw-r--r--   0 runner    (1001) docker     (127)        0 2024-04-10 09:06:40.000000 annet-0.8/annet/adapters/__init__.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-10 09:06:44.036765 annet-0.8/annet/adapters/netbox/
--rw-r--r--   0 runner    (1001) docker     (127)        0 2024-04-10 09:06:40.000000 annet-0.8/annet/adapters/netbox/__init__.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-10 09:06:44.036765 annet-0.8/annet/adapters/netbox/common/
--rw-r--r--   0 runner    (1001) docker     (127)        0 2024-04-10 09:06:40.000000 annet-0.8/annet/adapters/netbox/common/__init__.py
--rw-r--r--   0 runner    (1001) docker     (127)     2483 2024-04-10 09:06:40.000000 annet-0.8/annet/adapters/netbox/common/client.py
--rw-r--r--   0 runner    (1001) docker     (127)     1771 2024-04-10 09:06:40.000000 annet-0.8/annet/adapters/netbox/common/manufacturer.py
--rw-r--r--   0 runner    (1001) docker     (127)     1731 2024-04-10 09:06:40.000000 annet-0.8/annet/adapters/netbox/common/models.py
--rw-r--r--   0 runner    (1001) docker     (127)      577 2024-04-10 09:06:40.000000 annet-0.8/annet/adapters/netbox/common/query.py
--rw-r--r--   0 runner    (1001) docker     (127)      567 2024-04-10 09:06:40.000000 annet-0.8/annet/adapters/netbox/common/status_client.py
--rw-r--r--   0 runner    (1001) docker     (127)      337 2024-04-10 09:06:40.000000 annet-0.8/annet/adapters/netbox/common/storage_opts.py
--rw-r--r--   0 runner    (1001) docker     (127)     1024 2024-04-10 09:06:40.000000 annet-0.8/annet/adapters/netbox/provider.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-10 09:06:44.036765 annet-0.8/annet/adapters/netbox/v24/
--rw-r--r--   0 runner    (1001) docker     (127)        0 2024-04-10 09:06:40.000000 annet-0.8/annet/adapters/netbox/v24/__init__.py
--rw-r--r--   0 runner    (1001) docker     (127)     1314 2024-04-10 09:06:40.000000 annet-0.8/annet/adapters/netbox/v24/api_models.py
--rw-r--r--   0 runner    (1001) docker     (127)     1497 2024-04-10 09:06:40.000000 annet-0.8/annet/adapters/netbox/v24/client.py
--rw-r--r--   0 runner    (1001) docker     (127)     5620 2024-04-10 09:06:40.000000 annet-0.8/annet/adapters/netbox/v24/storage.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-10 09:06:44.036765 annet-0.8/annet/adapters/netbox/v37/
--rw-r--r--   0 runner    (1001) docker     (127)        0 2024-04-10 09:06:40.000000 annet-0.8/annet/adapters/netbox/v37/__init__.py
--rw-r--r--   0 runner    (1001) docker     (127)      886 2024-04-10 09:06:40.000000 annet-0.8/annet/adapters/netbox/v37/api_models.py
--rw-r--r--   0 runner    (1001) docker     (127)     1668 2024-04-10 09:06:40.000000 annet-0.8/annet/adapters/netbox/v37/client.py
--rw-r--r--   0 runner    (1001) docker     (127)     4216 2024-04-10 09:06:40.000000 annet-0.8/annet/adapters/netbox/v37/storage.py
--rwxr-xr-x   0 runner    (1001) docker     (127)      725 2024-04-10 09:06:40.000000 annet-0.8/annet/annet.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-10 09:06:44.040765 annet-0.8/annet/annlib/
--rw-r--r--   0 runner    (1001) docker     (127)      252 2024-04-10 09:06:40.000000 annet-0.8/annet/annlib/__init__.py
--rw-r--r--   0 runner    (1001) docker     (127)     1043 2024-04-10 09:06:40.000000 annet-0.8/annet/annlib/command.py
--rw-r--r--   0 runner    (1001) docker     (127)     4587 2024-04-10 09:06:40.000000 annet-0.8/annet/annlib/diff.py
--rw-r--r--   0 runner    (1001) docker     (127)      287 2024-04-10 09:06:40.000000 annet-0.8/annet/annlib/errors.py
--rw-r--r--   0 runner    (1001) docker     (127)     7203 2024-04-10 09:06:40.000000 annet-0.8/annet/annlib/filter_acl.py
--rw-r--r--   0 runner    (1001) docker     (127)     3364 2024-04-10 09:06:40.000000 annet-0.8/annet/annlib/jsontools.py
--rw-r--r--   0 runner    (1001) docker     (127)    15317 2024-04-10 09:06:40.000000 annet-0.8/annet/annlib/lib.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-10 09:06:44.040765 annet-0.8/annet/annlib/netdev/
--rw-r--r--   0 runner    (1001) docker     (127)        0 2024-04-10 09:06:40.000000 annet-0.8/annet/annlib/netdev/__init__.py
--rw-r--r--   0 runner    (1001) docker     (127)     1634 2024-04-10 09:06:40.000000 annet-0.8/annet/annlib/netdev/db.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-10 09:06:44.040765 annet-0.8/annet/annlib/netdev/devdb/
--rw-r--r--   0 runner    (1001) docker     (127)      892 2024-04-10 09:06:40.000000 annet-0.8/annet/annlib/netdev/devdb/__init__.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-10 09:06:44.040765 annet-0.8/annet/annlib/netdev/devdb/data/
--rw-r--r--   0 runner    (1001) docker     (127)     4733 2024-04-10 09:06:40.000000 annet-0.8/annet/annlib/netdev/devdb/data/devdb.json
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-10 09:06:44.040765 annet-0.8/annet/annlib/netdev/views/
--rw-r--r--   0 runner    (1001) docker     (127)        0 2024-04-10 09:06:40.000000 annet-0.8/annet/annlib/netdev/views/__init__.py
--rw-r--r--   0 runner    (1001) docker     (127)     4184 2024-04-10 09:06:40.000000 annet-0.8/annet/annlib/netdev/views/dump.py
--rw-r--r--   0 runner    (1001) docker     (127)     3192 2024-04-10 09:06:40.000000 annet-0.8/annet/annlib/netdev/views/hardware.py
--rw-r--r--   0 runner    (1001) docker     (127)     7569 2024-04-10 09:06:40.000000 annet-0.8/annet/annlib/output.py
--rw-r--r--   0 runner    (1001) docker     (127)    19784 2024-04-10 09:06:40.000000 annet-0.8/annet/annlib/patching.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-10 09:06:44.040765 annet-0.8/annet/annlib/rbparser/
--rw-r--r--   0 runner    (1001) docker     (127)        0 2024-04-10 09:06:40.000000 annet-0.8/annet/annlib/rbparser/__init__.py
--rw-r--r--   0 runner    (1001) docker     (127)     3931 2024-04-10 09:06:40.000000 annet-0.8/annet/annlib/rbparser/acl.py
--rw-r--r--   0 runner    (1001) docker     (127)     1649 2024-04-10 09:06:40.000000 annet-0.8/annet/annlib/rbparser/deploying.py
--rw-r--r--   0 runner    (1001) docker     (127)     1779 2024-04-10 09:06:40.000000 annet-0.8/annet/annlib/rbparser/ordering.py
--rw-r--r--   0 runner    (1001) docker     (127)     1231 2024-04-10 09:06:40.000000 annet-0.8/annet/annlib/rbparser/platform.py
--rw-r--r--   0 runner    (1001) docker     (127)     3572 2024-04-10 09:06:40.000000 annet-0.8/annet/annlib/rbparser/syntax.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-10 09:06:44.040765 annet-0.8/annet/annlib/rulebook/
--rw-r--r--   0 runner    (1001) docker     (127)        0 2024-04-10 09:06:40.000000 annet-0.8/annet/annlib/rulebook/__init__.py
--rw-r--r--   0 runner    (1001) docker     (127)    16054 2024-04-10 09:06:40.000000 annet-0.8/annet/annlib/rulebook/common.py
--rw-r--r--   0 runner    (1001) docker     (127)    22910 2024-04-10 09:06:40.000000 annet-0.8/annet/annlib/tabparser.py
--rw-r--r--   0 runner    (1001) docker     (127)      852 2024-04-10 09:06:40.000000 annet-0.8/annet/annlib/types.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-10 09:06:44.040765 annet-0.8/annet/api/
--rw-r--r--   0 runner    (1001) docker     (127)    33752 2024-04-10 09:06:40.000000 annet-0.8/annet/api/__init__.py
--rw-r--r--   0 runner    (1001) docker     (127)    12608 2024-04-10 09:06:40.000000 annet-0.8/annet/argparse.py
--rw-r--r--   0 runner    (1001) docker     (127)     8464 2024-04-10 09:06:40.000000 annet-0.8/annet/cli.py
--rw-r--r--   0 runner    (1001) docker     (127)    16152 2024-04-10 09:06:40.000000 annet-0.8/annet/cli_args.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-10 09:06:44.044765 annet-0.8/annet/configs/
--rw-r--r--   0 runner    (1001) docker     (127)      291 2024-04-10 09:06:40.000000 annet-0.8/annet/configs/context.yml
--rw-r--r--   0 runner    (1001) docker     (127)      970 2024-04-10 09:06:40.000000 annet-0.8/annet/configs/logging.yaml
--rw-r--r--   0 runner    (1001) docker     (127)     1908 2024-04-10 09:06:40.000000 annet-0.8/annet/connectors.py
--rw-r--r--   0 runner    (1001) docker     (127)    18893 2024-04-10 09:06:40.000000 annet-0.8/annet/deploy.py
--rw-r--r--   0 runner    (1001) docker     (127)     3391 2024-04-10 09:06:40.000000 annet-0.8/annet/diff.py
--rw-r--r--   0 runner    (1001) docker     (127)    19040 2024-04-10 09:06:40.000000 annet-0.8/annet/executor.py
--rw-r--r--   0 runner    (1001) docker     (127)      852 2024-04-10 09:06:40.000000 annet-0.8/annet/filtering.py
--rw-r--r--   0 runner    (1001) docker     (127)    32336 2024-04-10 09:06:40.000000 annet-0.8/annet/gen.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-10 09:06:44.044765 annet-0.8/annet/generators/
--rw-r--r--   0 runner    (1001) docker     (127)    34476 2024-04-10 09:06:40.000000 annet-0.8/annet/generators/__init__.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-10 09:06:44.044765 annet-0.8/annet/generators/common/
--rw-r--r--   0 runner    (1001) docker     (127)        0 2024-04-10 09:06:40.000000 annet-0.8/annet/generators/common/__init__.py
--rw-r--r--   0 runner    (1001) docker     (127)     1229 2024-04-10 09:06:40.000000 annet-0.8/annet/generators/common/initial.py
--rw-r--r--   0 runner    (1001) docker     (127)     1090 2024-04-10 09:06:40.000000 annet-0.8/annet/hardware.py
--rw-r--r--   0 runner    (1001) docker     (127)     5139 2024-04-10 09:06:40.000000 annet-0.8/annet/implicit.py
--rw-r--r--   0 runner    (1001) docker     (127)     3742 2024-04-10 09:06:40.000000 annet-0.8/annet/lib.py
--rw-r--r--   0 runner    (1001) docker     (127)     7090 2024-04-10 09:06:40.000000 annet-0.8/annet/output.py
--rw-r--r--   0 runner    (1001) docker     (127)    17160 2024-04-10 09:06:40.000000 annet-0.8/annet/parallel.py
--rw-r--r--   0 runner    (1001) docker     (127)      559 2024-04-10 09:06:40.000000 annet-0.8/annet/patching.py
--rw-r--r--   0 runner    (1001) docker     (127)     4035 2024-04-10 09:06:40.000000 annet-0.8/annet/reference.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-10 09:06:44.044765 annet-0.8/annet/rulebook/
--rw-r--r--   0 runner    (1001) docker     (127)     3847 2024-04-10 09:06:40.000000 annet-0.8/annet/rulebook/__init__.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-10 09:06:44.044765 annet-0.8/annet/rulebook/arista/
--rw-r--r--   0 runner    (1001) docker     (127)        0 2024-04-10 09:06:40.000000 annet-0.8/annet/rulebook/arista/__init__.py
--rw-r--r--   0 runner    (1001) docker     (127)      720 2024-04-10 09:06:40.000000 annet-0.8/annet/rulebook/arista/iface.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-10 09:06:44.044765 annet-0.8/annet/rulebook/aruba/
--rw-r--r--   0 runner    (1001) docker     (127)      500 2024-04-10 09:06:40.000000 annet-0.8/annet/rulebook/aruba/__init__.py
--rw-r--r--   0 runner    (1001) docker     (127)     4788 2024-04-10 09:06:40.000000 annet-0.8/annet/rulebook/aruba/ap_env.py
--rw-r--r--   0 runner    (1001) docker     (127)      234 2024-04-10 09:06:40.000000 annet-0.8/annet/rulebook/aruba/misc.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-10 09:06:44.044765 annet-0.8/annet/rulebook/cisco/
--rw-r--r--   0 runner    (1001) docker     (127)        0 2024-04-10 09:06:40.000000 annet-0.8/annet/rulebook/cisco/__init__.py
--rw-r--r--   0 runner    (1001) docker     (127)     1792 2024-04-10 09:06:40.000000 annet-0.8/annet/rulebook/cisco/iface.py
--rw-r--r--   0 runner    (1001) docker     (127)     2259 2024-04-10 09:06:40.000000 annet-0.8/annet/rulebook/cisco/misc.py
--rw-r--r--   0 runner    (1001) docker     (127)     3319 2024-04-10 09:06:40.000000 annet-0.8/annet/rulebook/cisco/vlandb.py
--rw-r--r--   0 runner    (1001) docker     (127)      721 2024-04-10 09:06:40.000000 annet-0.8/annet/rulebook/common.py
--rw-r--r--   0 runner    (1001) docker     (127)     2972 2024-04-10 09:06:40.000000 annet-0.8/annet/rulebook/deploying.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-10 09:06:44.044765 annet-0.8/annet/rulebook/huawei/
--rw-r--r--   0 runner    (1001) docker     (127)        0 2024-04-10 09:06:40.000000 annet-0.8/annet/rulebook/huawei/__init__.py
--rw-r--r--   0 runner    (1001) docker     (127)     3445 2024-04-10 09:06:40.000000 annet-0.8/annet/rulebook/huawei/aaa.py
--rw-r--r--   0 runner    (1001) docker     (127)     4015 2024-04-10 09:06:40.000000 annet-0.8/annet/rulebook/huawei/bgp.py
--rw-r--r--   0 runner    (1001) docker     (127)     1126 2024-04-10 09:06:40.000000 annet-0.8/annet/rulebook/huawei/iface.py
--rw-r--r--   0 runner    (1001) docker     (127)    14424 2024-04-10 09:06:40.000000 annet-0.8/annet/rulebook/huawei/misc.py
--rw-r--r--   0 runner    (1001) docker     (127)     4658 2024-04-10 09:06:40.000000 annet-0.8/annet/rulebook/huawei/vlandb.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-10 09:06:44.044765 annet-0.8/annet/rulebook/juniper/
--rw-r--r--   0 runner    (1001) docker     (127)     3887 2024-04-10 09:06:40.000000 annet-0.8/annet/rulebook/juniper/__init__.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-10 09:06:44.044765 annet-0.8/annet/rulebook/nexus/
--rw-r--r--   0 runner    (1001) docker     (127)        0 2024-04-10 09:06:40.000000 annet-0.8/annet/rulebook/nexus/__init__.py
--rw-r--r--   0 runner    (1001) docker     (127)     2923 2024-04-10 09:06:40.000000 annet-0.8/annet/rulebook/nexus/iface.py
--rw-r--r--   0 runner    (1001) docker     (127)     4970 2024-04-10 09:06:40.000000 annet-0.8/annet/rulebook/patching.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-10 09:06:44.044765 annet-0.8/annet/rulebook/ribbon/
--rw-r--r--   0 runner    (1001) docker     (127)      347 2024-04-10 09:06:40.000000 annet-0.8/annet/rulebook/ribbon/__init__.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-10 09:06:44.048766 annet-0.8/annet/rulebook/texts/
--rw-r--r--   0 runner    (1001) docker     (127)      792 2024-04-10 09:06:40.000000 annet-0.8/annet/rulebook/texts/arista.deploy
--rw-r--r--   0 runner    (1001) docker     (127)     1457 2024-04-10 09:06:40.000000 annet-0.8/annet/rulebook/texts/arista.order
--rw-r--r--   0 runner    (1001) docker     (127)      786 2024-04-10 09:06:40.000000 annet-0.8/annet/rulebook/texts/arista.rul
--rw-r--r--   0 runner    (1001) docker     (127)      841 2024-04-10 09:06:40.000000 annet-0.8/annet/rulebook/texts/aruba.deploy
--rw-r--r--   0 runner    (1001) docker     (127)     1158 2024-04-10 09:06:40.000000 annet-0.8/annet/rulebook/texts/aruba.order
--rw-r--r--   0 runner    (1001) docker     (127)     2584 2024-04-10 09:06:40.000000 annet-0.8/annet/rulebook/texts/aruba.rul
--rw-r--r--   0 runner    (1001) docker     (127)     1226 2024-04-10 09:06:40.000000 annet-0.8/annet/rulebook/texts/cisco.deploy
--rw-r--r--   0 runner    (1001) docker     (127)     1709 2024-04-10 09:06:40.000000 annet-0.8/annet/rulebook/texts/cisco.order
--rw-r--r--   0 runner    (1001) docker     (127)     2869 2024-04-10 09:06:40.000000 annet-0.8/annet/rulebook/texts/cisco.rul
--rw-r--r--   0 runner    (1001) docker     (127)    10444 2024-04-10 09:06:40.000000 annet-0.8/annet/rulebook/texts/huawei.deploy
--rw-r--r--   0 runner    (1001) docker     (127)    10657 2024-04-10 09:06:40.000000 annet-0.8/annet/rulebook/texts/huawei.order
--rw-r--r--   0 runner    (1001) docker     (127)    12958 2024-04-10 09:06:40.000000 annet-0.8/annet/rulebook/texts/huawei.rul
--rw-r--r--   0 runner    (1001) docker     (127)     2654 2024-04-10 09:06:40.000000 annet-0.8/annet/rulebook/texts/juniper.rul
--rw-r--r--   0 runner    (1001) docker     (127)     1120 2024-04-10 09:06:40.000000 annet-0.8/annet/rulebook/texts/nexus.deploy
--rw-r--r--   0 runner    (1001) docker     (127)     1834 2024-04-10 09:06:40.000000 annet-0.8/annet/rulebook/texts/nexus.order
--rw-r--r--   0 runner    (1001) docker     (127)     2558 2024-04-10 09:06:40.000000 annet-0.8/annet/rulebook/texts/nexus.rul
--rw-r--r--   0 runner    (1001) docker     (127)     1077 2024-04-10 09:06:40.000000 annet-0.8/annet/rulebook/texts/nokia.rul
--rw-r--r--   0 runner    (1001) docker     (127)      275 2024-04-10 09:06:40.000000 annet-0.8/annet/rulebook/texts/pc.order
--rw-r--r--   0 runner    (1001) docker     (127)      302 2024-04-10 09:06:40.000000 annet-0.8/annet/rulebook/texts/pc.rul
--rw-r--r--   0 runner    (1001) docker     (127)      864 2024-04-10 09:06:40.000000 annet-0.8/annet/rulebook/texts/ribbon.deploy
--rw-r--r--   0 runner    (1001) docker     (127)     2108 2024-04-10 09:06:40.000000 annet-0.8/annet/rulebook/texts/ribbon.rul
--rw-r--r--   0 runner    (1001) docker     (127)      905 2024-04-10 09:06:40.000000 annet-0.8/annet/rulebook/texts/routeros.order
--rw-r--r--   0 runner    (1001) docker     (127)     1203 2024-04-10 09:06:40.000000 annet-0.8/annet/rulebook/texts/routeros.rul
--rw-r--r--   0 runner    (1001) docker     (127)     2299 2024-04-10 09:06:40.000000 annet-0.8/annet/storage.py
--rw-r--r--   0 runner    (1001) docker     (127)      874 2024-04-10 09:06:40.000000 annet-0.8/annet/tabparser.py
--rw-r--r--   0 runner    (1001) docker     (127)     2813 2024-04-10 09:06:40.000000 annet-0.8/annet/text_term_format.py
--rw-r--r--   0 runner    (1001) docker     (127)     4044 2024-04-10 09:06:40.000000 annet-0.8/annet/tracing.py
--rw-r--r--   0 runner    (1001) docker     (127)     6962 2024-04-10 09:06:40.000000 annet-0.8/annet/types.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-10 09:06:44.048766 annet-0.8/annet.egg-info/
--rw-r--r--   0 runner    (1001) docker     (127)      674 2024-04-10 09:06:44.000000 annet-0.8/annet.egg-info/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (127)     3833 2024-04-10 09:06:44.000000 annet-0.8/annet.egg-info/SOURCES.txt
--rw-r--r--   0 runner    (1001) docker     (127)        1 2024-04-10 09:06:44.000000 annet-0.8/annet.egg-info/dependency_links.txt
--rw-r--r--   0 runner    (1001) docker     (127)      119 2024-04-10 09:06:44.000000 annet-0.8/annet.egg-info/entry_points.txt
--rw-r--r--   0 runner    (1001) docker     (127)      246 2024-04-10 09:06:44.000000 annet-0.8/annet.egg-info/requires.txt
--rw-r--r--   0 runner    (1001) docker     (127)       23 2024-04-10 09:06:44.000000 annet-0.8/annet.egg-info/top_level.txt
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-10 09:06:44.048766 annet-0.8/annet_generators/
--rw-r--r--   0 runner    (1001) docker     (127)        0 2024-04-10 09:06:40.000000 annet-0.8/annet_generators/__init__.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-10 09:06:44.048766 annet-0.8/annet_generators/example/
--rw-r--r--   0 runner    (1001) docker     (127)      228 2024-04-10 09:06:40.000000 annet-0.8/annet_generators/example/__init__.py
--rw-r--r--   0 runner    (1001) docker     (127)     1146 2024-04-10 09:06:40.000000 annet-0.8/annet_generators/example/lldp.py
--rw-r--r--   0 runner    (1001) docker     (127)      246 2024-04-10 09:06:40.000000 annet-0.8/requirements.txt
--rw-r--r--   0 runner    (1001) docker     (127)       38 2024-04-10 09:06:44.052765 annet-0.8/setup.cfg
--rwxr-xr-x   0 runner    (1001) docker     (127)     1283 2024-04-10 09:06:40.000000 annet-0.8/setup.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-10 14:33:35.646893 annet-0.9/
+-rw-r--r--   0 runner    (1001) docker     (127)      878 2024-04-10 14:33:30.000000 annet-0.9/AUTHORS
+-rw-r--r--   0 runner    (1001) docker     (127)     1079 2024-04-10 14:33:30.000000 annet-0.9/LICENSE
+-rw-r--r--   0 runner    (1001) docker     (127)       25 2024-04-10 14:33:30.000000 annet-0.9/MANIFEST.in
+-rw-r--r--   0 runner    (1001) docker     (127)      674 2024-04-10 14:33:35.646893 annet-0.9/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (127)     4794 2024-04-10 14:33:30.000000 annet-0.9/README.md
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-10 14:33:35.630894 annet-0.9/annet/
+-rw-r--r--   0 runner    (1001) docker     (127)     2139 2024-04-10 14:33:30.000000 annet-0.9/annet/__init__.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-10 14:33:35.630894 annet-0.9/annet/adapters/
+-rw-r--r--   0 runner    (1001) docker     (127)        0 2024-04-10 14:33:30.000000 annet-0.9/annet/adapters/__init__.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-10 14:33:35.630894 annet-0.9/annet/adapters/netbox/
+-rw-r--r--   0 runner    (1001) docker     (127)        0 2024-04-10 14:33:30.000000 annet-0.9/annet/adapters/netbox/__init__.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-10 14:33:35.634894 annet-0.9/annet/adapters/netbox/common/
+-rw-r--r--   0 runner    (1001) docker     (127)        0 2024-04-10 14:33:30.000000 annet-0.9/annet/adapters/netbox/common/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (127)     2483 2024-04-10 14:33:30.000000 annet-0.9/annet/adapters/netbox/common/client.py
+-rw-r--r--   0 runner    (1001) docker     (127)     1771 2024-04-10 14:33:30.000000 annet-0.9/annet/adapters/netbox/common/manufacturer.py
+-rw-r--r--   0 runner    (1001) docker     (127)     1731 2024-04-10 14:33:30.000000 annet-0.9/annet/adapters/netbox/common/models.py
+-rw-r--r--   0 runner    (1001) docker     (127)      577 2024-04-10 14:33:30.000000 annet-0.9/annet/adapters/netbox/common/query.py
+-rw-r--r--   0 runner    (1001) docker     (127)      567 2024-04-10 14:33:30.000000 annet-0.9/annet/adapters/netbox/common/status_client.py
+-rw-r--r--   0 runner    (1001) docker     (127)      337 2024-04-10 14:33:30.000000 annet-0.9/annet/adapters/netbox/common/storage_opts.py
+-rw-r--r--   0 runner    (1001) docker     (127)     1024 2024-04-10 14:33:30.000000 annet-0.9/annet/adapters/netbox/provider.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-10 14:33:35.634894 annet-0.9/annet/adapters/netbox/v24/
+-rw-r--r--   0 runner    (1001) docker     (127)        0 2024-04-10 14:33:30.000000 annet-0.9/annet/adapters/netbox/v24/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (127)     1314 2024-04-10 14:33:30.000000 annet-0.9/annet/adapters/netbox/v24/api_models.py
+-rw-r--r--   0 runner    (1001) docker     (127)     1497 2024-04-10 14:33:30.000000 annet-0.9/annet/adapters/netbox/v24/client.py
+-rw-r--r--   0 runner    (1001) docker     (127)     5620 2024-04-10 14:33:30.000000 annet-0.9/annet/adapters/netbox/v24/storage.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-10 14:33:35.634894 annet-0.9/annet/adapters/netbox/v37/
+-rw-r--r--   0 runner    (1001) docker     (127)        0 2024-04-10 14:33:30.000000 annet-0.9/annet/adapters/netbox/v37/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (127)      886 2024-04-10 14:33:30.000000 annet-0.9/annet/adapters/netbox/v37/api_models.py
+-rw-r--r--   0 runner    (1001) docker     (127)     1668 2024-04-10 14:33:30.000000 annet-0.9/annet/adapters/netbox/v37/client.py
+-rw-r--r--   0 runner    (1001) docker     (127)     4216 2024-04-10 14:33:30.000000 annet-0.9/annet/adapters/netbox/v37/storage.py
+-rwxr-xr-x   0 runner    (1001) docker     (127)      725 2024-04-10 14:33:30.000000 annet-0.9/annet/annet.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-10 14:33:35.634894 annet-0.9/annet/annlib/
+-rw-r--r--   0 runner    (1001) docker     (127)      252 2024-04-10 14:33:30.000000 annet-0.9/annet/annlib/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (127)     1043 2024-04-10 14:33:30.000000 annet-0.9/annet/annlib/command.py
+-rw-r--r--   0 runner    (1001) docker     (127)     4587 2024-04-10 14:33:30.000000 annet-0.9/annet/annlib/diff.py
+-rw-r--r--   0 runner    (1001) docker     (127)      287 2024-04-10 14:33:30.000000 annet-0.9/annet/annlib/errors.py
+-rw-r--r--   0 runner    (1001) docker     (127)     7203 2024-04-10 14:33:30.000000 annet-0.9/annet/annlib/filter_acl.py
+-rw-r--r--   0 runner    (1001) docker     (127)     3359 2024-04-10 14:33:30.000000 annet-0.9/annet/annlib/jsontools.py
+-rw-r--r--   0 runner    (1001) docker     (127)    15317 2024-04-10 14:33:30.000000 annet-0.9/annet/annlib/lib.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-10 14:33:35.634894 annet-0.9/annet/annlib/netdev/
+-rw-r--r--   0 runner    (1001) docker     (127)        0 2024-04-10 14:33:30.000000 annet-0.9/annet/annlib/netdev/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (127)     1634 2024-04-10 14:33:30.000000 annet-0.9/annet/annlib/netdev/db.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-10 14:33:35.638893 annet-0.9/annet/annlib/netdev/devdb/
+-rw-r--r--   0 runner    (1001) docker     (127)      892 2024-04-10 14:33:30.000000 annet-0.9/annet/annlib/netdev/devdb/__init__.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-10 14:33:35.638893 annet-0.9/annet/annlib/netdev/devdb/data/
+-rw-r--r--   0 runner    (1001) docker     (127)     4733 2024-04-10 14:33:30.000000 annet-0.9/annet/annlib/netdev/devdb/data/devdb.json
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-10 14:33:35.638893 annet-0.9/annet/annlib/netdev/views/
+-rw-r--r--   0 runner    (1001) docker     (127)        0 2024-04-10 14:33:30.000000 annet-0.9/annet/annlib/netdev/views/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (127)     4184 2024-04-10 14:33:30.000000 annet-0.9/annet/annlib/netdev/views/dump.py
+-rw-r--r--   0 runner    (1001) docker     (127)     3192 2024-04-10 14:33:30.000000 annet-0.9/annet/annlib/netdev/views/hardware.py
+-rw-r--r--   0 runner    (1001) docker     (127)     7569 2024-04-10 14:33:30.000000 annet-0.9/annet/annlib/output.py
+-rw-r--r--   0 runner    (1001) docker     (127)    19784 2024-04-10 14:33:30.000000 annet-0.9/annet/annlib/patching.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-10 14:33:35.638893 annet-0.9/annet/annlib/rbparser/
+-rw-r--r--   0 runner    (1001) docker     (127)        0 2024-04-10 14:33:30.000000 annet-0.9/annet/annlib/rbparser/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (127)     3931 2024-04-10 14:33:30.000000 annet-0.9/annet/annlib/rbparser/acl.py
+-rw-r--r--   0 runner    (1001) docker     (127)     1649 2024-04-10 14:33:30.000000 annet-0.9/annet/annlib/rbparser/deploying.py
+-rw-r--r--   0 runner    (1001) docker     (127)     1779 2024-04-10 14:33:30.000000 annet-0.9/annet/annlib/rbparser/ordering.py
+-rw-r--r--   0 runner    (1001) docker     (127)     1231 2024-04-10 14:33:30.000000 annet-0.9/annet/annlib/rbparser/platform.py
+-rw-r--r--   0 runner    (1001) docker     (127)     3572 2024-04-10 14:33:30.000000 annet-0.9/annet/annlib/rbparser/syntax.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-10 14:33:35.638893 annet-0.9/annet/annlib/rulebook/
+-rw-r--r--   0 runner    (1001) docker     (127)        0 2024-04-10 14:33:30.000000 annet-0.9/annet/annlib/rulebook/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (127)    16054 2024-04-10 14:33:30.000000 annet-0.9/annet/annlib/rulebook/common.py
+-rw-r--r--   0 runner    (1001) docker     (127)    22910 2024-04-10 14:33:30.000000 annet-0.9/annet/annlib/tabparser.py
+-rw-r--r--   0 runner    (1001) docker     (127)      852 2024-04-10 14:33:30.000000 annet-0.9/annet/annlib/types.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-10 14:33:35.638893 annet-0.9/annet/api/
+-rw-r--r--   0 runner    (1001) docker     (127)    33752 2024-04-10 14:33:30.000000 annet-0.9/annet/api/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (127)    12608 2024-04-10 14:33:30.000000 annet-0.9/annet/argparse.py
+-rw-r--r--   0 runner    (1001) docker     (127)     8464 2024-04-10 14:33:30.000000 annet-0.9/annet/cli.py
+-rw-r--r--   0 runner    (1001) docker     (127)    16152 2024-04-10 14:33:30.000000 annet-0.9/annet/cli_args.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-10 14:33:35.638893 annet-0.9/annet/configs/
+-rw-r--r--   0 runner    (1001) docker     (127)      291 2024-04-10 14:33:30.000000 annet-0.9/annet/configs/context.yml
+-rw-r--r--   0 runner    (1001) docker     (127)      970 2024-04-10 14:33:30.000000 annet-0.9/annet/configs/logging.yaml
+-rw-r--r--   0 runner    (1001) docker     (127)     1908 2024-04-10 14:33:30.000000 annet-0.9/annet/connectors.py
+-rw-r--r--   0 runner    (1001) docker     (127)    18893 2024-04-10 14:33:30.000000 annet-0.9/annet/deploy.py
+-rw-r--r--   0 runner    (1001) docker     (127)     3391 2024-04-10 14:33:30.000000 annet-0.9/annet/diff.py
+-rw-r--r--   0 runner    (1001) docker     (127)    19040 2024-04-10 14:33:30.000000 annet-0.9/annet/executor.py
+-rw-r--r--   0 runner    (1001) docker     (127)      852 2024-04-10 14:33:30.000000 annet-0.9/annet/filtering.py
+-rw-r--r--   0 runner    (1001) docker     (127)    33068 2024-04-10 14:33:30.000000 annet-0.9/annet/gen.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-10 14:33:35.638893 annet-0.9/annet/generators/
+-rw-r--r--   0 runner    (1001) docker     (127)    34964 2024-04-10 14:33:30.000000 annet-0.9/annet/generators/__init__.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-10 14:33:35.638893 annet-0.9/annet/generators/common/
+-rw-r--r--   0 runner    (1001) docker     (127)        0 2024-04-10 14:33:30.000000 annet-0.9/annet/generators/common/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (127)     1229 2024-04-10 14:33:30.000000 annet-0.9/annet/generators/common/initial.py
+-rw-r--r--   0 runner    (1001) docker     (127)     1090 2024-04-10 14:33:30.000000 annet-0.9/annet/hardware.py
+-rw-r--r--   0 runner    (1001) docker     (127)     5139 2024-04-10 14:33:30.000000 annet-0.9/annet/implicit.py
+-rw-r--r--   0 runner    (1001) docker     (127)     3742 2024-04-10 14:33:30.000000 annet-0.9/annet/lib.py
+-rw-r--r--   0 runner    (1001) docker     (127)     7090 2024-04-10 14:33:30.000000 annet-0.9/annet/output.py
+-rw-r--r--   0 runner    (1001) docker     (127)    17160 2024-04-10 14:33:30.000000 annet-0.9/annet/parallel.py
+-rw-r--r--   0 runner    (1001) docker     (127)      559 2024-04-10 14:33:30.000000 annet-0.9/annet/patching.py
+-rw-r--r--   0 runner    (1001) docker     (127)     4035 2024-04-10 14:33:30.000000 annet-0.9/annet/reference.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-10 14:33:35.638893 annet-0.9/annet/rulebook/
+-rw-r--r--   0 runner    (1001) docker     (127)     3847 2024-04-10 14:33:30.000000 annet-0.9/annet/rulebook/__init__.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-10 14:33:35.642893 annet-0.9/annet/rulebook/arista/
+-rw-r--r--   0 runner    (1001) docker     (127)        0 2024-04-10 14:33:30.000000 annet-0.9/annet/rulebook/arista/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (127)      720 2024-04-10 14:33:30.000000 annet-0.9/annet/rulebook/arista/iface.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-10 14:33:35.642893 annet-0.9/annet/rulebook/aruba/
+-rw-r--r--   0 runner    (1001) docker     (127)      500 2024-04-10 14:33:30.000000 annet-0.9/annet/rulebook/aruba/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (127)     4788 2024-04-10 14:33:30.000000 annet-0.9/annet/rulebook/aruba/ap_env.py
+-rw-r--r--   0 runner    (1001) docker     (127)      234 2024-04-10 14:33:30.000000 annet-0.9/annet/rulebook/aruba/misc.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-10 14:33:35.642893 annet-0.9/annet/rulebook/cisco/
+-rw-r--r--   0 runner    (1001) docker     (127)        0 2024-04-10 14:33:30.000000 annet-0.9/annet/rulebook/cisco/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (127)     1792 2024-04-10 14:33:30.000000 annet-0.9/annet/rulebook/cisco/iface.py
+-rw-r--r--   0 runner    (1001) docker     (127)     2259 2024-04-10 14:33:30.000000 annet-0.9/annet/rulebook/cisco/misc.py
+-rw-r--r--   0 runner    (1001) docker     (127)     3319 2024-04-10 14:33:30.000000 annet-0.9/annet/rulebook/cisco/vlandb.py
+-rw-r--r--   0 runner    (1001) docker     (127)      721 2024-04-10 14:33:30.000000 annet-0.9/annet/rulebook/common.py
+-rw-r--r--   0 runner    (1001) docker     (127)     2972 2024-04-10 14:33:30.000000 annet-0.9/annet/rulebook/deploying.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-10 14:33:35.642893 annet-0.9/annet/rulebook/huawei/
+-rw-r--r--   0 runner    (1001) docker     (127)        0 2024-04-10 14:33:30.000000 annet-0.9/annet/rulebook/huawei/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (127)     3445 2024-04-10 14:33:30.000000 annet-0.9/annet/rulebook/huawei/aaa.py
+-rw-r--r--   0 runner    (1001) docker     (127)     4015 2024-04-10 14:33:30.000000 annet-0.9/annet/rulebook/huawei/bgp.py
+-rw-r--r--   0 runner    (1001) docker     (127)     1126 2024-04-10 14:33:30.000000 annet-0.9/annet/rulebook/huawei/iface.py
+-rw-r--r--   0 runner    (1001) docker     (127)    14424 2024-04-10 14:33:30.000000 annet-0.9/annet/rulebook/huawei/misc.py
+-rw-r--r--   0 runner    (1001) docker     (127)     4658 2024-04-10 14:33:30.000000 annet-0.9/annet/rulebook/huawei/vlandb.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-10 14:33:35.642893 annet-0.9/annet/rulebook/juniper/
+-rw-r--r--   0 runner    (1001) docker     (127)     3887 2024-04-10 14:33:30.000000 annet-0.9/annet/rulebook/juniper/__init__.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-10 14:33:35.642893 annet-0.9/annet/rulebook/nexus/
+-rw-r--r--   0 runner    (1001) docker     (127)        0 2024-04-10 14:33:30.000000 annet-0.9/annet/rulebook/nexus/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (127)     2923 2024-04-10 14:33:30.000000 annet-0.9/annet/rulebook/nexus/iface.py
+-rw-r--r--   0 runner    (1001) docker     (127)     4970 2024-04-10 14:33:30.000000 annet-0.9/annet/rulebook/patching.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-10 14:33:35.642893 annet-0.9/annet/rulebook/ribbon/
+-rw-r--r--   0 runner    (1001) docker     (127)      347 2024-04-10 14:33:30.000000 annet-0.9/annet/rulebook/ribbon/__init__.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-10 14:33:35.646893 annet-0.9/annet/rulebook/texts/
+-rw-r--r--   0 runner    (1001) docker     (127)      792 2024-04-10 14:33:30.000000 annet-0.9/annet/rulebook/texts/arista.deploy
+-rw-r--r--   0 runner    (1001) docker     (127)     1457 2024-04-10 14:33:30.000000 annet-0.9/annet/rulebook/texts/arista.order
+-rw-r--r--   0 runner    (1001) docker     (127)      786 2024-04-10 14:33:30.000000 annet-0.9/annet/rulebook/texts/arista.rul
+-rw-r--r--   0 runner    (1001) docker     (127)      841 2024-04-10 14:33:30.000000 annet-0.9/annet/rulebook/texts/aruba.deploy
+-rw-r--r--   0 runner    (1001) docker     (127)     1158 2024-04-10 14:33:30.000000 annet-0.9/annet/rulebook/texts/aruba.order
+-rw-r--r--   0 runner    (1001) docker     (127)     2584 2024-04-10 14:33:30.000000 annet-0.9/annet/rulebook/texts/aruba.rul
+-rw-r--r--   0 runner    (1001) docker     (127)     1226 2024-04-10 14:33:30.000000 annet-0.9/annet/rulebook/texts/cisco.deploy
+-rw-r--r--   0 runner    (1001) docker     (127)     1709 2024-04-10 14:33:30.000000 annet-0.9/annet/rulebook/texts/cisco.order
+-rw-r--r--   0 runner    (1001) docker     (127)     2869 2024-04-10 14:33:30.000000 annet-0.9/annet/rulebook/texts/cisco.rul
+-rw-r--r--   0 runner    (1001) docker     (127)    10444 2024-04-10 14:33:30.000000 annet-0.9/annet/rulebook/texts/huawei.deploy
+-rw-r--r--   0 runner    (1001) docker     (127)    10657 2024-04-10 14:33:30.000000 annet-0.9/annet/rulebook/texts/huawei.order
+-rw-r--r--   0 runner    (1001) docker     (127)    12958 2024-04-10 14:33:30.000000 annet-0.9/annet/rulebook/texts/huawei.rul
+-rw-r--r--   0 runner    (1001) docker     (127)     2654 2024-04-10 14:33:30.000000 annet-0.9/annet/rulebook/texts/juniper.rul
+-rw-r--r--   0 runner    (1001) docker     (127)     1120 2024-04-10 14:33:30.000000 annet-0.9/annet/rulebook/texts/nexus.deploy
+-rw-r--r--   0 runner    (1001) docker     (127)     1834 2024-04-10 14:33:30.000000 annet-0.9/annet/rulebook/texts/nexus.order
+-rw-r--r--   0 runner    (1001) docker     (127)     2558 2024-04-10 14:33:30.000000 annet-0.9/annet/rulebook/texts/nexus.rul
+-rw-r--r--   0 runner    (1001) docker     (127)     1077 2024-04-10 14:33:30.000000 annet-0.9/annet/rulebook/texts/nokia.rul
+-rw-r--r--   0 runner    (1001) docker     (127)      275 2024-04-10 14:33:30.000000 annet-0.9/annet/rulebook/texts/pc.order
+-rw-r--r--   0 runner    (1001) docker     (127)      302 2024-04-10 14:33:30.000000 annet-0.9/annet/rulebook/texts/pc.rul
+-rw-r--r--   0 runner    (1001) docker     (127)      864 2024-04-10 14:33:30.000000 annet-0.9/annet/rulebook/texts/ribbon.deploy
+-rw-r--r--   0 runner    (1001) docker     (127)     2108 2024-04-10 14:33:30.000000 annet-0.9/annet/rulebook/texts/ribbon.rul
+-rw-r--r--   0 runner    (1001) docker     (127)      905 2024-04-10 14:33:30.000000 annet-0.9/annet/rulebook/texts/routeros.order
+-rw-r--r--   0 runner    (1001) docker     (127)     1203 2024-04-10 14:33:30.000000 annet-0.9/annet/rulebook/texts/routeros.rul
+-rw-r--r--   0 runner    (1001) docker     (127)     2299 2024-04-10 14:33:30.000000 annet-0.9/annet/storage.py
+-rw-r--r--   0 runner    (1001) docker     (127)      874 2024-04-10 14:33:30.000000 annet-0.9/annet/tabparser.py
+-rw-r--r--   0 runner    (1001) docker     (127)     2813 2024-04-10 14:33:30.000000 annet-0.9/annet/text_term_format.py
+-rw-r--r--   0 runner    (1001) docker     (127)     4044 2024-04-10 14:33:30.000000 annet-0.9/annet/tracing.py
+-rw-r--r--   0 runner    (1001) docker     (127)     7158 2024-04-10 14:33:30.000000 annet-0.9/annet/types.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-10 14:33:35.646893 annet-0.9/annet.egg-info/
+-rw-r--r--   0 runner    (1001) docker     (127)      674 2024-04-10 14:33:35.000000 annet-0.9/annet.egg-info/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (127)     3833 2024-04-10 14:33:35.000000 annet-0.9/annet.egg-info/SOURCES.txt
+-rw-r--r--   0 runner    (1001) docker     (127)        1 2024-04-10 14:33:35.000000 annet-0.9/annet.egg-info/dependency_links.txt
+-rw-r--r--   0 runner    (1001) docker     (127)      119 2024-04-10 14:33:35.000000 annet-0.9/annet.egg-info/entry_points.txt
+-rw-r--r--   0 runner    (1001) docker     (127)      246 2024-04-10 14:33:35.000000 annet-0.9/annet.egg-info/requires.txt
+-rw-r--r--   0 runner    (1001) docker     (127)       23 2024-04-10 14:33:35.000000 annet-0.9/annet.egg-info/top_level.txt
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-10 14:33:35.646893 annet-0.9/annet_generators/
+-rw-r--r--   0 runner    (1001) docker     (127)        0 2024-04-10 14:33:30.000000 annet-0.9/annet_generators/__init__.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-10 14:33:35.646893 annet-0.9/annet_generators/example/
+-rw-r--r--   0 runner    (1001) docker     (127)      228 2024-04-10 14:33:30.000000 annet-0.9/annet_generators/example/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (127)     1146 2024-04-10 14:33:30.000000 annet-0.9/annet_generators/example/lldp.py
+-rw-r--r--   0 runner    (1001) docker     (127)      246 2024-04-10 14:33:30.000000 annet-0.9/requirements.txt
+-rw-r--r--   0 runner    (1001) docker     (127)       38 2024-04-10 14:33:35.646893 annet-0.9/setup.cfg
+-rwxr-xr-x   0 runner    (1001) docker     (127)     1283 2024-04-10 14:33:30.000000 annet-0.9/setup.py
```

### Comparing `annet-0.8/AUTHORS` & `annet-0.9/AUTHORS`

 * *Files identical despite different names*

### Comparing `annet-0.8/LICENSE` & `annet-0.9/LICENSE`

 * *Files identical despite different names*

### Comparing `annet-0.8/PKG-INFO` & `annet-0.9/PKG-INFO`

 * *Files 7% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: annet
-Version: 0.8
+Version: 0.9
 Summary: annet
 Home-page: https://github.com/annetutil/annet
 License: MIT
 Requires-Python: >=3.8
 License-File: LICENSE
 License-File: AUTHORS
 Requires-Dist: colorama>=0.4.6
```

### Comparing `annet-0.8/README.md` & `annet-0.9/README.md`

 * *Files identical despite different names*

### Comparing `annet-0.8/annet/__init__.py` & `annet-0.9/annet/__init__.py`

 * *Files identical despite different names*

### Comparing `annet-0.8/annet/adapters/netbox/common/client.py` & `annet-0.9/annet/adapters/netbox/common/client.py`

 * *Files identical despite different names*

### Comparing `annet-0.8/annet/adapters/netbox/common/manufacturer.py` & `annet-0.9/annet/adapters/netbox/common/manufacturer.py`

 * *Files identical despite different names*

### Comparing `annet-0.8/annet/adapters/netbox/common/models.py` & `annet-0.9/annet/adapters/netbox/common/models.py`

 * *Files identical despite different names*

### Comparing `annet-0.8/annet/adapters/netbox/common/query.py` & `annet-0.9/annet/adapters/netbox/common/query.py`

 * *Files identical despite different names*

### Comparing `annet-0.8/annet/adapters/netbox/common/status_client.py` & `annet-0.9/annet/adapters/netbox/common/status_client.py`

 * *Files identical despite different names*

### Comparing `annet-0.8/annet/adapters/netbox/provider.py` & `annet-0.9/annet/adapters/netbox/provider.py`

 * *Files identical despite different names*

### Comparing `annet-0.8/annet/adapters/netbox/v24/api_models.py` & `annet-0.9/annet/adapters/netbox/v24/api_models.py`

 * *Files identical despite different names*

### Comparing `annet-0.8/annet/adapters/netbox/v24/client.py` & `annet-0.9/annet/adapters/netbox/v24/client.py`

 * *Files identical despite different names*

### Comparing `annet-0.8/annet/adapters/netbox/v24/storage.py` & `annet-0.9/annet/adapters/netbox/v24/storage.py`

 * *Files identical despite different names*

### Comparing `annet-0.8/annet/adapters/netbox/v37/api_models.py` & `annet-0.9/annet/adapters/netbox/v37/api_models.py`

 * *Files identical despite different names*

### Comparing `annet-0.8/annet/adapters/netbox/v37/client.py` & `annet-0.9/annet/adapters/netbox/v37/client.py`

 * *Files identical despite different names*

### Comparing `annet-0.8/annet/adapters/netbox/v37/storage.py` & `annet-0.9/annet/adapters/netbox/v37/storage.py`

 * *Files identical despite different names*

### Comparing `annet-0.8/annet/annet.py` & `annet-0.9/annet/annet.py`

 * *Files identical despite different names*

### Comparing `annet-0.8/annet/annlib/command.py` & `annet-0.9/annet/annlib/command.py`

 * *Files identical despite different names*

### Comparing `annet-0.8/annet/annlib/diff.py` & `annet-0.9/annet/annlib/diff.py`

 * *Files identical despite different names*

### Comparing `annet-0.8/annet/annlib/filter_acl.py` & `annet-0.9/annet/annlib/filter_acl.py`

 * *Files identical despite different names*

### Comparing `annet-0.8/annet/annlib/jsontools.py` & `annet-0.9/annet/annlib/jsontools.py`

 * *Files 2% similar despite different names*

```diff
@@ -102,11 +102,11 @@
                 if i not in sub_tree:
                     sub_tree[i] = {}
                 sub_tree = sub_tree[i]
 
             patch = jsonpatch.JsonPatch([{"op": "add", "path": f, "value": part}])
             result = patch.apply(result)
         except jsonpointer.JsonPointerException:
-            # no value found in new_fragment by the pointer, skip the ACL item
+            # no value found in content by the pointer, skip the ACL item
             continue
 
     return result
```

### Comparing `annet-0.8/annet/annlib/lib.py` & `annet-0.9/annet/annlib/lib.py`

 * *Files identical despite different names*

### Comparing `annet-0.8/annet/annlib/netdev/db.py` & `annet-0.9/annet/annlib/netdev/db.py`

 * *Files identical despite different names*

### Comparing `annet-0.8/annet/annlib/netdev/devdb/__init__.py` & `annet-0.9/annet/annlib/netdev/devdb/__init__.py`

 * *Files identical despite different names*

### Comparing `annet-0.8/annet/annlib/netdev/devdb/data/devdb.json` & `annet-0.9/annet/annlib/netdev/devdb/data/devdb.json`

 * *Files identical despite different names*

### Comparing `annet-0.8/annet/annlib/netdev/views/dump.py` & `annet-0.9/annet/annlib/netdev/views/dump.py`

 * *Files identical despite different names*

### Comparing `annet-0.8/annet/annlib/netdev/views/hardware.py` & `annet-0.9/annet/annlib/netdev/views/hardware.py`

 * *Files identical despite different names*

### Comparing `annet-0.8/annet/annlib/output.py` & `annet-0.9/annet/annlib/output.py`

 * *Files identical despite different names*

### Comparing `annet-0.8/annet/annlib/patching.py` & `annet-0.9/annet/annlib/patching.py`

 * *Files identical despite different names*

### Comparing `annet-0.8/annet/annlib/rbparser/acl.py` & `annet-0.9/annet/annlib/rbparser/acl.py`

 * *Files identical despite different names*

### Comparing `annet-0.8/annet/annlib/rbparser/deploying.py` & `annet-0.9/annet/annlib/rbparser/deploying.py`

 * *Files identical despite different names*

### Comparing `annet-0.8/annet/annlib/rbparser/ordering.py` & `annet-0.9/annet/annlib/rbparser/ordering.py`

 * *Files identical despite different names*

### Comparing `annet-0.8/annet/annlib/rbparser/platform.py` & `annet-0.9/annet/annlib/rbparser/platform.py`

 * *Files identical despite different names*

### Comparing `annet-0.8/annet/annlib/rbparser/syntax.py` & `annet-0.9/annet/annlib/rbparser/syntax.py`

 * *Files identical despite different names*

### Comparing `annet-0.8/annet/annlib/rulebook/common.py` & `annet-0.9/annet/annlib/rulebook/common.py`

 * *Files identical despite different names*

### Comparing `annet-0.8/annet/annlib/tabparser.py` & `annet-0.9/annet/annlib/tabparser.py`

 * *Files identical despite different names*

### Comparing `annet-0.8/annet/annlib/types.py` & `annet-0.9/annet/annlib/types.py`

 * *Files identical despite different names*

### Comparing `annet-0.8/annet/api/__init__.py` & `annet-0.9/annet/api/__init__.py`

 * *Files identical despite different names*

### Comparing `annet-0.8/annet/argparse.py` & `annet-0.9/annet/argparse.py`

 * *Files identical despite different names*

### Comparing `annet-0.8/annet/cli.py` & `annet-0.9/annet/cli.py`

 * *Files identical despite different names*

### Comparing `annet-0.8/annet/cli_args.py` & `annet-0.9/annet/cli_args.py`

 * *Files identical despite different names*

### Comparing `annet-0.8/annet/configs/logging.yaml` & `annet-0.9/annet/configs/logging.yaml`

 * *Files identical despite different names*

### Comparing `annet-0.8/annet/connectors.py` & `annet-0.9/annet/connectors.py`

 * *Files identical despite different names*

### Comparing `annet-0.8/annet/deploy.py` & `annet-0.9/annet/deploy.py`

 * *Files identical despite different names*

### Comparing `annet-0.8/annet/diff.py` & `annet-0.9/annet/diff.py`

 * *Files identical despite different names*

### Comparing `annet-0.8/annet/executor.py` & `annet-0.9/annet/executor.py`

 * *Files identical despite different names*

### Comparing `annet-0.8/annet/filtering.py` & `annet-0.9/annet/filtering.py`

 * *Files identical despite different names*

### Comparing `annet-0.8/annet/gen.py` & `annet-0.9/annet/gen.py`

 * *Files 1% similar despite different names*

```diff
@@ -212,14 +212,15 @@
         try:
             old_files = _old_new_get_config_files(ctx, device)
         except Exception as exc:
             return OldNewResult(device=device, err=exc)
 
     new_files = {}
     safe_new_files = {}
+    safe_new_json_fragment_files = {}
     if not ctx.no_new:
         if device in ctx.fetched_packages:
             if ctx.args.required_packages_check:
                 errors = generators.check_entire_generators_required_packages(ctx.gens.entire[device.fqdn],
                                                                               ctx.fetched_packages[device])
                 if errors:
                     error_msg = "; ".join(errors)
@@ -234,31 +235,42 @@
         entire_results = res.entire_results
         json_fragment_results = res.json_fragment_results
         old_json_fragment_files = old_files.json_fragment_files
 
         new_files = res.new_files()
         new_json_fragment_files = res.new_json_fragment_files(old_json_fragment_files)
 
+        filters: List[str] = []
+        filters_text = build_filter_text(filterer, device, ctx.stdin, ctx.args, ctx.config)
+        if filters_text:
+            filters = filters_text.split("\n")
+
+            for file_name in new_json_fragment_files:
+                new_json_fragment_files = _update_json_config(
+                    new_json_fragment_files,
+                    file_name,
+                    jsontools.apply_acl_filters(new_json_fragment_files[file_name][0], filters)
+                )
+            for file_name in old_json_fragment_files:
+                old_json_fragment_files = _update_json_config(
+                    old_json_fragment_files,
+                    file_name,
+                    jsontools.apply_acl_filters(old_json_fragment_files[file_name][0], filters)
+                )
+
         if ctx.args.acl_safe:
             safe_new_files = res.new_files(safe=True)
-
-        filters = build_filter_text(filterer, device, ctx.stdin, ctx.args, ctx.config).split("\n")
-
-        for file_name in new_json_fragment_files:
-            new_json_fragment_files = _update_json_config(
-                new_json_fragment_files,
-                file_name,
-                jsontools.apply_acl_filters(new_json_fragment_files[file_name][0], filters)
-            )
-        for file_name in old_json_fragment_files:
-            old_json_fragment_files = _update_json_config(
-                old_json_fragment_files,
-                file_name,
-                jsontools.apply_acl_filters(old_json_fragment_files[file_name][0], filters)
-            )
+            safe_new_json_fragment_files = res.new_json_fragment_files(old_json_fragment_files, safe=True)
+            if filters:
+                for file_name in safe_new_json_fragment_files:
+                    safe_new_json_fragment_files = _update_json_config(
+                        safe_new_json_fragment_files,
+                        file_name,
+                        jsontools.apply_acl_filters(safe_new_json_fragment_files[file_name][0], filters)
+                    )
 
     if ctx.args.profile:
         perf = res.perf_mesures()
         combined_perf[ALL_GENS] = {"total": time.monotonic() - start}
         combined_perf.update(perf)
         if ctx.do_print_perf:
             _print_perf("ENTIRE", perf)
@@ -277,14 +289,15 @@
         json_fragment_result=json_fragment_results,
         implicit_rules=implicit_rules,
         perf=combined_perf,
         acl_safe_rules=acl_safe_rules,
         safe_old=safe_old,
         safe_new=safe_new,
         safe_new_files=safe_new_files,
+        safe_new_json_fragment_files=safe_new_json_fragment_files,
         filter_acl_rules=filter_acl_rules,
     )
 
 
 def _update_json_config(json_files, file_name, new_config):
     file = list(json_files[file_name])
     file[0] = new_config
```

### Comparing `annet-0.8/annet/generators/__init__.py` & `annet-0.9/annet/generators/__init__.py`

 * *Files 1% similar despite different names*

```diff
@@ -176,29 +176,33 @@
 
     def acl_safe_text(self) -> str:
         return _combine_acl_text(self.partial_results, lambda gr: gr.acl_safe)
 
     def new_json_fragment_files(
             self,
             old_files: Dict[str, Optional[str]],
-            safe: bool = False,  # pylint: disable=unused-argument
+            safe: bool = False,
     ) -> Dict[str, Tuple[Any, Optional[str]]]:
-        # TODO: safe
         files: Dict[str, Tuple[Any, Optional[str]]] = {}
         reload_prios: Dict[str, int] = {}
         for generator_result in self.json_fragment_results.values():
             filepath = generator_result.path
             if filepath not in files:
                 if old_files.get(filepath) is not None:
                     files[filepath] = (old_files[filepath], None)
                 else:
                     files[filepath] = ({}, None)
             previous_config: Dict[str, Any] = files[filepath][0]
             new_fragment = generator_result.config
-            new_config = jsontools.apply_json_fragment(previous_config, new_fragment, generator_result.acl)
+
+            if safe:
+                new_config = jsontools.apply_json_fragment(previous_config, new_fragment, generator_result.acl_safe)
+            else:
+                new_config = jsontools.apply_json_fragment(previous_config, new_fragment, generator_result.acl)
+
             if filepath in reload_prios and reload_prios[filepath] > generator_result.reload_prio:
                 _, reload_cmd = files[filepath]
             else:
                 reload_cmd = generator_result.reload
                 reload_prios[filepath] = generator_result.reload_prio
             files[filepath] = (new_config, reload_cmd)
         return files
@@ -498,34 +502,39 @@
         logger.info("generator %s is not supported for device %s", gen, device.hostname)
 
     path = gen.path(device)
     if not path:
         raise RuntimeError("json fragment generator should return non-empty path")
 
     acl_item_or_list_of_items = gen.acl(device)
+    safe_acl_item_or_list_of_items = gen.acl_safe(device)
     if not acl_item_or_list_of_items:
         raise RuntimeError("json fragment generator should return non-empty acl")
     if isinstance(acl_item_or_list_of_items, list):
         acl = acl_item_or_list_of_items
     else:
         acl = [acl_item_or_list_of_items]
+    if isinstance(safe_acl_item_or_list_of_items, list):
+        acl_safe = safe_acl_item_or_list_of_items
+    else:
+        acl_safe = [safe_acl_item_or_list_of_items]
 
     logger.info("Generating JSON_FRAGMENT ...")
     with GeneratorPerfMesurer(gen, storage) as pm:
         config = gen(device)
     reload_cmds = gen.get_reload_cmds(device)
     return GeneratorJSONFragmentResult(
         name=gen.__class__.__name__,
         tags=gen.TAGS,
         path=path,
         acl=acl,
+        acl_safe=acl_safe,
         config=config,
         reload=reload_cmds,
         perf=pm.last_result,
-        is_safe=gen.is_safe(device),
         reload_prio=gen.reload_prio,
     )
 
 
 def _get_generators(module_paths: Union[List[str], dict], storage, device=None):
     if isinstance(module_paths, dict):
         if device is None:
@@ -931,22 +940,25 @@
         """
         Restrict the generator to a specified ACL using JSON Pointer syntax.
 
         Expected ACL to be a list of strings, but a single string is also allowed.
         """
         raise NotImplementedError("Required ACL for JSON_FRAGMENT generator")
 
+    def acl_safe(self, device: Device) -> Union[str, List[str]]:
+        """
+        Restrict the generator to a specified safe ACL using JSON Pointer syntax.
+
+        Expected ACL to be a list of strings, but a single string is also allowed.
+        """
+        raise NotImplementedError("Required ACL for JSON_FRAGMENT generator")
+
     def run(self, device: Device):
         raise NotImplementedError
 
-    # pylint: disable=unused-argument
-    def is_safe(self, device: Device) -> bool:
-        """Output gen results when --acl-safe flag is used"""
-        return False
-
     def get_reload_cmds(self, device: Device) -> str:
         ret = self.reload(device) or ""
         return ret
 
     def reload(self, device) -> Optional[str]:
         raise NotImplementedError
```

### Comparing `annet-0.8/annet/generators/common/initial.py` & `annet-0.9/annet/generators/common/initial.py`

 * *Files identical despite different names*

### Comparing `annet-0.8/annet/hardware.py` & `annet-0.9/annet/hardware.py`

 * *Files identical despite different names*

### Comparing `annet-0.8/annet/implicit.py` & `annet-0.9/annet/implicit.py`

 * *Files identical despite different names*

### Comparing `annet-0.8/annet/lib.py` & `annet-0.9/annet/lib.py`

 * *Files identical despite different names*

### Comparing `annet-0.8/annet/output.py` & `annet-0.9/annet/output.py`

 * *Files identical despite different names*

### Comparing `annet-0.8/annet/parallel.py` & `annet-0.9/annet/parallel.py`

 * *Files identical despite different names*

### Comparing `annet-0.8/annet/patching.py` & `annet-0.9/annet/patching.py`

 * *Files identical despite different names*

### Comparing `annet-0.8/annet/reference.py` & `annet-0.9/annet/reference.py`

 * *Files identical despite different names*

### Comparing `annet-0.8/annet/rulebook/__init__.py` & `annet-0.9/annet/rulebook/__init__.py`

 * *Files identical despite different names*

### Comparing `annet-0.8/annet/rulebook/arista/iface.py` & `annet-0.9/annet/rulebook/arista/iface.py`

 * *Files identical despite different names*

### Comparing `annet-0.8/annet/rulebook/aruba/ap_env.py` & `annet-0.9/annet/rulebook/aruba/ap_env.py`

 * *Files identical despite different names*

### Comparing `annet-0.8/annet/rulebook/cisco/iface.py` & `annet-0.9/annet/rulebook/cisco/iface.py`

 * *Files identical despite different names*

### Comparing `annet-0.8/annet/rulebook/cisco/misc.py` & `annet-0.9/annet/rulebook/cisco/misc.py`

 * *Files identical despite different names*

### Comparing `annet-0.8/annet/rulebook/cisco/vlandb.py` & `annet-0.9/annet/rulebook/cisco/vlandb.py`

 * *Files identical despite different names*

### Comparing `annet-0.8/annet/rulebook/common.py` & `annet-0.9/annet/rulebook/common.py`

 * *Files identical despite different names*

### Comparing `annet-0.8/annet/rulebook/deploying.py` & `annet-0.9/annet/rulebook/deploying.py`

 * *Files identical despite different names*

### Comparing `annet-0.8/annet/rulebook/huawei/aaa.py` & `annet-0.9/annet/rulebook/huawei/aaa.py`

 * *Files identical despite different names*

### Comparing `annet-0.8/annet/rulebook/huawei/bgp.py` & `annet-0.9/annet/rulebook/huawei/bgp.py`

 * *Files identical despite different names*

### Comparing `annet-0.8/annet/rulebook/huawei/iface.py` & `annet-0.9/annet/rulebook/huawei/iface.py`

 * *Files identical despite different names*

### Comparing `annet-0.8/annet/rulebook/huawei/misc.py` & `annet-0.9/annet/rulebook/huawei/misc.py`

 * *Files identical despite different names*

### Comparing `annet-0.8/annet/rulebook/huawei/vlandb.py` & `annet-0.9/annet/rulebook/huawei/vlandb.py`

 * *Files identical despite different names*

### Comparing `annet-0.8/annet/rulebook/juniper/__init__.py` & `annet-0.9/annet/rulebook/juniper/__init__.py`

 * *Files identical despite different names*

### Comparing `annet-0.8/annet/rulebook/nexus/iface.py` & `annet-0.9/annet/rulebook/nexus/iface.py`

 * *Files identical despite different names*

### Comparing `annet-0.8/annet/rulebook/patching.py` & `annet-0.9/annet/rulebook/patching.py`

 * *Files identical despite different names*

### Comparing `annet-0.8/annet/rulebook/texts/arista.deploy` & `annet-0.9/annet/rulebook/texts/arista.deploy`

 * *Files identical despite different names*

### Comparing `annet-0.8/annet/rulebook/texts/arista.order` & `annet-0.9/annet/rulebook/texts/arista.order`

 * *Files identical despite different names*

### Comparing `annet-0.8/annet/rulebook/texts/arista.rul` & `annet-0.9/annet/rulebook/texts/arista.rul`

 * *Files identical despite different names*

### Comparing `annet-0.8/annet/rulebook/texts/aruba.deploy` & `annet-0.9/annet/rulebook/texts/aruba.deploy`

 * *Files identical despite different names*

### Comparing `annet-0.8/annet/rulebook/texts/aruba.order` & `annet-0.9/annet/rulebook/texts/aruba.order`

 * *Files identical despite different names*

### Comparing `annet-0.8/annet/rulebook/texts/aruba.rul` & `annet-0.9/annet/rulebook/texts/aruba.rul`

 * *Files identical despite different names*

### Comparing `annet-0.8/annet/rulebook/texts/cisco.deploy` & `annet-0.9/annet/rulebook/texts/cisco.deploy`

 * *Files identical despite different names*

### Comparing `annet-0.8/annet/rulebook/texts/cisco.order` & `annet-0.9/annet/rulebook/texts/cisco.order`

 * *Files identical despite different names*

### Comparing `annet-0.8/annet/rulebook/texts/cisco.rul` & `annet-0.9/annet/rulebook/texts/cisco.rul`

 * *Files identical despite different names*

### Comparing `annet-0.8/annet/rulebook/texts/huawei.deploy` & `annet-0.9/annet/rulebook/texts/huawei.deploy`

 * *Files identical despite different names*

### Comparing `annet-0.8/annet/rulebook/texts/huawei.order` & `annet-0.9/annet/rulebook/texts/huawei.order`

 * *Files identical despite different names*

### Comparing `annet-0.8/annet/rulebook/texts/huawei.rul` & `annet-0.9/annet/rulebook/texts/huawei.rul`

 * *Files identical despite different names*

### Comparing `annet-0.8/annet/rulebook/texts/juniper.rul` & `annet-0.9/annet/rulebook/texts/juniper.rul`

 * *Files identical despite different names*

### Comparing `annet-0.8/annet/rulebook/texts/nexus.deploy` & `annet-0.9/annet/rulebook/texts/nexus.deploy`

 * *Files identical despite different names*

### Comparing `annet-0.8/annet/rulebook/texts/nexus.order` & `annet-0.9/annet/rulebook/texts/nexus.order`

 * *Files identical despite different names*

### Comparing `annet-0.8/annet/rulebook/texts/nexus.rul` & `annet-0.9/annet/rulebook/texts/nexus.rul`

 * *Files identical despite different names*

### Comparing `annet-0.8/annet/rulebook/texts/nokia.rul` & `annet-0.9/annet/rulebook/texts/nokia.rul`

 * *Files identical despite different names*

### Comparing `annet-0.8/annet/rulebook/texts/ribbon.deploy` & `annet-0.9/annet/rulebook/texts/ribbon.deploy`

 * *Files identical despite different names*

### Comparing `annet-0.8/annet/rulebook/texts/ribbon.rul` & `annet-0.9/annet/rulebook/texts/ribbon.rul`

 * *Files identical despite different names*

### Comparing `annet-0.8/annet/rulebook/texts/routeros.order` & `annet-0.9/annet/rulebook/texts/routeros.order`

 * *Files identical despite different names*

### Comparing `annet-0.8/annet/rulebook/texts/routeros.rul` & `annet-0.9/annet/rulebook/texts/routeros.rul`

 * *Files identical despite different names*

### Comparing `annet-0.8/annet/storage.py` & `annet-0.9/annet/storage.py`

 * *Files identical despite different names*

### Comparing `annet-0.8/annet/tabparser.py` & `annet-0.9/annet/tabparser.py`

 * *Files identical despite different names*

### Comparing `annet-0.8/annet/text_term_format.py` & `annet-0.9/annet/text_term_format.py`

 * *Files identical despite different names*

### Comparing `annet-0.8/annet/tracing.py` & `annet-0.9/annet/tracing.py`

 * *Files identical despite different names*

### Comparing `annet-0.8/annet/types.py` & `annet-0.9/annet/types.py`

 * *Files 2% similar despite different names*

```diff
@@ -122,28 +122,28 @@
 
     def __init__(
         self,
         name: str,
         tags: List[str],
         path: str,
         acl: List[str],
+        acl_safe: List[str],
         config: Dict[str, Any],
         reload: str,
         perf: GeneratorPerf,
-        is_safe: bool,
         reload_prio: int,
     ):
         self.name = name
         self.tags = tags
         self.path = path
         self.acl = acl
+        self.acl_safe = acl_safe
         self.config = config
         self.reload = reload
         self.perf = perf
-        self.is_safe = is_safe
         self.reload_prio = reload_prio
 
 
 GeneratorResult = Union[GeneratorEntireResult, GeneratorPartialResult, GeneratorJSONFragmentResult]
 
 
 class OldNewResult:
@@ -167,14 +167,15 @@
         json_fragment_result=None,
         implicit_rules=None,
         perf=None,
         acl_safe_rules=None,
         safe_old=None,
         safe_new=None,
         safe_new_files=None,
+        safe_new_json_fragment_files=None,
         filter_acl_rules=None
     ):
         self.device: Device = device
         self.old: MutableMapping = old if old else OrderedDict()
         self.new: MutableMapping = new if new else OrderedDict()
         self.acl_rules: MutableMapping = acl_rules
         self.new_files: MutableMapping = new_files if new_files else {}
@@ -189,14 +190,15 @@
         self.perf: Dict[str, Dict[str, float]] = perf or {}
 
         # safe acl and configs with it applied
         self.acl_safe_rules: MutableMapping = acl_safe_rules or {}
         self.safe_old: MutableMapping = safe_old if safe_old else OrderedDict()
         self.safe_new: MutableMapping = safe_new if safe_new else OrderedDict()
         self.safe_new_files: MutableMapping = safe_new_files if safe_new_files else {}
+        self.safe_new_json_fragment_files: MutableMapping = safe_new_json_fragment_files or {}
 
         self.filter_acl_rules: Optional[MutableMapping] = filter_acl_rules
 
     def get_old(self, safe: bool = False) -> MutableMapping:
         if safe:
             return self.safe_old
 
@@ -217,9 +219,11 @@
     def get_new_files(self, safe: bool = False) -> MutableMapping:
         if safe:
             return self.safe_new_files
 
         return self.new_files
 
     def get_new_file_fragments(self, safe: bool = False) -> Dict[str, Tuple[Any, Optional[str]]]:  # pylint: disable=unused-argument
-        # TODO: safe
+        if safe:
+            return self.safe_new_json_fragment_files
+
         return self.new_json_fragment_files
```

### Comparing `annet-0.8/annet.egg-info/PKG-INFO` & `annet-0.9/annet.egg-info/PKG-INFO`

 * *Files 7% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: annet
-Version: 0.8
+Version: 0.9
 Summary: annet
 Home-page: https://github.com/annetutil/annet
 License: MIT
 Requires-Python: >=3.8
 License-File: LICENSE
 License-File: AUTHORS
 Requires-Dist: colorama>=0.4.6
```

### Comparing `annet-0.8/annet.egg-info/SOURCES.txt` & `annet-0.9/annet.egg-info/SOURCES.txt`

 * *Files identical despite different names*

### Comparing `annet-0.8/annet_generators/example/lldp.py` & `annet-0.9/annet_generators/example/lldp.py`

 * *Files identical despite different names*

### Comparing `annet-0.8/setup.py` & `annet-0.9/setup.py`

 * *Files identical despite different names*

