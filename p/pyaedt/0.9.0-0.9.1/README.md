# Comparing `tmp/pyaedt-0.9.0.tar.gz` & `tmp/pyaedt-0.9.1.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "pyaedt-0.9.0.tar", last modified: Fri Jan  1 00:00:00 2016, max compression
+gzip compressed data, was "pyaedt-0.9.1.tar", last modified: Fri Jan  1 00:00:00 2016, max compression
```

## Comparing `pyaedt-0.9.0.tar` & `pyaedt-0.9.1.tar`

### file list

```diff
@@ -1,209 +1,210 @@
--rw-r--r--   0        0        0     1090 2024-05-06 22:48:42.851417 pyaedt-0.9.0/LICENSE
--rw-r--r--   0        0        0    10530 2024-05-06 22:48:42.851417 pyaedt-0.9.0/README.md
--rw-r--r--   0        0        0     3339 2024-05-06 22:48:44.915432 pyaedt-0.9.0/pyaedt/__init__.py
--rw-r--r--   0        0        0    32198 2024-05-06 22:48:44.915432 pyaedt-0.9.0/pyaedt/aedt_logger.py
--rw-r--r--   0        0        0     6766 2024-05-06 22:48:44.915432 pyaedt-0.9.0/pyaedt/application/AEDT_File_Management.py
--rw-r--r--   0        0        0    90489 2024-05-06 22:48:44.915432 pyaedt-0.9.0/pyaedt/application/Analysis.py
--rw-r--r--   0        0        0    55394 2024-05-06 22:48:44.915432 pyaedt-0.9.0/pyaedt/application/Analysis3D.py
--rw-r--r--   0        0        0    11416 2024-05-06 22:48:44.915432 pyaedt-0.9.0/pyaedt/application/Analysis3DLayout.py
--rw-r--r--   0        0        0     3136 2024-05-06 22:48:44.919432 pyaedt-0.9.0/pyaedt/application/AnalysisMaxwellCircuit.py
--rw-r--r--   0        0        0    13300 2024-05-06 22:48:44.919432 pyaedt-0.9.0/pyaedt/application/AnalysisNexxim.py
--rw-r--r--   0        0        0     4487 2024-05-06 22:48:44.919432 pyaedt-0.9.0/pyaedt/application/AnalysisRMxprt.py
--rw-r--r--   0        0        0     4723 2024-05-06 22:48:44.919432 pyaedt-0.9.0/pyaedt/application/AnalysisTwinBuilder.py
--rw-r--r--   0        0        0   140908 2024-05-06 22:48:44.919432 pyaedt-0.9.0/pyaedt/application/Design.py
--rw-r--r--   0        0        0     5985 2024-05-06 22:48:44.919432 pyaedt-0.9.0/pyaedt/application/JobManager.py
--rw-r--r--   0        0        0    79373 2024-05-06 22:48:44.919432 pyaedt-0.9.0/pyaedt/application/Variables.py
--rw-r--r--   0        0        0        0 2024-05-06 22:48:44.919432 pyaedt-0.9.0/pyaedt/application/__init__.py
--rw-r--r--   0        0        0    12942 2024-05-06 22:48:44.919432 pyaedt-0.9.0/pyaedt/application/aedt_objects.py
--rw-r--r--   0        0        0    13687 2024-05-06 22:48:44.919432 pyaedt-0.9.0/pyaedt/application/analysis_hf.py
--rw-r--r--   0        0        0    37712 2024-05-06 22:48:44.919432 pyaedt-0.9.0/pyaedt/application/design_solutions.py
--rw-r--r--   0        0        0    79315 2024-05-06 22:48:44.919432 pyaedt-0.9.0/pyaedt/circuit.py
--rw-r--r--   0        0        0    10493 2024-05-06 22:48:44.919432 pyaedt-0.9.0/pyaedt/common_rpc.py
--rw-r--r--   0        0        0    86622 2024-05-06 22:48:44.919432 pyaedt-0.9.0/pyaedt/desktop.py
--rw-r--r--   0        0        0    25696 2024-05-06 22:48:44.919432 pyaedt-0.9.0/pyaedt/downloads.py
--rw-r--r--   0        0        0      202 2024-05-06 22:48:44.919432 pyaedt-0.9.0/pyaedt/edb.py
--rw-r--r--   0        0        0    10953 2024-05-06 22:48:44.919432 pyaedt-0.9.0/pyaedt/emit.py
--rw-r--r--   0        0        0     5884 2024-05-06 22:48:44.919432 pyaedt-0.9.0/pyaedt/emit_core/Couplings.py
--rw-r--r--   0        0        0     3685 2024-05-06 22:48:44.919432 pyaedt-0.9.0/pyaedt/emit_core/__init__.py
--rw-r--r--   0        0        0     2574 2024-05-06 22:48:44.919432 pyaedt-0.9.0/pyaedt/emit_core/emit_constants.py
--rw-r--r--   0        0        0        1 2024-05-06 22:48:44.919432 pyaedt-0.9.0/pyaedt/emit_core/results/__init__.py
--rw-r--r--   0        0        0     7262 2024-05-06 22:48:44.919432 pyaedt-0.9.0/pyaedt/emit_core/results/results.py
--rw-r--r--   0        0        0    29656 2024-05-06 22:48:44.919432 pyaedt-0.9.0/pyaedt/emit_core/results/revision.py
--rw-r--r--   0        0        0     9836 2024-05-06 22:48:44.919432 pyaedt-0.9.0/pyaedt/generic/Ansys.png
--rw-r--r--   0        0        0      737 2024-05-06 22:48:44.919432 pyaedt-0.9.0/pyaedt/generic/AnsysTemplate.json
--rw-r--r--   0        0        0    15327 2024-05-06 22:48:44.919432 pyaedt-0.9.0/pyaedt/generic/DataHandlers.py
--rw-r--r--   0        0        0    16041 2024-05-06 22:48:44.919432 pyaedt-0.9.0/pyaedt/generic/LoadAEDTFile.py
--rw-r--r--   0        0        0        0 2024-05-06 22:48:44.919432 pyaedt-0.9.0/pyaedt/generic/__init__.py
--rw-r--r--   0        0        0     1345 2024-05-06 22:48:44.919432 pyaedt-0.9.0/pyaedt/generic/ami.json
--rw-r--r--   0        0        0     3356 2024-05-06 22:48:44.919432 pyaedt-0.9.0/pyaedt/generic/clr_module.py
--rw-r--r--   0        0        0        0 2024-05-06 22:48:44.919432 pyaedt-0.9.0/pyaedt/generic/com_parameters.py
--rw-r--r--   0        0        0    36938 2024-05-06 22:48:44.919432 pyaedt-0.9.0/pyaedt/generic/compliance.py
--rw-r--r--   0        0        0    88966 2024-05-06 22:48:44.919432 pyaedt-0.9.0/pyaedt/generic/configurations.py
--rw-r--r--   0        0        0    27640 2024-05-06 22:48:44.923431 pyaedt-0.9.0/pyaedt/generic/constants.py
--rw-r--r--   0        0        0    72540 2024-05-06 22:48:44.923431 pyaedt-0.9.0/pyaedt/generic/design_types.py
--rw-r--r--   0        0        0      184 2024-05-06 22:48:44.923431 pyaedt-0.9.0/pyaedt/generic/desktop_sessions.py
--rw-r--r--   0        0        0     3914 2024-05-06 22:48:44.923431 pyaedt-0.9.0/pyaedt/generic/filesystem.py
--rw-r--r--   0        0        0    67028 2024-05-06 22:48:44.923431 pyaedt-0.9.0/pyaedt/generic/general_methods.py
--rw-r--r--   0        0        0     9169 2024-05-06 22:48:44.923431 pyaedt-0.9.0/pyaedt/generic/grpc_plugin.py
--rw-r--r--   0        0        0     3369 2024-05-06 22:48:44.923431 pyaedt-0.9.0/pyaedt/generic/grpc_plugin_dll.py
--rw-r--r--   0        0        0    42850 2024-05-06 22:48:44.923431 pyaedt-0.9.0/pyaedt/generic/ibis_reader.py
--rw-r--r--   0        0        0     2642 2024-05-06 22:48:44.923431 pyaedt-0.9.0/pyaedt/generic/ibis_v7.json
--rw-r--r--   0        0        0     6857 2024-05-06 22:48:44.923431 pyaedt-0.9.0/pyaedt/generic/near_field_import.py
--rw-r--r--   0        0        0    21288 2024-05-06 22:48:44.923431 pyaedt-0.9.0/pyaedt/generic/pdf.py
--rw-r--r--   0        0        0    64559 2024-05-06 22:48:44.923431 pyaedt-0.9.0/pyaedt/generic/plot.py
--rw-r--r--   0        0        0    19739 2024-05-06 22:48:44.923431 pyaedt-0.9.0/pyaedt/generic/python_optimizers.py
--rw-r--r--   0        0        0     3468 2024-05-06 22:48:44.923431 pyaedt-0.9.0/pyaedt/generic/report_file_parser.py
--rw-r--r--   0        0        0    17193 2024-05-06 22:48:44.923431 pyaedt-0.9.0/pyaedt/generic/settings.py
--rw-r--r--   0        0        0    24726 2024-05-06 22:48:44.923431 pyaedt-0.9.0/pyaedt/generic/spisim.py
--rw-r--r--   0        0        0    19829 2024-05-06 22:48:44.923431 pyaedt-0.9.0/pyaedt/generic/touchstone_parser.py
--rw-r--r--   0        0        0   246456 2024-05-06 22:48:44.923431 pyaedt-0.9.0/pyaedt/hfss.py
--rw-r--r--   0        0        0    83948 2024-05-06 22:48:44.923431 pyaedt-0.9.0/pyaedt/hfss3dlayout.py
--rw-r--r--   0        0        0   269716 2024-05-06 22:48:44.923431 pyaedt-0.9.0/pyaedt/icepak.py
--rw-r--r--   0        0        0   127785 2024-05-06 22:48:44.923431 pyaedt-0.9.0/pyaedt/maxwell.py
--rw-r--r--   0        0        0     7746 2024-05-06 22:48:44.923431 pyaedt-0.9.0/pyaedt/maxwellcircuit.py
--rw-r--r--   0        0        0    24017 2024-05-06 22:48:44.923431 pyaedt-0.9.0/pyaedt/mechanical.py
--rw-r--r--   0        0        0     2154 2024-05-06 22:48:44.923431 pyaedt-0.9.0/pyaedt/misc/Job_Settings.areg
--rw-r--r--   0        0        0      198 2024-05-06 22:48:44.923431 pyaedt-0.9.0/pyaedt/misc/__init__.py
--rw-r--r--   0        0        0    19281 2024-05-06 22:48:44.923431 pyaedt-0.9.0/pyaedt/misc/amat.xml
--rw-r--r--   0        0        0     2536 2024-05-06 22:48:44.923431 pyaedt-0.9.0/pyaedt/misc/ansys_cloud.areg
--rw-r--r--   0        0        0     1951 2024-05-06 22:48:44.923431 pyaedt-0.9.0/pyaedt/misc/config.schema.json
--rw-r--r--   0        0        0       44 2024-05-06 22:48:44.923431 pyaedt-0.9.0/pyaedt/misc/create_remote_dir.py
--rw-r--r--   0        0        0     2623 2024-05-06 22:48:44.923431 pyaedt-0.9.0/pyaedt/misc/misc.py
--rw-r--r--   0        0        0   744826 2024-05-06 22:48:44.927432 pyaedt-0.9.0/pyaedt/misc/ml_data_file_train_100MHz_1GHz.json
--rw-r--r--   0        0        0   502580 2024-05-06 22:48:44.927432 pyaedt-0.9.0/pyaedt/misc/ml_data_file_train_1GHz_10GHz.json
--rw-r--r--   0        0        0   162026 2024-05-06 22:48:44.931432 pyaedt-0.9.0/pyaedt/misc/patch_svr_model_100MHz_1GHz.joblib
--rw-r--r--   0        0        0   134414 2024-05-06 22:48:44.931432 pyaedt-0.9.0/pyaedt/misc/patch_svr_model_1GHz_10GHz.joblib
--rw-r--r--   0        0        0      277 2024-05-06 22:48:44.931432 pyaedt-0.9.0/pyaedt/misc/pyaedt.runtimeconfig.json
--rw-r--r--   0        0        0      960 2024-05-06 22:48:44.931432 pyaedt-0.9.0/pyaedt/misc/pyaedt_local_config.acf
--rw-r--r--   0        0        0    16550 2024-05-06 22:48:44.931432 pyaedt-0.9.0/pyaedt/misc/pyansys-logo-black-cropped.png
--rw-r--r--   0        0        0       58 2024-05-06 22:48:44.931432 pyaedt-0.9.0/pyaedt/misc/spisim_com_configuration_files/__init__.py
--rw-r--r--   0        0        0     5001 2024-05-06 22:48:44.931432 pyaedt-0.9.0/pyaedt/misc/spisim_com_configuration_files/com_120d_8.json
--rw-r--r--   0        0        0     4962 2024-05-06 22:48:44.931432 pyaedt-0.9.0/pyaedt/misc/spisim_com_configuration_files/com_93_8.json
--rw-r--r--   0        0        0     4964 2024-05-06 22:48:44.931432 pyaedt-0.9.0/pyaedt/misc/spisim_com_configuration_files/com_94_17.json
--rw-r--r--   0        0        0    11888 2024-05-06 22:48:44.931432 pyaedt-0.9.0/pyaedt/misc/spisim_com_configuration_files/com_parameters.py
--rw-r--r--   0        0        0    15075 2024-05-06 22:48:44.931432 pyaedt-0.9.0/pyaedt/misc/spisim_com_configuration_files/com_settings_mapping.py
--rw-r--r--   0        0        0      868 2024-05-06 22:48:44.931432 pyaedt-0.9.0/pyaedt/misc/template.acf
--rw-r--r--   0        0        0        0 2024-05-06 22:48:44.931432 pyaedt-0.9.0/pyaedt/modeler/__init__.py
--rw-r--r--   0        0        0        0 2024-05-06 22:48:44.931432 pyaedt-0.9.0/pyaedt/modeler/advanced_cad/__init__.py
--rw-r--r--   0        0        0    13650 2024-05-06 22:48:44.931432 pyaedt-0.9.0/pyaedt/modeler/advanced_cad/actors.py
--rw-r--r--   0        0        0    19389 2024-05-06 22:48:44.931432 pyaedt-0.9.0/pyaedt/modeler/advanced_cad/multiparts.py
--rw-r--r--   0        0        0    18045 2024-05-06 22:48:44.931432 pyaedt-0.9.0/pyaedt/modeler/advanced_cad/oms.py
--rw-r--r--   0        0        0    16174 2024-05-06 22:48:44.931432 pyaedt-0.9.0/pyaedt/modeler/advanced_cad/parts.py
--rw-r--r--   0        0        0   122675 2024-05-06 22:48:44.931432 pyaedt-0.9.0/pyaedt/modeler/advanced_cad/stackup_3d.py
--rw-r--r--   0        0        0    78334 2024-05-06 22:48:44.931432 pyaedt-0.9.0/pyaedt/modeler/cad/Modeler.py
--rw-r--r--   0        0        0   332022 2024-05-06 22:48:44.931432 pyaedt-0.9.0/pyaedt/modeler/cad/Primitives.py
--rw-r--r--   0        0        0    14444 2024-05-06 22:48:44.935432 pyaedt-0.9.0/pyaedt/modeler/cad/Primitives2D.py
--rw-r--r--   0        0        0   142234 2024-05-06 22:48:44.935432 pyaedt-0.9.0/pyaedt/modeler/cad/Primitives3D.py
--rw-r--r--   0        0        0        0 2024-05-06 22:48:44.935432 pyaedt-0.9.0/pyaedt/modeler/cad/__init__.py
--rw-r--r--   0        0        0    28939 2024-05-06 22:48:44.935432 pyaedt-0.9.0/pyaedt/modeler/cad/component_array.py
--rw-r--r--   0        0        0    40806 2024-05-06 22:48:44.935432 pyaedt-0.9.0/pyaedt/modeler/cad/components_3d.py
--rw-r--r--   0        0        0    47933 2024-05-06 22:48:44.935432 pyaedt-0.9.0/pyaedt/modeler/cad/elements3d.py
--rw-r--r--   0        0        0    58466 2024-05-06 22:48:44.935432 pyaedt-0.9.0/pyaedt/modeler/cad/object3d.py
--rw-r--r--   0        0        0    51586 2024-05-06 22:48:44.935432 pyaedt-0.9.0/pyaedt/modeler/cad/polylines.py
--rw-r--r--   0        0        0    12204 2024-05-06 22:48:44.935432 pyaedt-0.9.0/pyaedt/modeler/calculators.py
--rw-r--r--   0        0        0    42521 2024-05-06 22:48:44.935432 pyaedt-0.9.0/pyaedt/modeler/circuits/PrimitivesCircuit.py
--rw-r--r--   0        0        0    38149 2024-05-06 22:48:44.935432 pyaedt-0.9.0/pyaedt/modeler/circuits/PrimitivesEmit.py
--rw-r--r--   0        0        0     8247 2024-05-06 22:48:44.935432 pyaedt-0.9.0/pyaedt/modeler/circuits/PrimitivesMaxwellCircuit.py
--rw-r--r--   0        0        0    66421 2024-05-06 22:48:44.935432 pyaedt-0.9.0/pyaedt/modeler/circuits/PrimitivesNexxim.py
--rw-r--r--   0        0        0    14701 2024-05-06 22:48:44.935432 pyaedt-0.9.0/pyaedt/modeler/circuits/PrimitivesTwinBuilder.py
--rw-r--r--   0        0        0        0 2024-05-06 22:48:44.935432 pyaedt-0.9.0/pyaedt/modeler/circuits/__init__.py
--rw-r--r--   0        0        0    33539 2024-05-06 22:48:44.935432 pyaedt-0.9.0/pyaedt/modeler/circuits/object3dcircuit.py
--rw-r--r--   0        0        0    66209 2024-05-06 22:48:44.935432 pyaedt-0.9.0/pyaedt/modeler/geometry_operators.py
--rw-r--r--   0        0        0     6750 2024-05-06 22:48:44.935432 pyaedt-0.9.0/pyaedt/modeler/modeler2d.py
--rw-r--r--   0        0        0    62989 2024-05-06 22:48:44.935432 pyaedt-0.9.0/pyaedt/modeler/modeler3d.py
--rw-r--r--   0        0        0    31625 2024-05-06 22:48:44.935432 pyaedt-0.9.0/pyaedt/modeler/modelerpcb.py
--rw-r--r--   0        0        0    49876 2024-05-06 22:48:44.935432 pyaedt-0.9.0/pyaedt/modeler/pcb/Primitives3DLayout.py
--rw-r--r--   0        0        0        0 2024-05-06 22:48:44.935432 pyaedt-0.9.0/pyaedt/modeler/pcb/__init__.py
--rw-r--r--   0        0        0    63930 2024-05-06 22:48:44.935432 pyaedt-0.9.0/pyaedt/modeler/pcb/object3dlayout.py
--rw-r--r--   0        0        0    23403 2024-05-06 22:48:44.935432 pyaedt-0.9.0/pyaedt/modeler/schematic.py
--rw-r--r--   0        0        0    50243 2024-05-06 22:48:44.935432 pyaedt-0.9.0/pyaedt/modules/AdvancedPostProcessing.py
--rw-r--r--   0        0        0   165188 2024-05-06 22:48:44.939432 pyaedt-0.9.0/pyaedt/modules/Boundary.py
--rw-r--r--   0        0        0    70334 2024-05-06 22:48:44.939432 pyaedt-0.9.0/pyaedt/modules/CableModeling.py
--rw-r--r--   0        0        0    15739 2024-05-06 22:48:44.939432 pyaedt-0.9.0/pyaedt/modules/CircuitTemplates.py
--rw-r--r--   0        0        0    55348 2024-05-06 22:48:44.939432 pyaedt-0.9.0/pyaedt/modules/DesignXPloration.py
--rw-r--r--   0        0        0    39012 2024-05-06 22:48:44.939432 pyaedt-0.9.0/pyaedt/modules/LayerStackup.py
--rw-r--r--   0        0        0   103157 2024-05-06 22:48:44.939432 pyaedt-0.9.0/pyaedt/modules/Material.py
--rw-r--r--   0        0        0    32810 2024-05-06 22:48:44.939432 pyaedt-0.9.0/pyaedt/modules/MaterialLib.py
--rw-r--r--   0        0        0    53498 2024-05-06 22:48:44.939432 pyaedt-0.9.0/pyaedt/modules/Mesh.py
--rw-r--r--   0        0        0    11939 2024-05-06 22:48:44.939432 pyaedt-0.9.0/pyaedt/modules/Mesh3DLayout.py
--rw-r--r--   0        0        0    49723 2024-05-06 22:48:44.939432 pyaedt-0.9.0/pyaedt/modules/MeshIcepak.py
--rw-r--r--   0        0        0     4309 2024-05-06 22:48:44.939432 pyaedt-0.9.0/pyaedt/modules/OptimetricsTemplates.py
--rw-r--r--   0        0        0   214450 2024-05-06 22:48:44.939432 pyaedt-0.9.0/pyaedt/modules/PostProcessor.py
--rw-r--r--   0        0        0    70341 2024-05-06 22:48:44.939432 pyaedt-0.9.0/pyaedt/modules/SetupTemplates.py
--rw-r--r--   0        0        0   145350 2024-05-06 22:48:44.939432 pyaedt-0.9.0/pyaedt/modules/SolveSetup.py
--rw-r--r--   0        0        0    32118 2024-05-06 22:48:44.939432 pyaedt-0.9.0/pyaedt/modules/SolveSweeps.py
--rw-r--r--   0        0        0        0 2024-05-06 22:48:44.939432 pyaedt-0.9.0/pyaedt/modules/__init__.py
--rw-r--r--   0        0        0    30459 2024-05-06 22:48:44.939432 pyaedt-0.9.0/pyaedt/modules/monitor_icepak.py
--rw-r--r--   0        0        0   133787 2024-05-06 22:48:44.939432 pyaedt-0.9.0/pyaedt/modules/report_templates.py
--rw-r--r--   0        0        0   134041 2024-05-06 22:48:44.943432 pyaedt-0.9.0/pyaedt/modules/solutions.py
--rw-r--r--   0        0        0    94112 2024-05-06 22:48:44.943432 pyaedt-0.9.0/pyaedt/q3d.py
--rw-r--r--   0        0        0    10417 2024-05-06 22:48:44.943432 pyaedt-0.9.0/pyaedt/rmxprt.py
--rw-r--r--   0        0        0        0 2024-05-06 22:48:44.943432 pyaedt-0.9.0/pyaedt/rpc/__init__.py
--rw-r--r--   0        0        0      398 2024-05-06 22:48:44.943432 pyaedt-0.9.0/pyaedt/rpc/local_server.py
--rw-r--r--   0        0        0    41447 2024-05-06 22:48:44.943432 pyaedt-0.9.0/pyaedt/rpc/rpyc_services.py
--rw-r--r--   0        0        0        0 2024-05-06 22:48:44.943432 pyaedt-0.9.0/pyaedt/sbrplus/__init__.py
--rw-r--r--   0        0        0     9235 2024-05-06 22:48:44.943432 pyaedt-0.9.0/pyaedt/sbrplus/hdm_parser.py
--rw-r--r--   0        0        0     2050 2024-05-06 22:48:44.943432 pyaedt-0.9.0/pyaedt/sbrplus/hdm_utils.py
--rw-r--r--   0        0        0     2546 2024-05-06 22:48:44.943432 pyaedt-0.9.0/pyaedt/sbrplus/matlab/HdmObject.m
--rw-r--r--   0        0        0       94 2024-05-06 22:48:44.943432 pyaedt-0.9.0/pyaedt/sbrplus/matlab/README.md
--rw-r--r--   0        0        0      717 2024-05-06 22:48:44.943432 pyaedt-0.9.0/pyaedt/sbrplus/matlab/SbrBounceType.m
--rw-r--r--   0        0        0     2795 2024-05-06 22:48:44.943432 pyaedt-0.9.0/pyaedt/sbrplus/matlab/StopWatch.m
--rw-r--r--   0        0        0     1352 2024-05-06 22:48:44.943432 pyaedt-0.9.0/pyaedt/sbrplus/matlab/add_3dlight.m
--rw-r--r--   0        0        0      325 2024-05-06 22:48:44.943432 pyaedt-0.9.0/pyaedt/sbrplus/matlab/amp2db.m
--rw-r--r--   0        0        0    35749 2024-05-06 22:48:44.943432 pyaedt-0.9.0/pyaedt/sbrplus/matlab/draw_rays1.m
--rw-r--r--   0        0        0     4195 2024-05-06 22:48:44.943432 pyaedt-0.9.0/pyaedt/sbrplus/matlab/draw_wfobj.m
--rw-r--r--   0        0        0    30633 2024-05-06 22:48:44.943432 pyaedt-0.9.0/pyaedt/sbrplus/matlab/filter_rays1.m
--rw-r--r--   0        0        0     1460 2024-05-06 22:48:44.943432 pyaedt-0.9.0/pyaedt/sbrplus/matlab/filtered_tracks.m
--rw-r--r--   0        0        0    20283 2024-05-06 22:48:44.943432 pyaedt-0.9.0/pyaedt/sbrplus/matlab/ld_sbrplushdm.m
--rw-r--r--   0        0        0    14337 2024-05-06 22:48:44.943432 pyaedt-0.9.0/pyaedt/sbrplus/matlab/ld_wfobj.m
--rw-r--r--   0        0        0      303 2024-05-06 22:48:44.943432 pyaedt-0.9.0/pyaedt/sbrplus/matlab/pwr2db.m
--rw-r--r--   0        0        0     2528 2024-05-06 22:48:44.943432 pyaedt-0.9.0/pyaedt/sbrplus/matlab/validate_sfields.m
--rw-r--r--   0        0        0     7410 2024-05-06 22:48:44.943432 pyaedt-0.9.0/pyaedt/sbrplus/plot.py
--rw-r--r--   0        0        0    20988 2024-05-06 22:48:44.943432 pyaedt-0.9.0/pyaedt/twinbuilder.py
--rw-r--r--   0        0        0     1153 2024-05-06 22:48:44.943432 pyaedt-0.9.0/pyaedt/workflows/__init__.py
--rw-r--r--   0        0        0     1153 2024-05-06 22:48:44.943432 pyaedt-0.9.0/pyaedt/workflows/circuit/__init__.py
--rw-r--r--   0        0        0    23239 2024-05-06 22:48:44.943432 pyaedt-0.9.0/pyaedt/workflows/customize_automation_tab.py
--rw-r--r--   0        0        0     1153 2024-05-06 22:48:44.943432 pyaedt-0.9.0/pyaedt/workflows/emit/__init__.py
--rw-r--r--   0        0        0     1153 2024-05-06 22:48:44.943432 pyaedt-0.9.0/pyaedt/workflows/hfss/__init__.py
--rw-r--r--   0        0        0     1145 2024-05-06 22:48:44.943432 pyaedt-0.9.0/pyaedt/workflows/hfss/images/large/antenna.png
--rw-r--r--   0        0        0      271 2024-05-06 22:48:44.943432 pyaedt-0.9.0/pyaedt/workflows/hfss/toolkits_catalog.toml
--rw-r--r--   0        0        0     1153 2024-05-06 22:48:44.943432 pyaedt-0.9.0/pyaedt/workflows/hfss3dlayout/__init__.py
--rw-r--r--   0        0        0     3445 2024-05-06 22:48:44.943432 pyaedt-0.9.0/pyaedt/workflows/hfss3dlayout/export_to_3D.py
--rw-r--r--   0        0        0     2447 2024-05-06 22:48:44.943432 pyaedt-0.9.0/pyaedt/workflows/hfss3dlayout/images/large/cad3d.png
--rw-r--r--   0        0        0      140 2024-05-06 22:48:44.943432 pyaedt-0.9.0/pyaedt/workflows/hfss3dlayout/toolkits_catalog.toml
--rw-r--r--   0        0        0     1153 2024-05-06 22:48:44.943432 pyaedt-0.9.0/pyaedt/workflows/icepak/__init__.py
--rw-r--r--   0        0        0    35360 2024-05-06 22:48:44.943432 pyaedt-0.9.0/pyaedt/workflows/images/large/logo.png
--rw-r--r--   0        0        0      855 2024-05-06 22:48:44.943432 pyaedt-0.9.0/pyaedt/workflows/images/large/pyansys.png
--rw-r--r--   0        0        0     1153 2024-05-06 22:48:44.943432 pyaedt-0.9.0/pyaedt/workflows/installer/__init__.py
--rw-r--r--   0        0        0     3454 2024-05-06 22:48:44.943432 pyaedt-0.9.0/pyaedt/workflows/installer/console_setup.py
--rw-r--r--   0        0        0     1506 2024-05-06 22:48:44.943432 pyaedt-0.9.0/pyaedt/workflows/installer/create_report.py
--rw-r--r--   0        0        0     1247 2024-05-06 22:48:44.943432 pyaedt-0.9.0/pyaedt/workflows/installer/images/large/console.png
--rw-r--r--   0        0        0     1920 2024-05-06 22:48:44.943432 pyaedt-0.9.0/pyaedt/workflows/installer/images/large/jupyter.png
--rw-r--r--   0        0        0     1845 2024-05-06 22:48:44.947432 pyaedt-0.9.0/pyaedt/workflows/installer/images/large/run_script.png
--rw-r--r--   0        0        0      719 2024-05-06 22:48:44.947432 pyaedt-0.9.0/pyaedt/workflows/installer/images/large/toolkit_manager.png
--rw-r--r--   0        0        0     1649 2024-05-06 22:48:44.947432 pyaedt-0.9.0/pyaedt/workflows/installer/jupyter_template.ipynb
--rw-r--r--   0        0        0     2821 2024-05-06 22:48:44.947432 pyaedt-0.9.0/pyaedt/workflows/installer/pyaedt_installer.py
--rw-r--r--   0        0        0    14570 2024-05-06 22:48:44.947432 pyaedt-0.9.0/pyaedt/workflows/installer/toolkit_manager.py
--rw-r--r--   0        0        0      467 2024-05-06 22:48:44.947432 pyaedt-0.9.0/pyaedt/workflows/installer/toolkits_catalog.toml
--rw-r--r--   0        0        0     1153 2024-05-06 22:48:44.947432 pyaedt-0.9.0/pyaedt/workflows/maxwell2d/__init__.py
--rw-r--r--   0        0        0     1153 2024-05-06 22:48:44.947432 pyaedt-0.9.0/pyaedt/workflows/maxwell3d/__init__.py
--rw-r--r--   0        0        0     1206 2024-05-06 22:48:44.947432 pyaedt-0.9.0/pyaedt/workflows/maxwell3d/images/large/magnet_segmentation.png
--rw-r--r--   0        0        0      302 2024-05-06 22:48:44.947432 pyaedt-0.9.0/pyaedt/workflows/maxwell3d/toolkits_catalog.toml
--rw-r--r--   0        0        0     1153 2024-05-06 22:48:44.947432 pyaedt-0.9.0/pyaedt/workflows/mechanical/__init__.py
--rw-r--r--   0        0        0     1153 2024-05-06 22:48:44.947432 pyaedt-0.9.0/pyaedt/workflows/project/__init__.py
--rw-r--r--   0        0        0     1507 2024-05-06 22:48:44.947432 pyaedt-0.9.0/pyaedt/workflows/project/create_report.py
--rw-r--r--   0        0        0     2447 2024-05-06 22:48:44.947432 pyaedt-0.9.0/pyaedt/workflows/project/images/large/cad3d.png
--rw-r--r--   0        0        0      573 2024-05-06 22:48:44.947432 pyaedt-0.9.0/pyaedt/workflows/project/images/large/pdf.png
--rw-r--r--   0        0        0     1276 2024-05-06 22:48:44.947432 pyaedt-0.9.0/pyaedt/workflows/project/import_nastran.py
--rw-r--r--   0        0        0      298 2024-05-06 22:48:44.947432 pyaedt-0.9.0/pyaedt/workflows/project/toolkits_catalog.toml
--rw-r--r--   0        0        0     1153 2024-05-06 22:48:44.947432 pyaedt-0.9.0/pyaedt/workflows/q2d/__init__.py
--rw-r--r--   0        0        0     1153 2024-05-06 22:48:44.947432 pyaedt-0.9.0/pyaedt/workflows/q3d/__init__.py
--rw-r--r--   0        0        0     1153 2024-05-06 22:48:44.947432 pyaedt-0.9.0/pyaedt/workflows/simplorer/__init__.py
--rw-r--r--   0        0        0     3301 2024-05-06 22:48:44.947432 pyaedt-0.9.0/pyaedt/workflows/templates/Jupyter.py_build
--rw-r--r--   0        0        0     3505 2024-05-06 22:48:44.947432 pyaedt-0.9.0/pyaedt/workflows/templates/PyAEDT_Console.py_build
--rw-r--r--   0        0        0     3992 2024-05-06 22:48:44.947432 pyaedt-0.9.0/pyaedt/workflows/templates/Run_PyAEDT_Script.py_build
--rw-r--r--   0        0        0     3267 2024-05-06 22:48:44.947432 pyaedt-0.9.0/pyaedt/workflows/templates/Run_PyAEDT_Toolkit_Script.py_build
--rw-r--r--   0        0        0     3766 2024-05-06 22:48:44.947432 pyaedt-0.9.0/pyaedt/workflows/templates/Run_Toolkit_Manager.py_build
--rw-r--r--   0        0        0     1153 2024-05-06 22:48:44.947432 pyaedt-0.9.0/pyaedt/workflows/templates/__init__.py
--rw-r--r--   0        0        0     6499 2024-05-06 22:48:44.947432 pyaedt-0.9.0/pyproject.toml
--rw-r--r--   0        0        0    16438 1970-01-01 00:00:00.000000 pyaedt-0.9.0/PKG-INFO
+-rw-r--r--   0        0        0     1090 2024-05-13 18:17:19.782796 pyaedt-0.9.1/LICENSE
+-rw-r--r--   0        0        0    10530 2024-05-13 18:17:19.782796 pyaedt-0.9.1/README.md
+-rw-r--r--   0        0        0     3339 2024-05-13 18:17:21.790801 pyaedt-0.9.1/pyaedt/__init__.py
+-rw-r--r--   0        0        0    32198 2024-05-13 18:17:21.790801 pyaedt-0.9.1/pyaedt/aedt_logger.py
+-rw-r--r--   0        0        0     6766 2024-05-13 18:17:21.790801 pyaedt-0.9.1/pyaedt/application/AEDT_File_Management.py
+-rw-r--r--   0        0        0    90489 2024-05-13 18:17:21.790801 pyaedt-0.9.1/pyaedt/application/Analysis.py
+-rw-r--r--   0        0        0    55394 2024-05-13 18:17:21.790801 pyaedt-0.9.1/pyaedt/application/Analysis3D.py
+-rw-r--r--   0        0        0    11416 2024-05-13 18:17:21.790801 pyaedt-0.9.1/pyaedt/application/Analysis3DLayout.py
+-rw-r--r--   0        0        0     3136 2024-05-13 18:17:21.790801 pyaedt-0.9.1/pyaedt/application/AnalysisMaxwellCircuit.py
+-rw-r--r--   0        0        0    13300 2024-05-13 18:17:21.790801 pyaedt-0.9.1/pyaedt/application/AnalysisNexxim.py
+-rw-r--r--   0        0        0     4487 2024-05-13 18:17:21.790801 pyaedt-0.9.1/pyaedt/application/AnalysisRMxprt.py
+-rw-r--r--   0        0        0     4723 2024-05-13 18:17:21.790801 pyaedt-0.9.1/pyaedt/application/AnalysisTwinBuilder.py
+-rw-r--r--   0        0        0   140908 2024-05-13 18:17:21.790801 pyaedt-0.9.1/pyaedt/application/Design.py
+-rw-r--r--   0        0        0     5985 2024-05-13 18:17:21.790801 pyaedt-0.9.1/pyaedt/application/JobManager.py
+-rw-r--r--   0        0        0    79373 2024-05-13 18:17:21.790801 pyaedt-0.9.1/pyaedt/application/Variables.py
+-rw-r--r--   0        0        0        0 2024-05-13 18:17:21.790801 pyaedt-0.9.1/pyaedt/application/__init__.py
+-rw-r--r--   0        0        0    12942 2024-05-13 18:17:21.790801 pyaedt-0.9.1/pyaedt/application/aedt_objects.py
+-rw-r--r--   0        0        0    15469 2024-05-13 18:17:21.790801 pyaedt-0.9.1/pyaedt/application/analysis_hf.py
+-rw-r--r--   0        0        0    37712 2024-05-13 18:17:21.790801 pyaedt-0.9.1/pyaedt/application/design_solutions.py
+-rw-r--r--   0        0        0    79315 2024-05-13 18:17:21.790801 pyaedt-0.9.1/pyaedt/circuit.py
+-rw-r--r--   0        0        0    10493 2024-05-13 18:17:21.794801 pyaedt-0.9.1/pyaedt/common_rpc.py
+-rw-r--r--   0        0        0    86622 2024-05-13 18:17:21.794801 pyaedt-0.9.1/pyaedt/desktop.py
+-rw-r--r--   0        0        0    25696 2024-05-13 18:17:21.794801 pyaedt-0.9.1/pyaedt/downloads.py
+-rw-r--r--   0        0        0      202 2024-05-13 18:17:21.794801 pyaedt-0.9.1/pyaedt/edb.py
+-rw-r--r--   0        0        0    10953 2024-05-13 18:17:21.794801 pyaedt-0.9.1/pyaedt/emit.py
+-rw-r--r--   0        0        0     5884 2024-05-13 18:17:21.794801 pyaedt-0.9.1/pyaedt/emit_core/Couplings.py
+-rw-r--r--   0        0        0     3685 2024-05-13 18:17:21.794801 pyaedt-0.9.1/pyaedt/emit_core/__init__.py
+-rw-r--r--   0        0        0     2574 2024-05-13 18:17:21.794801 pyaedt-0.9.1/pyaedt/emit_core/emit_constants.py
+-rw-r--r--   0        0        0        1 2024-05-13 18:17:21.794801 pyaedt-0.9.1/pyaedt/emit_core/results/__init__.py
+-rw-r--r--   0        0        0     7262 2024-05-13 18:17:21.794801 pyaedt-0.9.1/pyaedt/emit_core/results/results.py
+-rw-r--r--   0        0        0    29656 2024-05-13 18:17:21.794801 pyaedt-0.9.1/pyaedt/emit_core/results/revision.py
+-rw-r--r--   0        0        0     9836 2024-05-13 18:17:21.794801 pyaedt-0.9.1/pyaedt/generic/Ansys.png
+-rw-r--r--   0        0        0      737 2024-05-13 18:17:21.794801 pyaedt-0.9.1/pyaedt/generic/AnsysTemplate.json
+-rw-r--r--   0        0        0    15327 2024-05-13 18:17:21.794801 pyaedt-0.9.1/pyaedt/generic/DataHandlers.py
+-rw-r--r--   0        0        0    16041 2024-05-13 18:17:21.794801 pyaedt-0.9.1/pyaedt/generic/LoadAEDTFile.py
+-rw-r--r--   0        0        0        0 2024-05-13 18:17:21.794801 pyaedt-0.9.1/pyaedt/generic/__init__.py
+-rw-r--r--   0        0        0     1345 2024-05-13 18:17:21.794801 pyaedt-0.9.1/pyaedt/generic/ami.json
+-rw-r--r--   0        0        0     3356 2024-05-13 18:17:21.794801 pyaedt-0.9.1/pyaedt/generic/clr_module.py
+-rw-r--r--   0        0        0        0 2024-05-13 18:17:21.794801 pyaedt-0.9.1/pyaedt/generic/com_parameters.py
+-rw-r--r--   0        0        0    36938 2024-05-13 18:17:21.794801 pyaedt-0.9.1/pyaedt/generic/compliance.py
+-rw-r--r--   0        0        0    88966 2024-05-13 18:17:21.794801 pyaedt-0.9.1/pyaedt/generic/configurations.py
+-rw-r--r--   0        0        0    27640 2024-05-13 18:17:21.794801 pyaedt-0.9.1/pyaedt/generic/constants.py
+-rw-r--r--   0        0        0    72540 2024-05-13 18:17:21.794801 pyaedt-0.9.1/pyaedt/generic/design_types.py
+-rw-r--r--   0        0        0      184 2024-05-13 18:17:21.794801 pyaedt-0.9.1/pyaedt/generic/desktop_sessions.py
+-rw-r--r--   0        0        0     3914 2024-05-13 18:17:21.794801 pyaedt-0.9.1/pyaedt/generic/filesystem.py
+-rw-r--r--   0        0        0    67028 2024-05-13 18:17:21.794801 pyaedt-0.9.1/pyaedt/generic/general_methods.py
+-rw-r--r--   0        0        0     9169 2024-05-13 18:17:21.794801 pyaedt-0.9.1/pyaedt/generic/grpc_plugin.py
+-rw-r--r--   0        0        0     3369 2024-05-13 18:17:21.794801 pyaedt-0.9.1/pyaedt/generic/grpc_plugin_dll.py
+-rw-r--r--   0        0        0    43045 2024-05-13 18:17:21.794801 pyaedt-0.9.1/pyaedt/generic/ibis_reader.py
+-rw-r--r--   0        0        0     2642 2024-05-13 18:17:21.794801 pyaedt-0.9.1/pyaedt/generic/ibis_v7.json
+-rw-r--r--   0        0        0     6857 2024-05-13 18:17:21.794801 pyaedt-0.9.1/pyaedt/generic/near_field_import.py
+-rw-r--r--   0        0        0    21288 2024-05-13 18:17:21.794801 pyaedt-0.9.1/pyaedt/generic/pdf.py
+-rw-r--r--   0        0        0    66064 2024-05-13 18:17:21.794801 pyaedt-0.9.1/pyaedt/generic/plot.py
+-rw-r--r--   0        0        0    19739 2024-05-13 18:17:21.794801 pyaedt-0.9.1/pyaedt/generic/python_optimizers.py
+-rw-r--r--   0        0        0     3468 2024-05-13 18:17:21.794801 pyaedt-0.9.1/pyaedt/generic/report_file_parser.py
+-rw-r--r--   0        0        0    17193 2024-05-13 18:17:21.794801 pyaedt-0.9.1/pyaedt/generic/settings.py
+-rw-r--r--   0        0        0    25002 2024-05-13 18:17:21.794801 pyaedt-0.9.1/pyaedt/generic/spisim.py
+-rw-r--r--   0        0        0    19961 2024-05-13 18:17:21.794801 pyaedt-0.9.1/pyaedt/generic/touchstone_parser.py
+-rw-r--r--   0        0        0   247295 2024-05-13 18:17:21.794801 pyaedt-0.9.1/pyaedt/hfss.py
+-rw-r--r--   0        0        0    83948 2024-05-13 18:17:21.798801 pyaedt-0.9.1/pyaedt/hfss3dlayout.py
+-rw-r--r--   0        0        0   269716 2024-05-13 18:17:21.798801 pyaedt-0.9.1/pyaedt/icepak.py
+-rw-r--r--   0        0        0   127785 2024-05-13 18:17:21.798801 pyaedt-0.9.1/pyaedt/maxwell.py
+-rw-r--r--   0        0        0     7746 2024-05-13 18:17:21.798801 pyaedt-0.9.1/pyaedt/maxwellcircuit.py
+-rw-r--r--   0        0        0    24017 2024-05-13 18:17:21.798801 pyaedt-0.9.1/pyaedt/mechanical.py
+-rw-r--r--   0        0        0     2154 2024-05-13 18:17:21.798801 pyaedt-0.9.1/pyaedt/misc/Job_Settings.areg
+-rw-r--r--   0        0        0      198 2024-05-13 18:17:21.798801 pyaedt-0.9.1/pyaedt/misc/__init__.py
+-rw-r--r--   0        0        0    19281 2024-05-13 18:17:21.798801 pyaedt-0.9.1/pyaedt/misc/amat.xml
+-rw-r--r--   0        0        0     2536 2024-05-13 18:17:21.798801 pyaedt-0.9.1/pyaedt/misc/ansys_cloud.areg
+-rw-r--r--   0        0        0     1951 2024-05-13 18:17:21.798801 pyaedt-0.9.1/pyaedt/misc/config.schema.json
+-rw-r--r--   0        0        0       44 2024-05-13 18:17:21.798801 pyaedt-0.9.1/pyaedt/misc/create_remote_dir.py
+-rw-r--r--   0        0        0     2623 2024-05-13 18:17:21.798801 pyaedt-0.9.1/pyaedt/misc/misc.py
+-rw-r--r--   0        0        0   744826 2024-05-13 18:17:21.798801 pyaedt-0.9.1/pyaedt/misc/ml_data_file_train_100MHz_1GHz.json
+-rw-r--r--   0        0        0   502580 2024-05-13 18:17:21.802801 pyaedt-0.9.1/pyaedt/misc/ml_data_file_train_1GHz_10GHz.json
+-rw-r--r--   0        0        0   162026 2024-05-13 18:17:21.802801 pyaedt-0.9.1/pyaedt/misc/patch_svr_model_100MHz_1GHz.joblib
+-rw-r--r--   0        0        0   134414 2024-05-13 18:17:21.802801 pyaedt-0.9.1/pyaedt/misc/patch_svr_model_1GHz_10GHz.joblib
+-rw-r--r--   0        0        0      277 2024-05-13 18:17:21.802801 pyaedt-0.9.1/pyaedt/misc/pyaedt.runtimeconfig.json
+-rw-r--r--   0        0        0      960 2024-05-13 18:17:21.802801 pyaedt-0.9.1/pyaedt/misc/pyaedt_local_config.acf
+-rw-r--r--   0        0        0    16550 2024-05-13 18:17:21.802801 pyaedt-0.9.1/pyaedt/misc/pyansys-logo-black-cropped.png
+-rw-r--r--   0        0        0       58 2024-05-13 18:17:21.802801 pyaedt-0.9.1/pyaedt/misc/spisim_com_configuration_files/__init__.py
+-rw-r--r--   0        0        0     5001 2024-05-13 18:17:21.802801 pyaedt-0.9.1/pyaedt/misc/spisim_com_configuration_files/com_120d_8.json
+-rw-r--r--   0        0        0     4962 2024-05-13 18:17:21.802801 pyaedt-0.9.1/pyaedt/misc/spisim_com_configuration_files/com_93_8.json
+-rw-r--r--   0        0        0     4964 2024-05-13 18:17:21.802801 pyaedt-0.9.1/pyaedt/misc/spisim_com_configuration_files/com_94_17.json
+-rw-r--r--   0        0        0    11888 2024-05-13 18:17:21.802801 pyaedt-0.9.1/pyaedt/misc/spisim_com_configuration_files/com_parameters.py
+-rw-r--r--   0        0        0    15075 2024-05-13 18:17:21.802801 pyaedt-0.9.1/pyaedt/misc/spisim_com_configuration_files/com_settings_mapping.py
+-rw-r--r--   0        0        0      868 2024-05-13 18:17:21.802801 pyaedt-0.9.1/pyaedt/misc/template.acf
+-rw-r--r--   0        0        0        0 2024-05-13 18:17:21.802801 pyaedt-0.9.1/pyaedt/modeler/__init__.py
+-rw-r--r--   0        0        0        0 2024-05-13 18:17:21.802801 pyaedt-0.9.1/pyaedt/modeler/advanced_cad/__init__.py
+-rw-r--r--   0        0        0    13650 2024-05-13 18:17:21.802801 pyaedt-0.9.1/pyaedt/modeler/advanced_cad/actors.py
+-rw-r--r--   0        0        0    19389 2024-05-13 18:17:21.802801 pyaedt-0.9.1/pyaedt/modeler/advanced_cad/multiparts.py
+-rw-r--r--   0        0        0    18045 2024-05-13 18:17:21.802801 pyaedt-0.9.1/pyaedt/modeler/advanced_cad/oms.py
+-rw-r--r--   0        0        0    16174 2024-05-13 18:17:21.806801 pyaedt-0.9.1/pyaedt/modeler/advanced_cad/parts.py
+-rw-r--r--   0        0        0   122675 2024-05-13 18:17:21.806801 pyaedt-0.9.1/pyaedt/modeler/advanced_cad/stackup_3d.py
+-rw-r--r--   0        0        0    78334 2024-05-13 18:17:21.806801 pyaedt-0.9.1/pyaedt/modeler/cad/Modeler.py
+-rw-r--r--   0        0        0   332022 2024-05-13 18:17:21.806801 pyaedt-0.9.1/pyaedt/modeler/cad/Primitives.py
+-rw-r--r--   0        0        0    14444 2024-05-13 18:17:21.806801 pyaedt-0.9.1/pyaedt/modeler/cad/Primitives2D.py
+-rw-r--r--   0        0        0   142234 2024-05-13 18:17:21.806801 pyaedt-0.9.1/pyaedt/modeler/cad/Primitives3D.py
+-rw-r--r--   0        0        0        0 2024-05-13 18:17:21.806801 pyaedt-0.9.1/pyaedt/modeler/cad/__init__.py
+-rw-r--r--   0        0        0    28939 2024-05-13 18:17:21.806801 pyaedt-0.9.1/pyaedt/modeler/cad/component_array.py
+-rw-r--r--   0        0        0    40806 2024-05-13 18:17:21.806801 pyaedt-0.9.1/pyaedt/modeler/cad/components_3d.py
+-rw-r--r--   0        0        0    47933 2024-05-13 18:17:21.806801 pyaedt-0.9.1/pyaedt/modeler/cad/elements3d.py
+-rw-r--r--   0        0        0    58466 2024-05-13 18:17:21.806801 pyaedt-0.9.1/pyaedt/modeler/cad/object3d.py
+-rw-r--r--   0        0        0    51586 2024-05-13 18:17:21.806801 pyaedt-0.9.1/pyaedt/modeler/cad/polylines.py
+-rw-r--r--   0        0        0    12204 2024-05-13 18:17:21.806801 pyaedt-0.9.1/pyaedt/modeler/calculators.py
+-rw-r--r--   0        0        0    42613 2024-05-13 18:17:21.806801 pyaedt-0.9.1/pyaedt/modeler/circuits/PrimitivesCircuit.py
+-rw-r--r--   0        0        0    38149 2024-05-13 18:17:21.806801 pyaedt-0.9.1/pyaedt/modeler/circuits/PrimitivesEmit.py
+-rw-r--r--   0        0        0     8247 2024-05-13 18:17:21.806801 pyaedt-0.9.1/pyaedt/modeler/circuits/PrimitivesMaxwellCircuit.py
+-rw-r--r--   0        0        0    66421 2024-05-13 18:17:21.810801 pyaedt-0.9.1/pyaedt/modeler/circuits/PrimitivesNexxim.py
+-rw-r--r--   0        0        0    14701 2024-05-13 18:17:21.810801 pyaedt-0.9.1/pyaedt/modeler/circuits/PrimitivesTwinBuilder.py
+-rw-r--r--   0        0        0        0 2024-05-13 18:17:21.810801 pyaedt-0.9.1/pyaedt/modeler/circuits/__init__.py
+-rw-r--r--   0        0        0    34438 2024-05-13 18:17:21.810801 pyaedt-0.9.1/pyaedt/modeler/circuits/object3dcircuit.py
+-rw-r--r--   0        0        0    66209 2024-05-13 18:17:21.810801 pyaedt-0.9.1/pyaedt/modeler/geometry_operators.py
+-rw-r--r--   0        0        0     6750 2024-05-13 18:17:21.810801 pyaedt-0.9.1/pyaedt/modeler/modeler2d.py
+-rw-r--r--   0        0        0    63581 2024-05-13 18:17:21.810801 pyaedt-0.9.1/pyaedt/modeler/modeler3d.py
+-rw-r--r--   0        0        0    31625 2024-05-13 18:17:21.810801 pyaedt-0.9.1/pyaedt/modeler/modelerpcb.py
+-rw-r--r--   0        0        0    49876 2024-05-13 18:17:21.810801 pyaedt-0.9.1/pyaedt/modeler/pcb/Primitives3DLayout.py
+-rw-r--r--   0        0        0        0 2024-05-13 18:17:21.810801 pyaedt-0.9.1/pyaedt/modeler/pcb/__init__.py
+-rw-r--r--   0        0        0    63930 2024-05-13 18:17:21.810801 pyaedt-0.9.1/pyaedt/modeler/pcb/object3dlayout.py
+-rw-r--r--   0        0        0    23403 2024-05-13 18:17:21.810801 pyaedt-0.9.1/pyaedt/modeler/schematic.py
+-rw-r--r--   0        0        0    50243 2024-05-13 18:17:21.810801 pyaedt-0.9.1/pyaedt/modules/AdvancedPostProcessing.py
+-rw-r--r--   0        0        0   165188 2024-05-13 18:17:21.810801 pyaedt-0.9.1/pyaedt/modules/Boundary.py
+-rw-r--r--   0        0        0    70334 2024-05-13 18:17:21.810801 pyaedt-0.9.1/pyaedt/modules/CableModeling.py
+-rw-r--r--   0        0        0    15739 2024-05-13 18:17:21.810801 pyaedt-0.9.1/pyaedt/modules/CircuitTemplates.py
+-rw-r--r--   0        0        0    55348 2024-05-13 18:17:21.810801 pyaedt-0.9.1/pyaedt/modules/DesignXPloration.py
+-rw-r--r--   0        0        0    39012 2024-05-13 18:17:21.810801 pyaedt-0.9.1/pyaedt/modules/LayerStackup.py
+-rw-r--r--   0        0        0   103157 2024-05-13 18:17:21.810801 pyaedt-0.9.1/pyaedt/modules/Material.py
+-rw-r--r--   0        0        0    32810 2024-05-13 18:17:21.810801 pyaedt-0.9.1/pyaedt/modules/MaterialLib.py
+-rw-r--r--   0        0        0    53498 2024-05-13 18:17:21.810801 pyaedt-0.9.1/pyaedt/modules/Mesh.py
+-rw-r--r--   0        0        0    11939 2024-05-13 18:17:21.810801 pyaedt-0.9.1/pyaedt/modules/Mesh3DLayout.py
+-rw-r--r--   0        0        0    50524 2024-05-13 18:17:21.814801 pyaedt-0.9.1/pyaedt/modules/MeshIcepak.py
+-rw-r--r--   0        0        0     4309 2024-05-13 18:17:21.814801 pyaedt-0.9.1/pyaedt/modules/OptimetricsTemplates.py
+-rw-r--r--   0        0        0   215452 2024-05-13 18:17:21.814801 pyaedt-0.9.1/pyaedt/modules/PostProcessor.py
+-rw-r--r--   0        0        0    70341 2024-05-13 18:17:21.814801 pyaedt-0.9.1/pyaedt/modules/SetupTemplates.py
+-rw-r--r--   0        0        0   147490 2024-05-13 18:17:21.814801 pyaedt-0.9.1/pyaedt/modules/SolveSetup.py
+-rw-r--r--   0        0        0    32118 2024-05-13 18:17:21.814801 pyaedt-0.9.1/pyaedt/modules/SolveSweeps.py
+-rw-r--r--   0        0        0        0 2024-05-13 18:17:21.814801 pyaedt-0.9.1/pyaedt/modules/__init__.py
+-rw-r--r--   0        0        0    30459 2024-05-13 18:17:21.814801 pyaedt-0.9.1/pyaedt/modules/monitor_icepak.py
+-rw-r--r--   0        0        0   133787 2024-05-13 18:17:21.814801 pyaedt-0.9.1/pyaedt/modules/report_templates.py
+-rw-r--r--   0        0        0   136507 2024-05-13 18:17:21.814801 pyaedt-0.9.1/pyaedt/modules/solutions.py
+-rw-r--r--   0        0        0    94112 2024-05-13 18:17:21.814801 pyaedt-0.9.1/pyaedt/q3d.py
+-rw-r--r--   0        0        0    10417 2024-05-13 18:17:21.814801 pyaedt-0.9.1/pyaedt/rmxprt.py
+-rw-r--r--   0        0        0        0 2024-05-13 18:17:21.814801 pyaedt-0.9.1/pyaedt/rpc/__init__.py
+-rw-r--r--   0        0        0      398 2024-05-13 18:17:21.814801 pyaedt-0.9.1/pyaedt/rpc/local_server.py
+-rw-r--r--   0        0        0    41447 2024-05-13 18:17:21.814801 pyaedt-0.9.1/pyaedt/rpc/rpyc_services.py
+-rw-r--r--   0        0        0        0 2024-05-13 18:17:21.814801 pyaedt-0.9.1/pyaedt/sbrplus/__init__.py
+-rw-r--r--   0        0        0     9235 2024-05-13 18:17:21.814801 pyaedt-0.9.1/pyaedt/sbrplus/hdm_parser.py
+-rw-r--r--   0        0        0     2050 2024-05-13 18:17:21.814801 pyaedt-0.9.1/pyaedt/sbrplus/hdm_utils.py
+-rw-r--r--   0        0        0     2546 2024-05-13 18:17:21.814801 pyaedt-0.9.1/pyaedt/sbrplus/matlab/HdmObject.m
+-rw-r--r--   0        0        0       94 2024-05-13 18:17:21.814801 pyaedt-0.9.1/pyaedt/sbrplus/matlab/README.md
+-rw-r--r--   0        0        0      717 2024-05-13 18:17:21.814801 pyaedt-0.9.1/pyaedt/sbrplus/matlab/SbrBounceType.m
+-rw-r--r--   0        0        0     2795 2024-05-13 18:17:21.814801 pyaedt-0.9.1/pyaedt/sbrplus/matlab/StopWatch.m
+-rw-r--r--   0        0        0     1352 2024-05-13 18:17:21.814801 pyaedt-0.9.1/pyaedt/sbrplus/matlab/add_3dlight.m
+-rw-r--r--   0        0        0      325 2024-05-13 18:17:21.814801 pyaedt-0.9.1/pyaedt/sbrplus/matlab/amp2db.m
+-rw-r--r--   0        0        0    35749 2024-05-13 18:17:21.814801 pyaedt-0.9.1/pyaedt/sbrplus/matlab/draw_rays1.m
+-rw-r--r--   0        0        0     4195 2024-05-13 18:17:21.818801 pyaedt-0.9.1/pyaedt/sbrplus/matlab/draw_wfobj.m
+-rw-r--r--   0        0        0    30633 2024-05-13 18:17:21.818801 pyaedt-0.9.1/pyaedt/sbrplus/matlab/filter_rays1.m
+-rw-r--r--   0        0        0     1460 2024-05-13 18:17:21.818801 pyaedt-0.9.1/pyaedt/sbrplus/matlab/filtered_tracks.m
+-rw-r--r--   0        0        0    20283 2024-05-13 18:17:21.818801 pyaedt-0.9.1/pyaedt/sbrplus/matlab/ld_sbrplushdm.m
+-rw-r--r--   0        0        0    14337 2024-05-13 18:17:21.818801 pyaedt-0.9.1/pyaedt/sbrplus/matlab/ld_wfobj.m
+-rw-r--r--   0        0        0      303 2024-05-13 18:17:21.818801 pyaedt-0.9.1/pyaedt/sbrplus/matlab/pwr2db.m
+-rw-r--r--   0        0        0     2528 2024-05-13 18:17:21.818801 pyaedt-0.9.1/pyaedt/sbrplus/matlab/validate_sfields.m
+-rw-r--r--   0        0        0     7410 2024-05-13 18:17:21.818801 pyaedt-0.9.1/pyaedt/sbrplus/plot.py
+-rw-r--r--   0        0        0    20988 2024-05-13 18:17:21.818801 pyaedt-0.9.1/pyaedt/twinbuilder.py
+-rw-r--r--   0        0        0     1153 2024-05-13 18:17:21.818801 pyaedt-0.9.1/pyaedt/workflows/__init__.py
+-rw-r--r--   0        0        0     1153 2024-05-13 18:17:21.818801 pyaedt-0.9.1/pyaedt/workflows/circuit/__init__.py
+-rw-r--r--   0        0        0    23319 2024-05-13 18:17:21.818801 pyaedt-0.9.1/pyaedt/workflows/customize_automation_tab.py
+-rw-r--r--   0        0        0     1153 2024-05-13 18:17:21.818801 pyaedt-0.9.1/pyaedt/workflows/emit/__init__.py
+-rw-r--r--   0        0        0     1153 2024-05-13 18:17:21.818801 pyaedt-0.9.1/pyaedt/workflows/hfss/__init__.py
+-rw-r--r--   0        0        0     1145 2024-05-13 18:17:21.818801 pyaedt-0.9.1/pyaedt/workflows/hfss/images/large/antenna.png
+-rw-r--r--   0        0        0      271 2024-05-13 18:17:21.818801 pyaedt-0.9.1/pyaedt/workflows/hfss/toolkits_catalog.toml
+-rw-r--r--   0        0        0     1153 2024-05-13 18:17:21.818801 pyaedt-0.9.1/pyaedt/workflows/hfss3dlayout/__init__.py
+-rw-r--r--   0        0        0     3450 2024-05-13 18:17:21.818801 pyaedt-0.9.1/pyaedt/workflows/hfss3dlayout/export_to_3D.py
+-rw-r--r--   0        0        0     2447 2024-05-13 18:17:21.818801 pyaedt-0.9.1/pyaedt/workflows/hfss3dlayout/images/large/cad3d.png
+-rw-r--r--   0        0        0      140 2024-05-13 18:17:21.818801 pyaedt-0.9.1/pyaedt/workflows/hfss3dlayout/toolkits_catalog.toml
+-rw-r--r--   0        0        0     1153 2024-05-13 18:17:21.818801 pyaedt-0.9.1/pyaedt/workflows/icepak/__init__.py
+-rw-r--r--   0        0        0    35360 2024-05-13 18:17:21.818801 pyaedt-0.9.1/pyaedt/workflows/images/large/logo.png
+-rw-r--r--   0        0        0      855 2024-05-13 18:17:21.818801 pyaedt-0.9.1/pyaedt/workflows/images/large/pyansys.png
+-rw-r--r--   0        0        0     1153 2024-05-13 18:17:21.818801 pyaedt-0.9.1/pyaedt/workflows/installer/__init__.py
+-rw-r--r--   0        0        0     3454 2024-05-13 18:17:21.818801 pyaedt-0.9.1/pyaedt/workflows/installer/console_setup.py
+-rw-r--r--   0        0        0     1511 2024-05-13 18:17:21.818801 pyaedt-0.9.1/pyaedt/workflows/installer/create_report.py
+-rw-r--r--   0        0        0     1247 2024-05-13 18:17:21.818801 pyaedt-0.9.1/pyaedt/workflows/installer/images/large/console.png
+-rw-r--r--   0        0        0     1920 2024-05-13 18:17:21.818801 pyaedt-0.9.1/pyaedt/workflows/installer/images/large/jupyter.png
+-rw-r--r--   0        0        0     1845 2024-05-13 18:17:21.818801 pyaedt-0.9.1/pyaedt/workflows/installer/images/large/run_script.png
+-rw-r--r--   0        0        0      719 2024-05-13 18:17:21.818801 pyaedt-0.9.1/pyaedt/workflows/installer/images/large/toolkit_manager.png
+-rw-r--r--   0        0        0     1649 2024-05-13 18:17:21.818801 pyaedt-0.9.1/pyaedt/workflows/installer/jupyter_template.ipynb
+-rw-r--r--   0        0        0     2821 2024-05-13 18:17:21.818801 pyaedt-0.9.1/pyaedt/workflows/installer/pyaedt_installer.py
+-rw-r--r--   0        0        0    14741 2024-05-13 18:17:21.818801 pyaedt-0.9.1/pyaedt/workflows/installer/toolkit_manager.py
+-rw-r--r--   0        0        0      467 2024-05-13 18:17:21.818801 pyaedt-0.9.1/pyaedt/workflows/installer/toolkits_catalog.toml
+-rw-r--r--   0        0        0     1153 2024-05-13 18:17:21.818801 pyaedt-0.9.1/pyaedt/workflows/maxwell2d/__init__.py
+-rw-r--r--   0        0        0     1153 2024-05-13 18:17:21.818801 pyaedt-0.9.1/pyaedt/workflows/maxwell3d/__init__.py
+-rw-r--r--   0        0        0     1206 2024-05-13 18:17:21.818801 pyaedt-0.9.1/pyaedt/workflows/maxwell3d/images/large/magnet_segmentation.png
+-rw-r--r--   0        0        0      302 2024-05-13 18:17:21.818801 pyaedt-0.9.1/pyaedt/workflows/maxwell3d/toolkits_catalog.toml
+-rw-r--r--   0        0        0     1153 2024-05-13 18:17:21.818801 pyaedt-0.9.1/pyaedt/workflows/mechanical/__init__.py
+-rw-r--r--   0        0        0     1153 2024-05-13 18:17:21.818801 pyaedt-0.9.1/pyaedt/workflows/project/__init__.py
+-rw-r--r--   0        0        0     1512 2024-05-13 18:17:21.818801 pyaedt-0.9.1/pyaedt/workflows/project/create_report.py
+-rw-r--r--   0        0        0     2447 2024-05-13 18:17:21.818801 pyaedt-0.9.1/pyaedt/workflows/project/images/large/cad3d.png
+-rw-r--r--   0        0        0      573 2024-05-13 18:17:21.818801 pyaedt-0.9.1/pyaedt/workflows/project/images/large/pdf.png
+-rw-r--r--   0        0        0     1281 2024-05-13 18:17:21.818801 pyaedt-0.9.1/pyaedt/workflows/project/import_nastran.py
+-rw-r--r--   0        0        0      298 2024-05-13 18:17:21.818801 pyaedt-0.9.1/pyaedt/workflows/project/toolkits_catalog.toml
+-rw-r--r--   0        0        0     1153 2024-05-13 18:17:21.818801 pyaedt-0.9.1/pyaedt/workflows/q2d/__init__.py
+-rw-r--r--   0        0        0     1153 2024-05-13 18:17:21.818801 pyaedt-0.9.1/pyaedt/workflows/q3d/__init__.py
+-rw-r--r--   0        0        0     1153 2024-05-13 18:17:21.818801 pyaedt-0.9.1/pyaedt/workflows/simplorer/__init__.py
+-rw-r--r--   0        0        0     3301 2024-05-13 18:17:21.818801 pyaedt-0.9.1/pyaedt/workflows/templates/Jupyter.py_build
+-rw-r--r--   0        0        0     3505 2024-05-13 18:17:21.818801 pyaedt-0.9.1/pyaedt/workflows/templates/PyAEDT_Console.py_build
+-rw-r--r--   0        0        0     3992 2024-05-13 18:17:21.818801 pyaedt-0.9.1/pyaedt/workflows/templates/Run_PyAEDT_Script.py_build
+-rw-r--r--   0        0        0     4194 2024-05-13 18:17:21.818801 pyaedt-0.9.1/pyaedt/workflows/templates/Run_PyAEDT_Toolkit_Script.py_build
+-rw-r--r--   0        0        0     3766 2024-05-13 18:17:21.818801 pyaedt-0.9.1/pyaedt/workflows/templates/Run_Toolkit_Manager.py_build
+-rw-r--r--   0        0        0     1153 2024-05-13 18:17:21.818801 pyaedt-0.9.1/pyaedt/workflows/templates/__init__.py
+-rw-r--r--   0        0        0     1841 2024-05-13 18:17:21.818801 pyaedt-0.9.1/pyaedt/workflows/templates/toolkit_template.py
+-rw-r--r--   0        0        0     6323 2024-05-13 18:17:21.818801 pyaedt-0.9.1/pyproject.toml
+-rw-r--r--   0        0        0    16188 1970-01-01 00:00:00.000000 pyaedt-0.9.1/PKG-INFO
```

### Comparing `pyaedt-0.9.0/LICENSE` & `pyaedt-0.9.1/LICENSE`

 * *Files identical despite different names*

### Comparing `pyaedt-0.9.0/README.md` & `pyaedt-0.9.1/README.md`

 * *Files identical despite different names*

### Comparing `pyaedt-0.9.0/pyaedt/__init__.py` & `pyaedt-0.9.1/pyaedt/__init__.py`

 * *Files 1% similar despite different names*

```diff
@@ -36,15 +36,15 @@
 
 
 deprecation_warning()
 
 #
 
 pyaedt_path = os.path.dirname(__file__)
