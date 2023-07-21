# Comparing `tmp/rer.newsletter-2.0.0a2.tar.gz` & `tmp/rer.newsletter-2.0.0a3.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "rer.newsletter-2.0.0a2.tar", last modified: Thu Mar 16 14:37:27 2023, max compression
+gzip compressed data, was "rer.newsletter-2.0.0a3.tar", last modified: Fri Jul 21 13:50:05 2023, max compression
```

## Comparing `rer.newsletter-2.0.0a2.tar` & `rer.newsletter-2.0.0a3.tar`

### file list

```diff
@@ -1,214 +1,215 @@
-drwxr-xr-x   0 pieronicolli   (501) staff       (20)        0 2023-03-16 14:37:27.055803 rer.newsletter-2.0.0a2/
--rw-r--r--   0 pieronicolli   (501) staff       (20)     3868 2023-03-16 14:37:25.000000 rer.newsletter-2.0.0a2/CHANGES.rst
--rw-r--r--   0 pieronicolli   (501) staff       (20)       91 2023-03-16 14:37:25.000000 rer.newsletter-2.0.0a2/CONTRIBUTORS.rst
--rw-r--r--   0 pieronicolli   (501) staff       (20)    18092 2023-03-16 14:37:25.000000 rer.newsletter-2.0.0a2/LICENSE.GPL
--rw-r--r--   0 pieronicolli   (501) staff       (20)      658 2023-03-16 14:37:25.000000 rer.newsletter-2.0.0a2/LICENSE.rst
--rw-r--r--   0 pieronicolli   (501) staff       (20)      152 2023-03-16 14:37:25.000000 rer.newsletter-2.0.0a2/MANIFEST.in
--rw-r--r--   0 pieronicolli   (501) staff       (20)     9441 2023-03-16 14:37:27.055889 rer.newsletter-2.0.0a2/PKG-INFO
--rw-r--r--   0 pieronicolli   (501) staff       (20)     4554 2023-03-16 14:37:25.000000 rer.newsletter-2.0.0a2/README.rst
--rw-r--r--   0 pieronicolli   (501) staff       (20)       27 2023-03-16 14:37:25.000000 rer.newsletter-2.0.0a2/constraints.txt
--rw-r--r--   0 pieronicolli   (501) staff       (20)      105 2023-03-16 14:37:25.000000 rer.newsletter-2.0.0a2/constraints_plone51.txt
--rw-r--r--   0 pieronicolli   (501) staff       (20)      105 2023-03-16 14:37:25.000000 rer.newsletter-2.0.0a2/constraints_plone52.txt
--rw-r--r--   0 pieronicolli   (501) staff       (20)      105 2023-03-16 14:37:25.000000 rer.newsletter-2.0.0a2/constraints_plone60.txt
-drwxr-xr-x   0 pieronicolli   (501) staff       (20)        0 2023-03-16 14:37:27.036795 rer.newsletter-2.0.0a2/docs/
--rw-r--r--   0 pieronicolli   (501) staff       (20)       77 2023-03-16 14:37:25.000000 rer.newsletter-2.0.0a2/docs/index.rst
--rw-r--r--   0 pieronicolli   (501) staff       (20)    32560 2023-03-16 14:37:25.000000 rer.newsletter-2.0.0a2/docs/rer-logo.png
--rw-r--r--   0 pieronicolli   (501) staff       (20)       50 2023-03-16 14:37:25.000000 rer.newsletter-2.0.0a2/requirements.txt
--rw-r--r--   0 pieronicolli   (501) staff       (20)      270 2023-03-16 14:37:27.056218 rer.newsletter-2.0.0a2/setup.cfg
--rw-r--r--   0 pieronicolli   (501) staff       (20)     2391 2023-03-16 14:37:25.000000 rer.newsletter-2.0.0a2/setup.py
-drwxr-xr-x   0 pieronicolli   (501) staff       (20)        0 2023-03-16 14:37:27.032965 rer.newsletter-2.0.0a2/src/
-drwxr-xr-x   0 pieronicolli   (501) staff       (20)        0 2023-03-16 14:37:27.036920 rer.newsletter-2.0.0a2/src/rer/
--rw-r--r--   0 pieronicolli   (501) staff       (20)       80 2023-03-16 14:37:25.000000 rer.newsletter-2.0.0a2/src/rer/__init__.py
-drwxr-xr-x   0 pieronicolli   (501) staff       (20)        0 2023-03-16 14:37:27.038915 rer.newsletter-2.0.0a2/src/rer/newsletter/
--rw-r--r--   0 pieronicolli   (501) staff       (20)      184 2023-03-16 14:37:25.000000 rer.newsletter-2.0.0a2/src/rer/newsletter/__init__.py
-drwxr-xr-x   0 pieronicolli   (501) staff       (20)        0 2023-03-16 14:37:27.039333 rer.newsletter-2.0.0a2/src/rer/newsletter/adapter/
--rw-r--r--   0 pieronicolli   (501) staff       (20)        0 2023-03-16 14:37:25.000000 rer.newsletter-2.0.0a2/src/rer/newsletter/adapter/__init__.py
--rw-r--r--   0 pieronicolli   (501) staff       (20)      648 2023-03-16 14:37:25.000000 rer.newsletter-2.0.0a2/src/rer/newsletter/adapter/configure.zcml
--rw-r--r--   0 pieronicolli   (501) staff       (20)     7952 2023-03-16 14:37:25.000000 rer.newsletter-2.0.0a2/src/rer/newsletter/adapter/sender.py
--rw-r--r--   0 pieronicolli   (501) staff       (20)     8353 2023-03-16 14:37:25.000000 rer.newsletter-2.0.0a2/src/rer/newsletter/adapter/subscriptions.py
-drwxr-xr-x   0 pieronicolli   (501) staff       (20)        0 2023-03-16 14:37:27.039648 rer.newsletter-2.0.0a2/src/rer/newsletter/behaviors/
--rw-r--r--   0 pieronicolli   (501) staff       (20)        0 2023-03-16 14:37:25.000000 rer.newsletter-2.0.0a2/src/rer/newsletter/behaviors/__init__.py
--rw-r--r--   0 pieronicolli   (501) staff       (20)      441 2023-03-16 14:37:25.000000 rer.newsletter-2.0.0a2/src/rer/newsletter/behaviors/configure.zcml
--rw-r--r--   0 pieronicolli   (501) staff       (20)      970 2023-03-16 14:37:25.000000 rer.newsletter-2.0.0a2/src/rer/newsletter/behaviors/ships.py
-drwxr-xr-x   0 pieronicolli   (501) staff       (20)        0 2023-03-16 14:37:27.039988 rer.newsletter-2.0.0a2/src/rer/newsletter/browser/
--rw-r--r--   0 pieronicolli   (501) staff       (20)        0 2023-03-16 14:37:25.000000 rer.newsletter-2.0.0a2/src/rer/newsletter/browser/__init__.py
-drwxr-xr-x   0 pieronicolli   (501) staff       (20)        0 2023-03-16 14:37:27.042314 rer.newsletter-2.0.0a2/src/rer/newsletter/browser/channel/
--rw-r--r--   0 pieronicolli   (501) staff       (20)        0 2023-03-16 14:37:25.000000 rer.newsletter-2.0.0a2/src/rer/newsletter/browser/channel/__init__.py
--rw-r--r--   0 pieronicolli   (501) staff       (20)     1686 2023-03-16 14:37:25.000000 rer.newsletter-2.0.0a2/src/rer/newsletter/browser/channel/add.py
--rw-r--r--   0 pieronicolli   (501) staff       (20)     1372 2023-03-16 14:37:25.000000 rer.newsletter-2.0.0a2/src/rer/newsletter/browser/channel/channelhistory.py
--rw-r--r--   0 pieronicolli   (501) staff       (20)      708 2023-03-16 14:37:25.000000 rer.newsletter-2.0.0a2/src/rer/newsletter/browser/channel/channelview.py
--rw-r--r--   0 pieronicolli   (501) staff       (20)      383 2023-03-16 14:37:25.000000 rer.newsletter-2.0.0a2/src/rer/newsletter/browser/channel/channelviewlet.py
--rw-r--r--   0 pieronicolli   (501) staff       (20)     5308 2023-03-16 14:37:25.000000 rer.newsletter-2.0.0a2/src/rer/newsletter/browser/channel/configure.zcml
--rw-r--r--   0 pieronicolli   (501) staff       (20)     2208 2023-03-16 14:37:25.000000 rer.newsletter-2.0.0a2/src/rer/newsletter/browser/channel/deleteexpiredusers.py
--rw-r--r--   0 pieronicolli   (501) staff       (20)     3177 2023-03-16 14:37:25.000000 rer.newsletter-2.0.0a2/src/rer/newsletter/browser/channel/manageusers.py
--rw-r--r--   0 pieronicolli   (501) staff       (20)     5321 2023-03-16 14:37:25.000000 rer.newsletter-2.0.0a2/src/rer/newsletter/browser/channel/subscribe.py
-drwxr-xr-x   0 pieronicolli   (501) staff       (20)        0 2023-03-16 14:37:27.043096 rer.newsletter-2.0.0a2/src/rer/newsletter/browser/channel/templates/
--rw-r--r--   0 pieronicolli   (501) staff       (20)     1607 2023-03-16 14:37:25.000000 rer.newsletter-2.0.0a2/src/rer/newsletter/browser/channel/templates/channelhistoryview.pt
--rw-r--r--   0 pieronicolli   (501) staff       (20)     2608 2023-03-16 14:37:25.000000 rer.newsletter-2.0.0a2/src/rer/newsletter/browser/channel/templates/channelview.pt
--rw-r--r--   0 pieronicolli   (501) staff       (20)      787 2023-03-16 14:37:25.000000 rer.newsletter-2.0.0a2/src/rer/newsletter/browser/channel/templates/channelviewlet.pt
--rw-r--r--   0 pieronicolli   (501) staff       (20)      885 2023-03-16 14:37:25.000000 rer.newsletter-2.0.0a2/src/rer/newsletter/browser/channel/templates/confirm_subscription.pt
-drwxr-xr-x   0 pieronicolli   (501) staff       (20)        0 2023-03-16 14:37:27.043864 rer.newsletter-2.0.0a2/src/rer/newsletter/browser/channel/templates/mail_templates/
--rw-r--r--   0 pieronicolli   (501) staff       (20)      851 2023-03-16 14:37:25.000000 rer.newsletter-2.0.0a2/src/rer/newsletter/browser/channel/templates/mail_templates/active_user.pt
--rw-r--r--   0 pieronicolli   (501) staff       (20)      568 2023-03-16 14:37:25.000000 rer.newsletter-2.0.0a2/src/rer/newsletter/browser/channel/templates/mail_templates/active_user_confirm.pt
--rw-r--r--   0 pieronicolli   (501) staff       (20)      603 2023-03-16 14:37:25.000000 rer.newsletter-2.0.0a2/src/rer/newsletter/browser/channel/templates/mail_templates/asynch_send_fail.pt
--rw-r--r--   0 pieronicolli   (501) staff       (20)      728 2023-03-16 14:37:25.000000 rer.newsletter-2.0.0a2/src/rer/newsletter/browser/channel/templates/mail_templates/asynch_send_success.pt
--rw-r--r--   0 pieronicolli   (501) staff       (20)      571 2023-03-16 14:37:25.000000 rer.newsletter-2.0.0a2/src/rer/newsletter/browser/channel/templates/mail_templates/delete_user.pt
--rw-r--r--   0 pieronicolli   (501) staff       (20)      611 2023-03-16 14:37:25.000000 rer.newsletter-2.0.0a2/src/rer/newsletter/browser/channel/templates/mail_templates/delete_user_confirm.pt
--rw-r--r--   0 pieronicolli   (501) staff       (20)      592 2023-03-16 14:37:25.000000 rer.newsletter-2.0.0a2/src/rer/newsletter/browser/channel/templates/mail_templates/unsubscribe_channel.pt
--rw-r--r--   0 pieronicolli   (501) staff       (20)     3072 2023-03-16 14:37:25.000000 rer.newsletter-2.0.0a2/src/rer/newsletter/browser/channel/templates/manageusers.pt
--rw-r--r--   0 pieronicolli   (501) staff       (20)     1685 2023-03-16 14:37:25.000000 rer.newsletter-2.0.0a2/src/rer/newsletter/browser/channel/templates/subscribechannel.pt
--rw-r--r--   0 pieronicolli   (501) staff       (20)     1080 2023-03-16 14:37:25.000000 rer.newsletter-2.0.0a2/src/rer/newsletter/browser/channel/templates/unsubscribechannel.pt
--rw-r--r--   0 pieronicolli   (501) staff       (20)     4430 2023-03-16 14:37:25.000000 rer.newsletter-2.0.0a2/src/rer/newsletter/browser/channel/unsubscribe.py
-drwxr-xr-x   0 pieronicolli   (501) staff       (20)        0 2023-03-16 14:37:27.044268 rer.newsletter-2.0.0a2/src/rer/newsletter/browser/channel/users/
--rw-r--r--   0 pieronicolli   (501) staff       (20)        0 2023-03-16 14:37:25.000000 rer.newsletter-2.0.0a2/src/rer/newsletter/browser/channel/users/__init__.py
--rw-r--r--   0 pieronicolli   (501) staff       (20)     1828 2023-03-16 14:37:25.000000 rer.newsletter-2.0.0a2/src/rer/newsletter/browser/channel/users/add.py
--rw-r--r--   0 pieronicolli   (501) staff       (20)     3892 2023-03-16 14:37:25.000000 rer.newsletter-2.0.0a2/src/rer/newsletter/browser/channel/users/confirm_subscription.py
--rw-r--r--   0 pieronicolli   (501) staff       (20)     5980 2023-03-16 14:37:25.000000 rer.newsletter-2.0.0a2/src/rer/newsletter/browser/channel/users/usersimport.py
--rw-r--r--   0 pieronicolli   (501) staff       (20)      907 2023-03-16 14:37:25.000000 rer.newsletter-2.0.0a2/src/rer/newsletter/browser/configure.zcml
-drwxr-xr-x   0 pieronicolli   (501) staff       (20)        0 2023-03-16 14:37:27.045413 rer.newsletter-2.0.0a2/src/rer/newsletter/browser/message/
--rw-r--r--   0 pieronicolli   (501) staff       (20)        0 2023-03-16 14:37:25.000000 rer.newsletter-2.0.0a2/src/rer/newsletter/browser/message/__init__.py
--rw-r--r--   0 pieronicolli   (501) staff       (20)      525 2023-03-16 14:37:25.000000 rer.newsletter-2.0.0a2/src/rer/newsletter/browser/message/checkmessageview.py
--rw-r--r--   0 pieronicolli   (501) staff       (20)      442 2023-03-16 14:37:25.000000 rer.newsletter-2.0.0a2/src/rer/newsletter/browser/message/collectionview.py
--rw-r--r--   0 pieronicolli   (501) staff       (20)     2969 2023-03-16 14:37:25.000000 rer.newsletter-2.0.0a2/src/rer/newsletter/browser/message/configure.zcml
--rw-r--r--   0 pieronicolli   (501) staff       (20)     2603 2023-03-16 14:37:25.000000 rer.newsletter-2.0.0a2/src/rer/newsletter/browser/message/messagepreview.py
--rw-r--r--   0 pieronicolli   (501) staff       (20)      174 2023-03-16 14:37:25.000000 rer.newsletter-2.0.0a2/src/rer/newsletter/browser/message/messageview.py
--rw-r--r--   0 pieronicolli   (501) staff       (20)     1543 2023-03-16 14:37:25.000000 rer.newsletter-2.0.0a2/src/rer/newsletter/browser/message/messageviewlet.py
--rw-r--r--   0 pieronicolli   (501) staff       (20)     5408 2023-03-16 14:37:25.000000 rer.newsletter-2.0.0a2/src/rer/newsletter/browser/message/sendingtest.py
--rw-r--r--   0 pieronicolli   (501) staff       (20)     3057 2023-03-16 14:37:25.000000 rer.newsletter-2.0.0a2/src/rer/newsletter/browser/message/sendmessageview.py
--rw-r--r--   0 pieronicolli   (501) staff       (20)      288 2023-03-16 14:37:25.000000 rer.newsletter-2.0.0a2/src/rer/newsletter/browser/message/shippablecollection.py
-drwxr-xr-x   0 pieronicolli   (501) staff       (20)        0 2023-03-16 14:37:27.046144 rer.newsletter-2.0.0a2/src/rer/newsletter/browser/message/templates/
--rw-r--r--   0 pieronicolli   (501) staff       (20)     2687 2023-03-16 14:37:25.000000 rer.newsletter-2.0.0a2/src/rer/newsletter/browser/message/templates/collection_sending_view.pt
--rw-r--r--   0 pieronicolli   (501) staff       (20)      870 2023-03-16 14:37:25.000000 rer.newsletter-2.0.0a2/src/rer/newsletter/browser/message/templates/messagecontentcore.pt
--rw-r--r--   0 pieronicolli   (501) staff       (20)     1532 2023-03-16 14:37:25.000000 rer.newsletter-2.0.0a2/src/rer/newsletter/browser/message/templates/messagepreview.pt
--rw-r--r--   0 pieronicolli   (501) staff       (20)      952 2023-03-16 14:37:25.000000 rer.newsletter-2.0.0a2/src/rer/newsletter/browser/message/templates/messageview.pt
--rw-r--r--   0 pieronicolli   (501) staff       (20)     1542 2023-03-16 14:37:25.000000 rer.newsletter-2.0.0a2/src/rer/newsletter/browser/message/templates/messageviewlet.pt
--rw-r--r--   0 pieronicolli   (501) staff       (20)     1132 2023-03-16 14:37:25.000000 rer.newsletter-2.0.0a2/src/rer/newsletter/browser/message/templates/sendingtest.pt
--rw-r--r--   0 pieronicolli   (501) staff       (20)     1451 2023-03-16 14:37:25.000000 rer.newsletter-2.0.0a2/src/rer/newsletter/browser/message/templates/sendmessageview.pt
--rw-r--r--   0 pieronicolli   (501) staff       (20)      570 2023-03-16 14:37:25.000000 rer.newsletter-2.0.0a2/src/rer/newsletter/browser/message/versionview.py
-drwxr-xr-x   0 pieronicolli   (501) staff       (20)        0 2023-03-16 14:37:27.046254 rer.newsletter-2.0.0a2/src/rer/newsletter/browser/overrides/
--rw-r--r--   0 pieronicolli   (501) staff       (20)        0 2023-03-16 14:37:25.000000 rer.newsletter-2.0.0a2/src/rer/newsletter/browser/overrides/.gitkeep
--rw-r--r--   0 pieronicolli   (501) staff       (20)     1465 2023-03-16 14:37:25.000000 rer.newsletter-2.0.0a2/src/rer/newsletter/browser/settings.py
-drwxr-xr-x   0 pieronicolli   (501) staff       (20)        0 2023-03-16 14:37:27.046527 rer.newsletter-2.0.0a2/src/rer/newsletter/browser/static/
--rw-r--r--   0 pieronicolli   (501) staff       (20)        0 2023-03-16 14:37:25.000000 rer.newsletter-2.0.0a2/src/rer/newsletter/browser/static/.gitkeep
-drwxr-xr-x   0 pieronicolli   (501) staff       (20)        0 2023-03-16 14:37:27.046631 rer.newsletter-2.0.0a2/src/rer/newsletter/browser/static/DataTables-1.10.16/
--rw-r--r--   0 pieronicolli   (501) staff       (20)     6148 2023-03-16 14:37:25.000000 rer.newsletter-2.0.0a2/src/rer/newsletter/browser/static/DataTables-1.10.16/.DS_Store
-drwxr-xr-x   0 pieronicolli   (501) staff       (20)        0 2023-03-16 14:37:27.047165 rer.newsletter-2.0.0a2/src/rer/newsletter/browser/static/DataTables-1.10.16/images/
--rwxr-xr-x   0 pieronicolli   (501) staff       (20)      160 2023-03-16 14:37:25.000000 rer.newsletter-2.0.0a2/src/rer/newsletter/browser/static/DataTables-1.10.16/images/sort_asc.png
--rwxr-xr-x   0 pieronicolli   (501) staff       (20)      148 2023-03-16 14:37:25.000000 rer.newsletter-2.0.0a2/src/rer/newsletter/browser/static/DataTables-1.10.16/images/sort_asc_disabled.png
--rwxr-xr-x   0 pieronicolli   (501) staff       (20)      201 2023-03-16 14:37:25.000000 rer.newsletter-2.0.0a2/src/rer/newsletter/browser/static/DataTables-1.10.16/images/sort_both.png
--rwxr-xr-x   0 pieronicolli   (501) staff       (20)      158 2023-03-16 14:37:25.000000 rer.newsletter-2.0.0a2/src/rer/newsletter/browser/static/DataTables-1.10.16/images/sort_desc.png
--rwxr-xr-x   0 pieronicolli   (501) staff       (20)      146 2023-03-16 14:37:25.000000 rer.newsletter-2.0.0a2/src/rer/newsletter/browser/static/DataTables-1.10.16/images/sort_desc_disabled.png
--rw-r--r--   0 pieronicolli   (501) staff       (20)     1436 2023-03-16 14:37:25.000000 rer.newsletter-2.0.0a2/src/rer/newsletter/browser/static/custom.css
--rw-r--r--   0 pieronicolli   (501) staff       (20)    16203 2023-03-16 14:37:25.000000 rer.newsletter-2.0.0a2/src/rer/newsletter/browser/static/datatables.css
-drwxr-xr-x   0 pieronicolli   (501) staff       (20)        0 2023-03-16 14:37:27.047888 rer.newsletter-2.0.0a2/src/rer/newsletter/browser/static/scripts/
--rw-r--r--   0 pieronicolli   (501) staff       (20)     2707 2023-03-16 14:37:25.000000 rer.newsletter-2.0.0a2/src/rer/newsletter/browser/static/scripts/channelhistory.js
--rwxr-xr-x   0 pieronicolli   (501) staff       (20)   443959 2023-03-16 14:37:25.000000 rer.newsletter-2.0.0a2/src/rer/newsletter/browser/static/scripts/datatables.js
--rw-r--r--   0 pieronicolli   (501) staff       (20)     4087 2023-03-16 14:37:25.000000 rer.newsletter-2.0.0a2/src/rer/newsletter/browser/static/scripts/initializedModal.js
--rw-r--r--   0 pieronicolli   (501) staff       (20)     4000 2023-03-16 14:37:25.000000 rer.newsletter-2.0.0a2/src/rer/newsletter/browser/static/scripts/manageusers.js
--rw-r--r--   0 pieronicolli   (501) staff       (20)     2216 2023-03-16 14:37:25.000000 rer.newsletter-2.0.0a2/src/rer/newsletter/configure.zcml
-drwxr-xr-x   0 pieronicolli   (501) staff       (20)        0 2023-03-16 14:37:27.048304 rer.newsletter-2.0.0a2/src/rer/newsletter/content/
--rw-r--r--   0 pieronicolli   (501) staff       (20)        0 2023-03-16 14:37:25.000000 rer.newsletter-2.0.0a2/src/rer/newsletter/content/__init__.py
--rw-r--r--   0 pieronicolli   (501) staff       (20)      217 2023-03-16 14:37:25.000000 rer.newsletter-2.0.0a2/src/rer/newsletter/content/channel.py
--rw-r--r--   0 pieronicolli   (501) staff       (20)      217 2023-03-16 14:37:25.000000 rer.newsletter-2.0.0a2/src/rer/newsletter/content/message.py
--rw-r--r--   0 pieronicolli   (501) staff       (20)      261 2023-03-16 14:37:25.000000 rer.newsletter-2.0.0a2/src/rer/newsletter/content/shippable_collection.py
-drwxr-xr-x   0 pieronicolli   (501) staff       (20)        0 2023-03-16 14:37:27.049165 rer.newsletter-2.0.0a2/src/rer/newsletter/contentrules/
--rw-r--r--   0 pieronicolli   (501) staff       (20)       24 2023-03-16 14:37:25.000000 rer.newsletter-2.0.0a2/src/rer/newsletter/contentrules/__init__.py
--rw-r--r--   0 pieronicolli   (501) staff       (20)      871 2023-03-16 14:37:25.000000 rer.newsletter-2.0.0a2/src/rer/newsletter/contentrules/actions.py
--rw-r--r--   0 pieronicolli   (501) staff       (20)     3229 2023-03-16 14:37:25.000000 rer.newsletter-2.0.0a2/src/rer/newsletter/contentrules/configure.zcml
--rw-r--r--   0 pieronicolli   (501) staff       (20)      955 2023-03-16 14:37:25.000000 rer.newsletter-2.0.0a2/src/rer/newsletter/contentrules/events.py
--rw-r--r--   0 pieronicolli   (501) staff       (20)     2092 2023-03-16 14:37:25.000000 rer.newsletter-2.0.0a2/src/rer/newsletter/contentrules/executors.py
--rw-r--r--   0 pieronicolli   (501) staff       (20)     1907 2023-03-16 14:37:25.000000 rer.newsletter-2.0.0a2/src/rer/newsletter/contentrules/forms.py
--rw-r--r--   0 pieronicolli   (501) staff       (20)      216 2023-03-16 14:37:25.000000 rer.newsletter-2.0.0a2/src/rer/newsletter/contentrules/handlers.py
--rw-r--r--   0 pieronicolli   (501) staff       (20)     1376 2023-03-16 14:37:25.000000 rer.newsletter-2.0.0a2/src/rer/newsletter/contentrules/interfaces.py
-drwxr-xr-x   0 pieronicolli   (501) staff       (20)        0 2023-03-16 14:37:27.049358 rer.newsletter-2.0.0a2/src/rer/newsletter/exceptions/
--rw-r--r--   0 pieronicolli   (501) staff       (20)        0 2023-03-16 14:37:25.000000 rer.newsletter-2.0.0a2/src/rer/newsletter/exceptions/__init__.py
--rw-r--r--   0 pieronicolli   (501) staff       (20)      132 2023-03-16 14:37:25.000000 rer.newsletter-2.0.0a2/src/rer/newsletter/exceptions/exceptions.py
--rw-r--r--   0 pieronicolli   (501) staff       (20)     3577 2023-03-16 14:37:25.000000 rer.newsletter-2.0.0a2/src/rer/newsletter/interfaces.py
-drwxr-xr-x   0 pieronicolli   (501) staff       (20)        0 2023-03-16 14:37:27.049673 rer.newsletter-2.0.0a2/src/rer/newsletter/locales/
-drwxr-xr-x   0 pieronicolli   (501) staff       (20)        0 2023-03-16 14:37:27.034283 rer.newsletter-2.0.0a2/src/rer/newsletter/locales/it/
-drwxr-xr-x   0 pieronicolli   (501) staff       (20)        0 2023-03-16 14:37:27.049776 rer.newsletter-2.0.0a2/src/rer/newsletter/locales/it/LC_MESSAGES/
--rw-r--r--   0 pieronicolli   (501) staff       (20)    17392 2023-03-16 14:37:25.000000 rer.newsletter-2.0.0a2/src/rer/newsletter/locales/it/LC_MESSAGES/rer.newsletter.po
--rw-r--r--   0 pieronicolli   (501) staff       (20)    14638 2023-03-16 14:37:25.000000 rer.newsletter-2.0.0a2/src/rer/newsletter/locales/rer.newsletter.pot
--rw-r--r--   0 pieronicolli   (501) staff       (20)     1569 2023-03-16 14:37:25.000000 rer.newsletter-2.0.0a2/src/rer/newsletter/locales/update.py
--rwxr-xr-x   0 pieronicolli   (501) staff       (20)      503 2023-03-16 14:37:25.000000 rer.newsletter-2.0.0a2/src/rer/newsletter/locales/update.sh
-drwxr-xr-x   0 pieronicolli   (501) staff       (20)        0 2023-03-16 14:37:27.050334 rer.newsletter-2.0.0a2/src/rer/newsletter/portlets/
--rw-r--r--   0 pieronicolli   (501) staff       (20)        0 2023-03-16 14:37:25.000000 rer.newsletter-2.0.0a2/src/rer/newsletter/portlets/__init__.py
--rw-r--r--   0 pieronicolli   (501) staff       (20)      573 2023-03-16 14:37:25.000000 rer.newsletter-2.0.0a2/src/rer/newsletter/portlets/configure.zcml
--rw-r--r--   0 pieronicolli   (501) staff       (20)     1695 2023-03-16 14:37:25.000000 rer.newsletter-2.0.0a2/src/rer/newsletter/portlets/interface.py
--rw-r--r--   0 pieronicolli   (501) staff       (20)      873 2023-03-16 14:37:25.000000 rer.newsletter-2.0.0a2/src/rer/newsletter/portlets/subscribe.pt
--rw-r--r--   0 pieronicolli   (501) staff       (20)     1912 2023-03-16 14:37:25.000000 rer.newsletter-2.0.0a2/src/rer/newsletter/portlets/subscribe.py
-drwxr-xr-x   0 pieronicolli   (501) staff       (20)        0 2023-03-16 14:37:27.034749 rer.newsletter-2.0.0a2/src/rer/newsletter/profiles/
-drwxr-xr-x   0 pieronicolli   (501) staff       (20)        0 2023-03-16 14:37:27.051990 rer.newsletter-2.0.0a2/src/rer/newsletter/profiles/default/
--rw-r--r--   0 pieronicolli   (501) staff       (20)      178 2023-03-16 14:37:25.000000 rer.newsletter-2.0.0a2/src/rer/newsletter/profiles/default/actions.xml
--rw-r--r--   0 pieronicolli   (501) staff       (20)      161 2023-03-16 14:37:25.000000 rer.newsletter-2.0.0a2/src/rer/newsletter/profiles/default/browserlayer.xml
--rw-r--r--   0 pieronicolli   (501) staff       (20)      275 2023-03-16 14:37:25.000000 rer.newsletter-2.0.0a2/src/rer/newsletter/profiles/default/catalog.xml
--rw-r--r--   0 pieronicolli   (501) staff       (20)      570 2023-03-16 14:37:25.000000 rer.newsletter-2.0.0a2/src/rer/newsletter/profiles/default/controlpanel.xml
--rw-r--r--   0 pieronicolli   (501) staff       (20)      373 2023-03-16 14:37:25.000000 rer.newsletter-2.0.0a2/src/rer/newsletter/profiles/default/diff_tool.xml
--rw-r--r--   0 pieronicolli   (501) staff       (20)      184 2023-03-16 14:37:25.000000 rer.newsletter-2.0.0a2/src/rer/newsletter/profiles/default/metadata.xml
--rw-r--r--   0 pieronicolli   (501) staff       (20)      280 2023-03-16 14:37:25.000000 rer.newsletter-2.0.0a2/src/rer/newsletter/profiles/default/portlets.xml
--rw-r--r--   0 pieronicolli   (501) staff       (20)     3209 2023-03-16 14:37:25.000000 rer.newsletter-2.0.0a2/src/rer/newsletter/profiles/default/registry.xml
--rw-r--r--   0 pieronicolli   (501) staff       (20)      365 2023-03-16 14:37:25.000000 rer.newsletter-2.0.0a2/src/rer/newsletter/profiles/default/repositorytool.xml
--rw-r--r--   0 pieronicolli   (501) staff       (20)     1350 2023-03-16 14:37:25.000000 rer.newsletter-2.0.0a2/src/rer/newsletter/profiles/default/rolemap.xml
--rw-r--r--   0 pieronicolli   (501) staff       (20)      252 2023-03-16 14:37:25.000000 rer.newsletter-2.0.0a2/src/rer/newsletter/profiles/default/sharing.xml
-drwxr-xr-x   0 pieronicolli   (501) staff       (20)        0 2023-03-16 14:37:27.052318 rer.newsletter-2.0.0a2/src/rer/newsletter/profiles/default/types/
--rw-r--r--   0 pieronicolli   (501) staff       (20)     2961 2023-03-16 14:37:25.000000 rer.newsletter-2.0.0a2/src/rer/newsletter/profiles/default/types/Channel.xml
--rw-r--r--   0 pieronicolli   (501) staff       (20)     3036 2023-03-16 14:37:25.000000 rer.newsletter-2.0.0a2/src/rer/newsletter/profiles/default/types/Message.xml
--rw-r--r--   0 pieronicolli   (501) staff       (20)     3345 2023-03-16 14:37:25.000000 rer.newsletter-2.0.0a2/src/rer/newsletter/profiles/default/types/Shippable_Collection.xml
--rw-r--r--   0 pieronicolli   (501) staff       (20)      327 2023-03-16 14:37:25.000000 rer.newsletter-2.0.0a2/src/rer/newsletter/profiles/default/types.xml
-drwxr-xr-x   0 pieronicolli   (501) staff       (20)        0 2023-03-16 14:37:27.034688 rer.newsletter-2.0.0a2/src/rer/newsletter/profiles/default/workflows/
-drwxr-xr-x   0 pieronicolli   (501) staff       (20)        0 2023-03-16 14:37:27.052427 rer.newsletter-2.0.0a2/src/rer/newsletter/profiles/default/workflows/channel_workflow/
--rw-r--r--   0 pieronicolli   (501) staff       (20)     8132 2023-03-16 14:37:25.000000 rer.newsletter-2.0.0a2/src/rer/newsletter/profiles/default/workflows/channel_workflow/definition.xml
-drwxr-xr-x   0 pieronicolli   (501) staff       (20)        0 2023-03-16 14:37:27.052537 rer.newsletter-2.0.0a2/src/rer/newsletter/profiles/default/workflows/message_workflow/
--rw-r--r--   0 pieronicolli   (501) staff       (20)     9923 2023-03-16 14:37:25.000000 rer.newsletter-2.0.0a2/src/rer/newsletter/profiles/default/workflows/message_workflow/definition.xml
--rw-r--r--   0 pieronicolli   (501) staff       (20)      643 2023-03-16 14:37:25.000000 rer.newsletter-2.0.0a2/src/rer/newsletter/profiles/default/workflows.xml
-drwxr-xr-x   0 pieronicolli   (501) staff       (20)        0 2023-03-16 14:37:27.053074 rer.newsletter-2.0.0a2/src/rer/newsletter/profiles/uninstall/
--rw-r--r--   0 pieronicolli   (501) staff       (20)      824 2023-03-16 14:37:25.000000 rer.newsletter-2.0.0a2/src/rer/newsletter/profiles/uninstall/actions.xml
--rw-r--r--   0 pieronicolli   (501) staff       (20)      117 2023-03-16 14:37:25.000000 rer.newsletter-2.0.0a2/src/rer/newsletter/profiles/uninstall/browserlayer.xml
--rw-r--r--   0 pieronicolli   (501) staff       (20)      321 2023-03-16 14:37:25.000000 rer.newsletter-2.0.0a2/src/rer/newsletter/profiles/uninstall/controlpanel.xml
--rw-r--r--   0 pieronicolli   (501) staff       (20)      701 2023-03-16 14:37:25.000000 rer.newsletter-2.0.0a2/src/rer/newsletter/profiles/uninstall/registry.xml
--rw-r--r--   0 pieronicolli   (501) staff       (20)      296 2023-03-16 14:37:25.000000 rer.newsletter-2.0.0a2/src/rer/newsletter/profiles/uninstall/types.xml
--rw-r--r--   0 pieronicolli   (501) staff       (20)       30 2023-03-16 14:37:25.000000 rer.newsletter-2.0.0a2/src/rer/newsletter/pyproject.toml
-drwxr-xr-x   0 pieronicolli   (501) staff       (20)        0 2023-03-16 14:37:27.053603 rer.newsletter-2.0.0a2/src/rer/newsletter/queue/
--rw-r--r--   0 pieronicolli   (501) staff       (20)       24 2023-03-16 14:37:25.000000 rer.newsletter-2.0.0a2/src/rer/newsletter/queue/__init__.py
--rw-r--r--   0 pieronicolli   (501) staff       (20)      487 2023-03-16 14:37:25.000000 rer.newsletter-2.0.0a2/src/rer/newsletter/queue/configure.zcml
--rw-r--r--   0 pieronicolli   (501) staff       (20)      643 2023-03-16 14:37:25.000000 rer.newsletter-2.0.0a2/src/rer/newsletter/queue/handler.py
--rw-r--r--   0 pieronicolli   (501) staff       (20)      360 2023-03-16 14:37:25.000000 rer.newsletter-2.0.0a2/src/rer/newsletter/queue/interfaces.py
--rw-r--r--   0 pieronicolli   (501) staff       (20)     5050 2023-03-16 14:37:25.000000 rer.newsletter-2.0.0a2/src/rer/newsletter/queue/view.py
-drwxr-xr-x   0 pieronicolli   (501) staff       (20)        0 2023-03-16 14:37:27.053811 rer.newsletter-2.0.0a2/src/rer/newsletter/restapi/
--rw-r--r--   0 pieronicolli   (501) staff       (20)        0 2023-03-16 14:37:25.000000 rer.newsletter-2.0.0a2/src/rer/newsletter/restapi/__init__.py
--rw-r--r--   0 pieronicolli   (501) staff       (20)      240 2023-03-16 14:37:25.000000 rer.newsletter-2.0.0a2/src/rer/newsletter/restapi/configure.zcml
-drwxr-xr-x   0 pieronicolli   (501) staff       (20)        0 2023-03-16 14:37:27.054377 rer.newsletter-2.0.0a2/src/rer/newsletter/restapi/services/
--rw-r--r--   0 pieronicolli   (501) staff       (20)        0 2023-03-16 14:37:25.000000 rer.newsletter-2.0.0a2/src/rer/newsletter/restapi/services/__init__.py
--rw-r--r--   0 pieronicolli   (501) staff       (20)      784 2023-03-16 14:37:25.000000 rer.newsletter-2.0.0a2/src/rer/newsletter/restapi/services/configure.zcml
--rw-r--r--   0 pieronicolli   (501) staff       (20)     3875 2023-03-16 14:37:25.000000 rer.newsletter-2.0.0a2/src/rer/newsletter/restapi/services/confirm_subscription.py
--rw-r--r--   0 pieronicolli   (501) staff       (20)     3821 2023-03-16 14:37:25.000000 rer.newsletter-2.0.0a2/src/rer/newsletter/restapi/services/subscribe.py
--rw-r--r--   0 pieronicolli   (501) staff       (20)     3497 2023-03-16 14:37:25.000000 rer.newsletter-2.0.0a2/src/rer/newsletter/restapi/services/unsubscribe.py
--rw-r--r--   0 pieronicolli   (501) staff       (20)     1220 2023-03-16 14:37:25.000000 rer.newsletter-2.0.0a2/src/rer/newsletter/setuphandlers.py
--rw-r--r--   0 pieronicolli   (501) staff       (20)     1174 2023-03-16 14:37:25.000000 rer.newsletter-2.0.0a2/src/rer/newsletter/testing.py
-drwxr-xr-x   0 pieronicolli   (501) staff       (20)        0 2023-03-16 14:37:27.054850 rer.newsletter-2.0.0a2/src/rer/newsletter/tests/
--rw-r--r--   0 pieronicolli   (501) staff       (20)        0 2023-03-16 14:37:25.000000 rer.newsletter-2.0.0a2/src/rer/newsletter/tests/__init__.py
--rw-r--r--   0 pieronicolli   (501) staff       (20)     3009 2023-03-16 14:37:25.000000 rer.newsletter-2.0.0a2/src/rer/newsletter/tests/test_setup.py
--rw-r--r--   0 pieronicolli   (501) staff       (20)     2102 2023-03-16 14:37:25.000000 rer.newsletter-2.0.0a2/src/rer/newsletter/tests/test_subscription_tile.py
--rw-r--r--   0 pieronicolli   (501) staff       (20)     9313 2023-03-16 14:37:25.000000 rer.newsletter-2.0.0a2/src/rer/newsletter/tests/test_subscriptions_adapter.py
-drwxr-xr-x   0 pieronicolli   (501) staff       (20)        0 2023-03-16 14:37:27.055362 rer.newsletter-2.0.0a2/src/rer/newsletter/tiles/
--rw-r--r--   0 pieronicolli   (501) staff       (20)        0 2023-03-16 14:37:25.000000 rer.newsletter-2.0.0a2/src/rer/newsletter/tiles/__init__.py
--rw-r--r--   0 pieronicolli   (501) staff       (20)      635 2023-03-16 14:37:25.000000 rer.newsletter-2.0.0a2/src/rer/newsletter/tiles/configure.zcml
--rw-r--r--   0 pieronicolli   (501) staff       (20)     1250 2023-03-16 14:37:25.000000 rer.newsletter-2.0.0a2/src/rer/newsletter/tiles/subscribe.pt
--rw-r--r--   0 pieronicolli   (501) staff       (20)     1104 2023-03-16 14:37:25.000000 rer.newsletter-2.0.0a2/src/rer/newsletter/tiles/subscribe.py
-drwxr-xr-x   0 pieronicolli   (501) staff       (20)        0 2023-03-16 14:37:27.055696 rer.newsletter-2.0.0a2/src/rer/newsletter/transforms/
--rw-r--r--   0 pieronicolli   (501) staff       (20)        0 2023-03-16 14:37:25.000000 rer.newsletter-2.0.0a2/src/rer/newsletter/transforms/__init__.py
--rw-r--r--   0 pieronicolli   (501) staff       (20)     2037 2023-03-16 14:37:25.000000 rer.newsletter-2.0.0a2/src/rer/newsletter/transforms/link_transform.py
--rw-r--r--   0 pieronicolli   (501) staff       (20)      206 2023-03-16 14:37:25.000000 rer.newsletter-2.0.0a2/src/rer/newsletter/transforms/mimetype.py
--rw-r--r--   0 pieronicolli   (501) staff       (20)     3154 2023-03-16 14:37:25.000000 rer.newsletter-2.0.0a2/src/rer/newsletter/upgrades.py
--rw-r--r--   0 pieronicolli   (501) staff       (20)     1101 2023-03-16 14:37:25.000000 rer.newsletter-2.0.0a2/src/rer/newsletter/upgrades.zcml
--rw-r--r--   0 pieronicolli   (501) staff       (20)     1309 2023-03-16 14:37:25.000000 rer.newsletter-2.0.0a2/src/rer/newsletter/utils.py
--rw-r--r--   0 pieronicolli   (501) staff       (20)      864 2023-03-16 14:37:25.000000 rer.newsletter-2.0.0a2/src/rer/newsletter/vocabularies.py
-drwxr-xr-x   0 pieronicolli   (501) staff       (20)        0 2023-03-16 14:37:27.037826 rer.newsletter-2.0.0a2/src/rer.newsletter.egg-info/
--rw-r--r--   0 pieronicolli   (501) staff       (20)     9441 2023-03-16 14:37:26.000000 rer.newsletter-2.0.0a2/src/rer.newsletter.egg-info/PKG-INFO
--rw-r--r--   0 pieronicolli   (501) staff       (20)     8170 2023-03-16 14:37:26.000000 rer.newsletter-2.0.0a2/src/rer.newsletter.egg-info/SOURCES.txt
--rw-r--r--   0 pieronicolli   (501) staff       (20)        1 2023-03-16 14:37:26.000000 rer.newsletter-2.0.0a2/src/rer.newsletter.egg-info/dependency_links.txt
--rw-r--r--   0 pieronicolli   (501) staff       (20)      119 2023-03-16 14:37:26.000000 rer.newsletter-2.0.0a2/src/rer.newsletter.egg-info/entry_points.txt
--rw-r--r--   0 pieronicolli   (501) staff       (20)        4 2023-03-16 14:37:26.000000 rer.newsletter-2.0.0a2/src/rer.newsletter.egg-info/namespace_packages.txt
--rw-r--r--   0 pieronicolli   (501) staff       (20)        1 2023-03-16 14:37:26.000000 rer.newsletter-2.0.0a2/src/rer.newsletter.egg-info/not-zip-safe
--rw-r--r--   0 pieronicolli   (501) staff       (20)      292 2023-03-16 14:37:26.000000 rer.newsletter-2.0.0a2/src/rer.newsletter.egg-info/requires.txt
--rw-r--r--   0 pieronicolli   (501) staff       (20)        4 2023-03-16 14:37:26.000000 rer.newsletter-2.0.0a2/src/rer.newsletter.egg-info/top_level.txt
+drwxr-xr-x   0 pieronicolli   (501) staff       (20)        0 2023-07-21 13:50:05.192121 rer.newsletter-2.0.0a3/
+-rw-r--r--   0 pieronicolli   (501) staff       (20)     3965 2023-07-21 13:50:04.000000 rer.newsletter-2.0.0a3/CHANGES.rst
+-rw-r--r--   0 pieronicolli   (501) staff       (20)       91 2023-07-21 13:50:04.000000 rer.newsletter-2.0.0a3/CONTRIBUTORS.rst
+-rw-r--r--   0 pieronicolli   (501) staff       (20)    18092 2023-07-21 13:50:04.000000 rer.newsletter-2.0.0a3/LICENSE.GPL
+-rw-r--r--   0 pieronicolli   (501) staff       (20)      658 2023-07-21 13:50:04.000000 rer.newsletter-2.0.0a3/LICENSE.rst
+-rw-r--r--   0 pieronicolli   (501) staff       (20)      152 2023-07-21 13:50:04.000000 rer.newsletter-2.0.0a3/MANIFEST.in
+-rw-r--r--   0 pieronicolli   (501) staff       (20)     9538 2023-07-21 13:50:05.192210 rer.newsletter-2.0.0a3/PKG-INFO
+-rw-r--r--   0 pieronicolli   (501) staff       (20)     4554 2023-07-21 13:50:04.000000 rer.newsletter-2.0.0a3/README.rst
+-rw-r--r--   0 pieronicolli   (501) staff       (20)       27 2023-07-21 13:50:04.000000 rer.newsletter-2.0.0a3/constraints.txt
+-rw-r--r--   0 pieronicolli   (501) staff       (20)      105 2023-07-21 13:50:04.000000 rer.newsletter-2.0.0a3/constraints_plone51.txt
+-rw-r--r--   0 pieronicolli   (501) staff       (20)      105 2023-07-21 13:50:04.000000 rer.newsletter-2.0.0a3/constraints_plone52.txt
+-rw-r--r--   0 pieronicolli   (501) staff       (20)      105 2023-07-21 13:50:04.000000 rer.newsletter-2.0.0a3/constraints_plone60.txt
+drwxr-xr-x   0 pieronicolli   (501) staff       (20)        0 2023-07-21 13:50:05.174869 rer.newsletter-2.0.0a3/docs/
+-rw-r--r--   0 pieronicolli   (501) staff       (20)       77 2023-07-21 13:50:04.000000 rer.newsletter-2.0.0a3/docs/index.rst
+-rw-r--r--   0 pieronicolli   (501) staff       (20)    32560 2023-07-21 13:50:04.000000 rer.newsletter-2.0.0a3/docs/rer-logo.png
+-rw-r--r--   0 pieronicolli   (501) staff       (20)       23 2023-07-21 13:50:04.000000 rer.newsletter-2.0.0a3/requirements.txt
+-rw-r--r--   0 pieronicolli   (501) staff       (20)      270 2023-07-21 13:50:05.192549 rer.newsletter-2.0.0a3/setup.cfg
+-rw-r--r--   0 pieronicolli   (501) staff       (20)     2391 2023-07-21 13:50:04.000000 rer.newsletter-2.0.0a3/setup.py
+drwxr-xr-x   0 pieronicolli   (501) staff       (20)        0 2023-07-21 13:50:05.170982 rer.newsletter-2.0.0a3/src/
+drwxr-xr-x   0 pieronicolli   (501) staff       (20)        0 2023-07-21 13:50:05.174992 rer.newsletter-2.0.0a3/src/rer/
+-rw-r--r--   0 pieronicolli   (501) staff       (20)       80 2023-07-21 13:50:04.000000 rer.newsletter-2.0.0a3/src/rer/__init__.py
+drwxr-xr-x   0 pieronicolli   (501) staff       (20)        0 2023-07-21 13:50:05.176884 rer.newsletter-2.0.0a3/src/rer/newsletter/
+-rw-r--r--   0 pieronicolli   (501) staff       (20)      184 2023-07-21 13:50:04.000000 rer.newsletter-2.0.0a3/src/rer/newsletter/__init__.py
+drwxr-xr-x   0 pieronicolli   (501) staff       (20)        0 2023-07-21 13:50:05.177278 rer.newsletter-2.0.0a3/src/rer/newsletter/adapter/
+-rw-r--r--   0 pieronicolli   (501) staff       (20)        0 2023-07-21 13:50:04.000000 rer.newsletter-2.0.0a3/src/rer/newsletter/adapter/__init__.py
+-rw-r--r--   0 pieronicolli   (501) staff       (20)      648 2023-07-21 13:50:04.000000 rer.newsletter-2.0.0a3/src/rer/newsletter/adapter/configure.zcml
+-rw-r--r--   0 pieronicolli   (501) staff       (20)     7952 2023-07-21 13:50:04.000000 rer.newsletter-2.0.0a3/src/rer/newsletter/adapter/sender.py
+-rw-r--r--   0 pieronicolli   (501) staff       (20)     8353 2023-07-21 13:50:04.000000 rer.newsletter-2.0.0a3/src/rer/newsletter/adapter/subscriptions.py
+drwxr-xr-x   0 pieronicolli   (501) staff       (20)        0 2023-07-21 13:50:05.177579 rer.newsletter-2.0.0a3/src/rer/newsletter/behaviors/
+-rw-r--r--   0 pieronicolli   (501) staff       (20)        0 2023-07-21 13:50:04.000000 rer.newsletter-2.0.0a3/src/rer/newsletter/behaviors/__init__.py
+-rw-r--r--   0 pieronicolli   (501) staff       (20)      441 2023-07-21 13:50:04.000000 rer.newsletter-2.0.0a3/src/rer/newsletter/behaviors/configure.zcml
+-rw-r--r--   0 pieronicolli   (501) staff       (20)      970 2023-07-21 13:50:04.000000 rer.newsletter-2.0.0a3/src/rer/newsletter/behaviors/ships.py
+drwxr-xr-x   0 pieronicolli   (501) staff       (20)        0 2023-07-21 13:50:05.177878 rer.newsletter-2.0.0a3/src/rer/newsletter/browser/
+-rw-r--r--   0 pieronicolli   (501) staff       (20)        0 2023-07-21 13:50:04.000000 rer.newsletter-2.0.0a3/src/rer/newsletter/browser/__init__.py
+drwxr-xr-x   0 pieronicolli   (501) staff       (20)        0 2023-07-21 13:50:05.179054 rer.newsletter-2.0.0a3/src/rer/newsletter/browser/channel/
+-rw-r--r--   0 pieronicolli   (501) staff       (20)        0 2023-07-21 13:50:04.000000 rer.newsletter-2.0.0a3/src/rer/newsletter/browser/channel/__init__.py
+-rw-r--r--   0 pieronicolli   (501) staff       (20)     1686 2023-07-21 13:50:04.000000 rer.newsletter-2.0.0a3/src/rer/newsletter/browser/channel/add.py
+-rw-r--r--   0 pieronicolli   (501) staff       (20)     1372 2023-07-21 13:50:04.000000 rer.newsletter-2.0.0a3/src/rer/newsletter/browser/channel/channelhistory.py
+-rw-r--r--   0 pieronicolli   (501) staff       (20)      708 2023-07-21 13:50:04.000000 rer.newsletter-2.0.0a3/src/rer/newsletter/browser/channel/channelview.py
+-rw-r--r--   0 pieronicolli   (501) staff       (20)      383 2023-07-21 13:50:04.000000 rer.newsletter-2.0.0a3/src/rer/newsletter/browser/channel/channelviewlet.py
+-rw-r--r--   0 pieronicolli   (501) staff       (20)     5549 2023-07-21 13:50:04.000000 rer.newsletter-2.0.0a3/src/rer/newsletter/browser/channel/configure.zcml
+-rw-r--r--   0 pieronicolli   (501) staff       (20)     2208 2023-07-21 13:50:04.000000 rer.newsletter-2.0.0a3/src/rer/newsletter/browser/channel/deleteexpiredusers.py
+-rw-r--r--   0 pieronicolli   (501) staff       (20)     3177 2023-07-21 13:50:04.000000 rer.newsletter-2.0.0a3/src/rer/newsletter/browser/channel/manageusers.py
+-rw-r--r--   0 pieronicolli   (501) staff       (20)      365 2023-07-21 13:50:04.000000 rer.newsletter-2.0.0a3/src/rer/newsletter/browser/channel/plone_version.py
+-rw-r--r--   0 pieronicolli   (501) staff       (20)     5321 2023-07-21 13:50:04.000000 rer.newsletter-2.0.0a3/src/rer/newsletter/browser/channel/subscribe.py
+drwxr-xr-x   0 pieronicolli   (501) staff       (20)        0 2023-07-21 13:50:05.179823 rer.newsletter-2.0.0a3/src/rer/newsletter/browser/channel/templates/
+-rw-r--r--   0 pieronicolli   (501) staff       (20)     1746 2023-07-21 13:50:04.000000 rer.newsletter-2.0.0a3/src/rer/newsletter/browser/channel/templates/channelhistoryview.pt
+-rw-r--r--   0 pieronicolli   (501) staff       (20)     2608 2023-07-21 13:50:04.000000 rer.newsletter-2.0.0a3/src/rer/newsletter/browser/channel/templates/channelview.pt
+-rw-r--r--   0 pieronicolli   (501) staff       (20)      911 2023-07-21 13:50:04.000000 rer.newsletter-2.0.0a3/src/rer/newsletter/browser/channel/templates/channelviewlet.pt
+-rw-r--r--   0 pieronicolli   (501) staff       (20)      885 2023-07-21 13:50:04.000000 rer.newsletter-2.0.0a3/src/rer/newsletter/browser/channel/templates/confirm_subscription.pt
+drwxr-xr-x   0 pieronicolli   (501) staff       (20)        0 2023-07-21 13:50:05.180590 rer.newsletter-2.0.0a3/src/rer/newsletter/browser/channel/templates/mail_templates/
+-rw-r--r--   0 pieronicolli   (501) staff       (20)      851 2023-07-21 13:50:04.000000 rer.newsletter-2.0.0a3/src/rer/newsletter/browser/channel/templates/mail_templates/active_user.pt
+-rw-r--r--   0 pieronicolli   (501) staff       (20)      568 2023-07-21 13:50:04.000000 rer.newsletter-2.0.0a3/src/rer/newsletter/browser/channel/templates/mail_templates/active_user_confirm.pt
+-rw-r--r--   0 pieronicolli   (501) staff       (20)      603 2023-07-21 13:50:04.000000 rer.newsletter-2.0.0a3/src/rer/newsletter/browser/channel/templates/mail_templates/asynch_send_fail.pt
+-rw-r--r--   0 pieronicolli   (501) staff       (20)      728 2023-07-21 13:50:04.000000 rer.newsletter-2.0.0a3/src/rer/newsletter/browser/channel/templates/mail_templates/asynch_send_success.pt
+-rw-r--r--   0 pieronicolli   (501) staff       (20)      571 2023-07-21 13:50:04.000000 rer.newsletter-2.0.0a3/src/rer/newsletter/browser/channel/templates/mail_templates/delete_user.pt
+-rw-r--r--   0 pieronicolli   (501) staff       (20)      611 2023-07-21 13:50:04.000000 rer.newsletter-2.0.0a3/src/rer/newsletter/browser/channel/templates/mail_templates/delete_user_confirm.pt
+-rw-r--r--   0 pieronicolli   (501) staff       (20)      592 2023-07-21 13:50:04.000000 rer.newsletter-2.0.0a3/src/rer/newsletter/browser/channel/templates/mail_templates/unsubscribe_channel.pt
+-rw-r--r--   0 pieronicolli   (501) staff       (20)     3193 2023-07-21 13:50:04.000000 rer.newsletter-2.0.0a3/src/rer/newsletter/browser/channel/templates/manageusers.pt
+-rw-r--r--   0 pieronicolli   (501) staff       (20)     1839 2023-07-21 13:50:04.000000 rer.newsletter-2.0.0a3/src/rer/newsletter/browser/channel/templates/subscribechannel.pt
+-rw-r--r--   0 pieronicolli   (501) staff       (20)     1232 2023-07-21 13:50:04.000000 rer.newsletter-2.0.0a3/src/rer/newsletter/browser/channel/templates/unsubscribechannel.pt
+-rw-r--r--   0 pieronicolli   (501) staff       (20)     4430 2023-07-21 13:50:04.000000 rer.newsletter-2.0.0a3/src/rer/newsletter/browser/channel/unsubscribe.py
+drwxr-xr-x   0 pieronicolli   (501) staff       (20)        0 2023-07-21 13:50:05.180996 rer.newsletter-2.0.0a3/src/rer/newsletter/browser/channel/users/
+-rw-r--r--   0 pieronicolli   (501) staff       (20)        0 2023-07-21 13:50:04.000000 rer.newsletter-2.0.0a3/src/rer/newsletter/browser/channel/users/__init__.py
+-rw-r--r--   0 pieronicolli   (501) staff       (20)     1828 2023-07-21 13:50:04.000000 rer.newsletter-2.0.0a3/src/rer/newsletter/browser/channel/users/add.py
+-rw-r--r--   0 pieronicolli   (501) staff       (20)     3892 2023-07-21 13:50:04.000000 rer.newsletter-2.0.0a3/src/rer/newsletter/browser/channel/users/confirm_subscription.py
+-rw-r--r--   0 pieronicolli   (501) staff       (20)     5980 2023-07-21 13:50:04.000000 rer.newsletter-2.0.0a3/src/rer/newsletter/browser/channel/users/usersimport.py
+-rw-r--r--   0 pieronicolli   (501) staff       (20)      907 2023-07-21 13:50:04.000000 rer.newsletter-2.0.0a3/src/rer/newsletter/browser/configure.zcml
+drwxr-xr-x   0 pieronicolli   (501) staff       (20)        0 2023-07-21 13:50:05.182172 rer.newsletter-2.0.0a3/src/rer/newsletter/browser/message/
+-rw-r--r--   0 pieronicolli   (501) staff       (20)        0 2023-07-21 13:50:04.000000 rer.newsletter-2.0.0a3/src/rer/newsletter/browser/message/__init__.py
+-rw-r--r--   0 pieronicolli   (501) staff       (20)      525 2023-07-21 13:50:04.000000 rer.newsletter-2.0.0a3/src/rer/newsletter/browser/message/checkmessageview.py
+-rw-r--r--   0 pieronicolli   (501) staff       (20)      442 2023-07-21 13:50:04.000000 rer.newsletter-2.0.0a3/src/rer/newsletter/browser/message/collectionview.py
+-rw-r--r--   0 pieronicolli   (501) staff       (20)     2969 2023-07-21 13:50:04.000000 rer.newsletter-2.0.0a3/src/rer/newsletter/browser/message/configure.zcml
+-rw-r--r--   0 pieronicolli   (501) staff       (20)     2603 2023-07-21 13:50:04.000000 rer.newsletter-2.0.0a3/src/rer/newsletter/browser/message/messagepreview.py
+-rw-r--r--   0 pieronicolli   (501) staff       (20)      174 2023-07-21 13:50:04.000000 rer.newsletter-2.0.0a3/src/rer/newsletter/browser/message/messageview.py
+-rw-r--r--   0 pieronicolli   (501) staff       (20)     1543 2023-07-21 13:50:04.000000 rer.newsletter-2.0.0a3/src/rer/newsletter/browser/message/messageviewlet.py
+-rw-r--r--   0 pieronicolli   (501) staff       (20)     5408 2023-07-21 13:50:04.000000 rer.newsletter-2.0.0a3/src/rer/newsletter/browser/message/sendingtest.py
+-rw-r--r--   0 pieronicolli   (501) staff       (20)     3057 2023-07-21 13:50:04.000000 rer.newsletter-2.0.0a3/src/rer/newsletter/browser/message/sendmessageview.py
+-rw-r--r--   0 pieronicolli   (501) staff       (20)      288 2023-07-21 13:50:04.000000 rer.newsletter-2.0.0a3/src/rer/newsletter/browser/message/shippablecollection.py
+drwxr-xr-x   0 pieronicolli   (501) staff       (20)        0 2023-07-21 13:50:05.182918 rer.newsletter-2.0.0a3/src/rer/newsletter/browser/message/templates/
+-rw-r--r--   0 pieronicolli   (501) staff       (20)     2687 2023-07-21 13:50:04.000000 rer.newsletter-2.0.0a3/src/rer/newsletter/browser/message/templates/collection_sending_view.pt
+-rw-r--r--   0 pieronicolli   (501) staff       (20)      870 2023-07-21 13:50:04.000000 rer.newsletter-2.0.0a3/src/rer/newsletter/browser/message/templates/messagecontentcore.pt
+-rw-r--r--   0 pieronicolli   (501) staff       (20)     1532 2023-07-21 13:50:04.000000 rer.newsletter-2.0.0a3/src/rer/newsletter/browser/message/templates/messagepreview.pt
+-rw-r--r--   0 pieronicolli   (501) staff       (20)      952 2023-07-21 13:50:04.000000 rer.newsletter-2.0.0a3/src/rer/newsletter/browser/message/templates/messageview.pt
+-rw-r--r--   0 pieronicolli   (501) staff       (20)     1720 2023-07-21 13:50:04.000000 rer.newsletter-2.0.0a3/src/rer/newsletter/browser/message/templates/messageviewlet.pt
+-rw-r--r--   0 pieronicolli   (501) staff       (20)     1132 2023-07-21 13:50:04.000000 rer.newsletter-2.0.0a3/src/rer/newsletter/browser/message/templates/sendingtest.pt
+-rw-r--r--   0 pieronicolli   (501) staff       (20)     1451 2023-07-21 13:50:04.000000 rer.newsletter-2.0.0a3/src/rer/newsletter/browser/message/templates/sendmessageview.pt
+-rw-r--r--   0 pieronicolli   (501) staff       (20)      570 2023-07-21 13:50:04.000000 rer.newsletter-2.0.0a3/src/rer/newsletter/browser/message/versionview.py
+drwxr-xr-x   0 pieronicolli   (501) staff       (20)        0 2023-07-21 13:50:05.183034 rer.newsletter-2.0.0a3/src/rer/newsletter/browser/overrides/
+-rw-r--r--   0 pieronicolli   (501) staff       (20)        0 2023-07-21 13:50:04.000000 rer.newsletter-2.0.0a3/src/rer/newsletter/browser/overrides/.gitkeep
+-rw-r--r--   0 pieronicolli   (501) staff       (20)     1465 2023-07-21 13:50:04.000000 rer.newsletter-2.0.0a3/src/rer/newsletter/browser/settings.py
+drwxr-xr-x   0 pieronicolli   (501) staff       (20)        0 2023-07-21 13:50:05.183311 rer.newsletter-2.0.0a3/src/rer/newsletter/browser/static/
+-rw-r--r--   0 pieronicolli   (501) staff       (20)        0 2023-07-21 13:50:04.000000 rer.newsletter-2.0.0a3/src/rer/newsletter/browser/static/.gitkeep
+drwxr-xr-x   0 pieronicolli   (501) staff       (20)        0 2023-07-21 13:50:05.183416 rer.newsletter-2.0.0a3/src/rer/newsletter/browser/static/DataTables-1.10.16/
+-rw-r--r--   0 pieronicolli   (501) staff       (20)     6148 2023-07-21 13:50:04.000000 rer.newsletter-2.0.0a3/src/rer/newsletter/browser/static/DataTables-1.10.16/.DS_Store
+drwxr-xr-x   0 pieronicolli   (501) staff       (20)        0 2023-07-21 13:50:05.183956 rer.newsletter-2.0.0a3/src/rer/newsletter/browser/static/DataTables-1.10.16/images/
+-rwxr-xr-x   0 pieronicolli   (501) staff       (20)      160 2023-07-21 13:50:04.000000 rer.newsletter-2.0.0a3/src/rer/newsletter/browser/static/DataTables-1.10.16/images/sort_asc.png
+-rwxr-xr-x   0 pieronicolli   (501) staff       (20)      148 2023-07-21 13:50:04.000000 rer.newsletter-2.0.0a3/src/rer/newsletter/browser/static/DataTables-1.10.16/images/sort_asc_disabled.png
+-rwxr-xr-x   0 pieronicolli   (501) staff       (20)      201 2023-07-21 13:50:04.000000 rer.newsletter-2.0.0a3/src/rer/newsletter/browser/static/DataTables-1.10.16/images/sort_both.png
+-rwxr-xr-x   0 pieronicolli   (501) staff       (20)      158 2023-07-21 13:50:04.000000 rer.newsletter-2.0.0a3/src/rer/newsletter/browser/static/DataTables-1.10.16/images/sort_desc.png
+-rwxr-xr-x   0 pieronicolli   (501) staff       (20)      146 2023-07-21 13:50:04.000000 rer.newsletter-2.0.0a3/src/rer/newsletter/browser/static/DataTables-1.10.16/images/sort_desc_disabled.png
+-rw-r--r--   0 pieronicolli   (501) staff       (20)     1436 2023-07-21 13:50:04.000000 rer.newsletter-2.0.0a3/src/rer/newsletter/browser/static/custom.css
+-rw-r--r--   0 pieronicolli   (501) staff       (20)    16203 2023-07-21 13:50:04.000000 rer.newsletter-2.0.0a3/src/rer/newsletter/browser/static/datatables.css
+drwxr-xr-x   0 pieronicolli   (501) staff       (20)        0 2023-07-21 13:50:05.184675 rer.newsletter-2.0.0a3/src/rer/newsletter/browser/static/scripts/
+-rw-r--r--   0 pieronicolli   (501) staff       (20)     2707 2023-07-21 13:50:04.000000 rer.newsletter-2.0.0a3/src/rer/newsletter/browser/static/scripts/channelhistory.js
+-rwxr-xr-x   0 pieronicolli   (501) staff       (20)   443959 2023-07-21 13:50:04.000000 rer.newsletter-2.0.0a3/src/rer/newsletter/browser/static/scripts/datatables.js
+-rw-r--r--   0 pieronicolli   (501) staff       (20)     4087 2023-07-21 13:50:04.000000 rer.newsletter-2.0.0a3/src/rer/newsletter/browser/static/scripts/initializedModal.js
+-rw-r--r--   0 pieronicolli   (501) staff       (20)     4000 2023-07-21 13:50:04.000000 rer.newsletter-2.0.0a3/src/rer/newsletter/browser/static/scripts/manageusers.js
+-rw-r--r--   0 pieronicolli   (501) staff       (20)     2216 2023-07-21 13:50:04.000000 rer.newsletter-2.0.0a3/src/rer/newsletter/configure.zcml
+drwxr-xr-x   0 pieronicolli   (501) staff       (20)        0 2023-07-21 13:50:05.185081 rer.newsletter-2.0.0a3/src/rer/newsletter/content/
+-rw-r--r--   0 pieronicolli   (501) staff       (20)        0 2023-07-21 13:50:04.000000 rer.newsletter-2.0.0a3/src/rer/newsletter/content/__init__.py
+-rw-r--r--   0 pieronicolli   (501) staff       (20)      217 2023-07-21 13:50:04.000000 rer.newsletter-2.0.0a3/src/rer/newsletter/content/channel.py
+-rw-r--r--   0 pieronicolli   (501) staff       (20)      217 2023-07-21 13:50:04.000000 rer.newsletter-2.0.0a3/src/rer/newsletter/content/message.py
+-rw-r--r--   0 pieronicolli   (501) staff       (20)      261 2023-07-21 13:50:04.000000 rer.newsletter-2.0.0a3/src/rer/newsletter/content/shippable_collection.py
+drwxr-xr-x   0 pieronicolli   (501) staff       (20)        0 2023-07-21 13:50:05.185913 rer.newsletter-2.0.0a3/src/rer/newsletter/contentrules/
+-rw-r--r--   0 pieronicolli   (501) staff       (20)       24 2023-07-21 13:50:04.000000 rer.newsletter-2.0.0a3/src/rer/newsletter/contentrules/__init__.py
+-rw-r--r--   0 pieronicolli   (501) staff       (20)      871 2023-07-21 13:50:04.000000 rer.newsletter-2.0.0a3/src/rer/newsletter/contentrules/actions.py
+-rw-r--r--   0 pieronicolli   (501) staff       (20)     3229 2023-07-21 13:50:04.000000 rer.newsletter-2.0.0a3/src/rer/newsletter/contentrules/configure.zcml
+-rw-r--r--   0 pieronicolli   (501) staff       (20)      955 2023-07-21 13:50:04.000000 rer.newsletter-2.0.0a3/src/rer/newsletter/contentrules/events.py
+-rw-r--r--   0 pieronicolli   (501) staff       (20)     2092 2023-07-21 13:50:04.000000 rer.newsletter-2.0.0a3/src/rer/newsletter/contentrules/executors.py
+-rw-r--r--   0 pieronicolli   (501) staff       (20)     1907 2023-07-21 13:50:04.000000 rer.newsletter-2.0.0a3/src/rer/newsletter/contentrules/forms.py
+-rw-r--r--   0 pieronicolli   (501) staff       (20)      216 2023-07-21 13:50:04.000000 rer.newsletter-2.0.0a3/src/rer/newsletter/contentrules/handlers.py
+-rw-r--r--   0 pieronicolli   (501) staff       (20)     1376 2023-07-21 13:50:04.000000 rer.newsletter-2.0.0a3/src/rer/newsletter/contentrules/interfaces.py
+drwxr-xr-x   0 pieronicolli   (501) staff       (20)        0 2023-07-21 13:50:05.186106 rer.newsletter-2.0.0a3/src/rer/newsletter/exceptions/
+-rw-r--r--   0 pieronicolli   (501) staff       (20)        0 2023-07-21 13:50:04.000000 rer.newsletter-2.0.0a3/src/rer/newsletter/exceptions/__init__.py
+-rw-r--r--   0 pieronicolli   (501) staff       (20)      132 2023-07-21 13:50:04.000000 rer.newsletter-2.0.0a3/src/rer/newsletter/exceptions/exceptions.py
+-rw-r--r--   0 pieronicolli   (501) staff       (20)     3577 2023-07-21 13:50:04.000000 rer.newsletter-2.0.0a3/src/rer/newsletter/interfaces.py
+drwxr-xr-x   0 pieronicolli   (501) staff       (20)        0 2023-07-21 13:50:05.186418 rer.newsletter-2.0.0a3/src/rer/newsletter/locales/
+drwxr-xr-x   0 pieronicolli   (501) staff       (20)        0 2023-07-21 13:50:05.172311 rer.newsletter-2.0.0a3/src/rer/newsletter/locales/it/
+drwxr-xr-x   0 pieronicolli   (501) staff       (20)        0 2023-07-21 13:50:05.186533 rer.newsletter-2.0.0a3/src/rer/newsletter/locales/it/LC_MESSAGES/
+-rw-r--r--   0 pieronicolli   (501) staff       (20)    17210 2023-07-21 13:50:04.000000 rer.newsletter-2.0.0a3/src/rer/newsletter/locales/it/LC_MESSAGES/rer.newsletter.po
+-rw-r--r--   0 pieronicolli   (501) staff       (20)    14456 2023-07-21 13:50:04.000000 rer.newsletter-2.0.0a3/src/rer/newsletter/locales/rer.newsletter.pot
+-rw-r--r--   0 pieronicolli   (501) staff       (20)     1569 2023-07-21 13:50:04.000000 rer.newsletter-2.0.0a3/src/rer/newsletter/locales/update.py
+-rwxr-xr-x   0 pieronicolli   (501) staff       (20)      503 2023-07-21 13:50:04.000000 rer.newsletter-2.0.0a3/src/rer/newsletter/locales/update.sh
+drwxr-xr-x   0 pieronicolli   (501) staff       (20)        0 2023-07-21 13:50:05.187107 rer.newsletter-2.0.0a3/src/rer/newsletter/portlets/
+-rw-r--r--   0 pieronicolli   (501) staff       (20)        0 2023-07-21 13:50:04.000000 rer.newsletter-2.0.0a3/src/rer/newsletter/portlets/__init__.py
+-rw-r--r--   0 pieronicolli   (501) staff       (20)      573 2023-07-21 13:50:04.000000 rer.newsletter-2.0.0a3/src/rer/newsletter/portlets/configure.zcml
+-rw-r--r--   0 pieronicolli   (501) staff       (20)     1695 2023-07-21 13:50:04.000000 rer.newsletter-2.0.0a3/src/rer/newsletter/portlets/interface.py
+-rw-r--r--   0 pieronicolli   (501) staff       (20)      964 2023-07-21 13:50:04.000000 rer.newsletter-2.0.0a3/src/rer/newsletter/portlets/subscribe.pt
+-rw-r--r--   0 pieronicolli   (501) staff       (20)     1912 2023-07-21 13:50:04.000000 rer.newsletter-2.0.0a3/src/rer/newsletter/portlets/subscribe.py
+drwxr-xr-x   0 pieronicolli   (501) staff       (20)        0 2023-07-21 13:50:05.172796 rer.newsletter-2.0.0a3/src/rer/newsletter/profiles/
+drwxr-xr-x   0 pieronicolli   (501) staff       (20)        0 2023-07-21 13:50:05.188581 rer.newsletter-2.0.0a3/src/rer/newsletter/profiles/default/
+-rw-r--r--   0 pieronicolli   (501) staff       (20)      178 2023-07-21 13:50:04.000000 rer.newsletter-2.0.0a3/src/rer/newsletter/profiles/default/actions.xml
+-rw-r--r--   0 pieronicolli   (501) staff       (20)      161 2023-07-21 13:50:04.000000 rer.newsletter-2.0.0a3/src/rer/newsletter/profiles/default/browserlayer.xml
+-rw-r--r--   0 pieronicolli   (501) staff       (20)      275 2023-07-21 13:50:04.000000 rer.newsletter-2.0.0a3/src/rer/newsletter/profiles/default/catalog.xml
+-rw-r--r--   0 pieronicolli   (501) staff       (20)      570 2023-07-21 13:50:04.000000 rer.newsletter-2.0.0a3/src/rer/newsletter/profiles/default/controlpanel.xml
+-rw-r--r--   0 pieronicolli   (501) staff       (20)      373 2023-07-21 13:50:04.000000 rer.newsletter-2.0.0a3/src/rer/newsletter/profiles/default/diff_tool.xml
+-rw-r--r--   0 pieronicolli   (501) staff       (20)      184 2023-07-21 13:50:04.000000 rer.newsletter-2.0.0a3/src/rer/newsletter/profiles/default/metadata.xml
+-rw-r--r--   0 pieronicolli   (501) staff       (20)      280 2023-07-21 13:50:04.000000 rer.newsletter-2.0.0a3/src/rer/newsletter/profiles/default/portlets.xml
+-rw-r--r--   0 pieronicolli   (501) staff       (20)     3209 2023-07-21 13:50:04.000000 rer.newsletter-2.0.0a3/src/rer/newsletter/profiles/default/registry.xml
+-rw-r--r--   0 pieronicolli   (501) staff       (20)      365 2023-07-21 13:50:04.000000 rer.newsletter-2.0.0a3/src/rer/newsletter/profiles/default/repositorytool.xml
+-rw-r--r--   0 pieronicolli   (501) staff       (20)     1350 2023-07-21 13:50:04.000000 rer.newsletter-2.0.0a3/src/rer/newsletter/profiles/default/rolemap.xml
+-rw-r--r--   0 pieronicolli   (501) staff       (20)      252 2023-07-21 13:50:04.000000 rer.newsletter-2.0.0a3/src/rer/newsletter/profiles/default/sharing.xml
+drwxr-xr-x   0 pieronicolli   (501) staff       (20)        0 2023-07-21 13:50:05.188908 rer.newsletter-2.0.0a3/src/rer/newsletter/profiles/default/types/
+-rw-r--r--   0 pieronicolli   (501) staff       (20)     2961 2023-07-21 13:50:04.000000 rer.newsletter-2.0.0a3/src/rer/newsletter/profiles/default/types/Channel.xml
+-rw-r--r--   0 pieronicolli   (501) staff       (20)     3036 2023-07-21 13:50:04.000000 rer.newsletter-2.0.0a3/src/rer/newsletter/profiles/default/types/Message.xml
+-rw-r--r--   0 pieronicolli   (501) staff       (20)     3345 2023-07-21 13:50:04.000000 rer.newsletter-2.0.0a3/src/rer/newsletter/profiles/default/types/Shippable_Collection.xml
+-rw-r--r--   0 pieronicolli   (501) staff       (20)      327 2023-07-21 13:50:04.000000 rer.newsletter-2.0.0a3/src/rer/newsletter/profiles/default/types.xml
+drwxr-xr-x   0 pieronicolli   (501) staff       (20)        0 2023-07-21 13:50:05.172731 rer.newsletter-2.0.0a3/src/rer/newsletter/profiles/default/workflows/
+drwxr-xr-x   0 pieronicolli   (501) staff       (20)        0 2023-07-21 13:50:05.189022 rer.newsletter-2.0.0a3/src/rer/newsletter/profiles/default/workflows/channel_workflow/
+-rw-r--r--   0 pieronicolli   (501) staff       (20)     8132 2023-07-21 13:50:04.000000 rer.newsletter-2.0.0a3/src/rer/newsletter/profiles/default/workflows/channel_workflow/definition.xml
+drwxr-xr-x   0 pieronicolli   (501) staff       (20)        0 2023-07-21 13:50:05.189137 rer.newsletter-2.0.0a3/src/rer/newsletter/profiles/default/workflows/message_workflow/
+-rw-r--r--   0 pieronicolli   (501) staff       (20)     9923 2023-07-21 13:50:04.000000 rer.newsletter-2.0.0a3/src/rer/newsletter/profiles/default/workflows/message_workflow/definition.xml
+-rw-r--r--   0 pieronicolli   (501) staff       (20)      643 2023-07-21 13:50:04.000000 rer.newsletter-2.0.0a3/src/rer/newsletter/profiles/default/workflows.xml
+drwxr-xr-x   0 pieronicolli   (501) staff       (20)        0 2023-07-21 13:50:05.189674 rer.newsletter-2.0.0a3/src/rer/newsletter/profiles/uninstall/
+-rw-r--r--   0 pieronicolli   (501) staff       (20)      824 2023-07-21 13:50:04.000000 rer.newsletter-2.0.0a3/src/rer/newsletter/profiles/uninstall/actions.xml
+-rw-r--r--   0 pieronicolli   (501) staff       (20)      117 2023-07-21 13:50:04.000000 rer.newsletter-2.0.0a3/src/rer/newsletter/profiles/uninstall/browserlayer.xml
+-rw-r--r--   0 pieronicolli   (501) staff       (20)      321 2023-07-21 13:50:04.000000 rer.newsletter-2.0.0a3/src/rer/newsletter/profiles/uninstall/controlpanel.xml
+-rw-r--r--   0 pieronicolli   (501) staff       (20)      701 2023-07-21 13:50:04.000000 rer.newsletter-2.0.0a3/src/rer/newsletter/profiles/uninstall/registry.xml
+-rw-r--r--   0 pieronicolli   (501) staff       (20)      296 2023-07-21 13:50:04.000000 rer.newsletter-2.0.0a3/src/rer/newsletter/profiles/uninstall/types.xml
+-rw-r--r--   0 pieronicolli   (501) staff       (20)       30 2023-07-21 13:50:04.000000 rer.newsletter-2.0.0a3/src/rer/newsletter/pyproject.toml
+drwxr-xr-x   0 pieronicolli   (501) staff       (20)        0 2023-07-21 13:50:05.190194 rer.newsletter-2.0.0a3/src/rer/newsletter/queue/
+-rw-r--r--   0 pieronicolli   (501) staff       (20)       24 2023-07-21 13:50:04.000000 rer.newsletter-2.0.0a3/src/rer/newsletter/queue/__init__.py
+-rw-r--r--   0 pieronicolli   (501) staff       (20)      487 2023-07-21 13:50:04.000000 rer.newsletter-2.0.0a3/src/rer/newsletter/queue/configure.zcml
+-rw-r--r--   0 pieronicolli   (501) staff       (20)      643 2023-07-21 13:50:04.000000 rer.newsletter-2.0.0a3/src/rer/newsletter/queue/handler.py
+-rw-r--r--   0 pieronicolli   (501) staff       (20)      360 2023-07-21 13:50:04.000000 rer.newsletter-2.0.0a3/src/rer/newsletter/queue/interfaces.py
+-rw-r--r--   0 pieronicolli   (501) staff       (20)     5050 2023-07-21 13:50:04.000000 rer.newsletter-2.0.0a3/src/rer/newsletter/queue/view.py
+drwxr-xr-x   0 pieronicolli   (501) staff       (20)        0 2023-07-21 13:50:05.190389 rer.newsletter-2.0.0a3/src/rer/newsletter/restapi/
+-rw-r--r--   0 pieronicolli   (501) staff       (20)        0 2023-07-21 13:50:04.000000 rer.newsletter-2.0.0a3/src/rer/newsletter/restapi/__init__.py
+-rw-r--r--   0 pieronicolli   (501) staff       (20)      240 2023-07-21 13:50:04.000000 rer.newsletter-2.0.0a3/src/rer/newsletter/restapi/configure.zcml
+drwxr-xr-x   0 pieronicolli   (501) staff       (20)        0 2023-07-21 13:50:05.190909 rer.newsletter-2.0.0a3/src/rer/newsletter/restapi/services/
+-rw-r--r--   0 pieronicolli   (501) staff       (20)        0 2023-07-21 13:50:04.000000 rer.newsletter-2.0.0a3/src/rer/newsletter/restapi/services/__init__.py
+-rw-r--r--   0 pieronicolli   (501) staff       (20)      784 2023-07-21 13:50:04.000000 rer.newsletter-2.0.0a3/src/rer/newsletter/restapi/services/configure.zcml
+-rw-r--r--   0 pieronicolli   (501) staff       (20)     3875 2023-07-21 13:50:04.000000 rer.newsletter-2.0.0a3/src/rer/newsletter/restapi/services/confirm_subscription.py
+-rw-r--r--   0 pieronicolli   (501) staff       (20)     3821 2023-07-21 13:50:04.000000 rer.newsletter-2.0.0a3/src/rer/newsletter/restapi/services/subscribe.py
+-rw-r--r--   0 pieronicolli   (501) staff       (20)     3497 2023-07-21 13:50:04.000000 rer.newsletter-2.0.0a3/src/rer/newsletter/restapi/services/unsubscribe.py
+-rw-r--r--   0 pieronicolli   (501) staff       (20)     1220 2023-07-21 13:50:04.000000 rer.newsletter-2.0.0a3/src/rer/newsletter/setuphandlers.py
+-rw-r--r--   0 pieronicolli   (501) staff       (20)     1174 2023-07-21 13:50:04.000000 rer.newsletter-2.0.0a3/src/rer/newsletter/testing.py
+drwxr-xr-x   0 pieronicolli   (501) staff       (20)        0 2023-07-21 13:50:05.191313 rer.newsletter-2.0.0a3/src/rer/newsletter/tests/
+-rw-r--r--   0 pieronicolli   (501) staff       (20)        0 2023-07-21 13:50:04.000000 rer.newsletter-2.0.0a3/src/rer/newsletter/tests/__init__.py
+-rw-r--r--   0 pieronicolli   (501) staff       (20)     3009 2023-07-21 13:50:04.000000 rer.newsletter-2.0.0a3/src/rer/newsletter/tests/test_setup.py
+-rw-r--r--   0 pieronicolli   (501) staff       (20)     2102 2023-07-21 13:50:04.000000 rer.newsletter-2.0.0a3/src/rer/newsletter/tests/test_subscription_tile.py
+-rw-r--r--   0 pieronicolli   (501) staff       (20)     9313 2023-07-21 13:50:04.000000 rer.newsletter-2.0.0a3/src/rer/newsletter/tests/test_subscriptions_adapter.py
+drwxr-xr-x   0 pieronicolli   (501) staff       (20)        0 2023-07-21 13:50:05.191722 rer.newsletter-2.0.0a3/src/rer/newsletter/tiles/
+-rw-r--r--   0 pieronicolli   (501) staff       (20)        0 2023-07-21 13:50:04.000000 rer.newsletter-2.0.0a3/src/rer/newsletter/tiles/__init__.py
+-rw-r--r--   0 pieronicolli   (501) staff       (20)      635 2023-07-21 13:50:04.000000 rer.newsletter-2.0.0a3/src/rer/newsletter/tiles/configure.zcml
+-rw-r--r--   0 pieronicolli   (501) staff       (20)     1340 2023-07-21 13:50:04.000000 rer.newsletter-2.0.0a3/src/rer/newsletter/tiles/subscribe.pt
+-rw-r--r--   0 pieronicolli   (501) staff       (20)     1104 2023-07-21 13:50:04.000000 rer.newsletter-2.0.0a3/src/rer/newsletter/tiles/subscribe.py
+drwxr-xr-x   0 pieronicolli   (501) staff       (20)        0 2023-07-21 13:50:05.192022 rer.newsletter-2.0.0a3/src/rer/newsletter/transforms/
+-rw-r--r--   0 pieronicolli   (501) staff       (20)        0 2023-07-21 13:50:04.000000 rer.newsletter-2.0.0a3/src/rer/newsletter/transforms/__init__.py
+-rw-r--r--   0 pieronicolli   (501) staff       (20)     2037 2023-07-21 13:50:04.000000 rer.newsletter-2.0.0a3/src/rer/newsletter/transforms/link_transform.py
+-rw-r--r--   0 pieronicolli   (501) staff       (20)      206 2023-07-21 13:50:04.000000 rer.newsletter-2.0.0a3/src/rer/newsletter/transforms/mimetype.py
+-rw-r--r--   0 pieronicolli   (501) staff       (20)     3154 2023-07-21 13:50:04.000000 rer.newsletter-2.0.0a3/src/rer/newsletter/upgrades.py
+-rw-r--r--   0 pieronicolli   (501) staff       (20)     1101 2023-07-21 13:50:04.000000 rer.newsletter-2.0.0a3/src/rer/newsletter/upgrades.zcml
+-rw-r--r--   0 pieronicolli   (501) staff       (20)     1309 2023-07-21 13:50:04.000000 rer.newsletter-2.0.0a3/src/rer/newsletter/utils.py
+-rw-r--r--   0 pieronicolli   (501) staff       (20)      864 2023-07-21 13:50:04.000000 rer.newsletter-2.0.0a3/src/rer/newsletter/vocabularies.py
+drwxr-xr-x   0 pieronicolli   (501) staff       (20)        0 2023-07-21 13:50:05.175830 rer.newsletter-2.0.0a3/src/rer.newsletter.egg-info/
+-rw-r--r--   0 pieronicolli   (501) staff       (20)     9538 2023-07-21 13:50:04.000000 rer.newsletter-2.0.0a3/src/rer.newsletter.egg-info/PKG-INFO
+-rw-r--r--   0 pieronicolli   (501) staff       (20)     8222 2023-07-21 13:50:05.000000 rer.newsletter-2.0.0a3/src/rer.newsletter.egg-info/SOURCES.txt
+-rw-r--r--   0 pieronicolli   (501) staff       (20)        1 2023-07-21 13:50:04.000000 rer.newsletter-2.0.0a3/src/rer.newsletter.egg-info/dependency_links.txt
+-rw-r--r--   0 pieronicolli   (501) staff       (20)      119 2023-07-21 13:50:04.000000 rer.newsletter-2.0.0a3/src/rer.newsletter.egg-info/entry_points.txt
+-rw-r--r--   0 pieronicolli   (501) staff       (20)        4 2023-07-21 13:50:04.000000 rer.newsletter-2.0.0a3/src/rer.newsletter.egg-info/namespace_packages.txt
+-rw-r--r--   0 pieronicolli   (501) staff       (20)        1 2023-07-21 13:50:04.000000 rer.newsletter-2.0.0a3/src/rer.newsletter.egg-info/not-zip-safe
+-rw-r--r--   0 pieronicolli   (501) staff       (20)      292 2023-07-21 13:50:05.000000 rer.newsletter-2.0.0a3/src/rer.newsletter.egg-info/requires.txt
+-rw-r--r--   0 pieronicolli   (501) staff       (20)        4 2023-07-21 13:50:05.000000 rer.newsletter-2.0.0a3/src/rer.newsletter.egg-info/top_level.txt
```

### Comparing `rer.newsletter-2.0.0a2/CHANGES.rst` & `rer.newsletter-2.0.0a3/CHANGES.rst`

 * *Files 2% similar despite different names*

```diff
@@ -1,11 +1,18 @@
 =========
 Changelog
 =========
 
