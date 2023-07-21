# Comparing `tmp/chaosgarden-0.2.3.tar.gz` & `tmp/chaosgarden-0.2.4.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "chaosgarden-0.2.3.tar", last modified: Tue May 23 05:28:29 2023, max compression
+gzip compressed data, was "chaosgarden-0.2.4.tar", last modified: Fri Jul 21 12:36:01 2023, max compression
```

## Comparing `chaosgarden-0.2.3.tar` & `chaosgarden-0.2.4.tar`

### file list

```diff
@@ -1,63 +1,64 @@
-drwxr-xr-x   0 root         (0) root         (0)        0 2023-05-23 05:28:28.999263 chaosgarden-0.2.3/
--rw-r--r--   0 root         (0) root         (0)    10255 2023-05-23 05:27:38.000000 chaosgarden-0.2.3/LICENSE
--rw-r--r--   0 root         (0) root         (0)     1694 2023-05-23 05:28:28.999263 chaosgarden-0.2.3/PKG-INFO
-drwxr-xr-x   0 root         (0) root         (0)        0 2023-05-23 05:28:28.991263 chaosgarden-0.2.3/chaosgarden/
--rw-r--r--   0 root         (0) root         (0)        0 2023-05-23 05:27:38.000000 chaosgarden-0.2.3/chaosgarden/__init__.py
-drwxr-xr-x   0 root         (0) root         (0)        0 2023-05-23 05:28:28.995263 chaosgarden-0.2.3/chaosgarden/alicloud/
--rw-r--r--   0 root         (0) root         (0)        0 2023-05-23 05:27:38.000000 chaosgarden-0.2.3/chaosgarden/alicloud/__init__.py
-drwxr-xr-x   0 root         (0) root         (0)        0 2023-05-23 05:28:28.995263 chaosgarden-0.2.3/chaosgarden/aws/
--rw-r--r--   0 root         (0) root         (0)        0 2023-05-23 05:27:38.000000 chaosgarden-0.2.3/chaosgarden/aws/__init__.py
--rw-r--r--   0 root         (0) root         (0)    12486 2023-05-23 05:27:38.000000 chaosgarden-0.2.3/chaosgarden/aws/actions.py
-drwxr-xr-x   0 root         (0) root         (0)        0 2023-05-23 05:28:28.995263 chaosgarden-0.2.3/chaosgarden/azure/
--rw-r--r--   0 root         (0) root         (0)     7694 2023-05-23 05:27:38.000000 chaosgarden-0.2.3/chaosgarden/azure/__init__.py
--rw-r--r--   0 root         (0) root         (0)    14897 2023-05-23 05:27:38.000000 chaosgarden-0.2.3/chaosgarden/azure/actions.py
-drwxr-xr-x   0 root         (0) root         (0)        0 2023-05-23 05:28:28.995263 chaosgarden-0.2.3/chaosgarden/garden/
--rw-r--r--   0 root         (0) root         (0)      621 2023-05-23 05:27:38.000000 chaosgarden-0.2.3/chaosgarden/garden/__init__.py
--rw-r--r--   0 root         (0) root         (0)    21666 2023-05-23 05:27:38.000000 chaosgarden-0.2.3/chaosgarden/garden/actions.py
--rw-r--r--   0 root         (0) root         (0)     4235 2023-05-23 05:27:38.000000 chaosgarden-0.2.3/chaosgarden/garden/probes.py
-drwxr-xr-x   0 root         (0) root         (0)        0 2023-05-23 05:28:28.995263 chaosgarden-0.2.3/chaosgarden/gcp/
--rw-r--r--   0 root         (0) root         (0)     6984 2023-05-23 05:27:38.000000 chaosgarden-0.2.3/chaosgarden/gcp/__init__.py
--rw-r--r--   0 root         (0) root         (0)    15392 2023-05-23 05:27:38.000000 chaosgarden-0.2.3/chaosgarden/gcp/actions.py
-drwxr-xr-x   0 root         (0) root         (0)        0 2023-05-23 05:28:28.995263 chaosgarden-0.2.3/chaosgarden/human/
--rw-r--r--   0 root         (0) root         (0)        0 2023-05-23 05:27:38.000000 chaosgarden-0.2.3/chaosgarden/human/__init__.py
--rw-r--r--   0 root         (0) root         (0)      198 2023-05-23 05:27:38.000000 chaosgarden-0.2.3/chaosgarden/human/actions.py
-drwxr-xr-x   0 root         (0) root         (0)        0 2023-05-23 05:28:28.995263 chaosgarden-0.2.3/chaosgarden/k8s/
--rw-r--r--   0 root         (0) root         (0)     6886 2023-05-23 05:27:38.000000 chaosgarden-0.2.3/chaosgarden/k8s/__init__.py
--rw-r--r--   0 root         (0) root         (0)     4714 2023-05-23 05:27:38.000000 chaosgarden-0.2.3/chaosgarden/k8s/actions.py
-drwxr-xr-x   0 root         (0) root         (0)        0 2023-05-23 05:28:28.995263 chaosgarden-0.2.3/chaosgarden/k8s/api/
--rw-r--r--   0 root         (0) root         (0)        0 2023-05-23 05:27:38.000000 chaosgarden-0.2.3/chaosgarden/k8s/api/__init__.py
--rw-r--r--   0 root         (0) root         (0)     3425 2023-05-23 05:27:38.000000 chaosgarden-0.2.3/chaosgarden/k8s/api/authenticators.py
--rw-r--r--   0 root         (0) root         (0)     7365 2023-05-23 05:27:38.000000 chaosgarden-0.2.3/chaosgarden/k8s/api/clients.py
--rw-r--r--   0 root         (0) root         (0)     2143 2023-05-23 05:27:38.000000 chaosgarden-0.2.3/chaosgarden/k8s/api/cluster.py
-drwxr-xr-x   0 root         (0) root         (0)        0 2023-05-23 05:28:28.995263 chaosgarden-0.2.3/chaosgarden/k8s/probe/
--rw-r--r--   0 root         (0) root         (0)        0 2023-05-23 05:27:38.000000 chaosgarden-0.2.3/chaosgarden/k8s/probe/__init__.py
--rw-r--r--   0 root         (0) root         (0)    11170 2023-05-23 05:27:38.000000 chaosgarden-0.2.3/chaosgarden/k8s/probe/metrics.py
-drwxr-xr-x   0 root         (0) root         (0)        0 2023-05-23 05:28:28.999263 chaosgarden-0.2.3/chaosgarden/k8s/probe/resources/
--rw-r--r--   0 root         (0) root         (0)        0 2023-05-23 05:27:38.000000 chaosgarden-0.2.3/chaosgarden/k8s/probe/resources/__init__.py
--rw-r--r--   0 root         (0) root         (0)     2416 2023-05-23 05:27:38.000000 chaosgarden-0.2.3/chaosgarden/k8s/probe/resources/generate_resources.py
--rw-r--r--   0 root         (0) root         (0)    14856 2023-05-23 05:27:38.000000 chaosgarden-0.2.3/chaosgarden/k8s/probe/resources/probe_pod.py
--rw-r--r--   0 root         (0) root         (0)     2012 2023-05-23 05:27:38.000000 chaosgarden-0.2.3/chaosgarden/k8s/probe/resources/suicidal_pod.py
--rw-r--r--   0 root         (0) root         (0)     8099 2023-05-23 05:27:38.000000 chaosgarden-0.2.3/chaosgarden/k8s/probe/resources/templated_resources.yaml
--rw-r--r--   0 root         (0) root         (0)     1943 2023-05-23 05:27:38.000000 chaosgarden-0.2.3/chaosgarden/k8s/probe/thresholds.py
--rw-r--r--   0 root         (0) root         (0)    20971 2023-05-23 05:27:38.000000 chaosgarden-0.2.3/chaosgarden/k8s/probes.py
-drwxr-xr-x   0 root         (0) root         (0)        0 2023-05-23 05:28:28.999263 chaosgarden-0.2.3/chaosgarden/metal/
--rw-r--r--   0 root         (0) root         (0)        0 2023-05-23 05:27:38.000000 chaosgarden-0.2.3/chaosgarden/metal/__init__.py
-drwxr-xr-x   0 root         (0) root         (0)        0 2023-05-23 05:28:28.999263 chaosgarden-0.2.3/chaosgarden/openstack/
--rw-r--r--   0 root         (0) root         (0)     4446 2023-05-23 05:27:38.000000 chaosgarden-0.2.3/chaosgarden/openstack/__init__.py
--rw-r--r--   0 root         (0) root         (0)    13046 2023-05-23 05:27:38.000000 chaosgarden-0.2.3/chaosgarden/openstack/actions.py
-drwxr-xr-x   0 root         (0) root         (0)        0 2023-05-23 05:28:28.999263 chaosgarden-0.2.3/chaosgarden/util/
--rw-r--r--   0 root         (0) root         (0)      916 2023-05-23 05:27:38.000000 chaosgarden-0.2.3/chaosgarden/util/__init__.py
--rw-r--r--   0 root         (0) root         (0)     1875 2023-05-23 05:27:38.000000 chaosgarden-0.2.3/chaosgarden/util/terminator.py
--rw-r--r--   0 root         (0) root         (0)     3712 2023-05-23 05:27:38.000000 chaosgarden-0.2.3/chaosgarden/util/threading.py
-drwxr-xr-x   0 root         (0) root         (0)        0 2023-05-23 05:28:28.999263 chaosgarden-0.2.3/chaosgarden/vsphere/
--rw-r--r--   0 root         (0) root         (0)    11990 2023-05-23 05:27:38.000000 chaosgarden-0.2.3/chaosgarden/vsphere/__init__.py
--rw-r--r--   0 root         (0) root         (0)    10486 2023-05-23 05:27:38.000000 chaosgarden-0.2.3/chaosgarden/vsphere/actions.py
--rw-r--r--   0 root         (0) root         (0)     4821 2023-05-23 05:27:38.000000 chaosgarden-0.2.3/chaosgarden/vsphere/pchelper.py
-drwxr-xr-x   0 root         (0) root         (0)        0 2023-05-23 05:28:28.995263 chaosgarden-0.2.3/chaosgarden.egg-info/
--rw-r--r--   0 root         (0) root         (0)     1694 2023-05-23 05:28:28.000000 chaosgarden-0.2.3/chaosgarden.egg-info/PKG-INFO
--rw-r--r--   0 root         (0) root         (0)     1411 2023-05-23 05:28:28.000000 chaosgarden-0.2.3/chaosgarden.egg-info/SOURCES.txt
--rw-r--r--   0 root         (0) root         (0)        1 2023-05-23 05:28:28.000000 chaosgarden-0.2.3/chaosgarden.egg-info/dependency_links.txt
--rw-r--r--   0 root         (0) root         (0)      334 2023-05-23 05:28:28.000000 chaosgarden-0.2.3/chaosgarden.egg-info/requires.txt
--rw-r--r--   0 root         (0) root         (0)       18 2023-05-23 05:28:28.000000 chaosgarden-0.2.3/chaosgarden.egg-info/top_level.txt
--rw-r--r--   0 root         (0) root         (0)       38 2023-05-23 05:28:28.999263 chaosgarden-0.2.3/setup.cfg
--rw-r--r--   0 root         (0) root         (0)     3331 2023-05-23 05:27:38.000000 chaosgarden-0.2.3/setup.py
+drwxr-xr-x   0 root         (0) root         (0)        0 2023-07-21 12:36:01.855718 chaosgarden-0.2.4/
+-rw-r--r--   0 root         (0) root         (0)    10255 2023-07-21 12:35:06.000000 chaosgarden-0.2.4/LICENSE
+-rw-r--r--   0 root         (0) root         (0)     1694 2023-07-21 12:36:01.855718 chaosgarden-0.2.4/PKG-INFO
+drwxr-xr-x   0 root         (0) root         (0)        0 2023-07-21 12:36:01.847718 chaosgarden-0.2.4/chaosgarden/
+-rw-r--r--   0 root         (0) root         (0)        0 2023-07-21 12:35:06.000000 chaosgarden-0.2.4/chaosgarden/__init__.py
+drwxr-xr-x   0 root         (0) root         (0)        0 2023-07-21 12:36:01.847718 chaosgarden-0.2.4/chaosgarden/alicloud/
+-rw-r--r--   0 root         (0) root         (0)    27059 2023-07-21 12:35:06.000000 chaosgarden-0.2.4/chaosgarden/alicloud/__init__.py
+-rw-r--r--   0 root         (0) root         (0)    16698 2023-07-21 12:35:06.000000 chaosgarden-0.2.4/chaosgarden/alicloud/actions.py
+drwxr-xr-x   0 root         (0) root         (0)        0 2023-07-21 12:36:01.847718 chaosgarden-0.2.4/chaosgarden/aws/
+-rw-r--r--   0 root         (0) root         (0)        0 2023-07-21 12:35:06.000000 chaosgarden-0.2.4/chaosgarden/aws/__init__.py
+-rw-r--r--   0 root         (0) root         (0)    12486 2023-07-21 12:35:06.000000 chaosgarden-0.2.4/chaosgarden/aws/actions.py
+drwxr-xr-x   0 root         (0) root         (0)        0 2023-07-21 12:36:01.847718 chaosgarden-0.2.4/chaosgarden/azure/
+-rw-r--r--   0 root         (0) root         (0)     7694 2023-07-21 12:35:06.000000 chaosgarden-0.2.4/chaosgarden/azure/__init__.py
+-rw-r--r--   0 root         (0) root         (0)    14897 2023-07-21 12:35:06.000000 chaosgarden-0.2.4/chaosgarden/azure/actions.py
+drwxr-xr-x   0 root         (0) root         (0)        0 2023-07-21 12:36:01.851718 chaosgarden-0.2.4/chaosgarden/garden/
+-rw-r--r--   0 root         (0) root         (0)      621 2023-07-21 12:35:06.000000 chaosgarden-0.2.4/chaosgarden/garden/__init__.py
+-rw-r--r--   0 root         (0) root         (0)    22179 2023-07-21 12:35:06.000000 chaosgarden-0.2.4/chaosgarden/garden/actions.py
+-rw-r--r--   0 root         (0) root         (0)     4235 2023-07-21 12:35:06.000000 chaosgarden-0.2.4/chaosgarden/garden/probes.py
+drwxr-xr-x   0 root         (0) root         (0)        0 2023-07-21 12:36:01.851718 chaosgarden-0.2.4/chaosgarden/gcp/
+-rw-r--r--   0 root         (0) root         (0)     6984 2023-07-21 12:35:06.000000 chaosgarden-0.2.4/chaosgarden/gcp/__init__.py
+-rw-r--r--   0 root         (0) root         (0)    15392 2023-07-21 12:35:06.000000 chaosgarden-0.2.4/chaosgarden/gcp/actions.py
+drwxr-xr-x   0 root         (0) root         (0)        0 2023-07-21 12:36:01.851718 chaosgarden-0.2.4/chaosgarden/human/
+-rw-r--r--   0 root         (0) root         (0)        0 2023-07-21 12:35:06.000000 chaosgarden-0.2.4/chaosgarden/human/__init__.py
+-rw-r--r--   0 root         (0) root         (0)      198 2023-07-21 12:35:06.000000 chaosgarden-0.2.4/chaosgarden/human/actions.py
+drwxr-xr-x   0 root         (0) root         (0)        0 2023-07-21 12:36:01.851718 chaosgarden-0.2.4/chaosgarden/k8s/
+-rw-r--r--   0 root         (0) root         (0)     6886 2023-07-21 12:35:06.000000 chaosgarden-0.2.4/chaosgarden/k8s/__init__.py
+-rw-r--r--   0 root         (0) root         (0)     4714 2023-07-21 12:35:06.000000 chaosgarden-0.2.4/chaosgarden/k8s/actions.py
+drwxr-xr-x   0 root         (0) root         (0)        0 2023-07-21 12:36:01.851718 chaosgarden-0.2.4/chaosgarden/k8s/api/
+-rw-r--r--   0 root         (0) root         (0)        0 2023-07-21 12:35:06.000000 chaosgarden-0.2.4/chaosgarden/k8s/api/__init__.py
+-rw-r--r--   0 root         (0) root         (0)     3425 2023-07-21 12:35:06.000000 chaosgarden-0.2.4/chaosgarden/k8s/api/authenticators.py
+-rw-r--r--   0 root         (0) root         (0)     7365 2023-07-21 12:35:06.000000 chaosgarden-0.2.4/chaosgarden/k8s/api/clients.py
+-rw-r--r--   0 root         (0) root         (0)     2143 2023-07-21 12:35:06.000000 chaosgarden-0.2.4/chaosgarden/k8s/api/cluster.py
+drwxr-xr-x   0 root         (0) root         (0)        0 2023-07-21 12:36:01.851718 chaosgarden-0.2.4/chaosgarden/k8s/probe/
+-rw-r--r--   0 root         (0) root         (0)        0 2023-07-21 12:35:06.000000 chaosgarden-0.2.4/chaosgarden/k8s/probe/__init__.py
+-rw-r--r--   0 root         (0) root         (0)    11170 2023-07-21 12:35:06.000000 chaosgarden-0.2.4/chaosgarden/k8s/probe/metrics.py
+drwxr-xr-x   0 root         (0) root         (0)        0 2023-07-21 12:36:01.851718 chaosgarden-0.2.4/chaosgarden/k8s/probe/resources/
+-rw-r--r--   0 root         (0) root         (0)        0 2023-07-21 12:35:06.000000 chaosgarden-0.2.4/chaosgarden/k8s/probe/resources/__init__.py
+-rw-r--r--   0 root         (0) root         (0)     2416 2023-07-21 12:35:06.000000 chaosgarden-0.2.4/chaosgarden/k8s/probe/resources/generate_resources.py
+-rw-r--r--   0 root         (0) root         (0)    14856 2023-07-21 12:35:06.000000 chaosgarden-0.2.4/chaosgarden/k8s/probe/resources/probe_pod.py
+-rw-r--r--   0 root         (0) root         (0)     2012 2023-07-21 12:35:06.000000 chaosgarden-0.2.4/chaosgarden/k8s/probe/resources/suicidal_pod.py
+-rw-r--r--   0 root         (0) root         (0)     8099 2023-07-21 12:35:06.000000 chaosgarden-0.2.4/chaosgarden/k8s/probe/resources/templated_resources.yaml
+-rw-r--r--   0 root         (0) root         (0)     1943 2023-07-21 12:35:06.000000 chaosgarden-0.2.4/chaosgarden/k8s/probe/thresholds.py
+-rw-r--r--   0 root         (0) root         (0)    20971 2023-07-21 12:35:06.000000 chaosgarden-0.2.4/chaosgarden/k8s/probes.py
+drwxr-xr-x   0 root         (0) root         (0)        0 2023-07-21 12:36:01.851718 chaosgarden-0.2.4/chaosgarden/metal/
+-rw-r--r--   0 root         (0) root         (0)        0 2023-07-21 12:35:06.000000 chaosgarden-0.2.4/chaosgarden/metal/__init__.py
+drwxr-xr-x   0 root         (0) root         (0)        0 2023-07-21 12:36:01.851718 chaosgarden-0.2.4/chaosgarden/openstack/
+-rw-r--r--   0 root         (0) root         (0)     4446 2023-07-21 12:35:06.000000 chaosgarden-0.2.4/chaosgarden/openstack/__init__.py
+-rw-r--r--   0 root         (0) root         (0)    13046 2023-07-21 12:35:06.000000 chaosgarden-0.2.4/chaosgarden/openstack/actions.py
+drwxr-xr-x   0 root         (0) root         (0)        0 2023-07-21 12:36:01.855718 chaosgarden-0.2.4/chaosgarden/util/
+-rw-r--r--   0 root         (0) root         (0)      916 2023-07-21 12:35:06.000000 chaosgarden-0.2.4/chaosgarden/util/__init__.py
+-rw-r--r--   0 root         (0) root         (0)     1875 2023-07-21 12:35:06.000000 chaosgarden-0.2.4/chaosgarden/util/terminator.py
+-rw-r--r--   0 root         (0) root         (0)     3712 2023-07-21 12:35:06.000000 chaosgarden-0.2.4/chaosgarden/util/threading.py
+drwxr-xr-x   0 root         (0) root         (0)        0 2023-07-21 12:36:01.855718 chaosgarden-0.2.4/chaosgarden/vsphere/
+-rw-r--r--   0 root         (0) root         (0)    11990 2023-07-21 12:35:06.000000 chaosgarden-0.2.4/chaosgarden/vsphere/__init__.py
+-rw-r--r--   0 root         (0) root         (0)    10486 2023-07-21 12:35:06.000000 chaosgarden-0.2.4/chaosgarden/vsphere/actions.py
+-rw-r--r--   0 root         (0) root         (0)     4821 2023-07-21 12:35:06.000000 chaosgarden-0.2.4/chaosgarden/vsphere/pchelper.py
+drwxr-xr-x   0 root         (0) root         (0)        0 2023-07-21 12:36:01.847718 chaosgarden-0.2.4/chaosgarden.egg-info/
+-rw-r--r--   0 root         (0) root         (0)     1694 2023-07-21 12:36:01.000000 chaosgarden-0.2.4/chaosgarden.egg-info/PKG-INFO
+-rw-r--r--   0 root         (0) root         (0)     1443 2023-07-21 12:36:01.000000 chaosgarden-0.2.4/chaosgarden.egg-info/SOURCES.txt
+-rw-r--r--   0 root         (0) root         (0)        1 2023-07-21 12:36:01.000000 chaosgarden-0.2.4/chaosgarden.egg-info/dependency_links.txt
+-rw-r--r--   0 root         (0) root         (0)      436 2023-07-21 12:36:01.000000 chaosgarden-0.2.4/chaosgarden.egg-info/requires.txt
+-rw-r--r--   0 root         (0) root         (0)       18 2023-07-21 12:36:01.000000 chaosgarden-0.2.4/chaosgarden.egg-info/top_level.txt
+-rw-r--r--   0 root         (0) root         (0)       38 2023-07-21 12:36:01.855718 chaosgarden-0.2.4/setup.cfg
+-rw-r--r--   0 root         (0) root         (0)     3331 2023-07-21 12:35:06.000000 chaosgarden-0.2.4/setup.py
```

### Comparing `chaosgarden-0.2.3/LICENSE` & `chaosgarden-0.2.4/LICENSE`

 * *Files identical despite different names*

### Comparing `chaosgarden-0.2.3/PKG-INFO` & `chaosgarden-0.2.4/PKG-INFO`

 * *Files 1% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: chaosgarden
-Version: 0.2.3
+Version: 0.2.4
 Summary: Generic cloud provider zone outage and Kubernetes pod disruption simulations with specific support for Gardener
 Home-page: https://github.com/gardener/chaos-engineering
 Author: SAP SE
 License: License :: OSI Approved :: Apache Software License
 Keywords: chaostoolkit,kubernetes,gardener
 Platform: AWS
 Platform: Azure
```

