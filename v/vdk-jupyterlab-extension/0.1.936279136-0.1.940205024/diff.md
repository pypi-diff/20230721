# Comparing `tmp/vdk_jupyterlab_extension-0.1.936279136.tar.gz` & `tmp/vdk_jupyterlab_extension-0.1.940205024.tar.gz`

## Comparing `vdk_jupyterlab_extension-0.1.936279136.tar` & `vdk_jupyterlab_extension-0.1.940205024.tar`

### file list

```diff
@@ -1,79 +1,80 @@
--rw-r--r--   0        0        0       66 2020-02-02 00:00:00.000000 vdk_jupyterlab_extension-0.1.936279136/.eslintignore
--rw-r--r--   0        0        0     1109 2020-02-02 00:00:00.000000 vdk_jupyterlab_extension-0.1.936279136/.eslintrc.js
--rw-r--r--   0        0        0       77 2020-02-02 00:00:00.000000 vdk_jupyterlab_extension-0.1.936279136/.prettierignore
--rw-r--r--   0        0        0      102 2020-02-02 00:00:00.000000 vdk_jupyterlab_extension-0.1.936279136/.prettierrc
--rw-r--r--   0        0        0      260 2020-02-02 00:00:00.000000 vdk_jupyterlab_extension-0.1.936279136/.stylelintrc
--rw-r--r--   0        0        0      151 2020-02-02 00:00:00.000000 vdk_jupyterlab_extension-0.1.936279136/babel.config.js
--rw-r--r--   0        0        0      283 2020-02-02 00:00:00.000000 vdk_jupyterlab_extension-0.1.936279136/conftest.py
--rw-r--r--   0        0        0      209 2020-02-02 00:00:00.000000 vdk_jupyterlab_extension-0.1.936279136/install.json
--rw-r--r--   0        0        0     1023 2020-02-02 00:00:00.000000 vdk_jupyterlab_extension-0.1.936279136/jest.config.js
--rw-r--r--   0        0        0  1169752 2020-02-02 00:00:00.000000 vdk_jupyterlab_extension-0.1.936279136/package-lock.json
--rw-r--r--   0        0        0     5649 2020-02-02 00:00:00.000000 vdk_jupyterlab_extension-0.1.936279136/package.json
--rw-r--r--   0        0        0      583 2020-02-02 00:00:00.000000 vdk_jupyterlab_extension-0.1.936279136/tsconfig.json
--rw-r--r--   0        0        0   423537 2020-02-02 00:00:00.000000 vdk_jupyterlab_extension-0.1.936279136/yarn.lock
--rw-r--r--   0        0        0      101 2020-02-02 00:00:00.000000 vdk_jupyterlab_extension-0.1.936279136/jupyter-config/nb-config/vdk-jupyterlab-extension.json
--rw-r--r--   0        0        0       99 2020-02-02 00:00:00.000000 vdk_jupyterlab_extension-0.1.936279136/jupyter-config/server-config/vdk-jupyterlab-extension.json
--rw-r--r--   0        0        0      797 2020-02-02 00:00:00.000000 vdk_jupyterlab_extension-0.1.936279136/schema/plugin.json
--rw-r--r--   0        0        0     2959 2020-02-02 00:00:00.000000 vdk_jupyterlab_extension-0.1.936279136/src/commandsAndMenu.tsx
--rw-r--r--   0        0        0     1190 2020-02-02 00:00:00.000000 vdk_jupyterlab_extension-0.1.936279136/src/handler.ts
--rw-r--r--   0        0        0     1740 2020-02-02 00:00:00.000000 vdk_jupyterlab_extension-0.1.936279136/src/index.ts
--rw-r--r--   0        0        0     2250 2020-02-02 00:00:00.000000 vdk_jupyterlab_extension-0.1.936279136/src/jobData.ts
--rw-r--r--   0        0        0     5310 2020-02-02 00:00:00.000000 vdk_jupyterlab_extension-0.1.936279136/src/serverRequests.ts
--rw-r--r--   0        0        0      495 2020-02-02 00:00:00.000000 vdk_jupyterlab_extension-0.1.936279136/src/utils.ts
--rw-r--r--   0        0        0     4303 2020-02-02 00:00:00.000000 vdk_jupyterlab_extension-0.1.936279136/src/vdkTags.ts
--rw-r--r--   0        0        0     1351 2020-02-02 00:00:00.000000 vdk_jupyterlab_extension-0.1.936279136/src/__tests__/convert-job-to-notebook-component.spec.ts
--rw-r--r--   0        0        0     3694 2020-02-02 00:00:00.000000 vdk_jupyterlab_extension-0.1.936279136/src/__tests__/create-job-component.spec.ts
--rw-r--r--   0        0        0     3645 2020-02-02 00:00:00.000000 vdk_jupyterlab_extension-0.1.936279136/src/__tests__/deploy-job-component.spec.ts
--rw-r--r--   0        0        0     2667 2020-02-02 00:00:00.000000 vdk_jupyterlab_extension-0.1.936279136/src/__tests__/download-job-component.spec.ts
--rw-r--r--   0        0        0     2522 2020-02-02 00:00:00.000000 vdk_jupyterlab_extension-0.1.936279136/src/__tests__/handler.spec.ts
--rw-r--r--   0        0        0     5475 2020-02-02 00:00:00.000000 vdk_jupyterlab_extension-0.1.936279136/src/__tests__/resquests.spec.ts
--rw-r--r--   0        0        0     6323 2020-02-02 00:00:00.000000 vdk_jupyterlab_extension-0.1.936279136/src/__tests__/run-job-component.spec.tsx
--rw-r--r--   0        0        0     6907 2020-02-02 00:00:00.000000 vdk_jupyterlab_extension-0.1.936279136/src/__tests__/show-dialog.spec.tsx
--rw-r--r--   0        0        0     3076 2020-02-02 00:00:00.000000 vdk_jupyterlab_extension-0.1.936279136/src/__tests__/vdk-error-message.spec.ts
--rw-r--r--   0        0        0      282 2020-02-02 00:00:00.000000 vdk_jupyterlab_extension-0.1.936279136/src/__tests__/vdk-jupyterlab-extension.spec.ts
--rw-r--r--   0        0        0     3910 2020-02-02 00:00:00.000000 vdk_jupyterlab_extension-0.1.936279136/src/__tests__/vdk-tags.spec.ts
--rw-r--r--   0        0        0     3047 2020-02-02 00:00:00.000000 vdk_jupyterlab_extension-0.1.936279136/src/components/ConvertJobToNotebook.tsx
--rw-r--r--   0        0        0     3422 2020-02-02 00:00:00.000000 vdk_jupyterlab_extension-0.1.936279136/src/components/CreateJob.tsx
--rw-r--r--   0        0        0     3771 2020-02-02 00:00:00.000000 vdk_jupyterlab_extension-0.1.936279136/src/components/DeployJob.tsx
--rw-r--r--   0        0        0     1648 2020-02-02 00:00:00.000000 vdk_jupyterlab_extension-0.1.936279136/src/components/DownloadJob.tsx
--rw-r--r--   0        0        0     7861 2020-02-02 00:00:00.000000 vdk_jupyterlab_extension-0.1.936279136/src/components/RunJob.tsx
--rw-r--r--   0        0        0     1549 2020-02-02 00:00:00.000000 vdk_jupyterlab_extension-0.1.936279136/src/components/VdkErrorMessage.ts
--rw-r--r--   0        0        0     2054 2020-02-02 00:00:00.000000 vdk_jupyterlab_extension-0.1.936279136/src/components/VdkTextInput.tsx
--rw-r--r--   0        0        0      337 2020-02-02 00:00:00.000000 vdk_jupyterlab_extension-0.1.936279136/src/components/props.tsx
--rw-r--r--   0        0        0      312 2020-02-02 00:00:00.000000 vdk_jupyterlab_extension-0.1.936279136/src/vdkOptions/vdk_options.ts
--rw-r--r--   0        0        0      992 2020-02-02 00:00:00.000000 vdk_jupyterlab_extension-0.1.936279136/style/base.css
--rw-r--r--   0        0        0      108 2020-02-02 00:00:00.000000 vdk_jupyterlab_extension-0.1.936279136/style/index.css
--rw-r--r--   0        0        0      104 2020-02-02 00:00:00.000000 vdk_jupyterlab_extension-0.1.936279136/style/index.js
--rw-r--r--   0        0        0      865 2020-02-02 00:00:00.000000 vdk_jupyterlab_extension-0.1.936279136/style/vdkDialogs.css
--rw-r--r--   0        0        0     7626 2020-02-02 00:00:00.000000 vdk_jupyterlab_extension-0.1.936279136/style/images/versatile-data-kit-logo.svg
--rw-r--r--   0        0        0     3343 2020-02-02 00:00:00.000000 vdk_jupyterlab_extension-0.1.936279136/ui-tests/README.md
--rw-r--r--   0        0        0      682 2020-02-02 00:00:00.000000 vdk_jupyterlab_extension-0.1.936279136/ui-tests/jupyter_server_test_config.py
--rw-r--r--   0        0        0      350 2020-02-02 00:00:00.000000 vdk_jupyterlab_extension-0.1.936279136/ui-tests/package.json
--rw-r--r--   0        0        0      425 2020-02-02 00:00:00.000000 vdk_jupyterlab_extension-0.1.936279136/ui-tests/playwright.config.js
--rw-r--r--   0        0        0     4245 2020-02-02 00:00:00.000000 vdk_jupyterlab_extension-0.1.936279136/ui-tests/tests/vdk-jupyterlab-extension.spec.ts
--rw-r--r--   0        0        0      891 2020-02-02 00:00:00.000000 vdk_jupyterlab_extension-0.1.936279136/vdk_jupyterlab_extension/__init__.py
--rw-r--r--   0        0        0      179 2020-02-02 00:00:00.000000 vdk_jupyterlab_extension-0.1.936279136/vdk_jupyterlab_extension/_version.py
--rw-r--r--   0        0        0     6936 2020-02-02 00:00:00.000000 vdk_jupyterlab_extension-0.1.936279136/vdk_jupyterlab_extension/handlers.py
--rw-r--r--   0        0        0      724 2020-02-02 00:00:00.000000 vdk_jupyterlab_extension-0.1.936279136/vdk_jupyterlab_extension/job_data.py
--rw-r--r--   0        0        0     8397 2020-02-02 00:00:00.000000 vdk_jupyterlab_extension-0.1.936279136/vdk_jupyterlab_extension/vdk_ui.py
--rw-r--r--   0        0        0     2350 2020-02-02 00:00:00.000000 vdk_jupyterlab_extension-0.1.936279136/vdk_jupyterlab_extension/jupyter_sample_job/10_notebook.ipynb
--rw-r--r--   0        0        0     1534 2020-02-02 00:00:00.000000 vdk_jupyterlab_extension-0.1.936279136/vdk_jupyterlab_extension/jupyter_sample_job/README.md
--rw-r--r--   0        0        0     2850 2020-02-02 00:00:00.000000 vdk_jupyterlab_extension-0.1.936279136/vdk_jupyterlab_extension/jupyter_sample_job/config.ini
--rw-r--r--   0        0        0      243 2020-02-02 00:00:00.000000 vdk_jupyterlab_extension-0.1.936279136/vdk_jupyterlab_extension/jupyter_sample_job/requirements.txt
--rw-r--r--   0        0        0     5205 2020-02-02 00:00:00.000000 vdk_jupyterlab_extension-0.1.936279136/vdk_jupyterlab_extension/labextension/package.json
--rw-r--r--   0        0        0     5649 2020-02-02 00:00:00.000000 vdk_jupyterlab_extension-0.1.936279136/vdk_jupyterlab_extension/labextension/schemas/vdk-jupyterlab-extension/package.json.orig
--rw-r--r--   0        0        0      797 2020-02-02 00:00:00.000000 vdk_jupyterlab_extension-0.1.936279136/vdk_jupyterlab_extension/labextension/schemas/vdk-jupyterlab-extension/plugin.json
--rw-r--r--   0        0        0    15543 2020-02-02 00:00:00.000000 vdk_jupyterlab_extension-0.1.936279136/vdk_jupyterlab_extension/labextension/static/381.0485c5d1f906c39de85e.js
--rw-r--r--   0        0        0     5454 2020-02-02 00:00:00.000000 vdk_jupyterlab_extension-0.1.936279136/vdk_jupyterlab_extension/labextension/static/747.e678254df7945f8ed34d.js
--rw-r--r--   0        0        0     6841 2020-02-02 00:00:00.000000 vdk_jupyterlab_extension-0.1.936279136/vdk_jupyterlab_extension/labextension/static/remoteEntry.77b468e1169ec9f71a16.js
--rw-r--r--   0        0        0      167 2020-02-02 00:00:00.000000 vdk_jupyterlab_extension-0.1.936279136/vdk_jupyterlab_extension/labextension/static/style.js
--rw-r--r--   0        0        0     2452 2020-02-02 00:00:00.000000 vdk_jupyterlab_extension-0.1.936279136/vdk_jupyterlab_extension/labextension/static/third-party-licenses.json
--rw-r--r--   0        0        0      127 2020-02-02 00:00:00.000000 vdk_jupyterlab_extension-0.1.936279136/vdk_jupyterlab_extension/tests/__init__.py
--rw-r--r--   0        0        0      397 2020-02-02 00:00:00.000000 vdk_jupyterlab_extension-0.1.936279136/vdk_jupyterlab_extension/tests/test_handlers.py
--rw-r--r--   0        0        0       73 2020-02-02 00:00:00.000000 vdk_jupyterlab_extension-0.1.936279136/vdk_jupyterlab_extension/vdk_options/__init__.py
--rw-r--r--   0        0        0      332 2020-02-02 00:00:00.000000 vdk_jupyterlab_extension-0.1.936279136/vdk_jupyterlab_extension/vdk_options/vdk_options.py
--rw-r--r--   0        0        0     1628 2020-02-02 00:00:00.000000 vdk_jupyterlab_extension-0.1.936279136/.gitignore
--rw-r--r--   0        0        0       67 2020-02-02 00:00:00.000000 vdk_jupyterlab_extension-0.1.936279136/LICENSE
--rw-r--r--   0        0        0     7167 2020-02-02 00:00:00.000000 vdk_jupyterlab_extension-0.1.936279136/README.md
--rw-r--r--   0        0        0     2564 2020-02-02 00:00:00.000000 vdk_jupyterlab_extension-0.1.936279136/pyproject.toml
--rw-r--r--   0        0        0     8775 2020-02-02 00:00:00.000000 vdk_jupyterlab_extension-0.1.936279136/PKG-INFO
+-rw-r--r--   0        0        0       66 2020-02-02 00:00:00.000000 vdk_jupyterlab_extension-0.1.940205024/.eslintignore
+-rw-r--r--   0        0        0     1109 2020-02-02 00:00:00.000000 vdk_jupyterlab_extension-0.1.940205024/.eslintrc.js
+-rw-r--r--   0        0        0       77 2020-02-02 00:00:00.000000 vdk_jupyterlab_extension-0.1.940205024/.prettierignore
+-rw-r--r--   0        0        0      102 2020-02-02 00:00:00.000000 vdk_jupyterlab_extension-0.1.940205024/.prettierrc
+-rw-r--r--   0        0        0      260 2020-02-02 00:00:00.000000 vdk_jupyterlab_extension-0.1.940205024/.stylelintrc
+-rw-r--r--   0        0        0      151 2020-02-02 00:00:00.000000 vdk_jupyterlab_extension-0.1.940205024/babel.config.js
+-rw-r--r--   0        0        0      283 2020-02-02 00:00:00.000000 vdk_jupyterlab_extension-0.1.940205024/conftest.py
+-rw-r--r--   0        0        0      209 2020-02-02 00:00:00.000000 vdk_jupyterlab_extension-0.1.940205024/install.json
+-rw-r--r--   0        0        0     1023 2020-02-02 00:00:00.000000 vdk_jupyterlab_extension-0.1.940205024/jest.config.js
+-rw-r--r--   0        0        0  1169752 2020-02-02 00:00:00.000000 vdk_jupyterlab_extension-0.1.940205024/package-lock.json
+-rw-r--r--   0        0        0     5649 2020-02-02 00:00:00.000000 vdk_jupyterlab_extension-0.1.940205024/package.json
+-rw-r--r--   0        0        0      583 2020-02-02 00:00:00.000000 vdk_jupyterlab_extension-0.1.940205024/tsconfig.json
+-rw-r--r--   0        0        0   423537 2020-02-02 00:00:00.000000 vdk_jupyterlab_extension-0.1.940205024/yarn.lock
+-rw-r--r--   0        0        0      101 2020-02-02 00:00:00.000000 vdk_jupyterlab_extension-0.1.940205024/jupyter-config/nb-config/vdk-jupyterlab-extension.json
+-rw-r--r--   0        0        0       99 2020-02-02 00:00:00.000000 vdk_jupyterlab_extension-0.1.940205024/jupyter-config/server-config/vdk-jupyterlab-extension.json
+-rw-r--r--   0        0        0      797 2020-02-02 00:00:00.000000 vdk_jupyterlab_extension-0.1.940205024/schema/plugin.json
+-rw-r--r--   0        0        0     2959 2020-02-02 00:00:00.000000 vdk_jupyterlab_extension-0.1.940205024/src/commandsAndMenu.tsx
+-rw-r--r--   0        0        0     1190 2020-02-02 00:00:00.000000 vdk_jupyterlab_extension-0.1.940205024/src/handler.ts
+-rw-r--r--   0        0        0     1914 2020-02-02 00:00:00.000000 vdk_jupyterlab_extension-0.1.940205024/src/index.ts
+-rw-r--r--   0        0        0     1891 2020-02-02 00:00:00.000000 vdk_jupyterlab_extension-0.1.940205024/src/initVDKConfigCell.ts
+-rw-r--r--   0        0        0     2250 2020-02-02 00:00:00.000000 vdk_jupyterlab_extension-0.1.940205024/src/jobData.ts
+-rw-r--r--   0        0        0     5310 2020-02-02 00:00:00.000000 vdk_jupyterlab_extension-0.1.940205024/src/serverRequests.ts
+-rw-r--r--   0        0        0      495 2020-02-02 00:00:00.000000 vdk_jupyterlab_extension-0.1.940205024/src/utils.ts
+-rw-r--r--   0        0        0     4303 2020-02-02 00:00:00.000000 vdk_jupyterlab_extension-0.1.940205024/src/vdkTags.ts
+-rw-r--r--   0        0        0     1351 2020-02-02 00:00:00.000000 vdk_jupyterlab_extension-0.1.940205024/src/__tests__/convert-job-to-notebook-component.spec.ts
+-rw-r--r--   0        0        0     3694 2020-02-02 00:00:00.000000 vdk_jupyterlab_extension-0.1.940205024/src/__tests__/create-job-component.spec.ts
+-rw-r--r--   0        0        0     3645 2020-02-02 00:00:00.000000 vdk_jupyterlab_extension-0.1.940205024/src/__tests__/deploy-job-component.spec.ts
+-rw-r--r--   0        0        0     2667 2020-02-02 00:00:00.000000 vdk_jupyterlab_extension-0.1.940205024/src/__tests__/download-job-component.spec.ts
+-rw-r--r--   0        0        0     2522 2020-02-02 00:00:00.000000 vdk_jupyterlab_extension-0.1.940205024/src/__tests__/handler.spec.ts
+-rw-r--r--   0        0        0     5475 2020-02-02 00:00:00.000000 vdk_jupyterlab_extension-0.1.940205024/src/__tests__/resquests.spec.ts
+-rw-r--r--   0        0        0     6323 2020-02-02 00:00:00.000000 vdk_jupyterlab_extension-0.1.940205024/src/__tests__/run-job-component.spec.tsx
+-rw-r--r--   0        0        0     6907 2020-02-02 00:00:00.000000 vdk_jupyterlab_extension-0.1.940205024/src/__tests__/show-dialog.spec.tsx
+-rw-r--r--   0        0        0     3076 2020-02-02 00:00:00.000000 vdk_jupyterlab_extension-0.1.940205024/src/__tests__/vdk-error-message.spec.ts
+-rw-r--r--   0        0        0      282 2020-02-02 00:00:00.000000 vdk_jupyterlab_extension-0.1.940205024/src/__tests__/vdk-jupyterlab-extension.spec.ts
+-rw-r--r--   0        0        0     3910 2020-02-02 00:00:00.000000 vdk_jupyterlab_extension-0.1.940205024/src/__tests__/vdk-tags.spec.ts
+-rw-r--r--   0        0        0     3047 2020-02-02 00:00:00.000000 vdk_jupyterlab_extension-0.1.940205024/src/components/ConvertJobToNotebook.tsx
+-rw-r--r--   0        0        0     3422 2020-02-02 00:00:00.000000 vdk_jupyterlab_extension-0.1.940205024/src/components/CreateJob.tsx
+-rw-r--r--   0        0        0     3771 2020-02-02 00:00:00.000000 vdk_jupyterlab_extension-0.1.940205024/src/components/DeployJob.tsx
+-rw-r--r--   0        0        0     1648 2020-02-02 00:00:00.000000 vdk_jupyterlab_extension-0.1.940205024/src/components/DownloadJob.tsx
+-rw-r--r--   0        0        0     7861 2020-02-02 00:00:00.000000 vdk_jupyterlab_extension-0.1.940205024/src/components/RunJob.tsx
+-rw-r--r--   0        0        0     1549 2020-02-02 00:00:00.000000 vdk_jupyterlab_extension-0.1.940205024/src/components/VdkErrorMessage.ts
+-rw-r--r--   0        0        0     2054 2020-02-02 00:00:00.000000 vdk_jupyterlab_extension-0.1.940205024/src/components/VdkTextInput.tsx
+-rw-r--r--   0        0        0      337 2020-02-02 00:00:00.000000 vdk_jupyterlab_extension-0.1.940205024/src/components/props.tsx
+-rw-r--r--   0        0        0      312 2020-02-02 00:00:00.000000 vdk_jupyterlab_extension-0.1.940205024/src/vdkOptions/vdk_options.ts
+-rw-r--r--   0        0        0      992 2020-02-02 00:00:00.000000 vdk_jupyterlab_extension-0.1.940205024/style/base.css
+-rw-r--r--   0        0        0      108 2020-02-02 00:00:00.000000 vdk_jupyterlab_extension-0.1.940205024/style/index.css
+-rw-r--r--   0        0        0      104 2020-02-02 00:00:00.000000 vdk_jupyterlab_extension-0.1.940205024/style/index.js
+-rw-r--r--   0        0        0      865 2020-02-02 00:00:00.000000 vdk_jupyterlab_extension-0.1.940205024/style/vdkDialogs.css
+-rw-r--r--   0        0        0     7626 2020-02-02 00:00:00.000000 vdk_jupyterlab_extension-0.1.940205024/style/images/versatile-data-kit-logo.svg
+-rw-r--r--   0        0        0     3343 2020-02-02 00:00:00.000000 vdk_jupyterlab_extension-0.1.940205024/ui-tests/README.md
+-rw-r--r--   0        0        0      682 2020-02-02 00:00:00.000000 vdk_jupyterlab_extension-0.1.940205024/ui-tests/jupyter_server_test_config.py
+-rw-r--r--   0        0        0      350 2020-02-02 00:00:00.000000 vdk_jupyterlab_extension-0.1.940205024/ui-tests/package.json
+-rw-r--r--   0        0        0      425 2020-02-02 00:00:00.000000 vdk_jupyterlab_extension-0.1.940205024/ui-tests/playwright.config.js
+-rw-r--r--   0        0        0     4524 2020-02-02 00:00:00.000000 vdk_jupyterlab_extension-0.1.940205024/ui-tests/tests/vdk-jupyterlab-extension.spec.ts
+-rw-r--r--   0        0        0      891 2020-02-02 00:00:00.000000 vdk_jupyterlab_extension-0.1.940205024/vdk_jupyterlab_extension/__init__.py
+-rw-r--r--   0        0        0      179 2020-02-02 00:00:00.000000 vdk_jupyterlab_extension-0.1.940205024/vdk_jupyterlab_extension/_version.py
+-rw-r--r--   0        0        0     6936 2020-02-02 00:00:00.000000 vdk_jupyterlab_extension-0.1.940205024/vdk_jupyterlab_extension/handlers.py
+-rw-r--r--   0        0        0      724 2020-02-02 00:00:00.000000 vdk_jupyterlab_extension-0.1.940205024/vdk_jupyterlab_extension/job_data.py
+-rw-r--r--   0        0        0     8397 2020-02-02 00:00:00.000000 vdk_jupyterlab_extension-0.1.940205024/vdk_jupyterlab_extension/vdk_ui.py
+-rw-r--r--   0        0        0     2350 2020-02-02 00:00:00.000000 vdk_jupyterlab_extension-0.1.940205024/vdk_jupyterlab_extension/jupyter_sample_job/10_notebook.ipynb
+-rw-r--r--   0        0        0     1534 2020-02-02 00:00:00.000000 vdk_jupyterlab_extension-0.1.940205024/vdk_jupyterlab_extension/jupyter_sample_job/README.md
+-rw-r--r--   0        0        0     2850 2020-02-02 00:00:00.000000 vdk_jupyterlab_extension-0.1.940205024/vdk_jupyterlab_extension/jupyter_sample_job/config.ini
+-rw-r--r--   0        0        0      243 2020-02-02 00:00:00.000000 vdk_jupyterlab_extension-0.1.940205024/vdk_jupyterlab_extension/jupyter_sample_job/requirements.txt
+-rw-r--r--   0        0        0     5205 2020-02-02 00:00:00.000000 vdk_jupyterlab_extension-0.1.940205024/vdk_jupyterlab_extension/labextension/package.json
+-rw-r--r--   0        0        0     5649 2020-02-02 00:00:00.000000 vdk_jupyterlab_extension-0.1.940205024/vdk_jupyterlab_extension/labextension/schemas/vdk-jupyterlab-extension/package.json.orig
+-rw-r--r--   0        0        0      797 2020-02-02 00:00:00.000000 vdk_jupyterlab_extension-0.1.940205024/vdk_jupyterlab_extension/labextension/schemas/vdk-jupyterlab-extension/plugin.json
+-rw-r--r--   0        0        0    16736 2020-02-02 00:00:00.000000 vdk_jupyterlab_extension-0.1.940205024/vdk_jupyterlab_extension/labextension/static/161.d4f50a459898d1a8bc76.js
+-rw-r--r--   0        0        0     5454 2020-02-02 00:00:00.000000 vdk_jupyterlab_extension-0.1.940205024/vdk_jupyterlab_extension/labextension/static/747.e678254df7945f8ed34d.js
+-rw-r--r--   0        0        0     6841 2020-02-02 00:00:00.000000 vdk_jupyterlab_extension-0.1.940205024/vdk_jupyterlab_extension/labextension/static/remoteEntry.3b6333fd6a058bff7cf9.js
+-rw-r--r--   0        0        0      167 2020-02-02 00:00:00.000000 vdk_jupyterlab_extension-0.1.940205024/vdk_jupyterlab_extension/labextension/static/style.js
+-rw-r--r--   0        0        0     2452 2020-02-02 00:00:00.000000 vdk_jupyterlab_extension-0.1.940205024/vdk_jupyterlab_extension/labextension/static/third-party-licenses.json
+-rw-r--r--   0        0        0      127 2020-02-02 00:00:00.000000 vdk_jupyterlab_extension-0.1.940205024/vdk_jupyterlab_extension/tests/__init__.py
+-rw-r--r--   0        0        0      397 2020-02-02 00:00:00.000000 vdk_jupyterlab_extension-0.1.940205024/vdk_jupyterlab_extension/tests/test_handlers.py
+-rw-r--r--   0        0        0       73 2020-02-02 00:00:00.000000 vdk_jupyterlab_extension-0.1.940205024/vdk_jupyterlab_extension/vdk_options/__init__.py
+-rw-r--r--   0        0        0      332 2020-02-02 00:00:00.000000 vdk_jupyterlab_extension-0.1.940205024/vdk_jupyterlab_extension/vdk_options/vdk_options.py
+-rw-r--r--   0        0        0     1628 2020-02-02 00:00:00.000000 vdk_jupyterlab_extension-0.1.940205024/.gitignore
+-rw-r--r--   0        0        0       67 2020-02-02 00:00:00.000000 vdk_jupyterlab_extension-0.1.940205024/LICENSE
+-rw-r--r--   0        0        0     7167 2020-02-02 00:00:00.000000 vdk_jupyterlab_extension-0.1.940205024/README.md
+-rw-r--r--   0        0        0     2564 2020-02-02 00:00:00.000000 vdk_jupyterlab_extension-0.1.940205024/pyproject.toml
+-rw-r--r--   0        0        0     8775 2020-02-02 00:00:00.000000 vdk_jupyterlab_extension-0.1.940205024/PKG-INFO
```

