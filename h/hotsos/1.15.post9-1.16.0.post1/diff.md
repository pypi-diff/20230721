# Comparing `tmp/hotsos-1.15.post9.tar.gz` & `tmp/hotsos-1.16.0.post1.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "hotsos-1.15.post9.tar", last modified: Thu Jul  6 09:00:02 2023, max compression
+gzip compressed data, was "hotsos-1.16.0.post1.tar", last modified: Fri Jul 21 07:19:29 2023, max compression
```

## Comparing `hotsos-1.15.post9.tar` & `hotsos-1.16.0.post1.tar`

### file list

```diff
@@ -1,409 +1,410 @@
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-06 09:00:02.430256 hotsos-1.15.post9/
--rw-r--r--   0 runner    (1001) docker     (123)    11357 2023-07-06 08:59:40.000000 hotsos-1.15.post9/LICENSE
--rw-r--r--   0 runner    (1001) docker     (123)      102 2023-07-06 08:59:40.000000 hotsos-1.15.post9/MANIFEST.in
--rw-r--r--   0 runner    (1001) docker     (123)     1193 2023-07-06 09:00:02.430256 hotsos-1.15.post9/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (123)      908 2023-07-06 08:59:40.000000 hotsos-1.15.post9/README.md
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-06 09:00:02.394256 hotsos-1.15.post9/hotsos/
--rw-r--r--   0 runner    (1001) docker     (123)        9 2023-07-06 08:59:45.000000 hotsos-1.15.post9/hotsos/.repo-info
--rw-r--r--   0 runner    (1001) docker     (123)        0 2023-07-06 08:59:40.000000 hotsos-1.15.post9/hotsos/__init__.py
--rwxr-xr-x   0 runner    (1001) docker     (123)    15110 2023-07-06 08:59:40.000000 hotsos-1.15.post9/hotsos/cli.py
--rwxr-xr-x   0 runner    (1001) docker     (123)    15371 2023-07-06 08:59:40.000000 hotsos-1.15.post9/hotsos/client.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-06 09:00:02.398256 hotsos-1.15.post9/hotsos/core/
--rw-r--r--   0 runner    (1001) docker     (123)        0 2023-07-06 08:59:40.000000 hotsos-1.15.post9/hotsos/core/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)    10727 2023-07-06 08:59:40.000000 hotsos-1.15.post9/hotsos/core/analytics.py
--rw-r--r--   0 runner    (1001) docker     (123)    10126 2023-07-06 08:59:40.000000 hotsos-1.15.post9/hotsos/core/config.py
--rw-r--r--   0 runner    (1001) docker     (123)       46 2023-07-06 08:59:40.000000 hotsos-1.15.post9/hotsos/core/exceptions.py
--rw-r--r--   0 runner    (1001) docker     (123)      623 2023-07-06 08:59:40.000000 hotsos-1.15.post9/hotsos/core/factory.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-06 09:00:02.398256 hotsos-1.15.post9/hotsos/core/host_helpers/
--rw-r--r--   0 runner    (1001) docker     (123)      711 2023-07-06 08:59:40.000000 hotsos-1.15.post9/hotsos/core/host_helpers/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)    35388 2023-07-06 08:59:40.000000 hotsos-1.15.post9/hotsos/core/host_helpers/cli.py
--rw-r--r--   0 runner    (1001) docker     (123)     3068 2023-07-06 08:59:40.000000 hotsos-1.15.post9/hotsos/core/host_helpers/common.py
--rw-r--r--   0 runner    (1001) docker     (123)     4694 2023-07-06 08:59:40.000000 hotsos-1.15.post9/hotsos/core/host_helpers/config.py
--rw-r--r--   0 runner    (1001) docker     (123)     1245 2023-07-06 08:59:40.000000 hotsos-1.15.post9/hotsos/core/host_helpers/filestat.py
--rw-r--r--   0 runner    (1001) docker     (123)    11021 2023-07-06 08:59:40.000000 hotsos-1.15.post9/hotsos/core/host_helpers/network.py
--rw-r--r--   0 runner    (1001) docker     (123)    13241 2023-07-06 08:59:40.000000 hotsos-1.15.post9/hotsos/core/host_helpers/packaging.py
--rw-r--r--   0 runner    (1001) docker     (123)     3346 2023-07-06 08:59:40.000000 hotsos-1.15.post9/hotsos/core/host_helpers/pebble.py
--rw-r--r--   0 runner    (1001) docker     (123)     2341 2023-07-06 08:59:40.000000 hotsos-1.15.post9/hotsos/core/host_helpers/ssl.py
--rw-r--r--   0 runner    (1001) docker     (123)     2583 2023-07-06 08:59:40.000000 hotsos-1.15.post9/hotsos/core/host_helpers/sysctl.py
--rw-r--r--   0 runner    (1001) docker     (123)    11368 2023-07-06 08:59:40.000000 hotsos-1.15.post9/hotsos/core/host_helpers/systemd.py
--rw-r--r--   0 runner    (1001) docker     (123)     2673 2023-07-06 08:59:40.000000 hotsos-1.15.post9/hotsos/core/host_helpers/uptime.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-06 09:00:02.398256 hotsos-1.15.post9/hotsos/core/issues/
--rw-r--r--   0 runner    (1001) docker     (123)      126 2023-07-06 08:59:40.000000 hotsos-1.15.post9/hotsos/core/issues/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)     2961 2023-07-06 08:59:40.000000 hotsos-1.15.post9/hotsos/core/issues/issue_types.py
--rw-r--r--   0 runner    (1001) docker     (123)     5118 2023-07-06 08:59:40.000000 hotsos-1.15.post9/hotsos/core/issues/utils.py
--rw-r--r--   0 runner    (1001) docker     (123)      551 2023-07-06 08:59:40.000000 hotsos-1.15.post9/hotsos/core/log.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-06 09:00:02.398256 hotsos-1.15.post9/hotsos/core/plugins/
--rw-r--r--   0 runner    (1001) docker     (123)        0 2023-07-06 08:59:40.000000 hotsos-1.15.post9/hotsos/core/plugins/__init__.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-06 09:00:02.398256 hotsos-1.15.post9/hotsos/core/plugins/juju/
--rw-r--r--   0 runner    (1001) docker     (123)       54 2023-07-06 08:59:40.000000 hotsos-1.15.post9/hotsos/core/plugins/juju/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)     1462 2023-07-06 08:59:40.000000 hotsos-1.15.post9/hotsos/core/plugins/juju/common.py
--rw-r--r--   0 runner    (1001) docker     (123)     6396 2023-07-06 08:59:40.000000 hotsos-1.15.post9/hotsos/core/plugins/juju/resources.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-06 09:00:02.402256 hotsos-1.15.post9/hotsos/core/plugins/kernel/
--rw-r--r--   0 runner    (1001) docker     (123)      160 2023-07-06 08:59:40.000000 hotsos-1.15.post9/hotsos/core/plugins/kernel/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)     1597 2023-07-06 08:59:40.000000 hotsos-1.15.post9/hotsos/core/plugins/kernel/common.py
--rw-r--r--   0 runner    (1001) docker     (123)     1442 2023-07-06 08:59:40.000000 hotsos-1.15.post9/hotsos/core/plugins/kernel/config.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-06 09:00:02.402256 hotsos-1.15.post9/hotsos/core/plugins/kernel/kernlog/
--rw-r--r--   0 runner    (1001) docker     (123)      112 2023-07-06 08:59:40.000000 hotsos-1.15.post9/hotsos/core/plugins/kernel/kernlog/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)    14852 2023-07-06 08:59:40.000000 hotsos-1.15.post9/hotsos/core/plugins/kernel/kernlog/calltrace.py
--rw-r--r--   0 runner    (1001) docker     (123)     3835 2023-07-06 08:59:40.000000 hotsos-1.15.post9/hotsos/core/plugins/kernel/kernlog/common.py
--rw-r--r--   0 runner    (1001) docker     (123)     2487 2023-07-06 08:59:40.000000 hotsos-1.15.post9/hotsos/core/plugins/kernel/kernlog/events.py
--rw-r--r--   0 runner    (1001) docker     (123)     7491 2023-07-06 08:59:40.000000 hotsos-1.15.post9/hotsos/core/plugins/kernel/memory.py
--rw-r--r--   0 runner    (1001) docker     (123)    20366 2023-07-06 08:59:40.000000 hotsos-1.15.post9/hotsos/core/plugins/kernel/net.py
--rw-r--r--   0 runner    (1001) docker     (123)     2019 2023-07-06 08:59:40.000000 hotsos-1.15.post9/hotsos/core/plugins/kernel/sysfs.py
--rw-r--r--   0 runner    (1001) docker     (123)     3463 2023-07-06 08:59:40.000000 hotsos-1.15.post9/hotsos/core/plugins/kubernetes.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-06 09:00:02.402256 hotsos-1.15.post9/hotsos/core/plugins/lxd/
--rw-r--r--   0 runner    (1001) docker     (123)       58 2023-07-06 08:59:40.000000 hotsos-1.15.post9/hotsos/core/plugins/lxd/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)     1798 2023-07-06 08:59:40.000000 hotsos-1.15.post9/hotsos/core/plugins/lxd/common.py
--rw-r--r--   0 runner    (1001) docker     (123)      973 2023-07-06 08:59:40.000000 hotsos-1.15.post9/hotsos/core/plugins/maas.py
--rw-r--r--   0 runner    (1001) docker     (123)     1385 2023-07-06 08:59:40.000000 hotsos-1.15.post9/hotsos/core/plugins/mysql.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-06 09:00:02.402256 hotsos-1.15.post9/hotsos/core/plugins/openstack/
--rw-r--r--   0 runner    (1001) docker     (123)      175 2023-07-06 08:59:40.000000 hotsos-1.15.post9/hotsos/core/plugins/openstack/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)     8193 2023-07-06 08:59:40.000000 hotsos-1.15.post9/hotsos/core/plugins/openstack/common.py
--rw-r--r--   0 runner    (1001) docker     (123)    63860 2023-07-06 08:59:40.000000 hotsos-1.15.post9/hotsos/core/plugins/openstack/exceptions.py
--rw-r--r--   0 runner    (1001) docker     (123)     3799 2023-07-06 08:59:40.000000 hotsos-1.15.post9/hotsos/core/plugins/openstack/neutron.py
--rw-r--r--   0 runner    (1001) docker     (123)    10636 2023-07-06 08:59:40.000000 hotsos-1.15.post9/hotsos/core/plugins/openstack/nova.py
--rw-r--r--   0 runner    (1001) docker     (123)     1480 2023-07-06 08:59:40.000000 hotsos-1.15.post9/hotsos/core/plugins/openstack/octavia.py
--rw-r--r--   0 runner    (1001) docker     (123)    19464 2023-07-06 08:59:40.000000 hotsos-1.15.post9/hotsos/core/plugins/openstack/openstack.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-06 09:00:02.402256 hotsos-1.15.post9/hotsos/core/plugins/openvswitch/
--rw-r--r--   0 runner    (1001) docker     (123)      166 2023-07-06 08:59:40.000000 hotsos-1.15.post9/hotsos/core/plugins/openvswitch/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)     2276 2023-07-06 08:59:40.000000 hotsos-1.15.post9/hotsos/core/plugins/openvswitch/common.py
--rw-r--r--   0 runner    (1001) docker     (123)     4809 2023-07-06 08:59:40.000000 hotsos-1.15.post9/hotsos/core/plugins/openvswitch/ovn.py
--rw-r--r--   0 runner    (1001) docker     (123)     4804 2023-07-06 08:59:40.000000 hotsos-1.15.post9/hotsos/core/plugins/openvswitch/ovs.py
--rw-r--r--   0 runner    (1001) docker     (123)     1636 2023-07-06 08:59:40.000000 hotsos-1.15.post9/hotsos/core/plugins/pacemaker.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-06 09:00:02.402256 hotsos-1.15.post9/hotsos/core/plugins/rabbitmq/
--rw-r--r--   0 runner    (1001) docker     (123)      112 2023-07-06 08:59:40.000000 hotsos-1.15.post9/hotsos/core/plugins/rabbitmq/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)      947 2023-07-06 08:59:40.000000 hotsos-1.15.post9/hotsos/core/plugins/rabbitmq/common.py
--rw-r--r--   0 runner    (1001) docker     (123)     9001 2023-07-06 08:59:40.000000 hotsos-1.15.post9/hotsos/core/plugins/rabbitmq/report.py
--rw-r--r--   0 runner    (1001) docker     (123)     1801 2023-07-06 08:59:40.000000 hotsos-1.15.post9/hotsos/core/plugins/sosreport.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-06 09:00:02.402256 hotsos-1.15.post9/hotsos/core/plugins/storage/
--rw-r--r--   0 runner    (1001) docker     (123)       94 2023-07-06 08:59:40.000000 hotsos-1.15.post9/hotsos/core/plugins/storage/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)     6042 2023-07-06 08:59:40.000000 hotsos-1.15.post9/hotsos/core/plugins/storage/bcache.py
--rw-r--r--   0 runner    (1001) docker     (123)    38316 2023-07-06 08:59:40.000000 hotsos-1.15.post9/hotsos/core/plugins/storage/ceph.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-06 09:00:02.402256 hotsos-1.15.post9/hotsos/core/plugins/system/
--rw-r--r--   0 runner    (1001) docker     (123)       68 2023-07-06 08:59:40.000000 hotsos-1.15.post9/hotsos/core/plugins/system/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)      246 2023-07-06 08:59:40.000000 hotsos-1.15.post9/hotsos/core/plugins/system/common.py
--rw-r--r--   0 runner    (1001) docker     (123)     6752 2023-07-06 08:59:40.000000 hotsos-1.15.post9/hotsos/core/plugins/system/system.py
--rw-r--r--   0 runner    (1001) docker     (123)      806 2023-07-06 08:59:40.000000 hotsos-1.15.post9/hotsos/core/plugins/vault.py
--rw-r--r--   0 runner    (1001) docker     (123)    13833 2023-07-06 08:59:40.000000 hotsos-1.15.post9/hotsos/core/plugintools.py
--rw-r--r--   0 runner    (1001) docker     (123)     2416 2023-07-06 08:59:40.000000 hotsos-1.15.post9/hotsos/core/search.py
--rw-r--r--   0 runner    (1001) docker     (123)     2268 2023-07-06 08:59:40.000000 hotsos-1.15.post9/hotsos/core/utils.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-06 09:00:02.406256 hotsos-1.15.post9/hotsos/core/ycheck/
--rw-r--r--   0 runner    (1001) docker     (123)       59 2023-07-06 08:59:40.000000 hotsos-1.15.post9/hotsos/core/ycheck/__init__.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-06 09:00:02.406256 hotsos-1.15.post9/hotsos/core/ycheck/engine/
--rw-r--r--   0 runner    (1001) docker     (123)      134 2023-07-06 08:59:40.000000 hotsos-1.15.post9/hotsos/core/ycheck/engine/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)     4094 2023-07-06 08:59:40.000000 hotsos-1.15.post9/hotsos/core/ycheck/engine/common.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-06 09:00:02.406256 hotsos-1.15.post9/hotsos/core/ycheck/engine/properties/
--rw-r--r--   0 runner    (1001) docker     (123)      443 2023-07-06 08:59:40.000000 hotsos-1.15.post9/hotsos/core/ycheck/engine/properties/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)     6252 2023-07-06 08:59:40.000000 hotsos-1.15.post9/hotsos/core/ycheck/engine/properties/checks.py
--rw-r--r--   0 runner    (1001) docker     (123)    24973 2023-07-06 08:59:40.000000 hotsos-1.15.post9/hotsos/core/ycheck/engine/properties/common.py
--rw-r--r--   0 runner    (1001) docker     (123)     7608 2023-07-06 08:59:40.000000 hotsos-1.15.post9/hotsos/core/ycheck/engine/properties/conclusions.py
--rw-r--r--   0 runner    (1001) docker     (123)     3251 2023-07-06 08:59:40.000000 hotsos-1.15.post9/hotsos/core/ycheck/engine/properties/inputdef.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-06 09:00:02.406256 hotsos-1.15.post9/hotsos/core/ycheck/engine/properties/requires/
--rw-r--r--   0 runner    (1001) docker     (123)      215 2023-07-06 08:59:40.000000 hotsos-1.15.post9/hotsos/core/ycheck/engine/properties/requires/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)     7537 2023-07-06 08:59:40.000000 hotsos-1.15.post9/hotsos/core/ycheck/engine/properties/requires/common.py
--rw-r--r--   0 runner    (1001) docker     (123)     2378 2023-07-06 08:59:40.000000 hotsos-1.15.post9/hotsos/core/ycheck/engine/properties/requires/requires.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-06 09:00:02.406256 hotsos-1.15.post9/hotsos/core/ycheck/engine/properties/requires/types/
--rw-r--r--   0 runner    (1001) docker     (123)        0 2023-07-06 08:59:40.000000 hotsos-1.15.post9/hotsos/core/ycheck/engine/properties/requires/types/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)     2927 2023-07-06 08:59:40.000000 hotsos-1.15.post9/hotsos/core/ycheck/engine/properties/requires/types/apt.py
--rw-r--r--   0 runner    (1001) docker     (123)     5906 2023-07-06 08:59:40.000000 hotsos-1.15.post9/hotsos/core/ycheck/engine/properties/requires/types/config.py
--rw-r--r--   0 runner    (1001) docker     (123)     1296 2023-07-06 08:59:40.000000 hotsos-1.15.post9/hotsos/core/ycheck/engine/properties/requires/types/path.py
--rw-r--r--   0 runner    (1001) docker     (123)     2628 2023-07-06 08:59:40.000000 hotsos-1.15.post9/hotsos/core/ycheck/engine/properties/requires/types/pebble.py
--rw-r--r--   0 runner    (1001) docker     (123)      938 2023-07-06 08:59:40.000000 hotsos-1.15.post9/hotsos/core/ycheck/engine/properties/requires/types/property.py
--rw-r--r--   0 runner    (1001) docker     (123)     2384 2023-07-06 08:59:40.000000 hotsos-1.15.post9/hotsos/core/ycheck/engine/properties/requires/types/snap.py
--rw-r--r--   0 runner    (1001) docker     (123)     5034 2023-07-06 08:59:40.000000 hotsos-1.15.post9/hotsos/core/ycheck/engine/properties/requires/types/systemd.py
--rw-r--r--   0 runner    (1001) docker     (123)      927 2023-07-06 08:59:40.000000 hotsos-1.15.post9/hotsos/core/ycheck/engine/properties/requires/types/varops.py
--rw-r--r--   0 runner    (1001) docker     (123)    16533 2023-07-06 08:59:40.000000 hotsos-1.15.post9/hotsos/core/ycheck/engine/properties/search.py
--rw-r--r--   0 runner    (1001) docker     (123)     2961 2023-07-06 08:59:40.000000 hotsos-1.15.post9/hotsos/core/ycheck/engine/properties/vardef.py
--rw-r--r--   0 runner    (1001) docker     (123)    14358 2023-07-06 08:59:40.000000 hotsos-1.15.post9/hotsos/core/ycheck/events.py
--rw-r--r--   0 runner    (1001) docker     (123)     5179 2023-07-06 08:59:40.000000 hotsos-1.15.post9/hotsos/core/ycheck/scenarios.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-06 09:00:02.390256 hotsos-1.15.post9/hotsos/defs/
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-06 09:00:02.390256 hotsos-1.15.post9/hotsos/defs/events/
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-06 09:00:02.406256 hotsos-1.15.post9/hotsos/defs/events/openstack/
--rw-r--r--   0 runner    (1001) docker     (123)      240 2023-07-06 08:59:40.000000 hotsos-1.15.post9/hotsos/defs/events/openstack/apache.yaml
--rw-r--r--   0 runner    (1001) docker     (123)      287 2023-07-06 08:59:40.000000 hotsos-1.15.post9/hotsos/defs/events/openstack/apparmor.yaml
--rw-r--r--   0 runner    (1001) docker     (123)      375 2023-07-06 08:59:40.000000 hotsos-1.15.post9/hotsos/defs/events/openstack/http-requests.yaml
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-06 09:00:02.406256 hotsos-1.15.post9/hotsos/defs/events/openstack/neutron/
--rw-r--r--   0 runner    (1001) docker     (123)     2211 2023-07-06 08:59:40.000000 hotsos-1.15.post9/hotsos/defs/events/openstack/neutron/agents.yaml
--rw-r--r--   0 runner    (1001) docker     (123)      452 2023-07-06 08:59:40.000000 hotsos-1.15.post9/hotsos/defs/events/openstack/neutron/ml2-routers.yaml
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-06 09:00:02.406256 hotsos-1.15.post9/hotsos/defs/events/openstack/nova/
--rw-r--r--   0 runner    (1001) docker     (123)      734 2023-07-06 08:59:40.000000 hotsos-1.15.post9/hotsos/defs/events/openstack/nova/external-events.yaml
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-06 09:00:02.406256 hotsos-1.15.post9/hotsos/defs/events/openstack/nova/migrations/
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-06 09:00:02.406256 hotsos-1.15.post9/hotsos/defs/events/openstack/nova/migrations/live-migration/
--rw-r--r--   0 runner    (1001) docker     (123)      328 2023-07-06 08:59:40.000000 hotsos-1.15.post9/hotsos/defs/events/openstack/nova/migrations/live-migration/dst-pre-live-migration.yaml
--rw-r--r--   0 runner    (1001) docker     (123)      428 2023-07-06 08:59:40.000000 hotsos-1.15.post9/hotsos/defs/events/openstack/nova/migrations/live-migration/src-migration.yaml
--rw-r--r--   0 runner    (1001) docker     (123)      284 2023-07-06 08:59:40.000000 hotsos-1.15.post9/hotsos/defs/events/openstack/nova/migrations/live-migration/src-post-live-migration.yaml
--rw-r--r--   0 runner    (1001) docker     (123)       47 2023-07-06 08:59:40.000000 hotsos-1.15.post9/hotsos/defs/events/openstack/nova/migrations/migrations.yaml
--rw-r--r--   0 runner    (1001) docker     (123)      322 2023-07-06 08:59:40.000000 hotsos-1.15.post9/hotsos/defs/events/openstack/nova/nova-compute.yaml
--rw-r--r--   0 runner    (1001) docker     (123)      633 2023-07-06 08:59:40.000000 hotsos-1.15.post9/hotsos/defs/events/openstack/octavia.yaml
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-06 09:00:02.390256 hotsos-1.15.post9/hotsos/defs/events/openvswitch/
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-06 09:00:02.410256 hotsos-1.15.post9/hotsos/defs/events/openvswitch/ovn/
--rw-r--r--   0 runner    (1001) docker     (123)      699 2023-07-06 08:59:40.000000 hotsos-1.15.post9/hotsos/defs/events/openvswitch/ovn/errors-and-warnings.yaml
--rw-r--r--   0 runner    (1001) docker     (123)     1549 2023-07-06 08:59:40.000000 hotsos-1.15.post9/hotsos/defs/events/openvswitch/ovn/ovn-central.yaml
--rw-r--r--   0 runner    (1001) docker     (123)      661 2023-07-06 08:59:40.000000 hotsos-1.15.post9/hotsos/defs/events/openvswitch/ovn/ovn-controller.yaml
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-06 09:00:02.410256 hotsos-1.15.post9/hotsos/defs/events/openvswitch/ovs/
--rw-r--r--   0 runner    (1001) docker     (123)      240 2023-07-06 08:59:40.000000 hotsos-1.15.post9/hotsos/defs/events/openvswitch/ovs/bfd.yaml
--rw-r--r--   0 runner    (1001) docker     (123)      392 2023-07-06 08:59:40.000000 hotsos-1.15.post9/hotsos/defs/events/openvswitch/ovs/datapath-checks.yaml
--rw-r--r--   0 runner    (1001) docker     (123)      401 2023-07-06 08:59:40.000000 hotsos-1.15.post9/hotsos/defs/events/openvswitch/ovs/errors-and-warnings.yaml
--rw-r--r--   0 runner    (1001) docker     (123)     1252 2023-07-06 08:59:40.000000 hotsos-1.15.post9/hotsos/defs/events/openvswitch/ovs/ovs-vswitchd.yaml
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-06 09:00:02.390256 hotsos-1.15.post9/hotsos/defs/events/storage/
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-06 09:00:02.390256 hotsos-1.15.post9/hotsos/defs/events/storage/ceph/
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-06 09:00:02.410256 hotsos-1.15.post9/hotsos/defs/events/storage/ceph/mon/
--rw-r--r--   0 runner    (1001) docker     (123)      246 2023-07-06 08:59:40.000000 hotsos-1.15.post9/hotsos/defs/events/storage/ceph/mon/mon.yaml
--rw-r--r--   0 runner    (1001) docker     (123)      698 2023-07-06 08:59:40.000000 hotsos-1.15.post9/hotsos/defs/events/storage/ceph/mon/monlogs.yaml
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-06 09:00:02.410256 hotsos-1.15.post9/hotsos/defs/events/storage/ceph/osd/
--rw-r--r--   0 runner    (1001) docker     (123)       43 2023-07-06 08:59:40.000000 hotsos-1.15.post9/hotsos/defs/events/storage/ceph/osd/osd.yaml
--rw-r--r--   0 runner    (1001) docker     (123)      489 2023-07-06 08:59:40.000000 hotsos-1.15.post9/hotsos/defs/events/storage/ceph/osd/osdlogs.yaml
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-06 09:00:02.390256 hotsos-1.15.post9/hotsos/defs/scenarios/
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-06 09:00:02.410256 hotsos-1.15.post9/hotsos/defs/scenarios/juju/
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-06 09:00:02.410256 hotsos-1.15.post9/hotsos/defs/scenarios/juju/bugs/
--rw-r--r--   0 runner    (1001) docker     (123)      670 2023-07-06 08:59:40.000000 hotsos-1.15.post9/hotsos/defs/scenarios/juju/bugs/lp1812361.yaml
--rw-r--r--   0 runner    (1001) docker     (123)      640 2023-07-06 08:59:40.000000 hotsos-1.15.post9/hotsos/defs/scenarios/juju/bugs/lp1852502.yaml
--rw-r--r--   0 runner    (1001) docker     (123)      592 2023-07-06 08:59:40.000000 hotsos-1.15.post9/hotsos/defs/scenarios/juju/bugs/lp1858519.yaml
--rw-r--r--   0 runner    (1001) docker     (123)      604 2023-07-06 08:59:40.000000 hotsos-1.15.post9/hotsos/defs/scenarios/juju/bugs/lp1895040.yaml
--rw-r--r--   0 runner    (1001) docker     (123)      777 2023-07-06 08:59:40.000000 hotsos-1.15.post9/hotsos/defs/scenarios/juju/bugs/lp1910958.yaml
--rw-r--r--   0 runner    (1001) docker     (123)      614 2023-07-06 08:59:40.000000 hotsos-1.15.post9/hotsos/defs/scenarios/juju/bugs/lp1948906.yaml
--rw-r--r--   0 runner    (1001) docker     (123)      339 2023-07-06 08:59:40.000000 hotsos-1.15.post9/hotsos/defs/scenarios/juju/bugs/lp1983140.yaml
--rw-r--r--   0 runner    (1001) docker     (123)      362 2023-07-06 08:59:40.000000 hotsos-1.15.post9/hotsos/defs/scenarios/juju/bugs/lp1983506.yaml
--rw-r--r--   0 runner    (1001) docker     (123)      591 2023-07-06 08:59:40.000000 hotsos-1.15.post9/hotsos/defs/scenarios/juju/bugs/lp1996230.yaml
--rw-r--r--   0 runner    (1001) docker     (123)     1355 2023-07-06 08:59:40.000000 hotsos-1.15.post9/hotsos/defs/scenarios/juju/charm_unit_checks.yaml
--rw-r--r--   0 runner    (1001) docker     (123)      187 2023-07-06 08:59:40.000000 hotsos-1.15.post9/hotsos/defs/scenarios/juju/juju.yaml
--rw-r--r--   0 runner    (1001) docker     (123)      399 2023-07-06 08:59:40.000000 hotsos-1.15.post9/hotsos/defs/scenarios/juju/jujud_machine_checks.yaml
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-06 09:00:02.410256 hotsos-1.15.post9/hotsos/defs/scenarios/kernel/
--rw-r--r--   0 runner    (1001) docker     (123)      901 2023-07-06 08:59:40.000000 hotsos-1.15.post9/hotsos/defs/scenarios/kernel/amd_iommu_pt.yaml
--rw-r--r--   0 runner    (1001) docker     (123)      444 2023-07-06 08:59:40.000000 hotsos-1.15.post9/hotsos/defs/scenarios/kernel/disk_failure.yaml
--rw-r--r--   0 runner    (1001) docker     (123)     2490 2023-07-06 08:59:40.000000 hotsos-1.15.post9/hotsos/defs/scenarios/kernel/kernlog_calltrace.yaml
--rw-r--r--   0 runner    (1001) docker     (123)     2061 2023-07-06 08:59:40.000000 hotsos-1.15.post9/hotsos/defs/scenarios/kernel/memory.yaml
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-06 09:00:02.410256 hotsos-1.15.post9/hotsos/defs/scenarios/kernel/network/
--rw-r--r--   0 runner    (1001) docker     (123)      935 2023-07-06 08:59:40.000000 hotsos-1.15.post9/hotsos/defs/scenarios/kernel/network/misc.yaml
--rw-r--r--   0 runner    (1001) docker     (123)     7336 2023-07-06 08:59:40.000000 hotsos-1.15.post9/hotsos/defs/scenarios/kernel/network/tcp.yaml
--rw-r--r--   0 runner    (1001) docker     (123)     3581 2023-07-06 08:59:40.000000 hotsos-1.15.post9/hotsos/defs/scenarios/kernel/network/udp.yaml
--rw-r--r--   0 runner    (1001) docker     (123)      590 2023-07-06 08:59:40.000000 hotsos-1.15.post9/hotsos/defs/scenarios/kernel/qla2xxx.yaml
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-06 09:00:02.410256 hotsos-1.15.post9/hotsos/defs/scenarios/kubernetes/
--rw-r--r--   0 runner    (1001) docker     (123)      200 2023-07-06 08:59:40.000000 hotsos-1.15.post9/hotsos/defs/scenarios/kubernetes/kubernetes.yaml
--rw-r--r--   0 runner    (1001) docker     (123)     1911 2023-07-06 08:59:40.000000 hotsos-1.15.post9/hotsos/defs/scenarios/kubernetes/system_cpufreq_mode.yaml
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-06 09:00:02.410256 hotsos-1.15.post9/hotsos/defs/scenarios/lxd/
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-06 09:00:02.410256 hotsos-1.15.post9/hotsos/defs/scenarios/lxd/bugs/
--rw-r--r--   0 runner    (1001) docker     (123)     1407 2023-07-06 08:59:40.000000 hotsos-1.15.post9/hotsos/defs/scenarios/lxd/bugs/lp1807628.yaml
--rw-r--r--   0 runner    (1001) docker     (123)      938 2023-07-06 08:59:40.000000 hotsos-1.15.post9/hotsos/defs/scenarios/lxd/lxcfs_deadlock.yaml
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-06 09:00:02.410256 hotsos-1.15.post9/hotsos/defs/scenarios/mysql/
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-06 09:00:02.414256 hotsos-1.15.post9/hotsos/defs/scenarios/mysql/bugs/
--rw-r--r--   0 runner    (1001) docker     (123)      799 2023-07-06 08:59:40.000000 hotsos-1.15.post9/hotsos/defs/scenarios/mysql/bugs/lp1959861.yaml
--rw-r--r--   0 runner    (1001) docker     (123)     1442 2023-07-06 08:59:40.000000 hotsos-1.15.post9/hotsos/defs/scenarios/mysql/bugs/lp1971565.yaml
--rw-r--r--   0 runner    (1001) docker     (123)      418 2023-07-06 08:59:40.000000 hotsos-1.15.post9/hotsos/defs/scenarios/mysql/bugs/lp372017.yaml
--rw-r--r--   0 runner    (1001) docker     (123)      189 2023-07-06 08:59:40.000000 hotsos-1.15.post9/hotsos/defs/scenarios/mysql/mysql.yaml
--rw-r--r--   0 runner    (1001) docker     (123)      739 2023-07-06 08:59:40.000000 hotsos-1.15.post9/hotsos/defs/scenarios/mysql/mysql_connections.yaml
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-06 09:00:02.414256 hotsos-1.15.post9/hotsos/defs/scenarios/openstack/
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-06 09:00:02.390256 hotsos-1.15.post9/hotsos/defs/scenarios/openstack/barbican/
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-06 09:00:02.414256 hotsos-1.15.post9/hotsos/defs/scenarios/openstack/barbican/bugs/
--rw-r--r--   0 runner    (1001) docker     (123)      735 2023-07-06 08:59:40.000000 hotsos-1.15.post9/hotsos/defs/scenarios/openstack/barbican/bugs/lp1946787.yaml
--rw-r--r--   0 runner    (1001) docker     (123)      571 2023-07-06 08:59:40.000000 hotsos-1.15.post9/hotsos/defs/scenarios/openstack/eol.yaml
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-06 09:00:02.390256 hotsos-1.15.post9/hotsos/defs/scenarios/openstack/keystone/
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-06 09:00:02.414256 hotsos-1.15.post9/hotsos/defs/scenarios/openstack/keystone/bugs/
--rw-r--r--   0 runner    (1001) docker     (123)     1425 2023-07-06 08:59:40.000000 hotsos-1.15.post9/hotsos/defs/scenarios/openstack/keystone/bugs/lp1896125.yaml
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-06 09:00:02.414256 hotsos-1.15.post9/hotsos/defs/scenarios/openstack/masakari/
--rw-r--r--   0 runner    (1001) docker     (123)     1016 2023-07-06 08:59:40.000000 hotsos-1.15.post9/hotsos/defs/scenarios/openstack/masakari/pacemaker_remote.yaml
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-06 09:00:02.414256 hotsos-1.15.post9/hotsos/defs/scenarios/openstack/neutron/
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-06 09:00:02.414256 hotsos-1.15.post9/hotsos/defs/scenarios/openstack/neutron/bugs/
--rw-r--r--   0 runner    (1001) docker     (123)      585 2023-07-06 08:59:40.000000 hotsos-1.15.post9/hotsos/defs/scenarios/openstack/neutron/bugs/lp1794991.yaml
--rw-r--r--   0 runner    (1001) docker     (123)      417 2023-07-06 08:59:40.000000 hotsos-1.15.post9/hotsos/defs/scenarios/openstack/neutron/bugs/lp1883089.yaml
--rw-r--r--   0 runner    (1001) docker     (123)      387 2023-07-06 08:59:40.000000 hotsos-1.15.post9/hotsos/defs/scenarios/openstack/neutron/bugs/lp1896506.yaml
--rw-r--r--   0 runner    (1001) docker     (123)      530 2023-07-06 08:59:40.000000 hotsos-1.15.post9/hotsos/defs/scenarios/openstack/neutron/bugs/lp1907686.yaml
--rw-r--r--   0 runner    (1001) docker     (123)      804 2023-07-06 08:59:40.000000 hotsos-1.15.post9/hotsos/defs/scenarios/openstack/neutron/bugs/lp1927868.yaml
--rw-r--r--   0 runner    (1001) docker     (123)      414 2023-07-06 08:59:40.000000 hotsos-1.15.post9/hotsos/defs/scenarios/openstack/neutron/bugs/lp1928031.yaml
--rw-r--r--   0 runner    (1001) docker     (123)      486 2023-07-06 08:59:40.000000 hotsos-1.15.post9/hotsos/defs/scenarios/openstack/neutron/bugs/lp1929832.yaml
--rw-r--r--   0 runner    (1001) docker     (123)      744 2023-07-06 08:59:40.000000 hotsos-1.15.post9/hotsos/defs/scenarios/openstack/neutron/bugs/lp1960319.yaml
--rw-r--r--   0 runner    (1001) docker     (123)      448 2023-07-06 08:59:40.000000 hotsos-1.15.post9/hotsos/defs/scenarios/openstack/neutron/bugs/lp1965297.yaml
--rw-r--r--   0 runner    (1001) docker     (123)      941 2023-07-06 08:59:40.000000 hotsos-1.15.post9/hotsos/defs/scenarios/openstack/neutron/bugs/lp1979089.yaml
--rw-r--r--   0 runner    (1001) docker     (123)      577 2023-07-06 08:59:40.000000 hotsos-1.15.post9/hotsos/defs/scenarios/openstack/neutron/bugs/lp1993628.yaml
--rw-r--r--   0 runner    (1001) docker     (123)      821 2023-07-06 08:59:40.000000 hotsos-1.15.post9/hotsos/defs/scenarios/openstack/neutron/bugs/lp1996594.yaml
--rw-r--r--   0 runner    (1001) docker     (123)      531 2023-07-06 08:59:40.000000 hotsos-1.15.post9/hotsos/defs/scenarios/openstack/neutron/neutron_ovs_cleanup.yaml
--rw-r--r--   0 runner    (1001) docker     (123)     2128 2023-07-06 08:59:40.000000 hotsos-1.15.post9/hotsos/defs/scenarios/openstack/neutron/ovn_stale_db.yaml
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-06 09:00:02.414256 hotsos-1.15.post9/hotsos/defs/scenarios/openstack/nova/
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-06 09:00:02.414256 hotsos-1.15.post9/hotsos/defs/scenarios/openstack/nova/bugs/
--rw-r--r--   0 runner    (1001) docker     (123)      681 2023-07-06 08:59:40.000000 hotsos-1.15.post9/hotsos/defs/scenarios/openstack/nova/bugs/lp1860743.yaml
--rw-r--r--   0 runner    (1001) docker     (123)      594 2023-07-06 08:59:40.000000 hotsos-1.15.post9/hotsos/defs/scenarios/openstack/nova/bugs/lp1888395.yaml
--rw-r--r--   0 runner    (1001) docker     (123)      630 2023-07-06 08:59:40.000000 hotsos-1.15.post9/hotsos/defs/scenarios/openstack/nova/bugs/lp1904580.yaml
--rw-r--r--   0 runner    (1001) docker     (123)      394 2023-07-06 08:59:40.000000 hotsos-1.15.post9/hotsos/defs/scenarios/openstack/nova/bugs/lp1944619.yaml
--rw-r--r--   0 runner    (1001) docker     (123)      745 2023-07-06 08:59:40.000000 hotsos-1.15.post9/hotsos/defs/scenarios/openstack/nova/bugs/lp1967956.yaml
--rw-r--r--   0 runner    (1001) docker     (123)      800 2023-07-06 08:59:40.000000 hotsos-1.15.post9/hotsos/defs/scenarios/openstack/nova/config_checks.yaml
--rw-r--r--   0 runner    (1001) docker     (123)     6020 2023-07-06 08:59:40.000000 hotsos-1.15.post9/hotsos/defs/scenarios/openstack/nova/cpu_pinning.yaml
--rw-r--r--   0 runner    (1001) docker     (123)     1289 2023-07-06 08:59:40.000000 hotsos-1.15.post9/hotsos/defs/scenarios/openstack/nova/service_mem_usage.yaml
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-06 09:00:02.414256 hotsos-1.15.post9/hotsos/defs/scenarios/openstack/octavia/
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-06 09:00:02.414256 hotsos-1.15.post9/hotsos/defs/scenarios/openstack/octavia/bugs/
--rw-r--r--   0 runner    (1001) docker     (123)      878 2023-07-06 08:59:40.000000 hotsos-1.15.post9/hotsos/defs/scenarios/openstack/octavia/bugs/sb1896125.yaml
--rw-r--r--   0 runner    (1001) docker     (123)     2430 2023-07-06 08:59:40.000000 hotsos-1.15.post9/hotsos/defs/scenarios/openstack/octavia/excessive_failovers.yaml
--rw-r--r--   0 runner    (1001) docker     (123)     1364 2023-07-06 08:59:40.000000 hotsos-1.15.post9/hotsos/defs/scenarios/openstack/octavia/hm_port_health.yaml
--rw-r--r--   0 runner    (1001) docker     (123)      197 2023-07-06 08:59:40.000000 hotsos-1.15.post9/hotsos/defs/scenarios/openstack/openstack.yaml
--rw-r--r--   0 runner    (1001) docker     (123)      799 2023-07-06 08:59:40.000000 hotsos-1.15.post9/hotsos/defs/scenarios/openstack/openstack_apache2_certificates.yaml
--rw-r--r--   0 runner    (1001) docker     (123)     1053 2023-07-06 08:59:40.000000 hotsos-1.15.post9/hotsos/defs/scenarios/openstack/openstack_charm_conflicts.yaml
--rw-r--r--   0 runner    (1001) docker     (123)      489 2023-07-06 08:59:40.000000 hotsos-1.15.post9/hotsos/defs/scenarios/openstack/pkgs_from_mixed_releases_found.yaml
--rw-r--r--   0 runner    (1001) docker     (123)     2934 2023-07-06 08:59:40.000000 hotsos-1.15.post9/hotsos/defs/scenarios/openstack/system_cpufreq_mode.yaml
--rw-r--r--   0 runner    (1001) docker     (123)      559 2023-07-06 08:59:40.000000 hotsos-1.15.post9/hotsos/defs/scenarios/openstack/systemd_masked_services.yaml
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-06 09:00:02.418256 hotsos-1.15.post9/hotsos/defs/scenarios/openvswitch/
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-06 09:00:02.418256 hotsos-1.15.post9/hotsos/defs/scenarios/openvswitch/bugs/
--rw-r--r--   0 runner    (1001) docker     (123)      576 2023-07-06 08:59:40.000000 hotsos-1.15.post9/hotsos/defs/scenarios/openvswitch/bugs/lp1839592.yaml
--rw-r--r--   0 runner    (1001) docker     (123)     1190 2023-07-06 08:59:40.000000 hotsos-1.15.post9/hotsos/defs/scenarios/openvswitch/bugs/lp1978806.yaml
--rw-r--r--   0 runner    (1001) docker     (123)     2191 2023-07-06 08:59:40.000000 hotsos-1.15.post9/hotsos/defs/scenarios/openvswitch/dpif_lost_packets.yaml
--rw-r--r--   0 runner    (1001) docker     (123)     1062 2023-07-06 08:59:40.000000 hotsos-1.15.post9/hotsos/defs/scenarios/openvswitch/dpif_resubmit_actions.yaml
--rw-r--r--   0 runner    (1001) docker     (123)      201 2023-07-06 08:59:40.000000 hotsos-1.15.post9/hotsos/defs/scenarios/openvswitch/openvswitch.yaml
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-06 09:00:02.418256 hotsos-1.15.post9/hotsos/defs/scenarios/openvswitch/ovn/
--rw-r--r--   0 runner    (1001) docker     (123)     3058 2023-07-06 08:59:40.000000 hotsos-1.15.post9/hotsos/defs/scenarios/openvswitch/ovn/bfd_flapping.yaml
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-06 09:00:02.418256 hotsos-1.15.post9/hotsos/defs/scenarios/openvswitch/ovn/bugs/
--rw-r--r--   0 runner    (1001) docker     (123)      801 2023-07-06 08:59:40.000000 hotsos-1.15.post9/hotsos/defs/scenarios/openvswitch/ovn/bugs/lp1865127.yaml
--rw-r--r--   0 runner    (1001) docker     (123)      478 2023-07-06 08:59:40.000000 hotsos-1.15.post9/hotsos/defs/scenarios/openvswitch/ovn/bugs/lp1917475.yaml
--rw-r--r--   0 runner    (1001) docker     (123)     3543 2023-07-06 08:59:40.000000 hotsos-1.15.post9/hotsos/defs/scenarios/openvswitch/ovn/ovn_central_certs_logs.yaml
--rw-r--r--   0 runner    (1001) docker     (123)      572 2023-07-06 08:59:40.000000 hotsos-1.15.post9/hotsos/defs/scenarios/openvswitch/ovn/ovn_central_services.yaml
--rw-r--r--   0 runner    (1001) docker     (123)     2516 2023-07-06 08:59:40.000000 hotsos-1.15.post9/hotsos/defs/scenarios/openvswitch/ovn/ovn_certs_valid.yaml
--rw-r--r--   0 runner    (1001) docker     (123)     1952 2023-07-06 08:59:40.000000 hotsos-1.15.post9/hotsos/defs/scenarios/openvswitch/ovn/ovn_chassis_certs_logs.yaml
--rw-r--r--   0 runner    (1001) docker     (123)     1167 2023-07-06 08:59:40.000000 hotsos-1.15.post9/hotsos/defs/scenarios/openvswitch/ovn/ovn_db_upgrade.yaml
--rw-r--r--   0 runner    (1001) docker     (123)     1740 2023-07-06 08:59:40.000000 hotsos-1.15.post9/hotsos/defs/scenarios/openvswitch/ovn/ovn_elections.yaml
--rw-r--r--   0 runner    (1001) docker     (123)     1145 2023-07-06 08:59:40.000000 hotsos-1.15.post9/hotsos/defs/scenarios/openvswitch/ovn/ovsdb_reconnect_errors.yaml
--rw-r--r--   0 runner    (1001) docker     (123)      569 2023-07-06 08:59:40.000000 hotsos-1.15.post9/hotsos/defs/scenarios/openvswitch/ovn/service_mem_usage.yaml
--rw-r--r--   0 runner    (1001) docker     (123)      650 2023-07-06 08:59:40.000000 hotsos-1.15.post9/hotsos/defs/scenarios/openvswitch/service_restarts.yaml
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-06 09:00:02.418256 hotsos-1.15.post9/hotsos/defs/scenarios/pacemaker/
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-06 09:00:02.418256 hotsos-1.15.post9/hotsos/defs/scenarios/pacemaker/bugs/
--rw-r--r--   0 runner    (1001) docker     (123)      820 2023-07-06 08:59:40.000000 hotsos-1.15.post9/hotsos/defs/scenarios/pacemaker/bugs/lp1874719.yaml
--rw-r--r--   0 runner    (1001) docker     (123)       88 2023-07-06 08:59:40.000000 hotsos-1.15.post9/hotsos/defs/scenarios/pacemaker/pacemaker.yaml
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-06 09:00:02.418256 hotsos-1.15.post9/hotsos/defs/scenarios/rabbitmq/
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-06 09:00:02.418256 hotsos-1.15.post9/hotsos/defs/scenarios/rabbitmq/bugs/
--rw-r--r--   0 runner    (1001) docker     (123)      765 2023-07-06 08:59:40.000000 hotsos-1.15.post9/hotsos/defs/scenarios/rabbitmq/bugs/lp1943937.yaml
--rw-r--r--   0 runner    (1001) docker     (123)      554 2023-07-06 08:59:40.000000 hotsos-1.15.post9/hotsos/defs/scenarios/rabbitmq/cluster_config.yaml
--rw-r--r--   0 runner    (1001) docker     (123)     1236 2023-07-06 08:59:40.000000 hotsos-1.15.post9/hotsos/defs/scenarios/rabbitmq/cluster_logchecks.yaml
--rw-r--r--   0 runner    (1001) docker     (123)      516 2023-07-06 08:59:40.000000 hotsos-1.15.post9/hotsos/defs/scenarios/rabbitmq/cluster_resources.yaml
--rw-r--r--   0 runner    (1001) docker     (123)      195 2023-07-06 08:59:40.000000 hotsos-1.15.post9/hotsos/defs/scenarios/rabbitmq/rabbitmq.yaml
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-06 09:00:02.418256 hotsos-1.15.post9/hotsos/defs/scenarios/sosreport/
--rw-r--r--   0 runner    (1001) docker     (123)      525 2023-07-06 08:59:40.000000 hotsos-1.15.post9/hotsos/defs/scenarios/sosreport/plugin_timeouts.yaml
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-06 09:00:02.418256 hotsos-1.15.post9/hotsos/defs/scenarios/storage/
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-06 09:00:02.418256 hotsos-1.15.post9/hotsos/defs/scenarios/storage/bcache/
--rw-r--r--   0 runner    (1001) docker     (123)      179 2023-07-06 08:59:40.000000 hotsos-1.15.post9/hotsos/defs/scenarios/storage/bcache/bcache.yaml
--rw-r--r--   0 runner    (1001) docker     (123)      817 2023-07-06 08:59:40.000000 hotsos-1.15.post9/hotsos/defs/scenarios/storage/bcache/bdev.yaml
--rw-r--r--   0 runner    (1001) docker     (123)     1482 2023-07-06 08:59:40.000000 hotsos-1.15.post9/hotsos/defs/scenarios/storage/bcache/cacheset.yaml
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-06 09:00:02.390256 hotsos-1.15.post9/hotsos/defs/scenarios/storage/ceph/
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-06 09:00:02.418256 hotsos-1.15.post9/hotsos/defs/scenarios/storage/ceph/ceph-mgr/
--rw-r--r--   0 runner    (1001) docker     (123)      815 2023-07-06 08:59:40.000000 hotsos-1.15.post9/hotsos/defs/scenarios/storage/ceph/ceph-mgr/autoscaler_overlap_roots.yaml
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-06 09:00:02.422256 hotsos-1.15.post9/hotsos/defs/scenarios/storage/ceph/ceph-mon/
--rw-r--r--   0 runner    (1001) docker     (123)      866 2023-07-06 08:59:40.000000 hotsos-1.15.post9/hotsos/defs/scenarios/storage/ceph/ceph-mon/auth_insecure_global_id_reclaim_allowed.yaml
--rw-r--r--   0 runner    (1001) docker     (123)     2331 2023-07-06 08:59:40.000000 hotsos-1.15.post9/hotsos/defs/scenarios/storage/ceph/ceph-mon/autoscaler_bug.yaml
--rw-r--r--   0 runner    (1001) docker     (123)      926 2023-07-06 08:59:40.000000 hotsos-1.15.post9/hotsos/defs/scenarios/storage/ceph/ceph-mon/bluefs_size.yaml
--rw-r--r--   0 runner    (1001) docker     (123)      637 2023-07-06 08:59:40.000000 hotsos-1.15.post9/hotsos/defs/scenarios/storage/ceph/ceph-mon/bluefs_spillover.yaml
--rw-r--r--   0 runner    (1001) docker     (123)      792 2023-07-06 08:59:40.000000 hotsos-1.15.post9/hotsos/defs/scenarios/storage/ceph/ceph-mon/ceph-mon.yaml
--rw-r--r--   0 runner    (1001) docker     (123)     1134 2023-07-06 08:59:40.000000 hotsos-1.15.post9/hotsos/defs/scenarios/storage/ceph/ceph-mon/ceph_address_overlap.yaml
--rw-r--r--   0 runner    (1001) docker     (123)      644 2023-07-06 08:59:40.000000 hotsos-1.15.post9/hotsos/defs/scenarios/storage/ceph/ceph-mon/ceph_cluster_health.yaml
--rw-r--r--   0 runner    (1001) docker     (123)     1143 2023-07-06 08:59:40.000000 hotsos-1.15.post9/hotsos/defs/scenarios/storage/ceph/ceph-mon/ceph_versions_mismatch.yaml
--rw-r--r--   0 runner    (1001) docker     (123)     1419 2023-07-06 08:59:40.000000 hotsos-1.15.post9/hotsos/defs/scenarios/storage/ceph/ceph-mon/crushmap_bucket_checks.yaml
--rw-r--r--   0 runner    (1001) docker     (123)      909 2023-07-06 08:59:40.000000 hotsos-1.15.post9/hotsos/defs/scenarios/storage/ceph/ceph-mon/empty_clog.yaml
--rw-r--r--   0 runner    (1001) docker     (123)      557 2023-07-06 08:59:40.000000 hotsos-1.15.post9/hotsos/defs/scenarios/storage/ceph/ceph-mon/eol.yaml
--rw-r--r--   0 runner    (1001) docker     (123)      520 2023-07-06 08:59:40.000000 hotsos-1.15.post9/hotsos/defs/scenarios/storage/ceph/ceph-mon/laggy_pgs.yaml
--rw-r--r--   0 runner    (1001) docker     (123)      782 2023-07-06 08:59:40.000000 hotsos-1.15.post9/hotsos/defs/scenarios/storage/ceph/ceph-mon/large_omap_objects.yaml
--rw-r--r--   0 runner    (1001) docker     (123)      797 2023-07-06 08:59:40.000000 hotsos-1.15.post9/hotsos/defs/scenarios/storage/ceph/ceph-mon/meta_backend_mon.yaml
--rw-r--r--   0 runner    (1001) docker     (123)      854 2023-07-06 08:59:40.000000 hotsos-1.15.post9/hotsos/defs/scenarios/storage/ceph/ceph-mon/mon_db_too_big.yaml
--rw-r--r--   0 runner    (1001) docker     (123)     1450 2023-07-06 08:59:40.000000 hotsos-1.15.post9/hotsos/defs/scenarios/storage/ceph/ceph-mon/mon_elections_flapping.yaml
--rw-r--r--   0 runner    (1001) docker     (123)     1600 2023-07-06 08:59:40.000000 hotsos-1.15.post9/hotsos/defs/scenarios/storage/ceph/ceph-mon/osd_flapping.yaml
--rw-r--r--   0 runner    (1001) docker     (123)     1037 2023-07-06 08:59:40.000000 hotsos-1.15.post9/hotsos/defs/scenarios/storage/ceph/ceph-mon/osd_maps_backlog_too_large.yaml
--rw-r--r--   0 runner    (1001) docker     (123)      825 2023-07-06 08:59:40.000000 hotsos-1.15.post9/hotsos/defs/scenarios/storage/ceph/ceph-mon/osd_messenger_v2_protocol.yaml
--rw-r--r--   0 runner    (1001) docker     (123)      628 2023-07-06 08:59:40.000000 hotsos-1.15.post9/hotsos/defs/scenarios/storage/ceph/ceph-mon/osd_slow_heartbeats.yaml
--rw-r--r--   0 runner    (1001) docker     (123)     1507 2023-07-06 08:59:41.000000 hotsos-1.15.post9/hotsos/defs/scenarios/storage/ceph/ceph-mon/osd_slow_ops.yaml
--rw-r--r--   0 runner    (1001) docker     (123)     1687 2023-07-06 08:59:41.000000 hotsos-1.15.post9/hotsos/defs/scenarios/storage/ceph/ceph-mon/pg_imbalance.yaml
--rw-r--r--   0 runner    (1001) docker     (123)      706 2023-07-06 08:59:41.000000 hotsos-1.15.post9/hotsos/defs/scenarios/storage/ceph/ceph-mon/pg_overdose.yaml
--rw-r--r--   0 runner    (1001) docker     (123)      765 2023-07-06 08:59:41.000000 hotsos-1.15.post9/hotsos/defs/scenarios/storage/ceph/ceph-mon/required_osd_release_mismatch.yaml
--rw-r--r--   0 runner    (1001) docker     (123)     1012 2023-07-06 08:59:41.000000 hotsos-1.15.post9/hotsos/defs/scenarios/storage/ceph/ceph-mon/rgw_frontend.yaml
--rw-r--r--   0 runner    (1001) docker     (123)      888 2023-07-06 08:59:41.000000 hotsos-1.15.post9/hotsos/defs/scenarios/storage/ceph/ceph-mon/ssds_using_bcache.yaml
--rw-r--r--   0 runner    (1001) docker     (123)     1987 2023-07-06 08:59:41.000000 hotsos-1.15.post9/hotsos/defs/scenarios/storage/ceph/ceph-mon/unresponsive_mon_mgr.yaml
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-06 09:00:02.422256 hotsos-1.15.post9/hotsos/defs/scenarios/storage/ceph/ceph-osd/
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-06 09:00:02.426256 hotsos-1.15.post9/hotsos/defs/scenarios/storage/ceph/ceph-osd/bugs/
--rw-r--r--   0 runner    (1001) docker     (123)     1879 2023-07-06 08:59:41.000000 hotsos-1.15.post9/hotsos/defs/scenarios/storage/ceph/ceph-osd/bugs/lp1936136.yaml
--rw-r--r--   0 runner    (1001) docker     (123)      944 2023-07-06 08:59:41.000000 hotsos-1.15.post9/hotsos/defs/scenarios/storage/ceph/ceph-osd/bugs/lp1959649.yaml
--rw-r--r--   0 runner    (1001) docker     (123)     2044 2023-07-06 08:59:41.000000 hotsos-1.15.post9/hotsos/defs/scenarios/storage/ceph/ceph-osd/bugs/lp1996010.yaml
--rw-r--r--   0 runner    (1001) docker     (123)      746 2023-07-06 08:59:41.000000 hotsos-1.15.post9/hotsos/defs/scenarios/storage/ceph/ceph-osd/bugs/lp2013960.yaml
--rw-r--r--   0 runner    (1001) docker     (123)      837 2023-07-06 08:59:41.000000 hotsos-1.15.post9/hotsos/defs/scenarios/storage/ceph/ceph-osd/bugs/lp2016845.yaml
--rw-r--r--   0 runner    (1001) docker     (123)      246 2023-07-06 08:59:41.000000 hotsos-1.15.post9/hotsos/defs/scenarios/storage/ceph/ceph-osd/ceph-osd.yaml
--rw-r--r--   0 runner    (1001) docker     (123)     1134 2023-07-06 08:59:40.000000 hotsos-1.15.post9/hotsos/defs/scenarios/storage/ceph/ceph-osd/ceph_address_overlap.yaml
--rw-r--r--   0 runner    (1001) docker     (123)      557 2023-07-06 08:59:40.000000 hotsos-1.15.post9/hotsos/defs/scenarios/storage/ceph/ceph-osd/eol.yaml
--rw-r--r--   0 runner    (1001) docker     (123)      717 2023-07-06 08:59:41.000000 hotsos-1.15.post9/hotsos/defs/scenarios/storage/ceph/ceph-osd/filestore_to_bluestore_upgrade.yaml
--rw-r--r--   0 runner    (1001) docker     (123)      904 2023-07-06 08:59:41.000000 hotsos-1.15.post9/hotsos/defs/scenarios/storage/ceph/ceph-osd/juju_ceph_no_bcache_tuning.yaml
--rw-r--r--   0 runner    (1001) docker     (123)      625 2023-07-06 08:59:41.000000 hotsos-1.15.post9/hotsos/defs/scenarios/storage/ceph/ceph-osd/meta_backend_osd.yaml
--rw-r--r--   0 runner    (1001) docker     (123)     1600 2023-07-06 08:59:40.000000 hotsos-1.15.post9/hotsos/defs/scenarios/storage/ceph/ceph-osd/osd_flapping.yaml
--rw-r--r--   0 runner    (1001) docker     (123)      981 2023-07-06 08:59:41.000000 hotsos-1.15.post9/hotsos/defs/scenarios/storage/ceph/ceph-osd/osd_latency.yaml
--rw-r--r--   0 runner    (1001) docker     (123)     1507 2023-07-06 08:59:41.000000 hotsos-1.15.post9/hotsos/defs/scenarios/storage/ceph/ceph-osd/osd_slow_ops.yaml
--rw-r--r--   0 runner    (1001) docker     (123)     1207 2023-07-06 08:59:41.000000 hotsos-1.15.post9/hotsos/defs/scenarios/storage/ceph/ceph-osd/pg_overdose.yaml
--rw-r--r--   0 runner    (1001) docker     (123)      682 2023-07-06 08:59:41.000000 hotsos-1.15.post9/hotsos/defs/scenarios/storage/ceph/ceph-osd/ssd_osds_no_discard.yaml.disabled
--rw-r--r--   0 runner    (1001) docker     (123)     1632 2023-07-06 08:59:41.000000 hotsos-1.15.post9/hotsos/defs/scenarios/storage/ceph/ceph-osd/system_cpufreq_mode.yaml
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-06 09:00:02.426256 hotsos-1.15.post9/hotsos/defs/scenarios/storage/ceph/ceph-rgw/
--rw-r--r--   0 runner    (1001) docker     (123)     1012 2023-07-06 08:59:41.000000 hotsos-1.15.post9/hotsos/defs/scenarios/storage/ceph/ceph-rgw/rgw_frontend_rgw.yaml
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-06 09:00:02.426256 hotsos-1.15.post9/hotsos/defs/scenarios/storage/ceph/common/
--rw-r--r--   0 runner    (1001) docker     (123)     1587 2023-07-06 08:59:41.000000 hotsos-1.15.post9/hotsos/defs/scenarios/storage/ceph/common/ceph_charm_conflicts.yaml
--rw-r--r--   0 runner    (1001) docker     (123)      289 2023-07-06 08:59:41.000000 hotsos-1.15.post9/hotsos/defs/scenarios/storage/storage.yaml
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-06 09:00:02.426256 hotsos-1.15.post9/hotsos/defs/scenarios/system/
--rw-r--r--   0 runner    (1001) docker     (123)      191 2023-07-06 08:59:41.000000 hotsos-1.15.post9/hotsos/defs/scenarios/system/system.yaml
--rw-r--r--   0 runner    (1001) docker     (123)      434 2023-07-06 08:59:41.000000 hotsos-1.15.post9/hotsos/defs/scenarios/system/unattended_upgrades.yaml
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-06 09:00:02.426256 hotsos-1.15.post9/hotsos/plugin_extensions/
--rw-r--r--   0 runner    (1001) docker     (123)        0 2023-07-06 08:59:41.000000 hotsos-1.15.post9/hotsos/plugin_extensions/__init__.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-06 09:00:02.426256 hotsos-1.15.post9/hotsos/plugin_extensions/juju/
--rw-r--r--   0 runner    (1001) docker     (123)        0 2023-07-06 08:59:41.000000 hotsos-1.15.post9/hotsos/plugin_extensions/juju/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)     5256 2023-07-06 08:59:41.000000 hotsos-1.15.post9/hotsos/plugin_extensions/juju/summary.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-06 09:00:02.426256 hotsos-1.15.post9/hotsos/plugin_extensions/kernel/
--rw-r--r--   0 runner    (1001) docker     (123)        0 2023-07-06 08:59:41.000000 hotsos-1.15.post9/hotsos/plugin_extensions/kernel/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)     1996 2023-07-06 08:59:41.000000 hotsos-1.15.post9/hotsos/plugin_extensions/kernel/summary.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-06 09:00:02.426256 hotsos-1.15.post9/hotsos/plugin_extensions/kubernetes/
--rw-r--r--   0 runner    (1001) docker     (123)        0 2023-07-06 08:59:41.000000 hotsos-1.15.post9/hotsos/plugin_extensions/kubernetes/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)     1109 2023-07-06 08:59:41.000000 hotsos-1.15.post9/hotsos/plugin_extensions/kubernetes/summary.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-06 09:00:02.426256 hotsos-1.15.post9/hotsos/plugin_extensions/lxd/
--rw-r--r--   0 runner    (1001) docker     (123)        0 2023-07-06 08:59:41.000000 hotsos-1.15.post9/hotsos/plugin_extensions/lxd/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)      617 2023-07-06 08:59:41.000000 hotsos-1.15.post9/hotsos/plugin_extensions/lxd/summary.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-06 09:00:02.426256 hotsos-1.15.post9/hotsos/plugin_extensions/maas/
--rw-r--r--   0 runner    (1001) docker     (123)        0 2023-07-06 08:59:41.000000 hotsos-1.15.post9/hotsos/plugin_extensions/maas/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)      501 2023-07-06 08:59:41.000000 hotsos-1.15.post9/hotsos/plugin_extensions/maas/summary.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-06 09:00:02.426256 hotsos-1.15.post9/hotsos/plugin_extensions/mysql/
--rw-r--r--   0 runner    (1001) docker     (123)        0 2023-07-06 08:59:41.000000 hotsos-1.15.post9/hotsos/plugin_extensions/mysql/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)      471 2023-07-06 08:59:41.000000 hotsos-1.15.post9/hotsos/plugin_extensions/mysql/summary.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-06 09:00:02.426256 hotsos-1.15.post9/hotsos/plugin_extensions/openstack/
--rw-r--r--   0 runner    (1001) docker     (123)        0 2023-07-06 08:59:41.000000 hotsos-1.15.post9/hotsos/plugin_extensions/openstack/__init__.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-06 09:00:02.426256 hotsos-1.15.post9/hotsos/plugin_extensions/openstack/agent/
--rw-r--r--   0 runner    (1001) docker     (123)        0 2023-07-06 08:59:41.000000 hotsos-1.15.post9/hotsos/plugin_extensions/openstack/agent/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)    12198 2023-07-06 08:59:41.000000 hotsos-1.15.post9/hotsos/plugin_extensions/openstack/agent/events.py
--rw-r--r--   0 runner    (1001) docker     (123)    11600 2023-07-06 08:59:41.000000 hotsos-1.15.post9/hotsos/plugin_extensions/openstack/agent/exceptions.py
--rw-r--r--   0 runner    (1001) docker     (123)     3418 2023-07-06 08:59:41.000000 hotsos-1.15.post9/hotsos/plugin_extensions/openstack/nova_external_events.py
--rw-r--r--   0 runner    (1001) docker     (123)     3709 2023-07-06 08:59:41.000000 hotsos-1.15.post9/hotsos/plugin_extensions/openstack/service_features.py
--rw-r--r--   0 runner    (1001) docker     (123)     3959 2023-07-06 08:59:41.000000 hotsos-1.15.post9/hotsos/plugin_extensions/openstack/service_network_checks.py
--rw-r--r--   0 runner    (1001) docker     (123)     1442 2023-07-06 08:59:41.000000 hotsos-1.15.post9/hotsos/plugin_extensions/openstack/summary.py
--rw-r--r--   0 runner    (1001) docker     (123)     7226 2023-07-06 08:59:41.000000 hotsos-1.15.post9/hotsos/plugin_extensions/openstack/vm_info.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-06 09:00:02.426256 hotsos-1.15.post9/hotsos/plugin_extensions/openvswitch/
--rw-r--r--   0 runner    (1001) docker     (123)        0 2023-07-06 08:59:41.000000 hotsos-1.15.post9/hotsos/plugin_extensions/openvswitch/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)     9976 2023-07-06 08:59:41.000000 hotsos-1.15.post9/hotsos/plugin_extensions/openvswitch/event_checks.py
--rw-r--r--   0 runner    (1001) docker     (123)     3052 2023-07-06 08:59:41.000000 hotsos-1.15.post9/hotsos/plugin_extensions/openvswitch/summary.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-06 09:00:02.426256 hotsos-1.15.post9/hotsos/plugin_extensions/pacemaker/
--rw-r--r--   0 runner    (1001) docker     (123)        0 2023-07-06 08:59:41.000000 hotsos-1.15.post9/hotsos/plugin_extensions/pacemaker/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)      678 2023-07-06 08:59:41.000000 hotsos-1.15.post9/hotsos/plugin_extensions/pacemaker/summary.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-06 09:00:02.426256 hotsos-1.15.post9/hotsos/plugin_extensions/rabbitmq/
--rw-r--r--   0 runner    (1001) docker     (123)        0 2023-07-06 08:59:41.000000 hotsos-1.15.post9/hotsos/plugin_extensions/rabbitmq/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)     2398 2023-07-06 08:59:41.000000 hotsos-1.15.post9/hotsos/plugin_extensions/rabbitmq/summary.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-06 09:00:02.430256 hotsos-1.15.post9/hotsos/plugin_extensions/sosreport/
--rw-r--r--   0 runner    (1001) docker     (123)        0 2023-07-06 08:59:41.000000 hotsos-1.15.post9/hotsos/plugin_extensions/sosreport/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)      530 2023-07-06 08:59:41.000000 hotsos-1.15.post9/hotsos/plugin_extensions/sosreport/summary.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-06 09:00:02.430256 hotsos-1.15.post9/hotsos/plugin_extensions/storage/
--rw-r--r--   0 runner    (1001) docker     (123)        0 2023-07-06 08:59:41.000000 hotsos-1.15.post9/hotsos/plugin_extensions/storage/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)      715 2023-07-06 08:59:41.000000 hotsos-1.15.post9/hotsos/plugin_extensions/storage/bcache_summary.py
--rw-r--r--   0 runner    (1001) docker     (123)     4472 2023-07-06 08:59:41.000000 hotsos-1.15.post9/hotsos/plugin_extensions/storage/ceph_event_checks.py
--rw-r--r--   0 runner    (1001) docker     (123)     2366 2023-07-06 08:59:41.000000 hotsos-1.15.post9/hotsos/plugin_extensions/storage/ceph_summary.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-06 09:00:02.430256 hotsos-1.15.post9/hotsos/plugin_extensions/system/
--rw-r--r--   0 runner    (1001) docker     (123)        0 2023-07-06 08:59:41.000000 hotsos-1.15.post9/hotsos/plugin_extensions/system/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)     6474 2023-07-06 08:59:41.000000 hotsos-1.15.post9/hotsos/plugin_extensions/system/checks.py
--rw-r--r--   0 runner    (1001) docker     (123)     1350 2023-07-06 08:59:41.000000 hotsos-1.15.post9/hotsos/plugin_extensions/system/summary.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-06 09:00:02.430256 hotsos-1.15.post9/hotsos/plugin_extensions/vault/
--rw-r--r--   0 runner    (1001) docker     (123)        0 2023-07-06 08:59:41.000000 hotsos-1.15.post9/hotsos/plugin_extensions/vault/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)      466 2023-07-06 08:59:41.000000 hotsos-1.15.post9/hotsos/plugin_extensions/vault/summary.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-06 09:00:02.430256 hotsos-1.15.post9/hotsos/templates/
--rw-r--r--   0 runner    (1001) docker     (123)      232 2023-07-06 08:59:41.000000 hotsos-1.15.post9/hotsos/templates/content_dict.html
--rw-r--r--   0 runner    (1001) docker     (123)      116 2023-07-06 08:59:41.000000 hotsos-1.15.post9/hotsos/templates/content_list.html
--rw-r--r--   0 runner    (1001) docker     (123)       15 2023-07-06 08:59:41.000000 hotsos-1.15.post9/hotsos/templates/footer.html
--rw-r--r--   0 runner    (1001) docker     (123)     2335 2023-07-06 08:59:41.000000 hotsos-1.15.post9/hotsos/templates/header.html
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-06 09:00:02.394256 hotsos-1.15.post9/hotsos.egg-info/
--rw-r--r--   0 runner    (1001) docker     (123)     1193 2023-07-06 09:00:02.000000 hotsos-1.15.post9/hotsos.egg-info/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (123)    15385 2023-07-06 09:00:02.000000 hotsos-1.15.post9/hotsos.egg-info/SOURCES.txt
--rw-r--r--   0 runner    (1001) docker     (123)        1 2023-07-06 09:00:02.000000 hotsos-1.15.post9/hotsos.egg-info/dependency_links.txt
--rw-r--r--   0 runner    (1001) docker     (123)       43 2023-07-06 09:00:02.000000 hotsos-1.15.post9/hotsos.egg-info/entry_points.txt
--rw-r--r--   0 runner    (1001) docker     (123)      135 2023-07-06 09:00:02.000000 hotsos-1.15.post9/hotsos.egg-info/requires.txt
--rw-r--r--   0 runner    (1001) docker     (123)        7 2023-07-06 09:00:02.000000 hotsos-1.15.post9/hotsos.egg-info/top_level.txt
--rw-r--r--   0 runner    (1001) docker     (123)     1063 2023-07-06 08:59:41.000000 hotsos-1.15.post9/pyproject.toml
--rw-r--r--   0 runner    (1001) docker     (123)       38 2023-07-06 09:00:02.430256 hotsos-1.15.post9/setup.cfg
--rw-r--r--   0 runner    (1001) docker     (123)      123 2023-07-06 08:59:41.000000 hotsos-1.15.post9/setup.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-21 07:19:29.867990 hotsos-1.16.0.post1/
+-rw-r--r--   0 runner    (1001) docker     (123)    11357 2023-07-21 07:19:08.000000 hotsos-1.16.0.post1/LICENSE
+-rw-r--r--   0 runner    (1001) docker     (123)      102 2023-07-21 07:19:08.000000 hotsos-1.16.0.post1/MANIFEST.in
+-rw-r--r--   0 runner    (1001) docker     (123)     1195 2023-07-21 07:19:29.867990 hotsos-1.16.0.post1/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (123)      908 2023-07-21 07:19:08.000000 hotsos-1.16.0.post1/README.md
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-21 07:19:29.823989 hotsos-1.16.0.post1/hotsos/
+-rw-r--r--   0 runner    (1001) docker     (123)        9 2023-07-21 07:19:13.000000 hotsos-1.16.0.post1/hotsos/.repo-info
+-rw-r--r--   0 runner    (1001) docker     (123)        0 2023-07-21 07:19:08.000000 hotsos-1.16.0.post1/hotsos/__init__.py
+-rwxr-xr-x   0 runner    (1001) docker     (123)    13787 2023-07-21 07:19:08.000000 hotsos-1.16.0.post1/hotsos/cli.py
+-rwxr-xr-x   0 runner    (1001) docker     (123)    15371 2023-07-21 07:19:08.000000 hotsos-1.16.0.post1/hotsos/client.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-21 07:19:29.827990 hotsos-1.16.0.post1/hotsos/core/
+-rw-r--r--   0 runner    (1001) docker     (123)        0 2023-07-21 07:19:08.000000 hotsos-1.16.0.post1/hotsos/core/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)    10727 2023-07-21 07:19:08.000000 hotsos-1.16.0.post1/hotsos/core/analytics.py
+-rw-r--r--   0 runner    (1001) docker     (123)    10126 2023-07-21 07:19:08.000000 hotsos-1.16.0.post1/hotsos/core/config.py
+-rw-r--r--   0 runner    (1001) docker     (123)       46 2023-07-21 07:19:08.000000 hotsos-1.16.0.post1/hotsos/core/exceptions.py
+-rw-r--r--   0 runner    (1001) docker     (123)      623 2023-07-21 07:19:08.000000 hotsos-1.16.0.post1/hotsos/core/factory.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-21 07:19:29.831990 hotsos-1.16.0.post1/hotsos/core/host_helpers/
+-rw-r--r--   0 runner    (1001) docker     (123)      739 2023-07-21 07:19:08.000000 hotsos-1.16.0.post1/hotsos/core/host_helpers/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)    40487 2023-07-21 07:19:08.000000 hotsos-1.16.0.post1/hotsos/core/host_helpers/cli.py
+-rw-r--r--   0 runner    (1001) docker     (123)     3068 2023-07-21 07:19:08.000000 hotsos-1.16.0.post1/hotsos/core/host_helpers/common.py
+-rw-r--r--   0 runner    (1001) docker     (123)     4694 2023-07-21 07:19:08.000000 hotsos-1.16.0.post1/hotsos/core/host_helpers/config.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1245 2023-07-21 07:19:08.000000 hotsos-1.16.0.post1/hotsos/core/host_helpers/filestat.py
+-rw-r--r--   0 runner    (1001) docker     (123)    10947 2023-07-21 07:19:08.000000 hotsos-1.16.0.post1/hotsos/core/host_helpers/network.py
+-rw-r--r--   0 runner    (1001) docker     (123)    13241 2023-07-21 07:19:08.000000 hotsos-1.16.0.post1/hotsos/core/host_helpers/packaging.py
+-rw-r--r--   0 runner    (1001) docker     (123)     3367 2023-07-21 07:19:08.000000 hotsos-1.16.0.post1/hotsos/core/host_helpers/pebble.py
+-rw-r--r--   0 runner    (1001) docker     (123)     2341 2023-07-21 07:19:08.000000 hotsos-1.16.0.post1/hotsos/core/host_helpers/ssl.py
+-rw-r--r--   0 runner    (1001) docker     (123)     2428 2023-07-21 07:19:08.000000 hotsos-1.16.0.post1/hotsos/core/host_helpers/sysctl.py
+-rw-r--r--   0 runner    (1001) docker     (123)    14083 2023-07-21 07:19:08.000000 hotsos-1.16.0.post1/hotsos/core/host_helpers/systemd.py
+-rw-r--r--   0 runner    (1001) docker     (123)     2665 2023-07-21 07:19:08.000000 hotsos-1.16.0.post1/hotsos/core/host_helpers/uptime.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-21 07:19:29.831990 hotsos-1.16.0.post1/hotsos/core/issues/
+-rw-r--r--   0 runner    (1001) docker     (123)      126 2023-07-21 07:19:08.000000 hotsos-1.16.0.post1/hotsos/core/issues/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)     2961 2023-07-21 07:19:08.000000 hotsos-1.16.0.post1/hotsos/core/issues/issue_types.py
+-rw-r--r--   0 runner    (1001) docker     (123)     5118 2023-07-21 07:19:08.000000 hotsos-1.16.0.post1/hotsos/core/issues/utils.py
+-rw-r--r--   0 runner    (1001) docker     (123)      551 2023-07-21 07:19:08.000000 hotsos-1.16.0.post1/hotsos/core/log.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-21 07:19:29.831990 hotsos-1.16.0.post1/hotsos/core/plugins/
+-rw-r--r--   0 runner    (1001) docker     (123)        0 2023-07-21 07:19:08.000000 hotsos-1.16.0.post1/hotsos/core/plugins/__init__.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-21 07:19:29.835990 hotsos-1.16.0.post1/hotsos/core/plugins/juju/
+-rw-r--r--   0 runner    (1001) docker     (123)       54 2023-07-21 07:19:08.000000 hotsos-1.16.0.post1/hotsos/core/plugins/juju/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1462 2023-07-21 07:19:08.000000 hotsos-1.16.0.post1/hotsos/core/plugins/juju/common.py
+-rw-r--r--   0 runner    (1001) docker     (123)     6374 2023-07-21 07:19:08.000000 hotsos-1.16.0.post1/hotsos/core/plugins/juju/resources.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-21 07:19:29.835990 hotsos-1.16.0.post1/hotsos/core/plugins/kernel/
+-rw-r--r--   0 runner    (1001) docker     (123)      160 2023-07-21 07:19:08.000000 hotsos-1.16.0.post1/hotsos/core/plugins/kernel/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1589 2023-07-21 07:19:08.000000 hotsos-1.16.0.post1/hotsos/core/plugins/kernel/common.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1442 2023-07-21 07:19:08.000000 hotsos-1.16.0.post1/hotsos/core/plugins/kernel/config.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-21 07:19:29.835990 hotsos-1.16.0.post1/hotsos/core/plugins/kernel/kernlog/
+-rw-r--r--   0 runner    (1001) docker     (123)      112 2023-07-21 07:19:08.000000 hotsos-1.16.0.post1/hotsos/core/plugins/kernel/kernlog/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)    14852 2023-07-21 07:19:08.000000 hotsos-1.16.0.post1/hotsos/core/plugins/kernel/kernlog/calltrace.py
+-rw-r--r--   0 runner    (1001) docker     (123)     3835 2023-07-21 07:19:08.000000 hotsos-1.16.0.post1/hotsos/core/plugins/kernel/kernlog/common.py
+-rw-r--r--   0 runner    (1001) docker     (123)     2487 2023-07-21 07:19:08.000000 hotsos-1.16.0.post1/hotsos/core/plugins/kernel/kernlog/events.py
+-rw-r--r--   0 runner    (1001) docker     (123)     7491 2023-07-21 07:19:08.000000 hotsos-1.16.0.post1/hotsos/core/plugins/kernel/memory.py
+-rw-r--r--   0 runner    (1001) docker     (123)    20363 2023-07-21 07:19:08.000000 hotsos-1.16.0.post1/hotsos/core/plugins/kernel/net.py
+-rw-r--r--   0 runner    (1001) docker     (123)     2019 2023-07-21 07:19:08.000000 hotsos-1.16.0.post1/hotsos/core/plugins/kernel/sysfs.py
+-rw-r--r--   0 runner    (1001) docker     (123)     3455 2023-07-21 07:19:08.000000 hotsos-1.16.0.post1/hotsos/core/plugins/kubernetes.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-21 07:19:29.835990 hotsos-1.16.0.post1/hotsos/core/plugins/lxd/
+-rw-r--r--   0 runner    (1001) docker     (123)       58 2023-07-21 07:19:08.000000 hotsos-1.16.0.post1/hotsos/core/plugins/lxd/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1710 2023-07-21 07:19:08.000000 hotsos-1.16.0.post1/hotsos/core/plugins/lxd/common.py
+-rw-r--r--   0 runner    (1001) docker     (123)      966 2023-07-21 07:19:08.000000 hotsos-1.16.0.post1/hotsos/core/plugins/maas.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1385 2023-07-21 07:19:08.000000 hotsos-1.16.0.post1/hotsos/core/plugins/mysql.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-21 07:19:29.835990 hotsos-1.16.0.post1/hotsos/core/plugins/openstack/
+-rw-r--r--   0 runner    (1001) docker     (123)      175 2023-07-21 07:19:08.000000 hotsos-1.16.0.post1/hotsos/core/plugins/openstack/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)     8185 2023-07-21 07:19:08.000000 hotsos-1.16.0.post1/hotsos/core/plugins/openstack/common.py
+-rw-r--r--   0 runner    (1001) docker     (123)    63860 2023-07-21 07:19:08.000000 hotsos-1.16.0.post1/hotsos/core/plugins/openstack/exceptions.py
+-rw-r--r--   0 runner    (1001) docker     (123)     3791 2023-07-21 07:19:08.000000 hotsos-1.16.0.post1/hotsos/core/plugins/openstack/neutron.py
+-rw-r--r--   0 runner    (1001) docker     (123)    10628 2023-07-21 07:19:08.000000 hotsos-1.16.0.post1/hotsos/core/plugins/openstack/nova.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1473 2023-07-21 07:19:08.000000 hotsos-1.16.0.post1/hotsos/core/plugins/openstack/octavia.py
+-rw-r--r--   0 runner    (1001) docker     (123)    19456 2023-07-21 07:19:08.000000 hotsos-1.16.0.post1/hotsos/core/plugins/openstack/openstack.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-21 07:19:29.835990 hotsos-1.16.0.post1/hotsos/core/plugins/openvswitch/
+-rw-r--r--   0 runner    (1001) docker     (123)      166 2023-07-21 07:19:08.000000 hotsos-1.16.0.post1/hotsos/core/plugins/openvswitch/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)     2297 2023-07-21 07:19:08.000000 hotsos-1.16.0.post1/hotsos/core/plugins/openvswitch/common.py
+-rw-r--r--   0 runner    (1001) docker     (123)     4830 2023-07-21 07:19:08.000000 hotsos-1.16.0.post1/hotsos/core/plugins/openvswitch/ovn.py
+-rw-r--r--   0 runner    (1001) docker     (123)     4824 2023-07-21 07:19:08.000000 hotsos-1.16.0.post1/hotsos/core/plugins/openvswitch/ovs.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1628 2023-07-21 07:19:08.000000 hotsos-1.16.0.post1/hotsos/core/plugins/pacemaker.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-21 07:19:29.835990 hotsos-1.16.0.post1/hotsos/core/plugins/rabbitmq/
+-rw-r--r--   0 runner    (1001) docker     (123)      112 2023-07-21 07:19:08.000000 hotsos-1.16.0.post1/hotsos/core/plugins/rabbitmq/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)      947 2023-07-21 07:19:08.000000 hotsos-1.16.0.post1/hotsos/core/plugins/rabbitmq/common.py
+-rw-r--r--   0 runner    (1001) docker     (123)     8865 2023-07-21 07:19:08.000000 hotsos-1.16.0.post1/hotsos/core/plugins/rabbitmq/report.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1793 2023-07-21 07:19:08.000000 hotsos-1.16.0.post1/hotsos/core/plugins/sosreport.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-21 07:19:29.835990 hotsos-1.16.0.post1/hotsos/core/plugins/storage/
+-rw-r--r--   0 runner    (1001) docker     (123)       94 2023-07-21 07:19:08.000000 hotsos-1.16.0.post1/hotsos/core/plugins/storage/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)     5970 2023-07-21 07:19:08.000000 hotsos-1.16.0.post1/hotsos/core/plugins/storage/bcache.py
+-rw-r--r--   0 runner    (1001) docker     (123)    38230 2023-07-21 07:19:08.000000 hotsos-1.16.0.post1/hotsos/core/plugins/storage/ceph.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-21 07:19:29.839990 hotsos-1.16.0.post1/hotsos/core/plugins/system/
+-rw-r--r--   0 runner    (1001) docker     (123)       68 2023-07-21 07:19:08.000000 hotsos-1.16.0.post1/hotsos/core/plugins/system/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)      246 2023-07-21 07:19:08.000000 hotsos-1.16.0.post1/hotsos/core/plugins/system/common.py
+-rw-r--r--   0 runner    (1001) docker     (123)     6919 2023-07-21 07:19:08.000000 hotsos-1.16.0.post1/hotsos/core/plugins/system/system.py
+-rw-r--r--   0 runner    (1001) docker     (123)      799 2023-07-21 07:19:08.000000 hotsos-1.16.0.post1/hotsos/core/plugins/vault.py
+-rw-r--r--   0 runner    (1001) docker     (123)    13833 2023-07-21 07:19:08.000000 hotsos-1.16.0.post1/hotsos/core/plugintools.py
+-rw-r--r--   0 runner    (1001) docker     (123)     3184 2023-07-21 07:19:08.000000 hotsos-1.16.0.post1/hotsos/core/root_manager.py
+-rw-r--r--   0 runner    (1001) docker     (123)     2416 2023-07-21 07:19:08.000000 hotsos-1.16.0.post1/hotsos/core/search.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1710 2023-07-21 07:19:08.000000 hotsos-1.16.0.post1/hotsos/core/utils.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-21 07:19:29.839990 hotsos-1.16.0.post1/hotsos/core/ycheck/
+-rw-r--r--   0 runner    (1001) docker     (123)       59 2023-07-21 07:19:08.000000 hotsos-1.16.0.post1/hotsos/core/ycheck/__init__.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-21 07:19:29.839990 hotsos-1.16.0.post1/hotsos/core/ycheck/engine/
+-rw-r--r--   0 runner    (1001) docker     (123)      134 2023-07-21 07:19:08.000000 hotsos-1.16.0.post1/hotsos/core/ycheck/engine/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)     4094 2023-07-21 07:19:08.000000 hotsos-1.16.0.post1/hotsos/core/ycheck/engine/common.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-21 07:19:29.839990 hotsos-1.16.0.post1/hotsos/core/ycheck/engine/properties/
+-rw-r--r--   0 runner    (1001) docker     (123)      443 2023-07-21 07:19:08.000000 hotsos-1.16.0.post1/hotsos/core/ycheck/engine/properties/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)     6252 2023-07-21 07:19:08.000000 hotsos-1.16.0.post1/hotsos/core/ycheck/engine/properties/checks.py
+-rw-r--r--   0 runner    (1001) docker     (123)    24973 2023-07-21 07:19:08.000000 hotsos-1.16.0.post1/hotsos/core/ycheck/engine/properties/common.py
+-rw-r--r--   0 runner    (1001) docker     (123)     7608 2023-07-21 07:19:08.000000 hotsos-1.16.0.post1/hotsos/core/ycheck/engine/properties/conclusions.py
+-rw-r--r--   0 runner    (1001) docker     (123)     2819 2023-07-21 07:19:08.000000 hotsos-1.16.0.post1/hotsos/core/ycheck/engine/properties/inputdef.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-21 07:19:29.839990 hotsos-1.16.0.post1/hotsos/core/ycheck/engine/properties/requires/
+-rw-r--r--   0 runner    (1001) docker     (123)      215 2023-07-21 07:19:08.000000 hotsos-1.16.0.post1/hotsos/core/ycheck/engine/properties/requires/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)     7450 2023-07-21 07:19:08.000000 hotsos-1.16.0.post1/hotsos/core/ycheck/engine/properties/requires/common.py
+-rw-r--r--   0 runner    (1001) docker     (123)     2378 2023-07-21 07:19:08.000000 hotsos-1.16.0.post1/hotsos/core/ycheck/engine/properties/requires/requires.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-21 07:19:29.839990 hotsos-1.16.0.post1/hotsos/core/ycheck/engine/properties/requires/types/
+-rw-r--r--   0 runner    (1001) docker     (123)        0 2023-07-21 07:19:08.000000 hotsos-1.16.0.post1/hotsos/core/ycheck/engine/properties/requires/types/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)     2920 2023-07-21 07:19:08.000000 hotsos-1.16.0.post1/hotsos/core/ycheck/engine/properties/requires/types/apt.py
+-rw-r--r--   0 runner    (1001) docker     (123)     5906 2023-07-21 07:19:08.000000 hotsos-1.16.0.post1/hotsos/core/ycheck/engine/properties/requires/types/config.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1296 2023-07-21 07:19:08.000000 hotsos-1.16.0.post1/hotsos/core/ycheck/engine/properties/requires/types/path.py
+-rw-r--r--   0 runner    (1001) docker     (123)     2628 2023-07-21 07:19:08.000000 hotsos-1.16.0.post1/hotsos/core/ycheck/engine/properties/requires/types/pebble.py
+-rw-r--r--   0 runner    (1001) docker     (123)      938 2023-07-21 07:19:08.000000 hotsos-1.16.0.post1/hotsos/core/ycheck/engine/properties/requires/types/property.py
+-rw-r--r--   0 runner    (1001) docker     (123)     2377 2023-07-21 07:19:08.000000 hotsos-1.16.0.post1/hotsos/core/ycheck/engine/properties/requires/types/snap.py
+-rw-r--r--   0 runner    (1001) docker     (123)     5034 2023-07-21 07:19:08.000000 hotsos-1.16.0.post1/hotsos/core/ycheck/engine/properties/requires/types/systemd.py
+-rw-r--r--   0 runner    (1001) docker     (123)      927 2023-07-21 07:19:08.000000 hotsos-1.16.0.post1/hotsos/core/ycheck/engine/properties/requires/types/varops.py
+-rw-r--r--   0 runner    (1001) docker     (123)    16525 2023-07-21 07:19:08.000000 hotsos-1.16.0.post1/hotsos/core/ycheck/engine/properties/search.py
+-rw-r--r--   0 runner    (1001) docker     (123)     2961 2023-07-21 07:19:08.000000 hotsos-1.16.0.post1/hotsos/core/ycheck/engine/properties/vardef.py
+-rw-r--r--   0 runner    (1001) docker     (123)    14358 2023-07-21 07:19:08.000000 hotsos-1.16.0.post1/hotsos/core/ycheck/events.py
+-rw-r--r--   0 runner    (1001) docker     (123)     5179 2023-07-21 07:19:08.000000 hotsos-1.16.0.post1/hotsos/core/ycheck/scenarios.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-21 07:19:29.819990 hotsos-1.16.0.post1/hotsos/defs/
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-21 07:19:29.815989 hotsos-1.16.0.post1/hotsos/defs/events/
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-21 07:19:29.839990 hotsos-1.16.0.post1/hotsos/defs/events/openstack/
+-rw-r--r--   0 runner    (1001) docker     (123)      240 2023-07-21 07:19:08.000000 hotsos-1.16.0.post1/hotsos/defs/events/openstack/apache.yaml
+-rw-r--r--   0 runner    (1001) docker     (123)      287 2023-07-21 07:19:08.000000 hotsos-1.16.0.post1/hotsos/defs/events/openstack/apparmor.yaml
+-rw-r--r--   0 runner    (1001) docker     (123)      375 2023-07-21 07:19:08.000000 hotsos-1.16.0.post1/hotsos/defs/events/openstack/http-requests.yaml
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-21 07:19:29.839990 hotsos-1.16.0.post1/hotsos/defs/events/openstack/neutron/
+-rw-r--r--   0 runner    (1001) docker     (123)     2211 2023-07-21 07:19:08.000000 hotsos-1.16.0.post1/hotsos/defs/events/openstack/neutron/agents.yaml
+-rw-r--r--   0 runner    (1001) docker     (123)      452 2023-07-21 07:19:08.000000 hotsos-1.16.0.post1/hotsos/defs/events/openstack/neutron/ml2-routers.yaml
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-21 07:19:29.839990 hotsos-1.16.0.post1/hotsos/defs/events/openstack/nova/
+-rw-r--r--   0 runner    (1001) docker     (123)      734 2023-07-21 07:19:08.000000 hotsos-1.16.0.post1/hotsos/defs/events/openstack/nova/external-events.yaml
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-21 07:19:29.843990 hotsos-1.16.0.post1/hotsos/defs/events/openstack/nova/migrations/
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-21 07:19:29.843990 hotsos-1.16.0.post1/hotsos/defs/events/openstack/nova/migrations/live-migration/
+-rw-r--r--   0 runner    (1001) docker     (123)      328 2023-07-21 07:19:08.000000 hotsos-1.16.0.post1/hotsos/defs/events/openstack/nova/migrations/live-migration/dst-pre-live-migration.yaml
+-rw-r--r--   0 runner    (1001) docker     (123)      428 2023-07-21 07:19:08.000000 hotsos-1.16.0.post1/hotsos/defs/events/openstack/nova/migrations/live-migration/src-migration.yaml
+-rw-r--r--   0 runner    (1001) docker     (123)      284 2023-07-21 07:19:08.000000 hotsos-1.16.0.post1/hotsos/defs/events/openstack/nova/migrations/live-migration/src-post-live-migration.yaml
+-rw-r--r--   0 runner    (1001) docker     (123)       47 2023-07-21 07:19:08.000000 hotsos-1.16.0.post1/hotsos/defs/events/openstack/nova/migrations/migrations.yaml
+-rw-r--r--   0 runner    (1001) docker     (123)      322 2023-07-21 07:19:08.000000 hotsos-1.16.0.post1/hotsos/defs/events/openstack/nova/nova-compute.yaml
+-rw-r--r--   0 runner    (1001) docker     (123)      633 2023-07-21 07:19:08.000000 hotsos-1.16.0.post1/hotsos/defs/events/openstack/octavia.yaml
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-21 07:19:29.815989 hotsos-1.16.0.post1/hotsos/defs/events/openvswitch/
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-21 07:19:29.843990 hotsos-1.16.0.post1/hotsos/defs/events/openvswitch/ovn/
+-rw-r--r--   0 runner    (1001) docker     (123)      699 2023-07-21 07:19:08.000000 hotsos-1.16.0.post1/hotsos/defs/events/openvswitch/ovn/errors-and-warnings.yaml
+-rw-r--r--   0 runner    (1001) docker     (123)     1549 2023-07-21 07:19:08.000000 hotsos-1.16.0.post1/hotsos/defs/events/openvswitch/ovn/ovn-central.yaml
+-rw-r--r--   0 runner    (1001) docker     (123)      661 2023-07-21 07:19:08.000000 hotsos-1.16.0.post1/hotsos/defs/events/openvswitch/ovn/ovn-controller.yaml
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-21 07:19:29.843990 hotsos-1.16.0.post1/hotsos/defs/events/openvswitch/ovs/
+-rw-r--r--   0 runner    (1001) docker     (123)      240 2023-07-21 07:19:08.000000 hotsos-1.16.0.post1/hotsos/defs/events/openvswitch/ovs/bfd.yaml
+-rw-r--r--   0 runner    (1001) docker     (123)      392 2023-07-21 07:19:08.000000 hotsos-1.16.0.post1/hotsos/defs/events/openvswitch/ovs/datapath-checks.yaml
+-rw-r--r--   0 runner    (1001) docker     (123)      401 2023-07-21 07:19:08.000000 hotsos-1.16.0.post1/hotsos/defs/events/openvswitch/ovs/errors-and-warnings.yaml
+-rw-r--r--   0 runner    (1001) docker     (123)     1252 2023-07-21 07:19:08.000000 hotsos-1.16.0.post1/hotsos/defs/events/openvswitch/ovs/ovs-vswitchd.yaml
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-21 07:19:29.819990 hotsos-1.16.0.post1/hotsos/defs/events/storage/
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-21 07:19:29.819990 hotsos-1.16.0.post1/hotsos/defs/events/storage/ceph/
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-21 07:19:29.843990 hotsos-1.16.0.post1/hotsos/defs/events/storage/ceph/mon/
+-rw-r--r--   0 runner    (1001) docker     (123)      246 2023-07-21 07:19:08.000000 hotsos-1.16.0.post1/hotsos/defs/events/storage/ceph/mon/mon.yaml
+-rw-r--r--   0 runner    (1001) docker     (123)      698 2023-07-21 07:19:08.000000 hotsos-1.16.0.post1/hotsos/defs/events/storage/ceph/mon/monlogs.yaml
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-21 07:19:29.843990 hotsos-1.16.0.post1/hotsos/defs/events/storage/ceph/osd/
+-rw-r--r--   0 runner    (1001) docker     (123)       43 2023-07-21 07:19:08.000000 hotsos-1.16.0.post1/hotsos/defs/events/storage/ceph/osd/osd.yaml
+-rw-r--r--   0 runner    (1001) docker     (123)      489 2023-07-21 07:19:08.000000 hotsos-1.16.0.post1/hotsos/defs/events/storage/ceph/osd/osdlogs.yaml
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-21 07:19:29.823989 hotsos-1.16.0.post1/hotsos/defs/scenarios/
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-21 07:19:29.843990 hotsos-1.16.0.post1/hotsos/defs/scenarios/juju/
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-21 07:19:29.843990 hotsos-1.16.0.post1/hotsos/defs/scenarios/juju/bugs/
+-rw-r--r--   0 runner    (1001) docker     (123)      670 2023-07-21 07:19:08.000000 hotsos-1.16.0.post1/hotsos/defs/scenarios/juju/bugs/lp1812361.yaml
+-rw-r--r--   0 runner    (1001) docker     (123)      640 2023-07-21 07:19:08.000000 hotsos-1.16.0.post1/hotsos/defs/scenarios/juju/bugs/lp1852502.yaml
+-rw-r--r--   0 runner    (1001) docker     (123)      592 2023-07-21 07:19:08.000000 hotsos-1.16.0.post1/hotsos/defs/scenarios/juju/bugs/lp1858519.yaml
+-rw-r--r--   0 runner    (1001) docker     (123)      604 2023-07-21 07:19:08.000000 hotsos-1.16.0.post1/hotsos/defs/scenarios/juju/bugs/lp1895040.yaml
+-rw-r--r--   0 runner    (1001) docker     (123)      777 2023-07-21 07:19:08.000000 hotsos-1.16.0.post1/hotsos/defs/scenarios/juju/bugs/lp1910958.yaml
+-rw-r--r--   0 runner    (1001) docker     (123)      614 2023-07-21 07:19:08.000000 hotsos-1.16.0.post1/hotsos/defs/scenarios/juju/bugs/lp1948906.yaml
+-rw-r--r--   0 runner    (1001) docker     (123)      339 2023-07-21 07:19:08.000000 hotsos-1.16.0.post1/hotsos/defs/scenarios/juju/bugs/lp1983140.yaml
+-rw-r--r--   0 runner    (1001) docker     (123)      362 2023-07-21 07:19:08.000000 hotsos-1.16.0.post1/hotsos/defs/scenarios/juju/bugs/lp1983506.yaml
+-rw-r--r--   0 runner    (1001) docker     (123)      591 2023-07-21 07:19:08.000000 hotsos-1.16.0.post1/hotsos/defs/scenarios/juju/bugs/lp1996230.yaml
+-rw-r--r--   0 runner    (1001) docker     (123)     1355 2023-07-21 07:19:08.000000 hotsos-1.16.0.post1/hotsos/defs/scenarios/juju/charm_unit_checks.yaml
+-rw-r--r--   0 runner    (1001) docker     (123)      187 2023-07-21 07:19:08.000000 hotsos-1.16.0.post1/hotsos/defs/scenarios/juju/juju.yaml
+-rw-r--r--   0 runner    (1001) docker     (123)      399 2023-07-21 07:19:08.000000 hotsos-1.16.0.post1/hotsos/defs/scenarios/juju/jujud_machine_checks.yaml
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-21 07:19:29.843990 hotsos-1.16.0.post1/hotsos/defs/scenarios/kernel/
+-rw-r--r--   0 runner    (1001) docker     (123)      901 2023-07-21 07:19:08.000000 hotsos-1.16.0.post1/hotsos/defs/scenarios/kernel/amd_iommu_pt.yaml
+-rw-r--r--   0 runner    (1001) docker     (123)      444 2023-07-21 07:19:08.000000 hotsos-1.16.0.post1/hotsos/defs/scenarios/kernel/disk_failure.yaml
+-rw-r--r--   0 runner    (1001) docker     (123)     2490 2023-07-21 07:19:08.000000 hotsos-1.16.0.post1/hotsos/defs/scenarios/kernel/kernlog_calltrace.yaml
+-rw-r--r--   0 runner    (1001) docker     (123)     2061 2023-07-21 07:19:08.000000 hotsos-1.16.0.post1/hotsos/defs/scenarios/kernel/memory.yaml
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-21 07:19:29.847990 hotsos-1.16.0.post1/hotsos/defs/scenarios/kernel/network/
+-rw-r--r--   0 runner    (1001) docker     (123)      935 2023-07-21 07:19:08.000000 hotsos-1.16.0.post1/hotsos/defs/scenarios/kernel/network/misc.yaml
+-rw-r--r--   0 runner    (1001) docker     (123)     7336 2023-07-21 07:19:08.000000 hotsos-1.16.0.post1/hotsos/defs/scenarios/kernel/network/tcp.yaml
+-rw-r--r--   0 runner    (1001) docker     (123)     3581 2023-07-21 07:19:08.000000 hotsos-1.16.0.post1/hotsos/defs/scenarios/kernel/network/udp.yaml
+-rw-r--r--   0 runner    (1001) docker     (123)      590 2023-07-21 07:19:08.000000 hotsos-1.16.0.post1/hotsos/defs/scenarios/kernel/qla2xxx.yaml
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-21 07:19:29.847990 hotsos-1.16.0.post1/hotsos/defs/scenarios/kubernetes/
+-rw-r--r--   0 runner    (1001) docker     (123)      200 2023-07-21 07:19:08.000000 hotsos-1.16.0.post1/hotsos/defs/scenarios/kubernetes/kubernetes.yaml
+-rw-r--r--   0 runner    (1001) docker     (123)     1911 2023-07-21 07:19:08.000000 hotsos-1.16.0.post1/hotsos/defs/scenarios/kubernetes/system_cpufreq_mode.yaml
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-21 07:19:29.847990 hotsos-1.16.0.post1/hotsos/defs/scenarios/lxd/
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-21 07:19:29.847990 hotsos-1.16.0.post1/hotsos/defs/scenarios/lxd/bugs/
+-rw-r--r--   0 runner    (1001) docker     (123)     1407 2023-07-21 07:19:08.000000 hotsos-1.16.0.post1/hotsos/defs/scenarios/lxd/bugs/lp1807628.yaml
+-rw-r--r--   0 runner    (1001) docker     (123)      938 2023-07-21 07:19:08.000000 hotsos-1.16.0.post1/hotsos/defs/scenarios/lxd/lxcfs_deadlock.yaml
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-21 07:19:29.847990 hotsos-1.16.0.post1/hotsos/defs/scenarios/mysql/
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-21 07:19:29.847990 hotsos-1.16.0.post1/hotsos/defs/scenarios/mysql/bugs/
+-rw-r--r--   0 runner    (1001) docker     (123)      799 2023-07-21 07:19:08.000000 hotsos-1.16.0.post1/hotsos/defs/scenarios/mysql/bugs/lp1959861.yaml
+-rw-r--r--   0 runner    (1001) docker     (123)     1442 2023-07-21 07:19:08.000000 hotsos-1.16.0.post1/hotsos/defs/scenarios/mysql/bugs/lp1971565.yaml
+-rw-r--r--   0 runner    (1001) docker     (123)      418 2023-07-21 07:19:08.000000 hotsos-1.16.0.post1/hotsos/defs/scenarios/mysql/bugs/lp372017.yaml
+-rw-r--r--   0 runner    (1001) docker     (123)      189 2023-07-21 07:19:08.000000 hotsos-1.16.0.post1/hotsos/defs/scenarios/mysql/mysql.yaml
+-rw-r--r--   0 runner    (1001) docker     (123)      739 2023-07-21 07:19:08.000000 hotsos-1.16.0.post1/hotsos/defs/scenarios/mysql/mysql_connections.yaml
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-21 07:19:29.847990 hotsos-1.16.0.post1/hotsos/defs/scenarios/openstack/
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-21 07:19:29.819990 hotsos-1.16.0.post1/hotsos/defs/scenarios/openstack/barbican/
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-21 07:19:29.847990 hotsos-1.16.0.post1/hotsos/defs/scenarios/openstack/barbican/bugs/
+-rw-r--r--   0 runner    (1001) docker     (123)      735 2023-07-21 07:19:08.000000 hotsos-1.16.0.post1/hotsos/defs/scenarios/openstack/barbican/bugs/lp1946787.yaml
+-rw-r--r--   0 runner    (1001) docker     (123)      571 2023-07-21 07:19:08.000000 hotsos-1.16.0.post1/hotsos/defs/scenarios/openstack/eol.yaml
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-21 07:19:29.819990 hotsos-1.16.0.post1/hotsos/defs/scenarios/openstack/keystone/
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-21 07:19:29.847990 hotsos-1.16.0.post1/hotsos/defs/scenarios/openstack/keystone/bugs/
+-rw-r--r--   0 runner    (1001) docker     (123)     1425 2023-07-21 07:19:08.000000 hotsos-1.16.0.post1/hotsos/defs/scenarios/openstack/keystone/bugs/lp1896125.yaml
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-21 07:19:29.847990 hotsos-1.16.0.post1/hotsos/defs/scenarios/openstack/masakari/
+-rw-r--r--   0 runner    (1001) docker     (123)     1016 2023-07-21 07:19:08.000000 hotsos-1.16.0.post1/hotsos/defs/scenarios/openstack/masakari/pacemaker_remote.yaml
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-21 07:19:29.847990 hotsos-1.16.0.post1/hotsos/defs/scenarios/openstack/neutron/
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-21 07:19:29.847990 hotsos-1.16.0.post1/hotsos/defs/scenarios/openstack/neutron/bugs/
+-rw-r--r--   0 runner    (1001) docker     (123)      585 2023-07-21 07:19:08.000000 hotsos-1.16.0.post1/hotsos/defs/scenarios/openstack/neutron/bugs/lp1794991.yaml
+-rw-r--r--   0 runner    (1001) docker     (123)      417 2023-07-21 07:19:08.000000 hotsos-1.16.0.post1/hotsos/defs/scenarios/openstack/neutron/bugs/lp1883089.yaml
+-rw-r--r--   0 runner    (1001) docker     (123)      387 2023-07-21 07:19:08.000000 hotsos-1.16.0.post1/hotsos/defs/scenarios/openstack/neutron/bugs/lp1896506.yaml
+-rw-r--r--   0 runner    (1001) docker     (123)      530 2023-07-21 07:19:08.000000 hotsos-1.16.0.post1/hotsos/defs/scenarios/openstack/neutron/bugs/lp1907686.yaml
+-rw-r--r--   0 runner    (1001) docker     (123)      804 2023-07-21 07:19:08.000000 hotsos-1.16.0.post1/hotsos/defs/scenarios/openstack/neutron/bugs/lp1927868.yaml
+-rw-r--r--   0 runner    (1001) docker     (123)      414 2023-07-21 07:19:08.000000 hotsos-1.16.0.post1/hotsos/defs/scenarios/openstack/neutron/bugs/lp1928031.yaml
+-rw-r--r--   0 runner    (1001) docker     (123)      486 2023-07-21 07:19:08.000000 hotsos-1.16.0.post1/hotsos/defs/scenarios/openstack/neutron/bugs/lp1929832.yaml
+-rw-r--r--   0 runner    (1001) docker     (123)      744 2023-07-21 07:19:08.000000 hotsos-1.16.0.post1/hotsos/defs/scenarios/openstack/neutron/bugs/lp1960319.yaml
+-rw-r--r--   0 runner    (1001) docker     (123)      448 2023-07-21 07:19:08.000000 hotsos-1.16.0.post1/hotsos/defs/scenarios/openstack/neutron/bugs/lp1965297.yaml
+-rw-r--r--   0 runner    (1001) docker     (123)      941 2023-07-21 07:19:08.000000 hotsos-1.16.0.post1/hotsos/defs/scenarios/openstack/neutron/bugs/lp1979089.yaml
+-rw-r--r--   0 runner    (1001) docker     (123)      577 2023-07-21 07:19:08.000000 hotsos-1.16.0.post1/hotsos/defs/scenarios/openstack/neutron/bugs/lp1993628.yaml
+-rw-r--r--   0 runner    (1001) docker     (123)      821 2023-07-21 07:19:08.000000 hotsos-1.16.0.post1/hotsos/defs/scenarios/openstack/neutron/bugs/lp1996594.yaml
+-rw-r--r--   0 runner    (1001) docker     (123)      531 2023-07-21 07:19:08.000000 hotsos-1.16.0.post1/hotsos/defs/scenarios/openstack/neutron/neutron_ovs_cleanup.yaml
+-rw-r--r--   0 runner    (1001) docker     (123)     2128 2023-07-21 07:19:08.000000 hotsos-1.16.0.post1/hotsos/defs/scenarios/openstack/neutron/ovn_stale_db.yaml
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-21 07:19:29.851990 hotsos-1.16.0.post1/hotsos/defs/scenarios/openstack/nova/
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-21 07:19:29.851990 hotsos-1.16.0.post1/hotsos/defs/scenarios/openstack/nova/bugs/
+-rw-r--r--   0 runner    (1001) docker     (123)      681 2023-07-21 07:19:08.000000 hotsos-1.16.0.post1/hotsos/defs/scenarios/openstack/nova/bugs/lp1860743.yaml
+-rw-r--r--   0 runner    (1001) docker     (123)      594 2023-07-21 07:19:08.000000 hotsos-1.16.0.post1/hotsos/defs/scenarios/openstack/nova/bugs/lp1888395.yaml
+-rw-r--r--   0 runner    (1001) docker     (123)      630 2023-07-21 07:19:08.000000 hotsos-1.16.0.post1/hotsos/defs/scenarios/openstack/nova/bugs/lp1904580.yaml
+-rw-r--r--   0 runner    (1001) docker     (123)      394 2023-07-21 07:19:08.000000 hotsos-1.16.0.post1/hotsos/defs/scenarios/openstack/nova/bugs/lp1944619.yaml
+-rw-r--r--   0 runner    (1001) docker     (123)      745 2023-07-21 07:19:08.000000 hotsos-1.16.0.post1/hotsos/defs/scenarios/openstack/nova/bugs/lp1967956.yaml
+-rw-r--r--   0 runner    (1001) docker     (123)      800 2023-07-21 07:19:08.000000 hotsos-1.16.0.post1/hotsos/defs/scenarios/openstack/nova/config_checks.yaml
+-rw-r--r--   0 runner    (1001) docker     (123)     6020 2023-07-21 07:19:08.000000 hotsos-1.16.0.post1/hotsos/defs/scenarios/openstack/nova/cpu_pinning.yaml
+-rw-r--r--   0 runner    (1001) docker     (123)     1302 2023-07-21 07:19:08.000000 hotsos-1.16.0.post1/hotsos/defs/scenarios/openstack/nova/service_mem_usage.yaml
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-21 07:19:29.851990 hotsos-1.16.0.post1/hotsos/defs/scenarios/openstack/octavia/
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-21 07:19:29.851990 hotsos-1.16.0.post1/hotsos/defs/scenarios/openstack/octavia/bugs/
+-rw-r--r--   0 runner    (1001) docker     (123)      878 2023-07-21 07:19:08.000000 hotsos-1.16.0.post1/hotsos/defs/scenarios/openstack/octavia/bugs/sb1896125.yaml
+-rw-r--r--   0 runner    (1001) docker     (123)     2430 2023-07-21 07:19:08.000000 hotsos-1.16.0.post1/hotsos/defs/scenarios/openstack/octavia/excessive_failovers.yaml
+-rw-r--r--   0 runner    (1001) docker     (123)     1364 2023-07-21 07:19:08.000000 hotsos-1.16.0.post1/hotsos/defs/scenarios/openstack/octavia/hm_port_health.yaml
+-rw-r--r--   0 runner    (1001) docker     (123)      197 2023-07-21 07:19:08.000000 hotsos-1.16.0.post1/hotsos/defs/scenarios/openstack/openstack.yaml
+-rw-r--r--   0 runner    (1001) docker     (123)      799 2023-07-21 07:19:08.000000 hotsos-1.16.0.post1/hotsos/defs/scenarios/openstack/openstack_apache2_certificates.yaml
+-rw-r--r--   0 runner    (1001) docker     (123)     1053 2023-07-21 07:19:08.000000 hotsos-1.16.0.post1/hotsos/defs/scenarios/openstack/openstack_charm_conflicts.yaml
+-rw-r--r--   0 runner    (1001) docker     (123)      489 2023-07-21 07:19:08.000000 hotsos-1.16.0.post1/hotsos/defs/scenarios/openstack/pkgs_from_mixed_releases_found.yaml
+-rw-r--r--   0 runner    (1001) docker     (123)     2934 2023-07-21 07:19:08.000000 hotsos-1.16.0.post1/hotsos/defs/scenarios/openstack/system_cpufreq_mode.yaml
+-rw-r--r--   0 runner    (1001) docker     (123)      559 2023-07-21 07:19:08.000000 hotsos-1.16.0.post1/hotsos/defs/scenarios/openstack/systemd_masked_services.yaml
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-21 07:19:29.851990 hotsos-1.16.0.post1/hotsos/defs/scenarios/openvswitch/
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-21 07:19:29.851990 hotsos-1.16.0.post1/hotsos/defs/scenarios/openvswitch/bugs/
+-rw-r--r--   0 runner    (1001) docker     (123)      576 2023-07-21 07:19:08.000000 hotsos-1.16.0.post1/hotsos/defs/scenarios/openvswitch/bugs/lp1839592.yaml
+-rw-r--r--   0 runner    (1001) docker     (123)     1190 2023-07-21 07:19:08.000000 hotsos-1.16.0.post1/hotsos/defs/scenarios/openvswitch/bugs/lp1978806.yaml
+-rw-r--r--   0 runner    (1001) docker     (123)     2191 2023-07-21 07:19:08.000000 hotsos-1.16.0.post1/hotsos/defs/scenarios/openvswitch/dpif_lost_packets.yaml
+-rw-r--r--   0 runner    (1001) docker     (123)     1062 2023-07-21 07:19:08.000000 hotsos-1.16.0.post1/hotsos/defs/scenarios/openvswitch/dpif_resubmit_actions.yaml
+-rw-r--r--   0 runner    (1001) docker     (123)      201 2023-07-21 07:19:08.000000 hotsos-1.16.0.post1/hotsos/defs/scenarios/openvswitch/openvswitch.yaml
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-21 07:19:29.851990 hotsos-1.16.0.post1/hotsos/defs/scenarios/openvswitch/ovn/
+-rw-r--r--   0 runner    (1001) docker     (123)     3058 2023-07-21 07:19:08.000000 hotsos-1.16.0.post1/hotsos/defs/scenarios/openvswitch/ovn/bfd_flapping.yaml
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-21 07:19:29.851990 hotsos-1.16.0.post1/hotsos/defs/scenarios/openvswitch/ovn/bugs/
+-rw-r--r--   0 runner    (1001) docker     (123)      801 2023-07-21 07:19:08.000000 hotsos-1.16.0.post1/hotsos/defs/scenarios/openvswitch/ovn/bugs/lp1865127.yaml
+-rw-r--r--   0 runner    (1001) docker     (123)      478 2023-07-21 07:19:08.000000 hotsos-1.16.0.post1/hotsos/defs/scenarios/openvswitch/ovn/bugs/lp1917475.yaml
+-rw-r--r--   0 runner    (1001) docker     (123)     3867 2023-07-21 07:19:08.000000 hotsos-1.16.0.post1/hotsos/defs/scenarios/openvswitch/ovn/ovn_central_certs_logs.yaml
+-rw-r--r--   0 runner    (1001) docker     (123)      572 2023-07-21 07:19:08.000000 hotsos-1.16.0.post1/hotsos/defs/scenarios/openvswitch/ovn/ovn_central_services.yaml
+-rw-r--r--   0 runner    (1001) docker     (123)     2516 2023-07-21 07:19:08.000000 hotsos-1.16.0.post1/hotsos/defs/scenarios/openvswitch/ovn/ovn_certs_valid.yaml
+-rw-r--r--   0 runner    (1001) docker     (123)     2006 2023-07-21 07:19:08.000000 hotsos-1.16.0.post1/hotsos/defs/scenarios/openvswitch/ovn/ovn_chassis_certs_logs.yaml
+-rw-r--r--   0 runner    (1001) docker     (123)     1167 2023-07-21 07:19:08.000000 hotsos-1.16.0.post1/hotsos/defs/scenarios/openvswitch/ovn/ovn_db_upgrade.yaml
+-rw-r--r--   0 runner    (1001) docker     (123)     1740 2023-07-21 07:19:08.000000 hotsos-1.16.0.post1/hotsos/defs/scenarios/openvswitch/ovn/ovn_elections.yaml
+-rw-r--r--   0 runner    (1001) docker     (123)     1145 2023-07-21 07:19:08.000000 hotsos-1.16.0.post1/hotsos/defs/scenarios/openvswitch/ovn/ovsdb_reconnect_errors.yaml
+-rw-r--r--   0 runner    (1001) docker     (123)     1348 2023-07-21 07:19:08.000000 hotsos-1.16.0.post1/hotsos/defs/scenarios/openvswitch/ovn/service_mem_usage.yaml
+-rw-r--r--   0 runner    (1001) docker     (123)      650 2023-07-21 07:19:08.000000 hotsos-1.16.0.post1/hotsos/defs/scenarios/openvswitch/service_restarts.yaml
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-21 07:19:29.851990 hotsos-1.16.0.post1/hotsos/defs/scenarios/pacemaker/
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-21 07:19:29.851990 hotsos-1.16.0.post1/hotsos/defs/scenarios/pacemaker/bugs/
+-rw-r--r--   0 runner    (1001) docker     (123)      820 2023-07-21 07:19:08.000000 hotsos-1.16.0.post1/hotsos/defs/scenarios/pacemaker/bugs/lp1874719.yaml
+-rw-r--r--   0 runner    (1001) docker     (123)       88 2023-07-21 07:19:08.000000 hotsos-1.16.0.post1/hotsos/defs/scenarios/pacemaker/pacemaker.yaml
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-21 07:19:29.855990 hotsos-1.16.0.post1/hotsos/defs/scenarios/rabbitmq/
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-21 07:19:29.855990 hotsos-1.16.0.post1/hotsos/defs/scenarios/rabbitmq/bugs/
+-rw-r--r--   0 runner    (1001) docker     (123)      765 2023-07-21 07:19:08.000000 hotsos-1.16.0.post1/hotsos/defs/scenarios/rabbitmq/bugs/lp1943937.yaml
+-rw-r--r--   0 runner    (1001) docker     (123)      554 2023-07-21 07:19:08.000000 hotsos-1.16.0.post1/hotsos/defs/scenarios/rabbitmq/cluster_config.yaml
+-rw-r--r--   0 runner    (1001) docker     (123)     1236 2023-07-21 07:19:08.000000 hotsos-1.16.0.post1/hotsos/defs/scenarios/rabbitmq/cluster_logchecks.yaml
+-rw-r--r--   0 runner    (1001) docker     (123)      516 2023-07-21 07:19:08.000000 hotsos-1.16.0.post1/hotsos/defs/scenarios/rabbitmq/cluster_resources.yaml
+-rw-r--r--   0 runner    (1001) docker     (123)      195 2023-07-21 07:19:08.000000 hotsos-1.16.0.post1/hotsos/defs/scenarios/rabbitmq/rabbitmq.yaml
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-21 07:19:29.855990 hotsos-1.16.0.post1/hotsos/defs/scenarios/sosreport/
+-rw-r--r--   0 runner    (1001) docker     (123)      525 2023-07-21 07:19:08.000000 hotsos-1.16.0.post1/hotsos/defs/scenarios/sosreport/plugin_timeouts.yaml
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-21 07:19:29.855990 hotsos-1.16.0.post1/hotsos/defs/scenarios/storage/
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-21 07:19:29.855990 hotsos-1.16.0.post1/hotsos/defs/scenarios/storage/bcache/
+-rw-r--r--   0 runner    (1001) docker     (123)      179 2023-07-21 07:19:08.000000 hotsos-1.16.0.post1/hotsos/defs/scenarios/storage/bcache/bcache.yaml
+-rw-r--r--   0 runner    (1001) docker     (123)      817 2023-07-21 07:19:08.000000 hotsos-1.16.0.post1/hotsos/defs/scenarios/storage/bcache/bdev.yaml
+-rw-r--r--   0 runner    (1001) docker     (123)     1482 2023-07-21 07:19:08.000000 hotsos-1.16.0.post1/hotsos/defs/scenarios/storage/bcache/cacheset.yaml
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-21 07:19:29.823989 hotsos-1.16.0.post1/hotsos/defs/scenarios/storage/ceph/
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-21 07:19:29.855990 hotsos-1.16.0.post1/hotsos/defs/scenarios/storage/ceph/ceph-mgr/
+-rw-r--r--   0 runner    (1001) docker     (123)      815 2023-07-21 07:19:08.000000 hotsos-1.16.0.post1/hotsos/defs/scenarios/storage/ceph/ceph-mgr/autoscaler_overlap_roots.yaml
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-21 07:19:29.859990 hotsos-1.16.0.post1/hotsos/defs/scenarios/storage/ceph/ceph-mon/
+-rw-r--r--   0 runner    (1001) docker     (123)      862 2023-07-21 07:19:08.000000 hotsos-1.16.0.post1/hotsos/defs/scenarios/storage/ceph/ceph-mon/auth_insecure_global_id_reclaim_allowed.yaml
+-rw-r--r--   0 runner    (1001) docker     (123)     2331 2023-07-21 07:19:08.000000 hotsos-1.16.0.post1/hotsos/defs/scenarios/storage/ceph/ceph-mon/autoscaler_bug.yaml
+-rw-r--r--   0 runner    (1001) docker     (123)      926 2023-07-21 07:19:08.000000 hotsos-1.16.0.post1/hotsos/defs/scenarios/storage/ceph/ceph-mon/bluefs_size.yaml
+-rw-r--r--   0 runner    (1001) docker     (123)      637 2023-07-21 07:19:08.000000 hotsos-1.16.0.post1/hotsos/defs/scenarios/storage/ceph/ceph-mon/bluefs_spillover.yaml
+-rw-r--r--   0 runner    (1001) docker     (123)      792 2023-07-21 07:19:08.000000 hotsos-1.16.0.post1/hotsos/defs/scenarios/storage/ceph/ceph-mon/ceph-mon.yaml
+-rw-r--r--   0 runner    (1001) docker     (123)     1134 2023-07-21 07:19:08.000000 hotsos-1.16.0.post1/hotsos/defs/scenarios/storage/ceph/ceph-mon/ceph_address_overlap.yaml
+-rw-r--r--   0 runner    (1001) docker     (123)      644 2023-07-21 07:19:08.000000 hotsos-1.16.0.post1/hotsos/defs/scenarios/storage/ceph/ceph-mon/ceph_cluster_health.yaml
+-rw-r--r--   0 runner    (1001) docker     (123)     1143 2023-07-21 07:19:08.000000 hotsos-1.16.0.post1/hotsos/defs/scenarios/storage/ceph/ceph-mon/ceph_versions_mismatch.yaml
+-rw-r--r--   0 runner    (1001) docker     (123)     1419 2023-07-21 07:19:08.000000 hotsos-1.16.0.post1/hotsos/defs/scenarios/storage/ceph/ceph-mon/crushmap_bucket_checks.yaml
+-rw-r--r--   0 runner    (1001) docker     (123)      909 2023-07-21 07:19:08.000000 hotsos-1.16.0.post1/hotsos/defs/scenarios/storage/ceph/ceph-mon/empty_clog.yaml
+-rw-r--r--   0 runner    (1001) docker     (123)      557 2023-07-21 07:19:08.000000 hotsos-1.16.0.post1/hotsos/defs/scenarios/storage/ceph/ceph-mon/eol.yaml
+-rw-r--r--   0 runner    (1001) docker     (123)      520 2023-07-21 07:19:08.000000 hotsos-1.16.0.post1/hotsos/defs/scenarios/storage/ceph/ceph-mon/laggy_pgs.yaml
+-rw-r--r--   0 runner    (1001) docker     (123)      782 2023-07-21 07:19:08.000000 hotsos-1.16.0.post1/hotsos/defs/scenarios/storage/ceph/ceph-mon/large_omap_objects.yaml
+-rw-r--r--   0 runner    (1001) docker     (123)      797 2023-07-21 07:19:08.000000 hotsos-1.16.0.post1/hotsos/defs/scenarios/storage/ceph/ceph-mon/meta_backend_mon.yaml
+-rw-r--r--   0 runner    (1001) docker     (123)      854 2023-07-21 07:19:08.000000 hotsos-1.16.0.post1/hotsos/defs/scenarios/storage/ceph/ceph-mon/mon_db_too_big.yaml
+-rw-r--r--   0 runner    (1001) docker     (123)     1450 2023-07-21 07:19:08.000000 hotsos-1.16.0.post1/hotsos/defs/scenarios/storage/ceph/ceph-mon/mon_elections_flapping.yaml
+-rw-r--r--   0 runner    (1001) docker     (123)     1600 2023-07-21 07:19:08.000000 hotsos-1.16.0.post1/hotsos/defs/scenarios/storage/ceph/ceph-mon/osd_flapping.yaml
+-rw-r--r--   0 runner    (1001) docker     (123)     1037 2023-07-21 07:19:08.000000 hotsos-1.16.0.post1/hotsos/defs/scenarios/storage/ceph/ceph-mon/osd_maps_backlog_too_large.yaml
+-rw-r--r--   0 runner    (1001) docker     (123)      825 2023-07-21 07:19:08.000000 hotsos-1.16.0.post1/hotsos/defs/scenarios/storage/ceph/ceph-mon/osd_messenger_v2_protocol.yaml
+-rw-r--r--   0 runner    (1001) docker     (123)      628 2023-07-21 07:19:08.000000 hotsos-1.16.0.post1/hotsos/defs/scenarios/storage/ceph/ceph-mon/osd_slow_heartbeats.yaml
+-rw-r--r--   0 runner    (1001) docker     (123)     1507 2023-07-21 07:19:08.000000 hotsos-1.16.0.post1/hotsos/defs/scenarios/storage/ceph/ceph-mon/osd_slow_ops.yaml
+-rw-r--r--   0 runner    (1001) docker     (123)     1687 2023-07-21 07:19:08.000000 hotsos-1.16.0.post1/hotsos/defs/scenarios/storage/ceph/ceph-mon/pg_imbalance.yaml
+-rw-r--r--   0 runner    (1001) docker     (123)      706 2023-07-21 07:19:08.000000 hotsos-1.16.0.post1/hotsos/defs/scenarios/storage/ceph/ceph-mon/pg_overdose.yaml
+-rw-r--r--   0 runner    (1001) docker     (123)      765 2023-07-21 07:19:08.000000 hotsos-1.16.0.post1/hotsos/defs/scenarios/storage/ceph/ceph-mon/required_osd_release_mismatch.yaml
+-rw-r--r--   0 runner    (1001) docker     (123)     1012 2023-07-21 07:19:08.000000 hotsos-1.16.0.post1/hotsos/defs/scenarios/storage/ceph/ceph-mon/rgw_frontend.yaml
+-rw-r--r--   0 runner    (1001) docker     (123)      888 2023-07-21 07:19:08.000000 hotsos-1.16.0.post1/hotsos/defs/scenarios/storage/ceph/ceph-mon/ssds_using_bcache.yaml
+-rw-r--r--   0 runner    (1001) docker     (123)     1987 2023-07-21 07:19:08.000000 hotsos-1.16.0.post1/hotsos/defs/scenarios/storage/ceph/ceph-mon/unresponsive_mon_mgr.yaml
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-21 07:19:29.859990 hotsos-1.16.0.post1/hotsos/defs/scenarios/storage/ceph/ceph-osd/
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-21 07:19:29.859990 hotsos-1.16.0.post1/hotsos/defs/scenarios/storage/ceph/ceph-osd/bugs/
+-rw-r--r--   0 runner    (1001) docker     (123)     1879 2023-07-21 07:19:08.000000 hotsos-1.16.0.post1/hotsos/defs/scenarios/storage/ceph/ceph-osd/bugs/lp1936136.yaml
+-rw-r--r--   0 runner    (1001) docker     (123)      944 2023-07-21 07:19:08.000000 hotsos-1.16.0.post1/hotsos/defs/scenarios/storage/ceph/ceph-osd/bugs/lp1959649.yaml
+-rw-r--r--   0 runner    (1001) docker     (123)     2044 2023-07-21 07:19:08.000000 hotsos-1.16.0.post1/hotsos/defs/scenarios/storage/ceph/ceph-osd/bugs/lp1996010.yaml
+-rw-r--r--   0 runner    (1001) docker     (123)      746 2023-07-21 07:19:08.000000 hotsos-1.16.0.post1/hotsos/defs/scenarios/storage/ceph/ceph-osd/bugs/lp2013960.yaml
+-rw-r--r--   0 runner    (1001) docker     (123)      837 2023-07-21 07:19:08.000000 hotsos-1.16.0.post1/hotsos/defs/scenarios/storage/ceph/ceph-osd/bugs/lp2016845.yaml
+-rw-r--r--   0 runner    (1001) docker     (123)      246 2023-07-21 07:19:08.000000 hotsos-1.16.0.post1/hotsos/defs/scenarios/storage/ceph/ceph-osd/ceph-osd.yaml
+-rw-r--r--   0 runner    (1001) docker     (123)     1134 2023-07-21 07:19:08.000000 hotsos-1.16.0.post1/hotsos/defs/scenarios/storage/ceph/ceph-osd/ceph_address_overlap.yaml
+-rw-r--r--   0 runner    (1001) docker     (123)      557 2023-07-21 07:19:08.000000 hotsos-1.16.0.post1/hotsos/defs/scenarios/storage/ceph/ceph-osd/eol.yaml
+-rw-r--r--   0 runner    (1001) docker     (123)      717 2023-07-21 07:19:08.000000 hotsos-1.16.0.post1/hotsos/defs/scenarios/storage/ceph/ceph-osd/filestore_to_bluestore_upgrade.yaml
+-rw-r--r--   0 runner    (1001) docker     (123)      904 2023-07-21 07:19:08.000000 hotsos-1.16.0.post1/hotsos/defs/scenarios/storage/ceph/ceph-osd/juju_ceph_no_bcache_tuning.yaml
+-rw-r--r--   0 runner    (1001) docker     (123)      625 2023-07-21 07:19:08.000000 hotsos-1.16.0.post1/hotsos/defs/scenarios/storage/ceph/ceph-osd/meta_backend_osd.yaml
+-rw-r--r--   0 runner    (1001) docker     (123)     1600 2023-07-21 07:19:08.000000 hotsos-1.16.0.post1/hotsos/defs/scenarios/storage/ceph/ceph-osd/osd_flapping.yaml
+-rw-r--r--   0 runner    (1001) docker     (123)      981 2023-07-21 07:19:08.000000 hotsos-1.16.0.post1/hotsos/defs/scenarios/storage/ceph/ceph-osd/osd_latency.yaml
+-rw-r--r--   0 runner    (1001) docker     (123)     1507 2023-07-21 07:19:08.000000 hotsos-1.16.0.post1/hotsos/defs/scenarios/storage/ceph/ceph-osd/osd_slow_ops.yaml
+-rw-r--r--   0 runner    (1001) docker     (123)     1207 2023-07-21 07:19:08.000000 hotsos-1.16.0.post1/hotsos/defs/scenarios/storage/ceph/ceph-osd/pg_overdose.yaml
+-rw-r--r--   0 runner    (1001) docker     (123)      682 2023-07-21 07:19:08.000000 hotsos-1.16.0.post1/hotsos/defs/scenarios/storage/ceph/ceph-osd/ssd_osds_no_discard.yaml.disabled
+-rw-r--r--   0 runner    (1001) docker     (123)     1632 2023-07-21 07:19:08.000000 hotsos-1.16.0.post1/hotsos/defs/scenarios/storage/ceph/ceph-osd/system_cpufreq_mode.yaml
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-21 07:19:29.859990 hotsos-1.16.0.post1/hotsos/defs/scenarios/storage/ceph/ceph-rgw/
+-rw-r--r--   0 runner    (1001) docker     (123)     1012 2023-07-21 07:19:08.000000 hotsos-1.16.0.post1/hotsos/defs/scenarios/storage/ceph/ceph-rgw/rgw_frontend_rgw.yaml
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-21 07:19:29.859990 hotsos-1.16.0.post1/hotsos/defs/scenarios/storage/ceph/common/
+-rw-r--r--   0 runner    (1001) docker     (123)     1587 2023-07-21 07:19:08.000000 hotsos-1.16.0.post1/hotsos/defs/scenarios/storage/ceph/common/ceph_charm_conflicts.yaml
+-rw-r--r--   0 runner    (1001) docker     (123)      289 2023-07-21 07:19:08.000000 hotsos-1.16.0.post1/hotsos/defs/scenarios/storage/storage.yaml
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-21 07:19:29.859990 hotsos-1.16.0.post1/hotsos/defs/scenarios/system/
+-rw-r--r--   0 runner    (1001) docker     (123)      191 2023-07-21 07:19:08.000000 hotsos-1.16.0.post1/hotsos/defs/scenarios/system/system.yaml
+-rw-r--r--   0 runner    (1001) docker     (123)      434 2023-07-21 07:19:08.000000 hotsos-1.16.0.post1/hotsos/defs/scenarios/system/unattended_upgrades.yaml
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-21 07:19:29.859990 hotsos-1.16.0.post1/hotsos/plugin_extensions/
+-rw-r--r--   0 runner    (1001) docker     (123)        0 2023-07-21 07:19:08.000000 hotsos-1.16.0.post1/hotsos/plugin_extensions/__init__.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-21 07:19:29.859990 hotsos-1.16.0.post1/hotsos/plugin_extensions/juju/
+-rw-r--r--   0 runner    (1001) docker     (123)        0 2023-07-21 07:19:08.000000 hotsos-1.16.0.post1/hotsos/plugin_extensions/juju/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)     5256 2023-07-21 07:19:08.000000 hotsos-1.16.0.post1/hotsos/plugin_extensions/juju/summary.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-21 07:19:29.859990 hotsos-1.16.0.post1/hotsos/plugin_extensions/kernel/
+-rw-r--r--   0 runner    (1001) docker     (123)        0 2023-07-21 07:19:08.000000 hotsos-1.16.0.post1/hotsos/plugin_extensions/kernel/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1996 2023-07-21 07:19:08.000000 hotsos-1.16.0.post1/hotsos/plugin_extensions/kernel/summary.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-21 07:19:29.859990 hotsos-1.16.0.post1/hotsos/plugin_extensions/kubernetes/
+-rw-r--r--   0 runner    (1001) docker     (123)        0 2023-07-21 07:19:08.000000 hotsos-1.16.0.post1/hotsos/plugin_extensions/kubernetes/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1109 2023-07-21 07:19:08.000000 hotsos-1.16.0.post1/hotsos/plugin_extensions/kubernetes/summary.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-21 07:19:29.859990 hotsos-1.16.0.post1/hotsos/plugin_extensions/lxd/
+-rw-r--r--   0 runner    (1001) docker     (123)        0 2023-07-21 07:19:08.000000 hotsos-1.16.0.post1/hotsos/plugin_extensions/lxd/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)      617 2023-07-21 07:19:08.000000 hotsos-1.16.0.post1/hotsos/plugin_extensions/lxd/summary.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-21 07:19:29.863990 hotsos-1.16.0.post1/hotsos/plugin_extensions/maas/
+-rw-r--r--   0 runner    (1001) docker     (123)        0 2023-07-21 07:19:08.000000 hotsos-1.16.0.post1/hotsos/plugin_extensions/maas/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)      501 2023-07-21 07:19:08.000000 hotsos-1.16.0.post1/hotsos/plugin_extensions/maas/summary.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-21 07:19:29.863990 hotsos-1.16.0.post1/hotsos/plugin_extensions/mysql/
+-rw-r--r--   0 runner    (1001) docker     (123)        0 2023-07-21 07:19:08.000000 hotsos-1.16.0.post1/hotsos/plugin_extensions/mysql/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)      471 2023-07-21 07:19:08.000000 hotsos-1.16.0.post1/hotsos/plugin_extensions/mysql/summary.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-21 07:19:29.863990 hotsos-1.16.0.post1/hotsos/plugin_extensions/openstack/
+-rw-r--r--   0 runner    (1001) docker     (123)        0 2023-07-21 07:19:08.000000 hotsos-1.16.0.post1/hotsos/plugin_extensions/openstack/__init__.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-21 07:19:29.863990 hotsos-1.16.0.post1/hotsos/plugin_extensions/openstack/agent/
+-rw-r--r--   0 runner    (1001) docker     (123)        0 2023-07-21 07:19:08.000000 hotsos-1.16.0.post1/hotsos/plugin_extensions/openstack/agent/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)    12198 2023-07-21 07:19:08.000000 hotsos-1.16.0.post1/hotsos/plugin_extensions/openstack/agent/events.py
+-rw-r--r--   0 runner    (1001) docker     (123)    11600 2023-07-21 07:19:08.000000 hotsos-1.16.0.post1/hotsos/plugin_extensions/openstack/agent/exceptions.py
+-rw-r--r--   0 runner    (1001) docker     (123)     3418 2023-07-21 07:19:08.000000 hotsos-1.16.0.post1/hotsos/plugin_extensions/openstack/nova_external_events.py
+-rw-r--r--   0 runner    (1001) docker     (123)     3709 2023-07-21 07:19:08.000000 hotsos-1.16.0.post1/hotsos/plugin_extensions/openstack/service_features.py
+-rw-r--r--   0 runner    (1001) docker     (123)     3959 2023-07-21 07:19:08.000000 hotsos-1.16.0.post1/hotsos/plugin_extensions/openstack/service_network_checks.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1442 2023-07-21 07:19:08.000000 hotsos-1.16.0.post1/hotsos/plugin_extensions/openstack/summary.py
+-rw-r--r--   0 runner    (1001) docker     (123)     7226 2023-07-21 07:19:08.000000 hotsos-1.16.0.post1/hotsos/plugin_extensions/openstack/vm_info.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-21 07:19:29.863990 hotsos-1.16.0.post1/hotsos/plugin_extensions/openvswitch/
+-rw-r--r--   0 runner    (1001) docker     (123)        0 2023-07-21 07:19:08.000000 hotsos-1.16.0.post1/hotsos/plugin_extensions/openvswitch/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)     9976 2023-07-21 07:19:08.000000 hotsos-1.16.0.post1/hotsos/plugin_extensions/openvswitch/event_checks.py
+-rw-r--r--   0 runner    (1001) docker     (123)     3052 2023-07-21 07:19:08.000000 hotsos-1.16.0.post1/hotsos/plugin_extensions/openvswitch/summary.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-21 07:19:29.863990 hotsos-1.16.0.post1/hotsos/plugin_extensions/pacemaker/
+-rw-r--r--   0 runner    (1001) docker     (123)        0 2023-07-21 07:19:08.000000 hotsos-1.16.0.post1/hotsos/plugin_extensions/pacemaker/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)      678 2023-07-21 07:19:08.000000 hotsos-1.16.0.post1/hotsos/plugin_extensions/pacemaker/summary.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-21 07:19:29.863990 hotsos-1.16.0.post1/hotsos/plugin_extensions/rabbitmq/
+-rw-r--r--   0 runner    (1001) docker     (123)        0 2023-07-21 07:19:08.000000 hotsos-1.16.0.post1/hotsos/plugin_extensions/rabbitmq/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)     2398 2023-07-21 07:19:08.000000 hotsos-1.16.0.post1/hotsos/plugin_extensions/rabbitmq/summary.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-21 07:19:29.863990 hotsos-1.16.0.post1/hotsos/plugin_extensions/sosreport/
+-rw-r--r--   0 runner    (1001) docker     (123)        0 2023-07-21 07:19:08.000000 hotsos-1.16.0.post1/hotsos/plugin_extensions/sosreport/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)      530 2023-07-21 07:19:08.000000 hotsos-1.16.0.post1/hotsos/plugin_extensions/sosreport/summary.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-21 07:19:29.863990 hotsos-1.16.0.post1/hotsos/plugin_extensions/storage/
+-rw-r--r--   0 runner    (1001) docker     (123)        0 2023-07-21 07:19:08.000000 hotsos-1.16.0.post1/hotsos/plugin_extensions/storage/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)      715 2023-07-21 07:19:08.000000 hotsos-1.16.0.post1/hotsos/plugin_extensions/storage/bcache_summary.py
+-rw-r--r--   0 runner    (1001) docker     (123)     4472 2023-07-21 07:19:08.000000 hotsos-1.16.0.post1/hotsos/plugin_extensions/storage/ceph_event_checks.py
+-rw-r--r--   0 runner    (1001) docker     (123)     2366 2023-07-21 07:19:08.000000 hotsos-1.16.0.post1/hotsos/plugin_extensions/storage/ceph_summary.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-21 07:19:29.863990 hotsos-1.16.0.post1/hotsos/plugin_extensions/system/
+-rw-r--r--   0 runner    (1001) docker     (123)        0 2023-07-21 07:19:08.000000 hotsos-1.16.0.post1/hotsos/plugin_extensions/system/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)     6474 2023-07-21 07:19:08.000000 hotsos-1.16.0.post1/hotsos/plugin_extensions/system/checks.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1350 2023-07-21 07:19:08.000000 hotsos-1.16.0.post1/hotsos/plugin_extensions/system/summary.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-21 07:19:29.863990 hotsos-1.16.0.post1/hotsos/plugin_extensions/vault/
+-rw-r--r--   0 runner    (1001) docker     (123)        0 2023-07-21 07:19:08.000000 hotsos-1.16.0.post1/hotsos/plugin_extensions/vault/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)      466 2023-07-21 07:19:08.000000 hotsos-1.16.0.post1/hotsos/plugin_extensions/vault/summary.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-21 07:19:29.867990 hotsos-1.16.0.post1/hotsos/templates/
+-rw-r--r--   0 runner    (1001) docker     (123)      232 2023-07-21 07:19:08.000000 hotsos-1.16.0.post1/hotsos/templates/content_dict.html
+-rw-r--r--   0 runner    (1001) docker     (123)      116 2023-07-21 07:19:08.000000 hotsos-1.16.0.post1/hotsos/templates/content_list.html
+-rw-r--r--   0 runner    (1001) docker     (123)       15 2023-07-21 07:19:08.000000 hotsos-1.16.0.post1/hotsos/templates/footer.html
+-rw-r--r--   0 runner    (1001) docker     (123)     2335 2023-07-21 07:19:08.000000 hotsos-1.16.0.post1/hotsos/templates/header.html
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-21 07:19:29.823989 hotsos-1.16.0.post1/hotsos.egg-info/
+-rw-r--r--   0 runner    (1001) docker     (123)     1195 2023-07-21 07:19:29.000000 hotsos-1.16.0.post1/hotsos.egg-info/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (123)    15413 2023-07-21 07:19:29.000000 hotsos-1.16.0.post1/hotsos.egg-info/SOURCES.txt
+-rw-r--r--   0 runner    (1001) docker     (123)        1 2023-07-21 07:19:29.000000 hotsos-1.16.0.post1/hotsos.egg-info/dependency_links.txt
+-rw-r--r--   0 runner    (1001) docker     (123)       43 2023-07-21 07:19:29.000000 hotsos-1.16.0.post1/hotsos.egg-info/entry_points.txt
+-rw-r--r--   0 runner    (1001) docker     (123)      135 2023-07-21 07:19:29.000000 hotsos-1.16.0.post1/hotsos.egg-info/requires.txt
+-rw-r--r--   0 runner    (1001) docker     (123)        7 2023-07-21 07:19:29.000000 hotsos-1.16.0.post1/hotsos.egg-info/top_level.txt
+-rw-r--r--   0 runner    (1001) docker     (123)     1063 2023-07-21 07:19:08.000000 hotsos-1.16.0.post1/pyproject.toml
+-rw-r--r--   0 runner    (1001) docker     (123)       38 2023-07-21 07:19:29.867990 hotsos-1.16.0.post1/setup.cfg
+-rw-r--r--   0 runner    (1001) docker     (123)      123 2023-07-21 07:19:08.000000 hotsos-1.16.0.post1/setup.py
```

### Comparing `hotsos-1.15.post9/LICENSE` & `hotsos-1.16.0.post1/LICENSE`

 * *Files identical despite different names*

### Comparing `hotsos-1.15.post9/PKG-INFO` & `hotsos-1.16.0.post1/PKG-INFO`

 * *Files 2% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: hotsos
-Version: 1.15.post9
+Version: 1.16.0.post1
 Summary: Software analysis toolkit. Define checks in high-level language and leverage library to perform analysis of common Cloud applications.
 Requires-Python: >=3.8
 Description-Content-Type: text/markdown
 License-File: LICENSE
 
 # Hotsos
```

