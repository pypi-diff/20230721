# Comparing `tmp/fabric-message-bus-1.6.0b2.tar.gz` & `tmp/fabric-message-bus-1.6.0b3.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "fabric-message-bus-1.6.0b2.tar", last modified: Thu Jul 20 21:41:32 2023, max compression
+gzip compressed data, was "fabric-message-bus-1.6.0b3.tar", last modified: Fri Jul 21 13:30:55 2023, max compression
```

## Comparing `fabric-message-bus-1.6.0b2.tar` & `fabric-message-bus-1.6.0b3.tar`

### file list

```diff
@@ -1,105 +1,105 @@
--rw-r--r--   0        0        0     1856 2023-07-19 17:37:38.068966 fabric-message-bus-1.6.0b2/.gitignore
--rw-r--r--   0        0        0     1071 2023-07-19 17:37:38.069108 fabric-message-bus-1.6.0b2/LICENSE
--rw-r--r--   0        0        0     3990 2023-07-19 17:37:38.069228 fabric-message-bus-1.6.0b2/README.md
--rwxr-xr-x   0        0        0      203 2023-07-19 17:37:38.069320 fabric-message-bus-1.6.0b2/clean.sh
--rw-r--r--   0        0        0     1560 2023-07-19 17:37:38.069425 fabric-message-bus-1.6.0b2/docker-compose-no-ssl-kafka.yaml
--rw-r--r--   0        0        0     2857 2023-07-19 17:37:38.069540 fabric-message-bus-1.6.0b2/docker-compose.yml
--rw-r--r--   0        0        0       24 2023-07-20 21:41:20.891028 fabric-message-bus-1.6.0b2/fabric_mb/__init__.py
--rw-r--r--   0        0        0        0 2023-07-19 17:37:38.069800 fabric-message-bus-1.6.0b2/fabric_mb/message_bus/__init__.py
--rw-r--r--   0        0        0     2089 2023-07-19 17:37:38.069982 fabric-message-bus-1.6.0b2/fabric_mb/message_bus/abc_mb_api.py
--rw-r--r--   0        0        0     5899 2023-07-19 17:37:38.070165 fabric-message-bus-1.6.0b2/fabric_mb/message_bus/admin.py
--rw-r--r--   0        0        0     5881 2023-07-19 17:37:38.070360 fabric-message-bus-1.6.0b2/fabric_mb/message_bus/consumer.py
--rw-r--r--   0        0        0     1301 2023-07-19 17:37:38.070495 fabric-message-bus-1.6.0b2/fabric_mb/message_bus/message_bus_exception.py
--rw-r--r--   0        0        0        0 2023-07-19 17:37:38.070605 fabric-message-bus-1.6.0b2/fabric_mb/message_bus/messages/__init__.py
--rw-r--r--   0        0        0     8272 2023-07-19 17:40:51.541264 fabric-message-bus-1.6.0b2/fabric_mb/message_bus/messages/abc_message_avro.py
--rw-r--r--   0        0        0     3915 2023-07-19 17:37:38.071220 fabric-message-bus-1.6.0b2/fabric_mb/message_bus/messages/abc_object_avro.py
--rw-r--r--   0        0        0     6737 2023-07-19 17:37:38.071430 fabric-message-bus-1.6.0b2/fabric_mb/message_bus/messages/actor_avro.py
--rw-r--r--   0        0        0     2306 2023-07-19 17:37:38.071648 fabric-message-bus-1.6.0b2/fabric_mb/message_bus/messages/add_peer_avro.py
--rw-r--r--   0        0        0     1620 2023-07-19 17:37:38.071886 fabric-message-bus-1.6.0b2/fabric_mb/message_bus/messages/add_reservation_avro.py
--rw-r--r--   0        0        0     3647 2023-07-19 17:37:38.072020 fabric-message-bus-1.6.0b2/fabric_mb/message_bus/messages/add_reservations_avro.py
--rw-r--r--   0        0        0     1578 2023-07-19 17:37:38.072149 fabric-message-bus-1.6.0b2/fabric_mb/message_bus/messages/add_slice_avro.py
--rw-r--r--   0        0        0     3815 2023-07-19 17:37:38.072280 fabric-message-bus-1.6.0b2/fabric_mb/message_bus/messages/add_update_reservation_record.py
--rw-r--r--   0        0        0     3068 2023-07-19 17:37:38.072424 fabric-message-bus-1.6.0b2/fabric_mb/message_bus/messages/add_update_slice_record.py
--rw-r--r--   0        0        0     2077 2023-07-19 17:37:38.072561 fabric-message-bus-1.6.0b2/fabric_mb/message_bus/messages/auth_avro.py
--rw-r--r--   0        0        0     2275 2023-07-19 17:37:38.072723 fabric-message-bus-1.6.0b2/fabric_mb/message_bus/messages/broker_query_model_avro.py
--rw-r--r--   0        0        0     1965 2023-07-19 17:37:38.072837 fabric-message-bus-1.6.0b2/fabric_mb/message_bus/messages/claim_delegation_avro.py
--rw-r--r--   0        0        0     2036 2023-07-19 17:37:38.072988 fabric-message-bus-1.6.0b2/fabric_mb/message_bus/messages/claim_resources_avro.py
--rw-r--r--   0        0        0     1924 2023-07-19 17:37:38.073184 fabric-message-bus-1.6.0b2/fabric_mb/message_bus/messages/close_avro.py
--rw-r--r--   0        0        0     2025 2023-07-19 17:37:38.073383 fabric-message-bus-1.6.0b2/fabric_mb/message_bus/messages/close_delegations_avro.py
--rw-r--r--   0        0        0     2029 2023-07-19 17:37:38.073567 fabric-message-bus-1.6.0b2/fabric_mb/message_bus/messages/close_reservations_avro.py
--rw-r--r--   0        0        0     3122 2023-07-19 17:40:51.544986 fabric-message-bus-1.6.0b2/fabric_mb/message_bus/messages/constants.py
--rw-r--r--   0        0        0     3946 2023-07-19 17:37:38.074018 fabric-message-bus-1.6.0b2/fabric_mb/message_bus/messages/delegation_avro.py
--rw-r--r--   0        0        0     2063 2023-07-19 17:37:38.074227 fabric-message-bus-1.6.0b2/fabric_mb/message_bus/messages/demand_reservation_avro.py
--rw-r--r--   0        0        0     1950 2023-07-19 17:37:38.074424 fabric-message-bus-1.6.0b2/fabric_mb/message_bus/messages/extend_lease_avro.py
--rw-r--r--   0        0        0     3384 2023-07-19 17:37:38.074615 fabric-message-bus-1.6.0b2/fabric_mb/message_bus/messages/extend_reservation_avro.py
--rw-r--r--   0        0        0     1977 2023-07-19 17:37:38.074781 fabric-message-bus-1.6.0b2/fabric_mb/message_bus/messages/extend_ticket_avro.py
--rw-r--r--   0        0        0     2199 2023-07-19 17:37:38.074916 fabric-message-bus-1.6.0b2/fabric_mb/message_bus/messages/failed_rpc_avro.py
--rw-r--r--   0        0        0     1593 2023-07-19 17:37:38.075173 fabric-message-bus-1.6.0b2/fabric_mb/message_bus/messages/get_actors_request_avro.py
--rw-r--r--   0        0        0     1628 2023-07-19 17:37:38.075387 fabric-message-bus-1.6.0b2/fabric_mb/message_bus/messages/get_broker_query_model_request_avro.py
--rw-r--r--   0        0        0     1591 2023-07-19 17:37:38.075593 fabric-message-bus-1.6.0b2/fabric_mb/message_bus/messages/get_delegations_avro.py
--rw-r--r--   0        0        0     2016 2023-07-19 17:37:38.075724 fabric-message-bus-1.6.0b2/fabric_mb/message_bus/messages/get_reservation_units_request_avro.py
--rw-r--r--   0        0        0     1967 2023-07-19 17:37:38.075887 fabric-message-bus-1.6.0b2/fabric_mb/message_bus/messages/get_reservations_request_avro.py
--rw-r--r--   0        0        0     2544 2023-07-19 17:37:38.076013 fabric-message-bus-1.6.0b2/fabric_mb/message_bus/messages/get_reservations_state_request_avro.py
--rw-r--r--   0        0        0     1939 2023-07-19 17:37:38.076256 fabric-message-bus-1.6.0b2/fabric_mb/message_bus/messages/get_sites_request_avro.py
--rw-r--r--   0        0        0     1943 2023-07-19 17:37:38.076446 fabric-message-bus-1.6.0b2/fabric_mb/message_bus/messages/get_slices_request_avro.py
--rw-r--r--   0        0        0     1959 2023-07-19 17:37:38.076663 fabric-message-bus-1.6.0b2/fabric_mb/message_bus/messages/get_unit_request_avro.py
--rw-r--r--   0        0        0     5914 2023-07-19 17:37:38.076794 fabric-message-bus-1.6.0b2/fabric_mb/message_bus/messages/lease_reservation_avro.py
--rw-r--r--   0        0        0     1891 2023-07-19 17:37:38.077069 fabric-message-bus-1.6.0b2/fabric_mb/message_bus/messages/lease_reservation_state_avro.py
--rw-r--r--   0        0        0     3444 2023-07-19 17:37:38.077333 fabric-message-bus-1.6.0b2/fabric_mb/message_bus/messages/maintenance_request_avro.py
--rw-r--r--   0        0        0     1970 2023-07-19 17:37:38.077473 fabric-message-bus-1.6.0b2/fabric_mb/message_bus/messages/modify_lease_avro.py
--rw-r--r--   0        0        0     3804 2023-07-20 21:41:20.899001 fabric-message-bus-1.6.0b2/fabric_mb/message_bus/messages/poa_avro.py
--rw-r--r--   0        0        0     2961 2023-07-19 17:37:38.077945 fabric-message-bus-1.6.0b2/fabric_mb/message_bus/messages/poa_info_avro.py
--rw-r--r--   0        0        0     3103 2023-07-19 17:37:38.078078 fabric-message-bus-1.6.0b2/fabric_mb/message_bus/messages/proxy_avro.py
--rw-r--r--   0        0        0     2020 2023-07-19 17:37:38.078394 fabric-message-bus-1.6.0b2/fabric_mb/message_bus/messages/query_avro.py
--rw-r--r--   0        0        0     1904 2023-07-19 17:37:38.078562 fabric-message-bus-1.6.0b2/fabric_mb/message_bus/messages/query_result_avro.py
--rw-r--r--   0        0        0     1972 2023-07-19 17:37:38.078709 fabric-message-bus-1.6.0b2/fabric_mb/message_bus/messages/reclaim_delegation_avro.py
--rw-r--r--   0        0        0     2043 2023-07-19 17:37:38.078863 fabric-message-bus-1.6.0b2/fabric_mb/message_bus/messages/reclaim_resources_avro.py
--rw-r--r--   0        0        0     1948 2023-07-19 17:37:38.078960 fabric-message-bus-1.6.0b2/fabric_mb/message_bus/messages/redeem_avro.py
--rw-r--r--   0        0        0     1964 2023-07-19 17:37:38.079122 fabric-message-bus-1.6.0b2/fabric_mb/message_bus/messages/relinquish_avro.py
--rw-r--r--   0        0        0     1995 2023-07-19 17:37:38.079247 fabric-message-bus-1.6.0b2/fabric_mb/message_bus/messages/remove_delegation_avro.py
--rw-r--r--   0        0        0     1982 2023-07-19 17:37:38.079403 fabric-message-bus-1.6.0b2/fabric_mb/message_bus/messages/remove_reservation_avro.py
--rw-r--r--   0        0        0     1952 2023-07-19 17:37:38.079604 fabric-message-bus-1.6.0b2/fabric_mb/message_bus/messages/remove_slice_avro.py
--rw-r--r--   0        0        0     4120 2023-07-19 17:37:38.079862 fabric-message-bus-1.6.0b2/fabric_mb/message_bus/messages/request_by_id_record.py
--rw-r--r--   0        0        0     3019 2023-07-19 17:37:38.080019 fabric-message-bus-1.6.0b2/fabric_mb/message_bus/messages/reservation_avro.py
--rw-r--r--   0        0        0     7721 2023-07-19 17:37:38.080225 fabric-message-bus-1.6.0b2/fabric_mb/message_bus/messages/reservation_mng.py
--rw-r--r--   0        0        0     3126 2023-07-19 17:37:38.080339 fabric-message-bus-1.6.0b2/fabric_mb/message_bus/messages/reservation_or_delegation_record.py
--rw-r--r--   0        0        0     2059 2023-07-19 17:37:38.080472 fabric-message-bus-1.6.0b2/fabric_mb/message_bus/messages/reservation_predecessor_avro.py
--rw-r--r--   0        0        0     2513 2023-07-19 17:37:38.080611 fabric-message-bus-1.6.0b2/fabric_mb/message_bus/messages/reservation_state_avro.py
--rw-r--r--   0        0        0     3193 2023-07-19 17:37:38.080718 fabric-message-bus-1.6.0b2/fabric_mb/message_bus/messages/resource_set_avro.py
--rw-r--r--   0        0        0     3431 2023-07-19 17:37:38.080833 fabric-message-bus-1.6.0b2/fabric_mb/message_bus/messages/resource_ticket_avro.py
--rw-r--r--   0        0        0     1587 2023-07-19 17:37:38.081228 fabric-message-bus-1.6.0b2/fabric_mb/message_bus/messages/result_actor_avro.py
--rw-r--r--   0        0        0     2550 2023-07-19 17:37:38.081448 fabric-message-bus-1.6.0b2/fabric_mb/message_bus/messages/result_avro.py
--rw-r--r--   0        0        0     1625 2023-07-19 17:37:38.081577 fabric-message-bus-1.6.0b2/fabric_mb/message_bus/messages/result_broker_query_model_avro.py
--rw-r--r--   0        0        0     1607 2023-07-19 17:37:38.081676 fabric-message-bus-1.6.0b2/fabric_mb/message_bus/messages/result_delegation_avro.py
--rw-r--r--   0        0        0     1581 2023-07-19 17:37:38.081772 fabric-message-bus-1.6.0b2/fabric_mb/message_bus/messages/result_poa_avro.py
--rw-r--r--   0        0        0     1588 2023-07-19 17:37:38.081876 fabric-message-bus-1.6.0b2/fabric_mb/message_bus/messages/result_proxy_avro.py
--rw-r--r--   0        0        0    11980 2023-07-19 17:37:38.081977 fabric-message-bus-1.6.0b2/fabric_mb/message_bus/messages/result_record_list.py
--rw-r--r--   0        0        0     1611 2023-07-19 17:37:38.082140 fabric-message-bus-1.6.0b2/fabric_mb/message_bus/messages/result_reservation_avro.py
--rw-r--r--   0        0        0     1633 2023-07-19 17:37:38.082317 fabric-message-bus-1.6.0b2/fabric_mb/message_bus/messages/result_reservation_state_avro.py
--rw-r--r--   0        0        0     1662 2023-07-19 17:37:38.082460 fabric-message-bus-1.6.0b2/fabric_mb/message_bus/messages/result_sites_avro.py
--rw-r--r--   0        0        0     1587 2023-07-19 17:37:38.082601 fabric-message-bus-1.6.0b2/fabric_mb/message_bus/messages/result_slice_avro.py
--rw-r--r--   0        0        0     3167 2023-07-19 17:37:38.082715 fabric-message-bus-1.6.0b2/fabric_mb/message_bus/messages/result_string_avro.py
--rw-r--r--   0        0        0     3191 2023-07-19 17:37:38.082828 fabric-message-bus-1.6.0b2/fabric_mb/message_bus/messages/result_strings_avro.py
--rw-r--r--   0        0        0     1662 2023-07-19 17:37:38.082926 fabric-message-bus-1.6.0b2/fabric_mb/message_bus/messages/result_units_avro.py
--rw-r--r--   0        0        0     1900 2023-07-19 17:37:38.083029 fabric-message-bus-1.6.0b2/fabric_mb/message_bus/messages/site_avro.py
--rw-r--r--   0        0        0     8670 2023-07-19 17:37:38.083151 fabric-message-bus-1.6.0b2/fabric_mb/message_bus/messages/slice_avro.py
--rw-r--r--   0        0        0     1844 2023-07-19 17:37:38.083256 fabric-message-bus-1.6.0b2/fabric_mb/message_bus/messages/term_avro.py
--rw-r--r--   0        0        0     3474 2023-07-19 17:37:38.083477 fabric-message-bus-1.6.0b2/fabric_mb/message_bus/messages/ticket.py
--rw-r--r--   0        0        0     2810 2023-07-19 17:37:38.083602 fabric-message-bus-1.6.0b2/fabric_mb/message_bus/messages/ticket_avro.py
--rw-r--r--   0        0        0     4436 2023-07-19 17:37:38.083737 fabric-message-bus-1.6.0b2/fabric_mb/message_bus/messages/ticket_reservation_avro.py
--rw-r--r--   0        0        0     3512 2023-07-19 17:37:38.083848 fabric-message-bus-1.6.0b2/fabric_mb/message_bus/messages/unit_avro.py
--rw-r--r--   0        0        0     1759 2023-07-19 17:37:38.084005 fabric-message-bus-1.6.0b2/fabric_mb/message_bus/messages/update_data_avro.py
--rw-r--r--   0        0        0     1969 2023-07-19 17:37:38.084107 fabric-message-bus-1.6.0b2/fabric_mb/message_bus/messages/update_delegation_avro.py
--rw-r--r--   0        0        0     1971 2023-07-19 17:37:38.084211 fabric-message-bus-1.6.0b2/fabric_mb/message_bus/messages/update_lease_avro.py
--rw-r--r--   0        0        0     1631 2023-07-19 17:37:38.084357 fabric-message-bus-1.6.0b2/fabric_mb/message_bus/messages/update_reservation_avro.py
--rw-r--r--   0        0        0     1588 2023-07-19 17:37:38.084572 fabric-message-bus-1.6.0b2/fabric_mb/message_bus/messages/update_slice_avro.py
--rw-r--r--   0        0        0     1975 2023-07-19 17:37:38.084693 fabric-message-bus-1.6.0b2/fabric_mb/message_bus/messages/update_ticket_avro.py
--rw-r--r--   0        0        0     7894 2023-07-19 17:37:38.084799 fabric-message-bus-1.6.0b2/fabric_mb/message_bus/producer.py
--rw-r--r--   0        0        0       92 2023-07-19 17:37:38.084949 fabric-message-bus-1.6.0b2/fabric_mb/message_bus/schema/key.avsc
--rw-r--r--   0        0        0    30908 2023-07-19 17:38:26.148106 fabric-message-bus-1.6.0b2/fabric_mb/message_bus/schema/message.avsc
--rw-r--r--   0        0        0        0 2023-07-19 17:37:38.085420 fabric-message-bus-1.6.0b2/fabric_mb/message_bus/test/__init__.py
--rw-r--r--   0        0        0    15232 2023-07-19 17:37:38.085549 fabric-message-bus-1.6.0b2/fabric_mb/message_bus/test/abqm.graphml
--rw-r--r--   0        0        0    44737 2023-07-19 17:37:38.085809 fabric-message-bus-1.6.0b2/fabric_mb/message_bus/test/message_bus_test.py
--rw-r--r--   0        0        0      747 2023-07-19 17:37:38.085943 fabric-message-bus-1.6.0b2/pyproject.toml
--rwxr-xr-x   0        0        0     2190 2023-07-19 17:37:38.086123 fabric-message-bus-1.6.0b2/secrets/create-certs.sh
--rw-r--r--   0        0        0     4553 1970-01-01 00:00:00.000000 fabric-message-bus-1.6.0b2/PKG-INFO
+-rw-r--r--   0        0        0     1856 2023-07-19 17:37:38.068966 fabric-message-bus-1.6.0b3/.gitignore
+-rw-r--r--   0        0        0     1071 2023-07-19 17:37:38.069108 fabric-message-bus-1.6.0b3/LICENSE
+-rw-r--r--   0        0        0     3990 2023-07-19 17:37:38.069228 fabric-message-bus-1.6.0b3/README.md
+-rwxr-xr-x   0        0        0      203 2023-07-19 17:37:38.069320 fabric-message-bus-1.6.0b3/clean.sh
+-rw-r--r--   0        0        0     1560 2023-07-19 17:37:38.069425 fabric-message-bus-1.6.0b3/docker-compose-no-ssl-kafka.yaml
+-rw-r--r--   0        0        0     2857 2023-07-19 17:37:38.069540 fabric-message-bus-1.6.0b3/docker-compose.yml
+-rw-r--r--   0        0        0       24 2023-07-21 13:30:51.103968 fabric-message-bus-1.6.0b3/fabric_mb/__init__.py
+-rw-r--r--   0        0        0        0 2023-07-19 17:37:38.069800 fabric-message-bus-1.6.0b3/fabric_mb/message_bus/__init__.py
+-rw-r--r--   0        0        0     2089 2023-07-19 17:37:38.069982 fabric-message-bus-1.6.0b3/fabric_mb/message_bus/abc_mb_api.py
+-rw-r--r--   0        0        0     5899 2023-07-19 17:37:38.070165 fabric-message-bus-1.6.0b3/fabric_mb/message_bus/admin.py
+-rw-r--r--   0        0        0     5881 2023-07-19 17:37:38.070360 fabric-message-bus-1.6.0b3/fabric_mb/message_bus/consumer.py
+-rw-r--r--   0        0        0     1301 2023-07-19 17:37:38.070495 fabric-message-bus-1.6.0b3/fabric_mb/message_bus/message_bus_exception.py
+-rw-r--r--   0        0        0        0 2023-07-19 17:37:38.070605 fabric-message-bus-1.6.0b3/fabric_mb/message_bus/messages/__init__.py
+-rw-r--r--   0        0        0     8272 2023-07-19 17:40:51.541264 fabric-message-bus-1.6.0b3/fabric_mb/message_bus/messages/abc_message_avro.py
+-rw-r--r--   0        0        0     3915 2023-07-19 17:37:38.071220 fabric-message-bus-1.6.0b3/fabric_mb/message_bus/messages/abc_object_avro.py
+-rw-r--r--   0        0        0     6737 2023-07-19 17:37:38.071430 fabric-message-bus-1.6.0b3/fabric_mb/message_bus/messages/actor_avro.py
+-rw-r--r--   0        0        0     2306 2023-07-19 17:37:38.071648 fabric-message-bus-1.6.0b3/fabric_mb/message_bus/messages/add_peer_avro.py
+-rw-r--r--   0        0        0     1620 2023-07-19 17:37:38.071886 fabric-message-bus-1.6.0b3/fabric_mb/message_bus/messages/add_reservation_avro.py
+-rw-r--r--   0        0        0     3647 2023-07-19 17:37:38.072020 fabric-message-bus-1.6.0b3/fabric_mb/message_bus/messages/add_reservations_avro.py
+-rw-r--r--   0        0        0     1578 2023-07-19 17:37:38.072149 fabric-message-bus-1.6.0b3/fabric_mb/message_bus/messages/add_slice_avro.py
+-rw-r--r--   0        0        0     3815 2023-07-19 17:37:38.072280 fabric-message-bus-1.6.0b3/fabric_mb/message_bus/messages/add_update_reservation_record.py
+-rw-r--r--   0        0        0     3068 2023-07-19 17:37:38.072424 fabric-message-bus-1.6.0b3/fabric_mb/message_bus/messages/add_update_slice_record.py
+-rw-r--r--   0        0        0     2077 2023-07-19 17:37:38.072561 fabric-message-bus-1.6.0b3/fabric_mb/message_bus/messages/auth_avro.py
+-rw-r--r--   0        0        0     2275 2023-07-19 17:37:38.072723 fabric-message-bus-1.6.0b3/fabric_mb/message_bus/messages/broker_query_model_avro.py
+-rw-r--r--   0        0        0     1965 2023-07-19 17:37:38.072837 fabric-message-bus-1.6.0b3/fabric_mb/message_bus/messages/claim_delegation_avro.py
+-rw-r--r--   0        0        0     2036 2023-07-19 17:37:38.072988 fabric-message-bus-1.6.0b3/fabric_mb/message_bus/messages/claim_resources_avro.py
+-rw-r--r--   0        0        0     1924 2023-07-19 17:37:38.073184 fabric-message-bus-1.6.0b3/fabric_mb/message_bus/messages/close_avro.py
+-rw-r--r--   0        0        0     2025 2023-07-19 17:37:38.073383 fabric-message-bus-1.6.0b3/fabric_mb/message_bus/messages/close_delegations_avro.py
+-rw-r--r--   0        0        0     2029 2023-07-19 17:37:38.073567 fabric-message-bus-1.6.0b3/fabric_mb/message_bus/messages/close_reservations_avro.py
+-rw-r--r--   0        0        0     3122 2023-07-19 17:40:51.544986 fabric-message-bus-1.6.0b3/fabric_mb/message_bus/messages/constants.py
+-rw-r--r--   0        0        0     3946 2023-07-19 17:37:38.074018 fabric-message-bus-1.6.0b3/fabric_mb/message_bus/messages/delegation_avro.py
+-rw-r--r--   0        0        0     2063 2023-07-19 17:37:38.074227 fabric-message-bus-1.6.0b3/fabric_mb/message_bus/messages/demand_reservation_avro.py
+-rw-r--r--   0        0        0     1950 2023-07-19 17:37:38.074424 fabric-message-bus-1.6.0b3/fabric_mb/message_bus/messages/extend_lease_avro.py
+-rw-r--r--   0        0        0     3384 2023-07-19 17:37:38.074615 fabric-message-bus-1.6.0b3/fabric_mb/message_bus/messages/extend_reservation_avro.py
+-rw-r--r--   0        0        0     1977 2023-07-19 17:37:38.074781 fabric-message-bus-1.6.0b3/fabric_mb/message_bus/messages/extend_ticket_avro.py
+-rw-r--r--   0        0        0     2199 2023-07-19 17:37:38.074916 fabric-message-bus-1.6.0b3/fabric_mb/message_bus/messages/failed_rpc_avro.py
+-rw-r--r--   0        0        0     1593 2023-07-19 17:37:38.075173 fabric-message-bus-1.6.0b3/fabric_mb/message_bus/messages/get_actors_request_avro.py
+-rw-r--r--   0        0        0     1628 2023-07-19 17:37:38.075387 fabric-message-bus-1.6.0b3/fabric_mb/message_bus/messages/get_broker_query_model_request_avro.py
+-rw-r--r--   0        0        0     1591 2023-07-19 17:37:38.075593 fabric-message-bus-1.6.0b3/fabric_mb/message_bus/messages/get_delegations_avro.py
+-rw-r--r--   0        0        0     2016 2023-07-19 17:37:38.075724 fabric-message-bus-1.6.0b3/fabric_mb/message_bus/messages/get_reservation_units_request_avro.py
+-rw-r--r--   0        0        0     1967 2023-07-19 17:37:38.075887 fabric-message-bus-1.6.0b3/fabric_mb/message_bus/messages/get_reservations_request_avro.py
+-rw-r--r--   0        0        0     2544 2023-07-19 17:37:38.076013 fabric-message-bus-1.6.0b3/fabric_mb/message_bus/messages/get_reservations_state_request_avro.py
+-rw-r--r--   0        0        0     1939 2023-07-19 17:37:38.076256 fabric-message-bus-1.6.0b3/fabric_mb/message_bus/messages/get_sites_request_avro.py
+-rw-r--r--   0        0        0     1943 2023-07-19 17:37:38.076446 fabric-message-bus-1.6.0b3/fabric_mb/message_bus/messages/get_slices_request_avro.py
+-rw-r--r--   0        0        0     1959 2023-07-19 17:37:38.076663 fabric-message-bus-1.6.0b3/fabric_mb/message_bus/messages/get_unit_request_avro.py
+-rw-r--r--   0        0        0     5914 2023-07-19 17:37:38.076794 fabric-message-bus-1.6.0b3/fabric_mb/message_bus/messages/lease_reservation_avro.py
+-rw-r--r--   0        0        0     1891 2023-07-19 17:37:38.077069 fabric-message-bus-1.6.0b3/fabric_mb/message_bus/messages/lease_reservation_state_avro.py
+-rw-r--r--   0        0        0     3444 2023-07-19 17:37:38.077333 fabric-message-bus-1.6.0b3/fabric_mb/message_bus/messages/maintenance_request_avro.py
+-rw-r--r--   0        0        0     1970 2023-07-19 17:37:38.077473 fabric-message-bus-1.6.0b3/fabric_mb/message_bus/messages/modify_lease_avro.py
+-rw-r--r--   0        0        0     3804 2023-07-20 21:41:20.899001 fabric-message-bus-1.6.0b3/fabric_mb/message_bus/messages/poa_avro.py
+-rw-r--r--   0        0        0     2961 2023-07-19 17:37:38.077945 fabric-message-bus-1.6.0b3/fabric_mb/message_bus/messages/poa_info_avro.py
+-rw-r--r--   0        0        0     3103 2023-07-19 17:37:38.078078 fabric-message-bus-1.6.0b3/fabric_mb/message_bus/messages/proxy_avro.py
+-rw-r--r--   0        0        0     2020 2023-07-19 17:37:38.078394 fabric-message-bus-1.6.0b3/fabric_mb/message_bus/messages/query_avro.py
+-rw-r--r--   0        0        0     1904 2023-07-19 17:37:38.078562 fabric-message-bus-1.6.0b3/fabric_mb/message_bus/messages/query_result_avro.py
+-rw-r--r--   0        0        0     1972 2023-07-19 17:37:38.078709 fabric-message-bus-1.6.0b3/fabric_mb/message_bus/messages/reclaim_delegation_avro.py
+-rw-r--r--   0        0        0     2043 2023-07-19 17:37:38.078863 fabric-message-bus-1.6.0b3/fabric_mb/message_bus/messages/reclaim_resources_avro.py
+-rw-r--r--   0        0        0     1948 2023-07-19 17:37:38.078960 fabric-message-bus-1.6.0b3/fabric_mb/message_bus/messages/redeem_avro.py
+-rw-r--r--   0        0        0     1964 2023-07-19 17:37:38.079122 fabric-message-bus-1.6.0b3/fabric_mb/message_bus/messages/relinquish_avro.py
+-rw-r--r--   0        0        0     1995 2023-07-19 17:37:38.079247 fabric-message-bus-1.6.0b3/fabric_mb/message_bus/messages/remove_delegation_avro.py
+-rw-r--r--   0        0        0     1982 2023-07-19 17:37:38.079403 fabric-message-bus-1.6.0b3/fabric_mb/message_bus/messages/remove_reservation_avro.py
+-rw-r--r--   0        0        0     1952 2023-07-19 17:37:38.079604 fabric-message-bus-1.6.0b3/fabric_mb/message_bus/messages/remove_slice_avro.py
+-rw-r--r--   0        0        0     4120 2023-07-19 17:37:38.079862 fabric-message-bus-1.6.0b3/fabric_mb/message_bus/messages/request_by_id_record.py
+-rw-r--r--   0        0        0     3019 2023-07-19 17:37:38.080019 fabric-message-bus-1.6.0b3/fabric_mb/message_bus/messages/reservation_avro.py
+-rw-r--r--   0        0        0     7721 2023-07-19 17:37:38.080225 fabric-message-bus-1.6.0b3/fabric_mb/message_bus/messages/reservation_mng.py
+-rw-r--r--   0        0        0     3126 2023-07-19 17:37:38.080339 fabric-message-bus-1.6.0b3/fabric_mb/message_bus/messages/reservation_or_delegation_record.py
+-rw-r--r--   0        0        0     2059 2023-07-19 17:37:38.080472 fabric-message-bus-1.6.0b3/fabric_mb/message_bus/messages/reservation_predecessor_avro.py
+-rw-r--r--   0        0        0     2513 2023-07-19 17:37:38.080611 fabric-message-bus-1.6.0b3/fabric_mb/message_bus/messages/reservation_state_avro.py
+-rw-r--r--   0        0        0     3193 2023-07-19 17:37:38.080718 fabric-message-bus-1.6.0b3/fabric_mb/message_bus/messages/resource_set_avro.py
+-rw-r--r--   0        0        0     3431 2023-07-19 17:37:38.080833 fabric-message-bus-1.6.0b3/fabric_mb/message_bus/messages/resource_ticket_avro.py
+-rw-r--r--   0        0        0     1587 2023-07-19 17:37:38.081228 fabric-message-bus-1.6.0b3/fabric_mb/message_bus/messages/result_actor_avro.py
+-rw-r--r--   0        0        0     2550 2023-07-19 17:37:38.081448 fabric-message-bus-1.6.0b3/fabric_mb/message_bus/messages/result_avro.py
+-rw-r--r--   0        0        0     1625 2023-07-19 17:37:38.081577 fabric-message-bus-1.6.0b3/fabric_mb/message_bus/messages/result_broker_query_model_avro.py
+-rw-r--r--   0        0        0     1607 2023-07-19 17:37:38.081676 fabric-message-bus-1.6.0b3/fabric_mb/message_bus/messages/result_delegation_avro.py
+-rw-r--r--   0        0        0     1581 2023-07-19 17:37:38.081772 fabric-message-bus-1.6.0b3/fabric_mb/message_bus/messages/result_poa_avro.py
+-rw-r--r--   0        0        0     1588 2023-07-19 17:37:38.081876 fabric-message-bus-1.6.0b3/fabric_mb/message_bus/messages/result_proxy_avro.py
+-rw-r--r--   0        0        0    11980 2023-07-19 17:37:38.081977 fabric-message-bus-1.6.0b3/fabric_mb/message_bus/messages/result_record_list.py
+-rw-r--r--   0        0        0     1611 2023-07-19 17:37:38.082140 fabric-message-bus-1.6.0b3/fabric_mb/message_bus/messages/result_reservation_avro.py
+-rw-r--r--   0        0        0     1633 2023-07-19 17:37:38.082317 fabric-message-bus-1.6.0b3/fabric_mb/message_bus/messages/result_reservation_state_avro.py
+-rw-r--r--   0        0        0     1662 2023-07-19 17:37:38.082460 fabric-message-bus-1.6.0b3/fabric_mb/message_bus/messages/result_sites_avro.py
+-rw-r--r--   0        0        0     1587 2023-07-19 17:37:38.082601 fabric-message-bus-1.6.0b3/fabric_mb/message_bus/messages/result_slice_avro.py
+-rw-r--r--   0        0        0     3167 2023-07-19 17:37:38.082715 fabric-message-bus-1.6.0b3/fabric_mb/message_bus/messages/result_string_avro.py
+-rw-r--r--   0        0        0     3191 2023-07-19 17:37:38.082828 fabric-message-bus-1.6.0b3/fabric_mb/message_bus/messages/result_strings_avro.py
+-rw-r--r--   0        0        0     1662 2023-07-19 17:37:38.082926 fabric-message-bus-1.6.0b3/fabric_mb/message_bus/messages/result_units_avro.py
+-rw-r--r--   0        0        0     1900 2023-07-19 17:37:38.083029 fabric-message-bus-1.6.0b3/fabric_mb/message_bus/messages/site_avro.py
+-rw-r--r--   0        0        0     8670 2023-07-19 17:37:38.083151 fabric-message-bus-1.6.0b3/fabric_mb/message_bus/messages/slice_avro.py
+-rw-r--r--   0        0        0     1844 2023-07-19 17:37:38.083256 fabric-message-bus-1.6.0b3/fabric_mb/message_bus/messages/term_avro.py
+-rw-r--r--   0        0        0     3474 2023-07-19 17:37:38.083477 fabric-message-bus-1.6.0b3/fabric_mb/message_bus/messages/ticket.py
+-rw-r--r--   0        0        0     2810 2023-07-19 17:37:38.083602 fabric-message-bus-1.6.0b3/fabric_mb/message_bus/messages/ticket_avro.py
+-rw-r--r--   0        0        0     4436 2023-07-19 17:37:38.083737 fabric-message-bus-1.6.0b3/fabric_mb/message_bus/messages/ticket_reservation_avro.py
+-rw-r--r--   0        0        0     3512 2023-07-19 17:37:38.083848 fabric-message-bus-1.6.0b3/fabric_mb/message_bus/messages/unit_avro.py
+-rw-r--r--   0        0        0     1759 2023-07-19 17:37:38.084005 fabric-message-bus-1.6.0b3/fabric_mb/message_bus/messages/update_data_avro.py
+-rw-r--r--   0        0        0     1969 2023-07-19 17:37:38.084107 fabric-message-bus-1.6.0b3/fabric_mb/message_bus/messages/update_delegation_avro.py
+-rw-r--r--   0        0        0     1971 2023-07-19 17:37:38.084211 fabric-message-bus-1.6.0b3/fabric_mb/message_bus/messages/update_lease_avro.py
+-rw-r--r--   0        0        0     1631 2023-07-19 17:37:38.084357 fabric-message-bus-1.6.0b3/fabric_mb/message_bus/messages/update_reservation_avro.py
+-rw-r--r--   0        0        0     1588 2023-07-19 17:37:38.084572 fabric-message-bus-1.6.0b3/fabric_mb/message_bus/messages/update_slice_avro.py
+-rw-r--r--   0        0        0     1975 2023-07-19 17:37:38.084693 fabric-message-bus-1.6.0b3/fabric_mb/message_bus/messages/update_ticket_avro.py
+-rw-r--r--   0        0        0     7894 2023-07-19 17:37:38.084799 fabric-message-bus-1.6.0b3/fabric_mb/message_bus/producer.py
+-rw-r--r--   0        0        0       92 2023-07-19 17:37:38.084949 fabric-message-bus-1.6.0b3/fabric_mb/message_bus/schema/key.avsc
+-rw-r--r--   0        0        0    30908 2023-07-19 17:38:26.148106 fabric-message-bus-1.6.0b3/fabric_mb/message_bus/schema/message.avsc
+-rw-r--r--   0        0        0        0 2023-07-19 17:37:38.085420 fabric-message-bus-1.6.0b3/fabric_mb/message_bus/test/__init__.py
+-rw-r--r--   0        0        0    15232 2023-07-19 17:37:38.085549 fabric-message-bus-1.6.0b3/fabric_mb/message_bus/test/abqm.graphml
+-rw-r--r--   0        0        0    44737 2023-07-19 17:37:38.085809 fabric-message-bus-1.6.0b3/fabric_mb/message_bus/test/message_bus_test.py
+-rw-r--r--   0        0        0      747 2023-07-19 17:37:38.085943 fabric-message-bus-1.6.0b3/pyproject.toml
+-rwxr-xr-x   0        0        0     2190 2023-07-19 17:37:38.086123 fabric-message-bus-1.6.0b3/secrets/create-certs.sh
+-rw-r--r--   0        0        0     4553 1970-01-01 00:00:00.000000 fabric-message-bus-1.6.0b3/PKG-INFO
```

### Comparing `fabric-message-bus-1.6.0b2/.gitignore` & `fabric-message-bus-1.6.0b3/.gitignore`

 * *Files identical despite different names*

### Comparing `fabric-message-bus-1.6.0b2/LICENSE` & `fabric-message-bus-1.6.0b3/LICENSE`

 * *Files identical despite different names*

### Comparing `fabric-message-bus-1.6.0b2/README.md` & `fabric-message-bus-1.6.0b3/README.md`

 * *Files identical despite different names*

### Comparing `fabric-message-bus-1.6.0b2/docker-compose-no-ssl-kafka.yaml` & `fabric-message-bus-1.6.0b3/docker-compose-no-ssl-kafka.yaml`

 * *Files identical despite different names*

### Comparing `fabric-message-bus-1.6.0b2/docker-compose.yml` & `fabric-message-bus-1.6.0b3/docker-compose.yml`

 * *Files identical despite different names*

### Comparing `fabric-message-bus-1.6.0b2/fabric_mb/message_bus/abc_mb_api.py` & `fabric-message-bus-1.6.0b3/fabric_mb/message_bus/abc_mb_api.py`

 * *Files identical despite different names*

### Comparing `fabric-message-bus-1.6.0b2/fabric_mb/message_bus/admin.py` & `fabric-message-bus-1.6.0b3/fabric_mb/message_bus/admin.py`

 * *Files identical despite different names*

### Comparing `fabric-message-bus-1.6.0b2/fabric_mb/message_bus/consumer.py` & `fabric-message-bus-1.6.0b3/fabric_mb/message_bus/consumer.py`

 * *Files identical despite different names*

### Comparing `fabric-message-bus-1.6.0b2/fabric_mb/message_bus/message_bus_exception.py` & `fabric-message-bus-1.6.0b3/fabric_mb/message_bus/message_bus_exception.py`

 * *Files identical despite different names*

### Comparing `fabric-message-bus-1.6.0b2/fabric_mb/message_bus/messages/abc_message_avro.py` & `fabric-message-bus-1.6.0b3/fabric_mb/message_bus/messages/abc_message_avro.py`

 * *Files identical despite different names*

### Comparing `fabric-message-bus-1.6.0b2/fabric_mb/message_bus/messages/abc_object_avro.py` & `fabric-message-bus-1.6.0b3/fabric_mb/message_bus/messages/abc_object_avro.py`

 * *Files identical despite different names*

### Comparing `fabric-message-bus-1.6.0b2/fabric_mb/message_bus/messages/actor_avro.py` & `fabric-message-bus-1.6.0b3/fabric_mb/message_bus/messages/actor_avro.py`

 * *Files identical despite different names*

### Comparing `fabric-message-bus-1.6.0b2/fabric_mb/message_bus/messages/add_peer_avro.py` & `fabric-message-bus-1.6.0b3/fabric_mb/message_bus/messages/add_peer_avro.py`

 * *Files identical despite different names*

### Comparing `fabric-message-bus-1.6.0b2/fabric_mb/message_bus/messages/add_reservation_avro.py` & `fabric-message-bus-1.6.0b3/fabric_mb/message_bus/messages/add_reservation_avro.py`

 * *Files identical despite different names*

### Comparing `fabric-message-bus-1.6.0b2/fabric_mb/message_bus/messages/add_reservations_avro.py` & `fabric-message-bus-1.6.0b3/fabric_mb/message_bus/messages/add_reservations_avro.py`

 * *Files identical despite different names*

### Comparing `fabric-message-bus-1.6.0b2/fabric_mb/message_bus/messages/add_slice_avro.py` & `fabric-message-bus-1.6.0b3/fabric_mb/message_bus/messages/add_slice_avro.py`

 * *Files identical despite different names*

### Comparing `fabric-message-bus-1.6.0b2/fabric_mb/message_bus/messages/add_update_reservation_record.py` & `fabric-message-bus-1.6.0b3/fabric_mb/message_bus/messages/add_update_reservation_record.py`

 * *Files identical despite different names*

### Comparing `fabric-message-bus-1.6.0b2/fabric_mb/message_bus/messages/add_update_slice_record.py` & `fabric-message-bus-1.6.0b3/fabric_mb/message_bus/messages/add_update_slice_record.py`

 * *Files identical despite different names*

### Comparing `fabric-message-bus-1.6.0b2/fabric_mb/message_bus/messages/auth_avro.py` & `fabric-message-bus-1.6.0b3/fabric_mb/message_bus/messages/auth_avro.py`

 * *Files identical despite different names*

### Comparing `fabric-message-bus-1.6.0b2/fabric_mb/message_bus/messages/broker_query_model_avro.py` & `fabric-message-bus-1.6.0b3/fabric_mb/message_bus/messages/broker_query_model_avro.py`

 * *Files identical despite different names*

### Comparing `fabric-message-bus-1.6.0b2/fabric_mb/message_bus/messages/claim_delegation_avro.py` & `fabric-message-bus-1.6.0b3/fabric_mb/message_bus/messages/claim_delegation_avro.py`

 * *Files identical despite different names*

### Comparing `fabric-message-bus-1.6.0b2/fabric_mb/message_bus/messages/claim_resources_avro.py` & `fabric-message-bus-1.6.0b3/fabric_mb/message_bus/messages/claim_resources_avro.py`

 * *Files identical despite different names*

### Comparing `fabric-message-bus-1.6.0b2/fabric_mb/message_bus/messages/close_avro.py` & `fabric-message-bus-1.6.0b3/fabric_mb/message_bus/messages/close_avro.py`

 * *Files identical despite different names*

### Comparing `fabric-message-bus-1.6.0b2/fabric_mb/message_bus/messages/close_delegations_avro.py` & `fabric-message-bus-1.6.0b3/fabric_mb/message_bus/messages/close_delegations_avro.py`

 * *Files identical despite different names*

### Comparing `fabric-message-bus-1.6.0b2/fabric_mb/message_bus/messages/close_reservations_avro.py` & `fabric-message-bus-1.6.0b3/fabric_mb/message_bus/messages/close_reservations_avro.py`

 * *Files identical despite different names*

### Comparing `fabric-message-bus-1.6.0b2/fabric_mb/message_bus/messages/constants.py` & `fabric-message-bus-1.6.0b3/fabric_mb/message_bus/messages/constants.py`

 * *Files identical despite different names*

### Comparing `fabric-message-bus-1.6.0b2/fabric_mb/message_bus/messages/delegation_avro.py` & `fabric-message-bus-1.6.0b3/fabric_mb/message_bus/messages/delegation_avro.py`

 * *Files identical despite different names*

### Comparing `fabric-message-bus-1.6.0b2/fabric_mb/message_bus/messages/demand_reservation_avro.py` & `fabric-message-bus-1.6.0b3/fabric_mb/message_bus/messages/demand_reservation_avro.py`

 * *Files identical despite different names*

### Comparing `fabric-message-bus-1.6.0b2/fabric_mb/message_bus/messages/extend_lease_avro.py` & `fabric-message-bus-1.6.0b3/fabric_mb/message_bus/messages/extend_lease_avro.py`

 * *Files identical despite different names*

### Comparing `fabric-message-bus-1.6.0b2/fabric_mb/message_bus/messages/extend_reservation_avro.py` & `fabric-message-bus-1.6.0b3/fabric_mb/message_bus/messages/extend_reservation_avro.py`

 * *Files identical despite different names*

### Comparing `fabric-message-bus-1.6.0b2/fabric_mb/message_bus/messages/extend_ticket_avro.py` & `fabric-message-bus-1.6.0b3/fabric_mb/message_bus/messages/extend_ticket_avro.py`

 * *Files identical despite different names*

### Comparing `fabric-message-bus-1.6.0b2/fabric_mb/message_bus/messages/failed_rpc_avro.py` & `fabric-message-bus-1.6.0b3/fabric_mb/message_bus/messages/failed_rpc_avro.py`

 * *Files identical despite different names*

### Comparing `fabric-message-bus-1.6.0b2/fabric_mb/message_bus/messages/get_actors_request_avro.py` & `fabric-message-bus-1.6.0b3/fabric_mb/message_bus/messages/get_actors_request_avro.py`

 * *Files identical despite different names*

### Comparing `fabric-message-bus-1.6.0b2/fabric_mb/message_bus/messages/get_broker_query_model_request_avro.py` & `fabric-message-bus-1.6.0b3/fabric_mb/message_bus/messages/get_broker_query_model_request_avro.py`

 * *Files identical despite different names*

### Comparing `fabric-message-bus-1.6.0b2/fabric_mb/message_bus/messages/get_delegations_avro.py` & `fabric-message-bus-1.6.0b3/fabric_mb/message_bus/messages/get_delegations_avro.py`

 * *Files identical despite different names*

### Comparing `fabric-message-bus-1.6.0b2/fabric_mb/message_bus/messages/get_reservation_units_request_avro.py` & `fabric-message-bus-1.6.0b3/fabric_mb/message_bus/messages/get_reservation_units_request_avro.py`

 * *Files identical despite different names*

### Comparing `fabric-message-bus-1.6.0b2/fabric_mb/message_bus/messages/get_reservations_request_avro.py` & `fabric-message-bus-1.6.0b3/fabric_mb/message_bus/messages/get_reservations_request_avro.py`

 * *Files identical despite different names*

### Comparing `fabric-message-bus-1.6.0b2/fabric_mb/message_bus/messages/get_reservations_state_request_avro.py` & `fabric-message-bus-1.6.0b3/fabric_mb/message_bus/messages/get_reservations_state_request_avro.py`

 * *Files identical despite different names*

### Comparing `fabric-message-bus-1.6.0b2/fabric_mb/message_bus/messages/get_sites_request_avro.py` & `fabric-message-bus-1.6.0b3/fabric_mb/message_bus/messages/get_sites_request_avro.py`

 * *Files identical despite different names*

### Comparing `fabric-message-bus-1.6.0b2/fabric_mb/message_bus/messages/get_slices_request_avro.py` & `fabric-message-bus-1.6.0b3/fabric_mb/message_bus/messages/get_slices_request_avro.py`

 * *Files identical despite different names*

### Comparing `fabric-message-bus-1.6.0b2/fabric_mb/message_bus/messages/get_unit_request_avro.py` & `fabric-message-bus-1.6.0b3/fabric_mb/message_bus/messages/get_unit_request_avro.py`

 * *Files identical despite different names*

### Comparing `fabric-message-bus-1.6.0b2/fabric_mb/message_bus/messages/lease_reservation_avro.py` & `fabric-message-bus-1.6.0b3/fabric_mb/message_bus/messages/lease_reservation_avro.py`

 * *Files identical despite different names*

### Comparing `fabric-message-bus-1.6.0b2/fabric_mb/message_bus/messages/lease_reservation_state_avro.py` & `fabric-message-bus-1.6.0b3/fabric_mb/message_bus/messages/lease_reservation_state_avro.py`

 * *Files identical despite different names*

### Comparing `fabric-message-bus-1.6.0b2/fabric_mb/message_bus/messages/maintenance_request_avro.py` & `fabric-message-bus-1.6.0b3/fabric_mb/message_bus/messages/maintenance_request_avro.py`

 * *Files identical despite different names*

### Comparing `fabric-message-bus-1.6.0b2/fabric_mb/message_bus/messages/modify_lease_avro.py` & `fabric-message-bus-1.6.0b3/fabric_mb/message_bus/messages/modify_lease_avro.py`

 * *Files identical despite different names*

### Comparing `fabric-message-bus-1.6.0b2/fabric_mb/message_bus/messages/poa_avro.py` & `fabric-message-bus-1.6.0b3/fabric_mb/message_bus/messages/poa_avro.py`

 * *Files identical despite different names*

### Comparing `fabric-message-bus-1.6.0b2/fabric_mb/message_bus/messages/poa_info_avro.py` & `fabric-message-bus-1.6.0b3/fabric_mb/message_bus/messages/poa_info_avro.py`

 * *Files identical despite different names*

### Comparing `fabric-message-bus-1.6.0b2/fabric_mb/message_bus/messages/proxy_avro.py` & `fabric-message-bus-1.6.0b3/fabric_mb/message_bus/messages/proxy_avro.py`

 * *Files identical despite different names*

### Comparing `fabric-message-bus-1.6.0b2/fabric_mb/message_bus/messages/query_avro.py` & `fabric-message-bus-1.6.0b3/fabric_mb/message_bus/messages/query_avro.py`

 * *Files identical despite different names*

### Comparing `fabric-message-bus-1.6.0b2/fabric_mb/message_bus/messages/query_result_avro.py` & `fabric-message-bus-1.6.0b3/fabric_mb/message_bus/messages/query_result_avro.py`

 * *Files identical despite different names*

### Comparing `fabric-message-bus-1.6.0b2/fabric_mb/message_bus/messages/reclaim_delegation_avro.py` & `fabric-message-bus-1.6.0b3/fabric_mb/message_bus/messages/reclaim_delegation_avro.py`

 * *Files identical despite different names*

### Comparing `fabric-message-bus-1.6.0b2/fabric_mb/message_bus/messages/reclaim_resources_avro.py` & `fabric-message-bus-1.6.0b3/fabric_mb/message_bus/messages/reclaim_resources_avro.py`

 * *Files identical despite different names*

### Comparing `fabric-message-bus-1.6.0b2/fabric_mb/message_bus/messages/redeem_avro.py` & `fabric-message-bus-1.6.0b3/fabric_mb/message_bus/messages/redeem_avro.py`

 * *Files identical despite different names*

### Comparing `fabric-message-bus-1.6.0b2/fabric_mb/message_bus/messages/relinquish_avro.py` & `fabric-message-bus-1.6.0b3/fabric_mb/message_bus/messages/relinquish_avro.py`

 * *Files identical despite different names*

### Comparing `fabric-message-bus-1.6.0b2/fabric_mb/message_bus/messages/remove_delegation_avro.py` & `fabric-message-bus-1.6.0b3/fabric_mb/message_bus/messages/remove_delegation_avro.py`

 * *Files identical despite different names*

### Comparing `fabric-message-bus-1.6.0b2/fabric_mb/message_bus/messages/remove_reservation_avro.py` & `fabric-message-bus-1.6.0b3/fabric_mb/message_bus/messages/remove_reservation_avro.py`

 * *Files identical despite different names*

### Comparing `fabric-message-bus-1.6.0b2/fabric_mb/message_bus/messages/remove_slice_avro.py` & `fabric-message-bus-1.6.0b3/fabric_mb/message_bus/messages/remove_slice_avro.py`

 * *Files identical despite different names*

### Comparing `fabric-message-bus-1.6.0b2/fabric_mb/message_bus/messages/request_by_id_record.py` & `fabric-message-bus-1.6.0b3/fabric_mb/message_bus/messages/request_by_id_record.py`

 * *Files identical despite different names*

### Comparing `fabric-message-bus-1.6.0b2/fabric_mb/message_bus/messages/reservation_avro.py` & `fabric-message-bus-1.6.0b3/fabric_mb/message_bus/messages/reservation_avro.py`

 * *Files identical despite different names*

### Comparing `fabric-message-bus-1.6.0b2/fabric_mb/message_bus/messages/reservation_mng.py` & `fabric-message-bus-1.6.0b3/fabric_mb/message_bus/messages/reservation_mng.py`

 * *Files identical despite different names*

### Comparing `fabric-message-bus-1.6.0b2/fabric_mb/message_bus/messages/reservation_or_delegation_record.py` & `fabric-message-bus-1.6.0b3/fabric_mb/message_bus/messages/reservation_or_delegation_record.py`

 * *Files identical despite different names*

### Comparing `fabric-message-bus-1.6.0b2/fabric_mb/message_bus/messages/reservation_predecessor_avro.py` & `fabric-message-bus-1.6.0b3/fabric_mb/message_bus/messages/reservation_predecessor_avro.py`

 * *Files identical despite different names*

### Comparing `fabric-message-bus-1.6.0b2/fabric_mb/message_bus/messages/reservation_state_avro.py` & `fabric-message-bus-1.6.0b3/fabric_mb/message_bus/messages/reservation_state_avro.py`

 * *Files identical despite different names*

### Comparing `fabric-message-bus-1.6.0b2/fabric_mb/message_bus/messages/resource_set_avro.py` & `fabric-message-bus-1.6.0b3/fabric_mb/message_bus/messages/resource_set_avro.py`

 * *Files identical despite different names*

### Comparing `fabric-message-bus-1.6.0b2/fabric_mb/message_bus/messages/resource_ticket_avro.py` & `fabric-message-bus-1.6.0b3/fabric_mb/message_bus/messages/resource_ticket_avro.py`

 * *Files identical despite different names*

### Comparing `fabric-message-bus-1.6.0b2/fabric_mb/message_bus/messages/result_actor_avro.py` & `fabric-message-bus-1.6.0b3/fabric_mb/message_bus/messages/result_actor_avro.py`

 * *Files identical despite different names*

### Comparing `fabric-message-bus-1.6.0b2/fabric_mb/message_bus/messages/result_avro.py` & `fabric-message-bus-1.6.0b3/fabric_mb/message_bus/messages/result_avro.py`

 * *Files identical despite different names*

### Comparing `fabric-message-bus-1.6.0b2/fabric_mb/message_bus/messages/result_broker_query_model_avro.py` & `fabric-message-bus-1.6.0b3/fabric_mb/message_bus/messages/result_broker_query_model_avro.py`

 * *Files identical despite different names*

### Comparing `fabric-message-bus-1.6.0b2/fabric_mb/message_bus/messages/result_delegation_avro.py` & `fabric-message-bus-1.6.0b3/fabric_mb/message_bus/messages/result_delegation_avro.py`

 * *Files identical despite different names*

### Comparing `fabric-message-bus-1.6.0b2/fabric_mb/message_bus/messages/result_poa_avro.py` & `fabric-message-bus-1.6.0b3/fabric_mb/message_bus/messages/result_poa_avro.py`

 * *Files identical despite different names*

### Comparing `fabric-message-bus-1.6.0b2/fabric_mb/message_bus/messages/result_proxy_avro.py` & `fabric-message-bus-1.6.0b3/fabric_mb/message_bus/messages/result_proxy_avro.py`

 * *Files identical despite different names*

### Comparing `fabric-message-bus-1.6.0b2/fabric_mb/message_bus/messages/result_record_list.py` & `fabric-message-bus-1.6.0b3/fabric_mb/message_bus/messages/result_record_list.py`

 * *Files identical despite different names*

### Comparing `fabric-message-bus-1.6.0b2/fabric_mb/message_bus/messages/result_reservation_avro.py` & `fabric-message-bus-1.6.0b3/fabric_mb/message_bus/messages/result_reservation_avro.py`

 * *Files identical despite different names*

### Comparing `fabric-message-bus-1.6.0b2/fabric_mb/message_bus/messages/result_reservation_state_avro.py` & `fabric-message-bus-1.6.0b3/fabric_mb/message_bus/messages/result_reservation_state_avro.py`

 * *Files identical despite different names*

### Comparing `fabric-message-bus-1.6.0b2/fabric_mb/message_bus/messages/result_sites_avro.py` & `fabric-message-bus-1.6.0b3/fabric_mb/message_bus/messages/result_sites_avro.py`

 * *Files identical despite different names*

### Comparing `fabric-message-bus-1.6.0b2/fabric_mb/message_bus/messages/result_slice_avro.py` & `fabric-message-bus-1.6.0b3/fabric_mb/message_bus/messages/result_slice_avro.py`

 * *Files identical despite different names*

### Comparing `fabric-message-bus-1.6.0b2/fabric_mb/message_bus/messages/result_string_avro.py` & `fabric-message-bus-1.6.0b3/fabric_mb/message_bus/messages/result_string_avro.py`

 * *Files identical despite different names*

### Comparing `fabric-message-bus-1.6.0b2/fabric_mb/message_bus/messages/result_strings_avro.py` & `fabric-message-bus-1.6.0b3/fabric_mb/message_bus/messages/result_strings_avro.py`

 * *Files identical despite different names*

### Comparing `fabric-message-bus-1.6.0b2/fabric_mb/message_bus/messages/result_units_avro.py` & `fabric-message-bus-1.6.0b3/fabric_mb/message_bus/messages/result_units_avro.py`

 * *Files identical despite different names*

### Comparing `fabric-message-bus-1.6.0b2/fabric_mb/message_bus/messages/site_avro.py` & `fabric-message-bus-1.6.0b3/fabric_mb/message_bus/messages/site_avro.py`

 * *Files identical despite different names*

### Comparing `fabric-message-bus-1.6.0b2/fabric_mb/message_bus/messages/slice_avro.py` & `fabric-message-bus-1.6.0b3/fabric_mb/message_bus/messages/slice_avro.py`

 * *Files identical despite different names*

### Comparing `fabric-message-bus-1.6.0b2/fabric_mb/message_bus/messages/term_avro.py` & `fabric-message-bus-1.6.0b3/fabric_mb/message_bus/messages/term_avro.py`

 * *Files identical despite different names*

### Comparing `fabric-message-bus-1.6.0b2/fabric_mb/message_bus/messages/ticket.py` & `fabric-message-bus-1.6.0b3/fabric_mb/message_bus/messages/ticket.py`

 * *Files identical despite different names*

### Comparing `fabric-message-bus-1.6.0b2/fabric_mb/message_bus/messages/ticket_avro.py` & `fabric-message-bus-1.6.0b3/fabric_mb/message_bus/messages/ticket_avro.py`

 * *Files identical despite different names*

### Comparing `fabric-message-bus-1.6.0b2/fabric_mb/message_bus/messages/ticket_reservation_avro.py` & `fabric-message-bus-1.6.0b3/fabric_mb/message_bus/messages/ticket_reservation_avro.py`

 * *Files identical despite different names*

### Comparing `fabric-message-bus-1.6.0b2/fabric_mb/message_bus/messages/unit_avro.py` & `fabric-message-bus-1.6.0b3/fabric_mb/message_bus/messages/unit_avro.py`

 * *Files identical despite different names*

### Comparing `fabric-message-bus-1.6.0b2/fabric_mb/message_bus/messages/update_data_avro.py` & `fabric-message-bus-1.6.0b3/fabric_mb/message_bus/messages/update_data_avro.py`

 * *Files identical despite different names*

### Comparing `fabric-message-bus-1.6.0b2/fabric_mb/message_bus/messages/update_delegation_avro.py` & `fabric-message-bus-1.6.0b3/fabric_mb/message_bus/messages/update_delegation_avro.py`

 * *Files identical despite different names*

### Comparing `fabric-message-bus-1.6.0b2/fabric_mb/message_bus/messages/update_lease_avro.py` & `fabric-message-bus-1.6.0b3/fabric_mb/message_bus/messages/update_lease_avro.py`

 * *Files identical despite different names*

### Comparing `fabric-message-bus-1.6.0b2/fabric_mb/message_bus/messages/update_reservation_avro.py` & `fabric-message-bus-1.6.0b3/fabric_mb/message_bus/messages/update_reservation_avro.py`

 * *Files identical despite different names*

### Comparing `fabric-message-bus-1.6.0b2/fabric_mb/message_bus/messages/update_slice_avro.py` & `fabric-message-bus-1.6.0b3/fabric_mb/message_bus/messages/update_slice_avro.py`

 * *Files identical despite different names*

### Comparing `fabric-message-bus-1.6.0b2/fabric_mb/message_bus/messages/update_ticket_avro.py` & `fabric-message-bus-1.6.0b3/fabric_mb/message_bus/messages/update_ticket_avro.py`

 * *Files identical despite different names*

### Comparing `fabric-message-bus-1.6.0b2/fabric_mb/message_bus/producer.py` & `fabric-message-bus-1.6.0b3/fabric_mb/message_bus/producer.py`

 * *Files identical despite different names*

### Comparing `fabric-message-bus-1.6.0b2/fabric_mb/message_bus/schema/message.avsc` & `fabric-message-bus-1.6.0b3/fabric_mb/message_bus/schema/message.avsc`

 * *Files identical despite different names*

### Comparing `fabric-message-bus-1.6.0b2/fabric_mb/message_bus/test/abqm.graphml` & `fabric-message-bus-1.6.0b3/fabric_mb/message_bus/test/abqm.graphml`

 * *Files identical despite different names*

### Comparing `fabric-message-bus-1.6.0b2/fabric_mb/message_bus/test/message_bus_test.py` & `fabric-message-bus-1.6.0b3/fabric_mb/message_bus/test/message_bus_test.py`

 * *Files identical despite different names*

### Comparing `fabric-message-bus-1.6.0b2/pyproject.toml` & `fabric-message-bus-1.6.0b3/pyproject.toml`

 * *Files identical despite different names*

### Comparing `fabric-message-bus-1.6.0b2/secrets/create-certs.sh` & `fabric-message-bus-1.6.0b3/secrets/create-certs.sh`

 * *Files identical despite different names*

### Comparing `fabric-message-bus-1.6.0b2/PKG-INFO` & `fabric-message-bus-1.6.0b3/PKG-INFO`

 * *Files 0% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: fabric-message-bus
-Version: 1.6.0b2
+Version: 1.6.0b3
 Summary: Fabric Message Bus Schema
 Keywords: Kafka,Fabric Message Bus Schema,Avro
 Author-email: Komal Thareja <kthare10@renci.org>
 Requires-Python: >=3.9
 Description-Content-Type: text/markdown
 Classifier: Programming Language :: Python :: 3
 Classifier: License :: OSI Approved :: MIT License
```