-__version__ = "0.9.0"
+__version__ = "0.9.1"
 version = __version__
 
 #
 
 import pyaedt.downloads as downloads
 from pyaedt.generic import constants
 import pyaedt.generic.DataHandlers as data_handler
```

### Comparing `pyaedt-0.9.0/pyaedt/aedt_logger.py` & `pyaedt-0.9.1/pyaedt/aedt_logger.py`

 * *Files identical despite different names*

### Comparing `pyaedt-0.9.0/pyaedt/application/AEDT_File_Management.py` & `pyaedt-0.9.1/pyaedt/application/AEDT_File_Management.py`

 * *Files identical despite different names*

### Comparing `pyaedt-0.9.0/pyaedt/application/Analysis.py` & `pyaedt-0.9.1/pyaedt/application/Analysis.py`

 * *Files identical despite different names*

### Comparing `pyaedt-0.9.0/pyaedt/application/Analysis3D.py` & `pyaedt-0.9.1/pyaedt/application/Analysis3D.py`

 * *Files identical despite different names*

### Comparing `pyaedt-0.9.0/pyaedt/application/Analysis3DLayout.py` & `pyaedt-0.9.1/pyaedt/application/Analysis3DLayout.py`

 * *Files identical despite different names*

### Comparing `pyaedt-0.9.0/pyaedt/application/AnalysisMaxwellCircuit.py` & `pyaedt-0.9.1/pyaedt/application/AnalysisMaxwellCircuit.py`

 * *Files identical despite different names*

### Comparing `pyaedt-0.9.0/pyaedt/application/AnalysisNexxim.py` & `pyaedt-0.9.1/pyaedt/application/AnalysisNexxim.py`

 * *Files identical despite different names*

### Comparing `pyaedt-0.9.0/pyaedt/application/AnalysisRMxprt.py` & `pyaedt-0.9.1/pyaedt/application/AnalysisRMxprt.py`

 * *Files identical despite different names*

### Comparing `pyaedt-0.9.0/pyaedt/application/AnalysisTwinBuilder.py` & `pyaedt-0.9.1/pyaedt/application/AnalysisTwinBuilder.py`

 * *Files identical despite different names*

### Comparing `pyaedt-0.9.0/pyaedt/application/Design.py` & `pyaedt-0.9.1/pyaedt/application/Design.py`

 * *Files identical despite different names*

### Comparing `pyaedt-0.9.0/pyaedt/application/JobManager.py` & `pyaedt-0.9.1/pyaedt/application/JobManager.py`

 * *Files identical despite different names*

### Comparing `pyaedt-0.9.0/pyaedt/application/Variables.py` & `pyaedt-0.9.1/pyaedt/application/Variables.py`

 * *Files identical despite different names*

### Comparing `pyaedt-0.9.0/pyaedt/application/aedt_objects.py` & `pyaedt-0.9.1/pyaedt/application/aedt_objects.py`

 * *Files identical despite different names*

### Comparing `pyaedt-0.9.0/pyaedt/application/analysis_hf.py` & `pyaedt-0.9.1/pyaedt/application/analysis_hf.py`

 * *Files 8% similar despite different names*

```diff
@@ -356,7 +356,68 @@
             file_name=file_name,
             variations=variations,
             variations_value=variations_value,
             renormalization=renormalization,
             impedance=impedance,
             comments=gamma_impedance_comments,
         )
