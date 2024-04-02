# Comparing `tmp/ccpn_project_checker-0.1.5.tar.gz` & `tmp/ccpn_project_checker-0.1.6.tar.gz`

## Comparing `ccpn_project_checker-0.1.5.tar` & `ccpn_project_checker-0.1.6.tar`

### file list

```diff
@@ -1,367 +1,367 @@
--rw-r--r--   0        0        0        8 2020-02-02 00:00:00.000000 ccpn_project_checker-0.1.5/.python-version
--rw-r--r--   0        0        0     1100 2020-02-02 00:00:00.000000 ccpn_project_checker-0.1.5/TODO.txt
--rw-r--r--   0        0        0      604 2020-02-02 00:00:00.000000 ccpn_project_checker-0.1.5/requirements-dev.lock
--rw-r--r--   0        0        0      604 2020-02-02 00:00:00.000000 ccpn_project_checker-0.1.5/requirements.lock
--rw-r--r--   0        0        0      239 2020-02-02 00:00:00.000000 ccpn_project_checker-0.1.5/project_checker/.idea/.gitignore
--rw-r--r--   0        0        0      294 2020-02-02 00:00:00.000000 ccpn_project_checker-0.1.5/project_checker/.idea/misc.xml
--rw-r--r--   0        0        0      282 2020-02-02 00:00:00.000000 ccpn_project_checker-0.1.5/project_checker/.idea/modules.xml
--rw-r--r--   0        0        0      419 2020-02-02 00:00:00.000000 ccpn_project_checker-0.1.5/project_checker/.idea/project_checker.iml
--rw-r--r--   0        0        0      235 2020-02-02 00:00:00.000000 ccpn_project_checker-0.1.5/project_checker/.idea/vcs.xml
--rw-r--r--   0        0        0    13240 2020-02-02 00:00:00.000000 ccpn_project_checker-0.1.5/project_checker/.idea/workspace.xml
--rw-r--r--   0        0        0     5453 2020-02-02 00:00:00.000000 ccpn_project_checker-0.1.5/project_checker/.idea/copilot/chatSessions/00000000000.xd
--rw-r--r--   0        0        0    13526 2020-02-02 00:00:00.000000 ccpn_project_checker-0.1.5/project_checker/.idea/copilot/chatSessions/xd.lck
--rw-r--r--   0        0        0        4 2020-02-02 00:00:00.000000 ccpn_project_checker-0.1.5/project_checker/.idea/copilot/chatSessions/blobs/version
--rw-r--r--   0        0        0      174 2020-02-02 00:00:00.000000 ccpn_project_checker-0.1.5/project_checker/.idea/inspectionProfiles/profiles_settings.xml
--rwxr-xr-x   0        0        0      197 2020-02-02 00:00:00.000000 ccpn_project_checker-0.1.5/scripts/project_checker
--rwxr-xr-x   0        0        0      276 2020-02-02 00:00:00.000000 ccpn_project_checker-0.1.5/scripts/test
--rw-r--r--   0        0        0    83487 2020-02-02 00:00:00.000000 ccpn_project_checker-0.1.5/src/project_checker/DiskModelChecker.py
--rw-r--r--   0        0        0     8665 2020-02-02 00:00:00.000000 ccpn_project_checker-0.1.5/src/project_checker/MetaModelWalker.py
--rw-r--r--   0        0        0        0 2020-02-02 00:00:00.000000 ccpn_project_checker-0.1.5/src/project_checker/__init__.py
--rw-r--r--   0        0        0      123 2020-02-02 00:00:00.000000 ccpn_project_checker-0.1.5/src/project_checker/main.py
--rw-r--r--   0        0        0    47287 2020-02-02 00:00:00.000000 ccpn_project_checker-0.1.5/src/project_checker/model_info/data_file_names.txt
--rw-r--r--   0        0        0    81462 2020-02-02 00:00:00.000000 ccpn_project_checker-0.1.5/src/project_checker/model_info/v_3_1_0_guid_to_storage_location.json
--rw-r--r--   0        0        0   527533 2020-02-02 00:00:00.000000 ccpn_project_checker-0.1.5/src/project_checker/model_info/v_3_1_0_object_info.json
--rw-r--r--   0        0        0     2256 2020-02-02 00:00:00.000000 ccpn_project_checker-0.1.5/src/project_checker/model_info/v_3_1_0_short_name_to_guid.json
--rw-r--r--   0        0        0       43 2020-02-02 00:00:00.000000 ccpn_project_checker-0.1.5/src/project_checker/optional/__init__.py
--rw-r--r--   0        0        0      814 2020-02-02 00:00:00.000000 ccpn_project_checker-0.1.5/src/project_checker/optional/abstract_optional.py
--rw-r--r--   0        0        0      305 2020-02-02 00:00:00.000000 ccpn_project_checker-0.1.5/src/project_checker/optional/compatible_abc.py
--rw-r--r--   0        0        0      133 2020-02-02 00:00:00.000000 ccpn_project_checker-0.1.5/src/project_checker/optional/exceptions.py
--rw-r--r--   0        0        0     1142 2020-02-02 00:00:00.000000 ccpn_project_checker-0.1.5/src/project_checker/optional/nothing.py
--rw-r--r--   0        0        0     1056 2020-02-02 00:00:00.000000 ccpn_project_checker-0.1.5/src/project_checker/optional/optional.py
--rw-r--r--   0        0        0     1411 2020-02-02 00:00:00.000000 ccpn_project_checker-0.1.5/src/project_checker/optional/something.py
--rw-r--r--   0        0        0   233080 2020-02-02 00:00:00.000000 ccpn_project_checker-0.1.5/src/project_checker/test_data/cli_test_output.txt
--rw-r--r--   0        0        0        0 2020-02-02 00:00:00.000000 ccpn_project_checker-0.1.5/src/project_checker/test_data/project_is_file.ccpn
--rw-r--r--   0        0        0   179478 2020-02-02 00:00:00.000000 ccpn_project_checker-0.1.5/src/project_checker/test_data/bad_memops_root_xml.ccpn/ccpnv3/memops/Implementation/bad_memops_root_xml.xml
--rw-r--r--   0        0        0      868 2020-02-02 00:00:00.000000 ccpn_project_checker-0.1.5/src/project_checker/test_data/basic_exo_links_not_found.ccpn/ccpnv3/memops/Implementation/basic_exo_links_not_found.xml
--rw-r--r--   0        0        0      499 2020-02-02 00:00:00.000000 ccpn_project_checker-0.1.5/src/project_checker/test_data/delayed_errors/bad_embedded_exo_link_0_child_elements.ccpn/ccpnv3/ccp/lims/RefSampleComponent/default+default_user_2024-02-24-15-54-35-583_00003.xml
--rw-r--r--   0        0        0      699 2020-02-02 00:00:00.000000 ccpn_project_checker-0.1.5/src/project_checker/test_data/delayed_errors/bad_embedded_exo_link_0_child_elements.ccpn/ccpnv3/ccp/lims/Sample/default+default_user_2024-02-24-15-54-35-583_00002.xml
--rw-r--r--   0        0        0      462 2020-02-02 00:00:00.000000 ccpn_project_checker-0.1.5/src/project_checker/test_data/delayed_errors/bad_embedded_exo_link_0_child_elements.ccpn/ccpnv3/ccp/molecule/MolSystem/default+default_user_2024-02-24-15-54-35-583_00004.xml
--rw-r--r--   0        0        0     3732 2020-02-02 00:00:00.000000 ccpn_project_checker-0.1.5/src/project_checker/test_data/delayed_errors/bad_embedded_exo_link_0_child_elements.ccpn/ccpnv3/ccp/nmr/Nmr/default+default_user_2024-02-24-15-54-35-583_00001.xml
--rw-r--r--   0        0        0      868 2020-02-02 00:00:00.000000 ccpn_project_checker-0.1.5/src/project_checker/test_data/delayed_errors/bad_embedded_exo_link_0_child_elements.ccpn/ccpnv3/ccpnmr/gui/Task/user+View+default_user_2024-02-24-15-54-35-583_00006.xml
--rw-r--r--   0        0        0     1014 2020-02-02 00:00:00.000000 ccpn_project_checker-0.1.5/src/project_checker/test_data/delayed_errors/bad_embedded_exo_link_0_child_elements.ccpn/ccpnv3/ccpnmr/gui/Window/_ccp_nmr_Nmr_NmrProject___default___+default_user_2024-02-24-15-54-35-583_00005.xml
--rw-r--r--   0        0        0   179440 2020-02-02 00:00:00.000000 ccpn_project_checker-0.1.5/src/project_checker/test_data/delayed_errors/bad_embedded_exo_link_0_child_elements.ccpn/ccpnv3/memops/Implementation/bad_embedded_exo_link_0_child_elements.xml
--rw-r--r--   0        0        0      499 2020-02-02 00:00:00.000000 ccpn_project_checker-0.1.5/src/project_checker/test_data/delayed_errors/bad_embedded_exo_link_0_elements.ccpn/ccpnv3/ccp/lims/RefSampleComponent/default+default_user_2024-02-24-15-54-35-583_00003.xml
--rw-r--r--   0        0        0      699 2020-02-02 00:00:00.000000 ccpn_project_checker-0.1.5/src/project_checker/test_data/delayed_errors/bad_embedded_exo_link_0_elements.ccpn/ccpnv3/ccp/lims/Sample/default+default_user_2024-02-24-15-54-35-583_00002.xml
--rw-r--r--   0        0        0      462 2020-02-02 00:00:00.000000 ccpn_project_checker-0.1.5/src/project_checker/test_data/delayed_errors/bad_embedded_exo_link_0_elements.ccpn/ccpnv3/ccp/molecule/MolSystem/default+default_user_2024-02-24-15-54-35-583_00004.xml
--rw-r--r--   0        0        0     3732 2020-02-02 00:00:00.000000 ccpn_project_checker-0.1.5/src/project_checker/test_data/delayed_errors/bad_embedded_exo_link_0_elements.ccpn/ccpnv3/ccp/nmr/Nmr/default+default_user_2024-02-24-15-54-35-583_00001.xml
--rw-r--r--   0        0        0      868 2020-02-02 00:00:00.000000 ccpn_project_checker-0.1.5/src/project_checker/test_data/delayed_errors/bad_embedded_exo_link_0_elements.ccpn/ccpnv3/ccpnmr/gui/Task/user+View+default_user_2024-02-24-15-54-35-583_00006.xml
--rw-r--r--   0        0        0     1014 2020-02-02 00:00:00.000000 ccpn_project_checker-0.1.5/src/project_checker/test_data/delayed_errors/bad_embedded_exo_link_0_elements.ccpn/ccpnv3/ccpnmr/gui/Window/_ccp_nmr_Nmr_NmrProject___default___+default_user_2024-02-24-15-54-35-583_00005.xml
--rw-r--r--   0        0        0   179355 2020-02-02 00:00:00.000000 ccpn_project_checker-0.1.5/src/project_checker/test_data/delayed_errors/bad_embedded_exo_link_0_elements.ccpn/ccpnv3/memops/Implementation/bad_embedded_exo_link_0_elements.xml
--rw-r--r--   0        0        0      499 2020-02-02 00:00:00.000000 ccpn_project_checker-0.1.5/src/project_checker/test_data/delayed_errors/bad_role_exo_link_key_element_children.ccpn/ccpnv3/ccp/lims/RefSampleComponent/default+default_user_2024-02-24-15-54-35-583_00003.xml
--rw-r--r--   0        0        0      699 2020-02-02 00:00:00.000000 ccpn_project_checker-0.1.5/src/project_checker/test_data/delayed_errors/bad_role_exo_link_key_element_children.ccpn/ccpnv3/ccp/lims/Sample/default+default_user_2024-02-24-15-54-35-583_00002.xml
--rw-r--r--   0        0        0      462 2020-02-02 00:00:00.000000 ccpn_project_checker-0.1.5/src/project_checker/test_data/delayed_errors/bad_role_exo_link_key_element_children.ccpn/ccpnv3/ccp/molecule/MolSystem/default+default_user_2024-02-24-15-54-35-583_00004.xml
--rw-r--r--   0        0        0     3732 2020-02-02 00:00:00.000000 ccpn_project_checker-0.1.5/src/project_checker/test_data/delayed_errors/bad_role_exo_link_key_element_children.ccpn/ccpnv3/ccp/nmr/Nmr/default+default_user_2024-02-24-15-54-35-583_00001.xml
--rw-r--r--   0        0        0      868 2020-02-02 00:00:00.000000 ccpn_project_checker-0.1.5/src/project_checker/test_data/delayed_errors/bad_role_exo_link_key_element_children.ccpn/ccpnv3/ccpnmr/gui/Task/user+View+default_user_2024-02-24-15-54-35-583_00006.xml
--rw-r--r--   0        0        0     1014 2020-02-02 00:00:00.000000 ccpn_project_checker-0.1.5/src/project_checker/test_data/delayed_errors/bad_role_exo_link_key_element_children.ccpn/ccpnv3/ccpnmr/gui/Window/_ccp_nmr_Nmr_NmrProject___default___+default_user_2024-02-24-15-54-35-583_00005.xml
--rw-r--r--   0        0        0   179391 2020-02-02 00:00:00.000000 ccpn_project_checker-0.1.5/src/project_checker/test_data/delayed_errors/bad_role_exo_link_key_element_children.ccpn/ccpnv3/memops/Implementation/bad_role_exo_link_key_element_children.xml
--rw-r--r--   0        0        0      499 2020-02-02 00:00:00.000000 ccpn_project_checker-0.1.5/src/project_checker/test_data/delayed_errors/bad_role_exo_link_key_element_parent.ccpn/ccpnv3/ccp/lims/RefSampleComponent/default+default_user_2024-02-24-15-54-35-583_00003.xml
--rw-r--r--   0        0        0      699 2020-02-02 00:00:00.000000 ccpn_project_checker-0.1.5/src/project_checker/test_data/delayed_errors/bad_role_exo_link_key_element_parent.ccpn/ccpnv3/ccp/lims/Sample/default+default_user_2024-02-24-15-54-35-583_00002.xml
--rw-r--r--   0        0        0      462 2020-02-02 00:00:00.000000 ccpn_project_checker-0.1.5/src/project_checker/test_data/delayed_errors/bad_role_exo_link_key_element_parent.ccpn/ccpnv3/ccp/molecule/MolSystem/default+default_user_2024-02-24-15-54-35-583_00004.xml
--rw-r--r--   0        0        0     3732 2020-02-02 00:00:00.000000 ccpn_project_checker-0.1.5/src/project_checker/test_data/delayed_errors/bad_role_exo_link_key_element_parent.ccpn/ccpnv3/ccp/nmr/Nmr/default+default_user_2024-02-24-15-54-35-583_00001.xml
--rw-r--r--   0        0        0      868 2020-02-02 00:00:00.000000 ccpn_project_checker-0.1.5/src/project_checker/test_data/delayed_errors/bad_role_exo_link_key_element_parent.ccpn/ccpnv3/ccpnmr/gui/Task/user+View+default_user_2024-02-24-15-54-35-583_00006.xml
--rw-r--r--   0        0        0     1014 2020-02-02 00:00:00.000000 ccpn_project_checker-0.1.5/src/project_checker/test_data/delayed_errors/bad_role_exo_link_key_element_parent.ccpn/ccpnv3/ccpnmr/gui/Window/_ccp_nmr_Nmr_NmrProject___default___+default_user_2024-02-24-15-54-35-583_00005.xml
--rw-r--r--   0        0        0   179486 2020-02-02 00:00:00.000000 ccpn_project_checker-0.1.5/src/project_checker/test_data/delayed_errors/bad_role_exo_link_key_element_parent.ccpn/ccpnv3/memops/Implementation/bad_role_exo_link_key_element_parent.xml
--rw-r--r--   0        0        0      499 2020-02-02 00:00:00.000000 ccpn_project_checker-0.1.5/src/project_checker/test_data/delayed_errors/bad_root_exo_link_element.ccpn/ccpnv3/ccp/lims/RefSampleComponent/default+default_user_2024-02-24-15-54-35-583_00003.xml
--rw-r--r--   0        0        0      699 2020-02-02 00:00:00.000000 ccpn_project_checker-0.1.5/src/project_checker/test_data/delayed_errors/bad_root_exo_link_element.ccpn/ccpnv3/ccp/lims/Sample/default+default_user_2024-02-24-15-54-35-583_00002.xml
--rw-r--r--   0        0        0      462 2020-02-02 00:00:00.000000 ccpn_project_checker-0.1.5/src/project_checker/test_data/delayed_errors/bad_root_exo_link_element.ccpn/ccpnv3/ccp/molecule/MolSystem/default+default_user_2024-02-24-15-54-35-583_00004.xml
--rw-r--r--   0        0        0     3732 2020-02-02 00:00:00.000000 ccpn_project_checker-0.1.5/src/project_checker/test_data/delayed_errors/bad_root_exo_link_element.ccpn/ccpnv3/ccp/nmr/Nmr/default+default_user_2024-02-24-15-54-35-583_00001.xml
--rw-r--r--   0        0        0      868 2020-02-02 00:00:00.000000 ccpn_project_checker-0.1.5/src/project_checker/test_data/delayed_errors/bad_root_exo_link_element.ccpn/ccpnv3/ccpnmr/gui/Task/user+View+default_user_2024-02-24-15-54-35-583_00006.xml
--rw-r--r--   0        0        0     1014 2020-02-02 00:00:00.000000 ccpn_project_checker-0.1.5/src/project_checker/test_data/delayed_errors/bad_root_exo_link_element.ccpn/ccpnv3/ccpnmr/gui/Window/_ccp_nmr_Nmr_NmrProject___default___+default_user_2024-02-24-15-54-35-583_00005.xml
--rw-r--r--   0        0        0   179514 2020-02-02 00:00:00.000000 ccpn_project_checker-0.1.5/src/project_checker/test_data/delayed_errors/bad_root_exo_link_element.ccpn/ccpnv3/memops/Implementation/bad_root_exo_link_element.xml
--rw-r--r--   0        0        0      499 2020-02-02 00:00:00.000000 ccpn_project_checker-0.1.5/src/project_checker/test_data/delayed_errors/empty_good_project_with_non_ccpn_letter~.ccpn/ccpnv3/ccp/lims/RefSampleComponent/default+default_user_2024-02-24-15-54-35-583_00003.xml
--rw-r--r--   0        0        0      699 2020-02-02 00:00:00.000000 ccpn_project_checker-0.1.5/src/project_checker/test_data/delayed_errors/empty_good_project_with_non_ccpn_letter~.ccpn/ccpnv3/ccp/lims/Sample/default+default_user_2024-02-24-15-54-35-583_00002.xml
--rw-r--r--   0        0        0      462 2020-02-02 00:00:00.000000 ccpn_project_checker-0.1.5/src/project_checker/test_data/delayed_errors/empty_good_project_with_non_ccpn_letter~.ccpn/ccpnv3/ccp/molecule/MolSystem/default+default_user_2024-02-24-15-54-35-583_00004.xml
--rw-r--r--   0        0        0     3732 2020-02-02 00:00:00.000000 ccpn_project_checker-0.1.5/src/project_checker/test_data/delayed_errors/empty_good_project_with_non_ccpn_letter~.ccpn/ccpnv3/ccp/nmr/Nmr/default+default_user_2024-02-24-15-54-35-583_00001.xml
--rw-r--r--   0        0        0      868 2020-02-02 00:00:00.000000 ccpn_project_checker-0.1.5/src/project_checker/test_data/delayed_errors/empty_good_project_with_non_ccpn_letter~.ccpn/ccpnv3/ccpnmr/gui/Task/user+View+default_user_2024-02-24-15-54-35-583_00006.xml
--rw-r--r--   0        0        0     1014 2020-02-02 00:00:00.000000 ccpn_project_checker-0.1.5/src/project_checker/test_data/delayed_errors/empty_good_project_with_non_ccpn_letter~.ccpn/ccpnv3/ccpnmr/gui/Window/_ccp_nmr_Nmr_NmrProject___default___+default_user_2024-02-24-15-54-35-583_00005.xml
--rw-r--r--   0        0        0   179479 2020-02-02 00:00:00.000000 ccpn_project_checker-0.1.5/src/project_checker/test_data/delayed_errors/empty_good_project_with_non_ccpn_letter~.ccpn/ccpnv3/memops/Implementation/empty_good_project_with_non_ccpn_letter~.xml
--rw-r--r--   0        0        0      499 2020-02-02 00:00:00.000000 ccpn_project_checker-0.1.5/src/project_checker/test_data/delayed_errors/exo_file_bad_root_element_name.ccpn/ccpnv3/ccp/lims/RefSampleComponent/default+default_user_2024-02-24-15-54-35-583_00003.xml
--rw-r--r--   0        0        0      699 2020-02-02 00:00:00.000000 ccpn_project_checker-0.1.5/src/project_checker/test_data/delayed_errors/exo_file_bad_root_element_name.ccpn/ccpnv3/ccp/lims/Sample/default+default_user_2024-02-24-15-54-35-583_00002.xml
--rw-r--r--   0        0        0      462 2020-02-02 00:00:00.000000 ccpn_project_checker-0.1.5/src/project_checker/test_data/delayed_errors/exo_file_bad_root_element_name.ccpn/ccpnv3/ccp/molecule/MolSystem/default+default_user_2024-02-24-15-54-35-583_00004.xml
--rw-r--r--   0        0        0     3732 2020-02-02 00:00:00.000000 ccpn_project_checker-0.1.5/src/project_checker/test_data/delayed_errors/exo_file_bad_root_element_name.ccpn/ccpnv3/ccp/nmr/Nmr/default+default_user_2024-02-24-15-54-35-583_00001.xml
--rw-r--r--   0        0        0      868 2020-02-02 00:00:00.000000 ccpn_project_checker-0.1.5/src/project_checker/test_data/delayed_errors/exo_file_bad_root_element_name.ccpn/ccpnv3/ccpnmr/gui/Task/user+View+default_user_2024-02-24-15-54-35-583_00006.xml
--rw-r--r--   0        0        0     1014 2020-02-02 00:00:00.000000 ccpn_project_checker-0.1.5/src/project_checker/test_data/delayed_errors/exo_file_bad_root_element_name.ccpn/ccpnv3/ccpnmr/gui/Window/_ccp_nmr_Nmr_NmrProject___default___+default_user_2024-02-24-15-54-35-583_00005.xml
--rw-r--r--   0        0        0   179479 2020-02-02 00:00:00.000000 ccpn_project_checker-0.1.5/src/project_checker/test_data/delayed_errors/exo_file_bad_root_element_name.ccpn/ccpnv3/memops/Implementation/exo_file_bad_root_element_name.xml
--rw-r--r--   0        0        0      499 2020-02-02 00:00:00.000000 ccpn_project_checker-0.1.5/src/project_checker/test_data/delayed_errors/exo_file_key_doesnt_match_root.ccpn/ccpnv3/ccp/lims/RefSampleComponent/default+default_user_2024-02-24-15-54-35-583_00003.xml
--rw-r--r--   0        0        0      699 2020-02-02 00:00:00.000000 ccpn_project_checker-0.1.5/src/project_checker/test_data/delayed_errors/exo_file_key_doesnt_match_root.ccpn/ccpnv3/ccp/lims/Sample/default+default_user_2024-02-24-15-54-35-583_00002.xml
--rw-r--r--   0        0        0      462 2020-02-02 00:00:00.000000 ccpn_project_checker-0.1.5/src/project_checker/test_data/delayed_errors/exo_file_key_doesnt_match_root.ccpn/ccpnv3/ccp/molecule/MolSystem/wibble+default_user_2024-02-24-15-54-35-583_00004.xml
--rw-r--r--   0        0        0     3732 2020-02-02 00:00:00.000000 ccpn_project_checker-0.1.5/src/project_checker/test_data/delayed_errors/exo_file_key_doesnt_match_root.ccpn/ccpnv3/ccp/nmr/Nmr/default+default_user_2024-02-24-15-54-35-583_00001.xml
--rw-r--r--   0        0        0      868 2020-02-02 00:00:00.000000 ccpn_project_checker-0.1.5/src/project_checker/test_data/delayed_errors/exo_file_key_doesnt_match_root.ccpn/ccpnv3/ccpnmr/gui/Task/user+View+default_user_2024-02-24-15-54-35-583_00006.xml
--rw-r--r--   0        0        0     1014 2020-02-02 00:00:00.000000 ccpn_project_checker-0.1.5/src/project_checker/test_data/delayed_errors/exo_file_key_doesnt_match_root.ccpn/ccpnv3/ccpnmr/gui/Window/_ccp_nmr_Nmr_NmrProject___default___+default_user_2024-02-24-15-54-35-583_00005.xml
--rw-r--r--   0        0        0   179479 2020-02-02 00:00:00.000000 ccpn_project_checker-0.1.5/src/project_checker/test_data/delayed_errors/exo_file_key_doesnt_match_root.ccpn/ccpnv3/memops/Implementation/exo_file_key_doesnt_match_root.xml
--rw-r--r--   0        0        0      499 2020-02-02 00:00:00.000000 ccpn_project_checker-0.1.5/src/project_checker/test_data/delayed_errors/exo_file_no_package_guid.ccpn/ccpnv3/ccp/lims/RefSampleComponent/default+default_user_2024-02-24-15-54-35-583_00003.xml
--rw-r--r--   0        0        0      699 2020-02-02 00:00:00.000000 ccpn_project_checker-0.1.5/src/project_checker/test_data/delayed_errors/exo_file_no_package_guid.ccpn/ccpnv3/ccp/lims/Sample/default+default_user_2024-02-24-15-54-35-583_00002.xml
--rw-r--r--   0        0        0      402 2020-02-02 00:00:00.000000 ccpn_project_checker-0.1.5/src/project_checker/test_data/delayed_errors/exo_file_no_package_guid.ccpn/ccpnv3/ccp/molecule/MolSystem/default+default_user_2024-02-24-15-54-35-583_00004.xml
--rw-r--r--   0        0        0     3732 2020-02-02 00:00:00.000000 ccpn_project_checker-0.1.5/src/project_checker/test_data/delayed_errors/exo_file_no_package_guid.ccpn/ccpnv3/ccp/nmr/Nmr/default+default_user_2024-02-24-15-54-35-583_00001.xml
--rw-r--r--   0        0        0      868 2020-02-02 00:00:00.000000 ccpn_project_checker-0.1.5/src/project_checker/test_data/delayed_errors/exo_file_no_package_guid.ccpn/ccpnv3/ccpnmr/gui/Task/user+View+default_user_2024-02-24-15-54-35-583_00006.xml
--rw-r--r--   0        0        0     1014 2020-02-02 00:00:00.000000 ccpn_project_checker-0.1.5/src/project_checker/test_data/delayed_errors/exo_file_no_package_guid.ccpn/ccpnv3/ccpnmr/gui/Window/_ccp_nmr_Nmr_NmrProject___default___+default_user_2024-02-24-15-54-35-583_00005.xml
--rw-r--r--   0        0        0   179479 2020-02-02 00:00:00.000000 ccpn_project_checker-0.1.5/src/project_checker/test_data/delayed_errors/exo_file_no_package_guid.ccpn/ccpnv3/memops/Implementation/exo_file_no_package_guid.xml
--rw-r--r--   0        0        0      499 2020-02-02 00:00:00.000000 ccpn_project_checker-0.1.5/src/project_checker/test_data/delayed_errors/exo_file_release_attrib_invalid.ccpn/ccpnv3/ccp/lims/RefSampleComponent/default+default_user_2024-02-24-15-54-35-583_00003.xml
--rw-r--r--   0        0        0      699 2020-02-02 00:00:00.000000 ccpn_project_checker-0.1.5/src/project_checker/test_data/delayed_errors/exo_file_release_attrib_invalid.ccpn/ccpnv3/ccp/lims/Sample/default+default_user_2024-02-24-15-54-35-583_00002.xml
--rw-r--r--   0        0        0      463 2020-02-02 00:00:00.000000 ccpn_project_checker-0.1.5/src/project_checker/test_data/delayed_errors/exo_file_release_attrib_invalid.ccpn/ccpnv3/ccp/molecule/MolSystem/default+default_user_2024-02-24-15-54-35-583_00004.xml
--rw-r--r--   0        0        0     3732 2020-02-02 00:00:00.000000 ccpn_project_checker-0.1.5/src/project_checker/test_data/delayed_errors/exo_file_release_attrib_invalid.ccpn/ccpnv3/ccp/nmr/Nmr/default+default_user_2024-02-24-15-54-35-583_00001.xml
--rw-r--r--   0        0        0      868 2020-02-02 00:00:00.000000 ccpn_project_checker-0.1.5/src/project_checker/test_data/delayed_errors/exo_file_release_attrib_invalid.ccpn/ccpnv3/ccpnmr/gui/Task/user+View+default_user_2024-02-24-15-54-35-583_00006.xml
--rw-r--r--   0        0        0     1014 2020-02-02 00:00:00.000000 ccpn_project_checker-0.1.5/src/project_checker/test_data/delayed_errors/exo_file_release_attrib_invalid.ccpn/ccpnv3/ccpnmr/gui/Window/_ccp_nmr_Nmr_NmrProject___default___+default_user_2024-02-24-15-54-35-583_00005.xml
--rw-r--r--   0        0        0   179479 2020-02-02 00:00:00.000000 ccpn_project_checker-0.1.5/src/project_checker/test_data/delayed_errors/exo_file_release_attrib_invalid.ccpn/ccpnv3/memops/Implementation/exo_file_release_attrib_invalid.xml
--rw-r--r--   0        0        0      499 2020-02-02 00:00:00.000000 ccpn_project_checker-0.1.5/src/project_checker/test_data/delayed_errors/exo_file_release_attrib_missing.ccpn/ccpnv3/ccp/lims/RefSampleComponent/default+default_user_2024-02-24-15-54-35-583_00003.xml
--rw-r--r--   0        0        0      699 2020-02-02 00:00:00.000000 ccpn_project_checker-0.1.5/src/project_checker/test_data/delayed_errors/exo_file_release_attrib_missing.ccpn/ccpnv3/ccp/lims/Sample/default+default_user_2024-02-24-15-54-35-583_00002.xml
--rw-r--r--   0        0        0      465 2020-02-02 00:00:00.000000 ccpn_project_checker-0.1.5/src/project_checker/test_data/delayed_errors/exo_file_release_attrib_missing.ccpn/ccpnv3/ccp/molecule/MolSystem/default+default_user_2024-02-24-15-54-35-583_00004.xml
--rw-r--r--   0        0        0     3732 2020-02-02 00:00:00.000000 ccpn_project_checker-0.1.5/src/project_checker/test_data/delayed_errors/exo_file_release_attrib_missing.ccpn/ccpnv3/ccp/nmr/Nmr/default+default_user_2024-02-24-15-54-35-583_00001.xml
--rw-r--r--   0        0        0      868 2020-02-02 00:00:00.000000 ccpn_project_checker-0.1.5/src/project_checker/test_data/delayed_errors/exo_file_release_attrib_missing.ccpn/ccpnv3/ccpnmr/gui/Task/user+View+default_user_2024-02-24-15-54-35-583_00006.xml
--rw-r--r--   0        0        0     1014 2020-02-02 00:00:00.000000 ccpn_project_checker-0.1.5/src/project_checker/test_data/delayed_errors/exo_file_release_attrib_missing.ccpn/ccpnv3/ccpnmr/gui/Window/_ccp_nmr_Nmr_NmrProject___default___+default_user_2024-02-24-15-54-35-583_00005.xml
--rw-r--r--   0        0        0   179479 2020-02-02 00:00:00.000000 ccpn_project_checker-0.1.5/src/project_checker/test_data/delayed_errors/exo_file_release_attrib_missing.ccpn/ccpnv3/memops/Implementation/exo_file_release_attrib_missing.xml
--rw-r--r--   0        0        0      499 2020-02-02 00:00:00.000000 ccpn_project_checker-0.1.5/src/project_checker/test_data/delayed_errors/exo_file_release_doesnt_match_root.ccpn/ccpnv3/ccp/lims/RefSampleComponent/default+default_user_2024-02-24-15-54-35-583_00003.xml
--rw-r--r--   0        0        0      699 2020-02-02 00:00:00.000000 ccpn_project_checker-0.1.5/src/project_checker/test_data/delayed_errors/exo_file_release_doesnt_match_root.ccpn/ccpnv3/ccp/lims/Sample/default+default_user_2024-02-24-15-54-35-583_00002.xml
--rw-r--r--   0        0        0      462 2020-02-02 00:00:00.000000 ccpn_project_checker-0.1.5/src/project_checker/test_data/delayed_errors/exo_file_release_doesnt_match_root.ccpn/ccpnv3/ccp/molecule/MolSystem/default+default_user_2024-02-24-15-54-35-583_00004.xml
--rw-r--r--   0        0        0     3732 2020-02-02 00:00:00.000000 ccpn_project_checker-0.1.5/src/project_checker/test_data/delayed_errors/exo_file_release_doesnt_match_root.ccpn/ccpnv3/ccp/nmr/Nmr/default+default_user_2024-02-24-15-54-35-583_00001.xml
--rw-r--r--   0        0        0      868 2020-02-02 00:00:00.000000 ccpn_project_checker-0.1.5/src/project_checker/test_data/delayed_errors/exo_file_release_doesnt_match_root.ccpn/ccpnv3/ccpnmr/gui/Task/user+View+default_user_2024-02-24-15-54-35-583_00006.xml
--rw-r--r--   0        0        0     1014 2020-02-02 00:00:00.000000 ccpn_project_checker-0.1.5/src/project_checker/test_data/delayed_errors/exo_file_release_doesnt_match_root.ccpn/ccpnv3/ccpnmr/gui/Window/_ccp_nmr_Nmr_NmrProject___default___+default_user_2024-02-24-15-54-35-583_00005.xml
--rw-r--r--   0        0        0   179479 2020-02-02 00:00:00.000000 ccpn_project_checker-0.1.5/src/project_checker/test_data/delayed_errors/exo_file_release_doesnt_match_root.ccpn/ccpnv3/memops/Implementation/exo_file_release_doesnt_match_root.xml
--rw-r--r--   0        0        0      499 2020-02-02 00:00:00.000000 ccpn_project_checker-0.1.5/src/project_checker/test_data/delayed_errors/exo_file_short_name_guid_doesnt_match_package_guid.ccpn/ccpnv3/ccp/lims/RefSampleComponent/default+default_user_2024-02-24-15-54-35-583_00003.xml
--rw-r--r--   0        0        0      699 2020-02-02 00:00:00.000000 ccpn_project_checker-0.1.5/src/project_checker/test_data/delayed_errors/exo_file_short_name_guid_doesnt_match_package_guid.ccpn/ccpnv3/ccp/lims/Sample/default+default_user_2024-02-24-15-54-35-583_00002.xml
--rw-r--r--   0        0        0      462 2020-02-02 00:00:00.000000 ccpn_project_checker-0.1.5/src/project_checker/test_data/delayed_errors/exo_file_short_name_guid_doesnt_match_package_guid.ccpn/ccpnv3/ccp/molecule/MolSystem/default+default_user_2024-02-24-15-54-35-583_00004.xml
--rw-r--r--   0        0        0     3732 2020-02-02 00:00:00.000000 ccpn_project_checker-0.1.5/src/project_checker/test_data/delayed_errors/exo_file_short_name_guid_doesnt_match_package_guid.ccpn/ccpnv3/ccp/nmr/Nmr/default+default_user_2024-02-24-15-54-35-583_00001.xml
--rw-r--r--   0        0        0      868 2020-02-02 00:00:00.000000 ccpn_project_checker-0.1.5/src/project_checker/test_data/delayed_errors/exo_file_short_name_guid_doesnt_match_package_guid.ccpn/ccpnv3/ccpnmr/gui/Task/user+View+default_user_2024-02-24-15-54-35-583_00006.xml
--rw-r--r--   0        0        0     1014 2020-02-02 00:00:00.000000 ccpn_project_checker-0.1.5/src/project_checker/test_data/delayed_errors/exo_file_short_name_guid_doesnt_match_package_guid.ccpn/ccpnv3/ccpnmr/gui/Window/_ccp_nmr_Nmr_NmrProject___default___+default_user_2024-02-24-15-54-35-583_00005.xml
--rw-r--r--   0        0        0   179479 2020-02-02 00:00:00.000000 ccpn_project_checker-0.1.5/src/project_checker/test_data/delayed_errors/exo_file_short_name_guid_doesnt_match_package_guid.ccpn/ccpnv3/memops/Implementation/exo_file_short_name_guid_doesnt_match_package_guid.xml
--rw-r--r--   0        0        0      499 2020-02-02 00:00:00.000000 ccpn_project_checker-0.1.5/src/project_checker/test_data/delayed_errors/exo_file_time_attrib_invalid.ccpn/ccpnv3/ccp/lims/RefSampleComponent/default+default_user_2024-02-24-15-54-35-583_00003.xml
--rw-r--r--   0        0        0      699 2020-02-02 00:00:00.000000 ccpn_project_checker-0.1.5/src/project_checker/test_data/delayed_errors/exo_file_time_attrib_invalid.ccpn/ccpnv3/ccp/lims/Sample/default+default_user_2024-02-24-15-54-35-583_00002.xml
--rw-r--r--   0        0        0      444 2020-02-02 00:00:00.000000 ccpn_project_checker-0.1.5/src/project_checker/test_data/delayed_errors/exo_file_time_attrib_invalid.ccpn/ccpnv3/ccp/molecule/MolSystem/default+default_user_2024-02-24-15-54-35-583_00004.xml
--rw-r--r--   0        0        0     3732 2020-02-02 00:00:00.000000 ccpn_project_checker-0.1.5/src/project_checker/test_data/delayed_errors/exo_file_time_attrib_invalid.ccpn/ccpnv3/ccp/nmr/Nmr/default+default_user_2024-02-24-15-54-35-583_00001.xml
--rw-r--r--   0        0        0      868 2020-02-02 00:00:00.000000 ccpn_project_checker-0.1.5/src/project_checker/test_data/delayed_errors/exo_file_time_attrib_invalid.ccpn/ccpnv3/ccpnmr/gui/Task/user+View+default_user_2024-02-24-15-54-35-583_00006.xml
--rw-r--r--   0        0        0     1014 2020-02-02 00:00:00.000000 ccpn_project_checker-0.1.5/src/project_checker/test_data/delayed_errors/exo_file_time_attrib_invalid.ccpn/ccpnv3/ccpnmr/gui/Window/_ccp_nmr_Nmr_NmrProject___default___+default_user_2024-02-24-15-54-35-583_00005.xml
--rw-r--r--   0        0        0   179479 2020-02-02 00:00:00.000000 ccpn_project_checker-0.1.5/src/project_checker/test_data/delayed_errors/exo_file_time_attrib_invalid.ccpn/ccpnv3/memops/Implementation/exo_file_time_attrib_invalid.xml
--rw-r--r--   0        0        0      499 2020-02-02 00:00:00.000000 ccpn_project_checker-0.1.5/src/project_checker/test_data/delayed_errors/exo_file_time_attrib_missing.ccpn/ccpnv3/ccp/lims/RefSampleComponent/default+default_user_2024-02-24-15-54-35-583_00003.xml
--rw-r--r--   0        0        0      699 2020-02-02 00:00:00.000000 ccpn_project_checker-0.1.5/src/project_checker/test_data/delayed_errors/exo_file_time_attrib_missing.ccpn/ccpnv3/ccp/lims/Sample/default+default_user_2024-02-24-15-54-35-583_00002.xml
--rw-r--r--   0        0        0      465 2020-02-02 00:00:00.000000 ccpn_project_checker-0.1.5/src/project_checker/test_data/delayed_errors/exo_file_time_attrib_missing.ccpn/ccpnv3/ccp/molecule/MolSystem/default+default_user_2024-02-24-15-54-35-583_00004.xml
--rw-r--r--   0        0        0     3732 2020-02-02 00:00:00.000000 ccpn_project_checker-0.1.5/src/project_checker/test_data/delayed_errors/exo_file_time_attrib_missing.ccpn/ccpnv3/ccp/nmr/Nmr/default+default_user_2024-02-24-15-54-35-583_00001.xml
--rw-r--r--   0        0        0      868 2020-02-02 00:00:00.000000 ccpn_project_checker-0.1.5/src/project_checker/test_data/delayed_errors/exo_file_time_attrib_missing.ccpn/ccpnv3/ccpnmr/gui/Task/user+View+default_user_2024-02-24-15-54-35-583_00006.xml
--rw-r--r--   0        0        0     1014 2020-02-02 00:00:00.000000 ccpn_project_checker-0.1.5/src/project_checker/test_data/delayed_errors/exo_file_time_attrib_missing.ccpn/ccpnv3/ccpnmr/gui/Window/_ccp_nmr_Nmr_NmrProject___default___+default_user_2024-02-24-15-54-35-583_00005.xml
--rw-r--r--   0        0        0   179479 2020-02-02 00:00:00.000000 ccpn_project_checker-0.1.5/src/project_checker/test_data/delayed_errors/exo_file_time_attrib_missing.ccpn/ccpnv3/memops/Implementation/exo_file_time_attrib_missing.xml
--rw-r--r--   0        0        0      499 2020-02-02 00:00:00.000000 ccpn_project_checker-0.1.5/src/project_checker/test_data/delayed_errors/exo_file_unknown_package_guid.ccpn/ccpnv3/ccp/lims/RefSampleComponent/default+default_user_2024-02-24-15-54-35-583_00003.xml
--rw-r--r--   0        0        0      699 2020-02-02 00:00:00.000000 ccpn_project_checker-0.1.5/src/project_checker/test_data/delayed_errors/exo_file_unknown_package_guid.ccpn/ccpnv3/ccp/lims/Sample/default+default_user_2024-02-24-15-54-35-583_00002.xml
--rw-r--r--   0        0        0      466 2020-02-02 00:00:00.000000 ccpn_project_checker-0.1.5/src/project_checker/test_data/delayed_errors/exo_file_unknown_package_guid.ccpn/ccpnv3/ccp/molecule/MolSystem/default+default_user_2024-02-24-15-54-35-583_00004.xml
--rw-r--r--   0        0        0     3732 2020-02-02 00:00:00.000000 ccpn_project_checker-0.1.5/src/project_checker/test_data/delayed_errors/exo_file_unknown_package_guid.ccpn/ccpnv3/ccp/nmr/Nmr/default+default_user_2024-02-24-15-54-35-583_00001.xml
--rw-r--r--   0        0        0      868 2020-02-02 00:00:00.000000 ccpn_project_checker-0.1.5/src/project_checker/test_data/delayed_errors/exo_file_unknown_package_guid.ccpn/ccpnv3/ccpnmr/gui/Task/user+View+default_user_2024-02-24-15-54-35-583_00006.xml
--rw-r--r--   0        0        0     1014 2020-02-02 00:00:00.000000 ccpn_project_checker-0.1.5/src/project_checker/test_data/delayed_errors/exo_file_unknown_package_guid.ccpn/ccpnv3/ccpnmr/gui/Window/_ccp_nmr_Nmr_NmrProject___default___+default_user_2024-02-24-15-54-35-583_00005.xml
--rw-r--r--   0        0        0   179479 2020-02-02 00:00:00.000000 ccpn_project_checker-0.1.5/src/project_checker/test_data/delayed_errors/exo_file_unknown_package_guid.ccpn/ccpnv3/memops/Implementation/exo_file_unknown_package_guid.xml
--rw-r--r--   0        0        0      499 2020-02-02 00:00:00.000000 ccpn_project_checker-0.1.5/src/project_checker/test_data/delayed_errors/exo_file_unknown_short_package_name.ccpn/ccpnv3/ccp/lims/RefSampleComponent/default+default_user_2024-02-24-15-54-35-583_00003.xml
--rw-r--r--   0        0        0      699 2020-02-02 00:00:00.000000 ccpn_project_checker-0.1.5/src/project_checker/test_data/delayed_errors/exo_file_unknown_short_package_name.ccpn/ccpnv3/ccp/lims/Sample/default+default_user_2024-02-24-15-54-35-583_00002.xml
--rw-r--r--   0        0        0      464 2020-02-02 00:00:00.000000 ccpn_project_checker-0.1.5/src/project_checker/test_data/delayed_errors/exo_file_unknown_short_package_name.ccpn/ccpnv3/ccp/molecule/MolSystem/default+default_user_2024-02-24-15-54-35-583_00004.xml
--rw-r--r--   0        0        0     3732 2020-02-02 00:00:00.000000 ccpn_project_checker-0.1.5/src/project_checker/test_data/delayed_errors/exo_file_unknown_short_package_name.ccpn/ccpnv3/ccp/nmr/Nmr/default+default_user_2024-02-24-15-54-35-583_00001.xml
--rw-r--r--   0        0        0      868 2020-02-02 00:00:00.000000 ccpn_project_checker-0.1.5/src/project_checker/test_data/delayed_errors/exo_file_unknown_short_package_name.ccpn/ccpnv3/ccpnmr/gui/Task/user+View+default_user_2024-02-24-15-54-35-583_00006.xml
--rw-r--r--   0        0        0     1014 2020-02-02 00:00:00.000000 ccpn_project_checker-0.1.5/src/project_checker/test_data/delayed_errors/exo_file_unknown_short_package_name.ccpn/ccpnv3/ccpnmr/gui/Window/_ccp_nmr_Nmr_NmrProject___default___+default_user_2024-02-24-15-54-35-583_00005.xml
--rw-r--r--   0        0        0   179479 2020-02-02 00:00:00.000000 ccpn_project_checker-0.1.5/src/project_checker/test_data/delayed_errors/exo_file_unknown_short_package_name.ccpn/ccpnv3/memops/Implementation/exo_file_unknown_short_package_name.xml
--rw-r--r--   0        0        0      499 2020-02-02 00:00:00.000000 ccpn_project_checker-0.1.5/src/project_checker/test_data/delayed_errors/exo_file_wrong_storage_location.ccpn/ccpnv3/ccp/lims/RefSampleComponent/default+default_user_2024-02-24-15-54-35-583_00003.xml
--rw-r--r--   0        0        0      699 2020-02-02 00:00:00.000000 ccpn_project_checker-0.1.5/src/project_checker/test_data/delayed_errors/exo_file_wrong_storage_location.ccpn/ccpnv3/ccp/lims/Sample/default+default_user_2024-02-24-15-54-35-583_00002.xml
--rw-r--r--   0        0        0     3732 2020-02-02 00:00:00.000000 ccpn_project_checker-0.1.5/src/project_checker/test_data/delayed_errors/exo_file_wrong_storage_location.ccpn/ccpnv3/ccp/nmr/Nmr/default+default_user_2024-02-24-15-54-35-583_00001.xml
--rw-r--r--   0        0        0      462 2020-02-02 00:00:00.000000 ccpn_project_checker-0.1.5/src/project_checker/test_data/delayed_errors/exo_file_wrong_storage_location.ccpn/ccpnv3/ccp/nmr/Nmr/default+default_user_2024-02-24-15-54-35-583_00004.xml
--rw-r--r--   0        0        0      868 2020-02-02 00:00:00.000000 ccpn_project_checker-0.1.5/src/project_checker/test_data/delayed_errors/exo_file_wrong_storage_location.ccpn/ccpnv3/ccpnmr/gui/Task/user+View+default_user_2024-02-24-15-54-35-583_00006.xml
--rw-r--r--   0        0        0     1014 2020-02-02 00:00:00.000000 ccpn_project_checker-0.1.5/src/project_checker/test_data/delayed_errors/exo_file_wrong_storage_location.ccpn/ccpnv3/ccpnmr/gui/Window/_ccp_nmr_Nmr_NmrProject___default___+default_user_2024-02-24-15-54-35-583_00005.xml
--rw-r--r--   0        0        0   179479 2020-02-02 00:00:00.000000 ccpn_project_checker-0.1.5/src/project_checker/test_data/delayed_errors/exo_file_wrong_storage_location.ccpn/ccpnv3/memops/Implementation/exo_file_wrong_storage_location.xml
--rw-r--r--   0        0        0      499 2020-02-02 00:00:00.000000 ccpn_project_checker-0.1.5/src/project_checker/test_data/delayed_errors/exo_link_no_top_object.ccpn/ccpnv3/ccp/lims/RefSampleComponent/default+default_user_2024-02-24-15-54-35-583_00003.xml
--rw-r--r--   0        0        0      699 2020-02-02 00:00:00.000000 ccpn_project_checker-0.1.5/src/project_checker/test_data/delayed_errors/exo_link_no_top_object.ccpn/ccpnv3/ccp/lims/Sample/default+default_user_2024-02-24-15-54-35-583_00002.xml
--rw-r--r--   0        0        0      235 2020-02-02 00:00:00.000000 ccpn_project_checker-0.1.5/src/project_checker/test_data/delayed_errors/exo_link_no_top_object.ccpn/ccpnv3/ccp/molecule/MolSystem/default+default_user_2024-02-24-15-54-35-583_00004.xml
--rw-r--r--   0        0        0     3732 2020-02-02 00:00:00.000000 ccpn_project_checker-0.1.5/src/project_checker/test_data/delayed_errors/exo_link_no_top_object.ccpn/ccpnv3/ccp/nmr/Nmr/default+default_user_2024-02-24-15-54-35-583_00001.xml
--rw-r--r--   0        0        0      868 2020-02-02 00:00:00.000000 ccpn_project_checker-0.1.5/src/project_checker/test_data/delayed_errors/exo_link_no_top_object.ccpn/ccpnv3/ccpnmr/gui/Task/user+View+default_user_2024-02-24-15-54-35-583_00006.xml
--rw-r--r--   0        0        0     1014 2020-02-02 00:00:00.000000 ccpn_project_checker-0.1.5/src/project_checker/test_data/delayed_errors/exo_link_no_top_object.ccpn/ccpnv3/ccpnmr/gui/Window/_ccp_nmr_Nmr_NmrProject___default___+default_user_2024-02-24-15-54-35-583_00005.xml
--rw-r--r--   0        0        0   179479 2020-02-02 00:00:00.000000 ccpn_project_checker-0.1.5/src/project_checker/test_data/delayed_errors/exo_link_no_top_object.ccpn/ccpnv3/memops/Implementation/exo_link_no_top_object.xml
--rw-r--r--   0        0        0      499 2020-02-02 00:00:00.000000 ccpn_project_checker-0.1.5/src/project_checker/test_data/delayed_errors/exo_link_too_many_top_objects.ccpn/ccpnv3/ccp/lims/RefSampleComponent/default+default_user_2024-02-24-15-54-35-583_00003.xml
--rw-r--r--   0        0        0      699 2020-02-02 00:00:00.000000 ccpn_project_checker-0.1.5/src/project_checker/test_data/delayed_errors/exo_link_too_many_top_objects.ccpn/ccpnv3/ccp/lims/Sample/default+default_user_2024-02-24-15-54-35-583_00002.xml
--rw-r--r--   0        0        0      513 2020-02-02 00:00:00.000000 ccpn_project_checker-0.1.5/src/project_checker/test_data/delayed_errors/exo_link_too_many_top_objects.ccpn/ccpnv3/ccp/molecule/MolSystem/default+default_user_2024-02-24-15-54-35-583_00004.xml
--rw-r--r--   0        0        0     3732 2020-02-02 00:00:00.000000 ccpn_project_checker-0.1.5/src/project_checker/test_data/delayed_errors/exo_link_too_many_top_objects.ccpn/ccpnv3/ccp/nmr/Nmr/default+default_user_2024-02-24-15-54-35-583_00001.xml
--rw-r--r--   0        0        0      868 2020-02-02 00:00:00.000000 ccpn_project_checker-0.1.5/src/project_checker/test_data/delayed_errors/exo_link_too_many_top_objects.ccpn/ccpnv3/ccpnmr/gui/Task/user+View+default_user_2024-02-24-15-54-35-583_00006.xml
--rw-r--r--   0        0        0     1014 2020-02-02 00:00:00.000000 ccpn_project_checker-0.1.5/src/project_checker/test_data/delayed_errors/exo_link_too_many_top_objects.ccpn/ccpnv3/ccpnmr/gui/Window/_ccp_nmr_Nmr_NmrProject___default___+default_user_2024-02-24-15-54-35-583_00005.xml
--rw-r--r--   0        0        0   179479 2020-02-02 00:00:00.000000 ccpn_project_checker-0.1.5/src/project_checker/test_data/delayed_errors/exo_link_too_many_top_objects.ccpn/ccpnv3/memops/Implementation/exo_link_too_many_top_objects.xml
--rw-r--r--   0        0        0      499 2020-02-02 00:00:00.000000 ccpn_project_checker-0.1.5/src/project_checker/test_data/delayed_errors/exo_linked_file_bad_xml.ccpn/ccpnv3/ccp/lims/RefSampleComponent/default+default_user_2024-02-24-15-54-35-583_00003.xml
--rw-r--r--   0        0        0      699 2020-02-02 00:00:00.000000 ccpn_project_checker-0.1.5/src/project_checker/test_data/delayed_errors/exo_linked_file_bad_xml.ccpn/ccpnv3/ccp/lims/Sample/default+default_user_2024-02-24-15-54-35-583_00002.xml
--rw-r--r--   0        0        0      461 2020-02-02 00:00:00.000000 ccpn_project_checker-0.1.5/src/project_checker/test_data/delayed_errors/exo_linked_file_bad_xml.ccpn/ccpnv3/ccp/molecule/MolSystem/default+default_user_2024-02-24-15-54-35-583_00004.xml
--rw-r--r--   0        0        0     3732 2020-02-02 00:00:00.000000 ccpn_project_checker-0.1.5/src/project_checker/test_data/delayed_errors/exo_linked_file_bad_xml.ccpn/ccpnv3/ccp/nmr/Nmr/default+default_user_2024-02-24-15-54-35-583_00001.xml
--rw-r--r--   0        0        0      868 2020-02-02 00:00:00.000000 ccpn_project_checker-0.1.5/src/project_checker/test_data/delayed_errors/exo_linked_file_bad_xml.ccpn/ccpnv3/ccpnmr/gui/Task/user+View+default_user_2024-02-24-15-54-35-583_00006.xml
--rw-r--r--   0        0        0     1014 2020-02-02 00:00:00.000000 ccpn_project_checker-0.1.5/src/project_checker/test_data/delayed_errors/exo_linked_file_bad_xml.ccpn/ccpnv3/ccpnmr/gui/Window/_ccp_nmr_Nmr_NmrProject___default___+default_user_2024-02-24-15-54-35-583_00005.xml
--rw-r--r--   0        0        0   179479 2020-02-02 00:00:00.000000 ccpn_project_checker-0.1.5/src/project_checker/test_data/delayed_errors/exo_linked_file_bad_xml.ccpn/ccpnv3/memops/Implementation/exo_linked_file_bad_xml.xml
--rw-r--r--   0        0        0      499 2020-02-02 00:00:00.000000 ccpn_project_checker-0.1.5/src/project_checker/test_data/delayed_errors/exo_linked_file_missing.ccpn/ccpnv3/ccp/lims/RefSampleComponent/default+default_user_2024-02-24-15-54-35-583_00003.xml
--rw-r--r--   0        0        0      699 2020-02-02 00:00:00.000000 ccpn_project_checker-0.1.5/src/project_checker/test_data/delayed_errors/exo_linked_file_missing.ccpn/ccpnv3/ccp/lims/Sample/default+default_user_2024-02-24-15-54-35-583_00002.xml
--rw-r--r--   0        0        0        0 2020-02-02 00:00:00.000000 ccpn_project_checker-0.1.5/src/project_checker/test_data/delayed_errors/exo_linked_file_missing.ccpn/ccpnv3/ccp/molecule/MolSystem/.keep_alive
--rw-r--r--   0        0        0     3732 2020-02-02 00:00:00.000000 ccpn_project_checker-0.1.5/src/project_checker/test_data/delayed_errors/exo_linked_file_missing.ccpn/ccpnv3/ccp/nmr/Nmr/default+default_user_2024-02-24-15-54-35-583_00001.xml
--rw-r--r--   0        0        0      868 2020-02-02 00:00:00.000000 ccpn_project_checker-0.1.5/src/project_checker/test_data/delayed_errors/exo_linked_file_missing.ccpn/ccpnv3/ccpnmr/gui/Task/user+View+default_user_2024-02-24-15-54-35-583_00006.xml
--rw-r--r--   0        0        0     1014 2020-02-02 00:00:00.000000 ccpn_project_checker-0.1.5/src/project_checker/test_data/delayed_errors/exo_linked_file_missing.ccpn/ccpnv3/ccpnmr/gui/Window/_ccp_nmr_Nmr_NmrProject___default___+default_user_2024-02-24-15-54-35-583_00005.xml
--rw-r--r--   0        0        0   179479 2020-02-02 00:00:00.000000 ccpn_project_checker-0.1.5/src/project_checker/test_data/delayed_errors/exo_linked_file_missing.ccpn/ccpnv3/memops/Implementation/exo_linked_file_missing.xml
--rw-r--r--   0        0        0      499 2020-02-02 00:00:00.000000 ccpn_project_checker-0.1.5/src/project_checker/test_data/delayed_errors/exo_linked_file_no_storage_unit.ccpn/ccpnv3/ccp/lims/RefSampleComponent/default+default_user_2024-02-24-15-54-35-583_00003.xml
--rw-r--r--   0        0        0      699 2020-02-02 00:00:00.000000 ccpn_project_checker-0.1.5/src/project_checker/test_data/delayed_errors/exo_linked_file_no_storage_unit.ccpn/ccpnv3/ccp/lims/Sample/default+default_user_2024-02-24-15-54-35-583_00002.xml
--rw-r--r--   0        0        0      466 2020-02-02 00:00:00.000000 ccpn_project_checker-0.1.5/src/project_checker/test_data/delayed_errors/exo_linked_file_no_storage_unit.ccpn/ccpnv3/ccp/molecule/MolSystem/default+default_user_2024-02-24-15-54-35-583_00004.xml
--rw-r--r--   0        0        0     3732 2020-02-02 00:00:00.000000 ccpn_project_checker-0.1.5/src/project_checker/test_data/delayed_errors/exo_linked_file_no_storage_unit.ccpn/ccpnv3/ccp/nmr/Nmr/default+default_user_2024-02-24-15-54-35-583_00001.xml
--rw-r--r--   0        0        0      868 2020-02-02 00:00:00.000000 ccpn_project_checker-0.1.5/src/project_checker/test_data/delayed_errors/exo_linked_file_no_storage_unit.ccpn/ccpnv3/ccpnmr/gui/Task/user+View+default_user_2024-02-24-15-54-35-583_00006.xml
--rw-r--r--   0        0        0     1014 2020-02-02 00:00:00.000000 ccpn_project_checker-0.1.5/src/project_checker/test_data/delayed_errors/exo_linked_file_no_storage_unit.ccpn/ccpnv3/ccpnmr/gui/Window/_ccp_nmr_Nmr_NmrProject___default___+default_user_2024-02-24-15-54-35-583_00005.xml
--rw-r--r--   0        0        0   179479 2020-02-02 00:00:00.000000 ccpn_project_checker-0.1.5/src/project_checker/test_data/delayed_errors/exo_linked_file_no_storage_unit.ccpn/ccpnv3/memops/Implementation/exo_linked_file_no_storage_unit.xml
--rw-r--r--   0        0        0      499 2020-02-02 00:00:00.000000 ccpn_project_checker-0.1.5/src/project_checker/test_data/delayed_errors/exo_links_with_keys_outside_ccpn_character_set.ccpn/ccpnv3/ccp/lims/RefSampleComponent/default+default_user_2024-02-24-15-54-35-583_00003.xml
--rw-r--r--   0        0        0      699 2020-02-02 00:00:00.000000 ccpn_project_checker-0.1.5/src/project_checker/test_data/delayed_errors/exo_links_with_keys_outside_ccpn_character_set.ccpn/ccpnv3/ccp/lims/Sample/default+default_user_2024-02-24-15-54-35-583_00002.xml
--rw-r--r--   0        0        0      462 2020-02-02 00:00:00.000000 ccpn_project_checker-0.1.5/src/project_checker/test_data/delayed_errors/exo_links_with_keys_outside_ccpn_character_set.ccpn/ccpnv3/ccp/molecule/MolSystem/default+default_user_2024-02-24-15-54-35-583_00004.xml
--rw-r--r--   0        0        0     3732 2020-02-02 00:00:00.000000 ccpn_project_checker-0.1.5/src/project_checker/test_data/delayed_errors/exo_links_with_keys_outside_ccpn_character_set.ccpn/ccpnv3/ccp/nmr/Nmr/default+default_user_2024-02-24-15-54-35-583_00001.xml
--rw-r--r--   0        0        0      868 2020-02-02 00:00:00.000000 ccpn_project_checker-0.1.5/src/project_checker/test_data/delayed_errors/exo_links_with_keys_outside_ccpn_character_set.ccpn/ccpnv3/ccpnmr/gui/Task/user+View~+default_user_2024-02-24-15-54-35-583_00006.xml
--rw-r--r--   0        0        0     1014 2020-02-02 00:00:00.000000 ccpn_project_checker-0.1.5/src/project_checker/test_data/delayed_errors/exo_links_with_keys_outside_ccpn_character_set.ccpn/ccpnv3/ccpnmr/gui/Window/_ccp_nmr_Nmr_NmrProject___default___+default_user_2024-02-24-15-54-35-583_00005.xml
--rw-r--r--   0        0        0   179571 2020-02-02 00:00:00.000000 ccpn_project_checker-0.1.5/src/project_checker/test_data/delayed_errors/exo_links_with_keys_outside_ccpn_character_set.ccpn/ccpnv3/memops/Implementation/exo_links_with_keys_outside_ccpn_character_set.xml
--rw-r--r--   0        0        0      499 2020-02-02 00:00:00.000000 ccpn_project_checker-0.1.5/src/project_checker/test_data/delayed_errors/external_guid_doesnt_match_internal.ccpn/ccpnv3/ccp/lims/RefSampleComponent/default+default_user_2024-02-24-15-54-35-583_00003.xml
--rw-r--r--   0        0        0      699 2020-02-02 00:00:00.000000 ccpn_project_checker-0.1.5/src/project_checker/test_data/delayed_errors/external_guid_doesnt_match_internal.ccpn/ccpnv3/ccp/lims/Sample/default+default_user_2024-02-24-15-54-35-583_00002.xml
--rw-r--r--   0        0        0      451 2020-02-02 00:00:00.000000 ccpn_project_checker-0.1.5/src/project_checker/test_data/delayed_errors/external_guid_doesnt_match_internal.ccpn/ccpnv3/ccp/molecule/MolSystem/default+default_user_2024-02-24-15-54-35-583_00004.xml
--rw-r--r--   0        0        0     3732 2020-02-02 00:00:00.000000 ccpn_project_checker-0.1.5/src/project_checker/test_data/delayed_errors/external_guid_doesnt_match_internal.ccpn/ccpnv3/ccp/nmr/Nmr/default+default_user_2024-02-24-15-54-35-583_00001.xml
--rw-r--r--   0        0        0      868 2020-02-02 00:00:00.000000 ccpn_project_checker-0.1.5/src/project_checker/test_data/delayed_errors/external_guid_doesnt_match_internal.ccpn/ccpnv3/ccpnmr/gui/Task/user+View+default_user_2024-02-24-15-54-35-583_00006.xml
--rw-r--r--   0        0        0     1014 2020-02-02 00:00:00.000000 ccpn_project_checker-0.1.5/src/project_checker/test_data/delayed_errors/external_guid_doesnt_match_internal.ccpn/ccpnv3/ccpnmr/gui/Window/_ccp_nmr_Nmr_NmrProject___default___+default_user_2024-02-24-15-54-35-583_00005.xml
--rw-r--r--   0        0        0   179479 2020-02-02 00:00:00.000000 ccpn_project_checker-0.1.5/src/project_checker/test_data/delayed_errors/external_guid_doesnt_match_internal.ccpn/ccpnv3/memops/Implementation/external_guid_doesnt_match_internal.xml
--rw-r--r--   0        0        0      499 2020-02-02 00:00:00.000000 ccpn_project_checker-0.1.5/src/project_checker/test_data/delayed_errors/root_exo_link_missing_source_element.ccpn/ccpnv3/ccp/lims/RefSampleComponent/default+default_user_2024-02-24-15-54-35-583_00003.xml
--rw-r--r--   0        0        0      699 2020-02-02 00:00:00.000000 ccpn_project_checker-0.1.5/src/project_checker/test_data/delayed_errors/root_exo_link_missing_source_element.ccpn/ccpnv3/ccp/lims/Sample/default+default_user_2024-02-24-15-54-35-583_00002.xml
--rw-r--r--   0        0        0      462 2020-02-02 00:00:00.000000 ccpn_project_checker-0.1.5/src/project_checker/test_data/delayed_errors/root_exo_link_missing_source_element.ccpn/ccpnv3/ccp/molecule/MolSystem/default+default_user_2024-02-24-15-54-35-583_00004.xml
--rw-r--r--   0        0        0     3732 2020-02-02 00:00:00.000000 ccpn_project_checker-0.1.5/src/project_checker/test_data/delayed_errors/root_exo_link_missing_source_element.ccpn/ccpnv3/ccp/nmr/Nmr/default+default_user_2024-02-24-15-54-35-583_00001.xml
--rw-r--r--   0        0        0      868 2020-02-02 00:00:00.000000 ccpn_project_checker-0.1.5/src/project_checker/test_data/delayed_errors/root_exo_link_missing_source_element.ccpn/ccpnv3/ccpnmr/gui/Task/user+View+default_user_2024-02-24-15-54-35-583_00006.xml
--rw-r--r--   0        0        0     1014 2020-02-02 00:00:00.000000 ccpn_project_checker-0.1.5/src/project_checker/test_data/delayed_errors/root_exo_link_missing_source_element.ccpn/ccpnv3/ccpnmr/gui/Window/_ccp_nmr_Nmr_NmrProject___default___+default_user_2024-02-24-15-54-35-583_00005.xml
--rw-r--r--   0        0        0   179486 2020-02-02 00:00:00.000000 ccpn_project_checker-0.1.5/src/project_checker/test_data/delayed_errors/root_exo_link_missing_source_element.ccpn/ccpnv3/memops/Implementation/root_exo_link_missing_source_element.xml
--rw-r--r--   0        0        0      499 2020-02-02 00:00:00.000000 ccpn_project_checker-0.1.5/src/project_checker/test_data/delayed_errors/root_exo_link_too_many_source_elements.ccpn/ccpnv3/ccp/lims/RefSampleComponent/default+default_user_2024-02-24-15-54-35-583_00003.xml
--rw-r--r--   0        0        0      699 2020-02-02 00:00:00.000000 ccpn_project_checker-0.1.5/src/project_checker/test_data/delayed_errors/root_exo_link_too_many_source_elements.ccpn/ccpnv3/ccp/lims/Sample/default+default_user_2024-02-24-15-54-35-583_00002.xml
--rw-r--r--   0        0        0      462 2020-02-02 00:00:00.000000 ccpn_project_checker-0.1.5/src/project_checker/test_data/delayed_errors/root_exo_link_too_many_source_elements.ccpn/ccpnv3/ccp/molecule/MolSystem/default+default_user_2024-02-24-15-54-35-583_00004.xml
--rw-r--r--   0        0        0     3732 2020-02-02 00:00:00.000000 ccpn_project_checker-0.1.5/src/project_checker/test_data/delayed_errors/root_exo_link_too_many_source_elements.ccpn/ccpnv3/ccp/nmr/Nmr/default+default_user_2024-02-24-15-54-35-583_00001.xml
--rw-r--r--   0        0        0      868 2020-02-02 00:00:00.000000 ccpn_project_checker-0.1.5/src/project_checker/test_data/delayed_errors/root_exo_link_too_many_source_elements.ccpn/ccpnv3/ccpnmr/gui/Task/user+View+default_user_2024-02-24-15-54-35-583_00006.xml
--rw-r--r--   0        0        0     1014 2020-02-02 00:00:00.000000 ccpn_project_checker-0.1.5/src/project_checker/test_data/delayed_errors/root_exo_link_too_many_source_elements.ccpn/ccpnv3/ccpnmr/gui/Window/_ccp_nmr_Nmr_NmrProject___default___+default_user_2024-02-24-15-54-35-583_00005.xml
--rw-r--r--   0        0        0   179777 2020-02-02 00:00:00.000000 ccpn_project_checker-0.1.5/src/project_checker/test_data/delayed_errors/root_exo_link_too_many_source_elements.ccpn/ccpnv3/memops/Implementation/root_exo_link_too_many_source_elements.xml
--rw-r--r--   0        0        0        0 2020-02-02 00:00:00.000000 ccpn_project_checker-0.1.5/src/project_checker/test_data/empty_Implementation.ccpn/ccpnv3/memops/Implementation/.keep_alive
--rw-r--r--   0        0        0        0 2020-02-02 00:00:00.000000 ccpn_project_checker-0.1.5/src/project_checker/test_data/empty_ccpnv3.ccpn/ccpnv3/.keep_alive
--rw-r--r--   0        0        0      499 2020-02-02 00:00:00.000000 ccpn_project_checker-0.1.5/src/project_checker/test_data/empty_good_project_multiple_root_xml_files.ccpn/ccpnv3/ccp/lims/RefSampleComponent/default+default_user_2024-02-24-15-54-35-583_00003.xml
--rw-r--r--   0        0        0      699 2020-02-02 00:00:00.000000 ccpn_project_checker-0.1.5/src/project_checker/test_data/empty_good_project_multiple_root_xml_files.ccpn/ccpnv3/ccp/lims/Sample/default+default_user_2024-02-24-15-54-35-583_00002.xml
--rw-r--r--   0        0        0      462 2020-02-02 00:00:00.000000 ccpn_project_checker-0.1.5/src/project_checker/test_data/empty_good_project_multiple_root_xml_files.ccpn/ccpnv3/ccp/molecule/MolSystem/default+default_user_2024-02-24-15-54-35-583_00004.xml
--rw-r--r--   0        0        0     3732 2020-02-02 00:00:00.000000 ccpn_project_checker-0.1.5/src/project_checker/test_data/empty_good_project_multiple_root_xml_files.ccpn/ccpnv3/ccp/nmr/Nmr/default+default_user_2024-02-24-15-54-35-583_00001.xml
--rw-r--r--   0        0        0      868 2020-02-02 00:00:00.000000 ccpn_project_checker-0.1.5/src/project_checker/test_data/empty_good_project_multiple_root_xml_files.ccpn/ccpnv3/ccpnmr/gui/Task/user+View+default_user_2024-02-24-15-54-35-583_00006.xml
--rw-r--r--   0        0        0     1014 2020-02-02 00:00:00.000000 ccpn_project_checker-0.1.5/src/project_checker/test_data/empty_good_project_multiple_root_xml_files.ccpn/ccpnv3/ccpnmr/gui/Window/_ccp_nmr_Nmr_NmrProject___default___+default_user_2024-02-24-15-54-35-583_00005.xml
--rw-r--r--   0        0        0   179503 2020-02-02 00:00:00.000000 ccpn_project_checker-0.1.5/src/project_checker/test_data/empty_good_project_multiple_root_xml_files.ccpn/ccpnv3/memops/Implementation/empty_good_project_mutiple_root_xml_files_1.xml
--rw-r--r--   0        0        0   179503 2020-02-02 00:00:00.000000 ccpn_project_checker-0.1.5/src/project_checker/test_data/empty_good_project_multiple_root_xml_files.ccpn/ccpnv3/memops/Implementation/empty_good_project_mutiple_root_xml_files_2.xml
--rw-r--r--   0        0        0        0 2020-02-02 00:00:00.000000 ccpn_project_checker-0.1.5/src/project_checker/test_data/empty_project/.keep_alive
--rw-r--r--   0        0        0        0 2020-02-02 00:00:00.000000 ccpn_project_checker-0.1.5/src/project_checker/test_data/empty_project.ccpn/.keep_alive
--rw-r--r--   0        0        0        0 2020-02-02 00:00:00.000000 ccpn_project_checker-0.1.5/src/project_checker/test_data/empty_project_no_extension_ccpn/.keep_alive
--rw-r--r--   0        0        0      257 2020-02-02 00:00:00.000000 ccpn_project_checker-0.1.5/src/project_checker/test_data/empty_storage_unit.ccpn/ccpnv3/memops/Implementation/empty_storage_unit.xml
--rw-r--r--   0        0        0     1710 2020-02-02 00:00:00.000000 ccpn_project_checker-0.1.5/src/project_checker/test_data/good_projects/Sec5Part4.ccpn/ccpnv3/ccp/general/DataLocation/standard+default_user_2022-02-23-14-57-20-615_00001.xml
--rw-r--r--   0        0        0     1614 2020-02-02 00:00:00.000000 ccpn_project_checker-0.1.5/src/project_checker/test_data/good_projects/Sec5Part4.ccpn/ccpnv3/ccp/general/DataLocation/standard+default_user_2022-02-23-14-57-20-615_00001.xml.bak
--rw-r--r--   0        0        0     1501 2020-02-02 00:00:00.000000 ccpn_project_checker-0.1.5/src/project_checker/test_data/good_projects/Sec5Part4.ccpn/ccpnv3/ccp/lims/RefSampleComponent/default+default_user_2022-02-23-14-57-20-616_00003.xml
--rw-r--r--   0        0        0     1500 2020-02-02 00:00:00.000000 ccpn_project_checker-0.1.5/src/project_checker/test_data/good_projects/Sec5Part4.ccpn/ccpnv3/ccp/lims/RefSampleComponent/default+default_user_2022-02-23-14-57-20-616_00003.xml.bak
--rw-r--r--   0        0        0      699 2020-02-02 00:00:00.000000 ccpn_project_checker-0.1.5/src/project_checker/test_data/good_projects/Sec5Part4.ccpn/ccpnv3/ccp/lims/Sample/default+default_user_2022-02-23-14-57-20-616_00002.xml
--rw-r--r--   0        0        0  1148277 2020-02-02 00:00:00.000000 ccpn_project_checker-0.1.5/src/project_checker/test_data/good_projects/Sec5Part4.ccpn/ccpnv3/ccp/molecule/MolSystem/default+default_user_2022-02-23-14-57-20-617_00001.xml
--rw-r--r--   0        0        0  1146139 2020-02-02 00:00:00.000000 ccpn_project_checker-0.1.5/src/project_checker/test_data/good_projects/Sec5Part4.ccpn/ccpnv3/ccp/molecule/MolSystem/default+default_user_2022-02-23-14-57-20-617_00001.xml.bak
--rw-r--r--   0        0        0    76531 2020-02-02 00:00:00.000000 ccpn_project_checker-0.1.5/src/project_checker/test_data/good_projects/Sec5Part4.ccpn/ccpnv3/ccp/molecule/Molecule/Sec5+Sec5Part1_user_2022-02-23-15-20-24-415_00001.xml
--rw-r--r--   0        0        0  2057337 2020-02-02 00:00:00.000000 ccpn_project_checker-0.1.5/src/project_checker/test_data/good_projects/Sec5Part4.ccpn/ccpnv3/ccp/nmr/Nmr/default+default_user_2022-02-23-14-57-20-616_00001.xml
--rw-r--r--   0        0        0  2055804 2020-02-02 00:00:00.000000 ccpn_project_checker-0.1.5/src/project_checker/test_data/good_projects/Sec5Part4.ccpn/ccpnv3/ccp/nmr/Nmr/default+default_user_2022-02-23-14-57-20-616_00001.xml.bak
--rw-r--r--   0        0        0    14319 2020-02-02 00:00:00.000000 ccpn_project_checker-0.1.5/src/project_checker/test_data/good_projects/Sec5Part4.ccpn/ccpnv3/ccpnmr/gui/Task/user+View+default_user_2022-02-23-14-57-20-617_00003.xml
--rw-r--r--   0        0        0    11440 2020-02-02 00:00:00.000000 ccpn_project_checker-0.1.5/src/project_checker/test_data/good_projects/Sec5Part4.ccpn/ccpnv3/ccpnmr/gui/Task/user+View+default_user_2022-02-23-14-57-20-617_00003.xml.bak
--rw-r--r--   0        0        0     1021 2020-02-02 00:00:00.000000 ccpn_project_checker-0.1.5/src/project_checker/test_data/good_projects/Sec5Part4.ccpn/ccpnv3/ccpnmr/gui/Window/_ccp_nmr_Nmr_NmrProject___default___+default_user_2022-02-23-14-57-20-617_00002.xml
--rw-r--r--   0        0        0     1020 2020-02-02 00:00:00.000000 ccpn_project_checker-0.1.5/src/project_checker/test_data/good_projects/Sec5Part4.ccpn/ccpnv3/ccpnmr/gui/Window/_ccp_nmr_Nmr_NmrProject___default___+default_user_2022-02-23-14-57-20-617_00002.xml.bak
--rw-r--r--   0        0        0   182235 2020-02-02 00:00:00.000000 ccpn_project_checker-0.1.5/src/project_checker/test_data/good_projects/Sec5Part4.ccpn/ccpnv3/memops/Implementation/Sec5Part4.xml
--rw-r--r--   0        0        0   347669 2020-02-02 00:00:00.000000 ccpn_project_checker-0.1.5/src/project_checker/test_data/good_projects/Sec5Part4.ccpn/ccpnv3/memops/Implementation/Sec5Part4.xml.bak
--rw-r--r--   0        0        0      499 2020-02-02 00:00:00.000000 ccpn_project_checker-0.1.5/src/project_checker/test_data/good_projects/empty_good_project.ccpn/ccpnv3/ccp/lims/RefSampleComponent/default+default_user_2024-02-24-15-54-35-583_00003.xml
--rw-r--r--   0        0        0      699 2020-02-02 00:00:00.000000 ccpn_project_checker-0.1.5/src/project_checker/test_data/good_projects/empty_good_project.ccpn/ccpnv3/ccp/lims/Sample/default+default_user_2024-02-24-15-54-35-583_00002.xml
--rw-r--r--   0        0        0      462 2020-02-02 00:00:00.000000 ccpn_project_checker-0.1.5/src/project_checker/test_data/good_projects/empty_good_project.ccpn/ccpnv3/ccp/molecule/MolSystem/default+default_user_2024-02-24-15-54-35-583_00004.xml
--rw-r--r--   0        0        0     3732 2020-02-02 00:00:00.000000 ccpn_project_checker-0.1.5/src/project_checker/test_data/good_projects/empty_good_project.ccpn/ccpnv3/ccp/nmr/Nmr/default+default_user_2024-02-24-15-54-35-583_00001.xml
--rw-r--r--   0        0        0      868 2020-02-02 00:00:00.000000 ccpn_project_checker-0.1.5/src/project_checker/test_data/good_projects/empty_good_project.ccpn/ccpnv3/ccpnmr/gui/Task/user+View+default_user_2024-02-24-15-54-35-583_00006.xml
--rw-r--r--   0        0        0     1014 2020-02-02 00:00:00.000000 ccpn_project_checker-0.1.5/src/project_checker/test_data/good_projects/empty_good_project.ccpn/ccpnv3/ccpnmr/gui/Window/_ccp_nmr_Nmr_NmrProject___default___+default_user_2024-02-24-15-54-35-583_00005.xml
--rw-r--r--   0        0        0   179479 2020-02-02 00:00:00.000000 ccpn_project_checker-0.1.5/src/project_checker/test_data/good_projects/empty_good_project.ccpn/ccpnv3/memops/Implementation/empty_good_project.xml
--rw-r--r--   0        0        0      499 2020-02-02 00:00:00.000000 ccpn_project_checker-0.1.5/src/project_checker/test_data/good_projects/empty_good_project_renamed.ccpn/ccpnv3/ccp/lims/RefSampleComponent/default+default_user_2024-02-24-15-54-35-583_00003.xml
--rw-r--r--   0        0        0      699 2020-02-02 00:00:00.000000 ccpn_project_checker-0.1.5/src/project_checker/test_data/good_projects/empty_good_project_renamed.ccpn/ccpnv3/ccp/lims/Sample/default+default_user_2024-02-24-15-54-35-583_00002.xml
--rw-r--r--   0        0        0      462 2020-02-02 00:00:00.000000 ccpn_project_checker-0.1.5/src/project_checker/test_data/good_projects/empty_good_project_renamed.ccpn/ccpnv3/ccp/molecule/MolSystem/default+default_user_2024-02-24-15-54-35-583_00004.xml
--rw-r--r--   0        0        0     3732 2020-02-02 00:00:00.000000 ccpn_project_checker-0.1.5/src/project_checker/test_data/good_projects/empty_good_project_renamed.ccpn/ccpnv3/ccp/nmr/Nmr/default+default_user_2024-02-24-15-54-35-583_00001.xml
--rw-r--r--   0        0        0      868 2020-02-02 00:00:00.000000 ccpn_project_checker-0.1.5/src/project_checker/test_data/good_projects/empty_good_project_renamed.ccpn/ccpnv3/ccpnmr/gui/Task/user+View+default_user_2024-02-24-15-54-35-583_00006.xml
--rw-r--r--   0        0        0     1014 2020-02-02 00:00:00.000000 ccpn_project_checker-0.1.5/src/project_checker/test_data/good_projects/empty_good_project_renamed.ccpn/ccpnv3/ccpnmr/gui/Window/_ccp_nmr_Nmr_NmrProject___default___+default_user_2024-02-24-15-54-35-583_00005.xml
--rw-r--r--   0        0        0   179479 2020-02-02 00:00:00.000000 ccpn_project_checker-0.1.5/src/project_checker/test_data/good_projects/empty_good_project_renamed.ccpn/ccpnv3/memops/Implementation/empty_good_project_renamed.xml
--rw-r--r--   0        0        0      499 2020-02-02 00:00:00.000000 ccpn_project_checker-0.1.5/src/project_checker/test_data/memops_root_no_read_empty_good_project.ccpn/ccpnv3/ccp/lims/RefSampleComponent/default+default_user_2024-02-24-15-54-35-583_00003.xml
--rw-r--r--   0        0        0      699 2020-02-02 00:00:00.000000 ccpn_project_checker-0.1.5/src/project_checker/test_data/memops_root_no_read_empty_good_project.ccpn/ccpnv3/ccp/lims/Sample/default+default_user_2024-02-24-15-54-35-583_00002.xml
--rw-r--r--   0        0        0      462 2020-02-02 00:00:00.000000 ccpn_project_checker-0.1.5/src/project_checker/test_data/memops_root_no_read_empty_good_project.ccpn/ccpnv3/ccp/molecule/MolSystem/default+default_user_2024-02-24-15-54-35-583_00004.xml
--rw-r--r--   0        0        0     3732 2020-02-02 00:00:00.000000 ccpn_project_checker-0.1.5/src/project_checker/test_data/memops_root_no_read_empty_good_project.ccpn/ccpnv3/ccp/nmr/Nmr/default+default_user_2024-02-24-15-54-35-583_00001.xml
--rw-r--r--   0        0        0      868 2020-02-02 00:00:00.000000 ccpn_project_checker-0.1.5/src/project_checker/test_data/memops_root_no_read_empty_good_project.ccpn/ccpnv3/ccpnmr/gui/Task/user+View+default_user_2024-02-24-15-54-35-583_00006.xml
--rw-r--r--   0        0        0     1014 2020-02-02 00:00:00.000000 ccpn_project_checker-0.1.5/src/project_checker/test_data/memops_root_no_read_empty_good_project.ccpn/ccpnv3/ccpnmr/gui/Window/_ccp_nmr_Nmr_NmrProject___default___+default_user_2024-02-24-15-54-35-583_00005.xml
--rw-r--r--   0        0        0   179479 2020-02-02 00:00:00.000000 ccpn_project_checker-0.1.5/src/project_checker/test_data/memops_root_no_read_empty_good_project.ccpn/ccpnv3/memops/Implementation/memops_root_no_read_empty_good_project.xml
--rw-r--r--   0        0        0   179483 2020-02-02 00:00:00.000000 ccpn_project_checker-0.1.5/src/project_checker/test_data/memops_root_no_storage_unit.ccpn/ccpnv3/memops/Implementation/memops_root_no_storage_unit.xml
--rw-r--r--   0        0        0        0 2020-02-02 00:00:00.000000 ccpn_project_checker-0.1.5/src/project_checker/test_data/memops_root_xml_is_directory.ccpn/ccpnv3/memops/Implementation/memops_root_xml_is_directory.xml/.keep_alive
--rw-r--r--   0        0        0      455 2020-02-02 00:00:00.000000 ccpn_project_checker-0.1.5/src/project_checker/test_data/no_exo_links.ccpn/ccpnv3/memops/Implementation/no_exo_links.xml
--rw-r--r--   0        0        0      499 2020-02-02 00:00:00.000000 ccpn_project_checker-0.1.5/src/project_checker/test_data/no_memops_root_element.ccpn/ccpnv3/ccp/lims/RefSampleComponent/default+default_user_2024-02-24-15-54-35-583_00003.xml
--rw-r--r--   0        0        0      699 2020-02-02 00:00:00.000000 ccpn_project_checker-0.1.5/src/project_checker/test_data/no_memops_root_element.ccpn/ccpnv3/ccp/lims/Sample/default+default_user_2024-02-24-15-54-35-583_00002.xml
--rw-r--r--   0        0        0      462 2020-02-02 00:00:00.000000 ccpn_project_checker-0.1.5/src/project_checker/test_data/no_memops_root_element.ccpn/ccpnv3/ccp/molecule/MolSystem/default+default_user_2024-02-24-15-54-35-583_00004.xml
--rw-r--r--   0        0        0     3732 2020-02-02 00:00:00.000000 ccpn_project_checker-0.1.5/src/project_checker/test_data/no_memops_root_element.ccpn/ccpnv3/ccp/nmr/Nmr/default+default_user_2024-02-24-15-54-35-583_00001.xml
--rw-r--r--   0        0        0      868 2020-02-02 00:00:00.000000 ccpn_project_checker-0.1.5/src/project_checker/test_data/no_memops_root_element.ccpn/ccpnv3/ccpnmr/gui/Task/user+View+default_user_2024-02-24-15-54-35-583_00006.xml
--rw-r--r--   0        0        0     1014 2020-02-02 00:00:00.000000 ccpn_project_checker-0.1.5/src/project_checker/test_data/no_memops_root_element.ccpn/ccpnv3/ccpnmr/gui/Window/_ccp_nmr_Nmr_NmrProject___default___+default_user_2024-02-24-15-54-35-583_00005.xml
--rw-r--r--   0        0        0   179485 2020-02-02 00:00:00.000000 ccpn_project_checker-0.1.5/src/project_checker/test_data/no_memops_root_element.ccpn/ccpnv3/memops/Implementation/no_memops_root_element.xml
--rw-r--r--   0        0        0        0 2020-02-02 00:00:00.000000 ccpn_project_checker-0.1.5/src/project_checker/test_data/no_read_ccpnv3.ccpn/ccpnv3/.keep_alive
--rw-r--r--   0        0        0        0 2020-02-02 00:00:00.000000 ccpn_project_checker-0.1.5/src/project_checker/test_data/no_read_empty_project.ccpn/.keep_alive
--rw-r--r--   0        0        0      499 2020-02-02 00:00:00.000000 ccpn_project_checker-0.1.5/src/project_checker/test_data/root_not_memops_root_element.ccpn/ccpnv3/ccp/lims/RefSampleComponent/default+default_user_2024-02-24-15-54-35-583_00003.xml
--rw-r--r--   0        0        0      699 2020-02-02 00:00:00.000000 ccpn_project_checker-0.1.5/src/project_checker/test_data/root_not_memops_root_element.ccpn/ccpnv3/ccp/lims/Sample/default+default_user_2024-02-24-15-54-35-583_00002.xml
--rw-r--r--   0        0        0      462 2020-02-02 00:00:00.000000 ccpn_project_checker-0.1.5/src/project_checker/test_data/root_not_memops_root_element.ccpn/ccpnv3/ccp/molecule/MolSystem/default+default_user_2024-02-24-15-54-35-583_00004.xml
--rw-r--r--   0        0        0     3732 2020-02-02 00:00:00.000000 ccpn_project_checker-0.1.5/src/project_checker/test_data/root_not_memops_root_element.ccpn/ccpnv3/ccp/nmr/Nmr/default+default_user_2024-02-24-15-54-35-583_00001.xml
--rw-r--r--   0        0        0      868 2020-02-02 00:00:00.000000 ccpn_project_checker-0.1.5/src/project_checker/test_data/root_not_memops_root_element.ccpn/ccpnv3/ccpnmr/gui/Task/user+View+default_user_2024-02-24-15-54-35-583_00006.xml
--rw-r--r--   0        0        0     1014 2020-02-02 00:00:00.000000 ccpn_project_checker-0.1.5/src/project_checker/test_data/root_not_memops_root_element.ccpn/ccpnv3/ccpnmr/gui/Window/_ccp_nmr_Nmr_NmrProject___default___+default_user_2024-02-24-15-54-35-583_00005.xml
--rw-r--r--   0        0        0   179485 2020-02-02 00:00:00.000000 ccpn_project_checker-0.1.5/src/project_checker/test_data/root_not_memops_root_element.ccpn/ccpnv3/memops/Implementation/root_not_memops_root_element.xml
--rw-r--r--   0        0        0      499 2020-02-02 00:00:00.000000 ccpn_project_checker-0.1.5/src/project_checker/test_data/root_version_badly_formatted.ccpn/ccpnv3/ccp/lims/RefSampleComponent/default+default_user_2024-02-24-15-54-35-583_00003.xml
--rw-r--r--   0        0        0      699 2020-02-02 00:00:00.000000 ccpn_project_checker-0.1.5/src/project_checker/test_data/root_version_badly_formatted.ccpn/ccpnv3/ccp/lims/Sample/default+default_user_2024-02-24-15-54-35-583_00002.xml
--rw-r--r--   0        0        0      462 2020-02-02 00:00:00.000000 ccpn_project_checker-0.1.5/src/project_checker/test_data/root_version_badly_formatted.ccpn/ccpnv3/ccp/molecule/MolSystem/default+default_user_2024-02-24-15-54-35-583_00004.xml
--rw-r--r--   0        0        0     3732 2020-02-02 00:00:00.000000 ccpn_project_checker-0.1.5/src/project_checker/test_data/root_version_badly_formatted.ccpn/ccpnv3/ccp/nmr/Nmr/default+default_user_2024-02-24-15-54-35-583_00001.xml
--rw-r--r--   0        0        0      868 2020-02-02 00:00:00.000000 ccpn_project_checker-0.1.5/src/project_checker/test_data/root_version_badly_formatted.ccpn/ccpnv3/ccpnmr/gui/Task/user+View+default_user_2024-02-24-15-54-35-583_00006.xml
--rw-r--r--   0        0        0     1014 2020-02-02 00:00:00.000000 ccpn_project_checker-0.1.5/src/project_checker/test_data/root_version_badly_formatted.ccpn/ccpnv3/ccpnmr/gui/Window/_ccp_nmr_Nmr_NmrProject___default___+default_user_2024-02-24-15-54-35-583_00005.xml
--rw-r--r--   0        0        0   179480 2020-02-02 00:00:00.000000 ccpn_project_checker-0.1.5/src/project_checker/test_data/root_version_badly_formatted.ccpn/ccpnv3/memops/Implementation/root_version_badly_formatted.xml
--rw-r--r--   0        0        0      499 2020-02-02 00:00:00.000000 ccpn_project_checker-0.1.5/src/project_checker/test_data/root_version_missing.ccpn/ccpnv3/ccp/lims/RefSampleComponent/default+default_user_2024-02-24-15-54-35-583_00003.xml
--rw-r--r--   0        0        0      699 2020-02-02 00:00:00.000000 ccpn_project_checker-0.1.5/src/project_checker/test_data/root_version_missing.ccpn/ccpnv3/ccp/lims/Sample/default+default_user_2024-02-24-15-54-35-583_00002.xml
--rw-r--r--   0        0        0      462 2020-02-02 00:00:00.000000 ccpn_project_checker-0.1.5/src/project_checker/test_data/root_version_missing.ccpn/ccpnv3/ccp/molecule/MolSystem/default+default_user_2024-02-24-15-54-35-583_00004.xml
--rw-r--r--   0        0        0     3732 2020-02-02 00:00:00.000000 ccpn_project_checker-0.1.5/src/project_checker/test_data/root_version_missing.ccpn/ccpnv3/ccp/nmr/Nmr/default+default_user_2024-02-24-15-54-35-583_00001.xml
--rw-r--r--   0        0        0      868 2020-02-02 00:00:00.000000 ccpn_project_checker-0.1.5/src/project_checker/test_data/root_version_missing.ccpn/ccpnv3/ccpnmr/gui/Task/user+View+default_user_2024-02-24-15-54-35-583_00006.xml
--rw-r--r--   0        0        0     1014 2020-02-02 00:00:00.000000 ccpn_project_checker-0.1.5/src/project_checker/test_data/root_version_missing.ccpn/ccpnv3/ccpnmr/gui/Window/_ccp_nmr_Nmr_NmrProject___default___+default_user_2024-02-24-15-54-35-583_00005.xml
--rw-r--r--   0        0        0   179482 2020-02-02 00:00:00.000000 ccpn_project_checker-0.1.5/src/project_checker/test_data/root_version_missing.ccpn/ccpnv3/memops/Implementation/root_version_missing.xml
--rw-r--r--   0        0        0      499 2020-02-02 00:00:00.000000 ccpn_project_checker-0.1.5/src/project_checker/test_data/too_many_root_elements.ccpn/ccpnv3/ccp/lims/RefSampleComponent/default+default_user_2024-02-24-15-54-35-583_00003.xml
--rw-r--r--   0        0        0      699 2020-02-02 00:00:00.000000 ccpn_project_checker-0.1.5/src/project_checker/test_data/too_many_root_elements.ccpn/ccpnv3/ccp/lims/Sample/default+default_user_2024-02-24-15-54-35-583_00002.xml
--rw-r--r--   0        0        0      462 2020-02-02 00:00:00.000000 ccpn_project_checker-0.1.5/src/project_checker/test_data/too_many_root_elements.ccpn/ccpnv3/ccp/molecule/MolSystem/default+default_user_2024-02-24-15-54-35-583_00004.xml
--rw-r--r--   0        0        0     3732 2020-02-02 00:00:00.000000 ccpn_project_checker-0.1.5/src/project_checker/test_data/too_many_root_elements.ccpn/ccpnv3/ccp/nmr/Nmr/default+default_user_2024-02-24-15-54-35-583_00001.xml
--rw-r--r--   0        0        0      868 2020-02-02 00:00:00.000000 ccpn_project_checker-0.1.5/src/project_checker/test_data/too_many_root_elements.ccpn/ccpnv3/ccpnmr/gui/Task/user+View+default_user_2024-02-24-15-54-35-583_00006.xml
--rw-r--r--   0        0        0     1014 2020-02-02 00:00:00.000000 ccpn_project_checker-0.1.5/src/project_checker/test_data/too_many_root_elements.ccpn/ccpnv3/ccpnmr/gui/Window/_ccp_nmr_Nmr_NmrProject___default___+default_user_2024-02-24-15-54-35-583_00005.xml
--rw-r--r--   0        0        0      438 2020-02-02 00:00:00.000000 ccpn_project_checker-0.1.5/src/project_checker/test_data/too_many_root_elements.ccpn/ccpnv3/memops/Implementation/too_many_root_elements.xml
--rw-r--r--   0        0        0      499 2020-02-02 00:00:00.000000 ccpn_project_checker-0.1.5/src/project_checker/test_data/warn_projects/empty_good_project_extra_root_xml_files.ccpn/ccpnv3/ccp/lims/RefSampleComponent/default+default_user_2024-02-24-15-54-35-583_00003.xml
--rw-r--r--   0        0        0      699 2020-02-02 00:00:00.000000 ccpn_project_checker-0.1.5/src/project_checker/test_data/warn_projects/empty_good_project_extra_root_xml_files.ccpn/ccpnv3/ccp/lims/Sample/default+default_user_2024-02-24-15-54-35-583_00002.xml
--rw-r--r--   0        0        0      462 2020-02-02 00:00:00.000000 ccpn_project_checker-0.1.5/src/project_checker/test_data/warn_projects/empty_good_project_extra_root_xml_files.ccpn/ccpnv3/ccp/molecule/MolSystem/default+default_user_2024-02-24-15-54-35-583_00004.xml
--rw-r--r--   0        0        0     3732 2020-02-02 00:00:00.000000 ccpn_project_checker-0.1.5/src/project_checker/test_data/warn_projects/empty_good_project_extra_root_xml_files.ccpn/ccpnv3/ccp/nmr/Nmr/default+default_user_2024-02-24-15-54-35-583_00001.xml
--rw-r--r--   0        0        0      868 2020-02-02 00:00:00.000000 ccpn_project_checker-0.1.5/src/project_checker/test_data/warn_projects/empty_good_project_extra_root_xml_files.ccpn/ccpnv3/ccpnmr/gui/Task/user+View+default_user_2024-02-24-15-54-35-583_00006.xml
--rw-r--r--   0        0        0     1014 2020-02-02 00:00:00.000000 ccpn_project_checker-0.1.5/src/project_checker/test_data/warn_projects/empty_good_project_extra_root_xml_files.ccpn/ccpnv3/ccpnmr/gui/Window/_ccp_nmr_Nmr_NmrProject___default___+default_user_2024-02-24-15-54-35-583_00005.xml
--rw-r--r--   0        0        0   179479 2020-02-02 00:00:00.000000 ccpn_project_checker-0.1.5/src/project_checker/test_data/warn_projects/empty_good_project_extra_root_xml_files.ccpn/ccpnv3/memops/Implementation/empty_good_project_extra_root_xml_files.xml
--rw-r--r--   0        0        0   179479 2020-02-02 00:00:00.000000 ccpn_project_checker-0.1.5/src/project_checker/test_data/warn_projects/empty_good_project_extra_root_xml_files.ccpn/ccpnv3/memops/Implementation/empty_good_project_extra_root_xml_files_2.xml
--rw-r--r--   0        0        0      499 2020-02-02 00:00:00.000000 ccpn_project_checker-0.1.5/src/project_checker/test_data/warn_projects/empty_good_project_extra_xml_files.ccpn/ccpnv3/ccp/lims/RefSampleComponent/default+default_user_2024-02-24-15-54-35-583_00003.xml
--rw-r--r--   0        0        0      699 2020-02-02 00:00:00.000000 ccpn_project_checker-0.1.5/src/project_checker/test_data/warn_projects/empty_good_project_extra_xml_files.ccpn/ccpnv3/ccp/lims/Sample/default+default_user_2024-02-24-15-54-35-583_00002.xml
--rw-r--r--   0        0        0      462 2020-02-02 00:00:00.000000 ccpn_project_checker-0.1.5/src/project_checker/test_data/warn_projects/empty_good_project_extra_xml_files.ccpn/ccpnv3/ccp/molecule/MolSystem/default+default_user_2024-02-24-15-54-35-583_00004.xml
--rw-r--r--   0        0        0      462 2020-02-02 00:00:00.000000 ccpn_project_checker-0.1.5/src/project_checker/test_data/warn_projects/empty_good_project_extra_xml_files.ccpn/ccpnv3/ccp/molecule/MolSystem/molecule2.xml
--rw-r--r--   0        0        0     3732 2020-02-02 00:00:00.000000 ccpn_project_checker-0.1.5/src/project_checker/test_data/warn_projects/empty_good_project_extra_xml_files.ccpn/ccpnv3/ccp/nmr/Nmr/default+default_user_2024-02-24-15-54-35-583_00001.xml
--rw-r--r--   0        0        0      868 2020-02-02 00:00:00.000000 ccpn_project_checker-0.1.5/src/project_checker/test_data/warn_projects/empty_good_project_extra_xml_files.ccpn/ccpnv3/ccpnmr/gui/Task/task_2.xml
--rw-r--r--   0        0        0      868 2020-02-02 00:00:00.000000 ccpn_project_checker-0.1.5/src/project_checker/test_data/warn_projects/empty_good_project_extra_xml_files.ccpn/ccpnv3/ccpnmr/gui/Task/user+View+default_user_2024-02-24-15-54-35-583_00006.xml
--rw-r--r--   0        0        0     1014 2020-02-02 00:00:00.000000 ccpn_project_checker-0.1.5/src/project_checker/test_data/warn_projects/empty_good_project_extra_xml_files.ccpn/ccpnv3/ccpnmr/gui/Window/_ccp_nmr_Nmr_NmrProject___default___+default_user_2024-02-24-15-54-35-583_00005.xml
--rw-r--r--   0        0        0   179479 2020-02-02 00:00:00.000000 ccpn_project_checker-0.1.5/src/project_checker/test_data/warn_projects/empty_good_project_extra_xml_files.ccpn/ccpnv3/memops/Implementation/empty_good_project_extra_xml_files.xml
--rw-r--r--   0        0        0      499 2020-02-02 00:00:00.000000 ccpn_project_checker-0.1.5/src/project_checker/test_data/warn_projects/empty_good_project_with_empty_containers.ccpn/ccpnv3/ccp/lims/RefSampleComponent/default+default_user_2024-02-24-15-54-35-583_00003.xml
--rw-r--r--   0        0        0      699 2020-02-02 00:00:00.000000 ccpn_project_checker-0.1.5/src/project_checker/test_data/warn_projects/empty_good_project_with_empty_containers.ccpn/ccpnv3/ccp/lims/Sample/default+default_user_2024-02-24-15-54-35-583_00002.xml
--rw-r--r--   0        0        0        0 2020-02-02 00:00:00.000000 ccpn_project_checker-0.1.5/src/project_checker/test_data/warn_projects/empty_good_project_with_empty_containers.ccpn/ccpnv3/ccp/molecule/LabeledMolecule/.keep_alive
--rw-r--r--   0        0        0      462 2020-02-02 00:00:00.000000 ccpn_project_checker-0.1.5/src/project_checker/test_data/warn_projects/empty_good_project_with_empty_containers.ccpn/ccpnv3/ccp/molecule/MolSystem/default+default_user_2024-02-24-15-54-35-583_00004.xml
--rw-r--r--   0        0        0        0 2020-02-02 00:00:00.000000 ccpn_project_checker-0.1.5/src/project_checker/test_data/warn_projects/empty_good_project_with_empty_containers.ccpn/ccpnv3/ccp/molsim/Symmetry/.keep_alive
--rw-r--r--   0        0        0     3732 2020-02-02 00:00:00.000000 ccpn_project_checker-0.1.5/src/project_checker/test_data/warn_projects/empty_good_project_with_empty_containers.ccpn/ccpnv3/ccp/nmr/Nmr/default+default_user_2024-02-24-15-54-35-583_00001.xml
--rw-r--r--   0        0        0      868 2020-02-02 00:00:00.000000 ccpn_project_checker-0.1.5/src/project_checker/test_data/warn_projects/empty_good_project_with_empty_containers.ccpn/ccpnv3/ccpnmr/gui/Task/user+View+default_user_2024-02-24-15-54-35-583_00006.xml
--rw-r--r--   0        0        0     1014 2020-02-02 00:00:00.000000 ccpn_project_checker-0.1.5/src/project_checker/test_data/warn_projects/empty_good_project_with_empty_containers.ccpn/ccpnv3/ccpnmr/gui/Window/_ccp_nmr_Nmr_NmrProject___default___+default_user_2024-02-24-15-54-35-583_00005.xml
--rw-r--r--   0        0        0   179479 2020-02-02 00:00:00.000000 ccpn_project_checker-0.1.5/src/project_checker/test_data/warn_projects/empty_good_project_with_empty_containers.ccpn/ccpnv3/memops/Implementation/empty_good_project_with_empty_containers.xml
--rw-r--r--   0        0        0      499 2020-02-02 00:00:00.000000 ccpn_project_checker-0.1.5/src/project_checker/test_data/warn_projects/root_file_badly_formatted_time.ccpn/ccpnv3/ccp/lims/RefSampleComponent/default+default_user_2024-02-24-15-54-35-583_00003.xml
--rw-r--r--   0        0        0      699 2020-02-02 00:00:00.000000 ccpn_project_checker-0.1.5/src/project_checker/test_data/warn_projects/root_file_badly_formatted_time.ccpn/ccpnv3/ccp/lims/Sample/default+default_user_2024-02-24-15-54-35-583_00002.xml
--rw-r--r--   0        0        0      462 2020-02-02 00:00:00.000000 ccpn_project_checker-0.1.5/src/project_checker/test_data/warn_projects/root_file_badly_formatted_time.ccpn/ccpnv3/ccp/molecule/MolSystem/default+default_user_2024-02-24-15-54-35-583_00004.xml
--rw-r--r--   0        0        0     3732 2020-02-02 00:00:00.000000 ccpn_project_checker-0.1.5/src/project_checker/test_data/warn_projects/root_file_badly_formatted_time.ccpn/ccpnv3/ccp/nmr/Nmr/default+default_user_2024-02-24-15-54-35-583_00001.xml
--rw-r--r--   0        0        0      868 2020-02-02 00:00:00.000000 ccpn_project_checker-0.1.5/src/project_checker/test_data/warn_projects/root_file_badly_formatted_time.ccpn/ccpnv3/ccpnmr/gui/Task/user+View+default_user_2024-02-24-15-54-35-583_00006.xml
--rw-r--r--   0        0        0     1014 2020-02-02 00:00:00.000000 ccpn_project_checker-0.1.5/src/project_checker/test_data/warn_projects/root_file_badly_formatted_time.ccpn/ccpnv3/ccpnmr/gui/Window/_ccp_nmr_Nmr_NmrProject___default___+default_user_2024-02-24-15-54-35-583_00005.xml
--rw-r--r--   0        0        0   179479 2020-02-02 00:00:00.000000 ccpn_project_checker-0.1.5/src/project_checker/test_data/warn_projects/root_file_badly_formatted_time.ccpn/ccpnv3/memops/Implementation/root_file_badly_formatted_time.xml
--rw-r--r--   0        0        0      499 2020-02-02 00:00:00.000000 ccpn_project_checker-0.1.5/src/project_checker/test_data/warn_projects/root_file_missing_time.ccpn/ccpnv3/ccp/lims/RefSampleComponent/default+default_user_2024-02-24-15-54-35-583_00003.xml
--rw-r--r--   0        0        0      699 2020-02-02 00:00:00.000000 ccpn_project_checker-0.1.5/src/project_checker/test_data/warn_projects/root_file_missing_time.ccpn/ccpnv3/ccp/lims/Sample/default+default_user_2024-02-24-15-54-35-583_00002.xml
--rw-r--r--   0        0        0      462 2020-02-02 00:00:00.000000 ccpn_project_checker-0.1.5/src/project_checker/test_data/warn_projects/root_file_missing_time.ccpn/ccpnv3/ccp/molecule/MolSystem/default+default_user_2024-02-24-15-54-35-583_00004.xml
--rw-r--r--   0        0        0     3732 2020-02-02 00:00:00.000000 ccpn_project_checker-0.1.5/src/project_checker/test_data/warn_projects/root_file_missing_time.ccpn/ccpnv3/ccp/nmr/Nmr/default+default_user_2024-02-24-15-54-35-583_00001.xml
--rw-r--r--   0        0        0      868 2020-02-02 00:00:00.000000 ccpn_project_checker-0.1.5/src/project_checker/test_data/warn_projects/root_file_missing_time.ccpn/ccpnv3/ccpnmr/gui/Task/user+View+default_user_2024-02-24-15-54-35-583_00006.xml
--rw-r--r--   0        0        0     1014 2020-02-02 00:00:00.000000 ccpn_project_checker-0.1.5/src/project_checker/test_data/warn_projects/root_file_missing_time.ccpn/ccpnv3/ccpnmr/gui/Window/_ccp_nmr_Nmr_NmrProject___default___+default_user_2024-02-24-15-54-35-583_00005.xml
--rw-r--r--   0        0        0   179482 2020-02-02 00:00:00.000000 ccpn_project_checker-0.1.5/src/project_checker/test_data/warn_projects/root_file_missing_time.ccpn/ccpnv3/memops/Implementation/root_file_missing_time.xml
--rw-r--r--   0        0        0        0 2020-02-02 00:00:00.000000 ccpn_project_checker-0.1.5/src/project_checker/tests/__init__.py
--rw-r--r--   0        0        0    77076 2020-02-02 00:00:00.000000 ccpn_project_checker-0.1.5/src/project_checker/tests/api_test_data.py
--rw-r--r--   0        0        0     2171 2020-02-02 00:00:00.000000 ccpn_project_checker-0.1.5/src/project_checker/tests/api_test_data_internal.py
--rw-r--r--   0        0        0      137 2020-02-02 00:00:00.000000 ccpn_project_checker-0.1.5/src/project_checker/tests/cli_test_data.py
--rw-r--r--   0        0        0     5087 2020-02-02 00:00:00.000000 ccpn_project_checker-0.1.5/src/project_checker/tests/test_api.py
--rw-r--r--   0        0        0     1074 2020-02-02 00:00:00.000000 ccpn_project_checker-0.1.5/src/project_checker/tests/test_cli.py
--rw-r--r--   0        0        0     9510 2020-02-02 00:00:00.000000 ccpn_project_checker-0.1.5/src/project_checker/tests/testing_utils.py
--rw-r--r--   0        0        0      320 2020-02-02 00:00:00.000000 ccpn_project_checker-0.1.5/src/project_checker/tests/write_cli_test_data.py
--rw-r--r--   0        0        0       92 2020-02-02 00:00:00.000000 ccpn_project_checker-0.1.5/.gitignore
--rw-r--r--   0        0        0       51 2020-02-02 00:00:00.000000 ccpn_project_checker-0.1.5/README.md
--rw-r--r--   0        0        0      655 2020-02-02 00:00:00.000000 ccpn_project_checker-0.1.5/pyproject.toml
--rw-r--r--   0        0        0      378 2020-02-02 00:00:00.000000 ccpn_project_checker-0.1.5/PKG-INFO
+-rw-r--r--   0        0        0        8 2020-02-02 00:00:00.000000 ccpn_project_checker-0.1.6/.python-version
+-rw-r--r--   0        0        0     1100 2020-02-02 00:00:00.000000 ccpn_project_checker-0.1.6/TODO.txt
+-rw-r--r--   0        0        0      604 2020-02-02 00:00:00.000000 ccpn_project_checker-0.1.6/requirements-dev.lock
+-rw-r--r--   0        0        0      604 2020-02-02 00:00:00.000000 ccpn_project_checker-0.1.6/requirements.lock
+-rw-r--r--   0        0        0      239 2020-02-02 00:00:00.000000 ccpn_project_checker-0.1.6/project_checker/.idea/.gitignore
+-rw-r--r--   0        0        0      294 2020-02-02 00:00:00.000000 ccpn_project_checker-0.1.6/project_checker/.idea/misc.xml
+-rw-r--r--   0        0        0      282 2020-02-02 00:00:00.000000 ccpn_project_checker-0.1.6/project_checker/.idea/modules.xml
+-rw-r--r--   0        0        0      419 2020-02-02 00:00:00.000000 ccpn_project_checker-0.1.6/project_checker/.idea/project_checker.iml
+-rw-r--r--   0        0        0      235 2020-02-02 00:00:00.000000 ccpn_project_checker-0.1.6/project_checker/.idea/vcs.xml
+-rw-r--r--   0        0        0    13240 2020-02-02 00:00:00.000000 ccpn_project_checker-0.1.6/project_checker/.idea/workspace.xml
+-rw-r--r--   0        0        0     5453 2020-02-02 00:00:00.000000 ccpn_project_checker-0.1.6/project_checker/.idea/copilot/chatSessions/00000000000.xd
+-rw-r--r--   0        0        0    13526 2020-02-02 00:00:00.000000 ccpn_project_checker-0.1.6/project_checker/.idea/copilot/chatSessions/xd.lck
+-rw-r--r--   0        0        0        4 2020-02-02 00:00:00.000000 ccpn_project_checker-0.1.6/project_checker/.idea/copilot/chatSessions/blobs/version
+-rw-r--r--   0        0        0      174 2020-02-02 00:00:00.000000 ccpn_project_checker-0.1.6/project_checker/.idea/inspectionProfiles/profiles_settings.xml
+-rwxr-xr-x   0        0        0      197 2020-02-02 00:00:00.000000 ccpn_project_checker-0.1.6/scripts/project_checker
+-rwxr-xr-x   0        0        0      276 2020-02-02 00:00:00.000000 ccpn_project_checker-0.1.6/scripts/test
+-rw-r--r--   0        0        0    83487 2020-02-02 00:00:00.000000 ccpn_project_checker-0.1.6/src/project_checker/DiskModelChecker.py
+-rw-r--r--   0        0        0     8665 2020-02-02 00:00:00.000000 ccpn_project_checker-0.1.6/src/project_checker/MetaModelWalker.py
+-rw-r--r--   0        0        0        0 2020-02-02 00:00:00.000000 ccpn_project_checker-0.1.6/src/project_checker/__init__.py
+-rw-r--r--   0        0        0      123 2020-02-02 00:00:00.000000 ccpn_project_checker-0.1.6/src/project_checker/main.py
+-rw-r--r--   0        0        0    47287 2020-02-02 00:00:00.000000 ccpn_project_checker-0.1.6/src/project_checker/model_info/data_file_names.txt
+-rw-r--r--   0        0        0    81462 2020-02-02 00:00:00.000000 ccpn_project_checker-0.1.6/src/project_checker/model_info/v_3_1_0_guid_to_storage_location.json
+-rw-r--r--   0        0        0   527533 2020-02-02 00:00:00.000000 ccpn_project_checker-0.1.6/src/project_checker/model_info/v_3_1_0_object_info.json
+-rw-r--r--   0        0        0     2256 2020-02-02 00:00:00.000000 ccpn_project_checker-0.1.6/src/project_checker/model_info/v_3_1_0_short_name_to_guid.json
+-rw-r--r--   0        0        0       43 2020-02-02 00:00:00.000000 ccpn_project_checker-0.1.6/src/project_checker/optional/__init__.py
+-rw-r--r--   0        0        0      814 2020-02-02 00:00:00.000000 ccpn_project_checker-0.1.6/src/project_checker/optional/abstract_optional.py
+-rw-r--r--   0        0        0      305 2020-02-02 00:00:00.000000 ccpn_project_checker-0.1.6/src/project_checker/optional/compatible_abc.py
+-rw-r--r--   0        0        0      133 2020-02-02 00:00:00.000000 ccpn_project_checker-0.1.6/src/project_checker/optional/exceptions.py
+-rw-r--r--   0        0        0     1142 2020-02-02 00:00:00.000000 ccpn_project_checker-0.1.6/src/project_checker/optional/nothing.py
+-rw-r--r--   0        0        0     1056 2020-02-02 00:00:00.000000 ccpn_project_checker-0.1.6/src/project_checker/optional/optional.py
+-rw-r--r--   0        0        0     1411 2020-02-02 00:00:00.000000 ccpn_project_checker-0.1.6/src/project_checker/optional/something.py
+-rw-r--r--   0        0        0   233080 2020-02-02 00:00:00.000000 ccpn_project_checker-0.1.6/src/project_checker/test_data/cli_test_output.txt
+-rw-r--r--   0        0        0        0 2020-02-02 00:00:00.000000 ccpn_project_checker-0.1.6/src/project_checker/test_data/project_is_file.ccpn
+-rw-r--r--   0        0        0   179478 2020-02-02 00:00:00.000000 ccpn_project_checker-0.1.6/src/project_checker/test_data/bad_memops_root_xml.ccpn/ccpnv3/memops/Implementation/bad_memops_root_xml.xml
+-rw-r--r--   0        0        0      868 2020-02-02 00:00:00.000000 ccpn_project_checker-0.1.6/src/project_checker/test_data/basic_exo_links_not_found.ccpn/ccpnv3/memops/Implementation/basic_exo_links_not_found.xml
+-rw-r--r--   0        0        0      499 2020-02-02 00:00:00.000000 ccpn_project_checker-0.1.6/src/project_checker/test_data/delayed_errors/bad_embedded_exo_link_0_child_elements.ccpn/ccpnv3/ccp/lims/RefSampleComponent/default+default_user_2024-02-24-15-54-35-583_00003.xml
+-rw-r--r--   0        0        0      699 2020-02-02 00:00:00.000000 ccpn_project_checker-0.1.6/src/project_checker/test_data/delayed_errors/bad_embedded_exo_link_0_child_elements.ccpn/ccpnv3/ccp/lims/Sample/default+default_user_2024-02-24-15-54-35-583_00002.xml
+-rw-r--r--   0        0        0      462 2020-02-02 00:00:00.000000 ccpn_project_checker-0.1.6/src/project_checker/test_data/delayed_errors/bad_embedded_exo_link_0_child_elements.ccpn/ccpnv3/ccp/molecule/MolSystem/default+default_user_2024-02-24-15-54-35-583_00004.xml
+-rw-r--r--   0        0        0     3732 2020-02-02 00:00:00.000000 ccpn_project_checker-0.1.6/src/project_checker/test_data/delayed_errors/bad_embedded_exo_link_0_child_elements.ccpn/ccpnv3/ccp/nmr/Nmr/default+default_user_2024-02-24-15-54-35-583_00001.xml
+-rw-r--r--   0        0        0      868 2020-02-02 00:00:00.000000 ccpn_project_checker-0.1.6/src/project_checker/test_data/delayed_errors/bad_embedded_exo_link_0_child_elements.ccpn/ccpnv3/ccpnmr/gui/Task/user+View+default_user_2024-02-24-15-54-35-583_00006.xml
+-rw-r--r--   0        0        0     1014 2020-02-02 00:00:00.000000 ccpn_project_checker-0.1.6/src/project_checker/test_data/delayed_errors/bad_embedded_exo_link_0_child_elements.ccpn/ccpnv3/ccpnmr/gui/Window/_ccp_nmr_Nmr_NmrProject___default___+default_user_2024-02-24-15-54-35-583_00005.xml
+-rw-r--r--   0        0        0   179440 2020-02-02 00:00:00.000000 ccpn_project_checker-0.1.6/src/project_checker/test_data/delayed_errors/bad_embedded_exo_link_0_child_elements.ccpn/ccpnv3/memops/Implementation/bad_embedded_exo_link_0_child_elements.xml
+-rw-r--r--   0        0        0      499 2020-02-02 00:00:00.000000 ccpn_project_checker-0.1.6/src/project_checker/test_data/delayed_errors/bad_embedded_exo_link_0_elements.ccpn/ccpnv3/ccp/lims/RefSampleComponent/default+default_user_2024-02-24-15-54-35-583_00003.xml
+-rw-r--r--   0        0        0      699 2020-02-02 00:00:00.000000 ccpn_project_checker-0.1.6/src/project_checker/test_data/delayed_errors/bad_embedded_exo_link_0_elements.ccpn/ccpnv3/ccp/lims/Sample/default+default_user_2024-02-24-15-54-35-583_00002.xml
+-rw-r--r--   0        0        0      462 2020-02-02 00:00:00.000000 ccpn_project_checker-0.1.6/src/project_checker/test_data/delayed_errors/bad_embedded_exo_link_0_elements.ccpn/ccpnv3/ccp/molecule/MolSystem/default+default_user_2024-02-24-15-54-35-583_00004.xml
+-rw-r--r--   0        0        0     3732 2020-02-02 00:00:00.000000 ccpn_project_checker-0.1.6/src/project_checker/test_data/delayed_errors/bad_embedded_exo_link_0_elements.ccpn/ccpnv3/ccp/nmr/Nmr/default+default_user_2024-02-24-15-54-35-583_00001.xml
+-rw-r--r--   0        0        0      868 2020-02-02 00:00:00.000000 ccpn_project_checker-0.1.6/src/project_checker/test_data/delayed_errors/bad_embedded_exo_link_0_elements.ccpn/ccpnv3/ccpnmr/gui/Task/user+View+default_user_2024-02-24-15-54-35-583_00006.xml
+-rw-r--r--   0        0        0     1014 2020-02-02 00:00:00.000000 ccpn_project_checker-0.1.6/src/project_checker/test_data/delayed_errors/bad_embedded_exo_link_0_elements.ccpn/ccpnv3/ccpnmr/gui/Window/_ccp_nmr_Nmr_NmrProject___default___+default_user_2024-02-24-15-54-35-583_00005.xml
+-rw-r--r--   0        0        0   179355 2020-02-02 00:00:00.000000 ccpn_project_checker-0.1.6/src/project_checker/test_data/delayed_errors/bad_embedded_exo_link_0_elements.ccpn/ccpnv3/memops/Implementation/bad_embedded_exo_link_0_elements.xml
+-rw-r--r--   0        0        0      499 2020-02-02 00:00:00.000000 ccpn_project_checker-0.1.6/src/project_checker/test_data/delayed_errors/bad_role_exo_link_key_element_children.ccpn/ccpnv3/ccp/lims/RefSampleComponent/default+default_user_2024-02-24-15-54-35-583_00003.xml
+-rw-r--r--   0        0        0      699 2020-02-02 00:00:00.000000 ccpn_project_checker-0.1.6/src/project_checker/test_data/delayed_errors/bad_role_exo_link_key_element_children.ccpn/ccpnv3/ccp/lims/Sample/default+default_user_2024-02-24-15-54-35-583_00002.xml
+-rw-r--r--   0        0        0      462 2020-02-02 00:00:00.000000 ccpn_project_checker-0.1.6/src/project_checker/test_data/delayed_errors/bad_role_exo_link_key_element_children.ccpn/ccpnv3/ccp/molecule/MolSystem/default+default_user_2024-02-24-15-54-35-583_00004.xml
+-rw-r--r--   0        0        0     3732 2020-02-02 00:00:00.000000 ccpn_project_checker-0.1.6/src/project_checker/test_data/delayed_errors/bad_role_exo_link_key_element_children.ccpn/ccpnv3/ccp/nmr/Nmr/default+default_user_2024-02-24-15-54-35-583_00001.xml
+-rw-r--r--   0        0        0      868 2020-02-02 00:00:00.000000 ccpn_project_checker-0.1.6/src/project_checker/test_data/delayed_errors/bad_role_exo_link_key_element_children.ccpn/ccpnv3/ccpnmr/gui/Task/user+View+default_user_2024-02-24-15-54-35-583_00006.xml
+-rw-r--r--   0        0        0     1014 2020-02-02 00:00:00.000000 ccpn_project_checker-0.1.6/src/project_checker/test_data/delayed_errors/bad_role_exo_link_key_element_children.ccpn/ccpnv3/ccpnmr/gui/Window/_ccp_nmr_Nmr_NmrProject___default___+default_user_2024-02-24-15-54-35-583_00005.xml
+-rw-r--r--   0        0        0   179391 2020-02-02 00:00:00.000000 ccpn_project_checker-0.1.6/src/project_checker/test_data/delayed_errors/bad_role_exo_link_key_element_children.ccpn/ccpnv3/memops/Implementation/bad_role_exo_link_key_element_children.xml
+-rw-r--r--   0        0        0      499 2020-02-02 00:00:00.000000 ccpn_project_checker-0.1.6/src/project_checker/test_data/delayed_errors/bad_role_exo_link_key_element_parent.ccpn/ccpnv3/ccp/lims/RefSampleComponent/default+default_user_2024-02-24-15-54-35-583_00003.xml
+-rw-r--r--   0        0        0      699 2020-02-02 00:00:00.000000 ccpn_project_checker-0.1.6/src/project_checker/test_data/delayed_errors/bad_role_exo_link_key_element_parent.ccpn/ccpnv3/ccp/lims/Sample/default+default_user_2024-02-24-15-54-35-583_00002.xml
+-rw-r--r--   0        0        0      462 2020-02-02 00:00:00.000000 ccpn_project_checker-0.1.6/src/project_checker/test_data/delayed_errors/bad_role_exo_link_key_element_parent.ccpn/ccpnv3/ccp/molecule/MolSystem/default+default_user_2024-02-24-15-54-35-583_00004.xml
+-rw-r--r--   0        0        0     3732 2020-02-02 00:00:00.000000 ccpn_project_checker-0.1.6/src/project_checker/test_data/delayed_errors/bad_role_exo_link_key_element_parent.ccpn/ccpnv3/ccp/nmr/Nmr/default+default_user_2024-02-24-15-54-35-583_00001.xml
+-rw-r--r--   0        0        0      868 2020-02-02 00:00:00.000000 ccpn_project_checker-0.1.6/src/project_checker/test_data/delayed_errors/bad_role_exo_link_key_element_parent.ccpn/ccpnv3/ccpnmr/gui/Task/user+View+default_user_2024-02-24-15-54-35-583_00006.xml
+-rw-r--r--   0        0        0     1014 2020-02-02 00:00:00.000000 ccpn_project_checker-0.1.6/src/project_checker/test_data/delayed_errors/bad_role_exo_link_key_element_parent.ccpn/ccpnv3/ccpnmr/gui/Window/_ccp_nmr_Nmr_NmrProject___default___+default_user_2024-02-24-15-54-35-583_00005.xml
+-rw-r--r--   0        0        0   179486 2020-02-02 00:00:00.000000 ccpn_project_checker-0.1.6/src/project_checker/test_data/delayed_errors/bad_role_exo_link_key_element_parent.ccpn/ccpnv3/memops/Implementation/bad_role_exo_link_key_element_parent.xml
+-rw-r--r--   0        0        0      499 2020-02-02 00:00:00.000000 ccpn_project_checker-0.1.6/src/project_checker/test_data/delayed_errors/bad_root_exo_link_element.ccpn/ccpnv3/ccp/lims/RefSampleComponent/default+default_user_2024-02-24-15-54-35-583_00003.xml
+-rw-r--r--   0        0        0      699 2020-02-02 00:00:00.000000 ccpn_project_checker-0.1.6/src/project_checker/test_data/delayed_errors/bad_root_exo_link_element.ccpn/ccpnv3/ccp/lims/Sample/default+default_user_2024-02-24-15-54-35-583_00002.xml
+-rw-r--r--   0        0        0      462 2020-02-02 00:00:00.000000 ccpn_project_checker-0.1.6/src/project_checker/test_data/delayed_errors/bad_root_exo_link_element.ccpn/ccpnv3/ccp/molecule/MolSystem/default+default_user_2024-02-24-15-54-35-583_00004.xml
+-rw-r--r--   0        0        0     3732 2020-02-02 00:00:00.000000 ccpn_project_checker-0.1.6/src/project_checker/test_data/delayed_errors/bad_root_exo_link_element.ccpn/ccpnv3/ccp/nmr/Nmr/default+default_user_2024-02-24-15-54-35-583_00001.xml
+-rw-r--r--   0        0        0      868 2020-02-02 00:00:00.000000 ccpn_project_checker-0.1.6/src/project_checker/test_data/delayed_errors/bad_root_exo_link_element.ccpn/ccpnv3/ccpnmr/gui/Task/user+View+default_user_2024-02-24-15-54-35-583_00006.xml
+-rw-r--r--   0        0        0     1014 2020-02-02 00:00:00.000000 ccpn_project_checker-0.1.6/src/project_checker/test_data/delayed_errors/bad_root_exo_link_element.ccpn/ccpnv3/ccpnmr/gui/Window/_ccp_nmr_Nmr_NmrProject___default___+default_user_2024-02-24-15-54-35-583_00005.xml
+-rw-r--r--   0        0        0   179514 2020-02-02 00:00:00.000000 ccpn_project_checker-0.1.6/src/project_checker/test_data/delayed_errors/bad_root_exo_link_element.ccpn/ccpnv3/memops/Implementation/bad_root_exo_link_element.xml
+-rw-r--r--   0        0        0      499 2020-02-02 00:00:00.000000 ccpn_project_checker-0.1.6/src/project_checker/test_data/delayed_errors/empty_good_project_with_non_ccpn_letter~.ccpn/ccpnv3/ccp/lims/RefSampleComponent/default+default_user_2024-02-24-15-54-35-583_00003.xml
+-rw-r--r--   0        0        0      699 2020-02-02 00:00:00.000000 ccpn_project_checker-0.1.6/src/project_checker/test_data/delayed_errors/empty_good_project_with_non_ccpn_letter~.ccpn/ccpnv3/ccp/lims/Sample/default+default_user_2024-02-24-15-54-35-583_00002.xml
+-rw-r--r--   0        0        0      462 2020-02-02 00:00:00.000000 ccpn_project_checker-0.1.6/src/project_checker/test_data/delayed_errors/empty_good_project_with_non_ccpn_letter~.ccpn/ccpnv3/ccp/molecule/MolSystem/default+default_user_2024-02-24-15-54-35-583_00004.xml
+-rw-r--r--   0        0        0     3732 2020-02-02 00:00:00.000000 ccpn_project_checker-0.1.6/src/project_checker/test_data/delayed_errors/empty_good_project_with_non_ccpn_letter~.ccpn/ccpnv3/ccp/nmr/Nmr/default+default_user_2024-02-24-15-54-35-583_00001.xml
+-rw-r--r--   0        0        0      868 2020-02-02 00:00:00.000000 ccpn_project_checker-0.1.6/src/project_checker/test_data/delayed_errors/empty_good_project_with_non_ccpn_letter~.ccpn/ccpnv3/ccpnmr/gui/Task/user+View+default_user_2024-02-24-15-54-35-583_00006.xml
+-rw-r--r--   0        0        0     1014 2020-02-02 00:00:00.000000 ccpn_project_checker-0.1.6/src/project_checker/test_data/delayed_errors/empty_good_project_with_non_ccpn_letter~.ccpn/ccpnv3/ccpnmr/gui/Window/_ccp_nmr_Nmr_NmrProject___default___+default_user_2024-02-24-15-54-35-583_00005.xml
+-rw-r--r--   0        0        0   179479 2020-02-02 00:00:00.000000 ccpn_project_checker-0.1.6/src/project_checker/test_data/delayed_errors/empty_good_project_with_non_ccpn_letter~.ccpn/ccpnv3/memops/Implementation/empty_good_project_with_non_ccpn_letter~.xml
+-rw-r--r--   0        0        0      499 2020-02-02 00:00:00.000000 ccpn_project_checker-0.1.6/src/project_checker/test_data/delayed_errors/exo_file_bad_root_element_name.ccpn/ccpnv3/ccp/lims/RefSampleComponent/default+default_user_2024-02-24-15-54-35-583_00003.xml
+-rw-r--r--   0        0        0      699 2020-02-02 00:00:00.000000 ccpn_project_checker-0.1.6/src/project_checker/test_data/delayed_errors/exo_file_bad_root_element_name.ccpn/ccpnv3/ccp/lims/Sample/default+default_user_2024-02-24-15-54-35-583_00002.xml
+-rw-r--r--   0        0        0      462 2020-02-02 00:00:00.000000 ccpn_project_checker-0.1.6/src/project_checker/test_data/delayed_errors/exo_file_bad_root_element_name.ccpn/ccpnv3/ccp/molecule/MolSystem/default+default_user_2024-02-24-15-54-35-583_00004.xml
+-rw-r--r--   0        0        0     3732 2020-02-02 00:00:00.000000 ccpn_project_checker-0.1.6/src/project_checker/test_data/delayed_errors/exo_file_bad_root_element_name.ccpn/ccpnv3/ccp/nmr/Nmr/default+default_user_2024-02-24-15-54-35-583_00001.xml
+-rw-r--r--   0        0        0      868 2020-02-02 00:00:00.000000 ccpn_project_checker-0.1.6/src/project_checker/test_data/delayed_errors/exo_file_bad_root_element_name.ccpn/ccpnv3/ccpnmr/gui/Task/user+View+default_user_2024-02-24-15-54-35-583_00006.xml
+-rw-r--r--   0        0        0     1014 2020-02-02 00:00:00.000000 ccpn_project_checker-0.1.6/src/project_checker/test_data/delayed_errors/exo_file_bad_root_element_name.ccpn/ccpnv3/ccpnmr/gui/Window/_ccp_nmr_Nmr_NmrProject___default___+default_user_2024-02-24-15-54-35-583_00005.xml
+-rw-r--r--   0        0        0   179479 2020-02-02 00:00:00.000000 ccpn_project_checker-0.1.6/src/project_checker/test_data/delayed_errors/exo_file_bad_root_element_name.ccpn/ccpnv3/memops/Implementation/exo_file_bad_root_element_name.xml
+-rw-r--r--   0        0        0      499 2020-02-02 00:00:00.000000 ccpn_project_checker-0.1.6/src/project_checker/test_data/delayed_errors/exo_file_key_doesnt_match_root.ccpn/ccpnv3/ccp/lims/RefSampleComponent/default+default_user_2024-02-24-15-54-35-583_00003.xml
+-rw-r--r--   0        0        0      699 2020-02-02 00:00:00.000000 ccpn_project_checker-0.1.6/src/project_checker/test_data/delayed_errors/exo_file_key_doesnt_match_root.ccpn/ccpnv3/ccp/lims/Sample/default+default_user_2024-02-24-15-54-35-583_00002.xml
+-rw-r--r--   0        0        0      462 2020-02-02 00:00:00.000000 ccpn_project_checker-0.1.6/src/project_checker/test_data/delayed_errors/exo_file_key_doesnt_match_root.ccpn/ccpnv3/ccp/molecule/MolSystem/wibble+default_user_2024-02-24-15-54-35-583_00004.xml
+-rw-r--r--   0        0        0     3732 2020-02-02 00:00:00.000000 ccpn_project_checker-0.1.6/src/project_checker/test_data/delayed_errors/exo_file_key_doesnt_match_root.ccpn/ccpnv3/ccp/nmr/Nmr/default+default_user_2024-02-24-15-54-35-583_00001.xml
+-rw-r--r--   0        0        0      868 2020-02-02 00:00:00.000000 ccpn_project_checker-0.1.6/src/project_checker/test_data/delayed_errors/exo_file_key_doesnt_match_root.ccpn/ccpnv3/ccpnmr/gui/Task/user+View+default_user_2024-02-24-15-54-35-583_00006.xml
+-rw-r--r--   0        0        0     1014 2020-02-02 00:00:00.000000 ccpn_project_checker-0.1.6/src/project_checker/test_data/delayed_errors/exo_file_key_doesnt_match_root.ccpn/ccpnv3/ccpnmr/gui/Window/_ccp_nmr_Nmr_NmrProject___default___+default_user_2024-02-24-15-54-35-583_00005.xml
+-rw-r--r--   0        0        0   179479 2020-02-02 00:00:00.000000 ccpn_project_checker-0.1.6/src/project_checker/test_data/delayed_errors/exo_file_key_doesnt_match_root.ccpn/ccpnv3/memops/Implementation/exo_file_key_doesnt_match_root.xml
+-rw-r--r--   0        0        0      499 2020-02-02 00:00:00.000000 ccpn_project_checker-0.1.6/src/project_checker/test_data/delayed_errors/exo_file_no_package_guid.ccpn/ccpnv3/ccp/lims/RefSampleComponent/default+default_user_2024-02-24-15-54-35-583_00003.xml
+-rw-r--r--   0        0        0      699 2020-02-02 00:00:00.000000 ccpn_project_checker-0.1.6/src/project_checker/test_data/delayed_errors/exo_file_no_package_guid.ccpn/ccpnv3/ccp/lims/Sample/default+default_user_2024-02-24-15-54-35-583_00002.xml
+-rw-r--r--   0        0        0      402 2020-02-02 00:00:00.000000 ccpn_project_checker-0.1.6/src/project_checker/test_data/delayed_errors/exo_file_no_package_guid.ccpn/ccpnv3/ccp/molecule/MolSystem/default+default_user_2024-02-24-15-54-35-583_00004.xml
+-rw-r--r--   0        0        0     3732 2020-02-02 00:00:00.000000 ccpn_project_checker-0.1.6/src/project_checker/test_data/delayed_errors/exo_file_no_package_guid.ccpn/ccpnv3/ccp/nmr/Nmr/default+default_user_2024-02-24-15-54-35-583_00001.xml
+-rw-r--r--   0        0        0      868 2020-02-02 00:00:00.000000 ccpn_project_checker-0.1.6/src/project_checker/test_data/delayed_errors/exo_file_no_package_guid.ccpn/ccpnv3/ccpnmr/gui/Task/user+View+default_user_2024-02-24-15-54-35-583_00006.xml
+-rw-r--r--   0        0        0     1014 2020-02-02 00:00:00.000000 ccpn_project_checker-0.1.6/src/project_checker/test_data/delayed_errors/exo_file_no_package_guid.ccpn/ccpnv3/ccpnmr/gui/Window/_ccp_nmr_Nmr_NmrProject___default___+default_user_2024-02-24-15-54-35-583_00005.xml
+-rw-r--r--   0        0        0   179479 2020-02-02 00:00:00.000000 ccpn_project_checker-0.1.6/src/project_checker/test_data/delayed_errors/exo_file_no_package_guid.ccpn/ccpnv3/memops/Implementation/exo_file_no_package_guid.xml
+-rw-r--r--   0        0        0      499 2020-02-02 00:00:00.000000 ccpn_project_checker-0.1.6/src/project_checker/test_data/delayed_errors/exo_file_release_attrib_invalid.ccpn/ccpnv3/ccp/lims/RefSampleComponent/default+default_user_2024-02-24-15-54-35-583_00003.xml
+-rw-r--r--   0        0        0      699 2020-02-02 00:00:00.000000 ccpn_project_checker-0.1.6/src/project_checker/test_data/delayed_errors/exo_file_release_attrib_invalid.ccpn/ccpnv3/ccp/lims/Sample/default+default_user_2024-02-24-15-54-35-583_00002.xml
+-rw-r--r--   0        0        0      463 2020-02-02 00:00:00.000000 ccpn_project_checker-0.1.6/src/project_checker/test_data/delayed_errors/exo_file_release_attrib_invalid.ccpn/ccpnv3/ccp/molecule/MolSystem/default+default_user_2024-02-24-15-54-35-583_00004.xml
+-rw-r--r--   0        0        0     3732 2020-02-02 00:00:00.000000 ccpn_project_checker-0.1.6/src/project_checker/test_data/delayed_errors/exo_file_release_attrib_invalid.ccpn/ccpnv3/ccp/nmr/Nmr/default+default_user_2024-02-24-15-54-35-583_00001.xml
+-rw-r--r--   0        0        0      868 2020-02-02 00:00:00.000000 ccpn_project_checker-0.1.6/src/project_checker/test_data/delayed_errors/exo_file_release_attrib_invalid.ccpn/ccpnv3/ccpnmr/gui/Task/user+View+default_user_2024-02-24-15-54-35-583_00006.xml
+-rw-r--r--   0        0        0     1014 2020-02-02 00:00:00.000000 ccpn_project_checker-0.1.6/src/project_checker/test_data/delayed_errors/exo_file_release_attrib_invalid.ccpn/ccpnv3/ccpnmr/gui/Window/_ccp_nmr_Nmr_NmrProject___default___+default_user_2024-02-24-15-54-35-583_00005.xml
+-rw-r--r--   0        0        0   179479 2020-02-02 00:00:00.000000 ccpn_project_checker-0.1.6/src/project_checker/test_data/delayed_errors/exo_file_release_attrib_invalid.ccpn/ccpnv3/memops/Implementation/exo_file_release_attrib_invalid.xml
+-rw-r--r--   0        0        0      499 2020-02-02 00:00:00.000000 ccpn_project_checker-0.1.6/src/project_checker/test_data/delayed_errors/exo_file_release_attrib_missing.ccpn/ccpnv3/ccp/lims/RefSampleComponent/default+default_user_2024-02-24-15-54-35-583_00003.xml
+-rw-r--r--   0        0        0      699 2020-02-02 00:00:00.000000 ccpn_project_checker-0.1.6/src/project_checker/test_data/delayed_errors/exo_file_release_attrib_missing.ccpn/ccpnv3/ccp/lims/Sample/default+default_user_2024-02-24-15-54-35-583_00002.xml
+-rw-r--r--   0        0        0      465 2020-02-02 00:00:00.000000 ccpn_project_checker-0.1.6/src/project_checker/test_data/delayed_errors/exo_file_release_attrib_missing.ccpn/ccpnv3/ccp/molecule/MolSystem/default+default_user_2024-02-24-15-54-35-583_00004.xml
+-rw-r--r--   0        0        0     3732 2020-02-02 00:00:00.000000 ccpn_project_checker-0.1.6/src/project_checker/test_data/delayed_errors/exo_file_release_attrib_missing.ccpn/ccpnv3/ccp/nmr/Nmr/default+default_user_2024-02-24-15-54-35-583_00001.xml
+-rw-r--r--   0        0        0      868 2020-02-02 00:00:00.000000 ccpn_project_checker-0.1.6/src/project_checker/test_data/delayed_errors/exo_file_release_attrib_missing.ccpn/ccpnv3/ccpnmr/gui/Task/user+View+default_user_2024-02-24-15-54-35-583_00006.xml
+-rw-r--r--   0        0        0     1014 2020-02-02 00:00:00.000000 ccpn_project_checker-0.1.6/src/project_checker/test_data/delayed_errors/exo_file_release_attrib_missing.ccpn/ccpnv3/ccpnmr/gui/Window/_ccp_nmr_Nmr_NmrProject___default___+default_user_2024-02-24-15-54-35-583_00005.xml
+-rw-r--r--   0        0        0   179479 2020-02-02 00:00:00.000000 ccpn_project_checker-0.1.6/src/project_checker/test_data/delayed_errors/exo_file_release_attrib_missing.ccpn/ccpnv3/memops/Implementation/exo_file_release_attrib_missing.xml
+-rw-r--r--   0        0        0      499 2020-02-02 00:00:00.000000 ccpn_project_checker-0.1.6/src/project_checker/test_data/delayed_errors/exo_file_release_doesnt_match_root.ccpn/ccpnv3/ccp/lims/RefSampleComponent/default+default_user_2024-02-24-15-54-35-583_00003.xml
+-rw-r--r--   0        0        0      699 2020-02-02 00:00:00.000000 ccpn_project_checker-0.1.6/src/project_checker/test_data/delayed_errors/exo_file_release_doesnt_match_root.ccpn/ccpnv3/ccp/lims/Sample/default+default_user_2024-02-24-15-54-35-583_00002.xml
+-rw-r--r--   0        0        0      462 2020-02-02 00:00:00.000000 ccpn_project_checker-0.1.6/src/project_checker/test_data/delayed_errors/exo_file_release_doesnt_match_root.ccpn/ccpnv3/ccp/molecule/MolSystem/default+default_user_2024-02-24-15-54-35-583_00004.xml
+-rw-r--r--   0        0        0     3732 2020-02-02 00:00:00.000000 ccpn_project_checker-0.1.6/src/project_checker/test_data/delayed_errors/exo_file_release_doesnt_match_root.ccpn/ccpnv3/ccp/nmr/Nmr/default+default_user_2024-02-24-15-54-35-583_00001.xml
+-rw-r--r--   0        0        0      868 2020-02-02 00:00:00.000000 ccpn_project_checker-0.1.6/src/project_checker/test_data/delayed_errors/exo_file_release_doesnt_match_root.ccpn/ccpnv3/ccpnmr/gui/Task/user+View+default_user_2024-02-24-15-54-35-583_00006.xml
+-rw-r--r--   0        0        0     1014 2020-02-02 00:00:00.000000 ccpn_project_checker-0.1.6/src/project_checker/test_data/delayed_errors/exo_file_release_doesnt_match_root.ccpn/ccpnv3/ccpnmr/gui/Window/_ccp_nmr_Nmr_NmrProject___default___+default_user_2024-02-24-15-54-35-583_00005.xml
+-rw-r--r--   0        0        0   179479 2020-02-02 00:00:00.000000 ccpn_project_checker-0.1.6/src/project_checker/test_data/delayed_errors/exo_file_release_doesnt_match_root.ccpn/ccpnv3/memops/Implementation/exo_file_release_doesnt_match_root.xml
+-rw-r--r--   0        0        0      499 2020-02-02 00:00:00.000000 ccpn_project_checker-0.1.6/src/project_checker/test_data/delayed_errors/exo_file_short_name_guid_doesnt_match_package_guid.ccpn/ccpnv3/ccp/lims/RefSampleComponent/default+default_user_2024-02-24-15-54-35-583_00003.xml
+-rw-r--r--   0        0        0      699 2020-02-02 00:00:00.000000 ccpn_project_checker-0.1.6/src/project_checker/test_data/delayed_errors/exo_file_short_name_guid_doesnt_match_package_guid.ccpn/ccpnv3/ccp/lims/Sample/default+default_user_2024-02-24-15-54-35-583_00002.xml
+-rw-r--r--   0        0        0      462 2020-02-02 00:00:00.000000 ccpn_project_checker-0.1.6/src/project_checker/test_data/delayed_errors/exo_file_short_name_guid_doesnt_match_package_guid.ccpn/ccpnv3/ccp/molecule/MolSystem/default+default_user_2024-02-24-15-54-35-583_00004.xml
+-rw-r--r--   0        0        0     3732 2020-02-02 00:00:00.000000 ccpn_project_checker-0.1.6/src/project_checker/test_data/delayed_errors/exo_file_short_name_guid_doesnt_match_package_guid.ccpn/ccpnv3/ccp/nmr/Nmr/default+default_user_2024-02-24-15-54-35-583_00001.xml
+-rw-r--r--   0        0        0      868 2020-02-02 00:00:00.000000 ccpn_project_checker-0.1.6/src/project_checker/test_data/delayed_errors/exo_file_short_name_guid_doesnt_match_package_guid.ccpn/ccpnv3/ccpnmr/gui/Task/user+View+default_user_2024-02-24-15-54-35-583_00006.xml
+-rw-r--r--   0        0        0     1014 2020-02-02 00:00:00.000000 ccpn_project_checker-0.1.6/src/project_checker/test_data/delayed_errors/exo_file_short_name_guid_doesnt_match_package_guid.ccpn/ccpnv3/ccpnmr/gui/Window/_ccp_nmr_Nmr_NmrProject___default___+default_user_2024-02-24-15-54-35-583_00005.xml
+-rw-r--r--   0        0        0   179479 2020-02-02 00:00:00.000000 ccpn_project_checker-0.1.6/src/project_checker/test_data/delayed_errors/exo_file_short_name_guid_doesnt_match_package_guid.ccpn/ccpnv3/memops/Implementation/exo_file_short_name_guid_doesnt_match_package_guid.xml
+-rw-r--r--   0        0        0      499 2020-02-02 00:00:00.000000 ccpn_project_checker-0.1.6/src/project_checker/test_data/delayed_errors/exo_file_time_attrib_invalid.ccpn/ccpnv3/ccp/lims/RefSampleComponent/default+default_user_2024-02-24-15-54-35-583_00003.xml
+-rw-r--r--   0        0        0      699 2020-02-02 00:00:00.000000 ccpn_project_checker-0.1.6/src/project_checker/test_data/delayed_errors/exo_file_time_attrib_invalid.ccpn/ccpnv3/ccp/lims/Sample/default+default_user_2024-02-24-15-54-35-583_00002.xml
+-rw-r--r--   0        0        0      444 2020-02-02 00:00:00.000000 ccpn_project_checker-0.1.6/src/project_checker/test_data/delayed_errors/exo_file_time_attrib_invalid.ccpn/ccpnv3/ccp/molecule/MolSystem/default+default_user_2024-02-24-15-54-35-583_00004.xml
+-rw-r--r--   0        0        0     3732 2020-02-02 00:00:00.000000 ccpn_project_checker-0.1.6/src/project_checker/test_data/delayed_errors/exo_file_time_attrib_invalid.ccpn/ccpnv3/ccp/nmr/Nmr/default+default_user_2024-02-24-15-54-35-583_00001.xml
+-rw-r--r--   0        0        0      868 2020-02-02 00:00:00.000000 ccpn_project_checker-0.1.6/src/project_checker/test_data/delayed_errors/exo_file_time_attrib_invalid.ccpn/ccpnv3/ccpnmr/gui/Task/user+View+default_user_2024-02-24-15-54-35-583_00006.xml
+-rw-r--r--   0        0        0     1014 2020-02-02 00:00:00.000000 ccpn_project_checker-0.1.6/src/project_checker/test_data/delayed_errors/exo_file_time_attrib_invalid.ccpn/ccpnv3/ccpnmr/gui/Window/_ccp_nmr_Nmr_NmrProject___default___+default_user_2024-02-24-15-54-35-583_00005.xml
+-rw-r--r--   0        0        0   179479 2020-02-02 00:00:00.000000 ccpn_project_checker-0.1.6/src/project_checker/test_data/delayed_errors/exo_file_time_attrib_invalid.ccpn/ccpnv3/memops/Implementation/exo_file_time_attrib_invalid.xml
+-rw-r--r--   0        0        0      499 2020-02-02 00:00:00.000000 ccpn_project_checker-0.1.6/src/project_checker/test_data/delayed_errors/exo_file_time_attrib_missing.ccpn/ccpnv3/ccp/lims/RefSampleComponent/default+default_user_2024-02-24-15-54-35-583_00003.xml
+-rw-r--r--   0        0        0      699 2020-02-02 00:00:00.000000 ccpn_project_checker-0.1.6/src/project_checker/test_data/delayed_errors/exo_file_time_attrib_missing.ccpn/ccpnv3/ccp/lims/Sample/default+default_user_2024-02-24-15-54-35-583_00002.xml
+-rw-r--r--   0        0        0      465 2020-02-02 00:00:00.000000 ccpn_project_checker-0.1.6/src/project_checker/test_data/delayed_errors/exo_file_time_attrib_missing.ccpn/ccpnv3/ccp/molecule/MolSystem/default+default_user_2024-02-24-15-54-35-583_00004.xml
+-rw-r--r--   0        0        0     3732 2020-02-02 00:00:00.000000 ccpn_project_checker-0.1.6/src/project_checker/test_data/delayed_errors/exo_file_time_attrib_missing.ccpn/ccpnv3/ccp/nmr/Nmr/default+default_user_2024-02-24-15-54-35-583_00001.xml
+-rw-r--r--   0        0        0      868 2020-02-02 00:00:00.000000 ccpn_project_checker-0.1.6/src/project_checker/test_data/delayed_errors/exo_file_time_attrib_missing.ccpn/ccpnv3/ccpnmr/gui/Task/user+View+default_user_2024-02-24-15-54-35-583_00006.xml
+-rw-r--r--   0        0        0     1014 2020-02-02 00:00:00.000000 ccpn_project_checker-0.1.6/src/project_checker/test_data/delayed_errors/exo_file_time_attrib_missing.ccpn/ccpnv3/ccpnmr/gui/Window/_ccp_nmr_Nmr_NmrProject___default___+default_user_2024-02-24-15-54-35-583_00005.xml
+-rw-r--r--   0        0        0   179479 2020-02-02 00:00:00.000000 ccpn_project_checker-0.1.6/src/project_checker/test_data/delayed_errors/exo_file_time_attrib_missing.ccpn/ccpnv3/memops/Implementation/exo_file_time_attrib_missing.xml
+-rw-r--r--   0        0        0      499 2020-02-02 00:00:00.000000 ccpn_project_checker-0.1.6/src/project_checker/test_data/delayed_errors/exo_file_unknown_package_guid.ccpn/ccpnv3/ccp/lims/RefSampleComponent/default+default_user_2024-02-24-15-54-35-583_00003.xml
+-rw-r--r--   0        0        0      699 2020-02-02 00:00:00.000000 ccpn_project_checker-0.1.6/src/project_checker/test_data/delayed_errors/exo_file_unknown_package_guid.ccpn/ccpnv3/ccp/lims/Sample/default+default_user_2024-02-24-15-54-35-583_00002.xml
+-rw-r--r--   0        0        0      466 2020-02-02 00:00:00.000000 ccpn_project_checker-0.1.6/src/project_checker/test_data/delayed_errors/exo_file_unknown_package_guid.ccpn/ccpnv3/ccp/molecule/MolSystem/default+default_user_2024-02-24-15-54-35-583_00004.xml
+-rw-r--r--   0        0        0     3732 2020-02-02 00:00:00.000000 ccpn_project_checker-0.1.6/src/project_checker/test_data/delayed_errors/exo_file_unknown_package_guid.ccpn/ccpnv3/ccp/nmr/Nmr/default+default_user_2024-02-24-15-54-35-583_00001.xml
+-rw-r--r--   0        0        0      868 2020-02-02 00:00:00.000000 ccpn_project_checker-0.1.6/src/project_checker/test_data/delayed_errors/exo_file_unknown_package_guid.ccpn/ccpnv3/ccpnmr/gui/Task/user+View+default_user_2024-02-24-15-54-35-583_00006.xml
+-rw-r--r--   0        0        0     1014 2020-02-02 00:00:00.000000 ccpn_project_checker-0.1.6/src/project_checker/test_data/delayed_errors/exo_file_unknown_package_guid.ccpn/ccpnv3/ccpnmr/gui/Window/_ccp_nmr_Nmr_NmrProject___default___+default_user_2024-02-24-15-54-35-583_00005.xml
+-rw-r--r--   0        0        0   179479 2020-02-02 00:00:00.000000 ccpn_project_checker-0.1.6/src/project_checker/test_data/delayed_errors/exo_file_unknown_package_guid.ccpn/ccpnv3/memops/Implementation/exo_file_unknown_package_guid.xml
+-rw-r--r--   0        0        0      499 2020-02-02 00:00:00.000000 ccpn_project_checker-0.1.6/src/project_checker/test_data/delayed_errors/exo_file_unknown_short_package_name.ccpn/ccpnv3/ccp/lims/RefSampleComponent/default+default_user_2024-02-24-15-54-35-583_00003.xml
+-rw-r--r--   0        0        0      699 2020-02-02 00:00:00.000000 ccpn_project_checker-0.1.6/src/project_checker/test_data/delayed_errors/exo_file_unknown_short_package_name.ccpn/ccpnv3/ccp/lims/Sample/default+default_user_2024-02-24-15-54-35-583_00002.xml
+-rw-r--r--   0        0        0      464 2020-02-02 00:00:00.000000 ccpn_project_checker-0.1.6/src/project_checker/test_data/delayed_errors/exo_file_unknown_short_package_name.ccpn/ccpnv3/ccp/molecule/MolSystem/default+default_user_2024-02-24-15-54-35-583_00004.xml
+-rw-r--r--   0        0        0     3732 2020-02-02 00:00:00.000000 ccpn_project_checker-0.1.6/src/project_checker/test_data/delayed_errors/exo_file_unknown_short_package_name.ccpn/ccpnv3/ccp/nmr/Nmr/default+default_user_2024-02-24-15-54-35-583_00001.xml
+-rw-r--r--   0        0        0      868 2020-02-02 00:00:00.000000 ccpn_project_checker-0.1.6/src/project_checker/test_data/delayed_errors/exo_file_unknown_short_package_name.ccpn/ccpnv3/ccpnmr/gui/Task/user+View+default_user_2024-02-24-15-54-35-583_00006.xml
+-rw-r--r--   0        0        0     1014 2020-02-02 00:00:00.000000 ccpn_project_checker-0.1.6/src/project_checker/test_data/delayed_errors/exo_file_unknown_short_package_name.ccpn/ccpnv3/ccpnmr/gui/Window/_ccp_nmr_Nmr_NmrProject___default___+default_user_2024-02-24-15-54-35-583_00005.xml
+-rw-r--r--   0        0        0   179479 2020-02-02 00:00:00.000000 ccpn_project_checker-0.1.6/src/project_checker/test_data/delayed_errors/exo_file_unknown_short_package_name.ccpn/ccpnv3/memops/Implementation/exo_file_unknown_short_package_name.xml
+-rw-r--r--   0        0        0      499 2020-02-02 00:00:00.000000 ccpn_project_checker-0.1.6/src/project_checker/test_data/delayed_errors/exo_file_wrong_storage_location.ccpn/ccpnv3/ccp/lims/RefSampleComponent/default+default_user_2024-02-24-15-54-35-583_00003.xml
+-rw-r--r--   0        0        0      699 2020-02-02 00:00:00.000000 ccpn_project_checker-0.1.6/src/project_checker/test_data/delayed_errors/exo_file_wrong_storage_location.ccpn/ccpnv3/ccp/lims/Sample/default+default_user_2024-02-24-15-54-35-583_00002.xml
+-rw-r--r--   0        0        0     3732 2020-02-02 00:00:00.000000 ccpn_project_checker-0.1.6/src/project_checker/test_data/delayed_errors/exo_file_wrong_storage_location.ccpn/ccpnv3/ccp/nmr/Nmr/default+default_user_2024-02-24-15-54-35-583_00001.xml
+-rw-r--r--   0        0        0      462 2020-02-02 00:00:00.000000 ccpn_project_checker-0.1.6/src/project_checker/test_data/delayed_errors/exo_file_wrong_storage_location.ccpn/ccpnv3/ccp/nmr/Nmr/default+default_user_2024-02-24-15-54-35-583_00004.xml
+-rw-r--r--   0        0        0      868 2020-02-02 00:00:00.000000 ccpn_project_checker-0.1.6/src/project_checker/test_data/delayed_errors/exo_file_wrong_storage_location.ccpn/ccpnv3/ccpnmr/gui/Task/user+View+default_user_2024-02-24-15-54-35-583_00006.xml
+-rw-r--r--   0        0        0     1014 2020-02-02 00:00:00.000000 ccpn_project_checker-0.1.6/src/project_checker/test_data/delayed_errors/exo_file_wrong_storage_location.ccpn/ccpnv3/ccpnmr/gui/Window/_ccp_nmr_Nmr_NmrProject___default___+default_user_2024-02-24-15-54-35-583_00005.xml
+-rw-r--r--   0        0        0   179479 2020-02-02 00:00:00.000000 ccpn_project_checker-0.1.6/src/project_checker/test_data/delayed_errors/exo_file_wrong_storage_location.ccpn/ccpnv3/memops/Implementation/exo_file_wrong_storage_location.xml
+-rw-r--r--   0        0        0      499 2020-02-02 00:00:00.000000 ccpn_project_checker-0.1.6/src/project_checker/test_data/delayed_errors/exo_link_no_top_object.ccpn/ccpnv3/ccp/lims/RefSampleComponent/default+default_user_2024-02-24-15-54-35-583_00003.xml
+-rw-r--r--   0        0        0      699 2020-02-02 00:00:00.000000 ccpn_project_checker-0.1.6/src/project_checker/test_data/delayed_errors/exo_link_no_top_object.ccpn/ccpnv3/ccp/lims/Sample/default+default_user_2024-02-24-15-54-35-583_00002.xml
+-rw-r--r--   0        0        0      235 2020-02-02 00:00:00.000000 ccpn_project_checker-0.1.6/src/project_checker/test_data/delayed_errors/exo_link_no_top_object.ccpn/ccpnv3/ccp/molecule/MolSystem/default+default_user_2024-02-24-15-54-35-583_00004.xml
+-rw-r--r--   0        0        0     3732 2020-02-02 00:00:00.000000 ccpn_project_checker-0.1.6/src/project_checker/test_data/delayed_errors/exo_link_no_top_object.ccpn/ccpnv3/ccp/nmr/Nmr/default+default_user_2024-02-24-15-54-35-583_00001.xml
+-rw-r--r--   0        0        0      868 2020-02-02 00:00:00.000000 ccpn_project_checker-0.1.6/src/project_checker/test_data/delayed_errors/exo_link_no_top_object.ccpn/ccpnv3/ccpnmr/gui/Task/user+View+default_user_2024-02-24-15-54-35-583_00006.xml
+-rw-r--r--   0        0        0     1014 2020-02-02 00:00:00.000000 ccpn_project_checker-0.1.6/src/project_checker/test_data/delayed_errors/exo_link_no_top_object.ccpn/ccpnv3/ccpnmr/gui/Window/_ccp_nmr_Nmr_NmrProject___default___+default_user_2024-02-24-15-54-35-583_00005.xml
+-rw-r--r--   0        0        0   179479 2020-02-02 00:00:00.000000 ccpn_project_checker-0.1.6/src/project_checker/test_data/delayed_errors/exo_link_no_top_object.ccpn/ccpnv3/memops/Implementation/exo_link_no_top_object.xml
+-rw-r--r--   0        0        0      499 2020-02-02 00:00:00.000000 ccpn_project_checker-0.1.6/src/project_checker/test_data/delayed_errors/exo_link_too_many_top_objects.ccpn/ccpnv3/ccp/lims/RefSampleComponent/default+default_user_2024-02-24-15-54-35-583_00003.xml
+-rw-r--r--   0        0        0      699 2020-02-02 00:00:00.000000 ccpn_project_checker-0.1.6/src/project_checker/test_data/delayed_errors/exo_link_too_many_top_objects.ccpn/ccpnv3/ccp/lims/Sample/default+default_user_2024-02-24-15-54-35-583_00002.xml
+-rw-r--r--   0        0        0      513 2020-02-02 00:00:00.000000 ccpn_project_checker-0.1.6/src/project_checker/test_data/delayed_errors/exo_link_too_many_top_objects.ccpn/ccpnv3/ccp/molecule/MolSystem/default+default_user_2024-02-24-15-54-35-583_00004.xml
+-rw-r--r--   0        0        0     3732 2020-02-02 00:00:00.000000 ccpn_project_checker-0.1.6/src/project_checker/test_data/delayed_errors/exo_link_too_many_top_objects.ccpn/ccpnv3/ccp/nmr/Nmr/default+default_user_2024-02-24-15-54-35-583_00001.xml
+-rw-r--r--   0        0        0      868 2020-02-02 00:00:00.000000 ccpn_project_checker-0.1.6/src/project_checker/test_data/delayed_errors/exo_link_too_many_top_objects.ccpn/ccpnv3/ccpnmr/gui/Task/user+View+default_user_2024-02-24-15-54-35-583_00006.xml
+-rw-r--r--   0        0        0     1014 2020-02-02 00:00:00.000000 ccpn_project_checker-0.1.6/src/project_checker/test_data/delayed_errors/exo_link_too_many_top_objects.ccpn/ccpnv3/ccpnmr/gui/Window/_ccp_nmr_Nmr_NmrProject___default___+default_user_2024-02-24-15-54-35-583_00005.xml
+-rw-r--r--   0        0        0   179479 2020-02-02 00:00:00.000000 ccpn_project_checker-0.1.6/src/project_checker/test_data/delayed_errors/exo_link_too_many_top_objects.ccpn/ccpnv3/memops/Implementation/exo_link_too_many_top_objects.xml
+-rw-r--r--   0        0        0      499 2020-02-02 00:00:00.000000 ccpn_project_checker-0.1.6/src/project_checker/test_data/delayed_errors/exo_linked_file_bad_xml.ccpn/ccpnv3/ccp/lims/RefSampleComponent/default+default_user_2024-02-24-15-54-35-583_00003.xml
+-rw-r--r--   0        0        0      699 2020-02-02 00:00:00.000000 ccpn_project_checker-0.1.6/src/project_checker/test_data/delayed_errors/exo_linked_file_bad_xml.ccpn/ccpnv3/ccp/lims/Sample/default+default_user_2024-02-24-15-54-35-583_00002.xml
+-rw-r--r--   0        0        0      461 2020-02-02 00:00:00.000000 ccpn_project_checker-0.1.6/src/project_checker/test_data/delayed_errors/exo_linked_file_bad_xml.ccpn/ccpnv3/ccp/molecule/MolSystem/default+default_user_2024-02-24-15-54-35-583_00004.xml
+-rw-r--r--   0        0        0     3732 2020-02-02 00:00:00.000000 ccpn_project_checker-0.1.6/src/project_checker/test_data/delayed_errors/exo_linked_file_bad_xml.ccpn/ccpnv3/ccp/nmr/Nmr/default+default_user_2024-02-24-15-54-35-583_00001.xml
+-rw-r--r--   0        0        0      868 2020-02-02 00:00:00.000000 ccpn_project_checker-0.1.6/src/project_checker/test_data/delayed_errors/exo_linked_file_bad_xml.ccpn/ccpnv3/ccpnmr/gui/Task/user+View+default_user_2024-02-24-15-54-35-583_00006.xml
+-rw-r--r--   0        0        0     1014 2020-02-02 00:00:00.000000 ccpn_project_checker-0.1.6/src/project_checker/test_data/delayed_errors/exo_linked_file_bad_xml.ccpn/ccpnv3/ccpnmr/gui/Window/_ccp_nmr_Nmr_NmrProject___default___+default_user_2024-02-24-15-54-35-583_00005.xml
+-rw-r--r--   0        0        0   179479 2020-02-02 00:00:00.000000 ccpn_project_checker-0.1.6/src/project_checker/test_data/delayed_errors/exo_linked_file_bad_xml.ccpn/ccpnv3/memops/Implementation/exo_linked_file_bad_xml.xml
+-rw-r--r--   0        0        0      499 2020-02-02 00:00:00.000000 ccpn_project_checker-0.1.6/src/project_checker/test_data/delayed_errors/exo_linked_file_missing.ccpn/ccpnv3/ccp/lims/RefSampleComponent/default+default_user_2024-02-24-15-54-35-583_00003.xml
+-rw-r--r--   0        0        0      699 2020-02-02 00:00:00.000000 ccpn_project_checker-0.1.6/src/project_checker/test_data/delayed_errors/exo_linked_file_missing.ccpn/ccpnv3/ccp/lims/Sample/default+default_user_2024-02-24-15-54-35-583_00002.xml
+-rw-r--r--   0        0        0        0 2020-02-02 00:00:00.000000 ccpn_project_checker-0.1.6/src/project_checker/test_data/delayed_errors/exo_linked_file_missing.ccpn/ccpnv3/ccp/molecule/MolSystem/.keep_alive
+-rw-r--r--   0        0        0     3732 2020-02-02 00:00:00.000000 ccpn_project_checker-0.1.6/src/project_checker/test_data/delayed_errors/exo_linked_file_missing.ccpn/ccpnv3/ccp/nmr/Nmr/default+default_user_2024-02-24-15-54-35-583_00001.xml
+-rw-r--r--   0        0        0      868 2020-02-02 00:00:00.000000 ccpn_project_checker-0.1.6/src/project_checker/test_data/delayed_errors/exo_linked_file_missing.ccpn/ccpnv3/ccpnmr/gui/Task/user+View+default_user_2024-02-24-15-54-35-583_00006.xml
+-rw-r--r--   0        0        0     1014 2020-02-02 00:00:00.000000 ccpn_project_checker-0.1.6/src/project_checker/test_data/delayed_errors/exo_linked_file_missing.ccpn/ccpnv3/ccpnmr/gui/Window/_ccp_nmr_Nmr_NmrProject___default___+default_user_2024-02-24-15-54-35-583_00005.xml
+-rw-r--r--   0        0        0   179479 2020-02-02 00:00:00.000000 ccpn_project_checker-0.1.6/src/project_checker/test_data/delayed_errors/exo_linked_file_missing.ccpn/ccpnv3/memops/Implementation/exo_linked_file_missing.xml
+-rw-r--r--   0        0        0      499 2020-02-02 00:00:00.000000 ccpn_project_checker-0.1.6/src/project_checker/test_data/delayed_errors/exo_linked_file_no_storage_unit.ccpn/ccpnv3/ccp/lims/RefSampleComponent/default+default_user_2024-02-24-15-54-35-583_00003.xml
+-rw-r--r--   0        0        0      699 2020-02-02 00:00:00.000000 ccpn_project_checker-0.1.6/src/project_checker/test_data/delayed_errors/exo_linked_file_no_storage_unit.ccpn/ccpnv3/ccp/lims/Sample/default+default_user_2024-02-24-15-54-35-583_00002.xml
+-rw-r--r--   0        0        0      466 2020-02-02 00:00:00.000000 ccpn_project_checker-0.1.6/src/project_checker/test_data/delayed_errors/exo_linked_file_no_storage_unit.ccpn/ccpnv3/ccp/molecule/MolSystem/default+default_user_2024-02-24-15-54-35-583_00004.xml
+-rw-r--r--   0        0        0     3732 2020-02-02 00:00:00.000000 ccpn_project_checker-0.1.6/src/project_checker/test_data/delayed_errors/exo_linked_file_no_storage_unit.ccpn/ccpnv3/ccp/nmr/Nmr/default+default_user_2024-02-24-15-54-35-583_00001.xml
+-rw-r--r--   0        0        0      868 2020-02-02 00:00:00.000000 ccpn_project_checker-0.1.6/src/project_checker/test_data/delayed_errors/exo_linked_file_no_storage_unit.ccpn/ccpnv3/ccpnmr/gui/Task/user+View+default_user_2024-02-24-15-54-35-583_00006.xml
+-rw-r--r--   0        0        0     1014 2020-02-02 00:00:00.000000 ccpn_project_checker-0.1.6/src/project_checker/test_data/delayed_errors/exo_linked_file_no_storage_unit.ccpn/ccpnv3/ccpnmr/gui/Window/_ccp_nmr_Nmr_NmrProject___default___+default_user_2024-02-24-15-54-35-583_00005.xml
+-rw-r--r--   0        0        0   179479 2020-02-02 00:00:00.000000 ccpn_project_checker-0.1.6/src/project_checker/test_data/delayed_errors/exo_linked_file_no_storage_unit.ccpn/ccpnv3/memops/Implementation/exo_linked_file_no_storage_unit.xml
+-rw-r--r--   0        0        0      499 2020-02-02 00:00:00.000000 ccpn_project_checker-0.1.6/src/project_checker/test_data/delayed_errors/exo_links_with_keys_outside_ccpn_character_set.ccpn/ccpnv3/ccp/lims/RefSampleComponent/default+default_user_2024-02-24-15-54-35-583_00003.xml
+-rw-r--r--   0        0        0      699 2020-02-02 00:00:00.000000 ccpn_project_checker-0.1.6/src/project_checker/test_data/delayed_errors/exo_links_with_keys_outside_ccpn_character_set.ccpn/ccpnv3/ccp/lims/Sample/default+default_user_2024-02-24-15-54-35-583_00002.xml
+-rw-r--r--   0        0        0      462 2020-02-02 00:00:00.000000 ccpn_project_checker-0.1.6/src/project_checker/test_data/delayed_errors/exo_links_with_keys_outside_ccpn_character_set.ccpn/ccpnv3/ccp/molecule/MolSystem/default+default_user_2024-02-24-15-54-35-583_00004.xml
+-rw-r--r--   0        0        0     3732 2020-02-02 00:00:00.000000 ccpn_project_checker-0.1.6/src/project_checker/test_data/delayed_errors/exo_links_with_keys_outside_ccpn_character_set.ccpn/ccpnv3/ccp/nmr/Nmr/default+default_user_2024-02-24-15-54-35-583_00001.xml
+-rw-r--r--   0        0        0      868 2020-02-02 00:00:00.000000 ccpn_project_checker-0.1.6/src/project_checker/test_data/delayed_errors/exo_links_with_keys_outside_ccpn_character_set.ccpn/ccpnv3/ccpnmr/gui/Task/user+View~+default_user_2024-02-24-15-54-35-583_00006.xml
+-rw-r--r--   0        0        0     1014 2020-02-02 00:00:00.000000 ccpn_project_checker-0.1.6/src/project_checker/test_data/delayed_errors/exo_links_with_keys_outside_ccpn_character_set.ccpn/ccpnv3/ccpnmr/gui/Window/_ccp_nmr_Nmr_NmrProject___default___+default_user_2024-02-24-15-54-35-583_00005.xml
+-rw-r--r--   0        0        0   179571 2020-02-02 00:00:00.000000 ccpn_project_checker-0.1.6/src/project_checker/test_data/delayed_errors/exo_links_with_keys_outside_ccpn_character_set.ccpn/ccpnv3/memops/Implementation/exo_links_with_keys_outside_ccpn_character_set.xml
+-rw-r--r--   0        0        0      499 2020-02-02 00:00:00.000000 ccpn_project_checker-0.1.6/src/project_checker/test_data/delayed_errors/external_guid_doesnt_match_internal.ccpn/ccpnv3/ccp/lims/RefSampleComponent/default+default_user_2024-02-24-15-54-35-583_00003.xml
+-rw-r--r--   0        0        0      699 2020-02-02 00:00:00.000000 ccpn_project_checker-0.1.6/src/project_checker/test_data/delayed_errors/external_guid_doesnt_match_internal.ccpn/ccpnv3/ccp/lims/Sample/default+default_user_2024-02-24-15-54-35-583_00002.xml
+-rw-r--r--   0        0        0      451 2020-02-02 00:00:00.000000 ccpn_project_checker-0.1.6/src/project_checker/test_data/delayed_errors/external_guid_doesnt_match_internal.ccpn/ccpnv3/ccp/molecule/MolSystem/default+default_user_2024-02-24-15-54-35-583_00004.xml
+-rw-r--r--   0        0        0     3732 2020-02-02 00:00:00.000000 ccpn_project_checker-0.1.6/src/project_checker/test_data/delayed_errors/external_guid_doesnt_match_internal.ccpn/ccpnv3/ccp/nmr/Nmr/default+default_user_2024-02-24-15-54-35-583_00001.xml
+-rw-r--r--   0        0        0      868 2020-02-02 00:00:00.000000 ccpn_project_checker-0.1.6/src/project_checker/test_data/delayed_errors/external_guid_doesnt_match_internal.ccpn/ccpnv3/ccpnmr/gui/Task/user+View+default_user_2024-02-24-15-54-35-583_00006.xml
+-rw-r--r--   0        0        0     1014 2020-02-02 00:00:00.000000 ccpn_project_checker-0.1.6/src/project_checker/test_data/delayed_errors/external_guid_doesnt_match_internal.ccpn/ccpnv3/ccpnmr/gui/Window/_ccp_nmr_Nmr_NmrProject___default___+default_user_2024-02-24-15-54-35-583_00005.xml
+-rw-r--r--   0        0        0   179479 2020-02-02 00:00:00.000000 ccpn_project_checker-0.1.6/src/project_checker/test_data/delayed_errors/external_guid_doesnt_match_internal.ccpn/ccpnv3/memops/Implementation/external_guid_doesnt_match_internal.xml
+-rw-r--r--   0        0        0      499 2020-02-02 00:00:00.000000 ccpn_project_checker-0.1.6/src/project_checker/test_data/delayed_errors/root_exo_link_missing_source_element.ccpn/ccpnv3/ccp/lims/RefSampleComponent/default+default_user_2024-02-24-15-54-35-583_00003.xml
+-rw-r--r--   0        0        0      699 2020-02-02 00:00:00.000000 ccpn_project_checker-0.1.6/src/project_checker/test_data/delayed_errors/root_exo_link_missing_source_element.ccpn/ccpnv3/ccp/lims/Sample/default+default_user_2024-02-24-15-54-35-583_00002.xml
+-rw-r--r--   0        0        0      462 2020-02-02 00:00:00.000000 ccpn_project_checker-0.1.6/src/project_checker/test_data/delayed_errors/root_exo_link_missing_source_element.ccpn/ccpnv3/ccp/molecule/MolSystem/default+default_user_2024-02-24-15-54-35-583_00004.xml
+-rw-r--r--   0        0        0     3732 2020-02-02 00:00:00.000000 ccpn_project_checker-0.1.6/src/project_checker/test_data/delayed_errors/root_exo_link_missing_source_element.ccpn/ccpnv3/ccp/nmr/Nmr/default+default_user_2024-02-24-15-54-35-583_00001.xml
+-rw-r--r--   0        0        0      868 2020-02-02 00:00:00.000000 ccpn_project_checker-0.1.6/src/project_checker/test_data/delayed_errors/root_exo_link_missing_source_element.ccpn/ccpnv3/ccpnmr/gui/Task/user+View+default_user_2024-02-24-15-54-35-583_00006.xml
+-rw-r--r--   0        0        0     1014 2020-02-02 00:00:00.000000 ccpn_project_checker-0.1.6/src/project_checker/test_data/delayed_errors/root_exo_link_missing_source_element.ccpn/ccpnv3/ccpnmr/gui/Window/_ccp_nmr_Nmr_NmrProject___default___+default_user_2024-02-24-15-54-35-583_00005.xml
+-rw-r--r--   0        0        0   179486 2020-02-02 00:00:00.000000 ccpn_project_checker-0.1.6/src/project_checker/test_data/delayed_errors/root_exo_link_missing_source_element.ccpn/ccpnv3/memops/Implementation/root_exo_link_missing_source_element.xml
+-rw-r--r--   0        0        0      499 2020-02-02 00:00:00.000000 ccpn_project_checker-0.1.6/src/project_checker/test_data/delayed_errors/root_exo_link_too_many_source_elements.ccpn/ccpnv3/ccp/lims/RefSampleComponent/default+default_user_2024-02-24-15-54-35-583_00003.xml
+-rw-r--r--   0        0        0      699 2020-02-02 00:00:00.000000 ccpn_project_checker-0.1.6/src/project_checker/test_data/delayed_errors/root_exo_link_too_many_source_elements.ccpn/ccpnv3/ccp/lims/Sample/default+default_user_2024-02-24-15-54-35-583_00002.xml
+-rw-r--r--   0        0        0      462 2020-02-02 00:00:00.000000 ccpn_project_checker-0.1.6/src/project_checker/test_data/delayed_errors/root_exo_link_too_many_source_elements.ccpn/ccpnv3/ccp/molecule/MolSystem/default+default_user_2024-02-24-15-54-35-583_00004.xml
+-rw-r--r--   0        0        0     3732 2020-02-02 00:00:00.000000 ccpn_project_checker-0.1.6/src/project_checker/test_data/delayed_errors/root_exo_link_too_many_source_elements.ccpn/ccpnv3/ccp/nmr/Nmr/default+default_user_2024-02-24-15-54-35-583_00001.xml
+-rw-r--r--   0        0        0      868 2020-02-02 00:00:00.000000 ccpn_project_checker-0.1.6/src/project_checker/test_data/delayed_errors/root_exo_link_too_many_source_elements.ccpn/ccpnv3/ccpnmr/gui/Task/user+View+default_user_2024-02-24-15-54-35-583_00006.xml
+-rw-r--r--   0        0        0     1014 2020-02-02 00:00:00.000000 ccpn_project_checker-0.1.6/src/project_checker/test_data/delayed_errors/root_exo_link_too_many_source_elements.ccpn/ccpnv3/ccpnmr/gui/Window/_ccp_nmr_Nmr_NmrProject___default___+default_user_2024-02-24-15-54-35-583_00005.xml
+-rw-r--r--   0        0        0   179777 2020-02-02 00:00:00.000000 ccpn_project_checker-0.1.6/src/project_checker/test_data/delayed_errors/root_exo_link_too_many_source_elements.ccpn/ccpnv3/memops/Implementation/root_exo_link_too_many_source_elements.xml
+-rw-r--r--   0        0        0        0 2020-02-02 00:00:00.000000 ccpn_project_checker-0.1.6/src/project_checker/test_data/empty_Implementation.ccpn/ccpnv3/memops/Implementation/.keep_alive
+-rw-r--r--   0        0        0        0 2020-02-02 00:00:00.000000 ccpn_project_checker-0.1.6/src/project_checker/test_data/empty_ccpnv3.ccpn/ccpnv3/.keep_alive
+-rw-r--r--   0        0        0      499 2020-02-02 00:00:00.000000 ccpn_project_checker-0.1.6/src/project_checker/test_data/empty_good_project_multiple_root_xml_files.ccpn/ccpnv3/ccp/lims/RefSampleComponent/default+default_user_2024-02-24-15-54-35-583_00003.xml
+-rw-r--r--   0        0        0      699 2020-02-02 00:00:00.000000 ccpn_project_checker-0.1.6/src/project_checker/test_data/empty_good_project_multiple_root_xml_files.ccpn/ccpnv3/ccp/lims/Sample/default+default_user_2024-02-24-15-54-35-583_00002.xml
+-rw-r--r--   0        0        0      462 2020-02-02 00:00:00.000000 ccpn_project_checker-0.1.6/src/project_checker/test_data/empty_good_project_multiple_root_xml_files.ccpn/ccpnv3/ccp/molecule/MolSystem/default+default_user_2024-02-24-15-54-35-583_00004.xml
+-rw-r--r--   0        0        0     3732 2020-02-02 00:00:00.000000 ccpn_project_checker-0.1.6/src/project_checker/test_data/empty_good_project_multiple_root_xml_files.ccpn/ccpnv3/ccp/nmr/Nmr/default+default_user_2024-02-24-15-54-35-583_00001.xml
+-rw-r--r--   0        0        0      868 2020-02-02 00:00:00.000000 ccpn_project_checker-0.1.6/src/project_checker/test_data/empty_good_project_multiple_root_xml_files.ccpn/ccpnv3/ccpnmr/gui/Task/user+View+default_user_2024-02-24-15-54-35-583_00006.xml
+-rw-r--r--   0        0        0     1014 2020-02-02 00:00:00.000000 ccpn_project_checker-0.1.6/src/project_checker/test_data/empty_good_project_multiple_root_xml_files.ccpn/ccpnv3/ccpnmr/gui/Window/_ccp_nmr_Nmr_NmrProject___default___+default_user_2024-02-24-15-54-35-583_00005.xml
+-rw-r--r--   0        0        0   179503 2020-02-02 00:00:00.000000 ccpn_project_checker-0.1.6/src/project_checker/test_data/empty_good_project_multiple_root_xml_files.ccpn/ccpnv3/memops/Implementation/empty_good_project_mutiple_root_xml_files_1.xml
+-rw-r--r--   0        0        0   179503 2020-02-02 00:00:00.000000 ccpn_project_checker-0.1.6/src/project_checker/test_data/empty_good_project_multiple_root_xml_files.ccpn/ccpnv3/memops/Implementation/empty_good_project_mutiple_root_xml_files_2.xml
+-rw-r--r--   0        0        0        0 2020-02-02 00:00:00.000000 ccpn_project_checker-0.1.6/src/project_checker/test_data/empty_project/.keep_alive
+-rw-r--r--   0        0        0        0 2020-02-02 00:00:00.000000 ccpn_project_checker-0.1.6/src/project_checker/test_data/empty_project.ccpn/.keep_alive
+-rw-r--r--   0        0        0        0 2020-02-02 00:00:00.000000 ccpn_project_checker-0.1.6/src/project_checker/test_data/empty_project_no_extension_ccpn/.keep_alive
+-rw-r--r--   0        0        0      257 2020-02-02 00:00:00.000000 ccpn_project_checker-0.1.6/src/project_checker/test_data/empty_storage_unit.ccpn/ccpnv3/memops/Implementation/empty_storage_unit.xml
+-rw-r--r--   0        0        0     1710 2020-02-02 00:00:00.000000 ccpn_project_checker-0.1.6/src/project_checker/test_data/good_projects/Sec5Part4.ccpn/ccpnv3/ccp/general/DataLocation/standard+default_user_2022-02-23-14-57-20-615_00001.xml
+-rw-r--r--   0        0        0     1614 2020-02-02 00:00:00.000000 ccpn_project_checker-0.1.6/src/project_checker/test_data/good_projects/Sec5Part4.ccpn/ccpnv3/ccp/general/DataLocation/standard+default_user_2022-02-23-14-57-20-615_00001.xml.bak
+-rw-r--r--   0        0        0     1501 2020-02-02 00:00:00.000000 ccpn_project_checker-0.1.6/src/project_checker/test_data/good_projects/Sec5Part4.ccpn/ccpnv3/ccp/lims/RefSampleComponent/default+default_user_2022-02-23-14-57-20-616_00003.xml
+-rw-r--r--   0        0        0     1500 2020-02-02 00:00:00.000000 ccpn_project_checker-0.1.6/src/project_checker/test_data/good_projects/Sec5Part4.ccpn/ccpnv3/ccp/lims/RefSampleComponent/default+default_user_2022-02-23-14-57-20-616_00003.xml.bak
+-rw-r--r--   0        0        0      699 2020-02-02 00:00:00.000000 ccpn_project_checker-0.1.6/src/project_checker/test_data/good_projects/Sec5Part4.ccpn/ccpnv3/ccp/lims/Sample/default+default_user_2022-02-23-14-57-20-616_00002.xml
+-rw-r--r--   0        0        0  1148277 2020-02-02 00:00:00.000000 ccpn_project_checker-0.1.6/src/project_checker/test_data/good_projects/Sec5Part4.ccpn/ccpnv3/ccp/molecule/MolSystem/default+default_user_2022-02-23-14-57-20-617_00001.xml
+-rw-r--r--   0        0        0  1146139 2020-02-02 00:00:00.000000 ccpn_project_checker-0.1.6/src/project_checker/test_data/good_projects/Sec5Part4.ccpn/ccpnv3/ccp/molecule/MolSystem/default+default_user_2022-02-23-14-57-20-617_00001.xml.bak
+-rw-r--r--   0        0        0    76531 2020-02-02 00:00:00.000000 ccpn_project_checker-0.1.6/src/project_checker/test_data/good_projects/Sec5Part4.ccpn/ccpnv3/ccp/molecule/Molecule/Sec5+Sec5Part1_user_2022-02-23-15-20-24-415_00001.xml
+-rw-r--r--   0        0        0  2057337 2020-02-02 00:00:00.000000 ccpn_project_checker-0.1.6/src/project_checker/test_data/good_projects/Sec5Part4.ccpn/ccpnv3/ccp/nmr/Nmr/default+default_user_2022-02-23-14-57-20-616_00001.xml
+-rw-r--r--   0        0        0  2055804 2020-02-02 00:00:00.000000 ccpn_project_checker-0.1.6/src/project_checker/test_data/good_projects/Sec5Part4.ccpn/ccpnv3/ccp/nmr/Nmr/default+default_user_2022-02-23-14-57-20-616_00001.xml.bak
+-rw-r--r--   0        0        0    14319 2020-02-02 00:00:00.000000 ccpn_project_checker-0.1.6/src/project_checker/test_data/good_projects/Sec5Part4.ccpn/ccpnv3/ccpnmr/gui/Task/user+View+default_user_2022-02-23-14-57-20-617_00003.xml
+-rw-r--r--   0        0        0    11440 2020-02-02 00:00:00.000000 ccpn_project_checker-0.1.6/src/project_checker/test_data/good_projects/Sec5Part4.ccpn/ccpnv3/ccpnmr/gui/Task/user+View+default_user_2022-02-23-14-57-20-617_00003.xml.bak
+-rw-r--r--   0        0        0     1021 2020-02-02 00:00:00.000000 ccpn_project_checker-0.1.6/src/project_checker/test_data/good_projects/Sec5Part4.ccpn/ccpnv3/ccpnmr/gui/Window/_ccp_nmr_Nmr_NmrProject___default___+default_user_2022-02-23-14-57-20-617_00002.xml
+-rw-r--r--   0        0        0     1020 2020-02-02 00:00:00.000000 ccpn_project_checker-0.1.6/src/project_checker/test_data/good_projects/Sec5Part4.ccpn/ccpnv3/ccpnmr/gui/Window/_ccp_nmr_Nmr_NmrProject___default___+default_user_2022-02-23-14-57-20-617_00002.xml.bak
+-rw-r--r--   0        0        0   182235 2020-02-02 00:00:00.000000 ccpn_project_checker-0.1.6/src/project_checker/test_data/good_projects/Sec5Part4.ccpn/ccpnv3/memops/Implementation/Sec5Part4.xml
+-rw-r--r--   0        0        0   347669 2020-02-02 00:00:00.000000 ccpn_project_checker-0.1.6/src/project_checker/test_data/good_projects/Sec5Part4.ccpn/ccpnv3/memops/Implementation/Sec5Part4.xml.bak
+-rw-r--r--   0        0        0      499 2020-02-02 00:00:00.000000 ccpn_project_checker-0.1.6/src/project_checker/test_data/good_projects/empty_good_project.ccpn/ccpnv3/ccp/lims/RefSampleComponent/default+default_user_2024-02-24-15-54-35-583_00003.xml
+-rw-r--r--   0        0        0      699 2020-02-02 00:00:00.000000 ccpn_project_checker-0.1.6/src/project_checker/test_data/good_projects/empty_good_project.ccpn/ccpnv3/ccp/lims/Sample/default+default_user_2024-02-24-15-54-35-583_00002.xml
+-rw-r--r--   0        0        0      462 2020-02-02 00:00:00.000000 ccpn_project_checker-0.1.6/src/project_checker/test_data/good_projects/empty_good_project.ccpn/ccpnv3/ccp/molecule/MolSystem/default+default_user_2024-02-24-15-54-35-583_00004.xml
+-rw-r--r--   0        0        0     3732 2020-02-02 00:00:00.000000 ccpn_project_checker-0.1.6/src/project_checker/test_data/good_projects/empty_good_project.ccpn/ccpnv3/ccp/nmr/Nmr/default+default_user_2024-02-24-15-54-35-583_00001.xml
+-rw-r--r--   0        0        0      868 2020-02-02 00:00:00.000000 ccpn_project_checker-0.1.6/src/project_checker/test_data/good_projects/empty_good_project.ccpn/ccpnv3/ccpnmr/gui/Task/user+View+default_user_2024-02-24-15-54-35-583_00006.xml
+-rw-r--r--   0        0        0     1014 2020-02-02 00:00:00.000000 ccpn_project_checker-0.1.6/src/project_checker/test_data/good_projects/empty_good_project.ccpn/ccpnv3/ccpnmr/gui/Window/_ccp_nmr_Nmr_NmrProject___default___+default_user_2024-02-24-15-54-35-583_00005.xml
+-rw-r--r--   0        0        0   179479 2020-02-02 00:00:00.000000 ccpn_project_checker-0.1.6/src/project_checker/test_data/good_projects/empty_good_project.ccpn/ccpnv3/memops/Implementation/empty_good_project.xml
+-rw-r--r--   0        0        0      499 2020-02-02 00:00:00.000000 ccpn_project_checker-0.1.6/src/project_checker/test_data/good_projects/empty_good_project_renamed.ccpn/ccpnv3/ccp/lims/RefSampleComponent/default+default_user_2024-02-24-15-54-35-583_00003.xml
+-rw-r--r--   0        0        0      699 2020-02-02 00:00:00.000000 ccpn_project_checker-0.1.6/src/project_checker/test_data/good_projects/empty_good_project_renamed.ccpn/ccpnv3/ccp/lims/Sample/default+default_user_2024-02-24-15-54-35-583_00002.xml
+-rw-r--r--   0        0        0      462 2020-02-02 00:00:00.000000 ccpn_project_checker-0.1.6/src/project_checker/test_data/good_projects/empty_good_project_renamed.ccpn/ccpnv3/ccp/molecule/MolSystem/default+default_user_2024-02-24-15-54-35-583_00004.xml
+-rw-r--r--   0        0        0     3732 2020-02-02 00:00:00.000000 ccpn_project_checker-0.1.6/src/project_checker/test_data/good_projects/empty_good_project_renamed.ccpn/ccpnv3/ccp/nmr/Nmr/default+default_user_2024-02-24-15-54-35-583_00001.xml
+-rw-r--r--   0        0        0      868 2020-02-02 00:00:00.000000 ccpn_project_checker-0.1.6/src/project_checker/test_data/good_projects/empty_good_project_renamed.ccpn/ccpnv3/ccpnmr/gui/Task/user+View+default_user_2024-02-24-15-54-35-583_00006.xml
+-rw-r--r--   0        0        0     1014 2020-02-02 00:00:00.000000 ccpn_project_checker-0.1.6/src/project_checker/test_data/good_projects/empty_good_project_renamed.ccpn/ccpnv3/ccpnmr/gui/Window/_ccp_nmr_Nmr_NmrProject___default___+default_user_2024-02-24-15-54-35-583_00005.xml
+-rw-r--r--   0        0        0   179479 2020-02-02 00:00:00.000000 ccpn_project_checker-0.1.6/src/project_checker/test_data/good_projects/empty_good_project_renamed.ccpn/ccpnv3/memops/Implementation/empty_good_project_renamed.xml
+-rw-r--r--   0        0        0      499 2020-02-02 00:00:00.000000 ccpn_project_checker-0.1.6/src/project_checker/test_data/memops_root_no_read_empty_good_project.ccpn/ccpnv3/ccp/lims/RefSampleComponent/default+default_user_2024-02-24-15-54-35-583_00003.xml
+-rw-r--r--   0        0        0      699 2020-02-02 00:00:00.000000 ccpn_project_checker-0.1.6/src/project_checker/test_data/memops_root_no_read_empty_good_project.ccpn/ccpnv3/ccp/lims/Sample/default+default_user_2024-02-24-15-54-35-583_00002.xml
+-rw-r--r--   0        0        0      462 2020-02-02 00:00:00.000000 ccpn_project_checker-0.1.6/src/project_checker/test_data/memops_root_no_read_empty_good_project.ccpn/ccpnv3/ccp/molecule/MolSystem/default+default_user_2024-02-24-15-54-35-583_00004.xml
+-rw-r--r--   0        0        0     3732 2020-02-02 00:00:00.000000 ccpn_project_checker-0.1.6/src/project_checker/test_data/memops_root_no_read_empty_good_project.ccpn/ccpnv3/ccp/nmr/Nmr/default+default_user_2024-02-24-15-54-35-583_00001.xml
+-rw-r--r--   0        0        0      868 2020-02-02 00:00:00.000000 ccpn_project_checker-0.1.6/src/project_checker/test_data/memops_root_no_read_empty_good_project.ccpn/ccpnv3/ccpnmr/gui/Task/user+View+default_user_2024-02-24-15-54-35-583_00006.xml
+-rw-r--r--   0        0        0     1014 2020-02-02 00:00:00.000000 ccpn_project_checker-0.1.6/src/project_checker/test_data/memops_root_no_read_empty_good_project.ccpn/ccpnv3/ccpnmr/gui/Window/_ccp_nmr_Nmr_NmrProject___default___+default_user_2024-02-24-15-54-35-583_00005.xml
+-rw-r--r--   0        0        0   179479 2020-02-02 00:00:00.000000 ccpn_project_checker-0.1.6/src/project_checker/test_data/memops_root_no_read_empty_good_project.ccpn/ccpnv3/memops/Implementation/memops_root_no_read_empty_good_project.xml
+-rw-r--r--   0        0        0   179483 2020-02-02 00:00:00.000000 ccpn_project_checker-0.1.6/src/project_checker/test_data/memops_root_no_storage_unit.ccpn/ccpnv3/memops/Implementation/memops_root_no_storage_unit.xml
+-rw-r--r--   0        0        0        0 2020-02-02 00:00:00.000000 ccpn_project_checker-0.1.6/src/project_checker/test_data/memops_root_xml_is_directory.ccpn/ccpnv3/memops/Implementation/memops_root_xml_is_directory.xml/.keep_alive
+-rw-r--r--   0        0        0      455 2020-02-02 00:00:00.000000 ccpn_project_checker-0.1.6/src/project_checker/test_data/no_exo_links.ccpn/ccpnv3/memops/Implementation/no_exo_links.xml
+-rw-r--r--   0        0        0      499 2020-02-02 00:00:00.000000 ccpn_project_checker-0.1.6/src/project_checker/test_data/no_memops_root_element.ccpn/ccpnv3/ccp/lims/RefSampleComponent/default+default_user_2024-02-24-15-54-35-583_00003.xml
+-rw-r--r--   0        0        0      699 2020-02-02 00:00:00.000000 ccpn_project_checker-0.1.6/src/project_checker/test_data/no_memops_root_element.ccpn/ccpnv3/ccp/lims/Sample/default+default_user_2024-02-24-15-54-35-583_00002.xml
+-rw-r--r--   0        0        0      462 2020-02-02 00:00:00.000000 ccpn_project_checker-0.1.6/src/project_checker/test_data/no_memops_root_element.ccpn/ccpnv3/ccp/molecule/MolSystem/default+default_user_2024-02-24-15-54-35-583_00004.xml
+-rw-r--r--   0        0        0     3732 2020-02-02 00:00:00.000000 ccpn_project_checker-0.1.6/src/project_checker/test_data/no_memops_root_element.ccpn/ccpnv3/ccp/nmr/Nmr/default+default_user_2024-02-24-15-54-35-583_00001.xml
+-rw-r--r--   0        0        0      868 2020-02-02 00:00:00.000000 ccpn_project_checker-0.1.6/src/project_checker/test_data/no_memops_root_element.ccpn/ccpnv3/ccpnmr/gui/Task/user+View+default_user_2024-02-24-15-54-35-583_00006.xml
+-rw-r--r--   0        0        0     1014 2020-02-02 00:00:00.000000 ccpn_project_checker-0.1.6/src/project_checker/test_data/no_memops_root_element.ccpn/ccpnv3/ccpnmr/gui/Window/_ccp_nmr_Nmr_NmrProject___default___+default_user_2024-02-24-15-54-35-583_00005.xml
+-rw-r--r--   0        0        0   179485 2020-02-02 00:00:00.000000 ccpn_project_checker-0.1.6/src/project_checker/test_data/no_memops_root_element.ccpn/ccpnv3/memops/Implementation/no_memops_root_element.xml
+-rw-r--r--   0        0        0        0 2020-02-02 00:00:00.000000 ccpn_project_checker-0.1.6/src/project_checker/test_data/no_read_ccpnv3.ccpn/ccpnv3/.keep_alive
+-rw-r--r--   0        0        0        0 2020-02-02 00:00:00.000000 ccpn_project_checker-0.1.6/src/project_checker/test_data/no_read_empty_project.ccpn/.keep_alive
+-rw-r--r--   0        0        0      499 2020-02-02 00:00:00.000000 ccpn_project_checker-0.1.6/src/project_checker/test_data/root_not_memops_root_element.ccpn/ccpnv3/ccp/lims/RefSampleComponent/default+default_user_2024-02-24-15-54-35-583_00003.xml
+-rw-r--r--   0        0        0      699 2020-02-02 00:00:00.000000 ccpn_project_checker-0.1.6/src/project_checker/test_data/root_not_memops_root_element.ccpn/ccpnv3/ccp/lims/Sample/default+default_user_2024-02-24-15-54-35-583_00002.xml
+-rw-r--r--   0        0        0      462 2020-02-02 00:00:00.000000 ccpn_project_checker-0.1.6/src/project_checker/test_data/root_not_memops_root_element.ccpn/ccpnv3/ccp/molecule/MolSystem/default+default_user_2024-02-24-15-54-35-583_00004.xml
+-rw-r--r--   0        0        0     3732 2020-02-02 00:00:00.000000 ccpn_project_checker-0.1.6/src/project_checker/test_data/root_not_memops_root_element.ccpn/ccpnv3/ccp/nmr/Nmr/default+default_user_2024-02-24-15-54-35-583_00001.xml
+-rw-r--r--   0        0        0      868 2020-02-02 00:00:00.000000 ccpn_project_checker-0.1.6/src/project_checker/test_data/root_not_memops_root_element.ccpn/ccpnv3/ccpnmr/gui/Task/user+View+default_user_2024-02-24-15-54-35-583_00006.xml
+-rw-r--r--   0        0        0     1014 2020-02-02 00:00:00.000000 ccpn_project_checker-0.1.6/src/project_checker/test_data/root_not_memops_root_element.ccpn/ccpnv3/ccpnmr/gui/Window/_ccp_nmr_Nmr_NmrProject___default___+default_user_2024-02-24-15-54-35-583_00005.xml
+-rw-r--r--   0        0        0   179485 2020-02-02 00:00:00.000000 ccpn_project_checker-0.1.6/src/project_checker/test_data/root_not_memops_root_element.ccpn/ccpnv3/memops/Implementation/root_not_memops_root_element.xml
+-rw-r--r--   0        0        0      499 2020-02-02 00:00:00.000000 ccpn_project_checker-0.1.6/src/project_checker/test_data/root_version_badly_formatted.ccpn/ccpnv3/ccp/lims/RefSampleComponent/default+default_user_2024-02-24-15-54-35-583_00003.xml
+-rw-r--r--   0        0        0      699 2020-02-02 00:00:00.000000 ccpn_project_checker-0.1.6/src/project_checker/test_data/root_version_badly_formatted.ccpn/ccpnv3/ccp/lims/Sample/default+default_user_2024-02-24-15-54-35-583_00002.xml
+-rw-r--r--   0        0        0      462 2020-02-02 00:00:00.000000 ccpn_project_checker-0.1.6/src/project_checker/test_data/root_version_badly_formatted.ccpn/ccpnv3/ccp/molecule/MolSystem/default+default_user_2024-02-24-15-54-35-583_00004.xml
+-rw-r--r--   0        0        0     3732 2020-02-02 00:00:00.000000 ccpn_project_checker-0.1.6/src/project_checker/test_data/root_version_badly_formatted.ccpn/ccpnv3/ccp/nmr/Nmr/default+default_user_2024-02-24-15-54-35-583_00001.xml
+-rw-r--r--   0        0        0      868 2020-02-02 00:00:00.000000 ccpn_project_checker-0.1.6/src/project_checker/test_data/root_version_badly_formatted.ccpn/ccpnv3/ccpnmr/gui/Task/user+View+default_user_2024-02-24-15-54-35-583_00006.xml
+-rw-r--r--   0        0        0     1014 2020-02-02 00:00:00.000000 ccpn_project_checker-0.1.6/src/project_checker/test_data/root_version_badly_formatted.ccpn/ccpnv3/ccpnmr/gui/Window/_ccp_nmr_Nmr_NmrProject___default___+default_user_2024-02-24-15-54-35-583_00005.xml
+-rw-r--r--   0        0        0   179480 2020-02-02 00:00:00.000000 ccpn_project_checker-0.1.6/src/project_checker/test_data/root_version_badly_formatted.ccpn/ccpnv3/memops/Implementation/root_version_badly_formatted.xml
+-rw-r--r--   0        0        0      499 2020-02-02 00:00:00.000000 ccpn_project_checker-0.1.6/src/project_checker/test_data/root_version_missing.ccpn/ccpnv3/ccp/lims/RefSampleComponent/default+default_user_2024-02-24-15-54-35-583_00003.xml
+-rw-r--r--   0        0        0      699 2020-02-02 00:00:00.000000 ccpn_project_checker-0.1.6/src/project_checker/test_data/root_version_missing.ccpn/ccpnv3/ccp/lims/Sample/default+default_user_2024-02-24-15-54-35-583_00002.xml
+-rw-r--r--   0        0        0      462 2020-02-02 00:00:00.000000 ccpn_project_checker-0.1.6/src/project_checker/test_data/root_version_missing.ccpn/ccpnv3/ccp/molecule/MolSystem/default+default_user_2024-02-24-15-54-35-583_00004.xml
+-rw-r--r--   0        0        0     3732 2020-02-02 00:00:00.000000 ccpn_project_checker-0.1.6/src/project_checker/test_data/root_version_missing.ccpn/ccpnv3/ccp/nmr/Nmr/default+default_user_2024-02-24-15-54-35-583_00001.xml
+-rw-r--r--   0        0        0      868 2020-02-02 00:00:00.000000 ccpn_project_checker-0.1.6/src/project_checker/test_data/root_version_missing.ccpn/ccpnv3/ccpnmr/gui/Task/user+View+default_user_2024-02-24-15-54-35-583_00006.xml
+-rw-r--r--   0        0        0     1014 2020-02-02 00:00:00.000000 ccpn_project_checker-0.1.6/src/project_checker/test_data/root_version_missing.ccpn/ccpnv3/ccpnmr/gui/Window/_ccp_nmr_Nmr_NmrProject___default___+default_user_2024-02-24-15-54-35-583_00005.xml
+-rw-r--r--   0        0        0   179482 2020-02-02 00:00:00.000000 ccpn_project_checker-0.1.6/src/project_checker/test_data/root_version_missing.ccpn/ccpnv3/memops/Implementation/root_version_missing.xml
+-rw-r--r--   0        0        0      499 2020-02-02 00:00:00.000000 ccpn_project_checker-0.1.6/src/project_checker/test_data/too_many_root_elements.ccpn/ccpnv3/ccp/lims/RefSampleComponent/default+default_user_2024-02-24-15-54-35-583_00003.xml
+-rw-r--r--   0        0        0      699 2020-02-02 00:00:00.000000 ccpn_project_checker-0.1.6/src/project_checker/test_data/too_many_root_elements.ccpn/ccpnv3/ccp/lims/Sample/default+default_user_2024-02-24-15-54-35-583_00002.xml
+-rw-r--r--   0        0        0      462 2020-02-02 00:00:00.000000 ccpn_project_checker-0.1.6/src/project_checker/test_data/too_many_root_elements.ccpn/ccpnv3/ccp/molecule/MolSystem/default+default_user_2024-02-24-15-54-35-583_00004.xml
+-rw-r--r--   0        0        0     3732 2020-02-02 00:00:00.000000 ccpn_project_checker-0.1.6/src/project_checker/test_data/too_many_root_elements.ccpn/ccpnv3/ccp/nmr/Nmr/default+default_user_2024-02-24-15-54-35-583_00001.xml
+-rw-r--r--   0        0        0      868 2020-02-02 00:00:00.000000 ccpn_project_checker-0.1.6/src/project_checker/test_data/too_many_root_elements.ccpn/ccpnv3/ccpnmr/gui/Task/user+View+default_user_2024-02-24-15-54-35-583_00006.xml
+-rw-r--r--   0        0        0     1014 2020-02-02 00:00:00.000000 ccpn_project_checker-0.1.6/src/project_checker/test_data/too_many_root_elements.ccpn/ccpnv3/ccpnmr/gui/Window/_ccp_nmr_Nmr_NmrProject___default___+default_user_2024-02-24-15-54-35-583_00005.xml
+-rw-r--r--   0        0        0      438 2020-02-02 00:00:00.000000 ccpn_project_checker-0.1.6/src/project_checker/test_data/too_many_root_elements.ccpn/ccpnv3/memops/Implementation/too_many_root_elements.xml
+-rw-r--r--   0        0        0      499 2020-02-02 00:00:00.000000 ccpn_project_checker-0.1.6/src/project_checker/test_data/warn_projects/empty_good_project_extra_root_xml_files.ccpn/ccpnv3/ccp/lims/RefSampleComponent/default+default_user_2024-02-24-15-54-35-583_00003.xml
+-rw-r--r--   0        0        0      699 2020-02-02 00:00:00.000000 ccpn_project_checker-0.1.6/src/project_checker/test_data/warn_projects/empty_good_project_extra_root_xml_files.ccpn/ccpnv3/ccp/lims/Sample/default+default_user_2024-02-24-15-54-35-583_00002.xml
+-rw-r--r--   0        0        0      462 2020-02-02 00:00:00.000000 ccpn_project_checker-0.1.6/src/project_checker/test_data/warn_projects/empty_good_project_extra_root_xml_files.ccpn/ccpnv3/ccp/molecule/MolSystem/default+default_user_2024-02-24-15-54-35-583_00004.xml
+-rw-r--r--   0        0        0     3732 2020-02-02 00:00:00.000000 ccpn_project_checker-0.1.6/src/project_checker/test_data/warn_projects/empty_good_project_extra_root_xml_files.ccpn/ccpnv3/ccp/nmr/Nmr/default+default_user_2024-02-24-15-54-35-583_00001.xml
+-rw-r--r--   0        0        0      868 2020-02-02 00:00:00.000000 ccpn_project_checker-0.1.6/src/project_checker/test_data/warn_projects/empty_good_project_extra_root_xml_files.ccpn/ccpnv3/ccpnmr/gui/Task/user+View+default_user_2024-02-24-15-54-35-583_00006.xml
+-rw-r--r--   0        0        0     1014 2020-02-02 00:00:00.000000 ccpn_project_checker-0.1.6/src/project_checker/test_data/warn_projects/empty_good_project_extra_root_xml_files.ccpn/ccpnv3/ccpnmr/gui/Window/_ccp_nmr_Nmr_NmrProject___default___+default_user_2024-02-24-15-54-35-583_00005.xml
+-rw-r--r--   0        0        0   179479 2020-02-02 00:00:00.000000 ccpn_project_checker-0.1.6/src/project_checker/test_data/warn_projects/empty_good_project_extra_root_xml_files.ccpn/ccpnv3/memops/Implementation/empty_good_project_extra_root_xml_files.xml
+-rw-r--r--   0        0        0   179479 2020-02-02 00:00:00.000000 ccpn_project_checker-0.1.6/src/project_checker/test_data/warn_projects/empty_good_project_extra_root_xml_files.ccpn/ccpnv3/memops/Implementation/empty_good_project_extra_root_xml_files_2.xml
+-rw-r--r--   0        0        0      499 2020-02-02 00:00:00.000000 ccpn_project_checker-0.1.6/src/project_checker/test_data/warn_projects/empty_good_project_extra_xml_files.ccpn/ccpnv3/ccp/lims/RefSampleComponent/default+default_user_2024-02-24-15-54-35-583_00003.xml
+-rw-r--r--   0        0        0      699 2020-02-02 00:00:00.000000 ccpn_project_checker-0.1.6/src/project_checker/test_data/warn_projects/empty_good_project_extra_xml_files.ccpn/ccpnv3/ccp/lims/Sample/default+default_user_2024-02-24-15-54-35-583_00002.xml
+-rw-r--r--   0        0        0      462 2020-02-02 00:00:00.000000 ccpn_project_checker-0.1.6/src/project_checker/test_data/warn_projects/empty_good_project_extra_xml_files.ccpn/ccpnv3/ccp/molecule/MolSystem/default+default_user_2024-02-24-15-54-35-583_00004.xml
+-rw-r--r--   0        0        0      462 2020-02-02 00:00:00.000000 ccpn_project_checker-0.1.6/src/project_checker/test_data/warn_projects/empty_good_project_extra_xml_files.ccpn/ccpnv3/ccp/molecule/MolSystem/molecule2.xml
+-rw-r--r--   0        0        0     3732 2020-02-02 00:00:00.000000 ccpn_project_checker-0.1.6/src/project_checker/test_data/warn_projects/empty_good_project_extra_xml_files.ccpn/ccpnv3/ccp/nmr/Nmr/default+default_user_2024-02-24-15-54-35-583_00001.xml
+-rw-r--r--   0        0        0      868 2020-02-02 00:00:00.000000 ccpn_project_checker-0.1.6/src/project_checker/test_data/warn_projects/empty_good_project_extra_xml_files.ccpn/ccpnv3/ccpnmr/gui/Task/task_2.xml
+-rw-r--r--   0        0        0      868 2020-02-02 00:00:00.000000 ccpn_project_checker-0.1.6/src/project_checker/test_data/warn_projects/empty_good_project_extra_xml_files.ccpn/ccpnv3/ccpnmr/gui/Task/user+View+default_user_2024-02-24-15-54-35-583_00006.xml
+-rw-r--r--   0        0        0     1014 2020-02-02 00:00:00.000000 ccpn_project_checker-0.1.6/src/project_checker/test_data/warn_projects/empty_good_project_extra_xml_files.ccpn/ccpnv3/ccpnmr/gui/Window/_ccp_nmr_Nmr_NmrProject___default___+default_user_2024-02-24-15-54-35-583_00005.xml
+-rw-r--r--   0        0        0   179479 2020-02-02 00:00:00.000000 ccpn_project_checker-0.1.6/src/project_checker/test_data/warn_projects/empty_good_project_extra_xml_files.ccpn/ccpnv3/memops/Implementation/empty_good_project_extra_xml_files.xml
+-rw-r--r--   0        0        0      499 2020-02-02 00:00:00.000000 ccpn_project_checker-0.1.6/src/project_checker/test_data/warn_projects/empty_good_project_with_empty_containers.ccpn/ccpnv3/ccp/lims/RefSampleComponent/default+default_user_2024-02-24-15-54-35-583_00003.xml
+-rw-r--r--   0        0        0      699 2020-02-02 00:00:00.000000 ccpn_project_checker-0.1.6/src/project_checker/test_data/warn_projects/empty_good_project_with_empty_containers.ccpn/ccpnv3/ccp/lims/Sample/default+default_user_2024-02-24-15-54-35-583_00002.xml
+-rw-r--r--   0        0        0        0 2020-02-02 00:00:00.000000 ccpn_project_checker-0.1.6/src/project_checker/test_data/warn_projects/empty_good_project_with_empty_containers.ccpn/ccpnv3/ccp/molecule/LabeledMolecule/.keep_alive
+-rw-r--r--   0        0        0      462 2020-02-02 00:00:00.000000 ccpn_project_checker-0.1.6/src/project_checker/test_data/warn_projects/empty_good_project_with_empty_containers.ccpn/ccpnv3/ccp/molecule/MolSystem/default+default_user_2024-02-24-15-54-35-583_00004.xml
+-rw-r--r--   0        0        0        0 2020-02-02 00:00:00.000000 ccpn_project_checker-0.1.6/src/project_checker/test_data/warn_projects/empty_good_project_with_empty_containers.ccpn/ccpnv3/ccp/molsim/Symmetry/.keep_alive
+-rw-r--r--   0        0        0     3732 2020-02-02 00:00:00.000000 ccpn_project_checker-0.1.6/src/project_checker/test_data/warn_projects/empty_good_project_with_empty_containers.ccpn/ccpnv3/ccp/nmr/Nmr/default+default_user_2024-02-24-15-54-35-583_00001.xml
+-rw-r--r--   0        0        0      868 2020-02-02 00:00:00.000000 ccpn_project_checker-0.1.6/src/project_checker/test_data/warn_projects/empty_good_project_with_empty_containers.ccpn/ccpnv3/ccpnmr/gui/Task/user+View+default_user_2024-02-24-15-54-35-583_00006.xml
+-rw-r--r--   0        0        0     1014 2020-02-02 00:00:00.000000 ccpn_project_checker-0.1.6/src/project_checker/test_data/warn_projects/empty_good_project_with_empty_containers.ccpn/ccpnv3/ccpnmr/gui/Window/_ccp_nmr_Nmr_NmrProject___default___+default_user_2024-02-24-15-54-35-583_00005.xml
+-rw-r--r--   0        0        0   179479 2020-02-02 00:00:00.000000 ccpn_project_checker-0.1.6/src/project_checker/test_data/warn_projects/empty_good_project_with_empty_containers.ccpn/ccpnv3/memops/Implementation/empty_good_project_with_empty_containers.xml
+-rw-r--r--   0        0        0      499 2020-02-02 00:00:00.000000 ccpn_project_checker-0.1.6/src/project_checker/test_data/warn_projects/root_file_badly_formatted_time.ccpn/ccpnv3/ccp/lims/RefSampleComponent/default+default_user_2024-02-24-15-54-35-583_00003.xml
+-rw-r--r--   0        0        0      699 2020-02-02 00:00:00.000000 ccpn_project_checker-0.1.6/src/project_checker/test_data/warn_projects/root_file_badly_formatted_time.ccpn/ccpnv3/ccp/lims/Sample/default+default_user_2024-02-24-15-54-35-583_00002.xml
+-rw-r--r--   0        0        0      462 2020-02-02 00:00:00.000000 ccpn_project_checker-0.1.6/src/project_checker/test_data/warn_projects/root_file_badly_formatted_time.ccpn/ccpnv3/ccp/molecule/MolSystem/default+default_user_2024-02-24-15-54-35-583_00004.xml
+-rw-r--r--   0        0        0     3732 2020-02-02 00:00:00.000000 ccpn_project_checker-0.1.6/src/project_checker/test_data/warn_projects/root_file_badly_formatted_time.ccpn/ccpnv3/ccp/nmr/Nmr/default+default_user_2024-02-24-15-54-35-583_00001.xml
+-rw-r--r--   0        0        0      868 2020-02-02 00:00:00.000000 ccpn_project_checker-0.1.6/src/project_checker/test_data/warn_projects/root_file_badly_formatted_time.ccpn/ccpnv3/ccpnmr/gui/Task/user+View+default_user_2024-02-24-15-54-35-583_00006.xml
+-rw-r--r--   0        0        0     1014 2020-02-02 00:00:00.000000 ccpn_project_checker-0.1.6/src/project_checker/test_data/warn_projects/root_file_badly_formatted_time.ccpn/ccpnv3/ccpnmr/gui/Window/_ccp_nmr_Nmr_NmrProject___default___+default_user_2024-02-24-15-54-35-583_00005.xml
+-rw-r--r--   0        0        0   179479 2020-02-02 00:00:00.000000 ccpn_project_checker-0.1.6/src/project_checker/test_data/warn_projects/root_file_badly_formatted_time.ccpn/ccpnv3/memops/Implementation/root_file_badly_formatted_time.xml
+-rw-r--r--   0        0        0      499 2020-02-02 00:00:00.000000 ccpn_project_checker-0.1.6/src/project_checker/test_data/warn_projects/root_file_missing_time.ccpn/ccpnv3/ccp/lims/RefSampleComponent/default+default_user_2024-02-24-15-54-35-583_00003.xml
+-rw-r--r--   0        0        0      699 2020-02-02 00:00:00.000000 ccpn_project_checker-0.1.6/src/project_checker/test_data/warn_projects/root_file_missing_time.ccpn/ccpnv3/ccp/lims/Sample/default+default_user_2024-02-24-15-54-35-583_00002.xml
+-rw-r--r--   0        0        0      462 2020-02-02 00:00:00.000000 ccpn_project_checker-0.1.6/src/project_checker/test_data/warn_projects/root_file_missing_time.ccpn/ccpnv3/ccp/molecule/MolSystem/default+default_user_2024-02-24-15-54-35-583_00004.xml
+-rw-r--r--   0        0        0     3732 2020-02-02 00:00:00.000000 ccpn_project_checker-0.1.6/src/project_checker/test_data/warn_projects/root_file_missing_time.ccpn/ccpnv3/ccp/nmr/Nmr/default+default_user_2024-02-24-15-54-35-583_00001.xml
+-rw-r--r--   0        0        0      868 2020-02-02 00:00:00.000000 ccpn_project_checker-0.1.6/src/project_checker/test_data/warn_projects/root_file_missing_time.ccpn/ccpnv3/ccpnmr/gui/Task/user+View+default_user_2024-02-24-15-54-35-583_00006.xml
+-rw-r--r--   0        0        0     1014 2020-02-02 00:00:00.000000 ccpn_project_checker-0.1.6/src/project_checker/test_data/warn_projects/root_file_missing_time.ccpn/ccpnv3/ccpnmr/gui/Window/_ccp_nmr_Nmr_NmrProject___default___+default_user_2024-02-24-15-54-35-583_00005.xml
+-rw-r--r--   0        0        0   179482 2020-02-02 00:00:00.000000 ccpn_project_checker-0.1.6/src/project_checker/test_data/warn_projects/root_file_missing_time.ccpn/ccpnv3/memops/Implementation/root_file_missing_time.xml
+-rw-r--r--   0        0        0        0 2020-02-02 00:00:00.000000 ccpn_project_checker-0.1.6/src/project_checker/tests/__init__.py
+-rw-r--r--   0        0        0    77076 2020-02-02 00:00:00.000000 ccpn_project_checker-0.1.6/src/project_checker/tests/api_test_data.py
+-rw-r--r--   0        0        0     2171 2020-02-02 00:00:00.000000 ccpn_project_checker-0.1.6/src/project_checker/tests/api_test_data_internal.py
+-rw-r--r--   0        0        0      137 2020-02-02 00:00:00.000000 ccpn_project_checker-0.1.6/src/project_checker/tests/cli_test_data.py
+-rw-r--r--   0        0        0     5087 2020-02-02 00:00:00.000000 ccpn_project_checker-0.1.6/src/project_checker/tests/test_api.py
+-rw-r--r--   0        0        0     1074 2020-02-02 00:00:00.000000 ccpn_project_checker-0.1.6/src/project_checker/tests/test_cli.py
+-rw-r--r--   0        0        0     9510 2020-02-02 00:00:00.000000 ccpn_project_checker-0.1.6/src/project_checker/tests/testing_utils.py
+-rw-r--r--   0        0        0      320 2020-02-02 00:00:00.000000 ccpn_project_checker-0.1.6/src/project_checker/tests/write_cli_test_data.py
+-rw-r--r--   0        0        0       92 2020-02-02 00:00:00.000000 ccpn_project_checker-0.1.6/.gitignore
+-rw-r--r--   0        0        0       51 2020-02-02 00:00:00.000000 ccpn_project_checker-0.1.6/README.md
+-rw-r--r--   0        0        0      650 2020-02-02 00:00:00.000000 ccpn_project_checker-0.1.6/pyproject.toml
+-rw-r--r--   0        0        0      378 2020-02-02 00:00:00.000000 ccpn_project_checker-0.1.6/PKG-INFO
```

### Comparing `ccpn_project_checker-0.1.5/TODO.txt` & `ccpn_project_checker-0.1.6/TODO.txt`

 * *Files identical despite different names*

### Comparing `ccpn_project_checker-0.1.5/requirements-dev.lock` & `ccpn_project_checker-0.1.6/requirements-dev.lock`

 * *Files identical despite different names*

### Comparing `ccpn_project_checker-0.1.5/requirements.lock` & `ccpn_project_checker-0.1.6/requirements.lock`

 * *Files identical despite different names*

### Comparing `ccpn_project_checker-0.1.5/project_checker/.idea/workspace.xml` & `ccpn_project_checker-0.1.6/project_checker/.idea/workspace.xml`

 * *Files 0% similar despite different names*

#### Comparing `ccpn_project_checker-0.1.5/project_checker/.idea/workspace.xml` & `ccpn_project_checker-0.1.6/project_checker/.idea/workspace.xml`

```diff
@@ -155,15 +155,15 @@
   <component name="TaskManager">
     <task active="true" id="Default" summary="Default task">
       <changelist id="0806fef8-d399-4c5a-ae72-cc19a2a861c3" name="Changes" comment=""/>
       <created>1711986494142</created>
       <option name="number" value="Default"/>
       <option name="presentableId" value="Default"/>
       <updated>1711986494142</updated>
-      <workItem from="1711986497798" duration="5489000"/>
+      <workItem from="1711986497798" duration="6985000"/>
     </task>
     <task id="LOCAL-00001" summary="initial commit">
       <option name="closed" value="true"/>
       <created>1712045994338</created>
       <option name="number" value="00001"/>
       <option name="presentableId" value="LOCAL-00001"/>
       <option name="project" value="LOCAL"/>
```

### Comparing `ccpn_project_checker-0.1.5/project_checker/.idea/copilot/chatSessions/00000000000.xd` & `ccpn_project_checker-0.1.6/project_checker/.idea/copilot/chatSessions/00000000000.xd`

 * *Files identical despite different names*

### Comparing `ccpn_project_checker-0.1.5/project_checker/.idea/copilot/chatSessions/xd.lck` & `ccpn_project_checker-0.1.6/project_checker/.idea/copilot/chatSessions/xd.lck`

 * *Files identical despite different names*

### Comparing `ccpn_project_checker-0.1.5/src/project_checker/DiskModelChecker.py` & `ccpn_project_checker-0.1.6/src/project_checker/DiskModelChecker.py`

 * *Files identical despite different names*

### Comparing `ccpn_project_checker-0.1.5/src/project_checker/MetaModelWalker.py` & `ccpn_project_checker-0.1.6/src/project_checker/MetaModelWalker.py`

 * *Files identical despite different names*

### Comparing `ccpn_project_checker-0.1.5/src/project_checker/model_info/data_file_names.txt` & `ccpn_project_checker-0.1.6/src/project_checker/model_info/data_file_names.txt`

 * *Files identical despite different names*

### Comparing `ccpn_project_checker-0.1.5/src/project_checker/model_info/v_3_1_0_guid_to_storage_location.json` & `ccpn_project_checker-0.1.6/src/project_checker/model_info/v_3_1_0_guid_to_storage_location.json`

 * *Files identical despite different names*

### Comparing `ccpn_project_checker-0.1.5/src/project_checker/model_info/v_3_1_0_object_info.json` & `ccpn_project_checker-0.1.6/src/project_checker/model_info/v_3_1_0_object_info.json`

 * *Files identical despite different names*

### Comparing `ccpn_project_checker-0.1.5/src/project_checker/model_info/v_3_1_0_short_name_to_guid.json` & `ccpn_project_checker-0.1.6/src/project_checker/model_info/v_3_1_0_short_name_to_guid.json`

 * *Files identical despite different names*

### Comparing `ccpn_project_checker-0.1.5/src/project_checker/optional/abstract_optional.py` & `ccpn_project_checker-0.1.6/src/project_checker/optional/abstract_optional.py`

 * *Files identical despite different names*

### Comparing `ccpn_project_checker-0.1.5/src/project_checker/optional/nothing.py` & `ccpn_project_checker-0.1.6/src/project_checker/optional/nothing.py`

 * *Files identical despite different names*

### Comparing `ccpn_project_checker-0.1.5/src/project_checker/optional/optional.py` & `ccpn_project_checker-0.1.6/src/project_checker/optional/optional.py`

 * *Files identical despite different names*

### Comparing `ccpn_project_checker-0.1.5/src/project_checker/optional/something.py` & `ccpn_project_checker-0.1.6/src/project_checker/optional/something.py`

 * *Files identical despite different names*

### Comparing `ccpn_project_checker-0.1.5/src/project_checker/test_data/cli_test_output.txt` & `ccpn_project_checker-0.1.6/src/project_checker/test_data/cli_test_output.txt`

 * *Files identical despite different names*

### Comparing `ccpn_project_checker-0.1.5/src/project_checker/test_data/bad_memops_root_xml.ccpn/ccpnv3/memops/Implementation/bad_memops_root_xml.xml` & `ccpn_project_checker-0.1.6/src/project_checker/test_data/bad_memops_root_xml.ccpn/ccpnv3/memops/Implementation/bad_memops_root_xml.xml`

 * *Files identical despite different names*

### Comparing `ccpn_project_checker-0.1.5/src/project_checker/test_data/basic_exo_links_not_found.ccpn/ccpnv3/memops/Implementation/basic_exo_links_not_found.xml` & `ccpn_project_checker-0.1.6/src/project_checker/test_data/basic_exo_links_not_found.ccpn/ccpnv3/memops/Implementation/basic_exo_links_not_found.xml`

 * *Files identical despite different names*

### Comparing `ccpn_project_checker-0.1.5/src/project_checker/test_data/delayed_errors/bad_embedded_exo_link_0_child_elements.ccpn/ccpnv3/ccp/lims/Sample/default+default_user_2024-02-24-15-54-35-583_00002.xml` & `ccpn_project_checker-0.1.6/src/project_checker/test_data/delayed_errors/bad_embedded_exo_link_0_child_elements.ccpn/ccpnv3/ccp/lims/Sample/default+default_user_2024-02-24-15-54-35-583_00002.xml`

 * *Files identical despite different names*

### Comparing `ccpn_project_checker-0.1.5/src/project_checker/test_data/delayed_errors/bad_embedded_exo_link_0_child_elements.ccpn/ccpnv3/ccp/nmr/Nmr/default+default_user_2024-02-24-15-54-35-583_00001.xml` & `ccpn_project_checker-0.1.6/src/project_checker/test_data/delayed_errors/bad_embedded_exo_link_0_child_elements.ccpn/ccpnv3/ccp/nmr/Nmr/default+default_user_2024-02-24-15-54-35-583_00001.xml`

 * *Files identical despite different names*

### Comparing `ccpn_project_checker-0.1.5/src/project_checker/test_data/delayed_errors/bad_embedded_exo_link_0_child_elements.ccpn/ccpnv3/ccpnmr/gui/Task/user+View+default_user_2024-02-24-15-54-35-583_00006.xml` & `ccpn_project_checker-0.1.6/src/project_checker/test_data/delayed_errors/bad_embedded_exo_link_0_child_elements.ccpn/ccpnv3/ccpnmr/gui/Task/user+View+default_user_2024-02-24-15-54-35-583_00006.xml`

 * *Files identical despite different names*

### Comparing `ccpn_project_checker-0.1.5/src/project_checker/test_data/delayed_errors/bad_embedded_exo_link_0_child_elements.ccpn/ccpnv3/ccpnmr/gui/Window/_ccp_nmr_Nmr_NmrProject___default___+default_user_2024-02-24-15-54-35-583_00005.xml` & `ccpn_project_checker-0.1.6/src/project_checker/test_data/delayed_errors/bad_embedded_exo_link_0_child_elements.ccpn/ccpnv3/ccpnmr/gui/Window/_ccp_nmr_Nmr_NmrProject___default___+default_user_2024-02-24-15-54-35-583_00005.xml`

 * *Files identical despite different names*

### Comparing `ccpn_project_checker-0.1.5/src/project_checker/test_data/delayed_errors/bad_embedded_exo_link_0_child_elements.ccpn/ccpnv3/memops/Implementation/bad_embedded_exo_link_0_child_elements.xml` & `ccpn_project_checker-0.1.6/src/project_checker/test_data/delayed_errors/bad_embedded_exo_link_0_child_elements.ccpn/ccpnv3/memops/Implementation/bad_embedded_exo_link_0_child_elements.xml`

 * *Files identical despite different names*

### Comparing `ccpn_project_checker-0.1.5/src/project_checker/test_data/delayed_errors/bad_embedded_exo_link_0_elements.ccpn/ccpnv3/ccp/lims/Sample/default+default_user_2024-02-24-15-54-35-583_00002.xml` & `ccpn_project_checker-0.1.6/src/project_checker/test_data/delayed_errors/bad_embedded_exo_link_0_elements.ccpn/ccpnv3/ccp/lims/Sample/default+default_user_2024-02-24-15-54-35-583_00002.xml`

 * *Files identical despite different names*

### Comparing `ccpn_project_checker-0.1.5/src/project_checker/test_data/delayed_errors/bad_embedded_exo_link_0_elements.ccpn/ccpnv3/ccp/nmr/Nmr/default+default_user_2024-02-24-15-54-35-583_00001.xml` & `ccpn_project_checker-0.1.6/src/project_checker/test_data/delayed_errors/bad_embedded_exo_link_0_elements.ccpn/ccpnv3/ccp/nmr/Nmr/default+default_user_2024-02-24-15-54-35-583_00001.xml`

 * *Files identical despite different names*

### Comparing `ccpn_project_checker-0.1.5/src/project_checker/test_data/delayed_errors/bad_embedded_exo_link_0_elements.ccpn/ccpnv3/ccpnmr/gui/Task/user+View+default_user_2024-02-24-15-54-35-583_00006.xml` & `ccpn_project_checker-0.1.6/src/project_checker/test_data/delayed_errors/bad_embedded_exo_link_0_elements.ccpn/ccpnv3/ccpnmr/gui/Task/user+View+default_user_2024-02-24-15-54-35-583_00006.xml`

 * *Files identical despite different names*

### Comparing `ccpn_project_checker-0.1.5/src/project_checker/test_data/delayed_errors/bad_embedded_exo_link_0_elements.ccpn/ccpnv3/ccpnmr/gui/Window/_ccp_nmr_Nmr_NmrProject___default___+default_user_2024-02-24-15-54-35-583_00005.xml` & `ccpn_project_checker-0.1.6/src/project_checker/test_data/delayed_errors/bad_embedded_exo_link_0_elements.ccpn/ccpnv3/ccpnmr/gui/Window/_ccp_nmr_Nmr_NmrProject___default___+default_user_2024-02-24-15-54-35-583_00005.xml`

 * *Files identical despite different names*

### Comparing `ccpn_project_checker-0.1.5/src/project_checker/test_data/delayed_errors/bad_embedded_exo_link_0_elements.ccpn/ccpnv3/memops/Implementation/bad_embedded_exo_link_0_elements.xml` & `ccpn_project_checker-0.1.6/src/project_checker/test_data/delayed_errors/bad_embedded_exo_link_0_elements.ccpn/ccpnv3/memops/Implementation/bad_embedded_exo_link_0_elements.xml`

 * *Files identical despite different names*

### Comparing `ccpn_project_checker-0.1.5/src/project_checker/test_data/delayed_errors/bad_role_exo_link_key_element_children.ccpn/ccpnv3/ccp/lims/Sample/default+default_user_2024-02-24-15-54-35-583_00002.xml` & `ccpn_project_checker-0.1.6/src/project_checker/test_data/delayed_errors/bad_role_exo_link_key_element_children.ccpn/ccpnv3/ccp/lims/Sample/default+default_user_2024-02-24-15-54-35-583_00002.xml`

 * *Files identical despite different names*

### Comparing `ccpn_project_checker-0.1.5/src/project_checker/test_data/delayed_errors/bad_role_exo_link_key_element_children.ccpn/ccpnv3/ccp/nmr/Nmr/default+default_user_2024-02-24-15-54-35-583_00001.xml` & `ccpn_project_checker-0.1.6/src/project_checker/test_data/delayed_errors/bad_role_exo_link_key_element_children.ccpn/ccpnv3/ccp/nmr/Nmr/default+default_user_2024-02-24-15-54-35-583_00001.xml`

 * *Files identical despite different names*

### Comparing `ccpn_project_checker-0.1.5/src/project_checker/test_data/delayed_errors/bad_role_exo_link_key_element_children.ccpn/ccpnv3/ccpnmr/gui/Task/user+View+default_user_2024-02-24-15-54-35-583_00006.xml` & `ccpn_project_checker-0.1.6/src/project_checker/test_data/delayed_errors/bad_role_exo_link_key_element_children.ccpn/ccpnv3/ccpnmr/gui/Task/user+View+default_user_2024-02-24-15-54-35-583_00006.xml`

 * *Files identical despite different names*

### Comparing `ccpn_project_checker-0.1.5/src/project_checker/test_data/delayed_errors/bad_role_exo_link_key_element_children.ccpn/ccpnv3/ccpnmr/gui/Window/_ccp_nmr_Nmr_NmrProject___default___+default_user_2024-02-24-15-54-35-583_00005.xml` & `ccpn_project_checker-0.1.6/src/project_checker/test_data/delayed_errors/bad_role_exo_link_key_element_children.ccpn/ccpnv3/ccpnmr/gui/Window/_ccp_nmr_Nmr_NmrProject___default___+default_user_2024-02-24-15-54-35-583_00005.xml`

 * *Files identical despite different names*

### Comparing `ccpn_project_checker-0.1.5/src/project_checker/test_data/delayed_errors/bad_role_exo_link_key_element_children.ccpn/ccpnv3/memops/Implementation/bad_role_exo_link_key_element_children.xml` & `ccpn_project_checker-0.1.6/src/project_checker/test_data/delayed_errors/bad_role_exo_link_key_element_children.ccpn/ccpnv3/memops/Implementation/bad_role_exo_link_key_element_children.xml`

 * *Files identical despite different names*

### Comparing `ccpn_project_checker-0.1.5/src/project_checker/test_data/delayed_errors/bad_role_exo_link_key_element_parent.ccpn/ccpnv3/ccp/lims/Sample/default+default_user_2024-02-24-15-54-35-583_00002.xml` & `ccpn_project_checker-0.1.6/src/project_checker/test_data/delayed_errors/bad_role_exo_link_key_element_parent.ccpn/ccpnv3/ccp/lims/Sample/default+default_user_2024-02-24-15-54-35-583_00002.xml`

 * *Files identical despite different names*

### Comparing `ccpn_project_checker-0.1.5/src/project_checker/test_data/delayed_errors/bad_role_exo_link_key_element_parent.ccpn/ccpnv3/ccp/nmr/Nmr/default+default_user_2024-02-24-15-54-35-583_00001.xml` & `ccpn_project_checker-0.1.6/src/project_checker/test_data/delayed_errors/bad_role_exo_link_key_element_parent.ccpn/ccpnv3/ccp/nmr/Nmr/default+default_user_2024-02-24-15-54-35-583_00001.xml`

 * *Files identical despite different names*

### Comparing `ccpn_project_checker-0.1.5/src/project_checker/test_data/delayed_errors/bad_role_exo_link_key_element_parent.ccpn/ccpnv3/ccpnmr/gui/Task/user+View+default_user_2024-02-24-15-54-35-583_00006.xml` & `ccpn_project_checker-0.1.6/src/project_checker/test_data/delayed_errors/bad_role_exo_link_key_element_parent.ccpn/ccpnv3/ccpnmr/gui/Task/user+View+default_user_2024-02-24-15-54-35-583_00006.xml`

 * *Files identical despite different names*

### Comparing `ccpn_project_checker-0.1.5/src/project_checker/test_data/delayed_errors/bad_role_exo_link_key_element_parent.ccpn/ccpnv3/ccpnmr/gui/Window/_ccp_nmr_Nmr_NmrProject___default___+default_user_2024-02-24-15-54-35-583_00005.xml` & `ccpn_project_checker-0.1.6/src/project_checker/test_data/delayed_errors/bad_role_exo_link_key_element_parent.ccpn/ccpnv3/ccpnmr/gui/Window/_ccp_nmr_Nmr_NmrProject___default___+default_user_2024-02-24-15-54-35-583_00005.xml`

 * *Files identical despite different names*

### Comparing `ccpn_project_checker-0.1.5/src/project_checker/test_data/delayed_errors/bad_role_exo_link_key_element_parent.ccpn/ccpnv3/memops/Implementation/bad_role_exo_link_key_element_parent.xml` & `ccpn_project_checker-0.1.6/src/project_checker/test_data/delayed_errors/bad_role_exo_link_key_element_parent.ccpn/ccpnv3/memops/Implementation/bad_role_exo_link_key_element_parent.xml`

 * *Files identical despite different names*

### Comparing `ccpn_project_checker-0.1.5/src/project_checker/test_data/delayed_errors/bad_root_exo_link_element.ccpn/ccpnv3/ccp/lims/Sample/default+default_user_2024-02-24-15-54-35-583_00002.xml` & `ccpn_project_checker-0.1.6/src/project_checker/test_data/delayed_errors/bad_root_exo_link_element.ccpn/ccpnv3/ccp/lims/Sample/default+default_user_2024-02-24-15-54-35-583_00002.xml`

 * *Files identical despite different names*

### Comparing `ccpn_project_checker-0.1.5/src/project_checker/test_data/delayed_errors/bad_root_exo_link_element.ccpn/ccpnv3/ccp/nmr/Nmr/default+default_user_2024-02-24-15-54-35-583_00001.xml` & `ccpn_project_checker-0.1.6/src/project_checker/test_data/delayed_errors/bad_root_exo_link_element.ccpn/ccpnv3/ccp/nmr/Nmr/default+default_user_2024-02-24-15-54-35-583_00001.xml`

 * *Files identical despite different names*

### Comparing `ccpn_project_checker-0.1.5/src/project_checker/test_data/delayed_errors/bad_root_exo_link_element.ccpn/ccpnv3/ccpnmr/gui/Task/user+View+default_user_2024-02-24-15-54-35-583_00006.xml` & `ccpn_project_checker-0.1.6/src/project_checker/test_data/delayed_errors/bad_root_exo_link_element.ccpn/ccpnv3/ccpnmr/gui/Task/user+View+default_user_2024-02-24-15-54-35-583_00006.xml`

 * *Files identical despite different names*

### Comparing `ccpn_project_checker-0.1.5/src/project_checker/test_data/delayed_errors/bad_root_exo_link_element.ccpn/ccpnv3/ccpnmr/gui/Window/_ccp_nmr_Nmr_NmrProject___default___+default_user_2024-02-24-15-54-35-583_00005.xml` & `ccpn_project_checker-0.1.6/src/project_checker/test_data/delayed_errors/bad_root_exo_link_element.ccpn/ccpnv3/ccpnmr/gui/Window/_ccp_nmr_Nmr_NmrProject___default___+default_user_2024-02-24-15-54-35-583_00005.xml`

 * *Files identical despite different names*

### Comparing `ccpn_project_checker-0.1.5/src/project_checker/test_data/delayed_errors/bad_root_exo_link_element.ccpn/ccpnv3/memops/Implementation/bad_root_exo_link_element.xml` & `ccpn_project_checker-0.1.6/src/project_checker/test_data/delayed_errors/bad_root_exo_link_element.ccpn/ccpnv3/memops/Implementation/bad_root_exo_link_element.xml`

 * *Files identical despite different names*

### Comparing `ccpn_project_checker-0.1.5/src/project_checker/test_data/delayed_errors/empty_good_project_with_non_ccpn_letter~.ccpn/ccpnv3/ccp/lims/Sample/default+default_user_2024-02-24-15-54-35-583_00002.xml` & `ccpn_project_checker-0.1.6/src/project_checker/test_data/delayed_errors/empty_good_project_with_non_ccpn_letter~.ccpn/ccpnv3/ccp/lims/Sample/default+default_user_2024-02-24-15-54-35-583_00002.xml`

 * *Files identical despite different names*

### Comparing `ccpn_project_checker-0.1.5/src/project_checker/test_data/delayed_errors/empty_good_project_with_non_ccpn_letter~.ccpn/ccpnv3/ccp/nmr/Nmr/default+default_user_2024-02-24-15-54-35-583_00001.xml` & `ccpn_project_checker-0.1.6/src/project_checker/test_data/delayed_errors/empty_good_project_with_non_ccpn_letter~.ccpn/ccpnv3/ccp/nmr/Nmr/default+default_user_2024-02-24-15-54-35-583_00001.xml`

 * *Files identical despite different names*

### Comparing `ccpn_project_checker-0.1.5/src/project_checker/test_data/delayed_errors/empty_good_project_with_non_ccpn_letter~.ccpn/ccpnv3/ccpnmr/gui/Task/user+View+default_user_2024-02-24-15-54-35-583_00006.xml` & `ccpn_project_checker-0.1.6/src/project_checker/test_data/delayed_errors/empty_good_project_with_non_ccpn_letter~.ccpn/ccpnv3/ccpnmr/gui/Task/user+View+default_user_2024-02-24-15-54-35-583_00006.xml`

 * *Files identical despite different names*

### Comparing `ccpn_project_checker-0.1.5/src/project_checker/test_data/delayed_errors/empty_good_project_with_non_ccpn_letter~.ccpn/ccpnv3/ccpnmr/gui/Window/_ccp_nmr_Nmr_NmrProject___default___+default_user_2024-02-24-15-54-35-583_00005.xml` & `ccpn_project_checker-0.1.6/src/project_checker/test_data/delayed_errors/empty_good_project_with_non_ccpn_letter~.ccpn/ccpnv3/ccpnmr/gui/Window/_ccp_nmr_Nmr_NmrProject___default___+default_user_2024-02-24-15-54-35-583_00005.xml`

 * *Files identical despite different names*

### Comparing `ccpn_project_checker-0.1.5/src/project_checker/test_data/delayed_errors/empty_good_project_with_non_ccpn_letter~.ccpn/ccpnv3/memops/Implementation/empty_good_project_with_non_ccpn_letter~.xml` & `ccpn_project_checker-0.1.6/src/project_checker/test_data/delayed_errors/empty_good_project_with_non_ccpn_letter~.ccpn/ccpnv3/memops/Implementation/empty_good_project_with_non_ccpn_letter~.xml`

 * *Files identical despite different names*

### Comparing `ccpn_project_checker-0.1.5/src/project_checker/test_data/delayed_errors/exo_file_bad_root_element_name.ccpn/ccpnv3/ccp/lims/Sample/default+default_user_2024-02-24-15-54-35-583_00002.xml` & `ccpn_project_checker-0.1.6/src/project_checker/test_data/delayed_errors/exo_file_bad_root_element_name.ccpn/ccpnv3/ccp/lims/Sample/default+default_user_2024-02-24-15-54-35-583_00002.xml`

 * *Files identical despite different names*

### Comparing `ccpn_project_checker-0.1.5/src/project_checker/test_data/delayed_errors/exo_file_bad_root_element_name.ccpn/ccpnv3/ccp/nmr/Nmr/default+default_user_2024-02-24-15-54-35-583_00001.xml` & `ccpn_project_checker-0.1.6/src/project_checker/test_data/delayed_errors/exo_file_bad_root_element_name.ccpn/ccpnv3/ccp/nmr/Nmr/default+default_user_2024-02-24-15-54-35-583_00001.xml`

 * *Files identical despite different names*

### Comparing `ccpn_project_checker-0.1.5/src/project_checker/test_data/delayed_errors/exo_file_bad_root_element_name.ccpn/ccpnv3/ccpnmr/gui/Task/user+View+default_user_2024-02-24-15-54-35-583_00006.xml` & `ccpn_project_checker-0.1.6/src/project_checker/test_data/delayed_errors/exo_file_bad_root_element_name.ccpn/ccpnv3/ccpnmr/gui/Task/user+View+default_user_2024-02-24-15-54-35-583_00006.xml`

 * *Files identical despite different names*

### Comparing `ccpn_project_checker-0.1.5/src/project_checker/test_data/delayed_errors/exo_file_bad_root_element_name.ccpn/ccpnv3/ccpnmr/gui/Window/_ccp_nmr_Nmr_NmrProject___default___+default_user_2024-02-24-15-54-35-583_00005.xml` & `ccpn_project_checker-0.1.6/src/project_checker/test_data/delayed_errors/exo_file_bad_root_element_name.ccpn/ccpnv3/ccpnmr/gui/Window/_ccp_nmr_Nmr_NmrProject___default___+default_user_2024-02-24-15-54-35-583_00005.xml`

 * *Files identical despite different names*

### Comparing `ccpn_project_checker-0.1.5/src/project_checker/test_data/delayed_errors/exo_file_bad_root_element_name.ccpn/ccpnv3/memops/Implementation/exo_file_bad_root_element_name.xml` & `ccpn_project_checker-0.1.6/src/project_checker/test_data/delayed_errors/exo_file_bad_root_element_name.ccpn/ccpnv3/memops/Implementation/exo_file_bad_root_element_name.xml`

 * *Files identical despite different names*

### Comparing `ccpn_project_checker-0.1.5/src/project_checker/test_data/delayed_errors/exo_file_key_doesnt_match_root.ccpn/ccpnv3/ccp/lims/Sample/default+default_user_2024-02-24-15-54-35-583_00002.xml` & `ccpn_project_checker-0.1.6/src/project_checker/test_data/delayed_errors/exo_file_key_doesnt_match_root.ccpn/ccpnv3/ccp/lims/Sample/default+default_user_2024-02-24-15-54-35-583_00002.xml`

 * *Files identical despite different names*

### Comparing `ccpn_project_checker-0.1.5/src/project_checker/test_data/delayed_errors/exo_file_key_doesnt_match_root.ccpn/ccpnv3/ccp/nmr/Nmr/default+default_user_2024-02-24-15-54-35-583_00001.xml` & `ccpn_project_checker-0.1.6/src/project_checker/test_data/delayed_errors/exo_file_key_doesnt_match_root.ccpn/ccpnv3/ccp/nmr/Nmr/default+default_user_2024-02-24-15-54-35-583_00001.xml`

 * *Files identical despite different names*

### Comparing `ccpn_project_checker-0.1.5/src/project_checker/test_data/delayed_errors/exo_file_key_doesnt_match_root.ccpn/ccpnv3/ccpnmr/gui/Task/user+View+default_user_2024-02-24-15-54-35-583_00006.xml` & `ccpn_project_checker-0.1.6/src/project_checker/test_data/delayed_errors/exo_file_key_doesnt_match_root.ccpn/ccpnv3/ccpnmr/gui/Task/user+View+default_user_2024-02-24-15-54-35-583_00006.xml`

 * *Files identical despite different names*

### Comparing `ccpn_project_checker-0.1.5/src/project_checker/test_data/delayed_errors/exo_file_key_doesnt_match_root.ccpn/ccpnv3/ccpnmr/gui/Window/_ccp_nmr_Nmr_NmrProject___default___+default_user_2024-02-24-15-54-35-583_00005.xml` & `ccpn_project_checker-0.1.6/src/project_checker/test_data/delayed_errors/exo_file_key_doesnt_match_root.ccpn/ccpnv3/ccpnmr/gui/Window/_ccp_nmr_Nmr_NmrProject___default___+default_user_2024-02-24-15-54-35-583_00005.xml`

 * *Files identical despite different names*

### Comparing `ccpn_project_checker-0.1.5/src/project_checker/test_data/delayed_errors/exo_file_key_doesnt_match_root.ccpn/ccpnv3/memops/Implementation/exo_file_key_doesnt_match_root.xml` & `ccpn_project_checker-0.1.6/src/project_checker/test_data/delayed_errors/exo_file_key_doesnt_match_root.ccpn/ccpnv3/memops/Implementation/exo_file_key_doesnt_match_root.xml`

 * *Files identical despite different names*

### Comparing `ccpn_project_checker-0.1.5/src/project_checker/test_data/delayed_errors/exo_file_no_package_guid.ccpn/ccpnv3/ccp/lims/Sample/default+default_user_2024-02-24-15-54-35-583_00002.xml` & `ccpn_project_checker-0.1.6/src/project_checker/test_data/delayed_errors/exo_file_no_package_guid.ccpn/ccpnv3/ccp/lims/Sample/default+default_user_2024-02-24-15-54-35-583_00002.xml`

 * *Files identical despite different names*

### Comparing `ccpn_project_checker-0.1.5/src/project_checker/test_data/delayed_errors/exo_file_no_package_guid.ccpn/ccpnv3/ccp/nmr/Nmr/default+default_user_2024-02-24-15-54-35-583_00001.xml` & `ccpn_project_checker-0.1.6/src/project_checker/test_data/delayed_errors/exo_file_no_package_guid.ccpn/ccpnv3/ccp/nmr/Nmr/default+default_user_2024-02-24-15-54-35-583_00001.xml`

 * *Files identical despite different names*

### Comparing `ccpn_project_checker-0.1.5/src/project_checker/test_data/delayed_errors/exo_file_no_package_guid.ccpn/ccpnv3/ccpnmr/gui/Task/user+View+default_user_2024-02-24-15-54-35-583_00006.xml` & `ccpn_project_checker-0.1.6/src/project_checker/test_data/delayed_errors/exo_file_no_package_guid.ccpn/ccpnv3/ccpnmr/gui/Task/user+View+default_user_2024-02-24-15-54-35-583_00006.xml`

 * *Files identical despite different names*

### Comparing `ccpn_project_checker-0.1.5/src/project_checker/test_data/delayed_errors/exo_file_no_package_guid.ccpn/ccpnv3/ccpnmr/gui/Window/_ccp_nmr_Nmr_NmrProject___default___+default_user_2024-02-24-15-54-35-583_00005.xml` & `ccpn_project_checker-0.1.6/src/project_checker/test_data/delayed_errors/exo_file_no_package_guid.ccpn/ccpnv3/ccpnmr/gui/Window/_ccp_nmr_Nmr_NmrProject___default___+default_user_2024-02-24-15-54-35-583_00005.xml`

 * *Files identical despite different names*

### Comparing `ccpn_project_checker-0.1.5/src/project_checker/test_data/delayed_errors/exo_file_no_package_guid.ccpn/ccpnv3/memops/Implementation/exo_file_no_package_guid.xml` & `ccpn_project_checker-0.1.6/src/project_checker/test_data/delayed_errors/exo_file_no_package_guid.ccpn/ccpnv3/memops/Implementation/exo_file_no_package_guid.xml`

 * *Files identical despite different names*

### Comparing `ccpn_project_checker-0.1.5/src/project_checker/test_data/delayed_errors/exo_file_release_attrib_invalid.ccpn/ccpnv3/ccp/lims/Sample/default+default_user_2024-02-24-15-54-35-583_00002.xml` & `ccpn_project_checker-0.1.6/src/project_checker/test_data/delayed_errors/exo_file_release_attrib_invalid.ccpn/ccpnv3/ccp/lims/Sample/default+default_user_2024-02-24-15-54-35-583_00002.xml`

 * *Files identical despite different names*

### Comparing `ccpn_project_checker-0.1.5/src/project_checker/test_data/delayed_errors/exo_file_release_attrib_invalid.ccpn/ccpnv3/ccp/nmr/Nmr/default+default_user_2024-02-24-15-54-35-583_00001.xml` & `ccpn_project_checker-0.1.6/src/project_checker/test_data/delayed_errors/exo_file_release_attrib_invalid.ccpn/ccpnv3/ccp/nmr/Nmr/default+default_user_2024-02-24-15-54-35-583_00001.xml`

 * *Files identical despite different names*

### Comparing `ccpn_project_checker-0.1.5/src/project_checker/test_data/delayed_errors/exo_file_release_attrib_invalid.ccpn/ccpnv3/ccpnmr/gui/Task/user+View+default_user_2024-02-24-15-54-35-583_00006.xml` & `ccpn_project_checker-0.1.6/src/project_checker/test_data/delayed_errors/exo_file_release_attrib_invalid.ccpn/ccpnv3/ccpnmr/gui/Task/user+View+default_user_2024-02-24-15-54-35-583_00006.xml`

 * *Files identical despite different names*

### Comparing `ccpn_project_checker-0.1.5/src/project_checker/test_data/delayed_errors/exo_file_release_attrib_invalid.ccpn/ccpnv3/ccpnmr/gui/Window/_ccp_nmr_Nmr_NmrProject___default___+default_user_2024-02-24-15-54-35-583_00005.xml` & `ccpn_project_checker-0.1.6/src/project_checker/test_data/delayed_errors/exo_file_release_attrib_invalid.ccpn/ccpnv3/ccpnmr/gui/Window/_ccp_nmr_Nmr_NmrProject___default___+default_user_2024-02-24-15-54-35-583_00005.xml`

 * *Files identical despite different names*

### Comparing `ccpn_project_checker-0.1.5/src/project_checker/test_data/delayed_errors/exo_file_release_attrib_invalid.ccpn/ccpnv3/memops/Implementation/exo_file_release_attrib_invalid.xml` & `ccpn_project_checker-0.1.6/src/project_checker/test_data/delayed_errors/exo_file_release_attrib_invalid.ccpn/ccpnv3/memops/Implementation/exo_file_release_attrib_invalid.xml`

 * *Files identical despite different names*

### Comparing `ccpn_project_checker-0.1.5/src/project_checker/test_data/delayed_errors/exo_file_release_attrib_missing.ccpn/ccpnv3/ccp/lims/Sample/default+default_user_2024-02-24-15-54-35-583_00002.xml` & `ccpn_project_checker-0.1.6/src/project_checker/test_data/delayed_errors/exo_file_release_attrib_missing.ccpn/ccpnv3/ccp/lims/Sample/default+default_user_2024-02-24-15-54-35-583_00002.xml`

 * *Files identical despite different names*

### Comparing `ccpn_project_checker-0.1.5/src/project_checker/test_data/delayed_errors/exo_file_release_attrib_missing.ccpn/ccpnv3/ccp/nmr/Nmr/default+default_user_2024-02-24-15-54-35-583_00001.xml` & `ccpn_project_checker-0.1.6/src/project_checker/test_data/delayed_errors/exo_file_release_attrib_missing.ccpn/ccpnv3/ccp/nmr/Nmr/default+default_user_2024-02-24-15-54-35-583_00001.xml`

 * *Files identical despite different names*

### Comparing `ccpn_project_checker-0.1.5/src/project_checker/test_data/delayed_errors/exo_file_release_attrib_missing.ccpn/ccpnv3/ccpnmr/gui/Task/user+View+default_user_2024-02-24-15-54-35-583_00006.xml` & `ccpn_project_checker-0.1.6/src/project_checker/test_data/delayed_errors/exo_file_release_attrib_missing.ccpn/ccpnv3/ccpnmr/gui/Task/user+View+default_user_2024-02-24-15-54-35-583_00006.xml`

 * *Files identical despite different names*

### Comparing `ccpn_project_checker-0.1.5/src/project_checker/test_data/delayed_errors/exo_file_release_attrib_missing.ccpn/ccpnv3/ccpnmr/gui/Window/_ccp_nmr_Nmr_NmrProject___default___+default_user_2024-02-24-15-54-35-583_00005.xml` & `ccpn_project_checker-0.1.6/src/project_checker/test_data/delayed_errors/exo_file_release_attrib_missing.ccpn/ccpnv3/ccpnmr/gui/Window/_ccp_nmr_Nmr_NmrProject___default___+default_user_2024-02-24-15-54-35-583_00005.xml`

 * *Files identical despite different names*

### Comparing `ccpn_project_checker-0.1.5/src/project_checker/test_data/delayed_errors/exo_file_release_attrib_missing.ccpn/ccpnv3/memops/Implementation/exo_file_release_attrib_missing.xml` & `ccpn_project_checker-0.1.6/src/project_checker/test_data/delayed_errors/exo_file_release_attrib_missing.ccpn/ccpnv3/memops/Implementation/exo_file_release_attrib_missing.xml`

 * *Files identical despite different names*

### Comparing `ccpn_project_checker-0.1.5/src/project_checker/test_data/delayed_errors/exo_file_release_doesnt_match_root.ccpn/ccpnv3/ccp/lims/Sample/default+default_user_2024-02-24-15-54-35-583_00002.xml` & `ccpn_project_checker-0.1.6/src/project_checker/test_data/delayed_errors/exo_file_release_doesnt_match_root.ccpn/ccpnv3/ccp/lims/Sample/default+default_user_2024-02-24-15-54-35-583_00002.xml`

 * *Files identical despite different names*

### Comparing `ccpn_project_checker-0.1.5/src/project_checker/test_data/delayed_errors/exo_file_release_doesnt_match_root.ccpn/ccpnv3/ccp/nmr/Nmr/default+default_user_2024-02-24-15-54-35-583_00001.xml` & `ccpn_project_checker-0.1.6/src/project_checker/test_data/delayed_errors/exo_file_release_doesnt_match_root.ccpn/ccpnv3/ccp/nmr/Nmr/default+default_user_2024-02-24-15-54-35-583_00001.xml`

 * *Files identical despite different names*

### Comparing `ccpn_project_checker-0.1.5/src/project_checker/test_data/delayed_errors/exo_file_release_doesnt_match_root.ccpn/ccpnv3/ccpnmr/gui/Task/user+View+default_user_2024-02-24-15-54-35-583_00006.xml` & `ccpn_project_checker-0.1.6/src/project_checker/test_data/delayed_errors/exo_file_release_doesnt_match_root.ccpn/ccpnv3/ccpnmr/gui/Task/user+View+default_user_2024-02-24-15-54-35-583_00006.xml`

 * *Files identical despite different names*

### Comparing `ccpn_project_checker-0.1.5/src/project_checker/test_data/delayed_errors/exo_file_release_doesnt_match_root.ccpn/ccpnv3/ccpnmr/gui/Window/_ccp_nmr_Nmr_NmrProject___default___+default_user_2024-02-24-15-54-35-583_00005.xml` & `ccpn_project_checker-0.1.6/src/project_checker/test_data/delayed_errors/exo_file_release_doesnt_match_root.ccpn/ccpnv3/ccpnmr/gui/Window/_ccp_nmr_Nmr_NmrProject___default___+default_user_2024-02-24-15-54-35-583_00005.xml`

 * *Files identical despite different names*

### Comparing `ccpn_project_checker-0.1.5/src/project_checker/test_data/delayed_errors/exo_file_release_doesnt_match_root.ccpn/ccpnv3/memops/Implementation/exo_file_release_doesnt_match_root.xml` & `ccpn_project_checker-0.1.6/src/project_checker/test_data/delayed_errors/exo_file_release_doesnt_match_root.ccpn/ccpnv3/memops/Implementation/exo_file_release_doesnt_match_root.xml`

 * *Files identical despite different names*

### Comparing `ccpn_project_checker-0.1.5/src/project_checker/test_data/delayed_errors/exo_file_short_name_guid_doesnt_match_package_guid.ccpn/ccpnv3/ccp/lims/Sample/default+default_user_2024-02-24-15-54-35-583_00002.xml` & `ccpn_project_checker-0.1.6/src/project_checker/test_data/delayed_errors/exo_file_short_name_guid_doesnt_match_package_guid.ccpn/ccpnv3/ccp/lims/Sample/default+default_user_2024-02-24-15-54-35-583_00002.xml`

 * *Files identical despite different names*

### Comparing `ccpn_project_checker-0.1.5/src/project_checker/test_data/delayed_errors/exo_file_short_name_guid_doesnt_match_package_guid.ccpn/ccpnv3/ccp/nmr/Nmr/default+default_user_2024-02-24-15-54-35-583_00001.xml` & `ccpn_project_checker-0.1.6/src/project_checker/test_data/delayed_errors/exo_file_short_name_guid_doesnt_match_package_guid.ccpn/ccpnv3/ccp/nmr/Nmr/default+default_user_2024-02-24-15-54-35-583_00001.xml`

 * *Files identical despite different names*

### Comparing `ccpn_project_checker-0.1.5/src/project_checker/test_data/delayed_errors/exo_file_short_name_guid_doesnt_match_package_guid.ccpn/ccpnv3/ccpnmr/gui/Task/user+View+default_user_2024-02-24-15-54-35-583_00006.xml` & `ccpn_project_checker-0.1.6/src/project_checker/test_data/delayed_errors/exo_file_short_name_guid_doesnt_match_package_guid.ccpn/ccpnv3/ccpnmr/gui/Task/user+View+default_user_2024-02-24-15-54-35-583_00006.xml`

 * *Files identical despite different names*

### Comparing `ccpn_project_checker-0.1.5/src/project_checker/test_data/delayed_errors/exo_file_short_name_guid_doesnt_match_package_guid.ccpn/ccpnv3/ccpnmr/gui/Window/_ccp_nmr_Nmr_NmrProject___default___+default_user_2024-02-24-15-54-35-583_00005.xml` & `ccpn_project_checker-0.1.6/src/project_checker/test_data/delayed_errors/exo_file_short_name_guid_doesnt_match_package_guid.ccpn/ccpnv3/ccpnmr/gui/Window/_ccp_nmr_Nmr_NmrProject___default___+default_user_2024-02-24-15-54-35-583_00005.xml`

 * *Files identical despite different names*

### Comparing `ccpn_project_checker-0.1.5/src/project_checker/test_data/delayed_errors/exo_file_short_name_guid_doesnt_match_package_guid.ccpn/ccpnv3/memops/Implementation/exo_file_short_name_guid_doesnt_match_package_guid.xml` & `ccpn_project_checker-0.1.6/src/project_checker/test_data/delayed_errors/exo_file_short_name_guid_doesnt_match_package_guid.ccpn/ccpnv3/memops/Implementation/exo_file_short_name_guid_doesnt_match_package_guid.xml`

 * *Files identical despite different names*

### Comparing `ccpn_project_checker-0.1.5/src/project_checker/test_data/delayed_errors/exo_file_time_attrib_invalid.ccpn/ccpnv3/ccp/lims/Sample/default+default_user_2024-02-24-15-54-35-583_00002.xml` & `ccpn_project_checker-0.1.6/src/project_checker/test_data/delayed_errors/exo_file_time_attrib_invalid.ccpn/ccpnv3/ccp/lims/Sample/default+default_user_2024-02-24-15-54-35-583_00002.xml`

 * *Files identical despite different names*

### Comparing `ccpn_project_checker-0.1.5/src/project_checker/test_data/delayed_errors/exo_file_time_attrib_invalid.ccpn/ccpnv3/ccp/nmr/Nmr/default+default_user_2024-02-24-15-54-35-583_00001.xml` & `ccpn_project_checker-0.1.6/src/project_checker/test_data/delayed_errors/exo_file_time_attrib_invalid.ccpn/ccpnv3/ccp/nmr/Nmr/default+default_user_2024-02-24-15-54-35-583_00001.xml`

 * *Files identical despite different names*

### Comparing `ccpn_project_checker-0.1.5/src/project_checker/test_data/delayed_errors/exo_file_time_attrib_invalid.ccpn/ccpnv3/ccpnmr/gui/Task/user+View+default_user_2024-02-24-15-54-35-583_00006.xml` & `ccpn_project_checker-0.1.6/src/project_checker/test_data/delayed_errors/exo_file_time_attrib_invalid.ccpn/ccpnv3/ccpnmr/gui/Task/user+View+default_user_2024-02-24-15-54-35-583_00006.xml`

 * *Files identical despite different names*

### Comparing `ccpn_project_checker-0.1.5/src/project_checker/test_data/delayed_errors/exo_file_time_attrib_invalid.ccpn/ccpnv3/ccpnmr/gui/Window/_ccp_nmr_Nmr_NmrProject___default___+default_user_2024-02-24-15-54-35-583_00005.xml` & `ccpn_project_checker-0.1.6/src/project_checker/test_data/delayed_errors/exo_file_time_attrib_invalid.ccpn/ccpnv3/ccpnmr/gui/Window/_ccp_nmr_Nmr_NmrProject___default___+default_user_2024-02-24-15-54-35-583_00005.xml`

 * *Files identical despite different names*

### Comparing `ccpn_project_checker-0.1.5/src/project_checker/test_data/delayed_errors/exo_file_time_attrib_invalid.ccpn/ccpnv3/memops/Implementation/exo_file_time_attrib_invalid.xml` & `ccpn_project_checker-0.1.6/src/project_checker/test_data/delayed_errors/exo_file_time_attrib_invalid.ccpn/ccpnv3/memops/Implementation/exo_file_time_attrib_invalid.xml`

 * *Files identical despite different names*

### Comparing `ccpn_project_checker-0.1.5/src/project_checker/test_data/delayed_errors/exo_file_time_attrib_missing.ccpn/ccpnv3/ccp/lims/Sample/default+default_user_2024-02-24-15-54-35-583_00002.xml` & `ccpn_project_checker-0.1.6/src/project_checker/test_data/delayed_errors/exo_file_time_attrib_missing.ccpn/ccpnv3/ccp/lims/Sample/default+default_user_2024-02-24-15-54-35-583_00002.xml`

 * *Files identical despite different names*

### Comparing `ccpn_project_checker-0.1.5/src/project_checker/test_data/delayed_errors/exo_file_time_attrib_missing.ccpn/ccpnv3/ccp/nmr/Nmr/default+default_user_2024-02-24-15-54-35-583_00001.xml` & `ccpn_project_checker-0.1.6/src/project_checker/test_data/delayed_errors/exo_file_time_attrib_missing.ccpn/ccpnv3/ccp/nmr/Nmr/default+default_user_2024-02-24-15-54-35-583_00001.xml`

 * *Files identical despite different names*

### Comparing `ccpn_project_checker-0.1.5/src/project_checker/test_data/delayed_errors/exo_file_time_attrib_missing.ccpn/ccpnv3/ccpnmr/gui/Task/user+View+default_user_2024-02-24-15-54-35-583_00006.xml` & `ccpn_project_checker-0.1.6/src/project_checker/test_data/delayed_errors/exo_file_time_attrib_missing.ccpn/ccpnv3/ccpnmr/gui/Task/user+View+default_user_2024-02-24-15-54-35-583_00006.xml`

 * *Files identical despite different names*

### Comparing `ccpn_project_checker-0.1.5/src/project_checker/test_data/delayed_errors/exo_file_time_attrib_missing.ccpn/ccpnv3/ccpnmr/gui/Window/_ccp_nmr_Nmr_NmrProject___default___+default_user_2024-02-24-15-54-35-583_00005.xml` & `ccpn_project_checker-0.1.6/src/project_checker/test_data/delayed_errors/exo_file_time_attrib_missing.ccpn/ccpnv3/ccpnmr/gui/Window/_ccp_nmr_Nmr_NmrProject___default___+default_user_2024-02-24-15-54-35-583_00005.xml`

 * *Files identical despite different names*

### Comparing `ccpn_project_checker-0.1.5/src/project_checker/test_data/delayed_errors/exo_file_time_attrib_missing.ccpn/ccpnv3/memops/Implementation/exo_file_time_attrib_missing.xml` & `ccpn_project_checker-0.1.6/src/project_checker/test_data/delayed_errors/exo_file_time_attrib_missing.ccpn/ccpnv3/memops/Implementation/exo_file_time_attrib_missing.xml`

 * *Files identical despite different names*

### Comparing `ccpn_project_checker-0.1.5/src/project_checker/test_data/delayed_errors/exo_file_unknown_package_guid.ccpn/ccpnv3/ccp/lims/Sample/default+default_user_2024-02-24-15-54-35-583_00002.xml` & `ccpn_project_checker-0.1.6/src/project_checker/test_data/delayed_errors/exo_file_unknown_package_guid.ccpn/ccpnv3/ccp/lims/Sample/default+default_user_2024-02-24-15-54-35-583_00002.xml`

 * *Files identical despite different names*

### Comparing `ccpn_project_checker-0.1.5/src/project_checker/test_data/delayed_errors/exo_file_unknown_package_guid.ccpn/ccpnv3/ccp/nmr/Nmr/default+default_user_2024-02-24-15-54-35-583_00001.xml` & `ccpn_project_checker-0.1.6/src/project_checker/test_data/delayed_errors/exo_file_unknown_package_guid.ccpn/ccpnv3/ccp/nmr/Nmr/default+default_user_2024-02-24-15-54-35-583_00001.xml`

 * *Files identical despite different names*

### Comparing `ccpn_project_checker-0.1.5/src/project_checker/test_data/delayed_errors/exo_file_unknown_package_guid.ccpn/ccpnv3/ccpnmr/gui/Task/user+View+default_user_2024-02-24-15-54-35-583_00006.xml` & `ccpn_project_checker-0.1.6/src/project_checker/test_data/delayed_errors/exo_file_unknown_package_guid.ccpn/ccpnv3/ccpnmr/gui/Task/user+View+default_user_2024-02-24-15-54-35-583_00006.xml`

 * *Files identical despite different names*

### Comparing `ccpn_project_checker-0.1.5/src/project_checker/test_data/delayed_errors/exo_file_unknown_package_guid.ccpn/ccpnv3/ccpnmr/gui/Window/_ccp_nmr_Nmr_NmrProject___default___+default_user_2024-02-24-15-54-35-583_00005.xml` & `ccpn_project_checker-0.1.6/src/project_checker/test_data/delayed_errors/exo_file_unknown_package_guid.ccpn/ccpnv3/ccpnmr/gui/Window/_ccp_nmr_Nmr_NmrProject___default___+default_user_2024-02-24-15-54-35-583_00005.xml`

 * *Files identical despite different names*

### Comparing `ccpn_project_checker-0.1.5/src/project_checker/test_data/delayed_errors/exo_file_unknown_package_guid.ccpn/ccpnv3/memops/Implementation/exo_file_unknown_package_guid.xml` & `ccpn_project_checker-0.1.6/src/project_checker/test_data/delayed_errors/exo_file_unknown_package_guid.ccpn/ccpnv3/memops/Implementation/exo_file_unknown_package_guid.xml`

 * *Files identical despite different names*

### Comparing `ccpn_project_checker-0.1.5/src/project_checker/test_data/delayed_errors/exo_file_unknown_short_package_name.ccpn/ccpnv3/ccp/lims/Sample/default+default_user_2024-02-24-15-54-35-583_00002.xml` & `ccpn_project_checker-0.1.6/src/project_checker/test_data/delayed_errors/exo_file_unknown_short_package_name.ccpn/ccpnv3/ccp/lims/Sample/default+default_user_2024-02-24-15-54-35-583_00002.xml`

 * *Files identical despite different names*

### Comparing `ccpn_project_checker-0.1.5/src/project_checker/test_data/delayed_errors/exo_file_unknown_short_package_name.ccpn/ccpnv3/ccp/nmr/Nmr/default+default_user_2024-02-24-15-54-35-583_00001.xml` & `ccpn_project_checker-0.1.6/src/project_checker/test_data/delayed_errors/exo_file_unknown_short_package_name.ccpn/ccpnv3/ccp/nmr/Nmr/default+default_user_2024-02-24-15-54-35-583_00001.xml`

 * *Files identical despite different names*

### Comparing `ccpn_project_checker-0.1.5/src/project_checker/test_data/delayed_errors/exo_file_unknown_short_package_name.ccpn/ccpnv3/ccpnmr/gui/Task/user+View+default_user_2024-02-24-15-54-35-583_00006.xml` & `ccpn_project_checker-0.1.6/src/project_checker/test_data/delayed_errors/exo_file_unknown_short_package_name.ccpn/ccpnv3/ccpnmr/gui/Task/user+View+default_user_2024-02-24-15-54-35-583_00006.xml`

 * *Files identical despite different names*

### Comparing `ccpn_project_checker-0.1.5/src/project_checker/test_data/delayed_errors/exo_file_unknown_short_package_name.ccpn/ccpnv3/ccpnmr/gui/Window/_ccp_nmr_Nmr_NmrProject___default___+default_user_2024-02-24-15-54-35-583_00005.xml` & `ccpn_project_checker-0.1.6/src/project_checker/test_data/delayed_errors/exo_file_unknown_short_package_name.ccpn/ccpnv3/ccpnmr/gui/Window/_ccp_nmr_Nmr_NmrProject___default___+default_user_2024-02-24-15-54-35-583_00005.xml`

 * *Files identical despite different names*

### Comparing `ccpn_project_checker-0.1.5/src/project_checker/test_data/delayed_errors/exo_file_unknown_short_package_name.ccpn/ccpnv3/memops/Implementation/exo_file_unknown_short_package_name.xml` & `ccpn_project_checker-0.1.6/src/project_checker/test_data/delayed_errors/exo_file_unknown_short_package_name.ccpn/ccpnv3/memops/Implementation/exo_file_unknown_short_package_name.xml`

 * *Files identical despite different names*

### Comparing `ccpn_project_checker-0.1.5/src/project_checker/test_data/delayed_errors/exo_file_wrong_storage_location.ccpn/ccpnv3/ccp/lims/Sample/default+default_user_2024-02-24-15-54-35-583_00002.xml` & `ccpn_project_checker-0.1.6/src/project_checker/test_data/delayed_errors/exo_file_wrong_storage_location.ccpn/ccpnv3/ccp/lims/Sample/default+default_user_2024-02-24-15-54-35-583_00002.xml`

 * *Files identical despite different names*

### Comparing `ccpn_project_checker-0.1.5/src/project_checker/test_data/delayed_errors/exo_file_wrong_storage_location.ccpn/ccpnv3/ccp/nmr/Nmr/default+default_user_2024-02-24-15-54-35-583_00001.xml` & `ccpn_project_checker-0.1.6/src/project_checker/test_data/delayed_errors/exo_file_wrong_storage_location.ccpn/ccpnv3/ccp/nmr/Nmr/default+default_user_2024-02-24-15-54-35-583_00001.xml`

 * *Files identical despite different names*

### Comparing `ccpn_project_checker-0.1.5/src/project_checker/test_data/delayed_errors/exo_file_wrong_storage_location.ccpn/ccpnv3/ccpnmr/gui/Task/user+View+default_user_2024-02-24-15-54-35-583_00006.xml` & `ccpn_project_checker-0.1.6/src/project_checker/test_data/delayed_errors/exo_file_wrong_storage_location.ccpn/ccpnv3/ccpnmr/gui/Task/user+View+default_user_2024-02-24-15-54-35-583_00006.xml`

 * *Files identical despite different names*

### Comparing `ccpn_project_checker-0.1.5/src/project_checker/test_data/delayed_errors/exo_file_wrong_storage_location.ccpn/ccpnv3/ccpnmr/gui/Window/_ccp_nmr_Nmr_NmrProject___default___+default_user_2024-02-24-15-54-35-583_00005.xml` & `ccpn_project_checker-0.1.6/src/project_checker/test_data/delayed_errors/exo_file_wrong_storage_location.ccpn/ccpnv3/ccpnmr/gui/Window/_ccp_nmr_Nmr_NmrProject___default___+default_user_2024-02-24-15-54-35-583_00005.xml`

 * *Files identical despite different names*

### Comparing `ccpn_project_checker-0.1.5/src/project_checker/test_data/delayed_errors/exo_file_wrong_storage_location.ccpn/ccpnv3/memops/Implementation/exo_file_wrong_storage_location.xml` & `ccpn_project_checker-0.1.6/src/project_checker/test_data/delayed_errors/exo_file_wrong_storage_location.ccpn/ccpnv3/memops/Implementation/exo_file_wrong_storage_location.xml`

 * *Files identical despite different names*

### Comparing `ccpn_project_checker-0.1.5/src/project_checker/test_data/delayed_errors/exo_link_no_top_object.ccpn/ccpnv3/ccp/lims/Sample/default+default_user_2024-02-24-15-54-35-583_00002.xml` & `ccpn_project_checker-0.1.6/src/project_checker/test_data/delayed_errors/exo_link_no_top_object.ccpn/ccpnv3/ccp/lims/Sample/default+default_user_2024-02-24-15-54-35-583_00002.xml`

 * *Files identical despite different names*

### Comparing `ccpn_project_checker-0.1.5/src/project_checker/test_data/delayed_errors/exo_link_no_top_object.ccpn/ccpnv3/ccp/nmr/Nmr/default+default_user_2024-02-24-15-54-35-583_00001.xml` & `ccpn_project_checker-0.1.6/src/project_checker/test_data/delayed_errors/exo_link_no_top_object.ccpn/ccpnv3/ccp/nmr/Nmr/default+default_user_2024-02-24-15-54-35-583_00001.xml`

 * *Files identical despite different names*

### Comparing `ccpn_project_checker-0.1.5/src/project_checker/test_data/delayed_errors/exo_link_no_top_object.ccpn/ccpnv3/ccpnmr/gui/Task/user+View+default_user_2024-02-24-15-54-35-583_00006.xml` & `ccpn_project_checker-0.1.6/src/project_checker/test_data/delayed_errors/exo_link_no_top_object.ccpn/ccpnv3/ccpnmr/gui/Task/user+View+default_user_2024-02-24-15-54-35-583_00006.xml`

 * *Files identical despite different names*

### Comparing `ccpn_project_checker-0.1.5/src/project_checker/test_data/delayed_errors/exo_link_no_top_object.ccpn/ccpnv3/ccpnmr/gui/Window/_ccp_nmr_Nmr_NmrProject___default___+default_user_2024-02-24-15-54-35-583_00005.xml` & `ccpn_project_checker-0.1.6/src/project_checker/test_data/delayed_errors/exo_link_no_top_object.ccpn/ccpnv3/ccpnmr/gui/Window/_ccp_nmr_Nmr_NmrProject___default___+default_user_2024-02-24-15-54-35-583_00005.xml`

 * *Files identical despite different names*

### Comparing `ccpn_project_checker-0.1.5/src/project_checker/test_data/delayed_errors/exo_link_no_top_object.ccpn/ccpnv3/memops/Implementation/exo_link_no_top_object.xml` & `ccpn_project_checker-0.1.6/src/project_checker/test_data/delayed_errors/exo_link_no_top_object.ccpn/ccpnv3/memops/Implementation/exo_link_no_top_object.xml`

 * *Files identical despite different names*

### Comparing `ccpn_project_checker-0.1.5/src/project_checker/test_data/delayed_errors/exo_link_too_many_top_objects.ccpn/ccpnv3/ccp/lims/Sample/default+default_user_2024-02-24-15-54-35-583_00002.xml` & `ccpn_project_checker-0.1.6/src/project_checker/test_data/delayed_errors/exo_link_too_many_top_objects.ccpn/ccpnv3/ccp/lims/Sample/default+default_user_2024-02-24-15-54-35-583_00002.xml`

 * *Files identical despite different names*

### Comparing `ccpn_project_checker-0.1.5/src/project_checker/test_data/delayed_errors/exo_link_too_many_top_objects.ccpn/ccpnv3/ccp/molecule/MolSystem/default+default_user_2024-02-24-15-54-35-583_00004.xml` & `ccpn_project_checker-0.1.6/src/project_checker/test_data/delayed_errors/exo_link_too_many_top_objects.ccpn/ccpnv3/ccp/molecule/MolSystem/default+default_user_2024-02-24-15-54-35-583_00004.xml`

 * *Files identical despite different names*

### Comparing `ccpn_project_checker-0.1.5/src/project_checker/test_data/delayed_errors/exo_link_too_many_top_objects.ccpn/ccpnv3/ccp/nmr/Nmr/default+default_user_2024-02-24-15-54-35-583_00001.xml` & `ccpn_project_checker-0.1.6/src/project_checker/test_data/delayed_errors/exo_link_too_many_top_objects.ccpn/ccpnv3/ccp/nmr/Nmr/default+default_user_2024-02-24-15-54-35-583_00001.xml`

 * *Files identical despite different names*

### Comparing `ccpn_project_checker-0.1.5/src/project_checker/test_data/delayed_errors/exo_link_too_many_top_objects.ccpn/ccpnv3/ccpnmr/gui/Task/user+View+default_user_2024-02-24-15-54-35-583_00006.xml` & `ccpn_project_checker-0.1.6/src/project_checker/test_data/delayed_errors/exo_link_too_many_top_objects.ccpn/ccpnv3/ccpnmr/gui/Task/user+View+default_user_2024-02-24-15-54-35-583_00006.xml`

 * *Files identical despite different names*

### Comparing `ccpn_project_checker-0.1.5/src/project_checker/test_data/delayed_errors/exo_link_too_many_top_objects.ccpn/ccpnv3/ccpnmr/gui/Window/_ccp_nmr_Nmr_NmrProject___default___+default_user_2024-02-24-15-54-35-583_00005.xml` & `ccpn_project_checker-0.1.6/src/project_checker/test_data/delayed_errors/exo_link_too_many_top_objects.ccpn/ccpnv3/ccpnmr/gui/Window/_ccp_nmr_Nmr_NmrProject___default___+default_user_2024-02-24-15-54-35-583_00005.xml`

 * *Files identical despite different names*

### Comparing `ccpn_project_checker-0.1.5/src/project_checker/test_data/delayed_errors/exo_link_too_many_top_objects.ccpn/ccpnv3/memops/Implementation/exo_link_too_many_top_objects.xml` & `ccpn_project_checker-0.1.6/src/project_checker/test_data/delayed_errors/exo_link_too_many_top_objects.ccpn/ccpnv3/memops/Implementation/exo_link_too_many_top_objects.xml`

 * *Files identical despite different names*

### Comparing `ccpn_project_checker-0.1.5/src/project_checker/test_data/delayed_errors/exo_linked_file_bad_xml.ccpn/ccpnv3/ccp/lims/Sample/default+default_user_2024-02-24-15-54-35-583_00002.xml` & `ccpn_project_checker-0.1.6/src/project_checker/test_data/delayed_errors/exo_linked_file_bad_xml.ccpn/ccpnv3/ccp/lims/Sample/default+default_user_2024-02-24-15-54-35-583_00002.xml`

 * *Files identical despite different names*

### Comparing `ccpn_project_checker-0.1.5/src/project_checker/test_data/delayed_errors/exo_linked_file_bad_xml.ccpn/ccpnv3/ccp/nmr/Nmr/default+default_user_2024-02-24-15-54-35-583_00001.xml` & `ccpn_project_checker-0.1.6/src/project_checker/test_data/delayed_errors/exo_linked_file_bad_xml.ccpn/ccpnv3/ccp/nmr/Nmr/default+default_user_2024-02-24-15-54-35-583_00001.xml`

 * *Files identical despite different names*

### Comparing `ccpn_project_checker-0.1.5/src/project_checker/test_data/delayed_errors/exo_linked_file_bad_xml.ccpn/ccpnv3/ccpnmr/gui/Task/user+View+default_user_2024-02-24-15-54-35-583_00006.xml` & `ccpn_project_checker-0.1.6/src/project_checker/test_data/delayed_errors/exo_linked_file_bad_xml.ccpn/ccpnv3/ccpnmr/gui/Task/user+View+default_user_2024-02-24-15-54-35-583_00006.xml`

 * *Files identical despite different names*

### Comparing `ccpn_project_checker-0.1.5/src/project_checker/test_data/delayed_errors/exo_linked_file_bad_xml.ccpn/ccpnv3/ccpnmr/gui/Window/_ccp_nmr_Nmr_NmrProject___default___+default_user_2024-02-24-15-54-35-583_00005.xml` & `ccpn_project_checker-0.1.6/src/project_checker/test_data/delayed_errors/exo_linked_file_bad_xml.ccpn/ccpnv3/ccpnmr/gui/Window/_ccp_nmr_Nmr_NmrProject___default___+default_user_2024-02-24-15-54-35-583_00005.xml`

 * *Files identical despite different names*

### Comparing `ccpn_project_checker-0.1.5/src/project_checker/test_data/delayed_errors/exo_linked_file_bad_xml.ccpn/ccpnv3/memops/Implementation/exo_linked_file_bad_xml.xml` & `ccpn_project_checker-0.1.6/src/project_checker/test_data/delayed_errors/exo_linked_file_bad_xml.ccpn/ccpnv3/memops/Implementation/exo_linked_file_bad_xml.xml`

 * *Files identical despite different names*

### Comparing `ccpn_project_checker-0.1.5/src/project_checker/test_data/delayed_errors/exo_linked_file_missing.ccpn/ccpnv3/ccp/lims/Sample/default+default_user_2024-02-24-15-54-35-583_00002.xml` & `ccpn_project_checker-0.1.6/src/project_checker/test_data/delayed_errors/exo_linked_file_missing.ccpn/ccpnv3/ccp/lims/Sample/default+default_user_2024-02-24-15-54-35-583_00002.xml`

 * *Files identical despite different names*

### Comparing `ccpn_project_checker-0.1.5/src/project_checker/test_data/delayed_errors/exo_linked_file_missing.ccpn/ccpnv3/ccp/nmr/Nmr/default+default_user_2024-02-24-15-54-35-583_00001.xml` & `ccpn_project_checker-0.1.6/src/project_checker/test_data/delayed_errors/exo_linked_file_missing.ccpn/ccpnv3/ccp/nmr/Nmr/default+default_user_2024-02-24-15-54-35-583_00001.xml`

 * *Files identical despite different names*

### Comparing `ccpn_project_checker-0.1.5/src/project_checker/test_data/delayed_errors/exo_linked_file_missing.ccpn/ccpnv3/ccpnmr/gui/Task/user+View+default_user_2024-02-24-15-54-35-583_00006.xml` & `ccpn_project_checker-0.1.6/src/project_checker/test_data/delayed_errors/exo_linked_file_missing.ccpn/ccpnv3/ccpnmr/gui/Task/user+View+default_user_2024-02-24-15-54-35-583_00006.xml`

 * *Files identical despite different names*

### Comparing `ccpn_project_checker-0.1.5/src/project_checker/test_data/delayed_errors/exo_linked_file_missing.ccpn/ccpnv3/ccpnmr/gui/Window/_ccp_nmr_Nmr_NmrProject___default___+default_user_2024-02-24-15-54-35-583_00005.xml` & `ccpn_project_checker-0.1.6/src/project_checker/test_data/delayed_errors/exo_linked_file_missing.ccpn/ccpnv3/ccpnmr/gui/Window/_ccp_nmr_Nmr_NmrProject___default___+default_user_2024-02-24-15-54-35-583_00005.xml`

 * *Files identical despite different names*

### Comparing `ccpn_project_checker-0.1.5/src/project_checker/test_data/delayed_errors/exo_linked_file_missing.ccpn/ccpnv3/memops/Implementation/exo_linked_file_missing.xml` & `ccpn_project_checker-0.1.6/src/project_checker/test_data/delayed_errors/exo_linked_file_missing.ccpn/ccpnv3/memops/Implementation/exo_linked_file_missing.xml`

 * *Files identical despite different names*

### Comparing `ccpn_project_checker-0.1.5/src/project_checker/test_data/delayed_errors/exo_linked_file_no_storage_unit.ccpn/ccpnv3/ccp/lims/Sample/default+default_user_2024-02-24-15-54-35-583_00002.xml` & `ccpn_project_checker-0.1.6/src/project_checker/test_data/delayed_errors/exo_linked_file_no_storage_unit.ccpn/ccpnv3/ccp/lims/Sample/default+default_user_2024-02-24-15-54-35-583_00002.xml`

 * *Files identical despite different names*

### Comparing `ccpn_project_checker-0.1.5/src/project_checker/test_data/delayed_errors/exo_linked_file_no_storage_unit.ccpn/ccpnv3/ccp/nmr/Nmr/default+default_user_2024-02-24-15-54-35-583_00001.xml` & `ccpn_project_checker-0.1.6/src/project_checker/test_data/delayed_errors/exo_linked_file_no_storage_unit.ccpn/ccpnv3/ccp/nmr/Nmr/default+default_user_2024-02-24-15-54-35-583_00001.xml`

 * *Files identical despite different names*

### Comparing `ccpn_project_checker-0.1.5/src/project_checker/test_data/delayed_errors/exo_linked_file_no_storage_unit.ccpn/ccpnv3/ccpnmr/gui/Task/user+View+default_user_2024-02-24-15-54-35-583_00006.xml` & `ccpn_project_checker-0.1.6/src/project_checker/test_data/delayed_errors/exo_linked_file_no_storage_unit.ccpn/ccpnv3/ccpnmr/gui/Task/user+View+default_user_2024-02-24-15-54-35-583_00006.xml`

 * *Files identical despite different names*

### Comparing `ccpn_project_checker-0.1.5/src/project_checker/test_data/delayed_errors/exo_linked_file_no_storage_unit.ccpn/ccpnv3/ccpnmr/gui/Window/_ccp_nmr_Nmr_NmrProject___default___+default_user_2024-02-24-15-54-35-583_00005.xml` & `ccpn_project_checker-0.1.6/src/project_checker/test_data/delayed_errors/exo_linked_file_no_storage_unit.ccpn/ccpnv3/ccpnmr/gui/Window/_ccp_nmr_Nmr_NmrProject___default___+default_user_2024-02-24-15-54-35-583_00005.xml`

 * *Files identical despite different names*

### Comparing `ccpn_project_checker-0.1.5/src/project_checker/test_data/delayed_errors/exo_linked_file_no_storage_unit.ccpn/ccpnv3/memops/Implementation/exo_linked_file_no_storage_unit.xml` & `ccpn_project_checker-0.1.6/src/project_checker/test_data/delayed_errors/exo_linked_file_no_storage_unit.ccpn/ccpnv3/memops/Implementation/exo_linked_file_no_storage_unit.xml`

 * *Files identical despite different names*

### Comparing `ccpn_project_checker-0.1.5/src/project_checker/test_data/delayed_errors/exo_links_with_keys_outside_ccpn_character_set.ccpn/ccpnv3/ccp/lims/Sample/default+default_user_2024-02-24-15-54-35-583_00002.xml` & `ccpn_project_checker-0.1.6/src/project_checker/test_data/delayed_errors/exo_links_with_keys_outside_ccpn_character_set.ccpn/ccpnv3/ccp/lims/Sample/default+default_user_2024-02-24-15-54-35-583_00002.xml`

 * *Files identical despite different names*

### Comparing `ccpn_project_checker-0.1.5/src/project_checker/test_data/delayed_errors/exo_links_with_keys_outside_ccpn_character_set.ccpn/ccpnv3/ccp/nmr/Nmr/default+default_user_2024-02-24-15-54-35-583_00001.xml` & `ccpn_project_checker-0.1.6/src/project_checker/test_data/delayed_errors/exo_links_with_keys_outside_ccpn_character_set.ccpn/ccpnv3/ccp/nmr/Nmr/default+default_user_2024-02-24-15-54-35-583_00001.xml`

 * *Files identical despite different names*

### Comparing `ccpn_project_checker-0.1.5/src/project_checker/test_data/delayed_errors/exo_links_with_keys_outside_ccpn_character_set.ccpn/ccpnv3/ccpnmr/gui/Task/user+View~+default_user_2024-02-24-15-54-35-583_00006.xml` & `ccpn_project_checker-0.1.6/src/project_checker/test_data/delayed_errors/exo_links_with_keys_outside_ccpn_character_set.ccpn/ccpnv3/ccpnmr/gui/Task/user+View~+default_user_2024-02-24-15-54-35-583_00006.xml`

 * *Files identical despite different names*

### Comparing `ccpn_project_checker-0.1.5/src/project_checker/test_data/delayed_errors/exo_links_with_keys_outside_ccpn_character_set.ccpn/ccpnv3/ccpnmr/gui/Window/_ccp_nmr_Nmr_NmrProject___default___+default_user_2024-02-24-15-54-35-583_00005.xml` & `ccpn_project_checker-0.1.6/src/project_checker/test_data/delayed_errors/exo_links_with_keys_outside_ccpn_character_set.ccpn/ccpnv3/ccpnmr/gui/Window/_ccp_nmr_Nmr_NmrProject___default___+default_user_2024-02-24-15-54-35-583_00005.xml`

 * *Files identical despite different names*

### Comparing `ccpn_project_checker-0.1.5/src/project_checker/test_data/delayed_errors/exo_links_with_keys_outside_ccpn_character_set.ccpn/ccpnv3/memops/Implementation/exo_links_with_keys_outside_ccpn_character_set.xml` & `ccpn_project_checker-0.1.6/src/project_checker/test_data/delayed_errors/exo_links_with_keys_outside_ccpn_character_set.ccpn/ccpnv3/memops/Implementation/exo_links_with_keys_outside_ccpn_character_set.xml`

 * *Files identical despite different names*

### Comparing `ccpn_project_checker-0.1.5/src/project_checker/test_data/delayed_errors/external_guid_doesnt_match_internal.ccpn/ccpnv3/ccp/lims/Sample/default+default_user_2024-02-24-15-54-35-583_00002.xml` & `ccpn_project_checker-0.1.6/src/project_checker/test_data/delayed_errors/external_guid_doesnt_match_internal.ccpn/ccpnv3/ccp/lims/Sample/default+default_user_2024-02-24-15-54-35-583_00002.xml`

 * *Files identical despite different names*

### Comparing `ccpn_project_checker-0.1.5/src/project_checker/test_data/delayed_errors/external_guid_doesnt_match_internal.ccpn/ccpnv3/ccp/nmr/Nmr/default+default_user_2024-02-24-15-54-35-583_00001.xml` & `ccpn_project_checker-0.1.6/src/project_checker/test_data/delayed_errors/external_guid_doesnt_match_internal.ccpn/ccpnv3/ccp/nmr/Nmr/default+default_user_2024-02-24-15-54-35-583_00001.xml`

 * *Files identical despite different names*

### Comparing `ccpn_project_checker-0.1.5/src/project_checker/test_data/delayed_errors/external_guid_doesnt_match_internal.ccpn/ccpnv3/ccpnmr/gui/Task/user+View+default_user_2024-02-24-15-54-35-583_00006.xml` & `ccpn_project_checker-0.1.6/src/project_checker/test_data/delayed_errors/external_guid_doesnt_match_internal.ccpn/ccpnv3/ccpnmr/gui/Task/user+View+default_user_2024-02-24-15-54-35-583_00006.xml`

 * *Files identical despite different names*

### Comparing `ccpn_project_checker-0.1.5/src/project_checker/test_data/delayed_errors/external_guid_doesnt_match_internal.ccpn/ccpnv3/ccpnmr/gui/Window/_ccp_nmr_Nmr_NmrProject___default___+default_user_2024-02-24-15-54-35-583_00005.xml` & `ccpn_project_checker-0.1.6/src/project_checker/test_data/delayed_errors/external_guid_doesnt_match_internal.ccpn/ccpnv3/ccpnmr/gui/Window/_ccp_nmr_Nmr_NmrProject___default___+default_user_2024-02-24-15-54-35-583_00005.xml`

 * *Files identical despite different names*

### Comparing `ccpn_project_checker-0.1.5/src/project_checker/test_data/delayed_errors/external_guid_doesnt_match_internal.ccpn/ccpnv3/memops/Implementation/external_guid_doesnt_match_internal.xml` & `ccpn_project_checker-0.1.6/src/project_checker/test_data/delayed_errors/external_guid_doesnt_match_internal.ccpn/ccpnv3/memops/Implementation/external_guid_doesnt_match_internal.xml`

 * *Files identical despite different names*

### Comparing `ccpn_project_checker-0.1.5/src/project_checker/test_data/delayed_errors/root_exo_link_missing_source_element.ccpn/ccpnv3/ccp/lims/Sample/default+default_user_2024-02-24-15-54-35-583_00002.xml` & `ccpn_project_checker-0.1.6/src/project_checker/test_data/delayed_errors/root_exo_link_missing_source_element.ccpn/ccpnv3/ccp/lims/Sample/default+default_user_2024-02-24-15-54-35-583_00002.xml`

 * *Files identical despite different names*

### Comparing `ccpn_project_checker-0.1.5/src/project_checker/test_data/delayed_errors/root_exo_link_missing_source_element.ccpn/ccpnv3/ccp/nmr/Nmr/default+default_user_2024-02-24-15-54-35-583_00001.xml` & `ccpn_project_checker-0.1.6/src/project_checker/test_data/delayed_errors/root_exo_link_missing_source_element.ccpn/ccpnv3/ccp/nmr/Nmr/default+default_user_2024-02-24-15-54-35-583_00001.xml`

 * *Files identical despite different names*

### Comparing `ccpn_project_checker-0.1.5/src/project_checker/test_data/delayed_errors/root_exo_link_missing_source_element.ccpn/ccpnv3/ccpnmr/gui/Task/user+View+default_user_2024-02-24-15-54-35-583_00006.xml` & `ccpn_project_checker-0.1.6/src/project_checker/test_data/delayed_errors/root_exo_link_missing_source_element.ccpn/ccpnv3/ccpnmr/gui/Task/user+View+default_user_2024-02-24-15-54-35-583_00006.xml`

 * *Files identical despite different names*

### Comparing `ccpn_project_checker-0.1.5/src/project_checker/test_data/delayed_errors/root_exo_link_missing_source_element.ccpn/ccpnv3/ccpnmr/gui/Window/_ccp_nmr_Nmr_NmrProject___default___+default_user_2024-02-24-15-54-35-583_00005.xml` & `ccpn_project_checker-0.1.6/src/project_checker/test_data/delayed_errors/root_exo_link_missing_source_element.ccpn/ccpnv3/ccpnmr/gui/Window/_ccp_nmr_Nmr_NmrProject___default___+default_user_2024-02-24-15-54-35-583_00005.xml`

 * *Files identical despite different names*

### Comparing `ccpn_project_checker-0.1.5/src/project_checker/test_data/delayed_errors/root_exo_link_missing_source_element.ccpn/ccpnv3/memops/Implementation/root_exo_link_missing_source_element.xml` & `ccpn_project_checker-0.1.6/src/project_checker/test_data/delayed_errors/root_exo_link_missing_source_element.ccpn/ccpnv3/memops/Implementation/root_exo_link_missing_source_element.xml`

 * *Files identical despite different names*

### Comparing `ccpn_project_checker-0.1.5/src/project_checker/test_data/delayed_errors/root_exo_link_too_many_source_elements.ccpn/ccpnv3/ccp/lims/Sample/default+default_user_2024-02-24-15-54-35-583_00002.xml` & `ccpn_project_checker-0.1.6/src/project_checker/test_data/delayed_errors/root_exo_link_too_many_source_elements.ccpn/ccpnv3/ccp/lims/Sample/default+default_user_2024-02-24-15-54-35-583_00002.xml`

 * *Files identical despite different names*

### Comparing `ccpn_project_checker-0.1.5/src/project_checker/test_data/delayed_errors/root_exo_link_too_many_source_elements.ccpn/ccpnv3/ccp/nmr/Nmr/default+default_user_2024-02-24-15-54-35-583_00001.xml` & `ccpn_project_checker-0.1.6/src/project_checker/test_data/delayed_errors/root_exo_link_too_many_source_elements.ccpn/ccpnv3/ccp/nmr/Nmr/default+default_user_2024-02-24-15-54-35-583_00001.xml`

 * *Files identical despite different names*

### Comparing `ccpn_project_checker-0.1.5/src/project_checker/test_data/delayed_errors/root_exo_link_too_many_source_elements.ccpn/ccpnv3/ccpnmr/gui/Task/user+View+default_user_2024-02-24-15-54-35-583_00006.xml` & `ccpn_project_checker-0.1.6/src/project_checker/test_data/delayed_errors/root_exo_link_too_many_source_elements.ccpn/ccpnv3/ccpnmr/gui/Task/user+View+default_user_2024-02-24-15-54-35-583_00006.xml`

 * *Files identical despite different names*

### Comparing `ccpn_project_checker-0.1.5/src/project_checker/test_data/delayed_errors/root_exo_link_too_many_source_elements.ccpn/ccpnv3/ccpnmr/gui/Window/_ccp_nmr_Nmr_NmrProject___default___+default_user_2024-02-24-15-54-35-583_00005.xml` & `ccpn_project_checker-0.1.6/src/project_checker/test_data/delayed_errors/root_exo_link_too_many_source_elements.ccpn/ccpnv3/ccpnmr/gui/Window/_ccp_nmr_Nmr_NmrProject___default___+default_user_2024-02-24-15-54-35-583_00005.xml`

 * *Files identical despite different names*

### Comparing `ccpn_project_checker-0.1.5/src/project_checker/test_data/delayed_errors/root_exo_link_too_many_source_elements.ccpn/ccpnv3/memops/Implementation/root_exo_link_too_many_source_elements.xml` & `ccpn_project_checker-0.1.6/src/project_checker/test_data/delayed_errors/root_exo_link_too_many_source_elements.ccpn/ccpnv3/memops/Implementation/root_exo_link_too_many_source_elements.xml`

 * *Files identical despite different names*

### Comparing `ccpn_project_checker-0.1.5/src/project_checker/test_data/empty_good_project_multiple_root_xml_files.ccpn/ccpnv3/ccp/lims/Sample/default+default_user_2024-02-24-15-54-35-583_00002.xml` & `ccpn_project_checker-0.1.6/src/project_checker/test_data/empty_good_project_multiple_root_xml_files.ccpn/ccpnv3/ccp/lims/Sample/default+default_user_2024-02-24-15-54-35-583_00002.xml`

 * *Files identical despite different names*

### Comparing `ccpn_project_checker-0.1.5/src/project_checker/test_data/empty_good_project_multiple_root_xml_files.ccpn/ccpnv3/ccp/nmr/Nmr/default+default_user_2024-02-24-15-54-35-583_00001.xml` & `ccpn_project_checker-0.1.6/src/project_checker/test_data/empty_good_project_multiple_root_xml_files.ccpn/ccpnv3/ccp/nmr/Nmr/default+default_user_2024-02-24-15-54-35-583_00001.xml`

 * *Files identical despite different names*

### Comparing `ccpn_project_checker-0.1.5/src/project_checker/test_data/empty_good_project_multiple_root_xml_files.ccpn/ccpnv3/ccpnmr/gui/Task/user+View+default_user_2024-02-24-15-54-35-583_00006.xml` & `ccpn_project_checker-0.1.6/src/project_checker/test_data/empty_good_project_multiple_root_xml_files.ccpn/ccpnv3/ccpnmr/gui/Task/user+View+default_user_2024-02-24-15-54-35-583_00006.xml`

 * *Files identical despite different names*

### Comparing `ccpn_project_checker-0.1.5/src/project_checker/test_data/empty_good_project_multiple_root_xml_files.ccpn/ccpnv3/ccpnmr/gui/Window/_ccp_nmr_Nmr_NmrProject___default___+default_user_2024-02-24-15-54-35-583_00005.xml` & `ccpn_project_checker-0.1.6/src/project_checker/test_data/empty_good_project_multiple_root_xml_files.ccpn/ccpnv3/ccpnmr/gui/Window/_ccp_nmr_Nmr_NmrProject___default___+default_user_2024-02-24-15-54-35-583_00005.xml`

 * *Files identical despite different names*

### Comparing `ccpn_project_checker-0.1.5/src/project_checker/test_data/empty_good_project_multiple_root_xml_files.ccpn/ccpnv3/memops/Implementation/empty_good_project_mutiple_root_xml_files_1.xml` & `ccpn_project_checker-0.1.6/src/project_checker/test_data/empty_good_project_multiple_root_xml_files.ccpn/ccpnv3/memops/Implementation/empty_good_project_mutiple_root_xml_files_1.xml`

 * *Files identical despite different names*

### Comparing `ccpn_project_checker-0.1.5/src/project_checker/test_data/empty_good_project_multiple_root_xml_files.ccpn/ccpnv3/memops/Implementation/empty_good_project_mutiple_root_xml_files_2.xml` & `ccpn_project_checker-0.1.6/src/project_checker/test_data/empty_good_project_multiple_root_xml_files.ccpn/ccpnv3/memops/Implementation/empty_good_project_mutiple_root_xml_files_2.xml`

 * *Files identical despite different names*

### Comparing `ccpn_project_checker-0.1.5/src/project_checker/test_data/good_projects/Sec5Part4.ccpn/ccpnv3/ccp/general/DataLocation/standard+default_user_2022-02-23-14-57-20-615_00001.xml` & `ccpn_project_checker-0.1.6/src/project_checker/test_data/good_projects/Sec5Part4.ccpn/ccpnv3/ccp/general/DataLocation/standard+default_user_2022-02-23-14-57-20-615_00001.xml`

 * *Files identical despite different names*

### Comparing `ccpn_project_checker-0.1.5/src/project_checker/test_data/good_projects/Sec5Part4.ccpn/ccpnv3/ccp/general/DataLocation/standard+default_user_2022-02-23-14-57-20-615_00001.xml.bak` & `ccpn_project_checker-0.1.6/src/project_checker/test_data/good_projects/Sec5Part4.ccpn/ccpnv3/ccp/general/DataLocation/standard+default_user_2022-02-23-14-57-20-615_00001.xml.bak`

 * *Files identical despite different names*

### Comparing `ccpn_project_checker-0.1.5/src/project_checker/test_data/good_projects/Sec5Part4.ccpn/ccpnv3/ccp/lims/RefSampleComponent/default+default_user_2022-02-23-14-57-20-616_00003.xml` & `ccpn_project_checker-0.1.6/src/project_checker/test_data/good_projects/Sec5Part4.ccpn/ccpnv3/ccp/lims/RefSampleComponent/default+default_user_2022-02-23-14-57-20-616_00003.xml`

 * *Files identical despite different names*

### Comparing `ccpn_project_checker-0.1.5/src/project_checker/test_data/good_projects/Sec5Part4.ccpn/ccpnv3/ccp/lims/RefSampleComponent/default+default_user_2022-02-23-14-57-20-616_00003.xml.bak` & `ccpn_project_checker-0.1.6/src/project_checker/test_data/good_projects/Sec5Part4.ccpn/ccpnv3/ccp/lims/RefSampleComponent/default+default_user_2022-02-23-14-57-20-616_00003.xml.bak`

 * *Files identical despite different names*

### Comparing `ccpn_project_checker-0.1.5/src/project_checker/test_data/good_projects/Sec5Part4.ccpn/ccpnv3/ccp/lims/Sample/default+default_user_2022-02-23-14-57-20-616_00002.xml` & `ccpn_project_checker-0.1.6/src/project_checker/test_data/good_projects/Sec5Part4.ccpn/ccpnv3/ccp/lims/Sample/default+default_user_2022-02-23-14-57-20-616_00002.xml`

 * *Files identical despite different names*

### Comparing `ccpn_project_checker-0.1.5/src/project_checker/test_data/good_projects/Sec5Part4.ccpn/ccpnv3/ccp/molecule/MolSystem/default+default_user_2022-02-23-14-57-20-617_00001.xml` & `ccpn_project_checker-0.1.6/src/project_checker/test_data/good_projects/Sec5Part4.ccpn/ccpnv3/ccp/molecule/MolSystem/default+default_user_2022-02-23-14-57-20-617_00001.xml`

 * *Files identical despite different names*

### Comparing `ccpn_project_checker-0.1.5/src/project_checker/test_data/good_projects/Sec5Part4.ccpn/ccpnv3/ccp/molecule/MolSystem/default+default_user_2022-02-23-14-57-20-617_00001.xml.bak` & `ccpn_project_checker-0.1.6/src/project_checker/test_data/good_projects/Sec5Part4.ccpn/ccpnv3/ccp/molecule/MolSystem/default+default_user_2022-02-23-14-57-20-617_00001.xml.bak`

 * *Files identical despite different names*

### Comparing `ccpn_project_checker-0.1.5/src/project_checker/test_data/good_projects/Sec5Part4.ccpn/ccpnv3/ccp/molecule/Molecule/Sec5+Sec5Part1_user_2022-02-23-15-20-24-415_00001.xml` & `ccpn_project_checker-0.1.6/src/project_checker/test_data/good_projects/Sec5Part4.ccpn/ccpnv3/ccp/molecule/Molecule/Sec5+Sec5Part1_user_2022-02-23-15-20-24-415_00001.xml`

 * *Files identical despite different names*

### Comparing `ccpn_project_checker-0.1.5/src/project_checker/test_data/good_projects/Sec5Part4.ccpn/ccpnv3/ccp/nmr/Nmr/default+default_user_2022-02-23-14-57-20-616_00001.xml` & `ccpn_project_checker-0.1.6/src/project_checker/test_data/good_projects/Sec5Part4.ccpn/ccpnv3/ccp/nmr/Nmr/default+default_user_2022-02-23-14-57-20-616_00001.xml`

 * *Files identical despite different names*

### Comparing `ccpn_project_checker-0.1.5/src/project_checker/test_data/good_projects/Sec5Part4.ccpn/ccpnv3/ccp/nmr/Nmr/default+default_user_2022-02-23-14-57-20-616_00001.xml.bak` & `ccpn_project_checker-0.1.6/src/project_checker/test_data/good_projects/Sec5Part4.ccpn/ccpnv3/ccp/nmr/Nmr/default+default_user_2022-02-23-14-57-20-616_00001.xml.bak`

 * *Files identical despite different names*

### Comparing `ccpn_project_checker-0.1.5/src/project_checker/test_data/good_projects/Sec5Part4.ccpn/ccpnv3/ccpnmr/gui/Task/user+View+default_user_2022-02-23-14-57-20-617_00003.xml` & `ccpn_project_checker-0.1.6/src/project_checker/test_data/good_projects/Sec5Part4.ccpn/ccpnv3/ccpnmr/gui/Task/user+View+default_user_2022-02-23-14-57-20-617_00003.xml`

 * *Files identical despite different names*

### Comparing `ccpn_project_checker-0.1.5/src/project_checker/test_data/good_projects/Sec5Part4.ccpn/ccpnv3/ccpnmr/gui/Task/user+View+default_user_2022-02-23-14-57-20-617_00003.xml.bak` & `ccpn_project_checker-0.1.6/src/project_checker/test_data/good_projects/Sec5Part4.ccpn/ccpnv3/ccpnmr/gui/Task/user+View+default_user_2022-02-23-14-57-20-617_00003.xml.bak`

 * *Files identical despite different names*

### Comparing `ccpn_project_checker-0.1.5/src/project_checker/test_data/good_projects/Sec5Part4.ccpn/ccpnv3/ccpnmr/gui/Window/_ccp_nmr_Nmr_NmrProject___default___+default_user_2022-02-23-14-57-20-617_00002.xml` & `ccpn_project_checker-0.1.6/src/project_checker/test_data/good_projects/Sec5Part4.ccpn/ccpnv3/ccpnmr/gui/Window/_ccp_nmr_Nmr_NmrProject___default___+default_user_2022-02-23-14-57-20-617_00002.xml`

 * *Files identical despite different names*

### Comparing `ccpn_project_checker-0.1.5/src/project_checker/test_data/good_projects/Sec5Part4.ccpn/ccpnv3/ccpnmr/gui/Window/_ccp_nmr_Nmr_NmrProject___default___+default_user_2022-02-23-14-57-20-617_00002.xml.bak` & `ccpn_project_checker-0.1.6/src/project_checker/test_data/good_projects/Sec5Part4.ccpn/ccpnv3/ccpnmr/gui/Window/_ccp_nmr_Nmr_NmrProject___default___+default_user_2022-02-23-14-57-20-617_00002.xml.bak`

 * *Files identical despite different names*

### Comparing `ccpn_project_checker-0.1.5/src/project_checker/test_data/good_projects/Sec5Part4.ccpn/ccpnv3/memops/Implementation/Sec5Part4.xml` & `ccpn_project_checker-0.1.6/src/project_checker/test_data/good_projects/Sec5Part4.ccpn/ccpnv3/memops/Implementation/Sec5Part4.xml`

 * *Files identical despite different names*

### Comparing `ccpn_project_checker-0.1.5/src/project_checker/test_data/good_projects/Sec5Part4.ccpn/ccpnv3/memops/Implementation/Sec5Part4.xml.bak` & `ccpn_project_checker-0.1.6/src/project_checker/test_data/good_projects/Sec5Part4.ccpn/ccpnv3/memops/Implementation/Sec5Part4.xml.bak`

 * *Files identical despite different names*

### Comparing `ccpn_project_checker-0.1.5/src/project_checker/test_data/good_projects/empty_good_project.ccpn/ccpnv3/ccp/lims/Sample/default+default_user_2024-02-24-15-54-35-583_00002.xml` & `ccpn_project_checker-0.1.6/src/project_checker/test_data/good_projects/empty_good_project.ccpn/ccpnv3/ccp/lims/Sample/default+default_user_2024-02-24-15-54-35-583_00002.xml`

 * *Files identical despite different names*

### Comparing `ccpn_project_checker-0.1.5/src/project_checker/test_data/good_projects/empty_good_project.ccpn/ccpnv3/ccp/nmr/Nmr/default+default_user_2024-02-24-15-54-35-583_00001.xml` & `ccpn_project_checker-0.1.6/src/project_checker/test_data/good_projects/empty_good_project.ccpn/ccpnv3/ccp/nmr/Nmr/default+default_user_2024-02-24-15-54-35-583_00001.xml`

 * *Files identical despite different names*

### Comparing `ccpn_project_checker-0.1.5/src/project_checker/test_data/good_projects/empty_good_project.ccpn/ccpnv3/ccpnmr/gui/Task/user+View+default_user_2024-02-24-15-54-35-583_00006.xml` & `ccpn_project_checker-0.1.6/src/project_checker/test_data/good_projects/empty_good_project.ccpn/ccpnv3/ccpnmr/gui/Task/user+View+default_user_2024-02-24-15-54-35-583_00006.xml`

 * *Files identical despite different names*

### Comparing `ccpn_project_checker-0.1.5/src/project_checker/test_data/good_projects/empty_good_project.ccpn/ccpnv3/ccpnmr/gui/Window/_ccp_nmr_Nmr_NmrProject___default___+default_user_2024-02-24-15-54-35-583_00005.xml` & `ccpn_project_checker-0.1.6/src/project_checker/test_data/good_projects/empty_good_project.ccpn/ccpnv3/ccpnmr/gui/Window/_ccp_nmr_Nmr_NmrProject___default___+default_user_2024-02-24-15-54-35-583_00005.xml`

 * *Files identical despite different names*

### Comparing `ccpn_project_checker-0.1.5/src/project_checker/test_data/good_projects/empty_good_project.ccpn/ccpnv3/memops/Implementation/empty_good_project.xml` & `ccpn_project_checker-0.1.6/src/project_checker/test_data/good_projects/empty_good_project.ccpn/ccpnv3/memops/Implementation/empty_good_project.xml`

 * *Files identical despite different names*

### Comparing `ccpn_project_checker-0.1.5/src/project_checker/test_data/good_projects/empty_good_project_renamed.ccpn/ccpnv3/ccp/lims/Sample/default+default_user_2024-02-24-15-54-35-583_00002.xml` & `ccpn_project_checker-0.1.6/src/project_checker/test_data/good_projects/empty_good_project_renamed.ccpn/ccpnv3/ccp/lims/Sample/default+default_user_2024-02-24-15-54-35-583_00002.xml`

 * *Files identical despite different names*

### Comparing `ccpn_project_checker-0.1.5/src/project_checker/test_data/good_projects/empty_good_project_renamed.ccpn/ccpnv3/ccp/nmr/Nmr/default+default_user_2024-02-24-15-54-35-583_00001.xml` & `ccpn_project_checker-0.1.6/src/project_checker/test_data/good_projects/empty_good_project_renamed.ccpn/ccpnv3/ccp/nmr/Nmr/default+default_user_2024-02-24-15-54-35-583_00001.xml`

 * *Files identical despite different names*

### Comparing `ccpn_project_checker-0.1.5/src/project_checker/test_data/good_projects/empty_good_project_renamed.ccpn/ccpnv3/ccpnmr/gui/Task/user+View+default_user_2024-02-24-15-54-35-583_00006.xml` & `ccpn_project_checker-0.1.6/src/project_checker/test_data/good_projects/empty_good_project_renamed.ccpn/ccpnv3/ccpnmr/gui/Task/user+View+default_user_2024-02-24-15-54-35-583_00006.xml`

 * *Files identical despite different names*

### Comparing `ccpn_project_checker-0.1.5/src/project_checker/test_data/good_projects/empty_good_project_renamed.ccpn/ccpnv3/ccpnmr/gui/Window/_ccp_nmr_Nmr_NmrProject___default___+default_user_2024-02-24-15-54-35-583_00005.xml` & `ccpn_project_checker-0.1.6/src/project_checker/test_data/good_projects/empty_good_project_renamed.ccpn/ccpnv3/ccpnmr/gui/Window/_ccp_nmr_Nmr_NmrProject___default___+default_user_2024-02-24-15-54-35-583_00005.xml`

 * *Files identical despite different names*

### Comparing `ccpn_project_checker-0.1.5/src/project_checker/test_data/good_projects/empty_good_project_renamed.ccpn/ccpnv3/memops/Implementation/empty_good_project_renamed.xml` & `ccpn_project_checker-0.1.6/src/project_checker/test_data/good_projects/empty_good_project_renamed.ccpn/ccpnv3/memops/Implementation/empty_good_project_renamed.xml`

 * *Files identical despite different names*

### Comparing `ccpn_project_checker-0.1.5/src/project_checker/test_data/memops_root_no_read_empty_good_project.ccpn/ccpnv3/ccp/lims/Sample/default+default_user_2024-02-24-15-54-35-583_00002.xml` & `ccpn_project_checker-0.1.6/src/project_checker/test_data/memops_root_no_read_empty_good_project.ccpn/ccpnv3/ccp/lims/Sample/default+default_user_2024-02-24-15-54-35-583_00002.xml`

 * *Files identical despite different names*

### Comparing `ccpn_project_checker-0.1.5/src/project_checker/test_data/memops_root_no_read_empty_good_project.ccpn/ccpnv3/ccp/nmr/Nmr/default+default_user_2024-02-24-15-54-35-583_00001.xml` & `ccpn_project_checker-0.1.6/src/project_checker/test_data/memops_root_no_read_empty_good_project.ccpn/ccpnv3/ccp/nmr/Nmr/default+default_user_2024-02-24-15-54-35-583_00001.xml`

 * *Files identical despite different names*

### Comparing `ccpn_project_checker-0.1.5/src/project_checker/test_data/memops_root_no_read_empty_good_project.ccpn/ccpnv3/ccpnmr/gui/Task/user+View+default_user_2024-02-24-15-54-35-583_00006.xml` & `ccpn_project_checker-0.1.6/src/project_checker/test_data/memops_root_no_read_empty_good_project.ccpn/ccpnv3/ccpnmr/gui/Task/user+View+default_user_2024-02-24-15-54-35-583_00006.xml`

 * *Files identical despite different names*

### Comparing `ccpn_project_checker-0.1.5/src/project_checker/test_data/memops_root_no_read_empty_good_project.ccpn/ccpnv3/ccpnmr/gui/Window/_ccp_nmr_Nmr_NmrProject___default___+default_user_2024-02-24-15-54-35-583_00005.xml` & `ccpn_project_checker-0.1.6/src/project_checker/test_data/memops_root_no_read_empty_good_project.ccpn/ccpnv3/ccpnmr/gui/Window/_ccp_nmr_Nmr_NmrProject___default___+default_user_2024-02-24-15-54-35-583_00005.xml`

 * *Files identical despite different names*

### Comparing `ccpn_project_checker-0.1.5/src/project_checker/test_data/memops_root_no_read_empty_good_project.ccpn/ccpnv3/memops/Implementation/memops_root_no_read_empty_good_project.xml` & `ccpn_project_checker-0.1.6/src/project_checker/test_data/memops_root_no_read_empty_good_project.ccpn/ccpnv3/memops/Implementation/memops_root_no_read_empty_good_project.xml`

 * *Files identical despite different names*

### Comparing `ccpn_project_checker-0.1.5/src/project_checker/test_data/memops_root_no_storage_unit.ccpn/ccpnv3/memops/Implementation/memops_root_no_storage_unit.xml` & `ccpn_project_checker-0.1.6/src/project_checker/test_data/memops_root_no_storage_unit.ccpn/ccpnv3/memops/Implementation/memops_root_no_storage_unit.xml`

 * *Files identical despite different names*

### Comparing `ccpn_project_checker-0.1.5/src/project_checker/test_data/no_memops_root_element.ccpn/ccpnv3/ccp/lims/Sample/default+default_user_2024-02-24-15-54-35-583_00002.xml` & `ccpn_project_checker-0.1.6/src/project_checker/test_data/no_memops_root_element.ccpn/ccpnv3/ccp/lims/Sample/default+default_user_2024-02-24-15-54-35-583_00002.xml`

 * *Files identical despite different names*

### Comparing `ccpn_project_checker-0.1.5/src/project_checker/test_data/no_memops_root_element.ccpn/ccpnv3/ccp/nmr/Nmr/default+default_user_2024-02-24-15-54-35-583_00001.xml` & `ccpn_project_checker-0.1.6/src/project_checker/test_data/no_memops_root_element.ccpn/ccpnv3/ccp/nmr/Nmr/default+default_user_2024-02-24-15-54-35-583_00001.xml`

 * *Files identical despite different names*

### Comparing `ccpn_project_checker-0.1.5/src/project_checker/test_data/no_memops_root_element.ccpn/ccpnv3/ccpnmr/gui/Task/user+View+default_user_2024-02-24-15-54-35-583_00006.xml` & `ccpn_project_checker-0.1.6/src/project_checker/test_data/no_memops_root_element.ccpn/ccpnv3/ccpnmr/gui/Task/user+View+default_user_2024-02-24-15-54-35-583_00006.xml`

 * *Files identical despite different names*

### Comparing `ccpn_project_checker-0.1.5/src/project_checker/test_data/no_memops_root_element.ccpn/ccpnv3/ccpnmr/gui/Window/_ccp_nmr_Nmr_NmrProject___default___+default_user_2024-02-24-15-54-35-583_00005.xml` & `ccpn_project_checker-0.1.6/src/project_checker/test_data/no_memops_root_element.ccpn/ccpnv3/ccpnmr/gui/Window/_ccp_nmr_Nmr_NmrProject___default___+default_user_2024-02-24-15-54-35-583_00005.xml`

 * *Files identical despite different names*

### Comparing `ccpn_project_checker-0.1.5/src/project_checker/test_data/no_memops_root_element.ccpn/ccpnv3/memops/Implementation/no_memops_root_element.xml` & `ccpn_project_checker-0.1.6/src/project_checker/test_data/no_memops_root_element.ccpn/ccpnv3/memops/Implementation/no_memops_root_element.xml`

 * *Files identical despite different names*

### Comparing `ccpn_project_checker-0.1.5/src/project_checker/test_data/root_not_memops_root_element.ccpn/ccpnv3/ccp/lims/Sample/default+default_user_2024-02-24-15-54-35-583_00002.xml` & `ccpn_project_checker-0.1.6/src/project_checker/test_data/root_not_memops_root_element.ccpn/ccpnv3/ccp/lims/Sample/default+default_user_2024-02-24-15-54-35-583_00002.xml`

 * *Files identical despite different names*

### Comparing `ccpn_project_checker-0.1.5/src/project_checker/test_data/root_not_memops_root_element.ccpn/ccpnv3/ccp/nmr/Nmr/default+default_user_2024-02-24-15-54-35-583_00001.xml` & `ccpn_project_checker-0.1.6/src/project_checker/test_data/root_not_memops_root_element.ccpn/ccpnv3/ccp/nmr/Nmr/default+default_user_2024-02-24-15-54-35-583_00001.xml`

 * *Files identical despite different names*

### Comparing `ccpn_project_checker-0.1.5/src/project_checker/test_data/root_not_memops_root_element.ccpn/ccpnv3/ccpnmr/gui/Task/user+View+default_user_2024-02-24-15-54-35-583_00006.xml` & `ccpn_project_checker-0.1.6/src/project_checker/test_data/root_not_memops_root_element.ccpn/ccpnv3/ccpnmr/gui/Task/user+View+default_user_2024-02-24-15-54-35-583_00006.xml`

 * *Files identical despite different names*

### Comparing `ccpn_project_checker-0.1.5/src/project_checker/test_data/root_not_memops_root_element.ccpn/ccpnv3/ccpnmr/gui/Window/_ccp_nmr_Nmr_NmrProject___default___+default_user_2024-02-24-15-54-35-583_00005.xml` & `ccpn_project_checker-0.1.6/src/project_checker/test_data/root_not_memops_root_element.ccpn/ccpnv3/ccpnmr/gui/Window/_ccp_nmr_Nmr_NmrProject___default___+default_user_2024-02-24-15-54-35-583_00005.xml`

 * *Files identical despite different names*

### Comparing `ccpn_project_checker-0.1.5/src/project_checker/test_data/root_not_memops_root_element.ccpn/ccpnv3/memops/Implementation/root_not_memops_root_element.xml` & `ccpn_project_checker-0.1.6/src/project_checker/test_data/root_not_memops_root_element.ccpn/ccpnv3/memops/Implementation/root_not_memops_root_element.xml`

 * *Files identical despite different names*

### Comparing `ccpn_project_checker-0.1.5/src/project_checker/test_data/root_version_badly_formatted.ccpn/ccpnv3/ccp/lims/Sample/default+default_user_2024-02-24-15-54-35-583_00002.xml` & `ccpn_project_checker-0.1.6/src/project_checker/test_data/root_version_badly_formatted.ccpn/ccpnv3/ccp/lims/Sample/default+default_user_2024-02-24-15-54-35-583_00002.xml`

 * *Files identical despite different names*

### Comparing `ccpn_project_checker-0.1.5/src/project_checker/test_data/root_version_badly_formatted.ccpn/ccpnv3/ccp/nmr/Nmr/default+default_user_2024-02-24-15-54-35-583_00001.xml` & `ccpn_project_checker-0.1.6/src/project_checker/test_data/root_version_badly_formatted.ccpn/ccpnv3/ccp/nmr/Nmr/default+default_user_2024-02-24-15-54-35-583_00001.xml`

 * *Files identical despite different names*

### Comparing `ccpn_project_checker-0.1.5/src/project_checker/test_data/root_version_badly_formatted.ccpn/ccpnv3/ccpnmr/gui/Task/user+View+default_user_2024-02-24-15-54-35-583_00006.xml` & `ccpn_project_checker-0.1.6/src/project_checker/test_data/root_version_badly_formatted.ccpn/ccpnv3/ccpnmr/gui/Task/user+View+default_user_2024-02-24-15-54-35-583_00006.xml`

 * *Files identical despite different names*

### Comparing `ccpn_project_checker-0.1.5/src/project_checker/test_data/root_version_badly_formatted.ccpn/ccpnv3/ccpnmr/gui/Window/_ccp_nmr_Nmr_NmrProject___default___+default_user_2024-02-24-15-54-35-583_00005.xml` & `ccpn_project_checker-0.1.6/src/project_checker/test_data/root_version_badly_formatted.ccpn/ccpnv3/ccpnmr/gui/Window/_ccp_nmr_Nmr_NmrProject___default___+default_user_2024-02-24-15-54-35-583_00005.xml`

 * *Files identical despite different names*

### Comparing `ccpn_project_checker-0.1.5/src/project_checker/test_data/root_version_badly_formatted.ccpn/ccpnv3/memops/Implementation/root_version_badly_formatted.xml` & `ccpn_project_checker-0.1.6/src/project_checker/test_data/root_version_badly_formatted.ccpn/ccpnv3/memops/Implementation/root_version_badly_formatted.xml`

 * *Files identical despite different names*

### Comparing `ccpn_project_checker-0.1.5/src/project_checker/test_data/root_version_missing.ccpn/ccpnv3/ccp/lims/Sample/default+default_user_2024-02-24-15-54-35-583_00002.xml` & `ccpn_project_checker-0.1.6/src/project_checker/test_data/root_version_missing.ccpn/ccpnv3/ccp/lims/Sample/default+default_user_2024-02-24-15-54-35-583_00002.xml`

 * *Files identical despite different names*

### Comparing `ccpn_project_checker-0.1.5/src/project_checker/test_data/root_version_missing.ccpn/ccpnv3/ccp/nmr/Nmr/default+default_user_2024-02-24-15-54-35-583_00001.xml` & `ccpn_project_checker-0.1.6/src/project_checker/test_data/root_version_missing.ccpn/ccpnv3/ccp/nmr/Nmr/default+default_user_2024-02-24-15-54-35-583_00001.xml`

 * *Files identical despite different names*

### Comparing `ccpn_project_checker-0.1.5/src/project_checker/test_data/root_version_missing.ccpn/ccpnv3/ccpnmr/gui/Task/user+View+default_user_2024-02-24-15-54-35-583_00006.xml` & `ccpn_project_checker-0.1.6/src/project_checker/test_data/root_version_missing.ccpn/ccpnv3/ccpnmr/gui/Task/user+View+default_user_2024-02-24-15-54-35-583_00006.xml`

 * *Files identical despite different names*

### Comparing `ccpn_project_checker-0.1.5/src/project_checker/test_data/root_version_missing.ccpn/ccpnv3/ccpnmr/gui/Window/_ccp_nmr_Nmr_NmrProject___default___+default_user_2024-02-24-15-54-35-583_00005.xml` & `ccpn_project_checker-0.1.6/src/project_checker/test_data/root_version_missing.ccpn/ccpnv3/ccpnmr/gui/Window/_ccp_nmr_Nmr_NmrProject___default___+default_user_2024-02-24-15-54-35-583_00005.xml`

 * *Files identical despite different names*

### Comparing `ccpn_project_checker-0.1.5/src/project_checker/test_data/root_version_missing.ccpn/ccpnv3/memops/Implementation/root_version_missing.xml` & `ccpn_project_checker-0.1.6/src/project_checker/test_data/root_version_missing.ccpn/ccpnv3/memops/Implementation/root_version_missing.xml`

 * *Files identical despite different names*

### Comparing `ccpn_project_checker-0.1.5/src/project_checker/test_data/too_many_root_elements.ccpn/ccpnv3/ccp/lims/Sample/default+default_user_2024-02-24-15-54-35-583_00002.xml` & `ccpn_project_checker-0.1.6/src/project_checker/test_data/too_many_root_elements.ccpn/ccpnv3/ccp/lims/Sample/default+default_user_2024-02-24-15-54-35-583_00002.xml`

 * *Files identical despite different names*

### Comparing `ccpn_project_checker-0.1.5/src/project_checker/test_data/too_many_root_elements.ccpn/ccpnv3/ccp/nmr/Nmr/default+default_user_2024-02-24-15-54-35-583_00001.xml` & `ccpn_project_checker-0.1.6/src/project_checker/test_data/too_many_root_elements.ccpn/ccpnv3/ccp/nmr/Nmr/default+default_user_2024-02-24-15-54-35-583_00001.xml`

 * *Files identical despite different names*

### Comparing `ccpn_project_checker-0.1.5/src/project_checker/test_data/too_many_root_elements.ccpn/ccpnv3/ccpnmr/gui/Task/user+View+default_user_2024-02-24-15-54-35-583_00006.xml` & `ccpn_project_checker-0.1.6/src/project_checker/test_data/too_many_root_elements.ccpn/ccpnv3/ccpnmr/gui/Task/user+View+default_user_2024-02-24-15-54-35-583_00006.xml`

 * *Files identical despite different names*

### Comparing `ccpn_project_checker-0.1.5/src/project_checker/test_data/too_many_root_elements.ccpn/ccpnv3/ccpnmr/gui/Window/_ccp_nmr_Nmr_NmrProject___default___+default_user_2024-02-24-15-54-35-583_00005.xml` & `ccpn_project_checker-0.1.6/src/project_checker/test_data/too_many_root_elements.ccpn/ccpnv3/ccpnmr/gui/Window/_ccp_nmr_Nmr_NmrProject___default___+default_user_2024-02-24-15-54-35-583_00005.xml`

 * *Files identical despite different names*

### Comparing `ccpn_project_checker-0.1.5/src/project_checker/test_data/warn_projects/empty_good_project_extra_root_xml_files.ccpn/ccpnv3/ccp/lims/Sample/default+default_user_2024-02-24-15-54-35-583_00002.xml` & `ccpn_project_checker-0.1.6/src/project_checker/test_data/warn_projects/empty_good_project_extra_root_xml_files.ccpn/ccpnv3/ccp/lims/Sample/default+default_user_2024-02-24-15-54-35-583_00002.xml`

 * *Files identical despite different names*

### Comparing `ccpn_project_checker-0.1.5/src/project_checker/test_data/warn_projects/empty_good_project_extra_root_xml_files.ccpn/ccpnv3/ccp/nmr/Nmr/default+default_user_2024-02-24-15-54-35-583_00001.xml` & `ccpn_project_checker-0.1.6/src/project_checker/test_data/warn_projects/empty_good_project_extra_root_xml_files.ccpn/ccpnv3/ccp/nmr/Nmr/default+default_user_2024-02-24-15-54-35-583_00001.xml`

 * *Files identical despite different names*

### Comparing `ccpn_project_checker-0.1.5/src/project_checker/test_data/warn_projects/empty_good_project_extra_root_xml_files.ccpn/ccpnv3/ccpnmr/gui/Task/user+View+default_user_2024-02-24-15-54-35-583_00006.xml` & `ccpn_project_checker-0.1.6/src/project_checker/test_data/warn_projects/empty_good_project_extra_root_xml_files.ccpn/ccpnv3/ccpnmr/gui/Task/user+View+default_user_2024-02-24-15-54-35-583_00006.xml`

 * *Files identical despite different names*

### Comparing `ccpn_project_checker-0.1.5/src/project_checker/test_data/warn_projects/empty_good_project_extra_root_xml_files.ccpn/ccpnv3/ccpnmr/gui/Window/_ccp_nmr_Nmr_NmrProject___default___+default_user_2024-02-24-15-54-35-583_00005.xml` & `ccpn_project_checker-0.1.6/src/project_checker/test_data/warn_projects/empty_good_project_extra_root_xml_files.ccpn/ccpnv3/ccpnmr/gui/Window/_ccp_nmr_Nmr_NmrProject___default___+default_user_2024-02-24-15-54-35-583_00005.xml`

 * *Files identical despite different names*

### Comparing `ccpn_project_checker-0.1.5/src/project_checker/test_data/warn_projects/empty_good_project_extra_root_xml_files.ccpn/ccpnv3/memops/Implementation/empty_good_project_extra_root_xml_files.xml` & `ccpn_project_checker-0.1.6/src/project_checker/test_data/warn_projects/empty_good_project_extra_root_xml_files.ccpn/ccpnv3/memops/Implementation/empty_good_project_extra_root_xml_files.xml`

 * *Files identical despite different names*

### Comparing `ccpn_project_checker-0.1.5/src/project_checker/test_data/warn_projects/empty_good_project_extra_root_xml_files.ccpn/ccpnv3/memops/Implementation/empty_good_project_extra_root_xml_files_2.xml` & `ccpn_project_checker-0.1.6/src/project_checker/test_data/warn_projects/empty_good_project_extra_root_xml_files.ccpn/ccpnv3/memops/Implementation/empty_good_project_extra_root_xml_files_2.xml`

 * *Files identical despite different names*

### Comparing `ccpn_project_checker-0.1.5/src/project_checker/test_data/warn_projects/empty_good_project_extra_xml_files.ccpn/ccpnv3/ccp/lims/Sample/default+default_user_2024-02-24-15-54-35-583_00002.xml` & `ccpn_project_checker-0.1.6/src/project_checker/test_data/warn_projects/empty_good_project_extra_xml_files.ccpn/ccpnv3/ccp/lims/Sample/default+default_user_2024-02-24-15-54-35-583_00002.xml`

 * *Files identical despite different names*

### Comparing `ccpn_project_checker-0.1.5/src/project_checker/test_data/warn_projects/empty_good_project_extra_xml_files.ccpn/ccpnv3/ccp/nmr/Nmr/default+default_user_2024-02-24-15-54-35-583_00001.xml` & `ccpn_project_checker-0.1.6/src/project_checker/test_data/warn_projects/empty_good_project_extra_xml_files.ccpn/ccpnv3/ccp/nmr/Nmr/default+default_user_2024-02-24-15-54-35-583_00001.xml`

 * *Files identical despite different names*

### Comparing `ccpn_project_checker-0.1.5/src/project_checker/test_data/warn_projects/empty_good_project_extra_xml_files.ccpn/ccpnv3/ccpnmr/gui/Task/task_2.xml` & `ccpn_project_checker-0.1.6/src/project_checker/test_data/warn_projects/empty_good_project_extra_xml_files.ccpn/ccpnv3/ccpnmr/gui/Task/task_2.xml`

 * *Files identical despite different names*

### Comparing `ccpn_project_checker-0.1.5/src/project_checker/test_data/warn_projects/empty_good_project_extra_xml_files.ccpn/ccpnv3/ccpnmr/gui/Task/user+View+default_user_2024-02-24-15-54-35-583_00006.xml` & `ccpn_project_checker-0.1.6/src/project_checker/test_data/warn_projects/empty_good_project_extra_xml_files.ccpn/ccpnv3/ccpnmr/gui/Task/user+View+default_user_2024-02-24-15-54-35-583_00006.xml`

 * *Files identical despite different names*

### Comparing `ccpn_project_checker-0.1.5/src/project_checker/test_data/warn_projects/empty_good_project_extra_xml_files.ccpn/ccpnv3/ccpnmr/gui/Window/_ccp_nmr_Nmr_NmrProject___default___+default_user_2024-02-24-15-54-35-583_00005.xml` & `ccpn_project_checker-0.1.6/src/project_checker/test_data/warn_projects/empty_good_project_extra_xml_files.ccpn/ccpnv3/ccpnmr/gui/Window/_ccp_nmr_Nmr_NmrProject___default___+default_user_2024-02-24-15-54-35-583_00005.xml`

 * *Files identical despite different names*

### Comparing `ccpn_project_checker-0.1.5/src/project_checker/test_data/warn_projects/empty_good_project_extra_xml_files.ccpn/ccpnv3/memops/Implementation/empty_good_project_extra_xml_files.xml` & `ccpn_project_checker-0.1.6/src/project_checker/test_data/warn_projects/empty_good_project_extra_xml_files.ccpn/ccpnv3/memops/Implementation/empty_good_project_extra_xml_files.xml`

 * *Files identical despite different names*

### Comparing `ccpn_project_checker-0.1.5/src/project_checker/test_data/warn_projects/empty_good_project_with_empty_containers.ccpn/ccpnv3/ccp/lims/Sample/default+default_user_2024-02-24-15-54-35-583_00002.xml` & `ccpn_project_checker-0.1.6/src/project_checker/test_data/warn_projects/empty_good_project_with_empty_containers.ccpn/ccpnv3/ccp/lims/Sample/default+default_user_2024-02-24-15-54-35-583_00002.xml`

 * *Files identical despite different names*

### Comparing `ccpn_project_checker-0.1.5/src/project_checker/test_data/warn_projects/empty_good_project_with_empty_containers.ccpn/ccpnv3/ccp/nmr/Nmr/default+default_user_2024-02-24-15-54-35-583_00001.xml` & `ccpn_project_checker-0.1.6/src/project_checker/test_data/warn_projects/empty_good_project_with_empty_containers.ccpn/ccpnv3/ccp/nmr/Nmr/default+default_user_2024-02-24-15-54-35-583_00001.xml`

 * *Files identical despite different names*

### Comparing `ccpn_project_checker-0.1.5/src/project_checker/test_data/warn_projects/empty_good_project_with_empty_containers.ccpn/ccpnv3/ccpnmr/gui/Task/user+View+default_user_2024-02-24-15-54-35-583_00006.xml` & `ccpn_project_checker-0.1.6/src/project_checker/test_data/warn_projects/empty_good_project_with_empty_containers.ccpn/ccpnv3/ccpnmr/gui/Task/user+View+default_user_2024-02-24-15-54-35-583_00006.xml`

 * *Files identical despite different names*

### Comparing `ccpn_project_checker-0.1.5/src/project_checker/test_data/warn_projects/empty_good_project_with_empty_containers.ccpn/ccpnv3/ccpnmr/gui/Window/_ccp_nmr_Nmr_NmrProject___default___+default_user_2024-02-24-15-54-35-583_00005.xml` & `ccpn_project_checker-0.1.6/src/project_checker/test_data/warn_projects/empty_good_project_with_empty_containers.ccpn/ccpnv3/ccpnmr/gui/Window/_ccp_nmr_Nmr_NmrProject___default___+default_user_2024-02-24-15-54-35-583_00005.xml`

 * *Files identical despite different names*

### Comparing `ccpn_project_checker-0.1.5/src/project_checker/test_data/warn_projects/empty_good_project_with_empty_containers.ccpn/ccpnv3/memops/Implementation/empty_good_project_with_empty_containers.xml` & `ccpn_project_checker-0.1.6/src/project_checker/test_data/warn_projects/empty_good_project_with_empty_containers.ccpn/ccpnv3/memops/Implementation/empty_good_project_with_empty_containers.xml`

 * *Files identical despite different names*

### Comparing `ccpn_project_checker-0.1.5/src/project_checker/test_data/warn_projects/root_file_badly_formatted_time.ccpn/ccpnv3/ccp/lims/Sample/default+default_user_2024-02-24-15-54-35-583_00002.xml` & `ccpn_project_checker-0.1.6/src/project_checker/test_data/warn_projects/root_file_badly_formatted_time.ccpn/ccpnv3/ccp/lims/Sample/default+default_user_2024-02-24-15-54-35-583_00002.xml`

 * *Files identical despite different names*

### Comparing `ccpn_project_checker-0.1.5/src/project_checker/test_data/warn_projects/root_file_badly_formatted_time.ccpn/ccpnv3/ccp/nmr/Nmr/default+default_user_2024-02-24-15-54-35-583_00001.xml` & `ccpn_project_checker-0.1.6/src/project_checker/test_data/warn_projects/root_file_badly_formatted_time.ccpn/ccpnv3/ccp/nmr/Nmr/default+default_user_2024-02-24-15-54-35-583_00001.xml`

 * *Files identical despite different names*

### Comparing `ccpn_project_checker-0.1.5/src/project_checker/test_data/warn_projects/root_file_badly_formatted_time.ccpn/ccpnv3/ccpnmr/gui/Task/user+View+default_user_2024-02-24-15-54-35-583_00006.xml` & `ccpn_project_checker-0.1.6/src/project_checker/test_data/warn_projects/root_file_badly_formatted_time.ccpn/ccpnv3/ccpnmr/gui/Task/user+View+default_user_2024-02-24-15-54-35-583_00006.xml`

 * *Files identical despite different names*

### Comparing `ccpn_project_checker-0.1.5/src/project_checker/test_data/warn_projects/root_file_badly_formatted_time.ccpn/ccpnv3/ccpnmr/gui/Window/_ccp_nmr_Nmr_NmrProject___default___+default_user_2024-02-24-15-54-35-583_00005.xml` & `ccpn_project_checker-0.1.6/src/project_checker/test_data/warn_projects/root_file_badly_formatted_time.ccpn/ccpnv3/ccpnmr/gui/Window/_ccp_nmr_Nmr_NmrProject___default___+default_user_2024-02-24-15-54-35-583_00005.xml`

 * *Files identical despite different names*

### Comparing `ccpn_project_checker-0.1.5/src/project_checker/test_data/warn_projects/root_file_badly_formatted_time.ccpn/ccpnv3/memops/Implementation/root_file_badly_formatted_time.xml` & `ccpn_project_checker-0.1.6/src/project_checker/test_data/warn_projects/root_file_badly_formatted_time.ccpn/ccpnv3/memops/Implementation/root_file_badly_formatted_time.xml`

 * *Files identical despite different names*

### Comparing `ccpn_project_checker-0.1.5/src/project_checker/test_data/warn_projects/root_file_missing_time.ccpn/ccpnv3/ccp/lims/Sample/default+default_user_2024-02-24-15-54-35-583_00002.xml` & `ccpn_project_checker-0.1.6/src/project_checker/test_data/warn_projects/root_file_missing_time.ccpn/ccpnv3/ccp/lims/Sample/default+default_user_2024-02-24-15-54-35-583_00002.xml`

 * *Files identical despite different names*

### Comparing `ccpn_project_checker-0.1.5/src/project_checker/test_data/warn_projects/root_file_missing_time.ccpn/ccpnv3/ccp/nmr/Nmr/default+default_user_2024-02-24-15-54-35-583_00001.xml` & `ccpn_project_checker-0.1.6/src/project_checker/test_data/warn_projects/root_file_missing_time.ccpn/ccpnv3/ccp/nmr/Nmr/default+default_user_2024-02-24-15-54-35-583_00001.xml`

 * *Files identical despite different names*

### Comparing `ccpn_project_checker-0.1.5/src/project_checker/test_data/warn_projects/root_file_missing_time.ccpn/ccpnv3/ccpnmr/gui/Task/user+View+default_user_2024-02-24-15-54-35-583_00006.xml` & `ccpn_project_checker-0.1.6/src/project_checker/test_data/warn_projects/root_file_missing_time.ccpn/ccpnv3/ccpnmr/gui/Task/user+View+default_user_2024-02-24-15-54-35-583_00006.xml`

 * *Files identical despite different names*

### Comparing `ccpn_project_checker-0.1.5/src/project_checker/test_data/warn_projects/root_file_missing_time.ccpn/ccpnv3/ccpnmr/gui/Window/_ccp_nmr_Nmr_NmrProject___default___+default_user_2024-02-24-15-54-35-583_00005.xml` & `ccpn_project_checker-0.1.6/src/project_checker/test_data/warn_projects/root_file_missing_time.ccpn/ccpnv3/ccpnmr/gui/Window/_ccp_nmr_Nmr_NmrProject___default___+default_user_2024-02-24-15-54-35-583_00005.xml`

 * *Files identical despite different names*

### Comparing `ccpn_project_checker-0.1.5/src/project_checker/test_data/warn_projects/root_file_missing_time.ccpn/ccpnv3/memops/Implementation/root_file_missing_time.xml` & `ccpn_project_checker-0.1.6/src/project_checker/test_data/warn_projects/root_file_missing_time.ccpn/ccpnv3/memops/Implementation/root_file_missing_time.xml`

 * *Files identical despite different names*

### Comparing `ccpn_project_checker-0.1.5/src/project_checker/tests/api_test_data.py` & `ccpn_project_checker-0.1.6/src/project_checker/tests/api_test_data.py`

 * *Files identical despite different names*

### Comparing `ccpn_project_checker-0.1.5/src/project_checker/tests/api_test_data_internal.py` & `ccpn_project_checker-0.1.6/src/project_checker/tests/api_test_data_internal.py`

 * *Files identical despite different names*

### Comparing `ccpn_project_checker-0.1.5/src/project_checker/tests/test_api.py` & `ccpn_project_checker-0.1.6/src/project_checker/tests/test_api.py`

 * *Files identical despite different names*

### Comparing `ccpn_project_checker-0.1.5/src/project_checker/tests/test_cli.py` & `ccpn_project_checker-0.1.6/src/project_checker/tests/test_cli.py`

 * *Files identical despite different names*

### Comparing `ccpn_project_checker-0.1.5/src/project_checker/tests/testing_utils.py` & `ccpn_project_checker-0.1.6/src/project_checker/tests/testing_utils.py`

 * *Files identical despite different names*

### Comparing `ccpn_project_checker-0.1.5/pyproject.toml` & `ccpn_project_checker-0.1.6/pyproject.toml`

 * *Files 13% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 [project]
 name = "ccpn-project-checker"
-version = "0.1.5"
+version = "0.1.6"
 description = "A project checker for ccpn v3+ projects"
 authors = [
     { name = "varioustoxins", email = "garyt.and.sarahb@gmail.com" }
 ]
 dependencies = [
     "lxml>=5.2.0",
     "pytest>=8.1.1",
@@ -24,8 +24,8 @@
 managed = true
 dev-dependencies = []
 
 [tool.hatch.metadata]
 allow-direct-references = true
 
 [tool.hatch.build.targets.wheel]
-packages = ["src/ccpn_project_checker"]
+packages = ["src/project_checker"]
```