### Comparing `chaosgarden-0.2.3/chaosgarden/aws/actions.py` & `chaosgarden-0.2.4/chaosgarden/aws/actions.py`

 * *Files identical despite different names*

### Comparing `chaosgarden-0.2.3/chaosgarden/azure/__init__.py` & `chaosgarden-0.2.4/chaosgarden/azure/__init__.py`

 * *Files identical despite different names*

### Comparing `chaosgarden-0.2.3/chaosgarden/azure/actions.py` & `chaosgarden-0.2.4/chaosgarden/azure/actions.py`

 * *Files identical despite different names*

### Comparing `chaosgarden-0.2.3/chaosgarden/garden/__init__.py` & `chaosgarden-0.2.4/chaosgarden/garden/__init__.py`

 * *Files identical despite different names*

### Comparing `chaosgarden-0.2.3/chaosgarden/garden/actions.py` & `chaosgarden-0.2.4/chaosgarden/garden/actions.py`

 * *Files 2% similar despite different names*

```diff
@@ -382,14 +382,23 @@
             'instances': [{'Name': 'tag-key', 'Values': [f'kubernetes.io/cluster/{shoot.status.technicalID}']}],
             'vpcs': [{'Name': 'tag-key', 'Values': [f'kubernetes.io/cluster/{shoot.status.technicalID}']}]}
         configuration = {
             'aws_region': shoot.spec.region}
         secrets = {}
         b64decode_and_add(credentials, 'accessKeyID', secrets, 'aws_access_key_id')
         b64decode_and_add(credentials, 'secretAccessKey', secrets, 'aws_secret_access_key')
+    elif cloud_provider == 'alicloud':
+        filters = {
+            'instances': {'Tag-key': f'kubernetes.io/cluster/{shoot.status.technicalID}'},
+            'vpc': {'Name': f'shoot--{configuration.garden_project}--{configuration.garden_shoot}-vpc'}}
+        configuration = {
+            'ali_region': shoot.spec.region}
+        secrets = {}
+        b64decode_and_add(credentials, 'accessKeyID', secrets, 'ali_access_key')
+        b64decode_and_add(credentials, 'accessKeySecret', secrets, 'ali_secret_key')
     elif cloud_provider == 'azure':
         cloud = configuration.get('azure_cloud', 'AZURE_PUBLIC_CLOUD')
         filters = {
             'virtual_machines': f'where tags contains "kubernetes.io-cluster-{shoot.status.technicalID}"'}
         configuration = {
             'azure_region': shoot.spec.region,
             'azure_resource_group': shoot.spec.provider.infrastructureConfig.resourceGroup.name if 'resourceGroup' in shoot.spec.provider.infrastructureConfig else shoot.status.technicalID}
```

