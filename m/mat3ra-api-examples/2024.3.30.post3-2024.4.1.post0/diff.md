# Comparing `tmp/mat3ra-api-examples-2024.3.30.post3.tar.gz` & `tmp/mat3ra-api-examples-2024.4.1.post0.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "mat3ra-api-examples-2024.3.30.post3.tar", last modified: Sat Mar 30 03:47:22 2024, max compression
+gzip compressed data, was "mat3ra-api-examples-2024.4.1.post0.tar", last modified: Mon Apr  1 22:44:12 2024, max compression
```

## Comparing `mat3ra-api-examples-2024.3.30.post3.tar` & `mat3ra-api-examples-2024.4.1.post0.tar`

### file list

```diff
@@ -1,134 +1,135 @@
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-03-30 03:47:22.846752 mat3ra-api-examples-2024.3.30.post3/
--rw-r--r--   0 runner    (1001) docker     (127)     1141 2024-03-30 03:46:48.000000 mat3ra-api-examples-2024.3.30.post3/.gitattributes
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-03-30 03:47:22.818752 mat3ra-api-examples-2024.3.30.post3/.github/
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-03-30 03:47:22.826752 mat3ra-api-examples-2024.3.30.post3/.github/workflows/
--rw-r--r--   0 runner    (1001) docker     (127)      452 2024-03-30 03:46:48.000000 mat3ra-api-examples-2024.3.30.post3/.github/workflows/check_links.yml
--rw-r--r--   0 runner    (1001) docker     (127)     4311 2024-03-30 03:46:48.000000 mat3ra-api-examples-2024.3.30.post3/.github/workflows/cicd.yml
--rw-r--r--   0 runner    (1001) docker     (127)     1333 2024-03-30 03:46:48.000000 mat3ra-api-examples-2024.3.30.post3/.github/workflows/zip_release.yml
--rw-r--r--   0 runner    (1001) docker     (127)     1310 2024-03-30 03:46:48.000000 mat3ra-api-examples-2024.3.30.post3/.gitignore
--rw-r--r--   0 runner    (1001) docker     (127)      161 2024-03-30 03:46:48.000000 mat3ra-api-examples-2024.3.30.post3/.lycheeignore
--rw-r--r--   0 runner    (1001) docker     (127)      407 2024-03-30 03:46:48.000000 mat3ra-api-examples-2024.3.30.post3/.pre-commit-config.yaml
--rw-r--r--   0 runner    (1001) docker     (127)    11124 2024-03-30 03:47:22.846752 mat3ra-api-examples-2024.3.30.post3/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (127)     9816 2024-03-30 03:46:48.000000 mat3ra-api-examples-2024.3.30.post3/README.md
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-03-30 03:47:22.826752 mat3ra-api-examples-2024.3.30.post3/examples/
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-03-30 03:47:22.826752 mat3ra-api-examples-2024.3.30.post3/examples/assets/
--rw-r--r--   0 runner    (1001) docker     (127)      437 2024-03-30 03:46:48.000000 mat3ra-api-examples-2024.3.30.post3/examples/assets/README.md
--rw-r--r--   0 runner    (1001) docker     (127)      130 2024-03-30 03:46:48.000000 mat3ra-api-examples-2024.3.30.post3/examples/assets/Si.pz-vbc.UPF
--rw-r--r--   0 runner    (1001) docker     (127)     4003 2024-03-30 03:46:48.000000 mat3ra-api-examples-2024.3.30.post3/examples/assets/bash_workflow_template.json
--rw-r--r--   0 runner    (1001) docker     (127)      357 2024-03-30 03:46:48.000000 mat3ra-api-examples-2024.3.30.post3/examples/assets/mp-978534.poscar
--rw-r--r--   0 runner    (1001) docker     (127)     1487 2024-03-30 03:46:48.000000 mat3ra-api-examples-2024.3.30.post3/examples/config.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-03-30 03:47:22.826752 mat3ra-api-examples-2024.3.30.post3/examples/job/
--rw-r--r--   0 runner    (1001) docker     (127)     7697 2024-03-30 03:46:48.000000 mat3ra-api-examples-2024.3.30.post3/examples/job/create_and_submit_job.ipynb
--rw-r--r--   0 runner    (1001) docker     (127)     4122 2024-03-30 03:46:48.000000 mat3ra-api-examples-2024.3.30.post3/examples/job/create_and_submit_job.py
--rw-r--r--   0 runner    (1001) docker     (127)    15077 2024-03-30 03:46:48.000000 mat3ra-api-examples-2024.3.30.post3/examples/job/get-file-from-job.ipynb
--rw-r--r--   0 runner    (1001) docker     (127)    10084 2024-03-30 03:46:48.000000 mat3ra-api-examples-2024.3.30.post3/examples/job/get-file-from-job.py
--rw-r--r--   0 runner    (1001) docker     (127)    20232 2024-03-30 03:46:48.000000 mat3ra-api-examples-2024.3.30.post3/examples/job/ml-train-model-predict-properties.ipynb
--rw-r--r--   0 runner    (1001) docker     (127)    11044 2024-03-30 03:46:48.000000 mat3ra-api-examples-2024.3.30.post3/examples/job/ml-train-model-predict-properties.py
--rw-r--r--   0 runner    (1001) docker     (127)    21020 2024-03-30 03:46:48.000000 mat3ra-api-examples-2024.3.30.post3/examples/job/run-simulations-and-extract-properties.ipynb
--rw-r--r--   0 runner    (1001) docker     (127)    12744 2024-03-30 03:46:48.000000 mat3ra-api-examples-2024.3.30.post3/examples/job/run-simulations-and-extract-properties.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-03-30 03:47:22.830752 mat3ra-api-examples-2024.3.30.post3/examples/material/
--rw-r--r--   0 runner    (1001) docker     (127)     9232 2024-03-30 03:46:48.000000 mat3ra-api-examples-2024.3.30.post3/examples/material/api_interoperability_showcase.ipynb
--rw-r--r--   0 runner    (1001) docker     (127)     5708 2024-03-30 03:46:48.000000 mat3ra-api-examples-2024.3.30.post3/examples/material/api_interoperability_showcase.py
--rw-r--r--   0 runner    (1001) docker     (127)     6934 2024-03-30 03:46:48.000000 mat3ra-api-examples-2024.3.30.post3/examples/material/create_material.ipynb
--rw-r--r--   0 runner    (1001) docker     (127)     4029 2024-03-30 03:46:48.000000 mat3ra-api-examples-2024.3.30.post3/examples/material/create_material.py
--rw-r--r--   0 runner    (1001) docker     (127)     6220 2024-03-30 03:46:48.000000 mat3ra-api-examples-2024.3.30.post3/examples/material/get_materials_by_formula.ipynb
--rw-r--r--   0 runner    (1001) docker     (127)     3423 2024-03-30 03:46:48.000000 mat3ra-api-examples-2024.3.30.post3/examples/material/get_materials_by_formula.py
--rw-r--r--   0 runner    (1001) docker     (127)     6044 2024-03-30 03:46:48.000000 mat3ra-api-examples-2024.3.30.post3/examples/material/import_materials_from_materialsproject.ipynb
--rw-r--r--   0 runner    (1001) docker     (127)     3514 2024-03-30 03:46:48.000000 mat3ra-api-examples-2024.3.30.post3/examples/material/import_materials_from_materialsproject.py
--rw-r--r--   0 runner    (1001) docker     (127)     6132 2024-03-30 03:46:48.000000 mat3ra-api-examples-2024.3.30.post3/examples/material/upload_materials_from_file_poscar.ipynb
--rw-r--r--   0 runner    (1001) docker     (127)     3545 2024-03-30 03:46:48.000000 mat3ra-api-examples-2024.3.30.post3/examples/material/upload_materials_from_file_poscar.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-03-30 03:47:22.830752 mat3ra-api-examples-2024.3.30.post3/examples/system/
--rw-r--r--   0 runner    (1001) docker     (127)     3859 2024-03-30 03:46:48.000000 mat3ra-api-examples-2024.3.30.post3/examples/system/get_authentication_params.ipynb
--rw-r--r--   0 runner    (1001) docker     (127)     1996 2024-03-30 03:46:48.000000 mat3ra-api-examples-2024.3.30.post3/examples/system/get_authentication_params.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-03-30 03:47:22.830752 mat3ra-api-examples-2024.3.30.post3/examples/workflow/
--rw-r--r--   0 runner    (1001) docker     (127)     6714 2024-03-30 03:46:48.000000 mat3ra-api-examples-2024.3.30.post3/examples/workflow/get_workflows.ipynb
--rw-r--r--   0 runner    (1001) docker     (127)     3683 2024-03-30 03:46:48.000000 mat3ra-api-examples-2024.3.30.post3/examples/workflow/get_workflows.py
--rw-r--r--   0 runner    (1001) docker     (127)    11692 2024-03-30 03:46:48.000000 mat3ra-api-examples-2024.3.30.post3/examples/workflow/qe_scf_calculation.ipynb
--rw-r--r--   0 runner    (1001) docker     (127)     6954 2024-03-30 03:46:48.000000 mat3ra-api-examples-2024.3.30.post3/examples/workflow/qe_scf_calculation.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-03-30 03:47:22.818752 mat3ra-api-examples-2024.3.30.post3/extra/
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-03-30 03:47:22.830752 mat3ra-api-examples-2024.3.30.post3/extra/css/
--rw-r--r--   0 runner    (1001) docker     (127)      134 2024-03-30 03:46:48.000000 mat3ra-api-examples-2024.3.30.post3/extra/css/custom.css
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-03-30 03:47:22.830752 mat3ra-api-examples-2024.3.30.post3/images/
--rw-r--r--   0 runner    (1001) docker     (127)   413869 2024-03-30 03:46:48.000000 mat3ra-api-examples-2024.3.30.post3/images/reusable-kernel.png
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-03-30 03:47:22.846752 mat3ra-api-examples-2024.3.30.post3/mat3ra_api_examples.egg-info/
--rw-r--r--   0 runner    (1001) docker     (127)    11124 2024-03-30 03:47:22.000000 mat3ra-api-examples-2024.3.30.post3/mat3ra_api_examples.egg-info/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (127)     4346 2024-03-30 03:47:22.000000 mat3ra-api-examples-2024.3.30.post3/mat3ra_api_examples.egg-info/SOURCES.txt
--rw-r--r--   0 runner    (1001) docker     (127)        1 2024-03-30 03:47:22.000000 mat3ra-api-examples-2024.3.30.post3/mat3ra_api_examples.egg-info/dependency_links.txt
--rw-r--r--   0 runner    (1001) docker     (127)       69 2024-03-30 03:47:22.000000 mat3ra-api-examples-2024.3.30.post3/mat3ra_api_examples.egg-info/entry_points.txt
--rw-r--r--   0 runner    (1001) docker     (127)      399 2024-03-30 03:47:22.000000 mat3ra-api-examples-2024.3.30.post3/mat3ra_api_examples.egg-info/requires.txt
--rw-r--r--   0 runner    (1001) docker     (127)        6 2024-03-30 03:47:22.000000 mat3ra-api-examples-2024.3.30.post3/mat3ra_api_examples.egg-info/top_level.txt
--rw-r--r--   0 runner    (1001) docker     (127)     3227 2024-03-30 03:46:48.000000 mat3ra-api-examples-2024.3.30.post3/mkdocs.yml
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-03-30 03:47:22.822752 mat3ra-api-examples-2024.3.30.post3/other/
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-03-30 03:47:22.834752 mat3ra-api-examples-2024.3.30.post3/other/assets/
--rw-r--r--   0 runner    (1001) docker     (127)     5159 2024-03-30 03:46:48.000000 mat3ra-api-examples-2024.3.30.post3/other/assets/README.md
--rw-r--r--   0 runner    (1001) docker     (127)   638208 2024-03-30 03:46:48.000000 mat3ra-api-examples-2024.3.30.post3/other/assets/bitter-sweet.csv
--rw-r--r--   0 runner    (1001) docker     (127)      132 2024-03-30 03:46:48.000000 mat3ra-api-examples-2024.3.30.post3/other/assets/bittersweet_xgboost.pkl
--rw-r--r--   0 runner    (1001) docker     (127)      129 2024-03-30 03:46:48.000000 mat3ra-api-examples-2024.3.30.post3/other/assets/deepchem_smiles_vocab.txt
--rw-r--r--   0 runner    (1001) docker     (127)     2562 2024-03-30 03:46:48.000000 mat3ra-api-examples-2024.3.30.post3/other/assets/gamma_alumina_digne_et_al.poscar
--rwxr-xr-x   0 runner    (1001) docker     (127)    12157 2024-03-30 03:46:48.000000 mat3ra-api-examples-2024.3.30.post3/other/assets/sci_adv_dean_data.csv
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-03-30 03:47:22.834752 mat3ra-api-examples-2024.3.30.post3/other/experiments/
--rw-r--r--   0 runner    (1001) docker     (127)    25385 2024-03-30 03:46:48.000000 mat3ra-api-examples-2024.3.30.post3/other/experiments/create_interface_with_min_energy_by_miller_indices.ipynb
--rw-r--r--   0 runner    (1001) docker     (127)    24590 2024-03-30 03:46:48.000000 mat3ra-api-examples-2024.3.30.post3/other/experiments/create_interface_with_relaxation_alignn.ipynb
--rw-r--r--   0 runner    (1001) docker     (127)    24267 2024-03-30 03:46:48.000000 mat3ra-api-examples-2024.3.30.post3/other/experiments/create_interface_with_relaxation_ase_emt.ipynb
--rw-r--r--   0 runner    (1001) docker     (127)    24750 2024-03-30 03:46:48.000000 mat3ra-api-examples-2024.3.30.post3/other/experiments/create_interface_with_relaxation_matgl_m3gnet.ipynb
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-03-30 03:47:22.834752 mat3ra-api-examples-2024.3.30.post3/other/experiments/uploads/
--rw-r--r--   0 runner    (1001) docker     (127)      774 2024-03-30 03:46:48.000000 mat3ra-api-examples-2024.3.30.post3/other/experiments/uploads/Gr.json
--rw-r--r--   0 runner    (1001) docker     (127)      730 2024-03-30 03:46:48.000000 mat3ra-api-examples-2024.3.30.post3/other/experiments/uploads/Ni.json
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-03-30 03:47:22.834752 mat3ra-api-examples-2024.3.30.post3/other/jarvis/
--rw-r--r--   0 runner    (1001) docker     (127)     3615 2024-03-30 03:46:48.000000 mat3ra-api-examples-2024.3.30.post3/other/jarvis/import_material_from_jarvis_db_entry.ipynb
--rw-r--r--   0 runner    (1001) docker     (127)    15663 2024-03-30 03:46:48.000000 mat3ra-api-examples-2024.3.30.post3/other/jarvis/run_job_using_material_from_jarvis_db.ipynb
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-03-30 03:47:22.838752 mat3ra-api-examples-2024.3.30.post3/other/job/
--rw-r--r--   0 runner    (1001) docker     (127)      131 2024-03-30 03:46:48.000000 mat3ra-api-examples-2024.3.30.post3/other/job/Smiles_Generation_Markov_Chain.ipynb
--rw-r--r--   0 runner    (1001) docker     (127)    11316 2024-03-30 03:46:48.000000 mat3ra-api-examples-2024.3.30.post3/other/job/Smiles_Generation_Markov_Chain.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-03-30 03:47:22.838752 mat3ra-api-examples-2024.3.30.post3/other/jupyterlite/
--rw-r--r--   0 runner    (1001) docker     (127)     7503 2024-03-30 03:46:48.000000 mat3ra-api-examples-2024.3.30.post3/other/jupyterlite/utils.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-03-30 03:47:22.838752 mat3ra-api-examples-2024.3.30.post3/other/machine_learning/
--rw-r--r--   0 runner    (1001) docker     (127)      131 2024-03-30 03:46:48.000000 mat3ra-api-examples-2024.3.30.post3/other/machine_learning/Classification_of_Bitterness_XGBoost.ipynb
--rw-r--r--   0 runner    (1001) docker     (127)    18602 2024-03-30 03:46:48.000000 mat3ra-api-examples-2024.3.30.post3/other/machine_learning/Classification_of_Bitterness_XGBoost.py
--rw-r--r--   0 runner    (1001) docker     (127)      131 2024-03-30 03:46:48.000000 mat3ra-api-examples-2024.3.30.post3/other/machine_learning/Prediction_of_Perovskite_Unit_Cell_Volume.ipynb
--rw-r--r--   0 runner    (1001) docker     (127)    11454 2024-03-30 03:46:48.000000 mat3ra-api-examples-2024.3.30.post3/other/machine_learning/Prediction_of_Perovskite_Unit_Cell_Volume.py
--rw-r--r--   0 runner    (1001) docker     (127)      131 2024-03-30 03:46:48.000000 mat3ra-api-examples-2024.3.30.post3/other/machine_learning/neural_network_train.ipynb
--rw-r--r--   0 runner    (1001) docker     (127)    19205 2024-03-30 03:46:48.000000 mat3ra-api-examples-2024.3.30.post3/other/machine_learning/neural_network_train.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-03-30 03:47:22.838752 mat3ra-api-examples-2024.3.30.post3/other/materials_designer/
--rw-r--r--   0 runner    (1001) docker     (127)     2347 2024-03-30 03:46:48.000000 mat3ra-api-examples-2024.3.30.post3/other/materials_designer/Introduction.ipynb
--rw-r--r--   0 runner    (1001) docker     (127)     1890 2024-03-30 03:46:48.000000 mat3ra-api-examples-2024.3.30.post3/other/materials_designer/config.yml
--rw-r--r--   0 runner    (1001) docker     (127)    16625 2024-03-30 03:46:48.000000 mat3ra-api-examples-2024.3.30.post3/other/materials_designer/create_interface_with_min_strain_zsl.ipynb
--rw-r--r--   0 runner    (1001) docker     (127)    29841 2024-03-30 03:46:48.000000 mat3ra-api-examples-2024.3.30.post3/other/materials_designer/create_interface_with_relaxation_ase_emt.ipynb
--rw-r--r--   0 runner    (1001) docker     (127)     8402 2024-03-30 03:46:48.000000 mat3ra-api-examples-2024.3.30.post3/other/materials_designer/import_material_from_jarvis_db_entry.ipynb
--rw-r--r--   0 runner    (1001) docker     (127)     8443 2024-03-30 03:46:48.000000 mat3ra-api-examples-2024.3.30.post3/other/materials_designer/import_materials_from_files.ipynb
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-03-30 03:47:22.838752 mat3ra-api-examples-2024.3.30.post3/other/materials_designer/src/
--rw-r--r--   0 runner    (1001) docker     (127)    11964 2024-03-30 03:46:48.000000 mat3ra-api-examples-2024.3.30.post3/other/materials_designer/src/pymatgen_coherent_interface_builder.py
--rw-r--r--   0 runner    (1001) docker     (127)    12408 2024-03-30 03:46:48.000000 mat3ra-api-examples-2024.3.30.post3/other/materials_designer/src/utils.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-03-30 03:47:22.838752 mat3ra-api-examples-2024.3.30.post3/other/materials_designer/uploads/
--rw-r--r--   0 runner    (1001) docker     (127)       92 2024-03-30 03:46:48.000000 mat3ra-api-examples-2024.3.30.post3/other/materials_designer/uploads/README
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-03-30 03:47:22.842752 mat3ra-api-examples-2024.3.30.post3/other/python_transformations/
--rw-r--r--   0 runner    (1001) docker     (127)     8929 2024-03-30 03:46:48.000000 mat3ra-api-examples-2024.3.30.post3/other/python_transformations/1_layer_on_substrate.py
--rw-r--r--   0 runner    (1001) docker     (127)    19706 2024-03-30 03:46:48.000000 mat3ra-api-examples-2024.3.30.post3/other/python_transformations/2_strain_matching.py
--rw-r--r--   0 runner    (1001) docker     (127)     1339 2024-03-30 03:46:48.000000 mat3ra-api-examples-2024.3.30.post3/other/python_transformations/3_imports.py
--rw-r--r--   0 runner    (1001) docker     (127)     1121 2024-03-30 03:46:48.000000 mat3ra-api-examples-2024.3.30.post3/other/python_transformations/4_custom_transformation.py
--rw-r--r--   0 runner    (1001) docker     (127)      677 2024-03-30 03:46:48.000000 mat3ra-api-examples-2024.3.30.post3/other/python_transformations/README.md
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-03-30 03:47:22.842752 mat3ra-api-examples-2024.3.30.post3/other/webinar/
--rw-r--r--   0 runner    (1001) docker     (127)      130 2024-03-30 03:46:48.000000 mat3ra-api-examples-2024.3.30.post3/other/webinar/adsorption-study.ipynb
--rw-r--r--   0 runner    (1001) docker     (127)    10676 2024-03-30 03:46:48.000000 mat3ra-api-examples-2024.3.30.post3/other/webinar/adsorption-study.py
--rw-r--r--   0 runner    (1001) docker     (127)      130 2024-03-30 03:46:48.000000 mat3ra-api-examples-2024.3.30.post3/other/webinar/generate-al2o3-slab-structures.ipynb
--rw-r--r--   0 runner    (1001) docker     (127)     8820 2024-03-30 03:46:48.000000 mat3ra-api-examples-2024.3.30.post3/other/webinar/generate-al2o3-slab-structures.py
--rw-r--r--   0 runner    (1001) docker     (127)      130 2024-03-30 03:46:48.000000 mat3ra-api-examples-2024.3.30.post3/other/webinar/predict_with_machine_learning.ipynb
--rw-r--r--   0 runner    (1001) docker     (127)     5649 2024-03-30 03:46:48.000000 mat3ra-api-examples-2024.3.30.post3/other/webinar/predict_with_machine_learning.py
--rw-r--r--   0 runner    (1001) docker     (127)      130 2024-03-30 03:46:48.000000 mat3ra-api-examples-2024.3.30.post3/other/webinar/wulff-construction-surface-energy-study-cu.ipynb
--rw-r--r--   0 runner    (1001) docker     (127)    15454 2024-03-30 03:46:48.000000 mat3ra-api-examples-2024.3.30.post3/other/webinar/wulff-construction-surface-energy-study-cu.py
--rw-r--r--   0 runner    (1001) docker     (127)     1841 2024-03-30 03:46:48.000000 mat3ra-api-examples-2024.3.30.post3/pyproject.toml
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-03-30 03:47:22.842752 mat3ra-api-examples-2024.3.30.post3/scripts/
--rwxr-xr-x   0 runner    (1001) docker     (127)     1669 2024-03-30 03:46:48.000000 mat3ra-api-examples-2024.3.30.post3/scripts/change-branch-in-urls.sh
--rw-r--r--   0 runner    (1001) docker     (127)     1253 2024-03-30 03:46:48.000000 mat3ra-api-examples-2024.3.30.post3/scripts/env.sh
--rwxr-xr-x   0 runner    (1001) docker     (127)     2267 2024-03-30 03:46:48.000000 mat3ra-api-examples-2024.3.30.post3/scripts/render-notebooks.sh
--rw-r--r--   0 runner    (1001) docker     (127)       38 2024-03-30 03:47:22.846752 mat3ra-api-examples-2024.3.30.post3/setup.cfg
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-03-30 03:47:22.842752 mat3ra-api-examples-2024.3.30.post3/utils/
--rw-r--r--   0 runner    (1001) docker     (127)        0 2024-03-30 03:46:48.000000 mat3ra-api-examples-2024.3.30.post3/utils/__init__.py
--rw-r--r--   0 runner    (1001) docker     (127)     7875 2024-03-30 03:46:48.000000 mat3ra-api-examples-2024.3.30.post3/utils/generic.py
--rw-r--r--   0 runner    (1001) docker     (127)     7735 2024-03-30 03:46:48.000000 mat3ra-api-examples-2024.3.30.post3/utils/material.py
--rw-r--r--   0 runner    (1001) docker     (127)     1305 2024-03-30 03:46:48.000000 mat3ra-api-examples-2024.3.30.post3/utils/notebook.py
--rw-r--r--   0 runner    (1001) docker     (127)      171 2024-03-30 03:46:48.000000 mat3ra-api-examples-2024.3.30.post3/utils/settings.json
--rw-r--r--   0 runner    (1001) docker     (127)     2440 2024-03-30 03:46:48.000000 mat3ra-api-examples-2024.3.30.post3/utils/settings.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-03-30 03:47:22.842752 mat3ra-api-examples-2024.3.30.post3/utils/web/
--rw-r--r--   0 runner    (1001) docker     (127)      477 2024-03-30 03:46:48.000000 mat3ra-api-examples-2024.3.30.post3/utils/web/renderjson.css
--rw-r--r--   0 runner    (1001) docker     (127)    10845 2024-03-30 03:46:48.000000 mat3ra-api-examples-2024.3.30.post3/utils/web/renderjson.js
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-01 22:44:12.146363 mat3ra-api-examples-2024.4.1.post0/
+-rw-r--r--   0 runner    (1001) docker     (127)     1141 2024-04-01 22:43:37.000000 mat3ra-api-examples-2024.4.1.post0/.gitattributes
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-01 22:44:12.118363 mat3ra-api-examples-2024.4.1.post0/.github/
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-01 22:44:12.122363 mat3ra-api-examples-2024.4.1.post0/.github/workflows/
+-rw-r--r--   0 runner    (1001) docker     (127)      452 2024-04-01 22:43:37.000000 mat3ra-api-examples-2024.4.1.post0/.github/workflows/check_links.yml
+-rw-r--r--   0 runner    (1001) docker     (127)     4311 2024-04-01 22:43:37.000000 mat3ra-api-examples-2024.4.1.post0/.github/workflows/cicd.yml
+-rw-r--r--   0 runner    (1001) docker     (127)     1333 2024-04-01 22:43:37.000000 mat3ra-api-examples-2024.4.1.post0/.github/workflows/zip_release.yml
+-rw-r--r--   0 runner    (1001) docker     (127)     1310 2024-04-01 22:43:37.000000 mat3ra-api-examples-2024.4.1.post0/.gitignore
+-rw-r--r--   0 runner    (1001) docker     (127)      161 2024-04-01 22:43:37.000000 mat3ra-api-examples-2024.4.1.post0/.lycheeignore
+-rw-r--r--   0 runner    (1001) docker     (127)      407 2024-04-01 22:43:37.000000 mat3ra-api-examples-2024.4.1.post0/.pre-commit-config.yaml
+-rw-r--r--   0 runner    (1001) docker     (127)    10319 2024-04-01 22:44:12.146363 mat3ra-api-examples-2024.4.1.post0/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (127)     9012 2024-04-01 22:43:37.000000 mat3ra-api-examples-2024.4.1.post0/README.md
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-01 22:44:12.122363 mat3ra-api-examples-2024.4.1.post0/examples/
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-01 22:44:12.122363 mat3ra-api-examples-2024.4.1.post0/examples/assets/
+-rw-r--r--   0 runner    (1001) docker     (127)      437 2024-04-01 22:43:37.000000 mat3ra-api-examples-2024.4.1.post0/examples/assets/README.md
+-rw-r--r--   0 runner    (1001) docker     (127)      130 2024-04-01 22:43:37.000000 mat3ra-api-examples-2024.4.1.post0/examples/assets/Si.pz-vbc.UPF
+-rw-r--r--   0 runner    (1001) docker     (127)     4003 2024-04-01 22:43:37.000000 mat3ra-api-examples-2024.4.1.post0/examples/assets/bash_workflow_template.json
+-rw-r--r--   0 runner    (1001) docker     (127)      357 2024-04-01 22:43:37.000000 mat3ra-api-examples-2024.4.1.post0/examples/assets/mp-978534.poscar
+-rw-r--r--   0 runner    (1001) docker     (127)     1487 2024-04-01 22:43:37.000000 mat3ra-api-examples-2024.4.1.post0/examples/config.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-01 22:44:12.126363 mat3ra-api-examples-2024.4.1.post0/examples/job/
+-rw-r--r--   0 runner    (1001) docker     (127)     7697 2024-04-01 22:43:37.000000 mat3ra-api-examples-2024.4.1.post0/examples/job/create_and_submit_job.ipynb
+-rw-r--r--   0 runner    (1001) docker     (127)     4122 2024-04-01 22:43:37.000000 mat3ra-api-examples-2024.4.1.post0/examples/job/create_and_submit_job.py
+-rw-r--r--   0 runner    (1001) docker     (127)    15077 2024-04-01 22:43:37.000000 mat3ra-api-examples-2024.4.1.post0/examples/job/get-file-from-job.ipynb
+-rw-r--r--   0 runner    (1001) docker     (127)    10084 2024-04-01 22:43:37.000000 mat3ra-api-examples-2024.4.1.post0/examples/job/get-file-from-job.py
+-rw-r--r--   0 runner    (1001) docker     (127)    20232 2024-04-01 22:43:37.000000 mat3ra-api-examples-2024.4.1.post0/examples/job/ml-train-model-predict-properties.ipynb
+-rw-r--r--   0 runner    (1001) docker     (127)    11044 2024-04-01 22:43:37.000000 mat3ra-api-examples-2024.4.1.post0/examples/job/ml-train-model-predict-properties.py
+-rw-r--r--   0 runner    (1001) docker     (127)    21020 2024-04-01 22:43:37.000000 mat3ra-api-examples-2024.4.1.post0/examples/job/run-simulations-and-extract-properties.ipynb
+-rw-r--r--   0 runner    (1001) docker     (127)    12744 2024-04-01 22:43:37.000000 mat3ra-api-examples-2024.4.1.post0/examples/job/run-simulations-and-extract-properties.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-01 22:44:12.126363 mat3ra-api-examples-2024.4.1.post0/examples/material/
+-rw-r--r--   0 runner    (1001) docker     (127)     6934 2024-04-01 22:43:37.000000 mat3ra-api-examples-2024.4.1.post0/examples/material/create_material.ipynb
+-rw-r--r--   0 runner    (1001) docker     (127)     4029 2024-04-01 22:43:37.000000 mat3ra-api-examples-2024.4.1.post0/examples/material/create_material.py
+-rw-r--r--   0 runner    (1001) docker     (127)     6220 2024-04-01 22:43:37.000000 mat3ra-api-examples-2024.4.1.post0/examples/material/get_materials_by_formula.ipynb
+-rw-r--r--   0 runner    (1001) docker     (127)     3423 2024-04-01 22:43:37.000000 mat3ra-api-examples-2024.4.1.post0/examples/material/get_materials_by_formula.py
+-rw-r--r--   0 runner    (1001) docker     (127)     6044 2024-04-01 22:43:37.000000 mat3ra-api-examples-2024.4.1.post0/examples/material/import_materials_from_materialsproject.ipynb
+-rw-r--r--   0 runner    (1001) docker     (127)     3514 2024-04-01 22:43:37.000000 mat3ra-api-examples-2024.4.1.post0/examples/material/import_materials_from_materialsproject.py
+-rw-r--r--   0 runner    (1001) docker     (127)     6132 2024-04-01 22:43:37.000000 mat3ra-api-examples-2024.4.1.post0/examples/material/upload_materials_from_file_poscar.ipynb
+-rw-r--r--   0 runner    (1001) docker     (127)     3545 2024-04-01 22:43:37.000000 mat3ra-api-examples-2024.4.1.post0/examples/material/upload_materials_from_file_poscar.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-01 22:44:12.126363 mat3ra-api-examples-2024.4.1.post0/examples/system/
+-rw-r--r--   0 runner    (1001) docker     (127)     3859 2024-04-01 22:43:37.000000 mat3ra-api-examples-2024.4.1.post0/examples/system/get_authentication_params.ipynb
+-rw-r--r--   0 runner    (1001) docker     (127)     1996 2024-04-01 22:43:37.000000 mat3ra-api-examples-2024.4.1.post0/examples/system/get_authentication_params.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-01 22:44:12.130363 mat3ra-api-examples-2024.4.1.post0/examples/workflow/
+-rw-r--r--   0 runner    (1001) docker     (127)     6714 2024-04-01 22:43:37.000000 mat3ra-api-examples-2024.4.1.post0/examples/workflow/get_workflows.ipynb
+-rw-r--r--   0 runner    (1001) docker     (127)     3683 2024-04-01 22:43:37.000000 mat3ra-api-examples-2024.4.1.post0/examples/workflow/get_workflows.py
+-rw-r--r--   0 runner    (1001) docker     (127)    11692 2024-04-01 22:43:37.000000 mat3ra-api-examples-2024.4.1.post0/examples/workflow/qe_scf_calculation.ipynb
+-rw-r--r--   0 runner    (1001) docker     (127)     6954 2024-04-01 22:43:37.000000 mat3ra-api-examples-2024.4.1.post0/examples/workflow/qe_scf_calculation.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-01 22:44:12.118363 mat3ra-api-examples-2024.4.1.post0/extra/
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-01 22:44:12.130363 mat3ra-api-examples-2024.4.1.post0/extra/css/
+-rw-r--r--   0 runner    (1001) docker     (127)      134 2024-04-01 22:43:37.000000 mat3ra-api-examples-2024.4.1.post0/extra/css/custom.css
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-01 22:44:12.130363 mat3ra-api-examples-2024.4.1.post0/images/
+-rw-r--r--   0 runner    (1001) docker     (127)   413869 2024-04-01 22:43:37.000000 mat3ra-api-examples-2024.4.1.post0/images/reusable-kernel.png
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-01 22:44:12.142363 mat3ra-api-examples-2024.4.1.post0/mat3ra_api_examples.egg-info/
+-rw-r--r--   0 runner    (1001) docker     (127)    10319 2024-04-01 22:44:12.000000 mat3ra-api-examples-2024.4.1.post0/mat3ra_api_examples.egg-info/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (127)     4356 2024-04-01 22:44:12.000000 mat3ra-api-examples-2024.4.1.post0/mat3ra_api_examples.egg-info/SOURCES.txt
+-rw-r--r--   0 runner    (1001) docker     (127)        1 2024-04-01 22:44:12.000000 mat3ra-api-examples-2024.4.1.post0/mat3ra_api_examples.egg-info/dependency_links.txt
+-rw-r--r--   0 runner    (1001) docker     (127)       69 2024-04-01 22:44:12.000000 mat3ra-api-examples-2024.4.1.post0/mat3ra_api_examples.egg-info/entry_points.txt
+-rw-r--r--   0 runner    (1001) docker     (127)      399 2024-04-01 22:44:12.000000 mat3ra-api-examples-2024.4.1.post0/mat3ra_api_examples.egg-info/requires.txt
+-rw-r--r--   0 runner    (1001) docker     (127)        6 2024-04-01 22:44:12.000000 mat3ra-api-examples-2024.4.1.post0/mat3ra_api_examples.egg-info/top_level.txt
+-rw-r--r--   0 runner    (1001) docker     (127)     3227 2024-04-01 22:43:37.000000 mat3ra-api-examples-2024.4.1.post0/mkdocs.yml
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-01 22:44:12.122363 mat3ra-api-examples-2024.4.1.post0/other/
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-01 22:44:12.134363 mat3ra-api-examples-2024.4.1.post0/other/assets/
+-rw-r--r--   0 runner    (1001) docker     (127)     5159 2024-04-01 22:43:37.000000 mat3ra-api-examples-2024.4.1.post0/other/assets/README.md
+-rw-r--r--   0 runner    (1001) docker     (127)   638208 2024-04-01 22:43:37.000000 mat3ra-api-examples-2024.4.1.post0/other/assets/bitter-sweet.csv
+-rw-r--r--   0 runner    (1001) docker     (127)      132 2024-04-01 22:43:37.000000 mat3ra-api-examples-2024.4.1.post0/other/assets/bittersweet_xgboost.pkl
+-rw-r--r--   0 runner    (1001) docker     (127)      129 2024-04-01 22:43:37.000000 mat3ra-api-examples-2024.4.1.post0/other/assets/deepchem_smiles_vocab.txt
+-rw-r--r--   0 runner    (1001) docker     (127)     2562 2024-04-01 22:43:37.000000 mat3ra-api-examples-2024.4.1.post0/other/assets/gamma_alumina_digne_et_al.poscar
+-rwxr-xr-x   0 runner    (1001) docker     (127)    12157 2024-04-01 22:43:37.000000 mat3ra-api-examples-2024.4.1.post0/other/assets/sci_adv_dean_data.csv
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-01 22:44:12.134363 mat3ra-api-examples-2024.4.1.post0/other/experiments/
+-rw-r--r--   0 runner    (1001) docker     (127)    25385 2024-04-01 22:43:37.000000 mat3ra-api-examples-2024.4.1.post0/other/experiments/create_interface_with_min_energy_by_miller_indices.ipynb
+-rw-r--r--   0 runner    (1001) docker     (127)    24590 2024-04-01 22:43:37.000000 mat3ra-api-examples-2024.4.1.post0/other/experiments/create_interface_with_relaxation_alignn.ipynb
+-rw-r--r--   0 runner    (1001) docker     (127)    24267 2024-04-01 22:43:37.000000 mat3ra-api-examples-2024.4.1.post0/other/experiments/create_interface_with_relaxation_ase_emt.ipynb
+-rw-r--r--   0 runner    (1001) docker     (127)    24750 2024-04-01 22:43:37.000000 mat3ra-api-examples-2024.4.1.post0/other/experiments/create_interface_with_relaxation_matgl_m3gnet.ipynb
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-01 22:44:12.134363 mat3ra-api-examples-2024.4.1.post0/other/experiments/uploads/
+-rw-r--r--   0 runner    (1001) docker     (127)      774 2024-04-01 22:43:37.000000 mat3ra-api-examples-2024.4.1.post0/other/experiments/uploads/Gr.json
+-rw-r--r--   0 runner    (1001) docker     (127)      730 2024-04-01 22:43:37.000000 mat3ra-api-examples-2024.4.1.post0/other/experiments/uploads/Ni.json
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-01 22:44:12.134363 mat3ra-api-examples-2024.4.1.post0/other/jarvis/
+-rw-r--r--   0 runner    (1001) docker     (127)     3615 2024-04-01 22:43:37.000000 mat3ra-api-examples-2024.4.1.post0/other/jarvis/import_material_from_jarvis_db_entry.ipynb
+-rw-r--r--   0 runner    (1001) docker     (127)    15663 2024-04-01 22:43:37.000000 mat3ra-api-examples-2024.4.1.post0/other/jarvis/run_job_using_material_from_jarvis_db.ipynb
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-01 22:44:12.134363 mat3ra-api-examples-2024.4.1.post0/other/job/
+-rw-r--r--   0 runner    (1001) docker     (127)      131 2024-04-01 22:43:37.000000 mat3ra-api-examples-2024.4.1.post0/other/job/Smiles_Generation_Markov_Chain.ipynb
+-rw-r--r--   0 runner    (1001) docker     (127)    11316 2024-04-01 22:43:37.000000 mat3ra-api-examples-2024.4.1.post0/other/job/Smiles_Generation_Markov_Chain.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-01 22:44:12.134363 mat3ra-api-examples-2024.4.1.post0/other/jupyterlite/
+-rw-r--r--   0 runner    (1001) docker     (127)     7503 2024-04-01 22:43:37.000000 mat3ra-api-examples-2024.4.1.post0/other/jupyterlite/utils.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-01 22:44:12.134363 mat3ra-api-examples-2024.4.1.post0/other/machine_learning/
+-rw-r--r--   0 runner    (1001) docker     (127)      131 2024-04-01 22:43:37.000000 mat3ra-api-examples-2024.4.1.post0/other/machine_learning/Classification_of_Bitterness_XGBoost.ipynb
+-rw-r--r--   0 runner    (1001) docker     (127)    18602 2024-04-01 22:43:37.000000 mat3ra-api-examples-2024.4.1.post0/other/machine_learning/Classification_of_Bitterness_XGBoost.py
+-rw-r--r--   0 runner    (1001) docker     (127)      131 2024-04-01 22:43:37.000000 mat3ra-api-examples-2024.4.1.post0/other/machine_learning/Prediction_of_Perovskite_Unit_Cell_Volume.ipynb
+-rw-r--r--   0 runner    (1001) docker     (127)    11454 2024-04-01 22:43:37.000000 mat3ra-api-examples-2024.4.1.post0/other/machine_learning/Prediction_of_Perovskite_Unit_Cell_Volume.py
+-rw-r--r--   0 runner    (1001) docker     (127)      131 2024-04-01 22:43:37.000000 mat3ra-api-examples-2024.4.1.post0/other/machine_learning/neural_network_train.ipynb
+-rw-r--r--   0 runner    (1001) docker     (127)    19205 2024-04-01 22:43:37.000000 mat3ra-api-examples-2024.4.1.post0/other/machine_learning/neural_network_train.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-01 22:44:12.138363 mat3ra-api-examples-2024.4.1.post0/other/materials_designer/
+-rw-r--r--   0 runner    (1001) docker     (127)     2347 2024-04-01 22:43:37.000000 mat3ra-api-examples-2024.4.1.post0/other/materials_designer/Introduction.ipynb
+-rw-r--r--   0 runner    (1001) docker     (127)     1890 2024-04-01 22:43:37.000000 mat3ra-api-examples-2024.4.1.post0/other/materials_designer/config.yml
+-rw-r--r--   0 runner    (1001) docker     (127)    16625 2024-04-01 22:43:37.000000 mat3ra-api-examples-2024.4.1.post0/other/materials_designer/create_interface_with_min_strain_zsl.ipynb
+-rw-r--r--   0 runner    (1001) docker     (127)    29841 2024-04-01 22:43:37.000000 mat3ra-api-examples-2024.4.1.post0/other/materials_designer/create_interface_with_relaxation_ase_emt.ipynb
+-rw-r--r--   0 runner    (1001) docker     (127)     8402 2024-04-01 22:43:37.000000 mat3ra-api-examples-2024.4.1.post0/other/materials_designer/import_material_from_jarvis_db_entry.ipynb
+-rw-r--r--   0 runner    (1001) docker     (127)     8443 2024-04-01 22:43:37.000000 mat3ra-api-examples-2024.4.1.post0/other/materials_designer/import_materials_from_files.ipynb
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-01 22:44:12.138363 mat3ra-api-examples-2024.4.1.post0/other/materials_designer/src/
+-rw-r--r--   0 runner    (1001) docker     (127)    11964 2024-04-01 22:43:37.000000 mat3ra-api-examples-2024.4.1.post0/other/materials_designer/src/pymatgen_coherent_interface_builder.py
+-rw-r--r--   0 runner    (1001) docker     (127)    12408 2024-04-01 22:43:37.000000 mat3ra-api-examples-2024.4.1.post0/other/materials_designer/src/utils.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-01 22:44:12.138363 mat3ra-api-examples-2024.4.1.post0/other/materials_designer/uploads/
+-rw-r--r--   0 runner    (1001) docker     (127)       92 2024-04-01 22:43:37.000000 mat3ra-api-examples-2024.4.1.post0/other/materials_designer/uploads/README
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-01 22:44:12.138363 mat3ra-api-examples-2024.4.1.post0/other/materialsproject/
+-rw-r--r--   0 runner    (1001) docker     (127)     9232 2024-04-01 22:43:37.000000 mat3ra-api-examples-2024.4.1.post0/other/materialsproject/api_interoperability_showcase.ipynb
+-rw-r--r--   0 runner    (1001) docker     (127)     5708 2024-04-01 22:43:37.000000 mat3ra-api-examples-2024.4.1.post0/other/materialsproject/api_interoperability_showcase.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-01 22:44:12.138363 mat3ra-api-examples-2024.4.1.post0/other/python_transformations/
+-rw-r--r--   0 runner    (1001) docker     (127)     8929 2024-04-01 22:43:37.000000 mat3ra-api-examples-2024.4.1.post0/other/python_transformations/1_layer_on_substrate.py
+-rw-r--r--   0 runner    (1001) docker     (127)    19706 2024-04-01 22:43:37.000000 mat3ra-api-examples-2024.4.1.post0/other/python_transformations/2_strain_matching.py
+-rw-r--r--   0 runner    (1001) docker     (127)     1339 2024-04-01 22:43:37.000000 mat3ra-api-examples-2024.4.1.post0/other/python_transformations/3_imports.py
+-rw-r--r--   0 runner    (1001) docker     (127)     1121 2024-04-01 22:43:37.000000 mat3ra-api-examples-2024.4.1.post0/other/python_transformations/4_custom_transformation.py
+-rw-r--r--   0 runner    (1001) docker     (127)      677 2024-04-01 22:43:37.000000 mat3ra-api-examples-2024.4.1.post0/other/python_transformations/README.md
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-01 22:44:12.142363 mat3ra-api-examples-2024.4.1.post0/other/webinar/
+-rw-r--r--   0 runner    (1001) docker     (127)      130 2024-04-01 22:43:37.000000 mat3ra-api-examples-2024.4.1.post0/other/webinar/adsorption-study.ipynb
+-rw-r--r--   0 runner    (1001) docker     (127)    10676 2024-04-01 22:43:37.000000 mat3ra-api-examples-2024.4.1.post0/other/webinar/adsorption-study.py
+-rw-r--r--   0 runner    (1001) docker     (127)      130 2024-04-01 22:43:37.000000 mat3ra-api-examples-2024.4.1.post0/other/webinar/generate-al2o3-slab-structures.ipynb
+-rw-r--r--   0 runner    (1001) docker     (127)     8820 2024-04-01 22:43:37.000000 mat3ra-api-examples-2024.4.1.post0/other/webinar/generate-al2o3-slab-structures.py
+-rw-r--r--   0 runner    (1001) docker     (127)      130 2024-04-01 22:43:37.000000 mat3ra-api-examples-2024.4.1.post0/other/webinar/predict_with_machine_learning.ipynb
+-rw-r--r--   0 runner    (1001) docker     (127)     5649 2024-04-01 22:43:37.000000 mat3ra-api-examples-2024.4.1.post0/other/webinar/predict_with_machine_learning.py
+-rw-r--r--   0 runner    (1001) docker     (127)      130 2024-04-01 22:43:37.000000 mat3ra-api-examples-2024.4.1.post0/other/webinar/wulff-construction-surface-energy-study-cu.ipynb
+-rw-r--r--   0 runner    (1001) docker     (127)    15454 2024-04-01 22:43:37.000000 mat3ra-api-examples-2024.4.1.post0/other/webinar/wulff-construction-surface-energy-study-cu.py
+-rw-r--r--   0 runner    (1001) docker     (127)     1841 2024-04-01 22:43:37.000000 mat3ra-api-examples-2024.4.1.post0/pyproject.toml
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-01 22:44:12.142363 mat3ra-api-examples-2024.4.1.post0/scripts/
+-rwxr-xr-x   0 runner    (1001) docker     (127)     1669 2024-04-01 22:43:37.000000 mat3ra-api-examples-2024.4.1.post0/scripts/change-branch-in-urls.sh
+-rw-r--r--   0 runner    (1001) docker     (127)     1253 2024-04-01 22:43:37.000000 mat3ra-api-examples-2024.4.1.post0/scripts/env.sh
+-rwxr-xr-x   0 runner    (1001) docker     (127)     2267 2024-04-01 22:43:37.000000 mat3ra-api-examples-2024.4.1.post0/scripts/render-notebooks.sh
+-rw-r--r--   0 runner    (1001) docker     (127)       38 2024-04-01 22:44:12.146363 mat3ra-api-examples-2024.4.1.post0/setup.cfg
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-01 22:44:12.142363 mat3ra-api-examples-2024.4.1.post0/utils/
+-rw-r--r--   0 runner    (1001) docker     (127)        0 2024-04-01 22:43:37.000000 mat3ra-api-examples-2024.4.1.post0/utils/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (127)     7875 2024-04-01 22:43:37.000000 mat3ra-api-examples-2024.4.1.post0/utils/generic.py
+-rw-r--r--   0 runner    (1001) docker     (127)     7735 2024-04-01 22:43:37.000000 mat3ra-api-examples-2024.4.1.post0/utils/material.py
+-rw-r--r--   0 runner    (1001) docker     (127)     1305 2024-04-01 22:43:37.000000 mat3ra-api-examples-2024.4.1.post0/utils/notebook.py
+-rw-r--r--   0 runner    (1001) docker     (127)      171 2024-04-01 22:43:37.000000 mat3ra-api-examples-2024.4.1.post0/utils/settings.json
+-rw-r--r--   0 runner    (1001) docker     (127)     2440 2024-04-01 22:43:37.000000 mat3ra-api-examples-2024.4.1.post0/utils/settings.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-01 22:44:12.142363 mat3ra-api-examples-2024.4.1.post0/utils/web/
+-rw-r--r--   0 runner    (1001) docker     (127)      477 2024-04-01 22:43:37.000000 mat3ra-api-examples-2024.4.1.post0/utils/web/renderjson.css
+-rw-r--r--   0 runner    (1001) docker     (127)    10845 2024-04-01 22:43:37.000000 mat3ra-api-examples-2024.4.1.post0/utils/web/renderjson.js
```

### Comparing `mat3ra-api-examples-2024.3.30.post3/.gitattributes` & `mat3ra-api-examples-2024.4.1.post0/.gitattributes`

 * *Files identical despite different names*

### Comparing `mat3ra-api-examples-2024.3.30.post3/.github/workflows/cicd.yml` & `mat3ra-api-examples-2024.4.1.post0/.github/workflows/cicd.yml`

 * *Files identical despite different names*

### Comparing `mat3ra-api-examples-2024.3.30.post3/.github/workflows/zip_release.yml` & `mat3ra-api-examples-2024.4.1.post0/.github/workflows/zip_release.yml`

 * *Files identical despite different names*

### Comparing `mat3ra-api-examples-2024.3.30.post3/.gitignore` & `mat3ra-api-examples-2024.4.1.post0/.gitignore`

 * *Files identical despite different names*

### Comparing `mat3ra-api-examples-2024.3.30.post3/PKG-INFO` & `mat3ra-api-examples-2024.4.1.post0/PKG-INFO`

 * *Files 6% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: mat3ra-api-examples
-Version: 2024.3.30.post3
+Version: 2024.4.1.post0
 Summary: Mat3ra API Examples
 Project-URL: homepage, https://exabyte-io.github.io/api-examples
 Project-URL: documentation, https://exabyte-io.github.io/api-examples
 Project-URL: repository, https://github.com/Exabyte-io/api-examples
 Requires-Python: >=3.8
 Description-Content-Type: text/markdown
 Requires-Dist: ase>=3.21.1
@@ -34,26 +34,25 @@
 
 ## Contents of this Repository
 
 Below, we list the contents of this repository, in roughly the order that a user might want to go through it in order to learn how our API works.
 
 | Folder            | Notebook                                | Description |
 | ------------------|-----------------------------------------| ----------- |
-| [Examples/System](examples/system/)     | [Get Authentication Params](examples/system/get_authentication_params.ipynb)               | Demonstrates how to programatically find your user ID and access token, which is to [authenticate](https://docs.mat3ra.com/rest-api/authentication/) for many portions of the Mat3ra API.
+| [Examples/System](examples/system/)     | [Get Authentication Params](examples/system/get_authentication_params.ipynb)               | Demonstrates how to programatically find your user ID and access token.
 | [Examples/Workflow](examples/workflow/) | [Get Workflows](examples/workflow/get_workflows.ipynb)                           | Walks through how to [query](https://docs.mat3ra.com/rest-api/query-structure/) the Mat3ra API to programatically search for workflows. In this example, we search for workflows that calculate the total energy of a material.
 | [Examples/Workflow](examples/workflow/) | [Quantum Espresso Workflow and Job](examples/workflow/qe_scf_calculation.ipynb)  | Create Quantum Espresso workflow starting from QE input file; create and submit job; after the job is finished, download output file, and finally perform postprocessing analysis.
 | [Examples/Material](examples/material/) | [Get Materials by Formula](examples/material/get_materials_by_formula.ipynb)                | Shows how [queries](https://docs.mat3ra.com/rest-api/query-structure/) can be made to search for materials stored on your account by their formula. In this example, we search for a system containing Si.
 | [Examples/Material](examples/material/) | [Create Material](examples/material/create_material.ipynb)                         | Gives an overview of how materials can be generated in [JSON format](https://docs.mat3ra.com/materials/data/) and uploaded to your user account. In this example, we create an FCC Si crystal and upload it.
 | [Examples/Material](examples/material/) | [Import Materials from Materials Project](examples/material/import_materials_from_materialsproject.ipynb) | Demonstrates how materials can be imported from [Materials Project](https://materialsproject.org/about), if their Materials Project ID is known. In this example, we import monoclinic and hexagonal SiGe cells.
 | [Examples/Material](examples/material/) | [Import Materials from Poscar](examples/material/upload_materials_from_file_poscar.ipynb)            | Provides an example of how materials can be imported directly from Poscar files (a common chemical file format best-known [for its use in VASP](https://www.vasp.at/wiki/index.php/Input)). In this example, we import the unit cell of SiGe.
-| [Examples/Material](examples/material/) | [Interoperability between Mat3ra and Materials Project](examples/material/api_interoperability_showcase.ipynb)            | In this notebook, we showcase a major advantage of APIs: interoperability. We begin by performing a query using the [Materials Project](https://materialsproject.org) API for all systems containing Iron and Oxygen. We then filter our results (for demonstraiton purposes, we keep only the first 10 materials found). Finally, we upload our results to the Mat3ra platform, where further calculations could be performed to characterize these materials.
 | [Examples/Job](examples/job/)            | [Create and Submit Job](examples/job/create_and_submit_job.ipynb)                   | Shows how to use the Mat3ra API to [create jobs](https://docs.mat3ra.com/jobs/data/) and run them on our cluster. In this example, we run a DFT calculation to get the total energy of an FCC Si unit cell using Quantum Espresso.
-| [Examples/Job](examples/job/)            | [Get File from Job](examples/job/get-file-from-job.ipynb) | Guides you through using the Mat3ra API to query for a list of files produced by a job, describes the metadata assigned to each file, and ends by demonstrating how to download any remote file generated by a job to the local disk.
-| [Examples/Job](examples/job/)            | [Run Simulations and Extract Properties](examples/job/run-simulations-and-extract-properties.ipynb)  | Leads you through the process of copying a [bank workflow](https://docs.mat3ra.com/workflows/bank/) to your account and using it to automatically calculate the [properties](https://docs.mat3ra.com/properties/overview/) of multiple materials. In this example, we determine the [band gap](https://docs.mat3ra.com/properties-directory/non-scalar/band-gaps/) of Si and Ge.
-| [Examples/Job](examples/job/)            | [ML - Train Model Predict Properties](examples/job/ml-train-model-predict-properties.ipynb)     | Walks you through automated dataset generation and the training/prediction of material properties using [machine learning](https://docs.mat3ra.com/software-directory/overview/#machine-learning). In this example, we calculate the band gaps of Si and SiGe, and using various materials properties as descriptors, train a model to predict their band gaps. Finally, we use this trained model to predict the band gap of Ge.
+| [Examples/Job](examples/job/)            | [Get File from Job](examples/job/get-file-from-job.ipynb) | Uses the Mat3ra API to query for a list of files produced by a job, describes the metadata assigned to each file, and ends by demonstrating how to download any remote file generated by a job to the local disk.
+| [Examples/Job](examples/job/)            | [Run Simulations and Extract Properties](examples/job/run-simulations-and-extract-properties.ipynb)  | Demonstrates copying a [bank workflow](https://docs.mat3ra.com/workflows/bank/) to an account and using it to calculate the [properties](https://docs.mat3ra.com/properties/overview/) of multiple materials. In this example, we determine the [band gap](https://docs.mat3ra.com/properties-directory/non-scalar/band-gaps/) of Si and Ge.
+| [Examples/Job](examples/job/)            | [ML - Train Model Predict Properties](examples/job/ml-train-model-predict-properties.ipynb)     | Demonstrates the  generation of a training dataset and subsequent training of a [machine learning](https://docs.mat3ra.com/software-directory/overview/#machine-learning) model. In this example, we calculate the band gaps of Si and SiGe, and using various materials properties as descriptors, train a model to predict their band gaps. Finally, we use this trained model to predict the band gap of Ge.
 
 
 
 ## Setup
 
 NOTE: tested with Python version 3.8 and 3.10, please assert that the virtual environment is created with it. Use [`pyenv`](https://github.com/pyenv/pyenv#installation) to manage Python versions.
```