### Comparing `vdk_jupyterlab_extension-0.1.936279136/.eslintrc.js` & `vdk_jupyterlab_extension-0.1.940205024/.eslintrc.js`

 * *Files identical despite different names*

### Comparing `vdk_jupyterlab_extension-0.1.936279136/jest.config.js` & `vdk_jupyterlab_extension-0.1.940205024/jest.config.js`

 * *Files identical despite different names*

### Comparing `vdk_jupyterlab_extension-0.1.936279136/package-lock.json` & `vdk_jupyterlab_extension-0.1.940205024/package-lock.json`

 * *Files identical despite different names*

### Comparing `vdk_jupyterlab_extension-0.1.936279136/package.json` & `vdk_jupyterlab_extension-0.1.940205024/package.json`

 * *Files 2% similar despite different names*

#### Pretty-printed

 * *Similarity: 0.9772727272727273%*

 * *Differences: {"'version'": "'0.1.940205024'"}*

```diff
@@ -145,9 +145,9 @@
     "sideEffects": [
         "style/*.css",
         "style/index.js"
     ],
     "style": "style/index.css",
     "styleModule": "style/index.js",
     "types": "lib/index.d.ts",
-    "version": "0.1.936279136"
+    "version": "0.1.940205024"
 }
```

### Comparing `vdk_jupyterlab_extension-0.1.936279136/tsconfig.json` & `vdk_jupyterlab_extension-0.1.940205024/tsconfig.json`

 * *Files identical despite different names*