### Comparing `chaosgarden-0.2.3/chaosgarden/garden/probes.py` & `chaosgarden-0.2.4/chaosgarden/garden/probes.py`

 * *Files identical despite different names*

### Comparing `chaosgarden-0.2.3/chaosgarden/gcp/__init__.py` & `chaosgarden-0.2.4/chaosgarden/gcp/__init__.py`

 * *Files identical despite different names*

### Comparing `chaosgarden-0.2.3/chaosgarden/gcp/actions.py` & `chaosgarden-0.2.4/chaosgarden/gcp/actions.py`

 * *Files identical despite different names*

### Comparing `chaosgarden-0.2.3/chaosgarden/k8s/__init__.py` & `chaosgarden-0.2.4/chaosgarden/k8s/__init__.py`

 * *Files identical despite different names*

### Comparing `chaosgarden-0.2.3/chaosgarden/k8s/actions.py` & `chaosgarden-0.2.4/chaosgarden/k8s/actions.py`

 * *Files identical despite different names*

### Comparing `chaosgarden-0.2.3/chaosgarden/k8s/api/authenticators.py` & `chaosgarden-0.2.4/chaosgarden/k8s/api/authenticators.py`

 * *Files identical despite different names*

### Comparing `chaosgarden-0.2.3/chaosgarden/k8s/api/clients.py` & `chaosgarden-0.2.4/chaosgarden/k8s/api/clients.py`

 * *Files identical despite different names*

