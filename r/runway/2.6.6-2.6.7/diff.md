# Comparing `tmp/runway-2.6.6.tar.gz` & `tmp/runway-2.6.7.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "runway-2.6.6.tar", max compression
+gzip compressed data, was "runway-2.6.7.tar", max compression
```

## Comparing `runway-2.6.6.tar` & `runway-2.6.7.tar`

### file list

```diff
@@ -1,472 +1,472 @@
--rw-r--r--   0        0        0    11346 2023-05-26 23:21:54.305109 runway-2.6.6/LICENSE
--rw-r--r--   0        0        0     3587 2023-05-26 23:21:54.305109 runway-2.6.6/README.md
--rw-r--r--   0        0        0    10042 2023-05-26 23:22:30.925583 runway-2.6.6/pyproject.toml
--rw-r--r--   0        0        0      550 2023-05-26 23:21:54.337110 runway-2.6.6/runway/__init__.py
--rw-r--r--   0        0        0       59 2023-05-26 23:21:54.337110 runway-2.6.6/runway/_cli/__init__.py
--rw-r--r--   0        0        0      824 2023-05-26 23:21:54.337110 runway-2.6.6/runway/_cli/commands/__init__.py
--rw-r--r--   0        0        0     1692 2023-05-26 23:21:54.337110 runway-2.6.6/runway/_cli/commands/_deploy.py
--rw-r--r--   0        0        0     2192 2023-05-26 23:21:54.337110 runway-2.6.6/runway/_cli/commands/_destroy.py
--rw-r--r--   0        0        0      796 2023-05-26 23:21:54.337110 runway-2.6.6/runway/_cli/commands/_dismantle.py
--rw-r--r--   0        0        0     1464 2023-05-26 23:21:54.337110 runway-2.6.6/runway/_cli/commands/_docs.py
--rw-r--r--   0        0        0     2727 2023-05-26 23:21:54.337110 runway-2.6.6/runway/_cli/commands/_envvars.py
--rw-r--r--   0        0        0     1472 2023-05-26 23:21:54.337110 runway-2.6.6/runway/_cli/commands/_gen_sample/__init__.py
--rw-r--r--   0        0        0     1002 2023-05-26 23:21:54.337110 runway-2.6.6/runway/_cli/commands/_gen_sample/_cdk_csharp.py
--rw-r--r--   0        0        0      953 2023-05-26 23:21:54.337110 runway-2.6.6/runway/_cli/commands/_gen_sample/_cdk_py.py
--rw-r--r--   0        0        0      962 2023-05-26 23:21:54.337110 runway-2.6.6/runway/_cli/commands/_gen_sample/_cdk_tsc.py
--rw-r--r--   0        0        0      926 2023-05-26 23:21:54.337110 runway-2.6.6/runway/_cli/commands/_gen_sample/_cfn.py
--rw-r--r--   0        0        0     1226 2023-05-26 23:21:54.337110 runway-2.6.6/runway/_cli/commands/_gen_sample/_cfngin.py
--rw-r--r--   0        0        0     2068 2023-05-26 23:21:54.337110 runway-2.6.6/runway/_cli/commands/_gen_sample/_k8s_cfn_repo.py
--rw-r--r--   0        0        0     1921 2023-05-26 23:21:54.337110 runway-2.6.6/runway/_cli/commands/_gen_sample/_k8s_flux_repo.py
--rw-r--r--   0        0        0     1417 2023-05-26 23:21:54.337110 runway-2.6.6/runway/_cli/commands/_gen_sample/_k8s_tf_repo.py
--rw-r--r--   0        0        0      998 2023-05-26 23:21:54.337110 runway-2.6.6/runway/_cli/commands/_gen_sample/_sls_py.py
--rw-r--r--   0        0        0     1003 2023-05-26 23:21:54.337110 runway-2.6.6/runway/_cli/commands/_gen_sample/_sls_tsc.py
--rw-r--r--   0        0        0      973 2023-05-26 23:21:54.337110 runway-2.6.6/runway/_cli/commands/_gen_sample/_static_angular.py
--rw-r--r--   0        0        0      879 2023-05-26 23:21:54.337110 runway-2.6.6/runway/_cli/commands/_gen_sample/_static_react.py
--rw-r--r--   0        0        0     1050 2023-05-26 23:21:54.337110 runway-2.6.6/runway/_cli/commands/_gen_sample/_tf.py
--rw-r--r--   0        0        0     1748 2023-05-26 23:21:54.337110 runway-2.6.6/runway/_cli/commands/_gen_sample/utils.py
--rw-r--r--   0        0        0     2106 2023-05-26 23:21:54.337110 runway-2.6.6/runway/_cli/commands/_init.py
--rw-r--r--   0        0        0      739 2023-05-26 23:21:54.337110 runway-2.6.6/runway/_cli/commands/_kbenv/__init__.py
--rw-r--r--   0        0        0      889 2023-05-26 23:21:54.337110 runway-2.6.6/runway/_cli/commands/_kbenv/_install.py
--rw-r--r--   0        0        0      892 2023-05-26 23:21:54.337110 runway-2.6.6/runway/_cli/commands/_kbenv/_list.py
--rw-r--r--   0        0        0      919 2023-05-26 23:21:54.337110 runway-2.6.6/runway/_cli/commands/_kbenv/_run.py
--rw-r--r--   0        0        0     1851 2023-05-26 23:21:54.337110 runway-2.6.6/runway/_cli/commands/_kbenv/_uninstall.py
--rw-r--r--   0        0        0     1395 2023-05-26 23:21:54.337110 runway-2.6.6/runway/_cli/commands/_new.py
--rw-r--r--   0        0        0     1739 2023-05-26 23:21:54.337110 runway-2.6.6/runway/_cli/commands/_plan.py
--rw-r--r--   0        0        0      749 2023-05-26 23:21:54.337110 runway-2.6.6/runway/_cli/commands/_preflight.py
--rw-r--r--   0        0        0     1207 2023-05-26 23:21:54.337110 runway-2.6.6/runway/_cli/commands/_run_python.py
--rw-r--r--   0        0        0      460 2023-05-26 23:21:54.337110 runway-2.6.6/runway/_cli/commands/_schema/__init__.py
--rw-r--r--   0        0        0     1635 2023-05-26 23:21:54.337110 runway-2.6.6/runway/_cli/commands/_schema/_cfngin.py
--rw-r--r--   0        0        0     1631 2023-05-26 23:21:54.337110 runway-2.6.6/runway/_cli/commands/_schema/_runway.py
--rw-r--r--   0        0        0      783 2023-05-26 23:21:54.337110 runway-2.6.6/runway/_cli/commands/_takeoff.py
--rw-r--r--   0        0        0      760 2023-05-26 23:21:54.337110 runway-2.6.6/runway/_cli/commands/_taxi.py
--rw-r--r--   0        0        0      852 2023-05-26 23:21:54.337110 runway-2.6.6/runway/_cli/commands/_test.py
--rw-r--r--   0        0        0      924 2023-05-26 23:21:54.337110 runway-2.6.6/runway/_cli/commands/_tfenv/__init__.py
--rw-r--r--   0        0        0     1628 2023-05-26 23:21:54.337110 runway-2.6.6/runway/_cli/commands/_tfenv/_install.py
--rw-r--r--   0        0        0      900 2023-05-26 23:21:54.337110 runway-2.6.6/runway/_cli/commands/_tfenv/_list.py
--rw-r--r--   0        0        0     1611 2023-05-26 23:21:54.337110 runway-2.6.6/runway/_cli/commands/_tfenv/_run.py
--rw-r--r--   0        0        0     1721 2023-05-26 23:21:54.337110 runway-2.6.6/runway/_cli/commands/_tfenv/_uninstall.py
--rw-r--r--   0        0        0     1020 2023-05-26 23:21:54.337110 runway-2.6.6/runway/_cli/commands/_whichenv.py
--rw-r--r--   0        0        0     4394 2023-05-26 23:21:54.337110 runway-2.6.6/runway/_cli/logs.py
--rw-r--r--   0        0        0     2536 2023-05-26 23:21:54.337110 runway-2.6.6/runway/_cli/main.py
--rw-r--r--   0        0        0     1175 2023-05-26 23:21:54.337110 runway-2.6.6/runway/_cli/options.py
--rw-r--r--   0        0        0     9419 2023-05-26 23:21:54.337110 runway-2.6.6/runway/_cli/utils.py
--rw-r--r--   0        0        0     4463 2023-05-26 23:21:54.337110 runway-2.6.6/runway/_logging.py
--rw-r--r--   0        0        0      884 2023-05-26 23:21:54.337110 runway-2.6.6/runway/aws_sso_botocore/__init__.py
--rw-r--r--   0        0        0    11021 2023-05-26 23:21:54.341110 runway-2.6.6/runway/aws_sso_botocore/credentials.py
--rw-r--r--   0        0        0     1523 2023-05-26 23:21:54.341110 runway-2.6.6/runway/aws_sso_botocore/exceptions.py
--rw-r--r--   0        0        0     1061 2023-05-26 23:21:54.341110 runway-2.6.6/runway/aws_sso_botocore/session.py
--rw-r--r--   0        0        0     1616 2023-05-26 23:21:54.341110 runway-2.6.6/runway/aws_sso_botocore/util.py
--rw-r--r--   0        0        0       46 2023-05-26 23:21:54.341110 runway-2.6.6/runway/blueprints/__init__.py
--rw-r--r--   0        0        0       46 2023-05-26 23:21:54.341110 runway-2.6.6/runway/blueprints/k8s/__init__.py
--rwxr-xr-x   0        0        0     3943 2023-05-26 23:21:54.341110 runway-2.6.6/runway/blueprints/k8s/k8s_iam.py
--rwxr-xr-x   0        0        0     6214 2023-05-26 23:21:54.341110 runway-2.6.6/runway/blueprints/k8s/k8s_master.py
--rwxr-xr-x   0        0        0    14269 2023-05-26 23:21:54.341110 runway-2.6.6/runway/blueprints/k8s/k8s_workers.py
--rw-r--r--   0        0        0       46 2023-05-26 23:21:54.341110 runway-2.6.6/runway/blueprints/staticsite/__init__.py
--rw-r--r--   0        0        0    15799 2023-05-26 23:21:54.341110 runway-2.6.6/runway/blueprints/staticsite/auth_at_edge.py
--rwxr-xr-x   0        0        0     7147 2023-05-26 23:21:54.341110 runway-2.6.6/runway/blueprints/staticsite/dependencies.py
--rwxr-xr-x   0        0        0    21988 2023-05-26 23:21:54.341110 runway-2.6.6/runway/blueprints/staticsite/staticsite.py
--rw-r--r--   0        0        0      767 2023-05-26 23:21:54.341110 runway-2.6.6/runway/blueprints/staticsite/templates/cf_directory_index_rewrite.template.js
--rwxr-xr-x   0        0        0     6045 2023-05-26 23:21:54.341110 runway-2.6.6/runway/blueprints/tf_state.py
--rw-r--r--   0        0        0     1303 2023-05-26 23:21:54.341110 runway-2.6.6/runway/cfngin/LICENSE
--rw-r--r--   0        0        0       46 2023-05-26 23:21:54.341110 runway-2.6.6/runway/cfngin/__init__.py
--rw-r--r--   0        0        0       22 2023-05-26 23:21:54.341110 runway-2.6.6/runway/cfngin/actions/__init__.py
--rw-r--r--   0        0        0    10343 2023-05-26 23:21:54.341110 runway-2.6.6/runway/cfngin/actions/base.py
--rw-r--r--   0        0        0    22364 2023-05-26 23:21:54.341110 runway-2.6.6/runway/cfngin/actions/deploy.py
--rw-r--r--   0        0        0     5173 2023-05-26 23:21:54.341110 runway-2.6.6/runway/cfngin/actions/destroy.py
--rw-r--r--   0        0        0     9515 2023-05-26 23:21:54.341110 runway-2.6.6/runway/cfngin/actions/diff.py
--rw-r--r--   0        0        0     3044 2023-05-26 23:21:54.341110 runway-2.6.6/runway/cfngin/actions/graph.py
--rw-r--r--   0        0        0     1313 2023-05-26 23:21:54.341110 runway-2.6.6/runway/cfngin/actions/info.py
--rw-r--r--   0        0        0     5141 2023-05-26 23:21:54.341110 runway-2.6.6/runway/cfngin/actions/init.py
--rw-r--r--   0        0        0     2715 2023-05-26 23:21:54.341110 runway-2.6.6/runway/cfngin/awscli_yamlhelper.py
--rw-r--r--   0        0        0       22 2023-05-26 23:21:54.341110 runway-2.6.6/runway/cfngin/blueprints/__init__.py
--rw-r--r--   0        0        0    25454 2023-05-26 23:21:54.341110 runway-2.6.6/runway/cfngin/blueprints/base.py
--rw-r--r--   0        0        0     4140 2023-05-26 23:21:54.341110 runway-2.6.6/runway/cfngin/blueprints/cfngin_bucket.py
--rw-r--r--   0        0        0     8979 2023-05-26 23:21:54.341110 runway-2.6.6/runway/cfngin/blueprints/raw.py
--rw-r--r--   0        0        0     7129 2023-05-26 23:21:54.341110 runway-2.6.6/runway/cfngin/blueprints/testutil.py
--rw-r--r--   0        0        0     3658 2023-05-26 23:21:54.341110 runway-2.6.6/runway/cfngin/blueprints/type_defs.py
--rw-r--r--   0        0        0       22 2023-05-26 23:21:54.341110 runway-2.6.6/runway/cfngin/blueprints/variables/__init__.py
--rw-r--r--   0        0        0    18899 2023-05-26 23:21:54.341110 runway-2.6.6/runway/cfngin/blueprints/variables/types.py
--rw-r--r--   0        0        0    12931 2023-05-26 23:21:54.341110 runway-2.6.6/runway/cfngin/cfngin.py
--rw-r--r--   0        0        0    15228 2023-05-26 23:21:54.341110 runway-2.6.6/runway/cfngin/dag/__init__.py
--rw-r--r--   0        0        0      695 2023-05-26 23:21:54.341110 runway-2.6.6/runway/cfngin/environment.py
--rw-r--r--   0        0        0    18609 2023-05-26 23:21:54.341110 runway-2.6.6/runway/cfngin/exceptions.py
--rw-r--r--   0        0        0       22 2023-05-26 23:21:54.341110 runway-2.6.6/runway/cfngin/hooks/__init__.py
--rw-r--r--   0        0        0    17562 2023-05-26 23:21:54.341110 runway-2.6.6/runway/cfngin/hooks/acm.py
--rw-r--r--   0        0        0    41530 2023-05-26 23:21:54.341110 runway-2.6.6/runway/cfngin/hooks/aws_lambda.py
--rw-r--r--   0        0        0      483 2023-05-26 23:21:54.341110 runway-2.6.6/runway/cfngin/hooks/awslambda/__init__.py
--rw-r--r--   0        0        0     2408 2023-05-26 23:21:54.341110 runway-2.6.6/runway/cfngin/hooks/awslambda/_python_hooks.py
--rw-r--r--   0        0        0    16927 2023-05-26 23:21:54.345110 runway-2.6.6/runway/cfngin/hooks/awslambda/base_classes.py
--rw-r--r--   0        0        0      350 2023-05-26 23:21:54.345110 runway-2.6.6/runway/cfngin/hooks/awslambda/constants.py
--rw-r--r--   0        0        0    24668 2023-05-26 23:21:54.345110 runway-2.6.6/runway/cfngin/hooks/awslambda/deployment_package.py
--rw-r--r--   0        0        0    13239 2023-05-26 23:21:54.345110 runway-2.6.6/runway/cfngin/hooks/awslambda/docker.py
--rw-r--r--   0        0        0     1825 2023-05-26 23:21:54.345110 runway-2.6.6/runway/cfngin/hooks/awslambda/exceptions.py
--rw-r--r--   0        0        0       19 2023-05-26 23:21:54.345110 runway-2.6.6/runway/cfngin/hooks/awslambda/models/__init__.py
--rw-r--r--   0        0        0     9710 2023-05-26 23:21:54.345110 runway-2.6.6/runway/cfngin/hooks/awslambda/models/args.py
--rw-r--r--   0        0        0     2628 2023-05-26 23:21:54.345110 runway-2.6.6/runway/cfngin/hooks/awslambda/models/responses.py
--rw-r--r--   0        0        0      286 2023-05-26 23:21:54.345110 runway-2.6.6/runway/cfngin/hooks/awslambda/python_requirements/__init__.py
--rw-r--r--   0        0        0     1769 2023-05-26 23:21:54.345110 runway-2.6.6/runway/cfngin/hooks/awslambda/python_requirements/_deployment_package.py
--rw-r--r--   0        0        0     3594 2023-05-26 23:21:54.345110 runway-2.6.6/runway/cfngin/hooks/awslambda/python_requirements/_docker.py
--rw-r--r--   0        0        0     6717 2023-05-26 23:21:54.345110 runway-2.6.6/runway/cfngin/hooks/awslambda/python_requirements/_project.py
--rw-r--r--   0        0        0     5134 2023-05-26 23:21:54.345110 runway-2.6.6/runway/cfngin/hooks/awslambda/source_code.py
--rw-r--r--   0        0        0      423 2023-05-26 23:21:54.345110 runway-2.6.6/runway/cfngin/hooks/awslambda/type_defs.py
--rw-r--r--   0        0        0     9394 2023-05-26 23:21:54.345110 runway-2.6.6/runway/cfngin/hooks/base.py
--rw-r--r--   0        0        0     1157 2023-05-26 23:21:54.345110 runway-2.6.6/runway/cfngin/hooks/cleanup_s3.py
--rw-r--r--   0        0        0      895 2023-05-26 23:21:54.345110 runway-2.6.6/runway/cfngin/hooks/cleanup_ssm.py
--rw-r--r--   0        0        0     4765 2023-05-26 23:21:54.345110 runway-2.6.6/runway/cfngin/hooks/command.py
--rw-r--r--   0        0        0       90 2023-05-26 23:21:54.345110 runway-2.6.6/runway/cfngin/hooks/docker/__init__.py
--rw-r--r--   0        0        0     2341 2023-05-26 23:21:54.345110 runway-2.6.6/runway/cfngin/hooks/docker/_login.py
--rw-r--r--   0        0        0     4060 2023-05-26 23:21:54.345110 runway-2.6.6/runway/cfngin/hooks/docker/data_models.py
--rw-r--r--   0        0        0     1475 2023-05-26 23:21:54.345110 runway-2.6.6/runway/cfngin/hooks/docker/hook_data.py
--rw-r--r--   0        0        0      421 2023-05-26 23:21:54.345110 runway-2.6.6/runway/cfngin/hooks/docker/image/__init__.py
--rw-r--r--   0        0        0     6815 2023-05-26 23:21:54.345110 runway-2.6.6/runway/cfngin/hooks/docker/image/_build.py
--rw-r--r--   0        0        0     3744 2023-05-26 23:21:54.345110 runway-2.6.6/runway/cfngin/hooks/docker/image/_push.py
--rw-r--r--   0        0        0     4357 2023-05-26 23:21:54.345110 runway-2.6.6/runway/cfngin/hooks/docker/image/_remove.py
--rw-r--r--   0        0        0      129 2023-05-26 23:21:54.345110 runway-2.6.6/runway/cfngin/hooks/ecr/__init__.py
--rw-r--r--   0        0        0     2983 2023-05-26 23:21:54.345110 runway-2.6.6/runway/cfngin/hooks/ecr/_purge_repository.py
--rw-r--r--   0        0        0     1630 2023-05-26 23:21:54.345110 runway-2.6.6/runway/cfngin/hooks/ecs.py
--rw-r--r--   0        0        0     6204 2023-05-26 23:21:54.345110 runway-2.6.6/runway/cfngin/hooks/iam.py
--rw-r--r--   0        0        0     8766 2023-05-26 23:21:54.345110 runway-2.6.6/runway/cfngin/hooks/keypair.py
--rw-r--r--   0        0        0     3774 2023-05-26 23:21:54.345110 runway-2.6.6/runway/cfngin/hooks/protocols.py
--rw-r--r--   0        0        0      938 2023-05-26 23:21:54.345110 runway-2.6.6/runway/cfngin/hooks/route53.py
--rw-r--r--   0        0        0       21 2023-05-26 23:21:54.345110 runway-2.6.6/runway/cfngin/hooks/ssm/__init__.py
--rw-r--r--   0        0        0    11061 2023-05-26 23:21:54.345110 runway-2.6.6/runway/cfngin/hooks/ssm/parameter.py
--rw-r--r--   0        0        0       46 2023-05-26 23:21:54.345110 runway-2.6.6/runway/cfngin/hooks/staticsite/__init__.py
--rw-r--r--   0        0        0       46 2023-05-26 23:21:54.345110 runway-2.6.6/runway/cfngin/hooks/staticsite/auth_at_edge/__init__.py
--rw-r--r--   0        0        0     2644 2023-05-26 23:21:54.345110 runway-2.6.6/runway/cfngin/hooks/staticsite/auth_at_edge/callback_url_retriever.py
--rw-r--r--   0        0        0     2965 2023-05-26 23:21:54.345110 runway-2.6.6/runway/cfngin/hooks/staticsite/auth_at_edge/client_updater.py
--rw-r--r--   0        0        0     3784 2023-05-26 23:21:54.345110 runway-2.6.6/runway/cfngin/hooks/staticsite/auth_at_edge/domain_updater.py
--rw-r--r--   0        0        0     6704 2023-05-26 23:21:54.345110 runway-2.6.6/runway/cfngin/hooks/staticsite/auth_at_edge/lambda_config.py
--rw-r--r--   0        0        0       46 2023-05-26 23:21:54.345110 runway-2.6.6/runway/cfngin/hooks/staticsite/auth_at_edge/templates/__init__.py
--rw-r--r--   0        0        0     8317 2023-05-26 23:21:54.345110 runway-2.6.6/runway/cfngin/hooks/staticsite/auth_at_edge/templates/check_auth/__init__.py
--rw-r--r--   0        0        0      106 2023-05-26 23:21:54.345110 runway-2.6.6/runway/cfngin/hooks/staticsite/auth_at_edge/templates/check_auth/requirements.txt
--rw-r--r--   0        0        0      644 2023-05-26 23:21:54.345110 runway-2.6.6/runway/cfngin/hooks/staticsite/auth_at_edge/templates/http_headers/__init__.py
--rw-r--r--   0        0        0     8567 2023-05-26 23:21:54.345110 runway-2.6.6/runway/cfngin/hooks/staticsite/auth_at_edge/templates/parse_auth/__init__.py
--rw-r--r--   0        0        0      106 2023-05-26 23:21:54.345110 runway-2.6.6/runway/cfngin/hooks/staticsite/auth_at_edge/templates/parse_auth/requirements.txt
--rw-r--r--   0        0        0     4586 2023-05-26 23:21:54.345110 runway-2.6.6/runway/cfngin/hooks/staticsite/auth_at_edge/templates/refresh_auth/__init__.py
--rw-r--r--   0        0        0    12977 2023-05-26 23:21:54.345110 runway-2.6.6/runway/cfngin/hooks/staticsite/auth_at_edge/templates/shared.py
--rw-r--r--   0        0        0     7518 2023-05-26 23:21:54.345110 runway-2.6.6/runway/cfngin/hooks/staticsite/auth_at_edge/templates/shared_jose.py
--rw-r--r--   0        0        0     2314 2023-05-26 23:21:54.345110 runway-2.6.6/runway/cfngin/hooks/staticsite/auth_at_edge/templates/sign_out/__init__.py
--rw-r--r--   0        0        0     1151 2023-05-26 23:21:54.345110 runway-2.6.6/runway/cfngin/hooks/staticsite/auth_at_edge/user_pool_id_retriever.py
--rw-r--r--   0        0        0     6556 2023-05-26 23:21:54.345110 runway-2.6.6/runway/cfngin/hooks/staticsite/build_staticsite.py
--rw-r--r--   0        0        0     3478 2023-05-26 23:21:54.345110 runway-2.6.6/runway/cfngin/hooks/staticsite/cleanup.py
--rw-r--r--   0        0        0    13035 2023-05-26 23:21:54.345110 runway-2.6.6/runway/cfngin/hooks/staticsite/upload_staticsite.py
--rw-r--r--   0        0        0     2901 2023-05-26 23:21:54.345110 runway-2.6.6/runway/cfngin/hooks/staticsite/utils.py
--rw-r--r--   0        0        0     4913 2023-05-26 23:21:54.345110 runway-2.6.6/runway/cfngin/hooks/utils.py
--rw-r--r--   0        0        0     1582 2023-05-26 23:21:54.345110 runway-2.6.6/runway/cfngin/logger/__init__.py
--rw-r--r--   0        0        0      202 2023-05-26 23:21:54.345110 runway-2.6.6/runway/cfngin/lookups/__init__.py
--rw-r--r--   0        0        0       22 2023-05-26 23:21:54.345110 runway-2.6.6/runway/cfngin/lookups/handlers/__init__.py
--rw-r--r--   0        0        0     4480 2023-05-26 23:21:54.349110 runway-2.6.6/runway/cfngin/lookups/handlers/ami.py
--rw-r--r--   0        0        0    16481 2023-05-26 23:21:54.349110 runway-2.6.6/runway/cfngin/lookups/handlers/awslambda.py
--rw-r--r--   0        0        0     1682 2023-05-26 23:21:54.349110 runway-2.6.6/runway/cfngin/lookups/handlers/default.py
--rw-r--r--   0        0        0     9590 2023-05-26 23:21:54.349110 runway-2.6.6/runway/cfngin/lookups/handlers/dynamodb.py
--rw-r--r--   0        0        0     1667 2023-05-26 23:21:54.349110 runway-2.6.6/runway/cfngin/lookups/handlers/envvar.py
--rw-r--r--   0        0        0     6468 2023-05-26 23:21:54.349110 runway-2.6.6/runway/cfngin/lookups/handlers/file.py
--rw-r--r--   0        0        0     1606 2023-05-26 23:21:54.349110 runway-2.6.6/runway/cfngin/lookups/handlers/hook_data.py
--rw-r--r--   0        0        0     2188 2023-05-26 23:21:54.349110 runway-2.6.6/runway/cfngin/lookups/handlers/kms.py
--rw-r--r--   0        0        0     4487 2023-05-26 23:21:54.349110 runway-2.6.6/runway/cfngin/lookups/handlers/output.py
--rw-r--r--   0        0        0     2740 2023-05-26 23:21:54.349110 runway-2.6.6/runway/cfngin/lookups/handlers/rxref.py
--rw-r--r--   0        0        0     1649 2023-05-26 23:21:54.349110 runway-2.6.6/runway/cfngin/lookups/handlers/split.py
--rw-r--r--   0        0        0     1765 2023-05-26 23:21:54.349110 runway-2.6.6/runway/cfngin/lookups/handlers/xref.py
--rw-r--r--   0        0        0     4632 2023-05-26 23:21:54.349110 runway-2.6.6/runway/cfngin/lookups/registry.py
--rw-r--r--   0        0        0    24452 2023-05-26 23:21:54.349110 runway-2.6.6/runway/cfngin/plan.py
--rw-r--r--   0        0        0       22 2023-05-26 23:21:54.349110 runway-2.6.6/runway/cfngin/providers/__init__.py
--rw-r--r--   0        0        0       22 2023-05-26 23:21:54.349110 runway-2.6.6/runway/cfngin/providers/aws/__init__.py
--rw-r--r--   0        0        0    59113 2023-05-26 23:21:54.349110 runway-2.6.6/runway/cfngin/providers/aws/default.py
--rw-r--r--   0        0        0     1403 2023-05-26 23:21:54.349110 runway-2.6.6/runway/cfngin/providers/base.py
--rw-r--r--   0        0        0     1691 2023-05-26 23:21:54.349110 runway-2.6.6/runway/cfngin/session_cache.py
--rw-r--r--   0        0        0     8772 2023-05-26 23:21:54.349110 runway-2.6.6/runway/cfngin/stack.py
--rw-r--r--   0        0        0     4381 2023-05-26 23:21:54.349110 runway-2.6.6/runway/cfngin/status.py
--rw-r--r--   0        0        0     1556 2023-05-26 23:21:54.349110 runway-2.6.6/runway/cfngin/tokenize_userdata.py
--rw-r--r--   0        0        0     2914 2023-05-26 23:21:54.349110 runway-2.6.6/runway/cfngin/ui.py
--rw-r--r--   0        0        0    30329 2023-05-26 23:21:54.349110 runway-2.6.6/runway/cfngin/utils.py
--rw-r--r--   0        0        0      691 2023-05-26 23:21:54.349110 runway-2.6.6/runway/compat.py
--rw-r--r--   0        0        0    18286 2023-05-26 23:21:54.349110 runway-2.6.6/runway/config/__init__.py
--rw-r--r--   0        0        0       41 2023-05-26 23:21:54.349110 runway-2.6.6/runway/config/components/__init__.py
--rw-r--r--   0        0        0      587 2023-05-26 23:21:54.349110 runway-2.6.6/runway/config/components/runway/__init__.py
--rw-r--r--   0        0        0     6199 2023-05-26 23:21:54.349110 runway-2.6.6/runway/config/components/runway/_deployment_def.py
--rw-r--r--   0        0        0     3891 2023-05-26 23:21:54.349110 runway-2.6.6/runway/config/components/runway/_module_def.py
--rw-r--r--   0        0        0     4821 2023-05-26 23:21:54.349110 runway-2.6.6/runway/config/components/runway/_test_def.py
--rw-r--r--   0        0        0     2318 2023-05-26 23:21:54.349110 runway-2.6.6/runway/config/components/runway/_variables_def.py
--rw-r--r--   0        0        0     6232 2023-05-26 23:21:54.349110 runway-2.6.6/runway/config/components/runway/base.py
--rw-r--r--   0        0        0       37 2023-05-26 23:21:54.349110 runway-2.6.6/runway/config/models/__init__.py
--rw-r--r--   0        0        0      351 2023-05-26 23:21:54.349110 runway-2.6.6/runway/config/models/base.py
--rw-r--r--   0        0        0    14051 2023-05-26 23:21:54.349110 runway-2.6.6/runway/config/models/cfngin/__init__.py
--rw-r--r--   0        0        0     6629 2023-05-26 23:21:54.349110 runway-2.6.6/runway/config/models/cfngin/_package_sources.py
--rw-r--r--   0        0        0    24455 2023-05-26 23:21:54.349110 runway-2.6.6/runway/config/models/runway/__init__.py
--rw-r--r--   0        0        0     5959 2023-05-26 23:21:54.349110 runway-2.6.6/runway/config/models/runway/_builtin_tests.py
--rw-r--r--   0        0        0       29 2023-05-26 23:21:54.349110 runway-2.6.6/runway/config/models/runway/options/__init__.py
--rw-r--r--   0        0        0      542 2023-05-26 23:21:54.349110 runway-2.6.6/runway/config/models/runway/options/cdk.py
--rw-r--r--   0        0        0      546 2023-05-26 23:21:54.349110 runway-2.6.6/runway/config/models/runway/options/k8s.py
--rw-r--r--   0        0        0     1209 2023-05-26 23:21:54.349110 runway-2.6.6/runway/config/models/runway/options/serverless.py
--rw-r--r--   0        0        0     2299 2023-05-26 23:21:54.349110 runway-2.6.6/runway/config/models/runway/options/terraform.py
--rw-r--r--   0        0        0      920 2023-05-26 23:21:54.349110 runway-2.6.6/runway/config/models/utils.py
--rw-r--r--   0        0        0      292 2023-05-26 23:21:54.349110 runway-2.6.6/runway/constants.py
--rw-r--r--   0        0        0      139 2023-05-26 23:21:54.349110 runway-2.6.6/runway/context/__init__.py
--rw-r--r--   0        0        0     5799 2023-05-26 23:21:54.349110 runway-2.6.6/runway/context/_base.py
--rw-r--r--   0        0        0    19344 2023-05-26 23:21:54.349110 runway-2.6.6/runway/context/_cfngin.py
--rw-r--r--   0        0        0     3310 2023-05-26 23:21:54.349110 runway-2.6.6/runway/context/_runway.py
--rw-r--r--   0        0        0     2762 2023-05-26 23:21:54.349110 runway-2.6.6/runway/context/sys_info.py
--rw-r--r--   0        0        0      239 2023-05-26 23:21:54.349110 runway-2.6.6/runway/context/type_defs.py
--rw-r--r--   0        0        0     8802 2023-05-26 23:21:54.349110 runway-2.6.6/runway/core/__init__.py
--rw-r--r--   0        0        0      415 2023-05-26 23:21:54.353110 runway-2.6.6/runway/core/components/__init__.py
--rw-r--r--   0        0        0    12693 2023-05-26 23:21:54.353110 runway-2.6.6/runway/core/components/_deploy_environment.py
--rw-r--r--   0        0        0    11159 2023-05-26 23:21:54.353110 runway-2.6.6/runway/core/components/_deployment.py
--rw-r--r--   0        0        0    13116 2023-05-26 23:21:54.353110 runway-2.6.6/runway/core/components/_module.py
--rw-r--r--   0        0        0     5702 2023-05-26 23:21:54.353110 runway-2.6.6/runway/core/components/_module_path.py
--rw-r--r--   0        0        0     7426 2023-05-26 23:21:54.353110 runway-2.6.6/runway/core/components/_module_type.py
--rw-r--r--   0        0        0       24 2023-05-26 23:21:54.353110 runway-2.6.6/runway/core/providers/__init__.py
--rw-r--r--   0        0        0      316 2023-05-26 23:21:54.353110 runway-2.6.6/runway/core/providers/aws/__init__.py
--rw-r--r--   0        0        0     1659 2023-05-26 23:21:54.353110 runway-2.6.6/runway/core/providers/aws/_account.py
--rw-r--r--   0        0        0     5163 2023-05-26 23:21:54.353110 runway-2.6.6/runway/core/providers/aws/_assume_role.py
--rw-r--r--   0        0        0     2913 2023-05-26 23:21:54.353110 runway-2.6.6/runway/core/providers/aws/_response.py
--rw-r--r--   0        0        0      111 2023-05-26 23:21:54.353110 runway-2.6.6/runway/core/providers/aws/s3/__init__.py
--rw-r--r--   0        0        0     7768 2023-05-26 23:21:54.353110 runway-2.6.6/runway/core/providers/aws/s3/_bucket.py
--rw-r--r--   0        0        0       22 2023-05-26 23:21:54.353110 runway-2.6.6/runway/core/providers/aws/s3/_helpers/__init__.py
--rw-r--r--   0        0        0     9926 2023-05-26 23:21:54.353110 runway-2.6.6/runway/core/providers/aws/s3/_helpers/action_architecture.py
--rw-r--r--   0        0        0     6356 2023-05-26 23:21:54.353110 runway-2.6.6/runway/core/providers/aws/s3/_helpers/comparator.py
--rw-r--r--   0        0        0    15217 2023-05-26 23:21:54.353110 runway-2.6.6/runway/core/providers/aws/s3/_helpers/file_generator.py
--rw-r--r--   0        0        0     5021 2023-05-26 23:21:54.353110 runway-2.6.6/runway/core/providers/aws/s3/_helpers/file_info.py
--rw-r--r--   0        0        0     2227 2023-05-26 23:21:54.353110 runway-2.6.6/runway/core/providers/aws/s3/_helpers/file_info_builder.py
--rw-r--r--   0        0        0     6951 2023-05-26 23:21:54.353110 runway-2.6.6/runway/core/providers/aws/s3/_helpers/filters.py
--rw-r--r--   0        0        0     4450 2023-05-26 23:21:54.353110 runway-2.6.6/runway/core/providers/aws/s3/_helpers/format_path.py
--rw-r--r--   0        0        0     5394 2023-05-26 23:21:54.353110 runway-2.6.6/runway/core/providers/aws/s3/_helpers/parameters.py
--rw-r--r--   0        0        0    29422 2023-05-26 23:21:54.353110 runway-2.6.6/runway/core/providers/aws/s3/_helpers/results.py
--rw-r--r--   0        0        0    30172 2023-05-26 23:21:54.353110 runway-2.6.6/runway/core/providers/aws/s3/_helpers/s3handler.py
--rw-r--r--   0        0        0      660 2023-05-26 23:21:54.353110 runway-2.6.6/runway/core/providers/aws/s3/_helpers/sync_strategy/__init__.py
--rw-r--r--   0        0        0     7782 2023-05-26 23:21:54.353110 runway-2.6.6/runway/core/providers/aws/s3/_helpers/sync_strategy/base.py
--rw-r--r--   0        0        0     1126 2023-05-26 23:21:54.353110 runway-2.6.6/runway/core/providers/aws/s3/_helpers/sync_strategy/delete.py
--rw-r--r--   0        0        0     1461 2023-05-26 23:21:54.353110 runway-2.6.6/runway/core/providers/aws/s3/_helpers/sync_strategy/exact_timestamps.py
--rw-r--r--   0        0        0     1549 2023-05-26 23:21:54.353110 runway-2.6.6/runway/core/providers/aws/s3/_helpers/sync_strategy/register.py
--rw-r--r--   0        0        0     1208 2023-05-26 23:21:54.353110 runway-2.6.6/runway/core/providers/aws/s3/_helpers/sync_strategy/size_only.py
--rw-r--r--   0        0        0     5439 2023-05-26 23:21:54.353110 runway-2.6.6/runway/core/providers/aws/s3/_helpers/transfer_config.py
--rw-r--r--   0        0        0    32879 2023-05-26 23:21:54.353110 runway-2.6.6/runway/core/providers/aws/s3/_helpers/utils.py
--rw-r--r--   0        0        0     3088 2023-05-26 23:21:54.353110 runway-2.6.6/runway/core/providers/aws/s3/_sync_handler.py
--rw-r--r--   0        0        0     1609 2023-05-26 23:21:54.353110 runway-2.6.6/runway/core/providers/aws/s3/exceptions.py
--rw-r--r--   0        0        0      253 2023-05-26 23:21:54.353110 runway-2.6.6/runway/core/providers/aws/type_defs.py
--rw-r--r--   0        0        0      174 2023-05-26 23:21:54.353110 runway-2.6.6/runway/core/type_defs.py
--rw-r--r--   0        0        0      514 2023-05-26 23:21:54.353110 runway-2.6.6/runway/dependency_managers/__init__.py
--rw-r--r--   0        0        0     6370 2023-05-26 23:21:54.353110 runway-2.6.6/runway/dependency_managers/_pip.py
--rw-r--r--   0        0        0     3799 2023-05-26 23:21:54.353110 runway-2.6.6/runway/dependency_managers/_pipenv.py
--rw-r--r--   0        0        0     4732 2023-05-26 23:21:54.353110 runway-2.6.6/runway/dependency_managers/_poetry.py
--rw-r--r--   0        0        0     1595 2023-05-26 23:21:54.353110 runway-2.6.6/runway/dependency_managers/base_classes.py
--rw-r--r--   0        0        0     5147 2023-05-26 23:21:54.353110 runway-2.6.6/runway/env_mgr/__init__.py
--rw-r--r--   0        0        0    10321 2023-05-26 23:21:54.353110 runway-2.6.6/runway/env_mgr/kbenv.py
--rw-r--r--   0        0        0    15186 2023-05-26 23:21:54.353110 runway-2.6.6/runway/env_mgr/tfenv.py
--rw-r--r--   0        0        0    10958 2023-05-26 23:21:54.353110 runway-2.6.6/runway/exceptions.py
--rw-r--r--   0        0        0       46 2023-05-26 23:21:54.353110 runway-2.6.6/runway/lookups/__init__.py
--rw-r--r--   0        0        0      147 2023-05-26 23:21:54.353110 runway-2.6.6/runway/lookups/handlers/__init__.py
--rw-r--r--   0        0        0    10273 2023-05-26 23:21:54.353110 runway-2.6.6/runway/lookups/handlers/base.py
--rw-r--r--   0        0        0     4919 2023-05-26 23:21:54.353110 runway-2.6.6/runway/lookups/handlers/cfn.py
--rw-r--r--   0        0        0     1875 2023-05-26 23:21:54.353110 runway-2.6.6/runway/lookups/handlers/ecr.py
--rw-r--r--   0        0        0     1673 2023-05-26 23:21:54.353110 runway-2.6.6/runway/lookups/handlers/env.py
--rw-r--r--   0        0        0     3793 2023-05-26 23:21:54.353110 runway-2.6.6/runway/lookups/handlers/random_string.py
--rw-r--r--   0        0        0     1790 2023-05-26 23:21:54.353110 runway-2.6.6/runway/lookups/handlers/ssm.py
--rw-r--r--   0        0        0     1551 2023-05-26 23:21:54.353110 runway-2.6.6/runway/lookups/handlers/var.py
--rw-r--r--   0        0        0     2120 2023-05-26 23:21:54.353110 runway-2.6.6/runway/lookups/registry.py
--rw-r--r--   0        0        0     5049 2023-05-26 23:21:54.357110 runway-2.6.6/runway/mixins.py
--rw-r--r--   0        0        0       70 2023-05-26 23:21:54.357110 runway-2.6.6/runway/module/__init__.py
--rw-r--r--   0        0        0     7974 2023-05-26 23:21:54.357110 runway-2.6.6/runway/module/base.py
--rw-r--r--   0        0        0    10626 2023-05-26 23:21:54.357110 runway-2.6.6/runway/module/cdk.py
--rw-r--r--   0        0        0     3132 2023-05-26 23:21:54.357110 runway-2.6.6/runway/module/cloudformation.py
--rw-r--r--   0        0        0    10461 2023-05-26 23:21:54.357110 runway-2.6.6/runway/module/k8s.py
--rw-r--r--   0        0        0    19334 2023-05-26 23:21:54.357110 runway-2.6.6/runway/module/serverless.py
--rw-r--r--   0        0        0       91 2023-05-26 23:21:54.357110 runway-2.6.6/runway/module/staticsite/__init__.py
--rw-r--r--   0        0        0    26533 2023-05-26 23:21:54.357110 runway-2.6.6/runway/module/staticsite/handler.py
--rw-r--r--   0        0        0      605 2023-05-26 23:21:54.357110 runway-2.6.6/runway/module/staticsite/options/__init__.py
--rw-r--r--   0        0        0     1457 2023-05-26 23:21:54.357110 runway-2.6.6/runway/module/staticsite/options/components.py
--rw-r--r--   0        0        0     5411 2023-05-26 23:21:54.357110 runway-2.6.6/runway/module/staticsite/options/models.py
--rw-r--r--   0        0        0      395 2023-05-26 23:21:54.357110 runway-2.6.6/runway/module/staticsite/parameters/__init__.py
--rw-r--r--   0        0        0     8648 2023-05-26 23:21:54.357110 runway-2.6.6/runway/module/staticsite/parameters/models.py
--rw-r--r--   0        0        0      277 2023-05-26 23:21:54.357110 runway-2.6.6/runway/module/staticsite/utils.py
--rw-r--r--   0        0        0    25863 2023-05-26 23:21:54.357110 runway-2.6.6/runway/module/terraform.py
--rw-r--r--   0        0        0     4106 2023-05-26 23:21:54.357110 runway-2.6.6/runway/module/utils.py
--rw-r--r--   0        0        0     7947 2023-05-26 23:21:54.357110 runway-2.6.6/runway/s3_utils.py
--rw-r--r--   0        0        0       46 2023-05-26 23:21:54.357110 runway-2.6.6/runway/sources/__init__.py
--rw-r--r--   0        0        0     4143 2023-05-26 23:21:54.357110 runway-2.6.6/runway/sources/git.py
--rw-r--r--   0        0        0     1864 2023-05-26 23:21:54.357110 runway-2.6.6/runway/sources/source.py
--rw-r--r--   0        0        0       53 2023-05-26 23:21:54.357110 runway-2.6.6/runway/templates/.flake8
--rw-r--r--   0        0        0    16636 2023-05-26 23:21:54.357110 runway-2.6.6/runway/templates/.pylintrc
--rw-r--r--   0        0        0      408 2023-05-26 23:21:54.357110 runway-2.6.6/runway/templates/.yamllint.yml
--rw-r--r--   0        0        0      703 2023-05-26 23:21:54.357110 runway-2.6.6/runway/templates/cdk-csharp/README.md
--rw-r--r--   0        0        0       85 2023-05-26 23:21:54.357110 runway-2.6.6/runway/templates/cdk-csharp/add-project.hook.d.ts
--rw-r--r--   0        0        0      101 2023-05-26 23:21:54.357110 runway-2.6.6/runway/templates/cdk-csharp/cdk.json
--rw-r--r--   0        0        0     5721 2023-05-26 23:21:54.357110 runway-2.6.6/runway/templates/cdk-csharp/dot_gitignore
--rw-r--r--   0        0        0      261 2023-05-26 23:21:54.357110 runway-2.6.6/runway/templates/cdk-csharp/package.json
--rw-r--r--   0        0        0       51 2023-05-26 23:21:54.357110 runway-2.6.6/runway/templates/cdk-csharp/runway.module.yml
--rw-r--r--   0        0        0      476 2023-05-26 23:21:54.357110 runway-2.6.6/runway/templates/cdk-csharp/src/HelloCdk/HelloCdk.csproj
--rw-r--r--   0        0        0     1009 2023-05-26 23:21:54.357110 runway-2.6.6/runway/templates/cdk-csharp/src/HelloCdk/HelloConstruct.cs
--rw-r--r--   0        0        0     1166 2023-05-26 23:21:54.357110 runway-2.6.6/runway/templates/cdk-csharp/src/HelloCdk/HelloStack.cs
--rw-r--r--   0        0        0      537 2023-05-26 23:21:54.357110 runway-2.6.6/runway/templates/cdk-csharp/src/HelloCdk/Program.cs
--rw-r--r--   0        0        0     1697 2023-05-26 23:21:54.357110 runway-2.6.6/runway/templates/cdk-csharp/src/HelloCdk.sln
--rw-r--r--   0        0        0       21 2023-05-26 23:21:54.357110 runway-2.6.6/runway/templates/cdk-py/.gitignore
--rw-r--r--   0        0        0      172 2023-05-26 23:21:54.357110 runway-2.6.6/runway/templates/cdk-py/app.py
--rw-r--r--   0        0        0       69 2023-05-26 23:21:54.357110 runway-2.6.6/runway/templates/cdk-py/cdk.json
--rw-r--r--   0        0        0       46 2023-05-26 23:21:54.357110 runway-2.6.6/runway/templates/cdk-py/hello/__init__.py
--rw-r--r--   0        0        0      736 2023-05-26 23:21:54.357110 runway-2.6.6/runway/templates/cdk-py/hello/hello_construct.py
--rw-r--r--   0        0        0      850 2023-05-26 23:21:54.357110 runway-2.6.6/runway/templates/cdk-py/hello/hello_stack.py
--rw-r--r--   0        0        0      239 2023-05-26 23:21:54.357110 runway-2.6.6/runway/templates/cdk-py/package.json
--rw-r--r--   0        0        0    22817 2023-05-26 23:21:54.357110 runway-2.6.6/runway/templates/cdk-py/poetry.lock
--rw-r--r--   0        0        0      514 2023-05-26 23:21:54.357110 runway-2.6.6/runway/templates/cdk-py/pyproject.toml
--rw-r--r--   0        0        0       49 2023-05-26 23:21:54.357110 runway-2.6.6/runway/templates/cdk-py/runway.module.yml
--rw-r--r--   0        0        0       33 2023-05-26 23:21:54.357110 runway-2.6.6/runway/templates/cdk-tsc/.gitignore
--rw-r--r--   0        0        0       13 2023-05-26 23:21:54.357110 runway-2.6.6/runway/templates/cdk-tsc/.npmignore
--rw-r--r--   0        0        0      315 2023-05-26 23:21:54.357110 runway-2.6.6/runway/templates/cdk-tsc/README.md
--rw-r--r--   0        0        0      213 2023-05-26 23:21:54.357110 runway-2.6.6/runway/templates/cdk-tsc/bin/sample.ts
--rw-r--r--   0        0        0       63 2023-05-26 23:21:54.357110 runway-2.6.6/runway/templates/cdk-tsc/cdk.json
--rw-r--r--   0        0        0      239 2023-05-26 23:21:54.357110 runway-2.6.6/runway/templates/cdk-tsc/lib/sample-stack.ts
--rw-r--r--   0        0        0      448 2023-05-26 23:21:54.357110 runway-2.6.6/runway/templates/cdk-tsc/package.json
--rw-r--r--   0        0        0       48 2023-05-26 23:21:54.357110 runway-2.6.6/runway/templates/cdk-tsc/runway.module.yml
--rw-r--r--   0        0        0      620 2023-05-26 23:21:54.357110 runway-2.6.6/runway/templates/cdk-tsc/tsconfig.json
--rw-r--r--   0        0        0      229 2023-05-26 23:21:54.357110 runway-2.6.6/runway/templates/cfn/dev-us-east-1.env
--rw-r--r--   0        0        0      305 2023-05-26 23:21:54.357110 runway-2.6.6/runway/templates/cfn/stacks.yaml
--rw-r--r--   0        0        0      240 2023-05-26 23:21:54.357110 runway-2.6.6/runway/templates/cfngin/dev-us-east-1.env
--rw-r--r--   0        0        0      283 2023-05-26 23:21:54.357110 runway-2.6.6/runway/templates/cfngin/stacks.yaml
--rw-r--r--   0        0        0     2319 2023-05-26 23:21:54.357110 runway-2.6.6/runway/templates/k8s-cfn-repo/README.md
--rw-r--r--   0        0        0       35 2023-05-26 23:21:54.357110 runway-2.6.6/runway/templates/k8s-cfn-repo/_gitignore
--rw-r--r--   0        0        0       44 2023-05-26 23:21:54.357110 runway-2.6.6/runway/templates/k8s-cfn-repo/aws-auth-cm.k8s/base/kustomization.yaml
--rw-r--r--   0        0        0        7 2023-05-26 23:21:54.357110 runway-2.6.6/runway/templates/k8s-cfn-repo/aws-auth-cm.k8s/overlays/template/.kubectl-version
--rw-r--r--   0        0        0       54 2023-05-26 23:21:54.357110 runway-2.6.6/runway/templates/k8s-cfn-repo/aws-auth-cm.k8s/overlays/template/kustomization.yaml
--rw-r--r--   0        0        0       51 2023-05-26 23:21:54.357110 runway-2.6.6/runway/templates/k8s-cfn-repo/k8s-master.cfn/k8s_hooks/__init__.py
--rw-r--r--   0        0        0     2819 2023-05-26 23:21:54.357110 runway-2.6.6/runway/templates/k8s-cfn-repo/k8s-master.cfn/k8s_hooks/auth_map.py
--rw-r--r--   0        0        0      377 2023-05-26 23:21:54.357110 runway-2.6.6/runway/templates/k8s-cfn-repo/k8s-master.cfn/k8s_hooks/aws-auth-cm.yaml
--rw-r--r--   0        0        0     1643 2023-05-26 23:21:54.357110 runway-2.6.6/runway/templates/k8s-cfn-repo/k8s-master.cfn/k8s_hooks/awscli.py
--rw-r--r--   0        0        0     3153 2023-05-26 23:21:54.357110 runway-2.6.6/runway/templates/k8s-cfn-repo/k8s-master.cfn/k8s_hooks/bootstrap.py
--rw-r--r--   0        0        0     1078 2023-05-26 23:21:54.357110 runway-2.6.6/runway/templates/k8s-cfn-repo/k8s-master.cfn/stacks.yaml
--rw-r--r--   0        0        0      120 2023-05-26 23:21:54.357110 runway-2.6.6/runway/templates/k8s-cfn-repo/k8s-workers.cfn/local_lookups/__init__.py
--rw-r--r--   0        0        0     1893 2023-05-26 23:21:54.357110 runway-2.6.6/runway/templates/k8s-cfn-repo/k8s-workers.cfn/local_lookups/bootstrap_value.py
--rw-r--r--   0        0        0     1276 2023-05-26 23:21:54.357110 runway-2.6.6/runway/templates/k8s-cfn-repo/k8s-workers.cfn/stacks.yaml
--rw-r--r--   0        0        0     1095 2023-05-26 23:21:54.361111 runway-2.6.6/runway/templates/k8s-cfn-repo/runway.yml
--rw-r--r--   0        0        0      107 2023-05-26 23:21:54.361111 runway-2.6.6/runway/templates/k8s-cfn-repo/service-hello-world.k8s/README.md
--rw-r--r--   0        0        0      117 2023-05-26 23:21:54.361111 runway-2.6.6/runway/templates/k8s-cfn-repo/service-hello-world.k8s/base/configMap.yaml
--rw-r--r--   0        0        0      755 2023-05-26 23:21:54.361111 runway-2.6.6/runway/templates/k8s-cfn-repo/service-hello-world.k8s/base/deployment.yaml
--rw-r--r--   0        0        0      176 2023-05-26 23:21:54.361111 runway-2.6.6/runway/templates/k8s-cfn-repo/service-hello-world.k8s/base/kustomization.yaml
--rw-r--r--   0        0        0      189 2023-05-26 23:21:54.361111 runway-2.6.6/runway/templates/k8s-cfn-repo/service-hello-world.k8s/base/service.yaml
--rw-r--r--   0        0        0        7 2023-05-26 23:21:54.361111 runway-2.6.6/runway/templates/k8s-cfn-repo/service-hello-world.k8s/overlays/prod/.kubectl-version
--rw-r--r--   0        0        0       91 2023-05-26 23:21:54.361111 runway-2.6.6/runway/templates/k8s-cfn-repo/service-hello-world.k8s/overlays/prod/deployment.yaml
--rw-r--r--   0        0        0      177 2023-05-26 23:21:54.361111 runway-2.6.6/runway/templates/k8s-cfn-repo/service-hello-world.k8s/overlays/prod/kustomization.yaml
--rw-r--r--   0        0        0        7 2023-05-26 23:21:54.361111 runway-2.6.6/runway/templates/k8s-cfn-repo/service-hello-world.k8s/overlays/template/.kubectl-version
--rw-r--r--   0        0        0      188 2023-05-26 23:21:54.361111 runway-2.6.6/runway/templates/k8s-cfn-repo/service-hello-world.k8s/overlays/template/kustomization.yaml
--rw-r--r--   0        0        0      118 2023-05-26 23:21:54.361111 runway-2.6.6/runway/templates/k8s-cfn-repo/service-hello-world.k8s/overlays/template/map.yaml
--rw-r--r--   0        0        0        7 2023-05-26 23:21:54.361111 runway-2.6.6/runway/templates/k8s-flux-repo/.kubectl-version
--rw-r--r--   0        0        0     3343 2023-05-26 23:21:54.361111 runway-2.6.6/runway/templates/k8s-flux-repo/README.md
--rw-r--r--   0        0        0      120 2023-05-26 23:21:54.361111 runway-2.6.6/runway/templates/k8s-flux-repo/_gitignore
--rw-r--r--   0        0        0      109 2023-05-26 23:21:54.361111 runway-2.6.6/runway/templates/k8s-flux-repo/flux-dev/README.md
--rw-r--r--   0        0        0       33 2023-05-26 23:21:54.361111 runway-2.6.6/runway/templates/k8s-flux-repo/flux-dev/namespaces/README.md
--rw-r--r--   0        0        0       79 2023-05-26 23:21:54.361111 runway-2.6.6/runway/templates/k8s-flux-repo/flux-dev/namespaces/demo.yaml
--rw-r--r--   0        0        0       31 2023-05-26 23:21:54.361111 runway-2.6.6/runway/templates/k8s-flux-repo/flux-dev/workloads/README.md
--rw-r--r--   0        0        0       12 2023-05-26 23:21:54.361111 runway-2.6.6/runway/templates/k8s-flux-repo/flux.tf/.terraform-version
--rw-r--r--   0        0        0     3268 2023-05-26 23:21:54.361111 runway-2.6.6/runway/templates/k8s-flux-repo/flux.tf/.terraform.lock.hcl
--rw-r--r--   0        0        0      718 2023-05-26 23:21:54.361111 runway-2.6.6/runway/templates/k8s-flux-repo/flux.tf/docker/Dockerfile
--rw-r--r--   0        0        0    12304 2023-05-26 23:21:54.361111 runway-2.6.6/runway/templates/k8s-flux-repo/flux.tf/main.tf
--rw-r--r--   0        0        0       56 2023-05-26 23:21:54.361111 runway-2.6.6/runway/templates/k8s-flux-repo/flux.tf/sleep.py
--rw-r--r--   0        0        0      780 2023-05-26 23:21:54.361111 runway-2.6.6/runway/templates/k8s-flux-repo/runway.yml
--rw-r--r--   0        0        0        7 2023-05-26 23:21:54.361111 runway-2.6.6/runway/templates/k8s-tf-repo/.kubectl-version
--rw-r--r--   0        0        0     3600 2023-05-26 23:21:54.361111 runway-2.6.6/runway/templates/k8s-tf-repo/README.md
--rw-r--r--   0        0        0       46 2023-05-26 23:21:54.361111 runway-2.6.6/runway/templates/k8s-tf-repo/_gitignore
--rw-r--r--   0        0        0       12 2023-05-26 23:21:54.361111 runway-2.6.6/runway/templates/k8s-tf-repo/eks-base.tf/.terraform-version
--rw-r--r--   0        0        0     3123 2023-05-26 23:21:54.361111 runway-2.6.6/runway/templates/k8s-tf-repo/eks-base.tf/.terraform.lock.hcl
--rw-r--r--   0        0        0     8778 2023-05-26 23:21:54.361111 runway-2.6.6/runway/templates/k8s-tf-repo/eks-base.tf/main.tf
--rw-r--r--   0        0        0       57 2023-05-26 23:21:54.361111 runway-2.6.6/runway/templates/k8s-tf-repo/eks-base.tf/sleep.py
--rw-r--r--   0        0        0      222 2023-05-26 23:21:54.361111 runway-2.6.6/runway/templates/k8s-tf-repo/gen-kubeconfig.cfn/hooks.yaml
--rw-r--r--   0        0        0       51 2023-05-26 23:21:54.361111 runway-2.6.6/runway/templates/k8s-tf-repo/gen-kubeconfig.cfn/k8s_hooks/__init__.py
--rw-r--r--   0        0        0       12 2023-05-26 23:21:54.361111 runway-2.6.6/runway/templates/k8s-tf-repo/job-s3-echo.tf/.terraform-version
--rw-r--r--   0        0        0     2114 2023-05-26 23:21:54.361111 runway-2.6.6/runway/templates/k8s-tf-repo/job-s3-echo.tf/.terraform.lock.hcl
--rw-r--r--   0        0        0     4464 2023-05-26 23:21:54.361111 runway-2.6.6/runway/templates/k8s-tf-repo/job-s3-echo.tf/main.tf
--rw-r--r--   0        0        0       56 2023-05-26 23:21:54.361111 runway-2.6.6/runway/templates/k8s-tf-repo/job-s3-echo.tf/sleep.py
--rw-r--r--   0        0        0      825 2023-05-26 23:21:54.361111 runway-2.6.6/runway/templates/k8s-tf-repo/runway.yml
--rw-r--r--   0        0        0      107 2023-05-26 23:21:54.361111 runway-2.6.6/runway/templates/k8s-tf-repo/service-hello-world.k8s/README.md
--rw-r--r--   0        0        0      117 2023-05-26 23:21:54.361111 runway-2.6.6/runway/templates/k8s-tf-repo/service-hello-world.k8s/base/configMap.yaml
--rw-r--r--   0        0        0      755 2023-05-26 23:21:54.361111 runway-2.6.6/runway/templates/k8s-tf-repo/service-hello-world.k8s/base/deployment.yaml
--rw-r--r--   0        0        0      176 2023-05-26 23:21:54.361111 runway-2.6.6/runway/templates/k8s-tf-repo/service-hello-world.k8s/base/kustomization.yaml
--rw-r--r--   0        0        0      189 2023-05-26 23:21:54.361111 runway-2.6.6/runway/templates/k8s-tf-repo/service-hello-world.k8s/base/service.yaml
--rw-r--r--   0        0        0        7 2023-05-26 23:21:54.361111 runway-2.6.6/runway/templates/k8s-tf-repo/service-hello-world.k8s/overlays/dev/.kubectl-version
--rw-r--r--   0        0        0      161 2023-05-26 23:21:54.361111 runway-2.6.6/runway/templates/k8s-tf-repo/service-hello-world.k8s/overlays/dev/kustomization.yaml
--rw-r--r--   0        0        0      118 2023-05-26 23:21:54.361111 runway-2.6.6/runway/templates/k8s-tf-repo/service-hello-world.k8s/overlays/dev/map.yaml
--rw-r--r--   0        0        0        7 2023-05-26 23:21:54.361111 runway-2.6.6/runway/templates/k8s-tf-repo/service-hello-world.k8s/overlays/prod/.kubectl-version
--rw-r--r--   0        0        0       91 2023-05-26 23:21:54.361111 runway-2.6.6/runway/templates/k8s-tf-repo/service-hello-world.k8s/overlays/prod/deployment.yaml
--rw-r--r--   0        0        0      177 2023-05-26 23:21:54.361111 runway-2.6.6/runway/templates/k8s-tf-repo/service-hello-world.k8s/overlays/prod/kustomization.yaml
--rw-r--r--   0        0        0      440 2023-05-26 23:21:54.361111 runway-2.6.6/runway/templates/k8s-tf-repo/tfstate.cfn/stacks.yaml
--rw-r--r--   0        0        0       69 2023-05-26 23:21:54.361111 runway-2.6.6/runway/templates/sls-py/__init__.py
--rw-r--r--   0        0        0       31 2023-05-26 23:21:54.361111 runway-2.6.6/runway/templates/sls-py/_gitignore
--rw-r--r--   0        0        0        5 2023-05-26 23:21:54.361111 runway-2.6.6/runway/templates/sls-py/config-dev-us-east-1.json
--rw-r--r--   0        0        0      683 2023-05-26 23:21:54.361111 runway-2.6.6/runway/templates/sls-py/hello_world/__init__.py
--rw-r--r--   0        0        0      290 2023-05-26 23:21:54.361111 runway-2.6.6/runway/templates/sls-py/package.json
--rw-r--r--   0        0        0     4451 2023-05-26 23:21:54.361111 runway-2.6.6/runway/templates/sls-py/poetry.lock
--rw-r--r--   0        0        0      354 2023-05-26 23:21:54.361111 runway-2.6.6/runway/templates/sls-py/pyproject.toml
--rw-r--r--   0        0        0      529 2023-05-26 23:21:54.361111 runway-2.6.6/runway/templates/sls-py/serverless.yml
--rw-r--r--   0        0        0       27 2023-05-26 23:21:54.361111 runway-2.6.6/runway/templates/sls-tsc/.eslintignore
--rw-r--r--   0        0        0      265 2023-05-26 23:21:54.361111 runway-2.6.6/runway/templates/sls-tsc/.eslintrc.js
--rw-r--r--   0        0        0       49 2023-05-26 23:21:54.361111 runway-2.6.6/runway/templates/sls-tsc/_gitignore
--rw-r--r--   0        0        0      281 2023-05-26 23:21:54.361111 runway-2.6.6/runway/templates/sls-tsc/jest.config.js
--rw-r--r--   0        0        0     1087 2023-05-26 23:21:54.361111 runway-2.6.6/runway/templates/sls-tsc/package.json
--rw-r--r--   0        0        0      642 2023-05-26 23:21:54.361111 runway-2.6.6/runway/templates/sls-tsc/serverless.yml
--rw-r--r--   0        0        0      787 2023-05-26 23:21:54.361111 runway-2.6.6/runway/templates/sls-tsc/src/helloWorld.test.ts
--rw-r--r--   0        0        0      713 2023-05-26 23:21:54.361111 runway-2.6.6/runway/templates/sls-tsc/src/helloWorld.ts
--rw-r--r--   0        0        0      514 2023-05-26 23:21:54.361111 runway-2.6.6/runway/templates/sls-tsc/tsconfig.json
--rw-r--r--   0        0        0     1178 2023-05-26 23:21:54.361111 runway-2.6.6/runway/templates/sls-tsc/webpack.config.js
--rw-r--r--   0        0        0      444 2023-05-26 23:21:54.361111 runway-2.6.6/runway/templates/static-angular/runway.yml
--rw-r--r--   0        0        0      246 2023-05-26 23:21:54.361111 runway-2.6.6/runway/templates/static-angular/sampleapp.web/.editorconfig
--rw-r--r--   0        0        0     1027 2023-05-26 23:21:54.361111 runway-2.6.6/runway/templates/static-angular/sampleapp.web/README.md
--rw-r--r--   0        0        0      631 2023-05-26 23:21:54.361111 runway-2.6.6/runway/templates/static-angular/sampleapp.web/_gitignore
--rw-r--r--   0        0        0     3626 2023-05-26 23:21:54.361111 runway-2.6.6/runway/templates/static-angular/sampleapp.web/angular.json
--rw-r--r--   0        0        0      430 2023-05-26 23:21:54.361111 runway-2.6.6/runway/templates/static-angular/sampleapp.web/browserslist
--rw-r--r--   0        0        0      809 2023-05-26 23:21:54.361111 runway-2.6.6/runway/templates/static-angular/sampleapp.web/e2e/protractor.conf.js
--rw-r--r--   0        0        0      643 2023-05-26 23:21:54.361111 runway-2.6.6/runway/templates/static-angular/sampleapp.web/e2e/src/app.e2e-spec.ts
--rw-r--r--   0        0        0      262 2023-05-26 23:21:54.361111 runway-2.6.6/runway/templates/static-angular/sampleapp.web/e2e/src/app.po.ts
--rw-r--r--   0        0        0      214 2023-05-26 23:21:54.361111 runway-2.6.6/runway/templates/static-angular/sampleapp.web/e2e/tsconfig.json
--rw-r--r--   0        0        0     1022 2023-05-26 23:21:54.361111 runway-2.6.6/runway/templates/static-angular/sampleapp.web/karma.conf.js
--rw-r--r--   0        0        0   595303 2023-05-26 23:21:54.365110 runway-2.6.6/runway/templates/static-angular/sampleapp.web/package-lock.json
--rw-r--r--   0        0        0     1295 2023-05-26 23:21:54.365110 runway-2.6.6/runway/templates/static-angular/sampleapp.web/package.json
--rw-r--r--   0        0        0      246 2023-05-26 23:21:54.365110 runway-2.6.6/runway/templates/static-angular/sampleapp.web/src/app/app-routing.module.ts
--rw-r--r--   0        0        0        0 2023-05-26 23:21:54.365110 runway-2.6.6/runway/templates/static-angular/sampleapp.web/src/app/app.component.css
--rw-r--r--   0        0        0    25523 2023-05-26 23:21:54.365110 runway-2.6.6/runway/templates/static-angular/sampleapp.web/src/app/app.component.html
--rw-r--r--   0        0        0     1110 2023-05-26 23:21:54.365110 runway-2.6.6/runway/templates/static-angular/sampleapp.web/src/app/app.component.spec.ts
--rw-r--r--   0        0        0      214 2023-05-26 23:21:54.365110 runway-2.6.6/runway/templates/static-angular/sampleapp.web/src/app/app.component.ts
--rw-r--r--   0        0        0      393 2023-05-26 23:21:54.365110 runway-2.6.6/runway/templates/static-angular/sampleapp.web/src/app/app.module.ts
--rw-r--r--   0        0        0        0 2023-05-26 23:21:54.365110 runway-2.6.6/runway/templates/static-angular/sampleapp.web/src/assets/.gitkeep
--rw-r--r--   0        0        0       51 2023-05-26 23:21:54.365110 runway-2.6.6/runway/templates/static-angular/sampleapp.web/src/environments/environment.prod.ts
--rw-r--r--   0        0        0      662 2023-05-26 23:21:54.365110 runway-2.6.6/runway/templates/static-angular/sampleapp.web/src/environments/environment.ts
--rw-r--r--   0        0        0      948 2023-05-26 23:21:54.365110 runway-2.6.6/runway/templates/static-angular/sampleapp.web/src/favicon.ico
--rw-r--r--   0        0        0      295 2023-05-26 23:21:54.365110 runway-2.6.6/runway/templates/static-angular/sampleapp.web/src/index.html
--rw-r--r--   0        0        0      372 2023-05-26 23:21:54.365110 runway-2.6.6/runway/templates/static-angular/sampleapp.web/src/main.ts
--rw-r--r--   0        0        0     2838 2023-05-26 23:21:54.365110 runway-2.6.6/runway/templates/static-angular/sampleapp.web/src/polyfills.ts
--rw-r--r--   0        0        0       80 2023-05-26 23:21:54.365110 runway-2.6.6/runway/templates/static-angular/sampleapp.web/src/styles.css
--rw-r--r--   0        0        0      642 2023-05-26 23:21:54.365110 runway-2.6.6/runway/templates/static-angular/sampleapp.web/src/test.ts
--rw-r--r--   0        0        0      270 2023-05-26 23:21:54.365110 runway-2.6.6/runway/templates/static-angular/sampleapp.web/tsconfig.app.json
--rw-r--r--   0        0        0      543 2023-05-26 23:21:54.365110 runway-2.6.6/runway/templates/static-angular/sampleapp.web/tsconfig.json
--rw-r--r--   0        0        0      270 2023-05-26 23:21:54.365110 runway-2.6.6/runway/templates/static-angular/sampleapp.web/tsconfig.spec.json
--rw-r--r--   0        0        0     1954 2023-05-26 23:21:54.365110 runway-2.6.6/runway/templates/static-angular/sampleapp.web/tslint.json
--rw-r--r--   0        0        0      435 2023-05-26 23:21:54.365110 runway-2.6.6/runway/templates/static-react/runway.yml
--rw-r--r--   0        0        0      310 2023-05-26 23:21:54.365110 runway-2.6.6/runway/templates/static-react/sampleapp.web/.gitignore
--rw-r--r--   0        0        0     2889 2023-05-26 23:21:54.365110 runway-2.6.6/runway/templates/static-react/sampleapp.web/README.md
--rw-r--r--   0        0        0      746 2023-05-26 23:21:54.365110 runway-2.6.6/runway/templates/static-react/sampleapp.web/package.json
--rw-r--r--   0        0        0     3870 2023-05-26 23:21:54.365110 runway-2.6.6/runway/templates/static-react/sampleapp.web/public/favicon.ico
--rw-r--r--   0        0        0     1721 2023-05-26 23:21:54.365110 runway-2.6.6/runway/templates/static-react/sampleapp.web/public/index.html
--rw-r--r--   0        0        0     5347 2023-05-26 23:21:54.365110 runway-2.6.6/runway/templates/static-react/sampleapp.web/public/logo192.png
--rw-r--r--   0        0        0     9664 2023-05-26 23:21:54.365110 runway-2.6.6/runway/templates/static-react/sampleapp.web/public/logo512.png
--rw-r--r--   0        0        0      492 2023-05-26 23:21:54.365110 runway-2.6.6/runway/templates/static-react/sampleapp.web/public/manifest.json
--rw-r--r--   0        0        0       67 2023-05-26 23:21:54.365110 runway-2.6.6/runway/templates/static-react/sampleapp.web/public/robots.txt
--rw-r--r--   0        0        0      564 2023-05-26 23:21:54.365110 runway-2.6.6/runway/templates/static-react/sampleapp.web/src/App.css
--rw-r--r--   0        0        0      555 2023-05-26 23:21:54.365110 runway-2.6.6/runway/templates/static-react/sampleapp.web/src/App.js
--rw-r--r--   0        0        0      280 2023-05-26 23:21:54.365110 runway-2.6.6/runway/templates/static-react/sampleapp.web/src/App.test.js
--rw-r--r--   0        0        0      366 2023-05-26 23:21:54.365110 runway-2.6.6/runway/templates/static-react/sampleapp.web/src/index.css
--rw-r--r--   0        0        0      452 2023-05-26 23:21:54.365110 runway-2.6.6/runway/templates/static-react/sampleapp.web/src/index.js
--rw-r--r--   0        0        0     2671 2023-05-26 23:21:54.365110 runway-2.6.6/runway/templates/static-react/sampleapp.web/src/logo.svg
--rw-r--r--   0        0        0     5003 2023-05-26 23:21:54.365110 runway-2.6.6/runway/templates/static-react/sampleapp.web/src/serviceWorker.js
--rw-r--r--   0        0        0      255 2023-05-26 23:21:54.365110 runway-2.6.6/runway/templates/static-react/sampleapp.web/src/setupTests.js
--rw-r--r--   0        0        0       82 2023-05-26 23:21:54.365110 runway-2.6.6/runway/templates/terraform/backend-us-east-1.tfvars
--rw-r--r--   0        0        0       21 2023-05-26 23:21:54.365110 runway-2.6.6/runway/templates/terraform/dev-us-east-1.tfvars
--rw-r--r--   0        0        0      312 2023-05-26 23:21:54.365110 runway-2.6.6/runway/templates/terraform/main.tf
--rw-r--r--   0        0        0       46 2023-05-26 23:21:54.365110 runway-2.6.6/runway/tests/__init__.py
--rw-r--r--   0        0        0      111 2023-05-26 23:21:54.365110 runway-2.6.6/runway/tests/handlers/__init__.py
--rw-r--r--   0        0        0      757 2023-05-26 23:21:54.365110 runway-2.6.6/runway/tests/handlers/base.py
--rw-r--r--   0        0        0     1901 2023-05-26 23:21:54.365110 runway-2.6.6/runway/tests/handlers/cfn_lint.py
--rw-r--r--   0        0        0     1608 2023-05-26 23:21:54.365110 runway-2.6.6/runway/tests/handlers/script.py
--rw-r--r--   0        0        0     2025 2023-05-26 23:21:54.365110 runway-2.6.6/runway/tests/handlers/yaml_lint.py
--rw-r--r--   0        0        0     1112 2023-05-26 23:21:54.365110 runway-2.6.6/runway/tests/registry.py
--rw-r--r--   0        0        0      628 2023-05-26 23:21:54.365110 runway-2.6.6/runway/type_defs.py
--rw-r--r--   0        0        0    27539 2023-05-26 23:21:54.365110 runway-2.6.6/runway/utils/__init__.py
--rw-r--r--   0        0        0     4278 2023-05-26 23:21:54.369111 runway-2.6.6/runway/utils/_file_hash.py
--rw-r--r--   0        0        0      817 2023-05-26 23:21:54.369111 runway-2.6.6/runway/utils/_version.py
--rw-r--r--   0        0        0    29956 2023-05-26 23:21:54.369111 runway-2.6.6/runway/variables.py
--rw-r--r--   0        0        0     6147 1970-01-01 00:00:00.000000 runway-2.6.6/PKG-INFO
+-rw-r--r--   0        0        0    11346 2023-07-21 19:24:17.565800 runway-2.6.7/LICENSE
+-rw-r--r--   0        0        0     3587 2023-07-21 19:24:17.565800 runway-2.6.7/README.md
+-rw-r--r--   0        0        0    10039 2023-07-21 19:24:54.638045 runway-2.6.7/pyproject.toml
+-rw-r--r--   0        0        0      550 2023-07-21 19:24:17.601800 runway-2.6.7/runway/__init__.py
+-rw-r--r--   0        0        0       59 2023-07-21 19:24:17.601800 runway-2.6.7/runway/_cli/__init__.py
+-rw-r--r--   0        0        0      824 2023-07-21 19:24:17.601800 runway-2.6.7/runway/_cli/commands/__init__.py
+-rw-r--r--   0        0        0     1692 2023-07-21 19:24:17.601800 runway-2.6.7/runway/_cli/commands/_deploy.py
+-rw-r--r--   0        0        0     2192 2023-07-21 19:24:17.601800 runway-2.6.7/runway/_cli/commands/_destroy.py
+-rw-r--r--   0        0        0      796 2023-07-21 19:24:17.601800 runway-2.6.7/runway/_cli/commands/_dismantle.py
+-rw-r--r--   0        0        0     1464 2023-07-21 19:24:17.601800 runway-2.6.7/runway/_cli/commands/_docs.py
+-rw-r--r--   0        0        0     2727 2023-07-21 19:24:17.601800 runway-2.6.7/runway/_cli/commands/_envvars.py
+-rw-r--r--   0        0        0     1472 2023-07-21 19:24:17.601800 runway-2.6.7/runway/_cli/commands/_gen_sample/__init__.py
+-rw-r--r--   0        0        0     1002 2023-07-21 19:24:17.601800 runway-2.6.7/runway/_cli/commands/_gen_sample/_cdk_csharp.py
+-rw-r--r--   0        0        0      953 2023-07-21 19:24:17.601800 runway-2.6.7/runway/_cli/commands/_gen_sample/_cdk_py.py
+-rw-r--r--   0        0        0      962 2023-07-21 19:24:17.601800 runway-2.6.7/runway/_cli/commands/_gen_sample/_cdk_tsc.py
+-rw-r--r--   0        0        0      926 2023-07-21 19:24:17.601800 runway-2.6.7/runway/_cli/commands/_gen_sample/_cfn.py
+-rw-r--r--   0        0        0     1226 2023-07-21 19:24:17.601800 runway-2.6.7/runway/_cli/commands/_gen_sample/_cfngin.py
+-rw-r--r--   0        0        0     2068 2023-07-21 19:24:17.601800 runway-2.6.7/runway/_cli/commands/_gen_sample/_k8s_cfn_repo.py
+-rw-r--r--   0        0        0     1921 2023-07-21 19:24:17.601800 runway-2.6.7/runway/_cli/commands/_gen_sample/_k8s_flux_repo.py
+-rw-r--r--   0        0        0     1417 2023-07-21 19:24:17.601800 runway-2.6.7/runway/_cli/commands/_gen_sample/_k8s_tf_repo.py
+-rw-r--r--   0        0        0      998 2023-07-21 19:24:17.601800 runway-2.6.7/runway/_cli/commands/_gen_sample/_sls_py.py
+-rw-r--r--   0        0        0     1003 2023-07-21 19:24:17.601800 runway-2.6.7/runway/_cli/commands/_gen_sample/_sls_tsc.py
+-rw-r--r--   0        0        0      973 2023-07-21 19:24:17.601800 runway-2.6.7/runway/_cli/commands/_gen_sample/_static_angular.py
+-rw-r--r--   0        0        0      879 2023-07-21 19:24:17.601800 runway-2.6.7/runway/_cli/commands/_gen_sample/_static_react.py
+-rw-r--r--   0        0        0     1050 2023-07-21 19:24:17.601800 runway-2.6.7/runway/_cli/commands/_gen_sample/_tf.py
+-rw-r--r--   0        0        0     1748 2023-07-21 19:24:17.601800 runway-2.6.7/runway/_cli/commands/_gen_sample/utils.py
+-rw-r--r--   0        0        0     2106 2023-07-21 19:24:17.601800 runway-2.6.7/runway/_cli/commands/_init.py
+-rw-r--r--   0        0        0      739 2023-07-21 19:24:17.601800 runway-2.6.7/runway/_cli/commands/_kbenv/__init__.py
+-rw-r--r--   0        0        0      889 2023-07-21 19:24:17.601800 runway-2.6.7/runway/_cli/commands/_kbenv/_install.py
+-rw-r--r--   0        0        0      892 2023-07-21 19:24:17.601800 runway-2.6.7/runway/_cli/commands/_kbenv/_list.py
+-rw-r--r--   0        0        0      919 2023-07-21 19:24:17.601800 runway-2.6.7/runway/_cli/commands/_kbenv/_run.py
+-rw-r--r--   0        0        0     1851 2023-07-21 19:24:17.601800 runway-2.6.7/runway/_cli/commands/_kbenv/_uninstall.py
+-rw-r--r--   0        0        0     1395 2023-07-21 19:24:17.601800 runway-2.6.7/runway/_cli/commands/_new.py
+-rw-r--r--   0        0        0     1739 2023-07-21 19:24:17.601800 runway-2.6.7/runway/_cli/commands/_plan.py
+-rw-r--r--   0        0        0      749 2023-07-21 19:24:17.601800 runway-2.6.7/runway/_cli/commands/_preflight.py
+-rw-r--r--   0        0        0     1207 2023-07-21 19:24:17.601800 runway-2.6.7/runway/_cli/commands/_run_python.py
+-rw-r--r--   0        0        0      460 2023-07-21 19:24:17.601800 runway-2.6.7/runway/_cli/commands/_schema/__init__.py
+-rw-r--r--   0        0        0     1635 2023-07-21 19:24:17.601800 runway-2.6.7/runway/_cli/commands/_schema/_cfngin.py
+-rw-r--r--   0        0        0     1631 2023-07-21 19:24:17.601800 runway-2.6.7/runway/_cli/commands/_schema/_runway.py
+-rw-r--r--   0        0        0      783 2023-07-21 19:24:17.601800 runway-2.6.7/runway/_cli/commands/_takeoff.py
+-rw-r--r--   0        0        0      760 2023-07-21 19:24:17.601800 runway-2.6.7/runway/_cli/commands/_taxi.py
+-rw-r--r--   0        0        0      852 2023-07-21 19:24:17.601800 runway-2.6.7/runway/_cli/commands/_test.py
+-rw-r--r--   0        0        0      924 2023-07-21 19:24:17.601800 runway-2.6.7/runway/_cli/commands/_tfenv/__init__.py
+-rw-r--r--   0        0        0     1628 2023-07-21 19:24:17.601800 runway-2.6.7/runway/_cli/commands/_tfenv/_install.py
+-rw-r--r--   0        0        0      900 2023-07-21 19:24:17.601800 runway-2.6.7/runway/_cli/commands/_tfenv/_list.py
+-rw-r--r--   0        0        0     1611 2023-07-21 19:24:17.601800 runway-2.6.7/runway/_cli/commands/_tfenv/_run.py
+-rw-r--r--   0        0        0     1721 2023-07-21 19:24:17.601800 runway-2.6.7/runway/_cli/commands/_tfenv/_uninstall.py
+-rw-r--r--   0        0        0     1020 2023-07-21 19:24:17.601800 runway-2.6.7/runway/_cli/commands/_whichenv.py
+-rw-r--r--   0        0        0     4394 2023-07-21 19:24:17.601800 runway-2.6.7/runway/_cli/logs.py
+-rw-r--r--   0        0        0     2536 2023-07-21 19:24:17.601800 runway-2.6.7/runway/_cli/main.py
+-rw-r--r--   0        0        0     1175 2023-07-21 19:24:17.601800 runway-2.6.7/runway/_cli/options.py
+-rw-r--r--   0        0        0     9419 2023-07-21 19:24:17.601800 runway-2.6.7/runway/_cli/utils.py
+-rw-r--r--   0        0        0     4463 2023-07-21 19:24:17.601800 runway-2.6.7/runway/_logging.py
+-rw-r--r--   0        0        0      884 2023-07-21 19:24:17.601800 runway-2.6.7/runway/aws_sso_botocore/__init__.py
+-rw-r--r--   0        0        0    11021 2023-07-21 19:24:17.601800 runway-2.6.7/runway/aws_sso_botocore/credentials.py
+-rw-r--r--   0        0        0     1523 2023-07-21 19:24:17.601800 runway-2.6.7/runway/aws_sso_botocore/exceptions.py
+-rw-r--r--   0        0        0     1061 2023-07-21 19:24:17.601800 runway-2.6.7/runway/aws_sso_botocore/session.py
+-rw-r--r--   0        0        0     1616 2023-07-21 19:24:17.601800 runway-2.6.7/runway/aws_sso_botocore/util.py
+-rw-r--r--   0        0        0       46 2023-07-21 19:24:17.601800 runway-2.6.7/runway/blueprints/__init__.py
+-rw-r--r--   0        0        0       46 2023-07-21 19:24:17.601800 runway-2.6.7/runway/blueprints/k8s/__init__.py
+-rwxr-xr-x   0        0        0     3943 2023-07-21 19:24:17.601800 runway-2.6.7/runway/blueprints/k8s/k8s_iam.py
+-rwxr-xr-x   0        0        0     6214 2023-07-21 19:24:17.601800 runway-2.6.7/runway/blueprints/k8s/k8s_master.py
+-rwxr-xr-x   0        0        0    14269 2023-07-21 19:24:17.601800 runway-2.6.7/runway/blueprints/k8s/k8s_workers.py
+-rw-r--r--   0        0        0       46 2023-07-21 19:24:17.601800 runway-2.6.7/runway/blueprints/staticsite/__init__.py
+-rw-r--r--   0        0        0    15799 2023-07-21 19:24:17.601800 runway-2.6.7/runway/blueprints/staticsite/auth_at_edge.py
+-rwxr-xr-x   0        0        0     7147 2023-07-21 19:24:17.601800 runway-2.6.7/runway/blueprints/staticsite/dependencies.py
+-rwxr-xr-x   0        0        0    21988 2023-07-21 19:24:17.601800 runway-2.6.7/runway/blueprints/staticsite/staticsite.py
+-rw-r--r--   0        0        0      767 2023-07-21 19:24:17.601800 runway-2.6.7/runway/blueprints/staticsite/templates/cf_directory_index_rewrite.template.js
+-rwxr-xr-x   0        0        0     6045 2023-07-21 19:24:17.601800 runway-2.6.7/runway/blueprints/tf_state.py
+-rw-r--r--   0        0        0     1303 2023-07-21 19:24:17.601800 runway-2.6.7/runway/cfngin/LICENSE
+-rw-r--r--   0        0        0       46 2023-07-21 19:24:17.601800 runway-2.6.7/runway/cfngin/__init__.py
+-rw-r--r--   0        0        0       22 2023-07-21 19:24:17.605800 runway-2.6.7/runway/cfngin/actions/__init__.py
+-rw-r--r--   0        0        0    10343 2023-07-21 19:24:17.605800 runway-2.6.7/runway/cfngin/actions/base.py
+-rw-r--r--   0        0        0    22364 2023-07-21 19:24:17.605800 runway-2.6.7/runway/cfngin/actions/deploy.py
+-rw-r--r--   0        0        0     5173 2023-07-21 19:24:17.605800 runway-2.6.7/runway/cfngin/actions/destroy.py
+-rw-r--r--   0        0        0     9515 2023-07-21 19:24:17.605800 runway-2.6.7/runway/cfngin/actions/diff.py
+-rw-r--r--   0        0        0     3044 2023-07-21 19:24:17.605800 runway-2.6.7/runway/cfngin/actions/graph.py
+-rw-r--r--   0        0        0     1313 2023-07-21 19:24:17.605800 runway-2.6.7/runway/cfngin/actions/info.py
+-rw-r--r--   0        0        0     5141 2023-07-21 19:24:17.605800 runway-2.6.7/runway/cfngin/actions/init.py
+-rw-r--r--   0        0        0     2715 2023-07-21 19:24:17.605800 runway-2.6.7/runway/cfngin/awscli_yamlhelper.py
+-rw-r--r--   0        0        0       22 2023-07-21 19:24:17.605800 runway-2.6.7/runway/cfngin/blueprints/__init__.py
+-rw-r--r--   0        0        0    25454 2023-07-21 19:24:17.605800 runway-2.6.7/runway/cfngin/blueprints/base.py
+-rw-r--r--   0        0        0     4140 2023-07-21 19:24:17.605800 runway-2.6.7/runway/cfngin/blueprints/cfngin_bucket.py
+-rw-r--r--   0        0        0     8979 2023-07-21 19:24:17.605800 runway-2.6.7/runway/cfngin/blueprints/raw.py
+-rw-r--r--   0        0        0     7129 2023-07-21 19:24:17.605800 runway-2.6.7/runway/cfngin/blueprints/testutil.py
+-rw-r--r--   0        0        0     3658 2023-07-21 19:24:17.605800 runway-2.6.7/runway/cfngin/blueprints/type_defs.py
+-rw-r--r--   0        0        0       22 2023-07-21 19:24:17.605800 runway-2.6.7/runway/cfngin/blueprints/variables/__init__.py
+-rw-r--r--   0        0        0    18899 2023-07-21 19:24:17.605800 runway-2.6.7/runway/cfngin/blueprints/variables/types.py
+-rw-r--r--   0        0        0    12931 2023-07-21 19:24:17.605800 runway-2.6.7/runway/cfngin/cfngin.py
+-rw-r--r--   0        0        0    15228 2023-07-21 19:24:17.605800 runway-2.6.7/runway/cfngin/dag/__init__.py
+-rw-r--r--   0        0        0      695 2023-07-21 19:24:17.605800 runway-2.6.7/runway/cfngin/environment.py
+-rw-r--r--   0        0        0    18609 2023-07-21 19:24:17.605800 runway-2.6.7/runway/cfngin/exceptions.py
+-rw-r--r--   0        0        0       22 2023-07-21 19:24:17.605800 runway-2.6.7/runway/cfngin/hooks/__init__.py
+-rw-r--r--   0        0        0    17562 2023-07-21 19:24:17.605800 runway-2.6.7/runway/cfngin/hooks/acm.py
+-rw-r--r--   0        0        0    41530 2023-07-21 19:24:17.605800 runway-2.6.7/runway/cfngin/hooks/aws_lambda.py
+-rw-r--r--   0        0        0      483 2023-07-21 19:24:17.605800 runway-2.6.7/runway/cfngin/hooks/awslambda/__init__.py
+-rw-r--r--   0        0        0     2408 2023-07-21 19:24:17.605800 runway-2.6.7/runway/cfngin/hooks/awslambda/_python_hooks.py
+-rw-r--r--   0        0        0    16927 2023-07-21 19:24:17.605800 runway-2.6.7/runway/cfngin/hooks/awslambda/base_classes.py
+-rw-r--r--   0        0        0      350 2023-07-21 19:24:17.605800 runway-2.6.7/runway/cfngin/hooks/awslambda/constants.py
+-rw-r--r--   0        0        0    24668 2023-07-21 19:24:17.605800 runway-2.6.7/runway/cfngin/hooks/awslambda/deployment_package.py
+-rw-r--r--   0        0        0    13239 2023-07-21 19:24:17.605800 runway-2.6.7/runway/cfngin/hooks/awslambda/docker.py
+-rw-r--r--   0        0        0     1825 2023-07-21 19:24:17.605800 runway-2.6.7/runway/cfngin/hooks/awslambda/exceptions.py
+-rw-r--r--   0        0        0       19 2023-07-21 19:24:17.605800 runway-2.6.7/runway/cfngin/hooks/awslambda/models/__init__.py
+-rw-r--r--   0        0        0     9710 2023-07-21 19:24:17.605800 runway-2.6.7/runway/cfngin/hooks/awslambda/models/args.py
+-rw-r--r--   0        0        0     2628 2023-07-21 19:24:17.605800 runway-2.6.7/runway/cfngin/hooks/awslambda/models/responses.py
+-rw-r--r--   0        0        0      286 2023-07-21 19:24:17.605800 runway-2.6.7/runway/cfngin/hooks/awslambda/python_requirements/__init__.py
+-rw-r--r--   0        0        0     1769 2023-07-21 19:24:17.605800 runway-2.6.7/runway/cfngin/hooks/awslambda/python_requirements/_deployment_package.py
+-rw-r--r--   0        0        0     3594 2023-07-21 19:24:17.605800 runway-2.6.7/runway/cfngin/hooks/awslambda/python_requirements/_docker.py
+-rw-r--r--   0        0        0     6717 2023-07-21 19:24:17.605800 runway-2.6.7/runway/cfngin/hooks/awslambda/python_requirements/_project.py
+-rw-r--r--   0        0        0     5134 2023-07-21 19:24:17.605800 runway-2.6.7/runway/cfngin/hooks/awslambda/source_code.py
+-rw-r--r--   0        0        0      423 2023-07-21 19:24:17.605800 runway-2.6.7/runway/cfngin/hooks/awslambda/type_defs.py
+-rw-r--r--   0        0        0     9394 2023-07-21 19:24:17.605800 runway-2.6.7/runway/cfngin/hooks/base.py
+-rw-r--r--   0        0        0     1157 2023-07-21 19:24:17.605800 runway-2.6.7/runway/cfngin/hooks/cleanup_s3.py
+-rw-r--r--   0        0        0      895 2023-07-21 19:24:17.605800 runway-2.6.7/runway/cfngin/hooks/cleanup_ssm.py
+-rw-r--r--   0        0        0     4765 2023-07-21 19:24:17.605800 runway-2.6.7/runway/cfngin/hooks/command.py
+-rw-r--r--   0        0        0       90 2023-07-21 19:24:17.605800 runway-2.6.7/runway/cfngin/hooks/docker/__init__.py
+-rw-r--r--   0        0        0     2341 2023-07-21 19:24:17.605800 runway-2.6.7/runway/cfngin/hooks/docker/_login.py
+-rw-r--r--   0        0        0     4060 2023-07-21 19:24:17.609800 runway-2.6.7/runway/cfngin/hooks/docker/data_models.py
+-rw-r--r--   0        0        0     1475 2023-07-21 19:24:17.609800 runway-2.6.7/runway/cfngin/hooks/docker/hook_data.py
+-rw-r--r--   0        0        0      421 2023-07-21 19:24:17.609800 runway-2.6.7/runway/cfngin/hooks/docker/image/__init__.py
+-rw-r--r--   0        0        0     6815 2023-07-21 19:24:17.609800 runway-2.6.7/runway/cfngin/hooks/docker/image/_build.py
+-rw-r--r--   0        0        0     3744 2023-07-21 19:24:17.609800 runway-2.6.7/runway/cfngin/hooks/docker/image/_push.py
+-rw-r--r--   0        0        0     4357 2023-07-21 19:24:17.609800 runway-2.6.7/runway/cfngin/hooks/docker/image/_remove.py
+-rw-r--r--   0        0        0      129 2023-07-21 19:24:17.609800 runway-2.6.7/runway/cfngin/hooks/ecr/__init__.py
+-rw-r--r--   0        0        0     2983 2023-07-21 19:24:17.609800 runway-2.6.7/runway/cfngin/hooks/ecr/_purge_repository.py
+-rw-r--r--   0        0        0     1630 2023-07-21 19:24:17.609800 runway-2.6.7/runway/cfngin/hooks/ecs.py
+-rw-r--r--   0        0        0     6204 2023-07-21 19:24:17.609800 runway-2.6.7/runway/cfngin/hooks/iam.py
+-rw-r--r--   0        0        0     8766 2023-07-21 19:24:17.609800 runway-2.6.7/runway/cfngin/hooks/keypair.py
+-rw-r--r--   0        0        0     3774 2023-07-21 19:24:17.609800 runway-2.6.7/runway/cfngin/hooks/protocols.py
+-rw-r--r--   0        0        0      938 2023-07-21 19:24:17.609800 runway-2.6.7/runway/cfngin/hooks/route53.py
+-rw-r--r--   0        0        0       21 2023-07-21 19:24:17.609800 runway-2.6.7/runway/cfngin/hooks/ssm/__init__.py
+-rw-r--r--   0        0        0    11061 2023-07-21 19:24:17.609800 runway-2.6.7/runway/cfngin/hooks/ssm/parameter.py
+-rw-r--r--   0        0        0       46 2023-07-21 19:24:17.609800 runway-2.6.7/runway/cfngin/hooks/staticsite/__init__.py
+-rw-r--r--   0        0        0       46 2023-07-21 19:24:17.609800 runway-2.6.7/runway/cfngin/hooks/staticsite/auth_at_edge/__init__.py
+-rw-r--r--   0        0        0     2644 2023-07-21 19:24:17.609800 runway-2.6.7/runway/cfngin/hooks/staticsite/auth_at_edge/callback_url_retriever.py
+-rw-r--r--   0        0        0     2965 2023-07-21 19:24:17.609800 runway-2.6.7/runway/cfngin/hooks/staticsite/auth_at_edge/client_updater.py
+-rw-r--r--   0        0        0     3784 2023-07-21 19:24:17.609800 runway-2.6.7/runway/cfngin/hooks/staticsite/auth_at_edge/domain_updater.py
+-rw-r--r--   0        0        0     6704 2023-07-21 19:24:17.609800 runway-2.6.7/runway/cfngin/hooks/staticsite/auth_at_edge/lambda_config.py
+-rw-r--r--   0        0        0       46 2023-07-21 19:24:17.609800 runway-2.6.7/runway/cfngin/hooks/staticsite/auth_at_edge/templates/__init__.py
+-rw-r--r--   0        0        0     8317 2023-07-21 19:24:17.609800 runway-2.6.7/runway/cfngin/hooks/staticsite/auth_at_edge/templates/check_auth/__init__.py
+-rw-r--r--   0        0        0      106 2023-07-21 19:24:17.609800 runway-2.6.7/runway/cfngin/hooks/staticsite/auth_at_edge/templates/check_auth/requirements.txt
+-rw-r--r--   0        0        0      644 2023-07-21 19:24:17.609800 runway-2.6.7/runway/cfngin/hooks/staticsite/auth_at_edge/templates/http_headers/__init__.py
+-rw-r--r--   0        0        0     8567 2023-07-21 19:24:17.609800 runway-2.6.7/runway/cfngin/hooks/staticsite/auth_at_edge/templates/parse_auth/__init__.py
+-rw-r--r--   0        0        0      106 2023-07-21 19:24:17.609800 runway-2.6.7/runway/cfngin/hooks/staticsite/auth_at_edge/templates/parse_auth/requirements.txt
+-rw-r--r--   0        0        0     4586 2023-07-21 19:24:17.609800 runway-2.6.7/runway/cfngin/hooks/staticsite/auth_at_edge/templates/refresh_auth/__init__.py
+-rw-r--r--   0        0        0    12977 2023-07-21 19:24:17.609800 runway-2.6.7/runway/cfngin/hooks/staticsite/auth_at_edge/templates/shared.py
+-rw-r--r--   0        0        0     7518 2023-07-21 19:24:17.609800 runway-2.6.7/runway/cfngin/hooks/staticsite/auth_at_edge/templates/shared_jose.py
+-rw-r--r--   0        0        0     2314 2023-07-21 19:24:17.609800 runway-2.6.7/runway/cfngin/hooks/staticsite/auth_at_edge/templates/sign_out/__init__.py
+-rw-r--r--   0        0        0     1151 2023-07-21 19:24:17.609800 runway-2.6.7/runway/cfngin/hooks/staticsite/auth_at_edge/user_pool_id_retriever.py
+-rw-r--r--   0        0        0     6556 2023-07-21 19:24:17.609800 runway-2.6.7/runway/cfngin/hooks/staticsite/build_staticsite.py
+-rw-r--r--   0        0        0     3478 2023-07-21 19:24:17.609800 runway-2.6.7/runway/cfngin/hooks/staticsite/cleanup.py
+-rw-r--r--   0        0        0    13035 2023-07-21 19:24:17.609800 runway-2.6.7/runway/cfngin/hooks/staticsite/upload_staticsite.py
+-rw-r--r--   0        0        0     2901 2023-07-21 19:24:17.609800 runway-2.6.7/runway/cfngin/hooks/staticsite/utils.py
+-rw-r--r--   0        0        0     4913 2023-07-21 19:24:17.609800 runway-2.6.7/runway/cfngin/hooks/utils.py
+-rw-r--r--   0        0        0     1582 2023-07-21 19:24:17.609800 runway-2.6.7/runway/cfngin/logger/__init__.py
+-rw-r--r--   0        0        0      202 2023-07-21 19:24:17.609800 runway-2.6.7/runway/cfngin/lookups/__init__.py
+-rw-r--r--   0        0        0       22 2023-07-21 19:24:17.609800 runway-2.6.7/runway/cfngin/lookups/handlers/__init__.py
+-rw-r--r--   0        0        0     4480 2023-07-21 19:24:17.609800 runway-2.6.7/runway/cfngin/lookups/handlers/ami.py
+-rw-r--r--   0        0        0    16481 2023-07-21 19:24:17.609800 runway-2.6.7/runway/cfngin/lookups/handlers/awslambda.py
+-rw-r--r--   0        0        0     1682 2023-07-21 19:24:17.609800 runway-2.6.7/runway/cfngin/lookups/handlers/default.py
+-rw-r--r--   0        0        0     9590 2023-07-21 19:24:17.609800 runway-2.6.7/runway/cfngin/lookups/handlers/dynamodb.py
+-rw-r--r--   0        0        0     1667 2023-07-21 19:24:17.609800 runway-2.6.7/runway/cfngin/lookups/handlers/envvar.py
+-rw-r--r--   0        0        0     6468 2023-07-21 19:24:17.609800 runway-2.6.7/runway/cfngin/lookups/handlers/file.py
+-rw-r--r--   0        0        0     1606 2023-07-21 19:24:17.609800 runway-2.6.7/runway/cfngin/lookups/handlers/hook_data.py
+-rw-r--r--   0        0        0     2188 2023-07-21 19:24:17.609800 runway-2.6.7/runway/cfngin/lookups/handlers/kms.py
+-rw-r--r--   0        0        0     4487 2023-07-21 19:24:17.609800 runway-2.6.7/runway/cfngin/lookups/handlers/output.py
+-rw-r--r--   0        0        0     2740 2023-07-21 19:24:17.609800 runway-2.6.7/runway/cfngin/lookups/handlers/rxref.py
+-rw-r--r--   0        0        0     1649 2023-07-21 19:24:17.609800 runway-2.6.7/runway/cfngin/lookups/handlers/split.py
+-rw-r--r--   0        0        0     1765 2023-07-21 19:24:17.609800 runway-2.6.7/runway/cfngin/lookups/handlers/xref.py
+-rw-r--r--   0        0        0     4632 2023-07-21 19:24:17.609800 runway-2.6.7/runway/cfngin/lookups/registry.py
+-rw-r--r--   0        0        0    24452 2023-07-21 19:24:17.609800 runway-2.6.7/runway/cfngin/plan.py
+-rw-r--r--   0        0        0       22 2023-07-21 19:24:17.609800 runway-2.6.7/runway/cfngin/providers/__init__.py
+-rw-r--r--   0        0        0       22 2023-07-21 19:24:17.609800 runway-2.6.7/runway/cfngin/providers/aws/__init__.py
+-rw-r--r--   0        0        0    59113 2023-07-21 19:24:17.613800 runway-2.6.7/runway/cfngin/providers/aws/default.py
+-rw-r--r--   0        0        0     1403 2023-07-21 19:24:17.613800 runway-2.6.7/runway/cfngin/providers/base.py
+-rw-r--r--   0        0        0     1691 2023-07-21 19:24:17.613800 runway-2.6.7/runway/cfngin/session_cache.py
+-rw-r--r--   0        0        0     8772 2023-07-21 19:24:17.613800 runway-2.6.7/runway/cfngin/stack.py
+-rw-r--r--   0        0        0     4381 2023-07-21 19:24:17.613800 runway-2.6.7/runway/cfngin/status.py
+-rw-r--r--   0        0        0     1556 2023-07-21 19:24:17.613800 runway-2.6.7/runway/cfngin/tokenize_userdata.py
+-rw-r--r--   0        0        0     2914 2023-07-21 19:24:17.613800 runway-2.6.7/runway/cfngin/ui.py
+-rw-r--r--   0        0        0    30329 2023-07-21 19:24:17.613800 runway-2.6.7/runway/cfngin/utils.py
+-rw-r--r--   0        0        0      691 2023-07-21 19:24:17.613800 runway-2.6.7/runway/compat.py
+-rw-r--r--   0        0        0    18286 2023-07-21 19:24:17.613800 runway-2.6.7/runway/config/__init__.py
+-rw-r--r--   0        0        0       41 2023-07-21 19:24:17.613800 runway-2.6.7/runway/config/components/__init__.py
+-rw-r--r--   0        0        0      587 2023-07-21 19:24:17.613800 runway-2.6.7/runway/config/components/runway/__init__.py
+-rw-r--r--   0        0        0     6199 2023-07-21 19:24:17.613800 runway-2.6.7/runway/config/components/runway/_deployment_def.py
+-rw-r--r--   0        0        0     3891 2023-07-21 19:24:17.613800 runway-2.6.7/runway/config/components/runway/_module_def.py
+-rw-r--r--   0        0        0     4821 2023-07-21 19:24:17.613800 runway-2.6.7/runway/config/components/runway/_test_def.py
+-rw-r--r--   0        0        0     2318 2023-07-21 19:24:17.613800 runway-2.6.7/runway/config/components/runway/_variables_def.py
+-rw-r--r--   0        0        0     6232 2023-07-21 19:24:17.613800 runway-2.6.7/runway/config/components/runway/base.py
+-rw-r--r--   0        0        0       37 2023-07-21 19:24:17.613800 runway-2.6.7/runway/config/models/__init__.py
+-rw-r--r--   0        0        0      351 2023-07-21 19:24:17.613800 runway-2.6.7/runway/config/models/base.py
+-rw-r--r--   0        0        0    14051 2023-07-21 19:24:17.613800 runway-2.6.7/runway/config/models/cfngin/__init__.py
+-rw-r--r--   0        0        0     6629 2023-07-21 19:24:17.613800 runway-2.6.7/runway/config/models/cfngin/_package_sources.py
+-rw-r--r--   0        0        0    24455 2023-07-21 19:24:17.613800 runway-2.6.7/runway/config/models/runway/__init__.py
+-rw-r--r--   0        0        0     5959 2023-07-21 19:24:17.613800 runway-2.6.7/runway/config/models/runway/_builtin_tests.py
+-rw-r--r--   0        0        0       29 2023-07-21 19:24:17.613800 runway-2.6.7/runway/config/models/runway/options/__init__.py
+-rw-r--r--   0        0        0      542 2023-07-21 19:24:17.613800 runway-2.6.7/runway/config/models/runway/options/cdk.py
+-rw-r--r--   0        0        0      546 2023-07-21 19:24:17.613800 runway-2.6.7/runway/config/models/runway/options/k8s.py
+-rw-r--r--   0        0        0     1209 2023-07-21 19:24:17.613800 runway-2.6.7/runway/config/models/runway/options/serverless.py
+-rw-r--r--   0        0        0     2299 2023-07-21 19:24:17.613800 runway-2.6.7/runway/config/models/runway/options/terraform.py
+-rw-r--r--   0        0        0      920 2023-07-21 19:24:17.613800 runway-2.6.7/runway/config/models/utils.py
+-rw-r--r--   0        0        0      292 2023-07-21 19:24:17.613800 runway-2.6.7/runway/constants.py
+-rw-r--r--   0        0        0      139 2023-07-21 19:24:17.613800 runway-2.6.7/runway/context/__init__.py
+-rw-r--r--   0        0        0     5799 2023-07-21 19:24:17.613800 runway-2.6.7/runway/context/_base.py
+-rw-r--r--   0        0        0    19344 2023-07-21 19:24:17.613800 runway-2.6.7/runway/context/_cfngin.py
+-rw-r--r--   0        0        0     3310 2023-07-21 19:24:17.613800 runway-2.6.7/runway/context/_runway.py
+-rw-r--r--   0        0        0     2762 2023-07-21 19:24:17.613800 runway-2.6.7/runway/context/sys_info.py
+-rw-r--r--   0        0        0      239 2023-07-21 19:24:17.613800 runway-2.6.7/runway/context/type_defs.py
+-rw-r--r--   0        0        0     8802 2023-07-21 19:24:17.613800 runway-2.6.7/runway/core/__init__.py
+-rw-r--r--   0        0        0      415 2023-07-21 19:24:17.613800 runway-2.6.7/runway/core/components/__init__.py
+-rw-r--r--   0        0        0    12693 2023-07-21 19:24:17.613800 runway-2.6.7/runway/core/components/_deploy_environment.py
+-rw-r--r--   0        0        0    11159 2023-07-21 19:24:17.613800 runway-2.6.7/runway/core/components/_deployment.py
+-rw-r--r--   0        0        0    13116 2023-07-21 19:24:17.613800 runway-2.6.7/runway/core/components/_module.py
+-rw-r--r--   0        0        0     5702 2023-07-21 19:24:17.613800 runway-2.6.7/runway/core/components/_module_path.py
+-rw-r--r--   0        0        0     7426 2023-07-21 19:24:17.613800 runway-2.6.7/runway/core/components/_module_type.py
+-rw-r--r--   0        0        0       24 2023-07-21 19:24:17.613800 runway-2.6.7/runway/core/providers/__init__.py
+-rw-r--r--   0        0        0      316 2023-07-21 19:24:17.613800 runway-2.6.7/runway/core/providers/aws/__init__.py
+-rw-r--r--   0        0        0     1659 2023-07-21 19:24:17.613800 runway-2.6.7/runway/core/providers/aws/_account.py
+-rw-r--r--   0        0        0     5163 2023-07-21 19:24:17.613800 runway-2.6.7/runway/core/providers/aws/_assume_role.py
+-rw-r--r--   0        0        0     2913 2023-07-21 19:24:17.613800 runway-2.6.7/runway/core/providers/aws/_response.py
+-rw-r--r--   0        0        0      111 2023-07-21 19:24:17.613800 runway-2.6.7/runway/core/providers/aws/s3/__init__.py
+-rw-r--r--   0        0        0     7768 2023-07-21 19:24:17.613800 runway-2.6.7/runway/core/providers/aws/s3/_bucket.py
+-rw-r--r--   0        0        0       22 2023-07-21 19:24:17.613800 runway-2.6.7/runway/core/providers/aws/s3/_helpers/__init__.py
+-rw-r--r--   0        0        0     9926 2023-07-21 19:24:17.613800 runway-2.6.7/runway/core/providers/aws/s3/_helpers/action_architecture.py
+-rw-r--r--   0        0        0     6356 2023-07-21 19:24:17.613800 runway-2.6.7/runway/core/providers/aws/s3/_helpers/comparator.py
+-rw-r--r--   0        0        0    15217 2023-07-21 19:24:17.617800 runway-2.6.7/runway/core/providers/aws/s3/_helpers/file_generator.py
+-rw-r--r--   0        0        0     5021 2023-07-21 19:24:17.617800 runway-2.6.7/runway/core/providers/aws/s3/_helpers/file_info.py
+-rw-r--r--   0        0        0     2227 2023-07-21 19:24:17.617800 runway-2.6.7/runway/core/providers/aws/s3/_helpers/file_info_builder.py
+-rw-r--r--   0        0        0     6951 2023-07-21 19:24:17.617800 runway-2.6.7/runway/core/providers/aws/s3/_helpers/filters.py
+-rw-r--r--   0        0        0     4450 2023-07-21 19:24:17.617800 runway-2.6.7/runway/core/providers/aws/s3/_helpers/format_path.py
+-rw-r--r--   0        0        0     5394 2023-07-21 19:24:17.617800 runway-2.6.7/runway/core/providers/aws/s3/_helpers/parameters.py
+-rw-r--r--   0        0        0    29422 2023-07-21 19:24:17.617800 runway-2.6.7/runway/core/providers/aws/s3/_helpers/results.py
+-rw-r--r--   0        0        0    30172 2023-07-21 19:24:17.617800 runway-2.6.7/runway/core/providers/aws/s3/_helpers/s3handler.py
+-rw-r--r--   0        0        0      660 2023-07-21 19:24:17.617800 runway-2.6.7/runway/core/providers/aws/s3/_helpers/sync_strategy/__init__.py
+-rw-r--r--   0        0        0     7782 2023-07-21 19:24:17.617800 runway-2.6.7/runway/core/providers/aws/s3/_helpers/sync_strategy/base.py
+-rw-r--r--   0        0        0     1126 2023-07-21 19:24:17.617800 runway-2.6.7/runway/core/providers/aws/s3/_helpers/sync_strategy/delete.py
+-rw-r--r--   0        0        0     1461 2023-07-21 19:24:17.617800 runway-2.6.7/runway/core/providers/aws/s3/_helpers/sync_strategy/exact_timestamps.py
+-rw-r--r--   0        0        0     1549 2023-07-21 19:24:17.617800 runway-2.6.7/runway/core/providers/aws/s3/_helpers/sync_strategy/register.py
+-rw-r--r--   0        0        0     1208 2023-07-21 19:24:17.617800 runway-2.6.7/runway/core/providers/aws/s3/_helpers/sync_strategy/size_only.py
+-rw-r--r--   0        0        0     5439 2023-07-21 19:24:17.617800 runway-2.6.7/runway/core/providers/aws/s3/_helpers/transfer_config.py
+-rw-r--r--   0        0        0    32879 2023-07-21 19:24:17.617800 runway-2.6.7/runway/core/providers/aws/s3/_helpers/utils.py
+-rw-r--r--   0        0        0     3088 2023-07-21 19:24:17.617800 runway-2.6.7/runway/core/providers/aws/s3/_sync_handler.py
+-rw-r--r--   0        0        0     1609 2023-07-21 19:24:17.617800 runway-2.6.7/runway/core/providers/aws/s3/exceptions.py
+-rw-r--r--   0        0        0      253 2023-07-21 19:24:17.617800 runway-2.6.7/runway/core/providers/aws/type_defs.py
+-rw-r--r--   0        0        0      174 2023-07-21 19:24:17.617800 runway-2.6.7/runway/core/type_defs.py
+-rw-r--r--   0        0        0      514 2023-07-21 19:24:17.617800 runway-2.6.7/runway/dependency_managers/__init__.py
+-rw-r--r--   0        0        0     6370 2023-07-21 19:24:17.617800 runway-2.6.7/runway/dependency_managers/_pip.py
+-rw-r--r--   0        0        0     3799 2023-07-21 19:24:17.617800 runway-2.6.7/runway/dependency_managers/_pipenv.py
+-rw-r--r--   0        0        0     4732 2023-07-21 19:24:17.617800 runway-2.6.7/runway/dependency_managers/_poetry.py
+-rw-r--r--   0        0        0     1595 2023-07-21 19:24:17.617800 runway-2.6.7/runway/dependency_managers/base_classes.py
+-rw-r--r--   0        0        0     5147 2023-07-21 19:24:17.617800 runway-2.6.7/runway/env_mgr/__init__.py
+-rw-r--r--   0        0        0    10321 2023-07-21 19:24:17.617800 runway-2.6.7/runway/env_mgr/kbenv.py
+-rw-r--r--   0        0        0    15186 2023-07-21 19:24:17.617800 runway-2.6.7/runway/env_mgr/tfenv.py
+-rw-r--r--   0        0        0    10958 2023-07-21 19:24:17.617800 runway-2.6.7/runway/exceptions.py
+-rw-r--r--   0        0        0       46 2023-07-21 19:24:17.617800 runway-2.6.7/runway/lookups/__init__.py
+-rw-r--r--   0        0        0      147 2023-07-21 19:24:17.617800 runway-2.6.7/runway/lookups/handlers/__init__.py
+-rw-r--r--   0        0        0    10273 2023-07-21 19:24:17.617800 runway-2.6.7/runway/lookups/handlers/base.py
+-rw-r--r--   0        0        0     4919 2023-07-21 19:24:17.617800 runway-2.6.7/runway/lookups/handlers/cfn.py
+-rw-r--r--   0        0        0     1875 2023-07-21 19:24:17.617800 runway-2.6.7/runway/lookups/handlers/ecr.py
+-rw-r--r--   0        0        0     1673 2023-07-21 19:24:17.617800 runway-2.6.7/runway/lookups/handlers/env.py
+-rw-r--r--   0        0        0     3793 2023-07-21 19:24:17.617800 runway-2.6.7/runway/lookups/handlers/random_string.py
+-rw-r--r--   0        0        0     1790 2023-07-21 19:24:17.617800 runway-2.6.7/runway/lookups/handlers/ssm.py
+-rw-r--r--   0        0        0     1551 2023-07-21 19:24:17.617800 runway-2.6.7/runway/lookups/handlers/var.py
+-rw-r--r--   0        0        0     2120 2023-07-21 19:24:17.617800 runway-2.6.7/runway/lookups/registry.py
+-rw-r--r--   0        0        0     5049 2023-07-21 19:24:17.617800 runway-2.6.7/runway/mixins.py
+-rw-r--r--   0        0        0       70 2023-07-21 19:24:17.617800 runway-2.6.7/runway/module/__init__.py
+-rw-r--r--   0        0        0     7974 2023-07-21 19:24:17.617800 runway-2.6.7/runway/module/base.py
+-rw-r--r--   0        0        0    10626 2023-07-21 19:24:17.617800 runway-2.6.7/runway/module/cdk.py
+-rw-r--r--   0        0        0     3132 2023-07-21 19:24:17.617800 runway-2.6.7/runway/module/cloudformation.py
+-rw-r--r--   0        0        0    10461 2023-07-21 19:24:17.617800 runway-2.6.7/runway/module/k8s.py
+-rw-r--r--   0        0        0    19334 2023-07-21 19:24:17.617800 runway-2.6.7/runway/module/serverless.py
+-rw-r--r--   0        0        0       91 2023-07-21 19:24:17.617800 runway-2.6.7/runway/module/staticsite/__init__.py
+-rw-r--r--   0        0        0    26533 2023-07-21 19:24:17.617800 runway-2.6.7/runway/module/staticsite/handler.py
+-rw-r--r--   0        0        0      605 2023-07-21 19:24:17.617800 runway-2.6.7/runway/module/staticsite/options/__init__.py
+-rw-r--r--   0        0        0     1457 2023-07-21 19:24:17.617800 runway-2.6.7/runway/module/staticsite/options/components.py
+-rw-r--r--   0        0        0     5411 2023-07-21 19:24:17.617800 runway-2.6.7/runway/module/staticsite/options/models.py
+-rw-r--r--   0        0        0      395 2023-07-21 19:24:17.621800 runway-2.6.7/runway/module/staticsite/parameters/__init__.py
+-rw-r--r--   0        0        0     8648 2023-07-21 19:24:17.621800 runway-2.6.7/runway/module/staticsite/parameters/models.py
+-rw-r--r--   0        0        0      277 2023-07-21 19:24:17.621800 runway-2.6.7/runway/module/staticsite/utils.py
+-rw-r--r--   0        0        0    25863 2023-07-21 19:24:17.621800 runway-2.6.7/runway/module/terraform.py
+-rw-r--r--   0        0        0     4106 2023-07-21 19:24:17.621800 runway-2.6.7/runway/module/utils.py
+-rw-r--r--   0        0        0     7947 2023-07-21 19:24:17.621800 runway-2.6.7/runway/s3_utils.py
+-rw-r--r--   0        0        0       46 2023-07-21 19:24:17.621800 runway-2.6.7/runway/sources/__init__.py
+-rw-r--r--   0        0        0     4143 2023-07-21 19:24:17.621800 runway-2.6.7/runway/sources/git.py
+-rw-r--r--   0        0        0     1864 2023-07-21 19:24:17.621800 runway-2.6.7/runway/sources/source.py
+-rw-r--r--   0        0        0       53 2023-07-21 19:24:17.621800 runway-2.6.7/runway/templates/.flake8
+-rw-r--r--   0        0        0    16636 2023-07-21 19:24:17.621800 runway-2.6.7/runway/templates/.pylintrc
+-rw-r--r--   0        0        0      408 2023-07-21 19:24:17.621800 runway-2.6.7/runway/templates/.yamllint.yml
+-rw-r--r--   0        0        0      703 2023-07-21 19:24:17.621800 runway-2.6.7/runway/templates/cdk-csharp/README.md
+-rw-r--r--   0        0        0       85 2023-07-21 19:24:17.621800 runway-2.6.7/runway/templates/cdk-csharp/add-project.hook.d.ts
+-rw-r--r--   0        0        0      101 2023-07-21 19:24:17.621800 runway-2.6.7/runway/templates/cdk-csharp/cdk.json
+-rw-r--r--   0        0        0     5721 2023-07-21 19:24:17.621800 runway-2.6.7/runway/templates/cdk-csharp/dot_gitignore
+-rw-r--r--   0        0        0      261 2023-07-21 19:24:17.621800 runway-2.6.7/runway/templates/cdk-csharp/package.json
+-rw-r--r--   0        0        0       51 2023-07-21 19:24:17.621800 runway-2.6.7/runway/templates/cdk-csharp/runway.module.yml
+-rw-r--r--   0        0        0      476 2023-07-21 19:24:17.621800 runway-2.6.7/runway/templates/cdk-csharp/src/HelloCdk/HelloCdk.csproj
+-rw-r--r--   0        0        0     1009 2023-07-21 19:24:17.621800 runway-2.6.7/runway/templates/cdk-csharp/src/HelloCdk/HelloConstruct.cs
+-rw-r--r--   0        0        0     1166 2023-07-21 19:24:17.621800 runway-2.6.7/runway/templates/cdk-csharp/src/HelloCdk/HelloStack.cs
+-rw-r--r--   0        0        0      537 2023-07-21 19:24:17.621800 runway-2.6.7/runway/templates/cdk-csharp/src/HelloCdk/Program.cs
+-rw-r--r--   0        0        0     1697 2023-07-21 19:24:17.621800 runway-2.6.7/runway/templates/cdk-csharp/src/HelloCdk.sln
+-rw-r--r--   0        0        0       21 2023-07-21 19:24:17.621800 runway-2.6.7/runway/templates/cdk-py/.gitignore
+-rw-r--r--   0        0        0      172 2023-07-21 19:24:17.621800 runway-2.6.7/runway/templates/cdk-py/app.py
+-rw-r--r--   0        0        0       69 2023-07-21 19:24:17.621800 runway-2.6.7/runway/templates/cdk-py/cdk.json
+-rw-r--r--   0        0        0       46 2023-07-21 19:24:17.621800 runway-2.6.7/runway/templates/cdk-py/hello/__init__.py
+-rw-r--r--   0        0        0      736 2023-07-21 19:24:17.621800 runway-2.6.7/runway/templates/cdk-py/hello/hello_construct.py
+-rw-r--r--   0        0        0      850 2023-07-21 19:24:17.621800 runway-2.6.7/runway/templates/cdk-py/hello/hello_stack.py
+-rw-r--r--   0        0        0      239 2023-07-21 19:24:17.621800 runway-2.6.7/runway/templates/cdk-py/package.json
+-rw-r--r--   0        0        0    22817 2023-07-21 19:24:17.621800 runway-2.6.7/runway/templates/cdk-py/poetry.lock
+-rw-r--r--   0        0        0      514 2023-07-21 19:24:17.621800 runway-2.6.7/runway/templates/cdk-py/pyproject.toml
+-rw-r--r--   0        0        0       49 2023-07-21 19:24:17.621800 runway-2.6.7/runway/templates/cdk-py/runway.module.yml
+-rw-r--r--   0        0        0       33 2023-07-21 19:24:17.621800 runway-2.6.7/runway/templates/cdk-tsc/.gitignore
+-rw-r--r--   0        0        0       13 2023-07-21 19:24:17.621800 runway-2.6.7/runway/templates/cdk-tsc/.npmignore
+-rw-r--r--   0        0        0      315 2023-07-21 19:24:17.621800 runway-2.6.7/runway/templates/cdk-tsc/README.md
+-rw-r--r--   0        0        0      213 2023-07-21 19:24:17.621800 runway-2.6.7/runway/templates/cdk-tsc/bin/sample.ts
+-rw-r--r--   0        0        0       63 2023-07-21 19:24:17.621800 runway-2.6.7/runway/templates/cdk-tsc/cdk.json
+-rw-r--r--   0        0        0      239 2023-07-21 19:24:17.621800 runway-2.6.7/runway/templates/cdk-tsc/lib/sample-stack.ts
+-rw-r--r--   0        0        0      448 2023-07-21 19:24:17.621800 runway-2.6.7/runway/templates/cdk-tsc/package.json
+-rw-r--r--   0        0        0       48 2023-07-21 19:24:17.621800 runway-2.6.7/runway/templates/cdk-tsc/runway.module.yml
+-rw-r--r--   0        0        0      620 2023-07-21 19:24:17.621800 runway-2.6.7/runway/templates/cdk-tsc/tsconfig.json
+-rw-r--r--   0        0        0      229 2023-07-21 19:24:17.621800 runway-2.6.7/runway/templates/cfn/dev-us-east-1.env
+-rw-r--r--   0        0        0      305 2023-07-21 19:24:17.621800 runway-2.6.7/runway/templates/cfn/stacks.yaml
+-rw-r--r--   0        0        0      240 2023-07-21 19:24:17.621800 runway-2.6.7/runway/templates/cfngin/dev-us-east-1.env
+-rw-r--r--   0        0        0      283 2023-07-21 19:24:17.621800 runway-2.6.7/runway/templates/cfngin/stacks.yaml
+-rw-r--r--   0        0        0     2319 2023-07-21 19:24:17.621800 runway-2.6.7/runway/templates/k8s-cfn-repo/README.md
+-rw-r--r--   0        0        0       35 2023-07-21 19:24:17.621800 runway-2.6.7/runway/templates/k8s-cfn-repo/_gitignore
+-rw-r--r--   0        0        0       44 2023-07-21 19:24:17.621800 runway-2.6.7/runway/templates/k8s-cfn-repo/aws-auth-cm.k8s/base/kustomization.yaml
+-rw-r--r--   0        0        0        7 2023-07-21 19:24:17.621800 runway-2.6.7/runway/templates/k8s-cfn-repo/aws-auth-cm.k8s/overlays/template/.kubectl-version
+-rw-r--r--   0        0        0       54 2023-07-21 19:24:17.621800 runway-2.6.7/runway/templates/k8s-cfn-repo/aws-auth-cm.k8s/overlays/template/kustomization.yaml
+-rw-r--r--   0        0        0       51 2023-07-21 19:24:17.621800 runway-2.6.7/runway/templates/k8s-cfn-repo/k8s-master.cfn/k8s_hooks/__init__.py
+-rw-r--r--   0        0        0     2819 2023-07-21 19:24:17.621800 runway-2.6.7/runway/templates/k8s-cfn-repo/k8s-master.cfn/k8s_hooks/auth_map.py
+-rw-r--r--   0        0        0      377 2023-07-21 19:24:17.621800 runway-2.6.7/runway/templates/k8s-cfn-repo/k8s-master.cfn/k8s_hooks/aws-auth-cm.yaml
+-rw-r--r--   0        0        0     1643 2023-07-21 19:24:17.621800 runway-2.6.7/runway/templates/k8s-cfn-repo/k8s-master.cfn/k8s_hooks/awscli.py
+-rw-r--r--   0        0        0     3153 2023-07-21 19:24:17.621800 runway-2.6.7/runway/templates/k8s-cfn-repo/k8s-master.cfn/k8s_hooks/bootstrap.py
+-rw-r--r--   0        0        0     1078 2023-07-21 19:24:17.621800 runway-2.6.7/runway/templates/k8s-cfn-repo/k8s-master.cfn/stacks.yaml
+-rw-r--r--   0        0        0      120 2023-07-21 19:24:17.621800 runway-2.6.7/runway/templates/k8s-cfn-repo/k8s-workers.cfn/local_lookups/__init__.py
+-rw-r--r--   0        0        0     1893 2023-07-21 19:24:17.621800 runway-2.6.7/runway/templates/k8s-cfn-repo/k8s-workers.cfn/local_lookups/bootstrap_value.py
+-rw-r--r--   0        0        0     1276 2023-07-21 19:24:17.621800 runway-2.6.7/runway/templates/k8s-cfn-repo/k8s-workers.cfn/stacks.yaml
+-rw-r--r--   0        0        0     1095 2023-07-21 19:24:17.621800 runway-2.6.7/runway/templates/k8s-cfn-repo/runway.yml
+-rw-r--r--   0        0        0      107 2023-07-21 19:24:17.621800 runway-2.6.7/runway/templates/k8s-cfn-repo/service-hello-world.k8s/README.md
+-rw-r--r--   0        0        0      117 2023-07-21 19:24:17.621800 runway-2.6.7/runway/templates/k8s-cfn-repo/service-hello-world.k8s/base/configMap.yaml
+-rw-r--r--   0        0        0      755 2023-07-21 19:24:17.621800 runway-2.6.7/runway/templates/k8s-cfn-repo/service-hello-world.k8s/base/deployment.yaml
+-rw-r--r--   0        0        0      176 2023-07-21 19:24:17.621800 runway-2.6.7/runway/templates/k8s-cfn-repo/service-hello-world.k8s/base/kustomization.yaml
+-rw-r--r--   0        0        0      189 2023-07-21 19:24:17.621800 runway-2.6.7/runway/templates/k8s-cfn-repo/service-hello-world.k8s/base/service.yaml
+-rw-r--r--   0        0        0        7 2023-07-21 19:24:17.621800 runway-2.6.7/runway/templates/k8s-cfn-repo/service-hello-world.k8s/overlays/prod/.kubectl-version
+-rw-r--r--   0        0        0       91 2023-07-21 19:24:17.621800 runway-2.6.7/runway/templates/k8s-cfn-repo/service-hello-world.k8s/overlays/prod/deployment.yaml
+-rw-r--r--   0        0        0      177 2023-07-21 19:24:17.621800 runway-2.6.7/runway/templates/k8s-cfn-repo/service-hello-world.k8s/overlays/prod/kustomization.yaml
+-rw-r--r--   0        0        0        7 2023-07-21 19:24:17.621800 runway-2.6.7/runway/templates/k8s-cfn-repo/service-hello-world.k8s/overlays/template/.kubectl-version
+-rw-r--r--   0        0        0      188 2023-07-21 19:24:17.621800 runway-2.6.7/runway/templates/k8s-cfn-repo/service-hello-world.k8s/overlays/template/kustomization.yaml
+-rw-r--r--   0        0        0      118 2023-07-21 19:24:17.621800 runway-2.6.7/runway/templates/k8s-cfn-repo/service-hello-world.k8s/overlays/template/map.yaml
+-rw-r--r--   0        0        0        7 2023-07-21 19:24:17.621800 runway-2.6.7/runway/templates/k8s-flux-repo/.kubectl-version
+-rw-r--r--   0        0        0     3343 2023-07-21 19:24:17.621800 runway-2.6.7/runway/templates/k8s-flux-repo/README.md
+-rw-r--r--   0        0        0      120 2023-07-21 19:24:17.621800 runway-2.6.7/runway/templates/k8s-flux-repo/_gitignore
+-rw-r--r--   0        0        0      109 2023-07-21 19:24:17.621800 runway-2.6.7/runway/templates/k8s-flux-repo/flux-dev/README.md
+-rw-r--r--   0        0        0       33 2023-07-21 19:24:17.621800 runway-2.6.7/runway/templates/k8s-flux-repo/flux-dev/namespaces/README.md
+-rw-r--r--   0        0        0       79 2023-07-21 19:24:17.621800 runway-2.6.7/runway/templates/k8s-flux-repo/flux-dev/namespaces/demo.yaml
+-rw-r--r--   0        0        0       31 2023-07-21 19:24:17.621800 runway-2.6.7/runway/templates/k8s-flux-repo/flux-dev/workloads/README.md
+-rw-r--r--   0        0        0       12 2023-07-21 19:24:17.621800 runway-2.6.7/runway/templates/k8s-flux-repo/flux.tf/.terraform-version
+-rw-r--r--   0        0        0     3268 2023-07-21 19:24:17.621800 runway-2.6.7/runway/templates/k8s-flux-repo/flux.tf/.terraform.lock.hcl
+-rw-r--r--   0        0        0      718 2023-07-21 19:24:17.621800 runway-2.6.7/runway/templates/k8s-flux-repo/flux.tf/docker/Dockerfile
+-rw-r--r--   0        0        0    12304 2023-07-21 19:24:17.621800 runway-2.6.7/runway/templates/k8s-flux-repo/flux.tf/main.tf
+-rw-r--r--   0        0        0       56 2023-07-21 19:24:17.621800 runway-2.6.7/runway/templates/k8s-flux-repo/flux.tf/sleep.py
+-rw-r--r--   0        0        0      780 2023-07-21 19:24:17.621800 runway-2.6.7/runway/templates/k8s-flux-repo/runway.yml
+-rw-r--r--   0        0        0        7 2023-07-21 19:24:17.621800 runway-2.6.7/runway/templates/k8s-tf-repo/.kubectl-version
+-rw-r--r--   0        0        0     3600 2023-07-21 19:24:17.621800 runway-2.6.7/runway/templates/k8s-tf-repo/README.md
+-rw-r--r--   0        0        0       46 2023-07-21 19:24:17.621800 runway-2.6.7/runway/templates/k8s-tf-repo/_gitignore
+-rw-r--r--   0        0        0       12 2023-07-21 19:24:17.621800 runway-2.6.7/runway/templates/k8s-tf-repo/eks-base.tf/.terraform-version
+-rw-r--r--   0        0        0     3123 2023-07-21 19:24:17.621800 runway-2.6.7/runway/templates/k8s-tf-repo/eks-base.tf/.terraform.lock.hcl
+-rw-r--r--   0        0        0     8778 2023-07-21 19:24:17.621800 runway-2.6.7/runway/templates/k8s-tf-repo/eks-base.tf/main.tf
+-rw-r--r--   0        0        0       57 2023-07-21 19:24:17.621800 runway-2.6.7/runway/templates/k8s-tf-repo/eks-base.tf/sleep.py
+-rw-r--r--   0        0        0      222 2023-07-21 19:24:17.621800 runway-2.6.7/runway/templates/k8s-tf-repo/gen-kubeconfig.cfn/hooks.yaml
+-rw-r--r--   0        0        0       51 2023-07-21 19:24:17.621800 runway-2.6.7/runway/templates/k8s-tf-repo/gen-kubeconfig.cfn/k8s_hooks/__init__.py
+-rw-r--r--   0        0        0       12 2023-07-21 19:24:17.625800 runway-2.6.7/runway/templates/k8s-tf-repo/job-s3-echo.tf/.terraform-version
+-rw-r--r--   0        0        0     2114 2023-07-21 19:24:17.625800 runway-2.6.7/runway/templates/k8s-tf-repo/job-s3-echo.tf/.terraform.lock.hcl
+-rw-r--r--   0        0        0     4464 2023-07-21 19:24:17.625800 runway-2.6.7/runway/templates/k8s-tf-repo/job-s3-echo.tf/main.tf
+-rw-r--r--   0        0        0       56 2023-07-21 19:24:17.625800 runway-2.6.7/runway/templates/k8s-tf-repo/job-s3-echo.tf/sleep.py
+-rw-r--r--   0        0        0      825 2023-07-21 19:24:17.625800 runway-2.6.7/runway/templates/k8s-tf-repo/runway.yml
+-rw-r--r--   0        0        0      107 2023-07-21 19:24:17.625800 runway-2.6.7/runway/templates/k8s-tf-repo/service-hello-world.k8s/README.md
+-rw-r--r--   0        0        0      117 2023-07-21 19:24:17.625800 runway-2.6.7/runway/templates/k8s-tf-repo/service-hello-world.k8s/base/configMap.yaml
+-rw-r--r--   0        0        0      755 2023-07-21 19:24:17.625800 runway-2.6.7/runway/templates/k8s-tf-repo/service-hello-world.k8s/base/deployment.yaml
+-rw-r--r--   0        0        0      176 2023-07-21 19:24:17.625800 runway-2.6.7/runway/templates/k8s-tf-repo/service-hello-world.k8s/base/kustomization.yaml
+-rw-r--r--   0        0        0      189 2023-07-21 19:24:17.625800 runway-2.6.7/runway/templates/k8s-tf-repo/service-hello-world.k8s/base/service.yaml
+-rw-r--r--   0        0        0        7 2023-07-21 19:24:17.625800 runway-2.6.7/runway/templates/k8s-tf-repo/service-hello-world.k8s/overlays/dev/.kubectl-version
+-rw-r--r--   0        0        0      161 2023-07-21 19:24:17.625800 runway-2.6.7/runway/templates/k8s-tf-repo/service-hello-world.k8s/overlays/dev/kustomization.yaml
+-rw-r--r--   0        0        0      118 2023-07-21 19:24:17.625800 runway-2.6.7/runway/templates/k8s-tf-repo/service-hello-world.k8s/overlays/dev/map.yaml
+-rw-r--r--   0        0        0        7 2023-07-21 19:24:17.625800 runway-2.6.7/runway/templates/k8s-tf-repo/service-hello-world.k8s/overlays/prod/.kubectl-version
+-rw-r--r--   0        0        0       91 2023-07-21 19:24:17.625800 runway-2.6.7/runway/templates/k8s-tf-repo/service-hello-world.k8s/overlays/prod/deployment.yaml
+-rw-r--r--   0        0        0      177 2023-07-21 19:24:17.625800 runway-2.6.7/runway/templates/k8s-tf-repo/service-hello-world.k8s/overlays/prod/kustomization.yaml
+-rw-r--r--   0        0        0      440 2023-07-21 19:24:17.625800 runway-2.6.7/runway/templates/k8s-tf-repo/tfstate.cfn/stacks.yaml
+-rw-r--r--   0        0        0       69 2023-07-21 19:24:17.625800 runway-2.6.7/runway/templates/sls-py/__init__.py
+-rw-r--r--   0        0        0       31 2023-07-21 19:24:17.625800 runway-2.6.7/runway/templates/sls-py/_gitignore
+-rw-r--r--   0        0        0        5 2023-07-21 19:24:17.625800 runway-2.6.7/runway/templates/sls-py/config-dev-us-east-1.json
+-rw-r--r--   0        0        0      683 2023-07-21 19:24:17.625800 runway-2.6.7/runway/templates/sls-py/hello_world/__init__.py
+-rw-r--r--   0        0        0      290 2023-07-21 19:24:17.625800 runway-2.6.7/runway/templates/sls-py/package.json
+-rw-r--r--   0        0        0     4451 2023-07-21 19:24:17.625800 runway-2.6.7/runway/templates/sls-py/poetry.lock
+-rw-r--r--   0        0        0      354 2023-07-21 19:24:17.625800 runway-2.6.7/runway/templates/sls-py/pyproject.toml
+-rw-r--r--   0        0        0      529 2023-07-21 19:24:17.625800 runway-2.6.7/runway/templates/sls-py/serverless.yml
+-rw-r--r--   0        0        0       27 2023-07-21 19:24:17.625800 runway-2.6.7/runway/templates/sls-tsc/.eslintignore
+-rw-r--r--   0        0        0      265 2023-07-21 19:24:17.625800 runway-2.6.7/runway/templates/sls-tsc/.eslintrc.js
+-rw-r--r--   0        0        0       49 2023-07-21 19:24:17.625800 runway-2.6.7/runway/templates/sls-tsc/_gitignore
+-rw-r--r--   0        0        0      281 2023-07-21 19:24:17.625800 runway-2.6.7/runway/templates/sls-tsc/jest.config.js
+-rw-r--r--   0        0        0     1087 2023-07-21 19:24:17.625800 runway-2.6.7/runway/templates/sls-tsc/package.json
+-rw-r--r--   0        0        0      642 2023-07-21 19:24:17.625800 runway-2.6.7/runway/templates/sls-tsc/serverless.yml
+-rw-r--r--   0        0        0      787 2023-07-21 19:24:17.625800 runway-2.6.7/runway/templates/sls-tsc/src/helloWorld.test.ts
+-rw-r--r--   0        0        0      713 2023-07-21 19:24:17.625800 runway-2.6.7/runway/templates/sls-tsc/src/helloWorld.ts
+-rw-r--r--   0        0        0      514 2023-07-21 19:24:17.625800 runway-2.6.7/runway/templates/sls-tsc/tsconfig.json
+-rw-r--r--   0        0        0     1178 2023-07-21 19:24:17.625800 runway-2.6.7/runway/templates/sls-tsc/webpack.config.js
+-rw-r--r--   0        0        0      444 2023-07-21 19:24:17.625800 runway-2.6.7/runway/templates/static-angular/runway.yml
+-rw-r--r--   0        0        0      246 2023-07-21 19:24:17.625800 runway-2.6.7/runway/templates/static-angular/sampleapp.web/.editorconfig
+-rw-r--r--   0        0        0     1027 2023-07-21 19:24:17.625800 runway-2.6.7/runway/templates/static-angular/sampleapp.web/README.md
+-rw-r--r--   0        0        0      631 2023-07-21 19:24:17.625800 runway-2.6.7/runway/templates/static-angular/sampleapp.web/_gitignore
+-rw-r--r--   0        0        0     3626 2023-07-21 19:24:17.625800 runway-2.6.7/runway/templates/static-angular/sampleapp.web/angular.json
+-rw-r--r--   0        0        0      430 2023-07-21 19:24:17.625800 runway-2.6.7/runway/templates/static-angular/sampleapp.web/browserslist
+-rw-r--r--   0        0        0      809 2023-07-21 19:24:17.625800 runway-2.6.7/runway/templates/static-angular/sampleapp.web/e2e/protractor.conf.js
+-rw-r--r--   0        0        0      643 2023-07-21 19:24:17.625800 runway-2.6.7/runway/templates/static-angular/sampleapp.web/e2e/src/app.e2e-spec.ts
+-rw-r--r--   0        0        0      262 2023-07-21 19:24:17.625800 runway-2.6.7/runway/templates/static-angular/sampleapp.web/e2e/src/app.po.ts
+-rw-r--r--   0        0        0      214 2023-07-21 19:24:17.625800 runway-2.6.7/runway/templates/static-angular/sampleapp.web/e2e/tsconfig.json
+-rw-r--r--   0        0        0     1022 2023-07-21 19:24:17.625800 runway-2.6.7/runway/templates/static-angular/sampleapp.web/karma.conf.js
+-rw-r--r--   0        0        0   595303 2023-07-21 19:24:17.629800 runway-2.6.7/runway/templates/static-angular/sampleapp.web/package-lock.json
+-rw-r--r--   0        0        0     1295 2023-07-21 19:24:17.629800 runway-2.6.7/runway/templates/static-angular/sampleapp.web/package.json
+-rw-r--r--   0        0        0      246 2023-07-21 19:24:17.629800 runway-2.6.7/runway/templates/static-angular/sampleapp.web/src/app/app-routing.module.ts
+-rw-r--r--   0        0        0        0 2023-07-21 19:24:17.629800 runway-2.6.7/runway/templates/static-angular/sampleapp.web/src/app/app.component.css
+-rw-r--r--   0        0        0    25523 2023-07-21 19:24:17.629800 runway-2.6.7/runway/templates/static-angular/sampleapp.web/src/app/app.component.html
+-rw-r--r--   0        0        0     1110 2023-07-21 19:24:17.629800 runway-2.6.7/runway/templates/static-angular/sampleapp.web/src/app/app.component.spec.ts
+-rw-r--r--   0        0        0      214 2023-07-21 19:24:17.629800 runway-2.6.7/runway/templates/static-angular/sampleapp.web/src/app/app.component.ts
+-rw-r--r--   0        0        0      393 2023-07-21 19:24:17.629800 runway-2.6.7/runway/templates/static-angular/sampleapp.web/src/app/app.module.ts
+-rw-r--r--   0        0        0        0 2023-07-21 19:24:17.629800 runway-2.6.7/runway/templates/static-angular/sampleapp.web/src/assets/.gitkeep
+-rw-r--r--   0        0        0       51 2023-07-21 19:24:17.629800 runway-2.6.7/runway/templates/static-angular/sampleapp.web/src/environments/environment.prod.ts
+-rw-r--r--   0        0        0      662 2023-07-21 19:24:17.629800 runway-2.6.7/runway/templates/static-angular/sampleapp.web/src/environments/environment.ts
+-rw-r--r--   0        0        0      948 2023-07-21 19:24:17.629800 runway-2.6.7/runway/templates/static-angular/sampleapp.web/src/favicon.ico
+-rw-r--r--   0        0        0      295 2023-07-21 19:24:17.629800 runway-2.6.7/runway/templates/static-angular/sampleapp.web/src/index.html
+-rw-r--r--   0        0        0      372 2023-07-21 19:24:17.629800 runway-2.6.7/runway/templates/static-angular/sampleapp.web/src/main.ts
+-rw-r--r--   0        0        0     2838 2023-07-21 19:24:17.629800 runway-2.6.7/runway/templates/static-angular/sampleapp.web/src/polyfills.ts
+-rw-r--r--   0        0        0       80 2023-07-21 19:24:17.629800 runway-2.6.7/runway/templates/static-angular/sampleapp.web/src/styles.css
+-rw-r--r--   0        0        0      642 2023-07-21 19:24:17.629800 runway-2.6.7/runway/templates/static-angular/sampleapp.web/src/test.ts
+-rw-r--r--   0        0        0      270 2023-07-21 19:24:17.629800 runway-2.6.7/runway/templates/static-angular/sampleapp.web/tsconfig.app.json
+-rw-r--r--   0        0        0      543 2023-07-21 19:24:17.629800 runway-2.6.7/runway/templates/static-angular/sampleapp.web/tsconfig.json
+-rw-r--r--   0        0        0      270 2023-07-21 19:24:17.629800 runway-2.6.7/runway/templates/static-angular/sampleapp.web/tsconfig.spec.json
+-rw-r--r--   0        0        0     1954 2023-07-21 19:24:17.629800 runway-2.6.7/runway/templates/static-angular/sampleapp.web/tslint.json
+-rw-r--r--   0        0        0      435 2023-07-21 19:24:17.629800 runway-2.6.7/runway/templates/static-react/runway.yml
+-rw-r--r--   0        0        0      310 2023-07-21 19:24:17.629800 runway-2.6.7/runway/templates/static-react/sampleapp.web/.gitignore
+-rw-r--r--   0        0        0     2889 2023-07-21 19:24:17.629800 runway-2.6.7/runway/templates/static-react/sampleapp.web/README.md
+-rw-r--r--   0        0        0      746 2023-07-21 19:24:17.629800 runway-2.6.7/runway/templates/static-react/sampleapp.web/package.json
+-rw-r--r--   0        0        0     3870 2023-07-21 19:24:17.629800 runway-2.6.7/runway/templates/static-react/sampleapp.web/public/favicon.ico
+-rw-r--r--   0        0        0     1721 2023-07-21 19:24:17.629800 runway-2.6.7/runway/templates/static-react/sampleapp.web/public/index.html
+-rw-r--r--   0        0        0     5347 2023-07-21 19:24:17.629800 runway-2.6.7/runway/templates/static-react/sampleapp.web/public/logo192.png
+-rw-r--r--   0        0        0     9664 2023-07-21 19:24:17.629800 runway-2.6.7/runway/templates/static-react/sampleapp.web/public/logo512.png
+-rw-r--r--   0        0        0      492 2023-07-21 19:24:17.629800 runway-2.6.7/runway/templates/static-react/sampleapp.web/public/manifest.json
+-rw-r--r--   0        0        0       67 2023-07-21 19:24:17.629800 runway-2.6.7/runway/templates/static-react/sampleapp.web/public/robots.txt
+-rw-r--r--   0        0        0      564 2023-07-21 19:24:17.629800 runway-2.6.7/runway/templates/static-react/sampleapp.web/src/App.css
+-rw-r--r--   0        0        0      555 2023-07-21 19:24:17.629800 runway-2.6.7/runway/templates/static-react/sampleapp.web/src/App.js
+-rw-r--r--   0        0        0      280 2023-07-21 19:24:17.629800 runway-2.6.7/runway/templates/static-react/sampleapp.web/src/App.test.js
+-rw-r--r--   0        0        0      366 2023-07-21 19:24:17.629800 runway-2.6.7/runway/templates/static-react/sampleapp.web/src/index.css
+-rw-r--r--   0        0        0      452 2023-07-21 19:24:17.629800 runway-2.6.7/runway/templates/static-react/sampleapp.web/src/index.js
+-rw-r--r--   0        0        0     2671 2023-07-21 19:24:17.629800 runway-2.6.7/runway/templates/static-react/sampleapp.web/src/logo.svg
+-rw-r--r--   0        0        0     5003 2023-07-21 19:24:17.629800 runway-2.6.7/runway/templates/static-react/sampleapp.web/src/serviceWorker.js
+-rw-r--r--   0        0        0      255 2023-07-21 19:24:17.629800 runway-2.6.7/runway/templates/static-react/sampleapp.web/src/setupTests.js
+-rw-r--r--   0        0        0       82 2023-07-21 19:24:17.629800 runway-2.6.7/runway/templates/terraform/backend-us-east-1.tfvars
+-rw-r--r--   0        0        0       21 2023-07-21 19:24:17.629800 runway-2.6.7/runway/templates/terraform/dev-us-east-1.tfvars
+-rw-r--r--   0        0        0      312 2023-07-21 19:24:17.629800 runway-2.6.7/runway/templates/terraform/main.tf
+-rw-r--r--   0        0        0       46 2023-07-21 19:24:17.629800 runway-2.6.7/runway/tests/__init__.py
+-rw-r--r--   0        0        0      111 2023-07-21 19:24:17.629800 runway-2.6.7/runway/tests/handlers/__init__.py
+-rw-r--r--   0        0        0      757 2023-07-21 19:24:17.629800 runway-2.6.7/runway/tests/handlers/base.py
+-rw-r--r--   0        0        0     1901 2023-07-21 19:24:17.629800 runway-2.6.7/runway/tests/handlers/cfn_lint.py
+-rw-r--r--   0        0        0     1608 2023-07-21 19:24:17.629800 runway-2.6.7/runway/tests/handlers/script.py
+-rw-r--r--   0        0        0     2025 2023-07-21 19:24:17.629800 runway-2.6.7/runway/tests/handlers/yaml_lint.py
+-rw-r--r--   0        0        0     1112 2023-07-21 19:24:17.629800 runway-2.6.7/runway/tests/registry.py
+-rw-r--r--   0        0        0      628 2023-07-21 19:24:17.629800 runway-2.6.7/runway/type_defs.py
+-rw-r--r--   0        0        0    27539 2023-07-21 19:24:17.629800 runway-2.6.7/runway/utils/__init__.py
+-rw-r--r--   0        0        0     4278 2023-07-21 19:24:17.629800 runway-2.6.7/runway/utils/_file_hash.py
+-rw-r--r--   0        0        0      817 2023-07-21 19:24:17.629800 runway-2.6.7/runway/utils/_version.py
+-rw-r--r--   0        0        0    29956 2023-07-21 19:24:17.629800 runway-2.6.7/runway/variables.py
+-rw-r--r--   0        0        0     6144 1970-01-01 00:00:00.000000 runway-2.6.7/PKG-INFO
```

### Comparing `runway-2.6.6/LICENSE` & `runway-2.6.7/LICENSE`

 * *Files identical despite different names*

### Comparing `runway-2.6.6/README.md` & `runway-2.6.7/README.md`

 * *Files identical despite different names*

### Comparing `runway-2.6.6/pyproject.toml` & `runway-2.6.7/pyproject.toml`

 * *Files 1% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 [tool.poetry]
 name = "runway"
-version = "2.6.6"  # do not change
+version = "2.6.7"  # do not change
 description = "Simplify infrastructure/app testing/deployment"
 license = "Apache-2.0"
 authors = [
   "Onica Group LLC <opensource@onica.com>",
 ]
 maintainers = [
   "Kyle Finley <kyle@finley.sh>",
@@ -25,15 +25,15 @@
   "Programming Language :: Python :: 3.10",
 ]
 packages = [
   { include = "runway" },
 ]
 
 [tool.poetry.dependencies]
-python = ">=3.8, <3.12"
+python = ">=3.8, <4"
 
 # dependencies needed for building docs are included here.
 # they are marked as "optional" and are installed as the extra "docs".
 # this is a workaround for ReadTheDocs to work with poetry until fill support
 # is added or poetry dependency groups are added.
 
 "backports.cached_property" = { version = "*", python = "<3.8" }
```