### Comparing `mat3ra-api-examples-2024.3.30.post3/README.md` & `mat3ra-api-examples-2024.4.1.post0/README.md`

 * *Files 5% similar despite different names*

```diff
@@ -2,26 +2,25 @@
 
 ## Contents of this Repository
 
 Below, we list the contents of this repository, in roughly the order that a user might want to go through it in order to learn how our API works.
 
 | Folder            | Notebook                                | Description |
 | ------------------|-----------------------------------------| ----------- |
-| [Examples/System](examples/system/)     | [Get Authentication Params](examples/system/get_authentication_params.ipynb)               | Demonstrates how to programatically find your user ID and access token, which is to [authenticate](https://docs.mat3ra.com/rest-api/authentication/) for many portions of the Mat3ra API.
+| [Examples/System](examples/system/)     | [Get Authentication Params](examples/system/get_authentication_params.ipynb)               | Demonstrates how to programatically find your user ID and access token.
 | [Examples/Workflow](examples/workflow/) | [Get Workflows](examples/workflow/get_workflows.ipynb)                           | Walks through how to [query](https://docs.mat3ra.com/rest-api/query-structure/) the Mat3ra API to programatically search for workflows. In this example, we search for workflows that calculate the total energy of a material.
 | [Examples/Workflow](examples/workflow/) | [Quantum Espresso Workflow and Job](examples/workflow/qe_scf_calculation.ipynb)  | Create Quantum Espresso workflow starting from QE input file; create and submit job; after the job is finished, download output file, and finally perform postprocessing analysis.
 | [Examples/Material](examples/material/) | [Get Materials by Formula](examples/material/get_materials_by_formula.ipynb)                | Shows how [queries](https://docs.mat3ra.com/rest-api/query-structure/) can be made to search for materials stored on your account by their formula. In this example, we search for a system containing Si.
 | [Examples/Material](examples/material/) | [Create Material](examples/material/create_material.ipynb)                         | Gives an overview of how materials can be generated in [JSON format](https://docs.mat3ra.com/materials/data/) and uploaded to your user account. In this example, we create an FCC Si crystal and upload it.
 | [Examples/Material](examples/material/) | [Import Materials from Materials Project](examples/material/import_materials_from_materialsproject.ipynb) | Demonstrates how materials can be imported from [Materials Project](https://materialsproject.org/about), if their Materials Project ID is known. In this example, we import monoclinic and hexagonal SiGe cells.
 | [Examples/Material](examples/material/) | [Import Materials from Poscar](examples/material/upload_materials_from_file_poscar.ipynb)            | Provides an example of how materials can be imported directly from Poscar files (a common chemical file format best-known [for its use in VASP](https://www.vasp.at/wiki/index.php/Input)). In this example, we import the unit cell of SiGe.
-| [Examples/Material](examples/material/) | [Interoperability between Mat3ra and Materials Project](examples/material/api_interoperability_showcase.ipynb)            | In this notebook, we showcase a major advantage of APIs: interoperability. We begin by performing a query using the [Materials Project](https://materialsproject.org) API for all systems containing Iron and Oxygen. We then filter our results (for demonstraiton purposes, we keep only the first 10 materials found). Finally, we upload our results to the Mat3ra platform, where further calculations could be performed to characterize these materials.
 | [Examples/Job](examples/job/)            | [Create and Submit Job](examples/job/create_and_submit_job.ipynb)                   | Shows how to use the Mat3ra API to [create jobs](https://docs.mat3ra.com/jobs/data/) and run them on our cluster. In this example, we run a DFT calculation to get the total energy of an FCC Si unit cell using Quantum Espresso.
-| [Examples/Job](examples/job/)            | [Get File from Job](examples/job/get-file-from-job.ipynb) | Guides you through using the Mat3ra API to query for a list of files produced by a job, describes the metadata assigned to each file, and ends by demonstrating how to download any remote file generated by a job to the local disk.
-| [Examples/Job](examples/job/)            | [Run Simulations and Extract Properties](examples/job/run-simulations-and-extract-properties.ipynb)  | Leads you through the process of copying a [bank workflow](https://docs.mat3ra.com/workflows/bank/) to your account and using it to automatically calculate the [properties](https://docs.mat3ra.com/properties/overview/) of multiple materials. In this example, we determine the [band gap](https://docs.mat3ra.com/properties-directory/non-scalar/band-gaps/) of Si and Ge.
-| [Examples/Job](examples/job/)            | [ML - Train Model Predict Properties](examples/job/ml-train-model-predict-properties.ipynb)     | Walks you through automated dataset generation and the training/prediction of material properties using [machine learning](https://docs.mat3ra.com/software-directory/overview/#machine-learning). In this example, we calculate the band gaps of Si and SiGe, and using various materials properties as descriptors, train a model to predict their band gaps. Finally, we use this trained model to predict the band gap of Ge.
+| [Examples/Job](examples/job/)            | [Get File from Job](examples/job/get-file-from-job.ipynb) | Uses the Mat3ra API to query for a list of files produced by a job, describes the metadata assigned to each file, and ends by demonstrating how to download any remote file generated by a job to the local disk.
+| [Examples/Job](examples/job/)            | [Run Simulations and Extract Properties](examples/job/run-simulations-and-extract-properties.ipynb)  | Demonstrates copying a [bank workflow](https://docs.mat3ra.com/workflows/bank/) to an account and using it to calculate the [properties](https://docs.mat3ra.com/properties/overview/) of multiple materials. In this example, we determine the [band gap](https://docs.mat3ra.com/properties-directory/non-scalar/band-gaps/) of Si and Ge.
+| [Examples/Job](examples/job/)            | [ML - Train Model Predict Properties](examples/job/ml-train-model-predict-properties.ipynb)     | Demonstrates the  generation of a training dataset and subsequent training of a [machine learning](https://docs.mat3ra.com/software-directory/overview/#machine-learning) model. In this example, we calculate the band gaps of Si and SiGe, and using various materials properties as descriptors, train a model to predict their band gaps. Finally, we use this trained model to predict the band gap of Ge.
 
 
 
 ## Setup
 
 NOTE: tested with Python version 3.8 and 3.10, please assert that the virtual environment is created with it. Use [`pyenv`](https://github.com/pyenv/pyenv#installation) to manage Python versions.
```

