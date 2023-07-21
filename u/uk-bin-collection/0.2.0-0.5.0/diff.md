# Comparing `tmp/uk_bin_collection-0.2.0.tar.gz` & `tmp/uk_bin_collection-0.5.0.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "uk_bin_collection-0.2.0.tar", max compression
+gzip compressed data, was "uk_bin_collection-0.5.0.tar", max compression
```

## Comparing `uk_bin_collection-0.2.0.tar` & `uk_bin_collection-0.5.0.tar`

### file list

```diff
@@ -1,257 +1,256 @@
--rw-r--r--   0        0        0     1071 2023-07-18 18:09:18.711971 uk_bin_collection-0.2.0/LICENSE
--rw-r--r--   0        0        0     7292 2023-07-18 18:09:18.711971 uk_bin_collection-0.2.0/README.md
--rw-r--r--   0        0        0     1227 2023-07-18 18:10:14.088746 uk_bin_collection-0.2.0/pyproject.toml
--rw-r--r--   0        0        0        0 2023-07-18 18:09:18.711971 uk_bin_collection-0.2.0/uk_bin_collection/README.rst
--rw-r--r--   0        0        0      999 2023-07-18 18:09:18.711971 uk_bin_collection-0.2.0/uk_bin_collection/tests/council_schemas/BCPCouncil.schema
--rw-r--r--   0        0        0     1291 2023-07-18 18:09:18.711971 uk_bin_collection-0.2.0/uk_bin_collection/tests/council_schemas/BasingstokeCouncil.schema
--rw-r--r--   0        0        0     1357 2023-07-18 18:09:18.711971 uk_bin_collection-0.2.0/uk_bin_collection/tests/council_schemas/BexleyCouncil.schema
--rw-r--r--   0        0        0      999 2023-07-18 18:09:18.711971 uk_bin_collection-0.2.0/uk_bin_collection/tests/council_schemas/BlackburnCouncil.schema
--rw-r--r--   0        0        0      999 2023-07-18 18:09:18.711971 uk_bin_collection-0.2.0/uk_bin_collection/tests/council_schemas/BoltonCouncil.schema
--rw-r--r--   0        0        0      999 2023-07-18 18:09:18.711971 uk_bin_collection-0.2.0/uk_bin_collection/tests/council_schemas/BristolCityCouncil.schema
--rw-r--r--   0        0        0      999 2023-07-18 18:09:18.711971 uk_bin_collection-0.2.0/uk_bin_collection/tests/council_schemas/BromleyBoroughCouncil.schema
--rw-r--r--   0        0        0     1002 2023-07-18 18:09:18.711971 uk_bin_collection-0.2.0/uk_bin_collection/tests/council_schemas/BroxtoweBoroughCouncil.schema
--rw-r--r--   0        0        0      999 2023-07-18 18:09:18.711971 uk_bin_collection-0.2.0/uk_bin_collection/tests/council_schemas/CardiffCouncil.schema
--rw-r--r--   0        0        0      999 2023-07-18 18:09:18.711971 uk_bin_collection-0.2.0/uk_bin_collection/tests/council_schemas/CastlepointDistrictCouncil.schema
--rw-r--r--   0        0        0      999 2023-07-18 18:09:18.711971 uk_bin_collection-0.2.0/uk_bin_collection/tests/council_schemas/CharnwoodBoroughCouncil.schema
--rw-r--r--   0        0        0     1275 2023-07-18 18:09:18.711971 uk_bin_collection-0.2.0/uk_bin_collection/tests/council_schemas/ChelmsfordCityCouncil.schema
--rw-r--r--   0        0        0     1279 2023-07-18 18:09:18.711971 uk_bin_collection-0.2.0/uk_bin_collection/tests/council_schemas/CheshireEastCouncil.schema
--rw-r--r--   0        0        0      998 2023-07-18 18:09:18.711971 uk_bin_collection-0.2.0/uk_bin_collection/tests/council_schemas/Chilterns.schema
--rw-r--r--   0        0        0      999 2023-07-18 18:09:18.711971 uk_bin_collection-0.2.0/uk_bin_collection/tests/council_schemas/CrawleyBoroughCouncil.schema
--rw-r--r--   0        0        0      999 2023-07-18 18:09:18.711971 uk_bin_collection-0.2.0/uk_bin_collection/tests/council_schemas/CroydonCouncil.schema
--rw-r--r--   0        0        0     1002 2023-07-18 18:09:18.711971 uk_bin_collection-0.2.0/uk_bin_collection/tests/council_schemas/DerbyshireDalesDistrictCouncil.schema
--rw-r--r--   0        0        0      999 2023-07-18 18:09:18.711971 uk_bin_collection-0.2.0/uk_bin_collection/tests/council_schemas/DoncasterCouncil.schema
--rw-r--r--   0        0        0      999 2023-07-18 18:09:18.711971 uk_bin_collection-0.2.0/uk_bin_collection/tests/council_schemas/DurhamCouncil.schema
--rw-r--r--   0        0        0     1229 2023-07-18 18:09:18.711971 uk_bin_collection-0.2.0/uk_bin_collection/tests/council_schemas/EastCambridgeshireCouncil.schema
--rw-r--r--   0        0        0     1276 2023-07-18 18:09:18.711971 uk_bin_collection-0.2.0/uk_bin_collection/tests/council_schemas/EastDevonDC.schema
--rw-r--r--   0        0        0     1190 2023-07-18 18:09:18.711971 uk_bin_collection-0.2.0/uk_bin_collection/tests/council_schemas/EastNorthamptonshireCouncil.schema
--rw-r--r--   0        0        0      999 2023-07-18 18:09:18.711971 uk_bin_collection-0.2.0/uk_bin_collection/tests/council_schemas/EastRidingCouncil.schema
--rw-r--r--   0        0        0     1306 2023-07-18 18:09:18.711971 uk_bin_collection-0.2.0/uk_bin_collection/tests/council_schemas/EastleighBoroughCouncil.schema
--rw-r--r--   0        0        0      999 2023-07-18 18:09:18.711971 uk_bin_collection-0.2.0/uk_bin_collection/tests/council_schemas/ErewashBoroughCouncil.schema
--rw-r--r--   0        0        0      999 2023-07-18 18:09:18.711971 uk_bin_collection-0.2.0/uk_bin_collection/tests/council_schemas/FenlandDistrictCouncil.schema
--rw-r--r--   0        0        0     1317 2023-07-18 18:09:18.711971 uk_bin_collection-0.2.0/uk_bin_collection/tests/council_schemas/GlasgowCityCouncil.schema
--rw-r--r--   0        0        0     1211 2023-07-18 18:09:18.711971 uk_bin_collection-0.2.0/uk_bin_collection/tests/council_schemas/HighPeakCouncil.schema
--rw-r--r--   0        0        0      999 2023-07-18 18:09:18.711971 uk_bin_collection-0.2.0/uk_bin_collection/tests/council_schemas/HuntingdonDistrictCouncil.schema
--rw-r--r--   0        0        0      998 2023-07-18 18:09:18.711971 uk_bin_collection-0.2.0/uk_bin_collection/tests/council_schemas/KingstonUponThamesCouncil.schema
--rw-r--r--   0        0        0     1209 2023-07-18 18:09:18.711971 uk_bin_collection-0.2.0/uk_bin_collection/tests/council_schemas/LeedsCityCouncil.schema
--rw-r--r--   0        0        0     1223 2023-07-18 18:09:18.711971 uk_bin_collection-0.2.0/uk_bin_collection/tests/council_schemas/LisburnCastlereaghCityCouncil.schema
--rw-r--r--   0        0        0      999 2023-07-18 18:09:18.711971 uk_bin_collection-0.2.0/uk_bin_collection/tests/council_schemas/LondonBoroughHounslow.schema
--rw-r--r--   0        0        0      999 2023-07-18 18:09:18.711971 uk_bin_collection-0.2.0/uk_bin_collection/tests/council_schemas/MaldonDistrictCouncil.schema
--rw-r--r--   0        0        0      999 2023-07-18 18:09:18.711971 uk_bin_collection-0.2.0/uk_bin_collection/tests/council_schemas/MalvernHillsDC.schema
--rw-r--r--   0        0        0      999 2023-07-18 18:09:18.711971 uk_bin_collection-0.2.0/uk_bin_collection/tests/council_schemas/ManchesterCityCouncil.schema
--rw-r--r--   0        0        0     1007 2023-07-18 18:09:18.711971 uk_bin_collection-0.2.0/uk_bin_collection/tests/council_schemas/MertonCouncil.schema
--rw-r--r--   0        0        0      999 2023-07-18 18:09:18.711971 uk_bin_collection-0.2.0/uk_bin_collection/tests/council_schemas/MidSussexDistrictCouncil.schema
--rw-r--r--   0        0        0      999 2023-07-18 18:09:18.711971 uk_bin_collection-0.2.0/uk_bin_collection/tests/council_schemas/MiltonKeynesCityCouncil.schema
--rw-r--r--   0        0        0     1244 2023-07-18 18:09:18.711971 uk_bin_collection-0.2.0/uk_bin_collection/tests/council_schemas/NewarkAndSherwoodDC.schema
--rw-r--r--   0        0        0      999 2023-07-18 18:09:18.711971 uk_bin_collection-0.2.0/uk_bin_collection/tests/council_schemas/NewcastleCityCouncil.schema
--rw-r--r--   0        0        0     1319 2023-07-18 18:09:18.711971 uk_bin_collection-0.2.0/uk_bin_collection/tests/council_schemas/NorthEastLincs.schema
--rw-r--r--   0        0        0      999 2023-07-18 18:09:18.711971 uk_bin_collection-0.2.0/uk_bin_collection/tests/council_schemas/NorthKestevenDistrictCouncil.schema
--rw-r--r--   0        0        0      999 2023-07-18 18:09:18.711971 uk_bin_collection-0.2.0/uk_bin_collection/tests/council_schemas/NorthLanarkshireCouncil.schema
--rw-r--r--   0        0        0     1398 2023-07-18 18:09:18.711971 uk_bin_collection-0.2.0/uk_bin_collection/tests/council_schemas/NorthLincolnshireCouncil.schema
--rw-r--r--   0        0        0     1002 2023-07-18 18:09:18.711971 uk_bin_collection-0.2.0/uk_bin_collection/tests/council_schemas/NorthNorfolkDistrictCouncil.schema
--rw-r--r--   0        0        0     1002 2023-07-18 18:09:18.711971 uk_bin_collection-0.2.0/uk_bin_collection/tests/council_schemas/NorthSomersetCouncil.schema
--rw-r--r--   0        0        0     1262 2023-07-18 18:09:18.711971 uk_bin_collection-0.2.0/uk_bin_collection/tests/council_schemas/NorthTynesideCouncil.schema
--rw-r--r--   0        0        0     1310 2023-07-18 18:09:18.711971 uk_bin_collection-0.2.0/uk_bin_collection/tests/council_schemas/NorthumberlandCouncil.schema
--rw-r--r--   0        0        0     1337 2023-07-18 18:09:18.711971 uk_bin_collection-0.2.0/uk_bin_collection/tests/council_schemas/PrestonCityCouncil.schema
--rw-r--r--   0        0        0      999 2023-07-18 18:09:18.711971 uk_bin_collection-0.2.0/uk_bin_collection/tests/council_schemas/RochdaleCouncil.schema
--rw-r--r--   0        0        0      999 2023-07-18 18:09:18.711971 uk_bin_collection-0.2.0/uk_bin_collection/tests/council_schemas/RushcliffeBoroughCouncil.schema
--rw-r--r--   0        0        0     1209 2023-07-18 18:09:18.711971 uk_bin_collection-0.2.0/uk_bin_collection/tests/council_schemas/RushmoorCouncil.schema
--rw-r--r--   0        0        0     1313 2023-07-18 18:09:18.711971 uk_bin_collection-0.2.0/uk_bin_collection/tests/council_schemas/SalfordCityCouncil.schema
--rw-r--r--   0        0        0      999 2023-07-18 18:09:18.711971 uk_bin_collection-0.2.0/uk_bin_collection/tests/council_schemas/SheffieldCityCouncil.schema
--rw-r--r--   0        0        0      999 2023-07-18 18:09:18.711971 uk_bin_collection-0.2.0/uk_bin_collection/tests/council_schemas/SomersetCouncil.schema
--rw-r--r--   0        0        0      999 2023-07-18 18:09:18.711971 uk_bin_collection-0.2.0/uk_bin_collection/tests/council_schemas/SouthAyrshireCouncil.schema
--rw-r--r--   0        0        0     1219 2023-07-18 18:09:18.711971 uk_bin_collection-0.2.0/uk_bin_collection/tests/council_schemas/SouthCambridgeshireCouncil.schema
--rw-r--r--   0        0        0      999 2023-07-18 18:09:18.711971 uk_bin_collection-0.2.0/uk_bin_collection/tests/council_schemas/SouthLanarkshireCouncil.schema
--rw-r--r--   0        0        0      999 2023-07-18 18:09:18.711971 uk_bin_collection-0.2.0/uk_bin_collection/tests/council_schemas/SouthNorfolkCouncil.schema
--rw-r--r--   0        0        0      999 2023-07-18 18:09:18.711971 uk_bin_collection-0.2.0/uk_bin_collection/tests/council_schemas/SouthOxfordshireCouncil.schema
--rw-r--r--   0        0        0     1236 2023-07-18 18:09:18.711971 uk_bin_collection-0.2.0/uk_bin_collection/tests/council_schemas/SouthTynesideCouncil.schema
--rw-r--r--   0        0        0      999 2023-07-18 18:09:18.711971 uk_bin_collection-0.2.0/uk_bin_collection/tests/council_schemas/StHelensBC.schema
--rw-r--r--   0        0        0      999 2023-07-18 18:09:18.711971 uk_bin_collection-0.2.0/uk_bin_collection/tests/council_schemas/StockportBoroughCouncil.schema
--rw-r--r--   0        0        0      999 2023-07-18 18:09:18.711971 uk_bin_collection-0.2.0/uk_bin_collection/tests/council_schemas/SwaleBoroughCouncil.schema
--rw-r--r--   0        0        0      999 2023-07-18 18:09:18.711971 uk_bin_collection-0.2.0/uk_bin_collection/tests/council_schemas/TamesideMBCouncil.schema
--rw-r--r--   0        0        0     1002 2023-07-18 18:09:18.711971 uk_bin_collection-0.2.0/uk_bin_collection/tests/council_schemas/TonbridgeAndMallingBC.schema
--rw-r--r--   0        0        0     1002 2023-07-18 18:09:18.711971 uk_bin_collection-0.2.0/uk_bin_collection/tests/council_schemas/TorbayCouncil.schema
--rw-r--r--   0        0        0      999 2023-07-18 18:09:18.711971 uk_bin_collection-0.2.0/uk_bin_collection/tests/council_schemas/TorridgeDistrictCouncil.schema
--rw-r--r--   0        0        0     1202 2023-07-18 18:09:18.711971 uk_bin_collection-0.2.0/uk_bin_collection/tests/council_schemas/ValeofGlamorganCouncil.schema
--rw-r--r--   0        0        0      999 2023-07-18 18:09:18.711971 uk_bin_collection-0.2.0/uk_bin_collection/tests/council_schemas/WakefieldCityCouncil.schema
--rw-r--r--   0        0        0      999 2023-07-18 18:09:18.711971 uk_bin_collection-0.2.0/uk_bin_collection/tests/council_schemas/WarwickDistrictCouncil.schema
--rw-r--r--   0        0        0     1283 2023-07-18 18:09:18.711971 uk_bin_collection-0.2.0/uk_bin_collection/tests/council_schemas/WaverleyBoroughCouncil.schema
--rw-r--r--   0        0        0      999 2023-07-18 18:09:18.711971 uk_bin_collection-0.2.0/uk_bin_collection/tests/council_schemas/WealdenDistrictCouncil.schema
--rw-r--r--   0        0        0      999 2023-07-18 18:09:18.711971 uk_bin_collection-0.2.0/uk_bin_collection/tests/council_schemas/WelhatCouncil.schema
--rw-r--r--   0        0        0      382 2023-07-18 18:09:18.711971 uk_bin_collection-0.2.0/uk_bin_collection/tests/council_schemas/WiganBoroughCouncil.schema
--rw-r--r--   0        0        0     1273 2023-07-18 18:09:18.711971 uk_bin_collection-0.2.0/uk_bin_collection/tests/council_schemas/WiltshireCouncil.schema
--rw-r--r--   0        0        0      999 2023-07-18 18:09:18.711971 uk_bin_collection-0.2.0/uk_bin_collection/tests/council_schemas/WindsorAndMaidenheadCouncil.schema
--rw-r--r--   0        0        0      999 2023-07-18 18:09:18.711971 uk_bin_collection-0.2.0/uk_bin_collection/tests/council_schemas/WokingBoroughCouncil.schema
--rw-r--r--   0        0        0      999 2023-07-18 18:09:18.711971 uk_bin_collection-0.2.0/uk_bin_collection/tests/council_schemas/YorkCouncil.schema
--rw-r--r--   0        0        0      127 2023-07-18 18:09:18.711971 uk_bin_collection-0.2.0/uk_bin_collection/tests/features/environment.py
--rw-r--r--   0        0        0     3281 2023-07-18 18:09:18.711971 uk_bin_collection-0.2.0/uk_bin_collection/tests/features/validate_council_outputs.feature
--rw-r--r--   0        0        0    24132 2023-07-18 18:09:18.711971 uk_bin_collection-0.2.0/uk_bin_collection/tests/input.json
--rw-r--r--   0        0        0      606 2023-07-18 18:09:18.711971 uk_bin_collection-0.2.0/uk_bin_collection/tests/outputs/BCPCouncil.json
--rw-r--r--   0        0        0     2284 2023-07-18 18:09:18.711971 uk_bin_collection-0.2.0/uk_bin_collection/tests/outputs/BasingstokeCouncil.json
--rw-r--r--   0        0        0     3473 2023-07-18 18:09:18.711971 uk_bin_collection-0.2.0/uk_bin_collection/tests/outputs/BexleyCouncil.json
--rw-r--r--   0        0        0      501 2023-07-18 18:09:18.711971 uk_bin_collection-0.2.0/uk_bin_collection/tests/outputs/BlackburnCouncil.json
--rw-r--r--   0        0        0     1192 2023-07-18 18:09:18.715971 uk_bin_collection-0.2.0/uk_bin_collection/tests/outputs/BoltonCouncil.json
--rw-r--r--   0        0        0      557 2023-07-18 18:09:18.715971 uk_bin_collection-0.2.0/uk_bin_collection/tests/outputs/BristolCityCouncil.json
--rw-r--r--   0        0        0      462 2023-07-18 18:09:18.715971 uk_bin_collection-0.2.0/uk_bin_collection/tests/outputs/BromleyBoroughCouncil.json
--rw-r--r--   0        0        0      315 2023-07-18 18:09:18.715971 uk_bin_collection-0.2.0/uk_bin_collection/tests/outputs/BroxtoweBoroughCouncil.json
--rw-r--r--   0        0        0     1156 2023-07-18 18:09:18.715971 uk_bin_collection-0.2.0/uk_bin_collection/tests/outputs/CardiffCouncil.json
--rw-r--r--   0        0        0      958 2023-07-18 18:09:18.715971 uk_bin_collection-0.2.0/uk_bin_collection/tests/outputs/CastlepointDistrictCouncil.json
--rw-r--r--   0        0        0      213 2023-07-18 18:09:18.715971 uk_bin_collection-0.2.0/uk_bin_collection/tests/outputs/CharnwoodBoroughCouncil.json
--rw-r--r--   0        0        0     1830 2023-07-18 18:09:18.715971 uk_bin_collection-0.2.0/uk_bin_collection/tests/outputs/ChelmsfordCityCouncil.json
--rw-r--r--   0        0        0     1187 2023-07-18 18:09:18.715971 uk_bin_collection-0.2.0/uk_bin_collection/tests/outputs/CheshireEastCouncil.json
--rw-r--r--   0        0        0      493 2023-07-18 18:09:18.715971 uk_bin_collection-0.2.0/uk_bin_collection/tests/outputs/Chilterns.json
--rw-r--r--   0        0        0      271 2023-07-18 18:09:18.715971 uk_bin_collection-0.2.0/uk_bin_collection/tests/outputs/CrawleyBoroughCouncil.json
--rw-r--r--   0        0        0      466 2023-07-18 18:09:18.715971 uk_bin_collection-0.2.0/uk_bin_collection/tests/outputs/CroydonCouncil.json
--rw-r--r--   0        0        0      562 2023-07-18 18:09:18.715971 uk_bin_collection-0.2.0/uk_bin_collection/tests/outputs/DerbyshireDalesDistrictCouncil.json
--rw-r--r--   0        0        0      775 2023-07-18 18:09:18.715971 uk_bin_collection-0.2.0/uk_bin_collection/tests/outputs/DoncasterCouncil.json
--rw-r--r--   0        0        0      214 2023-07-18 18:09:18.715971 uk_bin_collection-0.2.0/uk_bin_collection/tests/outputs/DurhamCouncil.json
--rw-r--r--   0        0        0     1606 2023-07-18 18:09:18.715971 uk_bin_collection-0.2.0/uk_bin_collection/tests/outputs/EastCambridgeshireCouncil.json
--rw-r--r--   0        0        0     2635 2023-07-18 18:09:18.715971 uk_bin_collection-0.2.0/uk_bin_collection/tests/outputs/EastDevonDC.json
--rw-r--r--   0        0        0      982 2023-07-18 18:09:18.715971 uk_bin_collection-0.2.0/uk_bin_collection/tests/outputs/EastNorthamptonshireCouncil.json
--rw-r--r--   0        0        0      312 2023-07-18 18:09:18.715971 uk_bin_collection-0.2.0/uk_bin_collection/tests/outputs/EastRidingCouncil.json
--rw-r--r--   0        0        0      547 2023-07-18 18:09:18.715971 uk_bin_collection-0.2.0/uk_bin_collection/tests/outputs/EastleighBoroughCouncil.json
--rw-r--r--   0        0        0      325 2023-07-18 18:09:18.715971 uk_bin_collection-0.2.0/uk_bin_collection/tests/outputs/ErewashBoroughCouncil.json
--rw-r--r--   0        0        0     1362 2023-07-18 18:09:18.715971 uk_bin_collection-0.2.0/uk_bin_collection/tests/outputs/FenlandDistrictCouncil.json
--rw-r--r--   0        0        0     4251 2023-07-18 18:09:18.715971 uk_bin_collection-0.2.0/uk_bin_collection/tests/outputs/GlasgowCityCouncil.json
--rw-r--r--   0        0        0     1726 2023-07-18 18:09:18.715971 uk_bin_collection-0.2.0/uk_bin_collection/tests/outputs/HighPeakCouncil.json
--rw-r--r--   0        0        0      335 2023-07-18 18:09:18.715971 uk_bin_collection-0.2.0/uk_bin_collection/tests/outputs/HuntingdonDistrictCouncil.json
--rw-r--r--   0        0        0      534 2023-07-18 18:09:18.715971 uk_bin_collection-0.2.0/uk_bin_collection/tests/outputs/KingstonUponThamesCouncil.json
--rw-r--r--   0        0        0     1789 2023-07-18 18:09:18.715971 uk_bin_collection-0.2.0/uk_bin_collection/tests/outputs/LeedsCityCouncil.json
--rw-r--r--   0        0        0      608 2023-07-18 18:09:18.715971 uk_bin_collection-0.2.0/uk_bin_collection/tests/outputs/LisburnCastlereaghCityCouncil.json
--rw-r--r--   0        0        0     1445 2023-07-18 18:09:18.715971 uk_bin_collection-0.2.0/uk_bin_collection/tests/outputs/LondonBoroughHounslow.json
--rw-r--r--   0        0        0      409 2023-07-18 18:09:18.715971 uk_bin_collection-0.2.0/uk_bin_collection/tests/outputs/MaldonDistrictCouncil.json
--rw-r--r--   0        0        0      227 2023-07-18 18:09:18.715971 uk_bin_collection-0.2.0/uk_bin_collection/tests/outputs/MalvernHillsDC.json
--rw-r--r--   0        0        0      416 2023-07-18 18:09:18.715971 uk_bin_collection-0.2.0/uk_bin_collection/tests/outputs/ManchesterCityCouncil.json
--rw-r--r--   0        0        0      665 2023-07-18 18:09:18.715971 uk_bin_collection-0.2.0/uk_bin_collection/tests/outputs/MertonCouncil.json
--rw-r--r--   0        0        0      148 2023-07-18 18:09:18.715971 uk_bin_collection-0.2.0/uk_bin_collection/tests/outputs/MidSussexDistrictCouncil.json
--rw-r--r--   0        0        0      862 2023-07-18 18:09:18.715971 uk_bin_collection-0.2.0/uk_bin_collection/tests/outputs/MiltonKeynesCityCouncil.json
--rw-r--r--   0        0        0     1278 2023-07-18 18:09:18.715971 uk_bin_collection-0.2.0/uk_bin_collection/tests/outputs/NewarkAndSherwoodDC.json
--rw-r--r--   0        0        0      221 2023-07-18 18:09:18.715971 uk_bin_collection-0.2.0/uk_bin_collection/tests/outputs/NewcastleCityCouncil.json
--rw-r--r--   0        0        0     4096 2023-07-18 18:09:18.715971 uk_bin_collection-0.2.0/uk_bin_collection/tests/outputs/NorthEastLincs.json
--rw-r--r--   0        0        0      446 2023-07-18 18:09:18.715971 uk_bin_collection-0.2.0/uk_bin_collection/tests/outputs/NorthKestevenDistrictCouncil.json
--rw-r--r--   0        0        0      902 2023-07-18 18:09:18.715971 uk_bin_collection-0.2.0/uk_bin_collection/tests/outputs/NorthLanarkshireCouncil.json
--rw-r--r--   0        0        0     3042 2023-07-18 18:09:18.715971 uk_bin_collection-0.2.0/uk_bin_collection/tests/outputs/NorthLincolnshireCouncil.json
--rw-r--r--   0        0        0      300 2023-07-18 18:09:18.715971 uk_bin_collection-0.2.0/uk_bin_collection/tests/outputs/NorthNorfolkDistrictCouncil.json
--rw-r--r--   0        0        0      590 2023-07-18 18:09:18.715971 uk_bin_collection-0.2.0/uk_bin_collection/tests/outputs/NorthSomersetCouncil.json
--rw-r--r--   0        0        0     4935 2023-07-18 18:09:18.715971 uk_bin_collection-0.2.0/uk_bin_collection/tests/outputs/NorthTynesideCouncil.json
--rw-r--r--   0        0        0     3956 2023-07-18 18:09:18.715971 uk_bin_collection-0.2.0/uk_bin_collection/tests/outputs/NorthumberlandCouncil.json
--rw-r--r--   0        0        0    15934 2023-07-18 18:09:18.715971 uk_bin_collection-0.2.0/uk_bin_collection/tests/outputs/PrestonCityCouncil.json
--rw-r--r--   0        0        0      903 2023-07-18 18:09:18.715971 uk_bin_collection-0.2.0/uk_bin_collection/tests/outputs/RochdaleCouncil.json
--rw-r--r--   0        0        0      306 2023-07-18 18:09:18.715971 uk_bin_collection-0.2.0/uk_bin_collection/tests/outputs/RushcliffeBoroughCouncil.json
--rw-r--r--   0        0        0     1602 2023-07-18 18:09:18.715971 uk_bin_collection-0.2.0/uk_bin_collection/tests/outputs/RushmoorCouncil.json
--rw-r--r--   0        0        0     2734 2023-07-18 18:09:18.715971 uk_bin_collection-0.2.0/uk_bin_collection/tests/outputs/SalfordCityCouncil.json
--rw-r--r--   0        0        0      892 2023-07-18 18:09:18.715971 uk_bin_collection-0.2.0/uk_bin_collection/tests/outputs/SheffieldCityCouncil.json
--rw-r--r--   0        0        0      307 2023-07-18 18:09:18.715971 uk_bin_collection-0.2.0/uk_bin_collection/tests/outputs/SomersetCouncil.json
--rw-r--r--   0        0        0     1871 2023-07-18 18:09:18.715971 uk_bin_collection-0.2.0/uk_bin_collection/tests/outputs/SouthAyrshireCouncil.json
--rw-r--r--   0        0        0     2214 2023-07-18 18:09:18.715971 uk_bin_collection-0.2.0/uk_bin_collection/tests/outputs/SouthCambridgeshireCouncil.json
--rw-r--r--   0        0        0      258 2023-07-18 18:09:18.715971 uk_bin_collection-0.2.0/uk_bin_collection/tests/outputs/SouthLanarkshireCouncil.json
--rw-r--r--   0        0        0      217 2023-07-18 18:09:18.715971 uk_bin_collection-0.2.0/uk_bin_collection/tests/outputs/SouthNorfolkCouncil.json
--rw-r--r--   0        0        0      293 2023-07-18 18:09:18.715971 uk_bin_collection-0.2.0/uk_bin_collection/tests/outputs/SouthOxfordshireCouncil.json
--rw-r--r--   0        0        0     3283 2023-07-18 18:09:18.715971 uk_bin_collection-0.2.0/uk_bin_collection/tests/outputs/SouthTynesideCouncil.json
--rw-r--r--   0        0        0      358 2023-07-18 18:09:18.715971 uk_bin_collection-0.2.0/uk_bin_collection/tests/outputs/StHelensBC.json
--rw-r--r--   0        0        0      409 2023-07-18 18:09:18.715971 uk_bin_collection-0.2.0/uk_bin_collection/tests/outputs/StockportBoroughCouncil.json
--rw-r--r--   0        0        0      922 2023-07-18 18:09:18.715971 uk_bin_collection-0.2.0/uk_bin_collection/tests/outputs/SwaleBoroughCouncil.json
--rw-r--r--   0        0        0     1765 2023-07-18 18:09:18.715971 uk_bin_collection-0.2.0/uk_bin_collection/tests/outputs/TamesideMBCouncil.json
--rw-r--r--   0        0        0     1037 2023-07-18 18:09:18.715971 uk_bin_collection-0.2.0/uk_bin_collection/tests/outputs/TonbridgeAndMallingBC.json
--rw-r--r--   0        0        0     1406 2023-07-18 18:09:18.715971 uk_bin_collection-0.2.0/uk_bin_collection/tests/outputs/TorbayCouncil.json
--rw-r--r--   0        0        0      116 2023-07-18 18:09:18.715971 uk_bin_collection-0.2.0/uk_bin_collection/tests/outputs/TorridgeDistrictCouncil.json
--rw-r--r--   0        0        0     5934 2023-07-18 18:09:18.715971 uk_bin_collection-0.2.0/uk_bin_collection/tests/outputs/ValeofGlamorganCouncil.json
--rw-r--r--   0        0        0      225 2023-07-18 18:09:18.715971 uk_bin_collection-0.2.0/uk_bin_collection/tests/outputs/WakefieldCityCouncil.json
--rw-r--r--   0        0        0      318 2023-07-18 18:09:18.715971 uk_bin_collection-0.2.0/uk_bin_collection/tests/outputs/WarwickDistrictCouncil.json
--rw-r--r--   0        0        0      964 2023-07-18 18:09:18.715971 uk_bin_collection-0.2.0/uk_bin_collection/tests/outputs/WaverleyBoroughCouncil.json
--rw-r--r--   0        0        0      222 2023-07-18 18:09:18.715971 uk_bin_collection-0.2.0/uk_bin_collection/tests/outputs/WealdenDistrictCouncil.json
--rw-r--r--   0        0        0      495 2023-07-18 18:09:18.715971 uk_bin_collection-0.2.0/uk_bin_collection/tests/outputs/WelhatCouncil.json
--rw-r--r--   0        0        0      161 2023-07-18 18:09:18.715971 uk_bin_collection-0.2.0/uk_bin_collection/tests/outputs/WiganBoroughCouncil.json
--rw-r--r--   0        0        0     1737 2023-07-18 18:09:18.715971 uk_bin_collection-0.2.0/uk_bin_collection/tests/outputs/WiltshireCouncil.json
--rw-r--r--   0        0        0      367 2023-07-18 18:09:18.715971 uk_bin_collection-0.2.0/uk_bin_collection/tests/outputs/WindsorAndMaidenheadCouncil.json
--rw-r--r--   0        0        0     1482 2023-07-18 18:09:18.715971 uk_bin_collection-0.2.0/uk_bin_collection/tests/outputs/WokingBoroughCouncil.json
--rw-r--r--   0        0        0      307 2023-07-18 18:09:18.715971 uk_bin_collection-0.2.0/uk_bin_collection/tests/outputs/YorkCouncil.json
--rw-r--r--   0        0        0     1147 2023-07-18 18:09:18.715971 uk_bin_collection-0.2.0/uk_bin_collection/tests/step_defs/step_helpers/file_handler.py
--rw-r--r--   0        0        0     2546 2023-07-18 18:09:18.715971 uk_bin_collection-0.2.0/uk_bin_collection/tests/step_defs/test_validate_council.py
--rw-r--r--   0        0        0     2576 2023-07-18 18:09:18.715971 uk_bin_collection-0.2.0/uk_bin_collection/tests/test_collect_data.py
--rw-r--r--   0        0        0     3977 2023-07-18 18:09:18.715971 uk_bin_collection-0.2.0/uk_bin_collection/tests/test_common_functions.py
--rw-r--r--   0        0        0     2881 2023-07-18 18:09:18.715971 uk_bin_collection-0.2.0/uk_bin_collection/uk_bin_collection/collect_data.py
--rw-r--r--   0        0        0     6643 2023-07-18 18:09:18.715971 uk_bin_collection-0.2.0/uk_bin_collection/uk_bin_collection/common.py
--rw-r--r--   0        0        0     1579 2023-07-18 18:09:18.715971 uk_bin_collection-0.2.0/uk_bin_collection/uk_bin_collection/councils/BCPCouncil.py
--rw-r--r--   0        0        0     1936 2023-07-18 18:09:18.715971 uk_bin_collection-0.2.0/uk_bin_collection/uk_bin_collection/councils/BasingstokeCouncil.py
--rw-r--r--   0        0        0     2237 2023-07-18 18:09:18.715971 uk_bin_collection-0.2.0/uk_bin_collection/uk_bin_collection/councils/BexleyCouncil.py
--rw-r--r--   0        0        0     3156 2023-07-18 18:09:18.715971 uk_bin_collection-0.2.0/uk_bin_collection/uk_bin_collection/councils/BlackburnCouncil.py
--rw-r--r--   0        0        0     3028 2023-07-18 18:09:18.715971 uk_bin_collection-0.2.0/uk_bin_collection/uk_bin_collection/councils/BoltonCouncil.py
--rw-r--r--   0        0        0     5581 2023-07-18 18:09:18.715971 uk_bin_collection-0.2.0/uk_bin_collection/uk_bin_collection/councils/BristolCityCouncil.py
--rw-r--r--   0        0        0     1676 2023-07-18 18:09:18.715971 uk_bin_collection-0.2.0/uk_bin_collection/uk_bin_collection/councils/BromleyBoroughCouncil.py
--rw-r--r--   0        0        0     3733 2023-07-18 18:09:18.715971 uk_bin_collection-0.2.0/uk_bin_collection/uk_bin_collection/councils/BroxtoweBoroughCouncil.py
--rw-r--r--   0        0        0     7214 2023-07-18 18:09:18.715971 uk_bin_collection-0.2.0/uk_bin_collection/uk_bin_collection/councils/CardiffCouncil.py
--rw-r--r--   0        0        0     3946 2023-07-18 18:09:18.715971 uk_bin_collection-0.2.0/uk_bin_collection/uk_bin_collection/councils/CastlepointDistrictCouncil.py
--rw-r--r--   0        0        0     1339 2023-07-18 18:09:18.715971 uk_bin_collection-0.2.0/uk_bin_collection/uk_bin_collection/councils/CharnwoodBoroughCouncil.py
--rw-r--r--   0        0        0     2170 2023-07-18 18:09:18.715971 uk_bin_collection-0.2.0/uk_bin_collection/uk_bin_collection/councils/ChelmsfordCityCouncil.py
--rw-r--r--   0        0        0     1541 2023-07-18 18:09:18.715971 uk_bin_collection-0.2.0/uk_bin_collection/uk_bin_collection/councils/CheshireEastCouncil.py
--rw-r--r--   0        0        0     2938 2023-07-18 18:09:18.715971 uk_bin_collection-0.2.0/uk_bin_collection/uk_bin_collection/councils/Chilterns.py
--rw-r--r--   0        0        0     1983 2023-07-18 18:09:18.715971 uk_bin_collection-0.2.0/uk_bin_collection/uk_bin_collection/councils/CrawleyBoroughCouncil.py
--rw-r--r--   0        0        0    11599 2023-07-18 18:09:18.715971 uk_bin_collection-0.2.0/uk_bin_collection/uk_bin_collection/councils/CroydonCouncil.py
--rw-r--r--   0        0        0     3499 2023-07-18 18:09:18.715971 uk_bin_collection-0.2.0/uk_bin_collection/uk_bin_collection/councils/DerbyshireDalesDistrictCouncil.py
--rw-r--r--   0        0        0     3124 2023-07-18 18:09:18.715971 uk_bin_collection-0.2.0/uk_bin_collection/uk_bin_collection/councils/DoncasterCouncil.py
--rw-r--r--   0        0        0     1626 2023-07-18 18:09:18.715971 uk_bin_collection-0.2.0/uk_bin_collection/uk_bin_collection/councils/DurhamCouncil.py
--rw-r--r--   0        0        0     1506 2023-07-18 18:09:18.715971 uk_bin_collection-0.2.0/uk_bin_collection/uk_bin_collection/councils/EastCambridgeshireCouncil.py
--rw-r--r--   0        0        0     3267 2023-07-18 18:09:18.715971 uk_bin_collection-0.2.0/uk_bin_collection/uk_bin_collection/councils/EastDevonDC.py
--rw-r--r--   0        0        0     3756 2023-07-18 18:09:18.715971 uk_bin_collection-0.2.0/uk_bin_collection/uk_bin_collection/councils/EastNorthamptonshireCouncil.py
--rw-r--r--   0        0        0     2170 2023-07-18 18:09:18.715971 uk_bin_collection-0.2.0/uk_bin_collection/uk_bin_collection/councils/EastRidingCouncil.py
--rw-r--r--   0        0        0     2203 2023-07-18 18:09:18.715971 uk_bin_collection-0.2.0/uk_bin_collection/uk_bin_collection/councils/EastleighBoroughCouncil.py
--rw-r--r--   0        0        0     2507 2023-07-18 18:09:18.715971 uk_bin_collection-0.2.0/uk_bin_collection/uk_bin_collection/councils/ErewashBoroughCouncil.py
--rw-r--r--   0        0        0     2519 2023-07-18 18:09:18.715971 uk_bin_collection-0.2.0/uk_bin_collection/uk_bin_collection/councils/FenlandDistrictCouncil.py
--rw-r--r--   0        0        0     2534 2023-07-18 18:09:18.715971 uk_bin_collection-0.2.0/uk_bin_collection/uk_bin_collection/councils/GlasgowCityCouncil.py
--rw-r--r--   0        0        0     4416 2023-07-18 18:09:18.715971 uk_bin_collection-0.2.0/uk_bin_collection/uk_bin_collection/councils/HighPeakCouncil.py
--rw-r--r--   0        0        0     1114 2023-07-18 18:09:18.715971 uk_bin_collection-0.2.0/uk_bin_collection/uk_bin_collection/councils/HuntingdonDistrictCouncil.py
--rw-r--r--   0        0        0     1735 2023-07-18 18:09:18.715971 uk_bin_collection-0.2.0/uk_bin_collection/uk_bin_collection/councils/KingstonUponThamesCouncil.py
--rw-r--r--   0        0        0     3712 2023-07-18 18:09:18.715971 uk_bin_collection-0.2.0/uk_bin_collection/uk_bin_collection/councils/LeedsCityCouncil.py
--rw-r--r--   0        0        0     3313 2023-07-18 18:09:18.715971 uk_bin_collection-0.2.0/uk_bin_collection/uk_bin_collection/councils/LisburnCastlereaghCityCouncil.py
--rw-r--r--   0        0        0     2081 2023-07-18 18:09:18.715971 uk_bin_collection-0.2.0/uk_bin_collection/uk_bin_collection/councils/LondonBoroughHounslow.py
--rw-r--r--   0        0        0     2003 2023-07-18 18:09:18.715971 uk_bin_collection-0.2.0/uk_bin_collection/uk_bin_collection/councils/MaldonDistrictCouncil.py
--rw-r--r--   0        0        0     2092 2023-07-18 18:09:18.715971 uk_bin_collection-0.2.0/uk_bin_collection/uk_bin_collection/councils/MalvernHillsDC.py
--rw-r--r--   0        0        0     4949 2023-07-18 18:09:18.715971 uk_bin_collection-0.2.0/uk_bin_collection/uk_bin_collection/councils/ManchesterCityCouncil.py
--rw-r--r--   0        0        0     1895 2023-07-18 18:09:18.715971 uk_bin_collection-0.2.0/uk_bin_collection/uk_bin_collection/councils/MertonCouncil.py
--rw-r--r--   0        0        0     2711 2023-07-18 18:09:18.715971 uk_bin_collection-0.2.0/uk_bin_collection/uk_bin_collection/councils/MidSussexDistrictCouncil.py
--rw-r--r--   0        0        0     2011 2023-07-18 18:09:18.719971 uk_bin_collection-0.2.0/uk_bin_collection/uk_bin_collection/councils/MiltonKeynesCityCouncil.py
--rw-r--r--   0        0        0     2146 2023-07-18 18:09:18.719971 uk_bin_collection-0.2.0/uk_bin_collection/uk_bin_collection/councils/NewarkAndSherwoodDC.py
--rw-r--r--   0        0        0     1997 2023-07-18 18:09:18.719971 uk_bin_collection-0.2.0/uk_bin_collection/uk_bin_collection/councils/NewcastleCityCouncil.py
--rw-r--r--   0        0        0     1831 2023-07-18 18:09:18.719971 uk_bin_collection-0.2.0/uk_bin_collection/uk_bin_collection/councils/NorthEastLincs.py
--rw-r--r--   0        0        0     1522 2023-07-18 18:09:18.719971 uk_bin_collection-0.2.0/uk_bin_collection/uk_bin_collection/councils/NorthKestevenDistrictCouncil.py
--rw-r--r--   0        0        0     1675 2023-07-18 18:09:18.719971 uk_bin_collection-0.2.0/uk_bin_collection/uk_bin_collection/councils/NorthLanarkshireCouncil.py
--rw-r--r--   0        0        0     2407 2023-07-18 18:09:18.719971 uk_bin_collection-0.2.0/uk_bin_collection/uk_bin_collection/councils/NorthLincolnshireCouncil.py
--rw-r--r--   0        0        0     3723 2023-07-18 18:09:18.719971 uk_bin_collection-0.2.0/uk_bin_collection/uk_bin_collection/councils/NorthNorfolkDistrictCouncil.py
--rw-r--r--   0        0        0     2679 2023-07-18 18:09:18.719971 uk_bin_collection-0.2.0/uk_bin_collection/uk_bin_collection/councils/NorthSomersetCouncil.py
--rw-r--r--   0        0        0    10889 2023-07-18 18:09:18.719971 uk_bin_collection-0.2.0/uk_bin_collection/uk_bin_collection/councils/NorthTynesideCouncil.py
--rw-r--r--   0        0        0     4695 2023-07-18 18:09:18.719971 uk_bin_collection-0.2.0/uk_bin_collection/uk_bin_collection/councils/NorthumberlandCouncil.py
--rw-r--r--   0        0        0     3900 2023-07-18 18:09:18.719971 uk_bin_collection-0.2.0/uk_bin_collection/uk_bin_collection/councils/PrestonCityCouncil.py
--rw-r--r--   0        0        0     2347 2023-07-18 18:09:18.719971 uk_bin_collection-0.2.0/uk_bin_collection/uk_bin_collection/councils/RochdaleCouncil.py
--rw-r--r--   0        0        0     3514 2023-07-18 18:09:18.719971 uk_bin_collection-0.2.0/uk_bin_collection/uk_bin_collection/councils/RushcliffeBoroughCouncil.py
--rw-r--r--   0        0        0     2043 2023-07-18 18:09:18.719971 uk_bin_collection-0.2.0/uk_bin_collection/uk_bin_collection/councils/RushmoorCouncil.py
--rw-r--r--   0        0        0     2512 2023-07-18 18:09:18.719971 uk_bin_collection-0.2.0/uk_bin_collection/uk_bin_collection/councils/SalfordCityCouncil.py
--rw-r--r--   0        0        0     1997 2023-07-18 18:09:18.719971 uk_bin_collection-0.2.0/uk_bin_collection/uk_bin_collection/councils/SheffieldCityCouncil.py
--rw-r--r--   0        0        0     8499 2023-07-18 18:09:18.719971 uk_bin_collection-0.2.0/uk_bin_collection/uk_bin_collection/councils/SomersetCouncil.py
--rw-r--r--   0        0        0     2728 2023-07-18 18:09:18.719971 uk_bin_collection-0.2.0/uk_bin_collection/uk_bin_collection/councils/SouthAyrshireCouncil.py
--rw-r--r--   0        0        0     2313 2023-07-18 18:09:18.719971 uk_bin_collection-0.2.0/uk_bin_collection/uk_bin_collection/councils/SouthCambridgeshireCouncil.py
--rw-r--r--   0        0        0     3132 2023-07-18 18:09:18.719971 uk_bin_collection-0.2.0/uk_bin_collection/uk_bin_collection/councils/SouthLanarkshireCouncil.py
--rw-r--r--   0        0        0     3966 2023-07-18 18:09:18.719971 uk_bin_collection-0.2.0/uk_bin_collection/uk_bin_collection/councils/SouthNorfolkCouncil.py
--rw-r--r--   0        0        0     3208 2023-07-18 18:09:18.719971 uk_bin_collection-0.2.0/uk_bin_collection/uk_bin_collection/councils/SouthOxfordshireCouncil.py
--rw-r--r--   0        0        0     3432 2023-07-18 18:09:18.719971 uk_bin_collection-0.2.0/uk_bin_collection/uk_bin_collection/councils/SouthTynesideCouncil.py
--rw-r--r--   0        0        0     1960 2023-07-18 18:09:18.719971 uk_bin_collection-0.2.0/uk_bin_collection/uk_bin_collection/councils/StHelensBC.py
--rw-r--r--   0        0        0     1404 2023-07-18 18:09:18.719971 uk_bin_collection-0.2.0/uk_bin_collection/uk_bin_collection/councils/StockportBoroughCouncil.py
--rw-r--r--   0        0        0     2040 2023-07-18 18:09:18.719971 uk_bin_collection-0.2.0/uk_bin_collection/uk_bin_collection/councils/SwaleBoroughCouncil.py
--rw-r--r--   0        0        0     2001 2023-07-18 18:09:18.719971 uk_bin_collection-0.2.0/uk_bin_collection/uk_bin_collection/councils/TamesideMBCouncil.py
--rw-r--r--   0        0        0     4865 2023-07-18 18:09:18.719971 uk_bin_collection-0.2.0/uk_bin_collection/uk_bin_collection/councils/TonbridgeAndMallingBC.py
--rw-r--r--   0        0        0     2035 2023-07-18 18:09:18.719971 uk_bin_collection-0.2.0/uk_bin_collection/uk_bin_collection/councils/TorbayCouncil.py
--rw-r--r--   0        0        0     6074 2023-07-18 18:09:18.719971 uk_bin_collection-0.2.0/uk_bin_collection/uk_bin_collection/councils/TorridgeDistrictCouncil.py
--rw-r--r--   0        0        0     4863 2023-07-18 18:09:18.719971 uk_bin_collection-0.2.0/uk_bin_collection/uk_bin_collection/councils/ValeofGlamorganCouncil.py
--rw-r--r--   0        0        0     3916 2023-07-18 18:09:18.719971 uk_bin_collection-0.2.0/uk_bin_collection/uk_bin_collection/councils/WakefieldCityCouncil.py
--rw-r--r--   0        0        0     1153 2023-07-18 18:09:18.719971 uk_bin_collection-0.2.0/uk_bin_collection/uk_bin_collection/councils/WarwickDistrictCouncil.py
--rw-r--r--   0        0        0     4667 2023-07-18 18:09:18.719971 uk_bin_collection-0.2.0/uk_bin_collection/uk_bin_collection/councils/WaverleyBoroughCouncil.py
--rw-r--r--   0        0        0     3374 2023-07-18 18:09:18.719971 uk_bin_collection-0.2.0/uk_bin_collection/uk_bin_collection/councils/WealdenDistrictCouncil.py
--rw-r--r--   0        0        0     2284 2023-07-18 18:09:18.719971 uk_bin_collection-0.2.0/uk_bin_collection/uk_bin_collection/councils/WelhatCouncil.py
--rw-r--r--   0        0        0     3612 2023-07-18 18:09:18.719971 uk_bin_collection-0.2.0/uk_bin_collection/uk_bin_collection/councils/WiganBoroughCouncil.py
--rw-r--r--   0        0        0     5207 2023-07-18 18:09:18.719971 uk_bin_collection-0.2.0/uk_bin_collection/uk_bin_collection/councils/WiltshireCouncil.py
--rw-r--r--   0        0        0     5536 2023-07-18 18:09:18.719971 uk_bin_collection-0.2.0/uk_bin_collection/uk_bin_collection/councils/WindsorAndMaidenheadCouncil.py
--rw-r--r--   0        0        0     5027 2023-07-18 18:09:18.719971 uk_bin_collection-0.2.0/uk_bin_collection/uk_bin_collection/councils/WokingBoroughCouncil.py
--rw-r--r--   0        0        0     1496 2023-07-18 18:09:18.719971 uk_bin_collection-0.2.0/uk_bin_collection/uk_bin_collection/councils/YorkCouncil.py
--rw-r--r--   0        0        0     1121 2023-07-18 18:09:18.719971 uk_bin_collection-0.2.0/uk_bin_collection/uk_bin_collection/councils/council_class_template/councilclasstemplate.py
--rw-r--r--   0        0        0     4574 2023-07-18 18:09:18.719971 uk_bin_collection-0.2.0/uk_bin_collection/uk_bin_collection/get_bin_data.py
--rw-r--r--   0        0        0     8628 1970-01-01 00:00:00.000000 uk_bin_collection-0.2.0/setup.py
--rw-r--r--   0        0        0     7916 1970-01-01 00:00:00.000000 uk_bin_collection-0.2.0/PKG-INFO
+-rw-r--r--   0        0        0     1071 2023-07-21 16:31:26.451286 uk_bin_collection-0.5.0/LICENSE
+-rw-r--r--   0        0        0     7296 2023-07-21 16:31:26.451286 uk_bin_collection-0.5.0/README.md
+-rw-r--r--   0        0        0     1225 2023-07-21 16:32:02.203405 uk_bin_collection-0.5.0/pyproject.toml
+-rw-r--r--   0        0        0        0 2023-07-21 16:31:26.451286 uk_bin_collection-0.5.0/uk_bin_collection/README.rst
+-rw-r--r--   0        0        0      999 2023-07-21 16:31:26.451286 uk_bin_collection-0.5.0/uk_bin_collection/tests/council_schemas/BCPCouncil.schema
+-rw-r--r--   0        0        0     1291 2023-07-21 16:31:26.451286 uk_bin_collection-0.5.0/uk_bin_collection/tests/council_schemas/BasingstokeCouncil.schema
+-rw-r--r--   0        0        0     1357 2023-07-21 16:31:26.451286 uk_bin_collection-0.5.0/uk_bin_collection/tests/council_schemas/BexleyCouncil.schema
+-rw-r--r--   0        0        0      999 2023-07-21 16:31:26.451286 uk_bin_collection-0.5.0/uk_bin_collection/tests/council_schemas/BlackburnCouncil.schema
+-rw-r--r--   0        0        0      999 2023-07-21 16:31:26.451286 uk_bin_collection-0.5.0/uk_bin_collection/tests/council_schemas/BoltonCouncil.schema
+-rw-r--r--   0        0        0      999 2023-07-21 16:31:26.451286 uk_bin_collection-0.5.0/uk_bin_collection/tests/council_schemas/BristolCityCouncil.schema
+-rw-r--r--   0        0        0      999 2023-07-21 16:31:26.451286 uk_bin_collection-0.5.0/uk_bin_collection/tests/council_schemas/BromleyBoroughCouncil.schema
+-rw-r--r--   0        0        0     1002 2023-07-21 16:31:26.451286 uk_bin_collection-0.5.0/uk_bin_collection/tests/council_schemas/BroxtoweBoroughCouncil.schema
+-rw-r--r--   0        0        0      999 2023-07-21 16:31:26.455287 uk_bin_collection-0.5.0/uk_bin_collection/tests/council_schemas/CardiffCouncil.schema
+-rw-r--r--   0        0        0      999 2023-07-21 16:31:26.455287 uk_bin_collection-0.5.0/uk_bin_collection/tests/council_schemas/CastlepointDistrictCouncil.schema
+-rw-r--r--   0        0        0      999 2023-07-21 16:31:26.455287 uk_bin_collection-0.5.0/uk_bin_collection/tests/council_schemas/CharnwoodBoroughCouncil.schema
+-rw-r--r--   0        0        0     1275 2023-07-21 16:31:26.455287 uk_bin_collection-0.5.0/uk_bin_collection/tests/council_schemas/ChelmsfordCityCouncil.schema
+-rw-r--r--   0        0        0     1279 2023-07-21 16:31:26.455287 uk_bin_collection-0.5.0/uk_bin_collection/tests/council_schemas/CheshireEastCouncil.schema
+-rw-r--r--   0        0        0      998 2023-07-21 16:31:26.455287 uk_bin_collection-0.5.0/uk_bin_collection/tests/council_schemas/Chilterns.schema
+-rw-r--r--   0        0        0      999 2023-07-21 16:31:26.455287 uk_bin_collection-0.5.0/uk_bin_collection/tests/council_schemas/CrawleyBoroughCouncil.schema
+-rw-r--r--   0        0        0      999 2023-07-21 16:31:26.455287 uk_bin_collection-0.5.0/uk_bin_collection/tests/council_schemas/CroydonCouncil.schema
+-rw-r--r--   0        0        0     1002 2023-07-21 16:31:26.455287 uk_bin_collection-0.5.0/uk_bin_collection/tests/council_schemas/DerbyshireDalesDistrictCouncil.schema
+-rw-r--r--   0        0        0      999 2023-07-21 16:31:26.455287 uk_bin_collection-0.5.0/uk_bin_collection/tests/council_schemas/DoncasterCouncil.schema
+-rw-r--r--   0        0        0      999 2023-07-21 16:31:26.455287 uk_bin_collection-0.5.0/uk_bin_collection/tests/council_schemas/DurhamCouncil.schema
+-rw-r--r--   0        0        0     1229 2023-07-21 16:31:26.455287 uk_bin_collection-0.5.0/uk_bin_collection/tests/council_schemas/EastCambridgeshireCouncil.schema
+-rw-r--r--   0        0        0     1276 2023-07-21 16:31:26.455287 uk_bin_collection-0.5.0/uk_bin_collection/tests/council_schemas/EastDevonDC.schema
+-rw-r--r--   0        0        0     1190 2023-07-21 16:31:26.455287 uk_bin_collection-0.5.0/uk_bin_collection/tests/council_schemas/EastNorthamptonshireCouncil.schema
+-rw-r--r--   0        0        0      999 2023-07-21 16:31:26.455287 uk_bin_collection-0.5.0/uk_bin_collection/tests/council_schemas/EastRidingCouncil.schema
+-rw-r--r--   0        0        0     1306 2023-07-21 16:31:26.455287 uk_bin_collection-0.5.0/uk_bin_collection/tests/council_schemas/EastleighBoroughCouncil.schema
+-rw-r--r--   0        0        0      999 2023-07-21 16:31:26.455287 uk_bin_collection-0.5.0/uk_bin_collection/tests/council_schemas/ErewashBoroughCouncil.schema
+-rw-r--r--   0        0        0      999 2023-07-21 16:31:26.455287 uk_bin_collection-0.5.0/uk_bin_collection/tests/council_schemas/FenlandDistrictCouncil.schema
+-rw-r--r--   0        0        0     1317 2023-07-21 16:31:26.455287 uk_bin_collection-0.5.0/uk_bin_collection/tests/council_schemas/GlasgowCityCouncil.schema
+-rw-r--r--   0        0        0     1211 2023-07-21 16:31:26.455287 uk_bin_collection-0.5.0/uk_bin_collection/tests/council_schemas/HighPeakCouncil.schema
+-rw-r--r--   0        0        0      999 2023-07-21 16:31:26.455287 uk_bin_collection-0.5.0/uk_bin_collection/tests/council_schemas/HuntingdonDistrictCouncil.schema
+-rw-r--r--   0        0        0      998 2023-07-21 16:31:26.455287 uk_bin_collection-0.5.0/uk_bin_collection/tests/council_schemas/KingstonUponThamesCouncil.schema
+-rw-r--r--   0        0        0     1209 2023-07-21 16:31:26.455287 uk_bin_collection-0.5.0/uk_bin_collection/tests/council_schemas/LeedsCityCouncil.schema
+-rw-r--r--   0        0        0     1223 2023-07-21 16:31:26.455287 uk_bin_collection-0.5.0/uk_bin_collection/tests/council_schemas/LisburnCastlereaghCityCouncil.schema
+-rw-r--r--   0        0        0      999 2023-07-21 16:31:26.455287 uk_bin_collection-0.5.0/uk_bin_collection/tests/council_schemas/LondonBoroughHounslow.schema
+-rw-r--r--   0        0        0      999 2023-07-21 16:31:26.455287 uk_bin_collection-0.5.0/uk_bin_collection/tests/council_schemas/MaldonDistrictCouncil.schema
+-rw-r--r--   0        0        0      999 2023-07-21 16:31:26.455287 uk_bin_collection-0.5.0/uk_bin_collection/tests/council_schemas/MalvernHillsDC.schema
+-rw-r--r--   0        0        0      999 2023-07-21 16:31:26.455287 uk_bin_collection-0.5.0/uk_bin_collection/tests/council_schemas/ManchesterCityCouncil.schema
+-rw-r--r--   0        0        0     1007 2023-07-21 16:31:26.455287 uk_bin_collection-0.5.0/uk_bin_collection/tests/council_schemas/MertonCouncil.schema
+-rw-r--r--   0        0        0      999 2023-07-21 16:31:26.455287 uk_bin_collection-0.5.0/uk_bin_collection/tests/council_schemas/MidSussexDistrictCouncil.schema
+-rw-r--r--   0        0        0      999 2023-07-21 16:31:26.455287 uk_bin_collection-0.5.0/uk_bin_collection/tests/council_schemas/MiltonKeynesCityCouncil.schema
+-rw-r--r--   0        0        0     1244 2023-07-21 16:31:26.455287 uk_bin_collection-0.5.0/uk_bin_collection/tests/council_schemas/NewarkAndSherwoodDC.schema
+-rw-r--r--   0        0        0      999 2023-07-21 16:31:26.455287 uk_bin_collection-0.5.0/uk_bin_collection/tests/council_schemas/NewcastleCityCouncil.schema
+-rw-r--r--   0        0        0     1319 2023-07-21 16:31:26.455287 uk_bin_collection-0.5.0/uk_bin_collection/tests/council_schemas/NorthEastLincs.schema
+-rw-r--r--   0        0        0      999 2023-07-21 16:31:26.455287 uk_bin_collection-0.5.0/uk_bin_collection/tests/council_schemas/NorthKestevenDistrictCouncil.schema
+-rw-r--r--   0        0        0      999 2023-07-21 16:31:26.455287 uk_bin_collection-0.5.0/uk_bin_collection/tests/council_schemas/NorthLanarkshireCouncil.schema
+-rw-r--r--   0        0        0     1398 2023-07-21 16:31:26.455287 uk_bin_collection-0.5.0/uk_bin_collection/tests/council_schemas/NorthLincolnshireCouncil.schema
+-rw-r--r--   0        0        0     1002 2023-07-21 16:31:26.455287 uk_bin_collection-0.5.0/uk_bin_collection/tests/council_schemas/NorthNorfolkDistrictCouncil.schema
+-rw-r--r--   0        0        0     1002 2023-07-21 16:31:26.455287 uk_bin_collection-0.5.0/uk_bin_collection/tests/council_schemas/NorthSomersetCouncil.schema
+-rw-r--r--   0        0        0     1262 2023-07-21 16:31:26.455287 uk_bin_collection-0.5.0/uk_bin_collection/tests/council_schemas/NorthTynesideCouncil.schema
+-rw-r--r--   0        0        0     1310 2023-07-21 16:31:26.455287 uk_bin_collection-0.5.0/uk_bin_collection/tests/council_schemas/NorthumberlandCouncil.schema
+-rw-r--r--   0        0        0     1337 2023-07-21 16:31:26.455287 uk_bin_collection-0.5.0/uk_bin_collection/tests/council_schemas/PrestonCityCouncil.schema
+-rw-r--r--   0        0        0      999 2023-07-21 16:31:26.455287 uk_bin_collection-0.5.0/uk_bin_collection/tests/council_schemas/RochdaleCouncil.schema
+-rw-r--r--   0        0        0      999 2023-07-21 16:31:26.455287 uk_bin_collection-0.5.0/uk_bin_collection/tests/council_schemas/RushcliffeBoroughCouncil.schema
+-rw-r--r--   0        0        0     1209 2023-07-21 16:31:26.455287 uk_bin_collection-0.5.0/uk_bin_collection/tests/council_schemas/RushmoorCouncil.schema
+-rw-r--r--   0        0        0     1313 2023-07-21 16:31:26.455287 uk_bin_collection-0.5.0/uk_bin_collection/tests/council_schemas/SalfordCityCouncil.schema
+-rw-r--r--   0        0        0      999 2023-07-21 16:31:26.455287 uk_bin_collection-0.5.0/uk_bin_collection/tests/council_schemas/SheffieldCityCouncil.schema
+-rw-r--r--   0        0        0      999 2023-07-21 16:31:26.455287 uk_bin_collection-0.5.0/uk_bin_collection/tests/council_schemas/SomersetCouncil.schema
+-rw-r--r--   0        0        0      999 2023-07-21 16:31:26.455287 uk_bin_collection-0.5.0/uk_bin_collection/tests/council_schemas/SouthAyrshireCouncil.schema
+-rw-r--r--   0        0        0     1219 2023-07-21 16:31:26.455287 uk_bin_collection-0.5.0/uk_bin_collection/tests/council_schemas/SouthCambridgeshireCouncil.schema
+-rw-r--r--   0        0        0      999 2023-07-21 16:31:26.455287 uk_bin_collection-0.5.0/uk_bin_collection/tests/council_schemas/SouthLanarkshireCouncil.schema
+-rw-r--r--   0        0        0      999 2023-07-21 16:31:26.455287 uk_bin_collection-0.5.0/uk_bin_collection/tests/council_schemas/SouthNorfolkCouncil.schema
+-rw-r--r--   0        0        0      999 2023-07-21 16:31:26.455287 uk_bin_collection-0.5.0/uk_bin_collection/tests/council_schemas/SouthOxfordshireCouncil.schema
+-rw-r--r--   0        0        0     1236 2023-07-21 16:31:26.455287 uk_bin_collection-0.5.0/uk_bin_collection/tests/council_schemas/SouthTynesideCouncil.schema
+-rw-r--r--   0        0        0      999 2023-07-21 16:31:26.455287 uk_bin_collection-0.5.0/uk_bin_collection/tests/council_schemas/StHelensBC.schema
+-rw-r--r--   0        0        0      999 2023-07-21 16:31:26.455287 uk_bin_collection-0.5.0/uk_bin_collection/tests/council_schemas/StockportBoroughCouncil.schema
+-rw-r--r--   0        0        0      999 2023-07-21 16:31:26.455287 uk_bin_collection-0.5.0/uk_bin_collection/tests/council_schemas/SwaleBoroughCouncil.schema
+-rw-r--r--   0        0        0      999 2023-07-21 16:31:26.455287 uk_bin_collection-0.5.0/uk_bin_collection/tests/council_schemas/TamesideMBCouncil.schema
+-rw-r--r--   0        0        0     1002 2023-07-21 16:31:26.455287 uk_bin_collection-0.5.0/uk_bin_collection/tests/council_schemas/TonbridgeAndMallingBC.schema
+-rw-r--r--   0        0        0     1002 2023-07-21 16:31:26.455287 uk_bin_collection-0.5.0/uk_bin_collection/tests/council_schemas/TorbayCouncil.schema
+-rw-r--r--   0        0        0      999 2023-07-21 16:31:26.455287 uk_bin_collection-0.5.0/uk_bin_collection/tests/council_schemas/TorridgeDistrictCouncil.schema
+-rw-r--r--   0        0        0     1202 2023-07-21 16:31:26.455287 uk_bin_collection-0.5.0/uk_bin_collection/tests/council_schemas/ValeofGlamorganCouncil.schema
+-rw-r--r--   0        0        0      999 2023-07-21 16:31:26.455287 uk_bin_collection-0.5.0/uk_bin_collection/tests/council_schemas/WakefieldCityCouncil.schema
+-rw-r--r--   0        0        0      999 2023-07-21 16:31:26.455287 uk_bin_collection-0.5.0/uk_bin_collection/tests/council_schemas/WarwickDistrictCouncil.schema
+-rw-r--r--   0        0        0     1283 2023-07-21 16:31:26.455287 uk_bin_collection-0.5.0/uk_bin_collection/tests/council_schemas/WaverleyBoroughCouncil.schema
+-rw-r--r--   0        0        0      999 2023-07-21 16:31:26.455287 uk_bin_collection-0.5.0/uk_bin_collection/tests/council_schemas/WealdenDistrictCouncil.schema
+-rw-r--r--   0        0        0      999 2023-07-21 16:31:26.455287 uk_bin_collection-0.5.0/uk_bin_collection/tests/council_schemas/WelhatCouncil.schema
+-rw-r--r--   0        0        0      382 2023-07-21 16:31:26.455287 uk_bin_collection-0.5.0/uk_bin_collection/tests/council_schemas/WiganBoroughCouncil.schema
+-rw-r--r--   0        0        0     1273 2023-07-21 16:31:26.455287 uk_bin_collection-0.5.0/uk_bin_collection/tests/council_schemas/WiltshireCouncil.schema
+-rw-r--r--   0        0        0      999 2023-07-21 16:31:26.455287 uk_bin_collection-0.5.0/uk_bin_collection/tests/council_schemas/WindsorAndMaidenheadCouncil.schema
+-rw-r--r--   0        0        0      999 2023-07-21 16:31:26.455287 uk_bin_collection-0.5.0/uk_bin_collection/tests/council_schemas/WokingBoroughCouncil.schema
+-rw-r--r--   0        0        0      999 2023-07-21 16:31:26.455287 uk_bin_collection-0.5.0/uk_bin_collection/tests/council_schemas/YorkCouncil.schema
+-rw-r--r--   0        0        0      127 2023-07-21 16:31:26.455287 uk_bin_collection-0.5.0/uk_bin_collection/tests/features/environment.py
+-rw-r--r--   0        0        0     3281 2023-07-21 16:31:26.455287 uk_bin_collection-0.5.0/uk_bin_collection/tests/features/validate_council_outputs.feature
+-rw-r--r--   0        0        0    24132 2023-07-21 16:31:26.455287 uk_bin_collection-0.5.0/uk_bin_collection/tests/input.json
+-rw-r--r--   0        0        0      606 2023-07-21 16:31:26.455287 uk_bin_collection-0.5.0/uk_bin_collection/tests/outputs/BCPCouncil.json
+-rw-r--r--   0        0        0     2284 2023-07-21 16:31:26.455287 uk_bin_collection-0.5.0/uk_bin_collection/tests/outputs/BasingstokeCouncil.json
+-rw-r--r--   0        0        0     3473 2023-07-21 16:31:26.455287 uk_bin_collection-0.5.0/uk_bin_collection/tests/outputs/BexleyCouncil.json
+-rw-r--r--   0        0        0      501 2023-07-21 16:31:26.455287 uk_bin_collection-0.5.0/uk_bin_collection/tests/outputs/BlackburnCouncil.json
+-rw-r--r--   0        0        0     1192 2023-07-21 16:31:26.455287 uk_bin_collection-0.5.0/uk_bin_collection/tests/outputs/BoltonCouncil.json
+-rw-r--r--   0        0        0      557 2023-07-21 16:31:26.455287 uk_bin_collection-0.5.0/uk_bin_collection/tests/outputs/BristolCityCouncil.json
+-rw-r--r--   0        0        0      462 2023-07-21 16:31:26.455287 uk_bin_collection-0.5.0/uk_bin_collection/tests/outputs/BromleyBoroughCouncil.json
+-rw-r--r--   0        0        0      315 2023-07-21 16:31:26.455287 uk_bin_collection-0.5.0/uk_bin_collection/tests/outputs/BroxtoweBoroughCouncil.json
+-rw-r--r--   0        0        0     1156 2023-07-21 16:31:26.455287 uk_bin_collection-0.5.0/uk_bin_collection/tests/outputs/CardiffCouncil.json
+-rw-r--r--   0        0        0      958 2023-07-21 16:31:26.455287 uk_bin_collection-0.5.0/uk_bin_collection/tests/outputs/CastlepointDistrictCouncil.json
+-rw-r--r--   0        0        0      213 2023-07-21 16:31:26.455287 uk_bin_collection-0.5.0/uk_bin_collection/tests/outputs/CharnwoodBoroughCouncil.json
+-rw-r--r--   0        0        0     1830 2023-07-21 16:31:26.455287 uk_bin_collection-0.5.0/uk_bin_collection/tests/outputs/ChelmsfordCityCouncil.json
+-rw-r--r--   0        0        0     1187 2023-07-21 16:31:26.455287 uk_bin_collection-0.5.0/uk_bin_collection/tests/outputs/CheshireEastCouncil.json
+-rw-r--r--   0        0        0      493 2023-07-21 16:31:26.455287 uk_bin_collection-0.5.0/uk_bin_collection/tests/outputs/Chilterns.json
+-rw-r--r--   0        0        0      271 2023-07-21 16:31:26.455287 uk_bin_collection-0.5.0/uk_bin_collection/tests/outputs/CrawleyBoroughCouncil.json
+-rw-r--r--   0        0        0      466 2023-07-21 16:31:26.455287 uk_bin_collection-0.5.0/uk_bin_collection/tests/outputs/CroydonCouncil.json
+-rw-r--r--   0        0        0      562 2023-07-21 16:31:26.455287 uk_bin_collection-0.5.0/uk_bin_collection/tests/outputs/DerbyshireDalesDistrictCouncil.json
+-rw-r--r--   0        0        0      775 2023-07-21 16:31:26.455287 uk_bin_collection-0.5.0/uk_bin_collection/tests/outputs/DoncasterCouncil.json
+-rw-r--r--   0        0        0      214 2023-07-21 16:31:26.455287 uk_bin_collection-0.5.0/uk_bin_collection/tests/outputs/DurhamCouncil.json
+-rw-r--r--   0        0        0     1606 2023-07-21 16:31:26.455287 uk_bin_collection-0.5.0/uk_bin_collection/tests/outputs/EastCambridgeshireCouncil.json
+-rw-r--r--   0        0        0     2635 2023-07-21 16:31:26.455287 uk_bin_collection-0.5.0/uk_bin_collection/tests/outputs/EastDevonDC.json
+-rw-r--r--   0        0        0      982 2023-07-21 16:31:26.455287 uk_bin_collection-0.5.0/uk_bin_collection/tests/outputs/EastNorthamptonshireCouncil.json
+-rw-r--r--   0        0        0      312 2023-07-21 16:31:26.455287 uk_bin_collection-0.5.0/uk_bin_collection/tests/outputs/EastRidingCouncil.json
+-rw-r--r--   0        0        0      547 2023-07-21 16:31:26.455287 uk_bin_collection-0.5.0/uk_bin_collection/tests/outputs/EastleighBoroughCouncil.json
+-rw-r--r--   0        0        0      325 2023-07-21 16:31:26.455287 uk_bin_collection-0.5.0/uk_bin_collection/tests/outputs/ErewashBoroughCouncil.json
+-rw-r--r--   0        0        0     1362 2023-07-21 16:31:26.455287 uk_bin_collection-0.5.0/uk_bin_collection/tests/outputs/FenlandDistrictCouncil.json
+-rw-r--r--   0        0        0     4251 2023-07-21 16:31:26.455287 uk_bin_collection-0.5.0/uk_bin_collection/tests/outputs/GlasgowCityCouncil.json
+-rw-r--r--   0        0        0     1726 2023-07-21 16:31:26.455287 uk_bin_collection-0.5.0/uk_bin_collection/tests/outputs/HighPeakCouncil.json
+-rw-r--r--   0        0        0      335 2023-07-21 16:31:26.455287 uk_bin_collection-0.5.0/uk_bin_collection/tests/outputs/HuntingdonDistrictCouncil.json
+-rw-r--r--   0        0        0      534 2023-07-21 16:31:26.455287 uk_bin_collection-0.5.0/uk_bin_collection/tests/outputs/KingstonUponThamesCouncil.json
+-rw-r--r--   0        0        0     1789 2023-07-21 16:31:26.455287 uk_bin_collection-0.5.0/uk_bin_collection/tests/outputs/LeedsCityCouncil.json
+-rw-r--r--   0        0        0      608 2023-07-21 16:31:26.455287 uk_bin_collection-0.5.0/uk_bin_collection/tests/outputs/LisburnCastlereaghCityCouncil.json
+-rw-r--r--   0        0        0     1445 2023-07-21 16:31:26.455287 uk_bin_collection-0.5.0/uk_bin_collection/tests/outputs/LondonBoroughHounslow.json
+-rw-r--r--   0        0        0      409 2023-07-21 16:31:26.455287 uk_bin_collection-0.5.0/uk_bin_collection/tests/outputs/MaldonDistrictCouncil.json
+-rw-r--r--   0        0        0      227 2023-07-21 16:31:26.455287 uk_bin_collection-0.5.0/uk_bin_collection/tests/outputs/MalvernHillsDC.json
+-rw-r--r--   0        0        0      416 2023-07-21 16:31:26.455287 uk_bin_collection-0.5.0/uk_bin_collection/tests/outputs/ManchesterCityCouncil.json
+-rw-r--r--   0        0        0      665 2023-07-21 16:31:26.455287 uk_bin_collection-0.5.0/uk_bin_collection/tests/outputs/MertonCouncil.json
+-rw-r--r--   0        0        0      148 2023-07-21 16:31:26.455287 uk_bin_collection-0.5.0/uk_bin_collection/tests/outputs/MidSussexDistrictCouncil.json
+-rw-r--r--   0        0        0      862 2023-07-21 16:31:26.455287 uk_bin_collection-0.5.0/uk_bin_collection/tests/outputs/MiltonKeynesCityCouncil.json
+-rw-r--r--   0        0        0     1278 2023-07-21 16:31:26.455287 uk_bin_collection-0.5.0/uk_bin_collection/tests/outputs/NewarkAndSherwoodDC.json
+-rw-r--r--   0        0        0      221 2023-07-21 16:31:26.455287 uk_bin_collection-0.5.0/uk_bin_collection/tests/outputs/NewcastleCityCouncil.json
+-rw-r--r--   0        0        0     4096 2023-07-21 16:31:26.455287 uk_bin_collection-0.5.0/uk_bin_collection/tests/outputs/NorthEastLincs.json
+-rw-r--r--   0        0        0      446 2023-07-21 16:31:26.455287 uk_bin_collection-0.5.0/uk_bin_collection/tests/outputs/NorthKestevenDistrictCouncil.json
+-rw-r--r--   0        0        0      902 2023-07-21 16:31:26.459287 uk_bin_collection-0.5.0/uk_bin_collection/tests/outputs/NorthLanarkshireCouncil.json
+-rw-r--r--   0        0        0     3042 2023-07-21 16:31:26.459287 uk_bin_collection-0.5.0/uk_bin_collection/tests/outputs/NorthLincolnshireCouncil.json
+-rw-r--r--   0        0        0      300 2023-07-21 16:31:26.459287 uk_bin_collection-0.5.0/uk_bin_collection/tests/outputs/NorthNorfolkDistrictCouncil.json
+-rw-r--r--   0        0        0      590 2023-07-21 16:31:26.459287 uk_bin_collection-0.5.0/uk_bin_collection/tests/outputs/NorthSomersetCouncil.json
+-rw-r--r--   0        0        0     4935 2023-07-21 16:31:26.459287 uk_bin_collection-0.5.0/uk_bin_collection/tests/outputs/NorthTynesideCouncil.json
+-rw-r--r--   0        0        0     3956 2023-07-21 16:31:26.459287 uk_bin_collection-0.5.0/uk_bin_collection/tests/outputs/NorthumberlandCouncil.json
+-rw-r--r--   0        0        0    15934 2023-07-21 16:31:26.459287 uk_bin_collection-0.5.0/uk_bin_collection/tests/outputs/PrestonCityCouncil.json
+-rw-r--r--   0        0        0      903 2023-07-21 16:31:26.459287 uk_bin_collection-0.5.0/uk_bin_collection/tests/outputs/RochdaleCouncil.json
+-rw-r--r--   0        0        0      306 2023-07-21 16:31:26.459287 uk_bin_collection-0.5.0/uk_bin_collection/tests/outputs/RushcliffeBoroughCouncil.json
+-rw-r--r--   0        0        0     1602 2023-07-21 16:31:26.459287 uk_bin_collection-0.5.0/uk_bin_collection/tests/outputs/RushmoorCouncil.json
+-rw-r--r--   0        0        0     2734 2023-07-21 16:31:26.459287 uk_bin_collection-0.5.0/uk_bin_collection/tests/outputs/SalfordCityCouncil.json
+-rw-r--r--   0        0        0      892 2023-07-21 16:31:26.459287 uk_bin_collection-0.5.0/uk_bin_collection/tests/outputs/SheffieldCityCouncil.json
+-rw-r--r--   0        0        0      307 2023-07-21 16:31:26.459287 uk_bin_collection-0.5.0/uk_bin_collection/tests/outputs/SomersetCouncil.json
+-rw-r--r--   0        0        0     1871 2023-07-21 16:31:26.459287 uk_bin_collection-0.5.0/uk_bin_collection/tests/outputs/SouthAyrshireCouncil.json
+-rw-r--r--   0        0        0     2214 2023-07-21 16:31:26.459287 uk_bin_collection-0.5.0/uk_bin_collection/tests/outputs/SouthCambridgeshireCouncil.json
+-rw-r--r--   0        0        0      258 2023-07-21 16:31:26.459287 uk_bin_collection-0.5.0/uk_bin_collection/tests/outputs/SouthLanarkshireCouncil.json
+-rw-r--r--   0        0        0      217 2023-07-21 16:31:26.459287 uk_bin_collection-0.5.0/uk_bin_collection/tests/outputs/SouthNorfolkCouncil.json
+-rw-r--r--   0        0        0      293 2023-07-21 16:31:26.459287 uk_bin_collection-0.5.0/uk_bin_collection/tests/outputs/SouthOxfordshireCouncil.json
+-rw-r--r--   0        0        0     3283 2023-07-21 16:31:26.459287 uk_bin_collection-0.5.0/uk_bin_collection/tests/outputs/SouthTynesideCouncil.json
+-rw-r--r--   0        0        0      358 2023-07-21 16:31:26.459287 uk_bin_collection-0.5.0/uk_bin_collection/tests/outputs/StHelensBC.json
+-rw-r--r--   0        0        0      409 2023-07-21 16:31:26.459287 uk_bin_collection-0.5.0/uk_bin_collection/tests/outputs/StockportBoroughCouncil.json
+-rw-r--r--   0        0        0      922 2023-07-21 16:31:26.459287 uk_bin_collection-0.5.0/uk_bin_collection/tests/outputs/SwaleBoroughCouncil.json
+-rw-r--r--   0        0        0     1765 2023-07-21 16:31:26.459287 uk_bin_collection-0.5.0/uk_bin_collection/tests/outputs/TamesideMBCouncil.json
+-rw-r--r--   0        0        0     1037 2023-07-21 16:31:26.459287 uk_bin_collection-0.5.0/uk_bin_collection/tests/outputs/TonbridgeAndMallingBC.json
+-rw-r--r--   0        0        0     1406 2023-07-21 16:31:26.459287 uk_bin_collection-0.5.0/uk_bin_collection/tests/outputs/TorbayCouncil.json
+-rw-r--r--   0        0        0      116 2023-07-21 16:31:26.459287 uk_bin_collection-0.5.0/uk_bin_collection/tests/outputs/TorridgeDistrictCouncil.json
+-rw-r--r--   0        0        0     5934 2023-07-21 16:31:26.459287 uk_bin_collection-0.5.0/uk_bin_collection/tests/outputs/ValeofGlamorganCouncil.json
+-rw-r--r--   0        0        0      225 2023-07-21 16:31:26.459287 uk_bin_collection-0.5.0/uk_bin_collection/tests/outputs/WakefieldCityCouncil.json
+-rw-r--r--   0        0        0      318 2023-07-21 16:31:26.459287 uk_bin_collection-0.5.0/uk_bin_collection/tests/outputs/WarwickDistrictCouncil.json
+-rw-r--r--   0        0        0      964 2023-07-21 16:31:26.459287 uk_bin_collection-0.5.0/uk_bin_collection/tests/outputs/WaverleyBoroughCouncil.json
+-rw-r--r--   0        0        0      222 2023-07-21 16:31:26.459287 uk_bin_collection-0.5.0/uk_bin_collection/tests/outputs/WealdenDistrictCouncil.json
+-rw-r--r--   0        0        0      495 2023-07-21 16:31:26.459287 uk_bin_collection-0.5.0/uk_bin_collection/tests/outputs/WelhatCouncil.json
+-rw-r--r--   0        0        0      161 2023-07-21 16:31:26.459287 uk_bin_collection-0.5.0/uk_bin_collection/tests/outputs/WiganBoroughCouncil.json
+-rw-r--r--   0        0        0     1737 2023-07-21 16:31:26.459287 uk_bin_collection-0.5.0/uk_bin_collection/tests/outputs/WiltshireCouncil.json
+-rw-r--r--   0        0        0      367 2023-07-21 16:31:26.459287 uk_bin_collection-0.5.0/uk_bin_collection/tests/outputs/WindsorAndMaidenheadCouncil.json
+-rw-r--r--   0        0        0     1482 2023-07-21 16:31:26.459287 uk_bin_collection-0.5.0/uk_bin_collection/tests/outputs/WokingBoroughCouncil.json
+-rw-r--r--   0        0        0      307 2023-07-21 16:31:26.459287 uk_bin_collection-0.5.0/uk_bin_collection/tests/outputs/YorkCouncil.json
+-rw-r--r--   0        0        0     1147 2023-07-21 16:31:26.459287 uk_bin_collection-0.5.0/uk_bin_collection/tests/step_defs/step_helpers/file_handler.py
+-rw-r--r--   0        0        0     2546 2023-07-21 16:31:26.459287 uk_bin_collection-0.5.0/uk_bin_collection/tests/step_defs/test_validate_council.py
+-rw-r--r--   0        0        0     2576 2023-07-21 16:31:26.459287 uk_bin_collection-0.5.0/uk_bin_collection/tests/test_collect_data.py
+-rw-r--r--   0        0        0     3977 2023-07-21 16:31:26.459287 uk_bin_collection-0.5.0/uk_bin_collection/tests/test_common_functions.py
+-rw-r--r--   0        0        0     2881 2023-07-21 16:31:26.459287 uk_bin_collection-0.5.0/uk_bin_collection/uk_bin_collection/collect_data.py
+-rw-r--r--   0        0        0     6643 2023-07-21 16:31:26.459287 uk_bin_collection-0.5.0/uk_bin_collection/uk_bin_collection/common.py
+-rw-r--r--   0        0        0     1579 2023-07-21 16:31:26.459287 uk_bin_collection-0.5.0/uk_bin_collection/uk_bin_collection/councils/BCPCouncil.py
+-rw-r--r--   0        0        0     1936 2023-07-21 16:31:26.459287 uk_bin_collection-0.5.0/uk_bin_collection/uk_bin_collection/councils/BasingstokeCouncil.py
+-rw-r--r--   0        0        0     2237 2023-07-21 16:31:26.459287 uk_bin_collection-0.5.0/uk_bin_collection/uk_bin_collection/councils/BexleyCouncil.py
+-rw-r--r--   0        0        0     3156 2023-07-21 16:31:26.459287 uk_bin_collection-0.5.0/uk_bin_collection/uk_bin_collection/councils/BlackburnCouncil.py
+-rw-r--r--   0        0        0     3028 2023-07-21 16:31:26.459287 uk_bin_collection-0.5.0/uk_bin_collection/uk_bin_collection/councils/BoltonCouncil.py
+-rw-r--r--   0        0        0     5581 2023-07-21 16:31:26.459287 uk_bin_collection-0.5.0/uk_bin_collection/uk_bin_collection/councils/BristolCityCouncil.py
+-rw-r--r--   0        0        0     1676 2023-07-21 16:31:26.459287 uk_bin_collection-0.5.0/uk_bin_collection/uk_bin_collection/councils/BromleyBoroughCouncil.py
+-rw-r--r--   0        0        0     3733 2023-07-21 16:31:26.459287 uk_bin_collection-0.5.0/uk_bin_collection/uk_bin_collection/councils/BroxtoweBoroughCouncil.py
+-rw-r--r--   0        0        0     7214 2023-07-21 16:31:26.459287 uk_bin_collection-0.5.0/uk_bin_collection/uk_bin_collection/councils/CardiffCouncil.py
+-rw-r--r--   0        0        0     3946 2023-07-21 16:31:26.459287 uk_bin_collection-0.5.0/uk_bin_collection/uk_bin_collection/councils/CastlepointDistrictCouncil.py
+-rw-r--r--   0        0        0     1572 2023-07-21 16:31:26.459287 uk_bin_collection-0.5.0/uk_bin_collection/uk_bin_collection/councils/CharnwoodBoroughCouncil.py
+-rw-r--r--   0        0        0     2170 2023-07-21 16:31:26.459287 uk_bin_collection-0.5.0/uk_bin_collection/uk_bin_collection/councils/ChelmsfordCityCouncil.py
+-rw-r--r--   0        0        0     1541 2023-07-21 16:31:26.459287 uk_bin_collection-0.5.0/uk_bin_collection/uk_bin_collection/councils/CheshireEastCouncil.py
+-rw-r--r--   0        0        0     2938 2023-07-21 16:31:26.459287 uk_bin_collection-0.5.0/uk_bin_collection/uk_bin_collection/councils/Chilterns.py
+-rw-r--r--   0        0        0     1983 2023-07-21 16:31:26.459287 uk_bin_collection-0.5.0/uk_bin_collection/uk_bin_collection/councils/CrawleyBoroughCouncil.py
+-rw-r--r--   0        0        0    11599 2023-07-21 16:31:26.459287 uk_bin_collection-0.5.0/uk_bin_collection/uk_bin_collection/councils/CroydonCouncil.py
+-rw-r--r--   0        0        0     3499 2023-07-21 16:31:26.459287 uk_bin_collection-0.5.0/uk_bin_collection/uk_bin_collection/councils/DerbyshireDalesDistrictCouncil.py
+-rw-r--r--   0        0        0     3124 2023-07-21 16:31:26.459287 uk_bin_collection-0.5.0/uk_bin_collection/uk_bin_collection/councils/DoncasterCouncil.py
+-rw-r--r--   0        0        0     1626 2023-07-21 16:31:26.459287 uk_bin_collection-0.5.0/uk_bin_collection/uk_bin_collection/councils/DurhamCouncil.py
+-rw-r--r--   0        0        0     1506 2023-07-21 16:31:26.459287 uk_bin_collection-0.5.0/uk_bin_collection/uk_bin_collection/councils/EastCambridgeshireCouncil.py
+-rw-r--r--   0        0        0     3267 2023-07-21 16:31:26.459287 uk_bin_collection-0.5.0/uk_bin_collection/uk_bin_collection/councils/EastDevonDC.py
+-rw-r--r--   0        0        0     3756 2023-07-21 16:31:26.459287 uk_bin_collection-0.5.0/uk_bin_collection/uk_bin_collection/councils/EastNorthamptonshireCouncil.py
+-rw-r--r--   0        0        0     2170 2023-07-21 16:31:26.459287 uk_bin_collection-0.5.0/uk_bin_collection/uk_bin_collection/councils/EastRidingCouncil.py
+-rw-r--r--   0        0        0     2203 2023-07-21 16:31:26.459287 uk_bin_collection-0.5.0/uk_bin_collection/uk_bin_collection/councils/EastleighBoroughCouncil.py
+-rw-r--r--   0        0        0     2507 2023-07-21 16:31:26.459287 uk_bin_collection-0.5.0/uk_bin_collection/uk_bin_collection/councils/ErewashBoroughCouncil.py
+-rw-r--r--   0        0        0     2519 2023-07-21 16:31:26.459287 uk_bin_collection-0.5.0/uk_bin_collection/uk_bin_collection/councils/FenlandDistrictCouncil.py
+-rw-r--r--   0        0        0     2534 2023-07-21 16:31:26.459287 uk_bin_collection-0.5.0/uk_bin_collection/uk_bin_collection/councils/GlasgowCityCouncil.py
+-rw-r--r--   0        0        0     4416 2023-07-21 16:31:26.459287 uk_bin_collection-0.5.0/uk_bin_collection/uk_bin_collection/councils/HighPeakCouncil.py
+-rw-r--r--   0        0        0     1114 2023-07-21 16:31:26.459287 uk_bin_collection-0.5.0/uk_bin_collection/uk_bin_collection/councils/HuntingdonDistrictCouncil.py
+-rw-r--r--   0        0        0     1735 2023-07-21 16:31:26.459287 uk_bin_collection-0.5.0/uk_bin_collection/uk_bin_collection/councils/KingstonUponThamesCouncil.py
+-rw-r--r--   0        0        0     3712 2023-07-21 16:31:26.459287 uk_bin_collection-0.5.0/uk_bin_collection/uk_bin_collection/councils/LeedsCityCouncil.py
+-rw-r--r--   0        0        0     3313 2023-07-21 16:31:26.459287 uk_bin_collection-0.5.0/uk_bin_collection/uk_bin_collection/councils/LisburnCastlereaghCityCouncil.py
+-rw-r--r--   0        0        0     2081 2023-07-21 16:31:26.459287 uk_bin_collection-0.5.0/uk_bin_collection/uk_bin_collection/councils/LondonBoroughHounslow.py
+-rw-r--r--   0        0        0     2003 2023-07-21 16:31:26.459287 uk_bin_collection-0.5.0/uk_bin_collection/uk_bin_collection/councils/MaldonDistrictCouncil.py
+-rw-r--r--   0        0        0     2092 2023-07-21 16:31:26.459287 uk_bin_collection-0.5.0/uk_bin_collection/uk_bin_collection/councils/MalvernHillsDC.py
+-rw-r--r--   0        0        0     4949 2023-07-21 16:31:26.459287 uk_bin_collection-0.5.0/uk_bin_collection/uk_bin_collection/councils/ManchesterCityCouncil.py
+-rw-r--r--   0        0        0     1895 2023-07-21 16:31:26.459287 uk_bin_collection-0.5.0/uk_bin_collection/uk_bin_collection/councils/MertonCouncil.py
+-rw-r--r--   0        0        0     2711 2023-07-21 16:31:26.459287 uk_bin_collection-0.5.0/uk_bin_collection/uk_bin_collection/councils/MidSussexDistrictCouncil.py
+-rw-r--r--   0        0        0     2011 2023-07-21 16:31:26.459287 uk_bin_collection-0.5.0/uk_bin_collection/uk_bin_collection/councils/MiltonKeynesCityCouncil.py
+-rw-r--r--   0        0        0     2146 2023-07-21 16:31:26.459287 uk_bin_collection-0.5.0/uk_bin_collection/uk_bin_collection/councils/NewarkAndSherwoodDC.py
+-rw-r--r--   0        0        0     1997 2023-07-21 16:31:26.459287 uk_bin_collection-0.5.0/uk_bin_collection/uk_bin_collection/councils/NewcastleCityCouncil.py
+-rw-r--r--   0        0        0     1831 2023-07-21 16:31:26.459287 uk_bin_collection-0.5.0/uk_bin_collection/uk_bin_collection/councils/NorthEastLincs.py
+-rw-r--r--   0        0        0     1522 2023-07-21 16:31:26.463286 uk_bin_collection-0.5.0/uk_bin_collection/uk_bin_collection/councils/NorthKestevenDistrictCouncil.py
+-rw-r--r--   0        0        0     1675 2023-07-21 16:31:26.463286 uk_bin_collection-0.5.0/uk_bin_collection/uk_bin_collection/councils/NorthLanarkshireCouncil.py
+-rw-r--r--   0        0        0     2407 2023-07-21 16:31:26.463286 uk_bin_collection-0.5.0/uk_bin_collection/uk_bin_collection/councils/NorthLincolnshireCouncil.py
+-rw-r--r--   0        0        0     3723 2023-07-21 16:31:26.463286 uk_bin_collection-0.5.0/uk_bin_collection/uk_bin_collection/councils/NorthNorfolkDistrictCouncil.py
+-rw-r--r--   0        0        0     2679 2023-07-21 16:31:26.463286 uk_bin_collection-0.5.0/uk_bin_collection/uk_bin_collection/councils/NorthSomersetCouncil.py
+-rw-r--r--   0        0        0    10889 2023-07-21 16:31:26.463286 uk_bin_collection-0.5.0/uk_bin_collection/uk_bin_collection/councils/NorthTynesideCouncil.py
+-rw-r--r--   0        0        0     4695 2023-07-21 16:31:26.463286 uk_bin_collection-0.5.0/uk_bin_collection/uk_bin_collection/councils/NorthumberlandCouncil.py
+-rw-r--r--   0        0        0     3900 2023-07-21 16:31:26.463286 uk_bin_collection-0.5.0/uk_bin_collection/uk_bin_collection/councils/PrestonCityCouncil.py
+-rw-r--r--   0        0        0     2347 2023-07-21 16:31:26.463286 uk_bin_collection-0.5.0/uk_bin_collection/uk_bin_collection/councils/RochdaleCouncil.py
+-rw-r--r--   0        0        0     3514 2023-07-21 16:31:26.463286 uk_bin_collection-0.5.0/uk_bin_collection/uk_bin_collection/councils/RushcliffeBoroughCouncil.py
+-rw-r--r--   0        0        0     2043 2023-07-21 16:31:26.463286 uk_bin_collection-0.5.0/uk_bin_collection/uk_bin_collection/councils/RushmoorCouncil.py
+-rw-r--r--   0        0        0     2512 2023-07-21 16:31:26.463286 uk_bin_collection-0.5.0/uk_bin_collection/uk_bin_collection/councils/SalfordCityCouncil.py
+-rw-r--r--   0        0        0     1997 2023-07-21 16:31:26.463286 uk_bin_collection-0.5.0/uk_bin_collection/uk_bin_collection/councils/SheffieldCityCouncil.py
+-rw-r--r--   0        0        0     8499 2023-07-21 16:31:26.463286 uk_bin_collection-0.5.0/uk_bin_collection/uk_bin_collection/councils/SomersetCouncil.py
+-rw-r--r--   0        0        0     2728 2023-07-21 16:31:26.463286 uk_bin_collection-0.5.0/uk_bin_collection/uk_bin_collection/councils/SouthAyrshireCouncil.py
+-rw-r--r--   0        0        0     2313 2023-07-21 16:31:26.463286 uk_bin_collection-0.5.0/uk_bin_collection/uk_bin_collection/councils/SouthCambridgeshireCouncil.py
+-rw-r--r--   0        0        0     3132 2023-07-21 16:31:26.463286 uk_bin_collection-0.5.0/uk_bin_collection/uk_bin_collection/councils/SouthLanarkshireCouncil.py
+-rw-r--r--   0        0        0     3966 2023-07-21 16:31:26.463286 uk_bin_collection-0.5.0/uk_bin_collection/uk_bin_collection/councils/SouthNorfolkCouncil.py
+-rw-r--r--   0        0        0     3208 2023-07-21 16:31:26.463286 uk_bin_collection-0.5.0/uk_bin_collection/uk_bin_collection/councils/SouthOxfordshireCouncil.py
+-rw-r--r--   0        0        0     3432 2023-07-21 16:31:26.463286 uk_bin_collection-0.5.0/uk_bin_collection/uk_bin_collection/councils/SouthTynesideCouncil.py
+-rw-r--r--   0        0        0     1960 2023-07-21 16:31:26.463286 uk_bin_collection-0.5.0/uk_bin_collection/uk_bin_collection/councils/StHelensBC.py
+-rw-r--r--   0        0        0     1404 2023-07-21 16:31:26.463286 uk_bin_collection-0.5.0/uk_bin_collection/uk_bin_collection/councils/StockportBoroughCouncil.py
+-rw-r--r--   0        0        0     2040 2023-07-21 16:31:26.463286 uk_bin_collection-0.5.0/uk_bin_collection/uk_bin_collection/councils/SwaleBoroughCouncil.py
+-rw-r--r--   0        0        0     2001 2023-07-21 16:31:26.463286 uk_bin_collection-0.5.0/uk_bin_collection/uk_bin_collection/councils/TamesideMBCouncil.py
+-rw-r--r--   0        0        0     4865 2023-07-21 16:31:26.463286 uk_bin_collection-0.5.0/uk_bin_collection/uk_bin_collection/councils/TonbridgeAndMallingBC.py
+-rw-r--r--   0        0        0     2035 2023-07-21 16:31:26.463286 uk_bin_collection-0.5.0/uk_bin_collection/uk_bin_collection/councils/TorbayCouncil.py
+-rw-r--r--   0        0        0     6074 2023-07-21 16:31:26.463286 uk_bin_collection-0.5.0/uk_bin_collection/uk_bin_collection/councils/TorridgeDistrictCouncil.py
+-rw-r--r--   0        0        0     4863 2023-07-21 16:31:26.463286 uk_bin_collection-0.5.0/uk_bin_collection/uk_bin_collection/councils/ValeofGlamorganCouncil.py
+-rw-r--r--   0        0        0     3916 2023-07-21 16:31:26.463286 uk_bin_collection-0.5.0/uk_bin_collection/uk_bin_collection/councils/WakefieldCityCouncil.py
+-rw-r--r--   0        0        0     1153 2023-07-21 16:31:26.463286 uk_bin_collection-0.5.0/uk_bin_collection/uk_bin_collection/councils/WarwickDistrictCouncil.py
+-rw-r--r--   0        0        0     4667 2023-07-21 16:31:26.463286 uk_bin_collection-0.5.0/uk_bin_collection/uk_bin_collection/councils/WaverleyBoroughCouncil.py
+-rw-r--r--   0        0        0     3374 2023-07-21 16:31:26.463286 uk_bin_collection-0.5.0/uk_bin_collection/uk_bin_collection/councils/WealdenDistrictCouncil.py
+-rw-r--r--   0        0        0     2284 2023-07-21 16:31:26.463286 uk_bin_collection-0.5.0/uk_bin_collection/uk_bin_collection/councils/WelhatCouncil.py
+-rw-r--r--   0        0        0     3612 2023-07-21 16:31:26.463286 uk_bin_collection-0.5.0/uk_bin_collection/uk_bin_collection/councils/WiganBoroughCouncil.py
+-rw-r--r--   0        0        0     5207 2023-07-21 16:31:26.463286 uk_bin_collection-0.5.0/uk_bin_collection/uk_bin_collection/councils/WiltshireCouncil.py
+-rw-r--r--   0        0        0     5536 2023-07-21 16:31:26.463286 uk_bin_collection-0.5.0/uk_bin_collection/uk_bin_collection/councils/WindsorAndMaidenheadCouncil.py
+-rw-r--r--   0        0        0     5027 2023-07-21 16:31:26.463286 uk_bin_collection-0.5.0/uk_bin_collection/uk_bin_collection/councils/WokingBoroughCouncil.py
+-rw-r--r--   0        0        0     1496 2023-07-21 16:31:26.463286 uk_bin_collection-0.5.0/uk_bin_collection/uk_bin_collection/councils/YorkCouncil.py
+-rw-r--r--   0        0        0     1121 2023-07-21 16:31:26.463286 uk_bin_collection-0.5.0/uk_bin_collection/uk_bin_collection/councils/council_class_template/councilclasstemplate.py
+-rw-r--r--   0        0        0     4574 2023-07-21 16:31:26.463286 uk_bin_collection-0.5.0/uk_bin_collection/uk_bin_collection/get_bin_data.py
+-rw-r--r--   0        0        0     7818 1970-01-01 00:00:00.000000 uk_bin_collection-0.5.0/PKG-INFO
```

### Comparing `uk_bin_collection-0.2.0/LICENSE` & `uk_bin_collection-0.5.0/LICENSE`

 * *Files identical despite different names*

### Comparing `uk_bin_collection-0.2.0/README.md` & `uk_bin_collection-0.5.0/README.md`

 * *Files 2% similar despite different names*

```diff
@@ -81,16 +81,16 @@
 
 Please be aware that this project is run by volunteer contributors and completion depends on numerous factors - even with a request, we cannot guarantee if/when your council will get a script.
 
 ---
 
 ## Reports
 
