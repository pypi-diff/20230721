# Comparing `tmp/mypy-boto3-workspaces-1.28.0.tar.gz` & `tmp/mypy-boto3-workspaces-1.28.9.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "mypy-boto3-workspaces-1.28.0.tar", last modified: Thu Jul  6 21:00:52 2023, max compression
+gzip compressed data, was "mypy-boto3-workspaces-1.28.9.tar", last modified: Fri Jul 21 20:32:58 2023, max compression
```

## Comparing `mypy-boto3-workspaces-1.28.0.tar` & `mypy-boto3-workspaces-1.28.9.tar`

### file list

```diff
@@ -1,27 +1,27 @@
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-06 21:00:52.910462 mypy-boto3-workspaces-1.28.0/
--rw-r--r--   0 runner    (1001) docker     (123)     1070 2023-07-06 20:58:22.000000 mypy-boto3-workspaces-1.28.0/LICENSE
--rw-r--r--   0 runner    (1001) docker     (123)    21998 2023-07-06 21:00:52.910462 mypy-boto3-workspaces-1.28.0/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (123)    20501 2023-07-06 20:58:22.000000 mypy-boto3-workspaces-1.28.0/README.md
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-06 21:00:52.910462 mypy-boto3-workspaces-1.28.0/mypy_boto3_workspaces/
--rw-r--r--   0 runner    (1001) docker     (123)     2528 2023-07-06 20:58:22.000000 mypy-boto3-workspaces-1.28.0/mypy_boto3_workspaces/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)     2527 2023-07-06 20:58:22.000000 mypy-boto3-workspaces-1.28.0/mypy_boto3_workspaces/__init__.pyi
--rw-r--r--   0 runner    (1001) docker     (123)      916 2023-07-06 20:58:22.000000 mypy-boto3-workspaces-1.28.0/mypy_boto3_workspaces/__main__.py
--rw-r--r--   0 runner    (1001) docker     (123)    48055 2023-07-06 20:58:22.000000 mypy-boto3-workspaces-1.28.0/mypy_boto3_workspaces/client.py
--rw-r--r--   0 runner    (1001) docker     (123)    47975 2023-07-06 20:58:22.000000 mypy-boto3-workspaces-1.28.0/mypy_boto3_workspaces/client.pyi
--rw-r--r--   0 runner    (1001) docker     (123)    13276 2023-07-06 20:58:23.000000 mypy-boto3-workspaces-1.28.0/mypy_boto3_workspaces/literals.py
--rw-r--r--   0 runner    (1001) docker     (123)    13274 2023-07-06 20:58:23.000000 mypy-boto3-workspaces-1.28.0/mypy_boto3_workspaces/literals.pyi
--rw-r--r--   0 runner    (1001) docker     (123)    10780 2023-07-06 20:58:23.000000 mypy-boto3-workspaces-1.28.0/mypy_boto3_workspaces/paginator.py
--rw-r--r--   0 runner    (1001) docker     (123)    10770 2023-07-06 20:58:22.000000 mypy-boto3-workspaces-1.28.0/mypy_boto3_workspaces/paginator.pyi
--rw-r--r--   0 runner    (1001) docker     (123)        0 2023-07-06 20:58:22.000000 mypy-boto3-workspaces-1.28.0/mypy_boto3_workspaces/py.typed
--rw-r--r--   0 runner    (1001) docker     (123)    53990 2023-07-06 20:58:24.000000 mypy-boto3-workspaces-1.28.0/mypy_boto3_workspaces/type_defs.py
--rw-r--r--   0 runner    (1001) docker     (123)    53949 2023-07-06 20:58:24.000000 mypy-boto3-workspaces-1.28.0/mypy_boto3_workspaces/type_defs.pyi
--rw-r--r--   0 runner    (1001) docker     (123)       60 2023-07-06 20:58:22.000000 mypy-boto3-workspaces-1.28.0/mypy_boto3_workspaces/version.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-06 21:00:52.910462 mypy-boto3-workspaces-1.28.0/mypy_boto3_workspaces.egg-info/
--rw-r--r--   0 runner    (1001) docker     (123)    21998 2023-07-06 21:00:52.000000 mypy-boto3-workspaces-1.28.0/mypy_boto3_workspaces.egg-info/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (123)      737 2023-07-06 21:00:52.000000 mypy-boto3-workspaces-1.28.0/mypy_boto3_workspaces.egg-info/SOURCES.txt
--rw-r--r--   0 runner    (1001) docker     (123)        1 2023-07-06 21:00:52.000000 mypy-boto3-workspaces-1.28.0/mypy_boto3_workspaces.egg-info/dependency_links.txt
--rw-r--r--   0 runner    (1001) docker     (123)        1 2023-07-06 21:00:52.000000 mypy-boto3-workspaces-1.28.0/mypy_boto3_workspaces.egg-info/not-zip-safe
--rw-r--r--   0 runner    (1001) docker     (123)       52 2023-07-06 21:00:52.000000 mypy-boto3-workspaces-1.28.0/mypy_boto3_workspaces.egg-info/requires.txt
--rw-r--r--   0 runner    (1001) docker     (123)       22 2023-07-06 21:00:52.000000 mypy-boto3-workspaces-1.28.0/mypy_boto3_workspaces.egg-info/top_level.txt
--rw-r--r--   0 runner    (1001) docker     (123)       38 2023-07-06 21:00:52.910462 mypy-boto3-workspaces-1.28.0/setup.cfg
--rw-r--r--   0 runner    (1001) docker     (123)     2015 2023-07-06 20:58:22.000000 mypy-boto3-workspaces-1.28.0/setup.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-21 20:32:58.251903 mypy-boto3-workspaces-1.28.9/
+-rw-r--r--   0 runner    (1001) docker     (123)     1070 2023-07-21 20:32:46.000000 mypy-boto3-workspaces-1.28.9/LICENSE
+-rw-r--r--   0 runner    (1001) docker     (123)    22493 2023-07-21 20:32:58.243903 mypy-boto3-workspaces-1.28.9/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (123)    20996 2023-07-21 20:32:46.000000 mypy-boto3-workspaces-1.28.9/README.md
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-21 20:32:58.243903 mypy-boto3-workspaces-1.28.9/mypy_boto3_workspaces/
+-rw-r--r--   0 runner    (1001) docker     (123)     2528 2023-07-21 20:32:46.000000 mypy-boto3-workspaces-1.28.9/mypy_boto3_workspaces/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)     2527 2023-07-21 20:32:46.000000 mypy-boto3-workspaces-1.28.9/mypy_boto3_workspaces/__init__.pyi
+-rw-r--r--   0 runner    (1001) docker     (123)      916 2023-07-21 20:32:46.000000 mypy-boto3-workspaces-1.28.9/mypy_boto3_workspaces/__main__.py
+-rw-r--r--   0 runner    (1001) docker     (123)    48055 2023-07-21 20:32:47.000000 mypy-boto3-workspaces-1.28.9/mypy_boto3_workspaces/client.py
+-rw-r--r--   0 runner    (1001) docker     (123)    47975 2023-07-21 20:32:46.000000 mypy-boto3-workspaces-1.28.9/mypy_boto3_workspaces/client.pyi
+-rw-r--r--   0 runner    (1001) docker     (123)    13299 2023-07-21 20:32:47.000000 mypy-boto3-workspaces-1.28.9/mypy_boto3_workspaces/literals.py
+-rw-r--r--   0 runner    (1001) docker     (123)    13297 2023-07-21 20:32:47.000000 mypy-boto3-workspaces-1.28.9/mypy_boto3_workspaces/literals.pyi
+-rw-r--r--   0 runner    (1001) docker     (123)    10740 2023-07-21 20:32:47.000000 mypy-boto3-workspaces-1.28.9/mypy_boto3_workspaces/paginator.py
+-rw-r--r--   0 runner    (1001) docker     (123)    10730 2023-07-21 20:32:47.000000 mypy-boto3-workspaces-1.28.9/mypy_boto3_workspaces/paginator.pyi
+-rw-r--r--   0 runner    (1001) docker     (123)        0 2023-07-21 20:32:46.000000 mypy-boto3-workspaces-1.28.9/mypy_boto3_workspaces/py.typed
+-rw-r--r--   0 runner    (1001) docker     (123)    57338 2023-07-21 20:32:48.000000 mypy-boto3-workspaces-1.28.9/mypy_boto3_workspaces/type_defs.py
+-rw-r--r--   0 runner    (1001) docker     (123)    57297 2023-07-21 20:32:47.000000 mypy-boto3-workspaces-1.28.9/mypy_boto3_workspaces/type_defs.pyi
+-rw-r--r--   0 runner    (1001) docker     (123)       60 2023-07-21 20:32:46.000000 mypy-boto3-workspaces-1.28.9/mypy_boto3_workspaces/version.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-21 20:32:58.243903 mypy-boto3-workspaces-1.28.9/mypy_boto3_workspaces.egg-info/
+-rw-r--r--   0 runner    (1001) docker     (123)    22493 2023-07-21 20:32:58.000000 mypy-boto3-workspaces-1.28.9/mypy_boto3_workspaces.egg-info/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (123)      737 2023-07-21 20:32:58.000000 mypy-boto3-workspaces-1.28.9/mypy_boto3_workspaces.egg-info/SOURCES.txt
+-rw-r--r--   0 runner    (1001) docker     (123)        1 2023-07-21 20:32:58.000000 mypy-boto3-workspaces-1.28.9/mypy_boto3_workspaces.egg-info/dependency_links.txt
+-rw-r--r--   0 runner    (1001) docker     (123)        1 2023-07-21 20:32:58.000000 mypy-boto3-workspaces-1.28.9/mypy_boto3_workspaces.egg-info/not-zip-safe
+-rw-r--r--   0 runner    (1001) docker     (123)       52 2023-07-21 20:32:58.000000 mypy-boto3-workspaces-1.28.9/mypy_boto3_workspaces.egg-info/requires.txt
+-rw-r--r--   0 runner    (1001) docker     (123)       22 2023-07-21 20:32:58.000000 mypy-boto3-workspaces-1.28.9/mypy_boto3_workspaces.egg-info/top_level.txt
+-rw-r--r--   0 runner    (1001) docker     (123)       38 2023-07-21 20:32:58.251903 mypy-boto3-workspaces-1.28.9/setup.cfg
+-rw-r--r--   0 runner    (1001) docker     (123)     2015 2023-07-21 20:32:46.000000 mypy-boto3-workspaces-1.28.9/setup.py
```

### Comparing `mypy-boto3-workspaces-1.28.0/LICENSE` & `mypy-boto3-workspaces-1.28.9/LICENSE`

 * *Files identical despite different names*

### Comparing `mypy-boto3-workspaces-1.28.0/PKG-INFO` & `mypy-boto3-workspaces-1.28.9/PKG-INFO`

 * *Files 2% similar despite different names*

```diff
@@ -1,11 +1,11 @@
 Metadata-Version: 2.1
 Name: mypy-boto3-workspaces
-Version: 1.28.0
-Summary: Type annotations for boto3.WorkSpaces 1.28.0 service generated with mypy-boto3-builder 7.14.5
+Version: 1.28.9
+Summary: Type annotations for boto3.WorkSpaces 1.28.9 service generated with mypy-boto3-builder 7.15.1
 Home-page: https://github.com/youtype/mypy_boto3_builder
 Author: Vlad Emelianov
 Author-email: vlad.emelianov.nz@gmail.com
 License: MIT License
 Project-URL: Documentation, https://youtype.github.io/boto3_stubs_docs/mypy_boto3_workspaces/
 Project-URL: Source, https://github.com/youtype/mypy_boto3_builder
 Project-URL: Tracker, https://github.com/youtype/mypy_boto3_builder/issues