### Comparing `vdk_jupyterlab_extension-0.1.936279136/yarn.lock` & `vdk_jupyterlab_extension-0.1.940205024/yarn.lock`

 * *Files 1% similar despite different names*

```diff
@@ -3304,17 +3304,17 @@
 
 camelcase@^6.0.0, camelcase@^6.2.0:
   version "6.3.0"
   resolved "https://registry.yarnpkg.com/camelcase/-/camelcase-6.3.0.tgz#5685b95eb209ac9c0c177467778c9c84df58ba9a"
   integrity sha512-Gmy6FhYlCY7uOElZUSbxo2UCDH8owEk996gkbrpsgGtrJLM3J7jGxl9Ic7Qwwj4ivOE5AWZWRMecDdF7hqGjFA==
 
 caniuse-lite@^1.0.30001503:
-  version "1.0.30001516"
-  resolved "https://registry.yarnpkg.com/caniuse-lite/-/caniuse-lite-1.0.30001516.tgz#621b1be7d85a8843ee7d210fd9d87b52e3daab3a"
-  integrity sha512-Wmec9pCBY8CWbmI4HsjBeQLqDTqV91nFVR83DnZpYyRnPI1wePDsTg0bGLPC5VU/3OIZV1fmxEea1b+tFKe86g==
+  version "1.0.30001517"
+  resolved "https://registry.yarnpkg.com/caniuse-lite/-/caniuse-lite-1.0.30001517.tgz#90fabae294215c3495807eb24fc809e11dc2f0a8"
+  integrity sha512-Vdhm5S11DaFVLlyiKu4hiUTkpZu+y1KA/rZZqVQfOD5YdDT/eQKlkt7NaE0WGOFgX32diqt9MiP9CAiFeRklaA==
 
 capture-exit@^2.0.0:
   version "2.0.0"
   resolved "https://registry.yarnpkg.com/capture-exit/-/capture-exit-2.0.0.tgz#fb953bfaebeb781f62898239dabb426d08a509a4"
   integrity sha512-PiT/hQmTonHhl/HFGN+Lx3JJUznrVYJ3+AQsnthneZbvW7x+f08Tk7yLJTLEOUvBTbduLeeBkxEaYXUOUrRq6g==
   dependencies:
     rsvp "^4.8.4"
@@ -3889,17 +3889,17 @@
   dependencies:
     chalk "^2.3.0"
     find-root "^1.0.0"
     lodash "^4.17.4"
     semver "^5.4.1"
 
 electron-to-chromium@^1.4.431:
-  version "1.4.464"
-  resolved "https://registry.yarnpkg.com/electron-to-chromium/-/electron-to-chromium-1.4.464.tgz#2f94bad78dff34e527aacbfc5d0b1a33cf046507"
-  integrity sha512-guZ84yoou4+ILNdj0XEbmGs6DEWj6zpVOWYpY09GU66yEb0DSYvP/biBPzHn0GuW/3RC/pnaYNUWlQE1fJYtgA==
+  version "1.4.467"
+  resolved "https://registry.yarnpkg.com/electron-to-chromium/-/electron-to-chromium-1.4.467.tgz#b0660bf644baff7eedea33b8c742fb53ec60e3c2"
+  integrity sha512-2qI70O+rR4poYeF2grcuS/bCps5KJh6y1jtZMDDEteyKJQrzLOEhFyXCLcHW6DTBjKjWkk26JhWoAi+Ux9A0fg==
 
 emittery@^0.7.1:
   version "0.7.2"
   resolved "https://registry.yarnpkg.com/emittery/-/emittery-0.7.2.tgz#25595908e13af0f5674ab419396e2fb394cdfa82"
   integrity sha512-A8OG5SR/ij3SsJdWDJdkkSYUjQdCUx6APQXem0SaEePBSRg4eymGYwBkKo1Y6DU+af/Jn2dBQqDBvjnr9Vi8nQ==
 
 emittery@^0.8.1:
@@ -7364,17 +7364,17 @@
 
 postcss-value-parser@^4.1.0, postcss-value-parser@^4.2.0:
   version "4.2.0"
   resolved "https://registry.yarnpkg.com/postcss-value-parser/-/postcss-value-parser-4.2.0.tgz#723c09920836ba6d3e5af019f92bc0971c02e514"
   integrity sha512-1NNCs6uurfkVbeXG4S8JFT9t19m45ICnif8zWLd5oPSZ50QnwMfK+H3jv408d4jw/7Bttv5axS5IiHoLaVNHeQ==
 
 postcss@^8.2.15, postcss@^8.3.11, postcss@^8.4.5:
-  version "8.4.26"
-  resolved "https://registry.yarnpkg.com/postcss/-/postcss-8.4.26.tgz#1bc62ab19f8e1e5463d98cf74af39702a00a9e94"
-  integrity sha512-jrXHFF8iTloAenySjM/ob3gSj7pCu0Ji49hnjqzsgSRa50hkWCKD0HQ+gMNJkW38jBI68MpAAg7ZWwHwX8NMMw==
+  version "8.4.27"
+  resolved "https://registry.yarnpkg.com/postcss/-/postcss-8.4.27.tgz#234d7e4b72e34ba5a92c29636734349e0d9c3057"
+  integrity sha512-gY/ACJtJPSmUFPDCHtX78+01fHa64FaU4zaaWfuh1MhGJISufJAH4cun6k/8fwsHYeK4UQmENQK+tRLCFJE8JQ==
   dependencies:
     nanoid "^3.3.6"
     picocolors "^1.0.0"
     source-map-js "^1.0.2"
 
 prelude-ls@^1.2.1:
   version "1.2.1"
@@ -8526,17 +8526,17 @@
     "@jridgewell/trace-mapping" "^0.3.17"
     jest-worker "^27.4.5"
     schema-utils "^3.1.1"
     serialize-javascript "^6.0.1"
     terser "^5.16.8"
 
 terser@^5.16.8, terser@^5.3.4:
-  version "5.19.1"
-  resolved "https://registry.yarnpkg.com/terser/-/terser-5.19.1.tgz#dbd7231f224a9e2401d0f0959542ed74d76d340b"
-  integrity sha512-27hxBUVdV6GoNg1pKQ7Z5cbR6V9txPVyBA+FQw3BaZ1Wuzvztce5p156DaP0NVZNrMZZ+6iG9Syf7WgMNKDg2Q==
+  version "5.19.2"
+  resolved "https://registry.yarnpkg.com/terser/-/terser-5.19.2.tgz#bdb8017a9a4a8de4663a7983f45c506534f9234e"
+  integrity sha512-qC5+dmecKJA4cpYxRa5aVkKehYsQKc+AHeKl0Oe62aYjBL8ZA33tTljktDHJSaxxMnbI5ZYw+o/S2DxxLu8OfA==
   dependencies:
     "@jridgewell/source-map" "^0.3.3"
     acorn "^8.8.2"
     commander "^2.20.0"
     source-map-support "~0.5.20"
 
 test-exclude@^6.0.0:
```