### Comparing `mat3ra-api-examples-2024.3.30.post3/examples/assets/bash_workflow_template.json` & `mat3ra-api-examples-2024.4.1.post0/examples/assets/bash_workflow_template.json`

 * *Files identical despite different names*

### Comparing `mat3ra-api-examples-2024.3.30.post3/examples/config.py` & `mat3ra-api-examples-2024.4.1.post0/examples/config.py`

 * *Files identical despite different names*

### Comparing `mat3ra-api-examples-2024.3.30.post3/examples/job/create_and_submit_job.ipynb` & `mat3ra-api-examples-2024.4.1.post0/examples/job/create_and_submit_job.ipynb`

 * *Files identical despite different names*

### Comparing `mat3ra-api-examples-2024.3.30.post3/examples/job/create_and_submit_job.py` & `mat3ra-api-examples-2024.4.1.post0/examples/job/create_and_submit_job.py`

 * *Files identical despite different names*

### Comparing `mat3ra-api-examples-2024.3.30.post3/examples/job/get-file-from-job.ipynb` & `mat3ra-api-examples-2024.4.1.post0/examples/job/get-file-from-job.ipynb`

 * *Files identical despite different names*

### Comparing `mat3ra-api-examples-2024.3.30.post3/examples/job/get-file-from-job.py` & `mat3ra-api-examples-2024.4.1.post0/examples/job/get-file-from-job.py`

 * *Files identical despite different names*