@@ -38,24 +38,24 @@
 [![PyPI - Python Version](https://img.shields.io/pypi/pyversions/mypy-boto3-workspaces.svg?color=blue)](https://pypi.org/project/mypy-boto3-workspaces)
 [![Docs](https://img.shields.io/readthedocs/boto3-stubs.svg?color=blue)](https://youtype.github.io/boto3_stubs_docs/mypy_boto3_workspaces/)
 [![PyPI - Downloads](https://img.shields.io/pypi/dm/mypy-boto3-workspaces?color=blue)](https://pypistats.org/packages/mypy-boto3-workspaces)
 
 ![boto3.typed](https://github.com/youtype/mypy_boto3_builder/raw/main/logo.png)
 
 Type annotations for
-[boto3.WorkSpaces 1.28.0](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/workspaces.html#WorkSpaces)
+[boto3.WorkSpaces 1.28.9](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/workspaces.html#WorkSpaces)
 service compatible with [VSCode](https://code.visualstudio.com/),
 [PyCharm](https://www.jetbrains.com/pycharm/),
 [Emacs](https://www.gnu.org/software/emacs/),
 [Sublime Text](https://www.sublimetext.com/),
 [mypy](https://github.com/python/mypy),
 [pyright](https://github.com/microsoft/pyright) and other tools.
 
 Generated by
-[mypy-boto3-builder 7.14.5](https://github.com/youtype/mypy_boto3_builder).
+[mypy-boto3-builder 7.15.1](https://github.com/youtype/mypy_boto3_builder).
 
 More information can be found on
 [boto3-stubs](https://pypi.org/project/boto3-stubs/) page and in
 [mypy-boto3-workspaces docs](https://youtype.github.io/boto3_stubs_docs/mypy_boto3_workspaces/).
 
 See how it helps to find and fix potential bugs:
 
@@ -390,165 +390,179 @@
 `mypy_boto3_workspaces.type_defs` module contains structures and shapes
 assembled to typed dictionaries for additional type checking.
 
 ```python
 from mypy_boto3_workspaces.type_defs import (
     AccountModificationTypeDef,
     AssociateConnectionAliasRequestRequestTypeDef,
-    AssociateConnectionAliasResultTypeDef,
+    ResponseMetadataTypeDef,
     AssociateIpGroupsRequestRequestTypeDef,
     IpRuleItemTypeDef,
+    CertificateBasedAuthPropertiesOutputTypeDef,
     CertificateBasedAuthPropertiesTypeDef,
+    ClientPropertiesOutputTypeDef,
     ClientPropertiesTypeDef,
+    ComputeTypeOutputTypeDef,
     ComputeTypeTypeDef,
     ConnectClientAddInTypeDef,
     ConnectionAliasAssociationTypeDef,
+    ConnectionAliasPermissionOutputTypeDef,
     ConnectionAliasPermissionTypeDef,
     TagTypeDef,
-    CopyWorkspaceImageResultTypeDef,
     CreateConnectClientAddInRequestRequestTypeDef,
-    CreateConnectClientAddInResultTypeDef,
-    CreateConnectionAliasResultTypeDef,
-    CreateIpGroupResultTypeDef,
     PendingCreateStandbyWorkspacesRequestTypeDef,
-    CreateUpdatedWorkspaceImageResultTypeDef,
     RootStorageTypeDef,
     UserStorageTypeDef,
     OperatingSystemTypeDef,
     DefaultClientBrandingAttributesTypeDef,
     DefaultImportClientBrandingAttributesTypeDef,
     DefaultWorkspaceCreationPropertiesTypeDef,
     DeleteClientBrandingRequestRequestTypeDef,
     DeleteConnectClientAddInRequestRequestTypeDef,
     DeleteConnectionAliasRequestRequestTypeDef,
     DeleteIpGroupRequestRequestTypeDef,
     DeleteTagsRequestRequestTypeDef,
     DeleteWorkspaceBundleRequestRequestTypeDef,
     DeleteWorkspaceImageRequestRequestTypeDef,
     DeregisterWorkspaceDirectoryRequestRequestTypeDef,
-    DescribeAccountModificationsRequestDescribeAccountModificationsPaginateTypeDef,
+    PaginatorConfigTypeDef,
     DescribeAccountModificationsRequestRequestTypeDef,
-    DescribeAccountResultTypeDef,
     DescribeClientBrandingRequestRequestTypeDef,
     IosClientBrandingAttributesTypeDef,
     DescribeClientPropertiesRequestRequestTypeDef,
     DescribeConnectClientAddInsRequestRequestTypeDef,
     DescribeConnectionAliasPermissionsRequestRequestTypeDef,
     DescribeConnectionAliasesRequestRequestTypeDef,
-    DescribeIpGroupsRequestDescribeIpGroupsPaginateTypeDef,
     DescribeIpGroupsRequestRequestTypeDef,
     DescribeTagsRequestRequestTypeDef,
-    DescribeWorkspaceBundlesRequestDescribeWorkspaceBundlesPaginateTypeDef,
+    TagOutputTypeDef,
     DescribeWorkspaceBundlesRequestRequestTypeDef,
-    DescribeWorkspaceDirectoriesRequestDescribeWorkspaceDirectoriesPaginateTypeDef,
     DescribeWorkspaceDirectoriesRequestRequestTypeDef,
     DescribeWorkspaceImagePermissionsRequestRequestTypeDef,
     ImagePermissionTypeDef,
-    DescribeWorkspaceImagesRequestDescribeWorkspaceImagesPaginateTypeDef,
     DescribeWorkspaceImagesRequestRequestTypeDef,
     DescribeWorkspaceSnapshotsRequestRequestTypeDef,
     SnapshotTypeDef,
-    DescribeWorkspacesConnectionStatusRequestDescribeWorkspacesConnectionStatusPaginateTypeDef,
     DescribeWorkspacesConnectionStatusRequestRequestTypeDef,
     WorkspaceConnectionStatusTypeDef,
-    DescribeWorkspacesRequestDescribeWorkspacesPaginateTypeDef,
     DescribeWorkspacesRequestRequestTypeDef,
     DisassociateConnectionAliasRequestRequestTypeDef,
     DisassociateIpGroupsRequestRequestTypeDef,
     FailedWorkspaceChangeRequestTypeDef,
     IosImportClientBrandingAttributesTypeDef,
-    ImportWorkspaceImageResultTypeDef,
-    ListAvailableManagementCidrRangesRequestListAvailableManagementCidrRangesPaginateTypeDef,
+    IpRuleItemOutputTypeDef,
     ListAvailableManagementCidrRangesRequestRequestTypeDef,
-    ListAvailableManagementCidrRangesResultTypeDef,
     MigrateWorkspaceRequestRequestTypeDef,
-    MigrateWorkspaceResultTypeDef,
     ModificationStateTypeDef,
     ModifyAccountRequestRequestTypeDef,
     SamlPropertiesTypeDef,
     SelfservicePermissionsTypeDef,
     WorkspaceAccessPropertiesTypeDef,
     WorkspaceCreationPropertiesTypeDef,
     WorkspacePropertiesTypeDef,
     ModifyWorkspaceStateRequestRequestTypeDef,
-    PaginatorConfigTypeDef,
     RebootRequestTypeDef,
     RebuildRequestTypeDef,
     RelatedWorkspacePropertiesTypeDef,
-    ResponseMetadataTypeDef,
     RestoreWorkspaceRequestRequestTypeDef,
     RevokeIpRulesRequestRequestTypeDef,
+    RootStorageOutputTypeDef,
+    SamlPropertiesOutputTypeDef,
+    SelfservicePermissionsOutputTypeDef,
     StartRequestTypeDef,
     StopRequestTypeDef,
     TerminateRequestTypeDef,
     UpdateConnectClientAddInRequestRequestTypeDef,
     UpdateResultTypeDef,
     UpdateWorkspaceBundleRequestRequestTypeDef,
     UpdateWorkspaceImagePermissionRequestRequestTypeDef,
+    UserStorageOutputTypeDef,
+    WorkspaceAccessPropertiesOutputTypeDef,
+    WorkspacePropertiesOutputTypeDef,
+    AssociateConnectionAliasResultTypeDef,
+    CopyWorkspaceImageResultTypeDef,
+    CreateConnectClientAddInResultTypeDef,
+    CreateConnectionAliasResultTypeDef,
+    CreateIpGroupResultTypeDef,
+    CreateUpdatedWorkspaceImageResultTypeDef,
     DescribeAccountModificationsResultTypeDef,
+    DescribeAccountResultTypeDef,
+    ImportWorkspaceImageResultTypeDef,
+    ListAvailableManagementCidrRangesResultTypeDef,
+    MigrateWorkspaceResultTypeDef,
     AuthorizeIpRulesRequestRequestTypeDef,
     UpdateRulesOfIpGroupRequestRequestTypeDef,
-    WorkspacesIpGroupTypeDef,
     ModifyCertificateBasedAuthPropertiesRequestRequestTypeDef,
     ClientPropertiesResultTypeDef,
     ModifyClientPropertiesRequestRequestTypeDef,
     DescribeConnectClientAddInsResultTypeDef,
     ConnectionAliasTypeDef,
     DescribeConnectionAliasPermissionsResultTypeDef,
     UpdateConnectionAliasPermissionRequestRequestTypeDef,
     CopyWorkspaceImageRequestRequestTypeDef,
     CreateConnectionAliasRequestRequestTypeDef,
     CreateIpGroupRequestRequestTypeDef,
     CreateTagsRequestRequestTypeDef,
     CreateUpdatedWorkspaceImageRequestRequestTypeDef,
     CreateWorkspaceImageRequestRequestTypeDef,
-    DescribeTagsResultTypeDef,
     ImportWorkspaceImageRequestRequestTypeDef,
     RegisterWorkspaceDirectoryRequestRequestTypeDef,
     StandbyWorkspaceTypeDef,
     CreateWorkspaceBundleRequestRequestTypeDef,
-    WorkspaceBundleTypeDef,
     CreateWorkspaceImageResultTypeDef,
+    DescribeAccountModificationsRequestDescribeAccountModificationsPaginateTypeDef,
+    DescribeIpGroupsRequestDescribeIpGroupsPaginateTypeDef,
+    DescribeWorkspaceBundlesRequestDescribeWorkspaceBundlesPaginateTypeDef,
+    DescribeWorkspaceDirectoriesRequestDescribeWorkspaceDirectoriesPaginateTypeDef,
+    DescribeWorkspaceImagesRequestDescribeWorkspaceImagesPaginateTypeDef,
+    DescribeWorkspacesConnectionStatusRequestDescribeWorkspacesConnectionStatusPaginateTypeDef,
+    DescribeWorkspacesRequestDescribeWorkspacesPaginateTypeDef,
+    ListAvailableManagementCidrRangesRequestListAvailableManagementCidrRangesPaginateTypeDef,
     DescribeClientBrandingResultTypeDef,
     ImportClientBrandingResultTypeDef,
+    DescribeTagsResultTypeDef,
+    StandbyWorkspaceOutputTypeDef,
     DescribeWorkspaceImagePermissionsResultTypeDef,
     DescribeWorkspaceSnapshotsResultTypeDef,
     DescribeWorkspacesConnectionStatusResultTypeDef,
     RebootWorkspacesResultTypeDef,
     RebuildWorkspacesResultTypeDef,
     StartWorkspacesResultTypeDef,
     StopWorkspacesResultTypeDef,
     TerminateWorkspacesResultTypeDef,
     ImportClientBrandingRequestRequestTypeDef,
+    WorkspacesIpGroupTypeDef,
     ModifySamlPropertiesRequestRequestTypeDef,
     ModifySelfservicePermissionsRequestRequestTypeDef,
     ModifyWorkspaceAccessPropertiesRequestRequestTypeDef,
-    WorkspaceDirectoryTypeDef,
     ModifyWorkspaceCreationPropertiesRequestRequestTypeDef,
     ModifyWorkspacePropertiesRequestRequestTypeDef,
     WorkspaceRequestTypeDef,
     RebootWorkspacesRequestRequestTypeDef,
     RebuildWorkspacesRequestRequestTypeDef,
-    WorkspaceTypeDef,
     StartWorkspacesRequestRequestTypeDef,
     StopWorkspacesRequestRequestTypeDef,
     TerminateWorkspacesRequestRequestTypeDef,
     WorkspaceImageTypeDef,
-    DescribeIpGroupsResultTypeDef,
+    WorkspaceBundleTypeDef,
+    WorkspaceDirectoryTypeDef,
+    WorkspaceRequestOutputTypeDef,
+    WorkspaceTypeDef,
     DescribeClientPropertiesResultTypeDef,
     DescribeConnectionAliasesResultTypeDef,
     CreateStandbyWorkspacesRequestRequestTypeDef,
     FailedCreateStandbyWorkspacesRequestTypeDef,
+    DescribeIpGroupsResultTypeDef,
+    CreateWorkspacesRequestRequestTypeDef,
+    DescribeWorkspaceImagesResultTypeDef,
     CreateWorkspaceBundleResultTypeDef,
     DescribeWorkspaceBundlesResultTypeDef,
     DescribeWorkspaceDirectoriesResultTypeDef,
-    CreateWorkspacesRequestRequestTypeDef,
     FailedCreateWorkspaceRequestTypeDef,
     DescribeWorkspacesResultTypeDef,
-    DescribeWorkspaceImagesResultTypeDef,
     CreateStandbyWorkspacesResultTypeDef,
     CreateWorkspacesResultTypeDef,
 )
 
 
 def get_structure() -> AccountModificationTypeDef:
     return {...}
```

### Comparing `mypy-boto3-workspaces-1.28.0/README.md` & `mypy-boto3-workspaces-1.28.9/README.md`

 * *Files 3% similar despite different names*

```diff
@@ -6,24 +6,24 @@
 [![PyPI - Python Version](https://img.shields.io/pypi/pyversions/mypy-boto3-workspaces.svg?color=blue)](https://pypi.org/project/mypy-boto3-workspaces)
 [![Docs](https://img.shields.io/readthedocs/boto3-stubs.svg?color=blue)](https://youtype.github.io/boto3_stubs_docs/mypy_boto3_workspaces/)
 [![PyPI - Downloads](https://img.shields.io/pypi/dm/mypy-boto3-workspaces?color=blue)](https://pypistats.org/packages/mypy-boto3-workspaces)
 
 ![boto3.typed](https://github.com/youtype/mypy_boto3_builder/raw/main/logo.png)
 
 Type annotations for
-[boto3.WorkSpaces 1.28.0](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/workspaces.html#WorkSpaces)
+[boto3.WorkSpaces 1.28.9](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/workspaces.html#WorkSpaces)
 service compatible with [VSCode](https://code.visualstudio.com/),
 [PyCharm](https://www.jetbrains.com/pycharm/),
 [Emacs](https://www.gnu.org/software/emacs/),
 [Sublime Text](https://www.sublimetext.com/),
 [mypy](https://github.com/python/mypy),
 [pyright](https://github.com/microsoft/pyright) and other tools.
 
 Generated by
-[mypy-boto3-builder 7.14.5](https://github.com/youtype/mypy_boto3_builder).
+[mypy-boto3-builder 7.15.1](https://github.com/youtype/mypy_boto3_builder).
 
 More information can be found on
 [boto3-stubs](https://pypi.org/project/boto3-stubs/) page and in
 [mypy-boto3-workspaces docs](https://youtype.github.io/boto3_stubs_docs/mypy_boto3_workspaces/).
 
 See how it helps to find and fix potential bugs:
 
@@ -358,165 +358,179 @@
 `mypy_boto3_workspaces.type_defs` module contains structures and shapes
 assembled to typed dictionaries for additional type checking.
 
 ```python
 from mypy_boto3_workspaces.type_defs import (
     AccountModificationTypeDef,
     AssociateConnectionAliasRequestRequestTypeDef,
-    AssociateConnectionAliasResultTypeDef,
+    ResponseMetadataTypeDef,
     AssociateIpGroupsRequestRequestTypeDef,
     IpRuleItemTypeDef,
+    CertificateBasedAuthPropertiesOutputTypeDef,
     CertificateBasedAuthPropertiesTypeDef,
+    ClientPropertiesOutputTypeDef,
     ClientPropertiesTypeDef,
+    ComputeTypeOutputTypeDef,
     ComputeTypeTypeDef,
     ConnectClientAddInTypeDef,
     ConnectionAliasAssociationTypeDef,
+    ConnectionAliasPermissionOutputTypeDef,
     ConnectionAliasPermissionTypeDef,
     TagTypeDef,
-    CopyWorkspaceImageResultTypeDef,
     CreateConnectClientAddInRequestRequestTypeDef,
-    CreateConnectClientAddInResultTypeDef,
-    CreateConnectionAliasResultTypeDef,
-    CreateIpGroupResultTypeDef,
     PendingCreateStandbyWorkspacesRequestTypeDef,
-    CreateUpdatedWorkspaceImageResultTypeDef,
     RootStorageTypeDef,
     UserStorageTypeDef,
     OperatingSystemTypeDef,
     DefaultClientBrandingAttributesTypeDef,
     DefaultImportClientBrandingAttributesTypeDef,
     DefaultWorkspaceCreationPropertiesTypeDef,
     DeleteClientBrandingRequestRequestTypeDef,
     DeleteConnectClientAddInRequestRequestTypeDef,
     DeleteConnectionAliasRequestRequestTypeDef,
     DeleteIpGroupRequestRequestTypeDef,
     DeleteTagsRequestRequestTypeDef,
     DeleteWorkspaceBundleRequestRequestTypeDef,
     DeleteWorkspaceImageRequestRequestTypeDef,
     DeregisterWorkspaceDirectoryRequestRequestTypeDef,
-    DescribeAccountModificationsRequestDescribeAccountModificationsPaginateTypeDef,
+    PaginatorConfigTypeDef,
     DescribeAccountModificationsRequestRequestTypeDef,
-    DescribeAccountResultTypeDef,
     DescribeClientBrandingRequestRequestTypeDef,
     IosClientBrandingAttributesTypeDef,
     DescribeClientPropertiesRequestRequestTypeDef,
     DescribeConnectClientAddInsRequestRequestTypeDef,
     DescribeConnectionAliasPermissionsRequestRequestTypeDef,
     DescribeConnectionAliasesRequestRequestTypeDef,
-    DescribeIpGroupsRequestDescribeIpGroupsPaginateTypeDef,
     DescribeIpGroupsRequestRequestTypeDef,
     DescribeTagsRequestRequestTypeDef,
-    DescribeWorkspaceBundlesRequestDescribeWorkspaceBundlesPaginateTypeDef,
+    TagOutputTypeDef,
     DescribeWorkspaceBundlesRequestRequestTypeDef,
-    DescribeWorkspaceDirectoriesRequestDescribeWorkspaceDirectoriesPaginateTypeDef,
     DescribeWorkspaceDirectoriesRequestRequestTypeDef,
     DescribeWorkspaceImagePermissionsRequestRequestTypeDef,
     ImagePermissionTypeDef,
-    DescribeWorkspaceImagesRequestDescribeWorkspaceImagesPaginateTypeDef,
     DescribeWorkspaceImagesRequestRequestTypeDef,
     DescribeWorkspaceSnapshotsRequestRequestTypeDef,
     SnapshotTypeDef,
-    DescribeWorkspacesConnectionStatusRequestDescribeWorkspacesConnectionStatusPaginateTypeDef,
     DescribeWorkspacesConnectionStatusRequestRequestTypeDef,
     WorkspaceConnectionStatusTypeDef,
-    DescribeWorkspacesRequestDescribeWorkspacesPaginateTypeDef,
     DescribeWorkspacesRequestRequestTypeDef,
     DisassociateConnectionAliasRequestRequestTypeDef,
     DisassociateIpGroupsRequestRequestTypeDef,
     FailedWorkspaceChangeRequestTypeDef,
     IosImportClientBrandingAttributesTypeDef,
-    ImportWorkspaceImageResultTypeDef,
-    ListAvailableManagementCidrRangesRequestListAvailableManagementCidrRangesPaginateTypeDef,
+    IpRuleItemOutputTypeDef,
     ListAvailableManagementCidrRangesRequestRequestTypeDef,
-    ListAvailableManagementCidrRangesResultTypeDef,
     MigrateWorkspaceRequestRequestTypeDef,
-    MigrateWorkspaceResultTypeDef,
     ModificationStateTypeDef,
     ModifyAccountRequestRequestTypeDef,
     SamlPropertiesTypeDef,
     SelfservicePermissionsTypeDef,
     WorkspaceAccessPropertiesTypeDef,
     WorkspaceCreationPropertiesTypeDef,
     WorkspacePropertiesTypeDef,
     ModifyWorkspaceStateRequestRequestTypeDef,
-    PaginatorConfigTypeDef,
     RebootRequestTypeDef,
     RebuildRequestTypeDef,
     RelatedWorkspacePropertiesTypeDef,
-    ResponseMetadataTypeDef,
     RestoreWorkspaceRequestRequestTypeDef,
     RevokeIpRulesRequestRequestTypeDef,
+    RootStorageOutputTypeDef,
+    SamlPropertiesOutputTypeDef,
+    SelfservicePermissionsOutputTypeDef,
     StartRequestTypeDef,
     StopRequestTypeDef,
     TerminateRequestTypeDef,
     UpdateConnectClientAddInRequestRequestTypeDef,
     UpdateResultTypeDef,
     UpdateWorkspaceBundleRequestRequestTypeDef,
     UpdateWorkspaceImagePermissionRequestRequestTypeDef,
+    UserStorageOutputTypeDef,
+    WorkspaceAccessPropertiesOutputTypeDef,
+    WorkspacePropertiesOutputTypeDef,
+    AssociateConnectionAliasResultTypeDef,
+    CopyWorkspaceImageResultTypeDef,
+    CreateConnectClientAddInResultTypeDef,
+    CreateConnectionAliasResultTypeDef,
+    CreateIpGroupResultTypeDef,
+    CreateUpdatedWorkspaceImageResultTypeDef,
     DescribeAccountModificationsResultTypeDef,
+    DescribeAccountResultTypeDef,
+    ImportWorkspaceImageResultTypeDef,
+    ListAvailableManagementCidrRangesResultTypeDef,
+    MigrateWorkspaceResultTypeDef,
     AuthorizeIpRulesRequestRequestTypeDef,
     UpdateRulesOfIpGroupRequestRequestTypeDef,
-    WorkspacesIpGroupTypeDef,
     ModifyCertificateBasedAuthPropertiesRequestRequestTypeDef,
     ClientPropertiesResultTypeDef,
     ModifyClientPropertiesRequestRequestTypeDef,
     DescribeConnectClientAddInsResultTypeDef,
     ConnectionAliasTypeDef,
     DescribeConnectionAliasPermissionsResultTypeDef,
     UpdateConnectionAliasPermissionRequestRequestTypeDef,
     CopyWorkspaceImageRequestRequestTypeDef,
     CreateConnectionAliasRequestRequestTypeDef,
     CreateIpGroupRequestRequestTypeDef,
     CreateTagsRequestRequestTypeDef,
     CreateUpdatedWorkspaceImageRequestRequestTypeDef,
     CreateWorkspaceImageRequestRequestTypeDef,
-    DescribeTagsResultTypeDef,
     ImportWorkspaceImageRequestRequestTypeDef,
     RegisterWorkspaceDirectoryRequestRequestTypeDef,
     StandbyWorkspaceTypeDef,
     CreateWorkspaceBundleRequestRequestTypeDef,
-    WorkspaceBundleTypeDef,
     CreateWorkspaceImageResultTypeDef,
+    DescribeAccountModificationsRequestDescribeAccountModificationsPaginateTypeDef,
+    DescribeIpGroupsRequestDescribeIpGroupsPaginateTypeDef,
+    DescribeWorkspaceBundlesRequestDescribeWorkspaceBundlesPaginateTypeDef,
+    DescribeWorkspaceDirectoriesRequestDescribeWorkspaceDirectoriesPaginateTypeDef,
+    DescribeWorkspaceImagesRequestDescribeWorkspaceImagesPaginateTypeDef,
+    DescribeWorkspacesConnectionStatusRequestDescribeWorkspacesConnectionStatusPaginateTypeDef,
+    DescribeWorkspacesRequestDescribeWorkspacesPaginateTypeDef,
+    ListAvailableManagementCidrRangesRequestListAvailableManagementCidrRangesPaginateTypeDef,
     DescribeClientBrandingResultTypeDef,
     ImportClientBrandingResultTypeDef,
+    DescribeTagsResultTypeDef,
+    StandbyWorkspaceOutputTypeDef,
     DescribeWorkspaceImagePermissionsResultTypeDef,
     DescribeWorkspaceSnapshotsResultTypeDef,
     DescribeWorkspacesConnectionStatusResultTypeDef,
     RebootWorkspacesResultTypeDef,
     RebuildWorkspacesResultTypeDef,
     StartWorkspacesResultTypeDef,
     StopWorkspacesResultTypeDef,
     TerminateWorkspacesResultTypeDef,
     ImportClientBrandingRequestRequestTypeDef,
+    WorkspacesIpGroupTypeDef,
     ModifySamlPropertiesRequestRequestTypeDef,
     ModifySelfservicePermissionsRequestRequestTypeDef,
     ModifyWorkspaceAccessPropertiesRequestRequestTypeDef,
-    WorkspaceDirectoryTypeDef,
     ModifyWorkspaceCreationPropertiesRequestRequestTypeDef,
     ModifyWorkspacePropertiesRequestRequestTypeDef,
     WorkspaceRequestTypeDef,
     RebootWorkspacesRequestRequestTypeDef,
     RebuildWorkspacesRequestRequestTypeDef,
-    WorkspaceTypeDef,
     StartWorkspacesRequestRequestTypeDef,
     StopWorkspacesRequestRequestTypeDef,
     TerminateWorkspacesRequestRequestTypeDef,
     WorkspaceImageTypeDef,
-    DescribeIpGroupsResultTypeDef,
+    WorkspaceBundleTypeDef,
+    WorkspaceDirectoryTypeDef,
+    WorkspaceRequestOutputTypeDef,
+    WorkspaceTypeDef,
     DescribeClientPropertiesResultTypeDef,
     DescribeConnectionAliasesResultTypeDef,
     CreateStandbyWorkspacesRequestRequestTypeDef,
     FailedCreateStandbyWorkspacesRequestTypeDef,
+    DescribeIpGroupsResultTypeDef,
+    CreateWorkspacesRequestRequestTypeDef,
+    DescribeWorkspaceImagesResultTypeDef,
     CreateWorkspaceBundleResultTypeDef,
     DescribeWorkspaceBundlesResultTypeDef,
     DescribeWorkspaceDirectoriesResultTypeDef,
-    CreateWorkspacesRequestRequestTypeDef,
     FailedCreateWorkspaceRequestTypeDef,
     DescribeWorkspacesResultTypeDef,
-    DescribeWorkspaceImagesResultTypeDef,
     CreateStandbyWorkspacesResultTypeDef,
     CreateWorkspacesResultTypeDef,
 )
 
 
 def get_structure() -> AccountModificationTypeDef:
     return {...}
```

### Comparing `mypy-boto3-workspaces-1.28.0/mypy_boto3_workspaces/__init__.py` & `mypy-boto3-workspaces-1.28.9/mypy_boto3_workspaces/__init__.py`

 * *Files identical despite different names*

### Comparing `mypy-boto3-workspaces-1.28.0/mypy_boto3_workspaces/__init__.pyi` & `mypy-boto3-workspaces-1.28.9/mypy_boto3_workspaces/__init__.pyi`

 * *Files identical despite different names*

### Comparing `mypy-boto3-workspaces-1.28.0/mypy_boto3_workspaces/__main__.py` & `mypy-boto3-workspaces-1.28.9/mypy_boto3_workspaces/__main__.py`

 * *Files 4% similar despite different names*

```diff
@@ -5,28 +5,28 @@
 
 
 def print_info() -> None:
     """
     Print package info to stdout.
     """
     print(
-        "Type annotations for boto3.WorkSpaces 1.28.0\nVersion:         1.28.0\nBuilder version:"
-        " 7.14.5\nDocs:           "
+        "Type annotations for boto3.WorkSpaces 1.28.9\nVersion:         1.28.9\nBuilder version:"
+        " 7.15.1\nDocs:           "
         " https://youtype.github.io/boto3_stubs_docs/mypy_boto3_workspaces//\nBoto3 docs:     "
         " https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/workspaces.html#WorkSpaces\nOther"
         " services:  https://pypi.org/project/boto3-stubs/\nChangelog:      "
         " https://github.com/youtype/mypy_boto3_builder/releases"
     )
 
 
 def print_version() -> None:
     """
     Print package version to stdout.
     """
-    print("1.28.0")
+    print("1.28.9")
 
 
 def main() -> None:
     """
     Main CLI entrypoint.
     """
     if "--version" in sys.argv:
```

### Comparing `mypy-boto3-workspaces-1.28.0/mypy_boto3_workspaces/client.py` & `mypy-boto3-workspaces-1.28.9/mypy_boto3_workspaces/client.py`

 * *Files identical despite different names*

### Comparing `mypy-boto3-workspaces-1.28.0/mypy_boto3_workspaces/client.pyi` & `mypy-boto3-workspaces-1.28.9/mypy_boto3_workspaces/client.pyi`

 * *Files identical despite different names*

### Comparing `mypy-boto3-workspaces-1.28.0/mypy_boto3_workspaces/literals.py` & `mypy-boto3-workspaces-1.28.9/mypy_boto3_workspaces/literals.py`

 * *Files 0% similar despite different names*

```diff
@@ -379,14 +379,15 @@
     "medialive",
     "mediapackage",
     "mediapackage-vod",
     "mediapackagev2",
     "mediastore",
     "mediastore-data",
     "mediatailor",
+    "medical-imaging",
     "memorydb",
     "meteringmarketplace",
     "mgh",
     "mgn",
     "migration-hub-refactor-spaces",
     "migrationhub-config",
     "migrationhuborchestrator",
```

### Comparing `mypy-boto3-workspaces-1.28.0/mypy_boto3_workspaces/literals.pyi` & `mypy-boto3-workspaces-1.28.9/mypy_boto3_workspaces/literals.pyi`

 * *Files 0% similar despite different names*

```diff
@@ -377,14 +377,15 @@
     "medialive",
     "mediapackage",
     "mediapackage-vod",
     "mediapackagev2",
     "mediastore",
     "mediastore-data",
     "mediatailor",
+    "medical-imaging",
     "memorydb",
     "meteringmarketplace",
     "mgh",
     "mgn",
     "migration-hub-refactor-spaces",
     "migrationhub-config",
     "migrationhuborchestrator",
```

### Comparing `mypy-boto3-workspaces-1.28.0/mypy_boto3_workspaces/paginator.py` & `mypy-boto3-workspaces-1.28.9/mypy_boto3_workspaces/paginator.py`

 * *Files 3% similar despite different names*

```diff
@@ -75,30 +75,30 @@
 class DescribeAccountModificationsPaginator(Paginator):
     """
     [Show boto3 documentation](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/workspaces.html#WorkSpaces.Paginator.DescribeAccountModifications)
     [Show boto3-stubs documentation](https://youtype.github.io/boto3_stubs_docs/mypy_boto3_workspaces/paginators/#describeaccountmodificationspaginator)
     """
 
     def paginate(
-        self, *, PaginationConfig: "PaginatorConfigTypeDef" = ...
+        self, *, PaginationConfig: PaginatorConfigTypeDef = ...
     ) -> _PageIterator[DescribeAccountModificationsResultTypeDef]:
         """
         [Show boto3 documentation](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/workspaces.html#WorkSpaces.Paginator.DescribeAccountModifications.paginate)
         [Show boto3-stubs documentation](https://youtype.github.io/boto3_stubs_docs/mypy_boto3_workspaces/paginators/#describeaccountmodificationspaginator)
         """
 
 
 class DescribeIpGroupsPaginator(Paginator):
     """
     [Show boto3 documentation](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/workspaces.html#WorkSpaces.Paginator.DescribeIpGroups)
     [Show boto3-stubs documentation](https://youtype.github.io/boto3_stubs_docs/mypy_boto3_workspaces/paginators/#describeipgroupspaginator)
     """
 
     def paginate(
-        self, *, GroupIds: Sequence[str] = ..., PaginationConfig: "PaginatorConfigTypeDef" = ...
+        self, *, GroupIds: Sequence[str] = ..., PaginationConfig: PaginatorConfigTypeDef = ...
     ) -> _PageIterator[DescribeIpGroupsResultTypeDef]:
         """
         [Show boto3 documentation](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/workspaces.html#WorkSpaces.Paginator.DescribeIpGroups.paginate)
         [Show boto3-stubs documentation](https://youtype.github.io/boto3_stubs_docs/mypy_boto3_workspaces/paginators/#describeipgroupspaginator)
         """
 
 
@@ -109,15 +109,15 @@
     """
 
     def paginate(
         self,
         *,
         BundleIds: Sequence[str] = ...,
         Owner: str = ...,
-        PaginationConfig: "PaginatorConfigTypeDef" = ...
+        PaginationConfig: PaginatorConfigTypeDef = ...
     ) -> _PageIterator[DescribeWorkspaceBundlesResultTypeDef]:
         """
         [Show boto3 documentation](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/workspaces.html#WorkSpaces.Paginator.DescribeWorkspaceBundles.paginate)
         [Show boto3-stubs documentation](https://youtype.github.io/boto3_stubs_docs/mypy_boto3_workspaces/paginators/#describeworkspacebundlespaginator)
         """
 
 
@@ -128,15 +128,15 @@
     """
 
     def paginate(
         self,
         *,
         DirectoryIds: Sequence[str] = ...,
         Limit: int = ...,
-        PaginationConfig: "PaginatorConfigTypeDef" = ...
+        PaginationConfig: PaginatorConfigTypeDef = ...
     ) -> _PageIterator[DescribeWorkspaceDirectoriesResultTypeDef]:
         """
         [Show boto3 documentation](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/workspaces.html#WorkSpaces.Paginator.DescribeWorkspaceDirectories.paginate)
         [Show boto3-stubs documentation](https://youtype.github.io/boto3_stubs_docs/mypy_boto3_workspaces/paginators/#describeworkspacedirectoriespaginator)
         """
 
 
@@ -147,15 +147,15 @@
     """
 
     def paginate(
         self,
         *,
         ImageIds: Sequence[str] = ...,
         ImageType: ImageTypeType = ...,
-        PaginationConfig: "PaginatorConfigTypeDef" = ...
+        PaginationConfig: PaginatorConfigTypeDef = ...
     ) -> _PageIterator[DescribeWorkspaceImagesResultTypeDef]:
         """
         [Show boto3 documentation](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/workspaces.html#WorkSpaces.Paginator.DescribeWorkspaceImages.paginate)
         [Show boto3-stubs documentation](https://youtype.github.io/boto3_stubs_docs/mypy_boto3_workspaces/paginators/#describeworkspaceimagespaginator)
         """
 
 
@@ -168,46 +168,43 @@
     def paginate(
         self,
         *,
         WorkspaceIds: Sequence[str] = ...,
         DirectoryId: str = ...,
         UserName: str = ...,
         BundleId: str = ...,
-        PaginationConfig: "PaginatorConfigTypeDef" = ...
+        PaginationConfig: PaginatorConfigTypeDef = ...
     ) -> _PageIterator[DescribeWorkspacesResultTypeDef]:
         """
         [Show boto3 documentation](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/workspaces.html#WorkSpaces.Paginator.DescribeWorkspaces.paginate)
         [Show boto3-stubs documentation](https://youtype.github.io/boto3_stubs_docs/mypy_boto3_workspaces/paginators/#describeworkspacespaginator)
         """
 
 
 class DescribeWorkspacesConnectionStatusPaginator(Paginator):
     """
     [Show boto3 documentation](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/workspaces.html#WorkSpaces.Paginator.DescribeWorkspacesConnectionStatus)
     [Show boto3-stubs documentation](https://youtype.github.io/boto3_stubs_docs/mypy_boto3_workspaces/paginators/#describeworkspacesconnectionstatuspaginator)
     """
 
     def paginate(
-        self, *, WorkspaceIds: Sequence[str] = ..., PaginationConfig: "PaginatorConfigTypeDef" = ...
+        self, *, WorkspaceIds: Sequence[str] = ..., PaginationConfig: PaginatorConfigTypeDef = ...
     ) -> _PageIterator[DescribeWorkspacesConnectionStatusResultTypeDef]:
         """
         [Show boto3 documentation](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/workspaces.html#WorkSpaces.Paginator.DescribeWorkspacesConnectionStatus.paginate)
         [Show boto3-stubs documentation](https://youtype.github.io/boto3_stubs_docs/mypy_boto3_workspaces/paginators/#describeworkspacesconnectionstatuspaginator)
         """
 
 
 class ListAvailableManagementCidrRangesPaginator(Paginator):
     """
     [Show boto3 documentation](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/workspaces.html#WorkSpaces.Paginator.ListAvailableManagementCidrRanges)
     [Show boto3-stubs documentation](https://youtype.github.io/boto3_stubs_docs/mypy_boto3_workspaces/paginators/#listavailablemanagementcidrrangespaginator)
     """
 
     def paginate(
-        self,
-        *,
-        ManagementCidrRangeConstraint: str,
-        PaginationConfig: "PaginatorConfigTypeDef" = ...
+        self, *, ManagementCidrRangeConstraint: str, PaginationConfig: PaginatorConfigTypeDef = ...
     ) -> _PageIterator[ListAvailableManagementCidrRangesResultTypeDef]:
         """
         [Show boto3 documentation](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/workspaces.html#WorkSpaces.Paginator.ListAvailableManagementCidrRanges.paginate)
         [Show boto3-stubs documentation](https://youtype.github.io/boto3_stubs_docs/mypy_boto3_workspaces/paginators/#listavailablemanagementcidrrangespaginator)
         """
```

### Comparing `mypy-boto3-workspaces-1.28.0/mypy_boto3_workspaces/paginator.pyi` & `mypy-boto3-workspaces-1.28.9/mypy_boto3_workspaces/paginator.pyi`

 * *Files 6% similar despite different names*

```diff
@@ -72,29 +72,29 @@
 class DescribeAccountModificationsPaginator(Paginator):
     """
     [Show boto3 documentation](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/workspaces.html#WorkSpaces.Paginator.DescribeAccountModifications)
     [Show boto3-stubs documentation](https://youtype.github.io/boto3_stubs_docs/mypy_boto3_workspaces/paginators/#describeaccountmodificationspaginator)
     """
 
     def paginate(
-        self, *, PaginationConfig: "PaginatorConfigTypeDef" = ...
+        self, *, PaginationConfig: PaginatorConfigTypeDef = ...
     ) -> _PageIterator[DescribeAccountModificationsResultTypeDef]:
         """
         [Show boto3 documentation](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/workspaces.html#WorkSpaces.Paginator.DescribeAccountModifications.paginate)
         [Show boto3-stubs documentation](https://youtype.github.io/boto3_stubs_docs/mypy_boto3_workspaces/paginators/#describeaccountmodificationspaginator)
         """
 
 class DescribeIpGroupsPaginator(Paginator):
     """
     [Show boto3 documentation](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/workspaces.html#WorkSpaces.Paginator.DescribeIpGroups)
     [Show boto3-stubs documentation](https://youtype.github.io/boto3_stubs_docs/mypy_boto3_workspaces/paginators/#describeipgroupspaginator)
     """
 
     def paginate(
-        self, *, GroupIds: Sequence[str] = ..., PaginationConfig: "PaginatorConfigTypeDef" = ...
+        self, *, GroupIds: Sequence[str] = ..., PaginationConfig: PaginatorConfigTypeDef = ...
     ) -> _PageIterator[DescribeIpGroupsResultTypeDef]:
         """
         [Show boto3 documentation](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/workspaces.html#WorkSpaces.Paginator.DescribeIpGroups.paginate)
         [Show boto3-stubs documentation](https://youtype.github.io/boto3_stubs_docs/mypy_boto3_workspaces/paginators/#describeipgroupspaginator)
         """
 
 class DescribeWorkspaceBundlesPaginator(Paginator):
@@ -104,15 +104,15 @@
     """
 
     def paginate(
         self,
         *,
         BundleIds: Sequence[str] = ...,
         Owner: str = ...,
-        PaginationConfig: "PaginatorConfigTypeDef" = ...
+        PaginationConfig: PaginatorConfigTypeDef = ...
     ) -> _PageIterator[DescribeWorkspaceBundlesResultTypeDef]:
         """
         [Show boto3 documentation](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/workspaces.html#WorkSpaces.Paginator.DescribeWorkspaceBundles.paginate)
         [Show boto3-stubs documentation](https://youtype.github.io/boto3_stubs_docs/mypy_boto3_workspaces/paginators/#describeworkspacebundlespaginator)
         """
 
 class DescribeWorkspaceDirectoriesPaginator(Paginator):
@@ -122,15 +122,15 @@
     """
 
     def paginate(
         self,
         *,
         DirectoryIds: Sequence[str] = ...,
         Limit: int = ...,
-        PaginationConfig: "PaginatorConfigTypeDef" = ...
+        PaginationConfig: PaginatorConfigTypeDef = ...
     ) -> _PageIterator[DescribeWorkspaceDirectoriesResultTypeDef]:
         """
         [Show boto3 documentation](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/workspaces.html#WorkSpaces.Paginator.DescribeWorkspaceDirectories.paginate)
         [Show boto3-stubs documentation](https://youtype.github.io/boto3_stubs_docs/mypy_boto3_workspaces/paginators/#describeworkspacedirectoriespaginator)
         """
 
 class DescribeWorkspaceImagesPaginator(Paginator):
@@ -140,15 +140,15 @@
     """
 
     def paginate(
         self,
         *,
         ImageIds: Sequence[str] = ...,
         ImageType: ImageTypeType = ...,
-        PaginationConfig: "PaginatorConfigTypeDef" = ...
+        PaginationConfig: PaginatorConfigTypeDef = ...
     ) -> _PageIterator[DescribeWorkspaceImagesResultTypeDef]:
         """
         [Show boto3 documentation](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/workspaces.html#WorkSpaces.Paginator.DescribeWorkspaceImages.paginate)
         [Show boto3-stubs documentation](https://youtype.github.io/boto3_stubs_docs/mypy_boto3_workspaces/paginators/#describeworkspaceimagespaginator)
         """
 
 class DescribeWorkspacesPaginator(Paginator):
@@ -160,44 +160,41 @@
     def paginate(
         self,
         *,
         WorkspaceIds: Sequence[str] = ...,
         DirectoryId: str = ...,
         UserName: str = ...,
         BundleId: str = ...,
-        PaginationConfig: "PaginatorConfigTypeDef" = ...
+        PaginationConfig: PaginatorConfigTypeDef = ...
     ) -> _PageIterator[DescribeWorkspacesResultTypeDef]:
         """
         [Show boto3 documentation](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/workspaces.html#WorkSpaces.Paginator.DescribeWorkspaces.paginate)
         [Show boto3-stubs documentation](https://youtype.github.io/boto3_stubs_docs/mypy_boto3_workspaces/paginators/#describeworkspacespaginator)
         """
 
 class DescribeWorkspacesConnectionStatusPaginator(Paginator):
     """
     [Show boto3 documentation](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/workspaces.html#WorkSpaces.Paginator.DescribeWorkspacesConnectionStatus)
     [Show boto3-stubs documentation](https://youtype.github.io/boto3_stubs_docs/mypy_boto3_workspaces/paginators/#describeworkspacesconnectionstatuspaginator)
     """
 
     def paginate(
-        self, *, WorkspaceIds: Sequence[str] = ..., PaginationConfig: "PaginatorConfigTypeDef" = ...
+        self, *, WorkspaceIds: Sequence[str] = ..., PaginationConfig: PaginatorConfigTypeDef = ...
     ) -> _PageIterator[DescribeWorkspacesConnectionStatusResultTypeDef]:
         """
         [Show boto3 documentation](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/workspaces.html#WorkSpaces.Paginator.DescribeWorkspacesConnectionStatus.paginate)
         [Show boto3-stubs documentation](https://youtype.github.io/boto3_stubs_docs/mypy_boto3_workspaces/paginators/#describeworkspacesconnectionstatuspaginator)
         """
 
 class ListAvailableManagementCidrRangesPaginator(Paginator):
     """
     [Show boto3 documentation](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/workspaces.html#WorkSpaces.Paginator.ListAvailableManagementCidrRanges)
     [Show boto3-stubs documentation](https://youtype.github.io/boto3_stubs_docs/mypy_boto3_workspaces/paginators/#listavailablemanagementcidrrangespaginator)
     """
 
     def paginate(
-        self,
-        *,
-        ManagementCidrRangeConstraint: str,
-        PaginationConfig: "PaginatorConfigTypeDef" = ...
+        self, *, ManagementCidrRangeConstraint: str, PaginationConfig: PaginatorConfigTypeDef = ...
     ) -> _PageIterator[ListAvailableManagementCidrRangesResultTypeDef]:
         """
         [Show boto3 documentation](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/workspaces.html#WorkSpaces.Paginator.ListAvailableManagementCidrRanges.paginate)
         [Show boto3-stubs documentation](https://youtype.github.io/boto3_stubs_docs/mypy_boto3_workspaces/paginators/#listavailablemanagementcidrrangespaginator)
         """
```

### Comparing `mypy-boto3-workspaces-1.28.0/mypy_boto3_workspaces/type_defs.py` & `mypy-boto3-workspaces-1.28.9/mypy_boto3_workspaces/type_defs.py`

 * *Files 3% similar despite different names*

```diff
@@ -60,195 +60,211 @@
 else:
     from typing_extensions import TypedDict
 
 
 __all__ = (
     "AccountModificationTypeDef",
     "AssociateConnectionAliasRequestRequestTypeDef",
-    "AssociateConnectionAliasResultTypeDef",
+    "ResponseMetadataTypeDef",
     "AssociateIpGroupsRequestRequestTypeDef",
     "IpRuleItemTypeDef",
+    "CertificateBasedAuthPropertiesOutputTypeDef",
     "CertificateBasedAuthPropertiesTypeDef",
+    "ClientPropertiesOutputTypeDef",
     "ClientPropertiesTypeDef",
+    "ComputeTypeOutputTypeDef",
     "ComputeTypeTypeDef",
     "ConnectClientAddInTypeDef",
     "ConnectionAliasAssociationTypeDef",
+    "ConnectionAliasPermissionOutputTypeDef",
     "ConnectionAliasPermissionTypeDef",
     "TagTypeDef",
-    "CopyWorkspaceImageResultTypeDef",
     "CreateConnectClientAddInRequestRequestTypeDef",
-    "CreateConnectClientAddInResultTypeDef",
-    "CreateConnectionAliasResultTypeDef",
-    "CreateIpGroupResultTypeDef",
     "PendingCreateStandbyWorkspacesRequestTypeDef",
-    "CreateUpdatedWorkspaceImageResultTypeDef",
     "RootStorageTypeDef",
     "UserStorageTypeDef",
     "OperatingSystemTypeDef",
     "DefaultClientBrandingAttributesTypeDef",
     "DefaultImportClientBrandingAttributesTypeDef",
     "DefaultWorkspaceCreationPropertiesTypeDef",
     "DeleteClientBrandingRequestRequestTypeDef",
     "DeleteConnectClientAddInRequestRequestTypeDef",
     "DeleteConnectionAliasRequestRequestTypeDef",
     "DeleteIpGroupRequestRequestTypeDef",
     "DeleteTagsRequestRequestTypeDef",
     "DeleteWorkspaceBundleRequestRequestTypeDef",
     "DeleteWorkspaceImageRequestRequestTypeDef",
     "DeregisterWorkspaceDirectoryRequestRequestTypeDef",
-    "DescribeAccountModificationsRequestDescribeAccountModificationsPaginateTypeDef",
+    "PaginatorConfigTypeDef",
     "DescribeAccountModificationsRequestRequestTypeDef",
-    "DescribeAccountResultTypeDef",
     "DescribeClientBrandingRequestRequestTypeDef",
     "IosClientBrandingAttributesTypeDef",
     "DescribeClientPropertiesRequestRequestTypeDef",
     "DescribeConnectClientAddInsRequestRequestTypeDef",
     "DescribeConnectionAliasPermissionsRequestRequestTypeDef",
     "DescribeConnectionAliasesRequestRequestTypeDef",
-    "DescribeIpGroupsRequestDescribeIpGroupsPaginateTypeDef",
     "DescribeIpGroupsRequestRequestTypeDef",
     "DescribeTagsRequestRequestTypeDef",
-    "DescribeWorkspaceBundlesRequestDescribeWorkspaceBundlesPaginateTypeDef",
+    "TagOutputTypeDef",
     "DescribeWorkspaceBundlesRequestRequestTypeDef",
-    "DescribeWorkspaceDirectoriesRequestDescribeWorkspaceDirectoriesPaginateTypeDef",
     "DescribeWorkspaceDirectoriesRequestRequestTypeDef",
     "DescribeWorkspaceImagePermissionsRequestRequestTypeDef",
     "ImagePermissionTypeDef",
-    "DescribeWorkspaceImagesRequestDescribeWorkspaceImagesPaginateTypeDef",
     "DescribeWorkspaceImagesRequestRequestTypeDef",
     "DescribeWorkspaceSnapshotsRequestRequestTypeDef",
     "SnapshotTypeDef",
-    "DescribeWorkspacesConnectionStatusRequestDescribeWorkspacesConnectionStatusPaginateTypeDef",
     "DescribeWorkspacesConnectionStatusRequestRequestTypeDef",
     "WorkspaceConnectionStatusTypeDef",
-    "DescribeWorkspacesRequestDescribeWorkspacesPaginateTypeDef",
     "DescribeWorkspacesRequestRequestTypeDef",
     "DisassociateConnectionAliasRequestRequestTypeDef",
     "DisassociateIpGroupsRequestRequestTypeDef",
     "FailedWorkspaceChangeRequestTypeDef",
     "IosImportClientBrandingAttributesTypeDef",
-    "ImportWorkspaceImageResultTypeDef",
-    "ListAvailableManagementCidrRangesRequestListAvailableManagementCidrRangesPaginateTypeDef",
+    "IpRuleItemOutputTypeDef",
     "ListAvailableManagementCidrRangesRequestRequestTypeDef",
-    "ListAvailableManagementCidrRangesResultTypeDef",
     "MigrateWorkspaceRequestRequestTypeDef",
-    "MigrateWorkspaceResultTypeDef",
     "ModificationStateTypeDef",
     "ModifyAccountRequestRequestTypeDef",
     "SamlPropertiesTypeDef",
     "SelfservicePermissionsTypeDef",
     "WorkspaceAccessPropertiesTypeDef",
     "WorkspaceCreationPropertiesTypeDef",
     "WorkspacePropertiesTypeDef",
     "ModifyWorkspaceStateRequestRequestTypeDef",
-    "PaginatorConfigTypeDef",
     "RebootRequestTypeDef",
     "RebuildRequestTypeDef",
     "RelatedWorkspacePropertiesTypeDef",
-    "ResponseMetadataTypeDef",
     "RestoreWorkspaceRequestRequestTypeDef",
     "RevokeIpRulesRequestRequestTypeDef",
+    "RootStorageOutputTypeDef",
+    "SamlPropertiesOutputTypeDef",
+    "SelfservicePermissionsOutputTypeDef",
     "StartRequestTypeDef",
     "StopRequestTypeDef",
     "TerminateRequestTypeDef",
     "UpdateConnectClientAddInRequestRequestTypeDef",
     "UpdateResultTypeDef",
     "UpdateWorkspaceBundleRequestRequestTypeDef",
     "UpdateWorkspaceImagePermissionRequestRequestTypeDef",
+    "UserStorageOutputTypeDef",
+    "WorkspaceAccessPropertiesOutputTypeDef",
+    "WorkspacePropertiesOutputTypeDef",
+    "AssociateConnectionAliasResultTypeDef",
+    "CopyWorkspaceImageResultTypeDef",
+    "CreateConnectClientAddInResultTypeDef",
+    "CreateConnectionAliasResultTypeDef",
+    "CreateIpGroupResultTypeDef",
+    "CreateUpdatedWorkspaceImageResultTypeDef",
     "DescribeAccountModificationsResultTypeDef",
+    "DescribeAccountResultTypeDef",
+    "ImportWorkspaceImageResultTypeDef",
+    "ListAvailableManagementCidrRangesResultTypeDef",
+    "MigrateWorkspaceResultTypeDef",
     "AuthorizeIpRulesRequestRequestTypeDef",
     "UpdateRulesOfIpGroupRequestRequestTypeDef",
-    "WorkspacesIpGroupTypeDef",
     "ModifyCertificateBasedAuthPropertiesRequestRequestTypeDef",
     "ClientPropertiesResultTypeDef",
     "ModifyClientPropertiesRequestRequestTypeDef",
     "DescribeConnectClientAddInsResultTypeDef",
     "ConnectionAliasTypeDef",
     "DescribeConnectionAliasPermissionsResultTypeDef",
     "UpdateConnectionAliasPermissionRequestRequestTypeDef",
     "CopyWorkspaceImageRequestRequestTypeDef",
     "CreateConnectionAliasRequestRequestTypeDef",
     "CreateIpGroupRequestRequestTypeDef",
     "CreateTagsRequestRequestTypeDef",
     "CreateUpdatedWorkspaceImageRequestRequestTypeDef",
     "CreateWorkspaceImageRequestRequestTypeDef",
-    "DescribeTagsResultTypeDef",
     "ImportWorkspaceImageRequestRequestTypeDef",
     "RegisterWorkspaceDirectoryRequestRequestTypeDef",
     "StandbyWorkspaceTypeDef",
     "CreateWorkspaceBundleRequestRequestTypeDef",
-    "WorkspaceBundleTypeDef",
     "CreateWorkspaceImageResultTypeDef",
+    "DescribeAccountModificationsRequestDescribeAccountModificationsPaginateTypeDef",
+    "DescribeIpGroupsRequestDescribeIpGroupsPaginateTypeDef",
+    "DescribeWorkspaceBundlesRequestDescribeWorkspaceBundlesPaginateTypeDef",
+    "DescribeWorkspaceDirectoriesRequestDescribeWorkspaceDirectoriesPaginateTypeDef",
+    "DescribeWorkspaceImagesRequestDescribeWorkspaceImagesPaginateTypeDef",
+    "DescribeWorkspacesConnectionStatusRequestDescribeWorkspacesConnectionStatusPaginateTypeDef",
+    "DescribeWorkspacesRequestDescribeWorkspacesPaginateTypeDef",
+    "ListAvailableManagementCidrRangesRequestListAvailableManagementCidrRangesPaginateTypeDef",
     "DescribeClientBrandingResultTypeDef",
     "ImportClientBrandingResultTypeDef",
+    "DescribeTagsResultTypeDef",
+    "StandbyWorkspaceOutputTypeDef",
     "DescribeWorkspaceImagePermissionsResultTypeDef",
     "DescribeWorkspaceSnapshotsResultTypeDef",
     "DescribeWorkspacesConnectionStatusResultTypeDef",
     "RebootWorkspacesResultTypeDef",
     "RebuildWorkspacesResultTypeDef",
     "StartWorkspacesResultTypeDef",
     "StopWorkspacesResultTypeDef",
     "TerminateWorkspacesResultTypeDef",
     "ImportClientBrandingRequestRequestTypeDef",
+    "WorkspacesIpGroupTypeDef",
     "ModifySamlPropertiesRequestRequestTypeDef",
     "ModifySelfservicePermissionsRequestRequestTypeDef",
     "ModifyWorkspaceAccessPropertiesRequestRequestTypeDef",
-    "WorkspaceDirectoryTypeDef",
     "ModifyWorkspaceCreationPropertiesRequestRequestTypeDef",
     "ModifyWorkspacePropertiesRequestRequestTypeDef",
     "WorkspaceRequestTypeDef",
     "RebootWorkspacesRequestRequestTypeDef",
     "RebuildWorkspacesRequestRequestTypeDef",
-    "WorkspaceTypeDef",
     "StartWorkspacesRequestRequestTypeDef",
     "StopWorkspacesRequestRequestTypeDef",
     "TerminateWorkspacesRequestRequestTypeDef",
     "WorkspaceImageTypeDef",
-    "DescribeIpGroupsResultTypeDef",
+    "WorkspaceBundleTypeDef",
+    "WorkspaceDirectoryTypeDef",
+    "WorkspaceRequestOutputTypeDef",
+    "WorkspaceTypeDef",
     "DescribeClientPropertiesResultTypeDef",
     "DescribeConnectionAliasesResultTypeDef",
     "CreateStandbyWorkspacesRequestRequestTypeDef",
     "FailedCreateStandbyWorkspacesRequestTypeDef",
+    "DescribeIpGroupsResultTypeDef",
+    "CreateWorkspacesRequestRequestTypeDef",
+    "DescribeWorkspaceImagesResultTypeDef",
     "CreateWorkspaceBundleResultTypeDef",
     "DescribeWorkspaceBundlesResultTypeDef",
     "DescribeWorkspaceDirectoriesResultTypeDef",
-    "CreateWorkspacesRequestRequestTypeDef",
     "FailedCreateWorkspaceRequestTypeDef",
     "DescribeWorkspacesResultTypeDef",
-    "DescribeWorkspaceImagesResultTypeDef",
     "CreateStandbyWorkspacesResultTypeDef",
     "CreateWorkspacesResultTypeDef",
 )
 
 AccountModificationTypeDef = TypedDict(
     "AccountModificationTypeDef",
     {
         "ModificationState": DedicatedTenancyModificationStateEnumType,
         "DedicatedTenancySupport": DedicatedTenancySupportResultEnumType,
         "DedicatedTenancyManagementCidrRange": str,
         "StartTime": datetime,
         "ErrorCode": str,
         "ErrorMessage": str,
     },
-    total=False,
 )
 
 AssociateConnectionAliasRequestRequestTypeDef = TypedDict(
     "AssociateConnectionAliasRequestRequestTypeDef",
     {
         "AliasId": str,
         "ResourceId": str,
     },
 )
 
-AssociateConnectionAliasResultTypeDef = TypedDict(
-    "AssociateConnectionAliasResultTypeDef",
+ResponseMetadataTypeDef = TypedDict(
+    "ResponseMetadataTypeDef",
     {
-        "ConnectionIdentifier": str,
-        "ResponseMetadata": "ResponseMetadataTypeDef",
+        "RequestId": str,
+        "HostId": str,
+        "HTTPStatusCode": int,
+        "HTTPHeaders": Dict[str, str],
+        "RetryAttempts": int,
     },
 )
 
 AssociateIpGroupsRequestRequestTypeDef = TypedDict(
     "AssociateIpGroupsRequestRequestTypeDef",
     {
         "DirectoryId": str,
@@ -261,32 +277,55 @@
     {
         "ipRule": str,
         "ruleDesc": str,
     },
     total=False,
 )
 
+CertificateBasedAuthPropertiesOutputTypeDef = TypedDict(
+    "CertificateBasedAuthPropertiesOutputTypeDef",
+    {
+        "Status": CertificateBasedAuthStatusEnumType,
+        "CertificateAuthorityArn": str,
+    },
+)
+
 CertificateBasedAuthPropertiesTypeDef = TypedDict(
     "CertificateBasedAuthPropertiesTypeDef",
     {
         "Status": CertificateBasedAuthStatusEnumType,
         "CertificateAuthorityArn": str,
     },
     total=False,
 )
 
+ClientPropertiesOutputTypeDef = TypedDict(
+    "ClientPropertiesOutputTypeDef",
+    {
+        "ReconnectEnabled": ReconnectEnumType,
+        "LogUploadEnabled": LogUploadEnumType,
+    },
+)
+
 ClientPropertiesTypeDef = TypedDict(
     "ClientPropertiesTypeDef",
     {
         "ReconnectEnabled": ReconnectEnumType,
         "LogUploadEnabled": LogUploadEnumType,
     },
     total=False,
 )
 
+ComputeTypeOutputTypeDef = TypedDict(
+    "ComputeTypeOutputTypeDef",
+    {
+        "Name": ComputeType,
+    },
+)
+
 ComputeTypeTypeDef = TypedDict(
     "ComputeTypeTypeDef",
     {
         "Name": ComputeType,
     },
     total=False,
 )
@@ -295,26 +334,32 @@
     "ConnectClientAddInTypeDef",
     {
         "AddInId": str,
         "ResourceId": str,
         "Name": str,
         "URL": str,
     },
-    total=False,
 )
 
 ConnectionAliasAssociationTypeDef = TypedDict(
     "ConnectionAliasAssociationTypeDef",
     {
         "AssociationStatus": AssociationStatusType,
         "AssociatedAccountId": str,
         "ResourceId": str,
         "ConnectionIdentifier": str,
     },
-    total=False,
+)
+
+ConnectionAliasPermissionOutputTypeDef = TypedDict(
+    "ConnectionAliasPermissionOutputTypeDef",
+    {
+        "SharedAccountId": str,
+        "AllowAssociation": bool,
+    },
 )
 
 ConnectionAliasPermissionTypeDef = TypedDict(
     "ConnectionAliasPermissionTypeDef",
     {
         "SharedAccountId": str,
         "AllowAssociation": bool,
@@ -336,72 +381,31 @@
 )
 
 
 class TagTypeDef(_RequiredTagTypeDef, _OptionalTagTypeDef):
     pass
 
 
-CopyWorkspaceImageResultTypeDef = TypedDict(
-    "CopyWorkspaceImageResultTypeDef",
-    {
-        "ImageId": str,
-        "ResponseMetadata": "ResponseMetadataTypeDef",
-    },
-)
-
 CreateConnectClientAddInRequestRequestTypeDef = TypedDict(
     "CreateConnectClientAddInRequestRequestTypeDef",
     {
         "ResourceId": str,
         "Name": str,
         "URL": str,
     },
 )
 
-CreateConnectClientAddInResultTypeDef = TypedDict(
-    "CreateConnectClientAddInResultTypeDef",
-    {
-        "AddInId": str,
-        "ResponseMetadata": "ResponseMetadataTypeDef",
-    },
-)
-
-CreateConnectionAliasResultTypeDef = TypedDict(
-    "CreateConnectionAliasResultTypeDef",
-    {
-        "AliasId": str,
-        "ResponseMetadata": "ResponseMetadataTypeDef",
-    },
-)
-
-CreateIpGroupResultTypeDef = TypedDict(
-    "CreateIpGroupResultTypeDef",
-    {
-        "GroupId": str,
-        "ResponseMetadata": "ResponseMetadataTypeDef",
-    },
-)
-
 PendingCreateStandbyWorkspacesRequestTypeDef = TypedDict(
     "PendingCreateStandbyWorkspacesRequestTypeDef",
     {
         "UserName": str,
         "DirectoryId": str,
         "State": WorkspaceStateType,
         "WorkspaceId": str,
     },
-    total=False,
-)
-
-CreateUpdatedWorkspaceImageResultTypeDef = TypedDict(
-    "CreateUpdatedWorkspaceImageResultTypeDef",
-    {
-        "ImageId": str,
-        "ResponseMetadata": "ResponseMetadataTypeDef",
-    },
 )
 
 RootStorageTypeDef = TypedDict(
     "RootStorageTypeDef",
     {
         "Capacity": str,
     },
@@ -417,27 +421,25 @@
 )
 
 OperatingSystemTypeDef = TypedDict(
     "OperatingSystemTypeDef",
     {
         "Type": OperatingSystemTypeType,
     },
-    total=False,
 )
 
 DefaultClientBrandingAttributesTypeDef = TypedDict(
     "DefaultClientBrandingAttributesTypeDef",
     {
         "LogoUrl": str,
         "SupportEmail": str,
         "SupportLink": str,
         "ForgotPasswordLink": str,
         "LoginMessage": Dict[str, str],
     },
-    total=False,
 )
 
 DefaultImportClientBrandingAttributesTypeDef = TypedDict(
     "DefaultImportClientBrandingAttributesTypeDef",
     {
         "Logo": Union[str, bytes, IO[Any], StreamingBody],
         "SupportEmail": str,
@@ -454,15 +456,14 @@
         "EnableWorkDocs": bool,
         "EnableInternetAccess": bool,
         "DefaultOu": str,
         "CustomSecurityGroupId": str,
         "UserEnabledAsLocalAdministrator": bool,
         "EnableMaintenanceMode": bool,
     },
-    total=False,
 )
 
 DeleteClientBrandingRequestRequestTypeDef = TypedDict(
     "DeleteClientBrandingRequestRequestTypeDef",
     {
         "ResourceId": str,
         "Platforms": Sequence[ClientDeviceTypeType],
@@ -517,39 +518,32 @@
 DeregisterWorkspaceDirectoryRequestRequestTypeDef = TypedDict(
     "DeregisterWorkspaceDirectoryRequestRequestTypeDef",
     {
         "DirectoryId": str,
     },
 )
 
-DescribeAccountModificationsRequestDescribeAccountModificationsPaginateTypeDef = TypedDict(
-    "DescribeAccountModificationsRequestDescribeAccountModificationsPaginateTypeDef",
+PaginatorConfigTypeDef = TypedDict(
+    "PaginatorConfigTypeDef",
     {
-        "PaginationConfig": "PaginatorConfigTypeDef",
+        "MaxItems": int,
+        "PageSize": int,
+        "StartingToken": str,
     },
     total=False,
 )
 
 DescribeAccountModificationsRequestRequestTypeDef = TypedDict(
     "DescribeAccountModificationsRequestRequestTypeDef",
     {
         "NextToken": str,
     },
     total=False,
 )
 
-DescribeAccountResultTypeDef = TypedDict(
-    "DescribeAccountResultTypeDef",
-    {
-        "DedicatedTenancySupport": DedicatedTenancySupportResultEnumType,
-        "DedicatedTenancyManagementCidrRange": str,
-        "ResponseMetadata": "ResponseMetadataTypeDef",
-    },
-)
-
 DescribeClientBrandingRequestRequestTypeDef = TypedDict(
     "DescribeClientBrandingRequestRequestTypeDef",
     {
         "ResourceId": str,
     },
 )
 
@@ -560,15 +554,14 @@
         "Logo2xUrl": str,
         "Logo3xUrl": str,
         "SupportEmail": str,
         "SupportLink": str,
         "ForgotPasswordLink": str,
         "LoginMessage": Dict[str, str],
     },
-    total=False,
 )
 
 DescribeClientPropertiesRequestRequestTypeDef = TypedDict(
     "DescribeClientPropertiesRequestRequestTypeDef",
     {
         "ResourceIds": Sequence[str],
     },
@@ -627,23 +620,14 @@
         "ResourceId": str,
         "Limit": int,
         "NextToken": str,
     },
     total=False,
 )
 
-DescribeIpGroupsRequestDescribeIpGroupsPaginateTypeDef = TypedDict(
-    "DescribeIpGroupsRequestDescribeIpGroupsPaginateTypeDef",
-    {
-        "GroupIds": Sequence[str],
-        "PaginationConfig": "PaginatorConfigTypeDef",
-    },
-    total=False,
-)
-
 DescribeIpGroupsRequestRequestTypeDef = TypedDict(
     "DescribeIpGroupsRequestRequestTypeDef",
     {
         "GroupIds": Sequence[str],
         "NextToken": str,
         "MaxResults": int,
     },
@@ -653,44 +637,32 @@
 DescribeTagsRequestRequestTypeDef = TypedDict(
     "DescribeTagsRequestRequestTypeDef",
     {
         "ResourceId": str,
     },
 )
 
-DescribeWorkspaceBundlesRequestDescribeWorkspaceBundlesPaginateTypeDef = TypedDict(
-    "DescribeWorkspaceBundlesRequestDescribeWorkspaceBundlesPaginateTypeDef",
+TagOutputTypeDef = TypedDict(
+    "TagOutputTypeDef",
     {
-        "BundleIds": Sequence[str],
-        "Owner": str,
-        "PaginationConfig": "PaginatorConfigTypeDef",
+        "Key": str,
+        "Value": str,
     },
-    total=False,
 )
 
 DescribeWorkspaceBundlesRequestRequestTypeDef = TypedDict(
     "DescribeWorkspaceBundlesRequestRequestTypeDef",
     {
         "BundleIds": Sequence[str],
         "Owner": str,
         "NextToken": str,
     },
     total=False,
 )
 
-DescribeWorkspaceDirectoriesRequestDescribeWorkspaceDirectoriesPaginateTypeDef = TypedDict(
-    "DescribeWorkspaceDirectoriesRequestDescribeWorkspaceDirectoriesPaginateTypeDef",
-    {
-        "DirectoryIds": Sequence[str],
-        "Limit": int,
-        "PaginationConfig": "PaginatorConfigTypeDef",
-    },
-    total=False,
-)
-
 DescribeWorkspaceDirectoriesRequestRequestTypeDef = TypedDict(
     "DescribeWorkspaceDirectoriesRequestRequestTypeDef",
     {
         "DirectoryIds": Sequence[str],
         "Limit": int,
         "NextToken": str,
     },
@@ -721,25 +693,14 @@
 
 
 ImagePermissionTypeDef = TypedDict(
     "ImagePermissionTypeDef",
     {
         "SharedAccountId": str,
     },
-    total=False,
-)
-
-DescribeWorkspaceImagesRequestDescribeWorkspaceImagesPaginateTypeDef = TypedDict(
-    "DescribeWorkspaceImagesRequestDescribeWorkspaceImagesPaginateTypeDef",
-    {
-        "ImageIds": Sequence[str],
-        "ImageType": ImageTypeType,
-        "PaginationConfig": "PaginatorConfigTypeDef",
-    },
-    total=False,
 )
 
 DescribeWorkspaceImagesRequestRequestTypeDef = TypedDict(
     "DescribeWorkspaceImagesRequestRequestTypeDef",
     {
         "ImageIds": Sequence[str],
         "ImageType": ImageTypeType,
@@ -757,24 +718,14 @@
 )
 
 SnapshotTypeDef = TypedDict(
     "SnapshotTypeDef",
     {
         "SnapshotTime": datetime,
     },
-    total=False,
-)
-
-DescribeWorkspacesConnectionStatusRequestDescribeWorkspacesConnectionStatusPaginateTypeDef = TypedDict(
-    "DescribeWorkspacesConnectionStatusRequestDescribeWorkspacesConnectionStatusPaginateTypeDef",
-    {
-        "WorkspaceIds": Sequence[str],
-        "PaginationConfig": "PaginatorConfigTypeDef",
-    },
-    total=False,
 )
 
 DescribeWorkspacesConnectionStatusRequestRequestTypeDef = TypedDict(
     "DescribeWorkspacesConnectionStatusRequestRequestTypeDef",
     {
         "WorkspaceIds": Sequence[str],
         "NextToken": str,
@@ -786,27 +737,14 @@
     "WorkspaceConnectionStatusTypeDef",
     {
         "WorkspaceId": str,
         "ConnectionState": ConnectionStateType,
         "ConnectionStateCheckTimestamp": datetime,
         "LastKnownUserConnectionTimestamp": datetime,
     },
-    total=False,
-)
-
-DescribeWorkspacesRequestDescribeWorkspacesPaginateTypeDef = TypedDict(
-    "DescribeWorkspacesRequestDescribeWorkspacesPaginateTypeDef",
-    {
-        "WorkspaceIds": Sequence[str],
-        "DirectoryId": str,
-        "UserName": str,
-        "BundleId": str,
-        "PaginationConfig": "PaginatorConfigTypeDef",
-    },
-    total=False,
 )
 
 DescribeWorkspacesRequestRequestTypeDef = TypedDict(
     "DescribeWorkspacesRequestRequestTypeDef",
     {
         "WorkspaceIds": Sequence[str],
         "DirectoryId": str,
@@ -836,15 +774,14 @@
 FailedWorkspaceChangeRequestTypeDef = TypedDict(
     "FailedWorkspaceChangeRequestTypeDef",
     {
         "WorkspaceId": str,
         "ErrorCode": str,
         "ErrorMessage": str,
     },
-    total=False,
 )
 
 IosImportClientBrandingAttributesTypeDef = TypedDict(
     "IosImportClientBrandingAttributesTypeDef",
     {
         "Logo": Union[str, bytes, IO[Any], StreamingBody],
         "Logo2x": Union[str, bytes, IO[Any], StreamingBody],
@@ -853,44 +790,22 @@
         "SupportLink": str,
         "ForgotPasswordLink": str,
         "LoginMessage": Mapping[str, str],
     },
     total=False,
 )
 
-ImportWorkspaceImageResultTypeDef = TypedDict(
-    "ImportWorkspaceImageResultTypeDef",
-    {
-        "ImageId": str,
-        "ResponseMetadata": "ResponseMetadataTypeDef",
-    },
-)
-
-_RequiredListAvailableManagementCidrRangesRequestListAvailableManagementCidrRangesPaginateTypeDef = TypedDict(
-    "_RequiredListAvailableManagementCidrRangesRequestListAvailableManagementCidrRangesPaginateTypeDef",
-    {
-        "ManagementCidrRangeConstraint": str,
-    },
-)
-_OptionalListAvailableManagementCidrRangesRequestListAvailableManagementCidrRangesPaginateTypeDef = TypedDict(
-    "_OptionalListAvailableManagementCidrRangesRequestListAvailableManagementCidrRangesPaginateTypeDef",
+IpRuleItemOutputTypeDef = TypedDict(
+    "IpRuleItemOutputTypeDef",
     {
-        "PaginationConfig": "PaginatorConfigTypeDef",
+        "ipRule": str,
+        "ruleDesc": str,
     },
-    total=False,
 )
 
-
-class ListAvailableManagementCidrRangesRequestListAvailableManagementCidrRangesPaginateTypeDef(
-    _RequiredListAvailableManagementCidrRangesRequestListAvailableManagementCidrRangesPaginateTypeDef,
-    _OptionalListAvailableManagementCidrRangesRequestListAvailableManagementCidrRangesPaginateTypeDef,
-):
-    pass
-
-
 _RequiredListAvailableManagementCidrRangesRequestRequestTypeDef = TypedDict(
     "_RequiredListAvailableManagementCidrRangesRequestRequestTypeDef",
     {
         "ManagementCidrRangeConstraint": str,
     },
 )
 _OptionalListAvailableManagementCidrRangesRequestRequestTypeDef = TypedDict(
@@ -906,47 +821,28 @@
 class ListAvailableManagementCidrRangesRequestRequestTypeDef(
     _RequiredListAvailableManagementCidrRangesRequestRequestTypeDef,
     _OptionalListAvailableManagementCidrRangesRequestRequestTypeDef,
 ):
     pass
 
 
-ListAvailableManagementCidrRangesResultTypeDef = TypedDict(
-    "ListAvailableManagementCidrRangesResultTypeDef",
-    {
-        "ManagementCidrRanges": List[str],
-        "NextToken": str,
-        "ResponseMetadata": "ResponseMetadataTypeDef",
-    },
-)
-
 MigrateWorkspaceRequestRequestTypeDef = TypedDict(
     "MigrateWorkspaceRequestRequestTypeDef",
     {
         "SourceWorkspaceId": str,
         "BundleId": str,
     },
 )
 
-MigrateWorkspaceResultTypeDef = TypedDict(
-    "MigrateWorkspaceResultTypeDef",
-    {
-        "SourceWorkspaceId": str,
-        "TargetWorkspaceId": str,
-        "ResponseMetadata": "ResponseMetadataTypeDef",
-    },
-)
-
 ModificationStateTypeDef = TypedDict(
     "ModificationStateTypeDef",
     {
         "Resource": ModificationResourceEnumType,
         "State": ModificationStateEnumType,
     },
-    total=False,
 )
 
 ModifyAccountRequestRequestTypeDef = TypedDict(
     "ModifyAccountRequestRequestTypeDef",
     {
         "DedicatedTenancySupport": Literal["ENABLED"],
         "DedicatedTenancyManagementCidrRange": str,
@@ -1021,24 +917,14 @@
     "ModifyWorkspaceStateRequestRequestTypeDef",
     {
         "WorkspaceId": str,
         "WorkspaceState": TargetWorkspaceStateType,
     },
 )
 
-PaginatorConfigTypeDef = TypedDict(
-    "PaginatorConfigTypeDef",
-    {
-        "MaxItems": int,
-        "PageSize": int,
-        "StartingToken": str,
-    },
-    total=False,
-)
-
 RebootRequestTypeDef = TypedDict(
     "RebootRequestTypeDef",
     {
         "WorkspaceId": str,
     },
 )
 
@@ -1053,26 +939,14 @@
     "RelatedWorkspacePropertiesTypeDef",
     {
         "WorkspaceId": str,
         "Region": str,
         "State": WorkspaceStateType,
         "Type": StandbyWorkspaceRelationshipTypeType,
     },
-    total=False,
-)
-
-ResponseMetadataTypeDef = TypedDict(
-    "ResponseMetadataTypeDef",
-    {
-        "RequestId": str,
-        "HostId": str,
-        "HTTPStatusCode": int,
-        "HTTPHeaders": Dict[str, str],
-        "RetryAttempts": int,
-    },
 )
 
 RestoreWorkspaceRequestRequestTypeDef = TypedDict(
     "RestoreWorkspaceRequestRequestTypeDef",
     {
         "WorkspaceId": str,
     },
@@ -1082,14 +956,41 @@
     "RevokeIpRulesRequestRequestTypeDef",
     {
         "GroupId": str,
         "UserRules": Sequence[str],
     },
 )
 
+RootStorageOutputTypeDef = TypedDict(
+    "RootStorageOutputTypeDef",
+    {
+        "Capacity": str,
+    },
+)
+
+SamlPropertiesOutputTypeDef = TypedDict(
+    "SamlPropertiesOutputTypeDef",
+    {
+        "Status": SamlStatusEnumType,
+        "UserAccessUrl": str,
+        "RelayStateParameterName": str,
+    },
+)
+
+SelfservicePermissionsOutputTypeDef = TypedDict(
+    "SelfservicePermissionsOutputTypeDef",
+    {
+        "RestartWorkspace": ReconnectEnumType,
+        "IncreaseVolumeSize": ReconnectEnumType,
+        "ChangeComputeType": ReconnectEnumType,
+        "SwitchRunningMode": ReconnectEnumType,
+        "RebuildWorkspace": ReconnectEnumType,
+    },
+)
+
 StartRequestTypeDef = TypedDict(
     "StartRequestTypeDef",
     {
         "WorkspaceId": str,
     },
     total=False,
 )
@@ -1135,15 +1036,14 @@
 
 UpdateResultTypeDef = TypedDict(
     "UpdateResultTypeDef",
     {
         "UpdateAvailable": bool,
         "Description": str,
     },
-    total=False,
 )
 
 UpdateWorkspaceBundleRequestRequestTypeDef = TypedDict(
     "UpdateWorkspaceBundleRequestRequestTypeDef",
     {
         "BundleId": str,
         "ImageId": str,
@@ -1156,20 +1056,136 @@
     {
         "ImageId": str,
         "AllowCopyImage": bool,
         "SharedAccountId": str,
     },
 )
 
+UserStorageOutputTypeDef = TypedDict(
+    "UserStorageOutputTypeDef",
+    {
+        "Capacity": str,
+    },
+)
+
+WorkspaceAccessPropertiesOutputTypeDef = TypedDict(
+    "WorkspaceAccessPropertiesOutputTypeDef",
+    {
+        "DeviceTypeWindows": AccessPropertyValueType,
+        "DeviceTypeOsx": AccessPropertyValueType,
+        "DeviceTypeWeb": AccessPropertyValueType,
+        "DeviceTypeIos": AccessPropertyValueType,
+        "DeviceTypeAndroid": AccessPropertyValueType,
+        "DeviceTypeChromeOs": AccessPropertyValueType,
+        "DeviceTypeZeroClient": AccessPropertyValueType,
+        "DeviceTypeLinux": AccessPropertyValueType,
+    },
+)
+
+WorkspacePropertiesOutputTypeDef = TypedDict(
+    "WorkspacePropertiesOutputTypeDef",
+    {
+        "RunningMode": RunningModeType,
+        "RunningModeAutoStopTimeoutInMinutes": int,
+        "RootVolumeSizeGib": int,
+        "UserVolumeSizeGib": int,
+        "ComputeTypeName": ComputeType,
+        "Protocols": List[ProtocolType],
+    },
+)
+
+AssociateConnectionAliasResultTypeDef = TypedDict(
+    "AssociateConnectionAliasResultTypeDef",
+    {
+        "ConnectionIdentifier": str,
+        "ResponseMetadata": ResponseMetadataTypeDef,
+    },
+)
+
+CopyWorkspaceImageResultTypeDef = TypedDict(
+    "CopyWorkspaceImageResultTypeDef",
+    {
+        "ImageId": str,
+        "ResponseMetadata": ResponseMetadataTypeDef,
+    },
+)
+
+CreateConnectClientAddInResultTypeDef = TypedDict(
+    "CreateConnectClientAddInResultTypeDef",
+    {
+        "AddInId": str,
+        "ResponseMetadata": ResponseMetadataTypeDef,
+    },
+)
+
+CreateConnectionAliasResultTypeDef = TypedDict(
+    "CreateConnectionAliasResultTypeDef",
+    {
+        "AliasId": str,
+        "ResponseMetadata": ResponseMetadataTypeDef,
+    },
+)
+
+CreateIpGroupResultTypeDef = TypedDict(
+    "CreateIpGroupResultTypeDef",
+    {
+        "GroupId": str,
+        "ResponseMetadata": ResponseMetadataTypeDef,
+    },
+)
+
+CreateUpdatedWorkspaceImageResultTypeDef = TypedDict(
+    "CreateUpdatedWorkspaceImageResultTypeDef",
+    {
+        "ImageId": str,
+        "ResponseMetadata": ResponseMetadataTypeDef,
+    },
+)
+
 DescribeAccountModificationsResultTypeDef = TypedDict(
     "DescribeAccountModificationsResultTypeDef",
     {
         "AccountModifications": List[AccountModificationTypeDef],
         "NextToken": str,
-        "ResponseMetadata": "ResponseMetadataTypeDef",
+        "ResponseMetadata": ResponseMetadataTypeDef,
+    },
+)
+
+DescribeAccountResultTypeDef = TypedDict(
+    "DescribeAccountResultTypeDef",
+    {
+        "DedicatedTenancySupport": DedicatedTenancySupportResultEnumType,
+        "DedicatedTenancyManagementCidrRange": str,
+        "ResponseMetadata": ResponseMetadataTypeDef,
+    },
+)
+
+ImportWorkspaceImageResultTypeDef = TypedDict(
+    "ImportWorkspaceImageResultTypeDef",
+    {
+        "ImageId": str,
+        "ResponseMetadata": ResponseMetadataTypeDef,
+    },
+)
+
+ListAvailableManagementCidrRangesResultTypeDef = TypedDict(
+    "ListAvailableManagementCidrRangesResultTypeDef",
+    {
+        "ManagementCidrRanges": List[str],
+        "NextToken": str,
+        "ResponseMetadata": ResponseMetadataTypeDef,
+    },
+)
+
+MigrateWorkspaceResultTypeDef = TypedDict(
+    "MigrateWorkspaceResultTypeDef",
+    {
+        "SourceWorkspaceId": str,
+        "TargetWorkspaceId": str,
+        "ResponseMetadata": ResponseMetadataTypeDef,
     },
 )
 
 AuthorizeIpRulesRequestRequestTypeDef = TypedDict(
     "AuthorizeIpRulesRequestRequestTypeDef",
     {
         "GroupId": str,
@@ -1181,25 +1197,14 @@
     "UpdateRulesOfIpGroupRequestRequestTypeDef",
     {
         "GroupId": str,
         "UserRules": Sequence[IpRuleItemTypeDef],
     },
 )
 
-WorkspacesIpGroupTypeDef = TypedDict(
-    "WorkspacesIpGroupTypeDef",
-    {
-        "groupId": str,
-        "groupName": str,
-        "groupDesc": str,
-        "userRules": List[IpRuleItemTypeDef],
-    },
-    total=False,
-)
-
 _RequiredModifyCertificateBasedAuthPropertiesRequestRequestTypeDef = TypedDict(
     "_RequiredModifyCertificateBasedAuthPropertiesRequestRequestTypeDef",
     {
         "ResourceId": str,
     },
 )
 _OptionalModifyCertificateBasedAuthPropertiesRequestRequestTypeDef = TypedDict(
@@ -1221,17 +1226,16 @@
     pass
 
 
 ClientPropertiesResultTypeDef = TypedDict(
     "ClientPropertiesResultTypeDef",
     {
         "ResourceId": str,
-        "ClientProperties": ClientPropertiesTypeDef,
+        "ClientProperties": ClientPropertiesOutputTypeDef,
     },
-    total=False,
 )
 
 ModifyClientPropertiesRequestRequestTypeDef = TypedDict(
     "ModifyClientPropertiesRequestRequestTypeDef",
     {
         "ResourceId": str,
         "ClientProperties": ClientPropertiesTypeDef,
@@ -1239,37 +1243,36 @@
 )
 
 DescribeConnectClientAddInsResultTypeDef = TypedDict(
     "DescribeConnectClientAddInsResultTypeDef",
     {
         "AddIns": List[ConnectClientAddInTypeDef],
         "NextToken": str,
-        "ResponseMetadata": "ResponseMetadataTypeDef",
+        "ResponseMetadata": ResponseMetadataTypeDef,
     },
 )
 
 ConnectionAliasTypeDef = TypedDict(
     "ConnectionAliasTypeDef",
     {
         "ConnectionString": str,
         "AliasId": str,
         "State": ConnectionAliasStateType,
         "OwnerAccountId": str,
         "Associations": List[ConnectionAliasAssociationTypeDef],
     },
-    total=False,
 )
 
 DescribeConnectionAliasPermissionsResultTypeDef = TypedDict(
     "DescribeConnectionAliasPermissionsResultTypeDef",
     {
         "AliasId": str,
-        "ConnectionAliasPermissions": List[ConnectionAliasPermissionTypeDef],
+        "ConnectionAliasPermissions": List[ConnectionAliasPermissionOutputTypeDef],
         "NextToken": str,
-        "ResponseMetadata": "ResponseMetadataTypeDef",
+        "ResponseMetadata": ResponseMetadataTypeDef,
     },
 )
 
 UpdateConnectionAliasPermissionRequestRequestTypeDef = TypedDict(
     "UpdateConnectionAliasPermissionRequestRequestTypeDef",
     {
         "AliasId": str,
@@ -1399,22 +1402,14 @@
 class CreateWorkspaceImageRequestRequestTypeDef(
     _RequiredCreateWorkspaceImageRequestRequestTypeDef,
     _OptionalCreateWorkspaceImageRequestRequestTypeDef,
 ):
     pass
 
 
-DescribeTagsResultTypeDef = TypedDict(
-    "DescribeTagsResultTypeDef",
-    {
-        "TagList": List[TagTypeDef],
-        "ResponseMetadata": "ResponseMetadataTypeDef",
-    },
-)
-
 _RequiredImportWorkspaceImageRequestRequestTypeDef = TypedDict(
     "_RequiredImportWorkspaceImageRequestRequestTypeDef",
     {
         "Ec2ImageId": str,
         "IngestionProcess": WorkspaceImageIngestionProcessType,
         "ImageName": str,
         "ImageDescription": str,
@@ -1507,139 +1502,228 @@
 class CreateWorkspaceBundleRequestRequestTypeDef(
     _RequiredCreateWorkspaceBundleRequestRequestTypeDef,
     _OptionalCreateWorkspaceBundleRequestRequestTypeDef,
 ):
     pass
 
 
-WorkspaceBundleTypeDef = TypedDict(
-    "WorkspaceBundleTypeDef",
-    {
-        "BundleId": str,
-        "Name": str,
-        "Owner": str,
-        "Description": str,
-        "ImageId": str,
-        "RootStorage": RootStorageTypeDef,
-        "UserStorage": UserStorageTypeDef,
-        "ComputeType": ComputeTypeTypeDef,
-        "LastUpdatedTime": datetime,
-        "CreationTime": datetime,
-        "State": WorkspaceBundleStateType,
-        "BundleType": BundleTypeType,
-    },
-    total=False,
-)
-
 CreateWorkspaceImageResultTypeDef = TypedDict(
     "CreateWorkspaceImageResultTypeDef",
     {
         "ImageId": str,
         "Name": str,
         "Description": str,
         "OperatingSystem": OperatingSystemTypeDef,
         "State": WorkspaceImageStateType,
         "RequiredTenancy": WorkspaceImageRequiredTenancyType,
         "Created": datetime,
         "OwnerAccountId": str,
-        "ResponseMetadata": "ResponseMetadataTypeDef",
+        "ResponseMetadata": ResponseMetadataTypeDef,
+    },
+)
+
+DescribeAccountModificationsRequestDescribeAccountModificationsPaginateTypeDef = TypedDict(
+    "DescribeAccountModificationsRequestDescribeAccountModificationsPaginateTypeDef",
+    {
+        "PaginationConfig": PaginatorConfigTypeDef,
+    },
+    total=False,
+)
+
+DescribeIpGroupsRequestDescribeIpGroupsPaginateTypeDef = TypedDict(
+    "DescribeIpGroupsRequestDescribeIpGroupsPaginateTypeDef",
+    {
+        "GroupIds": Sequence[str],
+        "PaginationConfig": PaginatorConfigTypeDef,
+    },
+    total=False,
+)
+
+DescribeWorkspaceBundlesRequestDescribeWorkspaceBundlesPaginateTypeDef = TypedDict(
+    "DescribeWorkspaceBundlesRequestDescribeWorkspaceBundlesPaginateTypeDef",
+    {
+        "BundleIds": Sequence[str],
+        "Owner": str,
+        "PaginationConfig": PaginatorConfigTypeDef,
+    },
+    total=False,
+)
+
+DescribeWorkspaceDirectoriesRequestDescribeWorkspaceDirectoriesPaginateTypeDef = TypedDict(
+    "DescribeWorkspaceDirectoriesRequestDescribeWorkspaceDirectoriesPaginateTypeDef",
+    {
+        "DirectoryIds": Sequence[str],
+        "Limit": int,
+        "PaginationConfig": PaginatorConfigTypeDef,
+    },
+    total=False,
+)
+
+DescribeWorkspaceImagesRequestDescribeWorkspaceImagesPaginateTypeDef = TypedDict(
+    "DescribeWorkspaceImagesRequestDescribeWorkspaceImagesPaginateTypeDef",
+    {
+        "ImageIds": Sequence[str],
+        "ImageType": ImageTypeType,
+        "PaginationConfig": PaginatorConfigTypeDef,
+    },
+    total=False,
+)
+
+DescribeWorkspacesConnectionStatusRequestDescribeWorkspacesConnectionStatusPaginateTypeDef = TypedDict(
+    "DescribeWorkspacesConnectionStatusRequestDescribeWorkspacesConnectionStatusPaginateTypeDef",
+    {
+        "WorkspaceIds": Sequence[str],
+        "PaginationConfig": PaginatorConfigTypeDef,
+    },
+    total=False,
+)
+
+DescribeWorkspacesRequestDescribeWorkspacesPaginateTypeDef = TypedDict(
+    "DescribeWorkspacesRequestDescribeWorkspacesPaginateTypeDef",
+    {
+        "WorkspaceIds": Sequence[str],
+        "DirectoryId": str,
+        "UserName": str,
+        "BundleId": str,
+        "PaginationConfig": PaginatorConfigTypeDef,
     },
+    total=False,
 )
 
+_RequiredListAvailableManagementCidrRangesRequestListAvailableManagementCidrRangesPaginateTypeDef = TypedDict(
+    "_RequiredListAvailableManagementCidrRangesRequestListAvailableManagementCidrRangesPaginateTypeDef",
+    {
+        "ManagementCidrRangeConstraint": str,
+    },
+)
+_OptionalListAvailableManagementCidrRangesRequestListAvailableManagementCidrRangesPaginateTypeDef = TypedDict(
+    "_OptionalListAvailableManagementCidrRangesRequestListAvailableManagementCidrRangesPaginateTypeDef",
+    {
+        "PaginationConfig": PaginatorConfigTypeDef,
+    },
+    total=False,
+)
+
+
+class ListAvailableManagementCidrRangesRequestListAvailableManagementCidrRangesPaginateTypeDef(
+    _RequiredListAvailableManagementCidrRangesRequestListAvailableManagementCidrRangesPaginateTypeDef,
+    _OptionalListAvailableManagementCidrRangesRequestListAvailableManagementCidrRangesPaginateTypeDef,
+):
+    pass
+
+
 DescribeClientBrandingResultTypeDef = TypedDict(
     "DescribeClientBrandingResultTypeDef",
     {
         "DeviceTypeWindows": DefaultClientBrandingAttributesTypeDef,
         "DeviceTypeOsx": DefaultClientBrandingAttributesTypeDef,
         "DeviceTypeAndroid": DefaultClientBrandingAttributesTypeDef,
         "DeviceTypeIos": IosClientBrandingAttributesTypeDef,
         "DeviceTypeLinux": DefaultClientBrandingAttributesTypeDef,
         "DeviceTypeWeb": DefaultClientBrandingAttributesTypeDef,
-        "ResponseMetadata": "ResponseMetadataTypeDef",
+        "ResponseMetadata": ResponseMetadataTypeDef,
     },
 )
 
 ImportClientBrandingResultTypeDef = TypedDict(
     "ImportClientBrandingResultTypeDef",
     {
         "DeviceTypeWindows": DefaultClientBrandingAttributesTypeDef,
         "DeviceTypeOsx": DefaultClientBrandingAttributesTypeDef,
         "DeviceTypeAndroid": DefaultClientBrandingAttributesTypeDef,
         "DeviceTypeIos": IosClientBrandingAttributesTypeDef,
         "DeviceTypeLinux": DefaultClientBrandingAttributesTypeDef,
         "DeviceTypeWeb": DefaultClientBrandingAttributesTypeDef,
-        "ResponseMetadata": "ResponseMetadataTypeDef",
+        "ResponseMetadata": ResponseMetadataTypeDef,
+    },
+)
+
+DescribeTagsResultTypeDef = TypedDict(
+    "DescribeTagsResultTypeDef",
+    {
+        "TagList": List[TagOutputTypeDef],
+        "ResponseMetadata": ResponseMetadataTypeDef,
+    },
+)
+
+StandbyWorkspaceOutputTypeDef = TypedDict(
+    "StandbyWorkspaceOutputTypeDef",
+    {
+        "PrimaryWorkspaceId": str,
+        "VolumeEncryptionKey": str,
+        "DirectoryId": str,
+        "Tags": List[TagOutputTypeDef],
     },
 )
 
 DescribeWorkspaceImagePermissionsResultTypeDef = TypedDict(
     "DescribeWorkspaceImagePermissionsResultTypeDef",
     {
         "ImageId": str,
         "ImagePermissions": List[ImagePermissionTypeDef],
         "NextToken": str,
-        "ResponseMetadata": "ResponseMetadataTypeDef",
+        "ResponseMetadata": ResponseMetadataTypeDef,
     },
 )
 
 DescribeWorkspaceSnapshotsResultTypeDef = TypedDict(
     "DescribeWorkspaceSnapshotsResultTypeDef",
     {
         "RebuildSnapshots": List[SnapshotTypeDef],
         "RestoreSnapshots": List[SnapshotTypeDef],
-        "ResponseMetadata": "ResponseMetadataTypeDef",
+        "ResponseMetadata": ResponseMetadataTypeDef,
     },
 )
 
 DescribeWorkspacesConnectionStatusResultTypeDef = TypedDict(
     "DescribeWorkspacesConnectionStatusResultTypeDef",
     {
         "WorkspacesConnectionStatus": List[WorkspaceConnectionStatusTypeDef],
         "NextToken": str,
-        "ResponseMetadata": "ResponseMetadataTypeDef",
+        "ResponseMetadata": ResponseMetadataTypeDef,
     },
 )
 
 RebootWorkspacesResultTypeDef = TypedDict(
     "RebootWorkspacesResultTypeDef",
     {
         "FailedRequests": List[FailedWorkspaceChangeRequestTypeDef],
-        "ResponseMetadata": "ResponseMetadataTypeDef",
+        "ResponseMetadata": ResponseMetadataTypeDef,
     },
 )
 
 RebuildWorkspacesResultTypeDef = TypedDict(
     "RebuildWorkspacesResultTypeDef",
     {
         "FailedRequests": List[FailedWorkspaceChangeRequestTypeDef],
-        "ResponseMetadata": "ResponseMetadataTypeDef",
+        "ResponseMetadata": ResponseMetadataTypeDef,
     },
 )
 
 StartWorkspacesResultTypeDef = TypedDict(
     "StartWorkspacesResultTypeDef",
     {
         "FailedRequests": List[FailedWorkspaceChangeRequestTypeDef],
-        "ResponseMetadata": "ResponseMetadataTypeDef",
+        "ResponseMetadata": ResponseMetadataTypeDef,
     },
 )
 
 StopWorkspacesResultTypeDef = TypedDict(
     "StopWorkspacesResultTypeDef",
     {
         "FailedRequests": List[FailedWorkspaceChangeRequestTypeDef],
-        "ResponseMetadata": "ResponseMetadataTypeDef",
+        "ResponseMetadata": ResponseMetadataTypeDef,
     },
 )
 
 TerminateWorkspacesResultTypeDef = TypedDict(
     "TerminateWorkspacesResultTypeDef",
     {
         "FailedRequests": List[FailedWorkspaceChangeRequestTypeDef],
-        "ResponseMetadata": "ResponseMetadataTypeDef",
+        "ResponseMetadata": ResponseMetadataTypeDef,
     },
 )
 
 _RequiredImportClientBrandingRequestRequestTypeDef = TypedDict(
     "_RequiredImportClientBrandingRequestRequestTypeDef",
     {
         "ResourceId": str,
@@ -1662,14 +1746,24 @@
 class ImportClientBrandingRequestRequestTypeDef(
     _RequiredImportClientBrandingRequestRequestTypeDef,
     _OptionalImportClientBrandingRequestRequestTypeDef,
 ):
     pass
 
 
+WorkspacesIpGroupTypeDef = TypedDict(
+    "WorkspacesIpGroupTypeDef",
+    {
+        "groupId": str,
+        "groupName": str,
+        "groupDesc": str,
+        "userRules": List[IpRuleItemOutputTypeDef],
+    },
+)
+
 _RequiredModifySamlPropertiesRequestRequestTypeDef = TypedDict(
     "_RequiredModifySamlPropertiesRequestRequestTypeDef",
     {
         "ResourceId": str,
     },
 )
 _OptionalModifySamlPropertiesRequestRequestTypeDef = TypedDict(
@@ -1701,39 +1795,14 @@
     "ModifyWorkspaceAccessPropertiesRequestRequestTypeDef",
     {
         "ResourceId": str,
         "WorkspaceAccessProperties": WorkspaceAccessPropertiesTypeDef,
     },
 )
 
-WorkspaceDirectoryTypeDef = TypedDict(
-    "WorkspaceDirectoryTypeDef",
-    {
-        "DirectoryId": str,
-        "Alias": str,
-        "DirectoryName": str,
-        "RegistrationCode": str,
-        "SubnetIds": List[str],
-        "DnsIpAddresses": List[str],
-        "CustomerUserName": str,
-        "IamRoleId": str,
-        "DirectoryType": WorkspaceDirectoryTypeType,
-        "WorkspaceSecurityGroupId": str,
-        "State": WorkspaceDirectoryStateType,
-        "WorkspaceCreationProperties": DefaultWorkspaceCreationPropertiesTypeDef,
-        "ipGroupIds": List[str],
-        "WorkspaceAccessProperties": WorkspaceAccessPropertiesTypeDef,
-        "Tenancy": TenancyType,
-        "SelfservicePermissions": SelfservicePermissionsTypeDef,
-        "SamlProperties": SamlPropertiesTypeDef,
-        "CertificateBasedAuthProperties": CertificateBasedAuthPropertiesTypeDef,
-    },
-    total=False,
-)
-
 ModifyWorkspaceCreationPropertiesRequestRequestTypeDef = TypedDict(
     "ModifyWorkspaceCreationPropertiesRequestRequestTypeDef",
     {
         "ResourceId": str,
         "WorkspaceCreationProperties": WorkspaceCreationPropertiesTypeDef,
     },
 )
@@ -1781,37 +1850,14 @@
 RebuildWorkspacesRequestRequestTypeDef = TypedDict(
     "RebuildWorkspacesRequestRequestTypeDef",
     {
         "RebuildWorkspaceRequests": Sequence[RebuildRequestTypeDef],
     },
 )
 
-WorkspaceTypeDef = TypedDict(
-    "WorkspaceTypeDef",
-    {
-        "WorkspaceId": str,
-        "DirectoryId": str,
-        "UserName": str,
-        "IpAddress": str,
-        "State": WorkspaceStateType,
-        "BundleId": str,
-        "SubnetId": str,
-        "ErrorMessage": str,
-        "ErrorCode": str,
-        "ComputerName": str,
-        "VolumeEncryptionKey": str,
-        "UserVolumeEncryptionEnabled": bool,
-        "RootVolumeEncryptionEnabled": bool,
-        "WorkspaceProperties": WorkspacePropertiesTypeDef,
-        "ModificationStates": List[ModificationStateTypeDef],
-        "RelatedWorkspaces": List[RelatedWorkspacePropertiesTypeDef],
-    },
-    total=False,
-)
-
 StartWorkspacesRequestRequestTypeDef = TypedDict(
     "StartWorkspacesRequestRequestTypeDef",
     {
         "StartWorkspaceRequests": Sequence[StartRequestTypeDef],
     },
 )
 
@@ -1840,132 +1886,207 @@
         "RequiredTenancy": WorkspaceImageRequiredTenancyType,
         "ErrorCode": str,
         "ErrorMessage": str,
         "Created": datetime,
         "OwnerAccountId": str,
         "Updates": UpdateResultTypeDef,
     },
-    total=False,
 )
 
-DescribeIpGroupsResultTypeDef = TypedDict(
-    "DescribeIpGroupsResultTypeDef",
+WorkspaceBundleTypeDef = TypedDict(
+    "WorkspaceBundleTypeDef",
     {
-        "Result": List[WorkspacesIpGroupTypeDef],
-        "NextToken": str,
-        "ResponseMetadata": "ResponseMetadataTypeDef",
+        "BundleId": str,
+        "Name": str,
+        "Owner": str,
+        "Description": str,
+        "ImageId": str,
+        "RootStorage": RootStorageOutputTypeDef,
+        "UserStorage": UserStorageOutputTypeDef,
+        "ComputeType": ComputeTypeOutputTypeDef,
+        "LastUpdatedTime": datetime,
+        "CreationTime": datetime,
+        "State": WorkspaceBundleStateType,
+        "BundleType": BundleTypeType,
+    },
+)
+
+WorkspaceDirectoryTypeDef = TypedDict(
+    "WorkspaceDirectoryTypeDef",
+    {
+        "DirectoryId": str,
+        "Alias": str,
+        "DirectoryName": str,
+        "RegistrationCode": str,
+        "SubnetIds": List[str],
+        "DnsIpAddresses": List[str],
+        "CustomerUserName": str,
+        "IamRoleId": str,
+        "DirectoryType": WorkspaceDirectoryTypeType,
+        "WorkspaceSecurityGroupId": str,
+        "State": WorkspaceDirectoryStateType,
+        "WorkspaceCreationProperties": DefaultWorkspaceCreationPropertiesTypeDef,
+        "ipGroupIds": List[str],
+        "WorkspaceAccessProperties": WorkspaceAccessPropertiesOutputTypeDef,
+        "Tenancy": TenancyType,
+        "SelfservicePermissions": SelfservicePermissionsOutputTypeDef,
+        "SamlProperties": SamlPropertiesOutputTypeDef,
+        "CertificateBasedAuthProperties": CertificateBasedAuthPropertiesOutputTypeDef,
+    },
+)
+
+WorkspaceRequestOutputTypeDef = TypedDict(
+    "WorkspaceRequestOutputTypeDef",
+    {
+        "DirectoryId": str,
+        "UserName": str,
+        "BundleId": str,
+        "VolumeEncryptionKey": str,
+        "UserVolumeEncryptionEnabled": bool,
+        "RootVolumeEncryptionEnabled": bool,
+        "WorkspaceProperties": WorkspacePropertiesOutputTypeDef,
+        "Tags": List[TagOutputTypeDef],
+    },
+)
+
+WorkspaceTypeDef = TypedDict(
+    "WorkspaceTypeDef",
+    {
+        "WorkspaceId": str,
+        "DirectoryId": str,
+        "UserName": str,
+        "IpAddress": str,
+        "State": WorkspaceStateType,
+        "BundleId": str,
+        "SubnetId": str,
+        "ErrorMessage": str,
+        "ErrorCode": str,
+        "ComputerName": str,
+        "VolumeEncryptionKey": str,
+        "UserVolumeEncryptionEnabled": bool,
+        "RootVolumeEncryptionEnabled": bool,
+        "WorkspaceProperties": WorkspacePropertiesOutputTypeDef,
+        "ModificationStates": List[ModificationStateTypeDef],
+        "RelatedWorkspaces": List[RelatedWorkspacePropertiesTypeDef],
     },
 )
 
 DescribeClientPropertiesResultTypeDef = TypedDict(
     "DescribeClientPropertiesResultTypeDef",
     {
         "ClientPropertiesList": List[ClientPropertiesResultTypeDef],
-        "ResponseMetadata": "ResponseMetadataTypeDef",
+        "ResponseMetadata": ResponseMetadataTypeDef,
     },
 )
 
 DescribeConnectionAliasesResultTypeDef = TypedDict(
     "DescribeConnectionAliasesResultTypeDef",
     {
         "ConnectionAliases": List[ConnectionAliasTypeDef],
         "NextToken": str,
-        "ResponseMetadata": "ResponseMetadataTypeDef",
+        "ResponseMetadata": ResponseMetadataTypeDef,
     },
 )
 
 CreateStandbyWorkspacesRequestRequestTypeDef = TypedDict(
     "CreateStandbyWorkspacesRequestRequestTypeDef",
     {
         "PrimaryRegion": str,
         "StandbyWorkspaces": Sequence[StandbyWorkspaceTypeDef],
     },
 )
 
 FailedCreateStandbyWorkspacesRequestTypeDef = TypedDict(
     "FailedCreateStandbyWorkspacesRequestTypeDef",
     {
-        "StandbyWorkspaceRequest": StandbyWorkspaceTypeDef,
+        "StandbyWorkspaceRequest": StandbyWorkspaceOutputTypeDef,
         "ErrorCode": str,
         "ErrorMessage": str,
     },
-    total=False,
+)
+
+DescribeIpGroupsResultTypeDef = TypedDict(
+    "DescribeIpGroupsResultTypeDef",
+    {
+        "Result": List[WorkspacesIpGroupTypeDef],
+        "NextToken": str,
+        "ResponseMetadata": ResponseMetadataTypeDef,
+    },
+)
+
+CreateWorkspacesRequestRequestTypeDef = TypedDict(
+    "CreateWorkspacesRequestRequestTypeDef",
+    {
+        "Workspaces": Sequence[WorkspaceRequestTypeDef],
+    },
+)
+
+DescribeWorkspaceImagesResultTypeDef = TypedDict(
+    "DescribeWorkspaceImagesResultTypeDef",
+    {
+        "Images": List[WorkspaceImageTypeDef],
+        "NextToken": str,
+        "ResponseMetadata": ResponseMetadataTypeDef,
+    },
 )
 
 CreateWorkspaceBundleResultTypeDef = TypedDict(
     "CreateWorkspaceBundleResultTypeDef",
     {
         "WorkspaceBundle": WorkspaceBundleTypeDef,
-        "ResponseMetadata": "ResponseMetadataTypeDef",
+        "ResponseMetadata": ResponseMetadataTypeDef,
     },
 )
 
 DescribeWorkspaceBundlesResultTypeDef = TypedDict(
     "DescribeWorkspaceBundlesResultTypeDef",
     {
         "Bundles": List[WorkspaceBundleTypeDef],
         "NextToken": str,
-        "ResponseMetadata": "ResponseMetadataTypeDef",
+        "ResponseMetadata": ResponseMetadataTypeDef,
     },
 )
 
 DescribeWorkspaceDirectoriesResultTypeDef = TypedDict(
     "DescribeWorkspaceDirectoriesResultTypeDef",
     {
         "Directories": List[WorkspaceDirectoryTypeDef],
         "NextToken": str,
-        "ResponseMetadata": "ResponseMetadataTypeDef",
-    },
-)
-
-CreateWorkspacesRequestRequestTypeDef = TypedDict(
-    "CreateWorkspacesRequestRequestTypeDef",
-    {
-        "Workspaces": Sequence[WorkspaceRequestTypeDef],
+        "ResponseMetadata": ResponseMetadataTypeDef,
     },
 )
 
 FailedCreateWorkspaceRequestTypeDef = TypedDict(
     "FailedCreateWorkspaceRequestTypeDef",
     {
-        "WorkspaceRequest": WorkspaceRequestTypeDef,
+        "WorkspaceRequest": WorkspaceRequestOutputTypeDef,
         "ErrorCode": str,
         "ErrorMessage": str,
     },
-    total=False,
 )
 
 DescribeWorkspacesResultTypeDef = TypedDict(
     "DescribeWorkspacesResultTypeDef",
     {
         "Workspaces": List[WorkspaceTypeDef],
         "NextToken": str,
-        "ResponseMetadata": "ResponseMetadataTypeDef",
-    },
-)
-
-DescribeWorkspaceImagesResultTypeDef = TypedDict(
-    "DescribeWorkspaceImagesResultTypeDef",
-    {
-        "Images": List[WorkspaceImageTypeDef],
-        "NextToken": str,
-        "ResponseMetadata": "ResponseMetadataTypeDef",
+        "ResponseMetadata": ResponseMetadataTypeDef,
     },
 )
 
 CreateStandbyWorkspacesResultTypeDef = TypedDict(
     "CreateStandbyWorkspacesResultTypeDef",
     {
         "FailedStandbyRequests": List[FailedCreateStandbyWorkspacesRequestTypeDef],
         "PendingStandbyRequests": List[PendingCreateStandbyWorkspacesRequestTypeDef],
-        "ResponseMetadata": "ResponseMetadataTypeDef",
+        "ResponseMetadata": ResponseMetadataTypeDef,
     },
 )
 
 CreateWorkspacesResultTypeDef = TypedDict(
     "CreateWorkspacesResultTypeDef",
     {
         "FailedRequests": List[FailedCreateWorkspaceRequestTypeDef],
         "PendingRequests": List[WorkspaceTypeDef],
-        "ResponseMetadata": "ResponseMetadataTypeDef",
+        "ResponseMetadata": ResponseMetadataTypeDef,
     },
 )
```

### Comparing `mypy-boto3-workspaces-1.28.0/mypy_boto3_workspaces/type_defs.pyi` & `mypy-boto3-workspaces-1.28.9/mypy_boto3_workspaces/type_defs.pyi`

 * *Files 3% similar despite different names*

```diff
@@ -59,195 +59,211 @@
     from typing import TypedDict
 else:
     from typing_extensions import TypedDict
 
 __all__ = (
     "AccountModificationTypeDef",
     "AssociateConnectionAliasRequestRequestTypeDef",
-    "AssociateConnectionAliasResultTypeDef",
+    "ResponseMetadataTypeDef",
     "AssociateIpGroupsRequestRequestTypeDef",
     "IpRuleItemTypeDef",
+    "CertificateBasedAuthPropertiesOutputTypeDef",
     "CertificateBasedAuthPropertiesTypeDef",
+    "ClientPropertiesOutputTypeDef",
     "ClientPropertiesTypeDef",
+    "ComputeTypeOutputTypeDef",
     "ComputeTypeTypeDef",
     "ConnectClientAddInTypeDef",
     "ConnectionAliasAssociationTypeDef",
+    "ConnectionAliasPermissionOutputTypeDef",
     "ConnectionAliasPermissionTypeDef",
     "TagTypeDef",
-    "CopyWorkspaceImageResultTypeDef",
     "CreateConnectClientAddInRequestRequestTypeDef",
-    "CreateConnectClientAddInResultTypeDef",
-    "CreateConnectionAliasResultTypeDef",
-    "CreateIpGroupResultTypeDef",
     "PendingCreateStandbyWorkspacesRequestTypeDef",
-    "CreateUpdatedWorkspaceImageResultTypeDef",
     "RootStorageTypeDef",
     "UserStorageTypeDef",
     "OperatingSystemTypeDef",
     "DefaultClientBrandingAttributesTypeDef",
     "DefaultImportClientBrandingAttributesTypeDef",
     "DefaultWorkspaceCreationPropertiesTypeDef",
     "DeleteClientBrandingRequestRequestTypeDef",
     "DeleteConnectClientAddInRequestRequestTypeDef",
     "DeleteConnectionAliasRequestRequestTypeDef",
     "DeleteIpGroupRequestRequestTypeDef",
     "DeleteTagsRequestRequestTypeDef",
     "DeleteWorkspaceBundleRequestRequestTypeDef",
     "DeleteWorkspaceImageRequestRequestTypeDef",
     "DeregisterWorkspaceDirectoryRequestRequestTypeDef",
-    "DescribeAccountModificationsRequestDescribeAccountModificationsPaginateTypeDef",
+    "PaginatorConfigTypeDef",
     "DescribeAccountModificationsRequestRequestTypeDef",
-    "DescribeAccountResultTypeDef",
     "DescribeClientBrandingRequestRequestTypeDef",
     "IosClientBrandingAttributesTypeDef",
     "DescribeClientPropertiesRequestRequestTypeDef",
     "DescribeConnectClientAddInsRequestRequestTypeDef",
     "DescribeConnectionAliasPermissionsRequestRequestTypeDef",
     "DescribeConnectionAliasesRequestRequestTypeDef",
-    "DescribeIpGroupsRequestDescribeIpGroupsPaginateTypeDef",
     "DescribeIpGroupsRequestRequestTypeDef",
     "DescribeTagsRequestRequestTypeDef",
-    "DescribeWorkspaceBundlesRequestDescribeWorkspaceBundlesPaginateTypeDef",
+    "TagOutputTypeDef",
     "DescribeWorkspaceBundlesRequestRequestTypeDef",
-    "DescribeWorkspaceDirectoriesRequestDescribeWorkspaceDirectoriesPaginateTypeDef",
     "DescribeWorkspaceDirectoriesRequestRequestTypeDef",
     "DescribeWorkspaceImagePermissionsRequestRequestTypeDef",
     "ImagePermissionTypeDef",
-    "DescribeWorkspaceImagesRequestDescribeWorkspaceImagesPaginateTypeDef",
     "DescribeWorkspaceImagesRequestRequestTypeDef",
     "DescribeWorkspaceSnapshotsRequestRequestTypeDef",
     "SnapshotTypeDef",
-    "DescribeWorkspacesConnectionStatusRequestDescribeWorkspacesConnectionStatusPaginateTypeDef",
     "DescribeWorkspacesConnectionStatusRequestRequestTypeDef",
     "WorkspaceConnectionStatusTypeDef",
-    "DescribeWorkspacesRequestDescribeWorkspacesPaginateTypeDef",
     "DescribeWorkspacesRequestRequestTypeDef",
     "DisassociateConnectionAliasRequestRequestTypeDef",
     "DisassociateIpGroupsRequestRequestTypeDef",
     "FailedWorkspaceChangeRequestTypeDef",
     "IosImportClientBrandingAttributesTypeDef",
-    "ImportWorkspaceImageResultTypeDef",
-    "ListAvailableManagementCidrRangesRequestListAvailableManagementCidrRangesPaginateTypeDef",
+    "IpRuleItemOutputTypeDef",
     "ListAvailableManagementCidrRangesRequestRequestTypeDef",
-    "ListAvailableManagementCidrRangesResultTypeDef",
     "MigrateWorkspaceRequestRequestTypeDef",
-    "MigrateWorkspaceResultTypeDef",
     "ModificationStateTypeDef",
     "ModifyAccountRequestRequestTypeDef",
     "SamlPropertiesTypeDef",
     "SelfservicePermissionsTypeDef",
     "WorkspaceAccessPropertiesTypeDef",
     "WorkspaceCreationPropertiesTypeDef",
     "WorkspacePropertiesTypeDef",
     "ModifyWorkspaceStateRequestRequestTypeDef",
-    "PaginatorConfigTypeDef",
     "RebootRequestTypeDef",
     "RebuildRequestTypeDef",
     "RelatedWorkspacePropertiesTypeDef",
-    "ResponseMetadataTypeDef",
     "RestoreWorkspaceRequestRequestTypeDef",
     "RevokeIpRulesRequestRequestTypeDef",
+    "RootStorageOutputTypeDef",
+    "SamlPropertiesOutputTypeDef",
+    "SelfservicePermissionsOutputTypeDef",
     "StartRequestTypeDef",
     "StopRequestTypeDef",
     "TerminateRequestTypeDef",
     "UpdateConnectClientAddInRequestRequestTypeDef",
     "UpdateResultTypeDef",
     "UpdateWorkspaceBundleRequestRequestTypeDef",
     "UpdateWorkspaceImagePermissionRequestRequestTypeDef",
+    "UserStorageOutputTypeDef",
+    "WorkspaceAccessPropertiesOutputTypeDef",
+    "WorkspacePropertiesOutputTypeDef",
+    "AssociateConnectionAliasResultTypeDef",
+    "CopyWorkspaceImageResultTypeDef",
+    "CreateConnectClientAddInResultTypeDef",
+    "CreateConnectionAliasResultTypeDef",
+    "CreateIpGroupResultTypeDef",
+    "CreateUpdatedWorkspaceImageResultTypeDef",
     "DescribeAccountModificationsResultTypeDef",
+    "DescribeAccountResultTypeDef",
+    "ImportWorkspaceImageResultTypeDef",
+    "ListAvailableManagementCidrRangesResultTypeDef",
+    "MigrateWorkspaceResultTypeDef",
     "AuthorizeIpRulesRequestRequestTypeDef",
     "UpdateRulesOfIpGroupRequestRequestTypeDef",
-    "WorkspacesIpGroupTypeDef",
     "ModifyCertificateBasedAuthPropertiesRequestRequestTypeDef",
     "ClientPropertiesResultTypeDef",
     "ModifyClientPropertiesRequestRequestTypeDef",
     "DescribeConnectClientAddInsResultTypeDef",
     "ConnectionAliasTypeDef",
     "DescribeConnectionAliasPermissionsResultTypeDef",
     "UpdateConnectionAliasPermissionRequestRequestTypeDef",
     "CopyWorkspaceImageRequestRequestTypeDef",
     "CreateConnectionAliasRequestRequestTypeDef",
     "CreateIpGroupRequestRequestTypeDef",
     "CreateTagsRequestRequestTypeDef",
     "CreateUpdatedWorkspaceImageRequestRequestTypeDef",
     "CreateWorkspaceImageRequestRequestTypeDef",
-    "DescribeTagsResultTypeDef",
     "ImportWorkspaceImageRequestRequestTypeDef",
     "RegisterWorkspaceDirectoryRequestRequestTypeDef",
     "StandbyWorkspaceTypeDef",
     "CreateWorkspaceBundleRequestRequestTypeDef",
-    "WorkspaceBundleTypeDef",
     "CreateWorkspaceImageResultTypeDef",
+    "DescribeAccountModificationsRequestDescribeAccountModificationsPaginateTypeDef",
+    "DescribeIpGroupsRequestDescribeIpGroupsPaginateTypeDef",
+    "DescribeWorkspaceBundlesRequestDescribeWorkspaceBundlesPaginateTypeDef",
+    "DescribeWorkspaceDirectoriesRequestDescribeWorkspaceDirectoriesPaginateTypeDef",
+    "DescribeWorkspaceImagesRequestDescribeWorkspaceImagesPaginateTypeDef",
+    "DescribeWorkspacesConnectionStatusRequestDescribeWorkspacesConnectionStatusPaginateTypeDef",
+    "DescribeWorkspacesRequestDescribeWorkspacesPaginateTypeDef",
+    "ListAvailableManagementCidrRangesRequestListAvailableManagementCidrRangesPaginateTypeDef",
     "DescribeClientBrandingResultTypeDef",
     "ImportClientBrandingResultTypeDef",
+    "DescribeTagsResultTypeDef",
+    "StandbyWorkspaceOutputTypeDef",
     "DescribeWorkspaceImagePermissionsResultTypeDef",
     "DescribeWorkspaceSnapshotsResultTypeDef",
     "DescribeWorkspacesConnectionStatusResultTypeDef",
     "RebootWorkspacesResultTypeDef",
     "RebuildWorkspacesResultTypeDef",
     "StartWorkspacesResultTypeDef",
     "StopWorkspacesResultTypeDef",
     "TerminateWorkspacesResultTypeDef",
     "ImportClientBrandingRequestRequestTypeDef",
+    "WorkspacesIpGroupTypeDef",
     "ModifySamlPropertiesRequestRequestTypeDef",
     "ModifySelfservicePermissionsRequestRequestTypeDef",
     "ModifyWorkspaceAccessPropertiesRequestRequestTypeDef",
-    "WorkspaceDirectoryTypeDef",
     "ModifyWorkspaceCreationPropertiesRequestRequestTypeDef",
     "ModifyWorkspacePropertiesRequestRequestTypeDef",
     "WorkspaceRequestTypeDef",
     "RebootWorkspacesRequestRequestTypeDef",
     "RebuildWorkspacesRequestRequestTypeDef",
-    "WorkspaceTypeDef",
     "StartWorkspacesRequestRequestTypeDef",
     "StopWorkspacesRequestRequestTypeDef",
     "TerminateWorkspacesRequestRequestTypeDef",
     "WorkspaceImageTypeDef",
-    "DescribeIpGroupsResultTypeDef",
+    "WorkspaceBundleTypeDef",
+    "WorkspaceDirectoryTypeDef",
+    "WorkspaceRequestOutputTypeDef",
+    "WorkspaceTypeDef",
     "DescribeClientPropertiesResultTypeDef",
     "DescribeConnectionAliasesResultTypeDef",
     "CreateStandbyWorkspacesRequestRequestTypeDef",
     "FailedCreateStandbyWorkspacesRequestTypeDef",
+    "DescribeIpGroupsResultTypeDef",
+    "CreateWorkspacesRequestRequestTypeDef",
+    "DescribeWorkspaceImagesResultTypeDef",
     "CreateWorkspaceBundleResultTypeDef",
     "DescribeWorkspaceBundlesResultTypeDef",
     "DescribeWorkspaceDirectoriesResultTypeDef",
-    "CreateWorkspacesRequestRequestTypeDef",
     "FailedCreateWorkspaceRequestTypeDef",
     "DescribeWorkspacesResultTypeDef",
-    "DescribeWorkspaceImagesResultTypeDef",
     "CreateStandbyWorkspacesResultTypeDef",
     "CreateWorkspacesResultTypeDef",
 )
 
 AccountModificationTypeDef = TypedDict(
     "AccountModificationTypeDef",
     {
         "ModificationState": DedicatedTenancyModificationStateEnumType,
         "DedicatedTenancySupport": DedicatedTenancySupportResultEnumType,
         "DedicatedTenancyManagementCidrRange": str,
         "StartTime": datetime,
         "ErrorCode": str,
         "ErrorMessage": str,
     },
-    total=False,
 )
 
 AssociateConnectionAliasRequestRequestTypeDef = TypedDict(
     "AssociateConnectionAliasRequestRequestTypeDef",
     {
         "AliasId": str,
         "ResourceId": str,
     },
 )
 
-AssociateConnectionAliasResultTypeDef = TypedDict(
-    "AssociateConnectionAliasResultTypeDef",
+ResponseMetadataTypeDef = TypedDict(
+    "ResponseMetadataTypeDef",
     {
-        "ConnectionIdentifier": str,
-        "ResponseMetadata": "ResponseMetadataTypeDef",
+        "RequestId": str,
+        "HostId": str,
+        "HTTPStatusCode": int,
+        "HTTPHeaders": Dict[str, str],
+        "RetryAttempts": int,
     },
 )
 
 AssociateIpGroupsRequestRequestTypeDef = TypedDict(
     "AssociateIpGroupsRequestRequestTypeDef",
     {
         "DirectoryId": str,
@@ -260,32 +276,55 @@
     {
         "ipRule": str,
         "ruleDesc": str,
     },
     total=False,
 )
 
+CertificateBasedAuthPropertiesOutputTypeDef = TypedDict(
+    "CertificateBasedAuthPropertiesOutputTypeDef",
+    {
+        "Status": CertificateBasedAuthStatusEnumType,
+        "CertificateAuthorityArn": str,
+    },
+)
+
 CertificateBasedAuthPropertiesTypeDef = TypedDict(
     "CertificateBasedAuthPropertiesTypeDef",
     {
         "Status": CertificateBasedAuthStatusEnumType,
         "CertificateAuthorityArn": str,
     },
     total=False,
 )
 
+ClientPropertiesOutputTypeDef = TypedDict(
+    "ClientPropertiesOutputTypeDef",
+    {
+        "ReconnectEnabled": ReconnectEnumType,
+        "LogUploadEnabled": LogUploadEnumType,
+    },
+)
+
 ClientPropertiesTypeDef = TypedDict(
     "ClientPropertiesTypeDef",
     {
         "ReconnectEnabled": ReconnectEnumType,
         "LogUploadEnabled": LogUploadEnumType,
     },
     total=False,
 )
 
+ComputeTypeOutputTypeDef = TypedDict(
+    "ComputeTypeOutputTypeDef",
+    {
+        "Name": ComputeType,
+    },
+)
+
 ComputeTypeTypeDef = TypedDict(
     "ComputeTypeTypeDef",
     {
         "Name": ComputeType,
     },
     total=False,
 )
@@ -294,26 +333,32 @@
     "ConnectClientAddInTypeDef",
     {
         "AddInId": str,
         "ResourceId": str,
         "Name": str,
         "URL": str,
     },
-    total=False,
 )
 
 ConnectionAliasAssociationTypeDef = TypedDict(
     "ConnectionAliasAssociationTypeDef",
     {
         "AssociationStatus": AssociationStatusType,
         "AssociatedAccountId": str,
         "ResourceId": str,
         "ConnectionIdentifier": str,
     },
-    total=False,
+)
+
+ConnectionAliasPermissionOutputTypeDef = TypedDict(
+    "ConnectionAliasPermissionOutputTypeDef",
+    {
+        "SharedAccountId": str,
+        "AllowAssociation": bool,
+    },
 )
 
 ConnectionAliasPermissionTypeDef = TypedDict(
     "ConnectionAliasPermissionTypeDef",
     {
         "SharedAccountId": str,
         "AllowAssociation": bool,
@@ -333,72 +378,31 @@
     },
     total=False,
 )
 
 class TagTypeDef(_RequiredTagTypeDef, _OptionalTagTypeDef):
     pass
 
-CopyWorkspaceImageResultTypeDef = TypedDict(
-    "CopyWorkspaceImageResultTypeDef",
-    {
-        "ImageId": str,
-        "ResponseMetadata": "ResponseMetadataTypeDef",
-    },
-)
-
 CreateConnectClientAddInRequestRequestTypeDef = TypedDict(
     "CreateConnectClientAddInRequestRequestTypeDef",
     {
         "ResourceId": str,
         "Name": str,
         "URL": str,
     },
 )
 
-CreateConnectClientAddInResultTypeDef = TypedDict(
-    "CreateConnectClientAddInResultTypeDef",
-    {
-        "AddInId": str,
-        "ResponseMetadata": "ResponseMetadataTypeDef",
-    },
-)
-
-CreateConnectionAliasResultTypeDef = TypedDict(
-    "CreateConnectionAliasResultTypeDef",
-    {
-        "AliasId": str,
-        "ResponseMetadata": "ResponseMetadataTypeDef",
-    },
-)
-
-CreateIpGroupResultTypeDef = TypedDict(
-    "CreateIpGroupResultTypeDef",
-    {
-        "GroupId": str,
-        "ResponseMetadata": "ResponseMetadataTypeDef",
-    },
-)
-
 PendingCreateStandbyWorkspacesRequestTypeDef = TypedDict(
     "PendingCreateStandbyWorkspacesRequestTypeDef",
     {
         "UserName": str,
         "DirectoryId": str,
         "State": WorkspaceStateType,
         "WorkspaceId": str,
     },
-    total=False,
-)
-
-CreateUpdatedWorkspaceImageResultTypeDef = TypedDict(
-    "CreateUpdatedWorkspaceImageResultTypeDef",
-    {
-        "ImageId": str,
-        "ResponseMetadata": "ResponseMetadataTypeDef",
-    },
 )
 
 RootStorageTypeDef = TypedDict(
     "RootStorageTypeDef",
     {
         "Capacity": str,
     },
@@ -414,27 +418,25 @@
 )
 
 OperatingSystemTypeDef = TypedDict(
     "OperatingSystemTypeDef",
     {
         "Type": OperatingSystemTypeType,
     },
-    total=False,
 )
 
 DefaultClientBrandingAttributesTypeDef = TypedDict(
     "DefaultClientBrandingAttributesTypeDef",
     {
         "LogoUrl": str,
         "SupportEmail": str,
         "SupportLink": str,
         "ForgotPasswordLink": str,
         "LoginMessage": Dict[str, str],
     },
-    total=False,
 )
 
 DefaultImportClientBrandingAttributesTypeDef = TypedDict(
     "DefaultImportClientBrandingAttributesTypeDef",
     {
         "Logo": Union[str, bytes, IO[Any], StreamingBody],
         "SupportEmail": str,
@@ -451,15 +453,14 @@
         "EnableWorkDocs": bool,
         "EnableInternetAccess": bool,
         "DefaultOu": str,
         "CustomSecurityGroupId": str,
         "UserEnabledAsLocalAdministrator": bool,
         "EnableMaintenanceMode": bool,
     },
-    total=False,
 )
 
 DeleteClientBrandingRequestRequestTypeDef = TypedDict(
     "DeleteClientBrandingRequestRequestTypeDef",
     {
         "ResourceId": str,
         "Platforms": Sequence[ClientDeviceTypeType],
@@ -514,39 +515,32 @@
 DeregisterWorkspaceDirectoryRequestRequestTypeDef = TypedDict(
     "DeregisterWorkspaceDirectoryRequestRequestTypeDef",
     {
         "DirectoryId": str,
     },
 )
 
-DescribeAccountModificationsRequestDescribeAccountModificationsPaginateTypeDef = TypedDict(
-    "DescribeAccountModificationsRequestDescribeAccountModificationsPaginateTypeDef",
+PaginatorConfigTypeDef = TypedDict(
+    "PaginatorConfigTypeDef",
     {
-        "PaginationConfig": "PaginatorConfigTypeDef",
+        "MaxItems": int,
+        "PageSize": int,
+        "StartingToken": str,
     },
     total=False,
 )
 
 DescribeAccountModificationsRequestRequestTypeDef = TypedDict(
     "DescribeAccountModificationsRequestRequestTypeDef",
     {
         "NextToken": str,
     },
     total=False,
 )
 
-DescribeAccountResultTypeDef = TypedDict(
-    "DescribeAccountResultTypeDef",
-    {
-        "DedicatedTenancySupport": DedicatedTenancySupportResultEnumType,
-        "DedicatedTenancyManagementCidrRange": str,
-        "ResponseMetadata": "ResponseMetadataTypeDef",
-    },
-)
-
 DescribeClientBrandingRequestRequestTypeDef = TypedDict(
     "DescribeClientBrandingRequestRequestTypeDef",
     {
         "ResourceId": str,
     },
 )
 
@@ -557,15 +551,14 @@
         "Logo2xUrl": str,
         "Logo3xUrl": str,
         "SupportEmail": str,
         "SupportLink": str,
         "ForgotPasswordLink": str,
         "LoginMessage": Dict[str, str],
     },
-    total=False,
 )
 
 DescribeClientPropertiesRequestRequestTypeDef = TypedDict(
     "DescribeClientPropertiesRequestRequestTypeDef",
     {
         "ResourceIds": Sequence[str],
     },
@@ -620,23 +613,14 @@
         "ResourceId": str,
         "Limit": int,
         "NextToken": str,
     },
     total=False,
 )
 
-DescribeIpGroupsRequestDescribeIpGroupsPaginateTypeDef = TypedDict(
-    "DescribeIpGroupsRequestDescribeIpGroupsPaginateTypeDef",
-    {
-        "GroupIds": Sequence[str],
-        "PaginationConfig": "PaginatorConfigTypeDef",
-    },
-    total=False,
-)
-
 DescribeIpGroupsRequestRequestTypeDef = TypedDict(
     "DescribeIpGroupsRequestRequestTypeDef",
     {
         "GroupIds": Sequence[str],
         "NextToken": str,
         "MaxResults": int,
     },
@@ -646,44 +630,32 @@
 DescribeTagsRequestRequestTypeDef = TypedDict(
     "DescribeTagsRequestRequestTypeDef",
     {
         "ResourceId": str,
     },
 )
 
-DescribeWorkspaceBundlesRequestDescribeWorkspaceBundlesPaginateTypeDef = TypedDict(
-    "DescribeWorkspaceBundlesRequestDescribeWorkspaceBundlesPaginateTypeDef",
+TagOutputTypeDef = TypedDict(
+    "TagOutputTypeDef",
     {
-        "BundleIds": Sequence[str],
-        "Owner": str,
-        "PaginationConfig": "PaginatorConfigTypeDef",
+        "Key": str,
+        "Value": str,
     },
-    total=False,
 )
 
 DescribeWorkspaceBundlesRequestRequestTypeDef = TypedDict(
     "DescribeWorkspaceBundlesRequestRequestTypeDef",
     {
         "BundleIds": Sequence[str],
         "Owner": str,
         "NextToken": str,
     },
     total=False,
 )
 
-DescribeWorkspaceDirectoriesRequestDescribeWorkspaceDirectoriesPaginateTypeDef = TypedDict(
-    "DescribeWorkspaceDirectoriesRequestDescribeWorkspaceDirectoriesPaginateTypeDef",
-    {
-        "DirectoryIds": Sequence[str],
-        "Limit": int,
-        "PaginationConfig": "PaginatorConfigTypeDef",
-    },
-    total=False,
-)
-
 DescribeWorkspaceDirectoriesRequestRequestTypeDef = TypedDict(
     "DescribeWorkspaceDirectoriesRequestRequestTypeDef",
     {
         "DirectoryIds": Sequence[str],
         "Limit": int,
         "NextToken": str,
     },
@@ -712,25 +684,14 @@
     pass
 
 ImagePermissionTypeDef = TypedDict(
     "ImagePermissionTypeDef",
     {
         "SharedAccountId": str,
     },
-    total=False,
-)
-
-DescribeWorkspaceImagesRequestDescribeWorkspaceImagesPaginateTypeDef = TypedDict(
-    "DescribeWorkspaceImagesRequestDescribeWorkspaceImagesPaginateTypeDef",
-    {
-        "ImageIds": Sequence[str],
-        "ImageType": ImageTypeType,
-        "PaginationConfig": "PaginatorConfigTypeDef",
-    },
-    total=False,
 )
 
 DescribeWorkspaceImagesRequestRequestTypeDef = TypedDict(
     "DescribeWorkspaceImagesRequestRequestTypeDef",
     {
         "ImageIds": Sequence[str],
         "ImageType": ImageTypeType,
@@ -748,24 +709,14 @@
 )
 
 SnapshotTypeDef = TypedDict(
     "SnapshotTypeDef",
     {
         "SnapshotTime": datetime,
     },
-    total=False,
-)
-
-DescribeWorkspacesConnectionStatusRequestDescribeWorkspacesConnectionStatusPaginateTypeDef = TypedDict(
-    "DescribeWorkspacesConnectionStatusRequestDescribeWorkspacesConnectionStatusPaginateTypeDef",
-    {
-        "WorkspaceIds": Sequence[str],
-        "PaginationConfig": "PaginatorConfigTypeDef",
-    },
-    total=False,
 )
 
 DescribeWorkspacesConnectionStatusRequestRequestTypeDef = TypedDict(
     "DescribeWorkspacesConnectionStatusRequestRequestTypeDef",
     {
         "WorkspaceIds": Sequence[str],
         "NextToken": str,
@@ -777,27 +728,14 @@
     "WorkspaceConnectionStatusTypeDef",
     {
         "WorkspaceId": str,
         "ConnectionState": ConnectionStateType,
         "ConnectionStateCheckTimestamp": datetime,
         "LastKnownUserConnectionTimestamp": datetime,
     },
-    total=False,
-)
-
-DescribeWorkspacesRequestDescribeWorkspacesPaginateTypeDef = TypedDict(
-    "DescribeWorkspacesRequestDescribeWorkspacesPaginateTypeDef",
-    {
-        "WorkspaceIds": Sequence[str],
-        "DirectoryId": str,
-        "UserName": str,
-        "BundleId": str,
-        "PaginationConfig": "PaginatorConfigTypeDef",
-    },
-    total=False,
 )
 
 DescribeWorkspacesRequestRequestTypeDef = TypedDict(
     "DescribeWorkspacesRequestRequestTypeDef",
     {
         "WorkspaceIds": Sequence[str],
         "DirectoryId": str,
@@ -827,15 +765,14 @@
 FailedWorkspaceChangeRequestTypeDef = TypedDict(
     "FailedWorkspaceChangeRequestTypeDef",
     {
         "WorkspaceId": str,
         "ErrorCode": str,
         "ErrorMessage": str,
     },
-    total=False,
 )
 
 IosImportClientBrandingAttributesTypeDef = TypedDict(
     "IosImportClientBrandingAttributesTypeDef",
     {
         "Logo": Union[str, bytes, IO[Any], StreamingBody],
         "Logo2x": Union[str, bytes, IO[Any], StreamingBody],
@@ -844,42 +781,22 @@
         "SupportLink": str,
         "ForgotPasswordLink": str,
         "LoginMessage": Mapping[str, str],
     },
     total=False,
 )
 
-ImportWorkspaceImageResultTypeDef = TypedDict(
-    "ImportWorkspaceImageResultTypeDef",
-    {
-        "ImageId": str,
-        "ResponseMetadata": "ResponseMetadataTypeDef",
-    },
-)
-
-_RequiredListAvailableManagementCidrRangesRequestListAvailableManagementCidrRangesPaginateTypeDef = TypedDict(
-    "_RequiredListAvailableManagementCidrRangesRequestListAvailableManagementCidrRangesPaginateTypeDef",
+IpRuleItemOutputTypeDef = TypedDict(
+    "IpRuleItemOutputTypeDef",
     {
-        "ManagementCidrRangeConstraint": str,
-    },
-)
-_OptionalListAvailableManagementCidrRangesRequestListAvailableManagementCidrRangesPaginateTypeDef = TypedDict(
-    "_OptionalListAvailableManagementCidrRangesRequestListAvailableManagementCidrRangesPaginateTypeDef",
-    {
-        "PaginationConfig": "PaginatorConfigTypeDef",
+        "ipRule": str,
+        "ruleDesc": str,
     },
-    total=False,
 )
 
-class ListAvailableManagementCidrRangesRequestListAvailableManagementCidrRangesPaginateTypeDef(
-    _RequiredListAvailableManagementCidrRangesRequestListAvailableManagementCidrRangesPaginateTypeDef,
-    _OptionalListAvailableManagementCidrRangesRequestListAvailableManagementCidrRangesPaginateTypeDef,
-):
-    pass
-
 _RequiredListAvailableManagementCidrRangesRequestRequestTypeDef = TypedDict(
     "_RequiredListAvailableManagementCidrRangesRequestRequestTypeDef",
     {
         "ManagementCidrRangeConstraint": str,
     },
 )
 _OptionalListAvailableManagementCidrRangesRequestRequestTypeDef = TypedDict(
@@ -893,47 +810,28 @@
 
 class ListAvailableManagementCidrRangesRequestRequestTypeDef(
     _RequiredListAvailableManagementCidrRangesRequestRequestTypeDef,
     _OptionalListAvailableManagementCidrRangesRequestRequestTypeDef,
 ):
     pass
 
-ListAvailableManagementCidrRangesResultTypeDef = TypedDict(
-    "ListAvailableManagementCidrRangesResultTypeDef",
-    {
-        "ManagementCidrRanges": List[str],
-        "NextToken": str,
-        "ResponseMetadata": "ResponseMetadataTypeDef",
-    },
-)
-
 MigrateWorkspaceRequestRequestTypeDef = TypedDict(
     "MigrateWorkspaceRequestRequestTypeDef",
     {
         "SourceWorkspaceId": str,
         "BundleId": str,
     },
 )
 
-MigrateWorkspaceResultTypeDef = TypedDict(
-    "MigrateWorkspaceResultTypeDef",
-    {
-        "SourceWorkspaceId": str,
-        "TargetWorkspaceId": str,
-        "ResponseMetadata": "ResponseMetadataTypeDef",
-    },
-)
-
 ModificationStateTypeDef = TypedDict(
     "ModificationStateTypeDef",
     {
         "Resource": ModificationResourceEnumType,
         "State": ModificationStateEnumType,
     },
-    total=False,
 )
 
 ModifyAccountRequestRequestTypeDef = TypedDict(
     "ModifyAccountRequestRequestTypeDef",
     {
         "DedicatedTenancySupport": Literal["ENABLED"],
         "DedicatedTenancyManagementCidrRange": str,
@@ -1008,24 +906,14 @@
     "ModifyWorkspaceStateRequestRequestTypeDef",
     {
         "WorkspaceId": str,
         "WorkspaceState": TargetWorkspaceStateType,
     },
 )
 
-PaginatorConfigTypeDef = TypedDict(
-    "PaginatorConfigTypeDef",
-    {
-        "MaxItems": int,
-        "PageSize": int,
-        "StartingToken": str,
-    },
-    total=False,
-)
-
 RebootRequestTypeDef = TypedDict(
     "RebootRequestTypeDef",
     {
         "WorkspaceId": str,
     },
 )
 
@@ -1040,26 +928,14 @@
     "RelatedWorkspacePropertiesTypeDef",
     {
         "WorkspaceId": str,
         "Region": str,
         "State": WorkspaceStateType,
         "Type": StandbyWorkspaceRelationshipTypeType,
     },
-    total=False,
-)
-
-ResponseMetadataTypeDef = TypedDict(
-    "ResponseMetadataTypeDef",
-    {
-        "RequestId": str,
-        "HostId": str,
-        "HTTPStatusCode": int,
-        "HTTPHeaders": Dict[str, str],
-        "RetryAttempts": int,
-    },
 )
 
 RestoreWorkspaceRequestRequestTypeDef = TypedDict(
     "RestoreWorkspaceRequestRequestTypeDef",
     {
         "WorkspaceId": str,
     },
@@ -1069,14 +945,41 @@
     "RevokeIpRulesRequestRequestTypeDef",
     {
         "GroupId": str,
         "UserRules": Sequence[str],
     },
 )
 
+RootStorageOutputTypeDef = TypedDict(
+    "RootStorageOutputTypeDef",
+    {
+        "Capacity": str,
+    },
+)
+
+SamlPropertiesOutputTypeDef = TypedDict(
+    "SamlPropertiesOutputTypeDef",
+    {
+        "Status": SamlStatusEnumType,
+        "UserAccessUrl": str,
+        "RelayStateParameterName": str,
+    },
+)
+
+SelfservicePermissionsOutputTypeDef = TypedDict(
+    "SelfservicePermissionsOutputTypeDef",
+    {
+        "RestartWorkspace": ReconnectEnumType,
+        "IncreaseVolumeSize": ReconnectEnumType,
+        "ChangeComputeType": ReconnectEnumType,
+        "SwitchRunningMode": ReconnectEnumType,
+        "RebuildWorkspace": ReconnectEnumType,
+    },
+)
+
 StartRequestTypeDef = TypedDict(
     "StartRequestTypeDef",
     {
         "WorkspaceId": str,
     },
     total=False,
 )
@@ -1120,15 +1023,14 @@
 
 UpdateResultTypeDef = TypedDict(
     "UpdateResultTypeDef",
     {
         "UpdateAvailable": bool,
         "Description": str,
     },
-    total=False,
 )
 
 UpdateWorkspaceBundleRequestRequestTypeDef = TypedDict(
     "UpdateWorkspaceBundleRequestRequestTypeDef",
     {
         "BundleId": str,
         "ImageId": str,
@@ -1141,20 +1043,136 @@
     {
         "ImageId": str,
         "AllowCopyImage": bool,
         "SharedAccountId": str,
     },
 )
 
+UserStorageOutputTypeDef = TypedDict(
+    "UserStorageOutputTypeDef",
+    {
+        "Capacity": str,
+    },
+)
+
+WorkspaceAccessPropertiesOutputTypeDef = TypedDict(
+    "WorkspaceAccessPropertiesOutputTypeDef",
+    {
+        "DeviceTypeWindows": AccessPropertyValueType,
+        "DeviceTypeOsx": AccessPropertyValueType,
+        "DeviceTypeWeb": AccessPropertyValueType,
+        "DeviceTypeIos": AccessPropertyValueType,
+        "DeviceTypeAndroid": AccessPropertyValueType,
+        "DeviceTypeChromeOs": AccessPropertyValueType,
+        "DeviceTypeZeroClient": AccessPropertyValueType,
+        "DeviceTypeLinux": AccessPropertyValueType,
+    },
+)
+
+WorkspacePropertiesOutputTypeDef = TypedDict(
+    "WorkspacePropertiesOutputTypeDef",
+    {
+        "RunningMode": RunningModeType,
+        "RunningModeAutoStopTimeoutInMinutes": int,
+        "RootVolumeSizeGib": int,
+        "UserVolumeSizeGib": int,
+        "ComputeTypeName": ComputeType,
+        "Protocols": List[ProtocolType],
+    },
+)
+
+AssociateConnectionAliasResultTypeDef = TypedDict(
+    "AssociateConnectionAliasResultTypeDef",
+    {
+        "ConnectionIdentifier": str,
+        "ResponseMetadata": ResponseMetadataTypeDef,
+    },
+)
+
+CopyWorkspaceImageResultTypeDef = TypedDict(
+    "CopyWorkspaceImageResultTypeDef",
+    {
+        "ImageId": str,
+        "ResponseMetadata": ResponseMetadataTypeDef,
+    },
+)
+
+CreateConnectClientAddInResultTypeDef = TypedDict(
+    "CreateConnectClientAddInResultTypeDef",
+    {
+        "AddInId": str,
+        "ResponseMetadata": ResponseMetadataTypeDef,
+    },
+)
+
+CreateConnectionAliasResultTypeDef = TypedDict(
+    "CreateConnectionAliasResultTypeDef",
+    {
+        "AliasId": str,
+        "ResponseMetadata": ResponseMetadataTypeDef,
+    },
+)
+
+CreateIpGroupResultTypeDef = TypedDict(
+    "CreateIpGroupResultTypeDef",
+    {
+        "GroupId": str,
+        "ResponseMetadata": ResponseMetadataTypeDef,
+    },
+)
+
+CreateUpdatedWorkspaceImageResultTypeDef = TypedDict(
+    "CreateUpdatedWorkspaceImageResultTypeDef",
+    {
+        "ImageId": str,
+        "ResponseMetadata": ResponseMetadataTypeDef,
+    },
+)
+
 DescribeAccountModificationsResultTypeDef = TypedDict(
     "DescribeAccountModificationsResultTypeDef",
     {
         "AccountModifications": List[AccountModificationTypeDef],
         "NextToken": str,
-        "ResponseMetadata": "ResponseMetadataTypeDef",
+        "ResponseMetadata": ResponseMetadataTypeDef,
+    },
+)
+
+DescribeAccountResultTypeDef = TypedDict(
+    "DescribeAccountResultTypeDef",
+    {
+        "DedicatedTenancySupport": DedicatedTenancySupportResultEnumType,
+        "DedicatedTenancyManagementCidrRange": str,
+        "ResponseMetadata": ResponseMetadataTypeDef,
+    },
+)
+
+ImportWorkspaceImageResultTypeDef = TypedDict(
+    "ImportWorkspaceImageResultTypeDef",
+    {
+        "ImageId": str,
+        "ResponseMetadata": ResponseMetadataTypeDef,
+    },
+)
+
+ListAvailableManagementCidrRangesResultTypeDef = TypedDict(
+    "ListAvailableManagementCidrRangesResultTypeDef",
+    {
+        "ManagementCidrRanges": List[str],
+        "NextToken": str,
+        "ResponseMetadata": ResponseMetadataTypeDef,
+    },
+)
+
+MigrateWorkspaceResultTypeDef = TypedDict(
+    "MigrateWorkspaceResultTypeDef",
+    {
+        "SourceWorkspaceId": str,
+        "TargetWorkspaceId": str,
+        "ResponseMetadata": ResponseMetadataTypeDef,
     },
 )
 
 AuthorizeIpRulesRequestRequestTypeDef = TypedDict(
     "AuthorizeIpRulesRequestRequestTypeDef",
     {
         "GroupId": str,
@@ -1166,25 +1184,14 @@
     "UpdateRulesOfIpGroupRequestRequestTypeDef",
     {
         "GroupId": str,
         "UserRules": Sequence[IpRuleItemTypeDef],
     },
 )
 
-WorkspacesIpGroupTypeDef = TypedDict(
-    "WorkspacesIpGroupTypeDef",
-    {
-        "groupId": str,
-        "groupName": str,
-        "groupDesc": str,
-        "userRules": List[IpRuleItemTypeDef],
-    },
-    total=False,
-)
-
 _RequiredModifyCertificateBasedAuthPropertiesRequestRequestTypeDef = TypedDict(
     "_RequiredModifyCertificateBasedAuthPropertiesRequestRequestTypeDef",
     {
         "ResourceId": str,
     },
 )
 _OptionalModifyCertificateBasedAuthPropertiesRequestRequestTypeDef = TypedDict(
@@ -1204,17 +1211,16 @@
 ):
     pass
 
 ClientPropertiesResultTypeDef = TypedDict(
     "ClientPropertiesResultTypeDef",
     {
         "ResourceId": str,
-        "ClientProperties": ClientPropertiesTypeDef,
+        "ClientProperties": ClientPropertiesOutputTypeDef,
     },
-    total=False,
 )
 
 ModifyClientPropertiesRequestRequestTypeDef = TypedDict(
     "ModifyClientPropertiesRequestRequestTypeDef",
     {
         "ResourceId": str,
         "ClientProperties": ClientPropertiesTypeDef,
@@ -1222,37 +1228,36 @@
 )
 
 DescribeConnectClientAddInsResultTypeDef = TypedDict(
     "DescribeConnectClientAddInsResultTypeDef",
     {
         "AddIns": List[ConnectClientAddInTypeDef],
         "NextToken": str,
-        "ResponseMetadata": "ResponseMetadataTypeDef",
+        "ResponseMetadata": ResponseMetadataTypeDef,
     },
 )
 
 ConnectionAliasTypeDef = TypedDict(
     "ConnectionAliasTypeDef",
     {
         "ConnectionString": str,
         "AliasId": str,
         "State": ConnectionAliasStateType,
         "OwnerAccountId": str,
         "Associations": List[ConnectionAliasAssociationTypeDef],
     },
-    total=False,
 )
 
 DescribeConnectionAliasPermissionsResultTypeDef = TypedDict(
     "DescribeConnectionAliasPermissionsResultTypeDef",
     {
         "AliasId": str,
-        "ConnectionAliasPermissions": List[ConnectionAliasPermissionTypeDef],
+        "ConnectionAliasPermissions": List[ConnectionAliasPermissionOutputTypeDef],
         "NextToken": str,
-        "ResponseMetadata": "ResponseMetadataTypeDef",
+        "ResponseMetadata": ResponseMetadataTypeDef,
     },
 )
 
 UpdateConnectionAliasPermissionRequestRequestTypeDef = TypedDict(
     "UpdateConnectionAliasPermissionRequestRequestTypeDef",
     {
         "AliasId": str,
@@ -1372,22 +1377,14 @@
 
 class CreateWorkspaceImageRequestRequestTypeDef(
     _RequiredCreateWorkspaceImageRequestRequestTypeDef,
     _OptionalCreateWorkspaceImageRequestRequestTypeDef,
 ):
     pass
 
-DescribeTagsResultTypeDef = TypedDict(
-    "DescribeTagsResultTypeDef",
-    {
-        "TagList": List[TagTypeDef],
-        "ResponseMetadata": "ResponseMetadataTypeDef",
-    },
-)
-
 _RequiredImportWorkspaceImageRequestRequestTypeDef = TypedDict(
     "_RequiredImportWorkspaceImageRequestRequestTypeDef",
     {
         "Ec2ImageId": str,
         "IngestionProcess": WorkspaceImageIngestionProcessType,
         "ImageName": str,
         "ImageDescription": str,
@@ -1472,139 +1469,226 @@
 
 class CreateWorkspaceBundleRequestRequestTypeDef(
     _RequiredCreateWorkspaceBundleRequestRequestTypeDef,
     _OptionalCreateWorkspaceBundleRequestRequestTypeDef,
 ):
     pass
 
-WorkspaceBundleTypeDef = TypedDict(
-    "WorkspaceBundleTypeDef",
-    {
-        "BundleId": str,
-        "Name": str,
-        "Owner": str,
-        "Description": str,
-        "ImageId": str,
-        "RootStorage": RootStorageTypeDef,
-        "UserStorage": UserStorageTypeDef,
-        "ComputeType": ComputeTypeTypeDef,
-        "LastUpdatedTime": datetime,
-        "CreationTime": datetime,
-        "State": WorkspaceBundleStateType,
-        "BundleType": BundleTypeType,
-    },
-    total=False,
-)
-
 CreateWorkspaceImageResultTypeDef = TypedDict(
     "CreateWorkspaceImageResultTypeDef",
     {
         "ImageId": str,
         "Name": str,
         "Description": str,
         "OperatingSystem": OperatingSystemTypeDef,
         "State": WorkspaceImageStateType,
         "RequiredTenancy": WorkspaceImageRequiredTenancyType,
         "Created": datetime,
         "OwnerAccountId": str,
-        "ResponseMetadata": "ResponseMetadataTypeDef",
+        "ResponseMetadata": ResponseMetadataTypeDef,
     },
 )
 
+DescribeAccountModificationsRequestDescribeAccountModificationsPaginateTypeDef = TypedDict(
+    "DescribeAccountModificationsRequestDescribeAccountModificationsPaginateTypeDef",
+    {
+        "PaginationConfig": PaginatorConfigTypeDef,
+    },
+    total=False,
+)
+
+DescribeIpGroupsRequestDescribeIpGroupsPaginateTypeDef = TypedDict(
+    "DescribeIpGroupsRequestDescribeIpGroupsPaginateTypeDef",
+    {
+        "GroupIds": Sequence[str],
+        "PaginationConfig": PaginatorConfigTypeDef,
+    },
+    total=False,
+)
+
+DescribeWorkspaceBundlesRequestDescribeWorkspaceBundlesPaginateTypeDef = TypedDict(
+    "DescribeWorkspaceBundlesRequestDescribeWorkspaceBundlesPaginateTypeDef",
+    {
+        "BundleIds": Sequence[str],
+        "Owner": str,
+        "PaginationConfig": PaginatorConfigTypeDef,
+    },
+    total=False,
+)
+
+DescribeWorkspaceDirectoriesRequestDescribeWorkspaceDirectoriesPaginateTypeDef = TypedDict(
+    "DescribeWorkspaceDirectoriesRequestDescribeWorkspaceDirectoriesPaginateTypeDef",
+    {
+        "DirectoryIds": Sequence[str],
+        "Limit": int,
+        "PaginationConfig": PaginatorConfigTypeDef,
+    },
+    total=False,
+)
+
+DescribeWorkspaceImagesRequestDescribeWorkspaceImagesPaginateTypeDef = TypedDict(
+    "DescribeWorkspaceImagesRequestDescribeWorkspaceImagesPaginateTypeDef",
+    {
+        "ImageIds": Sequence[str],
+        "ImageType": ImageTypeType,
+        "PaginationConfig": PaginatorConfigTypeDef,
+    },
+    total=False,
+)
+
+DescribeWorkspacesConnectionStatusRequestDescribeWorkspacesConnectionStatusPaginateTypeDef = TypedDict(
+    "DescribeWorkspacesConnectionStatusRequestDescribeWorkspacesConnectionStatusPaginateTypeDef",
+    {
+        "WorkspaceIds": Sequence[str],
+        "PaginationConfig": PaginatorConfigTypeDef,
+    },
+    total=False,
+)
+
+DescribeWorkspacesRequestDescribeWorkspacesPaginateTypeDef = TypedDict(
+    "DescribeWorkspacesRequestDescribeWorkspacesPaginateTypeDef",
+    {
+        "WorkspaceIds": Sequence[str],
+        "DirectoryId": str,
+        "UserName": str,
+        "BundleId": str,
+        "PaginationConfig": PaginatorConfigTypeDef,
+    },
+    total=False,
+)
+
+_RequiredListAvailableManagementCidrRangesRequestListAvailableManagementCidrRangesPaginateTypeDef = TypedDict(
+    "_RequiredListAvailableManagementCidrRangesRequestListAvailableManagementCidrRangesPaginateTypeDef",
+    {
+        "ManagementCidrRangeConstraint": str,
+    },
+)
+_OptionalListAvailableManagementCidrRangesRequestListAvailableManagementCidrRangesPaginateTypeDef = TypedDict(
+    "_OptionalListAvailableManagementCidrRangesRequestListAvailableManagementCidrRangesPaginateTypeDef",
+    {
+        "PaginationConfig": PaginatorConfigTypeDef,
+    },
+    total=False,
+)
+
+class ListAvailableManagementCidrRangesRequestListAvailableManagementCidrRangesPaginateTypeDef(
+    _RequiredListAvailableManagementCidrRangesRequestListAvailableManagementCidrRangesPaginateTypeDef,
+    _OptionalListAvailableManagementCidrRangesRequestListAvailableManagementCidrRangesPaginateTypeDef,
+):
+    pass
+
 DescribeClientBrandingResultTypeDef = TypedDict(
     "DescribeClientBrandingResultTypeDef",
     {
         "DeviceTypeWindows": DefaultClientBrandingAttributesTypeDef,
         "DeviceTypeOsx": DefaultClientBrandingAttributesTypeDef,
         "DeviceTypeAndroid": DefaultClientBrandingAttributesTypeDef,
         "DeviceTypeIos": IosClientBrandingAttributesTypeDef,
         "DeviceTypeLinux": DefaultClientBrandingAttributesTypeDef,
         "DeviceTypeWeb": DefaultClientBrandingAttributesTypeDef,
-        "ResponseMetadata": "ResponseMetadataTypeDef",
+        "ResponseMetadata": ResponseMetadataTypeDef,
     },
 )
 
 ImportClientBrandingResultTypeDef = TypedDict(
     "ImportClientBrandingResultTypeDef",
     {
         "DeviceTypeWindows": DefaultClientBrandingAttributesTypeDef,
         "DeviceTypeOsx": DefaultClientBrandingAttributesTypeDef,
         "DeviceTypeAndroid": DefaultClientBrandingAttributesTypeDef,
         "DeviceTypeIos": IosClientBrandingAttributesTypeDef,
         "DeviceTypeLinux": DefaultClientBrandingAttributesTypeDef,
         "DeviceTypeWeb": DefaultClientBrandingAttributesTypeDef,
-        "ResponseMetadata": "ResponseMetadataTypeDef",
+        "ResponseMetadata": ResponseMetadataTypeDef,
+    },
+)
+
+DescribeTagsResultTypeDef = TypedDict(
+    "DescribeTagsResultTypeDef",
+    {
+        "TagList": List[TagOutputTypeDef],
+        "ResponseMetadata": ResponseMetadataTypeDef,
+    },
+)
+
+StandbyWorkspaceOutputTypeDef = TypedDict(
+    "StandbyWorkspaceOutputTypeDef",
+    {
+        "PrimaryWorkspaceId": str,
+        "VolumeEncryptionKey": str,
+        "DirectoryId": str,
+        "Tags": List[TagOutputTypeDef],
     },
 )
 
 DescribeWorkspaceImagePermissionsResultTypeDef = TypedDict(
     "DescribeWorkspaceImagePermissionsResultTypeDef",
     {
         "ImageId": str,
         "ImagePermissions": List[ImagePermissionTypeDef],
         "NextToken": str,
-        "ResponseMetadata": "ResponseMetadataTypeDef",
+        "ResponseMetadata": ResponseMetadataTypeDef,
     },
 )
 
 DescribeWorkspaceSnapshotsResultTypeDef = TypedDict(
     "DescribeWorkspaceSnapshotsResultTypeDef",
     {
         "RebuildSnapshots": List[SnapshotTypeDef],
         "RestoreSnapshots": List[SnapshotTypeDef],
-        "ResponseMetadata": "ResponseMetadataTypeDef",
+        "ResponseMetadata": ResponseMetadataTypeDef,
     },
 )
 
 DescribeWorkspacesConnectionStatusResultTypeDef = TypedDict(
     "DescribeWorkspacesConnectionStatusResultTypeDef",
     {
         "WorkspacesConnectionStatus": List[WorkspaceConnectionStatusTypeDef],
         "NextToken": str,
-        "ResponseMetadata": "ResponseMetadataTypeDef",
+        "ResponseMetadata": ResponseMetadataTypeDef,
     },
 )
 
 RebootWorkspacesResultTypeDef = TypedDict(
     "RebootWorkspacesResultTypeDef",
     {
         "FailedRequests": List[FailedWorkspaceChangeRequestTypeDef],
-        "ResponseMetadata": "ResponseMetadataTypeDef",
+        "ResponseMetadata": ResponseMetadataTypeDef,
     },
 )
 
 RebuildWorkspacesResultTypeDef = TypedDict(
     "RebuildWorkspacesResultTypeDef",
     {
         "FailedRequests": List[FailedWorkspaceChangeRequestTypeDef],
-        "ResponseMetadata": "ResponseMetadataTypeDef",
+        "ResponseMetadata": ResponseMetadataTypeDef,
     },
 )
 
 StartWorkspacesResultTypeDef = TypedDict(
     "StartWorkspacesResultTypeDef",
     {
         "FailedRequests": List[FailedWorkspaceChangeRequestTypeDef],
-        "ResponseMetadata": "ResponseMetadataTypeDef",
+        "ResponseMetadata": ResponseMetadataTypeDef,
     },
 )
 
 StopWorkspacesResultTypeDef = TypedDict(
     "StopWorkspacesResultTypeDef",
     {
         "FailedRequests": List[FailedWorkspaceChangeRequestTypeDef],
-        "ResponseMetadata": "ResponseMetadataTypeDef",
+        "ResponseMetadata": ResponseMetadataTypeDef,
     },
 )
 
 TerminateWorkspacesResultTypeDef = TypedDict(
     "TerminateWorkspacesResultTypeDef",
     {
         "FailedRequests": List[FailedWorkspaceChangeRequestTypeDef],
-        "ResponseMetadata": "ResponseMetadataTypeDef",
+        "ResponseMetadata": ResponseMetadataTypeDef,
     },
 )
 
 _RequiredImportClientBrandingRequestRequestTypeDef = TypedDict(
     "_RequiredImportClientBrandingRequestRequestTypeDef",
     {
         "ResourceId": str,
@@ -1625,14 +1709,24 @@
 
 class ImportClientBrandingRequestRequestTypeDef(
     _RequiredImportClientBrandingRequestRequestTypeDef,
     _OptionalImportClientBrandingRequestRequestTypeDef,
 ):
     pass
 
+WorkspacesIpGroupTypeDef = TypedDict(
+    "WorkspacesIpGroupTypeDef",
+    {
+        "groupId": str,
+        "groupName": str,
+        "groupDesc": str,
+        "userRules": List[IpRuleItemOutputTypeDef],
+    },
+)
+
 _RequiredModifySamlPropertiesRequestRequestTypeDef = TypedDict(
     "_RequiredModifySamlPropertiesRequestRequestTypeDef",
     {
         "ResourceId": str,
     },
 )
 _OptionalModifySamlPropertiesRequestRequestTypeDef = TypedDict(
@@ -1662,39 +1756,14 @@
     "ModifyWorkspaceAccessPropertiesRequestRequestTypeDef",
     {
         "ResourceId": str,
         "WorkspaceAccessProperties": WorkspaceAccessPropertiesTypeDef,
     },
 )
 
-WorkspaceDirectoryTypeDef = TypedDict(
-    "WorkspaceDirectoryTypeDef",
-    {
-        "DirectoryId": str,
-        "Alias": str,
-        "DirectoryName": str,
-        "RegistrationCode": str,
-        "SubnetIds": List[str],
-        "DnsIpAddresses": List[str],
-        "CustomerUserName": str,
-        "IamRoleId": str,
-        "DirectoryType": WorkspaceDirectoryTypeType,
-        "WorkspaceSecurityGroupId": str,
-        "State": WorkspaceDirectoryStateType,
-        "WorkspaceCreationProperties": DefaultWorkspaceCreationPropertiesTypeDef,
-        "ipGroupIds": List[str],
-        "WorkspaceAccessProperties": WorkspaceAccessPropertiesTypeDef,
-        "Tenancy": TenancyType,
-        "SelfservicePermissions": SelfservicePermissionsTypeDef,
-        "SamlProperties": SamlPropertiesTypeDef,
-        "CertificateBasedAuthProperties": CertificateBasedAuthPropertiesTypeDef,
-    },
-    total=False,
-)
-
 ModifyWorkspaceCreationPropertiesRequestRequestTypeDef = TypedDict(
     "ModifyWorkspaceCreationPropertiesRequestRequestTypeDef",
     {
         "ResourceId": str,
         "WorkspaceCreationProperties": WorkspaceCreationPropertiesTypeDef,
     },
 )
@@ -1740,37 +1809,14 @@
 RebuildWorkspacesRequestRequestTypeDef = TypedDict(
     "RebuildWorkspacesRequestRequestTypeDef",
     {
         "RebuildWorkspaceRequests": Sequence[RebuildRequestTypeDef],
     },
 )
 
-WorkspaceTypeDef = TypedDict(
-    "WorkspaceTypeDef",
-    {
-        "WorkspaceId": str,
-        "DirectoryId": str,
-        "UserName": str,
-        "IpAddress": str,
-        "State": WorkspaceStateType,
-        "BundleId": str,
-        "SubnetId": str,
-        "ErrorMessage": str,
-        "ErrorCode": str,
-        "ComputerName": str,
-        "VolumeEncryptionKey": str,
-        "UserVolumeEncryptionEnabled": bool,
-        "RootVolumeEncryptionEnabled": bool,
-        "WorkspaceProperties": WorkspacePropertiesTypeDef,
-        "ModificationStates": List[ModificationStateTypeDef],
-        "RelatedWorkspaces": List[RelatedWorkspacePropertiesTypeDef],
-    },
-    total=False,
-)
-
 StartWorkspacesRequestRequestTypeDef = TypedDict(
     "StartWorkspacesRequestRequestTypeDef",
     {
         "StartWorkspaceRequests": Sequence[StartRequestTypeDef],
     },
 )
 
@@ -1799,132 +1845,207 @@
         "RequiredTenancy": WorkspaceImageRequiredTenancyType,
         "ErrorCode": str,
         "ErrorMessage": str,
         "Created": datetime,
         "OwnerAccountId": str,
         "Updates": UpdateResultTypeDef,
     },
-    total=False,
 )
 
-DescribeIpGroupsResultTypeDef = TypedDict(
-    "DescribeIpGroupsResultTypeDef",
+WorkspaceBundleTypeDef = TypedDict(
+    "WorkspaceBundleTypeDef",
     {
-        "Result": List[WorkspacesIpGroupTypeDef],
-        "NextToken": str,
-        "ResponseMetadata": "ResponseMetadataTypeDef",
+        "BundleId": str,
+        "Name": str,
+        "Owner": str,
+        "Description": str,
+        "ImageId": str,
+        "RootStorage": RootStorageOutputTypeDef,
+        "UserStorage": UserStorageOutputTypeDef,
+        "ComputeType": ComputeTypeOutputTypeDef,
+        "LastUpdatedTime": datetime,
+        "CreationTime": datetime,
+        "State": WorkspaceBundleStateType,
+        "BundleType": BundleTypeType,
+    },
+)
+
+WorkspaceDirectoryTypeDef = TypedDict(
+    "WorkspaceDirectoryTypeDef",
+    {
+        "DirectoryId": str,
+        "Alias": str,
+        "DirectoryName": str,
+        "RegistrationCode": str,
+        "SubnetIds": List[str],
+        "DnsIpAddresses": List[str],
+        "CustomerUserName": str,
+        "IamRoleId": str,
+        "DirectoryType": WorkspaceDirectoryTypeType,
+        "WorkspaceSecurityGroupId": str,
+        "State": WorkspaceDirectoryStateType,
+        "WorkspaceCreationProperties": DefaultWorkspaceCreationPropertiesTypeDef,
+        "ipGroupIds": List[str],
+        "WorkspaceAccessProperties": WorkspaceAccessPropertiesOutputTypeDef,
+        "Tenancy": TenancyType,
+        "SelfservicePermissions": SelfservicePermissionsOutputTypeDef,
+        "SamlProperties": SamlPropertiesOutputTypeDef,
+        "CertificateBasedAuthProperties": CertificateBasedAuthPropertiesOutputTypeDef,
+    },
+)
+
+WorkspaceRequestOutputTypeDef = TypedDict(
+    "WorkspaceRequestOutputTypeDef",
+    {
+        "DirectoryId": str,
+        "UserName": str,
+        "BundleId": str,
+        "VolumeEncryptionKey": str,
+        "UserVolumeEncryptionEnabled": bool,
+        "RootVolumeEncryptionEnabled": bool,
+        "WorkspaceProperties": WorkspacePropertiesOutputTypeDef,
+        "Tags": List[TagOutputTypeDef],
+    },
+)
+
+WorkspaceTypeDef = TypedDict(
+    "WorkspaceTypeDef",
+    {
+        "WorkspaceId": str,
+        "DirectoryId": str,
+        "UserName": str,
+        "IpAddress": str,
+        "State": WorkspaceStateType,
+        "BundleId": str,
+        "SubnetId": str,
+        "ErrorMessage": str,
+        "ErrorCode": str,
+        "ComputerName": str,
+        "VolumeEncryptionKey": str,
+        "UserVolumeEncryptionEnabled": bool,
+        "RootVolumeEncryptionEnabled": bool,
+        "WorkspaceProperties": WorkspacePropertiesOutputTypeDef,
+        "ModificationStates": List[ModificationStateTypeDef],
+        "RelatedWorkspaces": List[RelatedWorkspacePropertiesTypeDef],
     },
 )
 
 DescribeClientPropertiesResultTypeDef = TypedDict(
     "DescribeClientPropertiesResultTypeDef",
     {
         "ClientPropertiesList": List[ClientPropertiesResultTypeDef],
-        "ResponseMetadata": "ResponseMetadataTypeDef",
+        "ResponseMetadata": ResponseMetadataTypeDef,
     },
 )
 
 DescribeConnectionAliasesResultTypeDef = TypedDict(
     "DescribeConnectionAliasesResultTypeDef",
     {
         "ConnectionAliases": List[ConnectionAliasTypeDef],
         "NextToken": str,
-        "ResponseMetadata": "ResponseMetadataTypeDef",
+        "ResponseMetadata": ResponseMetadataTypeDef,
     },
 )
 
 CreateStandbyWorkspacesRequestRequestTypeDef = TypedDict(
     "CreateStandbyWorkspacesRequestRequestTypeDef",
     {
         "PrimaryRegion": str,
         "StandbyWorkspaces": Sequence[StandbyWorkspaceTypeDef],
     },
 )
 
 FailedCreateStandbyWorkspacesRequestTypeDef = TypedDict(
     "FailedCreateStandbyWorkspacesRequestTypeDef",
     {
-        "StandbyWorkspaceRequest": StandbyWorkspaceTypeDef,
+        "StandbyWorkspaceRequest": StandbyWorkspaceOutputTypeDef,
         "ErrorCode": str,
         "ErrorMessage": str,
     },
-    total=False,
+)
+
+DescribeIpGroupsResultTypeDef = TypedDict(
+    "DescribeIpGroupsResultTypeDef",
+    {
+        "Result": List[WorkspacesIpGroupTypeDef],
+        "NextToken": str,
+        "ResponseMetadata": ResponseMetadataTypeDef,
+    },
+)
+
+CreateWorkspacesRequestRequestTypeDef = TypedDict(
+    "CreateWorkspacesRequestRequestTypeDef",
+    {
+        "Workspaces": Sequence[WorkspaceRequestTypeDef],
+    },
+)
+
+DescribeWorkspaceImagesResultTypeDef = TypedDict(
+    "DescribeWorkspaceImagesResultTypeDef",
+    {
+        "Images": List[WorkspaceImageTypeDef],
+        "NextToken": str,
+        "ResponseMetadata": ResponseMetadataTypeDef,
+    },
 )
 
 CreateWorkspaceBundleResultTypeDef = TypedDict(
     "CreateWorkspaceBundleResultTypeDef",
     {
         "WorkspaceBundle": WorkspaceBundleTypeDef,
-        "ResponseMetadata": "ResponseMetadataTypeDef",
+        "ResponseMetadata": ResponseMetadataTypeDef,
     },
 )
 
 DescribeWorkspaceBundlesResultTypeDef = TypedDict(
     "DescribeWorkspaceBundlesResultTypeDef",
     {
         "Bundles": List[WorkspaceBundleTypeDef],
         "NextToken": str,
-        "ResponseMetadata": "ResponseMetadataTypeDef",
+        "ResponseMetadata": ResponseMetadataTypeDef,
     },
 )
 
 DescribeWorkspaceDirectoriesResultTypeDef = TypedDict(
     "DescribeWorkspaceDirectoriesResultTypeDef",
     {
         "Directories": List[WorkspaceDirectoryTypeDef],
         "NextToken": str,
-        "ResponseMetadata": "ResponseMetadataTypeDef",
-    },
-)
-
-CreateWorkspacesRequestRequestTypeDef = TypedDict(
-    "CreateWorkspacesRequestRequestTypeDef",
-    {
-        "Workspaces": Sequence[WorkspaceRequestTypeDef],
+        "ResponseMetadata": ResponseMetadataTypeDef,
     },
 )
 
 FailedCreateWorkspaceRequestTypeDef = TypedDict(
     "FailedCreateWorkspaceRequestTypeDef",
     {
-        "WorkspaceRequest": WorkspaceRequestTypeDef,
+        "WorkspaceRequest": WorkspaceRequestOutputTypeDef,
         "ErrorCode": str,
         "ErrorMessage": str,
     },
-    total=False,
 )
 
 DescribeWorkspacesResultTypeDef = TypedDict(
     "DescribeWorkspacesResultTypeDef",
     {
         "Workspaces": List[WorkspaceTypeDef],
         "NextToken": str,
-        "ResponseMetadata": "ResponseMetadataTypeDef",
-    },
-)
-
-DescribeWorkspaceImagesResultTypeDef = TypedDict(
-    "DescribeWorkspaceImagesResultTypeDef",
-    {
-        "Images": List[WorkspaceImageTypeDef],
-        "NextToken": str,
-        "ResponseMetadata": "ResponseMetadataTypeDef",
+        "ResponseMetadata": ResponseMetadataTypeDef,
     },
 )
 
 CreateStandbyWorkspacesResultTypeDef = TypedDict(
     "CreateStandbyWorkspacesResultTypeDef",
     {
         "FailedStandbyRequests": List[FailedCreateStandbyWorkspacesRequestTypeDef],
         "PendingStandbyRequests": List[PendingCreateStandbyWorkspacesRequestTypeDef],
-        "ResponseMetadata": "ResponseMetadataTypeDef",
+        "ResponseMetadata": ResponseMetadataTypeDef,
     },
 )
 
 CreateWorkspacesResultTypeDef = TypedDict(
     "CreateWorkspacesResultTypeDef",
     {
         "FailedRequests": List[FailedCreateWorkspaceRequestTypeDef],
         "PendingRequests": List[WorkspaceTypeDef],
-        "ResponseMetadata": "ResponseMetadataTypeDef",
+        "ResponseMetadata": ResponseMetadataTypeDef,
     },
 )
```

### Comparing `mypy-boto3-workspaces-1.28.0/mypy_boto3_workspaces.egg-info/PKG-INFO` & `mypy-boto3-workspaces-1.28.9/mypy_boto3_workspaces.egg-info/PKG-INFO`

 * *Files 2% similar despite different names*

```diff
@@ -1,11 +1,11 @@
 Metadata-Version: 2.1
 Name: mypy-boto3-workspaces
-Version: 1.28.0
-Summary: Type annotations for boto3.WorkSpaces 1.28.0 service generated with mypy-boto3-builder 7.14.5
+Version: 1.28.9
+Summary: Type annotations for boto3.WorkSpaces 1.28.9 service generated with mypy-boto3-builder 7.15.1
 Home-page: https://github.com/youtype/mypy_boto3_builder
 Author: Vlad Emelianov
 Author-email: vlad.emelianov.nz@gmail.com
 License: MIT License
 Project-URL: Documentation, https://youtype.github.io/boto3_stubs_docs/mypy_boto3_workspaces/
 Project-URL: Source, https://github.com/youtype/mypy_boto3_builder
 Project-URL: Tracker, https://github.com/youtype/mypy_boto3_builder/issues
@@ -38,24 +38,24 @@
 [![PyPI - Python Version](https://img.shields.io/pypi/pyversions/mypy-boto3-workspaces.svg?color=blue)](https://pypi.org/project/mypy-boto3-workspaces)
 [![Docs](https://img.shields.io/readthedocs/boto3-stubs.svg?color=blue)](https://youtype.github.io/boto3_stubs_docs/mypy_boto3_workspaces/)
 [![PyPI - Downloads](https://img.shields.io/pypi/dm/mypy-boto3-workspaces?color=blue)](https://pypistats.org/packages/mypy-boto3-workspaces)
 
 ![boto3.typed](https://github.com/youtype/mypy_boto3_builder/raw/main/logo.png)
 
 Type annotations for
-[boto3.WorkSpaces 1.28.0](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/workspaces.html#WorkSpaces)
+[boto3.WorkSpaces 1.28.9](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/workspaces.html#WorkSpaces)
 service compatible with [VSCode](https://code.visualstudio.com/),
 [PyCharm](https://www.jetbrains.com/pycharm/),
 [Emacs](https://www.gnu.org/software/emacs/),
 [Sublime Text](https://www.sublimetext.com/),
 [mypy](https://github.com/python/mypy),
 [pyright](https://github.com/microsoft/pyright) and other tools.
 
 Generated by
-[mypy-boto3-builder 7.14.5](https://github.com/youtype/mypy_boto3_builder).
+[mypy-boto3-builder 7.15.1](https://github.com/youtype/mypy_boto3_builder).
 
 More information can be found on
 [boto3-stubs](https://pypi.org/project/boto3-stubs/) page and in
 [mypy-boto3-workspaces docs](https://youtype.github.io/boto3_stubs_docs/mypy_boto3_workspaces/).
 
 See how it helps to find and fix potential bugs:
 
@@ -390,165 +390,179 @@
 `mypy_boto3_workspaces.type_defs` module contains structures and shapes
 assembled to typed dictionaries for additional type checking.
 
 ```python
 from mypy_boto3_workspaces.type_defs import (
     AccountModificationTypeDef,
     AssociateConnectionAliasRequestRequestTypeDef,
-    AssociateConnectionAliasResultTypeDef,
+    ResponseMetadataTypeDef,
     AssociateIpGroupsRequestRequestTypeDef,
     IpRuleItemTypeDef,
+    CertificateBasedAuthPropertiesOutputTypeDef,
     CertificateBasedAuthPropertiesTypeDef,
+    ClientPropertiesOutputTypeDef,
     ClientPropertiesTypeDef,
+    ComputeTypeOutputTypeDef,
     ComputeTypeTypeDef,
     ConnectClientAddInTypeDef,
     ConnectionAliasAssociationTypeDef,
+    ConnectionAliasPermissionOutputTypeDef,
     ConnectionAliasPermissionTypeDef,
     TagTypeDef,
-    CopyWorkspaceImageResultTypeDef,
     CreateConnectClientAddInRequestRequestTypeDef,
-    CreateConnectClientAddInResultTypeDef,
-    CreateConnectionAliasResultTypeDef,
-    CreateIpGroupResultTypeDef,
     PendingCreateStandbyWorkspacesRequestTypeDef,
-    CreateUpdatedWorkspaceImageResultTypeDef,
     RootStorageTypeDef,
     UserStorageTypeDef,
     OperatingSystemTypeDef,
     DefaultClientBrandingAttributesTypeDef,
     DefaultImportClientBrandingAttributesTypeDef,
     DefaultWorkspaceCreationPropertiesTypeDef,
     DeleteClientBrandingRequestRequestTypeDef,
     DeleteConnectClientAddInRequestRequestTypeDef,
     DeleteConnectionAliasRequestRequestTypeDef,
     DeleteIpGroupRequestRequestTypeDef,
     DeleteTagsRequestRequestTypeDef,
     DeleteWorkspaceBundleRequestRequestTypeDef,
     DeleteWorkspaceImageRequestRequestTypeDef,
     DeregisterWorkspaceDirectoryRequestRequestTypeDef,
-    DescribeAccountModificationsRequestDescribeAccountModificationsPaginateTypeDef,
+    PaginatorConfigTypeDef,
     DescribeAccountModificationsRequestRequestTypeDef,
-    DescribeAccountResultTypeDef,
     DescribeClientBrandingRequestRequestTypeDef,
     IosClientBrandingAttributesTypeDef,
     DescribeClientPropertiesRequestRequestTypeDef,
     DescribeConnectClientAddInsRequestRequestTypeDef,
     DescribeConnectionAliasPermissionsRequestRequestTypeDef,
     DescribeConnectionAliasesRequestRequestTypeDef,
-    DescribeIpGroupsRequestDescribeIpGroupsPaginateTypeDef,
     DescribeIpGroupsRequestRequestTypeDef,
     DescribeTagsRequestRequestTypeDef,
-    DescribeWorkspaceBundlesRequestDescribeWorkspaceBundlesPaginateTypeDef,
+    TagOutputTypeDef,
     DescribeWorkspaceBundlesRequestRequestTypeDef,
-    DescribeWorkspaceDirectoriesRequestDescribeWorkspaceDirectoriesPaginateTypeDef,
     DescribeWorkspaceDirectoriesRequestRequestTypeDef,
     DescribeWorkspaceImagePermissionsRequestRequestTypeDef,
     ImagePermissionTypeDef,
-    DescribeWorkspaceImagesRequestDescribeWorkspaceImagesPaginateTypeDef,
     DescribeWorkspaceImagesRequestRequestTypeDef,
     DescribeWorkspaceSnapshotsRequestRequestTypeDef,
     SnapshotTypeDef,
-    DescribeWorkspacesConnectionStatusRequestDescribeWorkspacesConnectionStatusPaginateTypeDef,
     DescribeWorkspacesConnectionStatusRequestRequestTypeDef,
     WorkspaceConnectionStatusTypeDef,
-    DescribeWorkspacesRequestDescribeWorkspacesPaginateTypeDef,
     DescribeWorkspacesRequestRequestTypeDef,
     DisassociateConnectionAliasRequestRequestTypeDef,
     DisassociateIpGroupsRequestRequestTypeDef,
     FailedWorkspaceChangeRequestTypeDef,
     IosImportClientBrandingAttributesTypeDef,
-    ImportWorkspaceImageResultTypeDef,
-    ListAvailableManagementCidrRangesRequestListAvailableManagementCidrRangesPaginateTypeDef,
+    IpRuleItemOutputTypeDef,
     ListAvailableManagementCidrRangesRequestRequestTypeDef,
-    ListAvailableManagementCidrRangesResultTypeDef,
     MigrateWorkspaceRequestRequestTypeDef,
-    MigrateWorkspaceResultTypeDef,
     ModificationStateTypeDef,
     ModifyAccountRequestRequestTypeDef,
     SamlPropertiesTypeDef,
     SelfservicePermissionsTypeDef,
     WorkspaceAccessPropertiesTypeDef,
     WorkspaceCreationPropertiesTypeDef,
     WorkspacePropertiesTypeDef,
     ModifyWorkspaceStateRequestRequestTypeDef,
-    PaginatorConfigTypeDef,
     RebootRequestTypeDef,
     RebuildRequestTypeDef,
     RelatedWorkspacePropertiesTypeDef,
-    ResponseMetadataTypeDef,
     RestoreWorkspaceRequestRequestTypeDef,
     RevokeIpRulesRequestRequestTypeDef,
+    RootStorageOutputTypeDef,
+    SamlPropertiesOutputTypeDef,
+    SelfservicePermissionsOutputTypeDef,
     StartRequestTypeDef,
     StopRequestTypeDef,
     TerminateRequestTypeDef,
     UpdateConnectClientAddInRequestRequestTypeDef,
     UpdateResultTypeDef,
     UpdateWorkspaceBundleRequestRequestTypeDef,
     UpdateWorkspaceImagePermissionRequestRequestTypeDef,
+    UserStorageOutputTypeDef,
+    WorkspaceAccessPropertiesOutputTypeDef,
+    WorkspacePropertiesOutputTypeDef,
+    AssociateConnectionAliasResultTypeDef,
+    CopyWorkspaceImageResultTypeDef,
+    CreateConnectClientAddInResultTypeDef,
+    CreateConnectionAliasResultTypeDef,
+    CreateIpGroupResultTypeDef,
+    CreateUpdatedWorkspaceImageResultTypeDef,
     DescribeAccountModificationsResultTypeDef,
+    DescribeAccountResultTypeDef,
+    ImportWorkspaceImageResultTypeDef,
+    ListAvailableManagementCidrRangesResultTypeDef,
+    MigrateWorkspaceResultTypeDef,
     AuthorizeIpRulesRequestRequestTypeDef,
     UpdateRulesOfIpGroupRequestRequestTypeDef,
-    WorkspacesIpGroupTypeDef,
     ModifyCertificateBasedAuthPropertiesRequestRequestTypeDef,
     ClientPropertiesResultTypeDef,
     ModifyClientPropertiesRequestRequestTypeDef,
     DescribeConnectClientAddInsResultTypeDef,
     ConnectionAliasTypeDef,
     DescribeConnectionAliasPermissionsResultTypeDef,
     UpdateConnectionAliasPermissionRequestRequestTypeDef,
     CopyWorkspaceImageRequestRequestTypeDef,
     CreateConnectionAliasRequestRequestTypeDef,
     CreateIpGroupRequestRequestTypeDef,
     CreateTagsRequestRequestTypeDef,
     CreateUpdatedWorkspaceImageRequestRequestTypeDef,
     CreateWorkspaceImageRequestRequestTypeDef,
-    DescribeTagsResultTypeDef,
     ImportWorkspaceImageRequestRequestTypeDef,
     RegisterWorkspaceDirectoryRequestRequestTypeDef,
     StandbyWorkspaceTypeDef,
     CreateWorkspaceBundleRequestRequestTypeDef,
-    WorkspaceBundleTypeDef,
     CreateWorkspaceImageResultTypeDef,
+    DescribeAccountModificationsRequestDescribeAccountModificationsPaginateTypeDef,
+    DescribeIpGroupsRequestDescribeIpGroupsPaginateTypeDef,
+    DescribeWorkspaceBundlesRequestDescribeWorkspaceBundlesPaginateTypeDef,
+    DescribeWorkspaceDirectoriesRequestDescribeWorkspaceDirectoriesPaginateTypeDef,
+    DescribeWorkspaceImagesRequestDescribeWorkspaceImagesPaginateTypeDef,
+    DescribeWorkspacesConnectionStatusRequestDescribeWorkspacesConnectionStatusPaginateTypeDef,
+    DescribeWorkspacesRequestDescribeWorkspacesPaginateTypeDef,
+    ListAvailableManagementCidrRangesRequestListAvailableManagementCidrRangesPaginateTypeDef,
     DescribeClientBrandingResultTypeDef,
     ImportClientBrandingResultTypeDef,
+    DescribeTagsResultTypeDef,
+    StandbyWorkspaceOutputTypeDef,
     DescribeWorkspaceImagePermissionsResultTypeDef,
     DescribeWorkspaceSnapshotsResultTypeDef,
     DescribeWorkspacesConnectionStatusResultTypeDef,
     RebootWorkspacesResultTypeDef,
     RebuildWorkspacesResultTypeDef,
     StartWorkspacesResultTypeDef,
     StopWorkspacesResultTypeDef,
     TerminateWorkspacesResultTypeDef,
     ImportClientBrandingRequestRequestTypeDef,
+    WorkspacesIpGroupTypeDef,
     ModifySamlPropertiesRequestRequestTypeDef,
     ModifySelfservicePermissionsRequestRequestTypeDef,
     ModifyWorkspaceAccessPropertiesRequestRequestTypeDef,
-    WorkspaceDirectoryTypeDef,
     ModifyWorkspaceCreationPropertiesRequestRequestTypeDef,
     ModifyWorkspacePropertiesRequestRequestTypeDef,
     WorkspaceRequestTypeDef,
     RebootWorkspacesRequestRequestTypeDef,
     RebuildWorkspacesRequestRequestTypeDef,
-    WorkspaceTypeDef,
     StartWorkspacesRequestRequestTypeDef,
     StopWorkspacesRequestRequestTypeDef,
     TerminateWorkspacesRequestRequestTypeDef,
     WorkspaceImageTypeDef,
-    DescribeIpGroupsResultTypeDef,
+    WorkspaceBundleTypeDef,
+    WorkspaceDirectoryTypeDef,
+    WorkspaceRequestOutputTypeDef,
+    WorkspaceTypeDef,
     DescribeClientPropertiesResultTypeDef,
     DescribeConnectionAliasesResultTypeDef,
     CreateStandbyWorkspacesRequestRequestTypeDef,
     FailedCreateStandbyWorkspacesRequestTypeDef,
+    DescribeIpGroupsResultTypeDef,
+    CreateWorkspacesRequestRequestTypeDef,
+    DescribeWorkspaceImagesResultTypeDef,
     CreateWorkspaceBundleResultTypeDef,
     DescribeWorkspaceBundlesResultTypeDef,
     DescribeWorkspaceDirectoriesResultTypeDef,
-    CreateWorkspacesRequestRequestTypeDef,
     FailedCreateWorkspaceRequestTypeDef,
     DescribeWorkspacesResultTypeDef,
-    DescribeWorkspaceImagesResultTypeDef,
     CreateStandbyWorkspacesResultTypeDef,
     CreateWorkspacesResultTypeDef,
 )
 
 
 def get_structure() -> AccountModificationTypeDef:
     return {...}
```

### Comparing `mypy-boto3-workspaces-1.28.0/mypy_boto3_workspaces.egg-info/SOURCES.txt` & `mypy-boto3-workspaces-1.28.9/mypy_boto3_workspaces.egg-info/SOURCES.txt`

 * *Files identical despite different names*

### Comparing `mypy-boto3-workspaces-1.28.0/setup.py` & `mypy-boto3-workspaces-1.28.9/setup.py`

 * *Files 2% similar despite different names*

```diff
@@ -6,23 +6,23 @@
 from setuptools import setup
 
 LONG_DESCRIPTION = (Path(__file__).parent / "README.md").read_text()
 
 
 setup(
     name="mypy-boto3-workspaces",
-    version="1.28.0",
+    version="1.28.9",
     packages=["mypy_boto3_workspaces"],
     url="https://github.com/youtype/mypy_boto3_builder",
     license="MIT License",
     author="Vlad Emelianov",
     author_email="vlad.emelianov.nz@gmail.com",
     description=(
-        "Type annotations for boto3.WorkSpaces 1.28.0 service generated with mypy-boto3-builder"
-        " 7.14.5"
+        "Type annotations for boto3.WorkSpaces 1.28.9 service generated with mypy-boto3-builder"
+        " 7.15.1"
     ),
     classifiers=[
         "Development Status :: 5 - Production/Stable",
         "Intended Audience :: Developers",
         "Environment :: Console",
         "License :: OSI Approved :: MIT License",
         "Natural Language :: English",
```