### Comparing `vdk_jupyterlab_extension-0.1.936279136/schema/plugin.json` & `vdk_jupyterlab_extension-0.1.940205024/schema/plugin.json`

 * *Files identical despite different names*

### Comparing `vdk_jupyterlab_extension-0.1.936279136/src/commandsAndMenu.tsx` & `vdk_jupyterlab_extension-0.1.940205024/src/commandsAndMenu.tsx`

 * *Files identical despite different names*

### Comparing `vdk_jupyterlab_extension-0.1.936279136/src/handler.ts` & `vdk_jupyterlab_extension-0.1.940205024/src/handler.ts`

 * *Files identical despite different names*

### Comparing `vdk_jupyterlab_extension-0.1.936279136/src/index.ts` & `vdk_jupyterlab_extension-0.1.940205024/src/index.ts`

 * *Files 12% similar despite different names*

```diff
@@ -13,14 +13,15 @@
 
 import { FileBrowserModel, IFileBrowserFactory } from '@jupyterlab/filebrowser';
 import { IChangedArgs } from '@jupyterlab/coreutils';
 import { INotebookTracker } from '@jupyterlab/notebook';
 import { trackVdkTags } from './vdkTags';
 import { IThemeManager } from '@jupyterlab/apputils';
 import { IDocumentManager } from '@jupyterlab/docmanager';
+import { initVDKConfigCell } from './initVDKConfigCell';
 
 /**
  * Current working directory in Jupyter
  * The variable can be accessed anywhere in the JupyterFrontEndPlugin
  */
 export let workingDirectory: string = '';
 
@@ -45,14 +46,18 @@
     themeManager: IThemeManager,
     docManager: IDocumentManager
   ) => {
     const { commands } = app;
 
     updateVDKMenu(commands, docManager);
 
+    notebookTracker.activeCellChanged.connect((sender, args) => {
+      initVDKConfigCell(notebookTracker);
+    });
+
     const fileBrowser = factory.defaultBrowser;
     fileBrowser.model.pathChanged.connect(onPathChanged);
     trackVdkTags(notebookTracker, themeManager);
   }
 };
 
 export default plugin;
```

