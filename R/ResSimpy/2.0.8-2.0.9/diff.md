# Comparing `tmp/ressimpy-2.0.8.tar.gz` & `tmp/ressimpy-2.0.9.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "ressimpy-2.0.8.tar", max compression
+gzip compressed data, was "ressimpy-2.0.9.tar", max compression
```

## Comparing `ressimpy-2.0.8.tar` & `ressimpy-2.0.9.tar`

### file list

```diff
@@ -1,190 +1,190 @@
--rw-r--r--   0        0        0     9156 2024-02-27 16:37:15.261211 ressimpy-2.0.8/LICENSE.MD
--rw-r--r--   0        0        0     5660 2024-02-27 16:37:15.261211 ressimpy-2.0.8/README.md
--rw-r--r--   0        0        0      504 2024-02-27 16:37:15.261211 ressimpy-2.0.8/ResSimpy/Aquifer.py
--rw-r--r--   0        0        0     8573 2024-02-27 16:37:15.261211 ressimpy-2.0.8/ResSimpy/Completion.py
--rw-r--r--   0        0        0     1557 2024-02-27 16:37:15.261211 ressimpy-2.0.8/ResSimpy/Constraint.py
--rw-r--r--   0        0        0     1908 2024-02-27 16:37:15.261211 ressimpy-2.0.8/ResSimpy/Constraints.py
--rw-r--r--   0        0        0     3926 2024-02-27 16:37:15.261211 ressimpy-2.0.8/ResSimpy/DataObjectMixin.py
--rw-r--r--   0        0        0     4109 2024-02-27 16:37:15.261211 ressimpy-2.0.8/ResSimpy/DynamicProperty.py
--rw-r--r--   0        0        0      313 2024-02-27 16:37:15.261211 ressimpy-2.0.8/ResSimpy/Enums/ConstraintEnums.py
--rw-r--r--   0        0        0      369 2024-02-27 16:37:15.261211 ressimpy-2.0.8/ResSimpy/Enums/FrequencyEnum.py
--rw-r--r--   0        0        0      168 2024-02-27 16:37:15.261211 ressimpy-2.0.8/ResSimpy/Enums/HowEnum.py
--rw-r--r--   0        0        0      214 2024-02-27 16:37:15.261211 ressimpy-2.0.8/ResSimpy/Enums/OutputType.py
--rw-r--r--   0        0        0      282 2024-02-27 16:37:15.261211 ressimpy-2.0.8/ResSimpy/Enums/PenetrationDirectionEnum.py
--rw-r--r--   0        0        0      253 2024-02-27 16:37:15.261211 ressimpy-2.0.8/ResSimpy/Enums/TimeSteppingMethodEnum.py
--rw-r--r--   0        0        0      507 2024-02-27 16:37:15.261211 ressimpy-2.0.8/ResSimpy/Enums/UnitsEnum.py
--rw-r--r--   0        0        0      377 2024-02-27 16:37:15.261211 ressimpy-2.0.8/ResSimpy/Enums/WellTypeEnum.py
--rw-r--r--   0        0        0       62 2024-02-27 16:37:15.261211 ressimpy-2.0.8/ResSimpy/Enums/__init__.py
--rw-r--r--   0        0        0      506 2024-02-27 16:37:15.261211 ressimpy-2.0.8/ResSimpy/Equilibration.py
--rw-r--r--   0        0        0     8911 2024-02-27 16:37:15.261211 ressimpy-2.0.8/ResSimpy/File.py
--rw-r--r--   0        0        0     2257 2024-02-27 16:37:15.261211 ressimpy-2.0.8/ResSimpy/FileBase.py
--rw-r--r--   0        0        0        0 2024-02-27 16:37:15.261211 ressimpy-2.0.8/ResSimpy/FileOperations/__init__.py
--rw-r--r--   0        0        0    22606 2024-02-27 16:37:15.261211 ressimpy-2.0.8/ResSimpy/FileOperations/file_operations.py
--rw-r--r--   0        0        0      413 2024-02-27 16:37:15.261211 ressimpy-2.0.8/ResSimpy/Gaslift.py
--rw-r--r--   0        0        0     2631 2024-02-27 16:37:15.261211 ressimpy-2.0.8/ResSimpy/Grid.py
--rw-r--r--   0        0        0      393 2024-02-27 16:37:15.261211 ressimpy-2.0.8/ResSimpy/Grids.py
--rw-r--r--   0        0        0      470 2024-02-27 16:37:15.261211 ressimpy-2.0.8/ResSimpy/Hydraulics.py
--rw-r--r--   0        0        0     3147 2024-02-27 16:37:15.261211 ressimpy-2.0.8/ResSimpy/ISODateTime.py
--rw-r--r--   0        0        0      588 2024-02-27 16:37:15.261211 ressimpy-2.0.8/ResSimpy/Network.py
--rw-r--r--   0        0        0      545 2024-02-27 16:37:15.261211 ressimpy-2.0.8/ResSimpy/Nexus/DataModels/FcsConfig.py
--rw-r--r--   0        0        0    23652 2024-02-27 16:37:15.261211 ressimpy-2.0.8/ResSimpy/Nexus/DataModels/FcsFile.py
--rw-r--r--   0        0        0    21550 2024-02-27 16:37:15.261211 ressimpy-2.0.8/ResSimpy/Nexus/DataModels/Network/NexusConstraint.py
--rw-r--r--   0        0        0    17761 2024-02-27 16:37:15.261211 ressimpy-2.0.8/ResSimpy/Nexus/DataModels/Network/NexusConstraints.py
--rw-r--r--   0        0        0     1718 2024-02-27 16:37:15.261211 ressimpy-2.0.8/ResSimpy/Nexus/DataModels/Network/NexusNode.py
--rw-r--r--   0        0        0     4917 2024-02-27 16:37:15.261211 ressimpy-2.0.8/ResSimpy/Nexus/DataModels/Network/NexusNodeConnection.py
--rw-r--r--   0        0        0     6436 2024-02-27 16:37:15.261211 ressimpy-2.0.8/ResSimpy/Nexus/DataModels/Network/NexusNodeConnections.py
--rw-r--r--   0        0        0     6543 2024-02-27 16:37:15.261211 ressimpy-2.0.8/ResSimpy/Nexus/DataModels/Network/NexusNodes.py
--rw-r--r--   0        0        0     4071 2024-02-27 16:37:15.261211 ressimpy-2.0.8/ResSimpy/Nexus/DataModels/Network/NexusProc.py
--rw-r--r--   0        0        0     1124 2024-02-27 16:37:15.261211 ressimpy-2.0.8/ResSimpy/Nexus/DataModels/Network/NexusProcs.py
--rw-r--r--   0        0        0     2084 2024-02-27 16:37:15.261211 ressimpy-2.0.8/ResSimpy/Nexus/DataModels/Network/NexusTarget.py
--rw-r--r--   0        0        0     6763 2024-02-27 16:37:15.261211 ressimpy-2.0.8/ResSimpy/Nexus/DataModels/Network/NexusTargets.py
--rw-r--r--   0        0        0     6510 2024-02-27 16:37:15.261211 ressimpy-2.0.8/ResSimpy/Nexus/DataModels/Network/NexusWellConnection.py
--rw-r--r--   0        0        0     6647 2024-02-27 16:37:15.261211 ressimpy-2.0.8/ResSimpy/Nexus/DataModels/Network/NexusWellConnections.py
--rw-r--r--   0        0        0     2191 2024-02-27 16:37:15.261211 ressimpy-2.0.8/ResSimpy/Nexus/DataModels/Network/NexusWellLists.py
--rw-r--r--   0        0        0     2780 2024-02-27 16:37:15.261211 ressimpy-2.0.8/ResSimpy/Nexus/DataModels/Network/NexusWellbore.py
--rw-r--r--   0        0        0     5892 2024-02-27 16:37:15.261211 ressimpy-2.0.8/ResSimpy/Nexus/DataModels/Network/NexusWellbores.py
--rw-r--r--   0        0        0     4535 2024-02-27 16:37:15.261211 ressimpy-2.0.8/ResSimpy/Nexus/DataModels/Network/NexusWellhead.py
--rw-r--r--   0        0        0     5815 2024-02-27 16:37:15.261211 ressimpy-2.0.8/ResSimpy/Nexus/DataModels/Network/NexusWellheads.py
--rw-r--r--   0        0        0      329 2024-02-27 16:37:15.261211 ressimpy-2.0.8/ResSimpy/Nexus/DataModels/Network/__init__.py
--rw-r--r--   0        0        0     8313 2024-02-27 16:37:15.261211 ressimpy-2.0.8/ResSimpy/Nexus/DataModels/NexusAquiferMethod.py
--rw-r--r--   0        0        0    14155 2024-02-27 16:37:15.261211 ressimpy-2.0.8/ResSimpy/Nexus/DataModels/NexusCompletion.py
--rw-r--r--   0        0        0    10788 2024-02-27 16:37:15.261211 ressimpy-2.0.8/ResSimpy/Nexus/DataModels/NexusEquilMethod.py
--rw-r--r--   0        0        0    32379 2024-02-27 16:37:15.261211 ressimpy-2.0.8/ResSimpy/Nexus/DataModels/NexusFile.py
--rw-r--r--   0        0        0     6211 2024-02-27 16:37:15.261211 ressimpy-2.0.8/ResSimpy/Nexus/DataModels/NexusGasliftMethod.py
--rw-r--r--   0        0        0    13247 2024-02-27 16:37:15.261211 ressimpy-2.0.8/ResSimpy/Nexus/DataModels/NexusHydraulicsMethod.py
--rw-r--r--   0        0        0    30593 2024-02-27 16:37:15.261211 ressimpy-2.0.8/ResSimpy/Nexus/DataModels/NexusPVTMethod.py
--rw-r--r--   0        0        0     2718 2024-02-27 16:37:15.261211 ressimpy-2.0.8/ResSimpy/Nexus/DataModels/NexusRelPermEndPoint.py
--rw-r--r--   0        0        0    19602 2024-02-27 16:37:15.265210 ressimpy-2.0.8/ResSimpy/Nexus/DataModels/NexusRelPermMethod.py
--rw-r--r--   0        0        0     9467 2024-02-27 16:37:15.265210 ressimpy-2.0.8/ResSimpy/Nexus/DataModels/NexusRockMethod.py
--rw-r--r--   0        0        0     8848 2024-02-27 16:37:15.265210 ressimpy-2.0.8/ResSimpy/Nexus/DataModels/NexusSeparatorMethod.py
--rw-r--r--   0        0        0    15015 2024-02-27 16:37:15.265210 ressimpy-2.0.8/ResSimpy/Nexus/DataModels/NexusSolverParameter.py
--rw-r--r--   0        0        0     6112 2024-02-27 16:37:15.265210 ressimpy-2.0.8/ResSimpy/Nexus/DataModels/NexusValveMethod.py
--rw-r--r--   0        0        0    11098 2024-02-27 16:37:15.265210 ressimpy-2.0.8/ResSimpy/Nexus/DataModels/NexusWaterMethod.py
--rw-r--r--   0        0        0     8247 2024-02-27 16:37:15.265210 ressimpy-2.0.8/ResSimpy/Nexus/DataModels/NexusWell.py
--rw-r--r--   0        0        0      781 2024-02-27 16:37:15.265210 ressimpy-2.0.8/ResSimpy/Nexus/DataModels/NexusWellList.py
--rw-r--r--   0        0        0     2858 2024-02-27 16:37:15.265210 ressimpy-2.0.8/ResSimpy/Nexus/DataModels/NexusWellMod.py
--rw-r--r--   0        0        0    14838 2024-02-27 16:37:15.265210 ressimpy-2.0.8/ResSimpy/Nexus/DataModels/StructuredGrid/NexusGrid.py
--rw-r--r--   0        0        0       67 2024-02-27 16:37:15.265210 ressimpy-2.0.8/ResSimpy/Nexus/DataModels/StructuredGrid/__init__.py
--rw-r--r--   0        0        0       77 2024-02-27 16:37:15.265210 ressimpy-2.0.8/ResSimpy/Nexus/DataModels/__init__.py
--rw-r--r--   0        0        0     3396 2024-02-27 16:37:15.265210 ressimpy-2.0.8/ResSimpy/Nexus/NexusAquiferMethods.py
--rw-r--r--   0        0        0      273 2024-02-27 16:37:15.265210 ressimpy-2.0.8/ResSimpy/Nexus/NexusEnums/DateFormatEnum.py
--rw-r--r--   0        0        0      106 2024-02-27 16:37:15.265210 ressimpy-2.0.8/ResSimpy/Nexus/NexusEnums/__init__.py
--rw-r--r--   0        0        0     3374 2024-02-27 16:37:15.265210 ressimpy-2.0.8/ResSimpy/Nexus/NexusEquilMethods.py
--rw-r--r--   0        0        0     3345 2024-02-27 16:37:15.265210 ressimpy-2.0.8/ResSimpy/Nexus/NexusGasliftMethods.py
--rw-r--r--   0        0        0       43 2024-02-27 16:37:15.265210 ressimpy-2.0.8/ResSimpy/Nexus/NexusGrids.py
--rw-r--r--   0        0        0     3418 2024-02-27 16:37:15.265210 ressimpy-2.0.8/ResSimpy/Nexus/NexusHydraulicsMethods.py
--rw-r--r--   0        0        0       47 2024-02-27 16:37:15.265210 ressimpy-2.0.8/ResSimpy/Nexus/NexusKeywords/__init__.py
--rw-r--r--   0        0        0        0 2024-02-27 16:37:15.265210 ressimpy-2.0.8/ResSimpy/Nexus/NexusKeywords/adsorption_keywords.py
--rw-r--r--   0        0        0        0 2024-02-27 16:37:15.265210 ressimpy-2.0.8/ResSimpy/Nexus/NexusKeywords/alphaf_keywords.py
--rw-r--r--   0        0        0      757 2024-02-27 16:37:15.265210 ressimpy-2.0.8/ResSimpy/Nexus/NexusKeywords/aquifer_keywords.py
--rw-r--r--   0        0        0        0 2024-02-27 16:37:15.265210 ressimpy-2.0.8/ResSimpy/Nexus/NexusKeywords/choke_keywords.py
--rw-r--r--   0        0        0        0 2024-02-27 16:37:15.265210 ressimpy-2.0.8/ResSimpy/Nexus/NexusKeywords/compressor_keywords.py
--rw-r--r--   0        0        0        0 2024-02-27 16:37:15.265210 ressimpy-2.0.8/ResSimpy/Nexus/NexusKeywords/eos_defaults_keywords.py
--rw-r--r--   0        0        0     1210 2024-02-27 16:37:15.265210 ressimpy-2.0.8/ResSimpy/Nexus/NexusKeywords/equil_keywords.py
--rw-r--r--   0        0        0        0 2024-02-27 16:37:15.265210 ressimpy-2.0.8/ResSimpy/Nexus/NexusKeywords/esp_keywords.py
--rw-r--r--   0        0        0     1368 2024-02-27 16:37:15.265210 ressimpy-2.0.8/ResSimpy/Nexus/NexusKeywords/fcs_keywords.py
--rw-r--r--   0        0        0        0 2024-02-27 16:37:15.265210 ressimpy-2.0.8/ResSimpy/Nexus/NexusKeywords/fluxin_keywords.py
--rw-r--r--   0        0        0      170 2024-02-27 16:37:15.265210 ressimpy-2.0.8/ResSimpy/Nexus/NexusKeywords/gaslift_keywords.py
--rw-r--r--   0        0        0     1159 2024-02-27 16:37:15.265210 ressimpy-2.0.8/ResSimpy/Nexus/NexusKeywords/hyd_keywords.py
--rw-r--r--   0        0        0        0 2024-02-27 16:37:15.265210 ressimpy-2.0.8/ResSimpy/Nexus/NexusKeywords/icd_keywords.py
--rw-r--r--   0        0        0        0 2024-02-27 16:37:15.265210 ressimpy-2.0.8/ResSimpy/Nexus/NexusKeywords/ipr_keywords.py
--rw-r--r--   0        0        0     2658 2024-02-27 16:37:15.265210 ressimpy-2.0.8/ResSimpy/Nexus/NexusKeywords/nexus_keywords.py
--rw-r--r--   0        0        0      795 2024-02-27 16:37:15.265210 ressimpy-2.0.8/ResSimpy/Nexus/NexusKeywords/options_keywords.py
--rw-r--r--   0        0        0        0 2024-02-27 16:37:15.265210 ressimpy-2.0.8/ResSimpy/Nexus/NexusKeywords/polymer_keywords.py
--rw-r--r--   0        0        0     5130 2024-02-27 16:37:15.265210 ressimpy-2.0.8/ResSimpy/Nexus/NexusKeywords/proc_keywords.py
--rw-r--r--   0        0        0        0 2024-02-27 16:37:15.265210 ressimpy-2.0.8/ResSimpy/Nexus/NexusKeywords/pump_keywords.py
--rw-r--r--   0        0        0     2547 2024-02-27 16:37:15.265210 ressimpy-2.0.8/ResSimpy/Nexus/NexusKeywords/pvt_keywords.py
--rw-r--r--   0        0        0     1579 2024-02-27 16:37:15.265210 ressimpy-2.0.8/ResSimpy/Nexus/NexusKeywords/relpm_keywords.py
--rw-r--r--   0        0        0      896 2024-02-27 16:37:15.265210 ressimpy-2.0.8/ResSimpy/Nexus/NexusKeywords/rock_keywords.py
--rw-r--r--   0        0        0     4957 2024-02-27 16:37:15.265210 ressimpy-2.0.8/ResSimpy/Nexus/NexusKeywords/runcontrol_keywords.py
--rw-r--r--   0        0        0      880 2024-02-27 16:37:15.265210 ressimpy-2.0.8/ResSimpy/Nexus/NexusKeywords/separator_keywords.py
--rw-r--r--   0        0        0     3082 2024-02-27 16:37:15.265210 ressimpy-2.0.8/ResSimpy/Nexus/NexusKeywords/structured_grid_keywords.py
--rw-r--r--   0        0        0     4492 2024-02-27 16:37:15.265210 ressimpy-2.0.8/ResSimpy/Nexus/NexusKeywords/surface_keywords.py
--rw-r--r--   0        0        0        0 2024-02-27 16:37:15.265210 ressimpy-2.0.8/ResSimpy/Nexus/NexusKeywords/tracer_init_keywords.py
--rw-r--r--   0        0        0      306 2024-02-27 16:37:15.265210 ressimpy-2.0.8/ResSimpy/Nexus/NexusKeywords/valve_keywords.py
--rw-r--r--   0        0        0      243 2024-02-27 16:37:15.265210 ressimpy-2.0.8/ResSimpy/Nexus/NexusKeywords/water_keywords.py
--rw-r--r--   0        0        0      902 2024-02-27 16:37:15.265210 ressimpy-2.0.8/ResSimpy/Nexus/NexusKeywords/wells_keywords.py
--rw-r--r--   0        0        0    17025 2024-02-27 16:37:15.265210 ressimpy-2.0.8/ResSimpy/Nexus/NexusNetwork.py
--rw-r--r--   0        0        0     3287 2024-02-27 16:37:15.265210 ressimpy-2.0.8/ResSimpy/Nexus/NexusPVTMethods.py
--rw-r--r--   0        0        0     3560 2024-02-27 16:37:15.265210 ressimpy-2.0.8/ResSimpy/Nexus/NexusRelPermMethods.py
--rw-r--r--   0        0        0    12256 2024-02-27 16:37:15.265210 ressimpy-2.0.8/ResSimpy/Nexus/NexusReporting.py
--rw-r--r--   0        0        0     3337 2024-02-27 16:37:15.265210 ressimpy-2.0.8/ResSimpy/Nexus/NexusRockMethods.py
--rw-r--r--   0        0        0     3612 2024-02-27 16:37:15.265210 ressimpy-2.0.8/ResSimpy/Nexus/NexusSeparatorMethods.py
--rw-r--r--   0        0        0    35694 2024-02-27 16:37:15.265210 ressimpy-2.0.8/ResSimpy/Nexus/NexusSimulator.py
--rw-r--r--   0        0        0    16873 2024-02-27 16:37:15.265210 ressimpy-2.0.8/ResSimpy/Nexus/NexusSolverParameters.py
--rw-r--r--   0        0        0     3376 2024-02-27 16:37:15.265210 ressimpy-2.0.8/ResSimpy/Nexus/NexusValveMethods.py
--rw-r--r--   0        0        0     3371 2024-02-27 16:37:15.265210 ressimpy-2.0.8/ResSimpy/Nexus/NexusWaterMethods.py
--rw-r--r--   0        0        0    23059 2024-02-27 16:37:15.265210 ressimpy-2.0.8/ResSimpy/Nexus/NexusWells.py
--rw-r--r--   0        0        0      404 2024-02-27 16:37:15.265210 ressimpy-2.0.8/ResSimpy/Nexus/__init__.py
--rw-r--r--   0        0        0    12453 2024-02-27 16:37:15.265210 ressimpy-2.0.8/ResSimpy/Nexus/array_function_operations.py
--rw-r--r--   0        0        0      115 2024-02-27 16:37:15.265210 ressimpy-2.0.8/ResSimpy/Nexus/constants.py
--rw-r--r--   0        0        0    22655 2024-02-27 16:37:15.265210 ressimpy-2.0.8/ResSimpy/Nexus/load_wells.py
--rw-r--r--   0        0        0    14101 2024-02-27 16:37:15.265210 ressimpy-2.0.8/ResSimpy/Nexus/logfile_operations.py
--rw-r--r--   0        0        0    16194 2024-02-27 16:37:15.265210 ressimpy-2.0.8/ResSimpy/Nexus/nexus_add_new_object_to_file.py
--rw-r--r--   0        0        0     8672 2024-02-27 16:37:15.265210 ressimpy-2.0.8/ResSimpy/Nexus/nexus_collect_tables.py
--rw-r--r--   0        0        0     9521 2024-02-27 16:37:15.265210 ressimpy-2.0.8/ResSimpy/Nexus/nexus_constraint_operations.py
--rw-r--r--   0        0        0    23162 2024-02-27 16:37:15.265210 ressimpy-2.0.8/ResSimpy/Nexus/nexus_file_operations.py
--rw-r--r--   0        0        0     4132 2024-02-27 16:37:15.265210 ressimpy-2.0.8/ResSimpy/Nexus/nexus_load_well_list.py
--rw-r--r--   0        0        0     2046 2024-02-27 16:37:15.265210 ressimpy-2.0.8/ResSimpy/Nexus/nexus_modify_object_in_file.py
--rw-r--r--   0        0        0     7768 2024-02-27 16:37:15.265210 ressimpy-2.0.8/ResSimpy/Nexus/nexus_remove_object_from_file.py
--rw-r--r--   0        0        0     5422 2024-02-27 16:37:15.265210 ressimpy-2.0.8/ResSimpy/Nexus/rel_perm_operations.py
--rw-r--r--   0        0        0    18379 2024-02-27 16:37:15.265210 ressimpy-2.0.8/ResSimpy/Nexus/runcontrol_operations.py
--rw-r--r--   0        0        0     9027 2024-02-27 16:37:15.269210 ressimpy-2.0.8/ResSimpy/Nexus/structured_grid_operations.py
--rw-r--r--   0        0        0      744 2024-02-27 16:37:15.269210 ressimpy-2.0.8/ResSimpy/Node.py
--rw-r--r--   0        0        0      918 2024-02-27 16:37:15.269210 ressimpy-2.0.8/ResSimpy/NodeConnection.py
--rw-r--r--   0        0        0      456 2024-02-27 16:37:15.269210 ressimpy-2.0.8/ResSimpy/NodeConnections.py
--rw-r--r--   0        0        0      398 2024-02-27 16:37:15.269210 ressimpy-2.0.8/ResSimpy/Nodes.py
--rw-r--r--   0        0        0        0 2024-02-27 16:37:15.269210 ressimpy-2.0.8/ResSimpy/OpenGoSim/DataModels/Network/__init__.py
--rw-r--r--   0        0        0     2368 2024-02-27 16:37:15.269210 ressimpy-2.0.8/ResSimpy/OpenGoSim/DataModels/OpenGoSimCompletion.py
--rw-r--r--   0        0        0     2812 2024-02-27 16:37:15.269210 ressimpy-2.0.8/ResSimpy/OpenGoSim/DataModels/OpenGoSimWell.py
--rw-r--r--   0        0        0        0 2024-02-27 16:37:15.269210 ressimpy-2.0.8/ResSimpy/OpenGoSim/DataModels/__init__.py
--rw-r--r--   0        0        0      199 2024-02-27 16:37:15.269210 ressimpy-2.0.8/ResSimpy/OpenGoSim/Enums/SimulationTypeEnum.py
--rw-r--r--   0        0        0        0 2024-02-27 16:37:15.269210 ressimpy-2.0.8/ResSimpy/OpenGoSim/Enums/__init__.py
--rw-r--r--   0        0        0      525 2024-02-27 16:37:15.269210 ressimpy-2.0.8/ResSimpy/OpenGoSim/Model_Parts/OpenGoSimNetwork.py
--rw-r--r--   0        0        0        0 2024-02-27 16:37:15.269210 ressimpy-2.0.8/ResSimpy/OpenGoSim/Model_Parts/__init__.py
--rw-r--r--   0        0        0     2892 2024-02-27 16:37:15.269210 ressimpy-2.0.8/ResSimpy/OpenGoSim/OpenGoSimKeywords/OpenGoSimKeywords.py
--rw-r--r--   0        0        0        0 2024-02-27 16:37:15.269210 ressimpy-2.0.8/ResSimpy/OpenGoSim/OpenGoSimKeywords/__init__.py
--rw-r--r--   0        0        0    10767 2024-02-27 16:37:15.269210 ressimpy-2.0.8/ResSimpy/OpenGoSim/OpenGoSimSimulator.py
--rw-r--r--   0        0        0      462 2024-02-27 16:37:15.269210 ressimpy-2.0.8/ResSimpy/OpenGoSim/OpenGoSimWells.py
--rw-r--r--   0        0        0        0 2024-02-27 16:37:15.269210 ressimpy-2.0.8/ResSimpy/OpenGoSim/__init__.py
--rw-r--r--   0        0        0     2382 2024-02-27 16:37:15.269210 ressimpy-2.0.8/ResSimpy/OperationsMixin.py
--rw-r--r--   0        0        0      442 2024-02-27 16:37:15.269210 ressimpy-2.0.8/ResSimpy/PVT.py
--rw-r--r--   0        0        0      467 2024-02-27 16:37:15.269210 ressimpy-2.0.8/ResSimpy/RelPerm.py
--rw-r--r--   0        0        0     3389 2024-02-27 16:37:15.269210 ressimpy-2.0.8/ResSimpy/RelPermEndPoint.py
--rw-r--r--   0        0        0      473 2024-02-27 16:37:15.269210 ressimpy-2.0.8/ResSimpy/Rock.py
--rw-r--r--   0        0        0      493 2024-02-27 16:37:15.269210 ressimpy-2.0.8/ResSimpy/Separator.py
--rw-r--r--   0        0        0     4356 2024-02-27 16:37:15.269210 ressimpy-2.0.8/ResSimpy/Simulator.py
--rw-r--r--   0        0        0      407 2024-02-27 16:37:15.269210 ressimpy-2.0.8/ResSimpy/SolverParameter.py
--rw-r--r--   0        0        0      671 2024-02-27 16:37:15.269210 ressimpy-2.0.8/ResSimpy/SolverParameters.py
--rw-r--r--   0        0        0     1484 2024-02-27 16:37:15.269210 ressimpy-2.0.8/ResSimpy/Target.py
--rw-r--r--   0        0        0      412 2024-02-27 16:37:15.269210 ressimpy-2.0.8/ResSimpy/Targets.py
--rw-r--r--   0        0        0     1223 2024-02-27 16:37:15.269210 ressimpy-2.0.8/ResSimpy/Units/AttributeMapping.py
--rw-r--r--   0        0        0     2082 2024-02-27 16:37:15.269210 ressimpy-2.0.8/ResSimpy/Units/AttributeMappings/BaseUnitMapping.py
--rw-r--r--   0        0        0     8560 2024-02-27 16:37:15.269210 ressimpy-2.0.8/ResSimpy/Units/AttributeMappings/CompletionUnitMapping.py
--rw-r--r--   0        0        0    17243 2024-02-27 16:37:15.269210 ressimpy-2.0.8/ResSimpy/Units/AttributeMappings/ConstraintUnitMapping.py
--rw-r--r--   0        0        0    29827 2024-02-27 16:37:15.269210 ressimpy-2.0.8/ResSimpy/Units/AttributeMappings/DynamicPropertyUnitMapping.py
--rw-r--r--   0        0        0    15234 2024-02-27 16:37:15.269210 ressimpy-2.0.8/ResSimpy/Units/AttributeMappings/NetworkUnitMapping.py
--rw-r--r--   0        0        0       96 2024-02-27 16:37:15.269210 ressimpy-2.0.8/ResSimpy/Units/AttributeMappings/__init__.py
--rw-r--r--   0        0        0    14870 2024-02-27 16:37:15.269210 ressimpy-2.0.8/ResSimpy/Units/Units.py
--rw-r--r--   0        0        0       45 2024-02-27 16:37:15.269210 ressimpy-2.0.8/ResSimpy/Units/__init__.py
--rw-r--r--   0        0        0       95 2024-02-27 16:37:15.269210 ressimpy-2.0.8/ResSimpy/Utils/__init__.py
--rw-r--r--   0        0        0     2355 2024-02-27 16:37:15.269210 ressimpy-2.0.8/ResSimpy/Utils/factory_methods.py
--rw-r--r--   0        0        0     1315 2024-02-27 16:37:15.269210 ressimpy-2.0.8/ResSimpy/Utils/generic_repr.py
--rw-r--r--   0        0        0     1585 2024-02-27 16:37:15.269210 ressimpy-2.0.8/ResSimpy/Utils/invert_nexus_map.py
--rw-r--r--   0        0        0      453 2024-02-27 16:37:15.269210 ressimpy-2.0.8/ResSimpy/Utils/obj_to_dataframe.py
--rw-r--r--   0        0        0     1364 2024-02-27 16:37:15.269210 ressimpy-2.0.8/ResSimpy/Utils/obj_to_table_string.py
--rw-r--r--   0        0        0     2359 2024-02-27 16:37:15.269210 ressimpy-2.0.8/ResSimpy/Utils/to_dict_generic.py
--rw-r--r--   0        0        0      477 2024-02-27 16:37:15.269210 ressimpy-2.0.8/ResSimpy/Valve.py
--rw-r--r--   0        0        0      479 2024-02-27 16:37:15.269210 ressimpy-2.0.8/ResSimpy/Water.py
--rw-r--r--   0        0        0     4369 2024-02-27 16:37:15.269210 ressimpy-2.0.8/ResSimpy/Well.py
--rw-r--r--   0        0        0     1027 2024-02-27 16:37:15.269210 ressimpy-2.0.8/ResSimpy/WellConnection.py
--rw-r--r--   0        0        0      435 2024-02-27 16:37:15.269210 ressimpy-2.0.8/ResSimpy/WellConnections.py
--rw-r--r--   0        0        0      474 2024-02-27 16:37:15.269210 ressimpy-2.0.8/ResSimpy/WellLists.py
--rw-r--r--   0        0        0      755 2024-02-27 16:37:15.269210 ressimpy-2.0.8/ResSimpy/Wellbore.py
--rw-r--r--   0        0        0      439 2024-02-27 16:37:15.269210 ressimpy-2.0.8/ResSimpy/Wellbores.py
--rw-r--r--   0        0        0      809 2024-02-27 16:37:15.269210 ressimpy-2.0.8/ResSimpy/Wellhead.py
--rw-r--r--   0        0        0      426 2024-02-27 16:37:15.269210 ressimpy-2.0.8/ResSimpy/Wellheads.py
--rw-r--r--   0        0        0     3070 2024-02-27 16:37:15.269210 ressimpy-2.0.8/ResSimpy/Wells.py
--rw-r--r--   0        0        0      289 2024-02-27 16:37:26.781232 ressimpy-2.0.8/ResSimpy/__init__.py
--rw-r--r--   0        0        0     2741 2024-02-27 16:37:26.781232 ressimpy-2.0.8/pyproject.toml
--rw-r--r--   0        0        0     6550 1970-01-01 00:00:00.000000 ressimpy-2.0.8/PKG-INFO
+-rw-r--r--   0        0        0     9156 2024-03-05 13:51:34.234753 ressimpy-2.0.9/LICENSE.MD
+-rw-r--r--   0        0        0     5660 2024-03-05 13:51:34.234753 ressimpy-2.0.9/README.md
+-rw-r--r--   0        0        0      504 2024-03-05 13:51:34.234753 ressimpy-2.0.9/ResSimpy/Aquifer.py
+-rw-r--r--   0        0        0     8573 2024-03-05 13:51:34.234753 ressimpy-2.0.9/ResSimpy/Completion.py
+-rw-r--r--   0        0        0     1419 2024-03-05 13:51:34.234753 ressimpy-2.0.9/ResSimpy/Constraint.py
+-rw-r--r--   0        0        0     1908 2024-03-05 13:51:34.234753 ressimpy-2.0.9/ResSimpy/Constraints.py
+-rw-r--r--   0        0        0     3926 2024-03-05 13:51:34.234753 ressimpy-2.0.9/ResSimpy/DataObjectMixin.py
+-rw-r--r--   0        0        0     4109 2024-03-05 13:51:34.234753 ressimpy-2.0.9/ResSimpy/DynamicProperty.py
+-rw-r--r--   0        0        0      358 2024-03-05 13:51:34.234753 ressimpy-2.0.9/ResSimpy/Enums/FluidTypeEnums.py
+-rw-r--r--   0        0        0      369 2024-03-05 13:51:34.234753 ressimpy-2.0.9/ResSimpy/Enums/FrequencyEnum.py
+-rw-r--r--   0        0        0      168 2024-03-05 13:51:34.234753 ressimpy-2.0.9/ResSimpy/Enums/HowEnum.py
+-rw-r--r--   0        0        0      214 2024-03-05 13:51:34.234753 ressimpy-2.0.9/ResSimpy/Enums/OutputType.py
+-rw-r--r--   0        0        0      282 2024-03-05 13:51:34.234753 ressimpy-2.0.9/ResSimpy/Enums/PenetrationDirectionEnum.py
+-rw-r--r--   0        0        0      253 2024-03-05 13:51:34.234753 ressimpy-2.0.9/ResSimpy/Enums/TimeSteppingMethodEnum.py
+-rw-r--r--   0        0        0      507 2024-03-05 13:51:34.234753 ressimpy-2.0.9/ResSimpy/Enums/UnitsEnum.py
+-rw-r--r--   0        0        0      377 2024-03-05 13:51:34.234753 ressimpy-2.0.9/ResSimpy/Enums/WellTypeEnum.py
+-rw-r--r--   0        0        0       62 2024-03-05 13:51:34.234753 ressimpy-2.0.9/ResSimpy/Enums/__init__.py
+-rw-r--r--   0        0        0      506 2024-03-05 13:51:34.234753 ressimpy-2.0.9/ResSimpy/Equilibration.py
+-rw-r--r--   0        0        0     8911 2024-03-05 13:51:34.234753 ressimpy-2.0.9/ResSimpy/File.py
+-rw-r--r--   0        0        0     2257 2024-03-05 13:51:34.234753 ressimpy-2.0.9/ResSimpy/FileBase.py
+-rw-r--r--   0        0        0        0 2024-03-05 13:51:34.234753 ressimpy-2.0.9/ResSimpy/FileOperations/__init__.py
+-rw-r--r--   0        0        0    22606 2024-03-05 13:51:34.234753 ressimpy-2.0.9/ResSimpy/FileOperations/file_operations.py
+-rw-r--r--   0        0        0      413 2024-03-05 13:51:34.234753 ressimpy-2.0.9/ResSimpy/Gaslift.py
+-rw-r--r--   0        0        0     2631 2024-03-05 13:51:34.234753 ressimpy-2.0.9/ResSimpy/Grid.py
+-rw-r--r--   0        0        0      393 2024-03-05 13:51:34.234753 ressimpy-2.0.9/ResSimpy/Grids.py
+-rw-r--r--   0        0        0      470 2024-03-05 13:51:34.234753 ressimpy-2.0.9/ResSimpy/Hydraulics.py
+-rw-r--r--   0        0        0     3147 2024-03-05 13:51:34.234753 ressimpy-2.0.9/ResSimpy/ISODateTime.py
+-rw-r--r--   0        0        0      588 2024-03-05 13:51:34.234753 ressimpy-2.0.9/ResSimpy/Network.py
+-rw-r--r--   0        0        0      545 2024-03-05 13:51:34.238753 ressimpy-2.0.9/ResSimpy/Nexus/DataModels/FcsConfig.py
+-rw-r--r--   0        0        0    23652 2024-03-05 13:51:34.238753 ressimpy-2.0.9/ResSimpy/Nexus/DataModels/FcsFile.py
+-rw-r--r--   0        0        0    21550 2024-03-05 13:51:34.238753 ressimpy-2.0.9/ResSimpy/Nexus/DataModels/Network/NexusConstraint.py
+-rw-r--r--   0        0        0    17761 2024-03-05 13:51:34.238753 ressimpy-2.0.9/ResSimpy/Nexus/DataModels/Network/NexusConstraints.py
+-rw-r--r--   0        0        0     1718 2024-03-05 13:51:34.238753 ressimpy-2.0.9/ResSimpy/Nexus/DataModels/Network/NexusNode.py
+-rw-r--r--   0        0        0     4917 2024-03-05 13:51:34.238753 ressimpy-2.0.9/ResSimpy/Nexus/DataModels/Network/NexusNodeConnection.py
+-rw-r--r--   0        0        0     6436 2024-03-05 13:51:34.238753 ressimpy-2.0.9/ResSimpy/Nexus/DataModels/Network/NexusNodeConnections.py
+-rw-r--r--   0        0        0     6543 2024-03-05 13:51:34.238753 ressimpy-2.0.9/ResSimpy/Nexus/DataModels/Network/NexusNodes.py
+-rw-r--r--   0        0        0     4071 2024-03-05 13:51:34.238753 ressimpy-2.0.9/ResSimpy/Nexus/DataModels/Network/NexusProc.py
+-rw-r--r--   0        0        0     1124 2024-03-05 13:51:34.238753 ressimpy-2.0.9/ResSimpy/Nexus/DataModels/Network/NexusProcs.py
+-rw-r--r--   0        0        0     2084 2024-03-05 13:51:34.238753 ressimpy-2.0.9/ResSimpy/Nexus/DataModels/Network/NexusTarget.py
+-rw-r--r--   0        0        0     6763 2024-03-05 13:51:34.238753 ressimpy-2.0.9/ResSimpy/Nexus/DataModels/Network/NexusTargets.py
+-rw-r--r--   0        0        0     6510 2024-03-05 13:51:34.238753 ressimpy-2.0.9/ResSimpy/Nexus/DataModels/Network/NexusWellConnection.py
+-rw-r--r--   0        0        0     6647 2024-03-05 13:51:34.238753 ressimpy-2.0.9/ResSimpy/Nexus/DataModels/Network/NexusWellConnections.py
+-rw-r--r--   0        0        0     2191 2024-03-05 13:51:34.238753 ressimpy-2.0.9/ResSimpy/Nexus/DataModels/Network/NexusWellLists.py
+-rw-r--r--   0        0        0     2780 2024-03-05 13:51:34.238753 ressimpy-2.0.9/ResSimpy/Nexus/DataModels/Network/NexusWellbore.py
+-rw-r--r--   0        0        0     5892 2024-03-05 13:51:34.238753 ressimpy-2.0.9/ResSimpy/Nexus/DataModels/Network/NexusWellbores.py
+-rw-r--r--   0        0        0     4535 2024-03-05 13:51:34.238753 ressimpy-2.0.9/ResSimpy/Nexus/DataModels/Network/NexusWellhead.py
+-rw-r--r--   0        0        0     5815 2024-03-05 13:51:34.238753 ressimpy-2.0.9/ResSimpy/Nexus/DataModels/Network/NexusWellheads.py
+-rw-r--r--   0        0        0      329 2024-03-05 13:51:34.238753 ressimpy-2.0.9/ResSimpy/Nexus/DataModels/Network/__init__.py
+-rw-r--r--   0        0        0     8313 2024-03-05 13:51:34.238753 ressimpy-2.0.9/ResSimpy/Nexus/DataModels/NexusAquiferMethod.py
+-rw-r--r--   0        0        0    14155 2024-03-05 13:51:34.238753 ressimpy-2.0.9/ResSimpy/Nexus/DataModels/NexusCompletion.py
+-rw-r--r--   0        0        0    10788 2024-03-05 13:51:34.238753 ressimpy-2.0.9/ResSimpy/Nexus/DataModels/NexusEquilMethod.py
+-rw-r--r--   0        0        0    32379 2024-03-05 13:51:34.238753 ressimpy-2.0.9/ResSimpy/Nexus/DataModels/NexusFile.py
+-rw-r--r--   0        0        0     6211 2024-03-05 13:51:34.238753 ressimpy-2.0.9/ResSimpy/Nexus/DataModels/NexusGasliftMethod.py
+-rw-r--r--   0        0        0    13247 2024-03-05 13:51:34.238753 ressimpy-2.0.9/ResSimpy/Nexus/DataModels/NexusHydraulicsMethod.py
+-rw-r--r--   0        0        0    30699 2024-03-05 13:51:34.238753 ressimpy-2.0.9/ResSimpy/Nexus/DataModels/NexusPVTMethod.py
+-rw-r--r--   0        0        0     2718 2024-03-05 13:51:34.238753 ressimpy-2.0.9/ResSimpy/Nexus/DataModels/NexusRelPermEndPoint.py
+-rw-r--r--   0        0        0    19602 2024-03-05 13:51:34.238753 ressimpy-2.0.9/ResSimpy/Nexus/DataModels/NexusRelPermMethod.py
+-rw-r--r--   0        0        0     9467 2024-03-05 13:51:34.238753 ressimpy-2.0.9/ResSimpy/Nexus/DataModels/NexusRockMethod.py
+-rw-r--r--   0        0        0     9032 2024-03-05 13:51:34.238753 ressimpy-2.0.9/ResSimpy/Nexus/DataModels/NexusSeparatorMethod.py
+-rw-r--r--   0        0        0    15015 2024-03-05 13:51:34.238753 ressimpy-2.0.9/ResSimpy/Nexus/DataModels/NexusSolverParameter.py
+-rw-r--r--   0        0        0     6112 2024-03-05 13:51:34.238753 ressimpy-2.0.9/ResSimpy/Nexus/DataModels/NexusValveMethod.py
+-rw-r--r--   0        0        0    11098 2024-03-05 13:51:34.238753 ressimpy-2.0.9/ResSimpy/Nexus/DataModels/NexusWaterMethod.py
+-rw-r--r--   0        0        0     8247 2024-03-05 13:51:34.238753 ressimpy-2.0.9/ResSimpy/Nexus/DataModels/NexusWell.py
+-rw-r--r--   0        0        0      781 2024-03-05 13:51:34.238753 ressimpy-2.0.9/ResSimpy/Nexus/DataModels/NexusWellList.py
+-rw-r--r--   0        0        0     2858 2024-03-05 13:51:34.238753 ressimpy-2.0.9/ResSimpy/Nexus/DataModels/NexusWellMod.py
+-rw-r--r--   0        0        0    14838 2024-03-05 13:51:34.238753 ressimpy-2.0.9/ResSimpy/Nexus/DataModels/StructuredGrid/NexusGrid.py
+-rw-r--r--   0        0        0       67 2024-03-05 13:51:34.238753 ressimpy-2.0.9/ResSimpy/Nexus/DataModels/StructuredGrid/__init__.py
+-rw-r--r--   0        0        0       77 2024-03-05 13:51:34.238753 ressimpy-2.0.9/ResSimpy/Nexus/DataModels/__init__.py
+-rw-r--r--   0        0        0     3396 2024-03-05 13:51:34.238753 ressimpy-2.0.9/ResSimpy/Nexus/NexusAquiferMethods.py
+-rw-r--r--   0        0        0      273 2024-03-05 13:51:34.238753 ressimpy-2.0.9/ResSimpy/Nexus/NexusEnums/DateFormatEnum.py
+-rw-r--r--   0        0        0      106 2024-03-05 13:51:34.238753 ressimpy-2.0.9/ResSimpy/Nexus/NexusEnums/__init__.py
+-rw-r--r--   0        0        0     3374 2024-03-05 13:51:34.238753 ressimpy-2.0.9/ResSimpy/Nexus/NexusEquilMethods.py
+-rw-r--r--   0        0        0     3345 2024-03-05 13:51:34.238753 ressimpy-2.0.9/ResSimpy/Nexus/NexusGasliftMethods.py
+-rw-r--r--   0        0        0       43 2024-03-05 13:51:34.238753 ressimpy-2.0.9/ResSimpy/Nexus/NexusGrids.py
+-rw-r--r--   0        0        0     3418 2024-03-05 13:51:34.238753 ressimpy-2.0.9/ResSimpy/Nexus/NexusHydraulicsMethods.py
+-rw-r--r--   0        0        0       47 2024-03-05 13:51:34.238753 ressimpy-2.0.9/ResSimpy/Nexus/NexusKeywords/__init__.py
+-rw-r--r--   0        0        0        0 2024-03-05 13:51:34.238753 ressimpy-2.0.9/ResSimpy/Nexus/NexusKeywords/adsorption_keywords.py
+-rw-r--r--   0        0        0        0 2024-03-05 13:51:34.238753 ressimpy-2.0.9/ResSimpy/Nexus/NexusKeywords/alphaf_keywords.py
+-rw-r--r--   0        0        0      757 2024-03-05 13:51:34.238753 ressimpy-2.0.9/ResSimpy/Nexus/NexusKeywords/aquifer_keywords.py
+-rw-r--r--   0        0        0        0 2024-03-05 13:51:34.238753 ressimpy-2.0.9/ResSimpy/Nexus/NexusKeywords/choke_keywords.py
+-rw-r--r--   0        0        0        0 2024-03-05 13:51:34.238753 ressimpy-2.0.9/ResSimpy/Nexus/NexusKeywords/compressor_keywords.py
+-rw-r--r--   0        0        0        0 2024-03-05 13:51:34.238753 ressimpy-2.0.9/ResSimpy/Nexus/NexusKeywords/eos_defaults_keywords.py
+-rw-r--r--   0        0        0     1210 2024-03-05 13:51:34.238753 ressimpy-2.0.9/ResSimpy/Nexus/NexusKeywords/equil_keywords.py
+-rw-r--r--   0        0        0        0 2024-03-05 13:51:34.238753 ressimpy-2.0.9/ResSimpy/Nexus/NexusKeywords/esp_keywords.py
+-rw-r--r--   0        0        0     1368 2024-03-05 13:51:34.238753 ressimpy-2.0.9/ResSimpy/Nexus/NexusKeywords/fcs_keywords.py
+-rw-r--r--   0        0        0        0 2024-03-05 13:51:34.238753 ressimpy-2.0.9/ResSimpy/Nexus/NexusKeywords/fluxin_keywords.py
+-rw-r--r--   0        0        0      170 2024-03-05 13:51:34.238753 ressimpy-2.0.9/ResSimpy/Nexus/NexusKeywords/gaslift_keywords.py
+-rw-r--r--   0        0        0     1159 2024-03-05 13:51:34.238753 ressimpy-2.0.9/ResSimpy/Nexus/NexusKeywords/hyd_keywords.py
+-rw-r--r--   0        0        0        0 2024-03-05 13:51:34.238753 ressimpy-2.0.9/ResSimpy/Nexus/NexusKeywords/icd_keywords.py
+-rw-r--r--   0        0        0        0 2024-03-05 13:51:34.238753 ressimpy-2.0.9/ResSimpy/Nexus/NexusKeywords/ipr_keywords.py
+-rw-r--r--   0        0        0     2658 2024-03-05 13:51:34.238753 ressimpy-2.0.9/ResSimpy/Nexus/NexusKeywords/nexus_keywords.py
+-rw-r--r--   0        0        0      795 2024-03-05 13:51:34.238753 ressimpy-2.0.9/ResSimpy/Nexus/NexusKeywords/options_keywords.py
+-rw-r--r--   0        0        0        0 2024-03-05 13:51:34.238753 ressimpy-2.0.9/ResSimpy/Nexus/NexusKeywords/polymer_keywords.py
+-rw-r--r--   0        0        0     5130 2024-03-05 13:51:34.238753 ressimpy-2.0.9/ResSimpy/Nexus/NexusKeywords/proc_keywords.py
+-rw-r--r--   0        0        0        0 2024-03-05 13:51:34.238753 ressimpy-2.0.9/ResSimpy/Nexus/NexusKeywords/pump_keywords.py
+-rw-r--r--   0        0        0     2547 2024-03-05 13:51:34.242753 ressimpy-2.0.9/ResSimpy/Nexus/NexusKeywords/pvt_keywords.py
+-rw-r--r--   0        0        0     1579 2024-03-05 13:51:34.242753 ressimpy-2.0.9/ResSimpy/Nexus/NexusKeywords/relpm_keywords.py
+-rw-r--r--   0        0        0      896 2024-03-05 13:51:34.242753 ressimpy-2.0.9/ResSimpy/Nexus/NexusKeywords/rock_keywords.py
+-rw-r--r--   0        0        0     4957 2024-03-05 13:51:34.242753 ressimpy-2.0.9/ResSimpy/Nexus/NexusKeywords/runcontrol_keywords.py
+-rw-r--r--   0        0        0      880 2024-03-05 13:51:34.242753 ressimpy-2.0.9/ResSimpy/Nexus/NexusKeywords/separator_keywords.py
+-rw-r--r--   0        0        0     3082 2024-03-05 13:51:34.242753 ressimpy-2.0.9/ResSimpy/Nexus/NexusKeywords/structured_grid_keywords.py
+-rw-r--r--   0        0        0     4492 2024-03-05 13:51:34.242753 ressimpy-2.0.9/ResSimpy/Nexus/NexusKeywords/surface_keywords.py
+-rw-r--r--   0        0        0        0 2024-03-05 13:51:34.242753 ressimpy-2.0.9/ResSimpy/Nexus/NexusKeywords/tracer_init_keywords.py
+-rw-r--r--   0        0        0      306 2024-03-05 13:51:34.242753 ressimpy-2.0.9/ResSimpy/Nexus/NexusKeywords/valve_keywords.py
+-rw-r--r--   0        0        0      243 2024-03-05 13:51:34.242753 ressimpy-2.0.9/ResSimpy/Nexus/NexusKeywords/water_keywords.py
+-rw-r--r--   0        0        0      902 2024-03-05 13:51:34.242753 ressimpy-2.0.9/ResSimpy/Nexus/NexusKeywords/wells_keywords.py
+-rw-r--r--   0        0        0    17025 2024-03-05 13:51:34.242753 ressimpy-2.0.9/ResSimpy/Nexus/NexusNetwork.py
+-rw-r--r--   0        0        0     3287 2024-03-05 13:51:34.242753 ressimpy-2.0.9/ResSimpy/Nexus/NexusPVTMethods.py
+-rw-r--r--   0        0        0     3560 2024-03-05 13:51:34.242753 ressimpy-2.0.9/ResSimpy/Nexus/NexusRelPermMethods.py
+-rw-r--r--   0        0        0    12256 2024-03-05 13:51:34.242753 ressimpy-2.0.9/ResSimpy/Nexus/NexusReporting.py
+-rw-r--r--   0        0        0     3337 2024-03-05 13:51:34.242753 ressimpy-2.0.9/ResSimpy/Nexus/NexusRockMethods.py
+-rw-r--r--   0        0        0     3678 2024-03-05 13:51:34.242753 ressimpy-2.0.9/ResSimpy/Nexus/NexusSeparatorMethods.py
+-rw-r--r--   0        0        0    35694 2024-03-05 13:51:34.242753 ressimpy-2.0.9/ResSimpy/Nexus/NexusSimulator.py
+-rw-r--r--   0        0        0    16873 2024-03-05 13:51:34.242753 ressimpy-2.0.9/ResSimpy/Nexus/NexusSolverParameters.py
+-rw-r--r--   0        0        0     3376 2024-03-05 13:51:34.242753 ressimpy-2.0.9/ResSimpy/Nexus/NexusValveMethods.py
+-rw-r--r--   0        0        0     3371 2024-03-05 13:51:34.242753 ressimpy-2.0.9/ResSimpy/Nexus/NexusWaterMethods.py
+-rw-r--r--   0        0        0    23059 2024-03-05 13:51:34.242753 ressimpy-2.0.9/ResSimpy/Nexus/NexusWells.py
+-rw-r--r--   0        0        0      404 2024-03-05 13:51:34.242753 ressimpy-2.0.9/ResSimpy/Nexus/__init__.py
+-rw-r--r--   0        0        0    12453 2024-03-05 13:51:34.242753 ressimpy-2.0.9/ResSimpy/Nexus/array_function_operations.py
+-rw-r--r--   0        0        0      115 2024-03-05 13:51:34.242753 ressimpy-2.0.9/ResSimpy/Nexus/constants.py
+-rw-r--r--   0        0        0    22655 2024-03-05 13:51:34.242753 ressimpy-2.0.9/ResSimpy/Nexus/load_wells.py
+-rw-r--r--   0        0        0    14101 2024-03-05 13:51:34.242753 ressimpy-2.0.9/ResSimpy/Nexus/logfile_operations.py
+-rw-r--r--   0        0        0    16194 2024-03-05 13:51:34.242753 ressimpy-2.0.9/ResSimpy/Nexus/nexus_add_new_object_to_file.py
+-rw-r--r--   0        0        0     8573 2024-03-05 13:51:34.242753 ressimpy-2.0.9/ResSimpy/Nexus/nexus_collect_tables.py
+-rw-r--r--   0        0        0     7107 2024-03-05 13:51:34.242753 ressimpy-2.0.9/ResSimpy/Nexus/nexus_constraint_operations.py
+-rw-r--r--   0        0        0    23162 2024-03-05 13:51:34.242753 ressimpy-2.0.9/ResSimpy/Nexus/nexus_file_operations.py
+-rw-r--r--   0        0        0     4132 2024-03-05 13:51:34.242753 ressimpy-2.0.9/ResSimpy/Nexus/nexus_load_well_list.py
+-rw-r--r--   0        0        0     2046 2024-03-05 13:51:34.242753 ressimpy-2.0.9/ResSimpy/Nexus/nexus_modify_object_in_file.py
+-rw-r--r--   0        0        0     7768 2024-03-05 13:51:34.242753 ressimpy-2.0.9/ResSimpy/Nexus/nexus_remove_object_from_file.py
+-rw-r--r--   0        0        0     5422 2024-03-05 13:51:34.242753 ressimpy-2.0.9/ResSimpy/Nexus/rel_perm_operations.py
+-rw-r--r--   0        0        0    18379 2024-03-05 13:51:34.242753 ressimpy-2.0.9/ResSimpy/Nexus/runcontrol_operations.py
+-rw-r--r--   0        0        0     9027 2024-03-05 13:51:34.242753 ressimpy-2.0.9/ResSimpy/Nexus/structured_grid_operations.py
+-rw-r--r--   0        0        0      744 2024-03-05 13:51:34.242753 ressimpy-2.0.9/ResSimpy/Node.py
+-rw-r--r--   0        0        0      918 2024-03-05 13:51:34.242753 ressimpy-2.0.9/ResSimpy/NodeConnection.py
+-rw-r--r--   0        0        0      456 2024-03-05 13:51:34.242753 ressimpy-2.0.9/ResSimpy/NodeConnections.py
+-rw-r--r--   0        0        0      398 2024-03-05 13:51:34.242753 ressimpy-2.0.9/ResSimpy/Nodes.py
+-rw-r--r--   0        0        0        0 2024-03-05 13:51:34.242753 ressimpy-2.0.9/ResSimpy/OpenGoSim/DataModels/Network/__init__.py
+-rw-r--r--   0        0        0     2368 2024-03-05 13:51:34.242753 ressimpy-2.0.9/ResSimpy/OpenGoSim/DataModels/OpenGoSimCompletion.py
+-rw-r--r--   0        0        0     2812 2024-03-05 13:51:34.242753 ressimpy-2.0.9/ResSimpy/OpenGoSim/DataModels/OpenGoSimWell.py
+-rw-r--r--   0        0        0        0 2024-03-05 13:51:34.242753 ressimpy-2.0.9/ResSimpy/OpenGoSim/DataModels/__init__.py
+-rw-r--r--   0        0        0      199 2024-03-05 13:51:34.242753 ressimpy-2.0.9/ResSimpy/OpenGoSim/Enums/SimulationTypeEnum.py
+-rw-r--r--   0        0        0        0 2024-03-05 13:51:34.242753 ressimpy-2.0.9/ResSimpy/OpenGoSim/Enums/__init__.py
+-rw-r--r--   0        0        0      525 2024-03-05 13:51:34.242753 ressimpy-2.0.9/ResSimpy/OpenGoSim/Model_Parts/OpenGoSimNetwork.py
+-rw-r--r--   0        0        0        0 2024-03-05 13:51:34.242753 ressimpy-2.0.9/ResSimpy/OpenGoSim/Model_Parts/__init__.py
+-rw-r--r--   0        0        0     2892 2024-03-05 13:51:34.242753 ressimpy-2.0.9/ResSimpy/OpenGoSim/OpenGoSimKeywords/OpenGoSimKeywords.py
+-rw-r--r--   0        0        0        0 2024-03-05 13:51:34.242753 ressimpy-2.0.9/ResSimpy/OpenGoSim/OpenGoSimKeywords/__init__.py
+-rw-r--r--   0        0        0    10767 2024-03-05 13:51:34.242753 ressimpy-2.0.9/ResSimpy/OpenGoSim/OpenGoSimSimulator.py
+-rw-r--r--   0        0        0      462 2024-03-05 13:51:34.242753 ressimpy-2.0.9/ResSimpy/OpenGoSim/OpenGoSimWells.py
+-rw-r--r--   0        0        0        0 2024-03-05 13:51:34.242753 ressimpy-2.0.9/ResSimpy/OpenGoSim/__init__.py
+-rw-r--r--   0        0        0     2382 2024-03-05 13:51:34.242753 ressimpy-2.0.9/ResSimpy/OperationsMixin.py
+-rw-r--r--   0        0        0      442 2024-03-05 13:51:34.242753 ressimpy-2.0.9/ResSimpy/PVT.py
+-rw-r--r--   0        0        0      467 2024-03-05 13:51:34.242753 ressimpy-2.0.9/ResSimpy/RelPerm.py
+-rw-r--r--   0        0        0     3389 2024-03-05 13:51:34.242753 ressimpy-2.0.9/ResSimpy/RelPermEndPoint.py
+-rw-r--r--   0        0        0      473 2024-03-05 13:51:34.242753 ressimpy-2.0.9/ResSimpy/Rock.py
+-rw-r--r--   0        0        0      493 2024-03-05 13:51:34.242753 ressimpy-2.0.9/ResSimpy/Separator.py
+-rw-r--r--   0        0        0     4356 2024-03-05 13:51:34.242753 ressimpy-2.0.9/ResSimpy/Simulator.py
+-rw-r--r--   0        0        0      407 2024-03-05 13:51:34.242753 ressimpy-2.0.9/ResSimpy/SolverParameter.py
+-rw-r--r--   0        0        0      671 2024-03-05 13:51:34.242753 ressimpy-2.0.9/ResSimpy/SolverParameters.py
+-rw-r--r--   0        0        0     1484 2024-03-05 13:51:34.242753 ressimpy-2.0.9/ResSimpy/Target.py
+-rw-r--r--   0        0        0      412 2024-03-05 13:51:34.242753 ressimpy-2.0.9/ResSimpy/Targets.py
+-rw-r--r--   0        0        0     1223 2024-03-05 13:51:34.242753 ressimpy-2.0.9/ResSimpy/Units/AttributeMapping.py
+-rw-r--r--   0        0        0     2082 2024-03-05 13:51:34.242753 ressimpy-2.0.9/ResSimpy/Units/AttributeMappings/BaseUnitMapping.py
+-rw-r--r--   0        0        0     8560 2024-03-05 13:51:34.242753 ressimpy-2.0.9/ResSimpy/Units/AttributeMappings/CompletionUnitMapping.py
+-rw-r--r--   0        0        0    17243 2024-03-05 13:51:34.246753 ressimpy-2.0.9/ResSimpy/Units/AttributeMappings/ConstraintUnitMapping.py
+-rw-r--r--   0        0        0    29827 2024-03-05 13:51:34.246753 ressimpy-2.0.9/ResSimpy/Units/AttributeMappings/DynamicPropertyUnitMapping.py
+-rw-r--r--   0        0        0    15234 2024-03-05 13:51:34.246753 ressimpy-2.0.9/ResSimpy/Units/AttributeMappings/NetworkUnitMapping.py
+-rw-r--r--   0        0        0       96 2024-03-05 13:51:34.246753 ressimpy-2.0.9/ResSimpy/Units/AttributeMappings/__init__.py
+-rw-r--r--   0        0        0    14870 2024-03-05 13:51:34.246753 ressimpy-2.0.9/ResSimpy/Units/Units.py
+-rw-r--r--   0        0        0       45 2024-03-05 13:51:34.246753 ressimpy-2.0.9/ResSimpy/Units/__init__.py
+-rw-r--r--   0        0        0       95 2024-03-05 13:51:34.246753 ressimpy-2.0.9/ResSimpy/Utils/__init__.py
+-rw-r--r--   0        0        0     2355 2024-03-05 13:51:34.246753 ressimpy-2.0.9/ResSimpy/Utils/factory_methods.py
+-rw-r--r--   0        0        0     1315 2024-03-05 13:51:34.246753 ressimpy-2.0.9/ResSimpy/Utils/generic_repr.py
+-rw-r--r--   0        0        0     1585 2024-03-05 13:51:34.246753 ressimpy-2.0.9/ResSimpy/Utils/invert_nexus_map.py
+-rw-r--r--   0        0        0      453 2024-03-05 13:51:34.246753 ressimpy-2.0.9/ResSimpy/Utils/obj_to_dataframe.py
+-rw-r--r--   0        0        0     1364 2024-03-05 13:51:34.246753 ressimpy-2.0.9/ResSimpy/Utils/obj_to_table_string.py
+-rw-r--r--   0        0        0     2359 2024-03-05 13:51:34.246753 ressimpy-2.0.9/ResSimpy/Utils/to_dict_generic.py
+-rw-r--r--   0        0        0      477 2024-03-05 13:51:34.246753 ressimpy-2.0.9/ResSimpy/Valve.py
+-rw-r--r--   0        0        0      479 2024-03-05 13:51:34.246753 ressimpy-2.0.9/ResSimpy/Water.py
+-rw-r--r--   0        0        0     4369 2024-03-05 13:51:34.246753 ressimpy-2.0.9/ResSimpy/Well.py
+-rw-r--r--   0        0        0     1027 2024-03-05 13:51:34.246753 ressimpy-2.0.9/ResSimpy/WellConnection.py
+-rw-r--r--   0        0        0      435 2024-03-05 13:51:34.246753 ressimpy-2.0.9/ResSimpy/WellConnections.py
+-rw-r--r--   0        0        0      474 2024-03-05 13:51:34.246753 ressimpy-2.0.9/ResSimpy/WellLists.py
+-rw-r--r--   0        0        0      755 2024-03-05 13:51:34.246753 ressimpy-2.0.9/ResSimpy/Wellbore.py
+-rw-r--r--   0        0        0      439 2024-03-05 13:51:34.246753 ressimpy-2.0.9/ResSimpy/Wellbores.py
+-rw-r--r--   0        0        0      809 2024-03-05 13:51:34.246753 ressimpy-2.0.9/ResSimpy/Wellhead.py
+-rw-r--r--   0        0        0      426 2024-03-05 13:51:34.246753 ressimpy-2.0.9/ResSimpy/Wellheads.py
+-rw-r--r--   0        0        0     3070 2024-03-05 13:51:34.246753 ressimpy-2.0.9/ResSimpy/Wells.py
+-rw-r--r--   0        0        0      289 2024-03-05 13:52:01.130866 ressimpy-2.0.9/ResSimpy/__init__.py
+-rw-r--r--   0        0        0     2741 2024-03-05 13:52:01.130866 ressimpy-2.0.9/pyproject.toml
+-rw-r--r--   0        0        0     6550 1970-01-01 00:00:00.000000 ressimpy-2.0.9/PKG-INFO
```

### Comparing `ressimpy-2.0.8/LICENSE.MD` & `ressimpy-2.0.9/LICENSE.MD`

 * *Files identical despite different names*

### Comparing `ressimpy-2.0.8/README.md` & `ressimpy-2.0.9/README.md`

 * *Files identical despite different names*

### Comparing `ressimpy-2.0.8/ResSimpy/Completion.py` & `ressimpy-2.0.9/ResSimpy/Completion.py`

 * *Files identical despite different names*

### Comparing `ressimpy-2.0.8/ResSimpy/Constraint.py` & `ressimpy-2.0.9/ResSimpy/Constraint.py`

 * *Files 10% similar despite different names*

```diff
@@ -2,15 +2,14 @@
 
 from __future__ import annotations
 from abc import ABC
 from dataclasses import dataclass
 from typing import Optional
 
 from ResSimpy.DataObjectMixin import DataObjectMixin
