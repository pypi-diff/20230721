# Comparing `tmp/pyaedt-0.6.85.tar.gz` & `tmp/pyaedt-0.6.86.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "pyaedt-0.6.85.tar", last modified: Fri Jan  1 00:00:00 2016, max compression
+gzip compressed data, was "pyaedt-0.6.86.tar", last modified: Fri Jan  1 00:00:00 2016, max compression
```

## Comparing `pyaedt-0.6.85.tar` & `pyaedt-0.6.86.tar`

### file list

```diff
@@ -1,258 +1,259 @@
--rw-r--r--   0        0        0     1111 2023-05-18 13:27:42.185924 pyaedt-0.6.85/LICENSE
--rw-r--r--   0        0        0     9947 2023-05-18 13:27:42.185924 pyaedt-0.6.85/README.md
--rw-r--r--   0        0        0     2691 2023-07-14 12:25:57.045581 pyaedt-0.6.85/pyaedt/__init__.py
--rw-r--r--   0        0        0    26756 2023-07-06 12:41:13.683251 pyaedt-0.6.85/pyaedt/aedt_logger.py
--rw-r--r--   0        0        0     6965 2023-05-18 13:27:43.889057 pyaedt-0.6.85/pyaedt/application/AEDT_File_Management.py
--rw-r--r--   0        0        0    88917 2023-07-05 10:16:58.951877 pyaedt-0.6.85/pyaedt/application/Analysis.py
--rw-r--r--   0        0        0    50696 2023-07-11 09:19:45.814204 pyaedt-0.6.85/pyaedt/application/Analysis3D.py
--rw-r--r--   0        0        0    17066 2023-05-29 06:50:01.462409 pyaedt-0.6.85/pyaedt/application/Analysis3DLayout.py
--rw-r--r--   0        0        0     3088 2023-05-18 13:27:43.889057 pyaedt-0.6.85/pyaedt/application/AnalysisMaxwellCircuit.py
--rw-r--r--   0        0        0    19857 2023-07-13 12:17:05.981892 pyaedt-0.6.85/pyaedt/application/AnalysisNexxim.py
--rw-r--r--   0        0        0     4431 2023-05-29 06:50:01.462409 pyaedt-0.6.85/pyaedt/application/AnalysisRMxprt.py
--rw-r--r--   0        0        0     4596 2023-05-29 06:50:01.477983 pyaedt-0.6.85/pyaedt/application/AnalysisTwinBuilder.py
--rw-r--r--   0        0        0   135985 2023-07-11 09:19:45.814204 pyaedt-0.6.85/pyaedt/application/Design.py
--rw-r--r--   0        0        0     6115 2023-05-18 13:27:43.889057 pyaedt-0.6.85/pyaedt/application/JobManager.py
--rw-r--r--   0        0        0    75595 2023-07-11 09:19:45.814204 pyaedt-0.6.85/pyaedt/application/Variables.py
--rw-r--r--   0        0        0        0 2023-05-18 13:27:43.889057 pyaedt-0.6.85/pyaedt/application/__init__.py
--rw-r--r--   0        0        0    12464 2023-05-29 06:50:01.477983 pyaedt-0.6.85/pyaedt/application/aedt_objects.py
--rw-r--r--   0        0        0    36750 2023-06-29 10:10:15.395808 pyaedt-0.6.85/pyaedt/application/design_solutions.py
--rw-r--r--   0        0        0    62949 2023-07-12 14:57:59.361294 pyaedt-0.6.85/pyaedt/circuit.py
--rw-r--r--   0        0        0    10247 2023-06-05 09:37:00.357207 pyaedt-0.6.85/pyaedt/common_rpc.py
--rw-r--r--   0        0        0    84902 2023-07-14 12:25:57.045581 pyaedt-0.6.85/pyaedt/desktop.py
--rw-r--r--   0        0        0    15104 2023-05-18 13:27:43.904685 pyaedt-0.6.85/pyaedt/dlls/PDFReport/AnsysReport.deps.json
--rw-r--r--   0        0        0    23552 2023-05-18 13:27:43.904685 pyaedt-0.6.85/pyaedt/dlls/PDFReport/AnsysReport.dll
--rw-r--r--   0        0        0     1086 2023-06-29 10:10:15.395808 pyaedt-0.6.85/pyaedt/dlls/PDFReport/AnsysTemplate.json
--rw-r--r--   0        0        0   204800 2023-05-18 13:27:43.904685 pyaedt-0.6.85/pyaedt/dlls/PDFReport/ICSharpCode.SharpZipLib.dll
--rw-r--r--   0        0        0   577445 2023-05-18 13:27:43.904685 pyaedt-0.6.85/pyaedt/dlls/PDFReport/ICSharpCode.SharpZipLib.xml
--rw-r--r--   0        0        0     9836 2023-05-18 13:27:43.904685 pyaedt-0.6.85/pyaedt/dlls/PDFReport/Images/Ansys.png
--rw-r--r--   0        0        0   238592 2023-05-18 13:27:43.904685 pyaedt-0.6.85/pyaedt/dlls/PDFReport/MigraDocCore.DocumentObjectModel.dll
--rw-r--r--   0        0        0   115712 2023-05-18 13:27:43.904685 pyaedt-0.6.85/pyaedt/dlls/PDFReport/MigraDocCore.Rendering.dll
--rw-r--r--   0        0        0   705296 2023-05-18 13:27:43.920373 pyaedt-0.6.85/pyaedt/dlls/PDFReport/Newtonsoft.Json.dll
--rw-r--r--   0        0        0   712253 2023-05-18 13:27:43.920373 pyaedt-0.6.85/pyaedt/dlls/PDFReport/Newtonsoft.Json.xml
--rw-r--r--   0        0        0    80384 2023-05-18 13:27:43.920373 pyaedt-0.6.85/pyaedt/dlls/PDFReport/PdfSharpCore.Charting.dll
--rw-r--r--   0        0        0   546816 2023-05-18 13:27:43.935986 pyaedt-0.6.85/pyaedt/dlls/PDFReport/PdfSharpCore.dll
--rw-r--r--   0        0        0   367616 2023-05-18 13:27:43.935986 pyaedt-0.6.85/pyaedt/dlls/PDFReport/SixLabors.Fonts.dll
--rw-r--r--   0        0        0   536367 2023-05-18 13:27:43.935986 pyaedt-0.6.85/pyaedt/dlls/PDFReport/SixLabors.Fonts.xml
--rw-r--r--   0        0        0  1229824 2023-05-18 13:27:43.951639 pyaedt-0.6.85/pyaedt/dlls/PDFReport/SixLabors.ImageSharp.dll
--rw-r--r--   0        0        0  3285773 2023-05-18 13:27:43.967239 pyaedt-0.6.85/pyaedt/dlls/PDFReport/SixLabors.ImageSharp.xml
--rw-r--r--   0        0        0   120664 2023-05-18 13:27:43.967239 pyaedt-0.6.85/pyaedt/dlls/PDFReport/System.Runtime.dll
--rw-r--r--   0        0        0  1505294 2023-05-18 13:27:43.982863 pyaedt-0.6.85/pyaedt/dlls/PDFReport/System.Runtime.xml
--rw-r--r--   0        0        0     5632 2023-05-18 13:27:43.982863 pyaedt-0.6.85/pyaedt/dlls/PDFReport/de/PdfSharpCore.resources.dll
--rw-r--r--   0        0        0   160754 2023-05-18 13:27:43.982863 pyaedt-0.6.85/pyaedt/dlls/PDFReport/de/System.Collections.NonGeneric.xml
--rw-r--r--   0        0        0    24039 2023-07-14 08:27:52.560421 pyaedt-0.6.85/pyaedt/downloads.py
--rw-r--r--   0        0        0   137623 2023-06-29 16:42:04.115357 pyaedt-0.6.85/pyaedt/edb.py
--rw-r--r--   0        0        0      333 2023-05-18 13:27:43.982863 pyaedt-0.6.85/pyaedt/edb_core/__init__.py
--rw-r--r--   0        0        0    98675 2023-07-12 14:57:59.361294 pyaedt-0.6.85/pyaedt/edb_core/components.py
--rw-r--r--   0        0        0        0 2023-06-05 09:10:35.931330 pyaedt-0.6.85/pyaedt/edb_core/dotnet/__init__.py
--rw-r--r--   0        0        0    31497 2023-06-05 09:10:35.931330 pyaedt-0.6.85/pyaedt/edb_core/dotnet/database.py
--rw-r--r--   0        0        0     7909 2023-06-05 09:10:35.931330 pyaedt-0.6.85/pyaedt/edb_core/dotnet/layout.py
--rw-r--r--   0        0        0    48210 2023-06-05 09:10:35.931330 pyaedt-0.6.85/pyaedt/edb_core/dotnet/primitive.py
--rw-r--r--   0        0        0        0 2023-05-18 13:27:43.982863 pyaedt-0.6.85/pyaedt/edb_core/edb_data/__init__.py
--rw-r--r--   0        0        0    33195 2023-06-12 08:03:15.118737 pyaedt-0.6.85/pyaedt/edb_core/edb_data/components_data.py
--rw-r--r--   0        0        0    40100 2023-05-29 06:50:01.477983 pyaedt-0.6.85/pyaedt/edb_core/edb_data/control_file.py
--rw-r--r--   0        0        0      937 2023-05-18 13:27:43.982863 pyaedt-0.6.85/pyaedt/edb_core/edb_data/design_options.py
--rw-r--r--   0        0        0      867 2023-05-26 06:18:30.544561 pyaedt-0.6.85/pyaedt/edb_core/edb_data/edbvalue.py
--rw-r--r--   0        0        0    12243 2023-06-05 09:10:35.931330 pyaedt-0.6.85/pyaedt/edb_core/edb_data/hfss_extent_info.py
--rw-r--r--   0        0        0    65661 2023-06-05 09:10:35.931330 pyaedt-0.6.85/pyaedt/edb_core/edb_data/hfss_simulation_setup_data.py
--rw-r--r--   0        0        0    20386 2023-06-05 09:10:35.931330 pyaedt-0.6.85/pyaedt/edb_core/edb_data/layer_data.py
--rw-r--r--   0        0        0     6880 2023-07-14 09:29:55.878674 pyaedt-0.6.85/pyaedt/edb_core/edb_data/nets_data.py
--rw-r--r--   0        0        0    61171 2023-06-05 09:10:35.931330 pyaedt-0.6.85/pyaedt/edb_core/edb_data/padstacks_data.py
--rw-r--r--   0        0        0    32590 2023-06-29 17:19:42.860399 pyaedt-0.6.85/pyaedt/edb_core/edb_data/primitives_data.py
--rw-r--r--   0        0        0   102298 2023-06-14 08:55:18.804330 pyaedt-0.6.85/pyaedt/edb_core/edb_data/simulation_configuration.py
--rw-r--r--   0        0        0    36324 2023-06-05 09:10:35.931330 pyaedt-0.6.85/pyaedt/edb_core/edb_data/siwave_simulation_setup_data.py
--rw-r--r--   0        0        0    34944 2023-07-07 09:29:33.858435 pyaedt-0.6.85/pyaedt/edb_core/edb_data/sources.py
--rw-r--r--   0        0        0     3923 2023-06-05 14:55:02.766448 pyaedt-0.6.85/pyaedt/edb_core/edb_data/utilities.py
--rw-r--r--   0        0        0     2432 2023-06-05 09:10:35.931330 pyaedt-0.6.85/pyaedt/edb_core/edb_data/variables.py
--rw-r--r--   0        0        0     3258 2023-05-18 13:27:43.998437 pyaedt-0.6.85/pyaedt/edb_core/general.py
--rw-r--r--   0        0        0    68725 2023-06-29 10:33:27.694259 pyaedt-0.6.85/pyaedt/edb_core/hfss.py
--rw-r--r--   0        0        0        0 2023-05-18 13:27:43.998437 pyaedt-0.6.85/pyaedt/edb_core/ipc2581/__init__.py
--rw-r--r--   0        0        0        0 2023-05-18 13:27:43.998437 pyaedt-0.6.85/pyaedt/edb_core/ipc2581/bom/__init__.py
--rw-r--r--   0        0        0      673 2023-05-18 13:27:43.998437 pyaedt-0.6.85/pyaedt/edb_core/ipc2581/bom/bom.py
--rw-r--r--   0        0        0     1283 2023-05-18 13:27:43.998437 pyaedt-0.6.85/pyaedt/edb_core/ipc2581/bom/bom_item.py
--rw-r--r--   0        0        0     2213 2023-05-18 13:27:43.998437 pyaedt-0.6.85/pyaedt/edb_core/ipc2581/bom/characteristics.py
--rw-r--r--   0        0        0      524 2023-05-18 13:27:43.998437 pyaedt-0.6.85/pyaedt/edb_core/ipc2581/bom/refdes.py
--rw-r--r--   0        0        0        0 2023-05-18 13:27:43.998437 pyaedt-0.6.85/pyaedt/edb_core/ipc2581/content/__init__.py
--rw-r--r--   0        0        0      768 2023-05-18 13:27:43.998437 pyaedt-0.6.85/pyaedt/edb_core/ipc2581/content/color.py
--rw-r--r--   0        0        0     2118 2023-05-18 13:27:43.998437 pyaedt-0.6.85/pyaedt/edb_core/ipc2581/content/content.py
--rw-r--r--   0        0        0      938 2023-05-18 13:27:43.998437 pyaedt-0.6.85/pyaedt/edb_core/ipc2581/content/dictionary_color.py
--rw-r--r--   0        0        0      921 2023-05-18 13:27:43.998437 pyaedt-0.6.85/pyaedt/edb_core/ipc2581/content/dictionary_fill.py
--rw-r--r--   0        0        0     1029 2023-05-18 13:27:43.998437 pyaedt-0.6.85/pyaedt/edb_core/ipc2581/content/dictionary_line.py
--rw-r--r--   0        0        0      416 2023-05-18 13:27:43.998437 pyaedt-0.6.85/pyaedt/edb_core/ipc2581/content/entry_color.py
--rw-r--r--   0        0        0      548 2023-05-18 13:27:43.998437 pyaedt-0.6.85/pyaedt/edb_core/ipc2581/content/entry_line.py
--rw-r--r--   0        0        0      523 2023-05-18 13:27:43.998437 pyaedt-0.6.85/pyaedt/edb_core/ipc2581/content/fill.py
--rw-r--r--   0        0        0      284 2023-05-18 13:27:43.998437 pyaedt-0.6.85/pyaedt/edb_core/ipc2581/content/layer_ref.py
--rw-r--r--   0        0        0     2850 2023-06-05 09:10:35.946956 pyaedt-0.6.85/pyaedt/edb_core/ipc2581/content/standard_geometries_dictionary.py
--rw-r--r--   0        0        0        0 2023-05-18 13:27:43.998437 pyaedt-0.6.85/pyaedt/edb_core/ipc2581/ecad/__init__.py
--rw-r--r--   0        0        0        0 2023-05-18 13:27:43.998437 pyaedt-0.6.85/pyaedt/edb_core/ipc2581/ecad/cad_data/__init__.py
--rw-r--r--   0        0        0     1183 2023-05-18 13:27:43.998437 pyaedt-0.6.85/pyaedt/edb_core/ipc2581/ecad/cad_data/assembly_drawing.py
--rw-r--r--   0        0        0     1319 2023-05-18 13:27:44.014060 pyaedt-0.6.85/pyaedt/edb_core/ipc2581/ecad/cad_data/cad_data.py
--rw-r--r--   0        0        0     1516 2023-05-18 13:27:44.014060 pyaedt-0.6.85/pyaedt/edb_core/ipc2581/ecad/cad_data/component.py
--rw-r--r--   0        0        0      960 2023-05-18 13:27:44.014060 pyaedt-0.6.85/pyaedt/edb_core/ipc2581/ecad/cad_data/drill.py
--rw-r--r--   0        0        0     1964 2023-05-18 13:27:44.014060 pyaedt-0.6.85/pyaedt/edb_core/ipc2581/ecad/cad_data/feature.py
--rw-r--r--   0        0        0     1158 2023-05-18 13:27:44.014060 pyaedt-0.6.85/pyaedt/edb_core/ipc2581/ecad/cad_data/layer.py
--rw-r--r--   0        0        0     7763 2023-05-29 06:50:01.493602 pyaedt-0.6.85/pyaedt/edb_core/ipc2581/ecad/cad_data/layer_feature.py
--rw-r--r--   0        0        0      921 2023-05-18 13:27:44.014060 pyaedt-0.6.85/pyaedt/edb_core/ipc2581/ecad/cad_data/logical_net.py
--rw-r--r--   0        0        0     1079 2023-05-18 13:27:44.014060 pyaedt-0.6.85/pyaedt/edb_core/ipc2581/ecad/cad_data/outline.py
--rw-r--r--   0        0        0     4703 2023-05-29 06:50:01.493602 pyaedt-0.6.85/pyaedt/edb_core/ipc2581/ecad/cad_data/package.py
--rw-r--r--   0        0        0     1440 2023-05-18 13:27:44.014060 pyaedt-0.6.85/pyaedt/edb_core/ipc2581/ecad/cad_data/padstack_def.py
--rw-r--r--   0        0        0      875 2023-05-18 13:27:44.014060 pyaedt-0.6.85/pyaedt/edb_core/ipc2581/ecad/cad_data/padstack_hole_def.py
--rw-r--r--   0        0        0     2775 2023-05-18 13:27:44.014060 pyaedt-0.6.85/pyaedt/edb_core/ipc2581/ecad/cad_data/padstack_instance.py
--rw-r--r--   0        0        0      887 2023-05-18 13:27:44.014060 pyaedt-0.6.85/pyaedt/edb_core/ipc2581/ecad/cad_data/padstack_pad_def.py
--rw-r--r--   0        0        0     4104 2023-05-18 13:27:44.014060 pyaedt-0.6.85/pyaedt/edb_core/ipc2581/ecad/cad_data/path.py
--rw-r--r--   0        0        0     2567 2023-05-18 13:27:44.014060 pyaedt-0.6.85/pyaedt/edb_core/ipc2581/ecad/cad_data/phy_net.py
--rw-r--r--   0        0        0     1002 2023-05-18 13:27:44.014060 pyaedt-0.6.85/pyaedt/edb_core/ipc2581/ecad/cad_data/pin.py
--rw-r--r--   0        0        0     8010 2023-05-18 13:27:44.014060 pyaedt-0.6.85/pyaedt/edb_core/ipc2581/ecad/cad_data/polygon.py
--rw-r--r--   0        0        0      663 2023-05-18 13:27:44.014060 pyaedt-0.6.85/pyaedt/edb_core/ipc2581/ecad/cad_data/profile.py
--rw-r--r--   0        0        0     1162 2023-05-18 13:27:44.014060 pyaedt-0.6.85/pyaedt/edb_core/ipc2581/ecad/cad_data/stackup.py
--rw-r--r--   0        0        0     1626 2023-05-18 13:27:44.014060 pyaedt-0.6.85/pyaedt/edb_core/ipc2581/ecad/cad_data/stackup_group.py
--rw-r--r--   0        0        0      838 2023-05-18 13:27:44.014060 pyaedt-0.6.85/pyaedt/edb_core/ipc2581/ecad/cad_data/stackup_layer.py
--rw-r--r--   0        0        0    11390 2023-05-29 06:50:01.493602 pyaedt-0.6.85/pyaedt/edb_core/ipc2581/ecad/cad_data/step.py
--rw-r--r--   0        0        0     1033 2023-05-18 13:27:44.014060 pyaedt-0.6.85/pyaedt/edb_core/ipc2581/ecad/cad_header.py
--rw-r--r--   0        0        0      683 2023-05-18 13:27:44.014060 pyaedt-0.6.85/pyaedt/edb_core/ipc2581/ecad/ecad.py
--rw-r--r--   0        0        0     2008 2023-05-18 13:27:44.014060 pyaedt-0.6.85/pyaedt/edb_core/ipc2581/ecad/spec.py
--rw-r--r--   0        0        0     1624 2023-05-18 13:27:44.014060 pyaedt-0.6.85/pyaedt/edb_core/ipc2581/history_record.py
--rw-r--r--   0        0        0    21800 2023-06-05 09:10:35.946956 pyaedt-0.6.85/pyaedt/edb_core/ipc2581/ipc2581.py
--rw-r--r--   0        0        0      966 2023-05-18 13:27:44.014060 pyaedt-0.6.85/pyaedt/edb_core/ipc2581/logistic_header.py
--rw-r--r--   0        0        0    47176 2023-06-22 08:12:52.117360 pyaedt-0.6.85/pyaedt/edb_core/layout.py
--rw-r--r--   0        0        0    33310 2023-06-05 09:10:35.946956 pyaedt-0.6.85/pyaedt/edb_core/materials.py
--rw-r--r--   0        0        0    44030 2023-06-05 14:55:02.766448 pyaedt-0.6.85/pyaedt/edb_core/nets.py
--rw-r--r--   0        0        0    49394 2023-07-07 09:29:33.858435 pyaedt-0.6.85/pyaedt/edb_core/padstack.py
--rw-r--r--   0        0        0    58809 2023-06-19 09:51:41.631657 pyaedt-0.6.85/pyaedt/edb_core/siwave.py
--rw-r--r--   0        0        0   109207 2023-06-05 09:10:35.946956 pyaedt-0.6.85/pyaedt/edb_core/stackup.py
--rw-r--r--   0        0        0    11500 2023-07-05 14:41:01.487654 pyaedt-0.6.85/pyaedt/emit.py
--rw-r--r--   0        0        0     6100 2023-07-05 14:41:01.487654 pyaedt-0.6.85/pyaedt/emit_core/Couplings.py
--rw-r--r--   0        0        0     2813 2023-06-14 05:38:07.853286 pyaedt-0.6.85/pyaedt/emit_core/__init__.py
--rw-r--r--   0        0        0     1621 2023-06-14 05:38:07.853286 pyaedt-0.6.85/pyaedt/emit_core/emit_constants.py
--rw-r--r--   0        0        0        2 2023-05-18 13:27:44.029696 pyaedt-0.6.85/pyaedt/emit_core/results/__init__.py
--rw-r--r--   0        0        0     7406 2023-07-05 14:41:01.487654 pyaedt-0.6.85/pyaedt/emit_core/results/results.py
--rw-r--r--   0        0        0    13896 2023-07-05 14:41:01.503279 pyaedt-0.6.85/pyaedt/emit_core/results/revision.py
--rw-r--r--   0        0        0    14317 2023-05-18 13:27:44.029696 pyaedt-0.6.85/pyaedt/generic/DataHandlers.py
--rw-r--r--   0        0        0    12252 2023-06-21 10:09:54.048412 pyaedt-0.6.85/pyaedt/generic/LoadAEDTFile.py
--rw-r--r--   0        0        0        0 2023-05-18 13:27:44.029696 pyaedt-0.6.85/pyaedt/generic/__init__.py
--rw-r--r--   0        0        0     3257 2023-05-26 11:30:35.579837 pyaedt-0.6.85/pyaedt/generic/clr_module.py
--rw-r--r--   0        0        0    83444 2023-05-29 06:50:01.509226 pyaedt-0.6.85/pyaedt/generic/configurations.py
--rw-r--r--   0        0        0    28645 2023-05-18 13:27:44.029696 pyaedt-0.6.85/pyaedt/generic/constants.py
--rw-r--r--   0        0        0    21891 2023-05-26 06:18:30.560187 pyaedt-0.6.85/pyaedt/generic/design_types.py
--rw-r--r--   0        0        0     3442 2023-07-12 15:53:29.956835 pyaedt-0.6.85/pyaedt/generic/filesystem.py
--rw-r--r--   0        0        0    70821 2023-07-14 12:25:57.045581 pyaedt-0.6.85/pyaedt/generic/general_methods.py
--rw-r--r--   0        0        0     9417 2023-07-13 12:17:05.981892 pyaedt-0.6.85/pyaedt/generic/grpc_plugin.py
--rw-r--r--   0        0        0     3043 2023-07-11 09:19:45.814204 pyaedt-0.6.85/pyaedt/generic/grpc_plugin_dll.py
--rw-r--r--   0        0        0    25808 2023-05-18 13:27:44.029696 pyaedt-0.6.85/pyaedt/generic/ibis_reader.py
--rw-r--r--   0        0        0     7029 2023-07-12 14:57:59.361294 pyaedt-0.6.85/pyaedt/generic/near_field_import.py
--rw-r--r--   0        0        0     9795 2023-05-18 13:27:44.029696 pyaedt-0.6.85/pyaedt/generic/pdf.py
--rw-r--r--   0        0        0    62327 2023-05-29 06:50:01.509226 pyaedt-0.6.85/pyaedt/generic/plot.py
--rw-r--r--   0        0        0    11405 2023-06-22 08:12:52.117360 pyaedt-0.6.85/pyaedt/generic/process.py
--rw-r--r--   0        0        0    20326 2023-05-18 13:27:44.045311 pyaedt-0.6.85/pyaedt/generic/python_optimizers.py
--rw-r--r--   0        0        0     3536 2023-06-21 10:09:54.048412 pyaedt-0.6.85/pyaedt/generic/report_file_parser.py
--rw-r--r--   0        0        0    60412 2023-05-29 06:50:01.509226 pyaedt-0.6.85/pyaedt/generic/toolkit.py
--rw-r--r--   0        0        0    17095 2023-05-18 13:27:44.045311 pyaedt-0.6.85/pyaedt/generic/touchstone_parser.py
--rw-r--r--   0        0        0      438 2023-05-18 13:27:44.045311 pyaedt-0.6.85/pyaedt/generic/wpf_template.xaml
--rw-r--r--   0        0        0   255506 2023-07-13 12:17:05.981892 pyaedt-0.6.85/pyaedt/hfss.py
--rw-r--r--   0        0        0    84753 2023-07-06 12:04:15.245225 pyaedt-0.6.85/pyaedt/hfss3dlayout.py
--rw-r--r--   0        0        0   200124 2023-07-14 08:52:47.315413 pyaedt-0.6.85/pyaedt/icepak.py
--rw-r--r--   0        0        0   127831 2023-07-13 12:17:05.981892 pyaedt-0.6.85/pyaedt/maxwell.py
--rw-r--r--   0        0        0     7803 2023-05-18 13:27:44.045311 pyaedt-0.6.85/pyaedt/maxwellcircuit.py
--rw-r--r--   0        0        0    24372 2023-07-06 12:04:15.245225 pyaedt-0.6.85/pyaedt/mechanical.py
--rw-r--r--   0        0        0     3642 2023-05-18 13:27:44.045311 pyaedt-0.6.85/pyaedt/misc/Console.py_build
--rw-r--r--   0        0        0     2230 2023-05-18 13:27:44.045311 pyaedt-0.6.85/pyaedt/misc/Job_Settings.areg
--rw-r--r--   0        0        0     3035 2023-05-18 13:27:44.045311 pyaedt-0.6.85/pyaedt/misc/Jupyter.py_build
--rw-r--r--   0        0        0     3972 2023-07-07 09:29:33.874017 pyaedt-0.6.85/pyaedt/misc/Run_PyAEDT_Script.py_build
--rw-r--r--   0        0        0     3311 2023-07-07 09:29:33.874017 pyaedt-0.6.85/pyaedt/misc/Run_PyAEDT_Toolkit_Script.py_build
--rw-r--r--   0        0        0       53 2023-05-18 13:27:44.045311 pyaedt-0.6.85/pyaedt/misc/__init__.py
--rw-r--r--   0        0        0    10210 2023-05-18 13:27:44.045311 pyaedt-0.6.85/pyaedt/misc/aedtlib_personalib_install.py
--rw-r--r--   0        0        0    19870 2023-05-18 13:27:44.045311 pyaedt-0.6.85/pyaedt/misc/amat.xml
--rw-r--r--   0        0        0     2620 2023-07-05 06:36:05.694306 pyaedt-0.6.85/pyaedt/misc/ansys_cloud.areg
--rw-r--r--   0        0        0     3731 2023-05-18 13:27:44.045311 pyaedt-0.6.85/pyaedt/misc/console_setup.py
--rw-r--r--   0        0        0       48 2023-05-18 13:27:44.045311 pyaedt-0.6.85/pyaedt/misc/create_remote_dir.py
--rw-r--r--   0        0        0    15250 2023-05-18 13:27:44.045311 pyaedt-0.6.85/pyaedt/misc/images/gallery/PyAEDT.png
--rw-r--r--   0        0        0      855 2023-05-18 13:27:44.060935 pyaedt-0.6.85/pyaedt/misc/images/large/pyansys.png
--rw-r--r--   0        0        0     5611 2023-07-07 09:29:33.874017 pyaedt-0.6.85/pyaedt/misc/install_extra_toolkits.py
--rw-r--r--   0        0        0     1728 2023-05-18 13:27:44.060935 pyaedt-0.6.85/pyaedt/misc/jupyter_template.ipynb
--rw-r--r--   0        0        0      678 2023-05-18 13:27:44.060935 pyaedt-0.6.85/pyaedt/misc/misc.py
--rw-r--r--   0        0        0   771467 2023-05-18 13:27:44.060935 pyaedt-0.6.85/pyaedt/misc/ml_data_file_train_100MHz_1GHz.json
--rw-r--r--   0        0        0   502580 2023-05-18 13:27:44.060935 pyaedt-0.6.85/pyaedt/misc/ml_data_file_train_1GHz_10GHz.json
--rw-r--r--   0        0        0   162026 2023-05-18 13:27:44.060935 pyaedt-0.6.85/pyaedt/misc/patch_svr_model_100MHz_1GHz.joblib
--rw-r--r--   0        0        0   134414 2023-05-18 13:27:44.060935 pyaedt-0.6.85/pyaedt/misc/patch_svr_model_1GHz_10GHz.joblib
--rw-r--r--   0        0        0      289 2023-05-18 13:27:44.060935 pyaedt-0.6.85/pyaedt/misc/pyaedt.runtimeconfig.json
--rw-r--r--   0        0        0      953 2023-05-18 13:27:44.060935 pyaedt-0.6.85/pyaedt/misc/pyaedt_local_config.acf
--rw-r--r--   0        0        0    16550 2023-05-18 13:27:44.060935 pyaedt-0.6.85/pyaedt/misc/pyansys-logo-black-cropped.png
--rw-r--r--   0        0        0      868 2023-05-18 13:27:44.060935 pyaedt-0.6.85/pyaedt/misc/template.acf
--rw-r--r--   0        0        0        0 2023-05-18 13:27:44.076561 pyaedt-0.6.85/pyaedt/modeler/__init__.py
--rw-r--r--   0        0        0        0 2023-05-18 13:27:44.076561 pyaedt-0.6.85/pyaedt/modeler/advanced_cad/__init__.py
--rw-r--r--   0        0        0    14107 2023-05-29 06:50:01.509226 pyaedt-0.6.85/pyaedt/modeler/advanced_cad/actors.py
--rw-r--r--   0        0        0    20051 2023-05-29 06:50:01.509226 pyaedt-0.6.85/pyaedt/modeler/advanced_cad/multiparts.py
--rw-r--r--   0        0        0    18513 2023-05-18 13:27:44.076561 pyaedt-0.6.85/pyaedt/modeler/advanced_cad/oms.py
--rw-r--r--   0        0        0    16840 2023-05-29 06:50:01.509226 pyaedt-0.6.85/pyaedt/modeler/advanced_cad/parts.py
--rw-r--r--   0        0        0   120896 2023-07-13 12:17:05.981892 pyaedt-0.6.85/pyaedt/modeler/advanced_cad/stackup_3d.py
--rw-r--r--   0        0        0   198119 2023-07-13 12:17:05.981892 pyaedt-0.6.85/pyaedt/modeler/cad/Modeler.py
--rw-r--r--   0        0        0   116735 2023-07-13 12:17:05.997514 pyaedt-0.6.85/pyaedt/modeler/cad/Primitives.py
--rw-r--r--   0        0        0    11407 2023-07-13 12:17:05.997514 pyaedt-0.6.85/pyaedt/modeler/cad/Primitives2D.py
--rw-r--r--   0        0        0   129702 2023-07-13 12:17:05.997514 pyaedt-0.6.85/pyaedt/modeler/cad/Primitives3D.py
--rw-r--r--   0        0        0        0 2023-05-18 13:27:44.076561 pyaedt-0.6.85/pyaedt/modeler/cad/__init__.py
--rw-r--r--   0        0        0    38322 2023-07-11 09:19:45.829829 pyaedt-0.6.85/pyaedt/modeler/cad/components_3d.py
--rw-r--r--   0        0        0    49140 2023-07-13 12:17:05.997514 pyaedt-0.6.85/pyaedt/modeler/cad/elements3d.py
--rw-r--r--   0        0        0    59316 2023-07-13 12:17:05.997514 pyaedt-0.6.85/pyaedt/modeler/cad/object3d.py
--rw-r--r--   0        0        0    53078 2023-07-11 09:19:45.829829 pyaedt-0.6.85/pyaedt/modeler/cad/polylines.py
--rw-r--r--   0        0        0    12645 2023-05-29 06:50:01.524910 pyaedt-0.6.85/pyaedt/modeler/calculators.py
--rw-r--r--   0        0        0    43135 2023-07-14 12:06:38.284859 pyaedt-0.6.85/pyaedt/modeler/circuits/PrimitivesCircuit.py
--rw-r--r--   0        0        0    33551 2023-07-05 14:41:01.503279 pyaedt-0.6.85/pyaedt/modeler/circuits/PrimitivesEmit.py
--rw-r--r--   0        0        0     8236 2023-07-13 12:17:05.997514 pyaedt-0.6.85/pyaedt/modeler/circuits/PrimitivesMaxwellCircuit.py
--rw-r--r--   0        0        0    63132 2023-07-13 12:17:05.997514 pyaedt-0.6.85/pyaedt/modeler/circuits/PrimitivesNexxim.py
--rw-r--r--   0        0        0    15185 2023-07-13 12:17:05.997514 pyaedt-0.6.85/pyaedt/modeler/circuits/PrimitivesTwinBuilder.py
--rw-r--r--   0        0        0        0 2023-05-18 13:27:44.092187 pyaedt-0.6.85/pyaedt/modeler/circuits/__init__.py
--rw-r--r--   0        0        0    31781 2023-07-14 10:51:56.427377 pyaedt-0.6.85/pyaedt/modeler/circuits/object3dcircuit.py
--rw-r--r--   0        0        0    68135 2023-05-18 13:27:44.092187 pyaedt-0.6.85/pyaedt/modeler/geometry_operators.py
--rw-r--r--   0        0        0     6956 2023-07-13 12:17:05.997514 pyaedt-0.6.85/pyaedt/modeler/modeler2d.py
--rw-r--r--   0        0        0    64961 2023-07-14 12:06:38.284859 pyaedt-0.6.85/pyaedt/modeler/modeler3d.py
--rw-r--r--   0        0        0    32782 2023-07-11 09:19:45.829829 pyaedt-0.6.85/pyaedt/modeler/modelerpcb.py
--rw-r--r--   0        0        0    50049 2023-07-13 12:17:05.997514 pyaedt-0.6.85/pyaedt/modeler/pcb/Primitives3DLayout.py
--rw-r--r--   0        0        0        0 2023-05-18 13:27:44.092187 pyaedt-0.6.85/pyaedt/modeler/pcb/__init__.py
--rw-r--r--   0        0        0    65191 2023-07-13 12:17:05.997514 pyaedt-0.6.85/pyaedt/modeler/pcb/object3dlayout.py
--rw-r--r--   0        0        0    23687 2023-07-11 09:19:45.829829 pyaedt-0.6.85/pyaedt/modeler/schematic.py
--rw-r--r--   0        0        0    34537 2023-07-12 21:05:43.799165 pyaedt-0.6.85/pyaedt/modules/AdvancedPostProcessing.py
--rw-r--r--   0        0        0   159807 2023-07-06 12:04:15.260849 pyaedt-0.6.85/pyaedt/modules/Boundary.py
--rw-r--r--   0        0        0    71535 2023-06-21 10:09:54.048412 pyaedt-0.6.85/pyaedt/modules/CableModeling.py
--rw-r--r--   0        0        0    16319 2023-05-18 13:27:44.092187 pyaedt-0.6.85/pyaedt/modules/CircuitTemplates.py
--rw-r--r--   0        0        0    51967 2023-05-29 06:50:01.540477 pyaedt-0.6.85/pyaedt/modules/DesignXPloration.py
--rw-r--r--   0        0        0    40465 2023-05-29 06:50:01.540477 pyaedt-0.6.85/pyaedt/modules/LayerStackup.py
--rw-r--r--   0        0        0    82903 2023-05-29 06:50:01.540477 pyaedt-0.6.85/pyaedt/modules/Material.py
--rw-r--r--   0        0        0    28440 2023-07-11 09:19:45.829829 pyaedt-0.6.85/pyaedt/modules/MaterialLib.py
--rw-r--r--   0        0        0    53543 2023-07-13 12:17:05.997514 pyaedt-0.6.85/pyaedt/modules/Mesh.py
--rw-r--r--   0        0        0    11976 2023-05-29 06:50:01.540477 pyaedt-0.6.85/pyaedt/modules/Mesh3DLayout.py
--rw-r--r--   0        0        0    27635 2023-06-29 10:10:15.411431 pyaedt-0.6.85/pyaedt/modules/MeshIcepak.py
--rw-r--r--   0        0        0     4437 2023-05-18 13:27:44.107810 pyaedt-0.6.85/pyaedt/modules/OptimetricsTemplates.py
--rw-r--r--   0        0        0   181969 2023-07-11 09:19:45.845452 pyaedt-0.6.85/pyaedt/modules/PostProcessor.py
--rw-r--r--   0        0        0    64120 2023-06-29 10:10:15.411431 pyaedt-0.6.85/pyaedt/modules/SetupTemplates.py
--rw-r--r--   0        0        0   121445 2023-06-15 11:58:34.060146 pyaedt-0.6.85/pyaedt/modules/SolveSetup.py
--rw-r--r--   0        0        0    33257 2023-05-29 06:50:01.540477 pyaedt-0.6.85/pyaedt/modules/SolveSweeps.py
--rw-r--r--   0        0        0        0 2023-05-18 13:27:44.107810 pyaedt-0.6.85/pyaedt/modules/__init__.py
--rw-r--r--   0        0        0    30706 2023-06-29 10:10:15.427058 pyaedt-0.6.85/pyaedt/modules/monitor_icepak.py
--rw-r--r--   0        0        0   103333 2023-05-29 06:50:01.556103 pyaedt-0.6.85/pyaedt/modules/report_templates.py
--rw-r--r--   0        0        0   126124 2023-06-23 13:22:55.453306 pyaedt-0.6.85/pyaedt/modules/solutions.py
--rw-r--r--   0        0        0    95976 2023-07-13 12:17:05.997514 pyaedt-0.6.85/pyaedt/q3d.py
--rw-r--r--   0        0        0    10581 2023-05-29 06:50:01.556103 pyaedt-0.6.85/pyaedt/rmxprt.py
--rw-r--r--   0        0        0        0 2023-05-18 13:27:44.107810 pyaedt-0.6.85/pyaedt/rpc/__init__.py
--rw-r--r--   0        0        0      415 2023-05-18 13:27:44.107810 pyaedt-0.6.85/pyaedt/rpc/local_server.py
--rw-r--r--   0        0        0    40721 2023-05-18 13:27:44.107810 pyaedt-0.6.85/pyaedt/rpc/rpyc_services.py
--rw-r--r--   0        0        0        0 2023-05-18 13:27:44.107810 pyaedt-0.6.85/pyaedt/sbrplus/__init__.py
--rw-r--r--   0        0        0     9425 2023-05-18 13:27:44.107810 pyaedt-0.6.85/pyaedt/sbrplus/hdm_parser.py
--rw-r--r--   0        0        0     2096 2023-05-18 13:27:44.107810 pyaedt-0.6.85/pyaedt/sbrplus/hdm_utils.py
--rw-r--r--   0        0        0     2607 2023-05-18 13:27:44.107810 pyaedt-0.6.85/pyaedt/sbrplus/matlab/HdmObject.m
--rw-r--r--   0        0        0       97 2023-05-18 13:27:44.107810 pyaedt-0.6.85/pyaedt/sbrplus/matlab/README.md
--rw-r--r--   0        0        0      735 2023-05-18 13:27:44.123438 pyaedt-0.6.85/pyaedt/sbrplus/matlab/SbrBounceType.m
--rw-r--r--   0        0        0     2886 2023-05-18 13:27:44.123438 pyaedt-0.6.85/pyaedt/sbrplus/matlab/StopWatch.m
--rw-r--r--   0        0        0     1402 2023-05-18 13:27:44.123438 pyaedt-0.6.85/pyaedt/sbrplus/matlab/add_3dlight.m
--rw-r--r--   0        0        0      340 2023-05-18 13:27:44.123438 pyaedt-0.6.85/pyaedt/sbrplus/matlab/amp2db.m
--rw-r--r--   0        0        0    36837 2023-05-18 13:27:44.123438 pyaedt-0.6.85/pyaedt/sbrplus/matlab/draw_rays1.m
--rw-r--r--   0        0        0     4322 2023-05-18 13:27:44.123438 pyaedt-0.6.85/pyaedt/sbrplus/matlab/draw_wfobj.m
--rw-r--r--   0        0        0    31414 2023-05-18 13:27:44.123438 pyaedt-0.6.85/pyaedt/sbrplus/matlab/filter_rays1.m
--rw-r--r--   0        0        0     1504 2023-05-18 13:27:44.123438 pyaedt-0.6.85/pyaedt/sbrplus/matlab/filtered_tracks.m
--rw-r--r--   0        0        0    20853 2023-05-18 13:27:44.123438 pyaedt-0.6.85/pyaedt/sbrplus/matlab/ld_sbrplushdm.m
--rw-r--r--   0        0        0    14781 2023-05-18 13:27:44.123438 pyaedt-0.6.85/pyaedt/sbrplus/matlab/ld_wfobj.m
--rw-r--r--   0        0        0      318 2023-05-18 13:27:44.123438 pyaedt-0.6.85/pyaedt/sbrplus/matlab/pwr2db.m
--rw-r--r--   0        0        0     2607 2023-05-18 13:27:44.123438 pyaedt-0.6.85/pyaedt/sbrplus/matlab/validate_sfields.m
--rw-r--r--   0        0        0     7632 2023-05-29 06:50:01.556103 pyaedt-0.6.85/pyaedt/sbrplus/plot.py
--rw-r--r--   0        0        0    10410 2023-06-05 09:10:35.946956 pyaedt-0.6.85/pyaedt/siwave.py
--rw-r--r--   0        0        0    10527 2023-05-18 13:27:44.123438 pyaedt-0.6.85/pyaedt/twinbuilder.py
--rw-r--r--   0        0        0     4556 2023-07-14 07:11:37.571749 pyaedt-0.6.85/pyproject.toml
--rw-r--r--   0        0        0    15772 1970-01-01 00:00:00.000000 pyaedt-0.6.85/PKG-INFO
+-rw-r--r--   0        0        0     1111 2023-05-30 06:59:37.486926 pyaedt-0.6.86/LICENSE
+-rw-r--r--   0        0        0     9947 2023-05-30 06:59:37.486926 pyaedt-0.6.86/README.md
+-rw-r--r--   0        0        0     2629 2023-07-21 14:33:51.388714 pyaedt-0.6.86/pyaedt/__init__.py
+-rw-r--r--   0        0        0    26756 2023-07-21 09:35:13.229002 pyaedt-0.6.86/pyaedt/aedt_logger.py
+-rw-r--r--   0        0        0     6965 2023-05-30 06:59:39.408947 pyaedt-0.6.86/pyaedt/application/AEDT_File_Management.py
+-rw-r--r--   0        0        0    88967 2023-07-21 09:35:13.229002 pyaedt-0.6.86/pyaedt/application/Analysis.py
+-rw-r--r--   0        0        0    50696 2023-07-21 09:35:13.229002 pyaedt-0.6.86/pyaedt/application/Analysis3D.py
+-rw-r--r--   0        0        0    17066 2023-06-20 15:35:24.349674 pyaedt-0.6.86/pyaedt/application/Analysis3DLayout.py
+-rw-r--r--   0        0        0     3088 2023-05-30 06:59:39.408947 pyaedt-0.6.86/pyaedt/application/AnalysisMaxwellCircuit.py
+-rw-r--r--   0        0        0    19948 2023-07-19 13:20:21.575376 pyaedt-0.6.86/pyaedt/application/AnalysisNexxim.py
+-rw-r--r--   0        0        0     4431 2023-05-30 06:59:39.408947 pyaedt-0.6.86/pyaedt/application/AnalysisRMxprt.py
+-rw-r--r--   0        0        0     4596 2023-05-30 06:59:39.424579 pyaedt-0.6.86/pyaedt/application/AnalysisTwinBuilder.py
+-rw-r--r--   0        0        0   136452 2023-07-21 09:35:13.229002 pyaedt-0.6.86/pyaedt/application/Design.py
+-rw-r--r--   0        0        0     6115 2023-05-30 06:59:39.424579 pyaedt-0.6.86/pyaedt/application/JobManager.py
+-rw-r--r--   0        0        0    75793 2023-07-20 11:48:09.458225 pyaedt-0.6.86/pyaedt/application/Variables.py
+-rw-r--r--   0        0        0        0 2023-05-30 06:59:39.424579 pyaedt-0.6.86/pyaedt/application/__init__.py
+-rw-r--r--   0        0        0    12464 2023-05-30 06:59:39.424579 pyaedt-0.6.86/pyaedt/application/aedt_objects.py
+-rw-r--r--   0        0        0    36750 2023-06-29 09:15:20.741006 pyaedt-0.6.86/pyaedt/application/design_solutions.py
+-rw-r--r--   0        0        0    62949 2023-07-21 09:35:13.229002 pyaedt-0.6.86/pyaedt/circuit.py
+-rw-r--r--   0        0        0    10259 2023-07-20 07:33:55.805436 pyaedt-0.6.86/pyaedt/common_rpc.py
+-rw-r--r--   0        0        0    84793 2023-07-21 09:35:13.229002 pyaedt-0.6.86/pyaedt/desktop.py
+-rw-r--r--   0        0        0    15104 2023-05-30 06:59:39.424579 pyaedt-0.6.86/pyaedt/dlls/PDFReport/AnsysReport.deps.json
+-rw-r--r--   0        0        0    23552 2023-05-30 06:59:39.424579 pyaedt-0.6.86/pyaedt/dlls/PDFReport/AnsysReport.dll
+-rw-r--r--   0        0        0     1086 2023-06-28 08:36:59.983528 pyaedt-0.6.86/pyaedt/dlls/PDFReport/AnsysTemplate.json
+-rw-r--r--   0        0        0   204800 2023-05-30 06:59:39.424579 pyaedt-0.6.86/pyaedt/dlls/PDFReport/ICSharpCode.SharpZipLib.dll
+-rw-r--r--   0        0        0   577445 2023-05-30 06:59:39.440208 pyaedt-0.6.86/pyaedt/dlls/PDFReport/ICSharpCode.SharpZipLib.xml
+-rw-r--r--   0        0        0     9836 2023-05-30 06:59:39.440208 pyaedt-0.6.86/pyaedt/dlls/PDFReport/Images/Ansys.png
+-rw-r--r--   0        0        0   238592 2023-05-30 06:59:39.440208 pyaedt-0.6.86/pyaedt/dlls/PDFReport/MigraDocCore.DocumentObjectModel.dll
+-rw-r--r--   0        0        0   115712 2023-05-30 06:59:39.440208 pyaedt-0.6.86/pyaedt/dlls/PDFReport/MigraDocCore.Rendering.dll
+-rw-r--r--   0        0        0   705296 2023-05-30 06:59:39.455836 pyaedt-0.6.86/pyaedt/dlls/PDFReport/Newtonsoft.Json.dll
+-rw-r--r--   0        0        0   712253 2023-05-30 06:59:39.455836 pyaedt-0.6.86/pyaedt/dlls/PDFReport/Newtonsoft.Json.xml
+-rw-r--r--   0        0        0    80384 2023-05-30 06:59:39.455836 pyaedt-0.6.86/pyaedt/dlls/PDFReport/PdfSharpCore.Charting.dll
+-rw-r--r--   0        0        0   546816 2023-05-30 06:59:39.471459 pyaedt-0.6.86/pyaedt/dlls/PDFReport/PdfSharpCore.dll
+-rw-r--r--   0        0        0   367616 2023-05-30 06:59:39.471459 pyaedt-0.6.86/pyaedt/dlls/PDFReport/SixLabors.Fonts.dll
+-rw-r--r--   0        0        0   536367 2023-05-30 06:59:39.471459 pyaedt-0.6.86/pyaedt/dlls/PDFReport/SixLabors.Fonts.xml
+-rw-r--r--   0        0        0  1229824 2023-05-30 06:59:39.487088 pyaedt-0.6.86/pyaedt/dlls/PDFReport/SixLabors.ImageSharp.dll
+-rw-r--r--   0        0        0  3285773 2023-05-30 06:59:39.502713 pyaedt-0.6.86/pyaedt/dlls/PDFReport/SixLabors.ImageSharp.xml
+-rw-r--r--   0        0        0   120664 2023-05-30 06:59:39.502713 pyaedt-0.6.86/pyaedt/dlls/PDFReport/System.Runtime.dll
+-rw-r--r--   0        0        0  1505294 2023-05-30 06:59:39.518353 pyaedt-0.6.86/pyaedt/dlls/PDFReport/System.Runtime.xml
+-rw-r--r--   0        0        0     5632 2023-05-30 06:59:39.518353 pyaedt-0.6.86/pyaedt/dlls/PDFReport/de/PdfSharpCore.resources.dll
+-rw-r--r--   0        0        0   160754 2023-05-30 06:59:39.533962 pyaedt-0.6.86/pyaedt/dlls/PDFReport/de/System.Collections.NonGeneric.xml
+-rw-r--r--   0        0        0    24188 2023-07-21 12:41:58.329803 pyaedt-0.6.86/pyaedt/downloads.py
+-rw-r--r--   0        0        0   137623 2023-06-29 17:19:45.292504 pyaedt-0.6.86/pyaedt/edb.py
+-rw-r--r--   0        0        0      333 2023-05-30 06:59:39.533962 pyaedt-0.6.86/pyaedt/edb_core/__init__.py
+-rw-r--r--   0        0        0    98675 2023-07-13 12:00:19.155166 pyaedt-0.6.86/pyaedt/edb_core/components.py
+-rw-r--r--   0        0        0        0 2023-06-05 09:36:43.922575 pyaedt-0.6.86/pyaedt/edb_core/dotnet/__init__.py
+-rw-r--r--   0        0        0    31509 2023-07-20 07:33:55.805436 pyaedt-0.6.86/pyaedt/edb_core/dotnet/database.py
+-rw-r--r--   0        0        0     7909 2023-06-05 09:36:43.938202 pyaedt-0.6.86/pyaedt/edb_core/dotnet/layout.py
+-rw-r--r--   0        0        0    48210 2023-06-05 09:36:43.938202 pyaedt-0.6.86/pyaedt/edb_core/dotnet/primitive.py
+-rw-r--r--   0        0        0        0 2023-05-30 06:59:39.533962 pyaedt-0.6.86/pyaedt/edb_core/edb_data/__init__.py
+-rw-r--r--   0        0        0    33195 2023-06-12 08:05:31.703949 pyaedt-0.6.86/pyaedt/edb_core/edb_data/components_data.py
+-rw-r--r--   0        0        0    40112 2023-07-20 12:55:34.842217 pyaedt-0.6.86/pyaedt/edb_core/edb_data/control_file.py
+-rw-r--r--   0        0        0      937 2023-05-30 06:59:39.533962 pyaedt-0.6.86/pyaedt/edb_core/edb_data/design_options.py
+-rw-r--r--   0        0        0      867 2023-05-30 06:59:39.533962 pyaedt-0.6.86/pyaedt/edb_core/edb_data/edbvalue.py
+-rw-r--r--   0        0        0    12243 2023-06-05 09:36:43.938202 pyaedt-0.6.86/pyaedt/edb_core/edb_data/hfss_extent_info.py
+-rw-r--r--   0        0        0    65661 2023-06-05 09:36:43.938202 pyaedt-0.6.86/pyaedt/edb_core/edb_data/hfss_simulation_setup_data.py
+-rw-r--r--   0        0        0    20820 2023-07-17 10:14:12.806355 pyaedt-0.6.86/pyaedt/edb_core/edb_data/layer_data.py
+-rw-r--r--   0        0        0     6880 2023-07-21 11:59:44.723243 pyaedt-0.6.86/pyaedt/edb_core/edb_data/nets_data.py
+-rw-r--r--   0        0        0    61171 2023-07-21 12:41:58.329803 pyaedt-0.6.86/pyaedt/edb_core/edb_data/padstacks_data.py
+-rw-r--r--   0        0        0    32590 2023-06-29 16:47:26.445610 pyaedt-0.6.86/pyaedt/edb_core/edb_data/primitives_data.py
+-rw-r--r--   0        0        0   102298 2023-06-14 08:50:43.463988 pyaedt-0.6.86/pyaedt/edb_core/edb_data/simulation_configuration.py
+-rw-r--r--   0        0        0    36324 2023-06-05 09:36:43.938202 pyaedt-0.6.86/pyaedt/edb_core/edb_data/siwave_simulation_setup_data.py
+-rw-r--r--   0        0        0    34944 2023-07-10 08:39:13.777984 pyaedt-0.6.86/pyaedt/edb_core/edb_data/sources.py
+-rw-r--r--   0        0        0     3923 2023-06-05 14:54:59.781956 pyaedt-0.6.86/pyaedt/edb_core/edb_data/utilities.py
+-rw-r--r--   0        0        0     2432 2023-06-05 09:36:43.938202 pyaedt-0.6.86/pyaedt/edb_core/edb_data/variables.py
+-rw-r--r--   0        0        0     3258 2023-05-30 06:59:39.549589 pyaedt-0.6.86/pyaedt/edb_core/general.py
+-rw-r--r--   0        0        0    68725 2023-06-29 11:46:59.997639 pyaedt-0.6.86/pyaedt/edb_core/hfss.py
+-rw-r--r--   0        0        0        0 2023-05-30 06:59:39.549589 pyaedt-0.6.86/pyaedt/edb_core/ipc2581/__init__.py
+-rw-r--r--   0        0        0        0 2023-05-30 06:59:39.549589 pyaedt-0.6.86/pyaedt/edb_core/ipc2581/bom/__init__.py
+-rw-r--r--   0        0        0      673 2023-05-30 06:59:39.549589 pyaedt-0.6.86/pyaedt/edb_core/ipc2581/bom/bom.py
+-rw-r--r--   0        0        0     1283 2023-05-30 06:59:39.549589 pyaedt-0.6.86/pyaedt/edb_core/ipc2581/bom/bom_item.py
+-rw-r--r--   0        0        0     2213 2023-05-30 06:59:39.549589 pyaedt-0.6.86/pyaedt/edb_core/ipc2581/bom/characteristics.py
+-rw-r--r--   0        0        0      524 2023-05-30 06:59:39.549589 pyaedt-0.6.86/pyaedt/edb_core/ipc2581/bom/refdes.py
+-rw-r--r--   0        0        0        0 2023-05-30 06:59:39.549589 pyaedt-0.6.86/pyaedt/edb_core/ipc2581/content/__init__.py
+-rw-r--r--   0        0        0      768 2023-05-30 06:59:39.549589 pyaedt-0.6.86/pyaedt/edb_core/ipc2581/content/color.py
+-rw-r--r--   0        0        0     2118 2023-05-30 06:59:39.549589 pyaedt-0.6.86/pyaedt/edb_core/ipc2581/content/content.py
+-rw-r--r--   0        0        0      938 2023-05-30 06:59:39.549589 pyaedt-0.6.86/pyaedt/edb_core/ipc2581/content/dictionary_color.py
+-rw-r--r--   0        0        0      921 2023-05-30 06:59:39.549589 pyaedt-0.6.86/pyaedt/edb_core/ipc2581/content/dictionary_fill.py
+-rw-r--r--   0        0        0     1029 2023-05-30 06:59:39.549589 pyaedt-0.6.86/pyaedt/edb_core/ipc2581/content/dictionary_line.py
+-rw-r--r--   0        0        0      416 2023-05-30 06:59:39.549589 pyaedt-0.6.86/pyaedt/edb_core/ipc2581/content/entry_color.py
+-rw-r--r--   0        0        0      548 2023-05-30 06:59:39.549589 pyaedt-0.6.86/pyaedt/edb_core/ipc2581/content/entry_line.py
+-rw-r--r--   0        0        0      523 2023-05-30 06:59:39.549589 pyaedt-0.6.86/pyaedt/edb_core/ipc2581/content/fill.py
+-rw-r--r--   0        0        0      284 2023-05-30 06:59:39.549589 pyaedt-0.6.86/pyaedt/edb_core/ipc2581/content/layer_ref.py
+-rw-r--r--   0        0        0     2850 2023-06-05 09:36:43.953828 pyaedt-0.6.86/pyaedt/edb_core/ipc2581/content/standard_geometries_dictionary.py
+-rw-r--r--   0        0        0        0 2023-05-30 06:59:39.565215 pyaedt-0.6.86/pyaedt/edb_core/ipc2581/ecad/__init__.py
+-rw-r--r--   0        0        0        0 2023-05-30 06:59:39.565215 pyaedt-0.6.86/pyaedt/edb_core/ipc2581/ecad/cad_data/__init__.py
+-rw-r--r--   0        0        0     1183 2023-05-30 06:59:39.565215 pyaedt-0.6.86/pyaedt/edb_core/ipc2581/ecad/cad_data/assembly_drawing.py
+-rw-r--r--   0        0        0     1319 2023-05-30 06:59:39.565215 pyaedt-0.6.86/pyaedt/edb_core/ipc2581/ecad/cad_data/cad_data.py
+-rw-r--r--   0        0        0     1516 2023-05-30 06:59:39.565215 pyaedt-0.6.86/pyaedt/edb_core/ipc2581/ecad/cad_data/component.py
+-rw-r--r--   0        0        0      960 2023-05-30 06:59:39.565215 pyaedt-0.6.86/pyaedt/edb_core/ipc2581/ecad/cad_data/drill.py
+-rw-r--r--   0        0        0     1964 2023-05-30 06:59:39.565215 pyaedt-0.6.86/pyaedt/edb_core/ipc2581/ecad/cad_data/feature.py
+-rw-r--r--   0        0        0     1158 2023-05-30 06:59:39.565215 pyaedt-0.6.86/pyaedt/edb_core/ipc2581/ecad/cad_data/layer.py
+-rw-r--r--   0        0        0     7763 2023-05-30 06:59:39.565215 pyaedt-0.6.86/pyaedt/edb_core/ipc2581/ecad/cad_data/layer_feature.py
+-rw-r--r--   0        0        0      921 2023-05-30 06:59:39.565215 pyaedt-0.6.86/pyaedt/edb_core/ipc2581/ecad/cad_data/logical_net.py
+-rw-r--r--   0        0        0     1079 2023-05-30 06:59:39.565215 pyaedt-0.6.86/pyaedt/edb_core/ipc2581/ecad/cad_data/outline.py
+-rw-r--r--   0        0        0     4703 2023-05-30 06:59:39.565215 pyaedt-0.6.86/pyaedt/edb_core/ipc2581/ecad/cad_data/package.py
+-rw-r--r--   0        0        0     1440 2023-05-30 06:59:39.565215 pyaedt-0.6.86/pyaedt/edb_core/ipc2581/ecad/cad_data/padstack_def.py
+-rw-r--r--   0        0        0      875 2023-05-30 06:59:39.565215 pyaedt-0.6.86/pyaedt/edb_core/ipc2581/ecad/cad_data/padstack_hole_def.py
+-rw-r--r--   0        0        0     2775 2023-05-30 06:59:39.565215 pyaedt-0.6.86/pyaedt/edb_core/ipc2581/ecad/cad_data/padstack_instance.py
+-rw-r--r--   0        0        0      887 2023-05-30 06:59:39.565215 pyaedt-0.6.86/pyaedt/edb_core/ipc2581/ecad/cad_data/padstack_pad_def.py
+-rw-r--r--   0        0        0     4104 2023-05-30 06:59:39.565215 pyaedt-0.6.86/pyaedt/edb_core/ipc2581/ecad/cad_data/path.py
+-rw-r--r--   0        0        0     2567 2023-05-30 06:59:39.565215 pyaedt-0.6.86/pyaedt/edb_core/ipc2581/ecad/cad_data/phy_net.py
+-rw-r--r--   0        0        0     1002 2023-05-30 06:59:39.565215 pyaedt-0.6.86/pyaedt/edb_core/ipc2581/ecad/cad_data/pin.py
+-rw-r--r--   0        0        0     8010 2023-05-30 06:59:39.565215 pyaedt-0.6.86/pyaedt/edb_core/ipc2581/ecad/cad_data/polygon.py
+-rw-r--r--   0        0        0      663 2023-05-30 06:59:39.565215 pyaedt-0.6.86/pyaedt/edb_core/ipc2581/ecad/cad_data/profile.py
+-rw-r--r--   0        0        0     1162 2023-05-30 06:59:39.565215 pyaedt-0.6.86/pyaedt/edb_core/ipc2581/ecad/cad_data/stackup.py
+-rw-r--r--   0        0        0     1626 2023-05-30 06:59:39.565215 pyaedt-0.6.86/pyaedt/edb_core/ipc2581/ecad/cad_data/stackup_group.py
+-rw-r--r--   0        0        0      838 2023-05-30 06:59:39.565215 pyaedt-0.6.86/pyaedt/edb_core/ipc2581/ecad/cad_data/stackup_layer.py
+-rw-r--r--   0        0        0    11390 2023-05-30 06:59:39.565215 pyaedt-0.6.86/pyaedt/edb_core/ipc2581/ecad/cad_data/step.py
+-rw-r--r--   0        0        0     1033 2023-05-30 06:59:39.565215 pyaedt-0.6.86/pyaedt/edb_core/ipc2581/ecad/cad_header.py
+-rw-r--r--   0        0        0      683 2023-05-30 06:59:39.565215 pyaedt-0.6.86/pyaedt/edb_core/ipc2581/ecad/ecad.py
+-rw-r--r--   0        0        0     2008 2023-05-30 06:59:39.565215 pyaedt-0.6.86/pyaedt/edb_core/ipc2581/ecad/spec.py
+-rw-r--r--   0        0        0     1624 2023-05-30 06:59:39.580847 pyaedt-0.6.86/pyaedt/edb_core/ipc2581/history_record.py
+-rw-r--r--   0        0        0    21800 2023-06-05 09:36:43.953828 pyaedt-0.6.86/pyaedt/edb_core/ipc2581/ipc2581.py
+-rw-r--r--   0        0        0      966 2023-05-30 06:59:39.580847 pyaedt-0.6.86/pyaedt/edb_core/ipc2581/logistic_header.py
+-rw-r--r--   0        0        0    47176 2023-06-22 08:21:07.514633 pyaedt-0.6.86/pyaedt/edb_core/layout.py
+-rw-r--r--   0        0        0    33310 2023-06-05 09:36:43.953828 pyaedt-0.6.86/pyaedt/edb_core/materials.py
+-rw-r--r--   0        0        0    44030 2023-07-21 11:59:44.723243 pyaedt-0.6.86/pyaedt/edb_core/nets.py
+-rw-r--r--   0        0        0    49394 2023-07-21 11:24:42.095565 pyaedt-0.6.86/pyaedt/edb_core/padstack.py
+-rw-r--r--   0        0        0    58809 2023-06-19 10:47:11.266974 pyaedt-0.6.86/pyaedt/edb_core/siwave.py
+-rw-r--r--   0        0        0   111074 2023-07-17 10:14:12.806355 pyaedt-0.6.86/pyaedt/edb_core/stackup.py
+-rw-r--r--   0        0        0    11500 2023-07-21 09:35:13.244634 pyaedt-0.6.86/pyaedt/emit.py
+-rw-r--r--   0        0        0     6100 2023-07-06 12:50:33.852654 pyaedt-0.6.86/pyaedt/emit_core/Couplings.py
+-rw-r--r--   0        0        0     2825 2023-07-20 07:33:55.805436 pyaedt-0.6.86/pyaedt/emit_core/__init__.py
+-rw-r--r--   0        0        0     1621 2023-06-13 17:56:07.965688 pyaedt-0.6.86/pyaedt/emit_core/emit_constants.py
+-rw-r--r--   0        0        0    11102 2023-07-21 12:41:58.329803 pyaedt-0.6.86/pyaedt/emit_core/interference_classification.py
+-rw-r--r--   0        0        0        2 2023-05-30 06:59:39.580847 pyaedt-0.6.86/pyaedt/emit_core/results/__init__.py
+-rw-r--r--   0        0        0     7406 2023-07-06 12:50:33.852654 pyaedt-0.6.86/pyaedt/emit_core/results/results.py
+-rw-r--r--   0        0        0    13896 2023-07-06 12:50:33.852654 pyaedt-0.6.86/pyaedt/emit_core/results/revision.py
+-rw-r--r--   0        0        0    14317 2023-05-30 06:59:39.580847 pyaedt-0.6.86/pyaedt/generic/DataHandlers.py
+-rw-r--r--   0        0        0    12252 2023-06-21 12:50:18.007016 pyaedt-0.6.86/pyaedt/generic/LoadAEDTFile.py
+-rw-r--r--   0        0        0        0 2023-05-30 06:59:39.580847 pyaedt-0.6.86/pyaedt/generic/__init__.py
+-rw-r--r--   0        0        0     3257 2023-05-30 06:59:39.580847 pyaedt-0.6.86/pyaedt/generic/clr_module.py
+-rw-r--r--   0        0        0    83443 2023-07-20 11:48:09.458225 pyaedt-0.6.86/pyaedt/generic/configurations.py
+-rw-r--r--   0        0        0    28645 2023-05-30 06:59:39.596468 pyaedt-0.6.86/pyaedt/generic/constants.py
+-rw-r--r--   0        0        0    21891 2023-05-30 06:59:39.596468 pyaedt-0.6.86/pyaedt/generic/design_types.py
+-rw-r--r--   0        0        0     3442 2023-07-13 12:00:19.155166 pyaedt-0.6.86/pyaedt/generic/filesystem.py
+-rw-r--r--   0        0        0    71208 2023-07-21 09:35:13.244634 pyaedt-0.6.86/pyaedt/generic/general_methods.py
+-rw-r--r--   0        0        0     9410 2023-07-20 12:33:36.682607 pyaedt-0.6.86/pyaedt/generic/grpc_plugin.py
+-rw-r--r--   0        0        0     3043 2023-07-11 14:47:17.448018 pyaedt-0.6.86/pyaedt/generic/grpc_plugin_dll.py
+-rw-r--r--   0        0        0    25808 2023-05-30 06:59:39.596468 pyaedt-0.6.86/pyaedt/generic/ibis_reader.py
+-rw-r--r--   0        0        0     7029 2023-07-13 12:00:19.155166 pyaedt-0.6.86/pyaedt/generic/near_field_import.py
+-rw-r--r--   0        0        0     9795 2023-05-30 06:59:39.596468 pyaedt-0.6.86/pyaedt/generic/pdf.py
+-rw-r--r--   0        0        0    62327 2023-05-30 06:59:39.596468 pyaedt-0.6.86/pyaedt/generic/plot.py
+-rw-r--r--   0        0        0    11405 2023-06-22 08:21:07.514633 pyaedt-0.6.86/pyaedt/generic/process.py
+-rw-r--r--   0        0        0    20326 2023-05-30 06:59:39.596468 pyaedt-0.6.86/pyaedt/generic/python_optimizers.py
+-rw-r--r--   0        0        0     3536 2023-06-21 12:50:18.007016 pyaedt-0.6.86/pyaedt/generic/report_file_parser.py
+-rw-r--r--   0        0        0    60412 2023-05-30 06:59:39.596468 pyaedt-0.6.86/pyaedt/generic/toolkit.py
+-rw-r--r--   0        0        0    17095 2023-05-30 06:59:39.596468 pyaedt-0.6.86/pyaedt/generic/touchstone_parser.py
+-rw-r--r--   0        0        0      438 2023-05-30 06:59:39.596468 pyaedt-0.6.86/pyaedt/generic/wpf_template.xaml
+-rw-r--r--   0        0        0   255506 2023-07-21 09:35:13.244634 pyaedt-0.6.86/pyaedt/hfss.py
+-rw-r--r--   0        0        0    84753 2023-07-21 09:35:13.244634 pyaedt-0.6.86/pyaedt/hfss3dlayout.py
+-rw-r--r--   0        0        0   200361 2023-07-21 09:35:13.244634 pyaedt-0.6.86/pyaedt/icepak.py
+-rw-r--r--   0        0        0   127831 2023-07-21 09:35:13.244634 pyaedt-0.6.86/pyaedt/maxwell.py
+-rw-r--r--   0        0        0     7803 2023-07-21 09:35:13.244634 pyaedt-0.6.86/pyaedt/maxwellcircuit.py
+-rw-r--r--   0        0        0    24372 2023-07-21 09:35:13.244634 pyaedt-0.6.86/pyaedt/mechanical.py
+-rw-r--r--   0        0        0     3642 2023-05-30 06:59:39.612097 pyaedt-0.6.86/pyaedt/misc/Console.py_build
+-rw-r--r--   0        0        0     2230 2023-05-30 06:59:39.612097 pyaedt-0.6.86/pyaedt/misc/Job_Settings.areg
+-rw-r--r--   0        0        0     3035 2023-05-30 06:59:39.612097 pyaedt-0.6.86/pyaedt/misc/Jupyter.py_build
+-rw-r--r--   0        0        0     3972 2023-07-07 09:12:05.234128 pyaedt-0.6.86/pyaedt/misc/Run_PyAEDT_Script.py_build
+-rw-r--r--   0        0        0     3311 2023-07-07 09:12:05.234128 pyaedt-0.6.86/pyaedt/misc/Run_PyAEDT_Toolkit_Script.py_build
+-rw-r--r--   0        0        0       53 2023-07-21 09:35:13.244634 pyaedt-0.6.86/pyaedt/misc/__init__.py
+-rw-r--r--   0        0        0    10210 2023-05-30 06:59:39.612097 pyaedt-0.6.86/pyaedt/misc/aedtlib_personalib_install.py
+-rw-r--r--   0        0        0    19870 2023-05-30 06:59:39.612097 pyaedt-0.6.86/pyaedt/misc/amat.xml
+-rw-r--r--   0        0        0     2620 2023-07-05 06:36:09.681010 pyaedt-0.6.86/pyaedt/misc/ansys_cloud.areg
+-rw-r--r--   0        0        0     3731 2023-07-21 09:35:13.244634 pyaedt-0.6.86/pyaedt/misc/console_setup.py
+-rw-r--r--   0        0        0       48 2023-05-30 06:59:39.612097 pyaedt-0.6.86/pyaedt/misc/create_remote_dir.py
+-rw-r--r--   0        0        0    15250 2023-05-30 06:59:39.612097 pyaedt-0.6.86/pyaedt/misc/images/gallery/PyAEDT.png
+-rw-r--r--   0        0        0      855 2023-05-30 06:59:39.612097 pyaedt-0.6.86/pyaedt/misc/images/large/pyansys.png
+-rw-r--r--   0        0        0     5611 2023-07-07 06:30:25.350901 pyaedt-0.6.86/pyaedt/misc/install_extra_toolkits.py
+-rw-r--r--   0        0        0     1728 2023-05-30 06:59:39.612097 pyaedt-0.6.86/pyaedt/misc/jupyter_template.ipynb
+-rw-r--r--   0        0        0      678 2023-07-21 09:35:13.244634 pyaedt-0.6.86/pyaedt/misc/misc.py
+-rw-r--r--   0        0        0   771467 2023-05-30 06:59:39.627726 pyaedt-0.6.86/pyaedt/misc/ml_data_file_train_100MHz_1GHz.json
+-rw-r--r--   0        0        0   502580 2023-05-30 06:59:39.627726 pyaedt-0.6.86/pyaedt/misc/ml_data_file_train_1GHz_10GHz.json
+-rw-r--r--   0        0        0   162026 2023-05-30 06:59:39.627726 pyaedt-0.6.86/pyaedt/misc/patch_svr_model_100MHz_1GHz.joblib
+-rw-r--r--   0        0        0   134414 2023-05-30 06:59:39.627726 pyaedt-0.6.86/pyaedt/misc/patch_svr_model_1GHz_10GHz.joblib
+-rw-r--r--   0        0        0      289 2023-05-30 06:59:39.627726 pyaedt-0.6.86/pyaedt/misc/pyaedt.runtimeconfig.json
+-rw-r--r--   0        0        0      953 2023-05-30 06:59:39.627726 pyaedt-0.6.86/pyaedt/misc/pyaedt_local_config.acf
+-rw-r--r--   0        0        0    16550 2023-05-30 06:59:39.627726 pyaedt-0.6.86/pyaedt/misc/pyansys-logo-black-cropped.png
+-rw-r--r--   0        0        0      868 2023-05-30 06:59:39.627726 pyaedt-0.6.86/pyaedt/misc/template.acf
+-rw-r--r--   0        0        0        0 2023-05-30 06:59:39.627726 pyaedt-0.6.86/pyaedt/modeler/__init__.py
+-rw-r--r--   0        0        0        0 2023-05-30 06:59:39.627726 pyaedt-0.6.86/pyaedt/modeler/advanced_cad/__init__.py
+-rw-r--r--   0        0        0    14107 2023-05-30 06:59:39.627726 pyaedt-0.6.86/pyaedt/modeler/advanced_cad/actors.py
+-rw-r--r--   0        0        0    20051 2023-05-30 06:59:39.627726 pyaedt-0.6.86/pyaedt/modeler/advanced_cad/multiparts.py
+-rw-r--r--   0        0        0    18513 2023-05-30 06:59:39.627726 pyaedt-0.6.86/pyaedt/modeler/advanced_cad/oms.py
+-rw-r--r--   0        0        0    16840 2023-05-30 06:59:39.643351 pyaedt-0.6.86/pyaedt/modeler/advanced_cad/parts.py
+-rw-r--r--   0        0        0   120896 2023-07-13 12:00:19.170793 pyaedt-0.6.86/pyaedt/modeler/advanced_cad/stackup_3d.py
+-rw-r--r--   0        0        0   199311 2023-07-21 14:10:56.134350 pyaedt-0.6.86/pyaedt/modeler/cad/Modeler.py
+-rw-r--r--   0        0        0   116735 2023-07-13 12:00:19.170793 pyaedt-0.6.86/pyaedt/modeler/cad/Primitives.py
+-rw-r--r--   0        0        0    11407 2023-07-13 12:00:19.170793 pyaedt-0.6.86/pyaedt/modeler/cad/Primitives2D.py
+-rw-r--r--   0        0        0   129702 2023-07-13 12:00:19.170793 pyaedt-0.6.86/pyaedt/modeler/cad/Primitives3D.py
+-rw-r--r--   0        0        0        0 2023-05-30 06:59:39.643351 pyaedt-0.6.86/pyaedt/modeler/cad/__init__.py
+-rw-r--r--   0        0        0    38322 2023-07-21 09:35:13.260260 pyaedt-0.6.86/pyaedt/modeler/cad/components_3d.py
+-rw-r--r--   0        0        0    49140 2023-07-13 12:00:19.170793 pyaedt-0.6.86/pyaedt/modeler/cad/elements3d.py
+-rw-r--r--   0        0        0    59316 2023-07-21 09:35:13.260260 pyaedt-0.6.86/pyaedt/modeler/cad/object3d.py
+-rw-r--r--   0        0        0    53078 2023-07-11 14:47:17.463644 pyaedt-0.6.86/pyaedt/modeler/cad/polylines.py
+-rw-r--r--   0        0        0    12661 2023-07-19 13:20:21.575376 pyaedt-0.6.86/pyaedt/modeler/calculators.py
+-rw-r--r--   0        0        0    43135 2023-07-14 12:01:50.451661 pyaedt-0.6.86/pyaedt/modeler/circuits/PrimitivesCircuit.py
+-rw-r--r--   0        0        0    33551 2023-07-06 12:50:33.852654 pyaedt-0.6.86/pyaedt/modeler/circuits/PrimitivesEmit.py
+-rw-r--r--   0        0        0     8236 2023-07-13 12:00:19.186418 pyaedt-0.6.86/pyaedt/modeler/circuits/PrimitivesMaxwellCircuit.py
+-rw-r--r--   0        0        0    63132 2023-07-13 12:00:19.186418 pyaedt-0.6.86/pyaedt/modeler/circuits/PrimitivesNexxim.py
+-rw-r--r--   0        0        0    15185 2023-07-13 12:00:19.186418 pyaedt-0.6.86/pyaedt/modeler/circuits/PrimitivesTwinBuilder.py
+-rw-r--r--   0        0        0        0 2023-05-30 06:59:39.658979 pyaedt-0.6.86/pyaedt/modeler/circuits/__init__.py
+-rw-r--r--   0        0        0    31781 2023-07-21 09:35:13.260260 pyaedt-0.6.86/pyaedt/modeler/circuits/object3dcircuit.py
+-rw-r--r--   0        0        0    68135 2023-05-30 06:59:39.658979 pyaedt-0.6.86/pyaedt/modeler/geometry_operators.py
+-rw-r--r--   0        0        0     6956 2023-07-13 12:00:19.186418 pyaedt-0.6.86/pyaedt/modeler/modeler2d.py
+-rw-r--r--   0        0        0    65138 2023-07-18 12:25:32.970625 pyaedt-0.6.86/pyaedt/modeler/modeler3d.py
+-rw-r--r--   0        0        0    32782 2023-07-11 14:47:17.463644 pyaedt-0.6.86/pyaedt/modeler/modelerpcb.py
+-rw-r--r--   0        0        0    50049 2023-07-21 09:35:13.260260 pyaedt-0.6.86/pyaedt/modeler/pcb/Primitives3DLayout.py
+-rw-r--r--   0        0        0        0 2023-05-30 06:59:39.658979 pyaedt-0.6.86/pyaedt/modeler/pcb/__init__.py
+-rw-r--r--   0        0        0    65191 2023-07-13 12:00:19.186418 pyaedt-0.6.86/pyaedt/modeler/pcb/object3dlayout.py
+-rw-r--r--   0        0        0    23687 2023-07-11 14:47:17.463644 pyaedt-0.6.86/pyaedt/modeler/schematic.py
+-rw-r--r--   0        0        0    34537 2023-07-13 12:00:19.186418 pyaedt-0.6.86/pyaedt/modules/AdvancedPostProcessing.py
+-rw-r--r--   0        0        0   159025 2023-07-18 12:25:32.970625 pyaedt-0.6.86/pyaedt/modules/Boundary.py
+-rw-r--r--   0        0        0    71535 2023-06-21 12:50:18.022631 pyaedt-0.6.86/pyaedt/modules/CableModeling.py
+-rw-r--r--   0        0        0    16319 2023-05-30 06:59:39.658979 pyaedt-0.6.86/pyaedt/modules/CircuitTemplates.py
+-rw-r--r--   0        0        0    51967 2023-05-30 06:59:39.658979 pyaedt-0.6.86/pyaedt/modules/DesignXPloration.py
+-rw-r--r--   0        0        0    40465 2023-05-30 06:59:39.674599 pyaedt-0.6.86/pyaedt/modules/LayerStackup.py
+-rw-r--r--   0        0        0    82903 2023-05-30 06:59:39.674599 pyaedt-0.6.86/pyaedt/modules/Material.py
+-rw-r--r--   0        0        0    28440 2023-07-11 14:47:17.463644 pyaedt-0.6.86/pyaedt/modules/MaterialLib.py
+-rw-r--r--   0        0        0    53543 2023-07-13 12:00:19.186418 pyaedt-0.6.86/pyaedt/modules/Mesh.py
+-rw-r--r--   0        0        0    11976 2023-05-30 06:59:39.674599 pyaedt-0.6.86/pyaedt/modules/Mesh3DLayout.py
+-rw-r--r--   0        0        0    27635 2023-06-26 14:19:11.175189 pyaedt-0.6.86/pyaedt/modules/MeshIcepak.py
+-rw-r--r--   0        0        0     4437 2023-05-30 06:59:39.674599 pyaedt-0.6.86/pyaedt/modules/OptimetricsTemplates.py
+-rw-r--r--   0        0        0   181969 2023-07-21 09:35:13.260260 pyaedt-0.6.86/pyaedt/modules/PostProcessor.py
+-rw-r--r--   0        0        0    64120 2023-06-29 09:15:20.756674 pyaedt-0.6.86/pyaedt/modules/SetupTemplates.py
+-rw-r--r--   0        0        0   121445 2023-06-15 12:26:55.582508 pyaedt-0.6.86/pyaedt/modules/SolveSetup.py
+-rw-r--r--   0        0        0    33257 2023-05-30 06:59:39.674599 pyaedt-0.6.86/pyaedt/modules/SolveSweeps.py
+-rw-r--r--   0        0        0        0 2023-05-30 06:59:39.674599 pyaedt-0.6.86/pyaedt/modules/__init__.py
+-rw-r--r--   0        0        0    30706 2023-06-26 13:01:22.142566 pyaedt-0.6.86/pyaedt/modules/monitor_icepak.py
+-rw-r--r--   0        0        0   103333 2023-05-30 06:59:39.674599 pyaedt-0.6.86/pyaedt/modules/report_templates.py
+-rw-r--r--   0        0        0   126124 2023-06-23 15:25:31.221272 pyaedt-0.6.86/pyaedt/modules/solutions.py
+-rw-r--r--   0        0        0    95976 2023-07-21 09:35:13.260260 pyaedt-0.6.86/pyaedt/q3d.py
+-rw-r--r--   0        0        0    10581 2023-07-21 09:35:13.260260 pyaedt-0.6.86/pyaedt/rmxprt.py
+-rw-r--r--   0        0        0        0 2023-05-30 06:59:39.690227 pyaedt-0.6.86/pyaedt/rpc/__init__.py
+-rw-r--r--   0        0        0      415 2023-05-30 06:59:39.690227 pyaedt-0.6.86/pyaedt/rpc/local_server.py
+-rw-r--r--   0        0        0    40721 2023-05-30 06:59:39.690227 pyaedt-0.6.86/pyaedt/rpc/rpyc_services.py
+-rw-r--r--   0        0        0        0 2023-05-30 06:59:39.690227 pyaedt-0.6.86/pyaedt/sbrplus/__init__.py
+-rw-r--r--   0        0        0     9425 2023-05-30 06:59:39.690227 pyaedt-0.6.86/pyaedt/sbrplus/hdm_parser.py
+-rw-r--r--   0        0        0     2096 2023-05-30 06:59:39.690227 pyaedt-0.6.86/pyaedt/sbrplus/hdm_utils.py
+-rw-r--r--   0        0        0     2607 2023-05-30 06:59:39.690227 pyaedt-0.6.86/pyaedt/sbrplus/matlab/HdmObject.m
+-rw-r--r--   0        0        0       97 2023-05-30 06:59:39.690227 pyaedt-0.6.86/pyaedt/sbrplus/matlab/README.md
+-rw-r--r--   0        0        0      735 2023-05-30 06:59:39.690227 pyaedt-0.6.86/pyaedt/sbrplus/matlab/SbrBounceType.m
+-rw-r--r--   0        0        0     2886 2023-05-30 06:59:39.690227 pyaedt-0.6.86/pyaedt/sbrplus/matlab/StopWatch.m
+-rw-r--r--   0        0        0     1402 2023-05-30 06:59:39.690227 pyaedt-0.6.86/pyaedt/sbrplus/matlab/add_3dlight.m
+-rw-r--r--   0        0        0      340 2023-05-30 06:59:39.690227 pyaedt-0.6.86/pyaedt/sbrplus/matlab/amp2db.m
+-rw-r--r--   0        0        0    36837 2023-05-30 06:59:39.690227 pyaedt-0.6.86/pyaedt/sbrplus/matlab/draw_rays1.m
+-rw-r--r--   0        0        0     4322 2023-05-30 06:59:39.690227 pyaedt-0.6.86/pyaedt/sbrplus/matlab/draw_wfobj.m
+-rw-r--r--   0        0        0    31414 2023-05-30 06:59:39.690227 pyaedt-0.6.86/pyaedt/sbrplus/matlab/filter_rays1.m
+-rw-r--r--   0        0        0     1504 2023-05-30 06:59:39.690227 pyaedt-0.6.86/pyaedt/sbrplus/matlab/filtered_tracks.m
+-rw-r--r--   0        0        0    20853 2023-05-30 06:59:39.690227 pyaedt-0.6.86/pyaedt/sbrplus/matlab/ld_sbrplushdm.m
+-rw-r--r--   0        0        0    14781 2023-05-30 06:59:39.690227 pyaedt-0.6.86/pyaedt/sbrplus/matlab/ld_wfobj.m
+-rw-r--r--   0        0        0      318 2023-05-30 06:59:39.690227 pyaedt-0.6.86/pyaedt/sbrplus/matlab/pwr2db.m
+-rw-r--r--   0        0        0     2607 2023-05-30 06:59:39.690227 pyaedt-0.6.86/pyaedt/sbrplus/matlab/validate_sfields.m
+-rw-r--r--   0        0        0     7632 2023-05-30 06:59:39.690227 pyaedt-0.6.86/pyaedt/sbrplus/plot.py
+-rw-r--r--   0        0        0    10410 2023-06-05 09:36:43.953828 pyaedt-0.6.86/pyaedt/siwave.py
+-rw-r--r--   0        0        0    10527 2023-07-21 09:35:13.260260 pyaedt-0.6.86/pyaedt/twinbuilder.py
+-rw-r--r--   0        0        0     4556 2023-07-21 14:33:51.388714 pyaedt-0.6.86/pyproject.toml
+-rw-r--r--   0        0        0    15772 1970-01-01 00:00:00.000000 pyaedt-0.6.86/PKG-INFO
```

### Comparing `pyaedt-0.6.85/LICENSE` & `pyaedt-0.6.86/LICENSE`

 * *Files identical despite different names*

### Comparing `pyaedt-0.6.85/README.md` & `pyaedt-0.6.86/README.md`

 * *Files identical despite different names*

### Comparing `pyaedt-0.6.85/pyaedt/__init__.py` & `pyaedt-0.6.86/pyaedt/__init__.py`

 * *Files 10% similar despite different names*

```diff
@@ -8,15 +8,15 @@
 os.environ["ANSYSEM_FEATURE_SF159726_SCRIPTOBJECT_ENABLE"] = "1"
 os.environ["ANSYSEM_FEATURE_SF222134_CABLE_MODELING_ENHANCEMENTS_ENABLE"] = "1"
 os.environ["ANSYSEM_FEATURE_F395486_RIGID_FLEX_BENDING_ENABLE"] = "1"
 os.environ["ANSYSEM_FEATURE_S432616_LAYOUT_COMPONENT_IN_3D_ENABLE"] = "1"
 
 pyaedt_path = os.path.dirname(__file__)
 