### Comparing `vdk_jupyterlab_extension-0.1.936279136/src/jobData.ts` & `vdk_jupyterlab_extension-0.1.940205024/src/jobData.ts`

 * *Files identical despite different names*

### Comparing `vdk_jupyterlab_extension-0.1.936279136/src/serverRequests.ts` & `vdk_jupyterlab_extension-0.1.940205024/src/serverRequests.ts`

 * *Files identical despite different names*

### Comparing `vdk_jupyterlab_extension-0.1.936279136/src/vdkTags.ts` & `vdk_jupyterlab_extension-0.1.940205024/src/vdkTags.ts`

 * *Files identical despite different names*

### Comparing `vdk_jupyterlab_extension-0.1.936279136/src/__tests__/convert-job-to-notebook-component.spec.ts` & `vdk_jupyterlab_extension-0.1.940205024/src/__tests__/convert-job-to-notebook-component.spec.ts`

 * *Files identical despite different names*

### Comparing `vdk_jupyterlab_extension-0.1.936279136/src/__tests__/create-job-component.spec.ts` & `vdk_jupyterlab_extension-0.1.940205024/src/__tests__/create-job-component.spec.ts`

 * *Files identical despite different names*

### Comparing `vdk_jupyterlab_extension-0.1.936279136/src/__tests__/deploy-job-component.spec.ts` & `vdk_jupyterlab_extension-0.1.940205024/src/__tests__/deploy-job-component.spec.ts`

 * *Files identical despite different names*

### Comparing `vdk_jupyterlab_extension-0.1.936279136/src/__tests__/download-job-component.spec.ts` & `vdk_jupyterlab_extension-0.1.940205024/src/__tests__/download-job-component.spec.ts`

 * *Files identical despite different names*

### Comparing `vdk_jupyterlab_extension-0.1.936279136/src/__tests__/handler.spec.ts` & `vdk_jupyterlab_extension-0.1.940205024/src/__tests__/handler.spec.ts`

 * *Files identical despite different names*

### Comparing `vdk_jupyterlab_extension-0.1.936279136/src/__tests__/resquests.spec.ts` & `vdk_jupyterlab_extension-0.1.940205024/src/__tests__/resquests.spec.ts`

 * *Files identical despite different names*

### Comparing `vdk_jupyterlab_extension-0.1.936279136/src/__tests__/run-job-component.spec.tsx` & `vdk_jupyterlab_extension-0.1.940205024/src/__tests__/run-job-component.spec.tsx`

 * *Files identical despite different names*

### Comparing `vdk_jupyterlab_extension-0.1.936279136/src/__tests__/show-dialog.spec.tsx` & `vdk_jupyterlab_extension-0.1.940205024/src/__tests__/show-dialog.spec.tsx`

 * *Files identical despite different names*

### Comparing `vdk_jupyterlab_extension-0.1.936279136/src/__tests__/vdk-error-message.spec.ts` & `vdk_jupyterlab_extension-0.1.940205024/src/__tests__/vdk-error-message.spec.ts`

 * *Files identical despite different names*

### Comparing `vdk_jupyterlab_extension-0.1.936279136/src/__tests__/vdk-tags.spec.ts` & `vdk_jupyterlab_extension-0.1.940205024/src/__tests__/vdk-tags.spec.ts`

 * *Files identical despite different names*

### Comparing `vdk_jupyterlab_extension-0.1.936279136/src/components/ConvertJobToNotebook.tsx` & `vdk_jupyterlab_extension-0.1.940205024/src/components/ConvertJobToNotebook.tsx`

 * *Files identical despite different names*

### Comparing `vdk_jupyterlab_extension-0.1.936279136/src/components/CreateJob.tsx` & `vdk_jupyterlab_extension-0.1.940205024/src/components/CreateJob.tsx`

 * *Files identical despite different names*

### Comparing `vdk_jupyterlab_extension-0.1.936279136/src/components/DeployJob.tsx` & `vdk_jupyterlab_extension-0.1.940205024/src/components/DeployJob.tsx`

 * *Files identical despite different names*

### Comparing `vdk_jupyterlab_extension-0.1.936279136/src/components/DownloadJob.tsx` & `vdk_jupyterlab_extension-0.1.940205024/src/components/DownloadJob.tsx`

 * *Files identical despite different names*

### Comparing `vdk_jupyterlab_extension-0.1.936279136/src/components/RunJob.tsx` & `vdk_jupyterlab_extension-0.1.940205024/src/components/RunJob.tsx`

 * *Files identical despite different names*

### Comparing `vdk_jupyterlab_extension-0.1.936279136/src/components/VdkErrorMessage.ts` & `vdk_jupyterlab_extension-0.1.940205024/src/components/VdkErrorMessage.ts`

 * *Files identical despite different names*

### Comparing `vdk_jupyterlab_extension-0.1.936279136/src/components/VdkTextInput.tsx` & `vdk_jupyterlab_extension-0.1.940205024/src/components/VdkTextInput.tsx`

 * *Files identical despite different names*

### Comparing `vdk_jupyterlab_extension-0.1.936279136/style/base.css` & `vdk_jupyterlab_extension-0.1.940205024/style/base.css`

 * *Files identical despite different names*

### Comparing `vdk_jupyterlab_extension-0.1.936279136/style/vdkDialogs.css` & `vdk_jupyterlab_extension-0.1.940205024/style/vdkDialogs.css`

 * *Files identical despite different names*

### Comparing `vdk_jupyterlab_extension-0.1.936279136/style/images/versatile-data-kit-logo.svg` & `vdk_jupyterlab_extension-0.1.940205024/style/images/versatile-data-kit-logo.svg`

 * *Files identical despite different names*

### Comparing `vdk_jupyterlab_extension-0.1.936279136/ui-tests/README.md` & `vdk_jupyterlab_extension-0.1.940205024/ui-tests/README.md`

 * *Files identical despite different names*

### Comparing `vdk_jupyterlab_extension-0.1.936279136/ui-tests/jupyter_server_test_config.py` & `vdk_jupyterlab_extension-0.1.940205024/ui-tests/jupyter_server_test_config.py`

 * *Files identical despite different names*

### Comparing `vdk_jupyterlab_extension-0.1.936279136/ui-tests/tests/vdk-jupyterlab-extension.spec.ts` & `vdk_jupyterlab_extension-0.1.940205024/ui-tests/tests/vdk-jupyterlab-extension.spec.ts`

 * *Files 2% similar despite different names*

```diff
@@ -114,7 +114,17 @@
   await page.locator('div').filter({ hasText: 'Download Job' });
   await page.getByRole('button', { name: 'OK' }).click();
   await page.locator('div').filter({
     hasText: 'Encountered an error when trying to download the job. '
   });
   await page.getByRole('button', { name: 'OK' }).click();
 });
+
+test('should create an init cell when opening a new notebook', async ({
+  page
+}) => {
+  await page.goto('');
+  await page.locator('.jp-LauncherCard-icon').first().click();
+  await expect(
+    page.getByText(`job_input = VDK.get_initialized_job_input()`)
+  ).toBeVisible();
+});
```

### Comparing `vdk_jupyterlab_extension-0.1.936279136/vdk_jupyterlab_extension/__init__.py` & `vdk_jupyterlab_extension-0.1.940205024/vdk_jupyterlab_extension/__init__.py`

 * *Files identical despite different names*

### Comparing `vdk_jupyterlab_extension-0.1.936279136/vdk_jupyterlab_extension/handlers.py` & `vdk_jupyterlab_extension-0.1.940205024/vdk_jupyterlab_extension/handlers.py`

 * *Files identical despite different names*

### Comparing `vdk_jupyterlab_extension-0.1.936279136/vdk_jupyterlab_extension/job_data.py` & `vdk_jupyterlab_extension-0.1.940205024/vdk_jupyterlab_extension/job_data.py`

 * *Files identical despite different names*

### Comparing `vdk_jupyterlab_extension-0.1.936279136/vdk_jupyterlab_extension/vdk_ui.py` & `vdk_jupyterlab_extension-0.1.940205024/vdk_jupyterlab_extension/vdk_ui.py`

 * *Files identical despite different names*

### Comparing `vdk_jupyterlab_extension-0.1.936279136/vdk_jupyterlab_extension/jupyter_sample_job/10_notebook.ipynb` & `vdk_jupyterlab_extension-0.1.940205024/vdk_jupyterlab_extension/jupyter_sample_job/10_notebook.ipynb`

 * *Files identical despite different names*

### Comparing `vdk_jupyterlab_extension-0.1.936279136/vdk_jupyterlab_extension/jupyter_sample_job/README.md` & `vdk_jupyterlab_extension-0.1.940205024/vdk_jupyterlab_extension/jupyter_sample_job/README.md`

 * *Files identical despite different names*

### Comparing `vdk_jupyterlab_extension-0.1.936279136/vdk_jupyterlab_extension/jupyter_sample_job/config.ini` & `vdk_jupyterlab_extension-0.1.940205024/vdk_jupyterlab_extension/jupyter_sample_job/config.ini`

 * *Files identical despite different names*

### Comparing `vdk_jupyterlab_extension-0.1.936279136/vdk_jupyterlab_extension/labextension/package.json` & `vdk_jupyterlab_extension-0.1.940205024/vdk_jupyterlab_extension/labextension/package.json`

 * *Files 6% similar despite different names*