+
+
+def phase_expression(m, n, theta_name="theta_scan", phi_name="phi_scan"):
+    """Return an expression for the source phase angle in a rectangular antenna array.
+
+    Parameters
+    ----------
+    m : int, required
+        Index of the rectangular antenna array element in the x direction.
+    n : int, required
+        Index of the rectangular antenna array element in the y direction.
+    theta_name : str, optional
+        Postprocessing variable name in HFSS to use for the
+        theta component of the phase angle expression. The default is ``"theta_scan"``.
+    phi_name : str, optional
+        Postprocessing variable name in HFSS to use to generate
+        the phi component of the phase angle expression. The default is ``"phi_scan"``
+
+    Returns
+    -------
+    str
+        Phase angle expression for the (m,n) source of
+        the (m,n) antenna array element.
+
+    """
+    # px is the term for the phase variation in the x direction.
+    # py is the term for the phase variation in the y direction.
+
+    if n > 0:
+        add_char = " + "
+    else:
+        add_char = " - "
+    if m == 0:
+        px = ""
+    elif m == -1:
+        px = "-pi*sin(theta_scan)*cos(phi_scan)"
+    elif m == 1:
+        px = "pi*sin(theta_scan)*cos(phi_scan)"
+    else:
+        px = str(m) + "*pi*sin(theta_scan)*cos(phi_scan)"
+    if n == 0:
+        py = ""
+    elif n == -1 or n == 1:
+        py = "pi*sin(theta_scan)*sin(phi_scan)"
+
+    else:
+        py = str(abs(n)) + "*pi*sin(theta_scan)*sin(phi_scan)"
+    if m == 0:
+        if n == 0:
+            return "0"
+        elif n < 0:
+            return "-" + py
+        else:
+            return py
+    elif n == 0:
+        if m == 0:
+            return "0"
+        else:
+            return px
+    else:
+        return px + add_char + py
```

### Comparing `pyaedt-0.9.0/pyaedt/application/design_solutions.py` & `pyaedt-0.9.1/pyaedt/application/design_solutions.py`

 * *Files identical despite different names*

### Comparing `pyaedt-0.9.0/pyaedt/circuit.py` & `pyaedt-0.9.1/pyaedt/circuit.py`

 * *Files identical despite different names*

### Comparing `pyaedt-0.9.0/pyaedt/common_rpc.py` & `pyaedt-0.9.1/pyaedt/common_rpc.py`

 * *Files identical despite different names*

### Comparing `pyaedt-0.9.0/pyaedt/desktop.py` & `pyaedt-0.9.1/pyaedt/desktop.py`

 * *Files identical despite different names*

### Comparing `pyaedt-0.9.0/pyaedt/downloads.py` & `pyaedt-0.9.1/pyaedt/downloads.py`

 * *Files identical despite different names*

### Comparing `pyaedt-0.9.0/pyaedt/emit.py` & `pyaedt-0.9.1/pyaedt/emit.py`

 * *Files identical despite different names*

### Comparing `pyaedt-0.9.0/pyaedt/emit_core/Couplings.py` & `pyaedt-0.9.1/pyaedt/emit_core/Couplings.py`

 * *Files identical despite different names*

### Comparing `pyaedt-0.9.0/pyaedt/emit_core/__init__.py` & `pyaedt-0.9.1/pyaedt/emit_core/__init__.py`

 * *Files identical despite different names*

### Comparing `pyaedt-0.9.0/pyaedt/emit_core/emit_constants.py` & `pyaedt-0.9.1/pyaedt/emit_core/emit_constants.py`

 * *Files identical despite different names*

### Comparing `pyaedt-0.9.0/pyaedt/emit_core/results/results.py` & `pyaedt-0.9.1/pyaedt/emit_core/results/results.py`

 * *Files identical despite different names*

### Comparing `pyaedt-0.9.0/pyaedt/emit_core/results/revision.py` & `pyaedt-0.9.1/pyaedt/emit_core/results/revision.py`

 * *Files identical despite different names*

### Comparing `pyaedt-0.9.0/pyaedt/generic/Ansys.png` & `pyaedt-0.9.1/pyaedt/generic/Ansys.png`

 * *Files identical despite different names*

### Comparing `pyaedt-0.9.0/pyaedt/generic/AnsysTemplate.json` & `pyaedt-0.9.1/pyaedt/generic/AnsysTemplate.json`

 * *Files identical despite different names*

### Comparing `pyaedt-0.9.0/pyaedt/generic/DataHandlers.py` & `pyaedt-0.9.1/pyaedt/generic/DataHandlers.py`

 * *Files identical despite different names*

### Comparing `pyaedt-0.9.0/pyaedt/generic/LoadAEDTFile.py` & `pyaedt-0.9.1/pyaedt/generic/LoadAEDTFile.py`

 * *Files identical despite different names*

### Comparing `pyaedt-0.9.0/pyaedt/generic/ami.json` & `pyaedt-0.9.1/pyaedt/generic/ami.json`

 * *Files identical despite different names*

### Comparing `pyaedt-0.9.0/pyaedt/generic/clr_module.py` & `pyaedt-0.9.1/pyaedt/generic/clr_module.py`

 * *Files identical despite different names*

### Comparing `pyaedt-0.9.0/pyaedt/generic/compliance.py` & `pyaedt-0.9.1/pyaedt/generic/compliance.py`

 * *Files identical despite different names*

### Comparing `pyaedt-0.9.0/pyaedt/generic/configurations.py` & `pyaedt-0.9.1/pyaedt/generic/configurations.py`

 * *Files identical despite different names*

### Comparing `pyaedt-0.9.0/pyaedt/generic/constants.py` & `pyaedt-0.9.1/pyaedt/generic/constants.py`

 * *Files identical despite different names*

### Comparing `pyaedt-0.9.0/pyaedt/generic/design_types.py` & `pyaedt-0.9.1/pyaedt/generic/design_types.py`

 * *Files identical despite different names*

### Comparing `pyaedt-0.9.0/pyaedt/generic/filesystem.py` & `pyaedt-0.9.1/pyaedt/generic/filesystem.py`

 * *Files identical despite different names*

### Comparing `pyaedt-0.9.0/pyaedt/generic/general_methods.py` & `pyaedt-0.9.1/pyaedt/generic/general_methods.py`

 * *Files identical despite different names*

### Comparing `pyaedt-0.9.0/pyaedt/generic/grpc_plugin.py` & `pyaedt-0.9.1/pyaedt/generic/grpc_plugin.py`

 * *Files identical despite different names*

### Comparing `pyaedt-0.9.0/pyaedt/generic/grpc_plugin_dll.py` & `pyaedt-0.9.1/pyaedt/generic/grpc_plugin_dll.py`

 * *Files identical despite different names*

### Comparing `pyaedt-0.9.0/pyaedt/generic/ibis_reader.py` & `pyaedt-0.9.1/pyaedt/generic/ibis_reader.py`

 * *Files 0% similar despite different names*

```diff
@@ -970,19 +970,22 @@
             component.manufacturer = comp_info["manufacturer"]["manufacturer"]
             self.fill_package_info(component, comp_info["package"]["package"])
             pin_list = comp_info["pin"]["pin"].strip().split("\n")[1:]
             for pin_info in pin_list:
                 pin = self.make_pin_object(pin_info, component.name, ibis)
                 component.pins[pin.name] = pin
 
