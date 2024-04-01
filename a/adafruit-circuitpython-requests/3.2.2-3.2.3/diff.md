# Comparing `tmp/adafruit-circuitpython-requests-3.2.2.tar.gz` & `tmp/adafruit-circuitpython-requests-3.2.3.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "adafruit-circuitpython-requests-3.2.2.tar", last modified: Mon Mar 18 16:33:00 2024, max compression
+gzip compressed data, was "adafruit-circuitpython-requests-3.2.3.tar", last modified: Mon Apr  1 22:43:26 2024, max compression
```

## Comparing `adafruit-circuitpython-requests-3.2.2.tar` & `adafruit-circuitpython-requests-3.2.3.tar`

### file list

```diff
@@ -1,89 +1,89 @@
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-03-18 16:33:00.489318 adafruit-circuitpython-requests-3.2.2/
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-03-18 16:33:00.477318 adafruit-circuitpython-requests-3.2.2/.github/
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-03-18 16:33:00.481318 adafruit-circuitpython-requests-3.2.2/.github/PULL_REQUEST_TEMPLATE/
--rw-r--r--   0 runner    (1001) docker     (127)      880 2024-03-18 16:32:49.000000 adafruit-circuitpython-requests-3.2.2/.github/PULL_REQUEST_TEMPLATE/adafruit_circuitpython_pr.md
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-03-18 16:33:00.481318 adafruit-circuitpython-requests-3.2.2/.github/workflows/
--rw-r--r--   0 runner    (1001) docker     (127)      303 2024-03-18 16:32:49.000000 adafruit-circuitpython-requests-3.2.2/.github/workflows/build.yml
--rw-r--r--   0 runner    (1001) docker     (127)      479 2024-03-18 16:32:49.000000 adafruit-circuitpython-requests-3.2.2/.github/workflows/failure-help-text.yml
--rw-r--r--   0 runner    (1001) docker     (127)      482 2024-03-18 16:32:49.000000 adafruit-circuitpython-requests-3.2.2/.github/workflows/release_gh.yml
--rw-r--r--   0 runner    (1001) docker     (127)      475 2024-03-18 16:32:49.000000 adafruit-circuitpython-requests-3.2.2/.github/workflows/release_pypi.yml
--rwxr-xr-x   0 runner    (1001) docker     (127)     1724 2024-03-18 16:32:49.000000 adafruit-circuitpython-requests-3.2.2/.gitignore
--rw-r--r--   0 runner    (1001) docker     (127)     1430 2024-03-18 16:32:49.000000 adafruit-circuitpython-requests-3.2.2/.pre-commit-config.yaml
--rw-r--r--   0 runner    (1001) docker     (127)    13078 2024-03-18 16:32:49.000000 adafruit-circuitpython-requests-3.2.2/.pylintrc
--rw-r--r--   0 runner    (1001) docker     (127)      388 2024-03-18 16:32:49.000000 adafruit-circuitpython-requests-3.2.2/.readthedocs.yaml
--rwxr-xr-x   0 runner    (1001) docker     (127)     6147 2024-03-18 16:32:49.000000 adafruit-circuitpython-requests-3.2.2/CODE_OF_CONDUCT.md
--rwxr-xr-x   0 runner    (1001) docker     (127)     1098 2024-03-18 16:32:49.000000 adafruit-circuitpython-requests-3.2.2/LICENSE
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-03-18 16:33:00.481318 adafruit-circuitpython-requests-3.2.2/LICENSES/
--rw-r--r--   0 runner    (1001) docker     (127)    16814 2024-03-18 16:32:49.000000 adafruit-circuitpython-requests-3.2.2/LICENSES/CC-BY-4.0.txt
--rw-r--r--   0 runner    (1001) docker     (127)     1108 2024-03-18 16:32:49.000000 adafruit-circuitpython-requests-3.2.2/LICENSES/MIT.txt
--rw-r--r--   0 runner    (1001) docker     (127)     1211 2024-03-18 16:32:49.000000 adafruit-circuitpython-requests-3.2.2/LICENSES/Unlicense.txt
--rw-r--r--   0 runner    (1001) docker     (127)     3483 2024-03-18 16:33:00.489318 adafruit-circuitpython-requests-3.2.2/PKG-INFO
--rwxr-xr-x   0 runner    (1001) docker     (127)     2642 2024-03-18 16:32:49.000000 adafruit-circuitpython-requests-3.2.2/README.rst
--rw-r--r--   0 runner    (1001) docker     (127)      108 2024-03-18 16:32:49.000000 adafruit-circuitpython-requests-3.2.2/README.rst.license
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-03-18 16:33:00.489318 adafruit-circuitpython-requests-3.2.2/adafruit_circuitpython_requests.egg-info/
--rw-r--r--   0 runner    (1001) docker     (127)     3483 2024-03-18 16:33:00.000000 adafruit-circuitpython-requests-3.2.2/adafruit_circuitpython_requests.egg-info/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (127)     2482 2024-03-18 16:33:00.000000 adafruit-circuitpython-requests-3.2.2/adafruit_circuitpython_requests.egg-info/SOURCES.txt
--rw-r--r--   0 runner    (1001) docker     (127)        1 2024-03-18 16:33:00.000000 adafruit-circuitpython-requests-3.2.2/adafruit_circuitpython_requests.egg-info/dependency_links.txt
--rw-r--r--   0 runner    (1001) docker     (127)       69 2024-03-18 16:33:00.000000 adafruit-circuitpython-requests-3.2.2/adafruit_circuitpython_requests.egg-info/requires.txt
--rw-r--r--   0 runner    (1001) docker     (127)       18 2024-03-18 16:33:00.000000 adafruit-circuitpython-requests-3.2.2/adafruit_circuitpython_requests.egg-info/top_level.txt
--rw-r--r--   0 runner    (1001) docker     (127)    21346 2024-03-18 16:32:57.000000 adafruit-circuitpython-requests-3.2.2/adafruit_requests.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-03-18 16:33:00.485318 adafruit-circuitpython-requests-3.2.2/docs/
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-03-18 16:33:00.485318 adafruit-circuitpython-requests-3.2.2/docs/_static/
--rwxr-xr-x   0 runner    (1001) docker     (127)     4414 2024-03-18 16:32:49.000000 adafruit-circuitpython-requests-3.2.2/docs/_static/favicon.ico
--rw-r--r--   0 runner    (1001) docker     (127)      105 2024-03-18 16:32:49.000000 adafruit-circuitpython-requests-3.2.2/docs/_static/favicon.ico.license
--rwxr-xr-x   0 runner    (1001) docker     (127)      267 2024-03-18 16:32:49.000000 adafruit-circuitpython-requests-3.2.2/docs/api.rst
--rw-r--r--   0 runner    (1001) docker     (127)       96 2024-03-18 16:32:49.000000 adafruit-circuitpython-requests-3.2.2/docs/api.rst.license
--rwxr-xr-x   0 runner    (1001) docker     (127)     5400 2024-03-18 16:32:49.000000 adafruit-circuitpython-requests-3.2.2/docs/conf.py
--rwxr-xr-x   0 runner    (1001) docker     (127)      803 2024-03-18 16:32:49.000000 adafruit-circuitpython-requests-3.2.2/docs/examples.rst
--rw-r--r--   0 runner    (1001) docker     (127)       96 2024-03-18 16:32:49.000000 adafruit-circuitpython-requests-3.2.2/docs/examples.rst.license
--rwxr-xr-x   0 runner    (1001) docker     (127)      973 2024-03-18 16:32:49.000000 adafruit-circuitpython-requests-3.2.2/docs/index.rst
--rw-r--r--   0 runner    (1001) docker     (127)       96 2024-03-18 16:32:49.000000 adafruit-circuitpython-requests-3.2.2/docs/index.rst.license
--rw-r--r--   0 runner    (1001) docker     (127)      154 2024-03-18 16:32:49.000000 adafruit-circuitpython-requests-3.2.2/docs/requirements.txt
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-03-18 16:33:00.477318 adafruit-circuitpython-requests-3.2.2/examples/
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-03-18 16:33:00.485318 adafruit-circuitpython-requests-3.2.2/examples/cpython/
--rw-r--r--   0 runner    (1001) docker     (127)      837 2024-03-18 16:32:57.000000 adafruit-circuitpython-requests-3.2.2/examples/cpython/requests_cpython_advanced.py
--rw-r--r--   0 runner    (1001) docker     (127)     1412 2024-03-18 16:32:57.000000 adafruit-circuitpython-requests-3.2.2/examples/cpython/requests_cpython_simpletest.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-03-18 16:33:00.485318 adafruit-circuitpython-requests-3.2.2/examples/esp32spi/
--rw-r--r--   0 runner    (1001) docker     (127)     2163 2024-03-18 16:32:57.000000 adafruit-circuitpython-requests-3.2.2/examples/esp32spi/requests_esp32spi_advanced.py
--rw-r--r--   0 runner    (1001) docker     (127)     2738 2024-03-18 16:32:57.000000 adafruit-circuitpython-requests-3.2.2/examples/esp32spi/requests_esp32spi_simpletest.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-03-18 16:33:00.485318 adafruit-circuitpython-requests-3.2.2/examples/fona/
--rw-r--r--   0 runner    (1001) docker     (127)     1984 2024-03-18 16:32:57.000000 adafruit-circuitpython-requests-3.2.2/examples/fona/requests_fona_advanced.py
--rw-r--r--   0 runner    (1001) docker     (127)     2558 2024-03-18 16:32:57.000000 adafruit-circuitpython-requests-3.2.2/examples/fona/requests_fona_simpletest.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-03-18 16:33:00.485318 adafruit-circuitpython-requests-3.2.2/examples/wifi/
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-03-18 16:33:00.489318 adafruit-circuitpython-requests-3.2.2/examples/wifi/expanded/
--rw-r--r--   0 runner    (1001) docker     (127)     2965 2024-03-18 16:32:57.000000 adafruit-circuitpython-requests-3.2.2/examples/wifi/expanded/requests_wifi_adafruit_discord_active_online.py
--rw-r--r--   0 runner    (1001) docker     (127)     3470 2024-03-18 16:32:57.000000 adafruit-circuitpython-requests-3.2.2/examples/wifi/expanded/requests_wifi_api_discord.py
--rw-r--r--   0 runner    (1001) docker     (127)    15754 2024-03-18 16:32:57.000000 adafruit-circuitpython-requests-3.2.2/examples/wifi/expanded/requests_wifi_api_fitbit.py
--rw-r--r--   0 runner    (1001) docker     (127)     3317 2024-03-18 16:32:57.000000 adafruit-circuitpython-requests-3.2.2/examples/wifi/expanded/requests_wifi_api_github.py
--rw-r--r--   0 runner    (1001) docker     (127)     4261 2024-03-18 16:32:57.000000 adafruit-circuitpython-requests-3.2.2/examples/wifi/expanded/requests_wifi_api_mastodon.py
--rw-r--r--   0 runner    (1001) docker     (127)     5611 2024-03-18 16:32:57.000000 adafruit-circuitpython-requests-3.2.2/examples/wifi/expanded/requests_wifi_api_openskynetwork_private.py
--rw-r--r--   0 runner    (1001) docker     (127)     6850 2024-03-18 16:32:57.000000 adafruit-circuitpython-requests-3.2.2/examples/wifi/expanded/requests_wifi_api_openskynetwork_private_area.py
--rw-r--r--   0 runner    (1001) docker     (127)     4982 2024-03-18 16:32:57.000000 adafruit-circuitpython-requests-3.2.2/examples/wifi/expanded/requests_wifi_api_openskynetwork_public.py
--rw-r--r--   0 runner    (1001) docker     (127)     2797 2024-03-18 16:32:57.000000 adafruit-circuitpython-requests-3.2.2/examples/wifi/expanded/requests_wifi_api_premiereleague.py
--rw-r--r--   0 runner    (1001) docker     (127)     4543 2024-03-18 16:32:57.000000 adafruit-circuitpython-requests-3.2.2/examples/wifi/expanded/requests_wifi_api_rocketlaunch_live.py
--rw-r--r--   0 runner    (1001) docker     (127)     4157 2024-03-18 16:32:57.000000 adafruit-circuitpython-requests-3.2.2/examples/wifi/expanded/requests_wifi_api_steam.py
--rw-r--r--   0 runner    (1001) docker     (127)     6340 2024-03-18 16:32:57.000000 adafruit-circuitpython-requests-3.2.2/examples/wifi/expanded/requests_wifi_api_twitch.py
--rw-r--r--   0 runner    (1001) docker     (127)     3940 2024-03-18 16:32:57.000000 adafruit-circuitpython-requests-3.2.2/examples/wifi/expanded/requests_wifi_api_twitter.py
--rw-r--r--   0 runner    (1001) docker     (127)     3947 2024-03-18 16:32:57.000000 adafruit-circuitpython-requests-3.2.2/examples/wifi/expanded/requests_wifi_api_youtube.py
--rw-r--r--   0 runner    (1001) docker     (127)     1703 2024-03-18 16:32:57.000000 adafruit-circuitpython-requests-3.2.2/examples/wifi/expanded/requests_wifi_multiple_cookies.py
--rw-r--r--   0 runner    (1001) docker     (127)     1446 2024-03-18 16:32:57.000000 adafruit-circuitpython-requests-3.2.2/examples/wifi/requests_wifi_advanced.py
--rw-r--r--   0 runner    (1001) docker     (127)     2021 2024-03-18 16:32:57.000000 adafruit-circuitpython-requests-3.2.2/examples/wifi/requests_wifi_simpletest.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-03-18 16:33:00.489318 adafruit-circuitpython-requests-3.2.2/examples/wiznet5k/
--rw-r--r--   0 runner    (1001) docker     (127)     1241 2024-03-18 16:32:57.000000 adafruit-circuitpython-requests-3.2.2/examples/wiznet5k/requests_wiznet5k_advanced.py
--rw-r--r--   0 runner    (1001) docker     (127)     1815 2024-03-18 16:32:57.000000 adafruit-circuitpython-requests-3.2.2/examples/wiznet5k/requests_wiznet5k_simpletest.py
--rw-r--r--   0 runner    (1001) docker     (127)      108 2024-03-18 16:32:49.000000 adafruit-circuitpython-requests-3.2.2/optional_requirements.txt
--rw-r--r--   0 runner    (1001) docker     (127)     1209 2024-03-18 16:32:57.000000 adafruit-circuitpython-requests-3.2.2/pyproject.toml
--rwxr-xr-x   0 runner    (1001) docker     (127)      166 2024-03-18 16:32:49.000000 adafruit-circuitpython-requests-3.2.2/requirements.txt
--rw-r--r--   0 runner    (1001) docker     (127)       38 2024-03-18 16:33:00.489318 adafruit-circuitpython-requests-3.2.2/setup.cfg
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-03-18 16:33:00.489318 adafruit-circuitpython-requests-3.2.2/tests/
--rw-r--r--   0 runner    (1001) docker     (127)     4007 2024-03-18 16:32:57.000000 adafruit-circuitpython-requests-3.2.2/tests/chunk_test.py
--rw-r--r--   0 runner    (1001) docker     (127)    10156 2024-03-18 16:32:57.000000 adafruit-circuitpython-requests-3.2.2/tests/chunked_redirect_test.py
--rw-r--r--   0 runner    (1001) docker     (127)     2625 2024-03-18 16:32:57.000000 adafruit-circuitpython-requests-3.2.2/tests/concurrent_test.py
--rw-r--r--   0 runner    (1001) docker     (127)     1028 2024-03-18 16:32:57.000000 adafruit-circuitpython-requests-3.2.2/tests/conftest.py
--rw-r--r--   0 runner    (1001) docker     (127)     3063 2024-03-18 16:32:57.000000 adafruit-circuitpython-requests-3.2.2/tests/header_test.py
--rw-r--r--   0 runner    (1001) docker     (127)     2244 2024-03-18 16:32:57.000000 adafruit-circuitpython-requests-3.2.2/tests/method_test.py
--rw-r--r--   0 runner    (1001) docker     (127)     3068 2024-03-18 16:32:57.000000 adafruit-circuitpython-requests-3.2.2/tests/mocket.py
--rw-r--r--   0 runner    (1001) docker     (127)      923 2024-03-18 16:32:57.000000 adafruit-circuitpython-requests-3.2.2/tests/parse_test.py
--rw-r--r--   0 runner    (1001) docker     (127)     2314 2024-03-18 16:32:57.000000 adafruit-circuitpython-requests-3.2.2/tests/protocol_test.py
--rw-r--r--   0 runner    (1001) docker     (127)     6399 2024-03-18 16:32:57.000000 adafruit-circuitpython-requests-3.2.2/tests/reuse_test.py
--rw-r--r--   0 runner    (1001) docker     (127)      785 2024-03-18 16:32:49.000000 adafruit-circuitpython-requests-3.2.2/tox.ini
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-01 22:43:26.605120 adafruit-circuitpython-requests-3.2.3/
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-01 22:43:26.593120 adafruit-circuitpython-requests-3.2.3/.github/
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-01 22:43:26.597120 adafruit-circuitpython-requests-3.2.3/.github/PULL_REQUEST_TEMPLATE/
+-rw-r--r--   0 runner    (1001) docker     (127)      880 2024-04-01 22:43:17.000000 adafruit-circuitpython-requests-3.2.3/.github/PULL_REQUEST_TEMPLATE/adafruit_circuitpython_pr.md
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-01 22:43:26.597120 adafruit-circuitpython-requests-3.2.3/.github/workflows/
+-rw-r--r--   0 runner    (1001) docker     (127)      303 2024-04-01 22:43:17.000000 adafruit-circuitpython-requests-3.2.3/.github/workflows/build.yml
+-rw-r--r--   0 runner    (1001) docker     (127)      479 2024-04-01 22:43:17.000000 adafruit-circuitpython-requests-3.2.3/.github/workflows/failure-help-text.yml
+-rw-r--r--   0 runner    (1001) docker     (127)      482 2024-04-01 22:43:17.000000 adafruit-circuitpython-requests-3.2.3/.github/workflows/release_gh.yml
+-rw-r--r--   0 runner    (1001) docker     (127)      475 2024-04-01 22:43:17.000000 adafruit-circuitpython-requests-3.2.3/.github/workflows/release_pypi.yml
+-rwxr-xr-x   0 runner    (1001) docker     (127)     1724 2024-04-01 22:43:17.000000 adafruit-circuitpython-requests-3.2.3/.gitignore
+-rw-r--r--   0 runner    (1001) docker     (127)     1430 2024-04-01 22:43:17.000000 adafruit-circuitpython-requests-3.2.3/.pre-commit-config.yaml
+-rw-r--r--   0 runner    (1001) docker     (127)    13078 2024-04-01 22:43:17.000000 adafruit-circuitpython-requests-3.2.3/.pylintrc
+-rw-r--r--   0 runner    (1001) docker     (127)      388 2024-04-01 22:43:17.000000 adafruit-circuitpython-requests-3.2.3/.readthedocs.yaml
+-rwxr-xr-x   0 runner    (1001) docker     (127)     6147 2024-04-01 22:43:17.000000 adafruit-circuitpython-requests-3.2.3/CODE_OF_CONDUCT.md
+-rwxr-xr-x   0 runner    (1001) docker     (127)     1098 2024-04-01 22:43:17.000000 adafruit-circuitpython-requests-3.2.3/LICENSE
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-01 22:43:26.597120 adafruit-circuitpython-requests-3.2.3/LICENSES/
+-rw-r--r--   0 runner    (1001) docker     (127)    16814 2024-04-01 22:43:17.000000 adafruit-circuitpython-requests-3.2.3/LICENSES/CC-BY-4.0.txt
+-rw-r--r--   0 runner    (1001) docker     (127)     1108 2024-04-01 22:43:17.000000 adafruit-circuitpython-requests-3.2.3/LICENSES/MIT.txt
+-rw-r--r--   0 runner    (1001) docker     (127)     1211 2024-04-01 22:43:17.000000 adafruit-circuitpython-requests-3.2.3/LICENSES/Unlicense.txt
+-rw-r--r--   0 runner    (1001) docker     (127)     3483 2024-04-01 22:43:26.605120 adafruit-circuitpython-requests-3.2.3/PKG-INFO
+-rwxr-xr-x   0 runner    (1001) docker     (127)     2642 2024-04-01 22:43:17.000000 adafruit-circuitpython-requests-3.2.3/README.rst
+-rw-r--r--   0 runner    (1001) docker     (127)      108 2024-04-01 22:43:17.000000 adafruit-circuitpython-requests-3.2.3/README.rst.license
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-01 22:43:26.605120 adafruit-circuitpython-requests-3.2.3/adafruit_circuitpython_requests.egg-info/
+-rw-r--r--   0 runner    (1001) docker     (127)     3483 2024-04-01 22:43:26.000000 adafruit-circuitpython-requests-3.2.3/adafruit_circuitpython_requests.egg-info/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (127)     2482 2024-04-01 22:43:26.000000 adafruit-circuitpython-requests-3.2.3/adafruit_circuitpython_requests.egg-info/SOURCES.txt
+-rw-r--r--   0 runner    (1001) docker     (127)        1 2024-04-01 22:43:26.000000 adafruit-circuitpython-requests-3.2.3/adafruit_circuitpython_requests.egg-info/dependency_links.txt
+-rw-r--r--   0 runner    (1001) docker     (127)       69 2024-04-01 22:43:26.000000 adafruit-circuitpython-requests-3.2.3/adafruit_circuitpython_requests.egg-info/requires.txt
+-rw-r--r--   0 runner    (1001) docker     (127)       18 2024-04-01 22:43:26.000000 adafruit-circuitpython-requests-3.2.3/adafruit_circuitpython_requests.egg-info/top_level.txt
+-rw-r--r--   0 runner    (1001) docker     (127)    21346 2024-04-01 22:43:24.000000 adafruit-circuitpython-requests-3.2.3/adafruit_requests.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-01 22:43:26.597120 adafruit-circuitpython-requests-3.2.3/docs/
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-01 22:43:26.601120 adafruit-circuitpython-requests-3.2.3/docs/_static/
+-rwxr-xr-x   0 runner    (1001) docker     (127)     4414 2024-04-01 22:43:17.000000 adafruit-circuitpython-requests-3.2.3/docs/_static/favicon.ico
+-rw-r--r--   0 runner    (1001) docker     (127)      105 2024-04-01 22:43:17.000000 adafruit-circuitpython-requests-3.2.3/docs/_static/favicon.ico.license
+-rwxr-xr-x   0 runner    (1001) docker     (127)      267 2024-04-01 22:43:17.000000 adafruit-circuitpython-requests-3.2.3/docs/api.rst
+-rw-r--r--   0 runner    (1001) docker     (127)       96 2024-04-01 22:43:17.000000 adafruit-circuitpython-requests-3.2.3/docs/api.rst.license
+-rwxr-xr-x   0 runner    (1001) docker     (127)     5400 2024-04-01 22:43:17.000000 adafruit-circuitpython-requests-3.2.3/docs/conf.py
+-rwxr-xr-x   0 runner    (1001) docker     (127)      803 2024-04-01 22:43:17.000000 adafruit-circuitpython-requests-3.2.3/docs/examples.rst
+-rw-r--r--   0 runner    (1001) docker     (127)       96 2024-04-01 22:43:17.000000 adafruit-circuitpython-requests-3.2.3/docs/examples.rst.license
+-rwxr-xr-x   0 runner    (1001) docker     (127)      973 2024-04-01 22:43:17.000000 adafruit-circuitpython-requests-3.2.3/docs/index.rst
+-rw-r--r--   0 runner    (1001) docker     (127)       96 2024-04-01 22:43:17.000000 adafruit-circuitpython-requests-3.2.3/docs/index.rst.license
+-rw-r--r--   0 runner    (1001) docker     (127)      154 2024-04-01 22:43:17.000000 adafruit-circuitpython-requests-3.2.3/docs/requirements.txt
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-01 22:43:26.593120 adafruit-circuitpython-requests-3.2.3/examples/
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-01 22:43:26.601120 adafruit-circuitpython-requests-3.2.3/examples/cpython/
+-rw-r--r--   0 runner    (1001) docker     (127)      837 2024-04-01 22:43:24.000000 adafruit-circuitpython-requests-3.2.3/examples/cpython/requests_cpython_advanced.py
+-rw-r--r--   0 runner    (1001) docker     (127)     1412 2024-04-01 22:43:24.000000 adafruit-circuitpython-requests-3.2.3/examples/cpython/requests_cpython_simpletest.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-01 22:43:26.601120 adafruit-circuitpython-requests-3.2.3/examples/esp32spi/
+-rw-r--r--   0 runner    (1001) docker     (127)     2163 2024-04-01 22:43:24.000000 adafruit-circuitpython-requests-3.2.3/examples/esp32spi/requests_esp32spi_advanced.py
+-rw-r--r--   0 runner    (1001) docker     (127)     2738 2024-04-01 22:43:24.000000 adafruit-circuitpython-requests-3.2.3/examples/esp32spi/requests_esp32spi_simpletest.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-01 22:43:26.601120 adafruit-circuitpython-requests-3.2.3/examples/fona/
+-rw-r--r--   0 runner    (1001) docker     (127)     1984 2024-04-01 22:43:24.000000 adafruit-circuitpython-requests-3.2.3/examples/fona/requests_fona_advanced.py
+-rw-r--r--   0 runner    (1001) docker     (127)     2558 2024-04-01 22:43:24.000000 adafruit-circuitpython-requests-3.2.3/examples/fona/requests_fona_simpletest.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-01 22:43:26.601120 adafruit-circuitpython-requests-3.2.3/examples/wifi/
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-01 22:43:26.605120 adafruit-circuitpython-requests-3.2.3/examples/wifi/expanded/
+-rw-r--r--   0 runner    (1001) docker     (127)     2934 2024-04-01 22:43:24.000000 adafruit-circuitpython-requests-3.2.3/examples/wifi/expanded/requests_wifi_adafruit_discord_active_online.py
+-rw-r--r--   0 runner    (1001) docker     (127)     3439 2024-04-01 22:43:24.000000 adafruit-circuitpython-requests-3.2.3/examples/wifi/expanded/requests_wifi_api_discord.py
+-rw-r--r--   0 runner    (1001) docker     (127)    15732 2024-04-01 22:43:24.000000 adafruit-circuitpython-requests-3.2.3/examples/wifi/expanded/requests_wifi_api_fitbit.py
+-rw-r--r--   0 runner    (1001) docker     (127)     3286 2024-04-01 22:43:24.000000 adafruit-circuitpython-requests-3.2.3/examples/wifi/expanded/requests_wifi_api_github.py
+-rw-r--r--   0 runner    (1001) docker     (127)     4230 2024-04-01 22:43:24.000000 adafruit-circuitpython-requests-3.2.3/examples/wifi/expanded/requests_wifi_api_mastodon.py
+-rw-r--r--   0 runner    (1001) docker     (127)     5611 2024-04-01 22:43:24.000000 adafruit-circuitpython-requests-3.2.3/examples/wifi/expanded/requests_wifi_api_openskynetwork_private.py
+-rw-r--r--   0 runner    (1001) docker     (127)     6850 2024-04-01 22:43:24.000000 adafruit-circuitpython-requests-3.2.3/examples/wifi/expanded/requests_wifi_api_openskynetwork_private_area.py
+-rw-r--r--   0 runner    (1001) docker     (127)     4982 2024-04-01 22:43:24.000000 adafruit-circuitpython-requests-3.2.3/examples/wifi/expanded/requests_wifi_api_openskynetwork_public.py
+-rw-r--r--   0 runner    (1001) docker     (127)     2766 2024-04-01 22:43:24.000000 adafruit-circuitpython-requests-3.2.3/examples/wifi/expanded/requests_wifi_api_premiereleague.py
+-rw-r--r--   0 runner    (1001) docker     (127)     5223 2024-04-01 22:43:24.000000 adafruit-circuitpython-requests-3.2.3/examples/wifi/expanded/requests_wifi_api_rocketlaunch_live.py
+-rw-r--r--   0 runner    (1001) docker     (127)     4126 2024-04-01 22:43:24.000000 adafruit-circuitpython-requests-3.2.3/examples/wifi/expanded/requests_wifi_api_steam.py
+-rw-r--r--   0 runner    (1001) docker     (127)     6309 2024-04-01 22:43:24.000000 adafruit-circuitpython-requests-3.2.3/examples/wifi/expanded/requests_wifi_api_twitch.py
+-rw-r--r--   0 runner    (1001) docker     (127)     3940 2024-04-01 22:43:24.000000 adafruit-circuitpython-requests-3.2.3/examples/wifi/expanded/requests_wifi_api_twitter.py
+-rw-r--r--   0 runner    (1001) docker     (127)     4048 2024-04-01 22:43:24.000000 adafruit-circuitpython-requests-3.2.3/examples/wifi/expanded/requests_wifi_api_youtube.py
+-rw-r--r--   0 runner    (1001) docker     (127)     1703 2024-04-01 22:43:24.000000 adafruit-circuitpython-requests-3.2.3/examples/wifi/expanded/requests_wifi_multiple_cookies.py
+-rw-r--r--   0 runner    (1001) docker     (127)     1446 2024-04-01 22:43:24.000000 adafruit-circuitpython-requests-3.2.3/examples/wifi/requests_wifi_advanced.py
+-rw-r--r--   0 runner    (1001) docker     (127)     2021 2024-04-01 22:43:24.000000 adafruit-circuitpython-requests-3.2.3/examples/wifi/requests_wifi_simpletest.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-01 22:43:26.605120 adafruit-circuitpython-requests-3.2.3/examples/wiznet5k/
+-rw-r--r--   0 runner    (1001) docker     (127)     1241 2024-04-01 22:43:24.000000 adafruit-circuitpython-requests-3.2.3/examples/wiznet5k/requests_wiznet5k_advanced.py
+-rw-r--r--   0 runner    (1001) docker     (127)     1815 2024-04-01 22:43:24.000000 adafruit-circuitpython-requests-3.2.3/examples/wiznet5k/requests_wiznet5k_simpletest.py
+-rw-r--r--   0 runner    (1001) docker     (127)      108 2024-04-01 22:43:17.000000 adafruit-circuitpython-requests-3.2.3/optional_requirements.txt
+-rw-r--r--   0 runner    (1001) docker     (127)     1209 2024-04-01 22:43:24.000000 adafruit-circuitpython-requests-3.2.3/pyproject.toml
+-rwxr-xr-x   0 runner    (1001) docker     (127)      166 2024-04-01 22:43:17.000000 adafruit-circuitpython-requests-3.2.3/requirements.txt
+-rw-r--r--   0 runner    (1001) docker     (127)       38 2024-04-01 22:43:26.605120 adafruit-circuitpython-requests-3.2.3/setup.cfg
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-01 22:43:26.605120 adafruit-circuitpython-requests-3.2.3/tests/
+-rw-r--r--   0 runner    (1001) docker     (127)     4007 2024-04-01 22:43:24.000000 adafruit-circuitpython-requests-3.2.3/tests/chunk_test.py
+-rw-r--r--   0 runner    (1001) docker     (127)    10156 2024-04-01 22:43:24.000000 adafruit-circuitpython-requests-3.2.3/tests/chunked_redirect_test.py
+-rw-r--r--   0 runner    (1001) docker     (127)     2625 2024-04-01 22:43:24.000000 adafruit-circuitpython-requests-3.2.3/tests/concurrent_test.py
+-rw-r--r--   0 runner    (1001) docker     (127)     1028 2024-04-01 22:43:24.000000 adafruit-circuitpython-requests-3.2.3/tests/conftest.py
+-rw-r--r--   0 runner    (1001) docker     (127)     3063 2024-04-01 22:43:24.000000 adafruit-circuitpython-requests-3.2.3/tests/header_test.py
+-rw-r--r--   0 runner    (1001) docker     (127)     2244 2024-04-01 22:43:24.000000 adafruit-circuitpython-requests-3.2.3/tests/method_test.py
+-rw-r--r--   0 runner    (1001) docker     (127)     3068 2024-04-01 22:43:24.000000 adafruit-circuitpython-requests-3.2.3/tests/mocket.py
+-rw-r--r--   0 runner    (1001) docker     (127)      923 2024-04-01 22:43:24.000000 adafruit-circuitpython-requests-3.2.3/tests/parse_test.py
+-rw-r--r--   0 runner    (1001) docker     (127)     2314 2024-04-01 22:43:24.000000 adafruit-circuitpython-requests-3.2.3/tests/protocol_test.py
+-rw-r--r--   0 runner    (1001) docker     (127)     6399 2024-04-01 22:43:24.000000 adafruit-circuitpython-requests-3.2.3/tests/reuse_test.py
+-rw-r--r--   0 runner    (1001) docker     (127)      785 2024-04-01 22:43:17.000000 adafruit-circuitpython-requests-3.2.3/tox.ini
```

### Comparing `adafruit-circuitpython-requests-3.2.2/.github/PULL_REQUEST_TEMPLATE/adafruit_circuitpython_pr.md` & `adafruit-circuitpython-requests-3.2.3/.github/PULL_REQUEST_TEMPLATE/adafruit_circuitpython_pr.md`

 * *Files identical despite different names*

### Comparing `adafruit-circuitpython-requests-3.2.2/.gitignore` & `adafruit-circuitpython-requests-3.2.3/.gitignore`

 * *Files identical despite different names*

### Comparing `adafruit-circuitpython-requests-3.2.2/.pre-commit-config.yaml` & `adafruit-circuitpython-requests-3.2.3/.pre-commit-config.yaml`

 * *Files identical despite different names*

### Comparing `adafruit-circuitpython-requests-3.2.2/.pylintrc` & `adafruit-circuitpython-requests-3.2.3/.pylintrc`

 * *Files identical despite different names*

### Comparing `adafruit-circuitpython-requests-3.2.2/CODE_OF_CONDUCT.md` & `adafruit-circuitpython-requests-3.2.3/CODE_OF_CONDUCT.md`

 * *Files identical despite different names*

### Comparing `adafruit-circuitpython-requests-3.2.2/LICENSE` & `adafruit-circuitpython-requests-3.2.3/LICENSE`

 * *Files identical despite different names*

### Comparing `adafruit-circuitpython-requests-3.2.2/LICENSES/CC-BY-4.0.txt` & `adafruit-circuitpython-requests-3.2.3/LICENSES/CC-BY-4.0.txt`

 * *Files identical despite different names*

### Comparing `adafruit-circuitpython-requests-3.2.2/LICENSES/MIT.txt` & `adafruit-circuitpython-requests-3.2.3/LICENSES/MIT.txt`

 * *Files identical despite different names*

### Comparing `adafruit-circuitpython-requests-3.2.2/LICENSES/Unlicense.txt` & `adafruit-circuitpython-requests-3.2.3/LICENSES/Unlicense.txt`

 * *Files identical despite different names*

### Comparing `adafruit-circuitpython-requests-3.2.2/PKG-INFO` & `adafruit-circuitpython-requests-3.2.3/PKG-INFO`

 * *Files 0% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: adafruit-circuitpython-requests
-Version: 3.2.2
+Version: 3.2.3
 Summary: A requests-like library for web interfacing
 Author-email: Adafruit Industries <circuitpython@adafruit.com>
 License: MIT
 Project-URL: Homepage, https://github.com/adafruit/Adafruit_CircuitPython_Requests
 Keywords: adafruit,blinka,circuitpython,micropython,requests,requests,,networking
 Classifier: Intended Audience :: Developers
 Classifier: Topic :: Software Development :: Libraries
```