#### Pretty-printed

 * *Similarity: 0.9768939393939394%*

 * *Differences: {"'jupyterlab'": "{'_build': {'load': 'static/remoteEntry.3b6333fd6a058bff7cf9.js'}}",*

 * * "'version'": "'0.1.940205024'"}*

```diff
@@ -77,15 +77,15 @@
                 "jlpm clean:all"
             ]
         }
     },
     "jupyterlab": {
         "_build": {
             "extension": "./extension",
-            "load": "static/remoteEntry.77b468e1169ec9f71a16.js",
+            "load": "static/remoteEntry.3b6333fd6a058bff7cf9.js",
             "style": "./style"
         },
         "discovery": {
             "server": {
                 "base": {
                     "name": "vdk_jupyterlab_extension"
                 },
@@ -150,9 +150,9 @@
     "sideEffects": [
         "style/*.css",
         "style/index.js"
     ],
     "style": "style/index.css",
     "styleModule": "style/index.js",
     "types": "lib/index.d.ts",
-    "version": "0.1.936279136"
+    "version": "0.1.940205024"
 }
```

### Comparing `vdk_jupyterlab_extension-0.1.936279136/vdk_jupyterlab_extension/labextension/schemas/vdk-jupyterlab-extension/package.json.orig` & `vdk_jupyterlab_extension-0.1.940205024/vdk_jupyterlab_extension/labextension/schemas/vdk-jupyterlab-extension/package.json.orig`

 * *Files 2% similar despite different names*

#### Pretty-printed

 * *Similarity: 0.9772727272727273%*

 * *Differences: {"'version'": "'0.1.940205024'"}*

```diff
@@ -145,9 +145,9 @@
     "sideEffects": [
         "style/*.css",
         "style/index.js"
     ],
     "style": "style/index.css",
     "styleModule": "style/index.js",
     "types": "lib/index.d.ts",
-    "version": "0.1.936279136"
+    "version": "0.1.940205024"
 }
```

### Comparing `vdk_jupyterlab_extension-0.1.936279136/vdk_jupyterlab_extension/labextension/schemas/vdk-jupyterlab-extension/plugin.json` & `vdk_jupyterlab_extension-0.1.940205024/vdk_jupyterlab_extension/labextension/schemas/vdk-jupyterlab-extension/plugin.json`

 * *Files identical despite different names*

### Comparing `vdk_jupyterlab_extension-0.1.936279136/vdk_jupyterlab_extension/labextension/static/381.0485c5d1f906c39de85e.js` & `vdk_jupyterlab_extension-0.1.940205024/vdk_jupyterlab_extension/labextension/static/161.d4f50a459898d1a8bc76.js`

 * *Files 5% similar despite different names*

#### js-beautify {}

