# Comparing `tmp/followthemoney-3.4.4.tar.gz` & `tmp/followthemoney-3.5.0.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "followthemoney-3.4.4.tar", last modified: Wed Jul 12 16:39:17 2023, max compression
+gzip compressed data, was "followthemoney-3.5.0.tar", last modified: Fri Jul 21 12:19:59 2023, max compression
```

## Comparing `followthemoney-3.4.4.tar` & `followthemoney-3.5.0.tar`

### file list

```diff
@@ -1,193 +1,195 @@
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-12 16:39:17.047757 followthemoney-3.4.4/
--rw-r--r--   0 runner    (1001) docker     (123)     1098 2023-07-12 16:37:14.000000 followthemoney-3.4.4/LICENSE
--rw-r--r--   0 runner    (1001) docker     (123)      167 2023-07-12 16:37:14.000000 followthemoney-3.4.4/MANIFEST.in
--rw-r--r--   0 runner    (1001) docker     (123)     2972 2023-07-12 16:39:17.047757 followthemoney-3.4.4/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (123)     2508 2023-07-12 16:37:14.000000 followthemoney-3.4.4/README.md
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-12 16:39:17.035758 followthemoney-3.4.4/followthemoney/
--rw-r--r--   0 runner    (1001) docker     (123)      360 2023-07-12 16:37:14.000000 followthemoney-3.4.4/followthemoney/__init__.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-12 16:39:17.035758 followthemoney-3.4.4/followthemoney/cli/
--rw-r--r--   0 runner    (1001) docker     (123)      111 2023-07-12 16:37:14.000000 followthemoney-3.4.4/followthemoney/cli/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)     2142 2023-07-12 16:37:14.000000 followthemoney-3.4.4/followthemoney/cli/aggregate.py
--rw-r--r--   0 runner    (1001) docker     (123)     3345 2023-07-12 16:37:14.000000 followthemoney-3.4.4/followthemoney/cli/cli.py
--rw-r--r--   0 runner    (1001) docker     (123)     4016 2023-07-12 16:37:14.000000 followthemoney-3.4.4/followthemoney/cli/exports.py
--rw-r--r--   0 runner    (1001) docker     (123)     3284 2023-07-12 16:37:14.000000 followthemoney-3.4.4/followthemoney/cli/mapping.py
--rw-r--r--   0 runner    (1001) docker     (123)     1940 2023-07-12 16:37:14.000000 followthemoney-3.4.4/followthemoney/cli/sieve.py
--rw-r--r--   0 runner    (1001) docker     (123)     4769 2023-07-12 16:37:14.000000 followthemoney-3.4.4/followthemoney/cli/util.py
--rw-r--r--   0 runner    (1001) docker     (123)     5134 2023-07-12 16:37:14.000000 followthemoney-3.4.4/followthemoney/compare.py
--rw-r--r--   0 runner    (1001) docker     (123)      734 2023-07-12 16:37:14.000000 followthemoney-3.4.4/followthemoney/exc.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-12 16:39:17.035758 followthemoney-3.4.4/followthemoney/export/
--rw-r--r--   0 runner    (1001) docker     (123)        0 2023-07-12 16:37:14.000000 followthemoney-3.4.4/followthemoney/export/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)      986 2023-07-12 16:37:14.000000 followthemoney-3.4.4/followthemoney/export/common.py
--rw-r--r--   0 runner    (1001) docker     (123)     2635 2023-07-12 16:37:14.000000 followthemoney-3.4.4/followthemoney/export/csv.py
--rw-r--r--   0 runner    (1001) docker     (123)     2718 2023-07-12 16:37:14.000000 followthemoney-3.4.4/followthemoney/export/excel.py
--rw-r--r--   0 runner    (1001) docker     (123)     2765 2023-07-12 16:37:14.000000 followthemoney-3.4.4/followthemoney/export/graph.py
--rw-r--r--   0 runner    (1001) docker     (123)     7104 2023-07-12 16:37:14.000000 followthemoney-3.4.4/followthemoney/export/neo4j.py
--rw-r--r--   0 runner    (1001) docker     (123)      786 2023-07-12 16:37:14.000000 followthemoney-3.4.4/followthemoney/export/rdf.py
--rw-r--r--   0 runner    (1001) docker     (123)    10848 2023-07-12 16:37:14.000000 followthemoney-3.4.4/followthemoney/graph.py
--rw-r--r--   0 runner    (1001) docker     (123)     7956 2023-07-12 16:37:14.000000 followthemoney-3.4.4/followthemoney/helpers.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-12 16:39:17.035758 followthemoney-3.4.4/followthemoney/mapping/
--rw-r--r--   0 runner    (1001) docker     (123)       82 2023-07-12 16:37:14.000000 followthemoney-3.4.4/followthemoney/mapping/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)     3197 2023-07-12 16:37:14.000000 followthemoney-3.4.4/followthemoney/mapping/csv.py
--rw-r--r--   0 runner    (1001) docker     (123)     4579 2023-07-12 16:37:14.000000 followthemoney-3.4.4/followthemoney/mapping/entity.py
--rw-r--r--   0 runner    (1001) docker     (123)     4535 2023-07-12 16:37:14.000000 followthemoney-3.4.4/followthemoney/mapping/property.py
--rw-r--r--   0 runner    (1001) docker     (123)     2622 2023-07-12 16:37:14.000000 followthemoney-3.4.4/followthemoney/mapping/query.py
--rw-r--r--   0 runner    (1001) docker     (123)      644 2023-07-12 16:37:14.000000 followthemoney-3.4.4/followthemoney/mapping/source.py
--rw-r--r--   0 runner    (1001) docker     (123)     4864 2023-07-12 16:37:14.000000 followthemoney-3.4.4/followthemoney/mapping/sql.py
--rw-r--r--   0 runner    (1001) docker     (123)      813 2023-07-12 16:37:14.000000 followthemoney-3.4.4/followthemoney/messages.py
--rw-r--r--   0 runner    (1001) docker     (123)     6426 2023-07-12 16:37:14.000000 followthemoney-3.4.4/followthemoney/model.py
--rw-r--r--   0 runner    (1001) docker     (123)     4443 2023-07-12 16:37:14.000000 followthemoney-3.4.4/followthemoney/namespace.py
--rw-r--r--   0 runner    (1001) docker     (123)     1060 2023-07-12 16:37:14.000000 followthemoney-3.4.4/followthemoney/offshore.py
--rw-r--r--   0 runner    (1001) docker     (123)     3002 2023-07-12 16:37:14.000000 followthemoney-3.4.4/followthemoney/ontology.py
--rw-r--r--   0 runner    (1001) docker     (123)     6811 2023-07-12 16:37:14.000000 followthemoney-3.4.4/followthemoney/property.py
--rw-r--r--   0 runner    (1001) docker     (123)    19866 2023-07-12 16:37:14.000000 followthemoney-3.4.4/followthemoney/proxy.py
--rw-r--r--   0 runner    (1001) docker     (123)        0 2023-07-12 16:37:14.000000 followthemoney-3.4.4/followthemoney/py.typed
--rw-r--r--   0 runner    (1001) docker     (123)      328 2023-07-12 16:37:14.000000 followthemoney-3.4.4/followthemoney/rdf.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-12 16:39:17.043758 followthemoney-3.4.4/followthemoney/schema/
--rw-r--r--   0 runner    (1001) docker     (123)     1689 2023-07-12 16:37:14.000000 followthemoney-3.4.4/followthemoney/schema/Address.yaml
--rw-r--r--   0 runner    (1001) docker     (123)      573 2023-07-12 16:37:14.000000 followthemoney-3.4.4/followthemoney/schema/Airplane.yaml
--rw-r--r--   0 runner    (1001) docker     (123)     1191 2023-07-12 16:37:14.000000 followthemoney-3.4.4/followthemoney/schema/Analyzable.yaml
--rw-r--r--   0 runner    (1001) docker     (123)      260 2023-07-12 16:37:14.000000 followthemoney-3.4.4/followthemoney/schema/Article.yaml
--rw-r--r--   0 runner    (1001) docker     (123)      624 2023-07-12 16:37:14.000000 followthemoney-3.4.4/followthemoney/schema/Assessment.yaml
--rw-r--r--   0 runner    (1001) docker     (123)      260 2023-07-12 16:37:14.000000 followthemoney-3.4.4/followthemoney/schema/Asset.yaml
--rw-r--r--   0 runner    (1001) docker     (123)      887 2023-07-12 16:37:14.000000 followthemoney-3.4.4/followthemoney/schema/Associate.yaml
--rw-r--r--   0 runner    (1001) docker     (123)      446 2023-07-12 16:37:14.000000 followthemoney-3.4.4/followthemoney/schema/Audio.yaml
--rw-r--r--   0 runner    (1001) docker     (123)     1323 2023-07-12 16:37:14.000000 followthemoney-3.4.4/followthemoney/schema/BankAccount.yaml
--rw-r--r--   0 runner    (1001) docker     (123)      980 2023-07-12 16:37:14.000000 followthemoney-3.4.4/followthemoney/schema/Call.yaml
--rw-r--r--   0 runner    (1001) docker     (123)     3227 2023-07-12 16:37:14.000000 followthemoney-3.4.4/followthemoney/schema/CallForTenders.yaml
--rw-r--r--   0 runner    (1001) docker     (123)     3140 2023-07-12 16:37:14.000000 followthemoney-3.4.4/followthemoney/schema/Company.yaml
--rw-r--r--   0 runner    (1001) docker     (123)     1580 2023-07-12 16:37:14.000000 followthemoney-3.4.4/followthemoney/schema/Contract.yaml
--rw-r--r--   0 runner    (1001) docker     (123)     1681 2023-07-12 16:37:14.000000 followthemoney-3.4.4/followthemoney/schema/ContractAward.yaml
--rw-r--r--   0 runner    (1001) docker     (123)      593 2023-07-12 16:37:14.000000 followthemoney-3.4.4/followthemoney/schema/CourtCase.yaml
--rw-r--r--   0 runner    (1001) docker     (123)      574 2023-07-12 16:37:14.000000 followthemoney-3.4.4/followthemoney/schema/CourtCaseParty.yaml
--rw-r--r--   0 runner    (1001) docker     (123)     1047 2023-07-12 16:37:14.000000 followthemoney-3.4.4/followthemoney/schema/CryptoWallet.yaml
--rw-r--r--   0 runner    (1001) docker     (123)      649 2023-07-12 16:37:14.000000 followthemoney-3.4.4/followthemoney/schema/Debt.yaml
--rw-r--r--   0 runner    (1001) docker     (123)      759 2023-07-12 16:37:14.000000 followthemoney-3.4.4/followthemoney/schema/Directorship.yaml
--rw-r--r--   0 runner    (1001) docker     (123)     2927 2023-07-12 16:37:14.000000 followthemoney-3.4.4/followthemoney/schema/Document.yaml
--rw-r--r--   0 runner    (1001) docker     (123)      747 2023-07-12 16:37:14.000000 followthemoney-3.4.4/followthemoney/schema/Documentation.yml
--rw-r--r--   0 runner    (1001) docker     (123)     4049 2023-07-12 16:37:14.000000 followthemoney-3.4.4/followthemoney/schema/EconomicActivity.yaml
--rw-r--r--   0 runner    (1001) docker     (123)     1549 2023-07-12 16:37:14.000000 followthemoney-3.4.4/followthemoney/schema/Email.yaml
--rw-r--r--   0 runner    (1001) docker     (123)      660 2023-07-12 16:37:14.000000 followthemoney-3.4.4/followthemoney/schema/Employment.yaml
--rw-r--r--   0 runner    (1001) docker     (123)      751 2023-07-12 16:37:14.000000 followthemoney-3.4.4/followthemoney/schema/Event.yaml
--rw-r--r--   0 runner    (1001) docker     (123)      969 2023-07-12 16:37:14.000000 followthemoney-3.4.4/followthemoney/schema/Family.yaml
--rw-r--r--   0 runner    (1001) docker     (123)      174 2023-07-12 16:37:14.000000 followthemoney-3.4.4/followthemoney/schema/Folder.yaml
--rw-r--r--   0 runner    (1001) docker     (123)      313 2023-07-12 16:37:14.000000 followthemoney-3.4.4/followthemoney/schema/HyperText.yaml
--rw-r--r--   0 runner    (1001) docker     (123)      827 2023-07-12 16:37:14.000000 followthemoney-3.4.4/followthemoney/schema/Identification.yaml
--rw-r--r--   0 runner    (1001) docker     (123)      388 2023-07-12 16:37:14.000000 followthemoney-3.4.4/followthemoney/schema/Image.yaml
--rw-r--r--   0 runner    (1001) docker     (123)      276 2023-07-12 16:37:14.000000 followthemoney-3.4.4/followthemoney/schema/Interest.yaml
--rw-r--r--   0 runner    (1001) docker     (123)     1919 2023-07-12 16:37:14.000000 followthemoney-3.4.4/followthemoney/schema/Interval.yaml
--rw-r--r--   0 runner    (1001) docker     (123)     3568 2023-07-12 16:37:14.000000 followthemoney-3.4.4/followthemoney/schema/LegalEntity.yaml
--rw-r--r--   0 runner    (1001) docker     (123)      452 2023-07-12 16:37:14.000000 followthemoney-3.4.4/followthemoney/schema/License.yaml
--rw-r--r--   0 runner    (1001) docker     (123)      696 2023-07-12 16:37:14.000000 followthemoney-3.4.4/followthemoney/schema/Membership.yaml
--rw-r--r--   0 runner    (1001) docker     (123)     1086 2023-07-12 16:37:14.000000 followthemoney-3.4.4/followthemoney/schema/Mention.yaml
--rw-r--r--   0 runner    (1001) docker     (123)     1484 2023-07-12 16:37:14.000000 followthemoney-3.4.4/followthemoney/schema/Message.yaml
--rw-r--r--   0 runner    (1001) docker     (123)      411 2023-07-12 16:37:14.000000 followthemoney-3.4.4/followthemoney/schema/Note.yaml
--rw-r--r--   0 runner    (1001) docker     (123)      424 2023-07-12 16:37:14.000000 followthemoney-3.4.4/followthemoney/schema/Organization.yaml
--rw-r--r--   0 runner    (1001) docker     (123)      983 2023-07-12 16:37:14.000000 followthemoney-3.4.4/followthemoney/schema/Ownership.yaml
--rw-r--r--   0 runner    (1001) docker     (123)      304 2023-07-12 16:37:14.000000 followthemoney-3.4.4/followthemoney/schema/Package.yaml
--rw-r--r--   0 runner    (1001) docker     (123)     1107 2023-07-12 16:37:14.000000 followthemoney-3.4.4/followthemoney/schema/Page.yaml
--rw-r--r--   0 runner    (1001) docker     (123)      444 2023-07-12 16:37:14.000000 followthemoney-3.4.4/followthemoney/schema/Pages.yaml
--rw-r--r--   0 runner    (1001) docker     (123)      730 2023-07-12 16:37:14.000000 followthemoney-3.4.4/followthemoney/schema/Passport.yaml
--rw-r--r--   0 runner    (1001) docker     (123)     1757 2023-07-12 16:37:14.000000 followthemoney-3.4.4/followthemoney/schema/Payment.yaml
--rw-r--r--   0 runner    (1001) docker     (123)     1586 2023-07-12 16:37:14.000000 followthemoney-3.4.4/followthemoney/schema/Person.yaml
--rw-r--r--   0 runner    (1001) docker     (123)      272 2023-07-12 16:37:14.000000 followthemoney-3.4.4/followthemoney/schema/PlainText.yaml
--rw-r--r--   0 runner    (1001) docker     (123)     1010 2023-07-12 16:37:14.000000 followthemoney-3.4.4/followthemoney/schema/Post.yaml
--rw-r--r--   0 runner    (1001) docker     (123)      461 2023-07-12 16:37:14.000000 followthemoney-3.4.4/followthemoney/schema/Project.yaml
--rw-r--r--   0 runner    (1001) docker     (123)      713 2023-07-12 16:37:14.000000 followthemoney-3.4.4/followthemoney/schema/ProjectParticipant.yaml
--rw-r--r--   0 runner    (1001) docker     (123)      295 2023-07-12 16:37:14.000000 followthemoney-3.4.4/followthemoney/schema/PublicBody.yaml
--rw-r--r--   0 runner    (1001) docker     (123)     1118 2023-07-12 16:37:14.000000 followthemoney-3.4.4/followthemoney/schema/RealEstate.yaml
--rw-r--r--   0 runner    (1001) docker     (123)      778 2023-07-12 16:37:14.000000 followthemoney-3.4.4/followthemoney/schema/Representation.yaml
--rw-r--r--   0 runner    (1001) docker     (123)      931 2023-07-12 16:37:14.000000 followthemoney-3.4.4/followthemoney/schema/Sanction.yaml
--rw-r--r--   0 runner    (1001) docker     (123)      993 2023-07-12 16:37:14.000000 followthemoney-3.4.4/followthemoney/schema/Security.yaml
--rw-r--r--   0 runner    (1001) docker     (123)      817 2023-07-12 16:37:14.000000 followthemoney-3.4.4/followthemoney/schema/Similar.yaml
--rw-r--r--   0 runner    (1001) docker     (123)      735 2023-07-12 16:37:14.000000 followthemoney-3.4.4/followthemoney/schema/Succession.yaml
--rw-r--r--   0 runner    (1001) docker     (123)      635 2023-07-12 16:37:14.000000 followthemoney-3.4.4/followthemoney/schema/Table.yaml
--rw-r--r--   0 runner    (1001) docker     (123)      740 2023-07-12 16:37:14.000000 followthemoney-3.4.4/followthemoney/schema/TaxRoll.yaml
--rw-r--r--   0 runner    (1001) docker     (123)     2403 2023-07-12 16:37:14.000000 followthemoney-3.4.4/followthemoney/schema/Thing.yaml
--rw-r--r--   0 runner    (1001) docker     (123)      771 2023-07-12 16:37:14.000000 followthemoney-3.4.4/followthemoney/schema/Trip.yaml
--rw-r--r--   0 runner    (1001) docker     (123)      668 2023-07-12 16:37:14.000000 followthemoney-3.4.4/followthemoney/schema/UnknownLink.yaml
--rw-r--r--   0 runner    (1001) docker     (123)      763 2023-07-12 16:37:14.000000 followthemoney-3.4.4/followthemoney/schema/UserAccount.yaml
--rw-r--r--   0 runner    (1001) docker     (123)      310 2023-07-12 16:37:14.000000 followthemoney-3.4.4/followthemoney/schema/Value.yaml
--rw-r--r--   0 runner    (1001) docker     (123)      984 2023-07-12 16:37:14.000000 followthemoney-3.4.4/followthemoney/schema/Vehicle.yaml
--rw-r--r--   0 runner    (1001) docker     (123)      993 2023-07-12 16:37:14.000000 followthemoney-3.4.4/followthemoney/schema/Vessel.yaml
--rw-r--r--   0 runner    (1001) docker     (123)      321 2023-07-12 16:37:14.000000 followthemoney-3.4.4/followthemoney/schema/Video.yaml
--rw-r--r--   0 runner    (1001) docker     (123)      348 2023-07-12 16:37:14.000000 followthemoney-3.4.4/followthemoney/schema/Workbook.yaml
--rw-r--r--   0 runner    (1001) docker     (123)    16469 2023-07-12 16:37:14.000000 followthemoney-3.4.4/followthemoney/schema.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-12 16:39:17.043758 followthemoney-3.4.4/followthemoney/translations/
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-12 16:39:17.031758 followthemoney-3.4.4/followthemoney/translations/ar/
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-12 16:39:17.043758 followthemoney-3.4.4/followthemoney/translations/ar/LC_MESSAGES/
--rw-r--r--   0 runner    (1001) docker     (123)    38829 2023-07-12 16:37:14.000000 followthemoney-3.4.4/followthemoney/translations/ar/LC_MESSAGES/followthemoney.mo
--rw-r--r--   0 runner    (1001) docker     (123)   118608 2023-07-12 16:37:14.000000 followthemoney-3.4.4/followthemoney/translations/ar/LC_MESSAGES/followthemoney.po
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-12 16:39:17.031758 followthemoney-3.4.4/followthemoney/translations/bs/
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-12 16:39:17.043758 followthemoney-3.4.4/followthemoney/translations/bs/LC_MESSAGES/
--rw-r--r--   0 runner    (1001) docker     (123)    10751 2023-07-12 16:37:14.000000 followthemoney-3.4.4/followthemoney/translations/bs/LC_MESSAGES/followthemoney.mo
--rw-r--r--   0 runner    (1001) docker     (123)    93147 2023-07-12 16:37:14.000000 followthemoney-3.4.4/followthemoney/translations/bs/LC_MESSAGES/followthemoney.po
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-12 16:39:17.031758 followthemoney-3.4.4/followthemoney/translations/de/
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-12 16:39:17.043758 followthemoney-3.4.4/followthemoney/translations/de/LC_MESSAGES/
--rw-r--r--   0 runner    (1001) docker     (123)    36107 2023-07-12 16:37:14.000000 followthemoney-3.4.4/followthemoney/translations/de/LC_MESSAGES/followthemoney.mo
--rw-r--r--   0 runner    (1001) docker     (123)   112813 2023-07-12 16:37:14.000000 followthemoney-3.4.4/followthemoney/translations/de/LC_MESSAGES/followthemoney.po
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-12 16:39:17.031758 followthemoney-3.4.4/followthemoney/translations/es/
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-12 16:39:17.043758 followthemoney-3.4.4/followthemoney/translations/es/LC_MESSAGES/
--rw-r--r--   0 runner    (1001) docker     (123)    32176 2023-07-12 16:37:14.000000 followthemoney-3.4.4/followthemoney/translations/es/LC_MESSAGES/followthemoney.mo
--rw-r--r--   0 runner    (1001) docker     (123)   112460 2023-07-12 16:37:14.000000 followthemoney-3.4.4/followthemoney/translations/es/LC_MESSAGES/followthemoney.po
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-12 16:39:17.043758 followthemoney-3.4.4/followthemoney/translations/fr/
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-12 16:39:17.043758 followthemoney-3.4.4/followthemoney/translations/fr/LC_MESSAGES/
--rw-r--r--   0 runner    (1001) docker     (123)    42553 2023-07-12 16:37:14.000000 followthemoney-3.4.4/followthemoney/translations/fr/LC_MESSAGES/followthemoney.mo
--rw-r--r--   0 runner    (1001) docker     (123)   117244 2023-07-12 16:37:14.000000 followthemoney-3.4.4/followthemoney/translations/fr/LC_MESSAGES/followthemoney.po
--rw-r--r--   0 runner    (1001) docker     (123)   106802 2023-07-12 16:37:14.000000 followthemoney-3.4.4/followthemoney/translations/fr/followthemoney.po
--rw-r--r--   0 runner    (1001) docker     (123)   101212 2023-07-12 16:37:14.000000 followthemoney-3.4.4/followthemoney/translations/messages.pot
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-12 16:39:17.031758 followthemoney-3.4.4/followthemoney/translations/nb/
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-12 16:39:17.043758 followthemoney-3.4.4/followthemoney/translations/nb/LC_MESSAGES/
--rw-r--r--   0 runner    (1001) docker     (123)      498 2023-07-12 16:37:14.000000 followthemoney-3.4.4/followthemoney/translations/nb/LC_MESSAGES/followthemoney.mo
--rw-r--r--   0 runner    (1001) docker     (123)    89796 2023-07-12 16:37:14.000000 followthemoney-3.4.4/followthemoney/translations/nb/LC_MESSAGES/followthemoney.po
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-12 16:39:17.031758 followthemoney-3.4.4/followthemoney/translations/nl/
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-12 16:39:17.043758 followthemoney-3.4.4/followthemoney/translations/nl/LC_MESSAGES/
--rw-r--r--   0 runner    (1001) docker     (123)      486 2023-07-12 16:37:14.000000 followthemoney-3.4.4/followthemoney/translations/nl/LC_MESSAGES/followthemoney.mo
--rw-r--r--   0 runner    (1001) docker     (123)    90876 2023-07-12 16:37:14.000000 followthemoney-3.4.4/followthemoney/translations/nl/LC_MESSAGES/followthemoney.po
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-12 16:39:17.031758 followthemoney-3.4.4/followthemoney/translations/pt_BR/
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-12 16:39:17.043758 followthemoney-3.4.4/followthemoney/translations/pt_BR/LC_MESSAGES/
--rw-r--r--   0 runner    (1001) docker     (123)      505 2023-07-12 16:37:14.000000 followthemoney-3.4.4/followthemoney/translations/pt_BR/LC_MESSAGES/followthemoney.mo
--rw-r--r--   0 runner    (1001) docker     (123)    89847 2023-07-12 16:37:14.000000 followthemoney-3.4.4/followthemoney/translations/pt_BR/LC_MESSAGES/followthemoney.po
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-12 16:39:17.043758 followthemoney-3.4.4/followthemoney/translations/ru/
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-12 16:39:17.047757 followthemoney-3.4.4/followthemoney/translations/ru/LC_MESSAGES/
--rw-r--r--   0 runner    (1001) docker     (123)    61971 2023-07-12 16:37:14.000000 followthemoney-3.4.4/followthemoney/translations/ru/LC_MESSAGES/followthemoney.mo
--rw-r--r--   0 runner    (1001) docker     (123)   132951 2023-07-12 16:37:14.000000 followthemoney-3.4.4/followthemoney/translations/ru/LC_MESSAGES/followthemoney.po
--rw-r--r--   0 runner    (1001) docker     (123)   130621 2023-07-12 16:37:14.000000 followthemoney-3.4.4/followthemoney/translations/ru/followthemoney.po
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-12 16:39:17.031758 followthemoney-3.4.4/followthemoney/translations/tr/
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-12 16:39:17.047757 followthemoney-3.4.4/followthemoney/translations/tr/LC_MESSAGES/
--rw-r--r--   0 runner    (1001) docker     (123)      487 2023-07-12 16:37:14.000000 followthemoney-3.4.4/followthemoney/translations/tr/LC_MESSAGES/followthemoney.mo
--rw-r--r--   0 runner    (1001) docker     (123)    89829 2023-07-12 16:37:14.000000 followthemoney-3.4.4/followthemoney/translations/tr/LC_MESSAGES/followthemoney.po
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-12 16:39:17.047757 followthemoney-3.4.4/followthemoney/types/
--rw-r--r--   0 runner    (1001) docker     (123)     1690 2023-07-12 16:37:14.000000 followthemoney-3.4.4/followthemoney/types/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)     1651 2023-07-12 16:37:14.000000 followthemoney-3.4.4/followthemoney/types/address.py
--rw-r--r--   0 runner    (1001) docker     (123)      917 2023-07-12 16:37:14.000000 followthemoney-3.4.4/followthemoney/types/checksum.py
--rw-r--r--   0 runner    (1001) docker     (123)     9560 2023-07-12 16:37:14.000000 followthemoney-3.4.4/followthemoney/types/common.py
--rw-r--r--   0 runner    (1001) docker     (123)     3053 2023-07-12 16:37:14.000000 followthemoney-3.4.4/followthemoney/types/country.py
--rw-r--r--   0 runner    (1001) docker     (123)     2500 2023-07-12 16:37:14.000000 followthemoney-3.4.4/followthemoney/types/date.py
--rw-r--r--   0 runner    (1001) docker     (123)     2680 2023-07-12 16:37:14.000000 followthemoney-3.4.4/followthemoney/types/email.py
--rw-r--r--   0 runner    (1001) docker     (123)     2366 2023-07-12 16:37:14.000000 followthemoney-3.4.4/followthemoney/types/entity.py
--rw-r--r--   0 runner    (1001) docker     (123)     1800 2023-07-12 16:37:14.000000 followthemoney-3.4.4/followthemoney/types/gender.py
--rw-r--r--   0 runner    (1001) docker     (123)     1848 2023-07-12 16:37:14.000000 followthemoney-3.4.4/followthemoney/types/iban.py
--rw-r--r--   0 runner    (1001) docker     (123)     1510 2023-07-12 16:37:14.000000 followthemoney-3.4.4/followthemoney/types/identifier.py
--rw-r--r--   0 runner    (1001) docker     (123)     1327 2023-07-12 16:37:14.000000 followthemoney-3.4.4/followthemoney/types/ip.py
--rw-r--r--   0 runner    (1001) docker     (123)     1676 2023-07-12 16:37:14.000000 followthemoney-3.4.4/followthemoney/types/json.py
--rw-r--r--   0 runner    (1001) docker     (123)     2613 2023-07-12 16:37:14.000000 followthemoney-3.4.4/followthemoney/types/language.py
--rw-r--r--   0 runner    (1001) docker     (123)     1351 2023-07-12 16:37:14.000000 followthemoney-3.4.4/followthemoney/types/mimetype.py
--rw-r--r--   0 runner    (1001) docker     (123)     2855 2023-07-12 16:37:14.000000 followthemoney-3.4.4/followthemoney/types/name.py
--rw-r--r--   0 runner    (1001) docker     (123)      943 2023-07-12 16:37:14.000000 followthemoney-3.4.4/followthemoney/types/number.py
--rw-r--r--   0 runner    (1001) docker     (123)     3955 2023-07-12 16:37:14.000000 followthemoney-3.4.4/followthemoney/types/phone.py
--rw-r--r--   0 runner    (1001) docker     (123)     1936 2023-07-12 16:37:14.000000 followthemoney-3.4.4/followthemoney/types/registry.py
--rw-r--r--   0 runner    (1001) docker     (123)     1130 2023-07-12 16:37:14.000000 followthemoney-3.4.4/followthemoney/types/string.py
--rw-r--r--   0 runner    (1001) docker     (123)     2844 2023-07-12 16:37:14.000000 followthemoney-3.4.4/followthemoney/types/topic.py
--rw-r--r--   0 runner    (1001) docker     (123)     2162 2023-07-12 16:37:14.000000 followthemoney-3.4.4/followthemoney/types/url.py
--rw-r--r--   0 runner    (1001) docker     (123)     4508 2023-07-12 16:37:14.000000 followthemoney-3.4.4/followthemoney/util.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-12 16:39:17.035758 followthemoney-3.4.4/followthemoney.egg-info/
--rw-r--r--   0 runner    (1001) docker     (123)     2972 2023-07-12 16:39:16.000000 followthemoney-3.4.4/followthemoney.egg-info/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (123)     5927 2023-07-12 16:39:16.000000 followthemoney-3.4.4/followthemoney.egg-info/SOURCES.txt
--rw-r--r--   0 runner    (1001) docker     (123)        1 2023-07-12 16:39:16.000000 followthemoney-3.4.4/followthemoney.egg-info/dependency_links.txt
--rw-r--r--   0 runner    (1001) docker     (123)      593 2023-07-12 16:39:16.000000 followthemoney-3.4.4/followthemoney.egg-info/entry_points.txt
--rw-r--r--   0 runner    (1001) docker     (123)        1 2023-07-12 16:39:16.000000 followthemoney-3.4.4/followthemoney.egg-info/namespace_packages.txt
--rw-r--r--   0 runner    (1001) docker     (123)        1 2023-07-12 16:38:55.000000 followthemoney-3.4.4/followthemoney.egg-info/not-zip-safe
--rw-r--r--   0 runner    (1001) docker     (123)      725 2023-07-12 16:39:16.000000 followthemoney-3.4.4/followthemoney.egg-info/requires.txt
--rw-r--r--   0 runner    (1001) docker     (123)       21 2023-07-12 16:39:16.000000 followthemoney-3.4.4/followthemoney.egg-info/top_level.txt
--rw-r--r--   0 runner    (1001) docker     (123)      131 2023-07-12 16:39:17.047757 followthemoney-3.4.4/setup.cfg
--rw-r--r--   0 runner    (1001) docker     (123)     3214 2023-07-12 16:37:14.000000 followthemoney-3.4.4/setup.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-21 12:19:59.131589 followthemoney-3.5.0/
+-rw-r--r--   0 runner    (1001) docker     (123)     1098 2023-07-21 12:18:02.000000 followthemoney-3.5.0/LICENSE
+-rw-r--r--   0 runner    (1001) docker     (123)      167 2023-07-21 12:18:02.000000 followthemoney-3.5.0/MANIFEST.in
+-rw-r--r--   0 runner    (1001) docker     (123)     3598 2023-07-21 12:19:59.131589 followthemoney-3.5.0/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (123)     2508 2023-07-21 12:18:02.000000 followthemoney-3.5.0/README.md
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-21 12:19:59.111589 followthemoney-3.5.0/followthemoney/
+-rw-r--r--   0 runner    (1001) docker     (123)      360 2023-07-21 12:18:02.000000 followthemoney-3.5.0/followthemoney/__init__.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-21 12:19:59.115589 followthemoney-3.5.0/followthemoney/cli/
+-rw-r--r--   0 runner    (1001) docker     (123)      111 2023-07-21 12:18:02.000000 followthemoney-3.5.0/followthemoney/cli/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)     2142 2023-07-21 12:18:02.000000 followthemoney-3.5.0/followthemoney/cli/aggregate.py
+-rw-r--r--   0 runner    (1001) docker     (123)     3345 2023-07-21 12:18:02.000000 followthemoney-3.5.0/followthemoney/cli/cli.py
+-rw-r--r--   0 runner    (1001) docker     (123)     4016 2023-07-21 12:18:02.000000 followthemoney-3.5.0/followthemoney/cli/exports.py
+-rw-r--r--   0 runner    (1001) docker     (123)     3284 2023-07-21 12:18:02.000000 followthemoney-3.5.0/followthemoney/cli/mapping.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1940 2023-07-21 12:18:02.000000 followthemoney-3.5.0/followthemoney/cli/sieve.py
+-rw-r--r--   0 runner    (1001) docker     (123)     4769 2023-07-21 12:18:02.000000 followthemoney-3.5.0/followthemoney/cli/util.py
+-rw-r--r--   0 runner    (1001) docker     (123)     5134 2023-07-21 12:18:02.000000 followthemoney-3.5.0/followthemoney/compare.py
+-rw-r--r--   0 runner    (1001) docker     (123)      734 2023-07-21 12:18:02.000000 followthemoney-3.5.0/followthemoney/exc.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-21 12:19:59.115589 followthemoney-3.5.0/followthemoney/export/
+-rw-r--r--   0 runner    (1001) docker     (123)        0 2023-07-21 12:18:02.000000 followthemoney-3.5.0/followthemoney/export/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)      986 2023-07-21 12:18:02.000000 followthemoney-3.5.0/followthemoney/export/common.py
+-rw-r--r--   0 runner    (1001) docker     (123)     2635 2023-07-21 12:18:02.000000 followthemoney-3.5.0/followthemoney/export/csv.py
+-rw-r--r--   0 runner    (1001) docker     (123)     2718 2023-07-21 12:18:02.000000 followthemoney-3.5.0/followthemoney/export/excel.py
+-rw-r--r--   0 runner    (1001) docker     (123)     2765 2023-07-21 12:18:02.000000 followthemoney-3.5.0/followthemoney/export/graph.py
+-rw-r--r--   0 runner    (1001) docker     (123)     7104 2023-07-21 12:18:02.000000 followthemoney-3.5.0/followthemoney/export/neo4j.py
+-rw-r--r--   0 runner    (1001) docker     (123)      786 2023-07-21 12:18:02.000000 followthemoney-3.5.0/followthemoney/export/rdf.py
+-rw-r--r--   0 runner    (1001) docker     (123)    10848 2023-07-21 12:18:02.000000 followthemoney-3.5.0/followthemoney/graph.py
+-rw-r--r--   0 runner    (1001) docker     (123)     7956 2023-07-21 12:18:02.000000 followthemoney-3.5.0/followthemoney/helpers.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-21 12:19:59.115589 followthemoney-3.5.0/followthemoney/mapping/
+-rw-r--r--   0 runner    (1001) docker     (123)       82 2023-07-21 12:18:02.000000 followthemoney-3.5.0/followthemoney/mapping/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)     3197 2023-07-21 12:18:02.000000 followthemoney-3.5.0/followthemoney/mapping/csv.py
+-rw-r--r--   0 runner    (1001) docker     (123)     4798 2023-07-21 12:18:02.000000 followthemoney-3.5.0/followthemoney/mapping/entity.py
+-rw-r--r--   0 runner    (1001) docker     (123)     4763 2023-07-21 12:18:02.000000 followthemoney-3.5.0/followthemoney/mapping/property.py
+-rw-r--r--   0 runner    (1001) docker     (123)     2622 2023-07-21 12:18:02.000000 followthemoney-3.5.0/followthemoney/mapping/query.py
+-rw-r--r--   0 runner    (1001) docker     (123)      644 2023-07-21 12:18:02.000000 followthemoney-3.5.0/followthemoney/mapping/source.py
+-rw-r--r--   0 runner    (1001) docker     (123)     4864 2023-07-21 12:18:02.000000 followthemoney-3.5.0/followthemoney/mapping/sql.py
+-rw-r--r--   0 runner    (1001) docker     (123)      813 2023-07-21 12:18:02.000000 followthemoney-3.5.0/followthemoney/messages.py
+-rw-r--r--   0 runner    (1001) docker     (123)     6426 2023-07-21 12:18:02.000000 followthemoney-3.5.0/followthemoney/model.py
+-rw-r--r--   0 runner    (1001) docker     (123)     4443 2023-07-21 12:18:02.000000 followthemoney-3.5.0/followthemoney/namespace.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1060 2023-07-21 12:18:02.000000 followthemoney-3.5.0/followthemoney/offshore.py
+-rw-r--r--   0 runner    (1001) docker     (123)     3002 2023-07-21 12:18:02.000000 followthemoney-3.5.0/followthemoney/ontology.py
+-rw-r--r--   0 runner    (1001) docker     (123)     7052 2023-07-21 12:18:02.000000 followthemoney-3.5.0/followthemoney/property.py
+-rw-r--r--   0 runner    (1001) docker     (123)    19866 2023-07-21 12:18:02.000000 followthemoney-3.5.0/followthemoney/proxy.py
+-rw-r--r--   0 runner    (1001) docker     (123)        0 2023-07-21 12:18:02.000000 followthemoney-3.5.0/followthemoney/py.typed
+-rw-r--r--   0 runner    (1001) docker     (123)      328 2023-07-21 12:18:02.000000 followthemoney-3.5.0/followthemoney/rdf.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-21 12:19:59.123589 followthemoney-3.5.0/followthemoney/schema/
+-rw-r--r--   0 runner    (1001) docker     (123)     1689 2023-07-21 12:18:02.000000 followthemoney-3.5.0/followthemoney/schema/Address.yaml
+-rw-r--r--   0 runner    (1001) docker     (123)      573 2023-07-21 12:18:02.000000 followthemoney-3.5.0/followthemoney/schema/Airplane.yaml
+-rw-r--r--   0 runner    (1001) docker     (123)     1191 2023-07-21 12:18:02.000000 followthemoney-3.5.0/followthemoney/schema/Analyzable.yaml
+-rw-r--r--   0 runner    (1001) docker     (123)      260 2023-07-21 12:18:02.000000 followthemoney-3.5.0/followthemoney/schema/Article.yaml
+-rw-r--r--   0 runner    (1001) docker     (123)      624 2023-07-21 12:18:02.000000 followthemoney-3.5.0/followthemoney/schema/Assessment.yaml
+-rw-r--r--   0 runner    (1001) docker     (123)      260 2023-07-21 12:18:02.000000 followthemoney-3.5.0/followthemoney/schema/Asset.yaml
+-rw-r--r--   0 runner    (1001) docker     (123)      887 2023-07-21 12:18:02.000000 followthemoney-3.5.0/followthemoney/schema/Associate.yaml
+-rw-r--r--   0 runner    (1001) docker     (123)      446 2023-07-21 12:18:02.000000 followthemoney-3.5.0/followthemoney/schema/Audio.yaml
+-rw-r--r--   0 runner    (1001) docker     (123)     1323 2023-07-21 12:18:02.000000 followthemoney-3.5.0/followthemoney/schema/BankAccount.yaml
+-rw-r--r--   0 runner    (1001) docker     (123)      980 2023-07-21 12:18:02.000000 followthemoney-3.5.0/followthemoney/schema/Call.yaml
+-rw-r--r--   0 runner    (1001) docker     (123)     3227 2023-07-21 12:18:02.000000 followthemoney-3.5.0/followthemoney/schema/CallForTenders.yaml
+-rw-r--r--   0 runner    (1001) docker     (123)     3140 2023-07-21 12:18:02.000000 followthemoney-3.5.0/followthemoney/schema/Company.yaml
+-rw-r--r--   0 runner    (1001) docker     (123)     1580 2023-07-21 12:18:02.000000 followthemoney-3.5.0/followthemoney/schema/Contract.yaml
+-rw-r--r--   0 runner    (1001) docker     (123)     1681 2023-07-21 12:18:02.000000 followthemoney-3.5.0/followthemoney/schema/ContractAward.yaml
+-rw-r--r--   0 runner    (1001) docker     (123)      593 2023-07-21 12:18:02.000000 followthemoney-3.5.0/followthemoney/schema/CourtCase.yaml
+-rw-r--r--   0 runner    (1001) docker     (123)      574 2023-07-21 12:18:02.000000 followthemoney-3.5.0/followthemoney/schema/CourtCaseParty.yaml
+-rw-r--r--   0 runner    (1001) docker     (123)     1047 2023-07-21 12:18:02.000000 followthemoney-3.5.0/followthemoney/schema/CryptoWallet.yaml
+-rw-r--r--   0 runner    (1001) docker     (123)      649 2023-07-21 12:18:02.000000 followthemoney-3.5.0/followthemoney/schema/Debt.yaml
+-rw-r--r--   0 runner    (1001) docker     (123)      759 2023-07-21 12:18:02.000000 followthemoney-3.5.0/followthemoney/schema/Directorship.yaml
+-rw-r--r--   0 runner    (1001) docker     (123)     2927 2023-07-21 12:18:02.000000 followthemoney-3.5.0/followthemoney/schema/Document.yaml
+-rw-r--r--   0 runner    (1001) docker     (123)      747 2023-07-21 12:18:02.000000 followthemoney-3.5.0/followthemoney/schema/Documentation.yml
+-rw-r--r--   0 runner    (1001) docker     (123)     4049 2023-07-21 12:18:02.000000 followthemoney-3.5.0/followthemoney/schema/EconomicActivity.yaml
+-rw-r--r--   0 runner    (1001) docker     (123)     1549 2023-07-21 12:18:02.000000 followthemoney-3.5.0/followthemoney/schema/Email.yaml
+-rw-r--r--   0 runner    (1001) docker     (123)      660 2023-07-21 12:18:02.000000 followthemoney-3.5.0/followthemoney/schema/Employment.yaml
+-rw-r--r--   0 runner    (1001) docker     (123)      751 2023-07-21 12:18:02.000000 followthemoney-3.5.0/followthemoney/schema/Event.yaml
+-rw-r--r--   0 runner    (1001) docker     (123)      969 2023-07-21 12:18:02.000000 followthemoney-3.5.0/followthemoney/schema/Family.yaml
+-rw-r--r--   0 runner    (1001) docker     (123)      174 2023-07-21 12:18:02.000000 followthemoney-3.5.0/followthemoney/schema/Folder.yaml
+-rw-r--r--   0 runner    (1001) docker     (123)      313 2023-07-21 12:18:02.000000 followthemoney-3.5.0/followthemoney/schema/HyperText.yaml
+-rw-r--r--   0 runner    (1001) docker     (123)      827 2023-07-21 12:18:02.000000 followthemoney-3.5.0/followthemoney/schema/Identification.yaml
+-rw-r--r--   0 runner    (1001) docker     (123)      388 2023-07-21 12:18:02.000000 followthemoney-3.5.0/followthemoney/schema/Image.yaml
+-rw-r--r--   0 runner    (1001) docker     (123)      276 2023-07-21 12:18:02.000000 followthemoney-3.5.0/followthemoney/schema/Interest.yaml
+-rw-r--r--   0 runner    (1001) docker     (123)     1919 2023-07-21 12:18:02.000000 followthemoney-3.5.0/followthemoney/schema/Interval.yaml
+-rw-r--r--   0 runner    (1001) docker     (123)     3568 2023-07-21 12:18:02.000000 followthemoney-3.5.0/followthemoney/schema/LegalEntity.yaml
+-rw-r--r--   0 runner    (1001) docker     (123)      452 2023-07-21 12:18:02.000000 followthemoney-3.5.0/followthemoney/schema/License.yaml
+-rw-r--r--   0 runner    (1001) docker     (123)      696 2023-07-21 12:18:02.000000 followthemoney-3.5.0/followthemoney/schema/Membership.yaml
+-rw-r--r--   0 runner    (1001) docker     (123)     1086 2023-07-21 12:18:02.000000 followthemoney-3.5.0/followthemoney/schema/Mention.yaml
+-rw-r--r--   0 runner    (1001) docker     (123)     1484 2023-07-21 12:18:02.000000 followthemoney-3.5.0/followthemoney/schema/Message.yaml
+-rw-r--r--   0 runner    (1001) docker     (123)      411 2023-07-21 12:18:02.000000 followthemoney-3.5.0/followthemoney/schema/Note.yaml
+-rw-r--r--   0 runner    (1001) docker     (123)      774 2023-07-21 12:18:02.000000 followthemoney-3.5.0/followthemoney/schema/Occupancy.yaml
+-rw-r--r--   0 runner    (1001) docker     (123)      424 2023-07-21 12:18:02.000000 followthemoney-3.5.0/followthemoney/schema/Organization.yaml
+-rw-r--r--   0 runner    (1001) docker     (123)      983 2023-07-21 12:18:02.000000 followthemoney-3.5.0/followthemoney/schema/Ownership.yaml
+-rw-r--r--   0 runner    (1001) docker     (123)      304 2023-07-21 12:18:02.000000 followthemoney-3.5.0/followthemoney/schema/Package.yaml
+-rw-r--r--   0 runner    (1001) docker     (123)     1107 2023-07-21 12:18:02.000000 followthemoney-3.5.0/followthemoney/schema/Page.yaml
+-rw-r--r--   0 runner    (1001) docker     (123)      444 2023-07-21 12:18:02.000000 followthemoney-3.5.0/followthemoney/schema/Pages.yaml
+-rw-r--r--   0 runner    (1001) docker     (123)      730 2023-07-21 12:18:02.000000 followthemoney-3.5.0/followthemoney/schema/Passport.yaml
+-rw-r--r--   0 runner    (1001) docker     (123)     1757 2023-07-21 12:18:02.000000 followthemoney-3.5.0/followthemoney/schema/Payment.yaml
+-rw-r--r--   0 runner    (1001) docker     (123)     1586 2023-07-21 12:18:02.000000 followthemoney-3.5.0/followthemoney/schema/Person.yaml
+-rw-r--r--   0 runner    (1001) docker     (123)      272 2023-07-21 12:18:02.000000 followthemoney-3.5.0/followthemoney/schema/PlainText.yaml
+-rw-r--r--   0 runner    (1001) docker     (123)     1287 2023-07-21 12:18:02.000000 followthemoney-3.5.0/followthemoney/schema/Position.yaml
+-rw-r--r--   0 runner    (1001) docker     (123)     1029 2023-07-21 12:18:02.000000 followthemoney-3.5.0/followthemoney/schema/Post.yaml
+-rw-r--r--   0 runner    (1001) docker     (123)      461 2023-07-21 12:18:02.000000 followthemoney-3.5.0/followthemoney/schema/Project.yaml
+-rw-r--r--   0 runner    (1001) docker     (123)      713 2023-07-21 12:18:02.000000 followthemoney-3.5.0/followthemoney/schema/ProjectParticipant.yaml
+-rw-r--r--   0 runner    (1001) docker     (123)      295 2023-07-21 12:18:02.000000 followthemoney-3.5.0/followthemoney/schema/PublicBody.yaml
+-rw-r--r--   0 runner    (1001) docker     (123)     1118 2023-07-21 12:18:02.000000 followthemoney-3.5.0/followthemoney/schema/RealEstate.yaml
+-rw-r--r--   0 runner    (1001) docker     (123)      778 2023-07-21 12:18:02.000000 followthemoney-3.5.0/followthemoney/schema/Representation.yaml
+-rw-r--r--   0 runner    (1001) docker     (123)      931 2023-07-21 12:18:02.000000 followthemoney-3.5.0/followthemoney/schema/Sanction.yaml
+-rw-r--r--   0 runner    (1001) docker     (123)      993 2023-07-21 12:18:02.000000 followthemoney-3.5.0/followthemoney/schema/Security.yaml
+-rw-r--r--   0 runner    (1001) docker     (123)      817 2023-07-21 12:18:02.000000 followthemoney-3.5.0/followthemoney/schema/Similar.yaml
+-rw-r--r--   0 runner    (1001) docker     (123)      735 2023-07-21 12:18:02.000000 followthemoney-3.5.0/followthemoney/schema/Succession.yaml
+-rw-r--r--   0 runner    (1001) docker     (123)      635 2023-07-21 12:18:02.000000 followthemoney-3.5.0/followthemoney/schema/Table.yaml
+-rw-r--r--   0 runner    (1001) docker     (123)      740 2023-07-21 12:18:02.000000 followthemoney-3.5.0/followthemoney/schema/TaxRoll.yaml
+-rw-r--r--   0 runner    (1001) docker     (123)     2403 2023-07-21 12:18:02.000000 followthemoney-3.5.0/followthemoney/schema/Thing.yaml
+-rw-r--r--   0 runner    (1001) docker     (123)      771 2023-07-21 12:18:02.000000 followthemoney-3.5.0/followthemoney/schema/Trip.yaml
+-rw-r--r--   0 runner    (1001) docker     (123)      668 2023-07-21 12:18:02.000000 followthemoney-3.5.0/followthemoney/schema/UnknownLink.yaml
+-rw-r--r--   0 runner    (1001) docker     (123)      763 2023-07-21 12:18:02.000000 followthemoney-3.5.0/followthemoney/schema/UserAccount.yaml
+-rw-r--r--   0 runner    (1001) docker     (123)      310 2023-07-21 12:18:02.000000 followthemoney-3.5.0/followthemoney/schema/Value.yaml
+-rw-r--r--   0 runner    (1001) docker     (123)      984 2023-07-21 12:18:02.000000 followthemoney-3.5.0/followthemoney/schema/Vehicle.yaml
+-rw-r--r--   0 runner    (1001) docker     (123)      993 2023-07-21 12:18:02.000000 followthemoney-3.5.0/followthemoney/schema/Vessel.yaml
+-rw-r--r--   0 runner    (1001) docker     (123)      321 2023-07-21 12:18:02.000000 followthemoney-3.5.0/followthemoney/schema/Video.yaml
+-rw-r--r--   0 runner    (1001) docker     (123)      348 2023-07-21 12:18:02.000000 followthemoney-3.5.0/followthemoney/schema/Workbook.yaml
+-rw-r--r--   0 runner    (1001) docker     (123)    16736 2023-07-21 12:18:02.000000 followthemoney-3.5.0/followthemoney/schema.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-21 12:19:59.123589 followthemoney-3.5.0/followthemoney/translations/
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-21 12:19:59.107588 followthemoney-3.5.0/followthemoney/translations/ar/
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-21 12:19:59.123589 followthemoney-3.5.0/followthemoney/translations/ar/LC_MESSAGES/
+-rw-r--r--   0 runner    (1001) docker     (123)    38829 2023-07-21 12:18:02.000000 followthemoney-3.5.0/followthemoney/translations/ar/LC_MESSAGES/followthemoney.mo
+-rw-r--r--   0 runner    (1001) docker     (123)   118608 2023-07-21 12:18:02.000000 followthemoney-3.5.0/followthemoney/translations/ar/LC_MESSAGES/followthemoney.po
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-21 12:19:59.107588 followthemoney-3.5.0/followthemoney/translations/bs/
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-21 12:19:59.123589 followthemoney-3.5.0/followthemoney/translations/bs/LC_MESSAGES/
+-rw-r--r--   0 runner    (1001) docker     (123)    10751 2023-07-21 12:18:02.000000 followthemoney-3.5.0/followthemoney/translations/bs/LC_MESSAGES/followthemoney.mo
+-rw-r--r--   0 runner    (1001) docker     (123)    93147 2023-07-21 12:18:02.000000 followthemoney-3.5.0/followthemoney/translations/bs/LC_MESSAGES/followthemoney.po
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-21 12:19:59.107588 followthemoney-3.5.0/followthemoney/translations/de/
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-21 12:19:59.123589 followthemoney-3.5.0/followthemoney/translations/de/LC_MESSAGES/
+-rw-r--r--   0 runner    (1001) docker     (123)    36107 2023-07-21 12:18:02.000000 followthemoney-3.5.0/followthemoney/translations/de/LC_MESSAGES/followthemoney.mo
+-rw-r--r--   0 runner    (1001) docker     (123)   112813 2023-07-21 12:18:02.000000 followthemoney-3.5.0/followthemoney/translations/de/LC_MESSAGES/followthemoney.po
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-21 12:19:59.107588 followthemoney-3.5.0/followthemoney/translations/es/
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-21 12:19:59.123589 followthemoney-3.5.0/followthemoney/translations/es/LC_MESSAGES/
+-rw-r--r--   0 runner    (1001) docker     (123)    32176 2023-07-21 12:18:02.000000 followthemoney-3.5.0/followthemoney/translations/es/LC_MESSAGES/followthemoney.mo
+-rw-r--r--   0 runner    (1001) docker     (123)   112460 2023-07-21 12:18:02.000000 followthemoney-3.5.0/followthemoney/translations/es/LC_MESSAGES/followthemoney.po
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-21 12:19:59.123589 followthemoney-3.5.0/followthemoney/translations/fr/
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-21 12:19:59.123589 followthemoney-3.5.0/followthemoney/translations/fr/LC_MESSAGES/
+-rw-r--r--   0 runner    (1001) docker     (123)    42553 2023-07-21 12:18:02.000000 followthemoney-3.5.0/followthemoney/translations/fr/LC_MESSAGES/followthemoney.mo
+-rw-r--r--   0 runner    (1001) docker     (123)   117244 2023-07-21 12:18:02.000000 followthemoney-3.5.0/followthemoney/translations/fr/LC_MESSAGES/followthemoney.po
+-rw-r--r--   0 runner    (1001) docker     (123)   106802 2023-07-21 12:18:02.000000 followthemoney-3.5.0/followthemoney/translations/fr/followthemoney.po
+-rw-r--r--   0 runner    (1001) docker     (123)   101212 2023-07-21 12:18:02.000000 followthemoney-3.5.0/followthemoney/translations/messages.pot
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-21 12:19:59.107588 followthemoney-3.5.0/followthemoney/translations/nb/
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-21 12:19:59.127589 followthemoney-3.5.0/followthemoney/translations/nb/LC_MESSAGES/
+-rw-r--r--   0 runner    (1001) docker     (123)      498 2023-07-21 12:18:02.000000 followthemoney-3.5.0/followthemoney/translations/nb/LC_MESSAGES/followthemoney.mo
+-rw-r--r--   0 runner    (1001) docker     (123)    89796 2023-07-21 12:18:02.000000 followthemoney-3.5.0/followthemoney/translations/nb/LC_MESSAGES/followthemoney.po
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-21 12:19:59.107588 followthemoney-3.5.0/followthemoney/translations/nl/
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-21 12:19:59.127589 followthemoney-3.5.0/followthemoney/translations/nl/LC_MESSAGES/
+-rw-r--r--   0 runner    (1001) docker     (123)      486 2023-07-21 12:18:02.000000 followthemoney-3.5.0/followthemoney/translations/nl/LC_MESSAGES/followthemoney.mo
+-rw-r--r--   0 runner    (1001) docker     (123)    90876 2023-07-21 12:18:02.000000 followthemoney-3.5.0/followthemoney/translations/nl/LC_MESSAGES/followthemoney.po
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-21 12:19:59.107588 followthemoney-3.5.0/followthemoney/translations/pt_BR/
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-21 12:19:59.127589 followthemoney-3.5.0/followthemoney/translations/pt_BR/LC_MESSAGES/
+-rw-r--r--   0 runner    (1001) docker     (123)      505 2023-07-21 12:18:02.000000 followthemoney-3.5.0/followthemoney/translations/pt_BR/LC_MESSAGES/followthemoney.mo
+-rw-r--r--   0 runner    (1001) docker     (123)    89847 2023-07-21 12:18:02.000000 followthemoney-3.5.0/followthemoney/translations/pt_BR/LC_MESSAGES/followthemoney.po
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-21 12:19:59.127589 followthemoney-3.5.0/followthemoney/translations/ru/
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-21 12:19:59.127589 followthemoney-3.5.0/followthemoney/translations/ru/LC_MESSAGES/
+-rw-r--r--   0 runner    (1001) docker     (123)    61971 2023-07-21 12:18:02.000000 followthemoney-3.5.0/followthemoney/translations/ru/LC_MESSAGES/followthemoney.mo
+-rw-r--r--   0 runner    (1001) docker     (123)   133236 2023-07-21 12:18:02.000000 followthemoney-3.5.0/followthemoney/translations/ru/LC_MESSAGES/followthemoney.po
+-rw-r--r--   0 runner    (1001) docker     (123)   130621 2023-07-21 12:18:02.000000 followthemoney-3.5.0/followthemoney/translations/ru/followthemoney.po
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-21 12:19:59.111589 followthemoney-3.5.0/followthemoney/translations/tr/
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-21 12:19:59.127589 followthemoney-3.5.0/followthemoney/translations/tr/LC_MESSAGES/
+-rw-r--r--   0 runner    (1001) docker     (123)      487 2023-07-21 12:18:02.000000 followthemoney-3.5.0/followthemoney/translations/tr/LC_MESSAGES/followthemoney.mo
+-rw-r--r--   0 runner    (1001) docker     (123)    89829 2023-07-21 12:18:02.000000 followthemoney-3.5.0/followthemoney/translations/tr/LC_MESSAGES/followthemoney.po
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-21 12:19:59.131589 followthemoney-3.5.0/followthemoney/types/
+-rw-r--r--   0 runner    (1001) docker     (123)     1690 2023-07-21 12:18:02.000000 followthemoney-3.5.0/followthemoney/types/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1651 2023-07-21 12:18:02.000000 followthemoney-3.5.0/followthemoney/types/address.py
+-rw-r--r--   0 runner    (1001) docker     (123)      917 2023-07-21 12:18:02.000000 followthemoney-3.5.0/followthemoney/types/checksum.py
+-rw-r--r--   0 runner    (1001) docker     (123)     9560 2023-07-21 12:18:02.000000 followthemoney-3.5.0/followthemoney/types/common.py
+-rw-r--r--   0 runner    (1001) docker     (123)     3053 2023-07-21 12:18:02.000000 followthemoney-3.5.0/followthemoney/types/country.py
+-rw-r--r--   0 runner    (1001) docker     (123)     2500 2023-07-21 12:18:02.000000 followthemoney-3.5.0/followthemoney/types/date.py
+-rw-r--r--   0 runner    (1001) docker     (123)     2680 2023-07-21 12:18:02.000000 followthemoney-3.5.0/followthemoney/types/email.py
+-rw-r--r--   0 runner    (1001) docker     (123)     2366 2023-07-21 12:18:02.000000 followthemoney-3.5.0/followthemoney/types/entity.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1800 2023-07-21 12:18:02.000000 followthemoney-3.5.0/followthemoney/types/gender.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1848 2023-07-21 12:18:02.000000 followthemoney-3.5.0/followthemoney/types/iban.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1510 2023-07-21 12:18:02.000000 followthemoney-3.5.0/followthemoney/types/identifier.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1327 2023-07-21 12:18:02.000000 followthemoney-3.5.0/followthemoney/types/ip.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1676 2023-07-21 12:18:02.000000 followthemoney-3.5.0/followthemoney/types/json.py
+-rw-r--r--   0 runner    (1001) docker     (123)     2613 2023-07-21 12:18:02.000000 followthemoney-3.5.0/followthemoney/types/language.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1351 2023-07-21 12:18:02.000000 followthemoney-3.5.0/followthemoney/types/mimetype.py
+-rw-r--r--   0 runner    (1001) docker     (123)     2855 2023-07-21 12:18:02.000000 followthemoney-3.5.0/followthemoney/types/name.py
+-rw-r--r--   0 runner    (1001) docker     (123)      943 2023-07-21 12:18:02.000000 followthemoney-3.5.0/followthemoney/types/number.py
+-rw-r--r--   0 runner    (1001) docker     (123)     3955 2023-07-21 12:18:02.000000 followthemoney-3.5.0/followthemoney/types/phone.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1936 2023-07-21 12:18:02.000000 followthemoney-3.5.0/followthemoney/types/registry.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1130 2023-07-21 12:18:02.000000 followthemoney-3.5.0/followthemoney/types/string.py
+-rw-r--r--   0 runner    (1001) docker     (123)     2844 2023-07-21 12:18:02.000000 followthemoney-3.5.0/followthemoney/types/topic.py
+-rw-r--r--   0 runner    (1001) docker     (123)     2162 2023-07-21 12:18:02.000000 followthemoney-3.5.0/followthemoney/types/url.py
+-rw-r--r--   0 runner    (1001) docker     (123)     4508 2023-07-21 12:18:02.000000 followthemoney-3.5.0/followthemoney/util.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-21 12:19:59.111589 followthemoney-3.5.0/followthemoney.egg-info/
+-rw-r--r--   0 runner    (1001) docker     (123)     3598 2023-07-21 12:19:59.000000 followthemoney-3.5.0/followthemoney.egg-info/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (123)     6000 2023-07-21 12:19:59.000000 followthemoney-3.5.0/followthemoney.egg-info/SOURCES.txt
+-rw-r--r--   0 runner    (1001) docker     (123)        1 2023-07-21 12:19:59.000000 followthemoney-3.5.0/followthemoney.egg-info/dependency_links.txt
+-rw-r--r--   0 runner    (1001) docker     (123)      594 2023-07-21 12:19:59.000000 followthemoney-3.5.0/followthemoney.egg-info/entry_points.txt
+-rw-r--r--   0 runner    (1001) docker     (123)        1 2023-07-21 12:19:59.000000 followthemoney-3.5.0/followthemoney.egg-info/namespace_packages.txt
+-rw-r--r--   0 runner    (1001) docker     (123)        1 2023-07-21 12:19:38.000000 followthemoney-3.5.0/followthemoney.egg-info/not-zip-safe
+-rw-r--r--   0 runner    (1001) docker     (123)      725 2023-07-21 12:19:59.000000 followthemoney-3.5.0/followthemoney.egg-info/requires.txt
+-rw-r--r--   0 runner    (1001) docker     (123)       21 2023-07-21 12:19:59.000000 followthemoney-3.5.0/followthemoney.egg-info/top_level.txt
+-rw-r--r--   0 runner    (1001) docker     (123)      131 2023-07-21 12:19:59.131589 followthemoney-3.5.0/setup.cfg
+-rw-r--r--   0 runner    (1001) docker     (123)     3214 2023-07-21 12:18:02.000000 followthemoney-3.5.0/setup.py
```

### Comparing `followthemoney-3.4.4/LICENSE` & `followthemoney-3.5.0/LICENSE`

 * *Files identical despite different names*

### Comparing `followthemoney-3.4.4/PKG-INFO` & `followthemoney-3.5.0/README.md`

 * *Files 9% similar despite different names*

```diff
@@ -1,22 +1,7 @@
-Metadata-Version: 2.1
-Name: followthemoney
-Version: 3.4.4
-Home-page: https://followthemoney.tech/
-Author: Organized Crime and Corruption Reporting Project
-Author-email: data@occrp.org
-License: MIT
-Classifier: Intended Audience :: Developers
-Classifier: Operating System :: OS Independent
-Classifier: Programming Language :: Python
-Classifier: Programming Language :: Python :: 3.9
-Description-Content-Type: text/markdown
-Provides-Extra: dev
-License-File: LICENSE
-
 # Follow the Money
 
 [![ftm-build](https://github.com/alephdata/followthemoney/actions/workflows/build.yml/badge.svg)](https://github.com/alephdata/followthemoney/actions/workflows/build.yml)
 
 This repository contains a pragmatic data model for the entities most
 commonly used in investigative reporting: people, companies, assets,
 payments, court cases, etc.
```

### Comparing `followthemoney-3.4.4/followthemoney/cli/aggregate.py` & `followthemoney-3.5.0/followthemoney/cli/aggregate.py`

 * *Files identical despite different names*

### Comparing `followthemoney-3.4.4/followthemoney/cli/cli.py` & `followthemoney-3.5.0/followthemoney/cli/cli.py`

 * *Files identical despite different names*

### Comparing `followthemoney-3.4.4/followthemoney/cli/exports.py` & `followthemoney-3.5.0/followthemoney/cli/exports.py`

 * *Files identical despite different names*

### Comparing `followthemoney-3.4.4/followthemoney/cli/mapping.py` & `followthemoney-3.5.0/followthemoney/cli/mapping.py`

 * *Files identical despite different names*

### Comparing `followthemoney-3.4.4/followthemoney/cli/sieve.py` & `followthemoney-3.5.0/followthemoney/cli/sieve.py`

 * *Files identical despite different names*

### Comparing `followthemoney-3.4.4/followthemoney/cli/util.py` & `followthemoney-3.5.0/followthemoney/cli/util.py`

 * *Files identical despite different names*

### Comparing `followthemoney-3.4.4/followthemoney/compare.py` & `followthemoney-3.5.0/followthemoney/compare.py`

 * *Files identical despite different names*

### Comparing `followthemoney-3.4.4/followthemoney/exc.py` & `followthemoney-3.5.0/followthemoney/exc.py`

 * *Files identical despite different names*

### Comparing `followthemoney-3.4.4/followthemoney/export/common.py` & `followthemoney-3.5.0/followthemoney/export/common.py`

 * *Files identical despite different names*

### Comparing `followthemoney-3.4.4/followthemoney/export/csv.py` & `followthemoney-3.5.0/followthemoney/export/csv.py`

 * *Files identical despite different names*

### Comparing `followthemoney-3.4.4/followthemoney/export/excel.py` & `followthemoney-3.5.0/followthemoney/export/excel.py`

 * *Files identical despite different names*

### Comparing `followthemoney-3.4.4/followthemoney/export/graph.py` & `followthemoney-3.5.0/followthemoney/export/graph.py`

 * *Files identical despite different names*

### Comparing `followthemoney-3.4.4/followthemoney/export/neo4j.py` & `followthemoney-3.5.0/followthemoney/export/neo4j.py`

 * *Files identical despite different names*

### Comparing `followthemoney-3.4.4/followthemoney/export/rdf.py` & `followthemoney-3.5.0/followthemoney/export/rdf.py`

 * *Files identical despite different names*

### Comparing `followthemoney-3.4.4/followthemoney/graph.py` & `followthemoney-3.5.0/followthemoney/graph.py`

 * *Files identical despite different names*

### Comparing `followthemoney-3.4.4/followthemoney/helpers.py` & `followthemoney-3.5.0/followthemoney/helpers.py`

 * *Files identical despite different names*

### Comparing `followthemoney-3.4.4/followthemoney/mapping/csv.py` & `followthemoney-3.5.0/followthemoney/mapping/csv.py`

 * *Files identical despite different names*

### Comparing `followthemoney-3.4.4/followthemoney/mapping/entity.py` & `followthemoney-3.5.0/followthemoney/mapping/entity.py`

 * *Files 18% similar despite different names*

```diff
@@ -1,8 +1,9 @@
 from hashlib import sha1
+from warnings import warn
 from typing import TYPE_CHECKING, Any, Dict, List, Optional, Set
 from banal import keys_values
 from normality import stringify
 
 from followthemoney.types import registry
 from followthemoney.util import key_bytes
 from followthemoney.proxy import EntityProxy
@@ -53,14 +54,20 @@
 
         schema_name = stringify(data.get("schema"))
         if schema_name is None:
             raise InvalidMapping("No schema: %s" % name)
         schema = model.get(schema_name)
         if schema is None:
             raise InvalidMapping("Invalid schema: %s" % schema_name)
+        if schema.deprecated:
+            warn(
+                "Mapping uses a deprecated schema: %r" % schema,
+                DeprecationWarning,
+                stacklevel=2,
+            )
         self.schema = schema
 
         self.refs = set(self.keys)
         if self.id_column:
             self.refs.add(self.id_column)
         self.dependencies: Set[str] = set()
         self.properties: List[PropertyMapping] = []
```

### Comparing `followthemoney-3.4.4/followthemoney/mapping/property.py` & `followthemoney-3.5.0/followthemoney/mapping/property.py`

 * *Files 6% similar despite different names*

```diff
@@ -1,9 +1,10 @@
 import re
 from copy import deepcopy
+from warnings import warn
 from normality import stringify
 from typing import TYPE_CHECKING, Any, Dict, List, Optional, cast
 from banal import keys_values, as_bool
 
 from followthemoney.helpers import inline_names
 from followthemoney.exc import InvalidMapping
 from followthemoney.proxy import EntityProxy
@@ -60,14 +61,21 @@
                 self.refs.append(ref)
                 self.replacements["{{%s}}" % ref] = ref
 
     def bind(self) -> None:
         if self.prop.stub:
             raise InvalidMapping("Property for [%r] is a stub" % self.prop)
 
+        if self.prop.deprecated:
+            warn(
+                "Mapping uses a deprecated property: %r" % self.prop,
+                DeprecationWarning,
+                stacklevel=2,
+            )
+
         if self.entity is None:
             return
 
         # Figure out if the schema types of the referenced entities
         # are of a type compatible with the range of this property.
         # For example, an asset can be owned by a legal entity, but
         # by a bank payment or a ship.
```

### Comparing `followthemoney-3.4.4/followthemoney/mapping/query.py` & `followthemoney-3.5.0/followthemoney/mapping/query.py`

 * *Files identical despite different names*

### Comparing `followthemoney-3.4.4/followthemoney/mapping/source.py` & `followthemoney-3.5.0/followthemoney/mapping/source.py`

 * *Files identical despite different names*

### Comparing `followthemoney-3.4.4/followthemoney/mapping/sql.py` & `followthemoney-3.5.0/followthemoney/mapping/sql.py`

 * *Files identical despite different names*

### Comparing `followthemoney-3.4.4/followthemoney/messages.py` & `followthemoney-3.5.0/followthemoney/messages.py`

 * *Files identical despite different names*

### Comparing `followthemoney-3.4.4/followthemoney/model.py` & `followthemoney-3.5.0/followthemoney/model.py`

 * *Files identical despite different names*

### Comparing `followthemoney-3.4.4/followthemoney/namespace.py` & `followthemoney-3.5.0/followthemoney/namespace.py`

 * *Files identical despite different names*

### Comparing `followthemoney-3.4.4/followthemoney/offshore.py` & `followthemoney-3.5.0/followthemoney/offshore.py`

 * *Files identical despite different names*

### Comparing `followthemoney-3.4.4/followthemoney/ontology.py` & `followthemoney-3.5.0/followthemoney/ontology.py`

 * *Files identical despite different names*

### Comparing `followthemoney-3.4.4/followthemoney/property.py` & `followthemoney-3.5.0/followthemoney/property.py`

 * *Files 2% similar despite different names*

```diff
@@ -19,14 +19,15 @@
 
 class PropertyDict(TypedDict, total=False):
     label: Optional[str]
     description: Optional[str]
     type: Optional[str]
     hidden: Optional[bool]
     matchable: Optional[bool]
+    deprecated: Optional[bool]
     # stub: Optional[bool]
     rdf: Optional[str]
     range: Optional[str]
 
 
 class PropertySpec(PropertyDict):
     reverse: ReverseSpec
@@ -51,14 +52,15 @@
         "qname",
         "_label",
         "_hash",
         "_description",
         "hidden",
         "type",
         "matchable",
+        "deprecated",
         "_range",
         "range",
         "stub",
         "_reverse",
         "reverse",
         "uri",
     )
@@ -81,16 +83,19 @@
             raise InvalidModel("Reserved name: %s" % self.name)
 
         self._hash = hash("<Property(%r)>" % self.qname)
 
         self._label = data.get("label", name)
         self._description = data.get("description")
 
+        #: This property is deprecated and should not be used.
+        self.deprecated = as_bool(data.get("deprecated", False))
+
         #: This property should not be shown or mentioned in the user interface.
-        self.hidden = as_bool(data.get("hidden", False))
+        self.hidden = as_bool(data.get("hidden"))
 
         type_ = data.get("type", "string")
         if type_ is None or type_ not in registry.named:
             raise InvalidModel("Invalid type: %s" % type_)
 
         #: The data type for this property.
         self.type = registry[type_]
@@ -188,14 +193,16 @@
             data["description"] = self.description
         if self.stub:
             data["stub"] = True
         if self.matchable:
             data["matchable"] = True
         if self.hidden:
             data["hidden"] = True
+        if self.deprecated:
+            data["deprecated"] = True
         if self.range is not None:
             data["range"] = self.range.name
         if self.reverse is not None:
             data["reverse"] = self.reverse.name
         return data
 
     def __repr__(self) -> str:
```

### Comparing `followthemoney-3.4.4/followthemoney/proxy.py` & `followthemoney-3.5.0/followthemoney/proxy.py`

 * *Files identical despite different names*

### Comparing `followthemoney-3.4.4/followthemoney/schema/Address.yaml` & `followthemoney-3.5.0/followthemoney/schema/Address.yaml`

 * *Files identical despite different names*

### Comparing `followthemoney-3.4.4/followthemoney/schema/Airplane.yaml` & `followthemoney-3.5.0/followthemoney/schema/Airplane.yaml`

 * *Files identical despite different names*

### Comparing `followthemoney-3.4.4/followthemoney/schema/Analyzable.yaml` & `followthemoney-3.5.0/followthemoney/schema/Analyzable.yaml`

 * *Files identical despite different names*

### Comparing `followthemoney-3.4.4/followthemoney/schema/Assessment.yaml` & `followthemoney-3.5.0/followthemoney/schema/Assessment.yaml`

 * *Files identical despite different names*

### Comparing `followthemoney-3.4.4/followthemoney/schema/Associate.yaml` & `followthemoney-3.5.0/followthemoney/schema/Associate.yaml`

 * *Files identical despite different names*

### Comparing `followthemoney-3.4.4/followthemoney/schema/BankAccount.yaml` & `followthemoney-3.5.0/followthemoney/schema/BankAccount.yaml`

 * *Files identical despite different names*

### Comparing `followthemoney-3.4.4/followthemoney/schema/Call.yaml` & `followthemoney-3.5.0/followthemoney/schema/Call.yaml`

 * *Files identical despite different names*

### Comparing `followthemoney-3.4.4/followthemoney/schema/CallForTenders.yaml` & `followthemoney-3.5.0/followthemoney/schema/CallForTenders.yaml`

 * *Files identical despite different names*

### Comparing `followthemoney-3.4.4/followthemoney/schema/Company.yaml` & `followthemoney-3.5.0/followthemoney/schema/Company.yaml`

 * *Files identical despite different names*

### Comparing `followthemoney-3.4.4/followthemoney/schema/Contract.yaml` & `followthemoney-3.5.0/followthemoney/schema/Contract.yaml`

 * *Files identical despite different names*

### Comparing `followthemoney-3.4.4/followthemoney/schema/ContractAward.yaml` & `followthemoney-3.5.0/followthemoney/schema/ContractAward.yaml`

 * *Files identical despite different names*

### Comparing `followthemoney-3.4.4/followthemoney/schema/CourtCase.yaml` & `followthemoney-3.5.0/followthemoney/schema/CourtCase.yaml`

 * *Files identical despite different names*

### Comparing `followthemoney-3.4.4/followthemoney/schema/CourtCaseParty.yaml` & `followthemoney-3.5.0/followthemoney/schema/CourtCaseParty.yaml`

 * *Files identical despite different names*

### Comparing `followthemoney-3.4.4/followthemoney/schema/CryptoWallet.yaml` & `followthemoney-3.5.0/followthemoney/schema/CryptoWallet.yaml`

 * *Files identical despite different names*

### Comparing `followthemoney-3.4.4/followthemoney/schema/Debt.yaml` & `followthemoney-3.5.0/followthemoney/schema/Debt.yaml`

 * *Files identical despite different names*

### Comparing `followthemoney-3.4.4/followthemoney/schema/Directorship.yaml` & `followthemoney-3.5.0/followthemoney/schema/Directorship.yaml`

 * *Files identical despite different names*

### Comparing `followthemoney-3.4.4/followthemoney/schema/Document.yaml` & `followthemoney-3.5.0/followthemoney/schema/Document.yaml`

 * *Files identical despite different names*

### Comparing `followthemoney-3.4.4/followthemoney/schema/Documentation.yml` & `followthemoney-3.5.0/followthemoney/schema/Documentation.yml`

 * *Files identical despite different names*

### Comparing `followthemoney-3.4.4/followthemoney/schema/EconomicActivity.yaml` & `followthemoney-3.5.0/followthemoney/schema/EconomicActivity.yaml`

 * *Files identical despite different names*

### Comparing `followthemoney-3.4.4/followthemoney/schema/Email.yaml` & `followthemoney-3.5.0/followthemoney/schema/Email.yaml`

 * *Files identical despite different names*

### Comparing `followthemoney-3.4.4/followthemoney/schema/Employment.yaml` & `followthemoney-3.5.0/followthemoney/schema/Employment.yaml`

 * *Files identical despite different names*

### Comparing `followthemoney-3.4.4/followthemoney/schema/Event.yaml` & `followthemoney-3.5.0/followthemoney/schema/Event.yaml`

 * *Files identical despite different names*

### Comparing `followthemoney-3.4.4/followthemoney/schema/Family.yaml` & `followthemoney-3.5.0/followthemoney/schema/Family.yaml`

 * *Files identical despite different names*

### Comparing `followthemoney-3.4.4/followthemoney/schema/Identification.yaml` & `followthemoney-3.5.0/followthemoney/schema/Identification.yaml`

 * *Files identical despite different names*

### Comparing `followthemoney-3.4.4/followthemoney/schema/Interval.yaml` & `followthemoney-3.5.0/followthemoney/schema/Interval.yaml`

 * *Files identical despite different names*

### Comparing `followthemoney-3.4.4/followthemoney/schema/LegalEntity.yaml` & `followthemoney-3.5.0/followthemoney/schema/LegalEntity.yaml`

 * *Files identical despite different names*

### Comparing `followthemoney-3.4.4/followthemoney/schema/Membership.yaml` & `followthemoney-3.5.0/followthemoney/schema/Membership.yaml`

 * *Files identical despite different names*

### Comparing `followthemoney-3.4.4/followthemoney/schema/Mention.yaml` & `followthemoney-3.5.0/followthemoney/schema/Mention.yaml`

 * *Files identical despite different names*

### Comparing `followthemoney-3.4.4/followthemoney/schema/Message.yaml` & `followthemoney-3.5.0/followthemoney/schema/Message.yaml`

 * *Files identical despite different names*

### Comparing `followthemoney-3.4.4/followthemoney/schema/Ownership.yaml` & `followthemoney-3.5.0/followthemoney/schema/Ownership.yaml`

 * *Files identical despite different names*

### Comparing `followthemoney-3.4.4/followthemoney/schema/Page.yaml` & `followthemoney-3.5.0/followthemoney/schema/Page.yaml`

 * *Files identical despite different names*

### Comparing `followthemoney-3.4.4/followthemoney/schema/Passport.yaml` & `followthemoney-3.5.0/followthemoney/schema/Passport.yaml`

 * *Files identical despite different names*

### Comparing `followthemoney-3.4.4/followthemoney/schema/Payment.yaml` & `followthemoney-3.5.0/followthemoney/schema/Payment.yaml`

 * *Files identical despite different names*

### Comparing `followthemoney-3.4.4/followthemoney/schema/Person.yaml` & `followthemoney-3.5.0/followthemoney/schema/Person.yaml`

 * *Files identical despite different names*

### Comparing `followthemoney-3.4.4/followthemoney/schema/Post.yaml` & `followthemoney-3.5.0/followthemoney/schema/Post.yaml`

 * *Files 7% similar despite different names*

```diff
@@ -1,12 +1,13 @@
 Post:
   label: "Post"
   plural: "Posts"
   extends: Interest
   matchable: false
+  deprecated: true
   # cf. https://www.popoloproject.com/specs/post.html
   # But they're using it to define the post as an abstract thing, this
   # describes the interval in which it is held by an individual.
   description: >
     A post, role or position held by an individual within an organization 
     or body. This describes the period for which the position is held,
     not the abstract concept of the post.
```

### Comparing `followthemoney-3.4.4/followthemoney/schema/ProjectParticipant.yaml` & `followthemoney-3.5.0/followthemoney/schema/ProjectParticipant.yaml`

 * *Files identical despite different names*

### Comparing `followthemoney-3.4.4/followthemoney/schema/RealEstate.yaml` & `followthemoney-3.5.0/followthemoney/schema/RealEstate.yaml`

 * *Files identical despite different names*

### Comparing `followthemoney-3.4.4/followthemoney/schema/Representation.yaml` & `followthemoney-3.5.0/followthemoney/schema/Representation.yaml`

 * *Files identical despite different names*

### Comparing `followthemoney-3.4.4/followthemoney/schema/Sanction.yaml` & `followthemoney-3.5.0/followthemoney/schema/Sanction.yaml`

 * *Files identical despite different names*

### Comparing `followthemoney-3.4.4/followthemoney/schema/Security.yaml` & `followthemoney-3.5.0/followthemoney/schema/Security.yaml`

 * *Files identical despite different names*

### Comparing `followthemoney-3.4.4/followthemoney/schema/Similar.yaml` & `followthemoney-3.5.0/followthemoney/schema/Similar.yaml`

 * *Files identical despite different names*

### Comparing `followthemoney-3.4.4/followthemoney/schema/Succession.yaml` & `followthemoney-3.5.0/followthemoney/schema/Succession.yaml`

 * *Files identical despite different names*

### Comparing `followthemoney-3.4.4/followthemoney/schema/Table.yaml` & `followthemoney-3.5.0/followthemoney/schema/Table.yaml`

 * *Files identical despite different names*

### Comparing `followthemoney-3.4.4/followthemoney/schema/TaxRoll.yaml` & `followthemoney-3.5.0/followthemoney/schema/TaxRoll.yaml`

 * *Files identical despite different names*

### Comparing `followthemoney-3.4.4/followthemoney/schema/Thing.yaml` & `followthemoney-3.5.0/followthemoney/schema/Thing.yaml`

 * *Files identical despite different names*

### Comparing `followthemoney-3.4.4/followthemoney/schema/Trip.yaml` & `followthemoney-3.5.0/followthemoney/schema/Trip.yaml`

 * *Files identical despite different names*

### Comparing `followthemoney-3.4.4/followthemoney/schema/UnknownLink.yaml` & `followthemoney-3.5.0/followthemoney/schema/UnknownLink.yaml`

 * *Files identical despite different names*

### Comparing `followthemoney-3.4.4/followthemoney/schema/UserAccount.yaml` & `followthemoney-3.5.0/followthemoney/schema/UserAccount.yaml`

 * *Files identical despite different names*

### Comparing `followthemoney-3.4.4/followthemoney/schema/Vehicle.yaml` & `followthemoney-3.5.0/followthemoney/schema/Vehicle.yaml`

 * *Files identical despite different names*

### Comparing `followthemoney-3.4.4/followthemoney/schema/Vessel.yaml` & `followthemoney-3.5.0/followthemoney/schema/Vessel.yaml`

 * *Files identical despite different names*

### Comparing `followthemoney-3.4.4/followthemoney/schema.py` & `followthemoney-3.5.0/followthemoney/schema.py`

 * *Files 2% similar despite different names*

```diff
@@ -48,14 +48,15 @@
     temporalExtent: TemporalExtentSpec
     description: Optional[str]
     rdf: Optional[str]
     abstract: bool
     hidden: bool
     generated: bool
     matchable: bool
+    deprecated: Optional[bool]
 
 
 class SchemaToDict(TypedDict, total=False):
     label: str
     plural: str
     schemata: List[str]
     extends: List[str]
@@ -66,14 +67,15 @@
     edge: EdgeSpec
     temporalExtent: TemporalExtentSpec
     description: Optional[str]
     abstract: bool
     hidden: bool
     generated: bool
     matchable: bool
+    deprecated: bool
 
 
 class Schema:
     """A type definition for a class of entities that have certain properties.
 
     Schemata are arranged in a multi-rooted hierarchy: each schema can have multiple
     parent schemata from which it inherits all of their properties. A schema can also
@@ -91,14 +93,15 @@
         "uri",
         "abstract",
         "hidden",
         "generated",
         "matchable",
         "featured",
         "required",
+        "deprecated",
         "caption",
         "edge",
         "_edge_label",
         "edge_directed",
         "edge_source",
         "edge_target",
         "edge_caption",
@@ -125,14 +128,17 @@
         #: RDF identifier for this schema when it is transformed to a triple term.
         self.uri = URIRef(cast(str, data.get("rdf", NS[name])))
 
         #: Do not store or emit entities of this type, it is used only for
         #: inheritance.
         self.abstract = as_bool(data.get("abstract"), False)
 
+        #: This schema is deprecated and should not be used.
+        self.deprecated = as_bool(data.get("deprecated", False))
+
         #: Hide this schema in listings.
         self.hidden = as_bool(data.get("hidden"), False)
         self.hidden = self.hidden and not self.abstract
 
         #: Entities with this type are generated by the system - for example, via
         #: `ingest-file`. The user should not be offered an option to create them
         #: in the interface.
@@ -421,14 +427,16 @@
             data["abstract"] = True
         if self.hidden:
             data["hidden"] = True
         if self.generated:
             data["generated"] = True
         if self.matchable:
             data["matchable"] = True
+        if self.deprecated:
+            data["deprecated"] = True
         properties: Dict[str, PropertyToDict] = {}
         for name, prop in self.properties.items():
             if prop.schema == self:
                 properties[name] = prop.to_dict()
         data["properties"] = properties
         return data
```

### Comparing `followthemoney-3.4.4/followthemoney/translations/ar/LC_MESSAGES/followthemoney.mo` & `followthemoney-3.5.0/followthemoney/translations/ar/LC_MESSAGES/followthemoney.mo`

 * *Files identical despite different names*

### Comparing `followthemoney-3.4.4/followthemoney/translations/ar/LC_MESSAGES/followthemoney.po` & `followthemoney-3.5.0/followthemoney/translations/ar/LC_MESSAGES/followthemoney.po`

 * *Files identical despite different names*

### Comparing `followthemoney-3.4.4/followthemoney/translations/bs/LC_MESSAGES/followthemoney.mo` & `followthemoney-3.5.0/followthemoney/translations/bs/LC_MESSAGES/followthemoney.mo`

 * *Files identical despite different names*

### Comparing `followthemoney-3.4.4/followthemoney/translations/bs/LC_MESSAGES/followthemoney.po` & `followthemoney-3.5.0/followthemoney/translations/bs/LC_MESSAGES/followthemoney.po`

 * *Files identical despite different names*

### Comparing `followthemoney-3.4.4/followthemoney/translations/de/LC_MESSAGES/followthemoney.mo` & `followthemoney-3.5.0/followthemoney/translations/de/LC_MESSAGES/followthemoney.mo`

 * *Files identical despite different names*

### Comparing `followthemoney-3.4.4/followthemoney/translations/de/LC_MESSAGES/followthemoney.po` & `followthemoney-3.5.0/followthemoney/translations/de/LC_MESSAGES/followthemoney.po`

 * *Files identical despite different names*

### Comparing `followthemoney-3.4.4/followthemoney/translations/es/LC_MESSAGES/followthemoney.mo` & `followthemoney-3.5.0/followthemoney/translations/es/LC_MESSAGES/followthemoney.mo`

 * *Files identical despite different names*

### Comparing `followthemoney-3.4.4/followthemoney/translations/es/LC_MESSAGES/followthemoney.po` & `followthemoney-3.5.0/followthemoney/translations/es/LC_MESSAGES/followthemoney.po`

 * *Files identical despite different names*

### Comparing `followthemoney-3.4.4/followthemoney/translations/fr/LC_MESSAGES/followthemoney.mo` & `followthemoney-3.5.0/followthemoney/translations/fr/LC_MESSAGES/followthemoney.mo`

 * *Files identical despite different names*

### Comparing `followthemoney-3.4.4/followthemoney/translations/fr/LC_MESSAGES/followthemoney.po` & `followthemoney-3.5.0/followthemoney/translations/fr/LC_MESSAGES/followthemoney.po`

 * *Files identical despite different names*

### Comparing `followthemoney-3.4.4/followthemoney/translations/fr/followthemoney.po` & `followthemoney-3.5.0/followthemoney/translations/fr/followthemoney.po`

 * *Files identical despite different names*

### Comparing `followthemoney-3.4.4/followthemoney/translations/messages.pot` & `followthemoney-3.5.0/followthemoney/translations/messages.pot`

 * *Files identical despite different names*

### Comparing `followthemoney-3.4.4/followthemoney/translations/nb/LC_MESSAGES/followthemoney.po` & `followthemoney-3.5.0/followthemoney/translations/nb/LC_MESSAGES/followthemoney.po`

 * *Files identical despite different names*

### Comparing `followthemoney-3.4.4/followthemoney/translations/nl/LC_MESSAGES/followthemoney.po` & `followthemoney-3.5.0/followthemoney/translations/nl/LC_MESSAGES/followthemoney.po`

 * *Files identical despite different names*

### Comparing `followthemoney-3.4.4/followthemoney/translations/pt_BR/LC_MESSAGES/followthemoney.po` & `followthemoney-3.5.0/followthemoney/translations/pt_BR/LC_MESSAGES/followthemoney.po`

 * *Files identical despite different names*

### Comparing `followthemoney-3.4.4/followthemoney/translations/ru/LC_MESSAGES/followthemoney.mo` & `followthemoney-3.5.0/followthemoney/translations/ru/LC_MESSAGES/followthemoney.mo`

 * *Files identical despite different names*

### Comparing `followthemoney-3.4.4/followthemoney/translations/ru/LC_MESSAGES/followthemoney.po` & `followthemoney-3.5.0/followthemoney/translations/ru/LC_MESSAGES/followthemoney.po`

 * *Files 0% similar despite different names*

```diff
@@ -8,15 +8,15 @@
 # jen occrp, 2023
 # 
 #, fuzzy
 msgid ""
 msgstr ""
 "Project-Id-Version: PROJECT VERSION\n"
 "Report-Msgid-Bugs-To: EMAIL@ADDRESS\n"
-"POT-Creation-Date: 2023-06-27 15:36+0200\n"
+"POT-Creation-Date: 2023-07-12 18:31+0200\n"
 "PO-Revision-Date: 2022-11-21 11:38+0000\n"
 "Last-Translator: jen occrp, 2023\n"
 "Language-Team: Russian (https://app.transifex.com/aleph/teams/76591/ru/)\n"
 "MIME-Version: 1.0\n"
 "Content-Type: text/plain; charset=UTF-8\n"
 "Content-Transfer-Encoding: 8bit\n"
 "Generated-By: Babel 2.12.1\n"
@@ -31,20 +31,20 @@
 msgid "Invalid value"
 msgstr "Недопустимое значение"
 
 #: followthemoney/proxy.py:62
 msgid "No schema for entity."
 msgstr "Для сущности отсутствует схема."
 
-#: followthemoney/proxy.py:115
+#: followthemoney/proxy.py:119
 #, python-format
 msgid "Unknown property (%s): %s"
 msgstr "Неизвестный параметр (1%s): 1%s"
 
-#: followthemoney/proxy.py:188
+#: followthemoney/proxy.py:191
 #, python-format
 msgid "Stub property (%s): %s"
 msgstr "Неизвестное свойство (1%s): 1%s"
 
 #: followthemoney/schema.py:377
 msgid "Required"
 msgstr "Обязательное значение"
@@ -3037,14 +3037,24 @@
 msgstr "Матроним"
 
 #. Person.properties.lastName.label
 #: followthemoney/schema/Person.yaml
 msgid "Last name"
 msgstr "Фамилия"
 
+#. Person.properties.nameSuffix.label
+#: followthemoney/schema/Person.yaml
+msgid "Name suffix"
+msgstr "Фамильное окончание"
+
+#. Person.properties.birthCountry.label
+#: followthemoney/schema/Person.yaml
+msgid "Country of birth"
+msgstr "Страна рождения"
+
 #. Person.properties.deathDate.label
 #: followthemoney/schema/Person.yaml
 msgid "Death date"
 msgstr "Дата смерти"
 
 #. Person.properties.position.label
 #: followthemoney/schema/Person.yaml
```

### Comparing `followthemoney-3.4.4/followthemoney/translations/ru/followthemoney.po` & `followthemoney-3.5.0/followthemoney/translations/ru/followthemoney.po`

 * *Files identical despite different names*

### Comparing `followthemoney-3.4.4/followthemoney/translations/tr/LC_MESSAGES/followthemoney.po` & `followthemoney-3.5.0/followthemoney/translations/tr/LC_MESSAGES/followthemoney.po`

 * *Files identical despite different names*

### Comparing `followthemoney-3.4.4/followthemoney/types/__init__.py` & `followthemoney-3.5.0/followthemoney/types/__init__.py`

 * *Files identical despite different names*

### Comparing `followthemoney-3.4.4/followthemoney/types/address.py` & `followthemoney-3.5.0/followthemoney/types/address.py`

 * *Files identical despite different names*

### Comparing `followthemoney-3.4.4/followthemoney/types/checksum.py` & `followthemoney-3.5.0/followthemoney/types/checksum.py`

 * *Files identical despite different names*

### Comparing `followthemoney-3.4.4/followthemoney/types/common.py` & `followthemoney-3.5.0/followthemoney/types/common.py`

 * *Files identical despite different names*

### Comparing `followthemoney-3.4.4/followthemoney/types/country.py` & `followthemoney-3.5.0/followthemoney/types/country.py`

 * *Files identical despite different names*

### Comparing `followthemoney-3.4.4/followthemoney/types/date.py` & `followthemoney-3.5.0/followthemoney/types/date.py`

 * *Files identical despite different names*

### Comparing `followthemoney-3.4.4/followthemoney/types/email.py` & `followthemoney-3.5.0/followthemoney/types/email.py`

 * *Files identical despite different names*

### Comparing `followthemoney-3.4.4/followthemoney/types/entity.py` & `followthemoney-3.5.0/followthemoney/types/entity.py`

 * *Files identical despite different names*

### Comparing `followthemoney-3.4.4/followthemoney/types/gender.py` & `followthemoney-3.5.0/followthemoney/types/gender.py`

 * *Files identical despite different names*

### Comparing `followthemoney-3.4.4/followthemoney/types/iban.py` & `followthemoney-3.5.0/followthemoney/types/iban.py`

 * *Files identical despite different names*

### Comparing `followthemoney-3.4.4/followthemoney/types/identifier.py` & `followthemoney-3.5.0/followthemoney/types/identifier.py`

 * *Files identical despite different names*

### Comparing `followthemoney-3.4.4/followthemoney/types/ip.py` & `followthemoney-3.5.0/followthemoney/types/ip.py`

 * *Files identical despite different names*

### Comparing `followthemoney-3.4.4/followthemoney/types/json.py` & `followthemoney-3.5.0/followthemoney/types/json.py`

 * *Files identical despite different names*

### Comparing `followthemoney-3.4.4/followthemoney/types/language.py` & `followthemoney-3.5.0/followthemoney/types/language.py`

 * *Files identical despite different names*

### Comparing `followthemoney-3.4.4/followthemoney/types/mimetype.py` & `followthemoney-3.5.0/followthemoney/types/mimetype.py`

 * *Files identical despite different names*

### Comparing `followthemoney-3.4.4/followthemoney/types/name.py` & `followthemoney-3.5.0/followthemoney/types/name.py`

 * *Files identical despite different names*

### Comparing `followthemoney-3.4.4/followthemoney/types/number.py` & `followthemoney-3.5.0/followthemoney/types/number.py`

 * *Files identical despite different names*

### Comparing `followthemoney-3.4.4/followthemoney/types/phone.py` & `followthemoney-3.5.0/followthemoney/types/phone.py`

 * *Files identical despite different names*

### Comparing `followthemoney-3.4.4/followthemoney/types/registry.py` & `followthemoney-3.5.0/followthemoney/types/registry.py`

 * *Files identical despite different names*

### Comparing `followthemoney-3.4.4/followthemoney/types/string.py` & `followthemoney-3.5.0/followthemoney/types/string.py`

 * *Files identical despite different names*

### Comparing `followthemoney-3.4.4/followthemoney/types/topic.py` & `followthemoney-3.5.0/followthemoney/types/topic.py`

 * *Files identical despite different names*

### Comparing `followthemoney-3.4.4/followthemoney/types/url.py` & `followthemoney-3.5.0/followthemoney/types/url.py`

 * *Files identical despite different names*

### Comparing `followthemoney-3.4.4/followthemoney/util.py` & `followthemoney-3.5.0/followthemoney/util.py`

 * *Files identical despite different names*

### Comparing `followthemoney-3.4.4/followthemoney.egg-info/PKG-INFO` & `followthemoney-3.5.0/PKG-INFO`

 * *Files 25% similar despite different names*

```diff
@@ -1,90 +1,91 @@
 Metadata-Version: 2.1
 Name: followthemoney
-Version: 3.4.4
+Version: 3.5.0
+Summary: UNKNOWN
 Home-page: https://followthemoney.tech/
 Author: Organized Crime and Corruption Reporting Project
 Author-email: data@occrp.org
 License: MIT
+Description: # Follow the Money
+        
+        [![ftm-build](https://github.com/alephdata/followthemoney/actions/workflows/build.yml/badge.svg)](https://github.com/alephdata/followthemoney/actions/workflows/build.yml)
+        
+        This repository contains a pragmatic data model for the entities most
+        commonly used in investigative reporting: people, companies, assets,
+        payments, court cases, etc.
+        
+        The purpose of this is not to model reality in an ideal data model, but
+        rather to have a working data structure for researchers.
+        
+        `followthemoney` also contains code used to validate and normalize many
+        of the elements of data, and to map tabular data into the model.
+        
+        ## Documentation
+        
+        For a general introduction to `followthemoney`, check the high-level introduction:
+        
+        * https://followthemoney.tech
+        
+        Part of this package is a command-line tool that can be used to process and
+        transform data in various ways. You can find a tutorial here:
+        
+        * https://followthemoney.tech/docs/cli/
+        
+        Besides the introductions, there is also a full reference documentation for the
+        library and the contained ontology: 
+        
+        * https://followthemoney.tech/explorer/
+        
+        There's also a number of viewers for the RDF schema definitions generated
+        from FollowTheMoney, e.g.:
+        
+        * [LODE documentation](http://150.146.207.114/lode/extract?url=https%3A%2F%2Falephdata.github.io%2Ffollowthemoney%2Fns%2Fftm.xml&owlapi=true&imported=true&lang=en)
+        * [WebVOWL](https://service.tib.eu/webvowl/#iri=https://alephdata.github.io/followthemoney/ns/ftm.xml)
+        * RDF/OWL specification in [XML](https://alephdata.github.io/followthemoney/ns/ftm.xml).
+        
+        ## Development environment
+        
+        For local development with a virtualenv:
+        
+        ```bash
+        python3 -mvenv .env
+        source .env/bin/activate
+        pip install -e ".[dev]"
+        ```
+        
+        Now you can run the tests with
+        
+        ```bash
+        make test
+        ```
+        
+        ## Releasing
+        
+        We release a lot of version of `followthemoney` because even small changes
+        to the code base require a pypi release to begin being used in `aleph`. To
+        this end, here's the steps for making a release:
+        
+        ```bash
+        git pull --rebase
+        make build
+        make test
+        git add . && git commit -m "Updating translation files"
+        bumpversion patch
+        git push --atomic origin main $(git describe --tags --abbrev=0)
+        ```
+        
+        This will create a new patch release and upload a distribution of it. If
+        the changes are more significant, you can run `bumpversion` with the `minor`
+        or `major` arguments.
+        
+        When the schema is updated, please update the docs, ideally including the
+        diagrams. For the RDF namespace and JavaScript version of the model, 
+        run `make generate`.
+        
+Platform: UNKNOWN
 Classifier: Intended Audience :: Developers
 Classifier: Operating System :: OS Independent
 Classifier: Programming Language :: Python
 Classifier: Programming Language :: Python :: 3.9
 Description-Content-Type: text/markdown
 Provides-Extra: dev
-License-File: LICENSE
-
-# Follow the Money
-
-[![ftm-build](https://github.com/alephdata/followthemoney/actions/workflows/build.yml/badge.svg)](https://github.com/alephdata/followthemoney/actions/workflows/build.yml)
-
-This repository contains a pragmatic data model for the entities most
-commonly used in investigative reporting: people, companies, assets,
-payments, court cases, etc.
-
-The purpose of this is not to model reality in an ideal data model, but
-rather to have a working data structure for researchers.
-
-`followthemoney` also contains code used to validate and normalize many
-of the elements of data, and to map tabular data into the model.
-
-## Documentation
-
-For a general introduction to `followthemoney`, check the high-level introduction:
-
-* https://followthemoney.tech
-
-Part of this package is a command-line tool that can be used to process and
-transform data in various ways. You can find a tutorial here:
-
-* https://followthemoney.tech/docs/cli/
-
-Besides the introductions, there is also a full reference documentation for the
-library and the contained ontology: 
-
-* https://followthemoney.tech/explorer/
-
-There's also a number of viewers for the RDF schema definitions generated
-from FollowTheMoney, e.g.:
-
-* [LODE documentation](http://150.146.207.114/lode/extract?url=https%3A%2F%2Falephdata.github.io%2Ffollowthemoney%2Fns%2Fftm.xml&owlapi=true&imported=true&lang=en)
-* [WebVOWL](https://service.tib.eu/webvowl/#iri=https://alephdata.github.io/followthemoney/ns/ftm.xml)
-* RDF/OWL specification in [XML](https://alephdata.github.io/followthemoney/ns/ftm.xml).
-
-## Development environment
-
-For local development with a virtualenv:
-
-```bash
-python3 -mvenv .env
-source .env/bin/activate
-pip install -e ".[dev]"
-```
-
-Now you can run the tests with
-
-```bash
-make test
-```
-
-## Releasing
-
-We release a lot of version of `followthemoney` because even small changes
-to the code base require a pypi release to begin being used in `aleph`. To
-this end, here's the steps for making a release:
-
-```bash
-git pull --rebase
-make build
-make test
-git add . && git commit -m "Updating translation files"
-bumpversion patch
-git push --atomic origin main $(git describe --tags --abbrev=0)
-```
-
-This will create a new patch release and upload a distribution of it. If
-the changes are more significant, you can run `bumpversion` with the `minor`
-or `major` arguments.
-
-When the schema is updated, please update the docs, ideally including the
-diagrams. For the RDF namespace and JavaScript version of the model, 
-run `make generate`.
```

### Comparing `followthemoney-3.4.4/followthemoney.egg-info/SOURCES.txt` & `followthemoney-3.5.0/followthemoney.egg-info/SOURCES.txt`

 * *Files 1% similar despite different names*

```diff
@@ -82,23 +82,25 @@
 followthemoney/schema/Interval.yaml
 followthemoney/schema/LegalEntity.yaml
 followthemoney/schema/License.yaml
 followthemoney/schema/Membership.yaml
 followthemoney/schema/Mention.yaml
 followthemoney/schema/Message.yaml
 followthemoney/schema/Note.yaml
+followthemoney/schema/Occupancy.yaml
 followthemoney/schema/Organization.yaml
 followthemoney/schema/Ownership.yaml
 followthemoney/schema/Package.yaml
 followthemoney/schema/Page.yaml
 followthemoney/schema/Pages.yaml
 followthemoney/schema/Passport.yaml
 followthemoney/schema/Payment.yaml
 followthemoney/schema/Person.yaml
 followthemoney/schema/PlainText.yaml
+followthemoney/schema/Position.yaml
 followthemoney/schema/Post.yaml
 followthemoney/schema/Project.yaml
 followthemoney/schema/ProjectParticipant.yaml
 followthemoney/schema/PublicBody.yaml
 followthemoney/schema/RealEstate.yaml
 followthemoney/schema/Representation.yaml
 followthemoney/schema/Sanction.yaml
```

### Comparing `followthemoney-3.4.4/followthemoney.egg-info/entry_points.txt` & `followthemoney-3.5.0/followthemoney.egg-info/entry_points.txt`

 * *Files 0% similar despite different names*

```diff
@@ -11,7 +11,8 @@
 csv = followthemoney.cli.exports:export_csv
 cypher = followthemoney.cli.exports:export_cypher
 excel = followthemoney.cli.exports:export_excel
 gexf = followthemoney.cli.exports:export_gexf
 mapping = followthemoney.cli.mapping:run_mapping
 rdf = followthemoney.cli.exports:export_rdf
 sieve = followthemoney.cli.sieve:sieve
+
```

### Comparing `followthemoney-3.4.4/followthemoney.egg-info/requires.txt` & `followthemoney-3.5.0/followthemoney.egg-info/requires.txt`

 * *Files 1% similar despite different names*

```diff
@@ -1,13 +1,13 @@
 babel<3.0.0,>=2.9.1
 pyyaml<7.0.0,>=5.0.0
 types-PyYAML
 sqlalchemy2-stubs
 banal<1.1.0,>=1.0.1
-click<8.1.4,>=8.0
+click<8.1.7,>=8.0
 stringcase<2.0.0,>=1.2.0
 requests<3.0.0,>=2.21.0
 python-levenshtein<1.0.0,>=0.12.0
 normality<3.0.0,>=2.1.1
 sqlalchemy<3.0.0,>=1.2.0
 countrynames<2.0.0,>=1.13.0
 languagecodes<2.0.0,>=1.1.0
```

### Comparing `followthemoney-3.4.4/setup.py` & `followthemoney-3.5.0/setup.py`

 * *Files 4% similar despite different names*

```diff
@@ -1,15 +1,15 @@
 from setuptools import setup, find_packages  # type: ignore
 
 with open("README.md") as f:
     long_description = f.read()
 
 setup(
     name="followthemoney",
-    version="3.4.4",
+    version="3.5.0",
     author="Organized Crime and Corruption Reporting Project",
     author_email="data@occrp.org",
     url="https://followthemoney.tech/",
     long_description=long_description,
     long_description_content_type="text/markdown",
     license="MIT",
     classifiers=[
@@ -31,15 +31,15 @@
     zip_safe=False,
     install_requires=[
         "babel >= 2.9.1, < 3.0.0",
         "pyyaml >= 5.0.0, < 7.0.0",
         "types-PyYAML",
         "sqlalchemy2-stubs",
         "banal >= 1.0.1, < 1.1.0",
-        "click >= 8.0, < 8.1.4",
+        "click >= 8.0, < 8.1.7",
         "stringcase >= 1.2.0, < 2.0.0",
         "requests >= 2.21.0, < 3.0.0",
         "python-levenshtein >= 0.12.0, < 1.0.0",
         "normality >= 2.1.1, < 3.0.0",
         "sqlalchemy >= 1.2.0, < 3.0.0",
         "countrynames >= 1.13.0, < 2.0.0",
         "languagecodes >= 1.1.0, < 2.0.0",
```

