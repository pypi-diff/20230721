# Comparing `tmp/allianceauth-discordbot-3.6.2.tar.gz` & `tmp/allianceauth-discordbot-3.6.3.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "allianceauth-discordbot-3.6.2.tar", last modified: Tue Jun 27 23:30:52 2023, max compression
+gzip compressed data, was "allianceauth-discordbot-3.6.3.tar", last modified: Fri Jul 21 09:20:09 2023, max compression
```

## Comparing `allianceauth-discordbot-3.6.2.tar` & `allianceauth-discordbot-3.6.3.tar`

### file list

```diff
@@ -1,63 +1,66 @@
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-27 23:30:51.992964 allianceauth-discordbot-3.6.2/
--rw-r--r--   0 runner    (1001) docker     (123)      109 2023-06-27 23:30:02.000000 allianceauth-discordbot-3.6.2/MANIFEST.in
--rw-r--r--   0 runner    (1001) docker     (123)    14900 2023-06-27 23:30:51.992964 allianceauth-discordbot-3.6.2/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (123)    13993 2023-06-27 23:30:02.000000 allianceauth-discordbot-3.6.2/README.md
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-27 23:30:51.988964 allianceauth-discordbot-3.6.2/aadiscordbot/
--rw-r--r--   0 runner    (1001) docker     (123)      134 2023-06-27 23:30:02.000000 allianceauth-discordbot-3.6.2/aadiscordbot/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)     1854 2023-06-27 23:30:02.000000 allianceauth-discordbot-3.6.2/aadiscordbot/admin.py
--rw-r--r--   0 runner    (1001) docker     (123)     3768 2023-06-27 23:30:02.000000 allianceauth-discordbot-3.6.2/aadiscordbot/app_settings.py
--rw-r--r--   0 runner    (1001) docker     (123)      263 2023-06-27 23:30:02.000000 allianceauth-discordbot-3.6.2/aadiscordbot/apps.py
--rw-r--r--   0 runner    (1001) docker     (123)      928 2023-06-27 23:30:02.000000 allianceauth-discordbot-3.6.2/aadiscordbot/auth_hooks.py
--rw-r--r--   0 runner    (1001) docker     (123)    17002 2023-06-27 23:30:02.000000 allianceauth-discordbot-3.6.2/aadiscordbot/bot.py
--rw-r--r--   0 runner    (1001) docker     (123)     4126 2023-06-27 23:30:02.000000 allianceauth-discordbot-3.6.2/aadiscordbot/bot_tasks.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-27 23:30:51.988964 allianceauth-discordbot-3.6.2/aadiscordbot/cogs/
--rw-r--r--   0 runner    (1001) docker     (123)        0 2023-06-27 23:30:02.000000 allianceauth-discordbot-3.6.2/aadiscordbot/cogs/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)     3261 2023-06-27 23:30:02.000000 allianceauth-discordbot-3.6.2/aadiscordbot/cogs/about.py
--rw-r--r--   0 runner    (1001) docker     (123)     2931 2023-06-27 23:30:02.000000 allianceauth-discordbot-3.6.2/aadiscordbot/cogs/abuse.py
--rw-r--r--   0 runner    (1001) docker     (123)    16421 2023-06-27 23:30:02.000000 allianceauth-discordbot-3.6.2/aadiscordbot/cogs/admin.py
--rw-r--r--   0 runner    (1001) docker     (123)     2694 2023-06-27 23:30:02.000000 allianceauth-discordbot-3.6.2/aadiscordbot/cogs/auth.py
--rw-r--r--   0 runner    (1001) docker     (123)      909 2023-06-27 23:30:02.000000 allianceauth-discordbot-3.6.2/aadiscordbot/cogs/eastereggs.py
--rw-r--r--   0 runner    (1001) docker     (123)     1459 2023-06-27 23:30:02.000000 allianceauth-discordbot-3.6.2/aadiscordbot/cogs/eightball.py
--rw-r--r--   0 runner    (1001) docker     (123)     3827 2023-06-27 23:30:02.000000 allianceauth-discordbot-3.6.2/aadiscordbot/cogs/facwar.py
--rw-r--r--   0 runner    (1001) docker     (123)    12559 2023-06-27 23:30:02.000000 allianceauth-discordbot-3.6.2/aadiscordbot/cogs/members.py
--rw-r--r--   0 runner    (1001) docker     (123)     3531 2023-06-27 23:30:02.000000 allianceauth-discordbot-3.6.2/aadiscordbot/cogs/models.py
--rw-r--r--   0 runner    (1001) docker     (123)     5632 2023-06-27 23:30:02.000000 allianceauth-discordbot-3.6.2/aadiscordbot/cogs/price_check.py
--rw-r--r--   0 runner    (1001) docker     (123)     1495 2023-06-27 23:30:02.000000 allianceauth-discordbot-3.6.2/aadiscordbot/cogs/prom_export.py
--rw-r--r--   0 runner    (1001) docker     (123)     5180 2023-06-27 23:30:02.000000 allianceauth-discordbot-3.6.2/aadiscordbot/cogs/quote.py
--rw-r--r--   0 runner    (1001) docker     (123)     6214 2023-06-27 23:30:02.000000 allianceauth-discordbot-3.6.2/aadiscordbot/cogs/reaction_roles.py
--rw-r--r--   0 runner    (1001) docker     (123)     1105 2023-06-27 23:30:02.000000 allianceauth-discordbot-3.6.2/aadiscordbot/cogs/remind.py
--rw-r--r--   0 runner    (1001) docker     (123)     6532 2023-06-27 23:30:02.000000 allianceauth-discordbot-3.6.2/aadiscordbot/cogs/services.py
--rw-r--r--   0 runner    (1001) docker     (123)    15830 2023-06-27 23:30:02.000000 allianceauth-discordbot-3.6.2/aadiscordbot/cogs/sov.py
--rw-r--r--   0 runner    (1001) docker     (123)     1396 2023-06-27 23:30:02.000000 allianceauth-discordbot-3.6.2/aadiscordbot/cogs/time.py
--rw-r--r--   0 runner    (1001) docker     (123)     2171 2023-06-27 23:30:02.000000 allianceauth-discordbot-3.6.2/aadiscordbot/cogs/timers.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-27 23:30:51.992964 allianceauth-discordbot-3.6.2/aadiscordbot/cogs/utils/
--rw-r--r--   0 runner    (1001) docker     (123)        0 2023-06-27 23:30:02.000000 allianceauth-discordbot-3.6.2/aadiscordbot/cogs/utils/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)      207 2023-06-27 23:30:02.000000 allianceauth-discordbot-3.6.2/aadiscordbot/cogs/utils/context.py
--rw-r--r--   0 runner    (1001) docker     (123)     3883 2023-06-27 23:30:02.000000 allianceauth-discordbot-3.6.2/aadiscordbot/cogs/utils/decorators.py
--rw-r--r--   0 runner    (1001) docker     (123)      437 2023-06-27 23:30:02.000000 allianceauth-discordbot-3.6.2/aadiscordbot/cogs/utils/exceptions.py
--rw-r--r--   0 runner    (1001) docker     (123)     4373 2023-06-27 23:30:02.000000 allianceauth-discordbot-3.6.2/aadiscordbot/cogs/welcomegoodbye.py
--rw-r--r--   0 runner    (1001) docker     (123)      235 2023-06-27 23:30:02.000000 allianceauth-discordbot-3.6.2/aadiscordbot/launcher.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-27 23:30:51.992964 allianceauth-discordbot-3.6.2/aadiscordbot/migrations/
--rw-r--r--   0 runner    (1001) docker     (123)     1621 2023-06-27 23:30:02.000000 allianceauth-discordbot-3.6.2/aadiscordbot/migrations/0001_initial.py
--rw-r--r--   0 runner    (1001) docker     (123)     1410 2023-06-27 23:30:02.000000 allianceauth-discordbot-3.6.2/aadiscordbot/migrations/0002_reactionrolebinding_reactionrolemessage.py
--rw-r--r--   0 runner    (1001) docker     (123)      636 2023-06-27 23:30:02.000000 allianceauth-discordbot-3.6.2/aadiscordbot/migrations/0003_authbotconfiguration.py
--rw-r--r--   0 runner    (1001) docker     (123)      485 2023-06-27 23:30:02.000000 allianceauth-discordbot-3.6.2/aadiscordbot/migrations/0004_settings.py
--rw-r--r--   0 runner    (1001) docker     (123)      759 2023-06-27 23:30:02.000000 allianceauth-discordbot-3.6.2/aadiscordbot/migrations/0005_rr_fixes_blank_admins.py
--rw-r--r--   0 runner    (1001) docker     (123)     1773 2023-06-27 23:30:02.000000 allianceauth-discordbot-3.6.2/aadiscordbot/migrations/0006_goodbyemessage_welcomemessage.py
--rw-r--r--   0 runner    (1001) docker     (123)     1219 2023-06-27 23:30:02.000000 allianceauth-discordbot-3.6.2/aadiscordbot/migrations/0007_quotemessage.py
--rw-r--r--   0 runner    (1001) docker     (123)      413 2023-06-27 23:30:02.000000 allianceauth-discordbot-3.6.2/aadiscordbot/migrations/0008_channels_deleted.py
--rw-r--r--   0 runner    (1001) docker     (123)      507 2023-06-27 23:30:02.000000 allianceauth-discordbot-3.6.2/aadiscordbot/migrations/0009_alter_quotemessage_options.py
--rw-r--r--   0 runner    (1001) docker     (123)        0 2023-06-27 23:30:02.000000 allianceauth-discordbot-3.6.2/aadiscordbot/migrations/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)     4556 2023-06-27 23:30:02.000000 allianceauth-discordbot-3.6.2/aadiscordbot/models.py
--rw-r--r--   0 runner    (1001) docker     (123)      317 2023-06-27 23:30:02.000000 allianceauth-discordbot-3.6.2/aadiscordbot/providers.py
--rw-r--r--   0 runner    (1001) docker     (123)     3628 2023-06-27 23:30:02.000000 allianceauth-discordbot-3.6.2/aadiscordbot/tasks.py
--rw-r--r--   0 runner    (1001) docker     (123)       45 2023-06-27 23:30:02.000000 allianceauth-discordbot-3.6.2/aadiscordbot/urls.py
--rw-r--r--   0 runner    (1001) docker     (123)       15 2023-06-27 23:30:02.000000 allianceauth-discordbot-3.6.2/aadiscordbot/views.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-27 23:30:51.992964 allianceauth-discordbot-3.6.2/allianceauth_discordbot.egg-info/
--rw-r--r--   0 runner    (1001) docker     (123)    14900 2023-06-27 23:30:51.000000 allianceauth-discordbot-3.6.2/allianceauth_discordbot.egg-info/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (123)     1818 2023-06-27 23:30:51.000000 allianceauth-discordbot-3.6.2/allianceauth_discordbot.egg-info/SOURCES.txt
--rw-r--r--   0 runner    (1001) docker     (123)        1 2023-06-27 23:30:51.000000 allianceauth-discordbot-3.6.2/allianceauth_discordbot.egg-info/dependency_links.txt
--rw-r--r--   0 runner    (1001) docker     (123)       91 2023-06-27 23:30:51.000000 allianceauth-discordbot-3.6.2/allianceauth_discordbot.egg-info/requires.txt
--rw-r--r--   0 runner    (1001) docker     (123)       13 2023-06-27 23:30:51.000000 allianceauth-discordbot-3.6.2/allianceauth_discordbot.egg-info/top_level.txt
--rw-r--r--   0 runner    (1001) docker     (123)       38 2023-06-27 23:30:51.992964 allianceauth-discordbot-3.6.2/setup.cfg
--rw-r--r--   0 runner    (1001) docker     (123)     1516 2023-06-27 23:30:02.000000 allianceauth-discordbot-3.6.2/setup.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-21 09:20:09.894833 allianceauth-discordbot-3.6.3/
+-rw-r--r--   0 runner    (1001) docker     (123)      109 2023-07-21 09:19:22.000000 allianceauth-discordbot-3.6.3/MANIFEST.in
+-rw-r--r--   0 runner    (1001) docker     (123)    14977 2023-07-21 09:20:09.894833 allianceauth-discordbot-3.6.3/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (123)    14070 2023-07-21 09:19:22.000000 allianceauth-discordbot-3.6.3/README.md
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-21 09:20:09.890833 allianceauth-discordbot-3.6.3/aadiscordbot/
+-rw-r--r--   0 runner    (1001) docker     (123)      134 2023-07-21 09:19:22.000000 allianceauth-discordbot-3.6.3/aadiscordbot/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1977 2023-07-21 09:19:22.000000 allianceauth-discordbot-3.6.3/aadiscordbot/admin.py
+-rw-r--r--   0 runner    (1001) docker     (123)     3857 2023-07-21 09:19:22.000000 allianceauth-discordbot-3.6.3/aadiscordbot/app_settings.py
+-rw-r--r--   0 runner    (1001) docker     (123)      263 2023-07-21 09:19:22.000000 allianceauth-discordbot-3.6.3/aadiscordbot/apps.py
+-rw-r--r--   0 runner    (1001) docker     (123)      928 2023-07-21 09:19:22.000000 allianceauth-discordbot-3.6.3/aadiscordbot/auth_hooks.py
+-rw-r--r--   0 runner    (1001) docker     (123)    17002 2023-07-21 09:19:22.000000 allianceauth-discordbot-3.6.3/aadiscordbot/bot.py
+-rw-r--r--   0 runner    (1001) docker     (123)     4126 2023-07-21 09:19:22.000000 allianceauth-discordbot-3.6.3/aadiscordbot/bot_tasks.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-21 09:20:09.890833 allianceauth-discordbot-3.6.3/aadiscordbot/cogs/
+-rw-r--r--   0 runner    (1001) docker     (123)        0 2023-07-21 09:19:22.000000 allianceauth-discordbot-3.6.3/aadiscordbot/cogs/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)     3261 2023-07-21 09:19:22.000000 allianceauth-discordbot-3.6.3/aadiscordbot/cogs/about.py
+-rw-r--r--   0 runner    (1001) docker     (123)     2931 2023-07-21 09:19:22.000000 allianceauth-discordbot-3.6.3/aadiscordbot/cogs/abuse.py
+-rw-r--r--   0 runner    (1001) docker     (123)    16421 2023-07-21 09:19:22.000000 allianceauth-discordbot-3.6.3/aadiscordbot/cogs/admin.py
+-rw-r--r--   0 runner    (1001) docker     (123)     2694 2023-07-21 09:19:22.000000 allianceauth-discordbot-3.6.3/aadiscordbot/cogs/auth.py
+-rw-r--r--   0 runner    (1001) docker     (123)      909 2023-07-21 09:19:22.000000 allianceauth-discordbot-3.6.3/aadiscordbot/cogs/eastereggs.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1459 2023-07-21 09:19:22.000000 allianceauth-discordbot-3.6.3/aadiscordbot/cogs/eightball.py
+-rw-r--r--   0 runner    (1001) docker     (123)     3827 2023-07-21 09:19:22.000000 allianceauth-discordbot-3.6.3/aadiscordbot/cogs/facwar.py
+-rw-r--r--   0 runner    (1001) docker     (123)    12709 2023-07-21 09:19:22.000000 allianceauth-discordbot-3.6.3/aadiscordbot/cogs/members.py
+-rw-r--r--   0 runner    (1001) docker     (123)     3531 2023-07-21 09:19:22.000000 allianceauth-discordbot-3.6.3/aadiscordbot/cogs/models.py
+-rw-r--r--   0 runner    (1001) docker     (123)     5703 2023-07-21 09:19:22.000000 allianceauth-discordbot-3.6.3/aadiscordbot/cogs/price_check.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1495 2023-07-21 09:19:22.000000 allianceauth-discordbot-3.6.3/aadiscordbot/cogs/prom_export.py
+-rw-r--r--   0 runner    (1001) docker     (123)     5180 2023-07-21 09:19:22.000000 allianceauth-discordbot-3.6.3/aadiscordbot/cogs/quote.py
+-rw-r--r--   0 runner    (1001) docker     (123)     6214 2023-07-21 09:19:22.000000 allianceauth-discordbot-3.6.3/aadiscordbot/cogs/reaction_roles.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1105 2023-07-21 09:19:22.000000 allianceauth-discordbot-3.6.3/aadiscordbot/cogs/remind.py
+-rw-r--r--   0 runner    (1001) docker     (123)     6532 2023-07-21 09:19:22.000000 allianceauth-discordbot-3.6.3/aadiscordbot/cogs/services.py
+-rw-r--r--   0 runner    (1001) docker     (123)    15830 2023-07-21 09:19:22.000000 allianceauth-discordbot-3.6.3/aadiscordbot/cogs/sov.py
+-rw-r--r--   0 runner    (1001) docker     (123)     4070 2023-07-21 09:19:22.000000 allianceauth-discordbot-3.6.3/aadiscordbot/cogs/tickets.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1396 2023-07-21 09:19:22.000000 allianceauth-discordbot-3.6.3/aadiscordbot/cogs/time.py
+-rw-r--r--   0 runner    (1001) docker     (123)     2171 2023-07-21 09:19:22.000000 allianceauth-discordbot-3.6.3/aadiscordbot/cogs/timers.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-21 09:20:09.890833 allianceauth-discordbot-3.6.3/aadiscordbot/cogs/utils/
+-rw-r--r--   0 runner    (1001) docker     (123)        0 2023-07-21 09:19:22.000000 allianceauth-discordbot-3.6.3/aadiscordbot/cogs/utils/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)      207 2023-07-21 09:19:22.000000 allianceauth-discordbot-3.6.3/aadiscordbot/cogs/utils/context.py
+-rw-r--r--   0 runner    (1001) docker     (123)     3883 2023-07-21 09:19:22.000000 allianceauth-discordbot-3.6.3/aadiscordbot/cogs/utils/decorators.py
+-rw-r--r--   0 runner    (1001) docker     (123)      437 2023-07-21 09:19:22.000000 allianceauth-discordbot-3.6.3/aadiscordbot/cogs/utils/exceptions.py
+-rw-r--r--   0 runner    (1001) docker     (123)     4373 2023-07-21 09:19:22.000000 allianceauth-discordbot-3.6.3/aadiscordbot/cogs/welcomegoodbye.py
+-rw-r--r--   0 runner    (1001) docker     (123)      235 2023-07-21 09:19:22.000000 allianceauth-discordbot-3.6.3/aadiscordbot/launcher.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-21 09:20:09.894833 allianceauth-discordbot-3.6.3/aadiscordbot/migrations/
+-rw-r--r--   0 runner    (1001) docker     (123)     1621 2023-07-21 09:19:22.000000 allianceauth-discordbot-3.6.3/aadiscordbot/migrations/0001_initial.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1410 2023-07-21 09:19:22.000000 allianceauth-discordbot-3.6.3/aadiscordbot/migrations/0002_reactionrolebinding_reactionrolemessage.py
+-rw-r--r--   0 runner    (1001) docker     (123)      636 2023-07-21 09:19:22.000000 allianceauth-discordbot-3.6.3/aadiscordbot/migrations/0003_authbotconfiguration.py
+-rw-r--r--   0 runner    (1001) docker     (123)      485 2023-07-21 09:19:22.000000 allianceauth-discordbot-3.6.3/aadiscordbot/migrations/0004_settings.py
+-rw-r--r--   0 runner    (1001) docker     (123)      759 2023-07-21 09:19:22.000000 allianceauth-discordbot-3.6.3/aadiscordbot/migrations/0005_rr_fixes_blank_admins.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1773 2023-07-21 09:19:22.000000 allianceauth-discordbot-3.6.3/aadiscordbot/migrations/0006_goodbyemessage_welcomemessage.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1219 2023-07-21 09:19:22.000000 allianceauth-discordbot-3.6.3/aadiscordbot/migrations/0007_quotemessage.py
+-rw-r--r--   0 runner    (1001) docker     (123)      413 2023-07-21 09:19:22.000000 allianceauth-discordbot-3.6.3/aadiscordbot/migrations/0008_channels_deleted.py
+-rw-r--r--   0 runner    (1001) docker     (123)      507 2023-07-21 09:19:22.000000 allianceauth-discordbot-3.6.3/aadiscordbot/migrations/0009_alter_quotemessage_options.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1056 2023-07-21 09:19:22.000000 allianceauth-discordbot-3.6.3/aadiscordbot/migrations/0010_alter_discordbot_options_ticketgroups.py
+-rw-r--r--   0 runner    (1001) docker     (123)      805 2023-07-21 09:19:22.000000 allianceauth-discordbot-3.6.3/aadiscordbot/migrations/0011_alter_ticketgroups_options_and_more.py
+-rw-r--r--   0 runner    (1001) docker     (123)        0 2023-07-21 09:19:22.000000 allianceauth-discordbot-3.6.3/aadiscordbot/migrations/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)     5148 2023-07-21 09:19:22.000000 allianceauth-discordbot-3.6.3/aadiscordbot/models.py
+-rw-r--r--   0 runner    (1001) docker     (123)      317 2023-07-21 09:19:22.000000 allianceauth-discordbot-3.6.3/aadiscordbot/providers.py
+-rw-r--r--   0 runner    (1001) docker     (123)     3628 2023-07-21 09:19:22.000000 allianceauth-discordbot-3.6.3/aadiscordbot/tasks.py
+-rw-r--r--   0 runner    (1001) docker     (123)       45 2023-07-21 09:19:22.000000 allianceauth-discordbot-3.6.3/aadiscordbot/urls.py
+-rw-r--r--   0 runner    (1001) docker     (123)       15 2023-07-21 09:19:22.000000 allianceauth-discordbot-3.6.3/aadiscordbot/views.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-21 09:20:09.894833 allianceauth-discordbot-3.6.3/allianceauth_discordbot.egg-info/
+-rw-r--r--   0 runner    (1001) docker     (123)    14977 2023-07-21 09:20:09.000000 allianceauth-discordbot-3.6.3/allianceauth_discordbot.egg-info/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (123)     1985 2023-07-21 09:20:09.000000 allianceauth-discordbot-3.6.3/allianceauth_discordbot.egg-info/SOURCES.txt
+-rw-r--r--   0 runner    (1001) docker     (123)        1 2023-07-21 09:20:09.000000 allianceauth-discordbot-3.6.3/allianceauth_discordbot.egg-info/dependency_links.txt
+-rw-r--r--   0 runner    (1001) docker     (123)       91 2023-07-21 09:20:09.000000 allianceauth-discordbot-3.6.3/allianceauth_discordbot.egg-info/requires.txt
+-rw-r--r--   0 runner    (1001) docker     (123)       13 2023-07-21 09:20:09.000000 allianceauth-discordbot-3.6.3/allianceauth_discordbot.egg-info/top_level.txt
+-rw-r--r--   0 runner    (1001) docker     (123)       38 2023-07-21 09:20:09.894833 allianceauth-discordbot-3.6.3/setup.cfg
+-rw-r--r--   0 runner    (1001) docker     (123)     1516 2023-07-21 09:19:22.000000 allianceauth-discordbot-3.6.3/setup.py
```

### Comparing `allianceauth-discordbot-3.6.2/PKG-INFO` & `allianceauth-discordbot-3.6.3/PKG-INFO`

 * *Files 2% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: allianceauth-discordbot
-Version: 3.6.2
+Version: 3.6.3
 Summary: Alliance Auth Discord Bot
 Home-page: https://github.com/pvyParts/allianceauth-discordbot
 Author: ak
 Author-email: ak@ak.auth
 License: GNU General Public License v3 (GPLv3)
 Platform: UNKNOWN
 Classifier: Environment :: Web Environment
@@ -102,14 +102,16 @@
 
 DISCORD_BOT_SOV_STRUCTURE_OWNER_IDS = [1000169] # Centre for Advanced Studies example
 DISCORD_BOT_MEMBER_ALLIANCES = [111, 222, 333] # A list of alliances to be considered "Mains"
 
 DISCORD_BOT_ADM_REGIONS = [10000002] # The Forge Example
 DISCORD_BOT_ADM_SYSTEMS = [30000142] # Jita Example
 DISCORD_BOT_ADM_CONSTELLATIONS = [20000020] # Kimitoro Example
+
+PRICE_CHECK_HOSTNAME = "evepraisal.com" # Point to your favorite evepraisal
 ```
 
 ```python
 ## Insert AADiscordBot's logging into Django Logging config
 LOGGING['handlers']['bot_log_file']= {
             'level': 'INFO',
             'class': 'logging.handlers.RotatingFileHandler',
```