### Comparing `mat3ra-api-examples-2024.3.30.post3/examples/job/ml-train-model-predict-properties.ipynb` & `mat3ra-api-examples-2024.4.1.post0/examples/job/ml-train-model-predict-properties.ipynb`

 * *Files identical despite different names*

### Comparing `mat3ra-api-examples-2024.3.30.post3/examples/job/ml-train-model-predict-properties.py` & `mat3ra-api-examples-2024.4.1.post0/examples/job/ml-train-model-predict-properties.py`

 * *Files identical despite different names*

### Comparing `mat3ra-api-examples-2024.3.30.post3/examples/job/run-simulations-and-extract-properties.ipynb` & `mat3ra-api-examples-2024.4.1.post0/examples/job/run-simulations-and-extract-properties.ipynb`

 * *Files identical despite different names*

### Comparing `mat3ra-api-examples-2024.3.30.post3/examples/job/run-simulations-and-extract-properties.py` & `mat3ra-api-examples-2024.4.1.post0/examples/job/run-simulations-and-extract-properties.py`

 * *Files identical despite different names*

### Comparing `mat3ra-api-examples-2024.3.30.post3/examples/material/api_interoperability_showcase.ipynb` & `mat3ra-api-examples-2024.4.1.post0/other/materialsproject/api_interoperability_showcase.ipynb`

 * *Files identical despite different names*

