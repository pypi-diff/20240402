# Comparing `tmp/simpa-0.9.0.tar.gz` & `tmp/simpa-0.9.1.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "simpa-0.9.0.tar", max compression
+gzip compressed data, was "simpa-0.9.1.tar", max compression
```

## Comparing `simpa-0.9.0.tar` & `simpa-0.9.1.tar`

### file list

```diff
@@ -1,189 +1,189 @@
--rw-r--r--   0        0        0      236 2024-03-14 09:18:47.907300 simpa-0.9.0/LICENSE.md
-drwxr-xr-x   0        0        0        0 2024-03-14 09:18:47.907300 simpa-0.9.0/LICENSES/
--rw-r--r--   0        0        0     1144 2024-03-14 09:18:47.907300 simpa-0.9.0/LICENSES/MIT
--rwxr-xr-x   0        0        0    10700 2024-03-14 09:18:47.907300 simpa-0.9.0/README.md
--rw-r--r--   0        0        0     2049 2024-03-14 09:18:47.911300 simpa-0.9.0/pyproject.toml
--rw-r--r--   0        0        0     3314 2024-03-14 09:18:47.911300 simpa-0.9.0/simpa/__init__.py
--rw-r--r--   0        0        0      968 2024-03-14 09:18:47.911300 simpa-0.9.0/simpa/core/__init__.py
--rw-r--r--   0        0        0     1548 2024-03-14 09:18:47.911300 simpa-0.9.0/simpa/core/device_digital_twins/__init__.py
--rw-r--r--   0        0        0      152 2024-03-14 09:18:47.911300 simpa-0.9.0/simpa/core/device_digital_twins/detection_geometries/__init__.py
--rw-r--r--   0        0        0     5496 2024-03-14 09:18:47.911300 simpa-0.9.0/simpa/core/device_digital_twins/detection_geometries/curved_array.py
--rw-r--r--   0        0        0     6117 2024-03-14 09:18:47.911300 simpa-0.9.0/simpa/core/device_digital_twins/detection_geometries/detection_geometry_base.py
--rw-r--r--   0        0        0     4518 2024-03-14 09:18:47.911300 simpa-0.9.0/simpa/core/device_digital_twins/detection_geometries/linear_array.py
--rw-r--r--   0        0        0     5481 2024-03-14 09:18:47.911300 simpa-0.9.0/simpa/core/device_digital_twins/detection_geometries/planar_array.py
--rw-r--r--   0        0        0    13839 2024-03-14 09:18:47.911300 simpa-0.9.0/simpa/core/device_digital_twins/digital_device_twin_base.py
--rw-r--r--   0        0        0      152 2024-03-14 09:18:47.911300 simpa-0.9.0/simpa/core/device_digital_twins/illumination_geometries/__init__.py
--rw-r--r--   0        0        0     2558 2024-03-14 09:18:47.911300 simpa-0.9.0/simpa/core/device_digital_twins/illumination_geometries/disk_illumination.py
--rw-r--r--   0        0        0     3492 2024-03-14 09:18:47.911300 simpa-0.9.0/simpa/core/device_digital_twins/illumination_geometries/gaussian_beam_illumination.py
--rw-r--r--   0        0        0     2987 2024-03-14 09:18:47.911300 simpa-0.9.0/simpa/core/device_digital_twins/illumination_geometries/illumination_geometry_base.py
--rw-r--r--   0        0        0     2832 2024-03-14 09:18:47.911300 simpa-0.9.0/simpa/core/device_digital_twins/illumination_geometries/ithera_msot_acuity_illumination.py
--rw-r--r--   0        0        0     3420 2024-03-14 09:18:47.911300 simpa-0.9.0/simpa/core/device_digital_twins/illumination_geometries/ithera_msot_invision_illumination.py
--rw-r--r--   0        0        0     3246 2024-03-14 09:18:47.911300 simpa-0.9.0/simpa/core/device_digital_twins/illumination_geometries/pencil_array_illumination.py
--rw-r--r--   0        0        0     1515 2024-03-14 09:18:47.911300 simpa-0.9.0/simpa/core/device_digital_twins/illumination_geometries/pencil_beam_illumination.py
--rw-r--r--   0        0        0     3521 2024-03-14 09:18:47.911300 simpa-0.9.0/simpa/core/device_digital_twins/illumination_geometries/slit_illumination.py
--rw-r--r--   0        0        0      152 2024-03-14 09:18:47.911300 simpa-0.9.0/simpa/core/device_digital_twins/pa_devices/__init__.py
--rw-r--r--   0        0        0    12456 2024-03-14 09:18:47.911300 simpa-0.9.0/simpa/core/device_digital_twins/pa_devices/ithera_msot_acuity.py
--rw-r--r--   0        0        0     3730 2024-03-14 09:18:47.911300 simpa-0.9.0/simpa/core/device_digital_twins/pa_devices/ithera_msot_invision.py
--rw-r--r--   0        0        0     4931 2024-03-14 09:18:47.911300 simpa-0.9.0/simpa/core/device_digital_twins/pa_devices/ithera_rsom.py
--rw-r--r--   0        0        0      895 2024-03-14 09:18:47.915300 simpa-0.9.0/simpa/core/processing_components/__init__.py
--rw-r--r--   0        0        0      152 2024-03-14 09:18:47.915300 simpa-0.9.0/simpa/core/processing_components/monospectral/__init__.py
--rw-r--r--   0        0        0     5528 2024-03-14 09:18:47.915300 simpa-0.9.0/simpa/core/processing_components/monospectral/field_of_view_cropping.py
--rw-r--r--   0        0        0    27651 2024-03-14 09:18:47.915300 simpa-0.9.0/simpa/core/processing_components/monospectral/iterative_qPAI_algorithm.py
--rw-r--r--   0        0        0      365 2024-03-14 09:18:47.915300 simpa-0.9.0/simpa/core/processing_components/monospectral/noise/__init__.py
--rw-r--r--   0        0        0     2895 2024-03-14 09:18:47.915300 simpa-0.9.0/simpa/core/processing_components/monospectral/noise/gamma_noise.py
--rw-r--r--   0        0        0     3320 2024-03-14 09:18:47.915300 simpa-0.9.0/simpa/core/processing_components/monospectral/noise/gaussian_noise.py
--rw-r--r--   0        0        0     2543 2024-03-14 09:18:47.915300 simpa-0.9.0/simpa/core/processing_components/monospectral/noise/poisson_noise.py
--rw-r--r--   0        0        0     3207 2024-03-14 09:18:47.915300 simpa-0.9.0/simpa/core/processing_components/monospectral/noise/salt_and_pepper_noise.py
--rw-r--r--   0        0        0     2993 2024-03-14 09:18:47.915300 simpa-0.9.0/simpa/core/processing_components/monospectral/noise/uniform_noise.py
--rw-r--r--   0        0        0     2353 2024-03-14 09:18:47.915300 simpa-0.9.0/simpa/core/processing_components/multispectral/__init__.py
--rw-r--r--   0        0        0    11797 2024-03-14 09:18:47.915300 simpa-0.9.0/simpa/core/processing_components/multispectral/linear_unmixing.py
--rw-r--r--   0        0        0     5626 2024-03-14 09:18:47.915300 simpa-0.9.0/simpa/core/simulation.py
--rw-r--r--   0        0        0      152 2024-03-14 09:18:47.915300 simpa-0.9.0/simpa/core/simulation_modules/__init__.py
--rw-r--r--   0        0        0     3381 2024-03-14 09:18:47.915300 simpa-0.9.0/simpa/core/simulation_modules/acoustic_forward_module/__init__.py
--rw-r--r--   0        0        0      685 2024-03-14 09:18:47.915300 simpa-0.9.0/simpa/core/simulation_modules/acoustic_forward_module/acoustic_forward_model_test_adapter.py
--rw-r--r--   0        0        0    18268 2024-03-14 09:18:47.915300 simpa-0.9.0/simpa/core/simulation_modules/acoustic_forward_module/acoustic_forward_module_k_wave_adapter.py
--rw-r--r--   0        0        0     5592 2024-03-14 09:18:47.915300 simpa-0.9.0/simpa/core/simulation_modules/acoustic_forward_module/simulate_2D.m
--rw-r--r--   0        0        0     5963 2024-03-14 09:18:47.915300 simpa-0.9.0/simpa/core/simulation_modules/acoustic_forward_module/simulate_3D.m
--rw-r--r--   0        0        0     7435 2024-03-14 09:18:47.915300 simpa-0.9.0/simpa/core/simulation_modules/optical_simulation_module/__init__.py
--rw-r--r--   0        0        0    13487 2024-03-14 09:18:47.915300 simpa-0.9.0/simpa/core/simulation_modules/optical_simulation_module/optical_forward_model_mcx_adapter.py
--rw-r--r--   0        0        0    15424 2024-03-14 09:18:47.915300 simpa-0.9.0/simpa/core/simulation_modules/optical_simulation_module/optical_forward_model_mcx_reflectance_adapter.py
--rw-r--r--   0        0        0      624 2024-03-14 09:18:47.915300 simpa-0.9.0/simpa/core/simulation_modules/optical_simulation_module/optical_forward_model_test_adapter.py
--rw-r--r--   0        0        0     6006 2024-03-14 09:18:47.915300 simpa-0.9.0/simpa/core/simulation_modules/reconstruction_module/__init__.py
--rw-r--r--   0        0        0     4745 2024-03-14 09:18:47.915300 simpa-0.9.0/simpa/core/simulation_modules/reconstruction_module/reconstruction_module_delay_and_sum_adapter.py
--rw-r--r--   0        0        0     5499 2024-03-14 09:18:47.915300 simpa-0.9.0/simpa/core/simulation_modules/reconstruction_module/reconstruction_module_delay_multiply_and_sum_adapter.py
--rw-r--r--   0        0        0     5594 2024-03-14 09:18:47.915300 simpa-0.9.0/simpa/core/simulation_modules/reconstruction_module/reconstruction_module_signed_delay_multiply_and_sum_adapter.py
--rw-r--r--   0        0        0      445 2024-03-14 09:18:47.915300 simpa-0.9.0/simpa/core/simulation_modules/reconstruction_module/reconstruction_module_test_adapter.py
--rw-r--r--   0        0        0    10753 2024-03-14 09:18:47.915300 simpa-0.9.0/simpa/core/simulation_modules/reconstruction_module/reconstruction_module_time_reversal_adapter.py
--rw-r--r--   0        0        0    30174 2024-03-14 09:18:47.915300 simpa-0.9.0/simpa/core/simulation_modules/reconstruction_module/reconstruction_utils.py
--rw-r--r--   0        0        0     4140 2024-03-14 09:18:47.915300 simpa-0.9.0/simpa/core/simulation_modules/reconstruction_module/time_reversal_2D.m
--rw-r--r--   0        0        0     3953 2024-03-14 09:18:47.915300 simpa-0.9.0/simpa/core/simulation_modules/reconstruction_module/time_reversal_3D.m
--rw-r--r--   0        0        0     3405 2024-03-14 09:18:47.915300 simpa-0.9.0/simpa/core/simulation_modules/volume_creation_module/__init__.py
--rw-r--r--   0        0        0     5271 2024-03-14 09:18:47.915300 simpa-0.9.0/simpa/core/simulation_modules/volume_creation_module/volume_creation_module_model_based_adapter.py
--rw-r--r--   0        0        0     2323 2024-03-14 09:18:47.915300 simpa-0.9.0/simpa/core/simulation_modules/volume_creation_module/volume_creation_module_segmentation_based_adapter.py
--rw-r--r--   0        0        0      357 2024-03-14 09:18:47.915300 simpa-0.9.0/simpa/io_handling/__init__.py
--rw-r--r--   0        0        0     8235 2024-03-14 09:18:47.915300 simpa-0.9.0/simpa/io_handling/io_hdf5.py
--rw-r--r--   0        0        0     7835 2024-03-14 09:18:47.915300 simpa-0.9.0/simpa/io_handling/ipasc.py
--rw-r--r--   0        0        0      557 2024-03-14 09:18:47.915300 simpa-0.9.0/simpa/io_handling/serialization.py
--rw-r--r--   0        0        0     1054 2024-03-14 09:18:47.915300 simpa-0.9.0/simpa/io_handling/zenodo_download.py
--rw-r--r--   0        0        0      185 2024-03-14 09:18:47.915300 simpa-0.9.0/simpa/log/__init__.py
--rw-r--r--   0        0        0     4315 2024-03-14 09:18:47.915300 simpa-0.9.0/simpa/log/file_logger.py
--rw-r--r--   0        0        0     2962 2024-03-14 09:18:47.915300 simpa-0.9.0/simpa/utils/__init__.py
--rw-r--r--   0        0        0     7554 2024-03-14 09:18:47.915300 simpa-0.9.0/simpa/utils/calculate.py
--rw-r--r--   0        0        0     1852 2024-03-14 09:18:47.915300 simpa-0.9.0/simpa/utils/constants.py
--rw-r--r--   0        0        0     4064 2024-03-14 09:18:47.915300 simpa-0.9.0/simpa/utils/deformation_manager.py
--rw-r--r--   0        0        0     3487 2024-03-14 09:18:47.915300 simpa-0.9.0/simpa/utils/dict_path_manager.py
--rw-r--r--   0        0        0      152 2024-03-14 09:18:47.915300 simpa-0.9.0/simpa/utils/libraries/__init__.py
--rw-r--r--   0        0        0     3412 2024-03-14 09:18:47.915300 simpa-0.9.0/simpa/utils/libraries/absorption_spectra_data/Copper_Sulphide.npz
--rw-r--r--   0        0        0     7132 2024-03-14 09:18:47.915300 simpa-0.9.0/simpa/utils/libraries/absorption_spectra_data/Deoxyhemoglobin.npz
--rw-r--r--   0        0        0     7132 2024-03-14 09:18:47.915300 simpa-0.9.0/simpa/utils/libraries/absorption_spectra_data/Fat.npz
--rw-r--r--   0        0        0     7132 2024-03-14 09:18:47.915300 simpa-0.9.0/simpa/utils/libraries/absorption_spectra_data/Melanin.npz
--rw-r--r--   0        0        0     3412 2024-03-14 09:18:47.915300 simpa-0.9.0/simpa/utils/libraries/absorption_spectra_data/Nickel_Sulphide.npz
--rw-r--r--   0        0        0     7132 2024-03-14 09:18:47.915300 simpa-0.9.0/simpa/utils/libraries/absorption_spectra_data/Oxyhemoglobin.npz
--rw-r--r--   0        0        0     7132 2024-03-14 09:18:47.915300 simpa-0.9.0/simpa/utils/libraries/absorption_spectra_data/Skin_Baseline.npz
--rw-r--r--   0        0        0     7132 2024-03-14 09:18:47.915300 simpa-0.9.0/simpa/utils/libraries/absorption_spectra_data/Water.npz
--rw-r--r--   0        0        0      411 2024-03-14 09:18:47.915300 simpa-0.9.0/simpa/utils/libraries/absorption_spectra_data/__init__.py
--rw-r--r--   0        0        0      664 2024-03-14 09:18:47.915300 simpa-0.9.0/simpa/utils/libraries/anisotropy_spectra_data/Epidermis_Anisotropy.npz
--rw-r--r--   0        0        0      152 2024-03-14 09:18:47.915300 simpa-0.9.0/simpa/utils/libraries/anisotropy_spectra_data/__init__.py
--rw-r--r--   0        0        0    16697 2024-03-14 09:18:47.915300 simpa-0.9.0/simpa/utils/libraries/literature_values.py
--rw-r--r--   0        0        0    23574 2024-03-14 09:18:47.915300 simpa-0.9.0/simpa/utils/libraries/molecule_library.py
--rw-r--r--   0        0        0      152 2024-03-14 09:18:47.915300 simpa-0.9.0/simpa/utils/libraries/scattering_spectra_data/__init__.py
--rw-r--r--   0        0        0     7132 2024-03-14 09:18:47.915300 simpa-0.9.0/simpa/utils/libraries/scattering_spectra_data/background_scattering.npz
--rw-r--r--   0        0        0     7132 2024-03-14 09:18:47.919300 simpa-0.9.0/simpa/utils/libraries/scattering_spectra_data/blood_scattering.npz
--rw-r--r--   0        0        0     7132 2024-03-14 09:18:47.919300 simpa-0.9.0/simpa/utils/libraries/scattering_spectra_data/bone_scattering.npz
--rw-r--r--   0        0        0     7132 2024-03-14 09:18:47.919300 simpa-0.9.0/simpa/utils/libraries/scattering_spectra_data/fat_scattering.npz
--rw-r--r--   0        0        0     7132 2024-03-14 09:18:47.919300 simpa-0.9.0/simpa/utils/libraries/scattering_spectra_data/muscle_scattering.npz
--rw-r--r--   0        0        0     8132 2024-03-14 09:18:47.919300 simpa-0.9.0/simpa/utils/libraries/spectrum_library.py
--rw-r--r--   0        0        0     1976 2024-03-14 09:18:47.919300 simpa-0.9.0/simpa/utils/libraries/structure_library/BackgroundStructure.py
--rw-r--r--   0        0        0     6534 2024-03-14 09:18:47.919300 simpa-0.9.0/simpa/utils/libraries/structure_library/CircularTubularStructure.py
--rw-r--r--   0        0        0     8317 2024-03-14 09:18:47.919300 simpa-0.9.0/simpa/utils/libraries/structure_library/EllipticalTubularStructure.py
--rw-r--r--   0        0        0     6250 2024-03-14 09:18:47.919300 simpa-0.9.0/simpa/utils/libraries/structure_library/HorizontalLayerStructure.py
--rw-r--r--   0        0        0     4985 2024-03-14 09:18:47.919300 simpa-0.9.0/simpa/utils/libraries/structure_library/ParallelepipedStructure.py
--rw-r--r--   0        0        0     6778 2024-03-14 09:18:47.919300 simpa-0.9.0/simpa/utils/libraries/structure_library/RectangularCuboidStructure.py
--rw-r--r--   0        0        0     4486 2024-03-14 09:18:47.919300 simpa-0.9.0/simpa/utils/libraries/structure_library/SphericalStructure.py
--rw-r--r--   0        0        0     5672 2024-03-14 09:18:47.919300 simpa-0.9.0/simpa/utils/libraries/structure_library/StructureBase.py
--rw-r--r--   0        0        0    10451 2024-03-14 09:18:47.919300 simpa-0.9.0/simpa/utils/libraries/structure_library/VesselStructure.py
--rw-r--r--   0        0        0     2723 2024-03-14 09:18:47.919300 simpa-0.9.0/simpa/utils/libraries/structure_library/__init__.py
--rw-r--r--   0        0        0    13208 2024-03-14 09:18:47.919300 simpa-0.9.0/simpa/utils/libraries/tissue_library.py
--rw-r--r--   0        0        0      833 2024-03-14 09:18:47.919300 simpa-0.9.0/simpa/utils/matlab.py
--rw-r--r--   0        0        0     4829 2024-03-14 09:18:47.919300 simpa-0.9.0/simpa/utils/path_manager.py
--rw-r--r--   0        0        0     1523 2024-03-14 09:18:47.919300 simpa-0.9.0/simpa/utils/processing_device.py
--rw-r--r--   0        0        0      152 2024-03-14 09:18:47.919300 simpa-0.9.0/simpa/utils/quality_assurance/__init__.py
--rw-r--r--   0        0        0     2971 2024-03-14 09:18:47.919300 simpa-0.9.0/simpa/utils/quality_assurance/data_sanity_testing.py
--rw-r--r--   0        0        0      424 2024-03-14 09:18:47.919300 simpa-0.9.0/simpa/utils/serializer.py
--rw-r--r--   0        0        0     6282 2024-03-14 09:18:47.919300 simpa-0.9.0/simpa/utils/settings.py
--rw-r--r--   0        0        0    49074 2024-03-14 09:18:47.919300 simpa-0.9.0/simpa/utils/tags.py
--rw-r--r--   0        0        0     1127 2024-03-14 09:18:47.919300 simpa-0.9.0/simpa/utils/tissue_properties.py
--rw-r--r--   0        0        0      152 2024-03-14 09:18:47.919300 simpa-0.9.0/simpa/visualisation/__init__.py
--rw-r--r--   0        0        0    11487 2024-03-14 09:18:47.919300 simpa-0.9.0/simpa/visualisation/matplotlib_data_visualisation.py
--rw-r--r--   0        0        0     1792 2024-03-14 09:18:47.919300 simpa-0.9.0/simpa/visualisation/matplotlib_device_visualisation.py
--rw-r--r--   0        0        0      702 2024-03-14 09:18:47.919300 simpa-0.9.0/simpa_tests/__init__.py
--rw-r--r--   0        0        0      152 2024-03-14 09:18:47.919300 simpa-0.9.0/simpa_tests/automatic_tests/__init__.py
--rw-r--r--   0        0        0      152 2024-03-14 09:18:47.919300 simpa-0.9.0/simpa_tests/automatic_tests/device_tests/__init__.py
--rw-r--r--   0        0        0     3207 2024-03-14 09:18:47.919300 simpa-0.9.0/simpa_tests/automatic_tests/device_tests/test_curved_array.py
--rw-r--r--   0        0        0     5459 2024-03-14 09:18:47.919300 simpa-0.9.0/simpa_tests/automatic_tests/device_tests/test_field_of_view.py
--rw-r--r--   0        0        0     2200 2024-03-14 09:18:47.919300 simpa-0.9.0/simpa_tests/automatic_tests/device_tests/test_linear_array.py
--rw-r--r--   0        0        0      152 2024-03-14 09:18:47.919300 simpa-0.9.0/simpa_tests/automatic_tests/structure_tests/__init__.py
--rw-r--r--   0        0        0     5650 2024-03-14 09:18:47.919300 simpa-0.9.0/simpa_tests/automatic_tests/structure_tests/test_boxes.py
--rw-r--r--   0        0        0     6793 2024-03-14 09:18:47.919300 simpa-0.9.0/simpa_tests/automatic_tests/structure_tests/test_elliptical_tubes.py
--rw-r--r--   0        0        0     4752 2024-03-14 09:18:47.919300 simpa-0.9.0/simpa_tests/automatic_tests/structure_tests/test_layers.py
--rw-r--r--   0        0        0     6043 2024-03-14 09:18:47.919300 simpa-0.9.0/simpa_tests/automatic_tests/structure_tests/test_parallel_epipeds.py
--rw-r--r--   0        0        0     4704 2024-03-14 09:18:47.919300 simpa-0.9.0/simpa_tests/automatic_tests/structure_tests/test_spheres.py
--rw-r--r--   0        0        0     5212 2024-03-14 09:18:47.919300 simpa-0.9.0/simpa_tests/automatic_tests/structure_tests/test_tubes.py
--rw-r--r--   0        0        0     1850 2024-03-14 09:18:47.919300 simpa-0.9.0/simpa_tests/automatic_tests/structure_tests/test_vesseltree.py
--rw-r--r--   0        0        0     7170 2024-03-14 09:18:47.919300 simpa-0.9.0/simpa_tests/automatic_tests/test_IPASC_export.py
--rw-r--r--   0        0        0    14580 2024-03-14 09:18:47.919300 simpa-0.9.0/simpa_tests/automatic_tests/test_bandpass_filter.py
--rw-r--r--   0        0        0     4438 2024-03-14 09:18:47.919300 simpa-0.9.0/simpa_tests/automatic_tests/test_calculation_utils.py
--rw-r--r--   0        0        0     1462 2024-03-14 09:18:47.919300 simpa-0.9.0/simpa_tests/automatic_tests/test_create_a_volume.py
--rw-r--r--   0        0        0     1930 2024-03-14 09:18:47.919300 simpa-0.9.0/simpa_tests/automatic_tests/test_device_UUID.py
--rw-r--r--   0        0        0     5309 2024-03-14 09:18:47.919300 simpa-0.9.0/simpa_tests/automatic_tests/test_io_handling.py
--rw-r--r--   0        0        0    13319 2024-03-14 09:18:47.919300 simpa-0.9.0/simpa_tests/automatic_tests/test_linear_unmixing.py
--rw-r--r--   0        0        0     1059 2024-03-14 09:18:47.919300 simpa-0.9.0/simpa_tests/automatic_tests/test_logging.py
--rw-r--r--   0        0        0    18260 2024-03-14 09:18:47.919300 simpa-0.9.0/simpa_tests/automatic_tests/test_noise_models.py
--rw-r--r--   0        0        0     4903 2024-03-14 09:18:47.919300 simpa-0.9.0/simpa_tests/automatic_tests/test_path_manager.py
--rw-r--r--   0        0        0     3283 2024-03-14 09:18:47.919300 simpa-0.9.0/simpa_tests/automatic_tests/test_pipeline.py
--rw-r--r--   0        0        0     4697 2024-03-14 09:18:47.919300 simpa-0.9.0/simpa_tests/automatic_tests/test_processing.py
--rw-r--r--   0        0        0     6598 2024-03-14 09:18:47.919300 simpa-0.9.0/simpa_tests/automatic_tests/test_processing_device.py
--rw-r--r--   0        0        0     3137 2024-03-14 09:18:47.919300 simpa-0.9.0/simpa_tests/automatic_tests/test_quality_assurance.py
--rw-r--r--   0        0        0      152 2024-03-14 09:18:47.919300 simpa-0.9.0/simpa_tests/automatic_tests/tissue_library/__init__.py
--rw-r--r--   0        0        0     1165 2024-03-14 09:18:47.923300 simpa-0.9.0/simpa_tests/automatic_tests/tissue_library/test_core_assumptions.py
--rw-r--r--   0        0        0     1920 2024-03-14 09:18:47.923300 simpa-0.9.0/simpa_tests/automatic_tests/tissue_library/test_spectra_can_be_found.py
--rw-r--r--   0        0        0     2840 2024-03-14 09:18:47.923300 simpa-0.9.0/simpa_tests/automatic_tests/tissue_library/test_tissue_library_against_literature_values.py
--rw-r--r--   0        0        0     1670 2024-03-14 09:18:47.923300 simpa-0.9.0/simpa_tests/checklists/release_checklist.md
--rw-r--r--   0        0        0      744 2024-03-14 09:18:47.923300 simpa-0.9.0/simpa_tests/do_coverage.py
--rw-r--r--   0        0        0     1643 2024-03-14 09:18:47.923300 simpa-0.9.0/simpa_tests/full_integration_test.bat
--rw-r--r--   0        0        0    10714 2024-03-14 09:18:47.923300 simpa-0.9.0/simpa_tests/manual_tests/__init__.py
--rw-r--r--   0        0        0    11292 2024-03-14 09:18:47.923300 simpa-0.9.0/simpa_tests/manual_tests/acoustic_forward_models/KWaveAcousticForwardConvenienceFunction.py
--rw-r--r--   0        0        0     6535 2024-03-14 09:18:47.923300 simpa-0.9.0/simpa_tests/manual_tests/acoustic_forward_models/MinimalKWaveTest.py
--rw-r--r--   0        0        0      152 2024-03-14 09:18:47.923300 simpa-0.9.0/simpa_tests/manual_tests/acoustic_forward_models/__init__.py
--rw-r--r--   0        0        0    10727 2024-03-14 09:18:47.923300 simpa-0.9.0/simpa_tests/manual_tests/digital_device_twins/SimulationWithMSOTInvision.py
--rw-r--r--   0        0        0     1140 2024-03-14 09:18:47.923300 simpa-0.9.0/simpa_tests/manual_tests/digital_device_twins/VisualiseDevices.py
--rw-r--r--   0        0        0      152 2024-03-14 09:18:47.923300 simpa-0.9.0/simpa_tests/manual_tests/digital_device_twins/__init__.py
--rw-r--r--   0        0        0     3058 2024-03-14 09:18:47.923300 simpa-0.9.0/simpa_tests/manual_tests/image_reconstruction/DelayAndSumReconstruction.py
--rw-r--r--   0        0        0     3107 2024-03-14 09:18:47.923300 simpa-0.9.0/simpa_tests/manual_tests/image_reconstruction/DelayMultiplyAndSumReconstruction.py
--rw-r--r--   0        0        0    13992 2024-03-14 09:18:47.923300 simpa-0.9.0/simpa_tests/manual_tests/image_reconstruction/PointSourceReconstruction.py
--rw-r--r--   0        0        0     3208 2024-03-14 09:18:47.923300 simpa-0.9.0/simpa_tests/manual_tests/image_reconstruction/SignedDelayMultiplyAndSumReconstruction.py
--rw-r--r--   0        0        0     1893 2024-03-14 09:18:47.923300 simpa-0.9.0/simpa_tests/manual_tests/image_reconstruction/TimeReversalReconstruction.py
--rw-r--r--   0        0        0      152 2024-03-14 09:18:47.923300 simpa-0.9.0/simpa_tests/manual_tests/image_reconstruction/__init__.py
--rw-r--r--   0        0        0    13860 2024-03-14 09:18:47.923300 simpa-0.9.0/simpa_tests/manual_tests/optical_forward_models/AbsorptionAndScatteringWithInifinitesimalSlabExperiment.py
--rw-r--r--   0        0        0    14749 2024-03-14 09:18:47.923300 simpa-0.9.0/simpa_tests/manual_tests/optical_forward_models/AbsorptionAndScatteringWithinHomogenousMedium.py
--rw-r--r--   0        0        0     7943 2024-03-14 09:18:47.923300 simpa-0.9.0/simpa_tests/manual_tests/optical_forward_models/CompareMCXResultsWithDiffusionTheory.py
--rw-r--r--   0        0        0     9513 2024-03-14 09:18:47.923300 simpa-0.9.0/simpa_tests/manual_tests/optical_forward_models/ComputeDiffuseReflectance.py
--rw-r--r--   0        0        0      152 2024-03-14 09:18:47.923300 simpa-0.9.0/simpa_tests/manual_tests/optical_forward_models/__init__.py
--rw-r--r--   0        0        0    13374 2024-03-14 09:18:47.923300 simpa-0.9.0/simpa_tests/manual_tests/processing_components/QPAIReconstruction.py
--rw-r--r--   0        0        0     5325 2024-03-14 09:18:47.923300 simpa-0.9.0/simpa_tests/manual_tests/processing_components/TestLinearUnmixingVisual.py
--rw-r--r--   0        0        0      152 2024-03-14 09:18:47.923300 simpa-0.9.0/simpa_tests/manual_tests/processing_components/__init__.py
--rw-r--r--   0        0        0    13965 2024-03-14 09:18:47.923300 simpa-0.9.0/simpa_tests/manual_tests/test_with_experimental_measurements/ReproduceDISMeasurements.py
--rw-r--r--   0        0        0      152 2024-03-14 09:18:47.923300 simpa-0.9.0/simpa_tests/manual_tests/test_with_experimental_measurements/__init__.py
--rw-r--r--   0        0        0     5969 2024-03-14 09:18:47.923300 simpa-0.9.0/simpa_tests/manual_tests/test_with_experimental_measurements/test_data/background_material_dark.rxt
--rw-r--r--   0        0        0     7652 2024-03-14 09:18:47.923300 simpa-0.9.0/simpa_tests/manual_tests/test_with_experimental_measurements/test_data/background_material_dark_spectra.npz
--rw-r--r--   0        0        0     5969 2024-03-14 09:18:47.923300 simpa-0.9.0/simpa_tests/manual_tests/test_with_experimental_measurements/test_data/background_material_light.rxt
--rw-r--r--   0        0        0     7652 2024-03-14 09:18:47.923300 simpa-0.9.0/simpa_tests/manual_tests/test_with_experimental_measurements/test_data/background_material_light_spectra.npz
--rw-r--r--   0        0        0     5969 2024-03-14 09:18:47.923300 simpa-0.9.0/simpa_tests/manual_tests/test_with_experimental_measurements/test_data/inclusion_material.rxt
--rw-r--r--   0        0        0     7652 2024-03-14 09:18:47.923300 simpa-0.9.0/simpa_tests/manual_tests/test_with_experimental_measurements/test_data/inclusion_material_spectra.npz
--rw-r--r--   0        0        0     1258 2024-03-14 09:18:47.923300 simpa-0.9.0/simpa_tests/manual_tests/test_with_experimental_measurements/utils.py
--rw-r--r--   0        0        0     5035 2024-03-14 09:18:47.923300 simpa-0.9.0/simpa_tests/manual_tests/volume_creation/SegmentationLoader.py
--rw-r--r--   0        0        0      152 2024-03-14 09:18:47.923300 simpa-0.9.0/simpa_tests/manual_tests/volume_creation/__init__.py
--rw-r--r--   0        0        0     5070 2024-03-14 09:18:47.923300 simpa-0.9.0/simpa_tests/test_utils/__init__.py
--rw-r--r--   0        0        0    46399 2024-03-14 09:18:47.923300 simpa-0.9.0/simpa_tests/test_utils/tissue_composition_tests.py
--rw-r--r--   0        0        0     2458 2024-03-14 09:18:47.923300 simpa-0.9.0/simpa_tests/test_utils/tissue_models.py
--rw-r--r--   0        0        0    12141 1970-01-01 00:00:00.000000 simpa-0.9.0/PKG-INFO
+-rw-r--r--   0        0        0      236 2024-04-02 15:24:14.653687 simpa-0.9.1/LICENSE.md
+drwxr-xr-x   0        0        0        0 2024-04-02 15:24:14.653687 simpa-0.9.1/LICENSES/
+-rw-r--r--   0        0        0     1144 2024-04-02 15:24:14.653687 simpa-0.9.1/LICENSES/MIT
+-rwxr-xr-x   0        0        0    10700 2024-04-02 15:24:14.653687 simpa-0.9.1/README.md
+-rw-r--r--   0        0        0     2049 2024-04-02 15:24:14.657687 simpa-0.9.1/pyproject.toml
+-rw-r--r--   0        0        0     3314 2024-04-02 15:24:14.657687 simpa-0.9.1/simpa/__init__.py
+-rw-r--r--   0        0        0      968 2024-04-02 15:24:14.657687 simpa-0.9.1/simpa/core/__init__.py
+-rw-r--r--   0        0        0     1548 2024-04-02 15:24:14.657687 simpa-0.9.1/simpa/core/device_digital_twins/__init__.py
+-rw-r--r--   0        0        0      152 2024-04-02 15:24:14.657687 simpa-0.9.1/simpa/core/device_digital_twins/detection_geometries/__init__.py
+-rw-r--r--   0        0        0     5496 2024-04-02 15:24:14.657687 simpa-0.9.1/simpa/core/device_digital_twins/detection_geometries/curved_array.py
+-rw-r--r--   0        0        0     6117 2024-04-02 15:24:14.657687 simpa-0.9.1/simpa/core/device_digital_twins/detection_geometries/detection_geometry_base.py
+-rw-r--r--   0        0        0     4518 2024-04-02 15:24:14.657687 simpa-0.9.1/simpa/core/device_digital_twins/detection_geometries/linear_array.py
+-rw-r--r--   0        0        0     5481 2024-04-02 15:24:14.657687 simpa-0.9.1/simpa/core/device_digital_twins/detection_geometries/planar_array.py
+-rw-r--r--   0        0        0    13839 2024-04-02 15:24:14.657687 simpa-0.9.1/simpa/core/device_digital_twins/digital_device_twin_base.py
+-rw-r--r--   0        0        0      152 2024-04-02 15:24:14.657687 simpa-0.9.1/simpa/core/device_digital_twins/illumination_geometries/__init__.py
+-rw-r--r--   0        0        0     2558 2024-04-02 15:24:14.657687 simpa-0.9.1/simpa/core/device_digital_twins/illumination_geometries/disk_illumination.py
+-rw-r--r--   0        0        0     3492 2024-04-02 15:24:14.657687 simpa-0.9.1/simpa/core/device_digital_twins/illumination_geometries/gaussian_beam_illumination.py
+-rw-r--r--   0        0        0     2987 2024-04-02 15:24:14.657687 simpa-0.9.1/simpa/core/device_digital_twins/illumination_geometries/illumination_geometry_base.py
+-rw-r--r--   0        0        0     2832 2024-04-02 15:24:14.657687 simpa-0.9.1/simpa/core/device_digital_twins/illumination_geometries/ithera_msot_acuity_illumination.py
+-rw-r--r--   0        0        0     3420 2024-04-02 15:24:14.657687 simpa-0.9.1/simpa/core/device_digital_twins/illumination_geometries/ithera_msot_invision_illumination.py
+-rw-r--r--   0        0        0     3246 2024-04-02 15:24:14.657687 simpa-0.9.1/simpa/core/device_digital_twins/illumination_geometries/pencil_array_illumination.py
+-rw-r--r--   0        0        0     1515 2024-04-02 15:24:14.657687 simpa-0.9.1/simpa/core/device_digital_twins/illumination_geometries/pencil_beam_illumination.py
+-rw-r--r--   0        0        0     3521 2024-04-02 15:24:14.657687 simpa-0.9.1/simpa/core/device_digital_twins/illumination_geometries/slit_illumination.py
+-rw-r--r--   0        0        0      152 2024-04-02 15:24:14.657687 simpa-0.9.1/simpa/core/device_digital_twins/pa_devices/__init__.py
+-rw-r--r--   0        0        0    12456 2024-04-02 15:24:14.657687 simpa-0.9.1/simpa/core/device_digital_twins/pa_devices/ithera_msot_acuity.py
+-rw-r--r--   0        0        0     3730 2024-04-02 15:24:14.657687 simpa-0.9.1/simpa/core/device_digital_twins/pa_devices/ithera_msot_invision.py
+-rw-r--r--   0        0        0     4931 2024-04-02 15:24:14.657687 simpa-0.9.1/simpa/core/device_digital_twins/pa_devices/ithera_rsom.py
+-rw-r--r--   0        0        0      895 2024-04-02 15:24:14.657687 simpa-0.9.1/simpa/core/processing_components/__init__.py
+-rw-r--r--   0        0        0      152 2024-04-02 15:24:14.657687 simpa-0.9.1/simpa/core/processing_components/monospectral/__init__.py
+-rw-r--r--   0        0        0     5528 2024-04-02 15:24:14.661687 simpa-0.9.1/simpa/core/processing_components/monospectral/field_of_view_cropping.py
+-rw-r--r--   0        0        0    27651 2024-04-02 15:24:14.661687 simpa-0.9.1/simpa/core/processing_components/monospectral/iterative_qPAI_algorithm.py
+-rw-r--r--   0        0        0      365 2024-04-02 15:24:14.661687 simpa-0.9.1/simpa/core/processing_components/monospectral/noise/__init__.py
+-rw-r--r--   0        0        0     2895 2024-04-02 15:24:14.661687 simpa-0.9.1/simpa/core/processing_components/monospectral/noise/gamma_noise.py
+-rw-r--r--   0        0        0     3320 2024-04-02 15:24:14.661687 simpa-0.9.1/simpa/core/processing_components/monospectral/noise/gaussian_noise.py
+-rw-r--r--   0        0        0     2543 2024-04-02 15:24:14.661687 simpa-0.9.1/simpa/core/processing_components/monospectral/noise/poisson_noise.py
+-rw-r--r--   0        0        0     3207 2024-04-02 15:24:14.661687 simpa-0.9.1/simpa/core/processing_components/monospectral/noise/salt_and_pepper_noise.py
+-rw-r--r--   0        0        0     2993 2024-04-02 15:24:14.661687 simpa-0.9.1/simpa/core/processing_components/monospectral/noise/uniform_noise.py
+-rw-r--r--   0        0        0     2353 2024-04-02 15:24:14.661687 simpa-0.9.1/simpa/core/processing_components/multispectral/__init__.py
+-rw-r--r--   0        0        0    11797 2024-04-02 15:24:14.661687 simpa-0.9.1/simpa/core/processing_components/multispectral/linear_unmixing.py
+-rw-r--r--   0        0        0     5626 2024-04-02 15:24:14.661687 simpa-0.9.1/simpa/core/simulation.py
+-rw-r--r--   0        0        0      152 2024-04-02 15:24:14.661687 simpa-0.9.1/simpa/core/simulation_modules/__init__.py
+-rw-r--r--   0        0        0     3381 2024-04-02 15:24:14.661687 simpa-0.9.1/simpa/core/simulation_modules/acoustic_forward_module/__init__.py
+-rw-r--r--   0        0        0      685 2024-04-02 15:24:14.661687 simpa-0.9.1/simpa/core/simulation_modules/acoustic_forward_module/acoustic_forward_model_test_adapter.py
+-rw-r--r--   0        0        0    18268 2024-04-02 15:24:14.661687 simpa-0.9.1/simpa/core/simulation_modules/acoustic_forward_module/acoustic_forward_module_k_wave_adapter.py
+-rw-r--r--   0        0        0     5592 2024-04-02 15:24:14.661687 simpa-0.9.1/simpa/core/simulation_modules/acoustic_forward_module/simulate_2D.m
+-rw-r--r--   0        0        0     5963 2024-04-02 15:24:14.661687 simpa-0.9.1/simpa/core/simulation_modules/acoustic_forward_module/simulate_3D.m
+-rw-r--r--   0        0        0     7435 2024-04-02 15:24:14.661687 simpa-0.9.1/simpa/core/simulation_modules/optical_simulation_module/__init__.py
+-rw-r--r--   0        0        0    13487 2024-04-02 15:24:14.661687 simpa-0.9.1/simpa/core/simulation_modules/optical_simulation_module/optical_forward_model_mcx_adapter.py
+-rw-r--r--   0        0        0    15424 2024-04-02 15:24:14.661687 simpa-0.9.1/simpa/core/simulation_modules/optical_simulation_module/optical_forward_model_mcx_reflectance_adapter.py
+-rw-r--r--   0        0        0      624 2024-04-02 15:24:14.661687 simpa-0.9.1/simpa/core/simulation_modules/optical_simulation_module/optical_forward_model_test_adapter.py
+-rw-r--r--   0        0        0     6006 2024-04-02 15:24:14.661687 simpa-0.9.1/simpa/core/simulation_modules/reconstruction_module/__init__.py
+-rw-r--r--   0        0        0     4745 2024-04-02 15:24:14.661687 simpa-0.9.1/simpa/core/simulation_modules/reconstruction_module/reconstruction_module_delay_and_sum_adapter.py
+-rw-r--r--   0        0        0     5499 2024-04-02 15:24:14.661687 simpa-0.9.1/simpa/core/simulation_modules/reconstruction_module/reconstruction_module_delay_multiply_and_sum_adapter.py
+-rw-r--r--   0        0        0     5594 2024-04-02 15:24:14.661687 simpa-0.9.1/simpa/core/simulation_modules/reconstruction_module/reconstruction_module_signed_delay_multiply_and_sum_adapter.py
+-rw-r--r--   0        0        0      445 2024-04-02 15:24:14.661687 simpa-0.9.1/simpa/core/simulation_modules/reconstruction_module/reconstruction_module_test_adapter.py
+-rw-r--r--   0        0        0    10753 2024-04-02 15:24:14.661687 simpa-0.9.1/simpa/core/simulation_modules/reconstruction_module/reconstruction_module_time_reversal_adapter.py
+-rw-r--r--   0        0        0    30174 2024-04-02 15:24:14.661687 simpa-0.9.1/simpa/core/simulation_modules/reconstruction_module/reconstruction_utils.py
+-rw-r--r--   0        0        0     4140 2024-04-02 15:24:14.661687 simpa-0.9.1/simpa/core/simulation_modules/reconstruction_module/time_reversal_2D.m
+-rw-r--r--   0        0        0     3953 2024-04-02 15:24:14.661687 simpa-0.9.1/simpa/core/simulation_modules/reconstruction_module/time_reversal_3D.m
+-rw-r--r--   0        0        0     3405 2024-04-02 15:24:14.661687 simpa-0.9.1/simpa/core/simulation_modules/volume_creation_module/__init__.py
+-rw-r--r--   0        0        0     5271 2024-04-02 15:24:14.661687 simpa-0.9.1/simpa/core/simulation_modules/volume_creation_module/volume_creation_module_model_based_adapter.py
+-rw-r--r--   0        0        0     2629 2024-04-02 15:24:14.661687 simpa-0.9.1/simpa/core/simulation_modules/volume_creation_module/volume_creation_module_segmentation_based_adapter.py
+-rw-r--r--   0        0        0      357 2024-04-02 15:24:14.661687 simpa-0.9.1/simpa/io_handling/__init__.py
+-rw-r--r--   0        0        0     8235 2024-04-02 15:24:14.661687 simpa-0.9.1/simpa/io_handling/io_hdf5.py
+-rw-r--r--   0        0        0     7835 2024-04-02 15:24:14.661687 simpa-0.9.1/simpa/io_handling/ipasc.py
+-rw-r--r--   0        0        0      557 2024-04-02 15:24:14.661687 simpa-0.9.1/simpa/io_handling/serialization.py
+-rw-r--r--   0        0        0     1054 2024-04-02 15:24:14.661687 simpa-0.9.1/simpa/io_handling/zenodo_download.py
+-rw-r--r--   0        0        0      185 2024-04-02 15:24:14.661687 simpa-0.9.1/simpa/log/__init__.py
+-rw-r--r--   0        0        0     4315 2024-04-02 15:24:14.661687 simpa-0.9.1/simpa/log/file_logger.py
+-rw-r--r--   0        0        0     2962 2024-04-02 15:24:14.661687 simpa-0.9.1/simpa/utils/__init__.py
+-rw-r--r--   0        0        0     7554 2024-04-02 15:24:14.661687 simpa-0.9.1/simpa/utils/calculate.py
+-rw-r--r--   0        0        0     1852 2024-04-02 15:24:14.661687 simpa-0.9.1/simpa/utils/constants.py
+-rw-r--r--   0        0        0     4064 2024-04-02 15:24:14.661687 simpa-0.9.1/simpa/utils/deformation_manager.py
+-rw-r--r--   0        0        0     3487 2024-04-02 15:24:14.661687 simpa-0.9.1/simpa/utils/dict_path_manager.py
+-rw-r--r--   0        0        0      152 2024-04-02 15:24:14.661687 simpa-0.9.1/simpa/utils/libraries/__init__.py
+-rw-r--r--   0        0        0     3412 2024-04-02 15:24:14.661687 simpa-0.9.1/simpa/utils/libraries/absorption_spectra_data/Copper_Sulphide.npz
+-rw-r--r--   0        0        0     7132 2024-04-02 15:24:14.661687 simpa-0.9.1/simpa/utils/libraries/absorption_spectra_data/Deoxyhemoglobin.npz
+-rw-r--r--   0        0        0     7132 2024-04-02 15:24:14.661687 simpa-0.9.1/simpa/utils/libraries/absorption_spectra_data/Fat.npz
+-rw-r--r--   0        0        0     7132 2024-04-02 15:24:14.661687 simpa-0.9.1/simpa/utils/libraries/absorption_spectra_data/Melanin.npz
+-rw-r--r--   0        0        0     3412 2024-04-02 15:24:14.661687 simpa-0.9.1/simpa/utils/libraries/absorption_spectra_data/Nickel_Sulphide.npz
+-rw-r--r--   0        0        0     7132 2024-04-02 15:24:14.661687 simpa-0.9.1/simpa/utils/libraries/absorption_spectra_data/Oxyhemoglobin.npz
+-rw-r--r--   0        0        0     7132 2024-04-02 15:24:14.661687 simpa-0.9.1/simpa/utils/libraries/absorption_spectra_data/Skin_Baseline.npz
+-rw-r--r--   0        0        0     7132 2024-04-02 15:24:14.661687 simpa-0.9.1/simpa/utils/libraries/absorption_spectra_data/Water.npz
+-rw-r--r--   0        0        0      411 2024-04-02 15:24:14.661687 simpa-0.9.1/simpa/utils/libraries/absorption_spectra_data/__init__.py
+-rw-r--r--   0        0        0      664 2024-04-02 15:24:14.661687 simpa-0.9.1/simpa/utils/libraries/anisotropy_spectra_data/Epidermis_Anisotropy.npz
+-rw-r--r--   0        0        0      152 2024-04-02 15:24:14.661687 simpa-0.9.1/simpa/utils/libraries/anisotropy_spectra_data/__init__.py
+-rw-r--r--   0        0        0    16697 2024-04-02 15:24:14.661687 simpa-0.9.1/simpa/utils/libraries/literature_values.py
+-rw-r--r--   0        0        0    23574 2024-04-02 15:24:14.661687 simpa-0.9.1/simpa/utils/libraries/molecule_library.py
+-rw-r--r--   0        0        0      152 2024-04-02 15:24:14.661687 simpa-0.9.1/simpa/utils/libraries/scattering_spectra_data/__init__.py
+-rw-r--r--   0        0        0     7132 2024-04-02 15:24:14.661687 simpa-0.9.1/simpa/utils/libraries/scattering_spectra_data/background_scattering.npz
+-rw-r--r--   0        0        0     7132 2024-04-02 15:24:14.661687 simpa-0.9.1/simpa/utils/libraries/scattering_spectra_data/blood_scattering.npz
+-rw-r--r--   0        0        0     7132 2024-04-02 15:24:14.661687 simpa-0.9.1/simpa/utils/libraries/scattering_spectra_data/bone_scattering.npz
+-rw-r--r--   0        0        0     7132 2024-04-02 15:24:14.661687 simpa-0.9.1/simpa/utils/libraries/scattering_spectra_data/fat_scattering.npz
+-rw-r--r--   0        0        0     7132 2024-04-02 15:24:14.665687 simpa-0.9.1/simpa/utils/libraries/scattering_spectra_data/muscle_scattering.npz
+-rw-r--r--   0        0        0     8132 2024-04-02 15:24:14.665687 simpa-0.9.1/simpa/utils/libraries/spectrum_library.py
+-rw-r--r--   0        0        0     1976 2024-04-02 15:24:14.665687 simpa-0.9.1/simpa/utils/libraries/structure_library/BackgroundStructure.py
+-rw-r--r--   0        0        0     6534 2024-04-02 15:24:14.665687 simpa-0.9.1/simpa/utils/libraries/structure_library/CircularTubularStructure.py
+-rw-r--r--   0        0        0     8317 2024-04-02 15:24:14.665687 simpa-0.9.1/simpa/utils/libraries/structure_library/EllipticalTubularStructure.py
+-rw-r--r--   0        0        0     6250 2024-04-02 15:24:14.665687 simpa-0.9.1/simpa/utils/libraries/structure_library/HorizontalLayerStructure.py
+-rw-r--r--   0        0        0     4985 2024-04-02 15:24:14.665687 simpa-0.9.1/simpa/utils/libraries/structure_library/ParallelepipedStructure.py
+-rw-r--r--   0        0        0     6778 2024-04-02 15:24:14.665687 simpa-0.9.1/simpa/utils/libraries/structure_library/RectangularCuboidStructure.py
+-rw-r--r--   0        0        0     4486 2024-04-02 15:24:14.665687 simpa-0.9.1/simpa/utils/libraries/structure_library/SphericalStructure.py
+-rw-r--r--   0        0        0     5672 2024-04-02 15:24:14.665687 simpa-0.9.1/simpa/utils/libraries/structure_library/StructureBase.py
+-rw-r--r--   0        0        0    10451 2024-04-02 15:24:14.665687 simpa-0.9.1/simpa/utils/libraries/structure_library/VesselStructure.py
+-rw-r--r--   0        0        0     2723 2024-04-02 15:24:14.665687 simpa-0.9.1/simpa/utils/libraries/structure_library/__init__.py
+-rw-r--r--   0        0        0    13208 2024-04-02 15:24:14.665687 simpa-0.9.1/simpa/utils/libraries/tissue_library.py
+-rw-r--r--   0        0        0      833 2024-04-02 15:24:14.665687 simpa-0.9.1/simpa/utils/matlab.py
+-rw-r--r--   0        0        0     4829 2024-04-02 15:24:14.665687 simpa-0.9.1/simpa/utils/path_manager.py
+-rw-r--r--   0        0        0     1523 2024-04-02 15:24:14.665687 simpa-0.9.1/simpa/utils/processing_device.py
+-rw-r--r--   0        0        0      152 2024-04-02 15:24:14.665687 simpa-0.9.1/simpa/utils/quality_assurance/__init__.py
+-rw-r--r--   0        0        0     2971 2024-04-02 15:24:14.665687 simpa-0.9.1/simpa/utils/quality_assurance/data_sanity_testing.py
+-rw-r--r--   0        0        0      424 2024-04-02 15:24:14.665687 simpa-0.9.1/simpa/utils/serializer.py
+-rw-r--r--   0        0        0     6282 2024-04-02 15:24:14.665687 simpa-0.9.1/simpa/utils/settings.py
+-rw-r--r--   0        0        0    49074 2024-04-02 15:24:14.665687 simpa-0.9.1/simpa/utils/tags.py
+-rw-r--r--   0        0        0     1127 2024-04-02 15:24:14.665687 simpa-0.9.1/simpa/utils/tissue_properties.py
+-rw-r--r--   0        0        0      152 2024-04-02 15:24:14.665687 simpa-0.9.1/simpa/visualisation/__init__.py
+-rw-r--r--   0        0        0    11487 2024-04-02 15:24:14.665687 simpa-0.9.1/simpa/visualisation/matplotlib_data_visualisation.py
+-rw-r--r--   0        0        0     1792 2024-04-02 15:24:14.665687 simpa-0.9.1/simpa/visualisation/matplotlib_device_visualisation.py
+-rw-r--r--   0        0        0      702 2024-04-02 15:24:14.665687 simpa-0.9.1/simpa_tests/__init__.py
+-rw-r--r--   0        0        0      152 2024-04-02 15:24:14.665687 simpa-0.9.1/simpa_tests/automatic_tests/__init__.py
+-rw-r--r--   0        0        0      152 2024-04-02 15:24:14.665687 simpa-0.9.1/simpa_tests/automatic_tests/device_tests/__init__.py
+-rw-r--r--   0        0        0     3207 2024-04-02 15:24:14.665687 simpa-0.9.1/simpa_tests/automatic_tests/device_tests/test_curved_array.py
+-rw-r--r--   0        0        0     5459 2024-04-02 15:24:14.665687 simpa-0.9.1/simpa_tests/automatic_tests/device_tests/test_field_of_view.py
+-rw-r--r--   0        0        0     2200 2024-04-02 15:24:14.665687 simpa-0.9.1/simpa_tests/automatic_tests/device_tests/test_linear_array.py
+-rw-r--r--   0        0        0      152 2024-04-02 15:24:14.665687 simpa-0.9.1/simpa_tests/automatic_tests/structure_tests/__init__.py
+-rw-r--r--   0        0        0     5650 2024-04-02 15:24:14.665687 simpa-0.9.1/simpa_tests/automatic_tests/structure_tests/test_boxes.py
+-rw-r--r--   0        0        0     6793 2024-04-02 15:24:14.665687 simpa-0.9.1/simpa_tests/automatic_tests/structure_tests/test_elliptical_tubes.py
+-rw-r--r--   0        0        0     4752 2024-04-02 15:24:14.665687 simpa-0.9.1/simpa_tests/automatic_tests/structure_tests/test_layers.py
+-rw-r--r--   0        0        0     6043 2024-04-02 15:24:14.665687 simpa-0.9.1/simpa_tests/automatic_tests/structure_tests/test_parallel_epipeds.py
+-rw-r--r--   0        0        0     4704 2024-04-02 15:24:14.665687 simpa-0.9.1/simpa_tests/automatic_tests/structure_tests/test_spheres.py
+-rw-r--r--   0        0        0     5212 2024-04-02 15:24:14.665687 simpa-0.9.1/simpa_tests/automatic_tests/structure_tests/test_tubes.py
+-rw-r--r--   0        0        0     1850 2024-04-02 15:24:14.665687 simpa-0.9.1/simpa_tests/automatic_tests/structure_tests/test_vesseltree.py
+-rw-r--r--   0        0        0     7170 2024-04-02 15:24:14.665687 simpa-0.9.1/simpa_tests/automatic_tests/test_IPASC_export.py
+-rw-r--r--   0        0        0    14580 2024-04-02 15:24:14.665687 simpa-0.9.1/simpa_tests/automatic_tests/test_bandpass_filter.py
+-rw-r--r--   0        0        0     4438 2024-04-02 15:24:14.665687 simpa-0.9.1/simpa_tests/automatic_tests/test_calculation_utils.py
+-rw-r--r--   0        0        0     1462 2024-04-02 15:24:14.665687 simpa-0.9.1/simpa_tests/automatic_tests/test_create_a_volume.py
+-rw-r--r--   0        0        0     1930 2024-04-02 15:24:14.665687 simpa-0.9.1/simpa_tests/automatic_tests/test_device_UUID.py
+-rw-r--r--   0        0        0     5309 2024-04-02 15:24:14.665687 simpa-0.9.1/simpa_tests/automatic_tests/test_io_handling.py
+-rw-r--r--   0        0        0    13319 2024-04-02 15:24:14.665687 simpa-0.9.1/simpa_tests/automatic_tests/test_linear_unmixing.py
+-rw-r--r--   0        0        0     1059 2024-04-02 15:24:14.665687 simpa-0.9.1/simpa_tests/automatic_tests/test_logging.py
+-rw-r--r--   0        0        0    18260 2024-04-02 15:24:14.665687 simpa-0.9.1/simpa_tests/automatic_tests/test_noise_models.py
+-rw-r--r--   0        0        0     4903 2024-04-02 15:24:14.665687 simpa-0.9.1/simpa_tests/automatic_tests/test_path_manager.py
+-rw-r--r--   0        0        0     3283 2024-04-02 15:24:14.665687 simpa-0.9.1/simpa_tests/automatic_tests/test_pipeline.py
+-rw-r--r--   0        0        0     4697 2024-04-02 15:24:14.665687 simpa-0.9.1/simpa_tests/automatic_tests/test_processing.py
+-rw-r--r--   0        0        0     6598 2024-04-02 15:24:14.665687 simpa-0.9.1/simpa_tests/automatic_tests/test_processing_device.py
+-rw-r--r--   0        0        0     3137 2024-04-02 15:24:14.665687 simpa-0.9.1/simpa_tests/automatic_tests/test_quality_assurance.py
+-rw-r--r--   0        0        0      152 2024-04-02 15:24:14.665687 simpa-0.9.1/simpa_tests/automatic_tests/tissue_library/__init__.py
+-rw-r--r--   0        0        0     1165 2024-04-02 15:24:14.665687 simpa-0.9.1/simpa_tests/automatic_tests/tissue_library/test_core_assumptions.py
+-rw-r--r--   0        0        0     1920 2024-04-02 15:24:14.665687 simpa-0.9.1/simpa_tests/automatic_tests/tissue_library/test_spectra_can_be_found.py
+-rw-r--r--   0        0        0     2840 2024-04-02 15:24:14.665687 simpa-0.9.1/simpa_tests/automatic_tests/tissue_library/test_tissue_library_against_literature_values.py
+-rw-r--r--   0        0        0     1670 2024-04-02 15:24:14.665687 simpa-0.9.1/simpa_tests/checklists/release_checklist.md
+-rw-r--r--   0        0        0      744 2024-04-02 15:24:14.665687 simpa-0.9.1/simpa_tests/do_coverage.py
+-rw-r--r--   0        0        0     1643 2024-04-02 15:24:14.665687 simpa-0.9.1/simpa_tests/full_integration_test.bat
+-rw-r--r--   0        0        0    10714 2024-04-02 15:24:14.665687 simpa-0.9.1/simpa_tests/manual_tests/__init__.py
+-rw-r--r--   0        0        0    11292 2024-04-02 15:24:14.669688 simpa-0.9.1/simpa_tests/manual_tests/acoustic_forward_models/KWaveAcousticForwardConvenienceFunction.py
+-rw-r--r--   0        0        0     6535 2024-04-02 15:24:14.669688 simpa-0.9.1/simpa_tests/manual_tests/acoustic_forward_models/MinimalKWaveTest.py
+-rw-r--r--   0        0        0      152 2024-04-02 15:24:14.669688 simpa-0.9.1/simpa_tests/manual_tests/acoustic_forward_models/__init__.py
+-rw-r--r--   0        0        0    10727 2024-04-02 15:24:14.669688 simpa-0.9.1/simpa_tests/manual_tests/digital_device_twins/SimulationWithMSOTInvision.py
+-rw-r--r--   0        0        0     1140 2024-04-02 15:24:14.669688 simpa-0.9.1/simpa_tests/manual_tests/digital_device_twins/VisualiseDevices.py
+-rw-r--r--   0        0        0      152 2024-04-02 15:24:14.669688 simpa-0.9.1/simpa_tests/manual_tests/digital_device_twins/__init__.py
+-rw-r--r--   0        0        0     3058 2024-04-02 15:24:14.669688 simpa-0.9.1/simpa_tests/manual_tests/image_reconstruction/DelayAndSumReconstruction.py
+-rw-r--r--   0        0        0     3107 2024-04-02 15:24:14.669688 simpa-0.9.1/simpa_tests/manual_tests/image_reconstruction/DelayMultiplyAndSumReconstruction.py
+-rw-r--r--   0        0        0    13992 2024-04-02 15:24:14.669688 simpa-0.9.1/simpa_tests/manual_tests/image_reconstruction/PointSourceReconstruction.py
+-rw-r--r--   0        0        0     3208 2024-04-02 15:24:14.669688 simpa-0.9.1/simpa_tests/manual_tests/image_reconstruction/SignedDelayMultiplyAndSumReconstruction.py
+-rw-r--r--   0        0        0     1893 2024-04-02 15:24:14.669688 simpa-0.9.1/simpa_tests/manual_tests/image_reconstruction/TimeReversalReconstruction.py
+-rw-r--r--   0        0        0      152 2024-04-02 15:24:14.669688 simpa-0.9.1/simpa_tests/manual_tests/image_reconstruction/__init__.py
+-rw-r--r--   0        0        0    13860 2024-04-02 15:24:14.669688 simpa-0.9.1/simpa_tests/manual_tests/optical_forward_models/AbsorptionAndScatteringWithInifinitesimalSlabExperiment.py
+-rw-r--r--   0        0        0    14749 2024-04-02 15:24:14.669688 simpa-0.9.1/simpa_tests/manual_tests/optical_forward_models/AbsorptionAndScatteringWithinHomogenousMedium.py
+-rw-r--r--   0        0        0     7943 2024-04-02 15:24:14.669688 simpa-0.9.1/simpa_tests/manual_tests/optical_forward_models/CompareMCXResultsWithDiffusionTheory.py
+-rw-r--r--   0        0        0     9513 2024-04-02 15:24:14.669688 simpa-0.9.1/simpa_tests/manual_tests/optical_forward_models/ComputeDiffuseReflectance.py
+-rw-r--r--   0        0        0      152 2024-04-02 15:24:14.669688 simpa-0.9.1/simpa_tests/manual_tests/optical_forward_models/__init__.py
+-rw-r--r--   0        0        0    13374 2024-04-02 15:24:14.669688 simpa-0.9.1/simpa_tests/manual_tests/processing_components/QPAIReconstruction.py
+-rw-r--r--   0        0        0     5325 2024-04-02 15:24:14.669688 simpa-0.9.1/simpa_tests/manual_tests/processing_components/TestLinearUnmixingVisual.py
+-rw-r--r--   0        0        0      152 2024-04-02 15:24:14.669688 simpa-0.9.1/simpa_tests/manual_tests/processing_components/__init__.py
+-rw-r--r--   0        0        0    13965 2024-04-02 15:24:14.669688 simpa-0.9.1/simpa_tests/manual_tests/test_with_experimental_measurements/ReproduceDISMeasurements.py
+-rw-r--r--   0        0        0      152 2024-04-02 15:24:14.669688 simpa-0.9.1/simpa_tests/manual_tests/test_with_experimental_measurements/__init__.py
+-rw-r--r--   0        0        0     5969 2024-04-02 15:24:14.669688 simpa-0.9.1/simpa_tests/manual_tests/test_with_experimental_measurements/test_data/background_material_dark.rxt
+-rw-r--r--   0        0        0     7652 2024-04-02 15:24:14.669688 simpa-0.9.1/simpa_tests/manual_tests/test_with_experimental_measurements/test_data/background_material_dark_spectra.npz
+-rw-r--r--   0        0        0     5969 2024-04-02 15:24:14.669688 simpa-0.9.1/simpa_tests/manual_tests/test_with_experimental_measurements/test_data/background_material_light.rxt
+-rw-r--r--   0        0        0     7652 2024-04-02 15:24:14.669688 simpa-0.9.1/simpa_tests/manual_tests/test_with_experimental_measurements/test_data/background_material_light_spectra.npz
+-rw-r--r--   0        0        0     5969 2024-04-02 15:24:14.669688 simpa-0.9.1/simpa_tests/manual_tests/test_with_experimental_measurements/test_data/inclusion_material.rxt
+-rw-r--r--   0        0        0     7652 2024-04-02 15:24:14.669688 simpa-0.9.1/simpa_tests/manual_tests/test_with_experimental_measurements/test_data/inclusion_material_spectra.npz
+-rw-r--r--   0        0        0     1258 2024-04-02 15:24:14.669688 simpa-0.9.1/simpa_tests/manual_tests/test_with_experimental_measurements/utils.py
+-rw-r--r--   0        0        0     5035 2024-04-02 15:24:14.669688 simpa-0.9.1/simpa_tests/manual_tests/volume_creation/SegmentationLoader.py
+-rw-r--r--   0        0        0      152 2024-04-02 15:24:14.669688 simpa-0.9.1/simpa_tests/manual_tests/volume_creation/__init__.py
+-rw-r--r--   0        0        0     5070 2024-04-02 15:24:14.669688 simpa-0.9.1/simpa_tests/test_utils/__init__.py
+-rw-r--r--   0        0        0    46399 2024-04-02 15:24:14.669688 simpa-0.9.1/simpa_tests/test_utils/tissue_composition_tests.py
+-rw-r--r--   0        0        0     2458 2024-04-02 15:24:14.669688 simpa-0.9.1/simpa_tests/test_utils/tissue_models.py
+-rw-r--r--   0        0        0    12141 1970-01-01 00:00:00.000000 simpa-0.9.1/PKG-INFO
```

### Comparing `simpa-0.9.0/LICENSES/MIT` & `simpa-0.9.1/LICENSES/MIT`

 * *Files identical despite different names*

### Comparing `simpa-0.9.0/README.md` & `simpa-0.9.1/README.md`

 * *Files identical despite different names*

### Comparing `simpa-0.9.0/pyproject.toml` & `simpa-0.9.1/pyproject.toml`

 * *Files 4% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 [tool.poetry]
 name = "simpa"
-version = "0.9.0"
+version = "0.9.1"
 description = "Simulation and Image Processing for Photonics and Acoustics"
 authors = [
     "Division of Intelligent Medical Systems (IMSY), DKFZ <k.dreher@dkfz-heidelberg.de>",
     "Janek Groehl <>"]
 license = "MIT"
 readme = "README.md"
 # requires-python = ">=3.7"
@@ -37,15 +37,15 @@
 pacfish = ">=0.4.4"       # Uses BSD-License (MIT compatible)
 requests = ">=2.26.0"        # Uses Apache 2.0-License (MIT compatible)
 wget = ">=3.2"               # Is Public Domain (MIT compatible)
 jdata = ">=0.5.2"            # Uses Apache 2.0-License (MIT compatible)
 pre-commit = ">=3.2.2"       # Uses MIT-License (MIT compatible) 
 
 [tool.poetry.group.docs.dependencies]
-sphinx-rtd-theme = "^1.0.0"
+sphinx-rtd-theme = "^2.0.0"
 Sphinx = "^5.1.1"
 myst-parser = "0.18.0, <1.1"
 
 # autopep8 config
 [tool.autopep8]
 max_line_length = 120
```