-- [3.9](https://robbrad.github.io/UKBinCollectionData/3.9/)
-- [3.8](https://robbrad.github.io/UKBinCollectionData/3.8/)
+- [3.10](https://robbrad.github.io/UKBinCollectionData/3.10/)
+- [3.11](https://robbrad.github.io/UKBinCollectionData/3.11/)
 
 ---
 
 ## FAQ
 #### I've got an issue/support question - what do I do?
 Please post in the [HomeAssistant thread](https://community.home-assistant.io/t/bin-waste-collection/55451) or raise a new (non council request) [issue](https://github.com/robbrad/UKBinCollectionData/issues/new).
```

### Comparing `uk_bin_collection-0.2.0/pyproject.toml` & `uk_bin_collection-0.5.0/pyproject.toml`

 * *Files 8% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 [tool.poetry]
 name = "uk_bin_collection"
-version = "0.2.0"
+version = "0.5.0"
 description = "Python Lib to collect UK Bin Data"
 readme = "README.md"
 authors = ["Robert Bradley <robbrad182@gmail.com>"]
 packages = [
     { include = "uk_bin_collection", from = "." },
 ]
 include = ["uk_bin_collection"]
@@ -46,12 +46,12 @@
 envs = ["main"]
 to = {format = "poetry", path = "pyproject.toml"}
 
 [tool.poetry.dependencies]
 bs4 = "*"
 holidays = ">=0.16"
 pandas = "*"
-python = ">=3.8,<4"
+python = ">=3.10"
 requests = "*"
 selenium = "^4.8.0"
 lxml = "^4.9.2"
```

### Comparing `uk_bin_collection-0.2.0/uk_bin_collection/tests/council_schemas/BCPCouncil.schema` & `uk_bin_collection-0.5.0/uk_bin_collection/tests/council_schemas/BCPCouncil.schema`

 * *Files identical despite different names*

### Comparing `uk_bin_collection-0.2.0/uk_bin_collection/tests/council_schemas/BasingstokeCouncil.schema` & `uk_bin_collection-0.5.0/uk_bin_collection/tests/council_schemas/BasingstokeCouncil.schema`

 * *Files identical despite different names*

### Comparing `uk_bin_collection-0.2.0/uk_bin_collection/tests/council_schemas/BexleyCouncil.schema` & `uk_bin_collection-0.5.0/uk_bin_collection/tests/council_schemas/BexleyCouncil.schema`

 * *Files identical despite different names*

### Comparing `uk_bin_collection-0.2.0/uk_bin_collection/tests/council_schemas/BlackburnCouncil.schema` & `uk_bin_collection-0.5.0/uk_bin_collection/tests/council_schemas/BlackburnCouncil.schema`

 * *Files identical despite different names*

### Comparing `uk_bin_collection-0.2.0/uk_bin_collection/tests/council_schemas/BoltonCouncil.schema` & `uk_bin_collection-0.5.0/uk_bin_collection/tests/council_schemas/BoltonCouncil.schema`

 * *Files identical despite different names*

### Comparing `uk_bin_collection-0.2.0/uk_bin_collection/tests/council_schemas/BristolCityCouncil.schema` & `uk_bin_collection-0.5.0/uk_bin_collection/tests/council_schemas/BristolCityCouncil.schema`

 * *Files identical despite different names*

### Comparing `uk_bin_collection-0.2.0/uk_bin_collection/tests/council_schemas/BromleyBoroughCouncil.schema` & `uk_bin_collection-0.5.0/uk_bin_collection/tests/council_schemas/BromleyBoroughCouncil.schema`

 * *Files identical despite different names*

### Comparing `uk_bin_collection-0.2.0/uk_bin_collection/tests/council_schemas/BroxtoweBoroughCouncil.schema` & `uk_bin_collection-0.5.0/uk_bin_collection/tests/council_schemas/BroxtoweBoroughCouncil.schema`

 * *Files identical despite different names*

### Comparing `uk_bin_collection-0.2.0/uk_bin_collection/tests/council_schemas/CardiffCouncil.schema` & `uk_bin_collection-0.5.0/uk_bin_collection/tests/council_schemas/CardiffCouncil.schema`

 * *Files identical despite different names*

### Comparing `uk_bin_collection-0.2.0/uk_bin_collection/tests/council_schemas/CastlepointDistrictCouncil.schema` & `uk_bin_collection-0.5.0/uk_bin_collection/tests/council_schemas/CastlepointDistrictCouncil.schema`

 * *Files identical despite different names*

### Comparing `uk_bin_collection-0.2.0/uk_bin_collection/tests/council_schemas/CharnwoodBoroughCouncil.schema` & `uk_bin_collection-0.5.0/uk_bin_collection/tests/council_schemas/CharnwoodBoroughCouncil.schema`

 * *Files identical despite different names*

### Comparing `uk_bin_collection-0.2.0/uk_bin_collection/tests/council_schemas/ChelmsfordCityCouncil.schema` & `uk_bin_collection-0.5.0/uk_bin_collection/tests/council_schemas/ChelmsfordCityCouncil.schema`

 * *Files identical despite different names*

### Comparing `uk_bin_collection-0.2.0/uk_bin_collection/tests/council_schemas/CheshireEastCouncil.schema` & `uk_bin_collection-0.5.0/uk_bin_collection/tests/council_schemas/CheshireEastCouncil.schema`

 * *Files identical despite different names*

### Comparing `uk_bin_collection-0.2.0/uk_bin_collection/tests/council_schemas/Chilterns.schema` & `uk_bin_collection-0.5.0/uk_bin_collection/tests/council_schemas/Chilterns.schema`

 * *Files identical despite different names*

### Comparing `uk_bin_collection-0.2.0/uk_bin_collection/tests/council_schemas/CrawleyBoroughCouncil.schema` & `uk_bin_collection-0.5.0/uk_bin_collection/tests/council_schemas/CrawleyBoroughCouncil.schema`

 * *Files identical despite different names*

### Comparing `uk_bin_collection-0.2.0/uk_bin_collection/tests/council_schemas/CroydonCouncil.schema` & `uk_bin_collection-0.5.0/uk_bin_collection/tests/council_schemas/CroydonCouncil.schema`

 * *Files identical despite different names*

### Comparing `uk_bin_collection-0.2.0/uk_bin_collection/tests/council_schemas/DerbyshireDalesDistrictCouncil.schema` & `uk_bin_collection-0.5.0/uk_bin_collection/tests/council_schemas/DerbyshireDalesDistrictCouncil.schema`

 * *Files identical despite different names*

### Comparing `uk_bin_collection-0.2.0/uk_bin_collection/tests/council_schemas/DoncasterCouncil.schema` & `uk_bin_collection-0.5.0/uk_bin_collection/tests/council_schemas/DoncasterCouncil.schema`

 * *Files identical despite different names*

### Comparing `uk_bin_collection-0.2.0/uk_bin_collection/tests/council_schemas/DurhamCouncil.schema` & `uk_bin_collection-0.5.0/uk_bin_collection/tests/council_schemas/DurhamCouncil.schema`

 * *Files identical despite different names*

### Comparing `uk_bin_collection-0.2.0/uk_bin_collection/tests/council_schemas/EastCambridgeshireCouncil.schema` & `uk_bin_collection-0.5.0/uk_bin_collection/tests/council_schemas/EastCambridgeshireCouncil.schema`

 * *Files identical despite different names*

### Comparing `uk_bin_collection-0.2.0/uk_bin_collection/tests/council_schemas/EastDevonDC.schema` & `uk_bin_collection-0.5.0/uk_bin_collection/tests/council_schemas/EastDevonDC.schema`

 * *Files identical despite different names*

### Comparing `uk_bin_collection-0.2.0/uk_bin_collection/tests/council_schemas/EastNorthamptonshireCouncil.schema` & `uk_bin_collection-0.5.0/uk_bin_collection/tests/council_schemas/EastNorthamptonshireCouncil.schema`

 * *Files identical despite different names*

### Comparing `uk_bin_collection-0.2.0/uk_bin_collection/tests/council_schemas/EastRidingCouncil.schema` & `uk_bin_collection-0.5.0/uk_bin_collection/tests/council_schemas/EastRidingCouncil.schema`

 * *Files identical despite different names*

### Comparing `uk_bin_collection-0.2.0/uk_bin_collection/tests/council_schemas/EastleighBoroughCouncil.schema` & `uk_bin_collection-0.5.0/uk_bin_collection/tests/council_schemas/EastleighBoroughCouncil.schema`

 * *Files identical despite different names*

### Comparing `uk_bin_collection-0.2.0/uk_bin_collection/tests/council_schemas/ErewashBoroughCouncil.schema` & `uk_bin_collection-0.5.0/uk_bin_collection/tests/council_schemas/ErewashBoroughCouncil.schema`

 * *Files identical despite different names*

### Comparing `uk_bin_collection-0.2.0/uk_bin_collection/tests/council_schemas/FenlandDistrictCouncil.schema` & `uk_bin_collection-0.5.0/uk_bin_collection/tests/council_schemas/FenlandDistrictCouncil.schema`

 * *Files identical despite different names*

### Comparing `uk_bin_collection-0.2.0/uk_bin_collection/tests/council_schemas/GlasgowCityCouncil.schema` & `uk_bin_collection-0.5.0/uk_bin_collection/tests/council_schemas/GlasgowCityCouncil.schema`

 * *Files identical despite different names*

### Comparing `uk_bin_collection-0.2.0/uk_bin_collection/tests/council_schemas/HighPeakCouncil.schema` & `uk_bin_collection-0.5.0/uk_bin_collection/tests/council_schemas/HighPeakCouncil.schema`

 * *Files identical despite different names*

### Comparing `uk_bin_collection-0.2.0/uk_bin_collection/tests/council_schemas/HuntingdonDistrictCouncil.schema` & `uk_bin_collection-0.5.0/uk_bin_collection/tests/council_schemas/HuntingdonDistrictCouncil.schema`

 * *Files identical despite different names*

### Comparing `uk_bin_collection-0.2.0/uk_bin_collection/tests/council_schemas/KingstonUponThamesCouncil.schema` & `uk_bin_collection-0.5.0/uk_bin_collection/tests/council_schemas/KingstonUponThamesCouncil.schema`

 * *Files identical despite different names*

### Comparing `uk_bin_collection-0.2.0/uk_bin_collection/tests/council_schemas/LeedsCityCouncil.schema` & `uk_bin_collection-0.5.0/uk_bin_collection/tests/council_schemas/LeedsCityCouncil.schema`

 * *Files identical despite different names*

### Comparing `uk_bin_collection-0.2.0/uk_bin_collection/tests/council_schemas/LisburnCastlereaghCityCouncil.schema` & `uk_bin_collection-0.5.0/uk_bin_collection/tests/council_schemas/LisburnCastlereaghCityCouncil.schema`

 * *Files identical despite different names*

### Comparing `uk_bin_collection-0.2.0/uk_bin_collection/tests/council_schemas/LondonBoroughHounslow.schema` & `uk_bin_collection-0.5.0/uk_bin_collection/tests/council_schemas/LondonBoroughHounslow.schema`

 * *Files identical despite different names*

### Comparing `uk_bin_collection-0.2.0/uk_bin_collection/tests/council_schemas/MaldonDistrictCouncil.schema` & `uk_bin_collection-0.5.0/uk_bin_collection/tests/council_schemas/MaldonDistrictCouncil.schema`

 * *Files identical despite different names*

### Comparing `uk_bin_collection-0.2.0/uk_bin_collection/tests/council_schemas/MalvernHillsDC.schema` & `uk_bin_collection-0.5.0/uk_bin_collection/tests/council_schemas/MalvernHillsDC.schema`

 * *Files identical despite different names*

### Comparing `uk_bin_collection-0.2.0/uk_bin_collection/tests/council_schemas/ManchesterCityCouncil.schema` & `uk_bin_collection-0.5.0/uk_bin_collection/tests/council_schemas/ManchesterCityCouncil.schema`

 * *Files identical despite different names*

### Comparing `uk_bin_collection-0.2.0/uk_bin_collection/tests/council_schemas/MertonCouncil.schema` & `uk_bin_collection-0.5.0/uk_bin_collection/tests/council_schemas/MertonCouncil.schema`

 * *Files identical despite different names*

### Comparing `uk_bin_collection-0.2.0/uk_bin_collection/tests/council_schemas/MidSussexDistrictCouncil.schema` & `uk_bin_collection-0.5.0/uk_bin_collection/tests/council_schemas/MidSussexDistrictCouncil.schema`

 * *Files identical despite different names*

### Comparing `uk_bin_collection-0.2.0/uk_bin_collection/tests/council_schemas/MiltonKeynesCityCouncil.schema` & `uk_bin_collection-0.5.0/uk_bin_collection/tests/council_schemas/MiltonKeynesCityCouncil.schema`

 * *Files identical despite different names*

### Comparing `uk_bin_collection-0.2.0/uk_bin_collection/tests/council_schemas/NewarkAndSherwoodDC.schema` & `uk_bin_collection-0.5.0/uk_bin_collection/tests/council_schemas/NewarkAndSherwoodDC.schema`

 * *Files identical despite different names*

### Comparing `uk_bin_collection-0.2.0/uk_bin_collection/tests/council_schemas/NewcastleCityCouncil.schema` & `uk_bin_collection-0.5.0/uk_bin_collection/tests/council_schemas/NewcastleCityCouncil.schema`

 * *Files identical despite different names*

### Comparing `uk_bin_collection-0.2.0/uk_bin_collection/tests/council_schemas/NorthEastLincs.schema` & `uk_bin_collection-0.5.0/uk_bin_collection/tests/council_schemas/NorthEastLincs.schema`

 * *Files identical despite different names*

### Comparing `uk_bin_collection-0.2.0/uk_bin_collection/tests/council_schemas/NorthKestevenDistrictCouncil.schema` & `uk_bin_collection-0.5.0/uk_bin_collection/tests/council_schemas/NorthKestevenDistrictCouncil.schema`

 * *Files identical despite different names*

### Comparing `uk_bin_collection-0.2.0/uk_bin_collection/tests/council_schemas/NorthLanarkshireCouncil.schema` & `uk_bin_collection-0.5.0/uk_bin_collection/tests/council_schemas/NorthLanarkshireCouncil.schema`

 * *Files identical despite different names*

### Comparing `uk_bin_collection-0.2.0/uk_bin_collection/tests/council_schemas/NorthLincolnshireCouncil.schema` & `uk_bin_collection-0.5.0/uk_bin_collection/tests/council_schemas/NorthLincolnshireCouncil.schema`

 * *Files identical despite different names*

### Comparing `uk_bin_collection-0.2.0/uk_bin_collection/tests/council_schemas/NorthNorfolkDistrictCouncil.schema` & `uk_bin_collection-0.5.0/uk_bin_collection/tests/council_schemas/NorthNorfolkDistrictCouncil.schema`

 * *Files identical despite different names*

### Comparing `uk_bin_collection-0.2.0/uk_bin_collection/tests/council_schemas/NorthSomersetCouncil.schema` & `uk_bin_collection-0.5.0/uk_bin_collection/tests/council_schemas/NorthSomersetCouncil.schema`

 * *Files identical despite different names*

### Comparing `uk_bin_collection-0.2.0/uk_bin_collection/tests/council_schemas/NorthTynesideCouncil.schema` & `uk_bin_collection-0.5.0/uk_bin_collection/tests/council_schemas/NorthTynesideCouncil.schema`

 * *Files identical despite different names*

### Comparing `uk_bin_collection-0.2.0/uk_bin_collection/tests/council_schemas/NorthumberlandCouncil.schema` & `uk_bin_collection-0.5.0/uk_bin_collection/tests/council_schemas/NorthumberlandCouncil.schema`

 * *Files identical despite different names*

### Comparing `uk_bin_collection-0.2.0/uk_bin_collection/tests/council_schemas/PrestonCityCouncil.schema` & `uk_bin_collection-0.5.0/uk_bin_collection/tests/council_schemas/PrestonCityCouncil.schema`

 * *Files identical despite different names*

### Comparing `uk_bin_collection-0.2.0/uk_bin_collection/tests/council_schemas/RochdaleCouncil.schema` & `uk_bin_collection-0.5.0/uk_bin_collection/tests/council_schemas/RochdaleCouncil.schema`

 * *Files identical despite different names*

### Comparing `uk_bin_collection-0.2.0/uk_bin_collection/tests/council_schemas/RushcliffeBoroughCouncil.schema` & `uk_bin_collection-0.5.0/uk_bin_collection/tests/council_schemas/RushcliffeBoroughCouncil.schema`

 * *Files identical despite different names*

### Comparing `uk_bin_collection-0.2.0/uk_bin_collection/tests/council_schemas/RushmoorCouncil.schema` & `uk_bin_collection-0.5.0/uk_bin_collection/tests/council_schemas/RushmoorCouncil.schema`

 * *Files identical despite different names*

### Comparing `uk_bin_collection-0.2.0/uk_bin_collection/tests/council_schemas/SalfordCityCouncil.schema` & `uk_bin_collection-0.5.0/uk_bin_collection/tests/council_schemas/SalfordCityCouncil.schema`

 * *Files identical despite different names*

### Comparing `uk_bin_collection-0.2.0/uk_bin_collection/tests/council_schemas/SheffieldCityCouncil.schema` & `uk_bin_collection-0.5.0/uk_bin_collection/tests/council_schemas/SheffieldCityCouncil.schema`

 * *Files identical despite different names*

### Comparing `uk_bin_collection-0.2.0/uk_bin_collection/tests/council_schemas/SomersetCouncil.schema` & `uk_bin_collection-0.5.0/uk_bin_collection/tests/council_schemas/SomersetCouncil.schema`

 * *Files identical despite different names*

### Comparing `uk_bin_collection-0.2.0/uk_bin_collection/tests/council_schemas/SouthAyrshireCouncil.schema` & `uk_bin_collection-0.5.0/uk_bin_collection/tests/council_schemas/SouthAyrshireCouncil.schema`

 * *Files identical despite different names*

### Comparing `uk_bin_collection-0.2.0/uk_bin_collection/tests/council_schemas/SouthCambridgeshireCouncil.schema` & `uk_bin_collection-0.5.0/uk_bin_collection/tests/council_schemas/SouthCambridgeshireCouncil.schema`

 * *Files identical despite different names*

### Comparing `uk_bin_collection-0.2.0/uk_bin_collection/tests/council_schemas/SouthLanarkshireCouncil.schema` & `uk_bin_collection-0.5.0/uk_bin_collection/tests/council_schemas/SouthLanarkshireCouncil.schema`

 * *Files identical despite different names*

### Comparing `uk_bin_collection-0.2.0/uk_bin_collection/tests/council_schemas/SouthNorfolkCouncil.schema` & `uk_bin_collection-0.5.0/uk_bin_collection/tests/council_schemas/SouthNorfolkCouncil.schema`

 * *Files identical despite different names*

### Comparing `uk_bin_collection-0.2.0/uk_bin_collection/tests/council_schemas/SouthOxfordshireCouncil.schema` & `uk_bin_collection-0.5.0/uk_bin_collection/tests/council_schemas/SouthOxfordshireCouncil.schema`

 * *Files identical despite different names*

### Comparing `uk_bin_collection-0.2.0/uk_bin_collection/tests/council_schemas/SouthTynesideCouncil.schema` & `uk_bin_collection-0.5.0/uk_bin_collection/tests/council_schemas/SouthTynesideCouncil.schema`

 * *Files identical despite different names*

### Comparing `uk_bin_collection-0.2.0/uk_bin_collection/tests/council_schemas/StHelensBC.schema` & `uk_bin_collection-0.5.0/uk_bin_collection/tests/council_schemas/StHelensBC.schema`

 * *Files identical despite different names*

### Comparing `uk_bin_collection-0.2.0/uk_bin_collection/tests/council_schemas/StockportBoroughCouncil.schema` & `uk_bin_collection-0.5.0/uk_bin_collection/tests/council_schemas/StockportBoroughCouncil.schema`

 * *Files identical despite different names*

### Comparing `uk_bin_collection-0.2.0/uk_bin_collection/tests/council_schemas/SwaleBoroughCouncil.schema` & `uk_bin_collection-0.5.0/uk_bin_collection/tests/council_schemas/SwaleBoroughCouncil.schema`

 * *Files identical despite different names*

### Comparing `uk_bin_collection-0.2.0/uk_bin_collection/tests/council_schemas/TamesideMBCouncil.schema` & `uk_bin_collection-0.5.0/uk_bin_collection/tests/council_schemas/TamesideMBCouncil.schema`

 * *Files identical despite different names*

### Comparing `uk_bin_collection-0.2.0/uk_bin_collection/tests/council_schemas/TonbridgeAndMallingBC.schema` & `uk_bin_collection-0.5.0/uk_bin_collection/tests/council_schemas/TonbridgeAndMallingBC.schema`

 * *Files identical despite different names*

### Comparing `uk_bin_collection-0.2.0/uk_bin_collection/tests/council_schemas/TorbayCouncil.schema` & `uk_bin_collection-0.5.0/uk_bin_collection/tests/council_schemas/TorbayCouncil.schema`

 * *Files identical despite different names*

### Comparing `uk_bin_collection-0.2.0/uk_bin_collection/tests/council_schemas/TorridgeDistrictCouncil.schema` & `uk_bin_collection-0.5.0/uk_bin_collection/tests/council_schemas/TorridgeDistrictCouncil.schema`

 * *Files identical despite different names*

### Comparing `uk_bin_collection-0.2.0/uk_bin_collection/tests/council_schemas/ValeofGlamorganCouncil.schema` & `uk_bin_collection-0.5.0/uk_bin_collection/tests/council_schemas/ValeofGlamorganCouncil.schema`

 * *Files identical despite different names*

### Comparing `uk_bin_collection-0.2.0/uk_bin_collection/tests/council_schemas/WakefieldCityCouncil.schema` & `uk_bin_collection-0.5.0/uk_bin_collection/tests/council_schemas/WakefieldCityCouncil.schema`

 * *Files identical despite different names*

### Comparing `uk_bin_collection-0.2.0/uk_bin_collection/tests/council_schemas/WarwickDistrictCouncil.schema` & `uk_bin_collection-0.5.0/uk_bin_collection/tests/council_schemas/WarwickDistrictCouncil.schema`

 * *Files identical despite different names*

### Comparing `uk_bin_collection-0.2.0/uk_bin_collection/tests/council_schemas/WaverleyBoroughCouncil.schema` & `uk_bin_collection-0.5.0/uk_bin_collection/tests/council_schemas/WaverleyBoroughCouncil.schema`

 * *Files identical despite different names*

### Comparing `uk_bin_collection-0.2.0/uk_bin_collection/tests/council_schemas/WealdenDistrictCouncil.schema` & `uk_bin_collection-0.5.0/uk_bin_collection/tests/council_schemas/WealdenDistrictCouncil.schema`

 * *Files identical despite different names*

### Comparing `uk_bin_collection-0.2.0/uk_bin_collection/tests/council_schemas/WelhatCouncil.schema` & `uk_bin_collection-0.5.0/uk_bin_collection/tests/council_schemas/WelhatCouncil.schema`

 * *Files identical despite different names*

### Comparing `uk_bin_collection-0.2.0/uk_bin_collection/tests/council_schemas/WiltshireCouncil.schema` & `uk_bin_collection-0.5.0/uk_bin_collection/tests/council_schemas/WiltshireCouncil.schema`

 * *Files identical despite different names*

### Comparing `uk_bin_collection-0.2.0/uk_bin_collection/tests/council_schemas/WindsorAndMaidenheadCouncil.schema` & `uk_bin_collection-0.5.0/uk_bin_collection/tests/council_schemas/WindsorAndMaidenheadCouncil.schema`

 * *Files identical despite different names*

### Comparing `uk_bin_collection-0.2.0/uk_bin_collection/tests/council_schemas/WokingBoroughCouncil.schema` & `uk_bin_collection-0.5.0/uk_bin_collection/tests/council_schemas/WokingBoroughCouncil.schema`

 * *Files identical despite different names*

### Comparing `uk_bin_collection-0.2.0/uk_bin_collection/tests/council_schemas/YorkCouncil.schema` & `uk_bin_collection-0.5.0/uk_bin_collection/tests/council_schemas/YorkCouncil.schema`

 * *Files identical despite different names*

### Comparing `uk_bin_collection-0.2.0/uk_bin_collection/tests/features/validate_council_outputs.feature` & `uk_bin_collection-0.5.0/uk_bin_collection/tests/features/validate_council_outputs.feature`

 * *Files identical despite different names*

### Comparing `uk_bin_collection-0.2.0/uk_bin_collection/tests/input.json` & `uk_bin_collection-0.5.0/uk_bin_collection/tests/input.json`

 * *Files identical despite different names*

### Comparing `uk_bin_collection-0.2.0/uk_bin_collection/tests/outputs/BCPCouncil.json` & `uk_bin_collection-0.5.0/uk_bin_collection/tests/outputs/BCPCouncil.json`

 * *Files identical despite different names*

### Comparing `uk_bin_collection-0.2.0/uk_bin_collection/tests/outputs/BasingstokeCouncil.json` & `uk_bin_collection-0.5.0/uk_bin_collection/tests/outputs/BasingstokeCouncil.json`

 * *Files identical despite different names*

### Comparing `uk_bin_collection-0.2.0/uk_bin_collection/tests/outputs/BexleyCouncil.json` & `uk_bin_collection-0.5.0/uk_bin_collection/tests/outputs/BexleyCouncil.json`

 * *Files identical despite different names*

### Comparing `uk_bin_collection-0.2.0/uk_bin_collection/tests/outputs/BoltonCouncil.json` & `uk_bin_collection-0.5.0/uk_bin_collection/tests/outputs/BoltonCouncil.json`

 * *Files identical despite different names*

### Comparing `uk_bin_collection-0.2.0/uk_bin_collection/tests/outputs/BristolCityCouncil.json` & `uk_bin_collection-0.5.0/uk_bin_collection/tests/outputs/BristolCityCouncil.json`

 * *Files identical despite different names*

### Comparing `uk_bin_collection-0.2.0/uk_bin_collection/tests/outputs/CardiffCouncil.json` & `uk_bin_collection-0.5.0/uk_bin_collection/tests/outputs/CardiffCouncil.json`

 * *Files identical despite different names*

### Comparing `uk_bin_collection-0.2.0/uk_bin_collection/tests/outputs/CastlepointDistrictCouncil.json` & `uk_bin_collection-0.5.0/uk_bin_collection/tests/outputs/CastlepointDistrictCouncil.json`

 * *Files identical despite different names*

### Comparing `uk_bin_collection-0.2.0/uk_bin_collection/tests/outputs/ChelmsfordCityCouncil.json` & `uk_bin_collection-0.5.0/uk_bin_collection/tests/outputs/ChelmsfordCityCouncil.json`

 * *Files identical despite different names*

### Comparing `uk_bin_collection-0.2.0/uk_bin_collection/tests/outputs/CheshireEastCouncil.json` & `uk_bin_collection-0.5.0/uk_bin_collection/tests/outputs/CheshireEastCouncil.json`

 * *Files identical despite different names*

### Comparing `uk_bin_collection-0.2.0/uk_bin_collection/tests/outputs/DerbyshireDalesDistrictCouncil.json` & `uk_bin_collection-0.5.0/uk_bin_collection/tests/outputs/DerbyshireDalesDistrictCouncil.json`

 * *Files identical despite different names*

### Comparing `uk_bin_collection-0.2.0/uk_bin_collection/tests/outputs/DoncasterCouncil.json` & `uk_bin_collection-0.5.0/uk_bin_collection/tests/outputs/DoncasterCouncil.json`

 * *Files identical despite different names*

### Comparing `uk_bin_collection-0.2.0/uk_bin_collection/tests/outputs/EastCambridgeshireCouncil.json` & `uk_bin_collection-0.5.0/uk_bin_collection/tests/outputs/EastCambridgeshireCouncil.json`

 * *Files identical despite different names*

### Comparing `uk_bin_collection-0.2.0/uk_bin_collection/tests/outputs/EastDevonDC.json` & `uk_bin_collection-0.5.0/uk_bin_collection/tests/outputs/EastDevonDC.json`

 * *Files identical despite different names*

### Comparing `uk_bin_collection-0.2.0/uk_bin_collection/tests/outputs/EastNorthamptonshireCouncil.json` & `uk_bin_collection-0.5.0/uk_bin_collection/tests/outputs/EastNorthamptonshireCouncil.json`

 * *Files identical despite different names*

### Comparing `uk_bin_collection-0.2.0/uk_bin_collection/tests/outputs/EastleighBoroughCouncil.json` & `uk_bin_collection-0.5.0/uk_bin_collection/tests/outputs/EastleighBoroughCouncil.json`

 * *Files identical despite different names*

### Comparing `uk_bin_collection-0.2.0/uk_bin_collection/tests/outputs/FenlandDistrictCouncil.json` & `uk_bin_collection-0.5.0/uk_bin_collection/tests/outputs/FenlandDistrictCouncil.json`

 * *Files identical despite different names*

### Comparing `uk_bin_collection-0.2.0/uk_bin_collection/tests/outputs/GlasgowCityCouncil.json` & `uk_bin_collection-0.5.0/uk_bin_collection/tests/outputs/GlasgowCityCouncil.json`

 * *Files identical despite different names*

### Comparing `uk_bin_collection-0.2.0/uk_bin_collection/tests/outputs/HighPeakCouncil.json` & `uk_bin_collection-0.5.0/uk_bin_collection/tests/outputs/HighPeakCouncil.json`

 * *Files identical despite different names*

### Comparing `uk_bin_collection-0.2.0/uk_bin_collection/tests/outputs/KingstonUponThamesCouncil.json` & `uk_bin_collection-0.5.0/uk_bin_collection/tests/outputs/KingstonUponThamesCouncil.json`

 * *Files identical despite different names*

### Comparing `uk_bin_collection-0.2.0/uk_bin_collection/tests/outputs/LeedsCityCouncil.json` & `uk_bin_collection-0.5.0/uk_bin_collection/tests/outputs/LeedsCityCouncil.json`

 * *Files identical despite different names*

### Comparing `uk_bin_collection-0.2.0/uk_bin_collection/tests/outputs/LisburnCastlereaghCityCouncil.json` & `uk_bin_collection-0.5.0/uk_bin_collection/tests/outputs/LisburnCastlereaghCityCouncil.json`

 * *Files identical despite different names*

### Comparing `uk_bin_collection-0.2.0/uk_bin_collection/tests/outputs/LondonBoroughHounslow.json` & `uk_bin_collection-0.5.0/uk_bin_collection/tests/outputs/LondonBoroughHounslow.json`

 * *Files identical despite different names*

### Comparing `uk_bin_collection-0.2.0/uk_bin_collection/tests/outputs/MertonCouncil.json` & `uk_bin_collection-0.5.0/uk_bin_collection/tests/outputs/MertonCouncil.json`

 * *Files identical despite different names*

### Comparing `uk_bin_collection-0.2.0/uk_bin_collection/tests/outputs/MiltonKeynesCityCouncil.json` & `uk_bin_collection-0.5.0/uk_bin_collection/tests/outputs/MiltonKeynesCityCouncil.json`

 * *Files identical despite different names*

### Comparing `uk_bin_collection-0.2.0/uk_bin_collection/tests/outputs/NewarkAndSherwoodDC.json` & `uk_bin_collection-0.5.0/uk_bin_collection/tests/outputs/NewarkAndSherwoodDC.json`

 * *Files identical despite different names*

### Comparing `uk_bin_collection-0.2.0/uk_bin_collection/tests/outputs/NorthEastLincs.json` & `uk_bin_collection-0.5.0/uk_bin_collection/tests/outputs/NorthEastLincs.json`

 * *Files identical despite different names*

### Comparing `uk_bin_collection-0.2.0/uk_bin_collection/tests/outputs/NorthLanarkshireCouncil.json` & `uk_bin_collection-0.5.0/uk_bin_collection/tests/outputs/NorthLanarkshireCouncil.json`

 * *Files identical despite different names*

### Comparing `uk_bin_collection-0.2.0/uk_bin_collection/tests/outputs/NorthLincolnshireCouncil.json` & `uk_bin_collection-0.5.0/uk_bin_collection/tests/outputs/NorthLincolnshireCouncil.json`

 * *Files identical despite different names*

### Comparing `uk_bin_collection-0.2.0/uk_bin_collection/tests/outputs/NorthSomersetCouncil.json` & `uk_bin_collection-0.5.0/uk_bin_collection/tests/outputs/NorthSomersetCouncil.json`

 * *Files identical despite different names*

### Comparing `uk_bin_collection-0.2.0/uk_bin_collection/tests/outputs/NorthTynesideCouncil.json` & `uk_bin_collection-0.5.0/uk_bin_collection/tests/outputs/NorthTynesideCouncil.json`

 * *Files identical despite different names*

### Comparing `uk_bin_collection-0.2.0/uk_bin_collection/tests/outputs/NorthumberlandCouncil.json` & `uk_bin_collection-0.5.0/uk_bin_collection/tests/outputs/NorthumberlandCouncil.json`

 * *Files identical despite different names*

### Comparing `uk_bin_collection-0.2.0/uk_bin_collection/tests/outputs/PrestonCityCouncil.json` & `uk_bin_collection-0.5.0/uk_bin_collection/tests/outputs/PrestonCityCouncil.json`

 * *Files identical despite different names*

### Comparing `uk_bin_collection-0.2.0/uk_bin_collection/tests/outputs/RochdaleCouncil.json` & `uk_bin_collection-0.5.0/uk_bin_collection/tests/outputs/RochdaleCouncil.json`

 * *Files identical despite different names*

### Comparing `uk_bin_collection-0.2.0/uk_bin_collection/tests/outputs/RushmoorCouncil.json` & `uk_bin_collection-0.5.0/uk_bin_collection/tests/outputs/RushmoorCouncil.json`

 * *Files identical despite different names*

### Comparing `uk_bin_collection-0.2.0/uk_bin_collection/tests/outputs/SalfordCityCouncil.json` & `uk_bin_collection-0.5.0/uk_bin_collection/tests/outputs/SalfordCityCouncil.json`

 * *Files identical despite different names*

### Comparing `uk_bin_collection-0.2.0/uk_bin_collection/tests/outputs/SheffieldCityCouncil.json` & `uk_bin_collection-0.5.0/uk_bin_collection/tests/outputs/SheffieldCityCouncil.json`

 * *Files identical despite different names*

### Comparing `uk_bin_collection-0.2.0/uk_bin_collection/tests/outputs/SouthAyrshireCouncil.json` & `uk_bin_collection-0.5.0/uk_bin_collection/tests/outputs/SouthAyrshireCouncil.json`

 * *Files identical despite different names*

### Comparing `uk_bin_collection-0.2.0/uk_bin_collection/tests/outputs/SouthCambridgeshireCouncil.json` & `uk_bin_collection-0.5.0/uk_bin_collection/tests/outputs/SouthCambridgeshireCouncil.json`

 * *Files identical despite different names*

### Comparing `uk_bin_collection-0.2.0/uk_bin_collection/tests/outputs/SouthTynesideCouncil.json` & `uk_bin_collection-0.5.0/uk_bin_collection/tests/outputs/SouthTynesideCouncil.json`

 * *Files identical despite different names*

### Comparing `uk_bin_collection-0.2.0/uk_bin_collection/tests/outputs/SwaleBoroughCouncil.json` & `uk_bin_collection-0.5.0/uk_bin_collection/tests/outputs/SwaleBoroughCouncil.json`

 * *Files identical despite different names*

### Comparing `uk_bin_collection-0.2.0/uk_bin_collection/tests/outputs/TamesideMBCouncil.json` & `uk_bin_collection-0.5.0/uk_bin_collection/tests/outputs/TamesideMBCouncil.json`

 * *Files identical despite different names*

### Comparing `uk_bin_collection-0.2.0/uk_bin_collection/tests/outputs/TonbridgeAndMallingBC.json` & `uk_bin_collection-0.5.0/uk_bin_collection/tests/outputs/TonbridgeAndMallingBC.json`

 * *Files identical despite different names*

### Comparing `uk_bin_collection-0.2.0/uk_bin_collection/tests/outputs/TorbayCouncil.json` & `uk_bin_collection-0.5.0/uk_bin_collection/tests/outputs/TorbayCouncil.json`

 * *Files identical despite different names*

### Comparing `uk_bin_collection-0.2.0/uk_bin_collection/tests/outputs/ValeofGlamorganCouncil.json` & `uk_bin_collection-0.5.0/uk_bin_collection/tests/outputs/ValeofGlamorganCouncil.json`

 * *Files identical despite different names*

### Comparing `uk_bin_collection-0.2.0/uk_bin_collection/tests/outputs/WaverleyBoroughCouncil.json` & `uk_bin_collection-0.5.0/uk_bin_collection/tests/outputs/WaverleyBoroughCouncil.json`

 * *Files identical despite different names*

### Comparing `uk_bin_collection-0.2.0/uk_bin_collection/tests/outputs/WiltshireCouncil.json` & `uk_bin_collection-0.5.0/uk_bin_collection/tests/outputs/WiltshireCouncil.json`

 * *Files identical despite different names*

### Comparing `uk_bin_collection-0.2.0/uk_bin_collection/tests/outputs/WokingBoroughCouncil.json` & `uk_bin_collection-0.5.0/uk_bin_collection/tests/outputs/WokingBoroughCouncil.json`

 * *Files identical despite different names*

### Comparing `uk_bin_collection-0.2.0/uk_bin_collection/tests/step_defs/step_helpers/file_handler.py` & `uk_bin_collection-0.5.0/uk_bin_collection/tests/step_defs/step_helpers/file_handler.py`

 * *Files identical despite different names*

### Comparing `uk_bin_collection-0.2.0/uk_bin_collection/tests/step_defs/test_validate_council.py` & `uk_bin_collection-0.5.0/uk_bin_collection/tests/step_defs/test_validate_council.py`

 * *Files identical despite different names*

### Comparing `uk_bin_collection-0.2.0/uk_bin_collection/tests/test_collect_data.py` & `uk_bin_collection-0.5.0/uk_bin_collection/tests/test_collect_data.py`

 * *Files identical despite different names*

### Comparing `uk_bin_collection-0.2.0/uk_bin_collection/tests/test_common_functions.py` & `uk_bin_collection-0.5.0/uk_bin_collection/tests/test_common_functions.py`

 * *Files identical despite different names*

### Comparing `uk_bin_collection-0.2.0/uk_bin_collection/uk_bin_collection/collect_data.py` & `uk_bin_collection-0.5.0/uk_bin_collection/uk_bin_collection/collect_data.py`

 * *Files identical despite different names*

### Comparing `uk_bin_collection-0.2.0/uk_bin_collection/uk_bin_collection/common.py` & `uk_bin_collection-0.5.0/uk_bin_collection/uk_bin_collection/common.py`

 * *Files identical despite different names*

### Comparing `uk_bin_collection-0.2.0/uk_bin_collection/uk_bin_collection/councils/BCPCouncil.py` & `uk_bin_collection-0.5.0/uk_bin_collection/uk_bin_collection/councils/BCPCouncil.py`

 * *Files identical despite different names*

### Comparing `uk_bin_collection-0.2.0/uk_bin_collection/uk_bin_collection/councils/BasingstokeCouncil.py` & `uk_bin_collection-0.5.0/uk_bin_collection/uk_bin_collection/councils/BasingstokeCouncil.py`

 * *Files identical despite different names*

### Comparing `uk_bin_collection-0.2.0/uk_bin_collection/uk_bin_collection/councils/BexleyCouncil.py` & `uk_bin_collection-0.5.0/uk_bin_collection/uk_bin_collection/councils/BexleyCouncil.py`

 * *Files identical despite different names*

### Comparing `uk_bin_collection-0.2.0/uk_bin_collection/uk_bin_collection/councils/BlackburnCouncil.py` & `uk_bin_collection-0.5.0/uk_bin_collection/uk_bin_collection/councils/BlackburnCouncil.py`

 * *Files identical despite different names*

### Comparing `uk_bin_collection-0.2.0/uk_bin_collection/uk_bin_collection/councils/BoltonCouncil.py` & `uk_bin_collection-0.5.0/uk_bin_collection/uk_bin_collection/councils/BoltonCouncil.py`

 * *Files identical despite different names*

### Comparing `uk_bin_collection-0.2.0/uk_bin_collection/uk_bin_collection/councils/BristolCityCouncil.py` & `uk_bin_collection-0.5.0/uk_bin_collection/uk_bin_collection/councils/BristolCityCouncil.py`

 * *Files identical despite different names*

### Comparing `uk_bin_collection-0.2.0/uk_bin_collection/uk_bin_collection/councils/BromleyBoroughCouncil.py` & `uk_bin_collection-0.5.0/uk_bin_collection/uk_bin_collection/councils/BromleyBoroughCouncil.py`

 * *Files identical despite different names*

### Comparing `uk_bin_collection-0.2.0/uk_bin_collection/uk_bin_collection/councils/BroxtoweBoroughCouncil.py` & `uk_bin_collection-0.5.0/uk_bin_collection/uk_bin_collection/councils/BroxtoweBoroughCouncil.py`

 * *Files identical despite different names*

### Comparing `uk_bin_collection-0.2.0/uk_bin_collection/uk_bin_collection/councils/CardiffCouncil.py` & `uk_bin_collection-0.5.0/uk_bin_collection/uk_bin_collection/councils/CardiffCouncil.py`

 * *Files identical despite different names*

### Comparing `uk_bin_collection-0.2.0/uk_bin_collection/uk_bin_collection/councils/CastlepointDistrictCouncil.py` & `uk_bin_collection-0.5.0/uk_bin_collection/uk_bin_collection/councils/CastlepointDistrictCouncil.py`

 * *Files identical despite different names*

### Comparing `uk_bin_collection-0.2.0/uk_bin_collection/uk_bin_collection/councils/CharnwoodBoroughCouncil.py` & `uk_bin_collection-0.5.0/uk_bin_collection/uk_bin_collection/councils/StockportBoroughCouncil.py`

 * *Files 13% similar despite different names*

```diff
@@ -1,7 +1,9 @@
+# This script pulls (in one hit) the
+# data from Warick District Council Bins Data
 from bs4 import BeautifulSoup
 from uk_bin_collection.uk_bin_collection.common import *
 from uk_bin_collection.uk_bin_collection.get_bin_data import \
     AbstractGetBinDataClass
 
 
 # import the wonderful Beautiful Soup and the URL grabber
@@ -15,24 +17,22 @@
     def parse_data(self, page: str, **kwargs) -> dict:
         # Make a BS4 object
         soup = BeautifulSoup(page.text, features="html.parser")
         soup.prettify()
 
         data = {"bins": []}
 
-        for bins in soup.find_all("ul", {"class": "refuse"}):
-            binCollection = bins.find_all("li")
+        for bins in soup.select('div[class*="service-item"]'):
+            bin_type = bins.div.h3.text.strip()
+            binCollection = datetime.strptime(bins.select("div > p")[1].get_text(strip=True), "%A, %d %B %Y")
+            # binImage = "https://myaccount.stockport.gov.uk" + bins.img['src']
 
+            # batteries don't have a service date or other
+            # info associated with them.
             if binCollection:
-                for bin in binCollection:
-                    dict_data = {
-                        "type": bin.find("a").contents[0],
-                        "collectionDate": datetime.strptime(
-                            remove_ordinal_indicator_from_date_string(bin.find("strong", {"class": "date"}).contents[0])
-                            .strip(),
-                            "%a %d %b"
-                        ).strftime(date_format)
-                    }
-
-                    data["bins"].append(dict_data)
+                dict_data = {
+                    "type": bin_type,
+                    "collectionDate": binCollection.strftime(date_format)
+                }
+                data["bins"].append(dict_data)
 
         return data
```

### Comparing `uk_bin_collection-0.2.0/uk_bin_collection/uk_bin_collection/councils/ChelmsfordCityCouncil.py` & `uk_bin_collection-0.5.0/uk_bin_collection/uk_bin_collection/councils/ChelmsfordCityCouncil.py`

 * *Files identical despite different names*

### Comparing `uk_bin_collection-0.2.0/uk_bin_collection/uk_bin_collection/councils/CheshireEastCouncil.py` & `uk_bin_collection-0.5.0/uk_bin_collection/uk_bin_collection/councils/CheshireEastCouncil.py`

 * *Files identical despite different names*

### Comparing `uk_bin_collection-0.2.0/uk_bin_collection/uk_bin_collection/councils/Chilterns.py` & `uk_bin_collection-0.5.0/uk_bin_collection/uk_bin_collection/councils/Chilterns.py`

 * *Files identical despite different names*

### Comparing `uk_bin_collection-0.2.0/uk_bin_collection/uk_bin_collection/councils/CrawleyBoroughCouncil.py` & `uk_bin_collection-0.5.0/uk_bin_collection/uk_bin_collection/councils/CrawleyBoroughCouncil.py`

 * *Files identical despite different names*

### Comparing `uk_bin_collection-0.2.0/uk_bin_collection/uk_bin_collection/councils/CroydonCouncil.py` & `uk_bin_collection-0.5.0/uk_bin_collection/uk_bin_collection/councils/CroydonCouncil.py`

 * *Files identical despite different names*

### Comparing `uk_bin_collection-0.2.0/uk_bin_collection/uk_bin_collection/councils/DerbyshireDalesDistrictCouncil.py` & `uk_bin_collection-0.5.0/uk_bin_collection/uk_bin_collection/councils/DerbyshireDalesDistrictCouncil.py`

 * *Files identical despite different names*

### Comparing `uk_bin_collection-0.2.0/uk_bin_collection/uk_bin_collection/councils/DoncasterCouncil.py` & `uk_bin_collection-0.5.0/uk_bin_collection/uk_bin_collection/councils/DoncasterCouncil.py`

 * *Files identical despite different names*

### Comparing `uk_bin_collection-0.2.0/uk_bin_collection/uk_bin_collection/councils/DurhamCouncil.py` & `uk_bin_collection-0.5.0/uk_bin_collection/uk_bin_collection/councils/DurhamCouncil.py`

 * *Files identical despite different names*

### Comparing `uk_bin_collection-0.2.0/uk_bin_collection/uk_bin_collection/councils/EastCambridgeshireCouncil.py` & `uk_bin_collection-0.5.0/uk_bin_collection/uk_bin_collection/councils/EastCambridgeshireCouncil.py`

 * *Files identical despite different names*

### Comparing `uk_bin_collection-0.2.0/uk_bin_collection/uk_bin_collection/councils/EastDevonDC.py` & `uk_bin_collection-0.5.0/uk_bin_collection/uk_bin_collection/councils/EastDevonDC.py`

 * *Files identical despite different names*

### Comparing `uk_bin_collection-0.2.0/uk_bin_collection/uk_bin_collection/councils/EastNorthamptonshireCouncil.py` & `uk_bin_collection-0.5.0/uk_bin_collection/uk_bin_collection/councils/EastNorthamptonshireCouncil.py`

 * *Files identical despite different names*

### Comparing `uk_bin_collection-0.2.0/uk_bin_collection/uk_bin_collection/councils/EastRidingCouncil.py` & `uk_bin_collection-0.5.0/uk_bin_collection/uk_bin_collection/councils/EastRidingCouncil.py`

 * *Files identical despite different names*

### Comparing `uk_bin_collection-0.2.0/uk_bin_collection/uk_bin_collection/councils/EastleighBoroughCouncil.py` & `uk_bin_collection-0.5.0/uk_bin_collection/uk_bin_collection/councils/EastleighBoroughCouncil.py`

 * *Files identical despite different names*

### Comparing `uk_bin_collection-0.2.0/uk_bin_collection/uk_bin_collection/councils/ErewashBoroughCouncil.py` & `uk_bin_collection-0.5.0/uk_bin_collection/uk_bin_collection/councils/ErewashBoroughCouncil.py`

 * *Files identical despite different names*

### Comparing `uk_bin_collection-0.2.0/uk_bin_collection/uk_bin_collection/councils/FenlandDistrictCouncil.py` & `uk_bin_collection-0.5.0/uk_bin_collection/uk_bin_collection/councils/FenlandDistrictCouncil.py`

 * *Files identical despite different names*

### Comparing `uk_bin_collection-0.2.0/uk_bin_collection/uk_bin_collection/councils/GlasgowCityCouncil.py` & `uk_bin_collection-0.5.0/uk_bin_collection/uk_bin_collection/councils/GlasgowCityCouncil.py`

 * *Files identical despite different names*

### Comparing `uk_bin_collection-0.2.0/uk_bin_collection/uk_bin_collection/councils/HighPeakCouncil.py` & `uk_bin_collection-0.5.0/uk_bin_collection/uk_bin_collection/councils/HighPeakCouncil.py`

 * *Files identical despite different names*

### Comparing `uk_bin_collection-0.2.0/uk_bin_collection/uk_bin_collection/councils/HuntingdonDistrictCouncil.py` & `uk_bin_collection-0.5.0/uk_bin_collection/uk_bin_collection/councils/HuntingdonDistrictCouncil.py`

 * *Files identical despite different names*

### Comparing `uk_bin_collection-0.2.0/uk_bin_collection/uk_bin_collection/councils/KingstonUponThamesCouncil.py` & `uk_bin_collection-0.5.0/uk_bin_collection/uk_bin_collection/councils/KingstonUponThamesCouncil.py`

 * *Files identical despite different names*

### Comparing `uk_bin_collection-0.2.0/uk_bin_collection/uk_bin_collection/councils/LeedsCityCouncil.py` & `uk_bin_collection-0.5.0/uk_bin_collection/uk_bin_collection/councils/LeedsCityCouncil.py`

 * *Files identical despite different names*

### Comparing `uk_bin_collection-0.2.0/uk_bin_collection/uk_bin_collection/councils/LisburnCastlereaghCityCouncil.py` & `uk_bin_collection-0.5.0/uk_bin_collection/uk_bin_collection/councils/LisburnCastlereaghCityCouncil.py`

 * *Files identical despite different names*

### Comparing `uk_bin_collection-0.2.0/uk_bin_collection/uk_bin_collection/councils/LondonBoroughHounslow.py` & `uk_bin_collection-0.5.0/uk_bin_collection/uk_bin_collection/councils/LondonBoroughHounslow.py`

 * *Files identical despite different names*

### Comparing `uk_bin_collection-0.2.0/uk_bin_collection/uk_bin_collection/councils/MaldonDistrictCouncil.py` & `uk_bin_collection-0.5.0/uk_bin_collection/uk_bin_collection/councils/MaldonDistrictCouncil.py`

 * *Files identical despite different names*

### Comparing `uk_bin_collection-0.2.0/uk_bin_collection/uk_bin_collection/councils/MalvernHillsDC.py` & `uk_bin_collection-0.5.0/uk_bin_collection/uk_bin_collection/councils/MalvernHillsDC.py`

 * *Files identical despite different names*

### Comparing `uk_bin_collection-0.2.0/uk_bin_collection/uk_bin_collection/councils/ManchesterCityCouncil.py` & `uk_bin_collection-0.5.0/uk_bin_collection/uk_bin_collection/councils/ManchesterCityCouncil.py`

 * *Files identical despite different names*

### Comparing `uk_bin_collection-0.2.0/uk_bin_collection/uk_bin_collection/councils/MertonCouncil.py` & `uk_bin_collection-0.5.0/uk_bin_collection/uk_bin_collection/councils/MertonCouncil.py`

 * *Files identical despite different names*

### Comparing `uk_bin_collection-0.2.0/uk_bin_collection/uk_bin_collection/councils/MidSussexDistrictCouncil.py` & `uk_bin_collection-0.5.0/uk_bin_collection/uk_bin_collection/councils/MidSussexDistrictCouncil.py`

 * *Files identical despite different names*

### Comparing `uk_bin_collection-0.2.0/uk_bin_collection/uk_bin_collection/councils/MiltonKeynesCityCouncil.py` & `uk_bin_collection-0.5.0/uk_bin_collection/uk_bin_collection/councils/MiltonKeynesCityCouncil.py`

 * *Files identical despite different names*

### Comparing `uk_bin_collection-0.2.0/uk_bin_collection/uk_bin_collection/councils/NewarkAndSherwoodDC.py` & `uk_bin_collection-0.5.0/uk_bin_collection/uk_bin_collection/councils/NewarkAndSherwoodDC.py`

 * *Files identical despite different names*

### Comparing `uk_bin_collection-0.2.0/uk_bin_collection/uk_bin_collection/councils/NewcastleCityCouncil.py` & `uk_bin_collection-0.5.0/uk_bin_collection/uk_bin_collection/councils/NewcastleCityCouncil.py`

 * *Files identical despite different names*

### Comparing `uk_bin_collection-0.2.0/uk_bin_collection/uk_bin_collection/councils/NorthEastLincs.py` & `uk_bin_collection-0.5.0/uk_bin_collection/uk_bin_collection/councils/NorthEastLincs.py`

 * *Files identical despite different names*

### Comparing `uk_bin_collection-0.2.0/uk_bin_collection/uk_bin_collection/councils/NorthKestevenDistrictCouncil.py` & `uk_bin_collection-0.5.0/uk_bin_collection/uk_bin_collection/councils/NorthKestevenDistrictCouncil.py`

 * *Files identical despite different names*

### Comparing `uk_bin_collection-0.2.0/uk_bin_collection/uk_bin_collection/councils/NorthLanarkshireCouncil.py` & `uk_bin_collection-0.5.0/uk_bin_collection/uk_bin_collection/councils/NorthLanarkshireCouncil.py`

 * *Files identical despite different names*

### Comparing `uk_bin_collection-0.2.0/uk_bin_collection/uk_bin_collection/councils/NorthLincolnshireCouncil.py` & `uk_bin_collection-0.5.0/uk_bin_collection/uk_bin_collection/councils/NorthLincolnshireCouncil.py`

 * *Files identical despite different names*

### Comparing `uk_bin_collection-0.2.0/uk_bin_collection/uk_bin_collection/councils/NorthNorfolkDistrictCouncil.py` & `uk_bin_collection-0.5.0/uk_bin_collection/uk_bin_collection/councils/NorthNorfolkDistrictCouncil.py`

 * *Files identical despite different names*

### Comparing `uk_bin_collection-0.2.0/uk_bin_collection/uk_bin_collection/councils/NorthSomersetCouncil.py` & `uk_bin_collection-0.5.0/uk_bin_collection/uk_bin_collection/councils/NorthSomersetCouncil.py`

 * *Files identical despite different names*

### Comparing `uk_bin_collection-0.2.0/uk_bin_collection/uk_bin_collection/councils/NorthTynesideCouncil.py` & `uk_bin_collection-0.5.0/uk_bin_collection/uk_bin_collection/councils/NorthTynesideCouncil.py`

 * *Files identical despite different names*

### Comparing `uk_bin_collection-0.2.0/uk_bin_collection/uk_bin_collection/councils/NorthumberlandCouncil.py` & `uk_bin_collection-0.5.0/uk_bin_collection/uk_bin_collection/councils/NorthumberlandCouncil.py`

 * *Files identical despite different names*

### Comparing `uk_bin_collection-0.2.0/uk_bin_collection/uk_bin_collection/councils/PrestonCityCouncil.py` & `uk_bin_collection-0.5.0/uk_bin_collection/uk_bin_collection/councils/PrestonCityCouncil.py`

 * *Files identical despite different names*

### Comparing `uk_bin_collection-0.2.0/uk_bin_collection/uk_bin_collection/councils/RochdaleCouncil.py` & `uk_bin_collection-0.5.0/uk_bin_collection/uk_bin_collection/councils/RochdaleCouncil.py`

 * *Files identical despite different names*

### Comparing `uk_bin_collection-0.2.0/uk_bin_collection/uk_bin_collection/councils/RushcliffeBoroughCouncil.py` & `uk_bin_collection-0.5.0/uk_bin_collection/uk_bin_collection/councils/RushcliffeBoroughCouncil.py`

 * *Files identical despite different names*

### Comparing `uk_bin_collection-0.2.0/uk_bin_collection/uk_bin_collection/councils/RushmoorCouncil.py` & `uk_bin_collection-0.5.0/uk_bin_collection/uk_bin_collection/councils/RushmoorCouncil.py`

 * *Files identical despite different names*

### Comparing `uk_bin_collection-0.2.0/uk_bin_collection/uk_bin_collection/councils/SalfordCityCouncil.py` & `uk_bin_collection-0.5.0/uk_bin_collection/uk_bin_collection/councils/SalfordCityCouncil.py`

 * *Files identical despite different names*

### Comparing `uk_bin_collection-0.2.0/uk_bin_collection/uk_bin_collection/councils/SheffieldCityCouncil.py` & `uk_bin_collection-0.5.0/uk_bin_collection/uk_bin_collection/councils/SheffieldCityCouncil.py`

 * *Files identical despite different names*

### Comparing `uk_bin_collection-0.2.0/uk_bin_collection/uk_bin_collection/councils/SomersetCouncil.py` & `uk_bin_collection-0.5.0/uk_bin_collection/uk_bin_collection/councils/SomersetCouncil.py`

 * *Files identical despite different names*

### Comparing `uk_bin_collection-0.2.0/uk_bin_collection/uk_bin_collection/councils/SouthAyrshireCouncil.py` & `uk_bin_collection-0.5.0/uk_bin_collection/uk_bin_collection/councils/SouthAyrshireCouncil.py`

 * *Files identical despite different names*

### Comparing `uk_bin_collection-0.2.0/uk_bin_collection/uk_bin_collection/councils/SouthCambridgeshireCouncil.py` & `uk_bin_collection-0.5.0/uk_bin_collection/uk_bin_collection/councils/SouthCambridgeshireCouncil.py`

 * *Files identical despite different names*

### Comparing `uk_bin_collection-0.2.0/uk_bin_collection/uk_bin_collection/councils/SouthLanarkshireCouncil.py` & `uk_bin_collection-0.5.0/uk_bin_collection/uk_bin_collection/councils/SouthLanarkshireCouncil.py`

 * *Files identical despite different names*

### Comparing `uk_bin_collection-0.2.0/uk_bin_collection/uk_bin_collection/councils/SouthNorfolkCouncil.py` & `uk_bin_collection-0.5.0/uk_bin_collection/uk_bin_collection/councils/SouthNorfolkCouncil.py`

 * *Files identical despite different names*

### Comparing `uk_bin_collection-0.2.0/uk_bin_collection/uk_bin_collection/councils/SouthOxfordshireCouncil.py` & `uk_bin_collection-0.5.0/uk_bin_collection/uk_bin_collection/councils/SouthOxfordshireCouncil.py`

 * *Files identical despite different names*

### Comparing `uk_bin_collection-0.2.0/uk_bin_collection/uk_bin_collection/councils/SouthTynesideCouncil.py` & `uk_bin_collection-0.5.0/uk_bin_collection/uk_bin_collection/councils/SouthTynesideCouncil.py`

 * *Files identical despite different names*

### Comparing `uk_bin_collection-0.2.0/uk_bin_collection/uk_bin_collection/councils/StHelensBC.py` & `uk_bin_collection-0.5.0/uk_bin_collection/uk_bin_collection/councils/StHelensBC.py`

 * *Files identical despite different names*

### Comparing `uk_bin_collection-0.2.0/uk_bin_collection/uk_bin_collection/councils/StockportBoroughCouncil.py` & `uk_bin_collection-0.5.0/uk_bin_collection/uk_bin_collection/councils/council_class_template/councilclasstemplate.py`

 * *Files 16% similar despite different names*

```diff
@@ -1,9 +1,7 @@
-# This script pulls (in one hit) the
-# data from Warick District Council Bins Data
 from bs4 import BeautifulSoup
 from uk_bin_collection.uk_bin_collection.common import *
 from uk_bin_collection.uk_bin_collection.get_bin_data import \
     AbstractGetBinDataClass
 
 
 # import the wonderful Beautiful Soup and the URL grabber
@@ -19,20 +17,16 @@
         soup = BeautifulSoup(page.text, features="html.parser")
         soup.prettify()
 
         data = {"bins": []}
 
         for bins in soup.select('div[class*="service-item"]'):
             bin_type = bins.div.h3.text.strip()
-            binCollection = datetime.strptime(bins.select("div > p")[1].get_text(strip=True), "%A, %d %B %Y")
-            # binImage = "https://myaccount.stockport.gov.uk" + bins.img['src']
-
-            # batteries don't have a service date or other
-            # info associated with them.
-            if binCollection:
+            bin_collection = bins.select("div > p")[1]
+            if bin_collection:
                 dict_data = {
                     "type": bin_type,
-                    "collectionDate": binCollection.strftime(date_format)
+                    "collectionDate": datetime.strptime(bin_collection.get_text(strip=True), "%A, %d %B %Y")
                 }
                 data["bins"].append(dict_data)
 
         return data
```

### Comparing `uk_bin_collection-0.2.0/uk_bin_collection/uk_bin_collection/councils/SwaleBoroughCouncil.py` & `uk_bin_collection-0.5.0/uk_bin_collection/uk_bin_collection/councils/SwaleBoroughCouncil.py`

 * *Files identical despite different names*

### Comparing `uk_bin_collection-0.2.0/uk_bin_collection/uk_bin_collection/councils/TamesideMBCouncil.py` & `uk_bin_collection-0.5.0/uk_bin_collection/uk_bin_collection/councils/TamesideMBCouncil.py`

 * *Files identical despite different names*

### Comparing `uk_bin_collection-0.2.0/uk_bin_collection/uk_bin_collection/councils/TonbridgeAndMallingBC.py` & `uk_bin_collection-0.5.0/uk_bin_collection/uk_bin_collection/councils/TonbridgeAndMallingBC.py`

 * *Files identical despite different names*

### Comparing `uk_bin_collection-0.2.0/uk_bin_collection/uk_bin_collection/councils/TorbayCouncil.py` & `uk_bin_collection-0.5.0/uk_bin_collection/uk_bin_collection/councils/TorbayCouncil.py`

 * *Files identical despite different names*

### Comparing `uk_bin_collection-0.2.0/uk_bin_collection/uk_bin_collection/councils/TorridgeDistrictCouncil.py` & `uk_bin_collection-0.5.0/uk_bin_collection/uk_bin_collection/councils/TorridgeDistrictCouncil.py`

 * *Files identical despite different names*

### Comparing `uk_bin_collection-0.2.0/uk_bin_collection/uk_bin_collection/councils/ValeofGlamorganCouncil.py` & `uk_bin_collection-0.5.0/uk_bin_collection/uk_bin_collection/councils/ValeofGlamorganCouncil.py`

 * *Files identical despite different names*

### Comparing `uk_bin_collection-0.2.0/uk_bin_collection/uk_bin_collection/councils/WakefieldCityCouncil.py` & `uk_bin_collection-0.5.0/uk_bin_collection/uk_bin_collection/councils/WakefieldCityCouncil.py`

 * *Files identical despite different names*

### Comparing `uk_bin_collection-0.2.0/uk_bin_collection/uk_bin_collection/councils/WarwickDistrictCouncil.py` & `uk_bin_collection-0.5.0/uk_bin_collection/uk_bin_collection/councils/WarwickDistrictCouncil.py`

 * *Files identical despite different names*

### Comparing `uk_bin_collection-0.2.0/uk_bin_collection/uk_bin_collection/councils/WaverleyBoroughCouncil.py` & `uk_bin_collection-0.5.0/uk_bin_collection/uk_bin_collection/councils/WaverleyBoroughCouncil.py`

 * *Files identical despite different names*

### Comparing `uk_bin_collection-0.2.0/uk_bin_collection/uk_bin_collection/councils/WealdenDistrictCouncil.py` & `uk_bin_collection-0.5.0/uk_bin_collection/uk_bin_collection/councils/WealdenDistrictCouncil.py`

 * *Files identical despite different names*

### Comparing `uk_bin_collection-0.2.0/uk_bin_collection/uk_bin_collection/councils/WelhatCouncil.py` & `uk_bin_collection-0.5.0/uk_bin_collection/uk_bin_collection/councils/WelhatCouncil.py`

 * *Files identical despite different names*

### Comparing `uk_bin_collection-0.2.0/uk_bin_collection/uk_bin_collection/councils/WiganBoroughCouncil.py` & `uk_bin_collection-0.5.0/uk_bin_collection/uk_bin_collection/councils/WiganBoroughCouncil.py`

 * *Files identical despite different names*

### Comparing `uk_bin_collection-0.2.0/uk_bin_collection/uk_bin_collection/councils/WiltshireCouncil.py` & `uk_bin_collection-0.5.0/uk_bin_collection/uk_bin_collection/councils/WiltshireCouncil.py`

 * *Files identical despite different names*

### Comparing `uk_bin_collection-0.2.0/uk_bin_collection/uk_bin_collection/councils/WindsorAndMaidenheadCouncil.py` & `uk_bin_collection-0.5.0/uk_bin_collection/uk_bin_collection/councils/WindsorAndMaidenheadCouncil.py`

 * *Files identical despite different names*

### Comparing `uk_bin_collection-0.2.0/uk_bin_collection/uk_bin_collection/councils/WokingBoroughCouncil.py` & `uk_bin_collection-0.5.0/uk_bin_collection/uk_bin_collection/councils/WokingBoroughCouncil.py`

 * *Files identical despite different names*

### Comparing `uk_bin_collection-0.2.0/uk_bin_collection/uk_bin_collection/councils/YorkCouncil.py` & `uk_bin_collection-0.5.0/uk_bin_collection/uk_bin_collection/councils/YorkCouncil.py`

 * *Files identical despite different names*

### Comparing `uk_bin_collection-0.2.0/uk_bin_collection/uk_bin_collection/get_bin_data.py` & `uk_bin_collection-0.5.0/uk_bin_collection/uk_bin_collection/get_bin_data.py`

 * *Files identical despite different names*

### Comparing `uk_bin_collection-0.2.0/setup.py` & `uk_bin_collection-0.5.0/PKG-INFO`

 * *Files 14% similar despite different names*

```diff
@@ -1,51 +1,127 @@
-# -*- coding: utf-8 -*-
-from setuptools import setup
+Metadata-Version: 2.1
+Name: uk-bin-collection
+Version: 0.5.0
+Summary: Python Lib to collect UK Bin Data
+Author: Robert Bradley
+Author-email: robbrad182@gmail.com
+Requires-Python: >=3.10
+Classifier: Programming Language :: Python :: 3
+Classifier: Programming Language :: Python :: 3.10
+Classifier: Programming Language :: Python :: 3.11
+Requires-Dist: bs4
+Requires-Dist: holidays (>=0.16)
+Requires-Dist: lxml (>=4.9.2,<5.0.0)
+Requires-Dist: pandas
+Requires-Dist: requests
+Requires-Dist: selenium (>=4.8.0,<5.0.0)
+Project-URL: issues, https://github.com/robbrad/UKBinCollectionData/issues
+Description-Content-Type: text/markdown
 
-package_dir = \
-{'': '.'}
+[![forthebadge made-with-python](http://ForTheBadge.com/images/badges/made-with-python.svg)](https://www.python.org/)
 
-packages = \
-['uk_bin_collection',
- 'uk_bin_collection.tests',
- 'uk_bin_collection.tests.features',
- 'uk_bin_collection.tests.step_defs',
- 'uk_bin_collection.tests.step_defs.step_helpers',
- 'uk_bin_collection.uk_bin_collection',
- 'uk_bin_collection.uk_bin_collection.councils',
- 'uk_bin_collection.uk_bin_collection.councils.council_class_template']
-
-package_data = \
-{'': ['*'], 'uk_bin_collection.tests': ['council_schemas/*', 'outputs/*']}
-
-install_requires = \
-['bs4',
- 'holidays>=0.16',
- 'lxml>=4.9.2,<5.0.0',
- 'pandas',
- 'requests',
- 'selenium>=4.8.0,<5.0.0']
-
-entry_points = \
-{'console_scripts': ['uk_bin_collection = '
-                     'uk_bin_collection.uk_bin_collection:collect_data']}
-
-setup_kwargs = {
-    'name': 'uk-bin-collection',
-    'version': '0.2.0',
-    'description': 'Python Lib to collect UK Bin Data',
-    'long_description': '[![forthebadge made-with-python](http://ForTheBadge.com/images/badges/made-with-python.svg)](https://www.python.org/)\n\n![GitHub](https://img.shields.io/github/license/robbrad/UKBinCollectionData?style=for-the-badge) ![GitHub issues](https://img.shields.io/github/issues-raw/robbrad/UKBinCollectionData?style=for-the-badge) ![GitHub closed issues](https://img.shields.io/github/issues-closed-raw/robbrad/UKBinCollectionData?style=for-the-badge)\n![GitHub contributors](https://img.shields.io/github/contributors/robbrad/UKBinCollectionData?style=for-the-badge)\n\n![GitHub Workflow Status](https://img.shields.io/github/actions/workflow/status/robbrad/UKBinCollectionData/behave.yml?style=for-the-badge)\n![Codecov](https://img.shields.io/codecov/c/gh/robbrad/UKBinCollectionData?style=for-the-badge)\n\n[![pages-build-deployment](https://github.com/robbrad/UKBinCollectionData/actions/workflows/pages/pages-build-deployment/badge.svg)](https://github.com/robbrad/UKBinCollectionData/actions/workflows/pages/pages-build-deployment) [![Test Councils](https://github.com/robbrad/UKBinCollectionData/actions/workflows/behave.yml/badge.svg)](https://github.com/robbrad/UKBinCollectionData/actions/workflows/behave.yml)\n\n# UK Bin Collection Data (UKBCD)\nThis project aims to provide a neat and standard way of providing bin collection data in JSON format from UK councils that have no API to do so.\n\nWhy do this?\nYou might want to use this in a Home Automation - for example say you had an LED bar that lit up on the day of bin collection to the colour of the bin you want to take out, then this repo provides the data for that. \n\n**PLEASE respect a councils infrastructure / usage policy and only collect data for your own personal use on a sutable frequency to your collection schedule.**\n\nMost scripts make use of [Beautiful Soup 4](https://pypi.org/project/beautifulsoup4/) to scrape data, although others use different approaches, such as emulating web browser behaviour, or reading data from CSV files.\n\n[![](https://img.shields.io/badge/--41BDF5?logo=homeassistant&logoColor=white&label=HomeAssistant+Thread)](https://community.home-assistant.io/t/bin-waste-collection/55451) [![](https://img.shields.io/badge/--181717?logo=github&logoColor=white&label=Request+a+council)](https://github.com/robbrad/UKBinCollectionData/issues/new/choose)\n\n---\n\n## Usage\n```commandline\nPS G:\\Projects\\Python\\UKBinCollectionData\\uk_bin_collection\\collect_data.py\nusage: collect_data.py [-h] [-p POSTCODE] [-n NUMBER] [-u UPRN] module URL\n\npositional arguments:\n  module                Name of council module to use                           (required)\n  URL                   URL to parse                                            (required)\n\noptions:\n  -h, --help                            show this help message                  (optional)\n  -p POSTCODE, --postcode POSTCODE      Postcode to parse - should include      (optional)\n                                        a space and be wrapped in double\n                                        quotes                                  \n  -n NUMBER, --number NUMBER            House number to parse                   (optional)\n  -u UPRN, --uprn UPRN                  UPRN to parse                           (optional)\n```\n\n\n### Quickstart\nThe basic command to execute a script is:\n```commandline\npython collect_data.py <council_name> "<collection_url>"\n```\nwhere ```council_name``` is the name of the council\'s .py script (without the .py) and ```collection_url``` is the URL to scrape.\nThe help documentation refers to these as "module" and "URL", respectively. Supported council scripts can be found in the `uk_bin_collection/uk_bin_collection/councils` folder.\n\nSome scripts require additional parameters, for example, when a UPRN is not passed in a URL, or when the script is not scraping a web page.\nFor example, the Leeds City Council script needs two additional parameters - a postcode, and a house number. This is done like so:\n\n```commandline\npython collect_data.py LeedsCityCouncil https://www.leeds.gov.uk/residents/bins-and-recycling/check-your-bin-day -p "LS1 2JG" -n 41\n```\n- A **postcode** can be passed with `-p "postcode"` or `--postcode "postcode"`. The postcode must always include a space in the middle and\nbe wrapped in double quotes (due to how command line arguments are handled).\n- A **house number** can be passed with `-n number` or `--number number`.\n- A **UPRN reference** can be passed with `-u uprn` or `--uprn uprn`.\n\nTo check the parameters needed for your council\'s script, please check the [project wiki](https://github.com/robbrad/UKBinCollectionData/wiki) for more information.\n\n\n### Project dependencies\nSome scripts rely on external packages to function. A list of required scripts for both development and execution can be found in the project\'s [PROJECT_TOML](https://github.com/robbrad/UKBinCollectionData/blob/feature/%2353_integration_tests/pyproject.toml) \nInstall can be done via \n`poetry install` from within the root of the repo.\n\n\n### UPRN Finder\nSome councils make use of the UPRN (Unique property reference number) to identify your property. You can find yours [here](https://www.findmyaddress.co.uk/search) or [here](https://uprn.uk/).\n\n## Requesting your council\nTo make a request for your council, first check the [Issues](https://github.com/robbrad/UKBinCollectionData/issues) page to make sure it has not already been requested. If not, please fill in a new [Council Request](https://github.com/robbrad/UKBinCollectionData/issues/new/choose) form, including as much information as possible, including:\n- Name of the council\n- URL to bin collections\n- An example postcode and/or UPRN (whichever is relevant)\n- Any further information\n\nPlease be aware that this project is run by volunteer contributors and completion depends on numerous factors - even with a request, we cannot guarantee if/when your council will get a script.\n\n---\n\n## Reports\n\n- [3.9](https://robbrad.github.io/UKBinCollectionData/3.9/)\n- [3.8](https://robbrad.github.io/UKBinCollectionData/3.8/)\n\n---\n\n## FAQ\n#### I\'ve got an issue/support question - what do I do?\nPlease post in the [HomeAssistant thread](https://community.home-assistant.io/t/bin-waste-collection/55451) or raise a new (non council request) [issue](https://github.com/robbrad/UKBinCollectionData/issues/new).\n\n#### I\'d like to contribute, where do I start?\nContributions are always welcome! See ```CONTRIBUTING.md``` to get started. Please adhere to the project\'s [code of conduct](https://github.com/robbrad/UKBinCollectionData/blob/master/CODE_OF_CONDUCT.md).\n\n- If you\'re new to coding/Python/BeautifulSoup, feel free to check [here](https://github.com/robbrad/UKBinCollectionData/issues?q=is%3Aissue+is%3Aopen+label%3A%22good+first+issue%22) for issues that are good for newcomers!\n- If you would like to try writing your own scraper, feel free to fork this project and use existing scrapers as a base for your approach (or `councilclasstemplate.py`).\n\n## Contributors\n<a href="https://github.com/robbrad/UKBinCollectionData/graphs/contributors">\n  <img src="https://contrib.rocks/image?repo=robbrad/UKBinCollectionData"  alt="Image of contributors"/>\n</a>\n\n',
-    'author': 'Robert Bradley',
-    'author_email': 'robbrad182@gmail.com',
-    'maintainer': 'None',
-    'maintainer_email': 'None',
-    'url': 'None',
-    'package_dir': package_dir,
-    'packages': packages,
-    'package_data': package_data,
-    'install_requires': install_requires,
-    'entry_points': entry_points,
-    'python_requires': '>=3.8,<4',
-}
+![GitHub](https://img.shields.io/github/license/robbrad/UKBinCollectionData?style=for-the-badge) ![GitHub issues](https://img.shields.io/github/issues-raw/robbrad/UKBinCollectionData?style=for-the-badge) ![GitHub closed issues](https://img.shields.io/github/issues-closed-raw/robbrad/UKBinCollectionData?style=for-the-badge)
+![GitHub contributors](https://img.shields.io/github/contributors/robbrad/UKBinCollectionData?style=for-the-badge)
+
+![GitHub Workflow Status](https://img.shields.io/github/actions/workflow/status/robbrad/UKBinCollectionData/behave.yml?style=for-the-badge)
+![Codecov](https://img.shields.io/codecov/c/gh/robbrad/UKBinCollectionData?style=for-the-badge)
+
+[![pages-build-deployment](https://github.com/robbrad/UKBinCollectionData/actions/workflows/pages/pages-build-deployment/badge.svg)](https://github.com/robbrad/UKBinCollectionData/actions/workflows/pages/pages-build-deployment) [![Test Councils](https://github.com/robbrad/UKBinCollectionData/actions/workflows/behave.yml/badge.svg)](https://github.com/robbrad/UKBinCollectionData/actions/workflows/behave.yml)
+
+# UK Bin Collection Data (UKBCD)
+This project aims to provide a neat and standard way of providing bin collection data in JSON format from UK councils that have no API to do so.
+
+Why do this?
+You might want to use this in a Home Automation - for example say you had an LED bar that lit up on the day of bin collection to the colour of the bin you want to take out, then this repo provides the data for that. 
+
+**PLEASE respect a councils infrastructure / usage policy and only collect data for your own personal use on a sutable frequency to your collection schedule.**
+
+Most scripts make use of [Beautiful Soup 4](https://pypi.org/project/beautifulsoup4/) to scrape data, although others use different approaches, such as emulating web browser behaviour, or reading data from CSV files.
+
+[![](https://img.shields.io/badge/--41BDF5?logo=homeassistant&logoColor=white&label=HomeAssistant+Thread)](https://community.home-assistant.io/t/bin-waste-collection/55451) [![](https://img.shields.io/badge/--181717?logo=github&logoColor=white&label=Request+a+council)](https://github.com/robbrad/UKBinCollectionData/issues/new/choose)
+
+---
+
+## Usage
+```commandline
+PS G:\Projects\Python\UKBinCollectionData\uk_bin_collection\collect_data.py
+usage: collect_data.py [-h] [-p POSTCODE] [-n NUMBER] [-u UPRN] module URL
+
+positional arguments:
+  module                Name of council module to use                           (required)
+  URL                   URL to parse                                            (required)
+
+options:
+  -h, --help                            show this help message                  (optional)
+  -p POSTCODE, --postcode POSTCODE      Postcode to parse - should include      (optional)
+                                        a space and be wrapped in double
+                                        quotes                                  
+  -n NUMBER, --number NUMBER            House number to parse                   (optional)
+  -u UPRN, --uprn UPRN                  UPRN to parse                           (optional)
+```
+
+
+### Quickstart
+The basic command to execute a script is:
+```commandline
+python collect_data.py <council_name> "<collection_url>"
+```
+where ```council_name``` is the name of the council's .py script (without the .py) and ```collection_url``` is the URL to scrape.
+The help documentation refers to these as "module" and "URL", respectively. Supported council scripts can be found in the `uk_bin_collection/uk_bin_collection/councils` folder.
+
+Some scripts require additional parameters, for example, when a UPRN is not passed in a URL, or when the script is not scraping a web page.
+For example, the Leeds City Council script needs two additional parameters - a postcode, and a house number. This is done like so:
+
+```commandline
+python collect_data.py LeedsCityCouncil https://www.leeds.gov.uk/residents/bins-and-recycling/check-your-bin-day -p "LS1 2JG" -n 41
+```
+- A **postcode** can be passed with `-p "postcode"` or `--postcode "postcode"`. The postcode must always include a space in the middle and
+be wrapped in double quotes (due to how command line arguments are handled).
+- A **house number** can be passed with `-n number` or `--number number`.
+- A **UPRN reference** can be passed with `-u uprn` or `--uprn uprn`.
+
+To check the parameters needed for your council's script, please check the [project wiki](https://github.com/robbrad/UKBinCollectionData/wiki) for more information.
+
+
+### Project dependencies
+Some scripts rely on external packages to function. A list of required scripts for both development and execution can be found in the project's [PROJECT_TOML](https://github.com/robbrad/UKBinCollectionData/blob/feature/%2353_integration_tests/pyproject.toml) 
+Install can be done via 
+`poetry install` from within the root of the repo.
+
+
+### UPRN Finder
+Some councils make use of the UPRN (Unique property reference number) to identify your property. You can find yours [here](https://www.findmyaddress.co.uk/search) or [here](https://uprn.uk/).
+
+## Requesting your council
+To make a request for your council, first check the [Issues](https://github.com/robbrad/UKBinCollectionData/issues) page to make sure it has not already been requested. If not, please fill in a new [Council Request](https://github.com/robbrad/UKBinCollectionData/issues/new/choose) form, including as much information as possible, including:
+- Name of the council
+- URL to bin collections
+- An example postcode and/or UPRN (whichever is relevant)
+- Any further information
+
+Please be aware that this project is run by volunteer contributors and completion depends on numerous factors - even with a request, we cannot guarantee if/when your council will get a script.
+
+---
+
+## Reports
+
+- [3.10](https://robbrad.github.io/UKBinCollectionData/3.10/)
+- [3.11](https://robbrad.github.io/UKBinCollectionData/3.11/)
+
+---
+
+## FAQ
+#### I've got an issue/support question - what do I do?
+Please post in the [HomeAssistant thread](https://community.home-assistant.io/t/bin-waste-collection/55451) or raise a new (non council request) [issue](https://github.com/robbrad/UKBinCollectionData/issues/new).
+
+#### I'd like to contribute, where do I start?
+Contributions are always welcome! See ```CONTRIBUTING.md``` to get started. Please adhere to the project's [code of conduct](https://github.com/robbrad/UKBinCollectionData/blob/master/CODE_OF_CONDUCT.md).
+
+- If you're new to coding/Python/BeautifulSoup, feel free to check [here](https://github.com/robbrad/UKBinCollectionData/issues?q=is%3Aissue+is%3Aopen+label%3A%22good+first+issue%22) for issues that are good for newcomers!
+- If you would like to try writing your own scraper, feel free to fork this project and use existing scrapers as a base for your approach (or `councilclasstemplate.py`).
+
+## Contributors
+<a href="https://github.com/robbrad/UKBinCollectionData/graphs/contributors">
+  <img src="https://contrib.rocks/image?repo=robbrad/UKBinCollectionData"  alt="Image of contributors"/>
+</a>
 
 
-setup(**setup_kwargs)
```