### Comparing `hotsos-1.15.post9/README.md` & `hotsos-1.16.0.post1/README.md`

 * *Files identical despite different names*

### Comparing `hotsos-1.15.post9/hotsos/cli.py` & `hotsos-1.16.0.post1/hotsos/cli.py`

 * *Files 6% similar despite different names*

```diff
@@ -5,23 +5,30 @@
 import sys
 import threading
 from importlib import metadata, resources
 
 import click
 import distro
 from progress.spinner import Spinner
+from hotsos.core.root_manager import DataRootManager
 from hotsos.core.config import HotSOSConfig
 from hotsos.core.log import setup_logging, log
-from hotsos.core.host_helpers import CLIHelper
 from hotsos.client import (
     HotSOSClient,
     OutputManager,
     PLUGIN_CATALOG,
 )
 
+SNAP_ERROR_MSG = """ERROR: hotsos is installed as a snap which only supports
+running against a sosreport due to access restrictions.
+
+If you want to analyse a host you need to use an alternative installation
+method e.g. debian package - see https://hotsos.readthedocs.io/en/latest/install/index.html for more information."
+""" # noqa
+
 
 def is_snap():
     return os.environ.get('SNAP_NAME', '') == 'hotsos'
 
 
 def get_os_id():
     return distro.id()
@@ -139,43 +146,20 @@
     try:
         yield thread
     finally:
         done.set()
         thread.join()
 
 
-def fix_data_root(data_root):
-    if not data_root:
-        data_root = '/'
-    elif data_root[-1] != '/':
-        # Ensure trailing slash
-        data_root += '/'
-    return data_root
-
-
-def get_analysis_target(data_root):
-    if data_root == '/':
-        analysis_target = 'localhost'
-    else:
-        analysis_target = 'sosreport {}'.format(data_root)
-    return analysis_target
-
-
-def get_prefix(data_root):
-    if data_root != '/':
-        if data_root.endswith('/'):
-            data_root = data_root.rpartition('/')[0]
-
-        return os.path.basename(data_root)
-
-    return CLIHelper().hostname()
-
-
 def main():
     @click.command(name='hotsos')
+    @click.option('--sos-unpack-dir', default=None,
+                  help=('Location used to unpack sosreports. Useful if you '
+                        'want to cache the unpacked sosreport for subsequent '
+                        'use. The provided path must exist.'))
     @click.option('--command-timeout', default=HotSOSConfig.command_timeout,
                   help=('Amount of time command execution will wait before '
                         'timing out and moving on.'))
     @click.option('--allow-constraints-for-unverifiable-logs', default=False,
                   is_flag=True)
     @click.option('--output-path', default=None,
                   help=('Optional path to use for saving output (with '
@@ -190,16 +174,14 @@
                         'used is limited to a max of 8. You can '
                         'override that value with this option.'))
     @click.option('--max-logrotate-depth', default=7,
                   help=('Searching all available logrotate history for a '
                         'given log file can be costly so we cap the history '
                         'to this value. Only applies when --all-logs is '
                         'provided.'))
-    @click.option('--agent-error-key-by-time', default=False, is_flag=True,
-                  help='DEPRECATED: use --event-tally-granularity')
     @click.option('--event-tally-granularity', default='date',
                   help=('By default event tallies will be grouped by date, '
                         'for example when tallying occurrences of an event '
                         'in a file and displaying them in the summary. If '
                         'finer granularity is required this can be set to '
                         '"time".'))
     @click.option('--force', default=False, is_flag=True,
@@ -207,30 +189,21 @@
                         'pre-requisites are met (i.e. they are "runnable").'
                         'It might sometimes be the case that not all '
                         'pre-requisites are available but we still want to '
                         'try running plugins. An example would be where an '
                         "application is not installed but we have it's logs. "
                         'Using this option can obviously produce '
                         'unexpected results so should be used with caution.'))
-    @click.option('--full', default=False, is_flag=True,
-                  help=('[DEPRECATED] This is the default and tells hotsos to '
-                        'generate a full summary. If you want to save both a '
-                        'short and full summary you can specifiy this option '
-                        'when doing --short.'))
     @click.option('--very-short', default=False, is_flag=True,
                   help=('Minimal version of --short where only issue types or '
                         'bug ids are displayed with count of each (issues '
                         'only).'))
     @click.option('--short', default=False, is_flag=True,
                   help=('Filters the full summary so that it only includes '
                         'plugin known-bugs and potential-issues sections.'))
-    @click.option('--user-summary', default=None,
-                  help=('[DEPRECATED] Provide an existing summary so that it '
-                        'can be post-processed e.g. --format json. This '
-                        'option is deprecated and no longer does anything'))
     @click.option('--html-escape', default=False, is_flag=True,
                   help=('Apply html escaping to the output so that it is safe '
                         'to display in html.'))
     @click.option('--format', '--output-format', 'output_format',
                   type=click.Choice(OutputManager.SUMMARY_FORMATS),
                   default='yaml',
                   show_default=True,
@@ -246,31 +219,30 @@
     @click.option('--all-logs', default=False, is_flag=True,
                   help=('Some plugins may choose to only analyse the most '
                         'recent version of a log file by default since '
                         'parsing the full history could take a lot '
                         'longer. This tells plugins that we wish to analyse '
                         'all available log history (see --max-logrotate-depth '
                         'for limits).'))
-    @click.option('--defs-path', default=get_defs_path(),
-                  help='Path to yaml definitions (ydefs).')
     @click.option('--templates-path', default=get_templates_path(),
                   help='Path to Jinja templates.')
+    @click.option('--defs-path', default=get_defs_path(),
+                  help='Path to yaml definitions (ydefs).')
     @click.option('--version', '-v', default=False, is_flag=True,
                   help='Show the version.')
     @set_plugin_options
     @click.argument('data_root', required=False, type=click.Path(exists=True))
-    def cli(data_root, version, defs_path, templates_path, all_logs, quiet,
-            debug, save, output_format, html_escape, short, very_short,
-            force, full, agent_error_key_by_time, event_tally_granularity,
-            max_logrotate_depth, max_parallel_tasks, list_plugins,
-            machine_readable, output_path,
+    def cli(data_root, version, defs_path, templates_path, all_logs, debug,
+            quiet, save, output_format, html_escape, short, very_short,
+            force, event_tally_granularity, max_logrotate_depth,
+            max_parallel_tasks, list_plugins, machine_readable, output_path,
             allow_constraints_for_unverifiable_logs, command_timeout,
-            **kwargs):
+            sos_unpack_dir, **kwargs):
         """
-        Run this tool on a host or against an unpacked sosreport to perform
+        Run this tool on a host or against a sosreport to perform
         analysis of specific applications and the host itself. A summary of
         information is generated along with any issues or known bugs detected.
         Applications are defined as plugins and support currently includes
         Openstack, Kubernetes, Ceph and more (see --list-plugins). The
         standard output format is yaml to allow easy visual inspection and
         post-processing by other tools. Other formats are also supported.
 
@@ -280,22 +252,18 @@
 
         By default the output is printed to standard output. If saving to disk
         (--save) a directory called "hotsos-output" is created beneath which
         output is saved in all available formats e.g. yaml, json, short
 
         \b
         DATA_ROOT
-            Path to an unpacked sosreport. If none provided, will run against
-            local host.
+            Path to an sosreport. If none provided, will run against local
+            host.
         """  # noqa
 
-        if full:
-            # deprecated
-            pass
-
         minimal_mode = None
         if short:
             minimal_mode = 'short'
         elif very_short:
             minimal_mode = 'very-short'
 
         HotSOSConfig.force_mode = force
@@ -307,91 +275,77 @@
         HotSOSConfig.hotsos_version = _version
         HotSOSConfig.command_timeout = command_timeout
 
         if version:
             print(_version)
             return
 
-        data_root = fix_data_root(data_root)
-
-        if is_snap() and data_root == '/':
-            print("ERROR: hotsos is installed as a snap which only "
-                  "supports running against a sosreport due to access "
-                  "restrictions.\n\n"
-                  "If you want to analyse a host you need to "
-                  "use an alternative installation method e.g. debian "
-                  "package - see "
-                  "https://hotsos.readthedocs.io/en/latest/install/index.html"
-                  " for more information.")
-            sys.exit(1)
-
-        if agent_error_key_by_time:
-            print("WARNING: option --agent-error-key-by-time is DEPRECATED "
-                  "and longer has any effect. Use --event-tally-granularity "
-                  "instead.")
-
-        HotSOSConfig.set(use_all_logs=all_logs, plugin_yaml_defs=defs_path,
-                         templates_path=templates_path, data_root=data_root,
-                         event_tally_granularity=event_tally_granularity,
-                         max_logrotate_depth=max_logrotate_depth,
-                         max_parallel_tasks=max_parallel_tasks,
-                         machine_readable=machine_readable)
-        HotSOSConfig.allow_constraints_for_unverifiable_logs = \
-            allow_constraints_for_unverifiable_logs
-
-        if debug and quiet:
-            sys.stderr.write('ERROR: cannot use both --debug and --quiet\n')
-            return
-
-        HotSOSConfig.debug_mode = debug
-
-        setup_logging()
-        # Set a name so that logs have this until real plugins are run.
-        log.name = 'hotsos.cli'
-
-        if list_plugins:
-            sys.stdout.write('\n'.join(PLUGIN_CATALOG.keys()))
-            sys.stdout.write('\n')
-            return
-
-        analysis_target = get_analysis_target(data_root)
-
-        if quiet:
-            show_spinner = False
-            spinner_msg = ''
-        else:
-            show_spinner = not debug
-            spinner_msg = 'INFO: analysing {} '.format(analysis_target)
-
-        with progress_spinner(show_spinner, spinner_msg):
-            plugins = []
-            for k, v in kwargs.items():
-                if v is True:
-                    plugins.append(k)
-
-            if plugins:
-                # always run these
-                plugins.append('hotsos')
-                if 'system' not in plugins:
-                    plugins.append('system')
-
-            client = HotSOSClient(plugins)
-            client.run()
-            summary = client.summary
-
-        if save:
-            prefix = get_prefix(data_root)
-            path = summary.save(prefix, html_escape=html_escape,
-                                output_path=output_path)
-            sys.stdout.write("INFO: output saved to {}\n".format(path))
-        else:
-            out = summary.get(fmt=output_format, html_escape=html_escape,
-                              minimal_mode=minimal_mode)
-            if out:
-                sys.stdout.write("{}\n".format(out))
+        with DataRootManager(data_root, sos_unpack_dir=sos_unpack_dir) as drm:
+            if is_snap() and drm.data_root == '/':
+                print(SNAP_ERROR_MSG)
+                sys.exit(1)
+
+            HotSOSConfig.set(use_all_logs=all_logs, plugin_yaml_defs=defs_path,
+                             templates_path=templates_path,
+                             data_root=drm.data_root,
+                             event_tally_granularity=event_tally_granularity,
+                             max_logrotate_depth=max_logrotate_depth,
+                             max_parallel_tasks=max_parallel_tasks,
+                             machine_readable=machine_readable)
+            HotSOSConfig.allow_constraints_for_unverifiable_logs = \
+                allow_constraints_for_unverifiable_logs
+
+            if debug and quiet:
+                sys.stderr.write('ERROR: cannot use both --debug and '
+                                 '--quiet\n')
+                return
+
+            HotSOSConfig.debug_mode = debug
+
+            setup_logging()
+            # Set a name so that logs have this until real plugins are run.
+            log.name = 'hotsos.cli'
+
+            if list_plugins:
+                sys.stdout.write('\n'.join(PLUGIN_CATALOG.keys()))
+                sys.stdout.write('\n')
+                return
+
+            if quiet:
+                show_spinner = False
+                spinner_msg = ''
+            else:
+                show_spinner = not debug
+                spinner_msg = 'INFO: analysing {} '.format(drm.name)
+
+            with progress_spinner(show_spinner, spinner_msg):
+                plugins = []
+                for k, v in kwargs.items():
+                    if v is True:
+                        plugins.append(k)
+
+                if plugins:
+                    # always run these
+                    plugins.append('hotsos')
+                    if 'system' not in plugins:
+                        plugins.append('system')
+
+                client = HotSOSClient(plugins)
+                client.run()
+                summary = client.summary
+
+            if save:
+                path = summary.save(drm.basename, html_escape=html_escape,
+                                    output_path=output_path)
+                sys.stdout.write("INFO: output saved to {}\n".format(path))
+            else:
+                out = summary.get(fmt=output_format, html_escape=html_escape,
+                                  minimal_mode=minimal_mode)
+                if out:
+                    sys.stdout.write("{}\n".format(out))
 
     cli(prog_name='hotsos')
 
 
 def exit_if_os_version_not_supported_in_snap():
     if is_snap():
         if get_os_id() != 'ubuntu':
```