### Comparing `runway-2.6.6/runway/__init__.py` & `runway-2.6.7/runway/__init__.py`

 * *Files identical despite different names*

### Comparing `runway-2.6.6/runway/_cli/commands/__init__.py` & `runway-2.6.7/runway/_cli/commands/__init__.py`

 * *Files identical despite different names*

### Comparing `runway-2.6.6/runway/_cli/commands/_deploy.py` & `runway-2.6.7/runway/_cli/commands/_deploy.py`

 * *Files identical despite different names*

### Comparing `runway-2.6.6/runway/_cli/commands/_destroy.py` & `runway-2.6.7/runway/_cli/commands/_destroy.py`

 * *Files identical despite different names*

### Comparing `runway-2.6.6/runway/_cli/commands/_dismantle.py` & `runway-2.6.7/runway/_cli/commands/_dismantle.py`

 * *Files identical despite different names*

### Comparing `runway-2.6.6/runway/_cli/commands/_docs.py` & `runway-2.6.7/runway/_cli/commands/_docs.py`

 * *Files identical despite different names*

### Comparing `runway-2.6.6/runway/_cli/commands/_envvars.py` & `runway-2.6.7/runway/_cli/commands/_envvars.py`

 * *Files identical despite different names*

### Comparing `runway-2.6.6/runway/_cli/commands/_gen_sample/__init__.py` & `runway-2.6.7/runway/_cli/commands/_gen_sample/__init__.py`

 * *Files identical despite different names*