### Comparing `simpa-0.9.0/simpa/__init__.py` & `simpa-0.9.1/simpa/__init__.py`

 * *Files identical despite different names*

### Comparing `simpa-0.9.0/simpa/core/__init__.py` & `simpa-0.9.1/simpa/core/__init__.py`

 * *Files identical despite different names*

### Comparing `simpa-0.9.0/simpa/core/device_digital_twins/__init__.py` & `simpa-0.9.1/simpa/core/device_digital_twins/__init__.py`

 * *Files identical despite different names*

### Comparing `simpa-0.9.0/simpa/core/device_digital_twins/detection_geometries/curved_array.py` & `simpa-0.9.1/simpa/core/device_digital_twins/detection_geometries/curved_array.py`

 * *Files identical despite different names*

### Comparing `simpa-0.9.0/simpa/core/device_digital_twins/detection_geometries/detection_geometry_base.py` & `simpa-0.9.1/simpa/core/device_digital_twins/detection_geometries/detection_geometry_base.py`

 * *Files identical despite different names*

### Comparing `simpa-0.9.0/simpa/core/device_digital_twins/detection_geometries/linear_array.py` & `simpa-0.9.1/simpa/core/device_digital_twins/detection_geometries/linear_array.py`

 * *Files identical despite different names*

