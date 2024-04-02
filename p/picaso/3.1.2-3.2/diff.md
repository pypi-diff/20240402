# Comparing `tmp/picaso-3.1.2.tar.gz` & `tmp/picaso-3.2.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "picaso-3.1.2.tar", last modified: Thu Jul 27 06:06:42 2023, max compression
+gzip compressed data, was "picaso-3.2.tar", last modified: Tue Apr  2 07:51:12 2024, max compression
```

## Comparing `picaso-3.1.2.tar` & `picaso-3.2.tar`

### file list

```diff
@@ -1,37 +1,37 @@
-drwxr-xr-x   0 nbatalh1   (503) staff       (20)        0 2023-07-27 06:06:42.631588 picaso-3.1.2/
--rw-r--r--   0 nbatalh1   (503) staff       (20)    35141 2019-11-21 19:50:22.000000 picaso-3.1.2/LICENSE
--rw-r--r--   0 nbatalh1   (503) staff       (20)      717 2023-07-27 06:06:42.631832 picaso-3.1.2/PKG-INFO
--rw-r--r--   0 nbatalh1   (503) staff       (20)     9222 2023-03-24 18:45:38.000000 picaso-3.1.2/README.md
-drwxr-xr-x   0 nbatalh1   (503) staff       (20)        0 2023-07-27 06:06:42.625367 picaso-3.1.2/picaso/
--rwxr-xr-x   0 nbatalh1   (503) staff       (20)      188 2020-08-18 18:11:20.000000 picaso-3.1.2/picaso/__init__.py
--rw-r--r--   0 nbatalh1   (503) staff       (20)    41398 2023-07-27 06:00:56.000000 picaso-3.1.2/picaso/analyze.py
--rwxr-xr-x   0 nbatalh1   (503) staff       (20)    28553 2023-07-27 06:05:57.000000 picaso-3.1.2/picaso/atmsetup.py
--rwxr-xr-x   0 nbatalh1   (503) staff       (20)    16419 2022-10-25 17:12:52.000000 picaso-3.1.2/picaso/build_3d_input.py
--rwxr-xr-x   0 nbatalh1   (503) staff       (20)    10326 2022-10-25 17:12:52.000000 picaso-3.1.2/picaso/cia_interpolate.py
--rw-r--r--   0 nbatalh1   (503) staff       (20)    50616 2023-03-24 18:45:38.000000 picaso-3.1.2/picaso/climate.py
--rwxr-xr-x   0 nbatalh1   (503) staff       (20)    21239 2022-10-25 17:12:52.000000 picaso-3.1.2/picaso/deq_chem.py
--rwxr-xr-x   0 nbatalh1   (503) staff       (20)     5996 2022-10-25 17:12:52.000000 picaso-3.1.2/picaso/disco.py
--rwxr-xr-x   0 nbatalh1   (503) staff       (20)   123112 2023-07-26 21:49:17.000000 picaso-3.1.2/picaso/elements.py
--rw-r--r--   0 nbatalh1   (503) staff       (20)   169414 2023-03-24 18:45:38.000000 picaso-3.1.2/picaso/fluxes.py
--rwxr-xr-x   0 nbatalh1   (503) staff       (20)     1751 2022-10-25 17:12:52.000000 picaso-3.1.2/picaso/io_utils.py
--rwxr-xr-x   0 nbatalh1   (503) staff       (20)   288719 2023-07-26 21:49:17.000000 picaso-3.1.2/picaso/justdoit.py
--rwxr-xr-x   0 nbatalh1   (503) staff       (20)    80150 2023-07-26 21:49:17.000000 picaso-3.1.2/picaso/justplotit.py
--rwxr-xr-x   0 nbatalh1   (503) staff       (20)    65867 2023-07-17 22:26:27.000000 picaso-3.1.2/picaso/opacity_factory.py
--rwxr-xr-x   0 nbatalh1   (503) staff       (20)   118894 2023-07-26 21:49:17.000000 picaso-3.1.2/picaso/optics.py
--rwxr-xr-x   0 nbatalh1   (503) staff       (20)    28193 2022-08-19 21:57:10.000000 picaso-3.1.2/picaso/phasecurves.py
--rwxr-xr-x   0 nbatalh1   (503) staff       (20)    14066 2020-02-07 23:44:16.000000 picaso-3.1.2/picaso/rayleigh.py
--rw-r--r--   0 nbatalh1   (503) staff       (20)     4174 2022-10-25 17:12:52.000000 picaso-3.1.2/picaso/references.py
--rwxr-xr-x   0 nbatalh1   (503) staff       (20)     2993 2022-10-25 17:12:52.000000 picaso-3.1.2/picaso/run_opa_factory.py
--rwxr-xr-x   0 nbatalh1   (503) staff       (20)    10516 2023-03-24 18:45:38.000000 picaso-3.1.2/picaso/test.py
--rwxr-xr-x   0 nbatalh1   (503) staff       (20)     2481 2022-10-25 17:12:52.000000 picaso-3.1.2/picaso/test_optics.py
--rwxr-xr-x   0 nbatalh1   (503) staff       (20)     4880 2022-10-25 17:12:52.000000 picaso-3.1.2/picaso/vulcan.py
--rwxr-xr-x   0 nbatalh1   (503) staff       (20)     2577 2023-07-26 21:49:25.000000 picaso-3.1.2/picaso/wavelength.py
-drwxr-xr-x   0 nbatalh1   (503) staff       (20)        0 2023-07-27 06:06:42.631126 picaso-3.1.2/picaso.egg-info/
--rw-r--r--   0 nbatalh1   (503) staff       (20)      717 2023-07-27 06:06:42.000000 picaso-3.1.2/picaso.egg-info/PKG-INFO
--rw-r--r--   0 nbatalh1   (503) staff       (20)      675 2023-07-27 06:06:42.000000 picaso-3.1.2/picaso.egg-info/SOURCES.txt
--rw-r--r--   0 nbatalh1   (503) staff       (20)        1 2023-07-27 06:06:42.000000 picaso-3.1.2/picaso.egg-info/dependency_links.txt
--rw-r--r--   0 nbatalh1   (503) staff       (20)        1 2019-11-21 21:13:50.000000 picaso-3.1.2/picaso.egg-info/not-zip-safe
--rw-r--r--   0 nbatalh1   (503) staff       (20)      158 2023-07-27 06:06:42.000000 picaso-3.1.2/picaso.egg-info/requires.txt
--rw-r--r--   0 nbatalh1   (503) staff       (20)        7 2023-07-27 06:06:42.000000 picaso-3.1.2/picaso.egg-info/top_level.txt
--rw-r--r--   0 nbatalh1   (503) staff       (20)      767 2023-07-27 06:06:42.633452 picaso-3.1.2/setup.cfg
--rw-r--r--   0 nbatalh1   (503) staff       (20)     3216 2023-07-27 06:04:34.000000 picaso-3.1.2/setup.py
+drwxr-xr-x   0 nbatalh1   (503) staff       (20)        0 2024-04-02 07:51:12.788771 picaso-3.2/
+-rw-r--r--   0 nbatalh1   (503) staff       (20)    35141 2019-11-21 19:50:22.000000 picaso-3.2/LICENSE
+-rw-r--r--   0 nbatalh1   (503) staff       (20)     1117 2024-04-02 07:51:12.788370 picaso-3.2/PKG-INFO
+-rw-r--r--   0 nbatalh1   (503) staff       (20)    10507 2024-04-02 07:49:58.000000 picaso-3.2/README.md
+drwxr-xr-x   0 nbatalh1   (503) staff       (20)        0 2024-04-02 07:51:12.781265 picaso-3.2/picaso/
+-rwxr-xr-x   0 nbatalh1   (503) staff       (20)      188 2020-08-18 18:11:20.000000 picaso-3.2/picaso/__init__.py
+-rw-r--r--   0 nbatalh1   (503) staff       (20)    61170 2024-04-02 07:49:58.000000 picaso-3.2/picaso/analyze.py
+-rwxr-xr-x   0 nbatalh1   (503) staff       (20)    29344 2024-04-02 07:49:58.000000 picaso-3.2/picaso/atmsetup.py
+-rwxr-xr-x   0 nbatalh1   (503) staff       (20)    16419 2022-10-25 17:12:52.000000 picaso-3.2/picaso/build_3d_input.py
+-rwxr-xr-x   0 nbatalh1   (503) staff       (20)    10326 2022-10-25 17:12:52.000000 picaso-3.2/picaso/cia_interpolate.py
+-rw-r--r--   0 nbatalh1   (503) staff       (20)    53641 2024-04-02 07:49:58.000000 picaso-3.2/picaso/climate.py
+-rwxr-xr-x   0 nbatalh1   (503) staff       (20)    21587 2024-04-02 07:49:58.000000 picaso-3.2/picaso/deq_chem.py
+-rwxr-xr-x   0 nbatalh1   (503) staff       (20)     5996 2024-01-26 20:14:27.000000 picaso-3.2/picaso/disco.py
+-rwxr-xr-x   0 nbatalh1   (503) staff       (20)   123055 2024-04-02 07:49:58.000000 picaso-3.2/picaso/elements.py
+-rw-r--r--   0 nbatalh1   (503) staff       (20)   174137 2024-04-02 07:49:58.000000 picaso-3.2/picaso/fluxes.py
+-rwxr-xr-x   0 nbatalh1   (503) staff       (20)     1751 2022-10-25 17:12:52.000000 picaso-3.2/picaso/io_utils.py
+-rwxr-xr-x   0 nbatalh1   (503) staff       (20)   291082 2024-04-02 07:49:58.000000 picaso-3.2/picaso/justdoit.py
+-rwxr-xr-x   0 nbatalh1   (503) staff       (20)    83226 2024-04-02 07:49:58.000000 picaso-3.2/picaso/justplotit.py
+-rwxr-xr-x   0 nbatalh1   (503) staff       (20)    65867 2023-09-02 01:26:32.000000 picaso-3.2/picaso/opacity_factory.py
+-rwxr-xr-x   0 nbatalh1   (503) staff       (20)   119874 2024-04-02 07:49:58.000000 picaso-3.2/picaso/optics.py
+-rwxr-xr-x   0 nbatalh1   (503) staff       (20)    28193 2022-08-19 21:57:10.000000 picaso-3.2/picaso/phasecurves.py
+-rwxr-xr-x   0 nbatalh1   (503) staff       (20)    18719 2024-04-02 07:49:58.000000 picaso-3.2/picaso/photochem.py
+-rwxr-xr-x   0 nbatalh1   (503) staff       (20)    14066 2020-02-07 23:44:16.000000 picaso-3.2/picaso/rayleigh.py
+-rw-r--r--   0 nbatalh1   (503) staff       (20)     3838 2024-04-02 07:49:58.000000 picaso-3.2/picaso/references.py
+-rwxr-xr-x   0 nbatalh1   (503) staff       (20)     2993 2022-10-25 17:12:52.000000 picaso-3.2/picaso/run_opa_factory.py
+-rwxr-xr-x   0 nbatalh1   (503) staff       (20)    10642 2024-04-02 07:49:58.000000 picaso-3.2/picaso/test.py
+-rwxr-xr-x   0 nbatalh1   (503) staff       (20)     2481 2022-10-25 17:12:52.000000 picaso-3.2/picaso/test_optics.py
+-rwxr-xr-x   0 nbatalh1   (503) staff       (20)     2553 2024-04-02 07:49:58.000000 picaso-3.2/picaso/wavelength.py
+drwxr-xr-x   0 nbatalh1   (503) staff       (20)        0 2024-04-02 07:51:12.786822 picaso-3.2/picaso.egg-info/
+-rw-r--r--   0 nbatalh1   (503) staff       (20)     1117 2024-04-02 07:51:12.000000 picaso-3.2/picaso.egg-info/PKG-INFO
+-rw-r--r--   0 nbatalh1   (503) staff       (20)      678 2024-04-02 07:51:12.000000 picaso-3.2/picaso.egg-info/SOURCES.txt
+-rw-r--r--   0 nbatalh1   (503) staff       (20)        1 2024-04-02 07:51:12.000000 picaso-3.2/picaso.egg-info/dependency_links.txt
+-rw-r--r--   0 nbatalh1   (503) staff       (20)        1 2019-11-21 21:13:50.000000 picaso-3.2/picaso.egg-info/not-zip-safe
+-rw-r--r--   0 nbatalh1   (503) staff       (20)      162 2024-04-02 07:51:12.000000 picaso-3.2/picaso.egg-info/requires.txt
+-rw-r--r--   0 nbatalh1   (503) staff       (20)        7 2024-04-02 07:51:12.000000 picaso-3.2/picaso.egg-info/top_level.txt
+-rw-r--r--   0 nbatalh1   (503) staff       (20)      767 2024-04-02 07:51:12.789942 picaso-3.2/setup.cfg
+-rw-r--r--   0 nbatalh1   (503) staff       (20)     3219 2024-04-02 07:49:58.000000 picaso-3.2/setup.py
```

### Comparing `picaso-3.1.2/LICENSE` & `picaso-3.2/LICENSE`

 * *Files identical despite different names*

### Comparing `picaso-3.1.2/README.md` & `picaso-3.2/README.md`

 * *Files 4% similar despite different names*

```diff
@@ -34,15 +34,15 @@
 ```
 @all-contributors please add @<username> for <contributions>
 ```
 
 ## Contributors
 
 <!-- ALL-CONTRIBUTORS-BADGE:START - Do not remove or modify this section -->
-[![All Contributors](https://img.shields.io/badge/all_contributors-14-orange.svg?style=flat-square)](#contributors-)
+[![All Contributors](https://img.shields.io/badge/all_contributors-17-orange.svg?style=flat-square)](#contributors-)
 <!-- ALL-CONTRIBUTORS-BADGE:END -->
 
 Thanks goes to these wonderful people ([emoji key](https://allcontributors.org/docs/en/emoji-key)):
 <!-- ALL-CONTRIBUTORS-LIST:START - Do not remove or modify this section -->
 <!-- prettier-ignore-start -->
 <!-- markdownlint-disable -->
 <table>
@@ -61,14 +61,19 @@
       <td align="center" valign="top" width="14.28%"><a href="https://github.com/MartianColonist"><img src="https://avatars.githubusercontent.com/u/22718554?v=4?s=100" width="100px;" alt="Ryan MacDonald"/><br /><sub><b>Ryan MacDonald</b></sub></a><br /><a href="https://github.com/natashabatalha/picaso/issues?q=author%3AMartianColonist" title="Bug reports">🐛</a></td>
       <td align="center" valign="top" width="14.28%"><a href="https://epl.carnegiescience.edu/people/peter-gao"><img src="https://avatars.githubusercontent.com/u/20616506?v=4?s=100" width="100px;" alt="Peter Gao"/><br /><sub><b>Peter Gao</b></sub></a><br /><a href="https://github.com/natashabatalha/picaso/issues?q=author%3Asirpetergao" title="Bug reports">🐛</a></td>
       <td align="center" valign="top" width="14.28%"><a href="https://github.com/nklewis"><img src="https://avatars.githubusercontent.com/u/16822846?v=4?s=100" width="100px;" alt="Nikole Lewis"/><br /><sub><b>Nikole Lewis</b></sub></a><br /><a href="https://github.com/natashabatalha/picaso/issues?q=author%3Anklewis" title="Bug reports">🐛</a> <a href="#mentoring-nklewis" title="Mentoring">🧑‍🏫</a></td>
       <td align="center" valign="top" width="14.28%"><a href="https://github.com/exoBD"><img src="https://avatars.githubusercontent.com/u/38989139?v=4?s=100" width="100px;" alt="Mark Marley"/><br /><sub><b>Mark Marley</b></sub></a><br /><a href="#mentoring-exobd" title="Mentoring">🧑‍🏫</a> <a href="#ideas-exobd" title="Ideas, Planning, & Feedback">🤔</a> <a href="#research-exobd" title="Research">🔬</a></td>
       <td align="center" valign="top" width="14.28%"><a href="https://github.com/drtkat"><img src="https://avatars.githubusercontent.com/u/10516244?v=4?s=100" width="100px;" alt="Tiffany Kataria"/><br /><sub><b>Tiffany Kataria</b></sub></a><br /><a href="https://github.com/natashabatalha/picaso/issues?q=author%3Adrtkat" title="Bug reports">🐛</a> <a href="#mentoring-drtkat" title="Mentoring">🧑‍🏫</a></td>
       <td align="center" valign="top" width="14.28%"><a href="https://github.com/jjfplanet"><img src="https://avatars.githubusercontent.com/u/42284609?v=4?s=100" width="100px;" alt="jjfplanet"/><br /><sub><b>jjfplanet</b></sub></a><br /><a href="#ideas-jjfplanet" title="Ideas, Planning, & Feedback">🤔</a> <a href="#mentoring-jjfplanet" title="Mentoring">🧑‍🏫</a> <a href="#fundingFinding-jjfplanet" title="Funding Finding">🔍</a></td>
     </tr>
+    <tr>
+      <td align="center" valign="top" width="14.28%"><a href="https://github.com/Ziva18t"><img src="https://avatars.githubusercontent.com/u/107640508?v=4?s=100" width="100px;" alt="Ziva18t"/><br /><sub><b>Ziva18t</b></sub></a><br /><a href="https://github.com/natashabatalha/picaso/commits?author=Ziva18t" title="Code">💻</a></td>
+      <td align="center" valign="top" width="14.28%"><a href="https://jamesmang.wixsite.com/jamesmang"><img src="https://avatars.githubusercontent.com/u/33335954?v=4?s=100" width="100px;" alt="James"/><br /><sub><b>James</b></sub></a><br /><a href="https://github.com/natashabatalha/picaso/commits?author=James-Mang" title="Code">💻</a> <a href="#research-James-Mang" title="Research">🔬</a></td>
+      <td align="center" valign="top" width="14.28%"><a href="https://github.com/astrocaroline"><img src="https://avatars.githubusercontent.com/u/10456842?v=4?s=100" width="100px;" alt="astrocaroline"/><br /><sub><b>astrocaroline</b></sub></a><br /><a href="#mentoring-astrocaroline" title="Mentoring">🧑‍🏫</a> <a href="#ideas-astrocaroline" title="Ideas, Planning, & Feedback">🤔</a> <a href="#fundingFinding-astrocaroline" title="Funding Finding">🔍</a> <a href="#research-astrocaroline" title="Research">🔬</a></td>
+    </tr>
   </tbody>
 </table>
 
 <!-- markdownlint-restore -->
 <!-- prettier-ignore-end -->
 
 <!-- ALL-CONTRIBUTORS-LIST:END -->
```

#### html2text {}

```diff
@@ -28,26 +28,30 @@
 conda environments you can read our instructions here: https://
 natashabatalha.github.io/picaso/contribution.html Additionally all contributors
 agree to adhere to this project's [`code of conduct`](https://github.com/
 natashabatalha/picaso/blob/master/code_of_conduct.md) Anyone is free to use the
 [contributor bot to add their contribution](https://allcontributors.org/docs/
 en/bot/usage). Simply comment on an issue or pull request with: ``` @all-
 contributors please add @ for ``` ## Contributors [![All Contributors](https://
-img.shields.io/badge/all_contributors-14-orange.svg?style=flat-square)]
+img.shields.io/badge/all_contributors-17-orange.svg?style=flat-square)]
 (#contributors-) Thanks goes to these wonderful people ([emoji key](https://
 allcontributors.org/docs/en/emoji-key)):
- _[_N_a_t_a_s_h_a   _[_R_o_m_a_n_ _S_t_. _[_K_a_p_p_i_b_w_]  _[_L_a_u_r_a_ _C_.     _[_E_h_s_a_n    _[_C_a_o_i_m_h_e    _[_S_a_g_n_i_c_k
- _B_a_t_a_l_h_a_]    _G_e_r_a_r_d_]    _KK_aa_pp_pp_ii_bb_ww   _M_a_y_o_r_g_a_]      _G_h_a_r_i_b_-    _R_o_o_n_e_y_]   _M_u_k_h_e_r_j_e_e_]
-  _NN_aa_tt_aa_ss_hh_aa   _RR_oo_mm_aa_nn_ _SS_tt_..  _ð___ _ð___  _LL_aa_uu_rr_aa_ _CC_..      _N_e_z_h_a_d_]    _CC_aa_oo_ii_mm_hh_ee     _SS_aa_gg_nn_ii_cc_kk
-  _BB_aa_tt_aa_ll_hh_aa     _GG_ee_rr_aa_rr_dd               _MM_aa_yy_oo_rr_gg_aa       _EE_hh_ss_aa_nn     _RR_oo_oo_nn_ee_yy     _MM_uu_kk_hh_ee_rr_jj_ee_ee
-   _ð___»        _ð___»               _ð___ _ð___»     _GG_hh_aa_rr_ii_bb_--   _ð___¬ _ð___»   _ð___¬ _ð___»
-_ð__§__â___ð___«                                     _NN_ee_zz_hh_aa_dd
-   _ð___§                                          _ð___£
-    _[_N_i_n_a     _[_R_y_a_n     _[_P_e_t_e_r     _[_N_i_k_o_l_e      _[_M_a_r_k     _[_T_i_f_f_a_n_y   _[_j_j_f_p_l_a_n_e_t_]
-   _R_o_b_b_i_n_s  _M_a_c_D_o_n_a_l_d_]   _G_a_o_]      _L_e_w_i_s_]      _M_a_r_l_e_y_]    _K_a_t_a_r_i_a_]    _jj_jj_ff_pp_ll_aa_nn_ee_tt
-   _B_l_a_n_c_h_]     _RR_yy_aa_nn    _PP_ee_tt_ee_rr_ _GG_aa_oo   _NN_ii_kk_oo_ll_ee    _MM_aa_rr_kk_ _MM_aa_rr_ll_ee_yy   _TT_ii_ff_ff_aa_nn_yy      _ð__¤_
-    _NN_ii_nn_aa    _MM_aa_cc_DD_oo_nn_aa_ll_dd    _ð___       _LL_ee_ww_ii_ss    _ð__§__â___ð___«   _KK_aa_tt_aa_rr_ii_aa   _ð__§__â___ð___«
-   _RR_oo_bb_bb_ii_nn_ss     _ð___                 _ð___      _ð__¤_ _ð___¬     _ð___        _ð___
-   _BB_ll_aa_nn_cc_hh                        _ð__§__â___ð___«             _ð__§__â___ð___«
+ _[_N_a_t_a_s_h_a   _[_R_o_m_a_n_ _S_t_.     _[_K_a_p_p_i_b_w_]    _[_L_a_u_r_a_ _C_.     _[_E_h_s_a_n    _[_C_a_o_i_m_h_e    _[_S_a_g_n_i_c_k
+ _B_a_t_a_l_h_a_]    _G_e_r_a_r_d_]        _KK_aa_pp_pp_ii_bb_ww     _M_a_y_o_r_g_a_]      _G_h_a_r_i_b_-    _R_o_o_n_e_y_]   _M_u_k_h_e_r_j_e_e_]
+  _NN_aa_tt_aa_ss_hh_aa   _RR_oo_mm_aa_nn_ _SS_tt_..      _ð___ _ð___    _LL_aa_uu_rr_aa_ _CC_..      _N_e_z_h_a_d_]    _CC_aa_oo_ii_mm_hh_ee     _SS_aa_gg_nn_ii_cc_kk
+  _BB_aa_tt_aa_ll_hh_aa     _GG_ee_rr_aa_rr_dd                     _MM_aa_yy_oo_rr_gg_aa       _EE_hh_ss_aa_nn     _RR_oo_oo_nn_ee_yy     _MM_uu_kk_hh_ee_rr_jj_ee_ee
+   _ð___»        _ð___»                     _ð___ _ð___»     _GG_hh_aa_rr_ii_bb_--   _ð___¬ _ð___»   _ð___¬ _ð___»
+_ð__§__â___ð___«                                           _NN_ee_zz_hh_aa_dd
+   _ð___§                                                _ð___£
+    _[_N_i_n_a     _[_R_y_a_n       _[_P_e_t_e_r_ _G_a_o_]    _[_N_i_k_o_l_e      _[_M_a_r_k     _[_T_i_f_f_a_n_y   _[_j_j_f_p_l_a_n_e_t_]
+   _R_o_b_b_i_n_s  _M_a_c_D_o_n_a_l_d_]     _PP_ee_tt_ee_rr_ _GG_aa_oo     _L_e_w_i_s_]      _M_a_r_l_e_y_]    _K_a_t_a_r_i_a_]    _jj_jj_ff_pp_ll_aa_nn_ee_tt
+   _B_l_a_n_c_h_]     _RR_yy_aa_nn          _ð___        _NN_ii_kk_oo_ll_ee    _MM_aa_rr_kk_ _MM_aa_rr_ll_ee_yy   _TT_ii_ff_ff_aa_nn_yy      _ð__¤_
+    _NN_ii_nn_aa    _MM_aa_cc_DD_oo_nn_aa_ll_dd                     _LL_ee_ww_ii_ss    _ð__§__â___ð___«   _KK_aa_tt_aa_rr_ii_aa   _ð__§__â___ð___«
+   _RR_oo_bb_bb_ii_nn_ss     _ð___                       _ð___      _ð__¤_ _ð___¬     _ð___        _ð___
+   _BB_ll_aa_nn_cc_hh                              _ð__§__â___ð___«             _ð__§__â___ð___«
     _ð___»
+ _[_Z_i_v_a_1_8_t_]   _[_J_a_m_e_s_]   _[_a_s_t_r_o_c_a_r_o_l_i_n_e_]
+  _ZZ_ii_vv_aa_11_88_tt     _JJ_aa_mm_ee_ss     _aa_ss_tt_rr_oo_cc_aa_rr_oo_ll_ii_nn_ee
+   _ð___»     _ð___» _ð___¬    _ð__§__â___ð___«
+                       _ð__¤_ _ð___ _ð___¬
 [![Contributor Covenant](https://img.shields.io/badge/Contributor%20Covenant-
 2.1-4baaaa.svg)](code_of_conduct.md)
```

### Comparing `picaso-3.1.2/picaso/atmsetup.py` & `picaso-3.2/picaso/atmsetup.py`

 * *Files 5% similar despite different names*

```diff
@@ -84,15 +84,15 @@
         #get chemistry input from configuration
         #SET DIMENSIONALITY
         self.dimension = '3d'
         latitude, longitude = self.latitude*180/np.pi, self.longitude*180/np.pi
 
         read_3d = self.input['atmosphere']['profile'] #huge dictionary with [lat][lon][bundle]
 
-        self.c.nlevel = self.input['atmosphere']['profile'].dims['pressure']
+        self.c.nlevel = self.input['atmosphere']['profile'].sizes['pressure']
         self.c.nlayer = self.c.nlevel - 1  
         ng , nt = self.c.ngangle, self.c.ntangle
 
         self.level['temperature'] = np.zeros((self.c.nlevel, ng, nt))
         self.level['pressure'] = np.zeros((self.c.nlevel, ng, nt))
         self.level['electrons'] = np.zeros((self.c.nlevel, ng, nt))
 
@@ -356,14 +356,15 @@
         self.layer['mmw'] = 0.5*(weighted_matrix[:-1]+weighted_matrix[1:])
 
         return 
 
     def get_density(self):
         """
         Calculates density of atmospheres used on TP profile: LEVEL
+        units of cm-3
         """
         self.level['den'] = self.level['pressure'] / (self.c.k_b * self.level['temperature']) 
         return
 
     def get_altitude(self, p_reference=1,constant_gravity=False):
         """
         Calculates z and gravity  
@@ -522,15 +523,15 @@
         #3D with clouds
         elif ((self.dimension=='3d') & (not isinstance(self.input_wno, type(None)))):
             self.c.input_npts_wave = len(self.input_wno)
             latitude, longitude = self.latitude*180/np.pi, self.longitude*180/np.pi
             cld_input = self.input['clouds']['profile'] 
             cld_input = cld_input.sortby('wno').sortby('pressure')
             if regrid: cld_input = cld_input.interp(wno = wno)
-            if [i for i in cld_input.dims] != ["pressure","wno","lon", "lat"]:
+            if [i for i in cld_input.sizes] != ["pressure","wno","lon", "lat"]:
                 opd = cld_input['opd'].transpose("pressure","wno","lon", "lat").values
                 g0 = cld_input['g0'].transpose("pressure","wno","lon", "lat").values
                 w0 = cld_input['w0'].transpose("pressure","wno","lon", "lat").values
             else: 
                 opd = cld_input['opd'].values
                 g0 = cld_input['g0'].values
                 w0 = cld_input['w0'].values                
@@ -614,14 +615,21 @@
         df['taugas'] = self.taugas
         df['tauray'] = self.tauray
         df['taucld'] = self.taucld
 
         df['level'] = {}
         df['level']['pressure'] = self.level['pressure']/ self.c.pconv #bars
         df['level']['temperature'] = self.level['temperature']
+        
+        #return the level fluxes if the user requests that particular output
+        if self.get_lvl_flux:
+            if not isinstance(getattr(self,'lvl_output_thermal',None), type(None)):
+                df['level']['thermal_fluxes'] = self.lvl_output_thermal
+            if not isinstance(getattr(self,'lvl_output_reflected',None), type(None)):    
+                df['level']['reflected_fluxes'] = self.lvl_output_reflected
 
         df['latitude'] = self.latitude
         df['longitude'] = self.longitude
 
         df['star'] = {}
         df['star']['flux_unit'] = 'erg/cm2/s/cm'
         
@@ -649,14 +657,23 @@
         try: 
             x = self.flux_at_top
             df['thermal_unit'] = 'erg/cm2/s/cm'
             df['thermal_3d'] = x
         except:
             pass
 
+        try: 
+            x = self.flux_layers
+            df['layer']['flux_minus'] = self.flux_layers[0]
+            df['layer']['flux_plus'] = self.flux_layers[1]
+            df['layer']['flux_minus_mdpt'] = self.flux_layers[2]
+            df['layer']['flux_plus_mdpt'] = self.flux_layers[3]
+        except:
+            pass
+
         return df
 
 def convert_to_simple(iso_name):
     """
     Converts iso name (e.g. 13C-16O2 to CO2)
     Returns same name if not (e.g. CO2 gives CO2)
     """
```

### Comparing `picaso-3.1.2/picaso/build_3d_input.py` & `picaso-3.2/picaso/build_3d_input.py`

 * *Files identical despite different names*

### Comparing `picaso-3.1.2/picaso/cia_interpolate.py` & `picaso-3.2/picaso/cia_interpolate.py`

 * *Files identical despite different names*

### Comparing `picaso-3.1.2/picaso/climate.py` & `picaso-3.2/picaso/climate.py`

 * *Files 4% similar despite different names*

```diff
@@ -1,16 +1,19 @@
 import numpy as np 
 import warnings
 from numba import jit, vectorize
 from numpy import exp, zeros, where, sqrt, cumsum , pi, outer, sinh, cosh, min, dot, array,log,log10
-from .fluxes import get_reflected_1d, get_thermal_1d_gfluxi,get_thermal_1d,get_reflected_1d_gfluxv
+from .fluxes import get_reflected_1d,get_thermal_1d
+#from .fluxes import get_thermal_1d_newclima, get_thermal_1d_gfluxi,get_reflected_1d_gfluxv #deprecated
 from .atmsetup import ATMSETUP
 from .optics import compute_opacity
 from .disco import compress_thermal
 
+#testing error tracker
+# from loguru import logger 
 
 @jit(nopython=True, cache=True)
 def did_grad_cp( t, p, t_table, p_table, grad, cp, calc_type):
     """
     Parameters
     ----------
     t : float
@@ -160,14 +163,18 @@
     if (value <= array[0]): # if value lower than first point
         jl=0
     elif (value >= array[-1]): # if value higher than first point
         jl= n-1
     
     return jl
 
+
+
+
+
 @jit(nopython=True, cache=True)
 def mat_sol(a, nlevel, nstrat, dflux):
     """
     Parameters
     ----------
     A : array
         Matrix to be decomposed dimension nlevel*nlevel
@@ -224,15 +231,15 @@
 
     for i in range(n):
         aamax=0.0
         for j in range(n):
             if abs(a[i,j]) > aamax:
                 aamax=abs(a[i,j])
         if aamax == 0.0:
-        	raise ValueError("Array is singular, cannot be decomposed")
+        	raise ValueError("Array is singular, cannot be decomposed in n:" + str(n))
         vv[i]=1.0/aamax  
 
     for j in range(n):
         for i in range(j):
             sum= a[i,j]
             for k in range(i):
                 sum=sum-a[i,k]*a[k,j]
@@ -315,21 +322,23 @@
             sum=sum-a[i,j]*b[j]
         
         b[i]=sum/a[i,i]
         
     
     return b
 
+# @logger.catch # Add this to track errors
 @jit(nopython=True, cache=True)
 def t_start(nofczns,nstr,it_max,conv,x_max_mult, 
             rfaci, rfacv, nlevel, temp, pressure, p_table, t_table, 
             grad, cp, tidal, tmin,tmax, dwni , bb , y2, tp, DTAU, TAU, W0, COSB, 
             ftau_cld, ftau_ray,GCOS2, DTAU_OG, TAU_OG, W0_OG, COSB_OG, W0_no_raman , surf_reflect, ubar0,ubar1,
             cos_theta, FOPI, single_phase,multi_phase,frac_a,frac_b,frac_c,
-            constant_back,constant_forward, tridiagonal , wno,nwno,ng,nt, ngauss, gauss_wts, save_profile, all_profiles):
+            constant_back,constant_forward,  wno,nwno,ng,nt,gweight,tweight, ngauss, gauss_wts, save_profile, all_profiles,
+            verbose=1):
     """
     Module to iterate on the level TP profile to make the Net Flux as close to 0.
     Opacities/chemistry are not updated while iterating in this module.
     Parameters
     ----------
     nofczns : int
         # of convective zones 
@@ -376,14 +385,17 @@
         Spectral interval corrections (dimension= nwvno)   
     bb : array
         Array of BB fluxes used in RT
     y2 : array
         Output of set_bb function in fluxes.py
     tp : array
         Output of set_bb function in fluxes.py
+    verbose : int
+        If verbose=0, nothing will print out
+        If verbose=1, everything will print out during the run, 
     
     Returns
     -------
     array 
         Temperature array and lapse ratio array if converged
         else Temperature array twice
     """
@@ -397,35 +409,37 @@
     #Climate default is to run both reflected and thermal. Though sometimes, in most cases we only want thermal.
     eps=1e-4
 
     n_top_r=nstr[0]-1
 
     # here are other  convergence and tolerance criterias
 
-    step_max = 0.03e0 # scaled maximum step size in line searches
+    step_max = 0.01e0 # scaled maximum step size in line searches
     alf = 1.e-4    # ? 
     alam2 = 0.0   # ? 
     tolmin=1.e-5   # ?
     tolf = 5e-3    # tolerance in fractional Flux we are aiming for
-    tolx = tolf    # tolerance in fractional T change we are aiming for
+    tolx = 5e-3    # tolerance in fractional T change we are aiming for
 
     #both reflected and thermal
-    flux_net_v_layer_full, flux_net_v_full, flux_plus_v_full, flux_minus_v_full , flux_net_ir_layer_full, flux_net_ir_full, flux_plus_ir_full, flux_minus_ir_full = climate(pressure, temp, dwni, bb , y2, tp, tmin, tmax, DTAU, TAU, W0, 
+    #neb this double true in the first call to reflected light needs to be changed
+    if rfacv==0:compute_reflected=False
+    else:compute_reflected=True
+    flux_net_v_layer_full, flux_net_v_full, flux_plus_v_full, flux_minus_v_full , flux_net_ir_layer_full, flux_net_ir_full, flux_plus_ir_full, flux_minus_ir_full = get_fluxes(pressure, temp, dwni, bb , y2, tp, tmin, tmax, DTAU, TAU, W0, 
             COSB,ftau_cld, ftau_ray,GCOS2, DTAU_OG, TAU_OG, W0_OG, COSB_OG, W0_no_raman , surf_reflect, 
-            ubar0,ubar1,cos_theta, FOPI, single_phase,multi_phase,frac_a,frac_b,frac_c,constant_back,constant_forward, tridiagonal , 
-            wno,nwno,ng,nt, nlevel, ngauss, gauss_wts,True, True)#True for reflected, True for thermal
+            ubar0,ubar1,cos_theta, FOPI, single_phase,multi_phase,frac_a,frac_b,frac_c,constant_back,constant_forward, 
+            wno,nwno,ng,nt, gweight,tweight, nlevel, ngauss, gauss_wts,compute_reflected, True)#True for reflected, True for thermal
 
     # extract visible fluxes
     flux_net_v_layer = flux_net_v_layer_full[0,0,:]  #fmnetv
     flux_net_v = flux_net_v_full[0,0,:]#fnetv
     flux_plus_v =  flux_plus_v_full[0,0,:,:]
     flux_minus_v = flux_minus_v_full[0,0,:,:]
 
     # extract ir fluxes
-
     flux_net_ir_layer = flux_net_ir_layer_full[:] #fmneti
     flux_net_ir = flux_net_ir_full[:]     #fneti
     flux_plus_ir = flux_plus_ir_full[:,:]  
     flux_minus_ir = flux_minus_ir_full[:,:]
     
    
     
@@ -433,26 +447,30 @@
     flux_net=np.zeros(shape=(nlevel))
     flux_net_midpt=np.zeros(shape=(nlevel))
     dflux=np.zeros(shape=(nlevel))
     f_vec=np.zeros(shape=(nlevel)) #fvec
     p=np.zeros(shape=(nlevel)) #p
     g=np.zeros(shape=(nlevel))
     
-    #--SM-- jacobian?
+    # jacobian of zeros
     A= np.zeros(shape=(nlevel,nlevel)) 
     
 
     
     for its in range(it_max):
         
         # the total net flux = optical + ir + tidal component
         
         flux_net = rfaci* flux_net_ir + rfacv* flux_net_v +tidal #fnet
         flux_net_midpt = rfaci* flux_net_ir_layer + rfacv* flux_net_v_layer +tidal #fmnet
         
+        #print('flux_net_midpt',flux_net_midpt)
+
+        #raise Exception ('stop in tstart')
+
         beta= temp.copy() # beta vector
         
        
         # store old fluxes and temp before iteration
         # do not store the ir+vis flux because we are going to perturb only thermal structure
 
         
@@ -523,26 +541,32 @@
             nao += n_bot_a - n_strt_a
 
         
         f = 0.5*sum # used in linesearch, defined in NR function fmin
 
         # test if we are already at a root
         if (test/abs(tidal[0])) < 0.01*tolf :
-            print(" We are already at a root, tolf , test = ",0.01*tolf,", ",test/abs(tidal[0]))
+            if verbose: print(" We are already at a root, tolf , test = ",0.01*tolf,", ",test/abs(tidal[0]))
             flag_converge = 2
             dtdp=np.zeros(shape=(nlevel-1))
             for j in range(nlevel -1):
                 dtdp[j] = (log( temp[j]) - log( temp[j+1]))/(log(pressure[j]) - log(pressure[j+1]))
             
             return   temp,  dtdp, flag_converge, flux_net_ir, flux_plus_ir[0,:], all_profiles
             
         
-        # define maximum T step size
-        step_max *= max(sqrt(sum_1),n_total*1.0)
-
+        # NEB NOTE about step max 
+        # In the original fortran code this was originally 
+        # step_max = step_max_tolerance*max(sqrt(sum_1),n_total*1.0) #where step_max_tolerance=0.03
+        # however when this was fixed, the code was progressing very slowly 
+        # therefore, we are keeping this in the code for now 
+        # the result of this is that there are sometimes large temperature 
+        # steps that might be problematic for edge cases that get too hot or too cold 
+        step_max *= max(sqrt(sum_1),n_total*1.0)#step_max_tolerance*
+        #if verbose: print('maximum scaled step size',step_max, n_total, sum_1, its)
         no =n_top_r
         
         i_count= 1 #icount
         
         flag_no = 0
         if no < 0 :
             no_temporary = no
@@ -565,15 +589,16 @@
         # +1 to include last element
             for jm in range(n_top, n_strt+1):
 
                 # chose perturbation for each level
 
                 i_count += 1
 
-                del_t = eps * temp_old[jm] # perturbation
+                #eps is just a tolerance value currently fixed at 1e-4
+                del_t = max(eps * temp_old[jm], 3.0) # perturbation
 
                 beta[jm] += del_t # perturb
 
                 
                 # now reconstruct Temp profile
 
                 for nb in range(0, 3*nofczns, 3):
@@ -604,18 +629,18 @@
                         temp[j1]= exp(log(temp[j1-1]) + grad_x*(log(pressure[j1]) - log(pressure[j1-1])))
                 
                 
 
                 # temperature has been perturbed
                 # now recalculate the IR fluxes, so call picaso with only thermal
 
-                flux_net_v_layer_full, flux_net_v_full, flux_plus_v_full, flux_minus_v_full , flux_net_ir_layer_full, flux_net_ir_full, flux_plus_ir_full, flux_minus_ir_full = climate(pressure, temp, dwni, bb , y2, tp, tmin, tmax, DTAU, TAU, W0, 
+                flux_net_v_layer_full, flux_net_v_full, flux_plus_v_full, flux_minus_v_full , flux_net_ir_layer_full, flux_net_ir_full, flux_plus_ir_full, flux_minus_ir_full = get_fluxes(pressure, temp, dwni, bb , y2, tp, tmin, tmax, DTAU, TAU, W0, 
             COSB,ftau_cld, ftau_ray,GCOS2, DTAU_OG, TAU_OG, W0_OG, COSB_OG, W0_no_raman , surf_reflect, 
-            ubar0,ubar1,cos_theta, FOPI, single_phase,multi_phase,frac_a,frac_b,frac_c,constant_back,constant_forward, tridiagonal , 
-            wno,nwno,ng,nt, nlevel, ngauss, gauss_wts, False, True) #false for reflected, True for thermal
+            ubar0,ubar1,cos_theta, FOPI, single_phase,multi_phase,frac_a,frac_b,frac_c,constant_back,constant_forward, 
+            wno,nwno,ng,nt,gweight,tweight, nlevel, ngauss, gauss_wts, False, True) #false for reflected, True for thermal
 
 
                 # extract ir fluxes
 
                 flux_net_ir_layer = flux_net_ir_layer_full[:] #fmneti
                 flux_net_ir = flux_net_ir_full[:]     #fneti
                 flux_plus_ir = flux_plus_ir_full[:,:]  
@@ -694,14 +719,19 @@
             
             g[i] = sum
 
             p[i] = -f_vec[i]
         
         f_old = f #fold
         
+        #print('f_vec[0],f_vec[-1],min,max:f_vec', 
+        #    f_vec[0],f_vec[-1],min(f_vec),max(f_vec))
+        #print(f_vec)
+        #raise Exception ("stop")
+
         A, p = mat_sol(A, nlevel, n_total, p)
         
         #print(p)
         
         
 
         check = False
@@ -739,18 +769,19 @@
             if tmp > test :
                 test= tmp 
 
         alamin = tolx/test
         alam = 1.0
         
         f2= f #################### to avoid call before assignment and run using numba
-        #print(alamin)
-
-        ## stick a while loop here maybe for the weird fortran goto 1
-        # you have in tstart.
+        #     Convergence test:  Find magnitude of correction by comparing
+        #        temperature steps to a appropriate scale SCALT.  If average
+        #        correction ERR is large, use only a fraction of the step.
+        #        When ERR is less than CONV, routine has converged.
+        
         flag_converge = 0
         # instead of the goto statement here
         #ct_num = 0
         while flag_converge == 0 :
             #ct_num+=1
             err = 0.0
             dmx = 0.0
@@ -761,15 +792,15 @@
                 dzx= abs(p[j])
 
                 if dzx > dmx :
                     dmx = dzx
                     jmx = j+ n_top_r
                 err += dzx
             
-            err= err/(n_total*scalt)
+            err= err/(float(n_total)*scalt)
 
             if jmx > nstr[1] :
                 jmx+= nstr[2]-nstr[1]
             
             ndo = n_top_r
             flag_ndo = 0 
             if ndo < 0 :
@@ -813,18 +844,18 @@
             for j1 in range(n_top_r+1, nlevel):
                 if temp[j1] < tmin:
                     temp[j1] = tmin+ 0.1
                 elif temp[j1] > tmax:
                     temp[j1] = tmax- 0.1
             
             # re calculate thermal flux
-            flux_net_v_layer_full, flux_net_v_full, flux_plus_v_full, flux_minus_v_full , flux_net_ir_layer_full, flux_net_ir_full, flux_plus_ir_full, flux_minus_ir_full = climate(pressure, temp, dwni, bb , y2, tp, tmin, tmax, DTAU, TAU, W0, 
+            flux_net_v_layer_full, flux_net_v_full, flux_plus_v_full, flux_minus_v_full , flux_net_ir_layer_full, flux_net_ir_full, flux_plus_ir_full, flux_minus_ir_full = get_fluxes(pressure, temp, dwni, bb , y2, tp, tmin, tmax, DTAU, TAU, W0, 
             COSB,ftau_cld, ftau_ray,GCOS2, DTAU_OG, TAU_OG, W0_OG, COSB_OG, W0_no_raman , surf_reflect, 
-            ubar0,ubar1,cos_theta, FOPI, single_phase,multi_phase,frac_a,frac_b,frac_c,constant_back,constant_forward, tridiagonal , 
-            wno,nwno,ng,nt, nlevel, ngauss, gauss_wts, False, True) #false reflected, True thermal
+            ubar0,ubar1,cos_theta, FOPI, single_phase,multi_phase,frac_a,frac_b,frac_c,constant_back,constant_forward,
+            wno,nwno,ng,nt,gweight,tweight, nlevel, ngauss, gauss_wts, False, True) #false reflected, True thermal
 
 
            
 
             # extract ir fluxes
 
             flux_net_ir_layer = flux_net_ir_layer_full[:] #fmneti
@@ -871,60 +902,55 @@
                 if flag_nao == 1 :
                         nao= nao_temporary
                         flag_nao = 0
                 
                 nao+= n_bot_a - n_strt_a
                         
             f= 0.5*sum
-            # check_convergence is fortran from line indexed 9995 till next line of 19
+            #if verbose: print('cond1:alam.lt.alamin',alam, alamin)
+            #if verbose: print('cond2:f.le.CCC',f,f_old + alf*alam*slope)
+            #if verbose: print('f,fold,alf,alam,slope',f,f_old,alf,alam,slope)
+            #First check: Is T too small to continue? 
             if alam < alamin :
-                #print(alam, alamin)
                 check = True
-                #print(' CONVERGED ON SMALL T STEP')
-                #print("1st if")
-                #print(alam, alamin)
+                #if verbose: print(' CONVERGED ON SMALL T STEP alam, alamin', alam, alamin)
                 flag_converge, check = check_convergence(f_vec, n_total, tolf, check, f, dflux, tolmin, temp, temp_old, g , tolx)
  
-            
+            #Second check: Has the net flux decreased enough that we are happy in the line search
+            #If so you can proceed
             elif f <= f_old + alf*alam*slope :
-                #print("2nd if")
-                
-                
-                #print ('Exit with decreased f')
+                #if verbose: print ('Exit with decreased f')
                 flag_converge, check = check_convergence(f_vec, n_total, tolf, check, f, dflux, tolmin, temp, temp_old, g , tolx)
 
-                
+            #Else: Let's back track     
             else:
-                
-                # we backtrack
-                #print("3rd if")
-                #print(' Now backtracking, f, fold, alf, alam, slope', f, f_old, alf, alam, slope)
+                #if verbose: print(' Now backtracking, f, fold, alf, alam, slope', f, f_old, alf, alam, slope)
                 if alam == 1.0:
                     
                     tmplam= -slope/ (2*(f-f_old-slope))
                 else:
                     
                     rhs_1 = f- f_old - alam*slope
                     rhs_2 = f2 - f_old - alam2*slope
                     anr= ((rhs_1/alam**2)-(rhs_2/alam2**2))/(alam-alam2)
                     b= (-alam2*rhs_1/alam**2+alam*rhs_2/alam2**2)/(alam-alam2)
                     
 
                     if anr == 0 :
-                        tmplam= -slope/(2*b)
+                        tmplam= -slope/(2.0*b)
                         
                         
                     else:
                         disc= b*b - 3.0*anr*slope
                         
                         if disc < 0.0 :
                             tmplam= 0.5*alam
                            
                         elif b <= 0.0:
-                            tmplam=(-b + sqrt(disc))/(3*anr)
+                            tmplam=(-b + sqrt(disc))/(3.0*anr)
                             
 
                         else:
                             tmplam= -slope/(b+sqrt(disc))
                             
                     if tmplam > 0.5*alam:
                         
@@ -935,37 +961,38 @@
                 
                 alam = max(tmplam,0.1*alam)
 
             if np.isnan(np.sum(temp)) == True:
                 
                 flag_converge = 1 # to avoid getting stuck here unnecesarily.
                 temp = temp_old.copy() +0.5
-                print("Got stuck-- so escaping the while loop in tstart")
-        print("Iteration number ", its,", min , max temp ", min(temp),max(temp), ", flux balance ", flux_net[0]/abs(tidal[0]))
-        #print(f, f_old, tolf, np.max((temp-temp_old)/temp_old), tolx)
+                if verbose: print("Got stuck with temp NaN -- so escaping the while loop in tstart")
+        
+
+        if verbose: print("Iteration number ", its,", min , max temp ", min(temp),max(temp), ", flux balance ", flux_net[0]/abs(tidal[0]))
+
         if save_profile == 1:
             all_profiles = np.append(all_profiles,temp_old)
         if flag_converge == 2 : # converged
             # calculate  lapse rate
             dtdp=np.zeros(shape=(nlevel-1))
             for j in range(nlevel -1):
                 dtdp[j] = (log( temp[j]) - log( temp[j+1]))/(log(pressure[j]) - log(pressure[j+1]))
             
-            print("In t_start: Converged Solution in iterations ",its)
+            if verbose: print("In t_start: Converged Solution in iterations ",its)
             
            
            
             return   temp,  dtdp, flag_converge , flux_net_ir, flux_plus_ir[0,:] , all_profiles
         
-    print("Iterations exceeded it_max ! sorry ")#,np.max(dflux/tidal), tolf, np.max((temp-temp_old)/temp_old), tolx)
+    if verbose: print("Iterations exceeded it_max ! sorry ")
     dtdp=np.zeros(shape=(nlevel-1))
     for j in range(nlevel -1):
         dtdp[j] = (log( temp[j]) - log( temp[j+1]))/(log(pressure[j]) - log(pressure[j+1]))
 
-
     return temp, dtdp, flag_converge  , flux_net_ir_layer, flux_plus_ir[0,:], all_profiles
 
 @jit(nopython=True, cache=True)
 def check_convergence(f_vec, n_total, tolf, check, f, dflux, tolmin, temp, temp_old, g , tolx):
     """
     
     Module for checking convergence. Used in t_start module.
@@ -977,14 +1004,15 @@
             test=abs(f_vec[i])
     
     if test < tolf :
         check = False
         
         flag_converge = 2
         return flag_converge , check
+
     if check == True :
         test = 0.0
         den1 = max(f,0.5*(n_total))
         
         for i in range(n_total):
             tmp= abs(g[i])*dflux[i]/den1
             if tmp > test:
@@ -1039,18 +1067,18 @@
     n = 3+3*(nlv-1) -1 # -1 for the py referencing
     nstr[n] = nstr[n] + 1*ngrow
     nstr[n+1] = nstr[n+1] + 1*ngrow
 
     return nstr
 
 @jit(nopython=True, cache=True)
-def climate( pressure, temperature, dwni,  bb , y2, tp, tmin, tmax ,DTAU, TAU, W0, 
+def get_fluxes( pressure, temperature, dwni,  bb , y2, tp, tmin, tmax ,DTAU, TAU, W0, 
             COSB,ftau_cld, ftau_ray,GCOS2, DTAU_OG, TAU_OG, W0_OG, COSB_OG, W0_no_raman , surf_reflect, 
-            ubar0,ubar1,cos_theta, FOPI, single_phase,multi_phase,frac_a,frac_b,frac_c,constant_back,constant_forward, tridiagonal , 
-            wno,nwno,ng,nt, nlevel, ngauss, gauss_wts,reflected, thermal):
+            ubar0,ubar1,cos_theta, F0PI, single_phase,multi_phase,frac_a,frac_b,frac_c,constant_back,constant_forward,
+            wno,nwno,ng,nt,gweight,tweight, nlevel, ngauss, gauss_wts,reflected, thermal):
     """
     Program to run RT for climate calculations. Runs the thermal and reflected module.
     And combines the results with wavenumber widths.
 
     Parameters 
     ----------
     pressure : array 
@@ -1087,149 +1115,174 @@
     # for visible
     flux_net_v = np.zeros(shape=(ng,nt,nlevel)) #net level visible fluxes
     flux_net_v_layer=np.zeros(shape=(ng,nt,nlevel)) #net layer visible fluxes
 
     flux_plus_v= np.zeros(shape=(ng,nt,nlevel,nwno)) # level plus visible fluxes
     flux_minus_v= np.zeros(shape=(ng,nt,nlevel,nwno)) # level minus visible fluxes
     
-    """<<<<<<< NEWCLIMA
+    #"""<<<<<<< NEWCLIMA
     # for thermal
     flux_plus_midpt = np.zeros(shape=(ng,nt,nlevel,nwno))
     flux_minus_midpt = np.zeros(shape=(ng,nt,nlevel,nwno))
 
     flux_plus = np.zeros(shape=(ng,nt,nlevel,nwno))
     flux_minus = np.zeros(shape=(ng,nt,nlevel,nwno))
-    """
+    #"""
+
+    """<<<<<<< OG
     # for thermal
     flux_plus_midpt = np.zeros(shape=(nlevel,nwno))
     flux_minus_midpt = np.zeros(shape=(nlevel,nwno))
 
     flux_plus = np.zeros(shape=(nlevel,nwno))
     flux_minus = np.zeros(shape=(nlevel,nwno))
+    """
 
     # outputs needed for climate
     flux_net_ir = np.zeros(shape=(nlevel)) #net level visible fluxes
     flux_net_ir_layer=np.zeros(shape=(nlevel)) #net layer visible fluxes
 
     flux_plus_ir= np.zeros(shape=(nlevel,nwno)) # level plus visible fluxes
     flux_minus_ir= np.zeros(shape=(nlevel,nwno)) # level minus visible fluxes
 
     
-    ugauss_angles= np.array([0.0985350858,0.3045357266,0.5620251898,0.8019865821,0.9601901429])    
-    ugauss_weights = np.array([0.0157479145,0.0739088701,0.1463869871,0.1671746381,0.0967815902])
+    #ugauss_angles= np.array([0.0985350858,0.3045357266,0.5620251898,0.8019865821,0.9601901429])    
+    #ugauss_weights = np.array([0.0157479145,0.0739088701,0.1463869871,0.1671746381,0.0967815902])
     #ugauss_angles = np.array([0.66666])
     #ugauss_weights = np.array([0.5])
 
     if reflected:
         #use toon method (and tridiagonal matrix solver) to get net cumulative fluxes 
         b_top = 0.0
         for ig in range(ngauss): # correlated - loop (which is different from gauss-tchevychev angle)
-            """
-            <<<<<<< NEWCLIMA
+            #"""
+            #<<<<<<< NEWCLIMA
             #here only the fluxes are returned since we dont care about the outgoing intensity at the 
             #top, which is only used for albedo/ref light spectra
             ng_clima,nt_clima=1,1
             ubar0_clima = ubar0*0+0.5
             ubar1_clima = ubar1*0+0.5
-
-            _, out_ref_fluxes = get_reflected_1d_newclima(nlevel, wno,nwno,ng_clima,nt_clima,
+            _, out_ref_fluxes = get_reflected_1d(nlevel, wno,nwno,ng_clima,nt_clima,
                                     DTAU[:,:,ig], TAU[:,:,ig], W0[:,:,ig], COSB[:,:,ig],
                                     GCOS2[:,:,ig],ftau_cld[:,:,ig],ftau_ray[:,:,ig],
                                     DTAU_OG[:,:,ig], TAU_OG[:,:,ig], W0_OG[:,:,ig], COSB_OG[:,:,ig],
                                     surf_reflect, ubar0_clima,ubar1_clima,cos_theta, F0PI,
                                     single_phase,multi_phase,
-                                    frac_a,frac_b,frac_c,constant_back,constant_forward, tridiagonal,
+                                    frac_a,frac_b,frac_c,constant_back,constant_forward, 
                                     get_toa_intensity=0, get_lvl_flux=1)
 
             flux_minus_all_v, flux_plus_all_v, flux_minus_midpt_all_v, flux_plus_midpt_all_v = out_ref_fluxes
+            
+            #import pickle as pk
+            #pk.dump([flux_minus_all_v, flux_plus_all_v, flux_minus_midpt_all_v, flux_plus_midpt_all_v], open('newclima.pk','wb'))
 
             flux_net_v_layer += (np.sum(flux_plus_midpt_all_v,axis=3)-np.sum(flux_minus_midpt_all_v,axis=3))*gauss_wts[ig]
             flux_net_v += (np.sum(flux_plus_all_v,axis=3)-np.sum(flux_minus_all_v,axis=3))*gauss_wts[ig]
 
-            ======="""
+            #======="""
             #nlevel = atm.c.nlevel
+
+            """
+            <<<<<<< GFLUXV
+            ng_clima,nt_clima=1,1
+            ubar0_clima = ubar0*0+0.5
+            ubar1_clima = ubar1*0+0.5
+
             RSFV = 0.01 # from tgmdat.f of EGP
             
             b_surface = 0.0 +RSFV*ubar0[0]*FOPI*np.exp(-TAU[-1,:,ig]/ubar0[0])
             
             delta_approx = 0 # assuming delta approx is already applied on opds 
                         
-            flux_minus_all_v, flux_plus_all_v, flux_minus_midpt_all_v, flux_plus_midpt_all_v = get_reflected_1d_gfluxv(nlevel, wno,nwno, ng,nt, DTAU[:,:,ig], TAU[:,:,ig], W0[:,:,ig], COSB[:,:,ig],
-                                                                                       surf_reflect,b_top,b_surface,ubar0, FOPI,tridiagonal, delta_approx)
+            flux_minus_all_v, flux_plus_all_v, flux_minus_midpt_all_v, flux_plus_midpt_all_v = get_reflected_1d_gfluxv(nlevel, wno,nwno, ng_clima,nt_clima, DTAU[:,:,ig], TAU[:,:,ig], W0[:,:,ig], COSB[:,:,ig],
+                                                                                       surf_reflect,b_top,b_surface,ubar0_clima, F0PI,tridiagonal, delta_approx)
+            
+            import pickle as pk
+            pk.dump([flux_minus_all_v, flux_plus_all_v, flux_minus_midpt_all_v, flux_plus_midpt_all_v], open('gfluxv.pk','wb'))
             
-
             flux_net_v_layer += (np.sum(flux_plus_midpt_all_v,axis=3)-np.sum(flux_minus_midpt_all_v,axis=3))*gauss_wts[ig]
             flux_net_v += (np.sum(flux_plus_all_v,axis=3)-np.sum(flux_minus_all_v,axis=3))*gauss_wts[ig]
+            """
 
             flux_plus_v += flux_plus_all_v*gauss_wts[ig]
             flux_minus_v += flux_minus_all_v*gauss_wts[ig]
 
         #if full output is requested add in xint at top for 3d plots
 
 
-    #thermal=1
     if thermal:
 
         #use toon method (and tridiagonal matrix solver) to get net cumulative fluxes 
         
         for ig in range(ngauss): # correlated - loop (which is different from gauss-tchevychev angle)
             
             #remember all OG values (e.g. no delta eddington correction) go into thermal as well as 
             #the uncorrected raman single scattering 
             
-            """<<<<<<< NEWCLIMA
+            #"""<<<<<<< NEWCLIMA
             hard_surface = 0 
-            _,out_therm_fluxes = get_thermal_1d_newclima(nlevel, wno,nwno,ng,nt,temperature,
+            _,out_therm_fluxes = get_thermal_1d(nlevel, wno,nwno,ng,nt,temperature,
                                             DTAU_OG[:,:,ig], W0_no_raman[:,:,ig], COSB_OG[:,:,ig], 
                                             pressure,ubar1,
-                                            surf_reflect, hard_surface, tridiagonal)
-            flux_minus_all_i, flux_plus_all_i, flux_minus_midpt_all_i, flux_plus_midpt_all_i = out_therm_fluxes
+                                            surf_reflect, hard_surface, dwni, calc_type=1)
 
+            flux_minus_all_i, flux_plus_all_i, flux_minus_midpt_all_i, flux_plus_midpt_all_i = out_therm_fluxes
 
             flux_plus += flux_plus_all_i*gauss_wts[ig]
             flux_minus += flux_minus_all_i*gauss_wts[ig]
-            """
-
+            flux_plus_midpt += flux_plus_midpt_all_i*gauss_wts[ig]#*weights
+            flux_minus_midpt += flux_minus_midpt_all_i*gauss_wts[ig]#*weights
+            #"""
+            
+            """<<<<<<< OG CODE
             calc_type=1 # this line might change depending on Natasha's new function
             
             #for iubar,weights in zip(ugauss_angles,ugauss_weights):
-            flux_minus_all_i, flux_plus_all_i, flux_minus_midpt_all_i, flux_plus_midpt_all_i=get_thermal_1d_gfluxi(nlevel,wno,nwno,ng,nt,temperature,DTAU_OG[:,:,ig], W0_no_raman[:,:,ig], COSB_OG[:,:,ig], pressure,ubar1,surf_reflect, ugauss_angles,ugauss_weights, tridiagonal,calc_type, bb , y2, tp, tmin, tmax)
+            flux_minus_all_i, flux_plus_all_i, flux_minus_midpt_all_i, flux_plus_midpt_all_i=get_thermal_1d_gfluxi(nlevel,wno,nwno,ng,nt,temperature,DTAU_OG[:,:,ig], W0_no_raman[:,:,ig], COSB_OG[:,:,ig], pressure,ubar1,surf_reflect, ugauss_angles,ugauss_weights, tridiagonal,calc_type, dwni)#,bb , y2, tp, tmin, tmax)
 
             flux_plus += flux_plus_all_i*gauss_wts[ig]#*weights
             flux_minus += flux_minus_all_i*gauss_wts[ig]#*weights
 
             flux_plus_midpt += flux_plus_midpt_all_i*gauss_wts[ig]#*weights
             flux_minus_midpt += flux_minus_midpt_all_i*gauss_wts[ig]#*weights
+            """
 
-
-        """<<<<<<< NEWCLIMA
+        #"""<<<<<<< NEWCLIMA
         #compresses in gauss-chebyshev angle space 
         #the integration over the "disk" of the planet opposed to the 
         #other gauss angles which are for the correlatedk tables
-        gweight = np.array([0.01574791, 0.07390887, 0.14638699, 0.16717464, 0.09678159])
-        tweight = np.array([6.28318531])
+        #gweight = np.array([0.01574791, 0.07390887, 0.14638699, 0.16717464, 0.09678159])
+        #tweight = np.array([1])#[6.28318531])
         flux_plus = compress_thermal(nwno, flux_plus, gweight, tweight)
         flux_minus= compress_thermal(nwno, flux_minus, gweight, tweight)
         flux_plus_midpt= compress_thermal(nwno, flux_plus_midpt, gweight, tweight)
         flux_minus_midpt= compress_thermal(nwno, flux_minus_midpt, gweight, tweight)
-        """
+        #"""
 
         for wvi in range(nwno):
             flux_net_ir_layer += (flux_plus_midpt[:,wvi]-flux_minus_midpt[:,wvi]) * dwni[wvi]
             flux_net_ir += (flux_plus[:,wvi]-flux_minus[:,wvi]) * dwni[wvi]
 
             flux_plus_ir[:,wvi] += flux_plus[:,wvi] * dwni[wvi]
             flux_minus_ir[:,wvi] += flux_minus[:,wvi] * dwni[wvi]
-
-
+        """
+        print('debug fluxes in get_fluxes', temperature)
+        for wvi in range(nwno):
+            for il in range(len(flux_plus_midpt[:,0])):
+                print(wvi, dwni[wvi],flux_plus_midpt[il,wvi],flux_minus_midpt[il,wvi] )
+        """
 
         #if full output is requested add in flux at top for 3d plots
     
     return flux_net_v_layer, flux_net_v, flux_plus_v, flux_minus_v , flux_net_ir_layer, flux_net_ir, flux_plus_ir, flux_minus_ir
 
+#soon I will deprecate the function name "climate" as it is really confusing with what it 
+#actually does, which is just run the RT to get fluxes
+climate = get_fluxes
+
 def calculate_atm(bundle, opacityclass):
 
     inputs = bundle.inputs
 
     wno = opacityclass.wno
     nwno = opacityclass.nwno
     ngauss = opacityclass.ngauss
@@ -1243,15 +1296,14 @@
 
     #set approx numbers options (to be used in numba compiled functions)
     single_phase = inputs['approx']['rt_params']['toon']['single_phase']
     multi_phase = inputs['approx']['rt_params']['toon']['multi_phase']
     raman_approx =inputs['approx']['rt_params']['common']['raman']
     method = inputs['approx']['rt_method']
     stream = inputs['approx']['rt_params']['common']['stream']
-    tridiagonal = 0 
 
     #parameters needed for the two term hg phase function. 
     #Defaults are set in config.json
     f = inputs['approx']['rt_params']['common']['TTHG_params']['fraction']
     frac_a = f[0]
     frac_b = f[1]
     frac_c = f[2]
@@ -1269,32 +1321,30 @@
     
 
     #phase angle 
     phase_angle = inputs['phase_angle']
     #get geometry
     geom = inputs['disco']
 
-    """ NEWCLIMA
+    #""" NEWCLIMA
     ng, nt = geom['num_gangle'], geom['num_tangle']#1,1 #
     gangle,gweight,tangle,tweight = geom['gangle'], geom['gweight'],geom['tangle'], geom['tweight']
     lat, lon = geom['latitude'], geom['longitude']
     cos_theta = geom['cos_theta']
     ubar0, ubar1 = geom['ubar0'], geom['ubar1']
-    """
-    ng, nt = 1,1 #geom['num_gangle'], geom['num_tangle']
+    #"""
+    """ OG Code
+    ng, nt = 1,1
     gangle,gweight,tangle,tweight = geom['gangle'], geom['gweight'],geom['tangle'], geom['tweight']
     lat, lon = geom['latitude'], geom['longitude']
     cos_theta = geom['cos_theta']
-    #ubar0, ubar1 = geom['ubar0'], geom['ubar1']
-    #print(np.shape(ubar0),ubar0[0])
     ubar0,ubar1 = np.zeros((5,1)),np.zeros((5,1))
     ubar0 += 0.5
     ubar1 += 0.5
-    #print(ubar0,ubar1)
-
+    """
     #set star parameters
     radius_star = inputs['star']['radius']
 
     #semi major axis
     sa = inputs['star']['semi_major']
 
     #begin atm setup
@@ -1345,15 +1395,15 @@
             atm, opacityclass, ngauss=ngauss, stream=stream, delta_eddington=delta_eddington,test_mode=test_mode,raman=raman_approx,
             full_output=False, plot_opacity=False)
     
 
     #mmw = np.mean(atm.layer['mmw'])
     mmw = atm.layer['mmw']
     
-    return DTAU, TAU, W0, COSB,ftau_cld, ftau_ray,GCOS2, DTAU_OG, TAU_OG, W0_OG, COSB_OG, W0_no_raman , atm.surf_reflect, ubar0,ubar1,cos_theta, single_phase,multi_phase,frac_a,frac_b,frac_c,constant_back,constant_forward, tridiagonal , wno,nwno,ng,nt, nlevel, ngauss, gauss_wts, mmw
+    return DTAU, TAU, W0, COSB,ftau_cld, ftau_ray,GCOS2, DTAU_OG, TAU_OG, W0_OG, COSB_OG, W0_no_raman , atm.surf_reflect, ubar0,ubar1,cos_theta, single_phase,multi_phase,frac_a,frac_b,frac_c,constant_back,constant_forward, wno,nwno,ng,nt, nlevel, ngauss, gauss_wts, mmw,gweight,tweight
 
 
 def calculate_atm_deq(bundle, opacityclass,on_fly=False,gases_fly=None):
 
     inputs = bundle.inputs
 
     wno = opacityclass.wno
@@ -1369,15 +1419,14 @@
 
     #set approx numbers options (to be used in numba compiled functions)
     single_phase = inputs['approx']['rt_params']['toon']['single_phase']
     multi_phase = inputs['approx']['rt_params']['toon']['multi_phase']
     raman_approx =inputs['approx']['rt_params']['common']['raman']
     method = inputs['approx']['rt_method']
     stream = inputs['approx']['rt_params']['common']['stream']
-    tridiagonal = 0 
 
     #parameters needed for the two term hg phase function. 
     #Defaults are set in config.json
     f = inputs['approx']['rt_params']['common']['TTHG_params']['fraction']
     frac_a = f[0]
     frac_b = f[1]
     frac_c = f[2]
@@ -1395,24 +1444,31 @@
     
 
     #phase angle 
     phase_angle = inputs['phase_angle']
     #get geometry
     geom = inputs['disco']
 
+    ng, nt = geom['num_gangle'], geom['num_tangle']#1,1 #
+    gangle,gweight,tangle,tweight = geom['gangle'], geom['gweight'],geom['tangle'], geom['tweight']
+    lat, lon = geom['latitude'], geom['longitude']
+    cos_theta = geom['cos_theta']
+    ubar0, ubar1 = geom['ubar0'], geom['ubar1']
+    """
     ng, nt = 1,1 #geom['num_gangle'], geom['num_tangle']
     gangle,gweight,tangle,tweight = geom['gangle'], geom['gweight'],geom['tangle'], geom['tweight']
     lat, lon = geom['latitude'], geom['longitude']
     cos_theta = geom['cos_theta']
     #ubar0, ubar1 = geom['ubar0'], geom['ubar1']
     #print(np.shape(ubar0),ubar0[0])
     ubar0,ubar1 = np.zeros((5,1)),np.zeros((5,1))
     ubar0 += 0.5
     ubar1 += 0.5
     #print(ubar0,ubar1)
+    """
 
     #set star parameters
     radius_star = inputs['star']['radius']
     #F0PI = np.zeros(nwno) + 1.
     #semi major axis
     sa = inputs['star']['semi_major']
 
@@ -1466,8 +1522,8 @@
             atm, opacityclass, ngauss=ngauss, stream=stream, delta_eddington=delta_eddington,test_mode=test_mode,raman=raman_approx,
             full_output=False, plot_opacity=False)
     
 
     #mmw = np.mean(atm.layer['mmw'])
     mmw = atm.level['mmw']
     
-    return DTAU, TAU, W0, COSB,ftau_cld, ftau_ray,GCOS2, DTAU_OG, TAU_OG, W0_OG, COSB_OG, W0_no_raman , atm.surf_reflect, ubar0,ubar1,cos_theta, single_phase,multi_phase,frac_a,frac_b,frac_c,constant_back,constant_forward, tridiagonal , wno,nwno,ng,nt, nlevel, ngauss, gauss_wts, mmw
+    return DTAU, TAU, W0, COSB,ftau_cld, ftau_ray,GCOS2, DTAU_OG, TAU_OG, W0_OG, COSB_OG, W0_no_raman , atm.surf_reflect, ubar0,ubar1,cos_theta, single_phase,multi_phase,frac_a,frac_b,frac_c,constant_back,constant_forward, wno,nwno,ng,nt, nlevel, ngauss, gauss_wts, mmw,gweight,tweight
```

### Comparing `picaso-3.1.2/picaso/deq_chem.py` & `picaso-3.2/picaso/deq_chem.py`

 * *Files 2% similar despite different names*

```diff
@@ -170,15 +170,15 @@
 
                 ct+=1   
     # k coefficients were raised to exponentials in do_mixing_mono routine so taking a log to take them back
     return np.log(kappa_mixed) # this array will be interpolated now
 
 
 @jit(nopython=True, cache=True)
-def mix_all_gases_gasesfly(kappa1,kappa2,kappa3,kappa4,kappa5,kappa6,kappa7,kappa8,kappa9,kappa10,kappa11,kappa12,kappa13,kappa14,kappa15,mix1,mix2,mix3,mix4,mix5,mix6,mix7,mix8,mix9,mix10,mix11,mix12,mix13,mix14,mix15,gauss_pts, gauss_wts,indices):
+def mix_all_gases_gasesfly(kappa1,kappa2,kappa3,kappa4,kappa5,kappa6,kappa7,kappa8,kappa9,kappa10,kappa11,kappa12,kappa13,kappa14,kappa15,kappa16,kappa17,mix1,mix2,mix3,mix4,mix5,mix6,mix7,mix8,mix9,mix10,mix11,mix12,mix13,mix14,mix15,mix16,mix17,gauss_pts, gauss_wts,indices):
     """
     Function to perform "on-the-fly" mixing of 5 opacity sources from Amundsen et al. (2017)
     Parameters
     ----------
     kappa1 : array
         K-coefficients of gas mixture 1
     kappa2 : array 
@@ -222,28 +222,28 @@
     for ilayer in range(Nlayer):
         ct =0
         for p_ind in [indices[0][ilayer],indices[1][ilayer]]:
             for t_ind in [indices[2][ilayer],indices[3][ilayer]]: 
                 for iw in range(kappa1.shape[2]): # mixing needs to be done at each wno bin separately.
 
                     kmix_bin = do_mixing_mono_gasesfly(kappa1[p_ind,t_ind,iw,:],kappa2[p_ind,t_ind,iw,:],kappa3[p_ind,t_ind,iw,:],kappa4[p_ind,t_ind,iw,:],kappa5[p_ind,t_ind,iw,:],
-                                                        kappa6[p_ind,t_ind,iw,:],kappa7[p_ind,t_ind,iw,:],kappa8[p_ind,t_ind,iw,:],kappa9[p_ind,t_ind,iw,:],kappa10[p_ind,t_ind,iw,:],kappa11[p_ind,t_ind,iw,:],kappa12[p_ind,t_ind,iw,:],kappa13[p_ind,t_ind,iw,:],kappa14[p_ind,t_ind,iw,:],kappa15[p_ind,t_ind,iw,:],
-                                    mix1[ilayer],mix2[ilayer],mix3[ilayer],mix4[ilayer],mix5[ilayer],mix6[ilayer],mix7[ilayer],mix8[ilayer],mix9[ilayer],mix10[ilayer],mix11[ilayer],mix12[ilayer],mix13[ilayer],mix14[ilayer],mix15[ilayer],gauss_pts,gauss_wts)
+                                                        kappa6[p_ind,t_ind,iw,:],kappa7[p_ind,t_ind,iw,:],kappa8[p_ind,t_ind,iw,:],kappa9[p_ind,t_ind,iw,:],kappa10[p_ind,t_ind,iw,:],kappa11[p_ind,t_ind,iw,:],kappa12[p_ind,t_ind,iw,:],kappa13[p_ind,t_ind,iw,:],kappa14[p_ind,t_ind,iw,:],kappa15[p_ind,t_ind,iw,:],kappa16[p_ind,t_ind,iw,:],kappa17[p_ind,t_ind,iw,:],
+                                    mix1[ilayer],mix2[ilayer],mix3[ilayer],mix4[ilayer],mix5[ilayer],mix6[ilayer],mix7[ilayer],mix8[ilayer],mix9[ilayer],mix10[ilayer],mix11[ilayer],mix12[ilayer],mix13[ilayer],mix14[ilayer],mix15[ilayer],mix16[ilayer],mix17[ilayer],gauss_pts,gauss_wts)
 
                     kappa_mixed[ilayer,iw,:,ct] = kmix_bin
 
                 ct+=1   
     # k coefficients were raised to exponentials in do_mixing_mono routine so taking a log to take them back
     return np.log(kappa_mixed) # this array will be interpolated now
 
 
 @jit(nopython=True, cache=True)
 def do_mixing_mono_gasesfly(kappa1_mono,kappa2_mono,kappa3_mono,kappa4_mono,kappa5_mono,
-                          kappa6_mono,kappa7_mono,kappa8_mono,kappa9_mono,kappa10_mono,kappa11_mono,kappa12_mono,kappa13_mono,kappa14_mono,kappa15_mono,
-                          mix1,mix2,mix3,mix4,mix5,mix6,mix7,mix8,mix9,mix10,mix11,mix12,mix13,mix14,mix15,gauss_pts,gauss_wts):
+                          kappa6_mono,kappa7_mono,kappa8_mono,kappa9_mono,kappa10_mono,kappa11_mono,kappa12_mono,kappa13_mono,kappa14_mono,kappa15_mono,kappa16_mono,kappa17_mono,
+                          mix1,mix2,mix3,mix4,mix5,mix6,mix7,mix8,mix9,mix10,mix11,mix12,mix13,mix14,mix15,mix16,mix17,gauss_pts,gauss_wts):
     """
     Function which mixes all the gases together at a single wavenumber bin
     Parameters
     ----------
     kappa1_mono : array
         K-coefficients of gas mixture 1
     kappa2_mono : array 
@@ -299,14 +299,18 @@
     kmix_bin,mix_t = mix_2_gases(kmix_bin,np.exp(kappa12_mono), mix_t,mix12,gauss_pts,gauss_wts) 
 
     kmix_bin,mix_t = mix_2_gases(kmix_bin,np.exp(kappa13_mono), mix_t,mix13,gauss_pts,gauss_wts) 
 
     kmix_bin,mix_t = mix_2_gases(kmix_bin,np.exp(kappa14_mono), mix_t,mix14,gauss_pts,gauss_wts) 
 
     kmix_bin,mix_t = mix_2_gases(kmix_bin,np.exp(kappa15_mono), mix_t,mix15,gauss_pts,gauss_wts) 
+
+    kmix_bin,mix_t = mix_2_gases(kmix_bin,np.exp(kappa16_mono), mix_t,mix16,gauss_pts,gauss_wts) 
+    
+    kmix_bin,mix_t = mix_2_gases(kmix_bin,np.exp(kappa17_mono), mix_t,mix17,gauss_pts,gauss_wts) 
     
     '''
     kmix_bin,mix_t = mix_2_gases(kmix_bin,np.exp(kappa6_mono), mix_t,mix6,gauss_pts,gauss_wts)
     
     kmix_bin,mix_t = mix_2_gases(kmix_bin,np.exp(kappa7_mono), mix_t,mix6,gauss_pts,gauss_wts)
     
     kmix_bin,mix_t = mix_2_gases(kmix_bin,np.exp(kappa8_mono), mix_t,mix6,gauss_pts,gauss_wts)
```

### Comparing `picaso-3.1.2/picaso/disco.py` & `picaso-3.2/picaso/disco.py`

 * *Files identical despite different names*

### Comparing `picaso-3.1.2/picaso/elements.py` & `picaso-3.2/picaso/elements.py`

 * *Files 0% similar despite different names*

```diff
@@ -352,16 +352,15 @@
         group=1, period=1, block='s', series=1,
         mass=2.014101778, eleneg=2.2, eleaffin=0.75420375,
         covrad=0.32, atmrad=0.79, vdwrad=1.2,
         tboil=20.28, tmelt=13.81, density=0.084,
         eleconfig='1s',
         oxistates='1*, -1',
         ionenergy=(13.5984, ),
-        isotopes={1: Isotope(1.0078250321, 0.999885, 1),
-                  2: Isotope(2.014101778, 0.000115, 2)}),
+        isotopes={2: Isotope(2.014101778, 0.000115, 2)}),
     Element(
         2, 'He', 'Helium',
         group=18, period=1, block='s', series=2,
         mass=4.002602, eleneg=0.0, eleaffin=0.0,
         covrad=0.93, atmrad=0.49, vdwrad=1.4,
         tboil=4.216, tmelt=0.95, density=0.1785,
         eleconfig='1s2',
```

### Comparing `picaso-3.1.2/picaso/fluxes.py` & `picaso-3.2/picaso/fluxes.py`

 * *Files 3% similar despite different names*

```diff
@@ -2,65 +2,95 @@
 from numpy import exp, zeros, where, sqrt, cumsum , pi, outer, sinh, cosh, min, dot, array,log, log10,ones, array_equal
 import numpy as np
 import time
 import pickle as pk
 from scipy.linalg import solve_banded
 #from numpy.linalg import solve
 
-@jit(nopython=True, cache=True,fastmath=True)
+@jit(nopython=True, cache=True)
 def slice_eq(array, lim, value):
     """Funciton to replace values with upper or lower limit
     """
     for i in range(array.shape[0]):
         new = array[i,:] 
         new[where(new==lim)] = value
         array[i,:] = new     
     return array
 
-@jit(nopython=True, cache=True,fastmath=True)
+@jit(nopython=True, cache=True)
 def slice_lt(array, lim):
     """Funciton to replace values with upper or lower limit
     """
     for i in range(array.shape[0]):
         new = array[i,:] 
         new[where(new<lim)] = lim
         array[i,:] = new     
     return array
 
-@jit(nopython=True, cache=True,fastmath=True)
+@jit(nopython=True, cache=True)
 def slice_gt(array, lim):
     """Funciton to replace values with upper or lower limit
     """
     for i in range(array.shape[0]):
         new = array[i,:] 
         new[where(new>lim)] = lim
         array[i,:] = new     
     return array
 
 @jit(nopython=True, cache=True)
+def slice_lt_cond(array, cond_array, cond, newval):
+    """Funciton to replace values with upper or lower limit
+    """
+    for i in range(array.shape[0]):
+        new = array[i,:] 
+        new_cond = cond_array[i,:]
+        new[where(new_cond<cond)] = newval
+        array[i,:] = new     
+    return array
+
+
+@jit(nopython=True, cache=True)
+def slice_lt_cond_arr(array, cond_array, cond, newarray):
+    """Funciton to replace values with upper or lower limit
+    """
+    shape = cond_array.shape#e.g. dtau
+
+    cond_array=cond_array.ravel()
+    new = array.ravel() #e.g. b0 
+    newarray1 = newarray[0:-1,:].ravel()
+    newarray2 = newarray[1:,:].ravel()
+
+    #for i in range(array.shape[0]):
+    replace1 = newarray1[where(cond_array<cond)]
+    replace2 = newarray2[where(cond_array<cond)]
+    new[where(cond_array<cond)] = 0.5*(replace1+replace2)
+    array = new.reshape(shape)    
+    return array
+
+@jit(nopython=True, cache=True)
 def slice_rav(array, lim):
     """Funciton to replace values with upper or lower limit
     """
     shape = array.shape
     new = array.ravel()
     new[where(new>lim)] = lim
     new[where(new<-lim)] = -lim
     return new.reshape(shape)
 
-@jit(nopython=True, cache=True,fastmath=True)
+@jit(nopython=True, cache=True)
 def numba_cumsum(mat):
     """Function to compute cumsum along axis=0 to bypass numba not allowing kwargs in 
     cumsum 
     """
     new_mat = zeros(mat.shape)
     for i in range(mat.shape[1]):
         new_mat[:,i] = cumsum(mat[:,i])
     return new_mat
 
-@jit(nopython=True, cache=True)#, fastmath=True)
+@jit(nopython=True, cache=True)
 def setup_tri_diag(nlayer,nwno ,c_plus_up, c_minus_up, 
     c_plus_down, c_minus_down, b_top, b_surface, surf_reflect,
     gama, dtau, exptrm_positive,  exptrm_minus):
     """
     Before we can solve the tridiagonal matrix (See Toon+1989) section
     "SOLUTION OF THE TwO-STREAM EQUATIONS FOR MULTIPLE LAYERS", we 
     need to set up the coefficients. 
@@ -149,15 +179,15 @@
     A[-1,:] = e1[-1,:]-surf_reflect*e3[-1,:]
     B[-1,:] = e2[-1,:]-surf_reflect*e4[-1,:]
     C[-1,:] = 0.0
     D[-1,:] = b_surface-c_plus_down[-1,:] + surf_reflect*c_minus_down[-1,:]
 
     return A, B, C, D
 
-@jit(nopython=True, cache=True,fastmath=True)
+@jit(nopython=True, cache=True)
 def setup_pent_diag(nlayer,nwno ,c_plus_up, c_minus_up, 
     c_plus_down, c_minus_down, b_top, b_surface, surf_reflect,
     gama, dtau, exptrm_positive,  exptrm_minus, g1, g2, exptrm, lamda):
     """
     Parameters
     ----------
     nlayer : int 
@@ -252,15 +282,15 @@
     D[-1,:] = 0. 
     E[-1,:] = 0.
     F[-1,:] = b_surface - c_plus_down[-1,:] + surf_reflect*c_minus_down[-1,:]
 
     return A, B, C, D, E, F
 
 
-@jit(nopython=True, cache=True)#, fastmath=True)
+@jit(nopython=True, cache=True)
 def tri_diag_solve(l, a, b, c, d):
     """
     Tridiagonal Matrix Algorithm solver, a b c d can be NumPy array type or Python list type.
     refer to this wiki_ and to this explanation_. 
     
     .. _wiki: http://en.wikipedia.org/wiki/Tridiagonal_matrix_algorithm
     .. _explanation: http://www.cfd-online.com/Wiki/Tridiagonal_matrix_algorithm_-_TDMA_(Thomas_algorithm)
@@ -322,15 +352,15 @@
 
     return X
 
 @jit(nopython=True, cache=True)
 def get_reflected_3d(nlevel, wno,nwno, numg,numt, dtau_3d, tau_3d, w0_3d, cosb_3d,gcos2_3d, ftau_cld_3d,ftau_ray_3d,
     dtau_og_3d, tau_og_3d, w0_og_3d, cosb_og_3d, 
     surf_reflect,ubar0, ubar1,cos_theta, F0PI,single_phase, multi_phase,
-    frac_a, frac_b, frac_c, constant_back, constant_forward,tridiagonal):
+    frac_a, frac_b, frac_c, constant_back, constant_forward):
     """
     Computes toon fluxes given tau and everything is 3 dimensional. This is the exact same function 
     as `get_flux_geom_1d` but is kept separately so we don't have to do unecessary indexing for 
     retrievals. 
     Parameters
     ----------
     nlevel : int 
@@ -405,16 +435,15 @@
         of forward to back scattering (A + B * gcosb^C), Default is : 1 - gcosb^2
     constant_back : float 
         (Optional), If using the TTHG phase function. Must specify the assymetry of back scatterer. 
         Remember, the output of A & M code does not separate back and forward scattering.
     constant_forward : float 
         (Optional), If using the TTHG phase function. Must specify the assymetry of forward scatterer. 
         Remember, the output of A & M code does not separate back and forward scattering.
-    tridiagonal : int 
-        0 for tridiagonal, 1 for pentadiagonal 
+
     Returns
     -------
     intensity at the top of the atmosphere for all the different ubar1 and ubar2 
     To Do
     -----
     - F0PI Solar flux shouldn't always be 1.. Follow up to make sure that this isn't a bad 
           hardwiring to solar, despite "relative albedo"
@@ -491,36 +520,36 @@
 
 
             #boundary conditions 
             b_top = 0.0                                       
             b_surface = 0. + surf_reflect*ubar0[ng, nt]*F0PI*exp(-tau[-1, :]/ubar0[ng, nt])
 
             #Now we need the terms for the tridiagonal rotated layered method
-            if tridiagonal==0:
-                A, B, C, D = setup_tri_diag(nlayer,nwno,  c_plus_up, c_minus_up, 
-                                    c_plus_down, c_minus_down, b_top, b_surface, surf_reflect,
-                                     gama, dtau, 
-                                    exptrm_positive,  exptrm_minus) 
+            #if tridiagonal==0:
+            A, B, C, D = setup_tri_diag(nlayer,nwno,  c_plus_up, c_minus_up, 
+                                c_plus_down, c_minus_down, b_top, b_surface, surf_reflect,
+                                 gama, dtau, 
+                                exptrm_positive,  exptrm_minus) 
             #else:
             #   A_, B_, C_, D_, E_, F_ = setup_pent_diag(nlayer,nwno,  c_plus_up, c_minus_up, 
             #                       c_plus_down, c_minus_down, b_top, b_surface, surf_reflect,
             #                        gama, dtau, 
             #                       exptrm_positive,  exptrm_minus, g1,g2,exptrm,lamda) 
 
             positive = zeros((nlayer, nwno))
             negative = zeros((nlayer, nwno))
             #========================= Start loop over wavelength =========================
             L = 2*nlayer
             for w in range(nwno):
                 #coefficient of posive and negative exponential terms 
-                if tridiagonal==0:
-                    X = tri_diag_solve(L, A[:,w], B[:,w], C[:,w], D[:,w])
-                    #unmix the coefficients
-                    positive[:,w] = X[::2] + X[1::2] 
-                    negative[:,w] = X[::2] - X[1::2]
+                #if tridiagonal==0:
+                X = tri_diag_solve(L, A[:,w], B[:,w], C[:,w], D[:,w])
+                #unmix the coefficients
+                positive[:,w] = X[::2] + X[1::2] 
+                negative[:,w] = X[::2] - X[1::2]
                 #else:
                 #   X = pent_diag_solve(L, A_[:,w], B_[:,w], C_[:,w], D_[:,w], E_[:,w], F_[:,w])
                 #   #unmix the coefficients
                 #   positive[:,w] = exptrm_minus[:,w] * (X[::2] + X[1::2])
                 #   negative[:,w] = X[::2] - X[1::2]
 
             #========================= End loop over wavelength =========================
@@ -625,19 +654,19 @@
                         +H[i,:]*(1. - exp(-exptrm[i,:]*1-dtau[i,:]/ubar1[ng,nt]))/(lamda[i,:]*1*ubar1[ng,nt] + 1.0))
                         #thermal
 
             xint_at_top[ng,nt,:] = xint[0,:]    
     return xint_at_top
 
 @jit(nopython=True, cache=True)
-def get_reflected_1d(nlevel, wno,nwno, numg,numt, dtau, tau, w0, cosb,gcos2, ftau_cld, ftau_ray,
+def get_reflected_1d_deprecate(nlevel, wno,nwno, numg,numt, dtau, tau, w0, cosb,gcos2, ftau_cld, ftau_ray,
     dtau_og, tau_og, w0_og, cosb_og, 
     surf_reflect,ubar0, ubar1,cos_theta, F0PI,single_phase, multi_phase,
     frac_a, frac_b, frac_c, constant_back, constant_forward,
-    toon_coefficients=0, tridiagonal=0, b_top=0):
+    toon_coefficients=0,b_top=0):
     """
     Computes toon fluxes given tau and everything is 1 dimensional. This is the exact same function 
     as `get_flux_geom_3d` but is kept separately so we don't have to do unecessary indexing for fast
     retrievals. 
     Parameters
     ----------
     nlevel : int 
@@ -712,16 +741,14 @@
         of forward to back scattering (A + B * gcosb^C), Default is : 1 - gcosb^2
     constant_back : float 
         (Optional), If using the TTHG phase function. Must specify the assymetry of back scatterer. 
         Remember, the output of A & M code does not separate back and forward scattering.
     constant_forward : float 
         (Optional), If using the TTHG phase function. Must specify the assymetry of forward scatterer. 
         Remember, the output of A & M code does not separate back and forward scattering.
-    tridiagonal : int 
-        0 for tridiagonal, 1 for pentadiagonal 
     toon_coefficients : int     
         0 for quadrature (default) 1 for eddington
 
     Returns
     -------
     intensity at the top of the atmosphere for all the different ubar1 and ubar2 
     To Do
@@ -792,37 +819,37 @@
 
             #boundary conditions 
             #b_top = 0.0                                       
 
             b_surface = 0. + surf_reflect*u0*F0PI*exp(-tau[-1, :]/u0)
 
             #Now we need the terms for the tridiagonal rotated layered method
-            if tridiagonal==0:
-                A, B, C, D = setup_tri_diag(nlayer,nwno,  c_plus_up, c_minus_up, 
-                                    c_plus_down, c_minus_down, b_top, b_surface, surf_reflect,
-                                     gama, dtau, 
-                                    exptrm_positive,  exptrm_minus) 
+            #if tridiagonal==0:
+            A, B, C, D = setup_tri_diag(nlayer,nwno,  c_plus_up, c_minus_up, 
+                                c_plus_down, c_minus_down, b_top, b_surface, surf_reflect,
+                                 gama, dtau, 
+                                exptrm_positive,  exptrm_minus) 
 
             #else:
             #   A_, B_, C_, D_, E_, F_ = setup_pent_diag(nlayer,nwno,  c_plus_up, c_minus_up, 
             #                       c_plus_down, c_minus_down, b_top, b_surface, surf_reflect,
             #                        gama, dtau, 
             #                       exptrm_positive,  exptrm_minus, g1,g2,exptrm,lamda) 
 
             positive = zeros((nlayer, nwno))
             negative = zeros((nlayer, nwno))
             #========================= Start loop over wavelength =========================
             L = 2*nlayer
             for w in range(nwno):
                 #coefficient of posive and negative exponential terms 
-                if tridiagonal==0:
-                    X = tri_diag_solve(L, A[:,w], B[:,w], C[:,w], D[:,w])
-                    #unmix the coefficients
-                    positive[:,w] = X[::2] + X[1::2] 
-                    negative[:,w] = X[::2] - X[1::2]
+                #if tridiagonal==0:
+                X = tri_diag_solve(L, A[:,w], B[:,w], C[:,w], D[:,w])
+                #unmix the coefficients
+                positive[:,w] = X[::2] + X[1::2] 
+                negative[:,w] = X[::2] - X[1::2]
 
                 #else: 
                 #   X = pent_diag_solve(L, A_[:,w], B_[:,w], C_[:,w], D_[:,w], E_[:,w], F_[:,w])
                     #unmix the coefficients
                 #   positive[:,w] = exptrm_minus[:,w] * (X[::2] + X[1::2])
                 #   negative[:,w] = X[::2] - X[1::2]
 
@@ -969,23 +996,24 @@
                         +G[i,:]*(exp(exptrm[i,:]*1-dtau[i,:]/u1) - 1.0)/(lamda[i,:]*1*u1 - 1.0)
                         +H[i,:]*(1. - exp(-exptrm[i,:]*1-dtau[i,:]/u1))/(lamda[i,:]*1*u1 + 1.0)
                         )
 
             xint_at_top[ng,nt,:] = xint[0,:]
             #intensity[ng,nt,:,:] = xint
 
-#    import IPython; IPython.embed()
-#    import sys; sys.exit()
-    return xint_at_top #, flux_out, intensity
+    return xint_at_top 
 
-@jit(nopython=True, cache=True,fastmath=True)
-def get_reflected_1d_newclima(nlevel, wno,nwno, numg,numt, dtau, tau, w0, cosb,gcos2, ftau_cld, ftau_ray,
+
+@jit(nopython=True, cache=True)
+def get_reflected_1d(nlevel, wno,nwno, numg,numt, dtau, tau, w0, cosb,gcos2, ftau_cld, ftau_ray,
     dtau_og, tau_og, w0_og, cosb_og, 
     surf_reflect,ubar0, ubar1,cos_theta, F0PI,single_phase, multi_phase,
-    frac_a, frac_b, frac_c, constant_back, constant_forward, tridiagonal,get_toa_intensity,get_lvl_flux):
+    frac_a, frac_b, frac_c, constant_back, constant_forward, 
+    get_toa_intensity=1,get_lvl_flux=0,
+    toon_coefficients=0,b_top=0):
     """
     Computes toon fluxes given tau and everything is 1 dimensional. This is the exact same function 
     as `get_flux_geom_3d` but is kept separately so we don't have to do unecessary indexing for fast
     retrievals. 
     Parameters
     ----------
     nlevel : int 
@@ -1060,23 +1088,26 @@
         of forward to back scattering (A + B * gcosb^C), Default is : 1 - gcosb^2
     constant_back : float 
         (Optional), If using the TTHG phase function. Must specify the assymetry of back scatterer. 
         Remember, the output of A & M code does not separate back and forward scattering.
     constant_forward : float 
         (Optional), If using the TTHG phase function. Must specify the assymetry of forward scatterer. 
         Remember, the output of A & M code does not separate back and forward scattering.
-    tridiagonal : int 
-        0 for tridiagonal, 1 for pentadiagonal 
+    get_toa_intensity : int 
+        (Optional) Default=1 is to only return the TOA intensity you would need for a 1D spectrum (1)
+        otherwise it will return zeros for TOA intensity 
+    get_lvl_flux : int 
+        (Optional) Default=0 is to only compute TOA intensity and NOT return the lvl fluxes so this needs 
+        to be flipped on for the climate calculations
+    toon_coefficients : int     
+        (Optional) 0 for quadrature (default) 1 for eddington
+
     Returns
     -------
     intensity at the top of the atmosphere for all the different ubar1 and ubar2 
-    To Do
-    -----
-    - F0PI Solar flux shouldn't always be 1.. Follow up to make sure that this isn't a bad 
-          hardwiring to solar, despite "relative albedo"
     """
     #these are only filled in if get_toa_intensity=1
     #outgoing intensity as a function of all the different angles
     xint_at_top = zeros(shape=(numg, numt, nwno))
 
     #these are only filled in if get_lvl_flux=1
     #fluxes at the boundaries 
@@ -1092,60 +1123,69 @@
 
     #now define terms of Toon et al 1989 quadrature Table 1 
     #https://agupubs.onlinelibrary.wiley.com/doi/pdf/10.1029/JD094iD13p16287
     #see table of terms 
 
     #terms not dependent on incident angle
     sq3 = sqrt(3.)
-    g1  = (sq3*0.5)*(2. - w0*(1.+cosb)) #table 1 # (7-w0*(4+3*cosb))/4 #
-    g2  = (sq3*w0*0.5)*(1.-cosb)        #table 1 # -(1-w0*(4-3*cosb))/4 #
+    if toon_coefficients == 1:#eddington
+        g1  = (7-w0*(4+3*ftau_cld*cosb))/4 #(sq3*0.5)*(2. - w0*(1.+cosb)) #table 1 # 
+        g2  = -(1-w0*(4-3*ftau_cld*cosb))/4 #(sq3*w0*0.5)*(1.-cosb)        #table 1 # 
+    elif toon_coefficients == 0:#quadrature
+        g1  = (sq3*0.5)*(2. - w0*(1.+ftau_cld*cosb)) #table 1 # 
+        g2  = (sq3*w0*0.5)*(1.-ftau_cld*cosb)        #table 1 # 
+
     lamda = sqrt(g1**2 - g2**2)         #eqn 21
     gama  = (g1-lamda)/g2               #eqn 22
 
     #================ START CRAZE LOOP OVER ANGLE #================
     for ng in range(numg):
         for nt in range(numt):
-
-            g3  = 0.5*(1.-sq3*cosb*ubar0[ng, nt]) #(2-3*cosb*ubar0[ng,nt])/4#  #table 1 #ubar has dimensions [gauss angles by tchebyshev angles ]
+            u1 = ubar1[ng,nt]
+            u0 = ubar0[ng,nt]
+            if toon_coefficients == 1 : #eddington
+                g3  = (2-3*ftau_cld*cosb*u0)/4#0.5*(1.-sq3*cosb*ubar0[ng, nt]) #  #table 1 #ubar has dimensions [gauss angles by tchebyshev angles ]
+            elif toon_coefficients == 0 :#quadrature
+                g3  = 0.5*(1.-sq3*ftau_cld*cosb*u0) #  #table 1 #ubar has dimensions [gauss angles by tchebyshev angles ]
     
             # now calculate c_plus and c_minus (equation 23 and 24 toon)
             g4 = 1.0 - g3
-            denominator = lamda**2 - 1.0/ubar0[ng, nt]**2.0
+            denominator = lamda**2 - 1.0/u0**2.0
 
             #everything but the exponential 
-            a_minus = F0PI*w0* (g4*(g1 + 1.0/ubar0[ng, nt]) +g2*g3 ) / denominator
-            a_plus  = F0PI*w0*(g3*(g1-1.0/ubar0[ng, nt]) +g2*g4) / denominator
+            a_minus = F0PI*w0* (g4*(g1 + 1.0/u0) +g2*g3 ) / denominator
+            a_plus  = F0PI*w0*(g3*(g1-1.0/u0) +g2*g4) / denominator
 
             #add in exponential to get full eqn
             #_up is the terms evaluated at lower optical depths (higher altitudes)
             #_down is terms evaluated at higher optical depths (lower altitudes)
-            x = exp(-tau[:-1,:]/ubar0[ng, nt])
+            x = exp(-tau[:-1,:]/u0)
             c_minus_up = a_minus*x #CMM1
             c_plus_up  = a_plus*x #CPM1
-            x = exp(-tau[1:,:]/ubar0[ng, nt])
+            x = exp(-tau[1:,:]/u0)
             c_minus_down = a_minus*x #CM
             c_plus_down  = a_plus*x #CP
 
             #calculate exponential terms needed for the tridiagonal rotated layered method
             exptrm = lamda*dtau
             #save from overflow 
             exptrm = slice_gt (exptrm, 35.0) 
 
             exptrm_positive = exp(exptrm) #EP
             exptrm_minus = 1.0/exptrm_positive#EM
 
 
             #boundary conditions 
-            b_top = 0.0                                       
+            #b_top = 0.0                                       
 
-            b_surface = 0. + surf_reflect*ubar0[ng, nt]*F0PI*exp(-tau[-1, :]/ubar0[ng, nt])
+            b_surface = 0. + surf_reflect*u0*F0PI*exp(-tau[-1, :]/u0)
 
             #Now we need the terms for the tridiagonal rotated layered method
-            if tridiagonal==0:
-                A, B, C, D = setup_tri_diag(nlayer,nwno,  c_plus_up, c_minus_up, 
+            #if tridiagonal==0:
+            A, B, C, D = setup_tri_diag(nlayer,nwno,  c_plus_up, c_minus_up, 
                                     c_plus_down, c_minus_down, b_top, b_surface, surf_reflect,
                                      gama, dtau, 
                                     exptrm_positive,  exptrm_minus) 
 
             #else:
             #   A_, B_, C_, D_, E_, F_ = setup_pent_diag(nlayer,nwno,  c_plus_up, c_minus_up, 
             #                       c_plus_down, c_minus_down, b_top, b_surface, surf_reflect,
@@ -1154,25 +1194,26 @@
 
             positive = zeros((nlayer, nwno))
             negative = zeros((nlayer, nwno))
             #========================= Start loop over wavelength =========================
             L = 2*nlayer
             for w in range(nwno):
                 #coefficient of posive and negative exponential terms 
-                if tridiagonal==0:
-                    X = tri_diag_solve(L, A[:,w], B[:,w], C[:,w], D[:,w])
-                    #unmix the coefficients
-                    positive[:,w] = X[::2] + X[1::2] 
-                    negative[:,w] = X[::2] - X[1::2]
+                #if tridiagonal==0:
+                X = tri_diag_solve(L, A[:,w], B[:,w], C[:,w], D[:,w])
+                #unmix the coefficients
+                positive[:,w] = X[::2] + X[1::2] 
+                negative[:,w] = X[::2] - X[1::2]
 
                 #else: 
                 #   X = pent_diag_solve(L, A_[:,w], B_[:,w], C_[:,w], D_[:,w], E_[:,w], F_[:,w])
                     #unmix the coefficients
                 #   positive[:,w] = exptrm_minus[:,w] * (X[::2] + X[1::2])
                 #   negative[:,w] = X[::2] - X[1::2]
+
             #========================= End loop over wavelength =========================
 
             #========================= Get fluxes if needed for climate =========================
             if get_lvl_flux: 
                 flux_minus=np.zeros(shape=(nlevel,nwno))
                 flux_plus=np.zeros(shape=(nlevel,nwno))
                 
@@ -1185,15 +1226,15 @@
                 
                 flux_zero_minus  = gama[-1,:]*positive[-1,:]*exptrm_positive[-1,:] + negative[-1,:]*exptrm_minus[-1,:] + c_minus_down[-1,:]
                 flux_zero_plus  = positive[-1,:]*exptrm_positive[-1,:] + gama[-1,:]*negative[-1,:]*exptrm_minus[-1,:] + c_plus_down[-1,:]
                 
                 flux_minus[-1, :], flux_plus[-1, :] = flux_zero_minus, flux_zero_plus 
                 
                 #add in direct flux term to the downwelling radiation, liou 182
-                flux_minus = flux_minus + ubar0[ng, nt]*F0PI*exp(-tau/ubar0[ng, nt])
+                flux_minus = flux_minus + u0*F0PI*exp(-tau/u0)
 
                 #now get midpoint values 
                 exptrm_positive_midpt = exp(0.5*exptrm) #EP
                 exptrm_minus_midpt = 1.0/exptrm_positive_midpt#EM
                 
                 #taus at the midpoint
                 taumid=tau[:-1]+0.5*dtau
@@ -1210,15 +1251,15 @@
                 flux_minus_all[ng, nt, :, :]=flux_minus
                 flux_plus_all[ng, nt, :, :]=flux_plus
                 flux_minus_midpt_all[ng, nt, :, :]=flux_minus_midpt
                 flux_plus_midpt_all[ng, nt, :, :]=flux_plus_midpt
             #========================= End get fluxes if needed for climate =========================
 
 
-            #========================= Get intensities if needed for climate =========================
+            #========================= Get intensities if needed for spectrum =========================
             if get_toa_intensity:
                 ################################ BEGIN OPTIONS FOR MULTIPLE SCATTERING####################
                 #use expression for bottom flux to get the flux_plus and flux_minus at last
                 #bottom layer
                 flux_zero  = positive[-1,:]*exptrm_positive[-1,:] + gama[-1,:]*negative[-1,:]*exptrm_minus[-1,:] + c_plus_down[-1,:]
 
 
@@ -1230,21 +1271,21 @@
                 #Legendre polynomials for the Phase function due to multiple scatterers 
                 if multi_phase ==0:#'N=2':
                     #ubar2 is defined to deal with the integration over the second moment of the 
                     #intensity. It is FIT TO PURE RAYLEIGH LIMIT, ~(1/sqrt(3))^(1/2)
                     #this is a decent assumption because our second order legendre polynomial 
                     #is forced to be equal to the rayleigh phase function
                     ubar2 = 0.767  # 
-                    multi_plus = (1.0+1.5*cosb*ubar1[ng,nt] #!was 3
-                                    + gcos2*(3.0*ubar2*ubar2*ubar1[ng,nt]*ubar1[ng,nt] - 1.0)/2.0)
-                    multi_minus = (1.-1.5*cosb*ubar1[ng,nt] 
-                                    + gcos2*(3.0*ubar2*ubar2*ubar1[ng,nt]*ubar1[ng,nt] - 1.0)/2.0)
+                    multi_plus = (1.0+1.5*ftau_cld*cosb*u1 #!was 3
+                                    + gcos2*(3.0*ubar2*ubar2*u1*u1 - 1.0)/2.0)
+                    multi_minus = (1.-1.5*ftau_cld*cosb*u1 
+                                    + gcos2*(3.0*ubar2*ubar2*u1*u1 - 1.0)/2.0)
                 elif multi_phase ==1:#'N=1':
-                    multi_plus = 1.0+1.5*cosb*ubar1[ng,nt]  
-                    multi_minus = 1.-1.5*cosb*ubar1[ng,nt]
+                    multi_plus = 1.0+1.5*ftau_cld*cosb*u1  
+                    multi_minus = 1.-1.5*ftau_cld*cosb*u1
                 ################################ end options for multiple scatteirng ####################
 
                 G=positive*(multi_plus+gama*multi_minus)    *w0
                 H=negative*(gama*multi_plus+multi_minus)    *w0
                 A=(multi_plus*c_plus_up+multi_minus*c_minus_up) *w0
 
                 G=G*0.5/pi
@@ -1304,57 +1345,74 @@
                                 (1-f) * HG_back  #second term of TTHG: backward scattering  
                                 )+  
                             ftau_ray * (
                                 0.75*(1+cos_theta**2.0) #rayleigh phase function
                                 )
                             )
                 #exploring.... 
-                elif single_phase==4:#'P(HG) exact w/ approx costheta'
-                    deltaphi=0
-                    cos_theta_approx = (-ubar0[ng,nt])*ubar1[ng,nt] + sqrt(1-ubar1[ng,nt]**2)*sqrt(1-ubar0[ng,nt]**2)*cos(deltaphi)
-                    
-                    HG_forward =  (1-g_forward**2) /sqrt((1+g_forward**2+2*g_forward*cos_theta_approx)**3)    
-                    HG_back = (1-g_back**2)/sqrt((1+g_back**2+2*g_back*cos_theta_approx)**3)
-
-                    p_single=(
-                            ftau_cld * (          #opacity of cloud / total opacity
-                                f * HG_forward  + #first term of TTHG: forward scattering
-                                (1-f) * HG_back   #second term of TTHG: backward scattering  
-                                )+  
-                            ftau_ray * (
-                                0.75*(1+cos_theta_approx**2.0) #rayleigh phase function
-                                )
-                            )
+                #elif single_phase==4:#'P(HG) exact w/ approx costheta'
+                #    deltaphi=0
+                #    cos_theta_approx = (-ubar0[ng,nt])*ubar1[ng,nt] + sqrt(1-ubar1[ng,nt]**2)*sqrt(1-ubar0[ng,nt]**2)*cos(deltaphi)
+                #    
+                #    HG_forward =  (1-g_forward**2) /sqrt((1+g_forward**2+2*g_forward*cos_theta_approx)**3)    
+                #    HG_back = (1-g_back**2)/sqrt((1+g_back**2+2*g_back*cos_theta_approx)**3)
+
+                #    p_single=(
+                #            ftau_cld * (          #opacity of cloud / total opacity
+                #                f * HG_forward  + #first term of TTHG: forward scattering
+                #                (1-f) * HG_back   #second term of TTHG: backward scattering  
+                #                )+  
+                #            ftau_ray * (
+                #                0.75*(1+cos_theta_approx**2.0) #rayleigh phase function
+                #                )
+                #            )
 
                 
                 ################################ end options for direct scattering ####################
 
+                #in codes like DISORT the single and multiple scattering beams are reported separately
+                #in Rooney et al. 2023a we needed to separate these to 
+                #single_scat = zeros((nlevel,nwno))
+                #multi_scat = zeros((nlevel,nwno))
                 for i in range(nlayer-1,-1,-1):
+                    #single_scat[i,:] = ((w0_og[i,:]*F0PI/(4.*pi))
+                    #        *(p_single[i,:])*exp(-tau_og[i,:]/u0)
+                    #        *(1. - exp(-dtau_og[i,:]*(u0+u1)
+                    #        /(u0*u1)))*
+                    #        (u0/(u0+u1)))
+
+                    #multi_scat[i,:] = (A[i,:]*(1. - exp(-dtau[i,:] *(u0+1*u1)/(u0*u1)))*
+                    #        (u0/(u0+1*u1))
+                    #        +G[i,:]*(exp(exptrm[i,:]*1-dtau[i,:]/u1) - 1.0)/(lamda[i,:]*1*u1 - 1.0)
+                    #        +H[i,:]*(1. - exp(-exptrm[i,:]*1-dtau[i,:]/u1))/(lamda[i,:]*1*u1 + 1.0)
+                    #        )
+
                     #direct beam
-                    xint[i,:] =( xint[i+1,:]*exp(-dtau[i,:]/ubar1[ng,nt]) 
+                    xint[i,:] =( xint[i+1,:]*exp(-dtau[i,:]/u1) 
                             #single scattering albedo from sun beam (from ubar0 to ubar1)
                             +(w0_og[i,:]*F0PI/(4.*pi))
-                            *(p_single[i,:])*exp(-tau_og[i,:]/ubar0[ng,nt])
-                            *(1. - exp(-dtau_og[i,:]*(ubar0[ng,nt]+ubar1[ng,nt])
-                            /(ubar0[ng,nt]*ubar1[ng,nt])))*
-                            (ubar0[ng,nt]/(ubar0[ng,nt]+ubar1[ng,nt]))
+                            *(p_single[i,:])*exp(-tau_og[i,:]/u0)
+                            *(1. - exp(-dtau_og[i,:]*(u0+u1)
+                            /(u0*u1)))*
+                            (u0/(u0+u1))
                             #multiple scattering terms p_single
-                            +A[i,:]*(1. - exp(-dtau[i,:] *(ubar0[ng,nt]+1*ubar1[ng,nt])/(ubar0[ng,nt]*ubar1[ng,nt])))*
-                            (ubar0[ng,nt]/(ubar0[ng,nt]+1*ubar1[ng,nt]))
-                            +G[i,:]*(exp(exptrm[i,:]*1-dtau[i,:]/ubar1[ng,nt]) - 1.0)/(lamda[i,:]*1*ubar1[ng,nt] - 1.0)
-                            +H[i,:]*(1. - exp(-exptrm[i,:]*1-dtau[i,:]/ubar1[ng,nt]))/(lamda[i,:]*1*ubar1[ng,nt] + 1.0)
+                            +A[i,:]*(1. - exp(-dtau[i,:] *(u0+1*u1)/(u0*u1)))*
+                            (u0/(u0+1*u1))
+                            +G[i,:]*(exp(exptrm[i,:]*1-dtau[i,:]/u1) - 1.0)/(lamda[i,:]*1*u1 - 1.0)
+                            +H[i,:]*(1. - exp(-exptrm[i,:]*1-dtau[i,:]/u1))/(lamda[i,:]*1*u1 + 1.0)
                             )
 
+
                 xint_at_top[ng,nt,:] = xint[0,:]
-            #========================= End get intensities if needed for climate =========================
+            #========================= End get intensities if needed for spectrum =========================
     
     return xint_at_top, (flux_minus_all, flux_plus_all, flux_minus_midpt_all, flux_plus_midpt_all )
-
-@jit(nopython=True, cache=True,fastmath=True)
-def get_reflected_1d_gfluxv(nlevel, wno,nwno, numg,numt, dtau, tau, w0, cosb,
+    
+@jit(nopython=True, cache=True)
+def get_reflected_1d_gfluxv_deprecate(nlevel, wno,nwno, numg,numt, dtau, tau, w0, cosb,
     surf_reflect,b_top,b_surface,ubar0, F0PI,tridiagonal, delta_approx):
     """
     Computes upwelling and downwelling layer and level toon fluxes given tau and everything is 1 dimensional. This is the exact same function 
     as `GFLUXV.f'.
     retrievals. 
     Parameters
     ----------
@@ -1388,15 +1446,14 @@
         Surface reflectivity
     b_top : float 
         Top Boundary Conditions
     b_surface : float 
         Surface Boundary Conditions
     ubar0 : ndarray of float 
         matrix of cosine of the incident angle from geometric.json
-    
     F0PI : array 
         Downward incident solar radiation
     delta_approx : int 
         0 for no Delta Approx, 1 for Delta Approx
     Returns
     -------
     intensity at the top of the atmosphere for all the different ubar1 and ubar2 
@@ -1431,18 +1488,15 @@
     flux_plus_all = zeros(shape=(numg, numt, nlevel, nwno)) ## --SM-- level upwelling fluxes
     flux_minus_midpt_all = zeros(shape=(numg, numt, nlevel, nwno)) ## --SM-- layer downwelling fluxes
     flux_plus_midpt_all = zeros(shape=(numg, numt, nlevel, nwno))  ## --SM-- layer upwelling fluxes
     
     #now define terms of Toon et al 1989 quadrature Table 1 
     #https://agupubs.onlinelibrary.wiley.com/doi/pdf/10.1029/JD094iD13p16287
     #see table of terms 
-    
-    
-    
-    
+
     #terms not dependent on incident angle
     
     
     sq3 = sqrt(3.)
     g1  = (sq3*0.5)*(2. - w0*(1.+cosb)) #table 1 # (7-w0*(4+3*cosb))/4 #
     g2  = (sq3*w0*0.5)*(1.-cosb)        #table 1 # -(1-w0*(4-3*cosb))/4 #
     lamda = sqrt(g1**2 - g2**2)         #eqn 21
@@ -1542,40 +1596,91 @@
             
 
             flux_minus_midpt_all[ng, nt, :, :]=flux_minus_midpt
             flux_plus_midpt_all[ng, nt, :, :]=flux_plus_midpt
     
     return flux_minus_all, flux_plus_all, flux_minus_midpt_all, flux_plus_midpt_all 
 
+@jit(nopython=True, cache=True)
+def blackbody_integrated(T, wave, dwave):
+    """
+    This computes the total energey per wavenumber bin needed for the climate calculation 
+    Note that this is different than the raw flux at an isolated wavenumber. Therefore this function is 
+    different than the blackbody function in `picaso.fluxes` which computes blackbody in raw 
+    cgs units. 
+    
+    Parameters 
+    ----------
+    T : float, array 
+        temperature in Kelvin 
+    wave : float, array 
+        wavenumber in cm-1 
+    dwave : float, array 
+        Wavenumber bins in cm-1 
+    
+    Returns 
+    -------
+    array 
+        num temperatures by num wavenumbers 
+        units of ergs/cm*2/s/cm-1 for *integrated* bins ()
+    """
 
-@jit(nopython=True, cache=True,fastmath=True)
+    h = 6.62607004e-27 # erg s 
+    c = 2.99792458e+10 # cm/s
+    k = 1.38064852e-16 #erg / K
+    c1 = 2*h*c**2
+    c2 = h*c/k
+    
+    #this number was tested for accuracy against the original number of bins (4)
+    #nbb 1 create three wavenumber bins (one on either side of center)
+    #It achieves <1% integration accuracy up to black bodies ~50 K for the 
+    #legacy 196 and 661 (for 661 max error is only 1e-3%) wavenumber grids. 
+    nbb = 1 
+
+    num_wave = len(wave)
+    num_T = len(T)
+
+    planck_sum = zeros((num_T, num_wave))
+
+    for i in range(num_wave):
+        for j in range(num_T):
+            for k in range(-nbb, nbb + 1, 1):
+                wavenum = wave[i] + k * dwave[i] / (2.0 * nbb)
+                #erg/s/cm2/(cm-1)
+                planck_sum[j, i] += c1 * (wavenum**3) / (exp(c2 * wavenum / T[j])-1)
+                
+    planck_sum /= (2 * nbb + 1.0)
+
+    return planck_sum
+
+@jit(nopython=True, cache=True)
 def blackbody(t,w):
     """
-    Blackbody flux in cgs units in per unit wavelength
+    Blackbody flux in cgs units in per unit wavelength (cm)
 
     Parameters
     ----------
     t : array,float
         Temperature (K)
     w : array, float
         Wavelength (cm)
     
     Returns
     -------
-    ndarray with shape ntemp x numwave
+    ndarray with shape ntemp x numwave in units of erg/cm/s2/cm
     """
     h = 6.62607004e-27 # erg s 
     c = 2.99792458e+10 # cm/s
     k = 1.38064852e-16 #erg / K
 
     return ((2.0*h*c**2.0)/(w**5.0))*(1.0/(exp((h*c)/outer(t, w*k)) - 1.0)) #* (w*w)
 
 @jit(nopython=True, cache=True)
-def get_thermal_1d_newclima(nlevel, wno,nwno, numg,numt,tlevel, dtau, w0,cosb,plevel, ubar1,
-    surf_reflect, hard_surface, tridiagonal):
+def get_thermal_1d(nlevel, wno,nwno, numg,numt,tlevel, dtau, w0,cosb,plevel, ubar1,
+    surf_reflect, hard_surface, dwno, calc_type):
     """
     This function uses the source function method, which is outlined here : 
     https://agupubs.onlinelibrary.wiley.com/doi/pdf/10.1029/JD094iD13p16287
     
     The result of this routine is the top of the atmosphere thermal flux as 
     a function of gauss and chebychev points accross the disk. 
 
@@ -1619,101 +1724,127 @@
     ubar1 : numpy.ndarray
         This is a matrix of ng by nt. This describes the outgoing incident angles and is generally
         computed in `picaso.disco`
     surf_reflect : numpy.ndarray    
         Surface reflectivity as a function of wavenumber. 
     hard_surface : int
         0 for no hard surface (e.g. Jupiter/Neptune), 1 for hard surface (terrestrial)
-    tridiagonal : int 
-        0 for tridiagonal, 1 for pentadiagonal
-
+    dwno : int 
+        delta wno needed for climate
+    calc_type : int 
+        0 for spectrum model, 1 for climate solver
     Returns
     -------
     numpy.ndarray
         Thermal flux in CGS units (erg/cm3/s) in a matrix that is 
         numg x numt x nwno
     """
     nlayer = nlevel - 1 #nlayers 
 
     mu1 = 0.5#0.88#0.5 #from Table 1 Toon  
-    twopi = pi#+pi #NEB REMOVING A PI FROM HERE BECAUSE WE ASSUME NO SYMMETRY! 
 
     #get matrix of blackbodies 
-    all_b = blackbody(tlevel, 1/wno) #returns nlevel by nwave   
+    if calc_type == 0: 
+        all_b = blackbody(tlevel, 1/wno) #returns nlevel by nwave   
+    elif calc_type==1:
+        all_b = blackbody_integrated(tlevel, wno, dwno)
+
     b0 = all_b[0:-1,:]
     b1 = (all_b[1:,:] - b0) / dtau # eqn 26 toon 89
 
-    #hemispheric mean parameters from Tabel 1 toon 
-    #**originally written in terms of alpha which isn't in the table. 
-    #**changed to more closely resemble Toon (no change in actual values)
+    #hemispheric mean parameters from Tabe 1 toon 
+    g1 = 2.0 - w0*(1+cosb); g2 = w0*(1-cosb)
+
     alpha = sqrt( (1.-w0) / (1.-w0*cosb) )
-    g1 = 2 - w0*(1 + cosb) # (7-w0*(4+3*cosb))/4  # 
-    g2 = w0*(1 - cosb)     # -(1-w0*(4-3*cosb))/4 # 
-    lamda = alpha*(1.-w0*cosb)/mu1 #(g1**2 - g2**2)**0.5 #eqn 21 toon
-    gama = (1.-alpha)/(1.+alpha) #g2 / (g1 + lamda) #eqn 22 toon
-    g1_plus_g2 = mu1/(1.-w0*cosb) #effectively 1/(gamma1 + gamma2) .. second half of eqn.27
+    lamda = sqrt(g1**2 - g2**2) #eqn 21 toon 
+    gama = (g1-lamda)/g2 # #eqn 22 toon
+    
+    g1_plus_g2 = 1.0/(g1+g2) #second half of eqn.27
 
     #same as with reflected light, compute c_plus and c_minus 
     #these are eqns 27a & b in Toon89
     #_ups are evaluated at lower optical depth, TOA
     #_dows are evaluated at higher optical depth, bottom of atmosphere
-    c_plus_up = b0 + b1* g1_plus_g2 
-    c_minus_up = b0 - b1* g1_plus_g2
+    c_plus_up = 2*pi*mu1*(b0 + b1* g1_plus_g2) 
+    c_minus_up = 2*pi*mu1*(b0 - b1* g1_plus_g2)
+    #NOTE: to keep consistent with Toon, we keep these 2pis here. However, 
+    #in 3d cases where we no long assume azimuthal symmetry, we divide out 
+    #by 2pi when we multiply out the weights as seen in disco.compress_thermal 
+
+    c_plus_down = 2*pi*mu1*(b0 + b1 * dtau + b1 * g1_plus_g2) 
+    c_minus_down = 2*pi*mu1*(b0 + b1 * dtau - b1 * g1_plus_g2)
+
 
-    c_plus_down = (b0 + b1 * dtau + b1 * g1_plus_g2)
-    c_minus_down = (b0 + b1 * dtau - b1 * g1_plus_g2)
-    # note there should be a factor of 2mu1 in c expressions, need to include that if mu1 not 0.5
 
     #calculate exponential terms needed for the tridiagonal rotated layered method
     exptrm = lamda*dtau
     #save from overflow 
     exptrm = slice_gt (exptrm, 35.0) 
 
     exptrm_positive = exp(exptrm) 
     exptrm_minus = 1.0/exptrm_positive
 
+    #for flux heating calculations, the energy balance solver 
+    #does not like a fixed zero at the TOA. 
+    #to avoid a discontinuous kink at the last atmospher
+    #layer we create this "fake" boundary condition
+    #we imagine that the atmosphere continus up at an isothermal T and that 
+    #there is optical depth from above the top to infinity 
     tau_top = dtau[0,:]*plevel[0]/(plevel[1]-plevel[0]) #tried this.. no luck*exp(-1)# #tautop=dtau[0]*np.exp(-1)
-    b_top = (1.0 - exp(-tau_top / mu1 )) * all_b[0,:]  # Btop=(1.-np.exp(-tautop/ubari))*B[0]
+    #print(list(tau_top))
+    #tau_top = 26.75*plevel[0]/(plevel[1]-plevel[0]) 
+    b_top = (1.0 - exp(-tau_top / mu1 )) * all_b[0,:] * pi #  Btop=(1.-np.exp(-tautop/ubari))*B[0]
+    
     if hard_surface:
-        b_surface = all_b[-1,:] #for terrestrial, hard surface  
+        b_surface = all_b[-1,:]*pi #for terrestrial, hard surface  
     else: 
-        b_surface=all_b[-1,:] + b1[-1,:]*mu1 #(for non terrestrial)
+        b_surface= (all_b[-1,:] + b1[-1,:]*mu1)*pi #(for non terrestrial)
 
     #Now we need the terms for the tridiagonal rotated layered method
-    if tridiagonal==0:
-        A, B, C, D = setup_tri_diag(nlayer,nwno,  c_plus_up, c_minus_up, 
-                            c_plus_down, c_minus_down, b_top, b_surface, surf_reflect,
-                             gama, dtau, 
-                            exptrm_positive,  exptrm_minus) 
+    #pentadiagonal solver is left here because it may be useful someday 
+    #however, curret scipy implementation is too slow to use currently 
+    #if tridiagonal==0:
+    A, B, C, D = setup_tri_diag(nlayer,nwno,  c_plus_up, c_minus_up, 
+                        c_plus_down, c_minus_down, b_top, b_surface, surf_reflect,
+                         gama, dtau, 
+                        exptrm_positive,  exptrm_minus) 
+    #else:
+    #   A_, B_, C_, D_, E_, F_ = setup_pent_diag(nlayer,nwno,  c_plus_up, c_minus_up, 
+    #                       c_plus_down, c_minus_down, b_top, b_surface, surf_reflect,
+    #                        gama, dtau, 
+    #                       exptrm_positive,  exptrm_minus, g1,g2,exptrm,lamda) 
     positive = zeros((nlayer, nwno))
     negative = zeros((nlayer, nwno))
+
     #========================= Start loop over wavelength =========================
     L = nlayer+nlayer
     for w in range(nwno):
         #coefficient of posive and negative exponential terms 
-        if tridiagonal==0:
-            X = tri_diag_solve(L, A[:,w], B[:,w], C[:,w], D[:,w])
-            #unmix the coefficients
-            positive[:,w] = X[::2] + X[1::2] 
-            negative[:,w] = X[::2] - X[1::2]
+        X = tri_diag_solve(L, A[:,w], B[:,w], C[:,w], D[:,w])
+        #unmix the coefficients
+        positive[:,w] = X[::2] + X[1::2] 
+        negative[:,w] = X[::2] - X[1::2]
+        #else:
+        #   X = pent_diag_solve(L, A_[:,w], B_[:,w], C_[:,w], D_[:,w], E_[:,w], F_[:,w])
+        #   positive[:,w] = exptrm_minus[:,w] * (X[::2] + X[1::2])
+        #   negative[:,w] = X[::2] - X[1::2]
 
     #if you stop here this is regular ole 2 stream
-    f_up = pi*(positive * exptrm_positive + gama * negative * exptrm_minus + c_plus_up)
-
+    f_up = (positive * exptrm_positive + gama * negative * exptrm_minus + c_plus_up)
 
     #calculate everyting from Table 3 toon
-    alphax = ((1.0-w0)/(1.0-w0*cosb))**0.5
-    G = twopi*w0*positive*(1.0+cosb*alphax)/(1.0+alphax)#
-    H = twopi*w0*negative*(1.0-cosb*alphax)/(1.0+alphax)#
-    J = twopi*w0*positive*(1.0-cosb*alphax)/(1.0+alphax)#
-    K = twopi*w0*negative*(1.0+cosb*alphax)/(1.0+alphax)#
-    alpha1 = twopi*(b0+ b1*(mu1*w0*cosb/(1.0-w0*cosb)))
-    alpha2 = twopi*b1
-    sigma1 = twopi*(b0- b1*(mu1*w0*cosb/(1.0-w0*cosb)))
-    sigma2 = twopi*b1
+    #from here forward is source function technique in toon
+    G = (1/mu1 - lamda)*positive     
+    H = gama*(lamda + 1/mu1)*negative 
+    J = gama*(lamda + 1/mu1)*positive 
+    K = (1/mu1 - lamda)*negative     
+    alpha1 = 2*pi*(b0+b1*(g1_plus_g2 - mu1)) 
+    alpha2 = 2*pi*b1 
+    sigma1 = 2*pi*(b0-b1*(g1_plus_g2 - mu1)) 
+    sigma2 = 2*pi*b1 
 
     flux_minus = zeros((numg, numt,nlevel,nwno))
     flux_plus = zeros((numg, numt,nlevel,nwno))
     flux_minus_mdpt = zeros((numg, numt,nlevel,nwno))
     flux_plus_mdpt = zeros((numg, numt,nlevel,nwno))
 
     exptrm_positive_mdpt = exp(0.5*exptrm) 
@@ -1726,19 +1857,19 @@
     #work through building eqn 55 in toon (tons of bookeeping exponentials)
     for ng in range(numg):
         for nt in range(numt): 
 
             iubar = ubar1[ng,nt]
 
             if hard_surface:
-                flux_plus[ng,nt,-1,:] = twopi * (b_surface ) # terrestrial
+                flux_plus[ng,nt,-1,:] = all_b[-1,:] *2*pi  # terrestrial flux /pi = intensity
             else:
-                flux_plus[ng,nt,-1,:] = twopi*( all_b[-1,:] + b1[-1,:] * iubar) #no hard surface
+                flux_plus[ng,nt,-1,:] = ( all_b[-1,:] + b1[-1,:] * iubar)*2*pi #no hard surface   
                 
-            flux_minus[ng,nt,0,:] = twopi * (1 - exp(-tau_top / iubar)) * all_b[0,:]
+            flux_minus[ng,nt,0,:] = (1 - exp(-tau_top / iubar)) * all_b[0,:] *2*pi
             
             exptrm_angle = exp( - dtau / iubar)
             exptrm_angle_mdpt = exp( -0.5 * dtau / iubar) 
 
             for itop in range(nlayer):
 
                 #disbanning this for now because we dont need it in the thermal emission code
@@ -1770,15 +1901,15 @@
 
 
             flux_at_top[ng,nt,:] = flux_plus_mdpt[ng,nt,0,:] #nlevel by nwno 
 
     return flux_at_top , (flux_minus, flux_plus, flux_minus_mdpt, flux_plus_mdpt)
 
 @jit(nopython=True, cache=True)
-def get_thermal_1d(nlevel, wno,nwno, numg,numt,tlevel, dtau, w0,cosb,plevel, ubar1,
+def get_thermal_1d_deprecate(nlevel, wno,nwno, numg,numt,tlevel, dtau, w0,cosb,plevel, ubar1,
     surf_reflect, hard_surface, tridiagonal):
     """
     This function uses the source function method, which is outlined here : 
     https://agupubs.onlinelibrary.wiley.com/doi/pdf/10.1029/JD094iD13p16287
     
     The result of this routine is the top of the atmosphere thermal flux as 
     a function of gauss and chebychev points accross the disk. 
@@ -2004,15 +2135,15 @@
             #flux_minus_mdpt_disco[ng,nt,:,:] = flux_minus_mdpt #nlevel by nwno
             #flux_plus_mdpt_disco[ng,nt,:,:] = int_plus_mdpt #nlevel by nwno
 
     return int_at_top #, intensity, flux_out #, int_down# numg x numt x nwno
 
 @jit(nopython=True, cache=True)
 def get_thermal_3d(nlevel, wno,nwno, numg,numt,tlevel_3d, dtau_3d, w0_3d,cosb_3d,plevel_3d, ubar1,
-    surf_reflect, hard_surface, tridiagonal):
+    surf_reflect, hard_surface):
     """
     This function uses the source function method, which is outlined here : 
     https://agupubs.onlinelibrary.wiley.com/doi/pdf/10.1029/JD094iD13p16287
     
     The result of this routine is the top of the atmosphere thermal flux as 
     a function of gauss and chebychev points accross the disk. 
     Everything here is in CGS units:
@@ -2051,16 +2182,15 @@
         that is sometimes included in reflected light calculations.
         This 4d matrix has dimensions [nlevel, nwave,ngangle,ntangle].
     plevel : numpy.ndarray
         Pressure for each level (not layer, which is midpoints). CGS units (dyne/cm2)
     ubar1 : numpy.ndarray
         This is a matrix of ng by nt. This describes the outgoing incident angles and is generally
         computed in `picaso.disco`
-    tridiagonal : int 
-        Zero for tridiagonal solver. 1 for pentadiagonal (not yet implemented)
+
     Returns
     -------
     numpy.ndarray
         Thermal flux in CGS units (erg/cm3/s) in a matrix that is 
         numg x numt x nwno
     """ 
 
@@ -2116,36 +2246,36 @@
             b_top = pi*(1.0 - exp(-tau_top / mu1 )) * all_b[0,:] 
             
             if hard_surface:
                 b_surface = pi*all_b[-1,:] #for terrestrial, hard surface  
             else: 
                 b_surface= pi*(all_b[-1,:] + b1[-1,:]*mu1) #(for non terrestrial)
             #Now we need the terms for the tridiagonal rotated layered method
-            if tridiagonal==0:
-                A, B, C, D = setup_tri_diag(nlayer,nwno,  c_plus_up, c_minus_up, 
-                                    c_plus_down, c_minus_down, b_top, b_surface, surf_reflect,
-                                     gama, dtau, 
-                                    exptrm_positive,  exptrm_minus) 
+            #if tridiagonal==0:
+            A, B, C, D = setup_tri_diag(nlayer,nwno,  c_plus_up, c_minus_up, 
+                                c_plus_down, c_minus_down, b_top, b_surface, surf_reflect,
+                                 gama, dtau, 
+                                exptrm_positive,  exptrm_minus) 
             #else:
             #   A_, B_, C_, D_, E_, F_ = setup_pent_diag(nlayer,nwno,  c_plus_up, c_minus_up, 
             #                       c_plus_down, c_minus_down, b_top, b_surface, surf_reflect,
             #                        gama, dtau, 
             #                       exptrm_positive,  exptrm_minus, g1,g2,exptrm,lamda) 
 
             positive = zeros((nlayer, nwno))
             negative = zeros((nlayer, nwno))
             #========================= Start loop over wavelength =========================
             L = nlayer+nlayer
             for w in range(nwno):
                 #coefficient of posive and negative exponential terms 
-                if tridiagonal==0:
-                    X = tri_diag_solve(L, A[:,w], B[:,w], C[:,w], D[:,w])
-                    #unmix the coefficients
-                    positive[:,w] = X[::2] + X[1::2] #Y1+Y2 in toon (table 3)
-                    negative[:,w] = X[::2] - X[1::2] #Y1-Y2 in toon (table 3)
+                #if tridiagonal==0:
+                X = tri_diag_solve(L, A[:,w], B[:,w], C[:,w], D[:,w])
+                #unmix the coefficients
+                positive[:,w] = X[::2] + X[1::2] #Y1+Y2 in toon (table 3)
+                negative[:,w] = X[::2] - X[1::2] #Y1-Y2 in toon (table 3)
                 #else:
                 #   X = pent_diag_solve(L, A_[:,w], B_[:,w], C_[:,w], D_[:,w], E_[:,w], F_[:,w])
                 #   positive[:,w] = exptrm_minus[:,w] * (X[::2] + X[1::2])
                 #   negative[:,w] = X[::2] - X[1::2]
 
             f_up = (positive * exptrm_positive + gama * negative * exptrm_minus + c_plus_up)
 
@@ -2211,15 +2341,16 @@
 
             int_at_top[ng,nt,:] = int_plus_mdpt[0,:] #nlevel by nwno
             #int_down[ng,nt,:] = int_minus_mdpt[0,:] #nlevel by nwno, Dont really need to compute this for now
 
     return int_at_top #, int_down# numg x numt x nwno
 
 @jit(nopython=True, cache=True)
-def get_thermal_1d_gfluxi(nlevel, wno,nwno, numg,numt,tlevel, dtau, w0,cosb,plevel, ubar1,surf_reflect,ugauss_angles,ugauss_weights, tridiagonal, calc_type , bb , y2, tp, tmin, tmax):
+def get_thermal_1d_gfluxi_deprecate(nlevel, wno,nwno, numg,numt,tlevel, dtau, w0,cosb,plevel, ubar1,surf_reflect,ugauss_angles,ugauss_weights, tridiagonal, calc_type ,dwno): 
+    #bb , y2, tp, tmin, tmax):
     """
     This function uses the source function method, which is outlined here : 
     https://agupubs.onlinelibrary.wiley.com/doi/pdf/10.1029/JD094iD13p16287
     
     The result of this routine is the top of the atmosphere thermal flux as 
     a function of gauss and chebychev points accross the disk. 
     Everything here is in CGS units:
@@ -2287,19 +2418,25 @@
     flux_minus_midpt_all = zeros(( nlevel, nwno)) ##  layer downwelling fluxes
     flux_plus_midpt_all = zeros(( nlevel, nwno))  ## layer upwelling fluxes
 
     mu1 = 0.5#0.88#0.5 #from Table 1 Toon  
     twopi = 2*pi#+pi #NEB REMOVING A PI FROM HERE BECAUSE WE ASSUME NO SYMMETRY!  ############
 
     #get matrix of blackbodies 
-    all_b = blackbody_climate(wno, tlevel, bb, y2, tp, tmin, tmax) #returns nlevel by nwave 
-    
+    #all_b = blackbody_climate_deprecate(wno, tlevel, bb, y2, tp, tmin, tmax) #returns nlevel by nwave 
+    all_b = blackbody_integrated(tlevel, wno, dwno)
+
     b0 = all_b[0:-1,:]
     b1 = (all_b[1:,:] - b0) / dtau # eqn 26 toon 89
 
+    #if dtau is less than 1e-6 set b1 to zero 
+    #neb-was in fortran but doesnt look needed, keep for now
+    #b1 = slice_lt_cond(b1, dtau, 1e-6, 0.0)
+    #b0 = slice_lt_cond_arr(b0, dtau, 1e-6, all_b)
+
     #hemispheric mean parameters from Tabe 1 toon 
     alpha = sqrt( (1.-w0) / (1.-w0*cosb) )
     lamda = alpha*(1.-w0*cosb)/mu1 #eqn 21 toon
     gama = (1.-alpha)/(1.+alpha) #eqn 22 toon
     g1_plus_g2 = mu1/(1.-w0*cosb) #effectively 1/(gamma1 + gamma2) .. second half of eqn.27
 
     #same as with reflected light, compute c_plus and c_minus 
@@ -2316,14 +2453,15 @@
     exptrm = lamda*dtau
     #save from overflow 
     exptrm = slice_gt (exptrm, 35.0) 
 
     exptrm_positive = exp(exptrm) 
     exptrm_minus = 1.0/exptrm_positive
 
+    #*
     tau_top = dtau[0,:]*plevel[0]/(plevel[1]-plevel[0]) #tried this.. no luck*exp(-1)# #tautop=dtau[0]*np.exp(-1)
     b_top = (1.0 - exp(-tau_top / mu1 )) * all_b[0,:]  # Btop=(1.-np.exp(-tautop/ubari))*B[0]
     #b_surface = all_b[-1,:] #for terrestrial, hard surface  
     b_surface=all_b[-1,:] + b1[-1,:]*mu1 #(for non terrestrial)
 
     #Now we need the terms for the tridiagonal rotated layered method
     if tridiagonal==0:
@@ -3585,15 +3723,15 @@
 	Chapman function
     
     """
 
     chapman_func = exp(1.0+ hratio*log(pressure/pm)- (pressure/pm)**hratio) 
     return chapman_func
 
-def set_bb(wno,delta_wno,nwno,ntmps,dt,tmin,tmax):
+def set_bb_deprecate(wno,delta_wno,nwno,ntmps,dt,tmin,tmax):
     """
     Function to compute a grid of black bodies before the code runs. 
     This allows us to interpolate on a blackbody instead of computing the planck 
     function repetitively. This was done because historically computing the 
     planck function was a bottleneck in speed. 
 
     Parameters
@@ -3627,35 +3765,35 @@
     tp= np.zeros(shape=(ntmps))
     y2=np.zeros(shape=(ntmps,nwno))
     for it in range(ntmps):
         temp_bb = tmin +(it)*dt
         tp[it]= temp_bb
     #GET RID OF PLACK CGS     
         for ik in range(nwno):
-            x= planck_cgs(wno[ik],temp_bb,delta_wno[ik])
+            x= planck_cgs_deprecate(wno[ik],temp_bb,delta_wno[ik])
             if x > 0.0 :
                 bb[it,ik] = log(x)
             else:
                 bb[it,ik] = -700.0
     
     dts = 0.02
     for ik in range(nwno):
-        yp_n= (-bb[ntmps-1,ik]+log(planck_cgs(wno[ik],tmax+dts,delta_wno[ik])))/dts
-        yp_0 = (-bb[0,ik]+log(planck_cgs(wno[ik],tmin+dts,delta_wno[ik])))/dts
+        yp_n= (-bb[ntmps-1,ik]+log(planck_cgs_deprecate(wno[ik],tmax+dts,delta_wno[ik])))/dts
+        yp_0 = (-bb[0,ik]+log(planck_cgs_deprecate(wno[ik],tmin+dts,delta_wno[ik])))/dts
         
         pass0=bb[:,ik]
 
-        y2x = spline(tp,pass0,ntmps,yp_0,yp_n)
+        y2x = spline_deprecate(tp,pass0,ntmps,yp_0,yp_n)
         
         
         y2[:,ik] = y2x
     
     return bb , y2 , tp
 
-def spline(x , y, n, yp0, ypn):
+def spline_deprecate(x , y, n, yp0, ypn):
     
     u=np.zeros(shape=(n))
     y2 = np.zeros(shape=(n))
 
     if yp0 > 0.99 :
         y2[0] = 0.0
         u[0] =0.0
@@ -3679,15 +3817,15 @@
     y2[n-1] = (un - qn*u[n-2])/(qn*y2[n-2]+1.0)
 
     for k in range(n-2, -1, -1):
         y2[k] = y2[k] * y2[k+1] +u[k]
     
     return y2
 
-def planck_cgs(wave, T , dwave):
+def planck_cgs_deprecate(wave, T , dwave):
     # PLANCK FUNCTION RETURNS B IN CGS UNITS, ERGS CM-2 WAVENUMBER-1
     # wave IS WAVENUMBER IN CM-1
     # T IS IN KELVIN
     nbb = 4
 
     planck_sum = 0.0
 
@@ -3697,16 +3835,16 @@
     planck_sum = planck_sum/(2*nbb +1.0)
     if planck_sum <= 1e-300:
         planck_sum = 1e-300
     
     return planck_sum
 
 
-@jit(nopython=True, cache=True,fastmath=True)
-def planck_rad(iw, T, dT ,  tmin, tmax, bb , y2, tp):
+@jit(nopython=True, cache=True)
+def planck_rad_deprecate(iw, T, dT ,  tmin, tmax, bb , y2, tp):
 
     if T < tmin :
        # itchx = 1
         T= tmax
     elif T > tmax :
        # itchx = 1
         T=tmax
@@ -3721,22 +3859,22 @@
     
     planck_rad = exp(planck_rad)
 
     return planck_rad
 
 
 @jit(nopython=True, cache=True)
-def blackbody_climate(wave,temp, bb, y2, tp, tmin, tmax):
+def blackbody_climate_deprecate(wave,temp, bb, y2, tp, tmin, tmax):
 
     blackbody_array = np.zeros(shape=(len(temp),len(wave)))
     dT= 2.5
 
     for itemp in range(len(temp)):
         for iwave in range(len(wave)):
-            blackbody_array[itemp, iwave] = planck_rad(iwave, temp[itemp], dT ,  tmin, tmax, bb , y2, tp)
+            blackbody_array[itemp, iwave] = planck_rad_deprecate(iwave, temp[itemp], dT ,  tmin, tmax, bb , y2, tp)
 
     return blackbody_array
 
 # still not developed fully. virga has a function already maybe just use that
 @jit(nopython=True, cache=True)
 def get_kzz(pressure, temp,grav,mmw,tidal,flux_net_ir_layer, flux_plus_ir_attop,t_table, p_table, grad, cp, calc_type,nstr):
```

### Comparing `picaso-3.1.2/picaso/io_utils.py` & `picaso-3.2/picaso/io_utils.py`

 * *Files identical despite different names*

### Comparing `picaso-3.1.2/picaso/justdoit.py` & `picaso-3.2/picaso/justdoit.py`

 * *Files 4% similar despite different names*

```diff
@@ -1,23 +1,24 @@
 from .atmsetup import ATMSETUP
-from .fluxes import get_reflected_1d, get_reflected_3d , get_thermal_1d, get_thermal_3d, get_reflected_SH, get_transit_1d, get_thermal_SH
+from .fluxes import get_reflected_1d, get_reflected_3d , get_thermal_1d, get_thermal_3d, get_reflected_SH, get_thermal_SH,get_transit_1d
 
-from .fluxes import set_bb, tidal_flux, get_kzz
-from .climate import  calculate_atm_deq, did_grad_cp, convec, calculate_atm, t_start, growdown, growup, climate
+from .fluxes import tidal_flux, get_kzz#,set_bb_deprecate 
+from .climate import  calculate_atm_deq, did_grad_cp, convec, calculate_atm, t_start, growdown, growup, get_fluxes
 
 from .wavelength import get_cld_input_grid
 from .optics import RetrieveOpacities,compute_opacity,RetrieveCKs
 from .disco import get_angles_1d, get_angles_3d, compute_disco, compress_disco, compress_thermal
 from .justplotit import numba_cumsum, find_nearest_2d, mean_regrid
 from .deq_chem import quench_level,initiate_cld_matrices
-#from .vulcan import run_vulcan_chem
 from .build_3d_input import regrid_xarray
+from .photochem import run_photochem
+
 
 from virga import justdoit as vj
-from scipy.interpolate import UnivariateSpline
+from scipy.interpolate import UnivariateSpline, interp1d
 from scipy import special
 from numpy import exp, sqrt,log
 from numba import jit,njit
 from scipy.io import FortranFile
 
 
 import os
@@ -34,34 +35,36 @@
 import astropy.units as u
 import astropy.constants as c
 from astropy.utils.misc import JsonCustomEncoder
 import math
 import xarray as xr
 from joblib import Parallel, delayed, cpu_count
 
+# #testing error tracker
+# from loguru import logger 
 __refdata__ = os.environ.get('picaso_refdata')
-__version__ = 3.1
+__version__ = 3.2
 
 
 if not os.path.exists(__refdata__): 
     raise Exception("You have not downloaded the PICASO reference data. You can find it on github here: https://github.com/natashabatalha/picaso/tree/master/reference . If you think you have already downloaded it then you likely just need to set your environment variable. See instructions here: https://natashabatalha.github.io/picaso/installation.html#download-and-link-reference-documentation . You can use `os.environ['PYSYN_CDBS']=<yourpath>` directly in python if you run the line of code before you import PICASO.")
 else: 
     ref_v = json.load(open(os.path.join(__refdata__,'config.json'))).get('version',2.3)
     
     if __version__ > ref_v: 
         warnings.warn(f"Your code version is {__version__} but your reference data version is {ref_v}. For some functionality you may experience Keyword errors. Please download the newest ref version or update your code: https://github.com/natashabatalha/picaso/tree/master/reference")
 
 
 if not os.path.exists(os.environ.get('PYSYN_CDBS')): 
     raise Exception("You have not downloaded the Stellar reference data. Follow the installation instructions here: https://natashabatalha.github.io/picaso/installation.html#download-and-link-pysynphot-stellar-data. If you think you have already downloaded it then you likely just need to set your environment variable. You can use `os.environ['PYSYN_CDBS']=<yourpath>` directly in python if you run the line of code before you import PICASO.")
 
+#hello peter
 
-
-def picaso(bundle,opacityclass, dimension = '1d',calculation='reflected', full_output=False, 
-    plot_opacity= False, as_dict=True):
+def picaso(bundle,opacityclass, dimension = '1d',calculation='reflected', 
+    full_output=False, plot_opacity= False, as_dict=True):
     """
     Currently top level program to run albedo code 
     Parameters 
     ----------
     bundle : dict 
         This input dict is built by loading the input = `justdoit.load_inputs()` 
     opacityclass : class
@@ -112,15 +115,14 @@
     #define delta eddington approximinations 
     delta_eddington = inputs['approx']['rt_params']['common']['delta_eddington']
 
 
     #USED in TOON (if being used)
     single_phase = inputs['approx']['rt_params']['toon']['single_phase']
     toon_coefficients = inputs['approx']['rt_params']['toon']['toon_coefficients']
-    tridiagonal = 0 
     multi_phase = inputs['approx']['rt_params']['toon']['multi_phase']
 
     #USED in SH (if being used)
     single_form = inputs['approx']['rt_params']['SH']['single_form']
     w_single_form = inputs['approx']['rt_params']['SH']['w_single_form']
     w_multi_form = inputs['approx']['rt_params']['SH']['w_multi_form']
     psingle_form = inputs['approx']['rt_params']['SH']['psingle_form']
@@ -128,14 +130,19 @@
     w_multi_rayleigh = inputs['approx']['rt_params']['SH']['w_multi_rayleigh']
     psingle_rayleigh = inputs['approx']['rt_params']['SH']['psingle_rayleigh']
     calculate_fluxes = inputs['approx']['rt_params']['SH']['calculate_fluxes']
 
 
     # save returns to output file
     output_dir = inputs['output_dir']
+
+    #save level fluxes in addition to the top of atmosphere fluxes?
+    #default is false
+    get_lvl_flux = inputs['approx'].get('get_lvl_flux',False)
+
     
 
 
     #pressure assumption
     p_reference =  inputs['approx']['p_reference']
 
     ############# DEFINE ALL GEOMETRY USED IN CALCULATION #############
@@ -162,21 +169,23 @@
     b_top = 0.
     #semi major axis
     sa = inputs['star']['semi_major']
 
     #begin atm setup
     atm = ATMSETUP(inputs)
 
+
     #Add inputs to class 
     atm.surf_reflect = inputs['surface_reflect']
     atm.hard_surface = inputs['hard_surface']#0=no hard surface, 1=hard surface
     atm.wavenumber = wno
     atm.planet.gravity = inputs['planet']['gravity']
     atm.planet.radius = inputs['planet']['radius']
     atm.planet.mass = inputs['planet']['mass']
+    atm.get_lvl_flux=get_lvl_flux
 
     if dimension == '1d':
         atm.get_profile()
     elif dimension == '3d':
         atm.get_profile_3d()
 
     #now can get these 
@@ -240,61 +249,98 @@
                                     w_single_form, w_multi_form, psingle_form, 
                                     w_single_rayleigh, w_multi_rayleigh, psingle_rayleigh,
                                     frac_a, frac_b, frac_c, constant_back, constant_forward, 
                                     stream, b_top=b_top, flx=calculate_fluxes, 
                                     single_form=single_form) 
 
                 else:
-                    #getting intensities, not fluxes (which is why second return is null)
-                    xint = get_reflected_1d(nlevel, wno,nwno,ng,nt,
+                    if get_lvl_flux: 
+                        atm.lvl_output_reflected = dict(flux_minus=0, flux_plus=0, flux_minus_mdpt=0, flux_plus_mdpt=0)
+
+                    """xint = get_reflected_1d(nlevel, wno,nwno,ng,nt,
+                                        DTAU[:,:,ig], TAU[:,:,ig], W0[:,:,ig], COSB[:,:,ig],
+                                        GCOS2[:,:,ig],ftau_cld[:,:,ig],ftau_ray[:,:,ig],
+                                        DTAU_OG[:,:,ig], TAU_OG[:,:,ig], W0_OG[:,:,ig], COSB_OG[:,:,ig],
+                                        atm.surf_reflect, ubar0,ubar1,cos_theta, F0PI,
+                                        single_phase,multi_phase,
+                                        frac_a,frac_b,frac_c,constant_back,constant_forward, toon_coefficients,
+                                        b_top=b_top)
+                                        #get_toa_intensity=1, get_lvl_flux=0)"""
+                    
+                    xint,lvl_fluxes = get_reflected_1d(nlevel, wno,nwno,ng,nt,
                                     DTAU[:,:,ig], TAU[:,:,ig], W0[:,:,ig], COSB[:,:,ig],
                                     GCOS2[:,:,ig],ftau_cld[:,:,ig],ftau_ray[:,:,ig],
                                     DTAU_OG[:,:,ig], TAU_OG[:,:,ig], W0_OG[:,:,ig], COSB_OG[:,:,ig],
                                     atm.surf_reflect, ubar0,ubar1,cos_theta, F0PI,
                                     single_phase,multi_phase,
-                                    frac_a,frac_b,frac_c,constant_back,constant_forward, toon_coefficients,
-                                    b_top=b_top)
-                                    #get_toa_intensity=1, get_lvl_flux=0)
+                                    frac_a,frac_b,frac_c,constant_back,constant_forward,
+                                    get_toa_intensity=1,get_lvl_flux=int(atm.get_lvl_flux),
+                                    toon_coefficients=toon_coefficients,b_top=b_top) 
 
                 xint_at_top += xint*gauss_wts[ig]
 
+                if get_lvl_flux: 
+                    atm.lvl_output_reflected['flux_minus']+=lvl_fluxes[0]*gauss_wts[ig]
+                    atm.lvl_output_reflected['flux_plus']+=lvl_fluxes[1]*gauss_wts[ig]
+                    atm.lvl_output_reflected['flux_minus_mdpt']+=lvl_fluxes[2]*gauss_wts[ig]
+                    atm.lvl_output_reflected['flux_plus_mdpt']+=lvl_fluxes[3]*gauss_wts[ig]
+
             #if full output is requested add in xint at top for 3d plots
             if full_output: 
                 atm.xint_at_top = xint_at_top
                 #atm.flux= flux_out
                 #atm.int_layer = intensity
 
-
+        
         if 'thermal' in calculation:
             #use toon method (and tridiagonal matrix solver) to get net cumulative fluxes 
             flux_at_top = 0 
+
+            if get_lvl_flux: 
+                atm.lvl_output_thermal = dict(flux_minus=0, flux_plus=0, flux_minus_mdpt=0, flux_plus_mdpt=0)
+
+
             for ig in range(ngauss): # correlated-k - loop (which is different from gauss-tchevychev angle)
                 
                 #remember all OG values (e.g. no delta eddington correction) go into thermal as well as 
                 #the uncorrected raman single scattering 
                 if rt_method == 'toon':
-                    flux  = get_thermal_1d(nlevel, wno,nwno,ng,nt,atm.level['temperature'],
+                    #flux  = get_thermal_1d(nlevel, wno,nwno,ng,nt,atm.level['temperature'],
+                    #                                    DTAU_OG[:,:,ig], W0_no_raman[:,:,ig], COSB_OG[:,:,ig], 
+                    #                                    atm.level['pressure'],ubar1,
+                    #                                    atm.surf_reflect, atm.hard_surface, tridiagonal)
+                    flux,lvl_fluxes  = get_thermal_1d(nlevel, wno,nwno,ng,nt,atm.level['temperature'],
                                                         DTAU_OG[:,:,ig], W0_no_raman[:,:,ig], COSB_OG[:,:,ig], 
                                                         atm.level['pressure'],ubar1,
-                                                        atm.surf_reflect, atm.hard_surface, tridiagonal)
+                                                        atm.surf_reflect, atm.hard_surface,
+                                                        #setting wno to zero since only used for climate, calctype only gets TOA flx 
+                                                        wno*0, calc_type=0)
+
+
+
                 elif rt_method == 'SH':
-                    (flux, flux_out) = get_thermal_SH(nlevel, wno, nwno, ng, nt, atm.level['temperature'],
+                    flux, flux_layers = get_thermal_SH(nlevel, wno, nwno, ng, nt, atm.level['temperature'],
                                                 DTAU[:,:,ig], TAU[:,:,ig], W0[:,:,ig], COSB[:,:,ig], 
                                                 DTAU_OG[:,:,ig], TAU_OG[:,:,ig], W0_OG[:,:,ig], 
                                                 W0_no_raman[:,:,ig], COSB_OG[:,:,ig], 
                                                 atm.level['pressure'], ubar1, 
                                                 atm.surf_reflect, stream, atm.hard_surface)
 
+                if ((rt_method == 'toon') & get_lvl_flux): 
+                    atm.lvl_output_thermal['flux_minus']+=lvl_fluxes[0]*gauss_wts[ig]
+                    atm.lvl_output_thermal['flux_plus']+=lvl_fluxes[1]*gauss_wts[ig]
+                    atm.lvl_output_thermal['flux_minus_mdpt']+=lvl_fluxes[2]*gauss_wts[ig]
+                    atm.lvl_output_thermal['flux_plus_mdpt']+=lvl_fluxes[3]*gauss_wts[ig]
 
                 flux_at_top += flux*gauss_wts[ig]
                 
+                
             #if full output is requested add in flux at top for 3d plots
             if full_output: 
                 atm.flux_at_top = flux_at_top
-                #atm.intensity = intensity
 
         
         if 'transmission' in calculation:
             rprs2 = 0 
             for ig in range(ngauss): # correlated - loop (which is different from gauss-tchevychev angle)
 
                 rprs2_g = get_transit_1d(atm.level['z'],atm.level['dz'],
@@ -329,17 +375,24 @@
         #if users want to retain all the individual opacity info they can here 
         if full_output:
             TAUGAS_3d = np.zeros((nlayer, nwno, ng, nt, ngauss))
             TAUCLD_3d = np.zeros((nlayer, nwno, ng, nt, ngauss))
             TAURAY_3d = np.zeros((nlayer, nwno, ng, nt, ngauss))  
 
         #get opacities at each facet
+        #sample MPI code 
+        #from mpi4py improt MPI
+        #comm = MPI.COMM_WORLD
+        #rank = comm.Get_rank()
+        #size = comm.Get_size()
+        #idx = rank-1 
+        #gts = [[g,t] for g in range(ng) for t in range(nt)]
         for g in range(ng):
             for t in range(nt): 
-
+                #g,t = gts[idx]
                 #edit atm class to only have subsection of 3d stuff 
                 atm_1d = copy.deepcopy(atm)
 
                 #diesct just a subsection to get the opacity 
                 atm_1d.disect(g,t)
 
                 get_opacities(atm_1d)
@@ -376,58 +429,60 @@
             atm.taugas = TAUGAS_3d
             atm.taucld = TAUCLD_3d
             atm.tauray = TAURAY_3d
 
         if  'reflected' in calculation:
             xint_at_top=0
             for ig in range(ngauss): # correlated - loop (which is different from gauss-tchevychev angle)
-                #use toon method (and tridiagonal matrix solver) to get net cumulative fluxes 
+                #use toon method  to get net cumulative fluxes 
                 xint  = get_reflected_3d(nlevel, wno,nwno,ng,nt,
                                                 DTAU_3d[:,:,:,:,ig], TAU_3d[:,:,:,:,ig], W0_3d[:,:,:,:,ig], COSB_3d[:,:,:,:,ig],GCOS2_3d[:,:,:,:,ig],
                                                 FTAU_CLD_3d[:,:,:,:,ig],FTAU_RAY_3d[:,:,:,:,ig],
                                                 DTAU_OG_3d[:,:,:,:,ig], TAU_OG_3d[:,:,:,:,ig], W0_OG_3d[:,:,:,:,ig], COSB_OG_3d[:,:,:,:,ig],
                                                 atm.surf_reflect, ubar0,ubar1,cos_theta, F0PI,
                                                 single_phase,multi_phase,
-                                                frac_a,frac_b,frac_c,constant_back,constant_forward, tridiagonal)
+                                                frac_a,frac_b,frac_c,constant_back,constant_forward)
                 xint_at_top += xint*gauss_wts[ig]
                 #if full output is requested add in xint at top for 3d plots
             if full_output: 
                 atm.xint_at_top = xint_at_top
 
         if 'thermal' in calculation:
             flux_at_top=0
             for ig in range(ngauss): # correlated - loop (which is different from gauss-tchevychev angle)
                 #remember all OG values (e.g. no delta eddington correction) go into thermal as well as 
                 #the uncorrected raman single scattering 
                 flux  = get_thermal_3d(nlevel, wno,nwno,ng,nt,TLEVEL_3d,
                                             DTAU_OG_3d[:,:,:,:,ig], W0_no_raman_3d[:,:,:,:,ig], COSB_OG_3d[:,:,:,:,ig], 
-                                            PLEVEL_3d,ubar1, atm.surf_reflect, atm.hard_surface, tridiagonal)
+                                            PLEVEL_3d,ubar1, atm.surf_reflect, atm.hard_surface)
                 flux_at_top += flux*gauss_wts[ig]
             #if full output is requested add in flux at top for 3d plots
             if full_output: 
                 atm.flux_at_top = flux_at_top
 
-
-    #COMPRESS FULL TANGLE-GANGLE FLUX OUTPUT ONTO 1D FLUX GRID
-
     #set up initial returns
     returns = {}
     returns['wavenumber'] = wno
     #returns['flux'] = flux
     if 'transmission' in calculation: 
         returns['transit_depth'] = rprs2
 
+    #COMPRESS FULL TANGLE-GANGLE FLUX OUTPUT ONTO 1D FLUX GRID
 
     #for reflected light use compress_disco routine
     #this takes the intensity as a functin of tangle/gangle and creates a 1d spectrum
     if  ('reflected' in calculation):
         albedo = compress_disco(nwno, cos_theta, xint_at_top, gweight, tweight,F0PI)
         returns['albedo'] = albedo 
-        #returns['xint_at_top'] = xint_at_top 
-        #returns['intensity'] = intensity 
+
+        if ((rt_method == 'toon') & get_lvl_flux): 
+            for i in atm.lvl_output_reflected.keys():
+                atm.lvl_output_reflected[i] = compress_disco(nwno,cos_theta,atm.lvl_output_reflected[i], gweight, tweight,F0PI)   
+
+
         #see equation 18 Batalha+2019 PICASO 
         returns['bond_albedo'] = (np.trapz(x=1/wno, y=albedo*opacityclass.unshifted_stellar_spec)/
                                     np.trapz(x=1/wno, y=opacityclass.unshifted_stellar_spec))
 
         if ((not np.isnan(sa ) and (not np.isnan(atm.planet.radius))) ):
             returns['fpfs_reflected'] = albedo*(atm.planet.radius/sa)**2.0
         else: 
@@ -438,22 +493,23 @@
                 returns['fpfs_reflected'] += ['Planet Radius not supplied. If you want fpfs, add it to `gravity` function with a mass.']
 
     #for thermal light use the compress thermal routine
     #this takes the intensity as a functin of tangle/gangle and creates a 1d spectrum
     if ('thermal' in calculation):
         thermal = compress_thermal(nwno,flux_at_top, gweight, tweight)
         returns['thermal'] = thermal
-        #returns['xint_at_top'] = flux_at_top 
-        #returns['tau'] = TAU 
         returns['thermal_unit'] = 'erg/s/(cm^2)/(cm)'#'erg/s/(cm^2)/(cm^(-1))'
         returns['effective_temperature'] = (np.trapz(x=1/wno[::-1], y=thermal[::-1])/5.67e-5)**0.25
 
         if full_output: 
             atm.thermal_flux_planet = thermal
-            
+
+        if ((rt_method == 'toon') & get_lvl_flux): 
+            for i in atm.lvl_output_thermal.keys():
+                atm.lvl_output_thermal[i] = compress_thermal(nwno,atm.lvl_output_thermal[i], gweight, tweight)   
 
         #only need to return relative flux if not a browndwarf calculation
         if radius_star == 'nostar': 
             returns['fpfs_thermal'] = ['No star mode for Brown Dwarfs was used']
         elif ((not np.isnan(atm.planet.radius)) & (not np.isnan(radius_star))) :
             fpfs_thermal = thermal/(opacityclass.unshifted_stellar_spec)*(atm.planet.radius/radius_star)**2.0
             returns['fpfs_thermal'] = fpfs_thermal
@@ -473,27 +529,27 @@
     if full_output: 
         if as_dict:
             returns['full_output'] = atm.as_dict()
             if radius_star != 'nostar':returns['full_output']['star']['flux'] = opacityclass.unshifted_stellar_spec
         else:
             returns['full_output'] = atm
 
-    if output_dir != None:
-        filename = output_dir
-        pk.dump({'pressure': atm.level['pressure'], 'temperature': atm.level['temperature'], 
-            'nlevel':nlevel, 'wno':wno, 'nwno':nwno, 'ng':ng, 'nt':nt, 
-            'dtau':DTAU, 'tau':TAU, 'w0':W0, 'cosb':COSB, 'gcos2':GCOS2,'ftcld':ftau_cld,'ftray': ftau_ray,
-            'dtau_og':DTAU_OG, 'tau_og':TAU_OG, 'w0_og':W0_OG, 'cosb_og':COSB_OG, 
-            'surf_reflect':atm.surf_reflect, 'ubar0':ubar0, 'ubar1':ubar1, 'costheta':cos_theta, 'F0PI':F0PI, 
-            'single_phase':single_phase, 'multi_phase':multi_phase, 
-            'frac_a':frac_a, 'frac_b':frac_b, 'frac_c':frac_c, 'constant_back':constant_back, 
-            'constant_forward':constant_forward, 'dim':dimension, 'stream':stream,
-            #'xint_at_top': xint_at_top, 'albedo': albedo, 'flux': flux_out, 'xint': intensity,
-            'b_top': b_top, 'gweight': gweight, 'tweight': tweight, 'gangle': gangle, 'tangle': tangle}, 
-            open(filename,'wb'), protocol=2)
+    #if output_dir != None:
+    #    filename = output_dir
+    #    pk.dump({'pressure': atm.level['pressure'], 'temperature': atm.level['temperature'], 
+    #        'nlevel':nlevel, 'wno':wno, 'nwno':nwno, 'ng':ng, 'nt':nt, 
+    #        'dtau':DTAU, 'tau':TAU, 'w0':W0, 'cosb':COSB, 'gcos2':GCOS2,'ftcld':ftau_cld,'ftray': ftau_ray,
+    #        'dtau_og':DTAU_OG, 'tau_og':TAU_OG, 'w0_og':W0_OG, 'cosb_og':COSB_OG, 
+    #        'surf_reflect':atm.surf_reflect, 'ubar0':ubar0, 'ubar1':ubar1, 'costheta':cos_theta, 'F0PI':F0PI, 
+    #        'single_phase':single_phase, 'multi_phase':multi_phase, 
+    #        'frac_a':frac_a, 'frac_b':frac_b, 'frac_c':frac_c, 'constant_back':constant_back, 
+    #        'constant_forward':constant_forward, 'dim':dimension, 'stream':stream,
+    #        #'xint_at_top': xint_at_top, 'albedo': albedo, 'flux': flux_out, 'xint': intensity,
+    #        'b_top': b_top, 'gweight': gweight, 'tweight': tweight, 'gangle': gangle, 'tangle': tangle}, 
+    #        open(filename,'wb'), protocol=2)
     return returns
 
 def _finditem(obj, key):
     if key in obj: return obj[key]
     for k, v in obj.items():
         if isinstance(v,dict):
             item = _finditem(v, key)
@@ -540,14 +596,21 @@
     xarray can be used with input_xarray to rerun models. See Preservation notebook. 
     
     Parameters
     ----------
     df : dict 
         This is the output of your spectrum and must include "full_output=True"
         For example, df = case.spectrum(opa, full_output=True)
+        It can also be the output of your climate run. For example, out=case.climate(..., withSpec=True)
+        If running climate you must run withSpec=True OR add output of case.spectrum to your output dictionary
+        by doing (for example): 
+        >> out = case.climate(..., withSpec=False)
+        >> #add any post processing steps you desire (e.g. case.atmosphere or case.clouds)
+        >> df = case.spectrum(opa, calculation='thermal')
+        >> out['spectrum_output'] = df
     picaso_class : picaso.inputs
         This is the original class that you made to do your run. 
         For example, case=jdi.inputs();followed by case.atmosphere(), case.clouds(), etc
     add_output : dict
         These are any additional outputs you want included in your xarray metadata 
         This dictionary has a very specific struture if you want it to work correctly. 
         To see the structure you can run justdoit.standard_metadata() which will 
@@ -555,69 +618,126 @@
     savefile : str 
         Optional, if string it will save a xarray file for you 
     
     Returns
     -------
     xarray.Dataset
         this xarray dataset can be easily passed to justdoit.input_xarray to run a spectrum 
+    
+    Todo
+    ----
+    - figure out why pandas index are being returned for pressure and wavelenth 
+    - fix clouds wavenumber_layer which doesnt seem like it would work 
+    - add clima inputs : teff (or tint), number of convective zones
+    - cvs_locs array should be more clear
+    """ 
+    attrs = {}
+    if not isinstance(_finditem(df, 'full_output'), type(None)): 
+        #print("Found full_output!")
+        full_output = _finditem(df, 'full_output')
+        molecules_included = full_output['weights']
+    else: 
+        raise Exception("full_output is required. Either you need to run spectrum(opa, full_output=True), climate(..., with_Spec=True), or create and add info to spectrum_output")
+
+    if not isinstance(_finditem(df, 'wavenumber'), type(None)):
+        wavenumber = _finditem(df, 'wavenumber')
+    else: 
+        raise Exception("wavenumber is required to be in df somewhere")
         
-    """
         
-    full_output = df['full_output'] if 'full_output' in df.keys() else  df['spectrum_output']['full_output']
-    df_atmo = picaso_class.inputs['atmosphere']['profile']
-    molecules_included = full_output['weights']
+    #if they put in climate data, add it to xarray and create meta data
+    if not isinstance(_finditem(df, 'dtdp'), type(None)): 
+        attrs['climate_params'] = {}
     
+    #is df_atmo ran with climate calculations or hi-res spectrum
+    if not isinstance(_finditem(df, 'ptchem_df'), type(None)):
+        df_atmo = _finditem(df,'ptchem_df')
+    else:
+        df_atmo = picaso_class.inputs['atmosphere']['profile']
+
     #start with simple layer T
     data_vars=dict(temperature = (["pressure"], 
                                   df_atmo['temperature'],
                                   {'units': 'Kelvin'}))
-    
+
+    #add climate data
+    if not isinstance(_finditem(df, 'dtdp'), type(None)): 
+        dtdp = _finditem(df,'dtdp')
+        data_vars['dtdp'] = (["pressure_layer"], dtdp, {'units': 'K/bar'})
+   
+    if not isinstance(_finditem(df, 'cvz_locs'), type(None)): #for metadata (converged) and other(all_profiles/nlevel)
+        cvz_locs = _finditem(df, 'cvz_locs')
+        attrs['climate_params']['cvs_locs'] = cvz_locs
+        
+    if not isinstance(_finditem(df, 'converged'), type(None)):
+        converged = _finditem(df,'converged')
+        attrs['climate_params']['converged'] = converged
+        
+    if not isinstance(_finditem(df , 'all_profiles'), type(None)):
+        all_profiles = _finditem(df , 'all_profiles')
+        nlevel = len(df_atmo['pressure'])
+        for i in range((int(len(all_profiles)/nlevel))): 
+            #after each nlevel amount (ex: 91), restart guess count
+            index_start=nlevel*i
+            index_finish=nlevel*(i+1)
+            data_vars['guess '+str(i+1)]= (["pressure"], all_profiles[index_start:index_finish],{'units': 'Kelvin'})
+            
     #spectral data 
-    if 'thermal' in df.keys(): 
-        data_vars['flux_emission'] = (["wavelength"], df['thermal'],{'units': 'erg/cm**2/s/cm'}) 
-    if 'transit_depth' in df.keys(): 
-        data_vars['transit_depth'] = (["wavelength"], df['transit_depth'],{'units': 'R_jup**2/R_jup**2'}) 
-    if 'temp_brightness' in df.keys(): 
-        data_vars['temp_brightness'] = (["wavelength"], df['temp_brightness'],{'units': 'Kelvin'})
-    if 'fpfs_thermal' in df.keys(): 
-        if isinstance(df['fpfs_thermal'], np.ndarray): 
-            data_vars['fpfs_emission'] = (["wavelength"], df['fpfs_thermal'],{'units': 'erg/cm**2/s/cm/(erg/cm**2/s/cm)'})
-    if 'albedo' in df.keys(): 
-        data_vars['albedo'] = (["wavelength"], df['albedo'],{'units': 'none'})
-    if 'fpfs_reflected' in df.keys(): 
-        if isinstance(df['fpfs_reflected'], np.ndarray): 
-            data_vars['fpfs_reflected'] = (["wavelength"], df['fpfs_reflected'],{'units': 'erg/cm**2/s/cm/(erg/cm**2/s/cm)'})
-    
+    if not isinstance(_finditem(df, 'thermal'), type(None)):
+        thermal = _finditem(df,'thermal')
+        data_vars['flux_emission'] = (["wavelength"], thermal,{'units': 'erg/cm**2/s/cm'}) 
+    if not isinstance(_finditem(df, 'transit_depth'), type(None)):
+        transit_depth = _finditem(df, 'transit_depth')
+        data_vars['transit_depth'] = (["wavelength"], transit_depth,{'units': 'R_jup**2/R_jup**2'}) 
+    if not isinstance(_finditem(df, 'temp_brightness'), type(None)): 
+        temp_brightness = _finditem(df, 'temp_brightness')
+        data_vars['temp_brightness'] = (["wavelength"], temp_brightness,{'units': 'Kelvin'})
+    if not isinstance(_finditem(df, 'fpfs_thermal'), type(None)):
+        fpfs_thermal= _finditem(df, 'fpfs_thermal')
+        if isinstance(fpfs_thermal, np.ndarray):
+            data_vars['fpfs_emission'] = (["wavelength"], fpfs_thermal,{'units': 'erg/cm**2/s/cm/(erg/cm**2/s/cm)'})
+    if not isinstance(_finditem(df, 'albedo'), type(None)): 
+        albedo=_finditem(df, 'albedo')
+        data_vars['albedo'] = (["wavelength"], albedo,{'units': 'none'})
+    if not isinstance(_finditem(df, 'fpfs_reflected'), type(None)): 
+        fpfs_reflected=_finditem(df, 'fpfs_reflected')
+        if isinstance(fpfs_reflected, np.ndarray): 
+            data_vars['fpfs_reflected'] = (["wavelength"], fpfs_reflected,{'units': 'erg/cm**2/s/cm/(erg/cm**2/s/cm)'})
+
+
     #atmospheric data data 
     for ikey in molecules_included:
         data_vars[ikey] = (["pressure"], df_atmo[ikey].values,{'units': 'v/v'})
         
-    if 'kz' in picaso_class.inputs['atmosphere']['profile'].keys(): 
-        data_vars['kzz'] = (["pressure"], picaso_class.inputs['atmosphere']['profile']['kz'].values,{'units': 'cm**2/s'})
+    if 'kz' in df_atmo: 
+        data_vars['kzz'] = (["pressure"], df_atmo['kz'].values,{'units': 'cm**2/s'})
       
     #clouds if they exist 
     if 'clouds' in picaso_class.inputs: 
         if not isinstance(picaso_class.inputs['clouds']['profile'],type(None)):
             for ikey,lbl in zip( ['opd', 'w0', 'g0'], ['opd','ssa','asy']):
                 array = np.reshape(picaso_class.inputs['clouds']['profile'][ikey].values, 
                        (picaso_class.nlevel-1, 
                         len(picaso_class.inputs['clouds']['wavenumber'])))
 
-                data_vars[lbl]=(['pressure_cld','wavenumber_cld'],array,{'units': 'unitless'})
+                data_vars[lbl]=(['pressure_layer','wavenumber_layer'],array,{'units': 'unitless'})
     
-    attrs = {}
     #basic info
     for ikey in ['author','code','doi','contact']:
         if add_output.get(ikey,'optional') != 'optional':
             attrs[ikey] = add_output[ikey]
             
     #planet params 
     planet_params = add_output.get('planet_params',{})
     attrs['planet_params'] = {}
     
+    if not isinstance(_finditem(df, 'effective_temperature'), type(None)):
+        effective_temp = _finditem(df, 'effective_temperature')
+        attrs['planet_params']['effective_temp'] = effective_temp
+
     #find gravity in picaso
     gravity = picaso_class.inputs['planet'].get('gravity',np.nan)
     if np.isfinite(gravity): 
         gravity = gravity * check_units(picaso_class.inputs['planet']['gravity_unit'])
     #otherwise find gravity from user input
     else: 
         gravity = planet_params.get('logg', np.nan) 
@@ -631,15 +751,15 @@
     rp = picaso_class.inputs['planet'].get('radius',np.nan)
     if np.isfinite(mp):
         rp = rp * check_units(picaso_class.inputs['planet']['radius_unit'])
     else: 
         rp = planet_params.get('rp',np.nan) 
         
     #add required RP/MP or gravity
-    if (not np.isnan(mp) & (not np.isnan(rp))):
+    if (((not np.isnan(mp)) & (not np.isnan(rp))) & (((not isinstance(mp,str)) & (not isinstance(rp,str))))):
         attrs['planet_params']['mp'] = mp
         attrs['planet_params']['rp'] = rp
         assert isinstance(attrs['planet_params']['mp'],u.quantity.Quantity ), "User supplied mp in planet_params must be an astropy unit: e.g. 1*u.Unit('M_jup')"
         assert isinstance(attrs['planet_params']['rp'],u.quantity.Quantity ), "User supplied rp in planet_params must be an astropy unit: e.g. 1*u.Unit('R_jup')"
     elif (not np.isnan(gravity)): 
         attrs['planet_params']['gravity'] = gravity
         assert isinstance(attrs['planet_params']['gravity'],u.quantity.Quantity ), "User supplied gravity in planet_params must be an astropy unit: e.g. 1*u.Unit('m/s**2')"
@@ -708,40 +828,45 @@
                 if ikey not in ['sma']:
                     if orbit_params[ikey]!='optional':attrs['orbit_params'][ikey] = orbit_params[ikey] 
                     
             attrs['orbit_params'] = json.dumps(attrs['orbit_params'],cls=JsonCustomEncoder)
             
 
                
-        attrs['stellar_params'] = json.dumps(attrs['stellar_params'],cls=JsonCustomEncoder)
+        if 'stellar_params' in attrs.keys(): attrs['stellar_params'] = json.dumps(attrs['stellar_params'],cls=JsonCustomEncoder)
+        if 'climate_params' in attrs.keys(): attrs['climate_params'] = json.dumps(attrs['climate_params'],cls=JsonCustomEncoder)
         
         
     #add anything else requested by the user
     for ikey in add_output.keys(): 
         if ikey not in attrs.keys(): 
             if add_output[ikey]!="optional":attrs[ikey] = add_output[ikey]
     
     
     coords=dict(
-            pressure=(["pressure"], picaso_class.inputs['atmosphere']['profile']['pressure'].values,{'units': 'bar'}),#required*
-            wavelength=(["wavelength"], 1e4/df['wavenumber'],{'units': 'micron'})
+            pressure=(["pressure"], np.array(df_atmo['pressure'].values),{'units': 'bar'}),#required*
+            wavelength=(["wavelength"], np.array(1e4/wavenumber),{'units': 'micron'})
         )
     if 'clouds' in 'opd' in data_vars.keys(): 
-        coords['wavenumber_cld'] = (["wavenumber_cld"], picaso_class.inputs['clouds']['wavenumber'],{'units': 'cm**(-1)'})
-        coords['pressure_cld'] = (["pressure_cld"], full_output['layer']['pressure'] ,{'units': full_output['layer']['pressure_unit']})
-        
+        coords['wavenumber_layer'] = (["wavenumber_layer"], picaso_class.inputs['clouds']   ,{'units': 'cm**(-1)'})
+        coords['pressure_layer'] = (["pressure_layer"], full_output['layer']['pressure'] ,{'units': full_output['layer']['pressure_unit']})
+    if 'dtdp' in data_vars.keys():
+        coords['pressure_layer'] = (["pressure_layer"], full_output['layer']['pressure'] ,{'units': full_output['layer']['pressure_unit']})
+
     # put data into a dataset where each
     ds = xr.Dataset(
         data_vars=data_vars,
         coords=coords,
         attrs=attrs
     )
     
     if isinstance(savefile, str): ds.to_netcdf(savefile)
+
     return ds
+
 def input_xarray(xr_usr, opacity,p_reference=10, calculation='planet'):
     """
     This takes an input based on these standards and runs: 
     -gravity
     -phase_angle
     -star
     -approx (p_reference=10)
@@ -876,15 +1001,14 @@
     stream = inputs['approx']['rt_params']['common']['stream']
     
     #only used in toon
     multi_phase = inputs['approx']['rt_params']['toon']['multi_phase']
     single_phase = inputs['approx']['rt_params']['toon']['single_phase']
     #define delta eddington approximinations 
     delta_eddington = inputs['approx']['rt_params']['common']['delta_eddington']    
-    tridiagonal = 0 
     raman_approx = 2
 
     #parameters needed for the two term hg phase function. 
     #Defaults are set in config.json
     f = inputs['approx']['rt_params']['common']['TTHG_params']['fraction']
     frac_a = f[0]
     frac_b = f[1]
@@ -1371,168 +1495,15 @@
         self.inputs['climate']['p_table'] = np.array(cp_grad['pressure'])
         #\nabla_ad = d ln T/ d ln P |_S (at constant entropy)
         self.inputs['climate']['grad'] = np.array(cp_grad['adiabat_grad'])
         #log Cp (erg/g/K);Specific heat at constant pressure for the same H/He 
         self.inputs['climate']['cp'] = np.array(cp_grad['specific_heat'])
 
 
-    def inputs_climate(self, temp_guess= None, pressure= None, nstr = None, nofczns = None , rfacv = None, rfaci = None, cloudy = False, mh = None, CtoO = None, species = None, fsed = None):
-        """
-        Get Inputs for Climate run
-
-        Parameters
-        ----------
-        temp_guess : array 
-            Guess T(P) profile to begin with
-        pressure : array
-            Pressure Grid for climate code (this wont change on the fly)
-        nstr : array
-            NSTR vector describes state of the atmosphere:
-            0   is top layer [0]
-            1   is top layer of top convective region
-            2   is bottom layer of top convective region
-            3   is top layer of lower radiative region
-            4   is top layer of lower convective region
-            5   is bottom layer of lower convective region [nlayer-1]
-        rfacv : float
-            Fractional contribution of reflected light in net flux
-        rfaci : float
-            Fractional contribution of thermal light in net flux
-
-        
-        """
-
-        if self.inputs['planet']['T_eff'] == 0.0:
-            raise Exception('Need to specify Teff with jdi.input for climate run')
-        if self.inputs['planet']['gravity'] == 0.0:
-            raise Exception('Need to specify gravity with jdi.input for climate run')
-
-        
-        self.inputs['climate']['guess_temp'] = temp_guess
-        self.inputs['climate']['pressure'] = pressure
-        self.inputs['climate']['nstr'] = nstr
-        self.inputs['climate']['nofczns'] = nofczns
-        self.inputs['climate']['rfacv'] = rfacv
-        self.inputs['climate']['rfaci'] = rfaci
-        if cloudy:
-            self.inputs['climate']['cloudy'] = 1
-            self.inputs['climate']['cld_species'] = species
-            self.inputs['climate']['fsed'] = fsed
-        else :
-            self.inputs['climate']['cloudy'] = 0
-            self.inputs['climate']['cld_species'] = 0
-            self.inputs['climate']['fsed'] = 0
-        self.inputs['climate']['mh'] = mh
-        self.inputs['climate']['CtoO'] = CtoO
-
-    def old_run_climate_model(self, opacityclass):
-        """
-        Top Function to run the Climate Model
-
-        Parameters
-        -----------
-        
-        """
-        #get necessary parameters from opacity ck-tables 
-        wno = opacityclass.wno
-        delta_wno = opacityclass.delta_wno
-        nwno = opacityclass.nwno
-        min_temp = min(opacityclass.temps)
-        max_temp = max(opacityclass.temps)
-
-        
-        
-        # first calculate the BB grid
-        ntmps = self.inputs['climate']['ntemp_bb_grid']
-        dt = self.inputs['climate']['dt_bb_grid']
-        #we will extend the black body grid 30% beyond the min and max temp of the 
-        #opacity grid just to be safe with the spline
-        extension = 0.3 
-        tmin = min_temp*(1-extension)
-        tmax = max_temp*(1+extension)
-
-        bb , y2 , tp = set_bb(wno,delta_wno,nwno,ntmps,dt,tmin,tmax)
-
-        nofczns = self.inputs['climate']['nofczns']
-        nstr= self.inputs['climate']['nstr']
-
-        rfaci= self.inputs['climate']['rfaci']
-        
-        #turn off stellar radiation if user has run "setup_nostar() function"
-        if 'nostar' in self.inputs['star'].values():
-            rfacv=0.0 
-            F0PI = np.zeros(nwno) #+ 1.0
-        #otherwise assume that there is stellar irradiation 
-        else:
-            rfacv = self.inputs['climate']['rfacv']
-            r_star = self.inputs['star']['radius'] 
-            r_star_unit = self.inputs['star']['radius_unit'] 
-            semi_major = self.inputs['star']['semi_major']
-            semi_major_unit = self.inputs['star']['semi_major_unit'] 
-            
-
-            fine_flux_star  = self.inputs['star']['flux']  # erg/s/cm^2
-            F0PI = fine_flux_star * ((r_star/semi_major)**2)
-
-
-        TEMP1 = self.inputs['climate']['guess_temp']
-        pressure = self.inputs['climate']['pressure']
-        t_table = self.inputs['climate']['t_table']
-        p_table = self.inputs['climate']['p_table']
-        grad = self.inputs['climate']['grad']
-        cp = self.inputs['climate']['cp']
-
-
-        Teff = self.inputs['planet']['T_eff']
-        grav = 0.01*self.inputs['planet']['gravity'] # cgs to si
-        mh = float(self.inputs['climate']['mh'])
-        sigma_sb = 0.56687e-4 # stefan-boltzmann constant
-        
-        col_den = 1e6*(pressure[1:] -pressure[:-1] ) / (grav/0.01) # cgs g/cm^2
-        wave_in, nlevel, pm, hratio = 0.9, len(pressure), 0.001, 0.1
-        #tidal = tidal_flux(Teff, wave_in,nlevel, pressure, pm, hratio, col_den)
-        tidal = np.zeros_like(pressure) - sigma_sb *(Teff**4)
-        
-        cloudy = self.inputs['climate']['cloudy']
-        cld_species = self.inputs['climate']['cld_species']
-        fsed = self.inputs['climate']['fsed']
-        # first conv call
-        it_max= 10
-        itmx= 7
-        conv = 10.0
-        convt=5.0
-        x_max_mult=7.0
-        
-        #print('NEB FIRST PROFILE RUN')
-        final = False
-        pressure, temperature, dtdp, profile_flag = profile(it_max, itmx, conv, convt, nofczns,nstr,x_max_mult,
-            TEMP1,pressure, F0PI, t_table, p_table, grad, cp, opacityclass, grav, 
-            rfaci, rfacv, nlevel, tidal, tmin, tmax, delta_wno, bb , y2 , tp, final , cloudy, cld_species,mh,fsed )
-
-        # second convergence call
-        it_max= 7
-        itmx= 5
-        conv = 5.0
-        convt=4.0
-        x_max_mult=7.0
-
-
-        #print('NEB SECOND PROFILE RUN')
-        final = False
-        pressure, temperature, dtdp, profile_flag = profile(it_max, itmx, conv, convt, nofczns,nstr,x_max_mult,
-                    temperature,pressure, F0PI, t_table, p_table, grad, cp, opacityclass, grav, 
-                    rfaci, rfacv, nlevel, tidal, tmin, tmax, delta_wno, bb , y2 , tp, final, cloudy, cld_species, mh,fsed )   
-        
-        pressure, temp, dtdp, nstr_new, flux_plus_final =find_strat(pressure, temperature, dtdp ,F0PI, nofczns,nstr,x_max_mult,
-                             t_table, p_table, grad, cp, opacityclass, grav, 
-                             rfaci, rfacv, nlevel, tidal, tmin, tmax, delta_wno, bb , y2 , tp , cloudy, cld_species, mh,fsed)
-
-        
-        return pressure , temp, dtdp, nstr_new, flux_plus_final
-   
+    
 
     def setup_nostar(self):
         """
         Turns off planet specific things, so program can run as usual
         """
         self.inputs['approx']['rt_params']['common']['raman'] = 2 #turning off raman scattering
         self.inputs['star']['database'] = 'nostar'
@@ -1689,17 +1660,21 @@
                 
                 for k in range(1,len(wno_star)):
         
                     if  (wno_star[k] > wno_planet[j]) and (wno_star[k] < wno_planet[j+1]):
                         fl+= 0.5*(flux_star[k-1] +flux_star[k])*abs((1.0/wno_star[k])-(1.0/wno_star[k-1]))
                 fine_flux_star[j] = fl
 
-            #where_are_NaNs = np.isnan(fine_flux_star)
-            
-            #fine_flux_star[where_are_NaNs] = 0   
+            #fix issue if there are zeros in certain bins 
+            mask = np.logical_or(np.isnan(fine_flux_star), fine_flux_star == 0)
+            if len(fine_wno_star[mask])>20:
+                print(f"Having to replace {len(fine_wno_star[mask])} zeros or nans in stellar spectra with interpolated values. It is advised you check this is correct and something has not gone wrong by plotting classname.inputs['star']['wno'] vs classname.inputs'star'['flux']")
+                non_zero_indices = np.where(~mask)
+                zero_nans = np.interp(fine_wno_star[mask], fine_wno_star[non_zero_indices], fine_flux_star[non_zero_indices])
+                fine_flux_star[mask] = zero_nans  
             
             opannection.unshifted_stellar_spec = fine_flux_star  
             bin_flux_star = fine_flux_star          
         else :
             flux_star_interp = np.interp(wno_planet, wno_star, flux_star)
             _x,bin_flux_star = mean_regrid(wno_star, flux_star,newx=wno_planet)
             #where the star wasn't high enough resolution  
@@ -1711,17 +1686,21 @@
         self.inputs['star']['database'] = database
         self.inputs['star']['temp'] = temp
         self.inputs['star']['logg'] = logg
         self.inputs['star']['metal'] = metal
         self.inputs['star']['radius'] = r 
         self.inputs['star']['radius_unit'] = radius_unit 
         self.inputs['star']['flux'] = bin_flux_star
+        self.inputs['star']['flux_unit'] = 'ergs cm^{-2} s^{-1} cm^{-1}'
         self.inputs['star']['wno'] = wno_planet
         self.inputs['star']['semi_major'] = semi_major 
-        self.inputs['star']['semi_major_unit'] = semi_major_unit         
+        self.inputs['star']['semi_major_unit'] = semi_major_unit    
+        self.inputs['star']['filename'] = filename
+        self.inputs['star']['w_unit'] = w_unit
+        self.inputs['star']['f_unit'] = f_unit     
 
         """
         return not needed anymore
         if deq == True :
             FOPI = fine_flux_star * ((r/semi_major)**2)
             return FOPI
         """
@@ -1943,106 +1922,23 @@
             self.inputs['atmosphere']['profile']['H2'][0:quench_levels[2]+1] -= (dq_nh3 + dq_n2)
             self.inputs['atmosphere']['profile']['H2'][0:quench_levels[3]+1] -= (dq_hcn)
             
         #self.inputs['atmosphere']['profile'][species] = pd.DataFrame(abunds)
         
         return qvmrs, qvmrs2
     
-    def run_vulcan(self,pressure,temp,kz,grav,mmw,T_star=None, logg=None,metal=None,r_star=None,semi_major=None,r_planet=None, first = False,photochem = False):
-        
-        #if T_star == None & photochem == True :
-        #    raise Exception("Cannot do photochem without star Temperature")
-        k_b = 1.38e-23 # boltzmann constant
-        m_p = 1.66e-27 # proton mass
-        
-        if len(mmw) < len(temp):
-            mmw = np.append(mmw,mmw[-1])
-        con  = k_b/(mmw*m_p)
-
-        scale_H = con * temp*1e2/(grav)
-
-        t_mix = scale_H**2/kz ## level mixing timescales
-
-        if photochem == True:
-            #T_star = self.inputs['climate']['T_star']
-            #logg = self.inputs['climate']['logg']
-            #metal = self.inputs['climate']['metal']
-            #r_star = self.inputs['climate']['r_star']
-            #semi_major = self.inputs['climate']['semi_major']
-            #r_planet = self.inputs['climate']['r_planet']
-            path = "/Users/sagnickmukherjee/Documents/GitHub/Disequilibrium-Picaso/picaso/vulcan_whole/atm/stellar_flux/starfile.txt"
-            if os.path.exists(path) == False:
-                raise Exception("Starfile does not exist. Creat a Starfile first for photochem run. Use the script read_muscles_spectra_in_nm.py to produce the right file.") 
-            
-            print("I hope you have updated the starfile with the right UV fluxes for your planet.")
-            
-            '''
-            sp = psyn.Icat("phoenix", T_star, metal,logg )
-            sp.convert("um")
-            sp.convert('flam')  # ergs/s/cm^2/ang
-            wave_nm = sp.wave*1e3
-            wave_escmnm = sp.flux*10 #ergs/s/cm^2/nm
-            header =' WL(nm)     Flux(ergs/cm**2/s/nm)'
-            wh = np.where(wave_nm < 5500)
-            np.savetxt("/Users/sagnickmukherjee/Documents/GitHub/Disequilibrium-Picaso/picaso/vulcan_whole/atm/stellar_flux/starfile.txt",np.transpose([wave_nm[wh] ,wave_escmnm[wh]]),header= header)
-            '''
-            # extending the pressure grid for vulcan to run better
-            
-            nlevel_vulc = 150
-            dummy_pressure_grid = np.logspace(np.log10(np.min(pressure)),np.log10(np.max(pressure)),nlevel_vulc)
-            temp_interp =  np.interp(dummy_pressure_grid,pressure,temp)
-            kz_interp = np.interp(dummy_pressure_grid,pressure,kz)
-            ch4_,co_,co2_,h2o_,hcn_,nh3_,h_ = run_vulcan_chem(dummy_pressure_grid,temp_interp,kz_interp,grav,first = first,photochem=True, r_star=r_star,semi_major=semi_major,r_planet = r_planet)
-            ch4 = np.interp(pressure,dummy_pressure_grid,ch4_)
-            co = np.interp(pressure,dummy_pressure_grid,co_)
-            co2 = np.interp(pressure,dummy_pressure_grid,co2_)
-            h2o = np.interp(pressure,dummy_pressure_grid,h2o_)
-            hcn = np.interp(pressure,dummy_pressure_grid,hcn_)
-            nh3 = np.interp(pressure,dummy_pressure_grid,nh3_)
-            h = np.interp(pressure,dummy_pressure_grid,h_)
-            
 
-            #ch4,co,co2,h2o,hcn,nh3,h = run_vulcan_chem(pressure,temp,kz,grav,first = first,photochem=True, r_star=r_star,semi_major=semi_major,r_planet = r_planet)
-        else :   
-            '''
-            nlevel_vulc = 150
-            dummy_pressure_grid = np.logspace(np.log10(np.min(pressure)),np.log10(np.max(pressure)),nlevel_vulc)
-            temp_interp =  np.interp(dummy_pressure_grid,pressure,temp)
-            kz_interp = np.interp(dummy_pressure_grid,pressure,kz)
-            ch4_,co_,co2_,h2o_,hcn_,nh3_,h_ = run_vulcan_chem(dummy_pressure_grid,temp_interp,kz_interp,grav,first = first)
-            ch4 = np.interp(pressure,dummy_pressure_grid,ch4_)
-            co = np.interp(pressure,dummy_pressure_grid,co_)
-            co2 = np.interp(pressure,dummy_pressure_grid,co2_)
-            h2o = np.interp(pressure,dummy_pressure_grid,h2o_)
-            hcn = np.interp(pressure,dummy_pressure_grid,hcn_)
-            nh3 = np.interp(pressure,dummy_pressure_grid,nh3_)
-            h = np.interp(pressure,dummy_pressure_grid,h_)
-            '''
-            ch4,co,co2,h2o,hcn,nh3,h = run_vulcan_chem(pressure,temp,kz,grav,first = first)
-
-        
-        self.inputs['atmosphere']['profile']['H2O'] = h2o
-        self.inputs['atmosphere']['profile']['CO'] = co
-        self.inputs['atmosphere']['profile']['CH4'] = ch4
-        self.inputs['atmosphere']['profile']['CO2'] = co2
-        self.inputs['atmosphere']['profile']['NH3'] = nh3
-        self.inputs['atmosphere']['profile']['HCN'] = hcn
-        self.inputs['atmosphere']['profile']['H'] = h
-
-
-
-        return t_mix
     
     def sonora(self, sonora_path, teff, chem='low'):
         """
         This queries Sonora temperature profile that can be downloaded from profiles.tar on 
-        Zenodo: [profile.tar file](https://zenodo.org/record/1309035#.Xo5GbZNKjGJ)
-        
-        Alterntiavely you can grab the sonora bobcat models here: 
-        https://zenodo.org/record/5063476/files/structures_m%2B0.0.tar.gz?download=1
+        Zenodo: 
+
+            - Bobcat Models: [profile.tar file](https://zenodo.org/record/1309035#.Xo5GbZNKjGJ)
+            - Elf OWL Models: [L Type Models](https://zenodo.org/records/10385987), [T Type Models](https://zenodo.org/records/10385821), [Y Type Models](https://zenodo.org/records/10381250)
 
         Note gravity is not an input because it grabs gravity from self. 
 
         Parameters
         ----------
         sonora_path : str   
             Path to the untarred profile.tar file from sonora grid 
@@ -2074,15 +1970,15 @@
             coordinate = [teff, g]
 
             get_ind = min(pairs, key=lambda c: math.hypot(c[1]- coordinate[0], c[2]-coordinate[1]))[0]
 
             build_filename = 't'+ts[get_ind]+'g'+gs[get_ind]+'nc_m0.0.cmp.gz'
             if build_filename not in flist: 
                 raise Exception(f"The Sonora file you are looking for {build_filename} does not exist in your specified directory {sonora_path}. Please check that it is in there.")
-            ptchem = pd.read_csv(os.path.join(sonora_path,build_filename),delim_whitespace=True,compression='gzip')
+            ptchem = pd.read_csv(os.path.join(sonora_path,build_filename),sep='\s+',compression='gzip')
             ptchem = ptchem.rename(columns={'P(BARS)':'pressure',
                                             'TEMP':'temperature',
                                             'HE':'He'})
             self.nlevel = ptchem.shape[0]
 
             self.inputs['atmosphere']['profile'] = ptchem.loc[:,['pressure','temperature']]
         elif ('.dat' in str(flist)):
@@ -2157,15 +2053,15 @@
         #sort pressure
         self.inputs['atmosphere']['profile'] = df
         self.nlevel = df.shape[0]
         
         #player = df['pressure'].values
         #tlayer  = df['temperature'].values
         
-        grid = pd.read_csv(filename,delim_whitespace=True)
+        grid = pd.read_csv(filename,sep='\s+')
         grid['pressure'] = 10**grid['pressure']
 
         self.chem_interp(grid)
 
     def chemeq_visscher(self, c_o, log_mh):#, interp_window = 11, interp_poly=2):
         """
         Author of Data: Channon Visscher
@@ -2220,15 +2116,15 @@
         str_fe = str(grid_feh).replace('.','').replace('-','m')
 
         filename = os.path.join(__refdata__,'chemistry','visscher_grid',
             f'2015_06_1060grid_feh_{str_fe}_co_{str_co}.txt').replace('_m0','m0')
 
         header = pd.read_csv(filename).keys()[0]
         cols = header.replace('T (K)','temperature').replace('P (bar)','pressure').split()
-        a = pd.read_csv(filename,delim_whitespace=True,skiprows=1,header=None, names=cols)
+        a = pd.read_csv(filename,sep='\s+',skiprows=1,header=None, names=cols)
         a['pressure']=10**a['pressure']
 
 
         self.chem_interp(a)
 
     def channon_grid_low(self, filename = None):
         """
@@ -3101,16 +2997,16 @@
                 df.loc[((df['pressure'] >= minp) & (df['pressure'] <= maxp)),'w0']= iw
                 df.loc[((df['pressure'] >= minp) & (df['pressure'] <= maxp)),'opd']= io
 
             self.inputs['clouds']['profile'] = df  
     
     def virga(self, condensates, directory,
         fsed=1, b=1, eps=1e-2, param='const', 
-        mh=1, mmw=2.2, kz_min=1e5, sig=2, 
-        full_output=False, Teff=None, alpha_pressure=None, supsat=0,
+        mh=1, mmw=2.2, kz_min=1e5, sig=2,
+        Teff=None, alpha_pressure=None, supsat=0,
         gas_mmr=None, do_virtual=False, verbose=True): 
         """
         Runs virga cloud code based on the PT and Kzz profiles 
         that have been added to inptus class.
         Parameters
         ----------
         condensates : str 
@@ -3123,26 +3019,27 @@
             Minimum value of fsed function (if param=exp)
         param : str
             fsed parameterisation
             'const' (constant), 'exp' (exponential density derivation), 'pow' (power-law)
         mh : float 
             Metallicity 
         mmw : float 
-            Atmospheric mean molecular weight  
+            Atmospheric mean molecular weight 
+        gas_mmr : dict 
+            Gas MMR as a dictionary for individual gases. This allows users to override 
+            virga's chemistry. E.g. {'SiO2':1e-6}
         kz_min : float
             Minimum kzz value
         sig : float 
             Width of the log normal distribution for the particle sizes 
         Teff : float, optional
             Effective temperature. If None, Teff set to temperature at 1 bar
         alpha_pressure: float, optional
             Pressure at which we want fsed=alpha for variable fsed calculation.
             If None, pressure set to the top of the atmosphere
-        gas_mmr : float, optional
-            Temporary option to set gas_mmr of single condensate (this needs updated)
         do_virtual : bool 
             Turn on and off the "virtual" cloud which is a cloud that forms below 
             the pressure grid defined by the user. 
         verbose : bool 
             Turn off warnings 
         """
         
@@ -3157,29 +3054,29 @@
                 `case.inputs['atmosphere']['profile']['kz'] = KZ`")
         df = self.inputs['atmosphere']['profile'].loc[:,['pressure','temperature','kz']]
         
         cloud_p.gravity(gravity=self.inputs['planet']['gravity'],
                  gravity_unit=u.Unit(self.inputs['planet']['gravity_unit']))#
         
         cloud_p.ptk(df =df, kz_min = kz_min, Teff = Teff, alpha_pressure = alpha_pressure)
-        out = vj.compute(cloud_p, as_dict=full_output,
+        out = vj.compute(cloud_p, as_dict=True,
                           directory=directory, do_virtual=do_virtual)
-        if not full_output:
-            opd, w0, g0 = out
-            df = vj.picaso_format(opd, w0, g0)
-        else: 
-            opd, w0, g0 = out['opd_per_layer'],out['single_scattering'],out['asymmetry']
-            df = vj.picaso_format(opd, w0, g0)
+
+
+        opd, w0, g0 = out['opd_per_layer'],out['single_scattering'],out['asymmetry']
+        pres = out['pressure']
+        wno = 1e4/out['wave']
+        df = vj.picaso_format(opd, w0, g0, pressure = pres, wavenumber=wno)
         #only pass through clouds 1d if clouds are one dimension 
         self.clouds(df=df)
-        if full_output : return out
+        return out
     
     def virga_3d(self, condensates, directory,
-        fsed=1, mh=1, mmw=2.2,kz_min=1e5,sig=2, full_output=False,
-        n_cpu=1,verbose=True,smooth_kz=False):
+        fsed=1, mh=1, mmw=2.2,kz_min=1e5,sig=2,
+        n_cpu=1,verbose=True,smooth_kz=False,full_output=False):
         """
         Runs virga cloud code based on the PT and Kzz profiles 
         that have been added to inptus class.
 
         Parameters
         ----------
         condensates : str 
@@ -3193,14 +3090,16 @@
         n_cpu : int 
             number cpu to parallelize
         verbose : bool 
             Print statements to help user
         smooth_kz : bool 
             If true, it uses the min_kz value and does a UnivariateSpline
             accross the kz values to smooth out the profile
+        full_output : bool  
+            Returns full output of virga model run
         """
         lat =self.inputs['atmosphere']['profile'].coords['lat'].values
         lon = self.inputs['atmosphere']['profile'].coords['lon'].values
         nt = len(lat)
         ng = len(lon)
         self.nlevel = len(self.inputs['atmosphere']['profile'].coords['pressure'].values)
         nlayer = self.nlevel-1
@@ -3405,15 +3304,16 @@
         self.inputs['clouds']['wavenumber'] = ds.coords['wno'].values
     
     def approx(self,single_phase='TTHG_ray',multi_phase='N=2',delta_eddington=True,
         raman='pollack',tthg_frac=[1,-1,2], tthg_back=-0.5, tthg_forward=1,
         p_reference=1, rt_method='toon', stream=2, toon_coefficients="quadrature",
         single_form='explicit', calculate_fluxes='off', query='nearest_neighbor',
         w_single_form='TTHG', w_multi_form='TTHG', psingle_form='TTHG', 
-        w_single_rayleigh = 'on', w_multi_rayleigh='on', psingle_rayleigh='on'):
+        w_single_rayleigh = 'on', w_multi_rayleigh='on', psingle_rayleigh='on', 
+        get_lvl_flux = False):
         """
         This function REsets all the default approximations in the code from what is in config file.
         This means that it will rewrite what is specified via config file defaults.
         It transforms the string specificatons
         into a number so that they can be used in numba nopython routines. 
 
         To see the `str` cases such as `TTHG_ray` users see all the options by using the function `justdoit.single_phase_options`
@@ -3462,15 +3362,21 @@
             Scattering phase function approximation for psingle in SH
         w_single_rayleigh : str 
             Toggle rayleigh scattering on/off for single scattering in SH
         w_multi_rayleigh : str 
             Toggle rayleigh scattering on/off for multi scattering in SH
         psingle_rayleigh : str 
             Toggle rayleigh scattering on/off for psingle in SH
+        get_lvl_flux : bool 
+            This parameter returns the level by level and layer by layer 
+            fluxes in the full output
+            Default is False
         """
+        self.inputs['approx']['get_lvl_flux'] = get_lvl_flux
+
         self.inputs['approx']['rt_method'] = rt_method
 
         #common to any RT code
         if rt_method == 'toon':
                 self.inputs['approx']['rt_params']['common']['stream'] = 2 # having method="Toon" and stream=4 messes up delta-eddington stuff
         else:
                 self.inputs['approx']['rt_params']['common']['stream'] = stream
@@ -3627,17 +3533,17 @@
         """
         if Teff is not None:
             self.inputs['planet']['T_eff'] = Teff
         else :
             self.inputs['planet']['T_eff'] = 0
 
     def inputs_climate(self, temp_guess= None, pressure= None, rfaci = 1,nofczns = 1 ,
-        nstr = None,  rfacv = None, cloudy = False,
-        mh = None, CtoO = None, species = None, fsed = None, T_star = None, 
-        logg= None, metal=None, r_star= None, semi_major = None,r_planet=None):
+        nstr = None,  rfacv = None, m_planet=None,r_planet=None,
+        cloudy = False, mh = None, CtoO = None, species = None, fsed = None, mieff_dir = None,
+        photochem=False, photochem_file=None,photochem_stfile = None,photonetwork_file = None,photonetworkct_file=None,tstop=1e7,psurf=10):
         """
         Get Inputs for Climate run
 
         Parameters
         ----------
         temp_guess : array 
             Guess T(P) profile to begin with
@@ -3668,32 +3574,25 @@
             Metallicity string for 1060 grid, '+0.5','0.0','-0.5'.
         CtoO : string
             C/O ratio string for 1060 grid
         species : string
             Cloud species to be included if cloudy
         fsed : float
             Sedimentation Efficiency (f_sed) if cloudy
-        T_star : float
-            Star effective temperature if irradiated
-        logg : float
-            Star log(g)
-        metal : float
-            Star Metallicity
-        r_star : float
-            Stellar Radius in R_sun
-        semi_major : float
-            Semi-major axis of Planet (AU)
-        r_planet : planet radius
-            Radius of Planet (Rj)
-
-        
+        mieff_dir: str
+            path to directory with mieff files for virga
+        photochem : bool 
+            Turns off (False) and on (True) Photochem 
         """
+        
         if cloudy: 
-            raise Exception('Cloudy functionality still in beta form and not ready for public use.')
-        else: 
+            print("Cloudy functionality still in beta form and not ready for public use.")
+            # raise Exception('Cloudy functionality still in beta fosrm and not ready for public use.')
+        
+        elif photochem == False: 
             #dummy values only used for cloud model
             mh = 0 
             CtoO = 0 
 
         if self.inputs['planet']['T_eff'] == 0.0:
             raise Exception('Need to specify Teff with jdi.input for climate run')
         if self.inputs['planet']['gravity'] == 0.0:
@@ -3706,33 +3605,58 @@
         self.inputs['climate']['nofczns'] = nofczns
         self.inputs['climate']['rfacv'] = rfacv
         self.inputs['climate']['rfaci'] = rfaci
         if cloudy:
             self.inputs['climate']['cloudy'] = 1
             self.inputs['climate']['cld_species'] = species
             self.inputs['climate']['fsed'] = fsed
+            self.inputs['climate']['mieff_dir'] = mieff_dir
         else :
             self.inputs['climate']['cloudy'] = 0
             self.inputs['climate']['cld_species'] = 0
             self.inputs['climate']['fsed'] = 0
+            self.inputs['climate']['mieff_dir'] = mieff_dir
         self.inputs['climate']['mh'] = mh
         self.inputs['climate']['CtoO'] = CtoO
-        
-        # star properties needed to change wv grid for diseq runs
-        self.inputs['climate']['T_star'] = T_star #K
-        self.inputs['climate']['r_star'] = r_star # solar
-        self.inputs['climate']['logg'] = logg # cgs
-        self.inputs['climate']['metal'] = metal # solar
-        self.inputs['climate']['semi_major'] = semi_major # au
-        self.inputs['climate']['r_planet'] = r_planet # jupiter radii
+
+
+        if photochem:
+            if m_planet is None:
+                raiseExceptions("Supply planet mass if you want to run photochem")
+            else:
+                self.inputs['climate']['m_planet'] = m_planet
+
+            if r_planet is None:
+                raiseExceptions("Supply planet radius if you want to run photochem")
+            else:
+                self.inputs['climate']['r_planet'] = r_planet
+
+            if photochem_file is None:
+                raiseExceptions("Supply photochem_filename if you want to run photochem")
+            else:
+                self.inputs['climate']['photochem_file'] =photochem_file
+
+            if photochem_stfile is None:
+                raiseExceptions("Supply photochem star filename if you want to run photochem")
+            else:
+                self.inputs['climate']['photochem_stfile'] =photochem_stfile
+            self.inputs['climate']['tstop'] =tstop
+            self.inputs['climate']['psurf'] =psurf
+            self.inputs['climate']['photochem'] =photochem
+            self.inputs['climate']['photochem_network'] =photonetwork_file
+            self.inputs['climate']['photochem_networkct'] =photonetworkct_file
+            
+
+        else:
+            self.inputs['climate']['photochem'] =False
 
     def climate(self, opacityclass, save_all_profiles = False, as_dict=True,with_spec=False,
         save_all_kzz = False, diseq_chem = False, self_consistent_kzz =False, kz = None, 
-        on_fly=False,gases_fly=None, chemeq_first=True):#,
-        #vulcan_run = False, photochem=False,on_fly=False,gases_fly=None,mhdeq=None,CtoOdeq=None ):
+        on_fly=False,gases_fly=None, chemeq_first=True,verbose=True):#,
+       
         """
         Top Function to run the Climate Model
 
         Parameters
         -----------
         opacityclass : class
             Opacity class from `justdoit.opannection`
@@ -3744,26 +3668,19 @@
             If you want to save and return all iterations in the kzz profile,True/False
         diseq_chem : bool
             If you want to run `on-the-fly' mixing (takes longer),True/False
         self_consistent_kzz : bool
             If you want to run MLT in convective zones and Moses in the radiative zones
         kz : array
             Kzz input array if user wants constant or whatever input profile (cgs)
-        vulcan_run : bool
-            (beta, contact developers)If you want to run vulcan on the fly (takes longer),True/False
-        photochem : bool
-            (beta, contact developers)If you want to run photochemistry in vulcan on the fly (takes much longer),True/False
-        
+        verbose : bool  
+            If True, triggers prints throughout code 
         """
         #save to user 
         all_out = {}
-
-        vulcan_run=False;photochem=False;#on_fly=False;gases_fly=None;mhdeq=None;CtoOdeq=None
-        if (vulcan_run or photochem): 
-            raise Exception("Vulcan and photochemistry is not yet a live feature. If you are interesting in helping the development team, contact us.")
         
         #get necessary parameters from opacity ck-tables 
         wno = opacityclass.wno
         delta_wno = opacityclass.delta_wno
         nwno = opacityclass.nwno
         min_temp = min(opacityclass.temps)
         max_temp = max(opacityclass.temps)
@@ -3776,35 +3693,40 @@
         #we will extend the black body grid 30% beyond the min and max temp of the 
         #opacity grid just to be safe with the spline
         extension = 0.3 
         tmin = min_temp*(1-extension)
         tmax = max_temp*(1+extension)
         ntmps = int((tmax-tmin)/dt)
         
-        bb , y2 , tp = set_bb(wno,delta_wno,nwno,ntmps,dt,tmin,tmax)
+        bb , y2 , tp = 0,0,0
+        #bb , y2 , tp = set_bb_deprecate(wno,delta_wno,nwno,ntmps,dt,tmin,tmax)
 
         nofczns = self.inputs['climate']['nofczns']
         nstr= self.inputs['climate']['nstr']
 
         rfaci= self.inputs['climate']['rfaci']
         
         #turn off stellar radiation if user has run "setup_nostar() function"
-        if 'nostar' in self.inputs['star'].values():
+        if 'nostar' in self.inputs['star']['database']:
             rfacv=0.0 
             FOPI = np.zeros(nwno) + 1.0
         #otherwise assume that there is stellar irradiation 
         else:
             rfacv = self.inputs['climate']['rfacv']
             r_star = self.inputs['star']['radius'] 
             r_star_unit = self.inputs['star']['radius_unit'] 
             semi_major = self.inputs['star']['semi_major']
             semi_major_unit = self.inputs['star']['semi_major_unit'] 
             fine_flux_star  = self.inputs['star']['flux']  # erg/s/cm^2
             FOPI = fine_flux_star * ((r_star/semi_major)**2)
 
+        #turn off reflected light permanently for all these runs if rfacv=0 
+        if rfacv==0:compute_reflected=False
+        else:compute_reflected=True
+
         all_profiles= []
         if save_all_profiles:
             save_profile = 1
         else :
             save_profile = 0
 
         TEMP1 = self.inputs['climate']['guess_temp']
@@ -3814,25 +3736,27 @@
         p_table = self.inputs['climate']['p_table']
         grad = self.inputs['climate']['grad']
         cp = self.inputs['climate']['cp']
 
 
         Teff = self.inputs['planet']['T_eff']
         grav = 0.01*self.inputs['planet']['gravity'] # cgs to si
-        mh = float(self.inputs['climate']['mh'])
+        mh = self.inputs['climate']['mh']
+        mh = float(mh) if mh is not None else 0
         sigma_sb = 0.56687e-4 # stefan-boltzmann constant
         
         col_den = 1e6*(pressure[1:] -pressure[:-1] ) / (grav/0.01) # cgs g/cm^2
         wave_in, nlevel, pm, hratio = 0.9, len(pressure), 0.001, 0.1
         #tidal = tidal_flux(Teff, wave_in,nlevel, pressure, pm, hratio, col_den)
         tidal = np.zeros_like(pressure) - sigma_sb *(Teff**4)
         
         cloudy = self.inputs['climate']['cloudy']
         cld_species = self.inputs['climate']['cld_species']
         fsed = self.inputs['climate']['fsed']
+        mieff_dir = self.inputs['climate']['mieff_dir']
         
         opd_cld_climate = np.zeros(shape=(nlevel-1,nwno,4))
         g0_cld_climate = np.zeros(shape=(nlevel-1,nwno,4))
         w0_cld_climate = np.zeros(shape=(nlevel-1,nwno,4))
 
 
         # first conv call
@@ -3844,94 +3768,105 @@
         x_max_mult=7.0
         
 
         final = False
         flag_hack = False
 
         
-        if chemeq_first: pressure, temperature, dtdp, profile_flag, all_profiles,opd_cld_climate,g0_cld_climate,w0_cld_climate,flux_net_ir_layer, flux_plus_ir_attop = profile(it_max, itmx, conv, convt, nofczns,nstr,x_max_mult,
+        if chemeq_first: pressure, temperature, dtdp, profile_flag, all_profiles,opd_cld_climate,g0_cld_climate,w0_cld_climate,cld_out,flux_net_ir_layer, flux_plus_ir_attop = profile(mieff_dir,it_max, itmx, conv, convt, nofczns,nstr,x_max_mult,
             TEMP1,pressure, FOPI, t_table, p_table, grad, cp, opacityclass, grav, 
-            rfaci, rfacv, nlevel, tidal, tmin, tmax, delta_wno, bb , y2 , tp, final , cloudy, cld_species,mh,fsed,flag_hack, save_profile,all_profiles,opd_cld_climate,g0_cld_climate,w0_cld_climate,first_call_ever=True)
+            rfaci, rfacv, nlevel, tidal, tmin, tmax, delta_wno, bb , y2 , tp, final , 
+            cloudy, cld_species,mh,fsed,flag_hack, save_profile,all_profiles,
+            opd_cld_climate,g0_cld_climate,w0_cld_climate,
+            first_call_ever=True, verbose=verbose)
 
         # second convergence call
         it_max= 7
         itmx= 5
         conv = 5.0
         convt=4.0
         x_max_mult=7.0
 
         
         final = False
-        if chemeq_first: pressure, temperature, dtdp, profile_flag, all_profiles,opd_cld_climate,g0_cld_climate,w0_cld_climate,flux_net_ir_layer, flux_plus_ir_attop = profile(it_max, itmx, conv, convt, nofczns,nstr,x_max_mult,
+        if chemeq_first: pressure, temperature, dtdp, profile_flag, all_profiles,opd_cld_climate,g0_cld_climate,w0_cld_climate,cld_out,flux_net_ir_layer, flux_plus_ir_attop = profile(mieff_dir, it_max, itmx, conv, convt, nofczns,nstr,x_max_mult,
                     temperature,pressure, FOPI, t_table, p_table, grad, cp, opacityclass, grav, 
-                    rfaci, rfacv, nlevel, tidal, tmin, tmax, delta_wno, bb , y2 , tp, final, cloudy, cld_species, mh,fsed,flag_hack,save_profile,all_profiles,opd_cld_climate,g0_cld_climate,w0_cld_climate,flux_net_ir_layer, flux_plus_ir_attop )   
+                    rfaci, rfacv, nlevel, tidal, tmin, tmax, delta_wno, bb , y2 , tp, final, cloudy, 
+                    cld_species, mh,fsed,flag_hack,save_profile,all_profiles,
+                    opd_cld_climate,g0_cld_climate,w0_cld_climate,flux_net_ir_layer, 
+                    flux_plus_ir_attop, verbose=verbose )   
 
-        if chemeq_first: pressure, temp, dtdp, nstr_new, flux_plus_final, df, all_profiles, opd_now,w0_now,g0_now =find_strat(pressure, temperature, dtdp ,FOPI, nofczns,nstr,x_max_mult,
+        if chemeq_first: 
+            pressure, temp, dtdp, nstr_new, flux_plus_final, df, all_profiles, cld_out, final_conv_flag=find_strat(mieff_dir, pressure, temperature, dtdp ,FOPI, nofczns,nstr,x_max_mult,
                              t_table, p_table, grad, cp, opacityclass, grav, 
-                             rfaci, rfacv, nlevel, tidal, tmin, tmax, delta_wno, bb , y2 , tp , cloudy, cld_species, mh,fsed, flag_hack, save_profile,all_profiles,opd_cld_climate,g0_cld_climate,w0_cld_climate,flux_net_ir_layer, flux_plus_ir_attop)
-
+                             rfaci, rfacv, nlevel, tidal, tmin, tmax, delta_wno, bb , y2 , tp , cloudy, cld_species, mh,fsed, flag_hack, save_profile,all_profiles,opd_cld_climate,g0_cld_climate,w0_cld_climate,flux_net_ir_layer, flux_plus_ir_attop,
+                             verbose=verbose)
+            if cloudy == 1:
+                opd_now,w0_now,g0_now = cld_out['opd_per_layer'],cld_out['single_scattering'],cld_out['asymmetry']
+            else:
+                opd_now,w0_now,g0_now = 0,0,0
         
         if diseq_chem:
             #Starting with user's guess since there was no request to converge a chemeq profile first 
             if not chemeq_first: 
                 temp = TEMP1
 
             wv196 = 1e4/wno
 
             # first change the nstr vector because need to check if they grow or not
             # delete upper convective zone if one develops
             
-            del_zone =4 # move 4 levels deeper
+            del_zone =0 # move 4 levels deeper
             if (nstr[1] > 0) & (nstr[4] > 0) & (nstr[3] > 0) :
                 nstr[1] = nstr[4]+del_zone
                 nstr[2] = 89
                 nstr[3],nstr[4],nstr[5] = 0,0,0
                 
-                print("2 conv Zones, so making small adjustments")
+                if verbose: print("2 conv Zones, so making small adjustments")
             elif (nstr[1] > 0) & (nstr[3] == 0):
                 if nstr[4] == 0:
                     nstr[1]+= del_zone #5#15
                 else:
                     nstr[1] += del_zone #5#15  
                     nstr[3], nstr[4] ,nstr[5] = 0,0,0#6#16
-                print("1 conv Zone, so making small adjustment")
+                if verbose: print("1 conv Zone, so making small adjustment")
             if nstr[1] >= nlevel -2 : # making sure we haven't pushed zones too deep
                 nstr[1] = nlevel -4
             if nstr[4] >= nlevel -2:
                 nstr[4] = nlevel -3
             
-            print("New NSTR status is ", nstr)
+            if verbose: print("New NSTR status is ", nstr)
 
             
 
             bundle = inputs(calculation='brown')
 
-            bundle.phase_angle(0)
+            bundle.phase_angle(0,num_gangle=10, num_tangle=1)
             bundle.gravity(gravity=grav , gravity_unit=u.Unit('m/s**2'))
             bundle.add_pt( temp, pressure)
             bundle.premix_atmosphere(opacityclass, df = bundle.inputs['atmosphere']['profile'].loc[:,['pressure','temperature']])
             DTAU, TAU, W0, COSB,ftau_cld, ftau_ray,GCOS2, DTAU_OG, TAU_OG, W0_OG, COSB_OG, \
                 W0_no_raman , surf_reflect, ubar0,ubar1,cos_theta, single_phase,multi_phase, \
-                frac_a,frac_b,frac_c,constant_back,constant_forward, tridiagonal , \
-                wno,nwno,ng,nt, nlevel, ngauss, gauss_wts, mmw =  calculate_atm(bundle, opacityclass)
+                frac_a,frac_b,frac_c,constant_back,constant_forward, \
+                wno,nwno,ng,nt, nlevel, ngauss, gauss_wts, mmw,gweight,tweight =  calculate_atm(bundle, opacityclass)
             
             all_kzz= []
             if save_all_kzz == True :
                 save_kzz = 1
             else :
                 save_kzz = 0
             
             #here begins the self consistent Kzz calculation 
             # MLT plus some prescription in radiative zone
             if self_consistent_kzz or (not chemeq_first): 
-                
-                flux_net_v_layer_full, flux_net_v_full, flux_plus_v_full, flux_minus_v_full , flux_net_ir_layer_full, flux_net_ir_full, flux_plus_ir_full, flux_minus_ir_full = climate(pressure, temp, delta_wno, bb , y2, tp, tmin, tmax, DTAU, TAU, W0, 
+                #flux_net_v_layer, flux_net_v, flux_plus_v, flux_minus_v , flux_net_ir_layer, flux_net_ir, flux_plus_ir, flux_minus_ir
+                flux_net_v_layer_full, flux_net_v_full, flux_plus_v_full, flux_minus_v_full , flux_net_ir_layer_full, flux_net_ir_full, flux_plus_ir_full, flux_minus_ir_full = get_fluxes(pressure, temp, delta_wno, bb , y2, tp, tmin, tmax, DTAU, TAU, W0, 
                 COSB,ftau_cld, ftau_ray,GCOS2, DTAU_OG, TAU_OG, W0_OG, COSB_OG, W0_no_raman , surf_reflect, 
-                ubar0,ubar1,cos_theta, FOPI, single_phase,multi_phase,frac_a,frac_b,frac_c,constant_back,constant_forward, tridiagonal , 
-                wno,nwno,ng,nt, nlevel, ngauss, gauss_wts,True, True)#True for reflected, True for thermal
+                ubar0,ubar1,cos_theta, FOPI, single_phase,multi_phase,frac_a,frac_b,frac_c,constant_back,constant_forward, 
+                wno,nwno,ng,nt,gweight,tweight, nlevel, ngauss, gauss_wts,compute_reflected, True)#True for reflected, True for thermal
 
                 flux_net_ir_layer = flux_net_ir_layer_full[:]
                 flux_plus_ir_attop = flux_plus_ir_full[0,:] 
                 calc_type = 0
                 
                 # use mixing length theory to calculate Kzz profile
                 if self_consistent_kzz: 
@@ -3942,15 +3877,15 @@
             
             # shift everything to the 661 grid now.
             #mh = '+0.0'  #don't change these as the opacities you are using are based on these 
             #CtoO = '1.0' # don't change these as the opacities you are using are based on these #
             filename_db=os.path.join(__refdata__, 'climate_INPUTS/ck_cx_cont_opacities_661.db')
             
             if on_fly:
-                print("From now I will mix "+str(gases_fly)+" only on--the--fly")
+                if verbose: print("From now I will mix "+str(gases_fly)+" only on--the--fly")
                 #mhdeq and ctodeq will be auto by opannection
                 #NO Background, just CIA + whatever in gases_fly
                 #ck_db=os.path.join(__refdata__, 'climate_INPUTS/sonora_2020_feh'+mhdeq+'_co_'+CtoOdeq+'.data.196')
                 opacityclass = opannection(ck=True, 
                     ck_db=opacityclass.ck_filename,filename_db=filename_db,
                     deq = True,on_fly=True,gases_fly=gases_fly)
             else:
@@ -3962,41 +3897,46 @@
 
         
             
             
             if cloudy == 1:    
                 wv661 = 1e4/opacityclass.wno
                 opd_cld_climate,g0_cld_climate,w0_cld_climate = initiate_cld_matrices(opd_cld_climate,g0_cld_climate,w0_cld_climate,wv196,wv661)
-                print(np.shape(opd_cld_climate))
             
             #Rerun star so that F0PI can now be on the 
             #661 grid 
-            if 'nostar' in self.inputs['star'].values():
+            if 'nostar' in self.inputs['star']['database']:
                 FOPI = np.zeros(opacityclass.nwno) + 1.0
             else:
                 T_star = self.inputs['star']['temp']
                 r_star = self.inputs['star']['radius']
                 r_star_unit = self.inputs['star']['radius_unit']
                 logg = self.inputs['star']['logg']
                 metal =  self.inputs['star']['metal']
                 semi_major = self.inputs['star']['semi_major']
                 sm_unit = self.inputs['star']['semi_major_unit']
                 database = self.inputs['star']['database']
+                filename = self.inputs['star']['filename']
+                f_unit = self.inputs['star']['f_unit']
+                w_unit = self.inputs['star']['w_unit']
                 self.star(opacityclass, database=database,temp =T_star,metal =metal, logg =logg, 
                     radius = r_star, radius_unit=u.Unit(r_star_unit),semi_major= semi_major , 
-                    semi_major_unit = u.Unit(sm_unit))
+                    semi_major_unit = u.Unit(sm_unit), 
+                    filename = filename, 
+                    f_unit=f_unit, 
+                    w_unit=w_unit)
                 fine_flux_star  = self.inputs['star']['flux']  # erg/s/cm^2
                 FOPI = fine_flux_star * ((r_star/semi_major)**2)
             
-            if not vulcan_run:
+            if self.inputs['climate']['photochem']==False:
                 quench_levels, t_mix = quench_level(pressure, temp, kz ,mmw, grav, return_mix_timescale= True) # determine quench levels
 
                 all_kzz = np.append(all_kzz, t_mix) # save kzz
 
-                print("Quench Levels are CO, CO2, NH3, HCN, PH3 ", quench_levels) # print quench levels
+                if verbose: print("Quench Levels are CO, CO2, NH3, HCN, PH3 ", quench_levels) # print quench levels
                 
                 final = False
                 #finall = False #### what is this thing?
                 
                 ## this code block is mostly safeguarding
                 
                 if quench_levels[2] > nlevel -2 :
@@ -4017,70 +3957,108 @@
 
                 # determine the chemistry now
 
                 qvmrs, qvmrs2= bundle.premix_atmosphere_diseq(opacityclass, df = bundle.inputs['atmosphere']['profile'].loc[:,['pressure','temperature']], quench_levels= quench_levels,t_mix=t_mix)
                 #was for check SM
                 #bundle.inputs['atmosphere']['profile'].to_csv('/data/users/samukher/Disequilibrium-picaso/first_iteration_testpls300min500',sep='\t')
                 #raise SystemExit(0) 
+                photo_inputs_dict = {}
+                photo_inputs_dict['yesorno'] = False
             else :
-                t_mix = bundle.run_vulcan(pressure,temp,kz,grav,mmw,T_star=T_star, logg=logg,metal=metal,r_star=metal,semi_major=semi_major,r_planet=r_planet, first = True, photochem=photochem)    
-                all_kzz = np.append(all_kzz, t_mix)
+                bundle.premix_atmosphere(opacityclass, df = bundle.inputs['atmosphere']['profile'].loc[:,['pressure','temperature']])
+
+                pc= bundle.call_photochem(temp,pressure,float(self.inputs['climate']['mh']),float(self.inputs['climate']['CtoO']),self.inputs['climate']['psurf'],self.inputs['climate']['m_planet'],self.inputs['climate']['r_planet'],kz,tstop=self.inputs['climate']['tstop'],filename = self.inputs['climate']['photochem_file'],stfilename = self.inputs['climate']['photochem_stfile'],network = self.inputs['climate']['photochem_network'],network_ct = self.inputs['climate']['photochem_networkct'],first=True,pc=None)
+                all_kzz = np.append(all_kzz, kz)
                 quench_levels = np.array([0,0,0,0])
+                photo_inputs_dict = {}
+                photo_inputs_dict['yesorno'] = True
+                photo_inputs_dict['mh'] = float(self.inputs['climate']['mh'])
+                photo_inputs_dict['CtoO'] = float(self.inputs['climate']['CtoO'])
+                photo_inputs_dict['psurf'] = self.inputs['climate']['psurf']
+                photo_inputs_dict['m_planet'] = self.inputs['climate']['m_planet']
+                photo_inputs_dict['r_planet'] = self.inputs['climate']['r_planet']
+                photo_inputs_dict['tstop']=self.inputs['climate']['tstop']
+                photo_inputs_dict['photochem_file']=self.inputs['climate']['photochem_file']
+                photo_inputs_dict['photochem_stfile']=self.inputs['climate']['photochem_stfile']
+                photo_inputs_dict['photochem_network']=self.inputs['climate']['photochem_network']
+                photo_inputs_dict['photochem_networkct']=self.inputs['climate']['photochem_networkct']
+                photo_inputs_dict['pc'] = pc
+                photo_inputs_dict['kz'] = kz
+                
+
+
+
 
 
             wno = opacityclass.wno
             delta_wno = opacityclass.delta_wno
             nwno = opacityclass.nwno
             min_temp = min(opacityclass.temps)
             max_temp = max(opacityclass.temps)
 
-           
-            print(nwno)             
             # first calculate the BB grid
             ntmps = self.inputs['climate']['ntemp_bb_grid']
             dt = self.inputs['climate']['dt_bb_grid']
             
             extension = 0.3 
             tmin = min_temp*(1-extension)
             tmax = max_temp*(1+extension)
 
             ntmps = int((tmax-tmin)/dt)
             
 
-            bb , y2 , tp = set_bb(wno,delta_wno,nwno,ntmps,dt,tmin,tmax)
+            #bb , y2 , tp = set_bb(wno,delta_wno,nwno,ntmps,dt,tmin,tmax)
 
         
 
             
             final = False
 
             
             # diseq calculations start here actually
             
-            print("DOING DISEQ CALCULATIONS NOW")
+            if verbose: print("DOING DISEQ CALCULATIONS NOW")
             it_max= 7
             itmx= 5
             conv = 5.0
             convt=4.0
             x_max_mult=7.0
 
             #if nstr[2] < nstr[5]:
             #    nofczns = 2
             #    print("nofczns corrected") 
 
-            
-            pressure, temperature, dtdp, profile_flag, qvmrs, qvmrs2, all_profiles, all_kzz,opd_cld_climate,g0_cld_climate,w0_cld_climate,flux_net_ir_layer, flux_plus_ir_attop  = profile_deq(it_max, itmx, conv, convt, nofczns,nstr,x_max_mult,
-            temp,pressure, FOPI, t_table, p_table, grad, cp, opacityclass, grav, 
-            rfaci, rfacv, nlevel, tidal, tmin, tmax, delta_wno, bb , y2 , tp, final , cloudy, cld_species,mh,fsed,flag_hack, quench_levels, kz, mmw,save_profile,all_profiles, self_consistent_kzz,save_kzz,all_kzz, vulcan_run,opd_cld_climate,g0_cld_climate,w0_cld_climate,flux_net_ir_layer, flux_plus_ir_attop,on_fly=on_fly, gases_fly=gases_fly )
-            
-            pressure, temp, dtdp, nstr_new, flux_plus_final, qvmrs, qvmrs2, df, all_profiles, all_kzz,opd_now,g0_now,w0_now =find_strat_deq(pressure, temperature, dtdp ,FOPI, nofczns,nstr,x_max_mult,
-                            t_table, p_table, grad, cp, opacityclass, grav, 
-                            rfaci, rfacv, nlevel, tidal, tmin, tmax, delta_wno, bb , y2 , tp , cloudy, cld_species, mh,fsed, flag_hack, quench_levels,kz ,mmw, save_profile,all_profiles, self_consistent_kzz,save_kzz,all_kzz, vulcan_run,opd_cld_climate,g0_cld_climate,w0_cld_climate,flux_net_ir_layer, flux_plus_ir_attop,on_fly=on_fly, gases_fly=gases_fly  )
-            
+            if self.inputs['climate']['photochem']==False:
+                pressure, temperature, dtdp, profile_flag, qvmrs, qvmrs2, all_profiles, all_kzz,opd_cld_climate,g0_cld_climate,w0_cld_climate,cld_out,flux_net_ir_layer, flux_plus_ir_attop,photo_inputs_dict,_  = profile_deq(mieff_dir, it_max, itmx, conv, convt, nofczns,nstr,x_max_mult,
+                temp,pressure, FOPI, t_table, p_table, grad, cp, opacityclass, grav, 
+                rfaci, rfacv, nlevel, tidal, tmin, tmax, delta_wno, bb , y2 , tp, final , 
+            cloudy, cld_species,mh,fsed,flag_hack, quench_levels, kz, mmw,save_profile,
+            all_profiles, self_consistent_kzz,save_kzz,all_kzz, opd_cld_climate,
+            g0_cld_climate,w0_cld_climate,flux_net_ir_layer, flux_plus_ir_attop,
+            photo_inputs_dict,
+            on_fly=on_fly, gases_fly=gases_fly, verbose=verbose)
+                
+                pressure, temp, dtdp, nstr_new, flux_plus_final, qvmrs, qvmrs2, df, all_profiles, all_kzz,cld_out,photo_inputs_dict,final_conv_flag=find_strat_deq(mieff_dir, pressure, temperature, dtdp ,FOPI, nofczns,nstr,x_max_mult,
+                                t_table, p_table, grad, cp, opacityclass, grav, 
+                                rfaci, rfacv, nlevel, tidal, tmin, tmax, delta_wno, bb , y2 , tp , cloudy, cld_species, mh,fsed, flag_hack, quench_levels,kz ,mmw, save_profile,all_profiles, self_consistent_kzz,save_kzz,all_kzz, opd_cld_climate,g0_cld_climate,w0_cld_climate,flux_net_ir_layer, flux_plus_ir_attop,photo_inputs_dict,on_fly=on_fly, gases_fly=gases_fly,
+                             verbose=verbose)
+                if cloudy == 1:
+                    opd_now,w0_now,g0_now = cld_out['opd_per_layer'],cld_out['single_scattering'],cld_out['asymmetry']
+                else:
+                    opd_now,w0_now,g0_now = 0,0,0
                 
+            else:
+                print("Only doing Profiles and not extending/reducing CZs")
+                pressure, temperature, dtdp, profile_flag, qvmrs, qvmrs2, all_profiles, all_kzz,opd_cld_climate,g0_cld_climate,w0_cld_climate,cld_out,flux_net_ir_layer, flux_plus_ir_attop,photo_inputs_dict, df  = profile_deq(mieff_dir, it_max, itmx, conv, convt, nofczns,nstr,x_max_mult,
+                temp,pressure, FOPI, t_table, p_table, grad, cp, opacityclass, grav, 
+                rfaci, rfacv, nlevel, tidal, tmin, tmax, delta_wno, bb , y2 , tp, final , cloudy, cld_species,mh,fsed,flag_hack, quench_levels, kz, mmw,save_profile,all_profiles, self_consistent_kzz,save_kzz,all_kzz, opd_cld_climate,g0_cld_climate,w0_cld_climate,flux_net_ir_layer, flux_plus_ir_attop,photo_inputs_dict,on_fly=on_fly, gases_fly=gases_fly)
+                nstr_new = nstr.copy()
+                flux_plus_final = flux_plus_ir_attop.copy()
+                temp=temperature.copy()
+
 
             #diseq stuff
             all_out['diseq_out'] = {}
             if save_all_kzz: all_out['diseq_out']['all_kzz'] = all_kzz
             all_out['diseq_out']['quench_levels'] = quench_levels
 
 
@@ -4089,29 +4067,53 @@
         #all output to user
         all_out['pressure'] = pressure
         all_out['temperature'] = temp
         all_out['ptchem_df'] = df
         all_out['dtdp'] = dtdp
         all_out['cvz_locs'] = nstr_new
         all_out['flux']=flux_plus_final
+        all_out['converged']=final_conv_flag
+
         if save_all_profiles: all_out['all_profiles'] = all_profiles            
-           
         if with_spec:
             opacityclass = opannection(ck=True, ck_db=opacityclass.ck_filename,deq=False)
             bundle = inputs(calculation='brown')
             bundle.phase_angle(0)
             bundle.gravity(gravity=grav , gravity_unit=u.Unit('m/s**2'))
             bundle.premix_atmosphere(opacityclass,df)
             df_spec = bundle.spectrum(opacityclass,full_output=True)    
             all_out['spectrum_output'] = df_spec 
 
+        #put cld output in all_out
+        if cloudy == 1:
+            df_cld = vj.picaso_format(opd_now, w0_now, g0_now, pressure = cld_out['pressure'], wavenumber=1e4/cld_out['wave'])
+            all_out['cld_output_picaso'] = df_cld
+            all_out['virga_output'] = cld_out
         if as_dict: 
             return all_out
         else: 
             return pressure , temp, dtdp, nstr_new, flux_plus_final, df, all_profiles , opd_now,w0_now,g0_now
+    
+    def call_photochem(self,temp,pressure,logMH, cto,pressure_surf,mass,radius,kzz,tstop=1e7,filename = None,stfilename=None,network=None,network_ct=None,first=True,pc=None,user_psurf=True,user_psurf_add=3):
+        p_target = np.logspace(np.log10(np.min(pressure)),np.log10(np.max(pressure)),180)
+        interp_function = interp1d(np.log10(pressure),np.log10(temp),bounds_error=False,fill_value='extrapolate')
+        interp_function_kzz = interp1d(np.log10(pressure),np.log10(kzz),bounds_error=False,fill_value='extrapolate')
+        interp_temp  = 10**interp_function(np.log10(p_target))
+        interp_kzz = 10**interp_function_kzz(np.log10(p_target))
+        pc,output_array,species,pressure = run_photochem(interp_temp,p_target,logMH, cto,pressure_surf,mass,radius,interp_kzz,tstop=tstop,filename = filename,stfilename=stfilename,network=network,network_ct= network_ct,first=first,pc=pc,user_psurf=user_psurf,user_psurf_add=user_psurf_add)
+        #pc,output_array,species,pressure = run_photochem(temp,pressure,logMH, cto,pressure_surf,mass,radius,kzz,tstop=tstop,filename = filename,stfilename=stfilename,network=network,network_ct= network_ct,first=False,pc=pc)
+        #pc,output_array,species,pressure = run_photochem(temp,pressure,logMH, cto,pressure_surf,mass,radius,kzz,tstop=tstop,filename = filename,stfilename=stfilename,network=network,network_ct= network_ct,first=False,pc=pc)
+        #pc,output_array,species,pressure = run_photochem(temp,pressure,logMH, cto,pressure_surf,mass,radius,kzz,tstop=tstop,filename = filename,stfilename=stfilename,network=network,network_ct= network_ct,first=False,pc=pc)
+        #pc,output_array,species,pressure = run_photochem(temp,pressure,logMH, cto,pressure_surf,mass,radius,kzz,tstop=tstop,filename = filename,stfilename=stfilename,network=network,network_ct= network_ct,first=False,pc=pc)
+        #pc,output_array,species,pressure = run_photochem(temp,pressure,logMH, cto,pressure_surf,mass,radius,kzz,tstop=tstop,filename = filename,stfilename=stfilename,network=network,network_ct= network_ct,first=False,pc=pc)
+
+        for i in range(len(species)):
+            interp_sp = interp1d(np.log10(p_target),np.log10(output_array[i,:]),bounds_error=False,fill_value='extrapolate')
+            self.inputs['atmosphere']['profile'][species[i]] = 10**interp_sp(np.log10(pressure))#output_array[i,:]
+        return pc
 
 def get_targets():
     """Function to grab available targets using exoplanet archive data. 
 
     Returns
     -------
     Dataframe from Exoplanet Archive
@@ -4258,15 +4260,15 @@
     add_kz : bool 
         Returns kzz along with PT info
     input_file : str 
         point to input file in the same format as mitgcm example 
         file in base_cases/HJ_3d.pt
     """
     #input_file = os.path.join(__refdata__, 'base_cases','HJ_3d.pt')
-    threed_grid = pd.read_csv(input_file,delim_whitespace=True,names=['p','t','k'])
+    threed_grid = pd.read_csv(input_file,sep='\s+',names=['p','t','k'])
     all_lon= threed_grid.loc[np.isnan(threed_grid['k'])]['p'].values
     all_lat=  threed_grid.loc[np.isnan(threed_grid['k'])]['t'].values
     latlong_ind = np.concatenate((np.array(threed_grid.loc[np.isnan(threed_grid['k'])].index),[threed_grid.shape[0]] ))
     threed_grid = threed_grid.dropna() 
 
     lon = np.unique(all_lon)
     lat = np.unique(all_lat)
@@ -4382,19 +4384,19 @@
 
     if mass == 'all':
         all_cols = np.concatenate([[cols_return[0]]]+[[f'{cols_return[1]}{iv}Mj',f'{cols_return[2]}{iv}Mj'] for iv in valid_options])
         for imass in valid_options:
             mass = f'00{imass}0'            
             if len(mass)==5:mass=mass[1:]
             cold = pd.read_csv(os.path.join(__refdata__, 'evolution','cold_start',f'model_seq.{mass}'),
-                skiprows=12,delim_whitespace=True,
+                skiprows=12,sep='\s+',
                     header=None,names=['age_years','logL','R_cm','Ts','Teff',
                                        'log rc','log Pc','log Tc','grav_cgs','Uth','Ugrav','log Lnuc'])
             hot = pd.read_csv(os.path.join(__refdata__, 'evolution','hot_start',f'model_seq.{mass}'),
-                skiprows=12,delim_whitespace=True,
+                skiprows=12,sep='\s+',
                     header=None,names=['age_years','logL','R_cm','Ts','Teff',
                                        'log rc','log Pc','log Tc','grav_cgs','Uth','Ugrav','log Lnuc'])
             if imass==1 :
                 all_cold = pd.DataFrame(columns=all_cols,index=range(cold.shape[0]))
                 all_cold['age_years'] = cold['age_years'].values
                 all_hot = pd.DataFrame(columns=all_cols,index=range(hot.shape[0]))
                 all_hot['age_years'] = hot['age_years'].values
@@ -4425,18 +4427,18 @@
                 'cold': all_cold}
     else:   
         
         idx = np.argmin(abs(valid_options - mass))
         mass = int(valid_options[idx])
         mass = f'00{mass}0'
         if len(mass)==5:mass=mass[1:]
-        cold = pd.read_csv(os.path.join(__refdata__, 'evolution','cold_start',f'model_seq.{mass}'),skiprows=12,delim_whitespace=True,
+        cold = pd.read_csv(os.path.join(__refdata__, 'evolution','cold_start',f'model_seq.{mass}'),skiprows=12,sep='\s+',
                     header=None,names=['age_years','logL','R_cm','Ts','Teff',
                                        'log rc','log Pc','log Tc','grav_cgs','Uth','Ugrav','log Lnuc'])
-        hot = pd.read_csv(os.path.join(__refdata__, 'evolution','hot_start',f'model_seq.{mass}'),skiprows=12,delim_whitespace=True,
+        hot = pd.read_csv(os.path.join(__refdata__, 'evolution','hot_start',f'model_seq.{mass}'),skiprows=12,sep='\s+',
                     header=None,names=['age_years','logL','R_cm','Ts','Teff',
                                        'log rc','log Pc','log Tc','grav_cgs','Uth','Ugrav','log Lnuc'])
         #return only what we want
         hot = hot.loc[:,cols_return]
         cold = cold.loc[:,cols_return]
 
         #grab the desired age, if the user asks for it
@@ -4476,24 +4478,27 @@
     if printout: print("Can use 2-stream or 4-stream sperhical harmonics")
     return [2,4]
 def toon_phase_coefficients(printout=True):
     """Retrieve options for coefficients used in Toon calculation
     """
     return ["quadrature","eddington"]
 
-def profile(it_max, itmx, conv, convt, nofczns,nstr,x_max_mult,
+def profile(mieff_dir, it_max, itmx, conv, convt, nofczns,nstr,x_max_mult,
             temp,pressure,FOPI, t_table, p_table, grad, cp, opacityclass, grav, 
              rfaci, rfacv, nlevel, tidal, tmin, tmax, dwni, bb , y2 , tp, final, 
              cloudy, cld_species,mh,fsed,flag_hack, save_profile, 
              all_profiles,opd_cld_climate,g0_cld_climate,w0_cld_climate,
-             flux_net_ir_layer=None, flux_plus_ir_attop=None,first_call_ever=False):
+             flux_net_ir_layer=None, flux_plus_ir_attop=None,first_call_ever=False,
+             verbose=True):
     """
     Function iterating on the TP profile by calling tstart and changing opacities as well
     Parameters
     ----------
+    mieff_dir: str
+        path to directory with mieff files for virga
     it_max : int
         Maximum iterations allowed in the inner no opa change loop
     itmx : int
         Maximum iterations allowed in the outer opa change loop
     conv : float
         
     convt: float
@@ -4553,15 +4558,15 @@
         
     Returns
     -------
     array 
         Temperature array and lapse ratio array if converged
         else Temperature array twice
     """
-
+    conv_flag = 0
     # taudif is fixed to be 0 here since it is needed only for clouds mh
     taudif = 0.0
     taudif_tol = 0.1
     
     # first calculate the convective zones
     for nb in range(0,3*nofczns,3):
         
@@ -4576,45 +4581,47 @@
             temp[j1]= exp(log(temp[j1-1]) + grad_x*(log(pressure[j1]) - log(pressure[j1-1])))
     
     temp_old= np.copy(temp)
 
 
     
     bundle = inputs(calculation='brown')
-    bundle.phase_angle(0)
+    bundle.phase_angle(0,num_gangle=10, num_tangle=1)
     bundle.gravity(gravity=grav , gravity_unit=u.Unit('m/s**2'))
     bundle.add_pt( temp, pressure)
     
     bundle.premix_atmosphere(opacityclass, df = bundle.inputs['atmosphere']['profile'].loc[:,['pressure','temperature']])
     if save_profile == 1:
             all_profiles = np.append(all_profiles,temp_old)
     
     if first_call_ever == False:
         if cloudy == 1 :
             DTAU, TAU, W0, COSB,ftau_cld, ftau_ray,GCOS2, DTAU_OG, TAU_OG, W0_OG, COSB_OG, \
             W0_no_raman , surf_reflect, ubar0,ubar1,cos_theta, single_phase,multi_phase, \
-            frac_a,frac_b,frac_c,constant_back,constant_forward, tridiagonal , \
-            wno,nwno,ng,nt, nlevel, ngauss, gauss_wts, mmw =  calculate_atm(bundle, opacityclass )
+            frac_a,frac_b,frac_c,constant_back,constant_forward,  \
+            wno,nwno,ng,nt, nlevel, ngauss, gauss_wts, mmw,gweight,tweight =  calculate_atm(bundle, opacityclass )
 
 
             we0,we1,we2,we3 = 0.25,0.25,0.25,0.25
             opd_prev_cld_step = (we0*opd_cld_climate[:,:,0]+we1*opd_cld_climate[:,:,1]+we2*opd_cld_climate[:,:,2]+we3*opd_cld_climate[:,:,3]) # last average
             
             metallicity = 10**(mh) #atmospheric metallicity relative to Solar
             mean_molecular_weight = np.mean(mmw) # atmospheric mean molecular weight
-            directory ='/Users/sagnickmukherjee/Documents/GitHub/virga/refr_new'
+            # directory ='/Users/sagnickmukherjee/Documents/GitHub/virga/refr_new'
+            # directory = '/home/jjm6243/dev_virga/'
+            directory = mieff_dir
             
             kzz  = get_kzz(pressure, temp,grav,mmw,tidal,flux_net_ir_layer, flux_plus_ir_attop,t_table, p_table, grad, cp, calc_type,nstr)
             bundle.inputs['atmosphere']['profile']['kz'] = kzz
         
 
             cld_out = bundle.virga(cld_species,directory, fsed=fsed,mh=metallicity,
-                        mmw = mean_molecular_weight,full_output=False,climate=True)
+                        mmw = mean_molecular_weight) #,climate=True)
             
-            opd_now, w0_now, g0_now = cld_out
+            opd_now, w0_now, g0_now = cld_out['opd_per_layer'],cld_out['single_scattering'],cld_out['asymmetry']
             
             opd_cld_climate[:,:,3], g0_cld_climate[:,:,3], w0_cld_climate[:,:,3] = opd_cld_climate[:,:,2], g0_cld_climate[:,:,2], w0_cld_climate[:,:,2]
             opd_cld_climate[:,:,2], g0_cld_climate[:,:,2], w0_cld_climate[:,:,2] = opd_cld_climate[:,:,1], g0_cld_climate[:,:,1], w0_cld_climate[:,:,1]
             opd_cld_climate[:,:,1], g0_cld_climate[:,:,1], w0_cld_climate[:,:,1] = opd_cld_climate[:,:,0], g0_cld_climate[:,:,0], w0_cld_climate[:,:,0]
                         
             opd_cld_climate[:,:,0], g0_cld_climate[:,:,0], w0_cld_climate[:,:,0] = opd_now, g0_now, w0_now
             
@@ -4634,38 +4641,44 @@
             g0_clmt = (we0*opd_cld_climate[:,:,0]*g0_cld_climate[:,:,0]+we1*opd_cld_climate[:,:,1]*g0_cld_climate[:,:,1]+we2*opd_cld_climate[:,:,2]*g0_cld_climate[:,:,2]+we3*opd_cld_climate[:,:,3]*g0_cld_climate[:,:,3])/(sum_opd_clmt)
             w0_clmt = (we0*opd_cld_climate[:,:,0]*w0_cld_climate[:,:,0]+we1*opd_cld_climate[:,:,1]*w0_cld_climate[:,:,1]+we2*opd_cld_climate[:,:,2]*w0_cld_climate[:,:,2]+we3*opd_cld_climate[:,:,3]*w0_cld_climate[:,:,3])/(sum_opd_clmt)
             g0_clmt = np.nan_to_num(g0_clmt,nan=0.0)
             w0_clmt = np.nan_to_num(w0_clmt,nan=0.0)
             opd_clmt[np.where(opd_clmt <= 1e-5)] = 0.0
             
             
-            df_cld = vj.picaso_format(opd_clmt, w0_clmt, g0_clmt)
+            df_cld = vj.picaso_format(opd_clmt, w0_clmt, g0_clmt, pressure = cld_out['pressure'], wavenumber= 1e4/cld_out['wave'])
             bundle.clouds(df=df_cld)
 
 
-
     DTAU, TAU, W0, COSB,ftau_cld, ftau_ray,GCOS2, DTAU_OG, TAU_OG, W0_OG, COSB_OG, \
         W0_no_raman , surf_reflect, ubar0,ubar1,cos_theta, single_phase,multi_phase, \
-        frac_a,frac_b,frac_c,constant_back,constant_forward, tridiagonal , \
-        wno,nwno,ng,nt, nlevel, ngauss, gauss_wts, mmw =  calculate_atm(bundle, opacityclass )
+        frac_a,frac_b,frac_c,constant_back,constant_forward, \
+        wno,nwno,ng,nt, nlevel, ngauss, gauss_wts, mmw,gweight,tweight =  calculate_atm(bundle, opacityclass )
     
     ## begin bigger loop which gets opacities
     for iii in range(itmx):
         
-        temp, dtdp, flag_converge, flux_net_ir_layer, flux_plus_ir_attop, all_profiles = t_start(nofczns,nstr,it_max,conv,x_max_mult, 
-            rfaci, rfacv, nlevel, temp, pressure, p_table, t_table, 
-            grad, cp, tidal,tmin,tmax,dwni, bb , y2, tp, DTAU, TAU, W0, COSB,ftau_cld, ftau_ray,GCOS2, DTAU_OG, TAU_OG, W0_OG, COSB_OG, W0_no_raman , surf_reflect, ubar0,ubar1,cos_theta, FOPI, single_phase,multi_phase,frac_a,frac_b,frac_c,constant_back,constant_forward, tridiagonal , wno,nwno,ng,nt, ngauss, gauss_wts, save_profile, all_profiles)
-        
-        if (temp <= min(opacityclass.cia_temps)).any():
-            wh = np.where(temp <= min(opacityclass.cia_temps))
-            if len(wh[0]) <= 30 :
-                print(len(wh[0])," points went off the opacity grid. Correcting those.")
-                temp = correct_profile(temp,pressure,wh,min(opacityclass.cia_temps))
-            else :
-                raise Exception('Many points in your profile went off the grid. Try re-starting from a different guess profile. Parametrized profiles can work better sometime as guess profiles.')
+        temp, dtdp, flag_converge, flux_net_ir_layer, flux_plus_ir_attop, all_profiles = t_start(
+                    nofczns,nstr,it_max,conv,x_max_mult, 
+                    rfaci, rfacv, nlevel, temp, pressure, p_table, t_table, 
+                    grad, cp, tidal,tmin,tmax,dwni, bb , y2, tp, DTAU, TAU, W0, COSB,ftau_cld, ftau_ray,GCOS2, 
+                    DTAU_OG, TAU_OG, W0_OG, COSB_OG, W0_no_raman , surf_reflect, 
+                    ubar0,ubar1,cos_theta, FOPI, single_phase,multi_phase,frac_a,frac_b,frac_c,constant_back,constant_forward, 
+                    wno,nwno,ng,nt,gweight,tweight, 
+                    ngauss, gauss_wts, save_profile, all_profiles,
+                    verbose=verbose)
+        
+        #NEB stage delete after confirmation from SM
+        #if (temp <= min(opacityclass.cia_temps)).any():
+        #    wh = np.where(temp <= min(opacityclass.cia_temps))
+        #    if len(wh[0]) <= 30 :
+        #        if verbose: print(len(wh[0])," points went below the opacity grid. Correcting those.")
+        #        temp = correct_profile(temp,pressure,wh,min(opacityclass.cia_temps))
+        #    else :
+        #        raise Exception('Many points in your profile went off the grid to lower temperatures. Try re-starting from a different guess profile. Parametrized profiles can work better sometime as guess profiles.')
         
         
         
         bundle = inputs(calculation='brown')
         bundle.phase_angle(0)
         bundle.gravity(gravity=grav , gravity_unit=u.Unit('m/s**2'))
         bundle.add_pt( temp, pressure)
@@ -4675,24 +4688,25 @@
         #    all_profiles = np.append(all_profiles,bundle.inputs['atmosphere']['profile']['NH3'].values)
         if cloudy == 1 :
             we0,we1,we2,we3 = 0.25,0.25,0.25,0.25
             opd_prev_cld_step = (we0*opd_cld_climate[:,:,0]+we1*opd_cld_climate[:,:,1]+we2*opd_cld_climate[:,:,2]+we3*opd_cld_climate[:,:,3]) # last average
             
             metallicity = 10**(mh) #atmospheric metallicity relative to Solar
             mean_molecular_weight = np.mean(mmw) # atmospheric mean molecular weight
-            directory ='/Users/sagnickmukherjee/Documents/GitHub/virga/refr_new'
-            
+            # directory ='/Users/sagnickmukherjee/Documents/GitHub/virga/refr_new'
+            # directory = '/home/jjm6243/dev_virga/'
+            directory = mieff_dir
+
             kzz  = get_kzz(pressure, temp,grav,mmw,tidal,flux_net_ir_layer, flux_plus_ir_attop,t_table, p_table, grad, cp, calc_type,nstr)
             bundle.inputs['atmosphere']['profile']['kz'] = kzz
-        
     
             cld_out = bundle.virga(cld_species,directory, fsed=fsed,mh=metallicity,
-                        mmw = mean_molecular_weight,full_output=False,climate=True)
-            
-            opd_now, w0_now, g0_now = cld_out
+                        mmw = mean_molecular_weight)#,climate=True)
+
+            opd_now, w0_now, g0_now = cld_out['opd_per_layer'],cld_out['single_scattering'],cld_out['asymmetry']
             
             opd_cld_climate[:,:,3], g0_cld_climate[:,:,3], w0_cld_climate[:,:,3] = opd_cld_climate[:,:,2], g0_cld_climate[:,:,2], w0_cld_climate[:,:,2]
             opd_cld_climate[:,:,2], g0_cld_climate[:,:,2], w0_cld_climate[:,:,2] = opd_cld_climate[:,:,1], g0_cld_climate[:,:,1], w0_cld_climate[:,:,1]
             opd_cld_climate[:,:,1], g0_cld_climate[:,:,1], w0_cld_climate[:,:,1] = opd_cld_climate[:,:,0], g0_cld_climate[:,:,0], w0_cld_climate[:,:,0]
                         
             opd_cld_climate[:,:,0], g0_cld_climate[:,:,0], w0_cld_climate[:,:,0] = opd_now, g0_now, w0_now
             
@@ -4712,227 +4726,70 @@
             g0_clmt = (we0*opd_cld_climate[:,:,0]*g0_cld_climate[:,:,0]+we1*opd_cld_climate[:,:,1]*g0_cld_climate[:,:,1]+we2*opd_cld_climate[:,:,2]*g0_cld_climate[:,:,2]+we3*opd_cld_climate[:,:,3]*g0_cld_climate[:,:,3])/(sum_opd_clmt)
             w0_clmt = (we0*opd_cld_climate[:,:,0]*w0_cld_climate[:,:,0]+we1*opd_cld_climate[:,:,1]*w0_cld_climate[:,:,1]+we2*opd_cld_climate[:,:,2]*w0_cld_climate[:,:,2]+we3*opd_cld_climate[:,:,3]*w0_cld_climate[:,:,3])/(sum_opd_clmt)
             g0_clmt = np.nan_to_num(g0_clmt,nan=0.0)
             w0_clmt = np.nan_to_num(w0_clmt,nan=0.0)
             opd_clmt[np.where(opd_clmt <= 1e-5)] = 0.0
             
             
-            df_cld = vj.picaso_format(opd_clmt, w0_clmt, g0_clmt)
+            df_cld = vj.picaso_format(opd_clmt, w0_clmt, g0_clmt,pressure = cld_out['pressure'], wavenumber= 1e4/cld_out['wave'])
             bundle.clouds(df=df_cld)
             
             diff = (opd_clmt-opd_prev_cld_step)
             taudif = np.max(np.abs(diff))
             taudif_tol = 0.4*np.max(0.5*(opd_clmt+opd_prev_cld_step))
             
             print("Max TAUCLD diff is", taudif, " Tau tolerance is ", taudif_tol)
-
+        else:
+            cld_out = 0
 
 
         
 
         DTAU, TAU, W0, COSB,ftau_cld, ftau_ray,GCOS2, DTAU_OG, TAU_OG, W0_OG, COSB_OG, \
         W0_no_raman , surf_reflect, ubar0,ubar1,cos_theta, single_phase,multi_phase, \
-        frac_a,frac_b,frac_c,constant_back,constant_forward, tridiagonal , \
-        wno,nwno,ng,nt, nlevel, ngauss, gauss_wts, mmw =  calculate_atm(bundle, opacityclass)
+        frac_a,frac_b,frac_c,constant_back,constant_forward,  \
+        wno,nwno,ng,nt, nlevel, ngauss, gauss_wts, mmw,gweight,tweight  =  calculate_atm(bundle, opacityclass)
 
         ert = 0.0 # avg temp change
         scalt= 1.5
 
         dtx= abs(temp-temp_old)
-        ert = np.sum(dtx)
-        
-        ## this is a terrible hack but it perhaps works
-        ## do this hack only during findstrat maybe ?
-        ## otherwise problematic
-        #####################################
-     #   if flag_hack == True:
-     #       temp= 0.5*(temp+temp_old) 
-     #       print("Hack Activated")
-        #####################################   
+        ert = np.sum(dtx) 
         
         temp_old= np.copy(temp)
         
         ert = ert/(float(nlevel)*scalt)
         
         if ((iii > 0) & (ert < convt) & (taudif < taudif_tol)) :
-            print("Profile converged")
+            if verbose: print("Profile converged before itmx")
             conv_flag = 1
-            '''
-            if final == True :
-                itmx = 6
-                it_max = it_max
-            else :
-                itmx = 3
-                it_max= it_max
-            
-            if cloudy == 1:
-                for iprime in range(itmx):
-                    bundle = inputs(calculation='brown')
-                    bundle.phase_angle(0)
-                    bundle.gravity(gravity=grav , gravity_unit=u.Unit('m/s**2'))
-                    bundle.add_pt( temp, pressure)
-    
-                    bundle.premix_atmosphere(opacityclass, df = bundle.inputs['atmosphere']['profile'].loc[:,['pressure','temperature']])
-                    
-                    
-                    metallicity = 10**(mh) #atmospheric metallicity relative to Solar
-                    mean_molecular_weight = np.mean(mmw) # atmospheric mean molecular weight
-                    directory ='/Users/sagnickmukherjee/Documents/software/optics'
-            
-                    kzz  = get_kzz(pressure, temp,grav,mmw,tidal,flux_net_ir_layer, flux_plus_ir_attop,t_table, p_table, grad, cp, calc_type,nstr)
-                    bundle.inputs['atmosphere']['profile']['kz'] = kzz
-        
-    
-                    cld_out = bundle.virga(cld_species,directory, fsed=fsed,mh=metallicity,
-                            mmw = mean_molecular_weight,full_output=False,climate=True)
-            
-                    opd_now, w0_now, g0_now = cld_out
-            
-                    opd_cld_climate[:,:,3], g0_cld_climate[:,:,3], w0_cld_climate[:,:,3] = opd_cld_climate[:,:,2], g0_cld_climate[:,:,2], w0_cld_climate[:,:,2]
-                    opd_cld_climate[:,:,2], g0_cld_climate[:,:,2], w0_cld_climate[:,:,2] = opd_cld_climate[:,:,1], g0_cld_climate[:,:,1], w0_cld_climate[:,:,1]
-                    opd_cld_climate[:,:,1], g0_cld_climate[:,:,1], w0_cld_climate[:,:,1] = opd_cld_climate[:,:,0], g0_cld_climate[:,:,0], w0_cld_climate[:,:,0]
-                        
-                    opd_cld_climate[:,:,0], g0_cld_climate[:,:,0], w0_cld_climate[:,:,0] = opd_now, g0_now, w0_now
-            
-            
-                    we0,we1,we2,we3 = 0.6,0.25,0.1,0.05
-            
-                    #sum_opd_clmt = (opd_cld_climate[:,:,0]+opd_cld_climate[:,:,1]+opd_cld_climate[:,:,2]+opd_cld_climate[:,:,3])
-                    sum_opd_clmt = (we0*opd_cld_climate[:,:,0]+we1*opd_cld_climate[:,:,1]+we2*opd_cld_climate[:,:,2]+we3*opd_cld_climate[:,:,3])
-                    opd_clmt = (we0*opd_cld_climate[:,:,0]+we1*opd_cld_climate[:,:,1]+we2*opd_cld_climate[:,:,2]+we3*opd_cld_climate[:,:,3])
-                    g0_clmt = (we0*opd_cld_climate[:,:,0]*g0_cld_climate[:,:,0]+we1*opd_cld_climate[:,:,1]*g0_cld_climate[:,:,1]+we2*opd_cld_climate[:,:,2]*g0_cld_climate[:,:,2]+we3*opd_cld_climate[:,:,3]*g0_cld_climate[:,:,3])/(sum_opd_clmt)
-                    w0_clmt = (we0*opd_cld_climate[:,:,0]*w0_cld_climate[:,:,0]+we1*opd_cld_climate[:,:,1]*w0_cld_climate[:,:,1]+we2*opd_cld_climate[:,:,2]*w0_cld_climate[:,:,2]+we3*opd_cld_climate[:,:,3]*w0_cld_climate[:,:,3])/(sum_opd_clmt)
-                    g0_clmt = np.nan_to_num(g0_clmt,nan=0.0)
-                    w0_clmt = np.nan_to_num(w0_clmt,nan=0.0)
-                    opd_clmt[np.where(opd_clmt <= 1e-5)] = 0.0
-            
-            
-                    df_cld = vj.picaso_format(opd_clmt, w0_clmt, g0_clmt)
-                    bundle.clouds(df=df_cld)
-                    #taudif = np.max(np.abs(opd_cld_climate[:,:,0]-opd_cld_climate[:,:,1]))
-                    #diff = (opd_cld_climate[:,:,0]-opd_cld_climate[:,:,1])/(0.5*(opd_cld_climate[:,:,0]+opd_cld_climate[:,:,1]))
-                    #diff = np.nan_to_num(diff,nan=0.0)
-                    #taudif = np.max(np.abs(diff))
-            
-                    #print("Max TAUCLD diff is", taudif, " Tau at layer 40 and wv 150 is ", opd_now[40,150])
-                    
-                    DTAU, TAU, W0, COSB,ftau_cld, ftau_ray,GCOS2, DTAU_OG, TAU_OG, W0_OG, COSB_OG, \
-                    W0_no_raman , surf_reflect, ubar0,ubar1,cos_theta, single_phase,multi_phase, \
-                    frac_a,frac_b,frac_c,constant_back,constant_forward, tridiagonal , \
-                    wno,nwno,ng,nt, nlevel, ngauss, gauss_wts, mmw =  calculate_atm(bundle, opacityclass)
-                
-                    temp, dtdp, flag_converge, flux_net_ir_layer, flux_plus_ir_attop, all_profiles = t_start(nofczns,nstr,it_max,conv,x_max_mult, 
-                    rfaci, rfacv, nlevel, temp, pressure, p_table, t_table, 
-                    grad, cp, tidal,tmin,tmax,dwni, bb , y2, tp, DTAU, TAU, W0, COSB,ftau_cld, ftau_ray,GCOS2, DTAU_OG, TAU_OG, W0_OG, COSB_OG, W0_no_raman , surf_reflect, ubar0,ubar1,cos_theta, FOPI, single_phase,multi_phase,frac_a,frac_b,frac_c,constant_back,constant_forward, tridiagonal , wno,nwno,ng,nt, ngauss, gauss_wts, save_profile, all_profiles)
-                
-                
-                
-                    ert = 0.0 # avg temp change
-                    scalt= 1.0
-                    dtx= abs(temp-temp_old)
-                    ert = np.sum(dtx)
-                    temp_old= np.copy(temp)
-                '''
 
-            return pressure, temp , dtdp, conv_flag, all_profiles, opd_cld_climate,g0_cld_climate,w0_cld_climate, flux_net_ir_layer, flux_plus_ir_attop
+            return pressure, temp , dtdp, conv_flag, all_profiles, opd_cld_climate,g0_cld_climate,w0_cld_climate, cld_out,flux_net_ir_layer, flux_plus_ir_attop
         
-        print("Big iteration is ",min(temp), iii)
-    conv_flag = 0
-    ## this is supposed to be useless so testing this
-    '''
-    if final == True :
-        itmx = 6
-        it_max = it_max
-    else :
-        itmx = 3
-        it_max= it_max
+        if verbose: print("Big iteration is ",min(temp), iii)
     
-    if cloudy == 1:
-        for iprime in range(itmx):
-            bundle = inputs(calculation='brown')
-            bundle.phase_angle(0)
-            bundle.gravity(gravity=grav , gravity_unit=u.Unit('m/s**2'))
-            bundle.add_pt( temp, pressure)
-    
-            bundle.premix_atmosphere(opacityclass, df = bundle.inputs['atmosphere']['profile'].loc[:,['pressure','temperature']])
-                    
-                    
-            metallicity = 10**(mh) #atmospheric metallicity relative to Solar
-            mean_molecular_weight = np.mean(mmw) # atmospheric mean molecular weight
-            directory ='/Users/sagnickmukherjee/Documents/software/optics'
-            
-            kzz  = get_kzz(pressure, temp,grav,mmw,tidal,flux_net_ir_layer, flux_plus_ir_attop,t_table, p_table, grad, cp, calc_type,nstr)
-            bundle.inputs['atmosphere']['profile']['kz'] = kzz
-        
-    
-            cld_out = bundle.virga(cld_species,directory, fsed=fsed,mh=metallicity,
-                            mmw = mean_molecular_weight,full_output=False,climate=True)
-            
-            opd_now, w0_now, g0_now = cld_out
-            
-            opd_cld_climate[:,:,3], g0_cld_climate[:,:,3], w0_cld_climate[:,:,3] = opd_cld_climate[:,:,2], g0_cld_climate[:,:,2], w0_cld_climate[:,:,2]
-            opd_cld_climate[:,:,2], g0_cld_climate[:,:,2], w0_cld_climate[:,:,2] = opd_cld_climate[:,:,1], g0_cld_climate[:,:,1], w0_cld_climate[:,:,1]
-            opd_cld_climate[:,:,1], g0_cld_climate[:,:,1], w0_cld_climate[:,:,1] = opd_cld_climate[:,:,0], g0_cld_climate[:,:,0], w0_cld_climate[:,:,0]
-                        
-            opd_cld_climate[:,:,0], g0_cld_climate[:,:,0], w0_cld_climate[:,:,0] = opd_now, g0_now, w0_now
-            
-            
-            we0,we1,we2,we3 = 0.6,0.25,0.1,0.05
-            
-            #sum_opd_clmt = (opd_cld_climate[:,:,0]+opd_cld_climate[:,:,1]+opd_cld_climate[:,:,2]+opd_cld_climate[:,:,3])
-            sum_opd_clmt = (we0*opd_cld_climate[:,:,0]+we1*opd_cld_climate[:,:,1]+we2*opd_cld_climate[:,:,2]+we3*opd_cld_climate[:,:,3])
-            opd_clmt = (we0*opd_cld_climate[:,:,0]+we1*opd_cld_climate[:,:,1]+we2*opd_cld_climate[:,:,2]+we3*opd_cld_climate[:,:,3])
-            g0_clmt = (we0*opd_cld_climate[:,:,0]*g0_cld_climate[:,:,0]+we1*opd_cld_climate[:,:,1]*g0_cld_climate[:,:,1]+we2*opd_cld_climate[:,:,2]*g0_cld_climate[:,:,2]+we3*opd_cld_climate[:,:,3]*g0_cld_climate[:,:,3])/(sum_opd_clmt)
-            w0_clmt = (we0*opd_cld_climate[:,:,0]*w0_cld_climate[:,:,0]+we1*opd_cld_climate[:,:,1]*w0_cld_climate[:,:,1]+we2*opd_cld_climate[:,:,2]*w0_cld_climate[:,:,2]+we3*opd_cld_climate[:,:,3]*w0_cld_climate[:,:,3])/(sum_opd_clmt)
-            g0_clmt = np.nan_to_num(g0_clmt,nan=0.0)
-            w0_clmt = np.nan_to_num(w0_clmt,nan=0.0)
-            opd_clmt[np.where(opd_clmt <= 1e-5)] = 0.0
-            
-            
-            df_cld = vj.picaso_format(opd_clmt, w0_clmt, g0_clmt)
-            bundle.clouds(df=df_cld)
-            #taudif = np.max(np.abs(opd_cld_climate[:,:,0]-opd_cld_climate[:,:,1]))
-            #taudif = np.max(np.abs((opd_cld_climate[:,:,0]-opd_cld_climate[:,:,1])/opd_cld_climate[:,:,1]))
-            #diff = (opd_cld_climate[:,:,0]-opd_cld_climate[:,:,1])/(0.5*(opd_cld_climate[:,:,0]+opd_cld_climate[:,:,1]))
-            #diff = np.nan_to_num(diff,nan=0.0)
-            #taudif = np.max(np.abs(diff))
-            #print("Max TAUCLD diff is", taudif, " Tau at layer 40 and wv 150 is ", opd_now[40,150])
-                    
-            DTAU, TAU, W0, COSB,ftau_cld, ftau_ray,GCOS2, DTAU_OG, TAU_OG, W0_OG, COSB_OG, \
-            W0_no_raman , surf_reflect, ubar0,ubar1,cos_theta, single_phase,multi_phase, \
-            frac_a,frac_b,frac_c,constant_back,constant_forward, tridiagonal , \
-            wno,nwno,ng,nt, nlevel, ngauss, gauss_wts, mmw =  calculate_atm(bundle, opacityclass)
-                
-            temp, dtdp, flag_converge, flux_net_ir_layer, flux_plus_ir_attop, all_profiles = t_start(nofczns,nstr,it_max,conv,x_max_mult, 
-            rfaci, rfacv, nlevel, temp, pressure, p_table, t_table, 
-            grad, cp, tidal,tmin,tmax,dwni, bb , y2, tp, DTAU, TAU, W0, COSB,ftau_cld, ftau_ray,GCOS2, DTAU_OG, TAU_OG, W0_OG, COSB_OG, W0_no_raman , surf_reflect, ubar0,ubar1,cos_theta, FOPI, single_phase,multi_phase,frac_a,frac_b,frac_c,constant_back,constant_forward, tridiagonal , wno,nwno,ng,nt, ngauss, gauss_wts, save_profile, all_profiles)
-                
-    
-     
-            ert = 0.0 # avg temp change
-            scalt= 1.0
-            dtx= abs(temp-temp_old)
-            ert = np.sum(dtx)
-            temp_old= np.copy(temp)   
-            ert = ert/(float(nlevel)*scalt)
-    '''
     
     if conv_flag == 0:
-        print("Not converged")
+        if verbose: print("Not converged")
     else :
-        print("Profile converged")
-    return pressure, temp, dtdp, conv_flag, all_profiles, opd_cld_climate,g0_cld_climate,w0_cld_climate,flux_net_ir_layer, flux_plus_ir_attop
+        if verbose: print("Profile converged after itmx hit")
+    return pressure, temp, dtdp, conv_flag, all_profiles, opd_cld_climate,g0_cld_climate,w0_cld_climate, cld_out,flux_net_ir_layer, flux_plus_ir_attop
 
-def find_strat(pressure, temp, dtdp , FOPI, nofczns,nstr,x_max_mult,
+def find_strat(mieff_dir, pressure, temp, dtdp , FOPI, nofczns,nstr,x_max_mult,
              t_table, p_table, grad, cp, opacityclass, grav, 
-             rfaci, rfacv, nlevel, tidal, tmin, tmax, dwni, bb , y2 , tp, cloudy, cld_species,mh,fsed,flag_hack, save_profile, all_profiles, opd_cld_climate,g0_cld_climate,w0_cld_climate,flux_net_ir_layer, flux_plus_ir_attop):
+             rfaci, rfacv, nlevel, tidal, tmin, tmax, dwni, bb , y2 , tp, 
+             cloudy, cld_species,mh,fsed,flag_hack, save_profile, all_profiles, 
+             opd_cld_climate,g0_cld_climate,w0_cld_climate,flux_net_ir_layer, 
+             flux_plus_ir_attop,verbose=1):
     """
     Function iterating on the TP profile by calling tstart and changing opacities as well
     Parameters
     ----------
+    mieff_dir: str
+        path to directory with mieff files for virga
     it_max : int
         Maximum iterations allowed in the inner no opa change loop
     itmx : int
         Maximum iterations allowed in the outer opa change loop
     conv : float
         
     convt: float
@@ -4985,15 +4842,17 @@
         Tidal Fluxes dimension = nlevel
     tmin : float
         Minimum allwed Temp in the profile
     tmax : float
         Maximum allowed Temp in the profile
     dwni : array
         Spectral interval corrections (dimension= nwvno)
-       
+    verbose: int 
+        If 0 nothing gets printed
+        If 1 this prints everything out 
         
     Returns
     -------
     array 
         Temperature array and lapse ratio array if converged
         else Temperature array twice
     """
@@ -5012,67 +4871,74 @@
     final = False
 
     grad_x, cp_x =convec(temp,pressure, t_table, p_table, grad, cp)
     # grad_x = 
     while dtdp[nstr[1]-1] >= subad*grad_x[nstr[1]-1] :
         ratio = dtdp[nstr[1]-1]/grad_x[nstr[1]-1]
 
-        if ratio > 2 :
-            print("Move up two levels")
+        if ratio > 1.8 :
+            if verbose: print("Move up two levels")
             ngrow = 2
             nstr = growup( 1, nstr , ngrow)
         else :
             ngrow = 1
             nstr = growup( 1, nstr , ngrow)
         
-        if nstr[1] < 6 :
+        if nstr[1] < 5 :
             raise ValueError( "Convection zone grew to Top of atmosphere, Need to Stop")
         
-        pressure, temp, dtdp, profile_flag, all_profiles, opd_cld_climate,g0_cld_climate,w0_cld_climate,flux_net_ir_layer, flux_plus_ir_attop = profile(it_max_strat, itmx_strat, conv_strat, convt_strat, nofczns,nstr,x_max_mult,
-            temp,pressure, FOPI, t_table, p_table, grad, cp, opacityclass, grav, 
-             rfaci, rfacv, nlevel, tidal, tmin, tmax, dwni, bb , y2 , tp, final, cloudy, cld_species, mh,fsed,flag_hack, save_profile, all_profiles, opd_cld_climate,g0_cld_climate,w0_cld_climate,flux_net_ir_layer, flux_plus_ir_attop)
+        pressure, temp, dtdp, profile_flag, all_profiles, opd_cld_climate,g0_cld_climate,w0_cld_climate, cld_out, flux_net_ir_layer, flux_plus_ir_attop = profile(mieff_dir, it_max_strat, itmx_strat, conv_strat, convt_strat, nofczns,nstr,x_max_mult,
+                            temp,pressure, FOPI, t_table, p_table, grad, cp, opacityclass, grav, 
+                             rfaci, rfacv, nlevel, tidal, tmin, tmax, dwni, bb , y2 , tp, final, 
+                             cloudy, cld_species, mh,fsed,flag_hack, save_profile, all_profiles, 
+                             opd_cld_climate,g0_cld_climate,w0_cld_climate,flux_net_ir_layer, 
+                             flux_plus_ir_attop, verbose=verbose)
 
     # now for the 2nd convection zone
     dt_max = 0.0 #DTMAX
     i_max = 0 #IMAX
     # -1 in ifirst to include ifirst index
     flag_super = 0
     for i in range(nstr[1]-1, ifirst-1, -1):
         add = dtdp[i] - grad_x[i]
-        if add/grad_x[i] >= 0.02 : # non-neglegible super-adiabaticity
+        if add > dt_max and add/grad_x[i] >= 0.02 : # non-neglegible super-adiabaticity
+            dt_max = add
             i_max =i
             break
     
     flag_final_convergence =0
-    if i_max == 0: # no superadiabaticity, we are done
+    if i_max == 0 or dt_max/grad_x[i_max] < 0.02: # no superadiabaticity, we are done
         flag_final_convergence = 1
 
     if flag_final_convergence  == 0:
-        print(" convection zone status")
-        print(nstr[0],nstr[1],nstr[2],nstr[3],nstr[4],nstr[5])
-        print(nofczns)
+        if verbose: print(" convection zone status")
+        if verbose: print(nstr[0],nstr[1],nstr[2],nstr[3],nstr[4],nstr[5])
+        if verbose: print(nofczns)
 
         nofczns = 2
         nstr[4]= nstr[1]
         nstr[5]= nstr[2]
         nstr[1]= i_max
         nstr[2] = i_max
-        nstr[3] = i_max
-        print(nstr)
+        nstr[3] = i_max #+ 1
+        if verbose: print(nstr)
         if nstr[3] >= nstr[4] :
             #print(nstr[0],nstr[1],nstr[2],nstr[3],nstr[4],nstr[5])
             #print(nofczns)
             raise ValueError("Overlap happened !")
-        pressure, temp, dtdp, profile_flag, all_profiles, opd_cld_climate,g0_cld_climate,w0_cld_climate,flux_net_ir_layer, flux_plus_ir_attop = profile(it_max_strat, itmx_strat, conv_strat, convt_strat, nofczns,nstr,x_max_mult,
+        pressure, temp, dtdp, profile_flag, all_profiles, opd_cld_climate,g0_cld_climate,w0_cld_climate,cld_out,flux_net_ir_layer, flux_plus_ir_attop = profile(mieff_dir, it_max_strat, itmx_strat, conv_strat, convt_strat, nofczns,nstr,x_max_mult,
             temp,pressure, FOPI, t_table, p_table, grad, cp, opacityclass, grav, 
-             rfaci, rfacv, nlevel, tidal, tmin, tmax, dwni, bb , y2 , tp, final, cloudy, cld_species,mh, fsed,flag_hack,save_profile, all_profiles,opd_cld_climate,g0_cld_climate,w0_cld_climate,flux_net_ir_layer, flux_plus_ir_attop)
+             rfaci, rfacv, nlevel, tidal, tmin, tmax, dwni, bb , y2 , tp, final, 
+             cloudy, cld_species,mh, fsed,flag_hack,save_profile, all_profiles,
+             opd_cld_climate,g0_cld_climate,w0_cld_climate,flux_net_ir_layer, 
+             flux_plus_ir_attop, verbose=verbose)
 
         i_change = 1
         while i_change == 1 :
-            print("Grow Phase : Upper Zone")
+            if verbose: print("Grow Phase : Upper Zone")
             i_change = 0
 
             d1 = dtdp[nstr[1]-1]
             d2 = dtdp[nstr[3]]
             c1 = grad_x[nstr[1]-1]
             c2 = grad_x[nstr[3]]
 
@@ -5089,131 +4955,127 @@
                     nstr = growdown( 1, nstr , ngrow)
 
                     if nstr[2] == nstr[4]: # one conv zone
                         nofczns =1
                         nstr[2] = nstr[5]
                         nstr[3] = 0
                         i_change = 1
-                print(nstr)
-                pressure, temp, dtdp, profile_flag, all_profiles,opd_cld_climate,g0_cld_climate,w0_cld_climate,flux_net_ir_layer, flux_plus_ir_attop = profile(it_max_strat, itmx_strat, conv_strat, convt_strat, nofczns,nstr,x_max_mult,
-            temp,pressure, FOPI, t_table, p_table, grad, cp, opacityclass, grav, 
-             rfaci, rfacv, nlevel, tidal, tmin, tmax, dwni, bb , y2 , tp, final, cloudy, cld_species, mh,fsed,flag_hack,save_profile, all_profiles,opd_cld_climate,g0_cld_climate,w0_cld_climate,flux_net_ir_layer, flux_plus_ir_attop)
+                if verbose: print(nstr)
+                pressure, temp, dtdp, profile_flag, all_profiles,opd_cld_climate,g0_cld_climate,w0_cld_climate,cld_out,flux_net_ir_layer, flux_plus_ir_attop = profile(mieff_dir, it_max_strat, itmx_strat, conv_strat, convt_strat, nofczns,nstr,x_max_mult,
+                                temp,pressure, FOPI, t_table, p_table, grad, cp, opacityclass, grav, 
+                                 rfaci, rfacv, nlevel, tidal, tmin, tmax, dwni, bb , y2 , tp, final, 
+                                 cloudy, cld_species, mh,fsed,flag_hack,save_profile, all_profiles,
+                                 opd_cld_climate,g0_cld_climate,w0_cld_climate,flux_net_ir_layer, 
+                                 flux_plus_ir_attop, verbose=verbose)
 
                 d1 = dtdp[nstr[1]-1]
                 d2 = dtdp[nstr[3]]
                 c1 = grad_x[nstr[1]-1]
                 c2 = grad_x[nstr[3]]
             #Now grow the lower zone.
-            while ((dtdp[nstr[4]-1] >= subad*grad_x[nstr[5]-1]) and nofczns > 1):
+            while ((dtdp[nstr[4]-1] >= subad*grad_x[nstr[4]-1]) and nofczns > 1):
                 
                 ngrow = 1
                 nstr = growup( 2, nstr , ngrow)
                 #Now check to see if two zones have merged and stop further searching if so.
                 if nstr[2] == nstr[4] :
                     nofczns = 1
                     nstr[2] = nstr[5]
                     nstr[3] = 0
                     i_change =1
-                print(nstr)
-                pressure, temp, dtdp, profile_flag, all_profiles,opd_cld_climate,g0_cld_climate,w0_cld_climate,flux_net_ir_layer, flux_plus_ir_attop = profile(it_max_strat, itmx_strat, conv_strat, convt_strat, nofczns,nstr,x_max_mult,
+                if verbose: print(nstr)
+                pressure, temp, dtdp, profile_flag, all_profiles,opd_cld_climate,g0_cld_climate,w0_cld_climate,cld_out,flux_net_ir_layer, flux_plus_ir_attop = profile(mieff_dir, it_max_strat, itmx_strat, conv_strat, convt_strat, nofczns,nstr,x_max_mult,
                     temp,pressure, FOPI, t_table, p_table, grad, cp, opacityclass, grav, 
-                    rfaci, rfacv, nlevel, tidal, tmin, tmax, dwni, bb , y2 , tp, final, cloudy, cld_species, mh,fsed,flag_hack,save_profile, all_profiles,opd_cld_climate,g0_cld_climate,w0_cld_climate,flux_net_ir_layer, flux_plus_ir_attop)
+                    rfaci, rfacv, nlevel, tidal, tmin, tmax, dwni, bb , y2 , tp, final, 
+                    cloudy, cld_species, mh,fsed,flag_hack,save_profile, all_profiles,
+                    opd_cld_climate,g0_cld_climate,w0_cld_climate,flux_net_ir_layer, 
+                    flux_plus_ir_attop, verbose=verbose)
             
 
             flag_final_convergence = 1
         
     itmx_strat =6
     it_max_strat = 10
     convt_strat = 2.0
     convt_strat = 2.0
-    x_max_mult = 2.0
+    x_max_mult = x_max_mult/2.0
     ip2 = -10
 
     final = True
-    print("final",nstr)
-    pressure, temp, dtdp, profile_flag, all_profiles,opd_cld_climate,g0_cld_climate,w0_cld_climate,flux_net_ir_layer, flux_plus_ir_attop = profile(it_max_strat, itmx_strat, conv_strat, convt_strat, nofczns,nstr,x_max_mult,
+    if verbose: print("final",nstr)
+    pressure, temp, dtdp, profile_flag, all_profiles,opd_cld_climate,g0_cld_climate,w0_cld_climate,cld_out,flux_net_ir_layer, flux_plus_ir_attop = profile(mieff_dir, it_max_strat, itmx_strat, conv_strat, convt_strat, nofczns,nstr,x_max_mult,
                 temp,pressure, FOPI, t_table, p_table, grad, cp,opacityclass, grav, 
-                rfaci, rfacv, nlevel, tidal, tmin, tmax, dwni, bb , y2 , tp, final, cloudy, cld_species,mh,fsed,flag_hack,save_profile, all_profiles,opd_cld_climate,g0_cld_climate,w0_cld_climate,flux_net_ir_layer, flux_plus_ir_attop)
+                rfaci, rfacv, nlevel, tidal, tmin, tmax, dwni, bb , y2 , tp, final, 
+                cloudy, cld_species,mh,fsed,flag_hack,save_profile, all_profiles,
+                opd_cld_climate,g0_cld_climate,w0_cld_climate,flux_net_ir_layer, 
+                flux_plus_ir_attop, verbose=verbose)
 
     #    else :
     #        raise ValueError("Some problem here with goto 125")
         
     if profile_flag == 0:
-        print("ENDING WITHOUT CONVERGING")
+        if verbose: print("ENDING WITHOUT CONVERGING")
     elif profile_flag == 1:
-        print("YAY ! ENDING WITH CONVERGENCE")
+        if verbose: print("YAY ! ENDING WITH CONVERGENCE")
         
     bundle = inputs(calculation='brown')
     bundle.phase_angle(0)
     bundle.gravity(gravity=grav , gravity_unit=u.Unit('m/s**2'))
     bundle.add_pt( temp, pressure)
     
     bundle.premix_atmosphere(opacityclass, df = bundle.inputs['atmosphere']['profile'].loc[:,['pressure','temperature']])
 
     if cloudy == 1:
-        DTAU, TAU, W0, COSB,ftau_cld, ftau_ray,GCOS2, DTAU_OG, TAU_OG, W0_OG, COSB_OG, W0_no_raman , surf_reflect, ubar0,ubar1,cos_theta, single_phase,multi_phase,frac_a,frac_b,frac_c,constant_back,constant_forward, tridiagonal , wno,nwno,ng,nt, nlevel, ngauss, gauss_wts, mmw =  calculate_atm(bundle, opacityclass)
+        DTAU, TAU, W0, COSB,ftau_cld, ftau_ray,GCOS2, DTAU_OG, TAU_OG, W0_OG, COSB_OG, W0_no_raman , surf_reflect, ubar0,ubar1,cos_theta, single_phase,multi_phase,frac_a,frac_b,frac_c,constant_back,constant_forward, wno,nwno,ng,nt, nlevel, ngauss, gauss_wts, mmw,gweight,tweight  =  calculate_atm(bundle, opacityclass)
 
         metallicity = 10**(mh) #atmospheric metallicity relative to Solar
         mean_molecular_weight = np.mean(mmw) # atmospheric mean molecular weight
-        directory ='/Users/sagnickmukherjee/Documents/GitHub/virga/refr_new'
+        # directory ='/Users/sagnickmukherjee/Documents/GitHub/virga/refr_new'
+        # directory = '/home/jjm6243/dev_virga/'
+        directory = mieff_dir
+
         calc_type =0
         kzz  = get_kzz(pressure, temp,grav,mmw,tidal,flux_net_ir_layer, flux_plus_ir_attop,t_table, p_table, grad, cp, calc_type,nstr)
         bundle.inputs['atmosphere']['profile']['kz'] = kzz
 
 
         cld_out = bundle.virga(cld_species,directory, fsed=fsed,mh=metallicity,
-                        mmw = mean_molecular_weight,full_output=False,climate=True)
+                        mmw = mean_molecular_weight) #,climate=True)
         
-        opd_now, w0_now, g0_now = cld_out
-        df_cld = vj.picaso_format(opd_now, w0_now, g0_now)
-        bundle.clouds(df=df_cld)  
+        opd_now, w0_now, g0_now = cld_out['opd_per_layer'],cld_out['single_scattering'],cld_out['asymmetry']
+        df_cld = vj.picaso_format(opd_now, w0_now, g0_now,pressure = cld_out['pressure'], wavenumber= 1e4/cld_out['wave'])
+        bundle.clouds(df=df_cld)
     else:
         opd_now,w0_now,g0_now = 0,0,0
+        cld_out = 0
 
-    DTAU, TAU, W0, COSB,ftau_cld, ftau_ray,GCOS2, DTAU_OG, TAU_OG, W0_OG, COSB_OG, W0_no_raman , surf_reflect, ubar0,ubar1,cos_theta, single_phase,multi_phase,frac_a,frac_b,frac_c,constant_back,constant_forward, tridiagonal , wno,nwno,ng,nt, nlevel, ngauss, gauss_wts, mmw =  calculate_atm(bundle, opacityclass)
+    DTAU, TAU, W0, COSB,ftau_cld, ftau_ray,GCOS2, DTAU_OG, TAU_OG, W0_OG, COSB_OG, W0_no_raman , surf_reflect, ubar0,ubar1,cos_theta, single_phase,multi_phase,frac_a,frac_b,frac_c,constant_back,constant_forward,  wno,nwno,ng,nt, nlevel, ngauss, gauss_wts, mmw,gweight,tweight  =  calculate_atm(bundle, opacityclass)
     
-    flux_net_v_layer_full, flux_net_v_full, flux_plus_v_full, flux_minus_v_full , flux_net_ir_layer_full, flux_net_ir_full, flux_plus_ir_full, flux_minus_ir_full = climate(pressure, temp, dwni, bb , y2, tp, tmin, tmax, DTAU, TAU, W0, 
+    flux_net_v_layer_full, flux_net_v_full, flux_plus_v_full, flux_minus_v_full , flux_net_ir_layer_full, flux_net_ir_full, flux_plus_ir_full, flux_minus_ir_full = get_fluxes(pressure, temp, dwni, bb , y2, tp, tmin, tmax, DTAU, TAU, W0, 
             COSB,ftau_cld, ftau_ray,GCOS2, DTAU_OG, TAU_OG, W0_OG, COSB_OG, W0_no_raman , surf_reflect, 
-            ubar0,ubar1,cos_theta, FOPI, single_phase,multi_phase,frac_a,frac_b,frac_c,constant_back,constant_forward, tridiagonal , 
-            wno,nwno,ng,nt, nlevel, ngauss, gauss_wts, False, True) #false for reflected, true for thermal
+            ubar0,ubar1,cos_theta, FOPI, single_phase,multi_phase,frac_a,frac_b,frac_c,constant_back,constant_forward,
+            wno,nwno,ng,nt,gweight,tweight, nlevel, ngauss, gauss_wts, False, True) #false for reflected, true for thermal
 
       
     
-    return pressure, temp, dtdp, nstr , flux_plus_ir_full, bundle.inputs['atmosphere']['profile'], all_profiles,opd_now,w0_now,g0_now
+    return pressure, temp, dtdp, nstr , flux_plus_ir_full, bundle.inputs['atmosphere']['profile'], all_profiles, cld_out,profile_flag
 
-@jit(nopython=True, cache=True)
-def correct_profile(temp,pressure,wh,min_temp):
-    '''
-    indices = wh[0]
-    for i in range(len(indices)):
-        if indices[i] == 0:
-            temp[indices[i]] = min_temp+0.5
-        elif (temp[indices[i]-1] > min_temp) and (temp[indices[i]+1]) > min_temp :
-            temp_prev = temp[indices[i]-1]
-            temp_next = temp[indices[i]+1]
-            press_prev = pressure[indices[i]-1]
-            press_next = pressure[indices[i]+1]
-            dtdlnp = (temp_next-temp_prev)/np.log(press_next/press_prev)
-            temp[indices[i]] = temp_prev +np.log(pressure[indices[i]]/press_prev)*dtdlnp
-        else :
-            temp[indices[i]] = min_temp+0.5
-            temp[indices[i]-1] = min_temp+0.5
-            temp[indices[i]+1] = min_temp + 0.5
-    '''
-
-
-    return temp
-
-def profile_deq(it_max, itmx, conv, convt, nofczns,nstr,x_max_mult,
+def profile_deq(mieff_dir, it_max, itmx, conv, convt, nofczns,nstr,x_max_mult,
             temp,pressure,FOPI, t_table, p_table, grad, cp, opacityclass, grav, 
-             rfaci, rfacv, nlevel, tidal, tmin, tmax, dwni, bb , y2 , tp, final, cloudy, cld_species,mh,fsed,flag_hack,quench_levels,kz,mmw, save_profile, all_profiles,self_consistent_kzz,save_kzz,all_kzz, vulcan_run,opd_cld_climate,g0_cld_climate,w0_cld_climate,flux_net_ir_layer, flux_plus_ir_attop,on_fly=False,gases_fly=None ):
+             rfaci, rfacv, nlevel, tidal, tmin, tmax, dwni, bb , y2 , tp, final, 
+             cloudy, cld_species,mh,fsed,flag_hack,quench_levels,kz,mmw, save_profile,
+              all_profiles,self_consistent_kzz,save_kzz,all_kzz, opd_cld_climate,
+              g0_cld_climate,w0_cld_climate,flux_net_ir_layer, flux_plus_ir_attop,
+              photo_inputs_dict=None,on_fly=False,gases_fly=None,verbose=True ):
     """
     Function iterating on the TP profile by calling tstart and changing opacities as well
     Parameters
     ----------
+    mieff_dir: str
+        path to directory with mieff files for virga
     it_max : int
         Maximum iterations allowed in the inner no opa change loop
     itmx : int
         Maximum iterations allowed in the outer opa change loop
     conv : float
         
     convt: float
@@ -5266,22 +5128,28 @@
         Tidal Fluxes dimension = nlevel
     tmin : float
         Minimum allwed Temp in the profile
     tmax : float
         Maximum allowed Temp in the profile
     dwni : array
         Spectral interval corrections (dimension= nwvno)   
-        
+    verbose : bool 
+        If True, prints out messages 
     Returns
     -------
     array 
         Temperature array and lapse ratio array if converged
         else Temperature array twice
     """
 
+    #permanently turn of ref light for cases where rfacv is zero 
+    #turn off reflected light permanently for all these runs if rfacv=0 
+    if rfacv==0:compute_reflected=False
+    else:compute_reflected=True
+
     # taudif is fixed to be 0 here since it is needed only for clouds
     taudif = 0.0
     taudif_tol = 0.1
     
     # first calculate the convective zones
     for nb in range(0,3*nofczns,3):
         
@@ -5309,72 +5177,97 @@
 
     
     bundle = inputs(calculation='brown')
     bundle.phase_angle(0)
     bundle.gravity(gravity=grav , gravity_unit=u.Unit('m/s**2'))
     bundle.add_pt( temp, pressure)
     #### to get the last Kzz in the calculation
-    k_b = 1.38e-23 # boltzmann constant
-    m_p = 1.66e-27 # proton mass
     
-    if len(mmw) < len(temp):
-        mmw = np.append(mmw,mmw[-1])
-    con  = k_b/(mmw*m_p)
 
-    scale_H = con * temp*1e2/(grav)
+    if photo_inputs_dict['yesorno'] == False:
+        k_b = 1.38e-23 # boltzmann constant
+        m_p = 1.66e-27 # proton mass
+        
+        if len(mmw) < len(temp):
+            mmw = np.append(mmw,mmw[-1])
+        con  = k_b/(mmw*m_p)
 
-    kz = scale_H**2/all_kzz[-len(temp):] ## level mixing timescales
+        scale_H = con * temp*1e2/(grav)
 
-    if vulcan_run == False:
+        kz = scale_H**2/all_kzz[-len(temp):] ## level mixing timescales
         quench_levels, t_mix = quench_level(pressure, temp, kz ,mmw, grav, return_mix_timescale=True)
-        
+        if save_kzz == 1:
+            all_kzz = np.append(all_kzz,t_mix)
         qvmrs, qvmrs2 = bundle.premix_atmosphere_diseq(opacityclass, quench_levels=quench_levels, df = bundle.inputs['atmosphere']['profile'].loc[:,['pressure','temperature']],t_mix=t_mix)
     else :
         bundle.premix_atmosphere(opacityclass, df = bundle.inputs['atmosphere']['profile'].loc[:,['pressure','temperature']])
-        t_mix = bundle.run_vulcan(pressure,temp,kz,grav,mmw, first = False)
+        pc= bundle.call_photochem(temp,pressure,photo_inputs_dict['mh'],photo_inputs_dict['CtoO'],photo_inputs_dict['psurf'],photo_inputs_dict['m_planet'],photo_inputs_dict['r_planet'],photo_inputs_dict['kz'],tstop=photo_inputs_dict['tstop'],filename = photo_inputs_dict['photochem_file'],stfilename =photo_inputs_dict['photochem_stfile'],network = photo_inputs_dict['photochem_network'],network_ct=photo_inputs_dict['photochem_networkct'],first=False,pc=photo_inputs_dict['pc'])
+        photo_inputs_dict['pc'] = pc
+        all_kzz = np.append(all_kzz, kz)
+        quench_levels = np.array([0,0,0,0])
+        photo_inputs_dict['pc'] = pc
+        qvmrs, qvmrs2=0,0
     
     #if save_profile == 1:
     #        all_profiles = np.append(all_profiles,bundle.inputs['atmosphere']['profile']['NH3'].values)
     # no flux calculation yet so no cloud calculation needed
     #if cloudy == 1 :
     #    metallicity = mh #atmospheric metallicity relative to Solar
     #    mean_molecular_weight = 2.2 # atmospheric mean molecular weight
     #    directory ='/Users/sagnickmukherjee/Documents/software/optics'
     #    bundle.inputs['atmosphere']['profile']['kz'] = 1e5 + np.zeros_like(temp) # start with kzmin
     #    
     
     #    bundle.virga(cld_species,directory, fsed=fsed,mh=metallicity,
     #    mmw = mean_molecular_weight,full_output=False)
-    if save_kzz == 1:
-        all_kzz = np.append(all_kzz,t_mix)
+    
 
     if cloudy == 1 :
             
 
             we0,we1,we2,we3 = 0.25,0.25,0.25,0.25
             opd_prev_cld_step = (we0*opd_cld_climate[:,:,0]+we1*opd_cld_climate[:,:,1]+we2*opd_cld_climate[:,:,2]+we3*opd_cld_climate[:,:,3]) # last average
             
             metallicity = 10**(0) #atmospheric metallicity relative to Solar
             mean_molecular_weight = np.mean(mmw) # atmospheric mean molecular weight
-            directory ='/Users/sagnickmukherjee/Documents/GitHub/virga/refr_new661'
-            
+            # directory ='/Users/sagnickmukherjee/Documents/GitHub/virga/refr_new661'
+            # directory = '/home/jjm6243/dev_virga/'
+            directory = mieff_dir
+
             kzz  = get_kzz(pressure, temp,grav,mmw,tidal,flux_net_ir_layer, flux_plus_ir_attop,t_table, p_table, grad, cp, calc_type,nstr)
             bundle.inputs['atmosphere']['profile']['kz'] = kzz
-        
+            photo_inputs_dict['kz'] = kzz
 
             cld_out = bundle.virga(cld_species,directory, fsed=fsed,mh=metallicity,
-                        mmw = mean_molecular_weight,full_output=False,climate=True)
+                        mmw = mean_molecular_weight)#,climate=True)
             
-            opd_now, w0_now, g0_now = cld_out
+            opd_now, w0_now, g0_now = cld_out['opd_per_layer'],cld_out['single_scattering'],cld_out['asymmetry']
             
             opd_cld_climate[:,:,3], g0_cld_climate[:,:,3], w0_cld_climate[:,:,3] = opd_cld_climate[:,:,2], g0_cld_climate[:,:,2], w0_cld_climate[:,:,2]
             opd_cld_climate[:,:,2], g0_cld_climate[:,:,2], w0_cld_climate[:,:,2] = opd_cld_climate[:,:,1], g0_cld_climate[:,:,1], w0_cld_climate[:,:,1]
             opd_cld_climate[:,:,1], g0_cld_climate[:,:,1], w0_cld_climate[:,:,1] = opd_cld_climate[:,:,0], g0_cld_climate[:,:,0], w0_cld_climate[:,:,0]
-                        
-            opd_cld_climate[:,:,0], g0_cld_climate[:,:,0], w0_cld_climate[:,:,0] = opd_now, g0_now, w0_now
+           
+            # convert cld_out output to 661 grid similar to initiate_cld_matrices (JM)
+            wv196 = cld_out['wave']
+            wv661 = 1e4/opacityclass.wno[::-1] # flip to match the order of wv196 from virga
+
+            opd_now_661 =  np.zeros(shape=(len(opd_now[:,0]),len(wv661)))
+            g0_now_661,w0_now_661 = np.zeros_like(opd_now_661),np.zeros_like(opd_now_661)
+
+            for ilayer in range(len(opd_now[:,0])):
+                fopd = interp1d(wv196,opd_now[ilayer,:] , kind='cubic',fill_value="extrapolate")
+                fg0 = interp1d(wv196,g0_now[ilayer,:] , kind='cubic',fill_value="extrapolate")
+                fw0 = interp1d(wv196,w0_now[ilayer,:] , kind='cubic',fill_value="extrapolate")
+
+                opd_now_661[ilayer,:] = fopd(wv661)
+                g0_now_661[ilayer,:] = fg0(wv661)
+                w0_now_661[ilayer,:] = fw0(wv661)
+
+            opd_cld_climate[:,:,0], g0_cld_climate[:,:,0], w0_cld_climate[:,:,0] = opd_now_661, g0_now_661, w0_now_661                         
+            # opd_cld_climate[:,:,0], g0_cld_climate[:,:,0], w0_cld_climate[:,:,0] = opd_now, g0_now, w0_now
             
             #if np.sum(opd_cld_climate[:,:,1]) == 0 :
             #    w0,w1,w2,w3 = 1,0,0,0
             #elif (np.sum(opd_cld_climate[:,:,1]) != 0) and (np.sum(opd_cld_climate[:,:,2]) == 0):
             #    w0,w1,w2,w3 = 0.5,0.5,0,0
             #elif (np.sum(opd_cld_climate[:,:,2]) != 0) and (np.sum(opd_cld_climate[:,:,3]) == 0):
             #    w0,w1,w2,w3 = 0.33,0.33,0.33,0
@@ -5388,44 +5281,45 @@
             g0_clmt = (we0*opd_cld_climate[:,:,0]*g0_cld_climate[:,:,0]+we1*opd_cld_climate[:,:,1]*g0_cld_climate[:,:,1]+we2*opd_cld_climate[:,:,2]*g0_cld_climate[:,:,2]+we3*opd_cld_climate[:,:,3]*g0_cld_climate[:,:,3])/(sum_opd_clmt)
             w0_clmt = (we0*opd_cld_climate[:,:,0]*w0_cld_climate[:,:,0]+we1*opd_cld_climate[:,:,1]*w0_cld_climate[:,:,1]+we2*opd_cld_climate[:,:,2]*w0_cld_climate[:,:,2]+we3*opd_cld_climate[:,:,3]*w0_cld_climate[:,:,3])/(sum_opd_clmt)
             g0_clmt = np.nan_to_num(g0_clmt,nan=0.0)
             w0_clmt = np.nan_to_num(w0_clmt,nan=0.0)
             opd_clmt[np.where(opd_clmt <= 1e-5)] = 0.0
             
             
-            df_cld = vj.picaso_format(opd_clmt, w0_clmt, g0_clmt)
+            df_cld = vj.picaso_format(opd_clmt, w0_clmt, g0_clmt,pressure = cld_out['pressure'], wavenumber= wv661)
             bundle.clouds(df=df_cld)
 
     DTAU, TAU, W0, COSB,ftau_cld, ftau_ray,GCOS2, DTAU_OG, TAU_OG, W0_OG, COSB_OG, \
         W0_no_raman , surf_reflect, ubar0,ubar1,cos_theta, single_phase,multi_phase, \
-        frac_a,frac_b,frac_c,constant_back,constant_forward, tridiagonal , \
-        wno,nwno,ng,nt, nlevel, ngauss, gauss_wts, mmw =  calculate_atm_deq(bundle, opacityclass,on_fly=on_fly,gases_fly=gases_fly)
+        frac_a,frac_b,frac_c,constant_back,constant_forward, \
+        wno,nwno,ng,nt, nlevel, ngauss, gauss_wts, mmw,gweight,tweight =  calculate_atm_deq(bundle, opacityclass,on_fly=on_fly,gases_fly=gases_fly)
     if self_consistent_kzz == True :
                 
-        flux_net_v_layer_full, flux_net_v_full, flux_plus_v_full, flux_minus_v_full , flux_net_ir_layer_full, flux_net_ir_full, flux_plus_ir_full, flux_minus_ir_full = climate(pressure, temp, dwni, bb , y2, tp, tmin, tmax, DTAU, TAU, W0, 
+        flux_net_v_layer_full, flux_net_v_full, flux_plus_v_full, flux_minus_v_full , flux_net_ir_layer_full, flux_net_ir_full, flux_plus_ir_full, flux_minus_ir_full = get_fluxes(pressure, temp, dwni, bb , y2, tp, tmin, tmax, DTAU, TAU, W0, 
         COSB,ftau_cld, ftau_ray,GCOS2, DTAU_OG, TAU_OG, W0_OG, COSB_OG, W0_no_raman , surf_reflect, 
-        ubar0,ubar1,cos_theta, FOPI, single_phase,multi_phase,frac_a,frac_b,frac_c,constant_back,constant_forward, tridiagonal , 
-        wno,nwno,ng,nt, nlevel, ngauss, gauss_wts,True, True)#True for reflected, True for thermal
+        ubar0,ubar1,cos_theta, FOPI, single_phase,multi_phase,frac_a,frac_b,frac_c,constant_back,constant_forward, 
+        wno,nwno,ng,nt, gweight,tweight,nlevel, ngauss, gauss_wts,compute_reflected, True)#True for reflected, True for thermal
 
         flux_net_ir_layer = flux_net_ir_layer_full[:]
         flux_plus_ir_attop = flux_plus_ir_full[0,:] 
         calc_type = 0
     
         kz = get_kzz(pressure, temp,grav,mmw,tidal,flux_net_ir_layer, flux_plus_ir_attop,t_table, p_table, grad, cp, calc_type,nstr)
-    
+        photo_inputs_dict['kz'] = kz
     ## begin bigger loop which gets opacities
     for iii in range(itmx):
         
         temp, dtdp, flag_converge, flux_net_ir_layer, flux_plus_ir_attop, all_profiles = t_start(nofczns,nstr,it_max,conv,x_max_mult, 
             rfaci, rfacv, nlevel, temp, pressure, p_table, t_table, 
             grad, cp, tidal,tmin,tmax,dwni, bb , y2, tp, DTAU, TAU, W0, 
             COSB,ftau_cld, ftau_ray,GCOS2, DTAU_OG, TAU_OG, W0_OG, COSB_OG, 
             W0_no_raman , surf_reflect, ubar0,ubar1,cos_theta, FOPI, 
             single_phase,multi_phase,frac_a,frac_b,frac_c,constant_back,constant_forward, 
-            tridiagonal , wno,nwno,ng,nt, ngauss, gauss_wts, save_profile, all_profiles)
+            wno,nwno,ng,nt,gweight,tweight, ngauss, gauss_wts, save_profile, all_profiles,
+            verbose=verbose)
         '''
         if (temp <= min(opacityclass.cia_temps)).any():
             wh = np.where(temp <= min(opacityclass.cia_temps))
             if len(wh[0]) <= 30 :
                 print(len(wh[0])," points went off the opacity grid. Correcting those.")
                 temp = correct_profile(temp,pressure,wh,min(opacityclass.cia_temps))
             else :
@@ -5433,50 +5327,75 @@
        '''
         
         
         bundle = inputs(calculation='brown')
         bundle.phase_angle(0)
         bundle.gravity(gravity=grav , gravity_unit=u.Unit('m/s**2'))
         bundle.add_pt( temp, pressure)
-        if vulcan_run == False:
+        if photo_inputs_dict['yesorno'] == False:
             quench_levels, t_mix = quench_level(pressure, temp, kz ,mmw, grav, return_mix_timescale=True)
             
             qvmrs, qvmrs2 = bundle.premix_atmosphere_diseq(opacityclass, quench_levels=quench_levels, df = bundle.inputs['atmosphere']['profile'].loc[:,['pressure','temperature']],t_mix=t_mix)
             print("Quench Levels are CO, CO2, NH3, HCN ", quench_levels)
         else :
             bundle.premix_atmosphere(opacityclass, df = bundle.inputs['atmosphere']['profile'].loc[:,['pressure','temperature']])
-            t_mix = bundle.run_vulcan(pressure,temp,kz,grav,mmw, first = False)
-            qvmrs, qvmrs2 = 0,0
+            pc= bundle.call_photochem(temp,pressure,photo_inputs_dict['mh'],photo_inputs_dict['CtoO'],photo_inputs_dict['psurf'],photo_inputs_dict['m_planet'],photo_inputs_dict['r_planet'],photo_inputs_dict['kz'],tstop=photo_inputs_dict['tstop'],filename = photo_inputs_dict['photochem_file'],stfilename =photo_inputs_dict['photochem_stfile'],network = photo_inputs_dict['photochem_network'],network_ct=photo_inputs_dict['photochem_networkct'],first=False,pc=photo_inputs_dict['pc'])
+            photo_inputs_dict['pc'] = pc
+            all_kzz = np.append(all_kzz, kz)
+            quench_levels = np.array([0,0,0,0])
+            photo_inputs_dict['pc'] = pc
+            qvmrs, qvmrs2=0,0
+            photo_inputs_dict['kz'] = kz
         
     
         #if save_profile == 1:
         #    all_profiles = np.append(all_profiles,bundle.inputs['atmosphere']['profile']['NH3'].values)
         
         if cloudy == 1 :
             we0,we1,we2,we3 = 0.25,0.25,0.25,0.25
             opd_prev_cld_step = (we0*opd_cld_climate[:,:,0]+we1*opd_cld_climate[:,:,1]+we2*opd_cld_climate[:,:,2]+we3*opd_cld_climate[:,:,3]) # last average
             
             metallicity = 10**(0) #atmospheric metallicity relative to Solar
             mean_molecular_weight = np.mean(mmw) # atmospheric mean molecular weight
-            directory ='/Users/sagnickmukherjee/Documents/GitHub/virga/refr_new661'
-            
+            # directory ='/Users/sagnickmukherjee/Documents/GitHub/virga/refr_new661'
+            # directory = '/home/jjm6243/dev_virga/'
+            directory = mieff_dir
+
             kzz  = get_kzz(pressure, temp,grav,mmw,tidal,flux_net_ir_layer, flux_plus_ir_attop,t_table, p_table, grad, cp, calc_type,nstr)
             bundle.inputs['atmosphere']['profile']['kz'] = kzz
+            photo_inputs_dict['kz'] =kzz
         
     
             cld_out = bundle.virga(cld_species,directory, fsed=fsed,mh=metallicity,
-                        mmw = mean_molecular_weight,full_output=False,climate=True)
+                        mmw = mean_molecular_weight)#,climate=True)
             
-            opd_now, w0_now, g0_now = cld_out
+            opd_now, w0_now, g0_now = cld_out['opd_per_layer'],cld_out['single_scattering'],cld_out['asymmetry']
             
             opd_cld_climate[:,:,3], g0_cld_climate[:,:,3], w0_cld_climate[:,:,3] = opd_cld_climate[:,:,2], g0_cld_climate[:,:,2], w0_cld_climate[:,:,2]
             opd_cld_climate[:,:,2], g0_cld_climate[:,:,2], w0_cld_climate[:,:,2] = opd_cld_climate[:,:,1], g0_cld_climate[:,:,1], w0_cld_climate[:,:,1]
             opd_cld_climate[:,:,1], g0_cld_climate[:,:,1], w0_cld_climate[:,:,1] = opd_cld_climate[:,:,0], g0_cld_climate[:,:,0], w0_cld_climate[:,:,0]
-                        
-            opd_cld_climate[:,:,0], g0_cld_climate[:,:,0], w0_cld_climate[:,:,0] = opd_now, g0_now, w0_now
+            
+            # convert cld_out output to 661 grid similar to initiate_cld_matrices (JM)
+            wv196 = cld_out['wave']
+            wv661 = 1e4/opacityclass.wno[::-1] # flip to match the order of wv196 from virga
+
+            opd_now_661 =  np.zeros(shape=(len(opd_now[:,0]),len(wv661)))
+            g0_now_661,w0_now_661 = np.zeros_like(opd_now_661),np.zeros_like(opd_now_661)
+
+            for ilayer in range(len(opd_now[:,0])):
+                fopd = interp1d(wv196,opd_now[ilayer,:] , kind='cubic',fill_value="extrapolate")
+                fg0 = interp1d(wv196,g0_now[ilayer,:] , kind='cubic',fill_value="extrapolate")
+                fw0 = interp1d(wv196,w0_now[ilayer,:] , kind='cubic',fill_value="extrapolate")
+
+                opd_now_661[ilayer,:] = fopd(wv661)
+                g0_now_661[ilayer,:] = fg0(wv661)
+                w0_now_661[ilayer,:] = fw0(wv661)
+
+            opd_cld_climate[:,:,0], g0_cld_climate[:,:,0], w0_cld_climate[:,:,0] = opd_now_661, g0_now_661, w0_now_661                         
+            # opd_cld_climate[:,:,0], g0_cld_climate[:,:,0], w0_cld_climate[:,:,0] = opd_now, g0_now, w0_now
             
             #if np.sum(opd_cld_climate[:,:,1]) == 0 :
             #    w0,w1,w2,w3 = 1,0,0,0
             #elif (np.sum(opd_cld_climate[:,:,1]) != 0) and (np.sum(opd_cld_climate[:,:,2]) == 0):
             #    w0,w1,w2,w3 = 0.5,0.5,0,0
             #elif (np.sum(opd_cld_climate[:,:,2]) != 0) and (np.sum(opd_cld_climate[:,:,3]) == 0):
             #    w0,w1,w2,w3 = 0.33,0.33,0.33,0
@@ -5490,44 +5409,50 @@
             g0_clmt = (we0*opd_cld_climate[:,:,0]*g0_cld_climate[:,:,0]+we1*opd_cld_climate[:,:,1]*g0_cld_climate[:,:,1]+we2*opd_cld_climate[:,:,2]*g0_cld_climate[:,:,2]+we3*opd_cld_climate[:,:,3]*g0_cld_climate[:,:,3])/(sum_opd_clmt)
             w0_clmt = (we0*opd_cld_climate[:,:,0]*w0_cld_climate[:,:,0]+we1*opd_cld_climate[:,:,1]*w0_cld_climate[:,:,1]+we2*opd_cld_climate[:,:,2]*w0_cld_climate[:,:,2]+we3*opd_cld_climate[:,:,3]*w0_cld_climate[:,:,3])/(sum_opd_clmt)
             g0_clmt = np.nan_to_num(g0_clmt,nan=0.0)
             w0_clmt = np.nan_to_num(w0_clmt,nan=0.0)
             opd_clmt[np.where(opd_clmt <= 1e-5)] = 0.0
             
             
-            df_cld = vj.picaso_format(opd_clmt, w0_clmt, g0_clmt)
+            df_cld = vj.picaso_format(opd_clmt, w0_clmt, g0_clmt,pressure = cld_out['pressure'], wavenumber= wv661)
             bundle.clouds(df=df_cld)
             
             diff = (opd_clmt-opd_prev_cld_step)
             taudif = np.max(np.abs(diff))
             taudif_tol = 0.4*np.max(0.5*(opd_clmt+opd_prev_cld_step))
             
-            print("Max TAUCLD diff is", taudif, " Tau tolerance is ", taudif_tol)
+            if verbose: print("Max TAUCLD diff is", taudif, " Tau tolerance is ", taudif_tol)
+        else:
+            cld_out = 0
 
         
         DTAU, TAU, W0, COSB,ftau_cld, ftau_ray,GCOS2, DTAU_OG, TAU_OG, W0_OG, COSB_OG, \
         W0_no_raman , surf_reflect, ubar0,ubar1,cos_theta, single_phase,multi_phase, \
-        frac_a,frac_b,frac_c,constant_back,constant_forward, tridiagonal , \
-        wno,nwno,ng,nt, nlevel, ngauss, gauss_wts, mmw =  calculate_atm_deq(bundle, opacityclass,on_fly=on_fly, gases_fly=gases_fly)
+        frac_a,frac_b,frac_c,constant_back,constant_forward, \
+        wno,nwno,ng,nt, nlevel, ngauss, gauss_wts, mmw,gweight,tweight =  calculate_atm_deq(bundle, opacityclass,on_fly=on_fly, gases_fly=gases_fly)
 
         if self_consistent_kzz == True :
                 
-            flux_net_v_layer_full, flux_net_v_full, flux_plus_v_full, flux_minus_v_full , flux_net_ir_layer_full, flux_net_ir_full, flux_plus_ir_full, flux_minus_ir_full = climate(pressure, temp, dwni, bb , y2, tp, tmin, tmax, DTAU, TAU, W0, 
+            flux_net_v_layer_full, flux_net_v_full, flux_plus_v_full, flux_minus_v_full , flux_net_ir_layer_full, flux_net_ir_full, flux_plus_ir_full, flux_minus_ir_full = get_fluxes(pressure, temp, dwni, bb , y2, tp, tmin, tmax, DTAU, TAU, W0, 
             COSB,ftau_cld, ftau_ray,GCOS2, DTAU_OG, TAU_OG, W0_OG, COSB_OG, W0_no_raman , surf_reflect, 
-            ubar0,ubar1,cos_theta, FOPI, single_phase,multi_phase,frac_a,frac_b,frac_c,constant_back,constant_forward, tridiagonal , 
-            wno,nwno,ng,nt, nlevel, ngauss, gauss_wts,True, True)#True for reflected, True for thermal
+            ubar0,ubar1,cos_theta, FOPI, single_phase,multi_phase,frac_a,frac_b,frac_c,constant_back,constant_forward,  
+            wno,nwno,ng,nt, gweight,tweight, nlevel, ngauss, gauss_wts,compute_reflected, True)#True for reflected if rfacv!=0, True for thermal
 
             flux_net_ir_layer = flux_net_ir_layer_full[:]
             flux_plus_ir_attop = flux_plus_ir_full[0,:] 
             calc_type = 0
         
             kz = get_kzz(pressure, temp,grav,mmw,tidal,flux_net_ir_layer, flux_plus_ir_attop,t_table, p_table, grad, cp, calc_type,nstr)
+            photo_inputs_dict['kz'] = kz
+        if save_kzz == 1: 
+            if photo_inputs_dict['yesorno'] == False:
+                all_kzz = np.append(all_kzz,t_mix)
+            else:
+                all_kzz = np.append(all_kzz,kz)
 
-        if save_kzz == 1:
-            all_kzz = np.append(all_kzz,t_mix)
 
         ert = 0.0 # avg temp change
         scalt= 1.5
 
         dtx= abs(temp-temp_old)
         ert = np.sum(dtx)
         
@@ -5541,15 +5466,15 @@
         #####################################   
         
         temp_old= np.copy(temp)
         
         ert = ert/(float(nlevel)*scalt)
         
         if ((iii > 0) & (ert < convt) & (taudif < taudif_tol)) :
-            print("Profile converged")
+            if verbose: print("Profile converged")
             conv_flag = 1
             if final == True :
                 itmx = 6
                 it_max = it_max
             else :
                 itmx = 3
                 it_max= it_max
@@ -5592,18 +5517,18 @@
                 ert = 0.0 # avg temp change
                 scalt= 1.0
                 dtx= abs(temp-temp_old)
                 ert = np.sum(dtx)
                 temp_old= np.copy(temp)
                 '''
             
-            return pressure, temp , dtdp, conv_flag, qvmrs, qvmrs2, all_profiles, all_kzz, opd_cld_climate, g0_cld_climate, w0_cld_climate,flux_net_ir_layer, flux_plus_ir_attop
+            return pressure, temp , dtdp, conv_flag, qvmrs, qvmrs2, all_profiles, all_kzz, opd_cld_climate, g0_cld_climate, w0_cld_climate, cld_out, flux_net_ir_layer, flux_plus_ir_attop,photo_inputs_dict,bundle.inputs['atmosphere']['profile']
             
         
-        print("Big iteration is ",min(temp), iii)
+        if verbose: print("Big iteration is ",min(temp), iii)
     conv_flag = 0
     ## this is supposed to be useless so testing this
     '''
     if final == True :
         itmx = 6
         it_max = it_max
     else :
@@ -5649,27 +5574,35 @@
         temp_old= np.copy(temp)   
         ert = ert/(float(nlevel)*scalt)
         if ((iii > 0) & (ert < convt) & (taudif < 0.1)) :
             print("Profile converged")
             conv_flag = 1
     '''
     if conv_flag == 0:
-        print("Not converged")
+        if verbose: print("Not converged")
     else :
-        print("Profile converged")
+        if verbose: print("Profile converged")
     
-    return pressure, temp , dtdp, conv_flag, qvmrs, qvmrs2, all_profiles, all_kzz, opd_cld_climate, g0_cld_climate, w0_cld_climate,flux_net_ir_layer, flux_plus_ir_attop
+    return pressure, temp , dtdp, conv_flag, qvmrs, qvmrs2, all_profiles, all_kzz, opd_cld_climate, g0_cld_climate, w0_cld_climate, cld_out,flux_net_ir_layer, flux_plus_ir_attop,photo_inputs_dict,None
     
-def find_strat_deq(pressure, temp, dtdp , FOPI, nofczns,nstr,x_max_mult,
+def find_strat_deq(mieff_dir, pressure, temp, dtdp , FOPI, nofczns,nstr,x_max_mult,
              t_table, p_table, grad, cp, opacityclass, grav, 
-             rfaci, rfacv, nlevel, tidal, tmin, tmax, dwni, bb , y2 , tp, cloudy, cld_species,mh,fsed,flag_hack, quench_levels, kz,mmw, save_profile, all_profiles,self_consistent_kzz ,save_kzz,all_kzz, vulcan_run,opd_cld_climate,g0_cld_climate,w0_cld_climate,flux_net_ir_layer, flux_plus_ir_attop,on_fly=False, gases_fly=None ):
+             rfaci, rfacv, nlevel, tidal, tmin, tmax, dwni, 
+             bb , y2 , tp, cloudy, cld_species,mh,fsed,flag_hack, 
+             quench_levels, kz,mmw, save_profile, all_profiles,
+             self_consistent_kzz ,save_kzz,all_kzz, 
+             opd_cld_climate,g0_cld_climate,w0_cld_climate,
+             flux_net_ir_layer, flux_plus_ir_attop,
+             photo_inputs_dict=None,on_fly=False, gases_fly=None , verbose=1):
     """
     Function iterating on the TP profile by calling tstart and changing opacities as well
     Parameters
     ----------
+    mieff_dir: str
+        path to directory with mieff files for virga
     it_max : int
         Maximum iterations allowed in the inner no opa change loop
     itmx : int
         Maximum iterations allowed in the outer opa change loop
     conv : float
         
     convt: float
@@ -5722,14 +5655,17 @@
         Tidal Fluxes dimension = nlevel
     tmin : float
         Minimum allwed Temp in the profile
     tmax : float
         Maximum allowed Temp in the profile
     dwni : array
         Spectral interval corrections (dimension= nwvno)   
+    verbose : int 
+        If 1= prints out all output 
+        If 0= does not print anything out
         
     Returns
     -------
     array 
         Temperature array and lapse ratio array if converged
         else Temperature array twice
     """
@@ -5748,67 +5684,72 @@
     final = False
 
     grad_x, cp_x =convec(temp,pressure, t_table, p_table, grad, cp)
     # grad_x = 
     while dtdp[nstr[1]-1] >= subad*grad_x[nstr[1]-1] :
         ratio = dtdp[nstr[1]-1]/grad_x[nstr[1]-1]
 
-        if ratio > 2 :
-            print("Move up two levels")
+        if ratio > 1.8 :
+            if verbose: print("Move up two levels")
             ngrow = 2
             nstr = growup( 1, nstr , ngrow)
         else :
             ngrow = 1
             nstr = growup( 1, nstr , ngrow)
         
-        if nstr[1] < 6 :
+        if nstr[1] < 5 :
             raise ValueError( "Convection zone grew to Top of atmosphere, Need to Stop")
-        
-        pressure, temp, dtdp, profile_flag, qvmrs, qvmrs2, all_profiles, all_kzz,opd_cld_climate,g0_cld_climate,w0_cld_climate,flux_net_ir_layer, flux_plus_ir_attop = profile_deq(it_max_strat, itmx_strat, conv_strat, convt_strat, nofczns,nstr,x_max_mult,
-            temp,pressure, FOPI, t_table, p_table, grad, cp, opacityclass, grav, 
-             rfaci, rfacv, nlevel, tidal, tmin, tmax, dwni, bb , y2 , tp, final, cloudy, cld_species, mh,fsed,flag_hack, quench_levels, kz, mmw, save_profile, all_profiles, self_consistent_kzz,save_kzz,all_kzz,vulcan_run,opd_cld_climate,g0_cld_climate,w0_cld_climate,flux_net_ir_layer, flux_plus_ir_attop,on_fly=on_fly, gases_fly=gases_fly )
+        pressure, temp, dtdp, profile_flag, qvmrs, qvmrs2, all_profiles, all_kzz,opd_cld_climate,g0_cld_climate,w0_cld_climate,cld_out,flux_net_ir_layer, flux_plus_ir_attop,photo_inputs_dict,_= profile_deq(mieff_dir,it_max_strat, itmx_strat, conv_strat, convt_strat, nofczns,nstr,x_max_mult,\
+            temp,pressure, FOPI, t_table, p_table, grad, cp, opacityclass, grav,rfaci, rfacv, nlevel, tidal, tmin, tmax, dwni, bb , y2 , tp, final, cloudy, cld_species, mh,fsed,flag_hack, quench_levels, kz, mmw, save_profile, all_profiles, self_consistent_kzz,save_kzz,all_kzz,opd_cld_climate,g0_cld_climate,\
+            w0_cld_climate,flux_net_ir_layer, flux_plus_ir_attop,photo_inputs_dict,on_fly=on_fly, gases_fly=gases_fly , verbose=verbose)
 
     # now for the 2nd convection zone
     dt_max = 0.0 #DTMAX
     i_max = 0 #IMAX
     # -1 in ifirst to include ifirst index
     flag_super = 0
     for i in range(nstr[1]-1, ifirst-1, -1):
         add = dtdp[i] - grad_x[i]
-        if add/grad_x[i] >= 0.02 : # non-neglegible super-adiabaticity
+        if add > dt_max and add/grad_x[i] >= 0.02 : # non-neglegible super-adiabaticity
+            dt_max = add
             i_max =i
             break
     
     flag_final_convergence =0
-    if i_max == 0: # no superadiabaticity, we are done
+    if i_max == 0 or dt_max/grad_x[i_max] < 0.02: # no superadiabaticity, we are done
         flag_final_convergence = 1
 
     if flag_final_convergence  == 0:
-        print(" convection zone status")
-        print(nstr[0],nstr[1],nstr[2],nstr[3],nstr[4],nstr[5])
-        print(nofczns)
+        if verbose: print(" convection zone status")
+        if verbose: print(nstr[0],nstr[1],nstr[2],nstr[3],nstr[4],nstr[5])
+        if verbose: print(nofczns)
 
         nofczns = 2
         nstr[4]= nstr[1]
         nstr[5]= nstr[2]
         nstr[1]= i_max
         nstr[2] = i_max
-        nstr[3] = i_max
-        print(nstr)
+        nstr[3] = i_max #+ 1
+        if verbose: print(nstr)
         if nstr[3] >= nstr[4] :
             #print(nstr[0],nstr[1],nstr[2],nstr[3],nstr[4],nstr[5])
             #print(nofczns)
             raise ValueError("Overlap happened !")
-        pressure, temp, dtdp, profile_flag, qvmrs, qvmrs2, all_profiles, all_kzz,opd_cld_climate,g0_cld_climate,w0_cld_climate,flux_net_ir_layer, flux_plus_ir_attop = profile_deq(it_max_strat, itmx_strat, conv_strat, convt_strat, nofczns,nstr,x_max_mult,
-            temp,pressure, FOPI, t_table, p_table, grad, cp, opacityclass, grav, 
-             rfaci, rfacv, nlevel, tidal, tmin, tmax, dwni, bb , y2 , tp, final, cloudy, cld_species,mh, fsed,flag_hack, quench_levels, kz , mmw,save_profile, all_profiles, self_consistent_kzz, save_kzz,all_kzz,vulcan_run,opd_cld_climate,g0_cld_climate,w0_cld_climate,flux_net_ir_layer, flux_plus_ir_attop,on_fly=on_fly, gases_fly=gases_fly )
+        pressure, temp, dtdp, profile_flag, qvmrs, qvmrs2, all_profiles, all_kzz,opd_cld_climate,g0_cld_climate,w0_cld_climate,cld_out,flux_net_ir_layer, flux_plus_ir_attop,photo_inputs_dict,_= profile_deq(mieff_dir,it_max_strat, itmx_strat, conv_strat, convt_strat, nofczns,nstr,x_max_mult,\
+            temp,pressure, FOPI, t_table, p_table, grad, cp, opacityclass, grav, \
+             rfaci, rfacv, nlevel, tidal, tmin, tmax, dwni, bb , y2 , tp, final, 
+             cloudy, cld_species,mh, fsed,flag_hack, quench_levels, kz , mmw,
+             save_profile, all_profiles, self_consistent_kzz, save_kzz,all_kzz,
+             opd_cld_climate,g0_cld_climate,w0_cld_climate,flux_net_ir_layer, 
+             flux_plus_ir_attop,photo_inputs_dict,
+             on_fly=on_fly, gases_fly=gases_fly, verbose=verbose )
 
         i_change = 1
         while i_change == 1 :
-            print("Grow Phase : Upper Zone")
+            if verbose: print("Grow Phase : Upper Zone")
             i_change = 0
 
             d1 = dtdp[nstr[1]-1]
             d2 = dtdp[nstr[3]]
             c1 = grad_x[nstr[1]-1]
             c2 = grad_x[nstr[3]]
 
@@ -5826,68 +5767,67 @@
 
                     if nstr[2] == nstr[4]: # one conv zone
                         nofczns =1
                         nstr[2] = nstr[5]
                         nstr[3] = 0
                         i_change = 1
                 print(nstr)
-                pressure, temp, dtdp, profile_flag,qvmrs, qvmrs2, all_profiles, all_kzz,opd_cld_climate,g0_cld_climate,w0_cld_climate,flux_net_ir_layer, flux_plus_ir_attop = profile_deq(it_max_strat, itmx_strat, conv_strat, convt_strat, nofczns,nstr,x_max_mult,
-            temp,pressure, FOPI, t_table, p_table, grad, cp, opacityclass, grav, 
-             rfaci, rfacv, nlevel, tidal, tmin, tmax, dwni, bb , y2 , tp, final, cloudy, cld_species, mh,fsed,flag_hack, quench_levels, kz, mmw, save_profile, all_profiles,self_consistent_kzz,save_kzz,all_kzz, vulcan_run,opd_cld_climate,g0_cld_climate,w0_cld_climate,flux_net_ir_layer, flux_plus_ir_attop,on_fly=on_fly, gases_fly=gases_fly)
+                pressure, temp, dtdp, profile_flag,qvmrs, qvmrs2, all_profiles, all_kzz,opd_cld_climate,g0_cld_climate,w0_cld_climate,cld_out,flux_net_ir_layer, flux_plus_ir_attop,photo_inputs_dict,_ = profile_deq(mieff_dir,it_max_strat, itmx_strat, conv_strat, convt_strat, nofczns,nstr,x_max_mult,\
+            temp,pressure, FOPI, t_table, p_table, grad, cp, opacityclass, grav, \
+             rfaci, rfacv, nlevel, tidal, tmin, tmax, dwni, bb , y2 , tp, final, cloudy, cld_species, mh,fsed,flag_hack, quench_levels, kz, mmw, save_profile, all_profiles,self_consistent_kzz,save_kzz,all_kzz,opd_cld_climate,g0_cld_climate,w0_cld_climate,flux_net_ir_layer, flux_plus_ir_attop,photo_inputs_dict,on_fly=on_fly, gases_fly=gases_fly, verbose=verbose)
 
                 d1 = dtdp[nstr[1]-1]
                 d2 = dtdp[nstr[3]]
                 c1 = grad_x[nstr[1]-1]
                 c2 = grad_x[nstr[3]]
             #Now grow the lower zone.
-            while ((dtdp[nstr[4]-1] >= subad*grad_x[nstr[5]-1]) and nofczns > 1):
+            while ((dtdp[nstr[4]-1] >= subad*grad_x[nstr[4]-1]) and nofczns > 1):
                 
                 ngrow = 1
                 nstr = growup( 2, nstr , ngrow)
                 #Now check to see if two zones have merged and stop further searching if so.
                 if nstr[2] == nstr[4] :
                     nofczns = 1
                     nstr[2] = nstr[5]
                     nstr[3] = 0
                     i_change =1
                 print(nstr)
-                pressure, temp, dtdp, profile_flag, qvmrs, qvmrs2, all_profiles, all_kzz,opd_cld_climate,g0_cld_climate,w0_cld_climate,flux_net_ir_layer, flux_plus_ir_attop = profile_deq(it_max_strat, itmx_strat, conv_strat, convt_strat, nofczns,nstr,x_max_mult,
-                    temp,pressure, FOPI, t_table, p_table, grad, cp, opacityclass, grav, 
-                    rfaci, rfacv, nlevel, tidal, tmin, tmax, dwni, bb , y2 , tp, final, cloudy, cld_species, mh,fsed,flag_hack, quench_levels, kz, mmw,save_profile, all_profiles, self_consistent_kzz, save_kzz,all_kzz,vulcan_run,opd_cld_climate,g0_cld_climate,w0_cld_climate,flux_net_ir_layer, flux_plus_ir_attop,on_fly=on_fly, gases_fly=gases_fly)
+                pressure, temp, dtdp, profile_flag, qvmrs, qvmrs2, all_profiles, all_kzz,opd_cld_climate,g0_cld_climate,w0_cld_climate,cld_out,flux_net_ir_layer, flux_plus_ir_attop,photo_inputs_dict,_ = profile_deq(mieff_dir,it_max_strat, itmx_strat, conv_strat, convt_strat, nofczns,nstr,x_max_mult, \
+                                                        temp,pressure, FOPI, t_table, p_table, grad, cp, opacityclass, grav,rfaci, rfacv, nlevel, tidal, tmin, tmax, dwni, bb , y2 , tp, final, cloudy, cld_species, mh,fsed,flag_hack, quench_levels, kz, mmw,save_profile, all_profiles, self_consistent_kzz, save_kzz,all_kzz,opd_cld_climate,g0_cld_climate,w0_cld_climate,flux_net_ir_layer, flux_plus_ir_attop,photo_inputs_dict,on_fly=on_fly, gases_fly=gases_fly)
             
 
             flag_final_convergence = 1
         
     itmx_strat =6
     it_max_strat = 10
     convt_strat = 2.0
     convt_strat = 2.0
-    x_max_mult = 2.0
+    x_max_mult = x_max_mult/2.0
     ip2 = -10
 
     final = True
     print("final",nstr)
-    pressure, temp, dtdp, profile_flag,qvmrs, qvmrs2, all_profiles, all_kzz,opd_cld_climate,g0_cld_climate,w0_cld_climate,flux_net_ir_layer, flux_plus_ir_attop = profile_deq(it_max_strat, itmx_strat, conv_strat, convt_strat, nofczns,nstr,x_max_mult,
-                temp,pressure, FOPI, t_table, p_table, grad, cp,opacityclass, grav, 
-                rfaci, rfacv, nlevel, tidal, tmin, tmax, dwni, bb , y2 , tp, final, cloudy, cld_species,mh,fsed,flag_hack,quench_levels,kz, mmw,save_profile, all_profiles, self_consistent_kzz,save_kzz,all_kzz,vulcan_run,opd_cld_climate,g0_cld_climate,w0_cld_climate,flux_net_ir_layer, flux_plus_ir_attop,on_fly=on_fly, gases_fly=gases_fly)
+    pressure, temp, dtdp, profile_flag,qvmrs, qvmrs2, all_profiles, all_kzz,opd_cld_climate,g0_cld_climate,w0_cld_climate,cld_out,flux_net_ir_layer, flux_plus_ir_attop,photo_inputs_dict,_ = profile_deq(mieff_dir,it_max_strat, itmx_strat, conv_strat, convt_strat, nofczns,nstr,x_max_mult,\
+                temp,pressure, FOPI, t_table, p_table, grad, cp,opacityclass, grav, \
+                rfaci, rfacv, nlevel, tidal, tmin, tmax, dwni, bb , y2 , tp, final, cloudy, cld_species,mh,fsed,flag_hack,quench_levels,kz, mmw,save_profile, all_profiles, self_consistent_kzz,save_kzz,all_kzz,opd_cld_climate,g0_cld_climate,w0_cld_climate,flux_net_ir_layer, flux_plus_ir_attop,photo_inputs_dict,on_fly=on_fly, gases_fly=gases_fly, verbose=verbose)
 
     #    else :
     #        raise ValueError("Some problem here with goto 125")
         
     if profile_flag == 0:
-        print("ENDING WITHOUT CONVERGING")
+        if verbose: print("ENDING WITHOUT CONVERGING")
     elif profile_flag == 1:
-        print("YAY ! ENDING WITH CONVERGENCE")
+        if verbose: print("YAY ! ENDING WITH CONVERGENCE")
         
     bundle = inputs(calculation='brown')
     bundle.phase_angle(0)
     bundle.gravity(gravity=grav , gravity_unit=u.Unit('m/s**2'))
     bundle.add_pt( temp, pressure)
 
-    if vulcan_run == False:
+    if photo_inputs_dict['yesorno'] == False:
         k_b = 1.38e-23 # boltzmann constant
         m_p = 1.66e-27 # proton mass
 
         if len(mmw) < len(temp):
             mmw = np.append(mmw,mmw[-1])
         con  = k_b/(mmw*m_p)
 
@@ -5896,63 +5836,95 @@
         kz = scale_H**2/all_kzz[-len(temp):] ## level mixing timescales
 
         quench_levels, t_mix = quench_level(pressure, temp, kz ,mmw, grav, return_mix_timescale=True)
 
         qvmrs, qvmrs2 = bundle.premix_atmosphere_diseq(opacityclass, quench_levels=quench_levels, df = bundle.inputs['atmosphere']['profile'].loc[:,['pressure','temperature']],t_mix=t_mix)
     else :
         bundle.premix_atmosphere(opacityclass, df = bundle.inputs['atmosphere']['profile'].loc[:,['pressure','temperature']])
-        k_b = 1.38e-23 # boltzmann constant
-        m_p = 1.66e-27 # proton mass
         
-        if len(mmw) < len(temp):
-            mmw = np.append(mmw,mmw[-1])
-        con  = k_b/(mmw*m_p)
 
-        scale_H = con * temp*1e2/(grav)
-
-        kz = scale_H**2/all_kzz[-len(temp):] ## level mixing timescales
-        t_mix = bundle.run_vulcan(pressure,temp,kz,grav,mmw, first = False)    
+        kz = all_kzz[-len(temp):] ## level mixing timescales
+        pc= bundle.call_photochem(temp,pressure,photo_inputs_dict['mh'],photo_inputs_dict['CtoO'],photo_inputs_dict['psurf'],photo_inputs_dict['m_planet'],photo_inputs_dict['r_planet'],photo_inputs_dict['kz'],tstop=photo_inputs_dict['tstop'],filename = photo_inputs_dict['photochem_file'],stfilename =photo_inputs_dict['photochem_stfile'],network = photo_inputs_dict['photochem_network'],network_ct=photo_inputs_dict['photochem_networkct'],first=False,pc=photo_inputs_dict['pc'])
+        photo_inputs_dict['pc'] = pc
+        all_kzz = np.append(all_kzz, kz)
+        quench_levels = np.array([0,0,0,0])
+        photo_inputs_dict['pc'] = pc
+        
         qvmrs,qvmrs2 = 0,0
     
     if cloudy == 1:
-        DTAU, TAU, W0, COSB,ftau_cld, ftau_ray,GCOS2, DTAU_OG, TAU_OG, W0_OG, COSB_OG, W0_no_raman , surf_reflect, ubar0,ubar1,cos_theta, single_phase,multi_phase,frac_a,frac_b,frac_c,constant_back,constant_forward, tridiagonal , wno,nwno,ng,nt, nlevel, ngauss, gauss_wts, mmw =  calculate_atm_deq(bundle, opacityclass,on_fly=on_fly, gases_fly=gases_fly)
+        DTAU, TAU, W0, COSB,ftau_cld, ftau_ray,GCOS2, DTAU_OG, TAU_OG, W0_OG, COSB_OG, W0_no_raman , surf_reflect, ubar0,ubar1,cos_theta, single_phase,multi_phase,frac_a,frac_b,frac_c,constant_back,constant_forward, wno,nwno,ng,nt, nlevel, ngauss, gauss_wts, mmw,gweight,tweight =  calculate_atm_deq(bundle, opacityclass,on_fly=on_fly, gases_fly=gases_fly)
         metallicity = 10**(0.0) #atmospheric metallicity relative to Solar
         mean_molecular_weight = np.mean(mmw) # atmospheric mean molecular weight
-        directory ='/Users/sagnickmukherjee/Documents/GitHub/virga/refr_new661'
+        # directory ='/Users/sagnickmukherjee/Documents/GitHub/virga/refr_new661'
+        # directory = '/home/jjm6243/dev_virga/'
+        directory = mieff_dir
+
         calc_type =0
         kzz  = get_kzz(pressure, temp,grav,mmw,tidal,flux_net_ir_layer, flux_plus_ir_attop,t_table, p_table, grad, cp, calc_type,nstr)
         bundle.inputs['atmosphere']['profile']['kz'] = kzz
 
 
         cld_out = bundle.virga(cld_species,directory, fsed=fsed,mh=metallicity,
-                        mmw = mean_molecular_weight,full_output=False,climate=True)
+                        mmw = mean_molecular_weight)#,climate=True)
         
-        opd_now, w0_now, g0_now = cld_out
-        df_cld = vj.picaso_format(opd_now, w0_now, g0_now)
+        opd_now, w0_now, g0_now = cld_out['opd_per_layer'],cld_out['single_scattering'],cld_out['asymmetry']
+        df_cld = vj.picaso_format(opd_now, w0_now, g0_now,pressure = cld_out['pressure'], wavenumber= 1e4/cld_out['wave'])
         bundle.clouds(df=df_cld)  
     else:
         opd_now,w0_now,g0_now = 0,0,0
+        cld_out = 0
     
     #bundle.premix_atmosphere_diseq(opacityclass, quench_levels=quench_levels, df = bundle.inputs['atmosphere']['profile'].loc[:,['pressure','temperature']])
-    DTAU, TAU, W0, COSB,ftau_cld, ftau_ray,GCOS2, DTAU_OG, TAU_OG, W0_OG, COSB_OG, W0_no_raman , surf_reflect, ubar0,ubar1,cos_theta, single_phase,multi_phase,frac_a,frac_b,frac_c,constant_back,constant_forward, tridiagonal , wno,nwno,ng,nt, nlevel, ngauss, gauss_wts, mmw =  calculate_atm_deq(bundle, opacityclass,on_fly=on_fly, gases_fly=gases_fly)
+    DTAU, TAU, W0, COSB,ftau_cld, ftau_ray,GCOS2, DTAU_OG, TAU_OG, W0_OG, COSB_OG, W0_no_raman , surf_reflect, ubar0,ubar1,cos_theta, single_phase,multi_phase,frac_a,frac_b,frac_c,constant_back,constant_forward, wno,nwno,ng,nt, nlevel, ngauss, gauss_wts, mmw,gweight,tweight =  calculate_atm_deq(bundle, opacityclass,on_fly=on_fly, gases_fly=gases_fly)
     
-    flux_net_v_layer_full, flux_net_v_full, flux_plus_v_full, flux_minus_v_full , flux_net_ir_layer_full, flux_net_ir_full, flux_plus_ir_full, flux_minus_ir_full = climate(pressure, temp, dwni, bb , y2, tp, tmin, tmax, DTAU, TAU, W0, 
+    flux_net_v_layer_full, flux_net_v_full, flux_plus_v_full, flux_minus_v_full , flux_net_ir_layer_full, flux_net_ir_full, flux_plus_ir_full, flux_minus_ir_full = get_fluxes(pressure, temp, dwni, bb , y2, tp, tmin, tmax, DTAU, TAU, W0, 
             COSB,ftau_cld, ftau_ray,GCOS2, DTAU_OG, TAU_OG, W0_OG, COSB_OG, W0_no_raman , surf_reflect, 
-            ubar0,ubar1,cos_theta, FOPI, single_phase,multi_phase,frac_a,frac_b,frac_c,constant_back,constant_forward, tridiagonal , 
-            wno,nwno,ng,nt, nlevel, ngauss, gauss_wts, False, True) #false for reflected, true for thermal
+            ubar0,ubar1,cos_theta, FOPI, single_phase,multi_phase,frac_a,frac_b,frac_c,constant_back,constant_forward, 
+            wno,nwno,ng,nt,gweight,tweight, nlevel, ngauss, gauss_wts, False, True) #false for reflected, true for thermal
 
 
     
-    return pressure, temp, dtdp, nstr , flux_plus_ir_full, qvmrs, qvmrs2, bundle.inputs['atmosphere']['profile'], all_profiles, all_kzz,opd_now,w0_now,g0_now
+    return pressure, temp, dtdp, nstr , flux_plus_ir_full, qvmrs, qvmrs2, bundle.inputs['atmosphere']['profile'], all_profiles, all_kzz,cld_out,photo_inputs_dict,profile_flag
 
 #@jit(nopython=True, cache=True)
 def OH_conc(temp,press,x_h2o,x_h2):
     K = 10**(3.672 - (14791/temp))
     kb= 1.3807e-16 #cgs
     
     x_oh = K * x_h2o * (x_h2**(-0.5)) * (press**(-0.5))
     press_cgs = press*1e6
     
     n = press_cgs/(kb*temp)
     
     return x_oh*n
 
+
+
+'''
+12/13/2023 - NEB deprecated thi code from SM as it was not proven to help correct 
+profiles that went off the grid 
+
+@jit(nopython=True, cache=True)
+def correct_profile(temp,pressure,wh,min_temp):
+    
+    indices = wh[0]
+    for i in range(len(indices)):
+        if indices[i] == 0:
+            temp[indices[i]] = min_temp+0.5
+        elif (temp[indices[i]-1] > min_temp) and (temp[indices[i]+1]) > min_temp :
+            temp_prev = temp[indices[i]-1]
+            temp_next = temp[indices[i]+1]
+            press_prev = pressure[indices[i]-1]
+            press_next = pressure[indices[i]+1]
+            dtdlnp = (temp_next-temp_prev)/np.log(press_next/press_prev)
+            temp[indices[i]] = temp_prev +np.log(pressure[indices[i]]/press_prev)*dtdlnp
+        else :
+            temp[indices[i]] = min_temp+0.5
+            temp[indices[i]-1] = min_temp+0.5
+            temp[indices[i]+1] = min_temp + 0.5
+    
+
+
+    return temp
+'''
+
```

### Comparing `picaso-3.1.2/picaso/justplotit.py` & `picaso-3.2/picaso/justplotit.py`

 * *Files 1% similar despite different names*

```diff
@@ -22,18 +22,19 @@
 from matplotlib import rc
 
 from scipy.stats.stats import pearsonr  
 from scipy.stats import binned_statistic
 
 from .fluxes import blackbody, get_transit_1d
 from .opacity_factory import *
+from .climate import convec
 
 def mean_regrid(x, y, newx=None, R=None):
     """
-    Rebin the spectrum at a minimum R or on a fixed grid 
+    Rebin the spectrum at a minimum R or on a fixed grid! 
 
     Parameters
     ----------
     x : array 
         Wavenumbers
     y : array 
         Anything (e.g. albedo, flux)
@@ -57,15 +58,16 @@
     else: 
         raise Exception('Please either enter a newx or a R') 
     y, edges, binnum = binned_statistic(x,y,bins=newx)
     newx = (edges[0:-1]+edges[1:])/2.0
 
     return newx, y
 
-def plot_errorbar(x,y,e,plot=None,point_kwargs={}, error_kwargs={},plot_type='bokeh', plot_kwargs={}):
+def plot_errorbar(x,y,e,plot=None,point_kwargs={}, error_kwargs={},
+    plot_type='bokeh', plot_kwargs={}):
     """
     Plot only symmetric y error bars in bokeh plot
 
     Parameters
     ----------
     x : array 
         x data 
@@ -198,68 +200,117 @@
     err = []
     for i in range(len(newx)-1):
         loc = np.where(((oldx>newx[i]) & (oldx<=newx[i+1])))[0]
         err += [np.sqrt(np.sum(dy[loc]**2.0))/len(dy[loc])]
     return err
 
 
-def mixing_ratio(full_output,limit=50,ng=None,nt=None, **kwargs):
+def mixing_ratio(full_output,limit=50,ng=None,nt=None, plot_type='bokeh',
+        molecules=None,
+        **kwargs):
     """Returns plot of mixing ratios 
 
     Parameters
     ----------
     full_output : class
         picaso.atmsetup.ATMSETUP
     limit : int
         Limits the number of curves to 20. Will plot the top 20 molecules 
         with highest max(abundance). Limit must be >=3. 
+    molecules : list 
+        Directly specify which molecule to plot 
+    plot_type : str 
+        Options are "bokeh" or "matplotlib". Default is bokeh
     **kwargs : dict 
         Any key word argument for bokeh.figure() 
     """
-    molecules = full_output['weights'].keys()
     #set plot defaults
     if ((ng==None) & (nt==None)):
         pressure = full_output['layer']['pressure']
         mixingratios = full_output['layer']['mixingratios']
     else: 
         pressure = full_output['layer']['pressure'][:,ng,nt]
         mixingratios = pd.DataFrame(full_output['layer']['mixingratios'][:,:,ng,nt],columns=molecules)
 
-    kwargs['height'] = kwargs.get('plot_height',kwargs.get('height',300))
-    kwargs['width'] = kwargs.get('plot_width', kwargs.get('width',400))
-    if 'plot_width' in kwargs.keys() : kwargs.pop('plot_width')
-    if 'plot_height' in kwargs.keys() : kwargs.pop('plot_height')
-    kwargs['title'] = kwargs.get('title','Mixing Ratios')
-    kwargs['y_axis_label'] = kwargs.get('y_axis_label','Pressure(Bars)')
-    kwargs['x_axis_label'] = kwargs.get('x_axis_label','Mixing Ratio(v/v)')
-    kwargs['y_axis_type'] = kwargs.get('y_axis_type','log')
-    kwargs['x_axis_type'] = kwargs.get('x_axis_type','log') 
-    kwargs['y_range'] = kwargs.get('y_range',[np.max(pressure),np.min(pressure)])
-    kwargs['x_range'] = kwargs.get('x_range',[1e-20, 1e2])
+    #both bokeh/matplotlib get data 
+    if isinstance(molecules, type(None)):
+    # Check if the inputted molecule is actually in the list and remove 'pressure' and 'temperature'
+        to_plot = [mol for mol in mixingratios.keys() if mol not in ['pressure', 'temperature', 'kz']][:limit]
+    elif isinstance(molecules , str):
+        to_plot = [molecules]
+    elif isinstance((molecules) , list):
+        to_plot = molecules
 
-    #to plot (incl limit)
-    to_plot=mixingratios.max().sort_values(ascending=False)[0:limit].keys()
+    molecules=to_plot
 
-    fig = figure(**kwargs)
-    if len(molecules) < 3: ncol = 5
-    else: ncol = len(molecules)
-    if limit<3: 
-        cols = pals.magma(5) #magma needs at least 5 colors
-    else: 
-        cols = pals.magma(min([ncol,limit]))
-    legend_it=[]    
-    for mol , c in zip(to_plot,cols):
-        ind = np.where(mol==np.array(molecules))[0][0]
-        f = fig.line(mixingratios[mol],pressure, color=c, line_width=3,
-                    muted_color=c, muted_alpha=0.2)
-        legend_it.append((mol, [f]))
+    #sets defaults for the user for BOKEH
+    if plot_type=='bokeh':
+        kwargs['height'] = kwargs.get('plot_height',kwargs.get('height',300))
+        kwargs['width'] = kwargs.get('plot_width', kwargs.get('width',400))
+        if 'plot_width' in kwargs.keys() : kwargs.pop('plot_width')
+        if 'plot_height' in kwargs.keys() : kwargs.pop('plot_height')
+        kwargs['y_axis_label'] = kwargs.get('y_axis_label','Pressure(Bars)')
+        kwargs['x_axis_label'] = kwargs.get('x_axis_label','Mixing Ratio(v/v)')
+        kwargs['y_axis_type'] = kwargs.get('y_axis_type','log')
+        kwargs['x_axis_type'] = kwargs.get('x_axis_type','log') 
+        kwargs['y_range'] = kwargs.get('y_range',[np.max(pressure),np.min(pressure)])
+        kwargs['x_range'] = kwargs.get('x_range',[1e-20, 5])
+    elif plot_type=='matplotlib':
+        #adjusted kwargs for matplotlib
+        kwargs.setdefault('height', kwargs.get('plot_height', kwargs.get('height', 5)))
+        kwargs.setdefault('width', kwargs.get('plot_width', kwargs.get('width', 7)))
+        kwargs.pop('plot_width', None)
+        kwargs.pop('plot_height', None)
+        kwargs.setdefault('y_axis_label', 'Pressure(Bars)')
+        kwargs.setdefault('x_axis_label', 'Mixing Ratio(v/v)')
+        kwargs.setdefault('y_axis_type', 'log')
+        kwargs.setdefault('x_axis_type', 'log')
+        kwargs.setdefault('y_range', [np.max(pressure), np.min(pressure)])
+        kwargs.setdefault('x_range', [1e-25, 5])
 
-    legend = Legend(items=legend_it, location=(0, -20))
-    legend.click_policy="mute"
-    fig.add_layout(legend, 'left')  
+   # Determine what molecules to plot for the user
+    if plot_type=='bokeh':
+        fig = figure(**kwargs)
+        if len(molecules) < 3: ncol = 5
+        else: ncol = len(molecules)
+        if limit<3: 
+            cols = pals.magma(5) #magma needs at least 5 colors
+        else: 
+            cols = pals.magma(min([ncol,limit]))
+        legend_it=[]    
+        for mol , c in zip(to_plot,cols):
+            ind = np.where(mol==np.array(molecules))[0][0]
+            f = fig.line(mixingratios[mol],pressure, color=c, line_width=3,
+                        muted_color=c, muted_alpha=0.2)
+            legend_it.append((mol, [f]))
+
+        legend = Legend(items=legend_it, location=(0, -20))
+        legend.click_policy="mute"
+        fig.add_layout(legend, 'left')  
+
+    elif plot_type=='matplotlib':
+
+        #or fig, ax = plt.subplots(**kwargs)
+        fig = plt.figure(figsize=(kwargs['width'], kwargs['height']))
+        axes = fig.add_subplot(1,1,1)
+        ind = np.where(mol for mol in np.array(molecules))[0][0]
+
+        for mol in to_plot:
+            axes.plot(mixingratios[mol], pressure, label=mol)
+        axes.set_xlim(kwargs['x_range'])
+        #set y lim 
+
+        #add the legend 
+        axes.legend()
+
+        axes.set_xlabel("Mixing Ratios [v/v]") #change this to use kwargs x_axis_label
+        axes.set_ylabel("Pressure")#add units  and change this to use kwargs y_axis_label
+        axes.set_yscale('log')
+        axes.set_xscale('log')
+        axes.invert_yaxis()
 
     return fig
     
 def pt(full_output,ng=None, nt=None, **kwargs):
     """Returns plot of pressure temperature profile
 
     Parameters
@@ -1610,15 +1661,15 @@
 
     press2D = np.transpose(np.repeat(full_output['layer']['pressure'][np.newaxis], np.shape(sum_taus)[1], axis=0))
 
     bb = np.ones(np.shape(press2D))
     for i, temp in enumerate(full_output['layer']['temperature']):
         for j, wave in enumerate(1/full_output['wavenumber']):
             bb[i, j] = blackbody(temp, wave)[0][0]
-    CF = bb[0:-1, :] * np.exp(-sum_taus[0:-1, :]) * all_taus[0:-1, :] / np.diff(press2D, axis=0)
+    CF = bb[0:-1, :] * np.exp(-sum_taus[0:-1, :]) * all_taus[0:-1, :] / np.diff(np.log(press2D), axis=0)
 
     fig, ax = plt.subplots(figsize=(15,10))
     #if not isinstance( clim , type(None)):
     #    CF_clipped = np.clip(CF, clim[0],clim[1])
     #else: 
     #    CF_clipped = CF+0
     
@@ -2113,7 +2164,35 @@
     color_bar = ColorBar(color_mapper=mapper, major_label_text_font_size="12px",
                      ticker=BasicTicker(desired_num_ticks=len(colors)),
                      label_standoff=6, border_line_color=None, location=(0, 0))
     p.add_layout(color_bar, 'below')
     p.axis.major_label_text_font_size='12px'
     return p
 
+    
+def pt_adiabat(clima_out, input_class, plot=True):
+    """
+    Plot the PT profile with the adiabat 
+
+    Parameters
+    ----------
+    clima_out : dict
+        Full output from picaso 
+    input_class : justdoit.input
+        PICASO input class (e.g. the result of jdi.inputs()) 
+
+    Returns
+    -------
+    adiabat, dTdP, pressure 
+    """
+    layer_p = clima_out['spectrum_output']['full_output']['layer']['pressure']
+    
+    grad, cp = convec(clima_out['temperature'],clima_out['pressure'],
+                      input_class.inputs['climate']['t_table'], input_class.inputs['climate']['p_table'], 
+                      input_class.inputs['climate']['grad'], input_class.inputs['climate']['cp'])
+                      
+    plt.semilogy(clima_out['dtdp'], layer_p)
+    plt.semilogy(grad,layer_p) 
+    plt.ylim([1e2,1e-4]), 
+    plt.xlabel('dT/dP vs adiabat')
+    plt.ylabel('Pressure(bars)')
+    return cp, clima_out['dtdp'], layer_p
```

### Comparing `picaso-3.1.2/picaso/opacity_factory.py` & `picaso-3.2/picaso/opacity_factory.py`

 * *Files identical despite different names*

### Comparing `picaso-3.1.2/picaso/optics.py` & `picaso-3.2/picaso/optics.py`

 * *Files 0% similar despite different names*

```diff
@@ -298,15 +298,15 @@
     #====================== ADD CLOUD OPACITY====================== 
     for igauss in range(ngauss):
         TAUCLD[:,:,igauss] = atm.layer['cloud']['opd'] #TAUCLD is the total extinction from cloud = (abs + scattering)
         asym_factor_cld[:,:,igauss] = atm.layer['cloud']['g0']
         single_scattering_cld[:,:,igauss] = atm.layer['cloud']['w0'] 
 
     if return_mode: 
-        taus_by_species['cloud'] = TAUCLD[:,:,0]*single_scattering_cld[:,:,0]
+        taus_by_species['cloud'] = TAUCLD[:,:,0]#*single_scattering_cld[:,:,0]
         return taus_by_species
         
     #====================== If user requests full output, add Tau's to atmosphere class=====
     if full_output:
         atmosphere.taugas = TAUGAS
         atmosphere.tauray = TAURAY
         atmosphere.taucld = TAUCLD
@@ -616,15 +616,15 @@
     alpha_pl = ( 1. - f ) * alp[ip] + f * alp[ip+1]
     alpha_pr = ( 1. - f ) * arp[ip] + f * arp[ip+1]
     alpha_p2 = (( 2. * alpha_pr + alpha_pl ) / 3. ) ** 2
     gamma_p2 = ( alpha_pl - alpha_pr ) ** 2
     qv = facv / SHIFT( WAVEL, -SHIFTV0 ) ** 4 * ( 3. * alpha_p2 + 2./3. * gamma_p2 )    
     """
     dat = pd.read_csv(os.path.join(os.environ.get('picaso_refdata'), 'opacities','raman_fortran.txt'),
-                        delim_whitespace=True, header=None, names = ['w','f'])
+                        sep='\s+', header=None, names = ['w','f'])
     #fill in matrix to match real raman format
     interp_raman = np.interp(wave, dat['w'].values, dat['f'].values, )
     raman_factor = np.zeros((nlayer, len(wave)))
     for i in range(nlayer): 
         raman_factor[i,:] = interp_raman#return flipped values for raman
     return  raman_factor 
 
@@ -648,15 +648,15 @@
     """
     def __init__(self, ck_dir, cont_dir, wave_range=None, 
         deq=False, on_fly=False,gases_fly=None):
         self.ck_filename = ck_dir
         #read in the full abundance file sot hat we can check the number of kcoefficient layers 
         #this should either be 1460 or 1060
         self.full_abunds =  pd.read_csv(os.path.join(self.ck_filename,'full_abunds'),
-            delim_whitespace=True)
+            sep='\s+')
         self.kcoeff_layers = self.full_abunds.shape[0]
 
         if deq == False :
         #choose get data function based on layer number
             if self.kcoeff_layers==1060: 
                 self.get_legacy_data_1060(wave_range,deq=deq) #wave_range not used yet
             elif self.kcoeff_layers==1460:
@@ -705,15 +705,15 @@
 
         Note
         ----
         This function is **highly** sensitive to the file format. You cannot edit the ascii file and then 
         run this function. Each specific line is accounted for.
         """
         data = pd.read_csv(os.path.join(self.ck_filename,'ascii_data'), 
-                  delim_whitespace=True,header=None, 
+                  sep='\s+',header=None, 
                   names=list(range(9)),dtype=str)
 
         num_species = int(data.iloc[0,0])
         max_ele = 35 
         self.max_tc = 60 
         self.max_pc = 18
         max_windows = 200 
@@ -766,16 +766,16 @@
         self.ngauss = int(data.iloc[end_temps+1,0])
 
         assert self.ngauss == 8, 'Legacy code uses 8 gauss points not {0}. Check read in statements'.format(self.ngauss)
 
         gpts_wts = np.reshape(np.array(data.iloc[end_temps+1:2+end_temps+int(2*self.ngauss/3),0:3]
                  .astype(float)).ravel()[1:-1], (self.ngauss,2))
 
-        self.gauss_pts = [i[0] for i in gpts_wts]
-        self.gauss_wts = [i[1] for i in gpts_wts]
+        self.gauss_pts = np.array([i[0] for i in gpts_wts])
+        self.gauss_wts = np.array([i[1] for i in gpts_wts])
 
         if not deq:
             kappa = np.array(data.iloc[3+end_temps+int(2*self.ngauss/3):-2,0:3].astype(float)).ravel()
             kappa = np.reshape(kappa, (max_windows,self.ngauss*2,self.max_pc,self.max_tc),order='F')
             #want the axes to be [npressure, ntemperature, nwave, ngauss ]
             kappa = kappa.swapaxes(1,3)
             kappa = kappa.swapaxes(0,2)
@@ -791,15 +791,15 @@
 
         Note
         ----
         This function is **highly** sensitive to the file format. You cannot edit the ascii file and then 
         run this function. Each specific line is accounted for.
         """
         data = pd.read_csv(os.path.join(self.ck_filename,'ascii_data'), 
-                  delim_whitespace=True,header=None, 
+                  sep='\s+',header=None, 
                   names=list(range(9)),dtype=str)
 
         num_species = int(data.iloc[0,0])
         if num_species == 24:
             max_ele = 35 
             self.max_tc = 73 
             self.max_pc = 20
@@ -854,16 +854,16 @@
                 self.ngauss = int(data.iloc[end_temps,3])
                 
                 assert self.ngauss == 8, 'Legacy code uses 8 gauss points not {0}. Check read in statements'.format(self.ngauss)
 
                 gpts_wts = np.reshape(np.array(data.iloc[end_temps+1:2+end_temps+int(2*self.ngauss/3),0:3]
                  .astype(float)).ravel()[:-2], (self.ngauss,2))
                 
-                self.gauss_pts = [i[0] for i in gpts_wts]
-                self.gauss_wts = [i[1] for i in gpts_wts]
+                self.gauss_pts = np.array([i[0] for i in gpts_wts])
+                self.gauss_wts = np.array([i[1] for i in gpts_wts])
             
                 kappa = np.array(
                     data.iloc[3+end_temps+int(2*self.ngauss/3):-2,0:3]
                         .astype(float)).ravel()[0:-1]
                 
                 kappa = np.reshape(kappa, 
                             (max_windows,self.ngauss*2,self.max_pc,self.max_tc),order='F')
@@ -1054,16 +1054,16 @@
             
 
                 assert self.ngauss == 8, 'Legacy code uses 8 gauss points not {0}. Check read in statements'.format(self.ngauss)
 
                 gpts_wts = np.reshape(np.array(data.iloc[end_temps+1:2+end_temps+int(2*self.ngauss/3),0:3]
                  .astype(float)).ravel()[1:-1], (self.ngauss,2))
                 
-                self.gauss_pts = [i[0] for i in gpts_wts]
-                self.gauss_wts = [i[1] for i in gpts_wts]
+                self.gauss_pts = np.array([i[0] for i in gpts_wts])
+                self.gauss_wts = np.array([i[1] for i in gpts_wts])
             
                 kappa = np.array(
                     data.iloc[3+end_temps+int(2*self.ngauss/3):-2,0:3]
                         .astype(float)).ravel()[0:-2]
                 
                 kappa = np.reshape(kappa, 
                             (max_windows,self.ngauss*2,self.max_pc,self.max_tc),order='F')
@@ -1084,15 +1084,15 @@
         Function to read the legacy data of the 1060 grid computed by Roxana Lupu. 
         Note
         ----
         This function is **highly** sensitive to the file format. You cannot edit the ascii file and then 
         run this function. Each specific line is accounted for.
         """
         data = pd.read_csv(os.path.join(self.ck_filename,'ascii_data'), 
-                  delim_whitespace=True,header=None, 
+                  sep='\s+',header=None, 
                   names=list(range(9)),dtype=str)
 
         num_species = int(data.iloc[0,0])
         max_ele = 35 
         self.max_tc = 73 
         self.max_pc = 20
         max_windows = 200 
@@ -1143,16 +1143,16 @@
         self.ngauss = int(data.iloc[end_temps+1,1])
 
         assert self.ngauss == 8, 'Legacy code uses 8 gauss points not {0}. Check read in statements'.format(self.ngauss)
 
         gpts_wts = np.reshape(np.array(data.iloc[end_temps+1:2+end_temps+int(2*self.ngauss/3),0:3]
          .astype(float)).ravel()[2:], (self.ngauss,2))
 
-        self.gauss_pts = [i[0] for i in gpts_wts]
-        self.gauss_wts = [i[1] for i in gpts_wts]
+        self.gauss_pts = np.array([i[0] for i in gpts_wts])
+        self.gauss_wts = np.array([i[1] for i in gpts_wts])
         
         
         #finally add pressure/temperature scale to abundances
         self.full_abunds['pressure']= self.pressures[self.pressures>0]
         self.full_abunds['temperature'] = np.concatenate([[i]*max(self.nc_p) for i in self.temps])[self.pressures>0]
 
 
@@ -1396,26 +1396,36 @@
         else:
             mix_vo =   ( bundle.inputs['atmosphere']['profile']['VO'].values)*0.0
         
         if 'FeH' in gases_fly:
             mix_feh =   ( bundle.inputs['atmosphere']['profile']['FeH'].values)
         else:
             mix_feh =   ( bundle.inputs['atmosphere']['profile']['FeH'].values)*0.0
+        
+        if 'SO2' in gases_fly:
+            mix_so2 =   ( bundle.inputs['atmosphere']['profile']['SO2'].values)
+        else:
+            mix_so2 =   ( bundle.inputs['atmosphere']['profile']['H2O'].values)*0.0
+
+        if 'H2S' in gases_fly:
+            mix_h2s =   ( bundle.inputs['atmosphere']['profile']['H2S'].values)
+        else:
+            mix_h2s =   ( bundle.inputs['atmosphere']['profile']['H2O'].values)*0.0
 
                 
         
 
         indices, t_interp,p_interp = self.get_mixing_indices(atmosphere) # gets nearest neighbor indices
 
         # Mix all opacities in the four nearest neighbors of your T(P) profile
         # these nearest neighbors will be used for interpolation
         kappa_mixed = mix_all_gases_gasesfly(np.array(self.kappa_co),np.array(self.kappa_h2o),np.array(self.kappa_ch4),
                                     np.array(self.kappa_nh3),np.array(self.kappa_co2),np.array(self.kappa_n2),np.array(self.kappa_hcn),
-                                    np.array(self.kappa_h2),np.array(self.kappa_ph3),np.array(self.kappa_c2h2),np.array(self.kappa_na),np.array(self.kappa_k),np.array(self.kappa_tio),np.array(self.kappa_vo),np.array(self.kappa_feh),mix_co,mix_h2o,mix_ch4,mix_nh3,
-                                    mix_co2,mix_n2,mix_hcn,mix_h2,mix_ph3,mix_c2h2,mix_na,mix_k,mix_tio,mix_vo,mix_feh,
+                                    np.array(self.kappa_h2),np.array(self.kappa_ph3),np.array(self.kappa_c2h2),np.array(self.kappa_na),np.array(self.kappa_k),np.array(self.kappa_tio),np.array(self.kappa_vo),np.array(self.kappa_feh),np.array(self.kappa_so2),np.array(self.kappa_h2s),mix_co,mix_h2o,mix_ch4,mix_nh3,
+                                    mix_co2,mix_n2,mix_hcn,mix_h2,mix_ph3,mix_c2h2,mix_na,mix_k,mix_tio,mix_vo,mix_feh, mix_so2,mix_h2s,
                                     np.array(self.gauss_pts),np.array(self.gauss_wts),indices)
         kappa = np.zeros(shape=(len(mix_co)-1,self.nwno,self.ngauss))
         
         # now perform the old nearest neighbor interpolation to produce final opacities
         for i in range(len(mix_co)-1):
             kappa[i,:,:] = (((1-t_interp[i])* (1-p_interp[i]) * kappa_mixed[i,:,:,0]) +
                         ((t_interp[i])  * (1-p_interp[i]) * kappa_mixed[i,:,:,1]) + 
@@ -1493,15 +1503,15 @@
 
         
         t_interp = ((t_inv - t_inv_low) / (t_inv_hi - t_inv_low))#[:,np.newaxis,np.newaxis]
         p_interp = ((p_log - p_log_low) / (p_log_hi - p_log_low))#[:,np.newaxis,np.newaxis]
         
         #now get associated pressures 
         #p_log_low =  np.array([p_log_grid[i] for i in p_low_ind])
-        return [p_low_ind, p_hi_ind, t_low_ind, t_hi_ind], t_interp,p_interp
+        return np.array([p_low_ind, p_hi_ind, t_low_ind, t_hi_ind]), t_interp,p_interp
             
     def get_pre_mix_ck_nearest(self,atmosphere):
         """
         Takes in atmosphere profile and returns an array which is 
         nlayer by ngauss by nwno
         """
         nlayer =atmosphere.c.nlayer
@@ -1928,14 +1938,28 @@
         if 'FeH' in gases_fly:
             array = np.load(path+'/FeH_1460.npy')
             self.kappa_feh = array
         else:
             array = np.load(path+'/FeH_1460.npy')
             self.kappa_feh = array*0-250.0
         
+        if 'SO2' in gases_fly:
+            array = np.load(path+'/SO2_1460.npy')
+            self.kappa_so2 = array
+        else:
+            array = np.load(path+'/SO2_1460.npy')
+            self.kappa_so2 = array*0-250.0
+
+        if 'H2S' in gases_fly:
+            array = np.load(path+'/H2S_1460.npy')
+            self.kappa_h2s = array
+        else:
+            array = np.load(path+'/H2S_1460.npy')
+            self.kappa_h2s = array*0-250.0
+        
     def get_new_wvno_grid_661(self):
         path = os.path.join(__refdata__, 'climate_INPUTS/')#'/Users/sagnickmukherjee/Documents/GitHub/Disequilibrium-Picaso/reference/climate_INPUTS/'
         wvno_new,dwni_new = np.loadtxt(path+"wvno_661",usecols=[0,1],unpack=True)
         self.wno = wvno_new
         self.delta_wno = dwni_new
         self.nwno = len(wvno_new)
 
@@ -2227,26 +2251,26 @@
     get_opacities 
         Gets opacities after user specifies atmospheric profile (e.g. full PT and Composition)
     """
     def __init__(self, db_filename, raman_data, wave_range=None,location = 'local',resample=1):
 
         #monochromatic opacity option forces number of gauss points to 1
         self.ngauss = 1
-        self.gauss_wts = [1]
+        self.gauss_wts = np.array([1])
 
         if location == 'local':
             #self.conn = sqlite3.connect(db_filename, detect_types=sqlite3.PARSE_DECLTYPES)
             self.db_filename = db_filename
             self.db_connect = self.open_local
 
         self.get_available_data(wave_range, resample)
         
         #raman cross sections 
         self.raman_db = pd.read_csv(raman_data,
-                     delim_whitespace=True, skiprows=16,header=None, names=['ji','jf','vf','c','deltanu'])
+                     sep='\s+', skiprows=16,header=None, names=['ji','jf','vf','c','deltanu'])
         
         #compute available Rayleigh scatterers 
         self.get_available_rayleigh()
 
         self.preload=False
 
     def open_local(self):
```

### Comparing `picaso-3.1.2/picaso/phasecurves.py` & `picaso-3.2/picaso/phasecurves.py`

 * *Files identical despite different names*

### Comparing `picaso-3.1.2/picaso/rayleigh.py` & `picaso-3.2/picaso/rayleigh.py`

 * *Files identical despite different names*

### Comparing `picaso-3.1.2/picaso/references.py` & `picaso-3.2/picaso/references.py`

 * *Files 8% similar despite different names*

```diff
@@ -1,26 +1,20 @@
 import bibtexparser
-from bibtexparser.bibdatabase import BibDatabase
-from bibtexparser.bwriter import BibTexWriter
 import os
 import json 
 import numpy as np
 
 class References(): 
     """
     Class structure to get references from PICASO
     """
     def __init__(self): 
         bibfile = os.path.join(os.environ['picaso_refdata'],'references','references.bib')
         reflist = os.path.join(os.environ['picaso_refdata'],'references','reference_list.json')
-
-        with open(bibfile,'r') as bibtex_file:
-            #bib_database = bibtexparser.load(bibtex_file,common_strings=True)
-            bib_database=bibtexparser.bparser.BibTexParser(
-            common_strings=True).parse_file(bibtex_file)
+        bib_database = bibtexparser.parse_file(bibfile)
         self.bib_dict = {i['ID']:i for i in bib_database.entries}
         self.reflist = json.load(open(reflist))         
 
     def get_opa(self, full_output=None, molecules=[]):
         """
         Get opacities references based on full output or a list of molecules 
 
@@ -93,26 +87,24 @@
                 i_ids=','.join(all_opacity_refs_ids[imol])
                 all_ids += all_opacity_refs_ids[imol]
 
             opa_tex += opa_tex_mid.replace('ID',i_ids).replace('molXX',imol)
 
         opa_tex = opa_tex_start+opa_tex+opa_tex_end
 
-        bibdb = BibDatabase()
-        bibdb.entries = [self.bib_dict[ID] for ID in all_ids]
-
+        bibdb = bibtexparser.Library()
+        for ID in all_ids:
+            bibdb.add(self.bib_dict[ID])
         return opa_tex, bibdb
 
 def create_bib(bibdb, filename):
     """
     Creates bib file 
     
     Parameters
     ----------
     bibdb : bibtexparser.bibdatabase.BibDatabase
         bib database 
     file : str 
         filename
     """
-    writer = BibTexWriter()
-    with open(filename, 'w') as bibfile:
-        bibfile.write(writer.write(bibdb))
+    bibtexparser.write_file(filename, bibdb)
```

### Comparing `picaso-3.1.2/picaso/run_opa_factory.py` & `picaso-3.2/picaso/run_opa_factory.py`

 * *Files identical despite different names*

### Comparing `picaso-3.1.2/picaso/test.py` & `picaso-3.2/picaso/test.py`

 * *Files 2% similar despite different names*

```diff
@@ -6,15 +6,28 @@
 import numpy as np
 from .justdoit import opannection, inputs, brown_dwarf_pt,brown_dwarf_cld
 import os 
 import astropy.units as u
 
 __refdata__ = os.environ.get('picaso_refdata')
 
+def test_it_all(): 
+	#reflected 1d 
 
+	#thermal 1d 
+
+	#reflected 3d 
+
+	#thermal 3d 
+
+	#climate tests 
+
+	#transit 1d 
+	return 
+	
 def thermal_sh_test(single_phase = 'OTHG', output_dir = None, 
 	phase=True, method="toon", stream=2, toon_coefficients="quadrature", delta_eddington=True,
 	disort_data=False, phangle=0, tau=0.2):
 	"""
 	Generate data to compare against DISORT. Must also run picaso_compare.py in pyDISORT
 	Parameters
 	----------
```

### Comparing `picaso-3.1.2/picaso/test_optics.py` & `picaso-3.2/picaso/test_optics.py`

 * *Files identical despite different names*

### Comparing `picaso-3.1.2/picaso/wavelength.py` & `picaso-3.2/picaso/wavelength.py`

 * *Files 8% similar despite different names*

```diff
@@ -24,21 +24,21 @@
 	array 
 		array of wave numbers in increasing order 
 	"""
 	if grid661 == True:
 		grid,dwni_new = np.loadtxt(os.path.join(__refdata__, 'climate_INPUTS/wvno_661'),usecols=[0,1],unpack=True)
 		return grid
 	if filename_or_grid == 'wave_EGP.dat':
-		grid = pd.read_csv(os.path.join(__refdata__, 'opacities',filename_or_grid), delim_whitespace=True)
+		grid = pd.read_csv(os.path.join(__refdata__, 'opacities',filename_or_grid), sep='\s+')
 		grid = grid.sort_values('wavenumber')['wavenumber'].values
 	elif isinstance(filename_or_grid, np.ndarray):
 		grid = np.sort(filename_or_grid)
 	elif (isinstance(filename_or_grid, str) & (filename_or_grid != 'wave_EGP.dat') & 
 		os.path.exists(filename_or_grid)):	
-		grid = pd.read_csv(os.path.join(filename_or_grid), delim_whitespace=True)
+		grid = pd.read_csv(os.path.join(filename_or_grid), sep='\s+')
 		if 'wavenumber' in grid.keys():
 			grid = grid.sort_values('wavenumber')['wavenumber'].values
 		else: 
 			raise Exception('Please make sure there is a column named "wavenumber" in your cloud wavegrid file')
 	else:
 		raise Exception("Please enter valid cloud wavegrid filepath, or numpy array. Or use default in reference file.")
```

### Comparing `picaso-3.1.2/picaso.egg-info/SOURCES.txt` & `picaso-3.2/picaso.egg-info/SOURCES.txt`

 * *Files 19% similar despite different names*

```diff
@@ -14,20 +14,20 @@
 picaso/fluxes.py
 picaso/io_utils.py
 picaso/justdoit.py
 picaso/justplotit.py
 picaso/opacity_factory.py
 picaso/optics.py
 picaso/phasecurves.py
+picaso/photochem.py
 picaso/rayleigh.py
 picaso/references.py
 picaso/run_opa_factory.py
 picaso/test.py
 picaso/test_optics.py
-picaso/vulcan.py
 picaso/wavelength.py
 picaso.egg-info/PKG-INFO
 picaso.egg-info/SOURCES.txt
 picaso.egg-info/dependency_links.txt
 picaso.egg-info/not-zip-safe
 picaso.egg-info/requires.txt
 picaso.egg-info/top_level.txt
```

### Comparing `picaso-3.1.2/setup.cfg` & `picaso-3.2/setup.cfg`

 * *Files identical despite different names*

### Comparing `picaso-3.1.2/setup.py` & `picaso-3.2/setup.py`

 * *Files 3% similar despite different names*

```diff
@@ -37,15 +37,15 @@
 # from the setup.cfg file.
 #
 # use_2to3 and zip_safe are common options support by setuptools; these can
 # also be placed in the setup.cfg, as will be demonstrated in a future update
 # to this sample package.
 setup(
     name='picaso', 
-    version = '3.1.2',
+    version = '3.2',
     description = 'planetary intesity code for atmospheric scattering observations',
     long_description = 'README.md',
     author = 'Natasha E. Batalha',
     author_email = 'natasha.e.batalha@gmail.com',
     url = 'https://natashabatalha.github.io/picaso',
     license = 'GPL-3.0',
     download_url = 'https://github.com/natashabatalha/picaso',
@@ -56,26 +56,26 @@
                   'Programming Language :: Python',
                   'Programming Language :: Python :: 3',
                   'Topic :: Scientific/Engineering :: Astronomy',
                   'Topic :: Software Development :: Libraries :: Python Modules'
   ],
   packages=['picaso'],
   install_requires=[
-          'numpy<1.25',
-          'bokeh>=2.3.0,<3.1.0',
-          'holoviews',
+          'bokeh>=2.3.0,<3.5.0',
+          'numpy<1.27',
           'numba',
           'pandas',
           'joblib',
           'photutils',
           'astropy>=3.2.3',
           'matplotlib',
           'pysynphot',
           'sphinx',
           'scipy',
-          'virga-exo',
+          'virga-exo==0.4',
           'xarray',
           'bibtexparser',
-          'dynesty'
+          'netcdf4', 
+          'h5netcdf'
           ], 
     zip_safe = False,
 )
```

