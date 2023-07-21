# Comparing `tmp/elhub_python_sdk-0.1.4.tar.gz` & `tmp/elhub_python_sdk-0.1.5.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "elhub_python_sdk-0.1.4.tar", max compression
+gzip compressed data, was "elhub_python_sdk-0.1.5.tar", max compression
```

## Comparing `elhub_python_sdk-0.1.4.tar` & `elhub_python_sdk-0.1.5.tar`

### file list

```diff
@@ -1,105 +1,106 @@
--rw-r--r--   0        0        0     7652 2023-04-27 10:56:54.310448 elhub_python_sdk-0.1.4/LICENSE
--rw-r--r--   0        0        0     1283 2023-04-27 10:56:54.310448 elhub_python_sdk-0.1.4/README.md
--rw-r--r--   0        0        0      130 2023-04-27 10:56:54.310448 elhub_python_sdk-0.1.4/elhub_sdk/__init__.py
--rw-r--r--   0        0        0     3684 2023-04-27 10:56:54.310448 elhub_python_sdk-0.1.4/elhub_sdk/client.py
--rw-r--r--   0        0        0       92 2023-04-27 10:56:54.310448 elhub_python_sdk-0.1.4/elhub_sdk/constants.py
--rw-r--r--   0        0        0     5777 2023-04-27 10:56:54.310448 elhub_python_sdk-0.1.4/elhub_sdk/consumption.py
--rw-r--r--   0        0        0     3269 2023-04-27 10:56:54.314448 elhub_python_sdk-0.1.4/elhub_sdk/enrollment.py
--rw-r--r--   0        0        0     1453 2023-04-27 10:56:54.314448 elhub_python_sdk-0.1.4/elhub_sdk/enums.py
--rw-r--r--   0        0        0     1522 2023-04-27 10:56:54.314448 elhub_python_sdk-0.1.4/elhub_sdk/settings.py
--rw-r--r--   0        0        0     3783 2023-04-27 10:56:54.314448 elhub_python_sdk-0.1.4/elhub_sdk/third_party.py
--rw-r--r--   0        0        0     1033 2023-04-27 10:56:54.314448 elhub_python_sdk-0.1.4/elhub_sdk/wsdl/prod/2.3/bim/Acknowledgement.xsd
--rw-r--r--   0        0        0      996 2023-04-27 10:56:54.314448 elhub_python_sdk-0.1.4/elhub_sdk/wsdl/prod/2.3/bim/PollForData.xsd
--rw-r--r--   0        0        0    43445 2023-04-27 10:56:54.314448 elhub_python_sdk-0.1.4/elhub_sdk/wsdl/prod/2.3/bim/common/Elhub_AggregatedBusinessInformationEntities.xsd
--rw-r--r--   0        0        0    42145 2023-04-27 10:56:54.314448 elhub_python_sdk-0.1.4/elhub_sdk/wsdl/prod/2.3/bim/common/Elhub_BusinessDataType.xsd
--rw-r--r--   0        0        0     1072 2023-04-27 10:56:54.314448 elhub_python_sdk-0.1.4/elhub_sdk/wsdl/prod/2.3/bim/market/ConfirmEndOfSupply.xsd
--rw-r--r--   0        0        0     1084 2023-04-27 10:56:54.314448 elhub_python_sdk-0.1.4/elhub_sdk/wsdl/prod/2.3/bim/market/ConfirmStartOfSupply.xsd
--rw-r--r--   0        0        0     1065 2023-04-27 10:56:54.314448 elhub_python_sdk-0.1.4/elhub_sdk/wsdl/prod/2.3/bim/market/NotifyEndOfSupply.xsd
--rw-r--r--   0        0        0     1077 2023-04-27 10:56:54.314448 elhub_python_sdk-0.1.4/elhub_sdk/wsdl/prod/2.3/bim/market/NotifyStartOfSupply.xsd
--rw-r--r--   0        0        0     1068 2023-04-27 10:56:54.314448 elhub_python_sdk-0.1.4/elhub_sdk/wsdl/prod/2.3/bim/market/RejectEndOfSupply.xsd
--rw-r--r--   0        0        0     1078 2023-04-27 10:56:54.314448 elhub_python_sdk-0.1.4/elhub_sdk/wsdl/prod/2.3/bim/market/RejectStartOfSupply.xsd
--rw-r--r--   0        0        0     1066 2023-04-27 10:56:54.314448 elhub_python_sdk-0.1.4/elhub_sdk/wsdl/prod/2.3/bim/market/RequestEndOfSupply.xsd
--rw-r--r--   0        0        0     1078 2023-04-27 10:56:54.314448 elhub_python_sdk-0.1.4/elhub_sdk/wsdl/prod/2.3/bim/market/RequestStartOfSupply.xsd
--rw-r--r--   0        0        0     1126 2023-04-27 10:56:54.314448 elhub_python_sdk-0.1.4/elhub_sdk/wsdl/prod/2.3/bim/masterdata/NotifyCustomerInformation.xsd
--rw-r--r--   0        0        0     1188 2023-04-27 10:56:54.314448 elhub_python_sdk-0.1.4/elhub_sdk/wsdl/prod/2.3/bim/masterdata/NotifyMeteringPointCharacteristics.xsd
--rw-r--r--   0        0        0     1168 2023-04-27 10:56:54.314448 elhub_python_sdk-0.1.4/elhub_sdk/wsdl/prod/2.3/bim/masterdata/RequestUpdateCustomerInformation.xsd
--rw-r--r--   0        0        0     1393 2023-04-27 10:56:54.314448 elhub_python_sdk-0.1.4/elhub_sdk/wsdl/prod/2.3/bim/masterdata/RequestUpdateMasterDataMeteringPoint.xsd
--rw-r--r--   0        0        0     1415 2023-04-27 10:56:54.314448 elhub_python_sdk-0.1.4/elhub_sdk/wsdl/prod/2.3/bim/metering/CollectedData.xsd
--rw-r--r--   0        0        0     1184 2023-04-27 10:56:54.314448 elhub_python_sdk-0.1.4/elhub_sdk/wsdl/prod/2.3/bim/metering/NotifyValidatedDataForBillingEnergy.xsd
--rw-r--r--   0        0        0     1207 2023-04-27 10:56:54.314448 elhub_python_sdk-0.1.4/elhub_sdk/wsdl/prod/2.3/bim/metering/PriceVolumeCombinationForReconciliation.xsd
--rw-r--r--   0        0        0     1094 2023-04-27 10:56:54.314448 elhub_python_sdk-0.1.4/elhub_sdk/wsdl/prod/2.3/bim/metering/RequestCollectedData.xsd
--rw-r--r--   0        0        0     1076 2023-04-27 10:56:54.314448 elhub_python_sdk-0.1.4/elhub_sdk/wsdl/prod/2.3/bim/query/RequestDataFromElhub.xsd
--rw-r--r--   0        0        0     1040 2023-04-27 10:56:54.314448 elhub_python_sdk-0.1.4/elhub_sdk/wsdl/prod/2.3/bim/query/RequestToElhub.xsd
--rw-r--r--   0        0        0     1118 2023-04-27 10:56:54.314448 elhub_python_sdk-0.1.4/elhub_sdk/wsdl/prod/2.3/bim/query/RequestToGridAccessProvider.xsd
--rw-r--r--   0        0        0     1208 2023-04-27 10:56:54.314448 elhub_python_sdk-0.1.4/elhub_sdk/wsdl/prod/2.3/bim/query/RequestUpfrontMeteringPointCharacteristics.xsd
--rw-r--r--   0        0        0     1064 2023-04-27 10:56:54.314448 elhub_python_sdk-0.1.4/elhub_sdk/wsdl/prod/2.3/bim/query/ResponseFromElhub.xsd
--rw-r--r--   0        0        0     1142 2023-04-27 10:56:54.314448 elhub_python_sdk-0.1.4/elhub_sdk/wsdl/prod/2.3/bim/query/ResponseFromGridAccessProvider.xsd
--rw-r--r--   0        0        0     1225 2023-04-27 10:56:54.314448 elhub_python_sdk-0.1.4/elhub_sdk/wsdl/prod/2.3/bim/query/ResponseUpfrontMeteringPointCharacteristics.xsd
--rw-r--r--   0        0        0     1110 2023-04-27 10:56:54.314448 elhub_python_sdk-0.1.4/elhub_sdk/wsdl/prod/2.3/bim/thirdpartyaccess/UpdateThirdPartyAccess.xsd
--rw-r--r--   0        0        0    43165 2023-04-27 10:56:54.314448 elhub_python_sdk-0.1.4/elhub_sdk/wsdl/prod/2.3/bim v22 sorted/Elhub_AggregatedBusinessInformationEntities_v22_sorted.xsd
--rw-r--r--   0        0        0        0 2023-04-27 10:56:54.314448 elhub_python_sdk-0.1.4/elhub_sdk/wsdl/prod/2.3/bim v22 sorted/Elhub_BusinessDataType_v22_sorted.xsd
--rw-r--r--   0        0        0   126666 2023-04-27 10:56:54.314448 elhub_python_sdk-0.1.4/elhub_sdk/wsdl/prod/2.3/bindings/jaxb_numeric.xml
--rw-r--r--   0        0        0    12376 2023-04-27 10:56:54.314448 elhub_python_sdk-0.1.4/elhub_sdk/wsdl/prod/2.3/wsdl/MarketProcesses - WS-Security.wsdl
--rw-r--r--   0        0        0     6742 2023-04-27 10:56:54.314448 elhub_python_sdk-0.1.4/elhub_sdk/wsdl/prod/2.3/wsdl/MeteringValues - WS-Security.wsdl
--rw-r--r--   0        0        0     6972 2023-04-27 10:56:54.314448 elhub_python_sdk-0.1.4/elhub_sdk/wsdl/prod/2.3/wsdl/PollMarketProcesses - WS-Security.wsdl
--rw-r--r--   0        0        0     6961 2023-04-27 10:56:54.314448 elhub_python_sdk-0.1.4/elhub_sdk/wsdl/prod/2.3/wsdl/PollMeteringValues - WS-Security.wsdl
--rw-r--r--   0        0        0    11193 2023-04-27 10:56:54.314448 elhub_python_sdk-0.1.4/elhub_sdk/wsdl/prod/2.3/wsdl/Query - WS-Security.wsdl
--rw-r--r--   0        0        0     3056 2023-04-27 10:56:54.314448 elhub_python_sdk-0.1.4/elhub_sdk/wsdl/prod/2.3/wsdl/xsd/MarketProcesses.xsd
--rw-r--r--   0        0        0     1159 2023-04-27 10:56:54.314448 elhub_python_sdk-0.1.4/elhub_sdk/wsdl/prod/2.3/wsdl/xsd/MeteringValues.xsd
--rw-r--r--   0        0        0     6206 2023-04-27 10:56:54.314448 elhub_python_sdk-0.1.4/elhub_sdk/wsdl/prod/2.3/wsdl/xsd/PollMarketProcesses.xsd
--rw-r--r--   0        0        0     3176 2023-04-27 10:56:54.314448 elhub_python_sdk-0.1.4/elhub_sdk/wsdl/prod/2.3/wsdl/xsd/PollMeteringValues.xsd
--rw-r--r--   0        0        0     3263 2023-04-27 10:56:54.314448 elhub_python_sdk-0.1.4/elhub_sdk/wsdl/prod/2.3/wsdl/xsd/Query.xsd
--rw-r--r--   0        0        0     1613 2023-04-27 10:56:54.314448 elhub_python_sdk-0.1.4/elhub_sdk/wsdl/prod/2.3/wsdl/xsd/common.xsd
--rw-r--r--   0        0        0     1033 2023-04-27 10:56:54.314448 elhub_python_sdk-0.1.4/elhub_sdk/wsdl/test/2.3/bim/Acknowledgement.xsd
--rw-r--r--   0        0        0      996 2023-04-27 10:56:54.314448 elhub_python_sdk-0.1.4/elhub_sdk/wsdl/test/2.3/bim/PollForData.xsd
--rw-r--r--   0        0        0    43445 2023-04-27 10:56:54.314448 elhub_python_sdk-0.1.4/elhub_sdk/wsdl/test/2.3/bim/common/Elhub_AggregatedBusinessInformationEntities.xsd
--rw-r--r--   0        0        0    42145 2023-04-27 10:56:54.314448 elhub_python_sdk-0.1.4/elhub_sdk/wsdl/test/2.3/bim/common/Elhub_BusinessDataType.xsd
--rw-r--r--   0        0        0     1072 2023-04-27 10:56:54.314448 elhub_python_sdk-0.1.4/elhub_sdk/wsdl/test/2.3/bim/market/ConfirmEndOfSupply.xsd
--rw-r--r--   0        0        0     1084 2023-04-27 10:56:54.314448 elhub_python_sdk-0.1.4/elhub_sdk/wsdl/test/2.3/bim/market/ConfirmStartOfSupply.xsd
--rw-r--r--   0        0        0     1065 2023-04-27 10:56:54.314448 elhub_python_sdk-0.1.4/elhub_sdk/wsdl/test/2.3/bim/market/NotifyEndOfSupply.xsd
--rw-r--r--   0        0        0     1077 2023-04-27 10:56:54.314448 elhub_python_sdk-0.1.4/elhub_sdk/wsdl/test/2.3/bim/market/NotifyStartOfSupply.xsd
--rw-r--r--   0        0        0     1068 2023-04-27 10:56:54.314448 elhub_python_sdk-0.1.4/elhub_sdk/wsdl/test/2.3/bim/market/RejectEndOfSupply.xsd
--rw-r--r--   0        0        0     1078 2023-04-27 10:56:54.314448 elhub_python_sdk-0.1.4/elhub_sdk/wsdl/test/2.3/bim/market/RejectStartOfSupply.xsd
--rw-r--r--   0        0        0     1066 2023-04-27 10:56:54.314448 elhub_python_sdk-0.1.4/elhub_sdk/wsdl/test/2.3/bim/market/RequestEndOfSupply.xsd
--rw-r--r--   0        0        0     1078 2023-04-27 10:56:54.314448 elhub_python_sdk-0.1.4/elhub_sdk/wsdl/test/2.3/bim/market/RequestStartOfSupply.xsd
--rw-r--r--   0        0        0     1126 2023-04-27 10:56:54.314448 elhub_python_sdk-0.1.4/elhub_sdk/wsdl/test/2.3/bim/masterdata/NotifyCustomerInformation.xsd
--rw-r--r--   0        0        0     1188 2023-04-27 10:56:54.314448 elhub_python_sdk-0.1.4/elhub_sdk/wsdl/test/2.3/bim/masterdata/NotifyMeteringPointCharacteristics.xsd
--rw-r--r--   0        0        0     1168 2023-04-27 10:56:54.314448 elhub_python_sdk-0.1.4/elhub_sdk/wsdl/test/2.3/bim/masterdata/RequestUpdateCustomerInformation.xsd
--rw-r--r--   0        0        0     1393 2023-04-27 10:56:54.314448 elhub_python_sdk-0.1.4/elhub_sdk/wsdl/test/2.3/bim/masterdata/RequestUpdateMasterDataMeteringPoint.xsd
--rw-r--r--   0        0        0     1415 2023-04-27 10:56:54.314448 elhub_python_sdk-0.1.4/elhub_sdk/wsdl/test/2.3/bim/metering/CollectedData.xsd
--rw-r--r--   0        0        0     1184 2023-04-27 10:56:54.314448 elhub_python_sdk-0.1.4/elhub_sdk/wsdl/test/2.3/bim/metering/NotifyValidatedDataForBillingEnergy.xsd
--rw-r--r--   0        0        0     1207 2023-04-27 10:56:54.314448 elhub_python_sdk-0.1.4/elhub_sdk/wsdl/test/2.3/bim/metering/PriceVolumeCombinationForReconciliation.xsd
--rw-r--r--   0        0        0     1094 2023-04-27 10:56:54.314448 elhub_python_sdk-0.1.4/elhub_sdk/wsdl/test/2.3/bim/metering/RequestCollectedData.xsd
--rw-r--r--   0        0        0     1076 2023-04-27 10:56:54.314448 elhub_python_sdk-0.1.4/elhub_sdk/wsdl/test/2.3/bim/query/RequestDataFromElhub.xsd
--rw-r--r--   0        0        0     1040 2023-04-27 10:56:54.314448 elhub_python_sdk-0.1.4/elhub_sdk/wsdl/test/2.3/bim/query/RequestToElhub.xsd
--rw-r--r--   0        0        0     1118 2023-04-27 10:56:54.314448 elhub_python_sdk-0.1.4/elhub_sdk/wsdl/test/2.3/bim/query/RequestToGridAccessProvider.xsd
--rw-r--r--   0        0        0     1208 2023-04-27 10:56:54.314448 elhub_python_sdk-0.1.4/elhub_sdk/wsdl/test/2.3/bim/query/RequestUpfrontMeteringPointCharacteristics.xsd
--rw-r--r--   0        0        0     1064 2023-04-27 10:56:54.314448 elhub_python_sdk-0.1.4/elhub_sdk/wsdl/test/2.3/bim/query/ResponseFromElhub.xsd
--rw-r--r--   0        0        0     1142 2023-04-27 10:56:54.314448 elhub_python_sdk-0.1.4/elhub_sdk/wsdl/test/2.3/bim/query/ResponseFromGridAccessProvider.xsd
--rw-r--r--   0        0        0     1225 2023-04-27 10:56:54.314448 elhub_python_sdk-0.1.4/elhub_sdk/wsdl/test/2.3/bim/query/ResponseUpfrontMeteringPointCharacteristics.xsd
--rw-r--r--   0        0        0     1110 2023-04-27 10:56:54.314448 elhub_python_sdk-0.1.4/elhub_sdk/wsdl/test/2.3/bim/thirdpartyaccess/UpdateThirdPartyAccess.xsd
--rw-r--r--   0        0        0    43165 2023-04-27 10:56:54.314448 elhub_python_sdk-0.1.4/elhub_sdk/wsdl/test/2.3/bim v22 sorted/Elhub_AggregatedBusinessInformationEntities_v22_sorted.xsd
--rw-r--r--   0        0        0        0 2023-04-27 10:56:54.314448 elhub_python_sdk-0.1.4/elhub_sdk/wsdl/test/2.3/bim v22 sorted/Elhub_BusinessDataType_v22_sorted.xsd
--rw-r--r--   0        0        0   126666 2023-04-27 10:56:54.314448 elhub_python_sdk-0.1.4/elhub_sdk/wsdl/test/2.3/bindings/jaxb_numeric.xml
--rw-r--r--   0        0        0    12375 2023-04-27 10:56:54.314448 elhub_python_sdk-0.1.4/elhub_sdk/wsdl/test/2.3/wsdl/MarketProcesses - WS-Security.wsdl
--rw-r--r--   0        0        0     6741 2023-04-27 10:56:54.314448 elhub_python_sdk-0.1.4/elhub_sdk/wsdl/test/2.3/wsdl/MeteringValues - WS-Security.wsdl
--rw-r--r--   0        0        0     6971 2023-04-27 10:56:54.314448 elhub_python_sdk-0.1.4/elhub_sdk/wsdl/test/2.3/wsdl/PollMarketProcesses - WS-Security.wsdl
--rw-r--r--   0        0        0     6960 2023-04-27 10:56:54.314448 elhub_python_sdk-0.1.4/elhub_sdk/wsdl/test/2.3/wsdl/PollMeteringValues - WS-Security.wsdl
--rw-r--r--   0        0        0    11192 2023-04-27 10:56:54.314448 elhub_python_sdk-0.1.4/elhub_sdk/wsdl/test/2.3/wsdl/Query - WS-Security.wsdl
--rw-r--r--   0        0        0     3056 2023-04-27 10:56:54.314448 elhub_python_sdk-0.1.4/elhub_sdk/wsdl/test/2.3/wsdl/xsd/MarketProcesses.xsd
--rw-r--r--   0        0        0     1159 2023-04-27 10:56:54.314448 elhub_python_sdk-0.1.4/elhub_sdk/wsdl/test/2.3/wsdl/xsd/MeteringValues.xsd
--rw-r--r--   0        0        0     6206 2023-04-27 10:56:54.314448 elhub_python_sdk-0.1.4/elhub_sdk/wsdl/test/2.3/wsdl/xsd/PollMarketProcesses.xsd
--rw-r--r--   0        0        0     3176 2023-04-27 10:56:54.314448 elhub_python_sdk-0.1.4/elhub_sdk/wsdl/test/2.3/wsdl/xsd/PollMeteringValues.xsd
--rw-r--r--   0        0        0     3263 2023-04-27 10:56:54.314448 elhub_python_sdk-0.1.4/elhub_sdk/wsdl/test/2.3/wsdl/xsd/Query.xsd
--rw-r--r--   0        0        0     1613 2023-04-27 10:56:54.314448 elhub_python_sdk-0.1.4/elhub_sdk/wsdl/test/2.3/wsdl/xsd/common.xsd
--rw-r--r--   0        0        0     2506 2023-04-27 10:56:54.314448 elhub_python_sdk-0.1.4/pyproject.toml
--rw-r--r--   0        0        0       46 2023-04-27 10:56:54.314448 elhub_python_sdk-0.1.4/tests/__init__.py
--rw-r--r--   0        0        0     3218 2023-04-27 10:56:54.314448 elhub_python_sdk-0.1.4/tests/test_integration.py
--rw-r--r--   0        0        0     3914 2023-04-27 10:56:54.318448 elhub_python_sdk-0.1.4/tests/test_integration_soap.py
--rw-r--r--   0        0        0      283 2023-04-27 10:56:54.318448 elhub_python_sdk-0.1.4/tests/tests_examples/README.md
--rw-r--r--   0        0        0        0 2023-04-27 10:56:54.318448 elhub_python_sdk-0.1.4/tests/tests_examples/__init__.py
--rw-r--r--   0        0        0      932 2023-04-27 10:56:54.318448 elhub_python_sdk-0.1.4/tests/tests_examples/ag611-01-actor-test.py
--rw-r--r--   0        0        0     1987 2023-04-27 10:56:54.318448 elhub_python_sdk-0.1.4/tests/tests_examples/ag622-01-actor-test.py
--rw-r--r--   0        0        0     1966 2023-04-27 10:56:54.318448 elhub_python_sdk-0.1.4/tests/tests_examples/ag622-02-actor-test.py
--rw-r--r--   0        0        0      401 2023-04-27 10:56:54.318448 elhub_python_sdk-0.1.4/tests/tests_examples/config.py
--rw-r--r--   0        0        0     3573 1970-01-01 00:00:00.000000 elhub_python_sdk-0.1.4/PKG-INFO
+-rw-r--r--   0        0        0     7652 2023-07-21 06:57:20.395249 elhub_python_sdk-0.1.5/LICENSE
+-rw-r--r--   0        0        0     1283 2023-07-21 06:57:20.395249 elhub_python_sdk-0.1.5/README.md
+-rw-r--r--   0        0        0      130 2023-07-21 06:57:20.395249 elhub_python_sdk-0.1.5/elhub_sdk/__init__.py
+-rw-r--r--   0        0        0     3544 2023-07-21 06:57:20.395249 elhub_python_sdk-0.1.5/elhub_sdk/acknolwedgment.py
+-rw-r--r--   0        0        0     3684 2023-07-21 06:57:20.395249 elhub_python_sdk-0.1.5/elhub_sdk/client.py
+-rw-r--r--   0        0        0       92 2023-07-21 06:57:20.395249 elhub_python_sdk-0.1.5/elhub_sdk/constants.py
+-rw-r--r--   0        0        0     5777 2023-07-21 06:57:20.399249 elhub_python_sdk-0.1.5/elhub_sdk/consumption.py
+-rw-r--r--   0        0        0     3269 2023-07-21 06:57:20.399249 elhub_python_sdk-0.1.5/elhub_sdk/enrollment.py
+-rw-r--r--   0        0        0     1607 2023-07-21 06:57:20.399249 elhub_python_sdk-0.1.5/elhub_sdk/enums.py
+-rw-r--r--   0        0        0     1522 2023-07-21 06:57:20.399249 elhub_python_sdk-0.1.5/elhub_sdk/settings.py
+-rw-r--r--   0        0        0     3783 2023-07-21 06:57:20.399249 elhub_python_sdk-0.1.5/elhub_sdk/third_party.py
+-rw-r--r--   0        0        0     1033 2023-07-21 06:57:20.399249 elhub_python_sdk-0.1.5/elhub_sdk/wsdl/prod/2.3/bim/Acknowledgement.xsd
+-rw-r--r--   0        0        0      996 2023-07-21 06:57:20.399249 elhub_python_sdk-0.1.5/elhub_sdk/wsdl/prod/2.3/bim/PollForData.xsd
+-rw-r--r--   0        0        0    43445 2023-07-21 06:57:20.399249 elhub_python_sdk-0.1.5/elhub_sdk/wsdl/prod/2.3/bim/common/Elhub_AggregatedBusinessInformationEntities.xsd
+-rw-r--r--   0        0        0    42145 2023-07-21 06:57:20.399249 elhub_python_sdk-0.1.5/elhub_sdk/wsdl/prod/2.3/bim/common/Elhub_BusinessDataType.xsd
+-rw-r--r--   0        0        0     1072 2023-07-21 06:57:20.399249 elhub_python_sdk-0.1.5/elhub_sdk/wsdl/prod/2.3/bim/market/ConfirmEndOfSupply.xsd
+-rw-r--r--   0        0        0     1084 2023-07-21 06:57:20.399249 elhub_python_sdk-0.1.5/elhub_sdk/wsdl/prod/2.3/bim/market/ConfirmStartOfSupply.xsd
+-rw-r--r--   0        0        0     1065 2023-07-21 06:57:20.399249 elhub_python_sdk-0.1.5/elhub_sdk/wsdl/prod/2.3/bim/market/NotifyEndOfSupply.xsd
+-rw-r--r--   0        0        0     1077 2023-07-21 06:57:20.399249 elhub_python_sdk-0.1.5/elhub_sdk/wsdl/prod/2.3/bim/market/NotifyStartOfSupply.xsd
+-rw-r--r--   0        0        0     1068 2023-07-21 06:57:20.399249 elhub_python_sdk-0.1.5/elhub_sdk/wsdl/prod/2.3/bim/market/RejectEndOfSupply.xsd
+-rw-r--r--   0        0        0     1078 2023-07-21 06:57:20.399249 elhub_python_sdk-0.1.5/elhub_sdk/wsdl/prod/2.3/bim/market/RejectStartOfSupply.xsd
+-rw-r--r--   0        0        0     1066 2023-07-21 06:57:20.399249 elhub_python_sdk-0.1.5/elhub_sdk/wsdl/prod/2.3/bim/market/RequestEndOfSupply.xsd
+-rw-r--r--   0        0        0     1078 2023-07-21 06:57:20.399249 elhub_python_sdk-0.1.5/elhub_sdk/wsdl/prod/2.3/bim/market/RequestStartOfSupply.xsd
+-rw-r--r--   0        0        0     1126 2023-07-21 06:57:20.399249 elhub_python_sdk-0.1.5/elhub_sdk/wsdl/prod/2.3/bim/masterdata/NotifyCustomerInformation.xsd
+-rw-r--r--   0        0        0     1188 2023-07-21 06:57:20.399249 elhub_python_sdk-0.1.5/elhub_sdk/wsdl/prod/2.3/bim/masterdata/NotifyMeteringPointCharacteristics.xsd
+-rw-r--r--   0        0        0     1168 2023-07-21 06:57:20.399249 elhub_python_sdk-0.1.5/elhub_sdk/wsdl/prod/2.3/bim/masterdata/RequestUpdateCustomerInformation.xsd
+-rw-r--r--   0        0        0     1393 2023-07-21 06:57:20.399249 elhub_python_sdk-0.1.5/elhub_sdk/wsdl/prod/2.3/bim/masterdata/RequestUpdateMasterDataMeteringPoint.xsd
+-rw-r--r--   0        0        0     1415 2023-07-21 06:57:20.399249 elhub_python_sdk-0.1.5/elhub_sdk/wsdl/prod/2.3/bim/metering/CollectedData.xsd
+-rw-r--r--   0        0        0     1184 2023-07-21 06:57:20.399249 elhub_python_sdk-0.1.5/elhub_sdk/wsdl/prod/2.3/bim/metering/NotifyValidatedDataForBillingEnergy.xsd
+-rw-r--r--   0        0        0     1207 2023-07-21 06:57:20.399249 elhub_python_sdk-0.1.5/elhub_sdk/wsdl/prod/2.3/bim/metering/PriceVolumeCombinationForReconciliation.xsd
+-rw-r--r--   0        0        0     1094 2023-07-21 06:57:20.399249 elhub_python_sdk-0.1.5/elhub_sdk/wsdl/prod/2.3/bim/metering/RequestCollectedData.xsd
+-rw-r--r--   0        0        0     1076 2023-07-21 06:57:20.399249 elhub_python_sdk-0.1.5/elhub_sdk/wsdl/prod/2.3/bim/query/RequestDataFromElhub.xsd
+-rw-r--r--   0        0        0     1040 2023-07-21 06:57:20.399249 elhub_python_sdk-0.1.5/elhub_sdk/wsdl/prod/2.3/bim/query/RequestToElhub.xsd
+-rw-r--r--   0        0        0     1118 2023-07-21 06:57:20.399249 elhub_python_sdk-0.1.5/elhub_sdk/wsdl/prod/2.3/bim/query/RequestToGridAccessProvider.xsd
+-rw-r--r--   0        0        0     1208 2023-07-21 06:57:20.399249 elhub_python_sdk-0.1.5/elhub_sdk/wsdl/prod/2.3/bim/query/RequestUpfrontMeteringPointCharacteristics.xsd
+-rw-r--r--   0        0        0     1064 2023-07-21 06:57:20.399249 elhub_python_sdk-0.1.5/elhub_sdk/wsdl/prod/2.3/bim/query/ResponseFromElhub.xsd
+-rw-r--r--   0        0        0     1142 2023-07-21 06:57:20.399249 elhub_python_sdk-0.1.5/elhub_sdk/wsdl/prod/2.3/bim/query/ResponseFromGridAccessProvider.xsd
+-rw-r--r--   0        0        0     1225 2023-07-21 06:57:20.399249 elhub_python_sdk-0.1.5/elhub_sdk/wsdl/prod/2.3/bim/query/ResponseUpfrontMeteringPointCharacteristics.xsd
+-rw-r--r--   0        0        0     1110 2023-07-21 06:57:20.399249 elhub_python_sdk-0.1.5/elhub_sdk/wsdl/prod/2.3/bim/thirdpartyaccess/UpdateThirdPartyAccess.xsd
+-rw-r--r--   0        0        0    43165 2023-07-21 06:57:20.399249 elhub_python_sdk-0.1.5/elhub_sdk/wsdl/prod/2.3/bim v22 sorted/Elhub_AggregatedBusinessInformationEntities_v22_sorted.xsd
+-rw-r--r--   0        0        0        0 2023-07-21 06:57:20.399249 elhub_python_sdk-0.1.5/elhub_sdk/wsdl/prod/2.3/bim v22 sorted/Elhub_BusinessDataType_v22_sorted.xsd
+-rw-r--r--   0        0        0   126666 2023-07-21 06:57:20.399249 elhub_python_sdk-0.1.5/elhub_sdk/wsdl/prod/2.3/bindings/jaxb_numeric.xml
+-rw-r--r--   0        0        0    12376 2023-07-21 06:57:20.399249 elhub_python_sdk-0.1.5/elhub_sdk/wsdl/prod/2.3/wsdl/MarketProcesses - WS-Security.wsdl
+-rw-r--r--   0        0        0     6742 2023-07-21 06:57:20.399249 elhub_python_sdk-0.1.5/elhub_sdk/wsdl/prod/2.3/wsdl/MeteringValues - WS-Security.wsdl
+-rw-r--r--   0        0        0     6972 2023-07-21 06:57:20.399249 elhub_python_sdk-0.1.5/elhub_sdk/wsdl/prod/2.3/wsdl/PollMarketProcesses - WS-Security.wsdl
+-rw-r--r--   0        0        0     6961 2023-07-21 06:57:20.399249 elhub_python_sdk-0.1.5/elhub_sdk/wsdl/prod/2.3/wsdl/PollMeteringValues - WS-Security.wsdl
+-rw-r--r--   0        0        0    11193 2023-07-21 06:57:20.399249 elhub_python_sdk-0.1.5/elhub_sdk/wsdl/prod/2.3/wsdl/Query - WS-Security.wsdl
+-rw-r--r--   0        0        0     3056 2023-07-21 06:57:20.399249 elhub_python_sdk-0.1.5/elhub_sdk/wsdl/prod/2.3/wsdl/xsd/MarketProcesses.xsd
+-rw-r--r--   0        0        0     1159 2023-07-21 06:57:20.399249 elhub_python_sdk-0.1.5/elhub_sdk/wsdl/prod/2.3/wsdl/xsd/MeteringValues.xsd
+-rw-r--r--   0        0        0     6206 2023-07-21 06:57:20.399249 elhub_python_sdk-0.1.5/elhub_sdk/wsdl/prod/2.3/wsdl/xsd/PollMarketProcesses.xsd
+-rw-r--r--   0        0        0     3176 2023-07-21 06:57:20.399249 elhub_python_sdk-0.1.5/elhub_sdk/wsdl/prod/2.3/wsdl/xsd/PollMeteringValues.xsd
+-rw-r--r--   0        0        0     3263 2023-07-21 06:57:20.399249 elhub_python_sdk-0.1.5/elhub_sdk/wsdl/prod/2.3/wsdl/xsd/Query.xsd
+-rw-r--r--   0        0        0     1613 2023-07-21 06:57:20.399249 elhub_python_sdk-0.1.5/elhub_sdk/wsdl/prod/2.3/wsdl/xsd/common.xsd
+-rw-r--r--   0        0        0     1033 2023-07-21 06:57:20.399249 elhub_python_sdk-0.1.5/elhub_sdk/wsdl/test/2.3/bim/Acknowledgement.xsd
+-rw-r--r--   0        0        0      996 2023-07-21 06:57:20.399249 elhub_python_sdk-0.1.5/elhub_sdk/wsdl/test/2.3/bim/PollForData.xsd
+-rw-r--r--   0        0        0    43445 2023-07-21 06:57:20.399249 elhub_python_sdk-0.1.5/elhub_sdk/wsdl/test/2.3/bim/common/Elhub_AggregatedBusinessInformationEntities.xsd
+-rw-r--r--   0        0        0    42145 2023-07-21 06:57:20.399249 elhub_python_sdk-0.1.5/elhub_sdk/wsdl/test/2.3/bim/common/Elhub_BusinessDataType.xsd
+-rw-r--r--   0        0        0     1072 2023-07-21 06:57:20.399249 elhub_python_sdk-0.1.5/elhub_sdk/wsdl/test/2.3/bim/market/ConfirmEndOfSupply.xsd
+-rw-r--r--   0        0        0     1084 2023-07-21 06:57:20.399249 elhub_python_sdk-0.1.5/elhub_sdk/wsdl/test/2.3/bim/market/ConfirmStartOfSupply.xsd
+-rw-r--r--   0        0        0     1065 2023-07-21 06:57:20.399249 elhub_python_sdk-0.1.5/elhub_sdk/wsdl/test/2.3/bim/market/NotifyEndOfSupply.xsd
+-rw-r--r--   0        0        0     1077 2023-07-21 06:57:20.399249 elhub_python_sdk-0.1.5/elhub_sdk/wsdl/test/2.3/bim/market/NotifyStartOfSupply.xsd
+-rw-r--r--   0        0        0     1068 2023-07-21 06:57:20.399249 elhub_python_sdk-0.1.5/elhub_sdk/wsdl/test/2.3/bim/market/RejectEndOfSupply.xsd
+-rw-r--r--   0        0        0     1078 2023-07-21 06:57:20.399249 elhub_python_sdk-0.1.5/elhub_sdk/wsdl/test/2.3/bim/market/RejectStartOfSupply.xsd
+-rw-r--r--   0        0        0     1066 2023-07-21 06:57:20.399249 elhub_python_sdk-0.1.5/elhub_sdk/wsdl/test/2.3/bim/market/RequestEndOfSupply.xsd
+-rw-r--r--   0        0        0     1078 2023-07-21 06:57:20.399249 elhub_python_sdk-0.1.5/elhub_sdk/wsdl/test/2.3/bim/market/RequestStartOfSupply.xsd
+-rw-r--r--   0        0        0     1126 2023-07-21 06:57:20.399249 elhub_python_sdk-0.1.5/elhub_sdk/wsdl/test/2.3/bim/masterdata/NotifyCustomerInformation.xsd
+-rw-r--r--   0        0        0     1188 2023-07-21 06:57:20.399249 elhub_python_sdk-0.1.5/elhub_sdk/wsdl/test/2.3/bim/masterdata/NotifyMeteringPointCharacteristics.xsd
+-rw-r--r--   0        0        0     1168 2023-07-21 06:57:20.399249 elhub_python_sdk-0.1.5/elhub_sdk/wsdl/test/2.3/bim/masterdata/RequestUpdateCustomerInformation.xsd
+-rw-r--r--   0        0        0     1393 2023-07-21 06:57:20.399249 elhub_python_sdk-0.1.5/elhub_sdk/wsdl/test/2.3/bim/masterdata/RequestUpdateMasterDataMeteringPoint.xsd
+-rw-r--r--   0        0        0     1415 2023-07-21 06:57:20.399249 elhub_python_sdk-0.1.5/elhub_sdk/wsdl/test/2.3/bim/metering/CollectedData.xsd
+-rw-r--r--   0        0        0     1184 2023-07-21 06:57:20.399249 elhub_python_sdk-0.1.5/elhub_sdk/wsdl/test/2.3/bim/metering/NotifyValidatedDataForBillingEnergy.xsd
+-rw-r--r--   0        0        0     1207 2023-07-21 06:57:20.399249 elhub_python_sdk-0.1.5/elhub_sdk/wsdl/test/2.3/bim/metering/PriceVolumeCombinationForReconciliation.xsd
+-rw-r--r--   0        0        0     1094 2023-07-21 06:57:20.399249 elhub_python_sdk-0.1.5/elhub_sdk/wsdl/test/2.3/bim/metering/RequestCollectedData.xsd
+-rw-r--r--   0        0        0     1076 2023-07-21 06:57:20.399249 elhub_python_sdk-0.1.5/elhub_sdk/wsdl/test/2.3/bim/query/RequestDataFromElhub.xsd
+-rw-r--r--   0        0        0     1040 2023-07-21 06:57:20.399249 elhub_python_sdk-0.1.5/elhub_sdk/wsdl/test/2.3/bim/query/RequestToElhub.xsd
+-rw-r--r--   0        0        0     1118 2023-07-21 06:57:20.399249 elhub_python_sdk-0.1.5/elhub_sdk/wsdl/test/2.3/bim/query/RequestToGridAccessProvider.xsd
+-rw-r--r--   0        0        0     1208 2023-07-21 06:57:20.399249 elhub_python_sdk-0.1.5/elhub_sdk/wsdl/test/2.3/bim/query/RequestUpfrontMeteringPointCharacteristics.xsd
+-rw-r--r--   0        0        0     1064 2023-07-21 06:57:20.399249 elhub_python_sdk-0.1.5/elhub_sdk/wsdl/test/2.3/bim/query/ResponseFromElhub.xsd
+-rw-r--r--   0        0        0     1142 2023-07-21 06:57:20.399249 elhub_python_sdk-0.1.5/elhub_sdk/wsdl/test/2.3/bim/query/ResponseFromGridAccessProvider.xsd
+-rw-r--r--   0        0        0     1225 2023-07-21 06:57:20.399249 elhub_python_sdk-0.1.5/elhub_sdk/wsdl/test/2.3/bim/query/ResponseUpfrontMeteringPointCharacteristics.xsd
+-rw-r--r--   0        0        0     1110 2023-07-21 06:57:20.399249 elhub_python_sdk-0.1.5/elhub_sdk/wsdl/test/2.3/bim/thirdpartyaccess/UpdateThirdPartyAccess.xsd
+-rw-r--r--   0        0        0    43165 2023-07-21 06:57:20.399249 elhub_python_sdk-0.1.5/elhub_sdk/wsdl/test/2.3/bim v22 sorted/Elhub_AggregatedBusinessInformationEntities_v22_sorted.xsd
+-rw-r--r--   0        0        0        0 2023-07-21 06:57:20.399249 elhub_python_sdk-0.1.5/elhub_sdk/wsdl/test/2.3/bim v22 sorted/Elhub_BusinessDataType_v22_sorted.xsd
+-rw-r--r--   0        0        0   126666 2023-07-21 06:57:20.399249 elhub_python_sdk-0.1.5/elhub_sdk/wsdl/test/2.3/bindings/jaxb_numeric.xml
+-rw-r--r--   0        0        0    12375 2023-07-21 06:57:20.399249 elhub_python_sdk-0.1.5/elhub_sdk/wsdl/test/2.3/wsdl/MarketProcesses - WS-Security.wsdl
+-rw-r--r--   0        0        0     6741 2023-07-21 06:57:20.399249 elhub_python_sdk-0.1.5/elhub_sdk/wsdl/test/2.3/wsdl/MeteringValues - WS-Security.wsdl
+-rw-r--r--   0        0        0     6971 2023-07-21 06:57:20.399249 elhub_python_sdk-0.1.5/elhub_sdk/wsdl/test/2.3/wsdl/PollMarketProcesses - WS-Security.wsdl
+-rw-r--r--   0        0        0     6960 2023-07-21 06:57:20.399249 elhub_python_sdk-0.1.5/elhub_sdk/wsdl/test/2.3/wsdl/PollMeteringValues - WS-Security.wsdl
+-rw-r--r--   0        0        0    11192 2023-07-21 06:57:20.399249 elhub_python_sdk-0.1.5/elhub_sdk/wsdl/test/2.3/wsdl/Query - WS-Security.wsdl
+-rw-r--r--   0        0        0     3056 2023-07-21 06:57:20.399249 elhub_python_sdk-0.1.5/elhub_sdk/wsdl/test/2.3/wsdl/xsd/MarketProcesses.xsd
+-rw-r--r--   0        0        0     1159 2023-07-21 06:57:20.399249 elhub_python_sdk-0.1.5/elhub_sdk/wsdl/test/2.3/wsdl/xsd/MeteringValues.xsd
+-rw-r--r--   0        0        0     6206 2023-07-21 06:57:20.399249 elhub_python_sdk-0.1.5/elhub_sdk/wsdl/test/2.3/wsdl/xsd/PollMarketProcesses.xsd
+-rw-r--r--   0        0        0     3176 2023-07-21 06:57:20.399249 elhub_python_sdk-0.1.5/elhub_sdk/wsdl/test/2.3/wsdl/xsd/PollMeteringValues.xsd
+-rw-r--r--   0        0        0     3263 2023-07-21 06:57:20.399249 elhub_python_sdk-0.1.5/elhub_sdk/wsdl/test/2.3/wsdl/xsd/Query.xsd
+-rw-r--r--   0        0        0     1613 2023-07-21 06:57:20.399249 elhub_python_sdk-0.1.5/elhub_sdk/wsdl/test/2.3/wsdl/xsd/common.xsd
+-rw-r--r--   0        0        0     2506 2023-07-21 06:57:20.399249 elhub_python_sdk-0.1.5/pyproject.toml
+-rw-r--r--   0        0        0       46 2023-07-21 06:57:20.403250 elhub_python_sdk-0.1.5/tests/__init__.py
+-rw-r--r--   0        0        0     4674 2023-07-21 06:57:20.403250 elhub_python_sdk-0.1.5/tests/test_integration.py
+-rw-r--r--   0        0        0     3914 2023-07-21 06:57:20.403250 elhub_python_sdk-0.1.5/tests/test_integration_soap.py
+-rw-r--r--   0        0        0      283 2023-07-21 06:57:20.403250 elhub_python_sdk-0.1.5/tests/tests_examples/README.md
+-rw-r--r--   0        0        0        0 2023-07-21 06:57:20.403250 elhub_python_sdk-0.1.5/tests/tests_examples/__init__.py
+-rw-r--r--   0        0        0      932 2023-07-21 06:57:20.403250 elhub_python_sdk-0.1.5/tests/tests_examples/ag611-01-actor-test.py
+-rw-r--r--   0        0        0     1987 2023-07-21 06:57:20.403250 elhub_python_sdk-0.1.5/tests/tests_examples/ag622-01-actor-test.py
+-rw-r--r--   0        0        0     1966 2023-07-21 06:57:20.403250 elhub_python_sdk-0.1.5/tests/tests_examples/ag622-02-actor-test.py
+-rw-r--r--   0        0        0      401 2023-07-21 06:57:20.403250 elhub_python_sdk-0.1.5/tests/tests_examples/config.py
+-rw-r--r--   0        0        0     3424 1970-01-01 00:00:00.000000 elhub_python_sdk-0.1.5/PKG-INFO
```

### Comparing `elhub_python_sdk-0.1.4/LICENSE` & `elhub_python_sdk-0.1.5/LICENSE`

 * *Files identical despite different names*

### Comparing `elhub_python_sdk-0.1.4/README.md` & `elhub_python_sdk-0.1.5/README.md`

 * *Files identical despite different names*

### Comparing `elhub_python_sdk-0.1.4/elhub_sdk/client.py` & `elhub_python_sdk-0.1.5/elhub_sdk/client.py`

 * *Files identical despite different names*

### Comparing `elhub_python_sdk-0.1.4/elhub_sdk/consumption.py` & `elhub_python_sdk-0.1.5/elhub_sdk/consumption.py`

 * *Files identical despite different names*

### Comparing `elhub_python_sdk-0.1.4/elhub_sdk/enrollment.py` & `elhub_python_sdk-0.1.5/elhub_sdk/enrollment.py`

 * *Files identical despite different names*

### Comparing `elhub_python_sdk-0.1.4/elhub_sdk/enums.py` & `elhub_python_sdk-0.1.5/elhub_sdk/enums.py`

 * *Files 4% similar despite different names*

```diff
@@ -84,7 +84,18 @@
     """
     Determines the action you want to do
     """
 
     ADD = "Add"
     DELETE = "Delete"
     UPDATE = "Update"