### Comparing `simpa-0.9.0/simpa/core/device_digital_twins/detection_geometries/planar_array.py` & `simpa-0.9.1/simpa/core/device_digital_twins/detection_geometries/planar_array.py`

 * *Files identical despite different names*

### Comparing `simpa-0.9.0/simpa/core/device_digital_twins/digital_device_twin_base.py` & `simpa-0.9.1/simpa/core/device_digital_twins/digital_device_twin_base.py`

 * *Files identical despite different names*

### Comparing `simpa-0.9.0/simpa/core/device_digital_twins/illumination_geometries/disk_illumination.py` & `simpa-0.9.1/simpa/core/device_digital_twins/illumination_geometries/disk_illumination.py`

 * *Files identical despite different names*

### Comparing `simpa-0.9.0/simpa/core/device_digital_twins/illumination_geometries/gaussian_beam_illumination.py` & `simpa-0.9.1/simpa/core/device_digital_twins/illumination_geometries/gaussian_beam_illumination.py`

 * *Files identical despite different names*

### Comparing `simpa-0.9.0/simpa/core/device_digital_twins/illumination_geometries/illumination_geometry_base.py` & `simpa-0.9.1/simpa/core/device_digital_twins/illumination_geometries/illumination_geometry_base.py`

 * *Files identical despite different names*