### Comparing `chaosgarden-0.2.3/chaosgarden/k8s/api/cluster.py` & `chaosgarden-0.2.4/chaosgarden/k8s/api/cluster.py`

 * *Files identical despite different names*

### Comparing `chaosgarden-0.2.3/chaosgarden/k8s/probe/metrics.py` & `chaosgarden-0.2.4/chaosgarden/k8s/probe/metrics.py`

 * *Files identical despite different names*

### Comparing `chaosgarden-0.2.3/chaosgarden/k8s/probe/resources/generate_resources.py` & `chaosgarden-0.2.4/chaosgarden/k8s/probe/resources/generate_resources.py`

 * *Files identical despite different names*

### Comparing `chaosgarden-0.2.3/chaosgarden/k8s/probe/resources/probe_pod.py` & `chaosgarden-0.2.4/chaosgarden/k8s/probe/resources/probe_pod.py`

 * *Files identical despite different names*

### Comparing `chaosgarden-0.2.3/chaosgarden/k8s/probe/resources/suicidal_pod.py` & `chaosgarden-0.2.4/chaosgarden/k8s/probe/resources/suicidal_pod.py`

 * *Files identical despite different names*

### Comparing `chaosgarden-0.2.3/chaosgarden/k8s/probe/resources/templated_resources.yaml` & `chaosgarden-0.2.4/chaosgarden/k8s/probe/resources/templated_resources.yaml`

 * *Files identical despite different names*