+2.0.0a3 (2023-07-21)
+--------------------
+
+- Adapt management buttons for Plone 6
+  [pnicolli]
+
+
 2.0.0a2 (2023-03-16)
 --------------------
 
 - Updated subheader template
   [pnicolli]
```

### Comparing `rer.newsletter-2.0.0a2/LICENSE.GPL` & `rer.newsletter-2.0.0a3/LICENSE.GPL`

 * *Files identical despite different names*

### Comparing `rer.newsletter-2.0.0a2/LICENSE.rst` & `rer.newsletter-2.0.0a3/LICENSE.rst`

 * *Files identical despite different names*

### Comparing `rer.newsletter-2.0.0a2/PKG-INFO` & `rer.newsletter-2.0.0a3/PKG-INFO`

 * *Files 2% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: rer.newsletter
-Version: 2.0.0a2
+Version: 2.0.0a3
 Summary: An add-on for Plone
 Home-page: https://pypi.python.org/pypi/rer.newsletter
 Author: Filippo Campi
 Author-email: filippo.campi@redturtle.it
 License: GPL version 2
 Keywords: Python Plone
 Classifier: Development Status :: 5 - Production/Stable
@@ -204,14 +204,21 @@
 - RedTurtle Technology, sviluppoplone@redturtle.it
 
 
 =========
 Changelog
 =========
 
+2.0.0a3 (2023-07-21)
+--------------------
+
+- Adapt management buttons for Plone 6
+  [pnicolli]
+
+
 2.0.0a2 (2023-03-16)
 --------------------
 
 - Updated subheader template
   [pnicolli]
```