### Comparing `mat3ra-api-examples-2024.3.30.post3/examples/material/api_interoperability_showcase.py` & `mat3ra-api-examples-2024.4.1.post0/other/materialsproject/api_interoperability_showcase.py`

 * *Files identical despite different names*

### Comparing `mat3ra-api-examples-2024.3.30.post3/examples/material/create_material.ipynb` & `mat3ra-api-examples-2024.4.1.post0/examples/material/create_material.ipynb`

 * *Files identical despite different names*

### Comparing `mat3ra-api-examples-2024.3.30.post3/examples/material/create_material.py` & `mat3ra-api-examples-2024.4.1.post0/examples/material/create_material.py`

 * *Files identical despite different names*

### Comparing `mat3ra-api-examples-2024.3.30.post3/examples/material/get_materials_by_formula.ipynb` & `mat3ra-api-examples-2024.4.1.post0/examples/material/get_materials_by_formula.ipynb`

 * *Files identical despite different names*

### Comparing `mat3ra-api-examples-2024.3.30.post3/examples/material/get_materials_by_formula.py` & `mat3ra-api-examples-2024.4.1.post0/examples/material/get_materials_by_formula.py`

 * *Files identical despite different names*

### Comparing `mat3ra-api-examples-2024.3.30.post3/examples/material/import_materials_from_materialsproject.ipynb` & `mat3ra-api-examples-2024.4.1.post0/examples/material/import_materials_from_materialsproject.ipynb`

 * *Files identical despite different names*