+
+
+
+class STATUS_TYPE(Enum):
+    """
+    Status Type
+    ref: https://dok.elhub.no/ediel2/acknowledgement
+    """
+
+    ACCEPTED = '39'
+    REJECTED = '41'
```

### Comparing `elhub_python_sdk-0.1.4/elhub_sdk/settings.py` & `elhub_python_sdk-0.1.5/elhub_sdk/settings.py`

 * *Files identical despite different names*

### Comparing `elhub_python_sdk-0.1.4/elhub_sdk/third_party.py` & `elhub_python_sdk-0.1.5/elhub_sdk/third_party.py`

 * *Files identical despite different names*

### Comparing `elhub_python_sdk-0.1.4/elhub_sdk/wsdl/prod/2.3/bim/Acknowledgement.xsd` & `elhub_python_sdk-0.1.5/elhub_sdk/wsdl/prod/2.3/bim/Acknowledgement.xsd`

 * *Files identical despite different names*

### Comparing `elhub_python_sdk-0.1.4/elhub_sdk/wsdl/prod/2.3/bim/PollForData.xsd` & `elhub_python_sdk-0.1.5/elhub_sdk/wsdl/prod/2.3/bim/PollForData.xsd`

 * *Files identical despite different names*

### Comparing `elhub_python_sdk-0.1.4/elhub_sdk/wsdl/prod/2.3/bim/common/Elhub_AggregatedBusinessInformationEntities.xsd` & `elhub_python_sdk-0.1.5/elhub_sdk/wsdl/prod/2.3/bim/common/Elhub_AggregatedBusinessInformationEntities.xsd`

 * *Files identical despite different names*

### Comparing `elhub_python_sdk-0.1.4/elhub_sdk/wsdl/prod/2.3/bim/common/Elhub_BusinessDataType.xsd` & `elhub_python_sdk-0.1.5/elhub_sdk/wsdl/prod/2.3/bim/common/Elhub_BusinessDataType.xsd`

 * *Files identical despite different names*

### Comparing `elhub_python_sdk-0.1.4/elhub_sdk/wsdl/prod/2.3/bim/market/ConfirmEndOfSupply.xsd` & `elhub_python_sdk-0.1.5/elhub_sdk/wsdl/prod/2.3/bim/market/ConfirmEndOfSupply.xsd`

 * *Files identical despite different names*

### Comparing `elhub_python_sdk-0.1.4/elhub_sdk/wsdl/prod/2.3/bim/market/ConfirmStartOfSupply.xsd` & `elhub_python_sdk-0.1.5/elhub_sdk/wsdl/prod/2.3/bim/market/ConfirmStartOfSupply.xsd`

 * *Files identical despite different names*

### Comparing `elhub_python_sdk-0.1.4/elhub_sdk/wsdl/prod/2.3/bim/market/NotifyEndOfSupply.xsd` & `elhub_python_sdk-0.1.5/elhub_sdk/wsdl/prod/2.3/bim/market/NotifyEndOfSupply.xsd`

 * *Files identical despite different names*

### Comparing `elhub_python_sdk-0.1.4/elhub_sdk/wsdl/prod/2.3/bim/market/NotifyStartOfSupply.xsd` & `elhub_python_sdk-0.1.5/elhub_sdk/wsdl/prod/2.3/bim/market/NotifyStartOfSupply.xsd`

 * *Files identical despite different names*

### Comparing `elhub_python_sdk-0.1.4/elhub_sdk/wsdl/prod/2.3/bim/market/RejectEndOfSupply.xsd` & `elhub_python_sdk-0.1.5/elhub_sdk/wsdl/prod/2.3/bim/market/RejectEndOfSupply.xsd`

 * *Files identical despite different names*

### Comparing `elhub_python_sdk-0.1.4/elhub_sdk/wsdl/prod/2.3/bim/market/RejectStartOfSupply.xsd` & `elhub_python_sdk-0.1.5/elhub_sdk/wsdl/prod/2.3/bim/market/RejectStartOfSupply.xsd`

 * *Files identical despite different names*

### Comparing `elhub_python_sdk-0.1.4/elhub_sdk/wsdl/prod/2.3/bim/market/RequestEndOfSupply.xsd` & `elhub_python_sdk-0.1.5/elhub_sdk/wsdl/prod/2.3/bim/market/RequestEndOfSupply.xsd`

 * *Files identical despite different names*

### Comparing `elhub_python_sdk-0.1.4/elhub_sdk/wsdl/prod/2.3/bim/market/RequestStartOfSupply.xsd` & `elhub_python_sdk-0.1.5/elhub_sdk/wsdl/prod/2.3/bim/market/RequestStartOfSupply.xsd`

 * *Files identical despite different names*

### Comparing `elhub_python_sdk-0.1.4/elhub_sdk/wsdl/prod/2.3/bim/masterdata/NotifyCustomerInformation.xsd` & `elhub_python_sdk-0.1.5/elhub_sdk/wsdl/prod/2.3/bim/masterdata/NotifyCustomerInformation.xsd`

 * *Files identical despite different names*

### Comparing `elhub_python_sdk-0.1.4/elhub_sdk/wsdl/prod/2.3/bim/masterdata/NotifyMeteringPointCharacteristics.xsd` & `elhub_python_sdk-0.1.5/elhub_sdk/wsdl/prod/2.3/bim/masterdata/NotifyMeteringPointCharacteristics.xsd`

 * *Files identical despite different names*

### Comparing `elhub_python_sdk-0.1.4/elhub_sdk/wsdl/prod/2.3/bim/masterdata/RequestUpdateCustomerInformation.xsd` & `elhub_python_sdk-0.1.5/elhub_sdk/wsdl/prod/2.3/bim/masterdata/RequestUpdateCustomerInformation.xsd`

 * *Files identical despite different names*

### Comparing `elhub_python_sdk-0.1.4/elhub_sdk/wsdl/prod/2.3/bim/masterdata/RequestUpdateMasterDataMeteringPoint.xsd` & `elhub_python_sdk-0.1.5/elhub_sdk/wsdl/prod/2.3/bim/masterdata/RequestUpdateMasterDataMeteringPoint.xsd`

 * *Files identical despite different names*

### Comparing `elhub_python_sdk-0.1.4/elhub_sdk/wsdl/prod/2.3/bim/metering/CollectedData.xsd` & `elhub_python_sdk-0.1.5/elhub_sdk/wsdl/prod/2.3/bim/metering/CollectedData.xsd`

 * *Files identical despite different names*

### Comparing `elhub_python_sdk-0.1.4/elhub_sdk/wsdl/prod/2.3/bim/metering/NotifyValidatedDataForBillingEnergy.xsd` & `elhub_python_sdk-0.1.5/elhub_sdk/wsdl/prod/2.3/bim/metering/NotifyValidatedDataForBillingEnergy.xsd`

 * *Files identical despite different names*

### Comparing `elhub_python_sdk-0.1.4/elhub_sdk/wsdl/prod/2.3/bim/metering/PriceVolumeCombinationForReconciliation.xsd` & `elhub_python_sdk-0.1.5/elhub_sdk/wsdl/prod/2.3/bim/metering/PriceVolumeCombinationForReconciliation.xsd`

 * *Files identical despite different names*

### Comparing `elhub_python_sdk-0.1.4/elhub_sdk/wsdl/prod/2.3/bim/metering/RequestCollectedData.xsd` & `elhub_python_sdk-0.1.5/elhub_sdk/wsdl/prod/2.3/bim/metering/RequestCollectedData.xsd`

 * *Files identical despite different names*

### Comparing `elhub_python_sdk-0.1.4/elhub_sdk/wsdl/prod/2.3/bim/query/RequestDataFromElhub.xsd` & `elhub_python_sdk-0.1.5/elhub_sdk/wsdl/prod/2.3/bim/query/RequestDataFromElhub.xsd`

 * *Files identical despite different names*

### Comparing `elhub_python_sdk-0.1.4/elhub_sdk/wsdl/prod/2.3/bim/query/RequestToElhub.xsd` & `elhub_python_sdk-0.1.5/elhub_sdk/wsdl/prod/2.3/bim/query/RequestToElhub.xsd`

 * *Files identical despite different names*

### Comparing `elhub_python_sdk-0.1.4/elhub_sdk/wsdl/prod/2.3/bim/query/RequestToGridAccessProvider.xsd` & `elhub_python_sdk-0.1.5/elhub_sdk/wsdl/prod/2.3/bim/query/RequestToGridAccessProvider.xsd`

 * *Files identical despite different names*

### Comparing `elhub_python_sdk-0.1.4/elhub_sdk/wsdl/prod/2.3/bim/query/RequestUpfrontMeteringPointCharacteristics.xsd` & `elhub_python_sdk-0.1.5/elhub_sdk/wsdl/prod/2.3/bim/query/RequestUpfrontMeteringPointCharacteristics.xsd`

 * *Files identical despite different names*

### Comparing `elhub_python_sdk-0.1.4/elhub_sdk/wsdl/prod/2.3/bim/query/ResponseFromElhub.xsd` & `elhub_python_sdk-0.1.5/elhub_sdk/wsdl/prod/2.3/bim/query/ResponseFromElhub.xsd`

 * *Files identical despite different names*

### Comparing `elhub_python_sdk-0.1.4/elhub_sdk/wsdl/prod/2.3/bim/query/ResponseFromGridAccessProvider.xsd` & `elhub_python_sdk-0.1.5/elhub_sdk/wsdl/prod/2.3/bim/query/ResponseFromGridAccessProvider.xsd`

 * *Files identical despite different names*

### Comparing `elhub_python_sdk-0.1.4/elhub_sdk/wsdl/prod/2.3/bim/query/ResponseUpfrontMeteringPointCharacteristics.xsd` & `elhub_python_sdk-0.1.5/elhub_sdk/wsdl/prod/2.3/bim/query/ResponseUpfrontMeteringPointCharacteristics.xsd`

 * *Files identical despite different names*

### Comparing `elhub_python_sdk-0.1.4/elhub_sdk/wsdl/prod/2.3/bim/thirdpartyaccess/UpdateThirdPartyAccess.xsd` & `elhub_python_sdk-0.1.5/elhub_sdk/wsdl/prod/2.3/bim/thirdpartyaccess/UpdateThirdPartyAccess.xsd`

 * *Files identical despite different names*

### Comparing `elhub_python_sdk-0.1.4/elhub_sdk/wsdl/prod/2.3/bim v22 sorted/Elhub_AggregatedBusinessInformationEntities_v22_sorted.xsd` & `elhub_python_sdk-0.1.5/elhub_sdk/wsdl/prod/2.3/bim v22 sorted/Elhub_AggregatedBusinessInformationEntities_v22_sorted.xsd`

 * *Files identical despite different names*

### Comparing `elhub_python_sdk-0.1.4/elhub_sdk/wsdl/prod/2.3/bindings/jaxb_numeric.xml` & `elhub_python_sdk-0.1.5/elhub_sdk/wsdl/prod/2.3/bindings/jaxb_numeric.xml`

 * *Files identical despite different names*

### Comparing `elhub_python_sdk-0.1.4/elhub_sdk/wsdl/prod/2.3/wsdl/MarketProcesses - WS-Security.wsdl` & `elhub_python_sdk-0.1.5/elhub_sdk/wsdl/prod/2.3/wsdl/MarketProcesses - WS-Security.wsdl`

 * *Files identical despite different names*

### Comparing `elhub_python_sdk-0.1.4/elhub_sdk/wsdl/prod/2.3/wsdl/MeteringValues - WS-Security.wsdl` & `elhub_python_sdk-0.1.5/elhub_sdk/wsdl/prod/2.3/wsdl/MeteringValues - WS-Security.wsdl`

 * *Files identical despite different names*

### Comparing `elhub_python_sdk-0.1.4/elhub_sdk/wsdl/prod/2.3/wsdl/PollMarketProcesses - WS-Security.wsdl` & `elhub_python_sdk-0.1.5/elhub_sdk/wsdl/prod/2.3/wsdl/PollMarketProcesses - WS-Security.wsdl`

 * *Files identical despite different names*

### Comparing `elhub_python_sdk-0.1.4/elhub_sdk/wsdl/prod/2.3/wsdl/PollMeteringValues - WS-Security.wsdl` & `elhub_python_sdk-0.1.5/elhub_sdk/wsdl/prod/2.3/wsdl/PollMeteringValues - WS-Security.wsdl`

 * *Files identical despite different names*

### Comparing `elhub_python_sdk-0.1.4/elhub_sdk/wsdl/prod/2.3/wsdl/Query - WS-Security.wsdl` & `elhub_python_sdk-0.1.5/elhub_sdk/wsdl/prod/2.3/wsdl/Query - WS-Security.wsdl`

 * *Files identical despite different names*

### Comparing `elhub_python_sdk-0.1.4/elhub_sdk/wsdl/prod/2.3/wsdl/xsd/MarketProcesses.xsd` & `elhub_python_sdk-0.1.5/elhub_sdk/wsdl/prod/2.3/wsdl/xsd/MarketProcesses.xsd`

 * *Files identical despite different names*

### Comparing `elhub_python_sdk-0.1.4/elhub_sdk/wsdl/prod/2.3/wsdl/xsd/MeteringValues.xsd` & `elhub_python_sdk-0.1.5/elhub_sdk/wsdl/prod/2.3/wsdl/xsd/MeteringValues.xsd`

 * *Files identical despite different names*

### Comparing `elhub_python_sdk-0.1.4/elhub_sdk/wsdl/prod/2.3/wsdl/xsd/PollMarketProcesses.xsd` & `elhub_python_sdk-0.1.5/elhub_sdk/wsdl/prod/2.3/wsdl/xsd/PollMarketProcesses.xsd`

 * *Files identical despite different names*

### Comparing `elhub_python_sdk-0.1.4/elhub_sdk/wsdl/prod/2.3/wsdl/xsd/PollMeteringValues.xsd` & `elhub_python_sdk-0.1.5/elhub_sdk/wsdl/prod/2.3/wsdl/xsd/PollMeteringValues.xsd`

 * *Files identical despite different names*

### Comparing `elhub_python_sdk-0.1.4/elhub_sdk/wsdl/prod/2.3/wsdl/xsd/Query.xsd` & `elhub_python_sdk-0.1.5/elhub_sdk/wsdl/prod/2.3/wsdl/xsd/Query.xsd`

 * *Files identical despite different names*

### Comparing `elhub_python_sdk-0.1.4/elhub_sdk/wsdl/prod/2.3/wsdl/xsd/common.xsd` & `elhub_python_sdk-0.1.5/elhub_sdk/wsdl/prod/2.3/wsdl/xsd/common.xsd`

 * *Files identical despite different names*

### Comparing `elhub_python_sdk-0.1.4/elhub_sdk/wsdl/test/2.3/bim/Acknowledgement.xsd` & `elhub_python_sdk-0.1.5/elhub_sdk/wsdl/test/2.3/bim/Acknowledgement.xsd`

 * *Files identical despite different names*

### Comparing `elhub_python_sdk-0.1.4/elhub_sdk/wsdl/test/2.3/bim/PollForData.xsd` & `elhub_python_sdk-0.1.5/elhub_sdk/wsdl/test/2.3/bim/PollForData.xsd`

 * *Files identical despite different names*

### Comparing `elhub_python_sdk-0.1.4/elhub_sdk/wsdl/test/2.3/bim/common/Elhub_AggregatedBusinessInformationEntities.xsd` & `elhub_python_sdk-0.1.5/elhub_sdk/wsdl/test/2.3/bim/common/Elhub_AggregatedBusinessInformationEntities.xsd`

 * *Files identical despite different names*

### Comparing `elhub_python_sdk-0.1.4/elhub_sdk/wsdl/test/2.3/bim/common/Elhub_BusinessDataType.xsd` & `elhub_python_sdk-0.1.5/elhub_sdk/wsdl/test/2.3/bim/common/Elhub_BusinessDataType.xsd`

 * *Files identical despite different names*

### Comparing `elhub_python_sdk-0.1.4/elhub_sdk/wsdl/test/2.3/bim/market/ConfirmEndOfSupply.xsd` & `elhub_python_sdk-0.1.5/elhub_sdk/wsdl/test/2.3/bim/market/ConfirmEndOfSupply.xsd`

 * *Files identical despite different names*

### Comparing `elhub_python_sdk-0.1.4/elhub_sdk/wsdl/test/2.3/bim/market/ConfirmStartOfSupply.xsd` & `elhub_python_sdk-0.1.5/elhub_sdk/wsdl/test/2.3/bim/market/ConfirmStartOfSupply.xsd`

 * *Files identical despite different names*

### Comparing `elhub_python_sdk-0.1.4/elhub_sdk/wsdl/test/2.3/bim/market/NotifyEndOfSupply.xsd` & `elhub_python_sdk-0.1.5/elhub_sdk/wsdl/test/2.3/bim/market/NotifyEndOfSupply.xsd`

 * *Files identical despite different names*

### Comparing `elhub_python_sdk-0.1.4/elhub_sdk/wsdl/test/2.3/bim/market/NotifyStartOfSupply.xsd` & `elhub_python_sdk-0.1.5/elhub_sdk/wsdl/test/2.3/bim/market/NotifyStartOfSupply.xsd`

 * *Files identical despite different names*

### Comparing `elhub_python_sdk-0.1.4/elhub_sdk/wsdl/test/2.3/bim/market/RejectEndOfSupply.xsd` & `elhub_python_sdk-0.1.5/elhub_sdk/wsdl/test/2.3/bim/market/RejectEndOfSupply.xsd`

 * *Files identical despite different names*

### Comparing `elhub_python_sdk-0.1.4/elhub_sdk/wsdl/test/2.3/bim/market/RejectStartOfSupply.xsd` & `elhub_python_sdk-0.1.5/elhub_sdk/wsdl/test/2.3/bim/market/RejectStartOfSupply.xsd`

 * *Files identical despite different names*

### Comparing `elhub_python_sdk-0.1.4/elhub_sdk/wsdl/test/2.3/bim/market/RequestEndOfSupply.xsd` & `elhub_python_sdk-0.1.5/elhub_sdk/wsdl/test/2.3/bim/market/RequestEndOfSupply.xsd`

 * *Files identical despite different names*

### Comparing `elhub_python_sdk-0.1.4/elhub_sdk/wsdl/test/2.3/bim/market/RequestStartOfSupply.xsd` & `elhub_python_sdk-0.1.5/elhub_sdk/wsdl/test/2.3/bim/market/RequestStartOfSupply.xsd`

 * *Files identical despite different names*

### Comparing `elhub_python_sdk-0.1.4/elhub_sdk/wsdl/test/2.3/bim/masterdata/NotifyCustomerInformation.xsd` & `elhub_python_sdk-0.1.5/elhub_sdk/wsdl/test/2.3/bim/masterdata/NotifyCustomerInformation.xsd`

 * *Files identical despite different names*

### Comparing `elhub_python_sdk-0.1.4/elhub_sdk/wsdl/test/2.3/bim/masterdata/NotifyMeteringPointCharacteristics.xsd` & `elhub_python_sdk-0.1.5/elhub_sdk/wsdl/test/2.3/bim/masterdata/NotifyMeteringPointCharacteristics.xsd`

 * *Files identical despite different names*

### Comparing `elhub_python_sdk-0.1.4/elhub_sdk/wsdl/test/2.3/bim/masterdata/RequestUpdateCustomerInformation.xsd` & `elhub_python_sdk-0.1.5/elhub_sdk/wsdl/test/2.3/bim/masterdata/RequestUpdateCustomerInformation.xsd`

 * *Files identical despite different names*

### Comparing `elhub_python_sdk-0.1.4/elhub_sdk/wsdl/test/2.3/bim/masterdata/RequestUpdateMasterDataMeteringPoint.xsd` & `elhub_python_sdk-0.1.5/elhub_sdk/wsdl/test/2.3/bim/masterdata/RequestUpdateMasterDataMeteringPoint.xsd`

 * *Files identical despite different names*

### Comparing `elhub_python_sdk-0.1.4/elhub_sdk/wsdl/test/2.3/bim/metering/CollectedData.xsd` & `elhub_python_sdk-0.1.5/elhub_sdk/wsdl/test/2.3/bim/metering/CollectedData.xsd`

 * *Files identical despite different names*

### Comparing `elhub_python_sdk-0.1.4/elhub_sdk/wsdl/test/2.3/bim/metering/NotifyValidatedDataForBillingEnergy.xsd` & `elhub_python_sdk-0.1.5/elhub_sdk/wsdl/test/2.3/bim/metering/NotifyValidatedDataForBillingEnergy.xsd`

 * *Files identical despite different names*

### Comparing `elhub_python_sdk-0.1.4/elhub_sdk/wsdl/test/2.3/bim/metering/PriceVolumeCombinationForReconciliation.xsd` & `elhub_python_sdk-0.1.5/elhub_sdk/wsdl/test/2.3/bim/metering/PriceVolumeCombinationForReconciliation.xsd`

 * *Files identical despite different names*

### Comparing `elhub_python_sdk-0.1.4/elhub_sdk/wsdl/test/2.3/bim/metering/RequestCollectedData.xsd` & `elhub_python_sdk-0.1.5/elhub_sdk/wsdl/test/2.3/bim/metering/RequestCollectedData.xsd`

 * *Files identical despite different names*

### Comparing `elhub_python_sdk-0.1.4/elhub_sdk/wsdl/test/2.3/bim/query/RequestDataFromElhub.xsd` & `elhub_python_sdk-0.1.5/elhub_sdk/wsdl/test/2.3/bim/query/RequestDataFromElhub.xsd`

 * *Files identical despite different names*

### Comparing `elhub_python_sdk-0.1.4/elhub_sdk/wsdl/test/2.3/bim/query/RequestToElhub.xsd` & `elhub_python_sdk-0.1.5/elhub_sdk/wsdl/test/2.3/bim/query/RequestToElhub.xsd`

 * *Files identical despite different names*

### Comparing `elhub_python_sdk-0.1.4/elhub_sdk/wsdl/test/2.3/bim/query/RequestToGridAccessProvider.xsd` & `elhub_python_sdk-0.1.5/elhub_sdk/wsdl/test/2.3/bim/query/RequestToGridAccessProvider.xsd`

 * *Files identical despite different names*

### Comparing `elhub_python_sdk-0.1.4/elhub_sdk/wsdl/test/2.3/bim/query/RequestUpfrontMeteringPointCharacteristics.xsd` & `elhub_python_sdk-0.1.5/elhub_sdk/wsdl/test/2.3/bim/query/RequestUpfrontMeteringPointCharacteristics.xsd`

 * *Files identical despite different names*

### Comparing `elhub_python_sdk-0.1.4/elhub_sdk/wsdl/test/2.3/bim/query/ResponseFromElhub.xsd` & `elhub_python_sdk-0.1.5/elhub_sdk/wsdl/test/2.3/bim/query/ResponseFromElhub.xsd`

 * *Files identical despite different names*

### Comparing `elhub_python_sdk-0.1.4/elhub_sdk/wsdl/test/2.3/bim/query/ResponseFromGridAccessProvider.xsd` & `elhub_python_sdk-0.1.5/elhub_sdk/wsdl/test/2.3/bim/query/ResponseFromGridAccessProvider.xsd`

 * *Files identical despite different names*

### Comparing `elhub_python_sdk-0.1.4/elhub_sdk/wsdl/test/2.3/bim/query/ResponseUpfrontMeteringPointCharacteristics.xsd` & `elhub_python_sdk-0.1.5/elhub_sdk/wsdl/test/2.3/bim/query/ResponseUpfrontMeteringPointCharacteristics.xsd`

 * *Files identical despite different names*

### Comparing `elhub_python_sdk-0.1.4/elhub_sdk/wsdl/test/2.3/bim/thirdpartyaccess/UpdateThirdPartyAccess.xsd` & `elhub_python_sdk-0.1.5/elhub_sdk/wsdl/test/2.3/bim/thirdpartyaccess/UpdateThirdPartyAccess.xsd`

 * *Files identical despite different names*

### Comparing `elhub_python_sdk-0.1.4/elhub_sdk/wsdl/test/2.3/bim v22 sorted/Elhub_AggregatedBusinessInformationEntities_v22_sorted.xsd` & `elhub_python_sdk-0.1.5/elhub_sdk/wsdl/test/2.3/bim v22 sorted/Elhub_AggregatedBusinessInformationEntities_v22_sorted.xsd`

 * *Files identical despite different names*

### Comparing `elhub_python_sdk-0.1.4/elhub_sdk/wsdl/test/2.3/bindings/jaxb_numeric.xml` & `elhub_python_sdk-0.1.5/elhub_sdk/wsdl/test/2.3/bindings/jaxb_numeric.xml`

 * *Files identical despite different names*

### Comparing `elhub_python_sdk-0.1.4/elhub_sdk/wsdl/test/2.3/wsdl/MarketProcesses - WS-Security.wsdl` & `elhub_python_sdk-0.1.5/elhub_sdk/wsdl/test/2.3/wsdl/MarketProcesses - WS-Security.wsdl`

 * *Files identical despite different names*

### Comparing `elhub_python_sdk-0.1.4/elhub_sdk/wsdl/test/2.3/wsdl/MeteringValues - WS-Security.wsdl` & `elhub_python_sdk-0.1.5/elhub_sdk/wsdl/test/2.3/wsdl/MeteringValues - WS-Security.wsdl`

 * *Files identical despite different names*

### Comparing `elhub_python_sdk-0.1.4/elhub_sdk/wsdl/test/2.3/wsdl/PollMarketProcesses - WS-Security.wsdl` & `elhub_python_sdk-0.1.5/elhub_sdk/wsdl/test/2.3/wsdl/PollMarketProcesses - WS-Security.wsdl`

 * *Files identical despite different names*

### Comparing `elhub_python_sdk-0.1.4/elhub_sdk/wsdl/test/2.3/wsdl/PollMeteringValues - WS-Security.wsdl` & `elhub_python_sdk-0.1.5/elhub_sdk/wsdl/test/2.3/wsdl/PollMeteringValues - WS-Security.wsdl`

 * *Files identical despite different names*

### Comparing `elhub_python_sdk-0.1.4/elhub_sdk/wsdl/test/2.3/wsdl/Query - WS-Security.wsdl` & `elhub_python_sdk-0.1.5/elhub_sdk/wsdl/test/2.3/wsdl/Query - WS-Security.wsdl`

 * *Files identical despite different names*

### Comparing `elhub_python_sdk-0.1.4/elhub_sdk/wsdl/test/2.3/wsdl/xsd/MarketProcesses.xsd` & `elhub_python_sdk-0.1.5/elhub_sdk/wsdl/test/2.3/wsdl/xsd/MarketProcesses.xsd`

 * *Files identical despite different names*

### Comparing `elhub_python_sdk-0.1.4/elhub_sdk/wsdl/test/2.3/wsdl/xsd/MeteringValues.xsd` & `elhub_python_sdk-0.1.5/elhub_sdk/wsdl/test/2.3/wsdl/xsd/MeteringValues.xsd`

 * *Files identical despite different names*

### Comparing `elhub_python_sdk-0.1.4/elhub_sdk/wsdl/test/2.3/wsdl/xsd/PollMarketProcesses.xsd` & `elhub_python_sdk-0.1.5/elhub_sdk/wsdl/test/2.3/wsdl/xsd/PollMarketProcesses.xsd`

 * *Files identical despite different names*

### Comparing `elhub_python_sdk-0.1.4/elhub_sdk/wsdl/test/2.3/wsdl/xsd/PollMeteringValues.xsd` & `elhub_python_sdk-0.1.5/elhub_sdk/wsdl/test/2.3/wsdl/xsd/PollMeteringValues.xsd`

 * *Files identical despite different names*

### Comparing `elhub_python_sdk-0.1.4/elhub_sdk/wsdl/test/2.3/wsdl/xsd/Query.xsd` & `elhub_python_sdk-0.1.5/elhub_sdk/wsdl/test/2.3/wsdl/xsd/Query.xsd`

 * *Files identical despite different names*

### Comparing `elhub_python_sdk-0.1.4/elhub_sdk/wsdl/test/2.3/wsdl/xsd/common.xsd` & `elhub_python_sdk-0.1.5/elhub_sdk/wsdl/test/2.3/wsdl/xsd/common.xsd`

 * *Files identical despite different names*

### Comparing `elhub_python_sdk-0.1.4/pyproject.toml` & `elhub_python_sdk-0.1.5/pyproject.toml`

 * *Files 1% similar despite different names*

```diff
@@ -1,11 +1,11 @@
 [tool]
 [tool.poetry]
 name = "elhub-python-sdk"