### Comparing `simpa-0.9.0/simpa/core/device_digital_twins/illumination_geometries/ithera_msot_acuity_illumination.py` & `simpa-0.9.1/simpa/core/device_digital_twins/illumination_geometries/ithera_msot_acuity_illumination.py`

 * *Files identical despite different names*

### Comparing `simpa-0.9.0/simpa/core/device_digital_twins/illumination_geometries/ithera_msot_invision_illumination.py` & `simpa-0.9.1/simpa/core/device_digital_twins/illumination_geometries/ithera_msot_invision_illumination.py`

 * *Files identical despite different names*

### Comparing `simpa-0.9.0/simpa/core/device_digital_twins/illumination_geometries/pencil_array_illumination.py` & `simpa-0.9.1/simpa/core/device_digital_twins/illumination_geometries/pencil_array_illumination.py`

 * *Files identical despite different names*

### Comparing `simpa-0.9.0/simpa/core/device_digital_twins/illumination_geometries/pencil_beam_illumination.py` & `simpa-0.9.1/simpa/core/device_digital_twins/illumination_geometries/pencil_beam_illumination.py`

 * *Files identical despite different names*

### Comparing `simpa-0.9.0/simpa/core/device_digital_twins/illumination_geometries/slit_illumination.py` & `simpa-0.9.1/simpa/core/device_digital_twins/illumination_geometries/slit_illumination.py`

 * *Files identical despite different names*