### Comparing `allianceauth-discordbot-3.6.2/README.md` & `allianceauth-discordbot-3.6.3/README.md`

 * *Files 1% similar despite different names*

```diff
@@ -78,14 +78,16 @@
 
 DISCORD_BOT_SOV_STRUCTURE_OWNER_IDS = [1000169] # Centre for Advanced Studies example
 DISCORD_BOT_MEMBER_ALLIANCES = [111, 222, 333] # A list of alliances to be considered "Mains"
 
 DISCORD_BOT_ADM_REGIONS = [10000002] # The Forge Example
 DISCORD_BOT_ADM_SYSTEMS = [30000142] # Jita Example
 DISCORD_BOT_ADM_CONSTELLATIONS = [20000020] # Kimitoro Example
+
+PRICE_CHECK_HOSTNAME = "evepraisal.com" # Point to your favorite evepraisal
 ```
 
 ```python
 ## Insert AADiscordBot's logging into Django Logging config
 LOGGING['handlers']['bot_log_file']= {
             'level': 'INFO',
             'class': 'logging.handlers.RotatingFileHandler',
```

### Comparing `allianceauth-discordbot-3.6.2/aadiscordbot/admin.py` & `allianceauth-discordbot-3.6.3/aadiscordbot/admin.py`

 * *Files 12% similar despite different names*