-from ResSimpy.Enums.ConstraintEnums import ConstraintControlMode
 from ResSimpy.Enums.UnitsEnum import UnitSystem
 from ResSimpy.Units.AttributeMappings.ConstraintUnitMapping import ConstraintUnits
 
 
 @dataclass(repr=False)
 class Constraint(DataObjectMixin, ABC):
     """Base class object for storing data related to well and node constraints."""
@@ -22,15 +21,14 @@
     max_surface_gas_rate: Optional[float] = None
     max_surface_water_rate: Optional[float] = None
     max_surface_liquid_rate: Optional[float] = None
     max_reservoir_oil_rate: Optional[float] = None
     max_reservoir_gas_rate: Optional[float] = None
     max_reservoir_water_rate: Optional[float] = None
     max_reservoir_liquid_rate: Optional[float] = None
-    control_mode: ConstraintControlMode = ConstraintControlMode.OIL_RATE
     bottom_hole_pressure: Optional[float] = None
     tubing_head_pressure: Optional[float] = None
     max_reservoir_total_fluids_rate: Optional[float] = None
 
     @property
     def units(self) -> ConstraintUnits:
         """Returns the attribute to unit map for the constraint."""
```

### Comparing `ressimpy-2.0.8/ResSimpy/Constraints.py` & `ressimpy-2.0.9/ResSimpy/Constraints.py`

 * *Files identical despite different names*

### Comparing `ressimpy-2.0.8/ResSimpy/DataObjectMixin.py` & `ressimpy-2.0.9/ResSimpy/DataObjectMixin.py`

 * *Files identical despite different names*

### Comparing `ressimpy-2.0.8/ResSimpy/DynamicProperty.py` & `ressimpy-2.0.9/ResSimpy/DynamicProperty.py`

 * *Files identical despite different names*

### Comparing `ressimpy-2.0.8/ResSimpy/File.py` & `ressimpy-2.0.9/ResSimpy/File.py`

 * *Files identical despite different names*

### Comparing `ressimpy-2.0.8/ResSimpy/FileBase.py` & `ressimpy-2.0.9/ResSimpy/FileBase.py`

 * *Files identical despite different names*

### Comparing `ressimpy-2.0.8/ResSimpy/FileOperations/file_operations.py` & `ressimpy-2.0.9/ResSimpy/FileOperations/file_operations.py`

 * *Files identical despite different names*

### Comparing `ressimpy-2.0.8/ResSimpy/Grid.py` & `ressimpy-2.0.9/ResSimpy/Grid.py`

 * *Files identical despite different names*

### Comparing `ressimpy-2.0.8/ResSimpy/ISODateTime.py` & `ressimpy-2.0.9/ResSimpy/ISODateTime.py`

 * *Files identical despite different names*

### Comparing `ressimpy-2.0.8/ResSimpy/Network.py` & `ressimpy-2.0.9/ResSimpy/Network.py`

 * *Files identical despite different names*

### Comparing `ressimpy-2.0.8/ResSimpy/Nexus/DataModels/FcsConfig.py` & `ressimpy-2.0.9/ResSimpy/Nexus/DataModels/FcsConfig.py`

 * *Files identical despite different names*

### Comparing `ressimpy-2.0.8/ResSimpy/Nexus/DataModels/FcsFile.py` & `ressimpy-2.0.9/ResSimpy/Nexus/DataModels/FcsFile.py`

 * *Files identical despite different names*

### Comparing `ressimpy-2.0.8/ResSimpy/Nexus/DataModels/Network/NexusConstraint.py` & `ressimpy-2.0.9/ResSimpy/Nexus/DataModels/Network/NexusConstraint.py`

 * *Files identical despite different names*

### Comparing `ressimpy-2.0.8/ResSimpy/Nexus/DataModels/Network/NexusConstraints.py` & `ressimpy-2.0.9/ResSimpy/Nexus/DataModels/Network/NexusConstraints.py`

 * *Files identical despite different names*

### Comparing `ressimpy-2.0.8/ResSimpy/Nexus/DataModels/Network/NexusNode.py` & `ressimpy-2.0.9/ResSimpy/Nexus/DataModels/Network/NexusNode.py`

 * *Files identical despite different names*

### Comparing `ressimpy-2.0.8/ResSimpy/Nexus/DataModels/Network/NexusNodeConnection.py` & `ressimpy-2.0.9/ResSimpy/Nexus/DataModels/Network/NexusNodeConnection.py`

 * *Files identical despite different names*

### Comparing `ressimpy-2.0.8/ResSimpy/Nexus/DataModels/Network/NexusNodeConnections.py` & `ressimpy-2.0.9/ResSimpy/Nexus/DataModels/Network/NexusNodeConnections.py`

 * *Files identical despite different names*

### Comparing `ressimpy-2.0.8/ResSimpy/Nexus/DataModels/Network/NexusNodes.py` & `ressimpy-2.0.9/ResSimpy/Nexus/DataModels/Network/NexusNodes.py`

 * *Files identical despite different names*

### Comparing `ressimpy-2.0.8/ResSimpy/Nexus/DataModels/Network/NexusProc.py` & `ressimpy-2.0.9/ResSimpy/Nexus/DataModels/Network/NexusProc.py`

 * *Files identical despite different names*

### Comparing `ressimpy-2.0.8/ResSimpy/Nexus/DataModels/Network/NexusProcs.py` & `ressimpy-2.0.9/ResSimpy/Nexus/DataModels/Network/NexusProcs.py`

 * *Files identical despite different names*

### Comparing `ressimpy-2.0.8/ResSimpy/Nexus/DataModels/Network/NexusTarget.py` & `ressimpy-2.0.9/ResSimpy/Nexus/DataModels/Network/NexusTarget.py`

 * *Files identical despite different names*

### Comparing `ressimpy-2.0.8/ResSimpy/Nexus/DataModels/Network/NexusTargets.py` & `ressimpy-2.0.9/ResSimpy/Nexus/DataModels/Network/NexusTargets.py`

 * *Files identical despite different names*

### Comparing `ressimpy-2.0.8/ResSimpy/Nexus/DataModels/Network/NexusWellConnection.py` & `ressimpy-2.0.9/ResSimpy/Nexus/DataModels/Network/NexusWellConnection.py`

 * *Files identical despite different names*

### Comparing `ressimpy-2.0.8/ResSimpy/Nexus/DataModels/Network/NexusWellConnections.py` & `ressimpy-2.0.9/ResSimpy/Nexus/DataModels/Network/NexusWellConnections.py`

 * *Files identical despite different names*

### Comparing `ressimpy-2.0.8/ResSimpy/Nexus/DataModels/Network/NexusWellLists.py` & `ressimpy-2.0.9/ResSimpy/Nexus/DataModels/Network/NexusWellLists.py`

 * *Files identical despite different names*

### Comparing `ressimpy-2.0.8/ResSimpy/Nexus/DataModels/Network/NexusWellbore.py` & `ressimpy-2.0.9/ResSimpy/Nexus/DataModels/Network/NexusWellbore.py`

 * *Files identical despite different names*

### Comparing `ressimpy-2.0.8/ResSimpy/Nexus/DataModels/Network/NexusWellbores.py` & `ressimpy-2.0.9/ResSimpy/Nexus/DataModels/Network/NexusWellbores.py`

 * *Files identical despite different names*

### Comparing `ressimpy-2.0.8/ResSimpy/Nexus/DataModels/Network/NexusWellhead.py` & `ressimpy-2.0.9/ResSimpy/Nexus/DataModels/Network/NexusWellhead.py`

 * *Files identical despite different names*

### Comparing `ressimpy-2.0.8/ResSimpy/Nexus/DataModels/Network/NexusWellheads.py` & `ressimpy-2.0.9/ResSimpy/Nexus/DataModels/Network/NexusWellheads.py`

 * *Files identical despite different names*

### Comparing `ressimpy-2.0.8/ResSimpy/Nexus/DataModels/NexusAquiferMethod.py` & `ressimpy-2.0.9/ResSimpy/Nexus/DataModels/NexusAquiferMethod.py`

 * *Files identical despite different names*

### Comparing `ressimpy-2.0.8/ResSimpy/Nexus/DataModels/NexusCompletion.py` & `ressimpy-2.0.9/ResSimpy/Nexus/DataModels/NexusCompletion.py`

 * *Files identical despite different names*

### Comparing `ressimpy-2.0.8/ResSimpy/Nexus/DataModels/NexusEquilMethod.py` & `ressimpy-2.0.9/ResSimpy/Nexus/DataModels/NexusEquilMethod.py`

 * *Files identical despite different names*

### Comparing `ressimpy-2.0.8/ResSimpy/Nexus/DataModels/NexusFile.py` & `ressimpy-2.0.9/ResSimpy/Nexus/DataModels/NexusFile.py`

 * *Files identical despite different names*

### Comparing `ressimpy-2.0.8/ResSimpy/Nexus/DataModels/NexusGasliftMethod.py` & `ressimpy-2.0.9/ResSimpy/Nexus/DataModels/NexusGasliftMethod.py`

 * *Files identical despite different names*

### Comparing `ressimpy-2.0.8/ResSimpy/Nexus/DataModels/NexusHydraulicsMethod.py` & `ressimpy-2.0.9/ResSimpy/Nexus/DataModels/NexusHydraulicsMethod.py`

 * *Files identical despite different names*

### Comparing `ressimpy-2.0.8/ResSimpy/Nexus/DataModels/NexusPVTMethod.py` & `ressimpy-2.0.9/ResSimpy/Nexus/DataModels/NexusPVTMethod.py`

 * *Files 1% similar despite different names*

```diff
@@ -9,14 +9,15 @@
 from ResSimpy.Nexus.NexusKeywords.pvt_keywords import PVT_EOS_METHODS, PVT_EOSOPTIONS_PRIMARY_WORDS
 from ResSimpy.Nexus.NexusKeywords.pvt_keywords import PVT_EOSOPTIONS_PRIMARY_KEYS_INT, PVT_TABLE_KEYWORDS
 from ResSimpy.Nexus.NexusKeywords.pvt_keywords import PVT_TABLES_WITH_ENDWORDS, PVT_TABLES_WITHOUT_ENDWORDS
 from ResSimpy.Nexus.NexusKeywords.pvt_keywords import PVT_EOSOPTIONS_PRIMARY_KEYS_FLOAT, PVT_EOSOPTIONS_TRANS_KEYS
 from ResSimpy.Nexus.NexusKeywords.pvt_keywords import PVT_EOSOPTIONS_TRANS_TEST_KEYS, PVT_EOSOPTIONS_PHASEID_KEYS
 from ResSimpy.Nexus.NexusKeywords.pvt_keywords import PVT_EOSOPTIONS_TERTIARY_KEYS, PVT_ALL_TABLE_KEYWORDS
 from ResSimpy.Nexus.NexusKeywords.pvt_keywords import PVT_UNSAT_TABLE_INDICES