```diff
@@ -1,14 +1,14 @@
 "use strict";
 (self.webpackChunkvdk_jupyterlab_extension = self.webpackChunkvdk_jupyterlab_extension || []).push([
-    [381], {
-        381: (e, t, a) => {
+    [161], {
+        161: (e, t, a) => {
             a.r(t), a.d(t, {
-                default: () => q,
-                workingDirectory: () => V
+                default: () => Y,
+                workingDirectory: () => K
             });
             var n, o = a(38),
                 l = a(33),
                 s = a(271),
                 r = a.n(s);
             ! function(e) {
                 e.NAME = "jobName", e.TEAM = "jobTeam", e.PATH = "jobPath", e.CLOUD = "cloud", e.LOCAL = "local", e.ARGUMENTS = "jobArguments", e.DEPLOYMENT_REASON = "deploymentReason", e.DEPLOY_ENABLE = "enableDeploy"
@@ -101,26 +101,26 @@
                 } catch (e) {
                     return E(e), {
                         message: "",
                         status: !1
                     }
                 }
             }
-            async function k(e) {
+            async function y(e) {
                 if (await d(n.NAME) && await d(n.TEAM)) try {
                     const t = await b(e, {
                         body: JSON.stringify(u()),
                         method: "POST"
                     });
                     t.error ? await (0, l.showErrorMessage)("Encountered an error while trying the " + e + " operation. Error:", t.message, [l.Dialog.okButton()]) : alert(t.message)
                 } catch (e) {
                     E(e)
                 }
             }
-            class y {
+            class k {
                 constructor(e) {
                     this.exception_message = "", this.what_happened = "", this.why_it_happened = "", this.consequences = "", this.countermeasures = "", this.__parse_message(e)
                 }
                 __parse_message(e) {
                     const t = ["exception_message", "what_happened", "why_it_happened", "consequences", "countermeasures"],
                         a = ["ERROR : ", "WHAT HAPPENED :", "WHY IT HAPPENED :", "CONSEQUENCES :", "COUNTERMEASURES :"],
                         n = e.split("\n");
@@ -131,16 +131,16 @@
                             if (this[t[o]] = a[o] + n[l].substring(s + a[o].length), o++, o === t.length) break
                         } else this.exception_message = e
                     }
                 }
             }
             const w = "Convert Job To Notebook",
                 f = "Run Job",
-                N = "Create Deployment";
-            class j extends s.Component {
+                j = "Create Deployment";
+            class N extends s.Component {
                 constructor(e) {
                     super(e), this._onArgsChange = e => {
                         let t = e.currentTarget.value;
                         t && this._isJSON(t) && c.set(n.ARGUMENTS, t)
                     }, this._isJSON = e => {
                         try {
                             return JSON.parse(e), !0
@@ -170,15 +170,15 @@
                         className: "hidden"
                     }))
                 }
             }
             async function C(e) {
                 if ((await (0, l.showDialog)({
                         title: f,
-                        body: r().createElement(j, {
+                        body: r().createElement(N, {
                             jobPath: c.get(n.PATH)
                         }),
                         buttons: [l.Dialog.okButton(), l.Dialog.cancelButton()]
                     })).button.accept) {
                     let {
                         message: t,
                         status: a
@@ -190,15 +190,15 @@
                         }, r().createElement("p", {
                             className: "vdk-run-dialog-message"
                         }, "The job was executed successfully!")),
                         buttons: [l.Dialog.okButton()]
                     });
                     else {
                         t = "ERROR : " + t;
-                        const a = new y(t);
+                        const a = new k(t);
                         e && await P(a, e) || (0, l.showDialog)({
                             title: f,
                             body: r().createElement("div", {
                                 className: "vdk-run-error-message "
                             }, r().createElement("p", null, a.exception_message), r().createElement("p", null, a.what_happened), r().createElement("p", null, a.why_it_happened), r().createElement("p", null, a.consequences), r().createElement("p", null, a.countermeasures)),
                             buttons: [l.Dialog.okButton()]
                         })
@@ -330,37 +330,37 @@
                         const t = document.getElementById("enable");
                         (null == t ? void 0 : t.classList.contains("checked")) ? (t.classList.remove("checked"), c.set(n.DEPLOY_ENABLE, "")) : (null == t || t.classList.add("checked"), c.set(n.DEPLOY_ENABLE, "1"))
                     }
                 }
             }
             async function _() {
                 const e = await (0, l.showDialog)({
-                    title: N,
+                    title: j,
                     body: r().createElement(L, {
                         jobName: c.get(n.NAME),
                         jobPath: c.get(n.PATH),
                         jobTeam: c.get(n.TEAM)
                     }),
                     buttons: [l.Dialog.okButton(), l.Dialog.cancelButton()]
                 });
                 if (!e.value && e.button.accept) try {
                     if ((await (0, l.showDialog)({
-                            title: N,
+                            title: j,
                             body: "The job will be executed once before deployment.",
                             buttons: [l.Dialog.cancelButton({
                                 label: "Cancel"
                             }), l.Dialog.okButton({
                                 label: "Continue"
                             })]
                         })).button.accept) {
                         const {
                             message: e,
                             status: t
                         } = await v();
-                        t ? await d(n.DEPLOYMENT_REASON) && await k("deploy") : (0, l.showErrorMessage)("Encоuntered an error while running the job!", e, [l.Dialog.okButton()])
+                        t ? await d(n.DEPLOYMENT_REASON) && await y("deploy") : (0, l.showErrorMessage)("Encоuntered an error while running the job!", e, [l.Dialog.okButton()])
                     }
                 } catch (e) {
                     await (0, l.showErrorMessage)("Encountered an error when deploying the job. Error:", e, [l.Dialog.okButton()])
                 }
             }
             class x extends s.Component {
                 constructor(e) {
@@ -421,15 +421,15 @@
                     title: "Create Job",
                     body: r().createElement(x, {
                         jobPath: c.get(n.PATH),
                         jobName: c.get(n.NAME),
                         jobTeam: c.get(n.TEAM)
                     }),
                     buttons: [l.Dialog.okButton(), l.Dialog.cancelButton()]
-                })).button.accept && await k("create")
+                })).button.accept && await y("create")
             }
             class B extends s.Component {
                 constructor(e) {
                     super(e)
                 }
                 render() {
                     return r().createElement(r().Fragment, null, r().createElement(p, {
@@ -443,39 +443,39 @@
                     }), r().createElement(p, {
                         option: n.PATH,
                         value: this.props.jobPath,
                         label: "Path to job directory:"
                     }))
                 }
             }
-            async function M() {
+            async function S() {
                 (await (0, l.showDialog)({
                     title: "Download Job",
                     body: r().createElement(B, {
                         jobPath: c.get(n.PATH)
                     }),
                     buttons: [l.Dialog.okButton(), l.Dialog.cancelButton()]
-                })).button.accept && await k("download")
+                })).button.accept && await y("download")
             }
-            class S extends s.Component {
+            class M extends s.Component {
                 constructor(e) {
                     super(e)
                 }
                 render() {
                     return r().createElement(r().Fragment, null, r().createElement(p, {
                         option: n.PATH,
                         value: this.props.jobPath,
                         label: "Path to job directory:"
                     }))
                 }
             }
             async function J() {
                 if ((await (0, l.showDialog)({
                         title: w,
-                        body: r().createElement(S, {
+                        body: r().createElement(M, {
                             jobPath: c.get(n.PATH)
                         }),
                         buttons: [l.Dialog.okButton(), l.Dialog.cancelButton()]
                     })).button.accept && (await (0, l.showDialog)({
                         title: w,
                         body: r().createElement("p", null, "Are you sure you want to convert the Data Job with path:", " ", r().createElement("i", null, c.get(n.PATH)), " to notebook?"),
                         buttons: [l.Dialog.okButton(), l.Dialog.cancelButton()]
@@ -511,15 +511,15 @@
                         }, r().createElement("p", {
                             className: "vdk-convert-to-notebook-dialog-message"
                         }, "The Data Job with path ", r().createElement("i", null, c.get(n.PATH)), " was converted to notebook successfully!")),
                         buttons: [l.Dialog.okButton()]
                     });
                     else {
                         e = "ERROR : " + e;
-                        const t = new y(e);
+                        const t = new k(e);
                         await (0, l.showDialog)({
                             title: w,
                             body: r().createElement("div", {
                                 className: "vdk-convert-to-notebook-error-message "
                             }, r().createElement("p", null, t.exception_message), r().createElement("p", null, t.what_happened), r().createElement("p", null, t.why_it_happened), r().createElement("p", null, t.consequences), r().createElement("p", null, t.countermeasures)),
                             buttons: [l.Dialog.okButton()]
                         })
@@ -530,15 +530,15 @@
 
             function H(e, t, a, o, s, r) {
                 e.addCommand(t, {
                     label: a,
                     caption: o,
                     execute: async () => {
                         try {
-                            R ? (0, l.showErrorMessage)("Another VDK operation is currently running!", "Please wait until the operation ends!", [l.Dialog.okButton()]) : (R = !0, c.set(n.PATH, V), await async function() {
+                            R ? (0, l.showErrorMessage)("Another VDK operation is currently running!", "Please wait until the operation ends!", [l.Dialog.okButton()]) : (R = !0, c.set(n.PATH, K), await async function() {
                                 try {
                                     const e = await b("job", {
                                         body: JSON.stringify(JSON.stringify(u())),
                                         method: "POST"
                                     });
                                     e && (c.set(n.NAME, e[n.NAME]), c.set(n.TEAM, e[n.TEAM]), c.set(n.PATH, e[n.PATH]))
                                 } catch (e) {
@@ -557,27 +557,44 @@
                     const a = document.createElement("div");
                     a.innerText = String(e), t.classList.contains("jp-vdk-failing-cell") ? a.classList.add("jp-vdk-failing-cell-num") : a.classList.add("jp-vdk-cell-num"), t.appendChild(a)
                 },
                 W = e => {
                     const t = document.createElement("img");
                     t.setAttribute("src", "https://raw.githubusercontent.com/vmware/versatile-data-kit/dc15f7489f763a0e0e29370b2e06a714448fc234/support/images/versatile-data-kit-logo.svg"), t.setAttribute("width", "20"), t.setAttribute("height", "20"), t.classList.add("jp-vdk-logo"), e.appendChild(t)
                 };
-            var Y = a(986);
-            let V = "";
-            const q = {
+            var V = a(986);
+            let K = "";
+            const Y = {
                     id: "vdk-jupyterlab-extension:plugin",
                     autoStart: !0,
-                    optional: [o.ISettingRegistry, I.IFileBrowserFactory, F.INotebookTracker, l.IThemeManager, Y.IDocumentManager],
+                    optional: [o.ISettingRegistry, I.IFileBrowserFactory, F.INotebookTracker, l.IThemeManager, V.IDocumentManager],
                     activate: async (e, t, a, n, o, l) => {
                         const {
                             commands: s
                         } = e;
                         ! function(e, t) {
-                            H(e, "jp-vdk:menu-run", "Run", "Execute VDK Run Command", C, t), H(e, "jp-vdk:menu-create", "Create", "Execute VDK Create Command", O), H(e, "jp-vdk:menu-download", "Download", "Execute VDK Download Command", M), H(e, "jp-vdk:menu-convert-job-to-notebook", "Convert Job To Notebook", "Convert Data Job To Jupyter Notebook", J), H(e, "jp-vdk:menu-create-deployment", "Deploy", "Create deployment of a VDK job", _)
-                        }(s, l), a.defaultBrowser.model.pathChanged.connect(K), ((e, t) => {
+                            H(e, "jp-vdk:menu-run", "Run", "Execute VDK Run Command", C, t), H(e, "jp-vdk:menu-create", "Create", "Execute VDK Create Command", O), H(e, "jp-vdk:menu-download", "Download", "Execute VDK Download Command", S), H(e, "jp-vdk:menu-convert-job-to-notebook", "Convert Job To Notebook", "Convert Data Job To Jupyter Notebook", J), H(e, "jp-vdk:menu-create-deployment", "Deploy", "Create deployment of a VDK job", _)
+                        }(s, l), n.activeCellChanged.connect(((e, t) => {
+                            ! function(e) {
+                                var t, a, n, o;
+                                const l = e.currentWidget;
+                                if (l) {
+                                    const s = null === (a = null === (t = l.content.model) || void 0 === t ? void 0 : t.contentFactory) || void 0 === a ? void 0 : a.createCodeCell({
+                                            cell: {
+                                                cell_type: "code",
+                                                source: ['"""\n', "vdk_ipython extension introduces a magic command for Jupyter.\n", "The command enables the user to load VDK for the current notebook.\n", "VDK provides the job_input API, which has methods for:\n", "    * executing queries to an OLAP database;\n", "    * ingesting data into a database;\n", "    * processing data into a database.\n", "See the IJobInput documentation for more details.\n", "https://github.com/vmware/versatile-data-kit/blob/main/projects/vdk-core/src/vdk/api/job_input.py\n", "Please refrain from tagging this cell with VDK as it is not an actual part of the data job\n", "and is only used for development purposes.\n", '"""\n', "%reload_ext vdk_ipython\n", "%reload_VDK\n", "job_input = VDK.get_initialized_job_input()"],
+                                                metadata: {}
+                                            }
+                                        }),
+                                        r = null === (o = null === (n = e.currentWidget) || void 0 === n ? void 0 : n.content.model) || void 0 === o ? void 0 : o.cells,
+                                        c = null == r ? void 0 : r.get(0).value.text;
+                                    r && s && r.length <= 1 && "" == c && (r.insert(0, s), r.remove(1))
+                                }
+                            }(n)
+                        })), a.defaultBrowser.model.pathChanged.connect(q), ((e, t) => {
                             const a = async () => {
                                 if (e.currentWidget && e.currentWidget.model && 0 !== e.currentWidget.model.cells.length) {
                                     let a = [],
                                         n = 0;
                                     for (; e.currentWidget && e.currentWidget.model && e.currentWidget.model.cells.get(n);) {
                                         const t = e.currentWidget.model.cells.get(n).metadata.get("tags");
                                         t && t.includes("vdk") && a.push(n), n++
@@ -608,13 +625,13 @@
                                     })(Array.from(e.activeCell.parent.node.children), a, t, e.activeCell.node)
                                 }
                             };
                             e.activeCellChanged.connect(a), t.themeChanged.connect(a)
                         })(n, o)
                     }
                 },
-                K = async (e, t) => {
-                    V = t.newValue
+                q = async (e, t) => {
+                    K = t.newValue
                 }
         }
     }
 ]);
```

### Comparing `vdk_jupyterlab_extension-0.1.936279136/vdk_jupyterlab_extension/labextension/static/747.e678254df7945f8ed34d.js` & `vdk_jupyterlab_extension-0.1.940205024/vdk_jupyterlab_extension/labextension/static/747.e678254df7945f8ed34d.js`

 * *Files identical despite different names*

### Comparing `vdk_jupyterlab_extension-0.1.936279136/vdk_jupyterlab_extension/labextension/static/remoteEntry.77b468e1169ec9f71a16.js` & `vdk_jupyterlab_extension-0.1.940205024/vdk_jupyterlab_extension/labextension/static/remoteEntry.3b6333fd6a058bff7cf9.js`

 * *Files 6% similar despite different names*

#### js-beautify {}