```diff
@@ -1,14 +1,14 @@
 from django.contrib import admin
 
 from allianceauth.services.hooks import get_extension_logger
 
 from .models import (
     AuthBotConfiguration, Channels, GoodbyeMessage, ReactionRoleBinding,
-    ReactionRoleMessage, Servers, WelcomeMessage,
+    ReactionRoleMessage, Servers, TicketGroups, WelcomeMessage,
 )
 
 logger = get_extension_logger(__name__)
 
 
 @admin.register(Servers)
 class ServersAdmin(admin.ModelAdmin):
@@ -72,7 +72,12 @@
 class WelcomeMessageAdmin(admin.ModelAdmin):
     list_display = ('id', )
 
 
 @admin.register(GoodbyeMessage)
 class GoodbyeMessageAdmin(admin.ModelAdmin):
     list_display = ('id', )
+
+
+@admin.register(TicketGroups)
+class TicketGroupAdmin(admin.ModelAdmin):
+    filter_horizontal = ['groups']
```

### Comparing `allianceauth-discordbot-3.6.2/aadiscordbot/app_settings.py` & `allianceauth-discordbot-3.6.3/aadiscordbot/app_settings.py`

 * *Files 1% similar despite different names*

```diff
@@ -113,7 +113,10 @@
 DISCORD_BOT_ESS_PING_CHANNEL_ID = getattr(
     settings, 'DISCORD_BOT_ESS_PING_CHANNEL_ID', None)
 
 DISCORD_BOT_SEND_FAILURE_MESSAGES = getattr(
     settings, 'DISCORD_BOT_SEND_FAILURE_MESSAGES', False)
 DISCORD_BOT_FAILURE_MESSAGES_CHANNEL = getattr(
     settings, 'DISCORD_BOT_FAILURE_MESSAGES_CHANNEL', False)
+
+PRICE_CHECK_HOSTNAME = getattr(
+    settings, 'PRICE_CHECK_HOSTNAME', "evepraisal.com")
```