-__version__ = "0.6.85"
+__version__ = "0.6.86"
 
 version = __version__
 import pyaedt.downloads as downloads
 from pyaedt.generic import constants
 import pyaedt.generic.DataHandlers as data_handler
 import pyaedt.generic.general_methods as general_methods
 
@@ -30,16 +30,14 @@
 from pyaedt.generic.general_methods import is_ironpython
 from pyaedt.generic.general_methods import is_linux
 from pyaedt.generic.general_methods import is_windows
 from pyaedt.generic.general_methods import online_help
 from pyaedt.generic.general_methods import pyaedt_function_handler
 from pyaedt.generic.general_methods import settings
 
-from pyaedt.aedt_logger import pyaedt_logger  # isort:skip
-
 try:
     from pyaedt.generic.design_types import Hfss3dLayout
 except:
     from pyaedt.generic.design_types import Hfss3dLayout
 
 from pyaedt.generic.design_types import Circuit
 from pyaedt.generic.design_types import Desktop
```

### Comparing `pyaedt-0.6.85/pyaedt/aedt_logger.py` & `pyaedt-0.6.86/pyaedt/aedt_logger.py`

 * *Files identical despite different names*

### Comparing `pyaedt-0.6.85/pyaedt/application/AEDT_File_Management.py` & `pyaedt-0.6.86/pyaedt/application/AEDT_File_Management.py`

 * *Files identical despite different names*

### Comparing `pyaedt-0.6.85/pyaedt/application/Analysis.py` & `pyaedt-0.6.86/pyaedt/application/Analysis.py`

 * *Files 0% similar despite different names*

```diff
@@ -1522,15 +1522,15 @@
 
         return self.analyze(self.active_setup, num_cores, num_tasks, num_gpu, acf_file, use_auto_settings)
 
     @pyaedt_function_handler()
     def analyze(
         self,
         setup_name=None,
-        num_cores=1,
+        num_cores=4,
         num_tasks=1,
         num_gpu=1,
         acf_file=None,
         use_auto_settings=True,
         solve_in_batch=False,
         machine="localhost",
         run_in_thread=False,
@@ -1540,15 +1540,15 @@
         """Solve the active design.
 
         Parameters
         ----------
         setup_name : str, optional
             Setup to analyze. Default is ``None`` which solves all the setups.
         num_cores : int, optional
-            Number of simulation cores. Default is ``1``.
+            Number of simulation cores. Default is ``4`` which is the number of cores available in license.
         num_tasks : int, optional
             Number of simulation tasks. Default is ``1``.
             In bach solve, set num_tasks to ``-1`` to apply auto settings and distributed mode.
         num_gpu : int, optional
             Number of simulation graphic processing units to use. Default is ``0``.
         acf_file : str, optional
             Full path to the custom ACF file.
@@ -1600,15 +1600,15 @@
                 blocking=blocking,
             )
 
     @pyaedt_function_handler()
     def analyze_setup(
         self,
         name,
-        num_cores=1,
+        num_cores=4,
         num_tasks=1,
         num_gpu=0,
         acf_file=None,
         use_auto_settings=True,
         num_variations_to_distribute=None,
         allowed_distribution_types=None,
         revert_to_initial_mesh=False,
```

### Comparing `pyaedt-0.6.85/pyaedt/application/Analysis3D.py` & `pyaedt-0.6.86/pyaedt/application/Analysis3D.py`

 * *Files identical despite different names*

### Comparing `pyaedt-0.6.85/pyaedt/application/Analysis3DLayout.py` & `pyaedt-0.6.86/pyaedt/application/Analysis3DLayout.py`

 * *Files identical despite different names*

### Comparing `pyaedt-0.6.85/pyaedt/application/AnalysisMaxwellCircuit.py` & `pyaedt-0.6.86/pyaedt/application/AnalysisMaxwellCircuit.py`

 * *Files identical despite different names*

### Comparing `pyaedt-0.6.85/pyaedt/application/AnalysisNexxim.py` & `pyaedt-0.6.86/pyaedt/application/AnalysisNexxim.py`

 * *Files 2% similar despite different names*

```diff
@@ -331,15 +331,15 @@
         -------
         list of str
             List of strings representing the S parameters of the excitations.
             For example, ``"S(1,1)", "S(1,2)", "S(2,2)"``.
 
         """
         if not excitation_names:
-            excitation_names = self.excitations
+            excitation_names = list(self.excitations.keys())
         spar = []
         k = 0
         for i in excitation_names:
             k = excitation_names.index(i)
             while k < len(excitation_names):
                 spar.append("S({},{})".format(i, excitation_names[k]))
                 k += 1
@@ -369,15 +369,15 @@
 
         >>> oEditor.GetAllPorts
         """
         if excitation_names == None:
             excitation_names = []
 
         if not excitation_names:
-            excitation_names = self.excitations
+            excitation_names = list(self.excitations.keys())
         if excitation_name_prefix:
             excitation_names = [i for i in excitation_names if excitation_name_prefix.lower() in i.lower()]
         spar = []
         for i in excitation_names:
             spar.append("S({},{})".format(i, i))
         return spar
 
@@ -411,17 +411,17 @@
         if trlist == None:
             trlist = []
         if reclist == None:
             reclist = []
 
         spar = []
         if not trlist:
-            trlist = [i for i in self.excitations if tx_prefix in i]
+            trlist = [i for i in list(self.excitations.keys()) if tx_prefix in i]
         if not reclist:
-            reclist = [i for i in self.excitations if rx_prefix in i]
+            reclist = [i for i in list(self.excitations.keys()) if rx_prefix in i]
         if len(trlist) != len(reclist):
             self.logger.error("The TX and RX lists should be the same length.")
             return False
         for i, j in zip(trlist, reclist):
             spar.append("S({},{})".format(i, j))
         return spar
 
@@ -446,15 +446,15 @@
         References
         ----------
 
         >>> oEditor.GetAllPorts
         """
         next = []
         if not trlist:
-            trlist = [i for i in self.excitations if tx_prefix in i]
+            trlist = [i for i in list(self.excitations.keys()) if tx_prefix in i]
         for i in trlist:
             k = trlist.index(i) + 1
             while k < len(trlist):
                 next.append("S({},{})".format(i, trlist[k]))
                 k += 1
         return next
 
@@ -494,17 +494,17 @@
         if trlist == None:
             trlist = []
         if reclist == None:
             reclist = []
 
         fext = []
         if not trlist:
-            trlist = [i for i in self.excitations if tx_prefix in i]
+            trlist = [i for i in list(self.excitations.keys()) if tx_prefix in i]
         if not reclist:
-            reclist = [i for i in self.excitations if rx_prefix in i]
+            reclist = [i for i in list(self.excitations.keys()) if rx_prefix in i]
         for i in trlist:
             for k in reclist:
                 if not skip_same_index_couples or reclist.index(k) != trlist.index(i):
                     fext.append("S({},{})".format(i, k))
         return fext
 
     @pyaedt_function_handler()
```

### Comparing `pyaedt-0.6.85/pyaedt/application/AnalysisRMxprt.py` & `pyaedt-0.6.86/pyaedt/application/AnalysisRMxprt.py`

 * *Files identical despite different names*

### Comparing `pyaedt-0.6.85/pyaedt/application/AnalysisTwinBuilder.py` & `pyaedt-0.6.86/pyaedt/application/AnalysisTwinBuilder.py`

 * *Files identical despite different names*

### Comparing `pyaedt-0.6.85/pyaedt/application/Design.py` & `pyaedt-0.6.86/pyaedt/application/Design.py`

 * *Files 0% similar despite different names*

```diff
@@ -17,15 +17,15 @@
 import shutil
 import string
 import sys
 import threading
 import time
 import warnings
 
-from pyaedt import pyaedt_logger
+from pyaedt.aedt_logger import pyaedt_logger
 from pyaedt.application.Variables import DataSet
 from pyaedt.application.Variables import VariableManager
 from pyaedt.application.Variables import decompose_variable_value
 from pyaedt.application.aedt_objects import AedtObjects
 from pyaedt.application.design_solutions import DesignSolution
 from pyaedt.application.design_solutions import HFSSDesignSolution
 from pyaedt.application.design_solutions import IcepakDesignSolution
@@ -1135,17 +1135,17 @@
                     self._add_handler()
                     self.logger.info("Project %s has been opened.", self._oproject.GetName())
                     time.sleep(0.5)
             elif settings.force_error_on_missing_project and ".aedt" in proj_name:
                 raise Exception("Project doesn't exists. Check it and retry.")
             else:
                 self._oproject = self.odesktop.NewProject()
-                if ".aedt" in proj_name:
+                if proj_name.endswith(".aedt"):
                     self._oproject.Rename(proj_name, True)
-                else:
+                elif not proj_name.endswith(".aedtz"):
                     self._oproject.Rename(os.path.join(self.project_path, proj_name + ".aedt"), True)
                 self._add_handler()
                 self.logger.info("Project %s has been created.", self._oproject.GetName())
         if not self._oproject:
             self._oproject = self.odesktop.NewProject()
             self._add_handler()
             self.logger.info("Project %s has been created.", self._oproject.GetName())
@@ -3900,7 +3900,24 @@
         str
             Project name if loaded in Desktop.
         """
         for p in self.odesktop.GetProjects():
             if os.path.normpath(os.path.join(p.GetPath(), p.GetName()) + ".aedt") == os.path.normpath(project_path):
                 return p.GetName()
         return False
+
+    @pyaedt_function_handler
+    def set_temporary_directory(self, temp_dir_path):
+        """Set temporary directory path.
+
+        Returns
+        -------
+        bool
+            ``True`` when successful, ``False`` when failed.
+
+        References
+        ----------
+
+        >>> oDesktop.SetTempDirectory()
+        """
+        self.odesktop.SetTempDirectory(temp_dir_path)
+        return True
```

### Comparing `pyaedt-0.6.85/pyaedt/application/JobManager.py` & `pyaedt-0.6.86/pyaedt/application/JobManager.py`

 * *Files identical despite different names*

### Comparing `pyaedt-0.6.85/pyaedt/application/Variables.py` & `pyaedt-0.6.86/pyaedt/application/Variables.py`

 * *Files 0% similar despite different names*

```diff
@@ -253,15 +253,15 @@
 
 @pyaedt_function_handler()
 def decompose_variable_value(variable_value, full_variables={}):
     """Decompose a variable value.
 
     Parameters
     ----------
-    variable_value : float
+    variable_value : str
     full_variables : dict
 
     Returns
     -------
     tuples
         tuples made of the float value of the variable and the units exposed as a string.
     """
@@ -1192,23 +1192,30 @@
         return False
 
     @pyaedt_function_handler()
     def _get_var_list_from_aedt(self, desktop_object):
         var_list = []
         if self._app._is_object_oriented_enabled() and self._app.design_type != "Maxwell Circuit":
             # To retrieve local variables
-            var_list += list(self._app.get_oo_object(self._app.odesign, "LocalVariables").GetPropNames())
+            try:
+                v = list(self._app.get_oo_object(self._app.odesign, "LocalVariables").GetPropNames())
+            except AttributeError:
+                v = []
+            var_list += v
         if self._app._is_object_oriented_enabled() and self._app.design_type in [
             "Circuit Design",
             "Twin Builder",
             "HFSS 3D Layout Design",
         ]:
             # To retrieve Parameter Default Variables
-            var_list += list(self._app.get_oo_object(self._app.odesign, "DefinitionParameters").GetPropNames())
-
+            try:
+                v = list(self._app.get_oo_object(self._app.odesign, "DefinitionParameters").GetPropNames())
+            except AttributeError:
+                v = []
+            var_list += v
         var_list += [i for i in list(desktop_object.GetVariables()) if i not in var_list]
         var_list += [i for i in list(self._app.oproject.GetArrayVariables()) if i not in var_list]
         return var_list
 
 
 class Variable(object):
     """Stores design properties and project variables and provides operations to perform on them.
```

### Comparing `pyaedt-0.6.85/pyaedt/application/aedt_objects.py` & `pyaedt-0.6.86/pyaedt/application/aedt_objects.py`

 * *Files identical despite different names*

### Comparing `pyaedt-0.6.85/pyaedt/application/design_solutions.py` & `pyaedt-0.6.86/pyaedt/application/design_solutions.py`

 * *Files identical despite different names*

### Comparing `pyaedt-0.6.85/pyaedt/circuit.py` & `pyaedt-0.6.86/pyaedt/circuit.py`

 * *Files identical despite different names*

### Comparing `pyaedt-0.6.85/pyaedt/common_rpc.py` & `pyaedt-0.6.86/pyaedt/common_rpc.py`

 * *Files 0% similar despite different names*

```diff
@@ -2,16 +2,16 @@
 import signal
 import socket
 import sys
 import tempfile
 import time
 
 from pyaedt import is_ironpython
-from pyaedt import pyaedt_logger as logger
 from pyaedt import settings
+from pyaedt.aedt_logger import pyaedt_logger as logger
 from pyaedt.misc import list_installed_ansysem
 
 # import sys
 from pyaedt.rpc.rpyc_services import FileManagement
 from pyaedt.rpc.rpyc_services import GlobalService
 from pyaedt.rpc.rpyc_services import ServiceManager
 from pyaedt.rpc.rpyc_services import check_port
```

### Comparing `pyaedt-0.6.85/pyaedt/desktop.py` & `pyaedt-0.6.86/pyaedt/desktop.py`

 * *Files 0% similar despite different names*

```diff
@@ -21,15 +21,15 @@
 import time
 import traceback
 import warnings
 
 from pyaedt import is_ironpython
 from pyaedt import is_linux
 from pyaedt import is_windows
-from pyaedt import pyaedt_logger
+from pyaedt.aedt_logger import pyaedt_logger
 from pyaedt.generic.general_methods import generate_unique_name
 
 if is_linux:
     os.environ["ANS_NODEPCHECK"] = str(1)
 
 if is_linux and is_ironpython:
     import subprocessdotnet as subprocess
@@ -239,32 +239,33 @@
     except AttributeError:
         pass
     try:
         del module.AEDTVersion
     except AttributeError:
         pass
     try:
-        del sys.modules["PyDesktopPluginDll"]
-    except:
-        pass
-    try:
-        del sys.modules["PyDesktopPlugin"]
-    except:
-        pass
-    try:
         del sys.modules["glob"]
     except:
         pass
-    keys = [k for k in sys.modules.keys()]
-    for i in keys:
-        if "Ansys.Ansoft" in i:
-            del sys.modules[i]
-    for p in sys.path[::-1]:
-        if "AnsysEM" in p:
-            del sys.path[sys.path.index(p)]
+    # try:
+    #     del sys.modules["PyDesktopPluginDll"]
+    # except:
+    #     pass
+    # try:
+    #     del sys.modules["PyDesktopPlugin"]
+    # except:
+    #     pass
+
+    # keys = [k for k in sys.modules.keys()]
+    # for i in keys:
+    #     if "Ansys.Ansoft" in i:
+    #         del sys.modules[i]
+    # for p in sys.path[::-1]:
+    #     if "AnsysEM" in p:
+    #         del sys.path[sys.path.index(p)]
     gc.collect()
 
 
 @pyaedt_function_handler()
 def release_desktop(close_projects=True, close_desktop=True):
     """Release the AEDT API.
 
@@ -292,14 +293,15 @@
                 desktop.CloseProject(project)
         if settings.remote_rpc_session or (
             settings.aedt_version >= "2022.2" and settings.use_grpc_api and not is_ironpython
         ):
             try:
                 if close_desktop:
                     _main.oDesktop.QuitApplication()
+                    _main.oDesktop.QuitApplication()
                 else:
                     import pyaedt.generic.grpc_plugin as StandalonePyScriptWrapper
 
                     return StandalonePyScriptWrapper.Release()
             except:
                 pass
             _delete_objects()
@@ -1655,17 +1657,14 @@
             Full path to the image logo (a 30x30 pixel PNG file) to add to the UI.
             The default is ``None``.
         product : str, optional
             Product to which the toolkit applies. The default is ``"Project"``, in which case
             it applies to all designs. You can also specify a product, such as ``"HFSS"``.
         copy_to_personal_lib : bool, optional
             Whether to copy the script to Personal Lib or link the original script. Default is ``True``.
-        add_pyaedt_desktop_init : bool, optional
-            Whether to add Desktop initialization to the script or not.
-            This is needed to reference the Desktop which is launching the script.
 
         Returns
         -------
         bool
 
         """
         if not os.path.exists(script_path):
```

### Comparing `pyaedt-0.6.85/pyaedt/dlls/PDFReport/AnsysReport.deps.json` & `pyaedt-0.6.86/pyaedt/dlls/PDFReport/AnsysReport.deps.json`

 * *Files identical despite different names*

### Comparing `pyaedt-0.6.85/pyaedt/dlls/PDFReport/AnsysReport.dll` & `pyaedt-0.6.86/pyaedt/dlls/PDFReport/AnsysReport.dll`

 * *Files identical despite different names*

### Comparing `pyaedt-0.6.85/pyaedt/dlls/PDFReport/AnsysTemplate.json` & `pyaedt-0.6.86/pyaedt/dlls/PDFReport/AnsysTemplate.json`

 * *Files identical despite different names*

### Comparing `pyaedt-0.6.85/pyaedt/dlls/PDFReport/ICSharpCode.SharpZipLib.dll` & `pyaedt-0.6.86/pyaedt/dlls/PDFReport/ICSharpCode.SharpZipLib.dll`

 * *Files identical despite different names*

### Comparing `pyaedt-0.6.85/pyaedt/dlls/PDFReport/ICSharpCode.SharpZipLib.xml` & `pyaedt-0.6.86/pyaedt/dlls/PDFReport/ICSharpCode.SharpZipLib.xml`

 * *Files identical despite different names*

### Comparing `pyaedt-0.6.85/pyaedt/dlls/PDFReport/Images/Ansys.png` & `pyaedt-0.6.86/pyaedt/dlls/PDFReport/Images/Ansys.png`

 * *Files identical despite different names*

### Comparing `pyaedt-0.6.85/pyaedt/dlls/PDFReport/MigraDocCore.DocumentObjectModel.dll` & `pyaedt-0.6.86/pyaedt/dlls/PDFReport/MigraDocCore.DocumentObjectModel.dll`

 * *Files identical despite different names*

### Comparing `pyaedt-0.6.85/pyaedt/dlls/PDFReport/MigraDocCore.Rendering.dll` & `pyaedt-0.6.86/pyaedt/dlls/PDFReport/MigraDocCore.Rendering.dll`

 * *Files identical despite different names*

### Comparing `pyaedt-0.6.85/pyaedt/dlls/PDFReport/Newtonsoft.Json.dll` & `pyaedt-0.6.86/pyaedt/dlls/PDFReport/Newtonsoft.Json.dll`

 * *Files identical despite different names*

### Comparing `pyaedt-0.6.85/pyaedt/dlls/PDFReport/Newtonsoft.Json.xml` & `pyaedt-0.6.86/pyaedt/dlls/PDFReport/Newtonsoft.Json.xml`

 * *Files identical despite different names*

### Comparing `pyaedt-0.6.85/pyaedt/dlls/PDFReport/PdfSharpCore.Charting.dll` & `pyaedt-0.6.86/pyaedt/dlls/PDFReport/PdfSharpCore.Charting.dll`

 * *Files identical despite different names*

### Comparing `pyaedt-0.6.85/pyaedt/dlls/PDFReport/PdfSharpCore.dll` & `pyaedt-0.6.86/pyaedt/dlls/PDFReport/PdfSharpCore.dll`

 * *Files identical despite different names*

### Comparing `pyaedt-0.6.85/pyaedt/dlls/PDFReport/SixLabors.Fonts.dll` & `pyaedt-0.6.86/pyaedt/dlls/PDFReport/SixLabors.Fonts.dll`

 * *Files identical despite different names*

### Comparing `pyaedt-0.6.85/pyaedt/dlls/PDFReport/SixLabors.Fonts.xml` & `pyaedt-0.6.86/pyaedt/dlls/PDFReport/SixLabors.Fonts.xml`

 * *Files identical despite different names*

### Comparing `pyaedt-0.6.85/pyaedt/dlls/PDFReport/SixLabors.ImageSharp.dll` & `pyaedt-0.6.86/pyaedt/dlls/PDFReport/SixLabors.ImageSharp.dll`

 * *Files identical despite different names*

### Comparing `pyaedt-0.6.85/pyaedt/dlls/PDFReport/SixLabors.ImageSharp.xml` & `pyaedt-0.6.86/pyaedt/dlls/PDFReport/SixLabors.ImageSharp.xml`

 * *Files identical despite different names*

### Comparing `pyaedt-0.6.85/pyaedt/dlls/PDFReport/System.Runtime.dll` & `pyaedt-0.6.86/pyaedt/dlls/PDFReport/System.Runtime.dll`

 * *Files identical despite different names*

### Comparing `pyaedt-0.6.85/pyaedt/dlls/PDFReport/System.Runtime.xml` & `pyaedt-0.6.86/pyaedt/dlls/PDFReport/System.Runtime.xml`

 * *Files identical despite different names*

### Comparing `pyaedt-0.6.85/pyaedt/dlls/PDFReport/de/PdfSharpCore.resources.dll` & `pyaedt-0.6.86/pyaedt/dlls/PDFReport/de/PdfSharpCore.resources.dll`

 * *Files identical despite different names*

### Comparing `pyaedt-0.6.85/pyaedt/dlls/PDFReport/de/System.Collections.NonGeneric.xml` & `pyaedt-0.6.86/pyaedt/dlls/PDFReport/de/System.Collections.NonGeneric.xml`

 * *Files identical despite different names*

### Comparing `pyaedt-0.6.85/pyaedt/downloads.py` & `pyaedt-0.6.86/pyaedt/downloads.py`

 * *Files 2% similar despite different names*

```diff
@@ -139,14 +139,15 @@
         _retrieve_file(url, filename, directory, destination, local_paths)
     if settings.remote_rpc_session:
         remote_path = os.path.join(settings.remote_rpc_session_temp_folder, os.path.split(local_paths[-1])[-1])
         if not settings.remote_rpc_session.filemanager.pathexists(settings.remote_rpc_session_temp_folder):
             settings.remote_rpc_session.filemanager.makedirs(settings.remote_rpc_session_temp_folder)
         settings.remote_rpc_session.filemanager.upload(local_paths[-1], remote_path)
         local_paths[-1] = remote_path
+    return local_paths[-1]
 
 
 ###############################################################################
 # front-facing functions
 
 
 def download_aedb(destination=None):
@@ -172,15 +173,15 @@
     >>> path = pyaedt.downloads.download_aedb()
     >>> path
     'C:/Users/user/AppData/local/temp/Galileo.aedb'
     """
     local_paths = []
     _download_file("pyaedt/edb/Galileo.aedb", "GRM32ER72A225KA35_25C_0V.sp", destination, local_paths)
     _download_file("pyaedt/edb/Galileo.aedb", "edb.def", destination, local_paths)
-    return local_paths
+    return local_paths[-1]
 
 
 def download_edb_merge_utility(force_download=False, destination=None):
     """Download an example of WPF Project which allows to merge 2aedb files.
 
     Examples files are downloaded to a persistent cache to avoid
     re-downloading the same file twice.
@@ -362,15 +363,15 @@
     Download an example result file and return the path of the file.
 
     >>> import pyaedt
     >>> path = pyaedt.downloads.download_icepak()
     >>> pathavoid
     'C:/Users/user/AppData/local/temp/pyaedtexamples/Graphic_Card.aedt'
     """
-
+    _download_file("pyaedt/icepak", "Graphics_card.aedt", destination)
     return _download_file("pyaedt/icepak", "Graphics_card.aedt", destination)
 
 
 def download_icepak_3d_component(destination=None):  # pragma: no cover
     """Download an example of Icepak Array and return the def pathsw.
 
     Examples files are downloaded to a persistent cache to avoid
@@ -455,15 +456,15 @@
     >>> import pyaedt
     >>> path = pyaedt.downloads.download_touchstone()
     >>> path
     'C:/Users/user/AppData/local/temp/pyaedtexamples/ssn_ssn.s6p'
     """
     local_paths = []
     _download_file("pyaedt/touchstone", "SSN_ssn.s6p", destination, local_paths)
-    return local_paths
+    return local_paths[0]
 
 
 def download_sherlock(destination=None):
     """Download an example of sherlock needed files and return the def path.
 
     Examples files are downloaded to a persistent cache to avoid
     re-downloading the same file twice.
@@ -526,15 +527,15 @@
     """
     if not destination:
         destination = EXAMPLES_PATH
     local_paths = []
     _download_file("pyaedt/nissan", "30DH_20C_smooth.tab", destination, local_paths)
     _download_file("pyaedt/nissan", "BH_Arnold_Magnetics_N30UH_80C.tab", destination, local_paths)
 
-    return local_paths
+    return local_paths[0], local_paths[1]
 
 
 def download_custom_reports(force_download=False, destination=None):
     """Download an example of CISPR25 with customer reports json template files.
 
     Examples files are downloaded to a persistent cache to avoid
     re-downloading the same file twice.
@@ -555,22 +556,22 @@
     --------
     Download an example result file and return the path of the file.
     >>> import pyaedt
     >>> path = pyaedt.downloads.download_custom_reports(force_download=True)
     >>> path
     'C:/Users/user/AppData/local/temp/custom_reports'
     """
-
+    if not destination:
+        destination = EXAMPLES_PATH
     if force_download:
         local_path = os.path.join(destination, "custom_reports")
         if os.path.exists(local_path):
             shutil.rmtree(local_path, ignore_errors=True)
-    download_file("pyaedt/custom_reports")
-    if not destination:
-        destination = EXAMPLES_PATH
+    download_file("pyaedt/custom_reports", destination=destination)
+
     return os.path.join(destination, "custom_reports")
 
 
 def download_3dcomponent(force_download=False, destination=None):
     """Download an example of 3d component array with json template files.
 
     Examples files are downloaded to a persistent cache to avoid
```

### Comparing `pyaedt-0.6.85/pyaedt/edb.py` & `pyaedt-0.6.86/pyaedt/edb.py`

 * *Files identical despite different names*

### Comparing `pyaedt-0.6.85/pyaedt/edb_core/components.py` & `pyaedt-0.6.86/pyaedt/edb_core/components.py`

 * *Files identical despite different names*

### Comparing `pyaedt-0.6.85/pyaedt/edb_core/dotnet/database.py` & `pyaedt-0.6.86/pyaedt/edb_core/dotnet/database.py`

 * *Files 0% similar despite different names*

```diff
@@ -1,14 +1,14 @@
 """Database."""
 import os
 import re
 import sys
 
 from pyaedt import __version__
-from pyaedt import pyaedt_logger
+from pyaedt.aedt_logger import pyaedt_logger
 from pyaedt.edb_core.general import convert_py_list_to_net_list
 from pyaedt.generic.general_methods import env_path
 from pyaedt.generic.general_methods import env_path_student
 from pyaedt.generic.general_methods import env_value
 from pyaedt.generic.general_methods import is_ironpython
 from pyaedt.generic.general_methods import is_linux
 from pyaedt.generic.general_methods import settings
```

### Comparing `pyaedt-0.6.85/pyaedt/edb_core/dotnet/layout.py` & `pyaedt-0.6.86/pyaedt/edb_core/dotnet/layout.py`

 * *Files identical despite different names*

### Comparing `pyaedt-0.6.85/pyaedt/edb_core/dotnet/primitive.py` & `pyaedt-0.6.86/pyaedt/edb_core/dotnet/primitive.py`

 * *Files identical despite different names*

### Comparing `pyaedt-0.6.85/pyaedt/edb_core/edb_data/components_data.py` & `pyaedt-0.6.86/pyaedt/edb_core/edb_data/components_data.py`

 * *Files identical despite different names*

### Comparing `pyaedt-0.6.85/pyaedt/edb_core/edb_data/control_file.py` & `pyaedt-0.6.86/pyaedt/edb_core/edb_data/control_file.py`

 * *Files 0% similar despite different names*

```diff
@@ -1,13 +1,13 @@
 import copy
 import os
 import re
 import sys
 
-from pyaedt import pyaedt_logger
+from pyaedt.aedt_logger import pyaedt_logger
 
 # from pyaedt.generic.general_methods import property
 from pyaedt.generic.general_methods import ET
 from pyaedt.generic.general_methods import env_path
 from pyaedt.generic.general_methods import env_value
 from pyaedt.generic.general_methods import is_ironpython
 from pyaedt.generic.general_methods import is_linux
```

### Comparing `pyaedt-0.6.85/pyaedt/edb_core/edb_data/design_options.py` & `pyaedt-0.6.86/pyaedt/edb_core/edb_data/design_options.py`

 * *Files identical despite different names*

### Comparing `pyaedt-0.6.85/pyaedt/edb_core/edb_data/edbvalue.py` & `pyaedt-0.6.86/pyaedt/edb_core/edb_data/edbvalue.py`

 * *Files identical despite different names*

### Comparing `pyaedt-0.6.85/pyaedt/edb_core/edb_data/hfss_extent_info.py` & `pyaedt-0.6.86/pyaedt/edb_core/edb_data/hfss_extent_info.py`

 * *Files identical despite different names*

### Comparing `pyaedt-0.6.85/pyaedt/edb_core/edb_data/hfss_simulation_setup_data.py` & `pyaedt-0.6.86/pyaedt/edb_core/edb_data/hfss_simulation_setup_data.py`

 * *Files identical despite different names*

### Comparing `pyaedt-0.6.85/pyaedt/edb_core/edb_data/layer_data.py` & `pyaedt-0.6.86/pyaedt/edb_core/edb_data/layer_data.py`

 * *Files 0% similar despite different names*

```diff
@@ -1,76 +1,22 @@
 from __future__ import absolute_import
 
 import re
 
-# from pyaedt import property
 from pyaedt import pyaedt_function_handler
 
 
 class LayerEdbClass(object):
     """Manages Edb Layers. Replaces EDBLayer."""
 
     def __init__(self, pclass, name):
         self._pclass = pclass
         self._name = name
         self._color = ()
         self._type = ""
-        self._material = ""
-        self._conductivity = 0.0
-        self._permittivity = 0.0
-        self._loss_tangent = 0.0
-        self._dielectric_fill = ""
-        self._thickness = 0.0
-        self._etch_factor = 0.0
-        self._roughness_enabled = False
-        self._top_hallhuray_nodule_radius = 0.5e-6
-        self._top_hallhuray_surface_ratio = 2.9
-        self._bottom_hallhuray_nodule_radius = 0.5e-6
-        self._bottom_hallhuray_surface_ratio = 2.9
-        self._side_hallhuray_nodule_radius = 0.5e-6
-        self._side_hallhuray_surface_ratio = 2.9
-        self._material = None
-        self._upper_elevation = 0.0
-        self._lower_elevation = 0.0
-
-    @property
-    def lower_elevation(self):
-        """Lower elevation.
-
-        Returns
-        -------
-        float
-            Lower elevation.
-        """
-        try:
-            self._lower_elevation = self._edb_layer.GetLowerElevation()
-        except:
-            pass
-        return self._lower_elevation
-
-    @lower_elevation.setter
-    def lower_elevation(self, value):
-        layer_clone = self._edb_layer
-        layer_clone.SetLowerElevation(self._pclass._edb_value(value))
-        self._pclass._set_layout_stackup(layer_clone, "change_attribute")
-
-    @property
-    def upper_elevation(self):
-        """Upper elevation.
-
-        Returns
-        -------
-        float
-            Upper elevation.
-        """
-        try:
-            self._upper_elevation = self._edb_layer.GetUpperElevation()
-        except:
-            pass
-        return self._upper_elevation
 
     @property
     def _edb(self):
         return self._pclass._pedb.edb_api
 
     @property
     def _edb_layer(self):
@@ -86,29 +32,23 @@
         -------
         bool
             True if this layer is a stackup layer, False otherwise.
         """
         return self._edb_layer.IsStackupLayer()
 
     @property
-    def is_negative(self):
-        """Determine whether this layer is a negative layer.
+    def is_via_layer(self):
+        """Determine whether this layer is a via layer.
 
         Returns
         -------
         bool
-            True if this layer is a negative layer, False otherwise.
+            True if this layer is a via layer, False otherwise.
         """
-        return self._edb_layer.GetNegative()
-
-    @is_negative.setter
-    def is_negative(self, value):
-        layer_clone = self._edb_layer
-        layer_clone.SetNegative(value)
-        self._pclass._set_layout_stackup(layer_clone, "change_attribute")
+        return self._edb_layer.IsViaLayer()
 
     @property
     def color(self):
         """Retrieve color of the layer.
 
         Returns
         -------
@@ -164,22 +104,95 @@
         """Retrieve type of the layer."""
         return re.sub(r"Layer$", "", self._edb_layer.GetLayerType().ToString()).lower()
 
     @type.setter
     def type(self, new_type):
         if new_type == self.type:
             return
+
+        layer_clone = self._edb_layer
         if new_type == "signal":
-            self._edb_layer.SetLayerType(self._edb.cell.layer_type.SignalLayer)
+            layer_clone.SetLayerType(self._edb.cell.layer_type.SignalLayer)
             self._type = new_type
         elif new_type == "dielectric":
-            self._edb_layer.SetLayerType(self._edb.cell.layer_type.DielectricLayer)
+            layer_clone.SetLayerType(self._edb.cell.layer_type.DielectricLayer)
             self._type = new_type
         else:
             return
+        self._pclass._set_layout_stackup(layer_clone, "change_attribute")
+
+
+class StackupLayerEdbClass(LayerEdbClass):
+    def __init__(self, pclass, name):
+        super().__init__(pclass, name)
+        self._material = ""
+        self._conductivity = 0.0
+        self._permittivity = 0.0
+        self._loss_tangent = 0.0
+        self._dielectric_fill = ""
+        self._thickness = 0.0
+        self._etch_factor = 0.0
+        self._roughness_enabled = False
+        self._top_hallhuray_nodule_radius = 0.5e-6
+        self._top_hallhuray_surface_ratio = 2.9
+        self._bottom_hallhuray_nodule_radius = 0.5e-6
+        self._bottom_hallhuray_surface_ratio = 2.9
+        self._side_hallhuray_nodule_radius = 0.5e-6
+        self._side_hallhuray_surface_ratio = 2.9
+        self._material = None
+        self._upper_elevation = 0.0
+        self._lower_elevation = 0.0
+
+    @property
+    def lower_elevation(self):
+        """Lower elevation.
+
+        Returns
+        -------
+        float
+            Lower elevation.
+        """
+        self._lower_elevation = self._edb_layer.GetLowerElevation()
+        return self._lower_elevation
+
+    @lower_elevation.setter
+    def lower_elevation(self, value):
+        if self._pclass.mode == "Overlapping":
+            layer_clone = self._edb_layer
+            layer_clone.SetLowerElevation(self._pclass._edb_value(value))
+            self._pclass._set_layout_stackup(layer_clone, "change_attribute")
+
+    @property
+    def upper_elevation(self):
+        """Upper elevation.
+
+        Returns
+        -------
+        float
+            Upper elevation.
+        """
+        self._upper_elevation = self._edb_layer.GetUpperElevation()
+        return self._upper_elevation
+
+    @property
+    def is_negative(self):
+        """Determine whether this layer is a negative layer.
+
+        Returns
+        -------
+        bool
+            True if this layer is a negative layer, False otherwise.
+        """
+        return self._edb_layer.GetNegative()
+
+    @is_negative.setter
+    def is_negative(self, value):
+        layer_clone = self._edb_layer
+        layer_clone.SetNegative(value)
+        self._pclass._set_layout_stackup(layer_clone, "change_attribute")
 
     @property
     def material(self):
         """Get/Set the material loss_tangent.
 
         Returns
         -------
```

### Comparing `pyaedt-0.6.85/pyaedt/edb_core/edb_data/nets_data.py` & `pyaedt-0.6.86/pyaedt/edb_core/edb_data/nets_data.py`

 * *Files identical despite different names*

### Comparing `pyaedt-0.6.85/pyaedt/edb_core/edb_data/padstacks_data.py` & `pyaedt-0.6.86/pyaedt/edb_core/edb_data/padstacks_data.py`

 * *Files identical despite different names*

### Comparing `pyaedt-0.6.85/pyaedt/edb_core/edb_data/primitives_data.py` & `pyaedt-0.6.86/pyaedt/edb_core/edb_data/primitives_data.py`

 * *Files identical despite different names*

### Comparing `pyaedt-0.6.85/pyaedt/edb_core/edb_data/simulation_configuration.py` & `pyaedt-0.6.86/pyaedt/edb_core/edb_data/simulation_configuration.py`

 * *Files identical despite different names*

### Comparing `pyaedt-0.6.85/pyaedt/edb_core/edb_data/siwave_simulation_setup_data.py` & `pyaedt-0.6.86/pyaedt/edb_core/edb_data/siwave_simulation_setup_data.py`

 * *Files identical despite different names*

### Comparing `pyaedt-0.6.85/pyaedt/edb_core/edb_data/sources.py` & `pyaedt-0.6.86/pyaedt/edb_core/edb_data/sources.py`

 * *Files identical despite different names*

### Comparing `pyaedt-0.6.85/pyaedt/edb_core/edb_data/utilities.py` & `pyaedt-0.6.86/pyaedt/edb_core/edb_data/utilities.py`

 * *Files identical despite different names*

### Comparing `pyaedt-0.6.85/pyaedt/edb_core/edb_data/variables.py` & `pyaedt-0.6.86/pyaedt/edb_core/edb_data/variables.py`

 * *Files identical despite different names*

### Comparing `pyaedt-0.6.85/pyaedt/edb_core/general.py` & `pyaedt-0.6.86/pyaedt/edb_core/general.py`

 * *Files identical despite different names*

### Comparing `pyaedt-0.6.85/pyaedt/edb_core/hfss.py` & `pyaedt-0.6.86/pyaedt/edb_core/hfss.py`

 * *Files identical despite different names*

### Comparing `pyaedt-0.6.85/pyaedt/edb_core/ipc2581/bom/bom.py` & `pyaedt-0.6.86/pyaedt/edb_core/ipc2581/bom/bom.py`

 * *Files identical despite different names*

### Comparing `pyaedt-0.6.85/pyaedt/edb_core/ipc2581/bom/bom_item.py` & `pyaedt-0.6.86/pyaedt/edb_core/ipc2581/bom/bom_item.py`

 * *Files identical despite different names*

### Comparing `pyaedt-0.6.85/pyaedt/edb_core/ipc2581/bom/characteristics.py` & `pyaedt-0.6.86/pyaedt/edb_core/ipc2581/bom/characteristics.py`

 * *Files identical despite different names*

### Comparing `pyaedt-0.6.85/pyaedt/edb_core/ipc2581/bom/refdes.py` & `pyaedt-0.6.86/pyaedt/edb_core/ipc2581/bom/refdes.py`

 * *Files identical despite different names*

### Comparing `pyaedt-0.6.85/pyaedt/edb_core/ipc2581/content/color.py` & `pyaedt-0.6.86/pyaedt/edb_core/ipc2581/content/color.py`

 * *Files identical despite different names*

### Comparing `pyaedt-0.6.85/pyaedt/edb_core/ipc2581/content/content.py` & `pyaedt-0.6.86/pyaedt/edb_core/ipc2581/content/content.py`

 * *Files identical despite different names*

### Comparing `pyaedt-0.6.85/pyaedt/edb_core/ipc2581/content/dictionary_color.py` & `pyaedt-0.6.86/pyaedt/edb_core/ipc2581/content/dictionary_color.py`

 * *Files identical despite different names*

### Comparing `pyaedt-0.6.85/pyaedt/edb_core/ipc2581/content/dictionary_fill.py` & `pyaedt-0.6.86/pyaedt/edb_core/ipc2581/content/dictionary_fill.py`

 * *Files identical despite different names*

### Comparing `pyaedt-0.6.85/pyaedt/edb_core/ipc2581/content/dictionary_line.py` & `pyaedt-0.6.86/pyaedt/edb_core/ipc2581/content/dictionary_line.py`

 * *Files identical despite different names*

### Comparing `pyaedt-0.6.85/pyaedt/edb_core/ipc2581/content/entry_line.py` & `pyaedt-0.6.86/pyaedt/edb_core/ipc2581/content/entry_line.py`

 * *Files identical despite different names*

### Comparing `pyaedt-0.6.85/pyaedt/edb_core/ipc2581/content/fill.py` & `pyaedt-0.6.86/pyaedt/edb_core/ipc2581/content/fill.py`

 * *Files identical despite different names*

### Comparing `pyaedt-0.6.85/pyaedt/edb_core/ipc2581/content/standard_geometries_dictionary.py` & `pyaedt-0.6.86/pyaedt/edb_core/ipc2581/content/standard_geometries_dictionary.py`

 * *Files identical despite different names*

### Comparing `pyaedt-0.6.85/pyaedt/edb_core/ipc2581/ecad/cad_data/assembly_drawing.py` & `pyaedt-0.6.86/pyaedt/edb_core/ipc2581/ecad/cad_data/assembly_drawing.py`

 * *Files identical despite different names*

### Comparing `pyaedt-0.6.85/pyaedt/edb_core/ipc2581/ecad/cad_data/cad_data.py` & `pyaedt-0.6.86/pyaedt/edb_core/ipc2581/ecad/cad_data/cad_data.py`

 * *Files identical despite different names*

### Comparing `pyaedt-0.6.85/pyaedt/edb_core/ipc2581/ecad/cad_data/component.py` & `pyaedt-0.6.86/pyaedt/edb_core/ipc2581/ecad/cad_data/component.py`

 * *Files identical despite different names*

### Comparing `pyaedt-0.6.85/pyaedt/edb_core/ipc2581/ecad/cad_data/drill.py` & `pyaedt-0.6.86/pyaedt/edb_core/ipc2581/ecad/cad_data/drill.py`

 * *Files identical despite different names*

### Comparing `pyaedt-0.6.85/pyaedt/edb_core/ipc2581/ecad/cad_data/feature.py` & `pyaedt-0.6.86/pyaedt/edb_core/ipc2581/ecad/cad_data/feature.py`

 * *Files identical despite different names*

### Comparing `pyaedt-0.6.85/pyaedt/edb_core/ipc2581/ecad/cad_data/layer.py` & `pyaedt-0.6.86/pyaedt/edb_core/ipc2581/ecad/cad_data/layer.py`

 * *Files identical despite different names*

### Comparing `pyaedt-0.6.85/pyaedt/edb_core/ipc2581/ecad/cad_data/layer_feature.py` & `pyaedt-0.6.86/pyaedt/edb_core/ipc2581/ecad/cad_data/layer_feature.py`

 * *Files identical despite different names*

### Comparing `pyaedt-0.6.85/pyaedt/edb_core/ipc2581/ecad/cad_data/logical_net.py` & `pyaedt-0.6.86/pyaedt/edb_core/ipc2581/ecad/cad_data/logical_net.py`

 * *Files identical despite different names*

### Comparing `pyaedt-0.6.85/pyaedt/edb_core/ipc2581/ecad/cad_data/outline.py` & `pyaedt-0.6.86/pyaedt/edb_core/ipc2581/ecad/cad_data/outline.py`

 * *Files identical despite different names*

### Comparing `pyaedt-0.6.85/pyaedt/edb_core/ipc2581/ecad/cad_data/package.py` & `pyaedt-0.6.86/pyaedt/edb_core/ipc2581/ecad/cad_data/package.py`

 * *Files identical despite different names*

### Comparing `pyaedt-0.6.85/pyaedt/edb_core/ipc2581/ecad/cad_data/padstack_def.py` & `pyaedt-0.6.86/pyaedt/edb_core/ipc2581/ecad/cad_data/padstack_def.py`

 * *Files identical despite different names*

### Comparing `pyaedt-0.6.85/pyaedt/edb_core/ipc2581/ecad/cad_data/padstack_hole_def.py` & `pyaedt-0.6.86/pyaedt/edb_core/ipc2581/ecad/cad_data/padstack_hole_def.py`

 * *Files identical despite different names*

### Comparing `pyaedt-0.6.85/pyaedt/edb_core/ipc2581/ecad/cad_data/padstack_instance.py` & `pyaedt-0.6.86/pyaedt/edb_core/ipc2581/ecad/cad_data/padstack_instance.py`

 * *Files identical despite different names*

### Comparing `pyaedt-0.6.85/pyaedt/edb_core/ipc2581/ecad/cad_data/padstack_pad_def.py` & `pyaedt-0.6.86/pyaedt/edb_core/ipc2581/ecad/cad_data/padstack_pad_def.py`

 * *Files identical despite different names*

### Comparing `pyaedt-0.6.85/pyaedt/edb_core/ipc2581/ecad/cad_data/path.py` & `pyaedt-0.6.86/pyaedt/edb_core/ipc2581/ecad/cad_data/path.py`

 * *Files identical despite different names*

### Comparing `pyaedt-0.6.85/pyaedt/edb_core/ipc2581/ecad/cad_data/phy_net.py` & `pyaedt-0.6.86/pyaedt/edb_core/ipc2581/ecad/cad_data/phy_net.py`

 * *Files identical despite different names*

### Comparing `pyaedt-0.6.85/pyaedt/edb_core/ipc2581/ecad/cad_data/pin.py` & `pyaedt-0.6.86/pyaedt/edb_core/ipc2581/ecad/cad_data/pin.py`

 * *Files identical despite different names*

### Comparing `pyaedt-0.6.85/pyaedt/edb_core/ipc2581/ecad/cad_data/polygon.py` & `pyaedt-0.6.86/pyaedt/edb_core/ipc2581/ecad/cad_data/polygon.py`

 * *Files identical despite different names*

### Comparing `pyaedt-0.6.85/pyaedt/edb_core/ipc2581/ecad/cad_data/profile.py` & `pyaedt-0.6.86/pyaedt/edb_core/ipc2581/ecad/cad_data/profile.py`

 * *Files identical despite different names*

### Comparing `pyaedt-0.6.85/pyaedt/edb_core/ipc2581/ecad/cad_data/stackup.py` & `pyaedt-0.6.86/pyaedt/edb_core/ipc2581/ecad/cad_data/stackup.py`

 * *Files identical despite different names*

### Comparing `pyaedt-0.6.85/pyaedt/edb_core/ipc2581/ecad/cad_data/stackup_group.py` & `pyaedt-0.6.86/pyaedt/edb_core/ipc2581/ecad/cad_data/stackup_group.py`

 * *Files identical despite different names*

### Comparing `pyaedt-0.6.85/pyaedt/edb_core/ipc2581/ecad/cad_data/stackup_layer.py` & `pyaedt-0.6.86/pyaedt/edb_core/ipc2581/ecad/cad_data/stackup_layer.py`

 * *Files identical despite different names*

### Comparing `pyaedt-0.6.85/pyaedt/edb_core/ipc2581/ecad/cad_data/step.py` & `pyaedt-0.6.86/pyaedt/edb_core/ipc2581/ecad/cad_data/step.py`

 * *Files identical despite different names*

### Comparing `pyaedt-0.6.85/pyaedt/edb_core/ipc2581/ecad/cad_header.py` & `pyaedt-0.6.86/pyaedt/edb_core/ipc2581/ecad/cad_header.py`

 * *Files identical despite different names*

### Comparing `pyaedt-0.6.85/pyaedt/edb_core/ipc2581/ecad/ecad.py` & `pyaedt-0.6.86/pyaedt/edb_core/ipc2581/ecad/ecad.py`

 * *Files identical despite different names*

### Comparing `pyaedt-0.6.85/pyaedt/edb_core/ipc2581/ecad/spec.py` & `pyaedt-0.6.86/pyaedt/edb_core/ipc2581/ecad/spec.py`

 * *Files identical despite different names*

### Comparing `pyaedt-0.6.85/pyaedt/edb_core/ipc2581/history_record.py` & `pyaedt-0.6.86/pyaedt/edb_core/ipc2581/history_record.py`

 * *Files identical despite different names*

### Comparing `pyaedt-0.6.85/pyaedt/edb_core/ipc2581/ipc2581.py` & `pyaedt-0.6.86/pyaedt/edb_core/ipc2581/ipc2581.py`

 * *Files identical despite different names*

### Comparing `pyaedt-0.6.85/pyaedt/edb_core/ipc2581/logistic_header.py` & `pyaedt-0.6.86/pyaedt/edb_core/ipc2581/logistic_header.py`

 * *Files identical despite different names*

### Comparing `pyaedt-0.6.85/pyaedt/edb_core/layout.py` & `pyaedt-0.6.86/pyaedt/edb_core/layout.py`

 * *Files identical despite different names*

### Comparing `pyaedt-0.6.85/pyaedt/edb_core/materials.py` & `pyaedt-0.6.86/pyaedt/edb_core/materials.py`

 * *Files identical despite different names*

### Comparing `pyaedt-0.6.85/pyaedt/edb_core/nets.py` & `pyaedt-0.6.86/pyaedt/edb_core/nets.py`

 * *Files identical despite different names*

### Comparing `pyaedt-0.6.85/pyaedt/edb_core/padstack.py` & `pyaedt-0.6.86/pyaedt/edb_core/padstack.py`

 * *Files identical despite different names*

### Comparing `pyaedt-0.6.85/pyaedt/edb_core/siwave.py` & `pyaedt-0.6.86/pyaedt/edb_core/siwave.py`

 * *Files identical despite different names*

### Comparing `pyaedt-0.6.85/pyaedt/edb_core/stackup.py` & `pyaedt-0.6.86/pyaedt/edb_core/stackup.py`

 * *Files 1% similar despite different names*

```diff
@@ -5,19 +5,20 @@
 
 from __future__ import absolute_import  # noreorder
 
 from collections import OrderedDict
 import json
 import logging
 import math
-import os.path
+import re
 import warnings
 
 from pyaedt import generate_unique_name
 from pyaedt.edb_core.edb_data.layer_data import LayerEdbClass
+from pyaedt.edb_core.edb_data.layer_data import StackupLayerEdbClass
 from pyaedt.edb_core.general import convert_py_list_to_net_list
 
 # from pyaedt.generic.general_methods import property
 from pyaedt.generic.general_methods import ET
 from pyaedt.generic.general_methods import is_ironpython
 from pyaedt.generic.general_methods import pyaedt_function_handler
 from pyaedt.misc.aedtlib_personalib_install import write_pretty_xml
@@ -324,60 +325,88 @@
             Collection of layers.
         """
         if not self._lc:
             self.refresh_layer_collection()
         return self._lc
 
     @property
-    def stackup_mode(self):
+    def mode(self):
         """Stackup mode.
 
         Returns
         -------
         int, str
             Type of the stackup mode, where:
 
             * 0 - Laminate
             * 1 - Overlapping
             * 2 - MultiZone
         """
         self._stackup_mode = self._layer_collection.GetMode()
         return str(self._stackup_mode)
 
-    @stackup_mode.setter
-    def stackup_mode(self, value):
+    @mode.setter
+    def mode(self, value):
         mode = self._pedb.edb_api.Cell.LayerCollectionMode
         if value == 0 or value == mode.Laminate or value == "Laminate":
             self._layer_collection.SetMode(mode.Laminate)
         elif value == 1 or value == mode.Overlapping or value == "Overlapping":
             self._layer_collection.SetMode(mode.Overlapping)
         elif value == 2 or value == mode.MultiZone or value == "MultiZone":
             self._layer_collection.SetMode(mode.MultiZone)
         self._pedb.layout.layer_collection = self._layer_collection
 
     @property
+    def stackup_mode(self):
+        """Stackup mode.
+
+        .. deprecated:: 0.6.52
+           Use :func:`mode` method instead.
+        Returns
+        -------
+        int, str
+            Type of the stackup mode, where:
+
+            * 0 - Laminate
+            * 1 - Overlapping
+            * 2 - MultiZone
+        """
+        warnings.warn("`stackup_mode` is deprecated. Use `mode` method instead.", DeprecationWarning)
+        return self.mode
+
+    @stackup_mode.setter
+    def stackup_mode(self, value):
+        warnings.warn("`stackup_mode` is deprecated. Use `mode` method instead.", DeprecationWarning)
+        self.mode = value
+
+    @property
     def _edb_layer_list(self):
-        return list(self._layer_collection.Layers(self._pedb.edb_api.cell.layer_type_set.AllLayerSet))
+        layer_list = list(self._layer_collection.Layers(self._pedb.edb_api.cell.layer_type_set.AllLayerSet))
+        return [i.Clone() for i in layer_list]
 
     @property
     def _edb_layer_list_nonstackup(self):
-        return list(self._layer_collection.Layers(self._pedb.edb_api.cell.layer_type_set.NonStackupLayerSet))
+        layer_list = list(self._layer_collection.Layers(self._pedb.edb_api.cell.layer_type_set.NonStackupLayerSet))
+        return [i.Clone() for i in layer_list]
 
     @property
     def layers(self):
         """Retrieve the dictionary of layers.
 
         Returns
         -------
         Dict[str, :class:`pyaedt.edb_core.edb_data.layer_data.LayerEdbClass`]
         """
         _lays = OrderedDict()
         for l in self._edb_layer_list:
             name = l.GetName()
-            _lays[name] = LayerEdbClass(self, name)
+            if not l.IsStackupLayer():
+                _lays[name] = LayerEdbClass(self, name)
+            else:
+                _lays[name] = StackupLayerEdbClass(self, name)
         return _lays
 
     @property
     def signal_layers(self):
         """Retrieve the dictionary of signal layers.
 
         Returns
@@ -1657,64 +1686,51 @@
     @pyaedt_function_handler
     def _import_csv(self, file_path):
         """Import stackup defnition from a CSV file.
 
         Parameters
         ----------
         fpath : str
-            File path to the CSV or JSON file.
+            File path to the CSV file.
         """
         if not pd:
             self._pedb.logger.error("Pandas is needed. You must install it first.")
             return False
-        if os.path.splitext(file_path)[1] == ".json":
-            return self._import_layer_stackup(file_path)
         if is_ironpython:
             self._pedb.logger.error("Method works on CPython only.")
             return False
         df = pd.read_csv(file_path, index_col=0)
-        prev_layer = None
-        for row, val in df[::-1].iterrows():
-            if not self.stackup_layers:
-                self.add_layer(
-                    row,
-                    None,
-                    "add_on_top",
-                    val.Type,
-                    val.Material,
-                    val.Dielectric_Fill if not pd.isnull(val.Dielectric_Fill) else "",
-                    val.Thickness,
-                )
+
+        for name in self.stackup_layers.keys():  # pragma: no cover
+            if not name in df.index:
+                logger.error("{} doesn't exist in csv".format(name))
+                return False
+
+        for name, l in df.iterrows():
+            layer_type = l.Type
+            if name in self.layers:
+                layer = self.layers[name]
+                layer.type = layer_type
             else:
-                if row in self.stackup_layers.keys():
-                    lyr = self.stackup_layers[row]
-                    lyr.type = val.Type
-                    lyr.material = val.Material
-                    lyr.dielectric_fill = val.Dielectric_Fill if not pd.isnull(val.Dielectric_Fill) else ""
-                    lyr.thickness = val.Thickness
-                    if prev_layer:
-                        self._set_layout_stackup(lyr._edb_layer, "change_position", prev_layer)
-                else:
-                    if prev_layer and prev_layer in self.stackup_layers:
-                        layer_name = prev_layer
-                    else:
-                        layer_name = list(self.stackup_layers.keys())[-1] if self.stackup_layers else None
-                    self.add_layer(
-                        row,
-                        layer_name,
-                        "insert_above",
-                        val.Type,
-                        val.Material,
-                        val.Dielectric_Fill if not pd.isnull(val.Dielectric_Fill) else "",
-                        val.Thickness,
-                    )
-                prev_layer = row
-        for name in self.stackup_layers:
-            if name not in df.index:
-                self.remove_layer(name)
+                layer = self.add_layer(name, layer_type=layer_type, material="copper", fillMaterial="copper")
+
+            layer.material = l.Material
+            layer.thickness = l.Thickness
+            layer.dielectric_fill = l.Dielectric_Fill
+
+        lc_new = self._pedb.edb_api.Cell.LayerCollection()
+        for name, _ in df.iterrows():
+            layer = self.layers[name]
+            lc_new.AddLayerBottom(layer._edb_layer)
+
+        for name, layer in self.non_stackup_layers.items():
+            lc_new.AddLayerBottom(layer._edb_layer)
+
+        self._pedb.layout.layer_collection = lc_new
+        self.refresh_layer_collection()
         return True
 
     @pyaedt_function_handler
     def _set(self, layers=None, materials=None, roughness=None, non_stackup_layers=None):
         """Update stackup information.
 
         Parameters
@@ -1935,14 +1951,17 @@
                     local_material.permittivity = attr["Permittivity"]
                     local_material.loss_tanget = attr["DielectricLossTangent"]
         return True
 
     @pyaedt_function_handler
     def _import_xml(self, file_path):
         """Read external xml file and update stackup.
+        1, all existing layers must exist in xml file.
+        2, xml can have more layers than the existing stackup.
+        3, if xml has different layer order, reorder the layers according to xml definition.
 
         Parameters
         ----------
         file_path: str
             Path to external XML file.
         Returns
         -------
@@ -1957,20 +1976,57 @@
             material = {}
             for i in list(m):
                 material[i.tag] = list(i)[0].text
             material_dict[m.attrib["Name"]] = material
 
         self._add_materials_from_dictionary(material_dict)
 
-        new_layer_collection = self._pedb.edb_api.Cell.LayerCollection()
-        result = new_layer_collection.ImportFromControlFile(file_path)
-        if result:
-            self._pedb.layout.layer_collection = new_layer_collection
+        lc_import = self._pedb.edb_api.Cell.LayerCollection()
+
+        if not lc_import.ImportFromControlFile(file_path):  # pragma: no cover
+            logger.error("Import xml failed. Please check xml content.")
+            return False
+
+        if not len(self.stackup_layers):
+            self._pedb.layout.layer_collection = lc_import
+            self.refresh_layer_collection()
             return True
 
+        dumy_layers = OrderedDict()
+        for i in list(lc_import.Layers(self._pedb.edb_api.cell.layer_type_set.AllLayerSet)):
+            dumy_layers[i.GetName()] = i.Clone()
+
+        for name in self.layers.keys():
+            if not name in dumy_layers:
+                logger.error("{} doesn't exist in xml".format(name))
+                return False
+
+        for name, l in dumy_layers.items():
+            layer_type = re.sub(r"Layer$", "", l.GetLayerType().ToString()).lower()
+            if name in self.layers:
+                layer = self.layers[name]
+                layer.type = layer_type
+            else:
+                layer = self.add_layer(name, layer_type=layer_type, material="copper", fillMaterial="copper")
+
+            if l.IsStackupLayer():
+                layer.material = l.GetMaterial()
+                layer.thickness = l.GetThicknessValue().ToDouble()
+                layer.dielectric_fill = l.GetFillMaterial()
+                layer.etch_factor = l.GetEtchFactor().ToDouble()
+
+        lc_new = self._pedb.edb_api.Cell.LayerCollection()
+        for name, _ in dumy_layers.items():
+            layer = self.layers[name]
+            lc_new.AddLayerBottom(layer._edb_layer)
+
+        self._pedb.layout.layer_collection = lc_new
+        self.refresh_layer_collection()
+        return True
+
     @pyaedt_function_handler
     def _export_xml(self, file_path):
         """Export stackup information to an external XMLfile.
 
         Parameters
         ----------
         file_path: str
```

### Comparing `pyaedt-0.6.85/pyaedt/emit.py` & `pyaedt-0.6.86/pyaedt/emit.py`

 * *Files identical despite different names*

### Comparing `pyaedt-0.6.85/pyaedt/emit_core/Couplings.py` & `pyaedt-0.6.86/pyaedt/emit_core/Couplings.py`

 * *Files identical despite different names*

### Comparing `pyaedt-0.6.85/pyaedt/emit_core/__init__.py` & `pyaedt-0.6.86/pyaedt/emit_core/__init__.py`

 * *Files 0% similar despite different names*

```diff
@@ -1,13 +1,13 @@
 import imp
 from importlib import import_module
 import os
 import sys
 
-from pyaedt import pyaedt_logger as logger
+from pyaedt.aedt_logger import pyaedt_logger as logger
 from pyaedt.emit_core.emit_constants import InterfererType
 from pyaedt.emit_core.emit_constants import ResultType
 from pyaedt.emit_core.emit_constants import TxRxMode
 from pyaedt.emit_core.emit_constants import UnitType
 
 EMIT_API_PYTHON = None
```

### Comparing `pyaedt-0.6.85/pyaedt/emit_core/emit_constants.py` & `pyaedt-0.6.86/pyaedt/emit_core/emit_constants.py`

 * *Files identical despite different names*

### Comparing `pyaedt-0.6.85/pyaedt/emit_core/results/results.py` & `pyaedt-0.6.86/pyaedt/emit_core/results/results.py`

 * *Files identical despite different names*

### Comparing `pyaedt-0.6.85/pyaedt/emit_core/results/revision.py` & `pyaedt-0.6.86/pyaedt/emit_core/results/revision.py`

 * *Files identical despite different names*

### Comparing `pyaedt-0.6.85/pyaedt/generic/DataHandlers.py` & `pyaedt-0.6.86/pyaedt/generic/DataHandlers.py`

 * *Files identical despite different names*

### Comparing `pyaedt-0.6.85/pyaedt/generic/LoadAEDTFile.py` & `pyaedt-0.6.86/pyaedt/generic/LoadAEDTFile.py`

 * *Files identical despite different names*

### Comparing `pyaedt-0.6.85/pyaedt/generic/clr_module.py` & `pyaedt-0.6.86/pyaedt/generic/clr_module.py`

 * *Files identical despite different names*

### Comparing `pyaedt-0.6.85/pyaedt/generic/configurations.py` & `pyaedt-0.6.86/pyaedt/generic/configurations.py`

 * *Files 0% similar despite different names*

```diff
@@ -765,15 +765,15 @@
     #                 cs.props = props
     #                 cs.update()
     #             update = True
     #     if update:
     #         return True
     #     cs = FaceCoordinateSystem(self._app.modeler, props, name)
     #     try:
-    #         cs._modeler.oeditor.CreateFaceCS(cs._face_paramenters, cs._attributes)
+    #         cs._modeler.oeditor.CreateFaceCS(cs._face_parameters, cs._attributes)
     #         cs._modeler.coordinate_systems.append(cs)
     #         self._app.logger.info("Face Coordinate System {} added.".format(name))
     #     except Exception:
     #         self._app.logger.warning("Failed to add CS {} ".format(name))
 
     @pyaedt_function_handler()
     def _update_object_properties(self, name, val):
```

### Comparing `pyaedt-0.6.85/pyaedt/generic/constants.py` & `pyaedt-0.6.86/pyaedt/generic/constants.py`

 * *Files identical despite different names*

### Comparing `pyaedt-0.6.85/pyaedt/generic/design_types.py` & `pyaedt-0.6.86/pyaedt/generic/design_types.py`

 * *Files identical despite different names*

### Comparing `pyaedt-0.6.85/pyaedt/generic/filesystem.py` & `pyaedt-0.6.86/pyaedt/generic/filesystem.py`

 * *Files identical despite different names*

### Comparing `pyaedt-0.6.85/pyaedt/generic/general_methods.py` & `pyaedt-0.6.86/pyaedt/generic/general_methods.py`

 * *Files 1% similar despite different names*

```diff
@@ -659,35 +659,44 @@
     **kwargs :
 
 
     Returns
     -------
 
     """
+    func_name = None
+    if function.__name__ == "InvokeAedtObjMethod":
+        func_name = args[1]
     retry = 0
     ret_val = None
+    inclusion_list = [
+        "CreateVia",
+        "PasteDesign",
+        "Paste",
+        "PushExcitations",
+        "Rename",
+        "RestoreProjectArchive",
+    ]
+    # if func_name and func_name not in inclusion_list and not func_name.startswith("Get"):
+    if func_name and func_name not in inclusion_list:
+        n = 1
     while retry < n:
         try:
             ret_val = function(*args, **kwargs)
-            # if ret_val is None:
-            # if not ret_val and type(ret_val) not in [float, int, str, tuple, list]:
-            #    ret_val = True
         except:
             retry += 1
-            time.sleep(0.1)
+            time.sleep(1)
         else:
-            break
+            return ret_val
     if retry == n:
         if "__name__" in dir(function):
             raise AttributeError("Error in Executing Method {}.".format(function.__name__))
         else:
             raise AttributeError("Error in Executing Method.")
 
-    return ret_val
-
 
 def time_fn(fn, *args, **kwargs):
     start = datetime.datetime.now()
     results = fn(*args, **kwargs)
     end = datetime.datetime.now()
     fn_name = fn.__module__ + "." + fn.__name__
     delta = (end - start).microseconds * 1e-6
@@ -975,14 +984,16 @@
             result.append(key)
             i = j
     return tuple(result)
 
 
 @pyaedt_function_handler()
 def _create_json_file(json_dict, full_json_path):
+    if not os.path.exists(os.path.dirname(full_json_path)):
+        os.makedirs(os.path.dirname(full_json_path))
     if not is_ironpython:
         with open(full_json_path, "w") as fp:
             json.dump(json_dict, fp, indent=4)
     else:
         temp_path = full_json_path.replace(".json", "_temp.json")
         with open(temp_path, "w") as fp:
             json.dump(json_dict, fp, indent=4)
```

### Comparing `pyaedt-0.6.85/pyaedt/generic/grpc_plugin.py` & `pyaedt-0.6.86/pyaedt/generic/grpc_plugin.py`

 * *Files 1% similar despite different names*

```diff
@@ -110,22 +110,22 @@
         self.__dict__["__methodNames__"] = listFuncs
         # print(self.objectID)
 
     def __str__(self):
         return "Instance of an Aedt object:" + str(self.objectID)
 
     def __Invoke__(self, funcName, argv):
+        if settings.enable_debug_grpc_api_logger:
+            settings.logger.debug("{} {}".format(funcName, argv))
         try:
-            if settings.enable_debug_grpc_api_logger:
-                settings.logger.debug("{}{}".format(funcName, argv))
             return _retry_ntimes(
                 settings.number_of_grpc_api_retries, AedtAPI.InvokeAedtObjMethod, self.objectID, funcName, argv
             )  # Call C function
-        except BaseException as e:
-            raise GrpcApiError("Failed to execute grpc AEDT command:  {}".format(funcName))
+        except:  # pragma: no cover
+            raise GrpcApiError("Failed to execute grpc AEDT command: {}".format(funcName))
 
     def __dir__(self):
         return self.__methodNames__
 
     def __GetObjMethod__(self, funcName):
         try:
```

### Comparing `pyaedt-0.6.85/pyaedt/generic/grpc_plugin_dll.py` & `pyaedt-0.6.86/pyaedt/generic/grpc_plugin_dll.py`

 * *Files identical despite different names*

### Comparing `pyaedt-0.6.85/pyaedt/generic/ibis_reader.py` & `pyaedt-0.6.86/pyaedt/generic/ibis_reader.py`

 * *Files identical despite different names*

### Comparing `pyaedt-0.6.85/pyaedt/generic/near_field_import.py` & `pyaedt-0.6.86/pyaedt/generic/near_field_import.py`

 * *Files identical despite different names*

### Comparing `pyaedt-0.6.85/pyaedt/generic/pdf.py` & `pyaedt-0.6.86/pyaedt/generic/pdf.py`

 * *Files identical despite different names*

### Comparing `pyaedt-0.6.85/pyaedt/generic/plot.py` & `pyaedt-0.6.86/pyaedt/generic/plot.py`

 * *Files identical despite different names*

### Comparing `pyaedt-0.6.85/pyaedt/generic/process.py` & `pyaedt-0.6.86/pyaedt/generic/process.py`

 * *Files identical despite different names*

### Comparing `pyaedt-0.6.85/pyaedt/generic/python_optimizers.py` & `pyaedt-0.6.86/pyaedt/generic/python_optimizers.py`

 * *Files identical despite different names*

### Comparing `pyaedt-0.6.85/pyaedt/generic/report_file_parser.py` & `pyaedt-0.6.86/pyaedt/generic/report_file_parser.py`

 * *Files identical despite different names*

### Comparing `pyaedt-0.6.85/pyaedt/generic/toolkit.py` & `pyaedt-0.6.86/pyaedt/generic/toolkit.py`

 * *Files identical despite different names*

### Comparing `pyaedt-0.6.85/pyaedt/generic/touchstone_parser.py` & `pyaedt-0.6.86/pyaedt/generic/touchstone_parser.py`

 * *Files identical despite different names*

### Comparing `pyaedt-0.6.85/pyaedt/hfss.py` & `pyaedt-0.6.86/pyaedt/hfss.py`

 * *Files identical despite different names*

### Comparing `pyaedt-0.6.85/pyaedt/hfss3dlayout.py` & `pyaedt-0.6.86/pyaedt/hfss3dlayout.py`

 * *Files identical despite different names*

### Comparing `pyaedt-0.6.85/pyaedt/icepak.py` & `pyaedt-0.6.86/pyaedt/icepak.py`

 * *Files 0% similar despite different names*

```diff
@@ -1388,16 +1388,17 @@
         """Update the main settings of the design.
 
         Parameters
         ----------
         gravityDir : int, optional
             Gravity direction from -X to +Z. Options are ``0`` to ``5``.
             The default is ``0``.
-        ambtemp : optional
-            Ambient temperature. The default is ``22``.
+        ambtemp : float, str, optional
+            Ambient temperature. The default is ``20``.
+            The default unit is celsius for float or string including unit definition is accepted, e.g. ``325kel``.
         performvalidation : bool, optional
             Whether to perform validation. The default is ``False``.
         CheckLevel : str, optional
             Level of check to perform during validation. The default
             is ``"None"``.
         defaultfluid : str, optional
             Default fluid material. The default is ``"air"``.
@@ -1415,15 +1416,18 @@
             ``True`` when successful, ``False`` when failed.
 
         References
         ----------
 
         >>> oDesign.SetDesignSettings
         """
-        AmbientTemp = str(ambtemp) + "cel"
+        if ambtemp and not isinstance(ambtemp, str):
+            AmbientTemp = str(ambtemp) + "cel"
+        else:
+            AmbientTemp = ambtemp
         #
         # Configure design settings for gravity etc
         IceGravity = ["X", "Y", "Z"]
         GVPos = False
         if int(gravityDir) > 2:
             GVPos = True
         GVA = IceGravity[int(gravityDir) - 3]
```

### Comparing `pyaedt-0.6.85/pyaedt/maxwell.py` & `pyaedt-0.6.86/pyaedt/maxwell.py`

 * *Files identical despite different names*

### Comparing `pyaedt-0.6.85/pyaedt/maxwellcircuit.py` & `pyaedt-0.6.86/pyaedt/maxwellcircuit.py`

 * *Files identical despite different names*

### Comparing `pyaedt-0.6.85/pyaedt/mechanical.py` & `pyaedt-0.6.86/pyaedt/mechanical.py`

 * *Files identical despite different names*

### Comparing `pyaedt-0.6.85/pyaedt/misc/Console.py_build` & `pyaedt-0.6.86/pyaedt/misc/Console.py_build`

 * *Files identical despite different names*

### Comparing `pyaedt-0.6.85/pyaedt/misc/Job_Settings.areg` & `pyaedt-0.6.86/pyaedt/misc/Job_Settings.areg`

 * *Files identical despite different names*

### Comparing `pyaedt-0.6.85/pyaedt/misc/Jupyter.py_build` & `pyaedt-0.6.86/pyaedt/misc/Jupyter.py_build`

 * *Files identical despite different names*

### Comparing `pyaedt-0.6.85/pyaedt/misc/Run_PyAEDT_Script.py_build` & `pyaedt-0.6.86/pyaedt/misc/Run_PyAEDT_Script.py_build`

 * *Files identical despite different names*

### Comparing `pyaedt-0.6.85/pyaedt/misc/Run_PyAEDT_Toolkit_Script.py_build` & `pyaedt-0.6.86/pyaedt/misc/Run_PyAEDT_Toolkit_Script.py_build`

 * *Files identical despite different names*

### Comparing `pyaedt-0.6.85/pyaedt/misc/aedtlib_personalib_install.py` & `pyaedt-0.6.86/pyaedt/misc/aedtlib_personalib_install.py`

 * *Files identical despite different names*

### Comparing `pyaedt-0.6.85/pyaedt/misc/amat.xml` & `pyaedt-0.6.86/pyaedt/misc/amat.xml`

 * *Files identical despite different names*

### Comparing `pyaedt-0.6.85/pyaedt/misc/ansys_cloud.areg` & `pyaedt-0.6.86/pyaedt/misc/ansys_cloud.areg`

 * *Files identical despite different names*

### Comparing `pyaedt-0.6.85/pyaedt/misc/console_setup.py` & `pyaedt-0.6.86/pyaedt/misc/console_setup.py`

 * *Files identical despite different names*

### Comparing `pyaedt-0.6.85/pyaedt/misc/images/gallery/PyAEDT.png` & `pyaedt-0.6.86/pyaedt/misc/images/gallery/PyAEDT.png`

 * *Files identical despite different names*

### Comparing `pyaedt-0.6.85/pyaedt/misc/images/large/pyansys.png` & `pyaedt-0.6.86/pyaedt/misc/images/large/pyansys.png`

 * *Files identical despite different names*

### Comparing `pyaedt-0.6.85/pyaedt/misc/install_extra_toolkits.py` & `pyaedt-0.6.86/pyaedt/misc/install_extra_toolkits.py`

 * *Files identical despite different names*

### Comparing `pyaedt-0.6.85/pyaedt/misc/jupyter_template.ipynb` & `pyaedt-0.6.86/pyaedt/misc/jupyter_template.ipynb`

 * *Files identical despite different names*

### Comparing `pyaedt-0.6.85/pyaedt/misc/misc.py` & `pyaedt-0.6.86/pyaedt/misc/misc.py`

 * *Files identical despite different names*

### Comparing `pyaedt-0.6.85/pyaedt/misc/ml_data_file_train_100MHz_1GHz.json` & `pyaedt-0.6.86/pyaedt/misc/ml_data_file_train_100MHz_1GHz.json`

 * *Files identical despite different names*

### Comparing `pyaedt-0.6.85/pyaedt/misc/ml_data_file_train_1GHz_10GHz.json` & `pyaedt-0.6.86/pyaedt/misc/ml_data_file_train_1GHz_10GHz.json`

 * *Files identical despite different names*

### Comparing `pyaedt-0.6.85/pyaedt/misc/patch_svr_model_100MHz_1GHz.joblib` & `pyaedt-0.6.86/pyaedt/misc/patch_svr_model_100MHz_1GHz.joblib`

 * *Files identical despite different names*

### Comparing `pyaedt-0.6.85/pyaedt/misc/patch_svr_model_1GHz_10GHz.joblib` & `pyaedt-0.6.86/pyaedt/misc/patch_svr_model_1GHz_10GHz.joblib`

 * *Files identical despite different names*

### Comparing `pyaedt-0.6.85/pyaedt/misc/pyaedt_local_config.acf` & `pyaedt-0.6.86/pyaedt/misc/pyaedt_local_config.acf`

 * *Files identical despite different names*

### Comparing `pyaedt-0.6.85/pyaedt/misc/pyansys-logo-black-cropped.png` & `pyaedt-0.6.86/pyaedt/misc/pyansys-logo-black-cropped.png`

 * *Files identical despite different names*

### Comparing `pyaedt-0.6.85/pyaedt/misc/template.acf` & `pyaedt-0.6.86/pyaedt/misc/template.acf`

 * *Files identical despite different names*

### Comparing `pyaedt-0.6.85/pyaedt/modeler/advanced_cad/actors.py` & `pyaedt-0.6.86/pyaedt/modeler/advanced_cad/actors.py`

 * *Files identical despite different names*

### Comparing `pyaedt-0.6.85/pyaedt/modeler/advanced_cad/multiparts.py` & `pyaedt-0.6.86/pyaedt/modeler/advanced_cad/multiparts.py`

 * *Files identical despite different names*

### Comparing `pyaedt-0.6.85/pyaedt/modeler/advanced_cad/oms.py` & `pyaedt-0.6.86/pyaedt/modeler/advanced_cad/oms.py`

 * *Files identical despite different names*

### Comparing `pyaedt-0.6.85/pyaedt/modeler/advanced_cad/parts.py` & `pyaedt-0.6.86/pyaedt/modeler/advanced_cad/parts.py`

 * *Files identical despite different names*

### Comparing `pyaedt-0.6.85/pyaedt/modeler/advanced_cad/stackup_3d.py` & `pyaedt-0.6.86/pyaedt/modeler/advanced_cad/stackup_3d.py`

 * *Files identical despite different names*

### Comparing `pyaedt-0.6.85/pyaedt/modeler/cad/Modeler.py` & `pyaedt-0.6.86/pyaedt/modeler/cad/Modeler.py`

 * *Files 1% similar despite different names*

```diff
@@ -235,21 +235,39 @@
             self._props = CsProps(self, props)
             try:  # pragma: no cover
                 if "KernelVersion" in self.props:
                     del self.props["KernelVersion"]
             except:
                 pass
 
+    @property
     def props(self):
-        """Coordinate System Properties.
+        """Properties of the coordinate system.
 
         Returns
         -------
         :class:`pyaedt.modeler.Modeler.CSProps`
         """
+        if self._props or settings.aedt_version <= "2022.2" or self.name is None:
+            return self._props
+        obj1 = self._modeler.oeditor.GetChildObject(self.name)
+        props = {}
+        origin = obj1.GetPropValue("Origin")
+        props["Origin"] = origin
+        move_cs_to_end = obj1.GetPropValue("Always Move CS to End")
+        props["MoveToEnd"] = move_cs_to_end
+        move_cs_to_end = obj1.GetPropValue("Axis")
+        props["WhichAxis"] = move_cs_to_end
+        move_cs_to_end = obj1.GetPropValue("Z Rotation Angle")
+        props["ZRotationAngle"] = move_cs_to_end
+        move_cs_to_end = obj1.GetPropValue("Position Offset XY/X")
+        props["XOffset"] = move_cs_to_end
+        move_cs_to_end = obj1.GetPropValue("Position Offset XY/Y")
+        props["YOffset"] = move_cs_to_end
+        self._props = CsProps(self, props)
         return self._props
 
     @property
     def _part_name(self):
         """Internally get the part name which the face belongs to"""
         if not self.face_id:
             # face_id has not been defined yet
@@ -257,16 +275,16 @@
         for obj in self._modeler.objects.values():
             for face in obj.faces:
                 if face.id == self.face_id:
                     return obj.name
         return None  # part has not been found
 
     @property
-    def _face_paramenters(self):
-        """Internal named array for paramenteers of the face coordinate system."""
+    def _face_parameters(self):
+        """Internally named array with parameters of the face coordinate system."""
         arg = ["Name:FaceCSParameters"]
         _dict2arg(self.props, arg)
         return arg
 
     @property
     def _attributes(self):
         """Internal named array for attributes of the face coordinate system."""
@@ -404,16 +422,16 @@
         parameters["AxisPosn"] = positioningParameters
         parameters["WhichAxis"] = axis
         parameters["ZRotationAngle"] = str(rotation) + "deg"
         parameters["XOffset"] = self._dim_arg((offset[0]), self.model_units)
         parameters["YOffset"] = self._dim_arg((offset[1]), self.model_units)
         parameters["AutoAxis"] = False
 
-        self.props = CsProps(self, parameters)
-        self._modeler.oeditor.CreateFaceCS(self._face_paramenters, self._attributes)
+        self._props = CsProps(self, parameters)
+        self._modeler.oeditor.CreateFaceCS(self._face_parameters, self._attributes)
         self._modeler._coordinate_systems.insert(0, self)
         return True
 
     @pyaedt_function_handler()
     def _get_type_from_id(self, obj_id):
         """Get the entity type from the id"""
         for obj in self._modeler.objects.values():
@@ -538,17 +556,17 @@
             return self._props
         obj1 = self._modeler.oeditor.GetChildObject(self.name)
         props = {}
         origin = obj1.GetPropValue("Origin")
         props["OriginX"] = origin[1]
         props["OriginY"] = origin[3]
         props["OriginZ"] = origin[5]
-        axisvec = obj1.GetPropValue("X Axis")
         props["Mode"] = obj1.GetPropValue("Mode")
-        if props["Mode"] == "Axis/Position":
+        if "X Axis" in obj1.GetPropNames():
+            axisvec = obj1.GetPropValue("X Axis")
             props["XAxisXvec"] = axisvec[1]
             props["XAxisYvec"] = axisvec[3]
             props["XAxisZvec"] = axisvec[5]
             ypoint = obj1.GetPropValue("Y Point")
 
             props["YAxisXvec"] = ypoint[1]
             props["YAxisYvec"] = ypoint[3]
@@ -1293,15 +1311,18 @@
         """Coordinate Systems."""
         if settings.aedt_version > "2022.2":
             cs_names = [i for i in self.oeditor.GetChildNames("CoordinateSystems") if i != "Global"]
             for cs_name in cs_names:
                 props = {}
                 local_names = [i.name for i in self._coordinate_systems]
                 if cs_name not in local_names:
-                    self._coordinate_systems.append(CoordinateSystem(self, props, cs_name))
+                    if self.oeditor.GetChildObject(cs_name).GetPropValue("Type") == "Relative":
+                        self._coordinate_systems.append(CoordinateSystem(self, props, cs_name))
+                    elif self.oeditor.GetChildObject(cs_name).GetPropValue("Type") == "Face":
+                        self._coordinate_systems.append(FaceCoordinateSystem(self, props, cs_name))
             return self._coordinate_systems
         if not self._coordinate_systems:
             self._coordinate_systems = self._get_coordinates_data()
         return self._coordinate_systems
 
     @property
     def user_lists(self):
```

### Comparing `pyaedt-0.6.85/pyaedt/modeler/cad/Primitives.py` & `pyaedt-0.6.86/pyaedt/modeler/cad/Primitives.py`

 * *Files identical despite different names*

### Comparing `pyaedt-0.6.85/pyaedt/modeler/cad/Primitives2D.py` & `pyaedt-0.6.86/pyaedt/modeler/cad/Primitives2D.py`

 * *Files identical despite different names*

### Comparing `pyaedt-0.6.85/pyaedt/modeler/cad/Primitives3D.py` & `pyaedt-0.6.86/pyaedt/modeler/cad/Primitives3D.py`

 * *Files identical despite different names*

### Comparing `pyaedt-0.6.85/pyaedt/modeler/cad/components_3d.py` & `pyaedt-0.6.86/pyaedt/modeler/cad/components_3d.py`

 * *Files identical despite different names*

### Comparing `pyaedt-0.6.85/pyaedt/modeler/cad/elements3d.py` & `pyaedt-0.6.86/pyaedt/modeler/cad/elements3d.py`

 * *Files identical despite different names*

### Comparing `pyaedt-0.6.85/pyaedt/modeler/cad/object3d.py` & `pyaedt-0.6.86/pyaedt/modeler/cad/object3d.py`

 * *Files identical despite different names*

### Comparing `pyaedt-0.6.85/pyaedt/modeler/cad/polylines.py` & `pyaedt-0.6.86/pyaedt/modeler/cad/polylines.py`

 * *Files identical despite different names*

### Comparing `pyaedt-0.6.85/pyaedt/modeler/calculators.py` & `pyaedt-0.6.86/pyaedt/modeler/calculators.py`

 * *Files 1% similar despite different names*

```diff
@@ -12,15 +12,15 @@
     """Provides base methods common to transmission line calculation.
 
     Parameters
     ----------
     frequency : float, optional
         Center frequency. The default is ``10.0``.
     frequency_unit : str, optional
-        Frequency units. The default is ``GHz``.
+        Frequency units. The default is ``"GHz"``.
 
     Returns
     -------
     :class:`aedt.toolkits.antennas.common.TransmissionLine`
         Transmission line calculator object.
 
     Examples
@@ -224,15 +224,15 @@
     """Provides base methods common to standard waveguides.
 
     Parameters
     ----------
     frequency : float, optional
         Center frequency. The default is ``10.0``.
     frequency_unit : str, optional
-        Frequency units. The default is ``GHz``.
+        Frequency units. The default is ``"GHz"``.
 
     Returns
     -------
     :class:`aedt.toolkits.antennas.common.StandardWaveguide`
         Standard waveguide object.
 
     Examples
@@ -315,16 +315,16 @@
     def find_waveguide(self, freq, units="GHz"):  # pragma: no cover
         """Find the closest standard waveguide for the operational frequency.
 
         Parameters
         ----------
         freq : float
             Operational frequency.
-        units : str
-           Input frequency units. The default is ``GHz``.
+        units : str, optional
+           Input frequency units. The default is ``"GHz"``.
 
         Returns
         -------
         str
             Waveguide name.
         """
```

### Comparing `pyaedt-0.6.85/pyaedt/modeler/circuits/PrimitivesCircuit.py` & `pyaedt-0.6.86/pyaedt/modeler/circuits/PrimitivesCircuit.py`

 * *Files identical despite different names*

### Comparing `pyaedt-0.6.85/pyaedt/modeler/circuits/PrimitivesEmit.py` & `pyaedt-0.6.86/pyaedt/modeler/circuits/PrimitivesEmit.py`

 * *Files identical despite different names*

### Comparing `pyaedt-0.6.85/pyaedt/modeler/circuits/PrimitivesMaxwellCircuit.py` & `pyaedt-0.6.86/pyaedt/modeler/circuits/PrimitivesMaxwellCircuit.py`

 * *Files identical despite different names*

### Comparing `pyaedt-0.6.85/pyaedt/modeler/circuits/PrimitivesNexxim.py` & `pyaedt-0.6.86/pyaedt/modeler/circuits/PrimitivesNexxim.py`

 * *Files identical despite different names*

### Comparing `pyaedt-0.6.85/pyaedt/modeler/circuits/PrimitivesTwinBuilder.py` & `pyaedt-0.6.86/pyaedt/modeler/circuits/PrimitivesTwinBuilder.py`

 * *Files identical despite different names*

### Comparing `pyaedt-0.6.85/pyaedt/modeler/circuits/object3dcircuit.py` & `pyaedt-0.6.86/pyaedt/modeler/circuits/object3dcircuit.py`

 * *Files identical despite different names*

### Comparing `pyaedt-0.6.85/pyaedt/modeler/geometry_operators.py` & `pyaedt-0.6.86/pyaedt/modeler/geometry_operators.py`

 * *Files identical despite different names*

### Comparing `pyaedt-0.6.85/pyaedt/modeler/modeler2d.py` & `pyaedt-0.6.86/pyaedt/modeler/modeler2d.py`

 * *Files identical despite different names*

### Comparing `pyaedt-0.6.85/pyaedt/modeler/modeler3d.py` & `pyaedt-0.6.86/pyaedt/modeler/modeler3d.py`

 * *Files 1% similar despite different names*

```diff
@@ -351,17 +351,18 @@
                 out_dict["native components"] = config_dict["native components"]
                 cs_set = set()
                 for _, native_dict in out_dict["native components"].items():
                     for _, instance_dict in native_dict["Instances"].items():
                         if instance_dict["CS"] and instance_dict["CS"] != "Global":
                             cs = instance_dict["CS"]
                             cs_set.add(cs)
-                            while config_dict["coordinatesystems"][cs]["Reference CS"] != "Global":
-                                cs = config_dict["coordinatesystems"][cs]["Reference CS"]
-                                cs_set.add(cs)
+                            if cs in config_dict["coordinatesystems"]:
+                                while config_dict["coordinatesystems"][cs]["Reference CS"] != "Global":
+                                    cs = config_dict["coordinatesystems"][cs]["Reference CS"]
+                                    cs_set.add(cs)
                 out_dict["coordinatesystems"] = copy.deepcopy(config_dict["coordinatesystems"])
                 for cs in list(out_dict["coordinatesystems"]):
                     if cs not in cs_set:
                         del out_dict["coordinatesystems"][cs]
             with open(auxiliary_dict, "w") as outfile:
                 json.dump(out_dict, outfile)
         self.oeditor.Create3DComponent(arg, arg2, component_file, arg3)
@@ -1419,29 +1420,38 @@
 
         modify_props = []
         for i in range(len(padding_data)):
             modify_props.append(["NAME:" + direction[i] + " Padding Type", "Value:=", padding_type[i]])
             modify_props.append(["NAME:" + direction[i] + " Padding Data", "Value:=", padding_data[i]])
 
         try:
-            create_region_name = self.modeler.oeditor.GetChildObject(region_name).GetChildNames()[0]
+            region = self._app.get_oo_object(self._app.oeditor, region_name)
+            if not region:
+                self.logger.error("{} does not exist.".format(region))
+                return False
+            create_region_name = region.GetChildNames()[0]
             self.modeler.oeditor.ChangeProperty(
                 list(
                     [
                         "NAME:AllTabs",
                         list(
                             [
                                 "NAME:Geometry3DCmdTab",
                                 list(["NAME:PropServers", region_name + ":" + create_region_name]),
                                 list(["NAME:ChangedProps"] + modify_props),
                             ]
                         ),
                     ]
                 )
             )
+            create_region = self._app.get_oo_object(self._app.oeditor, region_name + "/" + create_region_name)
+            success = all(create_region.GetPropValue(lst[0].strip("NAME:")) == lst[-1] for lst in modify_props)
+            if not success:
+                self.logger.error("Settings update failed.")
+                return False
             return True
         except (GrpcApiError, SystemExit):
             return False
 
     @pyaedt_function_handler
     def change_region_coordinate_system(self, region_cs="Global", region_name="Region"):
         """
@@ -1463,25 +1473,12 @@
         ----------
         >>> import pyaedt
         >>> app = pyaedt.Icepak()
         >>> app.modeler.create_coordinate_system(origin=[1, 1, 1], name="NewCS")
         >>> app.modeler.change_region_coordinate_system(region_cs="NewCS")
         """
         try:
-            create_region_name = self.modeler.oeditor.GetChildObject(region_name).GetChildNames()[0]
-            self.modeler.oeditor.ChangeProperty(
-                list(
-                    [
-                        "NAME:AllTabs",
-                        list(
-                            [
-                                "NAME:Geometry3DCmdTab",
-                                list(["NAME:PropServers", region_name + ":" + create_region_name]),
-                                list(["NAME:ChangedProps", list(["NAME:Coordinate System", "Value:=", region_cs])]),
-                            ]
-                        ),
-                    ]
-                )
-            )
-            return True
+            create_region_name = self._app.get_oo_object(self._app.oeditor, region_name).GetChildNames()[0]
+            create_region = self._app.get_oo_object(self._app.oeditor, region_name + "/" + create_region_name)
+            return create_region.SetPropValue("Coordinate System", region_cs)
         except (GrpcApiError, SystemExit):
             return False
```

### Comparing `pyaedt-0.6.85/pyaedt/modeler/modelerpcb.py` & `pyaedt-0.6.86/pyaedt/modeler/modelerpcb.py`

 * *Files identical despite different names*

### Comparing `pyaedt-0.6.85/pyaedt/modeler/pcb/Primitives3DLayout.py` & `pyaedt-0.6.86/pyaedt/modeler/pcb/Primitives3DLayout.py`

 * *Files identical despite different names*

### Comparing `pyaedt-0.6.85/pyaedt/modeler/pcb/object3dlayout.py` & `pyaedt-0.6.86/pyaedt/modeler/pcb/object3dlayout.py`

 * *Files identical despite different names*

### Comparing `pyaedt-0.6.85/pyaedt/modeler/schematic.py` & `pyaedt-0.6.86/pyaedt/modeler/schematic.py`

 * *Files identical despite different names*

### Comparing `pyaedt-0.6.85/pyaedt/modules/AdvancedPostProcessing.py` & `pyaedt-0.6.86/pyaedt/modules/AdvancedPostProcessing.py`

 * *Files identical despite different names*

### Comparing `pyaedt-0.6.85/pyaedt/modules/Boundary.py` & `pyaedt-0.6.86/pyaedt/modules/Boundary.py`

 * *Files 0% similar despite different names*

```diff
@@ -96,62 +96,54 @@
         else:
             self._app.oboundary.DeleteBoundaries([self.name])
         for el in self._app.boundaries:
             if el.name == self.name:
                 self._app.boundaries.remove(el)
         return True
 
-    def _get_boundary_data(self):
-        dict_out = {}
-        if self._app.design_properties and "BoundarySetup" in self._app.design_properties:
-            for ds in self._app.design_properties["BoundarySetup"]["Boundaries"]:
-                try:
-                    if isinstance(self._app.design_properties["BoundarySetup"]["Boundaries"][ds], (OrderedDict, dict)):
-                        if (
-                            self._app.design_properties["BoundarySetup"]["Boundaries"][ds]["BoundType"] == "Network"
-                            and self._app.design_type == "Icepak"
-                        ):
-                            dict_out[ds] = [self._app.design_properties["BoundarySetup"]["Boundaries"][ds], ""]
-                        else:
-                            dict_out[ds] = [
-                                self._app.design_properties["BoundarySetup"]["Boundaries"][ds],
-                                self._app.design_properties["BoundarySetup"]["Boundaries"][ds]["BoundType"],
-                            ]
-
-                except:
-                    pass
-        if self._app.design_properties and "MaxwellParameterSetup" in self._app.design_properties:
-            for ds in self._app.design_properties["MaxwellParameterSetup"]["MaxwellParameters"]:
-                try:
-                    param = "MaxwellParameters"
-                    setup = "MaxwellParameterSetup"
-                    if isinstance(self._app.design_properties[setup][param][ds], (OrderedDict, dict)):
-                        dict_out[ds] = [
-                            self._app.design_properties["MaxwellParameterSetup"]["MaxwellParameters"][ds],
-                            self._app.design_properties["MaxwellParameterSetup"]["MaxwellParameters"][ds][
-                                "MaxwellParameterType"
-                            ],
-                        ]
-                except:
-                    pass
-        if self._app.design_properties and "ModelSetup" in self._app.design_properties:
+    def _get_boundary_data(self, ds):
+        try:
+            if "MaxwellParameterSetup" in self._app.design_properties:
+                param = "MaxwellParameters"
+                setup = "MaxwellParameterSetup"
+                if isinstance(self._app.design_properties[setup][param][ds], (OrderedDict, dict)):
+                    return [
+                        self._app.design_properties["MaxwellParameterSetup"]["MaxwellParameters"][ds],
+                        self._app.design_properties["MaxwellParameterSetup"]["MaxwellParameters"][ds][
+                            "MaxwellParameterType"
+                        ],
+                    ]
+        except:
+            pass
+        try:
             if "MotionSetupList" in self._app.design_properties["ModelSetup"]:
-                for ds in self._app.design_properties["ModelSetup"]["MotionSetupList"]:
-                    try:
-                        motion_list = "MotionSetupList"
-                        setup = "ModelSetup"
-                        # check moving part
-                        if isinstance(self._app.design_properties[setup][motion_list][ds], (OrderedDict, dict)):
-                            dict_out[ds] = [
-                                self._app.design_properties["ModelSetup"]["MotionSetupList"][ds],
-                                self._app.design_properties["ModelSetup"]["MotionSetupList"][ds]["MotionType"],
-                            ]
-                    except:
-                        pass
-        return dict_out
+                motion_list = "MotionSetupList"
+                setup = "ModelSetup"
+                # check moving part
+                if isinstance(self._app.design_properties[setup][motion_list][ds], (OrderedDict, dict)):
+                    return [
+                        self._app.design_properties["ModelSetup"]["MotionSetupList"][ds],
+                        self._app.design_properties["ModelSetup"]["MotionSetupList"][ds]["MotionType"],
+                    ]
+        except:
+            pass
+        try:
+            if ds in self._app.design_properties["BoundarySetup"]["Boundaries"]:
+                if (
+                    self._app.design_properties["BoundarySetup"]["Boundaries"][ds]["BoundType"] == "Network"
+                    and self._app.design_type == "Icepak"
+                ):
+                    return [self._app.design_properties["BoundarySetup"]["Boundaries"][ds], ""]
+                else:
+                    return [
+                        self._app.design_properties["BoundarySetup"]["Boundaries"][ds],
+                        self._app.design_properties["BoundarySetup"]["Boundaries"][ds]["BoundType"],
+                    ]
+        except:
+            return []
 
 
 class NativeComponentObject(BoundaryCommon, object):
     """Manages Native Component data and execution.
 
     Parameters
     ----------
@@ -430,19 +422,21 @@
     def props(self):
         """Boundary data.
 
         Returns
         -------
         :class:BoundaryProps
         """
-        props = self._get_boundary_data()
+        if self._props:
+            return self._props
+        props = self._get_boundary_data(self.name)
 
-        if self.name in props and not self._props:
-            self._props = BoundaryProps(self, OrderedDict(props[self.name][0]))
-            self._type = props[self.name][1]
+        if props:
+            self._props = BoundaryProps(self, OrderedDict(props[0]))
+            self._type = props[1]
         return self._props
 
     @property
     def type(self):
         """Boundary type.
 
         Returns
@@ -912,19 +906,21 @@
     def props(self):
         """Maxwell parameter data.
 
         Returns
         -------
         :class:BoundaryProps
         """
-        props = self._get_boundary_data()
+        if self._props:
+            return self._props
+        props = self._get_boundary_data(self.name)
 
-        if self.name in props:
-            self._props = BoundaryProps(self, OrderedDict(props[self.name][0]))
-            self._type = props[self.name][1]
+        if props:
+            self._props = BoundaryProps(self, OrderedDict(props[0]))
+            self._type = props[1]
         return self._props
 
     @property
     def name(self):
         """Boundary name."""
         return self._name
 
@@ -1832,19 +1828,21 @@
     def props(self):
         """Excitation data.
 
         Returns
         -------
         :class:BoundaryProps
         """
-        props = self._get_boundary_data()
+        if self._props:
+            return self._props
+        props = self._get_boundary_data(self.name)
 
-        if self.name in props:
-            self._props = BoundaryProps(self, OrderedDict(props[self.name][0]))
-            self._type = props[self.name][1]
+        if props:
+            self._props = BoundaryProps(self, OrderedDict(props[0]))
+            self._type = props[1]
         return self._props
 
     @pyaedt_function_handler()
     def _get_args(self, props=None):
         """Retrieve arguments.
 
         Parameters
```

### Comparing `pyaedt-0.6.85/pyaedt/modules/CableModeling.py` & `pyaedt-0.6.86/pyaedt/modules/CableModeling.py`

 * *Files identical despite different names*

### Comparing `pyaedt-0.6.85/pyaedt/modules/CircuitTemplates.py` & `pyaedt-0.6.86/pyaedt/modules/CircuitTemplates.py`

 * *Files identical despite different names*

### Comparing `pyaedt-0.6.85/pyaedt/modules/DesignXPloration.py` & `pyaedt-0.6.86/pyaedt/modules/DesignXPloration.py`

 * *Files identical despite different names*

### Comparing `pyaedt-0.6.85/pyaedt/modules/LayerStackup.py` & `pyaedt-0.6.86/pyaedt/modules/LayerStackup.py`

 * *Files identical despite different names*

### Comparing `pyaedt-0.6.85/pyaedt/modules/Material.py` & `pyaedt-0.6.86/pyaedt/modules/Material.py`

 * *Files identical despite different names*

### Comparing `pyaedt-0.6.85/pyaedt/modules/MaterialLib.py` & `pyaedt-0.6.86/pyaedt/modules/MaterialLib.py`

 * *Files identical despite different names*

### Comparing `pyaedt-0.6.85/pyaedt/modules/Mesh.py` & `pyaedt-0.6.86/pyaedt/modules/Mesh.py`

 * *Files identical despite different names*

### Comparing `pyaedt-0.6.85/pyaedt/modules/Mesh3DLayout.py` & `pyaedt-0.6.86/pyaedt/modules/Mesh3DLayout.py`

 * *Files identical despite different names*

### Comparing `pyaedt-0.6.85/pyaedt/modules/MeshIcepak.py` & `pyaedt-0.6.86/pyaedt/modules/MeshIcepak.py`

 * *Files identical despite different names*

### Comparing `pyaedt-0.6.85/pyaedt/modules/OptimetricsTemplates.py` & `pyaedt-0.6.86/pyaedt/modules/OptimetricsTemplates.py`

 * *Files identical despite different names*

### Comparing `pyaedt-0.6.85/pyaedt/modules/PostProcessor.py` & `pyaedt-0.6.86/pyaedt/modules/PostProcessor.py`

 * *Files identical despite different names*

### Comparing `pyaedt-0.6.85/pyaedt/modules/SetupTemplates.py` & `pyaedt-0.6.86/pyaedt/modules/SetupTemplates.py`

 * *Files identical despite different names*

### Comparing `pyaedt-0.6.85/pyaedt/modules/SolveSetup.py` & `pyaedt-0.6.86/pyaedt/modules/SolveSetup.py`

 * *Files identical despite different names*

### Comparing `pyaedt-0.6.85/pyaedt/modules/SolveSweeps.py` & `pyaedt-0.6.86/pyaedt/modules/SolveSweeps.py`

 * *Files identical despite different names*

### Comparing `pyaedt-0.6.85/pyaedt/modules/monitor_icepak.py` & `pyaedt-0.6.86/pyaedt/modules/monitor_icepak.py`

 * *Files identical despite different names*

### Comparing `pyaedt-0.6.85/pyaedt/modules/report_templates.py` & `pyaedt-0.6.86/pyaedt/modules/report_templates.py`

 * *Files identical despite different names*

### Comparing `pyaedt-0.6.85/pyaedt/modules/solutions.py` & `pyaedt-0.6.86/pyaedt/modules/solutions.py`

 * *Files identical despite different names*

### Comparing `pyaedt-0.6.85/pyaedt/q3d.py` & `pyaedt-0.6.86/pyaedt/q3d.py`

 * *Files identical despite different names*

### Comparing `pyaedt-0.6.85/pyaedt/rmxprt.py` & `pyaedt-0.6.86/pyaedt/rmxprt.py`

 * *Files identical despite different names*

### Comparing `pyaedt-0.6.85/pyaedt/rpc/rpyc_services.py` & `pyaedt-0.6.86/pyaedt/rpc/rpyc_services.py`

 * *Files identical despite different names*

### Comparing `pyaedt-0.6.85/pyaedt/sbrplus/hdm_parser.py` & `pyaedt-0.6.86/pyaedt/sbrplus/hdm_parser.py`

 * *Files identical despite different names*

### Comparing `pyaedt-0.6.85/pyaedt/sbrplus/hdm_utils.py` & `pyaedt-0.6.86/pyaedt/sbrplus/hdm_utils.py`

 * *Files identical despite different names*

### Comparing `pyaedt-0.6.85/pyaedt/sbrplus/matlab/HdmObject.m` & `pyaedt-0.6.86/pyaedt/sbrplus/matlab/HdmObject.m`

 * *Files identical despite different names*

### Comparing `pyaedt-0.6.85/pyaedt/sbrplus/matlab/SbrBounceType.m` & `pyaedt-0.6.86/pyaedt/sbrplus/matlab/SbrBounceType.m`

 * *Files identical despite different names*

### Comparing `pyaedt-0.6.85/pyaedt/sbrplus/matlab/StopWatch.m` & `pyaedt-0.6.86/pyaedt/sbrplus/matlab/StopWatch.m`

 * *Files identical despite different names*

### Comparing `pyaedt-0.6.85/pyaedt/sbrplus/matlab/add_3dlight.m` & `pyaedt-0.6.86/pyaedt/sbrplus/matlab/add_3dlight.m`

 * *Files identical despite different names*

### Comparing `pyaedt-0.6.85/pyaedt/sbrplus/matlab/draw_rays1.m` & `pyaedt-0.6.86/pyaedt/sbrplus/matlab/draw_rays1.m`

 * *Files identical despite different names*

### Comparing `pyaedt-0.6.85/pyaedt/sbrplus/matlab/draw_wfobj.m` & `pyaedt-0.6.86/pyaedt/sbrplus/matlab/draw_wfobj.m`

 * *Files identical despite different names*

### Comparing `pyaedt-0.6.85/pyaedt/sbrplus/matlab/filter_rays1.m` & `pyaedt-0.6.86/pyaedt/sbrplus/matlab/filter_rays1.m`

 * *Files identical despite different names*

### Comparing `pyaedt-0.6.85/pyaedt/sbrplus/matlab/filtered_tracks.m` & `pyaedt-0.6.86/pyaedt/sbrplus/matlab/filtered_tracks.m`

 * *Files identical despite different names*

### Comparing `pyaedt-0.6.85/pyaedt/sbrplus/matlab/ld_sbrplushdm.m` & `pyaedt-0.6.86/pyaedt/sbrplus/matlab/ld_sbrplushdm.m`

 * *Files identical despite different names*

### Comparing `pyaedt-0.6.85/pyaedt/sbrplus/matlab/ld_wfobj.m` & `pyaedt-0.6.86/pyaedt/sbrplus/matlab/ld_wfobj.m`

 * *Files identical despite different names*

### Comparing `pyaedt-0.6.85/pyaedt/sbrplus/matlab/validate_sfields.m` & `pyaedt-0.6.86/pyaedt/sbrplus/matlab/validate_sfields.m`

 * *Files identical despite different names*

### Comparing `pyaedt-0.6.85/pyaedt/sbrplus/plot.py` & `pyaedt-0.6.86/pyaedt/sbrplus/plot.py`

 * *Files identical despite different names*

### Comparing `pyaedt-0.6.85/pyaedt/siwave.py` & `pyaedt-0.6.86/pyaedt/siwave.py`

 * *Files identical despite different names*

### Comparing `pyaedt-0.6.85/pyaedt/twinbuilder.py` & `pyaedt-0.6.86/pyaedt/twinbuilder.py`

 * *Files identical despite different names*

### Comparing `pyaedt-0.6.85/pyproject.toml` & `pyaedt-0.6.86/pyproject.toml`

 * *Files 2% similar despite different names*

```diff
@@ -46,15 +46,15 @@
     "openpyxl==3.1.2",
     "osmnx",
     "pandas==1.3.5; python_version <= '3.7'",
     "pandas==2.0.3; python_version > '3.7'",
     "pytest==7.4.0",
     "pytest-cov==4.1.0",
     "pytest-xdist==3.3.1",
-    "pyvista==0.40.1; python_version > '3.7'",
+    "pyvista==0.40.2; python_version > '3.7'",
     "pyvista==0.38.0; python_version <= '3.7'",
     "scikit-learn==1.3.0",
     "SRTM.py",
     "utm",
     "scikit-rf",
 
 ]