### Comparing `simpa-0.9.0/simpa/core/device_digital_twins/pa_devices/ithera_msot_acuity.py` & `simpa-0.9.1/simpa/core/device_digital_twins/pa_devices/ithera_msot_acuity.py`

 * *Files identical despite different names*

### Comparing `simpa-0.9.0/simpa/core/device_digital_twins/pa_devices/ithera_msot_invision.py` & `simpa-0.9.1/simpa/core/device_digital_twins/pa_devices/ithera_msot_invision.py`

 * *Files identical despite different names*

### Comparing `simpa-0.9.0/simpa/core/device_digital_twins/pa_devices/ithera_rsom.py` & `simpa-0.9.1/simpa/core/device_digital_twins/pa_devices/ithera_rsom.py`

 * *Files identical despite different names*

### Comparing `simpa-0.9.0/simpa/core/processing_components/__init__.py` & `simpa-0.9.1/simpa/core/processing_components/__init__.py`

 * *Files identical despite different names*

### Comparing `simpa-0.9.0/simpa/core/processing_components/monospectral/field_of_view_cropping.py` & `simpa-0.9.1/simpa/core/processing_components/monospectral/field_of_view_cropping.py`

 * *Files identical despite different names*

### Comparing `simpa-0.9.0/simpa/core/processing_components/monospectral/iterative_qPAI_algorithm.py` & `simpa-0.9.1/simpa/core/processing_components/monospectral/iterative_qPAI_algorithm.py`

 * *Files identical despite different names*