### Comparing `allianceauth-discordbot-3.6.2/aadiscordbot/auth_hooks.py` & `allianceauth-discordbot-3.6.3/aadiscordbot/auth_hooks.py`

 * *Files identical despite different names*

### Comparing `allianceauth-discordbot-3.6.2/aadiscordbot/bot.py` & `allianceauth-discordbot-3.6.3/aadiscordbot/bot.py`

 * *Files identical despite different names*

### Comparing `allianceauth-discordbot-3.6.2/aadiscordbot/bot_tasks.py` & `allianceauth-discordbot-3.6.3/aadiscordbot/bot_tasks.py`

 * *Files identical despite different names*

### Comparing `allianceauth-discordbot-3.6.2/aadiscordbot/cogs/about.py` & `allianceauth-discordbot-3.6.3/aadiscordbot/cogs/about.py`

 * *Files identical despite different names*

### Comparing `allianceauth-discordbot-3.6.2/aadiscordbot/cogs/abuse.py` & `allianceauth-discordbot-3.6.3/aadiscordbot/cogs/abuse.py`

 * *Files identical despite different names*

### Comparing `allianceauth-discordbot-3.6.2/aadiscordbot/cogs/admin.py` & `allianceauth-discordbot-3.6.3/aadiscordbot/cogs/admin.py`

 * *Files identical despite different names*