### Comparing `hotsos-1.15.post9/hotsos/client.py` & `hotsos-1.16.0.post1/hotsos/client.py`

 * *Files identical despite different names*

### Comparing `hotsos-1.15.post9/hotsos/core/analytics.py` & `hotsos-1.16.0.post1/hotsos/core/analytics.py`

 * *Files identical despite different names*

### Comparing `hotsos-1.15.post9/hotsos/core/config.py` & `hotsos-1.16.0.post1/hotsos/core/config.py`

 * *Files identical despite different names*

### Comparing `hotsos-1.15.post9/hotsos/core/factory.py` & `hotsos-1.16.0.post1/hotsos/core/factory.py`

 * *Files identical despite different names*

### Comparing `hotsos-1.15.post9/hotsos/core/host_helpers/__init__.py` & `hotsos-1.16.0.post1/hotsos/core/host_helpers/__init__.py`

 * *Files 4% similar despite different names*

```diff
@@ -1,8 +1,11 @@
-from .cli import CLIHelper  # noqa: F403,F401
+from .cli import (  # noqa: F403,F401
+    CLIHelper,
+    CLIHelperFile,
+)
 from .config import (  # noqa: F403,F401
     ConfigBase,
     SectionalConfigBase,
 )
 from .network import (  # noqa: F403,F401
     NetworkPort,
     HostNetworkingHelper,
```