### Comparing `simpa-0.9.0/simpa/core/processing_components/monospectral/noise/gamma_noise.py` & `simpa-0.9.1/simpa/core/processing_components/monospectral/noise/gamma_noise.py`

 * *Files identical despite different names*

### Comparing `simpa-0.9.0/simpa/core/processing_components/monospectral/noise/gaussian_noise.py` & `simpa-0.9.1/simpa/core/processing_components/monospectral/noise/gaussian_noise.py`

 * *Files identical despite different names*

### Comparing `simpa-0.9.0/simpa/core/processing_components/monospectral/noise/poisson_noise.py` & `simpa-0.9.1/simpa/core/processing_components/monospectral/noise/poisson_noise.py`

 * *Files identical despite different names*

### Comparing `simpa-0.9.0/simpa/core/processing_components/monospectral/noise/salt_and_pepper_noise.py` & `simpa-0.9.1/simpa/core/processing_components/monospectral/noise/salt_and_pepper_noise.py`

 * *Files identical despite different names*

### Comparing `simpa-0.9.0/simpa/core/processing_components/monospectral/noise/uniform_noise.py` & `simpa-0.9.1/simpa/core/processing_components/monospectral/noise/uniform_noise.py`

 * *Files identical despite different names*

### Comparing `simpa-0.9.0/simpa/core/processing_components/multispectral/__init__.py` & `simpa-0.9.1/simpa/core/processing_components/multispectral/__init__.py`

 * *Files identical despite different names*

### Comparing `simpa-0.9.0/simpa/core/processing_components/multispectral/linear_unmixing.py` & `simpa-0.9.1/simpa/core/processing_components/multispectral/linear_unmixing.py`

 * *Files identical despite different names*

### Comparing `simpa-0.9.0/simpa/core/simulation.py` & `simpa-0.9.1/simpa/core/simulation.py`

 * *Files identical despite different names*

### Comparing `simpa-0.9.0/simpa/core/simulation_modules/acoustic_forward_module/__init__.py` & `simpa-0.9.1/simpa/core/simulation_modules/acoustic_forward_module/__init__.py`

 * *Files identical despite different names*

### Comparing `simpa-0.9.0/simpa/core/simulation_modules/acoustic_forward_module/acoustic_forward_model_test_adapter.py` & `simpa-0.9.1/simpa/core/simulation_modules/acoustic_forward_module/acoustic_forward_model_test_adapter.py`

 * *Files identical despite different names*

### Comparing `simpa-0.9.0/simpa/core/simulation_modules/acoustic_forward_module/acoustic_forward_module_k_wave_adapter.py` & `simpa-0.9.1/simpa/core/simulation_modules/acoustic_forward_module/acoustic_forward_module_k_wave_adapter.py`

 * *Files identical despite different names*

### Comparing `simpa-0.9.0/simpa/core/simulation_modules/acoustic_forward_module/simulate_2D.m` & `simpa-0.9.1/simpa/core/simulation_modules/acoustic_forward_module/simulate_2D.m`

 * *Files identical despite different names*

### Comparing `simpa-0.9.0/simpa/core/simulation_modules/acoustic_forward_module/simulate_3D.m` & `simpa-0.9.1/simpa/core/simulation_modules/acoustic_forward_module/simulate_3D.m`

 * *Files identical despite different names*

### Comparing `simpa-0.9.0/simpa/core/simulation_modules/optical_simulation_module/__init__.py` & `simpa-0.9.1/simpa/core/simulation_modules/optical_simulation_module/__init__.py`

 * *Files identical despite different names*

### Comparing `simpa-0.9.0/simpa/core/simulation_modules/optical_simulation_module/optical_forward_model_mcx_adapter.py` & `simpa-0.9.1/simpa/core/simulation_modules/optical_simulation_module/optical_forward_model_mcx_adapter.py`

 * *Files identical despite different names*

### Comparing `simpa-0.9.0/simpa/core/simulation_modules/optical_simulation_module/optical_forward_model_mcx_reflectance_adapter.py` & `simpa-0.9.1/simpa/core/simulation_modules/optical_simulation_module/optical_forward_model_mcx_reflectance_adapter.py`

 * *Files identical despite different names*

### Comparing `simpa-0.9.0/simpa/core/simulation_modules/optical_simulation_module/optical_forward_model_test_adapter.py` & `simpa-0.9.1/simpa/core/simulation_modules/optical_simulation_module/optical_forward_model_test_adapter.py`

 * *Files identical despite different names*

### Comparing `simpa-0.9.0/simpa/core/simulation_modules/reconstruction_module/__init__.py` & `simpa-0.9.1/simpa/core/simulation_modules/reconstruction_module/__init__.py`

 * *Files identical despite different names*

### Comparing `simpa-0.9.0/simpa/core/simulation_modules/reconstruction_module/reconstruction_module_delay_and_sum_adapter.py` & `simpa-0.9.1/simpa/core/simulation_modules/reconstruction_module/reconstruction_module_delay_and_sum_adapter.py`

 * *Files identical despite different names*

### Comparing `simpa-0.9.0/simpa/core/simulation_modules/reconstruction_module/reconstruction_module_delay_multiply_and_sum_adapter.py` & `simpa-0.9.1/simpa/core/simulation_modules/reconstruction_module/reconstruction_module_delay_multiply_and_sum_adapter.py`

 * *Files identical despite different names*

### Comparing `simpa-0.9.0/simpa/core/simulation_modules/reconstruction_module/reconstruction_module_signed_delay_multiply_and_sum_adapter.py` & `simpa-0.9.1/simpa/core/simulation_modules/reconstruction_module/reconstruction_module_signed_delay_multiply_and_sum_adapter.py`

 * *Files identical despite different names*

### Comparing `simpa-0.9.0/simpa/core/simulation_modules/reconstruction_module/reconstruction_module_time_reversal_adapter.py` & `simpa-0.9.1/simpa/core/simulation_modules/reconstruction_module/reconstruction_module_time_reversal_adapter.py`

 * *Files identical despite different names*

### Comparing `simpa-0.9.0/simpa/core/simulation_modules/reconstruction_module/reconstruction_utils.py` & `simpa-0.9.1/simpa/core/simulation_modules/reconstruction_module/reconstruction_utils.py`

 * *Files identical despite different names*

### Comparing `simpa-0.9.0/simpa/core/simulation_modules/reconstruction_module/time_reversal_2D.m` & `simpa-0.9.1/simpa/core/simulation_modules/reconstruction_module/time_reversal_2D.m`

 * *Files identical despite different names*

### Comparing `simpa-0.9.0/simpa/core/simulation_modules/reconstruction_module/time_reversal_3D.m` & `simpa-0.9.1/simpa/core/simulation_modules/reconstruction_module/time_reversal_3D.m`

 * *Files identical despite different names*

### Comparing `simpa-0.9.0/simpa/core/simulation_modules/volume_creation_module/__init__.py` & `simpa-0.9.1/simpa/core/simulation_modules/volume_creation_module/__init__.py`

 * *Files identical despite different names*

### Comparing `simpa-0.9.0/simpa/core/simulation_modules/volume_creation_module/volume_creation_module_model_based_adapter.py` & `simpa-0.9.1/simpa/core/simulation_modules/volume_creation_module/volume_creation_module_model_based_adapter.py`

 * *Files identical despite different names*

### Comparing `simpa-0.9.0/simpa/core/simulation_modules/volume_creation_module/volume_creation_module_segmentation_based_adapter.py` & `simpa-0.9.1/simpa/core/simulation_modules/volume_creation_module/volume_creation_module_segmentation_based_adapter.py`

 * *Files 11% similar despite different names*