### Comparing `allianceauth-discordbot-3.6.2/aadiscordbot/cogs/auth.py` & `allianceauth-discordbot-3.6.3/aadiscordbot/cogs/auth.py`

 * *Files identical despite different names*

### Comparing `allianceauth-discordbot-3.6.2/aadiscordbot/cogs/eastereggs.py` & `allianceauth-discordbot-3.6.3/aadiscordbot/cogs/eastereggs.py`

 * *Files identical despite different names*

### Comparing `allianceauth-discordbot-3.6.2/aadiscordbot/cogs/eightball.py` & `allianceauth-discordbot-3.6.3/aadiscordbot/cogs/eightball.py`

 * *Files identical despite different names*

### Comparing `allianceauth-discordbot-3.6.2/aadiscordbot/cogs/facwar.py` & `allianceauth-discordbot-3.6.3/aadiscordbot/cogs/facwar.py`

 * *Files identical despite different names*

### Comparing `allianceauth-discordbot-3.6.2/aadiscordbot/cogs/members.py` & `allianceauth-discordbot-3.6.3/aadiscordbot/cogs/members.py`

 * *Files 5% similar despite different names*

```diff
@@ -151,15 +151,15 @@
             embed.description = (
                 "Character **{character_name}** does not exist in our Auth system"
             ).format(character_name=input_name)
 
             return embed
 
     @commands.command(pass_context=True)
-    @sender_has_any_perm(['corputils.view_alliance_corpstats', 'corpstats.view_alliance_corpstats'])
+    @sender_has_any_perm(['corputils.view_alliance_corpstats', 'corpstats.view_alliance_corpstats', 'aadiscordbot.member_command_access'])
     @message_in_channels(settings.ADMIN_DISCORD_BOT_CHANNELS)
     async def lookup(self, ctx):
         """
         Gets Auth data about a character
         Input: a Eve Character Name
         """
         input_name = ctx.message.content[8:]
@@ -174,16 +174,16 @@
     async def slash_lookup(
         self,
         ctx,
         character: str,
     ):
         try:
             in_channels(ctx.channel.id, settings.ADMIN_DISCORD_BOT_CHANNELS)
-            has_any_perm(ctx.author.id, [
-                         'corputils.view_alliance_corpstats', 'corpstats.view_alliance_corpstats'])
+            has_any_perm(ctx.author.id, ['corputils.view_alliance_corpstats',
+                         'corpstats.view_alliance_corpstats', 'aadiscordbot.member_command_access'])
             await ctx.defer()
             return await ctx.respond(embed=self.get_lookup_embed(character))
         except commands.MissingPermissions as e:
             return await ctx.respond(e.missing_permissions[0], ephemeral=True)
 
     async def search_corps_on_characters(ctx: AutocompleteContext):
         """Returns a list of colors that begin with the characters entered so far."""
@@ -254,30 +254,30 @@
     async def slash_altcorp(
         self,
         ctx,
         corporation: str,
     ):
         try:
             in_channels(ctx.channel.id, settings.ADMIN_DISCORD_BOT_CHANNELS)
-            has_any_perm(ctx.author.id, [
-                         'corputils.view_alliance_corpstats', 'corpstats.view_alliance_corpstats'])
+            has_any_perm(ctx.author.id, ['corputils.view_alliance_corpstats',
+                         'corpstats.view_alliance_corpstats', 'aadiscordbot.member_command_access'])
             await ctx.defer()
             embeds = self.build_altcorp_embeds(corporation)
             if len(embeds):
                 e = embeds.pop(0)
                 await ctx.respond(embed=e)
                 for e in embeds:
                     await ctx.send(embed=e)
             else:
                 await ctx.respond("No Members Found!")
         except commands.MissingPermissions as e:
             return await ctx.respond(e.missing_permissions[0], ephemeral=True)
 
     @commands.command(pass_context=True)
-    @sender_has_any_perm(['corputils.view_alliance_corpstats', 'corpstats.view_alliance_corpstats'])
+    @sender_has_any_perm(['corputils.view_alliance_corpstats', 'corpstats.view_alliance_corpstats', 'aadiscordbot.member_command_access'])
     @message_in_channels(settings.ADMIN_DISCORD_BOT_CHANNELS)
     async def altcorp(self, ctx):
         """
         Gets Auth data about an altcorp
         Input: a Eve Character Name
         """
         corporation = ctx.message.content[9:]
```