### Comparing `rer.newsletter-2.0.0a2/README.rst` & `rer.newsletter-2.0.0a3/README.rst`

 * *Files identical despite different names*

### Comparing `rer.newsletter-2.0.0a2/docs/rer-logo.png` & `rer.newsletter-2.0.0a3/docs/rer-logo.png`

 * *Files identical despite different names*

### Comparing `rer.newsletter-2.0.0a2/setup.py` & `rer.newsletter-2.0.0a3/setup.py`

 * *Files 2% similar despite different names*

```diff
@@ -12,15 +12,15 @@
         open("CHANGES.rst").read(),
     ]
 )
 
 
 setup(
     name="rer.newsletter",
-    version="2.0.0a2",
+    version="2.0.0a3",
     description="An add-on for Plone",
     long_description=long_description,
     # Get more from https://pypi.python.org/pypi?%3Aaction=list_classifiers
     classifiers=[
         "Development Status :: 5 - Production/Stable",
         "Environment :: Web Environment",
         "Framework :: Plone",
```

### Comparing `rer.newsletter-2.0.0a2/src/rer/newsletter/adapter/configure.zcml` & `rer.newsletter-2.0.0a3/src/rer/newsletter/adapter/configure.zcml`

 * *Files identical despite different names*

### Comparing `rer.newsletter-2.0.0a2/src/rer/newsletter/adapter/sender.py` & `rer.newsletter-2.0.0a3/src/rer/newsletter/adapter/sender.py`

 * *Files identical despite different names*

