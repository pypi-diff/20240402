# Comparing `tmp/algokit-2.0.1-py3-none-any.whl.zip` & `tmp/algokit-2.0.2-py3-none-any.whl.zip`

## zipinfo {}

```diff
@@ -1,8 +1,8 @@
-Zip file size: 125670 bytes, number of entries: 73
+Zip file size: 125728 bytes, number of entries: 73
 -rw-r--r--  2.0 unx     1183 b- defN 80-Jan-01 00:00 algokit/__init__.py
 -rw-r--r--  2.0 unx      184 b- defN 80-Jan-01 00:00 algokit/__main__.py
 -rw-r--r--  2.0 unx     2392 b- defN 80-Jan-01 00:00 algokit/cli/__init__.py
 -rw-r--r--  2.0 unx        0 b- defN 80-Jan-01 00:00 algokit/cli/common/__init__.py
 -rw-r--r--  2.0 unx      796 b- defN 80-Jan-01 00:00 algokit/cli/common/constants.py
 -rw-r--r--  2.0 unx     5236 b- defN 80-Jan-01 00:00 algokit/cli/common/utils.py
 -rw-r--r--  2.0 unx     1310 b- defN 80-Jan-01 00:00 algokit/cli/compile.py
@@ -63,13 +63,13 @@
 -rw-r--r--  2.0 unx     5600 b- defN 80-Jan-01 00:00 algokit/core/tasks/vanity_address.py
 -rw-r--r--  2.0 unx     4870 b- defN 80-Jan-01 00:00 algokit/core/tasks/wallet.py
 -rw-r--r--  2.0 unx    11074 b- defN 80-Jan-01 00:00 algokit/core/typed_client_generation.py
 -rw-r--r--  2.0 unx     9525 b- defN 80-Jan-01 00:00 algokit/core/utils.py
 -rw-r--r--  2.0 unx     6020 b- defN 80-Jan-01 00:00 algokit/core/version_prompt.py
 -rw-r--r--  2.0 unx        0 b- defN 80-Jan-01 00:00 algokit/py.typed
 -rw-r--r--  2.0 unx        0 b- defN 80-Jan-01 00:00 algokit/resources/distribution-method
--rw-r--r--  2.0 unx     1081 b- defN 80-Jan-01 00:00 algokit-2.0.1.dist-info/LICENSE
--rw-r--r--  2.0 unx    15323 b- defN 80-Jan-01 00:00 algokit-2.0.1.dist-info/METADATA
--rw-r--r--  2.0 unx       88 b- defN 80-Jan-01 00:00 algokit-2.0.1.dist-info/WHEEL
--rw-r--r--  2.0 unx       47 b- defN 80-Jan-01 00:00 algokit-2.0.1.dist-info/entry_points.txt
-?rw-r--r--  2.0 unx     6080 b- defN 16-Jan-01 00:00 algokit-2.0.1.dist-info/RECORD
-73 files, 368484 bytes uncompressed, 116106 bytes compressed:  68.5%
+-rw-r--r--  2.0 unx     1081 b- defN 80-Jan-01 00:00 algokit-2.0.2.dist-info/LICENSE
+-rw-r--r--  2.0 unx    15477 b- defN 80-Jan-01 00:00 algokit-2.0.2.dist-info/METADATA
+-rw-r--r--  2.0 unx       88 b- defN 80-Jan-01 00:00 algokit-2.0.2.dist-info/WHEEL
+-rw-r--r--  2.0 unx       47 b- defN 80-Jan-01 00:00 algokit-2.0.2.dist-info/entry_points.txt
+?rw-r--r--  2.0 unx     6080 b- defN 16-Jan-01 00:00 algokit-2.0.2.dist-info/RECORD
+73 files, 368638 bytes uncompressed, 116164 bytes compressed:  68.5%
```

## zipnote {}