-            diff_pin_list = comp_info["diff pin"]["diff pin"].strip().split("\n")[1:]
-            for pin_info in diff_pin_list:
+            try:
+                diff_pin_list = comp_info["diff pin"]["diff pin"].strip().split("\n")[1:]
+                for pin_info in diff_pin_list:
 
-                pin = self.make_diff_pin_object(pin_info, component, ibis)
-                component.pins[pin.name] = pin
+                    pin = self.make_diff_pin_object(pin_info, component, ibis)
+                    component.pins[pin.name] = pin
+            except Exception as error:  # pragma: no cover
+                logger.warning("Cannot find Diff Pin. Ignore it. Exception message: {}".format(error))
             ibis.components[component.name] = component
 
     @classmethod
     def fill_package_info(cls, component, pkg_info):
         """Extracts model's info.
 
         Parameters
```

### Comparing `pyaedt-0.9.0/pyaedt/generic/ibis_v7.json` & `pyaedt-0.9.1/pyaedt/generic/ibis_v7.json`

 * *Files identical despite different names*

### Comparing `pyaedt-0.9.0/pyaedt/generic/near_field_import.py` & `pyaedt-0.9.1/pyaedt/generic/near_field_import.py`

 * *Files identical despite different names*

### Comparing `pyaedt-0.9.0/pyaedt/generic/pdf.py` & `pyaedt-0.9.1/pyaedt/generic/pdf.py`

 * *Files identical despite different names*

### Comparing `pyaedt-0.9.0/pyaedt/generic/plot.py` & `pyaedt-0.9.1/pyaedt/generic/plot.py`

 * *Files 2% similar despite different names*

```diff
@@ -34,21 +34,45 @@
         )
 
     try:
         from matplotlib.patches import PathPatch
         from matplotlib.path import Path
         import matplotlib.pyplot as plt
 
+        rc_params = {
+            "axes.titlesize": 26,  # Use these default settings for Matplotlb axes.
+            "axes.labelsize": 20,  # Apply the settings only in this module.
+            "xtick.labelsize": 18,
+            "ytick.labelsize": 18,
+        }
+
     except ImportError:
         warnings.warn(
             "The Matplotlib module is required to run some functionalities of PostProcess.\n"
             "Install with \n\npip install matplotlib\n\nRequires CPython."
         )
     except Exception:
-        pass
+        warnings.warn("Unknown error occurred while attempting to import Matplotlib.")
+
+
+# Override default settings for matplotlib
+def update_plot_settings(func, *args, **kwargs):
+    if callable(func):
+
+        def wrapper(*args, **kwargs):
+            default_rc_params = plt.rcParams.copy()
+            plt.rcParams.update(rc_params)  # Apply new settings.
+            out = func(*args, **kwargs)
+            plt.rcParams.update(default_rc_params)
+            return out
+
+    else:
+        wrapper = None
+        raise TypeError("First argument must be callable.")
+    return wrapper
 
 
 @pyaedt_function_handler()
 def get_structured_mesh(theta, phi, ff_data):
     if ff_data.min() < 0:
         ff_data_renorm = ff_data + np.abs(ff_data.min())
     else:
@@ -96,14 +120,15 @@
     -------
     float
         Converted float when successful, ``0`` when when failed.
     """
     try:
         return float(istring.strip())
     except Exception:
+        warnings.warn("Unable to convert '" + istring.strip() + "' to a float.")
         return 0
 
 
 def _triangle_vertex(elements_nodes, num_nodes_per_element, take_all_nodes=True):
     trg_vertex = []
     if num_nodes_per_element == 10 and take_all_nodes:
         for e in elements_nodes:
@@ -289,18 +314,19 @@
 
             elif new_line:
                 streamline.append(line.split(" "))
     return streamlines
 
 
 @pyaedt_function_handler()
+@update_plot_settings
 def plot_polar_chart(
-    plot_data, size=(2000, 1000), show_legend=True, xlabel="", ylabel="", title="", snapshot_path=None
+    plot_data, size=(2000, 1000), show_legend=True, xlabel="", ylabel="", title="", snapshot_path=None, show=True
 ):
-    """Create a matplotlib polar plot based on a list of data.
+    """Create a Matplotlib polar plot based on a list of data.
 
     Parameters
     ----------
     plot_data : list of list
         List of plot data. Every item has to be in the following format
         `[x points, y points, label]`.
     size : tuple, optional
@@ -308,17 +334,25 @@
     show_legend : bool
         Either to show legend or not.
     xlabel : str
         Plot X label.
     ylabel : str
         Plot Y label.
     title : str
-        Plot Title label.
+        Plot title label.
     snapshot_path : str
-        Full path to image file if a snapshot is needed.
+        Full path to the image file if a snapshot is needed.
+    show : bool, optional
+        Whether to render the figure. The default is ``True``. If ``False``, the
+        figure is not drawn.
+
+    Returns
+    -------
+    :class:`matplotlib.pyplot.Figure`
+        Matplotlib figure object.
     """
     dpi = 100.0
 
     ax = plt.subplot(111, projection="polar")
 
     label_id = 1
     legend = []
@@ -340,22 +374,23 @@
     if show_legend:
         ax.legend(legend)
 
     fig = plt.gcf()
     fig.set_size_inches(size[0] / dpi, size[1] / dpi)
     if snapshot_path:
         fig.savefig(snapshot_path)
-    else:
+    if show:
         fig.show()
     return fig
 
 
 @pyaedt_function_handler()
+@update_plot_settings
 def plot_3d_chart(plot_data, size=(2000, 1000), xlabel="", ylabel="", title="", snapshot_path=None):
-    """Create a matplotlib 3D plot based on a list of data.
+    """Create a Matplotlib 3D plot based on a list of data.
 
     Parameters
     ----------
     plot_data : list of list
         List of plot data. Every item has to be in the following format
         `[x points, y points, z points, label]`.
     size : tuple, optional
@@ -367,16 +402,16 @@
     title : str
         Plot Title label.
     snapshot_path : str
         Full path to image file if a snapshot is needed.
 
     Returns
     -------
-    :class:`matplotlib.plt`
-        Matplotlib fig object.
+    :class:`matplotlib.pyplot.Figure`
+        Matplotlib figure object.
     """
     dpi = 100.0
 
     ax = plt.subplot(111, projection="3d")
 
     if isinstance(plot_data[0], np.ndarray):
         x = plot_data[0]
@@ -399,17 +434,17 @@
         fig.savefig(snapshot_path)
     else:
         fig.show()
     return fig
 
 
 @pyaedt_function_handler()
+@update_plot_settings
 def plot_2d_chart(plot_data, size=(2000, 1000), show_legend=True, xlabel="", ylabel="", title="", snapshot_path=None):
-    """Create a matplotlib plot based on a list of data.
-
+    """Create a Matplotlib plot based on a list of data.
     Parameters
     ----------
     plot_data : list of list
         List of plot data. Every item has to be in the following format
         `[x points, y points, label]`.
     size : tuple, optional
         Image size in pixel (width, height).
@@ -423,16 +458,16 @@
         Plot Title label. The default value is ``""``.
     snapshot_path : str, optional
         Full path to image file if a snapshot is needed.
         The default value is ``None``.
 
     Returns
     -------
-    :class:`matplotlib.plt`
-        Matplotlib fig object.
+    :class:`matplotlib.pyplot.Figure`
+        Matplotlib figure object.
     """
     dpi = 100.0
     figsize = (size[0] / dpi, size[1] / dpi)
     fig, ax = plt.subplots(figsize=figsize)
     label_id = 1
     for plo_obj in plot_data:
         if len(plo_obj) == 3:
@@ -456,14 +491,15 @@
         fig.savefig(snapshot_path)
     elif not is_notebook():
         fig.show()
     return fig
 
 
 @pyaedt_function_handler()
+@update_plot_settings
 def plot_matplotlib(
     plot_data,
     size=(2000, 1000),
     show_legend=True,
     xlabel="",
     ylabel="",
     title="",
@@ -507,16 +543,16 @@
         Default is `None`.
     show : bool, optional
         Whether to show the plot or return the matplotlib object. Default is `True`.
 
 
     Returns
     -------
-    :class:`matplotlib.plt`
-        Matplotlib fig object.
+    :class:`matplotlib.pyplot.Figure`
+        Matplotlib Figure object.
     """
     dpi = 100.0
     figsize = (size[0] / dpi, size[1] / dpi)
     fig = plt.figure(figsize=figsize)
     ax = fig.add_subplot(1, 1, 1)
     if isinstance(plot_data, str):
         plot_data = ast.literal_eval(plot_data)