### Comparing `rer.newsletter-2.0.0a2/src/rer/newsletter/adapter/subscriptions.py` & `rer.newsletter-2.0.0a3/src/rer/newsletter/adapter/subscriptions.py`

 * *Files identical despite different names*

### Comparing `rer.newsletter-2.0.0a2/src/rer/newsletter/behaviors/ships.py` & `rer.newsletter-2.0.0a3/src/rer/newsletter/behaviors/ships.py`

 * *Files identical despite different names*

### Comparing `rer.newsletter-2.0.0a2/src/rer/newsletter/browser/channel/add.py` & `rer.newsletter-2.0.0a3/src/rer/newsletter/browser/channel/add.py`

 * *Files identical despite different names*

### Comparing `rer.newsletter-2.0.0a2/src/rer/newsletter/browser/channel/channelhistory.py` & `rer.newsletter-2.0.0a3/src/rer/newsletter/browser/channel/channelhistory.py`

 * *Files identical despite different names*

### Comparing `rer.newsletter-2.0.0a2/src/rer/newsletter/browser/channel/channelview.py` & `rer.newsletter-2.0.0a3/src/rer/newsletter/browser/channel/channelview.py`

 * *Files identical despite different names*

### Comparing `rer.newsletter-2.0.0a2/src/rer/newsletter/browser/channel/configure.zcml` & `rer.newsletter-2.0.0a3/src/rer/newsletter/browser/channel/configure.zcml`

 * *Files 2% similar despite different names*