```diff
@@ -198,23 +198,23 @@
 
 Filename: algokit/py.typed
 Comment: 
 
 Filename: algokit/resources/distribution-method
 Comment: 
 
-Filename: algokit-2.0.1.dist-info/LICENSE
+Filename: algokit-2.0.2.dist-info/LICENSE
 Comment: 
 
-Filename: algokit-2.0.1.dist-info/METADATA
+Filename: algokit-2.0.2.dist-info/METADATA
 Comment: 
 
-Filename: algokit-2.0.1.dist-info/WHEEL
+Filename: algokit-2.0.2.dist-info/WHEEL
 Comment: 
 
-Filename: algokit-2.0.1.dist-info/entry_points.txt
+Filename: algokit-2.0.2.dist-info/entry_points.txt
 Comment: 
 
-Filename: algokit-2.0.1.dist-info/RECORD
+Filename: algokit-2.0.2.dist-info/RECORD
 Comment: 
 
 Zip file comment:
```

## Comparing `algokit-2.0.1.dist-info/LICENSE` & `algokit-2.0.2.dist-info/LICENSE`

 * *Files identical despite different names*

## Comparing `algokit-2.0.1.dist-info/METADATA` & `algokit-2.0.2.dist-info/METADATA`

 * *Files 2% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: algokit
-Version: 2.0.1
+Version: 2.0.2
 Summary: Algorand development kit command-line interface
 License: MIT
 Author: Algorand Foundation
 Author-email: contact@algorand.foundation
 Requires-Python: >=3.10,<3.13
 Classifier: License :: OSI Approved :: MIT License
 Classifier: Programming Language :: Python :: 3
@@ -21,14 +21,15 @@
 Requires-Dist: keyring (==24.3.0)
 Requires-Dist: mslex (>=1.1.0,<2.0.0)
 Requires-Dist: multiformats (==0.3.1)
 Requires-Dist: multiformats_config (==0.3.1)
 Requires-Dist: pyclip (>=0.7.0,<0.8.0)
 Requires-Dist: pyjwt (>=2.8.0,<3.0.0)
 Requires-Dist: python-dotenv (>=1.0.0,<2.0.0)
+Requires-Dist: pyyaml-include (==1.4.1)
 Requires-Dist: questionary (>=1.10.0,<2.0.0)
 Requires-Dist: shellingham (>=1.5.0.post1,<2.0.0)
 Requires-Dist: tomli (>=2.0.1,<3.0.0) ; python_version < "3.11"
 Description-Content-Type: text/markdown
 
 <div align="center">
 <a href="https://github.com/algorandfoundation/algokit-cli"><img src="https://bafybeihfrtfg4vcufkcqmrtslkhx737ppz2fgn2lnctsd6waduqhhhibye.ipfs.nftstorage.link/" width=60%></a>
@@ -119,14 +120,15 @@
 AlgoKit also has some runtime dependencies that also need to be available for particular commands.
 
 > **Note**
 > You can still install and use AlgoKit without these dependencies and AlgoKit will tell you if you are missing one for a given command.
 
 - Git - Git is used when creating and updating projects from templates
 - Docker - Docker Compose (and by association, Docker) is used to run the AlgoKit LocalNet environment, we require Docker Compose 2.5.0+
