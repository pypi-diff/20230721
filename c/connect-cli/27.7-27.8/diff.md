# Comparing `tmp/connect_cli-27.7.tar.gz` & `tmp/connect_cli-27.8.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "connect_cli-27.7.tar", max compression
+gzip compressed data, was "connect_cli-27.8.tar", max compression
```

## Comparing `connect_cli-27.7.tar` & `connect_cli-27.8.tar`

### file list

```diff
@@ -1,287 +1,287 @@
--rw-r--r--   0        0        0    11357 2023-07-14 17:47:46.142966 connect_cli-27.7/LICENSE
--rw-r--r--   0        0        0     3280 2023-07-14 17:47:46.142966 connect_cli-27.7/README.md
--rw-r--r--   0        0        0     1823 2023-07-14 17:51:00.189972 connect_cli-27.7/connect/.data/connect_reports/.github/workflows/build.yml
--rw-r--r--   0        0        0      166 2023-07-14 17:51:00.189972 connect_cli-27.7/connect/.data/connect_reports/.gitignore
--rw-r--r--   0        0        0    10756 2023-07-14 17:51:00.189972 connect_cli-27.7/connect/.data/connect_reports/LICENSE
--rw-r--r--   0        0        0      708 2023-07-14 17:51:00.189972 connect_cli-27.7/connect/.data/connect_reports/README.md
--rw-r--r--   0        0        0   122573 2023-07-14 17:51:00.189972 connect_cli-27.7/connect/.data/connect_reports/poetry.lock
--rw-r--r--   0        0        0     1221 2023-07-14 17:51:00.189972 connect_cli-27.7/connect/.data/connect_reports/pyproject.toml
--rw-r--r--   0        0        0        0 2023-07-14 17:51:00.189972 connect_cli-27.7/connect/.data/connect_reports/reports/__init__.py
--rw-r--r--   0        0        0      215 2023-07-14 17:51:00.189972 connect_cli-27.7/connect/.data/connect_reports/reports/billing_requests/Readme.md
--rw-r--r--   0        0        0        0 2023-07-14 17:51:00.189972 connect_cli-27.7/connect/.data/connect_reports/reports/billing_requests/__init__.py
--rw-r--r--   0        0        0     3762 2023-07-14 17:51:00.189972 connect_cli-27.7/connect/.data/connect_reports/reports/billing_requests/entrypoint.py
--rw-r--r--   0        0        0     9038 2023-07-14 17:51:00.189972 connect_cli-27.7/connect/.data/connect_reports/reports/billing_requests/templates/xlsx/template.xlsx
--rw-r--r--   0        0        0      377 2023-07-14 17:51:00.189972 connect_cli-27.7/connect/.data/connect_reports/reports/billing_requests_line_item/Readme.md
--rw-r--r--   0        0        0        0 2023-07-14 17:51:00.189972 connect_cli-27.7/connect/.data/connect_reports/reports/billing_requests_line_item/__init__.py
--rw-r--r--   0        0        0     4313 2023-07-14 17:51:00.189972 connect_cli-27.7/connect/.data/connect_reports/reports/billing_requests_line_item/entrypoint.py
--rw-r--r--   0        0        0     9214 2023-07-14 17:51:00.189972 connect_cli-27.7/connect/.data/connect_reports/reports/billing_requests_line_item/templates/xlsx/template.xlsx
--rw-r--r--   0        0        0      151 2023-07-14 17:51:00.189972 connect_cli-27.7/connect/.data/connect_reports/reports/contract_list/Readme.md
--rw-r--r--   0        0        0        0 2023-07-14 17:51:00.189972 connect_cli-27.7/connect/.data/connect_reports/reports/contract_list/__init__.py
--rw-r--r--   0        0        0     3114 2023-07-14 17:51:00.189972 connect_cli-27.7/connect/.data/connect_reports/reports/contract_list/entrypoint.py
--rw-r--r--   0        0        0     8883 2023-07-14 17:51:00.189972 connect_cli-27.7/connect/.data/connect_reports/reports/contract_list/templates/xlsx/template.xlsx
--rw-r--r--   0        0        0      175 2023-07-14 17:51:00.189972 connect_cli-27.7/connect/.data/connect_reports/reports/customers_list/Readme.md
--rw-r--r--   0        0        0        0 2023-07-14 17:51:00.189972 connect_cli-27.7/connect/.data/connect_reports/reports/customers_list/__init__.py
--rw-r--r--   0        0        0     3595 2023-07-14 17:51:00.189972 connect_cli-27.7/connect/.data/connect_reports/reports/customers_list/entrypoint.py
--rw-r--r--   0        0        0     8914 2023-07-14 17:51:00.189972 connect_cli-27.7/connect/.data/connect_reports/reports/customers_list/templates/xlsx/template.xlsx
--rw-r--r--   0        0        0      546 2023-07-14 17:51:00.189972 connect_cli-27.7/connect/.data/connect_reports/reports/executive_fullfilment_requests/Readme.md
--rw-r--r--   0        0        0        0 2023-07-14 17:51:00.189972 connect_cli-27.7/connect/.data/connect_reports/reports/executive_fullfilment_requests/__init__.py
--rw-r--r--   0        0        0     6376 2023-07-14 17:51:00.189972 connect_cli-27.7/connect/.data/connect_reports/reports/executive_fullfilment_requests/constants.py
--rw-r--r--   0        0        0    17465 2023-07-14 17:51:00.189972 connect_cli-27.7/connect/.data/connect_reports/reports/executive_fullfilment_requests/entrypoint.py
--rw-r--r--   0        0        0     5254 2023-07-14 17:51:00.189972 connect_cli-27.7/connect/.data/connect_reports/reports/executive_fullfilment_requests/templates/pdf/img/ClouBlue-Logo.png
--rw-r--r--   0        0        0     3180 2023-07-14 17:51:00.189972 connect_cli-27.7/connect/.data/connect_reports/reports/executive_fullfilment_requests/templates/pdf/template.css
--rw-r--r--   0        0        0     1280 2023-07-14 17:51:00.189972 connect_cli-27.7/connect/.data/connect_reports/reports/executive_fullfilment_requests/templates/pdf/template.html.j2
--rw-r--r--   0        0        0      240 2023-07-14 17:51:00.189972 connect_cli-27.7/connect/.data/connect_reports/reports/fulfillment_requests/Readme.md
--rw-r--r--   0        0        0        0 2023-07-14 17:51:00.189972 connect_cli-27.7/connect/.data/connect_reports/reports/fulfillment_requests/__init__.py
--rw-r--r--   0        0        0     4584 2023-07-14 17:51:00.189972 connect_cli-27.7/connect/.data/connect_reports/reports/fulfillment_requests/entrypoint.py
--rw-r--r--   0        0        0     9160 2023-07-14 17:51:00.189972 connect_cli-27.7/connect/.data/connect_reports/reports/fulfillment_requests/templates/xlsx/template.xlsx
--rw-r--r--   0        0        0      301 2023-07-14 17:51:00.189972 connect_cli-27.7/connect/.data/connect_reports/reports/fulfillment_requests_failed/Readme.md
--rw-r--r--   0        0        0        0 2023-07-14 17:51:00.189972 connect_cli-27.7/connect/.data/connect_reports/reports/fulfillment_requests_failed/__init__.py
--rw-r--r--   0        0        0     4064 2023-07-14 17:51:00.189972 connect_cli-27.7/connect/.data/connect_reports/reports/fulfillment_requests_failed/entrypoint.py
--rw-r--r--   0        0        0     9050 2023-07-14 17:51:00.189972 connect_cli-27.7/connect/.data/connect_reports/reports/fulfillment_requests_failed/templates/xlsx/template.xlsx
--rw-r--r--   0        0        0      328 2023-07-14 17:51:00.189972 connect_cli-27.7/connect/.data/connect_reports/reports/fulfillment_requests_line_item/Readme.md
--rw-r--r--   0        0        0        0 2023-07-14 17:51:00.189972 connect_cli-27.7/connect/.data/connect_reports/reports/fulfillment_requests_line_item/__init__.py
--rw-r--r--   0        0        0     4982 2023-07-14 17:51:00.193973 connect_cli-27.7/connect/.data/connect_reports/reports/fulfillment_requests_line_item/entrypoint.py
--rw-r--r--   0        0        0     9234 2023-07-14 17:51:00.193973 connect_cli-27.7/connect/.data/connect_reports/reports/fulfillment_requests_line_item/templates/xlsx/template.xlsx
--rw-r--r--   0        0        0      180 2023-07-14 17:51:00.193973 connect_cli-27.7/connect/.data/connect_reports/reports/helpdesk/Readme.md
--rw-r--r--   0        0        0        0 2023-07-14 17:51:00.193973 connect_cli-27.7/connect/.data/connect_reports/reports/helpdesk/__init__.py
--rw-r--r--   0        0        0     2635 2023-07-14 17:51:00.193973 connect_cli-27.7/connect/.data/connect_reports/reports/helpdesk/entrypoint.py
--rw-r--r--   0        0        0     8749 2023-07-14 17:51:00.193973 connect_cli-27.7/connect/.data/connect_reports/reports/helpdesk/templates/xlsx/template.xlsx
--rw-r--r--   0        0        0      186 2023-07-14 17:51:00.193973 connect_cli-27.7/connect/.data/connect_reports/reports/listing_list/Readme.md
--rw-r--r--   0        0        0        0 2023-07-14 17:51:00.193973 connect_cli-27.7/connect/.data/connect_reports/reports/listing_list/__init__.py
--rw-r--r--   0        0        0     2632 2023-07-14 17:51:00.193973 connect_cli-27.7/connect/.data/connect_reports/reports/listing_list/entrypoint.py
--rw-r--r--   0        0        0     8703 2023-07-14 17:51:00.193973 connect_cli-27.7/connect/.data/connect_reports/reports/listing_list/templates/xlsx/template.xlsx
--rw-r--r--   0        0        0      194 2023-07-14 17:51:00.193973 connect_cli-27.7/connect/.data/connect_reports/reports/listing_requests/Readme.md
--rw-r--r--   0        0        0        0 2023-07-14 17:51:00.193973 connect_cli-27.7/connect/.data/connect_reports/reports/listing_requests/__init__.py
--rw-r--r--   0        0        0     2870 2023-07-14 17:51:00.193973 connect_cli-27.7/connect/.data/connect_reports/reports/listing_requests/entrypoint.py
--rw-r--r--   0        0        0     8746 2023-07-14 17:51:00.193973 connect_cli-27.7/connect/.data/connect_reports/reports/listing_requests/templates/xlsx/template.xlsx
--rw-r--r--   0        0        0      117 2023-07-14 17:51:00.193973 connect_cli-27.7/connect/.data/connect_reports/reports/products_catalog/Readme.md
--rw-r--r--   0        0        0        0 2023-07-14 17:51:00.193973 connect_cli-27.7/connect/.data/connect_reports/reports/products_catalog/__init__.py
--rw-r--r--   0        0        0     2582 2023-07-14 17:51:00.193973 connect_cli-27.7/connect/.data/connect_reports/reports/products_catalog/entrypoint.py
--rwxr-xr-x   0        0        0     7209 2023-07-14 17:51:00.193973 connect_cli-27.7/connect/.data/connect_reports/reports/products_catalog/templates/pdf/assets/cloudblue-connect-alone.png
--rw-r--r--   0        0        0    33448 2023-07-14 17:51:00.193973 connect_cli-27.7/connect/.data/connect_reports/reports/products_catalog/templates/pdf/assets/cloudblue-logo.png
--rw-r--r--   0        0        0    11287 2023-07-14 17:51:00.193973 connect_cli-27.7/connect/.data/connect_reports/reports/products_catalog/templates/pdf/assets/cloudblue-small-color-disabled.png
--rw-r--r--   0        0        0     9404 2023-07-14 17:51:00.193973 connect_cli-27.7/connect/.data/connect_reports/reports/products_catalog/templates/pdf/assets/cloudblue-small-color-enabled.png
--rw-r--r--   0        0        0    91722 2023-07-14 17:51:00.193973 connect_cli-27.7/connect/.data/connect_reports/reports/products_catalog/templates/pdf/assets/connect-logo.png
--rw-r--r--   0        0        0   465078 2023-07-14 17:51:00.197973 connect_cli-27.7/connect/.data/connect_reports/reports/products_catalog/templates/pdf/assets/cover-bg.png
--rw-r--r--   0        0        0    10941 2023-07-14 17:51:00.197973 connect_cli-27.7/connect/.data/connect_reports/reports/products_catalog/templates/pdf/assets/imc-small-color.png
--rw-r--r--   0        0        0    16685 2023-07-14 17:51:00.197973 connect_cli-27.7/connect/.data/connect_reports/reports/products_catalog/templates/pdf/img/ClouBlue-Logo-Black.png
--rw-r--r--   0        0        0     3555 2023-07-14 17:51:00.197973 connect_cli-27.7/connect/.data/connect_reports/reports/products_catalog/templates/pdf/img/ClouBlue-Logo-White.png
--rw-r--r--   0        0        0     5254 2023-07-14 17:51:00.197973 connect_cli-27.7/connect/.data/connect_reports/reports/products_catalog/templates/pdf/img/ClouBlue-Logo.png
--rw-r--r--   0        0        0     8250 2023-07-14 17:51:00.197973 connect_cli-27.7/connect/.data/connect_reports/reports/products_catalog/templates/pdf/img/accordo.png
--rw-r--r--   0        0        0     1311 2023-07-14 17:51:00.197973 connect_cli-27.7/connect/.data/connect_reports/reports/products_catalog/templates/pdf/img/acronis-blue.png
--rw-r--r--   0        0        0     1968 2023-07-14 17:51:00.197973 connect_cli-27.7/connect/.data/connect_reports/reports/products_catalog/templates/pdf/img/acronis-white.png
--rw-r--r--   0        0        0   124929 2023-07-14 17:51:00.197973 connect_cli-27.7/connect/.data/connect_reports/reports/products_catalog/templates/pdf/img/adobe.jpeg
--rw-r--r--   0        0        0    10421 2023-07-14 17:51:00.197973 connect_cli-27.7/connect/.data/connect_reports/reports/products_catalog/templates/pdf/img/airtame.png
--rw-r--r--   0        0        0      876 2023-07-14 17:51:00.197973 connect_cli-27.7/connect/.data/connect_reports/reports/products_catalog/templates/pdf/img/allyhub.png
--rw-r--r--   0        0        0     4615 2023-07-14 17:51:00.197973 connect_cli-27.7/connect/.data/connect_reports/reports/products_catalog/templates/pdf/img/alsid.png
--rw-r--r--   0        0        0    12369 2023-07-14 17:51:00.197973 connect_cli-27.7/connect/.data/connect_reports/reports/products_catalog/templates/pdf/img/anchor.png
--rw-r--r--   0        0        0     5200 2023-07-14 17:51:00.197973 connect_cli-27.7/connect/.data/connect_reports/reports/products_catalog/templates/pdf/img/australia.png
--rw-r--r--   0        0        0     3371 2023-07-14 17:51:00.197973 connect_cli-27.7/connect/.data/connect_reports/reports/products_catalog/templates/pdf/img/austria.png
--rw-r--r--   0        0        0    60306 2023-07-14 17:51:00.197973 connect_cli-27.7/connect/.data/connect_reports/reports/products_catalog/templates/pdf/img/aws.png
--rw-r--r--   0        0        0     3030 2023-07-14 17:51:00.197973 connect_cli-27.7/connect/.data/connect_reports/reports/products_catalog/templates/pdf/img/belgium.png
--rw-r--r--   0        0        0     5606 2023-07-14 17:51:00.197973 connect_cli-27.7/connect/.data/connect_reports/reports/products_catalog/templates/pdf/img/brazil.png
--rw-r--r--   0        0        0     3693 2023-07-14 17:51:00.197973 connect_cli-27.7/connect/.data/connect_reports/reports/products_catalog/templates/pdf/img/canada.png
--rw-r--r--   0        0        0     3870 2023-07-14 17:51:00.197973 connect_cli-27.7/connect/.data/connect_reports/reports/products_catalog/templates/pdf/img/chile.png
--rw-r--r--   0        0        0     3086 2023-07-14 17:51:00.197973 connect_cli-27.7/connect/.data/connect_reports/reports/products_catalog/templates/pdf/img/colombia.png
--rw-r--r--   0        0        0     3670 2023-07-14 17:51:00.197973 connect_cli-27.7/connect/.data/connect_reports/reports/products_catalog/templates/pdf/img/france.png
--rw-r--r--   0        0        0     3212 2023-07-14 17:51:00.197973 connect_cli-27.7/connect/.data/connect_reports/reports/products_catalog/templates/pdf/img/germany.png
--rw-r--r--   0        0        0     4521 2023-07-14 17:51:00.197973 connect_cli-27.7/connect/.data/connect_reports/reports/products_catalog/templates/pdf/img/hong-kong.png
--rw-r--r--   0        0        0    12000 2023-07-14 17:51:00.197973 connect_cli-27.7/connect/.data/connect_reports/reports/products_catalog/templates/pdf/img/icon.png
--rw-r--r--   0        0        0     4491 2023-07-14 17:51:00.197973 connect_cli-27.7/connect/.data/connect_reports/reports/products_catalog/templates/pdf/img/india.png
--rw-r--r--   0        0        0     3622 2023-07-14 17:51:00.197973 connect_cli-27.7/connect/.data/connect_reports/reports/products_catalog/templates/pdf/img/italy.png
--rw-r--r--   0        0        0     5096 2023-07-14 17:51:00.197973 connect_cli-27.7/connect/.data/connect_reports/reports/products_catalog/templates/pdf/img/malaysia.png
--rw-r--r--   0        0        0     3897 2023-07-14 17:51:00.197973 connect_cli-27.7/connect/.data/connect_reports/reports/products_catalog/templates/pdf/img/mexico.png
--rw-r--r--   0        0        0     3633 2023-07-14 17:51:00.197973 connect_cli-27.7/connect/.data/connect_reports/reports/products_catalog/templates/pdf/img/netherlands.png
--rw-r--r--   0        0        0     5173 2023-07-14 17:51:00.197973 connect_cli-27.7/connect/.data/connect_reports/reports/products_catalog/templates/pdf/img/new-zealand.png
--rw-r--r--   0        0        0     4163 2023-07-14 17:51:00.201973 connect_cli-27.7/connect/.data/connect_reports/reports/products_catalog/templates/pdf/img/singapore.png
--rw-r--r--   0        0        0     4670 2023-07-14 17:51:00.201973 connect_cli-27.7/connect/.data/connect_reports/reports/products_catalog/templates/pdf/img/spain.png
--rw-r--r--   0        0        0     4802 2023-07-14 17:51:00.201973 connect_cli-27.7/connect/.data/connect_reports/reports/products_catalog/templates/pdf/img/sweden.png
--rw-r--r--   0        0        0     3622 2023-07-14 17:51:00.201973 connect_cli-27.7/connect/.data/connect_reports/reports/products_catalog/templates/pdf/img/switzerland.png
--rw-r--r--   0        0        0     4073 2023-07-14 17:51:00.201973 connect_cli-27.7/connect/.data/connect_reports/reports/products_catalog/templates/pdf/img/turkey.png
--rw-r--r--   0        0        0     3350 2023-07-14 17:51:00.201973 connect_cli-27.7/connect/.data/connect_reports/reports/products_catalog/templates/pdf/img/uae.png
--rw-r--r--   0        0        0     5583 2023-07-14 17:51:00.201973 connect_cli-27.7/connect/.data/connect_reports/reports/products_catalog/templates/pdf/img/uk.png
--rw-r--r--   0        0        0     4892 2023-07-14 17:51:00.201973 connect_cli-27.7/connect/.data/connect_reports/reports/products_catalog/templates/pdf/img/usa.png
--rw-r--r--   0        0        0     4063 2023-07-14 17:51:00.201973 connect_cli-27.7/connect/.data/connect_reports/reports/products_catalog/templates/pdf/template.css
--rw-r--r--   0        0        0     1736 2023-07-14 17:51:00.201973 connect_cli-27.7/connect/.data/connect_reports/reports/products_catalog/templates/pdf/template.html.j2
--rw-r--r--   0        0        0      592 2023-07-14 17:51:00.201973 connect_cli-27.7/connect/.data/connect_reports/reports/sla/Readme.md
--rw-r--r--   0        0        0        0 2023-07-14 17:51:00.201973 connect_cli-27.7/connect/.data/connect_reports/reports/sla/__init__.py
--rw-r--r--   0        0        0     4125 2023-07-14 17:51:00.201973 connect_cli-27.7/connect/.data/connect_reports/reports/sla/entrypoint.py
--rw-r--r--   0        0        0     9679 2023-07-14 17:51:00.201973 connect_cli-27.7/connect/.data/connect_reports/reports/sla/templates/xlsx/template.xlsx
--rw-r--r--   0        0        0      260 2023-07-14 17:51:00.201973 connect_cli-27.7/connect/.data/connect_reports/reports/subscription_list/Readme.md
--rw-r--r--   0        0        0        0 2023-07-14 17:51:00.201973 connect_cli-27.7/connect/.data/connect_reports/reports/subscription_list/__init__.py
--rw-r--r--   0        0        0     6276 2023-07-14 17:51:00.201973 connect_cli-27.7/connect/.data/connect_reports/reports/subscription_list/entrypoint.py
--rw-r--r--   0        0        0     9302 2023-07-14 17:51:00.201973 connect_cli-27.7/connect/.data/connect_reports/reports/subscription_list/templates/xlsx/template.xlsx
--rw-r--r--   0        0        0      203 2023-07-14 17:51:00.201973 connect_cli-27.7/connect/.data/connect_reports/reports/tier_configuration_list/Readme.md
--rw-r--r--   0        0        0        0 2023-07-14 17:51:00.201973 connect_cli-27.7/connect/.data/connect_reports/reports/tier_configuration_list/__init__.py
--rw-r--r--   0        0        0     4282 2023-07-14 17:51:00.201973 connect_cli-27.7/connect/.data/connect_reports/reports/tier_configuration_list/entrypoint.py
--rw-r--r--   0        0        0     8925 2023-07-14 17:51:00.201973 connect_cli-27.7/connect/.data/connect_reports/reports/tier_configuration_list/templates/xlsx/template.xlsx
--rw-r--r--   0        0        0      228 2023-07-14 17:51:00.201973 connect_cli-27.7/connect/.data/connect_reports/reports/tier_configuration_requests/Readme.md
--rw-r--r--   0        0        0        0 2023-07-14 17:51:00.201973 connect_cli-27.7/connect/.data/connect_reports/reports/tier_configuration_requests/__init__.py
--rw-r--r--   0        0        0     5147 2023-07-14 17:51:00.201973 connect_cli-27.7/connect/.data/connect_reports/reports/tier_configuration_requests/entrypoint.py
--rw-r--r--   0        0        0     9070 2023-07-14 17:51:00.201973 connect_cli-27.7/connect/.data/connect_reports/reports/tier_configuration_requests/templates/xlsx/template.xlsx
--rw-r--r--   0        0        0      431 2023-07-14 17:51:00.201973 connect_cli-27.7/connect/.data/connect_reports/reports/usage_in_subscription/Readme.md
--rw-r--r--   0        0        0        0 2023-07-14 17:51:00.201973 connect_cli-27.7/connect/.data/connect_reports/reports/usage_in_subscription/__init__.py
--rw-r--r--   0        0        0     4106 2023-07-14 17:51:00.201973 connect_cli-27.7/connect/.data/connect_reports/reports/usage_in_subscription/entrypoint.py
--rw-r--r--   0        0        0     9137 2023-07-14 17:51:00.201973 connect_cli-27.7/connect/.data/connect_reports/reports/usage_in_subscription/templates/xlsx/template.xlsx
--rw-r--r--   0        0        0     1318 2023-07-14 17:51:00.201973 connect_cli-27.7/connect/.data/connect_reports/reports/utils.py
--rw-r--r--   0        0        0    37904 2023-07-14 17:51:00.189972 connect_cli-27.7/connect/.data/connect_reports/reports.json
--rw-r--r--   0        0        0      245 2023-07-14 17:51:00.201973 connect_cli-27.7/connect/.data/connect_reports/sonar-project.properties
--rw-r--r--   0        0        0      321 2023-07-14 17:51:00.201973 connect_cli-27.7/connect/.data/connect_reports/tox.ini
--rw-r--r--   0        0        0      352 2023-07-14 17:47:46.142966 connect_cli-27.7/connect/cli/__init__.py
--rw-r--r--   0        0        0     1763 2023-07-14 17:47:46.142966 connect_cli-27.7/connect/cli/ccli.py
--rw-r--r--   0        0        0       54 2023-07-14 17:47:46.142966 connect_cli-27.7/connect/cli/core/__init__.py
--rw-r--r--   0        0        0        0 2023-07-14 17:47:46.142966 connect_cli-27.7/connect/cli/core/account/__init__.py
--rw-r--r--   0        0        0     2433 2023-07-14 17:47:46.142966 connect_cli-27.7/connect/cli/core/account/commands.py
--rw-r--r--   0        0        0     1233 2023-07-14 17:47:46.142966 connect_cli-27.7/connect/cli/core/account/helpers.py
--rw-r--r--   0        0        0     2764 2023-07-14 17:47:46.142966 connect_cli-27.7/connect/cli/core/base.py
--rw-r--r--   0        0        0     4048 2023-07-14 17:47:46.142966 connect_cli-27.7/connect/cli/core/config.py
--rw-r--r--   0        0        0      573 2023-07-14 17:47:46.142966 connect_cli-27.7/connect/cli/core/constants.py
--rw-r--r--   0        0        0     1424 2023-07-14 17:47:46.142966 connect_cli-27.7/connect/cli/core/http.py
--rw-r--r--   0        0        0      838 2023-07-14 17:47:46.142966 connect_cli-27.7/connect/cli/core/plugins.py
--rw-r--r--   0        0        0     6836 2023-07-14 17:47:46.142966 connect_cli-27.7/connect/cli/core/terminal.py
--rw-r--r--   0        0        0     3139 2023-07-14 17:47:46.142966 connect_cli-27.7/connect/cli/core/utils.py
--rw-r--r--   0        0        0        0 2023-07-14 17:47:46.142966 connect_cli-27.7/connect/cli/plugins/__init__.py
--rw-r--r--   0        0        0        0 2023-07-14 17:47:46.142966 connect_cli-27.7/connect/cli/plugins/customer/__init__.py
--rw-r--r--   0        0        0     2137 2023-07-14 17:47:46.142966 connect_cli-27.7/connect/cli/plugins/customer/commands.py
--rw-r--r--   0        0        0      526 2023-07-14 17:47:46.142966 connect_cli-27.7/connect/cli/plugins/customer/constants.py
--rw-r--r--   0        0        0     6040 2023-07-14 17:47:46.142966 connect_cli-27.7/connect/cli/plugins/customer/export.py
--rw-r--r--   0        0        0    12696 2023-07-14 17:47:46.142966 connect_cli-27.7/connect/cli/plugins/customer/sync.py
--rw-r--r--   0        0        0        0 2023-07-14 17:47:46.146966 connect_cli-27.7/connect/cli/plugins/locale/__init__.py
--rw-r--r--   0        0        0     1363 2023-07-14 17:47:46.146966 connect_cli-27.7/connect/cli/plugins/locale/commands.py
--rw-r--r--   0        0        0      306 2023-07-14 17:47:46.146966 connect_cli-27.7/connect/cli/plugins/play/__init__.py
--rw-r--r--   0        0        0     2485 2023-07-14 17:47:46.146966 connect_cli-27.7/connect/cli/plugins/play/commands.py
--rw-r--r--   0        0        0     2395 2023-07-14 17:47:46.146966 connect_cli-27.7/connect/cli/plugins/play/context.py
--rw-r--r--   0        0        0      428 2023-07-14 17:47:46.146966 connect_cli-27.7/connect/cli/plugins/play/save.py
--rw-r--r--   0        0        0     1647 2023-07-14 17:47:46.146966 connect_cli-27.7/connect/cli/plugins/play/script.py
--rw-r--r--   0        0        0        0 2023-07-14 17:47:46.146966 connect_cli-27.7/connect/cli/plugins/product/__init__.py
--rw-r--r--   0        0        0     1575 2023-07-14 17:47:46.146966 connect_cli-27.7/connect/cli/plugins/product/api.py
--rw-r--r--   0        0        0     8628 2023-07-14 17:47:46.146966 connect_cli-27.7/connect/cli/plugins/product/clone.py
--rw-r--r--   0        0        0     9659 2023-07-14 17:47:46.146966 connect_cli-27.7/connect/cli/plugins/product/commands.py
--rw-r--r--   0        0        0     1289 2023-07-14 17:47:46.146966 connect_cli-27.7/connect/cli/plugins/product/constants.py
--rw-r--r--   0        0        0    33455 2023-07-14 17:47:46.146966 connect_cli-27.7/connect/cli/plugins/product/export.py
--rw-r--r--   0        0        0      846 2023-07-14 17:47:46.146966 connect_cli-27.7/connect/cli/plugins/product/sync/__init__.py
--rw-r--r--   0        0        0     5932 2023-07-14 17:47:46.146966 connect_cli-27.7/connect/cli/plugins/product/sync/actions.py
--rw-r--r--   0        0        0     8988 2023-07-14 17:47:46.146966 connect_cli-27.7/connect/cli/plugins/product/sync/capabilities.py
--rw-r--r--   0        0        0     3881 2023-07-14 17:47:46.146966 connect_cli-27.7/connect/cli/plugins/product/sync/configuration_values.py
--rw-r--r--   0        0        0     5096 2023-07-14 17:47:46.146966 connect_cli-27.7/connect/cli/plugins/product/sync/general.py
--rw-r--r--   0        0        0    11349 2023-07-14 17:47:46.146966 connect_cli-27.7/connect/cli/plugins/product/sync/items.py
--rw-r--r--   0        0        0     5846 2023-07-14 17:47:46.146966 connect_cli-27.7/connect/cli/plugins/product/sync/media.py
--rw-r--r--   0        0        0     9460 2023-07-14 17:47:46.146966 connect_cli-27.7/connect/cli/plugins/product/sync/params.py
--rw-r--r--   0        0        0     3598 2023-07-14 17:47:46.146966 connect_cli-27.7/connect/cli/plugins/product/sync/static_resources.py
--rw-r--r--   0        0        0     5303 2023-07-14 17:47:46.146966 connect_cli-27.7/connect/cli/plugins/product/sync/templates.py
--rw-r--r--   0        0        0      985 2023-07-14 17:47:46.146966 connect_cli-27.7/connect/cli/plugins/product/utils.py
--rw-r--r--   0        0        0        0 2023-07-14 17:47:46.146966 connect_cli-27.7/connect/cli/plugins/project/__init__.py
--rw-r--r--   0        0        0     5791 2023-07-14 17:47:46.146966 connect_cli-27.7/connect/cli/plugins/project/commands.py
--rw-r--r--   0        0        0        0 2023-07-14 17:47:46.146966 connect_cli-27.7/connect/cli/plugins/project/extension/__init__.py
--rw-r--r--   0        0        0      411 2023-07-14 17:47:46.146966 connect_cli-27.7/connect/cli/plugins/project/extension/constants.py
--rw-r--r--   0        0        0    10802 2023-07-14 17:47:46.146966 connect_cli-27.7/connect/cli/plugins/project/extension/helpers.py
--rw-r--r--   0        0        0      103 2023-07-14 17:47:46.146966 connect_cli-27.7/connect/cli/plugins/project/extension/templates/bootstrap/${project_slug}/${package_name}/__init__.py.j2
--rw-r--r--   0        0        0      852 2023-07-14 17:47:46.146966 connect_cli-27.7/connect/cli/plugins/project/extension/templates/bootstrap/${project_slug}/${package_name}/anvil.py.j2
--rw-r--r--   0        0        0     2920 2023-07-14 17:47:46.146966 connect_cli-27.7/connect/cli/plugins/project/extension/templates/bootstrap/${project_slug}/${package_name}/events.py.j2
--rw-r--r--   0        0        0      464 2023-07-14 17:47:46.146966 connect_cli-27.7/connect/cli/plugins/project/extension/templates/bootstrap/${project_slug}/${package_name}/extension.json.j2
--rw-r--r--   0        0        0      560 2023-07-14 17:47:46.146966 connect_cli-27.7/connect/cli/plugins/project/extension/templates/bootstrap/${project_slug}/${package_name}/schemas.py.j2
--rw-r--r--   0        0        0        0 2023-07-14 17:47:46.146966 connect_cli-27.7/connect/cli/plugins/project/extension/templates/bootstrap/${project_slug}/${package_name}/static/.gitkeep.j2
--rw-r--r--   0        0        0     1762 2023-07-14 17:47:46.146966 connect_cli-27.7/connect/cli/plugins/project/extension/templates/bootstrap/${project_slug}/${package_name}/tfnapp.py.j2
--rw-r--r--   0        0        0     7295 2023-07-14 17:47:46.146966 connect_cli-27.7/connect/cli/plugins/project/extension/templates/bootstrap/${project_slug}/${package_name}/webapp.py.j2
--rw-r--r--   0        0        0      702 2023-07-14 17:47:46.146966 connect_cli-27.7/connect/cli/plugins/project/extension/templates/bootstrap/${project_slug}/.${project_slug}_dev.env.j2
--rw-r--r--   0        0        0     1083 2023-07-14 17:47:46.146966 connect_cli-27.7/connect/cli/plugins/project/extension/templates/bootstrap/${project_slug}/.eslintrc.yaml.j2
--rw-r--r--   0        0        0      231 2023-07-14 17:47:46.146966 connect_cli-27.7/connect/cli/plugins/project/extension/templates/bootstrap/${project_slug}/.flake8.j2
--rw-r--r--   0        0        0     1309 2023-07-14 17:47:46.146966 connect_cli-27.7/connect/cli/plugins/project/extension/templates/bootstrap/${project_slug}/.github/workflows/test.yml.j2
--rw-r--r--   0        0        0       96 2023-07-14 17:47:46.146966 connect_cli-27.7/connect/cli/plugins/project/extension/templates/bootstrap/${project_slug}/.gitignore.j2
--rw-r--r--   0        0        0       63 2023-07-14 17:47:46.146966 connect_cli-27.7/connect/cli/plugins/project/extension/templates/bootstrap/${project_slug}/CHANGELOG.md.j2
--rw-r--r--   0        0        0      249 2023-07-14 17:47:46.146966 connect_cli-27.7/connect/cli/plugins/project/extension/templates/bootstrap/${project_slug}/Dockerfile.j2
--rw-r--r--   0        0        0     1661 2023-07-14 17:47:46.146966 connect_cli-27.7/connect/cli/plugins/project/extension/templates/bootstrap/${project_slug}/HOWTO.md.j2
--rw-r--r--   0        0        0    14063 2023-07-14 17:47:46.146966 connect_cli-27.7/connect/cli/plugins/project/extension/templates/bootstrap/${project_slug}/LICENSE.j2
--rw-r--r--   0        0        0      195 2023-07-14 17:47:46.146966 connect_cli-27.7/connect/cli/plugins/project/extension/templates/bootstrap/${project_slug}/README.md.j2
--rw-r--r--   0        0        0      111 2023-07-14 17:47:46.146966 connect_cli-27.7/connect/cli/plugins/project/extension/templates/bootstrap/${project_slug}/__mocks__/fileMock.js.j2
--rw-r--r--   0        0        0       97 2023-07-14 17:47:46.146966 connect_cli-27.7/connect/cli/plugins/project/extension/templates/bootstrap/${project_slug}/__mocks__/styleMock.js.j2
--rw-r--r--   0        0        0       39 2023-07-14 17:47:46.146966 connect_cli-27.7/connect/cli/plugins/project/extension/templates/bootstrap/${project_slug}/babel.config.json.j2
--rw-r--r--   0        0        0     1162 2023-07-14 17:47:46.146966 connect_cli-27.7/connect/cli/plugins/project/extension/templates/bootstrap/${project_slug}/docker-compose.yml.j2
--rw-r--r--   0        0        0      944 2023-07-14 17:47:46.146966 connect_cli-27.7/connect/cli/plugins/project/extension/templates/bootstrap/${project_slug}/jest.config.js.j2
--rw-r--r--   0        0        0     1246 2023-07-14 17:47:46.146966 connect_cli-27.7/connect/cli/plugins/project/extension/templates/bootstrap/${project_slug}/package.json.j2
--rw-r--r--   0        0        0       29 2023-07-14 17:47:46.146966 connect_cli-27.7/connect/cli/plugins/project/extension/templates/bootstrap/${project_slug}/poetry.toml.j2
--rw-r--r--   0        0        0     1960 2023-07-14 17:47:46.146966 connect_cli-27.7/connect/cli/plugins/project/extension/templates/bootstrap/${project_slug}/pyproject.toml.j2
--rw-r--r--   0        0        0      103 2023-07-14 17:47:46.146966 connect_cli-27.7/connect/cli/plugins/project/extension/templates/bootstrap/${project_slug}/tests/__init__.py.j2
--rw-r--r--   0        0        0      559 2023-07-14 17:47:46.146966 connect_cli-27.7/connect/cli/plugins/project/extension/templates/bootstrap/${project_slug}/tests/conftest.py.j2
--rw-r--r--   0        0        0      553 2023-07-14 17:47:46.146966 connect_cli-27.7/connect/cli/plugins/project/extension/templates/bootstrap/${project_slug}/tests/test_anvil.py.j2
--rw-r--r--   0        0        0     2602 2023-07-14 17:47:46.146966 connect_cli-27.7/connect/cli/plugins/project/extension/templates/bootstrap/${project_slug}/tests/test_events.py.j2
--rw-r--r--   0        0        0     1183 2023-07-14 17:47:46.146966 connect_cli-27.7/connect/cli/plugins/project/extension/templates/bootstrap/${project_slug}/tests/test_tfnapp.py.j2
--rw-r--r--   0        0        0     8794 2023-07-14 17:47:46.146966 connect_cli-27.7/connect/cli/plugins/project/extension/templates/bootstrap/${project_slug}/tests/test_webapp.py.j2
--rw-r--r--   0        0        0      947 2023-07-14 17:47:46.146966 connect_cli-27.7/connect/cli/plugins/project/extension/templates/bootstrap/${project_slug}/ui/images/mkp.svg.j2
--rw-r--r--   0        0        0      729 2023-07-14 17:47:46.146966 connect_cli-27.7/connect/cli/plugins/project/extension/templates/bootstrap/${project_slug}/ui/pages/index.html.j2
--rw-r--r--   0        0        0      928 2023-07-14 17:47:46.146966 connect_cli-27.7/connect/cli/plugins/project/extension/templates/bootstrap/${project_slug}/ui/pages/settings.html.j2
--rw-r--r--   0        0        0      470 2023-07-14 17:47:46.146966 connect_cli-27.7/connect/cli/plugins/project/extension/templates/bootstrap/${project_slug}/ui/pages/transformations/copy.html.j2
--rw-r--r--   0        0        0     1590 2023-07-14 17:47:46.146966 connect_cli-27.7/connect/cli/plugins/project/extension/templates/bootstrap/${project_slug}/ui/pages/transformations/manual.html.j2
--rw-r--r--   0        0        0     2609 2023-07-14 17:47:46.146966 connect_cli-27.7/connect/cli/plugins/project/extension/templates/bootstrap/${project_slug}/ui/src/components.js.j2
--rw-r--r--   0        0        0      323 2023-07-14 17:47:46.146966 connect_cli-27.7/connect/cli/plugins/project/extension/templates/bootstrap/${project_slug}/ui/src/pages/index.js.j2
--rw-r--r--   0        0        0      320 2023-07-14 17:47:46.146966 connect_cli-27.7/connect/cli/plugins/project/extension/templates/bootstrap/${project_slug}/ui/src/pages/settings.js.j2
--rw-r--r--   0        0        0      267 2023-07-14 17:47:46.146966 connect_cli-27.7/connect/cli/plugins/project/extension/templates/bootstrap/${project_slug}/ui/src/pages/transformations/copy.js.j2
--rw-r--r--   0        0        0      308 2023-07-14 17:47:46.146966 connect_cli-27.7/connect/cli/plugins/project/extension/templates/bootstrap/${project_slug}/ui/src/pages/transformations/manual.js.j2
--rw-r--r--   0        0        0    10273 2023-07-14 17:47:46.146966 connect_cli-27.7/connect/cli/plugins/project/extension/templates/bootstrap/${project_slug}/ui/src/pages.js.j2
--rw-r--r--   0        0        0     1579 2023-07-14 17:47:46.146966 connect_cli-27.7/connect/cli/plugins/project/extension/templates/bootstrap/${project_slug}/ui/src/utils.js.j2
--rw-r--r--   0        0        0     6381 2023-07-14 17:47:46.150966 connect_cli-27.7/connect/cli/plugins/project/extension/templates/bootstrap/${project_slug}/ui/styles/index.css.j2
--rw-r--r--   0        0        0      693 2023-07-14 17:47:46.150966 connect_cli-27.7/connect/cli/plugins/project/extension/templates/bootstrap/${project_slug}/ui/styles/manual.css.j2
--rw-r--r--   0        0        0     6508 2023-07-14 17:47:46.150966 connect_cli-27.7/connect/cli/plugins/project/extension/templates/bootstrap/${project_slug}/ui/tests/components.spec.js.j2
--rw-r--r--   0        0        0     9181 2023-07-14 17:47:46.150966 connect_cli-27.7/connect/cli/plugins/project/extension/templates/bootstrap/${project_slug}/ui/tests/pages.spec.js.j2
--rw-r--r--   0        0        0     4352 2023-07-14 17:47:46.150966 connect_cli-27.7/connect/cli/plugins/project/extension/templates/bootstrap/${project_slug}/ui/tests/utils.spec.js.j2
--rw-r--r--   0        0        0     2512 2023-07-14 17:47:46.150966 connect_cli-27.7/connect/cli/plugins/project/extension/templates/bootstrap/${project_slug}/webpack.config.js.j2
--rw-r--r--   0        0        0     4487 2023-07-14 17:47:46.150966 connect_cli-27.7/connect/cli/plugins/project/extension/utils.py
--rw-r--r--   0        0        0      805 2023-07-14 17:47:46.150966 connect_cli-27.7/connect/cli/plugins/project/extension/validators.py
--rw-r--r--   0        0        0    12083 2023-07-14 17:47:46.150966 connect_cli-27.7/connect/cli/plugins/project/extension/wizard.py
--rw-r--r--   0        0        0     5929 2023-07-14 17:47:46.150966 connect_cli-27.7/connect/cli/plugins/project/renderer.py
--rw-r--r--   0        0        0        0 2023-07-14 17:47:46.150966 connect_cli-27.7/connect/cli/plugins/project/report/__init__.py
--rw-r--r--   0        0        0     8611 2023-07-14 17:47:46.150966 connect_cli-27.7/connect/cli/plugins/project/report/helpers.py
--rw-r--r--   0        0        0       73 2023-07-14 17:47:46.150966 connect_cli-27.7/connect/cli/plugins/project/report/templates/add/${initial_report_slug}/README.md.j2
--rw-r--r--   0        0        0        0 2023-07-14 17:47:46.150966 connect_cli-27.7/connect/cli/plugins/project/report/templates/add/${initial_report_slug}/__init__.py.j2
--rw-r--r--   0        0        0     1507 2023-07-14 17:47:46.150966 connect_cli-27.7/connect/cli/plugins/project/report/templates/add/${initial_report_slug}/entrypoint.py.j2
--rw-r--r--   0        0        0        0 2023-07-14 17:47:46.150966 connect_cli-27.7/connect/cli/plugins/project/report/templates/add/${initial_report_slug}/templates/pdf/template.css.j2
--rw-r--r--   0        0        0      499 2023-07-14 17:47:46.150966 connect_cli-27.7/connect/cli/plugins/project/report/templates/add/${initial_report_slug}/templates/pdf/template.html.j2.j2
--rw-r--r--   0        0        0      150 2023-07-14 17:47:46.150966 connect_cli-27.7/connect/cli/plugins/project/report/templates/add/${initial_report_slug}/templates/xml/template.xml.j2.j2
--rw-r--r--   0        0        0       69 2023-07-14 17:47:46.150966 connect_cli-27.7/connect/cli/plugins/project/report/templates/bootstrap/${project_slug}/${package_name}/${initial_report_slug}/README.md.j2
--rw-r--r--   0        0        0        0 2023-07-14 17:47:46.150966 connect_cli-27.7/connect/cli/plugins/project/report/templates/bootstrap/${project_slug}/${package_name}/${initial_report_slug}/__init__.py.j2
--rw-r--r--   0        0        0     1507 2023-07-14 17:47:46.150966 connect_cli-27.7/connect/cli/plugins/project/report/templates/bootstrap/${project_slug}/${package_name}/${initial_report_slug}/entrypoint.py.j2
--rw-r--r--   0        0        0        0 2023-07-14 17:47:46.150966 connect_cli-27.7/connect/cli/plugins/project/report/templates/bootstrap/${project_slug}/${package_name}/${initial_report_slug}/templates/pdf/template.css.j2
--rw-r--r--   0        0        0      518 2023-07-14 17:47:46.150966 connect_cli-27.7/connect/cli/plugins/project/report/templates/bootstrap/${project_slug}/${package_name}/${initial_report_slug}/templates/pdf/template.html.j2.j2
--rw-r--r--   0        0        0      150 2023-07-14 17:47:46.150966 connect_cli-27.7/connect/cli/plugins/project/report/templates/bootstrap/${project_slug}/${package_name}/${initial_report_slug}/templates/xml/template.xml.j2.j2
--rw-r--r--   0        0        0      271 2023-07-14 17:47:46.150966 connect_cli-27.7/connect/cli/plugins/project/report/templates/bootstrap/${project_slug}/.flake8.j2
--rw-r--r--   0        0        0      803 2023-07-14 17:47:46.150966 connect_cli-27.7/connect/cli/plugins/project/report/templates/bootstrap/${project_slug}/.github/workflows/build.yml.j2
--rw-r--r--   0        0        0       37 2023-07-14 17:47:46.150966 connect_cli-27.7/connect/cli/plugins/project/report/templates/bootstrap/${project_slug}/.gitignore.j2
--rw-r--r--   0        0        0      458 2023-07-14 17:47:46.150966 connect_cli-27.7/connect/cli/plugins/project/report/templates/bootstrap/${project_slug}/HOWTO.md.j2
--rw-r--r--   0        0        0    14063 2023-07-14 17:47:46.150966 connect_cli-27.7/connect/cli/plugins/project/report/templates/bootstrap/${project_slug}/LICENSE.j2
--rw-r--r--   0        0        0      138 2023-07-14 17:47:46.150966 connect_cli-27.7/connect/cli/plugins/project/report/templates/bootstrap/${project_slug}/README.md.j2
--rw-r--r--   0        0        0       29 2023-07-14 17:47:46.150966 connect_cli-27.7/connect/cli/plugins/project/report/templates/bootstrap/${project_slug}/poetry.toml.j2
--rw-r--r--   0        0        0     1352 2023-07-14 17:47:46.150966 connect_cli-27.7/connect/cli/plugins/project/report/templates/bootstrap/${project_slug}/pyproject.toml.j2
--rw-r--r--   0        0        0     2589 2023-07-14 17:47:46.150966 connect_cli-27.7/connect/cli/plugins/project/report/templates/bootstrap/${project_slug}/reports.json.j2
--rw-r--r--   0        0        0      103 2023-07-14 17:47:46.150966 connect_cli-27.7/connect/cli/plugins/project/report/templates/bootstrap/${project_slug}/tests/__init__.py.j2
--rw-r--r--   0        0        0     6397 2023-07-14 17:47:46.150966 connect_cli-27.7/connect/cli/plugins/project/report/templates/bootstrap/${project_slug}/tests/conftest.py.j2
--rw-r--r--   0        0        0     2534 2023-07-14 17:47:46.150966 connect_cli-27.7/connect/cli/plugins/project/report/templates/bootstrap/${project_slug}/tests/test_${project_slug}.py.j2
--rw-r--r--   0        0        0     5877 2023-07-14 17:47:46.150966 connect_cli-27.7/connect/cli/plugins/project/report/validations.py
--rw-r--r--   0        0        0     8615 2023-07-14 17:47:46.150966 connect_cli-27.7/connect/cli/plugins/project/report/wizard.py
--rw-r--r--   0        0        0     1443 2023-07-14 17:47:46.150966 connect_cli-27.7/connect/cli/plugins/project/utils.py
--rw-r--r--   0        0        0     2798 2023-07-14 17:47:46.150966 connect_cli-27.7/connect/cli/plugins/project/validators.py
--rw-r--r--   0        0        0        0 2023-07-14 17:47:46.150966 connect_cli-27.7/connect/cli/plugins/report/__init__.py
--rw-r--r--   0        0        0     2405 2023-07-14 17:47:46.150966 connect_cli-27.7/connect/cli/plugins/report/commands.py
--rw-r--r--   0        0        0       86 2023-07-14 17:47:46.150966 connect_cli-27.7/connect/cli/plugins/report/constants.py
--rw-r--r--   0        0        0     6210 2023-07-14 17:47:46.150966 connect_cli-27.7/connect/cli/plugins/report/helpers.py
--rw-r--r--   0        0        0     2822 2023-07-14 17:47:46.150966 connect_cli-27.7/connect/cli/plugins/report/utils.py
--rw-r--r--   0        0        0     8345 2023-07-14 17:47:46.150966 connect_cli-27.7/connect/cli/plugins/report/wizard.py
--rw-r--r--   0        0        0        0 2023-07-14 17:47:46.150966 connect_cli-27.7/connect/cli/plugins/shared/__init__.py
--rw-r--r--   0        0        0     2441 2023-07-14 17:47:46.150966 connect_cli-27.7/connect/cli/plugins/shared/base.py
--rw-r--r--   0        0        0     1973 2023-07-14 17:47:46.150966 connect_cli-27.7/connect/cli/plugins/shared/constants.py
--rw-r--r--   0        0        0       46 2023-07-14 17:47:46.150966 connect_cli-27.7/connect/cli/plugins/shared/exceptions.py
--rw-r--r--   0        0        0     2375 2023-07-14 17:47:46.150966 connect_cli-27.7/connect/cli/plugins/shared/export.py
--rw-r--r--   0        0        0     6295 2023-07-14 17:47:46.150966 connect_cli-27.7/connect/cli/plugins/shared/sync_stats.py
--rw-r--r--   0        0        0     5739 2023-07-14 17:47:46.150966 connect_cli-27.7/connect/cli/plugins/shared/translation_attr_sync.py
--rw-r--r--   0        0        0     6534 2023-07-14 17:47:46.150966 connect_cli-27.7/connect/cli/plugins/shared/translation_sync.py
--rw-r--r--   0        0        0     2103 2023-07-14 17:47:46.150966 connect_cli-27.7/connect/cli/plugins/shared/translations_synchronizers.py
--rw-r--r--   0        0        0     6793 2023-07-14 17:47:46.150966 connect_cli-27.7/connect/cli/plugins/shared/utils.py
--rw-r--r--   0        0        0        0 2023-07-14 17:47:46.150966 connect_cli-27.7/connect/cli/plugins/translation/__init__.py
--rw-r--r--   0        0        0      707 2023-07-14 17:47:46.150966 connect_cli-27.7/connect/cli/plugins/translation/activate.py
--rw-r--r--   0        0        0     6932 2023-07-14 17:47:46.150966 connect_cli-27.7/connect/cli/plugins/translation/commands.py
--rw-r--r--   0        0        0      795 2023-07-14 17:47:46.150966 connect_cli-27.7/connect/cli/plugins/translation/constants.py
--rw-r--r--   0        0        0     1228 2023-07-14 17:47:46.150966 connect_cli-27.7/connect/cli/plugins/translation/export.py
--rw-r--r--   0        0        0      954 2023-07-14 17:47:46.150966 connect_cli-27.7/connect/cli/plugins/translation/primarize.py
--rw-r--r--   0        0        0     9152 2023-07-14 17:47:46.150966 connect_cli-27.7/connect/cli/plugins/translation/translation_sync.py
--rw-r--r--   0        0        0      818 2023-07-14 17:47:46.150966 connect_cli-27.7/connect/cli/plugins/translation/utils.py
--rw-r--r--   0        0        0     4086 2023-07-14 17:51:01.037980 connect_cli-27.7/pyproject.toml
--rw-r--r--   0        0        0     5060 1970-01-01 00:00:00.000000 connect_cli-27.7/PKG-INFO
+-rw-r--r--   0        0        0    11357 2023-07-21 16:49:35.986208 connect_cli-27.8/LICENSE
+-rw-r--r--   0        0        0     3280 2023-07-21 16:49:35.986208 connect_cli-27.8/README.md
+-rw-r--r--   0        0        0     1823 2023-07-21 16:53:07.374491 connect_cli-27.8/connect/.data/connect_reports/.github/workflows/build.yml
+-rw-r--r--   0        0        0      166 2023-07-21 16:53:07.374491 connect_cli-27.8/connect/.data/connect_reports/.gitignore
+-rw-r--r--   0        0        0    10756 2023-07-21 16:53:07.374491 connect_cli-27.8/connect/.data/connect_reports/LICENSE
+-rw-r--r--   0        0        0      708 2023-07-21 16:53:07.374491 connect_cli-27.8/connect/.data/connect_reports/README.md
+-rw-r--r--   0        0        0   122573 2023-07-21 16:53:07.374491 connect_cli-27.8/connect/.data/connect_reports/poetry.lock
+-rw-r--r--   0        0        0     1221 2023-07-21 16:53:07.374491 connect_cli-27.8/connect/.data/connect_reports/pyproject.toml
+-rw-r--r--   0        0        0        0 2023-07-21 16:53:07.374491 connect_cli-27.8/connect/.data/connect_reports/reports/__init__.py
+-rw-r--r--   0        0        0      215 2023-07-21 16:53:07.374491 connect_cli-27.8/connect/.data/connect_reports/reports/billing_requests/Readme.md
+-rw-r--r--   0        0        0        0 2023-07-21 16:53:07.374491 connect_cli-27.8/connect/.data/connect_reports/reports/billing_requests/__init__.py
+-rw-r--r--   0        0        0     3762 2023-07-21 16:53:07.374491 connect_cli-27.8/connect/.data/connect_reports/reports/billing_requests/entrypoint.py
+-rw-r--r--   0        0        0     9038 2023-07-21 16:53:07.374491 connect_cli-27.8/connect/.data/connect_reports/reports/billing_requests/templates/xlsx/template.xlsx
+-rw-r--r--   0        0        0      377 2023-07-21 16:53:07.374491 connect_cli-27.8/connect/.data/connect_reports/reports/billing_requests_line_item/Readme.md
+-rw-r--r--   0        0        0        0 2023-07-21 16:53:07.374491 connect_cli-27.8/connect/.data/connect_reports/reports/billing_requests_line_item/__init__.py
+-rw-r--r--   0        0        0     4313 2023-07-21 16:53:07.374491 connect_cli-27.8/connect/.data/connect_reports/reports/billing_requests_line_item/entrypoint.py
+-rw-r--r--   0        0        0     9214 2023-07-21 16:53:07.374491 connect_cli-27.8/connect/.data/connect_reports/reports/billing_requests_line_item/templates/xlsx/template.xlsx
+-rw-r--r--   0        0        0      151 2023-07-21 16:53:07.374491 connect_cli-27.8/connect/.data/connect_reports/reports/contract_list/Readme.md
+-rw-r--r--   0        0        0        0 2023-07-21 16:53:07.374491 connect_cli-27.8/connect/.data/connect_reports/reports/contract_list/__init__.py
+-rw-r--r--   0        0        0     3114 2023-07-21 16:53:07.374491 connect_cli-27.8/connect/.data/connect_reports/reports/contract_list/entrypoint.py
+-rw-r--r--   0        0        0     8883 2023-07-21 16:53:07.374491 connect_cli-27.8/connect/.data/connect_reports/reports/contract_list/templates/xlsx/template.xlsx
+-rw-r--r--   0        0        0      175 2023-07-21 16:53:07.374491 connect_cli-27.8/connect/.data/connect_reports/reports/customers_list/Readme.md
+-rw-r--r--   0        0        0        0 2023-07-21 16:53:07.374491 connect_cli-27.8/connect/.data/connect_reports/reports/customers_list/__init__.py
+-rw-r--r--   0        0        0     3595 2023-07-21 16:53:07.374491 connect_cli-27.8/connect/.data/connect_reports/reports/customers_list/entrypoint.py
+-rw-r--r--   0        0        0     8914 2023-07-21 16:53:07.374491 connect_cli-27.8/connect/.data/connect_reports/reports/customers_list/templates/xlsx/template.xlsx
+-rw-r--r--   0        0        0      546 2023-07-21 16:53:07.374491 connect_cli-27.8/connect/.data/connect_reports/reports/executive_fullfilment_requests/Readme.md
+-rw-r--r--   0        0        0        0 2023-07-21 16:53:07.374491 connect_cli-27.8/connect/.data/connect_reports/reports/executive_fullfilment_requests/__init__.py
+-rw-r--r--   0        0        0     6376 2023-07-21 16:53:07.374491 connect_cli-27.8/connect/.data/connect_reports/reports/executive_fullfilment_requests/constants.py
+-rw-r--r--   0        0        0    17465 2023-07-21 16:53:07.374491 connect_cli-27.8/connect/.data/connect_reports/reports/executive_fullfilment_requests/entrypoint.py
+-rw-r--r--   0        0        0     5254 2023-07-21 16:53:07.374491 connect_cli-27.8/connect/.data/connect_reports/reports/executive_fullfilment_requests/templates/pdf/img/ClouBlue-Logo.png
+-rw-r--r--   0        0        0     3180 2023-07-21 16:53:07.374491 connect_cli-27.8/connect/.data/connect_reports/reports/executive_fullfilment_requests/templates/pdf/template.css
+-rw-r--r--   0        0        0     1280 2023-07-21 16:53:07.374491 connect_cli-27.8/connect/.data/connect_reports/reports/executive_fullfilment_requests/templates/pdf/template.html.j2
+-rw-r--r--   0        0        0      240 2023-07-21 16:53:07.374491 connect_cli-27.8/connect/.data/connect_reports/reports/fulfillment_requests/Readme.md
+-rw-r--r--   0        0        0        0 2023-07-21 16:53:07.374491 connect_cli-27.8/connect/.data/connect_reports/reports/fulfillment_requests/__init__.py
+-rw-r--r--   0        0        0     4584 2023-07-21 16:53:07.374491 connect_cli-27.8/connect/.data/connect_reports/reports/fulfillment_requests/entrypoint.py
+-rw-r--r--   0        0        0     9160 2023-07-21 16:53:07.374491 connect_cli-27.8/connect/.data/connect_reports/reports/fulfillment_requests/templates/xlsx/template.xlsx
+-rw-r--r--   0        0        0      301 2023-07-21 16:53:07.378491 connect_cli-27.8/connect/.data/connect_reports/reports/fulfillment_requests_failed/Readme.md
+-rw-r--r--   0        0        0        0 2023-07-21 16:53:07.378491 connect_cli-27.8/connect/.data/connect_reports/reports/fulfillment_requests_failed/__init__.py
+-rw-r--r--   0        0        0     4064 2023-07-21 16:53:07.378491 connect_cli-27.8/connect/.data/connect_reports/reports/fulfillment_requests_failed/entrypoint.py
+-rw-r--r--   0        0        0     9050 2023-07-21 16:53:07.378491 connect_cli-27.8/connect/.data/connect_reports/reports/fulfillment_requests_failed/templates/xlsx/template.xlsx
+-rw-r--r--   0        0        0      328 2023-07-21 16:53:07.378491 connect_cli-27.8/connect/.data/connect_reports/reports/fulfillment_requests_line_item/Readme.md
+-rw-r--r--   0        0        0        0 2023-07-21 16:53:07.378491 connect_cli-27.8/connect/.data/connect_reports/reports/fulfillment_requests_line_item/__init__.py
+-rw-r--r--   0        0        0     4982 2023-07-21 16:53:07.378491 connect_cli-27.8/connect/.data/connect_reports/reports/fulfillment_requests_line_item/entrypoint.py
+-rw-r--r--   0        0        0     9234 2023-07-21 16:53:07.378491 connect_cli-27.8/connect/.data/connect_reports/reports/fulfillment_requests_line_item/templates/xlsx/template.xlsx
+-rw-r--r--   0        0        0      180 2023-07-21 16:53:07.378491 connect_cli-27.8/connect/.data/connect_reports/reports/helpdesk/Readme.md
+-rw-r--r--   0        0        0        0 2023-07-21 16:53:07.378491 connect_cli-27.8/connect/.data/connect_reports/reports/helpdesk/__init__.py
+-rw-r--r--   0        0        0     2635 2023-07-21 16:53:07.378491 connect_cli-27.8/connect/.data/connect_reports/reports/helpdesk/entrypoint.py
+-rw-r--r--   0        0        0     8749 2023-07-21 16:53:07.378491 connect_cli-27.8/connect/.data/connect_reports/reports/helpdesk/templates/xlsx/template.xlsx
+-rw-r--r--   0        0        0      186 2023-07-21 16:53:07.378491 connect_cli-27.8/connect/.data/connect_reports/reports/listing_list/Readme.md
+-rw-r--r--   0        0        0        0 2023-07-21 16:53:07.378491 connect_cli-27.8/connect/.data/connect_reports/reports/listing_list/__init__.py
+-rw-r--r--   0        0        0     2632 2023-07-21 16:53:07.378491 connect_cli-27.8/connect/.data/connect_reports/reports/listing_list/entrypoint.py
+-rw-r--r--   0        0        0     8703 2023-07-21 16:53:07.378491 connect_cli-27.8/connect/.data/connect_reports/reports/listing_list/templates/xlsx/template.xlsx
+-rw-r--r--   0        0        0      194 2023-07-21 16:53:07.378491 connect_cli-27.8/connect/.data/connect_reports/reports/listing_requests/Readme.md
+-rw-r--r--   0        0        0        0 2023-07-21 16:53:07.378491 connect_cli-27.8/connect/.data/connect_reports/reports/listing_requests/__init__.py
+-rw-r--r--   0        0        0     2870 2023-07-21 16:53:07.378491 connect_cli-27.8/connect/.data/connect_reports/reports/listing_requests/entrypoint.py
+-rw-r--r--   0        0        0     8746 2023-07-21 16:53:07.378491 connect_cli-27.8/connect/.data/connect_reports/reports/listing_requests/templates/xlsx/template.xlsx
+-rw-r--r--   0        0        0      117 2023-07-21 16:53:07.378491 connect_cli-27.8/connect/.data/connect_reports/reports/products_catalog/Readme.md
+-rw-r--r--   0        0        0        0 2023-07-21 16:53:07.378491 connect_cli-27.8/connect/.data/connect_reports/reports/products_catalog/__init__.py
+-rw-r--r--   0        0        0     2582 2023-07-21 16:53:07.378491 connect_cli-27.8/connect/.data/connect_reports/reports/products_catalog/entrypoint.py
+-rwxr-xr-x   0        0        0     7209 2023-07-21 16:53:07.378491 connect_cli-27.8/connect/.data/connect_reports/reports/products_catalog/templates/pdf/assets/cloudblue-connect-alone.png
+-rw-r--r--   0        0        0    33448 2023-07-21 16:53:07.378491 connect_cli-27.8/connect/.data/connect_reports/reports/products_catalog/templates/pdf/assets/cloudblue-logo.png
+-rw-r--r--   0        0        0    11287 2023-07-21 16:53:07.378491 connect_cli-27.8/connect/.data/connect_reports/reports/products_catalog/templates/pdf/assets/cloudblue-small-color-disabled.png
+-rw-r--r--   0        0        0     9404 2023-07-21 16:53:07.378491 connect_cli-27.8/connect/.data/connect_reports/reports/products_catalog/templates/pdf/assets/cloudblue-small-color-enabled.png
+-rw-r--r--   0        0        0    91722 2023-07-21 16:53:07.378491 connect_cli-27.8/connect/.data/connect_reports/reports/products_catalog/templates/pdf/assets/connect-logo.png
+-rw-r--r--   0        0        0   465078 2023-07-21 16:53:07.382491 connect_cli-27.8/connect/.data/connect_reports/reports/products_catalog/templates/pdf/assets/cover-bg.png
+-rw-r--r--   0        0        0    10941 2023-07-21 16:53:07.382491 connect_cli-27.8/connect/.data/connect_reports/reports/products_catalog/templates/pdf/assets/imc-small-color.png
+-rw-r--r--   0        0        0    16685 2023-07-21 16:53:07.382491 connect_cli-27.8/connect/.data/connect_reports/reports/products_catalog/templates/pdf/img/ClouBlue-Logo-Black.png
+-rw-r--r--   0        0        0     3555 2023-07-21 16:53:07.382491 connect_cli-27.8/connect/.data/connect_reports/reports/products_catalog/templates/pdf/img/ClouBlue-Logo-White.png
+-rw-r--r--   0        0        0     5254 2023-07-21 16:53:07.382491 connect_cli-27.8/connect/.data/connect_reports/reports/products_catalog/templates/pdf/img/ClouBlue-Logo.png
+-rw-r--r--   0        0        0     8250 2023-07-21 16:53:07.382491 connect_cli-27.8/connect/.data/connect_reports/reports/products_catalog/templates/pdf/img/accordo.png
+-rw-r--r--   0        0        0     1311 2023-07-21 16:53:07.382491 connect_cli-27.8/connect/.data/connect_reports/reports/products_catalog/templates/pdf/img/acronis-blue.png
+-rw-r--r--   0        0        0     1968 2023-07-21 16:53:07.382491 connect_cli-27.8/connect/.data/connect_reports/reports/products_catalog/templates/pdf/img/acronis-white.png
+-rw-r--r--   0        0        0   124929 2023-07-21 16:53:07.386491 connect_cli-27.8/connect/.data/connect_reports/reports/products_catalog/templates/pdf/img/adobe.jpeg
+-rw-r--r--   0        0        0    10421 2023-07-21 16:53:07.386491 connect_cli-27.8/connect/.data/connect_reports/reports/products_catalog/templates/pdf/img/airtame.png
+-rw-r--r--   0        0        0      876 2023-07-21 16:53:07.386491 connect_cli-27.8/connect/.data/connect_reports/reports/products_catalog/templates/pdf/img/allyhub.png
+-rw-r--r--   0        0        0     4615 2023-07-21 16:53:07.386491 connect_cli-27.8/connect/.data/connect_reports/reports/products_catalog/templates/pdf/img/alsid.png
+-rw-r--r--   0        0        0    12369 2023-07-21 16:53:07.386491 connect_cli-27.8/connect/.data/connect_reports/reports/products_catalog/templates/pdf/img/anchor.png
+-rw-r--r--   0        0        0     5200 2023-07-21 16:53:07.386491 connect_cli-27.8/connect/.data/connect_reports/reports/products_catalog/templates/pdf/img/australia.png
+-rw-r--r--   0        0        0     3371 2023-07-21 16:53:07.386491 connect_cli-27.8/connect/.data/connect_reports/reports/products_catalog/templates/pdf/img/austria.png
+-rw-r--r--   0        0        0    60306 2023-07-21 16:53:07.386491 connect_cli-27.8/connect/.data/connect_reports/reports/products_catalog/templates/pdf/img/aws.png
+-rw-r--r--   0        0        0     3030 2023-07-21 16:53:07.386491 connect_cli-27.8/connect/.data/connect_reports/reports/products_catalog/templates/pdf/img/belgium.png
+-rw-r--r--   0        0        0     5606 2023-07-21 16:53:07.386491 connect_cli-27.8/connect/.data/connect_reports/reports/products_catalog/templates/pdf/img/brazil.png
+-rw-r--r--   0        0        0     3693 2023-07-21 16:53:07.386491 connect_cli-27.8/connect/.data/connect_reports/reports/products_catalog/templates/pdf/img/canada.png
+-rw-r--r--   0        0        0     3870 2023-07-21 16:53:07.386491 connect_cli-27.8/connect/.data/connect_reports/reports/products_catalog/templates/pdf/img/chile.png
+-rw-r--r--   0        0        0     3086 2023-07-21 16:53:07.386491 connect_cli-27.8/connect/.data/connect_reports/reports/products_catalog/templates/pdf/img/colombia.png
+-rw-r--r--   0        0        0     3670 2023-07-21 16:53:07.386491 connect_cli-27.8/connect/.data/connect_reports/reports/products_catalog/templates/pdf/img/france.png
+-rw-r--r--   0        0        0     3212 2023-07-21 16:53:07.386491 connect_cli-27.8/connect/.data/connect_reports/reports/products_catalog/templates/pdf/img/germany.png
+-rw-r--r--   0        0        0     4521 2023-07-21 16:53:07.386491 connect_cli-27.8/connect/.data/connect_reports/reports/products_catalog/templates/pdf/img/hong-kong.png
+-rw-r--r--   0        0        0    12000 2023-07-21 16:53:07.386491 connect_cli-27.8/connect/.data/connect_reports/reports/products_catalog/templates/pdf/img/icon.png
+-rw-r--r--   0        0        0     4491 2023-07-21 16:53:07.386491 connect_cli-27.8/connect/.data/connect_reports/reports/products_catalog/templates/pdf/img/india.png
+-rw-r--r--   0        0        0     3622 2023-07-21 16:53:07.386491 connect_cli-27.8/connect/.data/connect_reports/reports/products_catalog/templates/pdf/img/italy.png
+-rw-r--r--   0        0        0     5096 2023-07-21 16:53:07.386491 connect_cli-27.8/connect/.data/connect_reports/reports/products_catalog/templates/pdf/img/malaysia.png
+-rw-r--r--   0        0        0     3897 2023-07-21 16:53:07.386491 connect_cli-27.8/connect/.data/connect_reports/reports/products_catalog/templates/pdf/img/mexico.png
+-rw-r--r--   0        0        0     3633 2023-07-21 16:53:07.386491 connect_cli-27.8/connect/.data/connect_reports/reports/products_catalog/templates/pdf/img/netherlands.png
+-rw-r--r--   0        0        0     5173 2023-07-21 16:53:07.386491 connect_cli-27.8/connect/.data/connect_reports/reports/products_catalog/templates/pdf/img/new-zealand.png
+-rw-r--r--   0        0        0     4163 2023-07-21 16:53:07.386491 connect_cli-27.8/connect/.data/connect_reports/reports/products_catalog/templates/pdf/img/singapore.png
+-rw-r--r--   0        0        0     4670 2023-07-21 16:53:07.386491 connect_cli-27.8/connect/.data/connect_reports/reports/products_catalog/templates/pdf/img/spain.png
+-rw-r--r--   0        0        0     4802 2023-07-21 16:53:07.386491 connect_cli-27.8/connect/.data/connect_reports/reports/products_catalog/templates/pdf/img/sweden.png
+-rw-r--r--   0        0        0     3622 2023-07-21 16:53:07.386491 connect_cli-27.8/connect/.data/connect_reports/reports/products_catalog/templates/pdf/img/switzerland.png
+-rw-r--r--   0        0        0     4073 2023-07-21 16:53:07.386491 connect_cli-27.8/connect/.data/connect_reports/reports/products_catalog/templates/pdf/img/turkey.png
+-rw-r--r--   0        0        0     3350 2023-07-21 16:53:07.386491 connect_cli-27.8/connect/.data/connect_reports/reports/products_catalog/templates/pdf/img/uae.png
+-rw-r--r--   0        0        0     5583 2023-07-21 16:53:07.386491 connect_cli-27.8/connect/.data/connect_reports/reports/products_catalog/templates/pdf/img/uk.png
+-rw-r--r--   0        0        0     4892 2023-07-21 16:53:07.386491 connect_cli-27.8/connect/.data/connect_reports/reports/products_catalog/templates/pdf/img/usa.png
+-rw-r--r--   0        0        0     4063 2023-07-21 16:53:07.386491 connect_cli-27.8/connect/.data/connect_reports/reports/products_catalog/templates/pdf/template.css
+-rw-r--r--   0        0        0     1736 2023-07-21 16:53:07.386491 connect_cli-27.8/connect/.data/connect_reports/reports/products_catalog/templates/pdf/template.html.j2
+-rw-r--r--   0        0        0      592 2023-07-21 16:53:07.386491 connect_cli-27.8/connect/.data/connect_reports/reports/sla/Readme.md
+-rw-r--r--   0        0        0        0 2023-07-21 16:53:07.386491 connect_cli-27.8/connect/.data/connect_reports/reports/sla/__init__.py
+-rw-r--r--   0        0        0     4125 2023-07-21 16:53:07.386491 connect_cli-27.8/connect/.data/connect_reports/reports/sla/entrypoint.py
+-rw-r--r--   0        0        0     9679 2023-07-21 16:53:07.386491 connect_cli-27.8/connect/.data/connect_reports/reports/sla/templates/xlsx/template.xlsx
+-rw-r--r--   0        0        0      260 2023-07-21 16:53:07.386491 connect_cli-27.8/connect/.data/connect_reports/reports/subscription_list/Readme.md
+-rw-r--r--   0        0        0        0 2023-07-21 16:53:07.386491 connect_cli-27.8/connect/.data/connect_reports/reports/subscription_list/__init__.py
+-rw-r--r--   0        0        0     6276 2023-07-21 16:53:07.386491 connect_cli-27.8/connect/.data/connect_reports/reports/subscription_list/entrypoint.py
+-rw-r--r--   0        0        0     9302 2023-07-21 16:53:07.386491 connect_cli-27.8/connect/.data/connect_reports/reports/subscription_list/templates/xlsx/template.xlsx
+-rw-r--r--   0        0        0      203 2023-07-21 16:53:07.386491 connect_cli-27.8/connect/.data/connect_reports/reports/tier_configuration_list/Readme.md
+-rw-r--r--   0        0        0        0 2023-07-21 16:53:07.386491 connect_cli-27.8/connect/.data/connect_reports/reports/tier_configuration_list/__init__.py
+-rw-r--r--   0        0        0     4282 2023-07-21 16:53:07.386491 connect_cli-27.8/connect/.data/connect_reports/reports/tier_configuration_list/entrypoint.py
+-rw-r--r--   0        0        0     8925 2023-07-21 16:53:07.386491 connect_cli-27.8/connect/.data/connect_reports/reports/tier_configuration_list/templates/xlsx/template.xlsx
+-rw-r--r--   0        0        0      228 2023-07-21 16:53:07.386491 connect_cli-27.8/connect/.data/connect_reports/reports/tier_configuration_requests/Readme.md
+-rw-r--r--   0        0        0        0 2023-07-21 16:53:07.386491 connect_cli-27.8/connect/.data/connect_reports/reports/tier_configuration_requests/__init__.py
+-rw-r--r--   0        0        0     5147 2023-07-21 16:53:07.386491 connect_cli-27.8/connect/.data/connect_reports/reports/tier_configuration_requests/entrypoint.py
+-rw-r--r--   0        0        0     9070 2023-07-21 16:53:07.386491 connect_cli-27.8/connect/.data/connect_reports/reports/tier_configuration_requests/templates/xlsx/template.xlsx
+-rw-r--r--   0        0        0      431 2023-07-21 16:53:07.386491 connect_cli-27.8/connect/.data/connect_reports/reports/usage_in_subscription/Readme.md
+-rw-r--r--   0        0        0        0 2023-07-21 16:53:07.386491 connect_cli-27.8/connect/.data/connect_reports/reports/usage_in_subscription/__init__.py
+-rw-r--r--   0        0        0     4106 2023-07-21 16:53:07.386491 connect_cli-27.8/connect/.data/connect_reports/reports/usage_in_subscription/entrypoint.py
+-rw-r--r--   0        0        0     9137 2023-07-21 16:53:07.386491 connect_cli-27.8/connect/.data/connect_reports/reports/usage_in_subscription/templates/xlsx/template.xlsx
+-rw-r--r--   0        0        0     1318 2023-07-21 16:53:07.386491 connect_cli-27.8/connect/.data/connect_reports/reports/utils.py
+-rw-r--r--   0        0        0    37904 2023-07-21 16:53:07.374491 connect_cli-27.8/connect/.data/connect_reports/reports.json
+-rw-r--r--   0        0        0      245 2023-07-21 16:53:07.386491 connect_cli-27.8/connect/.data/connect_reports/sonar-project.properties
+-rw-r--r--   0        0        0      321 2023-07-21 16:53:07.390491 connect_cli-27.8/connect/.data/connect_reports/tox.ini
+-rw-r--r--   0        0        0      352 2023-07-21 16:49:35.986208 connect_cli-27.8/connect/cli/__init__.py
+-rw-r--r--   0        0        0     1763 2023-07-21 16:49:35.986208 connect_cli-27.8/connect/cli/ccli.py
+-rw-r--r--   0        0        0       54 2023-07-21 16:49:35.986208 connect_cli-27.8/connect/cli/core/__init__.py
+-rw-r--r--   0        0        0        0 2023-07-21 16:49:35.986208 connect_cli-27.8/connect/cli/core/account/__init__.py
+-rw-r--r--   0        0        0     2433 2023-07-21 16:49:35.986208 connect_cli-27.8/connect/cli/core/account/commands.py
+-rw-r--r--   0        0        0     1233 2023-07-21 16:49:35.986208 connect_cli-27.8/connect/cli/core/account/helpers.py
+-rw-r--r--   0        0        0     2764 2023-07-21 16:49:35.986208 connect_cli-27.8/connect/cli/core/base.py
+-rw-r--r--   0        0        0     4048 2023-07-21 16:49:35.986208 connect_cli-27.8/connect/cli/core/config.py
+-rw-r--r--   0        0        0      573 2023-07-21 16:49:35.986208 connect_cli-27.8/connect/cli/core/constants.py
+-rw-r--r--   0        0        0     1424 2023-07-21 16:49:35.986208 connect_cli-27.8/connect/cli/core/http.py
+-rw-r--r--   0        0        0      838 2023-07-21 16:49:35.986208 connect_cli-27.8/connect/cli/core/plugins.py
+-rw-r--r--   0        0        0     6836 2023-07-21 16:49:35.986208 connect_cli-27.8/connect/cli/core/terminal.py
+-rw-r--r--   0        0        0     3139 2023-07-21 16:49:35.986208 connect_cli-27.8/connect/cli/core/utils.py
+-rw-r--r--   0        0        0        0 2023-07-21 16:49:35.986208 connect_cli-27.8/connect/cli/plugins/__init__.py
+-rw-r--r--   0        0        0        0 2023-07-21 16:49:35.986208 connect_cli-27.8/connect/cli/plugins/customer/__init__.py
+-rw-r--r--   0        0        0     2137 2023-07-21 16:49:35.986208 connect_cli-27.8/connect/cli/plugins/customer/commands.py
+-rw-r--r--   0        0        0      526 2023-07-21 16:49:35.986208 connect_cli-27.8/connect/cli/plugins/customer/constants.py
+-rw-r--r--   0        0        0     6040 2023-07-21 16:49:35.986208 connect_cli-27.8/connect/cli/plugins/customer/export.py
+-rw-r--r--   0        0        0    12696 2023-07-21 16:49:35.986208 connect_cli-27.8/connect/cli/plugins/customer/sync.py
+-rw-r--r--   0        0        0        0 2023-07-21 16:49:35.986208 connect_cli-27.8/connect/cli/plugins/locale/__init__.py
+-rw-r--r--   0        0        0     1363 2023-07-21 16:49:35.986208 connect_cli-27.8/connect/cli/plugins/locale/commands.py
+-rw-r--r--   0        0        0      306 2023-07-21 16:49:35.986208 connect_cli-27.8/connect/cli/plugins/play/__init__.py
+-rw-r--r--   0        0        0     2485 2023-07-21 16:49:35.986208 connect_cli-27.8/connect/cli/plugins/play/commands.py
+-rw-r--r--   0        0        0     2395 2023-07-21 16:49:35.986208 connect_cli-27.8/connect/cli/plugins/play/context.py
+-rw-r--r--   0        0        0      428 2023-07-21 16:49:35.986208 connect_cli-27.8/connect/cli/plugins/play/save.py
+-rw-r--r--   0        0        0     1647 2023-07-21 16:49:35.986208 connect_cli-27.8/connect/cli/plugins/play/script.py
+-rw-r--r--   0        0        0        0 2023-07-21 16:49:35.986208 connect_cli-27.8/connect/cli/plugins/product/__init__.py
+-rw-r--r--   0        0        0     1575 2023-07-21 16:49:35.986208 connect_cli-27.8/connect/cli/plugins/product/api.py
+-rw-r--r--   0        0        0     8628 2023-07-21 16:49:35.986208 connect_cli-27.8/connect/cli/plugins/product/clone.py
+-rw-r--r--   0        0        0     9659 2023-07-21 16:49:35.986208 connect_cli-27.8/connect/cli/plugins/product/commands.py
+-rw-r--r--   0        0        0     1289 2023-07-21 16:49:35.986208 connect_cli-27.8/connect/cli/plugins/product/constants.py
+-rw-r--r--   0        0        0    33457 2023-07-21 16:49:35.990208 connect_cli-27.8/connect/cli/plugins/product/export.py
+-rw-r--r--   0        0        0      846 2023-07-21 16:49:35.990208 connect_cli-27.8/connect/cli/plugins/product/sync/__init__.py
+-rw-r--r--   0        0        0     5932 2023-07-21 16:49:35.990208 connect_cli-27.8/connect/cli/plugins/product/sync/actions.py
+-rw-r--r--   0        0        0     8988 2023-07-21 16:49:35.990208 connect_cli-27.8/connect/cli/plugins/product/sync/capabilities.py
+-rw-r--r--   0        0        0     3881 2023-07-21 16:49:35.990208 connect_cli-27.8/connect/cli/plugins/product/sync/configuration_values.py
+-rw-r--r--   0        0        0     5096 2023-07-21 16:49:35.990208 connect_cli-27.8/connect/cli/plugins/product/sync/general.py
+-rw-r--r--   0        0        0    11768 2023-07-21 16:49:35.990208 connect_cli-27.8/connect/cli/plugins/product/sync/items.py
+-rw-r--r--   0        0        0     5846 2023-07-21 16:49:35.990208 connect_cli-27.8/connect/cli/plugins/product/sync/media.py
+-rw-r--r--   0        0        0     9460 2023-07-21 16:49:35.990208 connect_cli-27.8/connect/cli/plugins/product/sync/params.py
+-rw-r--r--   0        0        0     3598 2023-07-21 16:49:35.990208 connect_cli-27.8/connect/cli/plugins/product/sync/static_resources.py
+-rw-r--r--   0        0        0     5303 2023-07-21 16:49:35.990208 connect_cli-27.8/connect/cli/plugins/product/sync/templates.py
+-rw-r--r--   0        0        0      985 2023-07-21 16:49:35.990208 connect_cli-27.8/connect/cli/plugins/product/utils.py
+-rw-r--r--   0        0        0        0 2023-07-21 16:49:35.990208 connect_cli-27.8/connect/cli/plugins/project/__init__.py
+-rw-r--r--   0        0        0     5791 2023-07-21 16:49:35.990208 connect_cli-27.8/connect/cli/plugins/project/commands.py
+-rw-r--r--   0        0        0        0 2023-07-21 16:49:35.990208 connect_cli-27.8/connect/cli/plugins/project/extension/__init__.py
+-rw-r--r--   0        0        0      411 2023-07-21 16:49:35.990208 connect_cli-27.8/connect/cli/plugins/project/extension/constants.py
+-rw-r--r--   0        0        0    10802 2023-07-21 16:49:35.990208 connect_cli-27.8/connect/cli/plugins/project/extension/helpers.py
+-rw-r--r--   0        0        0      103 2023-07-21 16:49:35.990208 connect_cli-27.8/connect/cli/plugins/project/extension/templates/bootstrap/${project_slug}/${package_name}/__init__.py.j2
+-rw-r--r--   0        0        0      852 2023-07-21 16:49:35.990208 connect_cli-27.8/connect/cli/plugins/project/extension/templates/bootstrap/${project_slug}/${package_name}/anvil.py.j2
+-rw-r--r--   0        0        0     2920 2023-07-21 16:49:35.990208 connect_cli-27.8/connect/cli/plugins/project/extension/templates/bootstrap/${project_slug}/${package_name}/events.py.j2
+-rw-r--r--   0        0        0      464 2023-07-21 16:49:35.990208 connect_cli-27.8/connect/cli/plugins/project/extension/templates/bootstrap/${project_slug}/${package_name}/extension.json.j2
+-rw-r--r--   0        0        0      560 2023-07-21 16:49:35.990208 connect_cli-27.8/connect/cli/plugins/project/extension/templates/bootstrap/${project_slug}/${package_name}/schemas.py.j2
+-rw-r--r--   0        0        0        0 2023-07-21 16:49:35.990208 connect_cli-27.8/connect/cli/plugins/project/extension/templates/bootstrap/${project_slug}/${package_name}/static/.gitkeep.j2
+-rw-r--r--   0        0        0     1762 2023-07-21 16:49:35.990208 connect_cli-27.8/connect/cli/plugins/project/extension/templates/bootstrap/${project_slug}/${package_name}/tfnapp.py.j2
+-rw-r--r--   0        0        0     7295 2023-07-21 16:49:35.990208 connect_cli-27.8/connect/cli/plugins/project/extension/templates/bootstrap/${project_slug}/${package_name}/webapp.py.j2
+-rw-r--r--   0        0        0      702 2023-07-21 16:49:35.990208 connect_cli-27.8/connect/cli/plugins/project/extension/templates/bootstrap/${project_slug}/.${project_slug}_dev.env.j2
+-rw-r--r--   0        0        0     1083 2023-07-21 16:49:35.990208 connect_cli-27.8/connect/cli/plugins/project/extension/templates/bootstrap/${project_slug}/.eslintrc.yaml.j2
+-rw-r--r--   0        0        0      231 2023-07-21 16:49:35.990208 connect_cli-27.8/connect/cli/plugins/project/extension/templates/bootstrap/${project_slug}/.flake8.j2
+-rw-r--r--   0        0        0     1309 2023-07-21 16:49:35.990208 connect_cli-27.8/connect/cli/plugins/project/extension/templates/bootstrap/${project_slug}/.github/workflows/test.yml.j2
+-rw-r--r--   0        0        0       96 2023-07-21 16:49:35.990208 connect_cli-27.8/connect/cli/plugins/project/extension/templates/bootstrap/${project_slug}/.gitignore.j2
+-rw-r--r--   0        0        0       63 2023-07-21 16:49:35.990208 connect_cli-27.8/connect/cli/plugins/project/extension/templates/bootstrap/${project_slug}/CHANGELOG.md.j2
+-rw-r--r--   0        0        0      249 2023-07-21 16:49:35.990208 connect_cli-27.8/connect/cli/plugins/project/extension/templates/bootstrap/${project_slug}/Dockerfile.j2
+-rw-r--r--   0        0        0     1661 2023-07-21 16:49:35.990208 connect_cli-27.8/connect/cli/plugins/project/extension/templates/bootstrap/${project_slug}/HOWTO.md.j2
+-rw-r--r--   0        0        0    14063 2023-07-21 16:49:35.990208 connect_cli-27.8/connect/cli/plugins/project/extension/templates/bootstrap/${project_slug}/LICENSE.j2
+-rw-r--r--   0        0        0      195 2023-07-21 16:49:35.990208 connect_cli-27.8/connect/cli/plugins/project/extension/templates/bootstrap/${project_slug}/README.md.j2
+-rw-r--r--   0        0        0      111 2023-07-21 16:49:35.990208 connect_cli-27.8/connect/cli/plugins/project/extension/templates/bootstrap/${project_slug}/__mocks__/fileMock.js.j2
+-rw-r--r--   0        0        0       97 2023-07-21 16:49:35.990208 connect_cli-27.8/connect/cli/plugins/project/extension/templates/bootstrap/${project_slug}/__mocks__/styleMock.js.j2
+-rw-r--r--   0        0        0       39 2023-07-21 16:49:35.990208 connect_cli-27.8/connect/cli/plugins/project/extension/templates/bootstrap/${project_slug}/babel.config.json.j2
+-rw-r--r--   0        0        0     1162 2023-07-21 16:49:35.990208 connect_cli-27.8/connect/cli/plugins/project/extension/templates/bootstrap/${project_slug}/docker-compose.yml.j2
+-rw-r--r--   0        0        0      944 2023-07-21 16:49:35.990208 connect_cli-27.8/connect/cli/plugins/project/extension/templates/bootstrap/${project_slug}/jest.config.js.j2
+-rw-r--r--   0        0        0     1246 2023-07-21 16:49:35.990208 connect_cli-27.8/connect/cli/plugins/project/extension/templates/bootstrap/${project_slug}/package.json.j2
+-rw-r--r--   0        0        0       29 2023-07-21 16:49:35.990208 connect_cli-27.8/connect/cli/plugins/project/extension/templates/bootstrap/${project_slug}/poetry.toml.j2
+-rw-r--r--   0        0        0     1960 2023-07-21 16:49:35.990208 connect_cli-27.8/connect/cli/plugins/project/extension/templates/bootstrap/${project_slug}/pyproject.toml.j2
+-rw-r--r--   0        0        0      103 2023-07-21 16:49:35.990208 connect_cli-27.8/connect/cli/plugins/project/extension/templates/bootstrap/${project_slug}/tests/__init__.py.j2
+-rw-r--r--   0        0        0      559 2023-07-21 16:49:35.990208 connect_cli-27.8/connect/cli/plugins/project/extension/templates/bootstrap/${project_slug}/tests/conftest.py.j2
+-rw-r--r--   0        0        0      553 2023-07-21 16:49:35.990208 connect_cli-27.8/connect/cli/plugins/project/extension/templates/bootstrap/${project_slug}/tests/test_anvil.py.j2
+-rw-r--r--   0        0        0     2602 2023-07-21 16:49:35.990208 connect_cli-27.8/connect/cli/plugins/project/extension/templates/bootstrap/${project_slug}/tests/test_events.py.j2
+-rw-r--r--   0        0        0     1183 2023-07-21 16:49:35.990208 connect_cli-27.8/connect/cli/plugins/project/extension/templates/bootstrap/${project_slug}/tests/test_tfnapp.py.j2
+-rw-r--r--   0        0        0     8794 2023-07-21 16:49:35.990208 connect_cli-27.8/connect/cli/plugins/project/extension/templates/bootstrap/${project_slug}/tests/test_webapp.py.j2
+-rw-r--r--   0        0        0      947 2023-07-21 16:49:35.990208 connect_cli-27.8/connect/cli/plugins/project/extension/templates/bootstrap/${project_slug}/ui/images/mkp.svg.j2
+-rw-r--r--   0        0        0      729 2023-07-21 16:49:35.990208 connect_cli-27.8/connect/cli/plugins/project/extension/templates/bootstrap/${project_slug}/ui/pages/index.html.j2
+-rw-r--r--   0        0        0      928 2023-07-21 16:49:35.990208 connect_cli-27.8/connect/cli/plugins/project/extension/templates/bootstrap/${project_slug}/ui/pages/settings.html.j2
+-rw-r--r--   0        0        0      470 2023-07-21 16:49:35.990208 connect_cli-27.8/connect/cli/plugins/project/extension/templates/bootstrap/${project_slug}/ui/pages/transformations/copy.html.j2
+-rw-r--r--   0        0        0     1590 2023-07-21 16:49:35.994208 connect_cli-27.8/connect/cli/plugins/project/extension/templates/bootstrap/${project_slug}/ui/pages/transformations/manual.html.j2
+-rw-r--r--   0        0        0     2609 2023-07-21 16:49:35.994208 connect_cli-27.8/connect/cli/plugins/project/extension/templates/bootstrap/${project_slug}/ui/src/components.js.j2
+-rw-r--r--   0        0        0      323 2023-07-21 16:49:35.994208 connect_cli-27.8/connect/cli/plugins/project/extension/templates/bootstrap/${project_slug}/ui/src/pages/index.js.j2
+-rw-r--r--   0        0        0      320 2023-07-21 16:49:35.994208 connect_cli-27.8/connect/cli/plugins/project/extension/templates/bootstrap/${project_slug}/ui/src/pages/settings.js.j2
+-rw-r--r--   0        0        0      267 2023-07-21 16:49:35.994208 connect_cli-27.8/connect/cli/plugins/project/extension/templates/bootstrap/${project_slug}/ui/src/pages/transformations/copy.js.j2
+-rw-r--r--   0        0        0      308 2023-07-21 16:49:35.994208 connect_cli-27.8/connect/cli/plugins/project/extension/templates/bootstrap/${project_slug}/ui/src/pages/transformations/manual.js.j2
+-rw-r--r--   0        0        0    10273 2023-07-21 16:49:35.994208 connect_cli-27.8/connect/cli/plugins/project/extension/templates/bootstrap/${project_slug}/ui/src/pages.js.j2
+-rw-r--r--   0        0        0     1579 2023-07-21 16:49:35.994208 connect_cli-27.8/connect/cli/plugins/project/extension/templates/bootstrap/${project_slug}/ui/src/utils.js.j2
+-rw-r--r--   0        0        0     6381 2023-07-21 16:49:35.994208 connect_cli-27.8/connect/cli/plugins/project/extension/templates/bootstrap/${project_slug}/ui/styles/index.css.j2
+-rw-r--r--   0        0        0      693 2023-07-21 16:49:35.994208 connect_cli-27.8/connect/cli/plugins/project/extension/templates/bootstrap/${project_slug}/ui/styles/manual.css.j2
+-rw-r--r--   0        0        0     6508 2023-07-21 16:49:35.994208 connect_cli-27.8/connect/cli/plugins/project/extension/templates/bootstrap/${project_slug}/ui/tests/components.spec.js.j2
+-rw-r--r--   0        0        0     9181 2023-07-21 16:49:35.994208 connect_cli-27.8/connect/cli/plugins/project/extension/templates/bootstrap/${project_slug}/ui/tests/pages.spec.js.j2
+-rw-r--r--   0        0        0     4352 2023-07-21 16:49:35.994208 connect_cli-27.8/connect/cli/plugins/project/extension/templates/bootstrap/${project_slug}/ui/tests/utils.spec.js.j2
+-rw-r--r--   0        0        0     2512 2023-07-21 16:49:35.994208 connect_cli-27.8/connect/cli/plugins/project/extension/templates/bootstrap/${project_slug}/webpack.config.js.j2
+-rw-r--r--   0        0        0     4487 2023-07-21 16:49:35.994208 connect_cli-27.8/connect/cli/plugins/project/extension/utils.py
+-rw-r--r--   0        0        0      805 2023-07-21 16:49:35.994208 connect_cli-27.8/connect/cli/plugins/project/extension/validators.py
+-rw-r--r--   0        0        0    12083 2023-07-21 16:49:35.994208 connect_cli-27.8/connect/cli/plugins/project/extension/wizard.py
+-rw-r--r--   0        0        0     5929 2023-07-21 16:49:35.994208 connect_cli-27.8/connect/cli/plugins/project/renderer.py
+-rw-r--r--   0        0        0        0 2023-07-21 16:49:35.994208 connect_cli-27.8/connect/cli/plugins/project/report/__init__.py
+-rw-r--r--   0        0        0     8611 2023-07-21 16:49:35.994208 connect_cli-27.8/connect/cli/plugins/project/report/helpers.py
+-rw-r--r--   0        0        0       73 2023-07-21 16:49:35.994208 connect_cli-27.8/connect/cli/plugins/project/report/templates/add/${initial_report_slug}/README.md.j2
+-rw-r--r--   0        0        0        0 2023-07-21 16:49:35.994208 connect_cli-27.8/connect/cli/plugins/project/report/templates/add/${initial_report_slug}/__init__.py.j2
+-rw-r--r--   0        0        0     1507 2023-07-21 16:49:35.994208 connect_cli-27.8/connect/cli/plugins/project/report/templates/add/${initial_report_slug}/entrypoint.py.j2
+-rw-r--r--   0        0        0        0 2023-07-21 16:49:35.994208 connect_cli-27.8/connect/cli/plugins/project/report/templates/add/${initial_report_slug}/templates/pdf/template.css.j2
+-rw-r--r--   0        0        0      499 2023-07-21 16:49:35.994208 connect_cli-27.8/connect/cli/plugins/project/report/templates/add/${initial_report_slug}/templates/pdf/template.html.j2.j2
+-rw-r--r--   0        0        0      150 2023-07-21 16:49:35.994208 connect_cli-27.8/connect/cli/plugins/project/report/templates/add/${initial_report_slug}/templates/xml/template.xml.j2.j2
+-rw-r--r--   0        0        0       69 2023-07-21 16:49:35.994208 connect_cli-27.8/connect/cli/plugins/project/report/templates/bootstrap/${project_slug}/${package_name}/${initial_report_slug}/README.md.j2
+-rw-r--r--   0        0        0        0 2023-07-21 16:49:35.994208 connect_cli-27.8/connect/cli/plugins/project/report/templates/bootstrap/${project_slug}/${package_name}/${initial_report_slug}/__init__.py.j2
+-rw-r--r--   0        0        0     1507 2023-07-21 16:49:35.994208 connect_cli-27.8/connect/cli/plugins/project/report/templates/bootstrap/${project_slug}/${package_name}/${initial_report_slug}/entrypoint.py.j2
+-rw-r--r--   0        0        0        0 2023-07-21 16:49:35.994208 connect_cli-27.8/connect/cli/plugins/project/report/templates/bootstrap/${project_slug}/${package_name}/${initial_report_slug}/templates/pdf/template.css.j2
+-rw-r--r--   0        0        0      518 2023-07-21 16:49:35.994208 connect_cli-27.8/connect/cli/plugins/project/report/templates/bootstrap/${project_slug}/${package_name}/${initial_report_slug}/templates/pdf/template.html.j2.j2
+-rw-r--r--   0        0        0      150 2023-07-21 16:49:35.994208 connect_cli-27.8/connect/cli/plugins/project/report/templates/bootstrap/${project_slug}/${package_name}/${initial_report_slug}/templates/xml/template.xml.j2.j2
+-rw-r--r--   0        0        0      271 2023-07-21 16:49:35.994208 connect_cli-27.8/connect/cli/plugins/project/report/templates/bootstrap/${project_slug}/.flake8.j2
+-rw-r--r--   0        0        0      803 2023-07-21 16:49:35.994208 connect_cli-27.8/connect/cli/plugins/project/report/templates/bootstrap/${project_slug}/.github/workflows/build.yml.j2
+-rw-r--r--   0        0        0       37 2023-07-21 16:49:35.994208 connect_cli-27.8/connect/cli/plugins/project/report/templates/bootstrap/${project_slug}/.gitignore.j2
+-rw-r--r--   0        0        0      458 2023-07-21 16:49:35.994208 connect_cli-27.8/connect/cli/plugins/project/report/templates/bootstrap/${project_slug}/HOWTO.md.j2
+-rw-r--r--   0        0        0    14063 2023-07-21 16:49:35.994208 connect_cli-27.8/connect/cli/plugins/project/report/templates/bootstrap/${project_slug}/LICENSE.j2
+-rw-r--r--   0        0        0      138 2023-07-21 16:49:35.994208 connect_cli-27.8/connect/cli/plugins/project/report/templates/bootstrap/${project_slug}/README.md.j2
+-rw-r--r--   0        0        0       29 2023-07-21 16:49:35.994208 connect_cli-27.8/connect/cli/plugins/project/report/templates/bootstrap/${project_slug}/poetry.toml.j2
+-rw-r--r--   0        0        0     1352 2023-07-21 16:49:35.994208 connect_cli-27.8/connect/cli/plugins/project/report/templates/bootstrap/${project_slug}/pyproject.toml.j2
+-rw-r--r--   0        0        0     2589 2023-07-21 16:49:35.994208 connect_cli-27.8/connect/cli/plugins/project/report/templates/bootstrap/${project_slug}/reports.json.j2
+-rw-r--r--   0        0        0      103 2023-07-21 16:49:35.994208 connect_cli-27.8/connect/cli/plugins/project/report/templates/bootstrap/${project_slug}/tests/__init__.py.j2
+-rw-r--r--   0        0        0     6397 2023-07-21 16:49:35.994208 connect_cli-27.8/connect/cli/plugins/project/report/templates/bootstrap/${project_slug}/tests/conftest.py.j2
+-rw-r--r--   0        0        0     2534 2023-07-21 16:49:35.994208 connect_cli-27.8/connect/cli/plugins/project/report/templates/bootstrap/${project_slug}/tests/test_${project_slug}.py.j2
+-rw-r--r--   0        0        0     5877 2023-07-21 16:49:35.994208 connect_cli-27.8/connect/cli/plugins/project/report/validations.py
+-rw-r--r--   0        0        0     8615 2023-07-21 16:49:35.994208 connect_cli-27.8/connect/cli/plugins/project/report/wizard.py
+-rw-r--r--   0        0        0     1443 2023-07-21 16:49:35.994208 connect_cli-27.8/connect/cli/plugins/project/utils.py
+-rw-r--r--   0        0        0     2798 2023-07-21 16:49:35.994208 connect_cli-27.8/connect/cli/plugins/project/validators.py
+-rw-r--r--   0        0        0        0 2023-07-21 16:49:35.994208 connect_cli-27.8/connect/cli/plugins/report/__init__.py
+-rw-r--r--   0        0        0     2405 2023-07-21 16:49:35.994208 connect_cli-27.8/connect/cli/plugins/report/commands.py
+-rw-r--r--   0        0        0       86 2023-07-21 16:49:35.994208 connect_cli-27.8/connect/cli/plugins/report/constants.py
+-rw-r--r--   0        0        0     6210 2023-07-21 16:49:35.998208 connect_cli-27.8/connect/cli/plugins/report/helpers.py
+-rw-r--r--   0        0        0     2822 2023-07-21 16:49:35.998208 connect_cli-27.8/connect/cli/plugins/report/utils.py
+-rw-r--r--   0        0        0     8345 2023-07-21 16:49:35.998208 connect_cli-27.8/connect/cli/plugins/report/wizard.py
+-rw-r--r--   0        0        0        0 2023-07-21 16:49:35.998208 connect_cli-27.8/connect/cli/plugins/shared/__init__.py
+-rw-r--r--   0        0        0     2441 2023-07-21 16:49:35.998208 connect_cli-27.8/connect/cli/plugins/shared/base.py
+-rw-r--r--   0        0        0     1973 2023-07-21 16:49:35.998208 connect_cli-27.8/connect/cli/plugins/shared/constants.py
+-rw-r--r--   0        0        0       46 2023-07-21 16:49:35.998208 connect_cli-27.8/connect/cli/plugins/shared/exceptions.py
+-rw-r--r--   0        0        0     2375 2023-07-21 16:49:35.998208 connect_cli-27.8/connect/cli/plugins/shared/export.py
+-rw-r--r--   0        0        0     6295 2023-07-21 16:49:35.998208 connect_cli-27.8/connect/cli/plugins/shared/sync_stats.py
+-rw-r--r--   0        0        0     5739 2023-07-21 16:49:35.998208 connect_cli-27.8/connect/cli/plugins/shared/translation_attr_sync.py
+-rw-r--r--   0        0        0     6534 2023-07-21 16:49:35.998208 connect_cli-27.8/connect/cli/plugins/shared/translation_sync.py
+-rw-r--r--   0        0        0     2103 2023-07-21 16:49:35.998208 connect_cli-27.8/connect/cli/plugins/shared/translations_synchronizers.py
+-rw-r--r--   0        0        0     6793 2023-07-21 16:49:35.998208 connect_cli-27.8/connect/cli/plugins/shared/utils.py
+-rw-r--r--   0        0        0        0 2023-07-21 16:49:35.998208 connect_cli-27.8/connect/cli/plugins/translation/__init__.py
+-rw-r--r--   0        0        0      707 2023-07-21 16:49:35.998208 connect_cli-27.8/connect/cli/plugins/translation/activate.py
+-rw-r--r--   0        0        0     6932 2023-07-21 16:49:35.998208 connect_cli-27.8/connect/cli/plugins/translation/commands.py
+-rw-r--r--   0        0        0      795 2023-07-21 16:49:35.998208 connect_cli-27.8/connect/cli/plugins/translation/constants.py
+-rw-r--r--   0        0        0     1228 2023-07-21 16:49:35.998208 connect_cli-27.8/connect/cli/plugins/translation/export.py
+-rw-r--r--   0        0        0      954 2023-07-21 16:49:35.998208 connect_cli-27.8/connect/cli/plugins/translation/primarize.py
+-rw-r--r--   0        0        0     9152 2023-07-21 16:49:35.998208 connect_cli-27.8/connect/cli/plugins/translation/translation_sync.py
+-rw-r--r--   0        0        0      818 2023-07-21 16:49:35.998208 connect_cli-27.8/connect/cli/plugins/translation/utils.py
+-rw-r--r--   0        0        0     4086 2023-07-21 16:53:08.366493 connect_cli-27.8/pyproject.toml
+-rw-r--r--   0        0        0     5060 1970-01-01 00:00:00.000000 connect_cli-27.8/PKG-INFO
```

### Comparing `connect_cli-27.7/LICENSE` & `connect_cli-27.8/LICENSE`

 * *Files identical despite different names*

### Comparing `connect_cli-27.7/README.md` & `connect_cli-27.8/README.md`

 * *Files identical despite different names*

### Comparing `connect_cli-27.7/connect/.data/connect_reports/.github/workflows/build.yml` & `connect_cli-27.8/connect/.data/connect_reports/.github/workflows/build.yml`

 * *Files identical despite different names*

### Comparing `connect_cli-27.7/connect/.data/connect_reports/LICENSE` & `connect_cli-27.8/connect/.data/connect_reports/LICENSE`

 * *Files identical despite different names*

### Comparing `connect_cli-27.7/connect/.data/connect_reports/README.md` & `connect_cli-27.8/connect/.data/connect_reports/README.md`

 * *Files identical despite different names*

### Comparing `connect_cli-27.7/connect/.data/connect_reports/poetry.lock` & `connect_cli-27.8/connect/.data/connect_reports/poetry.lock`

 * *Files identical despite different names*

### Comparing `connect_cli-27.7/connect/.data/connect_reports/pyproject.toml` & `connect_cli-27.8/connect/.data/connect_reports/pyproject.toml`

 * *Files identical despite different names*

### Comparing `connect_cli-27.7/connect/.data/connect_reports/reports/billing_requests/entrypoint.py` & `connect_cli-27.8/connect/.data/connect_reports/reports/billing_requests/entrypoint.py`

 * *Files identical despite different names*

### Comparing `connect_cli-27.7/connect/.data/connect_reports/reports/billing_requests/templates/xlsx/template.xlsx` & `connect_cli-27.8/connect/.data/connect_reports/reports/billing_requests/templates/xlsx/template.xlsx`

 * *Files identical despite different names*

### Comparing `connect_cli-27.7/connect/.data/connect_reports/reports/billing_requests_line_item/entrypoint.py` & `connect_cli-27.8/connect/.data/connect_reports/reports/billing_requests_line_item/entrypoint.py`

 * *Files identical despite different names*

### Comparing `connect_cli-27.7/connect/.data/connect_reports/reports/billing_requests_line_item/templates/xlsx/template.xlsx` & `connect_cli-27.8/connect/.data/connect_reports/reports/billing_requests_line_item/templates/xlsx/template.xlsx`

 * *Files identical despite different names*

### Comparing `connect_cli-27.7/connect/.data/connect_reports/reports/contract_list/entrypoint.py` & `connect_cli-27.8/connect/.data/connect_reports/reports/contract_list/entrypoint.py`

 * *Files identical despite different names*

### Comparing `connect_cli-27.7/connect/.data/connect_reports/reports/contract_list/templates/xlsx/template.xlsx` & `connect_cli-27.8/connect/.data/connect_reports/reports/contract_list/templates/xlsx/template.xlsx`

 * *Files identical despite different names*

### Comparing `connect_cli-27.7/connect/.data/connect_reports/reports/customers_list/entrypoint.py` & `connect_cli-27.8/connect/.data/connect_reports/reports/customers_list/entrypoint.py`

 * *Files identical despite different names*

### Comparing `connect_cli-27.7/connect/.data/connect_reports/reports/customers_list/templates/xlsx/template.xlsx` & `connect_cli-27.8/connect/.data/connect_reports/reports/customers_list/templates/xlsx/template.xlsx`

 * *Files identical despite different names*

### Comparing `connect_cli-27.7/connect/.data/connect_reports/reports/executive_fullfilment_requests/Readme.md` & `connect_cli-27.8/connect/.data/connect_reports/reports/executive_fullfilment_requests/Readme.md`

 * *Files identical despite different names*

### Comparing `connect_cli-27.7/connect/.data/connect_reports/reports/executive_fullfilment_requests/constants.py` & `connect_cli-27.8/connect/.data/connect_reports/reports/executive_fullfilment_requests/constants.py`

 * *Files identical despite different names*

### Comparing `connect_cli-27.7/connect/.data/connect_reports/reports/executive_fullfilment_requests/entrypoint.py` & `connect_cli-27.8/connect/.data/connect_reports/reports/executive_fullfilment_requests/entrypoint.py`

 * *Files identical despite different names*

### Comparing `connect_cli-27.7/connect/.data/connect_reports/reports/executive_fullfilment_requests/templates/pdf/img/ClouBlue-Logo.png` & `connect_cli-27.8/connect/.data/connect_reports/reports/executive_fullfilment_requests/templates/pdf/img/ClouBlue-Logo.png`

 * *Files identical despite different names*

### Comparing `connect_cli-27.7/connect/.data/connect_reports/reports/executive_fullfilment_requests/templates/pdf/template.css` & `connect_cli-27.8/connect/.data/connect_reports/reports/executive_fullfilment_requests/templates/pdf/template.css`

 * *Files identical despite different names*

### Comparing `connect_cli-27.7/connect/.data/connect_reports/reports/executive_fullfilment_requests/templates/pdf/template.html.j2` & `connect_cli-27.8/connect/.data/connect_reports/reports/executive_fullfilment_requests/templates/pdf/template.html.j2`

 * *Files identical despite different names*

### Comparing `connect_cli-27.7/connect/.data/connect_reports/reports/fulfillment_requests/entrypoint.py` & `connect_cli-27.8/connect/.data/connect_reports/reports/fulfillment_requests/entrypoint.py`

 * *Files identical despite different names*

### Comparing `connect_cli-27.7/connect/.data/connect_reports/reports/fulfillment_requests/templates/xlsx/template.xlsx` & `connect_cli-27.8/connect/.data/connect_reports/reports/fulfillment_requests/templates/xlsx/template.xlsx`

 * *Files identical despite different names*

### Comparing `connect_cli-27.7/connect/.data/connect_reports/reports/fulfillment_requests_failed/entrypoint.py` & `connect_cli-27.8/connect/.data/connect_reports/reports/fulfillment_requests_failed/entrypoint.py`

 * *Files identical despite different names*

### Comparing `connect_cli-27.7/connect/.data/connect_reports/reports/fulfillment_requests_failed/templates/xlsx/template.xlsx` & `connect_cli-27.8/connect/.data/connect_reports/reports/fulfillment_requests_failed/templates/xlsx/template.xlsx`

 * *Files identical despite different names*

### Comparing `connect_cli-27.7/connect/.data/connect_reports/reports/fulfillment_requests_line_item/entrypoint.py` & `connect_cli-27.8/connect/.data/connect_reports/reports/fulfillment_requests_line_item/entrypoint.py`

 * *Files identical despite different names*

### Comparing `connect_cli-27.7/connect/.data/connect_reports/reports/fulfillment_requests_line_item/templates/xlsx/template.xlsx` & `connect_cli-27.8/connect/.data/connect_reports/reports/fulfillment_requests_line_item/templates/xlsx/template.xlsx`

 * *Files identical despite different names*

### Comparing `connect_cli-27.7/connect/.data/connect_reports/reports/helpdesk/entrypoint.py` & `connect_cli-27.8/connect/.data/connect_reports/reports/helpdesk/entrypoint.py`

 * *Files identical despite different names*

### Comparing `connect_cli-27.7/connect/.data/connect_reports/reports/helpdesk/templates/xlsx/template.xlsx` & `connect_cli-27.8/connect/.data/connect_reports/reports/helpdesk/templates/xlsx/template.xlsx`

 * *Files identical despite different names*

### Comparing `connect_cli-27.7/connect/.data/connect_reports/reports/listing_list/entrypoint.py` & `connect_cli-27.8/connect/.data/connect_reports/reports/listing_list/entrypoint.py`

 * *Files identical despite different names*

### Comparing `connect_cli-27.7/connect/.data/connect_reports/reports/listing_list/templates/xlsx/template.xlsx` & `connect_cli-27.8/connect/.data/connect_reports/reports/listing_list/templates/xlsx/template.xlsx`

 * *Files identical despite different names*

### Comparing `connect_cli-27.7/connect/.data/connect_reports/reports/listing_requests/entrypoint.py` & `connect_cli-27.8/connect/.data/connect_reports/reports/listing_requests/entrypoint.py`

 * *Files identical despite different names*

### Comparing `connect_cli-27.7/connect/.data/connect_reports/reports/listing_requests/templates/xlsx/template.xlsx` & `connect_cli-27.8/connect/.data/connect_reports/reports/listing_requests/templates/xlsx/template.xlsx`

 * *Files identical despite different names*

### Comparing `connect_cli-27.7/connect/.data/connect_reports/reports/products_catalog/entrypoint.py` & `connect_cli-27.8/connect/.data/connect_reports/reports/products_catalog/entrypoint.py`

 * *Files identical despite different names*

### Comparing `connect_cli-27.7/connect/.data/connect_reports/reports/products_catalog/templates/pdf/assets/cloudblue-connect-alone.png` & `connect_cli-27.8/connect/.data/connect_reports/reports/products_catalog/templates/pdf/assets/cloudblue-connect-alone.png`

 * *Files identical despite different names*

### Comparing `connect_cli-27.7/connect/.data/connect_reports/reports/products_catalog/templates/pdf/assets/cloudblue-logo.png` & `connect_cli-27.8/connect/.data/connect_reports/reports/products_catalog/templates/pdf/assets/cloudblue-logo.png`

 * *Files identical despite different names*

### Comparing `connect_cli-27.7/connect/.data/connect_reports/reports/products_catalog/templates/pdf/assets/cloudblue-small-color-disabled.png` & `connect_cli-27.8/connect/.data/connect_reports/reports/products_catalog/templates/pdf/assets/cloudblue-small-color-disabled.png`

 * *Files identical despite different names*

### Comparing `connect_cli-27.7/connect/.data/connect_reports/reports/products_catalog/templates/pdf/assets/cloudblue-small-color-enabled.png` & `connect_cli-27.8/connect/.data/connect_reports/reports/products_catalog/templates/pdf/assets/cloudblue-small-color-enabled.png`

 * *Files identical despite different names*

### Comparing `connect_cli-27.7/connect/.data/connect_reports/reports/products_catalog/templates/pdf/assets/connect-logo.png` & `connect_cli-27.8/connect/.data/connect_reports/reports/products_catalog/templates/pdf/assets/connect-logo.png`

 * *Files identical despite different names*

### Comparing `connect_cli-27.7/connect/.data/connect_reports/reports/products_catalog/templates/pdf/assets/cover-bg.png` & `connect_cli-27.8/connect/.data/connect_reports/reports/products_catalog/templates/pdf/assets/cover-bg.png`

 * *Files identical despite different names*

### Comparing `connect_cli-27.7/connect/.data/connect_reports/reports/products_catalog/templates/pdf/assets/imc-small-color.png` & `connect_cli-27.8/connect/.data/connect_reports/reports/products_catalog/templates/pdf/assets/imc-small-color.png`

 * *Files identical despite different names*

### Comparing `connect_cli-27.7/connect/.data/connect_reports/reports/products_catalog/templates/pdf/img/ClouBlue-Logo-Black.png` & `connect_cli-27.8/connect/.data/connect_reports/reports/products_catalog/templates/pdf/img/ClouBlue-Logo-Black.png`

 * *Files identical despite different names*

### Comparing `connect_cli-27.7/connect/.data/connect_reports/reports/products_catalog/templates/pdf/img/ClouBlue-Logo-White.png` & `connect_cli-27.8/connect/.data/connect_reports/reports/products_catalog/templates/pdf/img/ClouBlue-Logo-White.png`

 * *Files identical despite different names*

### Comparing `connect_cli-27.7/connect/.data/connect_reports/reports/products_catalog/templates/pdf/img/ClouBlue-Logo.png` & `connect_cli-27.8/connect/.data/connect_reports/reports/products_catalog/templates/pdf/img/ClouBlue-Logo.png`

 * *Files identical despite different names*

### Comparing `connect_cli-27.7/connect/.data/connect_reports/reports/products_catalog/templates/pdf/img/accordo.png` & `connect_cli-27.8/connect/.data/connect_reports/reports/products_catalog/templates/pdf/img/accordo.png`

 * *Files identical despite different names*

### Comparing `connect_cli-27.7/connect/.data/connect_reports/reports/products_catalog/templates/pdf/img/acronis-blue.png` & `connect_cli-27.8/connect/.data/connect_reports/reports/products_catalog/templates/pdf/img/acronis-blue.png`

 * *Files identical despite different names*

### Comparing `connect_cli-27.7/connect/.data/connect_reports/reports/products_catalog/templates/pdf/img/acronis-white.png` & `connect_cli-27.8/connect/.data/connect_reports/reports/products_catalog/templates/pdf/img/acronis-white.png`

 * *Files identical despite different names*

### Comparing `connect_cli-27.7/connect/.data/connect_reports/reports/products_catalog/templates/pdf/img/adobe.jpeg` & `connect_cli-27.8/connect/.data/connect_reports/reports/products_catalog/templates/pdf/img/adobe.jpeg`

 * *Files identical despite different names*

### Comparing `connect_cli-27.7/connect/.data/connect_reports/reports/products_catalog/templates/pdf/img/airtame.png` & `connect_cli-27.8/connect/.data/connect_reports/reports/products_catalog/templates/pdf/img/airtame.png`

 * *Files identical despite different names*

### Comparing `connect_cli-27.7/connect/.data/connect_reports/reports/products_catalog/templates/pdf/img/allyhub.png` & `connect_cli-27.8/connect/.data/connect_reports/reports/products_catalog/templates/pdf/img/allyhub.png`

 * *Files identical despite different names*

### Comparing `connect_cli-27.7/connect/.data/connect_reports/reports/products_catalog/templates/pdf/img/alsid.png` & `connect_cli-27.8/connect/.data/connect_reports/reports/products_catalog/templates/pdf/img/alsid.png`

 * *Files identical despite different names*

### Comparing `connect_cli-27.7/connect/.data/connect_reports/reports/products_catalog/templates/pdf/img/anchor.png` & `connect_cli-27.8/connect/.data/connect_reports/reports/products_catalog/templates/pdf/img/anchor.png`

 * *Files identical despite different names*

### Comparing `connect_cli-27.7/connect/.data/connect_reports/reports/products_catalog/templates/pdf/img/australia.png` & `connect_cli-27.8/connect/.data/connect_reports/reports/products_catalog/templates/pdf/img/australia.png`

 * *Files identical despite different names*

### Comparing `connect_cli-27.7/connect/.data/connect_reports/reports/products_catalog/templates/pdf/img/austria.png` & `connect_cli-27.8/connect/.data/connect_reports/reports/products_catalog/templates/pdf/img/austria.png`

 * *Files identical despite different names*

### Comparing `connect_cli-27.7/connect/.data/connect_reports/reports/products_catalog/templates/pdf/img/aws.png` & `connect_cli-27.8/connect/.data/connect_reports/reports/products_catalog/templates/pdf/img/aws.png`

 * *Files identical despite different names*

### Comparing `connect_cli-27.7/connect/.data/connect_reports/reports/products_catalog/templates/pdf/img/belgium.png` & `connect_cli-27.8/connect/.data/connect_reports/reports/products_catalog/templates/pdf/img/belgium.png`

 * *Files identical despite different names*

### Comparing `connect_cli-27.7/connect/.data/connect_reports/reports/products_catalog/templates/pdf/img/brazil.png` & `connect_cli-27.8/connect/.data/connect_reports/reports/products_catalog/templates/pdf/img/brazil.png`

 * *Files identical despite different names*

### Comparing `connect_cli-27.7/connect/.data/connect_reports/reports/products_catalog/templates/pdf/img/canada.png` & `connect_cli-27.8/connect/.data/connect_reports/reports/products_catalog/templates/pdf/img/canada.png`

 * *Files identical despite different names*

### Comparing `connect_cli-27.7/connect/.data/connect_reports/reports/products_catalog/templates/pdf/img/chile.png` & `connect_cli-27.8/connect/.data/connect_reports/reports/products_catalog/templates/pdf/img/chile.png`

 * *Files identical despite different names*

### Comparing `connect_cli-27.7/connect/.data/connect_reports/reports/products_catalog/templates/pdf/img/colombia.png` & `connect_cli-27.8/connect/.data/connect_reports/reports/products_catalog/templates/pdf/img/colombia.png`

 * *Files identical despite different names*

### Comparing `connect_cli-27.7/connect/.data/connect_reports/reports/products_catalog/templates/pdf/img/france.png` & `connect_cli-27.8/connect/.data/connect_reports/reports/products_catalog/templates/pdf/img/france.png`

 * *Files identical despite different names*

### Comparing `connect_cli-27.7/connect/.data/connect_reports/reports/products_catalog/templates/pdf/img/germany.png` & `connect_cli-27.8/connect/.data/connect_reports/reports/products_catalog/templates/pdf/img/germany.png`

 * *Files identical despite different names*

### Comparing `connect_cli-27.7/connect/.data/connect_reports/reports/products_catalog/templates/pdf/img/hong-kong.png` & `connect_cli-27.8/connect/.data/connect_reports/reports/products_catalog/templates/pdf/img/hong-kong.png`

 * *Files identical despite different names*

### Comparing `connect_cli-27.7/connect/.data/connect_reports/reports/products_catalog/templates/pdf/img/icon.png` & `connect_cli-27.8/connect/.data/connect_reports/reports/products_catalog/templates/pdf/img/icon.png`

 * *Files identical despite different names*

### Comparing `connect_cli-27.7/connect/.data/connect_reports/reports/products_catalog/templates/pdf/img/india.png` & `connect_cli-27.8/connect/.data/connect_reports/reports/products_catalog/templates/pdf/img/india.png`

 * *Files identical despite different names*

### Comparing `connect_cli-27.7/connect/.data/connect_reports/reports/products_catalog/templates/pdf/img/italy.png` & `connect_cli-27.8/connect/.data/connect_reports/reports/products_catalog/templates/pdf/img/italy.png`

 * *Files identical despite different names*

### Comparing `connect_cli-27.7/connect/.data/connect_reports/reports/products_catalog/templates/pdf/img/malaysia.png` & `connect_cli-27.8/connect/.data/connect_reports/reports/products_catalog/templates/pdf/img/malaysia.png`

 * *Files identical despite different names*

### Comparing `connect_cli-27.7/connect/.data/connect_reports/reports/products_catalog/templates/pdf/img/mexico.png` & `connect_cli-27.8/connect/.data/connect_reports/reports/products_catalog/templates/pdf/img/mexico.png`

 * *Files identical despite different names*

### Comparing `connect_cli-27.7/connect/.data/connect_reports/reports/products_catalog/templates/pdf/img/netherlands.png` & `connect_cli-27.8/connect/.data/connect_reports/reports/products_catalog/templates/pdf/img/netherlands.png`

 * *Files identical despite different names*

### Comparing `connect_cli-27.7/connect/.data/connect_reports/reports/products_catalog/templates/pdf/img/new-zealand.png` & `connect_cli-27.8/connect/.data/connect_reports/reports/products_catalog/templates/pdf/img/new-zealand.png`

 * *Files identical despite different names*

### Comparing `connect_cli-27.7/connect/.data/connect_reports/reports/products_catalog/templates/pdf/img/singapore.png` & `connect_cli-27.8/connect/.data/connect_reports/reports/products_catalog/templates/pdf/img/singapore.png`

 * *Files identical despite different names*

### Comparing `connect_cli-27.7/connect/.data/connect_reports/reports/products_catalog/templates/pdf/img/spain.png` & `connect_cli-27.8/connect/.data/connect_reports/reports/products_catalog/templates/pdf/img/spain.png`

 * *Files identical despite different names*

### Comparing `connect_cli-27.7/connect/.data/connect_reports/reports/products_catalog/templates/pdf/img/sweden.png` & `connect_cli-27.8/connect/.data/connect_reports/reports/products_catalog/templates/pdf/img/sweden.png`

 * *Files identical despite different names*

### Comparing `connect_cli-27.7/connect/.data/connect_reports/reports/products_catalog/templates/pdf/img/switzerland.png` & `connect_cli-27.8/connect/.data/connect_reports/reports/products_catalog/templates/pdf/img/switzerland.png`

 * *Files identical despite different names*

### Comparing `connect_cli-27.7/connect/.data/connect_reports/reports/products_catalog/templates/pdf/img/turkey.png` & `connect_cli-27.8/connect/.data/connect_reports/reports/products_catalog/templates/pdf/img/turkey.png`

 * *Files identical despite different names*

### Comparing `connect_cli-27.7/connect/.data/connect_reports/reports/products_catalog/templates/pdf/img/uae.png` & `connect_cli-27.8/connect/.data/connect_reports/reports/products_catalog/templates/pdf/img/uae.png`

 * *Files identical despite different names*

### Comparing `connect_cli-27.7/connect/.data/connect_reports/reports/products_catalog/templates/pdf/img/uk.png` & `connect_cli-27.8/connect/.data/connect_reports/reports/products_catalog/templates/pdf/img/uk.png`

 * *Files identical despite different names*

### Comparing `connect_cli-27.7/connect/.data/connect_reports/reports/products_catalog/templates/pdf/img/usa.png` & `connect_cli-27.8/connect/.data/connect_reports/reports/products_catalog/templates/pdf/img/usa.png`

 * *Files identical despite different names*

### Comparing `connect_cli-27.7/connect/.data/connect_reports/reports/products_catalog/templates/pdf/template.css` & `connect_cli-27.8/connect/.data/connect_reports/reports/products_catalog/templates/pdf/template.css`

 * *Files identical despite different names*

### Comparing `connect_cli-27.7/connect/.data/connect_reports/reports/products_catalog/templates/pdf/template.html.j2` & `connect_cli-27.8/connect/.data/connect_reports/reports/products_catalog/templates/pdf/template.html.j2`

 * *Files identical despite different names*

### Comparing `connect_cli-27.7/connect/.data/connect_reports/reports/sla/Readme.md` & `connect_cli-27.8/connect/.data/connect_reports/reports/sla/Readme.md`

 * *Files identical despite different names*

### Comparing `connect_cli-27.7/connect/.data/connect_reports/reports/sla/entrypoint.py` & `connect_cli-27.8/connect/.data/connect_reports/reports/sla/entrypoint.py`

 * *Files identical despite different names*

### Comparing `connect_cli-27.7/connect/.data/connect_reports/reports/sla/templates/xlsx/template.xlsx` & `connect_cli-27.8/connect/.data/connect_reports/reports/sla/templates/xlsx/template.xlsx`

 * *Files identical despite different names*

### Comparing `connect_cli-27.7/connect/.data/connect_reports/reports/subscription_list/entrypoint.py` & `connect_cli-27.8/connect/.data/connect_reports/reports/subscription_list/entrypoint.py`

 * *Files identical despite different names*

### Comparing `connect_cli-27.7/connect/.data/connect_reports/reports/subscription_list/templates/xlsx/template.xlsx` & `connect_cli-27.8/connect/.data/connect_reports/reports/subscription_list/templates/xlsx/template.xlsx`

 * *Files identical despite different names*

### Comparing `connect_cli-27.7/connect/.data/connect_reports/reports/tier_configuration_list/entrypoint.py` & `connect_cli-27.8/connect/.data/connect_reports/reports/tier_configuration_list/entrypoint.py`

 * *Files identical despite different names*

### Comparing `connect_cli-27.7/connect/.data/connect_reports/reports/tier_configuration_list/templates/xlsx/template.xlsx` & `connect_cli-27.8/connect/.data/connect_reports/reports/tier_configuration_list/templates/xlsx/template.xlsx`

 * *Files identical despite different names*

### Comparing `connect_cli-27.7/connect/.data/connect_reports/reports/tier_configuration_requests/entrypoint.py` & `connect_cli-27.8/connect/.data/connect_reports/reports/tier_configuration_requests/entrypoint.py`

 * *Files identical despite different names*

### Comparing `connect_cli-27.7/connect/.data/connect_reports/reports/tier_configuration_requests/templates/xlsx/template.xlsx` & `connect_cli-27.8/connect/.data/connect_reports/reports/tier_configuration_requests/templates/xlsx/template.xlsx`

 * *Files identical despite different names*

### Comparing `connect_cli-27.7/connect/.data/connect_reports/reports/usage_in_subscription/entrypoint.py` & `connect_cli-27.8/connect/.data/connect_reports/reports/usage_in_subscription/entrypoint.py`

 * *Files identical despite different names*

### Comparing `connect_cli-27.7/connect/.data/connect_reports/reports/usage_in_subscription/templates/xlsx/template.xlsx` & `connect_cli-27.8/connect/.data/connect_reports/reports/usage_in_subscription/templates/xlsx/template.xlsx`

 * *Files identical despite different names*

### Comparing `connect_cli-27.7/connect/.data/connect_reports/reports/utils.py` & `connect_cli-27.8/connect/.data/connect_reports/reports/utils.py`

 * *Files identical despite different names*

### Comparing `connect_cli-27.7/connect/.data/connect_reports/reports.json` & `connect_cli-27.8/connect/.data/connect_reports/reports.json`

 * *Files identical despite different names*

### Comparing `connect_cli-27.7/connect/cli/ccli.py` & `connect_cli-27.8/connect/cli/ccli.py`

 * *Files identical despite different names*

### Comparing `connect_cli-27.7/connect/cli/core/account/commands.py` & `connect_cli-27.8/connect/cli/core/account/commands.py`

 * *Files identical despite different names*

### Comparing `connect_cli-27.7/connect/cli/core/account/helpers.py` & `connect_cli-27.8/connect/cli/core/account/helpers.py`

 * *Files identical despite different names*

### Comparing `connect_cli-27.7/connect/cli/core/base.py` & `connect_cli-27.8/connect/cli/core/base.py`

 * *Files identical despite different names*

### Comparing `connect_cli-27.7/connect/cli/core/config.py` & `connect_cli-27.8/connect/cli/core/config.py`

 * *Files identical despite different names*

### Comparing `connect_cli-27.7/connect/cli/core/constants.py` & `connect_cli-27.8/connect/cli/core/constants.py`

 * *Files identical despite different names*

### Comparing `connect_cli-27.7/connect/cli/core/http.py` & `connect_cli-27.8/connect/cli/core/http.py`

 * *Files identical despite different names*

### Comparing `connect_cli-27.7/connect/cli/core/plugins.py` & `connect_cli-27.8/connect/cli/core/plugins.py`

 * *Files identical despite different names*

### Comparing `connect_cli-27.7/connect/cli/core/terminal.py` & `connect_cli-27.8/connect/cli/core/terminal.py`

 * *Files identical despite different names*

### Comparing `connect_cli-27.7/connect/cli/core/utils.py` & `connect_cli-27.8/connect/cli/core/utils.py`

 * *Files identical despite different names*

### Comparing `connect_cli-27.7/connect/cli/plugins/customer/commands.py` & `connect_cli-27.8/connect/cli/plugins/customer/commands.py`

 * *Files identical despite different names*

### Comparing `connect_cli-27.7/connect/cli/plugins/customer/constants.py` & `connect_cli-27.8/connect/cli/plugins/customer/constants.py`

 * *Files identical despite different names*

### Comparing `connect_cli-27.7/connect/cli/plugins/customer/export.py` & `connect_cli-27.8/connect/cli/plugins/customer/export.py`

 * *Files identical despite different names*

### Comparing `connect_cli-27.7/connect/cli/plugins/customer/sync.py` & `connect_cli-27.8/connect/cli/plugins/customer/sync.py`

 * *Files identical despite different names*

### Comparing `connect_cli-27.7/connect/cli/plugins/locale/commands.py` & `connect_cli-27.8/connect/cli/plugins/locale/commands.py`

 * *Files identical despite different names*

### Comparing `connect_cli-27.7/connect/cli/plugins/play/commands.py` & `connect_cli-27.8/connect/cli/plugins/play/commands.py`

 * *Files identical despite different names*

### Comparing `connect_cli-27.7/connect/cli/plugins/play/context.py` & `connect_cli-27.8/connect/cli/plugins/play/context.py`

 * *Files identical despite different names*

### Comparing `connect_cli-27.7/connect/cli/plugins/play/script.py` & `connect_cli-27.8/connect/cli/plugins/play/script.py`

 * *Files identical despite different names*

### Comparing `connect_cli-27.7/connect/cli/plugins/product/api.py` & `connect_cli-27.8/connect/cli/plugins/product/api.py`

 * *Files identical despite different names*

### Comparing `connect_cli-27.7/connect/cli/plugins/product/clone.py` & `connect_cli-27.8/connect/cli/plugins/product/clone.py`

 * *Files identical despite different names*

### Comparing `connect_cli-27.7/connect/cli/plugins/product/commands.py` & `connect_cli-27.8/connect/cli/plugins/product/commands.py`

 * *Files identical despite different names*

### Comparing `connect_cli-27.7/connect/cli/plugins/product/constants.py` & `connect_cli-27.8/connect/cli/plugins/product/constants.py`

 * *Files identical despite different names*

### Comparing `connect_cli-27.7/connect/cli/plugins/product/export.py` & `connect_cli-27.8/connect/cli/plugins/product/export.py`

 * *Files 0% similar despite different names*

```diff
@@ -398,15 +398,15 @@
     ws.cell(row_idx, 1, value=item['id'])
     ws.cell(row_idx, 2, value=item['mpn'])
     ws.cell(row_idx, 3, value='-')
     ws.cell(row_idx, 4, value=item['display_name'])
     ws.cell(row_idx, 5, value=item['description'])
     ws.cell(row_idx, 6, value=item['type'])
     ws.cell(row_idx, 7, value=item['precision'])