### Comparing `runway-2.6.6/runway/_cli/commands/_gen_sample/_cdk_csharp.py` & `runway-2.6.7/runway/_cli/commands/_gen_sample/_cdk_csharp.py`

 * *Files identical despite different names*

### Comparing `runway-2.6.6/runway/_cli/commands/_gen_sample/_cdk_py.py` & `runway-2.6.7/runway/_cli/commands/_gen_sample/_cdk_py.py`

 * *Files identical despite different names*

### Comparing `runway-2.6.6/runway/_cli/commands/_gen_sample/_cdk_tsc.py` & `runway-2.6.7/runway/_cli/commands/_gen_sample/_cdk_tsc.py`

 * *Files identical despite different names*

### Comparing `runway-2.6.6/runway/_cli/commands/_gen_sample/_cfn.py` & `runway-2.6.7/runway/_cli/commands/_gen_sample/_cfn.py`

 * *Files identical despite different names*

### Comparing `runway-2.6.6/runway/_cli/commands/_gen_sample/_cfngin.py` & `runway-2.6.7/runway/_cli/commands/_gen_sample/_cfngin.py`

 * *Files identical despite different names*

### Comparing `runway-2.6.6/runway/_cli/commands/_gen_sample/_k8s_cfn_repo.py` & `runway-2.6.7/runway/_cli/commands/_gen_sample/_k8s_cfn_repo.py`

 * *Files identical despite different names*