### Comparing `adafruit-circuitpython-requests-3.2.2/README.rst` & `adafruit-circuitpython-requests-3.2.3/README.rst`

 * *Files identical despite different names*

### Comparing `adafruit-circuitpython-requests-3.2.2/adafruit_circuitpython_requests.egg-info/PKG-INFO` & `adafruit-circuitpython-requests-3.2.3/adafruit_circuitpython_requests.egg-info/PKG-INFO`

 * *Files 0% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: adafruit-circuitpython-requests
-Version: 3.2.2
+Version: 3.2.3
 Summary: A requests-like library for web interfacing
 Author-email: Adafruit Industries <circuitpython@adafruit.com>
 License: MIT
 Project-URL: Homepage, https://github.com/adafruit/Adafruit_CircuitPython_Requests
 Keywords: adafruit,blinka,circuitpython,micropython,requests,requests,,networking
 Classifier: Intended Audience :: Developers
 Classifier: Topic :: Software Development :: Libraries
```

### Comparing `adafruit-circuitpython-requests-3.2.2/adafruit_circuitpython_requests.egg-info/SOURCES.txt` & `adafruit-circuitpython-requests-3.2.3/adafruit_circuitpython_requests.egg-info/SOURCES.txt`

 * *Files identical despite different names*

### Comparing `adafruit-circuitpython-requests-3.2.2/adafruit_requests.py` & `adafruit-circuitpython-requests-3.2.3/adafruit_requests.py`

 * *Files 0% similar despite different names*

```diff
@@ -32,15 +32,15 @@
   https://github.com/adafruit/circuitpython/releases
 
 * Adafruit's Connection Manager library:
   https://github.com/adafruit/Adafruit_CircuitPython_ConnectionManager
 
 """
 
-__version__ = "3.2.2"
+__version__ = "3.2.3"
 __repo__ = "https://github.com/adafruit/Adafruit_CircuitPython_Requests.git"
 
 import errno
 import json as json_module
 import sys
 
 from adafruit_connection_manager import get_connection_manager
```

### Comparing `adafruit-circuitpython-requests-3.2.2/docs/_static/favicon.ico` & `adafruit-circuitpython-requests-3.2.3/docs/_static/favicon.ico`

 * *Files identical despite different names*

### Comparing `adafruit-circuitpython-requests-3.2.2/docs/conf.py` & `adafruit-circuitpython-requests-3.2.3/docs/conf.py`

 * *Files identical despite different names*

### Comparing `adafruit-circuitpython-requests-3.2.2/docs/examples.rst` & `adafruit-circuitpython-requests-3.2.3/docs/examples.rst`

 * *Files identical despite different names*

### Comparing `adafruit-circuitpython-requests-3.2.2/docs/index.rst` & `adafruit-circuitpython-requests-3.2.3/docs/index.rst`

 * *Files identical despite different names*

### Comparing `adafruit-circuitpython-requests-3.2.2/examples/cpython/requests_cpython_advanced.py` & `adafruit-circuitpython-requests-3.2.3/examples/cpython/requests_cpython_advanced.py`

 * *Files identical despite different names*

### Comparing `adafruit-circuitpython-requests-3.2.2/examples/cpython/requests_cpython_simpletest.py` & `adafruit-circuitpython-requests-3.2.3/examples/cpython/requests_cpython_simpletest.py`

 * *Files identical despite different names*

### Comparing `adafruit-circuitpython-requests-3.2.2/examples/esp32spi/requests_esp32spi_advanced.py` & `adafruit-circuitpython-requests-3.2.3/examples/esp32spi/requests_esp32spi_advanced.py`

 * *Files identical despite different names*

### Comparing `adafruit-circuitpython-requests-3.2.2/examples/esp32spi/requests_esp32spi_simpletest.py` & `adafruit-circuitpython-requests-3.2.3/examples/esp32spi/requests_esp32spi_simpletest.py`

 * *Files identical despite different names*

### Comparing `adafruit-circuitpython-requests-3.2.2/examples/fona/requests_fona_advanced.py` & `adafruit-circuitpython-requests-3.2.3/examples/fona/requests_fona_advanced.py`

 * *Files identical despite different names*

### Comparing `adafruit-circuitpython-requests-3.2.2/examples/fona/requests_fona_simpletest.py` & `adafruit-circuitpython-requests-3.2.3/examples/fona/requests_fona_simpletest.py`

 * *Files identical despite different names*

### Comparing `adafruit-circuitpython-requests-3.2.2/examples/wifi/expanded/requests_wifi_adafruit_discord_active_online.py` & `adafruit-circuitpython-requests-3.2.3/examples/wifi/expanded/requests_wifi_adafruit_discord_active_online.py`

 * *Files 5% similar despite different names*

```diff
@@ -1,12 +1,11 @@
 # SPDX-FileCopyrightText: 2024 DJDevon3
 # SPDX-License-Identifier: MIT
 # Coded for Circuit Python 8.2.x
 """Discord Active Online Shields.IO Example"""
-# pylint: disable=import-error
 
 import os
 import time
 
 import adafruit_connection_manager
 import wifi
```

### Comparing `adafruit-circuitpython-requests-3.2.2/examples/wifi/expanded/requests_wifi_api_discord.py` & `adafruit-circuitpython-requests-3.2.3/examples/wifi/expanded/requests_wifi_api_discord.py`

 * *Files 11% similar despite different names*

```diff
@@ -1,12 +1,11 @@
 # SPDX-FileCopyrightText: 2024 DJDevon3
 # SPDX-License-Identifier: MIT
 # Coded for Circuit Python 8.2.x
 """Discord Web Scrape Example"""
-# pylint: disable=import-error
 
 import os
 import time
 
 import adafruit_connection_manager
 import wifi
```

### Comparing `adafruit-circuitpython-requests-3.2.2/examples/wifi/expanded/requests_wifi_api_fitbit.py` & `adafruit-circuitpython-requests-3.2.3/examples/wifi/expanded/requests_wifi_api_fitbit.py`

 * *Files 0% similar despite different names*

```diff
@@ -1,12 +1,12 @@
 # SPDX-FileCopyrightText: 2024 DJDevon3
 # SPDX-License-Identifier: MIT
 # Coded for Circuit Python 8.2.x
 """Fitbit API Example"""
-# pylint: disable=import-error, disable=no-member
+# pylint: disable=no-member
 
 import os
 import time
 
 import adafruit_connection_manager
 import microcontroller
 import wifi
```

### Comparing `adafruit-circuitpython-requests-3.2.2/examples/wifi/expanded/requests_wifi_api_github.py` & `adafruit-circuitpython-requests-3.2.3/examples/wifi/expanded/requests_wifi_api_github.py`

 * *Files 2% similar despite different names*

```diff
@@ -1,12 +1,11 @@
 # SPDX-FileCopyrightText: 2024 DJDevon3
 # SPDX-License-Identifier: MIT
 # Coded for Circuit Python 8.2.x
 """Github API Example"""
-# pylint: disable=import-error
 
 import os
 import time
 
 import adafruit_connection_manager
 import wifi
```

### Comparing `adafruit-circuitpython-requests-3.2.2/examples/wifi/expanded/requests_wifi_api_mastodon.py` & `adafruit-circuitpython-requests-3.2.3/examples/wifi/expanded/requests_wifi_api_mastodon.py`

 * *Files 2% similar despite different names*

```diff
@@ -1,12 +1,11 @@
 # SPDX-FileCopyrightText: 2024 DJDevon3
 # SPDX-License-Identifier: MIT
 # Coded for Circuit Python 8.2.x
 """Mastodon API Example"""
-# pylint: disable=import-error
 
 import os
 import time
 
 import adafruit_connection_manager
 import wifi
```

### Comparing `adafruit-circuitpython-requests-3.2.2/examples/wifi/expanded/requests_wifi_api_openskynetwork_private.py` & `adafruit-circuitpython-requests-3.2.3/examples/wifi/expanded/requests_wifi_api_openskynetwork_private.py`

 * *Files identical despite different names*

### Comparing `adafruit-circuitpython-requests-3.2.2/examples/wifi/expanded/requests_wifi_api_openskynetwork_private_area.py` & `adafruit-circuitpython-requests-3.2.3/examples/wifi/expanded/requests_wifi_api_openskynetwork_private_area.py`

 * *Files identical despite different names*

### Comparing `adafruit-circuitpython-requests-3.2.2/examples/wifi/expanded/requests_wifi_api_openskynetwork_public.py` & `adafruit-circuitpython-requests-3.2.3/examples/wifi/expanded/requests_wifi_api_openskynetwork_public.py`

 * *Files identical despite different names*

### Comparing `adafruit-circuitpython-requests-3.2.2/examples/wifi/expanded/requests_wifi_api_premiereleague.py` & `adafruit-circuitpython-requests-3.2.3/examples/wifi/expanded/requests_wifi_api_premiereleague.py`

 * *Files 2% similar despite different names*

```diff
@@ -1,12 +1,11 @@
 # SPDX-FileCopyrightText: 2024 DJDevon3
 # SPDX-License-Identifier: MIT
 # Coded for Circuit Python 8.2.x
 """Premiere League Total Players API Example"""
-# pylint: disable=import-error
 
 import os
 import time
 
 import adafruit_connection_manager
 import adafruit_json_stream as json_stream
 import wifi
```

### Comparing `adafruit-circuitpython-requests-3.2.2/examples/wifi/expanded/requests_wifi_api_rocketlaunch_live.py` & `adafruit-circuitpython-requests-3.2.3/examples/wifi/expanded/requests_wifi_api_youtube.py`

 * *Files 26% similar despite different names*

```diff
@@ -1,125 +1,120 @@
 # SPDX-FileCopyrightText: 2024 DJDevon3
 # SPDX-License-Identifier: MIT
 # Coded for Circuit Python 8.2.x
-"""RocketLaunch.Live API Example"""
+"""YouTube API Subscriber Count Example"""
 
 import os
 import time
 
 import adafruit_connection_manager
 import wifi
 
 import adafruit_requests
 
-# Time between API refreshes
+# Initalize Wifi, Socket Pool, Request Session
+pool = adafruit_connection_manager.get_radio_socketpool(wifi.radio)
+ssl_context = adafruit_connection_manager.get_radio_ssl_context(wifi.radio)
+requests = adafruit_requests.Session(pool, ssl_context)
+
+# API Polling Rate
 # 900 = 15 mins, 1800 = 30 mins, 3600 = 1 hour
-sleep_time = 43200
+SLEEP_TIME = 900
+
+# Set debug to True for full JSON response.
+# WARNING: Will show credentials
+DEBUG = False
+
+# Ensure these are uncommented and in settings.toml
+# YOUTUBE_USERNAME = "Your YouTube Username",
+# YOUTUBE_TOKEN = "Your long API developer token",
 
 # Get WiFi details, ensure these are setup in settings.toml
-ssid = os.getenv("WIFI_SSID")
-password = os.getenv("WIFI_PASSWORD")
+ssid = os.getenv("CIRCUITPY_WIFI_SSID")
+password = os.getenv("CIRCUITPY_WIFI_PASSWORD")
+# Requires YouTube/Google API key
+# https://console.cloud.google.com/apis/dashboard
+YT_USERNAME = os.getenv("YOUTUBE_USERNAME")
+YT_TOKEN = os.getenv("YOUTUBE_TOKEN")
 
 
-# Converts seconds in minutes/hours/days
 def time_calc(input_time):
+    """Converts seconds to minutes/hours/days"""
     if input_time < 60:
-        sleep_int = input_time
-        time_output = f"{sleep_int:.0f} seconds"
-    elif 60 <= input_time < 3600:
-        sleep_int = input_time / 60
-        time_output = f"{sleep_int:.0f} minutes"
-    elif 3600 <= input_time < 86400:
-        sleep_int = input_time / 60 / 60
-        time_output = f"{sleep_int:.0f} hours"
-    elif 86400 <= input_time < 432000:
-        sleep_int = input_time / 60 / 60 / 24
-        time_output = f"{sleep_int:.1f} days"
-    else:  # if > 5 days convert float to int & display whole days
-        sleep_int = input_time / 60 / 60 / 24
-        time_output = f"{sleep_int:.0f} days"
-    return time_output
-
-
-# Publicly available data no header required
-# The number at the end is the amount of launches (max 5 free api)
-ROCKETLAUNCH_SOURCE = "https://fdo.rocketlaunch.live/json/launches/next/1"
+        return f"{input_time:.0f} seconds"
+    if input_time < 3600:
+        return f"{input_time / 60:.0f} minutes"
+    if input_time < 86400:
+        return f"{input_time / 60 / 60:.0f} hours"
+    return f"{input_time / 60 / 60 / 24:.1f} days"
 
-# Initalize Wifi, Socket Pool, Request Session
-pool = adafruit_connection_manager.get_radio_socketpool(wifi.radio)
-ssl_context = adafruit_connection_manager.get_radio_ssl_context(wifi.radio)
-requests = adafruit_requests.Session(pool, ssl_context)
+
+# https://youtube.googleapis.com/youtube/v3/channels?part=statistics&forUsername=[YOUR_USERNAME]&key=[YOUR_API_KEY]
+YOUTUBE_SOURCE = (
+    "https://youtube.googleapis.com/youtube/v3/channels?part=statistics&forUsername="
+    + str(YT_USERNAME)
+    + "&key="
+    + str(YT_TOKEN)
+)
 
 while True:
     # Connect to Wi-Fi
-    print("\n===============================")
-    print("Connecting to WiFi...")
+    print("\nConnecting to WiFi...")
     while not wifi.radio.ipv4_address:
         try:
             wifi.radio.connect(ssid, password)
         except ConnectionError as e:
             print("❌ Connection Error:", e)
             print("Retrying in 10 seconds")
     print("✅ Wifi!")
     try:
-        # Print Request to Serial
-        print(" | Attempting to GET RocketLaunch.Live JSON!")
-        time.sleep(2)
-        debug_rocketlaunch_full_response = False
-
+        print(" | Attempting to GET YouTube JSON...")
         try:
-            rocketlaunch_response = requests.get(url=ROCKETLAUNCH_SOURCE)
-            rocketlaunch_json = rocketlaunch_response.json()
+            youtube_response = requests.get(url=YOUTUBE_SOURCE)
+            youtube_json = youtube_response.json()
         except ConnectionError as e:
             print("Connection Error:", e)
             print("Retrying in 10 seconds")
-        print(" | ✅ RocketLaunch.Live JSON!")
+        print(" | ✅ YouTube JSON!")
+
+        if DEBUG:
+            print(f" | Full API GET URL: {YOUTUBE_SOURCE}")
+            print(f" | Full API Dump: {youtube_json}")
+
+        # Key:Value RESPONSES
+        if "pageInfo" in youtube_json:
+            totalResults = youtube_json["pageInfo"]["totalResults"]
+            print(f" |  | Matching Results: {totalResults}")
+
+        if "items" in youtube_json:
+            YT_request_kind = youtube_json["items"][0]["kind"]
+            print(f" |  | Request Kind: {YT_request_kind}")
+
+            YT_channel_id = youtube_json["items"][0]["id"]
+            print(f" |  | Channel ID: {YT_channel_id}")
+
+            YT_videoCount = youtube_json["items"][0]["statistics"]["videoCount"]
+            print(f" |  | Videos: {YT_videoCount}")
+
+            YT_viewCount = youtube_json["items"][0]["statistics"]["viewCount"]
+            print(f" |  | Views: {YT_viewCount}")
+
+            YT_subsCount = youtube_json["items"][0]["statistics"]["subscriberCount"]
+            print(f" |  | Subscribers: {YT_subsCount}")
+
+        if "kind" in youtube_json:
+            YT_response_kind = youtube_json["kind"]
+            print(f" |  | Response Kind: {YT_response_kind}")
 
-        if debug_rocketlaunch_full_response:
-            print("Full API GET URL: ", ROCKETLAUNCH_SOURCE)
-            print(rocketlaunch_json)
-
-        # JSON Endpoints
-        RLFN = str(rocketlaunch_json["result"][0]["name"])
-        RLWO = str(rocketlaunch_json["result"][0]["win_open"])
-        TMINUS = str(rocketlaunch_json["result"][0]["t0"])
-        RLWC = str(rocketlaunch_json["result"][0]["win_close"])
-        RLP = str(rocketlaunch_json["result"][0]["provider"]["name"])
-        RLVN = str(rocketlaunch_json["result"][0]["vehicle"]["name"])
-        RLPN = str(rocketlaunch_json["result"][0]["pad"]["name"])
-        RLLS = str(rocketlaunch_json["result"][0]["pad"]["location"]["name"])
-        RLLD = str(rocketlaunch_json["result"][0]["launch_description"])
-        RLM = str(rocketlaunch_json["result"][0]["mission_description"])
-        RLDATE = str(rocketlaunch_json["result"][0]["date_str"])
-
-        # Print to serial & display label if endpoint not "None"
-        if RLDATE != "None":
-            print(f" |  | Date: {RLDATE}")
-        if RLFN != "None":
-            print(f" |  | Flight: {RLFN}")
-        if RLP != "None":
-            print(f" |  | Provider: {RLP}")
-        if RLVN != "None":
-            print(f" |  | Vehicle: {RLVN}")
-        if RLWO != "None":
-            print(f" |  | Window: {RLWO} to {RLWC}")
-        elif TMINUS != "None":
-            print(f" |  | Window: {TMINUS} to {RLWC}")
-        if RLLS != "None":
-            print(f" |  | Site: {RLLS}")
-        if RLPN != "None":
-            print(f" |  | Pad: {RLPN}")
-        if RLLD != "None":
-            print(f" |  | Description: {RLLD}")
-        if RLM != "None":
-            print(f" |  | Mission: {RLM}")
+        youtube_response.close()
+        print("✂️ Disconnected from YouTube API")
 
         print("\nFinished!")
-        print("Board Uptime: ", time.monotonic())
-        print("Next Update in: ", time_calc(sleep_time))
+        print(f"Board Uptime: {time_calc(time.monotonic())}")
+        print(f"Next Update: {time_calc(SLEEP_TIME)}")
         print("===============================")
 
     except (ValueError, RuntimeError) as e:
-        print("Failed to get data, retrying\n", e)
+        print(f"Failed to get data, retrying\n {e}")
         time.sleep(60)
         break
-    time.sleep(sleep_time)
+    time.sleep(SLEEP_TIME)
```

### Comparing `adafruit-circuitpython-requests-3.2.2/examples/wifi/expanded/requests_wifi_api_steam.py` & `adafruit-circuitpython-requests-3.2.3/examples/wifi/expanded/requests_wifi_api_steam.py`

 * *Files 2% similar despite different names*

```diff
@@ -1,12 +1,11 @@
 # SPDX-FileCopyrightText: 2024 DJDevon3
 # SPDX-License-Identifier: MIT
 # Coded for Circuit Python 8.2.x
 """Steam API Get Owned Games Example"""
-# pylint: disable=import-error
 
 import os
 import time
 
 import adafruit_connection_manager
 import wifi
```

### Comparing `adafruit-circuitpython-requests-3.2.2/examples/wifi/expanded/requests_wifi_api_twitch.py` & `adafruit-circuitpython-requests-3.2.3/examples/wifi/expanded/requests_wifi_api_twitch.py`

 * *Files 2% similar despite different names*

```diff
@@ -1,12 +1,11 @@
 # SPDX-FileCopyrightText: 2024 DJDevon3
 # SPDX-License-Identifier: MIT
 # Coded for Circuit Python 8.2.x
 """Twitch API Example"""
-# pylint: disable=import-error
 
 import os
 import time
 
 import adafruit_connection_manager
 import wifi
```

### Comparing `adafruit-circuitpython-requests-3.2.2/examples/wifi/expanded/requests_wifi_api_twitter.py` & `adafruit-circuitpython-requests-3.2.3/examples/wifi/expanded/requests_wifi_api_twitter.py`

 * *Files identical despite different names*

### Comparing `adafruit-circuitpython-requests-3.2.2/examples/wifi/expanded/requests_wifi_multiple_cookies.py` & `adafruit-circuitpython-requests-3.2.3/examples/wifi/expanded/requests_wifi_multiple_cookies.py`

 * *Files identical despite different names*

### Comparing `adafruit-circuitpython-requests-3.2.2/examples/wifi/requests_wifi_advanced.py` & `adafruit-circuitpython-requests-3.2.3/examples/wifi/requests_wifi_advanced.py`

 * *Files identical despite different names*

### Comparing `adafruit-circuitpython-requests-3.2.2/examples/wifi/requests_wifi_simpletest.py` & `adafruit-circuitpython-requests-3.2.3/examples/wifi/requests_wifi_simpletest.py`

 * *Files identical despite different names*

### Comparing `adafruit-circuitpython-requests-3.2.2/examples/wiznet5k/requests_wiznet5k_advanced.py` & `adafruit-circuitpython-requests-3.2.3/examples/wiznet5k/requests_wiznet5k_advanced.py`

 * *Files identical despite different names*

### Comparing `adafruit-circuitpython-requests-3.2.2/examples/wiznet5k/requests_wiznet5k_simpletest.py` & `adafruit-circuitpython-requests-3.2.3/examples/wiznet5k/requests_wiznet5k_simpletest.py`

 * *Files identical despite different names*

### Comparing `adafruit-circuitpython-requests-3.2.2/pyproject.toml` & `adafruit-circuitpython-requests-3.2.3/pyproject.toml`

 * *Files 1% similar despite different names*

```diff
@@ -8,15 +8,15 @@
     "wheel",
     "setuptools-scm",
 ]
 
 [project]
 name = "adafruit-circuitpython-requests"
 description = "A requests-like library for web interfacing"
-version = "3.2.2"
+version = "3.2.3"
 readme = "README.rst"
 authors = [
     {name = "Adafruit Industries", email = "circuitpython@adafruit.com"}
 ]
 urls = {Homepage = "https://github.com/adafruit/Adafruit_CircuitPython_Requests"}
 keywords = [
     "adafruit",
```

### Comparing `adafruit-circuitpython-requests-3.2.2/tests/chunk_test.py` & `adafruit-circuitpython-requests-3.2.3/tests/chunk_test.py`

 * *Files identical despite different names*

### Comparing `adafruit-circuitpython-requests-3.2.2/tests/chunked_redirect_test.py` & `adafruit-circuitpython-requests-3.2.3/tests/chunked_redirect_test.py`

 * *Files identical despite different names*

### Comparing `adafruit-circuitpython-requests-3.2.2/tests/concurrent_test.py` & `adafruit-circuitpython-requests-3.2.3/tests/concurrent_test.py`

 * *Files identical despite different names*

### Comparing `adafruit-circuitpython-requests-3.2.2/tests/conftest.py` & `adafruit-circuitpython-requests-3.2.3/tests/conftest.py`

 * *Files identical despite different names*

### Comparing `adafruit-circuitpython-requests-3.2.2/tests/header_test.py` & `adafruit-circuitpython-requests-3.2.3/tests/header_test.py`

 * *Files identical despite different names*

### Comparing `adafruit-circuitpython-requests-3.2.2/tests/method_test.py` & `adafruit-circuitpython-requests-3.2.3/tests/method_test.py`

 * *Files identical despite different names*

### Comparing `adafruit-circuitpython-requests-3.2.2/tests/mocket.py` & `adafruit-circuitpython-requests-3.2.3/tests/mocket.py`

 * *Files identical despite different names*

### Comparing `adafruit-circuitpython-requests-3.2.2/tests/parse_test.py` & `adafruit-circuitpython-requests-3.2.3/tests/parse_test.py`

 * *Files identical despite different names*

### Comparing `adafruit-circuitpython-requests-3.2.2/tests/protocol_test.py` & `adafruit-circuitpython-requests-3.2.3/tests/protocol_test.py`

 * *Files identical despite different names*

### Comparing `adafruit-circuitpython-requests-3.2.2/tests/reuse_test.py` & `adafruit-circuitpython-requests-3.2.3/tests/reuse_test.py`

 * *Files identical despite different names*

### Comparing `adafruit-circuitpython-requests-3.2.2/tox.ini` & `adafruit-circuitpython-requests-3.2.3/tox.ini`

 * *Files identical despite different names*