### Comparing `mat3ra-api-examples-2024.3.30.post3/examples/material/import_materials_from_materialsproject.py` & `mat3ra-api-examples-2024.4.1.post0/examples/material/import_materials_from_materialsproject.py`

 * *Files identical despite different names*

### Comparing `mat3ra-api-examples-2024.3.30.post3/examples/material/upload_materials_from_file_poscar.ipynb` & `mat3ra-api-examples-2024.4.1.post0/examples/material/upload_materials_from_file_poscar.ipynb`

 * *Files identical despite different names*

### Comparing `mat3ra-api-examples-2024.3.30.post3/examples/material/upload_materials_from_file_poscar.py` & `mat3ra-api-examples-2024.4.1.post0/examples/material/upload_materials_from_file_poscar.py`

 * *Files identical despite different names*

### Comparing `mat3ra-api-examples-2024.3.30.post3/examples/system/get_authentication_params.ipynb` & `mat3ra-api-examples-2024.4.1.post0/examples/system/get_authentication_params.ipynb`

 * *Files identical despite different names*

### Comparing `mat3ra-api-examples-2024.3.30.post3/examples/system/get_authentication_params.py` & `mat3ra-api-examples-2024.4.1.post0/examples/system/get_authentication_params.py`

 * *Files identical despite different names*