### Comparing `hotsos-1.15.post9/hotsos/core/host_helpers/cli.py` & `hotsos-1.16.0.post1/hotsos/core/host_helpers/cli.py`

 * *Files 6% similar despite different names*

```diff
@@ -1,15 +1,17 @@
+import abc
 import datetime
 import glob
 import json
 import os
 import pickle
 import re
 import subprocess
 import tempfile
+from functools import cached_property
 
 from hotsos.core.config import HotSOSConfig
 from hotsos.core.host_helpers.common import HostHelpersBase
 from hotsos.core.log import log
 
 CLI_COMMON_EXCEPTIONS = (OSError, subprocess.CalledProcessError,
                          subprocess.TimeoutExpired,
@@ -49,24 +51,24 @@
 
 
 class SourceNotFound(Exception):
     pass
 
 
 class CommandNotFound(Exception):
-    def __init__(self, cmd):
-        self.msg = "command not found in catalog: '{}'".format(cmd)
+    def __init__(self, cmd, msg):
+        self.msg = "command '{}' not found in catalog: '{}'".format(cmd, msg)
 
     def __str__(self):
         return self.msg
 
 
 class NullSource(object):
     def __call__(self, *args, **kwargs):
-        return []
+        return CmdOutput([])
 
 
 def run_pre_exec_hooks(f):
     """ pre-exec hooks are run before running __call__ method.
 
     These hooks are not expected to return anything and are used to manipulate
     the instance variables used by the main __call__ method.
@@ -106,14 +108,20 @@
         out = f(self, *args, **kwargs)
         self.reset()
         return out
 
     return reset_command_inner
 
 
+class CmdOutput(object):
+    def __init__(self, value, source=None):
+        self.value = value
+        self.source = source
+
+
 class CmdBase(object):
     """ Base class for all command source types. """
 
     def __init__(self):
         self.hooks = {}
         self.reset()
 
@@ -171,72 +179,107 @@
         if args:
             cmd = cmd.format(*args)
 
         if kwargs:
             cmd = cmd.format(**kwargs)
 
         _cmd = cmd.split() + self.original_cmd_extras
-        output = subprocess.check_output(_cmd,
-                                         timeout=HotSOSConfig.command_timeout,
-                                         stderr=subprocess.STDOUT)
+        out = subprocess.run(_cmd, timeout=HotSOSConfig.command_timeout,
+                             capture_output=True, check=False)
+        output = out.stdout
+        if out.stderr:
+            output += out.stderr
+
+        if out.returncode != 0:
+            log.info("command '%s' exited with non-zero code '%s'", cmd,
+                     out.returncode)
+
+        try:
+            output = output.decode('UTF-8')
+        except UnicodeDecodeError:
+            log.exception("failed to decode command output for '%s'", cmd)
+            output = ''
 
         if self.json_decode:
-            return json.loads(output.decode('UTF-8'))
+            return CmdOutput(json.loads(output))
 
         if self.singleline:
-            return output.decode('UTF-8').strip()
+            return CmdOutput(output.strip())
 
-        return output.decode('UTF-8').splitlines(keepends=True)
+        return CmdOutput(output.splitlines(keepends=True))
 
 
 class FileCmd(CmdBase):
     TYPE = "FILE"
 
-    def __init__(self, path, safe_decode=False, json_decode=False,
-                 singleline=False):
+    def __init__(self, path, json_decode=False,
+                 singleline=False, decode_error_handling=None):
         self.original_path = os.path.join(HotSOSConfig.data_root, path)
-        self.original_safe_decode = safe_decode
         self.original_json_decode = json_decode
         self.original_singleline = singleline
+        self.original_decode_error_handling = decode_error_handling
         super().__init__()
 
     def reset(self):
         self.path = self.original_path
-        self.safe_decode = self.original_safe_decode
         self.json_decode = self.original_json_decode
         self.singleline = self.original_singleline
+        self.decode_error_handling = self.original_decode_error_handling
 
     @catch_exceptions(*CLI_COMMON_EXCEPTIONS)
     @reset_command
     @run_post_exec_hooks
     @run_pre_exec_hooks
-    def __call__(self, *args, **kwargs):
+    def __call__(self, *args, skip_load_contents=False, **kwargs):
         if args:
             self.path = self.path.format(*args)
 
         if kwargs:
             self.path = self.path.format(**kwargs)
 
         if not os.path.exists(self.path):
             raise SourceNotFound()
 
-        # NOTE: any post-exec hooks much be aware that their input will be
+        if skip_load_contents:
+            CmdOutput(None, self.path)
+
+        # NOTE: any post-exec hooks must be aware that their input will be
         # defined by the following.
-        if self.safe_decode:
-            # Some content can result in UnicodeDecodeError so use
-            # surrogateescape but only seldom.
-            output = self.safe_readlines(self.path)
-        elif self.json_decode:
+        if self.json_decode:
             output = json.load(open(self.path))
         else:
-            output = open(self.path, 'r').readlines()
+            output = []
+            ln = 0
+            with open(self.path, 'rb') as fd:
+                for line in fd:
+                    ln += 1
+                    try:
+                        decode_kwargs = {}
+                        if self.decode_error_handling:
+                            decode_kwargs['errors'] = \
+                                                     self.decode_error_handling
+
+                        _out = line.decode(**decode_kwargs)
+                        output.append(_out)
+                    except UnicodeDecodeError:
+                        # maintain line count but store empty line.
+                        # we could in the future consider other decode options
+                        # as a fallback.
+                        output.append('')
+                        log.exception("failed to decode line %s "
+                                      "(decode_error_handling=%s)", ln,
+                                      self.decode_error_handling)
+
+                    if self.singleline:
+                        break
+
             if self.singleline:
-                return output[0].strip()
+                return CmdOutput(output[0].strip(), self.path)
 
-        return output
+        return CmdOutput(output, self.path)
 
 
 class BinFileCmd(FileCmd):
     """ This is used when we are executing an actual binary/command against a
     file. """
 
     @catch_exceptions(*CLI_COMMON_EXCEPTIONS)
@@ -256,24 +299,25 @@
             self.path = self.path.format(**kwargs)
 
         # If this file is part of a sosreport we want to make sure it is run
         # in the same timezone context as the sosreport host.
         env = {}
         try:
             env['TZ'] = DateFileCmd('sos_commands/date/date',
-                                    singleline=True)(format="+%Z")
+                                    singleline=True)(format="+%Z").value
         except SourceNotFound:
             pass
 
         # Now split into a command and run
         output = subprocess.check_output(self.path.split(),
                                          timeout=HotSOSConfig.command_timeout,
                                          stderr=subprocess.STDOUT, env=env)
 
-        return output.decode('UTF-8').splitlines(keepends=True)
+        output = output.decode('UTF-8')
+        return CmdOutput(output.splitlines(keepends=True))
 
 
 class JournalctlBase(object):
 
     @property
     def since_date(self):
         """
@@ -364,15 +408,15 @@
             self.reset()
             self.cmd = "ovs-ofctl -O {} {}".format(ver, self.cmd)
             try:
                 return super().__call__(*args, **kwargs)
             except CLIExecError:
                 log.debug("ofctl command with protocol version %s failed", ver)
 
-        return []
+        return CmdOutput([])
 
 
 class DateBinCmd(BinCmd):
 
     def __init__(self, *args, **kwargs):
         super().__init__(*args, **kwargs)
         self.register_hook("pre-exec", self.format_date_cmd)
@@ -393,28 +437,32 @@
 class DateFileCmd(FileCmd):
 
     def __init__(self, *args, **kwargs):
         super().__init__(*args, **kwargs)
         self.register_hook("post-exec", self.format_date)
 
     def format_date(self, output, **kwargs):
-        """ Apply some post-processing to the date output. """
+        """ Apply some post-processing to the date output.
+
+        @param output: CmdOutput object
+        """
         no_format = kwargs.get('no_format', False)
         fmt = kwargs.get('format')
         if not no_format and fmt is None:
             fmt = '+%s'
 
         ret = re.match(r"^(\S+ \S*\s*[0-9]+ [0-9:]+)\s*"
                        r"([A-Z]*|[+-]?[0-9]*)?"
                        r"\s*([0-9]+)$",
-                       output)
+                       output.value)
 
         if ret is None:
-            log.error("%s has invalid date string '%s'", self.path, output)
-            return ""
+            log.error("%s has invalid date string '%s'", self.path,
+                      output.value)
+            return CmdOutput('', self.path)
 
         tz = ret[2]
         # NOTE: date command doesn't recognise HKT for some reason so we
         # convert to a format that is recognised.
         if tz == 'HKT':
             tz = 'UTC+8'
 
@@ -427,15 +475,15 @@
         output = subprocess.check_output(cmd,
                                          timeout=HotSOSConfig.command_timeout)
         # date sometimes adds multiple whitespaces between fields so collapse
         # them.
         output = re.compile(r"\s+").sub(' ', output.decode('UTF-8'))
         ret = output.splitlines(keepends=True)[0]
         # always singleline so always strip trailing newline
-        return ret.strip()
+        return CmdOutput(ret.strip(), self.path)
 
 
 class CephJSONFileCmd(FileCmd):
     """
     Some ceph commands that use --format json have some extra text added to the
     end of the file (typically from stderr) which causes it to be invalid json
     so we have to strip that final line before decoding the contents.
@@ -467,55 +515,39 @@
             with tempfile.NamedTemporaryFile(mode='w+t', delete=False) as tmp:
                 tmp.write(''.join(lines))
                 tmp.close()
                 self.orig_path = self.path
                 self.path = tmp.name
 
     def cleanup(self, output, **kwargs):  # pylint: disable=W0613
+        """
+        @param output: CmdOutput object
+        """
         if self.orig_path:
             os.unlink(self.path)
             self.path = self.orig_path
             self.orig_path = None
 
         return output
 
 
 class SourceRunner(object):
 
-    def __init__(self, cmdkey, sources, cache):
+    def __init__(self, cmdkey, sources, cache, output_file=None):
         """
         @param cmdkey: unique key identifying this command.
         @param sources: list of command source implementations.
         @param cache: CLICacheWrapper object.
         """
         self.cmdkey = cmdkey
         self.sources = sources
         self.cache = cache
+        self.output_file = output_file
 
-    def __call__(self, *args, **kwargs):
-        """
-        Execute the command using the appropriate source runner. These can be
-        binary or file-based depending on whether data root points to / or a
-        sosreport. File-based are attempted first.
-
-        A command can have more than one source implementation so we must
-        ensure they all have a chance to run.
-        """
-        # always try file sources first
-        for fsource in [s for s in self.sources if s.TYPE == "FILE"]:
-            try:
-                return fsource(*args, **kwargs)
-            except CLIExecError as exc:
-                return exc.return_value
-            except SourceNotFound:
-                pass
-
-        if HotSOSConfig.data_root != '/':
-            return NullSource()()
-
+    def bsource(self, *args, **kwargs):
         # binary sources only apply if data_root is system root
         bin_out = None
         for bsource in [s for s in self.sources if s.TYPE == "BIN"]:
             cache = False
             # NOTE: we currently only support caching commands with no
             #       args.
             if not any([args, kwargs]):
@@ -533,33 +565,82 @@
                         log.info("unable to cache command '%s' output: %s",
                                  self.cmdkey, exc)
 
                 # if command executed but returned nothing that still counts
                 # as success.
                 break
             except CLIExecError as exc:
-                bin_out = exc.return_value
+                bin_out = CmdOutput(exc.return_value)
 
         return bin_out
 
+    def fsource(self, *args, **kwargs):
+        for fsource in [s for s in self.sources if s.TYPE == "FILE"]:
+            try:
+                skip_load_contents = False
+                if self.output_file:
+                    skip_load_contents = True
+
+                return fsource(*args, **kwargs,
+                               skip_load_contents=skip_load_contents)
+            except CLIExecError as exc:
+                return CmdOutput(exc.return_value)
+            except SourceNotFound:
+                pass
+
+    def _execute(self, *args, **kwargs):
+        # always try file sources first
+        ret = self.fsource(*args, **kwargs)
+        if ret is not None:
+            return ret
+
+        if HotSOSConfig.data_root != '/':
+            return NullSource()()
+
+        return self.bsource(*args, **kwargs)
+
+    def __call__(self, *args, **kwargs):
+        """
+        Execute the command using the appropriate source runner. These can be
+        binary or file-based depending on whether data root points to / or a
+        sosreport. File-based are attempted first.
+
+        A command can have more than one source implementation so we must
+        ensure they all have a chance to run.
+        """
+        out = self._execute(*args, **kwargs)
+        if self.output_file:
+            if out.source is not None:
+                return out.source
+
+            with open(self.output_file, 'w') as fd:
+                if isinstance(out.value, list):
+                    fd.write(''.join(out.value))
+                else:
+                    fd.write(out.value)
+
+                return self.output_file
+
+        return out.value
+
 
 class CLICacheWrapper(object):
 
     def __init__(self, cache_load_f, cache_save_f):
         self.load_f = cache_load_f
         self.save_f = cache_save_f
 
     def load(self, key):
         return self.load_f(key)
 
     def save(self, key, value):
         return self.save_f(key, value)
 
 
-class CLIHelper(HostHelpersBase):
+class CLIHelperBase(HostHelpersBase):
 
     def __init__(self):
         self._command_catalog = None
         super().__init__()
         self.cli_cache = CLICacheWrapper(self.cache_load, self.cache_save)
 
     @property
@@ -749,15 +830,16 @@
                 [BinCmd('docker images'),
                  FileCmd('sos_commands/docker/docker_images')],
             'docker_ps':
                 [BinCmd('docker ps'),
                  FileCmd('sos_commands/docker/docker_ps')],
             'dpkg_l':
                 [BinCmd('dpkg -l'),
-                 FileCmd('sos_commands/dpkg/dpkg_-l', safe_decode=True)],
+                 FileCmd('sos_commands/dpkg/dpkg_-l',
+                         decode_error_handling='surrogateecape')],
             'ethtool':
                 [BinCmd('ethtool {interface}'),
                  FileCmd('sos_commands/networking/ethtool_{interface}')],
             'hostname':
                 [BinCmd('hostname', singleline=True),
                  FileCmd('hostname', singleline=True)],
             'hostnamectl':
@@ -875,15 +957,16 @@
                  # sos legacy
                  FileCmd('sos_commands/snappy/snap_list_--all')],
             'sysctl_all':
                 [BinCmd('sysctl -a'),
                  FileCmd('sos_commands/kernel/sysctl_-a')],
             'systemctl_status_all':
                 [BinCmd('systemctl status --all'),
-                 FileCmd('sos_commands/systemd/systemctl_status_--all')],
+                 FileCmd('sos_commands/systemd/systemctl_status_--all',
+                         decode_error_handling='backslashreplace')],
             'systemctl_list_units':
                 [BinCmd('systemctl list-units'),
                  FileCmd('sos_commands/systemd/systemctl_list-units')],
             'systemctl_list_unit_files':
                 [BinCmd('systemctl list-unit-files'),
                  FileCmd('sos_commands/systemd/systemctl_list-unit-files')],
             'udevadm_info_dev':
@@ -897,20 +980,83 @@
                  FileCmd('sos_commands/kernel/uname_-a', singleline=True)],
             'uptime':
                 [BinCmd('uptime', singleline=True),
                  FileCmd('uptime', singleline=True)],
         }
         return self._command_catalog
 
+    @abc.abstractmethod
+    def __getattr__(self, cmdname):
+        """ This is how commands are run. The command is looked up in the
+        catalog and it's runner object is returned. The caller is expetced to
+        call() the returned object to execute the command.
+
+        @param cmdname: name of command we want to execute. This must match a
+        name used to register a handler in the catalog.
+        @return: SourceRunner object.
+        """
+
+
+class CLIHelper(CLIHelperBase):
+    """
+    This is used when we want to have command output as the return value when
+    a command is executed.
+    """
+
     def __getattr__(self, cmdname):
-        cmd = self.command_catalog.get(cmdname)
-        if cmd:
-            return SourceRunner(cmdname, cmd, self.cli_cache)
+        try:
+            return SourceRunner(cmdname, self.command_catalog[cmdname],
+                                self.cli_cache)
+        except KeyError as exc:
+            raise CommandNotFound(cmdname, exc) from exc
+
 
-        raise CommandNotFound(cmdname)
+class CLIHelperFile(CLIHelperBase):
+    """
+    This is used when we want the return value of a command to be a path to a
+    file containing the return value of executing that command.
+
+    This will do one of two things; if the command output originates from a
+    file e.g. a sosreport command output file, it will return the path to that
+    file. If the command is executed as a binary, its output is written to a
+    temporary file and the path to that file is returned.
+    """
+
+    def __init__(self, *args, delete_temp=True, **kwargs):
+        super().__init__(*args, **kwargs)
+        self.delete_temp = delete_temp
+        self._tmp_file_mtime = None
+
+    def __enter__(self):
+        return self
+
+    def __exit__(self, *args, **kwargs):
+        do_delete = (self.delete_temp or
+                     self._tmp_file_mtime ==
+                     os.path.getmtime(self.output_file))
+        if do_delete:
+            os.remove(self.output_file)
+
+        # We want exceptions to be raised
+        return False
+
+    @cached_property
+    def output_file(self):
+        path = tempfile.mktemp(dir=HotSOSConfig.plugin_tmp_dir)
+        open(path, 'w').close()
+        self._tmp_file_mtime = os.path.getmtime(path)
+        return path
+
+    def __getattr__(self, cmdname):
+        try:
+            ret = SourceRunner(cmdname, self.command_catalog[cmdname],
+                               self.cli_cache, output_file=self.output_file)
+            return ret
+        except KeyError as exc:
+            raise CommandNotFound(cmdname, exc) from exc
 
 
 def get_ps_axo_flags_available():
     path = os.path.join(HotSOSConfig.data_root,
                         "sos_commands/process/ps_axo_flags_state_"
                         "uid_pid_ppid_pgid_sid_cls_pri_addr_sz_wchan*_lstart_"
                         "tty_time_cmd")
```