### Comparing `chaosgarden-0.2.3/chaosgarden/k8s/probe/thresholds.py` & `chaosgarden-0.2.4/chaosgarden/k8s/probe/thresholds.py`

 * *Files identical despite different names*

### Comparing `chaosgarden-0.2.3/chaosgarden/k8s/probes.py` & `chaosgarden-0.2.4/chaosgarden/k8s/probes.py`

 * *Files identical despite different names*

### Comparing `chaosgarden-0.2.3/chaosgarden/openstack/__init__.py` & `chaosgarden-0.2.4/chaosgarden/openstack/__init__.py`

 * *Files identical despite different names*

### Comparing `chaosgarden-0.2.3/chaosgarden/openstack/actions.py` & `chaosgarden-0.2.4/chaosgarden/openstack/actions.py`

 * *Files identical despite different names*

### Comparing `chaosgarden-0.2.3/chaosgarden/util/__init__.py` & `chaosgarden-0.2.4/chaosgarden/util/__init__.py`

 * *Files identical despite different names*

### Comparing `chaosgarden-0.2.3/chaosgarden/util/terminator.py` & `chaosgarden-0.2.4/chaosgarden/util/terminator.py`

 * *Files identical despite different names*

### Comparing `chaosgarden-0.2.3/chaosgarden/util/threading.py` & `chaosgarden-0.2.4/chaosgarden/util/threading.py`

 * *Files identical despite different names*

