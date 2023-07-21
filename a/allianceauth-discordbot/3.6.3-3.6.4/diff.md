# Comparing `tmp/allianceauth-discordbot-3.6.3.tar.gz` & `tmp/allianceauth_discordbot-3.6.4.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "allianceauth-discordbot-3.6.3.tar", last modified: Fri Jul 21 09:20:09 2023, max compression
+gzip compressed data, was "allianceauth_discordbot-3.6.4.tar", last modified: Fri Jan  1 00:00:00 2016, max compression
```

## Comparing `allianceauth-discordbot-3.6.3.tar` & `allianceauth_discordbot-3.6.4.tar`

### file list

```diff
@@ -1,66 +1,63 @@
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-21 09:20:09.894833 allianceauth-discordbot-3.6.3/
--rw-r--r--   0 runner    (1001) docker     (123)      109 2023-07-21 09:19:22.000000 allianceauth-discordbot-3.6.3/MANIFEST.in
--rw-r--r--   0 runner    (1001) docker     (123)    14977 2023-07-21 09:20:09.894833 allianceauth-discordbot-3.6.3/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (123)    14070 2023-07-21 09:19:22.000000 allianceauth-discordbot-3.6.3/README.md
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-21 09:20:09.890833 allianceauth-discordbot-3.6.3/aadiscordbot/
--rw-r--r--   0 runner    (1001) docker     (123)      134 2023-07-21 09:19:22.000000 allianceauth-discordbot-3.6.3/aadiscordbot/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)     1977 2023-07-21 09:19:22.000000 allianceauth-discordbot-3.6.3/aadiscordbot/admin.py
--rw-r--r--   0 runner    (1001) docker     (123)     3857 2023-07-21 09:19:22.000000 allianceauth-discordbot-3.6.3/aadiscordbot/app_settings.py
--rw-r--r--   0 runner    (1001) docker     (123)      263 2023-07-21 09:19:22.000000 allianceauth-discordbot-3.6.3/aadiscordbot/apps.py
--rw-r--r--   0 runner    (1001) docker     (123)      928 2023-07-21 09:19:22.000000 allianceauth-discordbot-3.6.3/aadiscordbot/auth_hooks.py
--rw-r--r--   0 runner    (1001) docker     (123)    17002 2023-07-21 09:19:22.000000 allianceauth-discordbot-3.6.3/aadiscordbot/bot.py
--rw-r--r--   0 runner    (1001) docker     (123)     4126 2023-07-21 09:19:22.000000 allianceauth-discordbot-3.6.3/aadiscordbot/bot_tasks.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-21 09:20:09.890833 allianceauth-discordbot-3.6.3/aadiscordbot/cogs/
--rw-r--r--   0 runner    (1001) docker     (123)        0 2023-07-21 09:19:22.000000 allianceauth-discordbot-3.6.3/aadiscordbot/cogs/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)     3261 2023-07-21 09:19:22.000000 allianceauth-discordbot-3.6.3/aadiscordbot/cogs/about.py
--rw-r--r--   0 runner    (1001) docker     (123)     2931 2023-07-21 09:19:22.000000 allianceauth-discordbot-3.6.3/aadiscordbot/cogs/abuse.py
--rw-r--r--   0 runner    (1001) docker     (123)    16421 2023-07-21 09:19:22.000000 allianceauth-discordbot-3.6.3/aadiscordbot/cogs/admin.py
--rw-r--r--   0 runner    (1001) docker     (123)     2694 2023-07-21 09:19:22.000000 allianceauth-discordbot-3.6.3/aadiscordbot/cogs/auth.py
--rw-r--r--   0 runner    (1001) docker     (123)      909 2023-07-21 09:19:22.000000 allianceauth-discordbot-3.6.3/aadiscordbot/cogs/eastereggs.py
--rw-r--r--   0 runner    (1001) docker     (123)     1459 2023-07-21 09:19:22.000000 allianceauth-discordbot-3.6.3/aadiscordbot/cogs/eightball.py
--rw-r--r--   0 runner    (1001) docker     (123)     3827 2023-07-21 09:19:22.000000 allianceauth-discordbot-3.6.3/aadiscordbot/cogs/facwar.py
--rw-r--r--   0 runner    (1001) docker     (123)    12709 2023-07-21 09:19:22.000000 allianceauth-discordbot-3.6.3/aadiscordbot/cogs/members.py
--rw-r--r--   0 runner    (1001) docker     (123)     3531 2023-07-21 09:19:22.000000 allianceauth-discordbot-3.6.3/aadiscordbot/cogs/models.py
--rw-r--r--   0 runner    (1001) docker     (123)     5703 2023-07-21 09:19:22.000000 allianceauth-discordbot-3.6.3/aadiscordbot/cogs/price_check.py
--rw-r--r--   0 runner    (1001) docker     (123)     1495 2023-07-21 09:19:22.000000 allianceauth-discordbot-3.6.3/aadiscordbot/cogs/prom_export.py
--rw-r--r--   0 runner    (1001) docker     (123)     5180 2023-07-21 09:19:22.000000 allianceauth-discordbot-3.6.3/aadiscordbot/cogs/quote.py
--rw-r--r--   0 runner    (1001) docker     (123)     6214 2023-07-21 09:19:22.000000 allianceauth-discordbot-3.6.3/aadiscordbot/cogs/reaction_roles.py
--rw-r--r--   0 runner    (1001) docker     (123)     1105 2023-07-21 09:19:22.000000 allianceauth-discordbot-3.6.3/aadiscordbot/cogs/remind.py
--rw-r--r--   0 runner    (1001) docker     (123)     6532 2023-07-21 09:19:22.000000 allianceauth-discordbot-3.6.3/aadiscordbot/cogs/services.py
--rw-r--r--   0 runner    (1001) docker     (123)    15830 2023-07-21 09:19:22.000000 allianceauth-discordbot-3.6.3/aadiscordbot/cogs/sov.py
--rw-r--r--   0 runner    (1001) docker     (123)     4070 2023-07-21 09:19:22.000000 allianceauth-discordbot-3.6.3/aadiscordbot/cogs/tickets.py
--rw-r--r--   0 runner    (1001) docker     (123)     1396 2023-07-21 09:19:22.000000 allianceauth-discordbot-3.6.3/aadiscordbot/cogs/time.py
--rw-r--r--   0 runner    (1001) docker     (123)     2171 2023-07-21 09:19:22.000000 allianceauth-discordbot-3.6.3/aadiscordbot/cogs/timers.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-21 09:20:09.890833 allianceauth-discordbot-3.6.3/aadiscordbot/cogs/utils/
--rw-r--r--   0 runner    (1001) docker     (123)        0 2023-07-21 09:19:22.000000 allianceauth-discordbot-3.6.3/aadiscordbot/cogs/utils/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)      207 2023-07-21 09:19:22.000000 allianceauth-discordbot-3.6.3/aadiscordbot/cogs/utils/context.py
--rw-r--r--   0 runner    (1001) docker     (123)     3883 2023-07-21 09:19:22.000000 allianceauth-discordbot-3.6.3/aadiscordbot/cogs/utils/decorators.py
--rw-r--r--   0 runner    (1001) docker     (123)      437 2023-07-21 09:19:22.000000 allianceauth-discordbot-3.6.3/aadiscordbot/cogs/utils/exceptions.py
--rw-r--r--   0 runner    (1001) docker     (123)     4373 2023-07-21 09:19:22.000000 allianceauth-discordbot-3.6.3/aadiscordbot/cogs/welcomegoodbye.py
--rw-r--r--   0 runner    (1001) docker     (123)      235 2023-07-21 09:19:22.000000 allianceauth-discordbot-3.6.3/aadiscordbot/launcher.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-21 09:20:09.894833 allianceauth-discordbot-3.6.3/aadiscordbot/migrations/
--rw-r--r--   0 runner    (1001) docker     (123)     1621 2023-07-21 09:19:22.000000 allianceauth-discordbot-3.6.3/aadiscordbot/migrations/0001_initial.py
--rw-r--r--   0 runner    (1001) docker     (123)     1410 2023-07-21 09:19:22.000000 allianceauth-discordbot-3.6.3/aadiscordbot/migrations/0002_reactionrolebinding_reactionrolemessage.py
--rw-r--r--   0 runner    (1001) docker     (123)      636 2023-07-21 09:19:22.000000 allianceauth-discordbot-3.6.3/aadiscordbot/migrations/0003_authbotconfiguration.py
--rw-r--r--   0 runner    (1001) docker     (123)      485 2023-07-21 09:19:22.000000 allianceauth-discordbot-3.6.3/aadiscordbot/migrations/0004_settings.py
--rw-r--r--   0 runner    (1001) docker     (123)      759 2023-07-21 09:19:22.000000 allianceauth-discordbot-3.6.3/aadiscordbot/migrations/0005_rr_fixes_blank_admins.py
--rw-r--r--   0 runner    (1001) docker     (123)     1773 2023-07-21 09:19:22.000000 allianceauth-discordbot-3.6.3/aadiscordbot/migrations/0006_goodbyemessage_welcomemessage.py
--rw-r--r--   0 runner    (1001) docker     (123)     1219 2023-07-21 09:19:22.000000 allianceauth-discordbot-3.6.3/aadiscordbot/migrations/0007_quotemessage.py
--rw-r--r--   0 runner    (1001) docker     (123)      413 2023-07-21 09:19:22.000000 allianceauth-discordbot-3.6.3/aadiscordbot/migrations/0008_channels_deleted.py
--rw-r--r--   0 runner    (1001) docker     (123)      507 2023-07-21 09:19:22.000000 allianceauth-discordbot-3.6.3/aadiscordbot/migrations/0009_alter_quotemessage_options.py
--rw-r--r--   0 runner    (1001) docker     (123)     1056 2023-07-21 09:19:22.000000 allianceauth-discordbot-3.6.3/aadiscordbot/migrations/0010_alter_discordbot_options_ticketgroups.py
--rw-r--r--   0 runner    (1001) docker     (123)      805 2023-07-21 09:19:22.000000 allianceauth-discordbot-3.6.3/aadiscordbot/migrations/0011_alter_ticketgroups_options_and_more.py
--rw-r--r--   0 runner    (1001) docker     (123)        0 2023-07-21 09:19:22.000000 allianceauth-discordbot-3.6.3/aadiscordbot/migrations/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)     5148 2023-07-21 09:19:22.000000 allianceauth-discordbot-3.6.3/aadiscordbot/models.py
--rw-r--r--   0 runner    (1001) docker     (123)      317 2023-07-21 09:19:22.000000 allianceauth-discordbot-3.6.3/aadiscordbot/providers.py
--rw-r--r--   0 runner    (1001) docker     (123)     3628 2023-07-21 09:19:22.000000 allianceauth-discordbot-3.6.3/aadiscordbot/tasks.py
--rw-r--r--   0 runner    (1001) docker     (123)       45 2023-07-21 09:19:22.000000 allianceauth-discordbot-3.6.3/aadiscordbot/urls.py
--rw-r--r--   0 runner    (1001) docker     (123)       15 2023-07-21 09:19:22.000000 allianceauth-discordbot-3.6.3/aadiscordbot/views.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-21 09:20:09.894833 allianceauth-discordbot-3.6.3/allianceauth_discordbot.egg-info/
--rw-r--r--   0 runner    (1001) docker     (123)    14977 2023-07-21 09:20:09.000000 allianceauth-discordbot-3.6.3/allianceauth_discordbot.egg-info/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (123)     1985 2023-07-21 09:20:09.000000 allianceauth-discordbot-3.6.3/allianceauth_discordbot.egg-info/SOURCES.txt
--rw-r--r--   0 runner    (1001) docker     (123)        1 2023-07-21 09:20:09.000000 allianceauth-discordbot-3.6.3/allianceauth_discordbot.egg-info/dependency_links.txt
--rw-r--r--   0 runner    (1001) docker     (123)       91 2023-07-21 09:20:09.000000 allianceauth-discordbot-3.6.3/allianceauth_discordbot.egg-info/requires.txt
--rw-r--r--   0 runner    (1001) docker     (123)       13 2023-07-21 09:20:09.000000 allianceauth-discordbot-3.6.3/allianceauth_discordbot.egg-info/top_level.txt
--rw-r--r--   0 runner    (1001) docker     (123)       38 2023-07-21 09:20:09.894833 allianceauth-discordbot-3.6.3/setup.cfg
--rw-r--r--   0 runner    (1001) docker     (123)     1516 2023-07-21 09:19:22.000000 allianceauth-discordbot-3.6.3/setup.py
+-rw-r--r--   0        0        0     1322 2023-07-21 13:44:57.261411 allianceauth_discordbot-3.6.4/.github/workflows/main.yml
+-rw-r--r--   0        0        0      719 2023-07-21 13:44:57.261411 allianceauth_discordbot-3.6.4/.github/workflows/publish.yml
+-rw-r--r--   0        0        0      339 2023-07-21 13:44:57.261411 allianceauth_discordbot-3.6.4/.gitignore
+-rw-r--r--   0        0        0      179 2023-07-21 13:44:57.261411 allianceauth_discordbot-3.6.4/.isort.cfg
+-rw-r--r--   0        0        0     1164 2023-07-21 13:44:57.261411 allianceauth_discordbot-3.6.4/.pre-commit-config.yaml
+-rw-r--r--   0        0        0     3233 2023-07-21 13:44:57.261411 allianceauth_discordbot-3.6.4/CHANGELOG.md
+-rw-r--r--   0        0        0     1077 2023-07-21 13:44:57.261411 allianceauth_discordbot-3.6.4/LICENSE
+-rw-r--r--   0        0        0      109 2023-07-21 13:44:57.261411 allianceauth_discordbot-3.6.4/MANIFEST.in
+-rw-r--r--   0        0        0      636 2023-07-21 13:44:57.261411 allianceauth_discordbot-3.6.4/Makefile
+-rw-r--r--   0        0        0    14226 2023-07-21 13:44:57.261411 allianceauth_discordbot-3.6.4/README.md
+-rw-r--r--   0        0        0      176 2023-07-21 13:44:57.261411 allianceauth_discordbot-3.6.4/aadiscordbot/__init__.py
+-rw-r--r--   0        0        0     1977 2023-07-21 13:44:57.261411 allianceauth_discordbot-3.6.4/aadiscordbot/admin.py
+-rw-r--r--   0        0        0     3857 2023-07-21 13:44:57.261411 allianceauth_discordbot-3.6.4/aadiscordbot/app_settings.py
+-rw-r--r--   0        0        0      263 2023-07-21 13:44:57.261411 allianceauth_discordbot-3.6.4/aadiscordbot/apps.py
+-rw-r--r--   0        0        0      928 2023-07-21 13:44:57.261411 allianceauth_discordbot-3.6.4/aadiscordbot/auth_hooks.py
+-rw-r--r--   0        0        0    17002 2023-07-21 13:44:57.261411 allianceauth_discordbot-3.6.4/aadiscordbot/bot.py
+-rw-r--r--   0        0        0     4126 2023-07-21 13:44:57.261411 allianceauth_discordbot-3.6.4/aadiscordbot/bot_tasks.py
+-rw-r--r--   0        0        0        0 2023-07-21 13:44:57.261411 allianceauth_discordbot-3.6.4/aadiscordbot/cogs/__init__.py
+-rw-r--r--   0        0        0     3261 2023-07-21 13:44:57.261411 allianceauth_discordbot-3.6.4/aadiscordbot/cogs/about.py
+-rw-r--r--   0        0        0     2931 2023-07-21 13:44:57.265411 allianceauth_discordbot-3.6.4/aadiscordbot/cogs/abuse.py
+-rw-r--r--   0        0        0    16421 2023-07-21 13:44:57.265411 allianceauth_discordbot-3.6.4/aadiscordbot/cogs/admin.py
+-rw-r--r--   0        0        0     2694 2023-07-21 13:44:57.265411 allianceauth_discordbot-3.6.4/aadiscordbot/cogs/auth.py
+-rw-r--r--   0        0        0      909 2023-07-21 13:44:57.265411 allianceauth_discordbot-3.6.4/aadiscordbot/cogs/eastereggs.py
+-rw-r--r--   0        0        0     1459 2023-07-21 13:44:57.265411 allianceauth_discordbot-3.6.4/aadiscordbot/cogs/eightball.py
+-rw-r--r--   0        0        0     3827 2023-07-21 13:44:57.265411 allianceauth_discordbot-3.6.4/aadiscordbot/cogs/facwar.py
+-rw-r--r--   0        0        0    12709 2023-07-21 13:44:57.265411 allianceauth_discordbot-3.6.4/aadiscordbot/cogs/members.py
+-rw-r--r--   0        0        0     3531 2023-07-21 13:44:57.265411 allianceauth_discordbot-3.6.4/aadiscordbot/cogs/models.py
+-rw-r--r--   0        0        0     5703 2023-07-21 13:44:57.265411 allianceauth_discordbot-3.6.4/aadiscordbot/cogs/price_check.py
+-rw-r--r--   0        0        0     1495 2023-07-21 13:44:57.265411 allianceauth_discordbot-3.6.4/aadiscordbot/cogs/prom_export.py
+-rw-r--r--   0        0        0     5180 2023-07-21 13:44:57.265411 allianceauth_discordbot-3.6.4/aadiscordbot/cogs/quote.py
+-rw-r--r--   0        0        0     6214 2023-07-21 13:44:57.265411 allianceauth_discordbot-3.6.4/aadiscordbot/cogs/reaction_roles.py
+-rw-r--r--   0        0        0     1105 2023-07-21 13:44:57.265411 allianceauth_discordbot-3.6.4/aadiscordbot/cogs/remind.py
+-rw-r--r--   0        0        0     6532 2023-07-21 13:44:57.265411 allianceauth_discordbot-3.6.4/aadiscordbot/cogs/services.py
+-rw-r--r--   0        0        0    15830 2023-07-21 13:44:57.265411 allianceauth_discordbot-3.6.4/aadiscordbot/cogs/sov.py
+-rw-r--r--   0        0        0     4070 2023-07-21 13:44:57.265411 allianceauth_discordbot-3.6.4/aadiscordbot/cogs/tickets.py
+-rw-r--r--   0        0        0     1396 2023-07-21 13:44:57.265411 allianceauth_discordbot-3.6.4/aadiscordbot/cogs/time.py
+-rw-r--r--   0        0        0     2171 2023-07-21 13:44:57.265411 allianceauth_discordbot-3.6.4/aadiscordbot/cogs/timers.py
+-rw-r--r--   0        0        0        0 2023-07-21 13:44:57.265411 allianceauth_discordbot-3.6.4/aadiscordbot/cogs/utils/__init__.py
+-rw-r--r--   0        0        0      207 2023-07-21 13:44:57.265411 allianceauth_discordbot-3.6.4/aadiscordbot/cogs/utils/context.py
+-rw-r--r--   0        0        0     3883 2023-07-21 13:44:57.265411 allianceauth_discordbot-3.6.4/aadiscordbot/cogs/utils/decorators.py
+-rw-r--r--   0        0        0      437 2023-07-21 13:44:57.265411 allianceauth_discordbot-3.6.4/aadiscordbot/cogs/utils/exceptions.py
+-rw-r--r--   0        0        0     4373 2023-07-21 13:44:57.265411 allianceauth_discordbot-3.6.4/aadiscordbot/cogs/welcomegoodbye.py
+-rw-r--r--   0        0        0      235 2023-07-21 13:44:57.265411 allianceauth_discordbot-3.6.4/aadiscordbot/launcher.py
+-rw-r--r--   0        0        0     1621 2023-07-21 13:44:57.265411 allianceauth_discordbot-3.6.4/aadiscordbot/migrations/0001_initial.py
+-rw-r--r--   0        0        0     1410 2023-07-21 13:44:57.265411 allianceauth_discordbot-3.6.4/aadiscordbot/migrations/0002_reactionrolebinding_reactionrolemessage.py
+-rw-r--r--   0        0        0      636 2023-07-21 13:44:57.265411 allianceauth_discordbot-3.6.4/aadiscordbot/migrations/0003_authbotconfiguration.py
+-rw-r--r--   0        0        0      485 2023-07-21 13:44:57.265411 allianceauth_discordbot-3.6.4/aadiscordbot/migrations/0004_settings.py
+-rw-r--r--   0        0        0      759 2023-07-21 13:44:57.265411 allianceauth_discordbot-3.6.4/aadiscordbot/migrations/0005_rr_fixes_blank_admins.py
+-rw-r--r--   0        0        0     1773 2023-07-21 13:44:57.265411 allianceauth_discordbot-3.6.4/aadiscordbot/migrations/0006_goodbyemessage_welcomemessage.py
+-rw-r--r--   0        0        0     1219 2023-07-21 13:44:57.265411 allianceauth_discordbot-3.6.4/aadiscordbot/migrations/0007_quotemessage.py
+-rw-r--r--   0        0        0      413 2023-07-21 13:44:57.265411 allianceauth_discordbot-3.6.4/aadiscordbot/migrations/0008_channels_deleted.py
+-rw-r--r--   0        0        0      507 2023-07-21 13:44:57.265411 allianceauth_discordbot-3.6.4/aadiscordbot/migrations/0009_alter_quotemessage_options.py
+-rw-r--r--   0        0        0     1056 2023-07-21 13:44:57.265411 allianceauth_discordbot-3.6.4/aadiscordbot/migrations/0010_alter_discordbot_options_ticketgroups.py
+-rw-r--r--   0        0        0      805 2023-07-21 13:44:57.265411 allianceauth_discordbot-3.6.4/aadiscordbot/migrations/0011_alter_ticketgroups_options_and_more.py
+-rw-r--r--   0        0        0        0 2023-07-21 13:44:57.265411 allianceauth_discordbot-3.6.4/aadiscordbot/migrations/__init__.py
+-rw-r--r--   0        0        0     5148 2023-07-21 13:44:57.265411 allianceauth_discordbot-3.6.4/aadiscordbot/models.py
+-rw-r--r--   0        0        0      317 2023-07-21 13:44:57.265411 allianceauth_discordbot-3.6.4/aadiscordbot/providers.py
+-rw-r--r--   0        0        0     3628 2023-07-21 13:44:57.265411 allianceauth_discordbot-3.6.4/aadiscordbot/tasks.py
+-rw-r--r--   0        0        0       45 2023-07-21 13:44:57.265411 allianceauth_discordbot-3.6.4/aadiscordbot/urls.py
+-rw-r--r--   0        0        0       15 2023-07-21 13:44:57.265411 allianceauth_discordbot-3.6.4/aadiscordbot/views.py
+-rw-r--r--   0        0        0      315 2023-07-21 13:44:57.265411 allianceauth_discordbot-3.6.4/bot_conf.py
+-rw-r--r--   0        0        0      873 2023-07-21 13:44:57.265411 allianceauth_discordbot-3.6.4/pyproject.toml
+-rw-r--r--   0        0        0    15001 1970-01-01 00:00:00.000000 allianceauth_discordbot-3.6.4/PKG-INFO
```

### Comparing `allianceauth-discordbot-3.6.3/PKG-INFO` & `allianceauth_discordbot-3.6.4/PKG-INFO`

 * *Files 6% similar despite different names*

```diff
@@ -1,30 +1,23 @@
 Metadata-Version: 2.1
 Name: allianceauth-discordbot