-    ws.cell(row_idx, 8, value=item['unit']['id'])
+    ws.cell(row_idx, 8, value=item['unit']['name'])
     period = item.get('period', 'monthly')
     if period.startswith('years_'):
         period = f'{period.rsplit("_")[-1]} years'
     ws.cell(row_idx, 9, value=period)
     ws.cell(row_idx, 10, value=_calculate_commitment(item))
     ws.cell(row_idx, 11, value=item['status'])
     events = item.get('events', {})
```

### Comparing `connect_cli-27.7/connect/cli/plugins/product/sync/__init__.py` & `connect_cli-27.8/connect/cli/plugins/product/sync/__init__.py`

 * *Files identical despite different names*

### Comparing `connect_cli-27.7/connect/cli/plugins/product/sync/actions.py` & `connect_cli-27.8/connect/cli/plugins/product/sync/actions.py`

 * *Files identical despite different names*

### Comparing `connect_cli-27.7/connect/cli/plugins/product/sync/capabilities.py` & `connect_cli-27.8/connect/cli/plugins/product/sync/capabilities.py`

 * *Files identical despite different names*

### Comparing `connect_cli-27.7/connect/cli/plugins/product/sync/configuration_values.py` & `connect_cli-27.8/connect/cli/plugins/product/sync/configuration_values.py`

 * *Files identical despite different names*

### Comparing `connect_cli-27.7/connect/cli/plugins/product/sync/general.py` & `connect_cli-27.8/connect/cli/plugins/product/sync/general.py`

 * *Files identical despite different names*

### Comparing `connect_cli-27.7/connect/cli/plugins/product/sync/items.py` & `connect_cli-27.8/connect/cli/plugins/product/sync/items.py`

 * *Files 2% similar despite different names*

```diff
@@ -28,15 +28,23 @@
 fields = (v.replace(' ', '_').lower() for v in ITEMS_COLS_HEADERS.values())
 
 _RowData = namedtuple('RowData', fields)
 
 
 class ItemSynchronizer(ProductSynchronizer):
     def __init__(self, client, progress, stats):