```diff
@@ -3,14 +3,15 @@
 # SPDX-License-Identifier: MIT
 
 from simpa.core.simulation_modules.volume_creation_module import VolumeCreatorModuleBase
 from simpa.utils import Tags
 from simpa.utils.constants import property_tags
 from simpa.io_handling import save_hdf5
 import numpy as np
+import torch
 
 
 class SegmentationBasedVolumeCreationAdapter(VolumeCreatorModuleBase):
     """
     This volume creator expects a np.ndarray to be in the settigs
     under the Tags.INPUT_SEGMENTATION_VOLUME tag and uses this array
     together with a SegmentationClass mapping which is a dict defined in
@@ -38,12 +39,19 @@
                              .format(z_dim_px, z_dim_seg_px))
 
         class_mapping = self.component_settings[Tags.SEGMENTATION_CLASS_MAPPING]
 
         for seg_class in segmentation_classes:
             class_properties = class_mapping[seg_class].get_properties_for_wavelength(wavelength)
             for prop_tag in property_tags:
-                volumes[prop_tag][segmentation_volume == seg_class] = class_properties[prop_tag]
+                assigned_prop = class_properties[prop_tag]
+                if assigned_prop is None:
+                    assigned_prop = torch.nan
+                volumes[prop_tag][segmentation_volume == seg_class] = assigned_prop
 
         save_hdf5(self.global_settings, self.global_settings[Tags.SIMPA_OUTPUT_PATH], "/settings/")
 
+        # convert volumes back to CPU
+        for key in volumes.keys():
+            volumes[key] = volumes[key].cpu().numpy().astype(np.float64, copy=False)
+
         return volumes
```

### Comparing `simpa-0.9.0/simpa/io_handling/io_hdf5.py` & `simpa-0.9.1/simpa/io_handling/io_hdf5.py`

 * *Files identical despite different names*

### Comparing `simpa-0.9.0/simpa/io_handling/ipasc.py` & `simpa-0.9.1/simpa/io_handling/ipasc.py`

 * *Files identical despite different names*

### Comparing `simpa-0.9.0/simpa/io_handling/serialization.py` & `simpa-0.9.1/simpa/io_handling/serialization.py`

 * *Files identical despite different names*

### Comparing `simpa-0.9.0/simpa/io_handling/zenodo_download.py` & `simpa-0.9.1/simpa/io_handling/zenodo_download.py`

 * *Files identical despite different names*

### Comparing `simpa-0.9.0/simpa/log/file_logger.py` & `simpa-0.9.1/simpa/log/file_logger.py`

 * *Files identical despite different names*

### Comparing `simpa-0.9.0/simpa/utils/__init__.py` & `simpa-0.9.1/simpa/utils/__init__.py`

 * *Files identical despite different names*

### Comparing `simpa-0.9.0/simpa/utils/calculate.py` & `simpa-0.9.1/simpa/utils/calculate.py`

 * *Files identical despite different names*

### Comparing `simpa-0.9.0/simpa/utils/constants.py` & `simpa-0.9.1/simpa/utils/constants.py`

 * *Files identical despite different names*

### Comparing `simpa-0.9.0/simpa/utils/deformation_manager.py` & `simpa-0.9.1/simpa/utils/deformation_manager.py`

 * *Files identical despite different names*

### Comparing `simpa-0.9.0/simpa/utils/dict_path_manager.py` & `simpa-0.9.1/simpa/utils/dict_path_manager.py`

 * *Files identical despite different names*

### Comparing `simpa-0.9.0/simpa/utils/libraries/absorption_spectra_data/Copper_Sulphide.npz` & `simpa-0.9.1/simpa/utils/libraries/absorption_spectra_data/Copper_Sulphide.npz`

 * *Files identical despite different names*

### Comparing `simpa-0.9.0/simpa/utils/libraries/absorption_spectra_data/Deoxyhemoglobin.npz` & `simpa-0.9.1/simpa/utils/libraries/absorption_spectra_data/Deoxyhemoglobin.npz`

 * *Files identical despite different names*

### Comparing `simpa-0.9.0/simpa/utils/libraries/absorption_spectra_data/Fat.npz` & `simpa-0.9.1/simpa/utils/libraries/absorption_spectra_data/Fat.npz`

 * *Files identical despite different names*

### Comparing `simpa-0.9.0/simpa/utils/libraries/absorption_spectra_data/Melanin.npz` & `simpa-0.9.1/simpa/utils/libraries/absorption_spectra_data/Melanin.npz`

 * *Files identical despite different names*

### Comparing `simpa-0.9.0/simpa/utils/libraries/absorption_spectra_data/Nickel_Sulphide.npz` & `simpa-0.9.1/simpa/utils/libraries/absorption_spectra_data/Nickel_Sulphide.npz`

 * *Files identical despite different names*

### Comparing `simpa-0.9.0/simpa/utils/libraries/absorption_spectra_data/Oxyhemoglobin.npz` & `simpa-0.9.1/simpa/utils/libraries/absorption_spectra_data/Oxyhemoglobin.npz`

 * *Files identical despite different names*

### Comparing `simpa-0.9.0/simpa/utils/libraries/absorption_spectra_data/Skin_Baseline.npz` & `simpa-0.9.1/simpa/utils/libraries/absorption_spectra_data/Skin_Baseline.npz`

 * *Files identical despite different names*

### Comparing `simpa-0.9.0/simpa/utils/libraries/absorption_spectra_data/Water.npz` & `simpa-0.9.1/simpa/utils/libraries/absorption_spectra_data/Water.npz`

 * *Files identical despite different names*

### Comparing `simpa-0.9.0/simpa/utils/libraries/anisotropy_spectra_data/Epidermis_Anisotropy.npz` & `simpa-0.9.1/simpa/utils/libraries/anisotropy_spectra_data/Epidermis_Anisotropy.npz`

 * *Files identical despite different names*

### Comparing `simpa-0.9.0/simpa/utils/libraries/literature_values.py` & `simpa-0.9.1/simpa/utils/libraries/literature_values.py`

 * *Files identical despite different names*

### Comparing `simpa-0.9.0/simpa/utils/libraries/molecule_library.py` & `simpa-0.9.1/simpa/utils/libraries/molecule_library.py`

 * *Files identical despite different names*

### Comparing `simpa-0.9.0/simpa/utils/libraries/scattering_spectra_data/background_scattering.npz` & `simpa-0.9.1/simpa/utils/libraries/scattering_spectra_data/background_scattering.npz`

 * *Files identical despite different names*

### Comparing `simpa-0.9.0/simpa/utils/libraries/scattering_spectra_data/blood_scattering.npz` & `simpa-0.9.1/simpa/utils/libraries/scattering_spectra_data/blood_scattering.npz`

 * *Files identical despite different names*

### Comparing `simpa-0.9.0/simpa/utils/libraries/scattering_spectra_data/bone_scattering.npz` & `simpa-0.9.1/simpa/utils/libraries/scattering_spectra_data/bone_scattering.npz`

 * *Files identical despite different names*

### Comparing `simpa-0.9.0/simpa/utils/libraries/scattering_spectra_data/fat_scattering.npz` & `simpa-0.9.1/simpa/utils/libraries/scattering_spectra_data/fat_scattering.npz`

 * *Files identical despite different names*

### Comparing `simpa-0.9.0/simpa/utils/libraries/scattering_spectra_data/muscle_scattering.npz` & `simpa-0.9.1/simpa/utils/libraries/scattering_spectra_data/muscle_scattering.npz`

 * *Files identical despite different names*

### Comparing `simpa-0.9.0/simpa/utils/libraries/spectrum_library.py` & `simpa-0.9.1/simpa/utils/libraries/spectrum_library.py`

 * *Files identical despite different names*

### Comparing `simpa-0.9.0/simpa/utils/libraries/structure_library/BackgroundStructure.py` & `simpa-0.9.1/simpa/utils/libraries/structure_library/BackgroundStructure.py`

 * *Files identical despite different names*

### Comparing `simpa-0.9.0/simpa/utils/libraries/structure_library/CircularTubularStructure.py` & `simpa-0.9.1/simpa/utils/libraries/structure_library/CircularTubularStructure.py`

 * *Files identical despite different names*

### Comparing `simpa-0.9.0/simpa/utils/libraries/structure_library/EllipticalTubularStructure.py` & `simpa-0.9.1/simpa/utils/libraries/structure_library/EllipticalTubularStructure.py`

 * *Files identical despite different names*

### Comparing `simpa-0.9.0/simpa/utils/libraries/structure_library/HorizontalLayerStructure.py` & `simpa-0.9.1/simpa/utils/libraries/structure_library/HorizontalLayerStructure.py`

 * *Files identical despite different names*

### Comparing `simpa-0.9.0/simpa/utils/libraries/structure_library/ParallelepipedStructure.py` & `simpa-0.9.1/simpa/utils/libraries/structure_library/ParallelepipedStructure.py`

 * *Files identical despite different names*

### Comparing `simpa-0.9.0/simpa/utils/libraries/structure_library/RectangularCuboidStructure.py` & `simpa-0.9.1/simpa/utils/libraries/structure_library/RectangularCuboidStructure.py`

 * *Files identical despite different names*

### Comparing `simpa-0.9.0/simpa/utils/libraries/structure_library/SphericalStructure.py` & `simpa-0.9.1/simpa/utils/libraries/structure_library/SphericalStructure.py`

 * *Files identical despite different names*

### Comparing `simpa-0.9.0/simpa/utils/libraries/structure_library/StructureBase.py` & `simpa-0.9.1/simpa/utils/libraries/structure_library/StructureBase.py`

 * *Files identical despite different names*

### Comparing `simpa-0.9.0/simpa/utils/libraries/structure_library/VesselStructure.py` & `simpa-0.9.1/simpa/utils/libraries/structure_library/VesselStructure.py`

 * *Files identical despite different names*

### Comparing `simpa-0.9.0/simpa/utils/libraries/structure_library/__init__.py` & `simpa-0.9.1/simpa/utils/libraries/structure_library/__init__.py`

 * *Files identical despite different names*

### Comparing `simpa-0.9.0/simpa/utils/libraries/tissue_library.py` & `simpa-0.9.1/simpa/utils/libraries/tissue_library.py`

 * *Files identical despite different names*

### Comparing `simpa-0.9.0/simpa/utils/matlab.py` & `simpa-0.9.1/simpa/utils/matlab.py`

 * *Files identical despite different names*

### Comparing `simpa-0.9.0/simpa/utils/path_manager.py` & `simpa-0.9.1/simpa/utils/path_manager.py`

 * *Files identical despite different names*

### Comparing `simpa-0.9.0/simpa/utils/processing_device.py` & `simpa-0.9.1/simpa/utils/processing_device.py`

 * *Files identical despite different names*

### Comparing `simpa-0.9.0/simpa/utils/quality_assurance/data_sanity_testing.py` & `simpa-0.9.1/simpa/utils/quality_assurance/data_sanity_testing.py`

 * *Files identical despite different names*

### Comparing `simpa-0.9.0/simpa/utils/settings.py` & `simpa-0.9.1/simpa/utils/settings.py`

 * *Files identical despite different names*

### Comparing `simpa-0.9.0/simpa/utils/tags.py` & `simpa-0.9.1/simpa/utils/tags.py`

 * *Files identical despite different names*

### Comparing `simpa-0.9.0/simpa/utils/tissue_properties.py` & `simpa-0.9.1/simpa/utils/tissue_properties.py`

 * *Files identical despite different names*

### Comparing `simpa-0.9.0/simpa/visualisation/matplotlib_data_visualisation.py` & `simpa-0.9.1/simpa/visualisation/matplotlib_data_visualisation.py`

 * *Files identical despite different names*

### Comparing `simpa-0.9.0/simpa/visualisation/matplotlib_device_visualisation.py` & `simpa-0.9.1/simpa/visualisation/matplotlib_device_visualisation.py`

 * *Files identical despite different names*

### Comparing `simpa-0.9.0/simpa_tests/__init__.py` & `simpa-0.9.1/simpa_tests/__init__.py`

 * *Files identical despite different names*

### Comparing `simpa-0.9.0/simpa_tests/automatic_tests/device_tests/test_curved_array.py` & `simpa-0.9.1/simpa_tests/automatic_tests/device_tests/test_curved_array.py`

 * *Files identical despite different names*

### Comparing `simpa-0.9.0/simpa_tests/automatic_tests/device_tests/test_field_of_view.py` & `simpa-0.9.1/simpa_tests/automatic_tests/device_tests/test_field_of_view.py`

 * *Files identical despite different names*

### Comparing `simpa-0.9.0/simpa_tests/automatic_tests/device_tests/test_linear_array.py` & `simpa-0.9.1/simpa_tests/automatic_tests/device_tests/test_linear_array.py`

 * *Files identical despite different names*

### Comparing `simpa-0.9.0/simpa_tests/automatic_tests/structure_tests/test_boxes.py` & `simpa-0.9.1/simpa_tests/automatic_tests/structure_tests/test_boxes.py`

 * *Files identical despite different names*

### Comparing `simpa-0.9.0/simpa_tests/automatic_tests/structure_tests/test_elliptical_tubes.py` & `simpa-0.9.1/simpa_tests/automatic_tests/structure_tests/test_elliptical_tubes.py`

 * *Files identical despite different names*

### Comparing `simpa-0.9.0/simpa_tests/automatic_tests/structure_tests/test_layers.py` & `simpa-0.9.1/simpa_tests/automatic_tests/structure_tests/test_layers.py`

 * *Files identical despite different names*

### Comparing `simpa-0.9.0/simpa_tests/automatic_tests/structure_tests/test_parallel_epipeds.py` & `simpa-0.9.1/simpa_tests/automatic_tests/structure_tests/test_parallel_epipeds.py`

 * *Files identical despite different names*