@@ -565,22 +601,25 @@
 
     if annotations:
         for annotation in annotations:
             plt.text(annotation[0], annotation[1], annotation[2], **annotation[3])
 
     if snapshot_path:
         plt.savefig(snapshot_path)
-    elif show:
+    if show:
         plt.show()
-    return plt
+    return fig
 
 
 @pyaedt_function_handler()
-def plot_contour(qty_to_plot, x, y, size=(2000, 1600), xlabel="", ylabel="", title="", levels=64, snapshot_path=None):
-    """Create a matplotlib contour plot.
+@update_plot_settings
+def plot_contour(
+    qty_to_plot, x, y, size=(2000, 1600), xlabel="", ylabel="", title="", levels=64, snapshot_path=None, show=True
+):
+    """Create a Matplotlib contour plot.
 
     Parameters
     ----------
     qty_to_plot : :class:`numpy.ndarray`
         Quantity to plot.
     x : :class:`numpy.ndarray`
         X axis quantity.
@@ -591,22 +630,25 @@
     xlabel : str, optional
         X Label. Default is `""`.
     ylabel : str, optional
         Y Label. Default is `""`.
     title : str, optional
         Plot Title Label. Default is `""`.
     levels : int, optional
-        Color map levels. Default is `64`.
+        Color map levels. The default is ``64``.
     snapshot_path : str, optional
-        Full path to image to save. Default is None.
+        Full path to save the image save. The default is ``None``.
+    show : bool, optional
+        Whether to render the figure. The default is ``True``. If
+        ``False``, the image is not drawn.
 
     Returns
     -------
-    :class:`matplotlib.plt`
-        Matplotlib fig object.
+    :class:`matplotlib.pyplot.Figure`
+        Matplotlib figure object.
     """
     dpi = 100.0
     figsize = (size[0] / dpi, size[1] / dpi)
     fig, ax = plt.subplots(figsize=figsize)
     if title:
         plt.title(title)
     if xlabel:
@@ -621,17 +663,17 @@
         levels=levels,
         cmap="jet",
     )
 
     plt.colorbar()
     if snapshot_path:
         plt.savefig(snapshot_path)
-    else:
+    if show:
         plt.show()
-    return plt
+    return fig
 
 
 class ObjClass(object):
     """Manages mesh files to be plotted in pyvista.
 
     Parameters
     ----------
```

### Comparing `pyaedt-0.9.0/pyaedt/generic/python_optimizers.py` & `pyaedt-0.9.1/pyaedt/generic/python_optimizers.py`

 * *Files identical despite different names*

### Comparing `pyaedt-0.9.0/pyaedt/generic/report_file_parser.py` & `pyaedt-0.9.1/pyaedt/generic/report_file_parser.py`

 * *Files identical despite different names*

### Comparing `pyaedt-0.9.0/pyaedt/generic/settings.py` & `pyaedt-0.9.1/pyaedt/generic/settings.py`

 * *Files identical despite different names*

### Comparing `pyaedt-0.9.0/pyaedt/generic/spisim.py` & `pyaedt-0.9.1/pyaedt/generic/spisim.py`

 * *Files 1% similar despite different names*

```diff
@@ -55,31 +55,36 @@
         exec_name = "SPISimJNI_LX64.exe" if is_linux else "SPISimJNI_WIN64.exe"
         spisimExe = os.path.join(self.desktop_install_dir, "spisim", "SPISim", "modules", "ext", exec_name)
 
         cfgCmmd = ""
         if touchstone_file != "":
             cfgCmmd = cfgCmmd + '-i "%s"' % touchstone_file
         if config_file != "":
-            cfgCmmd = '-v CFGFILE="%s"' % config_file
+            if is_linux:
+                cfgCmmd = "-v CFGFILE=%s" % config_file
+            else:
+                cfgCmmd = '-v CFGFILE="%s"' % config_file
         if out_file:
-            cfgCmmd += ' -o "%s"' % out_file
+            cfgCmmd += ', -o "%s"' % out_file
         command = [spisimExe, parameter, cfgCmmd]
         # Debug('%s %s' % (cmdList[0], ' '.join(arguments)))
         # try up to three times to be sure
         if out_file:
             out_processing = os.path.join(out_file, generate_unique_name("spsim_out") + ".txt")
         else:
             out_processing = os.path.join(generate_unique_folder_name(), generate_unique_name("spsim_out") + ".txt")
 
         my_env = os.environ.copy()
         my_env.update(settings.aedt_environment_variables)
+
         if is_linux:  # pragma: no cover
-            if "ANSYSEM_ROOT_PATH" not in my_env:
+            if "ANSYSEM_ROOT_PATH" not in my_env:  # pragma: no cover
                 my_env["ANSYSEM_ROOT_PATH"] = self.desktop_install_dir
-            command.append("&")
+            if "SPISIM_OUTPUT_LOG" not in my_env:  # pragma: no cover
+                my_env["SPISIM_OUTPUT_LOG"] = os.path.join(out_file, generate_unique_name("spsim_out") + ".log")
             with open_file(out_processing, "w") as outfile:
                 subprocess.Popen(command, env=my_env, stdout=outfile, stderr=outfile).wait()  # nosec
         else:
             with open_file(out_processing, "w") as outfile:
                 subprocess.Popen(" ".join(command), env=my_env, stdout=outfile, stderr=outfile).wait()  # nosec
         return out_processing
```

### Comparing `pyaedt-0.9.0/pyaedt/generic/touchstone_parser.py` & `pyaedt-0.9.1/pyaedt/generic/touchstone_parser.py`

 * *Files 2% similar despite different names*

```diff
@@ -522,17 +522,22 @@
         else:
             genequiv_path = os.path.join(aedt_install_folder, "genequiv")
         cmd = [genequiv_path]
         if passivity:
             cmd.append("-checkpassivity")
         if causality:
             cmd.append("-checkcausality")
+
         cmd.append(sNpFiles[snpf])
-        output_str = str(subprocess.Popen(cmd, stdout=subprocess.PIPE).communicate()[0])
+        my_env = os.environ.copy()
+        p = subprocess.Popen(cmd, shell=True, stdout=subprocess.PIPE, stderr=subprocess.PIPE, env=my_env)  # nosec
+        output = p.communicate()
+        output_str = str(output[0])
         output_lst = output_str.split("\\r\\n")
+
         if len(output_lst) == 1:
             output_lst = output_str.splitlines()
         for line in output_lst:
             if "Input data" in line and passivity:
                 msg_log = line[17:]
                 is_passive = True
                 if "non-passive" in msg_log:
```

### Comparing `pyaedt-0.9.0/pyaedt/hfss.py` & `pyaedt-0.9.1/pyaedt/hfss.py`

 * *Files 1% similar despite different names*

```diff
@@ -5233,21 +5233,22 @@
         if len(self.oboundary.GetDiffPairs()) == num_old_pairs + 1:
             return True
         else:
             return False
 
     @pyaedt_function_handler(array_name="name", json_file="input_data")
     def add_3d_component_array_from_json(self, input_data, name=None):
-        """Add or edit a 3D component array from a JSON file or TOML file.
+        """Add or edit a 3D component array from a JSON file, TOML file, or dictionary.
         The 3D component is placed in the layout if it is not present.
 
         Parameters
         ----------
         input_data : str, dict
-            Full path to either the JSON file or dictionary containing the array information.
+            Full path to either the JSON file, TOML file, or the dictionary
+            containing the array information.
         name : str, optional
              Name of the boundary to add or edit.
 
         Returns
         -------
         class:`pyaedt.modeler.cad.component_array.ComponentArray`
 
@@ -5413,16 +5414,19 @@
     def get_antenna_ffd_solution_data(
         self,
         frequencies,
         setup=None,
         sphere=None,
         variations=None,
         overwrite=True,
+        link_to_hfss=True,
     ):
-        """Export antennas parameters to Far Field Data (FFD) files and return the ``FfdSolutionDataExporter`` object.
+        """Export the antenna parameters to Far Field Data (FFD) files and return an
+        instance of the
+        ``FfdSolutionDataExporter`` object.
 
         For phased array cases, only one phased array is calculated.
 
         Parameters
         ----------
         frequencies : float, list
             Frequency value or list of frequencies to compute far field data.
@@ -5431,20 +5435,28 @@
         sphere : str, optional
             Infinite sphere to use. The default is ``None``, in which case an existing sphere is used or a new
             one is created.
         variations : dict, optional
             Variation dictionary.
         overwrite : bool, optional
             Whether to overwrite FFD files. The default is ``True``.
+        link_to_hfss : bool, optional
+            Whether to return an instance of the
+            :class:`pyaedt.modules.solutions.FfdSolutionDataExporter` class,
+            which requires a connection to an instance of the :class:`Hfss` class.
+            The default is `` True``. If ``False``, returns an instance of
+            :class:`pyaedt.modules.solutions.FfdSolutionData` class, which is
+            independent from the running HFSS instance.
 
         Returns
         -------
         :class:`pyaedt.modules.solutions.FfdSolutionDataExporter`
             SolutionData object.
         """
+        from pyaedt.modules.solutions import FfdSolutionData
         from pyaedt.modules.solutions import FfdSolutionDataExporter
 
         if not variations:
             variations = self.available_variations.nominal_w_values_dict_w_dependent
         if not setup:
             setup = self.nominal_adaptive
         if sphere:
@@ -5463,22 +5475,28 @@
         else:
             sphere = "Infinite Sphere1"
             self.insert_infinite_sphere(
                 x_start=0, x_stop=180, x_step=5, y_start=-180, y_stop=180, y_step=5, name=sphere
             )
             self.logger.info("Far field sphere %s is created.", setup)
 
-        return FfdSolutionDataExporter(
+        ffd = FfdSolutionDataExporter(
             self,
             sphere_name=sphere,
             setup_name=setup,
             frequencies=frequencies,
             variations=variations,
             overwrite=overwrite,
         )
+        if link_to_hfss:
+            return ffd
+        else:
+            eep_file = ffd.eep_files
+            frequencies = ffd.frequencies
+            return FfdSolutionData(frequencies=frequencies, eep_files=eep_file)
 
     @pyaedt_function_handler()
     def set_material_threshold(self, threshold=100000):
         """Set the material conductivity threshold.
 
         Parameters
         ----------
```

### Comparing `pyaedt-0.9.0/pyaedt/hfss3dlayout.py` & `pyaedt-0.9.1/pyaedt/hfss3dlayout.py`

 * *Files identical despite different names*

### Comparing `pyaedt-0.9.0/pyaedt/icepak.py` & `pyaedt-0.9.1/pyaedt/icepak.py`

 * *Files identical despite different names*

### Comparing `pyaedt-0.9.0/pyaedt/maxwell.py` & `pyaedt-0.9.1/pyaedt/maxwell.py`

 * *Files identical despite different names*

### Comparing `pyaedt-0.9.0/pyaedt/maxwellcircuit.py` & `pyaedt-0.9.1/pyaedt/maxwellcircuit.py`

 * *Files identical despite different names*

### Comparing `pyaedt-0.9.0/pyaedt/mechanical.py` & `pyaedt-0.9.1/pyaedt/mechanical.py`

 * *Files identical despite different names*

### Comparing `pyaedt-0.9.0/pyaedt/misc/Job_Settings.areg` & `pyaedt-0.9.1/pyaedt/misc/Job_Settings.areg`

 * *Files identical despite different names*

### Comparing `pyaedt-0.9.0/pyaedt/misc/amat.xml` & `pyaedt-0.9.1/pyaedt/misc/amat.xml`

 * *Files identical despite different names*

### Comparing `pyaedt-0.9.0/pyaedt/misc/ansys_cloud.areg` & `pyaedt-0.9.1/pyaedt/misc/ansys_cloud.areg`

 * *Files identical despite different names*

### Comparing `pyaedt-0.9.0/pyaedt/misc/config.schema.json` & `pyaedt-0.9.1/pyaedt/misc/config.schema.json`

 * *Files identical despite different names*

### Comparing `pyaedt-0.9.0/pyaedt/misc/misc.py` & `pyaedt-0.9.1/pyaedt/misc/misc.py`

 * *Files identical despite different names*

### Comparing `pyaedt-0.9.0/pyaedt/misc/ml_data_file_train_100MHz_1GHz.json` & `pyaedt-0.9.1/pyaedt/misc/ml_data_file_train_100MHz_1GHz.json`

 * *Files identical despite different names*

### Comparing `pyaedt-0.9.0/pyaedt/misc/ml_data_file_train_1GHz_10GHz.json` & `pyaedt-0.9.1/pyaedt/misc/ml_data_file_train_1GHz_10GHz.json`

 * *Files identical despite different names*

### Comparing `pyaedt-0.9.0/pyaedt/misc/patch_svr_model_100MHz_1GHz.joblib` & `pyaedt-0.9.1/pyaedt/misc/patch_svr_model_100MHz_1GHz.joblib`

 * *Files identical despite different names*

### Comparing `pyaedt-0.9.0/pyaedt/misc/patch_svr_model_1GHz_10GHz.joblib` & `pyaedt-0.9.1/pyaedt/misc/patch_svr_model_1GHz_10GHz.joblib`

 * *Files identical despite different names*

### Comparing `pyaedt-0.9.0/pyaedt/misc/pyaedt_local_config.acf` & `pyaedt-0.9.1/pyaedt/misc/pyaedt_local_config.acf`

 * *Files identical despite different names*

### Comparing `pyaedt-0.9.0/pyaedt/misc/pyansys-logo-black-cropped.png` & `pyaedt-0.9.1/pyaedt/misc/pyansys-logo-black-cropped.png`

 * *Files identical despite different names*

### Comparing `pyaedt-0.9.0/pyaedt/misc/spisim_com_configuration_files/com_120d_8.json` & `pyaedt-0.9.1/pyaedt/misc/spisim_com_configuration_files/com_120d_8.json`

 * *Files identical despite different names*

### Comparing `pyaedt-0.9.0/pyaedt/misc/spisim_com_configuration_files/com_93_8.json` & `pyaedt-0.9.1/pyaedt/misc/spisim_com_configuration_files/com_93_8.json`

 * *Files identical despite different names*

### Comparing `pyaedt-0.9.0/pyaedt/misc/spisim_com_configuration_files/com_94_17.json` & `pyaedt-0.9.1/pyaedt/misc/spisim_com_configuration_files/com_94_17.json`

 * *Files identical despite different names*

### Comparing `pyaedt-0.9.0/pyaedt/misc/spisim_com_configuration_files/com_parameters.py` & `pyaedt-0.9.1/pyaedt/misc/spisim_com_configuration_files/com_parameters.py`

 * *Files identical despite different names*

### Comparing `pyaedt-0.9.0/pyaedt/misc/spisim_com_configuration_files/com_settings_mapping.py` & `pyaedt-0.9.1/pyaedt/misc/spisim_com_configuration_files/com_settings_mapping.py`

 * *Files identical despite different names*

### Comparing `pyaedt-0.9.0/pyaedt/misc/template.acf` & `pyaedt-0.9.1/pyaedt/misc/template.acf`

 * *Files identical despite different names*

### Comparing `pyaedt-0.9.0/pyaedt/modeler/advanced_cad/actors.py` & `pyaedt-0.9.1/pyaedt/modeler/advanced_cad/actors.py`

 * *Files identical despite different names*

### Comparing `pyaedt-0.9.0/pyaedt/modeler/advanced_cad/multiparts.py` & `pyaedt-0.9.1/pyaedt/modeler/advanced_cad/multiparts.py`

 * *Files identical despite different names*

### Comparing `pyaedt-0.9.0/pyaedt/modeler/advanced_cad/oms.py` & `pyaedt-0.9.1/pyaedt/modeler/advanced_cad/oms.py`

 * *Files identical despite different names*

### Comparing `pyaedt-0.9.0/pyaedt/modeler/advanced_cad/parts.py` & `pyaedt-0.9.1/pyaedt/modeler/advanced_cad/parts.py`

 * *Files identical despite different names*

### Comparing `pyaedt-0.9.0/pyaedt/modeler/advanced_cad/stackup_3d.py` & `pyaedt-0.9.1/pyaedt/modeler/advanced_cad/stackup_3d.py`

 * *Files identical despite different names*

### Comparing `pyaedt-0.9.0/pyaedt/modeler/cad/Modeler.py` & `pyaedt-0.9.1/pyaedt/modeler/cad/Modeler.py`

 * *Files identical despite different names*

### Comparing `pyaedt-0.9.0/pyaedt/modeler/cad/Primitives.py` & `pyaedt-0.9.1/pyaedt/modeler/cad/Primitives.py`

 * *Files identical despite different names*

### Comparing `pyaedt-0.9.0/pyaedt/modeler/cad/Primitives2D.py` & `pyaedt-0.9.1/pyaedt/modeler/cad/Primitives2D.py`

 * *Files identical despite different names*

### Comparing `pyaedt-0.9.0/pyaedt/modeler/cad/Primitives3D.py` & `pyaedt-0.9.1/pyaedt/modeler/cad/Primitives3D.py`

 * *Files identical despite different names*

### Comparing `pyaedt-0.9.0/pyaedt/modeler/cad/component_array.py` & `pyaedt-0.9.1/pyaedt/modeler/cad/component_array.py`

 * *Files identical despite different names*

### Comparing `pyaedt-0.9.0/pyaedt/modeler/cad/components_3d.py` & `pyaedt-0.9.1/pyaedt/modeler/cad/components_3d.py`

 * *Files identical despite different names*

### Comparing `pyaedt-0.9.0/pyaedt/modeler/cad/elements3d.py` & `pyaedt-0.9.1/pyaedt/modeler/cad/elements3d.py`

 * *Files identical despite different names*

### Comparing `pyaedt-0.9.0/pyaedt/modeler/cad/object3d.py` & `pyaedt-0.9.1/pyaedt/modeler/cad/object3d.py`

 * *Files identical despite different names*

### Comparing `pyaedt-0.9.0/pyaedt/modeler/cad/polylines.py` & `pyaedt-0.9.1/pyaedt/modeler/cad/polylines.py`

 * *Files identical despite different names*

### Comparing `pyaedt-0.9.0/pyaedt/modeler/calculators.py` & `pyaedt-0.9.1/pyaedt/modeler/calculators.py`

 * *Files identical despite different names*

### Comparing `pyaedt-0.9.0/pyaedt/modeler/circuits/PrimitivesCircuit.py` & `pyaedt-0.9.1/pyaedt/modeler/circuits/PrimitivesCircuit.py`

 * *Files 0% similar despite different names*

```diff
@@ -399,14 +399,16 @@
                     line = file.readline()
             else:  # pragma: no cover
                 portnames = ["Port" + str(n) for n in range(1, num_terminal + 1)]
             return portnames
 
         if not model_name:
             model_name = os.path.splitext(os.path.basename(input_file))[0]
+            if "." in model_name:
+                model_name = model_name.replace(".", "_")
         if model_name in list(self.o_model_manager.GetNames()):
             model_name = generate_unique_name(model_name, n=2)
         num_terminal = int(os.path.splitext(input_file)[1].lower().strip(".sp"))
         # with open_file(touchstone_full_path, "r") as f:
         # port_names = _parse_ports_name(f, num_terminal)
 
         port_names = []
```

### Comparing `pyaedt-0.9.0/pyaedt/modeler/circuits/PrimitivesEmit.py` & `pyaedt-0.9.1/pyaedt/modeler/circuits/PrimitivesEmit.py`

 * *Files identical despite different names*

### Comparing `pyaedt-0.9.0/pyaedt/modeler/circuits/PrimitivesMaxwellCircuit.py` & `pyaedt-0.9.1/pyaedt/modeler/circuits/PrimitivesMaxwellCircuit.py`

 * *Files identical despite different names*

### Comparing `pyaedt-0.9.0/pyaedt/modeler/circuits/PrimitivesNexxim.py` & `pyaedt-0.9.1/pyaedt/modeler/circuits/PrimitivesNexxim.py`

 * *Files identical despite different names*

### Comparing `pyaedt-0.9.0/pyaedt/modeler/circuits/PrimitivesTwinBuilder.py` & `pyaedt-0.9.1/pyaedt/modeler/circuits/PrimitivesTwinBuilder.py`

 * *Files identical despite different names*

### Comparing `pyaedt-0.9.0/pyaedt/modeler/circuits/object3dcircuit.py` & `pyaedt-0.9.1/pyaedt/modeler/circuits/object3dcircuit.py`

 * *Files 1% similar despite different names*

```diff
@@ -1,12 +1,13 @@
 # -*- coding: utf-8 -*-
 from __future__ import absolute_import
 
 from collections import OrderedDict
 import math
+import time
 
 from pyaedt import pyaedt_function_handler
 from pyaedt.application.Variables import decompose_variable_value
 from pyaedt.generic.constants import AEDT_UNITS
 from pyaedt.generic.general_methods import _arg2dict
 from pyaedt.generic.general_methods import _dim_arg
 from pyaedt.modeler.cad.elements3d import _dict2arg
@@ -867,14 +868,46 @@
             vGeo3dlayout = ["NAME:" + tabname, vPropServers, vChangedProps]
             vOut = ["NAME:AllTabs", vGeo3dlayout]
             if "NAME:Component Location" in str(vChangedProps) and "PagePort" not in self.composed_name:
                 self._oeditor.ChangeProperty(vOut)
             return self._oeditor.ChangeProperty(vOut)
         return False
 