-        self._units = list(client.ns('settings').units.all())
+        self._units = []
+        self._shared_units = []
+
+        for unit in client.ns('settings').units.all():
+            if 'owner' in unit:
+                self._units.append(unit)
+            else:
+                self._shared_units.append(unit)
+
         self._mstats = stats['Items']
         super().__init__(client, progress)
 
     def sync(self):  # noqa: CCR001
         ws = self._wb['Items']
 
         task = self._progress.add_task('Processing item', total=ws.max_row - 1)
@@ -270,14 +278,20 @@
     def _get_or_create_unit(self, data):
         for unit in self._units:
             if unit['id'] == data.unit:
                 return unit['id']
             if unit['type'] == data.type and unit['description'] == data.unit:
                 return unit['id']
 
+        for unit in self._shared_units:
+            if unit['id'] == data.unit:
+                return unit['id']
+            if unit['type'] == data.type and unit['description'] == data.unit:
+                return unit['id']
+
         created = create_unit(
             self._client,
             {
                 'description': data.unit,
                 'type': data.type,
                 'unit': 'unit' if data.type == 'reservation' else 'unit-h',
             },
```

### Comparing `connect_cli-27.7/connect/cli/plugins/product/sync/media.py` & `connect_cli-27.8/connect/cli/plugins/product/sync/media.py`

 * *Files identical despite different names*

### Comparing `connect_cli-27.7/connect/cli/plugins/product/sync/params.py` & `connect_cli-27.8/connect/cli/plugins/product/sync/params.py`

 * *Files identical despite different names*

### Comparing `connect_cli-27.7/connect/cli/plugins/product/sync/static_resources.py` & `connect_cli-27.8/connect/cli/plugins/product/sync/static_resources.py`

 * *Files identical despite different names*

### Comparing `connect_cli-27.7/connect/cli/plugins/product/sync/templates.py` & `connect_cli-27.8/connect/cli/plugins/product/sync/templates.py`

 * *Files identical despite different names*

### Comparing `connect_cli-27.7/connect/cli/plugins/product/utils.py` & `connect_cli-27.8/connect/cli/plugins/product/utils.py`

 * *Files identical despite different names*

### Comparing `connect_cli-27.7/connect/cli/plugins/project/commands.py` & `connect_cli-27.8/connect/cli/plugins/project/commands.py`

 * *Files identical despite different names*

### Comparing `connect_cli-27.7/connect/cli/plugins/project/extension/helpers.py` & `connect_cli-27.8/connect/cli/plugins/project/extension/helpers.py`

 * *Files identical despite different names*

### Comparing `connect_cli-27.7/connect/cli/plugins/project/extension/templates/bootstrap/${project_slug}/${package_name}/anvil.py.j2` & `connect_cli-27.8/connect/cli/plugins/project/extension/templates/bootstrap/${project_slug}/${package_name}/anvil.py.j2`

 * *Files identical despite different names*

### Comparing `connect_cli-27.7/connect/cli/plugins/project/extension/templates/bootstrap/${project_slug}/${package_name}/events.py.j2` & `connect_cli-27.8/connect/cli/plugins/project/extension/templates/bootstrap/${project_slug}/${package_name}/events.py.j2`

 * *Files identical despite different names*

### Comparing `connect_cli-27.7/connect/cli/plugins/project/extension/templates/bootstrap/${project_slug}/${package_name}/schemas.py.j2` & `connect_cli-27.8/connect/cli/plugins/project/extension/templates/bootstrap/${project_slug}/${package_name}/schemas.py.j2`

 * *Files identical despite different names*

### Comparing `connect_cli-27.7/connect/cli/plugins/project/extension/templates/bootstrap/${project_slug}/${package_name}/tfnapp.py.j2` & `connect_cli-27.8/connect/cli/plugins/project/extension/templates/bootstrap/${project_slug}/${package_name}/tfnapp.py.j2`

 * *Files identical despite different names*

### Comparing `connect_cli-27.7/connect/cli/plugins/project/extension/templates/bootstrap/${project_slug}/${package_name}/webapp.py.j2` & `connect_cli-27.8/connect/cli/plugins/project/extension/templates/bootstrap/${project_slug}/${package_name}/webapp.py.j2`

 * *Files identical despite different names*

### Comparing `connect_cli-27.7/connect/cli/plugins/project/extension/templates/bootstrap/${project_slug}/.${project_slug}_dev.env.j2` & `connect_cli-27.8/connect/cli/plugins/project/extension/templates/bootstrap/${project_slug}/.${project_slug}_dev.env.j2`

 * *Files identical despite different names*

### Comparing `connect_cli-27.7/connect/cli/plugins/project/extension/templates/bootstrap/${project_slug}/.eslintrc.yaml.j2` & `connect_cli-27.8/connect/cli/plugins/project/extension/templates/bootstrap/${project_slug}/.eslintrc.yaml.j2`

 * *Files identical despite different names*

### Comparing `connect_cli-27.7/connect/cli/plugins/project/extension/templates/bootstrap/${project_slug}/.github/workflows/test.yml.j2` & `connect_cli-27.8/connect/cli/plugins/project/extension/templates/bootstrap/${project_slug}/.github/workflows/test.yml.j2`

 * *Files identical despite different names*

### Comparing `connect_cli-27.7/connect/cli/plugins/project/extension/templates/bootstrap/${project_slug}/HOWTO.md.j2` & `connect_cli-27.8/connect/cli/plugins/project/extension/templates/bootstrap/${project_slug}/HOWTO.md.j2`

 * *Files identical despite different names*

### Comparing `connect_cli-27.7/connect/cli/plugins/project/extension/templates/bootstrap/${project_slug}/LICENSE.j2` & `connect_cli-27.8/connect/cli/plugins/project/extension/templates/bootstrap/${project_slug}/LICENSE.j2`

 * *Files identical despite different names*

### Comparing `connect_cli-27.7/connect/cli/plugins/project/extension/templates/bootstrap/${project_slug}/docker-compose.yml.j2` & `connect_cli-27.8/connect/cli/plugins/project/extension/templates/bootstrap/${project_slug}/docker-compose.yml.j2`

 * *Files identical despite different names*

### Comparing `connect_cli-27.7/connect/cli/plugins/project/extension/templates/bootstrap/${project_slug}/jest.config.js.j2` & `connect_cli-27.8/connect/cli/plugins/project/extension/templates/bootstrap/${project_slug}/jest.config.js.j2`

 * *Files identical despite different names*

### Comparing `connect_cli-27.7/connect/cli/plugins/project/extension/templates/bootstrap/${project_slug}/package.json.j2` & `connect_cli-27.8/connect/cli/plugins/project/extension/templates/bootstrap/${project_slug}/package.json.j2`

 * *Files identical despite different names*

### Comparing `connect_cli-27.7/connect/cli/plugins/project/extension/templates/bootstrap/${project_slug}/pyproject.toml.j2` & `connect_cli-27.8/connect/cli/plugins/project/extension/templates/bootstrap/${project_slug}/pyproject.toml.j2`

 * *Files identical despite different names*

### Comparing `connect_cli-27.7/connect/cli/plugins/project/extension/templates/bootstrap/${project_slug}/tests/conftest.py.j2` & `connect_cli-27.8/connect/cli/plugins/project/extension/templates/bootstrap/${project_slug}/tests/conftest.py.j2`

 * *Files identical despite different names*

### Comparing `connect_cli-27.7/connect/cli/plugins/project/extension/templates/bootstrap/${project_slug}/tests/test_anvil.py.j2` & `connect_cli-27.8/connect/cli/plugins/project/extension/templates/bootstrap/${project_slug}/tests/test_anvil.py.j2`

 * *Files identical despite different names*

### Comparing `connect_cli-27.7/connect/cli/plugins/project/extension/templates/bootstrap/${project_slug}/tests/test_events.py.j2` & `connect_cli-27.8/connect/cli/plugins/project/extension/templates/bootstrap/${project_slug}/tests/test_events.py.j2`

 * *Files identical despite different names*

### Comparing `connect_cli-27.7/connect/cli/plugins/project/extension/templates/bootstrap/${project_slug}/tests/test_tfnapp.py.j2` & `connect_cli-27.8/connect/cli/plugins/project/extension/templates/bootstrap/${project_slug}/tests/test_tfnapp.py.j2`

 * *Files identical despite different names*

### Comparing `connect_cli-27.7/connect/cli/plugins/project/extension/templates/bootstrap/${project_slug}/tests/test_webapp.py.j2` & `connect_cli-27.8/connect/cli/plugins/project/extension/templates/bootstrap/${project_slug}/tests/test_webapp.py.j2`

 * *Files identical despite different names*

### Comparing `connect_cli-27.7/connect/cli/plugins/project/extension/templates/bootstrap/${project_slug}/ui/images/mkp.svg.j2` & `connect_cli-27.8/connect/cli/plugins/project/extension/templates/bootstrap/${project_slug}/ui/images/mkp.svg.j2`

 * *Files identical despite different names*

### Comparing `connect_cli-27.7/connect/cli/plugins/project/extension/templates/bootstrap/${project_slug}/ui/pages/index.html.j2` & `connect_cli-27.8/connect/cli/plugins/project/extension/templates/bootstrap/${project_slug}/ui/pages/index.html.j2`

 * *Files identical despite different names*

### Comparing `connect_cli-27.7/connect/cli/plugins/project/extension/templates/bootstrap/${project_slug}/ui/pages/settings.html.j2` & `connect_cli-27.8/connect/cli/plugins/project/extension/templates/bootstrap/${project_slug}/ui/pages/settings.html.j2`

 * *Files identical despite different names*

### Comparing `connect_cli-27.7/connect/cli/plugins/project/extension/templates/bootstrap/${project_slug}/ui/pages/transformations/manual.html.j2` & `connect_cli-27.8/connect/cli/plugins/project/extension/templates/bootstrap/${project_slug}/ui/pages/transformations/manual.html.j2`

 * *Files identical despite different names*

### Comparing `connect_cli-27.7/connect/cli/plugins/project/extension/templates/bootstrap/${project_slug}/ui/src/components.js.j2` & `connect_cli-27.8/connect/cli/plugins/project/extension/templates/bootstrap/${project_slug}/ui/src/components.js.j2`

 * *Files identical despite different names*

### Comparing `connect_cli-27.7/connect/cli/plugins/project/extension/templates/bootstrap/${project_slug}/ui/src/pages.js.j2` & `connect_cli-27.8/connect/cli/plugins/project/extension/templates/bootstrap/${project_slug}/ui/src/pages.js.j2`

 * *Files identical despite different names*

### Comparing `connect_cli-27.7/connect/cli/plugins/project/extension/templates/bootstrap/${project_slug}/ui/src/utils.js.j2` & `connect_cli-27.8/connect/cli/plugins/project/extension/templates/bootstrap/${project_slug}/ui/src/utils.js.j2`

 * *Files identical despite different names*

### Comparing `connect_cli-27.7/connect/cli/plugins/project/extension/templates/bootstrap/${project_slug}/ui/styles/index.css.j2` & `connect_cli-27.8/connect/cli/plugins/project/extension/templates/bootstrap/${project_slug}/ui/styles/index.css.j2`

 * *Files identical despite different names*

### Comparing `connect_cli-27.7/connect/cli/plugins/project/extension/templates/bootstrap/${project_slug}/ui/styles/manual.css.j2` & `connect_cli-27.8/connect/cli/plugins/project/extension/templates/bootstrap/${project_slug}/ui/styles/manual.css.j2`

 * *Files identical despite different names*

### Comparing `connect_cli-27.7/connect/cli/plugins/project/extension/templates/bootstrap/${project_slug}/ui/tests/components.spec.js.j2` & `connect_cli-27.8/connect/cli/plugins/project/extension/templates/bootstrap/${project_slug}/ui/tests/components.spec.js.j2`

 * *Files identical despite different names*

### Comparing `connect_cli-27.7/connect/cli/plugins/project/extension/templates/bootstrap/${project_slug}/ui/tests/pages.spec.js.j2` & `connect_cli-27.8/connect/cli/plugins/project/extension/templates/bootstrap/${project_slug}/ui/tests/pages.spec.js.j2`

 * *Files identical despite different names*

### Comparing `connect_cli-27.7/connect/cli/plugins/project/extension/templates/bootstrap/${project_slug}/ui/tests/utils.spec.js.j2` & `connect_cli-27.8/connect/cli/plugins/project/extension/templates/bootstrap/${project_slug}/ui/tests/utils.spec.js.j2`

 * *Files identical despite different names*

### Comparing `connect_cli-27.7/connect/cli/plugins/project/extension/templates/bootstrap/${project_slug}/webpack.config.js.j2` & `connect_cli-27.8/connect/cli/plugins/project/extension/templates/bootstrap/${project_slug}/webpack.config.js.j2`

 * *Files identical despite different names*

### Comparing `connect_cli-27.7/connect/cli/plugins/project/extension/utils.py` & `connect_cli-27.8/connect/cli/plugins/project/extension/utils.py`

 * *Files identical despite different names*

### Comparing `connect_cli-27.7/connect/cli/plugins/project/extension/validators.py` & `connect_cli-27.8/connect/cli/plugins/project/extension/validators.py`

 * *Files identical despite different names*

### Comparing `connect_cli-27.7/connect/cli/plugins/project/extension/wizard.py` & `connect_cli-27.8/connect/cli/plugins/project/extension/wizard.py`

 * *Files identical despite different names*

### Comparing `connect_cli-27.7/connect/cli/plugins/project/renderer.py` & `connect_cli-27.8/connect/cli/plugins/project/renderer.py`

 * *Files identical despite different names*

### Comparing `connect_cli-27.7/connect/cli/plugins/project/report/helpers.py` & `connect_cli-27.8/connect/cli/plugins/project/report/helpers.py`

 * *Files identical despite different names*

### Comparing `connect_cli-27.7/connect/cli/plugins/project/report/templates/add/${initial_report_slug}/entrypoint.py.j2` & `connect_cli-27.8/connect/cli/plugins/project/report/templates/add/${initial_report_slug}/entrypoint.py.j2`

 * *Files identical despite different names*

### Comparing `connect_cli-27.7/connect/cli/plugins/project/report/templates/bootstrap/${project_slug}/${package_name}/${initial_report_slug}/entrypoint.py.j2` & `connect_cli-27.8/connect/cli/plugins/project/report/templates/bootstrap/${project_slug}/${package_name}/${initial_report_slug}/entrypoint.py.j2`

 * *Files identical despite different names*

### Comparing `connect_cli-27.7/connect/cli/plugins/project/report/templates/bootstrap/${project_slug}/${package_name}/${initial_report_slug}/templates/pdf/template.html.j2.j2` & `connect_cli-27.8/connect/cli/plugins/project/report/templates/bootstrap/${project_slug}/${package_name}/${initial_report_slug}/templates/pdf/template.html.j2.j2`

 * *Files identical despite different names*

### Comparing `connect_cli-27.7/connect/cli/plugins/project/report/templates/bootstrap/${project_slug}/.github/workflows/build.yml.j2` & `connect_cli-27.8/connect/cli/plugins/project/report/templates/bootstrap/${project_slug}/.github/workflows/build.yml.j2`

 * *Files identical despite different names*

### Comparing `connect_cli-27.7/connect/cli/plugins/project/report/templates/bootstrap/${project_slug}/LICENSE.j2` & `connect_cli-27.8/connect/cli/plugins/project/report/templates/bootstrap/${project_slug}/LICENSE.j2`

 * *Files identical despite different names*

### Comparing `connect_cli-27.7/connect/cli/plugins/project/report/templates/bootstrap/${project_slug}/pyproject.toml.j2` & `connect_cli-27.8/connect/cli/plugins/project/report/templates/bootstrap/${project_slug}/pyproject.toml.j2`

 * *Files identical despite different names*

### Comparing `connect_cli-27.7/connect/cli/plugins/project/report/templates/bootstrap/${project_slug}/reports.json.j2` & `connect_cli-27.8/connect/cli/plugins/project/report/templates/bootstrap/${project_slug}/reports.json.j2`

 * *Files identical despite different names*

### Comparing `connect_cli-27.7/connect/cli/plugins/project/report/templates/bootstrap/${project_slug}/tests/conftest.py.j2` & `connect_cli-27.8/connect/cli/plugins/project/report/templates/bootstrap/${project_slug}/tests/conftest.py.j2`

 * *Files identical despite different names*

### Comparing `connect_cli-27.7/connect/cli/plugins/project/report/templates/bootstrap/${project_slug}/tests/test_${project_slug}.py.j2` & `connect_cli-27.8/connect/cli/plugins/project/report/templates/bootstrap/${project_slug}/tests/test_${project_slug}.py.j2`

 * *Files identical despite different names*

### Comparing `connect_cli-27.7/connect/cli/plugins/project/report/validations.py` & `connect_cli-27.8/connect/cli/plugins/project/report/validations.py`

 * *Files identical despite different names*

### Comparing `connect_cli-27.7/connect/cli/plugins/project/report/wizard.py` & `connect_cli-27.8/connect/cli/plugins/project/report/wizard.py`

 * *Files identical despite different names*

### Comparing `connect_cli-27.7/connect/cli/plugins/project/utils.py` & `connect_cli-27.8/connect/cli/plugins/project/utils.py`

 * *Files identical despite different names*

### Comparing `connect_cli-27.7/connect/cli/plugins/project/validators.py` & `connect_cli-27.8/connect/cli/plugins/project/validators.py`

 * *Files identical despite different names*

### Comparing `connect_cli-27.7/connect/cli/plugins/report/commands.py` & `connect_cli-27.8/connect/cli/plugins/report/commands.py`

 * *Files identical despite different names*

### Comparing `connect_cli-27.7/connect/cli/plugins/report/helpers.py` & `connect_cli-27.8/connect/cli/plugins/report/helpers.py`

 * *Files identical despite different names*

### Comparing `connect_cli-27.7/connect/cli/plugins/report/utils.py` & `connect_cli-27.8/connect/cli/plugins/report/utils.py`

 * *Files identical despite different names*

### Comparing `connect_cli-27.7/connect/cli/plugins/report/wizard.py` & `connect_cli-27.8/connect/cli/plugins/report/wizard.py`

 * *Files identical despite different names*

### Comparing `connect_cli-27.7/connect/cli/plugins/shared/base.py` & `connect_cli-27.8/connect/cli/plugins/shared/base.py`

 * *Files identical despite different names*

### Comparing `connect_cli-27.7/connect/cli/plugins/shared/constants.py` & `connect_cli-27.8/connect/cli/plugins/shared/constants.py`

 * *Files identical despite different names*

### Comparing `connect_cli-27.7/connect/cli/plugins/shared/export.py` & `connect_cli-27.8/connect/cli/plugins/shared/export.py`

 * *Files identical despite different names*

### Comparing `connect_cli-27.7/connect/cli/plugins/shared/sync_stats.py` & `connect_cli-27.8/connect/cli/plugins/shared/sync_stats.py`

 * *Files identical despite different names*

### Comparing `connect_cli-27.7/connect/cli/plugins/shared/translation_attr_sync.py` & `connect_cli-27.8/connect/cli/plugins/shared/translation_attr_sync.py`

 * *Files identical despite different names*

### Comparing `connect_cli-27.7/connect/cli/plugins/shared/translation_sync.py` & `connect_cli-27.8/connect/cli/plugins/shared/translation_sync.py`

 * *Files identical despite different names*

### Comparing `connect_cli-27.7/connect/cli/plugins/shared/translations_synchronizers.py` & `connect_cli-27.8/connect/cli/plugins/shared/translations_synchronizers.py`

 * *Files identical despite different names*

### Comparing `connect_cli-27.7/connect/cli/plugins/shared/utils.py` & `connect_cli-27.8/connect/cli/plugins/shared/utils.py`

 * *Files identical despite different names*

### Comparing `connect_cli-27.7/connect/cli/plugins/translation/activate.py` & `connect_cli-27.8/connect/cli/plugins/translation/activate.py`

 * *Files identical despite different names*

### Comparing `connect_cli-27.7/connect/cli/plugins/translation/commands.py` & `connect_cli-27.8/connect/cli/plugins/translation/commands.py`

 * *Files identical despite different names*

### Comparing `connect_cli-27.7/connect/cli/plugins/translation/constants.py` & `connect_cli-27.8/connect/cli/plugins/translation/constants.py`

 * *Files identical despite different names*

### Comparing `connect_cli-27.7/connect/cli/plugins/translation/export.py` & `connect_cli-27.8/connect/cli/plugins/translation/export.py`

 * *Files identical despite different names*

### Comparing `connect_cli-27.7/connect/cli/plugins/translation/primarize.py` & `connect_cli-27.8/connect/cli/plugins/translation/primarize.py`

 * *Files identical despite different names*

### Comparing `connect_cli-27.7/connect/cli/plugins/translation/translation_sync.py` & `connect_cli-27.8/connect/cli/plugins/translation/translation_sync.py`

 * *Files identical despite different names*

### Comparing `connect_cli-27.7/connect/cli/plugins/translation/utils.py` & `connect_cli-27.8/connect/cli/plugins/translation/utils.py`

 * *Files identical despite different names*

### Comparing `connect_cli-27.7/pyproject.toml` & `connect_cli-27.8/pyproject.toml`

 * *Files 0% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 [tool.poetry]
 name = "connect-cli"
-version = "27.7"
+version = "27.8"
 description = "CloudBlue Connect Command Line Interface"
 authors = ["CloudBlue LLC"]
 license = "Apache-2.0"
 
 packages = [
     { include = "connect" },
 ]
```

### Comparing `connect_cli-27.7/PKG-INFO` & `connect_cli-27.8/PKG-INFO`

 * *Files 0% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: connect-cli
-Version: 27.7
+Version: 27.8
 Summary: CloudBlue Connect Command Line Interface
 Home-page: https://connect.cloudblue.com
 License: Apache-2.0
 Keywords: fulfillment,command,line,interface,utility,cli,vendor,connect,cloudblue
 Author: CloudBlue LLC
 Requires-Python: >=3.8,<4
 Classifier: Development Status :: 5 - Production/Stable
```