@@ -70,15 +70,15 @@
     "matplotlib==3.5.3; python_version <= '3.7'",
     "matplotlib==3.7.2; python_version > '3.7'",
     "nbsphinx==0.9.2",
     "numpydoc==1.5.0",
     "osmnx",
     "pypandoc==1.11",
     "pytest-sphinx==0.5.0",
-    "pyvista==0.40.1; python_version > '3.7'",
+    "pyvista==0.40.2; python_version > '3.7'",
     "pyvista==0.38.0; python_version <= '3.7'",
     "recommonmark==0.7.1",
     "scikit-learn==1.3.0",
     "Sphinx==7.0.1",
     "sphinx-autobuild==2021.3.14",
     "sphinx-autodoc-typehints==1.23.3",
     "sphinx-copybutton==0.5.2",
@@ -95,15 +95,15 @@
     "matplotlib==3.5.3; python_version <= '3.7'",
     "matplotlib==3.7.2; python_version > '3.7'",
     "numpy==1.21.6; python_version <= '3.9'",
     "numpy==1.25.1; python_version > '3.9'",
     "pandas==1.3.5; python_version <= '3.7'",
     "pandas==2.0.3; python_version > '3.7'",
     "osmnx",
-    "pyvista==0.40.1; python_version > '3.7'",
+    "pyvista==0.40.2; python_version > '3.7'",
     "pyvista==0.38.0; python_version <= '3.7'",
     "SRTM.py",
     "utm",
     "scikit-rf",
     "openpyxl==3.1.2",
 ]
 all = [
@@ -111,15 +111,15 @@
     "matplotlib==3.5.3; python_version <= '3.7'",
     "matplotlib==3.7.2; python_version > '3.7'",
     "numpy==1.21.6; python_version <= '3.9'",
     "numpy==1.25.1; python_version > '3.9'",
     "pandas==1.3.5; python_version <= '3.7'",
     "pandas==2.0.3; python_version > '3.7'",
     "osmnx",
-    "pyvista==0.40.1; python_version > '3.7'",
+    "pyvista==0.40.2; python_version > '3.7'",
     "pyvista==0.38.0; python_version <= '3.7'",
     "SRTM.py",
     "utm",
     "scikit-rf",
     "openpyxl==3.1.2",
 ]