```diff
@@ -176,8 +176,17 @@
   <browser:page
       name="delete_expired_users"
       for="*"
       class=".deleteexpiredusers.DeleteExpiredUsersView"
       permission="rer.newsletter.ManageNewsletter"
       />
 
+  <browser:page
+      name="plone_version"
+      for="*"
+      class=".plone_version.PloneVersionView"
+      attribute="is_plone_6_or_above"
+      permission="zope2.View"
+      layer="rer.newsletter.interfaces.IRerNewsletterLayer"
+      />
+
 </configure>
```

### Comparing `rer.newsletter-2.0.0a2/src/rer/newsletter/browser/channel/deleteexpiredusers.py` & `rer.newsletter-2.0.0a3/src/rer/newsletter/browser/channel/deleteexpiredusers.py`

 * *Files identical despite different names*

### Comparing `rer.newsletter-2.0.0a2/src/rer/newsletter/browser/channel/manageusers.py` & `rer.newsletter-2.0.0a3/src/rer/newsletter/browser/channel/manageusers.py`

 * *Files identical despite different names*

### Comparing `rer.newsletter-2.0.0a2/src/rer/newsletter/browser/channel/subscribe.py` & `rer.newsletter-2.0.0a3/src/rer/newsletter/browser/channel/subscribe.py`

 * *Files identical despite different names*