+    @pyaedt_function_handler()
+    def enforce_touchstone_model_passive(self):
+        """Enforce touchstone model passive.
+
+        Returns
+        -------
+        bool
+            ``True`` when successful, ``False`` when failed.
+
+        References
+        ----------
+
+        >>> oModelManager.EditWithComps
+        """
+        props = self.model_data.props
+        passive = OrderedDict(
+            [
+                ("DCOption", -1),
+                ("InterpOption", 1),
+                ("ExtrapOption", 3),
+                ("Convolution", 0),
+                ("Passivity", 6),
+                ("Reciprocal", False),
+                ("ModelOption", ""),
+                ("DataType", 2),
+            ]
+        )
+        props["NexximCustomization"] = passive
+        props["ModTime"] = int(time.time())
+        self.model_data.props = props
+        return self.model_data.update()
+
 
 class Wire(object):
     """Creates and manipulates a wire."""
 
     def __init__(self, modeler):
         self._app = modeler._app
         self._modeler = modeler
```

### Comparing `pyaedt-0.9.0/pyaedt/modeler/geometry_operators.py` & `pyaedt-0.9.1/pyaedt/modeler/geometry_operators.py`

 * *Files identical despite different names*

### Comparing `pyaedt-0.9.0/pyaedt/modeler/modeler2d.py` & `pyaedt-0.9.1/pyaedt/modeler/modeler2d.py`

 * *Files identical despite different names*

### Comparing `pyaedt-0.9.0/pyaedt/modeler/modeler3d.py` & `pyaedt-0.9.1/pyaedt/modeler/modeler3d.py`

 * *Files 1% similar despite different names*

```diff
@@ -211,15 +211,15 @@
             component_outline,
         ]
         if object_list:
             objs = object_list
         else:
             native_objs = [obj.name for _, v in self.user_defined_components.items() for _, obj in v.parts.items()]
             objs = [obj for obj in self.object_names if obj not in native_objs]
-            if not native_components and native_objs:
+            if not native_components and native_objs and not auxiliary_dict:
                 self.logger.warning(
                     "Native component objects cannot be exported. Use native_components argument to"
                     " export an auxiliary dictionary file containing 3D components information"
                 )
         for el in objs:
             if "CreateRegion:1" in self.oeditor.GetChildObject(el).GetChildNames():
                 objs.remove(el)
@@ -943,21 +943,21 @@
                 elif line_type in ["GRID", "CTRIA3"]:
                     grid_id = int(line[8:16])
                     if line_type == "CTRIA3":
                         tria_id = int(line[16:24])
                         if tria_id not in nas_to_dict["Triangles"]:
                             nas_to_dict["Triangles"][tria_id] = []
                     n1 = line[24:32].strip()
-                    if "-" in n1[1:]:
+                    if "-" in n1[1:] and "e" not in n1[1:].lower():
                         n1 = n1[0] + n1[1:].replace("-", "e-")
                     n2 = line[32:40].strip()
-                    if "-" in n2[1:]:
+                    if "-" in n2[1:] and "e" not in n2[1:].lower():
                         n2 = n2[0] + n2[1:].replace("-", "e-")
                     n3 = line[40:48].strip()
-                    if "-" in n3[1:]:
+                    if "-" in n3[1:] and "e" not in n3[1:].lower():
                         n3 = n3[0] + n3[1:].replace("-", "e-")
                     if line_type == "GRID":
                         nas_to_dict["Points"][grid_id] = [float(n1), float(n2), float(n3)]
                         nas_to_dict["PointsId"][grid_id] = grid_id
                         id += 1
                     else:
                         tri = [int(n1), int(n2), int(n3)]
@@ -966,28 +966,31 @@
                 elif line_type in ["GRID*", "CTRIA3*"]:
                     grid_id = int(line[8:24])
                     if line_type == "CTRIA3*":
                         tria_id = int(line[24:40])
                         if tria_id not in nas_to_dict["Triangles"]:
                             nas_to_dict["Triangles"][tria_id] = []
                     n1 = line[40:56].strip()
-                    if "-" in n1[1:]:
+                    if "-" in n1[1:] and "e" not in n1[1:].lower():
                         n1 = n1[0] + n1[1:].replace("-", "e-")
                     n2 = line[56:72].strip()
-                    if "-" in n2[1:]:
+                    if "-" in n2[1:] and "e" not in n2[1:].lower():
                         n2 = n2[0] + n2[1:].replace("-", "e-")
 
                     n3 = line[72:88].strip()
                     if not n3 or n3.startswith("*"):
                         lk += 1
                         n3 = lines[lk][8:24].strip()
-                    if "-" in n3[1:]:
+                    if "-" in n3[1:] and "e" not in n3[1:].lower():
                         n3 = n3[0] + n3[1:].replace("-", "e-")
                     if line_type == "GRID*":
-                        nas_to_dict["Points"][grid_id] = [float(n1), float(n2), float(n3)]
+                        try:
+                            nas_to_dict["Points"][grid_id] = [float(n1), float(n2), float(n3)]
+                        except Exception:  # nosec
+                            continue
                         nas_to_dict["PointsId"][grid_id] = id
                         id += 1
                     else:
                         tri = (int(n1), int(n2), int(n3))
                         nas_to_dict["Triangles"][tria_id].append(tri)
 
                 elif line_type in ["CPENTA", "CHEXA", "CTETRA"]:
@@ -1046,15 +1049,15 @@
                     if obj_id in nas_to_dict["Lines"]:
                         nas_to_dict["Lines"][obj_id].append([n1, n2])
                     else:
                         nas_to_dict["Lines"][obj_id] = [[n1, n2]]
 
         self.logger.info_timer("File loaded")
         objs_before = [i for i in self.object_names]
-        if nas_to_dict["Triangles"]:
+        if nas_to_dict["Triangles"] or nas_to_dict["Solids"] or nas_to_dict["Lines"]:
             self.logger.reset_timer()
             self.logger.info("Creating STL file with detected faces")
             f = open(os.path.join(self._app.working_directory, self._app.design_name + "_test.stl"), "w")
             for tri_id, triangles in nas_to_dict["Triangles"].items():
                 f.write("solid Sheet_{}\n".format(tri_id))
                 for triangle in triangles:
                     _write_solid_stl(triangle, nas_to_dict)
@@ -1065,26 +1068,29 @@
 
                 df = pd.Series(solid_triangles)
                 undulicated_values = df.drop_duplicates(keep=False).to_list()
                 for triangle in undulicated_values:
                     _write_solid_stl(triangle, nas_to_dict)
                 f.write("endsolid\n")
             f.close()
-            self.logger.info("STL file created")
+            self.logger.info_timer("STL file created")
+            self._app.odesktop.CloseAllWindows()
+            self.logger.reset_timer()
+            self.logger.info("Importing STL in 3D Modeler")
             self.import_3d_cad(
                 os.path.join(self._app.working_directory, self._app.design_name + "_test.stl"),
                 create_lightweigth_part=import_as_light_weight,
             )
             for el in nas_to_dict["Solids"].keys():
                 obj_names = [i for i in self.object_names if i.startswith("Solid_{}".format(el))]
                 self.create_group(obj_names, group_name=str(el))
             for el in nas_to_dict["Triangles"].keys():
                 obj_names = [i for i in self.object_names if i.startswith("Sheet_{}".format(el))]
                 self.create_group(obj_names, group_name=str(el))
-            self.logger.info_timer("Faces imported")
+            self.logger.info_timer("Model imported")
 
         if import_lines:
             for line_name, lines in nas_to_dict["Lines"].items():
                 if lines_thickness:
                     self._app["x_section_{}".format(line_name)] = lines_thickness
                 polys = []
                 id = 0
@@ -1110,14 +1116,15 @@
                 if len(polys) > 1:
                     out_poly = self.unite(polys, purge=not lines_thickness)
                     if not lines_thickness and out_poly:
                         self.generate_object_history(out_poly)
 
         objs_after = [i for i in self.object_names]
         new_objects = [self[i] for i in objs_after if i not in objs_before]
+        self._app.oproject.SetActiveDesign(self._app.design_name)
         return new_objects
 
     @pyaedt_function_handler()
     def import_from_openstreet_map(
         self,
         latitude_longitude,
         env_name="default",
```

### Comparing `pyaedt-0.9.0/pyaedt/modeler/modelerpcb.py` & `pyaedt-0.9.1/pyaedt/modeler/modelerpcb.py`

 * *Files identical despite different names*

### Comparing `pyaedt-0.9.0/pyaedt/modeler/pcb/Primitives3DLayout.py` & `pyaedt-0.9.1/pyaedt/modeler/pcb/Primitives3DLayout.py`

 * *Files identical despite different names*

### Comparing `pyaedt-0.9.0/pyaedt/modeler/pcb/object3dlayout.py` & `pyaedt-0.9.1/pyaedt/modeler/pcb/object3dlayout.py`

 * *Files identical despite different names*

### Comparing `pyaedt-0.9.0/pyaedt/modeler/schematic.py` & `pyaedt-0.9.1/pyaedt/modeler/schematic.py`

 * *Files identical despite different names*

### Comparing `pyaedt-0.9.0/pyaedt/modules/AdvancedPostProcessing.py` & `pyaedt-0.9.1/pyaedt/modules/AdvancedPostProcessing.py`

 * *Files identical despite different names*

### Comparing `pyaedt-0.9.0/pyaedt/modules/Boundary.py` & `pyaedt-0.9.1/pyaedt/modules/Boundary.py`

 * *Files identical despite different names*

### Comparing `pyaedt-0.9.0/pyaedt/modules/CableModeling.py` & `pyaedt-0.9.1/pyaedt/modules/CableModeling.py`

 * *Files identical despite different names*

### Comparing `pyaedt-0.9.0/pyaedt/modules/CircuitTemplates.py` & `pyaedt-0.9.1/pyaedt/modules/CircuitTemplates.py`

 * *Files identical despite different names*

### Comparing `pyaedt-0.9.0/pyaedt/modules/DesignXPloration.py` & `pyaedt-0.9.1/pyaedt/modules/DesignXPloration.py`

 * *Files identical despite different names*

### Comparing `pyaedt-0.9.0/pyaedt/modules/LayerStackup.py` & `pyaedt-0.9.1/pyaedt/modules/LayerStackup.py`

 * *Files identical despite different names*

### Comparing `pyaedt-0.9.0/pyaedt/modules/Material.py` & `pyaedt-0.9.1/pyaedt/modules/Material.py`

 * *Files identical despite different names*

### Comparing `pyaedt-0.9.0/pyaedt/modules/MaterialLib.py` & `pyaedt-0.9.1/pyaedt/modules/MaterialLib.py`

 * *Files identical despite different names*

### Comparing `pyaedt-0.9.0/pyaedt/modules/Mesh.py` & `pyaedt-0.9.1/pyaedt/modules/Mesh.py`

 * *Files identical despite different names*

### Comparing `pyaedt-0.9.0/pyaedt/modules/Mesh3DLayout.py` & `pyaedt-0.9.1/pyaedt/modules/Mesh3DLayout.py`

 * *Files identical despite different names*

### Comparing `pyaedt-0.9.0/pyaedt/modules/MeshIcepak.py` & `pyaedt-0.9.1/pyaedt/modules/MeshIcepak.py`

 * *Files 1% similar despite different names*

```diff
@@ -1063,16 +1063,21 @@
                             MeshOperation(
                                 self,
                                 ds,
                                 self._app.design_properties["MeshRegion"]["MeshSetup"]["MeshOperations"][ds],
                                 "Icepak",
                             )
                         )
-        except Exception as e:
-            self._app.logger.error(e)
+        except TypeError:
+            # design_properties not loaded, maybe there are mesh region, we need to warn the user
+            self._app.logger.warning("No mesh operation found.")
+            self._app.logger.debug("Failed to get mesh operation from `design_properties`.")
+        except KeyError:
+            # design_properties loaded, mesh region related keys missing, no need to warn the user
+            self._app.logger.debug("Failed to get mesh operation.")
 
         return meshops
 
     @pyaedt_function_handler()
     def _get_design_mesh_regions(self):
         """Retrieve design mesh regions."""
         meshops = []
@@ -1100,16 +1105,21 @@
                             meshop = GlobalMeshRegion(self._app)
                         else:
                             meshop = MeshRegion(self._app, None, ds)
                         for el in dict_prop:
                             if el in meshop.__dict__:
                                 meshop.__dict__[el] = dict_prop[el]
                         meshops.append(meshop)
-        except Exception as e:
-            self._app.logger.error(e)
+        except TypeError:
+            # design_properties not loaded, maybe there are mesh region, we need to warn the user
+            self._app.logger.warning("No mesh region found.")
+            self._app.logger.debug("Failed to get mesh region from `design_properties`.")
+        except KeyError:
+            # design_properties loaded, mesh region related keys missing, no need to warn the user
+            self._app.logger.debug("Failed to get mesh region.")
 
         return meshops
 
     @pyaedt_function_handler(meshop_name="name")
     def assign_mesh_level(self, mesh_order, name=None):
         """Assign a mesh level to objects.
```

### Comparing `pyaedt-0.9.0/pyaedt/modules/OptimetricsTemplates.py` & `pyaedt-0.9.1/pyaedt/modules/OptimetricsTemplates.py`

 * *Files identical despite different names*

### Comparing `pyaedt-0.9.0/pyaedt/modules/PostProcessor.py` & `pyaedt-0.9.1/pyaedt/modules/PostProcessor.py`

 * *Files 0% similar despite different names*

```diff
@@ -2533,19 +2533,20 @@
         if intrinsics:
             if "Transient" in solution:  # pragma: no cover
                 variation.append("Time:=")
                 variation.append(intrinsics)
             else:
                 variation.append("Freq:=")
                 variation.append(intrinsics)
-                variation.append("Phase:=")
-                if phase:  # pragma: no cover
-                    variation.append(phase)
-                else:
-                    variation.append("0deg")
+                if self._app.design_type not in ["Icepak", "Mechanical", "Q3D Extractor"]:
+                    variation.append("Phase:=")
+                    if phase:  # pragma: no cover
+                        variation.append(phase)
+                    else:
+                        variation.append("0deg")
 
         file_name = os.path.join(self._app.working_directory, generate_unique_name("temp_fld") + ".fld")
         self.ofieldsreporter.CalculatorWrite(file_name, ["Solution:=", solution], variation)
         value = None
         if os.path.exists(file_name) or settings.remote_rpc_session:
             with open_file(file_name, "r") as f:
                 lines = f.readlines()
@@ -2715,19 +2716,20 @@
         if intrinsics:
             if "Transient" in solution:
                 variation.append("Time:=")
                 variation.append(intrinsics)
             else:
                 variation.append("Freq:=")
                 variation.append(intrinsics)
-                variation.append("Phase:=")
-                if phase:
-                    variation.append(phase)
-                else:
-                    variation.append("0deg")
+                if self._app.design_type not in ["Icepak", "Mechanical", "Q3D Extractor"]:
+                    variation.append("Phase:=")
+                    if phase:
+                        variation.append(phase)
+                    else:
+                        variation.append("0deg")
 
         export_options = [
             "NAME:ExportOption",
             "IncludePtInOutput:=",
             export_with_sample_points,
             "RefCSName:=",
             reference_coordinate_system,
@@ -2866,19 +2868,20 @@
         if intrinsics:
             if "Transient" in solution:
                 variation.append("Time:=")
                 variation.append(intrinsics)
             else:
                 variation.append("Freq:=")
                 variation.append(intrinsics)
-                variation.append("Phase:=")
-                if phase:
-                    variation.append(phase)
-                else:
-                    variation.append("0deg")
+                if self._app.design_type not in ["Icepak", "Mechanical", "Q3D Extractor"]:
+                    variation.append("Phase:=")
+                    if phase:
+                        variation.append(phase)
+                    else:
+                        variation.append("0deg")
         if not sample_points_file and not sample_points:
             if objects_type == "Vol":
                 self.ofieldsreporter.EnterVol(assignment)
             elif objects_type == "Surf":
                 self.ofieldsreporter.EnterSurf(assignment)
             else:
                 self.logger.error("No correct choice.")
@@ -4704,14 +4707,35 @@
         vrt.start_index = ray_index_start
         vrt.stop_index = ray_index_stop
         vrt.step_index = ray_index_step
         vrt.ray_box = ray_box
         vrt.create()
         return vrt
 
+    @pyaedt_function_handler()
+    def set_tuning_offset(self, setup, offsets):
+        """Set derivative variable to a specific offset value.
+
+        Parameters
+        ----------
+        setup : str
+            Setup name.
+        offsets : dict
+            Dictionary containing the variable name and it's offset value.
+
+        Returns
+        -------
+        bool
+        """
+        setup_obj = self._app.get_setup(setup)
+        if setup_obj and "set_tuning_offset" in dir(setup_obj):
+            return setup_obj.set_tuning_offset(offsets)
+        self.logger.error("Tuning offset applies only to solved setup with derivatives enabled.")
+        return False
+
 
 class CircuitPostProcessor(PostProcessorCommon, object):
     """Manages the main AEDT Nexxim postprocessing functions.
 
 
     .. note::
        Some functionalities are available only when AEDT is running in the graphical mode.
```

### Comparing `pyaedt-0.9.0/pyaedt/modules/SetupTemplates.py` & `pyaedt-0.9.1/pyaedt/modules/SetupTemplates.py`

 * *Files identical despite different names*

### Comparing `pyaedt-0.9.0/pyaedt/modules/SolveSetup.py` & `pyaedt-0.9.1/pyaedt/modules/SolveSetup.py`

 * *Files 2% similar despite different names*

```diff
@@ -383,15 +383,14 @@
             Name of the plot. The default is ``None``.
         polyline_points : int, optional,
             Number of points for creating the report for plots on polylines.
         subdesign_id : int, optional
             Specify a subdesign ID to export a Touchstone file of this subdesign to.
             This parameter is valid only for a circuit.
             The default value is ``None``.
-        context : str, optional
         sweep : str, optional
             Name of the sweep adaptive setup to get solutions from. The default is ``LastAdaptive``.
 
         Returns
         -------
         :class:`pyaedt.modules.report_templates.Standard`
             ``True`` when successful, ``False`` when failed.
@@ -2316,14 +2315,44 @@
         if not isinstance(derivative_list, list):
             derivative_list = [derivative_list]
         self.auto_update = False
         self.props["VariablesForDerivatives"] = derivative_list + self.get_derivative_variables()
         self.auto_update = True
         return self.update()
 