```

### Comparing `pyaedt-0.6.85/PKG-INFO` & `pyaedt-0.6.86/PKG-INFO`

 * *Files 2% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: pyaedt
-Version: 0.6.85
+Version: 0.6.86
 Summary: Higher-Level Pythonic Ansys Electronics Desktop Framework
 Author-email: "ANSYS, Inc." <pyansys.core@ansys.com>
 Maintainer-email: PyAEDT developers <massimo.capodiferro@ansys.com>
 Requires-Python: >=3.7,<4
 Description-Content-Type: text/markdown
 Classifier: Development Status :: 4 - Beta
 Classifier: Intended Audience :: Science/Research
@@ -25,15 +25,15 @@
 Requires-Dist: matplotlib==3.5.3 ; extra == "all" and ( python_version <= '3.7')
 Requires-Dist: matplotlib==3.7.2 ; extra == "all" and ( python_version > '3.7')
 Requires-Dist: numpy==1.21.6 ; extra == "all" and ( python_version <= '3.9')
 Requires-Dist: numpy==1.25.1 ; extra == "all" and ( python_version > '3.9')
 Requires-Dist: pandas==1.3.5 ; extra == "all" and ( python_version <= '3.7')
 Requires-Dist: pandas==2.0.3 ; extra == "all" and ( python_version > '3.7')
 Requires-Dist: osmnx ; extra == "all"
-Requires-Dist: pyvista==0.40.1 ; extra == "all" and ( python_version > '3.7')
+Requires-Dist: pyvista==0.40.2 ; extra == "all" and ( python_version > '3.7')
 Requires-Dist: pyvista==0.38.0 ; extra == "all" and ( python_version <= '3.7')
 Requires-Dist: SRTM.py ; extra == "all"
 Requires-Dist: utm ; extra == "all"
 Requires-Dist: scikit-rf ; extra == "all"
 Requires-Dist: openpyxl==3.1.2 ; extra == "all"
 Requires-Dist: ansys-sphinx-theme==0.9.9 ; extra == "doc"
 Requires-Dist: imageio==2.31.1 ; extra == "doc"
@@ -46,15 +46,15 @@
 Requires-Dist: matplotlib==3.5.3 ; extra == "doc" and ( python_version <= '3.7')
 Requires-Dist: matplotlib==3.7.2 ; extra == "doc" and ( python_version > '3.7')
 Requires-Dist: nbsphinx==0.9.2 ; extra == "doc"
 Requires-Dist: numpydoc==1.5.0 ; extra == "doc"
 Requires-Dist: osmnx ; extra == "doc"
 Requires-Dist: pypandoc==1.11 ; extra == "doc"
 Requires-Dist: pytest-sphinx==0.5.0 ; extra == "doc"
-Requires-Dist: pyvista==0.40.1 ; extra == "doc" and ( python_version > '3.7')
+Requires-Dist: pyvista==0.40.2 ; extra == "doc" and ( python_version > '3.7')
 Requires-Dist: pyvista==0.38.0 ; extra == "doc" and ( python_version <= '3.7')
 Requires-Dist: recommonmark==0.7.1 ; extra == "doc"
 Requires-Dist: scikit-learn==1.3.0 ; extra == "doc"
 Requires-Dist: Sphinx==7.0.1 ; extra == "doc"
 Requires-Dist: sphinx-autobuild==2021.3.14 ; extra == "doc"
 Requires-Dist: sphinx-autodoc-typehints==1.23.3 ; extra == "doc"
 Requires-Dist: sphinx-copybutton==0.5.2 ; extra == "doc"
@@ -69,15 +69,15 @@
 Requires-Dist: matplotlib==3.5.3 ; extra == "full" and ( python_version <= '3.7')
 Requires-Dist: matplotlib==3.7.2 ; extra == "full" and ( python_version > '3.7')
 Requires-Dist: numpy==1.21.6 ; extra == "full" and ( python_version <= '3.9')
 Requires-Dist: numpy==1.25.1 ; extra == "full" and ( python_version > '3.9')
 Requires-Dist: pandas==1.3.5 ; extra == "full" and ( python_version <= '3.7')
 Requires-Dist: pandas==2.0.3 ; extra == "full" and ( python_version > '3.7')
 Requires-Dist: osmnx ; extra == "full"
-Requires-Dist: pyvista==0.40.1 ; extra == "full" and ( python_version > '3.7')
+Requires-Dist: pyvista==0.40.2 ; extra == "full" and ( python_version > '3.7')
 Requires-Dist: pyvista==0.38.0 ; extra == "full" and ( python_version <= '3.7')
 Requires-Dist: SRTM.py ; extra == "full"
 Requires-Dist: utm ; extra == "full"
 Requires-Dist: scikit-rf ; extra == "full"
 Requires-Dist: openpyxl==3.1.2 ; extra == "full"
 Requires-Dist: ipython==8.13.0 ; extra == "tests" and ( python_version < '3.9')
 Requires-Dist: ipython==8.14.0 ; extra == "tests" and ( python_version >= '3.9')
@@ -90,15 +90,15 @@
 Requires-Dist: openpyxl==3.1.2 ; extra == "tests"
 Requires-Dist: osmnx ; extra == "tests"
 Requires-Dist: pandas==1.3.5 ; extra == "tests" and ( python_version <= '3.7')
 Requires-Dist: pandas==2.0.3 ; extra == "tests" and ( python_version > '3.7')
 Requires-Dist: pytest==7.4.0 ; extra == "tests"
 Requires-Dist: pytest-cov==4.1.0 ; extra == "tests"
 Requires-Dist: pytest-xdist==3.3.1 ; extra == "tests"
-Requires-Dist: pyvista==0.40.1 ; extra == "tests" and ( python_version > '3.7')
+Requires-Dist: pyvista==0.40.2 ; extra == "tests" and ( python_version > '3.7')
 Requires-Dist: pyvista==0.38.0 ; extra == "tests" and ( python_version <= '3.7')
 Requires-Dist: scikit-learn==1.3.0 ; extra == "tests"
 Requires-Dist: SRTM.py ; extra == "tests"
 Requires-Dist: utm ; extra == "tests"
 Requires-Dist: scikit-rf ; extra == "tests"
 Project-URL: Bug Tracker, https://github.com/pyansys/pyaedt/issues
 Project-URL: Documentation, https://aedt.docs.pyansys.com
```