### Comparing `allianceauth-discordbot-3.6.2/aadiscordbot/cogs/models.py` & `allianceauth-discordbot-3.6.3/aadiscordbot/cogs/models.py`

 * *Files identical despite different names*

### Comparing `allianceauth-discordbot-3.6.2/aadiscordbot/cogs/price_check.py` & `allianceauth-discordbot-3.6.3/aadiscordbot/cogs/price_check.py`

 * *Files 2% similar despite different names*

```diff
@@ -5,14 +5,18 @@
 import logging
 
 import requests
 from discord.colour import Color
 from discord.embeds import Embed
 from discord.ext import commands
 
+from ..app_settings import (
+    PRICE_CHECK_HOSTNAME
+)
+
 logger = logging.getLogger(__name__)
 
 
 class PriceCheck(commands.Cog):
     """
     price checks on Jita and Amarr markets
     """
@@ -102,15 +106,15 @@
                     value="Prices for {item_name} on the {market_name} Market.".format(
                         item_name=item_name, market_name=market["name"]
                     ),
                     inline=False,
                 )
 
                 market_data = requests.post(
-                    "https://evepraisal.com/appraisal/structured.json",
+                    "https://" + PRICE_CHECK_HOSTNAME + "/appraisal/structured.json",
                     json={
                         "market_name": market["api_key"],
                         "items": [{"name": item_name}],
                     },
                 )
 
                 if market_data.status_code == 200:
```