### Comparing `runway-2.6.6/runway/_cli/commands/_gen_sample/_k8s_flux_repo.py` & `runway-2.6.7/runway/_cli/commands/_gen_sample/_k8s_flux_repo.py`

 * *Files identical despite different names*

### Comparing `runway-2.6.6/runway/_cli/commands/_gen_sample/_k8s_tf_repo.py` & `runway-2.6.7/runway/_cli/commands/_gen_sample/_k8s_tf_repo.py`

 * *Files identical despite different names*

### Comparing `runway-2.6.6/runway/_cli/commands/_gen_sample/_sls_py.py` & `runway-2.6.7/runway/_cli/commands/_gen_sample/_sls_py.py`

 * *Files identical despite different names*

### Comparing `runway-2.6.6/runway/_cli/commands/_gen_sample/_sls_tsc.py` & `runway-2.6.7/runway/_cli/commands/_gen_sample/_sls_tsc.py`

 * *Files identical despite different names*

### Comparing `runway-2.6.6/runway/_cli/commands/_gen_sample/_static_angular.py` & `runway-2.6.7/runway/_cli/commands/_gen_sample/_static_angular.py`

 * *Files identical despite different names*

### Comparing `runway-2.6.6/runway/_cli/commands/_gen_sample/_static_react.py` & `runway-2.6.7/runway/_cli/commands/_gen_sample/_static_react.py`

 * *Files identical despite different names*