### Comparing `chaosgarden-0.2.3/chaosgarden/vsphere/__init__.py` & `chaosgarden-0.2.4/chaosgarden/vsphere/__init__.py`

 * *Files identical despite different names*

### Comparing `chaosgarden-0.2.3/chaosgarden/vsphere/actions.py` & `chaosgarden-0.2.4/chaosgarden/vsphere/actions.py`

 * *Files identical despite different names*

### Comparing `chaosgarden-0.2.3/chaosgarden/vsphere/pchelper.py` & `chaosgarden-0.2.4/chaosgarden/vsphere/pchelper.py`

 * *Files identical despite different names*

### Comparing `chaosgarden-0.2.3/chaosgarden.egg-info/PKG-INFO` & `chaosgarden-0.2.4/chaosgarden.egg-info/PKG-INFO`

 * *Files 1% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: chaosgarden
-Version: 0.2.3
+Version: 0.2.4
 Summary: Generic cloud provider zone outage and Kubernetes pod disruption simulations with specific support for Gardener
 Home-page: https://github.com/gardener/chaos-engineering
 Author: SAP SE
 License: License :: OSI Approved :: Apache Software License
 Keywords: chaostoolkit,kubernetes,gardener
 Platform: AWS
 Platform: Azure
```

### Comparing `chaosgarden-0.2.3/chaosgarden.egg-info/SOURCES.txt` & `chaosgarden-0.2.4/chaosgarden.egg-info/SOURCES.txt`

 * *Files 2% similar despite different names*

```diff
@@ -3,14 +3,15 @@
 chaosgarden/__init__.py
 chaosgarden.egg-info/PKG-INFO
 chaosgarden.egg-info/SOURCES.txt
 chaosgarden.egg-info/dependency_links.txt
 chaosgarden.egg-info/requires.txt
 chaosgarden.egg-info/top_level.txt
 chaosgarden/alicloud/__init__.py
+chaosgarden/alicloud/actions.py
 chaosgarden/aws/__init__.py
 chaosgarden/aws/actions.py
 chaosgarden/azure/__init__.py
 chaosgarden/azure/actions.py
 chaosgarden/garden/__init__.py
 chaosgarden/garden/actions.py
 chaosgarden/garden/probes.py
```

### Comparing `chaosgarden-0.2.3/setup.py` & `chaosgarden-0.2.4/setup.py`

 * *Files identical despite different names*