-version = "0.1.4"
+version = "0.1.5"
 homepage = "https://github.com/bkkas/elhub-python-sdk"
 description = "Non official Python SDK for ElHub API."
 authors = ["Volte <jesus.condon@eviny.no>"]
 readme = "README.md"
 license =  "GPL-3.0-only"
 classifiers=[
     'Development Status :: 2 - Pre-Alpha',
```

### Comparing `elhub_python_sdk-0.1.4/tests/test_integration.py` & `elhub_python_sdk-0.1.5/tests/tests_examples/ag622-02-actor-test.py`

 * *Files 25% similar despite different names*

```diff
@@ -1,118 +1,68 @@
-import datetime
 import logging
 
-import pytest
-
-from elhub_sdk.client import APIClient, ElHubEnvironment, ElHubService
-from elhub_sdk.consumption import poll_consumption, request_consumption
-from elhub_sdk.enrollment import get_meter_characteristics
+from elhub_sdk.client import APIClient
+from elhub_sdk.consumption import poll_consumption
 from elhub_sdk.enums import THIRD_PARTY_ACTION
-from elhub_sdk.settings import CERT_FILE, KEY_FILE
+from elhub_sdk.settings import CERT_FILE, KEY_FILE, WSDL_FILES_CONFIG_TEST
 from elhub_sdk.third_party import request_action
-from tests.tests_examples.config import THIRD_PARTY_GSN_EXA
-
-logger = logging.getLogger(__name__)
-
-
-@pytest.mark.integrationtest
-def test_meter_characteristics():
-    """Test meter characteristics"""
-    meter_identificator = "707057500010503271"
-
-    client, history = APIClient.get_client(
-        environment=ElHubEnvironment.TEST,
-        service=ElHubService.QUERY,
-        key_file=KEY_FILE,
-        cert_file=CERT_FILE,
-    )
-
-    response = get_meter_characteristics(
-        client=client, history=history, meter_identificator=meter_identificator, sender_gsn=THIRD_PARTY_GSN_EXA
-    )
+from tests.tests_examples.config import TEST_METER_IDENTIFICATORS, THIRD_PARTY_GSN_EXA
 
-    assert response is not None
+logger = logging.getLogger()
+logging.basicConfig(level=logging.DEBUG)
 
 
-@pytest.mark.integrationtest
-def test_third_party_delete():
-    """
-    Tests the addition of a third party against Exa2
-    Returns:
+METER_IDENTIFICATOR = TEST_METER_IDENTIFICATORS["non_profiled"][0]
 
-    """
 
-    client, history = APIClient.get_client(
-        environment=ElHubEnvironment.TEST,
-        service=ElHubService.MARKET_PROCESSES,
-        key_file=KEY_FILE,
-        cert_file=CERT_FILE,
+def add_third_party():
+    logger.debug("Adding meter as third party")
+    client, history = APIClient.get_zeep_client(
+        wsdl=WSDL_FILES_CONFIG_TEST['MARKET_PROCESSES'], secure=True, key_file=KEY_FILE, cert_file=CERT_FILE
     )
-
-    meter_identificator = "707057500084111792"
     response = request_action(
-        client, history, THIRD_PARTY_GSN_EXA, meter_identificator=meter_identificator, action=THIRD_PARTY_ACTION.DELETE
+        client, history, THIRD_PARTY_GSN_EXA, meter_identificator=METER_IDENTIFICATOR, action=THIRD_PARTY_ACTION.ADD
     )
-    assert response != False
+    return response
 
 
-@pytest.mark.integrationtest
-def test_third_party_add():
-    """
-    Tests the addition of a third party against Exa2
-    Returns:
-
-    """
-    client, history = APIClient.get_client(
-        environment=ElHubEnvironment.TEST,
-        service=ElHubService.MARKET_PROCESSES,
-        key_file=KEY_FILE,
-        cert_file=CERT_FILE,
-    )
-
-    meter_identificator = "707057500084111792"
-    response = request_action(
-        client, history, THIRD_PARTY_GSN_EXA, meter_identificator=meter_identificator, action=THIRD_PARTY_ACTION.ADD
-    )
-    assert response != False
-
-
-@pytest.mark.integrationtest
-def test_poll_consumption():
+def get_consumption():
     """
     Pooling data from Elhub
     Returns:
 
     """
-    client, history = APIClient.get_client(
-        environment=ElHubEnvironment.TEST,
-        service=ElHubService.POOL_METERING_VALUES,
-        key_file=KEY_FILE,
-        cert_file=CERT_FILE,
+    logger.debug("Getting consumption...")
+    client, history = APIClient.get_zeep_client(
+        wsdl=WSDL_FILES_CONFIG_TEST['POOL_METERING'], secure=True, key_file=KEY_FILE, cert_file=CERT_FILE
     )
 
     response = poll_consumption(client, history, THIRD_PARTY_GSN_EXA)
-    assert response is not None
+    return response
 
 
-@pytest.mark.integrationtest
-def test_request_consumption():
+def extended_storage():
     """
-    Query requesting consumption for a meter
+
     Returns:
 
     """
-    meter_identificator = "707057500057411768"
-    start = datetime.datetime(2022, 5, 1)
-    end = start + datetime.timedelta(days=7)
-
-    client, history = APIClient.get_client(
-        environment=ElHubEnvironment.TEST,
-        service=ElHubService.QUERY,
-        key_file=KEY_FILE,
-        cert_file=CERT_FILE,
+    client, history = APIClient.get_zeep_client(
+        wsdl=WSDL_FILES_CONFIG_TEST['MARKET_PROCESSES'], secure=True, key_file=KEY_FILE, cert_file=CERT_FILE
     )
 
-    response = request_consumption(
-        client, history, meter_identificator, sender_gsn=THIRD_PARTY_GSN_EXA, start=start, end=end
-    )
-    assert response != False
+    response = request_action(
+        client,
+        history,
+        THIRD_PARTY_GSN_EXA,
+        meter_identificator=METER_IDENTIFICATOR,
+        action=THIRD_PARTY_ACTION.ADD,
+        extended_storage=True,
+    )
+    return response
+
+
+if __name__ == "__main__":
+    logger.debug(f"Initiating tests with identificator: {METER_IDENTIFICATOR}")
+    # response = add_third_party()
+    # response = get_consumption()
+    response = extended_storage()
```

### Comparing `elhub_python_sdk-0.1.4/tests/test_integration_soap.py` & `elhub_python_sdk-0.1.5/tests/test_integration_soap.py`

 * *Files identical despite different names*

### Comparing `elhub_python_sdk-0.1.4/tests/tests_examples/ag611-01-actor-test.py` & `elhub_python_sdk-0.1.5/tests/tests_examples/ag611-01-actor-test.py`

 * *Files identical despite different names*

### Comparing `elhub_python_sdk-0.1.4/tests/tests_examples/ag622-01-actor-test.py` & `elhub_python_sdk-0.1.5/tests/tests_examples/ag622-01-actor-test.py`

 * *Files identical despite different names*

### Comparing `elhub_python_sdk-0.1.4/PKG-INFO` & `elhub_python_sdk-0.1.5/PKG-INFO`

 * *Files 7% similar despite different names*

```diff
@@ -1,28 +1,25 @@
 Metadata-Version: 2.1
 Name: elhub-python-sdk
-Version: 0.1.4
+Version: 0.1.5
 Summary: Non official Python SDK for ElHub API.
 Home-page: https://github.com/bkkas/elhub-python-sdk
 License: GPL-3.0-only
 Author: Volte
 Author-email: jesus.condon@eviny.no
 Requires-Python: >=3.8.2,<4.0
 Classifier: Development Status :: 2 - Pre-Alpha
 Classifier: Intended Audience :: Developers
 Classifier: License :: OSI Approved :: GNU General Public License v3 (GPLv3)
 Classifier: Natural Language :: English
 Classifier: Programming Language :: Python :: 3
 Classifier: Programming Language :: Python :: 3.9
 Classifier: Programming Language :: Python :: 3.10
 Classifier: Programming Language :: Python :: 3.11
-Classifier: Programming Language :: Python :: 3
-Classifier: Programming Language :: Python :: 3.10
 Classifier: Programming Language :: Python :: 3.8
-Classifier: Programming Language :: Python :: 3.9
 Provides-Extra: dev
 Provides-Extra: doc
 Provides-Extra: test
 Requires-Dist: black (>=22.8.0,<23.0.0) ; extra == "test"
 Requires-Dist: bump2version (>=1.0.1,<2.0.0) ; extra == "dev"
 Requires-Dist: flake8 (>=5.0.4,<6.0.0) ; extra == "test"
 Requires-Dist: flake8-docstrings (>=1.6.0,<2.0.0) ; extra == "test"
```