### Comparing `runway-2.6.6/runway/_cli/commands/_gen_sample/_tf.py` & `runway-2.6.7/runway/_cli/commands/_gen_sample/_tf.py`

 * *Files identical despite different names*

### Comparing `runway-2.6.6/runway/_cli/commands/_gen_sample/utils.py` & `runway-2.6.7/runway/_cli/commands/_gen_sample/utils.py`

 * *Files identical despite different names*

### Comparing `runway-2.6.6/runway/_cli/commands/_init.py` & `runway-2.6.7/runway/_cli/commands/_init.py`

 * *Files identical despite different names*

### Comparing `runway-2.6.6/runway/_cli/commands/_kbenv/__init__.py` & `runway-2.6.7/runway/_cli/commands/_kbenv/__init__.py`

 * *Files identical despite different names*

### Comparing `runway-2.6.6/runway/_cli/commands/_kbenv/_install.py` & `runway-2.6.7/runway/_cli/commands/_kbenv/_install.py`

 * *Files identical despite different names*

### Comparing `runway-2.6.6/runway/_cli/commands/_kbenv/_list.py` & `runway-2.6.7/runway/_cli/commands/_kbenv/_list.py`

 * *Files identical despite different names*

### Comparing `runway-2.6.6/runway/_cli/commands/_kbenv/_run.py` & `runway-2.6.7/runway/_cli/commands/_kbenv/_run.py`

 * *Files identical despite different names*