### Comparing `hotsos-1.15.post9/hotsos/core/host_helpers/common.py` & `hotsos-1.16.0.post1/hotsos/core/host_helpers/common.py`

 * *Files identical despite different names*

### Comparing `hotsos-1.15.post9/hotsos/core/host_helpers/config.py` & `hotsos-1.16.0.post1/hotsos/core/host_helpers/config.py`

 * *Files identical despite different names*

### Comparing `hotsos-1.15.post9/hotsos/core/host_helpers/filestat.py` & `hotsos-1.16.0.post1/hotsos/core/host_helpers/filestat.py`

 * *Files identical despite different names*

### Comparing `hotsos-1.15.post9/hotsos/core/host_helpers/network.py` & `hotsos-1.16.0.post1/hotsos/core/host_helpers/network.py`

 * *Files 2% similar despite different names*

```diff
@@ -6,15 +6,15 @@
 #       avoid circular dependency issues.
 from searchkit import (
     FileSearcher,
     SearchDef,
     SequenceSearchDef,
 )
 from hotsos.core.config import HotSOSConfig
-from hotsos.core.host_helpers.cli import CLIHelper
+from hotsos.core.host_helpers.cli import CLIHelper, CLIHelperFile
 from hotsos.core.host_helpers.common import HostHelpersBase
 from hotsos.core.log import log
 from hotsos.core.utils import mktemp_dump
 
 # compatible with ip addr and ip link
 # this one is name and state
 IP_IFACE_NAME = r"^\d+:\s+(\S+):\s+.+state\s+(\S+)"
@@ -33,15 +33,14 @@
                  namespace=None):
         self.name = name
         self.addresses = addresses
         self.hwaddr = hwaddr
         self.state = state
         self.encap_info = encap_info
         self.namespace = namespace
-        self.cli_helper = CLIHelper()
         super().__init__()
 
     @property
     def cache_root(self):
         """
         Cache this information at the plugin level rather than globally.
         """
@@ -81,15 +80,15 @@
 
         return {self.name: info}
 
     @property
     def speed(self):
         # need to strip @* since sosreport does that too
         name = self.name.partition('@')[0]
-        out = self.cli_helper.ethtool(interface=name)
+        out = CLIHelper().ethtool(interface=name)
         if out:
             for line in out:
                 ret = re.match(r'\s*Speed:\s+(\S+)', line)
                 if ret:
                     return ret.group(1)
 
         return 'unknown'
@@ -106,23 +105,22 @@
                     # match start of interface
                     start=SearchDef(IP_IFACE_NAME_TEMPLATE.format(self.name)),
                     # match body of interface
                     body=SearchDef(r".+"),
                     # match next interface or EOF
                     end=SearchDef([IP_IFACE_NAME, IP_EOF]),
                     tag="ifaces")
-        f_ip_link_show = mktemp_dump(''.join(self.cli_helper.ip_link()))
-        s.add(seqdef, path=f_ip_link_show)
-        results = s.run()
-        os.unlink(f_ip_link_show)
         stats_raw = []
-        for section in results.find_sequence_sections(seqdef).values():
-            for result in section:
-                if result.tag == seqdef.body_tag:
-                    stats_raw.append(result.get(0))
+        with CLIHelperFile() as cli:
+            s.add(seqdef, path=cli.ip_link())
+            results = s.run()
+            for section in results.find_sequence_sections(seqdef).values():
+                for result in section:
+                    if result.tag == seqdef.body_tag:
+                        stats_raw.append(result.get(0))
 
         if not stats_raw:
             return {}
 
         # NOTE: we only expect one match
         for i, line in enumerate(stats_raw):
             ret = re.compile(r"\s+([RT]X):\s+.+").findall(line)
```

### Comparing `hotsos-1.15.post9/hotsos/core/host_helpers/packaging.py` & `hotsos-1.16.0.post1/hotsos/core/host_helpers/packaging.py`

 * *Files identical despite different names*

### Comparing `hotsos-1.15.post9/hotsos/core/host_helpers/pebble.py` & `hotsos-1.16.0.post1/hotsos/core/host_helpers/pebble.py`

 * *Files 2% similar despite different names*

```diff
@@ -1,14 +1,15 @@
 import re
+from functools import cached_property
 
 from hotsos.core.log import log
 from hotsos.core.factory import FactoryBase
 from hotsos.core.host_helpers import CLIHelper
 from hotsos.core.host_helpers.common import ServiceManagerBase
-from hotsos.core.utils import cached_property, sorted_dict
+from hotsos.core.utils import sorted_dict
 
 
 class PebbleService(object):
 
     def __init__(self, name, state):
         self.name = name
         self.state = state
```

### Comparing `hotsos-1.15.post9/hotsos/core/host_helpers/ssl.py` & `hotsos-1.16.0.post1/hotsos/core/host_helpers/ssl.py`

 * *Files identical despite different names*

### Comparing `hotsos-1.15.post9/hotsos/core/host_helpers/sysctl.py` & `hotsos-1.16.0.post1/hotsos/core/host_helpers/sysctl.py`

 * *Files 16% similar despite different names*

```diff
@@ -1,12 +1,12 @@
 import os
+from functools import cached_property
 
 from hotsos.core.factory import FactoryBase
 from hotsos.core.host_helpers.cli import CLIHelper
-from hotsos.core.utils import cached_property
 
 
 class SYSCtlFactory(FactoryBase):
     """
     Factory to create interface objects to sysctl. This allows us to load
     values dynamically without continuously loaded from the kernel.
     """
@@ -28,18 +28,14 @@
         """
         return self.sysctl_all.get(key)
 
     def __getattr__(self, name):
         """
         Return a value for given sysctl key.
         """
-        if name == '__cached_property_sysctl_all':
-            # require to allow the property caching to work
-            raise AttributeError()
-
         return self.get(name)
 
 
 class SYSCtlConfHelper(object):
 
     def __init__(self, path):
         self.path = path
```

### Comparing `hotsos-1.15.post9/hotsos/core/host_helpers/systemd.py` & `hotsos-1.16.0.post1/hotsos/core/host_helpers/systemd.py`

 * *Files 20% similar despite different names*