-Version: 3.6.3
-Summary: Alliance Auth Discord Bot
-Home-page: https://github.com/pvyParts/allianceauth-discordbot
-Author: ak
-Author-email: ak@ak.auth
-License: GNU General Public License v3 (GPLv3)
-Platform: UNKNOWN
-Classifier: Environment :: Web Environment
-Classifier: Framework :: Django
-Classifier: Framework :: Django :: 3.2
-Classifier: Framework :: Django :: 4.0
-Classifier: Intended Audience :: Developers
-Classifier: License :: OSI Approved :: GNU General Public License v3 (GPLv3)
-Classifier: Operating System :: OS Independent
-Classifier: Programming Language :: Python :: 3.10
-Classifier: Programming Language :: Python :: 3.9
-Classifier: Programming Language :: Python :: 3.8
-Classifier: Topic :: Internet :: WWW/HTTP
-Classifier: Topic :: Internet :: WWW/HTTP :: Dynamic Content
-Requires-Python: >=3.8
+Version: 3.6.4
+Summary: Alliance Auth Modular Discord Bot
+Author-email: AaronKable <aaronkable@gmail.com>
 Description-Content-Type: text/markdown
+Classifier: Framework :: Django
+Classifier: License :: OSI Approved :: MIT License
+Requires-Dist: allianceauth>=2.9.0,<4.0.0
+Requires-Dist: py-cord>2.0.0,<3.0.0
+Requires-Dist: pendulum>=2.1.2,<3.0.0
+Requires-Dist: redis>=4.2.0,<5.0.0
+Requires-Dist: django-solo>=2.1.0,<3.0.0
+Project-URL: Home, https://github.com/Solar-Helix-Independent-Transport/allianceauth-discordbot
+Project-URL: Source, https://github.com/Solar-Helix-Independent-Transport/allianceauth-discordbot
+Project-URL: Tracker, https://github.com/Solar-Helix-Independent-Transport/allianceauth-discordbot/issues
 
 # AA-Discordbot
 
 AA-Discordbot for [Alliance Auth](https://gitlab.com/allianceauth/allianceauth).
 
 [![PyPi](https://img.shields.io/pypi/v/allianceauth-discordbot?color=green)](https://pypi.org/project/allianceauth-discordbot/)
 
@@ -83,19 +76,19 @@
 
 * Install the app with your venv active
 
 ```bash
 pip install allianceauth-discordbot
 ```
 
-* Add `'aadiscordbot',` to your INSTALLED_APPS list in local.py.
+* Add `'aadiscordbot',` and  `'solo',` to your INSTALLED_APPS list in local.py.
 
 * Add the below lines to your `local.py` settings file, Changing the contexts to yours.
 
- ```python
+```python
 ## Settings for Allianceauth-Discordbot
 # Admin Commands
 ADMIN_DISCORD_BOT_CHANNELS = [111, 222, 333]
 # Sov Commands
 SOV_DISCORD_BOT_CHANNELS = [111, 222, 333]
 # Adm Commands
 ADM_DISCORD_BOT_CHANNELS = [111, 222, 333]
@@ -192,15 +185,20 @@
 ```ini
 #This block should already exist, add authbot to it
 [group:myauth]
 programs=beat,worker,gunicorn,authbot
 priority=999
 ```
 
-Last but not least, go to admin and configure your admin users in the bot config model.
+Go to admin and configure your admin users in the bot config model.
+
+> Enable groups/states/users to utilize the lookup command by adding permissions under **corputils | corp stats |**
+```ini
+corputils.view_alliance_corpstats
+```
 
 ## Reaction Roles
 > ❗❗❗ **This will bypass the Group Leadership/Join Request System**: This is intended for open groups but not limited to it! ❗❗❗
 
 The bot is able to run a reaction roles system that is compatible with auth and public users on a discord.
  - If a member is part of auth it will do auth syncing of roles
  - If a member is not found in auth and the reaction role message has the public flag set it will assign roles to anyone who reacts
@@ -358,8 +356,7 @@
 This is due to the Py-cord lib sharing the `discord` namespace. Py-Cord is however a drop in replacement. So no issues should arise from using it over the now legacy discord.py lib. **YMMV**
 
 **Fix:**
  1. Uninstall `discord.py` by running `pip uninstall discord.py` with your venv active.
  2. Reinstall `py-cord` by running `pip install -U py-cord==2.0.0b3` with your venv active.
  3. Approach the dev from the app that overrode your py-cord to update to a maintained lib.
 
-
```

### Comparing `allianceauth-discordbot-3.6.3/README.md` & `allianceauth_discordbot-3.6.4/README.md`

 * *Files 2% similar despite different names*

```diff
@@ -59,19 +59,19 @@
 
 * Install the app with your venv active
 
 ```bash
 pip install allianceauth-discordbot
 ```
 
-* Add `'aadiscordbot',` to your INSTALLED_APPS list in local.py.
+* Add `'aadiscordbot',` and  `'solo',` to your INSTALLED_APPS list in local.py.
 
 * Add the below lines to your `local.py` settings file, Changing the contexts to yours.
 
- ```python
+```python
 ## Settings for Allianceauth-Discordbot
 # Admin Commands
 ADMIN_DISCORD_BOT_CHANNELS = [111, 222, 333]
 # Sov Commands
 SOV_DISCORD_BOT_CHANNELS = [111, 222, 333]
 # Adm Commands
 ADM_DISCORD_BOT_CHANNELS = [111, 222, 333]
@@ -168,15 +168,20 @@
 ```ini
 #This block should already exist, add authbot to it
 [group:myauth]
 programs=beat,worker,gunicorn,authbot
 priority=999
 ```
 
-Last but not least, go to admin and configure your admin users in the bot config model.
+Go to admin and configure your admin users in the bot config model.
+
+> Enable groups/states/users to utilize the lookup command by adding permissions under **corputils | corp stats |**
+```ini
+corputils.view_alliance_corpstats
+```
 
 ## Reaction Roles
 > ❗❗❗ **This will bypass the Group Leadership/Join Request System**: This is intended for open groups but not limited to it! ❗❗❗
 
 The bot is able to run a reaction roles system that is compatible with auth and public users on a discord.
  - If a member is part of auth it will do auth syncing of roles
  - If a member is not found in auth and the reaction role message has the public flag set it will assign roles to anyone who reacts
```

### Comparing `allianceauth-discordbot-3.6.3/aadiscordbot/admin.py` & `allianceauth_discordbot-3.6.4/aadiscordbot/admin.py`

 * *Files identical despite different names*

### Comparing `allianceauth-discordbot-3.6.3/aadiscordbot/app_settings.py` & `allianceauth_discordbot-3.6.4/aadiscordbot/app_settings.py`

 * *Files identical despite different names*

### Comparing `allianceauth-discordbot-3.6.3/aadiscordbot/auth_hooks.py` & `allianceauth_discordbot-3.6.4/aadiscordbot/auth_hooks.py`

 * *Files identical despite different names*

### Comparing `allianceauth-discordbot-3.6.3/aadiscordbot/bot.py` & `allianceauth_discordbot-3.6.4/aadiscordbot/bot.py`

 * *Files identical despite different names*

### Comparing `allianceauth-discordbot-3.6.3/aadiscordbot/bot_tasks.py` & `allianceauth_discordbot-3.6.4/aadiscordbot/bot_tasks.py`

 * *Files identical despite different names*

### Comparing `allianceauth-discordbot-3.6.3/aadiscordbot/cogs/about.py` & `allianceauth_discordbot-3.6.4/aadiscordbot/cogs/about.py`

 * *Files identical despite different names*

### Comparing `allianceauth-discordbot-3.6.3/aadiscordbot/cogs/abuse.py` & `allianceauth_discordbot-3.6.4/aadiscordbot/cogs/abuse.py`

 * *Files identical despite different names*

### Comparing `allianceauth-discordbot-3.6.3/aadiscordbot/cogs/admin.py` & `allianceauth_discordbot-3.6.4/aadiscordbot/cogs/admin.py`

 * *Files identical despite different names*

### Comparing `allianceauth-discordbot-3.6.3/aadiscordbot/cogs/auth.py` & `allianceauth_discordbot-3.6.4/aadiscordbot/cogs/auth.py`

 * *Files identical despite different names*

### Comparing `allianceauth-discordbot-3.6.3/aadiscordbot/cogs/eastereggs.py` & `allianceauth_discordbot-3.6.4/aadiscordbot/cogs/eastereggs.py`

 * *Files identical despite different names*

### Comparing `allianceauth-discordbot-3.6.3/aadiscordbot/cogs/eightball.py` & `allianceauth_discordbot-3.6.4/aadiscordbot/cogs/eightball.py`

 * *Files identical despite different names*

### Comparing `allianceauth-discordbot-3.6.3/aadiscordbot/cogs/facwar.py` & `allianceauth_discordbot-3.6.4/aadiscordbot/cogs/facwar.py`

 * *Files identical despite different names*

### Comparing `allianceauth-discordbot-3.6.3/aadiscordbot/cogs/members.py` & `allianceauth_discordbot-3.6.4/aadiscordbot/cogs/members.py`

 * *Files identical despite different names*

### Comparing `allianceauth-discordbot-3.6.3/aadiscordbot/cogs/models.py` & `allianceauth_discordbot-3.6.4/aadiscordbot/cogs/models.py`

 * *Files identical despite different names*

### Comparing `allianceauth-discordbot-3.6.3/aadiscordbot/cogs/price_check.py` & `allianceauth_discordbot-3.6.4/aadiscordbot/cogs/price_check.py`

 * *Files identical despite different names*

### Comparing `allianceauth-discordbot-3.6.3/aadiscordbot/cogs/prom_export.py` & `allianceauth_discordbot-3.6.4/aadiscordbot/cogs/prom_export.py`

 * *Files identical despite different names*

### Comparing `allianceauth-discordbot-3.6.3/aadiscordbot/cogs/quote.py` & `allianceauth_discordbot-3.6.4/aadiscordbot/cogs/quote.py`

 * *Files identical despite different names*

### Comparing `allianceauth-discordbot-3.6.3/aadiscordbot/cogs/reaction_roles.py` & `allianceauth_discordbot-3.6.4/aadiscordbot/cogs/reaction_roles.py`

 * *Files identical despite different names*

### Comparing `allianceauth-discordbot-3.6.3/aadiscordbot/cogs/remind.py` & `allianceauth_discordbot-3.6.4/aadiscordbot/cogs/remind.py`

 * *Files identical despite different names*

### Comparing `allianceauth-discordbot-3.6.3/aadiscordbot/cogs/services.py` & `allianceauth_discordbot-3.6.4/aadiscordbot/cogs/services.py`

 * *Files identical despite different names*

### Comparing `allianceauth-discordbot-3.6.3/aadiscordbot/cogs/sov.py` & `allianceauth_discordbot-3.6.4/aadiscordbot/cogs/sov.py`

 * *Files identical despite different names*

### Comparing `allianceauth-discordbot-3.6.3/aadiscordbot/cogs/tickets.py` & `allianceauth_discordbot-3.6.4/aadiscordbot/cogs/tickets.py`

 * *Files identical despite different names*

### Comparing `allianceauth-discordbot-3.6.3/aadiscordbot/cogs/time.py` & `allianceauth_discordbot-3.6.4/aadiscordbot/cogs/time.py`

 * *Files identical despite different names*

### Comparing `allianceauth-discordbot-3.6.3/aadiscordbot/cogs/timers.py` & `allianceauth_discordbot-3.6.4/aadiscordbot/cogs/timers.py`

 * *Files identical despite different names*

### Comparing `allianceauth-discordbot-3.6.3/aadiscordbot/cogs/utils/decorators.py` & `allianceauth_discordbot-3.6.4/aadiscordbot/cogs/utils/decorators.py`

 * *Files identical despite different names*

### Comparing `allianceauth-discordbot-3.6.3/aadiscordbot/cogs/welcomegoodbye.py` & `allianceauth_discordbot-3.6.4/aadiscordbot/cogs/welcomegoodbye.py`

 * *Files identical despite different names*

### Comparing `allianceauth-discordbot-3.6.3/aadiscordbot/migrations/0001_initial.py` & `allianceauth_discordbot-3.6.4/aadiscordbot/migrations/0001_initial.py`

 * *Files identical despite different names*

### Comparing `allianceauth-discordbot-3.6.3/aadiscordbot/migrations/0002_reactionrolebinding_reactionrolemessage.py` & `allianceauth_discordbot-3.6.4/aadiscordbot/migrations/0002_reactionrolebinding_reactionrolemessage.py`

 * *Files identical despite different names*

### Comparing `allianceauth-discordbot-3.6.3/aadiscordbot/migrations/0003_authbotconfiguration.py` & `allianceauth_discordbot-3.6.4/aadiscordbot/migrations/0003_authbotconfiguration.py`

 * *Files identical despite different names*

### Comparing `allianceauth-discordbot-3.6.3/aadiscordbot/migrations/0005_rr_fixes_blank_admins.py` & `allianceauth_discordbot-3.6.4/aadiscordbot/migrations/0005_rr_fixes_blank_admins.py`

 * *Files identical despite different names*

### Comparing `allianceauth-discordbot-3.6.3/aadiscordbot/migrations/0006_goodbyemessage_welcomemessage.py` & `allianceauth_discordbot-3.6.4/aadiscordbot/migrations/0006_goodbyemessage_welcomemessage.py`

 * *Files identical despite different names*

### Comparing `allianceauth-discordbot-3.6.3/aadiscordbot/migrations/0007_quotemessage.py` & `allianceauth_discordbot-3.6.4/aadiscordbot/migrations/0007_quotemessage.py`

 * *Files identical despite different names*

### Comparing `allianceauth-discordbot-3.6.3/aadiscordbot/migrations/0010_alter_discordbot_options_ticketgroups.py` & `allianceauth_discordbot-3.6.4/aadiscordbot/migrations/0010_alter_discordbot_options_ticketgroups.py`

 * *Files identical despite different names*

### Comparing `allianceauth-discordbot-3.6.3/aadiscordbot/migrations/0011_alter_ticketgroups_options_and_more.py` & `allianceauth_discordbot-3.6.4/aadiscordbot/migrations/0011_alter_ticketgroups_options_and_more.py`

 * *Files identical despite different names*

### Comparing `allianceauth-discordbot-3.6.3/aadiscordbot/models.py` & `allianceauth_discordbot-3.6.4/aadiscordbot/models.py`

 * *Files identical despite different names*

### Comparing `allianceauth-discordbot-3.6.3/aadiscordbot/tasks.py` & `allianceauth_discordbot-3.6.4/aadiscordbot/tasks.py`

 * *Files identical despite different names*