### Comparing `simpa-0.9.0/simpa_tests/automatic_tests/structure_tests/test_spheres.py` & `simpa-0.9.1/simpa_tests/automatic_tests/structure_tests/test_spheres.py`

 * *Files identical despite different names*

### Comparing `simpa-0.9.0/simpa_tests/automatic_tests/structure_tests/test_tubes.py` & `simpa-0.9.1/simpa_tests/automatic_tests/structure_tests/test_tubes.py`

 * *Files identical despite different names*

### Comparing `simpa-0.9.0/simpa_tests/automatic_tests/structure_tests/test_vesseltree.py` & `simpa-0.9.1/simpa_tests/automatic_tests/structure_tests/test_vesseltree.py`

 * *Files identical despite different names*

### Comparing `simpa-0.9.0/simpa_tests/automatic_tests/test_IPASC_export.py` & `simpa-0.9.1/simpa_tests/automatic_tests/test_IPASC_export.py`

 * *Files identical despite different names*

### Comparing `simpa-0.9.0/simpa_tests/automatic_tests/test_bandpass_filter.py` & `simpa-0.9.1/simpa_tests/automatic_tests/test_bandpass_filter.py`

 * *Files identical despite different names*

### Comparing `simpa-0.9.0/simpa_tests/automatic_tests/test_calculation_utils.py` & `simpa-0.9.1/simpa_tests/automatic_tests/test_calculation_utils.py`

 * *Files identical despite different names*

### Comparing `simpa-0.9.0/simpa_tests/automatic_tests/test_create_a_volume.py` & `simpa-0.9.1/simpa_tests/automatic_tests/test_create_a_volume.py`

 * *Files identical despite different names*

### Comparing `simpa-0.9.0/simpa_tests/automatic_tests/test_device_UUID.py` & `simpa-0.9.1/simpa_tests/automatic_tests/test_device_UUID.py`

 * *Files identical despite different names*

### Comparing `simpa-0.9.0/simpa_tests/automatic_tests/test_io_handling.py` & `simpa-0.9.1/simpa_tests/automatic_tests/test_io_handling.py`

 * *Files identical despite different names*

### Comparing `simpa-0.9.0/simpa_tests/automatic_tests/test_linear_unmixing.py` & `simpa-0.9.1/simpa_tests/automatic_tests/test_linear_unmixing.py`

 * *Files identical despite different names*

### Comparing `simpa-0.9.0/simpa_tests/automatic_tests/test_logging.py` & `simpa-0.9.1/simpa_tests/automatic_tests/test_logging.py`

 * *Files identical despite different names*

### Comparing `simpa-0.9.0/simpa_tests/automatic_tests/test_noise_models.py` & `simpa-0.9.1/simpa_tests/automatic_tests/test_noise_models.py`

 * *Files identical despite different names*

### Comparing `simpa-0.9.0/simpa_tests/automatic_tests/test_path_manager.py` & `simpa-0.9.1/simpa_tests/automatic_tests/test_path_manager.py`

 * *Files identical despite different names*

### Comparing `simpa-0.9.0/simpa_tests/automatic_tests/test_pipeline.py` & `simpa-0.9.1/simpa_tests/automatic_tests/test_pipeline.py`

 * *Files identical despite different names*

### Comparing `simpa-0.9.0/simpa_tests/automatic_tests/test_processing.py` & `simpa-0.9.1/simpa_tests/automatic_tests/test_processing.py`

 * *Files identical despite different names*

### Comparing `simpa-0.9.0/simpa_tests/automatic_tests/test_processing_device.py` & `simpa-0.9.1/simpa_tests/automatic_tests/test_processing_device.py`

 * *Files identical despite different names*

### Comparing `simpa-0.9.0/simpa_tests/automatic_tests/test_quality_assurance.py` & `simpa-0.9.1/simpa_tests/automatic_tests/test_quality_assurance.py`

 * *Files identical despite different names*

### Comparing `simpa-0.9.0/simpa_tests/automatic_tests/tissue_library/test_core_assumptions.py` & `simpa-0.9.1/simpa_tests/automatic_tests/tissue_library/test_core_assumptions.py`

 * *Files identical despite different names*

### Comparing `simpa-0.9.0/simpa_tests/automatic_tests/tissue_library/test_spectra_can_be_found.py` & `simpa-0.9.1/simpa_tests/automatic_tests/tissue_library/test_spectra_can_be_found.py`

 * *Files identical despite different names*

### Comparing `simpa-0.9.0/simpa_tests/automatic_tests/tissue_library/test_tissue_library_against_literature_values.py` & `simpa-0.9.1/simpa_tests/automatic_tests/tissue_library/test_tissue_library_against_literature_values.py`

 * *Files identical despite different names*

### Comparing `simpa-0.9.0/simpa_tests/checklists/release_checklist.md` & `simpa-0.9.1/simpa_tests/checklists/release_checklist.md`

 * *Files identical despite different names*

### Comparing `simpa-0.9.0/simpa_tests/do_coverage.py` & `simpa-0.9.1/simpa_tests/do_coverage.py`

 * *Files identical despite different names*

### Comparing `simpa-0.9.0/simpa_tests/full_integration_test.bat` & `simpa-0.9.1/simpa_tests/full_integration_test.bat`

 * *Files identical despite different names*

### Comparing `simpa-0.9.0/simpa_tests/manual_tests/__init__.py` & `simpa-0.9.1/simpa_tests/manual_tests/__init__.py`

 * *Files identical despite different names*

### Comparing `simpa-0.9.0/simpa_tests/manual_tests/acoustic_forward_models/KWaveAcousticForwardConvenienceFunction.py` & `simpa-0.9.1/simpa_tests/manual_tests/acoustic_forward_models/KWaveAcousticForwardConvenienceFunction.py`

 * *Files identical despite different names*

### Comparing `simpa-0.9.0/simpa_tests/manual_tests/acoustic_forward_models/MinimalKWaveTest.py` & `simpa-0.9.1/simpa_tests/manual_tests/acoustic_forward_models/MinimalKWaveTest.py`

 * *Files identical despite different names*

### Comparing `simpa-0.9.0/simpa_tests/manual_tests/digital_device_twins/SimulationWithMSOTInvision.py` & `simpa-0.9.1/simpa_tests/manual_tests/digital_device_twins/SimulationWithMSOTInvision.py`

 * *Files identical despite different names*

### Comparing `simpa-0.9.0/simpa_tests/manual_tests/digital_device_twins/VisualiseDevices.py` & `simpa-0.9.1/simpa_tests/manual_tests/digital_device_twins/VisualiseDevices.py`

 * *Files identical despite different names*

### Comparing `simpa-0.9.0/simpa_tests/manual_tests/image_reconstruction/DelayAndSumReconstruction.py` & `simpa-0.9.1/simpa_tests/manual_tests/image_reconstruction/DelayAndSumReconstruction.py`

 * *Files identical despite different names*

### Comparing `simpa-0.9.0/simpa_tests/manual_tests/image_reconstruction/DelayMultiplyAndSumReconstruction.py` & `simpa-0.9.1/simpa_tests/manual_tests/image_reconstruction/DelayMultiplyAndSumReconstruction.py`

 * *Files identical despite different names*

### Comparing `simpa-0.9.0/simpa_tests/manual_tests/image_reconstruction/PointSourceReconstruction.py` & `simpa-0.9.1/simpa_tests/manual_tests/image_reconstruction/PointSourceReconstruction.py`

 * *Files identical despite different names*

### Comparing `simpa-0.9.0/simpa_tests/manual_tests/image_reconstruction/SignedDelayMultiplyAndSumReconstruction.py` & `simpa-0.9.1/simpa_tests/manual_tests/image_reconstruction/SignedDelayMultiplyAndSumReconstruction.py`

 * *Files identical despite different names*

### Comparing `simpa-0.9.0/simpa_tests/manual_tests/image_reconstruction/TimeReversalReconstruction.py` & `simpa-0.9.1/simpa_tests/manual_tests/image_reconstruction/TimeReversalReconstruction.py`

 * *Files identical despite different names*

### Comparing `simpa-0.9.0/simpa_tests/manual_tests/optical_forward_models/AbsorptionAndScatteringWithInifinitesimalSlabExperiment.py` & `simpa-0.9.1/simpa_tests/manual_tests/optical_forward_models/AbsorptionAndScatteringWithInifinitesimalSlabExperiment.py`

 * *Files identical despite different names*

### Comparing `simpa-0.9.0/simpa_tests/manual_tests/optical_forward_models/AbsorptionAndScatteringWithinHomogenousMedium.py` & `simpa-0.9.1/simpa_tests/manual_tests/optical_forward_models/AbsorptionAndScatteringWithinHomogenousMedium.py`

 * *Files identical despite different names*

### Comparing `simpa-0.9.0/simpa_tests/manual_tests/optical_forward_models/CompareMCXResultsWithDiffusionTheory.py` & `simpa-0.9.1/simpa_tests/manual_tests/optical_forward_models/CompareMCXResultsWithDiffusionTheory.py`

 * *Files identical despite different names*

### Comparing `simpa-0.9.0/simpa_tests/manual_tests/optical_forward_models/ComputeDiffuseReflectance.py` & `simpa-0.9.1/simpa_tests/manual_tests/optical_forward_models/ComputeDiffuseReflectance.py`

 * *Files identical despite different names*

### Comparing `simpa-0.9.0/simpa_tests/manual_tests/processing_components/QPAIReconstruction.py` & `simpa-0.9.1/simpa_tests/manual_tests/processing_components/QPAIReconstruction.py`

 * *Files identical despite different names*

### Comparing `simpa-0.9.0/simpa_tests/manual_tests/processing_components/TestLinearUnmixingVisual.py` & `simpa-0.9.1/simpa_tests/manual_tests/processing_components/TestLinearUnmixingVisual.py`

 * *Files identical despite different names*

### Comparing `simpa-0.9.0/simpa_tests/manual_tests/test_with_experimental_measurements/ReproduceDISMeasurements.py` & `simpa-0.9.1/simpa_tests/manual_tests/test_with_experimental_measurements/ReproduceDISMeasurements.py`

 * *Files identical despite different names*

### Comparing `simpa-0.9.0/simpa_tests/manual_tests/test_with_experimental_measurements/test_data/background_material_dark.rxt` & `simpa-0.9.1/simpa_tests/manual_tests/test_with_experimental_measurements/test_data/background_material_dark.rxt`

 * *Files identical despite different names*

### Comparing `simpa-0.9.0/simpa_tests/manual_tests/test_with_experimental_measurements/test_data/background_material_dark_spectra.npz` & `simpa-0.9.1/simpa_tests/manual_tests/test_with_experimental_measurements/test_data/background_material_dark_spectra.npz`

 * *Files identical despite different names*

### Comparing `simpa-0.9.0/simpa_tests/manual_tests/test_with_experimental_measurements/test_data/background_material_light.rxt` & `simpa-0.9.1/simpa_tests/manual_tests/test_with_experimental_measurements/test_data/background_material_light.rxt`

 * *Files identical despite different names*

### Comparing `simpa-0.9.0/simpa_tests/manual_tests/test_with_experimental_measurements/test_data/background_material_light_spectra.npz` & `simpa-0.9.1/simpa_tests/manual_tests/test_with_experimental_measurements/test_data/background_material_light_spectra.npz`

 * *Files identical despite different names*

### Comparing `simpa-0.9.0/simpa_tests/manual_tests/test_with_experimental_measurements/test_data/inclusion_material.rxt` & `simpa-0.9.1/simpa_tests/manual_tests/test_with_experimental_measurements/test_data/inclusion_material.rxt`

 * *Files identical despite different names*

### Comparing `simpa-0.9.0/simpa_tests/manual_tests/test_with_experimental_measurements/test_data/inclusion_material_spectra.npz` & `simpa-0.9.1/simpa_tests/manual_tests/test_with_experimental_measurements/test_data/inclusion_material_spectra.npz`

 * *Files identical despite different names*

### Comparing `simpa-0.9.0/simpa_tests/manual_tests/test_with_experimental_measurements/utils.py` & `simpa-0.9.1/simpa_tests/manual_tests/test_with_experimental_measurements/utils.py`

 * *Files identical despite different names*

### Comparing `simpa-0.9.0/simpa_tests/manual_tests/volume_creation/SegmentationLoader.py` & `simpa-0.9.1/simpa_tests/manual_tests/volume_creation/SegmentationLoader.py`

 * *Files identical despite different names*

### Comparing `simpa-0.9.0/simpa_tests/test_utils/__init__.py` & `simpa-0.9.1/simpa_tests/test_utils/__init__.py`

 * *Files identical despite different names*

### Comparing `simpa-0.9.0/simpa_tests/test_utils/tissue_composition_tests.py` & `simpa-0.9.1/simpa_tests/test_utils/tissue_composition_tests.py`

 * *Files identical despite different names*

### Comparing `simpa-0.9.0/simpa_tests/test_utils/tissue_models.py` & `simpa-0.9.1/simpa_tests/test_utils/tissue_models.py`

 * *Files identical despite different names*

### Comparing `simpa-0.9.0/PKG-INFO` & `simpa-0.9.1/PKG-INFO`

 * *Files 0% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: simpa
-Version: 0.9.0
+Version: 0.9.1
 Summary: Simulation and Image Processing for Photonics and Acoustics
 Home-page: https://github.com/IMSY-DKFZ/simpa
 License: MIT
 Keywords: simulation,photonics,acoustics
 Author: Division of Intelligent Medical Systems (IMSY), DKFZ
 Author-email: k.dreher@dkfz-heidelberg.de
 Requires-Python: >=3.8
```