```diff
@@ -1,47 +1,86 @@
 import glob
 import os
 import re
 from datetime import datetime
+from functools import cached_property
 
+# NOTE: we import direct from searchkit rather than hotsos.core.search to
+#       avoid circular dependency issues.
+from searchkit import (
+    FileSearcher,
+    SearchDef,
+    SequenceSearchDef,
+)
 from hotsos.core.config import HotSOSConfig
 from hotsos.core.factory import FactoryBase
-from hotsos.core.host_helpers import CLIHelper
+from hotsos.core.host_helpers import CLIHelper, CLIHelperFile
 from hotsos.core.host_helpers.common import ServiceManagerBase
 from hotsos.core.log import log
-from hotsos.core.utils import cached_property, sorted_dict
+from hotsos.core.utils import sorted_dict
 
 
 class SystemdService(object):
 
     def __init__(self, name, state, has_instances=False):
         self.name = name
         self.state = state
         self.has_instances = has_instances
 
     @cached_property
     def start_time(self):
         """ Get most recent start time of this service unit.
 
+        We first look in systemd journal since that should be the fastest and
+        if not found (perhaps because service not restarted for a long time)
+        we look in service status.
+
         @returns: datetime.datetime object or None if time not found.
         """
         log.debug("fetching start time for svc %s", self.name)
-        # must be in short-iso format
-        cexpr = re.compile(r"^(([0-9-]+)T[\d:]+\+[\d]+)\s+.+: "
-                           "(Started|Starting) .+")
-        journal = CLIHelper().journalctl(unit=self.name)
+        cli = CLIHelper()
+        # must be in short-iso format e.g. 2023-07-04T00:05:23+0100
+        cexpr = re.compile(r"^(\d{4}-\d{2}-\d{2}T\d{2}:\d{2}:\d{2}\+\d{4})"
+                           r"\s+.+: (Started|Starting)")
+        journal = cli.journalctl(unit=self.name)
         last = None
         for line in journal:
             ret = cexpr.search(line)
             if ret:
                 last = ret.group(1)
 
         if last:
             return datetime.strptime(last, "%Y-%m-%dT%H:%M:%S%z")
 
+        log.debug("start time not found in journal, trying service status")
+        # NOTE: should consider getting service status directly rather than
+        #       searching in all but currently do this to have parity with
+        #       sosreport.
+        fs = FileSearcher()
+        # The following expressions need to take account of control characters
+        # that might exist in the output e.g. line can start with '*' or U+25CF
+        seqdef = SequenceSearchDef(
+                    start=SearchDef(r'\S+ ({}.service) -'.format(self.name)),
+                    body=SearchDef(r"\s+Active: active \(?\S*\)?\s*since "
+                                   r"\S{3} (\d{4}-\d{2}-\d{2} "
+                                   r"\d{2}:\d{2}:\d{2})"),
+                    end=SearchDef(r'(\S+) \S+.service'),
+                    tag='systemd')
+        with CLIHelperFile() as cli:
+            fs.add(seqdef, path=cli.systemctl_status_all())
+            sections = list(fs.run().find_sequence_sections(seqdef).values())
+            if len(sections) > 1:
+                log.warning("more than one status found for %s.service",
+                            self.name)
+
+            for result in sections[0]:
+                if result.tag == seqdef.body_tag:
+                    return datetime.strptime(result.get(1),
+                                             "%Y-%m-%d %H:%M:%S")
+
         log.debug("no start time identified for svc %s", self.name)
 
     @cached_property
     def start_time_secs(self):
         """ Get most recent start time of this service unit in seconds.
 
         @returns: posix timestamp
@@ -49,33 +88,55 @@
         t = self.start_time
         if t is None:
             return 0
 
         return t.timestamp()
 
     @property
-    def memory_current(self):
-        """ Returns service current memory usage in bytes. """
-        path = os.path.join(HotSOSConfig.data_root,
-                            'sys/fs/cgroup/memory/system.slice',
-                            "{}.service".format(self.name),
-                            'memory.usage_in_bytes')
-        if not os.path.exists(path):
-            # path changed between Ubuntu Focal and Jammy releases.
-            path = os.path.join(HotSOSConfig.data_root,
-                                'sys/fs/cgroup/system.slice',
-                                "{}.service".format(self.name),
-                                'memory.current')
+    def memory_current_kb(self):
+        """ Returns service current memory usage in kbytes.
 
-        if not os.path.exists(path):
-            log.warning("service memory info not found at %s", path)
+        See https://www.kernel.org/doc/Documentation/cgroup-v1/memory.txt
+        See https://www.kernel.org/doc/Documentation/cgroup-v2.txt
+        """
+        cgroupv1 = os.path.join(HotSOSConfig.data_root, 'sys/fs/cgroup',
+                                "memory/system.slice/{}.service".
+                                format(self.name), 'memory.stat')
+        cgroupv2 = os.path.join(HotSOSConfig.data_root, 'sys/fs/cgroup',
+                                'system.slice', "{}.service".
+                                format(self.name), 'memory.current')
+        if os.path.exists(cgroupv1):
+            total_usage = {}
+            fs = FileSearcher()
+            fs.add(SearchDef(r'(cache|rss|swap) (\d+)'), path=cgroupv1)
+            for result in fs.run().get(cgroupv1, {}):
+                total_usage[result.get(1)] = int(result.get(2))
+
+            if len(total_usage) == 0:
+                log.warning("failed to identify mem usage info for %s in %s",
+                            "{}.service".format(self.name), cgroupv1)
+
+            total = sum(total_usage.values())
+            if total == 0:
+                return total
+
+            return int(total / 1024)
+
+        # NOTE: memory.current (v2) is assumed not to be an approximation like
+        #       memory.usage_in_bytes in v1
+        if not os.path.exists(cgroupv2):
+            log.warning("service memory info not found at %s", cgroupv2)
             return 0
 
-        with open(path) as fd:
-            return int(fd.read())
+        with open(cgroupv2) as fd:
+            total = int(fd.read())
+            if total == 0:
+                return total
+
+            return int(total / 1024)
 
     def __repr__(self):
         return ("name={}, state={}, start_time={}, has_instances={}".
                 format(self.name, self.state, self.start_time,
                        self.has_instances))
```

### Comparing `hotsos-1.15.post9/hotsos/core/host_helpers/uptime.py` & `hotsos-1.16.0.post1/hotsos/core/host_helpers/uptime.py`

 * *Files 4% similar despite different names*

```diff
@@ -1,12 +1,12 @@
 import re
+from functools import cached_property
 
 from hotsos.core.host_helpers import CLIHelper
 from hotsos.core.log import log
-from hotsos.core.utils import cached_property
 
 
 class UptimeHelper(object):
     def __init__(self):
         # unfortunately sosreports dont have proc/uptime otherwise we would use
         # that.
         self.uptime = CLIHelper().uptime() or ""
```

### Comparing `hotsos-1.15.post9/hotsos/core/issues/issue_types.py` & `hotsos-1.16.0.post1/hotsos/core/issues/issue_types.py`

 * *Files identical despite different names*

### Comparing `hotsos-1.15.post9/hotsos/core/issues/utils.py` & `hotsos-1.16.0.post1/hotsos/core/issues/utils.py`

 * *Files identical despite different names*

### Comparing `hotsos-1.15.post9/hotsos/core/log.py` & `hotsos-1.16.0.post1/hotsos/core/log.py`

 * *Files identical despite different names*

### Comparing `hotsos-1.15.post9/hotsos/core/plugins/juju/common.py` & `hotsos-1.16.0.post1/hotsos/core/plugins/juju/common.py`

 * *Files identical despite different names*

### Comparing `hotsos-1.15.post9/hotsos/core/plugins/juju/resources.py` & `hotsos-1.16.0.post1/hotsos/core/plugins/juju/resources.py`

 * *Files 8% similar despite different names*

```diff
@@ -1,10 +1,11 @@
 import glob
 import os
 import re
+from functools import cached_property
 
 import yaml
 from hotsos.core.config import HotSOSConfig
 from hotsos.core.log import log
 from hotsos.core import utils
 
 
@@ -16,15 +17,15 @@
 
     @property
     def id(self):
         name = self.agent_service_name
         if name:
             return name.partition("jujud-machine-")[2]
 
-    @utils.cached_property
+    @cached_property
     def config(self):
         if not self.cfg:
             path = glob.glob(os.path.join(self.juju_lib_path,
                                           "agents/machine-*/agent.conf"))
             if not path:
                 return self.cfg
 
@@ -41,23 +42,23 @@
                                 fdtmp.write(line)
 
                 self.cfg = yaml.safe_load(open(ftmp))
                 os.remove(ftmp)
 
         return self.cfg
 
-    @utils.cached_property
+    @cached_property
     def agent_service_name(self):
         return self.config.get("values", {}).get("AGENT_SERVICE_NAME")
 
-    @utils.cached_property
+    @cached_property
     def version(self):
         return self.config.get("upgradedToVersion", "unknown")
 
-    @utils.cached_property
+    @cached_property
     def deployed_units(self):
         units = []
         # requires >= 2.9.x
         _units = self.config.get("values", {}).get("deployed-units", "")
         if not _units:
             return units
 
@@ -76,15 +77,15 @@
     def __init__(self, unit_id, application, juju_lib_path, path=None):
         self.id = unit_id
         self.application = application
         self.name = '{}-{}'.format(application, unit_id)
         self.juju_lib_path = juju_lib_path
         self.path = path
 
-    @utils.cached_property
+    @cached_property
     def charm_name(self):
         """
         The deployer manifest file will give us the name of the charm used to
         deploy the unit whose name may not match the charm. It also tells us
         where the charm was deployed from i.e. cs:, ch: etc
         """
         manifest_path = ("agents/unit-{}/state/deployer/manifests/*".
@@ -92,15 +93,15 @@
         for entry in glob.glob(os.path.join(self.juju_lib_path,
                                             manifest_path)):
             # we expect only one
             manifest_file = os.path.basename(entry)
             # e.g. ch_3a_amd64_2f_focal_2f_mysql-innodb-cluster-30
             return manifest_file.split('_')[-1].rpartition('-')[0]
 
-    @utils.cached_property
+    @cached_property
     def repo_info(self):
         """
         Some charms, e.g. the Openstack charms, provide a repo-info file that
         contains information from the charm's repository e.g. commit id.
         """
         info = {}
         path = os.path.join(self.path, 'charm/repo-info')
@@ -127,24 +128,24 @@
 class JujuBase(object):
     CHARM_MANIFEST_GLOB = "agents/unit-*/state/deployer/manifests"
 
     @property
     def juju_lib_path(self):
         return os.path.join(HotSOSConfig.data_root, "var/lib/juju")
 
-    @utils.cached_property
+    @cached_property
     def machine(self):
         machine = JujuMachine(self.juju_lib_path)
         if not machine.config:
             log.debug("no juju machine identified")
             return
 
         return machine
 
-    @utils.cached_property
+    @cached_property
     def units(self):
         """
         Returns units running on this host.
 
         @return: dict of JujuUnit objects keyed by unit name.
         """
         _units = {}
@@ -163,15 +164,15 @@
                     app = ret.group(1)
                     unit_id = ret.group(2)
                     u = JujuUnit(unit_id, app, self.juju_lib_path, path=unit)
                     _units[u.name] = u
 
         return _units
 
-    @utils.cached_property
+    @cached_property
     def charms(self):
         """
         Returns charms used by units on this host.
 
         @return: dict of JujuCharm objects keyed by charm name.
         """
         _charms = {}
@@ -190,13 +191,13 @@
                     versions.append(int(ret.group(2)))
 
             if name and versions:
                 _charms[name] = JujuCharm(name, max(versions))
 
         return _charms
 
-    @utils.cached_property
+    @cached_property
     def charm_names(self):
         if not self.charms:
             return []
 
         return list(self.charms.keys())
```

### Comparing `hotsos-1.15.post9/hotsos/core/plugins/kernel/common.py` & `hotsos-1.16.0.post1/hotsos/core/plugins/kernel/common.py`

 * *Files 6% similar despite different names*

```diff
@@ -1,11 +1,11 @@
 import os
 import re
+from functools import cached_property
 
-from hotsos.core.utils import cached_property
 from hotsos.core import host_helpers, plugintools
 from hotsos.core.config import HotSOSConfig
 from hotsos.core.plugins.kernel.config import KernelConfig
 
 
 class KernelBase(object):
```

### Comparing `hotsos-1.15.post9/hotsos/core/plugins/kernel/config.py` & `hotsos-1.16.0.post1/hotsos/core/plugins/kernel/config.py`

 * *Files identical despite different names*

### Comparing `hotsos-1.15.post9/hotsos/core/plugins/kernel/kernlog/calltrace.py` & `hotsos-1.16.0.post1/hotsos/core/plugins/kernel/kernlog/calltrace.py`

 * *Files identical despite different names*

### Comparing `hotsos-1.15.post9/hotsos/core/plugins/kernel/kernlog/common.py` & `hotsos-1.16.0.post1/hotsos/core/plugins/kernel/kernlog/common.py`

 * *Files identical despite different names*

### Comparing `hotsos-1.15.post9/hotsos/core/plugins/kernel/kernlog/events.py` & `hotsos-1.16.0.post1/hotsos/core/plugins/kernel/kernlog/events.py`

 * *Files identical despite different names*

### Comparing `hotsos-1.15.post9/hotsos/core/plugins/kernel/memory.py` & `hotsos-1.16.0.post1/hotsos/core/plugins/kernel/memory.py`

 * *Files identical despite different names*

### Comparing `hotsos-1.15.post9/hotsos/core/plugins/kernel/net.py` & `hotsos-1.16.0.post1/hotsos/core/plugins/kernel/net.py`

 * *Files 2% similar despite different names*

```diff
@@ -1,16 +1,15 @@
 import abc
 import os
 from collections import OrderedDict, UserList
 
 from hotsos.core.config import HotSOSConfig
-from hotsos.core.host_helpers import SYSCtlFactory, CLIHelper
+from hotsos.core.host_helpers import SYSCtlFactory, CLIHelperFile
 from hotsos.core.log import log
 from hotsos.core.search import FileSearcher, SearchDef, ResultFieldInfo
-from hotsos.core.utils import mktemp_dump
 
 
 class ProcNetBase(abc.ABC):
     """
     Provides a common way to extract fields from /proc/net/snmp and netstat.
 
     Expected file format is:
@@ -464,21 +463,22 @@
     systemd   1 0 txt  REG    9,1  1589552 54275 /lib/
     systemd   1 0 mem  REG    9,1    18976 51133 /lib/
     /*...*/
     """
 
     def _load(self):
         search = FileSearcher()
-        ftmp = mktemp_dump(''.join(CLIHelper().lsof_Mnlc()))
-        search.add(SearchDef(self._header_matcher, tag='header'), ftmp)
-        search.add(SearchDef(self._field_matcher, tag='content',
-                             field_info=self._search_field_info), ftmp)
-        results = search.run()
-        for r in results.find_by_tag('content'):
-            self.data.append(r)
+        with CLIHelperFile() as cli:
+            fout = cli.lsof_Mnlc()
+            search.add(SearchDef(self._header_matcher, tag='header'), fout)
+            search.add(SearchDef(self._field_matcher, tag='content',
+                                 field_info=self._search_field_info), fout)
+            results = search.run()
+            for r in results.find_by_tag('content'):
+                self.data.append(r)
 
     def _int_if_numeric(self, value):
         if value.isnumeric():
             return int(value)
 
         return value
```

### Comparing `hotsos-1.15.post9/hotsos/core/plugins/kernel/sysfs.py` & `hotsos-1.16.0.post1/hotsos/core/plugins/kernel/sysfs.py`

 * *Files identical despite different names*

### Comparing `hotsos-1.15.post9/hotsos/core/plugins/kubernetes.py` & `hotsos-1.16.0.post1/hotsos/core/plugins/kubernetes.py`

 * *Files 4% similar despite different names*

```diff
@@ -1,19 +1,19 @@
 import os
+from functools import cached_property
 
 from hotsos.core.config import HotSOSConfig
 from hotsos.core.host_helpers import (
     APTPackageHelper,
     HostNetworkingHelper,
     PebbleHelper,
     SnapPackageHelper,
     SystemdHelper,
 )
 from hotsos.core import plugintools
-from hotsos.core.utils import cached_property
 
 SERVICES = [r"etcd\S*",
             r"calico\S*",
             r"flannel\S*",
             r"containerd\S*",
             r"dockerd\S*",
             r"kubelet\S*",
```

### Comparing `hotsos-1.15.post9/hotsos/core/plugins/lxd/common.py` & `hotsos-1.16.0.post1/hotsos/core/plugins/lxd/common.py`

 * *Files 6% similar despite different names*

```diff
@@ -1,49 +1,46 @@
+from functools import cached_property
+
 from hotsos.core.host_helpers import (
     APTPackageHelper,
-    CLIHelper,
+    CLIHelperFile,
     SnapPackageHelper,
     SystemdHelper,
 )
 from hotsos.core.plugintools import PluginPartBase
-from hotsos.core.utils import cached_property, mktemp_dump
 from hotsos.core.search import (
     FileSearcher, SearchDef,
     SequenceSearchDef
 )
 
 
 CORE_APT = ['lxd', 'lxc']
 CORE_SNAPS = [r"(?:snap\.)?{}".format(p) for p in CORE_APT]
 SERVICE_EXPRS = [r"{}\S*".format(s) for s in CORE_SNAPS]
 
 
 class LXD(object):
 
     @cached_property
-    def buginfo_tmpfile(self):
-        out = CLIHelper().lxd_buginfo()
-        return mktemp_dump(''.join(out))
-
-    @cached_property
     def instances(self):
         """ Return a list of instance names. """
         _instances = []
         s = FileSearcher()
         seq = SequenceSearchDef(start=SearchDef(r'^## Instances$'),
                                 body=SearchDef(r'^\|\s+(\S+)\s+\|'),
                                 end=SearchDef(r'##.*'),
                                 tag='instances')
-        s.add(seq, path=self.buginfo_tmpfile)
-        results = s.run()
-        for section in results.find_sequence_sections(seq).values():
-            for r in section:
-                if 'body' in r.tag:
-                    if r.get(1) != 'NAME' and r.get(1) != '|':
-                        _instances.append(r.get(1))
+        with CLIHelperFile() as cli:
+            s.add(seq, path=cli.lxd_buginfo())
+            results = s.run()
+            for section in results.find_sequence_sections(seq).values():
+                for r in section:
+                    if 'body' in r.tag:
+                        if r.get(1) != 'NAME' and r.get(1) != '|':
+                            _instances.append(r.get(1))
 
         return _instances
 
 
 class LXDChecksBase(PluginPartBase):
 
     def __init__(self, *args, **kwargs):
```

### Comparing `hotsos-1.15.post9/hotsos/core/plugins/maas.py` & `hotsos-1.16.0.post1/hotsos/core/plugins/maas.py`

 * *Files 4% similar despite different names*

```diff
@@ -1,14 +1,15 @@
+from functools import cached_property
+
 from hotsos.core.host_helpers import (
     APTPackageHelper,
     SnapPackageHelper,
     SystemdHelper,
 )
 from hotsos.core.plugintools import PluginPartBase
-from hotsos.core.utils import cached_property
 
 CORE_APT = ['maas', 'postgres']
 APT_DEPS = ['isc-dhcp', 'bind9']
 CORE_SNAPS = CORE_APT
 
 SERVICE_EXPRS = [s + '[A-Za-z0-9-]*' for s in CORE_APT + APT_DEPS]
```

### Comparing `hotsos-1.15.post9/hotsos/core/plugins/mysql.py` & `hotsos-1.16.0.post1/hotsos/core/plugins/mysql.py`

 * *Files identical despite different names*

### Comparing `hotsos-1.15.post9/hotsos/core/plugins/openstack/common.py` & `hotsos-1.16.0.post1/hotsos/core/plugins/openstack/common.py`

 * *Files 1% similar despite different names*

```diff
@@ -1,10 +1,11 @@
 from datetime import datetime
 import os
 import re
+from functools import cached_property
 
 from hotsos.core.config import HotSOSConfig
 from hotsos.core.host_helpers.cli import CLIHelper, CmdBase
 from hotsos.core.host_helpers import (
     APTPackageHelper,
     DockerImageHelper,
     DPKGVersionCompare,
@@ -19,15 +20,14 @@
     OST_EOL_INFO,
     OST_REL_INFO,
 )
 from hotsos.core.plugins.openstack.neutron import NeutronBase
 from hotsos.core.plugins.openstack.nova import NovaBase
 from hotsos.core.plugins.openstack.octavia import OctaviaBase
 from hotsos.core import plugintools
-from hotsos.core.utils import cached_property
 from hotsos.core.ycheck.events import YEventCheckerBase
 
 
 class OpenstackBase(object):
 
     def __init__(self, *args, **kwargs):
         super().__init__(*args, **kwargs)
```

### Comparing `hotsos-1.15.post9/hotsos/core/plugins/openstack/exceptions.py` & `hotsos-1.16.0.post1/hotsos/core/plugins/openstack/exceptions.py`

 * *Files identical despite different names*

### Comparing `hotsos-1.15.post9/hotsos/core/plugins/openstack/neutron.py` & `hotsos-1.16.0.post1/hotsos/core/plugins/openstack/neutron.py`

 * *Files 1% similar despite different names*

```diff
@@ -1,18 +1,18 @@
 import os
 import re
+from functools import cached_property
 
 from hotsos.core.config import HotSOSConfig
 from hotsos.core.factory import FactoryBase
 from hotsos.core.host_helpers import CLIHelper
 from hotsos.core.plugins.openstack.openstack import (
     OpenstackConfig,
     OSTServiceBase,
 )
-from hotsos.core.utils import cached_property
 
 
 class NeutronBase(OSTServiceBase):
 
     def __init__(self, *args, **kwargs):
         super().__init__('neutron', *args, **kwargs)
         self.neutron_ovs_config = self.project.config['openvswitch-agent']
```

### Comparing `hotsos-1.15.post9/hotsos/core/plugins/openstack/nova.py` & `hotsos-1.16.0.post1/hotsos/core/plugins/openstack/nova.py`

 * *Files 1% similar despite different names*

```diff
@@ -1,9 +1,10 @@
 import os
 import re
+from functools import cached_property
 
 from hotsos.core.plugins.kernel.sysfs import CPU
 from hotsos.core.config import HotSOSConfig
 from hotsos.core.plugins.openstack.openstack import (
     OSTServiceBase,
     OpenstackConfig,
 )
@@ -17,15 +18,14 @@
     SearchDef,
     SequenceSearchDef,
 )
 from hotsos.core.plugins.system.system import (
     NUMAInfo,
     SystemBase,
 )
-from hotsos.core.utils import cached_property
 
 
 class NovaBase(OSTServiceBase):
 
     def __init__(self, *args, **kwargs):
         super().__init__('nova', *args, **kwargs)
         self.nova_config = self.project.config['main']
```

### Comparing `hotsos-1.15.post9/hotsos/core/plugins/openstack/octavia.py` & `hotsos-1.16.0.post1/hotsos/core/plugins/openstack/octavia.py`

 * *Files 2% similar despite different names*

```diff
@@ -1,9 +1,10 @@
+from functools import cached_property
+
 from hotsos.core.plugins.openstack.openstack import OSTServiceBase
-from hotsos.core.utils import cached_property
 
 OCTAVIA_HM_PORT_NAME = 'o-hm0'
 
 
 class OctaviaBase(OSTServiceBase):
 
     def __init__(self, *args, **kwargs):
```

### Comparing `hotsos-1.15.post9/hotsos/core/plugins/openstack/openstack.py` & `hotsos-1.16.0.post1/hotsos/core/plugins/openstack/openstack.py`

 * *Files 0% similar despite different names*

```diff
@@ -1,9 +1,10 @@
 import os
 from datetime import datetime
+from functools import cached_property
 
 from searchkit.constraints import TimestampMatcherBase
 from hotsos.core.config import HotSOSConfig
 from hotsos.core import host_helpers
 from hotsos.core.log import log
 from hotsos.core.plugins.openstack.exceptions import (
     EXCEPTIONS_COMMON,
@@ -22,15 +23,14 @@
     NEUTRON_EXCEPTIONS,
     NEUTRONCLIENT_EXCEPTIONS,
     OCTAVIA_EXCEPTIONS,
     OS_VIF_EXCEPTIONS,
     OVSDBAPP_EXCEPTIONS,
     MASAKARI_EXCEPTIONS,
 )
-from hotsos.core.utils import cached_property
 
 
 # NOTE(tpsilva): when updating this, refer to the Charmed Openstack supported
 # versions page: https://ubuntu.com/openstack/docs/supported-versions
 OST_EOL_INFO = {
     'antelope': datetime(2026, 4, 30),
     'zed': datetime(2024, 4, 30),
```

### Comparing `hotsos-1.15.post9/hotsos/core/plugins/openvswitch/common.py` & `hotsos-1.16.0.post1/hotsos/core/plugins/openvswitch/common.py`

 * *Files 8% similar despite different names*

```diff
@@ -1,17 +1,18 @@
+from functools import cached_property
 
 from searchkit.constraints import TimestampMatcherBase
 from hotsos.core import plugintools
 from hotsos.core.host_helpers import (
     APTPackageHelper,
     PebbleHelper,
     SystemdHelper,
 )
 from hotsos.core.ycheck.events import YEventCheckerBase
-from hotsos.core.utils import cached_property, sorted_dict
+from hotsos.core.utils import sorted_dict
 
 OVS_SERVICES_EXPRS = [r'ovsdb[a-zA-Z-]*',
                       r'ovs-vswitch[a-zA-Z-]*',
                       r'ovn[a-zA-Z-]*',
                       'openvswitch-switch',
                       ]
 OVS_PKGS_CORE = ['openvswitch-switch',
```

### Comparing `hotsos-1.15.post9/hotsos/core/plugins/openvswitch/ovn.py` & `hotsos-1.16.0.post1/hotsos/core/plugins/openvswitch/ovn.py`

 * *Files 1% similar despite different names*

```diff
@@ -1,18 +1,19 @@
 import abc
+from functools import cached_property
 
 from hotsos.core.log import log
 from hotsos.core.search import (
     SearchDef,
     SequenceSearchDef,
     FileSearcher,
 )
 from hotsos.core.config import HotSOSConfig
 from hotsos.core.host_helpers import CLIHelper
-from hotsos.core.utils import cached_property, mktemp_dump
+from hotsos.core.utils import mktemp_dump
 from hotsos.core.host_helpers import SystemdHelper
 from hotsos.core.plugins.openvswitch.common import OVS_SERVICES_EXPRS
 
 
 class OVNSBDBPort(object):
 
     def __init__(self, name, port_type):
```

### Comparing `hotsos-1.15.post9/hotsos/core/plugins/openvswitch/ovs.py` & `hotsos-1.16.0.post1/hotsos/core/plugins/openvswitch/ovs.py`

 * *Files 15% similar despite different names*

```diff
@@ -1,14 +1,17 @@
 import re
+from functools import cached_property
 
 from hotsos.core.log import log
-from hotsos.core.host_helpers import CLIHelper, HostNetworkingHelper
-from hotsos.core.utils import cached_property
+from hotsos.core.host_helpers import (
+    CLIHelper,
+    CLIHelperFile,
+    HostNetworkingHelper
+)
 from hotsos.core.search import FileSearcher, SearchDef
-from hotsos.core.utils import mktemp_dump
 
 
 class OVSDB(object):
 
     def __init__(self):
         self.cli = CLIHelper()
 
@@ -101,32 +104,32 @@
             # there.
             proto = ovn_external_ids.get('ovn-encap-type')
             if proto:
                 local_addr = ovn_external_ids['ovn-encap-ip']
                 tunnel_info[proto] = {'local': local_addr}
 
         nethelp = HostNetworkingHelper()
-        out = CLIHelper().ovs_appctl_ofproto_list_tunnels()
-        path = mktemp_dump(''.join(out))
-        s = FileSearcher()
-        expr = r'.+ \(([a-z]+): ([a-f\d\.:]+)->([a-f\d\.:]+), .+'
-        s.add(SearchDef(expr, tag='all'), path)
-        results = s.run()
-        for r in results.find_by_tag('all'):
-            proto = r.get(1)
-            if proto not in tunnel_info:
-                tunnel_info[proto] = {}
+        with CLIHelperFile() as cli:
+            s = FileSearcher()
+            expr = r'.+ \(([a-z]+): ([a-f\d\.:]+)->([a-f\d\.:]+), .+'
+            s.add(SearchDef(expr, tag='all'),
+                  cli.ovs_appctl_ofproto_list_tunnels())
+            results = s.run()
+            for r in results.find_by_tag('all'):
+                proto = r.get(1)
+                if proto not in tunnel_info:
+                    tunnel_info[proto] = {}
 
-            if 'remotes' not in tunnel_info[proto]:
-                tunnel_info[proto]['remotes'] = []
+                if 'remotes' not in tunnel_info[proto]:
+                    tunnel_info[proto]['remotes'] = []
 
-            if 'local' not in tunnel_info[proto]:
-                tunnel_info[proto]['local'] = r.get(2)
+                if 'local' not in tunnel_info[proto]:
+                    tunnel_info[proto]['local'] = r.get(2)
 
-            tunnel_info[proto]['remotes'].append(r.get(3))
+                tunnel_info[proto]['remotes'].append(r.get(3))
 
         for proto in tunnel_info:
             tunnel_info[proto]['remotes'] = len(tunnel_info[proto]['remotes'])
             local_addr = tunnel_info[proto]['local']
             if local_addr:
                 iface = nethelp.get_interface_with_addr(local_addr)
                 if iface:
```

### Comparing `hotsos-1.15.post9/hotsos/core/plugins/pacemaker.py` & `hotsos-1.16.0.post1/hotsos/core/plugins/pacemaker.py`

 * *Files 5% similar despite different names*

```diff
@@ -1,16 +1,16 @@
 import re
+from functools import cached_property
 
 from hotsos.core.host_helpers import (
     APTPackageHelper,
     CLIHelper,
     SystemdHelper,
 )
 from hotsos.core.plugintools import PluginPartBase
-from hotsos.core.utils import cached_property
 
 PACEMAKER_PKGS_CORE = ['pacemaker', r'pacemaker-\S+', 'crmsh', 'corosync']
 PACEMAKER_SVC_EXPR = ['pacemaker[a-zA-Z-]*',
                       'corosync']
 
 
 class PacemakerBase(object):
```

### Comparing `hotsos-1.15.post9/hotsos/core/plugins/rabbitmq/common.py` & `hotsos-1.16.0.post1/hotsos/core/plugins/rabbitmq/common.py`

 * *Files identical despite different names*

### Comparing `hotsos-1.15.post9/hotsos/core/plugins/rabbitmq/report.py` & `hotsos-1.16.0.post1/hotsos/core/plugins/rabbitmq/report.py`

 * *Files 6% similar despite different names*

```diff
@@ -1,17 +1,17 @@
-import os
+from functools import cached_property
 
 from hotsos.core.log import log
-from hotsos.core.utils import mktemp_dump, sorted_dict, cached_property
+from hotsos.core.utils import sorted_dict
 from hotsos.core.search import (
     SearchDef,
     SequenceSearchDef,
     FileSearcher,
 )
-from hotsos.core.host_helpers import CLIHelper
+from hotsos.core.host_helpers import CLIHelperFile
 
 
 class RabbitMQReport(object):
     """
     Class providing easy access to the contents of a rabbitmqctl report.
 
     First registers search definitions to execute against rabbitmqctl report
@@ -21,26 +21,22 @@
     NOTE: the rabbitmqctl report output differs between versions 3.6.x and
           3.8.x and we try to account for either by providing optional
           regex expressions to match either.
     """
 
     def __init__(self):
         # save to file so we can search it later
-        cli = CLIHelper()
-        self._f_report = mktemp_dump(''.join(cli.rabbitmqctl_report()))
-        searcher = FileSearcher()
-        searcher.add(self.connections_searchdef, self._f_report)
-        searcher.add(self.memory_searchdef, self._f_report)
-        searcher.add(self.cluster_partition_handling_searchdef, self._f_report)
-        searcher.add(self.queues_searchdef, self._f_report)
-        self.results = searcher.run()
-
-    def __del__(self):
-        if os.path.exists(self._f_report):
-            os.unlink(self._f_report)
+        with CLIHelperFile() as cli:
+            searcher = FileSearcher()
+            fout = cli.rabbitmqctl_report()
+            searcher.add(self.connections_searchdef, fout)
+            searcher.add(self.memory_searchdef, fout)
+            searcher.add(self.cluster_partition_handling_searchdef, fout)
+            searcher.add(self.queues_searchdef, fout)
+            self.results = searcher.run()
 
     @cached_property
     def queues_searchdef(self):
         start = SearchDef([r"^Queues on ([^:]+):",
                            (r"^Listing queues for vhost ([^:]+) "
                             r"...")])
         # NOTE: we don't use a list for the body here because
```

### Comparing `hotsos-1.15.post9/hotsos/core/plugins/sosreport.py` & `hotsos-1.16.0.post1/hotsos/core/plugins/sosreport.py`

 * *Files 9% similar despite different names*

```diff
@@ -1,17 +1,17 @@
 import os
+from functools import cached_property
 
 from hotsos.core.config import HotSOSConfig
 from hotsos.core.host_helpers import APTPackageHelper
 from hotsos.core.plugintools import PluginPartBase
 from hotsos.core.search import (
     SearchDef,
     FileSearcher,
 )
-from hotsos.core.utils import cached_property
 
 CORE_APT = ['sosreport']
 
 
 class SOSReportChecksBase(PluginPartBase):
 
     def __init__(self, *args, **kwargs):
```

### Comparing `hotsos-1.15.post9/hotsos/core/plugins/storage/bcache.py` & `hotsos-1.16.0.post1/hotsos/core/plugins/storage/bcache.py`

 * *Files 3% similar despite different names*

```diff
@@ -1,21 +1,21 @@
 import glob
 import os
 import re
+from functools import cached_property
 
 from hotsos.core.config import HotSOSConfig
-from hotsos.core.host_helpers import CLIHelper
+from hotsos.core.host_helpers import CLIHelper, CLIHelperFile
 from hotsos.core.host_helpers.config import ConfigBase
 from hotsos.core.plugins.storage import StorageBase
 from hotsos.core.search import (
     FileSearcher,
     SequenceSearchDef,
     SearchDef
 )
-from hotsos.core.utils import cached_property, mktemp_dump
 
 
 class BcacheConfig(ConfigBase):
 
     def get(self, key):
         cfg = os.path.join(self.path, key)
         if os.path.exists(cfg):
@@ -84,15 +84,14 @@
 
 class BcacheBase(StorageBase):
 
     def __init__(self, *args, **kwargs):
         super().__init__(*args, **kwargs)
         self.cachesets = []
         self._bcache_devs = []
-        self.cli = CLIHelper()
 
         for entry in glob.glob(os.path.join(HotSOSConfig.data_root,
                                'sys/fs/bcache/*')):
             if not os.path.isdir(entry):
                 continue
 
             if not os.path.exists(os.path.join(entry,
@@ -113,34 +112,31 @@
 
     @cached_property
     def udev_bcache_devs(self):
         """ If bcache devices exist fetch information and return as a list. """
         if self._bcache_devs:
             return self._bcache_devs
 
-        udevadm_info = self.cli.udevadm_info_exportdb()
-        if not udevadm_info:
-            return self._bcache_devs
-
-        s = FileSearcher()
-        sdef = SequenceSearchDef(start=SearchDef(r"^P: .+/(bcache\S+)"),
-                                 body=SearchDef(r"^S: disk/by-uuid/(\S+)"),
-                                 tag="bcacheinfo")
-        s.add(sdef, mktemp_dump('\n'.join(udevadm_info)))
-        results = s.run()
-        devs = []
-        for section in results.find_sequence_sections(sdef).values():
-            dev = {}
-            for r in section:
-                if r.tag == sdef.start_tag:
-                    dev["name"] = r.get(1)
-                else:
-                    dev["by-uuid"] = r.get(1)
+        with CLIHelperFile() as cli:
+            s = FileSearcher()
+            sdef = SequenceSearchDef(start=SearchDef(r"^P: .+/(bcache\S+)"),
+                                     body=SearchDef(r"^S: disk/by-uuid/(\S+)"),
+                                     tag="bcacheinfo")
+            s.add(sdef, cli.udevadm_info_exportdb())
+            results = s.run()
+            devs = []
+            for section in results.find_sequence_sections(sdef).values():
+                dev = {}
+                for r in section:
+                    if r.tag == sdef.start_tag:
+                        dev["name"] = r.get(1)
+                    else:
+                        dev["by-uuid"] = r.get(1)
 
-            devs.append(dev)
+                devs.append(dev)
 
         self._bcache_devs = devs
         return self._bcache_devs
 
     def resolve_bdev_from_dev(self, devpath):
         """
         Given a device path, resolve it to a corresponding bcache BDev object.
```

### Comparing `hotsos-1.15.post9/hotsos/core/plugins/storage/ceph.py` & `hotsos-1.16.0.post1/hotsos/core/plugins/storage/ceph.py`

 * *Files 1% similar despite different names*