+- (Optional) Node.js - Node.js is used for frontend templates, or if you want to build contracts using TEALScript
 
 ## Cross-platform installation
 
 AlgoKit can be installed using OS specific package managers, or using the python tool [pipx](https://pypa.github.io/pipx/) see below for specific installation instructions.
 
 - [Windows](#install-algokit-on-windows)
 - [Mac](#install-algokit-on-mac)
```

### html2text {}

```diff
@@ -1,24 +1,25 @@
-Metadata-Version: 2.1 Name: algokit Version: 2.0.1 Summary: Algorand
+Metadata-Version: 2.1 Name: algokit Version: 2.0.2 Summary: Algorand
 development kit command-line interface License: MIT Author: Algorand Foundation
 Author-email: contact@algorand.foundation Requires-Python: >=3.10,<3.13
 Classifier: License :: OSI Approved :: MIT License Classifier: Programming
 Language :: Python :: 3 Classifier: Programming Language :: Python :: 3.10
 Classifier: Programming Language :: Python :: 3.11 Classifier: Programming
 Language :: Python :: 3.12 Requires-Dist: aiohttp (==3.9.3) Requires-Dist:
 algokit-utils (>=2.2.1,<3.0.0) Requires-Dist: auth0-python (>=4.4.0,<5.0.0)
 Requires-Dist: click (>=8.1.3,<9.0.0) Requires-Dist: copier (>=9.0.0,<10.0.0)
 Requires-Dist: httpx (>=0.23.1,<0.24.0) Requires-Dist: jsondiff
 (>=2.0.0,<3.0.0) Requires-Dist: keyring (==24.3.0) Requires-Dist: mslex
 (>=1.1.0,<2.0.0) Requires-Dist: multiformats (==0.3.1) Requires-Dist:
 multiformats_config (==0.3.1) Requires-Dist: pyclip (>=0.7.0,<0.8.0) Requires-
 Dist: pyjwt (>=2.8.0,<3.0.0) Requires-Dist: python-dotenv (>=1.0.0,<2.0.0)
-Requires-Dist: questionary (>=1.10.0,<2.0.0) Requires-Dist: shellingham
-(>=1.5.0.post1,<2.0.0) Requires-Dist: tomli (>=2.0.1,<3.0.0) ; python_version <
-"3.11" Description-Content-Type: text/markdown
+Requires-Dist: pyyaml-include (==1.4.1) Requires-Dist: questionary
+(>=1.10.0,<2.0.0) Requires-Dist: shellingham (>=1.5.0.post1,<2.0.0) Requires-
+Dist: tomli (>=2.0.1,<3.0.0) ; python_version < "3.11" Description-Content-
+Type: text/markdown
                                    _[_h_t_t_p_s_:_/_/
 _b_a_f_y_b_e_i_h_f_r_t_f_g_4_v_c_u_f_k_c_q_m_r_t_s_l_k_h_x_7_3_7_p_p_z_2_f_g_n_2_l_n_c_t_s_d_6_w_a_d_u_q_h_h_h_i_b_y_e_._i_p_f_s_._n_f_t_s_t_o_r_a_g_e_._l_i_n_k_/
                                        _]
                 _[_h_t_t_p_s_:_/_/_i_m_g_._s_h_i_e_l_d_s_._i_o_/_b_a_d_g_e_/_d_o_c_s_-_r_e_p_o_s_i_t_o_r_y_-
 _0_0_d_c_9_4_?_l_o_g_o_=_g_i_t_h_u_b_&_s_t_y_l_e_=_f_l_a_t_._s_v_g_]_[_h_t_t_p_s_:_/_/_i_m_g_._s_h_i_e_l_d_s_._i_o_/_b_a_d_g_e_/_l_e_a_r_n_-_A_l_g_o_K_i_t_-
     _0_0_d_c_9_4_?_l_o_g_o_=_a_l_g_o_r_a_n_d_&_m_a_c_=_f_l_a_t_._s_v_g_]_[_h_t_t_p_s_:_/_/_i_m_g_._s_h_i_e_l_d_s_._i_o_/_g_i_t_h_u_b_/_s_t_a_r_s_/
   _a_l_g_o_r_a_n_d_f_o_u_n_d_a_t_i_o_n_/_a_l_g_o_k_i_t_-_c_l_i_?_c_o_l_o_r_=_0_0_d_c_9_4_&_l_o_g_o_=_s_t_a_r_&_s_t_y_l_e_=_f_l_a_t_]_[_h_t_t_p_s_:_/_/
@@ -111,87 +112,88 @@
 below will install that for you. We recommend using Python 3.12+, as the
 `algokit compile python` command requires this version. AlgoKit also has some
 runtime dependencies that also need to be available for particular commands. >
 **Note** > You can still install and use AlgoKit without these dependencies and
 AlgoKit will tell you if you are missing one for a given command. - Git - Git
 is used when creating and updating projects from templates - Docker - Docker
 Compose (and by association, Docker) is used to run the AlgoKit LocalNet
-environment, we require Docker Compose 2.5.0+ ## Cross-platform installation
-AlgoKit can be installed using OS specific package managers, or using the
-python tool [pipx](https://pypa.github.io/pipx/) see below for specific
-installation instructions. - [Windows](#install-algokit-on-windows) - [Mac]
-(#install-algokit-on-mac) - [Linux](#install-algokit-on-linux) - [pipx]
-(#install-algokit-with-pipx-on-any-os) ## Install AlgoKit on Windows > **Note**
-> This method will install the most recent python3 version [via winget](https:/
-/learn.microsoft.com/en-us/windows/package-manager/winget/). If you already
-have python 3.10+ installed, you may [prefer to use pipx directly instead]
-(#install-algokit-with-pipx-on-any-os) so you can control the python version
-used. 1. Ensure prerequisites are installed - [Git](https://github.com/git-
-guides/install-git#install-git-on-windows) (or `winget install git.git`) -
-[Docker](https://docs.docker.com/desktop/install/windows-install/) (or `winget
-install docker.dockerdesktop`) > **Note** > See [our LocalNet documentation]
-(https://github.com/algorandfoundation/algokit-cli/blob/main/docs/features/
-localnet.md#prerequisites) for more tips on installing Docker on Windows 2.
-Install using WinGet 1. Install python: `winget install python.python.3.11` 2.
-Restart the terminal to ensure Python and pip are available on the path >
-**Note** > Windows has a feature called **App Execution Aliases** that provides
-redirects for the Python command that guide users to the > Windows Store.
-Unfortunately these aliases can prevent normal execution of Python if Python is
-installed via other means, to disable them > search for **Manage app execution
-aliases** from the start menu, and then turn off entries listed as > **App
-Installer python.exe** or **App Installer python3.exe**. 3. Install pipx: ```
-pip install --user pipx python -m pipx ensurepath ``` 4. Restart the terminal
-to ensure pipx is available on the path 5. Install AlgoKit via pipx: `pipx
-install algokit` 6. Restart the terminal to ensure AlgoKit is available on the
-path 3. [Verify installation](#verify-installation) ### Maintenance Some useful
-commands for updating or removing AlgoKit in the future. - To update AlgoKit:
-`pipx upgrade algokit` - To remove AlgoKit: `pipx uninstall algokit` ## Install
-AlgoKit on Mac > **Note** > This method will install Python 3.10 as a
-dependency via Homebrew. If you already have python installed, you may prefer
-to use `pipx install algokit` as explained [here](#install-algokit-with-pipx-
-on-any-os). 1. Ensure prerequisites are installed - [Homebrew](https://
-docs.brew.sh/Installation) - [Git](https://github.com/git-guides/install-
-git#install-git-on-mac) (should already be available if `brew` is installed) -
-[Docker](https://docs.docker.com/desktop/install/mac-install/), (or `brew
-install --cask docker`) > **Note** > Docker requires MacOS 11+ 2. Install using
-Homebrew `brew install algorandfoundation/tap/algokit` 3. Restart the terminal
-to ensure AlgoKit is available on the path 4. [Verify installation](#verify-
-installation) ### Maintenance Some useful commands for updating or removing
-AlgoKit in the future. - To update AlgoKit: `brew upgrade algokit` - To remove
-AlgoKit: `brew uninstall algokit` ## Install AlgoKit on Linux 1. Ensure
-prerequisites are installed - [Python 3.10+](https://www.python.org/downloads/
-) > **Note** > There is probably a better way to install Python than to
-download it directly, e.g. your local Linux package manager - [pipx](https://
-pypa.github.io/pipx/#on-linux-install-via-pip-requires-pip-190-or-later) -
-[Git](https://github.com/git-guides/install-git#install-git-on-linux) -
-[Docker](https://docs.docker.com/desktop/install/linux-install/) 2. Continue
-with step 2 in the following section to install via [pipx](#install-algokit-
-with-pipx-on-any-os) ## Install AlgoKit with pipx on any OS 1. Ensure desired
-prerequisites are installed - [Python 3.10+](https://www.python.org/downloads/
-) - [pipx](https://pypa.github.io/pipx/installation/) - [Git](https://
-github.com/git-guides/install-git) - [Docker](https://docs.docker.com/get-
-docker/) 2. Install using pipx `pipx install algokit` 3. Restart the terminal
-to ensure AlgoKit is available on the path 4. [Verify installation](#verify-
-installation) ### Maintenance Some useful commands for updating or removing
-AlgoKit in the future. - To update AlgoKit: `pipx upgrade algokit` - To remove
-AlgoKit: `pipx uninstall algokit` ## Verify installation Verify AlgoKit is
-installed correctly by running `algokit --version` and you should see output
-similar to: ``` algokit, version 1.0.1 ``` > **Note** > If you get receive one
-of the following errors: > > - `command not found: algokit` (bash/zsh) > - `The
-term 'algokit' is not recognized as the name of a cmdlet, function, script
-file, or operable program.` (PowerShell) > > Then ensure that `algokit` is
-available on the PATH by running `pipx ensurepath` and restarting the terminal.
-It is also recommended that you run `algokit doctor` to verify there are no
-issues in your local environment and to diagnose any problems if you do have
-difficulties running AlgoKit. The output of this command will look similar to:
-``` timestamp: 2023-03-27T01:23:45+00:00 AlgoKit: 1.0.1 AlgoKit Python: 3.11.1
-(main, Dec 23 2022, 09:28:24) [Clang 14.0.0 (clang-1400.0.29.202)] (location: /
-Users/algokit/.local/pipx/venvs/algokit) OS: macOS-13.1-arm64-arm-64bit docker:
-20.10.21 docker compose: 2.13.0 git: 2.37.1 python: 3.10.9 (location: /opt/
-homebrew/bin/python) python3: 3.10.9 (location: /opt/homebrew/bin/python3)
-pipx: 1.1.0 poetry: 1.3.2 node: 18.12.1 npm: 8.19.2 brew: 3.6.18 If you are
-experiencing a problem with AlgoKit, feel free to submit an issue via: https://
-github.com/algorandfoundation/algokit-cli/issues/new Please include this
-output, if you want to populate this message in your clipboard, run `algokit
-doctor -c` ``` Per the above output, the doctor command output is a helpful
-tool if you need to ask for support or [raise an issue](https://github.com/
-algorandfoundation/algokit-cli/issues/new).
+environment, we require Docker Compose 2.5.0+ - (Optional) Node.js - Node.js is
+used for frontend templates, or if you want to build contracts using TEALScript
+## Cross-platform installation AlgoKit can be installed using OS specific
+package managers, or using the python tool [pipx](https://pypa.github.io/pipx/
+) see below for specific installation instructions. - [Windows](#install-
+algokit-on-windows) - [Mac](#install-algokit-on-mac) - [Linux](#install-
+algokit-on-linux) - [pipx](#install-algokit-with-pipx-on-any-os) ## Install
+AlgoKit on Windows > **Note** > This method will install the most recent
+python3 version [via winget](https://learn.microsoft.com/en-us/windows/package-
+manager/winget/). If you already have python 3.10+ installed, you may [prefer
+to use pipx directly instead](#install-algokit-with-pipx-on-any-os) so you can
+control the python version used. 1. Ensure prerequisites are installed - [Git]
+(https://github.com/git-guides/install-git#install-git-on-windows) (or `winget
+install git.git`) - [Docker](https://docs.docker.com/desktop/install/windows-
+install/) (or `winget install docker.dockerdesktop`) > **Note** > See [our
+LocalNet documentation](https://github.com/algorandfoundation/algokit-cli/blob/
+main/docs/features/localnet.md#prerequisites) for more tips on installing
+Docker on Windows 2. Install using WinGet 1. Install python: `winget install
+python.python.3.11` 2. Restart the terminal to ensure Python and pip are
+available on the path > **Note** > Windows has a feature called **App Execution
+Aliases** that provides redirects for the Python command that guide users to
+the > Windows Store. Unfortunately these aliases can prevent normal execution
+of Python if Python is installed via other means, to disable them > search for
+**Manage app execution aliases** from the start menu, and then turn off entries
+listed as > **App Installer python.exe** or **App Installer python3.exe**. 3.
+Install pipx: ``` pip install --user pipx python -m pipx ensurepath ``` 4.
+Restart the terminal to ensure pipx is available on the path 5. Install AlgoKit
+via pipx: `pipx install algokit` 6. Restart the terminal to ensure AlgoKit is
+available on the path 3. [Verify installation](#verify-installation) ###
+Maintenance Some useful commands for updating or removing AlgoKit in the
+future. - To update AlgoKit: `pipx upgrade algokit` - To remove AlgoKit: `pipx
+uninstall algokit` ## Install AlgoKit on Mac > **Note** > This method will
+install Python 3.10 as a dependency via Homebrew. If you already have python
+installed, you may prefer to use `pipx install algokit` as explained [here]
+(#install-algokit-with-pipx-on-any-os). 1. Ensure prerequisites are installed -
+[Homebrew](https://docs.brew.sh/Installation) - [Git](https://github.com/git-
+guides/install-git#install-git-on-mac) (should already be available if `brew`
+is installed) - [Docker](https://docs.docker.com/desktop/install/mac-install/),
+(or `brew install --cask docker`) > **Note** > Docker requires MacOS 11+ 2.
+Install using Homebrew `brew install algorandfoundation/tap/algokit` 3. Restart
+the terminal to ensure AlgoKit is available on the path 4. [Verify
+installation](#verify-installation) ### Maintenance Some useful commands for
+updating or removing AlgoKit in the future. - To update AlgoKit: `brew upgrade
+algokit` - To remove AlgoKit: `brew uninstall algokit` ## Install AlgoKit on
+Linux 1. Ensure prerequisites are installed - [Python 3.10+](https://
+www.python.org/downloads/) > **Note** > There is probably a better way to
+install Python than to download it directly, e.g. your local Linux package
+manager - [pipx](https://pypa.github.io/pipx/#on-linux-install-via-pip-
+requires-pip-190-or-later) - [Git](https://github.com/git-guides/install-
+git#install-git-on-linux) - [Docker](https://docs.docker.com/desktop/install/
+linux-install/) 2. Continue with step 2 in the following section to install via
+[pipx](#install-algokit-with-pipx-on-any-os) ## Install AlgoKit with pipx on
+any OS 1. Ensure desired prerequisites are installed - [Python 3.10+](https://
+www.python.org/downloads/) - [pipx](https://pypa.github.io/pipx/installation/
+) - [Git](https://github.com/git-guides/install-git) - [Docker](https://
+docs.docker.com/get-docker/) 2. Install using pipx `pipx install algokit` 3.
+Restart the terminal to ensure AlgoKit is available on the path 4. [Verify
+installation](#verify-installation) ### Maintenance Some useful commands for
+updating or removing AlgoKit in the future. - To update AlgoKit: `pipx upgrade
+algokit` - To remove AlgoKit: `pipx uninstall algokit` ## Verify installation
+Verify AlgoKit is installed correctly by running `algokit --version` and you
+should see output similar to: ``` algokit, version 1.0.1 ``` > **Note** > If
+you get receive one of the following errors: > > - `command not found: algokit`
+(bash/zsh) > - `The term 'algokit' is not recognized as the name of a cmdlet,
+function, script file, or operable program.` (PowerShell) > > Then ensure that
+`algokit` is available on the PATH by running `pipx ensurepath` and restarting
+the terminal. It is also recommended that you run `algokit doctor` to verify
+there are no issues in your local environment and to diagnose any problems if
+you do have difficulties running AlgoKit. The output of this command will look
+similar to: ``` timestamp: 2023-03-27T01:23:45+00:00 AlgoKit: 1.0.1 AlgoKit
+Python: 3.11.1 (main, Dec 23 2022, 09:28:24) [Clang 14.0.0 (clang-
+1400.0.29.202)] (location: /Users/algokit/.local/pipx/venvs/algokit) OS: macOS-
+13.1-arm64-arm-64bit docker: 20.10.21 docker compose: 2.13.0 git: 2.37.1
+python: 3.10.9 (location: /opt/homebrew/bin/python) python3: 3.10.9 (location:
+/opt/homebrew/bin/python3) pipx: 1.1.0 poetry: 1.3.2 node: 18.12.1 npm: 8.19.2
+brew: 3.6.18 If you are experiencing a problem with AlgoKit, feel free to
+submit an issue via: https://github.com/algorandfoundation/algokit-cli/issues/
+new Please include this output, if you want to populate this message in your
+clipboard, run `algokit doctor -c` ``` Per the above output, the doctor command
+output is a helpful tool if you need to ask for support or [raise an issue]
+(https://github.com/algorandfoundation/algokit-cli/issues/new).
```

## Comparing `algokit-2.0.1.dist-info/RECORD` & `algokit-2.0.2.dist-info/RECORD`

 * *Files 3% similar despite different names*

```diff
@@ -62,12 +62,12 @@
 algokit/core/tasks/vanity_address.py,sha256=rz7H_4-KGfURrEaC2P4S5sX2rBZSKZoloHywdjBDEFk,5600
 algokit/core/tasks/wallet.py,sha256=mdh0EkA-UREJrLxpcKTKYl5C-g9JZ2GoNG3G4RlqiAo,4870
 algokit/core/typed_client_generation.py,sha256=hXy1dHqWaGX6W3Qwx6O3o9lnLqcphR0lkqnKqDldeSo,11074
 algokit/core/utils.py,sha256=5QijArArCN1BcRZjP17OjH9z42dUyckojdT953mEXug,9525
 algokit/core/version_prompt.py,sha256=viInWjxyS71vqjZtXNvqrIr-oYxL9YsU9UDAA6mq9xs,6020
 algokit/py.typed,sha256=47DEQpj8HBSa-_TImW-5JCeuQeRkm5NMpJWZG3hSuFU,0
 algokit/resources/distribution-method,sha256=47DEQpj8HBSa-_TImW-5JCeuQeRkm5NMpJWZG3hSuFU,0
-algokit-2.0.1.dist-info/LICENSE,sha256=CPjn5HTZL3VUJ8E1lxtdBx6SLzNnQlOoezdFYom9R24,1081
-algokit-2.0.1.dist-info/METADATA,sha256=-KeLUtfOIeSWz1SSWmKVaQCzrgbCTBsrWUsPXPAUWt4,15323
-algokit-2.0.1.dist-info/WHEEL,sha256=sP946D7jFCHeNz5Iq4fL4Lu-PrWrFsgfLXbbkciIZwg,88
-algokit-2.0.1.dist-info/entry_points.txt,sha256=JJtH-iaVJa6YUrN69B7AMycsg9-q6OwV52olGIU65rc,47
-algokit-2.0.1.dist-info/RECORD,,
+algokit-2.0.2.dist-info/LICENSE,sha256=CPjn5HTZL3VUJ8E1lxtdBx6SLzNnQlOoezdFYom9R24,1081
+algokit-2.0.2.dist-info/METADATA,sha256=NaPNZ7gUUctaRn4kIHK6lMdUmJvl_z4oVK15QGuKThA,15477
+algokit-2.0.2.dist-info/WHEEL,sha256=sP946D7jFCHeNz5Iq4fL4Lu-PrWrFsgfLXbbkciIZwg,88
+algokit-2.0.2.dist-info/entry_points.txt,sha256=JJtH-iaVJa6YUrN69B7AMycsg9-q6OwV52olGIU65rc,47
+algokit-2.0.2.dist-info/RECORD,,
```