### Comparing `rer.newsletter-2.0.0a2/src/rer/newsletter/browser/channel/templates/channelhistoryview.pt` & `rer.newsletter-2.0.0a3/src/rer/newsletter/browser/channel/templates/channelhistoryview.pt`

 * *Files 11% similar despite different names*

```diff
@@ -27,15 +27,16 @@
            style="display:none;"
       >
         <strong></strong>
       </div>
 
       <div style="margin-bottom: 2%;">
         <span id="delete-message-sent">
-          <span class="plone-btn plone-btn-primary"
+          <span tal:define="plone_6 context/@@plone_version/is_plone_6_or_above"
+                tal:attributes="class python: plone_6 and 'btn btn-primary' or 'plone-btn plone-btn-primary'"
                 i18n:translate="delete_message_sent"
           >
                 Cancella messaggio inviato
           </span>
         </span>
       </div>
```

### Comparing `rer.newsletter-2.0.0a2/src/rer/newsletter/browser/channel/templates/channelview.pt` & `rer.newsletter-2.0.0a3/src/rer/newsletter/browser/channel/templates/channelview.pt`

 * *Files identical despite different names*

### Comparing `rer.newsletter-2.0.0a2/src/rer/newsletter/browser/channel/templates/confirm_subscription.pt` & `rer.newsletter-2.0.0a3/src/rer/newsletter/browser/channel/templates/confirm_subscription.pt`

 * *Files identical despite different names*