```diff
@@ -1,20 +1,22 @@
 import os
 import re
 import subprocess
 import sys
 from datetime import datetime
+from functools import cached_property
 
 from searchkit.constraints import TimestampMatcherBase
 from hotsos.core.config import HotSOSConfig
 from hotsos.core.factory import FactoryBase
 from hotsos.core.host_helpers.cli import get_ps_axo_flags_available
 from hotsos.core.host_helpers import (
     APTPackageHelper,
     CLIHelper,
+    CLIHelperFile,
     DPKGVersionCompare,
     HostNetworkingHelper,
     PebbleHelper,
     SystemdHelper,
     SectionalConfigBase,
 )
 from hotsos.core.log import log
@@ -23,16 +25,14 @@
 from hotsos.core.plugins.storage.bcache import BcacheBase
 from hotsos.core.search import (
     FileSearcher,
     SequenceSearchDef,
     SearchDef
 )
 from hotsos.core.utils import (
-    cached_property,
-    mktemp_dump,
     sorted_dict,
     seconds_to_date,
 )
 from hotsos.core.ycheck.events import YEventCheckerBase
 
 CEPH_SERVICES_EXPRS = [r"ceph-[a-z0-9-]+",
                        r"rados[a-z0-9-:]+"]
@@ -141,33 +141,30 @@
     @csv_to_set
     def public_network_set(self):
         return self.get('public network')
 
 
 class CephCrushMap(object):
 
-    def __init__(self):
-        self.cli = CLIHelper()
-
     def _filter_pools_by_rule(self, pools, crush_rule):
         res_pool = []
         for pool in pools:
             if pool['crush_rule'] == crush_rule:
                 pool_str = pool['pool_name'] + ' (' + str(pool['pool']) + ')'
                 res_pool.append(pool_str)
 
         return res_pool
 
     @cached_property
     def osd_crush_dump(self):
-        return self.cli.ceph_osd_crush_dump_json_decoded() or {}
+        return CLIHelper().ceph_osd_crush_dump_json_decoded() or {}
 
     @cached_property
     def ceph_report(self):
-        return self.cli.ceph_report_json_decoded() or {}
+        return CLIHelper().ceph_report_json_decoded() or {}
 
     @cached_property
     def rules(self):
         """
         Returns a list of crush rules, mapped to the respective pools.
         """
         if not self.ceph_report:
@@ -351,37 +348,36 @@
     OSD_PG_OPTIMAL_NUM_MAX = 200
     OSD_PG_OPTIMAL_NUM_MIN = 50
     # If a pool's utilisation is below this value, we consider is "empty"
     POOL_EMPTY_THRESHOLD = 2
 
     def __init__(self):
         self.crush_map = CephCrushMap()
-        self.cli = CLIHelper()
 
     @cached_property
     def health_status(self):
-        status = self.cli.ceph_status_json_decoded()
+        status = CLIHelper().ceph_status_json_decoded()
         if status:
             return status['health']['status']
 
     @cached_property
     def mon_dump(self):
-        return self.cli.ceph_mon_dump_json_decoded() or {}
+        return CLIHelper().ceph_mon_dump_json_decoded() or {}
 
     @cached_property
     def osd_dump(self):
-        return self.cli.ceph_osd_dump_json_decoded() or {}
+        return CLIHelper().ceph_osd_dump_json_decoded() or {}
 
     @cached_property
     def pg_dump(self):
-        return self.cli.ceph_pg_dump_json_decoded() or {}
+        return CLIHelper().ceph_pg_dump_json_decoded() or {}
 
     @cached_property
     def ceph_mgr_module_ls(self):
-        return self.cli.ceph_mgr_module_ls() or {}
+        return CLIHelper().ceph_mgr_module_ls() or {}
 
     @cached_property
     def mons(self):
         _mons = []
         for mon in self.mon_dump.get('mons', {}):
             _mons.append(CephMon(mon['name']))
 
@@ -401,19 +397,19 @@
             if self.ceph_mgr_module_ls[category]:
                 _modules += self.ceph_mgr_module_ls[category]
 
         return _modules
 
     @cached_property
     def osd_df_tree(self):
-        return self.cli.ceph_osd_df_tree_json_decoded() or {}
+        return CLIHelper().ceph_osd_df_tree_json_decoded() or {}
 
     @cached_property
     def ceph_df(self):
-        return self.cli.ceph_df_json_decoded() or {}
+        return CLIHelper().ceph_df_json_decoded() or {}
 
     @cached_property
     def osds(self):
         """ Returns a list of CephOSD objects for all osds in the cluster. """
         _osds = []
         for osd in self.osd_dump.get('osds', {}):
             _osds.append(CephOSD(osd['osd'], osd['uuid'], dump=osd))
@@ -435,46 +431,42 @@
     def _get_version_info(self, daemon_type=None):
         """
         Returns a dict of ceph versions info for the provided daemon type. If
         no daemon type provided, version info is collected for all types and
         the resulting dict is keyed by daemon type otherwise it is keyed by
         version (and only versions for that daemon type.)
         """
-        out = CLIHelper().ceph_versions()
-        if not out:
-            return
-
-        out_path = mktemp_dump('\n'.join(out))
         versions = {}
         s = FileSearcher()
         body = SearchDef(r"\s+\"ceph version (\S+) .+ (\S+) "
                          r"\(\S+\)\":\s+(\d)+,?$")
         if daemon_type is None:
             # all/any - start matches any so no seq ending needed
             sd = SequenceSearchDef(start=SearchDef(r"^\s+\"(\S+)\":\s+{"),
                                    body=body, tag='versions')
         else:
             start = SearchDef(r"^\s+\"({})\":\s+{{".format(daemon_type))
             sd = SequenceSearchDef(start=start, body=body,
                                    end=SearchDef(r"^\s+\"\S+\":\s+{"),
                                    tag='versions')
 
-        s.add(sd, path=out_path)
-        for section in s.run().find_sequence_sections(sd).values():
-            _versions = {}
-            for result in section:
-                if result.tag == sd.start_tag:
-                    _daemon_type = result.get(1)
-                    versions[_daemon_type] = _versions
-                elif result.tag == sd.body_tag:
-                    version = result.get(1)
-                    rname = result.get(2)
-                    amount = result.get(3)
-                    _versions[version] = {'release_name': rname,
-                                          'count': int(amount)}
+        with CLIHelperFile() as cli:
+            s.add(sd, path=cli.ceph_versions())
+            for section in s.run().find_sequence_sections(sd).values():
+                _versions = {}
+                for result in section:
+                    if result.tag == sd.start_tag:
+                        _daemon_type = result.get(1)
+                        versions[_daemon_type] = _versions
+                    elif result.tag == sd.body_tag:
+                        version = result.get(1)
+                        rname = result.get(2)
+                        amount = result.get(3)
+                        _versions[version] = {'release_name': rname,
+                                              'count': int(amount)}
 
         # If specific daemon_type provided only return version for that type
         # otherwise all.
         if daemon_type is not None:
             versions = versions.get(daemon_type)
 
         return versions
@@ -709,15 +701,15 @@
             if cl_top > mon_top:
                 return False
 
         return True
 
     @cached_property
     def osdmaps_count(self):
-        report = self.cli.ceph_report_json_decoded()
+        report = CLIHelper().ceph_report_json_decoded()
         if not report:
             return 0
 
         try:
             return len(report['osdmap_manifest']['pinned_maps'])
         except (ValueError, KeyError):
             return 0
@@ -753,15 +745,15 @@
             if margin_high < num_pgs or margin_low > num_pgs:
                 _osds_pgs[osd] = num_pgs
 
         return sorted_dict(_osds_pgs, key=lambda e: e[1], reverse=True)
 
     @cached_property
     def ssds_using_bcache(self):
-        report = self.cli.ceph_report_json_decoded()
+        report = CLIHelper().ceph_report_json_decoded()
         if not report:
             return []
 
         ssd_osds_using_bcache = []
         for osd in report['osd_metadata']:
             if osd['bluestore_bdev_type'] == 'ssd' and \
                     osd['bluestore_bdev_rotational'] == '0' and \
@@ -772,15 +764,14 @@
 
 
 class CephDaemonBase(object):
 
     def __init__(self, daemon_type):
         self.daemon_type = daemon_type
         self.id = None
-        self.cli = CLIHelper()
         self.date_in_secs = self.get_date_secs()
 
     @classmethod
     def get_date_secs(cls, datestring=None):
         if datestring:
             cmd = ["date", "--utc", "--date={}".format(datestring), "+%s"]
             date_in_secs = subprocess.check_output(cmd)
@@ -803,21 +794,22 @@
             ceph_id = r"--id\s+{}".format(self.id)
         else:
             ceph_id = ''
 
         expr = (r"\S+\s+\d+\s+\S+\s+\S+\s+\d+\s+(\d+)\s+.+/ceph-{}\s+.+{}\s+.+"
                 r".+".format(self.daemon_type, ceph_id))
         sd = SearchDef(expr)
-        ps_out = mktemp_dump('\n'.join(self.cli.ps()))
-        s.add(sd, path=ps_out)
-        rss = 0
-        # we only expect one result
-        for result in s.run().find_by_path(ps_out):
-            rss = int(int(result.get(1)) / 1024)
-            break
+        with CLIHelperFile() as cli:
+            ps_out = cli.ps()
+            s.add(sd, path=ps_out)
+            rss = 0
+            # we only expect one result
+            for result in s.run().find_by_path(ps_out):
+                rss = int(int(result.get(1)) / 1024)
+                break
 
         return "{}M".format(rss)
 
     @cached_property
     def etime(self):
         """Return process etime for a given daemon.
 
@@ -828,15 +820,15 @@
             return
 
         if self.id is None:
             return
 
         ps_info = []
         daemon = "ceph-{}".format(self.daemon_type)
-        for line in self.cli.ps_axo_flags():
+        for line in CLIHelper().ps_axo_flags():
             ret = re.compile(daemon).search(line)
             if not ret:
                 continue
 
             expt_tmplt = SystemdHelper.PS_CMD_EXPR_TEMPLATES['absolute']
             ret = re.compile(expt_tmplt.format(daemon)).search(line)
             if ret:
@@ -901,15 +893,15 @@
         if self.rss:
             d[self.id]['rss'] = self.rss
 
         return d
 
     @cached_property
     def devtype(self):
-        osd_tree = self.cli.ceph_osd_df_tree_json_decoded()
+        osd_tree = CLIHelper().ceph_osd_df_tree_json_decoded()
         if not osd_tree:
             return
 
         _devtype = None
         for node in osd_tree.get('nodes'):
             if node.get('type') == 'osd' and node['id'] == self.id:
                 _devtype = node['device_class']
@@ -924,15 +916,14 @@
         self.ceph_config = CephConfig()
         self.bcache = BcacheBase()
         self.apt = APTPackageHelper(core_pkgs=CEPH_PKGS_CORE,
                                     other_pkgs=CEPH_PKGS_OTHER)
         self.pebble = PebbleHelper(service_exprs=CEPH_SERVICES_EXPRS)
         self.systemd = SystemdHelper(service_exprs=CEPH_SERVICES_EXPRS)
         self.cluster = CephCluster()
-        self.cli = CLIHelper()
         self.lsof = Lsof()
 
     @property
     def summary_subkey(self):
         return 'ceph'
 
     @property
@@ -1016,39 +1007,37 @@
 
     @cached_property
     def local_osds(self):
         """
         Returns a list of CephOSD objects for osds found on the local host.
         """
         osds = []
-        out = self.cli.ceph_volume_lvm_list()
-        if not out:
-            return osds
 
-        out_path = mktemp_dump('\n'.join(out))
         s = FileSearcher()
         sd = SequenceSearchDef(start=SearchDef(r"^=+\s+osd\.(\d+)\s+=+.*"),
                                body=SearchDef([r"\s+osd\s+(fsid)\s+(\S+)\s*",
                                                r"\s+(devices)\s+([\S]+)\s*"]),
                                tag="ceph-lvm")
-        s.add(sd, path=out_path)
-        for results in s.run().find_sequence_sections(sd).values():
-            osdid = None
-            fsid = None
-            dev = None
-            for result in results:
-                if result.tag == sd.start_tag:
-                    osdid = int(result.get(1))
-                elif result.tag == sd.body_tag:
-                    if result.get(1) == "fsid":
-                        fsid = result.get(2)
-                    elif result.get(1) == "devices":
-                        dev = result.get(2)
+        with CLIHelperFile() as cli:
+            fout = cli.ceph_volume_lvm_list()
+            s.add(sd, path=fout)
+            for results in s.run().find_sequence_sections(sd).values():
+                osdid = None
+                fsid = None
+                dev = None
+                for result in results:
+                    if result.tag == sd.start_tag:
+                        osdid = int(result.get(1))
+                    elif result.tag == sd.body_tag:
+                        if result.get(1) == "fsid":
+                            fsid = result.get(2)
+                        elif result.get(1) == "devices":
+                            dev = result.get(2)
 
-            osds.append(CephOSD(osdid, fsid, dev))
+                osds.append(CephOSD(osdid, fsid, dev))
 
         return osds
 
     @cached_property
     def local_osds_use_bcache(self):
         """
         Returns True if any local osds are using bcache devices.
```

### Comparing `hotsos-1.15.post9/hotsos/core/plugins/system/system.py` & `hotsos-1.16.0.post1/hotsos/core/plugins/system/system.py`

 * *Files 2% similar despite different names*

```diff
@@ -1,18 +1,18 @@
 import os
 import re
+from functools import cached_property
 
 from hotsos.core.config import HotSOSConfig
-from hotsos.core.host_helpers import CLIHelper, SYSCtlFactory
+from hotsos.core.host_helpers import CLIHelper, CLIHelperFile, SYSCtlFactory
 from hotsos.core.log import log
 from hotsos.core.search import (
     FileSearcher, SearchDef,
     SequenceSearchDef
 )
-from hotsos.core.utils import cached_property, mktemp_dump
 
 
 class NUMAInfo(object):
     numactl = ""
 
     def __init__(self):
         try:
@@ -170,47 +170,49 @@
             body=SearchDef(r" *?([\S ]+): (.*)\n"),
             end=SearchDef(r" *?(Technical support level): (.*)\n"),
             tag="account-status")
         not_attached_def = SearchDef(
             r".*not attached to.*(Ubuntu (Pro|Advantage)|UA).*",
             tag="not-attached")
 
-        f = mktemp_dump("".join(CLIHelper().pro_status()))
-        s.add(not_attached_def, f)
-        s.add(service_status_seqdef, f)
-        s.add(account_status_seqdef, f)
-        results = s.run()
-
-        if results.find_by_tag("not-attached"):
-            return {"status": "not-attached"}
-
-        ssects = results.find_sequence_sections(service_status_seqdef)
-        asects = results.find_sequence_sections(account_status_seqdef)
-        if not all([ssects, asects]):
-            log.debug("badness: `pro status` does not match "
-                      "the expected format")
-            return {"status": "error"}
-
-        result = {}
-        result["status"] = "attached"
-        result["services"] = {}
-
-        for sid in ssects:
-            result["services"] = {**result["services"], **{
-                v.get(1): {
-                    "entitled": v.get(2),
-                    "status": v.get(3)
-                }
-                for v in ssects[sid] if v.tag == service_status_seqdef.body_tag
-            }}
-
-        for sid in asects:
-            result = {**result, **{
-                re.sub(r'\W+', '_', v.get(1).strip()).lower(): v.get(2).strip()
-                for v in asects[sid]
-            }}
+        with CLIHelperFile() as cli:
+            f = cli.pro_status()
+            s.add(not_attached_def, f)
+            s.add(service_status_seqdef, f)
+            s.add(account_status_seqdef, f)
+            results = s.run()
+            if results.find_by_tag("not-attached"):
+                return {"status": "not-attached"}
+
+            ssects = results.find_sequence_sections(service_status_seqdef)
+            asects = results.find_sequence_sections(account_status_seqdef)
+            if not all([ssects, asects]):
+                log.debug("badness: `pro status` does not match "
+                          "the expected format")
+                return {"status": "error"}
+
+            result = {}
+            result["status"] = "attached"
+            result["services"] = {}
+
+            for sid in ssects:
+                result["services"] = {**result["services"], **{
+                    v.get(1): {
+                        "entitled": v.get(2),
+                        "status": v.get(3)
+                    }
+                    for v in ssects[sid]
+                    if v.tag == service_status_seqdef.body_tag
+                }}
+
+            for sid in asects:
+                result = {**result, **{
+                    re.sub(r'\W+', '_',
+                           v.get(1).strip()).lower(): v.get(2).strip()
+                    for v in asects[sid]
+                }}
 
-        return result
+            return result
 
     @cached_property
     def sysctl_all(self):
         return SYSCtlFactory().sysctl_all
```

### Comparing `hotsos-1.15.post9/hotsos/core/plugins/vault.py` & `hotsos-1.16.0.post1/hotsos/core/plugins/vault.py`

 * *Files 4% similar despite different names*

```diff
@@ -1,14 +1,15 @@
+from functools import cached_property
+
 from hotsos.core.plugintools import PluginPartBase
 from hotsos.core.host_helpers import (
     PebbleHelper,
     SnapPackageHelper,
     SystemdHelper,
 )
-from hotsos.core.utils import cached_property
 
 CORE_SNAPS = ['vault']
 SERVICE_EXPRS = [s + '[A-Za-z0-9-]*' for s in CORE_SNAPS]
 
 
 class VaultChecksBase(PluginPartBase):
```

### Comparing `hotsos-1.15.post9/hotsos/core/plugintools.py` & `hotsos-1.16.0.post1/hotsos/core/plugintools.py`

 * *Files identical despite different names*

### Comparing `hotsos-1.15.post9/hotsos/core/search.py` & `hotsos-1.16.0.post1/hotsos/core/search.py`

 * *Files identical despite different names*

### Comparing `hotsos-1.15.post9/hotsos/core/utils.py` & `hotsos-1.16.0.post1/hotsos/core/utils.py`

 * *Files 10% similar despite different names*

```diff
@@ -1,35 +1,12 @@
 import tempfile
 
 from hotsos.core.config import HotSOSConfig
 
 
-def cached_property(f):
-    """
-    This is used to cache properties and can be replaced once we no longer need
-    to support versions of Python (< 3.8) that don't support
-    functools.cached_property.
-    """
-
-    @property
-    def _cached_property(self):
-        key = "__cached_property_{}".format(f.__name__)
-        try:
-            if hasattr(self, key):
-                return getattr(self, key)
-        except AttributeError:
-            pass
-
-        val = f(self)
-        setattr(self, key, val)
-        return val
-
-    return _cached_property
-
-
 def sorted_dict(d, key=None, reverse=False):
     """
     Return dictionary sorted using key. If no key provided sorted by dict keys.
     """
     if key is None:
         return dict(sorted(d.items(), key=lambda e: e[0], reverse=reverse))
```

### Comparing `hotsos-1.15.post9/hotsos/core/ycheck/engine/common.py` & `hotsos-1.16.0.post1/hotsos/core/ycheck/engine/common.py`

 * *Files identical despite different names*

### Comparing `hotsos-1.15.post9/hotsos/core/ycheck/engine/properties/checks.py` & `hotsos-1.16.0.post1/hotsos/core/ycheck/engine/properties/checks.py`

 * *Files identical despite different names*

### Comparing `hotsos-1.15.post9/hotsos/core/ycheck/engine/properties/common.py` & `hotsos-1.16.0.post1/hotsos/core/ycheck/engine/properties/common.py`

 * *Files identical despite different names*

### Comparing `hotsos-1.15.post9/hotsos/core/ycheck/engine/properties/conclusions.py` & `hotsos-1.16.0.post1/hotsos/core/ycheck/engine/properties/conclusions.py`

 * *Files identical despite different names*

### Comparing `hotsos-1.15.post9/hotsos/core/ycheck/engine/properties/inputdef.py` & `hotsos-1.16.0.post1/hotsos/core/ycheck/engine/properties/inputdef.py`

 * *Files 9% similar despite different names*

```diff
@@ -1,13 +1,12 @@
 import os
 
 from hotsos.core.config import HotSOSConfig
-from hotsos.core.host_helpers import CLIHelper
+from hotsos.core.host_helpers import CLIHelperFile
 from hotsos.core.log import log
-from hotsos.core.utils import mktemp_dump
 from hotsos.core.ycheck.engine.properties.common import (
     cached_yproperty_attr,
     YPropertyOverrideBase,
     add_to_property_catalog,
 )
 
 
@@ -75,28 +74,18 @@
             args_callback = self.options['args-callback']
             if args_callback:
                 args, kwargs = self.get_method(args_callback)  # noqa, pylint: disable=E1101
             else:
                 args = self.options['args']
                 kwargs = self.options['kwargs']
 
-            # get command output
-            out = getattr(CLIHelper(), self.command)(*args, **kwargs)
-            # store in temp file to make it searchable
-            # NOTE: we dont need to delete this at the the end since they are
-            # created in the plugin tmp dir which is wiped at the end of the
-            # plugin run.
-            if type(out) == list:
-                out = ''.join(out)
-            elif type(out) == dict:
-                out = str(out)
-
-            cmd_tmp_path = mktemp_dump(out)
-            self.cache.set('cmd_tmp_path', cmd_tmp_path)  # noqa, pylint: disable=E1101
-            return [cmd_tmp_path]
+            with CLIHelperFile(delete_temp=False) as cli:
+                outfile = getattr(cli, self.command)(*args, **kwargs)
+                self.cache.set('cmd_tmp_path', outfile)  # noqa, pylint: disable=E1101
+                return [outfile]
 
         log.debug("no input provided")
 
 
 @add_to_property_catalog
 class YPropertyInput(YPropertyOverrideBase, YPropertyInputBase):
```

### Comparing `hotsos-1.15.post9/hotsos/core/ycheck/engine/properties/requires/common.py` & `hotsos-1.16.0.post1/hotsos/core/ycheck/engine/properties/requires/common.py`

 * *Files 2% similar despite different names*

```diff
@@ -1,12 +1,12 @@
 import abc
 import operator
+from functools import cached_property
 
 from hotsos.core.log import log
-from hotsos.core.utils import cached_property
 from hotsos.core.ycheck.engine.properties.common import YPropertyOverrideBase
 
 
 def intercept_exception(f):
     """
     If a call raises an AttributeError it will first be handled by
     the propertree engine which can produce confusing/misleading logs
@@ -71,16 +71,15 @@
             if self.packaging_helper.is_installed(p):  # pylint: disable=E1101
                 _installed.append(p)
 
         return _installed
 
     @cached_property
     def not_installed(self):
-        _all = self.packages_to_check
-        return set(self.installed).symmetric_difference(_all)
+        return set(self.packages_to_check).difference(self.installed)
 
 
 class OpsUtils(object):
 
     def ops_to_str(self, ops):
         """
         Convert an ops list of tuples to a string. This is typically used when
@@ -227,16 +226,15 @@
     @property
     @abc.abstractmethod
     def _svcs_info(self):
         """ ServiceManagerBase implementation with _svcs_all as input. """
 
     @cached_property
     def not_installed(self):
-        _installed = self.installed.keys()
-        return set(_installed).symmetric_difference(self._svcs_all)
+        return set(self._svcs_all).difference(self.installed)
 
     @cached_property
     def installed(self):
         return self._svcs_info.services
 
     def processes_running(self, processes):
         """ Check any processes provided. """
```

### Comparing `hotsos-1.15.post9/hotsos/core/ycheck/engine/properties/requires/requires.py` & `hotsos-1.16.0.post1/hotsos/core/ycheck/engine/properties/requires/requires.py`

 * *Files identical despite different names*

### Comparing `hotsos-1.15.post9/hotsos/core/ycheck/engine/properties/requires/types/apt.py` & `hotsos-1.16.0.post1/hotsos/core/ycheck/engine/properties/requires/types/apt.py`

 * *Files 2% similar despite different names*

```diff
@@ -1,9 +1,10 @@
+from functools import cached_property
+
 from hotsos.core.log import log
-from hotsos.core.utils import cached_property
 from hotsos.core.host_helpers import (
     APTPackageHelper,
     DPKGVersionCompare,
 )
 from hotsos.core.ycheck.engine.properties.requires import (
     intercept_exception,
     YRequirementTypeBase,
```

### Comparing `hotsos-1.15.post9/hotsos/core/ycheck/engine/properties/requires/types/config.py` & `hotsos-1.16.0.post1/hotsos/core/ycheck/engine/properties/requires/types/config.py`

 * *Files identical despite different names*

### Comparing `hotsos-1.15.post9/hotsos/core/ycheck/engine/properties/requires/types/path.py` & `hotsos-1.16.0.post1/hotsos/core/ycheck/engine/properties/requires/types/path.py`

 * *Files identical despite different names*

### Comparing `hotsos-1.15.post9/hotsos/core/ycheck/engine/properties/requires/types/pebble.py` & `hotsos-1.16.0.post1/hotsos/core/ycheck/engine/properties/requires/types/pebble.py`

 * *Files identical despite different names*

### Comparing `hotsos-1.15.post9/hotsos/core/ycheck/engine/properties/requires/types/property.py` & `hotsos-1.16.0.post1/hotsos/core/ycheck/engine/properties/requires/types/property.py`

 * *Files identical despite different names*

### Comparing `hotsos-1.15.post9/hotsos/core/ycheck/engine/properties/requires/types/snap.py` & `hotsos-1.16.0.post1/hotsos/core/ycheck/engine/properties/requires/types/snap.py`

 * *Files 4% similar despite different names*

```diff
@@ -1,10 +1,11 @@
+from functools import cached_property
+
 from hotsos.core.host_helpers import SnapPackageHelper
 from hotsos.core.log import log
-from hotsos.core.utils import cached_property
 from hotsos.core.ycheck.engine.properties.requires import (
     intercept_exception,
     YRequirementTypeBase,
     PackageCheckItemsBase,
 )
```

### Comparing `hotsos-1.15.post9/hotsos/core/ycheck/engine/properties/requires/types/systemd.py` & `hotsos-1.16.0.post1/hotsos/core/ycheck/engine/properties/requires/types/systemd.py`

 * *Files identical despite different names*

### Comparing `hotsos-1.15.post9/hotsos/core/ycheck/engine/properties/requires/types/varops.py` & `hotsos-1.16.0.post1/hotsos/core/ycheck/engine/properties/requires/types/varops.py`

 * *Files identical despite different names*

### Comparing `hotsos-1.15.post9/hotsos/core/ycheck/engine/properties/search.py` & `hotsos-1.16.0.post1/hotsos/core/ycheck/engine/properties/search.py`

 * *Files 0% similar despite different names*

```diff
@@ -1,17 +1,17 @@
 import re
 from datetime import (
     datetime,
     timedelta,
 )
+from functools import cached_property
 
 from searchkit.constraints import TimestampMatcherBase
 from hotsos.core.host_helpers import UptimeHelper, CLIHelper
 from hotsos.core.log import log
-from hotsos.core.utils import cached_property
 from hotsos.core.search import (
     SearchDef,
     SequenceSearchDef,
     SearchConstraintSearchSince,
 )
 from hotsos.core.ycheck.engine.properties.common import (
     cached_yproperty_attr,
```

### Comparing `hotsos-1.15.post9/hotsos/core/ycheck/engine/properties/vardef.py` & `hotsos-1.16.0.post1/hotsos/core/ycheck/engine/properties/vardef.py`

 * *Files identical despite different names*

### Comparing `hotsos-1.15.post9/hotsos/core/ycheck/events.py` & `hotsos-1.16.0.post1/hotsos/core/ycheck/events.py`

 * *Files identical despite different names*

### Comparing `hotsos-1.15.post9/hotsos/core/ycheck/scenarios.py` & `hotsos-1.16.0.post1/hotsos/core/ycheck/scenarios.py`

 * *Files identical despite different names*

### Comparing `hotsos-1.15.post9/hotsos/defs/events/openstack/neutron/agents.yaml` & `hotsos-1.16.0.post1/hotsos/defs/events/openstack/neutron/agents.yaml`

 * *Files identical despite different names*

### Comparing `hotsos-1.15.post9/hotsos/defs/events/openstack/nova/external-events.yaml` & `hotsos-1.16.0.post1/hotsos/defs/events/openstack/nova/external-events.yaml`

 * *Files identical despite different names*

### Comparing `hotsos-1.15.post9/hotsos/defs/events/openstack/octavia.yaml` & `hotsos-1.16.0.post1/hotsos/defs/events/openstack/octavia.yaml`

 * *Files identical despite different names*

### Comparing `hotsos-1.15.post9/hotsos/defs/events/openvswitch/ovn/errors-and-warnings.yaml` & `hotsos-1.16.0.post1/hotsos/defs/events/openvswitch/ovn/errors-and-warnings.yaml`

 * *Files identical despite different names*

### Comparing `hotsos-1.15.post9/hotsos/defs/events/openvswitch/ovn/ovn-central.yaml` & `hotsos-1.16.0.post1/hotsos/defs/events/openvswitch/ovn/ovn-central.yaml`

 * *Files identical despite different names*

### Comparing `hotsos-1.15.post9/hotsos/defs/events/openvswitch/ovn/ovn-controller.yaml` & `hotsos-1.16.0.post1/hotsos/defs/events/openvswitch/ovn/ovn-controller.yaml`

 * *Files identical despite different names*

### Comparing `hotsos-1.15.post9/hotsos/defs/events/openvswitch/ovs/ovs-vswitchd.yaml` & `hotsos-1.16.0.post1/hotsos/defs/events/openvswitch/ovs/ovs-vswitchd.yaml`

 * *Files identical despite different names*

### Comparing `hotsos-1.15.post9/hotsos/defs/events/storage/ceph/mon/monlogs.yaml` & `hotsos-1.16.0.post1/hotsos/defs/events/storage/ceph/mon/monlogs.yaml`

 * *Files identical despite different names*

### Comparing `hotsos-1.15.post9/hotsos/defs/scenarios/juju/bugs/lp1812361.yaml` & `hotsos-1.16.0.post1/hotsos/defs/scenarios/juju/bugs/lp1812361.yaml`

 * *Files identical despite different names*

### Comparing `hotsos-1.15.post9/hotsos/defs/scenarios/juju/bugs/lp1852502.yaml` & `hotsos-1.16.0.post1/hotsos/defs/scenarios/juju/bugs/lp1852502.yaml`

 * *Files identical despite different names*

### Comparing `hotsos-1.15.post9/hotsos/defs/scenarios/juju/bugs/lp1858519.yaml` & `hotsos-1.16.0.post1/hotsos/defs/scenarios/juju/bugs/lp1858519.yaml`

 * *Files identical despite different names*

### Comparing `hotsos-1.15.post9/hotsos/defs/scenarios/juju/bugs/lp1895040.yaml` & `hotsos-1.16.0.post1/hotsos/defs/scenarios/juju/bugs/lp1895040.yaml`

 * *Files identical despite different names*

### Comparing `hotsos-1.15.post9/hotsos/defs/scenarios/juju/bugs/lp1910958.yaml` & `hotsos-1.16.0.post1/hotsos/defs/scenarios/juju/bugs/lp1910958.yaml`

 * *Files identical despite different names*

### Comparing `hotsos-1.15.post9/hotsos/defs/scenarios/juju/bugs/lp1948906.yaml` & `hotsos-1.16.0.post1/hotsos/defs/scenarios/juju/bugs/lp1948906.yaml`

 * *Files identical despite different names*

### Comparing `hotsos-1.15.post9/hotsos/defs/scenarios/juju/bugs/lp1996230.yaml` & `hotsos-1.16.0.post1/hotsos/defs/scenarios/juju/bugs/lp1996230.yaml`

 * *Files identical despite different names*

### Comparing `hotsos-1.15.post9/hotsos/defs/scenarios/juju/charm_unit_checks.yaml` & `hotsos-1.16.0.post1/hotsos/defs/scenarios/juju/charm_unit_checks.yaml`

 * *Files identical despite different names*

### Comparing `hotsos-1.15.post9/hotsos/defs/scenarios/kernel/amd_iommu_pt.yaml` & `hotsos-1.16.0.post1/hotsos/defs/scenarios/kernel/amd_iommu_pt.yaml`

 * *Files identical despite different names*

### Comparing `hotsos-1.15.post9/hotsos/defs/scenarios/kernel/kernlog_calltrace.yaml` & `hotsos-1.16.0.post1/hotsos/defs/scenarios/kernel/kernlog_calltrace.yaml`

 * *Files identical despite different names*

### Comparing `hotsos-1.15.post9/hotsos/defs/scenarios/kernel/memory.yaml` & `hotsos-1.16.0.post1/hotsos/defs/scenarios/kernel/memory.yaml`

 * *Files identical despite different names*

### Comparing `hotsos-1.15.post9/hotsos/defs/scenarios/kernel/network/misc.yaml` & `hotsos-1.16.0.post1/hotsos/defs/scenarios/kernel/network/misc.yaml`

 * *Files identical despite different names*

### Comparing `hotsos-1.15.post9/hotsos/defs/scenarios/kernel/network/tcp.yaml` & `hotsos-1.16.0.post1/hotsos/defs/scenarios/kernel/network/tcp.yaml`

 * *Files identical despite different names*

### Comparing `hotsos-1.15.post9/hotsos/defs/scenarios/kernel/network/udp.yaml` & `hotsos-1.16.0.post1/hotsos/defs/scenarios/kernel/network/udp.yaml`

 * *Files identical despite different names*

### Comparing `hotsos-1.15.post9/hotsos/defs/scenarios/kernel/qla2xxx.yaml` & `hotsos-1.16.0.post1/hotsos/defs/scenarios/kernel/qla2xxx.yaml`

 * *Files identical despite different names*

### Comparing `hotsos-1.15.post9/hotsos/defs/scenarios/kubernetes/system_cpufreq_mode.yaml` & `hotsos-1.16.0.post1/hotsos/defs/scenarios/kubernetes/system_cpufreq_mode.yaml`

 * *Files identical despite different names*

### Comparing `hotsos-1.15.post9/hotsos/defs/scenarios/lxd/bugs/lp1807628.yaml` & `hotsos-1.16.0.post1/hotsos/defs/scenarios/lxd/bugs/lp1807628.yaml`

 * *Files identical despite different names*

### Comparing `hotsos-1.15.post9/hotsos/defs/scenarios/lxd/lxcfs_deadlock.yaml` & `hotsos-1.16.0.post1/hotsos/defs/scenarios/lxd/lxcfs_deadlock.yaml`

 * *Files identical despite different names*

### Comparing `hotsos-1.15.post9/hotsos/defs/scenarios/mysql/bugs/lp1959861.yaml` & `hotsos-1.16.0.post1/hotsos/defs/scenarios/mysql/bugs/lp1959861.yaml`

 * *Files identical despite different names*

### Comparing `hotsos-1.15.post9/hotsos/defs/scenarios/mysql/bugs/lp1971565.yaml` & `hotsos-1.16.0.post1/hotsos/defs/scenarios/mysql/bugs/lp1971565.yaml`

 * *Files identical despite different names*

### Comparing `hotsos-1.15.post9/hotsos/defs/scenarios/mysql/mysql_connections.yaml` & `hotsos-1.16.0.post1/hotsos/defs/scenarios/mysql/mysql_connections.yaml`

 * *Files identical despite different names*

### Comparing `hotsos-1.15.post9/hotsos/defs/scenarios/openstack/barbican/bugs/lp1946787.yaml` & `hotsos-1.16.0.post1/hotsos/defs/scenarios/openstack/barbican/bugs/lp1946787.yaml`

 * *Files identical despite different names*

### Comparing `hotsos-1.15.post9/hotsos/defs/scenarios/openstack/eol.yaml` & `hotsos-1.16.0.post1/hotsos/defs/scenarios/openstack/eol.yaml`

 * *Files identical despite different names*

### Comparing `hotsos-1.15.post9/hotsos/defs/scenarios/openstack/keystone/bugs/lp1896125.yaml` & `hotsos-1.16.0.post1/hotsos/defs/scenarios/openstack/keystone/bugs/lp1896125.yaml`

 * *Files identical despite different names*

### Comparing `hotsos-1.15.post9/hotsos/defs/scenarios/openstack/masakari/pacemaker_remote.yaml` & `hotsos-1.16.0.post1/hotsos/defs/scenarios/openstack/masakari/pacemaker_remote.yaml`

 * *Files identical despite different names*

### Comparing `hotsos-1.15.post9/hotsos/defs/scenarios/openstack/neutron/bugs/lp1794991.yaml` & `hotsos-1.16.0.post1/hotsos/defs/scenarios/openstack/neutron/bugs/lp1794991.yaml`

 * *Files identical despite different names*

### Comparing `hotsos-1.15.post9/hotsos/defs/scenarios/openstack/neutron/bugs/lp1907686.yaml` & `hotsos-1.16.0.post1/hotsos/defs/scenarios/openstack/neutron/bugs/lp1907686.yaml`

 * *Files identical despite different names*

### Comparing `hotsos-1.15.post9/hotsos/defs/scenarios/openstack/neutron/bugs/lp1927868.yaml` & `hotsos-1.16.0.post1/hotsos/defs/scenarios/openstack/neutron/bugs/lp1927868.yaml`

 * *Files identical despite different names*

### Comparing `hotsos-1.15.post9/hotsos/defs/scenarios/openstack/neutron/bugs/lp1960319.yaml` & `hotsos-1.16.0.post1/hotsos/defs/scenarios/openstack/neutron/bugs/lp1960319.yaml`

 * *Files identical despite different names*

### Comparing `hotsos-1.15.post9/hotsos/defs/scenarios/openstack/neutron/bugs/lp1979089.yaml` & `hotsos-1.16.0.post1/hotsos/defs/scenarios/openstack/neutron/bugs/lp1979089.yaml`

 * *Files identical despite different names*

### Comparing `hotsos-1.15.post9/hotsos/defs/scenarios/openstack/neutron/bugs/lp1993628.yaml` & `hotsos-1.16.0.post1/hotsos/defs/scenarios/openstack/neutron/bugs/lp1993628.yaml`

 * *Files identical despite different names*

### Comparing `hotsos-1.15.post9/hotsos/defs/scenarios/openstack/neutron/bugs/lp1996594.yaml` & `hotsos-1.16.0.post1/hotsos/defs/scenarios/openstack/neutron/bugs/lp1996594.yaml`

 * *Files identical despite different names*

### Comparing `hotsos-1.15.post9/hotsos/defs/scenarios/openstack/neutron/neutron_ovs_cleanup.yaml` & `hotsos-1.16.0.post1/hotsos/defs/scenarios/openstack/neutron/neutron_ovs_cleanup.yaml`

 * *Files identical despite different names*

### Comparing `hotsos-1.15.post9/hotsos/defs/scenarios/openstack/neutron/ovn_stale_db.yaml` & `hotsos-1.16.0.post1/hotsos/defs/scenarios/openstack/neutron/ovn_stale_db.yaml`

 * *Files identical despite different names*

### Comparing `hotsos-1.15.post9/hotsos/defs/scenarios/openstack/nova/bugs/lp1860743.yaml` & `hotsos-1.16.0.post1/hotsos/defs/scenarios/openstack/nova/bugs/lp1860743.yaml`

 * *Files identical despite different names*

### Comparing `hotsos-1.15.post9/hotsos/defs/scenarios/openstack/nova/bugs/lp1888395.yaml` & `hotsos-1.16.0.post1/hotsos/defs/scenarios/openstack/nova/bugs/lp1888395.yaml`

 * *Files identical despite different names*

### Comparing `hotsos-1.15.post9/hotsos/defs/scenarios/openstack/nova/bugs/lp1904580.yaml` & `hotsos-1.16.0.post1/hotsos/defs/scenarios/openstack/nova/bugs/lp1904580.yaml`

 * *Files identical despite different names*

### Comparing `hotsos-1.15.post9/hotsos/defs/scenarios/openstack/nova/bugs/lp1967956.yaml` & `hotsos-1.16.0.post1/hotsos/defs/scenarios/openstack/nova/bugs/lp1967956.yaml`

 * *Files identical despite different names*

### Comparing `hotsos-1.15.post9/hotsos/defs/scenarios/openstack/nova/config_checks.yaml` & `hotsos-1.16.0.post1/hotsos/defs/scenarios/openstack/nova/config_checks.yaml`

 * *Files identical despite different names*