### Comparing `allianceauth-discordbot-3.6.2/aadiscordbot/cogs/prom_export.py` & `allianceauth-discordbot-3.6.3/aadiscordbot/cogs/prom_export.py`

 * *Files identical despite different names*

### Comparing `allianceauth-discordbot-3.6.2/aadiscordbot/cogs/quote.py` & `allianceauth-discordbot-3.6.3/aadiscordbot/cogs/quote.py`

 * *Files identical despite different names*

### Comparing `allianceauth-discordbot-3.6.2/aadiscordbot/cogs/reaction_roles.py` & `allianceauth-discordbot-3.6.3/aadiscordbot/cogs/reaction_roles.py`

 * *Files identical despite different names*

### Comparing `allianceauth-discordbot-3.6.2/aadiscordbot/cogs/remind.py` & `allianceauth-discordbot-3.6.3/aadiscordbot/cogs/remind.py`

 * *Files identical despite different names*

### Comparing `allianceauth-discordbot-3.6.2/aadiscordbot/cogs/services.py` & `allianceauth-discordbot-3.6.3/aadiscordbot/cogs/services.py`

 * *Files identical despite different names*

### Comparing `allianceauth-discordbot-3.6.2/aadiscordbot/cogs/sov.py` & `allianceauth-discordbot-3.6.3/aadiscordbot/cogs/sov.py`

 * *Files identical despite different names*

### Comparing `allianceauth-discordbot-3.6.2/aadiscordbot/cogs/time.py` & `allianceauth-discordbot-3.6.3/aadiscordbot/cogs/time.py`

 * *Files identical despite different names*

### Comparing `allianceauth-discordbot-3.6.2/aadiscordbot/cogs/timers.py` & `allianceauth-discordbot-3.6.3/aadiscordbot/cogs/timers.py`

 * *Files identical despite different names*

### Comparing `allianceauth-discordbot-3.6.2/aadiscordbot/cogs/utils/decorators.py` & `allianceauth-discordbot-3.6.3/aadiscordbot/cogs/utils/decorators.py`

 * *Files identical despite different names*

### Comparing `allianceauth-discordbot-3.6.2/aadiscordbot/cogs/welcomegoodbye.py` & `allianceauth-discordbot-3.6.3/aadiscordbot/cogs/welcomegoodbye.py`

 * *Files identical despite different names*

### Comparing `allianceauth-discordbot-3.6.2/aadiscordbot/migrations/0001_initial.py` & `allianceauth-discordbot-3.6.3/aadiscordbot/migrations/0001_initial.py`

 * *Files identical despite different names*

### Comparing `allianceauth-discordbot-3.6.2/aadiscordbot/migrations/0002_reactionrolebinding_reactionrolemessage.py` & `allianceauth-discordbot-3.6.3/aadiscordbot/migrations/0002_reactionrolebinding_reactionrolemessage.py`

 * *Files identical despite different names*

### Comparing `allianceauth-discordbot-3.6.2/aadiscordbot/migrations/0003_authbotconfiguration.py` & `allianceauth-discordbot-3.6.3/aadiscordbot/migrations/0003_authbotconfiguration.py`

 * *Files identical despite different names*

### Comparing `allianceauth-discordbot-3.6.2/aadiscordbot/migrations/0005_rr_fixes_blank_admins.py` & `allianceauth-discordbot-3.6.3/aadiscordbot/migrations/0005_rr_fixes_blank_admins.py`

 * *Files identical despite different names*

### Comparing `allianceauth-discordbot-3.6.2/aadiscordbot/migrations/0006_goodbyemessage_welcomemessage.py` & `allianceauth-discordbot-3.6.3/aadiscordbot/migrations/0006_goodbyemessage_welcomemessage.py`

 * *Files identical despite different names*

### Comparing `allianceauth-discordbot-3.6.2/aadiscordbot/migrations/0007_quotemessage.py` & `allianceauth-discordbot-3.6.3/aadiscordbot/migrations/0007_quotemessage.py`

 * *Files identical despite different names*

### Comparing `allianceauth-discordbot-3.6.2/aadiscordbot/models.py` & `allianceauth-discordbot-3.6.3/aadiscordbot/models.py`

 * *Files 16% similar despite different names*