### Comparing `rer.newsletter-2.0.0a2/src/rer/newsletter/browser/channel/templates/mail_templates/active_user.pt` & `rer.newsletter-2.0.0a3/src/rer/newsletter/browser/channel/templates/mail_templates/active_user.pt`

 * *Files identical despite different names*

### Comparing `rer.newsletter-2.0.0a2/src/rer/newsletter/browser/channel/templates/mail_templates/active_user_confirm.pt` & `rer.newsletter-2.0.0a3/src/rer/newsletter/browser/channel/templates/mail_templates/active_user_confirm.pt`

 * *Files identical despite different names*

### Comparing `rer.newsletter-2.0.0a2/src/rer/newsletter/browser/channel/templates/mail_templates/asynch_send_fail.pt` & `rer.newsletter-2.0.0a3/src/rer/newsletter/browser/channel/templates/mail_templates/asynch_send_fail.pt`

 * *Files identical despite different names*

### Comparing `rer.newsletter-2.0.0a2/src/rer/newsletter/browser/channel/templates/mail_templates/asynch_send_success.pt` & `rer.newsletter-2.0.0a3/src/rer/newsletter/browser/channel/templates/mail_templates/asynch_send_success.pt`

 * *Files identical despite different names*

### Comparing `rer.newsletter-2.0.0a2/src/rer/newsletter/browser/channel/templates/mail_templates/delete_user.pt` & `rer.newsletter-2.0.0a3/src/rer/newsletter/browser/channel/templates/mail_templates/delete_user.pt`

 * *Files identical despite different names*

### Comparing `rer.newsletter-2.0.0a2/src/rer/newsletter/browser/channel/templates/mail_templates/delete_user_confirm.pt` & `rer.newsletter-2.0.0a3/src/rer/newsletter/browser/channel/templates/mail_templates/delete_user_confirm.pt`

 * *Files identical despite different names*

### Comparing `rer.newsletter-2.0.0a2/src/rer/newsletter/browser/channel/templates/mail_templates/unsubscribe_channel.pt` & `rer.newsletter-2.0.0a3/src/rer/newsletter/browser/channel/templates/mail_templates/unsubscribe_channel.pt`

 * *Files identical despite different names*

### Comparing `rer.newsletter-2.0.0a2/src/rer/newsletter/browser/channel/templates/manageusers.pt` & `rer.newsletter-2.0.0a3/src/rer/newsletter/browser/channel/templates/manageusers.pt`

 * *Files 16% similar despite different names*

```diff
@@ -35,54 +35,54 @@
            href python:context.absolute_url();
          "
          i18n:translate="come_back"
       >
         Come Back
       </a>
 
-      <div id="content-core">
+      <div id="content-core"
+           tal:define="plone_6 context/@@plone_version/is_plone_6_or_above"
+      >
         <div class="portalMessage"
              style="display:none;"
         >
           <strong></strong>
         </div>
 
         <div style="margin-bottom: 2%;">
           <span id="users-import">
-            <a class="plone-btn plone-btn-primary"
+            <a tal:attributes="class python: plone_6 and 'btn btn-primary' or 'plone-btn plone-btn-primary'"
                id="button-import-users"
                href="users_import"
                i18n:translate="import_user_list"
             >
-              <!-- <a href="users_import" class="plone-btn plone-btn-primary pat-plone-modal"
-                data-pat-plone-modal="width: '770px',height: '430px'," i18n:translate="import_user_list"> -->
               Import Users List
             </a>
           </span>
 
           <span id="users-export">
-            <span class="plone-btn plone-btn-primary"
+            <span tal:attributes="class python: plone_6 and 'btn btn-primary' or 'plone-btn plone-btn-primary'"
                   i18n:translate="export_user_list"
             >
               Export Users List
             </span>
           </span>
 
           <span id="add-user">
-            <a class="plone-btn plone-btn-large plone-btn-primary"
+            <a tal:attributes="class python: plone_6 and 'btn btn-large btn-primary' or 'plone-btn plone-btn-large plone-btn-primary'"
                id="button-add-user"
                href="adduser_channel"
                i18n:translate="add_user"
             >
               Add User
             </a>
           </span>
 
           <span id="delete-user">
-            <span class="plone-btn plone-btn-primary"
+            <span tal:attributes="class python: plone_6 and 'btn btn-primary' or 'plone-btn plone-btn-primary'"
                   i18n:translate="delete_user"
             >
               Delete User
             </span>
           </span>
         </div>
```

#### html2text {}

```diff
@@ -1,6 +1,6 @@
 
 ****** Gestione degli Utenti ******
 
  Come Back
- _Import_Users_List    Export Users List    Add_User    Delete User
+ Import_Users_List    Export Users List    Add_User    Delete User
 Email Data di creazione Stato di attivazione
```

### Comparing `rer.newsletter-2.0.0a2/src/rer/newsletter/browser/channel/templates/subscribechannel.pt` & `rer.newsletter-2.0.0a3/src/rer/newsletter/browser/channel/templates/subscribechannel.pt`

 * *Files 5% similar despite different names*

```diff
@@ -9,15 +9,16 @@
 >
 
   <body>
     <metal:main fill-slot="main">
       <metal:main-macro define-macro="main">
 
         <div id="content">
-          <button class="button-plone-modal-close plone-btn"
+          <button tal:define="plone_6 context/@@plone_version/is_plone_6_or_above"
+                  tal:attributes="class python: plone_6 and 'button-plone-modal-close btn' or 'button-plone-modal-close plone-btn'"
                   title="chiudi"
                   type="button"
           >Chiudi</button>
 
           <div class="content_container">
             <div class="informativa"
                  tal:define="
```

### Comparing `rer.newsletter-2.0.0a2/src/rer/newsletter/browser/channel/templates/unsubscribechannel.pt` & `rer.newsletter-2.0.0a3/src/rer/newsletter/browser/channel/templates/unsubscribechannel.pt`

 * *Files 6% similar despite different names*

```diff
@@ -11,15 +11,16 @@
   <body>
     <metal:main fill-slot="main">
       <metal:main-macro define-macro="main">
         <div id="content-core"
              tal:condition="view/form_instance/isVisible"
              tal:content="structure view/contents"
         ></div>
-        <button class="button-plone-modal-close plone-btn"
+        <button tal:define="plone_6 context/@@plone_version/is_plone_6_or_above"
+                tal:attributes="class python: plone_6 and 'button-plone-modal-close btn' or 'button-plone-modal-close plone-btn'"
                 title="chiudi"
                 type="button"
         >Chiudi</button>
         <div class="filter">
           <div class="portalMessage error"
                role="alert"
                tal:condition="not: view/form_instance/isVisible"
```

### Comparing `rer.newsletter-2.0.0a2/src/rer/newsletter/browser/channel/unsubscribe.py` & `rer.newsletter-2.0.0a3/src/rer/newsletter/browser/channel/unsubscribe.py`

 * *Files identical despite different names*

### Comparing `rer.newsletter-2.0.0a2/src/rer/newsletter/browser/channel/users/add.py` & `rer.newsletter-2.0.0a3/src/rer/newsletter/browser/channel/users/add.py`

 * *Files identical despite different names*

### Comparing `rer.newsletter-2.0.0a2/src/rer/newsletter/browser/channel/users/confirm_subscription.py` & `rer.newsletter-2.0.0a3/src/rer/newsletter/browser/channel/users/confirm_subscription.py`

 * *Files identical despite different names*

### Comparing `rer.newsletter-2.0.0a2/src/rer/newsletter/browser/channel/users/usersimport.py` & `rer.newsletter-2.0.0a3/src/rer/newsletter/browser/channel/users/usersimport.py`

 * *Files identical despite different names*

### Comparing `rer.newsletter-2.0.0a2/src/rer/newsletter/browser/configure.zcml` & `rer.newsletter-2.0.0a3/src/rer/newsletter/browser/configure.zcml`

 * *Files identical despite different names*

### Comparing `rer.newsletter-2.0.0a2/src/rer/newsletter/browser/message/checkmessageview.py` & `rer.newsletter-2.0.0a3/src/rer/newsletter/browser/message/checkmessageview.py`

 * *Files identical despite different names*

### Comparing `rer.newsletter-2.0.0a2/src/rer/newsletter/browser/message/configure.zcml` & `rer.newsletter-2.0.0a3/src/rer/newsletter/browser/message/configure.zcml`

 * *Files identical despite different names*

### Comparing `rer.newsletter-2.0.0a2/src/rer/newsletter/browser/message/messagepreview.py` & `rer.newsletter-2.0.0a3/src/rer/newsletter/browser/message/messagepreview.py`

 * *Files identical despite different names*

### Comparing `rer.newsletter-2.0.0a2/src/rer/newsletter/browser/message/messageviewlet.py` & `rer.newsletter-2.0.0a3/src/rer/newsletter/browser/message/messageviewlet.py`

 * *Files identical despite different names*

### Comparing `rer.newsletter-2.0.0a2/src/rer/newsletter/browser/message/sendingtest.py` & `rer.newsletter-2.0.0a3/src/rer/newsletter/browser/message/sendingtest.py`

 * *Files identical despite different names*

### Comparing `rer.newsletter-2.0.0a2/src/rer/newsletter/browser/message/sendmessageview.py` & `rer.newsletter-2.0.0a3/src/rer/newsletter/browser/message/sendmessageview.py`

 * *Files identical despite different names*

### Comparing `rer.newsletter-2.0.0a2/src/rer/newsletter/browser/message/templates/collection_sending_view.pt` & `rer.newsletter-2.0.0a3/src/rer/newsletter/browser/message/templates/collection_sending_view.pt`

 * *Files identical despite different names*

### Comparing `rer.newsletter-2.0.0a2/src/rer/newsletter/browser/message/templates/messagecontentcore.pt` & `rer.newsletter-2.0.0a3/src/rer/newsletter/browser/message/templates/messagecontentcore.pt`

 * *Files identical despite different names*

### Comparing `rer.newsletter-2.0.0a2/src/rer/newsletter/browser/message/templates/messagepreview.pt` & `rer.newsletter-2.0.0a3/src/rer/newsletter/browser/message/templates/messagepreview.pt`

 * *Files identical despite different names*

### Comparing `rer.newsletter-2.0.0a2/src/rer/newsletter/browser/message/templates/messageview.pt` & `rer.newsletter-2.0.0a3/src/rer/newsletter/browser/message/templates/messageview.pt`

 * *Files identical despite different names*

### Comparing `rer.newsletter-2.0.0a2/src/rer/newsletter/browser/message/templates/sendingtest.pt` & `rer.newsletter-2.0.0a3/src/rer/newsletter/browser/message/templates/sendingtest.pt`

 * *Files identical despite different names*

### Comparing `rer.newsletter-2.0.0a2/src/rer/newsletter/browser/message/templates/sendmessageview.pt` & `rer.newsletter-2.0.0a3/src/rer/newsletter/browser/message/templates/sendmessageview.pt`

 * *Files identical despite different names*

### Comparing `rer.newsletter-2.0.0a2/src/rer/newsletter/browser/message/versionview.py` & `rer.newsletter-2.0.0a3/src/rer/newsletter/browser/message/versionview.py`

 * *Files identical despite different names*

### Comparing `rer.newsletter-2.0.0a2/src/rer/newsletter/browser/settings.py` & `rer.newsletter-2.0.0a3/src/rer/newsletter/browser/settings.py`

 * *Files identical despite different names*

### Comparing `rer.newsletter-2.0.0a2/src/rer/newsletter/browser/static/DataTables-1.10.16/.DS_Store` & `rer.newsletter-2.0.0a3/src/rer/newsletter/browser/static/DataTables-1.10.16/.DS_Store`

 * *Files identical despite different names*

### Comparing `rer.newsletter-2.0.0a2/src/rer/newsletter/browser/static/custom.css` & `rer.newsletter-2.0.0a3/src/rer/newsletter/browser/static/custom.css`

 * *Files identical despite different names*

### Comparing `rer.newsletter-2.0.0a2/src/rer/newsletter/browser/static/datatables.css` & `rer.newsletter-2.0.0a3/src/rer/newsletter/browser/static/datatables.css`

 * *Files identical despite different names*

### Comparing `rer.newsletter-2.0.0a2/src/rer/newsletter/browser/static/scripts/channelhistory.js` & `rer.newsletter-2.0.0a3/src/rer/newsletter/browser/static/scripts/channelhistory.js`

 * *Files identical despite different names*

### Comparing `rer.newsletter-2.0.0a2/src/rer/newsletter/browser/static/scripts/datatables.js` & `rer.newsletter-2.0.0a3/src/rer/newsletter/browser/static/scripts/datatables.js`

 * *Files identical despite different names*

### Comparing `rer.newsletter-2.0.0a2/src/rer/newsletter/browser/static/scripts/initializedModal.js` & `rer.newsletter-2.0.0a3/src/rer/newsletter/browser/static/scripts/initializedModal.js`

 * *Files identical despite different names*

### Comparing `rer.newsletter-2.0.0a2/src/rer/newsletter/browser/static/scripts/manageusers.js` & `rer.newsletter-2.0.0a3/src/rer/newsletter/browser/static/scripts/manageusers.js`

 * *Files identical despite different names*

### Comparing `rer.newsletter-2.0.0a2/src/rer/newsletter/configure.zcml` & `rer.newsletter-2.0.0a3/src/rer/newsletter/configure.zcml`

 * *Files identical despite different names*

### Comparing `rer.newsletter-2.0.0a2/src/rer/newsletter/contentrules/actions.py` & `rer.newsletter-2.0.0a3/src/rer/newsletter/contentrules/actions.py`

 * *Files identical despite different names*

### Comparing `rer.newsletter-2.0.0a2/src/rer/newsletter/contentrules/configure.zcml` & `rer.newsletter-2.0.0a3/src/rer/newsletter/contentrules/configure.zcml`

 * *Files identical despite different names*