### Comparing `hotsos-1.15.post9/hotsos/defs/scenarios/openstack/nova/cpu_pinning.yaml` & `hotsos-1.16.0.post1/hotsos/defs/scenarios/openstack/nova/cpu_pinning.yaml`

 * *Files identical despite different names*

### Comparing `hotsos-1.15.post9/hotsos/defs/scenarios/openstack/nova/service_mem_usage.yaml` & `hotsos-1.16.0.post1/hotsos/defs/scenarios/openstack/nova/service_mem_usage.yaml`

 * *Files 4% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 vars:
-  limit: 536870912  # 5G
-  libvirtd_usage: '@hotsos.core.host_helpers.systemd.ServiceFactory.memory_current:libvirtd'
+  limit: 5242880  # 5G in kb
+  libvirtd_usage: '@hotsos.core.host_helpers.systemd.ServiceFactory.memory_current_kb:libvirtd'
 checks:
   libvirtd_mem_use_above_limit:
     systemd: libvirtd
     varops: [[$libvirtd_usage], [gt, $limit]]
   pkg_has_lp2024114:
     apt:
       libvirt-daemon:
@@ -13,26 +13,26 @@
           max: 8.0.0-1ubuntu7.5
 conclusions:
   libvirtd_overuse:
     decision: libvirtd_mem_use_above_limit
     raises:
       type: OpenstackWarning
       message: >-
-        The libvirtd service is consuming more than 5G memory (current={usage}). This is
+        The libvirtd service is consuming more than 5G memory (current_kb={usage}). This is
         not normal and could indicate a memory leak. Please check.
       format-dict:
         usage: $libvirtd_usage
   libvirtd_mem_leak_lp2024114:
     priority: 2
     decision:
       - libvirtd_mem_use_above_limit
       - pkg_has_lp2024114
     raises:
       type: LaunchpadBug
       bug-id: 2024114
       message: >-
-        The libvirtd service on this host is consuming more than 5G memory (current={usage}). This is
+        The libvirtd service on this host is consuming more than 5G memory (current_kb={usage}). This is
         not normal and could indicate a memory leak. The installed version ({installed})
         is also known to be impacted by a memory leak bug. Recommendation is to upgrade.
       format-dict:
         usage: $libvirtd_usage
         installed: '@checks.pkg_has_lp2024114.requires.version'
```

### Comparing `hotsos-1.15.post9/hotsos/defs/scenarios/openstack/octavia/bugs/sb1896125.yaml` & `hotsos-1.16.0.post1/hotsos/defs/scenarios/openstack/octavia/bugs/sb1896125.yaml`

 * *Files identical despite different names*

### Comparing `hotsos-1.15.post9/hotsos/defs/scenarios/openstack/octavia/excessive_failovers.yaml` & `hotsos-1.16.0.post1/hotsos/defs/scenarios/openstack/octavia/excessive_failovers.yaml`

 * *Files identical despite different names*

### Comparing `hotsos-1.15.post9/hotsos/defs/scenarios/openstack/octavia/hm_port_health.yaml` & `hotsos-1.16.0.post1/hotsos/defs/scenarios/openstack/octavia/hm_port_health.yaml`

 * *Files identical despite different names*

### Comparing `hotsos-1.15.post9/hotsos/defs/scenarios/openstack/openstack_apache2_certificates.yaml` & `hotsos-1.16.0.post1/hotsos/defs/scenarios/openstack/openstack_apache2_certificates.yaml`

 * *Files identical despite different names*

### Comparing `hotsos-1.15.post9/hotsos/defs/scenarios/openstack/openstack_charm_conflicts.yaml` & `hotsos-1.16.0.post1/hotsos/defs/scenarios/openstack/openstack_charm_conflicts.yaml`

 * *Files identical despite different names*

### Comparing `hotsos-1.15.post9/hotsos/defs/scenarios/openstack/system_cpufreq_mode.yaml` & `hotsos-1.16.0.post1/hotsos/defs/scenarios/openstack/system_cpufreq_mode.yaml`

 * *Files identical despite different names*

### Comparing `hotsos-1.15.post9/hotsos/defs/scenarios/openstack/systemd_masked_services.yaml` & `hotsos-1.16.0.post1/hotsos/defs/scenarios/openstack/systemd_masked_services.yaml`

 * *Files identical despite different names*

### Comparing `hotsos-1.15.post9/hotsos/defs/scenarios/openvswitch/bugs/lp1839592.yaml` & `hotsos-1.16.0.post1/hotsos/defs/scenarios/openvswitch/bugs/lp1839592.yaml`

 * *Files identical despite different names*

### Comparing `hotsos-1.15.post9/hotsos/defs/scenarios/openvswitch/bugs/lp1978806.yaml` & `hotsos-1.16.0.post1/hotsos/defs/scenarios/openvswitch/bugs/lp1978806.yaml`

 * *Files identical despite different names*

### Comparing `hotsos-1.15.post9/hotsos/defs/scenarios/openvswitch/dpif_lost_packets.yaml` & `hotsos-1.16.0.post1/hotsos/defs/scenarios/openvswitch/dpif_lost_packets.yaml`

 * *Files identical despite different names*

### Comparing `hotsos-1.15.post9/hotsos/defs/scenarios/openvswitch/dpif_resubmit_actions.yaml` & `hotsos-1.16.0.post1/hotsos/defs/scenarios/openvswitch/dpif_resubmit_actions.yaml`

 * *Files identical despite different names*

### Comparing `hotsos-1.15.post9/hotsos/defs/scenarios/openvswitch/ovn/bfd_flapping.yaml` & `hotsos-1.16.0.post1/hotsos/defs/scenarios/openvswitch/ovn/bfd_flapping.yaml`

 * *Files identical despite different names*

### Comparing `hotsos-1.15.post9/hotsos/defs/scenarios/openvswitch/ovn/bugs/lp1865127.yaml` & `hotsos-1.16.0.post1/hotsos/defs/scenarios/openvswitch/ovn/bugs/lp1865127.yaml`

 * *Files identical despite different names*

### Comparing `hotsos-1.15.post9/hotsos/defs/scenarios/openvswitch/ovn/ovn_central_certs_logs.yaml` & `hotsos-1.16.0.post1/hotsos/defs/scenarios/openvswitch/ovn/ovn_central_certs_logs.yaml`

 * *Files 8% similar despite different names*

```diff
@@ -3,23 +3,29 @@
   ovn_central_cert_mtime: '@hotsos.core.host_helpers.filestat.FileFactory.mtime:etc/ovn/ovn-central.crt'
   northd_start_time: '@hotsos.core.host_helpers.systemd.ServiceFactory.start_time_secs:ovn-northd'
   ovsdb_nb_start_time: '@hotsos.core.host_helpers.systemd.ServiceFactory.start_time_secs:ovn-ovsdb-server-nb'
   ovsdb_sb_start_time: '@hotsos.core.host_helpers.systemd.ServiceFactory.start_time_secs:ovn-ovsdb-server-sb'
   cert_expired_expr: '([\d-]+)T([\d:]+)\.\d+Z\|\S+\|stream_ssl\|WARN\|SSL_accept: error:\S+:SSL routines:ssl3_read_bytes:sslv3 alert certificate expired'
   cert_invalid_expr: '([\d-]+)T([\d:]+)\.\d+Z\|\S+\|stream_ssl\|WARN\|SSL_accept: error:\S+:SSL routines:tls_process_client_certificate:certificate verify failed'
 checks:
-  services_not_restarted_after_cert_update:
-    - systemd: [ovn-northd, ovn-ovsdb-server-nb, ovn-ovsdb-server-sb]
-    - or:
-        - varops: [[$host_cert_mtime], [gt, $northd_start_time]]
-        - varops: [[$host_cert_mtime], [gt, $ovsdb_nb_start_time]]
-        - varops: [[$host_cert_mtime], [gt, $ovsdb_sb_start_time]]
-        - varops: [[$ovn_central_cert_mtime], [gt, $northd_start_time]]
-        - varops: [[$ovn_central_cert_mtime], [gt, $ovsdb_nb_start_time]]
-        - varops: [[$ovn_central_cert_mtime], [gt, $ovsdb_sb_start_time]]
+  northd_not_restarted_after_cert_update:
+    - systemd: ovn-northd
+    - varops: [[$northd_start_time], [gt, 0]]
+    - varops: [[$host_cert_mtime], [gt, $northd_start_time]]
+    - varops: [[$ovn_central_cert_mtime], [gt, $northd_start_time]]
+  nbdb_not_restarted_after_cert_update:
+    - systemd: ovn-ovsdb-server-nb
+    - varops: [[$ovsdb_nb_start_time], [gt, 0]]
+    - varops: [[$host_cert_mtime], [gt, $ovsdb_nb_start_time]]
+    - varops: [[$ovn_central_cert_mtime], [gt, $ovsdb_nb_start_time]]
+  sbdb_not_restarted_after_cert_update:
+    - systemd: ovn-ovsdb-server-sb
+    - varops: [[$ovsdb_sb_start_time], [gt, 0]]
+    - varops: [[$host_cert_mtime], [gt, $ovsdb_sb_start_time]]
+    - varops: [[$ovn_central_cert_mtime], [gt, $ovsdb_sb_start_time]]
   northd_certs_invalid_logs:
     input: var/log/ovn/ovn-northd.log
     expr: $cert_invalid_expr
     constraints:
       search-result-age-hours: 24
   northd_certs_expired_logs:
     input: var/log/ovn/ovn-northd.log
@@ -38,15 +44,19 @@
       - var/log/ovn/ovsdb-server-nb.log
       - var/log/ovn/ovsdb-server-sb.log
     expr: $cert_expired_expr
     constraints:
       search-result-age-hours: 24
 conclusions:
   services_not_restarted_after_cert_update:
-    decision: services_not_restarted_after_cert_update
+    decision:
+      or:
+        - northd_not_restarted_after_cert_update
+        - nbdb_not_restarted_after_cert_update
+        - sbdb_not_restarted_after_cert_update
     raises:
       type: OVNWarning
       message: >-
         One or more of services ovn-northd, ovn-ovsdb-server-nb and ovn-ovsdb-server-sb has not
         been restarted since ssl certs were updated and this may breaking their ability to
         connect to other services.
   northd_certs_invalid:
```

### Comparing `hotsos-1.15.post9/hotsos/defs/scenarios/openvswitch/ovn/ovn_central_services.yaml` & `hotsos-1.16.0.post1/hotsos/defs/scenarios/openvswitch/ovn/ovn_central_services.yaml`

 * *Files identical despite different names*

### Comparing `hotsos-1.15.post9/hotsos/defs/scenarios/openvswitch/ovn/ovn_certs_valid.yaml` & `hotsos-1.16.0.post1/hotsos/defs/scenarios/openvswitch/ovn/ovn_certs_valid.yaml`

 * *Files identical despite different names*

### Comparing `hotsos-1.15.post9/hotsos/defs/scenarios/openvswitch/ovn/ovn_chassis_certs_logs.yaml` & `hotsos-1.16.0.post1/hotsos/defs/scenarios/openvswitch/ovn/ovn_chassis_certs_logs.yaml`

 * *Files 4% similar despite different names*

```diff
@@ -3,14 +3,15 @@
   ovn_chassis_cert_mtime: '@hotsos.core.host_helpers.filestat.FileFactory.mtime:etc/ovn/ovn-chassis.crt'
   ovn_controller_start_time: '@hotsos.core.host_helpers.systemd.ServiceFactory.start_time_secs:ovn-controller'
   cert_expired_expr: '([\d-]+)T([\d:]+)\.\d+Z\|\S+\|stream_ssl\|WARN\|SSL_accept: error:\S+:SSL routines:ssl3_read_bytes:sslv3 alert certificate expired'
   cert_invalid_expr: '([\d-]+)T([\d:]+)\.\d+Z\|\S+\|stream_ssl\|WARN\|SSL_accept: error:\S+:SSL routines:tls_process_client_certificate:certificate verify failed'
 checks:
   services_not_restarted_after_cert_update:
     - systemd: ovn-controller
+    - varops: [[$ovn_controller_start_time], [gt, 0]]
     - varops: [[$host_cert_mtime], [gt, $ovn_controller_start_time]]
     - varops: [[$ovn_chassis_cert_mtime], [gt, $ovn_controller_start_time]]
   certs_expired_logs:
     input: var/log/ovn/ovn-controller.log
     expr: $cert_expired_expr
     constraints:
       search-result-age-hours: 24
```

### Comparing `hotsos-1.15.post9/hotsos/defs/scenarios/openvswitch/ovn/ovn_db_upgrade.yaml` & `hotsos-1.16.0.post1/hotsos/defs/scenarios/openvswitch/ovn/ovn_db_upgrade.yaml`

 * *Files identical despite different names*

### Comparing `hotsos-1.15.post9/hotsos/defs/scenarios/openvswitch/ovn/ovn_elections.yaml` & `hotsos-1.16.0.post1/hotsos/defs/scenarios/openvswitch/ovn/ovn_elections.yaml`

 * *Files identical despite different names*

### Comparing `hotsos-1.15.post9/hotsos/defs/scenarios/openvswitch/ovn/ovsdb_reconnect_errors.yaml` & `hotsos-1.16.0.post1/hotsos/defs/scenarios/openvswitch/ovn/ovsdb_reconnect_errors.yaml`

 * *Files identical despite different names*

### Comparing `hotsos-1.15.post9/hotsos/defs/scenarios/openvswitch/service_restarts.yaml` & `hotsos-1.16.0.post1/hotsos/defs/scenarios/openvswitch/service_restarts.yaml`

 * *Files identical despite different names*

### Comparing `hotsos-1.15.post9/hotsos/defs/scenarios/pacemaker/bugs/lp1874719.yaml` & `hotsos-1.16.0.post1/hotsos/defs/scenarios/pacemaker/bugs/lp1874719.yaml`

 * *Files identical despite different names*

### Comparing `hotsos-1.15.post9/hotsos/defs/scenarios/rabbitmq/bugs/lp1943937.yaml` & `hotsos-1.16.0.post1/hotsos/defs/scenarios/rabbitmq/bugs/lp1943937.yaml`

 * *Files identical despite different names*

### Comparing `hotsos-1.15.post9/hotsos/defs/scenarios/rabbitmq/cluster_config.yaml` & `hotsos-1.16.0.post1/hotsos/defs/scenarios/rabbitmq/cluster_config.yaml`

 * *Files identical despite different names*

### Comparing `hotsos-1.15.post9/hotsos/defs/scenarios/rabbitmq/cluster_logchecks.yaml` & `hotsos-1.16.0.post1/hotsos/defs/scenarios/rabbitmq/cluster_logchecks.yaml`

 * *Files identical despite different names*

### Comparing `hotsos-1.15.post9/hotsos/defs/scenarios/rabbitmq/cluster_resources.yaml` & `hotsos-1.16.0.post1/hotsos/defs/scenarios/rabbitmq/cluster_resources.yaml`

 * *Files identical despite different names*

### Comparing `hotsos-1.15.post9/hotsos/defs/scenarios/sosreport/plugin_timeouts.yaml` & `hotsos-1.16.0.post1/hotsos/defs/scenarios/sosreport/plugin_timeouts.yaml`

 * *Files identical despite different names*

### Comparing `hotsos-1.15.post9/hotsos/defs/scenarios/storage/bcache/bdev.yaml` & `hotsos-1.16.0.post1/hotsos/defs/scenarios/storage/bcache/bdev.yaml`

 * *Files identical despite different names*

### Comparing `hotsos-1.15.post9/hotsos/defs/scenarios/storage/bcache/cacheset.yaml` & `hotsos-1.16.0.post1/hotsos/defs/scenarios/storage/bcache/cacheset.yaml`

 * *Files identical despite different names*

### Comparing `hotsos-1.15.post9/hotsos/defs/scenarios/storage/ceph/ceph-mgr/autoscaler_overlap_roots.yaml` & `hotsos-1.16.0.post1/hotsos/defs/scenarios/storage/ceph/ceph-mgr/autoscaler_overlap_roots.yaml`

 * *Files identical despite different names*

### Comparing `hotsos-1.15.post9/hotsos/defs/scenarios/storage/ceph/ceph-mon/auth_insecure_global_id_reclaim_allowed.yaml` & `hotsos-1.16.0.post1/hotsos/defs/scenarios/storage/ceph/ceph-mon/auth_insecure_global_id_reclaim_allowed.yaml`

 * *Files 13% similar despite different names*

```diff
@@ -1,12 +1,12 @@
 checks:
   insecure_auth_allowed:
     input:
       command: ceph_health_detail_json_decoded
-    expr: '.+''message'': ''mon is allowing insecure global_id reclaim'''
+    expr: '.+"message": "mon is allowing insecure global_id reclaim"'
   health_warning:
     property:
       path: hotsos.core.plugins.storage.ceph.CephCluster.health_status
       ops: [[eq, HEALTH_WARN]]
 conclusions:
   insecure-auth-allowed:
     decision:
```

### Comparing `hotsos-1.15.post9/hotsos/defs/scenarios/storage/ceph/ceph-mon/autoscaler_bug.yaml` & `hotsos-1.16.0.post1/hotsos/defs/scenarios/storage/ceph/ceph-mon/autoscaler_bug.yaml`

 * *Files identical despite different names*

### Comparing `hotsos-1.15.post9/hotsos/defs/scenarios/storage/ceph/ceph-mon/bluefs_size.yaml` & `hotsos-1.16.0.post1/hotsos/defs/scenarios/storage/ceph/ceph-mon/bluefs_size.yaml`

 * *Files identical despite different names*

### Comparing `hotsos-1.15.post9/hotsos/defs/scenarios/storage/ceph/ceph-mon/bluefs_spillover.yaml` & `hotsos-1.16.0.post1/hotsos/defs/scenarios/storage/ceph/ceph-mon/bluefs_spillover.yaml`

 * *Files identical despite different names*

### Comparing `hotsos-1.15.post9/hotsos/defs/scenarios/storage/ceph/ceph-mon/ceph-mon.yaml` & `hotsos-1.16.0.post1/hotsos/defs/scenarios/storage/ceph/ceph-mon/ceph-mon.yaml`

 * *Files identical despite different names*

### Comparing `hotsos-1.15.post9/hotsos/defs/scenarios/storage/ceph/ceph-mon/ceph_address_overlap.yaml` & `hotsos-1.16.0.post1/hotsos/defs/scenarios/storage/ceph/ceph-mon/ceph_address_overlap.yaml`

 * *Files identical despite different names*

### Comparing `hotsos-1.15.post9/hotsos/defs/scenarios/storage/ceph/ceph-mon/ceph_cluster_health.yaml` & `hotsos-1.16.0.post1/hotsos/defs/scenarios/storage/ceph/ceph-mon/ceph_cluster_health.yaml`

 * *Files identical despite different names*

### Comparing `hotsos-1.15.post9/hotsos/defs/scenarios/storage/ceph/ceph-mon/ceph_versions_mismatch.yaml` & `hotsos-1.16.0.post1/hotsos/defs/scenarios/storage/ceph/ceph-mon/ceph_versions_mismatch.yaml`

 * *Files identical despite different names*

### Comparing `hotsos-1.15.post9/hotsos/defs/scenarios/storage/ceph/ceph-mon/crushmap_bucket_checks.yaml` & `hotsos-1.16.0.post1/hotsos/defs/scenarios/storage/ceph/ceph-mon/crushmap_bucket_checks.yaml`

 * *Files identical despite different names*

### Comparing `hotsos-1.15.post9/hotsos/defs/scenarios/storage/ceph/ceph-mon/empty_clog.yaml` & `hotsos-1.16.0.post1/hotsos/defs/scenarios/storage/ceph/ceph-mon/empty_clog.yaml`

 * *Files identical despite different names*

### Comparing `hotsos-1.15.post9/hotsos/defs/scenarios/storage/ceph/ceph-mon/eol.yaml` & `hotsos-1.16.0.post1/hotsos/defs/scenarios/storage/ceph/ceph-mon/eol.yaml`

 * *Files identical despite different names*

### Comparing `hotsos-1.15.post9/hotsos/defs/scenarios/storage/ceph/ceph-mon/laggy_pgs.yaml` & `hotsos-1.16.0.post1/hotsos/defs/scenarios/storage/ceph/ceph-mon/laggy_pgs.yaml`

 * *Files identical despite different names*

### Comparing `hotsos-1.15.post9/hotsos/defs/scenarios/storage/ceph/ceph-mon/large_omap_objects.yaml` & `hotsos-1.16.0.post1/hotsos/defs/scenarios/storage/ceph/ceph-mon/large_omap_objects.yaml`

 * *Files identical despite different names*

### Comparing `hotsos-1.15.post9/hotsos/defs/scenarios/storage/ceph/ceph-mon/meta_backend_mon.yaml` & `hotsos-1.16.0.post1/hotsos/defs/scenarios/storage/ceph/ceph-mon/meta_backend_mon.yaml`

 * *Files identical despite different names*

### Comparing `hotsos-1.15.post9/hotsos/defs/scenarios/storage/ceph/ceph-mon/mon_db_too_big.yaml` & `hotsos-1.16.0.post1/hotsos/defs/scenarios/storage/ceph/ceph-mon/mon_db_too_big.yaml`

 * *Files identical despite different names*

### Comparing `hotsos-1.15.post9/hotsos/defs/scenarios/storage/ceph/ceph-mon/mon_elections_flapping.yaml` & `hotsos-1.16.0.post1/hotsos/defs/scenarios/storage/ceph/ceph-mon/mon_elections_flapping.yaml`

 * *Files identical despite different names*

### Comparing `hotsos-1.15.post9/hotsos/defs/scenarios/storage/ceph/ceph-mon/osd_flapping.yaml` & `hotsos-1.16.0.post1/hotsos/defs/scenarios/storage/ceph/ceph-mon/osd_flapping.yaml`

 * *Files identical despite different names*

### Comparing `hotsos-1.15.post9/hotsos/defs/scenarios/storage/ceph/ceph-mon/osd_maps_backlog_too_large.yaml` & `hotsos-1.16.0.post1/hotsos/defs/scenarios/storage/ceph/ceph-mon/osd_maps_backlog_too_large.yaml`

 * *Files identical despite different names*

### Comparing `hotsos-1.15.post9/hotsos/defs/scenarios/storage/ceph/ceph-mon/osd_messenger_v2_protocol.yaml` & `hotsos-1.16.0.post1/hotsos/defs/scenarios/storage/ceph/ceph-mon/osd_messenger_v2_protocol.yaml`

 * *Files identical despite different names*

### Comparing `hotsos-1.15.post9/hotsos/defs/scenarios/storage/ceph/ceph-mon/osd_slow_heartbeats.yaml` & `hotsos-1.16.0.post1/hotsos/defs/scenarios/storage/ceph/ceph-mon/osd_slow_heartbeats.yaml`

 * *Files identical despite different names*

### Comparing `hotsos-1.15.post9/hotsos/defs/scenarios/storage/ceph/ceph-mon/osd_slow_ops.yaml` & `hotsos-1.16.0.post1/hotsos/defs/scenarios/storage/ceph/ceph-mon/osd_slow_ops.yaml`

 * *Files identical despite different names*

### Comparing `hotsos-1.15.post9/hotsos/defs/scenarios/storage/ceph/ceph-mon/pg_imbalance.yaml` & `hotsos-1.16.0.post1/hotsos/defs/scenarios/storage/ceph/ceph-mon/pg_imbalance.yaml`

 * *Files identical despite different names*

### Comparing `hotsos-1.15.post9/hotsos/defs/scenarios/storage/ceph/ceph-mon/pg_overdose.yaml` & `hotsos-1.16.0.post1/hotsos/defs/scenarios/storage/ceph/ceph-mon/pg_overdose.yaml`

 * *Files identical despite different names*

### Comparing `hotsos-1.15.post9/hotsos/defs/scenarios/storage/ceph/ceph-mon/required_osd_release_mismatch.yaml` & `hotsos-1.16.0.post1/hotsos/defs/scenarios/storage/ceph/ceph-mon/required_osd_release_mismatch.yaml`

 * *Files identical despite different names*

### Comparing `hotsos-1.15.post9/hotsos/defs/scenarios/storage/ceph/ceph-mon/rgw_frontend.yaml` & `hotsos-1.16.0.post1/hotsos/defs/scenarios/storage/ceph/ceph-mon/rgw_frontend.yaml`

 * *Files identical despite different names*

### Comparing `hotsos-1.15.post9/hotsos/defs/scenarios/storage/ceph/ceph-mon/ssds_using_bcache.yaml` & `hotsos-1.16.0.post1/hotsos/defs/scenarios/storage/ceph/ceph-mon/ssds_using_bcache.yaml`

 * *Files identical despite different names*

### Comparing `hotsos-1.15.post9/hotsos/defs/scenarios/storage/ceph/ceph-mon/unresponsive_mon_mgr.yaml` & `hotsos-1.16.0.post1/hotsos/defs/scenarios/storage/ceph/ceph-mon/unresponsive_mon_mgr.yaml`

 * *Files identical despite different names*

### Comparing `hotsos-1.15.post9/hotsos/defs/scenarios/storage/ceph/ceph-osd/bugs/lp1936136.yaml` & `hotsos-1.16.0.post1/hotsos/defs/scenarios/storage/ceph/ceph-osd/bugs/lp1936136.yaml`

 * *Files identical despite different names*

### Comparing `hotsos-1.15.post9/hotsos/defs/scenarios/storage/ceph/ceph-osd/bugs/lp1959649.yaml` & `hotsos-1.16.0.post1/hotsos/defs/scenarios/storage/ceph/ceph-osd/bugs/lp1959649.yaml`

 * *Files identical despite different names*

### Comparing `hotsos-1.15.post9/hotsos/defs/scenarios/storage/ceph/ceph-osd/bugs/lp1996010.yaml` & `hotsos-1.16.0.post1/hotsos/defs/scenarios/storage/ceph/ceph-osd/bugs/lp1996010.yaml`

 * *Files identical despite different names*

### Comparing `hotsos-1.15.post9/hotsos/defs/scenarios/storage/ceph/ceph-osd/bugs/lp2013960.yaml` & `hotsos-1.16.0.post1/hotsos/defs/scenarios/storage/ceph/ceph-osd/bugs/lp2013960.yaml`

 * *Files identical despite different names*

### Comparing `hotsos-1.15.post9/hotsos/defs/scenarios/storage/ceph/ceph-osd/bugs/lp2016845.yaml` & `hotsos-1.16.0.post1/hotsos/defs/scenarios/storage/ceph/ceph-osd/bugs/lp2016845.yaml`

 * *Files identical despite different names*

### Comparing `hotsos-1.15.post9/hotsos/defs/scenarios/storage/ceph/ceph-osd/ceph_address_overlap.yaml` & `hotsos-1.16.0.post1/hotsos/defs/scenarios/storage/ceph/ceph-osd/ceph_address_overlap.yaml`

 * *Files identical despite different names*

### Comparing `hotsos-1.15.post9/hotsos/defs/scenarios/storage/ceph/ceph-osd/eol.yaml` & `hotsos-1.16.0.post1/hotsos/defs/scenarios/storage/ceph/ceph-osd/eol.yaml`

 * *Files identical despite different names*

### Comparing `hotsos-1.15.post9/hotsos/defs/scenarios/storage/ceph/ceph-osd/filestore_to_bluestore_upgrade.yaml` & `hotsos-1.16.0.post1/hotsos/defs/scenarios/storage/ceph/ceph-osd/filestore_to_bluestore_upgrade.yaml`

 * *Files identical despite different names*

### Comparing `hotsos-1.15.post9/hotsos/defs/scenarios/storage/ceph/ceph-osd/juju_ceph_no_bcache_tuning.yaml` & `hotsos-1.16.0.post1/hotsos/defs/scenarios/storage/ceph/ceph-osd/juju_ceph_no_bcache_tuning.yaml`

 * *Files identical despite different names*

### Comparing `hotsos-1.15.post9/hotsos/defs/scenarios/storage/ceph/ceph-osd/meta_backend_osd.yaml` & `hotsos-1.16.0.post1/hotsos/defs/scenarios/storage/ceph/ceph-osd/meta_backend_osd.yaml`

 * *Files identical despite different names*

### Comparing `hotsos-1.15.post9/hotsos/defs/scenarios/storage/ceph/ceph-osd/osd_flapping.yaml` & `hotsos-1.16.0.post1/hotsos/defs/scenarios/storage/ceph/ceph-osd/osd_flapping.yaml`

 * *Files identical despite different names*

### Comparing `hotsos-1.15.post9/hotsos/defs/scenarios/storage/ceph/ceph-osd/osd_latency.yaml` & `hotsos-1.16.0.post1/hotsos/defs/scenarios/storage/ceph/ceph-osd/osd_latency.yaml`

 * *Files identical despite different names*

### Comparing `hotsos-1.15.post9/hotsos/defs/scenarios/storage/ceph/ceph-osd/osd_slow_ops.yaml` & `hotsos-1.16.0.post1/hotsos/defs/scenarios/storage/ceph/ceph-osd/osd_slow_ops.yaml`

 * *Files identical despite different names*

### Comparing `hotsos-1.15.post9/hotsos/defs/scenarios/storage/ceph/ceph-osd/pg_overdose.yaml` & `hotsos-1.16.0.post1/hotsos/defs/scenarios/storage/ceph/ceph-osd/pg_overdose.yaml`

 * *Files identical despite different names*

### Comparing `hotsos-1.15.post9/hotsos/defs/scenarios/storage/ceph/ceph-osd/ssd_osds_no_discard.yaml.disabled` & `hotsos-1.16.0.post1/hotsos/defs/scenarios/storage/ceph/ceph-osd/ssd_osds_no_discard.yaml.disabled`

 * *Files identical despite different names*

### Comparing `hotsos-1.15.post9/hotsos/defs/scenarios/storage/ceph/ceph-osd/system_cpufreq_mode.yaml` & `hotsos-1.16.0.post1/hotsos/defs/scenarios/storage/ceph/ceph-osd/system_cpufreq_mode.yaml`

 * *Files identical despite different names*

### Comparing `hotsos-1.15.post9/hotsos/defs/scenarios/storage/ceph/ceph-rgw/rgw_frontend_rgw.yaml` & `hotsos-1.16.0.post1/hotsos/defs/scenarios/storage/ceph/ceph-rgw/rgw_frontend_rgw.yaml`

 * *Files identical despite different names*

### Comparing `hotsos-1.15.post9/hotsos/defs/scenarios/storage/ceph/common/ceph_charm_conflicts.yaml` & `hotsos-1.16.0.post1/hotsos/defs/scenarios/storage/ceph/common/ceph_charm_conflicts.yaml`

 * *Files identical despite different names*

### Comparing `hotsos-1.15.post9/hotsos/plugin_extensions/juju/summary.py` & `hotsos-1.16.0.post1/hotsos/plugin_extensions/juju/summary.py`

 * *Files identical despite different names*

### Comparing `hotsos-1.15.post9/hotsos/plugin_extensions/kernel/summary.py` & `hotsos-1.16.0.post1/hotsos/plugin_extensions/kernel/summary.py`

 * *Files identical despite different names*

### Comparing `hotsos-1.15.post9/hotsos/plugin_extensions/kubernetes/summary.py` & `hotsos-1.16.0.post1/hotsos/plugin_extensions/kubernetes/summary.py`

 * *Files identical despite different names*

### Comparing `hotsos-1.15.post9/hotsos/plugin_extensions/lxd/summary.py` & `hotsos-1.16.0.post1/hotsos/plugin_extensions/lxd/summary.py`

 * *Files identical despite different names*

### Comparing `hotsos-1.15.post9/hotsos/plugin_extensions/openstack/agent/events.py` & `hotsos-1.16.0.post1/hotsos/plugin_extensions/openstack/agent/events.py`

 * *Files identical despite different names*

### Comparing `hotsos-1.15.post9/hotsos/plugin_extensions/openstack/agent/exceptions.py` & `hotsos-1.16.0.post1/hotsos/plugin_extensions/openstack/agent/exceptions.py`

 * *Files identical despite different names*

### Comparing `hotsos-1.15.post9/hotsos/plugin_extensions/openstack/nova_external_events.py` & `hotsos-1.16.0.post1/hotsos/plugin_extensions/openstack/nova_external_events.py`

 * *Files identical despite different names*

### Comparing `hotsos-1.15.post9/hotsos/plugin_extensions/openstack/service_features.py` & `hotsos-1.16.0.post1/hotsos/plugin_extensions/openstack/service_features.py`

 * *Files identical despite different names*

### Comparing `hotsos-1.15.post9/hotsos/plugin_extensions/openstack/service_network_checks.py` & `hotsos-1.16.0.post1/hotsos/plugin_extensions/openstack/service_network_checks.py`

 * *Files identical despite different names*

### Comparing `hotsos-1.15.post9/hotsos/plugin_extensions/openstack/summary.py` & `hotsos-1.16.0.post1/hotsos/plugin_extensions/openstack/summary.py`

 * *Files identical despite different names*

### Comparing `hotsos-1.15.post9/hotsos/plugin_extensions/openstack/vm_info.py` & `hotsos-1.16.0.post1/hotsos/plugin_extensions/openstack/vm_info.py`

 * *Files identical despite different names*

### Comparing `hotsos-1.15.post9/hotsos/plugin_extensions/openvswitch/event_checks.py` & `hotsos-1.16.0.post1/hotsos/plugin_extensions/openvswitch/event_checks.py`

 * *Files identical despite different names*

### Comparing `hotsos-1.15.post9/hotsos/plugin_extensions/openvswitch/summary.py` & `hotsos-1.16.0.post1/hotsos/plugin_extensions/openvswitch/summary.py`

 * *Files identical despite different names*

### Comparing `hotsos-1.15.post9/hotsos/plugin_extensions/pacemaker/summary.py` & `hotsos-1.16.0.post1/hotsos/plugin_extensions/pacemaker/summary.py`

 * *Files identical despite different names*

### Comparing `hotsos-1.15.post9/hotsos/plugin_extensions/rabbitmq/summary.py` & `hotsos-1.16.0.post1/hotsos/plugin_extensions/rabbitmq/summary.py`

 * *Files identical despite different names*

### Comparing `hotsos-1.15.post9/hotsos/plugin_extensions/sosreport/summary.py` & `hotsos-1.16.0.post1/hotsos/plugin_extensions/sosreport/summary.py`

 * *Files identical despite different names*

### Comparing `hotsos-1.15.post9/hotsos/plugin_extensions/storage/bcache_summary.py` & `hotsos-1.16.0.post1/hotsos/plugin_extensions/storage/bcache_summary.py`

 * *Files identical despite different names*

### Comparing `hotsos-1.15.post9/hotsos/plugin_extensions/storage/ceph_event_checks.py` & `hotsos-1.16.0.post1/hotsos/plugin_extensions/storage/ceph_event_checks.py`

 * *Files identical despite different names*

### Comparing `hotsos-1.15.post9/hotsos/plugin_extensions/storage/ceph_summary.py` & `hotsos-1.16.0.post1/hotsos/plugin_extensions/storage/ceph_summary.py`

 * *Files identical despite different names*

### Comparing `hotsos-1.15.post9/hotsos/plugin_extensions/system/checks.py` & `hotsos-1.16.0.post1/hotsos/plugin_extensions/system/checks.py`

 * *Files identical despite different names*

### Comparing `hotsos-1.15.post9/hotsos/plugin_extensions/system/summary.py` & `hotsos-1.16.0.post1/hotsos/plugin_extensions/system/summary.py`

 * *Files identical despite different names*

### Comparing `hotsos-1.15.post9/hotsos/templates/header.html` & `hotsos-1.16.0.post1/hotsos/templates/header.html`

 * *Files identical despite different names*

### Comparing `hotsos-1.15.post9/hotsos.egg-info/PKG-INFO` & `hotsos-1.16.0.post1/hotsos.egg-info/PKG-INFO`

 * *Files 2% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: hotsos
-Version: 1.15.post9
+Version: 1.16.0.post1
 Summary: Software analysis toolkit. Define checks in high-level language and leverage library to perform analysis of common Cloud applications.
 Requires-Python: >=3.8
 Description-Content-Type: text/markdown
 License-File: LICENSE
 
 # Hotsos
```

### Comparing `hotsos-1.15.post9/hotsos.egg-info/SOURCES.txt` & `hotsos-1.16.0.post1/hotsos.egg-info/SOURCES.txt`

 * *Files 0% similar despite different names*

```diff
@@ -16,14 +16,15 @@
 hotsos/core/__init__.py
 hotsos/core/analytics.py
 hotsos/core/config.py
 hotsos/core/exceptions.py
 hotsos/core/factory.py
 hotsos/core/log.py
 hotsos/core/plugintools.py
+hotsos/core/root_manager.py
 hotsos/core/search.py
 hotsos/core/utils.py
 hotsos/core/host_helpers/__init__.py
 hotsos/core/host_helpers/cli.py
 hotsos/core/host_helpers/common.py
 hotsos/core/host_helpers/config.py
 hotsos/core/host_helpers/filestat.py
```

### Comparing `hotsos-1.15.post9/pyproject.toml` & `hotsos-1.16.0.post1/pyproject.toml`

 * *Files identical despite different names*