+from ResSimpy.Enums.FluidTypeEnums import PvtType
 from ResSimpy.Enums.UnitsEnum import UnitSystem, SUnits, TemperatureUnits
 from ResSimpy.DynamicProperty import DynamicProperty
 from ResSimpy.Units.AttributeMappings.DynamicPropertyUnitMapping import PVTUnits
 
 from ResSimpy.Utils.factory_methods import get_empty_dict_union, get_empty_list_str, get_empty_eosopt_dict_union
 import ResSimpy.Nexus.nexus_file_operations as nfo
 import ResSimpy.FileOperations.file_operations as fo
@@ -39,29 +40,29 @@
         properties (dict[str, Union[str, int, float, Enum, list[str], pd.DataFrame,
                     dict[str, Union[float, pd.DataFrame]]]]):
             Dictionary holding all properties for a specific PVT method. Defaults to empty dictionary.
     """
 
     # General parameters
     file: NexusFile
-    pvt_type: Optional[str] = None
+    pvt_type: Optional[PvtType] = None
     eos_nhc: Optional[int] = None  # Number of hydrocarbon components
     eos_temp: Optional[float] = None  # Default temperature for EOS method
     eos_components: Optional[list[str]] = field(default_factory=get_empty_list_str)
     eos_options: dict[str, Union[
         str, int, float, pd.DataFrame, list[str], dict[str, float], tuple[str, dict[str, float]], dict[
             str, pd.DataFrame]]] \
         = field(default_factory=get_empty_eosopt_dict_union)
     properties: dict[str, Union[str, int, float, Enum, list[str],
                                 pd.DataFrame, dict[str, Union[float, pd.DataFrame]]]] \
         = field(default_factory=get_empty_dict_union)
     unit_system: UnitSystem
 
     def __init__(self, file: NexusFile, input_number: int, model_unit_system: UnitSystem,
-                 pvt_type: Optional[str] = None,
+                 pvt_type: Optional[PvtType] = None,
                  eos_nhc: Optional[int] = None, eos_temp: Optional[float] = None,
                  eos_components: Optional[list[str]] = None,
                  eos_options: Optional[dict[str, Union[str, int, float, pd.DataFrame, list[str], dict[str, float],
                                        tuple[str, dict[str, float]], dict[str, pd.DataFrame]]]] = None,
                  properties: Optional[dict[str, Union[str, int, float, Enum, list[str], pd.DataFrame,
                                       dict[str, Union[float, pd.DataFrame]]]]] = None) -> None:
         if pvt_type is not None:
@@ -133,15 +134,15 @@
         printable_str = ''
         pvt_dict = self.properties
         # Print description if present
         if 'DESC' in pvt_dict.keys() and isinstance(pvt_dict['DESC'], list):
             for desc_line in pvt_dict['DESC']:
                 printable_str += 'DESC ' + desc_line + '\n'
         # Print PVT type and associated properties
-        printable_str += f'{self.pvt_type}'
+        printable_str += '' if self.pvt_type is None else f'{self.pvt_type.value}'
         if self.eos_nhc is not None:
             printable_str += f' NHC {self.eos_nhc}'
         for pvt_key in PVT_BLACKOIL_PRIMARY_KEYWORDS:
             if pvt_key in pvt_dict.keys():
                 printable_str += f' {pvt_key} {pvt_dict[pvt_key]}'
         printable_str += '\n'
         if 'DRYGAS_MFP' in pvt_dict.keys():
@@ -368,15 +369,15 @@
 
         line_indx = 0
         for line in file_as_list:
 
             # Determine PVT type, i.e., BLACKOIL, WATEROIL, EOS, etc.
             for pvt_type in PVT_TYPE_KEYWORDS:
                 if nfo.check_token(pvt_type, line):
-                    self.pvt_type = pvt_type
+                    self.pvt_type = PvtType[pvt_type]
 
             # Extract blackoil fluid density parameters
             for fluid_param in PVT_BLACKOIL_PRIMARY_KEYWORDS:
                 if nfo.check_token(fluid_param, line):
                     self.properties[fluid_param] = float(nfo.get_expected_token_value(
                         fluid_param, line, file_as_list, custom_message=f"Property {fluid_param} does \
                         not have a numerical value."))
```

### Comparing `ressimpy-2.0.8/ResSimpy/Nexus/DataModels/NexusRelPermEndPoint.py` & `ressimpy-2.0.9/ResSimpy/Nexus/DataModels/NexusRelPermEndPoint.py`

 * *Files identical despite different names*

### Comparing `ressimpy-2.0.8/ResSimpy/Nexus/DataModels/NexusRelPermMethod.py` & `ressimpy-2.0.9/ResSimpy/Nexus/DataModels/NexusRelPermMethod.py`

 * *Files identical despite different names*

### Comparing `ressimpy-2.0.8/ResSimpy/Nexus/DataModels/NexusRockMethod.py` & `ressimpy-2.0.9/ResSimpy/Nexus/DataModels/NexusRockMethod.py`

 * *Files identical despite different names*

### Comparing `ressimpy-2.0.8/ResSimpy/Nexus/DataModels/NexusSeparatorMethod.py` & `ressimpy-2.0.9/ResSimpy/Nexus/DataModels/NexusSeparatorMethod.py`

 * *Files 7% similar despite different names*

```diff
@@ -8,14 +8,15 @@
 from ResSimpy.Utils.factory_methods import get_empty_dict_union
 import ResSimpy.Nexus.nexus_file_operations as nfo
 from ResSimpy.Nexus.NexusKeywords.separator_keywords import SEPARATOR_KEYS_INT, SEPARATOR_KEYS_FLOAT
 from ResSimpy.Nexus.NexusKeywords.separator_keywords import SEPARATOR_KEYWORDS
 from ResSimpy.DynamicProperty import DynamicProperty
 from ResSimpy.Units.AttributeMappings.DynamicPropertyUnitMapping import SeparatorUnits
 from ResSimpy.Enums.UnitsEnum import UnitSystem, SUnits, TemperatureUnits
+from ResSimpy.Enums.FluidTypeEnums import SeparatorType
 
 
 @dataclass(kw_only=True, repr=False)  # Doesn't need to write an _init_, _eq_ methods, etc.
 class NexusSeparatorMethod(DynamicProperty):
     """Class to hold data input for a Nexus Separator method.
 
     Attributes:
@@ -24,22 +25,22 @@
         separator_type (Optional[str]): Type of separator method, e.g., BLACKOIL, GASPLANT or EOS. Defaults to None
         properties (dict[str, Union[str, int, float, Enum, list[str], pd.DataFrame,
                     dict[str, Union[float, pd.DataFrame]]]]):
             Dictionary holding all properties for a specific separator method. Defaults to empty dictionary.
     """
 
     file: NexusFile
-    separator_type: Optional[str] = None
+    separator_type: Optional[SeparatorType] = None
     properties: dict[str, Union[str, int, float, Enum, list[str],
                      pd.DataFrame, dict[str, Union[float, pd.DataFrame]]]] \
         = field(default_factory=get_empty_dict_union)
     unit_system: UnitSystem
 
     def __init__(self, file: NexusFile, input_number: int, model_unit_system: UnitSystem,
-                 separator_type: Optional[str] = None,
+                 separator_type: Optional[SeparatorType] = None,
                  properties: Optional[dict[str, Union[str, int, float, Enum, list[str], pd.DataFrame,
                                       dict[str, Union[float, pd.DataFrame]]]]] = None) -> None:
         if separator_type is not None:
             self.separator_type = separator_type
         if properties is not None:
             self.properties = properties
         else:
@@ -71,18 +72,18 @@
         printable_str = ''
         sep_dict = self.properties
         for key, value in sep_dict.items():
             if key == 'DESC' and isinstance(value, list):
                 for desc_line in value:
                     printable_str += 'DESC ' + desc_line + '\n'
             elif key == 'SEPARATOR_TABLE' and isinstance(value, pd.DataFrame):
-                if self.separator_type == 'GASPLANT':
+                if self.separator_type == SeparatorType.GASPLANT:
                     printable_str += 'RECFAC_TABLE\n'
                 printable_str += value.to_string(na_rep='', index=False) + '\n'
-                if self.separator_type == 'GASPLANT':
+                if self.separator_type == SeparatorType.GASPLANT:
                     printable_str += 'ENDRECFAC_TABLE\n'
                 printable_str += '\n'
             elif isinstance(value, Enum):
                 if isinstance(value, UnitSystem) or isinstance(value, TemperatureUnits):
                     printable_str += f'{value.value}\n'
                 elif isinstance(value, SUnits):
                     printable_str += f'SUNITS {value.value}\n'
@@ -112,29 +113,29 @@
         start_reading_table: bool = False
 
         line_indx = 0
         for line in file_as_list:
 
             # Determine separator type, i.e., EOS multistage, gas plant data or black oil
             if nfo.check_token('TEMP', line):  # EOS multistage separator table
-                self.separator_type = 'EOS'
+                self.separator_type = SeparatorType.EOS
                 sep_table_indices[0] = line_indx  # Specify EOS multistage separator table starting index
                 start_reading_table = True
                 line_indx += 1
                 continue
             elif nfo.check_token('KEYCPTLIST', line):  # Gas plant data
-                self.separator_type = 'GASPLANT'
+                self.separator_type = SeparatorType.GASPLANT
                 elems = line.split('!')[0].split()
                 cpt_index = elems.index('KEYCPTLIST')
                 if 'KEYCPTLIST' not in self.properties.keys():
                     self.properties['KEYCPTLIST'] = elems[cpt_index + 1:]
                 line_indx += 1
                 continue
             elif nfo.check_token('BOSEP', line):  # Black oil separator table
-                self.separator_type = 'BLACKOIL'
+                self.separator_type = SeparatorType.BLACKOIL
                 self.properties['BOSEP'] = ''
                 line_indx += 1
                 continue
 
             # Find SEPARATOR key-value pairs, such as WATERMETHOD 1 or PRES_STD 14.7
             if [i for i in line.split() if i in SEPARATOR_KEYS_FLOAT]:
                 for key in SEPARATOR_KEYS_FLOAT:
@@ -142,32 +143,32 @@
                         self.properties[key] = float(nfo.get_expected_token_value(key, line, file_as_list))
             if [i for i in line.split() if i in SEPARATOR_KEYS_INT]:
                 for key in SEPARATOR_KEYS_INT:
                     if nfo.check_token(key, line):
                         self.properties[key] = int(nfo.get_expected_token_value(key, line, file_as_list))
 
             # Find starting index for black oil separator table
-            if self.separator_type == 'BLACKOIL':
+            if self.separator_type == SeparatorType.BLACKOIL:
                 if nfo.check_token('KVOIL', line):
                     sep_table_indices[0] = line_indx
                     start_reading_table = True
                     line_indx += 1
                     continue
 
             # Find ending index for EOS multistage and black oil separator tables
             if start_reading_table:
-                if self.separator_type in ['EOS', 'BLACKOIL']:
+                if self.separator_type in [SeparatorType.EOS, SeparatorType.BLACKOIL]:
                     for keyword in SEPARATOR_KEYWORDS:
                         if nfo.check_token(keyword, line):
                             sep_table_indices[1] = line_indx
                             start_reading_table = False
                             break
 
             # Find starting and ending indices for gas plant separator table
-            if self.separator_type == 'GASPLANT':
+            if self.separator_type == SeparatorType.GASPLANT:
                 if nfo.check_token('RECFAC_TABLE', line):
                     sep_table_indices[0] = line_indx + 1
                     start_reading_table = True
                 if nfo.check_token('ENDRECFAC_TABLE', line):
                     sep_table_indices[1] = line_indx
                     start_reading_table = False
```

### Comparing `ressimpy-2.0.8/ResSimpy/Nexus/DataModels/NexusSolverParameter.py` & `ressimpy-2.0.9/ResSimpy/Nexus/DataModels/NexusSolverParameter.py`

 * *Files identical despite different names*

### Comparing `ressimpy-2.0.8/ResSimpy/Nexus/DataModels/NexusValveMethod.py` & `ressimpy-2.0.9/ResSimpy/Nexus/DataModels/NexusValveMethod.py`

 * *Files identical despite different names*

### Comparing `ressimpy-2.0.8/ResSimpy/Nexus/DataModels/NexusWaterMethod.py` & `ressimpy-2.0.9/ResSimpy/Nexus/DataModels/NexusWaterMethod.py`

 * *Files identical despite different names*

### Comparing `ressimpy-2.0.8/ResSimpy/Nexus/DataModels/NexusWell.py` & `ressimpy-2.0.9/ResSimpy/Nexus/DataModels/NexusWell.py`

 * *Files identical despite different names*

### Comparing `ressimpy-2.0.8/ResSimpy/Nexus/DataModels/NexusWellList.py` & `ressimpy-2.0.9/ResSimpy/Nexus/DataModels/NexusWellList.py`

 * *Files identical despite different names*

### Comparing `ressimpy-2.0.8/ResSimpy/Nexus/DataModels/NexusWellMod.py` & `ressimpy-2.0.9/ResSimpy/Nexus/DataModels/NexusWellMod.py`

 * *Files identical despite different names*

### Comparing `ressimpy-2.0.8/ResSimpy/Nexus/DataModels/StructuredGrid/NexusGrid.py` & `ressimpy-2.0.9/ResSimpy/Nexus/DataModels/StructuredGrid/NexusGrid.py`

 * *Files identical despite different names*

### Comparing `ressimpy-2.0.8/ResSimpy/Nexus/NexusAquiferMethods.py` & `ressimpy-2.0.9/ResSimpy/Nexus/NexusAquiferMethods.py`

 * *Files identical despite different names*

### Comparing `ressimpy-2.0.8/ResSimpy/Nexus/NexusEquilMethods.py` & `ressimpy-2.0.9/ResSimpy/Nexus/NexusEquilMethods.py`

 * *Files identical despite different names*

### Comparing `ressimpy-2.0.8/ResSimpy/Nexus/NexusGasliftMethods.py` & `ressimpy-2.0.9/ResSimpy/Nexus/NexusGasliftMethods.py`

 * *Files identical despite different names*

### Comparing `ressimpy-2.0.8/ResSimpy/Nexus/NexusHydraulicsMethods.py` & `ressimpy-2.0.9/ResSimpy/Nexus/NexusHydraulicsMethods.py`

 * *Files identical despite different names*

### Comparing `ressimpy-2.0.8/ResSimpy/Nexus/NexusKeywords/aquifer_keywords.py` & `ressimpy-2.0.9/ResSimpy/Nexus/NexusKeywords/aquifer_keywords.py`

 * *Files identical despite different names*

### Comparing `ressimpy-2.0.8/ResSimpy/Nexus/NexusKeywords/equil_keywords.py` & `ressimpy-2.0.9/ResSimpy/Nexus/NexusKeywords/equil_keywords.py`

 * *Files identical despite different names*

### Comparing `ressimpy-2.0.8/ResSimpy/Nexus/NexusKeywords/fcs_keywords.py` & `ressimpy-2.0.9/ResSimpy/Nexus/NexusKeywords/fcs_keywords.py`

 * *Files identical despite different names*

### Comparing `ressimpy-2.0.8/ResSimpy/Nexus/NexusKeywords/hyd_keywords.py` & `ressimpy-2.0.9/ResSimpy/Nexus/NexusKeywords/hyd_keywords.py`

 * *Files identical despite different names*

### Comparing `ressimpy-2.0.8/ResSimpy/Nexus/NexusKeywords/nexus_keywords.py` & `ressimpy-2.0.9/ResSimpy/Nexus/NexusKeywords/nexus_keywords.py`

 * *Files identical despite different names*

### Comparing `ressimpy-2.0.8/ResSimpy/Nexus/NexusKeywords/options_keywords.py` & `ressimpy-2.0.9/ResSimpy/Nexus/NexusKeywords/options_keywords.py`

 * *Files identical despite different names*

### Comparing `ressimpy-2.0.8/ResSimpy/Nexus/NexusKeywords/proc_keywords.py` & `ressimpy-2.0.9/ResSimpy/Nexus/NexusKeywords/proc_keywords.py`

 * *Files identical despite different names*

### Comparing `ressimpy-2.0.8/ResSimpy/Nexus/NexusKeywords/pvt_keywords.py` & `ressimpy-2.0.9/ResSimpy/Nexus/NexusKeywords/pvt_keywords.py`

 * *Files identical despite different names*

### Comparing `ressimpy-2.0.8/ResSimpy/Nexus/NexusKeywords/relpm_keywords.py` & `ressimpy-2.0.9/ResSimpy/Nexus/NexusKeywords/relpm_keywords.py`

 * *Files identical despite different names*

### Comparing `ressimpy-2.0.8/ResSimpy/Nexus/NexusKeywords/rock_keywords.py` & `ressimpy-2.0.9/ResSimpy/Nexus/NexusKeywords/rock_keywords.py`

 * *Files identical despite different names*

### Comparing `ressimpy-2.0.8/ResSimpy/Nexus/NexusKeywords/runcontrol_keywords.py` & `ressimpy-2.0.9/ResSimpy/Nexus/NexusKeywords/runcontrol_keywords.py`

 * *Files identical despite different names*

### Comparing `ressimpy-2.0.8/ResSimpy/Nexus/NexusKeywords/separator_keywords.py` & `ressimpy-2.0.9/ResSimpy/Nexus/NexusKeywords/separator_keywords.py`

 * *Files identical despite different names*

### Comparing `ressimpy-2.0.8/ResSimpy/Nexus/NexusKeywords/structured_grid_keywords.py` & `ressimpy-2.0.9/ResSimpy/Nexus/NexusKeywords/structured_grid_keywords.py`

 * *Files identical despite different names*

### Comparing `ressimpy-2.0.8/ResSimpy/Nexus/NexusKeywords/surface_keywords.py` & `ressimpy-2.0.9/ResSimpy/Nexus/NexusKeywords/surface_keywords.py`

 * *Files identical despite different names*

### Comparing `ressimpy-2.0.8/ResSimpy/Nexus/NexusKeywords/wells_keywords.py` & `ressimpy-2.0.9/ResSimpy/Nexus/NexusKeywords/wells_keywords.py`

 * *Files identical despite different names*

### Comparing `ressimpy-2.0.8/ResSimpy/Nexus/NexusNetwork.py` & `ressimpy-2.0.9/ResSimpy/Nexus/NexusNetwork.py`

 * *Files identical despite different names*

### Comparing `ressimpy-2.0.8/ResSimpy/Nexus/NexusPVTMethods.py` & `ressimpy-2.0.9/ResSimpy/Nexus/NexusPVTMethods.py`

 * *Files identical despite different names*

### Comparing `ressimpy-2.0.8/ResSimpy/Nexus/NexusRelPermMethods.py` & `ressimpy-2.0.9/ResSimpy/Nexus/NexusRelPermMethods.py`

 * *Files identical despite different names*

### Comparing `ressimpy-2.0.8/ResSimpy/Nexus/NexusReporting.py` & `ressimpy-2.0.9/ResSimpy/Nexus/NexusReporting.py`

 * *Files identical despite different names*

### Comparing `ressimpy-2.0.8/ResSimpy/Nexus/NexusRockMethods.py` & `ressimpy-2.0.9/ResSimpy/Nexus/NexusRockMethods.py`

 * *Files identical despite different names*

### Comparing `ressimpy-2.0.8/ResSimpy/Nexus/NexusSeparatorMethods.py` & `ressimpy-2.0.9/ResSimpy/Nexus/NexusSeparatorMethods.py`

 * *Files 2% similar despite different names*

```diff
@@ -42,15 +42,16 @@
         if not self.__properties_loaded:
             self.load_separator_methods()
         printable_str = ''
         for table_num in self.__inputs.keys():
             printable_str += '\n--------------------------------\n'
             printable_str += f'SEPARATOR method {table_num}\n'
             printable_str += '--------------------------------\n'
-            printable_str += f'\nSEPARATOR_TYPE: {self.__inputs[table_num].separator_type}\n'
+            sep_type = self.__inputs[table_num].separator_type
+            printable_str += f"\nSEPARATOR_TYPE: {'' if sep_type is None else sep_type.value}\n"
             printable_str += self.__inputs[table_num].__repr__()
             printable_str += '\n'
 
         return printable_str
 
     @property
     def inputs(self) -> MutableMapping[int, NexusSeparatorMethod]:
```

### Comparing `ressimpy-2.0.8/ResSimpy/Nexus/NexusSimulator.py` & `ressimpy-2.0.9/ResSimpy/Nexus/NexusSimulator.py`

 * *Files identical despite different names*

### Comparing `ressimpy-2.0.8/ResSimpy/Nexus/NexusSolverParameters.py` & `ressimpy-2.0.9/ResSimpy/Nexus/NexusSolverParameters.py`

 * *Files identical despite different names*

### Comparing `ressimpy-2.0.8/ResSimpy/Nexus/NexusValveMethods.py` & `ressimpy-2.0.9/ResSimpy/Nexus/NexusValveMethods.py`

 * *Files identical despite different names*

### Comparing `ressimpy-2.0.8/ResSimpy/Nexus/NexusWaterMethods.py` & `ressimpy-2.0.9/ResSimpy/Nexus/NexusWaterMethods.py`

 * *Files identical despite different names*

### Comparing `ressimpy-2.0.8/ResSimpy/Nexus/NexusWells.py` & `ressimpy-2.0.9/ResSimpy/Nexus/NexusWells.py`

 * *Files identical despite different names*

### Comparing `ressimpy-2.0.8/ResSimpy/Nexus/array_function_operations.py` & `ressimpy-2.0.9/ResSimpy/Nexus/array_function_operations.py`

 * *Files identical despite different names*

### Comparing `ressimpy-2.0.8/ResSimpy/Nexus/load_wells.py` & `ressimpy-2.0.9/ResSimpy/Nexus/load_wells.py`

 * *Files identical despite different names*

### Comparing `ressimpy-2.0.8/ResSimpy/Nexus/logfile_operations.py` & `ressimpy-2.0.9/ResSimpy/Nexus/logfile_operations.py`

 * *Files identical despite different names*

### Comparing `ressimpy-2.0.8/ResSimpy/Nexus/nexus_add_new_object_to_file.py` & `ressimpy-2.0.9/ResSimpy/Nexus/nexus_add_new_object_to_file.py`

 * *Files identical despite different names*

### Comparing `ressimpy-2.0.8/ResSimpy/Nexus/nexus_collect_tables.py` & `ressimpy-2.0.9/ResSimpy/Nexus/nexus_collect_tables.py`

 * *Files 1% similar despite different names*

```diff
@@ -2,15 +2,15 @@
 from __future__ import annotations
 
 from typing import Any, Optional
 
 from ResSimpy.File import File
 from ResSimpy.Nexus.DataModels.Network.NexusConstraint import NexusConstraint
 from ResSimpy.Enums.UnitsEnum import UnitSystem
-from ResSimpy.Nexus.nexus_constraint_operations import load_inline_constraints, update_constraint_control_mode
+from ResSimpy.Nexus.nexus_constraint_operations import load_inline_constraints
 from ResSimpy.Nexus.nexus_file_operations import check_property_in_line, check_token, get_expected_token_value, \
     check_list_tokens, load_table_to_objects
 from ResSimpy.Nexus.nexus_load_well_list import load_well_lists
 
 
 # TODO refactor the collection of tables to an object with proper typing
 def collect_all_tables_to_objects(nexus_file: File, table_object_map: dict[str, Any], start_date: Optional[str],
@@ -121,15 +121,14 @@
             # This statement ensures that CONSTRAINT that are found in tables are actually added to the dictionary
             # under the same key as constraints to preserve their order
             if (token_found == 'CONSTRAINT' or token_found == 'QMULT') and list_objects is not None:
                 for constraint, id_index in list_objects:
                     if isinstance(constraint, NexusConstraint):
                         obj_id = constraint.id
                         well_name = constraint.name
-                        update_constraint_control_mode(constraint)
                     else:
                         obj_id = constraint
                         well_name = None
                     correct_line_index = id_index + table_start
                     nexus_file.add_object_locations(obj_id, [correct_line_index])
                     if well_name is None:
                         continue
```

### Comparing `ressimpy-2.0.8/ResSimpy/Nexus/nexus_file_operations.py` & `ressimpy-2.0.9/ResSimpy/Nexus/nexus_file_operations.py`

 * *Files identical despite different names*

### Comparing `ressimpy-2.0.8/ResSimpy/Nexus/nexus_load_well_list.py` & `ressimpy-2.0.9/ResSimpy/Nexus/nexus_load_well_list.py`

 * *Files identical despite different names*

### Comparing `ressimpy-2.0.8/ResSimpy/Nexus/nexus_modify_object_in_file.py` & `ressimpy-2.0.9/ResSimpy/Nexus/nexus_modify_object_in_file.py`

 * *Files identical despite different names*

### Comparing `ressimpy-2.0.8/ResSimpy/Nexus/nexus_remove_object_from_file.py` & `ressimpy-2.0.9/ResSimpy/Nexus/nexus_remove_object_from_file.py`

 * *Files identical despite different names*

### Comparing `ressimpy-2.0.8/ResSimpy/Nexus/rel_perm_operations.py` & `ressimpy-2.0.9/ResSimpy/Nexus/rel_perm_operations.py`

 * *Files identical despite different names*

### Comparing `ressimpy-2.0.8/ResSimpy/Nexus/runcontrol_operations.py` & `ressimpy-2.0.9/ResSimpy/Nexus/runcontrol_operations.py`

 * *Files identical despite different names*

### Comparing `ressimpy-2.0.8/ResSimpy/Nexus/structured_grid_operations.py` & `ressimpy-2.0.9/ResSimpy/Nexus/structured_grid_operations.py`

 * *Files identical despite different names*

### Comparing `ressimpy-2.0.8/ResSimpy/Node.py` & `ressimpy-2.0.9/ResSimpy/Node.py`

 * *Files identical despite different names*

### Comparing `ressimpy-2.0.8/ResSimpy/NodeConnection.py` & `ressimpy-2.0.9/ResSimpy/NodeConnection.py`

 * *Files identical despite different names*

### Comparing `ressimpy-2.0.8/ResSimpy/OpenGoSim/DataModels/OpenGoSimCompletion.py` & `ressimpy-2.0.9/ResSimpy/OpenGoSim/DataModels/OpenGoSimCompletion.py`

 * *Files identical despite different names*

### Comparing `ressimpy-2.0.8/ResSimpy/OpenGoSim/DataModels/OpenGoSimWell.py` & `ressimpy-2.0.9/ResSimpy/OpenGoSim/DataModels/OpenGoSimWell.py`

 * *Files identical despite different names*

### Comparing `ressimpy-2.0.8/ResSimpy/OpenGoSim/Model_Parts/OpenGoSimNetwork.py` & `ressimpy-2.0.9/ResSimpy/OpenGoSim/Model_Parts/OpenGoSimNetwork.py`

 * *Files identical despite different names*

### Comparing `ressimpy-2.0.8/ResSimpy/OpenGoSim/OpenGoSimKeywords/OpenGoSimKeywords.py` & `ressimpy-2.0.9/ResSimpy/OpenGoSim/OpenGoSimKeywords/OpenGoSimKeywords.py`

 * *Files identical despite different names*

### Comparing `ressimpy-2.0.8/ResSimpy/OpenGoSim/OpenGoSimSimulator.py` & `ressimpy-2.0.9/ResSimpy/OpenGoSim/OpenGoSimSimulator.py`

 * *Files identical despite different names*

### Comparing `ressimpy-2.0.8/ResSimpy/OperationsMixin.py` & `ressimpy-2.0.9/ResSimpy/OperationsMixin.py`

 * *Files identical despite different names*

### Comparing `ressimpy-2.0.8/ResSimpy/RelPermEndPoint.py` & `ressimpy-2.0.9/ResSimpy/RelPermEndPoint.py`

 * *Files identical despite different names*

### Comparing `ressimpy-2.0.8/ResSimpy/Simulator.py` & `ressimpy-2.0.9/ResSimpy/Simulator.py`

 * *Files identical despite different names*

### Comparing `ressimpy-2.0.8/ResSimpy/SolverParameters.py` & `ressimpy-2.0.9/ResSimpy/SolverParameters.py`

 * *Files identical despite different names*

### Comparing `ressimpy-2.0.8/ResSimpy/Target.py` & `ressimpy-2.0.9/ResSimpy/Target.py`

 * *Files identical despite different names*

### Comparing `ressimpy-2.0.8/ResSimpy/Units/AttributeMapping.py` & `ressimpy-2.0.9/ResSimpy/Units/AttributeMapping.py`

 * *Files identical despite different names*

### Comparing `ressimpy-2.0.8/ResSimpy/Units/AttributeMappings/BaseUnitMapping.py` & `ressimpy-2.0.9/ResSimpy/Units/AttributeMappings/BaseUnitMapping.py`

 * *Files identical despite different names*

### Comparing `ressimpy-2.0.8/ResSimpy/Units/AttributeMappings/CompletionUnitMapping.py` & `ressimpy-2.0.9/ResSimpy/Units/AttributeMappings/CompletionUnitMapping.py`

 * *Files identical despite different names*

### Comparing `ressimpy-2.0.8/ResSimpy/Units/AttributeMappings/ConstraintUnitMapping.py` & `ressimpy-2.0.9/ResSimpy/Units/AttributeMappings/ConstraintUnitMapping.py`

 * *Files identical despite different names*

### Comparing `ressimpy-2.0.8/ResSimpy/Units/AttributeMappings/DynamicPropertyUnitMapping.py` & `ressimpy-2.0.9/ResSimpy/Units/AttributeMappings/DynamicPropertyUnitMapping.py`

 * *Files identical despite different names*

### Comparing `ressimpy-2.0.8/ResSimpy/Units/AttributeMappings/NetworkUnitMapping.py` & `ressimpy-2.0.9/ResSimpy/Units/AttributeMappings/NetworkUnitMapping.py`

 * *Files identical despite different names*

### Comparing `ressimpy-2.0.8/ResSimpy/Units/Units.py` & `ressimpy-2.0.9/ResSimpy/Units/Units.py`

 * *Files identical despite different names*

### Comparing `ressimpy-2.0.8/ResSimpy/Utils/factory_methods.py` & `ressimpy-2.0.9/ResSimpy/Utils/factory_methods.py`

 * *Files identical despite different names*

### Comparing `ressimpy-2.0.8/ResSimpy/Utils/generic_repr.py` & `ressimpy-2.0.9/ResSimpy/Utils/generic_repr.py`

 * *Files identical despite different names*

### Comparing `ressimpy-2.0.8/ResSimpy/Utils/invert_nexus_map.py` & `ressimpy-2.0.9/ResSimpy/Utils/invert_nexus_map.py`

 * *Files identical despite different names*

### Comparing `ressimpy-2.0.8/ResSimpy/Utils/obj_to_table_string.py` & `ressimpy-2.0.9/ResSimpy/Utils/obj_to_table_string.py`

 * *Files identical despite different names*

### Comparing `ressimpy-2.0.8/ResSimpy/Utils/to_dict_generic.py` & `ressimpy-2.0.9/ResSimpy/Utils/to_dict_generic.py`

 * *Files identical despite different names*

### Comparing `ressimpy-2.0.8/ResSimpy/Well.py` & `ressimpy-2.0.9/ResSimpy/Well.py`

 * *Files identical despite different names*

### Comparing `ressimpy-2.0.8/ResSimpy/WellConnection.py` & `ressimpy-2.0.9/ResSimpy/WellConnection.py`

 * *Files identical despite different names*

### Comparing `ressimpy-2.0.8/ResSimpy/Wellbore.py` & `ressimpy-2.0.9/ResSimpy/Wellbore.py`

 * *Files identical despite different names*

### Comparing `ressimpy-2.0.8/ResSimpy/Wellhead.py` & `ressimpy-2.0.9/ResSimpy/Wellhead.py`

 * *Files identical despite different names*

### Comparing `ressimpy-2.0.8/ResSimpy/Wells.py` & `ressimpy-2.0.9/ResSimpy/Wells.py`

 * *Files identical despite different names*

### Comparing `ressimpy-2.0.8/pyproject.toml` & `ressimpy-2.0.9/pyproject.toml`

 * *Files 0% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 [tool.poetry]
 name = "ResSimpy"
-version = "2.0.8" # Set at build time
+version = "2.0.9" # Set at build time
 description = "A Python library for working with Reservoir Simulator Models."
 authors = ["BP"]
 readme = "README.md"
 license = "Apache-2.0"
 keywords = ["ResSimpy", "Reservoir Engineering"]
 classifiers = [
     "Operating System :: OS Independent",
```

### Comparing `ressimpy-2.0.8/PKG-INFO` & `ressimpy-2.0.9/PKG-INFO`

 * *Files 0% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: ResSimpy
-Version: 2.0.8
+Version: 2.0.9
 Summary: A Python library for working with Reservoir Simulator Models.
 License: Apache-2.0
 Keywords: ResSimpy,Reservoir Engineering
 Author: BP
 Requires-Python: >=3.10,<3.12
 Classifier: Development Status :: 5 - Production/Stable
 Classifier: License :: OSI Approved :: Apache Software License
```