+    @pyaedt_function_handler()
+    def set_tuning_offset(self, offsets):
+        """Set derivative variable to a specific offset value.
+
+        Parameters
+        ----------
+        offsets : dict
+            Dictionary containing the variable name and it's offset value.
+
+        Returns
+        -------
+        bool
+        """
+        variables = self.get_derivative_variables()
+        for v in variables:
+            if v not in offsets:
+                offsets[v] = 0
+        arg = []
+        for k, v in offsets.items():
+            arg.append("DeltaOffset({})".format(k))
+            arg.append("{}".format(abs(self._app.variable_manager[k].numeric_value) * (-0.1)))
+            arg.append("{}".format(v))
+            arg.append("{}".format(abs(self._app.variable_manager[k].numeric_value) * 0.1))
+        if self.is_solved:
+            self._app.osolution.SetTuningOffsets(["TuningRanges:=", arg])
+            return True
+        else:
+            self._app.logger.error("Setup {} is not solved. Solve it before tuning variables.".format(self.name))
+            return False
+
     @pyaedt_function_handler(freqstart="start_frequency", freqstop="stop_frequency", sweepname="name")
     def create_frequency_sweep(
         self,
         unit=None,
         start_frequency=1.0,
         stop_frequency=10.0,
         num_of_freq_points=None,
@@ -2913,14 +2942,44 @@
         if not isinstance(derivative_list, list):
             derivative_list = [derivative_list]
         self.auto_update = False
         self.props["VariablesForDerivatives"] = derivative_list + self.get_derivative_variables()
         self.auto_update = True
         return self.update()
 
+    @pyaedt_function_handler()
+    def set_tuning_offset(self, offsets):
+        """Set derivative variable to a specific offset value.
+
+        Parameters
+        ----------
+        offsets : dict
+            Dictionary containing the variable name and it's offset value.
+
+        Returns
+        -------
+        bool
+        """
+        variables = self.get_derivative_variables()
+        for v in variables:
+            if v not in offsets:
+                offsets[v] = 0
+        arg = []
+        for k, v in offsets.items():
+            arg.append("DeltaOffset({})".format(k))
+            arg.append("{}".format(abs(self._app.variable_manager[k].numeric_value) * (-0.1)))
+            arg.append("{}".format(v))
+            arg.append("{}".format(abs(self._app.variable_manager[k].numeric_value) * 0.1))
+        if self.is_solved:
+            self._app.osolution.SetTuningOffsets(["TuningRanges:=", arg])
+            return True
+        else:
+            self._app.logger.error("Setup {} is not solved. Solve it before tuning variables.".format(self.name))
+            return False
+
     @pyaedt_function_handler(rangetype="range_type")
     def add_subrange(self, range_type, start, end=None, count=None, unit="GHz", clear=False):
         """Add a subrange to the sweep.
 
         Parameters
         ----------
         range_type : str
```

### Comparing `pyaedt-0.9.0/pyaedt/modules/SolveSweeps.py` & `pyaedt-0.9.1/pyaedt/modules/SolveSweeps.py`

 * *Files identical despite different names*

### Comparing `pyaedt-0.9.0/pyaedt/modules/monitor_icepak.py` & `pyaedt-0.9.1/pyaedt/modules/monitor_icepak.py`

 * *Files identical despite different names*

### Comparing `pyaedt-0.9.0/pyaedt/modules/report_templates.py` & `pyaedt-0.9.1/pyaedt/modules/report_templates.py`

 * *Files identical despite different names*

### Comparing `pyaedt-0.9.0/pyaedt/modules/solutions.py` & `pyaedt-0.9.1/pyaedt/modules/solutions.py`

 * *Files 1% similar despite different names*

```diff
@@ -20,15 +20,14 @@
 from pyaedt.generic.general_methods import conversion_function
 from pyaedt.generic.general_methods import open_file
 from pyaedt.generic.general_methods import write_csv
 from pyaedt.generic.plot import get_structured_mesh
 from pyaedt.generic.plot import is_notebook
 from pyaedt.generic.plot import plot_2d_chart
 from pyaedt.generic.plot import plot_3d_chart
-from pyaedt.generic.plot import plot_contour
 from pyaedt.generic.plot import plot_polar_chart
 from pyaedt.generic.settings import settings
 from pyaedt.modeler.cad.elements3d import FacePrimitive
 
 np = None
 pd = None
 pv = None
@@ -41,14 +40,18 @@
         import pandas as pd
     except ImportError:
         pd = None
     try:
         import pyvista as pv
     except ImportError:
         pv = None
+    try:
+        import matplotlib.pyplot as plt
+    except ImportError:
+        plt = None
 
 
 class SolutionData(object):
     """Contains information from the :func:`GetSolutionDataPerVariation` method."""
 
     def __init__(self, aedtdata):
         self._original_data = aedtdata
@@ -1084,26 +1087,29 @@
         for element in csv_list:
             textfile.write(element + "\n")
         textfile.close()
         return txt_file_name
 
 
 class FfdSolutionData(object):
-    """Contains information from the far field solution data.
+    """Provides antenna array far-field data.
 
-    Load far field data from the element pattern files.
+    Read embedded element patterns generated in HFSS and return the Python interface
+    to plot and analyze the array far-field data.
 
     Parameters
     ----------
     eep_files : list or str
-        List of element pattern files for each frequency.
-        If the input is string, it is assumed to be a single frequency.
+        List of embedded element pattern files for each frequency.
+        If data is only provided for a single frequency, then a string can be passed
+        instead of a one-element list.
     frequencies : list, str, int, or float
         List of frequencies.
-        If the input is not a list, it is assumed to be a single frequency.
+        If data is only available for a single frequency, then a float or integer may be passed
+        instead of a one-element list.
 
     Examples
     --------
 
     >>> import pyaedt
     >>> from pyaedt.modules.solutions import FfdSolutionData
     >>> app = pyaedt.Hfss(specified_version="2023.2", designname="Antenna")
@@ -1522,19 +1528,22 @@
                              theta_scan="theta",
                              export_image_path="image_path")
     def plot_farfield_contour(
             self,
             quantity="RealizedGain",
             phi=0,
             theta=0,
-            title="RectangularPlot",
+            size=None,
+            title=None,
             quantity_format="dB10",
             image_path=None,
             levels=64,
             show=True,
+            polar=True,
+            max_theta=180,
             **kwargs
     ):
         # fmt: on
         """Create a contour plot of a specified quantity.
 
         Parameters
         ----------
@@ -1542,46 +1551,55 @@
             Far field quantity to plot. The default is ``"RealizedGain"``.
             Available quantities are: ``"RealizedGain"``, ``"RealizedGain_Phi"``, ``"RealizedGain_Theta"``,
             ``"rEPhi"``, ``"rETheta"``, and ``"rETotal"``.
         phi : float, int, optional
             Phi scan angle in degrees. The default is ``0``.
         theta : float, int, optional
             Theta scan angle in degrees. The default is ``0``.
+        size : tuple, optional
+            Image size in pixel (width, height). The default is ``None``, in which case resolution
+            is determined automatically.
         title : str, optional
             Plot title. The default is ``"RectangularPlot"``.
         quantity_format : str, optional
             Conversion data function.
             Available functions are: ``"abs"``, ``"ang"``, ``"dB10"``, ``"dB20"``, ``"deg"``, ``"imag"``, ``"norm"``,
             and ``"real"``.
         image_path : str, optional
             Full path for the image file. The default is ``None``, in which case the file is not exported.
         levels : int, optional
             Color map levels. The default is ``64``.
         show : bool, optional
             Whether to show the plot. The default is ``True``. If ``False``, the Matplotlib
             instance of the plot is shown.
+        polar : bool, optional
+            Generate the plot in polar coordinates. The default is ``True``. If ``False``, the plot
+            generated is rectangular.
+        max_theta : float or int, optional
+            Maxmum theta angle for plotting. The default is ``180``, which plots the far-field data for
+            all angles. Setting ``max_theta`` to 90 limits the displayed data to the upper
+            hemisphere, that is (0 < theta < 90).
 
         Returns
         -------
-        :class:`matplotlib.plt`
-            Whether to show the plotted curve.
-            If ``show=True``, a Matplotlib figure instance of the plot is returned.
-            If ``show=False``, the plotted curve is returned.
+        :class:`matplotlib.pyplot.Figure`
 
         Examples
         --------
         >>> import pyaedt
-        >>> app = pyaedt.Hfss(specified_version="2023.2", designname="Antenna")
+        >>> app = pyaedt.Hfss(specified_version="2024.1", designname="Antenna")
         >>> setup_name = "Setup1 : LastAdaptive"
         >>> frequencies = [77e9]
         >>> sphere = "3D"
         >>> data = app.get_antenna_ffd_solution_data(frequencies,setup_name,sphere)
         >>> data.plot_farfield_contour()
 
         """
+        if not title:
+            title = quantity
         for k in kwargs:
             if k == "convert_to_db":  # pragma: no cover
                 self.logger.warning("`convert_to_db` is deprecated since v0.7.8. Use `quantity_format` instead.")
                 quantity_format = "dB10" if kwargs["convert_to_db"] else "abs"
             elif k == "qty_str":  # pragma: no cover
                 self.logger.warning("`qty_str` is deprecated since v0.7.8. Use `quantity` instead.")
                 quantity = kwargs["qty_str"]
@@ -1590,35 +1608,62 @@
                 self.logger.error(msg)
                 raise TypeError(msg)
 
         data = self.combine_farfield(phi, theta)
         if quantity not in data:  # pragma: no cover
             self.logger.error("Far field quantity is not available.")
             return False
+        select = np.abs(data["Theta"]) <= max_theta  # Limit theta range for plotting.
 
-        data_to_plot = data[quantity]
+        data_to_plot = data[quantity][select, :]
         data_to_plot = conversion_function(data_to_plot, quantity_format)
         if not isinstance(data_to_plot, np.ndarray):  # pragma: no cover
             self.logger.error("Wrong format quantity")
             return False
-        data_to_plot = np.reshape(data_to_plot, (data["nTheta"], data["nPhi"]))
-        th, ph = np.meshgrid(data["Theta"], data["Phi"])
-        if show:
-            return plot_contour(
-                x=th,
-                y=ph,
-                qty_to_plot=data_to_plot,
-                xlabel="Theta (degree)",
-                ylabel="Phi (degree)",
-                title=title,
-                levels=levels,
-                snapshot_path=image_path,
-            )
-        else:
-            return data_to_plot
+        ph, th = np.meshgrid(data["Phi"], data["Theta"][select])
+        ph = ph * np.pi/180 if polar else ph
+        # Convert to radians for polar plot.
+
+        # TODO: Is it necessary to set the plot size?
+
+        default_figsize = plt.rcParams["figure.figsize"]
+        if size:  # Retain this code to remain consistent with other plotting methods.
+            dpi = 100.0
+            figsize = (size[0] / dpi, size[1] / dpi)
+            plt.rcParams["figure.figsize"] = figsize
+        else:
+            figsize = default_figsize
+
+        projection = 'polar' if polar else 'rectilinear'
+        fig, ax = plt.subplots(subplot_kw={'projection': projection}, figsize=figsize)
+
+        fig.suptitle(title)
+        ax.set_xlabel("$\phi$ (Degrees)")
+        if polar:
+            ax.set_rticks(np.linspace(0, max_theta, 3))
+        else:
+            ax.set_ylabel("$\\theta (Degrees")
+
+        plt.contourf(
+            ph,
+            th,
+            data_to_plot,
+            levels=levels,
+            cmap="jet",
+        )
+        cbar = plt.colorbar()
+        cbar.set_label(quantity_format, rotation=270, labelpad=20)
+
+        if image_path:
+            plt.savefig(image_path)
+        if show:  # pragma: no cover
+            plt.show()
+
+        plt.rcParams["figure.figsize"] = default_figsize
+        return fig
 
     # fmt: off
     @pyaedt_function_handler(farfield_quantity="quantity",
                              phi_scan="phi",
                              theta_scan="theta",
                              export_image_path="image_path")
     def plot_2d_cut(
@@ -1861,15 +1906,15 @@
         phi = np.deg2rad(np.array(data["Phi"]))
         phi_grid, theta_grid = np.meshgrid(phi, theta)
         r = np.reshape(ff_data_renorm, (len(data["Theta"]), len(data["Phi"])))
 
         x = r * np.sin(theta_grid) * np.cos(phi_grid)
         y = r * np.sin(theta_grid) * np.sin(phi_grid)
         z = r * np.cos(theta_grid)
-        if show:
+        if show:  # pragma: no cover
             plot_3d_chart([x, y, z], xlabel="Theta", ylabel="Phi", title=title, snapshot_path=image_path)
         else:
             return x, y, z
 
     # fmt: off
     @pyaedt_function_handler(farfield_quantity="quantity", export_image_path="image_path")
     def polar_plot_3d_pyvista(
@@ -2416,15 +2461,27 @@
             x = math.atan2(-R[1, 2], R[1, 1])
             y = math.atan2(-R[2, 0], sy)
             z = 0
         return np.array([x, y, z])
 
 
 class FfdSolutionDataExporter(FfdSolutionData):
-    """Export far field solution data.
+    """Class to enable export of embedded element pattern data from HFSS.
+
+    An instance of this class is returned from the
+    :meth:`pyaedt.Hfss.get_antenna_ffd_solution_data` method. This method allows creation of
+    the embedded
+    element pattern (EEP) files for an antenna array that have been solved in HFSS. The
+    ``frequencies`` and ``eep_files`` properties can then be passed as arguments to
+    instantiate an instance of the :class:`pyaedt.modules.solutions.FfdSolutionData` class for
+    subsequent analysis and postprocessing of the array data.
+
+    Note that this class is derived from the :class:`FfdSolutionData` class and can be used directly for
+    far-field postprocessing and array analysis, but it remains a property of the
+    :class:`pyaedt.Hfss` application.
 
     Parameters
     ----------
     app : :class:`pyaedt.Hfss`
         HFSS application instance.
     sphere_name : str
         Infinite sphere to use.
```

### Comparing `pyaedt-0.9.0/pyaedt/q3d.py` & `pyaedt-0.9.1/pyaedt/q3d.py`

 * *Files identical despite different names*

### Comparing `pyaedt-0.9.0/pyaedt/rmxprt.py` & `pyaedt-0.9.1/pyaedt/rmxprt.py`

 * *Files identical despite different names*

### Comparing `pyaedt-0.9.0/pyaedt/rpc/rpyc_services.py` & `pyaedt-0.9.1/pyaedt/rpc/rpyc_services.py`

 * *Files identical despite different names*

### Comparing `pyaedt-0.9.0/pyaedt/sbrplus/hdm_parser.py` & `pyaedt-0.9.1/pyaedt/sbrplus/hdm_parser.py`

 * *Files identical despite different names*

### Comparing `pyaedt-0.9.0/pyaedt/sbrplus/hdm_utils.py` & `pyaedt-0.9.1/pyaedt/sbrplus/hdm_utils.py`

 * *Files identical despite different names*

### Comparing `pyaedt-0.9.0/pyaedt/sbrplus/matlab/HdmObject.m` & `pyaedt-0.9.1/pyaedt/sbrplus/matlab/HdmObject.m`

 * *Files identical despite different names*

### Comparing `pyaedt-0.9.0/pyaedt/sbrplus/matlab/SbrBounceType.m` & `pyaedt-0.9.1/pyaedt/sbrplus/matlab/SbrBounceType.m`

 * *Files identical despite different names*

### Comparing `pyaedt-0.9.0/pyaedt/sbrplus/matlab/StopWatch.m` & `pyaedt-0.9.1/pyaedt/sbrplus/matlab/StopWatch.m`

 * *Files identical despite different names*

### Comparing `pyaedt-0.9.0/pyaedt/sbrplus/matlab/add_3dlight.m` & `pyaedt-0.9.1/pyaedt/sbrplus/matlab/add_3dlight.m`

 * *Files identical despite different names*

### Comparing `pyaedt-0.9.0/pyaedt/sbrplus/matlab/draw_rays1.m` & `pyaedt-0.9.1/pyaedt/sbrplus/matlab/draw_rays1.m`

 * *Files identical despite different names*

### Comparing `pyaedt-0.9.0/pyaedt/sbrplus/matlab/draw_wfobj.m` & `pyaedt-0.9.1/pyaedt/sbrplus/matlab/draw_wfobj.m`

 * *Files identical despite different names*

### Comparing `pyaedt-0.9.0/pyaedt/sbrplus/matlab/filter_rays1.m` & `pyaedt-0.9.1/pyaedt/sbrplus/matlab/filter_rays1.m`

 * *Files identical despite different names*

### Comparing `pyaedt-0.9.0/pyaedt/sbrplus/matlab/filtered_tracks.m` & `pyaedt-0.9.1/pyaedt/sbrplus/matlab/filtered_tracks.m`

 * *Files identical despite different names*

### Comparing `pyaedt-0.9.0/pyaedt/sbrplus/matlab/ld_sbrplushdm.m` & `pyaedt-0.9.1/pyaedt/sbrplus/matlab/ld_sbrplushdm.m`

 * *Files identical despite different names*

### Comparing `pyaedt-0.9.0/pyaedt/sbrplus/matlab/ld_wfobj.m` & `pyaedt-0.9.1/pyaedt/sbrplus/matlab/ld_wfobj.m`

 * *Files identical despite different names*

### Comparing `pyaedt-0.9.0/pyaedt/sbrplus/matlab/validate_sfields.m` & `pyaedt-0.9.1/pyaedt/sbrplus/matlab/validate_sfields.m`

 * *Files identical despite different names*

### Comparing `pyaedt-0.9.0/pyaedt/sbrplus/plot.py` & `pyaedt-0.9.1/pyaedt/sbrplus/plot.py`

 * *Files identical despite different names*

### Comparing `pyaedt-0.9.0/pyaedt/twinbuilder.py` & `pyaedt-0.9.1/pyaedt/twinbuilder.py`

 * *Files identical despite different names*

### Comparing `pyaedt-0.9.0/pyaedt/workflows/__init__.py` & `pyaedt-0.9.1/pyaedt/workflows/__init__.py`

 * *Files identical despite different names*

### Comparing `pyaedt-0.9.0/pyaedt/workflows/circuit/__init__.py` & `pyaedt-0.9.1/pyaedt/workflows/circuit/__init__.py`

 * *Files identical despite different names*

### Comparing `pyaedt-0.9.0/pyaedt/workflows/customize_automation_tab.py` & `pyaedt-0.9.1/pyaedt/workflows/customize_automation_tab.py`

 * *Files 0% similar despite different names*

```diff
@@ -362,14 +362,15 @@
         file_name_dest = template_file.replace("_", " ")
         with open(os.path.join(tool_dir, file_name_dest + ".py"), "w") as out_file:
             build_file_data = build_file.read()
             build_file_data = build_file_data.replace("##TOOLKIT_REL_LIB_DIR##", toolkit_rel_lib_dir)
             build_file_data = build_file_data.replace("##IPYTHON_EXE##", ipython_executable)
             build_file_data = build_file_data.replace("##PYTHON_EXE##", executable_version_agnostic)
             build_file_data = build_file_data.replace("##JUPYTER_EXE##", jupyter_executable)
+            build_file_data = build_file_data.replace("##TOOLKIT_NAME##", name)
             if dest_script_path:
                 build_file_data = build_file_data.replace("##PYTHON_SCRIPT##", dest_script_path)
 
             if version_agnostic:
                 build_file_data = build_file_data.replace(" % version", "")
             out_file.write(build_file_data)
```

### Comparing `pyaedt-0.9.0/pyaedt/workflows/emit/__init__.py` & `pyaedt-0.9.1/pyaedt/workflows/emit/__init__.py`

 * *Files identical despite different names*

### Comparing `pyaedt-0.9.0/pyaedt/workflows/hfss/__init__.py` & `pyaedt-0.9.1/pyaedt/workflows/hfss/__init__.py`

 * *Files identical despite different names*

### Comparing `pyaedt-0.9.0/pyaedt/workflows/hfss/images/large/antenna.png` & `pyaedt-0.9.1/pyaedt/workflows/hfss/images/large/antenna.png`

 * *Files identical despite different names*

### Comparing `pyaedt-0.9.0/pyaedt/workflows/hfss3dlayout/__init__.py` & `pyaedt-0.9.1/pyaedt/workflows/hfss3dlayout/__init__.py`

 * *Files identical despite different names*

### Comparing `pyaedt-0.9.0/pyaedt/workflows/hfss3dlayout/export_to_3D.py` & `pyaedt-0.9.1/pyaedt/workflows/hfss3dlayout/export_to_3D.py`

 * *Files 1% similar despite different names*

```diff
@@ -61,15 +61,15 @@
 b.pack(pady=10)
 
 mainloop()
 
 suffixes = {"Export to HFSS": "HFSS", "Export to Q3D": "Q3D", "Export to Maxwell 3D": "M3D", "Export to Icepak": "IPK"}
 
 if "PYAEDT_SCRIPT_PORT" in os.environ and "PYAEDT_SCRIPT_VERSION" in os.environ:
-    port = os.environ["PYAEDT_SCRIPT_PORT"]
+    port = int(os.environ["PYAEDT_SCRIPT_PORT"])
     version = os.environ["PYAEDT_SCRIPT_VERSION"]
 else:
     port = 0
     version = "2024.1"
 
 with Desktop(new_desktop_session=False, close_on_exit=False, specified_version=version, port=port) as d:
     proj = d.active_project()
```

### Comparing `pyaedt-0.9.0/pyaedt/workflows/hfss3dlayout/images/large/cad3d.png` & `pyaedt-0.9.1/pyaedt/workflows/hfss3dlayout/images/large/cad3d.png`

 * *Files identical despite different names*

### Comparing `pyaedt-0.9.0/pyaedt/workflows/icepak/__init__.py` & `pyaedt-0.9.1/pyaedt/workflows/icepak/__init__.py`

 * *Files identical despite different names*

### Comparing `pyaedt-0.9.0/pyaedt/workflows/images/large/logo.png` & `pyaedt-0.9.1/pyaedt/workflows/images/large/logo.png`

 * *Files identical despite different names*

### Comparing `pyaedt-0.9.0/pyaedt/workflows/images/large/pyansys.png` & `pyaedt-0.9.1/pyaedt/workflows/images/large/pyansys.png`

 * *Files identical despite different names*

### Comparing `pyaedt-0.9.0/pyaedt/workflows/installer/__init__.py` & `pyaedt-0.9.1/pyaedt/workflows/installer/__init__.py`

 * *Files identical despite different names*

### Comparing `pyaedt-0.9.0/pyaedt/workflows/installer/console_setup.py` & `pyaedt-0.9.1/pyaedt/workflows/installer/console_setup.py`

 * *Files identical despite different names*

### Comparing `pyaedt-0.9.0/pyaedt/workflows/installer/create_report.py` & `pyaedt-0.9.1/pyaedt/workflows/installer/create_report.py`

 * *Files 2% similar despite different names*

```diff
@@ -4,15 +4,15 @@
 import os
 
 from pyaedt import Desktop
 from pyaedt import get_pyaedt_app
 from pyaedt.generic.pdf import AnsysReport
 
 if "PYAEDT_SCRIPT_PORT" in os.environ and "PYAEDT_SCRIPT_VERSION" in os.environ:
-    port = os.environ["PYAEDT_SCRIPT_PORT"]
+    port = int(os.environ["PYAEDT_SCRIPT_PORT"])
     version = os.environ["PYAEDT_SCRIPT_VERSION"]
 else:
     port = 0
     version = "2024.1"
 
 with Desktop(new_desktop_session=False, close_on_exit=False, specified_version=version, port=port) as d:
```

### Comparing `pyaedt-0.9.0/pyaedt/workflows/installer/images/large/console.png` & `pyaedt-0.9.1/pyaedt/workflows/installer/images/large/console.png`

 * *Files identical despite different names*

### Comparing `pyaedt-0.9.0/pyaedt/workflows/installer/images/large/jupyter.png` & `pyaedt-0.9.1/pyaedt/workflows/installer/images/large/jupyter.png`

 * *Files identical despite different names*

### Comparing `pyaedt-0.9.0/pyaedt/workflows/installer/images/large/run_script.png` & `pyaedt-0.9.1/pyaedt/workflows/installer/images/large/run_script.png`

 * *Files identical despite different names*

### Comparing `pyaedt-0.9.0/pyaedt/workflows/installer/images/large/toolkit_manager.png` & `pyaedt-0.9.1/pyaedt/workflows/installer/images/large/toolkit_manager.png`

 * *Files identical despite different names*

### Comparing `pyaedt-0.9.0/pyaedt/workflows/installer/jupyter_template.ipynb` & `pyaedt-0.9.1/pyaedt/workflows/installer/jupyter_template.ipynb`

 * *Files identical despite different names*

### Comparing `pyaedt-0.9.0/pyaedt/workflows/installer/pyaedt_installer.py` & `pyaedt-0.9.1/pyaedt/workflows/installer/pyaedt_installer.py`

 * *Files identical despite different names*

### Comparing `pyaedt-0.9.0/pyaedt/workflows/installer/toolkit_manager.py` & `pyaedt-0.9.1/pyaedt/workflows/installer/toolkit_manager.py`

 * *Files 0% similar despite different names*

```diff
@@ -30,14 +30,15 @@
 from pyaedt import Desktop
 from pyaedt import is_windows
 import pyaedt.workflows
 from pyaedt.workflows.customize_automation_tab import add_custom_toolkit
 from pyaedt.workflows.customize_automation_tab import add_script_to_menu
 from pyaedt.workflows.customize_automation_tab import available_toolkits
 from pyaedt.workflows.customize_automation_tab import remove_script_from_menu
+import pyaedt.workflows.templates
 
 env_vars = ["PYAEDT_SCRIPT_VERSION", "PYAEDT_SCRIPT_PORT", "PYAEDT_STUDENT_VERSION"]
 if all(var in os.environ for var in env_vars):
     version = os.environ["PYAEDT_SCRIPT_VERSION"]
     port = int(os.environ["PYAEDT_SCRIPT_PORT"])
     student_version = False if os.environ["PYAEDT_STUDENT_VERSION"] == "False" else True
 else:
@@ -274,15 +275,16 @@
             desktop.logger.info("Install {}".format(name))
             if is_windows:
                 pyaedt_venv_dir = os.path.join(os.environ["APPDATA"], "pyaedt_env_ide", "v{}".format(version))
                 executable_interpreter = os.path.join(pyaedt_venv_dir, "Scripts", "python.exe")
             else:
                 pyaedt_venv_dir = os.path.join(os.environ["HOME"], "pyaedt_env_ide", "v{}".format(version))
                 executable_interpreter = os.path.join(pyaedt_venv_dir, "bin", "python")
-
+            if not file:
+                file = os.path.join(os.path.dirname(pyaedt.workflows.templates.__file__), "toolkit_template.py")
             if os.path.isfile(executable_interpreter):
                 add_script_to_menu(
                     name=name,
                     script_file=file,
                     product=toolkit_level,
                     icon_file=icon,
                     executable_interpreter=executable_interpreter,
```

### Comparing `pyaedt-0.9.0/pyaedt/workflows/maxwell2d/__init__.py` & `pyaedt-0.9.1/pyaedt/workflows/maxwell2d/__init__.py`

 * *Files identical despite different names*

### Comparing `pyaedt-0.9.0/pyaedt/workflows/maxwell3d/__init__.py` & `pyaedt-0.9.1/pyaedt/workflows/maxwell3d/__init__.py`

 * *Files identical despite different names*

### Comparing `pyaedt-0.9.0/pyaedt/workflows/maxwell3d/images/large/magnet_segmentation.png` & `pyaedt-0.9.1/pyaedt/workflows/maxwell3d/images/large/magnet_segmentation.png`

 * *Files identical despite different names*

### Comparing `pyaedt-0.9.0/pyaedt/workflows/mechanical/__init__.py` & `pyaedt-0.9.1/pyaedt/workflows/mechanical/__init__.py`

 * *Files identical despite different names*

### Comparing `pyaedt-0.9.0/pyaedt/workflows/project/__init__.py` & `pyaedt-0.9.1/pyaedt/workflows/project/__init__.py`

 * *Files identical despite different names*

### Comparing `pyaedt-0.9.0/pyaedt/workflows/project/create_report.py` & `pyaedt-0.9.1/pyaedt/workflows/project/create_report.py`

 * *Files 8% similar despite different names*

```diff
@@ -4,15 +4,15 @@
 import os
 
 from pyaedt import Desktop
 from pyaedt import get_pyaedt_app
 from pyaedt.generic.pdf import AnsysReport
 
 if "PYAEDT_SCRIPT_PORT" in os.environ and "PYAEDT_SCRIPT_VERSION" in os.environ:
-    port = os.environ["PYAEDT_SCRIPT_PORT"]
+    port = int(os.environ["PYAEDT_SCRIPT_PORT"])
     version = os.environ["PYAEDT_SCRIPT_VERSION"]
 else:
     port = 0
     version = "2024.1"
 
 with Desktop(new_desktop_session=False, close_on_exit=False, specified_version=version, port=port) as d:
```

### Comparing `pyaedt-0.9.0/pyaedt/workflows/project/images/large/cad3d.png` & `pyaedt-0.9.1/pyaedt/workflows/project/images/large/cad3d.png`

 * *Files identical despite different names*

### Comparing `pyaedt-0.9.0/pyaedt/workflows/project/images/large/pdf.png` & `pyaedt-0.9.1/pyaedt/workflows/project/images/large/pdf.png`

 * *Files identical despite different names*

### Comparing `pyaedt-0.9.0/pyaedt/workflows/project/import_nastran.py` & `pyaedt-0.9.1/pyaedt/workflows/project/import_nastran.py`

 * *Files 1% similar despite different names*

```diff
@@ -16,19 +16,19 @@
 
     # Change label contents
     return filename
 
 
 nas_input = browseFiles()
 if "PYAEDT_SCRIPT_PORT" in os.environ and "PYAEDT_SCRIPT_VERSION" in os.environ:
-    port = os.environ["PYAEDT_SCRIPT_PORT"]
+    port = int(os.environ["PYAEDT_SCRIPT_PORT"])
     version = os.environ["PYAEDT_SCRIPT_VERSION"]
 else:
     port = 0
-    version = "2024.2"
+    version = "2024.1"
 if os.path.exists(nas_input):
     with Desktop(new_desktop_session=False, close_on_exit=False, specified_version=version, port=port) as d:
         proj = d.active_project()
         des = d.active_design()
         projname = proj.GetName()
         desname = des.GetName()
         app = get_pyaedt_app(projname, desname)
```

### Comparing `pyaedt-0.9.0/pyaedt/workflows/q2d/__init__.py` & `pyaedt-0.9.1/pyaedt/workflows/q2d/__init__.py`

 * *Files identical despite different names*

### Comparing `pyaedt-0.9.0/pyaedt/workflows/q3d/__init__.py` & `pyaedt-0.9.1/pyaedt/workflows/q3d/__init__.py`

 * *Files identical despite different names*

### Comparing `pyaedt-0.9.0/pyaedt/workflows/simplorer/__init__.py` & `pyaedt-0.9.1/pyaedt/workflows/simplorer/__init__.py`

 * *Files identical despite different names*

### Comparing `pyaedt-0.9.0/pyaedt/workflows/templates/Jupyter.py_build` & `pyaedt-0.9.1/pyaedt/workflows/templates/Jupyter.py_build`

 * *Files identical despite different names*

### Comparing `pyaedt-0.9.0/pyaedt/workflows/templates/PyAEDT_Console.py_build` & `pyaedt-0.9.1/pyaedt/workflows/templates/PyAEDT_Console.py_build`

 * *Files identical despite different names*

### Comparing `pyaedt-0.9.0/pyaedt/workflows/templates/Run_PyAEDT_Script.py_build` & `pyaedt-0.9.1/pyaedt/workflows/templates/Run_PyAEDT_Script.py_build`

 * *Files identical despite different names*

### Comparing `pyaedt-0.9.0/pyaedt/workflows/templates/Run_PyAEDT_Toolkit_Script.py_build` & `pyaedt-0.9.1/pyaedt/workflows/templates/Run_Toolkit_Manager.py_build`

 * *Files 13% similar despite different names*

```diff
@@ -14,78 +14,85 @@
 """
 import os
 import sys
 
 from System.Windows.Forms import MessageBox
 from System.Windows.Forms import MessageBoxButtons
 from System.Windows.Forms import MessageBoxIcon
+from System.Windows.Forms import OpenFileDialog
 
 is_linux = os.name == "posix"
 script_name = os.path.splitext(os.path.basename(__file__))[0]
 
 if is_linux:
     import subprocessdotnet as subprocess
 else:
     import subprocess
 
 
 def main():
     try:
-        oDesktop.AddMessage("", "", 0, "Toolkit launched. Please wait.")
-        # launch file
-        python_exe = r"##PYTHON_EXE##"
-        pyaedt_script = r"##PYTHON_SCRIPT##"
+        version = oDesktop.GetVersion()[2:6].replace(".", "")
+        # launch toolkit manager
+        python_exe = r"##PYTHON_EXE##" % version
+        current_dir = os.path.dirname(os.path.abspath(os.path.realpath(__file__)))
+        pyaedt_toolkit_dir = os.path.normpath(os.path.join(current_dir, r"##TOOLKIT_REL_LIB_DIR##"))
+        pyaedt_script = os.path.join(pyaedt_toolkit_dir, "toolkit_manager.py")
         check_file(python_exe)
         check_file(pyaedt_script)
         os.environ["PYAEDT_SCRIPT_PROCESS_ID"] = str(oDesktop.GetProcessID())
-        version = str(oDesktop.GetVersion()[:6])
         os.environ["PYAEDT_SCRIPT_VERSION"] = version
+        if "Ansys Student" in str(oDesktop.GetExeDir()):
+            os.environ["PYAEDT_STUDENT_VERSION"] = "True"
+        else:
+            os.environ["PYAEDT_STUDENT_VERSION"] = "False"
         if version > "2022.2":
             os.environ["PYAEDT_SCRIPT_PORT"] = str(oDesktop.GetGrpcServerPort())
         if is_linux:
+
             edt_root = os.path.normpath(oDesktop.GetExeDir())
             os.environ["ANSYSEM_ROOT{}".format(version)] = edt_root
             ld_library_path_dirs_to_add = [
                 "{}/commonfiles/CPython/3_7/linx64/Release/python/lib".format(edt_root),
                 "{}/commonfiles/CPython/3_10/linx64/Release/python/lib".format(edt_root),
                 "{}/common/mono/Linux64/lib64".format(edt_root),
                 "{}/Delcross".format(edt_root),
                 "{}".format(edt_root),
             ]
             os.environ["LD_LIBRARY_PATH"] = ":".join(ld_library_path_dirs_to_add) + ":" + os.getenv(
                 "LD_LIBRARY_PATH", "")
             command = [
                 python_exe,
                 pyaedt_script,
-                str(oDesktop.GetProcessID()),
-                str(oDesktop.GetVersion()[:6]),
             ]
             my_env = os.environ.copy()
-            subprocess.Popen(command, env=my_env)
+            subprocess.Popen(command, env=my_env, stdout=subprocess.PIPE, stderr=subprocess.PIPE, stdin=subprocess.PIPE)
         else:
-            CREATE_NO_WINDOW = 0x08000000
             command = [
                 '"{}"'.format(python_exe),
                 '"{}"'.format(pyaedt_script),
-                str(oDesktop.GetProcessID()),
-                str(oDesktop.GetVersion()[:6]),
             ]
             my_env = os.environ.copy()
-            subprocess.Popen(" ".join(command), env=my_env, creationflags=CREATE_NO_WINDOW)
+            subprocess.Popen(" ".join(command), env=my_env, stdout=subprocess.PIPE, stderr=subprocess.PIPE, stdin=subprocess.PIPE, shell=True)
     except Exception as e:
         show_error(str(e))
 
 
 def check_file(file_path):
     if not os.path.isfile(file_path):
-        show_error('"{}" does not exist.'.format(
+        show_error('"{}" does not exist. Click the "Install PyAEDT" button in the Automation ribbon.'.format(
             file_path))
 
 
 def show_error(msg):
     oDesktop.AddMessage("", "", 2, str(msg))
     MessageBox.Show(str(msg), "Error", MessageBoxButtons.OK, MessageBoxIcon.Error)
     sys.exit()
 
 
+def debug(msg):
+    print("[debug] {}: {}".format(script_name, str(msg)))
+    LogDebug("{}: {}\n".format(script_name, str(msg)))
+
+
 if __name__ == "__main__":
     main()
```

### Comparing `pyaedt-0.9.0/pyaedt/workflows/templates/Run_Toolkit_Manager.py_build` & `pyaedt-0.9.1/pyaedt/workflows/templates/Run_PyAEDT_Toolkit_Script.py_build`

 * *Files 20% similar despite different names*

```diff
@@ -14,85 +14,83 @@
 """
 import os
 import sys
 
 from System.Windows.Forms import MessageBox
 from System.Windows.Forms import MessageBoxButtons
 from System.Windows.Forms import MessageBoxIcon
-from System.Windows.Forms import OpenFileDialog
 
 is_linux = os.name == "posix"
 script_name = os.path.splitext(os.path.basename(__file__))[0]
 
 if is_linux:
     import subprocessdotnet as subprocess
-else:
-    import subprocess
-
 
 def main():
     try:
-        version = oDesktop.GetVersion()[2:6].replace(".", "")
-        # launch toolkit manager
-        python_exe = r"##PYTHON_EXE##" % version
-        current_dir = os.path.dirname(os.path.abspath(os.path.realpath(__file__)))
-        pyaedt_toolkit_dir = os.path.normpath(os.path.join(current_dir, r"##TOOLKIT_REL_LIB_DIR##"))
-        pyaedt_script = os.path.join(pyaedt_toolkit_dir, "toolkit_manager.py")
+        oDesktop.AddMessage("", "", 0, "Toolkit launched. Please wait.")
+        # launch file
+        python_exe = r"##PYTHON_EXE##"
+        pyaedt_script = r"##PYTHON_SCRIPT##"
         check_file(python_exe)
         check_file(pyaedt_script)
         os.environ["PYAEDT_SCRIPT_PROCESS_ID"] = str(oDesktop.GetProcessID())
+        version = str(oDesktop.GetVersion()[:6])
         os.environ["PYAEDT_SCRIPT_VERSION"] = version
-        if "Ansys Student" in str(oDesktop.GetExeDir()):
-            os.environ["PYAEDT_STUDENT_VERSION"] = "True"
-        else:
-            os.environ["PYAEDT_STUDENT_VERSION"] = "False"
         if version > "2022.2":
             os.environ["PYAEDT_SCRIPT_PORT"] = str(oDesktop.GetGrpcServerPort())
-        if is_linux:
 
+        if is_linux:
             edt_root = os.path.normpath(oDesktop.GetExeDir())
             os.environ["ANSYSEM_ROOT{}".format(version)] = edt_root
             ld_library_path_dirs_to_add = [
                 "{}/commonfiles/CPython/3_7/linx64/Release/python/lib".format(edt_root),
                 "{}/commonfiles/CPython/3_10/linx64/Release/python/lib".format(edt_root),
                 "{}/common/mono/Linux64/lib64".format(edt_root),
                 "{}/Delcross".format(edt_root),
                 "{}".format(edt_root),
             ]
             os.environ["LD_LIBRARY_PATH"] = ":".join(ld_library_path_dirs_to_add) + ":" + os.getenv(
                 "LD_LIBRARY_PATH", "")
-            command = [
-                python_exe,
-                pyaedt_script,
-            ]
-            my_env = os.environ.copy()
-            subprocess.Popen(command, env=my_env, stdout=subprocess.PIPE, stderr=subprocess.PIPE, stdin=subprocess.PIPE)
+
+            if version > "2023.1":
+                os.environ["TCL_LIBRARY"] = os.path.join("{}/commonfiles/CPython/3_10/linx64/Release/python/lib".format(edt_root), "tcl8.5")
+                os.environ["TK_LIBRARY"] = os.path.join("{}/commonfiles/CPython/3_10/linx64/Release/python/lib".format(edt_root), "tk8.5")
+                os.environ["TKPATH"] = os.path.join("{}/commonfiles/CPython/3_10/linx64/Release/python/lib".format(edt_root), "tk8.5")
+            else:
+                os.environ["TCL_LIBRARY"] = os.path.join("{}/commonfiles/CPython/3_7/linx64/Release/python/lib".format(edt_root), "tcl8.5")
+                os.environ["TK_LIBRARY"] = os.path.join("{}/commonfiles/CPython/3_7/linx64/Release/python/lib".format(edt_root), "tk8.5")
+                os.environ["TKPATH"] = os.path.join("{}/commonfiles/CPython/3_7/linx64/Release/python/lib".format(edt_root), "tk8.5")
+
+            my_env = dict(os.environ.copy())
+            command = [python_exe, pyaedt_script]
+            subprocess.Popen(command, env=my_env)
         else:
-            command = [
-                '"{}"'.format(python_exe),
-                '"{}"'.format(pyaedt_script),
-            ]
-            my_env = os.environ.copy()
-            subprocess.Popen(" ".join(command), env=my_env, stdout=subprocess.PIPE, stderr=subprocess.PIPE, stdin=subprocess.PIPE, shell=True)
+            toolkit_name = r"##TOOLKIT_NAME##"
+            runme = "run_pyaedt_toolkit_{0}.cmd".format(toolkit_name)
+            edt_temp = oDesktop.GetTempDirectory()
+            cmd = '"{0}"'.format(pyaedt_script)
+            target = os.path.join(edt_temp, runme)
+            my_env = dict(os.environ.copy())
+            with open(target, 'w') as cmdfile:
+                for env in my_env:
+                    cmdfile.write('SET {0}={1}\n'.format(env, my_env[env]))
+                cmdfile.write('"{0}" {1}\n'.format(python_exe, cmd))
+            oDesktop.RunProgram(runme, edt_temp, edt_temp, "")
     except Exception as e:
         show_error(str(e))
 
 
 def check_file(file_path):
     if not os.path.isfile(file_path):
-        show_error('"{}" does not exist. Click the "Install PyAEDT" button in the Automation ribbon.'.format(
+        show_error('"{}" does not exist.'.format(
             file_path))
 
 
 def show_error(msg):
     oDesktop.AddMessage("", "", 2, str(msg))
     MessageBox.Show(str(msg), "Error", MessageBoxButtons.OK, MessageBoxIcon.Error)
     sys.exit()
 
 
-def debug(msg):
-    print("[debug] {}: {}".format(script_name, str(msg)))
-    LogDebug("{}: {}\n".format(script_name, str(msg)))
-
-
 if __name__ == "__main__":
     main()
```

### Comparing `pyaedt-0.9.0/pyaedt/workflows/templates/__init__.py` & `pyaedt-0.9.1/pyaedt/workflows/templates/__init__.py`

 * *Files identical despite different names*

### Comparing `pyaedt-0.9.0/pyproject.toml` & `pyaedt-0.9.1/pyproject.toml`

 * *Files 4% similar despite different names*

```diff
@@ -25,16 +25,15 @@
     "Programming Language :: Python :: 3.11",
 ]
 
 dependencies = [
     "fpdf2",
     "jsonschema",
     "psutil",
-    "pyedb>=0.4.0,<0.10; python_version == '3.7'",
-    "pyedb>=0.5.0; python_version > '3.7'",
+    "pyedb>=0.4.0",
     "pytomlpp; python_version < '3.12'",
     "rpyc>=6.0.0,<6.1",
 ]
 
 [project.optional-dependencies]
 tests = [
     "imageio>=2.30.0,<2.35",
@@ -45,16 +44,14 @@
     "numpy>=1.20.0,<2",
     "openpyxl>=3.1.0,<3.3",
     "osmnx>=1.1.0,<1.10",
     "pandas>=1.1.0,<2.3",
     "pytest>=7.4.0,<8.3",
     "pytest-cov>=4.0.0,<5.1",
     "pytest-xdist>=3.5.0,<3.7",
-    "pyedb>=0.4.0,<0.10; python_version == '3.7'",
-    "pyedb>=0.5.0,<0.11; python_version > '3.7'",
     "pyvista>=0.38.0,<0.44",
     "scikit-learn>=1.0.0,<1.5",
     "scikit-rf>=0.30.0,<1.1",
     "SRTM.py",
     "utm",
     "vtk==9.2.6",
 ]
```

### Comparing `pyaedt-0.9.0/PKG-INFO` & `pyaedt-0.9.1/PKG-INFO`

 * *Files 2% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: pyaedt
-Version: 0.9.0
+Version: 0.9.1
 Summary: Higher-Level Pythonic Ansys Electronics Desktop Framework
 Author-email: "ANSYS, Inc." <pyansys.core@ansys.com>
 Maintainer-email: PyAEDT developers <massimo.capodiferro@ansys.com>
 Requires-Python: >=3.7,<4
 Description-Content-Type: text/markdown
 Classifier: Development Status :: 4 - Beta
 Classifier: Intended Audience :: Science/Research
@@ -15,16 +15,15 @@
 Classifier: Programming Language :: Python :: 3.8
 Classifier: Programming Language :: Python :: 3.9
 Classifier: Programming Language :: Python :: 3.10
 Classifier: Programming Language :: Python :: 3.11
 Requires-Dist: fpdf2
 Requires-Dist: jsonschema
 Requires-Dist: psutil
-Requires-Dist: pyedb>=0.4.0,<0.10; python_version == '3.7'
-Requires-Dist: pyedb>=0.5.0; python_version > '3.7'
+Requires-Dist: pyedb>=0.4.0
 Requires-Dist: pytomlpp; python_version < '3.12'
 Requires-Dist: rpyc>=6.0.0,<6.1
 Requires-Dist: imageio>=2.30.0,<2.35 ; extra == "all"
 Requires-Dist: matplotlib>=3.5.0,<3.9 ; extra == "all"
 Requires-Dist: numpy>=1.20.0,<2 ; extra == "all"
 Requires-Dist: openpyxl>=3.1.0,<3.3 ; extra == "all"
 Requires-Dist: osmnx>=1.1.0,<1.10 ; extra == "all"
@@ -85,16 +84,14 @@
 Requires-Dist: numpy>=1.20.0,<2 ; extra == "tests"
 Requires-Dist: openpyxl>=3.1.0,<3.3 ; extra == "tests"
 Requires-Dist: osmnx>=1.1.0,<1.10 ; extra == "tests"
 Requires-Dist: pandas>=1.1.0,<2.3 ; extra == "tests"
 Requires-Dist: pytest>=7.4.0,<8.3 ; extra == "tests"
 Requires-Dist: pytest-cov>=4.0.0,<5.1 ; extra == "tests"
 Requires-Dist: pytest-xdist>=3.5.0,<3.7 ; extra == "tests"
-Requires-Dist: pyedb>=0.4.0,<0.10 ; extra == "tests" and ( python_version == '3.7')
-Requires-Dist: pyedb>=0.5.0,<0.11 ; extra == "tests" and ( python_version > '3.7')
 Requires-Dist: pyvista>=0.38.0,<0.44 ; extra == "tests"
 Requires-Dist: scikit-learn>=1.0.0,<1.5 ; extra == "tests"
 Requires-Dist: scikit-rf>=0.30.0,<1.1 ; extra == "tests"
 Requires-Dist: SRTM.py ; extra == "tests"
 Requires-Dist: utm ; extra == "tests"
 Requires-Dist: vtk==9.2.6 ; extra == "tests"
 Project-URL: Bugs, https://github.com/ansys/pyaedt/issues
```