### Comparing `runway-2.6.6/runway/_cli/commands/_kbenv/_uninstall.py` & `runway-2.6.7/runway/_cli/commands/_kbenv/_uninstall.py`

 * *Files identical despite different names*

### Comparing `runway-2.6.6/runway/_cli/commands/_new.py` & `runway-2.6.7/runway/_cli/commands/_new.py`

 * *Files identical despite different names*

### Comparing `runway-2.6.6/runway/_cli/commands/_plan.py` & `runway-2.6.7/runway/_cli/commands/_plan.py`

 * *Files identical despite different names*

### Comparing `runway-2.6.6/runway/_cli/commands/_preflight.py` & `runway-2.6.7/runway/_cli/commands/_preflight.py`

 * *Files identical despite different names*

### Comparing `runway-2.6.6/runway/_cli/commands/_run_python.py` & `runway-2.6.7/runway/_cli/commands/_run_python.py`

 * *Files identical despite different names*

### Comparing `runway-2.6.6/runway/_cli/commands/_schema/_cfngin.py` & `runway-2.6.7/runway/_cli/commands/_schema/_cfngin.py`

 * *Files identical despite different names*

### Comparing `runway-2.6.6/runway/_cli/commands/_schema/_runway.py` & `runway-2.6.7/runway/_cli/commands/_schema/_runway.py`

 * *Files identical despite different names*

### Comparing `runway-2.6.6/runway/_cli/commands/_takeoff.py` & `runway-2.6.7/runway/_cli/commands/_takeoff.py`

 * *Files identical despite different names*

### Comparing `runway-2.6.6/runway/_cli/commands/_taxi.py` & `runway-2.6.7/runway/_cli/commands/_taxi.py`

 * *Files identical despite different names*

### Comparing `runway-2.6.6/runway/_cli/commands/_test.py` & `runway-2.6.7/runway/_cli/commands/_test.py`

 * *Files identical despite different names*

### Comparing `runway-2.6.6/runway/_cli/commands/_tfenv/__init__.py` & `runway-2.6.7/runway/_cli/commands/_tfenv/__init__.py`

 * *Files identical despite different names*

### Comparing `runway-2.6.6/runway/_cli/commands/_tfenv/_install.py` & `runway-2.6.7/runway/_cli/commands/_tfenv/_install.py`

 * *Files identical despite different names*

### Comparing `runway-2.6.6/runway/_cli/commands/_tfenv/_list.py` & `runway-2.6.7/runway/_cli/commands/_tfenv/_list.py`

 * *Files identical despite different names*

### Comparing `runway-2.6.6/runway/_cli/commands/_tfenv/_run.py` & `runway-2.6.7/runway/_cli/commands/_tfenv/_run.py`

 * *Files identical despite different names*

### Comparing `runway-2.6.6/runway/_cli/commands/_tfenv/_uninstall.py` & `runway-2.6.7/runway/_cli/commands/_tfenv/_uninstall.py`

 * *Files identical despite different names*

### Comparing `runway-2.6.6/runway/_cli/commands/_whichenv.py` & `runway-2.6.7/runway/_cli/commands/_whichenv.py`

 * *Files identical despite different names*

### Comparing `runway-2.6.6/runway/_cli/logs.py` & `runway-2.6.7/runway/_cli/logs.py`

 * *Files identical despite different names*

### Comparing `runway-2.6.6/runway/_cli/main.py` & `runway-2.6.7/runway/_cli/main.py`

 * *Files identical despite different names*

### Comparing `runway-2.6.6/runway/_cli/options.py` & `runway-2.6.7/runway/_cli/options.py`

 * *Files identical despite different names*

### Comparing `runway-2.6.6/runway/_cli/utils.py` & `runway-2.6.7/runway/_cli/utils.py`

 * *Files identical despite different names*

### Comparing `runway-2.6.6/runway/_logging.py` & `runway-2.6.7/runway/_logging.py`

 * *Files identical despite different names*

### Comparing `runway-2.6.6/runway/aws_sso_botocore/__init__.py` & `runway-2.6.7/runway/aws_sso_botocore/__init__.py`

 * *Files identical despite different names*

### Comparing `runway-2.6.6/runway/aws_sso_botocore/credentials.py` & `runway-2.6.7/runway/aws_sso_botocore/credentials.py`

 * *Files identical despite different names*