### Comparing `mat3ra-api-examples-2024.3.30.post3/examples/workflow/get_workflows.ipynb` & `mat3ra-api-examples-2024.4.1.post0/examples/workflow/get_workflows.ipynb`

 * *Files identical despite different names*

### Comparing `mat3ra-api-examples-2024.3.30.post3/examples/workflow/get_workflows.py` & `mat3ra-api-examples-2024.4.1.post0/examples/workflow/get_workflows.py`

 * *Files identical despite different names*

### Comparing `mat3ra-api-examples-2024.3.30.post3/examples/workflow/qe_scf_calculation.ipynb` & `mat3ra-api-examples-2024.4.1.post0/examples/workflow/qe_scf_calculation.ipynb`

 * *Files identical despite different names*

### Comparing `mat3ra-api-examples-2024.3.30.post3/examples/workflow/qe_scf_calculation.py` & `mat3ra-api-examples-2024.4.1.post0/examples/workflow/qe_scf_calculation.py`

 * *Files identical despite different names*

### Comparing `mat3ra-api-examples-2024.3.30.post3/images/reusable-kernel.png` & `mat3ra-api-examples-2024.4.1.post0/images/reusable-kernel.png`

 * *Files identical despite different names*

### Comparing `mat3ra-api-examples-2024.3.30.post3/mat3ra_api_examples.egg-info/PKG-INFO` & `mat3ra-api-examples-2024.4.1.post0/mat3ra_api_examples.egg-info/PKG-INFO`

 * *Files 6% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: mat3ra-api-examples
-Version: 2024.3.30.post3
+Version: 2024.4.1.post0
 Summary: Mat3ra API Examples
 Project-URL: homepage, https://exabyte-io.github.io/api-examples
 Project-URL: documentation, https://exabyte-io.github.io/api-examples
 Project-URL: repository, https://github.com/Exabyte-io/api-examples
 Requires-Python: >=3.8
 Description-Content-Type: text/markdown
 Requires-Dist: ase>=3.21.1
@@ -34,26 +34,25 @@
 
 ## Contents of this Repository
 
 Below, we list the contents of this repository, in roughly the order that a user might want to go through it in order to learn how our API works.
 
 | Folder            | Notebook                                | Description |
 | ------------------|-----------------------------------------| ----------- |
