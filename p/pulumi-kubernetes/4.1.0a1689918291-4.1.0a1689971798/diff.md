# Comparing `tmp/pulumi_kubernetes-4.1.0a1689918291.tar.gz` & `tmp/pulumi_kubernetes-4.1.0a1689971798.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "dist/pulumi_kubernetes-4.1.0a1689918291.tar", last modified: Fri Jul 21 05:53:04 2023, max compression
+gzip compressed data, was "dist/pulumi_kubernetes-4.1.0a1689971798.tar", last modified: Fri Jul 21 20:45:53 2023, max compression
```

## Comparing `pulumi_kubernetes-4.1.0a1689918291.tar` & `pulumi_kubernetes-4.1.0a1689971798.tar`

### file list

```diff
@@ -1,658 +1,658 @@
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-21 05:53:04.000000 pulumi_kubernetes-4.1.0a1689918291/
--rw-r--r--   0 runner    (1001) docker     (123)    11092 2023-07-21 05:53:04.000000 pulumi_kubernetes-4.1.0a1689918291/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (123)     8829 2023-07-21 05:53:03.000000 pulumi_kubernetes-4.1.0a1689918291/README.md
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-21 05:53:04.000000 pulumi_kubernetes-4.1.0a1689918291/pulumi_kubernetes/
--rw-r--r--   0 runner    (1001) docker     (123)    39084 2023-07-21 05:53:03.000000 pulumi_kubernetes-4.1.0a1689918291/pulumi_kubernetes/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)     6932 2023-07-21 05:53:03.000000 pulumi_kubernetes-4.1.0a1689918291/pulumi_kubernetes/_inputs.py
--rw-r--r--   0 runner    (1001) docker     (123)    40823 2023-07-21 05:53:03.000000 pulumi_kubernetes-4.1.0a1689918291/pulumi_kubernetes/_tables.py
--rw-r--r--   0 runner    (1001) docker     (123)     8050 2023-07-21 05:53:03.000000 pulumi_kubernetes-4.1.0a1689918291/pulumi_kubernetes/_utilities.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-21 05:53:04.000000 pulumi_kubernetes-4.1.0a1689918291/pulumi_kubernetes/admissionregistration/
--rw-r--r--   0 runner    (1001) docker     (123)      785 2023-07-21 05:53:03.000000 pulumi_kubernetes-4.1.0a1689918291/pulumi_kubernetes/admissionregistration/__init__.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-21 05:53:04.000000 pulumi_kubernetes-4.1.0a1689918291/pulumi_kubernetes/admissionregistration/v1/
--rw-r--r--   0 runner    (1001) docker     (123)    11822 2023-07-21 05:53:03.000000 pulumi_kubernetes-4.1.0a1689918291/pulumi_kubernetes/admissionregistration/v1/MutatingWebhookConfiguration.py
--rw-r--r--   0 runner    (1001) docker     (123)    11454 2023-07-21 05:53:03.000000 pulumi_kubernetes-4.1.0a1689918291/pulumi_kubernetes/admissionregistration/v1/MutatingWebhookConfigurationList.py
--rw-r--r--   0 runner    (1001) docker     (123)    13420 2023-07-21 05:53:03.000000 pulumi_kubernetes-4.1.0a1689918291/pulumi_kubernetes/admissionregistration/v1/MutatingWebhookConfigurationPatch.py
--rw-r--r--   0 runner    (1001) docker     (123)    11892 2023-07-21 05:53:03.000000 pulumi_kubernetes-4.1.0a1689918291/pulumi_kubernetes/admissionregistration/v1/ValidatingWebhookConfiguration.py
--rw-r--r--   0 runner    (1001) docker     (123)    11524 2023-07-21 05:53:03.000000 pulumi_kubernetes-4.1.0a1689918291/pulumi_kubernetes/admissionregistration/v1/ValidatingWebhookConfigurationList.py
--rw-r--r--   0 runner    (1001) docker     (123)    13490 2023-07-21 05:53:03.000000 pulumi_kubernetes-4.1.0a1689918291/pulumi_kubernetes/admissionregistration/v1/ValidatingWebhookConfigurationPatch.py
--rw-r--r--   0 runner    (1001) docker     (123)      572 2023-07-21 05:53:03.000000 pulumi_kubernetes-4.1.0a1689918291/pulumi_kubernetes/admissionregistration/v1/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)   126842 2023-07-21 05:53:03.000000 pulumi_kubernetes-4.1.0a1689918291/pulumi_kubernetes/admissionregistration/v1/_inputs.py
--rw-r--r--   0 runner    (1001) docker     (123)   121022 2023-07-21 05:53:03.000000 pulumi_kubernetes-4.1.0a1689918291/pulumi_kubernetes/admissionregistration/v1/outputs.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-21 05:53:04.000000 pulumi_kubernetes-4.1.0a1689918291/pulumi_kubernetes/admissionregistration/v1alpha1/
--rw-r--r--   0 runner    (1001) docker     (123)    11903 2023-07-21 05:53:03.000000 pulumi_kubernetes-4.1.0a1689918291/pulumi_kubernetes/admissionregistration/v1alpha1/ValidatingAdmissionPolicy.py
--rw-r--r--   0 runner    (1001) docker     (123)    11826 2023-07-21 05:53:03.000000 pulumi_kubernetes-4.1.0a1689918291/pulumi_kubernetes/admissionregistration/v1alpha1/ValidatingAdmissionPolicyBinding.py
--rw-r--r--   0 runner    (1001) docker     (123)    11508 2023-07-21 05:53:03.000000 pulumi_kubernetes-4.1.0a1689918291/pulumi_kubernetes/admissionregistration/v1alpha1/ValidatingAdmissionPolicyBindingList.py
--rw-r--r--   0 runner    (1001) docker     (123)    13419 2023-07-21 05:53:03.000000 pulumi_kubernetes-4.1.0a1689918291/pulumi_kubernetes/admissionregistration/v1alpha1/ValidatingAdmissionPolicyBindingPatch.py
--rw-r--r--   0 runner    (1001) docker     (123)    11339 2023-07-21 05:53:03.000000 pulumi_kubernetes-4.1.0a1689918291/pulumi_kubernetes/admissionregistration/v1alpha1/ValidatingAdmissionPolicyList.py
--rw-r--r--   0 runner    (1001) docker     (123)    13501 2023-07-21 05:53:03.000000 pulumi_kubernetes-4.1.0a1689918291/pulumi_kubernetes/admissionregistration/v1alpha1/ValidatingAdmissionPolicyPatch.py
--rw-r--r--   0 runner    (1001) docker     (123)      569 2023-07-21 05:53:03.000000 pulumi_kubernetes-4.1.0a1689918291/pulumi_kubernetes/admissionregistration/v1alpha1/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)   136918 2023-07-21 05:53:03.000000 pulumi_kubernetes-4.1.0a1689918291/pulumi_kubernetes/admissionregistration/v1alpha1/_inputs.py
--rw-r--r--   0 runner    (1001) docker     (123)   143284 2023-07-21 05:53:03.000000 pulumi_kubernetes-4.1.0a1689918291/pulumi_kubernetes/admissionregistration/v1alpha1/outputs.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-21 05:53:04.000000 pulumi_kubernetes-4.1.0a1689918291/pulumi_kubernetes/admissionregistration/v1beta1/
--rw-r--r--   0 runner    (1001) docker     (123)    12082 2023-07-21 05:53:03.000000 pulumi_kubernetes-4.1.0a1689918291/pulumi_kubernetes/admissionregistration/v1beta1/MutatingWebhookConfiguration.py
--rw-r--r--   0 runner    (1001) docker     (123)    11469 2023-07-21 05:53:03.000000 pulumi_kubernetes-4.1.0a1689918291/pulumi_kubernetes/admissionregistration/v1beta1/MutatingWebhookConfigurationList.py
--rw-r--r--   0 runner    (1001) docker     (123)    13680 2023-07-21 05:53:03.000000 pulumi_kubernetes-4.1.0a1689918291/pulumi_kubernetes/admissionregistration/v1beta1/MutatingWebhookConfigurationPatch.py
--rw-r--r--   0 runner    (1001) docker     (123)    12156 2023-07-21 05:53:03.000000 pulumi_kubernetes-4.1.0a1689918291/pulumi_kubernetes/admissionregistration/v1beta1/ValidatingWebhookConfiguration.py
--rw-r--r--   0 runner    (1001) docker     (123)    11539 2023-07-21 05:53:03.000000 pulumi_kubernetes-4.1.0a1689918291/pulumi_kubernetes/admissionregistration/v1beta1/ValidatingWebhookConfigurationList.py
--rw-r--r--   0 runner    (1001) docker     (123)    13754 2023-07-21 05:53:03.000000 pulumi_kubernetes-4.1.0a1689918291/pulumi_kubernetes/admissionregistration/v1beta1/ValidatingWebhookConfigurationPatch.py
--rw-r--r--   0 runner    (1001) docker     (123)      572 2023-07-21 05:53:03.000000 pulumi_kubernetes-4.1.0a1689918291/pulumi_kubernetes/admissionregistration/v1beta1/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)   108512 2023-07-21 05:53:03.000000 pulumi_kubernetes-4.1.0a1689918291/pulumi_kubernetes/admissionregistration/v1beta1/_inputs.py
--rw-r--r--   0 runner    (1001) docker     (123)   104062 2023-07-21 05:53:03.000000 pulumi_kubernetes-4.1.0a1689918291/pulumi_kubernetes/admissionregistration/v1beta1/outputs.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-21 05:53:04.000000 pulumi_kubernetes-4.1.0a1689918291/pulumi_kubernetes/apiextensions/
--rw-r--r--   0 runner    (1001) docker     (123)     9255 2023-07-21 05:53:03.000000 pulumi_kubernetes-4.1.0a1689918291/pulumi_kubernetes/apiextensions/CustomResource.py
--rw-r--r--   0 runner    (1001) docker     (123)     7835 2023-07-21 05:53:03.000000 pulumi_kubernetes-4.1.0a1689918291/pulumi_kubernetes/apiextensions/CustomResourcePatch.py
--rw-r--r--   0 runner    (1001) docker     (123)      672 2023-07-21 05:53:03.000000 pulumi_kubernetes-4.1.0a1689918291/pulumi_kubernetes/apiextensions/__init__.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-21 05:53:04.000000 pulumi_kubernetes-4.1.0a1689918291/pulumi_kubernetes/apiextensions/v1/
--rw-r--r--   0 runner    (1001) docker     (123)    11920 2023-07-21 05:53:03.000000 pulumi_kubernetes-4.1.0a1689918291/pulumi_kubernetes/apiextensions/v1/CustomResourceDefinition.py
--rw-r--r--   0 runner    (1001) docker     (123)    11390 2023-07-21 05:53:03.000000 pulumi_kubernetes-4.1.0a1689918291/pulumi_kubernetes/apiextensions/v1/CustomResourceDefinitionList.py
--rw-r--r--   0 runner    (1001) docker     (123)    13496 2023-07-21 05:53:03.000000 pulumi_kubernetes-4.1.0a1689918291/pulumi_kubernetes/apiextensions/v1/CustomResourceDefinitionPatch.py
--rw-r--r--   0 runner    (1001) docker     (123)      413 2023-07-21 05:53:03.000000 pulumi_kubernetes-4.1.0a1689918291/pulumi_kubernetes/apiextensions/v1/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)   198456 2023-07-21 05:53:03.000000 pulumi_kubernetes-4.1.0a1689918291/pulumi_kubernetes/apiextensions/v1/_inputs.py
--rw-r--r--   0 runner    (1001) docker     (123)   189683 2023-07-21 05:53:03.000000 pulumi_kubernetes-4.1.0a1689918291/pulumi_kubernetes/apiextensions/v1/outputs.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-21 05:53:04.000000 pulumi_kubernetes-4.1.0a1689918291/pulumi_kubernetes/apiextensions/v1beta1/
--rw-r--r--   0 runner    (1001) docker     (123)    11420 2023-07-21 05:53:03.000000 pulumi_kubernetes-4.1.0a1689918291/pulumi_kubernetes/apiextensions/v1beta1/CustomResourceDefinition.py
--rw-r--r--   0 runner    (1001) docker     (123)    10673 2023-07-21 05:53:03.000000 pulumi_kubernetes-4.1.0a1689918291/pulumi_kubernetes/apiextensions/v1beta1/CustomResourceDefinitionList.py
--rw-r--r--   0 runner    (1001) docker     (123)    12986 2023-07-21 05:53:03.000000 pulumi_kubernetes-4.1.0a1689918291/pulumi_kubernetes/apiextensions/v1beta1/CustomResourceDefinitionPatch.py
--rw-r--r--   0 runner    (1001) docker     (123)      413 2023-07-21 05:53:03.000000 pulumi_kubernetes-4.1.0a1689918291/pulumi_kubernetes/apiextensions/v1beta1/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)   183209 2023-07-21 05:53:03.000000 pulumi_kubernetes-4.1.0a1689918291/pulumi_kubernetes/apiextensions/v1beta1/_inputs.py
--rw-r--r--   0 runner    (1001) docker     (123)   173449 2023-07-21 05:53:03.000000 pulumi_kubernetes-4.1.0a1689918291/pulumi_kubernetes/apiextensions/v1beta1/outputs.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-21 05:53:04.000000 pulumi_kubernetes-4.1.0a1689918291/pulumi_kubernetes/apiregistration/
--rw-r--r--   0 runner    (1001) docker     (123)      571 2023-07-21 05:53:03.000000 pulumi_kubernetes-4.1.0a1689918291/pulumi_kubernetes/apiregistration/__init__.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-21 05:53:04.000000 pulumi_kubernetes-4.1.0a1689918291/pulumi_kubernetes/apiregistration/v1/
--rw-r--r--   0 runner    (1001) docker     (123)    11560 2023-07-21 05:53:03.000000 pulumi_kubernetes-4.1.0a1689918291/pulumi_kubernetes/apiregistration/v1/APIService.py
--rw-r--r--   0 runner    (1001) docker     (123)    11038 2023-07-21 05:53:03.000000 pulumi_kubernetes-4.1.0a1689918291/pulumi_kubernetes/apiregistration/v1/APIServiceList.py
--rw-r--r--   0 runner    (1001) docker     (123)    13173 2023-07-21 05:53:03.000000 pulumi_kubernetes-4.1.0a1689918291/pulumi_kubernetes/apiregistration/v1/APIServicePatch.py
--rw-r--r--   0 runner    (1001) docker     (123)      371 2023-07-21 05:53:03.000000 pulumi_kubernetes-4.1.0a1689918291/pulumi_kubernetes/apiregistration/v1/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)    30708 2023-07-21 05:53:03.000000 pulumi_kubernetes-4.1.0a1689918291/pulumi_kubernetes/apiregistration/v1/_inputs.py
--rw-r--r--   0 runner    (1001) docker     (123)    32896 2023-07-21 05:53:03.000000 pulumi_kubernetes-4.1.0a1689918291/pulumi_kubernetes/apiregistration/v1/outputs.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-21 05:53:04.000000 pulumi_kubernetes-4.1.0a1689918291/pulumi_kubernetes/apiregistration/v1beta1/
--rw-r--r--   0 runner    (1001) docker     (123)    10830 2023-07-21 05:53:03.000000 pulumi_kubernetes-4.1.0a1689918291/pulumi_kubernetes/apiregistration/v1beta1/APIService.py
--rw-r--r--   0 runner    (1001) docker     (123)     9978 2023-07-21 05:53:03.000000 pulumi_kubernetes-4.1.0a1689918291/pulumi_kubernetes/apiregistration/v1beta1/APIServiceList.py
--rw-r--r--   0 runner    (1001) docker     (123)    12433 2023-07-21 05:53:03.000000 pulumi_kubernetes-4.1.0a1689918291/pulumi_kubernetes/apiregistration/v1beta1/APIServicePatch.py
--rw-r--r--   0 runner    (1001) docker     (123)      371 2023-07-21 05:53:03.000000 pulumi_kubernetes-4.1.0a1689918291/pulumi_kubernetes/apiregistration/v1beta1/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)    30275 2023-07-21 05:53:03.000000 pulumi_kubernetes-4.1.0a1689918291/pulumi_kubernetes/apiregistration/v1beta1/_inputs.py
--rw-r--r--   0 runner    (1001) docker     (123)    32487 2023-07-21 05:53:03.000000 pulumi_kubernetes-4.1.0a1689918291/pulumi_kubernetes/apiregistration/v1beta1/outputs.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-21 05:53:04.000000 pulumi_kubernetes-4.1.0a1689918291/pulumi_kubernetes/apps/
--rw-r--r--   0 runner    (1001) docker     (123)      677 2023-07-21 05:53:03.000000 pulumi_kubernetes-4.1.0a1689918291/pulumi_kubernetes/apps/__init__.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-21 05:53:04.000000 pulumi_kubernetes-4.1.0a1689918291/pulumi_kubernetes/apps/v1/
--rw-r--r--   0 runner    (1001) docker     (123)    13236 2023-07-21 05:53:03.000000 pulumi_kubernetes-4.1.0a1689918291/pulumi_kubernetes/apps/v1/ControllerRevision.py
--rw-r--r--   0 runner    (1001) docker     (123)    11036 2023-07-21 05:53:03.000000 pulumi_kubernetes-4.1.0a1689918291/pulumi_kubernetes/apps/v1/ControllerRevisionList.py
--rw-r--r--   0 runner    (1001) docker     (123)    14778 2023-07-21 05:53:03.000000 pulumi_kubernetes-4.1.0a1689918291/pulumi_kubernetes/apps/v1/ControllerRevisionPatch.py
--rw-r--r--   0 runner    (1001) docker     (123)    11854 2023-07-21 05:53:03.000000 pulumi_kubernetes-4.1.0a1689918291/pulumi_kubernetes/apps/v1/DaemonSet.py
--rw-r--r--   0 runner    (1001) docker     (123)    10767 2023-07-21 05:53:03.000000 pulumi_kubernetes-4.1.0a1689918291/pulumi_kubernetes/apps/v1/DaemonSetList.py
--rw-r--r--   0 runner    (1001) docker     (123)    13462 2023-07-21 05:53:03.000000 pulumi_kubernetes-4.1.0a1689918291/pulumi_kubernetes/apps/v1/DaemonSetPatch.py
--rw-r--r--   0 runner    (1001) docker     (123)    19970 2023-07-21 05:53:03.000000 pulumi_kubernetes-4.1.0a1689918291/pulumi_kubernetes/apps/v1/Deployment.py
--rw-r--r--   0 runner    (1001) docker     (123)    10412 2023-07-21 05:53:03.000000 pulumi_kubernetes-4.1.0a1689918291/pulumi_kubernetes/apps/v1/DeploymentList.py
--rw-r--r--   0 runner    (1001) docker     (123)    16049 2023-07-21 05:53:03.000000 pulumi_kubernetes-4.1.0a1689918291/pulumi_kubernetes/apps/v1/DeploymentPatch.py
--rw-r--r--   0 runner    (1001) docker     (123)    12580 2023-07-21 05:53:03.000000 pulumi_kubernetes-4.1.0a1689918291/pulumi_kubernetes/apps/v1/ReplicaSet.py
--rw-r--r--   0 runner    (1001) docker     (123)    11164 2023-07-21 05:53:03.000000 pulumi_kubernetes-4.1.0a1689918291/pulumi_kubernetes/apps/v1/ReplicaSetList.py
--rw-r--r--   0 runner    (1001) docker     (123)    14188 2023-07-21 05:53:03.000000 pulumi_kubernetes-4.1.0a1689918291/pulumi_kubernetes/apps/v1/ReplicaSetPatch.py
--rw-r--r--   0 runner    (1001) docker     (123)    24360 2023-07-21 05:53:03.000000 pulumi_kubernetes-4.1.0a1689918291/pulumi_kubernetes/apps/v1/StatefulSet.py
--rw-r--r--   0 runner    (1001) docker     (123)    10887 2023-07-21 05:53:03.000000 pulumi_kubernetes-4.1.0a1689918291/pulumi_kubernetes/apps/v1/StatefulSetList.py
--rw-r--r--   0 runner    (1001) docker     (123)    15062 2023-07-21 05:53:03.000000 pulumi_kubernetes-4.1.0a1689918291/pulumi_kubernetes/apps/v1/StatefulSetPatch.py
--rw-r--r--   0 runner    (1001) docker     (123)      743 2023-07-21 05:53:03.000000 pulumi_kubernetes-4.1.0a1689918291/pulumi_kubernetes/apps/v1/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)   177605 2023-07-21 05:53:03.000000 pulumi_kubernetes-4.1.0a1689918291/pulumi_kubernetes/apps/v1/_inputs.py
--rw-r--r--   0 runner    (1001) docker     (123)   218849 2023-07-21 05:53:03.000000 pulumi_kubernetes-4.1.0a1689918291/pulumi_kubernetes/apps/v1/outputs.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-21 05:53:04.000000 pulumi_kubernetes-4.1.0a1689918291/pulumi_kubernetes/apps/v1beta1/
--rw-r--r--   0 runner    (1001) docker     (123)    13246 2023-07-21 05:53:03.000000 pulumi_kubernetes-4.1.0a1689918291/pulumi_kubernetes/apps/v1beta1/ControllerRevision.py
--rw-r--r--   0 runner    (1001) docker     (123)    11051 2023-07-21 05:53:03.000000 pulumi_kubernetes-4.1.0a1689918291/pulumi_kubernetes/apps/v1beta1/ControllerRevisionList.py
--rw-r--r--   0 runner    (1001) docker     (123)    14788 2023-07-21 05:53:03.000000 pulumi_kubernetes-4.1.0a1689918291/pulumi_kubernetes/apps/v1beta1/ControllerRevisionPatch.py
--rw-r--r--   0 runner    (1001) docker     (123)    14022 2023-07-21 05:53:03.000000 pulumi_kubernetes-4.1.0a1689918291/pulumi_kubernetes/apps/v1beta1/Deployment.py
--rw-r--r--   0 runner    (1001) docker     (123)    10427 2023-07-21 05:53:03.000000 pulumi_kubernetes-4.1.0a1689918291/pulumi_kubernetes/apps/v1beta1/DeploymentList.py
--rw-r--r--   0 runner    (1001) docker     (123)    15635 2023-07-21 05:53:03.000000 pulumi_kubernetes-4.1.0a1689918291/pulumi_kubernetes/apps/v1beta1/DeploymentPatch.py
--rw-r--r--   0 runner    (1001) docker     (123)    12724 2023-07-21 05:53:03.000000 pulumi_kubernetes-4.1.0a1689918291/pulumi_kubernetes/apps/v1beta1/StatefulSet.py
--rw-r--r--   0 runner    (1001) docker     (123)     9792 2023-07-21 05:53:03.000000 pulumi_kubernetes-4.1.0a1689918291/pulumi_kubernetes/apps/v1beta1/StatefulSetList.py
--rw-r--r--   0 runner    (1001) docker     (123)    14322 2023-07-21 05:53:03.000000 pulumi_kubernetes-4.1.0a1689918291/pulumi_kubernetes/apps/v1beta1/StatefulSetPatch.py
--rw-r--r--   0 runner    (1001) docker     (123)      572 2023-07-21 05:53:03.000000 pulumi_kubernetes-4.1.0a1689918291/pulumi_kubernetes/apps/v1beta1/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)    92195 2023-07-21 05:53:03.000000 pulumi_kubernetes-4.1.0a1689918291/pulumi_kubernetes/apps/v1beta1/_inputs.py
--rw-r--r--   0 runner    (1001) docker     (123)   112665 2023-07-21 05:53:03.000000 pulumi_kubernetes-4.1.0a1689918291/pulumi_kubernetes/apps/v1beta1/outputs.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-21 05:53:04.000000 pulumi_kubernetes-4.1.0a1689918291/pulumi_kubernetes/apps/v1beta2/
--rw-r--r--   0 runner    (1001) docker     (123)    13246 2023-07-21 05:53:03.000000 pulumi_kubernetes-4.1.0a1689918291/pulumi_kubernetes/apps/v1beta2/ControllerRevision.py
--rw-r--r--   0 runner    (1001) docker     (123)    11051 2023-07-21 05:53:03.000000 pulumi_kubernetes-4.1.0a1689918291/pulumi_kubernetes/apps/v1beta2/ControllerRevisionList.py
--rw-r--r--   0 runner    (1001) docker     (123)    14788 2023-07-21 05:53:03.000000 pulumi_kubernetes-4.1.0a1689918291/pulumi_kubernetes/apps/v1beta2/ControllerRevisionPatch.py
--rw-r--r--   0 runner    (1001) docker     (123)    11864 2023-07-21 05:53:03.000000 pulumi_kubernetes-4.1.0a1689918291/pulumi_kubernetes/apps/v1beta2/DaemonSet.py
--rw-r--r--   0 runner    (1001) docker     (123)    10782 2023-07-21 05:53:03.000000 pulumi_kubernetes-4.1.0a1689918291/pulumi_kubernetes/apps/v1beta2/DaemonSetList.py
--rw-r--r--   0 runner    (1001) docker     (123)    13472 2023-07-21 05:53:03.000000 pulumi_kubernetes-4.1.0a1689918291/pulumi_kubernetes/apps/v1beta2/DaemonSetPatch.py
--rw-r--r--   0 runner    (1001) docker     (123)    14022 2023-07-21 05:53:03.000000 pulumi_kubernetes-4.1.0a1689918291/pulumi_kubernetes/apps/v1beta2/Deployment.py
--rw-r--r--   0 runner    (1001) docker     (123)    10427 2023-07-21 05:53:03.000000 pulumi_kubernetes-4.1.0a1689918291/pulumi_kubernetes/apps/v1beta2/DeploymentList.py
--rw-r--r--   0 runner    (1001) docker     (123)    15635 2023-07-21 05:53:03.000000 pulumi_kubernetes-4.1.0a1689918291/pulumi_kubernetes/apps/v1beta2/DeploymentPatch.py
--rw-r--r--   0 runner    (1001) docker     (123)    12590 2023-07-21 05:53:03.000000 pulumi_kubernetes-4.1.0a1689918291/pulumi_kubernetes/apps/v1beta2/ReplicaSet.py
--rw-r--r--   0 runner    (1001) docker     (123)    11179 2023-07-21 05:53:03.000000 pulumi_kubernetes-4.1.0a1689918291/pulumi_kubernetes/apps/v1beta2/ReplicaSetList.py
--rw-r--r--   0 runner    (1001) docker     (123)    14198 2023-07-21 05:53:03.000000 pulumi_kubernetes-4.1.0a1689918291/pulumi_kubernetes/apps/v1beta2/ReplicaSetPatch.py
--rw-r--r--   0 runner    (1001) docker     (123)    12724 2023-07-21 05:53:03.000000 pulumi_kubernetes-4.1.0a1689918291/pulumi_kubernetes/apps/v1beta2/StatefulSet.py
--rw-r--r--   0 runner    (1001) docker     (123)     9792 2023-07-21 05:53:03.000000 pulumi_kubernetes-4.1.0a1689918291/pulumi_kubernetes/apps/v1beta2/StatefulSetList.py
--rw-r--r--   0 runner    (1001) docker     (123)    14322 2023-07-21 05:53:03.000000 pulumi_kubernetes-4.1.0a1689918291/pulumi_kubernetes/apps/v1beta2/StatefulSetPatch.py
--rw-r--r--   0 runner    (1001) docker     (123)      743 2023-07-21 05:53:03.000000 pulumi_kubernetes-4.1.0a1689918291/pulumi_kubernetes/apps/v1beta2/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)   147337 2023-07-21 05:53:03.000000 pulumi_kubernetes-4.1.0a1689918291/pulumi_kubernetes/apps/v1beta2/_inputs.py
--rw-r--r--   0 runner    (1001) docker     (123)   187289 2023-07-21 05:53:03.000000 pulumi_kubernetes-4.1.0a1689918291/pulumi_kubernetes/apps/v1beta2/outputs.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-21 05:53:04.000000 pulumi_kubernetes-4.1.0a1689918291/pulumi_kubernetes/auditregistration/
--rw-r--r--   0 runner    (1001) docker     (123)      439 2023-07-21 05:53:03.000000 pulumi_kubernetes-4.1.0a1689918291/pulumi_kubernetes/auditregistration/__init__.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-21 05:53:04.000000 pulumi_kubernetes-4.1.0a1689918291/pulumi_kubernetes/auditregistration/v1alpha1/
--rw-r--r--   0 runner    (1001) docker     (123)     9955 2023-07-21 05:53:03.000000 pulumi_kubernetes-4.1.0a1689918291/pulumi_kubernetes/auditregistration/v1alpha1/AuditSink.py
--rw-r--r--   0 runner    (1001) docker     (123)    10119 2023-07-21 05:53:03.000000 pulumi_kubernetes-4.1.0a1689918291/pulumi_kubernetes/auditregistration/v1alpha1/AuditSinkList.py
--rw-r--r--   0 runner    (1001) docker     (123)    11538 2023-07-21 05:53:03.000000 pulumi_kubernetes-4.1.0a1689918291/pulumi_kubernetes/auditregistration/v1alpha1/AuditSinkPatch.py
--rw-r--r--   0 runner    (1001) docker     (123)      368 2023-07-21 05:53:03.000000 pulumi_kubernetes-4.1.0a1689918291/pulumi_kubernetes/auditregistration/v1alpha1/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)    30765 2023-07-21 05:53:03.000000 pulumi_kubernetes-4.1.0a1689918291/pulumi_kubernetes/auditregistration/v1alpha1/_inputs.py
--rw-r--r--   0 runner    (1001) docker     (123)    28907 2023-07-21 05:53:03.000000 pulumi_kubernetes-4.1.0a1689918291/pulumi_kubernetes/auditregistration/v1alpha1/outputs.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-21 05:53:04.000000 pulumi_kubernetes-4.1.0a1689918291/pulumi_kubernetes/autoscaling/
--rw-r--r--   0 runner    (1001) docker     (123)      853 2023-07-21 05:53:03.000000 pulumi_kubernetes-4.1.0a1689918291/pulumi_kubernetes/autoscaling/__init__.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-21 05:53:04.000000 pulumi_kubernetes-4.1.0a1689918291/pulumi_kubernetes/autoscaling/v1/
--rw-r--r--   0 runner    (1001) docker     (123)    12143 2023-07-21 05:53:03.000000 pulumi_kubernetes-4.1.0a1689918291/pulumi_kubernetes/autoscaling/v1/HorizontalPodAutoscaler.py
--rw-r--r--   0 runner    (1001) docker     (123)    10846 2023-07-21 05:53:03.000000 pulumi_kubernetes-4.1.0a1689918291/pulumi_kubernetes/autoscaling/v1/HorizontalPodAutoscalerList.py
--rw-r--r--   0 runner    (1001) docker     (123)    13756 2023-07-21 05:53:03.000000 pulumi_kubernetes-4.1.0a1689918291/pulumi_kubernetes/autoscaling/v1/HorizontalPodAutoscalerPatch.py
--rw-r--r--   0 runner    (1001) docker     (123)      410 2023-07-21 05:53:03.000000 pulumi_kubernetes-4.1.0a1689918291/pulumi_kubernetes/autoscaling/v1/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)    22804 2023-07-21 05:53:03.000000 pulumi_kubernetes-4.1.0a1689918291/pulumi_kubernetes/autoscaling/v1/_inputs.py
--rw-r--r--   0 runner    (1001) docker     (123)    28045 2023-07-21 05:53:03.000000 pulumi_kubernetes-4.1.0a1689918291/pulumi_kubernetes/autoscaling/v1/outputs.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-21 05:53:04.000000 pulumi_kubernetes-4.1.0a1689918291/pulumi_kubernetes/autoscaling/v2/
--rw-r--r--   0 runner    (1001) docker     (123)    12613 2023-07-21 05:53:03.000000 pulumi_kubernetes-4.1.0a1689918291/pulumi_kubernetes/autoscaling/v2/HorizontalPodAutoscaler.py
--rw-r--r--   0 runner    (1001) docker     (123)    10976 2023-07-21 05:53:03.000000 pulumi_kubernetes-4.1.0a1689918291/pulumi_kubernetes/autoscaling/v2/HorizontalPodAutoscalerList.py
--rw-r--r--   0 runner    (1001) docker     (123)    14226 2023-07-21 05:53:03.000000 pulumi_kubernetes-4.1.0a1689918291/pulumi_kubernetes/autoscaling/v2/HorizontalPodAutoscalerPatch.py
--rw-r--r--   0 runner    (1001) docker     (123)      410 2023-07-21 05:53:03.000000 pulumi_kubernetes-4.1.0a1689918291/pulumi_kubernetes/autoscaling/v2/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)   109207 2023-07-21 05:53:03.000000 pulumi_kubernetes-4.1.0a1689918291/pulumi_kubernetes/autoscaling/v2/_inputs.py
--rw-r--r--   0 runner    (1001) docker     (123)   137695 2023-07-21 05:53:03.000000 pulumi_kubernetes-4.1.0a1689918291/pulumi_kubernetes/autoscaling/v2/outputs.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-21 05:53:04.000000 pulumi_kubernetes-4.1.0a1689918291/pulumi_kubernetes/autoscaling/v2beta1/
--rw-r--r--   0 runner    (1001) docker     (123)    12623 2023-07-21 05:53:03.000000 pulumi_kubernetes-4.1.0a1689918291/pulumi_kubernetes/autoscaling/v2beta1/HorizontalPodAutoscaler.py
--rw-r--r--   0 runner    (1001) docker     (123)    10983 2023-07-21 05:53:03.000000 pulumi_kubernetes-4.1.0a1689918291/pulumi_kubernetes/autoscaling/v2beta1/HorizontalPodAutoscalerList.py
--rw-r--r--   0 runner    (1001) docker     (123)    14236 2023-07-21 05:53:03.000000 pulumi_kubernetes-4.1.0a1689918291/pulumi_kubernetes/autoscaling/v2beta1/HorizontalPodAutoscalerPatch.py
--rw-r--r--   0 runner    (1001) docker     (123)      410 2023-07-21 05:53:03.000000 pulumi_kubernetes-4.1.0a1689918291/pulumi_kubernetes/autoscaling/v2beta1/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)    99993 2023-07-21 05:53:03.000000 pulumi_kubernetes-4.1.0a1689918291/pulumi_kubernetes/autoscaling/v2beta1/_inputs.py
--rw-r--r--   0 runner    (1001) docker     (123)   138421 2023-07-21 05:53:03.000000 pulumi_kubernetes-4.1.0a1689918291/pulumi_kubernetes/autoscaling/v2beta1/outputs.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-21 05:53:04.000000 pulumi_kubernetes-4.1.0a1689918291/pulumi_kubernetes/autoscaling/v2beta2/
--rw-r--r--   0 runner    (1001) docker     (123)    12623 2023-07-21 05:53:03.000000 pulumi_kubernetes-4.1.0a1689918291/pulumi_kubernetes/autoscaling/v2beta2/HorizontalPodAutoscaler.py
--rw-r--r--   0 runner    (1001) docker     (123)    10991 2023-07-21 05:53:03.000000 pulumi_kubernetes-4.1.0a1689918291/pulumi_kubernetes/autoscaling/v2beta2/HorizontalPodAutoscalerList.py
--rw-r--r--   0 runner    (1001) docker     (123)    14236 2023-07-21 05:53:03.000000 pulumi_kubernetes-4.1.0a1689918291/pulumi_kubernetes/autoscaling/v2beta2/HorizontalPodAutoscalerPatch.py
--rw-r--r--   0 runner    (1001) docker     (123)      410 2023-07-21 05:53:03.000000 pulumi_kubernetes-4.1.0a1689918291/pulumi_kubernetes/autoscaling/v2beta2/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)   107200 2023-07-21 05:53:03.000000 pulumi_kubernetes-4.1.0a1689918291/pulumi_kubernetes/autoscaling/v2beta2/_inputs.py
--rw-r--r--   0 runner    (1001) docker     (123)   135212 2023-07-21 05:53:03.000000 pulumi_kubernetes-4.1.0a1689918291/pulumi_kubernetes/autoscaling/v2beta2/outputs.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-21 05:53:04.000000 pulumi_kubernetes-4.1.0a1689918291/pulumi_kubernetes/batch/
--rw-r--r--   0 runner    (1001) docker     (123)      689 2023-07-21 05:53:03.000000 pulumi_kubernetes-4.1.0a1689918291/pulumi_kubernetes/batch/__init__.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-21 05:53:04.000000 pulumi_kubernetes-4.1.0a1689918291/pulumi_kubernetes/batch/v1/
--rw-r--r--   0 runner    (1001) docker     (123)    11846 2023-07-21 05:53:03.000000 pulumi_kubernetes-4.1.0a1689918291/pulumi_kubernetes/batch/v1/CronJob.py
--rw-r--r--   0 runner    (1001) docker     (123)    10740 2023-07-21 05:53:03.000000 pulumi_kubernetes-4.1.0a1689918291/pulumi_kubernetes/batch/v1/CronJobList.py
--rw-r--r--   0 runner    (1001) docker     (123)    13454 2023-07-21 05:53:03.000000 pulumi_kubernetes-4.1.0a1689918291/pulumi_kubernetes/batch/v1/CronJobPatch.py
--rw-r--r--   0 runner    (1001) docker     (123)    17964 2023-07-21 05:53:03.000000 pulumi_kubernetes-4.1.0a1689918291/pulumi_kubernetes/batch/v1/Job.py
--rw-r--r--   0 runner    (1001) docker     (123)    10598 2023-07-21 05:53:03.000000 pulumi_kubernetes-4.1.0a1689918291/pulumi_kubernetes/batch/v1/JobList.py
--rw-r--r--   0 runner    (1001) docker     (123)    15544 2023-07-21 05:53:03.000000 pulumi_kubernetes-4.1.0a1689918291/pulumi_kubernetes/batch/v1/JobPatch.py
--rw-r--r--   0 runner    (1001) docker     (123)      428 2023-07-21 05:53:03.000000 pulumi_kubernetes-4.1.0a1689918291/pulumi_kubernetes/batch/v1/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)   107978 2023-07-21 05:53:03.000000 pulumi_kubernetes-4.1.0a1689918291/pulumi_kubernetes/batch/v1/_inputs.py
--rw-r--r--   0 runner    (1001) docker     (123)   121425 2023-07-21 05:53:03.000000 pulumi_kubernetes-4.1.0a1689918291/pulumi_kubernetes/batch/v1/outputs.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-21 05:53:04.000000 pulumi_kubernetes-4.1.0a1689918291/pulumi_kubernetes/batch/v1beta1/
--rw-r--r--   0 runner    (1001) docker     (123)    11888 2023-07-21 05:53:03.000000 pulumi_kubernetes-4.1.0a1689918291/pulumi_kubernetes/batch/v1beta1/CronJob.py
--rw-r--r--   0 runner    (1001) docker     (123)    10787 2023-07-21 05:53:03.000000 pulumi_kubernetes-4.1.0a1689918291/pulumi_kubernetes/batch/v1beta1/CronJobList.py
--rw-r--r--   0 runner    (1001) docker     (123)    13496 2023-07-21 05:53:03.000000 pulumi_kubernetes-4.1.0a1689918291/pulumi_kubernetes/batch/v1beta1/CronJobPatch.py
--rw-r--r--   0 runner    (1001) docker     (123)      362 2023-07-21 05:53:03.000000 pulumi_kubernetes-4.1.0a1689918291/pulumi_kubernetes/batch/v1beta1/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)    23861 2023-07-21 05:53:03.000000 pulumi_kubernetes-4.1.0a1689918291/pulumi_kubernetes/batch/v1beta1/_inputs.py
--rw-r--r--   0 runner    (1001) docker     (123)    24638 2023-07-21 05:53:03.000000 pulumi_kubernetes-4.1.0a1689918291/pulumi_kubernetes/batch/v1beta1/outputs.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-21 05:53:04.000000 pulumi_kubernetes-4.1.0a1689918291/pulumi_kubernetes/batch/v2alpha1/
--rw-r--r--   0 runner    (1001) docker     (123)    11890 2023-07-21 05:53:03.000000 pulumi_kubernetes-4.1.0a1689918291/pulumi_kubernetes/batch/v2alpha1/CronJob.py
--rw-r--r--   0 runner    (1001) docker     (123)    10790 2023-07-21 05:53:03.000000 pulumi_kubernetes-4.1.0a1689918291/pulumi_kubernetes/batch/v2alpha1/CronJobList.py
--rw-r--r--   0 runner    (1001) docker     (123)    13498 2023-07-21 05:53:03.000000 pulumi_kubernetes-4.1.0a1689918291/pulumi_kubernetes/batch/v2alpha1/CronJobPatch.py
--rw-r--r--   0 runner    (1001) docker     (123)      362 2023-07-21 05:53:03.000000 pulumi_kubernetes-4.1.0a1689918291/pulumi_kubernetes/batch/v2alpha1/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)    23742 2023-07-21 05:53:03.000000 pulumi_kubernetes-4.1.0a1689918291/pulumi_kubernetes/batch/v2alpha1/_inputs.py
--rw-r--r--   0 runner    (1001) docker     (123)    24519 2023-07-21 05:53:03.000000 pulumi_kubernetes-4.1.0a1689918291/pulumi_kubernetes/batch/v2alpha1/outputs.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-21 05:53:04.000000 pulumi_kubernetes-4.1.0a1689918291/pulumi_kubernetes/certificates/
--rw-r--r--   0 runner    (1001) docker     (123)      731 2023-07-21 05:53:03.000000 pulumi_kubernetes-4.1.0a1689918291/pulumi_kubernetes/certificates/__init__.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-21 05:53:04.000000 pulumi_kubernetes-4.1.0a1689918291/pulumi_kubernetes/certificates/v1/
--rw-r--r--   0 runner    (1001) docker     (123)    13158 2023-07-21 05:53:03.000000 pulumi_kubernetes-4.1.0a1689918291/pulumi_kubernetes/certificates/v1/CertificateSigningRequest.py
--rw-r--r--   0 runner    (1001) docker     (123)    10712 2023-07-21 05:53:03.000000 pulumi_kubernetes-4.1.0a1689918291/pulumi_kubernetes/certificates/v1/CertificateSigningRequestList.py
--rw-r--r--   0 runner    (1001) docker     (123)    14724 2023-07-21 05:53:03.000000 pulumi_kubernetes-4.1.0a1689918291/pulumi_kubernetes/certificates/v1/CertificateSigningRequestPatch.py
--rw-r--r--   0 runner    (1001) docker     (123)      416 2023-07-21 05:53:03.000000 pulumi_kubernetes-4.1.0a1689918291/pulumi_kubernetes/certificates/v1/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)    44481 2023-07-21 05:53:03.000000 pulumi_kubernetes-4.1.0a1689918291/pulumi_kubernetes/certificates/v1/_inputs.py
--rw-r--r--   0 runner    (1001) docker     (123)    53207 2023-07-21 05:53:03.000000 pulumi_kubernetes-4.1.0a1689918291/pulumi_kubernetes/certificates/v1/outputs.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-21 05:53:04.000000 pulumi_kubernetes-4.1.0a1689918291/pulumi_kubernetes/certificates/v1alpha1/
--rw-r--r--   0 runner    (1001) docker     (123)    12314 2023-07-21 05:53:03.000000 pulumi_kubernetes-4.1.0a1689918291/pulumi_kubernetes/certificates/v1alpha1/ClusterTrustBundle.py
--rw-r--r--   0 runner    (1001) docker     (123)    10841 2023-07-21 05:53:03.000000 pulumi_kubernetes-4.1.0a1689918291/pulumi_kubernetes/certificates/v1alpha1/ClusterTrustBundleList.py
--rw-r--r--   0 runner    (1001) docker     (123)    13880 2023-07-21 05:53:03.000000 pulumi_kubernetes-4.1.0a1689918291/pulumi_kubernetes/certificates/v1alpha1/ClusterTrustBundlePatch.py
--rw-r--r--   0 runner    (1001) docker     (123)      395 2023-07-21 05:53:03.000000 pulumi_kubernetes-4.1.0a1689918291/pulumi_kubernetes/certificates/v1alpha1/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)    13356 2023-07-21 05:53:03.000000 pulumi_kubernetes-4.1.0a1689918291/pulumi_kubernetes/certificates/v1alpha1/_inputs.py
--rw-r--r--   0 runner    (1001) docker     (123)    14968 2023-07-21 05:53:03.000000 pulumi_kubernetes-4.1.0a1689918291/pulumi_kubernetes/certificates/v1alpha1/outputs.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-21 05:53:04.000000 pulumi_kubernetes-4.1.0a1689918291/pulumi_kubernetes/certificates/v1beta1/
--rw-r--r--   0 runner    (1001) docker     (123)    10967 2023-07-21 05:53:03.000000 pulumi_kubernetes-4.1.0a1689918291/pulumi_kubernetes/certificates/v1beta1/CertificateSigningRequest.py
--rw-r--r--   0 runner    (1001) docker     (123)    10249 2023-07-21 05:53:03.000000 pulumi_kubernetes-4.1.0a1689918291/pulumi_kubernetes/certificates/v1beta1/CertificateSigningRequestList.py
--rw-r--r--   0 runner    (1001) docker     (123)    12560 2023-07-21 05:53:03.000000 pulumi_kubernetes-4.1.0a1689918291/pulumi_kubernetes/certificates/v1beta1/CertificateSigningRequestPatch.py
--rw-r--r--   0 runner    (1001) docker     (123)      416 2023-07-21 05:53:03.000000 pulumi_kubernetes-4.1.0a1689918291/pulumi_kubernetes/certificates/v1beta1/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)    23273 2023-07-21 05:53:03.000000 pulumi_kubernetes-4.1.0a1689918291/pulumi_kubernetes/certificates/v1beta1/_inputs.py
--rw-r--r--   0 runner    (1001) docker     (123)    26601 2023-07-21 05:53:03.000000 pulumi_kubernetes-4.1.0a1689918291/pulumi_kubernetes/certificates/v1beta1/outputs.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-21 05:53:04.000000 pulumi_kubernetes-4.1.0a1689918291/pulumi_kubernetes/coordination/
--rw-r--r--   0 runner    (1001) docker     (123)      559 2023-07-21 05:53:03.000000 pulumi_kubernetes-4.1.0a1689918291/pulumi_kubernetes/coordination/__init__.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-21 05:53:04.000000 pulumi_kubernetes-4.1.0a1689918291/pulumi_kubernetes/coordination/v1/
--rw-r--r--   0 runner    (1001) docker     (123)    11052 2023-07-21 05:53:03.000000 pulumi_kubernetes-4.1.0a1689918291/pulumi_kubernetes/coordination/v1/Lease.py
--rw-r--r--   0 runner    (1001) docker     (123)    10706 2023-07-21 05:53:03.000000 pulumi_kubernetes-4.1.0a1689918291/pulumi_kubernetes/coordination/v1/LeaseList.py
--rw-r--r--   0 runner    (1001) docker     (123)    12650 2023-07-21 05:53:03.000000 pulumi_kubernetes-4.1.0a1689918291/pulumi_kubernetes/coordination/v1/LeasePatch.py
--rw-r--r--   0 runner    (1001) docker     (123)      356 2023-07-21 05:53:03.000000 pulumi_kubernetes-4.1.0a1689918291/pulumi_kubernetes/coordination/v1/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)    12162 2023-07-21 05:53:03.000000 pulumi_kubernetes-4.1.0a1689918291/pulumi_kubernetes/coordination/v1/_inputs.py
--rw-r--r--   0 runner    (1001) docker     (123)    12069 2023-07-21 05:53:03.000000 pulumi_kubernetes-4.1.0a1689918291/pulumi_kubernetes/coordination/v1/outputs.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-21 05:53:04.000000 pulumi_kubernetes-4.1.0a1689918291/pulumi_kubernetes/coordination/v1beta1/
--rw-r--r--   0 runner    (1001) docker     (123)    10990 2023-07-21 05:53:03.000000 pulumi_kubernetes-4.1.0a1689918291/pulumi_kubernetes/coordination/v1beta1/Lease.py
--rw-r--r--   0 runner    (1001) docker     (123)    10721 2023-07-21 05:53:03.000000 pulumi_kubernetes-4.1.0a1689918291/pulumi_kubernetes/coordination/v1beta1/LeaseList.py
--rw-r--r--   0 runner    (1001) docker     (123)    12588 2023-07-21 05:53:03.000000 pulumi_kubernetes-4.1.0a1689918291/pulumi_kubernetes/coordination/v1beta1/LeasePatch.py
--rw-r--r--   0 runner    (1001) docker     (123)      356 2023-07-21 05:53:03.000000 pulumi_kubernetes-4.1.0a1689918291/pulumi_kubernetes/coordination/v1beta1/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)    12131 2023-07-21 05:53:03.000000 pulumi_kubernetes-4.1.0a1689918291/pulumi_kubernetes/coordination/v1beta1/_inputs.py
--rw-r--r--   0 runner    (1001) docker     (123)    12038 2023-07-21 05:53:03.000000 pulumi_kubernetes-4.1.0a1689918291/pulumi_kubernetes/coordination/v1beta1/outputs.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-21 05:53:04.000000 pulumi_kubernetes-4.1.0a1689918291/pulumi_kubernetes/core/
--rw-r--r--   0 runner    (1001) docker     (123)      377 2023-07-21 05:53:03.000000 pulumi_kubernetes-4.1.0a1689918291/pulumi_kubernetes/core/__init__.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-21 05:53:04.000000 pulumi_kubernetes-4.1.0a1689918291/pulumi_kubernetes/core/v1/
--rw-r--r--   0 runner    (1001) docker     (123)    10930 2023-07-21 05:53:03.000000 pulumi_kubernetes-4.1.0a1689918291/pulumi_kubernetes/core/v1/Binding.py
--rw-r--r--   0 runner    (1001) docker     (123)    12530 2023-07-21 05:53:03.000000 pulumi_kubernetes-4.1.0a1689918291/pulumi_kubernetes/core/v1/BindingPatch.py
--rw-r--r--   0 runner    (1001) docker     (123)    16018 2023-07-21 05:53:03.000000 pulumi_kubernetes-4.1.0a1689918291/pulumi_kubernetes/core/v1/ConfigMap.py
--rw-r--r--   0 runner    (1001) docker     (123)    10715 2023-07-21 05:53:03.000000 pulumi_kubernetes-4.1.0a1689918291/pulumi_kubernetes/core/v1/ConfigMapList.py
--rw-r--r--   0 runner    (1001) docker     (123)    17591 2023-07-21 05:53:03.000000 pulumi_kubernetes-4.1.0a1689918291/pulumi_kubernetes/core/v1/ConfigMapPatch.py
--rw-r--r--   0 runner    (1001) docker     (123)    13511 2023-07-21 05:53:03.000000 pulumi_kubernetes-4.1.0a1689918291/pulumi_kubernetes/core/v1/Endpoints.py
--rw-r--r--   0 runner    (1001) docker     (123)    10707 2023-07-21 05:53:03.000000 pulumi_kubernetes-4.1.0a1689918291/pulumi_kubernetes/core/v1/EndpointsList.py
--rw-r--r--   0 runner    (1001) docker     (123)    15104 2023-07-21 05:53:03.000000 pulumi_kubernetes-4.1.0a1689918291/pulumi_kubernetes/core/v1/EndpointsPatch.py
--rw-r--r--   0 runner    (1001) docker     (123)    28454 2023-07-21 05:53:03.000000 pulumi_kubernetes-4.1.0a1689918291/pulumi_kubernetes/core/v1/Event.py
--rw-r--r--   0 runner    (1001) docker     (123)    10569 2023-07-21 05:53:03.000000 pulumi_kubernetes-4.1.0a1689918291/pulumi_kubernetes/core/v1/EventList.py
--rw-r--r--   0 runner    (1001) docker     (123)    30221 2023-07-21 05:53:03.000000 pulumi_kubernetes-4.1.0a1689918291/pulumi_kubernetes/core/v1/EventPatch.py
--rw-r--r--   0 runner    (1001) docker     (123)    11110 2023-07-21 05:53:03.000000 pulumi_kubernetes-4.1.0a1689918291/pulumi_kubernetes/core/v1/LimitRange.py
--rw-r--r--   0 runner    (1001) docker     (123)    11190 2023-07-21 05:53:03.000000 pulumi_kubernetes-4.1.0a1689918291/pulumi_kubernetes/core/v1/LimitRangeList.py
--rw-r--r--   0 runner    (1001) docker     (123)    12703 2023-07-21 05:53:03.000000 pulumi_kubernetes-4.1.0a1689918291/pulumi_kubernetes/core/v1/LimitRangePatch.py
--rw-r--r--   0 runner    (1001) docker     (123)    11558 2023-07-21 05:53:03.000000 pulumi_kubernetes-4.1.0a1689918291/pulumi_kubernetes/core/v1/Namespace.py
--rw-r--r--   0 runner    (1001) docker     (123)    11197 2023-07-21 05:53:03.000000 pulumi_kubernetes-4.1.0a1689918291/pulumi_kubernetes/core/v1/NamespaceList.py
--rw-r--r--   0 runner    (1001) docker     (123)    13156 2023-07-21 05:53:03.000000 pulumi_kubernetes-4.1.0a1689918291/pulumi_kubernetes/core/v1/NamespacePatch.py
--rw-r--r--   0 runner    (1001) docker     (123)    11429 2023-07-21 05:53:03.000000 pulumi_kubernetes-4.1.0a1689918291/pulumi_kubernetes/core/v1/Node.py
--rw-r--r--   0 runner    (1001) docker     (123)    10636 2023-07-21 05:53:03.000000 pulumi_kubernetes-4.1.0a1689918291/pulumi_kubernetes/core/v1/NodeList.py
--rw-r--r--   0 runner    (1001) docker     (123)    13027 2023-07-21 05:53:03.000000 pulumi_kubernetes-4.1.0a1689918291/pulumi_kubernetes/core/v1/NodePatch.py
--rw-r--r--   0 runner    (1001) docker     (123)    12176 2023-07-21 05:53:03.000000 pulumi_kubernetes-4.1.0a1689918291/pulumi_kubernetes/core/v1/PersistentVolume.py
--rw-r--r--   0 runner    (1001) docker     (123)    12008 2023-07-21 05:53:03.000000 pulumi_kubernetes-4.1.0a1689918291/pulumi_kubernetes/core/v1/PersistentVolumeClaim.py
--rw-r--r--   0 runner    (1001) docker     (123)    11583 2023-07-21 05:53:03.000000 pulumi_kubernetes-4.1.0a1689918291/pulumi_kubernetes/core/v1/PersistentVolumeClaimList.py
--rw-r--r--   0 runner    (1001) docker     (123)    13642 2023-07-21 05:53:03.000000 pulumi_kubernetes-4.1.0a1689918291/pulumi_kubernetes/core/v1/PersistentVolumeClaimPatch.py
--rw-r--r--   0 runner    (1001) docker     (123)    11312 2023-07-21 05:53:03.000000 pulumi_kubernetes-4.1.0a1689918291/pulumi_kubernetes/core/v1/PersistentVolumeList.py
--rw-r--r--   0 runner    (1001) docker     (123)    13774 2023-07-21 05:53:03.000000 pulumi_kubernetes-4.1.0a1689918291/pulumi_kubernetes/core/v1/PersistentVolumePatch.py
--rw-r--r--   0 runner    (1001) docker     (123)    15709 2023-07-21 05:53:03.000000 pulumi_kubernetes-4.1.0a1689918291/pulumi_kubernetes/core/v1/Pod.py
--rw-r--r--   0 runner    (1001) docker     (123)    10883 2023-07-21 05:53:03.000000 pulumi_kubernetes-4.1.0a1689918291/pulumi_kubernetes/core/v1/PodList.py
--rw-r--r--   0 runner    (1001) docker     (123)    14961 2023-07-21 05:53:03.000000 pulumi_kubernetes-4.1.0a1689918291/pulumi_kubernetes/core/v1/PodPatch.py
--rw-r--r--   0 runner    (1001) docker     (123)    11301 2023-07-21 05:53:03.000000 pulumi_kubernetes-4.1.0a1689918291/pulumi_kubernetes/core/v1/PodTemplate.py
--rw-r--r--   0 runner    (1001) docker     (123)    10783 2023-07-21 05:53:03.000000 pulumi_kubernetes-4.1.0a1689918291/pulumi_kubernetes/core/v1/PodTemplateList.py
--rw-r--r--   0 runner    (1001) docker     (123)    12894 2023-07-21 05:53:03.000000 pulumi_kubernetes-4.1.0a1689918291/pulumi_kubernetes/core/v1/PodTemplatePatch.py
--rw-r--r--   0 runner    (1001) docker     (123)    12742 2023-07-21 05:53:03.000000 pulumi_kubernetes-4.1.0a1689918291/pulumi_kubernetes/core/v1/ReplicationController.py
--rw-r--r--   0 runner    (1001) docker     (123)    11515 2023-07-21 05:53:03.000000 pulumi_kubernetes-4.1.0a1689918291/pulumi_kubernetes/core/v1/ReplicationControllerList.py
--rw-r--r--   0 runner    (1001) docker     (123)    14340 2023-07-21 05:53:03.000000 pulumi_kubernetes-4.1.0a1689918291/pulumi_kubernetes/core/v1/ReplicationControllerPatch.py
--rw-r--r--   0 runner    (1001) docker     (123)    11565 2023-07-21 05:53:03.000000 pulumi_kubernetes-4.1.0a1689918291/pulumi_kubernetes/core/v1/ResourceQuota.py
--rw-r--r--   0 runner    (1001) docker     (123)    11219 2023-07-21 05:53:03.000000 pulumi_kubernetes-4.1.0a1689918291/pulumi_kubernetes/core/v1/ResourceQuotaList.py
--rw-r--r--   0 runner    (1001) docker     (123)    13163 2023-07-21 05:53:03.000000 pulumi_kubernetes-4.1.0a1689918291/pulumi_kubernetes/core/v1/ResourceQuotaPatch.py
--rw-r--r--   0 runner    (1001) docker     (123)    18698 2023-07-21 05:53:03.000000 pulumi_kubernetes-4.1.0a1689918291/pulumi_kubernetes/core/v1/Secret.py
--rw-r--r--   0 runner    (1001) docker     (123)    10950 2023-07-21 05:53:03.000000 pulumi_kubernetes-4.1.0a1689918291/pulumi_kubernetes/core/v1/SecretList.py
--rw-r--r--   0 runner    (1001) docker     (123)    20020 2023-07-21 05:53:03.000000 pulumi_kubernetes-4.1.0a1689918291/pulumi_kubernetes/core/v1/SecretPatch.py
--rw-r--r--   0 runner    (1001) docker     (123)    17132 2023-07-21 05:53:03.000000 pulumi_kubernetes-4.1.0a1689918291/pulumi_kubernetes/core/v1/Service.py
--rw-r--r--   0 runner    (1001) docker     (123)    18490 2023-07-21 05:53:03.000000 pulumi_kubernetes-4.1.0a1689918291/pulumi_kubernetes/core/v1/ServiceAccount.py
--rw-r--r--   0 runner    (1001) docker     (123)    11280 2023-07-21 05:53:03.000000 pulumi_kubernetes-4.1.0a1689918291/pulumi_kubernetes/core/v1/ServiceAccountList.py
--rw-r--r--   0 runner    (1001) docker     (123)    20143 2023-07-21 05:53:03.000000 pulumi_kubernetes-4.1.0a1689918291/pulumi_kubernetes/core/v1/ServiceAccountPatch.py
--rw-r--r--   0 runner    (1001) docker     (123)    10667 2023-07-21 05:53:03.000000 pulumi_kubernetes-4.1.0a1689918291/pulumi_kubernetes/core/v1/ServiceList.py
--rw-r--r--   0 runner    (1001) docker     (123)    16406 2023-07-21 05:53:03.000000 pulumi_kubernetes-4.1.0a1689918291/pulumi_kubernetes/core/v1/ServicePatch.py
--rw-r--r--   0 runner    (1001) docker     (123)     1686 2023-07-21 05:53:03.000000 pulumi_kubernetes-4.1.0a1689918291/pulumi_kubernetes/core/v1/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)      376 2023-07-21 05:53:03.000000 pulumi_kubernetes-4.1.0a1689918291/pulumi_kubernetes/core/v1/_enums.py
--rw-r--r--   0 runner    (1001) docker     (123)  1507480 2023-07-21 05:53:03.000000 pulumi_kubernetes-4.1.0a1689918291/pulumi_kubernetes/core/v1/_inputs.py
--rw-r--r--   0 runner    (1001) docker     (123)  1546761 2023-07-21 05:53:03.000000 pulumi_kubernetes-4.1.0a1689918291/pulumi_kubernetes/core/v1/outputs.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-21 05:53:04.000000 pulumi_kubernetes-4.1.0a1689918291/pulumi_kubernetes/discovery/
--rw-r--r--   0 runner    (1001) docker     (123)      547 2023-07-21 05:53:03.000000 pulumi_kubernetes-4.1.0a1689918291/pulumi_kubernetes/discovery/__init__.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-21 05:53:04.000000 pulumi_kubernetes-4.1.0a1689918291/pulumi_kubernetes/discovery/v1/
--rw-r--r--   0 runner    (1001) docker     (123)    16252 2023-07-21 05:53:03.000000 pulumi_kubernetes-4.1.0a1689918291/pulumi_kubernetes/discovery/v1/EndpointSlice.py
--rw-r--r--   0 runner    (1001) docker     (123)    10569 2023-07-21 05:53:03.000000 pulumi_kubernetes-4.1.0a1689918291/pulumi_kubernetes/discovery/v1/EndpointSliceList.py
--rw-r--r--   0 runner    (1001) docker     (123)    17826 2023-07-21 05:53:03.000000 pulumi_kubernetes-4.1.0a1689918291/pulumi_kubernetes/discovery/v1/EndpointSlicePatch.py
--rw-r--r--   0 runner    (1001) docker     (123)      380 2023-07-21 05:53:03.000000 pulumi_kubernetes-4.1.0a1689918291/pulumi_kubernetes/discovery/v1/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)    42431 2023-07-21 05:53:03.000000 pulumi_kubernetes-4.1.0a1689918291/pulumi_kubernetes/discovery/v1/_inputs.py
--rw-r--r--   0 runner    (1001) docker     (123)    40504 2023-07-21 05:53:03.000000 pulumi_kubernetes-4.1.0a1689918291/pulumi_kubernetes/discovery/v1/outputs.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-21 05:53:04.000000 pulumi_kubernetes-4.1.0a1689918291/pulumi_kubernetes/discovery/v1beta1/
--rw-r--r--   0 runner    (1001) docker     (123)    16262 2023-07-21 05:53:03.000000 pulumi_kubernetes-4.1.0a1689918291/pulumi_kubernetes/discovery/v1beta1/EndpointSlice.py
--rw-r--r--   0 runner    (1001) docker     (123)    10532 2023-07-21 05:53:03.000000 pulumi_kubernetes-4.1.0a1689918291/pulumi_kubernetes/discovery/v1beta1/EndpointSliceList.py
--rw-r--r--   0 runner    (1001) docker     (123)    17836 2023-07-21 05:53:03.000000 pulumi_kubernetes-4.1.0a1689918291/pulumi_kubernetes/discovery/v1beta1/EndpointSlicePatch.py
--rw-r--r--   0 runner    (1001) docker     (123)      380 2023-07-21 05:53:03.000000 pulumi_kubernetes-4.1.0a1689918291/pulumi_kubernetes/discovery/v1beta1/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)    35598 2023-07-21 05:53:03.000000 pulumi_kubernetes-4.1.0a1689918291/pulumi_kubernetes/discovery/v1beta1/_inputs.py
--rw-r--r--   0 runner    (1001) docker     (123)    33494 2023-07-21 05:53:03.000000 pulumi_kubernetes-4.1.0a1689918291/pulumi_kubernetes/discovery/v1beta1/outputs.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-21 05:53:04.000000 pulumi_kubernetes-4.1.0a1689918291/pulumi_kubernetes/events/
--rw-r--r--   0 runner    (1001) docker     (123)      535 2023-07-21 05:53:03.000000 pulumi_kubernetes-4.1.0a1689918291/pulumi_kubernetes/events/__init__.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-21 05:53:04.000000 pulumi_kubernetes-4.1.0a1689918291/pulumi_kubernetes/events/v1/
--rw-r--r--   0 runner    (1001) docker     (123)    33307 2023-07-21 05:53:03.000000 pulumi_kubernetes-4.1.0a1689918291/pulumi_kubernetes/events/v1/Event.py
--rw-r--r--   0 runner    (1001) docker     (123)    10718 2023-07-21 05:53:03.000000 pulumi_kubernetes-4.1.0a1689918291/pulumi_kubernetes/events/v1/EventList.py
--rw-r--r--   0 runner    (1001) docker     (123)    35127 2023-07-21 05:53:03.000000 pulumi_kubernetes-4.1.0a1689918291/pulumi_kubernetes/events/v1/EventPatch.py
--rw-r--r--   0 runner    (1001) docker     (123)      356 2023-07-21 05:53:03.000000 pulumi_kubernetes-4.1.0a1689918291/pulumi_kubernetes/events/v1/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)    19318 2023-07-21 05:53:03.000000 pulumi_kubernetes-4.1.0a1689918291/pulumi_kubernetes/events/v1/_inputs.py
--rw-r--r--   0 runner    (1001) docker     (123)    19050 2023-07-21 05:53:03.000000 pulumi_kubernetes-4.1.0a1689918291/pulumi_kubernetes/events/v1/outputs.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-21 05:53:04.000000 pulumi_kubernetes-4.1.0a1689918291/pulumi_kubernetes/events/v1beta1/
--rw-r--r--   0 runner    (1001) docker     (123)    29243 2023-07-21 05:53:03.000000 pulumi_kubernetes-4.1.0a1689918291/pulumi_kubernetes/events/v1beta1/Event.py
--rw-r--r--   0 runner    (1001) docker     (123)    10733 2023-07-21 05:53:03.000000 pulumi_kubernetes-4.1.0a1689918291/pulumi_kubernetes/events/v1beta1/EventList.py
--rw-r--r--   0 runner    (1001) docker     (123)    31053 2023-07-21 05:53:03.000000 pulumi_kubernetes-4.1.0a1689918291/pulumi_kubernetes/events/v1beta1/EventPatch.py
--rw-r--r--   0 runner    (1001) docker     (123)      356 2023-07-21 05:53:03.000000 pulumi_kubernetes-4.1.0a1689918291/pulumi_kubernetes/events/v1beta1/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)    17860 2023-07-21 05:53:03.000000 pulumi_kubernetes-4.1.0a1689918291/pulumi_kubernetes/events/v1beta1/_inputs.py
--rw-r--r--   0 runner    (1001) docker     (123)    16467 2023-07-21 05:53:03.000000 pulumi_kubernetes-4.1.0a1689918291/pulumi_kubernetes/events/v1beta1/outputs.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-21 05:53:04.000000 pulumi_kubernetes-4.1.0a1689918291/pulumi_kubernetes/extensions/
--rw-r--r--   0 runner    (1001) docker     (123)      419 2023-07-21 05:53:03.000000 pulumi_kubernetes-4.1.0a1689918291/pulumi_kubernetes/extensions/__init__.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-21 05:53:04.000000 pulumi_kubernetes-4.1.0a1689918291/pulumi_kubernetes/extensions/v1beta1/
--rw-r--r--   0 runner    (1001) docker     (123)    11876 2023-07-21 05:53:03.000000 pulumi_kubernetes-4.1.0a1689918291/pulumi_kubernetes/extensions/v1beta1/DaemonSet.py
--rw-r--r--   0 runner    (1001) docker     (123)    10800 2023-07-21 05:53:03.000000 pulumi_kubernetes-4.1.0a1689918291/pulumi_kubernetes/extensions/v1beta1/DaemonSetList.py
--rw-r--r--   0 runner    (1001) docker     (123)    13484 2023-07-21 05:53:03.000000 pulumi_kubernetes-4.1.0a1689918291/pulumi_kubernetes/extensions/v1beta1/DaemonSetPatch.py
--rw-r--r--   0 runner    (1001) docker     (123)    14034 2023-07-21 05:53:03.000000 pulumi_kubernetes-4.1.0a1689918291/pulumi_kubernetes/extensions/v1beta1/Deployment.py
--rw-r--r--   0 runner    (1001) docker     (123)    10445 2023-07-21 05:53:03.000000 pulumi_kubernetes-4.1.0a1689918291/pulumi_kubernetes/extensions/v1beta1/DeploymentList.py
--rw-r--r--   0 runner    (1001) docker     (123)    15647 2023-07-21 05:53:03.000000 pulumi_kubernetes-4.1.0a1689918291/pulumi_kubernetes/extensions/v1beta1/DeploymentPatch.py
--rw-r--r--   0 runner    (1001) docker     (123)    13728 2023-07-21 05:53:03.000000 pulumi_kubernetes-4.1.0a1689918291/pulumi_kubernetes/extensions/v1beta1/Ingress.py
--rw-r--r--   0 runner    (1001) docker     (123)    10778 2023-07-21 05:53:03.000000 pulumi_kubernetes-4.1.0a1689918291/pulumi_kubernetes/extensions/v1beta1/IngressList.py
--rw-r--r--   0 runner    (1001) docker     (123)    15336 2023-07-21 05:53:03.000000 pulumi_kubernetes-4.1.0a1689918291/pulumi_kubernetes/extensions/v1beta1/IngressPatch.py
--rw-r--r--   0 runner    (1001) docker     (123)    11273 2023-07-21 05:53:03.000000 pulumi_kubernetes-4.1.0a1689918291/pulumi_kubernetes/extensions/v1beta1/NetworkPolicy.py
--rw-r--r--   0 runner    (1001) docker     (123)    11160 2023-07-21 05:53:03.000000 pulumi_kubernetes-4.1.0a1689918291/pulumi_kubernetes/extensions/v1beta1/NetworkPolicyList.py
--rw-r--r--   0 runner    (1001) docker     (123)    12871 2023-07-21 05:53:03.000000 pulumi_kubernetes-4.1.0a1689918291/pulumi_kubernetes/extensions/v1beta1/NetworkPolicyPatch.py
--rw-r--r--   0 runner    (1001) docker     (123)    11347 2023-07-21 05:53:03.000000 pulumi_kubernetes-4.1.0a1689918291/pulumi_kubernetes/extensions/v1beta1/PodSecurityPolicy.py
--rw-r--r--   0 runner    (1001) docker     (123)    11234 2023-07-21 05:53:03.000000 pulumi_kubernetes-4.1.0a1689918291/pulumi_kubernetes/extensions/v1beta1/PodSecurityPolicyList.py
--rw-r--r--   0 runner    (1001) docker     (123)    12945 2023-07-21 05:53:03.000000 pulumi_kubernetes-4.1.0a1689918291/pulumi_kubernetes/extensions/v1beta1/PodSecurityPolicyPatch.py
--rw-r--r--   0 runner    (1001) docker     (123)    12602 2023-07-21 05:53:03.000000 pulumi_kubernetes-4.1.0a1689918291/pulumi_kubernetes/extensions/v1beta1/ReplicaSet.py
--rw-r--r--   0 runner    (1001) docker     (123)    11197 2023-07-21 05:53:03.000000 pulumi_kubernetes-4.1.0a1689918291/pulumi_kubernetes/extensions/v1beta1/ReplicaSetList.py
--rw-r--r--   0 runner    (1001) docker     (123)    14210 2023-07-21 05:53:03.000000 pulumi_kubernetes-4.1.0a1689918291/pulumi_kubernetes/extensions/v1beta1/ReplicaSetPatch.py
--rw-r--r--   0 runner    (1001) docker     (123)      824 2023-07-21 05:53:03.000000 pulumi_kubernetes-4.1.0a1689918291/pulumi_kubernetes/extensions/v1beta1/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)   288488 2023-07-21 05:53:03.000000 pulumi_kubernetes-4.1.0a1689918291/pulumi_kubernetes/extensions/v1beta1/_inputs.py
--rw-r--r--   0 runner    (1001) docker     (123)   316040 2023-07-21 05:53:03.000000 pulumi_kubernetes-4.1.0a1689918291/pulumi_kubernetes/extensions/v1beta1/outputs.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-21 05:53:04.000000 pulumi_kubernetes-4.1.0a1689918291/pulumi_kubernetes/flowcontrol/
--rw-r--r--   0 runner    (1001) docker     (123)      919 2023-07-21 05:53:03.000000 pulumi_kubernetes-4.1.0a1689918291/pulumi_kubernetes/flowcontrol/__init__.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-21 05:53:04.000000 pulumi_kubernetes-4.1.0a1689918291/pulumi_kubernetes/flowcontrol/v1alpha1/
--rw-r--r--   0 runner    (1001) docker     (123)    12522 2023-07-21 05:53:03.000000 pulumi_kubernetes-4.1.0a1689918291/pulumi_kubernetes/flowcontrol/v1alpha1/FlowSchema.py
--rw-r--r--   0 runner    (1001) docker     (123)    10974 2023-07-21 05:53:03.000000 pulumi_kubernetes-4.1.0a1689918291/pulumi_kubernetes/flowcontrol/v1alpha1/FlowSchemaList.py
--rw-r--r--   0 runner    (1001) docker     (123)    14135 2023-07-21 05:53:03.000000 pulumi_kubernetes-4.1.0a1689918291/pulumi_kubernetes/flowcontrol/v1alpha1/FlowSchemaPatch.py
--rw-r--r--   0 runner    (1001) docker     (123)    12750 2023-07-21 05:53:03.000000 pulumi_kubernetes-4.1.0a1689918291/pulumi_kubernetes/flowcontrol/v1alpha1/PriorityLevelConfiguration.py
--rw-r--r--   0 runner    (1001) docker     (123)    11514 2023-07-21 05:53:03.000000 pulumi_kubernetes-4.1.0a1689918291/pulumi_kubernetes/flowcontrol/v1alpha1/PriorityLevelConfigurationList.py
--rw-r--r--   0 runner    (1001) docker     (123)    14363 2023-07-21 05:53:03.000000 pulumi_kubernetes-4.1.0a1689918291/pulumi_kubernetes/flowcontrol/v1alpha1/PriorityLevelConfigurationPatch.py
--rw-r--r--   0 runner    (1001) docker     (123)      506 2023-07-21 05:53:03.000000 pulumi_kubernetes-4.1.0a1689918291/pulumi_kubernetes/flowcontrol/v1alpha1/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)    93706 2023-07-21 05:53:03.000000 pulumi_kubernetes-4.1.0a1689918291/pulumi_kubernetes/flowcontrol/v1alpha1/_inputs.py
--rw-r--r--   0 runner    (1001) docker     (123)   102811 2023-07-21 05:53:03.000000 pulumi_kubernetes-4.1.0a1689918291/pulumi_kubernetes/flowcontrol/v1alpha1/outputs.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-21 05:53:04.000000 pulumi_kubernetes-4.1.0a1689918291/pulumi_kubernetes/flowcontrol/v1beta1/
--rw-r--r--   0 runner    (1001) docker     (123)    12520 2023-07-21 05:53:03.000000 pulumi_kubernetes-4.1.0a1689918291/pulumi_kubernetes/flowcontrol/v1beta1/FlowSchema.py
--rw-r--r--   0 runner    (1001) docker     (123)    10971 2023-07-21 05:53:03.000000 pulumi_kubernetes-4.1.0a1689918291/pulumi_kubernetes/flowcontrol/v1beta1/FlowSchemaList.py
--rw-r--r--   0 runner    (1001) docker     (123)    14133 2023-07-21 05:53:03.000000 pulumi_kubernetes-4.1.0a1689918291/pulumi_kubernetes/flowcontrol/v1beta1/FlowSchemaPatch.py
--rw-r--r--   0 runner    (1001) docker     (123)    12748 2023-07-21 05:53:03.000000 pulumi_kubernetes-4.1.0a1689918291/pulumi_kubernetes/flowcontrol/v1beta1/PriorityLevelConfiguration.py
--rw-r--r--   0 runner    (1001) docker     (123)    11511 2023-07-21 05:53:03.000000 pulumi_kubernetes-4.1.0a1689918291/pulumi_kubernetes/flowcontrol/v1beta1/PriorityLevelConfigurationList.py
--rw-r--r--   0 runner    (1001) docker     (123)    14361 2023-07-21 05:53:03.000000 pulumi_kubernetes-4.1.0a1689918291/pulumi_kubernetes/flowcontrol/v1beta1/PriorityLevelConfigurationPatch.py
--rw-r--r--   0 runner    (1001) docker     (123)      506 2023-07-21 05:53:03.000000 pulumi_kubernetes-4.1.0a1689918291/pulumi_kubernetes/flowcontrol/v1beta1/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)    93700 2023-07-21 05:53:03.000000 pulumi_kubernetes-4.1.0a1689918291/pulumi_kubernetes/flowcontrol/v1beta1/_inputs.py
--rw-r--r--   0 runner    (1001) docker     (123)   102805 2023-07-21 05:53:03.000000 pulumi_kubernetes-4.1.0a1689918291/pulumi_kubernetes/flowcontrol/v1beta1/outputs.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-21 05:53:04.000000 pulumi_kubernetes-4.1.0a1689918291/pulumi_kubernetes/flowcontrol/v1beta2/
--rw-r--r--   0 runner    (1001) docker     (123)    12520 2023-07-21 05:53:03.000000 pulumi_kubernetes-4.1.0a1689918291/pulumi_kubernetes/flowcontrol/v1beta2/FlowSchema.py
--rw-r--r--   0 runner    (1001) docker     (123)    10971 2023-07-21 05:53:03.000000 pulumi_kubernetes-4.1.0a1689918291/pulumi_kubernetes/flowcontrol/v1beta2/FlowSchemaList.py
--rw-r--r--   0 runner    (1001) docker     (123)    14133 2023-07-21 05:53:03.000000 pulumi_kubernetes-4.1.0a1689918291/pulumi_kubernetes/flowcontrol/v1beta2/FlowSchemaPatch.py
--rw-r--r--   0 runner    (1001) docker     (123)    12748 2023-07-21 05:53:03.000000 pulumi_kubernetes-4.1.0a1689918291/pulumi_kubernetes/flowcontrol/v1beta2/PriorityLevelConfiguration.py
--rw-r--r--   0 runner    (1001) docker     (123)    11511 2023-07-21 05:53:03.000000 pulumi_kubernetes-4.1.0a1689918291/pulumi_kubernetes/flowcontrol/v1beta2/PriorityLevelConfigurationList.py
--rw-r--r--   0 runner    (1001) docker     (123)    14361 2023-07-21 05:53:03.000000 pulumi_kubernetes-4.1.0a1689918291/pulumi_kubernetes/flowcontrol/v1beta2/PriorityLevelConfigurationPatch.py
--rw-r--r--   0 runner    (1001) docker     (123)      506 2023-07-21 05:53:03.000000 pulumi_kubernetes-4.1.0a1689918291/pulumi_kubernetes/flowcontrol/v1beta2/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)   102903 2023-07-21 05:53:03.000000 pulumi_kubernetes-4.1.0a1689918291/pulumi_kubernetes/flowcontrol/v1beta2/_inputs.py
--rw-r--r--   0 runner    (1001) docker     (123)   111784 2023-07-21 05:53:03.000000 pulumi_kubernetes-4.1.0a1689918291/pulumi_kubernetes/flowcontrol/v1beta2/outputs.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-21 05:53:04.000000 pulumi_kubernetes-4.1.0a1689918291/pulumi_kubernetes/flowcontrol/v1beta3/
--rw-r--r--   0 runner    (1001) docker     (123)    12520 2023-07-21 05:53:03.000000 pulumi_kubernetes-4.1.0a1689918291/pulumi_kubernetes/flowcontrol/v1beta3/FlowSchema.py
--rw-r--r--   0 runner    (1001) docker     (123)    10971 2023-07-21 05:53:03.000000 pulumi_kubernetes-4.1.0a1689918291/pulumi_kubernetes/flowcontrol/v1beta3/FlowSchemaList.py
--rw-r--r--   0 runner    (1001) docker     (123)    14133 2023-07-21 05:53:03.000000 pulumi_kubernetes-4.1.0a1689918291/pulumi_kubernetes/flowcontrol/v1beta3/FlowSchemaPatch.py
--rw-r--r--   0 runner    (1001) docker     (123)    12748 2023-07-21 05:53:03.000000 pulumi_kubernetes-4.1.0a1689918291/pulumi_kubernetes/flowcontrol/v1beta3/PriorityLevelConfiguration.py
--rw-r--r--   0 runner    (1001) docker     (123)    11511 2023-07-21 05:53:03.000000 pulumi_kubernetes-4.1.0a1689918291/pulumi_kubernetes/flowcontrol/v1beta3/PriorityLevelConfigurationList.py
--rw-r--r--   0 runner    (1001) docker     (123)    14361 2023-07-21 05:53:03.000000 pulumi_kubernetes-4.1.0a1689918291/pulumi_kubernetes/flowcontrol/v1beta3/PriorityLevelConfigurationPatch.py
--rw-r--r--   0 runner    (1001) docker     (123)      506 2023-07-21 05:53:03.000000 pulumi_kubernetes-4.1.0a1689918291/pulumi_kubernetes/flowcontrol/v1beta3/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)   102963 2023-07-21 05:53:03.000000 pulumi_kubernetes-4.1.0a1689918291/pulumi_kubernetes/flowcontrol/v1beta3/_inputs.py
--rw-r--r--   0 runner    (1001) docker     (123)   111844 2023-07-21 05:53:03.000000 pulumi_kubernetes-4.1.0a1689918291/pulumi_kubernetes/flowcontrol/v1beta3/outputs.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-21 05:53:04.000000 pulumi_kubernetes-4.1.0a1689918291/pulumi_kubernetes/helm/
--rw-r--r--   0 runner    (1001) docker     (123)      377 2023-07-21 05:53:03.000000 pulumi_kubernetes-4.1.0a1689918291/pulumi_kubernetes/helm/__init__.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-21 05:53:04.000000 pulumi_kubernetes-4.1.0a1689918291/pulumi_kubernetes/helm/v3/
--rw-r--r--   0 runner    (1001) docker     (123)    60748 2023-07-21 05:53:03.000000 pulumi_kubernetes-4.1.0a1689918291/pulumi_kubernetes/helm/v3/Release.py
--rw-r--r--   0 runner    (1001) docker     (123)      327 2023-07-21 05:53:03.000000 pulumi_kubernetes-4.1.0a1689918291/pulumi_kubernetes/helm/v3/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)     3999 2023-07-21 05:53:03.000000 pulumi_kubernetes-4.1.0a1689918291/pulumi_kubernetes/helm/v3/_inputs.py
--rw-r--r--   0 runner    (1001) docker     (123)    26887 2023-07-21 05:53:03.000000 pulumi_kubernetes-4.1.0a1689918291/pulumi_kubernetes/helm/v3/helm.py
--rw-r--r--   0 runner    (1001) docker     (123)     7187 2023-07-21 05:53:03.000000 pulumi_kubernetes-4.1.0a1689918291/pulumi_kubernetes/helm/v3/outputs.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-21 05:53:04.000000 pulumi_kubernetes-4.1.0a1689918291/pulumi_kubernetes/kustomize/
--rw-r--r--   0 runner    (1001) docker     (123)      263 2023-07-21 05:53:03.000000 pulumi_kubernetes-4.1.0a1689918291/pulumi_kubernetes/kustomize/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)     6818 2023-07-21 05:53:03.000000 pulumi_kubernetes-4.1.0a1689918291/pulumi_kubernetes/kustomize/kustomize.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-21 05:53:04.000000 pulumi_kubernetes-4.1.0a1689918291/pulumi_kubernetes/meta/
--rw-r--r--   0 runner    (1001) docker     (123)      377 2023-07-21 05:53:03.000000 pulumi_kubernetes-4.1.0a1689918291/pulumi_kubernetes/meta/__init__.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-21 05:53:04.000000 pulumi_kubernetes-4.1.0a1689918291/pulumi_kubernetes/meta/v1/
--rw-r--r--   0 runner    (1001) docker     (123)    15520 2023-07-21 05:53:03.000000 pulumi_kubernetes-4.1.0a1689918291/pulumi_kubernetes/meta/v1/Status.py
--rw-r--r--   0 runner    (1001) docker     (123)    17179 2023-07-21 05:53:03.000000 pulumi_kubernetes-4.1.0a1689918291/pulumi_kubernetes/meta/v1/StatusPatch.py
--rw-r--r--   0 runner    (1001) docker     (123)      333 2023-07-21 05:53:03.000000 pulumi_kubernetes-4.1.0a1689918291/pulumi_kubernetes/meta/v1/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)   115603 2023-07-21 05:53:03.000000 pulumi_kubernetes-4.1.0a1689918291/pulumi_kubernetes/meta/v1/_inputs.py
--rw-r--r--   0 runner    (1001) docker     (123)   115305 2023-07-21 05:53:03.000000 pulumi_kubernetes-4.1.0a1689918291/pulumi_kubernetes/meta/v1/outputs.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-21 05:53:04.000000 pulumi_kubernetes-4.1.0a1689918291/pulumi_kubernetes/networking/
--rw-r--r--   0 runner    (1001) docker     (123)      719 2023-07-21 05:53:03.000000 pulumi_kubernetes-4.1.0a1689918291/pulumi_kubernetes/networking/__init__.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-21 05:53:04.000000 pulumi_kubernetes-4.1.0a1689918291/pulumi_kubernetes/networking/v1/
--rw-r--r--   0 runner    (1001) docker     (123)    19184 2023-07-21 05:53:03.000000 pulumi_kubernetes-4.1.0a1689918291/pulumi_kubernetes/networking/v1/Ingress.py
--rw-r--r--   0 runner    (1001) docker     (123)    12038 2023-07-21 05:53:03.000000 pulumi_kubernetes-4.1.0a1689918291/pulumi_kubernetes/networking/v1/IngressClass.py
--rw-r--r--   0 runner    (1001) docker     (123)    10509 2023-07-21 05:53:03.000000 pulumi_kubernetes-4.1.0a1689918291/pulumi_kubernetes/networking/v1/IngressClassList.py
--rw-r--r--   0 runner    (1001) docker     (123)    13636 2023-07-21 05:53:03.000000 pulumi_kubernetes-4.1.0a1689918291/pulumi_kubernetes/networking/v1/IngressClassPatch.py
--rw-r--r--   0 runner    (1001) docker     (123)    10784 2023-07-21 05:53:03.000000 pulumi_kubernetes-4.1.0a1689918291/pulumi_kubernetes/networking/v1/IngressList.py
--rw-r--r--   0 runner    (1001) docker     (123)    15340 2023-07-21 05:53:03.000000 pulumi_kubernetes-4.1.0a1689918291/pulumi_kubernetes/networking/v1/IngressPatch.py
--rw-r--r--   0 runner    (1001) docker     (123)    11608 2023-07-21 05:53:03.000000 pulumi_kubernetes-4.1.0a1689918291/pulumi_kubernetes/networking/v1/NetworkPolicy.py
--rw-r--r--   0 runner    (1001) docker     (123)    10948 2023-07-21 05:53:03.000000 pulumi_kubernetes-4.1.0a1689918291/pulumi_kubernetes/networking/v1/NetworkPolicyList.py
--rw-r--r--   0 runner    (1001) docker     (123)    13211 2023-07-21 05:53:03.000000 pulumi_kubernetes-4.1.0a1689918291/pulumi_kubernetes/networking/v1/NetworkPolicyPatch.py
--rw-r--r--   0 runner    (1001) docker     (123)      551 2023-07-21 05:53:03.000000 pulumi_kubernetes-4.1.0a1689918291/pulumi_kubernetes/networking/v1/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)   126779 2023-07-21 05:53:03.000000 pulumi_kubernetes-4.1.0a1689918291/pulumi_kubernetes/networking/v1/_inputs.py
--rw-r--r--   0 runner    (1001) docker     (123)   133959 2023-07-21 05:53:03.000000 pulumi_kubernetes-4.1.0a1689918291/pulumi_kubernetes/networking/v1/outputs.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-21 05:53:04.000000 pulumi_kubernetes-4.1.0a1689918291/pulumi_kubernetes/networking/v1alpha1/
--rw-r--r--   0 runner    (1001) docker     (123)    12370 2023-07-21 05:53:03.000000 pulumi_kubernetes-4.1.0a1689918291/pulumi_kubernetes/networking/v1alpha1/ClusterCIDR.py
--rw-r--r--   0 runner    (1001) docker     (123)    10946 2023-07-21 05:53:03.000000 pulumi_kubernetes-4.1.0a1689918291/pulumi_kubernetes/networking/v1alpha1/ClusterCIDRList.py
--rw-r--r--   0 runner    (1001) docker     (123)    13963 2023-07-21 05:53:03.000000 pulumi_kubernetes-4.1.0a1689918291/pulumi_kubernetes/networking/v1alpha1/ClusterCIDRPatch.py
--rw-r--r--   0 runner    (1001) docker     (123)    12226 2023-07-21 05:53:03.000000 pulumi_kubernetes-4.1.0a1689918291/pulumi_kubernetes/networking/v1alpha1/IPAddress.py
--rw-r--r--   0 runner    (1001) docker     (123)    10850 2023-07-21 05:53:03.000000 pulumi_kubernetes-4.1.0a1689918291/pulumi_kubernetes/networking/v1alpha1/IPAddressList.py
--rw-r--r--   0 runner    (1001) docker     (123)    13819 2023-07-21 05:53:03.000000 pulumi_kubernetes-4.1.0a1689918291/pulumi_kubernetes/networking/v1alpha1/IPAddressPatch.py
--rw-r--r--   0 runner    (1001) docker     (123)      458 2023-07-21 05:53:03.000000 pulumi_kubernetes-4.1.0a1689918291/pulumi_kubernetes/networking/v1alpha1/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)    25728 2023-07-21 05:53:03.000000 pulumi_kubernetes-4.1.0a1689918291/pulumi_kubernetes/networking/v1alpha1/_inputs.py
--rw-r--r--   0 runner    (1001) docker     (123)    26254 2023-07-21 05:53:03.000000 pulumi_kubernetes-4.1.0a1689918291/pulumi_kubernetes/networking/v1alpha1/outputs.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-21 05:53:04.000000 pulumi_kubernetes-4.1.0a1689918291/pulumi_kubernetes/networking/v1beta1/
--rw-r--r--   0 runner    (1001) docker     (123)    13742 2023-07-21 05:53:03.000000 pulumi_kubernetes-4.1.0a1689918291/pulumi_kubernetes/networking/v1beta1/Ingress.py
--rw-r--r--   0 runner    (1001) docker     (123)    12078 2023-07-21 05:53:03.000000 pulumi_kubernetes-4.1.0a1689918291/pulumi_kubernetes/networking/v1beta1/IngressClass.py
--rw-r--r--   0 runner    (1001) docker     (123)    10554 2023-07-21 05:53:03.000000 pulumi_kubernetes-4.1.0a1689918291/pulumi_kubernetes/networking/v1beta1/IngressClassList.py
--rw-r--r--   0 runner    (1001) docker     (123)    13676 2023-07-21 05:53:03.000000 pulumi_kubernetes-4.1.0a1689918291/pulumi_kubernetes/networking/v1beta1/IngressClassPatch.py
--rw-r--r--   0 runner    (1001) docker     (123)    10799 2023-07-21 05:53:03.000000 pulumi_kubernetes-4.1.0a1689918291/pulumi_kubernetes/networking/v1beta1/IngressList.py
--rw-r--r--   0 runner    (1001) docker     (123)    15350 2023-07-21 05:53:03.000000 pulumi_kubernetes-4.1.0a1689918291/pulumi_kubernetes/networking/v1beta1/IngressPatch.py
--rw-r--r--   0 runner    (1001) docker     (123)      455 2023-07-21 05:53:03.000000 pulumi_kubernetes-4.1.0a1689918291/pulumi_kubernetes/networking/v1beta1/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)    54059 2023-07-21 05:53:03.000000 pulumi_kubernetes-4.1.0a1689918291/pulumi_kubernetes/networking/v1beta1/_inputs.py
--rw-r--r--   0 runner    (1001) docker     (123)    57257 2023-07-21 05:53:03.000000 pulumi_kubernetes-4.1.0a1689918291/pulumi_kubernetes/networking/v1beta1/outputs.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-21 05:53:04.000000 pulumi_kubernetes-4.1.0a1689918291/pulumi_kubernetes/node/
--rw-r--r--   0 runner    (1001) docker     (123)      683 2023-07-21 05:53:03.000000 pulumi_kubernetes-4.1.0a1689918291/pulumi_kubernetes/node/__init__.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-21 05:53:04.000000 pulumi_kubernetes-4.1.0a1689918291/pulumi_kubernetes/node/v1/
--rw-r--r--   0 runner    (1001) docker     (123)    17524 2023-07-21 05:53:03.000000 pulumi_kubernetes-4.1.0a1689918291/pulumi_kubernetes/node/v1/RuntimeClass.py
--rw-r--r--   0 runner    (1001) docker     (123)    10929 2023-07-21 05:53:03.000000 pulumi_kubernetes-4.1.0a1689918291/pulumi_kubernetes/node/v1/RuntimeClassList.py
--rw-r--r--   0 runner    (1001) docker     (123)    19157 2023-07-21 05:53:03.000000 pulumi_kubernetes-4.1.0a1689918291/pulumi_kubernetes/node/v1/RuntimeClassPatch.py
--rw-r--r--   0 runner    (1001) docker     (123)      377 2023-07-21 05:53:03.000000 pulumi_kubernetes-4.1.0a1689918291/pulumi_kubernetes/node/v1/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)    14552 2023-07-21 05:53:03.000000 pulumi_kubernetes-4.1.0a1689918291/pulumi_kubernetes/node/v1/_inputs.py
--rw-r--r--   0 runner    (1001) docker     (123)    15712 2023-07-21 05:53:03.000000 pulumi_kubernetes-4.1.0a1689918291/pulumi_kubernetes/node/v1/outputs.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-21 05:53:04.000000 pulumi_kubernetes-4.1.0a1689918291/pulumi_kubernetes/node/v1alpha1/
--rw-r--r--   0 runner    (1001) docker     (123)    12189 2023-07-21 05:53:03.000000 pulumi_kubernetes-4.1.0a1689918291/pulumi_kubernetes/node/v1alpha1/RuntimeClass.py
--rw-r--r--   0 runner    (1001) docker     (123)    10947 2023-07-21 05:53:03.000000 pulumi_kubernetes-4.1.0a1689918291/pulumi_kubernetes/node/v1alpha1/RuntimeClassList.py
--rw-r--r--   0 runner    (1001) docker     (123)    13765 2023-07-21 05:53:03.000000 pulumi_kubernetes-4.1.0a1689918291/pulumi_kubernetes/node/v1alpha1/RuntimeClassPatch.py
--rw-r--r--   0 runner    (1001) docker     (123)      377 2023-07-21 05:53:03.000000 pulumi_kubernetes-4.1.0a1689918291/pulumi_kubernetes/node/v1alpha1/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)    20390 2023-07-21 05:53:03.000000 pulumi_kubernetes-4.1.0a1689918291/pulumi_kubernetes/node/v1alpha1/_inputs.py
--rw-r--r--   0 runner    (1001) docker     (123)    22634 2023-07-21 05:53:03.000000 pulumi_kubernetes-4.1.0a1689918291/pulumi_kubernetes/node/v1alpha1/outputs.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-21 05:53:04.000000 pulumi_kubernetes-4.1.0a1689918291/pulumi_kubernetes/node/v1beta1/
--rw-r--r--   0 runner    (1001) docker     (123)    17930 2023-07-21 05:53:03.000000 pulumi_kubernetes-4.1.0a1689918291/pulumi_kubernetes/node/v1beta1/RuntimeClass.py
--rw-r--r--   0 runner    (1001) docker     (123)    10944 2023-07-21 05:53:03.000000 pulumi_kubernetes-4.1.0a1689918291/pulumi_kubernetes/node/v1beta1/RuntimeClassList.py
--rw-r--r--   0 runner    (1001) docker     (123)    19563 2023-07-21 05:53:03.000000 pulumi_kubernetes-4.1.0a1689918291/pulumi_kubernetes/node/v1beta1/RuntimeClassPatch.py
--rw-r--r--   0 runner    (1001) docker     (123)      377 2023-07-21 05:53:03.000000 pulumi_kubernetes-4.1.0a1689918291/pulumi_kubernetes/node/v1beta1/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)    14755 2023-07-21 05:53:03.000000 pulumi_kubernetes-4.1.0a1689918291/pulumi_kubernetes/node/v1beta1/_inputs.py
--rw-r--r--   0 runner    (1001) docker     (123)    15928 2023-07-21 05:53:03.000000 pulumi_kubernetes-4.1.0a1689918291/pulumi_kubernetes/node/v1beta1/outputs.py
--rw-r--r--   0 runner    (1001) docker     (123)     1685 2023-07-21 05:53:03.000000 pulumi_kubernetes-4.1.0a1689918291/pulumi_kubernetes/outputs.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-21 05:53:04.000000 pulumi_kubernetes-4.1.0a1689918291/pulumi_kubernetes/policy/
--rw-r--r--   0 runner    (1001) docker     (123)      535 2023-07-21 05:53:03.000000 pulumi_kubernetes-4.1.0a1689918291/pulumi_kubernetes/policy/__init__.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-21 05:53:04.000000 pulumi_kubernetes-4.1.0a1689918291/pulumi_kubernetes/policy/v1/
--rw-r--r--   0 runner    (1001) docker     (123)    11632 2023-07-21 05:53:03.000000 pulumi_kubernetes-4.1.0a1689918291/pulumi_kubernetes/policy/v1/PodDisruptionBudget.py
--rw-r--r--   0 runner    (1001) docker     (123)    11135 2023-07-21 05:53:03.000000 pulumi_kubernetes-4.1.0a1689918291/pulumi_kubernetes/policy/v1/PodDisruptionBudgetList.py
--rw-r--r--   0 runner    (1001) docker     (123)    13235 2023-07-21 05:53:03.000000 pulumi_kubernetes-4.1.0a1689918291/pulumi_kubernetes/policy/v1/PodDisruptionBudgetPatch.py
--rw-r--r--   0 runner    (1001) docker     (123)      398 2023-07-21 05:53:03.000000 pulumi_kubernetes-4.1.0a1689918291/pulumi_kubernetes/policy/v1/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)    27765 2023-07-21 05:53:03.000000 pulumi_kubernetes-4.1.0a1689918291/pulumi_kubernetes/policy/v1/_inputs.py
--rw-r--r--   0 runner    (1001) docker     (123)    36012 2023-07-21 05:53:03.000000 pulumi_kubernetes-4.1.0a1689918291/pulumi_kubernetes/policy/v1/outputs.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-21 05:53:04.000000 pulumi_kubernetes-4.1.0a1689918291/pulumi_kubernetes/policy/v1beta1/
--rw-r--r--   0 runner    (1001) docker     (123)    10902 2023-07-21 05:53:03.000000 pulumi_kubernetes-4.1.0a1689918291/pulumi_kubernetes/policy/v1beta1/PodDisruptionBudget.py
--rw-r--r--   0 runner    (1001) docker     (123)    10000 2023-07-21 05:53:03.000000 pulumi_kubernetes-4.1.0a1689918291/pulumi_kubernetes/policy/v1beta1/PodDisruptionBudgetList.py
--rw-r--r--   0 runner    (1001) docker     (123)    12495 2023-07-21 05:53:03.000000 pulumi_kubernetes-4.1.0a1689918291/pulumi_kubernetes/policy/v1beta1/PodDisruptionBudgetPatch.py
--rw-r--r--   0 runner    (1001) docker     (123)    11209 2023-07-21 05:53:03.000000 pulumi_kubernetes-4.1.0a1689918291/pulumi_kubernetes/policy/v1beta1/PodSecurityPolicy.py
--rw-r--r--   0 runner    (1001) docker     (123)    11084 2023-07-21 05:53:03.000000 pulumi_kubernetes-4.1.0a1689918291/pulumi_kubernetes/policy/v1beta1/PodSecurityPolicyList.py
--rw-r--r--   0 runner    (1001) docker     (123)    12807 2023-07-21 05:53:03.000000 pulumi_kubernetes-4.1.0a1689918291/pulumi_kubernetes/policy/v1beta1/PodSecurityPolicyPatch.py
--rw-r--r--   0 runner    (1001) docker     (123)      506 2023-07-21 05:53:03.000000 pulumi_kubernetes-4.1.0a1689918291/pulumi_kubernetes/policy/v1beta1/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)   106813 2023-07-21 05:53:03.000000 pulumi_kubernetes-4.1.0a1689918291/pulumi_kubernetes/policy/v1beta1/_inputs.py
--rw-r--r--   0 runner    (1001) docker     (123)   106119 2023-07-21 05:53:03.000000 pulumi_kubernetes-4.1.0a1689918291/pulumi_kubernetes/policy/v1beta1/outputs.py
--rw-r--r--   0 runner    (1001) docker     (123)    22916 2023-07-21 05:53:03.000000 pulumi_kubernetes-4.1.0a1689918291/pulumi_kubernetes/provider.py
--rw-r--r--   0 runner    (1001) docker     (123)       47 2023-07-21 05:53:03.000000 pulumi_kubernetes-4.1.0a1689918291/pulumi_kubernetes/pulumi-plugin.json
--rw-r--r--   0 runner    (1001) docker     (123)        0 2023-07-21 05:53:03.000000 pulumi_kubernetes-4.1.0a1689918291/pulumi_kubernetes/py.typed
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-21 05:53:04.000000 pulumi_kubernetes-4.1.0a1689918291/pulumi_kubernetes/rbac/
--rw-r--r--   0 runner    (1001) docker     (123)      683 2023-07-21 05:53:03.000000 pulumi_kubernetes-4.1.0a1689918291/pulumi_kubernetes/rbac/__init__.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-21 05:53:04.000000 pulumi_kubernetes-4.1.0a1689918291/pulumi_kubernetes/rbac/v1/
--rw-r--r--   0 runner    (1001) docker     (123)    13177 2023-07-21 05:53:03.000000 pulumi_kubernetes-4.1.0a1689918291/pulumi_kubernetes/rbac/v1/ClusterRole.py
--rw-r--r--   0 runner    (1001) docker     (123)    12895 2023-07-21 05:53:03.000000 pulumi_kubernetes-4.1.0a1689918291/pulumi_kubernetes/rbac/v1/ClusterRoleBinding.py
--rw-r--r--   0 runner    (1001) docker     (123)    10739 2023-07-21 05:53:03.000000 pulumi_kubernetes-4.1.0a1689918291/pulumi_kubernetes/rbac/v1/ClusterRoleBindingList.py
--rw-r--r--   0 runner    (1001) docker     (123)    14517 2023-07-21 05:53:03.000000 pulumi_kubernetes-4.1.0a1689918291/pulumi_kubernetes/rbac/v1/ClusterRoleBindingPatch.py
--rw-r--r--   0 runner    (1001) docker     (123)    10494 2023-07-21 05:53:03.000000 pulumi_kubernetes-4.1.0a1689918291/pulumi_kubernetes/rbac/v1/ClusterRoleList.py
--rw-r--r--   0 runner    (1001) docker     (123)    14830 2023-07-21 05:53:03.000000 pulumi_kubernetes-4.1.0a1689918291/pulumi_kubernetes/rbac/v1/ClusterRolePatch.py
--rw-r--r--   0 runner    (1001) docker     (123)    10734 2023-07-21 05:53:03.000000 pulumi_kubernetes-4.1.0a1689918291/pulumi_kubernetes/rbac/v1/Role.py
--rw-r--r--   0 runner    (1001) docker     (123)    13172 2023-07-21 05:53:03.000000 pulumi_kubernetes-4.1.0a1689918291/pulumi_kubernetes/rbac/v1/RoleBinding.py
--rw-r--r--   0 runner    (1001) docker     (123)    10494 2023-07-21 05:53:03.000000 pulumi_kubernetes-4.1.0a1689918291/pulumi_kubernetes/rbac/v1/RoleBindingList.py
--rw-r--r--   0 runner    (1001) docker     (123)    14794 2023-07-21 05:53:03.000000 pulumi_kubernetes-4.1.0a1689918291/pulumi_kubernetes/rbac/v1/RoleBindingPatch.py
--rw-r--r--   0 runner    (1001) docker     (123)    10249 2023-07-21 05:53:03.000000 pulumi_kubernetes-4.1.0a1689918291/pulumi_kubernetes/rbac/v1/RoleList.py
--rw-r--r--   0 runner    (1001) docker     (123)    12337 2023-07-21 05:53:03.000000 pulumi_kubernetes-4.1.0a1689918291/pulumi_kubernetes/rbac/v1/RolePatch.py
--rw-r--r--   0 runner    (1001) docker     (123)      644 2023-07-21 05:53:03.000000 pulumi_kubernetes-4.1.0a1689918291/pulumi_kubernetes/rbac/v1/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)    42139 2023-07-21 05:53:03.000000 pulumi_kubernetes-4.1.0a1689918291/pulumi_kubernetes/rbac/v1/_inputs.py
--rw-r--r--   0 runner    (1001) docker     (123)    42588 2023-07-21 05:53:03.000000 pulumi_kubernetes-4.1.0a1689918291/pulumi_kubernetes/rbac/v1/outputs.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-21 05:53:04.000000 pulumi_kubernetes-4.1.0a1689918291/pulumi_kubernetes/rbac/v1alpha1/
--rw-r--r--   0 runner    (1001) docker     (123)    13415 2023-07-21 05:53:03.000000 pulumi_kubernetes-4.1.0a1689918291/pulumi_kubernetes/rbac/v1alpha1/ClusterRole.py
--rw-r--r--   0 runner    (1001) docker     (123)    13147 2023-07-21 05:53:03.000000 pulumi_kubernetes-4.1.0a1689918291/pulumi_kubernetes/rbac/v1alpha1/ClusterRoleBinding.py
--rw-r--r--   0 runner    (1001) docker     (123)    11001 2023-07-21 05:53:03.000000 pulumi_kubernetes-4.1.0a1689918291/pulumi_kubernetes/rbac/v1alpha1/ClusterRoleBindingList.py
--rw-r--r--   0 runner    (1001) docker     (123)    14769 2023-07-21 05:53:03.000000 pulumi_kubernetes-4.1.0a1689918291/pulumi_kubernetes/rbac/v1alpha1/ClusterRoleBindingPatch.py
--rw-r--r--   0 runner    (1001) docker     (123)    10742 2023-07-21 05:53:03.000000 pulumi_kubernetes-4.1.0a1689918291/pulumi_kubernetes/rbac/v1alpha1/ClusterRoleList.py
--rw-r--r--   0 runner    (1001) docker     (123)    15068 2023-07-21 05:53:03.000000 pulumi_kubernetes-4.1.0a1689918291/pulumi_kubernetes/rbac/v1alpha1/ClusterRolePatch.py
--rw-r--r--   0 runner    (1001) docker     (123)    10958 2023-07-21 05:53:03.000000 pulumi_kubernetes-4.1.0a1689918291/pulumi_kubernetes/rbac/v1alpha1/Role.py
--rw-r--r--   0 runner    (1001) docker     (123)    13410 2023-07-21 05:53:03.000000 pulumi_kubernetes-4.1.0a1689918291/pulumi_kubernetes/rbac/v1alpha1/RoleBinding.py
--rw-r--r--   0 runner    (1001) docker     (123)    10746 2023-07-21 05:53:03.000000 pulumi_kubernetes-4.1.0a1689918291/pulumi_kubernetes/rbac/v1alpha1/RoleBindingList.py
--rw-r--r--   0 runner    (1001) docker     (123)    15032 2023-07-21 05:53:03.000000 pulumi_kubernetes-4.1.0a1689918291/pulumi_kubernetes/rbac/v1alpha1/RoleBindingPatch.py
--rw-r--r--   0 runner    (1001) docker     (123)    10489 2023-07-21 05:53:03.000000 pulumi_kubernetes-4.1.0a1689918291/pulumi_kubernetes/rbac/v1alpha1/RoleList.py
--rw-r--r--   0 runner    (1001) docker     (123)    12561 2023-07-21 05:53:03.000000 pulumi_kubernetes-4.1.0a1689918291/pulumi_kubernetes/rbac/v1alpha1/RolePatch.py
--rw-r--r--   0 runner    (1001) docker     (123)      644 2023-07-21 05:53:03.000000 pulumi_kubernetes-4.1.0a1689918291/pulumi_kubernetes/rbac/v1alpha1/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)    43219 2023-07-21 05:53:03.000000 pulumi_kubernetes-4.1.0a1689918291/pulumi_kubernetes/rbac/v1alpha1/_inputs.py
--rw-r--r--   0 runner    (1001) docker     (123)    44116 2023-07-21 05:53:03.000000 pulumi_kubernetes-4.1.0a1689918291/pulumi_kubernetes/rbac/v1alpha1/outputs.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-21 05:53:04.000000 pulumi_kubernetes-4.1.0a1689918291/pulumi_kubernetes/rbac/v1beta1/
--rw-r--r--   0 runner    (1001) docker     (123)    13413 2023-07-21 05:53:03.000000 pulumi_kubernetes-4.1.0a1689918291/pulumi_kubernetes/rbac/v1beta1/ClusterRole.py
--rw-r--r--   0 runner    (1001) docker     (123)    13145 2023-07-21 05:53:03.000000 pulumi_kubernetes-4.1.0a1689918291/pulumi_kubernetes/rbac/v1beta1/ClusterRoleBinding.py
--rw-r--r--   0 runner    (1001) docker     (123)    11004 2023-07-21 05:53:03.000000 pulumi_kubernetes-4.1.0a1689918291/pulumi_kubernetes/rbac/v1beta1/ClusterRoleBindingList.py
--rw-r--r--   0 runner    (1001) docker     (123)    14767 2023-07-21 05:53:03.000000 pulumi_kubernetes-4.1.0a1689918291/pulumi_kubernetes/rbac/v1beta1/ClusterRoleBindingPatch.py
--rw-r--r--   0 runner    (1001) docker     (123)    10739 2023-07-21 05:53:03.000000 pulumi_kubernetes-4.1.0a1689918291/pulumi_kubernetes/rbac/v1beta1/ClusterRoleList.py
--rw-r--r--   0 runner    (1001) docker     (123)    15066 2023-07-21 05:53:03.000000 pulumi_kubernetes-4.1.0a1689918291/pulumi_kubernetes/rbac/v1beta1/ClusterRolePatch.py
--rw-r--r--   0 runner    (1001) docker     (123)    10956 2023-07-21 05:53:03.000000 pulumi_kubernetes-4.1.0a1689918291/pulumi_kubernetes/rbac/v1beta1/Role.py
--rw-r--r--   0 runner    (1001) docker     (123)    13408 2023-07-21 05:53:03.000000 pulumi_kubernetes-4.1.0a1689918291/pulumi_kubernetes/rbac/v1beta1/RoleBinding.py
--rw-r--r--   0 runner    (1001) docker     (123)    10743 2023-07-21 05:53:03.000000 pulumi_kubernetes-4.1.0a1689918291/pulumi_kubernetes/rbac/v1beta1/RoleBindingList.py
--rw-r--r--   0 runner    (1001) docker     (123)    15030 2023-07-21 05:53:03.000000 pulumi_kubernetes-4.1.0a1689918291/pulumi_kubernetes/rbac/v1beta1/RoleBindingPatch.py
--rw-r--r--   0 runner    (1001) docker     (123)    10484 2023-07-21 05:53:03.000000 pulumi_kubernetes-4.1.0a1689918291/pulumi_kubernetes/rbac/v1beta1/RoleList.py
--rw-r--r--   0 runner    (1001) docker     (123)    12559 2023-07-21 05:53:03.000000 pulumi_kubernetes-4.1.0a1689918291/pulumi_kubernetes/rbac/v1beta1/RolePatch.py
--rw-r--r--   0 runner    (1001) docker     (123)      644 2023-07-21 05:53:03.000000 pulumi_kubernetes-4.1.0a1689918291/pulumi_kubernetes/rbac/v1beta1/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)    42923 2023-07-21 05:53:03.000000 pulumi_kubernetes-4.1.0a1689918291/pulumi_kubernetes/rbac/v1beta1/_inputs.py
--rw-r--r--   0 runner    (1001) docker     (123)    43824 2023-07-21 05:53:03.000000 pulumi_kubernetes-4.1.0a1689918291/pulumi_kubernetes/rbac/v1beta1/outputs.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-21 05:53:04.000000 pulumi_kubernetes-4.1.0a1689918291/pulumi_kubernetes/resource/
--rw-r--r--   0 runner    (1001) docker     (123)      585 2023-07-21 05:53:03.000000 pulumi_kubernetes-4.1.0a1689918291/pulumi_kubernetes/resource/__init__.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-21 05:53:04.000000 pulumi_kubernetes-4.1.0a1689918291/pulumi_kubernetes/resource/v1alpha1/
--rw-r--r--   0 runner    (1001) docker     (123)    11150 2023-07-21 05:53:03.000000 pulumi_kubernetes-4.1.0a1689918291/pulumi_kubernetes/resource/v1alpha1/PodScheduling.py
--rw-r--r--   0 runner    (1001) docker     (123)    10590 2023-07-21 05:53:03.000000 pulumi_kubernetes-4.1.0a1689918291/pulumi_kubernetes/resource/v1alpha1/PodSchedulingList.py
--rw-r--r--   0 runner    (1001) docker     (123)    12721 2023-07-21 05:53:03.000000 pulumi_kubernetes-4.1.0a1689918291/pulumi_kubernetes/resource/v1alpha1/PodSchedulingPatch.py
--rw-r--r--   0 runner    (1001) docker     (123)    11794 2023-07-21 05:53:03.000000 pulumi_kubernetes-4.1.0a1689918291/pulumi_kubernetes/resource/v1alpha1/ResourceClaim.py
--rw-r--r--   0 runner    (1001) docker     (123)    10564 2023-07-21 05:53:03.000000 pulumi_kubernetes-4.1.0a1689918291/pulumi_kubernetes/resource/v1alpha1/ResourceClaimList.py
--rw-r--r--   0 runner    (1001) docker     (123)    13370 2023-07-21 05:53:03.000000 pulumi_kubernetes-4.1.0a1689918291/pulumi_kubernetes/resource/v1alpha1/ResourceClaimPatch.py
--rw-r--r--   0 runner    (1001) docker     (123)    11484 2023-07-21 05:53:03.000000 pulumi_kubernetes-4.1.0a1689918291/pulumi_kubernetes/resource/v1alpha1/ResourceClaimTemplate.py
--rw-r--r--   0 runner    (1001) docker     (123)    10820 2023-07-21 05:53:03.000000 pulumi_kubernetes-4.1.0a1689918291/pulumi_kubernetes/resource/v1alpha1/ResourceClaimTemplateList.py
--rw-r--r--   0 runner    (1001) docker     (123)    13055 2023-07-21 05:53:03.000000 pulumi_kubernetes-4.1.0a1689918291/pulumi_kubernetes/resource/v1alpha1/ResourceClaimTemplatePatch.py
--rw-r--r--   0 runner    (1001) docker     (123)    16437 2023-07-21 05:53:03.000000 pulumi_kubernetes-4.1.0a1689918291/pulumi_kubernetes/resource/v1alpha1/ResourceClass.py
--rw-r--r--   0 runner    (1001) docker     (123)    10570 2023-07-21 05:53:03.000000 pulumi_kubernetes-4.1.0a1689918291/pulumi_kubernetes/resource/v1alpha1/ResourceClassList.py
--rw-r--r--   0 runner    (1001) docker     (123)    18061 2023-07-21 05:53:03.000000 pulumi_kubernetes-4.1.0a1689918291/pulumi_kubernetes/resource/v1alpha1/ResourceClassPatch.py
--rw-r--r--   0 runner    (1001) docker     (123)      692 2023-07-21 05:53:03.000000 pulumi_kubernetes-4.1.0a1689918291/pulumi_kubernetes/resource/v1alpha1/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)    59521 2023-07-21 05:53:03.000000 pulumi_kubernetes-4.1.0a1689918291/pulumi_kubernetes/resource/v1alpha1/_inputs.py
--rw-r--r--   0 runner    (1001) docker     (123)    77374 2023-07-21 05:53:03.000000 pulumi_kubernetes-4.1.0a1689918291/pulumi_kubernetes/resource/v1alpha1/outputs.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-21 05:53:04.000000 pulumi_kubernetes-4.1.0a1689918291/pulumi_kubernetes/resource/v1alpha2/
--rw-r--r--   0 runner    (1001) docker     (123)    11360 2023-07-21 05:53:03.000000 pulumi_kubernetes-4.1.0a1689918291/pulumi_kubernetes/resource/v1alpha2/PodSchedulingContext.py
--rw-r--r--   0 runner    (1001) docker     (123)    10821 2023-07-21 05:53:03.000000 pulumi_kubernetes-4.1.0a1689918291/pulumi_kubernetes/resource/v1alpha2/PodSchedulingContextList.py
--rw-r--r--   0 runner    (1001) docker     (123)    12931 2023-07-21 05:53:03.000000 pulumi_kubernetes-4.1.0a1689918291/pulumi_kubernetes/resource/v1alpha2/PodSchedulingContextPatch.py
--rw-r--r--   0 runner    (1001) docker     (123)    11794 2023-07-21 05:53:03.000000 pulumi_kubernetes-4.1.0a1689918291/pulumi_kubernetes/resource/v1alpha2/ResourceClaim.py
--rw-r--r--   0 runner    (1001) docker     (123)    10564 2023-07-21 05:53:03.000000 pulumi_kubernetes-4.1.0a1689918291/pulumi_kubernetes/resource/v1alpha2/ResourceClaimList.py
--rw-r--r--   0 runner    (1001) docker     (123)    13370 2023-07-21 05:53:03.000000 pulumi_kubernetes-4.1.0a1689918291/pulumi_kubernetes/resource/v1alpha2/ResourceClaimPatch.py
--rw-r--r--   0 runner    (1001) docker     (123)    11484 2023-07-21 05:53:03.000000 pulumi_kubernetes-4.1.0a1689918291/pulumi_kubernetes/resource/v1alpha2/ResourceClaimTemplate.py
--rw-r--r--   0 runner    (1001) docker     (123)    10820 2023-07-21 05:53:03.000000 pulumi_kubernetes-4.1.0a1689918291/pulumi_kubernetes/resource/v1alpha2/ResourceClaimTemplateList.py
--rw-r--r--   0 runner    (1001) docker     (123)    13055 2023-07-21 05:53:03.000000 pulumi_kubernetes-4.1.0a1689918291/pulumi_kubernetes/resource/v1alpha2/ResourceClaimTemplatePatch.py
--rw-r--r--   0 runner    (1001) docker     (123)    16437 2023-07-21 05:53:03.000000 pulumi_kubernetes-4.1.0a1689918291/pulumi_kubernetes/resource/v1alpha2/ResourceClass.py
--rw-r--r--   0 runner    (1001) docker     (123)    10570 2023-07-21 05:53:03.000000 pulumi_kubernetes-4.1.0a1689918291/pulumi_kubernetes/resource/v1alpha2/ResourceClassList.py
--rw-r--r--   0 runner    (1001) docker     (123)    18061 2023-07-21 05:53:03.000000 pulumi_kubernetes-4.1.0a1689918291/pulumi_kubernetes/resource/v1alpha2/ResourceClassPatch.py
--rw-r--r--   0 runner    (1001) docker     (123)      713 2023-07-21 05:53:03.000000 pulumi_kubernetes-4.1.0a1689918291/pulumi_kubernetes/resource/v1alpha2/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)    63467 2023-07-21 05:53:03.000000 pulumi_kubernetes-4.1.0a1689918291/pulumi_kubernetes/resource/v1alpha2/_inputs.py
--rw-r--r--   0 runner    (1001) docker     (123)    85824 2023-07-21 05:53:03.000000 pulumi_kubernetes-4.1.0a1689918291/pulumi_kubernetes/resource/v1alpha2/outputs.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-21 05:53:04.000000 pulumi_kubernetes-4.1.0a1689918291/pulumi_kubernetes/scheduling/
--rw-r--r--   0 runner    (1001) docker     (123)      719 2023-07-21 05:53:03.000000 pulumi_kubernetes-4.1.0a1689918291/pulumi_kubernetes/scheduling/__init__.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-21 05:53:04.000000 pulumi_kubernetes-4.1.0a1689918291/pulumi_kubernetes/scheduling/v1/
--rw-r--r--   0 runner    (1001) docker     (123)    17212 2023-07-21 05:53:03.000000 pulumi_kubernetes-4.1.0a1689918291/pulumi_kubernetes/scheduling/v1/PriorityClass.py
--rw-r--r--   0 runner    (1001) docker     (123)    10954 2023-07-21 05:53:03.000000 pulumi_kubernetes-4.1.0a1689918291/pulumi_kubernetes/scheduling/v1/PriorityClassList.py
--rw-r--r--   0 runner    (1001) docker     (123)    18777 2023-07-21 05:53:03.000000 pulumi_kubernetes-4.1.0a1689918291/pulumi_kubernetes/scheduling/v1/PriorityClassPatch.py
--rw-r--r--   0 runner    (1001) docker     (123)      380 2023-07-21 05:53:03.000000 pulumi_kubernetes-4.1.0a1689918291/pulumi_kubernetes/scheduling/v1/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)     7318 2023-07-21 05:53:03.000000 pulumi_kubernetes-4.1.0a1689918291/pulumi_kubernetes/scheduling/v1/_inputs.py
--rw-r--r--   0 runner    (1001) docker     (123)     6955 2023-07-21 05:53:03.000000 pulumi_kubernetes-4.1.0a1689918291/pulumi_kubernetes/scheduling/v1/outputs.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-21 05:53:04.000000 pulumi_kubernetes-4.1.0a1689918291/pulumi_kubernetes/scheduling/v1alpha1/
--rw-r--r--   0 runner    (1001) docker     (123)    17744 2023-07-21 05:53:03.000000 pulumi_kubernetes-4.1.0a1689918291/pulumi_kubernetes/scheduling/v1alpha1/PriorityClass.py
--rw-r--r--   0 runner    (1001) docker     (123)    10972 2023-07-21 05:53:03.000000 pulumi_kubernetes-4.1.0a1689918291/pulumi_kubernetes/scheduling/v1alpha1/PriorityClassList.py
--rw-r--r--   0 runner    (1001) docker     (123)    19309 2023-07-21 05:53:03.000000 pulumi_kubernetes-4.1.0a1689918291/pulumi_kubernetes/scheduling/v1alpha1/PriorityClassPatch.py
--rw-r--r--   0 runner    (1001) docker     (123)      380 2023-07-21 05:53:03.000000 pulumi_kubernetes-4.1.0a1689918291/pulumi_kubernetes/scheduling/v1alpha1/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)     7584 2023-07-21 05:53:03.000000 pulumi_kubernetes-4.1.0a1689918291/pulumi_kubernetes/scheduling/v1alpha1/_inputs.py
--rw-r--r--   0 runner    (1001) docker     (123)     7323 2023-07-21 05:53:03.000000 pulumi_kubernetes-4.1.0a1689918291/pulumi_kubernetes/scheduling/v1alpha1/outputs.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-21 05:53:04.000000 pulumi_kubernetes-4.1.0a1689918291/pulumi_kubernetes/scheduling/v1beta1/
--rw-r--r--   0 runner    (1001) docker     (123)    17742 2023-07-21 05:53:03.000000 pulumi_kubernetes-4.1.0a1689918291/pulumi_kubernetes/scheduling/v1beta1/PriorityClass.py
--rw-r--r--   0 runner    (1001) docker     (123)    10969 2023-07-21 05:53:03.000000 pulumi_kubernetes-4.1.0a1689918291/pulumi_kubernetes/scheduling/v1beta1/PriorityClassList.py
--rw-r--r--   0 runner    (1001) docker     (123)    19307 2023-07-21 05:53:03.000000 pulumi_kubernetes-4.1.0a1689918291/pulumi_kubernetes/scheduling/v1beta1/PriorityClassPatch.py
--rw-r--r--   0 runner    (1001) docker     (123)      380 2023-07-21 05:53:03.000000 pulumi_kubernetes-4.1.0a1689918291/pulumi_kubernetes/scheduling/v1beta1/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)     7583 2023-07-21 05:53:03.000000 pulumi_kubernetes-4.1.0a1689918291/pulumi_kubernetes/scheduling/v1beta1/_inputs.py
--rw-r--r--   0 runner    (1001) docker     (123)     7322 2023-07-21 05:53:03.000000 pulumi_kubernetes-4.1.0a1689918291/pulumi_kubernetes/scheduling/v1beta1/outputs.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-21 05:53:04.000000 pulumi_kubernetes-4.1.0a1689918291/pulumi_kubernetes/settings/
--rw-r--r--   0 runner    (1001) docker     (123)      421 2023-07-21 05:53:03.000000 pulumi_kubernetes-4.1.0a1689918291/pulumi_kubernetes/settings/__init__.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-21 05:53:04.000000 pulumi_kubernetes-4.1.0a1689918291/pulumi_kubernetes/settings/v1alpha1/
--rw-r--r--   0 runner    (1001) docker     (123)     9676 2023-07-21 05:53:03.000000 pulumi_kubernetes-4.1.0a1689918291/pulumi_kubernetes/settings/v1alpha1/PodPreset.py
--rw-r--r--   0 runner    (1001) docker     (123)    10866 2023-07-21 05:53:03.000000 pulumi_kubernetes-4.1.0a1689918291/pulumi_kubernetes/settings/v1alpha1/PodPresetList.py
--rw-r--r--   0 runner    (1001) docker     (123)    11249 2023-07-21 05:53:03.000000 pulumi_kubernetes-4.1.0a1689918291/pulumi_kubernetes/settings/v1alpha1/PodPresetPatch.py
--rw-r--r--   0 runner    (1001) docker     (123)      368 2023-07-21 05:53:03.000000 pulumi_kubernetes-4.1.0a1689918291/pulumi_kubernetes/settings/v1alpha1/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)    12130 2023-07-21 05:53:03.000000 pulumi_kubernetes-4.1.0a1689918291/pulumi_kubernetes/settings/v1alpha1/_inputs.py
--rw-r--r--   0 runner    (1001) docker     (123)    11192 2023-07-21 05:53:03.000000 pulumi_kubernetes-4.1.0a1689918291/pulumi_kubernetes/settings/v1alpha1/outputs.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-21 05:53:04.000000 pulumi_kubernetes-4.1.0a1689918291/pulumi_kubernetes/storage/
--rw-r--r--   0 runner    (1001) docker     (123)      701 2023-07-21 05:53:03.000000 pulumi_kubernetes-4.1.0a1689918291/pulumi_kubernetes/storage/__init__.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-21 05:53:04.000000 pulumi_kubernetes-4.1.0a1689918291/pulumi_kubernetes/storage/v1/
--rw-r--r--   0 runner    (1001) docker     (123)    12783 2023-07-21 05:53:03.000000 pulumi_kubernetes-4.1.0a1689918291/pulumi_kubernetes/storage/v1/CSIDriver.py
--rw-r--r--   0 runner    (1001) docker     (123)    10807 2023-07-21 05:53:03.000000 pulumi_kubernetes-4.1.0a1689918291/pulumi_kubernetes/storage/v1/CSIDriverList.py
--rw-r--r--   0 runner    (1001) docker     (123)    14354 2023-07-21 05:53:03.000000 pulumi_kubernetes-4.1.0a1689918291/pulumi_kubernetes/storage/v1/CSIDriverPatch.py
--rw-r--r--   0 runner    (1001) docker     (123)    11643 2023-07-21 05:53:03.000000 pulumi_kubernetes-4.1.0a1689918291/pulumi_kubernetes/storage/v1/CSINode.py
--rw-r--r--   0 runner    (1001) docker     (123)    10737 2023-07-21 05:53:03.000000 pulumi_kubernetes-4.1.0a1689918291/pulumi_kubernetes/storage/v1/CSINodeList.py
--rw-r--r--   0 runner    (1001) docker     (123)    13214 2023-07-21 05:53:03.000000 pulumi_kubernetes-4.1.0a1689918291/pulumi_kubernetes/storage/v1/CSINodePatch.py
--rw-r--r--   0 runner    (1001) docker     (123)    24161 2023-07-21 05:53:03.000000 pulumi_kubernetes-4.1.0a1689918291/pulumi_kubernetes/storage/v1/CSIStorageCapacity.py
--rw-r--r--   0 runner    (1001) docker     (123)    11158 2023-07-21 05:53:03.000000 pulumi_kubernetes-4.1.0a1689918291/pulumi_kubernetes/storage/v1/CSIStorageCapacityList.py
--rw-r--r--   0 runner    (1001) docker     (123)    25753 2023-07-21 05:53:03.000000 pulumi_kubernetes-4.1.0a1689918291/pulumi_kubernetes/storage/v1/CSIStorageCapacityPatch.py
--rw-r--r--   0 runner    (1001) docker     (123)    22861 2023-07-21 05:53:03.000000 pulumi_kubernetes-4.1.0a1689918291/pulumi_kubernetes/storage/v1/StorageClass.py
--rw-r--r--   0 runner    (1001) docker     (123)    10940 2023-07-21 05:53:03.000000 pulumi_kubernetes-4.1.0a1689918291/pulumi_kubernetes/storage/v1/StorageClassList.py
--rw-r--r--   0 runner    (1001) docker     (123)    24485 2023-07-21 05:53:03.000000 pulumi_kubernetes-4.1.0a1689918291/pulumi_kubernetes/storage/v1/StorageClassPatch.py
--rw-r--r--   0 runner    (1001) docker     (123)    12090 2023-07-21 05:53:03.000000 pulumi_kubernetes-4.1.0a1689918291/pulumi_kubernetes/storage/v1/VolumeAttachment.py
--rw-r--r--   0 runner    (1001) docker     (123)    11086 2023-07-21 05:53:03.000000 pulumi_kubernetes-4.1.0a1689918291/pulumi_kubernetes/storage/v1/VolumeAttachmentList.py
--rw-r--r--   0 runner    (1001) docker     (123)    13671 2023-07-21 05:53:03.000000 pulumi_kubernetes-4.1.0a1689918291/pulumi_kubernetes/storage/v1/VolumeAttachmentPatch.py
--rw-r--r--   0 runner    (1001) docker     (123)      755 2023-07-21 05:53:03.000000 pulumi_kubernetes-4.1.0a1689918291/pulumi_kubernetes/storage/v1/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)   105129 2023-07-21 05:53:03.000000 pulumi_kubernetes-4.1.0a1689918291/pulumi_kubernetes/storage/v1/_inputs.py
--rw-r--r--   0 runner    (1001) docker     (123)   111767 2023-07-21 05:53:03.000000 pulumi_kubernetes-4.1.0a1689918291/pulumi_kubernetes/storage/v1/outputs.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-21 05:53:04.000000 pulumi_kubernetes-4.1.0a1689918291/pulumi_kubernetes/storage/v1alpha1/
--rw-r--r--   0 runner    (1001) docker     (123)    12020 2023-07-21 05:53:03.000000 pulumi_kubernetes-4.1.0a1689918291/pulumi_kubernetes/storage/v1alpha1/VolumeAttachment.py
--rw-r--r--   0 runner    (1001) docker     (123)    11104 2023-07-21 05:53:03.000000 pulumi_kubernetes-4.1.0a1689918291/pulumi_kubernetes/storage/v1alpha1/VolumeAttachmentList.py
--rw-r--r--   0 runner    (1001) docker     (123)    13601 2023-07-21 05:53:03.000000 pulumi_kubernetes-4.1.0a1689918291/pulumi_kubernetes/storage/v1alpha1/VolumeAttachmentPatch.py
--rw-r--r--   0 runner    (1001) docker     (123)      389 2023-07-21 05:53:03.000000 pulumi_kubernetes-4.1.0a1689918291/pulumi_kubernetes/storage/v1alpha1/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)    20227 2023-07-21 05:53:03.000000 pulumi_kubernetes-4.1.0a1689918291/pulumi_kubernetes/storage/v1alpha1/_inputs.py
--rw-r--r--   0 runner    (1001) docker     (123)    26754 2023-07-21 05:53:03.000000 pulumi_kubernetes-4.1.0a1689918291/pulumi_kubernetes/storage/v1alpha1/outputs.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-21 05:53:04.000000 pulumi_kubernetes-4.1.0a1689918291/pulumi_kubernetes/storage/v1beta1/
--rw-r--r--   0 runner    (1001) docker     (123)    13183 2023-07-21 05:53:03.000000 pulumi_kubernetes-4.1.0a1689918291/pulumi_kubernetes/storage/v1beta1/CSIDriver.py
--rw-r--r--   0 runner    (1001) docker     (123)    10822 2023-07-21 05:53:03.000000 pulumi_kubernetes-4.1.0a1689918291/pulumi_kubernetes/storage/v1beta1/CSIDriverList.py
--rw-r--r--   0 runner    (1001) docker     (123)    14754 2023-07-21 05:53:03.000000 pulumi_kubernetes-4.1.0a1689918291/pulumi_kubernetes/storage/v1beta1/CSIDriverPatch.py
--rw-r--r--   0 runner    (1001) docker     (123)    11541 2023-07-21 05:53:03.000000 pulumi_kubernetes-4.1.0a1689918291/pulumi_kubernetes/storage/v1beta1/CSINode.py
--rw-r--r--   0 runner    (1001) docker     (123)    10752 2023-07-21 05:53:03.000000 pulumi_kubernetes-4.1.0a1689918291/pulumi_kubernetes/storage/v1beta1/CSINodeList.py
--rw-r--r--   0 runner    (1001) docker     (123)    13112 2023-07-21 05:53:03.000000 pulumi_kubernetes-4.1.0a1689918291/pulumi_kubernetes/storage/v1beta1/CSINodePatch.py
--rw-r--r--   0 runner    (1001) docker     (123)    24071 2023-07-21 05:53:03.000000 pulumi_kubernetes-4.1.0a1689918291/pulumi_kubernetes/storage/v1beta1/CSIStorageCapacity.py
--rw-r--r--   0 runner    (1001) docker     (123)    11173 2023-07-21 05:53:03.000000 pulumi_kubernetes-4.1.0a1689918291/pulumi_kubernetes/storage/v1beta1/CSIStorageCapacityList.py
--rw-r--r--   0 runner    (1001) docker     (123)    25663 2023-07-21 05:53:03.000000 pulumi_kubernetes-4.1.0a1689918291/pulumi_kubernetes/storage/v1beta1/CSIStorageCapacityPatch.py
--rw-r--r--   0 runner    (1001) docker     (123)    22731 2023-07-21 05:53:03.000000 pulumi_kubernetes-4.1.0a1689918291/pulumi_kubernetes/storage/v1beta1/StorageClass.py
--rw-r--r--   0 runner    (1001) docker     (123)    10955 2023-07-21 05:53:03.000000 pulumi_kubernetes-4.1.0a1689918291/pulumi_kubernetes/storage/v1beta1/StorageClassList.py
--rw-r--r--   0 runner    (1001) docker     (123)    24355 2023-07-21 05:53:03.000000 pulumi_kubernetes-4.1.0a1689918291/pulumi_kubernetes/storage/v1beta1/StorageClassPatch.py
--rw-r--r--   0 runner    (1001) docker     (123)    12018 2023-07-21 05:53:03.000000 pulumi_kubernetes-4.1.0a1689918291/pulumi_kubernetes/storage/v1beta1/VolumeAttachment.py
--rw-r--r--   0 runner    (1001) docker     (123)    11101 2023-07-21 05:53:03.000000 pulumi_kubernetes-4.1.0a1689918291/pulumi_kubernetes/storage/v1beta1/VolumeAttachmentList.py
--rw-r--r--   0 runner    (1001) docker     (123)    13599 2023-07-21 05:53:03.000000 pulumi_kubernetes-4.1.0a1689918291/pulumi_kubernetes/storage/v1beta1/VolumeAttachmentPatch.py
--rw-r--r--   0 runner    (1001) docker     (123)      755 2023-07-21 05:53:03.000000 pulumi_kubernetes-4.1.0a1689918291/pulumi_kubernetes/storage/v1beta1/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)    98721 2023-07-21 05:53:03.000000 pulumi_kubernetes-4.1.0a1689918291/pulumi_kubernetes/storage/v1beta1/_inputs.py
--rw-r--r--   0 runner    (1001) docker     (123)   105646 2023-07-21 05:53:03.000000 pulumi_kubernetes-4.1.0a1689918291/pulumi_kubernetes/storage/v1beta1/outputs.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-21 05:53:04.000000 pulumi_kubernetes-4.1.0a1689918291/pulumi_kubernetes/yaml/
--rw-r--r--   0 runner    (1001) docker     (123)      258 2023-07-21 05:53:03.000000 pulumi_kubernetes-4.1.0a1689918291/pulumi_kubernetes/yaml/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)   100539 2023-07-21 05:53:03.000000 pulumi_kubernetes-4.1.0a1689918291/pulumi_kubernetes/yaml/yaml.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-21 05:53:04.000000 pulumi_kubernetes-4.1.0a1689918291/pulumi_kubernetes.egg-info/
--rw-r--r--   0 runner    (1001) docker     (123)    11092 2023-07-21 05:53:04.000000 pulumi_kubernetes-4.1.0a1689918291/pulumi_kubernetes.egg-info/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (123)    28617 2023-07-21 05:53:04.000000 pulumi_kubernetes-4.1.0a1689918291/pulumi_kubernetes.egg-info/SOURCES.txt
--rw-r--r--   0 runner    (1001) docker     (123)        1 2023-07-21 05:53:04.000000 pulumi_kubernetes-4.1.0a1689918291/pulumi_kubernetes.egg-info/dependency_links.txt
--rw-r--r--   0 runner    (1001) docker     (123)        1 2023-07-21 05:53:03.000000 pulumi_kubernetes-4.1.0a1689918291/pulumi_kubernetes.egg-info/not-zip-safe
--rw-r--r--   0 runner    (1001) docker     (123)       70 2023-07-21 05:53:04.000000 pulumi_kubernetes-4.1.0a1689918291/pulumi_kubernetes.egg-info/requires.txt
--rw-r--r--   0 runner    (1001) docker     (123)       18 2023-07-21 05:53:04.000000 pulumi_kubernetes-4.1.0a1689918291/pulumi_kubernetes.egg-info/top_level.txt
--rw-r--r--   0 runner    (1001) docker     (123)       38 2023-07-21 05:53:04.000000 pulumi_kubernetes-4.1.0a1689918291/setup.cfg
--rw-r--r--   0 runner    (1001) docker     (123)     2216 2023-07-21 05:53:03.000000 pulumi_kubernetes-4.1.0a1689918291/setup.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-21 20:45:53.000000 pulumi_kubernetes-4.1.0a1689971798/
+-rw-r--r--   0 runner    (1001) docker     (123)    11092 2023-07-21 20:45:53.000000 pulumi_kubernetes-4.1.0a1689971798/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (123)     8829 2023-07-21 20:45:52.000000 pulumi_kubernetes-4.1.0a1689971798/README.md
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-21 20:45:53.000000 pulumi_kubernetes-4.1.0a1689971798/pulumi_kubernetes/
+-rw-r--r--   0 runner    (1001) docker     (123)    39084 2023-07-21 20:45:52.000000 pulumi_kubernetes-4.1.0a1689971798/pulumi_kubernetes/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)     6932 2023-07-21 20:45:52.000000 pulumi_kubernetes-4.1.0a1689971798/pulumi_kubernetes/_inputs.py
+-rw-r--r--   0 runner    (1001) docker     (123)    40823 2023-07-21 20:45:52.000000 pulumi_kubernetes-4.1.0a1689971798/pulumi_kubernetes/_tables.py
+-rw-r--r--   0 runner    (1001) docker     (123)     8050 2023-07-21 20:45:52.000000 pulumi_kubernetes-4.1.0a1689971798/pulumi_kubernetes/_utilities.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-21 20:45:53.000000 pulumi_kubernetes-4.1.0a1689971798/pulumi_kubernetes/admissionregistration/
+-rw-r--r--   0 runner    (1001) docker     (123)      785 2023-07-21 20:45:52.000000 pulumi_kubernetes-4.1.0a1689971798/pulumi_kubernetes/admissionregistration/__init__.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-21 20:45:53.000000 pulumi_kubernetes-4.1.0a1689971798/pulumi_kubernetes/admissionregistration/v1/
+-rw-r--r--   0 runner    (1001) docker     (123)    11822 2023-07-21 20:45:52.000000 pulumi_kubernetes-4.1.0a1689971798/pulumi_kubernetes/admissionregistration/v1/MutatingWebhookConfiguration.py
+-rw-r--r--   0 runner    (1001) docker     (123)    11454 2023-07-21 20:45:52.000000 pulumi_kubernetes-4.1.0a1689971798/pulumi_kubernetes/admissionregistration/v1/MutatingWebhookConfigurationList.py
+-rw-r--r--   0 runner    (1001) docker     (123)    13420 2023-07-21 20:45:52.000000 pulumi_kubernetes-4.1.0a1689971798/pulumi_kubernetes/admissionregistration/v1/MutatingWebhookConfigurationPatch.py
+-rw-r--r--   0 runner    (1001) docker     (123)    11892 2023-07-21 20:45:52.000000 pulumi_kubernetes-4.1.0a1689971798/pulumi_kubernetes/admissionregistration/v1/ValidatingWebhookConfiguration.py
+-rw-r--r--   0 runner    (1001) docker     (123)    11524 2023-07-21 20:45:52.000000 pulumi_kubernetes-4.1.0a1689971798/pulumi_kubernetes/admissionregistration/v1/ValidatingWebhookConfigurationList.py
+-rw-r--r--   0 runner    (1001) docker     (123)    13490 2023-07-21 20:45:52.000000 pulumi_kubernetes-4.1.0a1689971798/pulumi_kubernetes/admissionregistration/v1/ValidatingWebhookConfigurationPatch.py
+-rw-r--r--   0 runner    (1001) docker     (123)      572 2023-07-21 20:45:52.000000 pulumi_kubernetes-4.1.0a1689971798/pulumi_kubernetes/admissionregistration/v1/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)   126842 2023-07-21 20:45:52.000000 pulumi_kubernetes-4.1.0a1689971798/pulumi_kubernetes/admissionregistration/v1/_inputs.py
+-rw-r--r--   0 runner    (1001) docker     (123)   121022 2023-07-21 20:45:52.000000 pulumi_kubernetes-4.1.0a1689971798/pulumi_kubernetes/admissionregistration/v1/outputs.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-21 20:45:53.000000 pulumi_kubernetes-4.1.0a1689971798/pulumi_kubernetes/admissionregistration/v1alpha1/
+-rw-r--r--   0 runner    (1001) docker     (123)    11903 2023-07-21 20:45:52.000000 pulumi_kubernetes-4.1.0a1689971798/pulumi_kubernetes/admissionregistration/v1alpha1/ValidatingAdmissionPolicy.py
+-rw-r--r--   0 runner    (1001) docker     (123)    11826 2023-07-21 20:45:52.000000 pulumi_kubernetes-4.1.0a1689971798/pulumi_kubernetes/admissionregistration/v1alpha1/ValidatingAdmissionPolicyBinding.py
+-rw-r--r--   0 runner    (1001) docker     (123)    11508 2023-07-21 20:45:52.000000 pulumi_kubernetes-4.1.0a1689971798/pulumi_kubernetes/admissionregistration/v1alpha1/ValidatingAdmissionPolicyBindingList.py
+-rw-r--r--   0 runner    (1001) docker     (123)    13419 2023-07-21 20:45:52.000000 pulumi_kubernetes-4.1.0a1689971798/pulumi_kubernetes/admissionregistration/v1alpha1/ValidatingAdmissionPolicyBindingPatch.py
+-rw-r--r--   0 runner    (1001) docker     (123)    11339 2023-07-21 20:45:52.000000 pulumi_kubernetes-4.1.0a1689971798/pulumi_kubernetes/admissionregistration/v1alpha1/ValidatingAdmissionPolicyList.py
+-rw-r--r--   0 runner    (1001) docker     (123)    13501 2023-07-21 20:45:52.000000 pulumi_kubernetes-4.1.0a1689971798/pulumi_kubernetes/admissionregistration/v1alpha1/ValidatingAdmissionPolicyPatch.py
+-rw-r--r--   0 runner    (1001) docker     (123)      569 2023-07-21 20:45:52.000000 pulumi_kubernetes-4.1.0a1689971798/pulumi_kubernetes/admissionregistration/v1alpha1/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)   136918 2023-07-21 20:45:52.000000 pulumi_kubernetes-4.1.0a1689971798/pulumi_kubernetes/admissionregistration/v1alpha1/_inputs.py
+-rw-r--r--   0 runner    (1001) docker     (123)   143284 2023-07-21 20:45:52.000000 pulumi_kubernetes-4.1.0a1689971798/pulumi_kubernetes/admissionregistration/v1alpha1/outputs.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-21 20:45:53.000000 pulumi_kubernetes-4.1.0a1689971798/pulumi_kubernetes/admissionregistration/v1beta1/
+-rw-r--r--   0 runner    (1001) docker     (123)    12082 2023-07-21 20:45:52.000000 pulumi_kubernetes-4.1.0a1689971798/pulumi_kubernetes/admissionregistration/v1beta1/MutatingWebhookConfiguration.py
+-rw-r--r--   0 runner    (1001) docker     (123)    11469 2023-07-21 20:45:52.000000 pulumi_kubernetes-4.1.0a1689971798/pulumi_kubernetes/admissionregistration/v1beta1/MutatingWebhookConfigurationList.py
+-rw-r--r--   0 runner    (1001) docker     (123)    13680 2023-07-21 20:45:52.000000 pulumi_kubernetes-4.1.0a1689971798/pulumi_kubernetes/admissionregistration/v1beta1/MutatingWebhookConfigurationPatch.py
+-rw-r--r--   0 runner    (1001) docker     (123)    12156 2023-07-21 20:45:52.000000 pulumi_kubernetes-4.1.0a1689971798/pulumi_kubernetes/admissionregistration/v1beta1/ValidatingWebhookConfiguration.py
+-rw-r--r--   0 runner    (1001) docker     (123)    11539 2023-07-21 20:45:52.000000 pulumi_kubernetes-4.1.0a1689971798/pulumi_kubernetes/admissionregistration/v1beta1/ValidatingWebhookConfigurationList.py
+-rw-r--r--   0 runner    (1001) docker     (123)    13754 2023-07-21 20:45:52.000000 pulumi_kubernetes-4.1.0a1689971798/pulumi_kubernetes/admissionregistration/v1beta1/ValidatingWebhookConfigurationPatch.py
+-rw-r--r--   0 runner    (1001) docker     (123)      572 2023-07-21 20:45:52.000000 pulumi_kubernetes-4.1.0a1689971798/pulumi_kubernetes/admissionregistration/v1beta1/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)   108512 2023-07-21 20:45:52.000000 pulumi_kubernetes-4.1.0a1689971798/pulumi_kubernetes/admissionregistration/v1beta1/_inputs.py
+-rw-r--r--   0 runner    (1001) docker     (123)   104062 2023-07-21 20:45:52.000000 pulumi_kubernetes-4.1.0a1689971798/pulumi_kubernetes/admissionregistration/v1beta1/outputs.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-21 20:45:53.000000 pulumi_kubernetes-4.1.0a1689971798/pulumi_kubernetes/apiextensions/
+-rw-r--r--   0 runner    (1001) docker     (123)     9255 2023-07-21 20:45:52.000000 pulumi_kubernetes-4.1.0a1689971798/pulumi_kubernetes/apiextensions/CustomResource.py
+-rw-r--r--   0 runner    (1001) docker     (123)     7835 2023-07-21 20:45:52.000000 pulumi_kubernetes-4.1.0a1689971798/pulumi_kubernetes/apiextensions/CustomResourcePatch.py
+-rw-r--r--   0 runner    (1001) docker     (123)      672 2023-07-21 20:45:52.000000 pulumi_kubernetes-4.1.0a1689971798/pulumi_kubernetes/apiextensions/__init__.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-21 20:45:53.000000 pulumi_kubernetes-4.1.0a1689971798/pulumi_kubernetes/apiextensions/v1/
+-rw-r--r--   0 runner    (1001) docker     (123)    11920 2023-07-21 20:45:52.000000 pulumi_kubernetes-4.1.0a1689971798/pulumi_kubernetes/apiextensions/v1/CustomResourceDefinition.py
+-rw-r--r--   0 runner    (1001) docker     (123)    11390 2023-07-21 20:45:52.000000 pulumi_kubernetes-4.1.0a1689971798/pulumi_kubernetes/apiextensions/v1/CustomResourceDefinitionList.py
+-rw-r--r--   0 runner    (1001) docker     (123)    13496 2023-07-21 20:45:52.000000 pulumi_kubernetes-4.1.0a1689971798/pulumi_kubernetes/apiextensions/v1/CustomResourceDefinitionPatch.py
+-rw-r--r--   0 runner    (1001) docker     (123)      413 2023-07-21 20:45:52.000000 pulumi_kubernetes-4.1.0a1689971798/pulumi_kubernetes/apiextensions/v1/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)   198456 2023-07-21 20:45:52.000000 pulumi_kubernetes-4.1.0a1689971798/pulumi_kubernetes/apiextensions/v1/_inputs.py
+-rw-r--r--   0 runner    (1001) docker     (123)   189683 2023-07-21 20:45:52.000000 pulumi_kubernetes-4.1.0a1689971798/pulumi_kubernetes/apiextensions/v1/outputs.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-21 20:45:53.000000 pulumi_kubernetes-4.1.0a1689971798/pulumi_kubernetes/apiextensions/v1beta1/
+-rw-r--r--   0 runner    (1001) docker     (123)    11420 2023-07-21 20:45:52.000000 pulumi_kubernetes-4.1.0a1689971798/pulumi_kubernetes/apiextensions/v1beta1/CustomResourceDefinition.py
+-rw-r--r--   0 runner    (1001) docker     (123)    10673 2023-07-21 20:45:52.000000 pulumi_kubernetes-4.1.0a1689971798/pulumi_kubernetes/apiextensions/v1beta1/CustomResourceDefinitionList.py
+-rw-r--r--   0 runner    (1001) docker     (123)    12986 2023-07-21 20:45:52.000000 pulumi_kubernetes-4.1.0a1689971798/pulumi_kubernetes/apiextensions/v1beta1/CustomResourceDefinitionPatch.py
+-rw-r--r--   0 runner    (1001) docker     (123)      413 2023-07-21 20:45:52.000000 pulumi_kubernetes-4.1.0a1689971798/pulumi_kubernetes/apiextensions/v1beta1/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)   183209 2023-07-21 20:45:52.000000 pulumi_kubernetes-4.1.0a1689971798/pulumi_kubernetes/apiextensions/v1beta1/_inputs.py
+-rw-r--r--   0 runner    (1001) docker     (123)   173449 2023-07-21 20:45:52.000000 pulumi_kubernetes-4.1.0a1689971798/pulumi_kubernetes/apiextensions/v1beta1/outputs.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-21 20:45:53.000000 pulumi_kubernetes-4.1.0a1689971798/pulumi_kubernetes/apiregistration/
+-rw-r--r--   0 runner    (1001) docker     (123)      571 2023-07-21 20:45:52.000000 pulumi_kubernetes-4.1.0a1689971798/pulumi_kubernetes/apiregistration/__init__.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-21 20:45:53.000000 pulumi_kubernetes-4.1.0a1689971798/pulumi_kubernetes/apiregistration/v1/
+-rw-r--r--   0 runner    (1001) docker     (123)    11560 2023-07-21 20:45:52.000000 pulumi_kubernetes-4.1.0a1689971798/pulumi_kubernetes/apiregistration/v1/APIService.py
+-rw-r--r--   0 runner    (1001) docker     (123)    11038 2023-07-21 20:45:52.000000 pulumi_kubernetes-4.1.0a1689971798/pulumi_kubernetes/apiregistration/v1/APIServiceList.py
+-rw-r--r--   0 runner    (1001) docker     (123)    13173 2023-07-21 20:45:52.000000 pulumi_kubernetes-4.1.0a1689971798/pulumi_kubernetes/apiregistration/v1/APIServicePatch.py
+-rw-r--r--   0 runner    (1001) docker     (123)      371 2023-07-21 20:45:52.000000 pulumi_kubernetes-4.1.0a1689971798/pulumi_kubernetes/apiregistration/v1/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)    30708 2023-07-21 20:45:52.000000 pulumi_kubernetes-4.1.0a1689971798/pulumi_kubernetes/apiregistration/v1/_inputs.py
+-rw-r--r--   0 runner    (1001) docker     (123)    32896 2023-07-21 20:45:52.000000 pulumi_kubernetes-4.1.0a1689971798/pulumi_kubernetes/apiregistration/v1/outputs.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-21 20:45:53.000000 pulumi_kubernetes-4.1.0a1689971798/pulumi_kubernetes/apiregistration/v1beta1/
+-rw-r--r--   0 runner    (1001) docker     (123)    10830 2023-07-21 20:45:52.000000 pulumi_kubernetes-4.1.0a1689971798/pulumi_kubernetes/apiregistration/v1beta1/APIService.py
+-rw-r--r--   0 runner    (1001) docker     (123)     9978 2023-07-21 20:45:52.000000 pulumi_kubernetes-4.1.0a1689971798/pulumi_kubernetes/apiregistration/v1beta1/APIServiceList.py
+-rw-r--r--   0 runner    (1001) docker     (123)    12433 2023-07-21 20:45:52.000000 pulumi_kubernetes-4.1.0a1689971798/pulumi_kubernetes/apiregistration/v1beta1/APIServicePatch.py
+-rw-r--r--   0 runner    (1001) docker     (123)      371 2023-07-21 20:45:52.000000 pulumi_kubernetes-4.1.0a1689971798/pulumi_kubernetes/apiregistration/v1beta1/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)    30275 2023-07-21 20:45:52.000000 pulumi_kubernetes-4.1.0a1689971798/pulumi_kubernetes/apiregistration/v1beta1/_inputs.py
+-rw-r--r--   0 runner    (1001) docker     (123)    32487 2023-07-21 20:45:52.000000 pulumi_kubernetes-4.1.0a1689971798/pulumi_kubernetes/apiregistration/v1beta1/outputs.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-21 20:45:53.000000 pulumi_kubernetes-4.1.0a1689971798/pulumi_kubernetes/apps/
+-rw-r--r--   0 runner    (1001) docker     (123)      677 2023-07-21 20:45:52.000000 pulumi_kubernetes-4.1.0a1689971798/pulumi_kubernetes/apps/__init__.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-21 20:45:53.000000 pulumi_kubernetes-4.1.0a1689971798/pulumi_kubernetes/apps/v1/
+-rw-r--r--   0 runner    (1001) docker     (123)    13236 2023-07-21 20:45:52.000000 pulumi_kubernetes-4.1.0a1689971798/pulumi_kubernetes/apps/v1/ControllerRevision.py
+-rw-r--r--   0 runner    (1001) docker     (123)    11036 2023-07-21 20:45:52.000000 pulumi_kubernetes-4.1.0a1689971798/pulumi_kubernetes/apps/v1/ControllerRevisionList.py
+-rw-r--r--   0 runner    (1001) docker     (123)    14778 2023-07-21 20:45:52.000000 pulumi_kubernetes-4.1.0a1689971798/pulumi_kubernetes/apps/v1/ControllerRevisionPatch.py
+-rw-r--r--   0 runner    (1001) docker     (123)    11854 2023-07-21 20:45:52.000000 pulumi_kubernetes-4.1.0a1689971798/pulumi_kubernetes/apps/v1/DaemonSet.py
+-rw-r--r--   0 runner    (1001) docker     (123)    10767 2023-07-21 20:45:52.000000 pulumi_kubernetes-4.1.0a1689971798/pulumi_kubernetes/apps/v1/DaemonSetList.py
+-rw-r--r--   0 runner    (1001) docker     (123)    13462 2023-07-21 20:45:52.000000 pulumi_kubernetes-4.1.0a1689971798/pulumi_kubernetes/apps/v1/DaemonSetPatch.py
+-rw-r--r--   0 runner    (1001) docker     (123)    19970 2023-07-21 20:45:52.000000 pulumi_kubernetes-4.1.0a1689971798/pulumi_kubernetes/apps/v1/Deployment.py
+-rw-r--r--   0 runner    (1001) docker     (123)    10412 2023-07-21 20:45:52.000000 pulumi_kubernetes-4.1.0a1689971798/pulumi_kubernetes/apps/v1/DeploymentList.py
+-rw-r--r--   0 runner    (1001) docker     (123)    16049 2023-07-21 20:45:52.000000 pulumi_kubernetes-4.1.0a1689971798/pulumi_kubernetes/apps/v1/DeploymentPatch.py
+-rw-r--r--   0 runner    (1001) docker     (123)    12580 2023-07-21 20:45:52.000000 pulumi_kubernetes-4.1.0a1689971798/pulumi_kubernetes/apps/v1/ReplicaSet.py
+-rw-r--r--   0 runner    (1001) docker     (123)    11164 2023-07-21 20:45:52.000000 pulumi_kubernetes-4.1.0a1689971798/pulumi_kubernetes/apps/v1/ReplicaSetList.py
+-rw-r--r--   0 runner    (1001) docker     (123)    14188 2023-07-21 20:45:52.000000 pulumi_kubernetes-4.1.0a1689971798/pulumi_kubernetes/apps/v1/ReplicaSetPatch.py
+-rw-r--r--   0 runner    (1001) docker     (123)    24360 2023-07-21 20:45:52.000000 pulumi_kubernetes-4.1.0a1689971798/pulumi_kubernetes/apps/v1/StatefulSet.py
+-rw-r--r--   0 runner    (1001) docker     (123)    10887 2023-07-21 20:45:52.000000 pulumi_kubernetes-4.1.0a1689971798/pulumi_kubernetes/apps/v1/StatefulSetList.py
+-rw-r--r--   0 runner    (1001) docker     (123)    15062 2023-07-21 20:45:52.000000 pulumi_kubernetes-4.1.0a1689971798/pulumi_kubernetes/apps/v1/StatefulSetPatch.py
+-rw-r--r--   0 runner    (1001) docker     (123)      743 2023-07-21 20:45:52.000000 pulumi_kubernetes-4.1.0a1689971798/pulumi_kubernetes/apps/v1/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)   177605 2023-07-21 20:45:52.000000 pulumi_kubernetes-4.1.0a1689971798/pulumi_kubernetes/apps/v1/_inputs.py
+-rw-r--r--   0 runner    (1001) docker     (123)   218849 2023-07-21 20:45:52.000000 pulumi_kubernetes-4.1.0a1689971798/pulumi_kubernetes/apps/v1/outputs.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-21 20:45:53.000000 pulumi_kubernetes-4.1.0a1689971798/pulumi_kubernetes/apps/v1beta1/
+-rw-r--r--   0 runner    (1001) docker     (123)    13246 2023-07-21 20:45:52.000000 pulumi_kubernetes-4.1.0a1689971798/pulumi_kubernetes/apps/v1beta1/ControllerRevision.py
+-rw-r--r--   0 runner    (1001) docker     (123)    11051 2023-07-21 20:45:52.000000 pulumi_kubernetes-4.1.0a1689971798/pulumi_kubernetes/apps/v1beta1/ControllerRevisionList.py
+-rw-r--r--   0 runner    (1001) docker     (123)    14788 2023-07-21 20:45:52.000000 pulumi_kubernetes-4.1.0a1689971798/pulumi_kubernetes/apps/v1beta1/ControllerRevisionPatch.py
+-rw-r--r--   0 runner    (1001) docker     (123)    14022 2023-07-21 20:45:52.000000 pulumi_kubernetes-4.1.0a1689971798/pulumi_kubernetes/apps/v1beta1/Deployment.py
+-rw-r--r--   0 runner    (1001) docker     (123)    10427 2023-07-21 20:45:52.000000 pulumi_kubernetes-4.1.0a1689971798/pulumi_kubernetes/apps/v1beta1/DeploymentList.py
+-rw-r--r--   0 runner    (1001) docker     (123)    15635 2023-07-21 20:45:52.000000 pulumi_kubernetes-4.1.0a1689971798/pulumi_kubernetes/apps/v1beta1/DeploymentPatch.py
+-rw-r--r--   0 runner    (1001) docker     (123)    12724 2023-07-21 20:45:52.000000 pulumi_kubernetes-4.1.0a1689971798/pulumi_kubernetes/apps/v1beta1/StatefulSet.py
+-rw-r--r--   0 runner    (1001) docker     (123)     9792 2023-07-21 20:45:52.000000 pulumi_kubernetes-4.1.0a1689971798/pulumi_kubernetes/apps/v1beta1/StatefulSetList.py
+-rw-r--r--   0 runner    (1001) docker     (123)    14322 2023-07-21 20:45:52.000000 pulumi_kubernetes-4.1.0a1689971798/pulumi_kubernetes/apps/v1beta1/StatefulSetPatch.py
+-rw-r--r--   0 runner    (1001) docker     (123)      572 2023-07-21 20:45:52.000000 pulumi_kubernetes-4.1.0a1689971798/pulumi_kubernetes/apps/v1beta1/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)    92195 2023-07-21 20:45:52.000000 pulumi_kubernetes-4.1.0a1689971798/pulumi_kubernetes/apps/v1beta1/_inputs.py
+-rw-r--r--   0 runner    (1001) docker     (123)   112665 2023-07-21 20:45:52.000000 pulumi_kubernetes-4.1.0a1689971798/pulumi_kubernetes/apps/v1beta1/outputs.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-21 20:45:53.000000 pulumi_kubernetes-4.1.0a1689971798/pulumi_kubernetes/apps/v1beta2/
+-rw-r--r--   0 runner    (1001) docker     (123)    13246 2023-07-21 20:45:52.000000 pulumi_kubernetes-4.1.0a1689971798/pulumi_kubernetes/apps/v1beta2/ControllerRevision.py
+-rw-r--r--   0 runner    (1001) docker     (123)    11051 2023-07-21 20:45:52.000000 pulumi_kubernetes-4.1.0a1689971798/pulumi_kubernetes/apps/v1beta2/ControllerRevisionList.py
+-rw-r--r--   0 runner    (1001) docker     (123)    14788 2023-07-21 20:45:52.000000 pulumi_kubernetes-4.1.0a1689971798/pulumi_kubernetes/apps/v1beta2/ControllerRevisionPatch.py
+-rw-r--r--   0 runner    (1001) docker     (123)    11864 2023-07-21 20:45:52.000000 pulumi_kubernetes-4.1.0a1689971798/pulumi_kubernetes/apps/v1beta2/DaemonSet.py
+-rw-r--r--   0 runner    (1001) docker     (123)    10782 2023-07-21 20:45:52.000000 pulumi_kubernetes-4.1.0a1689971798/pulumi_kubernetes/apps/v1beta2/DaemonSetList.py
+-rw-r--r--   0 runner    (1001) docker     (123)    13472 2023-07-21 20:45:52.000000 pulumi_kubernetes-4.1.0a1689971798/pulumi_kubernetes/apps/v1beta2/DaemonSetPatch.py
+-rw-r--r--   0 runner    (1001) docker     (123)    14022 2023-07-21 20:45:52.000000 pulumi_kubernetes-4.1.0a1689971798/pulumi_kubernetes/apps/v1beta2/Deployment.py
+-rw-r--r--   0 runner    (1001) docker     (123)    10427 2023-07-21 20:45:52.000000 pulumi_kubernetes-4.1.0a1689971798/pulumi_kubernetes/apps/v1beta2/DeploymentList.py
+-rw-r--r--   0 runner    (1001) docker     (123)    15635 2023-07-21 20:45:52.000000 pulumi_kubernetes-4.1.0a1689971798/pulumi_kubernetes/apps/v1beta2/DeploymentPatch.py
+-rw-r--r--   0 runner    (1001) docker     (123)    12590 2023-07-21 20:45:52.000000 pulumi_kubernetes-4.1.0a1689971798/pulumi_kubernetes/apps/v1beta2/ReplicaSet.py
+-rw-r--r--   0 runner    (1001) docker     (123)    11179 2023-07-21 20:45:52.000000 pulumi_kubernetes-4.1.0a1689971798/pulumi_kubernetes/apps/v1beta2/ReplicaSetList.py
+-rw-r--r--   0 runner    (1001) docker     (123)    14198 2023-07-21 20:45:52.000000 pulumi_kubernetes-4.1.0a1689971798/pulumi_kubernetes/apps/v1beta2/ReplicaSetPatch.py
+-rw-r--r--   0 runner    (1001) docker     (123)    12724 2023-07-21 20:45:52.000000 pulumi_kubernetes-4.1.0a1689971798/pulumi_kubernetes/apps/v1beta2/StatefulSet.py
+-rw-r--r--   0 runner    (1001) docker     (123)     9792 2023-07-21 20:45:52.000000 pulumi_kubernetes-4.1.0a1689971798/pulumi_kubernetes/apps/v1beta2/StatefulSetList.py
+-rw-r--r--   0 runner    (1001) docker     (123)    14322 2023-07-21 20:45:52.000000 pulumi_kubernetes-4.1.0a1689971798/pulumi_kubernetes/apps/v1beta2/StatefulSetPatch.py
+-rw-r--r--   0 runner    (1001) docker     (123)      743 2023-07-21 20:45:52.000000 pulumi_kubernetes-4.1.0a1689971798/pulumi_kubernetes/apps/v1beta2/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)   147337 2023-07-21 20:45:52.000000 pulumi_kubernetes-4.1.0a1689971798/pulumi_kubernetes/apps/v1beta2/_inputs.py
+-rw-r--r--   0 runner    (1001) docker     (123)   187289 2023-07-21 20:45:52.000000 pulumi_kubernetes-4.1.0a1689971798/pulumi_kubernetes/apps/v1beta2/outputs.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-21 20:45:53.000000 pulumi_kubernetes-4.1.0a1689971798/pulumi_kubernetes/auditregistration/
+-rw-r--r--   0 runner    (1001) docker     (123)      439 2023-07-21 20:45:52.000000 pulumi_kubernetes-4.1.0a1689971798/pulumi_kubernetes/auditregistration/__init__.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-21 20:45:53.000000 pulumi_kubernetes-4.1.0a1689971798/pulumi_kubernetes/auditregistration/v1alpha1/
+-rw-r--r--   0 runner    (1001) docker     (123)     9955 2023-07-21 20:45:52.000000 pulumi_kubernetes-4.1.0a1689971798/pulumi_kubernetes/auditregistration/v1alpha1/AuditSink.py
+-rw-r--r--   0 runner    (1001) docker     (123)    10119 2023-07-21 20:45:52.000000 pulumi_kubernetes-4.1.0a1689971798/pulumi_kubernetes/auditregistration/v1alpha1/AuditSinkList.py
+-rw-r--r--   0 runner    (1001) docker     (123)    11538 2023-07-21 20:45:52.000000 pulumi_kubernetes-4.1.0a1689971798/pulumi_kubernetes/auditregistration/v1alpha1/AuditSinkPatch.py
+-rw-r--r--   0 runner    (1001) docker     (123)      368 2023-07-21 20:45:52.000000 pulumi_kubernetes-4.1.0a1689971798/pulumi_kubernetes/auditregistration/v1alpha1/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)    30765 2023-07-21 20:45:52.000000 pulumi_kubernetes-4.1.0a1689971798/pulumi_kubernetes/auditregistration/v1alpha1/_inputs.py
+-rw-r--r--   0 runner    (1001) docker     (123)    28907 2023-07-21 20:45:52.000000 pulumi_kubernetes-4.1.0a1689971798/pulumi_kubernetes/auditregistration/v1alpha1/outputs.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-21 20:45:53.000000 pulumi_kubernetes-4.1.0a1689971798/pulumi_kubernetes/autoscaling/
+-rw-r--r--   0 runner    (1001) docker     (123)      853 2023-07-21 20:45:52.000000 pulumi_kubernetes-4.1.0a1689971798/pulumi_kubernetes/autoscaling/__init__.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-21 20:45:53.000000 pulumi_kubernetes-4.1.0a1689971798/pulumi_kubernetes/autoscaling/v1/
+-rw-r--r--   0 runner    (1001) docker     (123)    12143 2023-07-21 20:45:52.000000 pulumi_kubernetes-4.1.0a1689971798/pulumi_kubernetes/autoscaling/v1/HorizontalPodAutoscaler.py
+-rw-r--r--   0 runner    (1001) docker     (123)    10846 2023-07-21 20:45:52.000000 pulumi_kubernetes-4.1.0a1689971798/pulumi_kubernetes/autoscaling/v1/HorizontalPodAutoscalerList.py
+-rw-r--r--   0 runner    (1001) docker     (123)    13756 2023-07-21 20:45:52.000000 pulumi_kubernetes-4.1.0a1689971798/pulumi_kubernetes/autoscaling/v1/HorizontalPodAutoscalerPatch.py
+-rw-r--r--   0 runner    (1001) docker     (123)      410 2023-07-21 20:45:52.000000 pulumi_kubernetes-4.1.0a1689971798/pulumi_kubernetes/autoscaling/v1/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)    22804 2023-07-21 20:45:52.000000 pulumi_kubernetes-4.1.0a1689971798/pulumi_kubernetes/autoscaling/v1/_inputs.py
+-rw-r--r--   0 runner    (1001) docker     (123)    28045 2023-07-21 20:45:52.000000 pulumi_kubernetes-4.1.0a1689971798/pulumi_kubernetes/autoscaling/v1/outputs.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-21 20:45:53.000000 pulumi_kubernetes-4.1.0a1689971798/pulumi_kubernetes/autoscaling/v2/
+-rw-r--r--   0 runner    (1001) docker     (123)    12613 2023-07-21 20:45:52.000000 pulumi_kubernetes-4.1.0a1689971798/pulumi_kubernetes/autoscaling/v2/HorizontalPodAutoscaler.py
+-rw-r--r--   0 runner    (1001) docker     (123)    10976 2023-07-21 20:45:52.000000 pulumi_kubernetes-4.1.0a1689971798/pulumi_kubernetes/autoscaling/v2/HorizontalPodAutoscalerList.py
+-rw-r--r--   0 runner    (1001) docker     (123)    14226 2023-07-21 20:45:52.000000 pulumi_kubernetes-4.1.0a1689971798/pulumi_kubernetes/autoscaling/v2/HorizontalPodAutoscalerPatch.py
+-rw-r--r--   0 runner    (1001) docker     (123)      410 2023-07-21 20:45:52.000000 pulumi_kubernetes-4.1.0a1689971798/pulumi_kubernetes/autoscaling/v2/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)   109207 2023-07-21 20:45:52.000000 pulumi_kubernetes-4.1.0a1689971798/pulumi_kubernetes/autoscaling/v2/_inputs.py
+-rw-r--r--   0 runner    (1001) docker     (123)   137695 2023-07-21 20:45:52.000000 pulumi_kubernetes-4.1.0a1689971798/pulumi_kubernetes/autoscaling/v2/outputs.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-21 20:45:53.000000 pulumi_kubernetes-4.1.0a1689971798/pulumi_kubernetes/autoscaling/v2beta1/
+-rw-r--r--   0 runner    (1001) docker     (123)    12623 2023-07-21 20:45:52.000000 pulumi_kubernetes-4.1.0a1689971798/pulumi_kubernetes/autoscaling/v2beta1/HorizontalPodAutoscaler.py
+-rw-r--r--   0 runner    (1001) docker     (123)    10983 2023-07-21 20:45:52.000000 pulumi_kubernetes-4.1.0a1689971798/pulumi_kubernetes/autoscaling/v2beta1/HorizontalPodAutoscalerList.py
+-rw-r--r--   0 runner    (1001) docker     (123)    14236 2023-07-21 20:45:52.000000 pulumi_kubernetes-4.1.0a1689971798/pulumi_kubernetes/autoscaling/v2beta1/HorizontalPodAutoscalerPatch.py
+-rw-r--r--   0 runner    (1001) docker     (123)      410 2023-07-21 20:45:52.000000 pulumi_kubernetes-4.1.0a1689971798/pulumi_kubernetes/autoscaling/v2beta1/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)    99993 2023-07-21 20:45:52.000000 pulumi_kubernetes-4.1.0a1689971798/pulumi_kubernetes/autoscaling/v2beta1/_inputs.py
+-rw-r--r--   0 runner    (1001) docker     (123)   138421 2023-07-21 20:45:52.000000 pulumi_kubernetes-4.1.0a1689971798/pulumi_kubernetes/autoscaling/v2beta1/outputs.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-21 20:45:53.000000 pulumi_kubernetes-4.1.0a1689971798/pulumi_kubernetes/autoscaling/v2beta2/
+-rw-r--r--   0 runner    (1001) docker     (123)    12623 2023-07-21 20:45:52.000000 pulumi_kubernetes-4.1.0a1689971798/pulumi_kubernetes/autoscaling/v2beta2/HorizontalPodAutoscaler.py
+-rw-r--r--   0 runner    (1001) docker     (123)    10991 2023-07-21 20:45:52.000000 pulumi_kubernetes-4.1.0a1689971798/pulumi_kubernetes/autoscaling/v2beta2/HorizontalPodAutoscalerList.py
+-rw-r--r--   0 runner    (1001) docker     (123)    14236 2023-07-21 20:45:52.000000 pulumi_kubernetes-4.1.0a1689971798/pulumi_kubernetes/autoscaling/v2beta2/HorizontalPodAutoscalerPatch.py
+-rw-r--r--   0 runner    (1001) docker     (123)      410 2023-07-21 20:45:52.000000 pulumi_kubernetes-4.1.0a1689971798/pulumi_kubernetes/autoscaling/v2beta2/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)   107200 2023-07-21 20:45:52.000000 pulumi_kubernetes-4.1.0a1689971798/pulumi_kubernetes/autoscaling/v2beta2/_inputs.py
+-rw-r--r--   0 runner    (1001) docker     (123)   135212 2023-07-21 20:45:52.000000 pulumi_kubernetes-4.1.0a1689971798/pulumi_kubernetes/autoscaling/v2beta2/outputs.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-21 20:45:53.000000 pulumi_kubernetes-4.1.0a1689971798/pulumi_kubernetes/batch/
+-rw-r--r--   0 runner    (1001) docker     (123)      689 2023-07-21 20:45:52.000000 pulumi_kubernetes-4.1.0a1689971798/pulumi_kubernetes/batch/__init__.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-21 20:45:53.000000 pulumi_kubernetes-4.1.0a1689971798/pulumi_kubernetes/batch/v1/
+-rw-r--r--   0 runner    (1001) docker     (123)    11846 2023-07-21 20:45:52.000000 pulumi_kubernetes-4.1.0a1689971798/pulumi_kubernetes/batch/v1/CronJob.py
+-rw-r--r--   0 runner    (1001) docker     (123)    10740 2023-07-21 20:45:52.000000 pulumi_kubernetes-4.1.0a1689971798/pulumi_kubernetes/batch/v1/CronJobList.py
+-rw-r--r--   0 runner    (1001) docker     (123)    13454 2023-07-21 20:45:52.000000 pulumi_kubernetes-4.1.0a1689971798/pulumi_kubernetes/batch/v1/CronJobPatch.py
+-rw-r--r--   0 runner    (1001) docker     (123)    17964 2023-07-21 20:45:52.000000 pulumi_kubernetes-4.1.0a1689971798/pulumi_kubernetes/batch/v1/Job.py
+-rw-r--r--   0 runner    (1001) docker     (123)    10598 2023-07-21 20:45:52.000000 pulumi_kubernetes-4.1.0a1689971798/pulumi_kubernetes/batch/v1/JobList.py
+-rw-r--r--   0 runner    (1001) docker     (123)    15544 2023-07-21 20:45:52.000000 pulumi_kubernetes-4.1.0a1689971798/pulumi_kubernetes/batch/v1/JobPatch.py
+-rw-r--r--   0 runner    (1001) docker     (123)      428 2023-07-21 20:45:52.000000 pulumi_kubernetes-4.1.0a1689971798/pulumi_kubernetes/batch/v1/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)   107978 2023-07-21 20:45:52.000000 pulumi_kubernetes-4.1.0a1689971798/pulumi_kubernetes/batch/v1/_inputs.py
+-rw-r--r--   0 runner    (1001) docker     (123)   121425 2023-07-21 20:45:52.000000 pulumi_kubernetes-4.1.0a1689971798/pulumi_kubernetes/batch/v1/outputs.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-21 20:45:53.000000 pulumi_kubernetes-4.1.0a1689971798/pulumi_kubernetes/batch/v1beta1/
+-rw-r--r--   0 runner    (1001) docker     (123)    11888 2023-07-21 20:45:52.000000 pulumi_kubernetes-4.1.0a1689971798/pulumi_kubernetes/batch/v1beta1/CronJob.py
+-rw-r--r--   0 runner    (1001) docker     (123)    10787 2023-07-21 20:45:52.000000 pulumi_kubernetes-4.1.0a1689971798/pulumi_kubernetes/batch/v1beta1/CronJobList.py
+-rw-r--r--   0 runner    (1001) docker     (123)    13496 2023-07-21 20:45:52.000000 pulumi_kubernetes-4.1.0a1689971798/pulumi_kubernetes/batch/v1beta1/CronJobPatch.py
+-rw-r--r--   0 runner    (1001) docker     (123)      362 2023-07-21 20:45:52.000000 pulumi_kubernetes-4.1.0a1689971798/pulumi_kubernetes/batch/v1beta1/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)    23861 2023-07-21 20:45:52.000000 pulumi_kubernetes-4.1.0a1689971798/pulumi_kubernetes/batch/v1beta1/_inputs.py
+-rw-r--r--   0 runner    (1001) docker     (123)    24638 2023-07-21 20:45:52.000000 pulumi_kubernetes-4.1.0a1689971798/pulumi_kubernetes/batch/v1beta1/outputs.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-21 20:45:53.000000 pulumi_kubernetes-4.1.0a1689971798/pulumi_kubernetes/batch/v2alpha1/
+-rw-r--r--   0 runner    (1001) docker     (123)    11890 2023-07-21 20:45:52.000000 pulumi_kubernetes-4.1.0a1689971798/pulumi_kubernetes/batch/v2alpha1/CronJob.py
+-rw-r--r--   0 runner    (1001) docker     (123)    10790 2023-07-21 20:45:52.000000 pulumi_kubernetes-4.1.0a1689971798/pulumi_kubernetes/batch/v2alpha1/CronJobList.py
+-rw-r--r--   0 runner    (1001) docker     (123)    13498 2023-07-21 20:45:52.000000 pulumi_kubernetes-4.1.0a1689971798/pulumi_kubernetes/batch/v2alpha1/CronJobPatch.py
+-rw-r--r--   0 runner    (1001) docker     (123)      362 2023-07-21 20:45:52.000000 pulumi_kubernetes-4.1.0a1689971798/pulumi_kubernetes/batch/v2alpha1/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)    23742 2023-07-21 20:45:52.000000 pulumi_kubernetes-4.1.0a1689971798/pulumi_kubernetes/batch/v2alpha1/_inputs.py
+-rw-r--r--   0 runner    (1001) docker     (123)    24519 2023-07-21 20:45:52.000000 pulumi_kubernetes-4.1.0a1689971798/pulumi_kubernetes/batch/v2alpha1/outputs.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-21 20:45:53.000000 pulumi_kubernetes-4.1.0a1689971798/pulumi_kubernetes/certificates/
+-rw-r--r--   0 runner    (1001) docker     (123)      731 2023-07-21 20:45:52.000000 pulumi_kubernetes-4.1.0a1689971798/pulumi_kubernetes/certificates/__init__.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-21 20:45:53.000000 pulumi_kubernetes-4.1.0a1689971798/pulumi_kubernetes/certificates/v1/
+-rw-r--r--   0 runner    (1001) docker     (123)    13158 2023-07-21 20:45:52.000000 pulumi_kubernetes-4.1.0a1689971798/pulumi_kubernetes/certificates/v1/CertificateSigningRequest.py
+-rw-r--r--   0 runner    (1001) docker     (123)    10712 2023-07-21 20:45:52.000000 pulumi_kubernetes-4.1.0a1689971798/pulumi_kubernetes/certificates/v1/CertificateSigningRequestList.py
+-rw-r--r--   0 runner    (1001) docker     (123)    14724 2023-07-21 20:45:52.000000 pulumi_kubernetes-4.1.0a1689971798/pulumi_kubernetes/certificates/v1/CertificateSigningRequestPatch.py
+-rw-r--r--   0 runner    (1001) docker     (123)      416 2023-07-21 20:45:52.000000 pulumi_kubernetes-4.1.0a1689971798/pulumi_kubernetes/certificates/v1/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)    44481 2023-07-21 20:45:52.000000 pulumi_kubernetes-4.1.0a1689971798/pulumi_kubernetes/certificates/v1/_inputs.py
+-rw-r--r--   0 runner    (1001) docker     (123)    53207 2023-07-21 20:45:52.000000 pulumi_kubernetes-4.1.0a1689971798/pulumi_kubernetes/certificates/v1/outputs.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-21 20:45:53.000000 pulumi_kubernetes-4.1.0a1689971798/pulumi_kubernetes/certificates/v1alpha1/
+-rw-r--r--   0 runner    (1001) docker     (123)    12314 2023-07-21 20:45:52.000000 pulumi_kubernetes-4.1.0a1689971798/pulumi_kubernetes/certificates/v1alpha1/ClusterTrustBundle.py
+-rw-r--r--   0 runner    (1001) docker     (123)    10841 2023-07-21 20:45:52.000000 pulumi_kubernetes-4.1.0a1689971798/pulumi_kubernetes/certificates/v1alpha1/ClusterTrustBundleList.py
+-rw-r--r--   0 runner    (1001) docker     (123)    13880 2023-07-21 20:45:52.000000 pulumi_kubernetes-4.1.0a1689971798/pulumi_kubernetes/certificates/v1alpha1/ClusterTrustBundlePatch.py
+-rw-r--r--   0 runner    (1001) docker     (123)      395 2023-07-21 20:45:52.000000 pulumi_kubernetes-4.1.0a1689971798/pulumi_kubernetes/certificates/v1alpha1/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)    13356 2023-07-21 20:45:52.000000 pulumi_kubernetes-4.1.0a1689971798/pulumi_kubernetes/certificates/v1alpha1/_inputs.py
+-rw-r--r--   0 runner    (1001) docker     (123)    14968 2023-07-21 20:45:52.000000 pulumi_kubernetes-4.1.0a1689971798/pulumi_kubernetes/certificates/v1alpha1/outputs.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-21 20:45:53.000000 pulumi_kubernetes-4.1.0a1689971798/pulumi_kubernetes/certificates/v1beta1/
+-rw-r--r--   0 runner    (1001) docker     (123)    10967 2023-07-21 20:45:52.000000 pulumi_kubernetes-4.1.0a1689971798/pulumi_kubernetes/certificates/v1beta1/CertificateSigningRequest.py
+-rw-r--r--   0 runner    (1001) docker     (123)    10249 2023-07-21 20:45:52.000000 pulumi_kubernetes-4.1.0a1689971798/pulumi_kubernetes/certificates/v1beta1/CertificateSigningRequestList.py
+-rw-r--r--   0 runner    (1001) docker     (123)    12560 2023-07-21 20:45:52.000000 pulumi_kubernetes-4.1.0a1689971798/pulumi_kubernetes/certificates/v1beta1/CertificateSigningRequestPatch.py
+-rw-r--r--   0 runner    (1001) docker     (123)      416 2023-07-21 20:45:52.000000 pulumi_kubernetes-4.1.0a1689971798/pulumi_kubernetes/certificates/v1beta1/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)    23273 2023-07-21 20:45:52.000000 pulumi_kubernetes-4.1.0a1689971798/pulumi_kubernetes/certificates/v1beta1/_inputs.py
+-rw-r--r--   0 runner    (1001) docker     (123)    26601 2023-07-21 20:45:52.000000 pulumi_kubernetes-4.1.0a1689971798/pulumi_kubernetes/certificates/v1beta1/outputs.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-21 20:45:53.000000 pulumi_kubernetes-4.1.0a1689971798/pulumi_kubernetes/coordination/
+-rw-r--r--   0 runner    (1001) docker     (123)      559 2023-07-21 20:45:52.000000 pulumi_kubernetes-4.1.0a1689971798/pulumi_kubernetes/coordination/__init__.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-21 20:45:53.000000 pulumi_kubernetes-4.1.0a1689971798/pulumi_kubernetes/coordination/v1/
+-rw-r--r--   0 runner    (1001) docker     (123)    11052 2023-07-21 20:45:52.000000 pulumi_kubernetes-4.1.0a1689971798/pulumi_kubernetes/coordination/v1/Lease.py
+-rw-r--r--   0 runner    (1001) docker     (123)    10706 2023-07-21 20:45:52.000000 pulumi_kubernetes-4.1.0a1689971798/pulumi_kubernetes/coordination/v1/LeaseList.py
+-rw-r--r--   0 runner    (1001) docker     (123)    12650 2023-07-21 20:45:52.000000 pulumi_kubernetes-4.1.0a1689971798/pulumi_kubernetes/coordination/v1/LeasePatch.py
+-rw-r--r--   0 runner    (1001) docker     (123)      356 2023-07-21 20:45:52.000000 pulumi_kubernetes-4.1.0a1689971798/pulumi_kubernetes/coordination/v1/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)    12162 2023-07-21 20:45:52.000000 pulumi_kubernetes-4.1.0a1689971798/pulumi_kubernetes/coordination/v1/_inputs.py
+-rw-r--r--   0 runner    (1001) docker     (123)    12069 2023-07-21 20:45:52.000000 pulumi_kubernetes-4.1.0a1689971798/pulumi_kubernetes/coordination/v1/outputs.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-21 20:45:53.000000 pulumi_kubernetes-4.1.0a1689971798/pulumi_kubernetes/coordination/v1beta1/
+-rw-r--r--   0 runner    (1001) docker     (123)    10990 2023-07-21 20:45:52.000000 pulumi_kubernetes-4.1.0a1689971798/pulumi_kubernetes/coordination/v1beta1/Lease.py
+-rw-r--r--   0 runner    (1001) docker     (123)    10721 2023-07-21 20:45:52.000000 pulumi_kubernetes-4.1.0a1689971798/pulumi_kubernetes/coordination/v1beta1/LeaseList.py
+-rw-r--r--   0 runner    (1001) docker     (123)    12588 2023-07-21 20:45:52.000000 pulumi_kubernetes-4.1.0a1689971798/pulumi_kubernetes/coordination/v1beta1/LeasePatch.py
+-rw-r--r--   0 runner    (1001) docker     (123)      356 2023-07-21 20:45:52.000000 pulumi_kubernetes-4.1.0a1689971798/pulumi_kubernetes/coordination/v1beta1/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)    12131 2023-07-21 20:45:52.000000 pulumi_kubernetes-4.1.0a1689971798/pulumi_kubernetes/coordination/v1beta1/_inputs.py
+-rw-r--r--   0 runner    (1001) docker     (123)    12038 2023-07-21 20:45:52.000000 pulumi_kubernetes-4.1.0a1689971798/pulumi_kubernetes/coordination/v1beta1/outputs.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-21 20:45:53.000000 pulumi_kubernetes-4.1.0a1689971798/pulumi_kubernetes/core/
+-rw-r--r--   0 runner    (1001) docker     (123)      377 2023-07-21 20:45:52.000000 pulumi_kubernetes-4.1.0a1689971798/pulumi_kubernetes/core/__init__.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-21 20:45:53.000000 pulumi_kubernetes-4.1.0a1689971798/pulumi_kubernetes/core/v1/
+-rw-r--r--   0 runner    (1001) docker     (123)    10930 2023-07-21 20:45:52.000000 pulumi_kubernetes-4.1.0a1689971798/pulumi_kubernetes/core/v1/Binding.py
+-rw-r--r--   0 runner    (1001) docker     (123)    12530 2023-07-21 20:45:52.000000 pulumi_kubernetes-4.1.0a1689971798/pulumi_kubernetes/core/v1/BindingPatch.py
+-rw-r--r--   0 runner    (1001) docker     (123)    16018 2023-07-21 20:45:52.000000 pulumi_kubernetes-4.1.0a1689971798/pulumi_kubernetes/core/v1/ConfigMap.py
+-rw-r--r--   0 runner    (1001) docker     (123)    10715 2023-07-21 20:45:52.000000 pulumi_kubernetes-4.1.0a1689971798/pulumi_kubernetes/core/v1/ConfigMapList.py
+-rw-r--r--   0 runner    (1001) docker     (123)    17591 2023-07-21 20:45:52.000000 pulumi_kubernetes-4.1.0a1689971798/pulumi_kubernetes/core/v1/ConfigMapPatch.py
+-rw-r--r--   0 runner    (1001) docker     (123)    13511 2023-07-21 20:45:52.000000 pulumi_kubernetes-4.1.0a1689971798/pulumi_kubernetes/core/v1/Endpoints.py
+-rw-r--r--   0 runner    (1001) docker     (123)    10707 2023-07-21 20:45:52.000000 pulumi_kubernetes-4.1.0a1689971798/pulumi_kubernetes/core/v1/EndpointsList.py
+-rw-r--r--   0 runner    (1001) docker     (123)    15104 2023-07-21 20:45:52.000000 pulumi_kubernetes-4.1.0a1689971798/pulumi_kubernetes/core/v1/EndpointsPatch.py
+-rw-r--r--   0 runner    (1001) docker     (123)    28454 2023-07-21 20:45:52.000000 pulumi_kubernetes-4.1.0a1689971798/pulumi_kubernetes/core/v1/Event.py
+-rw-r--r--   0 runner    (1001) docker     (123)    10569 2023-07-21 20:45:52.000000 pulumi_kubernetes-4.1.0a1689971798/pulumi_kubernetes/core/v1/EventList.py
+-rw-r--r--   0 runner    (1001) docker     (123)    30221 2023-07-21 20:45:52.000000 pulumi_kubernetes-4.1.0a1689971798/pulumi_kubernetes/core/v1/EventPatch.py
+-rw-r--r--   0 runner    (1001) docker     (123)    11110 2023-07-21 20:45:52.000000 pulumi_kubernetes-4.1.0a1689971798/pulumi_kubernetes/core/v1/LimitRange.py
+-rw-r--r--   0 runner    (1001) docker     (123)    11190 2023-07-21 20:45:52.000000 pulumi_kubernetes-4.1.0a1689971798/pulumi_kubernetes/core/v1/LimitRangeList.py
+-rw-r--r--   0 runner    (1001) docker     (123)    12703 2023-07-21 20:45:52.000000 pulumi_kubernetes-4.1.0a1689971798/pulumi_kubernetes/core/v1/LimitRangePatch.py
+-rw-r--r--   0 runner    (1001) docker     (123)    11558 2023-07-21 20:45:52.000000 pulumi_kubernetes-4.1.0a1689971798/pulumi_kubernetes/core/v1/Namespace.py
+-rw-r--r--   0 runner    (1001) docker     (123)    11197 2023-07-21 20:45:52.000000 pulumi_kubernetes-4.1.0a1689971798/pulumi_kubernetes/core/v1/NamespaceList.py
+-rw-r--r--   0 runner    (1001) docker     (123)    13156 2023-07-21 20:45:52.000000 pulumi_kubernetes-4.1.0a1689971798/pulumi_kubernetes/core/v1/NamespacePatch.py
+-rw-r--r--   0 runner    (1001) docker     (123)    11429 2023-07-21 20:45:52.000000 pulumi_kubernetes-4.1.0a1689971798/pulumi_kubernetes/core/v1/Node.py
+-rw-r--r--   0 runner    (1001) docker     (123)    10636 2023-07-21 20:45:52.000000 pulumi_kubernetes-4.1.0a1689971798/pulumi_kubernetes/core/v1/NodeList.py
+-rw-r--r--   0 runner    (1001) docker     (123)    13027 2023-07-21 20:45:52.000000 pulumi_kubernetes-4.1.0a1689971798/pulumi_kubernetes/core/v1/NodePatch.py
+-rw-r--r--   0 runner    (1001) docker     (123)    12176 2023-07-21 20:45:52.000000 pulumi_kubernetes-4.1.0a1689971798/pulumi_kubernetes/core/v1/PersistentVolume.py
+-rw-r--r--   0 runner    (1001) docker     (123)    12008 2023-07-21 20:45:52.000000 pulumi_kubernetes-4.1.0a1689971798/pulumi_kubernetes/core/v1/PersistentVolumeClaim.py
+-rw-r--r--   0 runner    (1001) docker     (123)    11583 2023-07-21 20:45:52.000000 pulumi_kubernetes-4.1.0a1689971798/pulumi_kubernetes/core/v1/PersistentVolumeClaimList.py
+-rw-r--r--   0 runner    (1001) docker     (123)    13642 2023-07-21 20:45:52.000000 pulumi_kubernetes-4.1.0a1689971798/pulumi_kubernetes/core/v1/PersistentVolumeClaimPatch.py
+-rw-r--r--   0 runner    (1001) docker     (123)    11312 2023-07-21 20:45:52.000000 pulumi_kubernetes-4.1.0a1689971798/pulumi_kubernetes/core/v1/PersistentVolumeList.py
+-rw-r--r--   0 runner    (1001) docker     (123)    13774 2023-07-21 20:45:52.000000 pulumi_kubernetes-4.1.0a1689971798/pulumi_kubernetes/core/v1/PersistentVolumePatch.py
+-rw-r--r--   0 runner    (1001) docker     (123)    15709 2023-07-21 20:45:52.000000 pulumi_kubernetes-4.1.0a1689971798/pulumi_kubernetes/core/v1/Pod.py
+-rw-r--r--   0 runner    (1001) docker     (123)    10883 2023-07-21 20:45:52.000000 pulumi_kubernetes-4.1.0a1689971798/pulumi_kubernetes/core/v1/PodList.py
+-rw-r--r--   0 runner    (1001) docker     (123)    14961 2023-07-21 20:45:52.000000 pulumi_kubernetes-4.1.0a1689971798/pulumi_kubernetes/core/v1/PodPatch.py
+-rw-r--r--   0 runner    (1001) docker     (123)    11301 2023-07-21 20:45:52.000000 pulumi_kubernetes-4.1.0a1689971798/pulumi_kubernetes/core/v1/PodTemplate.py
+-rw-r--r--   0 runner    (1001) docker     (123)    10783 2023-07-21 20:45:52.000000 pulumi_kubernetes-4.1.0a1689971798/pulumi_kubernetes/core/v1/PodTemplateList.py
+-rw-r--r--   0 runner    (1001) docker     (123)    12894 2023-07-21 20:45:52.000000 pulumi_kubernetes-4.1.0a1689971798/pulumi_kubernetes/core/v1/PodTemplatePatch.py
+-rw-r--r--   0 runner    (1001) docker     (123)    12742 2023-07-21 20:45:52.000000 pulumi_kubernetes-4.1.0a1689971798/pulumi_kubernetes/core/v1/ReplicationController.py
+-rw-r--r--   0 runner    (1001) docker     (123)    11515 2023-07-21 20:45:52.000000 pulumi_kubernetes-4.1.0a1689971798/pulumi_kubernetes/core/v1/ReplicationControllerList.py
+-rw-r--r--   0 runner    (1001) docker     (123)    14340 2023-07-21 20:45:52.000000 pulumi_kubernetes-4.1.0a1689971798/pulumi_kubernetes/core/v1/ReplicationControllerPatch.py
+-rw-r--r--   0 runner    (1001) docker     (123)    11565 2023-07-21 20:45:52.000000 pulumi_kubernetes-4.1.0a1689971798/pulumi_kubernetes/core/v1/ResourceQuota.py
+-rw-r--r--   0 runner    (1001) docker     (123)    11219 2023-07-21 20:45:52.000000 pulumi_kubernetes-4.1.0a1689971798/pulumi_kubernetes/core/v1/ResourceQuotaList.py
+-rw-r--r--   0 runner    (1001) docker     (123)    13163 2023-07-21 20:45:52.000000 pulumi_kubernetes-4.1.0a1689971798/pulumi_kubernetes/core/v1/ResourceQuotaPatch.py
+-rw-r--r--   0 runner    (1001) docker     (123)    18698 2023-07-21 20:45:52.000000 pulumi_kubernetes-4.1.0a1689971798/pulumi_kubernetes/core/v1/Secret.py
+-rw-r--r--   0 runner    (1001) docker     (123)    10950 2023-07-21 20:45:52.000000 pulumi_kubernetes-4.1.0a1689971798/pulumi_kubernetes/core/v1/SecretList.py
+-rw-r--r--   0 runner    (1001) docker     (123)    20020 2023-07-21 20:45:52.000000 pulumi_kubernetes-4.1.0a1689971798/pulumi_kubernetes/core/v1/SecretPatch.py
+-rw-r--r--   0 runner    (1001) docker     (123)    17132 2023-07-21 20:45:52.000000 pulumi_kubernetes-4.1.0a1689971798/pulumi_kubernetes/core/v1/Service.py
+-rw-r--r--   0 runner    (1001) docker     (123)    18490 2023-07-21 20:45:52.000000 pulumi_kubernetes-4.1.0a1689971798/pulumi_kubernetes/core/v1/ServiceAccount.py
+-rw-r--r--   0 runner    (1001) docker     (123)    11280 2023-07-21 20:45:52.000000 pulumi_kubernetes-4.1.0a1689971798/pulumi_kubernetes/core/v1/ServiceAccountList.py
+-rw-r--r--   0 runner    (1001) docker     (123)    20143 2023-07-21 20:45:52.000000 pulumi_kubernetes-4.1.0a1689971798/pulumi_kubernetes/core/v1/ServiceAccountPatch.py
+-rw-r--r--   0 runner    (1001) docker     (123)    10667 2023-07-21 20:45:52.000000 pulumi_kubernetes-4.1.0a1689971798/pulumi_kubernetes/core/v1/ServiceList.py
+-rw-r--r--   0 runner    (1001) docker     (123)    16406 2023-07-21 20:45:52.000000 pulumi_kubernetes-4.1.0a1689971798/pulumi_kubernetes/core/v1/ServicePatch.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1686 2023-07-21 20:45:52.000000 pulumi_kubernetes-4.1.0a1689971798/pulumi_kubernetes/core/v1/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)      376 2023-07-21 20:45:52.000000 pulumi_kubernetes-4.1.0a1689971798/pulumi_kubernetes/core/v1/_enums.py
+-rw-r--r--   0 runner    (1001) docker     (123)  1507480 2023-07-21 20:45:52.000000 pulumi_kubernetes-4.1.0a1689971798/pulumi_kubernetes/core/v1/_inputs.py
+-rw-r--r--   0 runner    (1001) docker     (123)  1546761 2023-07-21 20:45:52.000000 pulumi_kubernetes-4.1.0a1689971798/pulumi_kubernetes/core/v1/outputs.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-21 20:45:53.000000 pulumi_kubernetes-4.1.0a1689971798/pulumi_kubernetes/discovery/
+-rw-r--r--   0 runner    (1001) docker     (123)      547 2023-07-21 20:45:52.000000 pulumi_kubernetes-4.1.0a1689971798/pulumi_kubernetes/discovery/__init__.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-21 20:45:53.000000 pulumi_kubernetes-4.1.0a1689971798/pulumi_kubernetes/discovery/v1/
+-rw-r--r--   0 runner    (1001) docker     (123)    16252 2023-07-21 20:45:52.000000 pulumi_kubernetes-4.1.0a1689971798/pulumi_kubernetes/discovery/v1/EndpointSlice.py
+-rw-r--r--   0 runner    (1001) docker     (123)    10569 2023-07-21 20:45:52.000000 pulumi_kubernetes-4.1.0a1689971798/pulumi_kubernetes/discovery/v1/EndpointSliceList.py
+-rw-r--r--   0 runner    (1001) docker     (123)    17826 2023-07-21 20:45:52.000000 pulumi_kubernetes-4.1.0a1689971798/pulumi_kubernetes/discovery/v1/EndpointSlicePatch.py
+-rw-r--r--   0 runner    (1001) docker     (123)      380 2023-07-21 20:45:52.000000 pulumi_kubernetes-4.1.0a1689971798/pulumi_kubernetes/discovery/v1/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)    42431 2023-07-21 20:45:52.000000 pulumi_kubernetes-4.1.0a1689971798/pulumi_kubernetes/discovery/v1/_inputs.py
+-rw-r--r--   0 runner    (1001) docker     (123)    40504 2023-07-21 20:45:52.000000 pulumi_kubernetes-4.1.0a1689971798/pulumi_kubernetes/discovery/v1/outputs.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-21 20:45:53.000000 pulumi_kubernetes-4.1.0a1689971798/pulumi_kubernetes/discovery/v1beta1/
+-rw-r--r--   0 runner    (1001) docker     (123)    16262 2023-07-21 20:45:52.000000 pulumi_kubernetes-4.1.0a1689971798/pulumi_kubernetes/discovery/v1beta1/EndpointSlice.py
+-rw-r--r--   0 runner    (1001) docker     (123)    10532 2023-07-21 20:45:52.000000 pulumi_kubernetes-4.1.0a1689971798/pulumi_kubernetes/discovery/v1beta1/EndpointSliceList.py
+-rw-r--r--   0 runner    (1001) docker     (123)    17836 2023-07-21 20:45:52.000000 pulumi_kubernetes-4.1.0a1689971798/pulumi_kubernetes/discovery/v1beta1/EndpointSlicePatch.py
+-rw-r--r--   0 runner    (1001) docker     (123)      380 2023-07-21 20:45:52.000000 pulumi_kubernetes-4.1.0a1689971798/pulumi_kubernetes/discovery/v1beta1/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)    35598 2023-07-21 20:45:52.000000 pulumi_kubernetes-4.1.0a1689971798/pulumi_kubernetes/discovery/v1beta1/_inputs.py
+-rw-r--r--   0 runner    (1001) docker     (123)    33494 2023-07-21 20:45:52.000000 pulumi_kubernetes-4.1.0a1689971798/pulumi_kubernetes/discovery/v1beta1/outputs.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-21 20:45:53.000000 pulumi_kubernetes-4.1.0a1689971798/pulumi_kubernetes/events/
+-rw-r--r--   0 runner    (1001) docker     (123)      535 2023-07-21 20:45:52.000000 pulumi_kubernetes-4.1.0a1689971798/pulumi_kubernetes/events/__init__.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-21 20:45:53.000000 pulumi_kubernetes-4.1.0a1689971798/pulumi_kubernetes/events/v1/
+-rw-r--r--   0 runner    (1001) docker     (123)    33307 2023-07-21 20:45:52.000000 pulumi_kubernetes-4.1.0a1689971798/pulumi_kubernetes/events/v1/Event.py
+-rw-r--r--   0 runner    (1001) docker     (123)    10718 2023-07-21 20:45:52.000000 pulumi_kubernetes-4.1.0a1689971798/pulumi_kubernetes/events/v1/EventList.py
+-rw-r--r--   0 runner    (1001) docker     (123)    35127 2023-07-21 20:45:52.000000 pulumi_kubernetes-4.1.0a1689971798/pulumi_kubernetes/events/v1/EventPatch.py
+-rw-r--r--   0 runner    (1001) docker     (123)      356 2023-07-21 20:45:52.000000 pulumi_kubernetes-4.1.0a1689971798/pulumi_kubernetes/events/v1/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)    19318 2023-07-21 20:45:52.000000 pulumi_kubernetes-4.1.0a1689971798/pulumi_kubernetes/events/v1/_inputs.py
+-rw-r--r--   0 runner    (1001) docker     (123)    19050 2023-07-21 20:45:52.000000 pulumi_kubernetes-4.1.0a1689971798/pulumi_kubernetes/events/v1/outputs.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-21 20:45:53.000000 pulumi_kubernetes-4.1.0a1689971798/pulumi_kubernetes/events/v1beta1/
+-rw-r--r--   0 runner    (1001) docker     (123)    29243 2023-07-21 20:45:52.000000 pulumi_kubernetes-4.1.0a1689971798/pulumi_kubernetes/events/v1beta1/Event.py
+-rw-r--r--   0 runner    (1001) docker     (123)    10733 2023-07-21 20:45:52.000000 pulumi_kubernetes-4.1.0a1689971798/pulumi_kubernetes/events/v1beta1/EventList.py
+-rw-r--r--   0 runner    (1001) docker     (123)    31053 2023-07-21 20:45:52.000000 pulumi_kubernetes-4.1.0a1689971798/pulumi_kubernetes/events/v1beta1/EventPatch.py
+-rw-r--r--   0 runner    (1001) docker     (123)      356 2023-07-21 20:45:52.000000 pulumi_kubernetes-4.1.0a1689971798/pulumi_kubernetes/events/v1beta1/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)    17860 2023-07-21 20:45:52.000000 pulumi_kubernetes-4.1.0a1689971798/pulumi_kubernetes/events/v1beta1/_inputs.py
+-rw-r--r--   0 runner    (1001) docker     (123)    16467 2023-07-21 20:45:52.000000 pulumi_kubernetes-4.1.0a1689971798/pulumi_kubernetes/events/v1beta1/outputs.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-21 20:45:53.000000 pulumi_kubernetes-4.1.0a1689971798/pulumi_kubernetes/extensions/
+-rw-r--r--   0 runner    (1001) docker     (123)      419 2023-07-21 20:45:52.000000 pulumi_kubernetes-4.1.0a1689971798/pulumi_kubernetes/extensions/__init__.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-21 20:45:53.000000 pulumi_kubernetes-4.1.0a1689971798/pulumi_kubernetes/extensions/v1beta1/
+-rw-r--r--   0 runner    (1001) docker     (123)    11876 2023-07-21 20:45:52.000000 pulumi_kubernetes-4.1.0a1689971798/pulumi_kubernetes/extensions/v1beta1/DaemonSet.py
+-rw-r--r--   0 runner    (1001) docker     (123)    10800 2023-07-21 20:45:52.000000 pulumi_kubernetes-4.1.0a1689971798/pulumi_kubernetes/extensions/v1beta1/DaemonSetList.py
+-rw-r--r--   0 runner    (1001) docker     (123)    13484 2023-07-21 20:45:52.000000 pulumi_kubernetes-4.1.0a1689971798/pulumi_kubernetes/extensions/v1beta1/DaemonSetPatch.py
+-rw-r--r--   0 runner    (1001) docker     (123)    14034 2023-07-21 20:45:52.000000 pulumi_kubernetes-4.1.0a1689971798/pulumi_kubernetes/extensions/v1beta1/Deployment.py
+-rw-r--r--   0 runner    (1001) docker     (123)    10445 2023-07-21 20:45:52.000000 pulumi_kubernetes-4.1.0a1689971798/pulumi_kubernetes/extensions/v1beta1/DeploymentList.py
+-rw-r--r--   0 runner    (1001) docker     (123)    15647 2023-07-21 20:45:52.000000 pulumi_kubernetes-4.1.0a1689971798/pulumi_kubernetes/extensions/v1beta1/DeploymentPatch.py
+-rw-r--r--   0 runner    (1001) docker     (123)    13728 2023-07-21 20:45:52.000000 pulumi_kubernetes-4.1.0a1689971798/pulumi_kubernetes/extensions/v1beta1/Ingress.py
+-rw-r--r--   0 runner    (1001) docker     (123)    10778 2023-07-21 20:45:52.000000 pulumi_kubernetes-4.1.0a1689971798/pulumi_kubernetes/extensions/v1beta1/IngressList.py
+-rw-r--r--   0 runner    (1001) docker     (123)    15336 2023-07-21 20:45:52.000000 pulumi_kubernetes-4.1.0a1689971798/pulumi_kubernetes/extensions/v1beta1/IngressPatch.py
+-rw-r--r--   0 runner    (1001) docker     (123)    11273 2023-07-21 20:45:52.000000 pulumi_kubernetes-4.1.0a1689971798/pulumi_kubernetes/extensions/v1beta1/NetworkPolicy.py
+-rw-r--r--   0 runner    (1001) docker     (123)    11160 2023-07-21 20:45:52.000000 pulumi_kubernetes-4.1.0a1689971798/pulumi_kubernetes/extensions/v1beta1/NetworkPolicyList.py
+-rw-r--r--   0 runner    (1001) docker     (123)    12871 2023-07-21 20:45:52.000000 pulumi_kubernetes-4.1.0a1689971798/pulumi_kubernetes/extensions/v1beta1/NetworkPolicyPatch.py
+-rw-r--r--   0 runner    (1001) docker     (123)    11347 2023-07-21 20:45:52.000000 pulumi_kubernetes-4.1.0a1689971798/pulumi_kubernetes/extensions/v1beta1/PodSecurityPolicy.py
+-rw-r--r--   0 runner    (1001) docker     (123)    11234 2023-07-21 20:45:52.000000 pulumi_kubernetes-4.1.0a1689971798/pulumi_kubernetes/extensions/v1beta1/PodSecurityPolicyList.py
+-rw-r--r--   0 runner    (1001) docker     (123)    12945 2023-07-21 20:45:52.000000 pulumi_kubernetes-4.1.0a1689971798/pulumi_kubernetes/extensions/v1beta1/PodSecurityPolicyPatch.py
+-rw-r--r--   0 runner    (1001) docker     (123)    12602 2023-07-21 20:45:52.000000 pulumi_kubernetes-4.1.0a1689971798/pulumi_kubernetes/extensions/v1beta1/ReplicaSet.py
+-rw-r--r--   0 runner    (1001) docker     (123)    11197 2023-07-21 20:45:52.000000 pulumi_kubernetes-4.1.0a1689971798/pulumi_kubernetes/extensions/v1beta1/ReplicaSetList.py
+-rw-r--r--   0 runner    (1001) docker     (123)    14210 2023-07-21 20:45:52.000000 pulumi_kubernetes-4.1.0a1689971798/pulumi_kubernetes/extensions/v1beta1/ReplicaSetPatch.py
+-rw-r--r--   0 runner    (1001) docker     (123)      824 2023-07-21 20:45:52.000000 pulumi_kubernetes-4.1.0a1689971798/pulumi_kubernetes/extensions/v1beta1/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)   288488 2023-07-21 20:45:52.000000 pulumi_kubernetes-4.1.0a1689971798/pulumi_kubernetes/extensions/v1beta1/_inputs.py
+-rw-r--r--   0 runner    (1001) docker     (123)   316040 2023-07-21 20:45:52.000000 pulumi_kubernetes-4.1.0a1689971798/pulumi_kubernetes/extensions/v1beta1/outputs.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-21 20:45:53.000000 pulumi_kubernetes-4.1.0a1689971798/pulumi_kubernetes/flowcontrol/
+-rw-r--r--   0 runner    (1001) docker     (123)      919 2023-07-21 20:45:52.000000 pulumi_kubernetes-4.1.0a1689971798/pulumi_kubernetes/flowcontrol/__init__.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-21 20:45:53.000000 pulumi_kubernetes-4.1.0a1689971798/pulumi_kubernetes/flowcontrol/v1alpha1/
+-rw-r--r--   0 runner    (1001) docker     (123)    12522 2023-07-21 20:45:52.000000 pulumi_kubernetes-4.1.0a1689971798/pulumi_kubernetes/flowcontrol/v1alpha1/FlowSchema.py
+-rw-r--r--   0 runner    (1001) docker     (123)    10974 2023-07-21 20:45:52.000000 pulumi_kubernetes-4.1.0a1689971798/pulumi_kubernetes/flowcontrol/v1alpha1/FlowSchemaList.py
+-rw-r--r--   0 runner    (1001) docker     (123)    14135 2023-07-21 20:45:52.000000 pulumi_kubernetes-4.1.0a1689971798/pulumi_kubernetes/flowcontrol/v1alpha1/FlowSchemaPatch.py
+-rw-r--r--   0 runner    (1001) docker     (123)    12750 2023-07-21 20:45:52.000000 pulumi_kubernetes-4.1.0a1689971798/pulumi_kubernetes/flowcontrol/v1alpha1/PriorityLevelConfiguration.py
+-rw-r--r--   0 runner    (1001) docker     (123)    11514 2023-07-21 20:45:52.000000 pulumi_kubernetes-4.1.0a1689971798/pulumi_kubernetes/flowcontrol/v1alpha1/PriorityLevelConfigurationList.py
+-rw-r--r--   0 runner    (1001) docker     (123)    14363 2023-07-21 20:45:52.000000 pulumi_kubernetes-4.1.0a1689971798/pulumi_kubernetes/flowcontrol/v1alpha1/PriorityLevelConfigurationPatch.py
+-rw-r--r--   0 runner    (1001) docker     (123)      506 2023-07-21 20:45:52.000000 pulumi_kubernetes-4.1.0a1689971798/pulumi_kubernetes/flowcontrol/v1alpha1/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)    93706 2023-07-21 20:45:52.000000 pulumi_kubernetes-4.1.0a1689971798/pulumi_kubernetes/flowcontrol/v1alpha1/_inputs.py
+-rw-r--r--   0 runner    (1001) docker     (123)   102811 2023-07-21 20:45:52.000000 pulumi_kubernetes-4.1.0a1689971798/pulumi_kubernetes/flowcontrol/v1alpha1/outputs.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-21 20:45:53.000000 pulumi_kubernetes-4.1.0a1689971798/pulumi_kubernetes/flowcontrol/v1beta1/
+-rw-r--r--   0 runner    (1001) docker     (123)    12520 2023-07-21 20:45:52.000000 pulumi_kubernetes-4.1.0a1689971798/pulumi_kubernetes/flowcontrol/v1beta1/FlowSchema.py
+-rw-r--r--   0 runner    (1001) docker     (123)    10971 2023-07-21 20:45:52.000000 pulumi_kubernetes-4.1.0a1689971798/pulumi_kubernetes/flowcontrol/v1beta1/FlowSchemaList.py
+-rw-r--r--   0 runner    (1001) docker     (123)    14133 2023-07-21 20:45:52.000000 pulumi_kubernetes-4.1.0a1689971798/pulumi_kubernetes/flowcontrol/v1beta1/FlowSchemaPatch.py
+-rw-r--r--   0 runner    (1001) docker     (123)    12748 2023-07-21 20:45:52.000000 pulumi_kubernetes-4.1.0a1689971798/pulumi_kubernetes/flowcontrol/v1beta1/PriorityLevelConfiguration.py
+-rw-r--r--   0 runner    (1001) docker     (123)    11511 2023-07-21 20:45:52.000000 pulumi_kubernetes-4.1.0a1689971798/pulumi_kubernetes/flowcontrol/v1beta1/PriorityLevelConfigurationList.py
+-rw-r--r--   0 runner    (1001) docker     (123)    14361 2023-07-21 20:45:52.000000 pulumi_kubernetes-4.1.0a1689971798/pulumi_kubernetes/flowcontrol/v1beta1/PriorityLevelConfigurationPatch.py
+-rw-r--r--   0 runner    (1001) docker     (123)      506 2023-07-21 20:45:52.000000 pulumi_kubernetes-4.1.0a1689971798/pulumi_kubernetes/flowcontrol/v1beta1/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)    93700 2023-07-21 20:45:52.000000 pulumi_kubernetes-4.1.0a1689971798/pulumi_kubernetes/flowcontrol/v1beta1/_inputs.py
+-rw-r--r--   0 runner    (1001) docker     (123)   102805 2023-07-21 20:45:52.000000 pulumi_kubernetes-4.1.0a1689971798/pulumi_kubernetes/flowcontrol/v1beta1/outputs.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-21 20:45:53.000000 pulumi_kubernetes-4.1.0a1689971798/pulumi_kubernetes/flowcontrol/v1beta2/
+-rw-r--r--   0 runner    (1001) docker     (123)    12520 2023-07-21 20:45:52.000000 pulumi_kubernetes-4.1.0a1689971798/pulumi_kubernetes/flowcontrol/v1beta2/FlowSchema.py
+-rw-r--r--   0 runner    (1001) docker     (123)    10971 2023-07-21 20:45:52.000000 pulumi_kubernetes-4.1.0a1689971798/pulumi_kubernetes/flowcontrol/v1beta2/FlowSchemaList.py
+-rw-r--r--   0 runner    (1001) docker     (123)    14133 2023-07-21 20:45:52.000000 pulumi_kubernetes-4.1.0a1689971798/pulumi_kubernetes/flowcontrol/v1beta2/FlowSchemaPatch.py
+-rw-r--r--   0 runner    (1001) docker     (123)    12748 2023-07-21 20:45:52.000000 pulumi_kubernetes-4.1.0a1689971798/pulumi_kubernetes/flowcontrol/v1beta2/PriorityLevelConfiguration.py
+-rw-r--r--   0 runner    (1001) docker     (123)    11511 2023-07-21 20:45:52.000000 pulumi_kubernetes-4.1.0a1689971798/pulumi_kubernetes/flowcontrol/v1beta2/PriorityLevelConfigurationList.py
+-rw-r--r--   0 runner    (1001) docker     (123)    14361 2023-07-21 20:45:52.000000 pulumi_kubernetes-4.1.0a1689971798/pulumi_kubernetes/flowcontrol/v1beta2/PriorityLevelConfigurationPatch.py
+-rw-r--r--   0 runner    (1001) docker     (123)      506 2023-07-21 20:45:52.000000 pulumi_kubernetes-4.1.0a1689971798/pulumi_kubernetes/flowcontrol/v1beta2/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)   102903 2023-07-21 20:45:52.000000 pulumi_kubernetes-4.1.0a1689971798/pulumi_kubernetes/flowcontrol/v1beta2/_inputs.py
+-rw-r--r--   0 runner    (1001) docker     (123)   111784 2023-07-21 20:45:52.000000 pulumi_kubernetes-4.1.0a1689971798/pulumi_kubernetes/flowcontrol/v1beta2/outputs.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-21 20:45:53.000000 pulumi_kubernetes-4.1.0a1689971798/pulumi_kubernetes/flowcontrol/v1beta3/
+-rw-r--r--   0 runner    (1001) docker     (123)    12520 2023-07-21 20:45:52.000000 pulumi_kubernetes-4.1.0a1689971798/pulumi_kubernetes/flowcontrol/v1beta3/FlowSchema.py
+-rw-r--r--   0 runner    (1001) docker     (123)    10971 2023-07-21 20:45:52.000000 pulumi_kubernetes-4.1.0a1689971798/pulumi_kubernetes/flowcontrol/v1beta3/FlowSchemaList.py
+-rw-r--r--   0 runner    (1001) docker     (123)    14133 2023-07-21 20:45:52.000000 pulumi_kubernetes-4.1.0a1689971798/pulumi_kubernetes/flowcontrol/v1beta3/FlowSchemaPatch.py
+-rw-r--r--   0 runner    (1001) docker     (123)    12748 2023-07-21 20:45:52.000000 pulumi_kubernetes-4.1.0a1689971798/pulumi_kubernetes/flowcontrol/v1beta3/PriorityLevelConfiguration.py
+-rw-r--r--   0 runner    (1001) docker     (123)    11511 2023-07-21 20:45:52.000000 pulumi_kubernetes-4.1.0a1689971798/pulumi_kubernetes/flowcontrol/v1beta3/PriorityLevelConfigurationList.py
+-rw-r--r--   0 runner    (1001) docker     (123)    14361 2023-07-21 20:45:52.000000 pulumi_kubernetes-4.1.0a1689971798/pulumi_kubernetes/flowcontrol/v1beta3/PriorityLevelConfigurationPatch.py
+-rw-r--r--   0 runner    (1001) docker     (123)      506 2023-07-21 20:45:52.000000 pulumi_kubernetes-4.1.0a1689971798/pulumi_kubernetes/flowcontrol/v1beta3/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)   102963 2023-07-21 20:45:52.000000 pulumi_kubernetes-4.1.0a1689971798/pulumi_kubernetes/flowcontrol/v1beta3/_inputs.py
+-rw-r--r--   0 runner    (1001) docker     (123)   111844 2023-07-21 20:45:52.000000 pulumi_kubernetes-4.1.0a1689971798/pulumi_kubernetes/flowcontrol/v1beta3/outputs.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-21 20:45:53.000000 pulumi_kubernetes-4.1.0a1689971798/pulumi_kubernetes/helm/
+-rw-r--r--   0 runner    (1001) docker     (123)      377 2023-07-21 20:45:52.000000 pulumi_kubernetes-4.1.0a1689971798/pulumi_kubernetes/helm/__init__.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-21 20:45:53.000000 pulumi_kubernetes-4.1.0a1689971798/pulumi_kubernetes/helm/v3/
+-rw-r--r--   0 runner    (1001) docker     (123)    60748 2023-07-21 20:45:52.000000 pulumi_kubernetes-4.1.0a1689971798/pulumi_kubernetes/helm/v3/Release.py
+-rw-r--r--   0 runner    (1001) docker     (123)      327 2023-07-21 20:45:52.000000 pulumi_kubernetes-4.1.0a1689971798/pulumi_kubernetes/helm/v3/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)     3999 2023-07-21 20:45:52.000000 pulumi_kubernetes-4.1.0a1689971798/pulumi_kubernetes/helm/v3/_inputs.py
+-rw-r--r--   0 runner    (1001) docker     (123)    26887 2023-07-21 20:45:52.000000 pulumi_kubernetes-4.1.0a1689971798/pulumi_kubernetes/helm/v3/helm.py
+-rw-r--r--   0 runner    (1001) docker     (123)     7187 2023-07-21 20:45:52.000000 pulumi_kubernetes-4.1.0a1689971798/pulumi_kubernetes/helm/v3/outputs.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-21 20:45:53.000000 pulumi_kubernetes-4.1.0a1689971798/pulumi_kubernetes/kustomize/
+-rw-r--r--   0 runner    (1001) docker     (123)      263 2023-07-21 20:45:52.000000 pulumi_kubernetes-4.1.0a1689971798/pulumi_kubernetes/kustomize/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)     6818 2023-07-21 20:45:52.000000 pulumi_kubernetes-4.1.0a1689971798/pulumi_kubernetes/kustomize/kustomize.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-21 20:45:53.000000 pulumi_kubernetes-4.1.0a1689971798/pulumi_kubernetes/meta/
+-rw-r--r--   0 runner    (1001) docker     (123)      377 2023-07-21 20:45:52.000000 pulumi_kubernetes-4.1.0a1689971798/pulumi_kubernetes/meta/__init__.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-21 20:45:53.000000 pulumi_kubernetes-4.1.0a1689971798/pulumi_kubernetes/meta/v1/
+-rw-r--r--   0 runner    (1001) docker     (123)    15520 2023-07-21 20:45:52.000000 pulumi_kubernetes-4.1.0a1689971798/pulumi_kubernetes/meta/v1/Status.py
+-rw-r--r--   0 runner    (1001) docker     (123)    17179 2023-07-21 20:45:52.000000 pulumi_kubernetes-4.1.0a1689971798/pulumi_kubernetes/meta/v1/StatusPatch.py
+-rw-r--r--   0 runner    (1001) docker     (123)      333 2023-07-21 20:45:52.000000 pulumi_kubernetes-4.1.0a1689971798/pulumi_kubernetes/meta/v1/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)   115603 2023-07-21 20:45:52.000000 pulumi_kubernetes-4.1.0a1689971798/pulumi_kubernetes/meta/v1/_inputs.py
+-rw-r--r--   0 runner    (1001) docker     (123)   115305 2023-07-21 20:45:52.000000 pulumi_kubernetes-4.1.0a1689971798/pulumi_kubernetes/meta/v1/outputs.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-21 20:45:53.000000 pulumi_kubernetes-4.1.0a1689971798/pulumi_kubernetes/networking/
+-rw-r--r--   0 runner    (1001) docker     (123)      719 2023-07-21 20:45:52.000000 pulumi_kubernetes-4.1.0a1689971798/pulumi_kubernetes/networking/__init__.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-21 20:45:53.000000 pulumi_kubernetes-4.1.0a1689971798/pulumi_kubernetes/networking/v1/
+-rw-r--r--   0 runner    (1001) docker     (123)    19184 2023-07-21 20:45:52.000000 pulumi_kubernetes-4.1.0a1689971798/pulumi_kubernetes/networking/v1/Ingress.py
+-rw-r--r--   0 runner    (1001) docker     (123)    12038 2023-07-21 20:45:52.000000 pulumi_kubernetes-4.1.0a1689971798/pulumi_kubernetes/networking/v1/IngressClass.py
+-rw-r--r--   0 runner    (1001) docker     (123)    10509 2023-07-21 20:45:52.000000 pulumi_kubernetes-4.1.0a1689971798/pulumi_kubernetes/networking/v1/IngressClassList.py
+-rw-r--r--   0 runner    (1001) docker     (123)    13636 2023-07-21 20:45:52.000000 pulumi_kubernetes-4.1.0a1689971798/pulumi_kubernetes/networking/v1/IngressClassPatch.py
+-rw-r--r--   0 runner    (1001) docker     (123)    10784 2023-07-21 20:45:52.000000 pulumi_kubernetes-4.1.0a1689971798/pulumi_kubernetes/networking/v1/IngressList.py
+-rw-r--r--   0 runner    (1001) docker     (123)    15340 2023-07-21 20:45:52.000000 pulumi_kubernetes-4.1.0a1689971798/pulumi_kubernetes/networking/v1/IngressPatch.py
+-rw-r--r--   0 runner    (1001) docker     (123)    11608 2023-07-21 20:45:52.000000 pulumi_kubernetes-4.1.0a1689971798/pulumi_kubernetes/networking/v1/NetworkPolicy.py
+-rw-r--r--   0 runner    (1001) docker     (123)    10948 2023-07-21 20:45:52.000000 pulumi_kubernetes-4.1.0a1689971798/pulumi_kubernetes/networking/v1/NetworkPolicyList.py
+-rw-r--r--   0 runner    (1001) docker     (123)    13211 2023-07-21 20:45:52.000000 pulumi_kubernetes-4.1.0a1689971798/pulumi_kubernetes/networking/v1/NetworkPolicyPatch.py
+-rw-r--r--   0 runner    (1001) docker     (123)      551 2023-07-21 20:45:52.000000 pulumi_kubernetes-4.1.0a1689971798/pulumi_kubernetes/networking/v1/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)   126779 2023-07-21 20:45:52.000000 pulumi_kubernetes-4.1.0a1689971798/pulumi_kubernetes/networking/v1/_inputs.py
+-rw-r--r--   0 runner    (1001) docker     (123)   133959 2023-07-21 20:45:52.000000 pulumi_kubernetes-4.1.0a1689971798/pulumi_kubernetes/networking/v1/outputs.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-21 20:45:53.000000 pulumi_kubernetes-4.1.0a1689971798/pulumi_kubernetes/networking/v1alpha1/
+-rw-r--r--   0 runner    (1001) docker     (123)    12370 2023-07-21 20:45:52.000000 pulumi_kubernetes-4.1.0a1689971798/pulumi_kubernetes/networking/v1alpha1/ClusterCIDR.py
+-rw-r--r--   0 runner    (1001) docker     (123)    10946 2023-07-21 20:45:52.000000 pulumi_kubernetes-4.1.0a1689971798/pulumi_kubernetes/networking/v1alpha1/ClusterCIDRList.py
+-rw-r--r--   0 runner    (1001) docker     (123)    13963 2023-07-21 20:45:52.000000 pulumi_kubernetes-4.1.0a1689971798/pulumi_kubernetes/networking/v1alpha1/ClusterCIDRPatch.py
+-rw-r--r--   0 runner    (1001) docker     (123)    12226 2023-07-21 20:45:52.000000 pulumi_kubernetes-4.1.0a1689971798/pulumi_kubernetes/networking/v1alpha1/IPAddress.py
+-rw-r--r--   0 runner    (1001) docker     (123)    10850 2023-07-21 20:45:52.000000 pulumi_kubernetes-4.1.0a1689971798/pulumi_kubernetes/networking/v1alpha1/IPAddressList.py
+-rw-r--r--   0 runner    (1001) docker     (123)    13819 2023-07-21 20:45:52.000000 pulumi_kubernetes-4.1.0a1689971798/pulumi_kubernetes/networking/v1alpha1/IPAddressPatch.py
+-rw-r--r--   0 runner    (1001) docker     (123)      458 2023-07-21 20:45:52.000000 pulumi_kubernetes-4.1.0a1689971798/pulumi_kubernetes/networking/v1alpha1/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)    25728 2023-07-21 20:45:52.000000 pulumi_kubernetes-4.1.0a1689971798/pulumi_kubernetes/networking/v1alpha1/_inputs.py
+-rw-r--r--   0 runner    (1001) docker     (123)    26254 2023-07-21 20:45:52.000000 pulumi_kubernetes-4.1.0a1689971798/pulumi_kubernetes/networking/v1alpha1/outputs.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-21 20:45:53.000000 pulumi_kubernetes-4.1.0a1689971798/pulumi_kubernetes/networking/v1beta1/
+-rw-r--r--   0 runner    (1001) docker     (123)    13742 2023-07-21 20:45:52.000000 pulumi_kubernetes-4.1.0a1689971798/pulumi_kubernetes/networking/v1beta1/Ingress.py
+-rw-r--r--   0 runner    (1001) docker     (123)    12078 2023-07-21 20:45:52.000000 pulumi_kubernetes-4.1.0a1689971798/pulumi_kubernetes/networking/v1beta1/IngressClass.py
+-rw-r--r--   0 runner    (1001) docker     (123)    10554 2023-07-21 20:45:52.000000 pulumi_kubernetes-4.1.0a1689971798/pulumi_kubernetes/networking/v1beta1/IngressClassList.py
+-rw-r--r--   0 runner    (1001) docker     (123)    13676 2023-07-21 20:45:52.000000 pulumi_kubernetes-4.1.0a1689971798/pulumi_kubernetes/networking/v1beta1/IngressClassPatch.py
+-rw-r--r--   0 runner    (1001) docker     (123)    10799 2023-07-21 20:45:52.000000 pulumi_kubernetes-4.1.0a1689971798/pulumi_kubernetes/networking/v1beta1/IngressList.py
+-rw-r--r--   0 runner    (1001) docker     (123)    15350 2023-07-21 20:45:52.000000 pulumi_kubernetes-4.1.0a1689971798/pulumi_kubernetes/networking/v1beta1/IngressPatch.py
+-rw-r--r--   0 runner    (1001) docker     (123)      455 2023-07-21 20:45:52.000000 pulumi_kubernetes-4.1.0a1689971798/pulumi_kubernetes/networking/v1beta1/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)    54059 2023-07-21 20:45:52.000000 pulumi_kubernetes-4.1.0a1689971798/pulumi_kubernetes/networking/v1beta1/_inputs.py
+-rw-r--r--   0 runner    (1001) docker     (123)    57257 2023-07-21 20:45:52.000000 pulumi_kubernetes-4.1.0a1689971798/pulumi_kubernetes/networking/v1beta1/outputs.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-21 20:45:53.000000 pulumi_kubernetes-4.1.0a1689971798/pulumi_kubernetes/node/
+-rw-r--r--   0 runner    (1001) docker     (123)      683 2023-07-21 20:45:52.000000 pulumi_kubernetes-4.1.0a1689971798/pulumi_kubernetes/node/__init__.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-21 20:45:53.000000 pulumi_kubernetes-4.1.0a1689971798/pulumi_kubernetes/node/v1/
+-rw-r--r--   0 runner    (1001) docker     (123)    17524 2023-07-21 20:45:52.000000 pulumi_kubernetes-4.1.0a1689971798/pulumi_kubernetes/node/v1/RuntimeClass.py
+-rw-r--r--   0 runner    (1001) docker     (123)    10929 2023-07-21 20:45:52.000000 pulumi_kubernetes-4.1.0a1689971798/pulumi_kubernetes/node/v1/RuntimeClassList.py
+-rw-r--r--   0 runner    (1001) docker     (123)    19157 2023-07-21 20:45:52.000000 pulumi_kubernetes-4.1.0a1689971798/pulumi_kubernetes/node/v1/RuntimeClassPatch.py
+-rw-r--r--   0 runner    (1001) docker     (123)      377 2023-07-21 20:45:52.000000 pulumi_kubernetes-4.1.0a1689971798/pulumi_kubernetes/node/v1/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)    14552 2023-07-21 20:45:52.000000 pulumi_kubernetes-4.1.0a1689971798/pulumi_kubernetes/node/v1/_inputs.py
+-rw-r--r--   0 runner    (1001) docker     (123)    15712 2023-07-21 20:45:52.000000 pulumi_kubernetes-4.1.0a1689971798/pulumi_kubernetes/node/v1/outputs.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-21 20:45:53.000000 pulumi_kubernetes-4.1.0a1689971798/pulumi_kubernetes/node/v1alpha1/
+-rw-r--r--   0 runner    (1001) docker     (123)    12189 2023-07-21 20:45:52.000000 pulumi_kubernetes-4.1.0a1689971798/pulumi_kubernetes/node/v1alpha1/RuntimeClass.py
+-rw-r--r--   0 runner    (1001) docker     (123)    10947 2023-07-21 20:45:52.000000 pulumi_kubernetes-4.1.0a1689971798/pulumi_kubernetes/node/v1alpha1/RuntimeClassList.py
+-rw-r--r--   0 runner    (1001) docker     (123)    13765 2023-07-21 20:45:52.000000 pulumi_kubernetes-4.1.0a1689971798/pulumi_kubernetes/node/v1alpha1/RuntimeClassPatch.py
+-rw-r--r--   0 runner    (1001) docker     (123)      377 2023-07-21 20:45:52.000000 pulumi_kubernetes-4.1.0a1689971798/pulumi_kubernetes/node/v1alpha1/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)    20390 2023-07-21 20:45:52.000000 pulumi_kubernetes-4.1.0a1689971798/pulumi_kubernetes/node/v1alpha1/_inputs.py
+-rw-r--r--   0 runner    (1001) docker     (123)    22634 2023-07-21 20:45:52.000000 pulumi_kubernetes-4.1.0a1689971798/pulumi_kubernetes/node/v1alpha1/outputs.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-21 20:45:53.000000 pulumi_kubernetes-4.1.0a1689971798/pulumi_kubernetes/node/v1beta1/
+-rw-r--r--   0 runner    (1001) docker     (123)    17930 2023-07-21 20:45:52.000000 pulumi_kubernetes-4.1.0a1689971798/pulumi_kubernetes/node/v1beta1/RuntimeClass.py
+-rw-r--r--   0 runner    (1001) docker     (123)    10944 2023-07-21 20:45:52.000000 pulumi_kubernetes-4.1.0a1689971798/pulumi_kubernetes/node/v1beta1/RuntimeClassList.py
+-rw-r--r--   0 runner    (1001) docker     (123)    19563 2023-07-21 20:45:52.000000 pulumi_kubernetes-4.1.0a1689971798/pulumi_kubernetes/node/v1beta1/RuntimeClassPatch.py
+-rw-r--r--   0 runner    (1001) docker     (123)      377 2023-07-21 20:45:52.000000 pulumi_kubernetes-4.1.0a1689971798/pulumi_kubernetes/node/v1beta1/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)    14755 2023-07-21 20:45:52.000000 pulumi_kubernetes-4.1.0a1689971798/pulumi_kubernetes/node/v1beta1/_inputs.py
+-rw-r--r--   0 runner    (1001) docker     (123)    15928 2023-07-21 20:45:52.000000 pulumi_kubernetes-4.1.0a1689971798/pulumi_kubernetes/node/v1beta1/outputs.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1685 2023-07-21 20:45:52.000000 pulumi_kubernetes-4.1.0a1689971798/pulumi_kubernetes/outputs.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-21 20:45:53.000000 pulumi_kubernetes-4.1.0a1689971798/pulumi_kubernetes/policy/
+-rw-r--r--   0 runner    (1001) docker     (123)      535 2023-07-21 20:45:52.000000 pulumi_kubernetes-4.1.0a1689971798/pulumi_kubernetes/policy/__init__.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-21 20:45:53.000000 pulumi_kubernetes-4.1.0a1689971798/pulumi_kubernetes/policy/v1/
+-rw-r--r--   0 runner    (1001) docker     (123)    11632 2023-07-21 20:45:52.000000 pulumi_kubernetes-4.1.0a1689971798/pulumi_kubernetes/policy/v1/PodDisruptionBudget.py
+-rw-r--r--   0 runner    (1001) docker     (123)    11135 2023-07-21 20:45:52.000000 pulumi_kubernetes-4.1.0a1689971798/pulumi_kubernetes/policy/v1/PodDisruptionBudgetList.py
+-rw-r--r--   0 runner    (1001) docker     (123)    13235 2023-07-21 20:45:52.000000 pulumi_kubernetes-4.1.0a1689971798/pulumi_kubernetes/policy/v1/PodDisruptionBudgetPatch.py
+-rw-r--r--   0 runner    (1001) docker     (123)      398 2023-07-21 20:45:52.000000 pulumi_kubernetes-4.1.0a1689971798/pulumi_kubernetes/policy/v1/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)    27765 2023-07-21 20:45:52.000000 pulumi_kubernetes-4.1.0a1689971798/pulumi_kubernetes/policy/v1/_inputs.py
+-rw-r--r--   0 runner    (1001) docker     (123)    36012 2023-07-21 20:45:52.000000 pulumi_kubernetes-4.1.0a1689971798/pulumi_kubernetes/policy/v1/outputs.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-21 20:45:53.000000 pulumi_kubernetes-4.1.0a1689971798/pulumi_kubernetes/policy/v1beta1/
+-rw-r--r--   0 runner    (1001) docker     (123)    10902 2023-07-21 20:45:52.000000 pulumi_kubernetes-4.1.0a1689971798/pulumi_kubernetes/policy/v1beta1/PodDisruptionBudget.py
+-rw-r--r--   0 runner    (1001) docker     (123)    10000 2023-07-21 20:45:52.000000 pulumi_kubernetes-4.1.0a1689971798/pulumi_kubernetes/policy/v1beta1/PodDisruptionBudgetList.py
+-rw-r--r--   0 runner    (1001) docker     (123)    12495 2023-07-21 20:45:52.000000 pulumi_kubernetes-4.1.0a1689971798/pulumi_kubernetes/policy/v1beta1/PodDisruptionBudgetPatch.py
+-rw-r--r--   0 runner    (1001) docker     (123)    11209 2023-07-21 20:45:52.000000 pulumi_kubernetes-4.1.0a1689971798/pulumi_kubernetes/policy/v1beta1/PodSecurityPolicy.py
+-rw-r--r--   0 runner    (1001) docker     (123)    11084 2023-07-21 20:45:52.000000 pulumi_kubernetes-4.1.0a1689971798/pulumi_kubernetes/policy/v1beta1/PodSecurityPolicyList.py
+-rw-r--r--   0 runner    (1001) docker     (123)    12807 2023-07-21 20:45:52.000000 pulumi_kubernetes-4.1.0a1689971798/pulumi_kubernetes/policy/v1beta1/PodSecurityPolicyPatch.py
+-rw-r--r--   0 runner    (1001) docker     (123)      506 2023-07-21 20:45:52.000000 pulumi_kubernetes-4.1.0a1689971798/pulumi_kubernetes/policy/v1beta1/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)   106813 2023-07-21 20:45:52.000000 pulumi_kubernetes-4.1.0a1689971798/pulumi_kubernetes/policy/v1beta1/_inputs.py
+-rw-r--r--   0 runner    (1001) docker     (123)   106119 2023-07-21 20:45:52.000000 pulumi_kubernetes-4.1.0a1689971798/pulumi_kubernetes/policy/v1beta1/outputs.py
+-rw-r--r--   0 runner    (1001) docker     (123)    22916 2023-07-21 20:45:52.000000 pulumi_kubernetes-4.1.0a1689971798/pulumi_kubernetes/provider.py
+-rw-r--r--   0 runner    (1001) docker     (123)       47 2023-07-21 20:45:52.000000 pulumi_kubernetes-4.1.0a1689971798/pulumi_kubernetes/pulumi-plugin.json
+-rw-r--r--   0 runner    (1001) docker     (123)        0 2023-07-21 20:45:52.000000 pulumi_kubernetes-4.1.0a1689971798/pulumi_kubernetes/py.typed
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-21 20:45:53.000000 pulumi_kubernetes-4.1.0a1689971798/pulumi_kubernetes/rbac/
+-rw-r--r--   0 runner    (1001) docker     (123)      683 2023-07-21 20:45:52.000000 pulumi_kubernetes-4.1.0a1689971798/pulumi_kubernetes/rbac/__init__.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-21 20:45:53.000000 pulumi_kubernetes-4.1.0a1689971798/pulumi_kubernetes/rbac/v1/
+-rw-r--r--   0 runner    (1001) docker     (123)    13177 2023-07-21 20:45:52.000000 pulumi_kubernetes-4.1.0a1689971798/pulumi_kubernetes/rbac/v1/ClusterRole.py
+-rw-r--r--   0 runner    (1001) docker     (123)    12895 2023-07-21 20:45:52.000000 pulumi_kubernetes-4.1.0a1689971798/pulumi_kubernetes/rbac/v1/ClusterRoleBinding.py
+-rw-r--r--   0 runner    (1001) docker     (123)    10739 2023-07-21 20:45:52.000000 pulumi_kubernetes-4.1.0a1689971798/pulumi_kubernetes/rbac/v1/ClusterRoleBindingList.py
+-rw-r--r--   0 runner    (1001) docker     (123)    14517 2023-07-21 20:45:52.000000 pulumi_kubernetes-4.1.0a1689971798/pulumi_kubernetes/rbac/v1/ClusterRoleBindingPatch.py
+-rw-r--r--   0 runner    (1001) docker     (123)    10494 2023-07-21 20:45:52.000000 pulumi_kubernetes-4.1.0a1689971798/pulumi_kubernetes/rbac/v1/ClusterRoleList.py
+-rw-r--r--   0 runner    (1001) docker     (123)    14830 2023-07-21 20:45:52.000000 pulumi_kubernetes-4.1.0a1689971798/pulumi_kubernetes/rbac/v1/ClusterRolePatch.py
+-rw-r--r--   0 runner    (1001) docker     (123)    10734 2023-07-21 20:45:52.000000 pulumi_kubernetes-4.1.0a1689971798/pulumi_kubernetes/rbac/v1/Role.py
+-rw-r--r--   0 runner    (1001) docker     (123)    13172 2023-07-21 20:45:52.000000 pulumi_kubernetes-4.1.0a1689971798/pulumi_kubernetes/rbac/v1/RoleBinding.py
+-rw-r--r--   0 runner    (1001) docker     (123)    10494 2023-07-21 20:45:52.000000 pulumi_kubernetes-4.1.0a1689971798/pulumi_kubernetes/rbac/v1/RoleBindingList.py
+-rw-r--r--   0 runner    (1001) docker     (123)    14794 2023-07-21 20:45:52.000000 pulumi_kubernetes-4.1.0a1689971798/pulumi_kubernetes/rbac/v1/RoleBindingPatch.py
+-rw-r--r--   0 runner    (1001) docker     (123)    10249 2023-07-21 20:45:52.000000 pulumi_kubernetes-4.1.0a1689971798/pulumi_kubernetes/rbac/v1/RoleList.py
+-rw-r--r--   0 runner    (1001) docker     (123)    12337 2023-07-21 20:45:52.000000 pulumi_kubernetes-4.1.0a1689971798/pulumi_kubernetes/rbac/v1/RolePatch.py
+-rw-r--r--   0 runner    (1001) docker     (123)      644 2023-07-21 20:45:52.000000 pulumi_kubernetes-4.1.0a1689971798/pulumi_kubernetes/rbac/v1/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)    42139 2023-07-21 20:45:52.000000 pulumi_kubernetes-4.1.0a1689971798/pulumi_kubernetes/rbac/v1/_inputs.py
+-rw-r--r--   0 runner    (1001) docker     (123)    42588 2023-07-21 20:45:52.000000 pulumi_kubernetes-4.1.0a1689971798/pulumi_kubernetes/rbac/v1/outputs.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-21 20:45:53.000000 pulumi_kubernetes-4.1.0a1689971798/pulumi_kubernetes/rbac/v1alpha1/
+-rw-r--r--   0 runner    (1001) docker     (123)    13415 2023-07-21 20:45:52.000000 pulumi_kubernetes-4.1.0a1689971798/pulumi_kubernetes/rbac/v1alpha1/ClusterRole.py
+-rw-r--r--   0 runner    (1001) docker     (123)    13147 2023-07-21 20:45:52.000000 pulumi_kubernetes-4.1.0a1689971798/pulumi_kubernetes/rbac/v1alpha1/ClusterRoleBinding.py
+-rw-r--r--   0 runner    (1001) docker     (123)    11001 2023-07-21 20:45:52.000000 pulumi_kubernetes-4.1.0a1689971798/pulumi_kubernetes/rbac/v1alpha1/ClusterRoleBindingList.py
+-rw-r--r--   0 runner    (1001) docker     (123)    14769 2023-07-21 20:45:52.000000 pulumi_kubernetes-4.1.0a1689971798/pulumi_kubernetes/rbac/v1alpha1/ClusterRoleBindingPatch.py
+-rw-r--r--   0 runner    (1001) docker     (123)    10742 2023-07-21 20:45:52.000000 pulumi_kubernetes-4.1.0a1689971798/pulumi_kubernetes/rbac/v1alpha1/ClusterRoleList.py
+-rw-r--r--   0 runner    (1001) docker     (123)    15068 2023-07-21 20:45:52.000000 pulumi_kubernetes-4.1.0a1689971798/pulumi_kubernetes/rbac/v1alpha1/ClusterRolePatch.py
+-rw-r--r--   0 runner    (1001) docker     (123)    10958 2023-07-21 20:45:52.000000 pulumi_kubernetes-4.1.0a1689971798/pulumi_kubernetes/rbac/v1alpha1/Role.py
+-rw-r--r--   0 runner    (1001) docker     (123)    13410 2023-07-21 20:45:52.000000 pulumi_kubernetes-4.1.0a1689971798/pulumi_kubernetes/rbac/v1alpha1/RoleBinding.py
+-rw-r--r--   0 runner    (1001) docker     (123)    10746 2023-07-21 20:45:52.000000 pulumi_kubernetes-4.1.0a1689971798/pulumi_kubernetes/rbac/v1alpha1/RoleBindingList.py
+-rw-r--r--   0 runner    (1001) docker     (123)    15032 2023-07-21 20:45:52.000000 pulumi_kubernetes-4.1.0a1689971798/pulumi_kubernetes/rbac/v1alpha1/RoleBindingPatch.py
+-rw-r--r--   0 runner    (1001) docker     (123)    10489 2023-07-21 20:45:52.000000 pulumi_kubernetes-4.1.0a1689971798/pulumi_kubernetes/rbac/v1alpha1/RoleList.py
+-rw-r--r--   0 runner    (1001) docker     (123)    12561 2023-07-21 20:45:52.000000 pulumi_kubernetes-4.1.0a1689971798/pulumi_kubernetes/rbac/v1alpha1/RolePatch.py
+-rw-r--r--   0 runner    (1001) docker     (123)      644 2023-07-21 20:45:52.000000 pulumi_kubernetes-4.1.0a1689971798/pulumi_kubernetes/rbac/v1alpha1/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)    43219 2023-07-21 20:45:52.000000 pulumi_kubernetes-4.1.0a1689971798/pulumi_kubernetes/rbac/v1alpha1/_inputs.py
+-rw-r--r--   0 runner    (1001) docker     (123)    44116 2023-07-21 20:45:52.000000 pulumi_kubernetes-4.1.0a1689971798/pulumi_kubernetes/rbac/v1alpha1/outputs.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-21 20:45:53.000000 pulumi_kubernetes-4.1.0a1689971798/pulumi_kubernetes/rbac/v1beta1/
+-rw-r--r--   0 runner    (1001) docker     (123)    13413 2023-07-21 20:45:52.000000 pulumi_kubernetes-4.1.0a1689971798/pulumi_kubernetes/rbac/v1beta1/ClusterRole.py
+-rw-r--r--   0 runner    (1001) docker     (123)    13145 2023-07-21 20:45:52.000000 pulumi_kubernetes-4.1.0a1689971798/pulumi_kubernetes/rbac/v1beta1/ClusterRoleBinding.py
+-rw-r--r--   0 runner    (1001) docker     (123)    11004 2023-07-21 20:45:52.000000 pulumi_kubernetes-4.1.0a1689971798/pulumi_kubernetes/rbac/v1beta1/ClusterRoleBindingList.py
+-rw-r--r--   0 runner    (1001) docker     (123)    14767 2023-07-21 20:45:52.000000 pulumi_kubernetes-4.1.0a1689971798/pulumi_kubernetes/rbac/v1beta1/ClusterRoleBindingPatch.py
+-rw-r--r--   0 runner    (1001) docker     (123)    10739 2023-07-21 20:45:52.000000 pulumi_kubernetes-4.1.0a1689971798/pulumi_kubernetes/rbac/v1beta1/ClusterRoleList.py
+-rw-r--r--   0 runner    (1001) docker     (123)    15066 2023-07-21 20:45:52.000000 pulumi_kubernetes-4.1.0a1689971798/pulumi_kubernetes/rbac/v1beta1/ClusterRolePatch.py
+-rw-r--r--   0 runner    (1001) docker     (123)    10956 2023-07-21 20:45:52.000000 pulumi_kubernetes-4.1.0a1689971798/pulumi_kubernetes/rbac/v1beta1/Role.py
+-rw-r--r--   0 runner    (1001) docker     (123)    13408 2023-07-21 20:45:52.000000 pulumi_kubernetes-4.1.0a1689971798/pulumi_kubernetes/rbac/v1beta1/RoleBinding.py
+-rw-r--r--   0 runner    (1001) docker     (123)    10743 2023-07-21 20:45:52.000000 pulumi_kubernetes-4.1.0a1689971798/pulumi_kubernetes/rbac/v1beta1/RoleBindingList.py
+-rw-r--r--   0 runner    (1001) docker     (123)    15030 2023-07-21 20:45:52.000000 pulumi_kubernetes-4.1.0a1689971798/pulumi_kubernetes/rbac/v1beta1/RoleBindingPatch.py
+-rw-r--r--   0 runner    (1001) docker     (123)    10484 2023-07-21 20:45:52.000000 pulumi_kubernetes-4.1.0a1689971798/pulumi_kubernetes/rbac/v1beta1/RoleList.py
+-rw-r--r--   0 runner    (1001) docker     (123)    12559 2023-07-21 20:45:52.000000 pulumi_kubernetes-4.1.0a1689971798/pulumi_kubernetes/rbac/v1beta1/RolePatch.py
+-rw-r--r--   0 runner    (1001) docker     (123)      644 2023-07-21 20:45:52.000000 pulumi_kubernetes-4.1.0a1689971798/pulumi_kubernetes/rbac/v1beta1/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)    42923 2023-07-21 20:45:52.000000 pulumi_kubernetes-4.1.0a1689971798/pulumi_kubernetes/rbac/v1beta1/_inputs.py
+-rw-r--r--   0 runner    (1001) docker     (123)    43824 2023-07-21 20:45:52.000000 pulumi_kubernetes-4.1.0a1689971798/pulumi_kubernetes/rbac/v1beta1/outputs.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-21 20:45:53.000000 pulumi_kubernetes-4.1.0a1689971798/pulumi_kubernetes/resource/
+-rw-r--r--   0 runner    (1001) docker     (123)      585 2023-07-21 20:45:52.000000 pulumi_kubernetes-4.1.0a1689971798/pulumi_kubernetes/resource/__init__.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-21 20:45:53.000000 pulumi_kubernetes-4.1.0a1689971798/pulumi_kubernetes/resource/v1alpha1/
+-rw-r--r--   0 runner    (1001) docker     (123)    11150 2023-07-21 20:45:52.000000 pulumi_kubernetes-4.1.0a1689971798/pulumi_kubernetes/resource/v1alpha1/PodScheduling.py
+-rw-r--r--   0 runner    (1001) docker     (123)    10590 2023-07-21 20:45:52.000000 pulumi_kubernetes-4.1.0a1689971798/pulumi_kubernetes/resource/v1alpha1/PodSchedulingList.py
+-rw-r--r--   0 runner    (1001) docker     (123)    12721 2023-07-21 20:45:52.000000 pulumi_kubernetes-4.1.0a1689971798/pulumi_kubernetes/resource/v1alpha1/PodSchedulingPatch.py
+-rw-r--r--   0 runner    (1001) docker     (123)    11794 2023-07-21 20:45:52.000000 pulumi_kubernetes-4.1.0a1689971798/pulumi_kubernetes/resource/v1alpha1/ResourceClaim.py
+-rw-r--r--   0 runner    (1001) docker     (123)    10564 2023-07-21 20:45:52.000000 pulumi_kubernetes-4.1.0a1689971798/pulumi_kubernetes/resource/v1alpha1/ResourceClaimList.py
+-rw-r--r--   0 runner    (1001) docker     (123)    13370 2023-07-21 20:45:52.000000 pulumi_kubernetes-4.1.0a1689971798/pulumi_kubernetes/resource/v1alpha1/ResourceClaimPatch.py
+-rw-r--r--   0 runner    (1001) docker     (123)    11484 2023-07-21 20:45:52.000000 pulumi_kubernetes-4.1.0a1689971798/pulumi_kubernetes/resource/v1alpha1/ResourceClaimTemplate.py
+-rw-r--r--   0 runner    (1001) docker     (123)    10820 2023-07-21 20:45:52.000000 pulumi_kubernetes-4.1.0a1689971798/pulumi_kubernetes/resource/v1alpha1/ResourceClaimTemplateList.py
+-rw-r--r--   0 runner    (1001) docker     (123)    13055 2023-07-21 20:45:52.000000 pulumi_kubernetes-4.1.0a1689971798/pulumi_kubernetes/resource/v1alpha1/ResourceClaimTemplatePatch.py
+-rw-r--r--   0 runner    (1001) docker     (123)    16437 2023-07-21 20:45:52.000000 pulumi_kubernetes-4.1.0a1689971798/pulumi_kubernetes/resource/v1alpha1/ResourceClass.py
+-rw-r--r--   0 runner    (1001) docker     (123)    10570 2023-07-21 20:45:52.000000 pulumi_kubernetes-4.1.0a1689971798/pulumi_kubernetes/resource/v1alpha1/ResourceClassList.py
+-rw-r--r--   0 runner    (1001) docker     (123)    18061 2023-07-21 20:45:52.000000 pulumi_kubernetes-4.1.0a1689971798/pulumi_kubernetes/resource/v1alpha1/ResourceClassPatch.py
+-rw-r--r--   0 runner    (1001) docker     (123)      692 2023-07-21 20:45:52.000000 pulumi_kubernetes-4.1.0a1689971798/pulumi_kubernetes/resource/v1alpha1/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)    59521 2023-07-21 20:45:52.000000 pulumi_kubernetes-4.1.0a1689971798/pulumi_kubernetes/resource/v1alpha1/_inputs.py
+-rw-r--r--   0 runner    (1001) docker     (123)    77374 2023-07-21 20:45:52.000000 pulumi_kubernetes-4.1.0a1689971798/pulumi_kubernetes/resource/v1alpha1/outputs.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-21 20:45:53.000000 pulumi_kubernetes-4.1.0a1689971798/pulumi_kubernetes/resource/v1alpha2/
+-rw-r--r--   0 runner    (1001) docker     (123)    11360 2023-07-21 20:45:52.000000 pulumi_kubernetes-4.1.0a1689971798/pulumi_kubernetes/resource/v1alpha2/PodSchedulingContext.py
+-rw-r--r--   0 runner    (1001) docker     (123)    10821 2023-07-21 20:45:52.000000 pulumi_kubernetes-4.1.0a1689971798/pulumi_kubernetes/resource/v1alpha2/PodSchedulingContextList.py
+-rw-r--r--   0 runner    (1001) docker     (123)    12931 2023-07-21 20:45:52.000000 pulumi_kubernetes-4.1.0a1689971798/pulumi_kubernetes/resource/v1alpha2/PodSchedulingContextPatch.py
+-rw-r--r--   0 runner    (1001) docker     (123)    11794 2023-07-21 20:45:52.000000 pulumi_kubernetes-4.1.0a1689971798/pulumi_kubernetes/resource/v1alpha2/ResourceClaim.py
+-rw-r--r--   0 runner    (1001) docker     (123)    10564 2023-07-21 20:45:52.000000 pulumi_kubernetes-4.1.0a1689971798/pulumi_kubernetes/resource/v1alpha2/ResourceClaimList.py
+-rw-r--r--   0 runner    (1001) docker     (123)    13370 2023-07-21 20:45:52.000000 pulumi_kubernetes-4.1.0a1689971798/pulumi_kubernetes/resource/v1alpha2/ResourceClaimPatch.py
+-rw-r--r--   0 runner    (1001) docker     (123)    11484 2023-07-21 20:45:52.000000 pulumi_kubernetes-4.1.0a1689971798/pulumi_kubernetes/resource/v1alpha2/ResourceClaimTemplate.py
+-rw-r--r--   0 runner    (1001) docker     (123)    10820 2023-07-21 20:45:52.000000 pulumi_kubernetes-4.1.0a1689971798/pulumi_kubernetes/resource/v1alpha2/ResourceClaimTemplateList.py
+-rw-r--r--   0 runner    (1001) docker     (123)    13055 2023-07-21 20:45:52.000000 pulumi_kubernetes-4.1.0a1689971798/pulumi_kubernetes/resource/v1alpha2/ResourceClaimTemplatePatch.py
+-rw-r--r--   0 runner    (1001) docker     (123)    16437 2023-07-21 20:45:52.000000 pulumi_kubernetes-4.1.0a1689971798/pulumi_kubernetes/resource/v1alpha2/ResourceClass.py
+-rw-r--r--   0 runner    (1001) docker     (123)    10570 2023-07-21 20:45:52.000000 pulumi_kubernetes-4.1.0a1689971798/pulumi_kubernetes/resource/v1alpha2/ResourceClassList.py
+-rw-r--r--   0 runner    (1001) docker     (123)    18061 2023-07-21 20:45:52.000000 pulumi_kubernetes-4.1.0a1689971798/pulumi_kubernetes/resource/v1alpha2/ResourceClassPatch.py
+-rw-r--r--   0 runner    (1001) docker     (123)      713 2023-07-21 20:45:52.000000 pulumi_kubernetes-4.1.0a1689971798/pulumi_kubernetes/resource/v1alpha2/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)    63467 2023-07-21 20:45:52.000000 pulumi_kubernetes-4.1.0a1689971798/pulumi_kubernetes/resource/v1alpha2/_inputs.py
+-rw-r--r--   0 runner    (1001) docker     (123)    85824 2023-07-21 20:45:52.000000 pulumi_kubernetes-4.1.0a1689971798/pulumi_kubernetes/resource/v1alpha2/outputs.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-21 20:45:53.000000 pulumi_kubernetes-4.1.0a1689971798/pulumi_kubernetes/scheduling/
+-rw-r--r--   0 runner    (1001) docker     (123)      719 2023-07-21 20:45:52.000000 pulumi_kubernetes-4.1.0a1689971798/pulumi_kubernetes/scheduling/__init__.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-21 20:45:53.000000 pulumi_kubernetes-4.1.0a1689971798/pulumi_kubernetes/scheduling/v1/
+-rw-r--r--   0 runner    (1001) docker     (123)    17212 2023-07-21 20:45:52.000000 pulumi_kubernetes-4.1.0a1689971798/pulumi_kubernetes/scheduling/v1/PriorityClass.py
+-rw-r--r--   0 runner    (1001) docker     (123)    10954 2023-07-21 20:45:52.000000 pulumi_kubernetes-4.1.0a1689971798/pulumi_kubernetes/scheduling/v1/PriorityClassList.py
+-rw-r--r--   0 runner    (1001) docker     (123)    18777 2023-07-21 20:45:52.000000 pulumi_kubernetes-4.1.0a1689971798/pulumi_kubernetes/scheduling/v1/PriorityClassPatch.py
+-rw-r--r--   0 runner    (1001) docker     (123)      380 2023-07-21 20:45:52.000000 pulumi_kubernetes-4.1.0a1689971798/pulumi_kubernetes/scheduling/v1/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)     7318 2023-07-21 20:45:52.000000 pulumi_kubernetes-4.1.0a1689971798/pulumi_kubernetes/scheduling/v1/_inputs.py
+-rw-r--r--   0 runner    (1001) docker     (123)     6955 2023-07-21 20:45:52.000000 pulumi_kubernetes-4.1.0a1689971798/pulumi_kubernetes/scheduling/v1/outputs.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-21 20:45:53.000000 pulumi_kubernetes-4.1.0a1689971798/pulumi_kubernetes/scheduling/v1alpha1/
+-rw-r--r--   0 runner    (1001) docker     (123)    17744 2023-07-21 20:45:52.000000 pulumi_kubernetes-4.1.0a1689971798/pulumi_kubernetes/scheduling/v1alpha1/PriorityClass.py
+-rw-r--r--   0 runner    (1001) docker     (123)    10972 2023-07-21 20:45:52.000000 pulumi_kubernetes-4.1.0a1689971798/pulumi_kubernetes/scheduling/v1alpha1/PriorityClassList.py
+-rw-r--r--   0 runner    (1001) docker     (123)    19309 2023-07-21 20:45:52.000000 pulumi_kubernetes-4.1.0a1689971798/pulumi_kubernetes/scheduling/v1alpha1/PriorityClassPatch.py
+-rw-r--r--   0 runner    (1001) docker     (123)      380 2023-07-21 20:45:52.000000 pulumi_kubernetes-4.1.0a1689971798/pulumi_kubernetes/scheduling/v1alpha1/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)     7584 2023-07-21 20:45:52.000000 pulumi_kubernetes-4.1.0a1689971798/pulumi_kubernetes/scheduling/v1alpha1/_inputs.py
+-rw-r--r--   0 runner    (1001) docker     (123)     7323 2023-07-21 20:45:52.000000 pulumi_kubernetes-4.1.0a1689971798/pulumi_kubernetes/scheduling/v1alpha1/outputs.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-21 20:45:53.000000 pulumi_kubernetes-4.1.0a1689971798/pulumi_kubernetes/scheduling/v1beta1/
+-rw-r--r--   0 runner    (1001) docker     (123)    17742 2023-07-21 20:45:52.000000 pulumi_kubernetes-4.1.0a1689971798/pulumi_kubernetes/scheduling/v1beta1/PriorityClass.py
+-rw-r--r--   0 runner    (1001) docker     (123)    10969 2023-07-21 20:45:52.000000 pulumi_kubernetes-4.1.0a1689971798/pulumi_kubernetes/scheduling/v1beta1/PriorityClassList.py
+-rw-r--r--   0 runner    (1001) docker     (123)    19307 2023-07-21 20:45:52.000000 pulumi_kubernetes-4.1.0a1689971798/pulumi_kubernetes/scheduling/v1beta1/PriorityClassPatch.py
+-rw-r--r--   0 runner    (1001) docker     (123)      380 2023-07-21 20:45:52.000000 pulumi_kubernetes-4.1.0a1689971798/pulumi_kubernetes/scheduling/v1beta1/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)     7583 2023-07-21 20:45:52.000000 pulumi_kubernetes-4.1.0a1689971798/pulumi_kubernetes/scheduling/v1beta1/_inputs.py
+-rw-r--r--   0 runner    (1001) docker     (123)     7322 2023-07-21 20:45:52.000000 pulumi_kubernetes-4.1.0a1689971798/pulumi_kubernetes/scheduling/v1beta1/outputs.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-21 20:45:53.000000 pulumi_kubernetes-4.1.0a1689971798/pulumi_kubernetes/settings/
+-rw-r--r--   0 runner    (1001) docker     (123)      421 2023-07-21 20:45:52.000000 pulumi_kubernetes-4.1.0a1689971798/pulumi_kubernetes/settings/__init__.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-21 20:45:53.000000 pulumi_kubernetes-4.1.0a1689971798/pulumi_kubernetes/settings/v1alpha1/
+-rw-r--r--   0 runner    (1001) docker     (123)     9676 2023-07-21 20:45:52.000000 pulumi_kubernetes-4.1.0a1689971798/pulumi_kubernetes/settings/v1alpha1/PodPreset.py
+-rw-r--r--   0 runner    (1001) docker     (123)    10866 2023-07-21 20:45:52.000000 pulumi_kubernetes-4.1.0a1689971798/pulumi_kubernetes/settings/v1alpha1/PodPresetList.py
+-rw-r--r--   0 runner    (1001) docker     (123)    11249 2023-07-21 20:45:52.000000 pulumi_kubernetes-4.1.0a1689971798/pulumi_kubernetes/settings/v1alpha1/PodPresetPatch.py
+-rw-r--r--   0 runner    (1001) docker     (123)      368 2023-07-21 20:45:52.000000 pulumi_kubernetes-4.1.0a1689971798/pulumi_kubernetes/settings/v1alpha1/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)    12130 2023-07-21 20:45:52.000000 pulumi_kubernetes-4.1.0a1689971798/pulumi_kubernetes/settings/v1alpha1/_inputs.py
+-rw-r--r--   0 runner    (1001) docker     (123)    11192 2023-07-21 20:45:52.000000 pulumi_kubernetes-4.1.0a1689971798/pulumi_kubernetes/settings/v1alpha1/outputs.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-21 20:45:53.000000 pulumi_kubernetes-4.1.0a1689971798/pulumi_kubernetes/storage/
+-rw-r--r--   0 runner    (1001) docker     (123)      701 2023-07-21 20:45:52.000000 pulumi_kubernetes-4.1.0a1689971798/pulumi_kubernetes/storage/__init__.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-21 20:45:53.000000 pulumi_kubernetes-4.1.0a1689971798/pulumi_kubernetes/storage/v1/
+-rw-r--r--   0 runner    (1001) docker     (123)    12783 2023-07-21 20:45:52.000000 pulumi_kubernetes-4.1.0a1689971798/pulumi_kubernetes/storage/v1/CSIDriver.py
+-rw-r--r--   0 runner    (1001) docker     (123)    10807 2023-07-21 20:45:52.000000 pulumi_kubernetes-4.1.0a1689971798/pulumi_kubernetes/storage/v1/CSIDriverList.py
+-rw-r--r--   0 runner    (1001) docker     (123)    14354 2023-07-21 20:45:52.000000 pulumi_kubernetes-4.1.0a1689971798/pulumi_kubernetes/storage/v1/CSIDriverPatch.py
+-rw-r--r--   0 runner    (1001) docker     (123)    11643 2023-07-21 20:45:52.000000 pulumi_kubernetes-4.1.0a1689971798/pulumi_kubernetes/storage/v1/CSINode.py
+-rw-r--r--   0 runner    (1001) docker     (123)    10737 2023-07-21 20:45:52.000000 pulumi_kubernetes-4.1.0a1689971798/pulumi_kubernetes/storage/v1/CSINodeList.py
+-rw-r--r--   0 runner    (1001) docker     (123)    13214 2023-07-21 20:45:52.000000 pulumi_kubernetes-4.1.0a1689971798/pulumi_kubernetes/storage/v1/CSINodePatch.py
+-rw-r--r--   0 runner    (1001) docker     (123)    24161 2023-07-21 20:45:52.000000 pulumi_kubernetes-4.1.0a1689971798/pulumi_kubernetes/storage/v1/CSIStorageCapacity.py
+-rw-r--r--   0 runner    (1001) docker     (123)    11158 2023-07-21 20:45:52.000000 pulumi_kubernetes-4.1.0a1689971798/pulumi_kubernetes/storage/v1/CSIStorageCapacityList.py
+-rw-r--r--   0 runner    (1001) docker     (123)    25753 2023-07-21 20:45:52.000000 pulumi_kubernetes-4.1.0a1689971798/pulumi_kubernetes/storage/v1/CSIStorageCapacityPatch.py
+-rw-r--r--   0 runner    (1001) docker     (123)    22861 2023-07-21 20:45:52.000000 pulumi_kubernetes-4.1.0a1689971798/pulumi_kubernetes/storage/v1/StorageClass.py
+-rw-r--r--   0 runner    (1001) docker     (123)    10940 2023-07-21 20:45:52.000000 pulumi_kubernetes-4.1.0a1689971798/pulumi_kubernetes/storage/v1/StorageClassList.py
+-rw-r--r--   0 runner    (1001) docker     (123)    24485 2023-07-21 20:45:52.000000 pulumi_kubernetes-4.1.0a1689971798/pulumi_kubernetes/storage/v1/StorageClassPatch.py
+-rw-r--r--   0 runner    (1001) docker     (123)    12090 2023-07-21 20:45:52.000000 pulumi_kubernetes-4.1.0a1689971798/pulumi_kubernetes/storage/v1/VolumeAttachment.py
+-rw-r--r--   0 runner    (1001) docker     (123)    11086 2023-07-21 20:45:52.000000 pulumi_kubernetes-4.1.0a1689971798/pulumi_kubernetes/storage/v1/VolumeAttachmentList.py
+-rw-r--r--   0 runner    (1001) docker     (123)    13671 2023-07-21 20:45:52.000000 pulumi_kubernetes-4.1.0a1689971798/pulumi_kubernetes/storage/v1/VolumeAttachmentPatch.py
+-rw-r--r--   0 runner    (1001) docker     (123)      755 2023-07-21 20:45:52.000000 pulumi_kubernetes-4.1.0a1689971798/pulumi_kubernetes/storage/v1/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)   105129 2023-07-21 20:45:52.000000 pulumi_kubernetes-4.1.0a1689971798/pulumi_kubernetes/storage/v1/_inputs.py
+-rw-r--r--   0 runner    (1001) docker     (123)   111767 2023-07-21 20:45:52.000000 pulumi_kubernetes-4.1.0a1689971798/pulumi_kubernetes/storage/v1/outputs.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-21 20:45:53.000000 pulumi_kubernetes-4.1.0a1689971798/pulumi_kubernetes/storage/v1alpha1/
+-rw-r--r--   0 runner    (1001) docker     (123)    12020 2023-07-21 20:45:52.000000 pulumi_kubernetes-4.1.0a1689971798/pulumi_kubernetes/storage/v1alpha1/VolumeAttachment.py
+-rw-r--r--   0 runner    (1001) docker     (123)    11104 2023-07-21 20:45:52.000000 pulumi_kubernetes-4.1.0a1689971798/pulumi_kubernetes/storage/v1alpha1/VolumeAttachmentList.py
+-rw-r--r--   0 runner    (1001) docker     (123)    13601 2023-07-21 20:45:52.000000 pulumi_kubernetes-4.1.0a1689971798/pulumi_kubernetes/storage/v1alpha1/VolumeAttachmentPatch.py
+-rw-r--r--   0 runner    (1001) docker     (123)      389 2023-07-21 20:45:52.000000 pulumi_kubernetes-4.1.0a1689971798/pulumi_kubernetes/storage/v1alpha1/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)    20227 2023-07-21 20:45:52.000000 pulumi_kubernetes-4.1.0a1689971798/pulumi_kubernetes/storage/v1alpha1/_inputs.py
+-rw-r--r--   0 runner    (1001) docker     (123)    26754 2023-07-21 20:45:52.000000 pulumi_kubernetes-4.1.0a1689971798/pulumi_kubernetes/storage/v1alpha1/outputs.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-21 20:45:53.000000 pulumi_kubernetes-4.1.0a1689971798/pulumi_kubernetes/storage/v1beta1/
+-rw-r--r--   0 runner    (1001) docker     (123)    13183 2023-07-21 20:45:52.000000 pulumi_kubernetes-4.1.0a1689971798/pulumi_kubernetes/storage/v1beta1/CSIDriver.py
+-rw-r--r--   0 runner    (1001) docker     (123)    10822 2023-07-21 20:45:52.000000 pulumi_kubernetes-4.1.0a1689971798/pulumi_kubernetes/storage/v1beta1/CSIDriverList.py
+-rw-r--r--   0 runner    (1001) docker     (123)    14754 2023-07-21 20:45:52.000000 pulumi_kubernetes-4.1.0a1689971798/pulumi_kubernetes/storage/v1beta1/CSIDriverPatch.py
+-rw-r--r--   0 runner    (1001) docker     (123)    11541 2023-07-21 20:45:52.000000 pulumi_kubernetes-4.1.0a1689971798/pulumi_kubernetes/storage/v1beta1/CSINode.py
+-rw-r--r--   0 runner    (1001) docker     (123)    10752 2023-07-21 20:45:52.000000 pulumi_kubernetes-4.1.0a1689971798/pulumi_kubernetes/storage/v1beta1/CSINodeList.py
+-rw-r--r--   0 runner    (1001) docker     (123)    13112 2023-07-21 20:45:52.000000 pulumi_kubernetes-4.1.0a1689971798/pulumi_kubernetes/storage/v1beta1/CSINodePatch.py
+-rw-r--r--   0 runner    (1001) docker     (123)    24071 2023-07-21 20:45:52.000000 pulumi_kubernetes-4.1.0a1689971798/pulumi_kubernetes/storage/v1beta1/CSIStorageCapacity.py
+-rw-r--r--   0 runner    (1001) docker     (123)    11173 2023-07-21 20:45:52.000000 pulumi_kubernetes-4.1.0a1689971798/pulumi_kubernetes/storage/v1beta1/CSIStorageCapacityList.py
+-rw-r--r--   0 runner    (1001) docker     (123)    25663 2023-07-21 20:45:52.000000 pulumi_kubernetes-4.1.0a1689971798/pulumi_kubernetes/storage/v1beta1/CSIStorageCapacityPatch.py
+-rw-r--r--   0 runner    (1001) docker     (123)    22731 2023-07-21 20:45:52.000000 pulumi_kubernetes-4.1.0a1689971798/pulumi_kubernetes/storage/v1beta1/StorageClass.py
+-rw-r--r--   0 runner    (1001) docker     (123)    10955 2023-07-21 20:45:52.000000 pulumi_kubernetes-4.1.0a1689971798/pulumi_kubernetes/storage/v1beta1/StorageClassList.py
+-rw-r--r--   0 runner    (1001) docker     (123)    24355 2023-07-21 20:45:52.000000 pulumi_kubernetes-4.1.0a1689971798/pulumi_kubernetes/storage/v1beta1/StorageClassPatch.py
+-rw-r--r--   0 runner    (1001) docker     (123)    12018 2023-07-21 20:45:52.000000 pulumi_kubernetes-4.1.0a1689971798/pulumi_kubernetes/storage/v1beta1/VolumeAttachment.py
+-rw-r--r--   0 runner    (1001) docker     (123)    11101 2023-07-21 20:45:52.000000 pulumi_kubernetes-4.1.0a1689971798/pulumi_kubernetes/storage/v1beta1/VolumeAttachmentList.py
+-rw-r--r--   0 runner    (1001) docker     (123)    13599 2023-07-21 20:45:52.000000 pulumi_kubernetes-4.1.0a1689971798/pulumi_kubernetes/storage/v1beta1/VolumeAttachmentPatch.py
+-rw-r--r--   0 runner    (1001) docker     (123)      755 2023-07-21 20:45:52.000000 pulumi_kubernetes-4.1.0a1689971798/pulumi_kubernetes/storage/v1beta1/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)    98721 2023-07-21 20:45:52.000000 pulumi_kubernetes-4.1.0a1689971798/pulumi_kubernetes/storage/v1beta1/_inputs.py
+-rw-r--r--   0 runner    (1001) docker     (123)   105646 2023-07-21 20:45:52.000000 pulumi_kubernetes-4.1.0a1689971798/pulumi_kubernetes/storage/v1beta1/outputs.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-21 20:45:53.000000 pulumi_kubernetes-4.1.0a1689971798/pulumi_kubernetes/yaml/
+-rw-r--r--   0 runner    (1001) docker     (123)      258 2023-07-21 20:45:52.000000 pulumi_kubernetes-4.1.0a1689971798/pulumi_kubernetes/yaml/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)   100539 2023-07-21 20:45:52.000000 pulumi_kubernetes-4.1.0a1689971798/pulumi_kubernetes/yaml/yaml.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-21 20:45:53.000000 pulumi_kubernetes-4.1.0a1689971798/pulumi_kubernetes.egg-info/
+-rw-r--r--   0 runner    (1001) docker     (123)    11092 2023-07-21 20:45:53.000000 pulumi_kubernetes-4.1.0a1689971798/pulumi_kubernetes.egg-info/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (123)    28617 2023-07-21 20:45:53.000000 pulumi_kubernetes-4.1.0a1689971798/pulumi_kubernetes.egg-info/SOURCES.txt
+-rw-r--r--   0 runner    (1001) docker     (123)        1 2023-07-21 20:45:53.000000 pulumi_kubernetes-4.1.0a1689971798/pulumi_kubernetes.egg-info/dependency_links.txt
+-rw-r--r--   0 runner    (1001) docker     (123)        1 2023-07-21 20:45:52.000000 pulumi_kubernetes-4.1.0a1689971798/pulumi_kubernetes.egg-info/not-zip-safe
+-rw-r--r--   0 runner    (1001) docker     (123)       70 2023-07-21 20:45:53.000000 pulumi_kubernetes-4.1.0a1689971798/pulumi_kubernetes.egg-info/requires.txt
+-rw-r--r--   0 runner    (1001) docker     (123)       18 2023-07-21 20:45:53.000000 pulumi_kubernetes-4.1.0a1689971798/pulumi_kubernetes.egg-info/top_level.txt
+-rw-r--r--   0 runner    (1001) docker     (123)       38 2023-07-21 20:45:53.000000 pulumi_kubernetes-4.1.0a1689971798/setup.cfg
+-rw-r--r--   0 runner    (1001) docker     (123)     2216 2023-07-21 20:45:52.000000 pulumi_kubernetes-4.1.0a1689971798/setup.py
```

### Comparing `pulumi_kubernetes-4.1.0a1689918291/PKG-INFO` & `pulumi_kubernetes-4.1.0a1689971798/PKG-INFO`

 * *Files 1% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: pulumi_kubernetes
-Version: 4.1.0a1689918291
+Version: 4.1.0a1689971798
 Summary: A Pulumi package for creating and managing Kubernetes resources.
 Home-page: https://pulumi.com
 License: Apache-2.0
 Project-URL: Repository, https://github.com/pulumi/pulumi-kubernetes
 Description: [![Build Status](https://travis-ci.com/pulumi/pulumi-kubernetes.svg?token=eHg7Zp5zdDDJfTjY8ejq&branch=master)](https://travis-ci.com/pulumi/pulumi-kubernetes)
         [![Slack](http://www.pulumi.com/images/docs/badges/slack.svg)](https://slack.pulumi.com)
         [![NPM version](https://badge.fury.io/js/%40pulumi%2Fkubernetes.svg)](https://www.npmjs.com/package/@pulumi/kubernetes)
```

#### html2text {}

```diff
@@ -1,8 +1,8 @@
-Metadata-Version: 2.1 Name: pulumi_kubernetes Version: 4.1.0a1689918291
+Metadata-Version: 2.1 Name: pulumi_kubernetes Version: 4.1.0a1689971798
 Summary: A Pulumi package for creating and managing Kubernetes resources. Home-
 page: https://pulumi.com License: Apache-2.0 Project-URL: Repository, https://
 github.com/pulumi/pulumi-kubernetes Description: [![Build Status](https://
 travis-ci.com/pulumi/pulumi-
 kubernetes.svg?token=eHg7Zp5zdDDJfTjY8ejq&branch=master)](https://travis-
 ci.com/pulumi/pulumi-kubernetes) [![Slack](http://www.pulumi.com/images/docs/
 badges/slack.svg)](https://slack.pulumi.com) [![NPM version](https://
```

### Comparing `pulumi_kubernetes-4.1.0a1689918291/README.md` & `pulumi_kubernetes-4.1.0a1689971798/README.md`

 * *Files identical despite different names*

### Comparing `pulumi_kubernetes-4.1.0a1689918291/pulumi_kubernetes/__init__.py` & `pulumi_kubernetes-4.1.0a1689971798/pulumi_kubernetes/__init__.py`

 * *Files identical despite different names*

### Comparing `pulumi_kubernetes-4.1.0a1689918291/pulumi_kubernetes/_inputs.py` & `pulumi_kubernetes-4.1.0a1689971798/pulumi_kubernetes/_inputs.py`

 * *Files identical despite different names*

### Comparing `pulumi_kubernetes-4.1.0a1689918291/pulumi_kubernetes/_tables.py` & `pulumi_kubernetes-4.1.0a1689971798/pulumi_kubernetes/_tables.py`

 * *Files identical despite different names*

### Comparing `pulumi_kubernetes-4.1.0a1689918291/pulumi_kubernetes/_utilities.py` & `pulumi_kubernetes-4.1.0a1689971798/pulumi_kubernetes/_utilities.py`

 * *Files identical despite different names*

### Comparing `pulumi_kubernetes-4.1.0a1689918291/pulumi_kubernetes/admissionregistration/__init__.py` & `pulumi_kubernetes-4.1.0a1689971798/pulumi_kubernetes/admissionregistration/__init__.py`

 * *Files identical despite different names*

### Comparing `pulumi_kubernetes-4.1.0a1689918291/pulumi_kubernetes/admissionregistration/v1/MutatingWebhookConfiguration.py` & `pulumi_kubernetes-4.1.0a1689971798/pulumi_kubernetes/admissionregistration/v1/MutatingWebhookConfiguration.py`

 * *Files identical despite different names*

### Comparing `pulumi_kubernetes-4.1.0a1689918291/pulumi_kubernetes/admissionregistration/v1/MutatingWebhookConfigurationList.py` & `pulumi_kubernetes-4.1.0a1689971798/pulumi_kubernetes/admissionregistration/v1/MutatingWebhookConfigurationList.py`

 * *Files identical despite different names*

### Comparing `pulumi_kubernetes-4.1.0a1689918291/pulumi_kubernetes/admissionregistration/v1/MutatingWebhookConfigurationPatch.py` & `pulumi_kubernetes-4.1.0a1689971798/pulumi_kubernetes/admissionregistration/v1/MutatingWebhookConfigurationPatch.py`

 * *Files identical despite different names*

### Comparing `pulumi_kubernetes-4.1.0a1689918291/pulumi_kubernetes/admissionregistration/v1/ValidatingWebhookConfiguration.py` & `pulumi_kubernetes-4.1.0a1689971798/pulumi_kubernetes/admissionregistration/v1/ValidatingWebhookConfiguration.py`

 * *Files identical despite different names*

### Comparing `pulumi_kubernetes-4.1.0a1689918291/pulumi_kubernetes/admissionregistration/v1/ValidatingWebhookConfigurationList.py` & `pulumi_kubernetes-4.1.0a1689971798/pulumi_kubernetes/admissionregistration/v1/ValidatingWebhookConfigurationList.py`

 * *Files identical despite different names*

### Comparing `pulumi_kubernetes-4.1.0a1689918291/pulumi_kubernetes/admissionregistration/v1/ValidatingWebhookConfigurationPatch.py` & `pulumi_kubernetes-4.1.0a1689971798/pulumi_kubernetes/admissionregistration/v1/ValidatingWebhookConfigurationPatch.py`

 * *Files identical despite different names*

### Comparing `pulumi_kubernetes-4.1.0a1689918291/pulumi_kubernetes/admissionregistration/v1/__init__.py` & `pulumi_kubernetes-4.1.0a1689971798/pulumi_kubernetes/admissionregistration/v1/__init__.py`

 * *Files identical despite different names*

### Comparing `pulumi_kubernetes-4.1.0a1689918291/pulumi_kubernetes/admissionregistration/v1/_inputs.py` & `pulumi_kubernetes-4.1.0a1689971798/pulumi_kubernetes/admissionregistration/v1/_inputs.py`

 * *Files identical despite different names*

### Comparing `pulumi_kubernetes-4.1.0a1689918291/pulumi_kubernetes/admissionregistration/v1/outputs.py` & `pulumi_kubernetes-4.1.0a1689971798/pulumi_kubernetes/admissionregistration/v1/outputs.py`

 * *Files identical despite different names*

### Comparing `pulumi_kubernetes-4.1.0a1689918291/pulumi_kubernetes/admissionregistration/v1alpha1/ValidatingAdmissionPolicy.py` & `pulumi_kubernetes-4.1.0a1689971798/pulumi_kubernetes/admissionregistration/v1alpha1/ValidatingAdmissionPolicy.py`

 * *Files identical despite different names*

### Comparing `pulumi_kubernetes-4.1.0a1689918291/pulumi_kubernetes/admissionregistration/v1alpha1/ValidatingAdmissionPolicyBinding.py` & `pulumi_kubernetes-4.1.0a1689971798/pulumi_kubernetes/admissionregistration/v1alpha1/ValidatingAdmissionPolicyBinding.py`

 * *Files identical despite different names*

### Comparing `pulumi_kubernetes-4.1.0a1689918291/pulumi_kubernetes/admissionregistration/v1alpha1/ValidatingAdmissionPolicyBindingList.py` & `pulumi_kubernetes-4.1.0a1689971798/pulumi_kubernetes/admissionregistration/v1alpha1/ValidatingAdmissionPolicyBindingList.py`

 * *Files identical despite different names*

### Comparing `pulumi_kubernetes-4.1.0a1689918291/pulumi_kubernetes/admissionregistration/v1alpha1/ValidatingAdmissionPolicyBindingPatch.py` & `pulumi_kubernetes-4.1.0a1689971798/pulumi_kubernetes/admissionregistration/v1alpha1/ValidatingAdmissionPolicyBindingPatch.py`

 * *Files identical despite different names*

### Comparing `pulumi_kubernetes-4.1.0a1689918291/pulumi_kubernetes/admissionregistration/v1alpha1/ValidatingAdmissionPolicyList.py` & `pulumi_kubernetes-4.1.0a1689971798/pulumi_kubernetes/admissionregistration/v1alpha1/ValidatingAdmissionPolicyList.py`

 * *Files identical despite different names*

### Comparing `pulumi_kubernetes-4.1.0a1689918291/pulumi_kubernetes/admissionregistration/v1alpha1/ValidatingAdmissionPolicyPatch.py` & `pulumi_kubernetes-4.1.0a1689971798/pulumi_kubernetes/admissionregistration/v1alpha1/ValidatingAdmissionPolicyPatch.py`

 * *Files identical despite different names*

### Comparing `pulumi_kubernetes-4.1.0a1689918291/pulumi_kubernetes/admissionregistration/v1alpha1/__init__.py` & `pulumi_kubernetes-4.1.0a1689971798/pulumi_kubernetes/admissionregistration/v1alpha1/__init__.py`

 * *Files identical despite different names*

### Comparing `pulumi_kubernetes-4.1.0a1689918291/pulumi_kubernetes/admissionregistration/v1alpha1/_inputs.py` & `pulumi_kubernetes-4.1.0a1689971798/pulumi_kubernetes/admissionregistration/v1alpha1/_inputs.py`

 * *Files identical despite different names*

### Comparing `pulumi_kubernetes-4.1.0a1689918291/pulumi_kubernetes/admissionregistration/v1alpha1/outputs.py` & `pulumi_kubernetes-4.1.0a1689971798/pulumi_kubernetes/admissionregistration/v1alpha1/outputs.py`

 * *Files identical despite different names*

### Comparing `pulumi_kubernetes-4.1.0a1689918291/pulumi_kubernetes/admissionregistration/v1beta1/MutatingWebhookConfiguration.py` & `pulumi_kubernetes-4.1.0a1689971798/pulumi_kubernetes/admissionregistration/v1beta1/MutatingWebhookConfiguration.py`

 * *Files identical despite different names*

### Comparing `pulumi_kubernetes-4.1.0a1689918291/pulumi_kubernetes/admissionregistration/v1beta1/MutatingWebhookConfigurationList.py` & `pulumi_kubernetes-4.1.0a1689971798/pulumi_kubernetes/admissionregistration/v1beta1/MutatingWebhookConfigurationList.py`

 * *Files identical despite different names*

### Comparing `pulumi_kubernetes-4.1.0a1689918291/pulumi_kubernetes/admissionregistration/v1beta1/MutatingWebhookConfigurationPatch.py` & `pulumi_kubernetes-4.1.0a1689971798/pulumi_kubernetes/admissionregistration/v1beta1/MutatingWebhookConfigurationPatch.py`

 * *Files identical despite different names*

### Comparing `pulumi_kubernetes-4.1.0a1689918291/pulumi_kubernetes/admissionregistration/v1beta1/ValidatingWebhookConfiguration.py` & `pulumi_kubernetes-4.1.0a1689971798/pulumi_kubernetes/admissionregistration/v1beta1/ValidatingWebhookConfiguration.py`

 * *Files identical despite different names*

### Comparing `pulumi_kubernetes-4.1.0a1689918291/pulumi_kubernetes/admissionregistration/v1beta1/ValidatingWebhookConfigurationList.py` & `pulumi_kubernetes-4.1.0a1689971798/pulumi_kubernetes/admissionregistration/v1beta1/ValidatingWebhookConfigurationList.py`

 * *Files identical despite different names*

### Comparing `pulumi_kubernetes-4.1.0a1689918291/pulumi_kubernetes/admissionregistration/v1beta1/ValidatingWebhookConfigurationPatch.py` & `pulumi_kubernetes-4.1.0a1689971798/pulumi_kubernetes/admissionregistration/v1beta1/ValidatingWebhookConfigurationPatch.py`

 * *Files identical despite different names*

### Comparing `pulumi_kubernetes-4.1.0a1689918291/pulumi_kubernetes/admissionregistration/v1beta1/__init__.py` & `pulumi_kubernetes-4.1.0a1689971798/pulumi_kubernetes/admissionregistration/v1beta1/__init__.py`

 * *Files identical despite different names*

### Comparing `pulumi_kubernetes-4.1.0a1689918291/pulumi_kubernetes/admissionregistration/v1beta1/_inputs.py` & `pulumi_kubernetes-4.1.0a1689971798/pulumi_kubernetes/admissionregistration/v1beta1/_inputs.py`

 * *Files identical despite different names*

### Comparing `pulumi_kubernetes-4.1.0a1689918291/pulumi_kubernetes/admissionregistration/v1beta1/outputs.py` & `pulumi_kubernetes-4.1.0a1689971798/pulumi_kubernetes/admissionregistration/v1beta1/outputs.py`

 * *Files identical despite different names*

### Comparing `pulumi_kubernetes-4.1.0a1689918291/pulumi_kubernetes/apiextensions/CustomResource.py` & `pulumi_kubernetes-4.1.0a1689971798/pulumi_kubernetes/apiextensions/CustomResource.py`

 * *Files identical despite different names*

### Comparing `pulumi_kubernetes-4.1.0a1689918291/pulumi_kubernetes/apiextensions/CustomResourcePatch.py` & `pulumi_kubernetes-4.1.0a1689971798/pulumi_kubernetes/apiextensions/CustomResourcePatch.py`

 * *Files identical despite different names*

### Comparing `pulumi_kubernetes-4.1.0a1689918291/pulumi_kubernetes/apiextensions/__init__.py` & `pulumi_kubernetes-4.1.0a1689971798/pulumi_kubernetes/apiextensions/__init__.py`

 * *Files identical despite different names*

### Comparing `pulumi_kubernetes-4.1.0a1689918291/pulumi_kubernetes/apiextensions/v1/CustomResourceDefinition.py` & `pulumi_kubernetes-4.1.0a1689971798/pulumi_kubernetes/apiextensions/v1/CustomResourceDefinition.py`

 * *Files identical despite different names*

### Comparing `pulumi_kubernetes-4.1.0a1689918291/pulumi_kubernetes/apiextensions/v1/CustomResourceDefinitionList.py` & `pulumi_kubernetes-4.1.0a1689971798/pulumi_kubernetes/apiextensions/v1/CustomResourceDefinitionList.py`

 * *Files identical despite different names*

### Comparing `pulumi_kubernetes-4.1.0a1689918291/pulumi_kubernetes/apiextensions/v1/CustomResourceDefinitionPatch.py` & `pulumi_kubernetes-4.1.0a1689971798/pulumi_kubernetes/apiextensions/v1/CustomResourceDefinitionPatch.py`

 * *Files identical despite different names*

### Comparing `pulumi_kubernetes-4.1.0a1689918291/pulumi_kubernetes/apiextensions/v1/_inputs.py` & `pulumi_kubernetes-4.1.0a1689971798/pulumi_kubernetes/apiextensions/v1/_inputs.py`

 * *Files identical despite different names*

### Comparing `pulumi_kubernetes-4.1.0a1689918291/pulumi_kubernetes/apiextensions/v1/outputs.py` & `pulumi_kubernetes-4.1.0a1689971798/pulumi_kubernetes/apiextensions/v1/outputs.py`

 * *Files identical despite different names*

### Comparing `pulumi_kubernetes-4.1.0a1689918291/pulumi_kubernetes/apiextensions/v1beta1/CustomResourceDefinition.py` & `pulumi_kubernetes-4.1.0a1689971798/pulumi_kubernetes/apiextensions/v1beta1/CustomResourceDefinition.py`

 * *Files identical despite different names*

### Comparing `pulumi_kubernetes-4.1.0a1689918291/pulumi_kubernetes/apiextensions/v1beta1/CustomResourceDefinitionList.py` & `pulumi_kubernetes-4.1.0a1689971798/pulumi_kubernetes/apiextensions/v1beta1/CustomResourceDefinitionList.py`

 * *Files identical despite different names*

### Comparing `pulumi_kubernetes-4.1.0a1689918291/pulumi_kubernetes/apiextensions/v1beta1/CustomResourceDefinitionPatch.py` & `pulumi_kubernetes-4.1.0a1689971798/pulumi_kubernetes/apiextensions/v1beta1/CustomResourceDefinitionPatch.py`

 * *Files identical despite different names*

### Comparing `pulumi_kubernetes-4.1.0a1689918291/pulumi_kubernetes/apiextensions/v1beta1/_inputs.py` & `pulumi_kubernetes-4.1.0a1689971798/pulumi_kubernetes/apiextensions/v1beta1/_inputs.py`

 * *Files identical despite different names*

### Comparing `pulumi_kubernetes-4.1.0a1689918291/pulumi_kubernetes/apiextensions/v1beta1/outputs.py` & `pulumi_kubernetes-4.1.0a1689971798/pulumi_kubernetes/apiextensions/v1beta1/outputs.py`

 * *Files identical despite different names*

### Comparing `pulumi_kubernetes-4.1.0a1689918291/pulumi_kubernetes/apiregistration/__init__.py` & `pulumi_kubernetes-4.1.0a1689971798/pulumi_kubernetes/apiregistration/__init__.py`

 * *Files identical despite different names*

### Comparing `pulumi_kubernetes-4.1.0a1689918291/pulumi_kubernetes/apiregistration/v1/APIService.py` & `pulumi_kubernetes-4.1.0a1689971798/pulumi_kubernetes/apiregistration/v1/APIService.py`

 * *Files identical despite different names*

### Comparing `pulumi_kubernetes-4.1.0a1689918291/pulumi_kubernetes/apiregistration/v1/APIServiceList.py` & `pulumi_kubernetes-4.1.0a1689971798/pulumi_kubernetes/apiregistration/v1/APIServiceList.py`

 * *Files identical despite different names*

### Comparing `pulumi_kubernetes-4.1.0a1689918291/pulumi_kubernetes/apiregistration/v1/APIServicePatch.py` & `pulumi_kubernetes-4.1.0a1689971798/pulumi_kubernetes/apiregistration/v1/APIServicePatch.py`

 * *Files identical despite different names*

### Comparing `pulumi_kubernetes-4.1.0a1689918291/pulumi_kubernetes/apiregistration/v1/_inputs.py` & `pulumi_kubernetes-4.1.0a1689971798/pulumi_kubernetes/apiregistration/v1/_inputs.py`

 * *Files identical despite different names*

### Comparing `pulumi_kubernetes-4.1.0a1689918291/pulumi_kubernetes/apiregistration/v1/outputs.py` & `pulumi_kubernetes-4.1.0a1689971798/pulumi_kubernetes/apiregistration/v1/outputs.py`

 * *Files identical despite different names*

### Comparing `pulumi_kubernetes-4.1.0a1689918291/pulumi_kubernetes/apiregistration/v1beta1/APIService.py` & `pulumi_kubernetes-4.1.0a1689971798/pulumi_kubernetes/apiregistration/v1beta1/APIService.py`

 * *Files identical despite different names*

### Comparing `pulumi_kubernetes-4.1.0a1689918291/pulumi_kubernetes/apiregistration/v1beta1/APIServiceList.py` & `pulumi_kubernetes-4.1.0a1689971798/pulumi_kubernetes/apiregistration/v1beta1/APIServiceList.py`

 * *Files identical despite different names*

### Comparing `pulumi_kubernetes-4.1.0a1689918291/pulumi_kubernetes/apiregistration/v1beta1/APIServicePatch.py` & `pulumi_kubernetes-4.1.0a1689971798/pulumi_kubernetes/apiregistration/v1beta1/APIServicePatch.py`

 * *Files identical despite different names*

### Comparing `pulumi_kubernetes-4.1.0a1689918291/pulumi_kubernetes/apiregistration/v1beta1/_inputs.py` & `pulumi_kubernetes-4.1.0a1689971798/pulumi_kubernetes/apiregistration/v1beta1/_inputs.py`

 * *Files identical despite different names*

### Comparing `pulumi_kubernetes-4.1.0a1689918291/pulumi_kubernetes/apiregistration/v1beta1/outputs.py` & `pulumi_kubernetes-4.1.0a1689971798/pulumi_kubernetes/apiregistration/v1beta1/outputs.py`

 * *Files identical despite different names*

### Comparing `pulumi_kubernetes-4.1.0a1689918291/pulumi_kubernetes/apps/__init__.py` & `pulumi_kubernetes-4.1.0a1689971798/pulumi_kubernetes/apps/__init__.py`

 * *Files identical despite different names*

### Comparing `pulumi_kubernetes-4.1.0a1689918291/pulumi_kubernetes/apps/v1/ControllerRevision.py` & `pulumi_kubernetes-4.1.0a1689971798/pulumi_kubernetes/apps/v1/ControllerRevision.py`

 * *Files identical despite different names*

### Comparing `pulumi_kubernetes-4.1.0a1689918291/pulumi_kubernetes/apps/v1/ControllerRevisionList.py` & `pulumi_kubernetes-4.1.0a1689971798/pulumi_kubernetes/apps/v1/ControllerRevisionList.py`

 * *Files identical despite different names*

### Comparing `pulumi_kubernetes-4.1.0a1689918291/pulumi_kubernetes/apps/v1/ControllerRevisionPatch.py` & `pulumi_kubernetes-4.1.0a1689971798/pulumi_kubernetes/apps/v1/ControllerRevisionPatch.py`

 * *Files identical despite different names*

### Comparing `pulumi_kubernetes-4.1.0a1689918291/pulumi_kubernetes/apps/v1/DaemonSet.py` & `pulumi_kubernetes-4.1.0a1689971798/pulumi_kubernetes/apps/v1/DaemonSet.py`

 * *Files identical despite different names*

### Comparing `pulumi_kubernetes-4.1.0a1689918291/pulumi_kubernetes/apps/v1/DaemonSetList.py` & `pulumi_kubernetes-4.1.0a1689971798/pulumi_kubernetes/apps/v1/DaemonSetList.py`

 * *Files identical despite different names*

### Comparing `pulumi_kubernetes-4.1.0a1689918291/pulumi_kubernetes/apps/v1/DaemonSetPatch.py` & `pulumi_kubernetes-4.1.0a1689971798/pulumi_kubernetes/apps/v1/DaemonSetPatch.py`

 * *Files identical despite different names*

### Comparing `pulumi_kubernetes-4.1.0a1689918291/pulumi_kubernetes/apps/v1/Deployment.py` & `pulumi_kubernetes-4.1.0a1689971798/pulumi_kubernetes/apps/v1/Deployment.py`

 * *Files identical despite different names*

### Comparing `pulumi_kubernetes-4.1.0a1689918291/pulumi_kubernetes/apps/v1/DeploymentList.py` & `pulumi_kubernetes-4.1.0a1689971798/pulumi_kubernetes/apps/v1/DeploymentList.py`

 * *Files identical despite different names*

### Comparing `pulumi_kubernetes-4.1.0a1689918291/pulumi_kubernetes/apps/v1/DeploymentPatch.py` & `pulumi_kubernetes-4.1.0a1689971798/pulumi_kubernetes/apps/v1/DeploymentPatch.py`

 * *Files identical despite different names*

### Comparing `pulumi_kubernetes-4.1.0a1689918291/pulumi_kubernetes/apps/v1/ReplicaSet.py` & `pulumi_kubernetes-4.1.0a1689971798/pulumi_kubernetes/apps/v1/ReplicaSet.py`

 * *Files identical despite different names*

### Comparing `pulumi_kubernetes-4.1.0a1689918291/pulumi_kubernetes/apps/v1/ReplicaSetList.py` & `pulumi_kubernetes-4.1.0a1689971798/pulumi_kubernetes/apps/v1/ReplicaSetList.py`

 * *Files identical despite different names*

### Comparing `pulumi_kubernetes-4.1.0a1689918291/pulumi_kubernetes/apps/v1/ReplicaSetPatch.py` & `pulumi_kubernetes-4.1.0a1689971798/pulumi_kubernetes/apps/v1/ReplicaSetPatch.py`

 * *Files identical despite different names*

### Comparing `pulumi_kubernetes-4.1.0a1689918291/pulumi_kubernetes/apps/v1/StatefulSet.py` & `pulumi_kubernetes-4.1.0a1689971798/pulumi_kubernetes/apps/v1/StatefulSet.py`

 * *Files identical despite different names*

### Comparing `pulumi_kubernetes-4.1.0a1689918291/pulumi_kubernetes/apps/v1/StatefulSetList.py` & `pulumi_kubernetes-4.1.0a1689971798/pulumi_kubernetes/apps/v1/StatefulSetList.py`

 * *Files identical despite different names*

### Comparing `pulumi_kubernetes-4.1.0a1689918291/pulumi_kubernetes/apps/v1/StatefulSetPatch.py` & `pulumi_kubernetes-4.1.0a1689971798/pulumi_kubernetes/apps/v1/StatefulSetPatch.py`

 * *Files identical despite different names*

### Comparing `pulumi_kubernetes-4.1.0a1689918291/pulumi_kubernetes/apps/v1/__init__.py` & `pulumi_kubernetes-4.1.0a1689971798/pulumi_kubernetes/apps/v1/__init__.py`

 * *Files identical despite different names*

### Comparing `pulumi_kubernetes-4.1.0a1689918291/pulumi_kubernetes/apps/v1/_inputs.py` & `pulumi_kubernetes-4.1.0a1689971798/pulumi_kubernetes/apps/v1/_inputs.py`

 * *Files identical despite different names*

### Comparing `pulumi_kubernetes-4.1.0a1689918291/pulumi_kubernetes/apps/v1/outputs.py` & `pulumi_kubernetes-4.1.0a1689971798/pulumi_kubernetes/apps/v1/outputs.py`

 * *Files identical despite different names*

### Comparing `pulumi_kubernetes-4.1.0a1689918291/pulumi_kubernetes/apps/v1beta1/ControllerRevision.py` & `pulumi_kubernetes-4.1.0a1689971798/pulumi_kubernetes/apps/v1beta1/ControllerRevision.py`

 * *Files identical despite different names*

### Comparing `pulumi_kubernetes-4.1.0a1689918291/pulumi_kubernetes/apps/v1beta1/ControllerRevisionList.py` & `pulumi_kubernetes-4.1.0a1689971798/pulumi_kubernetes/apps/v1beta1/ControllerRevisionList.py`

 * *Files identical despite different names*

### Comparing `pulumi_kubernetes-4.1.0a1689918291/pulumi_kubernetes/apps/v1beta1/ControllerRevisionPatch.py` & `pulumi_kubernetes-4.1.0a1689971798/pulumi_kubernetes/apps/v1beta1/ControllerRevisionPatch.py`

 * *Files identical despite different names*

### Comparing `pulumi_kubernetes-4.1.0a1689918291/pulumi_kubernetes/apps/v1beta1/Deployment.py` & `pulumi_kubernetes-4.1.0a1689971798/pulumi_kubernetes/apps/v1beta1/Deployment.py`

 * *Files identical despite different names*

### Comparing `pulumi_kubernetes-4.1.0a1689918291/pulumi_kubernetes/apps/v1beta1/DeploymentList.py` & `pulumi_kubernetes-4.1.0a1689971798/pulumi_kubernetes/apps/v1beta1/DeploymentList.py`

 * *Files identical despite different names*

### Comparing `pulumi_kubernetes-4.1.0a1689918291/pulumi_kubernetes/apps/v1beta1/DeploymentPatch.py` & `pulumi_kubernetes-4.1.0a1689971798/pulumi_kubernetes/apps/v1beta1/DeploymentPatch.py`

 * *Files identical despite different names*

### Comparing `pulumi_kubernetes-4.1.0a1689918291/pulumi_kubernetes/apps/v1beta1/StatefulSet.py` & `pulumi_kubernetes-4.1.0a1689971798/pulumi_kubernetes/apps/v1beta1/StatefulSet.py`

 * *Files identical despite different names*

### Comparing `pulumi_kubernetes-4.1.0a1689918291/pulumi_kubernetes/apps/v1beta1/StatefulSetList.py` & `pulumi_kubernetes-4.1.0a1689971798/pulumi_kubernetes/apps/v1beta1/StatefulSetList.py`

 * *Files identical despite different names*

### Comparing `pulumi_kubernetes-4.1.0a1689918291/pulumi_kubernetes/apps/v1beta1/StatefulSetPatch.py` & `pulumi_kubernetes-4.1.0a1689971798/pulumi_kubernetes/apps/v1beta1/StatefulSetPatch.py`

 * *Files identical despite different names*

### Comparing `pulumi_kubernetes-4.1.0a1689918291/pulumi_kubernetes/apps/v1beta1/__init__.py` & `pulumi_kubernetes-4.1.0a1689971798/pulumi_kubernetes/apps/v1beta1/__init__.py`

 * *Files identical despite different names*

### Comparing `pulumi_kubernetes-4.1.0a1689918291/pulumi_kubernetes/apps/v1beta1/_inputs.py` & `pulumi_kubernetes-4.1.0a1689971798/pulumi_kubernetes/apps/v1beta1/_inputs.py`

 * *Files identical despite different names*

### Comparing `pulumi_kubernetes-4.1.0a1689918291/pulumi_kubernetes/apps/v1beta1/outputs.py` & `pulumi_kubernetes-4.1.0a1689971798/pulumi_kubernetes/apps/v1beta1/outputs.py`

 * *Files identical despite different names*

### Comparing `pulumi_kubernetes-4.1.0a1689918291/pulumi_kubernetes/apps/v1beta2/ControllerRevision.py` & `pulumi_kubernetes-4.1.0a1689971798/pulumi_kubernetes/apps/v1beta2/ControllerRevision.py`

 * *Files identical despite different names*

### Comparing `pulumi_kubernetes-4.1.0a1689918291/pulumi_kubernetes/apps/v1beta2/ControllerRevisionList.py` & `pulumi_kubernetes-4.1.0a1689971798/pulumi_kubernetes/apps/v1beta2/ControllerRevisionList.py`

 * *Files identical despite different names*

### Comparing `pulumi_kubernetes-4.1.0a1689918291/pulumi_kubernetes/apps/v1beta2/ControllerRevisionPatch.py` & `pulumi_kubernetes-4.1.0a1689971798/pulumi_kubernetes/apps/v1beta2/ControllerRevisionPatch.py`

 * *Files identical despite different names*

### Comparing `pulumi_kubernetes-4.1.0a1689918291/pulumi_kubernetes/apps/v1beta2/DaemonSet.py` & `pulumi_kubernetes-4.1.0a1689971798/pulumi_kubernetes/apps/v1beta2/DaemonSet.py`

 * *Files identical despite different names*

### Comparing `pulumi_kubernetes-4.1.0a1689918291/pulumi_kubernetes/apps/v1beta2/DaemonSetList.py` & `pulumi_kubernetes-4.1.0a1689971798/pulumi_kubernetes/apps/v1beta2/DaemonSetList.py`

 * *Files identical despite different names*

### Comparing `pulumi_kubernetes-4.1.0a1689918291/pulumi_kubernetes/apps/v1beta2/DaemonSetPatch.py` & `pulumi_kubernetes-4.1.0a1689971798/pulumi_kubernetes/apps/v1beta2/DaemonSetPatch.py`

 * *Files identical despite different names*

### Comparing `pulumi_kubernetes-4.1.0a1689918291/pulumi_kubernetes/apps/v1beta2/Deployment.py` & `pulumi_kubernetes-4.1.0a1689971798/pulumi_kubernetes/apps/v1beta2/Deployment.py`

 * *Files identical despite different names*

### Comparing `pulumi_kubernetes-4.1.0a1689918291/pulumi_kubernetes/apps/v1beta2/DeploymentList.py` & `pulumi_kubernetes-4.1.0a1689971798/pulumi_kubernetes/apps/v1beta2/DeploymentList.py`

 * *Files identical despite different names*

### Comparing `pulumi_kubernetes-4.1.0a1689918291/pulumi_kubernetes/apps/v1beta2/DeploymentPatch.py` & `pulumi_kubernetes-4.1.0a1689971798/pulumi_kubernetes/apps/v1beta2/DeploymentPatch.py`

 * *Files identical despite different names*

### Comparing `pulumi_kubernetes-4.1.0a1689918291/pulumi_kubernetes/apps/v1beta2/ReplicaSet.py` & `pulumi_kubernetes-4.1.0a1689971798/pulumi_kubernetes/apps/v1beta2/ReplicaSet.py`

 * *Files identical despite different names*

### Comparing `pulumi_kubernetes-4.1.0a1689918291/pulumi_kubernetes/apps/v1beta2/ReplicaSetList.py` & `pulumi_kubernetes-4.1.0a1689971798/pulumi_kubernetes/apps/v1beta2/ReplicaSetList.py`

 * *Files identical despite different names*

### Comparing `pulumi_kubernetes-4.1.0a1689918291/pulumi_kubernetes/apps/v1beta2/ReplicaSetPatch.py` & `pulumi_kubernetes-4.1.0a1689971798/pulumi_kubernetes/apps/v1beta2/ReplicaSetPatch.py`

 * *Files identical despite different names*

### Comparing `pulumi_kubernetes-4.1.0a1689918291/pulumi_kubernetes/apps/v1beta2/StatefulSet.py` & `pulumi_kubernetes-4.1.0a1689971798/pulumi_kubernetes/apps/v1beta2/StatefulSet.py`

 * *Files identical despite different names*

### Comparing `pulumi_kubernetes-4.1.0a1689918291/pulumi_kubernetes/apps/v1beta2/StatefulSetList.py` & `pulumi_kubernetes-4.1.0a1689971798/pulumi_kubernetes/apps/v1beta2/StatefulSetList.py`

 * *Files identical despite different names*

### Comparing `pulumi_kubernetes-4.1.0a1689918291/pulumi_kubernetes/apps/v1beta2/StatefulSetPatch.py` & `pulumi_kubernetes-4.1.0a1689971798/pulumi_kubernetes/apps/v1beta2/StatefulSetPatch.py`

 * *Files identical despite different names*

### Comparing `pulumi_kubernetes-4.1.0a1689918291/pulumi_kubernetes/apps/v1beta2/__init__.py` & `pulumi_kubernetes-4.1.0a1689971798/pulumi_kubernetes/apps/v1beta2/__init__.py`

 * *Files identical despite different names*

### Comparing `pulumi_kubernetes-4.1.0a1689918291/pulumi_kubernetes/apps/v1beta2/_inputs.py` & `pulumi_kubernetes-4.1.0a1689971798/pulumi_kubernetes/apps/v1beta2/_inputs.py`

 * *Files identical despite different names*

### Comparing `pulumi_kubernetes-4.1.0a1689918291/pulumi_kubernetes/apps/v1beta2/outputs.py` & `pulumi_kubernetes-4.1.0a1689971798/pulumi_kubernetes/apps/v1beta2/outputs.py`

 * *Files identical despite different names*

### Comparing `pulumi_kubernetes-4.1.0a1689918291/pulumi_kubernetes/auditregistration/v1alpha1/AuditSink.py` & `pulumi_kubernetes-4.1.0a1689971798/pulumi_kubernetes/auditregistration/v1alpha1/AuditSink.py`

 * *Files identical despite different names*

### Comparing `pulumi_kubernetes-4.1.0a1689918291/pulumi_kubernetes/auditregistration/v1alpha1/AuditSinkList.py` & `pulumi_kubernetes-4.1.0a1689971798/pulumi_kubernetes/auditregistration/v1alpha1/AuditSinkList.py`

 * *Files identical despite different names*

### Comparing `pulumi_kubernetes-4.1.0a1689918291/pulumi_kubernetes/auditregistration/v1alpha1/AuditSinkPatch.py` & `pulumi_kubernetes-4.1.0a1689971798/pulumi_kubernetes/auditregistration/v1alpha1/AuditSinkPatch.py`

 * *Files identical despite different names*

### Comparing `pulumi_kubernetes-4.1.0a1689918291/pulumi_kubernetes/auditregistration/v1alpha1/_inputs.py` & `pulumi_kubernetes-4.1.0a1689971798/pulumi_kubernetes/auditregistration/v1alpha1/_inputs.py`

 * *Files identical despite different names*

### Comparing `pulumi_kubernetes-4.1.0a1689918291/pulumi_kubernetes/auditregistration/v1alpha1/outputs.py` & `pulumi_kubernetes-4.1.0a1689971798/pulumi_kubernetes/auditregistration/v1alpha1/outputs.py`

 * *Files identical despite different names*

### Comparing `pulumi_kubernetes-4.1.0a1689918291/pulumi_kubernetes/autoscaling/__init__.py` & `pulumi_kubernetes-4.1.0a1689971798/pulumi_kubernetes/autoscaling/__init__.py`

 * *Files identical despite different names*

### Comparing `pulumi_kubernetes-4.1.0a1689918291/pulumi_kubernetes/autoscaling/v1/HorizontalPodAutoscaler.py` & `pulumi_kubernetes-4.1.0a1689971798/pulumi_kubernetes/autoscaling/v1/HorizontalPodAutoscaler.py`

 * *Files identical despite different names*

### Comparing `pulumi_kubernetes-4.1.0a1689918291/pulumi_kubernetes/autoscaling/v1/HorizontalPodAutoscalerList.py` & `pulumi_kubernetes-4.1.0a1689971798/pulumi_kubernetes/autoscaling/v1/HorizontalPodAutoscalerList.py`

 * *Files identical despite different names*

### Comparing `pulumi_kubernetes-4.1.0a1689918291/pulumi_kubernetes/autoscaling/v1/HorizontalPodAutoscalerPatch.py` & `pulumi_kubernetes-4.1.0a1689971798/pulumi_kubernetes/autoscaling/v1/HorizontalPodAutoscalerPatch.py`

 * *Files identical despite different names*

### Comparing `pulumi_kubernetes-4.1.0a1689918291/pulumi_kubernetes/autoscaling/v1/_inputs.py` & `pulumi_kubernetes-4.1.0a1689971798/pulumi_kubernetes/autoscaling/v1/_inputs.py`

 * *Files identical despite different names*

### Comparing `pulumi_kubernetes-4.1.0a1689918291/pulumi_kubernetes/autoscaling/v1/outputs.py` & `pulumi_kubernetes-4.1.0a1689971798/pulumi_kubernetes/autoscaling/v1/outputs.py`

 * *Files identical despite different names*

### Comparing `pulumi_kubernetes-4.1.0a1689918291/pulumi_kubernetes/autoscaling/v2/HorizontalPodAutoscaler.py` & `pulumi_kubernetes-4.1.0a1689971798/pulumi_kubernetes/autoscaling/v2/HorizontalPodAutoscaler.py`

 * *Files identical despite different names*

### Comparing `pulumi_kubernetes-4.1.0a1689918291/pulumi_kubernetes/autoscaling/v2/HorizontalPodAutoscalerList.py` & `pulumi_kubernetes-4.1.0a1689971798/pulumi_kubernetes/autoscaling/v2/HorizontalPodAutoscalerList.py`

 * *Files identical despite different names*

### Comparing `pulumi_kubernetes-4.1.0a1689918291/pulumi_kubernetes/autoscaling/v2/HorizontalPodAutoscalerPatch.py` & `pulumi_kubernetes-4.1.0a1689971798/pulumi_kubernetes/autoscaling/v2/HorizontalPodAutoscalerPatch.py`

 * *Files identical despite different names*

### Comparing `pulumi_kubernetes-4.1.0a1689918291/pulumi_kubernetes/autoscaling/v2/_inputs.py` & `pulumi_kubernetes-4.1.0a1689971798/pulumi_kubernetes/autoscaling/v2/_inputs.py`

 * *Files identical despite different names*

### Comparing `pulumi_kubernetes-4.1.0a1689918291/pulumi_kubernetes/autoscaling/v2/outputs.py` & `pulumi_kubernetes-4.1.0a1689971798/pulumi_kubernetes/autoscaling/v2/outputs.py`

 * *Files identical despite different names*

### Comparing `pulumi_kubernetes-4.1.0a1689918291/pulumi_kubernetes/autoscaling/v2beta1/HorizontalPodAutoscaler.py` & `pulumi_kubernetes-4.1.0a1689971798/pulumi_kubernetes/autoscaling/v2beta1/HorizontalPodAutoscaler.py`

 * *Files identical despite different names*

### Comparing `pulumi_kubernetes-4.1.0a1689918291/pulumi_kubernetes/autoscaling/v2beta1/HorizontalPodAutoscalerList.py` & `pulumi_kubernetes-4.1.0a1689971798/pulumi_kubernetes/autoscaling/v2beta1/HorizontalPodAutoscalerList.py`

 * *Files identical despite different names*

### Comparing `pulumi_kubernetes-4.1.0a1689918291/pulumi_kubernetes/autoscaling/v2beta1/HorizontalPodAutoscalerPatch.py` & `pulumi_kubernetes-4.1.0a1689971798/pulumi_kubernetes/autoscaling/v2beta1/HorizontalPodAutoscalerPatch.py`

 * *Files identical despite different names*

### Comparing `pulumi_kubernetes-4.1.0a1689918291/pulumi_kubernetes/autoscaling/v2beta1/_inputs.py` & `pulumi_kubernetes-4.1.0a1689971798/pulumi_kubernetes/autoscaling/v2beta1/_inputs.py`

 * *Files identical despite different names*

### Comparing `pulumi_kubernetes-4.1.0a1689918291/pulumi_kubernetes/autoscaling/v2beta1/outputs.py` & `pulumi_kubernetes-4.1.0a1689971798/pulumi_kubernetes/autoscaling/v2beta1/outputs.py`

 * *Files identical despite different names*

### Comparing `pulumi_kubernetes-4.1.0a1689918291/pulumi_kubernetes/autoscaling/v2beta2/HorizontalPodAutoscaler.py` & `pulumi_kubernetes-4.1.0a1689971798/pulumi_kubernetes/autoscaling/v2beta2/HorizontalPodAutoscaler.py`

 * *Files identical despite different names*

### Comparing `pulumi_kubernetes-4.1.0a1689918291/pulumi_kubernetes/autoscaling/v2beta2/HorizontalPodAutoscalerList.py` & `pulumi_kubernetes-4.1.0a1689971798/pulumi_kubernetes/autoscaling/v2beta2/HorizontalPodAutoscalerList.py`

 * *Files identical despite different names*

### Comparing `pulumi_kubernetes-4.1.0a1689918291/pulumi_kubernetes/autoscaling/v2beta2/HorizontalPodAutoscalerPatch.py` & `pulumi_kubernetes-4.1.0a1689971798/pulumi_kubernetes/autoscaling/v2beta2/HorizontalPodAutoscalerPatch.py`

 * *Files identical despite different names*

### Comparing `pulumi_kubernetes-4.1.0a1689918291/pulumi_kubernetes/autoscaling/v2beta2/_inputs.py` & `pulumi_kubernetes-4.1.0a1689971798/pulumi_kubernetes/autoscaling/v2beta2/_inputs.py`

 * *Files identical despite different names*

### Comparing `pulumi_kubernetes-4.1.0a1689918291/pulumi_kubernetes/autoscaling/v2beta2/outputs.py` & `pulumi_kubernetes-4.1.0a1689971798/pulumi_kubernetes/autoscaling/v2beta2/outputs.py`

 * *Files identical despite different names*

### Comparing `pulumi_kubernetes-4.1.0a1689918291/pulumi_kubernetes/batch/__init__.py` & `pulumi_kubernetes-4.1.0a1689971798/pulumi_kubernetes/batch/__init__.py`

 * *Files identical despite different names*

### Comparing `pulumi_kubernetes-4.1.0a1689918291/pulumi_kubernetes/batch/v1/CronJob.py` & `pulumi_kubernetes-4.1.0a1689971798/pulumi_kubernetes/batch/v1/CronJob.py`

 * *Files identical despite different names*

### Comparing `pulumi_kubernetes-4.1.0a1689918291/pulumi_kubernetes/batch/v1/CronJobList.py` & `pulumi_kubernetes-4.1.0a1689971798/pulumi_kubernetes/batch/v1/CronJobList.py`

 * *Files identical despite different names*

### Comparing `pulumi_kubernetes-4.1.0a1689918291/pulumi_kubernetes/batch/v1/CronJobPatch.py` & `pulumi_kubernetes-4.1.0a1689971798/pulumi_kubernetes/batch/v1/CronJobPatch.py`

 * *Files identical despite different names*

### Comparing `pulumi_kubernetes-4.1.0a1689918291/pulumi_kubernetes/batch/v1/Job.py` & `pulumi_kubernetes-4.1.0a1689971798/pulumi_kubernetes/batch/v1/Job.py`

 * *Files identical despite different names*

### Comparing `pulumi_kubernetes-4.1.0a1689918291/pulumi_kubernetes/batch/v1/JobList.py` & `pulumi_kubernetes-4.1.0a1689971798/pulumi_kubernetes/batch/v1/JobList.py`

 * *Files identical despite different names*

### Comparing `pulumi_kubernetes-4.1.0a1689918291/pulumi_kubernetes/batch/v1/JobPatch.py` & `pulumi_kubernetes-4.1.0a1689971798/pulumi_kubernetes/batch/v1/JobPatch.py`

 * *Files identical despite different names*

### Comparing `pulumi_kubernetes-4.1.0a1689918291/pulumi_kubernetes/batch/v1/_inputs.py` & `pulumi_kubernetes-4.1.0a1689971798/pulumi_kubernetes/batch/v1/_inputs.py`

 * *Files identical despite different names*

### Comparing `pulumi_kubernetes-4.1.0a1689918291/pulumi_kubernetes/batch/v1/outputs.py` & `pulumi_kubernetes-4.1.0a1689971798/pulumi_kubernetes/batch/v1/outputs.py`

 * *Files identical despite different names*

### Comparing `pulumi_kubernetes-4.1.0a1689918291/pulumi_kubernetes/batch/v1beta1/CronJob.py` & `pulumi_kubernetes-4.1.0a1689971798/pulumi_kubernetes/batch/v1beta1/CronJob.py`

 * *Files identical despite different names*

### Comparing `pulumi_kubernetes-4.1.0a1689918291/pulumi_kubernetes/batch/v1beta1/CronJobList.py` & `pulumi_kubernetes-4.1.0a1689971798/pulumi_kubernetes/batch/v1beta1/CronJobList.py`

 * *Files identical despite different names*

### Comparing `pulumi_kubernetes-4.1.0a1689918291/pulumi_kubernetes/batch/v1beta1/CronJobPatch.py` & `pulumi_kubernetes-4.1.0a1689971798/pulumi_kubernetes/batch/v1beta1/CronJobPatch.py`

 * *Files identical despite different names*

### Comparing `pulumi_kubernetes-4.1.0a1689918291/pulumi_kubernetes/batch/v1beta1/_inputs.py` & `pulumi_kubernetes-4.1.0a1689971798/pulumi_kubernetes/batch/v1beta1/_inputs.py`

 * *Files identical despite different names*

### Comparing `pulumi_kubernetes-4.1.0a1689918291/pulumi_kubernetes/batch/v1beta1/outputs.py` & `pulumi_kubernetes-4.1.0a1689971798/pulumi_kubernetes/batch/v1beta1/outputs.py`

 * *Files identical despite different names*

### Comparing `pulumi_kubernetes-4.1.0a1689918291/pulumi_kubernetes/batch/v2alpha1/CronJob.py` & `pulumi_kubernetes-4.1.0a1689971798/pulumi_kubernetes/batch/v2alpha1/CronJob.py`

 * *Files identical despite different names*

### Comparing `pulumi_kubernetes-4.1.0a1689918291/pulumi_kubernetes/batch/v2alpha1/CronJobList.py` & `pulumi_kubernetes-4.1.0a1689971798/pulumi_kubernetes/batch/v2alpha1/CronJobList.py`

 * *Files identical despite different names*

### Comparing `pulumi_kubernetes-4.1.0a1689918291/pulumi_kubernetes/batch/v2alpha1/CronJobPatch.py` & `pulumi_kubernetes-4.1.0a1689971798/pulumi_kubernetes/batch/v2alpha1/CronJobPatch.py`

 * *Files identical despite different names*

### Comparing `pulumi_kubernetes-4.1.0a1689918291/pulumi_kubernetes/batch/v2alpha1/_inputs.py` & `pulumi_kubernetes-4.1.0a1689971798/pulumi_kubernetes/batch/v2alpha1/_inputs.py`

 * *Files identical despite different names*

### Comparing `pulumi_kubernetes-4.1.0a1689918291/pulumi_kubernetes/batch/v2alpha1/outputs.py` & `pulumi_kubernetes-4.1.0a1689971798/pulumi_kubernetes/batch/v2alpha1/outputs.py`

 * *Files identical despite different names*

### Comparing `pulumi_kubernetes-4.1.0a1689918291/pulumi_kubernetes/certificates/__init__.py` & `pulumi_kubernetes-4.1.0a1689971798/pulumi_kubernetes/certificates/__init__.py`

 * *Files identical despite different names*

### Comparing `pulumi_kubernetes-4.1.0a1689918291/pulumi_kubernetes/certificates/v1/CertificateSigningRequest.py` & `pulumi_kubernetes-4.1.0a1689971798/pulumi_kubernetes/certificates/v1/CertificateSigningRequest.py`

 * *Files identical despite different names*

### Comparing `pulumi_kubernetes-4.1.0a1689918291/pulumi_kubernetes/certificates/v1/CertificateSigningRequestList.py` & `pulumi_kubernetes-4.1.0a1689971798/pulumi_kubernetes/certificates/v1/CertificateSigningRequestList.py`

 * *Files identical despite different names*

### Comparing `pulumi_kubernetes-4.1.0a1689918291/pulumi_kubernetes/certificates/v1/CertificateSigningRequestPatch.py` & `pulumi_kubernetes-4.1.0a1689971798/pulumi_kubernetes/certificates/v1/CertificateSigningRequestPatch.py`

 * *Files identical despite different names*

### Comparing `pulumi_kubernetes-4.1.0a1689918291/pulumi_kubernetes/certificates/v1/_inputs.py` & `pulumi_kubernetes-4.1.0a1689971798/pulumi_kubernetes/certificates/v1/_inputs.py`

 * *Files identical despite different names*

### Comparing `pulumi_kubernetes-4.1.0a1689918291/pulumi_kubernetes/certificates/v1/outputs.py` & `pulumi_kubernetes-4.1.0a1689971798/pulumi_kubernetes/certificates/v1/outputs.py`

 * *Files identical despite different names*

### Comparing `pulumi_kubernetes-4.1.0a1689918291/pulumi_kubernetes/certificates/v1alpha1/ClusterTrustBundle.py` & `pulumi_kubernetes-4.1.0a1689971798/pulumi_kubernetes/certificates/v1alpha1/ClusterTrustBundle.py`

 * *Files identical despite different names*

### Comparing `pulumi_kubernetes-4.1.0a1689918291/pulumi_kubernetes/certificates/v1alpha1/ClusterTrustBundleList.py` & `pulumi_kubernetes-4.1.0a1689971798/pulumi_kubernetes/certificates/v1alpha1/ClusterTrustBundleList.py`

 * *Files identical despite different names*

### Comparing `pulumi_kubernetes-4.1.0a1689918291/pulumi_kubernetes/certificates/v1alpha1/ClusterTrustBundlePatch.py` & `pulumi_kubernetes-4.1.0a1689971798/pulumi_kubernetes/certificates/v1alpha1/ClusterTrustBundlePatch.py`

 * *Files identical despite different names*

### Comparing `pulumi_kubernetes-4.1.0a1689918291/pulumi_kubernetes/certificates/v1alpha1/_inputs.py` & `pulumi_kubernetes-4.1.0a1689971798/pulumi_kubernetes/certificates/v1alpha1/_inputs.py`

 * *Files identical despite different names*

### Comparing `pulumi_kubernetes-4.1.0a1689918291/pulumi_kubernetes/certificates/v1alpha1/outputs.py` & `pulumi_kubernetes-4.1.0a1689971798/pulumi_kubernetes/certificates/v1alpha1/outputs.py`

 * *Files identical despite different names*

### Comparing `pulumi_kubernetes-4.1.0a1689918291/pulumi_kubernetes/certificates/v1beta1/CertificateSigningRequest.py` & `pulumi_kubernetes-4.1.0a1689971798/pulumi_kubernetes/certificates/v1beta1/CertificateSigningRequest.py`

 * *Files identical despite different names*

### Comparing `pulumi_kubernetes-4.1.0a1689918291/pulumi_kubernetes/certificates/v1beta1/CertificateSigningRequestList.py` & `pulumi_kubernetes-4.1.0a1689971798/pulumi_kubernetes/certificates/v1beta1/CertificateSigningRequestList.py`

 * *Files identical despite different names*

### Comparing `pulumi_kubernetes-4.1.0a1689918291/pulumi_kubernetes/certificates/v1beta1/CertificateSigningRequestPatch.py` & `pulumi_kubernetes-4.1.0a1689971798/pulumi_kubernetes/certificates/v1beta1/CertificateSigningRequestPatch.py`

 * *Files identical despite different names*

### Comparing `pulumi_kubernetes-4.1.0a1689918291/pulumi_kubernetes/certificates/v1beta1/_inputs.py` & `pulumi_kubernetes-4.1.0a1689971798/pulumi_kubernetes/certificates/v1beta1/_inputs.py`

 * *Files identical despite different names*

### Comparing `pulumi_kubernetes-4.1.0a1689918291/pulumi_kubernetes/certificates/v1beta1/outputs.py` & `pulumi_kubernetes-4.1.0a1689971798/pulumi_kubernetes/certificates/v1beta1/outputs.py`

 * *Files identical despite different names*

### Comparing `pulumi_kubernetes-4.1.0a1689918291/pulumi_kubernetes/coordination/__init__.py` & `pulumi_kubernetes-4.1.0a1689971798/pulumi_kubernetes/coordination/__init__.py`

 * *Files identical despite different names*

### Comparing `pulumi_kubernetes-4.1.0a1689918291/pulumi_kubernetes/coordination/v1/Lease.py` & `pulumi_kubernetes-4.1.0a1689971798/pulumi_kubernetes/coordination/v1/Lease.py`

 * *Files identical despite different names*

### Comparing `pulumi_kubernetes-4.1.0a1689918291/pulumi_kubernetes/coordination/v1/LeaseList.py` & `pulumi_kubernetes-4.1.0a1689971798/pulumi_kubernetes/coordination/v1/LeaseList.py`

 * *Files identical despite different names*

### Comparing `pulumi_kubernetes-4.1.0a1689918291/pulumi_kubernetes/coordination/v1/LeasePatch.py` & `pulumi_kubernetes-4.1.0a1689971798/pulumi_kubernetes/coordination/v1/LeasePatch.py`

 * *Files identical despite different names*

### Comparing `pulumi_kubernetes-4.1.0a1689918291/pulumi_kubernetes/coordination/v1/_inputs.py` & `pulumi_kubernetes-4.1.0a1689971798/pulumi_kubernetes/coordination/v1/_inputs.py`

 * *Files identical despite different names*

### Comparing `pulumi_kubernetes-4.1.0a1689918291/pulumi_kubernetes/coordination/v1/outputs.py` & `pulumi_kubernetes-4.1.0a1689971798/pulumi_kubernetes/coordination/v1/outputs.py`

 * *Files identical despite different names*

### Comparing `pulumi_kubernetes-4.1.0a1689918291/pulumi_kubernetes/coordination/v1beta1/Lease.py` & `pulumi_kubernetes-4.1.0a1689971798/pulumi_kubernetes/coordination/v1beta1/Lease.py`

 * *Files identical despite different names*

### Comparing `pulumi_kubernetes-4.1.0a1689918291/pulumi_kubernetes/coordination/v1beta1/LeaseList.py` & `pulumi_kubernetes-4.1.0a1689971798/pulumi_kubernetes/coordination/v1beta1/LeaseList.py`

 * *Files identical despite different names*

### Comparing `pulumi_kubernetes-4.1.0a1689918291/pulumi_kubernetes/coordination/v1beta1/LeasePatch.py` & `pulumi_kubernetes-4.1.0a1689971798/pulumi_kubernetes/coordination/v1beta1/LeasePatch.py`

 * *Files identical despite different names*

### Comparing `pulumi_kubernetes-4.1.0a1689918291/pulumi_kubernetes/coordination/v1beta1/_inputs.py` & `pulumi_kubernetes-4.1.0a1689971798/pulumi_kubernetes/coordination/v1beta1/_inputs.py`

 * *Files identical despite different names*

### Comparing `pulumi_kubernetes-4.1.0a1689918291/pulumi_kubernetes/coordination/v1beta1/outputs.py` & `pulumi_kubernetes-4.1.0a1689971798/pulumi_kubernetes/coordination/v1beta1/outputs.py`

 * *Files identical despite different names*

### Comparing `pulumi_kubernetes-4.1.0a1689918291/pulumi_kubernetes/core/v1/Binding.py` & `pulumi_kubernetes-4.1.0a1689971798/pulumi_kubernetes/core/v1/Binding.py`

 * *Files identical despite different names*

### Comparing `pulumi_kubernetes-4.1.0a1689918291/pulumi_kubernetes/core/v1/BindingPatch.py` & `pulumi_kubernetes-4.1.0a1689971798/pulumi_kubernetes/core/v1/BindingPatch.py`

 * *Files identical despite different names*

### Comparing `pulumi_kubernetes-4.1.0a1689918291/pulumi_kubernetes/core/v1/ConfigMap.py` & `pulumi_kubernetes-4.1.0a1689971798/pulumi_kubernetes/core/v1/ConfigMap.py`

 * *Files identical despite different names*

### Comparing `pulumi_kubernetes-4.1.0a1689918291/pulumi_kubernetes/core/v1/ConfigMapList.py` & `pulumi_kubernetes-4.1.0a1689971798/pulumi_kubernetes/core/v1/ConfigMapList.py`

 * *Files identical despite different names*

### Comparing `pulumi_kubernetes-4.1.0a1689918291/pulumi_kubernetes/core/v1/ConfigMapPatch.py` & `pulumi_kubernetes-4.1.0a1689971798/pulumi_kubernetes/core/v1/ConfigMapPatch.py`

 * *Files identical despite different names*

### Comparing `pulumi_kubernetes-4.1.0a1689918291/pulumi_kubernetes/core/v1/Endpoints.py` & `pulumi_kubernetes-4.1.0a1689971798/pulumi_kubernetes/core/v1/Endpoints.py`

 * *Files identical despite different names*

### Comparing `pulumi_kubernetes-4.1.0a1689918291/pulumi_kubernetes/core/v1/EndpointsList.py` & `pulumi_kubernetes-4.1.0a1689971798/pulumi_kubernetes/core/v1/EndpointsList.py`

 * *Files identical despite different names*

### Comparing `pulumi_kubernetes-4.1.0a1689918291/pulumi_kubernetes/core/v1/EndpointsPatch.py` & `pulumi_kubernetes-4.1.0a1689971798/pulumi_kubernetes/core/v1/EndpointsPatch.py`

 * *Files identical despite different names*

### Comparing `pulumi_kubernetes-4.1.0a1689918291/pulumi_kubernetes/core/v1/Event.py` & `pulumi_kubernetes-4.1.0a1689971798/pulumi_kubernetes/core/v1/Event.py`

 * *Files identical despite different names*

### Comparing `pulumi_kubernetes-4.1.0a1689918291/pulumi_kubernetes/core/v1/EventList.py` & `pulumi_kubernetes-4.1.0a1689971798/pulumi_kubernetes/core/v1/EventList.py`

 * *Files identical despite different names*

### Comparing `pulumi_kubernetes-4.1.0a1689918291/pulumi_kubernetes/core/v1/EventPatch.py` & `pulumi_kubernetes-4.1.0a1689971798/pulumi_kubernetes/core/v1/EventPatch.py`

 * *Files identical despite different names*

### Comparing `pulumi_kubernetes-4.1.0a1689918291/pulumi_kubernetes/core/v1/LimitRange.py` & `pulumi_kubernetes-4.1.0a1689971798/pulumi_kubernetes/core/v1/LimitRange.py`

 * *Files identical despite different names*

### Comparing `pulumi_kubernetes-4.1.0a1689918291/pulumi_kubernetes/core/v1/LimitRangeList.py` & `pulumi_kubernetes-4.1.0a1689971798/pulumi_kubernetes/core/v1/LimitRangeList.py`

 * *Files identical despite different names*

### Comparing `pulumi_kubernetes-4.1.0a1689918291/pulumi_kubernetes/core/v1/LimitRangePatch.py` & `pulumi_kubernetes-4.1.0a1689971798/pulumi_kubernetes/core/v1/LimitRangePatch.py`

 * *Files identical despite different names*

### Comparing `pulumi_kubernetes-4.1.0a1689918291/pulumi_kubernetes/core/v1/Namespace.py` & `pulumi_kubernetes-4.1.0a1689971798/pulumi_kubernetes/core/v1/Namespace.py`

 * *Files identical despite different names*

### Comparing `pulumi_kubernetes-4.1.0a1689918291/pulumi_kubernetes/core/v1/NamespaceList.py` & `pulumi_kubernetes-4.1.0a1689971798/pulumi_kubernetes/core/v1/NamespaceList.py`

 * *Files identical despite different names*

### Comparing `pulumi_kubernetes-4.1.0a1689918291/pulumi_kubernetes/core/v1/NamespacePatch.py` & `pulumi_kubernetes-4.1.0a1689971798/pulumi_kubernetes/core/v1/NamespacePatch.py`

 * *Files identical despite different names*

### Comparing `pulumi_kubernetes-4.1.0a1689918291/pulumi_kubernetes/core/v1/Node.py` & `pulumi_kubernetes-4.1.0a1689971798/pulumi_kubernetes/core/v1/Node.py`

 * *Files identical despite different names*

### Comparing `pulumi_kubernetes-4.1.0a1689918291/pulumi_kubernetes/core/v1/NodeList.py` & `pulumi_kubernetes-4.1.0a1689971798/pulumi_kubernetes/core/v1/NodeList.py`

 * *Files identical despite different names*

### Comparing `pulumi_kubernetes-4.1.0a1689918291/pulumi_kubernetes/core/v1/NodePatch.py` & `pulumi_kubernetes-4.1.0a1689971798/pulumi_kubernetes/core/v1/NodePatch.py`

 * *Files identical despite different names*

### Comparing `pulumi_kubernetes-4.1.0a1689918291/pulumi_kubernetes/core/v1/PersistentVolume.py` & `pulumi_kubernetes-4.1.0a1689971798/pulumi_kubernetes/core/v1/PersistentVolume.py`

 * *Files identical despite different names*

### Comparing `pulumi_kubernetes-4.1.0a1689918291/pulumi_kubernetes/core/v1/PersistentVolumeClaim.py` & `pulumi_kubernetes-4.1.0a1689971798/pulumi_kubernetes/core/v1/PersistentVolumeClaim.py`

 * *Files identical despite different names*

### Comparing `pulumi_kubernetes-4.1.0a1689918291/pulumi_kubernetes/core/v1/PersistentVolumeClaimList.py` & `pulumi_kubernetes-4.1.0a1689971798/pulumi_kubernetes/core/v1/PersistentVolumeClaimList.py`

 * *Files identical despite different names*

### Comparing `pulumi_kubernetes-4.1.0a1689918291/pulumi_kubernetes/core/v1/PersistentVolumeClaimPatch.py` & `pulumi_kubernetes-4.1.0a1689971798/pulumi_kubernetes/core/v1/PersistentVolumeClaimPatch.py`

 * *Files identical despite different names*

### Comparing `pulumi_kubernetes-4.1.0a1689918291/pulumi_kubernetes/core/v1/PersistentVolumeList.py` & `pulumi_kubernetes-4.1.0a1689971798/pulumi_kubernetes/core/v1/PersistentVolumeList.py`

 * *Files identical despite different names*

### Comparing `pulumi_kubernetes-4.1.0a1689918291/pulumi_kubernetes/core/v1/PersistentVolumePatch.py` & `pulumi_kubernetes-4.1.0a1689971798/pulumi_kubernetes/core/v1/PersistentVolumePatch.py`

 * *Files identical despite different names*

### Comparing `pulumi_kubernetes-4.1.0a1689918291/pulumi_kubernetes/core/v1/Pod.py` & `pulumi_kubernetes-4.1.0a1689971798/pulumi_kubernetes/core/v1/Pod.py`

 * *Files identical despite different names*

### Comparing `pulumi_kubernetes-4.1.0a1689918291/pulumi_kubernetes/core/v1/PodList.py` & `pulumi_kubernetes-4.1.0a1689971798/pulumi_kubernetes/core/v1/PodList.py`

 * *Files identical despite different names*

### Comparing `pulumi_kubernetes-4.1.0a1689918291/pulumi_kubernetes/core/v1/PodPatch.py` & `pulumi_kubernetes-4.1.0a1689971798/pulumi_kubernetes/core/v1/PodPatch.py`

 * *Files identical despite different names*

### Comparing `pulumi_kubernetes-4.1.0a1689918291/pulumi_kubernetes/core/v1/PodTemplate.py` & `pulumi_kubernetes-4.1.0a1689971798/pulumi_kubernetes/core/v1/PodTemplate.py`

 * *Files identical despite different names*

### Comparing `pulumi_kubernetes-4.1.0a1689918291/pulumi_kubernetes/core/v1/PodTemplateList.py` & `pulumi_kubernetes-4.1.0a1689971798/pulumi_kubernetes/core/v1/PodTemplateList.py`

 * *Files identical despite different names*

### Comparing `pulumi_kubernetes-4.1.0a1689918291/pulumi_kubernetes/core/v1/PodTemplatePatch.py` & `pulumi_kubernetes-4.1.0a1689971798/pulumi_kubernetes/core/v1/PodTemplatePatch.py`

 * *Files identical despite different names*

### Comparing `pulumi_kubernetes-4.1.0a1689918291/pulumi_kubernetes/core/v1/ReplicationController.py` & `pulumi_kubernetes-4.1.0a1689971798/pulumi_kubernetes/core/v1/ReplicationController.py`

 * *Files identical despite different names*

### Comparing `pulumi_kubernetes-4.1.0a1689918291/pulumi_kubernetes/core/v1/ReplicationControllerList.py` & `pulumi_kubernetes-4.1.0a1689971798/pulumi_kubernetes/core/v1/ReplicationControllerList.py`

 * *Files identical despite different names*

### Comparing `pulumi_kubernetes-4.1.0a1689918291/pulumi_kubernetes/core/v1/ReplicationControllerPatch.py` & `pulumi_kubernetes-4.1.0a1689971798/pulumi_kubernetes/core/v1/ReplicationControllerPatch.py`

 * *Files identical despite different names*

### Comparing `pulumi_kubernetes-4.1.0a1689918291/pulumi_kubernetes/core/v1/ResourceQuota.py` & `pulumi_kubernetes-4.1.0a1689971798/pulumi_kubernetes/core/v1/ResourceQuota.py`

 * *Files identical despite different names*

### Comparing `pulumi_kubernetes-4.1.0a1689918291/pulumi_kubernetes/core/v1/ResourceQuotaList.py` & `pulumi_kubernetes-4.1.0a1689971798/pulumi_kubernetes/core/v1/ResourceQuotaList.py`

 * *Files identical despite different names*

### Comparing `pulumi_kubernetes-4.1.0a1689918291/pulumi_kubernetes/core/v1/ResourceQuotaPatch.py` & `pulumi_kubernetes-4.1.0a1689971798/pulumi_kubernetes/core/v1/ResourceQuotaPatch.py`

 * *Files identical despite different names*

### Comparing `pulumi_kubernetes-4.1.0a1689918291/pulumi_kubernetes/core/v1/Secret.py` & `pulumi_kubernetes-4.1.0a1689971798/pulumi_kubernetes/core/v1/Secret.py`

 * *Files identical despite different names*

### Comparing `pulumi_kubernetes-4.1.0a1689918291/pulumi_kubernetes/core/v1/SecretList.py` & `pulumi_kubernetes-4.1.0a1689971798/pulumi_kubernetes/core/v1/SecretList.py`

 * *Files identical despite different names*

### Comparing `pulumi_kubernetes-4.1.0a1689918291/pulumi_kubernetes/core/v1/SecretPatch.py` & `pulumi_kubernetes-4.1.0a1689971798/pulumi_kubernetes/core/v1/SecretPatch.py`

 * *Files identical despite different names*

### Comparing `pulumi_kubernetes-4.1.0a1689918291/pulumi_kubernetes/core/v1/Service.py` & `pulumi_kubernetes-4.1.0a1689971798/pulumi_kubernetes/core/v1/Service.py`

 * *Files identical despite different names*

### Comparing `pulumi_kubernetes-4.1.0a1689918291/pulumi_kubernetes/core/v1/ServiceAccount.py` & `pulumi_kubernetes-4.1.0a1689971798/pulumi_kubernetes/core/v1/ServiceAccount.py`

 * *Files identical despite different names*

### Comparing `pulumi_kubernetes-4.1.0a1689918291/pulumi_kubernetes/core/v1/ServiceAccountList.py` & `pulumi_kubernetes-4.1.0a1689971798/pulumi_kubernetes/core/v1/ServiceAccountList.py`

 * *Files identical despite different names*

### Comparing `pulumi_kubernetes-4.1.0a1689918291/pulumi_kubernetes/core/v1/ServiceAccountPatch.py` & `pulumi_kubernetes-4.1.0a1689971798/pulumi_kubernetes/core/v1/ServiceAccountPatch.py`

 * *Files identical despite different names*

### Comparing `pulumi_kubernetes-4.1.0a1689918291/pulumi_kubernetes/core/v1/ServiceList.py` & `pulumi_kubernetes-4.1.0a1689971798/pulumi_kubernetes/core/v1/ServiceList.py`

 * *Files identical despite different names*

### Comparing `pulumi_kubernetes-4.1.0a1689918291/pulumi_kubernetes/core/v1/ServicePatch.py` & `pulumi_kubernetes-4.1.0a1689971798/pulumi_kubernetes/core/v1/ServicePatch.py`

 * *Files identical despite different names*

### Comparing `pulumi_kubernetes-4.1.0a1689918291/pulumi_kubernetes/core/v1/__init__.py` & `pulumi_kubernetes-4.1.0a1689971798/pulumi_kubernetes/core/v1/__init__.py`

 * *Files identical despite different names*

### Comparing `pulumi_kubernetes-4.1.0a1689918291/pulumi_kubernetes/core/v1/_inputs.py` & `pulumi_kubernetes-4.1.0a1689971798/pulumi_kubernetes/core/v1/_inputs.py`

 * *Files identical despite different names*

### Comparing `pulumi_kubernetes-4.1.0a1689918291/pulumi_kubernetes/core/v1/outputs.py` & `pulumi_kubernetes-4.1.0a1689971798/pulumi_kubernetes/core/v1/outputs.py`

 * *Files identical despite different names*

### Comparing `pulumi_kubernetes-4.1.0a1689918291/pulumi_kubernetes/discovery/__init__.py` & `pulumi_kubernetes-4.1.0a1689971798/pulumi_kubernetes/discovery/__init__.py`

 * *Files identical despite different names*

### Comparing `pulumi_kubernetes-4.1.0a1689918291/pulumi_kubernetes/discovery/v1/EndpointSlice.py` & `pulumi_kubernetes-4.1.0a1689971798/pulumi_kubernetes/discovery/v1/EndpointSlice.py`

 * *Files identical despite different names*

### Comparing `pulumi_kubernetes-4.1.0a1689918291/pulumi_kubernetes/discovery/v1/EndpointSliceList.py` & `pulumi_kubernetes-4.1.0a1689971798/pulumi_kubernetes/discovery/v1/EndpointSliceList.py`

 * *Files identical despite different names*

### Comparing `pulumi_kubernetes-4.1.0a1689918291/pulumi_kubernetes/discovery/v1/EndpointSlicePatch.py` & `pulumi_kubernetes-4.1.0a1689971798/pulumi_kubernetes/discovery/v1/EndpointSlicePatch.py`

 * *Files identical despite different names*

### Comparing `pulumi_kubernetes-4.1.0a1689918291/pulumi_kubernetes/discovery/v1/_inputs.py` & `pulumi_kubernetes-4.1.0a1689971798/pulumi_kubernetes/discovery/v1/_inputs.py`

 * *Files identical despite different names*

### Comparing `pulumi_kubernetes-4.1.0a1689918291/pulumi_kubernetes/discovery/v1/outputs.py` & `pulumi_kubernetes-4.1.0a1689971798/pulumi_kubernetes/discovery/v1/outputs.py`

 * *Files identical despite different names*

### Comparing `pulumi_kubernetes-4.1.0a1689918291/pulumi_kubernetes/discovery/v1beta1/EndpointSlice.py` & `pulumi_kubernetes-4.1.0a1689971798/pulumi_kubernetes/discovery/v1beta1/EndpointSlice.py`

 * *Files identical despite different names*

### Comparing `pulumi_kubernetes-4.1.0a1689918291/pulumi_kubernetes/discovery/v1beta1/EndpointSliceList.py` & `pulumi_kubernetes-4.1.0a1689971798/pulumi_kubernetes/discovery/v1beta1/EndpointSliceList.py`

 * *Files identical despite different names*

### Comparing `pulumi_kubernetes-4.1.0a1689918291/pulumi_kubernetes/discovery/v1beta1/EndpointSlicePatch.py` & `pulumi_kubernetes-4.1.0a1689971798/pulumi_kubernetes/discovery/v1beta1/EndpointSlicePatch.py`

 * *Files identical despite different names*

### Comparing `pulumi_kubernetes-4.1.0a1689918291/pulumi_kubernetes/discovery/v1beta1/_inputs.py` & `pulumi_kubernetes-4.1.0a1689971798/pulumi_kubernetes/discovery/v1beta1/_inputs.py`

 * *Files identical despite different names*

### Comparing `pulumi_kubernetes-4.1.0a1689918291/pulumi_kubernetes/discovery/v1beta1/outputs.py` & `pulumi_kubernetes-4.1.0a1689971798/pulumi_kubernetes/discovery/v1beta1/outputs.py`

 * *Files identical despite different names*

### Comparing `pulumi_kubernetes-4.1.0a1689918291/pulumi_kubernetes/events/__init__.py` & `pulumi_kubernetes-4.1.0a1689971798/pulumi_kubernetes/events/__init__.py`

 * *Files identical despite different names*

### Comparing `pulumi_kubernetes-4.1.0a1689918291/pulumi_kubernetes/events/v1/Event.py` & `pulumi_kubernetes-4.1.0a1689971798/pulumi_kubernetes/events/v1/Event.py`

 * *Files identical despite different names*

### Comparing `pulumi_kubernetes-4.1.0a1689918291/pulumi_kubernetes/events/v1/EventList.py` & `pulumi_kubernetes-4.1.0a1689971798/pulumi_kubernetes/events/v1/EventList.py`

 * *Files identical despite different names*

### Comparing `pulumi_kubernetes-4.1.0a1689918291/pulumi_kubernetes/events/v1/EventPatch.py` & `pulumi_kubernetes-4.1.0a1689971798/pulumi_kubernetes/events/v1/EventPatch.py`

 * *Files identical despite different names*

### Comparing `pulumi_kubernetes-4.1.0a1689918291/pulumi_kubernetes/events/v1/_inputs.py` & `pulumi_kubernetes-4.1.0a1689971798/pulumi_kubernetes/events/v1/_inputs.py`

 * *Files identical despite different names*

### Comparing `pulumi_kubernetes-4.1.0a1689918291/pulumi_kubernetes/events/v1/outputs.py` & `pulumi_kubernetes-4.1.0a1689971798/pulumi_kubernetes/events/v1/outputs.py`

 * *Files identical despite different names*

### Comparing `pulumi_kubernetes-4.1.0a1689918291/pulumi_kubernetes/events/v1beta1/Event.py` & `pulumi_kubernetes-4.1.0a1689971798/pulumi_kubernetes/events/v1beta1/Event.py`

 * *Files identical despite different names*

### Comparing `pulumi_kubernetes-4.1.0a1689918291/pulumi_kubernetes/events/v1beta1/EventList.py` & `pulumi_kubernetes-4.1.0a1689971798/pulumi_kubernetes/events/v1beta1/EventList.py`

 * *Files identical despite different names*

### Comparing `pulumi_kubernetes-4.1.0a1689918291/pulumi_kubernetes/events/v1beta1/EventPatch.py` & `pulumi_kubernetes-4.1.0a1689971798/pulumi_kubernetes/events/v1beta1/EventPatch.py`

 * *Files identical despite different names*

### Comparing `pulumi_kubernetes-4.1.0a1689918291/pulumi_kubernetes/events/v1beta1/_inputs.py` & `pulumi_kubernetes-4.1.0a1689971798/pulumi_kubernetes/events/v1beta1/_inputs.py`

 * *Files identical despite different names*

### Comparing `pulumi_kubernetes-4.1.0a1689918291/pulumi_kubernetes/events/v1beta1/outputs.py` & `pulumi_kubernetes-4.1.0a1689971798/pulumi_kubernetes/events/v1beta1/outputs.py`

 * *Files identical despite different names*

### Comparing `pulumi_kubernetes-4.1.0a1689918291/pulumi_kubernetes/extensions/v1beta1/DaemonSet.py` & `pulumi_kubernetes-4.1.0a1689971798/pulumi_kubernetes/extensions/v1beta1/DaemonSet.py`

 * *Files identical despite different names*

### Comparing `pulumi_kubernetes-4.1.0a1689918291/pulumi_kubernetes/extensions/v1beta1/DaemonSetList.py` & `pulumi_kubernetes-4.1.0a1689971798/pulumi_kubernetes/extensions/v1beta1/DaemonSetList.py`

 * *Files identical despite different names*

### Comparing `pulumi_kubernetes-4.1.0a1689918291/pulumi_kubernetes/extensions/v1beta1/DaemonSetPatch.py` & `pulumi_kubernetes-4.1.0a1689971798/pulumi_kubernetes/extensions/v1beta1/DaemonSetPatch.py`

 * *Files identical despite different names*

### Comparing `pulumi_kubernetes-4.1.0a1689918291/pulumi_kubernetes/extensions/v1beta1/Deployment.py` & `pulumi_kubernetes-4.1.0a1689971798/pulumi_kubernetes/extensions/v1beta1/Deployment.py`

 * *Files identical despite different names*

### Comparing `pulumi_kubernetes-4.1.0a1689918291/pulumi_kubernetes/extensions/v1beta1/DeploymentList.py` & `pulumi_kubernetes-4.1.0a1689971798/pulumi_kubernetes/extensions/v1beta1/DeploymentList.py`

 * *Files identical despite different names*

### Comparing `pulumi_kubernetes-4.1.0a1689918291/pulumi_kubernetes/extensions/v1beta1/DeploymentPatch.py` & `pulumi_kubernetes-4.1.0a1689971798/pulumi_kubernetes/extensions/v1beta1/DeploymentPatch.py`

 * *Files identical despite different names*

### Comparing `pulumi_kubernetes-4.1.0a1689918291/pulumi_kubernetes/extensions/v1beta1/Ingress.py` & `pulumi_kubernetes-4.1.0a1689971798/pulumi_kubernetes/extensions/v1beta1/Ingress.py`

 * *Files identical despite different names*

### Comparing `pulumi_kubernetes-4.1.0a1689918291/pulumi_kubernetes/extensions/v1beta1/IngressList.py` & `pulumi_kubernetes-4.1.0a1689971798/pulumi_kubernetes/extensions/v1beta1/IngressList.py`

 * *Files identical despite different names*

### Comparing `pulumi_kubernetes-4.1.0a1689918291/pulumi_kubernetes/extensions/v1beta1/IngressPatch.py` & `pulumi_kubernetes-4.1.0a1689971798/pulumi_kubernetes/extensions/v1beta1/IngressPatch.py`

 * *Files identical despite different names*

### Comparing `pulumi_kubernetes-4.1.0a1689918291/pulumi_kubernetes/extensions/v1beta1/NetworkPolicy.py` & `pulumi_kubernetes-4.1.0a1689971798/pulumi_kubernetes/extensions/v1beta1/NetworkPolicy.py`

 * *Files identical despite different names*

### Comparing `pulumi_kubernetes-4.1.0a1689918291/pulumi_kubernetes/extensions/v1beta1/NetworkPolicyList.py` & `pulumi_kubernetes-4.1.0a1689971798/pulumi_kubernetes/extensions/v1beta1/NetworkPolicyList.py`

 * *Files identical despite different names*

### Comparing `pulumi_kubernetes-4.1.0a1689918291/pulumi_kubernetes/extensions/v1beta1/NetworkPolicyPatch.py` & `pulumi_kubernetes-4.1.0a1689971798/pulumi_kubernetes/extensions/v1beta1/NetworkPolicyPatch.py`

 * *Files identical despite different names*

### Comparing `pulumi_kubernetes-4.1.0a1689918291/pulumi_kubernetes/extensions/v1beta1/PodSecurityPolicy.py` & `pulumi_kubernetes-4.1.0a1689971798/pulumi_kubernetes/extensions/v1beta1/PodSecurityPolicy.py`

 * *Files identical despite different names*

### Comparing `pulumi_kubernetes-4.1.0a1689918291/pulumi_kubernetes/extensions/v1beta1/PodSecurityPolicyList.py` & `pulumi_kubernetes-4.1.0a1689971798/pulumi_kubernetes/extensions/v1beta1/PodSecurityPolicyList.py`

 * *Files identical despite different names*

### Comparing `pulumi_kubernetes-4.1.0a1689918291/pulumi_kubernetes/extensions/v1beta1/PodSecurityPolicyPatch.py` & `pulumi_kubernetes-4.1.0a1689971798/pulumi_kubernetes/extensions/v1beta1/PodSecurityPolicyPatch.py`

 * *Files identical despite different names*

### Comparing `pulumi_kubernetes-4.1.0a1689918291/pulumi_kubernetes/extensions/v1beta1/ReplicaSet.py` & `pulumi_kubernetes-4.1.0a1689971798/pulumi_kubernetes/extensions/v1beta1/ReplicaSet.py`

 * *Files identical despite different names*

### Comparing `pulumi_kubernetes-4.1.0a1689918291/pulumi_kubernetes/extensions/v1beta1/ReplicaSetList.py` & `pulumi_kubernetes-4.1.0a1689971798/pulumi_kubernetes/extensions/v1beta1/ReplicaSetList.py`

 * *Files identical despite different names*

### Comparing `pulumi_kubernetes-4.1.0a1689918291/pulumi_kubernetes/extensions/v1beta1/ReplicaSetPatch.py` & `pulumi_kubernetes-4.1.0a1689971798/pulumi_kubernetes/extensions/v1beta1/ReplicaSetPatch.py`

 * *Files identical despite different names*

### Comparing `pulumi_kubernetes-4.1.0a1689918291/pulumi_kubernetes/extensions/v1beta1/__init__.py` & `pulumi_kubernetes-4.1.0a1689971798/pulumi_kubernetes/extensions/v1beta1/__init__.py`

 * *Files identical despite different names*

### Comparing `pulumi_kubernetes-4.1.0a1689918291/pulumi_kubernetes/extensions/v1beta1/_inputs.py` & `pulumi_kubernetes-4.1.0a1689971798/pulumi_kubernetes/extensions/v1beta1/_inputs.py`

 * *Files identical despite different names*

### Comparing `pulumi_kubernetes-4.1.0a1689918291/pulumi_kubernetes/extensions/v1beta1/outputs.py` & `pulumi_kubernetes-4.1.0a1689971798/pulumi_kubernetes/extensions/v1beta1/outputs.py`

 * *Files identical despite different names*

### Comparing `pulumi_kubernetes-4.1.0a1689918291/pulumi_kubernetes/flowcontrol/__init__.py` & `pulumi_kubernetes-4.1.0a1689971798/pulumi_kubernetes/flowcontrol/__init__.py`

 * *Files identical despite different names*

### Comparing `pulumi_kubernetes-4.1.0a1689918291/pulumi_kubernetes/flowcontrol/v1alpha1/FlowSchema.py` & `pulumi_kubernetes-4.1.0a1689971798/pulumi_kubernetes/flowcontrol/v1alpha1/FlowSchema.py`

 * *Files identical despite different names*

### Comparing `pulumi_kubernetes-4.1.0a1689918291/pulumi_kubernetes/flowcontrol/v1alpha1/FlowSchemaList.py` & `pulumi_kubernetes-4.1.0a1689971798/pulumi_kubernetes/flowcontrol/v1alpha1/FlowSchemaList.py`

 * *Files identical despite different names*

### Comparing `pulumi_kubernetes-4.1.0a1689918291/pulumi_kubernetes/flowcontrol/v1alpha1/FlowSchemaPatch.py` & `pulumi_kubernetes-4.1.0a1689971798/pulumi_kubernetes/flowcontrol/v1alpha1/FlowSchemaPatch.py`

 * *Files identical despite different names*

### Comparing `pulumi_kubernetes-4.1.0a1689918291/pulumi_kubernetes/flowcontrol/v1alpha1/PriorityLevelConfiguration.py` & `pulumi_kubernetes-4.1.0a1689971798/pulumi_kubernetes/flowcontrol/v1alpha1/PriorityLevelConfiguration.py`

 * *Files identical despite different names*

### Comparing `pulumi_kubernetes-4.1.0a1689918291/pulumi_kubernetes/flowcontrol/v1alpha1/PriorityLevelConfigurationList.py` & `pulumi_kubernetes-4.1.0a1689971798/pulumi_kubernetes/flowcontrol/v1alpha1/PriorityLevelConfigurationList.py`

 * *Files identical despite different names*

### Comparing `pulumi_kubernetes-4.1.0a1689918291/pulumi_kubernetes/flowcontrol/v1alpha1/PriorityLevelConfigurationPatch.py` & `pulumi_kubernetes-4.1.0a1689971798/pulumi_kubernetes/flowcontrol/v1alpha1/PriorityLevelConfigurationPatch.py`

 * *Files identical despite different names*

### Comparing `pulumi_kubernetes-4.1.0a1689918291/pulumi_kubernetes/flowcontrol/v1alpha1/_inputs.py` & `pulumi_kubernetes-4.1.0a1689971798/pulumi_kubernetes/flowcontrol/v1alpha1/_inputs.py`

 * *Files identical despite different names*

### Comparing `pulumi_kubernetes-4.1.0a1689918291/pulumi_kubernetes/flowcontrol/v1alpha1/outputs.py` & `pulumi_kubernetes-4.1.0a1689971798/pulumi_kubernetes/flowcontrol/v1alpha1/outputs.py`

 * *Files identical despite different names*

### Comparing `pulumi_kubernetes-4.1.0a1689918291/pulumi_kubernetes/flowcontrol/v1beta1/FlowSchema.py` & `pulumi_kubernetes-4.1.0a1689971798/pulumi_kubernetes/flowcontrol/v1beta1/FlowSchema.py`

 * *Files identical despite different names*

### Comparing `pulumi_kubernetes-4.1.0a1689918291/pulumi_kubernetes/flowcontrol/v1beta1/FlowSchemaList.py` & `pulumi_kubernetes-4.1.0a1689971798/pulumi_kubernetes/flowcontrol/v1beta1/FlowSchemaList.py`

 * *Files identical despite different names*

### Comparing `pulumi_kubernetes-4.1.0a1689918291/pulumi_kubernetes/flowcontrol/v1beta1/FlowSchemaPatch.py` & `pulumi_kubernetes-4.1.0a1689971798/pulumi_kubernetes/flowcontrol/v1beta1/FlowSchemaPatch.py`

 * *Files identical despite different names*

### Comparing `pulumi_kubernetes-4.1.0a1689918291/pulumi_kubernetes/flowcontrol/v1beta1/PriorityLevelConfiguration.py` & `pulumi_kubernetes-4.1.0a1689971798/pulumi_kubernetes/flowcontrol/v1beta1/PriorityLevelConfiguration.py`

 * *Files identical despite different names*

### Comparing `pulumi_kubernetes-4.1.0a1689918291/pulumi_kubernetes/flowcontrol/v1beta1/PriorityLevelConfigurationList.py` & `pulumi_kubernetes-4.1.0a1689971798/pulumi_kubernetes/flowcontrol/v1beta1/PriorityLevelConfigurationList.py`

 * *Files identical despite different names*

### Comparing `pulumi_kubernetes-4.1.0a1689918291/pulumi_kubernetes/flowcontrol/v1beta1/PriorityLevelConfigurationPatch.py` & `pulumi_kubernetes-4.1.0a1689971798/pulumi_kubernetes/flowcontrol/v1beta1/PriorityLevelConfigurationPatch.py`

 * *Files identical despite different names*

### Comparing `pulumi_kubernetes-4.1.0a1689918291/pulumi_kubernetes/flowcontrol/v1beta1/_inputs.py` & `pulumi_kubernetes-4.1.0a1689971798/pulumi_kubernetes/flowcontrol/v1beta1/_inputs.py`

 * *Files identical despite different names*

### Comparing `pulumi_kubernetes-4.1.0a1689918291/pulumi_kubernetes/flowcontrol/v1beta1/outputs.py` & `pulumi_kubernetes-4.1.0a1689971798/pulumi_kubernetes/flowcontrol/v1beta1/outputs.py`

 * *Files identical despite different names*

### Comparing `pulumi_kubernetes-4.1.0a1689918291/pulumi_kubernetes/flowcontrol/v1beta2/FlowSchema.py` & `pulumi_kubernetes-4.1.0a1689971798/pulumi_kubernetes/flowcontrol/v1beta2/FlowSchema.py`

 * *Files identical despite different names*

### Comparing `pulumi_kubernetes-4.1.0a1689918291/pulumi_kubernetes/flowcontrol/v1beta2/FlowSchemaList.py` & `pulumi_kubernetes-4.1.0a1689971798/pulumi_kubernetes/flowcontrol/v1beta2/FlowSchemaList.py`

 * *Files identical despite different names*

### Comparing `pulumi_kubernetes-4.1.0a1689918291/pulumi_kubernetes/flowcontrol/v1beta2/FlowSchemaPatch.py` & `pulumi_kubernetes-4.1.0a1689971798/pulumi_kubernetes/flowcontrol/v1beta2/FlowSchemaPatch.py`

 * *Files identical despite different names*

### Comparing `pulumi_kubernetes-4.1.0a1689918291/pulumi_kubernetes/flowcontrol/v1beta2/PriorityLevelConfiguration.py` & `pulumi_kubernetes-4.1.0a1689971798/pulumi_kubernetes/flowcontrol/v1beta2/PriorityLevelConfiguration.py`

 * *Files identical despite different names*

### Comparing `pulumi_kubernetes-4.1.0a1689918291/pulumi_kubernetes/flowcontrol/v1beta2/PriorityLevelConfigurationList.py` & `pulumi_kubernetes-4.1.0a1689971798/pulumi_kubernetes/flowcontrol/v1beta2/PriorityLevelConfigurationList.py`

 * *Files identical despite different names*

### Comparing `pulumi_kubernetes-4.1.0a1689918291/pulumi_kubernetes/flowcontrol/v1beta2/PriorityLevelConfigurationPatch.py` & `pulumi_kubernetes-4.1.0a1689971798/pulumi_kubernetes/flowcontrol/v1beta2/PriorityLevelConfigurationPatch.py`

 * *Files identical despite different names*

### Comparing `pulumi_kubernetes-4.1.0a1689918291/pulumi_kubernetes/flowcontrol/v1beta2/_inputs.py` & `pulumi_kubernetes-4.1.0a1689971798/pulumi_kubernetes/flowcontrol/v1beta2/_inputs.py`

 * *Files identical despite different names*

### Comparing `pulumi_kubernetes-4.1.0a1689918291/pulumi_kubernetes/flowcontrol/v1beta2/outputs.py` & `pulumi_kubernetes-4.1.0a1689971798/pulumi_kubernetes/flowcontrol/v1beta2/outputs.py`

 * *Files identical despite different names*

### Comparing `pulumi_kubernetes-4.1.0a1689918291/pulumi_kubernetes/flowcontrol/v1beta3/FlowSchema.py` & `pulumi_kubernetes-4.1.0a1689971798/pulumi_kubernetes/flowcontrol/v1beta3/FlowSchema.py`

 * *Files identical despite different names*

### Comparing `pulumi_kubernetes-4.1.0a1689918291/pulumi_kubernetes/flowcontrol/v1beta3/FlowSchemaList.py` & `pulumi_kubernetes-4.1.0a1689971798/pulumi_kubernetes/flowcontrol/v1beta3/FlowSchemaList.py`

 * *Files identical despite different names*

### Comparing `pulumi_kubernetes-4.1.0a1689918291/pulumi_kubernetes/flowcontrol/v1beta3/FlowSchemaPatch.py` & `pulumi_kubernetes-4.1.0a1689971798/pulumi_kubernetes/flowcontrol/v1beta3/FlowSchemaPatch.py`

 * *Files identical despite different names*

### Comparing `pulumi_kubernetes-4.1.0a1689918291/pulumi_kubernetes/flowcontrol/v1beta3/PriorityLevelConfiguration.py` & `pulumi_kubernetes-4.1.0a1689971798/pulumi_kubernetes/flowcontrol/v1beta3/PriorityLevelConfiguration.py`

 * *Files identical despite different names*

### Comparing `pulumi_kubernetes-4.1.0a1689918291/pulumi_kubernetes/flowcontrol/v1beta3/PriorityLevelConfigurationList.py` & `pulumi_kubernetes-4.1.0a1689971798/pulumi_kubernetes/flowcontrol/v1beta3/PriorityLevelConfigurationList.py`

 * *Files identical despite different names*

### Comparing `pulumi_kubernetes-4.1.0a1689918291/pulumi_kubernetes/flowcontrol/v1beta3/PriorityLevelConfigurationPatch.py` & `pulumi_kubernetes-4.1.0a1689971798/pulumi_kubernetes/flowcontrol/v1beta3/PriorityLevelConfigurationPatch.py`

 * *Files identical despite different names*

### Comparing `pulumi_kubernetes-4.1.0a1689918291/pulumi_kubernetes/flowcontrol/v1beta3/_inputs.py` & `pulumi_kubernetes-4.1.0a1689971798/pulumi_kubernetes/flowcontrol/v1beta3/_inputs.py`

 * *Files identical despite different names*

### Comparing `pulumi_kubernetes-4.1.0a1689918291/pulumi_kubernetes/flowcontrol/v1beta3/outputs.py` & `pulumi_kubernetes-4.1.0a1689971798/pulumi_kubernetes/flowcontrol/v1beta3/outputs.py`

 * *Files identical despite different names*

### Comparing `pulumi_kubernetes-4.1.0a1689918291/pulumi_kubernetes/helm/v3/Release.py` & `pulumi_kubernetes-4.1.0a1689971798/pulumi_kubernetes/helm/v3/Release.py`

 * *Files identical despite different names*

### Comparing `pulumi_kubernetes-4.1.0a1689918291/pulumi_kubernetes/helm/v3/_inputs.py` & `pulumi_kubernetes-4.1.0a1689971798/pulumi_kubernetes/helm/v3/_inputs.py`

 * *Files identical despite different names*

### Comparing `pulumi_kubernetes-4.1.0a1689918291/pulumi_kubernetes/helm/v3/helm.py` & `pulumi_kubernetes-4.1.0a1689971798/pulumi_kubernetes/helm/v3/helm.py`

 * *Files identical despite different names*

### Comparing `pulumi_kubernetes-4.1.0a1689918291/pulumi_kubernetes/helm/v3/outputs.py` & `pulumi_kubernetes-4.1.0a1689971798/pulumi_kubernetes/helm/v3/outputs.py`

 * *Files identical despite different names*

### Comparing `pulumi_kubernetes-4.1.0a1689918291/pulumi_kubernetes/kustomize/kustomize.py` & `pulumi_kubernetes-4.1.0a1689971798/pulumi_kubernetes/kustomize/kustomize.py`

 * *Files identical despite different names*

### Comparing `pulumi_kubernetes-4.1.0a1689918291/pulumi_kubernetes/meta/v1/Status.py` & `pulumi_kubernetes-4.1.0a1689971798/pulumi_kubernetes/meta/v1/Status.py`

 * *Files identical despite different names*

### Comparing `pulumi_kubernetes-4.1.0a1689918291/pulumi_kubernetes/meta/v1/StatusPatch.py` & `pulumi_kubernetes-4.1.0a1689971798/pulumi_kubernetes/meta/v1/StatusPatch.py`

 * *Files identical despite different names*

### Comparing `pulumi_kubernetes-4.1.0a1689918291/pulumi_kubernetes/meta/v1/_inputs.py` & `pulumi_kubernetes-4.1.0a1689971798/pulumi_kubernetes/meta/v1/_inputs.py`

 * *Files identical despite different names*

### Comparing `pulumi_kubernetes-4.1.0a1689918291/pulumi_kubernetes/meta/v1/outputs.py` & `pulumi_kubernetes-4.1.0a1689971798/pulumi_kubernetes/meta/v1/outputs.py`

 * *Files identical despite different names*

### Comparing `pulumi_kubernetes-4.1.0a1689918291/pulumi_kubernetes/networking/__init__.py` & `pulumi_kubernetes-4.1.0a1689971798/pulumi_kubernetes/networking/__init__.py`

 * *Files identical despite different names*

### Comparing `pulumi_kubernetes-4.1.0a1689918291/pulumi_kubernetes/networking/v1/Ingress.py` & `pulumi_kubernetes-4.1.0a1689971798/pulumi_kubernetes/networking/v1/Ingress.py`

 * *Files identical despite different names*

### Comparing `pulumi_kubernetes-4.1.0a1689918291/pulumi_kubernetes/networking/v1/IngressClass.py` & `pulumi_kubernetes-4.1.0a1689971798/pulumi_kubernetes/networking/v1/IngressClass.py`

 * *Files identical despite different names*

### Comparing `pulumi_kubernetes-4.1.0a1689918291/pulumi_kubernetes/networking/v1/IngressClassList.py` & `pulumi_kubernetes-4.1.0a1689971798/pulumi_kubernetes/networking/v1/IngressClassList.py`

 * *Files identical despite different names*

### Comparing `pulumi_kubernetes-4.1.0a1689918291/pulumi_kubernetes/networking/v1/IngressClassPatch.py` & `pulumi_kubernetes-4.1.0a1689971798/pulumi_kubernetes/networking/v1/IngressClassPatch.py`

 * *Files identical despite different names*

### Comparing `pulumi_kubernetes-4.1.0a1689918291/pulumi_kubernetes/networking/v1/IngressList.py` & `pulumi_kubernetes-4.1.0a1689971798/pulumi_kubernetes/networking/v1/IngressList.py`

 * *Files identical despite different names*

### Comparing `pulumi_kubernetes-4.1.0a1689918291/pulumi_kubernetes/networking/v1/IngressPatch.py` & `pulumi_kubernetes-4.1.0a1689971798/pulumi_kubernetes/networking/v1/IngressPatch.py`

 * *Files identical despite different names*

### Comparing `pulumi_kubernetes-4.1.0a1689918291/pulumi_kubernetes/networking/v1/NetworkPolicy.py` & `pulumi_kubernetes-4.1.0a1689971798/pulumi_kubernetes/networking/v1/NetworkPolicy.py`

 * *Files identical despite different names*

### Comparing `pulumi_kubernetes-4.1.0a1689918291/pulumi_kubernetes/networking/v1/NetworkPolicyList.py` & `pulumi_kubernetes-4.1.0a1689971798/pulumi_kubernetes/networking/v1/NetworkPolicyList.py`

 * *Files identical despite different names*

### Comparing `pulumi_kubernetes-4.1.0a1689918291/pulumi_kubernetes/networking/v1/NetworkPolicyPatch.py` & `pulumi_kubernetes-4.1.0a1689971798/pulumi_kubernetes/networking/v1/NetworkPolicyPatch.py`

 * *Files identical despite different names*

### Comparing `pulumi_kubernetes-4.1.0a1689918291/pulumi_kubernetes/networking/v1/__init__.py` & `pulumi_kubernetes-4.1.0a1689971798/pulumi_kubernetes/networking/v1/__init__.py`

 * *Files identical despite different names*

### Comparing `pulumi_kubernetes-4.1.0a1689918291/pulumi_kubernetes/networking/v1/_inputs.py` & `pulumi_kubernetes-4.1.0a1689971798/pulumi_kubernetes/networking/v1/_inputs.py`

 * *Files identical despite different names*

### Comparing `pulumi_kubernetes-4.1.0a1689918291/pulumi_kubernetes/networking/v1/outputs.py` & `pulumi_kubernetes-4.1.0a1689971798/pulumi_kubernetes/networking/v1/outputs.py`

 * *Files identical despite different names*

### Comparing `pulumi_kubernetes-4.1.0a1689918291/pulumi_kubernetes/networking/v1alpha1/ClusterCIDR.py` & `pulumi_kubernetes-4.1.0a1689971798/pulumi_kubernetes/networking/v1alpha1/ClusterCIDR.py`

 * *Files identical despite different names*

### Comparing `pulumi_kubernetes-4.1.0a1689918291/pulumi_kubernetes/networking/v1alpha1/ClusterCIDRList.py` & `pulumi_kubernetes-4.1.0a1689971798/pulumi_kubernetes/networking/v1alpha1/ClusterCIDRList.py`

 * *Files identical despite different names*

### Comparing `pulumi_kubernetes-4.1.0a1689918291/pulumi_kubernetes/networking/v1alpha1/ClusterCIDRPatch.py` & `pulumi_kubernetes-4.1.0a1689971798/pulumi_kubernetes/networking/v1alpha1/ClusterCIDRPatch.py`

 * *Files identical despite different names*

### Comparing `pulumi_kubernetes-4.1.0a1689918291/pulumi_kubernetes/networking/v1alpha1/IPAddress.py` & `pulumi_kubernetes-4.1.0a1689971798/pulumi_kubernetes/networking/v1alpha1/IPAddress.py`

 * *Files identical despite different names*

### Comparing `pulumi_kubernetes-4.1.0a1689918291/pulumi_kubernetes/networking/v1alpha1/IPAddressList.py` & `pulumi_kubernetes-4.1.0a1689971798/pulumi_kubernetes/networking/v1alpha1/IPAddressList.py`

 * *Files identical despite different names*

### Comparing `pulumi_kubernetes-4.1.0a1689918291/pulumi_kubernetes/networking/v1alpha1/IPAddressPatch.py` & `pulumi_kubernetes-4.1.0a1689971798/pulumi_kubernetes/networking/v1alpha1/IPAddressPatch.py`

 * *Files identical despite different names*

### Comparing `pulumi_kubernetes-4.1.0a1689918291/pulumi_kubernetes/networking/v1alpha1/_inputs.py` & `pulumi_kubernetes-4.1.0a1689971798/pulumi_kubernetes/networking/v1alpha1/_inputs.py`

 * *Files identical despite different names*

### Comparing `pulumi_kubernetes-4.1.0a1689918291/pulumi_kubernetes/networking/v1alpha1/outputs.py` & `pulumi_kubernetes-4.1.0a1689971798/pulumi_kubernetes/networking/v1alpha1/outputs.py`

 * *Files identical despite different names*

### Comparing `pulumi_kubernetes-4.1.0a1689918291/pulumi_kubernetes/networking/v1beta1/Ingress.py` & `pulumi_kubernetes-4.1.0a1689971798/pulumi_kubernetes/networking/v1beta1/Ingress.py`

 * *Files identical despite different names*

### Comparing `pulumi_kubernetes-4.1.0a1689918291/pulumi_kubernetes/networking/v1beta1/IngressClass.py` & `pulumi_kubernetes-4.1.0a1689971798/pulumi_kubernetes/networking/v1beta1/IngressClass.py`

 * *Files identical despite different names*

### Comparing `pulumi_kubernetes-4.1.0a1689918291/pulumi_kubernetes/networking/v1beta1/IngressClassList.py` & `pulumi_kubernetes-4.1.0a1689971798/pulumi_kubernetes/networking/v1beta1/IngressClassList.py`

 * *Files identical despite different names*

### Comparing `pulumi_kubernetes-4.1.0a1689918291/pulumi_kubernetes/networking/v1beta1/IngressClassPatch.py` & `pulumi_kubernetes-4.1.0a1689971798/pulumi_kubernetes/networking/v1beta1/IngressClassPatch.py`

 * *Files identical despite different names*

### Comparing `pulumi_kubernetes-4.1.0a1689918291/pulumi_kubernetes/networking/v1beta1/IngressList.py` & `pulumi_kubernetes-4.1.0a1689971798/pulumi_kubernetes/networking/v1beta1/IngressList.py`

 * *Files identical despite different names*

### Comparing `pulumi_kubernetes-4.1.0a1689918291/pulumi_kubernetes/networking/v1beta1/IngressPatch.py` & `pulumi_kubernetes-4.1.0a1689971798/pulumi_kubernetes/networking/v1beta1/IngressPatch.py`

 * *Files identical despite different names*

### Comparing `pulumi_kubernetes-4.1.0a1689918291/pulumi_kubernetes/networking/v1beta1/_inputs.py` & `pulumi_kubernetes-4.1.0a1689971798/pulumi_kubernetes/networking/v1beta1/_inputs.py`

 * *Files identical despite different names*

### Comparing `pulumi_kubernetes-4.1.0a1689918291/pulumi_kubernetes/networking/v1beta1/outputs.py` & `pulumi_kubernetes-4.1.0a1689971798/pulumi_kubernetes/networking/v1beta1/outputs.py`

 * *Files identical despite different names*

### Comparing `pulumi_kubernetes-4.1.0a1689918291/pulumi_kubernetes/node/__init__.py` & `pulumi_kubernetes-4.1.0a1689971798/pulumi_kubernetes/node/__init__.py`

 * *Files identical despite different names*

### Comparing `pulumi_kubernetes-4.1.0a1689918291/pulumi_kubernetes/node/v1/RuntimeClass.py` & `pulumi_kubernetes-4.1.0a1689971798/pulumi_kubernetes/node/v1/RuntimeClass.py`

 * *Files identical despite different names*

### Comparing `pulumi_kubernetes-4.1.0a1689918291/pulumi_kubernetes/node/v1/RuntimeClassList.py` & `pulumi_kubernetes-4.1.0a1689971798/pulumi_kubernetes/node/v1/RuntimeClassList.py`

 * *Files identical despite different names*

### Comparing `pulumi_kubernetes-4.1.0a1689918291/pulumi_kubernetes/node/v1/RuntimeClassPatch.py` & `pulumi_kubernetes-4.1.0a1689971798/pulumi_kubernetes/node/v1/RuntimeClassPatch.py`

 * *Files identical despite different names*

### Comparing `pulumi_kubernetes-4.1.0a1689918291/pulumi_kubernetes/node/v1/_inputs.py` & `pulumi_kubernetes-4.1.0a1689971798/pulumi_kubernetes/node/v1/_inputs.py`

 * *Files identical despite different names*

### Comparing `pulumi_kubernetes-4.1.0a1689918291/pulumi_kubernetes/node/v1/outputs.py` & `pulumi_kubernetes-4.1.0a1689971798/pulumi_kubernetes/node/v1/outputs.py`

 * *Files identical despite different names*

### Comparing `pulumi_kubernetes-4.1.0a1689918291/pulumi_kubernetes/node/v1alpha1/RuntimeClass.py` & `pulumi_kubernetes-4.1.0a1689971798/pulumi_kubernetes/node/v1alpha1/RuntimeClass.py`

 * *Files identical despite different names*

### Comparing `pulumi_kubernetes-4.1.0a1689918291/pulumi_kubernetes/node/v1alpha1/RuntimeClassList.py` & `pulumi_kubernetes-4.1.0a1689971798/pulumi_kubernetes/node/v1alpha1/RuntimeClassList.py`

 * *Files identical despite different names*

### Comparing `pulumi_kubernetes-4.1.0a1689918291/pulumi_kubernetes/node/v1alpha1/RuntimeClassPatch.py` & `pulumi_kubernetes-4.1.0a1689971798/pulumi_kubernetes/node/v1alpha1/RuntimeClassPatch.py`

 * *Files identical despite different names*

### Comparing `pulumi_kubernetes-4.1.0a1689918291/pulumi_kubernetes/node/v1alpha1/_inputs.py` & `pulumi_kubernetes-4.1.0a1689971798/pulumi_kubernetes/node/v1alpha1/_inputs.py`

 * *Files identical despite different names*

### Comparing `pulumi_kubernetes-4.1.0a1689918291/pulumi_kubernetes/node/v1alpha1/outputs.py` & `pulumi_kubernetes-4.1.0a1689971798/pulumi_kubernetes/node/v1alpha1/outputs.py`

 * *Files identical despite different names*

### Comparing `pulumi_kubernetes-4.1.0a1689918291/pulumi_kubernetes/node/v1beta1/RuntimeClass.py` & `pulumi_kubernetes-4.1.0a1689971798/pulumi_kubernetes/node/v1beta1/RuntimeClass.py`

 * *Files identical despite different names*

### Comparing `pulumi_kubernetes-4.1.0a1689918291/pulumi_kubernetes/node/v1beta1/RuntimeClassList.py` & `pulumi_kubernetes-4.1.0a1689971798/pulumi_kubernetes/node/v1beta1/RuntimeClassList.py`

 * *Files identical despite different names*

### Comparing `pulumi_kubernetes-4.1.0a1689918291/pulumi_kubernetes/node/v1beta1/RuntimeClassPatch.py` & `pulumi_kubernetes-4.1.0a1689971798/pulumi_kubernetes/node/v1beta1/RuntimeClassPatch.py`

 * *Files identical despite different names*

### Comparing `pulumi_kubernetes-4.1.0a1689918291/pulumi_kubernetes/node/v1beta1/_inputs.py` & `pulumi_kubernetes-4.1.0a1689971798/pulumi_kubernetes/node/v1beta1/_inputs.py`

 * *Files identical despite different names*

### Comparing `pulumi_kubernetes-4.1.0a1689918291/pulumi_kubernetes/node/v1beta1/outputs.py` & `pulumi_kubernetes-4.1.0a1689971798/pulumi_kubernetes/node/v1beta1/outputs.py`

 * *Files identical despite different names*

### Comparing `pulumi_kubernetes-4.1.0a1689918291/pulumi_kubernetes/outputs.py` & `pulumi_kubernetes-4.1.0a1689971798/pulumi_kubernetes/outputs.py`

 * *Files identical despite different names*

### Comparing `pulumi_kubernetes-4.1.0a1689918291/pulumi_kubernetes/policy/__init__.py` & `pulumi_kubernetes-4.1.0a1689971798/pulumi_kubernetes/policy/__init__.py`

 * *Files identical despite different names*

### Comparing `pulumi_kubernetes-4.1.0a1689918291/pulumi_kubernetes/policy/v1/PodDisruptionBudget.py` & `pulumi_kubernetes-4.1.0a1689971798/pulumi_kubernetes/policy/v1/PodDisruptionBudget.py`

 * *Files identical despite different names*

### Comparing `pulumi_kubernetes-4.1.0a1689918291/pulumi_kubernetes/policy/v1/PodDisruptionBudgetList.py` & `pulumi_kubernetes-4.1.0a1689971798/pulumi_kubernetes/policy/v1/PodDisruptionBudgetList.py`

 * *Files identical despite different names*

### Comparing `pulumi_kubernetes-4.1.0a1689918291/pulumi_kubernetes/policy/v1/PodDisruptionBudgetPatch.py` & `pulumi_kubernetes-4.1.0a1689971798/pulumi_kubernetes/policy/v1/PodDisruptionBudgetPatch.py`

 * *Files identical despite different names*

### Comparing `pulumi_kubernetes-4.1.0a1689918291/pulumi_kubernetes/policy/v1/_inputs.py` & `pulumi_kubernetes-4.1.0a1689971798/pulumi_kubernetes/policy/v1/_inputs.py`

 * *Files identical despite different names*

### Comparing `pulumi_kubernetes-4.1.0a1689918291/pulumi_kubernetes/policy/v1/outputs.py` & `pulumi_kubernetes-4.1.0a1689971798/pulumi_kubernetes/policy/v1/outputs.py`

 * *Files identical despite different names*

### Comparing `pulumi_kubernetes-4.1.0a1689918291/pulumi_kubernetes/policy/v1beta1/PodDisruptionBudget.py` & `pulumi_kubernetes-4.1.0a1689971798/pulumi_kubernetes/policy/v1beta1/PodDisruptionBudget.py`

 * *Files identical despite different names*

### Comparing `pulumi_kubernetes-4.1.0a1689918291/pulumi_kubernetes/policy/v1beta1/PodDisruptionBudgetList.py` & `pulumi_kubernetes-4.1.0a1689971798/pulumi_kubernetes/policy/v1beta1/PodDisruptionBudgetList.py`

 * *Files identical despite different names*

### Comparing `pulumi_kubernetes-4.1.0a1689918291/pulumi_kubernetes/policy/v1beta1/PodDisruptionBudgetPatch.py` & `pulumi_kubernetes-4.1.0a1689971798/pulumi_kubernetes/policy/v1beta1/PodDisruptionBudgetPatch.py`

 * *Files identical despite different names*

### Comparing `pulumi_kubernetes-4.1.0a1689918291/pulumi_kubernetes/policy/v1beta1/PodSecurityPolicy.py` & `pulumi_kubernetes-4.1.0a1689971798/pulumi_kubernetes/policy/v1beta1/PodSecurityPolicy.py`

 * *Files identical despite different names*

### Comparing `pulumi_kubernetes-4.1.0a1689918291/pulumi_kubernetes/policy/v1beta1/PodSecurityPolicyList.py` & `pulumi_kubernetes-4.1.0a1689971798/pulumi_kubernetes/policy/v1beta1/PodSecurityPolicyList.py`

 * *Files identical despite different names*

### Comparing `pulumi_kubernetes-4.1.0a1689918291/pulumi_kubernetes/policy/v1beta1/PodSecurityPolicyPatch.py` & `pulumi_kubernetes-4.1.0a1689971798/pulumi_kubernetes/policy/v1beta1/PodSecurityPolicyPatch.py`

 * *Files identical despite different names*

### Comparing `pulumi_kubernetes-4.1.0a1689918291/pulumi_kubernetes/policy/v1beta1/_inputs.py` & `pulumi_kubernetes-4.1.0a1689971798/pulumi_kubernetes/policy/v1beta1/_inputs.py`

 * *Files identical despite different names*

### Comparing `pulumi_kubernetes-4.1.0a1689918291/pulumi_kubernetes/policy/v1beta1/outputs.py` & `pulumi_kubernetes-4.1.0a1689971798/pulumi_kubernetes/policy/v1beta1/outputs.py`

 * *Files identical despite different names*

### Comparing `pulumi_kubernetes-4.1.0a1689918291/pulumi_kubernetes/provider.py` & `pulumi_kubernetes-4.1.0a1689971798/pulumi_kubernetes/provider.py`

 * *Files identical despite different names*

### Comparing `pulumi_kubernetes-4.1.0a1689918291/pulumi_kubernetes/rbac/__init__.py` & `pulumi_kubernetes-4.1.0a1689971798/pulumi_kubernetes/rbac/__init__.py`

 * *Files identical despite different names*

### Comparing `pulumi_kubernetes-4.1.0a1689918291/pulumi_kubernetes/rbac/v1/ClusterRole.py` & `pulumi_kubernetes-4.1.0a1689971798/pulumi_kubernetes/rbac/v1/ClusterRole.py`

 * *Files identical despite different names*

### Comparing `pulumi_kubernetes-4.1.0a1689918291/pulumi_kubernetes/rbac/v1/ClusterRoleBinding.py` & `pulumi_kubernetes-4.1.0a1689971798/pulumi_kubernetes/rbac/v1/ClusterRoleBinding.py`

 * *Files identical despite different names*

### Comparing `pulumi_kubernetes-4.1.0a1689918291/pulumi_kubernetes/rbac/v1/ClusterRoleBindingList.py` & `pulumi_kubernetes-4.1.0a1689971798/pulumi_kubernetes/rbac/v1/ClusterRoleBindingList.py`

 * *Files identical despite different names*

### Comparing `pulumi_kubernetes-4.1.0a1689918291/pulumi_kubernetes/rbac/v1/ClusterRoleBindingPatch.py` & `pulumi_kubernetes-4.1.0a1689971798/pulumi_kubernetes/rbac/v1/ClusterRoleBindingPatch.py`

 * *Files identical despite different names*

### Comparing `pulumi_kubernetes-4.1.0a1689918291/pulumi_kubernetes/rbac/v1/ClusterRoleList.py` & `pulumi_kubernetes-4.1.0a1689971798/pulumi_kubernetes/rbac/v1/ClusterRoleList.py`

 * *Files identical despite different names*

### Comparing `pulumi_kubernetes-4.1.0a1689918291/pulumi_kubernetes/rbac/v1/ClusterRolePatch.py` & `pulumi_kubernetes-4.1.0a1689971798/pulumi_kubernetes/rbac/v1/ClusterRolePatch.py`

 * *Files identical despite different names*

### Comparing `pulumi_kubernetes-4.1.0a1689918291/pulumi_kubernetes/rbac/v1/Role.py` & `pulumi_kubernetes-4.1.0a1689971798/pulumi_kubernetes/rbac/v1/Role.py`

 * *Files identical despite different names*

### Comparing `pulumi_kubernetes-4.1.0a1689918291/pulumi_kubernetes/rbac/v1/RoleBinding.py` & `pulumi_kubernetes-4.1.0a1689971798/pulumi_kubernetes/rbac/v1/RoleBinding.py`

 * *Files identical despite different names*

### Comparing `pulumi_kubernetes-4.1.0a1689918291/pulumi_kubernetes/rbac/v1/RoleBindingList.py` & `pulumi_kubernetes-4.1.0a1689971798/pulumi_kubernetes/rbac/v1/RoleBindingList.py`

 * *Files identical despite different names*

### Comparing `pulumi_kubernetes-4.1.0a1689918291/pulumi_kubernetes/rbac/v1/RoleBindingPatch.py` & `pulumi_kubernetes-4.1.0a1689971798/pulumi_kubernetes/rbac/v1/RoleBindingPatch.py`

 * *Files identical despite different names*

### Comparing `pulumi_kubernetes-4.1.0a1689918291/pulumi_kubernetes/rbac/v1/RoleList.py` & `pulumi_kubernetes-4.1.0a1689971798/pulumi_kubernetes/rbac/v1/RoleList.py`

 * *Files identical despite different names*

### Comparing `pulumi_kubernetes-4.1.0a1689918291/pulumi_kubernetes/rbac/v1/RolePatch.py` & `pulumi_kubernetes-4.1.0a1689971798/pulumi_kubernetes/rbac/v1/RolePatch.py`

 * *Files identical despite different names*

### Comparing `pulumi_kubernetes-4.1.0a1689918291/pulumi_kubernetes/rbac/v1/__init__.py` & `pulumi_kubernetes-4.1.0a1689971798/pulumi_kubernetes/rbac/v1/__init__.py`

 * *Files identical despite different names*

### Comparing `pulumi_kubernetes-4.1.0a1689918291/pulumi_kubernetes/rbac/v1/_inputs.py` & `pulumi_kubernetes-4.1.0a1689971798/pulumi_kubernetes/rbac/v1/_inputs.py`

 * *Files identical despite different names*

### Comparing `pulumi_kubernetes-4.1.0a1689918291/pulumi_kubernetes/rbac/v1/outputs.py` & `pulumi_kubernetes-4.1.0a1689971798/pulumi_kubernetes/rbac/v1/outputs.py`

 * *Files identical despite different names*

### Comparing `pulumi_kubernetes-4.1.0a1689918291/pulumi_kubernetes/rbac/v1alpha1/ClusterRole.py` & `pulumi_kubernetes-4.1.0a1689971798/pulumi_kubernetes/rbac/v1alpha1/ClusterRole.py`

 * *Files identical despite different names*

### Comparing `pulumi_kubernetes-4.1.0a1689918291/pulumi_kubernetes/rbac/v1alpha1/ClusterRoleBinding.py` & `pulumi_kubernetes-4.1.0a1689971798/pulumi_kubernetes/rbac/v1alpha1/ClusterRoleBinding.py`

 * *Files identical despite different names*

### Comparing `pulumi_kubernetes-4.1.0a1689918291/pulumi_kubernetes/rbac/v1alpha1/ClusterRoleBindingList.py` & `pulumi_kubernetes-4.1.0a1689971798/pulumi_kubernetes/rbac/v1alpha1/ClusterRoleBindingList.py`

 * *Files identical despite different names*

### Comparing `pulumi_kubernetes-4.1.0a1689918291/pulumi_kubernetes/rbac/v1alpha1/ClusterRoleBindingPatch.py` & `pulumi_kubernetes-4.1.0a1689971798/pulumi_kubernetes/rbac/v1alpha1/ClusterRoleBindingPatch.py`

 * *Files identical despite different names*

### Comparing `pulumi_kubernetes-4.1.0a1689918291/pulumi_kubernetes/rbac/v1alpha1/ClusterRoleList.py` & `pulumi_kubernetes-4.1.0a1689971798/pulumi_kubernetes/rbac/v1alpha1/ClusterRoleList.py`

 * *Files identical despite different names*

### Comparing `pulumi_kubernetes-4.1.0a1689918291/pulumi_kubernetes/rbac/v1alpha1/ClusterRolePatch.py` & `pulumi_kubernetes-4.1.0a1689971798/pulumi_kubernetes/rbac/v1alpha1/ClusterRolePatch.py`

 * *Files identical despite different names*

### Comparing `pulumi_kubernetes-4.1.0a1689918291/pulumi_kubernetes/rbac/v1alpha1/Role.py` & `pulumi_kubernetes-4.1.0a1689971798/pulumi_kubernetes/rbac/v1alpha1/Role.py`

 * *Files identical despite different names*

### Comparing `pulumi_kubernetes-4.1.0a1689918291/pulumi_kubernetes/rbac/v1alpha1/RoleBinding.py` & `pulumi_kubernetes-4.1.0a1689971798/pulumi_kubernetes/rbac/v1alpha1/RoleBinding.py`

 * *Files identical despite different names*

### Comparing `pulumi_kubernetes-4.1.0a1689918291/pulumi_kubernetes/rbac/v1alpha1/RoleBindingList.py` & `pulumi_kubernetes-4.1.0a1689971798/pulumi_kubernetes/rbac/v1alpha1/RoleBindingList.py`

 * *Files identical despite different names*

### Comparing `pulumi_kubernetes-4.1.0a1689918291/pulumi_kubernetes/rbac/v1alpha1/RoleBindingPatch.py` & `pulumi_kubernetes-4.1.0a1689971798/pulumi_kubernetes/rbac/v1alpha1/RoleBindingPatch.py`

 * *Files identical despite different names*

### Comparing `pulumi_kubernetes-4.1.0a1689918291/pulumi_kubernetes/rbac/v1alpha1/RoleList.py` & `pulumi_kubernetes-4.1.0a1689971798/pulumi_kubernetes/rbac/v1alpha1/RoleList.py`

 * *Files identical despite different names*

### Comparing `pulumi_kubernetes-4.1.0a1689918291/pulumi_kubernetes/rbac/v1alpha1/RolePatch.py` & `pulumi_kubernetes-4.1.0a1689971798/pulumi_kubernetes/rbac/v1alpha1/RolePatch.py`

 * *Files identical despite different names*

### Comparing `pulumi_kubernetes-4.1.0a1689918291/pulumi_kubernetes/rbac/v1alpha1/__init__.py` & `pulumi_kubernetes-4.1.0a1689971798/pulumi_kubernetes/rbac/v1alpha1/__init__.py`

 * *Files identical despite different names*

### Comparing `pulumi_kubernetes-4.1.0a1689918291/pulumi_kubernetes/rbac/v1alpha1/_inputs.py` & `pulumi_kubernetes-4.1.0a1689971798/pulumi_kubernetes/rbac/v1alpha1/_inputs.py`

 * *Files identical despite different names*

### Comparing `pulumi_kubernetes-4.1.0a1689918291/pulumi_kubernetes/rbac/v1alpha1/outputs.py` & `pulumi_kubernetes-4.1.0a1689971798/pulumi_kubernetes/rbac/v1alpha1/outputs.py`

 * *Files identical despite different names*

### Comparing `pulumi_kubernetes-4.1.0a1689918291/pulumi_kubernetes/rbac/v1beta1/ClusterRole.py` & `pulumi_kubernetes-4.1.0a1689971798/pulumi_kubernetes/rbac/v1beta1/ClusterRole.py`

 * *Files identical despite different names*

### Comparing `pulumi_kubernetes-4.1.0a1689918291/pulumi_kubernetes/rbac/v1beta1/ClusterRoleBinding.py` & `pulumi_kubernetes-4.1.0a1689971798/pulumi_kubernetes/rbac/v1beta1/ClusterRoleBinding.py`

 * *Files identical despite different names*

### Comparing `pulumi_kubernetes-4.1.0a1689918291/pulumi_kubernetes/rbac/v1beta1/ClusterRoleBindingList.py` & `pulumi_kubernetes-4.1.0a1689971798/pulumi_kubernetes/rbac/v1beta1/ClusterRoleBindingList.py`

 * *Files identical despite different names*

### Comparing `pulumi_kubernetes-4.1.0a1689918291/pulumi_kubernetes/rbac/v1beta1/ClusterRoleBindingPatch.py` & `pulumi_kubernetes-4.1.0a1689971798/pulumi_kubernetes/rbac/v1beta1/ClusterRoleBindingPatch.py`

 * *Files identical despite different names*

### Comparing `pulumi_kubernetes-4.1.0a1689918291/pulumi_kubernetes/rbac/v1beta1/ClusterRoleList.py` & `pulumi_kubernetes-4.1.0a1689971798/pulumi_kubernetes/rbac/v1beta1/ClusterRoleList.py`

 * *Files identical despite different names*

### Comparing `pulumi_kubernetes-4.1.0a1689918291/pulumi_kubernetes/rbac/v1beta1/ClusterRolePatch.py` & `pulumi_kubernetes-4.1.0a1689971798/pulumi_kubernetes/rbac/v1beta1/ClusterRolePatch.py`

 * *Files identical despite different names*

### Comparing `pulumi_kubernetes-4.1.0a1689918291/pulumi_kubernetes/rbac/v1beta1/Role.py` & `pulumi_kubernetes-4.1.0a1689971798/pulumi_kubernetes/rbac/v1beta1/Role.py`

 * *Files identical despite different names*

### Comparing `pulumi_kubernetes-4.1.0a1689918291/pulumi_kubernetes/rbac/v1beta1/RoleBinding.py` & `pulumi_kubernetes-4.1.0a1689971798/pulumi_kubernetes/rbac/v1beta1/RoleBinding.py`

 * *Files identical despite different names*

### Comparing `pulumi_kubernetes-4.1.0a1689918291/pulumi_kubernetes/rbac/v1beta1/RoleBindingList.py` & `pulumi_kubernetes-4.1.0a1689971798/pulumi_kubernetes/rbac/v1beta1/RoleBindingList.py`

 * *Files identical despite different names*

### Comparing `pulumi_kubernetes-4.1.0a1689918291/pulumi_kubernetes/rbac/v1beta1/RoleBindingPatch.py` & `pulumi_kubernetes-4.1.0a1689971798/pulumi_kubernetes/rbac/v1beta1/RoleBindingPatch.py`

 * *Files identical despite different names*

### Comparing `pulumi_kubernetes-4.1.0a1689918291/pulumi_kubernetes/rbac/v1beta1/RoleList.py` & `pulumi_kubernetes-4.1.0a1689971798/pulumi_kubernetes/rbac/v1beta1/RoleList.py`

 * *Files identical despite different names*

### Comparing `pulumi_kubernetes-4.1.0a1689918291/pulumi_kubernetes/rbac/v1beta1/RolePatch.py` & `pulumi_kubernetes-4.1.0a1689971798/pulumi_kubernetes/rbac/v1beta1/RolePatch.py`

 * *Files identical despite different names*

### Comparing `pulumi_kubernetes-4.1.0a1689918291/pulumi_kubernetes/rbac/v1beta1/__init__.py` & `pulumi_kubernetes-4.1.0a1689971798/pulumi_kubernetes/rbac/v1beta1/__init__.py`

 * *Files identical despite different names*

### Comparing `pulumi_kubernetes-4.1.0a1689918291/pulumi_kubernetes/rbac/v1beta1/_inputs.py` & `pulumi_kubernetes-4.1.0a1689971798/pulumi_kubernetes/rbac/v1beta1/_inputs.py`

 * *Files identical despite different names*

### Comparing `pulumi_kubernetes-4.1.0a1689918291/pulumi_kubernetes/rbac/v1beta1/outputs.py` & `pulumi_kubernetes-4.1.0a1689971798/pulumi_kubernetes/rbac/v1beta1/outputs.py`

 * *Files identical despite different names*

### Comparing `pulumi_kubernetes-4.1.0a1689918291/pulumi_kubernetes/resource/__init__.py` & `pulumi_kubernetes-4.1.0a1689971798/pulumi_kubernetes/resource/__init__.py`

 * *Files identical despite different names*

### Comparing `pulumi_kubernetes-4.1.0a1689918291/pulumi_kubernetes/resource/v1alpha1/PodScheduling.py` & `pulumi_kubernetes-4.1.0a1689971798/pulumi_kubernetes/resource/v1alpha1/PodScheduling.py`

 * *Files identical despite different names*

### Comparing `pulumi_kubernetes-4.1.0a1689918291/pulumi_kubernetes/resource/v1alpha1/PodSchedulingList.py` & `pulumi_kubernetes-4.1.0a1689971798/pulumi_kubernetes/resource/v1alpha1/PodSchedulingList.py`

 * *Files identical despite different names*

### Comparing `pulumi_kubernetes-4.1.0a1689918291/pulumi_kubernetes/resource/v1alpha1/PodSchedulingPatch.py` & `pulumi_kubernetes-4.1.0a1689971798/pulumi_kubernetes/resource/v1alpha1/PodSchedulingPatch.py`

 * *Files identical despite different names*

### Comparing `pulumi_kubernetes-4.1.0a1689918291/pulumi_kubernetes/resource/v1alpha1/ResourceClaim.py` & `pulumi_kubernetes-4.1.0a1689971798/pulumi_kubernetes/resource/v1alpha1/ResourceClaim.py`

 * *Files identical despite different names*

### Comparing `pulumi_kubernetes-4.1.0a1689918291/pulumi_kubernetes/resource/v1alpha1/ResourceClaimList.py` & `pulumi_kubernetes-4.1.0a1689971798/pulumi_kubernetes/resource/v1alpha1/ResourceClaimList.py`

 * *Files identical despite different names*

### Comparing `pulumi_kubernetes-4.1.0a1689918291/pulumi_kubernetes/resource/v1alpha1/ResourceClaimPatch.py` & `pulumi_kubernetes-4.1.0a1689971798/pulumi_kubernetes/resource/v1alpha1/ResourceClaimPatch.py`

 * *Files identical despite different names*

### Comparing `pulumi_kubernetes-4.1.0a1689918291/pulumi_kubernetes/resource/v1alpha1/ResourceClaimTemplate.py` & `pulumi_kubernetes-4.1.0a1689971798/pulumi_kubernetes/resource/v1alpha1/ResourceClaimTemplate.py`

 * *Files identical despite different names*

### Comparing `pulumi_kubernetes-4.1.0a1689918291/pulumi_kubernetes/resource/v1alpha1/ResourceClaimTemplateList.py` & `pulumi_kubernetes-4.1.0a1689971798/pulumi_kubernetes/resource/v1alpha1/ResourceClaimTemplateList.py`

 * *Files identical despite different names*

### Comparing `pulumi_kubernetes-4.1.0a1689918291/pulumi_kubernetes/resource/v1alpha1/ResourceClaimTemplatePatch.py` & `pulumi_kubernetes-4.1.0a1689971798/pulumi_kubernetes/resource/v1alpha1/ResourceClaimTemplatePatch.py`

 * *Files identical despite different names*

### Comparing `pulumi_kubernetes-4.1.0a1689918291/pulumi_kubernetes/resource/v1alpha1/ResourceClass.py` & `pulumi_kubernetes-4.1.0a1689971798/pulumi_kubernetes/resource/v1alpha1/ResourceClass.py`

 * *Files identical despite different names*

### Comparing `pulumi_kubernetes-4.1.0a1689918291/pulumi_kubernetes/resource/v1alpha1/ResourceClassList.py` & `pulumi_kubernetes-4.1.0a1689971798/pulumi_kubernetes/resource/v1alpha1/ResourceClassList.py`

 * *Files identical despite different names*

### Comparing `pulumi_kubernetes-4.1.0a1689918291/pulumi_kubernetes/resource/v1alpha1/ResourceClassPatch.py` & `pulumi_kubernetes-4.1.0a1689971798/pulumi_kubernetes/resource/v1alpha1/ResourceClassPatch.py`

 * *Files identical despite different names*

### Comparing `pulumi_kubernetes-4.1.0a1689918291/pulumi_kubernetes/resource/v1alpha1/__init__.py` & `pulumi_kubernetes-4.1.0a1689971798/pulumi_kubernetes/resource/v1alpha1/__init__.py`

 * *Files identical despite different names*

### Comparing `pulumi_kubernetes-4.1.0a1689918291/pulumi_kubernetes/resource/v1alpha1/_inputs.py` & `pulumi_kubernetes-4.1.0a1689971798/pulumi_kubernetes/resource/v1alpha1/_inputs.py`

 * *Files identical despite different names*

### Comparing `pulumi_kubernetes-4.1.0a1689918291/pulumi_kubernetes/resource/v1alpha1/outputs.py` & `pulumi_kubernetes-4.1.0a1689971798/pulumi_kubernetes/resource/v1alpha1/outputs.py`

 * *Files identical despite different names*

### Comparing `pulumi_kubernetes-4.1.0a1689918291/pulumi_kubernetes/resource/v1alpha2/PodSchedulingContext.py` & `pulumi_kubernetes-4.1.0a1689971798/pulumi_kubernetes/resource/v1alpha2/PodSchedulingContext.py`

 * *Files identical despite different names*

### Comparing `pulumi_kubernetes-4.1.0a1689918291/pulumi_kubernetes/resource/v1alpha2/PodSchedulingContextList.py` & `pulumi_kubernetes-4.1.0a1689971798/pulumi_kubernetes/resource/v1alpha2/PodSchedulingContextList.py`

 * *Files identical despite different names*

### Comparing `pulumi_kubernetes-4.1.0a1689918291/pulumi_kubernetes/resource/v1alpha2/PodSchedulingContextPatch.py` & `pulumi_kubernetes-4.1.0a1689971798/pulumi_kubernetes/resource/v1alpha2/PodSchedulingContextPatch.py`

 * *Files identical despite different names*

### Comparing `pulumi_kubernetes-4.1.0a1689918291/pulumi_kubernetes/resource/v1alpha2/ResourceClaim.py` & `pulumi_kubernetes-4.1.0a1689971798/pulumi_kubernetes/resource/v1alpha2/ResourceClaim.py`

 * *Files identical despite different names*

### Comparing `pulumi_kubernetes-4.1.0a1689918291/pulumi_kubernetes/resource/v1alpha2/ResourceClaimList.py` & `pulumi_kubernetes-4.1.0a1689971798/pulumi_kubernetes/resource/v1alpha2/ResourceClaimList.py`

 * *Files identical despite different names*

### Comparing `pulumi_kubernetes-4.1.0a1689918291/pulumi_kubernetes/resource/v1alpha2/ResourceClaimPatch.py` & `pulumi_kubernetes-4.1.0a1689971798/pulumi_kubernetes/resource/v1alpha2/ResourceClaimPatch.py`

 * *Files identical despite different names*

### Comparing `pulumi_kubernetes-4.1.0a1689918291/pulumi_kubernetes/resource/v1alpha2/ResourceClaimTemplate.py` & `pulumi_kubernetes-4.1.0a1689971798/pulumi_kubernetes/resource/v1alpha2/ResourceClaimTemplate.py`

 * *Files identical despite different names*

### Comparing `pulumi_kubernetes-4.1.0a1689918291/pulumi_kubernetes/resource/v1alpha2/ResourceClaimTemplateList.py` & `pulumi_kubernetes-4.1.0a1689971798/pulumi_kubernetes/resource/v1alpha2/ResourceClaimTemplateList.py`

 * *Files identical despite different names*

### Comparing `pulumi_kubernetes-4.1.0a1689918291/pulumi_kubernetes/resource/v1alpha2/ResourceClaimTemplatePatch.py` & `pulumi_kubernetes-4.1.0a1689971798/pulumi_kubernetes/resource/v1alpha2/ResourceClaimTemplatePatch.py`

 * *Files identical despite different names*

### Comparing `pulumi_kubernetes-4.1.0a1689918291/pulumi_kubernetes/resource/v1alpha2/ResourceClass.py` & `pulumi_kubernetes-4.1.0a1689971798/pulumi_kubernetes/resource/v1alpha2/ResourceClass.py`

 * *Files identical despite different names*

### Comparing `pulumi_kubernetes-4.1.0a1689918291/pulumi_kubernetes/resource/v1alpha2/ResourceClassList.py` & `pulumi_kubernetes-4.1.0a1689971798/pulumi_kubernetes/resource/v1alpha2/ResourceClassList.py`

 * *Files identical despite different names*

### Comparing `pulumi_kubernetes-4.1.0a1689918291/pulumi_kubernetes/resource/v1alpha2/ResourceClassPatch.py` & `pulumi_kubernetes-4.1.0a1689971798/pulumi_kubernetes/resource/v1alpha2/ResourceClassPatch.py`

 * *Files identical despite different names*

### Comparing `pulumi_kubernetes-4.1.0a1689918291/pulumi_kubernetes/resource/v1alpha2/__init__.py` & `pulumi_kubernetes-4.1.0a1689971798/pulumi_kubernetes/resource/v1alpha2/__init__.py`

 * *Files identical despite different names*

### Comparing `pulumi_kubernetes-4.1.0a1689918291/pulumi_kubernetes/resource/v1alpha2/_inputs.py` & `pulumi_kubernetes-4.1.0a1689971798/pulumi_kubernetes/resource/v1alpha2/_inputs.py`

 * *Files identical despite different names*

### Comparing `pulumi_kubernetes-4.1.0a1689918291/pulumi_kubernetes/resource/v1alpha2/outputs.py` & `pulumi_kubernetes-4.1.0a1689971798/pulumi_kubernetes/resource/v1alpha2/outputs.py`

 * *Files identical despite different names*

### Comparing `pulumi_kubernetes-4.1.0a1689918291/pulumi_kubernetes/scheduling/__init__.py` & `pulumi_kubernetes-4.1.0a1689971798/pulumi_kubernetes/scheduling/__init__.py`

 * *Files identical despite different names*

### Comparing `pulumi_kubernetes-4.1.0a1689918291/pulumi_kubernetes/scheduling/v1/PriorityClass.py` & `pulumi_kubernetes-4.1.0a1689971798/pulumi_kubernetes/scheduling/v1/PriorityClass.py`

 * *Files identical despite different names*

### Comparing `pulumi_kubernetes-4.1.0a1689918291/pulumi_kubernetes/scheduling/v1/PriorityClassList.py` & `pulumi_kubernetes-4.1.0a1689971798/pulumi_kubernetes/scheduling/v1/PriorityClassList.py`

 * *Files identical despite different names*

### Comparing `pulumi_kubernetes-4.1.0a1689918291/pulumi_kubernetes/scheduling/v1/PriorityClassPatch.py` & `pulumi_kubernetes-4.1.0a1689971798/pulumi_kubernetes/scheduling/v1/PriorityClassPatch.py`

 * *Files identical despite different names*

### Comparing `pulumi_kubernetes-4.1.0a1689918291/pulumi_kubernetes/scheduling/v1/_inputs.py` & `pulumi_kubernetes-4.1.0a1689971798/pulumi_kubernetes/scheduling/v1/_inputs.py`

 * *Files identical despite different names*

### Comparing `pulumi_kubernetes-4.1.0a1689918291/pulumi_kubernetes/scheduling/v1/outputs.py` & `pulumi_kubernetes-4.1.0a1689971798/pulumi_kubernetes/scheduling/v1/outputs.py`

 * *Files identical despite different names*

### Comparing `pulumi_kubernetes-4.1.0a1689918291/pulumi_kubernetes/scheduling/v1alpha1/PriorityClass.py` & `pulumi_kubernetes-4.1.0a1689971798/pulumi_kubernetes/scheduling/v1alpha1/PriorityClass.py`

 * *Files identical despite different names*

### Comparing `pulumi_kubernetes-4.1.0a1689918291/pulumi_kubernetes/scheduling/v1alpha1/PriorityClassList.py` & `pulumi_kubernetes-4.1.0a1689971798/pulumi_kubernetes/scheduling/v1alpha1/PriorityClassList.py`

 * *Files identical despite different names*

### Comparing `pulumi_kubernetes-4.1.0a1689918291/pulumi_kubernetes/scheduling/v1alpha1/PriorityClassPatch.py` & `pulumi_kubernetes-4.1.0a1689971798/pulumi_kubernetes/scheduling/v1alpha1/PriorityClassPatch.py`

 * *Files identical despite different names*

### Comparing `pulumi_kubernetes-4.1.0a1689918291/pulumi_kubernetes/scheduling/v1alpha1/_inputs.py` & `pulumi_kubernetes-4.1.0a1689971798/pulumi_kubernetes/scheduling/v1alpha1/_inputs.py`

 * *Files identical despite different names*

### Comparing `pulumi_kubernetes-4.1.0a1689918291/pulumi_kubernetes/scheduling/v1alpha1/outputs.py` & `pulumi_kubernetes-4.1.0a1689971798/pulumi_kubernetes/scheduling/v1alpha1/outputs.py`

 * *Files identical despite different names*

### Comparing `pulumi_kubernetes-4.1.0a1689918291/pulumi_kubernetes/scheduling/v1beta1/PriorityClass.py` & `pulumi_kubernetes-4.1.0a1689971798/pulumi_kubernetes/scheduling/v1beta1/PriorityClass.py`

 * *Files identical despite different names*

### Comparing `pulumi_kubernetes-4.1.0a1689918291/pulumi_kubernetes/scheduling/v1beta1/PriorityClassList.py` & `pulumi_kubernetes-4.1.0a1689971798/pulumi_kubernetes/scheduling/v1beta1/PriorityClassList.py`

 * *Files identical despite different names*

### Comparing `pulumi_kubernetes-4.1.0a1689918291/pulumi_kubernetes/scheduling/v1beta1/PriorityClassPatch.py` & `pulumi_kubernetes-4.1.0a1689971798/pulumi_kubernetes/scheduling/v1beta1/PriorityClassPatch.py`

 * *Files identical despite different names*

### Comparing `pulumi_kubernetes-4.1.0a1689918291/pulumi_kubernetes/scheduling/v1beta1/_inputs.py` & `pulumi_kubernetes-4.1.0a1689971798/pulumi_kubernetes/scheduling/v1beta1/_inputs.py`

 * *Files identical despite different names*

### Comparing `pulumi_kubernetes-4.1.0a1689918291/pulumi_kubernetes/scheduling/v1beta1/outputs.py` & `pulumi_kubernetes-4.1.0a1689971798/pulumi_kubernetes/scheduling/v1beta1/outputs.py`

 * *Files identical despite different names*

### Comparing `pulumi_kubernetes-4.1.0a1689918291/pulumi_kubernetes/settings/v1alpha1/PodPreset.py` & `pulumi_kubernetes-4.1.0a1689971798/pulumi_kubernetes/settings/v1alpha1/PodPreset.py`

 * *Files identical despite different names*

### Comparing `pulumi_kubernetes-4.1.0a1689918291/pulumi_kubernetes/settings/v1alpha1/PodPresetList.py` & `pulumi_kubernetes-4.1.0a1689971798/pulumi_kubernetes/settings/v1alpha1/PodPresetList.py`

 * *Files identical despite different names*

### Comparing `pulumi_kubernetes-4.1.0a1689918291/pulumi_kubernetes/settings/v1alpha1/PodPresetPatch.py` & `pulumi_kubernetes-4.1.0a1689971798/pulumi_kubernetes/settings/v1alpha1/PodPresetPatch.py`

 * *Files identical despite different names*

### Comparing `pulumi_kubernetes-4.1.0a1689918291/pulumi_kubernetes/settings/v1alpha1/_inputs.py` & `pulumi_kubernetes-4.1.0a1689971798/pulumi_kubernetes/settings/v1alpha1/_inputs.py`

 * *Files identical despite different names*

### Comparing `pulumi_kubernetes-4.1.0a1689918291/pulumi_kubernetes/settings/v1alpha1/outputs.py` & `pulumi_kubernetes-4.1.0a1689971798/pulumi_kubernetes/settings/v1alpha1/outputs.py`

 * *Files identical despite different names*

### Comparing `pulumi_kubernetes-4.1.0a1689918291/pulumi_kubernetes/storage/__init__.py` & `pulumi_kubernetes-4.1.0a1689971798/pulumi_kubernetes/storage/__init__.py`

 * *Files identical despite different names*

### Comparing `pulumi_kubernetes-4.1.0a1689918291/pulumi_kubernetes/storage/v1/CSIDriver.py` & `pulumi_kubernetes-4.1.0a1689971798/pulumi_kubernetes/storage/v1/CSIDriver.py`

 * *Files identical despite different names*

### Comparing `pulumi_kubernetes-4.1.0a1689918291/pulumi_kubernetes/storage/v1/CSIDriverList.py` & `pulumi_kubernetes-4.1.0a1689971798/pulumi_kubernetes/storage/v1/CSIDriverList.py`

 * *Files identical despite different names*

### Comparing `pulumi_kubernetes-4.1.0a1689918291/pulumi_kubernetes/storage/v1/CSIDriverPatch.py` & `pulumi_kubernetes-4.1.0a1689971798/pulumi_kubernetes/storage/v1/CSIDriverPatch.py`

 * *Files identical despite different names*

### Comparing `pulumi_kubernetes-4.1.0a1689918291/pulumi_kubernetes/storage/v1/CSINode.py` & `pulumi_kubernetes-4.1.0a1689971798/pulumi_kubernetes/storage/v1/CSINode.py`

 * *Files identical despite different names*

### Comparing `pulumi_kubernetes-4.1.0a1689918291/pulumi_kubernetes/storage/v1/CSINodeList.py` & `pulumi_kubernetes-4.1.0a1689971798/pulumi_kubernetes/storage/v1/CSINodeList.py`

 * *Files identical despite different names*

### Comparing `pulumi_kubernetes-4.1.0a1689918291/pulumi_kubernetes/storage/v1/CSINodePatch.py` & `pulumi_kubernetes-4.1.0a1689971798/pulumi_kubernetes/storage/v1/CSINodePatch.py`

 * *Files identical despite different names*

### Comparing `pulumi_kubernetes-4.1.0a1689918291/pulumi_kubernetes/storage/v1/CSIStorageCapacity.py` & `pulumi_kubernetes-4.1.0a1689971798/pulumi_kubernetes/storage/v1/CSIStorageCapacity.py`

 * *Files identical despite different names*

### Comparing `pulumi_kubernetes-4.1.0a1689918291/pulumi_kubernetes/storage/v1/CSIStorageCapacityList.py` & `pulumi_kubernetes-4.1.0a1689971798/pulumi_kubernetes/storage/v1/CSIStorageCapacityList.py`

 * *Files identical despite different names*

### Comparing `pulumi_kubernetes-4.1.0a1689918291/pulumi_kubernetes/storage/v1/CSIStorageCapacityPatch.py` & `pulumi_kubernetes-4.1.0a1689971798/pulumi_kubernetes/storage/v1/CSIStorageCapacityPatch.py`

 * *Files identical despite different names*

### Comparing `pulumi_kubernetes-4.1.0a1689918291/pulumi_kubernetes/storage/v1/StorageClass.py` & `pulumi_kubernetes-4.1.0a1689971798/pulumi_kubernetes/storage/v1/StorageClass.py`

 * *Files identical despite different names*

### Comparing `pulumi_kubernetes-4.1.0a1689918291/pulumi_kubernetes/storage/v1/StorageClassList.py` & `pulumi_kubernetes-4.1.0a1689971798/pulumi_kubernetes/storage/v1/StorageClassList.py`

 * *Files identical despite different names*

### Comparing `pulumi_kubernetes-4.1.0a1689918291/pulumi_kubernetes/storage/v1/StorageClassPatch.py` & `pulumi_kubernetes-4.1.0a1689971798/pulumi_kubernetes/storage/v1/StorageClassPatch.py`

 * *Files identical despite different names*

### Comparing `pulumi_kubernetes-4.1.0a1689918291/pulumi_kubernetes/storage/v1/VolumeAttachment.py` & `pulumi_kubernetes-4.1.0a1689971798/pulumi_kubernetes/storage/v1/VolumeAttachment.py`

 * *Files identical despite different names*

### Comparing `pulumi_kubernetes-4.1.0a1689918291/pulumi_kubernetes/storage/v1/VolumeAttachmentList.py` & `pulumi_kubernetes-4.1.0a1689971798/pulumi_kubernetes/storage/v1/VolumeAttachmentList.py`

 * *Files identical despite different names*

### Comparing `pulumi_kubernetes-4.1.0a1689918291/pulumi_kubernetes/storage/v1/VolumeAttachmentPatch.py` & `pulumi_kubernetes-4.1.0a1689971798/pulumi_kubernetes/storage/v1/VolumeAttachmentPatch.py`

 * *Files identical despite different names*

### Comparing `pulumi_kubernetes-4.1.0a1689918291/pulumi_kubernetes/storage/v1/__init__.py` & `pulumi_kubernetes-4.1.0a1689971798/pulumi_kubernetes/storage/v1/__init__.py`

 * *Files identical despite different names*

### Comparing `pulumi_kubernetes-4.1.0a1689918291/pulumi_kubernetes/storage/v1/_inputs.py` & `pulumi_kubernetes-4.1.0a1689971798/pulumi_kubernetes/storage/v1/_inputs.py`

 * *Files identical despite different names*

### Comparing `pulumi_kubernetes-4.1.0a1689918291/pulumi_kubernetes/storage/v1/outputs.py` & `pulumi_kubernetes-4.1.0a1689971798/pulumi_kubernetes/storage/v1/outputs.py`

 * *Files identical despite different names*

### Comparing `pulumi_kubernetes-4.1.0a1689918291/pulumi_kubernetes/storage/v1alpha1/VolumeAttachment.py` & `pulumi_kubernetes-4.1.0a1689971798/pulumi_kubernetes/storage/v1alpha1/VolumeAttachment.py`

 * *Files identical despite different names*

### Comparing `pulumi_kubernetes-4.1.0a1689918291/pulumi_kubernetes/storage/v1alpha1/VolumeAttachmentList.py` & `pulumi_kubernetes-4.1.0a1689971798/pulumi_kubernetes/storage/v1alpha1/VolumeAttachmentList.py`

 * *Files identical despite different names*

### Comparing `pulumi_kubernetes-4.1.0a1689918291/pulumi_kubernetes/storage/v1alpha1/VolumeAttachmentPatch.py` & `pulumi_kubernetes-4.1.0a1689971798/pulumi_kubernetes/storage/v1alpha1/VolumeAttachmentPatch.py`

 * *Files identical despite different names*

### Comparing `pulumi_kubernetes-4.1.0a1689918291/pulumi_kubernetes/storage/v1alpha1/_inputs.py` & `pulumi_kubernetes-4.1.0a1689971798/pulumi_kubernetes/storage/v1alpha1/_inputs.py`

 * *Files identical despite different names*

### Comparing `pulumi_kubernetes-4.1.0a1689918291/pulumi_kubernetes/storage/v1alpha1/outputs.py` & `pulumi_kubernetes-4.1.0a1689971798/pulumi_kubernetes/storage/v1alpha1/outputs.py`

 * *Files identical despite different names*

### Comparing `pulumi_kubernetes-4.1.0a1689918291/pulumi_kubernetes/storage/v1beta1/CSIDriver.py` & `pulumi_kubernetes-4.1.0a1689971798/pulumi_kubernetes/storage/v1beta1/CSIDriver.py`

 * *Files identical despite different names*

### Comparing `pulumi_kubernetes-4.1.0a1689918291/pulumi_kubernetes/storage/v1beta1/CSIDriverList.py` & `pulumi_kubernetes-4.1.0a1689971798/pulumi_kubernetes/storage/v1beta1/CSIDriverList.py`

 * *Files identical despite different names*

### Comparing `pulumi_kubernetes-4.1.0a1689918291/pulumi_kubernetes/storage/v1beta1/CSIDriverPatch.py` & `pulumi_kubernetes-4.1.0a1689971798/pulumi_kubernetes/storage/v1beta1/CSIDriverPatch.py`

 * *Files identical despite different names*

### Comparing `pulumi_kubernetes-4.1.0a1689918291/pulumi_kubernetes/storage/v1beta1/CSINode.py` & `pulumi_kubernetes-4.1.0a1689971798/pulumi_kubernetes/storage/v1beta1/CSINode.py`

 * *Files identical despite different names*

### Comparing `pulumi_kubernetes-4.1.0a1689918291/pulumi_kubernetes/storage/v1beta1/CSINodeList.py` & `pulumi_kubernetes-4.1.0a1689971798/pulumi_kubernetes/storage/v1beta1/CSINodeList.py`

 * *Files identical despite different names*

### Comparing `pulumi_kubernetes-4.1.0a1689918291/pulumi_kubernetes/storage/v1beta1/CSINodePatch.py` & `pulumi_kubernetes-4.1.0a1689971798/pulumi_kubernetes/storage/v1beta1/CSINodePatch.py`

 * *Files identical despite different names*

### Comparing `pulumi_kubernetes-4.1.0a1689918291/pulumi_kubernetes/storage/v1beta1/CSIStorageCapacity.py` & `pulumi_kubernetes-4.1.0a1689971798/pulumi_kubernetes/storage/v1beta1/CSIStorageCapacity.py`

 * *Files identical despite different names*

### Comparing `pulumi_kubernetes-4.1.0a1689918291/pulumi_kubernetes/storage/v1beta1/CSIStorageCapacityList.py` & `pulumi_kubernetes-4.1.0a1689971798/pulumi_kubernetes/storage/v1beta1/CSIStorageCapacityList.py`

 * *Files identical despite different names*

### Comparing `pulumi_kubernetes-4.1.0a1689918291/pulumi_kubernetes/storage/v1beta1/CSIStorageCapacityPatch.py` & `pulumi_kubernetes-4.1.0a1689971798/pulumi_kubernetes/storage/v1beta1/CSIStorageCapacityPatch.py`

 * *Files identical despite different names*

### Comparing `pulumi_kubernetes-4.1.0a1689918291/pulumi_kubernetes/storage/v1beta1/StorageClass.py` & `pulumi_kubernetes-4.1.0a1689971798/pulumi_kubernetes/storage/v1beta1/StorageClass.py`

 * *Files identical despite different names*

### Comparing `pulumi_kubernetes-4.1.0a1689918291/pulumi_kubernetes/storage/v1beta1/StorageClassList.py` & `pulumi_kubernetes-4.1.0a1689971798/pulumi_kubernetes/storage/v1beta1/StorageClassList.py`

 * *Files identical despite different names*

### Comparing `pulumi_kubernetes-4.1.0a1689918291/pulumi_kubernetes/storage/v1beta1/StorageClassPatch.py` & `pulumi_kubernetes-4.1.0a1689971798/pulumi_kubernetes/storage/v1beta1/StorageClassPatch.py`

 * *Files identical despite different names*

### Comparing `pulumi_kubernetes-4.1.0a1689918291/pulumi_kubernetes/storage/v1beta1/VolumeAttachment.py` & `pulumi_kubernetes-4.1.0a1689971798/pulumi_kubernetes/storage/v1beta1/VolumeAttachment.py`

 * *Files identical despite different names*

### Comparing `pulumi_kubernetes-4.1.0a1689918291/pulumi_kubernetes/storage/v1beta1/VolumeAttachmentList.py` & `pulumi_kubernetes-4.1.0a1689971798/pulumi_kubernetes/storage/v1beta1/VolumeAttachmentList.py`

 * *Files identical despite different names*

### Comparing `pulumi_kubernetes-4.1.0a1689918291/pulumi_kubernetes/storage/v1beta1/VolumeAttachmentPatch.py` & `pulumi_kubernetes-4.1.0a1689971798/pulumi_kubernetes/storage/v1beta1/VolumeAttachmentPatch.py`

 * *Files identical despite different names*

### Comparing `pulumi_kubernetes-4.1.0a1689918291/pulumi_kubernetes/storage/v1beta1/__init__.py` & `pulumi_kubernetes-4.1.0a1689971798/pulumi_kubernetes/storage/v1beta1/__init__.py`

 * *Files identical despite different names*

### Comparing `pulumi_kubernetes-4.1.0a1689918291/pulumi_kubernetes/storage/v1beta1/_inputs.py` & `pulumi_kubernetes-4.1.0a1689971798/pulumi_kubernetes/storage/v1beta1/_inputs.py`

 * *Files identical despite different names*

### Comparing `pulumi_kubernetes-4.1.0a1689918291/pulumi_kubernetes/storage/v1beta1/outputs.py` & `pulumi_kubernetes-4.1.0a1689971798/pulumi_kubernetes/storage/v1beta1/outputs.py`

 * *Files identical despite different names*

### Comparing `pulumi_kubernetes-4.1.0a1689918291/pulumi_kubernetes/yaml/yaml.py` & `pulumi_kubernetes-4.1.0a1689971798/pulumi_kubernetes/yaml/yaml.py`

 * *Files identical despite different names*

### Comparing `pulumi_kubernetes-4.1.0a1689918291/pulumi_kubernetes.egg-info/PKG-INFO` & `pulumi_kubernetes-4.1.0a1689971798/pulumi_kubernetes.egg-info/PKG-INFO`

 * *Files 1% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: pulumi-kubernetes
-Version: 4.1.0a1689918291
+Version: 4.1.0a1689971798
 Summary: A Pulumi package for creating and managing Kubernetes resources.
 Home-page: https://pulumi.com
 License: Apache-2.0
 Project-URL: Repository, https://github.com/pulumi/pulumi-kubernetes
 Description: [![Build Status](https://travis-ci.com/pulumi/pulumi-kubernetes.svg?token=eHg7Zp5zdDDJfTjY8ejq&branch=master)](https://travis-ci.com/pulumi/pulumi-kubernetes)
         [![Slack](http://www.pulumi.com/images/docs/badges/slack.svg)](https://slack.pulumi.com)
         [![NPM version](https://badge.fury.io/js/%40pulumi%2Fkubernetes.svg)](https://www.npmjs.com/package/@pulumi/kubernetes)
```

#### html2text {}

```diff
@@ -1,8 +1,8 @@
-Metadata-Version: 2.1 Name: pulumi-kubernetes Version: 4.1.0a1689918291
+Metadata-Version: 2.1 Name: pulumi-kubernetes Version: 4.1.0a1689971798
 Summary: A Pulumi package for creating and managing Kubernetes resources. Home-
 page: https://pulumi.com License: Apache-2.0 Project-URL: Repository, https://
 github.com/pulumi/pulumi-kubernetes Description: [![Build Status](https://
 travis-ci.com/pulumi/pulumi-
 kubernetes.svg?token=eHg7Zp5zdDDJfTjY8ejq&branch=master)](https://travis-
 ci.com/pulumi/pulumi-kubernetes) [![Slack](http://www.pulumi.com/images/docs/
 badges/slack.svg)](https://slack.pulumi.com) [![NPM version](https://
```

### Comparing `pulumi_kubernetes-4.1.0a1689918291/pulumi_kubernetes.egg-info/SOURCES.txt` & `pulumi_kubernetes-4.1.0a1689971798/pulumi_kubernetes.egg-info/SOURCES.txt`

 * *Files identical despite different names*

### Comparing `pulumi_kubernetes-4.1.0a1689918291/setup.py` & `pulumi_kubernetes-4.1.0a1689971798/setup.py`

 * *Files 8% similar despite different names*

```diff
@@ -4,16 +4,16 @@
 
 import errno
 from setuptools import setup, find_packages
 from setuptools.command.install import install
 from subprocess import check_call
 
 
-VERSION = "4.1.0a1689918291"
-PLUGIN_VERSION = "4.1.0-alpha.1689918291+26ddf792"
+VERSION = "4.1.0a1689971798"
+PLUGIN_VERSION = "4.1.0-alpha.1689971798+d88c6c17"
 
 class InstallPluginCommand(install):
     def run(self):
         install.run(self)
         try:
             check_call(['pulumi', 'plugin', 'install', 'resource', 'kubernetes', PLUGIN_VERSION])
         except OSError as error:
```