```diff
@@ -1,15 +1,15 @@
 var _JUPYTERLAB;
 (() => {
     "use strict";
-    var e, r, t, n, o, a, i, u, l, s, f, d, p, c, h, v, b = {
+    var e, r, t, n, o, a, i, u, l, f, d, s, p, c, h, v, b = {
             913: (e, r, t) => {
                 var n = {
-                        "./index": () => t.e(381).then((() => () => t(381))),
-                        "./extension": () => t.e(381).then((() => () => t(381))),
+                        "./index": () => t.e(161).then((() => () => t(161))),
+                        "./extension": () => t.e(161).then((() => () => t(161))),
                         "./style": () => t.e(747).then((() => () => t(747)))
                     },
                     o = (e, r) => (t.R = r, r = t.o(n, e) ? n[e]() : Promise.resolve().then((() => {
                         throw new Error('Module "' + e + '" does not exist in container.')
                     })), t.R = void 0, r),
                     a = (e, r) => {
                         if (t.S) {
@@ -43,49 +43,49 @@
         }), r
     }, y.d = (e, r) => {
         for (var t in r) y.o(r, t) && !y.o(e, t) && Object.defineProperty(e, t, {
             enumerable: !0,
             get: r[t]
         })
     }, y.f = {}, y.e = e => Promise.all(Object.keys(y.f).reduce(((r, t) => (y.f[t](e, r), r)), [])), y.u = e => e + "." + {
-        381: "0485c5d1f906c39de85e",
+        161: "d4f50a459898d1a8bc76",
         747: "e678254df7945f8ed34d"
     } [e] + ".js?v=" + {
-        381: "0485c5d1f906c39de85e",
+        161: "d4f50a459898d1a8bc76",
         747: "e678254df7945f8ed34d"
     } [e], y.g = function() {
         if ("object" == typeof globalThis) return globalThis;
         try {
             return this || new Function("return this")()
         } catch (e) {
             if ("object" == typeof window) return window
         }
     }(), y.o = (e, r) => Object.prototype.hasOwnProperty.call(e, r), e = {}, r = "vdk-jupyterlab-extension:", y.l = (t, n, o, a) => {
         if (e[t]) e[t].push(n);
         else {
             var i, u;
             if (void 0 !== o)
-                for (var l = document.getElementsByTagName("script"), s = 0; s < l.length; s++) {
-                    var f = l[s];
-                    if (f.getAttribute("src") == t || f.getAttribute("data-webpack") == r + o) {
-                        i = f;
+                for (var l = document.getElementsByTagName("script"), f = 0; f < l.length; f++) {
+                    var d = l[f];
+                    if (d.getAttribute("src") == t || d.getAttribute("data-webpack") == r + o) {
+                        i = d;
                         break
                     }
                 }
             i || (u = !0, (i = document.createElement("script")).charset = "utf-8", i.timeout = 120, y.nc && i.setAttribute("nonce", y.nc), i.setAttribute("data-webpack", r + o), i.src = t), e[t] = [n];
-            var d = (r, n) => {
+            var s = (r, n) => {
                     i.onerror = i.onload = null, clearTimeout(p);
                     var o = e[t];
                     if (delete e[t], i.parentNode && i.parentNode.removeChild(i), o && o.forEach((e => e(n))), r) return r(n)
                 },
-                p = setTimeout(d.bind(null, void 0, {
+                p = setTimeout(s.bind(null, void 0, {
                     type: "timeout",
                     target: i
                 }), 12e4);
-            i.onerror = d.bind(null, i.onerror), i.onload = d.bind(null, i.onload), u && document.head.appendChild(i)
+            i.onerror = s.bind(null, i.onerror), i.onload = s.bind(null, i.onload), u && document.head.appendChild(i)
         }
     }, y.r = e => {
         "undefined" != typeof Symbol && Symbol.toStringTag && Object.defineProperty(e, Symbol.toStringTag, {
             value: "Module"
         }), Object.defineProperty(e, "__esModule", {
             value: !0
         })
@@ -102,19 +102,19 @@
                 var a = y.S[t],
                     i = "vdk-jupyterlab-extension",
                     u = [];
                 return "default" === t && ((e, r, t, n) => {
                     var o = a[e] = a[e] || {},
                         u = o[r];
                     (!u || !u.loaded && (1 != !u.eager ? n : i > u.from)) && (o[r] = {
-                        get: () => y.e(381).then((() => () => y(381))),
+                        get: () => y.e(161).then((() => () => y(161))),
                         from: i,
                         eager: !1
                     })
-                })("vdk-jupyterlab-extension", "0.1.936279136"), e[t] = u.length ? Promise.all(u).then((() => e[t] = 1)) : 1
+                })("vdk-jupyterlab-extension", "0.1.940205024"), e[t] = u.length ? Promise.all(u).then((() => e[t] = 1)) : 1
             }
         }
     })(), (() => {
         var e;
         y.g.importScripts && (e = y.g.location + "");
         var r = y.g.document;
         if (!e && r && (r.currentScript && (e = r.currentScript.src), !e)) {
@@ -164,33 +164,33 @@
     }, a = (e, r) => {
         if (0 in e) {
             r = t(r);
             var n = e[0],
                 o = n < 0;
             o && (n = -n - 1);
             for (var i = 0, u = 1, l = !0;; u++, i++) {
-                var s, f, d = u < e.length ? (typeof e[u])[0] : "";
-                if (i >= r.length || "o" == (f = (typeof(s = r[i]))[0])) return !l || ("u" == d ? u > n && !o : "" == d != o);
-                if ("u" == f) {
-                    if (!l || "u" != d) return !1
+                var f, d, s = u < e.length ? (typeof e[u])[0] : "";
+                if (i >= r.length || "o" == (d = (typeof(f = r[i]))[0])) return !l || ("u" == s ? u > n && !o : "" == s != o);
+                if ("u" == d) {
+                    if (!l || "u" != s) return !1
                 } else if (l)
-                    if (d == f)
+                    if (s == d)
                         if (u <= n) {
-                            if (s != e[u]) return !1
+                            if (f != e[u]) return !1
                         } else {
-                            if (o ? s > e[u] : s < e[u]) return !1;
-                            s != e[u] && (l = !1)
+                            if (o ? f > e[u] : f < e[u]) return !1;
+                            f != e[u] && (l = !1)
                         }
-                else if ("s" != d && "n" != d) {
+                else if ("s" != s && "n" != s) {
                     if (o || u <= n) return !1;
                     l = !1, u--
                 } else {
-                    if (u <= n || f < d != o) return !1;
+                    if (u <= n || d < s != o) return !1;
                     l = !1
-                } else "s" != d && "n" != d && (l = !1, u--)
+                } else "s" != s && "n" != s && (l = !1, u--)
             }
         }
         var p = [],
             c = p.pop.bind(p);
         for (i = 1; i < e.length; i++) {
             var h = e[i];
             p.push(1 == h ? c() | c() : 2 == h ? c() & c() : h ? a(h, r) : !c())
@@ -199,33 +199,33 @@
     }, i = (e, r) => {
         var t = y.S[e];
         if (!t || !y.o(t, r)) throw new Error("Shared module " + r + " doesn't exist in shared scope " + e);
         return t
     }, u = (e, r) => {
         var t = e[r];
         return Object.keys(t).reduce(((e, r) => !e || !t[e].loaded && n(e, r) ? r : e), 0)
-    }, l = (e, r, t, n) => "Unsatisfied version " + t + " from " + (t && e[r][t].from) + " of shared singleton module " + r + " (required " + o(n) + ")", s = (e, r, t, n) => {
+    }, l = (e, r, t, n) => "Unsatisfied version " + t + " from " + (t && e[r][t].from) + " of shared singleton module " + r + " (required " + o(n) + ")", f = (e, r, t, n) => {
         var o = u(e, t);
-        return a(n, o) || f(l(e, t, o, n)), d(e[t][o])
-    }, f = e => {
+        return a(n, o) || d(l(e, t, o, n)), s(e[t][o])
+    }, d = e => {
         "undefined" != typeof console && console.warn && console.warn(e)
-    }, d = e => (e.loaded = 1, e.get()), p = (e => function(r, t, n, o) {
+    }, s = e => (e.loaded = 1, e.get()), p = (e => function(r, t, n, o) {
         var a = y.I(r);
         return a && a.then ? a.then(e.bind(e, r, y.S[r], t, n, o)) : e(r, y.S[r], t, n)
-    })(((e, r, t, n) => (i(e, t), s(r, 0, t, n)))), c = {}, h = {
+    })(((e, r, t, n) => (i(e, t), f(r, 0, t, n)))), c = {}, h = {
         33: () => p("default", "@jupyterlab/apputils", [1, 3, 6, 3]),
         38: () => p("default", "@jupyterlab/settingregistry", [1, 3, 6, 3]),
         123: () => p("default", "@jupyterlab/notebook", [1, 3, 6, 3]),
         142: () => p("default", "@jupyterlab/coreutils", [1, 5, 6, 3]),
         271: () => p("default", "react", [1, 17, 0, 1]),
         280: () => p("default", "@jupyterlab/filebrowser", [1, 3, 6, 3]),
         820: () => p("default", "@jupyterlab/services", [1, 6, 6, 3]),
         986: () => p("default", "@jupyterlab/docmanager", [1, 3, 6, 3])
     }, v = {
-        381: [33, 38, 123, 142, 271, 280, 820, 986]
+        161: [33, 38, 123, 142, 271, 280, 820, 986]
     }, y.f.consumes = (e, r) => {
         y.o(v, e) && v[e].forEach((e => {
             if (y.o(c, e)) return r.push(c[e]);
             var t = r => {
                     c[e] = 0, y.m[e] = t => {
                         delete y.c[e], t.exports = r()
                     }
```

### Comparing `vdk_jupyterlab_extension-0.1.936279136/vdk_jupyterlab_extension/labextension/static/third-party-licenses.json` & `vdk_jupyterlab_extension-0.1.940205024/vdk_jupyterlab_extension/labextension/static/third-party-licenses.json`

 * *Files identical despite different names*

### Comparing `vdk_jupyterlab_extension-0.1.936279136/.gitignore` & `vdk_jupyterlab_extension-0.1.940205024/.gitignore`

 * *Files identical despite different names*

### Comparing `vdk_jupyterlab_extension-0.1.936279136/README.md` & `vdk_jupyterlab_extension-0.1.940205024/README.md`

 * *Files identical despite different names*

### Comparing `vdk_jupyterlab_extension-0.1.936279136/pyproject.toml` & `vdk_jupyterlab_extension-0.1.940205024/pyproject.toml`

 * *Files identical despite different names*

### Comparing `vdk_jupyterlab_extension-0.1.936279136/PKG-INFO` & `vdk_jupyterlab_extension-0.1.940205024/PKG-INFO`

 * *Files 0% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: vdk-jupyterlab-extension
-Version: 0.1.936279136
+Version: 0.1.940205024
 Summary: A Jupyterlab extension for using VDK
 Project-URL: Homepage, https://github.com/vmware/versatile-data-kit
 Project-URL: Bug Tracker, https://github.com/vmware/versatile-data-kit/issues
 Project-URL: Repository, https://github.com/vmware/versatile-data-kit
 Author-email: Versatile Data Kit Development Team <versatile-data-kit@vmware.com>
 License: See https://github.com/vmware/versatile-data-kit/blob/main/LICENSE
 License-File: LICENSE
```