### Comparing `rer.newsletter-2.0.0a2/src/rer/newsletter/contentrules/events.py` & `rer.newsletter-2.0.0a3/src/rer/newsletter/contentrules/events.py`

 * *Files identical despite different names*

### Comparing `rer.newsletter-2.0.0a2/src/rer/newsletter/contentrules/executors.py` & `rer.newsletter-2.0.0a3/src/rer/newsletter/contentrules/executors.py`

 * *Files identical despite different names*

### Comparing `rer.newsletter-2.0.0a2/src/rer/newsletter/contentrules/forms.py` & `rer.newsletter-2.0.0a3/src/rer/newsletter/contentrules/forms.py`

 * *Files identical despite different names*

### Comparing `rer.newsletter-2.0.0a2/src/rer/newsletter/contentrules/interfaces.py` & `rer.newsletter-2.0.0a3/src/rer/newsletter/contentrules/interfaces.py`

 * *Files identical despite different names*

### Comparing `rer.newsletter-2.0.0a2/src/rer/newsletter/interfaces.py` & `rer.newsletter-2.0.0a3/src/rer/newsletter/interfaces.py`

 * *Files identical despite different names*

### Comparing `rer.newsletter-2.0.0a2/src/rer/newsletter/locales/it/LC_MESSAGES/rer.newsletter.po` & `rer.newsletter-2.0.0a3/src/rer/newsletter/locales/it/LC_MESSAGES/rer.newsletter.po`

 * *Files 1% similar despite different names*

```diff
@@ -346,15 +346,15 @@
 msgstr "Id del canale"
 
 #. Default: "Error parsing CSV file. Probably it has a different separator."
 #: rer/newsletter/browser/channel/users/usersimport.py:171
 msgid "import_error_index"
 msgstr "Errore nella lettura del file CSV. Probabilmente hai selezionato un separatore differente."
 
-#. Default: "<!-- <a href=\"users_import\" class=\"plone-btn plone-btn-primary pat-plone-modal\" data-pat-plone-modal=\"width: '770px',height: '430px',\" i18n:translate=\"import_user_list\"> --> Import Users List"
+#. Default: "Import Users List"
 #: rer/newsletter/browser/channel/templates/manageusers.pt:39
 msgid "import_user_list"
 msgstr "Importa la lista di utenti"
 
 #. Default: "Is Subscribable"
 #: rer/newsletter/interfaces.py:106
 msgid "is_subscribable"
```

### Comparing `rer.newsletter-2.0.0a2/src/rer/newsletter/locales/rer.newsletter.pot` & `rer.newsletter-2.0.0a3/src/rer/newsletter/locales/rer.newsletter.pot`

 * *Files 2% similar despite different names*

```diff
@@ -349,15 +349,15 @@
 msgstr ""
 
 #. Default: "Error parsing CSV file. Probably it has a different separator."
 #: rer/newsletter/browser/channel/users/usersimport.py:171
 msgid "import_error_index"
 msgstr ""
 
-#. Default: "<!-- <a href=\"users_import\" class=\"plone-btn plone-btn-primary pat-plone-modal\" data-pat-plone-modal=\"width: '770px',height: '430px',\" i18n:translate=\"import_user_list\"> --> Import Users List"
+#. Default: "Import Users List"
 #: rer/newsletter/browser/channel/templates/manageusers.pt:39
 msgid "import_user_list"
 msgstr ""
 
 #. Default: "Is Subscribable"
 #: rer/newsletter/interfaces.py:106
 msgid "is_subscribable"
```

### Comparing `rer.newsletter-2.0.0a2/src/rer/newsletter/locales/update.py` & `rer.newsletter-2.0.0a3/src/rer/newsletter/locales/update.py`

 * *Files identical despite different names*

### Comparing `rer.newsletter-2.0.0a2/src/rer/newsletter/portlets/configure.zcml` & `rer.newsletter-2.0.0a3/src/rer/newsletter/portlets/configure.zcml`

 * *Files identical despite different names*

### Comparing `rer.newsletter-2.0.0a2/src/rer/newsletter/portlets/interface.py` & `rer.newsletter-2.0.0a3/src/rer/newsletter/portlets/interface.py`

 * *Files identical despite different names*

### Comparing `rer.newsletter-2.0.0a2/src/rer/newsletter/portlets/subscribe.pt` & `rer.newsletter-2.0.0a3/src/rer/newsletter/portlets/subscribe.pt`

 * *Files 7% similar despite different names*

```diff
@@ -14,24 +14,24 @@
         tal:condition="header"
         tal:content="header"
     >
         Title
     </h4>
   </header>
   <div id="channel-subscribe">
-    <a class="plone-btn plone-btn-primary"
-       href=""
-       style="margin: 1em"
+    <a style="margin: 1em"
        tal:define="
          is_subscribable view/is_subscribable;
          absUrl view/getNewsletterUrl;
+         plone_6 context/@@plone_version/is_plone_6_or_above;
        "
        tal:condition="python:is_subscribable and absUrl"
        tal:attributes="
          href python:absUrl + '/@@subscribe';
+         class python: plone_6 and 'btn btn-primary' or 'plone-btn plone-btn-primary';
        "
        i18n:translate="subscribe"
     >
         Subscribe
     </a>
   </div>
 </section>
```

### Comparing `rer.newsletter-2.0.0a2/src/rer/newsletter/portlets/subscribe.py` & `rer.newsletter-2.0.0a3/src/rer/newsletter/portlets/subscribe.py`

 * *Files identical despite different names*

### Comparing `rer.newsletter-2.0.0a2/src/rer/newsletter/profiles/default/controlpanel.xml` & `rer.newsletter-2.0.0a3/src/rer/newsletter/profiles/default/controlpanel.xml`

 * *Files identical despite different names*

### Comparing `rer.newsletter-2.0.0a2/src/rer/newsletter/profiles/default/registry.xml` & `rer.newsletter-2.0.0a3/src/rer/newsletter/profiles/default/registry.xml`

 * *Files identical despite different names*

### Comparing `rer.newsletter-2.0.0a2/src/rer/newsletter/profiles/default/rolemap.xml` & `rer.newsletter-2.0.0a3/src/rer/newsletter/profiles/default/rolemap.xml`

 * *Files identical despite different names*

### Comparing `rer.newsletter-2.0.0a2/src/rer/newsletter/profiles/default/types/Channel.xml` & `rer.newsletter-2.0.0a3/src/rer/newsletter/profiles/default/types/Channel.xml`

 * *Files identical despite different names*

### Comparing `rer.newsletter-2.0.0a2/src/rer/newsletter/profiles/default/types/Message.xml` & `rer.newsletter-2.0.0a3/src/rer/newsletter/profiles/default/types/Message.xml`

 * *Files identical despite different names*

### Comparing `rer.newsletter-2.0.0a2/src/rer/newsletter/profiles/default/types/Shippable_Collection.xml` & `rer.newsletter-2.0.0a3/src/rer/newsletter/profiles/default/types/Shippable_Collection.xml`

 * *Files identical despite different names*

### Comparing `rer.newsletter-2.0.0a2/src/rer/newsletter/profiles/default/workflows/channel_workflow/definition.xml` & `rer.newsletter-2.0.0a3/src/rer/newsletter/profiles/default/workflows/channel_workflow/definition.xml`

 * *Files identical despite different names*

### Comparing `rer.newsletter-2.0.0a2/src/rer/newsletter/profiles/default/workflows/message_workflow/definition.xml` & `rer.newsletter-2.0.0a3/src/rer/newsletter/profiles/default/workflows/message_workflow/definition.xml`

 * *Files identical despite different names*

### Comparing `rer.newsletter-2.0.0a2/src/rer/newsletter/profiles/default/workflows.xml` & `rer.newsletter-2.0.0a3/src/rer/newsletter/profiles/default/workflows.xml`

 * *Files identical despite different names*

### Comparing `rer.newsletter-2.0.0a2/src/rer/newsletter/profiles/uninstall/actions.xml` & `rer.newsletter-2.0.0a3/src/rer/newsletter/profiles/uninstall/actions.xml`

 * *Files identical despite different names*

### Comparing `rer.newsletter-2.0.0a2/src/rer/newsletter/profiles/uninstall/registry.xml` & `rer.newsletter-2.0.0a3/src/rer/newsletter/profiles/uninstall/registry.xml`

 * *Files identical despite different names*

### Comparing `rer.newsletter-2.0.0a2/src/rer/newsletter/queue/handler.py` & `rer.newsletter-2.0.0a3/src/rer/newsletter/queue/handler.py`

 * *Files identical despite different names*

### Comparing `rer.newsletter-2.0.0a2/src/rer/newsletter/queue/view.py` & `rer.newsletter-2.0.0a3/src/rer/newsletter/queue/view.py`

 * *Files identical despite different names*

### Comparing `rer.newsletter-2.0.0a2/src/rer/newsletter/restapi/services/configure.zcml` & `rer.newsletter-2.0.0a3/src/rer/newsletter/restapi/services/configure.zcml`

 * *Files identical despite different names*

### Comparing `rer.newsletter-2.0.0a2/src/rer/newsletter/restapi/services/confirm_subscription.py` & `rer.newsletter-2.0.0a3/src/rer/newsletter/restapi/services/confirm_subscription.py`

 * *Files identical despite different names*

### Comparing `rer.newsletter-2.0.0a2/src/rer/newsletter/restapi/services/subscribe.py` & `rer.newsletter-2.0.0a3/src/rer/newsletter/restapi/services/subscribe.py`

 * *Files identical despite different names*

### Comparing `rer.newsletter-2.0.0a2/src/rer/newsletter/restapi/services/unsubscribe.py` & `rer.newsletter-2.0.0a3/src/rer/newsletter/restapi/services/unsubscribe.py`

 * *Files identical despite different names*

### Comparing `rer.newsletter-2.0.0a2/src/rer/newsletter/setuphandlers.py` & `rer.newsletter-2.0.0a3/src/rer/newsletter/setuphandlers.py`

 * *Files identical despite different names*

### Comparing `rer.newsletter-2.0.0a2/src/rer/newsletter/testing.py` & `rer.newsletter-2.0.0a3/src/rer/newsletter/testing.py`

 * *Files identical despite different names*

### Comparing `rer.newsletter-2.0.0a2/src/rer/newsletter/tests/test_setup.py` & `rer.newsletter-2.0.0a3/src/rer/newsletter/tests/test_setup.py`

 * *Files identical despite different names*

### Comparing `rer.newsletter-2.0.0a2/src/rer/newsletter/tests/test_subscription_tile.py` & `rer.newsletter-2.0.0a3/src/rer/newsletter/tests/test_subscription_tile.py`

 * *Files identical despite different names*

### Comparing `rer.newsletter-2.0.0a2/src/rer/newsletter/tests/test_subscriptions_adapter.py` & `rer.newsletter-2.0.0a3/src/rer/newsletter/tests/test_subscriptions_adapter.py`

 * *Files identical despite different names*

### Comparing `rer.newsletter-2.0.0a2/src/rer/newsletter/tiles/configure.zcml` & `rer.newsletter-2.0.0a3/src/rer/newsletter/tiles/configure.zcml`

 * *Files identical despite different names*

### Comparing `rer.newsletter-2.0.0a2/src/rer/newsletter/tiles/subscribe.pt` & `rer.newsletter-2.0.0a3/src/rer/newsletter/tiles/subscribe.pt`

 * *Files 7% similar despite different names*

```diff
@@ -16,23 +16,23 @@
         <h3 class="tileTitle"
             tal:condition="view/data/header"
         >
                     ${view/data/header}
         </h3>
         <div class="tileBody">
           <div id="channel-subscribe">
-            <a class="plone-btn plone-btn-primary"
-               href="#"
-               tal:define="
+            <a tal:define="
                  is_subscribable view/is_subscribable;
                  absUrl view/getNewsletterUrl;
+                 plone_6 context/@@plone_version/is_plone_6_or_above;
                "
                tal:condition="python:is_subscribable and absUrl"
                tal:attributes="
                  href python:absUrl + '/@@subscribe';
+                 class python: plone_6 and 'btn btn-primary' or 'plone-btn plone-btn-primary';
                "
                i18n:translate="subscribe"
             >
                             Subscribe
             </a>
           </div>
         </div>
```

### Comparing `rer.newsletter-2.0.0a2/src/rer/newsletter/tiles/subscribe.py` & `rer.newsletter-2.0.0a3/src/rer/newsletter/tiles/subscribe.py`

 * *Files identical despite different names*

### Comparing `rer.newsletter-2.0.0a2/src/rer/newsletter/transforms/link_transform.py` & `rer.newsletter-2.0.0a3/src/rer/newsletter/transforms/link_transform.py`

 * *Files identical despite different names*

### Comparing `rer.newsletter-2.0.0a2/src/rer/newsletter/upgrades.py` & `rer.newsletter-2.0.0a3/src/rer/newsletter/upgrades.py`

 * *Files identical despite different names*

### Comparing `rer.newsletter-2.0.0a2/src/rer/newsletter/upgrades.zcml` & `rer.newsletter-2.0.0a3/src/rer/newsletter/upgrades.zcml`

 * *Files identical despite different names*

### Comparing `rer.newsletter-2.0.0a2/src/rer/newsletter/utils.py` & `rer.newsletter-2.0.0a3/src/rer/newsletter/utils.py`

 * *Files identical despite different names*

### Comparing `rer.newsletter-2.0.0a2/src/rer/newsletter/vocabularies.py` & `rer.newsletter-2.0.0a3/src/rer/newsletter/vocabularies.py`

 * *Files identical despite different names*

### Comparing `rer.newsletter-2.0.0a2/src/rer.newsletter.egg-info/PKG-INFO` & `rer.newsletter-2.0.0a3/src/rer.newsletter.egg-info/PKG-INFO`

 * *Files 2% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: rer.newsletter
-Version: 2.0.0a2
+Version: 2.0.0a3
 Summary: An add-on for Plone
 Home-page: https://pypi.python.org/pypi/rer.newsletter
 Author: Filippo Campi
 Author-email: filippo.campi@redturtle.it
 License: GPL version 2
 Keywords: Python Plone
 Classifier: Development Status :: 5 - Production/Stable
@@ -204,14 +204,21 @@
 - RedTurtle Technology, sviluppoplone@redturtle.it
 
 
 =========
 Changelog
 =========
 
+2.0.0a3 (2023-07-21)
+--------------------
+
+- Adapt management buttons for Plone 6
+  [pnicolli]
+
+
 2.0.0a2 (2023-03-16)
 --------------------
 
 - Updated subheader template
   [pnicolli]
```

### Comparing `rer.newsletter-2.0.0a2/src/rer.newsletter.egg-info/SOURCES.txt` & `rer.newsletter-2.0.0a3/src/rer.newsletter.egg-info/SOURCES.txt`

 * *Files 1% similar despite different names*

```diff
@@ -46,14 +46,15 @@
 src/rer/newsletter/browser/channel/add.py
 src/rer/newsletter/browser/channel/channelhistory.py
 src/rer/newsletter/browser/channel/channelview.py
 src/rer/newsletter/browser/channel/channelviewlet.py
 src/rer/newsletter/browser/channel/configure.zcml
 src/rer/newsletter/browser/channel/deleteexpiredusers.py
 src/rer/newsletter/browser/channel/manageusers.py
+src/rer/newsletter/browser/channel/plone_version.py
 src/rer/newsletter/browser/channel/subscribe.py
 src/rer/newsletter/browser/channel/unsubscribe.py
 src/rer/newsletter/browser/channel/templates/channelhistoryview.pt
 src/rer/newsletter/browser/channel/templates/channelview.pt
 src/rer/newsletter/browser/channel/templates/channelviewlet.pt
 src/rer/newsletter/browser/channel/templates/confirm_subscription.pt
 src/rer/newsletter/browser/channel/templates/manageusers.pt
```