```diff
@@ -1,7 +1,9 @@
+from solo.models import SingletonModel
+
 from django.conf import settings
 from django.contrib.auth.models import Group
 from django.core.exceptions import ValidationError
 from django.db import models
 from django.utils.translation import gettext_lazy as _
 
 from allianceauth.services.modules.discord.models import DiscordUser
@@ -10,15 +12,16 @@
 class DiscordBot(models.Model):
     """Meta model for app permissions"""
 
     class Meta:
         managed = False
         default_permissions = ()
         permissions = (
-            ('basic_access', 'Can access this app'),
+            ('basic_access', 'Can access this app.'),
+            ('member_command_access', 'can access the member commands.')
         )
 
 
 class Servers(models.Model):
     """Servers and their ID"""
 
     server = models.BigIntegerField(primary_key=True)
@@ -138,7 +141,22 @@
     class Meta:
         default_permissions = ()
         verbose_name = 'Quote Message'
         verbose_name_plural = 'Quote Messages'
         permissions = (
             ('quote_save', 'Can save quotes'),
         )
+
+
+class TicketGroups(SingletonModel):
+    groups = models.ManyToManyField(
+        Group, blank=True, help_text="Pingable groups for ticketing")
+    ticket_channel = models.ForeignKey(
+        Channels, on_delete=models.SET_NULL, null=True, default=None)
+
+    class Meta:
+        default_permissions = ()
+        verbose_name = 'Ticket Cog Configuration'
+        verbose_name_plural = 'Ticket Cog Configuration'
+
+    def __str__(self):
+        return "Ticket Cog Configuration"
```

### Comparing `allianceauth-discordbot-3.6.2/aadiscordbot/tasks.py` & `allianceauth-discordbot-3.6.3/aadiscordbot/tasks.py`

 * *Files identical despite different names*

### Comparing `allianceauth-discordbot-3.6.2/allianceauth_discordbot.egg-info/PKG-INFO` & `allianceauth-discordbot-3.6.3/allianceauth_discordbot.egg-info/PKG-INFO`

 * *Files 2% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: allianceauth-discordbot
-Version: 3.6.2
+Version: 3.6.3
 Summary: Alliance Auth Discord Bot
 Home-page: https://github.com/pvyParts/allianceauth-discordbot
 Author: ak
 Author-email: ak@ak.auth
 License: GNU General Public License v3 (GPLv3)
 Platform: UNKNOWN
 Classifier: Environment :: Web Environment
@@ -102,14 +102,16 @@
 
 DISCORD_BOT_SOV_STRUCTURE_OWNER_IDS = [1000169] # Centre for Advanced Studies example
 DISCORD_BOT_MEMBER_ALLIANCES = [111, 222, 333] # A list of alliances to be considered "Mains"
 
 DISCORD_BOT_ADM_REGIONS = [10000002] # The Forge Example
 DISCORD_BOT_ADM_SYSTEMS = [30000142] # Jita Example
 DISCORD_BOT_ADM_CONSTELLATIONS = [20000020] # Kimitoro Example
+
+PRICE_CHECK_HOSTNAME = "evepraisal.com" # Point to your favorite evepraisal
 ```
 
 ```python
 ## Insert AADiscordBot's logging into Django Logging config
 LOGGING['handlers']['bot_log_file']= {
             'level': 'INFO',
             'class': 'logging.handlers.RotatingFileHandler',
```

### Comparing `allianceauth-discordbot-3.6.2/allianceauth_discordbot.egg-info/SOURCES.txt` & `allianceauth-discordbot-3.6.3/allianceauth_discordbot.egg-info/SOURCES.txt`

 * *Files 4% similar despite different names*

```diff
@@ -27,14 +27,15 @@
 aadiscordbot/cogs/price_check.py
 aadiscordbot/cogs/prom_export.py
 aadiscordbot/cogs/quote.py
 aadiscordbot/cogs/reaction_roles.py
 aadiscordbot/cogs/remind.py
 aadiscordbot/cogs/services.py
 aadiscordbot/cogs/sov.py
+aadiscordbot/cogs/tickets.py
 aadiscordbot/cogs/time.py
 aadiscordbot/cogs/timers.py
 aadiscordbot/cogs/welcomegoodbye.py
 aadiscordbot/cogs/utils/__init__.py
 aadiscordbot/cogs/utils/context.py
 aadiscordbot/cogs/utils/decorators.py
 aadiscordbot/cogs/utils/exceptions.py
@@ -43,13 +44,15 @@
 aadiscordbot/migrations/0003_authbotconfiguration.py
 aadiscordbot/migrations/0004_settings.py
 aadiscordbot/migrations/0005_rr_fixes_blank_admins.py
 aadiscordbot/migrations/0006_goodbyemessage_welcomemessage.py
 aadiscordbot/migrations/0007_quotemessage.py
 aadiscordbot/migrations/0008_channels_deleted.py
 aadiscordbot/migrations/0009_alter_quotemessage_options.py
+aadiscordbot/migrations/0010_alter_discordbot_options_ticketgroups.py
+aadiscordbot/migrations/0011_alter_ticketgroups_options_and_more.py
 aadiscordbot/migrations/__init__.py
 allianceauth_discordbot.egg-info/PKG-INFO
 allianceauth_discordbot.egg-info/SOURCES.txt
 allianceauth_discordbot.egg-info/dependency_links.txt
 allianceauth_discordbot.egg-info/requires.txt
 allianceauth_discordbot.egg-info/top_level.txt
```

### Comparing `allianceauth-discordbot-3.6.2/setup.py` & `allianceauth-discordbot-3.6.3/setup.py`

 * *Files identical despite different names*