### Comparing `runway-2.6.6/runway/aws_sso_botocore/exceptions.py` & `runway-2.6.7/runway/aws_sso_botocore/exceptions.py`

 * *Files identical despite different names*

### Comparing `runway-2.6.6/runway/aws_sso_botocore/session.py` & `runway-2.6.7/runway/aws_sso_botocore/session.py`

 * *Files identical despite different names*

### Comparing `runway-2.6.6/runway/aws_sso_botocore/util.py` & `runway-2.6.7/runway/aws_sso_botocore/util.py`

 * *Files identical despite different names*

### Comparing `runway-2.6.6/runway/blueprints/k8s/k8s_iam.py` & `runway-2.6.7/runway/blueprints/k8s/k8s_iam.py`

 * *Files identical despite different names*

### Comparing `runway-2.6.6/runway/blueprints/k8s/k8s_master.py` & `runway-2.6.7/runway/blueprints/k8s/k8s_master.py`

 * *Files identical despite different names*

### Comparing `runway-2.6.6/runway/blueprints/k8s/k8s_workers.py` & `runway-2.6.7/runway/blueprints/k8s/k8s_workers.py`

 * *Files identical despite different names*

### Comparing `runway-2.6.6/runway/blueprints/staticsite/auth_at_edge.py` & `runway-2.6.7/runway/blueprints/staticsite/auth_at_edge.py`

 * *Files identical despite different names*

### Comparing `runway-2.6.6/runway/blueprints/staticsite/dependencies.py` & `runway-2.6.7/runway/blueprints/staticsite/dependencies.py`

 * *Files identical despite different names*

### Comparing `runway-2.6.6/runway/blueprints/staticsite/staticsite.py` & `runway-2.6.7/runway/blueprints/staticsite/staticsite.py`

 * *Files identical despite different names*

### Comparing `runway-2.6.6/runway/blueprints/staticsite/templates/cf_directory_index_rewrite.template.js` & `runway-2.6.7/runway/blueprints/staticsite/templates/cf_directory_index_rewrite.template.js`

 * *Files identical despite different names*

### Comparing `runway-2.6.6/runway/blueprints/tf_state.py` & `runway-2.6.7/runway/blueprints/tf_state.py`

 * *Files identical despite different names*

### Comparing `runway-2.6.6/runway/cfngin/LICENSE` & `runway-2.6.7/runway/cfngin/LICENSE`

 * *Files identical despite different names*

### Comparing `runway-2.6.6/runway/cfngin/actions/base.py` & `runway-2.6.7/runway/cfngin/actions/base.py`

 * *Files identical despite different names*

### Comparing `runway-2.6.6/runway/cfngin/actions/deploy.py` & `runway-2.6.7/runway/cfngin/actions/deploy.py`

 * *Files identical despite different names*

### Comparing `runway-2.6.6/runway/cfngin/actions/destroy.py` & `runway-2.6.7/runway/cfngin/actions/destroy.py`

 * *Files identical despite different names*

### Comparing `runway-2.6.6/runway/cfngin/actions/diff.py` & `runway-2.6.7/runway/cfngin/actions/diff.py`

 * *Files identical despite different names*

### Comparing `runway-2.6.6/runway/cfngin/actions/graph.py` & `runway-2.6.7/runway/cfngin/actions/graph.py`

 * *Files identical despite different names*

### Comparing `runway-2.6.6/runway/cfngin/actions/info.py` & `runway-2.6.7/runway/cfngin/actions/info.py`

 * *Files identical despite different names*

### Comparing `runway-2.6.6/runway/cfngin/actions/init.py` & `runway-2.6.7/runway/cfngin/actions/init.py`

 * *Files identical despite different names*

### Comparing `runway-2.6.6/runway/cfngin/awscli_yamlhelper.py` & `runway-2.6.7/runway/cfngin/awscli_yamlhelper.py`

 * *Files identical despite different names*

### Comparing `runway-2.6.6/runway/cfngin/blueprints/base.py` & `runway-2.6.7/runway/cfngin/blueprints/base.py`

 * *Files identical despite different names*

### Comparing `runway-2.6.6/runway/cfngin/blueprints/cfngin_bucket.py` & `runway-2.6.7/runway/cfngin/blueprints/cfngin_bucket.py`

 * *Files identical despite different names*

### Comparing `runway-2.6.6/runway/cfngin/blueprints/raw.py` & `runway-2.6.7/runway/cfngin/blueprints/raw.py`

 * *Files identical despite different names*

### Comparing `runway-2.6.6/runway/cfngin/blueprints/testutil.py` & `runway-2.6.7/runway/cfngin/blueprints/testutil.py`

 * *Files identical despite different names*

### Comparing `runway-2.6.6/runway/cfngin/blueprints/type_defs.py` & `runway-2.6.7/runway/cfngin/blueprints/type_defs.py`

 * *Files identical despite different names*

### Comparing `runway-2.6.6/runway/cfngin/blueprints/variables/types.py` & `runway-2.6.7/runway/cfngin/blueprints/variables/types.py`

 * *Files identical despite different names*

### Comparing `runway-2.6.6/runway/cfngin/cfngin.py` & `runway-2.6.7/runway/cfngin/cfngin.py`

 * *Files identical despite different names*

### Comparing `runway-2.6.6/runway/cfngin/dag/__init__.py` & `runway-2.6.7/runway/cfngin/dag/__init__.py`

 * *Files identical despite different names*

### Comparing `runway-2.6.6/runway/cfngin/environment.py` & `runway-2.6.7/runway/cfngin/environment.py`

 * *Files identical despite different names*

### Comparing `runway-2.6.6/runway/cfngin/exceptions.py` & `runway-2.6.7/runway/cfngin/exceptions.py`

 * *Files identical despite different names*

### Comparing `runway-2.6.6/runway/cfngin/hooks/acm.py` & `runway-2.6.7/runway/cfngin/hooks/acm.py`

 * *Files identical despite different names*

### Comparing `runway-2.6.6/runway/cfngin/hooks/aws_lambda.py` & `runway-2.6.7/runway/cfngin/hooks/aws_lambda.py`

 * *Files identical despite different names*

### Comparing `runway-2.6.6/runway/cfngin/hooks/awslambda/_python_hooks.py` & `runway-2.6.7/runway/cfngin/hooks/awslambda/_python_hooks.py`

 * *Files identical despite different names*

### Comparing `runway-2.6.6/runway/cfngin/hooks/awslambda/base_classes.py` & `runway-2.6.7/runway/cfngin/hooks/awslambda/base_classes.py`

 * *Files identical despite different names*

### Comparing `runway-2.6.6/runway/cfngin/hooks/awslambda/deployment_package.py` & `runway-2.6.7/runway/cfngin/hooks/awslambda/deployment_package.py`

 * *Files identical despite different names*

### Comparing `runway-2.6.6/runway/cfngin/hooks/awslambda/docker.py` & `runway-2.6.7/runway/cfngin/hooks/awslambda/docker.py`

 * *Files identical despite different names*

### Comparing `runway-2.6.6/runway/cfngin/hooks/awslambda/exceptions.py` & `runway-2.6.7/runway/cfngin/hooks/awslambda/exceptions.py`

 * *Files identical despite different names*

### Comparing `runway-2.6.6/runway/cfngin/hooks/awslambda/models/args.py` & `runway-2.6.7/runway/cfngin/hooks/awslambda/models/args.py`

 * *Files identical despite different names*

### Comparing `runway-2.6.6/runway/cfngin/hooks/awslambda/models/responses.py` & `runway-2.6.7/runway/cfngin/hooks/awslambda/models/responses.py`

 * *Files identical despite different names*

### Comparing `runway-2.6.6/runway/cfngin/hooks/awslambda/python_requirements/_deployment_package.py` & `runway-2.6.7/runway/cfngin/hooks/awslambda/python_requirements/_deployment_package.py`

 * *Files identical despite different names*

### Comparing `runway-2.6.6/runway/cfngin/hooks/awslambda/python_requirements/_docker.py` & `runway-2.6.7/runway/cfngin/hooks/awslambda/python_requirements/_docker.py`

 * *Files identical despite different names*

### Comparing `runway-2.6.6/runway/cfngin/hooks/awslambda/python_requirements/_project.py` & `runway-2.6.7/runway/cfngin/hooks/awslambda/python_requirements/_project.py`

 * *Files identical despite different names*

### Comparing `runway-2.6.6/runway/cfngin/hooks/awslambda/source_code.py` & `runway-2.6.7/runway/cfngin/hooks/awslambda/source_code.py`

 * *Files identical despite different names*

### Comparing `runway-2.6.6/runway/cfngin/hooks/base.py` & `runway-2.6.7/runway/cfngin/hooks/base.py`

 * *Files identical despite different names*

### Comparing `runway-2.6.6/runway/cfngin/hooks/cleanup_s3.py` & `runway-2.6.7/runway/cfngin/hooks/cleanup_s3.py`

 * *Files identical despite different names*

### Comparing `runway-2.6.6/runway/cfngin/hooks/cleanup_ssm.py` & `runway-2.6.7/runway/cfngin/hooks/cleanup_ssm.py`

 * *Files identical despite different names*

### Comparing `runway-2.6.6/runway/cfngin/hooks/command.py` & `runway-2.6.7/runway/cfngin/hooks/command.py`

 * *Files identical despite different names*

### Comparing `runway-2.6.6/runway/cfngin/hooks/docker/_login.py` & `runway-2.6.7/runway/cfngin/hooks/docker/_login.py`

 * *Files identical despite different names*

### Comparing `runway-2.6.6/runway/cfngin/hooks/docker/data_models.py` & `runway-2.6.7/runway/cfngin/hooks/docker/data_models.py`

 * *Files identical despite different names*

### Comparing `runway-2.6.6/runway/cfngin/hooks/docker/hook_data.py` & `runway-2.6.7/runway/cfngin/hooks/docker/hook_data.py`

 * *Files identical despite different names*

### Comparing `runway-2.6.6/runway/cfngin/hooks/docker/image/_build.py` & `runway-2.6.7/runway/cfngin/hooks/docker/image/_build.py`

 * *Files identical despite different names*

### Comparing `runway-2.6.6/runway/cfngin/hooks/docker/image/_push.py` & `runway-2.6.7/runway/cfngin/hooks/docker/image/_push.py`

 * *Files identical despite different names*

### Comparing `runway-2.6.6/runway/cfngin/hooks/docker/image/_remove.py` & `runway-2.6.7/runway/cfngin/hooks/docker/image/_remove.py`

 * *Files identical despite different names*

### Comparing `runway-2.6.6/runway/cfngin/hooks/ecr/_purge_repository.py` & `runway-2.6.7/runway/cfngin/hooks/ecr/_purge_repository.py`

 * *Files identical despite different names*

### Comparing `runway-2.6.6/runway/cfngin/hooks/ecs.py` & `runway-2.6.7/runway/cfngin/hooks/ecs.py`

 * *Files identical despite different names*

### Comparing `runway-2.6.6/runway/cfngin/hooks/iam.py` & `runway-2.6.7/runway/cfngin/hooks/iam.py`

 * *Files identical despite different names*

### Comparing `runway-2.6.6/runway/cfngin/hooks/keypair.py` & `runway-2.6.7/runway/cfngin/hooks/keypair.py`

 * *Files identical despite different names*

### Comparing `runway-2.6.6/runway/cfngin/hooks/protocols.py` & `runway-2.6.7/runway/cfngin/hooks/protocols.py`

 * *Files identical despite different names*

### Comparing `runway-2.6.6/runway/cfngin/hooks/route53.py` & `runway-2.6.7/runway/cfngin/hooks/route53.py`

 * *Files identical despite different names*

### Comparing `runway-2.6.6/runway/cfngin/hooks/ssm/parameter.py` & `runway-2.6.7/runway/cfngin/hooks/ssm/parameter.py`

 * *Files identical despite different names*

### Comparing `runway-2.6.6/runway/cfngin/hooks/staticsite/auth_at_edge/callback_url_retriever.py` & `runway-2.6.7/runway/cfngin/hooks/staticsite/auth_at_edge/callback_url_retriever.py`

 * *Files identical despite different names*

### Comparing `runway-2.6.6/runway/cfngin/hooks/staticsite/auth_at_edge/client_updater.py` & `runway-2.6.7/runway/cfngin/hooks/staticsite/auth_at_edge/client_updater.py`

 * *Files identical despite different names*

### Comparing `runway-2.6.6/runway/cfngin/hooks/staticsite/auth_at_edge/domain_updater.py` & `runway-2.6.7/runway/cfngin/hooks/staticsite/auth_at_edge/domain_updater.py`

 * *Files identical despite different names*

### Comparing `runway-2.6.6/runway/cfngin/hooks/staticsite/auth_at_edge/lambda_config.py` & `runway-2.6.7/runway/cfngin/hooks/staticsite/auth_at_edge/lambda_config.py`

 * *Files identical despite different names*

### Comparing `runway-2.6.6/runway/cfngin/hooks/staticsite/auth_at_edge/templates/check_auth/__init__.py` & `runway-2.6.7/runway/cfngin/hooks/staticsite/auth_at_edge/templates/check_auth/__init__.py`

 * *Files identical despite different names*

### Comparing `runway-2.6.6/runway/cfngin/hooks/staticsite/auth_at_edge/templates/http_headers/__init__.py` & `runway-2.6.7/runway/cfngin/hooks/staticsite/auth_at_edge/templates/http_headers/__init__.py`

 * *Files identical despite different names*

### Comparing `runway-2.6.6/runway/cfngin/hooks/staticsite/auth_at_edge/templates/parse_auth/__init__.py` & `runway-2.6.7/runway/cfngin/hooks/staticsite/auth_at_edge/templates/parse_auth/__init__.py`

 * *Files identical despite different names*

### Comparing `runway-2.6.6/runway/cfngin/hooks/staticsite/auth_at_edge/templates/refresh_auth/__init__.py` & `runway-2.6.7/runway/cfngin/hooks/staticsite/auth_at_edge/templates/refresh_auth/__init__.py`

 * *Files identical despite different names*

### Comparing `runway-2.6.6/runway/cfngin/hooks/staticsite/auth_at_edge/templates/shared.py` & `runway-2.6.7/runway/cfngin/hooks/staticsite/auth_at_edge/templates/shared.py`

 * *Files identical despite different names*

### Comparing `runway-2.6.6/runway/cfngin/hooks/staticsite/auth_at_edge/templates/shared_jose.py` & `runway-2.6.7/runway/cfngin/hooks/staticsite/auth_at_edge/templates/shared_jose.py`

 * *Files identical despite different names*

### Comparing `runway-2.6.6/runway/cfngin/hooks/staticsite/auth_at_edge/templates/sign_out/__init__.py` & `runway-2.6.7/runway/cfngin/hooks/staticsite/auth_at_edge/templates/sign_out/__init__.py`

 * *Files identical despite different names*

### Comparing `runway-2.6.6/runway/cfngin/hooks/staticsite/auth_at_edge/user_pool_id_retriever.py` & `runway-2.6.7/runway/cfngin/hooks/staticsite/auth_at_edge/user_pool_id_retriever.py`

 * *Files identical despite different names*

### Comparing `runway-2.6.6/runway/cfngin/hooks/staticsite/build_staticsite.py` & `runway-2.6.7/runway/cfngin/hooks/staticsite/build_staticsite.py`

 * *Files identical despite different names*

### Comparing `runway-2.6.6/runway/cfngin/hooks/staticsite/cleanup.py` & `runway-2.6.7/runway/cfngin/hooks/staticsite/cleanup.py`

 * *Files identical despite different names*

### Comparing `runway-2.6.6/runway/cfngin/hooks/staticsite/upload_staticsite.py` & `runway-2.6.7/runway/cfngin/hooks/staticsite/upload_staticsite.py`

 * *Files identical despite different names*

### Comparing `runway-2.6.6/runway/cfngin/hooks/staticsite/utils.py` & `runway-2.6.7/runway/cfngin/hooks/staticsite/utils.py`

 * *Files identical despite different names*

### Comparing `runway-2.6.6/runway/cfngin/hooks/utils.py` & `runway-2.6.7/runway/cfngin/hooks/utils.py`

 * *Files identical despite different names*

### Comparing `runway-2.6.6/runway/cfngin/logger/__init__.py` & `runway-2.6.7/runway/cfngin/logger/__init__.py`

 * *Files identical despite different names*

### Comparing `runway-2.6.6/runway/cfngin/lookups/handlers/ami.py` & `runway-2.6.7/runway/cfngin/lookups/handlers/ami.py`

 * *Files identical despite different names*

### Comparing `runway-2.6.6/runway/cfngin/lookups/handlers/awslambda.py` & `runway-2.6.7/runway/cfngin/lookups/handlers/awslambda.py`

 * *Files identical despite different names*

### Comparing `runway-2.6.6/runway/cfngin/lookups/handlers/default.py` & `runway-2.6.7/runway/cfngin/lookups/handlers/default.py`

 * *Files identical despite different names*

### Comparing `runway-2.6.6/runway/cfngin/lookups/handlers/dynamodb.py` & `runway-2.6.7/runway/cfngin/lookups/handlers/dynamodb.py`

 * *Files identical despite different names*

### Comparing `runway-2.6.6/runway/cfngin/lookups/handlers/envvar.py` & `runway-2.6.7/runway/cfngin/lookups/handlers/envvar.py`

 * *Files identical despite different names*

### Comparing `runway-2.6.6/runway/cfngin/lookups/handlers/file.py` & `runway-2.6.7/runway/cfngin/lookups/handlers/file.py`

 * *Files identical despite different names*

### Comparing `runway-2.6.6/runway/cfngin/lookups/handlers/hook_data.py` & `runway-2.6.7/runway/cfngin/lookups/handlers/hook_data.py`

 * *Files identical despite different names*

### Comparing `runway-2.6.6/runway/cfngin/lookups/handlers/kms.py` & `runway-2.6.7/runway/cfngin/lookups/handlers/kms.py`

 * *Files identical despite different names*

### Comparing `runway-2.6.6/runway/cfngin/lookups/handlers/output.py` & `runway-2.6.7/runway/cfngin/lookups/handlers/output.py`

 * *Files identical despite different names*

### Comparing `runway-2.6.6/runway/cfngin/lookups/handlers/rxref.py` & `runway-2.6.7/runway/cfngin/lookups/handlers/rxref.py`

 * *Files identical despite different names*

### Comparing `runway-2.6.6/runway/cfngin/lookups/handlers/split.py` & `runway-2.6.7/runway/cfngin/lookups/handlers/split.py`

 * *Files identical despite different names*

### Comparing `runway-2.6.6/runway/cfngin/lookups/handlers/xref.py` & `runway-2.6.7/runway/cfngin/lookups/handlers/xref.py`

 * *Files identical despite different names*

### Comparing `runway-2.6.6/runway/cfngin/lookups/registry.py` & `runway-2.6.7/runway/cfngin/lookups/registry.py`

 * *Files identical despite different names*

### Comparing `runway-2.6.6/runway/cfngin/plan.py` & `runway-2.6.7/runway/cfngin/plan.py`

 * *Files identical despite different names*

### Comparing `runway-2.6.6/runway/cfngin/providers/aws/default.py` & `runway-2.6.7/runway/cfngin/providers/aws/default.py`

 * *Files identical despite different names*

### Comparing `runway-2.6.6/runway/cfngin/providers/base.py` & `runway-2.6.7/runway/cfngin/providers/base.py`

 * *Files identical despite different names*

### Comparing `runway-2.6.6/runway/cfngin/session_cache.py` & `runway-2.6.7/runway/cfngin/session_cache.py`

 * *Files identical despite different names*

### Comparing `runway-2.6.6/runway/cfngin/stack.py` & `runway-2.6.7/runway/cfngin/stack.py`

 * *Files identical despite different names*

### Comparing `runway-2.6.6/runway/cfngin/status.py` & `runway-2.6.7/runway/cfngin/status.py`

 * *Files identical despite different names*

### Comparing `runway-2.6.6/runway/cfngin/tokenize_userdata.py` & `runway-2.6.7/runway/cfngin/tokenize_userdata.py`

 * *Files identical despite different names*

### Comparing `runway-2.6.6/runway/cfngin/ui.py` & `runway-2.6.7/runway/cfngin/ui.py`

 * *Files identical despite different names*

### Comparing `runway-2.6.6/runway/cfngin/utils.py` & `runway-2.6.7/runway/cfngin/utils.py`

 * *Files identical despite different names*

### Comparing `runway-2.6.6/runway/compat.py` & `runway-2.6.7/runway/compat.py`

 * *Files identical despite different names*

### Comparing `runway-2.6.6/runway/config/__init__.py` & `runway-2.6.7/runway/config/__init__.py`

 * *Files identical despite different names*

### Comparing `runway-2.6.6/runway/config/components/runway/__init__.py` & `runway-2.6.7/runway/config/components/runway/__init__.py`

 * *Files identical despite different names*

### Comparing `runway-2.6.6/runway/config/components/runway/_deployment_def.py` & `runway-2.6.7/runway/config/components/runway/_deployment_def.py`

 * *Files identical despite different names*

### Comparing `runway-2.6.6/runway/config/components/runway/_module_def.py` & `runway-2.6.7/runway/config/components/runway/_module_def.py`

 * *Files identical despite different names*

### Comparing `runway-2.6.6/runway/config/components/runway/_test_def.py` & `runway-2.6.7/runway/config/components/runway/_test_def.py`

 * *Files identical despite different names*

### Comparing `runway-2.6.6/runway/config/components/runway/_variables_def.py` & `runway-2.6.7/runway/config/components/runway/_variables_def.py`

 * *Files identical despite different names*

### Comparing `runway-2.6.6/runway/config/components/runway/base.py` & `runway-2.6.7/runway/config/components/runway/base.py`

 * *Files identical despite different names*

### Comparing `runway-2.6.6/runway/config/models/cfngin/__init__.py` & `runway-2.6.7/runway/config/models/cfngin/__init__.py`

 * *Files identical despite different names*

### Comparing `runway-2.6.6/runway/config/models/cfngin/_package_sources.py` & `runway-2.6.7/runway/config/models/cfngin/_package_sources.py`

 * *Files identical despite different names*

### Comparing `runway-2.6.6/runway/config/models/runway/__init__.py` & `runway-2.6.7/runway/config/models/runway/__init__.py`

 * *Files identical despite different names*

### Comparing `runway-2.6.6/runway/config/models/runway/_builtin_tests.py` & `runway-2.6.7/runway/config/models/runway/_builtin_tests.py`

 * *Files identical despite different names*

### Comparing `runway-2.6.6/runway/config/models/runway/options/cdk.py` & `runway-2.6.7/runway/config/models/runway/options/cdk.py`

 * *Files identical despite different names*

### Comparing `runway-2.6.6/runway/config/models/runway/options/k8s.py` & `runway-2.6.7/runway/config/models/runway/options/k8s.py`

 * *Files identical despite different names*

### Comparing `runway-2.6.6/runway/config/models/runway/options/serverless.py` & `runway-2.6.7/runway/config/models/runway/options/serverless.py`

 * *Files identical despite different names*

### Comparing `runway-2.6.6/runway/config/models/runway/options/terraform.py` & `runway-2.6.7/runway/config/models/runway/options/terraform.py`

 * *Files identical despite different names*

### Comparing `runway-2.6.6/runway/config/models/utils.py` & `runway-2.6.7/runway/config/models/utils.py`

 * *Files identical despite different names*

### Comparing `runway-2.6.6/runway/context/_base.py` & `runway-2.6.7/runway/context/_base.py`

 * *Files identical despite different names*

### Comparing `runway-2.6.6/runway/context/_cfngin.py` & `runway-2.6.7/runway/context/_cfngin.py`

 * *Files identical despite different names*

### Comparing `runway-2.6.6/runway/context/_runway.py` & `runway-2.6.7/runway/context/_runway.py`

 * *Files identical despite different names*

### Comparing `runway-2.6.6/runway/context/sys_info.py` & `runway-2.6.7/runway/context/sys_info.py`

 * *Files identical despite different names*

### Comparing `runway-2.6.6/runway/core/__init__.py` & `runway-2.6.7/runway/core/__init__.py`

 * *Files identical despite different names*

### Comparing `runway-2.6.6/runway/core/components/_deploy_environment.py` & `runway-2.6.7/runway/core/components/_deploy_environment.py`

 * *Files identical despite different names*

### Comparing `runway-2.6.6/runway/core/components/_deployment.py` & `runway-2.6.7/runway/core/components/_deployment.py`

 * *Files identical despite different names*

### Comparing `runway-2.6.6/runway/core/components/_module.py` & `runway-2.6.7/runway/core/components/_module.py`

 * *Files identical despite different names*

### Comparing `runway-2.6.6/runway/core/components/_module_path.py` & `runway-2.6.7/runway/core/components/_module_path.py`

 * *Files identical despite different names*

### Comparing `runway-2.6.6/runway/core/components/_module_type.py` & `runway-2.6.7/runway/core/components/_module_type.py`

 * *Files identical despite different names*

### Comparing `runway-2.6.6/runway/core/providers/aws/_account.py` & `runway-2.6.7/runway/core/providers/aws/_account.py`

 * *Files identical despite different names*

### Comparing `runway-2.6.6/runway/core/providers/aws/_assume_role.py` & `runway-2.6.7/runway/core/providers/aws/_assume_role.py`

 * *Files identical despite different names*

### Comparing `runway-2.6.6/runway/core/providers/aws/_response.py` & `runway-2.6.7/runway/core/providers/aws/_response.py`

 * *Files identical despite different names*

### Comparing `runway-2.6.6/runway/core/providers/aws/s3/_bucket.py` & `runway-2.6.7/runway/core/providers/aws/s3/_bucket.py`

 * *Files identical despite different names*

### Comparing `runway-2.6.6/runway/core/providers/aws/s3/_helpers/action_architecture.py` & `runway-2.6.7/runway/core/providers/aws/s3/_helpers/action_architecture.py`

 * *Files identical despite different names*

### Comparing `runway-2.6.6/runway/core/providers/aws/s3/_helpers/comparator.py` & `runway-2.6.7/runway/core/providers/aws/s3/_helpers/comparator.py`

 * *Files identical despite different names*

### Comparing `runway-2.6.6/runway/core/providers/aws/s3/_helpers/file_generator.py` & `runway-2.6.7/runway/core/providers/aws/s3/_helpers/file_generator.py`

 * *Files identical despite different names*

### Comparing `runway-2.6.6/runway/core/providers/aws/s3/_helpers/file_info.py` & `runway-2.6.7/runway/core/providers/aws/s3/_helpers/file_info.py`

 * *Files identical despite different names*

### Comparing `runway-2.6.6/runway/core/providers/aws/s3/_helpers/file_info_builder.py` & `runway-2.6.7/runway/core/providers/aws/s3/_helpers/file_info_builder.py`

 * *Files identical despite different names*

### Comparing `runway-2.6.6/runway/core/providers/aws/s3/_helpers/filters.py` & `runway-2.6.7/runway/core/providers/aws/s3/_helpers/filters.py`

 * *Files identical despite different names*