-| [Examples/System](examples/system/)     | [Get Authentication Params](examples/system/get_authentication_params.ipynb)               | Demonstrates how to programatically find your user ID and access token, which is to [authenticate](https://docs.mat3ra.com/rest-api/authentication/) for many portions of the Mat3ra API.
+| [Examples/System](examples/system/)     | [Get Authentication Params](examples/system/get_authentication_params.ipynb)               | Demonstrates how to programatically find your user ID and access token.
 | [Examples/Workflow](examples/workflow/) | [Get Workflows](examples/workflow/get_workflows.ipynb)                           | Walks through how to [query](https://docs.mat3ra.com/rest-api/query-structure/) the Mat3ra API to programatically search for workflows. In this example, we search for workflows that calculate the total energy of a material.
 | [Examples/Workflow](examples/workflow/) | [Quantum Espresso Workflow and Job](examples/workflow/qe_scf_calculation.ipynb)  | Create Quantum Espresso workflow starting from QE input file; create and submit job; after the job is finished, download output file, and finally perform postprocessing analysis.
 | [Examples/Material](examples/material/) | [Get Materials by Formula](examples/material/get_materials_by_formula.ipynb)                | Shows how [queries](https://docs.mat3ra.com/rest-api/query-structure/) can be made to search for materials stored on your account by their formula. In this example, we search for a system containing Si.
 | [Examples/Material](examples/material/) | [Create Material](examples/material/create_material.ipynb)                         | Gives an overview of how materials can be generated in [JSON format](https://docs.mat3ra.com/materials/data/) and uploaded to your user account. In this example, we create an FCC Si crystal and upload it.
 | [Examples/Material](examples/material/) | [Import Materials from Materials Project](examples/material/import_materials_from_materialsproject.ipynb) | Demonstrates how materials can be imported from [Materials Project](https://materialsproject.org/about), if their Materials Project ID is known. In this example, we import monoclinic and hexagonal SiGe cells.
 | [Examples/Material](examples/material/) | [Import Materials from Poscar](examples/material/upload_materials_from_file_poscar.ipynb)            | Provides an example of how materials can be imported directly from Poscar files (a common chemical file format best-known [for its use in VASP](https://www.vasp.at/wiki/index.php/Input)). In this example, we import the unit cell of SiGe.
-| [Examples/Material](examples/material/) | [Interoperability between Mat3ra and Materials Project](examples/material/api_interoperability_showcase.ipynb)            | In this notebook, we showcase a major advantage of APIs: interoperability. We begin by performing a query using the [Materials Project](https://materialsproject.org) API for all systems containing Iron and Oxygen. We then filter our results (for demonstraiton purposes, we keep only the first 10 materials found). Finally, we upload our results to the Mat3ra platform, where further calculations could be performed to characterize these materials.
 | [Examples/Job](examples/job/)            | [Create and Submit Job](examples/job/create_and_submit_job.ipynb)                   | Shows how to use the Mat3ra API to [create jobs](https://docs.mat3ra.com/jobs/data/) and run them on our cluster. In this example, we run a DFT calculation to get the total energy of an FCC Si unit cell using Quantum Espresso.
-| [Examples/Job](examples/job/)            | [Get File from Job](examples/job/get-file-from-job.ipynb) | Guides you through using the Mat3ra API to query for a list of files produced by a job, describes the metadata assigned to each file, and ends by demonstrating how to download any remote file generated by a job to the local disk.
-| [Examples/Job](examples/job/)            | [Run Simulations and Extract Properties](examples/job/run-simulations-and-extract-properties.ipynb)  | Leads you through the process of copying a [bank workflow](https://docs.mat3ra.com/workflows/bank/) to your account and using it to automatically calculate the [properties](https://docs.mat3ra.com/properties/overview/) of multiple materials. In this example, we determine the [band gap](https://docs.mat3ra.com/properties-directory/non-scalar/band-gaps/) of Si and Ge.
-| [Examples/Job](examples/job/)            | [ML - Train Model Predict Properties](examples/job/ml-train-model-predict-properties.ipynb)     | Walks you through automated dataset generation and the training/prediction of material properties using [machine learning](https://docs.mat3ra.com/software-directory/overview/#machine-learning). In this example, we calculate the band gaps of Si and SiGe, and using various materials properties as descriptors, train a model to predict their band gaps. Finally, we use this trained model to predict the band gap of Ge.
+| [Examples/Job](examples/job/)            | [Get File from Job](examples/job/get-file-from-job.ipynb) | Uses the Mat3ra API to query for a list of files produced by a job, describes the metadata assigned to each file, and ends by demonstrating how to download any remote file generated by a job to the local disk.
+| [Examples/Job](examples/job/)            | [Run Simulations and Extract Properties](examples/job/run-simulations-and-extract-properties.ipynb)  | Demonstrates copying a [bank workflow](https://docs.mat3ra.com/workflows/bank/) to an account and using it to calculate the [properties](https://docs.mat3ra.com/properties/overview/) of multiple materials. In this example, we determine the [band gap](https://docs.mat3ra.com/properties-directory/non-scalar/band-gaps/) of Si and Ge.
+| [Examples/Job](examples/job/)            | [ML - Train Model Predict Properties](examples/job/ml-train-model-predict-properties.ipynb)     | Demonstrates the  generation of a training dataset and subsequent training of a [machine learning](https://docs.mat3ra.com/software-directory/overview/#machine-learning) model. In this example, we calculate the band gaps of Si and SiGe, and using various materials properties as descriptors, train a model to predict their band gaps. Finally, we use this trained model to predict the band gap of Ge.
 
 
 
 ## Setup
 
 NOTE: tested with Python version 3.8 and 3.10, please assert that the virtual environment is created with it. Use [`pyenv`](https://github.com/pyenv/pyenv#installation) to manage Python versions.
```

### Comparing `mat3ra-api-examples-2024.3.30.post3/mat3ra_api_examples.egg-info/SOURCES.txt` & `mat3ra-api-examples-2024.4.1.post0/mat3ra_api_examples.egg-info/SOURCES.txt`

 * *Files 5% similar despite different names*

```diff
@@ -17,16 +17,14 @@
 examples/job/create_and_submit_job.py
 examples/job/get-file-from-job.ipynb
 examples/job/get-file-from-job.py
 examples/job/ml-train-model-predict-properties.ipynb
 examples/job/ml-train-model-predict-properties.py
 examples/job/run-simulations-and-extract-properties.ipynb
 examples/job/run-simulations-and-extract-properties.py
-examples/material/api_interoperability_showcase.ipynb
-examples/material/api_interoperability_showcase.py
 examples/material/create_material.ipynb
 examples/material/create_material.py
 examples/material/get_materials_by_formula.ipynb
 examples/material/get_materials_by_formula.py
 examples/material/import_materials_from_materialsproject.ipynb
 examples/material/import_materials_from_materialsproject.py
 examples/material/upload_materials_from_file_poscar.ipynb
@@ -75,14 +73,16 @@
 other/materials_designer/create_interface_with_relaxation_ase_emt.ipynb
 other/materials_designer/import_material_from_jarvis_db_entry.ipynb
 other/materials_designer/import_materials_from_files.ipynb
 other/materials_designer/jupyterlite
 other/materials_designer/src/pymatgen_coherent_interface_builder.py
 other/materials_designer/src/utils.py
 other/materials_designer/uploads/README
+other/materialsproject/api_interoperability_showcase.ipynb
+other/materialsproject/api_interoperability_showcase.py
 other/python_transformations/1_layer_on_substrate.py
 other/python_transformations/2_strain_matching.py
 other/python_transformations/3_imports.py
 other/python_transformations/4_custom_transformation.py
 other/python_transformations/README.md
 other/webinar/adsorption-study.ipynb
 other/webinar/adsorption-study.py
```

### Comparing `mat3ra-api-examples-2024.3.30.post3/mkdocs.yml` & `mat3ra-api-examples-2024.4.1.post0/mkdocs.yml`

 * *Files identical despite different names*

### Comparing `mat3ra-api-examples-2024.3.30.post3/other/assets/README.md` & `mat3ra-api-examples-2024.4.1.post0/other/assets/README.md`

 * *Files identical despite different names*

### Comparing `mat3ra-api-examples-2024.3.30.post3/other/assets/bitter-sweet.csv` & `mat3ra-api-examples-2024.4.1.post0/other/assets/bitter-sweet.csv`

 * *Files identical despite different names*

### Comparing `mat3ra-api-examples-2024.3.30.post3/other/assets/gamma_alumina_digne_et_al.poscar` & `mat3ra-api-examples-2024.4.1.post0/other/assets/gamma_alumina_digne_et_al.poscar`

 * *Files identical despite different names*

### Comparing `mat3ra-api-examples-2024.3.30.post3/other/assets/sci_adv_dean_data.csv` & `mat3ra-api-examples-2024.4.1.post0/other/assets/sci_adv_dean_data.csv`

 * *Files identical despite different names*

### Comparing `mat3ra-api-examples-2024.3.30.post3/other/experiments/create_interface_with_min_energy_by_miller_indices.ipynb` & `mat3ra-api-examples-2024.4.1.post0/other/experiments/create_interface_with_min_energy_by_miller_indices.ipynb`

 * *Files identical despite different names*

### Comparing `mat3ra-api-examples-2024.3.30.post3/other/experiments/create_interface_with_relaxation_alignn.ipynb` & `mat3ra-api-examples-2024.4.1.post0/other/experiments/create_interface_with_relaxation_alignn.ipynb`

 * *Files identical despite different names*

### Comparing `mat3ra-api-examples-2024.3.30.post3/other/experiments/create_interface_with_relaxation_ase_emt.ipynb` & `mat3ra-api-examples-2024.4.1.post0/other/experiments/create_interface_with_relaxation_ase_emt.ipynb`

 * *Files identical despite different names*

### Comparing `mat3ra-api-examples-2024.3.30.post3/other/experiments/create_interface_with_relaxation_matgl_m3gnet.ipynb` & `mat3ra-api-examples-2024.4.1.post0/other/experiments/create_interface_with_relaxation_matgl_m3gnet.ipynb`

 * *Files identical despite different names*

### Comparing `mat3ra-api-examples-2024.3.30.post3/other/experiments/uploads/Gr.json` & `mat3ra-api-examples-2024.4.1.post0/other/experiments/uploads/Gr.json`

 * *Files identical despite different names*

### Comparing `mat3ra-api-examples-2024.3.30.post3/other/experiments/uploads/Ni.json` & `mat3ra-api-examples-2024.4.1.post0/other/experiments/uploads/Ni.json`

 * *Files identical despite different names*

### Comparing `mat3ra-api-examples-2024.3.30.post3/other/jarvis/import_material_from_jarvis_db_entry.ipynb` & `mat3ra-api-examples-2024.4.1.post0/other/jarvis/import_material_from_jarvis_db_entry.ipynb`

 * *Files identical despite different names*

### Comparing `mat3ra-api-examples-2024.3.30.post3/other/jarvis/run_job_using_material_from_jarvis_db.ipynb` & `mat3ra-api-examples-2024.4.1.post0/other/jarvis/run_job_using_material_from_jarvis_db.ipynb`

 * *Files identical despite different names*

### Comparing `mat3ra-api-examples-2024.3.30.post3/other/job/Smiles_Generation_Markov_Chain.py` & `mat3ra-api-examples-2024.4.1.post0/other/job/Smiles_Generation_Markov_Chain.py`

 * *Files identical despite different names*

### Comparing `mat3ra-api-examples-2024.3.30.post3/other/jupyterlite/utils.py` & `mat3ra-api-examples-2024.4.1.post0/other/jupyterlite/utils.py`

 * *Files identical despite different names*

### Comparing `mat3ra-api-examples-2024.3.30.post3/other/machine_learning/Classification_of_Bitterness_XGBoost.py` & `mat3ra-api-examples-2024.4.1.post0/other/machine_learning/Classification_of_Bitterness_XGBoost.py`

 * *Files identical despite different names*

### Comparing `mat3ra-api-examples-2024.3.30.post3/other/machine_learning/Prediction_of_Perovskite_Unit_Cell_Volume.py` & `mat3ra-api-examples-2024.4.1.post0/other/machine_learning/Prediction_of_Perovskite_Unit_Cell_Volume.py`

 * *Files identical despite different names*

### Comparing `mat3ra-api-examples-2024.3.30.post3/other/machine_learning/neural_network_train.py` & `mat3ra-api-examples-2024.4.1.post0/other/machine_learning/neural_network_train.py`

 * *Files identical despite different names*

### Comparing `mat3ra-api-examples-2024.3.30.post3/other/materials_designer/Introduction.ipynb` & `mat3ra-api-examples-2024.4.1.post0/other/materials_designer/Introduction.ipynb`

 * *Files identical despite different names*

### Comparing `mat3ra-api-examples-2024.3.30.post3/other/materials_designer/config.yml` & `mat3ra-api-examples-2024.4.1.post0/other/materials_designer/config.yml`

 * *Files identical despite different names*

### Comparing `mat3ra-api-examples-2024.3.30.post3/other/materials_designer/create_interface_with_min_strain_zsl.ipynb` & `mat3ra-api-examples-2024.4.1.post0/other/materials_designer/create_interface_with_min_strain_zsl.ipynb`

 * *Files identical despite different names*

### Comparing `mat3ra-api-examples-2024.3.30.post3/other/materials_designer/create_interface_with_relaxation_ase_emt.ipynb` & `mat3ra-api-examples-2024.4.1.post0/other/materials_designer/create_interface_with_relaxation_ase_emt.ipynb`

 * *Files identical despite different names*

### Comparing `mat3ra-api-examples-2024.3.30.post3/other/materials_designer/import_material_from_jarvis_db_entry.ipynb` & `mat3ra-api-examples-2024.4.1.post0/other/materials_designer/import_material_from_jarvis_db_entry.ipynb`

 * *Files identical despite different names*

### Comparing `mat3ra-api-examples-2024.3.30.post3/other/materials_designer/import_materials_from_files.ipynb` & `mat3ra-api-examples-2024.4.1.post0/other/materials_designer/import_materials_from_files.ipynb`

 * *Files identical despite different names*

### Comparing `mat3ra-api-examples-2024.3.30.post3/other/materials_designer/src/pymatgen_coherent_interface_builder.py` & `mat3ra-api-examples-2024.4.1.post0/other/materials_designer/src/pymatgen_coherent_interface_builder.py`

 * *Files identical despite different names*

### Comparing `mat3ra-api-examples-2024.3.30.post3/other/materials_designer/src/utils.py` & `mat3ra-api-examples-2024.4.1.post0/other/materials_designer/src/utils.py`

 * *Files identical despite different names*

### Comparing `mat3ra-api-examples-2024.3.30.post3/other/python_transformations/1_layer_on_substrate.py` & `mat3ra-api-examples-2024.4.1.post0/other/python_transformations/1_layer_on_substrate.py`

 * *Files identical despite different names*

### Comparing `mat3ra-api-examples-2024.3.30.post3/other/python_transformations/2_strain_matching.py` & `mat3ra-api-examples-2024.4.1.post0/other/python_transformations/2_strain_matching.py`

 * *Files identical despite different names*

### Comparing `mat3ra-api-examples-2024.3.30.post3/other/python_transformations/3_imports.py` & `mat3ra-api-examples-2024.4.1.post0/other/python_transformations/3_imports.py`

 * *Files identical despite different names*

### Comparing `mat3ra-api-examples-2024.3.30.post3/other/python_transformations/4_custom_transformation.py` & `mat3ra-api-examples-2024.4.1.post0/other/python_transformations/4_custom_transformation.py`

 * *Files identical despite different names*

### Comparing `mat3ra-api-examples-2024.3.30.post3/other/python_transformations/README.md` & `mat3ra-api-examples-2024.4.1.post0/other/python_transformations/README.md`

 * *Files identical despite different names*

### Comparing `mat3ra-api-examples-2024.3.30.post3/other/webinar/adsorption-study.py` & `mat3ra-api-examples-2024.4.1.post0/other/webinar/adsorption-study.py`

 * *Files identical despite different names*

### Comparing `mat3ra-api-examples-2024.3.30.post3/other/webinar/generate-al2o3-slab-structures.py` & `mat3ra-api-examples-2024.4.1.post0/other/webinar/generate-al2o3-slab-structures.py`

 * *Files identical despite different names*

### Comparing `mat3ra-api-examples-2024.3.30.post3/other/webinar/predict_with_machine_learning.py` & `mat3ra-api-examples-2024.4.1.post0/other/webinar/predict_with_machine_learning.py`

 * *Files identical despite different names*

### Comparing `mat3ra-api-examples-2024.3.30.post3/other/webinar/wulff-construction-surface-energy-study-cu.py` & `mat3ra-api-examples-2024.4.1.post0/other/webinar/wulff-construction-surface-energy-study-cu.py`

 * *Files identical despite different names*

### Comparing `mat3ra-api-examples-2024.3.30.post3/pyproject.toml` & `mat3ra-api-examples-2024.4.1.post0/pyproject.toml`

 * *Files identical despite different names*

### Comparing `mat3ra-api-examples-2024.3.30.post3/scripts/change-branch-in-urls.sh` & `mat3ra-api-examples-2024.4.1.post0/scripts/change-branch-in-urls.sh`

 * *Files identical despite different names*

### Comparing `mat3ra-api-examples-2024.3.30.post3/scripts/env.sh` & `mat3ra-api-examples-2024.4.1.post0/scripts/env.sh`

 * *Files identical despite different names*

### Comparing `mat3ra-api-examples-2024.3.30.post3/scripts/render-notebooks.sh` & `mat3ra-api-examples-2024.4.1.post0/scripts/render-notebooks.sh`

 * *Files identical despite different names*

### Comparing `mat3ra-api-examples-2024.3.30.post3/utils/generic.py` & `mat3ra-api-examples-2024.4.1.post0/utils/generic.py`

 * *Files identical despite different names*

### Comparing `mat3ra-api-examples-2024.3.30.post3/utils/material.py` & `mat3ra-api-examples-2024.4.1.post0/utils/material.py`

 * *Files identical despite different names*

### Comparing `mat3ra-api-examples-2024.3.30.post3/utils/notebook.py` & `mat3ra-api-examples-2024.4.1.post0/utils/notebook.py`

 * *Files identical despite different names*

### Comparing `mat3ra-api-examples-2024.3.30.post3/utils/settings.py` & `mat3ra-api-examples-2024.4.1.post0/utils/settings.py`

 * *Files identical despite different names*

### Comparing `mat3ra-api-examples-2024.3.30.post3/utils/web/renderjson.js` & `mat3ra-api-examples-2024.4.1.post0/utils/web/renderjson.js`

 * *Files identical despite different names*