### Comparing `runway-2.6.6/runway/core/providers/aws/s3/_helpers/format_path.py` & `runway-2.6.7/runway/core/providers/aws/s3/_helpers/format_path.py`

 * *Files identical despite different names*

### Comparing `runway-2.6.6/runway/core/providers/aws/s3/_helpers/parameters.py` & `runway-2.6.7/runway/core/providers/aws/s3/_helpers/parameters.py`

 * *Files identical despite different names*

### Comparing `runway-2.6.6/runway/core/providers/aws/s3/_helpers/results.py` & `runway-2.6.7/runway/core/providers/aws/s3/_helpers/results.py`

 * *Files identical despite different names*

### Comparing `runway-2.6.6/runway/core/providers/aws/s3/_helpers/s3handler.py` & `runway-2.6.7/runway/core/providers/aws/s3/_helpers/s3handler.py`

 * *Files identical despite different names*

### Comparing `runway-2.6.6/runway/core/providers/aws/s3/_helpers/sync_strategy/__init__.py` & `runway-2.6.7/runway/core/providers/aws/s3/_helpers/sync_strategy/__init__.py`

 * *Files identical despite different names*

### Comparing `runway-2.6.6/runway/core/providers/aws/s3/_helpers/sync_strategy/base.py` & `runway-2.6.7/runway/core/providers/aws/s3/_helpers/sync_strategy/base.py`

 * *Files identical despite different names*

### Comparing `runway-2.6.6/runway/core/providers/aws/s3/_helpers/sync_strategy/delete.py` & `runway-2.6.7/runway/core/providers/aws/s3/_helpers/sync_strategy/delete.py`

 * *Files identical despite different names*

### Comparing `runway-2.6.6/runway/core/providers/aws/s3/_helpers/sync_strategy/exact_timestamps.py` & `runway-2.6.7/runway/core/providers/aws/s3/_helpers/sync_strategy/exact_timestamps.py`

 * *Files identical despite different names*

### Comparing `runway-2.6.6/runway/core/providers/aws/s3/_helpers/sync_strategy/register.py` & `runway-2.6.7/runway/core/providers/aws/s3/_helpers/sync_strategy/register.py`

 * *Files identical despite different names*

### Comparing `runway-2.6.6/runway/core/providers/aws/s3/_helpers/sync_strategy/size_only.py` & `runway-2.6.7/runway/core/providers/aws/s3/_helpers/sync_strategy/size_only.py`

 * *Files identical despite different names*

### Comparing `runway-2.6.6/runway/core/providers/aws/s3/_helpers/transfer_config.py` & `runway-2.6.7/runway/core/providers/aws/s3/_helpers/transfer_config.py`

 * *Files identical despite different names*

### Comparing `runway-2.6.6/runway/core/providers/aws/s3/_helpers/utils.py` & `runway-2.6.7/runway/core/providers/aws/s3/_helpers/utils.py`

 * *Files identical despite different names*

### Comparing `runway-2.6.6/runway/core/providers/aws/s3/_sync_handler.py` & `runway-2.6.7/runway/core/providers/aws/s3/_sync_handler.py`

 * *Files identical despite different names*

### Comparing `runway-2.6.6/runway/core/providers/aws/s3/exceptions.py` & `runway-2.6.7/runway/core/providers/aws/s3/exceptions.py`

 * *Files identical despite different names*

### Comparing `runway-2.6.6/runway/dependency_managers/__init__.py` & `runway-2.6.7/runway/dependency_managers/__init__.py`

 * *Files identical despite different names*

### Comparing `runway-2.6.6/runway/dependency_managers/_pip.py` & `runway-2.6.7/runway/dependency_managers/_pip.py`

 * *Files identical despite different names*

### Comparing `runway-2.6.6/runway/dependency_managers/_pipenv.py` & `runway-2.6.7/runway/dependency_managers/_pipenv.py`

 * *Files identical despite different names*

### Comparing `runway-2.6.6/runway/dependency_managers/_poetry.py` & `runway-2.6.7/runway/dependency_managers/_poetry.py`

 * *Files identical despite different names*

### Comparing `runway-2.6.6/runway/dependency_managers/base_classes.py` & `runway-2.6.7/runway/dependency_managers/base_classes.py`

 * *Files identical despite different names*

### Comparing `runway-2.6.6/runway/env_mgr/__init__.py` & `runway-2.6.7/runway/env_mgr/__init__.py`

 * *Files identical despite different names*

### Comparing `runway-2.6.6/runway/env_mgr/kbenv.py` & `runway-2.6.7/runway/env_mgr/kbenv.py`

 * *Files identical despite different names*

### Comparing `runway-2.6.6/runway/env_mgr/tfenv.py` & `runway-2.6.7/runway/env_mgr/tfenv.py`

 * *Files identical despite different names*

### Comparing `runway-2.6.6/runway/exceptions.py` & `runway-2.6.7/runway/exceptions.py`

 * *Files identical despite different names*

### Comparing `runway-2.6.6/runway/lookups/handlers/base.py` & `runway-2.6.7/runway/lookups/handlers/base.py`

 * *Files identical despite different names*

### Comparing `runway-2.6.6/runway/lookups/handlers/cfn.py` & `runway-2.6.7/runway/lookups/handlers/cfn.py`

 * *Files identical despite different names*

### Comparing `runway-2.6.6/runway/lookups/handlers/ecr.py` & `runway-2.6.7/runway/lookups/handlers/ecr.py`

 * *Files identical despite different names*

### Comparing `runway-2.6.6/runway/lookups/handlers/env.py` & `runway-2.6.7/runway/lookups/handlers/env.py`

 * *Files identical despite different names*

### Comparing `runway-2.6.6/runway/lookups/handlers/random_string.py` & `runway-2.6.7/runway/lookups/handlers/random_string.py`

 * *Files identical despite different names*

### Comparing `runway-2.6.6/runway/lookups/handlers/ssm.py` & `runway-2.6.7/runway/lookups/handlers/ssm.py`

 * *Files identical despite different names*

### Comparing `runway-2.6.6/runway/lookups/handlers/var.py` & `runway-2.6.7/runway/lookups/handlers/var.py`

 * *Files identical despite different names*

### Comparing `runway-2.6.6/runway/lookups/registry.py` & `runway-2.6.7/runway/lookups/registry.py`

 * *Files identical despite different names*

### Comparing `runway-2.6.6/runway/mixins.py` & `runway-2.6.7/runway/mixins.py`

 * *Files identical despite different names*

### Comparing `runway-2.6.6/runway/module/base.py` & `runway-2.6.7/runway/module/base.py`

 * *Files identical despite different names*

### Comparing `runway-2.6.6/runway/module/cdk.py` & `runway-2.6.7/runway/module/cdk.py`

 * *Files identical despite different names*

### Comparing `runway-2.6.6/runway/module/cloudformation.py` & `runway-2.6.7/runway/module/cloudformation.py`

 * *Files identical despite different names*

### Comparing `runway-2.6.6/runway/module/k8s.py` & `runway-2.6.7/runway/module/k8s.py`

 * *Files identical despite different names*

### Comparing `runway-2.6.6/runway/module/serverless.py` & `runway-2.6.7/runway/module/serverless.py`

 * *Files identical despite different names*

### Comparing `runway-2.6.6/runway/module/staticsite/handler.py` & `runway-2.6.7/runway/module/staticsite/handler.py`

 * *Files identical despite different names*

### Comparing `runway-2.6.6/runway/module/staticsite/options/__init__.py` & `runway-2.6.7/runway/module/staticsite/options/__init__.py`

 * *Files identical despite different names*

### Comparing `runway-2.6.6/runway/module/staticsite/options/components.py` & `runway-2.6.7/runway/module/staticsite/options/components.py`

 * *Files identical despite different names*

### Comparing `runway-2.6.6/runway/module/staticsite/options/models.py` & `runway-2.6.7/runway/module/staticsite/options/models.py`

 * *Files identical despite different names*

### Comparing `runway-2.6.6/runway/module/staticsite/parameters/models.py` & `runway-2.6.7/runway/module/staticsite/parameters/models.py`

 * *Files identical despite different names*

### Comparing `runway-2.6.6/runway/module/terraform.py` & `runway-2.6.7/runway/module/terraform.py`

 * *Files identical despite different names*

### Comparing `runway-2.6.6/runway/module/utils.py` & `runway-2.6.7/runway/module/utils.py`

 * *Files identical despite different names*

### Comparing `runway-2.6.6/runway/s3_utils.py` & `runway-2.6.7/runway/s3_utils.py`

 * *Files identical despite different names*

### Comparing `runway-2.6.6/runway/sources/git.py` & `runway-2.6.7/runway/sources/git.py`

 * *Files identical despite different names*

### Comparing `runway-2.6.6/runway/sources/source.py` & `runway-2.6.7/runway/sources/source.py`

 * *Files identical despite different names*

### Comparing `runway-2.6.6/runway/templates/.pylintrc` & `runway-2.6.7/runway/templates/.pylintrc`

 * *Files identical despite different names*

### Comparing `runway-2.6.6/runway/templates/cdk-csharp/README.md` & `runway-2.6.7/runway/templates/cdk-csharp/README.md`

 * *Files identical despite different names*

### Comparing `runway-2.6.6/runway/templates/cdk-csharp/dot_gitignore` & `runway-2.6.7/runway/templates/cdk-csharp/dot_gitignore`

 * *Files identical despite different names*

### Comparing `runway-2.6.6/runway/templates/cdk-csharp/src/HelloCdk/HelloConstruct.cs` & `runway-2.6.7/runway/templates/cdk-csharp/src/HelloCdk/HelloConstruct.cs`

 * *Files identical despite different names*

### Comparing `runway-2.6.6/runway/templates/cdk-csharp/src/HelloCdk/HelloStack.cs` & `runway-2.6.7/runway/templates/cdk-csharp/src/HelloCdk/HelloStack.cs`

 * *Files identical despite different names*

### Comparing `runway-2.6.6/runway/templates/cdk-csharp/src/HelloCdk/Program.cs` & `runway-2.6.7/runway/templates/cdk-csharp/src/HelloCdk/Program.cs`

 * *Files identical despite different names*

### Comparing `runway-2.6.6/runway/templates/cdk-csharp/src/HelloCdk.sln` & `runway-2.6.7/runway/templates/cdk-csharp/src/HelloCdk.sln`

 * *Files identical despite different names*

### Comparing `runway-2.6.6/runway/templates/cdk-py/hello/hello_construct.py` & `runway-2.6.7/runway/templates/cdk-py/hello/hello_construct.py`

 * *Files identical despite different names*

### Comparing `runway-2.6.6/runway/templates/cdk-py/hello/hello_stack.py` & `runway-2.6.7/runway/templates/cdk-py/hello/hello_stack.py`

 * *Files identical despite different names*

### Comparing `runway-2.6.6/runway/templates/cdk-py/poetry.lock` & `runway-2.6.7/runway/templates/cdk-py/poetry.lock`

 * *Files identical despite different names*

### Comparing `runway-2.6.6/runway/templates/cdk-py/pyproject.toml` & `runway-2.6.7/runway/templates/cdk-py/pyproject.toml`

 * *Files identical despite different names*

### Comparing `runway-2.6.6/runway/templates/cdk-tsc/tsconfig.json` & `runway-2.6.7/runway/templates/cdk-tsc/tsconfig.json`

 * *Files identical despite different names*

### Comparing `runway-2.6.6/runway/templates/k8s-cfn-repo/README.md` & `runway-2.6.7/runway/templates/k8s-cfn-repo/README.md`

 * *Files identical despite different names*

### Comparing `runway-2.6.6/runway/templates/k8s-cfn-repo/k8s-master.cfn/k8s_hooks/auth_map.py` & `runway-2.6.7/runway/templates/k8s-cfn-repo/k8s-master.cfn/k8s_hooks/auth_map.py`

 * *Files identical despite different names*

### Comparing `runway-2.6.6/runway/templates/k8s-cfn-repo/k8s-master.cfn/k8s_hooks/awscli.py` & `runway-2.6.7/runway/templates/k8s-cfn-repo/k8s-master.cfn/k8s_hooks/awscli.py`

 * *Files identical despite different names*

### Comparing `runway-2.6.6/runway/templates/k8s-cfn-repo/k8s-master.cfn/k8s_hooks/bootstrap.py` & `runway-2.6.7/runway/templates/k8s-cfn-repo/k8s-master.cfn/k8s_hooks/bootstrap.py`

 * *Files identical despite different names*

### Comparing `runway-2.6.6/runway/templates/k8s-cfn-repo/k8s-master.cfn/stacks.yaml` & `runway-2.6.7/runway/templates/k8s-cfn-repo/k8s-master.cfn/stacks.yaml`

 * *Files identical despite different names*

### Comparing `runway-2.6.6/runway/templates/k8s-cfn-repo/k8s-workers.cfn/local_lookups/bootstrap_value.py` & `runway-2.6.7/runway/templates/k8s-cfn-repo/k8s-workers.cfn/local_lookups/bootstrap_value.py`

 * *Files identical despite different names*

### Comparing `runway-2.6.6/runway/templates/k8s-cfn-repo/k8s-workers.cfn/stacks.yaml` & `runway-2.6.7/runway/templates/k8s-cfn-repo/k8s-workers.cfn/stacks.yaml`

 * *Files identical despite different names*

### Comparing `runway-2.6.6/runway/templates/k8s-cfn-repo/runway.yml` & `runway-2.6.7/runway/templates/k8s-cfn-repo/runway.yml`

 * *Files identical despite different names*

### Comparing `runway-2.6.6/runway/templates/k8s-cfn-repo/service-hello-world.k8s/base/deployment.yaml` & `runway-2.6.7/runway/templates/k8s-cfn-repo/service-hello-world.k8s/base/deployment.yaml`

 * *Files identical despite different names*

### Comparing `runway-2.6.6/runway/templates/k8s-flux-repo/README.md` & `runway-2.6.7/runway/templates/k8s-flux-repo/README.md`

 * *Files identical despite different names*

### Comparing `runway-2.6.6/runway/templates/k8s-flux-repo/flux.tf/.terraform.lock.hcl` & `runway-2.6.7/runway/templates/k8s-flux-repo/flux.tf/.terraform.lock.hcl`

 * *Files identical despite different names*

### Comparing `runway-2.6.6/runway/templates/k8s-flux-repo/flux.tf/docker/Dockerfile` & `runway-2.6.7/runway/templates/k8s-flux-repo/flux.tf/docker/Dockerfile`

 * *Files identical despite different names*

### Comparing `runway-2.6.6/runway/templates/k8s-flux-repo/flux.tf/main.tf` & `runway-2.6.7/runway/templates/k8s-flux-repo/flux.tf/main.tf`

 * *Files identical despite different names*

### Comparing `runway-2.6.6/runway/templates/k8s-flux-repo/runway.yml` & `runway-2.6.7/runway/templates/k8s-flux-repo/runway.yml`

 * *Files identical despite different names*

### Comparing `runway-2.6.6/runway/templates/k8s-tf-repo/README.md` & `runway-2.6.7/runway/templates/k8s-tf-repo/README.md`

 * *Files identical despite different names*

### Comparing `runway-2.6.6/runway/templates/k8s-tf-repo/eks-base.tf/.terraform.lock.hcl` & `runway-2.6.7/runway/templates/k8s-tf-repo/eks-base.tf/.terraform.lock.hcl`

 * *Files identical despite different names*

### Comparing `runway-2.6.6/runway/templates/k8s-tf-repo/eks-base.tf/main.tf` & `runway-2.6.7/runway/templates/k8s-tf-repo/eks-base.tf/main.tf`

 * *Files identical despite different names*

### Comparing `runway-2.6.6/runway/templates/k8s-tf-repo/job-s3-echo.tf/.terraform.lock.hcl` & `runway-2.6.7/runway/templates/k8s-tf-repo/job-s3-echo.tf/.terraform.lock.hcl`

 * *Files identical despite different names*

### Comparing `runway-2.6.6/runway/templates/k8s-tf-repo/job-s3-echo.tf/main.tf` & `runway-2.6.7/runway/templates/k8s-tf-repo/job-s3-echo.tf/main.tf`

 * *Files identical despite different names*

### Comparing `runway-2.6.6/runway/templates/k8s-tf-repo/runway.yml` & `runway-2.6.7/runway/templates/k8s-tf-repo/runway.yml`

 * *Files identical despite different names*

### Comparing `runway-2.6.6/runway/templates/k8s-tf-repo/service-hello-world.k8s/base/deployment.yaml` & `runway-2.6.7/runway/templates/k8s-tf-repo/service-hello-world.k8s/base/deployment.yaml`

 * *Files identical despite different names*

### Comparing `runway-2.6.6/runway/templates/sls-py/hello_world/__init__.py` & `runway-2.6.7/runway/templates/sls-py/hello_world/__init__.py`

 * *Files identical despite different names*

### Comparing `runway-2.6.6/runway/templates/sls-py/poetry.lock` & `runway-2.6.7/runway/templates/sls-py/poetry.lock`

 * *Files identical despite different names*

### Comparing `runway-2.6.6/runway/templates/sls-py/serverless.yml` & `runway-2.6.7/runway/templates/sls-py/serverless.yml`

 * *Files identical despite different names*

### Comparing `runway-2.6.6/runway/templates/sls-tsc/package.json` & `runway-2.6.7/runway/templates/sls-tsc/package.json`

 * *Files identical despite different names*

### Comparing `runway-2.6.6/runway/templates/sls-tsc/serverless.yml` & `runway-2.6.7/runway/templates/sls-tsc/serverless.yml`

 * *Files identical despite different names*

### Comparing `runway-2.6.6/runway/templates/sls-tsc/src/helloWorld.test.ts` & `runway-2.6.7/runway/templates/sls-tsc/src/helloWorld.test.ts`

 * *Files identical despite different names*

### Comparing `runway-2.6.6/runway/templates/sls-tsc/src/helloWorld.ts` & `runway-2.6.7/runway/templates/sls-tsc/src/helloWorld.ts`

 * *Files identical despite different names*

### Comparing `runway-2.6.6/runway/templates/sls-tsc/tsconfig.json` & `runway-2.6.7/runway/templates/sls-tsc/tsconfig.json`

 * *Files identical despite different names*

### Comparing `runway-2.6.6/runway/templates/sls-tsc/webpack.config.js` & `runway-2.6.7/runway/templates/sls-tsc/webpack.config.js`

 * *Files identical despite different names*

### Comparing `runway-2.6.6/runway/templates/static-angular/sampleapp.web/README.md` & `runway-2.6.7/runway/templates/static-angular/sampleapp.web/README.md`

 * *Files identical despite different names*

### Comparing `runway-2.6.6/runway/templates/static-angular/sampleapp.web/_gitignore` & `runway-2.6.7/runway/templates/static-angular/sampleapp.web/_gitignore`

 * *Files identical despite different names*

### Comparing `runway-2.6.6/runway/templates/static-angular/sampleapp.web/angular.json` & `runway-2.6.7/runway/templates/static-angular/sampleapp.web/angular.json`

 * *Files identical despite different names*

### Comparing `runway-2.6.6/runway/templates/static-angular/sampleapp.web/e2e/protractor.conf.js` & `runway-2.6.7/runway/templates/static-angular/sampleapp.web/e2e/protractor.conf.js`

 * *Files identical despite different names*

### Comparing `runway-2.6.6/runway/templates/static-angular/sampleapp.web/e2e/src/app.e2e-spec.ts` & `runway-2.6.7/runway/templates/static-angular/sampleapp.web/e2e/src/app.e2e-spec.ts`

 * *Files identical despite different names*

### Comparing `runway-2.6.6/runway/templates/static-angular/sampleapp.web/karma.conf.js` & `runway-2.6.7/runway/templates/static-angular/sampleapp.web/karma.conf.js`

 * *Files identical despite different names*

### Comparing `runway-2.6.6/runway/templates/static-angular/sampleapp.web/package-lock.json` & `runway-2.6.7/runway/templates/static-angular/sampleapp.web/package-lock.json`

 * *Files identical despite different names*

### Comparing `runway-2.6.6/runway/templates/static-angular/sampleapp.web/package.json` & `runway-2.6.7/runway/templates/static-angular/sampleapp.web/package.json`

 * *Files identical despite different names*

### Comparing `runway-2.6.6/runway/templates/static-angular/sampleapp.web/src/app/app.component.html` & `runway-2.6.7/runway/templates/static-angular/sampleapp.web/src/app/app.component.html`

 * *Files identical despite different names*

### Comparing `runway-2.6.6/runway/templates/static-angular/sampleapp.web/src/app/app.component.spec.ts` & `runway-2.6.7/runway/templates/static-angular/sampleapp.web/src/app/app.component.spec.ts`

 * *Files identical despite different names*

### Comparing `runway-2.6.6/runway/templates/static-angular/sampleapp.web/src/environments/environment.ts` & `runway-2.6.7/runway/templates/static-angular/sampleapp.web/src/environments/environment.ts`

 * *Files identical despite different names*

### Comparing `runway-2.6.6/runway/templates/static-angular/sampleapp.web/src/favicon.ico` & `runway-2.6.7/runway/templates/static-angular/sampleapp.web/src/favicon.ico`

 * *Files identical despite different names*

### Comparing `runway-2.6.6/runway/templates/static-angular/sampleapp.web/src/polyfills.ts` & `runway-2.6.7/runway/templates/static-angular/sampleapp.web/src/polyfills.ts`

 * *Files identical despite different names*

### Comparing `runway-2.6.6/runway/templates/static-angular/sampleapp.web/src/test.ts` & `runway-2.6.7/runway/templates/static-angular/sampleapp.web/src/test.ts`

 * *Files identical despite different names*

### Comparing `runway-2.6.6/runway/templates/static-angular/sampleapp.web/tsconfig.json` & `runway-2.6.7/runway/templates/static-angular/sampleapp.web/tsconfig.json`

 * *Files identical despite different names*

### Comparing `runway-2.6.6/runway/templates/static-angular/sampleapp.web/tslint.json` & `runway-2.6.7/runway/templates/static-angular/sampleapp.web/tslint.json`

 * *Files identical despite different names*

### Comparing `runway-2.6.6/runway/templates/static-react/sampleapp.web/README.md` & `runway-2.6.7/runway/templates/static-react/sampleapp.web/README.md`

 * *Files identical despite different names*

### Comparing `runway-2.6.6/runway/templates/static-react/sampleapp.web/package.json` & `runway-2.6.7/runway/templates/static-react/sampleapp.web/package.json`

 * *Files identical despite different names*

### Comparing `runway-2.6.6/runway/templates/static-react/sampleapp.web/public/favicon.ico` & `runway-2.6.7/runway/templates/static-react/sampleapp.web/public/favicon.ico`

 * *Files identical despite different names*

### Comparing `runway-2.6.6/runway/templates/static-react/sampleapp.web/public/index.html` & `runway-2.6.7/runway/templates/static-react/sampleapp.web/public/index.html`

 * *Files identical despite different names*

### Comparing `runway-2.6.6/runway/templates/static-react/sampleapp.web/public/logo192.png` & `runway-2.6.7/runway/templates/static-react/sampleapp.web/public/logo192.png`

 * *Files identical despite different names*

### Comparing `runway-2.6.6/runway/templates/static-react/sampleapp.web/public/logo512.png` & `runway-2.6.7/runway/templates/static-react/sampleapp.web/public/logo512.png`

 * *Files identical despite different names*

### Comparing `runway-2.6.6/runway/templates/static-react/sampleapp.web/src/App.css` & `runway-2.6.7/runway/templates/static-react/sampleapp.web/src/App.css`

 * *Files identical despite different names*

### Comparing `runway-2.6.6/runway/templates/static-react/sampleapp.web/src/App.js` & `runway-2.6.7/runway/templates/static-react/sampleapp.web/src/App.js`

 * *Files identical despite different names*

### Comparing `runway-2.6.6/runway/templates/static-react/sampleapp.web/src/logo.svg` & `runway-2.6.7/runway/templates/static-react/sampleapp.web/src/logo.svg`

 * *Files identical despite different names*

### Comparing `runway-2.6.6/runway/templates/static-react/sampleapp.web/src/serviceWorker.js` & `runway-2.6.7/runway/templates/static-react/sampleapp.web/src/serviceWorker.js`

 * *Files identical despite different names*

### Comparing `runway-2.6.6/runway/tests/handlers/base.py` & `runway-2.6.7/runway/tests/handlers/base.py`

 * *Files identical despite different names*

### Comparing `runway-2.6.6/runway/tests/handlers/cfn_lint.py` & `runway-2.6.7/runway/tests/handlers/cfn_lint.py`

 * *Files identical despite different names*

### Comparing `runway-2.6.6/runway/tests/handlers/script.py` & `runway-2.6.7/runway/tests/handlers/script.py`

 * *Files identical despite different names*

### Comparing `runway-2.6.6/runway/tests/handlers/yaml_lint.py` & `runway-2.6.7/runway/tests/handlers/yaml_lint.py`

 * *Files identical despite different names*

### Comparing `runway-2.6.6/runway/tests/registry.py` & `runway-2.6.7/runway/tests/registry.py`

 * *Files identical despite different names*

### Comparing `runway-2.6.6/runway/type_defs.py` & `runway-2.6.7/runway/type_defs.py`

 * *Files identical despite different names*

### Comparing `runway-2.6.6/runway/utils/__init__.py` & `runway-2.6.7/runway/utils/__init__.py`

 * *Files identical despite different names*

### Comparing `runway-2.6.6/runway/utils/_file_hash.py` & `runway-2.6.7/runway/utils/_file_hash.py`

 * *Files identical despite different names*

### Comparing `runway-2.6.6/runway/utils/_version.py` & `runway-2.6.7/runway/utils/_version.py`

 * *Files identical despite different names*

### Comparing `runway-2.6.6/runway/variables.py` & `runway-2.6.7/runway/variables.py`

 * *Files identical despite different names*

### Comparing `runway-2.6.6/PKG-INFO` & `runway-2.6.7/PKG-INFO`

 * *Files 0% similar despite different names*

```diff
@@ -1,19 +1,19 @@
 Metadata-Version: 2.1
 Name: runway
-Version: 2.6.6
+Version: 2.6.7
 Summary: Simplify infrastructure/app testing/deployment
 Home-page: https://github.com/onicagroup/runway
 License: Apache-2.0
 Keywords: cli
 Author: Onica Group LLC
 Author-email: opensource@onica.com
 Maintainer: Kyle Finley
 Maintainer-email: kyle@finley.sh
-Requires-Python: >=3.8,<3.12
+Requires-Python: >=3.8,<4
 Classifier: Intended Audience :: Developers
 Classifier: License :: OSI Approved :: Apache Software License
 Classifier: Natural Language :: English
 Classifier: Operating System :: OS Independent
 Classifier: Programming Language :: Python :: 3
 Classifier: Programming Language :: Python :: 3.8
 Classifier: Programming Language :: Python :: 3.9
```

